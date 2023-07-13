# Comparing `tmp/mypy-boto3-s3-1.28.0.tar.gz` & `tmp/mypy-boto3-s3-1.28.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-s3-1.28.0.tar", last modified: Thu Jul  6 21:00:30 2023, max compression
+gzip compressed data, was "mypy-boto3-s3-1.28.2.tar", last modified: Thu Jul 13 18:56:47 2023, max compression
```

## Comparing `mypy-boto3-s3-1.28.0.tar` & `mypy-boto3-s3-1.28.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:30.014416 mypy-boto3-s3-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:53:53.000000 mypy-boto3-s3-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    34064 2023-07-06 21:00:30.010415 mypy-boto3-s3-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    32599 2023-07-06 20:53:53.000000 mypy-boto3-s3-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:30.010415 mypy-boto3-s3-1.28.0/mypy_boto3_s3/
--rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-07-06 20:53:53.000000 mypy-boto3-s3-1.28.0/mypy_boto3_s3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-07-06 20:53:53.000000 mypy-boto3-s3-1.28.0/mypy_boto3_s3/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-07-06 20:53:53.000000 mypy-boto3-s3-1.28.0/mypy_boto3_s3/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    83859 2023-07-06 20:53:54.000000 mypy-boto3-s3-1.28.0/mypy_boto3_s3/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    83740 2023-07-06 20:53:54.000000 mypy-boto3-s3-1.28.0/mypy_boto3_s3/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    16518 2023-07-06 20:53:56.000000 mypy-boto3-s3-1.28.0/mypy_boto3_s3/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    16516 2023-07-06 20:53:56.000000 mypy-boto3-s3-1.28.0/mypy_boto3_s3/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7326 2023-07-06 20:53:56.000000 mypy-boto3-s3-1.28.0/mypy_boto3_s3/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7318 2023-07-06 20:53:56.000000 mypy-boto3-s3-1.28.0/mypy_boto3_s3/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:53:53.000000 mypy-boto3-s3-1.28.0/mypy_boto3_s3/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   117751 2023-07-06 20:53:55.000000 mypy-boto3-s3-1.28.0/mypy_boto3_s3/service_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)   117535 2023-07-06 20:53:55.000000 mypy-boto3-s3-1.28.0/mypy_boto3_s3/service_resource.pyi
--rw-r--r--   0 runner    (1001) docker     (123)   185102 2023-07-06 20:54:04.000000 mypy-boto3-s3-1.28.0/mypy_boto3_s3/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   184790 2023-07-06 20:54:02.000000 mypy-boto3-s3-1.28.0/mypy_boto3_s3/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:53:53.000000 mypy-boto3-s3-1.28.0/mypy_boto3_s3/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     5328 2023-07-06 20:53:56.000000 mypy-boto3-s3-1.28.0/mypy_boto3_s3/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5323 2023-07-06 20:53:56.000000 mypy-boto3-s3-1.28.0/mypy_boto3_s3/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:30.010415 mypy-boto3-s3-1.28.0/mypy_boto3_s3.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    34064 2023-07-06 21:00:29.000000 mypy-boto3-s3-1.28.0/mypy_boto3_s3.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-07-06 21:00:29.000000 mypy-boto3-s3-1.28.0/mypy_boto3_s3.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:29.000000 mypy-boto3-s3-1.28.0/mypy_boto3_s3.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:29.000000 mypy-boto3-s3-1.28.0/mypy_boto3_s3.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 21:00:29.000000 mypy-boto3-s3-1.28.0/mypy_boto3_s3.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-06 21:00:29.000000 mypy-boto3-s3-1.28.0/mypy_boto3_s3.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 21:00:30.014416 mypy-boto3-s3-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1948 2023-07-06 20:53:53.000000 mypy-boto3-s3-1.28.0/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-07-13 18:56:47.546654 mypy-boto3-s3-1.28.2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-07-13 18:55:30.000000 mypy-boto3-s3-1.28.2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    34064 2023-07-13 18:56:47.546654 mypy-boto3-s3-1.28.2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    32599 2023-07-13 18:55:30.000000 mypy-boto3-s3-1.28.2/README.md
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-07-13 18:56:47.546654 mypy-boto3-s3-1.28.2/mypy_boto3_s3/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2283 2023-07-13 18:55:30.000000 mypy-boto3-s3-1.28.2/mypy_boto3_s3/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2281 2023-07-13 18:55:30.000000 mypy-boto3-s3-1.28.2/mypy_boto3_s3/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      884 2023-07-13 18:55:30.000000 mypy-boto3-s3-1.28.2/mypy_boto3_s3/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    83859 2023-07-13 18:55:31.000000 mypy-boto3-s3-1.28.2/mypy_boto3_s3/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    83740 2023-07-13 18:55:30.000000 mypy-boto3-s3-1.28.2/mypy_boto3_s3/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    16518 2023-07-13 18:55:33.000000 mypy-boto3-s3-1.28.2/mypy_boto3_s3/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    16516 2023-07-13 18:55:33.000000 mypy-boto3-s3-1.28.2/mypy_boto3_s3/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     7316 2023-07-13 18:55:32.000000 mypy-boto3-s3-1.28.2/mypy_boto3_s3/paginator.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     7308 2023-07-13 18:55:32.000000 mypy-boto3-s3-1.28.2/mypy_boto3_s3/paginator.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-07-13 18:55:30.000000 mypy-boto3-s3-1.28.2/mypy_boto3_s3/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)   117751 2023-07-13 18:55:32.000000 mypy-boto3-s3-1.28.2/mypy_boto3_s3/service_resource.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)   117535 2023-07-13 18:55:31.000000 mypy-boto3-s3-1.28.2/mypy_boto3_s3/service_resource.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)   178786 2023-07-13 18:55:36.000000 mypy-boto3-s3-1.28.2/mypy_boto3_s3/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)   178514 2023-07-13 18:55:34.000000 mypy-boto3-s3-1.28.2/mypy_boto3_s3/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       60 2023-07-13 18:55:30.000000 mypy-boto3-s3-1.28.2/mypy_boto3_s3/version.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     5328 2023-07-13 18:55:32.000000 mypy-boto3-s3-1.28.2/mypy_boto3_s3/waiter.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     5323 2023-07-13 18:55:32.000000 mypy-boto3-s3-1.28.2/mypy_boto3_s3/waiter.pyi
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-07-13 18:56:47.546654 mypy-boto3-s3-1.28.2/mypy_boto3_s3.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    34064 2023-07-13 18:56:47.000000 mypy-boto3-s3-1.28.2/mypy_boto3_s3.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      703 2023-07-13 18:56:47.000000 mypy-boto3-s3-1.28.2/mypy_boto3_s3.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-07-13 18:56:47.000000 mypy-boto3-s3-1.28.2/mypy_boto3_s3.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-07-13 18:56:47.000000 mypy-boto3-s3-1.28.2/mypy_boto3_s3.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-07-13 18:56:47.000000 mypy-boto3-s3-1.28.2/mypy_boto3_s3.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       14 2023-07-13 18:56:47.000000 mypy-boto3-s3-1.28.2/mypy_boto3_s3.egg-info/top_level.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-07-13 18:56:47.546654 mypy-boto3-s3-1.28.2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1948 2023-07-13 18:55:30.000000 mypy-boto3-s3-1.28.2/setup.py
```

### Comparing `mypy-boto3-s3-1.28.0/LICENSE` & `mypy-boto3-s3-1.28.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-s3-1.28.0/PKG-INFO` & `mypy-boto3-s3-1.28.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-s3
-Version: 1.28.0
-Summary: Type annotations for boto3.S3 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.2
+Summary: Type annotations for boto3.S3 1.28.2 service generated with mypy-boto3-builder 7.14.6
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-s3.svg?color=blue)](https://pypi.org/project/mypy-boto3-s3)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-s3?color=blue)](https://pypistats.org/packages/mypy-boto3-s3)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.S3 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3)
+[boto3.S3 1.28.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3)
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
 [mypy-boto3-s3 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/).
 
 See how it helps to find and fix potential bugs:
 
@@ -552,15 +552,15 @@
 
 `mypy_boto3_s3.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_s3.type_defs import (
     AbortIncompleteMultipartUploadTypeDef,
-    AbortMultipartUploadOutputTypeDef,
+    ResponseMetadataTypeDef,
     AbortMultipartUploadRequestMultipartUploadAbortTypeDef,
     AbortMultipartUploadRequestRequestTypeDef,
     AccelerateConfigurationTypeDef,
     OwnerTypeDef,
     AccessControlTranslationTypeDef,
     TagTypeDef,
     AnalyticsS3BucketDestinationTypeDef,
@@ -577,24 +577,21 @@
     ClientDownloadFileRequestTypeDef,
     ClientDownloadFileobjRequestTypeDef,
     ClientGeneratePresignedPostRequestTypeDef,
     ClientUploadFileRequestTypeDef,
     ClientUploadFileobjRequestTypeDef,
     CloudFunctionConfigurationTypeDef,
     CommonPrefixTypeDef,
-    CompleteMultipartUploadOutputTypeDef,
     CompletedPartTypeDef,
     ConditionTypeDef,
     CopyObjectResultTypeDef,
     CopyObjectRequestObjectCopyFromTypeDef,
     CopyObjectRequestObjectSummaryCopyFromTypeDef,
     CopyPartResultTypeDef,
     CreateBucketConfigurationTypeDef,
-    CreateBucketOutputTypeDef,
-    CreateMultipartUploadOutputTypeDef,
     CreateMultipartUploadRequestObjectInitiateMultipartUploadTypeDef,
     CreateMultipartUploadRequestObjectSummaryInitiateMultipartUploadTypeDef,
     CreateMultipartUploadRequestRequestTypeDef,
     DefaultRetentionTypeDef,
     DeleteBucketAnalyticsConfigurationRequestRequestTypeDef,
     DeleteBucketCorsRequestBucketCorsDeleteTypeDef,
     DeleteBucketCorsRequestRequestTypeDef,
@@ -612,88 +609,74 @@
     DeleteBucketRequestBucketDeleteTypeDef,
     DeleteBucketRequestRequestTypeDef,
     DeleteBucketTaggingRequestBucketTaggingDeleteTypeDef,
     DeleteBucketTaggingRequestRequestTypeDef,
     DeleteBucketWebsiteRequestBucketWebsiteDeleteTypeDef,
     DeleteBucketWebsiteRequestRequestTypeDef,
     DeleteMarkerReplicationTypeDef,
-    DeleteObjectOutputTypeDef,
     DeleteObjectRequestObjectDeleteTypeDef,
     DeleteObjectRequestObjectSummaryDeleteTypeDef,
     DeleteObjectRequestObjectVersionDeleteTypeDef,
     DeleteObjectRequestRequestTypeDef,
-    DeleteObjectTaggingOutputTypeDef,
     DeleteObjectTaggingRequestRequestTypeDef,
     DeletedObjectTypeDef,
     ErrorTypeDef,
     DeletePublicAccessBlockRequestRequestTypeDef,
     ObjectIdentifierTypeDef,
     EncryptionConfigurationTypeDef,
-    EmptyResponseMetadataTypeDef,
     EncryptionTypeDef,
-    ErrorDocumentResponseMetadataTypeDef,
     ErrorDocumentTypeDef,
     ExistingObjectReplicationTypeDef,
     FilterRuleTypeDef,
-    GetBucketAccelerateConfigurationOutputTypeDef,
     GetBucketAccelerateConfigurationRequestRequestTypeDef,
     GetBucketAclRequestRequestTypeDef,
     GetBucketAnalyticsConfigurationRequestRequestTypeDef,
     GetBucketCorsRequestRequestTypeDef,
     GetBucketEncryptionRequestRequestTypeDef,
     GetBucketIntelligentTieringConfigurationRequestRequestTypeDef,
     GetBucketInventoryConfigurationRequestRequestTypeDef,
     GetBucketLifecycleConfigurationRequestRequestTypeDef,
     GetBucketLifecycleRequestRequestTypeDef,
-    GetBucketLocationOutputTypeDef,
     GetBucketLocationRequestRequestTypeDef,
     GetBucketLoggingRequestRequestTypeDef,
     GetBucketMetricsConfigurationRequestRequestTypeDef,
     GetBucketNotificationConfigurationRequestRequestTypeDef,
     GetBucketOwnershipControlsRequestRequestTypeDef,
-    GetBucketPolicyOutputTypeDef,
     GetBucketPolicyRequestRequestTypeDef,
     PolicyStatusTypeDef,
     GetBucketPolicyStatusRequestRequestTypeDef,
     GetBucketReplicationRequestRequestTypeDef,
-    GetBucketRequestPaymentOutputTypeDef,
     GetBucketRequestPaymentRequestRequestTypeDef,
     GetBucketTaggingRequestRequestTypeDef,
-    GetBucketVersioningOutputTypeDef,
     GetBucketVersioningRequestRequestTypeDef,
     IndexDocumentTypeDef,
     RedirectAllRequestsToTypeDef,
     GetBucketWebsiteRequestRequestTypeDef,
     GetObjectAclRequestRequestTypeDef,
     ObjectPartTypeDef,
     GetObjectAttributesRequestRequestTypeDef,
     ObjectLockLegalHoldTypeDef,
     GetObjectLegalHoldRequestRequestTypeDef,
     GetObjectLockConfigurationRequestRequestTypeDef,
-    GetObjectOutputTypeDef,
     GetObjectRequestObjectGetTypeDef,
     GetObjectRequestObjectSummaryGetTypeDef,
     GetObjectRequestObjectVersionGetTypeDef,
     GetObjectRequestRequestTypeDef,
     ObjectLockRetentionTypeDef,
     GetObjectRetentionRequestRequestTypeDef,
     GetObjectTaggingRequestRequestTypeDef,
-    GetObjectTorrentOutputTypeDef,
     GetObjectTorrentRequestRequestTypeDef,
     PublicAccessBlockConfigurationTypeDef,
     GetPublicAccessBlockRequestRequestTypeDef,
     GlacierJobParametersTypeDef,
     GranteeTypeDef,
     WaiterConfigTypeDef,
     HeadBucketRequestRequestTypeDef,
-    HeadObjectOutputTypeDef,
     HeadObjectRequestObjectVersionHeadTypeDef,
     HeadObjectRequestRequestTypeDef,
-    IndexDocumentResponseMetadataTypeDef,
-    InitiatorResponseMetadataTypeDef,
     InitiatorTypeDef,
     JSONInputTypeDef,
     TieringTypeDef,
     InventoryFilterTypeDef,
     InventoryScheduleTypeDef,
     SSEKMSTypeDef,
     JSONOutputTypeDef,
@@ -701,70 +684,82 @@
     NoncurrentVersionExpirationTypeDef,
     NoncurrentVersionTransitionTypeDef,
     TransitionTypeDef,
     ListBucketAnalyticsConfigurationsRequestRequestTypeDef,
     ListBucketIntelligentTieringConfigurationsRequestRequestTypeDef,
     ListBucketInventoryConfigurationsRequestRequestTypeDef,
     ListBucketMetricsConfigurationsRequestRequestTypeDef,
-    ListMultipartUploadsRequestListMultipartUploadsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListMultipartUploadsRequestRequestTypeDef,
-    ListObjectVersionsRequestListObjectVersionsPaginateTypeDef,
     ListObjectVersionsRequestRequestTypeDef,
-    ListObjectsRequestListObjectsPaginateTypeDef,
     ListObjectsRequestRequestTypeDef,
-    ListObjectsV2RequestListObjectsV2PaginateTypeDef,
     ListObjectsV2RequestRequestTypeDef,
     PartTypeDef,
-    ListPartsRequestListPartsPaginateTypeDef,
     ListPartsRequestRequestTypeDef,
     MetadataEntryTypeDef,
     ReplicationTimeValueTypeDef,
     QueueConfigurationDeprecatedTypeDef,
     TopicConfigurationDeprecatedTypeDef,
     ObjectDownloadFileRequestTypeDef,
     ObjectDownloadFileobjRequestTypeDef,
     RestoreStatusTypeDef,
     ObjectUploadFileRequestTypeDef,
     ObjectUploadFileobjRequestTypeDef,
-    OwnerResponseMetadataTypeDef,
     OwnershipControlsRuleTypeDef,
-    PaginatorConfigTypeDef,
     ProgressTypeDef,
     PutBucketPolicyRequestBucketPolicyPutTypeDef,
     PutBucketPolicyRequestRequestTypeDef,
     RequestPaymentConfigurationTypeDef,
     PutBucketVersioningRequestBucketVersioningEnableTypeDef,
     VersioningConfigurationTypeDef,
     PutBucketVersioningRequestBucketVersioningSuspendTypeDef,
-    PutObjectAclOutputTypeDef,
-    PutObjectLegalHoldOutputTypeDef,
-    PutObjectLockConfigurationOutputTypeDef,
-    PutObjectOutputTypeDef,
     PutObjectRequestBucketPutObjectTypeDef,
     PutObjectRequestObjectPutTypeDef,
     PutObjectRequestObjectSummaryPutTypeDef,
     PutObjectRequestRequestTypeDef,
-    PutObjectRetentionOutputTypeDef,
-    PutObjectTaggingOutputTypeDef,
     RecordsEventTypeDef,
-    RedirectAllRequestsToResponseMetadataTypeDef,
     RedirectTypeDef,
     ReplicaModificationsTypeDef,
     RequestProgressTypeDef,
-    ResponseMetadataTypeDef,
-    RestoreObjectOutputTypeDef,
-    RestoreStatusResponseMetadataTypeDef,
     ScanRangeTypeDef,
     ServerSideEncryptionByDefaultTypeDef,
     SseKmsEncryptedObjectsTypeDef,
     StatsTypeDef,
-    UploadPartOutputTypeDef,
     UploadPartRequestMultipartUploadPartUploadTypeDef,
     UploadPartRequestRequestTypeDef,
     WriteGetObjectResponseRequestRequestTypeDef,
+    AbortMultipartUploadOutputTypeDef,
+    CompleteMultipartUploadOutputTypeDef,
+    CreateBucketOutputTypeDef,
+    CreateMultipartUploadOutputTypeDef,
+    DeleteObjectOutputTypeDef,
+    DeleteObjectTaggingOutputTypeDef,
+    EmptyResponseMetadataTypeDef,
+    ErrorDocumentResponseMetadataTypeDef,
+    GetBucketAccelerateConfigurationOutputTypeDef,
+    GetBucketLocationOutputTypeDef,
+    GetBucketPolicyOutputTypeDef,
+    GetBucketRequestPaymentOutputTypeDef,
+    GetBucketVersioningOutputTypeDef,
+    GetObjectOutputTypeDef,
+    GetObjectTorrentOutputTypeDef,
+    HeadObjectOutputTypeDef,
+    IndexDocumentResponseMetadataTypeDef,
+    InitiatorResponseMetadataTypeDef,
+    OwnerResponseMetadataTypeDef,
+    PutObjectAclOutputTypeDef,
+    PutObjectLegalHoldOutputTypeDef,
+    PutObjectLockConfigurationOutputTypeDef,
+    PutObjectOutputTypeDef,
+    PutObjectRetentionOutputTypeDef,
+    PutObjectTaggingOutputTypeDef,
+    RedirectAllRequestsToResponseMetadataTypeDef,
+    RestoreObjectOutputTypeDef,
+    RestoreStatusResponseMetadataTypeDef,
+    UploadPartOutputTypeDef,
     PutBucketAccelerateConfigurationRequestRequestTypeDef,
     DeleteMarkerEntryTypeDef,
     AnalyticsAndOperatorTypeDef,
     GetBucketTaggingOutputTypeDef,
     GetObjectTaggingOutputTypeDef,
     IntelligentTieringAndOperatorTypeDef,
     LifecycleRuleAndOperatorTypeDef,
@@ -806,14 +801,19 @@
     HeadObjectRequestObjectExistsWaitTypeDef,
     HeadObjectRequestObjectNotExistsWaitTypeDef,
     MultipartUploadTypeDef,
     InputSerializationTypeDef,
     InventoryEncryptionTypeDef,
     OutputSerializationTypeDef,
     RuleTypeDef,
+    ListMultipartUploadsRequestListMultipartUploadsPaginateTypeDef,
+    ListObjectVersionsRequestListObjectVersionsPaginateTypeDef,
+    ListObjectsRequestListObjectsPaginateTypeDef,
+    ListObjectsV2RequestListObjectsV2PaginateTypeDef,
+    ListPartsRequestListPartsPaginateTypeDef,
     ListPartsOutputTypeDef,
     MetricsTypeDef,
     ReplicationTimeTypeDef,
     NotificationConfigurationDeprecatedResponseMetadataTypeDef,
     NotificationConfigurationDeprecatedTypeDef,
     ObjectTypeDef,
     ObjectVersionTypeDef,
```

### Comparing `mypy-boto3-s3-1.28.0/README.md` & `mypy-boto3-s3-1.28.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-s3.svg?color=blue)](https://pypi.org/project/mypy-boto3-s3)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-s3?color=blue)](https://pypistats.org/packages/mypy-boto3-s3)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.S3 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3)
+[boto3.S3 1.28.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3)
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
 [mypy-boto3-s3 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/).
 
 See how it helps to find and fix potential bugs:
 
@@ -520,15 +520,15 @@
 
 `mypy_boto3_s3.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_s3.type_defs import (
     AbortIncompleteMultipartUploadTypeDef,
-    AbortMultipartUploadOutputTypeDef,
+    ResponseMetadataTypeDef,
     AbortMultipartUploadRequestMultipartUploadAbortTypeDef,
     AbortMultipartUploadRequestRequestTypeDef,
     AccelerateConfigurationTypeDef,
     OwnerTypeDef,
     AccessControlTranslationTypeDef,
     TagTypeDef,
     AnalyticsS3BucketDestinationTypeDef,
@@ -545,24 +545,21 @@
     ClientDownloadFileRequestTypeDef,
     ClientDownloadFileobjRequestTypeDef,
     ClientGeneratePresignedPostRequestTypeDef,
     ClientUploadFileRequestTypeDef,
     ClientUploadFileobjRequestTypeDef,
     CloudFunctionConfigurationTypeDef,
     CommonPrefixTypeDef,
-    CompleteMultipartUploadOutputTypeDef,
     CompletedPartTypeDef,
     ConditionTypeDef,
     CopyObjectResultTypeDef,
     CopyObjectRequestObjectCopyFromTypeDef,
     CopyObjectRequestObjectSummaryCopyFromTypeDef,
     CopyPartResultTypeDef,
     CreateBucketConfigurationTypeDef,
-    CreateBucketOutputTypeDef,
-    CreateMultipartUploadOutputTypeDef,
     CreateMultipartUploadRequestObjectInitiateMultipartUploadTypeDef,
     CreateMultipartUploadRequestObjectSummaryInitiateMultipartUploadTypeDef,
     CreateMultipartUploadRequestRequestTypeDef,
     DefaultRetentionTypeDef,
     DeleteBucketAnalyticsConfigurationRequestRequestTypeDef,
     DeleteBucketCorsRequestBucketCorsDeleteTypeDef,
     DeleteBucketCorsRequestRequestTypeDef,
@@ -580,88 +577,74 @@
     DeleteBucketRequestBucketDeleteTypeDef,
     DeleteBucketRequestRequestTypeDef,
     DeleteBucketTaggingRequestBucketTaggingDeleteTypeDef,
     DeleteBucketTaggingRequestRequestTypeDef,
     DeleteBucketWebsiteRequestBucketWebsiteDeleteTypeDef,
     DeleteBucketWebsiteRequestRequestTypeDef,
     DeleteMarkerReplicationTypeDef,
-    DeleteObjectOutputTypeDef,
     DeleteObjectRequestObjectDeleteTypeDef,
     DeleteObjectRequestObjectSummaryDeleteTypeDef,
     DeleteObjectRequestObjectVersionDeleteTypeDef,
     DeleteObjectRequestRequestTypeDef,
-    DeleteObjectTaggingOutputTypeDef,
     DeleteObjectTaggingRequestRequestTypeDef,
     DeletedObjectTypeDef,
     ErrorTypeDef,
     DeletePublicAccessBlockRequestRequestTypeDef,
     ObjectIdentifierTypeDef,
     EncryptionConfigurationTypeDef,
-    EmptyResponseMetadataTypeDef,
     EncryptionTypeDef,
-    ErrorDocumentResponseMetadataTypeDef,
     ErrorDocumentTypeDef,
     ExistingObjectReplicationTypeDef,
     FilterRuleTypeDef,
-    GetBucketAccelerateConfigurationOutputTypeDef,
     GetBucketAccelerateConfigurationRequestRequestTypeDef,
     GetBucketAclRequestRequestTypeDef,
     GetBucketAnalyticsConfigurationRequestRequestTypeDef,
     GetBucketCorsRequestRequestTypeDef,
     GetBucketEncryptionRequestRequestTypeDef,
     GetBucketIntelligentTieringConfigurationRequestRequestTypeDef,
     GetBucketInventoryConfigurationRequestRequestTypeDef,
     GetBucketLifecycleConfigurationRequestRequestTypeDef,
     GetBucketLifecycleRequestRequestTypeDef,
-    GetBucketLocationOutputTypeDef,
     GetBucketLocationRequestRequestTypeDef,
     GetBucketLoggingRequestRequestTypeDef,
     GetBucketMetricsConfigurationRequestRequestTypeDef,
     GetBucketNotificationConfigurationRequestRequestTypeDef,
     GetBucketOwnershipControlsRequestRequestTypeDef,
-    GetBucketPolicyOutputTypeDef,
     GetBucketPolicyRequestRequestTypeDef,
     PolicyStatusTypeDef,
     GetBucketPolicyStatusRequestRequestTypeDef,
     GetBucketReplicationRequestRequestTypeDef,
-    GetBucketRequestPaymentOutputTypeDef,
     GetBucketRequestPaymentRequestRequestTypeDef,
     GetBucketTaggingRequestRequestTypeDef,
-    GetBucketVersioningOutputTypeDef,
     GetBucketVersioningRequestRequestTypeDef,
     IndexDocumentTypeDef,
     RedirectAllRequestsToTypeDef,
     GetBucketWebsiteRequestRequestTypeDef,
     GetObjectAclRequestRequestTypeDef,
     ObjectPartTypeDef,
     GetObjectAttributesRequestRequestTypeDef,
     ObjectLockLegalHoldTypeDef,
     GetObjectLegalHoldRequestRequestTypeDef,
     GetObjectLockConfigurationRequestRequestTypeDef,
-    GetObjectOutputTypeDef,
     GetObjectRequestObjectGetTypeDef,
     GetObjectRequestObjectSummaryGetTypeDef,
     GetObjectRequestObjectVersionGetTypeDef,
     GetObjectRequestRequestTypeDef,
     ObjectLockRetentionTypeDef,
     GetObjectRetentionRequestRequestTypeDef,
     GetObjectTaggingRequestRequestTypeDef,
-    GetObjectTorrentOutputTypeDef,
     GetObjectTorrentRequestRequestTypeDef,
     PublicAccessBlockConfigurationTypeDef,
     GetPublicAccessBlockRequestRequestTypeDef,
     GlacierJobParametersTypeDef,
     GranteeTypeDef,
     WaiterConfigTypeDef,
     HeadBucketRequestRequestTypeDef,
-    HeadObjectOutputTypeDef,
     HeadObjectRequestObjectVersionHeadTypeDef,
     HeadObjectRequestRequestTypeDef,
-    IndexDocumentResponseMetadataTypeDef,
-    InitiatorResponseMetadataTypeDef,
     InitiatorTypeDef,
     JSONInputTypeDef,
     TieringTypeDef,
     InventoryFilterTypeDef,
     InventoryScheduleTypeDef,
     SSEKMSTypeDef,
     JSONOutputTypeDef,
@@ -669,70 +652,82 @@
     NoncurrentVersionExpirationTypeDef,
     NoncurrentVersionTransitionTypeDef,
     TransitionTypeDef,
     ListBucketAnalyticsConfigurationsRequestRequestTypeDef,
     ListBucketIntelligentTieringConfigurationsRequestRequestTypeDef,
     ListBucketInventoryConfigurationsRequestRequestTypeDef,
     ListBucketMetricsConfigurationsRequestRequestTypeDef,
-    ListMultipartUploadsRequestListMultipartUploadsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListMultipartUploadsRequestRequestTypeDef,
-    ListObjectVersionsRequestListObjectVersionsPaginateTypeDef,
     ListObjectVersionsRequestRequestTypeDef,
-    ListObjectsRequestListObjectsPaginateTypeDef,
     ListObjectsRequestRequestTypeDef,
-    ListObjectsV2RequestListObjectsV2PaginateTypeDef,
     ListObjectsV2RequestRequestTypeDef,
     PartTypeDef,
-    ListPartsRequestListPartsPaginateTypeDef,
     ListPartsRequestRequestTypeDef,
     MetadataEntryTypeDef,
     ReplicationTimeValueTypeDef,
     QueueConfigurationDeprecatedTypeDef,
     TopicConfigurationDeprecatedTypeDef,
     ObjectDownloadFileRequestTypeDef,
     ObjectDownloadFileobjRequestTypeDef,
     RestoreStatusTypeDef,
     ObjectUploadFileRequestTypeDef,
     ObjectUploadFileobjRequestTypeDef,
-    OwnerResponseMetadataTypeDef,
     OwnershipControlsRuleTypeDef,
-    PaginatorConfigTypeDef,
     ProgressTypeDef,
     PutBucketPolicyRequestBucketPolicyPutTypeDef,
     PutBucketPolicyRequestRequestTypeDef,
     RequestPaymentConfigurationTypeDef,
     PutBucketVersioningRequestBucketVersioningEnableTypeDef,
     VersioningConfigurationTypeDef,
     PutBucketVersioningRequestBucketVersioningSuspendTypeDef,
-    PutObjectAclOutputTypeDef,
-    PutObjectLegalHoldOutputTypeDef,
-    PutObjectLockConfigurationOutputTypeDef,
-    PutObjectOutputTypeDef,
     PutObjectRequestBucketPutObjectTypeDef,
     PutObjectRequestObjectPutTypeDef,
     PutObjectRequestObjectSummaryPutTypeDef,
     PutObjectRequestRequestTypeDef,
-    PutObjectRetentionOutputTypeDef,
-    PutObjectTaggingOutputTypeDef,
     RecordsEventTypeDef,
-    RedirectAllRequestsToResponseMetadataTypeDef,
     RedirectTypeDef,
     ReplicaModificationsTypeDef,
     RequestProgressTypeDef,
-    ResponseMetadataTypeDef,
-    RestoreObjectOutputTypeDef,
-    RestoreStatusResponseMetadataTypeDef,
     ScanRangeTypeDef,
     ServerSideEncryptionByDefaultTypeDef,
     SseKmsEncryptedObjectsTypeDef,
     StatsTypeDef,
-    UploadPartOutputTypeDef,
     UploadPartRequestMultipartUploadPartUploadTypeDef,
     UploadPartRequestRequestTypeDef,
     WriteGetObjectResponseRequestRequestTypeDef,
+    AbortMultipartUploadOutputTypeDef,
+    CompleteMultipartUploadOutputTypeDef,
+    CreateBucketOutputTypeDef,
+    CreateMultipartUploadOutputTypeDef,
+    DeleteObjectOutputTypeDef,
+    DeleteObjectTaggingOutputTypeDef,
+    EmptyResponseMetadataTypeDef,
+    ErrorDocumentResponseMetadataTypeDef,
+    GetBucketAccelerateConfigurationOutputTypeDef,
+    GetBucketLocationOutputTypeDef,
+    GetBucketPolicyOutputTypeDef,
+    GetBucketRequestPaymentOutputTypeDef,
+    GetBucketVersioningOutputTypeDef,
+    GetObjectOutputTypeDef,
+    GetObjectTorrentOutputTypeDef,
+    HeadObjectOutputTypeDef,
+    IndexDocumentResponseMetadataTypeDef,
+    InitiatorResponseMetadataTypeDef,
+    OwnerResponseMetadataTypeDef,
+    PutObjectAclOutputTypeDef,
+    PutObjectLegalHoldOutputTypeDef,
+    PutObjectLockConfigurationOutputTypeDef,
+    PutObjectOutputTypeDef,
+    PutObjectRetentionOutputTypeDef,
+    PutObjectTaggingOutputTypeDef,
+    RedirectAllRequestsToResponseMetadataTypeDef,
+    RestoreObjectOutputTypeDef,
+    RestoreStatusResponseMetadataTypeDef,
+    UploadPartOutputTypeDef,
     PutBucketAccelerateConfigurationRequestRequestTypeDef,
     DeleteMarkerEntryTypeDef,
     AnalyticsAndOperatorTypeDef,
     GetBucketTaggingOutputTypeDef,
     GetObjectTaggingOutputTypeDef,
     IntelligentTieringAndOperatorTypeDef,
     LifecycleRuleAndOperatorTypeDef,
@@ -774,14 +769,19 @@
     HeadObjectRequestObjectExistsWaitTypeDef,
     HeadObjectRequestObjectNotExistsWaitTypeDef,
     MultipartUploadTypeDef,
     InputSerializationTypeDef,
     InventoryEncryptionTypeDef,
     OutputSerializationTypeDef,
     RuleTypeDef,
+    ListMultipartUploadsRequestListMultipartUploadsPaginateTypeDef,
+    ListObjectVersionsRequestListObjectVersionsPaginateTypeDef,
+    ListObjectsRequestListObjectsPaginateTypeDef,
+    ListObjectsV2RequestListObjectsV2PaginateTypeDef,
+    ListPartsRequestListPartsPaginateTypeDef,
     ListPartsOutputTypeDef,
     MetricsTypeDef,
     ReplicationTimeTypeDef,
     NotificationConfigurationDeprecatedResponseMetadataTypeDef,
     NotificationConfigurationDeprecatedTypeDef,
     ObjectTypeDef,
     ObjectVersionTypeDef,
```

### Comparing `mypy-boto3-s3-1.28.0/mypy_boto3_s3/__init__.py` & `mypy-boto3-s3-1.28.2/mypy_boto3_s3/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-s3-1.28.0/mypy_boto3_s3/__init__.pyi` & `mypy-boto3-s3-1.28.2/mypy_boto3_s3/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-s3-1.28.0/mypy_boto3_s3/__main__.py` & `mypy-boto3-s3-1.28.2/mypy_boto3_s3/__main__.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.S3 1.28.0\nVersion:         1.28.0\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.S3 1.28.2\nVersion:         1.28.2\nBuilder version:"
+        " 7.14.6\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.28.0")
+    print("1.28.2")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-s3-1.28.0/mypy_boto3_s3/client.py` & `mypy-boto3-s3-1.28.2/mypy_boto3_s3/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-s3-1.28.0/mypy_boto3_s3/client.pyi` & `mypy-boto3-s3-1.28.2/mypy_boto3_s3/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-s3-1.28.0/mypy_boto3_s3/literals.py` & `mypy-boto3-s3-1.28.2/mypy_boto3_s3/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-s3-1.28.0/mypy_boto3_s3/literals.pyi` & `mypy-boto3-s3-1.28.2/mypy_boto3_s3/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-s3-1.28.0/mypy_boto3_s3/paginator.py` & `mypy-boto3-s3-1.28.2/mypy_boto3_s3/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,15 +77,15 @@
         *,
         Bucket: str,
         Delimiter: str = ...,
         EncodingType: Literal["url"] = ...,
         Prefix: str = ...,
         ExpectedBucketOwner: str = ...,
         RequestPayer: Literal["requester"] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListMultipartUploadsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Paginator.ListMultipartUploads.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/paginators/#listmultipartuploadspaginator)
         """
 
 
@@ -101,15 +101,15 @@
         Bucket: str,
         Delimiter: str = ...,
         EncodingType: Literal["url"] = ...,
         Prefix: str = ...,
         ExpectedBucketOwner: str = ...,
         RequestPayer: Literal["requester"] = ...,
         OptionalObjectAttributes: Sequence[Literal["RestoreStatus"]] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListObjectVersionsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Paginator.ListObjectVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/paginators/#listobjectversionspaginator)
         """
 
 
@@ -125,15 +125,15 @@
         Bucket: str,
         Delimiter: str = ...,
         EncodingType: Literal["url"] = ...,
         Prefix: str = ...,
         RequestPayer: Literal["requester"] = ...,
         ExpectedBucketOwner: str = ...,
         OptionalObjectAttributes: Sequence[Literal["RestoreStatus"]] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListObjectsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Paginator.ListObjects.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/paginators/#listobjectspaginator)
         """
 
 
@@ -151,15 +151,15 @@
         EncodingType: Literal["url"] = ...,
         Prefix: str = ...,
         FetchOwner: bool = ...,
         StartAfter: str = ...,
         RequestPayer: Literal["requester"] = ...,
         ExpectedBucketOwner: str = ...,
         OptionalObjectAttributes: Sequence[Literal["RestoreStatus"]] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListObjectsV2OutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Paginator.ListObjectsV2.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/paginators/#listobjectsv2paginator)
         """
 
 
@@ -176,13 +176,13 @@
         Key: str,
         UploadId: str,
         RequestPayer: Literal["requester"] = ...,
         ExpectedBucketOwner: str = ...,
         SSECustomerAlgorithm: str = ...,
         SSECustomerKey: str = ...,
         SSECustomerKeyMD5: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListPartsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Paginator.ListParts.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/paginators/#listpartspaginator)
         """
```

### Comparing `mypy-boto3-s3-1.28.0/mypy_boto3_s3/paginator.pyi` & `mypy-boto3-s3-1.28.2/mypy_boto3_s3/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -73,15 +73,15 @@
         *,
         Bucket: str,
         Delimiter: str = ...,
         EncodingType: Literal["url"] = ...,
         Prefix: str = ...,
         ExpectedBucketOwner: str = ...,
         RequestPayer: Literal["requester"] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListMultipartUploadsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Paginator.ListMultipartUploads.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/paginators/#listmultipartuploadspaginator)
         """
 
 class ListObjectVersionsPaginator(Paginator):
@@ -96,15 +96,15 @@
         Bucket: str,
         Delimiter: str = ...,
         EncodingType: Literal["url"] = ...,
         Prefix: str = ...,
         ExpectedBucketOwner: str = ...,
         RequestPayer: Literal["requester"] = ...,
         OptionalObjectAttributes: Sequence[Literal["RestoreStatus"]] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListObjectVersionsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Paginator.ListObjectVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/paginators/#listobjectversionspaginator)
         """
 
 class ListObjectsPaginator(Paginator):
@@ -119,15 +119,15 @@
         Bucket: str,
         Delimiter: str = ...,
         EncodingType: Literal["url"] = ...,
         Prefix: str = ...,
         RequestPayer: Literal["requester"] = ...,
         ExpectedBucketOwner: str = ...,
         OptionalObjectAttributes: Sequence[Literal["RestoreStatus"]] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListObjectsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Paginator.ListObjects.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/paginators/#listobjectspaginator)
         """
 
 class ListObjectsV2Paginator(Paginator):
@@ -144,15 +144,15 @@
         EncodingType: Literal["url"] = ...,
         Prefix: str = ...,
         FetchOwner: bool = ...,
         StartAfter: str = ...,
         RequestPayer: Literal["requester"] = ...,
         ExpectedBucketOwner: str = ...,
         OptionalObjectAttributes: Sequence[Literal["RestoreStatus"]] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListObjectsV2OutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Paginator.ListObjectsV2.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/paginators/#listobjectsv2paginator)
         """
 
 class ListPartsPaginator(Paginator):
@@ -168,13 +168,13 @@
         Key: str,
         UploadId: str,
         RequestPayer: Literal["requester"] = ...,
         ExpectedBucketOwner: str = ...,
         SSECustomerAlgorithm: str = ...,
         SSECustomerKey: str = ...,
         SSECustomerKeyMD5: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListPartsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Paginator.ListParts.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/paginators/#listpartspaginator)
         """
```

### Comparing `mypy-boto3-s3-1.28.0/mypy_boto3_s3/service_resource.py` & `mypy-boto3-s3-1.28.2/mypy_boto3_s3/service_resource.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-s3-1.28.0/mypy_boto3_s3/service_resource.pyi` & `mypy-boto3-s3-1.28.2/mypy_boto3_s3/service_resource.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-s3-1.28.0/mypy_boto3_s3/type_defs.py` & `mypy-boto3-s3-1.28.2/mypy_boto3_s3/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Callable, Dict, List, Mapping, Sequence, Union
 
 from boto3.s3.transfer import TransferConfig
 from botocore.client import BaseClient
+from botocore.eventstream import EventStream
 from botocore.response import StreamingBody
 
 from .literals import (
     ArchiveStatusType,
     BucketAccelerateStatusType,
     BucketCannedACLType,
     BucketLocationConstraintType,
@@ -74,18 +75,17 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AbortIncompleteMultipartUploadTypeDef",
-    "AbortMultipartUploadOutputTypeDef",
+    "ResponseMetadataTypeDef",
     "AbortMultipartUploadRequestMultipartUploadAbortTypeDef",
     "AbortMultipartUploadRequestRequestTypeDef",
     "AccelerateConfigurationTypeDef",
     "OwnerTypeDef",
     "AccessControlTranslationTypeDef",
     "TagTypeDef",
     "AnalyticsS3BucketDestinationTypeDef",
@@ -102,24 +102,21 @@
     "ClientDownloadFileRequestTypeDef",
     "ClientDownloadFileobjRequestTypeDef",
     "ClientGeneratePresignedPostRequestTypeDef",
     "ClientUploadFileRequestTypeDef",
     "ClientUploadFileobjRequestTypeDef",
     "CloudFunctionConfigurationTypeDef",
     "CommonPrefixTypeDef",
-    "CompleteMultipartUploadOutputTypeDef",
     "CompletedPartTypeDef",
     "ConditionTypeDef",
     "CopyObjectResultTypeDef",
     "CopyObjectRequestObjectCopyFromTypeDef",
     "CopyObjectRequestObjectSummaryCopyFromTypeDef",
     "CopyPartResultTypeDef",
     "CreateBucketConfigurationTypeDef",
-    "CreateBucketOutputTypeDef",
-    "CreateMultipartUploadOutputTypeDef",
     "CreateMultipartUploadRequestObjectInitiateMultipartUploadTypeDef",
     "CreateMultipartUploadRequestObjectSummaryInitiateMultipartUploadTypeDef",
     "CreateMultipartUploadRequestRequestTypeDef",
     "DefaultRetentionTypeDef",
     "DeleteBucketAnalyticsConfigurationRequestRequestTypeDef",
     "DeleteBucketCorsRequestBucketCorsDeleteTypeDef",
     "DeleteBucketCorsRequestRequestTypeDef",
@@ -137,88 +134,74 @@
     "DeleteBucketRequestBucketDeleteTypeDef",
     "DeleteBucketRequestRequestTypeDef",
     "DeleteBucketTaggingRequestBucketTaggingDeleteTypeDef",
     "DeleteBucketTaggingRequestRequestTypeDef",
     "DeleteBucketWebsiteRequestBucketWebsiteDeleteTypeDef",
     "DeleteBucketWebsiteRequestRequestTypeDef",
     "DeleteMarkerReplicationTypeDef",
-    "DeleteObjectOutputTypeDef",
     "DeleteObjectRequestObjectDeleteTypeDef",
     "DeleteObjectRequestObjectSummaryDeleteTypeDef",
     "DeleteObjectRequestObjectVersionDeleteTypeDef",
     "DeleteObjectRequestRequestTypeDef",
-    "DeleteObjectTaggingOutputTypeDef",
     "DeleteObjectTaggingRequestRequestTypeDef",
     "DeletedObjectTypeDef",
     "ErrorTypeDef",
     "DeletePublicAccessBlockRequestRequestTypeDef",
     "ObjectIdentifierTypeDef",
     "EncryptionConfigurationTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "EncryptionTypeDef",
-    "ErrorDocumentResponseMetadataTypeDef",
     "ErrorDocumentTypeDef",
     "ExistingObjectReplicationTypeDef",
     "FilterRuleTypeDef",
-    "GetBucketAccelerateConfigurationOutputTypeDef",
     "GetBucketAccelerateConfigurationRequestRequestTypeDef",
     "GetBucketAclRequestRequestTypeDef",
     "GetBucketAnalyticsConfigurationRequestRequestTypeDef",
     "GetBucketCorsRequestRequestTypeDef",
     "GetBucketEncryptionRequestRequestTypeDef",
     "GetBucketIntelligentTieringConfigurationRequestRequestTypeDef",
     "GetBucketInventoryConfigurationRequestRequestTypeDef",
     "GetBucketLifecycleConfigurationRequestRequestTypeDef",
     "GetBucketLifecycleRequestRequestTypeDef",
-    "GetBucketLocationOutputTypeDef",
     "GetBucketLocationRequestRequestTypeDef",
     "GetBucketLoggingRequestRequestTypeDef",
     "GetBucketMetricsConfigurationRequestRequestTypeDef",
     "GetBucketNotificationConfigurationRequestRequestTypeDef",
     "GetBucketOwnershipControlsRequestRequestTypeDef",
-    "GetBucketPolicyOutputTypeDef",
     "GetBucketPolicyRequestRequestTypeDef",
     "PolicyStatusTypeDef",
     "GetBucketPolicyStatusRequestRequestTypeDef",
     "GetBucketReplicationRequestRequestTypeDef",
-    "GetBucketRequestPaymentOutputTypeDef",
     "GetBucketRequestPaymentRequestRequestTypeDef",
     "GetBucketTaggingRequestRequestTypeDef",
-    "GetBucketVersioningOutputTypeDef",
     "GetBucketVersioningRequestRequestTypeDef",
     "IndexDocumentTypeDef",
     "RedirectAllRequestsToTypeDef",
     "GetBucketWebsiteRequestRequestTypeDef",
     "GetObjectAclRequestRequestTypeDef",
     "ObjectPartTypeDef",
     "GetObjectAttributesRequestRequestTypeDef",
     "ObjectLockLegalHoldTypeDef",
     "GetObjectLegalHoldRequestRequestTypeDef",
     "GetObjectLockConfigurationRequestRequestTypeDef",
-    "GetObjectOutputTypeDef",
     "GetObjectRequestObjectGetTypeDef",
     "GetObjectRequestObjectSummaryGetTypeDef",
     "GetObjectRequestObjectVersionGetTypeDef",
     "GetObjectRequestRequestTypeDef",
     "ObjectLockRetentionTypeDef",
     "GetObjectRetentionRequestRequestTypeDef",
     "GetObjectTaggingRequestRequestTypeDef",
-    "GetObjectTorrentOutputTypeDef",
     "GetObjectTorrentRequestRequestTypeDef",
     "PublicAccessBlockConfigurationTypeDef",
     "GetPublicAccessBlockRequestRequestTypeDef",
     "GlacierJobParametersTypeDef",
     "GranteeTypeDef",
     "WaiterConfigTypeDef",
     "HeadBucketRequestRequestTypeDef",
-    "HeadObjectOutputTypeDef",
     "HeadObjectRequestObjectVersionHeadTypeDef",
     "HeadObjectRequestRequestTypeDef",
-    "IndexDocumentResponseMetadataTypeDef",
-    "InitiatorResponseMetadataTypeDef",
     "InitiatorTypeDef",
     "JSONInputTypeDef",
     "TieringTypeDef",
     "InventoryFilterTypeDef",
     "InventoryScheduleTypeDef",
     "SSEKMSTypeDef",
     "JSONOutputTypeDef",
@@ -226,70 +209,82 @@
     "NoncurrentVersionExpirationTypeDef",
     "NoncurrentVersionTransitionTypeDef",
     "TransitionTypeDef",
     "ListBucketAnalyticsConfigurationsRequestRequestTypeDef",
     "ListBucketIntelligentTieringConfigurationsRequestRequestTypeDef",
     "ListBucketInventoryConfigurationsRequestRequestTypeDef",
     "ListBucketMetricsConfigurationsRequestRequestTypeDef",
-    "ListMultipartUploadsRequestListMultipartUploadsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListMultipartUploadsRequestRequestTypeDef",
-    "ListObjectVersionsRequestListObjectVersionsPaginateTypeDef",
     "ListObjectVersionsRequestRequestTypeDef",
-    "ListObjectsRequestListObjectsPaginateTypeDef",
     "ListObjectsRequestRequestTypeDef",
-    "ListObjectsV2RequestListObjectsV2PaginateTypeDef",
     "ListObjectsV2RequestRequestTypeDef",
     "PartTypeDef",
-    "ListPartsRequestListPartsPaginateTypeDef",
     "ListPartsRequestRequestTypeDef",
     "MetadataEntryTypeDef",
     "ReplicationTimeValueTypeDef",
     "QueueConfigurationDeprecatedTypeDef",
     "TopicConfigurationDeprecatedTypeDef",
     "ObjectDownloadFileRequestTypeDef",
     "ObjectDownloadFileobjRequestTypeDef",
     "RestoreStatusTypeDef",
     "ObjectUploadFileRequestTypeDef",
     "ObjectUploadFileobjRequestTypeDef",
-    "OwnerResponseMetadataTypeDef",
     "OwnershipControlsRuleTypeDef",
-    "PaginatorConfigTypeDef",
     "ProgressTypeDef",
     "PutBucketPolicyRequestBucketPolicyPutTypeDef",
     "PutBucketPolicyRequestRequestTypeDef",
     "RequestPaymentConfigurationTypeDef",
     "PutBucketVersioningRequestBucketVersioningEnableTypeDef",
     "VersioningConfigurationTypeDef",
     "PutBucketVersioningRequestBucketVersioningSuspendTypeDef",
-    "PutObjectAclOutputTypeDef",
-    "PutObjectLegalHoldOutputTypeDef",
-    "PutObjectLockConfigurationOutputTypeDef",
-    "PutObjectOutputTypeDef",
     "PutObjectRequestBucketPutObjectTypeDef",
     "PutObjectRequestObjectPutTypeDef",
     "PutObjectRequestObjectSummaryPutTypeDef",
     "PutObjectRequestRequestTypeDef",
-    "PutObjectRetentionOutputTypeDef",
-    "PutObjectTaggingOutputTypeDef",
     "RecordsEventTypeDef",
-    "RedirectAllRequestsToResponseMetadataTypeDef",
     "RedirectTypeDef",
     "ReplicaModificationsTypeDef",
     "RequestProgressTypeDef",
-    "ResponseMetadataTypeDef",
-    "RestoreObjectOutputTypeDef",
-    "RestoreStatusResponseMetadataTypeDef",
     "ScanRangeTypeDef",
     "ServerSideEncryptionByDefaultTypeDef",
     "SseKmsEncryptedObjectsTypeDef",
     "StatsTypeDef",
-    "UploadPartOutputTypeDef",
     "UploadPartRequestMultipartUploadPartUploadTypeDef",
     "UploadPartRequestRequestTypeDef",
     "WriteGetObjectResponseRequestRequestTypeDef",
+    "AbortMultipartUploadOutputTypeDef",
+    "CompleteMultipartUploadOutputTypeDef",
+    "CreateBucketOutputTypeDef",
+    "CreateMultipartUploadOutputTypeDef",
+    "DeleteObjectOutputTypeDef",
+    "DeleteObjectTaggingOutputTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "ErrorDocumentResponseMetadataTypeDef",
+    "GetBucketAccelerateConfigurationOutputTypeDef",
+    "GetBucketLocationOutputTypeDef",
+    "GetBucketPolicyOutputTypeDef",
+    "GetBucketRequestPaymentOutputTypeDef",
+    "GetBucketVersioningOutputTypeDef",
+    "GetObjectOutputTypeDef",
+    "GetObjectTorrentOutputTypeDef",
+    "HeadObjectOutputTypeDef",
+    "IndexDocumentResponseMetadataTypeDef",
+    "InitiatorResponseMetadataTypeDef",
+    "OwnerResponseMetadataTypeDef",
+    "PutObjectAclOutputTypeDef",
+    "PutObjectLegalHoldOutputTypeDef",
+    "PutObjectLockConfigurationOutputTypeDef",
+    "PutObjectOutputTypeDef",
+    "PutObjectRetentionOutputTypeDef",
+    "PutObjectTaggingOutputTypeDef",
+    "RedirectAllRequestsToResponseMetadataTypeDef",
+    "RestoreObjectOutputTypeDef",
+    "RestoreStatusResponseMetadataTypeDef",
+    "UploadPartOutputTypeDef",
     "PutBucketAccelerateConfigurationRequestRequestTypeDef",
     "DeleteMarkerEntryTypeDef",
     "AnalyticsAndOperatorTypeDef",
     "GetBucketTaggingOutputTypeDef",
     "GetObjectTaggingOutputTypeDef",
     "IntelligentTieringAndOperatorTypeDef",
     "LifecycleRuleAndOperatorTypeDef",
@@ -331,14 +326,19 @@
     "HeadObjectRequestObjectExistsWaitTypeDef",
     "HeadObjectRequestObjectNotExistsWaitTypeDef",
     "MultipartUploadTypeDef",
     "InputSerializationTypeDef",
     "InventoryEncryptionTypeDef",
     "OutputSerializationTypeDef",
     "RuleTypeDef",
+    "ListMultipartUploadsRequestListMultipartUploadsPaginateTypeDef",
+    "ListObjectVersionsRequestListObjectVersionsPaginateTypeDef",
+    "ListObjectsRequestListObjectsPaginateTypeDef",
+    "ListObjectsV2RequestListObjectsV2PaginateTypeDef",
+    "ListPartsRequestListPartsPaginateTypeDef",
     "ListPartsOutputTypeDef",
     "MetricsTypeDef",
     "ReplicationTimeTypeDef",
     "NotificationConfigurationDeprecatedResponseMetadataTypeDef",
     "NotificationConfigurationDeprecatedTypeDef",
     "ObjectTypeDef",
     "ObjectVersionTypeDef",
@@ -452,22 +452,24 @@
 )
 
 AbortIncompleteMultipartUploadTypeDef = TypedDict(
     "AbortIncompleteMultipartUploadTypeDef",
     {
         "DaysAfterInitiation": int,
     },
-    total=False,
 )
 
-AbortMultipartUploadOutputTypeDef = TypedDict(
-    "AbortMultipartUploadOutputTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "RequestCharged": Literal["requester"],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 AbortMultipartUploadRequestMultipartUploadAbortTypeDef = TypedDict(
     "AbortMultipartUploadRequestMultipartUploadAbortTypeDef",
     {
         "RequestPayer": Literal["requester"],
@@ -489,37 +491,34 @@
     {
         "RequestPayer": Literal["requester"],
         "ExpectedBucketOwner": str,
     },
     total=False,
 )
 
-
 class AbortMultipartUploadRequestRequestTypeDef(
     _RequiredAbortMultipartUploadRequestRequestTypeDef,
     _OptionalAbortMultipartUploadRequestRequestTypeDef,
 ):
     pass
 
-
 AccelerateConfigurationTypeDef = TypedDict(
     "AccelerateConfigurationTypeDef",
     {
         "Status": BucketAccelerateStatusType,
     },
     total=False,
 )
 
 OwnerTypeDef = TypedDict(
     "OwnerTypeDef",
     {
         "DisplayName": str,
         "ID": str,
     },
-    total=False,
 )
 
 AccessControlTranslationTypeDef = TypedDict(
     "AccessControlTranslationTypeDef",
     {
         "Owner": Literal["Destination"],
     },
@@ -529,37 +528,24 @@
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
-_RequiredAnalyticsS3BucketDestinationTypeDef = TypedDict(
-    "_RequiredAnalyticsS3BucketDestinationTypeDef",
+AnalyticsS3BucketDestinationTypeDef = TypedDict(
+    "AnalyticsS3BucketDestinationTypeDef",
     {
         "Format": Literal["CSV"],
-        "Bucket": str,
-    },
-)
-_OptionalAnalyticsS3BucketDestinationTypeDef = TypedDict(
-    "_OptionalAnalyticsS3BucketDestinationTypeDef",
-    {
         "BucketAccountId": str,
+        "Bucket": str,
         "Prefix": str,
     },
-    total=False,
 )
 
-
-class AnalyticsS3BucketDestinationTypeDef(
-    _RequiredAnalyticsS3BucketDestinationTypeDef, _OptionalAnalyticsS3BucketDestinationTypeDef
-):
-    pass
-
-
 _RequiredCopySourceTypeDef = TypedDict(
     "_RequiredCopySourceTypeDef",
     {
         "Bucket": str,
         "Key": str,
     },
 )
@@ -567,19 +553,17 @@
     "_OptionalCopySourceTypeDef",
     {
         "VersionId": str,
     },
     total=False,
 )
 
-
 class CopySourceTypeDef(_RequiredCopySourceTypeDef, _OptionalCopySourceTypeDef):
     pass
 
-
 _RequiredBucketDownloadFileRequestTypeDef = TypedDict(
     "_RequiredBucketDownloadFileRequestTypeDef",
     {
         "Key": str,
         "Filename": str,
     },
 )
@@ -589,21 +573,19 @@
         "ExtraArgs": Dict[str, Any],
         "Callback": Callable[..., Any],
         "Config": TransferConfig,
     },
     total=False,
 )
 
-
 class BucketDownloadFileRequestTypeDef(
     _RequiredBucketDownloadFileRequestTypeDef, _OptionalBucketDownloadFileRequestTypeDef
 ):
     pass
 
-
 _RequiredBucketDownloadFileobjRequestTypeDef = TypedDict(
     "_RequiredBucketDownloadFileobjRequestTypeDef",
     {
         "Key": str,
         "Fileobj": Union[IO[Any], StreamingBody],
     },
 )
@@ -613,28 +595,25 @@
         "ExtraArgs": Dict[str, Any],
         "Callback": Callable[..., Any],
         "Config": TransferConfig,
     },
     total=False,
 )
 
-
 class BucketDownloadFileobjRequestTypeDef(
     _RequiredBucketDownloadFileobjRequestTypeDef, _OptionalBucketDownloadFileobjRequestTypeDef
 ):
     pass
 
-
 BucketTypeDef = TypedDict(
     "BucketTypeDef",
     {
         "Name": str,
         "CreationDate": datetime,
     },
-    total=False,
 )
 
 _RequiredBucketUploadFileRequestTypeDef = TypedDict(
     "_RequiredBucketUploadFileRequestTypeDef",
     {
         "Filename": str,
         "Key": str,
@@ -646,21 +625,19 @@
         "ExtraArgs": Dict[str, Any],
         "Callback": Callable[..., Any],
         "Config": TransferConfig,
     },
     total=False,
 )
 
-
 class BucketUploadFileRequestTypeDef(
     _RequiredBucketUploadFileRequestTypeDef, _OptionalBucketUploadFileRequestTypeDef
 ):
     pass
 
-
 _RequiredBucketUploadFileobjRequestTypeDef = TypedDict(
     "_RequiredBucketUploadFileobjRequestTypeDef",
     {
         "Fileobj": Union[IO[Any], StreamingBody],
         "Key": str,
     },
 )
@@ -670,44 +647,31 @@
         "ExtraArgs": Dict[str, Any],
         "Callback": Callable[..., Any],
         "Config": TransferConfig,
     },
     total=False,
 )
 
-
 class BucketUploadFileobjRequestTypeDef(
     _RequiredBucketUploadFileobjRequestTypeDef, _OptionalBucketUploadFileobjRequestTypeDef
 ):
     pass
 
-
-_RequiredCORSRuleTypeDef = TypedDict(
-    "_RequiredCORSRuleTypeDef",
-    {
-        "AllowedMethods": List[str],
-        "AllowedOrigins": List[str],
-    },
-)
-_OptionalCORSRuleTypeDef = TypedDict(
-    "_OptionalCORSRuleTypeDef",
+CORSRuleTypeDef = TypedDict(
+    "CORSRuleTypeDef",
     {
         "ID": str,
         "AllowedHeaders": List[str],
+        "AllowedMethods": List[str],
+        "AllowedOrigins": List[str],
         "ExposeHeaders": List[str],
         "MaxAgeSeconds": int,
     },
-    total=False,
 )
 
-
-class CORSRuleTypeDef(_RequiredCORSRuleTypeDef, _OptionalCORSRuleTypeDef):
-    pass
-
-
 CSVInputTypeDef = TypedDict(
     "CSVInputTypeDef",
     {
         "FileHeaderInfo": FileHeaderInfoType,
         "Comments": str,
         "QuoteEscapeCharacter": str,
         "RecordDelimiter": str,
@@ -734,15 +698,14 @@
     "ChecksumTypeDef",
     {
         "ChecksumCRC32": str,
         "ChecksumCRC32C": str,
         "ChecksumSHA1": str,
         "ChecksumSHA256": str,
     },
-    total=False,
 )
 
 _RequiredClientDownloadFileRequestTypeDef = TypedDict(
     "_RequiredClientDownloadFileRequestTypeDef",
     {
         "Bucket": str,
         "Key": str,
@@ -755,21 +718,19 @@
         "ExtraArgs": Dict[str, Any],
         "Callback": Callable[..., Any],
         "Config": TransferConfig,
     },
     total=False,
 )
 
-
 class ClientDownloadFileRequestTypeDef(
     _RequiredClientDownloadFileRequestTypeDef, _OptionalClientDownloadFileRequestTypeDef
 ):
     pass
 
-
 _RequiredClientDownloadFileobjRequestTypeDef = TypedDict(
     "_RequiredClientDownloadFileobjRequestTypeDef",
     {
         "Bucket": str,
         "Key": str,
         "Fileobj": Union[IO[Any], StreamingBody],
     },
@@ -780,21 +741,19 @@
         "ExtraArgs": Dict[str, Any],
         "Callback": Callable[..., Any],
         "Config": TransferConfig,
     },
     total=False,
 )
 
-
 class ClientDownloadFileobjRequestTypeDef(
     _RequiredClientDownloadFileobjRequestTypeDef, _OptionalClientDownloadFileobjRequestTypeDef
 ):
     pass
 
-
 _RequiredClientGeneratePresignedPostRequestTypeDef = TypedDict(
     "_RequiredClientGeneratePresignedPostRequestTypeDef",
     {
         "Bucket": str,
         "Key": str,
     },
 )
@@ -804,22 +763,20 @@
         "Fields": Dict[str, Any],
         "Conditions": Union[List[Any], Dict[str, Any]],
         "ExpiresIn": int,
     },
     total=False,
 )
 
-
 class ClientGeneratePresignedPostRequestTypeDef(
     _RequiredClientGeneratePresignedPostRequestTypeDef,
     _OptionalClientGeneratePresignedPostRequestTypeDef,
 ):
     pass
 
-
 _RequiredClientUploadFileRequestTypeDef = TypedDict(
     "_RequiredClientUploadFileRequestTypeDef",
     {
         "Filename": str,
         "Bucket": str,
         "Key": str,
     },
@@ -830,21 +787,19 @@
         "ExtraArgs": Dict[str, Any],
         "Callback": Callable[..., Any],
         "Config": TransferConfig,
     },
     total=False,
 )
 
-
 class ClientUploadFileRequestTypeDef(
     _RequiredClientUploadFileRequestTypeDef, _OptionalClientUploadFileRequestTypeDef
 ):
     pass
 
-
 _RequiredClientUploadFileobjRequestTypeDef = TypedDict(
     "_RequiredClientUploadFileobjRequestTypeDef",
     {
         "Fileobj": Union[IO[Any], StreamingBody],
         "Bucket": str,
         "Key": str,
     },
@@ -855,60 +810,35 @@
         "ExtraArgs": Dict[str, Any],
         "Callback": Callable[..., Any],
         "Config": TransferConfig,
     },
     total=False,
 )
 
-
 class ClientUploadFileobjRequestTypeDef(
     _RequiredClientUploadFileobjRequestTypeDef, _OptionalClientUploadFileobjRequestTypeDef
 ):
     pass
 
-
 CloudFunctionConfigurationTypeDef = TypedDict(
     "CloudFunctionConfigurationTypeDef",
     {
         "Id": str,
         "Event": EventType,
         "Events": List[EventType],
         "CloudFunction": str,
         "InvocationRole": str,
     },
-    total=False,
 )
 
 CommonPrefixTypeDef = TypedDict(
     "CommonPrefixTypeDef",
     {
         "Prefix": str,
     },
-    total=False,
-)
-
-CompleteMultipartUploadOutputTypeDef = TypedDict(
-    "CompleteMultipartUploadOutputTypeDef",
-    {
-        "Location": str,
-        "Bucket": str,
-        "Key": str,
-        "Expiration": str,
-        "ETag": str,
-        "ChecksumCRC32": str,
-        "ChecksumCRC32C": str,
-        "ChecksumSHA1": str,
-        "ChecksumSHA256": str,
-        "ServerSideEncryption": ServerSideEncryptionType,
-        "VersionId": str,
-        "SSEKMSKeyId": str,
-        "BucketKeyEnabled": bool,
-        "RequestCharged": Literal["requester"],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
 )
 
 CompletedPartTypeDef = TypedDict(
     "CompletedPartTypeDef",
     {
         "ETag": str,
         "ChecksumCRC32": str,
@@ -922,28 +852,26 @@
 
 ConditionTypeDef = TypedDict(
     "ConditionTypeDef",
     {
         "HttpErrorCodeReturnedEquals": str,
         "KeyPrefixEquals": str,
     },
-    total=False,
 )
 
 CopyObjectResultTypeDef = TypedDict(
     "CopyObjectResultTypeDef",
     {
         "ETag": str,
         "LastModified": datetime,
         "ChecksumCRC32": str,
         "ChecksumCRC32C": str,
         "ChecksumSHA1": str,
         "ChecksumSHA256": str,
     },
-    total=False,
 )
 
 _RequiredCopyObjectRequestObjectCopyFromTypeDef = TypedDict(
     "_RequiredCopyObjectRequestObjectCopyFromTypeDef",
     {
         "CopySource": str,
     },
@@ -989,21 +917,19 @@
         "ObjectLockLegalHoldStatus": ObjectLockLegalHoldStatusType,
         "ExpectedBucketOwner": str,
         "ExpectedSourceBucketOwner": str,
     },
     total=False,
 )
 
-
 class CopyObjectRequestObjectCopyFromTypeDef(
     _RequiredCopyObjectRequestObjectCopyFromTypeDef, _OptionalCopyObjectRequestObjectCopyFromTypeDef
 ):
     pass
 
-
 _RequiredCopyObjectRequestObjectSummaryCopyFromTypeDef = TypedDict(
     "_RequiredCopyObjectRequestObjectSummaryCopyFromTypeDef",
     {
         "CopySource": str,
     },
 )
 _OptionalCopyObjectRequestObjectSummaryCopyFromTypeDef = TypedDict(
@@ -1047,71 +973,40 @@
         "ObjectLockLegalHoldStatus": ObjectLockLegalHoldStatusType,
         "ExpectedBucketOwner": str,
         "ExpectedSourceBucketOwner": str,
     },
     total=False,
 )
 
-
 class CopyObjectRequestObjectSummaryCopyFromTypeDef(
     _RequiredCopyObjectRequestObjectSummaryCopyFromTypeDef,
     _OptionalCopyObjectRequestObjectSummaryCopyFromTypeDef,
 ):
     pass
 
-
 CopyPartResultTypeDef = TypedDict(
     "CopyPartResultTypeDef",
     {
         "ETag": str,
         "LastModified": datetime,
         "ChecksumCRC32": str,
         "ChecksumCRC32C": str,
         "ChecksumSHA1": str,
         "ChecksumSHA256": str,
     },
-    total=False,
 )
 
 CreateBucketConfigurationTypeDef = TypedDict(
     "CreateBucketConfigurationTypeDef",
     {
         "LocationConstraint": BucketLocationConstraintType,
     },
     total=False,
 )
 
-CreateBucketOutputTypeDef = TypedDict(
-    "CreateBucketOutputTypeDef",
-    {
-        "Location": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateMultipartUploadOutputTypeDef = TypedDict(
-    "CreateMultipartUploadOutputTypeDef",
-    {
-        "AbortDate": datetime,
-        "AbortRuleId": str,
-        "Bucket": str,
-        "Key": str,
-        "UploadId": str,
-        "ServerSideEncryption": ServerSideEncryptionType,
-        "SSECustomerAlgorithm": str,
-        "SSECustomerKeyMD5": str,
-        "SSEKMSKeyId": str,
-        "SSEKMSEncryptionContext": str,
-        "BucketKeyEnabled": bool,
-        "RequestCharged": Literal["requester"],
-        "ChecksumAlgorithm": ChecksumAlgorithmType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CreateMultipartUploadRequestObjectInitiateMultipartUploadTypeDef = TypedDict(
     "CreateMultipartUploadRequestObjectInitiateMultipartUploadTypeDef",
     {
         "ACL": ObjectCannedACLType,
         "CacheControl": str,
         "ContentDisposition": str,
         "ContentEncoding": str,
@@ -1216,30 +1111,27 @@
         "ObjectLockLegalHoldStatus": ObjectLockLegalHoldStatusType,
         "ExpectedBucketOwner": str,
         "ChecksumAlgorithm": ChecksumAlgorithmType,
     },
     total=False,
 )
 
-
 class CreateMultipartUploadRequestRequestTypeDef(
     _RequiredCreateMultipartUploadRequestRequestTypeDef,
     _OptionalCreateMultipartUploadRequestRequestTypeDef,
 ):
     pass
 
-
 DefaultRetentionTypeDef = TypedDict(
     "DefaultRetentionTypeDef",
     {
         "Mode": ObjectLockRetentionModeType,
         "Days": int,
         "Years": int,
     },
-    total=False,
 )
 
 _RequiredDeleteBucketAnalyticsConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteBucketAnalyticsConfigurationRequestRequestTypeDef",
     {
         "Bucket": str,
         "Id": str,
@@ -1249,22 +1141,20 @@
     "_OptionalDeleteBucketAnalyticsConfigurationRequestRequestTypeDef",
     {
         "ExpectedBucketOwner": str,
     },
     total=False,
 )
 
-
 class DeleteBucketAnalyticsConfigurationRequestRequestTypeDef(
     _RequiredDeleteBucketAnalyticsConfigurationRequestRequestTypeDef,
     _OptionalDeleteBucketAnalyticsConfigurationRequestRequestTypeDef,
 ):
     pass
 
-
 DeleteBucketCorsRequestBucketCorsDeleteTypeDef = TypedDict(
     "DeleteBucketCorsRequestBucketCorsDeleteTypeDef",
     {
         "ExpectedBucketOwner": str,
     },
     total=False,
 )
@@ -1279,43 +1169,39 @@
     "_OptionalDeleteBucketCorsRequestRequestTypeDef",
     {
         "ExpectedBucketOwner": str,
     },
     total=False,
 )
 
-
 class DeleteBucketCorsRequestRequestTypeDef(
     _RequiredDeleteBucketCorsRequestRequestTypeDef, _OptionalDeleteBucketCorsRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredDeleteBucketEncryptionRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteBucketEncryptionRequestRequestTypeDef",
     {
         "Bucket": str,
     },
 )
 _OptionalDeleteBucketEncryptionRequestRequestTypeDef = TypedDict(
     "_OptionalDeleteBucketEncryptionRequestRequestTypeDef",
     {
         "ExpectedBucketOwner": str,
     },
     total=False,
 )
 
-
 class DeleteBucketEncryptionRequestRequestTypeDef(
     _RequiredDeleteBucketEncryptionRequestRequestTypeDef,
     _OptionalDeleteBucketEncryptionRequestRequestTypeDef,
 ):
     pass
 
-
 DeleteBucketIntelligentTieringConfigurationRequestRequestTypeDef = TypedDict(
     "DeleteBucketIntelligentTieringConfigurationRequestRequestTypeDef",
     {
         "Bucket": str,
         "Id": str,
     },
 )
@@ -1331,22 +1217,20 @@
     "_OptionalDeleteBucketInventoryConfigurationRequestRequestTypeDef",
     {
         "ExpectedBucketOwner": str,
     },
     total=False,
 )
 
-
 class DeleteBucketInventoryConfigurationRequestRequestTypeDef(
     _RequiredDeleteBucketInventoryConfigurationRequestRequestTypeDef,
     _OptionalDeleteBucketInventoryConfigurationRequestRequestTypeDef,
 ):
     pass
 
-
 DeleteBucketLifecycleRequestBucketLifecycleConfigurationDeleteTypeDef = TypedDict(
     "DeleteBucketLifecycleRequestBucketLifecycleConfigurationDeleteTypeDef",
     {
         "ExpectedBucketOwner": str,
     },
     total=False,
 )
@@ -1369,22 +1253,20 @@
     "_OptionalDeleteBucketLifecycleRequestRequestTypeDef",
     {
         "ExpectedBucketOwner": str,
     },
     total=False,
 )
 
-
 class DeleteBucketLifecycleRequestRequestTypeDef(
     _RequiredDeleteBucketLifecycleRequestRequestTypeDef,
     _OptionalDeleteBucketLifecycleRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredDeleteBucketMetricsConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteBucketMetricsConfigurationRequestRequestTypeDef",
     {
         "Bucket": str,
         "Id": str,
     },
 )
@@ -1392,44 +1274,40 @@
     "_OptionalDeleteBucketMetricsConfigurationRequestRequestTypeDef",
     {
         "ExpectedBucketOwner": str,
     },
     total=False,
 )
 
-
 class DeleteBucketMetricsConfigurationRequestRequestTypeDef(
     _RequiredDeleteBucketMetricsConfigurationRequestRequestTypeDef,
     _OptionalDeleteBucketMetricsConfigurationRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredDeleteBucketOwnershipControlsRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteBucketOwnershipControlsRequestRequestTypeDef",
     {
         "Bucket": str,
     },
 )
 _OptionalDeleteBucketOwnershipControlsRequestRequestTypeDef = TypedDict(
     "_OptionalDeleteBucketOwnershipControlsRequestRequestTypeDef",
     {
         "ExpectedBucketOwner": str,
     },
     total=False,
 )
 
-
 class DeleteBucketOwnershipControlsRequestRequestTypeDef(
     _RequiredDeleteBucketOwnershipControlsRequestRequestTypeDef,
     _OptionalDeleteBucketOwnershipControlsRequestRequestTypeDef,
 ):
     pass
 
-
 DeleteBucketPolicyRequestBucketPolicyDeleteTypeDef = TypedDict(
     "DeleteBucketPolicyRequestBucketPolicyDeleteTypeDef",
     {
         "ExpectedBucketOwner": str,
     },
     total=False,
 )
@@ -1444,44 +1322,40 @@
     "_OptionalDeleteBucketPolicyRequestRequestTypeDef",
     {
         "ExpectedBucketOwner": str,
     },
     total=False,
 )
 
-
 class DeleteBucketPolicyRequestRequestTypeDef(
     _RequiredDeleteBucketPolicyRequestRequestTypeDef,
     _OptionalDeleteBucketPolicyRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredDeleteBucketReplicationRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteBucketReplicationRequestRequestTypeDef",
     {
         "Bucket": str,
     },
 )
 _OptionalDeleteBucketReplicationRequestRequestTypeDef = TypedDict(
     "_OptionalDeleteBucketReplicationRequestRequestTypeDef",
     {
         "ExpectedBucketOwner": str,
     },
     total=False,
 )
 
-
 class DeleteBucketReplicationRequestRequestTypeDef(
     _RequiredDeleteBucketReplicationRequestRequestTypeDef,
     _OptionalDeleteBucketReplicationRequestRequestTypeDef,
 ):
     pass
 
-
 DeleteBucketRequestBucketDeleteTypeDef = TypedDict(
     "DeleteBucketRequestBucketDeleteTypeDef",
     {
         "ExpectedBucketOwner": str,
     },
     total=False,
 )
@@ -1496,21 +1370,19 @@
     "_OptionalDeleteBucketRequestRequestTypeDef",
     {
         "ExpectedBucketOwner": str,
     },
     total=False,
 )
 
-
 class DeleteBucketRequestRequestTypeDef(
     _RequiredDeleteBucketRequestRequestTypeDef, _OptionalDeleteBucketRequestRequestTypeDef
 ):
     pass
 
-
 DeleteBucketTaggingRequestBucketTaggingDeleteTypeDef = TypedDict(
     "DeleteBucketTaggingRequestBucketTaggingDeleteTypeDef",
     {
         "ExpectedBucketOwner": str,
     },
     total=False,
 )
@@ -1525,22 +1397,20 @@
     "_OptionalDeleteBucketTaggingRequestRequestTypeDef",
     {
         "ExpectedBucketOwner": str,
     },
     total=False,
 )
 
-
 class DeleteBucketTaggingRequestRequestTypeDef(
     _RequiredDeleteBucketTaggingRequestRequestTypeDef,
     _OptionalDeleteBucketTaggingRequestRequestTypeDef,
 ):
     pass
 
-
 DeleteBucketWebsiteRequestBucketWebsiteDeleteTypeDef = TypedDict(
     "DeleteBucketWebsiteRequestBucketWebsiteDeleteTypeDef",
     {
         "ExpectedBucketOwner": str,
     },
     total=False,
 )
@@ -1555,38 +1425,25 @@
     "_OptionalDeleteBucketWebsiteRequestRequestTypeDef",
     {
         "ExpectedBucketOwner": str,
     },
     total=False,
 )
 
-
 class DeleteBucketWebsiteRequestRequestTypeDef(
     _RequiredDeleteBucketWebsiteRequestRequestTypeDef,
     _OptionalDeleteBucketWebsiteRequestRequestTypeDef,
 ):
     pass
 
-
 DeleteMarkerReplicationTypeDef = TypedDict(
     "DeleteMarkerReplicationTypeDef",
     {
         "Status": DeleteMarkerReplicationStatusType,
     },
-    total=False,
-)
-
-DeleteObjectOutputTypeDef = TypedDict(
-    "DeleteObjectOutputTypeDef",
-    {
-        "DeleteMarker": bool,
-        "VersionId": str,
-        "RequestCharged": Literal["requester"],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
 )
 
 DeleteObjectRequestObjectDeleteTypeDef = TypedDict(
     "DeleteObjectRequestObjectDeleteTypeDef",
     {
         "MFA": str,
         "VersionId": str,
@@ -1635,29 +1492,19 @@
         "RequestPayer": Literal["requester"],
         "BypassGovernanceRetention": bool,
         "ExpectedBucketOwner": str,
     },
     total=False,
 )
 
-
 class DeleteObjectRequestRequestTypeDef(
     _RequiredDeleteObjectRequestRequestTypeDef, _OptionalDeleteObjectRequestRequestTypeDef
 ):
     pass
 
-
-DeleteObjectTaggingOutputTypeDef = TypedDict(
-    "DeleteObjectTaggingOutputTypeDef",
-    {
-        "VersionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDeleteObjectTaggingRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteObjectTaggingRequestRequestTypeDef",
     {
         "Bucket": str,
         "Key": str,
     },
 )
@@ -1666,42 +1513,38 @@
     {
         "VersionId": str,
         "ExpectedBucketOwner": str,
     },
     total=False,
 )
 
-
 class DeleteObjectTaggingRequestRequestTypeDef(
     _RequiredDeleteObjectTaggingRequestRequestTypeDef,
     _OptionalDeleteObjectTaggingRequestRequestTypeDef,
 ):
     pass
 
-
 DeletedObjectTypeDef = TypedDict(
     "DeletedObjectTypeDef",
     {
         "Key": str,
         "VersionId": str,
         "DeleteMarker": bool,
         "DeleteMarkerVersionId": str,
     },
-    total=False,
 )
 
 ErrorTypeDef = TypedDict(
     "ErrorTypeDef",
     {
         "Key": str,
         "VersionId": str,
         "Code": str,
         "Message": str,
     },
-    total=False,
 )
 
 _RequiredDeletePublicAccessBlockRequestRequestTypeDef = TypedDict(
     "_RequiredDeletePublicAccessBlockRequestRequestTypeDef",
     {
         "Bucket": str,
     },
@@ -1710,54 +1553,42 @@
     "_OptionalDeletePublicAccessBlockRequestRequestTypeDef",
     {
         "ExpectedBucketOwner": str,
     },
     total=False,
 )
 
-
 class DeletePublicAccessBlockRequestRequestTypeDef(
     _RequiredDeletePublicAccessBlockRequestRequestTypeDef,
     _OptionalDeletePublicAccessBlockRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredObjectIdentifierTypeDef = TypedDict(
     "_RequiredObjectIdentifierTypeDef",
     {
         "Key": str,
     },
 )
 _OptionalObjectIdentifierTypeDef = TypedDict(
     "_OptionalObjectIdentifierTypeDef",
     {
         "VersionId": str,
     },
     total=False,
 )
 
-
 class ObjectIdentifierTypeDef(_RequiredObjectIdentifierTypeDef, _OptionalObjectIdentifierTypeDef):
     pass
 
-
 EncryptionConfigurationTypeDef = TypedDict(
     "EncryptionConfigurationTypeDef",
     {
         "ReplicaKmsKeyID": str,
     },
-    total=False,
-)
-
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
 )
 
 _RequiredEncryptionTypeDef = TypedDict(
     "_RequiredEncryptionTypeDef",
     {
         "EncryptionType": ServerSideEncryptionType,
     },
@@ -1767,27 +1598,17 @@
     {
         "KMSKeyId": str,
         "KMSContext": str,
     },
     total=False,
 )
 
-
 class EncryptionTypeDef(_RequiredEncryptionTypeDef, _OptionalEncryptionTypeDef):
     pass
 
-
-ErrorDocumentResponseMetadataTypeDef = TypedDict(
-    "ErrorDocumentResponseMetadataTypeDef",
-    {
-        "Key": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ErrorDocumentTypeDef = TypedDict(
     "ErrorDocumentTypeDef",
     {
         "Key": str,
     },
 )
 
@@ -1800,24 +1621,14 @@
 
 FilterRuleTypeDef = TypedDict(
     "FilterRuleTypeDef",
     {
         "Name": FilterRuleNameType,
         "Value": str,
     },
-    total=False,
-)
-
-GetBucketAccelerateConfigurationOutputTypeDef = TypedDict(
-    "GetBucketAccelerateConfigurationOutputTypeDef",
-    {
-        "Status": BucketAccelerateStatusType,
-        "RequestCharged": Literal["requester"],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
 )
 
 _RequiredGetBucketAccelerateConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredGetBucketAccelerateConfigurationRequestRequestTypeDef",
     {
         "Bucket": str,
     },
@@ -1827,43 +1638,39 @@
     {
         "ExpectedBucketOwner": str,
         "RequestPayer": Literal["requester"],
     },
     total=False,
 )
 
-
 class GetBucketAccelerateConfigurationRequestRequestTypeDef(
     _RequiredGetBucketAccelerateConfigurationRequestRequestTypeDef,
     _OptionalGetBucketAccelerateConfigurationRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredGetBucketAclRequestRequestTypeDef = TypedDict(
     "_RequiredGetBucketAclRequestRequestTypeDef",
     {
         "Bucket": str,
     },
 )
 _OptionalGetBucketAclRequestRequestTypeDef = TypedDict(
     "_OptionalGetBucketAclRequestRequestTypeDef",
     {
         "ExpectedBucketOwner": str,
     },
     total=False,
 )
 
-
 class GetBucketAclRequestRequestTypeDef(
     _RequiredGetBucketAclRequestRequestTypeDef, _OptionalGetBucketAclRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredGetBucketAnalyticsConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredGetBucketAnalyticsConfigurationRequestRequestTypeDef",
     {
         "Bucket": str,
         "Id": str,
     },
 )
@@ -1871,65 +1678,59 @@
     "_OptionalGetBucketAnalyticsConfigurationRequestRequestTypeDef",
     {
         "ExpectedBucketOwner": str,
     },
     total=False,
 )
 
-
 class GetBucketAnalyticsConfigurationRequestRequestTypeDef(
     _RequiredGetBucketAnalyticsConfigurationRequestRequestTypeDef,
     _OptionalGetBucketAnalyticsConfigurationRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredGetBucketCorsRequestRequestTypeDef = TypedDict(
     "_RequiredGetBucketCorsRequestRequestTypeDef",
     {
         "Bucket": str,
     },
 )
 _OptionalGetBucketCorsRequestRequestTypeDef = TypedDict(
     "_OptionalGetBucketCorsRequestRequestTypeDef",
     {
         "ExpectedBucketOwner": str,
     },
     total=False,
 )
 
-
 class GetBucketCorsRequestRequestTypeDef(
     _RequiredGetBucketCorsRequestRequestTypeDef, _OptionalGetBucketCorsRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredGetBucketEncryptionRequestRequestTypeDef = TypedDict(
     "_RequiredGetBucketEncryptionRequestRequestTypeDef",
     {
         "Bucket": str,
     },
 )
 _OptionalGetBucketEncryptionRequestRequestTypeDef = TypedDict(
     "_OptionalGetBucketEncryptionRequestRequestTypeDef",
     {
         "ExpectedBucketOwner": str,
     },
     total=False,
 )
 
-
 class GetBucketEncryptionRequestRequestTypeDef(
     _RequiredGetBucketEncryptionRequestRequestTypeDef,
     _OptionalGetBucketEncryptionRequestRequestTypeDef,
 ):
     pass
 
-
 GetBucketIntelligentTieringConfigurationRequestRequestTypeDef = TypedDict(
     "GetBucketIntelligentTieringConfigurationRequestRequestTypeDef",
     {
         "Bucket": str,
         "Id": str,
     },
 )
@@ -1945,116 +1746,98 @@
     "_OptionalGetBucketInventoryConfigurationRequestRequestTypeDef",
     {
         "ExpectedBucketOwner": str,
     },
     total=False,
 )
 
-
 class GetBucketInventoryConfigurationRequestRequestTypeDef(
     _RequiredGetBucketInventoryConfigurationRequestRequestTypeDef,
     _OptionalGetBucketInventoryConfigurationRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredGetBucketLifecycleConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredGetBucketLifecycleConfigurationRequestRequestTypeDef",
     {
         "Bucket": str,
     },
 )
 _OptionalGetBucketLifecycleConfigurationRequestRequestTypeDef = TypedDict(
     "_OptionalGetBucketLifecycleConfigurationRequestRequestTypeDef",
     {
         "ExpectedBucketOwner": str,
     },
     total=False,
 )
 
-
 class GetBucketLifecycleConfigurationRequestRequestTypeDef(
     _RequiredGetBucketLifecycleConfigurationRequestRequestTypeDef,
     _OptionalGetBucketLifecycleConfigurationRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredGetBucketLifecycleRequestRequestTypeDef = TypedDict(
     "_RequiredGetBucketLifecycleRequestRequestTypeDef",
     {
         "Bucket": str,
     },
 )
 _OptionalGetBucketLifecycleRequestRequestTypeDef = TypedDict(
     "_OptionalGetBucketLifecycleRequestRequestTypeDef",
     {
         "ExpectedBucketOwner": str,
     },
     total=False,
 )
 
-
 class GetBucketLifecycleRequestRequestTypeDef(
     _RequiredGetBucketLifecycleRequestRequestTypeDef,
     _OptionalGetBucketLifecycleRequestRequestTypeDef,
 ):
     pass
 
-
-GetBucketLocationOutputTypeDef = TypedDict(
-    "GetBucketLocationOutputTypeDef",
-    {
-        "LocationConstraint": BucketLocationConstraintType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetBucketLocationRequestRequestTypeDef = TypedDict(
     "_RequiredGetBucketLocationRequestRequestTypeDef",
     {
         "Bucket": str,
     },
 )
 _OptionalGetBucketLocationRequestRequestTypeDef = TypedDict(
     "_OptionalGetBucketLocationRequestRequestTypeDef",
     {
         "ExpectedBucketOwner": str,
     },
     total=False,
 )
 
-
 class GetBucketLocationRequestRequestTypeDef(
     _RequiredGetBucketLocationRequestRequestTypeDef, _OptionalGetBucketLocationRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredGetBucketLoggingRequestRequestTypeDef = TypedDict(
     "_RequiredGetBucketLoggingRequestRequestTypeDef",
     {
         "Bucket": str,
     },
 )
 _OptionalGetBucketLoggingRequestRequestTypeDef = TypedDict(
     "_OptionalGetBucketLoggingRequestRequestTypeDef",
     {
         "ExpectedBucketOwner": str,
     },
     total=False,
 )
 
-
 class GetBucketLoggingRequestRequestTypeDef(
     _RequiredGetBucketLoggingRequestRequestTypeDef, _OptionalGetBucketLoggingRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredGetBucketMetricsConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredGetBucketMetricsConfigurationRequestRequestTypeDef",
     {
         "Bucket": str,
         "Id": str,
     },
 )
@@ -2062,101 +1845,84 @@
     "_OptionalGetBucketMetricsConfigurationRequestRequestTypeDef",
     {
         "ExpectedBucketOwner": str,
     },
     total=False,
 )
 
-
 class GetBucketMetricsConfigurationRequestRequestTypeDef(
     _RequiredGetBucketMetricsConfigurationRequestRequestTypeDef,
     _OptionalGetBucketMetricsConfigurationRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredGetBucketNotificationConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredGetBucketNotificationConfigurationRequestRequestTypeDef",
     {
         "Bucket": str,
     },
 )
 _OptionalGetBucketNotificationConfigurationRequestRequestTypeDef = TypedDict(
     "_OptionalGetBucketNotificationConfigurationRequestRequestTypeDef",
     {
         "ExpectedBucketOwner": str,
     },
     total=False,
 )
 
-
 class GetBucketNotificationConfigurationRequestRequestTypeDef(
     _RequiredGetBucketNotificationConfigurationRequestRequestTypeDef,
     _OptionalGetBucketNotificationConfigurationRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredGetBucketOwnershipControlsRequestRequestTypeDef = TypedDict(
     "_RequiredGetBucketOwnershipControlsRequestRequestTypeDef",
     {
         "Bucket": str,
     },
 )
 _OptionalGetBucketOwnershipControlsRequestRequestTypeDef = TypedDict(
     "_OptionalGetBucketOwnershipControlsRequestRequestTypeDef",
     {
         "ExpectedBucketOwner": str,
     },
     total=False,
 )
 
-
 class GetBucketOwnershipControlsRequestRequestTypeDef(
     _RequiredGetBucketOwnershipControlsRequestRequestTypeDef,
     _OptionalGetBucketOwnershipControlsRequestRequestTypeDef,
 ):
     pass
 
-
-GetBucketPolicyOutputTypeDef = TypedDict(
-    "GetBucketPolicyOutputTypeDef",
-    {
-        "Policy": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetBucketPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredGetBucketPolicyRequestRequestTypeDef",
     {
         "Bucket": str,
     },
 )
 _OptionalGetBucketPolicyRequestRequestTypeDef = TypedDict(
     "_OptionalGetBucketPolicyRequestRequestTypeDef",
     {
         "ExpectedBucketOwner": str,
     },
     total=False,
 )
 
-
 class GetBucketPolicyRequestRequestTypeDef(
     _RequiredGetBucketPolicyRequestRequestTypeDef, _OptionalGetBucketPolicyRequestRequestTypeDef
 ):
     pass
 
-
 PolicyStatusTypeDef = TypedDict(
     "PolicyStatusTypeDef",
     {
         "IsPublic": bool,
     },
-    total=False,
 )
 
 _RequiredGetBucketPolicyStatusRequestRequestTypeDef = TypedDict(
     "_RequiredGetBucketPolicyStatusRequestRequestTypeDef",
     {
         "Bucket": str,
     },
@@ -2165,175 +1931,133 @@
     "_OptionalGetBucketPolicyStatusRequestRequestTypeDef",
     {
         "ExpectedBucketOwner": str,
     },
     total=False,
 )
 
-
 class GetBucketPolicyStatusRequestRequestTypeDef(
     _RequiredGetBucketPolicyStatusRequestRequestTypeDef,
     _OptionalGetBucketPolicyStatusRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredGetBucketReplicationRequestRequestTypeDef = TypedDict(
     "_RequiredGetBucketReplicationRequestRequestTypeDef",
     {
         "Bucket": str,
     },
 )
 _OptionalGetBucketReplicationRequestRequestTypeDef = TypedDict(
     "_OptionalGetBucketReplicationRequestRequestTypeDef",
     {
         "ExpectedBucketOwner": str,
     },
     total=False,
 )
 
-
 class GetBucketReplicationRequestRequestTypeDef(
     _RequiredGetBucketReplicationRequestRequestTypeDef,
     _OptionalGetBucketReplicationRequestRequestTypeDef,
 ):
     pass
 
-
-GetBucketRequestPaymentOutputTypeDef = TypedDict(
-    "GetBucketRequestPaymentOutputTypeDef",
-    {
-        "Payer": PayerType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetBucketRequestPaymentRequestRequestTypeDef = TypedDict(
     "_RequiredGetBucketRequestPaymentRequestRequestTypeDef",
     {
         "Bucket": str,
     },
 )
 _OptionalGetBucketRequestPaymentRequestRequestTypeDef = TypedDict(
     "_OptionalGetBucketRequestPaymentRequestRequestTypeDef",
     {
         "ExpectedBucketOwner": str,
     },
     total=False,
 )
 
-
 class GetBucketRequestPaymentRequestRequestTypeDef(
     _RequiredGetBucketRequestPaymentRequestRequestTypeDef,
     _OptionalGetBucketRequestPaymentRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredGetBucketTaggingRequestRequestTypeDef = TypedDict(
     "_RequiredGetBucketTaggingRequestRequestTypeDef",
     {
         "Bucket": str,
     },
 )
 _OptionalGetBucketTaggingRequestRequestTypeDef = TypedDict(
     "_OptionalGetBucketTaggingRequestRequestTypeDef",
     {
         "ExpectedBucketOwner": str,
     },
     total=False,
 )
 
-
 class GetBucketTaggingRequestRequestTypeDef(
     _RequiredGetBucketTaggingRequestRequestTypeDef, _OptionalGetBucketTaggingRequestRequestTypeDef
 ):
     pass
 
-
-GetBucketVersioningOutputTypeDef = TypedDict(
-    "GetBucketVersioningOutputTypeDef",
-    {
-        "Status": BucketVersioningStatusType,
-        "MFADelete": MFADeleteStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetBucketVersioningRequestRequestTypeDef = TypedDict(
     "_RequiredGetBucketVersioningRequestRequestTypeDef",
     {
         "Bucket": str,
     },
 )
 _OptionalGetBucketVersioningRequestRequestTypeDef = TypedDict(
     "_OptionalGetBucketVersioningRequestRequestTypeDef",
     {
         "ExpectedBucketOwner": str,
     },
     total=False,
 )
 
-
 class GetBucketVersioningRequestRequestTypeDef(
     _RequiredGetBucketVersioningRequestRequestTypeDef,
     _OptionalGetBucketVersioningRequestRequestTypeDef,
 ):
     pass
 
-
 IndexDocumentTypeDef = TypedDict(
     "IndexDocumentTypeDef",
     {
         "Suffix": str,
     },
 )
 
-_RequiredRedirectAllRequestsToTypeDef = TypedDict(
-    "_RequiredRedirectAllRequestsToTypeDef",
+RedirectAllRequestsToTypeDef = TypedDict(
+    "RedirectAllRequestsToTypeDef",
     {
         "HostName": str,
-    },
-)
-_OptionalRedirectAllRequestsToTypeDef = TypedDict(
-    "_OptionalRedirectAllRequestsToTypeDef",
-    {
         "Protocol": ProtocolType,
     },
-    total=False,
 )
 
-
-class RedirectAllRequestsToTypeDef(
-    _RequiredRedirectAllRequestsToTypeDef, _OptionalRedirectAllRequestsToTypeDef
-):
-    pass
-
-
 _RequiredGetBucketWebsiteRequestRequestTypeDef = TypedDict(
     "_RequiredGetBucketWebsiteRequestRequestTypeDef",
     {
         "Bucket": str,
     },
 )
 _OptionalGetBucketWebsiteRequestRequestTypeDef = TypedDict(
     "_OptionalGetBucketWebsiteRequestRequestTypeDef",
     {
         "ExpectedBucketOwner": str,
     },
     total=False,
 )
 
-
 class GetBucketWebsiteRequestRequestTypeDef(
     _RequiredGetBucketWebsiteRequestRequestTypeDef, _OptionalGetBucketWebsiteRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredGetObjectAclRequestRequestTypeDef = TypedDict(
     "_RequiredGetObjectAclRequestRequestTypeDef",
     {
         "Bucket": str,
         "Key": str,
     },
 )
@@ -2343,32 +2067,29 @@
         "VersionId": str,
         "RequestPayer": Literal["requester"],
         "ExpectedBucketOwner": str,
     },
     total=False,
 )
 
-
 class GetObjectAclRequestRequestTypeDef(
     _RequiredGetObjectAclRequestRequestTypeDef, _OptionalGetObjectAclRequestRequestTypeDef
 ):
     pass
 
-
 ObjectPartTypeDef = TypedDict(
     "ObjectPartTypeDef",
     {
         "PartNumber": int,
         "Size": int,
         "ChecksumCRC32": str,
         "ChecksumCRC32C": str,
         "ChecksumSHA1": str,
         "ChecksumSHA256": str,
     },
-    total=False,
 )
 
 _RequiredGetObjectAttributesRequestRequestTypeDef = TypedDict(
     "_RequiredGetObjectAttributesRequestRequestTypeDef",
     {
         "Bucket": str,
         "Key": str,
@@ -2386,28 +2107,25 @@
         "SSECustomerKeyMD5": str,
         "RequestPayer": Literal["requester"],
         "ExpectedBucketOwner": str,
     },
     total=False,
 )
 
-
 class GetObjectAttributesRequestRequestTypeDef(
     _RequiredGetObjectAttributesRequestRequestTypeDef,
     _OptionalGetObjectAttributesRequestRequestTypeDef,
 ):
     pass
 
-
 ObjectLockLegalHoldTypeDef = TypedDict(
     "ObjectLockLegalHoldTypeDef",
     {
         "Status": ObjectLockLegalHoldStatusType,
     },
-    total=False,
 )
 
 _RequiredGetObjectLegalHoldRequestRequestTypeDef = TypedDict(
     "_RequiredGetObjectLegalHoldRequestRequestTypeDef",
     {
         "Bucket": str,
         "Key": str,
@@ -2419,87 +2137,40 @@
         "VersionId": str,
         "RequestPayer": Literal["requester"],
         "ExpectedBucketOwner": str,
     },
     total=False,
 )
 
-
 class GetObjectLegalHoldRequestRequestTypeDef(
     _RequiredGetObjectLegalHoldRequestRequestTypeDef,
     _OptionalGetObjectLegalHoldRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredGetObjectLockConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredGetObjectLockConfigurationRequestRequestTypeDef",
     {
         "Bucket": str,
     },
 )
 _OptionalGetObjectLockConfigurationRequestRequestTypeDef = TypedDict(
     "_OptionalGetObjectLockConfigurationRequestRequestTypeDef",
     {
         "ExpectedBucketOwner": str,
     },
     total=False,
 )
 
-
 class GetObjectLockConfigurationRequestRequestTypeDef(
     _RequiredGetObjectLockConfigurationRequestRequestTypeDef,
     _OptionalGetObjectLockConfigurationRequestRequestTypeDef,
 ):
     pass
 
-
-GetObjectOutputTypeDef = TypedDict(
-    "GetObjectOutputTypeDef",
-    {
-        "Body": StreamingBody,
-        "DeleteMarker": bool,
-        "AcceptRanges": str,
-        "Expiration": str,
-        "Restore": str,
-        "LastModified": datetime,
-        "ContentLength": int,
-        "ETag": str,
-        "ChecksumCRC32": str,
-        "ChecksumCRC32C": str,
-        "ChecksumSHA1": str,
-        "ChecksumSHA256": str,
-        "MissingMeta": int,
-        "VersionId": str,
-        "CacheControl": str,
-        "ContentDisposition": str,
-        "ContentEncoding": str,
-        "ContentLanguage": str,
-        "ContentRange": str,
-        "ContentType": str,
-        "Expires": datetime,
-        "WebsiteRedirectLocation": str,
-        "ServerSideEncryption": ServerSideEncryptionType,
-        "Metadata": Dict[str, str],
-        "SSECustomerAlgorithm": str,
-        "SSECustomerKeyMD5": str,
-        "SSEKMSKeyId": str,
-        "BucketKeyEnabled": bool,
-        "StorageClass": StorageClassType,
-        "RequestCharged": Literal["requester"],
-        "ReplicationStatus": ReplicationStatusType,
-        "PartsCount": int,
-        "TagCount": int,
-        "ObjectLockMode": ObjectLockModeType,
-        "ObjectLockRetainUntilDate": datetime,
-        "ObjectLockLegalHoldStatus": ObjectLockLegalHoldStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetObjectRequestObjectGetTypeDef = TypedDict(
     "GetObjectRequestObjectGetTypeDef",
     {
         "IfMatch": str,
         "IfModifiedSince": Union[datetime, str],
         "IfNoneMatch": str,
         "IfUnmodifiedSince": Union[datetime, str],
@@ -2602,28 +2273,25 @@
         "PartNumber": int,
         "ExpectedBucketOwner": str,
         "ChecksumMode": Literal["ENABLED"],
     },
     total=False,
 )
 
-
 class GetObjectRequestRequestTypeDef(
     _RequiredGetObjectRequestRequestTypeDef, _OptionalGetObjectRequestRequestTypeDef
 ):
     pass
 
-
 ObjectLockRetentionTypeDef = TypedDict(
     "ObjectLockRetentionTypeDef",
     {
         "Mode": ObjectLockRetentionModeType,
         "RetainUntilDate": datetime,
     },
-    total=False,
 )
 
 _RequiredGetObjectRetentionRequestRequestTypeDef = TypedDict(
     "_RequiredGetObjectRetentionRequestRequestTypeDef",
     {
         "Bucket": str,
         "Key": str,
@@ -2635,22 +2303,20 @@
         "VersionId": str,
         "RequestPayer": Literal["requester"],
         "ExpectedBucketOwner": str,
     },
     total=False,
 )
 
-
 class GetObjectRetentionRequestRequestTypeDef(
     _RequiredGetObjectRetentionRequestRequestTypeDef,
     _OptionalGetObjectRetentionRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredGetObjectTaggingRequestRequestTypeDef = TypedDict(
     "_RequiredGetObjectTaggingRequestRequestTypeDef",
     {
         "Bucket": str,
         "Key": str,
     },
 )
@@ -2660,30 +2326,19 @@
         "VersionId": str,
         "ExpectedBucketOwner": str,
         "RequestPayer": Literal["requester"],
     },
     total=False,
 )
 
-
 class GetObjectTaggingRequestRequestTypeDef(
     _RequiredGetObjectTaggingRequestRequestTypeDef, _OptionalGetObjectTaggingRequestRequestTypeDef
 ):
     pass
 
-
-GetObjectTorrentOutputTypeDef = TypedDict(
-    "GetObjectTorrentOutputTypeDef",
-    {
-        "Body": StreamingBody,
-        "RequestCharged": Literal["requester"],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetObjectTorrentRequestRequestTypeDef = TypedDict(
     "_RequiredGetObjectTorrentRequestRequestTypeDef",
     {
         "Bucket": str,
         "Key": str,
     },
 )
@@ -2692,30 +2347,27 @@
     {
         "RequestPayer": Literal["requester"],
         "ExpectedBucketOwner": str,
     },
     total=False,
 )
 
-
 class GetObjectTorrentRequestRequestTypeDef(
     _RequiredGetObjectTorrentRequestRequestTypeDef, _OptionalGetObjectTorrentRequestRequestTypeDef
 ):
     pass
 
-
 PublicAccessBlockConfigurationTypeDef = TypedDict(
     "PublicAccessBlockConfigurationTypeDef",
     {
         "BlockPublicAcls": bool,
         "IgnorePublicAcls": bool,
         "BlockPublicPolicy": bool,
         "RestrictPublicBuckets": bool,
     },
-    total=False,
 )
 
 _RequiredGetPublicAccessBlockRequestRequestTypeDef = TypedDict(
     "_RequiredGetPublicAccessBlockRequestRequestTypeDef",
     {
         "Bucket": str,
     },
@@ -2724,51 +2376,38 @@
     "_OptionalGetPublicAccessBlockRequestRequestTypeDef",
     {
         "ExpectedBucketOwner": str,
     },
     total=False,
 )
 
-
 class GetPublicAccessBlockRequestRequestTypeDef(
     _RequiredGetPublicAccessBlockRequestRequestTypeDef,
     _OptionalGetPublicAccessBlockRequestRequestTypeDef,
 ):
     pass
 
-
 GlacierJobParametersTypeDef = TypedDict(
     "GlacierJobParametersTypeDef",
     {
         "Tier": TierType,
     },
 )
 
-_RequiredGranteeTypeDef = TypedDict(
-    "_RequiredGranteeTypeDef",
-    {
-        "Type": TypeType,
-    },
-)
-_OptionalGranteeTypeDef = TypedDict(
-    "_OptionalGranteeTypeDef",
+GranteeTypeDef = TypedDict(
+    "GranteeTypeDef",
     {
         "DisplayName": str,
         "EmailAddress": str,
         "ID": str,
+        "Type": TypeType,
         "URI": str,
     },
-    total=False,
 )
 
-
-class GranteeTypeDef(_RequiredGranteeTypeDef, _OptionalGranteeTypeDef):
-    pass
-
-
 WaiterConfigTypeDef = TypedDict(
     "WaiterConfigTypeDef",
     {
         "Delay": int,
         "MaxAttempts": int,
     },
     total=False,
@@ -2784,62 +2423,19 @@
     "_OptionalHeadBucketRequestRequestTypeDef",
     {
         "ExpectedBucketOwner": str,
     },
     total=False,
 )
 
-
 class HeadBucketRequestRequestTypeDef(
     _RequiredHeadBucketRequestRequestTypeDef, _OptionalHeadBucketRequestRequestTypeDef
 ):
     pass
 
-
-HeadObjectOutputTypeDef = TypedDict(
-    "HeadObjectOutputTypeDef",
-    {
-        "DeleteMarker": bool,
-        "AcceptRanges": str,
-        "Expiration": str,
-        "Restore": str,
-        "ArchiveStatus": ArchiveStatusType,
-        "LastModified": datetime,
-        "ContentLength": int,
-        "ChecksumCRC32": str,
-        "ChecksumCRC32C": str,
-        "ChecksumSHA1": str,
-        "ChecksumSHA256": str,
-        "ETag": str,
-        "MissingMeta": int,
-        "VersionId": str,
-        "CacheControl": str,
-        "ContentDisposition": str,
-        "ContentEncoding": str,
-        "ContentLanguage": str,
-        "ContentType": str,
-        "Expires": datetime,
-        "WebsiteRedirectLocation": str,
-        "ServerSideEncryption": ServerSideEncryptionType,
-        "Metadata": Dict[str, str],
-        "SSECustomerAlgorithm": str,
-        "SSECustomerKeyMD5": str,
-        "SSEKMSKeyId": str,
-        "BucketKeyEnabled": bool,
-        "StorageClass": StorageClassType,
-        "RequestCharged": Literal["requester"],
-        "ReplicationStatus": ReplicationStatusType,
-        "PartsCount": int,
-        "ObjectLockMode": ObjectLockModeType,
-        "ObjectLockRetainUntilDate": datetime,
-        "ObjectLockLegalHoldStatus": ObjectLockLegalHoldStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 HeadObjectRequestObjectVersionHeadTypeDef = TypedDict(
     "HeadObjectRequestObjectVersionHeadTypeDef",
     {
         "IfMatch": str,
         "IfModifiedSince": Union[datetime, str],
         "IfNoneMatch": str,
         "IfUnmodifiedSince": Union[datetime, str],
@@ -2878,45 +2474,25 @@
         "PartNumber": int,
         "ExpectedBucketOwner": str,
         "ChecksumMode": Literal["ENABLED"],
     },
     total=False,
 )
 
-
 class HeadObjectRequestRequestTypeDef(
     _RequiredHeadObjectRequestRequestTypeDef, _OptionalHeadObjectRequestRequestTypeDef
 ):
     pass
 
-
-IndexDocumentResponseMetadataTypeDef = TypedDict(
-    "IndexDocumentResponseMetadataTypeDef",
-    {
-        "Suffix": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-InitiatorResponseMetadataTypeDef = TypedDict(
-    "InitiatorResponseMetadataTypeDef",
-    {
-        "ID": str,
-        "DisplayName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 InitiatorTypeDef = TypedDict(
     "InitiatorTypeDef",
     {
         "ID": str,
         "DisplayName": str,
     },
-    total=False,
 )
 
 JSONInputTypeDef = TypedDict(
     "JSONInputTypeDef",
     {
         "Type": JSONTypeType,
     },
@@ -2963,44 +2539,40 @@
 LifecycleExpirationTypeDef = TypedDict(
     "LifecycleExpirationTypeDef",
     {
         "Date": datetime,
         "Days": int,
         "ExpiredObjectDeleteMarker": bool,
     },
-    total=False,
 )
 
 NoncurrentVersionExpirationTypeDef = TypedDict(
     "NoncurrentVersionExpirationTypeDef",
     {
         "NoncurrentDays": int,
         "NewerNoncurrentVersions": int,
     },
-    total=False,
 )
 
 NoncurrentVersionTransitionTypeDef = TypedDict(
     "NoncurrentVersionTransitionTypeDef",
     {
         "NoncurrentDays": int,
         "StorageClass": TransitionStorageClassType,
         "NewerNoncurrentVersions": int,
     },
-    total=False,
 )
 
 TransitionTypeDef = TypedDict(
     "TransitionTypeDef",
     {
         "Date": datetime,
         "Days": int,
         "StorageClass": TransitionStorageClassType,
     },
-    total=False,
 )
 
 _RequiredListBucketAnalyticsConfigurationsRequestRequestTypeDef = TypedDict(
     "_RequiredListBucketAnalyticsConfigurationsRequestRequestTypeDef",
     {
         "Bucket": str,
     },
@@ -3010,44 +2582,40 @@
     {
         "ContinuationToken": str,
         "ExpectedBucketOwner": str,
     },
     total=False,
 )
 
-
 class ListBucketAnalyticsConfigurationsRequestRequestTypeDef(
     _RequiredListBucketAnalyticsConfigurationsRequestRequestTypeDef,
     _OptionalListBucketAnalyticsConfigurationsRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredListBucketIntelligentTieringConfigurationsRequestRequestTypeDef = TypedDict(
     "_RequiredListBucketIntelligentTieringConfigurationsRequestRequestTypeDef",
     {
         "Bucket": str,
     },
 )
 _OptionalListBucketIntelligentTieringConfigurationsRequestRequestTypeDef = TypedDict(
     "_OptionalListBucketIntelligentTieringConfigurationsRequestRequestTypeDef",
     {
         "ContinuationToken": str,
     },
     total=False,
 )
 
-
 class ListBucketIntelligentTieringConfigurationsRequestRequestTypeDef(
     _RequiredListBucketIntelligentTieringConfigurationsRequestRequestTypeDef,
     _OptionalListBucketIntelligentTieringConfigurationsRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredListBucketInventoryConfigurationsRequestRequestTypeDef = TypedDict(
     "_RequiredListBucketInventoryConfigurationsRequestRequestTypeDef",
     {
         "Bucket": str,
     },
 )
 _OptionalListBucketInventoryConfigurationsRequestRequestTypeDef = TypedDict(
@@ -3055,22 +2623,20 @@
     {
         "ContinuationToken": str,
         "ExpectedBucketOwner": str,
     },
     total=False,
 )
 
-
 class ListBucketInventoryConfigurationsRequestRequestTypeDef(
     _RequiredListBucketInventoryConfigurationsRequestRequestTypeDef,
     _OptionalListBucketInventoryConfigurationsRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredListBucketMetricsConfigurationsRequestRequestTypeDef = TypedDict(
     "_RequiredListBucketMetricsConfigurationsRequestRequestTypeDef",
     {
         "Bucket": str,
     },
 )
 _OptionalListBucketMetricsConfigurationsRequestRequestTypeDef = TypedDict(
@@ -3078,49 +2644,30 @@
     {
         "ContinuationToken": str,
         "ExpectedBucketOwner": str,
     },
     total=False,
 )
 
-
 class ListBucketMetricsConfigurationsRequestRequestTypeDef(
     _RequiredListBucketMetricsConfigurationsRequestRequestTypeDef,
     _OptionalListBucketMetricsConfigurationsRequestRequestTypeDef,
 ):
     pass
 
-
-_RequiredListMultipartUploadsRequestListMultipartUploadsPaginateTypeDef = TypedDict(
-    "_RequiredListMultipartUploadsRequestListMultipartUploadsPaginateTypeDef",
-    {
-        "Bucket": str,
-    },
-)
-_OptionalListMultipartUploadsRequestListMultipartUploadsPaginateTypeDef = TypedDict(
-    "_OptionalListMultipartUploadsRequestListMultipartUploadsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "Delimiter": str,
-        "EncodingType": Literal["url"],
-        "Prefix": str,
-        "ExpectedBucketOwner": str,
-        "RequestPayer": Literal["requester"],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
-
-class ListMultipartUploadsRequestListMultipartUploadsPaginateTypeDef(
-    _RequiredListMultipartUploadsRequestListMultipartUploadsPaginateTypeDef,
-    _OptionalListMultipartUploadsRequestListMultipartUploadsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListMultipartUploadsRequestRequestTypeDef = TypedDict(
     "_RequiredListMultipartUploadsRequestRequestTypeDef",
     {
         "Bucket": str,
     },
 )
 _OptionalListMultipartUploadsRequestRequestTypeDef = TypedDict(
@@ -3134,50 +2681,20 @@
         "UploadIdMarker": str,
         "ExpectedBucketOwner": str,
         "RequestPayer": Literal["requester"],
     },
     total=False,
 )
 
-
 class ListMultipartUploadsRequestRequestTypeDef(
     _RequiredListMultipartUploadsRequestRequestTypeDef,
     _OptionalListMultipartUploadsRequestRequestTypeDef,
 ):
     pass
 
-
-_RequiredListObjectVersionsRequestListObjectVersionsPaginateTypeDef = TypedDict(
-    "_RequiredListObjectVersionsRequestListObjectVersionsPaginateTypeDef",
-    {
-        "Bucket": str,
-    },
-)
-_OptionalListObjectVersionsRequestListObjectVersionsPaginateTypeDef = TypedDict(
-    "_OptionalListObjectVersionsRequestListObjectVersionsPaginateTypeDef",
-    {
-        "Delimiter": str,
-        "EncodingType": Literal["url"],
-        "Prefix": str,
-        "ExpectedBucketOwner": str,
-        "RequestPayer": Literal["requester"],
-        "OptionalObjectAttributes": Sequence[Literal["RestoreStatus"]],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListObjectVersionsRequestListObjectVersionsPaginateTypeDef(
-    _RequiredListObjectVersionsRequestListObjectVersionsPaginateTypeDef,
-    _OptionalListObjectVersionsRequestListObjectVersionsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListObjectVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredListObjectVersionsRequestRequestTypeDef",
     {
         "Bucket": str,
     },
 )
 _OptionalListObjectVersionsRequestRequestTypeDef = TypedDict(
@@ -3192,50 +2709,20 @@
         "ExpectedBucketOwner": str,
         "RequestPayer": Literal["requester"],
         "OptionalObjectAttributes": Sequence[Literal["RestoreStatus"]],
     },
     total=False,
 )
 
-
 class ListObjectVersionsRequestRequestTypeDef(
     _RequiredListObjectVersionsRequestRequestTypeDef,
     _OptionalListObjectVersionsRequestRequestTypeDef,
 ):
     pass
 
-
-_RequiredListObjectsRequestListObjectsPaginateTypeDef = TypedDict(
-    "_RequiredListObjectsRequestListObjectsPaginateTypeDef",
-    {
-        "Bucket": str,
-    },
-)
-_OptionalListObjectsRequestListObjectsPaginateTypeDef = TypedDict(
-    "_OptionalListObjectsRequestListObjectsPaginateTypeDef",
-    {
-        "Delimiter": str,
-        "EncodingType": Literal["url"],
-        "Prefix": str,
-        "RequestPayer": Literal["requester"],
-        "ExpectedBucketOwner": str,
-        "OptionalObjectAttributes": Sequence[Literal["RestoreStatus"]],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListObjectsRequestListObjectsPaginateTypeDef(
-    _RequiredListObjectsRequestListObjectsPaginateTypeDef,
-    _OptionalListObjectsRequestListObjectsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListObjectsRequestRequestTypeDef = TypedDict(
     "_RequiredListObjectsRequestRequestTypeDef",
     {
         "Bucket": str,
     },
 )
 _OptionalListObjectsRequestRequestTypeDef = TypedDict(
@@ -3249,51 +2736,19 @@
         "RequestPayer": Literal["requester"],
         "ExpectedBucketOwner": str,
         "OptionalObjectAttributes": Sequence[Literal["RestoreStatus"]],
     },
     total=False,
 )
 
-
 class ListObjectsRequestRequestTypeDef(
     _RequiredListObjectsRequestRequestTypeDef, _OptionalListObjectsRequestRequestTypeDef
 ):
     pass
 
-
-_RequiredListObjectsV2RequestListObjectsV2PaginateTypeDef = TypedDict(
-    "_RequiredListObjectsV2RequestListObjectsV2PaginateTypeDef",
-    {
-        "Bucket": str,
-    },
-)
-_OptionalListObjectsV2RequestListObjectsV2PaginateTypeDef = TypedDict(
-    "_OptionalListObjectsV2RequestListObjectsV2PaginateTypeDef",
-    {
-        "Delimiter": str,
-        "EncodingType": Literal["url"],
-        "Prefix": str,
-        "FetchOwner": bool,
-        "StartAfter": str,
-        "RequestPayer": Literal["requester"],
-        "ExpectedBucketOwner": str,
-        "OptionalObjectAttributes": Sequence[Literal["RestoreStatus"]],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListObjectsV2RequestListObjectsV2PaginateTypeDef(
-    _RequiredListObjectsV2RequestListObjectsV2PaginateTypeDef,
-    _OptionalListObjectsV2RequestListObjectsV2PaginateTypeDef,
-):
-    pass
-
-
 _RequiredListObjectsV2RequestRequestTypeDef = TypedDict(
     "_RequiredListObjectsV2RequestRequestTypeDef",
     {
         "Bucket": str,
     },
 )
 _OptionalListObjectsV2RequestRequestTypeDef = TypedDict(
@@ -3309,65 +2764,33 @@
         "RequestPayer": Literal["requester"],
         "ExpectedBucketOwner": str,
         "OptionalObjectAttributes": Sequence[Literal["RestoreStatus"]],
     },
     total=False,
 )
 
-
 class ListObjectsV2RequestRequestTypeDef(
     _RequiredListObjectsV2RequestRequestTypeDef, _OptionalListObjectsV2RequestRequestTypeDef
 ):
     pass
 
-
 PartTypeDef = TypedDict(
     "PartTypeDef",
     {
         "PartNumber": int,
         "LastModified": datetime,
         "ETag": str,
         "Size": int,
         "ChecksumCRC32": str,
         "ChecksumCRC32C": str,
         "ChecksumSHA1": str,
         "ChecksumSHA256": str,
     },
-    total=False,
 )
 
-_RequiredListPartsRequestListPartsPaginateTypeDef = TypedDict(
-    "_RequiredListPartsRequestListPartsPaginateTypeDef",
-    {
-        "Bucket": str,
-        "Key": str,
-        "UploadId": str,
-    },
-)
-_OptionalListPartsRequestListPartsPaginateTypeDef = TypedDict(
-    "_OptionalListPartsRequestListPartsPaginateTypeDef",
-    {
-        "RequestPayer": Literal["requester"],
-        "ExpectedBucketOwner": str,
-        "SSECustomerAlgorithm": str,
-        "SSECustomerKey": str,
-        "SSECustomerKeyMD5": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListPartsRequestListPartsPaginateTypeDef(
-    _RequiredListPartsRequestListPartsPaginateTypeDef,
-    _OptionalListPartsRequestListPartsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListPartsRequestRequestTypeDef = TypedDict(
     "_RequiredListPartsRequestRequestTypeDef",
     {
         "Bucket": str,
         "Key": str,
         "UploadId": str,
     },
@@ -3382,58 +2805,53 @@
         "SSECustomerAlgorithm": str,
         "SSECustomerKey": str,
         "SSECustomerKeyMD5": str,
     },
     total=False,
 )
 
-
 class ListPartsRequestRequestTypeDef(
     _RequiredListPartsRequestRequestTypeDef, _OptionalListPartsRequestRequestTypeDef
 ):
     pass
 
-
 MetadataEntryTypeDef = TypedDict(
     "MetadataEntryTypeDef",
     {
         "Name": str,
         "Value": str,
     },
     total=False,
 )
 
 ReplicationTimeValueTypeDef = TypedDict(
     "ReplicationTimeValueTypeDef",
     {
         "Minutes": int,
     },
-    total=False,
 )
 
 QueueConfigurationDeprecatedTypeDef = TypedDict(
     "QueueConfigurationDeprecatedTypeDef",
     {
         "Id": str,
         "Event": EventType,
         "Events": List[EventType],
         "Queue": str,
     },
-    total=False,
 )
 
 TopicConfigurationDeprecatedTypeDef = TypedDict(
     "TopicConfigurationDeprecatedTypeDef",
     {
         "Id": str,
         "Events": List[EventType],
         "Event": EventType,
         "Topic": str,
     },
-    total=False,
 )
 
 _RequiredObjectDownloadFileRequestTypeDef = TypedDict(
     "_RequiredObjectDownloadFileRequestTypeDef",
     {
         "Filename": str,
     },
@@ -3444,21 +2862,19 @@
         "ExtraArgs": Dict[str, Any],
         "Callback": Callable[..., Any],
         "Config": TransferConfig,
     },
     total=False,
 )
 
-
 class ObjectDownloadFileRequestTypeDef(
     _RequiredObjectDownloadFileRequestTypeDef, _OptionalObjectDownloadFileRequestTypeDef
 ):
     pass
 
-
 _RequiredObjectDownloadFileobjRequestTypeDef = TypedDict(
     "_RequiredObjectDownloadFileobjRequestTypeDef",
     {
         "Fileobj": Union[IO[Any], StreamingBody],
     },
 )
 _OptionalObjectDownloadFileobjRequestTypeDef = TypedDict(
@@ -3467,28 +2883,25 @@
         "ExtraArgs": Dict[str, Any],
         "Callback": Callable[..., Any],
         "Config": TransferConfig,
     },
     total=False,
 )
 
-
 class ObjectDownloadFileobjRequestTypeDef(
     _RequiredObjectDownloadFileobjRequestTypeDef, _OptionalObjectDownloadFileobjRequestTypeDef
 ):
     pass
 
-
 RestoreStatusTypeDef = TypedDict(
     "RestoreStatusTypeDef",
     {
         "IsRestoreInProgress": bool,
         "RestoreExpiryDate": datetime,
     },
-    total=False,
 )
 
 _RequiredObjectUploadFileRequestTypeDef = TypedDict(
     "_RequiredObjectUploadFileRequestTypeDef",
     {
         "Filename": str,
     },
@@ -3499,21 +2912,19 @@
         "ExtraArgs": Dict[str, Any],
         "Callback": Callable[..., Any],
         "Config": TransferConfig,
     },
     total=False,
 )
 
-
 class ObjectUploadFileRequestTypeDef(
     _RequiredObjectUploadFileRequestTypeDef, _OptionalObjectUploadFileRequestTypeDef
 ):
     pass
 
-
 _RequiredObjectUploadFileobjRequestTypeDef = TypedDict(
     "_RequiredObjectUploadFileobjRequestTypeDef",
     {
         "Fileobj": Union[IO[Any], StreamingBody],
     },
 )
 _OptionalObjectUploadFileobjRequestTypeDef = TypedDict(
@@ -3522,55 +2933,33 @@
         "ExtraArgs": Dict[str, Any],
         "Callback": Callable[..., Any],
         "Config": TransferConfig,
     },
     total=False,
 )
 
-
 class ObjectUploadFileobjRequestTypeDef(
     _RequiredObjectUploadFileobjRequestTypeDef, _OptionalObjectUploadFileobjRequestTypeDef
 ):
     pass
 
-
-OwnerResponseMetadataTypeDef = TypedDict(
-    "OwnerResponseMetadataTypeDef",
-    {
-        "DisplayName": str,
-        "ID": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 OwnershipControlsRuleTypeDef = TypedDict(
     "OwnershipControlsRuleTypeDef",
     {
         "ObjectOwnership": ObjectOwnershipType,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
-    {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
-    },
-    total=False,
-)
-
 ProgressTypeDef = TypedDict(
     "ProgressTypeDef",
     {
         "BytesScanned": int,
         "BytesProcessed": int,
         "BytesReturned": int,
     },
-    total=False,
 )
 
 _RequiredPutBucketPolicyRequestBucketPolicyPutTypeDef = TypedDict(
     "_RequiredPutBucketPolicyRequestBucketPolicyPutTypeDef",
     {
         "Policy": str,
     },
@@ -3581,22 +2970,20 @@
         "ChecksumAlgorithm": ChecksumAlgorithmType,
         "ConfirmRemoveSelfBucketAccess": bool,
         "ExpectedBucketOwner": str,
     },
     total=False,
 )
 
-
 class PutBucketPolicyRequestBucketPolicyPutTypeDef(
     _RequiredPutBucketPolicyRequestBucketPolicyPutTypeDef,
     _OptionalPutBucketPolicyRequestBucketPolicyPutTypeDef,
 ):
     pass
 
-
 _RequiredPutBucketPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredPutBucketPolicyRequestRequestTypeDef",
     {
         "Bucket": str,
         "Policy": str,
     },
 )
@@ -3606,21 +2993,19 @@
         "ChecksumAlgorithm": ChecksumAlgorithmType,
         "ConfirmRemoveSelfBucketAccess": bool,
         "ExpectedBucketOwner": str,
     },
     total=False,
 )
 
-
 class PutBucketPolicyRequestRequestTypeDef(
     _RequiredPutBucketPolicyRequestRequestTypeDef, _OptionalPutBucketPolicyRequestRequestTypeDef
 ):
     pass
 
-
 RequestPaymentConfigurationTypeDef = TypedDict(
     "RequestPaymentConfigurationTypeDef",
     {
         "Payer": PayerType,
     },
 )
 
@@ -3649,59 +3034,14 @@
         "ChecksumAlgorithm": ChecksumAlgorithmType,
         "MFA": str,
         "ExpectedBucketOwner": str,
     },
     total=False,
 )
 
-PutObjectAclOutputTypeDef = TypedDict(
-    "PutObjectAclOutputTypeDef",
-    {
-        "RequestCharged": Literal["requester"],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-PutObjectLegalHoldOutputTypeDef = TypedDict(
-    "PutObjectLegalHoldOutputTypeDef",
-    {
-        "RequestCharged": Literal["requester"],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-PutObjectLockConfigurationOutputTypeDef = TypedDict(
-    "PutObjectLockConfigurationOutputTypeDef",
-    {
-        "RequestCharged": Literal["requester"],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-PutObjectOutputTypeDef = TypedDict(
-    "PutObjectOutputTypeDef",
-    {
-        "Expiration": str,
-        "ETag": str,
-        "ChecksumCRC32": str,
-        "ChecksumCRC32C": str,
-        "ChecksumSHA1": str,
-        "ChecksumSHA256": str,
-        "ServerSideEncryption": ServerSideEncryptionType,
-        "VersionId": str,
-        "SSECustomerAlgorithm": str,
-        "SSECustomerKeyMD5": str,
-        "SSEKMSKeyId": str,
-        "SSEKMSEncryptionContext": str,
-        "BucketKeyEnabled": bool,
-        "RequestCharged": Literal["requester"],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredPutObjectRequestBucketPutObjectTypeDef = TypedDict(
     "_RequiredPutObjectRequestBucketPutObjectTypeDef",
     {
         "Key": str,
     },
 )
 _OptionalPutObjectRequestBucketPutObjectTypeDef = TypedDict(
@@ -3742,21 +3082,19 @@
         "ObjectLockRetainUntilDate": Union[datetime, str],
         "ObjectLockLegalHoldStatus": ObjectLockLegalHoldStatusType,
         "ExpectedBucketOwner": str,
     },
     total=False,
 )
 
-
 class PutObjectRequestBucketPutObjectTypeDef(
     _RequiredPutObjectRequestBucketPutObjectTypeDef, _OptionalPutObjectRequestBucketPutObjectTypeDef
 ):
     pass
 
-
 PutObjectRequestObjectPutTypeDef = TypedDict(
     "PutObjectRequestObjectPutTypeDef",
     {
         "ACL": ObjectCannedACLType,
         "Body": Union[str, bytes, IO[Any], StreamingBody],
         "CacheControl": str,
         "ContentDisposition": str,
@@ -3882,64 +3220,35 @@
         "ObjectLockRetainUntilDate": Union[datetime, str],
         "ObjectLockLegalHoldStatus": ObjectLockLegalHoldStatusType,
         "ExpectedBucketOwner": str,
     },
     total=False,
 )
 
-
 class PutObjectRequestRequestTypeDef(
     _RequiredPutObjectRequestRequestTypeDef, _OptionalPutObjectRequestRequestTypeDef
 ):
     pass
 
-
-PutObjectRetentionOutputTypeDef = TypedDict(
-    "PutObjectRetentionOutputTypeDef",
-    {
-        "RequestCharged": Literal["requester"],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-PutObjectTaggingOutputTypeDef = TypedDict(
-    "PutObjectTaggingOutputTypeDef",
-    {
-        "VersionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 RecordsEventTypeDef = TypedDict(
     "RecordsEventTypeDef",
     {
         "Payload": bytes,
     },
-    total=False,
-)
-
-RedirectAllRequestsToResponseMetadataTypeDef = TypedDict(
-    "RedirectAllRequestsToResponseMetadataTypeDef",
-    {
-        "HostName": str,
-        "Protocol": ProtocolType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
 )
 
 RedirectTypeDef = TypedDict(
     "RedirectTypeDef",
     {
         "HostName": str,
         "HttpRedirectCode": str,
         "Protocol": ProtocolType,
         "ReplaceKeyPrefixWith": str,
         "ReplaceKeyWith": str,
     },
-    total=False,
 )
 
 ReplicaModificationsTypeDef = TypedDict(
     "ReplicaModificationsTypeDef",
     {
         "Status": ReplicaModificationsStatusType,
     },
@@ -3949,106 +3258,45 @@
     "RequestProgressTypeDef",
     {
         "Enabled": bool,
     },
     total=False,
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
-RestoreObjectOutputTypeDef = TypedDict(
-    "RestoreObjectOutputTypeDef",
-    {
-        "RequestCharged": Literal["requester"],
-        "RestoreOutputPath": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-RestoreStatusResponseMetadataTypeDef = TypedDict(
-    "RestoreStatusResponseMetadataTypeDef",
-    {
-        "IsRestoreInProgress": bool,
-        "RestoreExpiryDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ScanRangeTypeDef = TypedDict(
     "ScanRangeTypeDef",
     {
         "Start": int,
         "End": int,
     },
     total=False,
 )
 
-_RequiredServerSideEncryptionByDefaultTypeDef = TypedDict(
-    "_RequiredServerSideEncryptionByDefaultTypeDef",
+ServerSideEncryptionByDefaultTypeDef = TypedDict(
+    "ServerSideEncryptionByDefaultTypeDef",
     {
         "SSEAlgorithm": ServerSideEncryptionType,
-    },
-)
-_OptionalServerSideEncryptionByDefaultTypeDef = TypedDict(
-    "_OptionalServerSideEncryptionByDefaultTypeDef",
-    {
         "KMSMasterKeyID": str,
     },
-    total=False,
 )
 
-
-class ServerSideEncryptionByDefaultTypeDef(
-    _RequiredServerSideEncryptionByDefaultTypeDef, _OptionalServerSideEncryptionByDefaultTypeDef
-):
-    pass
-
-
 SseKmsEncryptedObjectsTypeDef = TypedDict(
     "SseKmsEncryptedObjectsTypeDef",
     {
         "Status": SseKmsEncryptedObjectsStatusType,
     },
 )
 
 StatsTypeDef = TypedDict(
     "StatsTypeDef",
     {
         "BytesScanned": int,
         "BytesProcessed": int,
         "BytesReturned": int,
     },
-    total=False,
-)
-
-UploadPartOutputTypeDef = TypedDict(
-    "UploadPartOutputTypeDef",
-    {
-        "ServerSideEncryption": ServerSideEncryptionType,
-        "ETag": str,
-        "ChecksumCRC32": str,
-        "ChecksumCRC32C": str,
-        "ChecksumSHA1": str,
-        "ChecksumSHA256": str,
-        "SSECustomerAlgorithm": str,
-        "SSECustomerKeyMD5": str,
-        "SSEKMSKeyId": str,
-        "BucketKeyEnabled": bool,
-        "RequestCharged": Literal["requester"],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
 )
 
 UploadPartRequestMultipartUploadPartUploadTypeDef = TypedDict(
     "UploadPartRequestMultipartUploadPartUploadTypeDef",
     {
         "Body": Union[str, bytes, IO[Any], StreamingBody],
         "ContentLength": int,
@@ -4092,21 +3340,19 @@
         "SSECustomerKeyMD5": str,
         "RequestPayer": Literal["requester"],
         "ExpectedBucketOwner": str,
     },
     total=False,
 )
 
-
 class UploadPartRequestRequestTypeDef(
     _RequiredUploadPartRequestRequestTypeDef, _OptionalUploadPartRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredWriteGetObjectResponseRequestRequestTypeDef = TypedDict(
     "_RequiredWriteGetObjectResponseRequestRequestTypeDef",
     {
         "RequestRoute": str,
         "RequestToken": str,
     },
 )
@@ -4151,21 +3397,376 @@
         "TagCount": int,
         "VersionId": str,
         "BucketKeyEnabled": bool,
     },
     total=False,
 )
 
-
 class WriteGetObjectResponseRequestRequestTypeDef(
     _RequiredWriteGetObjectResponseRequestRequestTypeDef,
     _OptionalWriteGetObjectResponseRequestRequestTypeDef,
 ):
     pass
 
+AbortMultipartUploadOutputTypeDef = TypedDict(
+    "AbortMultipartUploadOutputTypeDef",
+    {
+        "RequestCharged": Literal["requester"],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CompleteMultipartUploadOutputTypeDef = TypedDict(
+    "CompleteMultipartUploadOutputTypeDef",
+    {
+        "Location": str,
+        "Bucket": str,
+        "Key": str,
+        "Expiration": str,
+        "ETag": str,
+        "ChecksumCRC32": str,
+        "ChecksumCRC32C": str,
+        "ChecksumSHA1": str,
+        "ChecksumSHA256": str,
+        "ServerSideEncryption": ServerSideEncryptionType,
+        "VersionId": str,
+        "SSEKMSKeyId": str,
+        "BucketKeyEnabled": bool,
+        "RequestCharged": Literal["requester"],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateBucketOutputTypeDef = TypedDict(
+    "CreateBucketOutputTypeDef",
+    {
+        "Location": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateMultipartUploadOutputTypeDef = TypedDict(
+    "CreateMultipartUploadOutputTypeDef",
+    {
+        "AbortDate": datetime,
+        "AbortRuleId": str,
+        "Bucket": str,
+        "Key": str,
+        "UploadId": str,
+        "ServerSideEncryption": ServerSideEncryptionType,
+        "SSECustomerAlgorithm": str,
+        "SSECustomerKeyMD5": str,
+        "SSEKMSKeyId": str,
+        "SSEKMSEncryptionContext": str,
+        "BucketKeyEnabled": bool,
+        "RequestCharged": Literal["requester"],
+        "ChecksumAlgorithm": ChecksumAlgorithmType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteObjectOutputTypeDef = TypedDict(
+    "DeleteObjectOutputTypeDef",
+    {
+        "DeleteMarker": bool,
+        "VersionId": str,
+        "RequestCharged": Literal["requester"],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteObjectTaggingOutputTypeDef = TypedDict(
+    "DeleteObjectTaggingOutputTypeDef",
+    {
+        "VersionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ErrorDocumentResponseMetadataTypeDef = TypedDict(
+    "ErrorDocumentResponseMetadataTypeDef",
+    {
+        "Key": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetBucketAccelerateConfigurationOutputTypeDef = TypedDict(
+    "GetBucketAccelerateConfigurationOutputTypeDef",
+    {
+        "Status": BucketAccelerateStatusType,
+        "RequestCharged": Literal["requester"],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetBucketLocationOutputTypeDef = TypedDict(
+    "GetBucketLocationOutputTypeDef",
+    {
+        "LocationConstraint": BucketLocationConstraintType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetBucketPolicyOutputTypeDef = TypedDict(
+    "GetBucketPolicyOutputTypeDef",
+    {
+        "Policy": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetBucketRequestPaymentOutputTypeDef = TypedDict(
+    "GetBucketRequestPaymentOutputTypeDef",
+    {
+        "Payer": PayerType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetBucketVersioningOutputTypeDef = TypedDict(
+    "GetBucketVersioningOutputTypeDef",
+    {
+        "Status": BucketVersioningStatusType,
+        "MFADelete": MFADeleteStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetObjectOutputTypeDef = TypedDict(
+    "GetObjectOutputTypeDef",
+    {
+        "Body": StreamingBody,
+        "DeleteMarker": bool,
+        "AcceptRanges": str,
+        "Expiration": str,
+        "Restore": str,
+        "LastModified": datetime,
+        "ContentLength": int,
+        "ETag": str,
+        "ChecksumCRC32": str,
+        "ChecksumCRC32C": str,
+        "ChecksumSHA1": str,
+        "ChecksumSHA256": str,
+        "MissingMeta": int,
+        "VersionId": str,
+        "CacheControl": str,
+        "ContentDisposition": str,
+        "ContentEncoding": str,
+        "ContentLanguage": str,
+        "ContentRange": str,
+        "ContentType": str,
+        "Expires": datetime,
+        "WebsiteRedirectLocation": str,
+        "ServerSideEncryption": ServerSideEncryptionType,
+        "Metadata": Dict[str, str],
+        "SSECustomerAlgorithm": str,
+        "SSECustomerKeyMD5": str,
+        "SSEKMSKeyId": str,
+        "BucketKeyEnabled": bool,
+        "StorageClass": StorageClassType,
+        "RequestCharged": Literal["requester"],
+        "ReplicationStatus": ReplicationStatusType,
+        "PartsCount": int,
+        "TagCount": int,
+        "ObjectLockMode": ObjectLockModeType,
+        "ObjectLockRetainUntilDate": datetime,
+        "ObjectLockLegalHoldStatus": ObjectLockLegalHoldStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetObjectTorrentOutputTypeDef = TypedDict(
+    "GetObjectTorrentOutputTypeDef",
+    {
+        "Body": StreamingBody,
+        "RequestCharged": Literal["requester"],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+HeadObjectOutputTypeDef = TypedDict(
+    "HeadObjectOutputTypeDef",
+    {
+        "DeleteMarker": bool,
+        "AcceptRanges": str,
+        "Expiration": str,
+        "Restore": str,
+        "ArchiveStatus": ArchiveStatusType,
+        "LastModified": datetime,
+        "ContentLength": int,
+        "ChecksumCRC32": str,
+        "ChecksumCRC32C": str,
+        "ChecksumSHA1": str,
+        "ChecksumSHA256": str,
+        "ETag": str,
+        "MissingMeta": int,
+        "VersionId": str,
+        "CacheControl": str,
+        "ContentDisposition": str,
+        "ContentEncoding": str,
+        "ContentLanguage": str,
+        "ContentType": str,
+        "Expires": datetime,
+        "WebsiteRedirectLocation": str,
+        "ServerSideEncryption": ServerSideEncryptionType,
+        "Metadata": Dict[str, str],
+        "SSECustomerAlgorithm": str,
+        "SSECustomerKeyMD5": str,
+        "SSEKMSKeyId": str,
+        "BucketKeyEnabled": bool,
+        "StorageClass": StorageClassType,
+        "RequestCharged": Literal["requester"],
+        "ReplicationStatus": ReplicationStatusType,
+        "PartsCount": int,
+        "ObjectLockMode": ObjectLockModeType,
+        "ObjectLockRetainUntilDate": datetime,
+        "ObjectLockLegalHoldStatus": ObjectLockLegalHoldStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+IndexDocumentResponseMetadataTypeDef = TypedDict(
+    "IndexDocumentResponseMetadataTypeDef",
+    {
+        "Suffix": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+InitiatorResponseMetadataTypeDef = TypedDict(
+    "InitiatorResponseMetadataTypeDef",
+    {
+        "ID": str,
+        "DisplayName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+OwnerResponseMetadataTypeDef = TypedDict(
+    "OwnerResponseMetadataTypeDef",
+    {
+        "DisplayName": str,
+        "ID": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutObjectAclOutputTypeDef = TypedDict(
+    "PutObjectAclOutputTypeDef",
+    {
+        "RequestCharged": Literal["requester"],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutObjectLegalHoldOutputTypeDef = TypedDict(
+    "PutObjectLegalHoldOutputTypeDef",
+    {
+        "RequestCharged": Literal["requester"],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutObjectLockConfigurationOutputTypeDef = TypedDict(
+    "PutObjectLockConfigurationOutputTypeDef",
+    {
+        "RequestCharged": Literal["requester"],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutObjectOutputTypeDef = TypedDict(
+    "PutObjectOutputTypeDef",
+    {
+        "Expiration": str,
+        "ETag": str,
+        "ChecksumCRC32": str,
+        "ChecksumCRC32C": str,
+        "ChecksumSHA1": str,
+        "ChecksumSHA256": str,
+        "ServerSideEncryption": ServerSideEncryptionType,
+        "VersionId": str,
+        "SSECustomerAlgorithm": str,
+        "SSECustomerKeyMD5": str,
+        "SSEKMSKeyId": str,
+        "SSEKMSEncryptionContext": str,
+        "BucketKeyEnabled": bool,
+        "RequestCharged": Literal["requester"],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutObjectRetentionOutputTypeDef = TypedDict(
+    "PutObjectRetentionOutputTypeDef",
+    {
+        "RequestCharged": Literal["requester"],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutObjectTaggingOutputTypeDef = TypedDict(
+    "PutObjectTaggingOutputTypeDef",
+    {
+        "VersionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RedirectAllRequestsToResponseMetadataTypeDef = TypedDict(
+    "RedirectAllRequestsToResponseMetadataTypeDef",
+    {
+        "HostName": str,
+        "Protocol": ProtocolType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RestoreObjectOutputTypeDef = TypedDict(
+    "RestoreObjectOutputTypeDef",
+    {
+        "RequestCharged": Literal["requester"],
+        "RestoreOutputPath": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RestoreStatusResponseMetadataTypeDef = TypedDict(
+    "RestoreStatusResponseMetadataTypeDef",
+    {
+        "IsRestoreInProgress": bool,
+        "RestoreExpiryDate": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UploadPartOutputTypeDef = TypedDict(
+    "UploadPartOutputTypeDef",
+    {
+        "ServerSideEncryption": ServerSideEncryptionType,
+        "ETag": str,
+        "ChecksumCRC32": str,
+        "ChecksumCRC32C": str,
+        "ChecksumSHA1": str,
+        "ChecksumSHA256": str,
+        "SSECustomerAlgorithm": str,
+        "SSECustomerKeyMD5": str,
+        "SSEKMSKeyId": str,
+        "BucketKeyEnabled": bool,
+        "RequestCharged": Literal["requester"],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
 _RequiredPutBucketAccelerateConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredPutBucketAccelerateConfigurationRequestRequestTypeDef",
     {
         "Bucket": str,
         "AccelerateConfiguration": AccelerateConfigurationTypeDef,
     },
@@ -4175,97 +3776,89 @@
     {
         "ExpectedBucketOwner": str,
         "ChecksumAlgorithm": ChecksumAlgorithmType,
     },
     total=False,
 )
 
-
 class PutBucketAccelerateConfigurationRequestRequestTypeDef(
     _RequiredPutBucketAccelerateConfigurationRequestRequestTypeDef,
     _OptionalPutBucketAccelerateConfigurationRequestRequestTypeDef,
 ):
     pass
 
-
 DeleteMarkerEntryTypeDef = TypedDict(
     "DeleteMarkerEntryTypeDef",
     {
         "Owner": OwnerTypeDef,
         "Key": str,
         "VersionId": str,
         "IsLatest": bool,
         "LastModified": datetime,
     },
-    total=False,
 )
 
 AnalyticsAndOperatorTypeDef = TypedDict(
     "AnalyticsAndOperatorTypeDef",
     {
         "Prefix": str,
         "Tags": List[TagTypeDef],
     },
-    total=False,
 )
 
 GetBucketTaggingOutputTypeDef = TypedDict(
     "GetBucketTaggingOutputTypeDef",
     {
         "TagSet": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetObjectTaggingOutputTypeDef = TypedDict(
     "GetObjectTaggingOutputTypeDef",
     {
         "VersionId": str,
         "TagSet": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 IntelligentTieringAndOperatorTypeDef = TypedDict(
     "IntelligentTieringAndOperatorTypeDef",
     {
         "Prefix": str,
         "Tags": List[TagTypeDef],
     },
-    total=False,
 )
 
 LifecycleRuleAndOperatorTypeDef = TypedDict(
     "LifecycleRuleAndOperatorTypeDef",
     {
         "Prefix": str,
         "Tags": List[TagTypeDef],
         "ObjectSizeGreaterThan": int,
         "ObjectSizeLessThan": int,
     },
-    total=False,
 )
 
 MetricsAndOperatorTypeDef = TypedDict(
     "MetricsAndOperatorTypeDef",
     {
         "Prefix": str,
         "Tags": List[TagTypeDef],
         "AccessPointArn": str,
     },
-    total=False,
 )
 
 ReplicationRuleAndOperatorTypeDef = TypedDict(
     "ReplicationRuleAndOperatorTypeDef",
     {
         "Prefix": str,
         "Tags": List[TagTypeDef],
     },
-    total=False,
 )
 
 TaggingTypeDef = TypedDict(
     "TaggingTypeDef",
     {
         "TagSet": Sequence[TagTypeDef],
     },
@@ -4292,21 +3885,19 @@
         "Callback": Callable[..., Any],
         "SourceClient": BaseClient,
         "Config": TransferConfig,
     },
     total=False,
 )
 
-
 class BucketCopyRequestTypeDef(
     _RequiredBucketCopyRequestTypeDef, _OptionalBucketCopyRequestTypeDef
 ):
     pass
 
-
 _RequiredClientCopyRequestTypeDef = TypedDict(
     "_RequiredClientCopyRequestTypeDef",
     {
         "CopySource": CopySourceTypeDef,
         "Bucket": str,
         "Key": str,
     },
@@ -4318,21 +3909,19 @@
         "Callback": Callable[..., Any],
         "SourceClient": BaseClient,
         "Config": TransferConfig,
     },
     total=False,
 )
 
-
 class ClientCopyRequestTypeDef(
     _RequiredClientCopyRequestTypeDef, _OptionalClientCopyRequestTypeDef
 ):
     pass
 
-
 _RequiredCopyObjectRequestRequestTypeDef = TypedDict(
     "_RequiredCopyObjectRequestRequestTypeDef",
     {
         "Bucket": str,
         "CopySource": Union[str, CopySourceTypeDef],
         "Key": str,
     },
@@ -4378,21 +3967,19 @@
         "ObjectLockLegalHoldStatus": ObjectLockLegalHoldStatusType,
         "ExpectedBucketOwner": str,
         "ExpectedSourceBucketOwner": str,
     },
     total=False,
 )
 
-
 class CopyObjectRequestRequestTypeDef(
     _RequiredCopyObjectRequestRequestTypeDef, _OptionalCopyObjectRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredObjectCopyRequestTypeDef = TypedDict(
     "_RequiredObjectCopyRequestTypeDef",
     {
         "CopySource": CopySourceTypeDef,
     },
 )
 _OptionalObjectCopyRequestTypeDef = TypedDict(
@@ -4402,21 +3989,19 @@
         "Callback": Callable[..., Any],
         "SourceClient": BaseClient,
         "Config": TransferConfig,
     },
     total=False,
 )
 
-
 class ObjectCopyRequestTypeDef(
     _RequiredObjectCopyRequestTypeDef, _OptionalObjectCopyRequestTypeDef
 ):
     pass
 
-
 _RequiredUploadPartCopyRequestMultipartUploadPartCopyFromTypeDef = TypedDict(
     "_RequiredUploadPartCopyRequestMultipartUploadPartCopyFromTypeDef",
     {
         "CopySource": Union[str, CopySourceTypeDef],
     },
 )
 _OptionalUploadPartCopyRequestMultipartUploadPartCopyFromTypeDef = TypedDict(
@@ -4436,22 +4021,20 @@
         "RequestPayer": Literal["requester"],
         "ExpectedBucketOwner": str,
         "ExpectedSourceBucketOwner": str,
     },
     total=False,
 )
 
-
 class UploadPartCopyRequestMultipartUploadPartCopyFromTypeDef(
     _RequiredUploadPartCopyRequestMultipartUploadPartCopyFromTypeDef,
     _OptionalUploadPartCopyRequestMultipartUploadPartCopyFromTypeDef,
 ):
     pass
 
-
 _RequiredUploadPartCopyRequestRequestTypeDef = TypedDict(
     "_RequiredUploadPartCopyRequestRequestTypeDef",
     {
         "Bucket": str,
         "CopySource": Union[str, CopySourceTypeDef],
         "Key": str,
         "PartNumber": int,
@@ -4475,42 +4058,40 @@
         "RequestPayer": Literal["requester"],
         "ExpectedBucketOwner": str,
         "ExpectedSourceBucketOwner": str,
     },
     total=False,
 )
 
-
 class UploadPartCopyRequestRequestTypeDef(
     _RequiredUploadPartCopyRequestRequestTypeDef, _OptionalUploadPartCopyRequestRequestTypeDef
 ):
     pass
 
-
 ListBucketsOutputTypeDef = TypedDict(
     "ListBucketsOutputTypeDef",
     {
         "Buckets": List[BucketTypeDef],
         "Owner": OwnerTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CORSConfigurationTypeDef = TypedDict(
     "CORSConfigurationTypeDef",
     {
         "CORSRules": Sequence[CORSRuleTypeDef],
     },
 )
 
 GetBucketCorsOutputTypeDef = TypedDict(
     "GetBucketCorsOutputTypeDef",
     {
         "CORSRules": List[CORSRuleTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CompletedMultipartUploadTypeDef = TypedDict(
     "CompletedMultipartUploadTypeDef",
     {
         "Parts": Sequence[CompletedPartTypeDef],
@@ -4528,30 +4109,30 @@
         "ServerSideEncryption": ServerSideEncryptionType,
         "SSECustomerAlgorithm": str,
         "SSECustomerKeyMD5": str,
         "SSEKMSKeyId": str,
         "SSEKMSEncryptionContext": str,
         "BucketKeyEnabled": bool,
         "RequestCharged": Literal["requester"],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UploadPartCopyOutputTypeDef = TypedDict(
     "UploadPartCopyOutputTypeDef",
     {
         "CopySourceVersionId": str,
         "CopyPartResult": CopyPartResultTypeDef,
         "ServerSideEncryption": ServerSideEncryptionType,
         "SSECustomerAlgorithm": str,
         "SSECustomerKeyMD5": str,
         "SSEKMSKeyId": str,
         "BucketKeyEnabled": bool,
         "RequestCharged": Literal["requester"],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateBucketRequestBucketCreateTypeDef = TypedDict(
     "CreateBucketRequestBucketCreateTypeDef",
     {
         "ACL": BucketCannedACLType,
@@ -4585,21 +4166,19 @@
         "GrantWriteACP": str,
         "ObjectLockEnabledForBucket": bool,
         "ObjectOwnership": ObjectOwnershipType,
     },
     total=False,
 )
 
-
 class CreateBucketRequestRequestTypeDef(
     _RequiredCreateBucketRequestRequestTypeDef, _OptionalCreateBucketRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredCreateBucketRequestServiceResourceCreateBucketTypeDef = TypedDict(
     "_RequiredCreateBucketRequestServiceResourceCreateBucketTypeDef",
     {
         "Bucket": str,
     },
 )
 _OptionalCreateBucketRequestServiceResourceCreateBucketTypeDef = TypedDict(
@@ -4614,37 +4193,34 @@
         "GrantWriteACP": str,
         "ObjectLockEnabledForBucket": bool,
         "ObjectOwnership": ObjectOwnershipType,
     },
     total=False,
 )
 
-
 class CreateBucketRequestServiceResourceCreateBucketTypeDef(
     _RequiredCreateBucketRequestServiceResourceCreateBucketTypeDef,
     _OptionalCreateBucketRequestServiceResourceCreateBucketTypeDef,
 ):
     pass
 
-
 ObjectLockRuleTypeDef = TypedDict(
     "ObjectLockRuleTypeDef",
     {
         "DefaultRetention": DefaultRetentionTypeDef,
     },
-    total=False,
 )
 
 DeleteObjectsOutputTypeDef = TypedDict(
     "DeleteObjectsOutputTypeDef",
     {
         "Deleted": List[DeletedObjectTypeDef],
         "RequestCharged": Literal["requester"],
         "Errors": List[ErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredDeleteTypeDef = TypedDict(
     "_RequiredDeleteTypeDef",
     {
         "Objects": Sequence[ObjectIdentifierTypeDef],
@@ -4654,53 +4230,49 @@
     "_OptionalDeleteTypeDef",
     {
         "Quiet": bool,
     },
     total=False,
 )
 
-
 class DeleteTypeDef(_RequiredDeleteTypeDef, _OptionalDeleteTypeDef):
     pass
 
-
 S3KeyFilterTypeDef = TypedDict(
     "S3KeyFilterTypeDef",
     {
         "FilterRules": List[FilterRuleTypeDef],
     },
-    total=False,
 )
 
 GetBucketPolicyStatusOutputTypeDef = TypedDict(
     "GetBucketPolicyStatusOutputTypeDef",
     {
         "PolicyStatus": PolicyStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetObjectAttributesPartsTypeDef = TypedDict(
     "GetObjectAttributesPartsTypeDef",
     {
         "TotalPartsCount": int,
         "PartNumberMarker": int,
         "NextPartNumberMarker": int,
         "MaxParts": int,
         "IsTruncated": bool,
         "Parts": List[ObjectPartTypeDef],
     },
-    total=False,
 )
 
 GetObjectLegalHoldOutputTypeDef = TypedDict(
     "GetObjectLegalHoldOutputTypeDef",
     {
         "LegalHold": ObjectLockLegalHoldTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredPutObjectLegalHoldRequestRequestTypeDef = TypedDict(
     "_RequiredPutObjectLegalHoldRequestRequestTypeDef",
     {
         "Bucket": str,
@@ -4716,27 +4288,25 @@
         "ContentMD5": str,
         "ChecksumAlgorithm": ChecksumAlgorithmType,
         "ExpectedBucketOwner": str,
     },
     total=False,
 )
 
-
 class PutObjectLegalHoldRequestRequestTypeDef(
     _RequiredPutObjectLegalHoldRequestRequestTypeDef,
     _OptionalPutObjectLegalHoldRequestRequestTypeDef,
 ):
     pass
 
-
 GetObjectRetentionOutputTypeDef = TypedDict(
     "GetObjectRetentionOutputTypeDef",
     {
         "Retention": ObjectLockRetentionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredPutObjectRetentionRequestRequestTypeDef = TypedDict(
     "_RequiredPutObjectRetentionRequestRequestTypeDef",
     {
         "Bucket": str,
@@ -4753,27 +4323,25 @@
         "ContentMD5": str,
         "ChecksumAlgorithm": ChecksumAlgorithmType,
         "ExpectedBucketOwner": str,
     },
     total=False,
 )
 
-
 class PutObjectRetentionRequestRequestTypeDef(
     _RequiredPutObjectRetentionRequestRequestTypeDef,
     _OptionalPutObjectRetentionRequestRequestTypeDef,
 ):
     pass
 
-
 GetPublicAccessBlockOutputTypeDef = TypedDict(
     "GetPublicAccessBlockOutputTypeDef",
     {
         "PublicAccessBlockConfiguration": PublicAccessBlockConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredPutPublicAccessBlockRequestRequestTypeDef = TypedDict(
     "_RequiredPutPublicAccessBlockRequestRequestTypeDef",
     {
         "Bucket": str,
@@ -4786,38 +4354,34 @@
         "ContentMD5": str,
         "ChecksumAlgorithm": ChecksumAlgorithmType,
         "ExpectedBucketOwner": str,
     },
     total=False,
 )
 
-
 class PutPublicAccessBlockRequestRequestTypeDef(
     _RequiredPutPublicAccessBlockRequestRequestTypeDef,
     _OptionalPutPublicAccessBlockRequestRequestTypeDef,
 ):
     pass
 
-
 GrantTypeDef = TypedDict(
     "GrantTypeDef",
     {
         "Grantee": GranteeTypeDef,
         "Permission": PermissionType,
     },
-    total=False,
 )
 
 TargetGrantTypeDef = TypedDict(
     "TargetGrantTypeDef",
     {
         "Grantee": GranteeTypeDef,
         "Permission": BucketLogsPermissionType,
     },
-    total=False,
 )
 
 _RequiredHeadBucketRequestBucketExistsWaitTypeDef = TypedDict(
     "_RequiredHeadBucketRequestBucketExistsWaitTypeDef",
     {
         "Bucket": str,
     },
@@ -4827,22 +4391,20 @@
     {
         "ExpectedBucketOwner": str,
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
-
 class HeadBucketRequestBucketExistsWaitTypeDef(
     _RequiredHeadBucketRequestBucketExistsWaitTypeDef,
     _OptionalHeadBucketRequestBucketExistsWaitTypeDef,
 ):
     pass
 
-
 _RequiredHeadBucketRequestBucketNotExistsWaitTypeDef = TypedDict(
     "_RequiredHeadBucketRequestBucketNotExistsWaitTypeDef",
     {
         "Bucket": str,
     },
 )
 _OptionalHeadBucketRequestBucketNotExistsWaitTypeDef = TypedDict(
@@ -4850,22 +4412,20 @@
     {
         "ExpectedBucketOwner": str,
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
-
 class HeadBucketRequestBucketNotExistsWaitTypeDef(
     _RequiredHeadBucketRequestBucketNotExistsWaitTypeDef,
     _OptionalHeadBucketRequestBucketNotExistsWaitTypeDef,
 ):
     pass
 
-
 _RequiredHeadObjectRequestObjectExistsWaitTypeDef = TypedDict(
     "_RequiredHeadObjectRequestObjectExistsWaitTypeDef",
     {
         "Bucket": str,
         "Key": str,
     },
 )
@@ -4886,22 +4446,20 @@
         "ExpectedBucketOwner": str,
         "ChecksumMode": Literal["ENABLED"],
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
-
 class HeadObjectRequestObjectExistsWaitTypeDef(
     _RequiredHeadObjectRequestObjectExistsWaitTypeDef,
     _OptionalHeadObjectRequestObjectExistsWaitTypeDef,
 ):
     pass
 
-
 _RequiredHeadObjectRequestObjectNotExistsWaitTypeDef = TypedDict(
     "_RequiredHeadObjectRequestObjectNotExistsWaitTypeDef",
     {
         "Bucket": str,
         "Key": str,
     },
 )
@@ -4922,34 +4480,31 @@
         "ExpectedBucketOwner": str,
         "ChecksumMode": Literal["ENABLED"],
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
-
 class HeadObjectRequestObjectNotExistsWaitTypeDef(
     _RequiredHeadObjectRequestObjectNotExistsWaitTypeDef,
     _OptionalHeadObjectRequestObjectNotExistsWaitTypeDef,
 ):
     pass
 
-
 MultipartUploadTypeDef = TypedDict(
     "MultipartUploadTypeDef",
     {
         "UploadId": str,
         "Key": str,
         "Initiated": datetime,
         "StorageClass": StorageClassType,
         "Owner": OwnerTypeDef,
         "Initiator": InitiatorTypeDef,
         "ChecksumAlgorithm": ChecksumAlgorithmType,
     },
-    total=False,
 )
 
 InputSerializationTypeDef = TypedDict(
     "InputSerializationTypeDef",
     {
         "CSV": CSVInputTypeDef,
         "CompressionType": CompressionTypeType,
@@ -4961,50 +4516,170 @@
 
 InventoryEncryptionTypeDef = TypedDict(
     "InventoryEncryptionTypeDef",
     {
         "SSES3": Dict[str, Any],
         "SSEKMS": SSEKMSTypeDef,
     },
-    total=False,
 )
 
 OutputSerializationTypeDef = TypedDict(
     "OutputSerializationTypeDef",
     {
         "CSV": CSVOutputTypeDef,
         "JSON": JSONOutputTypeDef,
     },
     total=False,
 )
 
-_RequiredRuleTypeDef = TypedDict(
-    "_RequiredRuleTypeDef",
-    {
-        "Prefix": str,
-        "Status": ExpirationStatusType,
-    },
-)
-_OptionalRuleTypeDef = TypedDict(
-    "_OptionalRuleTypeDef",
+RuleTypeDef = TypedDict(
+    "RuleTypeDef",
     {
         "Expiration": LifecycleExpirationTypeDef,
         "ID": str,
+        "Prefix": str,
+        "Status": ExpirationStatusType,
         "Transition": TransitionTypeDef,
         "NoncurrentVersionTransition": NoncurrentVersionTransitionTypeDef,
         "NoncurrentVersionExpiration": NoncurrentVersionExpirationTypeDef,
         "AbortIncompleteMultipartUpload": AbortIncompleteMultipartUploadTypeDef,
     },
+)
+
+_RequiredListMultipartUploadsRequestListMultipartUploadsPaginateTypeDef = TypedDict(
+    "_RequiredListMultipartUploadsRequestListMultipartUploadsPaginateTypeDef",
+    {
+        "Bucket": str,
+    },
+)
+_OptionalListMultipartUploadsRequestListMultipartUploadsPaginateTypeDef = TypedDict(
+    "_OptionalListMultipartUploadsRequestListMultipartUploadsPaginateTypeDef",
+    {
+        "Delimiter": str,
+        "EncodingType": Literal["url"],
+        "Prefix": str,
+        "ExpectedBucketOwner": str,
+        "RequestPayer": Literal["requester"],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
     total=False,
 )
 
+class ListMultipartUploadsRequestListMultipartUploadsPaginateTypeDef(
+    _RequiredListMultipartUploadsRequestListMultipartUploadsPaginateTypeDef,
+    _OptionalListMultipartUploadsRequestListMultipartUploadsPaginateTypeDef,
+):
+    pass
+
+_RequiredListObjectVersionsRequestListObjectVersionsPaginateTypeDef = TypedDict(
+    "_RequiredListObjectVersionsRequestListObjectVersionsPaginateTypeDef",
+    {
+        "Bucket": str,
+    },
+)
+_OptionalListObjectVersionsRequestListObjectVersionsPaginateTypeDef = TypedDict(
+    "_OptionalListObjectVersionsRequestListObjectVersionsPaginateTypeDef",
+    {
+        "Delimiter": str,
+        "EncodingType": Literal["url"],
+        "Prefix": str,
+        "ExpectedBucketOwner": str,
+        "RequestPayer": Literal["requester"],
+        "OptionalObjectAttributes": Sequence[Literal["RestoreStatus"]],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
 
-class RuleTypeDef(_RequiredRuleTypeDef, _OptionalRuleTypeDef):
+class ListObjectVersionsRequestListObjectVersionsPaginateTypeDef(
+    _RequiredListObjectVersionsRequestListObjectVersionsPaginateTypeDef,
+    _OptionalListObjectVersionsRequestListObjectVersionsPaginateTypeDef,
+):
     pass
 
+_RequiredListObjectsRequestListObjectsPaginateTypeDef = TypedDict(
+    "_RequiredListObjectsRequestListObjectsPaginateTypeDef",
+    {
+        "Bucket": str,
+    },
+)
+_OptionalListObjectsRequestListObjectsPaginateTypeDef = TypedDict(
+    "_OptionalListObjectsRequestListObjectsPaginateTypeDef",
+    {
+        "Delimiter": str,
+        "EncodingType": Literal["url"],
+        "Prefix": str,
+        "RequestPayer": Literal["requester"],
+        "ExpectedBucketOwner": str,
+        "OptionalObjectAttributes": Sequence[Literal["RestoreStatus"]],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListObjectsRequestListObjectsPaginateTypeDef(
+    _RequiredListObjectsRequestListObjectsPaginateTypeDef,
+    _OptionalListObjectsRequestListObjectsPaginateTypeDef,
+):
+    pass
+
+_RequiredListObjectsV2RequestListObjectsV2PaginateTypeDef = TypedDict(
+    "_RequiredListObjectsV2RequestListObjectsV2PaginateTypeDef",
+    {
+        "Bucket": str,
+    },
+)
+_OptionalListObjectsV2RequestListObjectsV2PaginateTypeDef = TypedDict(
+    "_OptionalListObjectsV2RequestListObjectsV2PaginateTypeDef",
+    {
+        "Delimiter": str,
+        "EncodingType": Literal["url"],
+        "Prefix": str,
+        "FetchOwner": bool,
+        "StartAfter": str,
+        "RequestPayer": Literal["requester"],
+        "ExpectedBucketOwner": str,
+        "OptionalObjectAttributes": Sequence[Literal["RestoreStatus"]],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListObjectsV2RequestListObjectsV2PaginateTypeDef(
+    _RequiredListObjectsV2RequestListObjectsV2PaginateTypeDef,
+    _OptionalListObjectsV2RequestListObjectsV2PaginateTypeDef,
+):
+    pass
+
+_RequiredListPartsRequestListPartsPaginateTypeDef = TypedDict(
+    "_RequiredListPartsRequestListPartsPaginateTypeDef",
+    {
+        "Bucket": str,
+        "Key": str,
+        "UploadId": str,
+    },
+)
+_OptionalListPartsRequestListPartsPaginateTypeDef = TypedDict(
+    "_OptionalListPartsRequestListPartsPaginateTypeDef",
+    {
+        "RequestPayer": Literal["requester"],
+        "ExpectedBucketOwner": str,
+        "SSECustomerAlgorithm": str,
+        "SSECustomerKey": str,
+        "SSECustomerKeyMD5": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListPartsRequestListPartsPaginateTypeDef(
+    _RequiredListPartsRequestListPartsPaginateTypeDef,
+    _OptionalListPartsRequestListPartsPaginateTypeDef,
+):
+    pass
 
 ListPartsOutputTypeDef = TypedDict(
     "ListPartsOutputTypeDef",
     {
         "AbortDate": datetime,
         "AbortRuleId": str,
         "Bucket": str,
@@ -5016,52 +4691,41 @@
         "IsTruncated": bool,
         "Parts": List[PartTypeDef],
         "Initiator": InitiatorTypeDef,
         "Owner": OwnerTypeDef,
         "StorageClass": StorageClassType,
         "RequestCharged": Literal["requester"],
         "ChecksumAlgorithm": ChecksumAlgorithmType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredMetricsTypeDef = TypedDict(
-    "_RequiredMetricsTypeDef",
+MetricsTypeDef = TypedDict(
+    "MetricsTypeDef",
     {
         "Status": MetricsStatusType,
-    },
-)
-_OptionalMetricsTypeDef = TypedDict(
-    "_OptionalMetricsTypeDef",
-    {
         "EventThreshold": ReplicationTimeValueTypeDef,
     },
-    total=False,
 )
 
-
-class MetricsTypeDef(_RequiredMetricsTypeDef, _OptionalMetricsTypeDef):
-    pass
-
-
 ReplicationTimeTypeDef = TypedDict(
     "ReplicationTimeTypeDef",
     {
         "Status": ReplicationTimeStatusType,
         "Time": ReplicationTimeValueTypeDef,
     },
 )
 
 NotificationConfigurationDeprecatedResponseMetadataTypeDef = TypedDict(
     "NotificationConfigurationDeprecatedResponseMetadataTypeDef",
     {
         "TopicConfiguration": TopicConfigurationDeprecatedTypeDef,
         "QueueConfiguration": QueueConfigurationDeprecatedTypeDef,
         "CloudFunctionConfiguration": CloudFunctionConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 NotificationConfigurationDeprecatedTypeDef = TypedDict(
     "NotificationConfigurationDeprecatedTypeDef",
     {
         "TopicConfiguration": TopicConfigurationDeprecatedTypeDef,
@@ -5079,15 +4743,14 @@
         "ETag": str,
         "ChecksumAlgorithm": List[ChecksumAlgorithmType],
         "Size": int,
         "StorageClass": ObjectStorageClassType,
         "Owner": OwnerTypeDef,
         "RestoreStatus": RestoreStatusTypeDef,
     },
-    total=False,
 )
 
 ObjectVersionTypeDef = TypedDict(
     "ObjectVersionTypeDef",
     {
         "ETag": str,
         "ChecksumAlgorithm": List[ChecksumAlgorithmType],
@@ -5096,30 +4759,28 @@
         "Key": str,
         "VersionId": str,
         "IsLatest": bool,
         "LastModified": datetime,
         "Owner": OwnerTypeDef,
         "RestoreStatus": RestoreStatusTypeDef,
     },
-    total=False,
 )
 
 OwnershipControlsTypeDef = TypedDict(
     "OwnershipControlsTypeDef",
     {
         "Rules": List[OwnershipControlsRuleTypeDef],
     },
 )
 
 ProgressEventTypeDef = TypedDict(
     "ProgressEventTypeDef",
     {
         "Details": ProgressTypeDef,
     },
-    total=False,
 )
 
 _RequiredPutBucketRequestPaymentRequestBucketRequestPaymentPutTypeDef = TypedDict(
     "_RequiredPutBucketRequestPaymentRequestBucketRequestPaymentPutTypeDef",
     {
         "RequestPaymentConfiguration": RequestPaymentConfigurationTypeDef,
     },
@@ -5129,22 +4790,20 @@
     {
         "ChecksumAlgorithm": ChecksumAlgorithmType,
         "ExpectedBucketOwner": str,
     },
     total=False,
 )
 
-
 class PutBucketRequestPaymentRequestBucketRequestPaymentPutTypeDef(
     _RequiredPutBucketRequestPaymentRequestBucketRequestPaymentPutTypeDef,
     _OptionalPutBucketRequestPaymentRequestBucketRequestPaymentPutTypeDef,
 ):
     pass
 
-
 _RequiredPutBucketRequestPaymentRequestRequestTypeDef = TypedDict(
     "_RequiredPutBucketRequestPaymentRequestRequestTypeDef",
     {
         "Bucket": str,
         "RequestPaymentConfiguration": RequestPaymentConfigurationTypeDef,
     },
 )
@@ -5153,22 +4812,20 @@
     {
         "ChecksumAlgorithm": ChecksumAlgorithmType,
         "ExpectedBucketOwner": str,
     },
     total=False,
 )
 
-
 class PutBucketRequestPaymentRequestRequestTypeDef(
     _RequiredPutBucketRequestPaymentRequestRequestTypeDef,
     _OptionalPutBucketRequestPaymentRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredPutBucketVersioningRequestBucketVersioningPutTypeDef = TypedDict(
     "_RequiredPutBucketVersioningRequestBucketVersioningPutTypeDef",
     {
         "VersioningConfiguration": VersioningConfigurationTypeDef,
     },
 )
 _OptionalPutBucketVersioningRequestBucketVersioningPutTypeDef = TypedDict(
@@ -5177,22 +4834,20 @@
         "ChecksumAlgorithm": ChecksumAlgorithmType,
         "MFA": str,
         "ExpectedBucketOwner": str,
     },
     total=False,
 )
 
-
 class PutBucketVersioningRequestBucketVersioningPutTypeDef(
     _RequiredPutBucketVersioningRequestBucketVersioningPutTypeDef,
     _OptionalPutBucketVersioningRequestBucketVersioningPutTypeDef,
 ):
     pass
 
-
 _RequiredPutBucketVersioningRequestRequestTypeDef = TypedDict(
     "_RequiredPutBucketVersioningRequestRequestTypeDef",
     {
         "Bucket": str,
         "VersioningConfiguration": VersioningConfigurationTypeDef,
     },
 )
@@ -5202,118 +4857,97 @@
         "ChecksumAlgorithm": ChecksumAlgorithmType,
         "MFA": str,
         "ExpectedBucketOwner": str,
     },
     total=False,
 )
 
-
 class PutBucketVersioningRequestRequestTypeDef(
     _RequiredPutBucketVersioningRequestRequestTypeDef,
     _OptionalPutBucketVersioningRequestRequestTypeDef,
 ):
     pass
 
-
-_RequiredRoutingRuleTypeDef = TypedDict(
-    "_RequiredRoutingRuleTypeDef",
-    {
-        "Redirect": RedirectTypeDef,
-    },
-)
-_OptionalRoutingRuleTypeDef = TypedDict(
-    "_OptionalRoutingRuleTypeDef",
+RoutingRuleTypeDef = TypedDict(
+    "RoutingRuleTypeDef",
     {
         "Condition": ConditionTypeDef,
+        "Redirect": RedirectTypeDef,
     },
-    total=False,
 )
 
-
-class RoutingRuleTypeDef(_RequiredRoutingRuleTypeDef, _OptionalRoutingRuleTypeDef):
-    pass
-
-
 ServerSideEncryptionRuleTypeDef = TypedDict(
     "ServerSideEncryptionRuleTypeDef",
     {
         "ApplyServerSideEncryptionByDefault": ServerSideEncryptionByDefaultTypeDef,
         "BucketKeyEnabled": bool,
     },
-    total=False,
 )
 
 SourceSelectionCriteriaTypeDef = TypedDict(
     "SourceSelectionCriteriaTypeDef",
     {
         "SseKmsEncryptedObjects": SseKmsEncryptedObjectsTypeDef,
         "ReplicaModifications": ReplicaModificationsTypeDef,
     },
-    total=False,
 )
 
 StatsEventTypeDef = TypedDict(
     "StatsEventTypeDef",
     {
         "Details": StatsTypeDef,
     },
-    total=False,
 )
 
 AnalyticsFilterTypeDef = TypedDict(
     "AnalyticsFilterTypeDef",
     {
         "Prefix": str,
         "Tag": TagTypeDef,
         "And": AnalyticsAndOperatorTypeDef,
     },
-    total=False,
 )
 
 IntelligentTieringFilterTypeDef = TypedDict(
     "IntelligentTieringFilterTypeDef",
     {
         "Prefix": str,
         "Tag": TagTypeDef,
         "And": IntelligentTieringAndOperatorTypeDef,
     },
-    total=False,
 )
 
 LifecycleRuleFilterTypeDef = TypedDict(
     "LifecycleRuleFilterTypeDef",
     {
         "Prefix": str,
         "Tag": TagTypeDef,
         "ObjectSizeGreaterThan": int,
         "ObjectSizeLessThan": int,
         "And": LifecycleRuleAndOperatorTypeDef,
     },
-    total=False,
 )
 
 MetricsFilterTypeDef = TypedDict(
     "MetricsFilterTypeDef",
     {
         "Prefix": str,
         "Tag": TagTypeDef,
         "AccessPointArn": str,
         "And": MetricsAndOperatorTypeDef,
     },
-    total=False,
 )
 
 ReplicationRuleFilterTypeDef = TypedDict(
     "ReplicationRuleFilterTypeDef",
     {
         "Prefix": str,
         "Tag": TagTypeDef,
         "And": ReplicationRuleAndOperatorTypeDef,
     },
-    total=False,
 )
 
 _RequiredPutBucketTaggingRequestBucketTaggingPutTypeDef = TypedDict(
     "_RequiredPutBucketTaggingRequestBucketTaggingPutTypeDef",
     {
         "Tagging": TaggingTypeDef,
     },
@@ -5323,22 +4957,20 @@
     {
         "ChecksumAlgorithm": ChecksumAlgorithmType,
         "ExpectedBucketOwner": str,
     },
     total=False,
 )
 
-
 class PutBucketTaggingRequestBucketTaggingPutTypeDef(
     _RequiredPutBucketTaggingRequestBucketTaggingPutTypeDef,
     _OptionalPutBucketTaggingRequestBucketTaggingPutTypeDef,
 ):
     pass
 
-
 _RequiredPutBucketTaggingRequestRequestTypeDef = TypedDict(
     "_RequiredPutBucketTaggingRequestRequestTypeDef",
     {
         "Bucket": str,
         "Tagging": TaggingTypeDef,
     },
 )
@@ -5347,21 +4979,19 @@
     {
         "ChecksumAlgorithm": ChecksumAlgorithmType,
         "ExpectedBucketOwner": str,
     },
     total=False,
 )
 
-
 class PutBucketTaggingRequestRequestTypeDef(
     _RequiredPutBucketTaggingRequestRequestTypeDef, _OptionalPutBucketTaggingRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredPutObjectTaggingRequestRequestTypeDef = TypedDict(
     "_RequiredPutObjectTaggingRequestRequestTypeDef",
     {
         "Bucket": str,
         "Key": str,
         "Tagging": TaggingTypeDef,
     },
@@ -5374,21 +5004,19 @@
         "ChecksumAlgorithm": ChecksumAlgorithmType,
         "ExpectedBucketOwner": str,
         "RequestPayer": Literal["requester"],
     },
     total=False,
 )
 
-
 class PutObjectTaggingRequestRequestTypeDef(
     _RequiredPutObjectTaggingRequestRequestTypeDef, _OptionalPutObjectTaggingRequestRequestTypeDef
 ):
     pass
 
-
 StorageClassAnalysisDataExportTypeDef = TypedDict(
     "StorageClassAnalysisDataExportTypeDef",
     {
         "OutputSchemaVersion": Literal["V_1"],
         "Destination": AnalyticsExportDestinationTypeDef,
     },
 )
@@ -5404,22 +5032,20 @@
     {
         "ChecksumAlgorithm": ChecksumAlgorithmType,
         "ExpectedBucketOwner": str,
     },
     total=False,
 )
 
-
 class PutBucketCorsRequestBucketCorsPutTypeDef(
     _RequiredPutBucketCorsRequestBucketCorsPutTypeDef,
     _OptionalPutBucketCorsRequestBucketCorsPutTypeDef,
 ):
     pass
 
-
 _RequiredPutBucketCorsRequestRequestTypeDef = TypedDict(
     "_RequiredPutBucketCorsRequestRequestTypeDef",
     {
         "Bucket": str,
         "CORSConfiguration": CORSConfigurationTypeDef,
     },
 )
@@ -5428,21 +5054,19 @@
     {
         "ChecksumAlgorithm": ChecksumAlgorithmType,
         "ExpectedBucketOwner": str,
     },
     total=False,
 )
 
-
 class PutBucketCorsRequestRequestTypeDef(
     _RequiredPutBucketCorsRequestRequestTypeDef, _OptionalPutBucketCorsRequestRequestTypeDef
 ):
     pass
 
-
 CompleteMultipartUploadRequestMultipartUploadCompleteTypeDef = TypedDict(
     "CompleteMultipartUploadRequestMultipartUploadCompleteTypeDef",
     {
         "MultipartUpload": CompletedMultipartUploadTypeDef,
         "ChecksumCRC32": str,
         "ChecksumCRC32C": str,
         "ChecksumSHA1": str,
@@ -5477,29 +5101,26 @@
         "SSECustomerAlgorithm": str,
         "SSECustomerKey": str,
         "SSECustomerKeyMD5": str,
     },
     total=False,
 )
 
-
 class CompleteMultipartUploadRequestRequestTypeDef(
     _RequiredCompleteMultipartUploadRequestRequestTypeDef,
     _OptionalCompleteMultipartUploadRequestRequestTypeDef,
 ):
     pass
 
-
 ObjectLockConfigurationTypeDef = TypedDict(
     "ObjectLockConfigurationTypeDef",
     {
         "ObjectLockEnabled": Literal["Enabled"],
         "Rule": ObjectLockRuleTypeDef,
     },
-    total=False,
 )
 
 _RequiredDeleteObjectsRequestBucketDeleteObjectsTypeDef = TypedDict(
     "_RequiredDeleteObjectsRequestBucketDeleteObjectsTypeDef",
     {
         "Delete": DeleteTypeDef,
     },
@@ -5512,22 +5133,20 @@
         "BypassGovernanceRetention": bool,
         "ExpectedBucketOwner": str,
         "ChecksumAlgorithm": ChecksumAlgorithmType,
     },
     total=False,
 )
 
-
 class DeleteObjectsRequestBucketDeleteObjectsTypeDef(
     _RequiredDeleteObjectsRequestBucketDeleteObjectsTypeDef,
     _OptionalDeleteObjectsRequestBucketDeleteObjectsTypeDef,
 ):
     pass
 
-
 _RequiredDeleteObjectsRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteObjectsRequestRequestTypeDef",
     {
         "Bucket": str,
         "Delete": DeleteTypeDef,
     },
 )
@@ -5539,42 +5158,39 @@
         "BypassGovernanceRetention": bool,
         "ExpectedBucketOwner": str,
         "ChecksumAlgorithm": ChecksumAlgorithmType,
     },
     total=False,
 )
 
-
 class DeleteObjectsRequestRequestTypeDef(
     _RequiredDeleteObjectsRequestRequestTypeDef, _OptionalDeleteObjectsRequestRequestTypeDef
 ):
     pass
 
-
 NotificationConfigurationFilterTypeDef = TypedDict(
     "NotificationConfigurationFilterTypeDef",
     {
         "Key": S3KeyFilterTypeDef,
     },
-    total=False,
 )
 
 GetObjectAttributesOutputTypeDef = TypedDict(
     "GetObjectAttributesOutputTypeDef",
     {
         "DeleteMarker": bool,
         "LastModified": datetime,
         "VersionId": str,
         "RequestCharged": Literal["requester"],
         "ETag": str,
         "Checksum": ChecksumTypeDef,
         "ObjectParts": GetObjectAttributesPartsTypeDef,
         "StorageClass": StorageClassType,
         "ObjectSize": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AccessControlPolicyTypeDef = TypedDict(
     "AccessControlPolicyTypeDef",
     {
         "Grants": Sequence[GrantTypeDef],
@@ -5584,25 +5200,25 @@
 )
 
 GetBucketAclOutputTypeDef = TypedDict(
     "GetBucketAclOutputTypeDef",
     {
         "Owner": OwnerTypeDef,
         "Grants": List[GrantTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetObjectAclOutputTypeDef = TypedDict(
     "GetObjectAclOutputTypeDef",
     {
         "Owner": OwnerTypeDef,
         "Grants": List[GrantTypeDef],
         "RequestCharged": Literal["requester"],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredS3LocationTypeDef = TypedDict(
     "_RequiredS3LocationTypeDef",
     {
         "BucketName": str,
@@ -5618,49 +5234,36 @@
         "Tagging": TaggingTypeDef,
         "UserMetadata": Sequence[MetadataEntryTypeDef],
         "StorageClass": StorageClassType,
     },
     total=False,
 )
 
-
 class S3LocationTypeDef(_RequiredS3LocationTypeDef, _OptionalS3LocationTypeDef):
     pass
 
-
 LoggingEnabledResponseMetadataTypeDef = TypedDict(
     "LoggingEnabledResponseMetadataTypeDef",
     {
         "TargetBucket": str,
         "TargetGrants": List[TargetGrantTypeDef],
         "TargetPrefix": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredLoggingEnabledTypeDef = TypedDict(
-    "_RequiredLoggingEnabledTypeDef",
+LoggingEnabledTypeDef = TypedDict(
+    "LoggingEnabledTypeDef",
     {
         "TargetBucket": str,
-        "TargetPrefix": str,
-    },
-)
-_OptionalLoggingEnabledTypeDef = TypedDict(
-    "_OptionalLoggingEnabledTypeDef",
-    {
         "TargetGrants": List[TargetGrantTypeDef],
+        "TargetPrefix": str,
     },
-    total=False,
 )
 
-
-class LoggingEnabledTypeDef(_RequiredLoggingEnabledTypeDef, _OptionalLoggingEnabledTypeDef):
-    pass
-
-
 ListMultipartUploadsOutputTypeDef = TypedDict(
     "ListMultipartUploadsOutputTypeDef",
     {
         "Bucket": str,
         "KeyMarker": str,
         "UploadIdMarker": str,
         "NextKeyMarker": str,
@@ -5669,42 +5272,29 @@
         "NextUploadIdMarker": str,
         "MaxUploads": int,
         "IsTruncated": bool,
         "Uploads": List[MultipartUploadTypeDef],
         "CommonPrefixes": List[CommonPrefixTypeDef],
         "EncodingType": Literal["url"],
         "RequestCharged": Literal["requester"],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredInventoryS3BucketDestinationTypeDef = TypedDict(
-    "_RequiredInventoryS3BucketDestinationTypeDef",
+InventoryS3BucketDestinationTypeDef = TypedDict(
+    "InventoryS3BucketDestinationTypeDef",
     {
+        "AccountId": str,
         "Bucket": str,
         "Format": InventoryFormatType,
-    },
-)
-_OptionalInventoryS3BucketDestinationTypeDef = TypedDict(
-    "_OptionalInventoryS3BucketDestinationTypeDef",
-    {
-        "AccountId": str,
         "Prefix": str,
         "Encryption": InventoryEncryptionTypeDef,
     },
-    total=False,
 )
 
-
-class InventoryS3BucketDestinationTypeDef(
-    _RequiredInventoryS3BucketDestinationTypeDef, _OptionalInventoryS3BucketDestinationTypeDef
-):
-    pass
-
-
 _RequiredSelectObjectContentRequestRequestTypeDef = TypedDict(
     "_RequiredSelectObjectContentRequestRequestTypeDef",
     {
         "Bucket": str,
         "Key": str,
         "Expression": str,
         "ExpressionType": Literal["SQL"],
@@ -5721,71 +5311,58 @@
         "RequestProgress": RequestProgressTypeDef,
         "ScanRange": ScanRangeTypeDef,
         "ExpectedBucketOwner": str,
     },
     total=False,
 )
 
-
 class SelectObjectContentRequestRequestTypeDef(
     _RequiredSelectObjectContentRequestRequestTypeDef,
     _OptionalSelectObjectContentRequestRequestTypeDef,
 ):
     pass
 
-
 SelectParametersTypeDef = TypedDict(
     "SelectParametersTypeDef",
     {
         "InputSerialization": InputSerializationTypeDef,
         "ExpressionType": Literal["SQL"],
         "Expression": str,
         "OutputSerialization": OutputSerializationTypeDef,
     },
 )
 
 GetBucketLifecycleOutputTypeDef = TypedDict(
     "GetBucketLifecycleOutputTypeDef",
     {
         "Rules": List[RuleTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 LifecycleConfigurationTypeDef = TypedDict(
     "LifecycleConfigurationTypeDef",
     {
         "Rules": Sequence[RuleTypeDef],
     },
 )
 
-_RequiredDestinationTypeDef = TypedDict(
-    "_RequiredDestinationTypeDef",
+DestinationTypeDef = TypedDict(
+    "DestinationTypeDef",
     {
         "Bucket": str,
-    },
-)
-_OptionalDestinationTypeDef = TypedDict(
-    "_OptionalDestinationTypeDef",
-    {
         "Account": str,
         "StorageClass": StorageClassType,
         "AccessControlTranslation": AccessControlTranslationTypeDef,
         "EncryptionConfiguration": EncryptionConfigurationTypeDef,
         "ReplicationTime": ReplicationTimeTypeDef,
         "Metrics": MetricsTypeDef,
     },
-    total=False,
 )
 
-
-class DestinationTypeDef(_RequiredDestinationTypeDef, _OptionalDestinationTypeDef):
-    pass
-
-
 _RequiredPutBucketNotificationRequestRequestTypeDef = TypedDict(
     "_RequiredPutBucketNotificationRequestRequestTypeDef",
     {
         "Bucket": str,
         "NotificationConfiguration": NotificationConfigurationDeprecatedTypeDef,
     },
 )
@@ -5794,37 +5371,35 @@
     {
         "ChecksumAlgorithm": ChecksumAlgorithmType,
         "ExpectedBucketOwner": str,
     },
     total=False,
 )
 
-
 class PutBucketNotificationRequestRequestTypeDef(
     _RequiredPutBucketNotificationRequestRequestTypeDef,
     _OptionalPutBucketNotificationRequestRequestTypeDef,
 ):
     pass
 
-
 ListObjectsOutputTypeDef = TypedDict(
     "ListObjectsOutputTypeDef",
     {
         "IsTruncated": bool,
         "Marker": str,
         "NextMarker": str,
         "Contents": List[ObjectTypeDef],
         "Name": str,
         "Prefix": str,
         "Delimiter": str,
         "MaxKeys": int,
         "CommonPrefixes": List[CommonPrefixTypeDef],
         "EncodingType": Literal["url"],
         "RequestCharged": Literal["requester"],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListObjectsV2OutputTypeDef = TypedDict(
     "ListObjectsV2OutputTypeDef",
     {
         "IsTruncated": bool,
@@ -5836,15 +5411,15 @@
         "CommonPrefixes": List[CommonPrefixTypeDef],
         "EncodingType": Literal["url"],
         "KeyCount": int,
         "ContinuationToken": str,
         "NextContinuationToken": str,
         "StartAfter": str,
         "RequestCharged": Literal["requester"],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListObjectVersionsOutputTypeDef = TypedDict(
     "ListObjectVersionsOutputTypeDef",
     {
         "IsTruncated": bool,
@@ -5857,23 +5432,23 @@
         "Name": str,
         "Prefix": str,
         "Delimiter": str,
         "MaxKeys": int,
         "CommonPrefixes": List[CommonPrefixTypeDef],
         "EncodingType": Literal["url"],
         "RequestCharged": Literal["requester"],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetBucketOwnershipControlsOutputTypeDef = TypedDict(
     "GetBucketOwnershipControlsOutputTypeDef",
     {
         "OwnershipControls": OwnershipControlsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredPutBucketOwnershipControlsRequestRequestTypeDef = TypedDict(
     "_RequiredPutBucketOwnershipControlsRequestRequestTypeDef",
     {
         "Bucket": str,
@@ -5885,30 +5460,28 @@
     {
         "ContentMD5": str,
         "ExpectedBucketOwner": str,
     },
     total=False,
 )
 
-
 class PutBucketOwnershipControlsRequestRequestTypeDef(
     _RequiredPutBucketOwnershipControlsRequestRequestTypeDef,
     _OptionalPutBucketOwnershipControlsRequestRequestTypeDef,
 ):
     pass
 
-
 GetBucketWebsiteOutputTypeDef = TypedDict(
     "GetBucketWebsiteOutputTypeDef",
     {
         "RedirectAllRequestsTo": RedirectAllRequestsToTypeDef,
         "IndexDocument": IndexDocumentTypeDef,
         "ErrorDocument": ErrorDocumentTypeDef,
         "RoutingRules": List[RoutingRuleTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 WebsiteConfigurationTypeDef = TypedDict(
     "WebsiteConfigurationTypeDef",
     {
         "ErrorDocument": ErrorDocumentTypeDef,
@@ -5931,100 +5504,61 @@
     {
         "Records": RecordsEventTypeDef,
         "Stats": StatsEventTypeDef,
         "Progress": ProgressEventTypeDef,
         "Cont": Dict[str, Any],
         "End": Dict[str, Any],
     },
-    total=False,
 )
 
-_RequiredIntelligentTieringConfigurationTypeDef = TypedDict(
-    "_RequiredIntelligentTieringConfigurationTypeDef",
+IntelligentTieringConfigurationTypeDef = TypedDict(
+    "IntelligentTieringConfigurationTypeDef",
     {
         "Id": str,
+        "Filter": IntelligentTieringFilterTypeDef,
         "Status": IntelligentTieringStatusType,
         "Tierings": List[TieringTypeDef],
     },
 )
-_OptionalIntelligentTieringConfigurationTypeDef = TypedDict(
-    "_OptionalIntelligentTieringConfigurationTypeDef",
-    {
-        "Filter": IntelligentTieringFilterTypeDef,
-    },
-    total=False,
-)
-
-
-class IntelligentTieringConfigurationTypeDef(
-    _RequiredIntelligentTieringConfigurationTypeDef, _OptionalIntelligentTieringConfigurationTypeDef
-):
-    pass
-
 
-_RequiredLifecycleRuleTypeDef = TypedDict(
-    "_RequiredLifecycleRuleTypeDef",
-    {
-        "Status": ExpirationStatusType,
-    },
-)
-_OptionalLifecycleRuleTypeDef = TypedDict(
-    "_OptionalLifecycleRuleTypeDef",
+LifecycleRuleTypeDef = TypedDict(
+    "LifecycleRuleTypeDef",
     {
         "Expiration": LifecycleExpirationTypeDef,
         "ID": str,
         "Prefix": str,
         "Filter": LifecycleRuleFilterTypeDef,
+        "Status": ExpirationStatusType,
         "Transitions": List[TransitionTypeDef],
         "NoncurrentVersionTransitions": List[NoncurrentVersionTransitionTypeDef],
         "NoncurrentVersionExpiration": NoncurrentVersionExpirationTypeDef,
         "AbortIncompleteMultipartUpload": AbortIncompleteMultipartUploadTypeDef,
     },
-    total=False,
 )
 
-
-class LifecycleRuleTypeDef(_RequiredLifecycleRuleTypeDef, _OptionalLifecycleRuleTypeDef):
-    pass
-
-
-_RequiredMetricsConfigurationTypeDef = TypedDict(
-    "_RequiredMetricsConfigurationTypeDef",
+MetricsConfigurationTypeDef = TypedDict(
+    "MetricsConfigurationTypeDef",
     {
         "Id": str,
-    },
-)
-_OptionalMetricsConfigurationTypeDef = TypedDict(
-    "_OptionalMetricsConfigurationTypeDef",
-    {
         "Filter": MetricsFilterTypeDef,
     },
-    total=False,
 )
 
-
-class MetricsConfigurationTypeDef(
-    _RequiredMetricsConfigurationTypeDef, _OptionalMetricsConfigurationTypeDef
-):
-    pass
-
-
 StorageClassAnalysisTypeDef = TypedDict(
     "StorageClassAnalysisTypeDef",
     {
         "DataExport": StorageClassAnalysisDataExportTypeDef,
     },
-    total=False,
 )
 
 GetObjectLockConfigurationOutputTypeDef = TypedDict(
     "GetObjectLockConfigurationOutputTypeDef",
     {
         "ObjectLockConfiguration": ObjectLockConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredPutObjectLockConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredPutObjectLockConfigurationRequestRequestTypeDef",
     {
         "Bucket": str,
@@ -6039,91 +5573,50 @@
         "ContentMD5": str,
         "ChecksumAlgorithm": ChecksumAlgorithmType,
         "ExpectedBucketOwner": str,
     },
     total=False,
 )
 
-
 class PutObjectLockConfigurationRequestRequestTypeDef(
     _RequiredPutObjectLockConfigurationRequestRequestTypeDef,
     _OptionalPutObjectLockConfigurationRequestRequestTypeDef,
 ):
     pass
 
-
-_RequiredLambdaFunctionConfigurationTypeDef = TypedDict(
-    "_RequiredLambdaFunctionConfigurationTypeDef",
+LambdaFunctionConfigurationTypeDef = TypedDict(
+    "LambdaFunctionConfigurationTypeDef",
     {
+        "Id": str,
         "LambdaFunctionArn": str,
         "Events": List[EventType],
-    },
-)
-_OptionalLambdaFunctionConfigurationTypeDef = TypedDict(
-    "_OptionalLambdaFunctionConfigurationTypeDef",
-    {
-        "Id": str,
         "Filter": NotificationConfigurationFilterTypeDef,
     },
-    total=False,
 )
 
-
-class LambdaFunctionConfigurationTypeDef(
-    _RequiredLambdaFunctionConfigurationTypeDef, _OptionalLambdaFunctionConfigurationTypeDef
-):
-    pass
-
-
-_RequiredQueueConfigurationTypeDef = TypedDict(
-    "_RequiredQueueConfigurationTypeDef",
+QueueConfigurationTypeDef = TypedDict(
+    "QueueConfigurationTypeDef",
     {
+        "Id": str,
         "QueueArn": str,
         "Events": List[EventType],
-    },
-)
-_OptionalQueueConfigurationTypeDef = TypedDict(
-    "_OptionalQueueConfigurationTypeDef",
-    {
-        "Id": str,
         "Filter": NotificationConfigurationFilterTypeDef,
     },
-    total=False,
 )
 
-
-class QueueConfigurationTypeDef(
-    _RequiredQueueConfigurationTypeDef, _OptionalQueueConfigurationTypeDef
-):
-    pass
-
-
-_RequiredTopicConfigurationTypeDef = TypedDict(
-    "_RequiredTopicConfigurationTypeDef",
+TopicConfigurationTypeDef = TypedDict(
+    "TopicConfigurationTypeDef",
     {
+        "Id": str,
         "TopicArn": str,
         "Events": List[EventType],
-    },
-)
-_OptionalTopicConfigurationTypeDef = TypedDict(
-    "_OptionalTopicConfigurationTypeDef",
-    {
-        "Id": str,
         "Filter": NotificationConfigurationFilterTypeDef,
     },
-    total=False,
 )
 
-
-class TopicConfigurationTypeDef(
-    _RequiredTopicConfigurationTypeDef, _OptionalTopicConfigurationTypeDef
-):
-    pass
-
-
 PutBucketAclRequestBucketAclPutTypeDef = TypedDict(
     "PutBucketAclRequestBucketAclPutTypeDef",
     {
         "ACL": BucketCannedACLType,
         "AccessControlPolicy": AccessControlPolicyTypeDef,
         "ChecksumAlgorithm": ChecksumAlgorithmType,
         "GrantFullControl": str,
@@ -6154,21 +5647,19 @@
         "GrantWrite": str,
         "GrantWriteACP": str,
         "ExpectedBucketOwner": str,
     },
     total=False,
 )
 
-
 class PutBucketAclRequestRequestTypeDef(
     _RequiredPutBucketAclRequestRequestTypeDef, _OptionalPutBucketAclRequestRequestTypeDef
 ):
     pass
 
-
 PutObjectAclRequestObjectAclPutTypeDef = TypedDict(
     "PutObjectAclRequestObjectAclPutTypeDef",
     {
         "ACL": ObjectCannedACLType,
         "AccessControlPolicy": AccessControlPolicyTypeDef,
         "ChecksumAlgorithm": ChecksumAlgorithmType,
         "GrantFullControl": str,
@@ -6204,21 +5695,19 @@
         "RequestPayer": Literal["requester"],
         "VersionId": str,
         "ExpectedBucketOwner": str,
     },
     total=False,
 )
 
-
 class PutObjectAclRequestRequestTypeDef(
     _RequiredPutObjectAclRequestRequestTypeDef, _OptionalPutObjectAclRequestRequestTypeDef
 ):
     pass
 
-
 OutputLocationTypeDef = TypedDict(
     "OutputLocationTypeDef",
     {
         "S3": S3LocationTypeDef,
     },
     total=False,
 )
@@ -6231,15 +5720,15 @@
     total=False,
 )
 
 GetBucketLoggingOutputTypeDef = TypedDict(
     "GetBucketLoggingOutputTypeDef",
     {
         "LoggingEnabled": LoggingEnabledTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 InventoryDestinationTypeDef = TypedDict(
     "InventoryDestinationTypeDef",
     {
         "S3BucketDestination": InventoryS3BucketDestinationTypeDef,
@@ -6268,48 +5757,35 @@
         "ChecksumAlgorithm": ChecksumAlgorithmType,
         "LifecycleConfiguration": LifecycleConfigurationTypeDef,
         "ExpectedBucketOwner": str,
     },
     total=False,
 )
 
-
 class PutBucketLifecycleRequestRequestTypeDef(
     _RequiredPutBucketLifecycleRequestRequestTypeDef,
     _OptionalPutBucketLifecycleRequestRequestTypeDef,
 ):
     pass
 
-
-_RequiredReplicationRuleTypeDef = TypedDict(
-    "_RequiredReplicationRuleTypeDef",
-    {
-        "Status": ReplicationRuleStatusType,
-        "Destination": DestinationTypeDef,
-    },
-)
-_OptionalReplicationRuleTypeDef = TypedDict(
-    "_OptionalReplicationRuleTypeDef",
+ReplicationRuleTypeDef = TypedDict(
+    "ReplicationRuleTypeDef",
     {
         "ID": str,
         "Priority": int,
         "Prefix": str,
         "Filter": ReplicationRuleFilterTypeDef,
+        "Status": ReplicationRuleStatusType,
         "SourceSelectionCriteria": SourceSelectionCriteriaTypeDef,
         "ExistingObjectReplication": ExistingObjectReplicationTypeDef,
+        "Destination": DestinationTypeDef,
         "DeleteMarkerReplication": DeleteMarkerReplicationTypeDef,
     },
-    total=False,
 )
 
-
-class ReplicationRuleTypeDef(_RequiredReplicationRuleTypeDef, _OptionalReplicationRuleTypeDef):
-    pass
-
-
 _RequiredPutBucketWebsiteRequestBucketWebsitePutTypeDef = TypedDict(
     "_RequiredPutBucketWebsiteRequestBucketWebsitePutTypeDef",
     {
         "WebsiteConfiguration": WebsiteConfigurationTypeDef,
     },
 )
 _OptionalPutBucketWebsiteRequestBucketWebsitePutTypeDef = TypedDict(
@@ -6317,22 +5793,20 @@
     {
         "ChecksumAlgorithm": ChecksumAlgorithmType,
         "ExpectedBucketOwner": str,
     },
     total=False,
 )
 
-
 class PutBucketWebsiteRequestBucketWebsitePutTypeDef(
     _RequiredPutBucketWebsiteRequestBucketWebsitePutTypeDef,
     _OptionalPutBucketWebsiteRequestBucketWebsitePutTypeDef,
 ):
     pass
 
-
 _RequiredPutBucketWebsiteRequestRequestTypeDef = TypedDict(
     "_RequiredPutBucketWebsiteRequestRequestTypeDef",
     {
         "Bucket": str,
         "WebsiteConfiguration": WebsiteConfigurationTypeDef,
     },
 )
@@ -6341,26 +5815,24 @@
     {
         "ChecksumAlgorithm": ChecksumAlgorithmType,
         "ExpectedBucketOwner": str,
     },
     total=False,
 )
 
-
 class PutBucketWebsiteRequestRequestTypeDef(
     _RequiredPutBucketWebsiteRequestRequestTypeDef, _OptionalPutBucketWebsiteRequestRequestTypeDef
 ):
     pass
 
-
 GetBucketEncryptionOutputTypeDef = TypedDict(
     "GetBucketEncryptionOutputTypeDef",
     {
         "ServerSideEncryptionConfiguration": ServerSideEncryptionConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredPutBucketEncryptionRequestRequestTypeDef = TypedDict(
     "_RequiredPutBucketEncryptionRequestRequestTypeDef",
     {
         "Bucket": str,
@@ -6373,46 +5845,44 @@
         "ContentMD5": str,
         "ChecksumAlgorithm": ChecksumAlgorithmType,
         "ExpectedBucketOwner": str,
     },
     total=False,
 )
 
-
 class PutBucketEncryptionRequestRequestTypeDef(
     _RequiredPutBucketEncryptionRequestRequestTypeDef,
     _OptionalPutBucketEncryptionRequestRequestTypeDef,
 ):
     pass
 
-
 SelectObjectContentOutputTypeDef = TypedDict(
     "SelectObjectContentOutputTypeDef",
     {
-        "Payload": SelectObjectContentEventStreamTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Payload": "EventStream[SelectObjectContentEventStreamTypeDef]",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetBucketIntelligentTieringConfigurationOutputTypeDef = TypedDict(
     "GetBucketIntelligentTieringConfigurationOutputTypeDef",
     {
         "IntelligentTieringConfiguration": IntelligentTieringConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListBucketIntelligentTieringConfigurationsOutputTypeDef = TypedDict(
     "ListBucketIntelligentTieringConfigurationsOutputTypeDef",
     {
         "IsTruncated": bool,
         "ContinuationToken": str,
         "NextContinuationToken": str,
         "IntelligentTieringConfigurationList": List[IntelligentTieringConfigurationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutBucketIntelligentTieringConfigurationRequestRequestTypeDef = TypedDict(
     "PutBucketIntelligentTieringConfigurationRequestRequestTypeDef",
     {
         "Bucket": str,
@@ -6428,34 +5898,34 @@
     },
 )
 
 GetBucketLifecycleConfigurationOutputTypeDef = TypedDict(
     "GetBucketLifecycleConfigurationOutputTypeDef",
     {
         "Rules": List[LifecycleRuleTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetBucketMetricsConfigurationOutputTypeDef = TypedDict(
     "GetBucketMetricsConfigurationOutputTypeDef",
     {
         "MetricsConfiguration": MetricsConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListBucketMetricsConfigurationsOutputTypeDef = TypedDict(
     "ListBucketMetricsConfigurationsOutputTypeDef",
     {
         "IsTruncated": bool,
         "ContinuationToken": str,
         "NextContinuationToken": str,
         "MetricsConfigurationList": List[MetricsConfigurationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredPutBucketMetricsConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredPutBucketMetricsConfigurationRequestRequestTypeDef",
     {
         "Bucket": str,
@@ -6467,52 +5937,37 @@
     "_OptionalPutBucketMetricsConfigurationRequestRequestTypeDef",
     {
         "ExpectedBucketOwner": str,
     },
     total=False,
 )
 
-
 class PutBucketMetricsConfigurationRequestRequestTypeDef(
     _RequiredPutBucketMetricsConfigurationRequestRequestTypeDef,
     _OptionalPutBucketMetricsConfigurationRequestRequestTypeDef,
 ):
     pass
 
-
-_RequiredAnalyticsConfigurationTypeDef = TypedDict(
-    "_RequiredAnalyticsConfigurationTypeDef",
+AnalyticsConfigurationTypeDef = TypedDict(
+    "AnalyticsConfigurationTypeDef",
     {
         "Id": str,
-        "StorageClassAnalysis": StorageClassAnalysisTypeDef,
-    },
-)
-_OptionalAnalyticsConfigurationTypeDef = TypedDict(
-    "_OptionalAnalyticsConfigurationTypeDef",
-    {
         "Filter": AnalyticsFilterTypeDef,
+        "StorageClassAnalysis": StorageClassAnalysisTypeDef,
     },
-    total=False,
 )
 
-
-class AnalyticsConfigurationTypeDef(
-    _RequiredAnalyticsConfigurationTypeDef, _OptionalAnalyticsConfigurationTypeDef
-):
-    pass
-
-
 NotificationConfigurationResponseMetadataTypeDef = TypedDict(
     "NotificationConfigurationResponseMetadataTypeDef",
     {
         "TopicConfigurations": List[TopicConfigurationTypeDef],
         "QueueConfigurations": List[QueueConfigurationTypeDef],
         "LambdaFunctionConfigurations": List[LambdaFunctionConfigurationTypeDef],
         "EventBridgeConfiguration": Dict[str, Any],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 NotificationConfigurationTypeDef = TypedDict(
     "NotificationConfigurationTypeDef",
     {
         "TopicConfigurations": Sequence[TopicConfigurationTypeDef],
@@ -6548,22 +6003,20 @@
     {
         "ChecksumAlgorithm": ChecksumAlgorithmType,
         "ExpectedBucketOwner": str,
     },
     total=False,
 )
 
-
 class PutBucketLoggingRequestBucketLoggingPutTypeDef(
     _RequiredPutBucketLoggingRequestBucketLoggingPutTypeDef,
     _OptionalPutBucketLoggingRequestBucketLoggingPutTypeDef,
 ):
     pass
 
-
 _RequiredPutBucketLoggingRequestRequestTypeDef = TypedDict(
     "_RequiredPutBucketLoggingRequestRequestTypeDef",
     {
         "Bucket": str,
         "BucketLoggingStatus": BucketLoggingStatusTypeDef,
     },
 )
@@ -6572,47 +6025,32 @@
     {
         "ChecksumAlgorithm": ChecksumAlgorithmType,
         "ExpectedBucketOwner": str,
     },
     total=False,
 )
 
-
 class PutBucketLoggingRequestRequestTypeDef(
     _RequiredPutBucketLoggingRequestRequestTypeDef, _OptionalPutBucketLoggingRequestRequestTypeDef
 ):
     pass
 
-
-_RequiredInventoryConfigurationTypeDef = TypedDict(
-    "_RequiredInventoryConfigurationTypeDef",
+InventoryConfigurationTypeDef = TypedDict(
+    "InventoryConfigurationTypeDef",
     {
         "Destination": InventoryDestinationTypeDef,
         "IsEnabled": bool,
+        "Filter": InventoryFilterTypeDef,
         "Id": str,
         "IncludedObjectVersions": InventoryIncludedObjectVersionsType,
-        "Schedule": InventoryScheduleTypeDef,
-    },
-)
-_OptionalInventoryConfigurationTypeDef = TypedDict(
-    "_OptionalInventoryConfigurationTypeDef",
-    {
-        "Filter": InventoryFilterTypeDef,
         "OptionalFields": List[InventoryOptionalFieldType],
+        "Schedule": InventoryScheduleTypeDef,
     },
-    total=False,
 )
 
-
-class InventoryConfigurationTypeDef(
-    _RequiredInventoryConfigurationTypeDef, _OptionalInventoryConfigurationTypeDef
-):
-    pass
-
-
 ReplicationConfigurationTypeDef = TypedDict(
     "ReplicationConfigurationTypeDef",
     {
         "Role": str,
         "Rules": List[ReplicationRuleTypeDef],
     },
 )
@@ -6639,38 +6077,36 @@
         "ChecksumAlgorithm": ChecksumAlgorithmType,
         "LifecycleConfiguration": BucketLifecycleConfigurationTypeDef,
         "ExpectedBucketOwner": str,
     },
     total=False,
 )
 
-
 class PutBucketLifecycleConfigurationRequestRequestTypeDef(
     _RequiredPutBucketLifecycleConfigurationRequestRequestTypeDef,
     _OptionalPutBucketLifecycleConfigurationRequestRequestTypeDef,
 ):
     pass
 
-
 GetBucketAnalyticsConfigurationOutputTypeDef = TypedDict(
     "GetBucketAnalyticsConfigurationOutputTypeDef",
     {
         "AnalyticsConfiguration": AnalyticsConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListBucketAnalyticsConfigurationsOutputTypeDef = TypedDict(
     "ListBucketAnalyticsConfigurationsOutputTypeDef",
     {
         "IsTruncated": bool,
         "ContinuationToken": str,
         "NextContinuationToken": str,
         "AnalyticsConfigurationList": List[AnalyticsConfigurationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredPutBucketAnalyticsConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredPutBucketAnalyticsConfigurationRequestRequestTypeDef",
     {
         "Bucket": str,
@@ -6682,22 +6118,20 @@
     "_OptionalPutBucketAnalyticsConfigurationRequestRequestTypeDef",
     {
         "ExpectedBucketOwner": str,
     },
     total=False,
 )
 
-
 class PutBucketAnalyticsConfigurationRequestRequestTypeDef(
     _RequiredPutBucketAnalyticsConfigurationRequestRequestTypeDef,
     _OptionalPutBucketAnalyticsConfigurationRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredPutBucketNotificationConfigurationRequestBucketNotificationPutTypeDef = TypedDict(
     "_RequiredPutBucketNotificationConfigurationRequestBucketNotificationPutTypeDef",
     {
         "NotificationConfiguration": NotificationConfigurationTypeDef,
     },
 )
 _OptionalPutBucketNotificationConfigurationRequestBucketNotificationPutTypeDef = TypedDict(
@@ -6705,22 +6139,20 @@
     {
         "ExpectedBucketOwner": str,
         "SkipDestinationValidation": bool,
     },
     total=False,
 )
 
-
 class PutBucketNotificationConfigurationRequestBucketNotificationPutTypeDef(
     _RequiredPutBucketNotificationConfigurationRequestBucketNotificationPutTypeDef,
     _OptionalPutBucketNotificationConfigurationRequestBucketNotificationPutTypeDef,
 ):
     pass
 
-
 _RequiredPutBucketNotificationConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredPutBucketNotificationConfigurationRequestRequestTypeDef",
     {
         "Bucket": str,
         "NotificationConfiguration": NotificationConfigurationTypeDef,
     },
 )
@@ -6729,22 +6161,20 @@
     {
         "ExpectedBucketOwner": str,
         "SkipDestinationValidation": bool,
     },
     total=False,
 )
 
-
 class PutBucketNotificationConfigurationRequestRequestTypeDef(
     _RequiredPutBucketNotificationConfigurationRequestRequestTypeDef,
     _OptionalPutBucketNotificationConfigurationRequestRequestTypeDef,
 ):
     pass
 
-
 RestoreObjectRequestObjectRestoreObjectTypeDef = TypedDict(
     "RestoreObjectRequestObjectRestoreObjectTypeDef",
     {
         "VersionId": str,
         "RestoreRequest": RestoreRequestTypeDef,
         "RequestPayer": Literal["requester"],
         "ChecksumAlgorithm": ChecksumAlgorithmType,
@@ -6780,37 +6210,35 @@
         "RequestPayer": Literal["requester"],
         "ChecksumAlgorithm": ChecksumAlgorithmType,
         "ExpectedBucketOwner": str,
     },
     total=False,
 )
 
-
 class RestoreObjectRequestRequestTypeDef(
     _RequiredRestoreObjectRequestRequestTypeDef, _OptionalRestoreObjectRequestRequestTypeDef
 ):
     pass
 
-
 GetBucketInventoryConfigurationOutputTypeDef = TypedDict(
     "GetBucketInventoryConfigurationOutputTypeDef",
     {
         "InventoryConfiguration": InventoryConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListBucketInventoryConfigurationsOutputTypeDef = TypedDict(
     "ListBucketInventoryConfigurationsOutputTypeDef",
     {
         "ContinuationToken": str,
         "InventoryConfigurationList": List[InventoryConfigurationTypeDef],
         "IsTruncated": bool,
         "NextContinuationToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredPutBucketInventoryConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredPutBucketInventoryConfigurationRequestRequestTypeDef",
     {
         "Bucket": str,
@@ -6822,27 +6250,25 @@
     "_OptionalPutBucketInventoryConfigurationRequestRequestTypeDef",
     {
         "ExpectedBucketOwner": str,
     },
     total=False,
 )
 
-
 class PutBucketInventoryConfigurationRequestRequestTypeDef(
     _RequiredPutBucketInventoryConfigurationRequestRequestTypeDef,
     _OptionalPutBucketInventoryConfigurationRequestRequestTypeDef,
 ):
     pass
 
-
 GetBucketReplicationOutputTypeDef = TypedDict(
     "GetBucketReplicationOutputTypeDef",
     {
         "ReplicationConfiguration": ReplicationConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredPutBucketReplicationRequestRequestTypeDef = TypedDict(
     "_RequiredPutBucketReplicationRequestRequestTypeDef",
     {
         "Bucket": str,
@@ -6855,13 +6281,12 @@
         "ChecksumAlgorithm": ChecksumAlgorithmType,
         "Token": str,
         "ExpectedBucketOwner": str,
     },
     total=False,
 )
 
-
 class PutBucketReplicationRequestRequestTypeDef(
     _RequiredPutBucketReplicationRequestRequestTypeDef,
     _OptionalPutBucketReplicationRequestRequestTypeDef,
 ):
     pass
```

### Comparing `mypy-boto3-s3-1.28.0/mypy_boto3_s3/type_defs.pyi` & `mypy-boto3-s3-1.28.2/mypy_boto3_s3/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Callable, Dict, List, Mapping, Sequence, Union
 
 from boto3.s3.transfer import TransferConfig
 from botocore.client import BaseClient
+from botocore.eventstream import EventStream
 from botocore.response import StreamingBody
 
 from .literals import (
     ArchiveStatusType,
     BucketAccelerateStatusType,
     BucketCannedACLType,
     BucketLocationConstraintType,
@@ -74,17 +75,18 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "AbortIncompleteMultipartUploadTypeDef",
-    "AbortMultipartUploadOutputTypeDef",
+    "ResponseMetadataTypeDef",
     "AbortMultipartUploadRequestMultipartUploadAbortTypeDef",
     "AbortMultipartUploadRequestRequestTypeDef",
     "AccelerateConfigurationTypeDef",
     "OwnerTypeDef",
     "AccessControlTranslationTypeDef",
     "TagTypeDef",
     "AnalyticsS3BucketDestinationTypeDef",
@@ -101,24 +103,21 @@
     "ClientDownloadFileRequestTypeDef",
     "ClientDownloadFileobjRequestTypeDef",
     "ClientGeneratePresignedPostRequestTypeDef",
     "ClientUploadFileRequestTypeDef",
     "ClientUploadFileobjRequestTypeDef",
     "CloudFunctionConfigurationTypeDef",
     "CommonPrefixTypeDef",
-    "CompleteMultipartUploadOutputTypeDef",
     "CompletedPartTypeDef",
     "ConditionTypeDef",
     "CopyObjectResultTypeDef",
     "CopyObjectRequestObjectCopyFromTypeDef",
     "CopyObjectRequestObjectSummaryCopyFromTypeDef",
     "CopyPartResultTypeDef",
     "CreateBucketConfigurationTypeDef",
-    "CreateBucketOutputTypeDef",
-    "CreateMultipartUploadOutputTypeDef",
     "CreateMultipartUploadRequestObjectInitiateMultipartUploadTypeDef",
     "CreateMultipartUploadRequestObjectSummaryInitiateMultipartUploadTypeDef",
     "CreateMultipartUploadRequestRequestTypeDef",
     "DefaultRetentionTypeDef",
     "DeleteBucketAnalyticsConfigurationRequestRequestTypeDef",
     "DeleteBucketCorsRequestBucketCorsDeleteTypeDef",
     "DeleteBucketCorsRequestRequestTypeDef",
@@ -136,88 +135,74 @@
     "DeleteBucketRequestBucketDeleteTypeDef",
     "DeleteBucketRequestRequestTypeDef",
     "DeleteBucketTaggingRequestBucketTaggingDeleteTypeDef",
     "DeleteBucketTaggingRequestRequestTypeDef",
     "DeleteBucketWebsiteRequestBucketWebsiteDeleteTypeDef",
     "DeleteBucketWebsiteRequestRequestTypeDef",
     "DeleteMarkerReplicationTypeDef",
-    "DeleteObjectOutputTypeDef",
     "DeleteObjectRequestObjectDeleteTypeDef",
     "DeleteObjectRequestObjectSummaryDeleteTypeDef",
     "DeleteObjectRequestObjectVersionDeleteTypeDef",
     "DeleteObjectRequestRequestTypeDef",
-    "DeleteObjectTaggingOutputTypeDef",
     "DeleteObjectTaggingRequestRequestTypeDef",
     "DeletedObjectTypeDef",
     "ErrorTypeDef",
     "DeletePublicAccessBlockRequestRequestTypeDef",
     "ObjectIdentifierTypeDef",
     "EncryptionConfigurationTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "EncryptionTypeDef",
-    "ErrorDocumentResponseMetadataTypeDef",
     "ErrorDocumentTypeDef",
     "ExistingObjectReplicationTypeDef",
     "FilterRuleTypeDef",
-    "GetBucketAccelerateConfigurationOutputTypeDef",
     "GetBucketAccelerateConfigurationRequestRequestTypeDef",
     "GetBucketAclRequestRequestTypeDef",
     "GetBucketAnalyticsConfigurationRequestRequestTypeDef",
     "GetBucketCorsRequestRequestTypeDef",
     "GetBucketEncryptionRequestRequestTypeDef",
     "GetBucketIntelligentTieringConfigurationRequestRequestTypeDef",
     "GetBucketInventoryConfigurationRequestRequestTypeDef",
     "GetBucketLifecycleConfigurationRequestRequestTypeDef",
     "GetBucketLifecycleRequestRequestTypeDef",
-    "GetBucketLocationOutputTypeDef",
     "GetBucketLocationRequestRequestTypeDef",
     "GetBucketLoggingRequestRequestTypeDef",
     "GetBucketMetricsConfigurationRequestRequestTypeDef",
     "GetBucketNotificationConfigurationRequestRequestTypeDef",
     "GetBucketOwnershipControlsRequestRequestTypeDef",
-    "GetBucketPolicyOutputTypeDef",
     "GetBucketPolicyRequestRequestTypeDef",
     "PolicyStatusTypeDef",
     "GetBucketPolicyStatusRequestRequestTypeDef",
     "GetBucketReplicationRequestRequestTypeDef",
-    "GetBucketRequestPaymentOutputTypeDef",
     "GetBucketRequestPaymentRequestRequestTypeDef",
     "GetBucketTaggingRequestRequestTypeDef",
-    "GetBucketVersioningOutputTypeDef",
     "GetBucketVersioningRequestRequestTypeDef",
     "IndexDocumentTypeDef",
     "RedirectAllRequestsToTypeDef",
     "GetBucketWebsiteRequestRequestTypeDef",
     "GetObjectAclRequestRequestTypeDef",
     "ObjectPartTypeDef",
     "GetObjectAttributesRequestRequestTypeDef",
     "ObjectLockLegalHoldTypeDef",
     "GetObjectLegalHoldRequestRequestTypeDef",
     "GetObjectLockConfigurationRequestRequestTypeDef",
-    "GetObjectOutputTypeDef",
     "GetObjectRequestObjectGetTypeDef",
     "GetObjectRequestObjectSummaryGetTypeDef",
     "GetObjectRequestObjectVersionGetTypeDef",
     "GetObjectRequestRequestTypeDef",
     "ObjectLockRetentionTypeDef",
     "GetObjectRetentionRequestRequestTypeDef",
     "GetObjectTaggingRequestRequestTypeDef",
-    "GetObjectTorrentOutputTypeDef",
     "GetObjectTorrentRequestRequestTypeDef",
     "PublicAccessBlockConfigurationTypeDef",
     "GetPublicAccessBlockRequestRequestTypeDef",
     "GlacierJobParametersTypeDef",
     "GranteeTypeDef",
     "WaiterConfigTypeDef",
     "HeadBucketRequestRequestTypeDef",
-    "HeadObjectOutputTypeDef",
     "HeadObjectRequestObjectVersionHeadTypeDef",
     "HeadObjectRequestRequestTypeDef",
-    "IndexDocumentResponseMetadataTypeDef",
-    "InitiatorResponseMetadataTypeDef",
     "InitiatorTypeDef",
     "JSONInputTypeDef",
     "TieringTypeDef",
     "InventoryFilterTypeDef",
     "InventoryScheduleTypeDef",
     "SSEKMSTypeDef",
     "JSONOutputTypeDef",
@@ -225,70 +210,82 @@
     "NoncurrentVersionExpirationTypeDef",
     "NoncurrentVersionTransitionTypeDef",
     "TransitionTypeDef",
     "ListBucketAnalyticsConfigurationsRequestRequestTypeDef",
     "ListBucketIntelligentTieringConfigurationsRequestRequestTypeDef",
     "ListBucketInventoryConfigurationsRequestRequestTypeDef",
     "ListBucketMetricsConfigurationsRequestRequestTypeDef",
-    "ListMultipartUploadsRequestListMultipartUploadsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListMultipartUploadsRequestRequestTypeDef",
-    "ListObjectVersionsRequestListObjectVersionsPaginateTypeDef",
     "ListObjectVersionsRequestRequestTypeDef",
-    "ListObjectsRequestListObjectsPaginateTypeDef",
     "ListObjectsRequestRequestTypeDef",
-    "ListObjectsV2RequestListObjectsV2PaginateTypeDef",
     "ListObjectsV2RequestRequestTypeDef",
     "PartTypeDef",
-    "ListPartsRequestListPartsPaginateTypeDef",
     "ListPartsRequestRequestTypeDef",
     "MetadataEntryTypeDef",
     "ReplicationTimeValueTypeDef",
     "QueueConfigurationDeprecatedTypeDef",
     "TopicConfigurationDeprecatedTypeDef",
     "ObjectDownloadFileRequestTypeDef",
     "ObjectDownloadFileobjRequestTypeDef",
     "RestoreStatusTypeDef",
     "ObjectUploadFileRequestTypeDef",
     "ObjectUploadFileobjRequestTypeDef",
-    "OwnerResponseMetadataTypeDef",
     "OwnershipControlsRuleTypeDef",
-    "PaginatorConfigTypeDef",
     "ProgressTypeDef",
     "PutBucketPolicyRequestBucketPolicyPutTypeDef",
     "PutBucketPolicyRequestRequestTypeDef",
     "RequestPaymentConfigurationTypeDef",
     "PutBucketVersioningRequestBucketVersioningEnableTypeDef",
     "VersioningConfigurationTypeDef",
     "PutBucketVersioningRequestBucketVersioningSuspendTypeDef",
-    "PutObjectAclOutputTypeDef",
-    "PutObjectLegalHoldOutputTypeDef",
-    "PutObjectLockConfigurationOutputTypeDef",
-    "PutObjectOutputTypeDef",
     "PutObjectRequestBucketPutObjectTypeDef",
     "PutObjectRequestObjectPutTypeDef",
     "PutObjectRequestObjectSummaryPutTypeDef",
     "PutObjectRequestRequestTypeDef",
-    "PutObjectRetentionOutputTypeDef",
-    "PutObjectTaggingOutputTypeDef",
     "RecordsEventTypeDef",
-    "RedirectAllRequestsToResponseMetadataTypeDef",
     "RedirectTypeDef",
     "ReplicaModificationsTypeDef",
     "RequestProgressTypeDef",
-    "ResponseMetadataTypeDef",
-    "RestoreObjectOutputTypeDef",
-    "RestoreStatusResponseMetadataTypeDef",
     "ScanRangeTypeDef",
     "ServerSideEncryptionByDefaultTypeDef",
     "SseKmsEncryptedObjectsTypeDef",
     "StatsTypeDef",
-    "UploadPartOutputTypeDef",
     "UploadPartRequestMultipartUploadPartUploadTypeDef",
     "UploadPartRequestRequestTypeDef",
     "WriteGetObjectResponseRequestRequestTypeDef",
+    "AbortMultipartUploadOutputTypeDef",
+    "CompleteMultipartUploadOutputTypeDef",
+    "CreateBucketOutputTypeDef",
+    "CreateMultipartUploadOutputTypeDef",
+    "DeleteObjectOutputTypeDef",
+    "DeleteObjectTaggingOutputTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "ErrorDocumentResponseMetadataTypeDef",
+    "GetBucketAccelerateConfigurationOutputTypeDef",
+    "GetBucketLocationOutputTypeDef",
+    "GetBucketPolicyOutputTypeDef",
+    "GetBucketRequestPaymentOutputTypeDef",
+    "GetBucketVersioningOutputTypeDef",
+    "GetObjectOutputTypeDef",
+    "GetObjectTorrentOutputTypeDef",
+    "HeadObjectOutputTypeDef",
+    "IndexDocumentResponseMetadataTypeDef",
+    "InitiatorResponseMetadataTypeDef",
+    "OwnerResponseMetadataTypeDef",
+    "PutObjectAclOutputTypeDef",
+    "PutObjectLegalHoldOutputTypeDef",
+    "PutObjectLockConfigurationOutputTypeDef",
+    "PutObjectOutputTypeDef",
+    "PutObjectRetentionOutputTypeDef",
+    "PutObjectTaggingOutputTypeDef",
+    "RedirectAllRequestsToResponseMetadataTypeDef",
+    "RestoreObjectOutputTypeDef",
+    "RestoreStatusResponseMetadataTypeDef",
+    "UploadPartOutputTypeDef",
     "PutBucketAccelerateConfigurationRequestRequestTypeDef",
     "DeleteMarkerEntryTypeDef",
     "AnalyticsAndOperatorTypeDef",
     "GetBucketTaggingOutputTypeDef",
     "GetObjectTaggingOutputTypeDef",
     "IntelligentTieringAndOperatorTypeDef",
     "LifecycleRuleAndOperatorTypeDef",
@@ -330,14 +327,19 @@
     "HeadObjectRequestObjectExistsWaitTypeDef",
     "HeadObjectRequestObjectNotExistsWaitTypeDef",
     "MultipartUploadTypeDef",
     "InputSerializationTypeDef",
     "InventoryEncryptionTypeDef",
     "OutputSerializationTypeDef",
     "RuleTypeDef",
+    "ListMultipartUploadsRequestListMultipartUploadsPaginateTypeDef",
+    "ListObjectVersionsRequestListObjectVersionsPaginateTypeDef",
+    "ListObjectsRequestListObjectsPaginateTypeDef",
+    "ListObjectsV2RequestListObjectsV2PaginateTypeDef",
+    "ListPartsRequestListPartsPaginateTypeDef",
     "ListPartsOutputTypeDef",
     "MetricsTypeDef",
     "ReplicationTimeTypeDef",
     "NotificationConfigurationDeprecatedResponseMetadataTypeDef",
     "NotificationConfigurationDeprecatedTypeDef",
     "ObjectTypeDef",
     "ObjectVersionTypeDef",
@@ -451,22 +453,24 @@
 )
 
 AbortIncompleteMultipartUploadTypeDef = TypedDict(
     "AbortIncompleteMultipartUploadTypeDef",
     {
         "DaysAfterInitiation": int,
     },
-    total=False,
 )
 
-AbortMultipartUploadOutputTypeDef = TypedDict(
-    "AbortMultipartUploadOutputTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "RequestCharged": Literal["requester"],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 AbortMultipartUploadRequestMultipartUploadAbortTypeDef = TypedDict(
     "AbortMultipartUploadRequestMultipartUploadAbortTypeDef",
     {
         "RequestPayer": Literal["requester"],
@@ -488,35 +492,36 @@
     {
         "RequestPayer": Literal["requester"],
         "ExpectedBucketOwner": str,
     },
     total=False,
 )
 
+
 class AbortMultipartUploadRequestRequestTypeDef(
     _RequiredAbortMultipartUploadRequestRequestTypeDef,
     _OptionalAbortMultipartUploadRequestRequestTypeDef,
 ):
     pass
 
+
 AccelerateConfigurationTypeDef = TypedDict(
     "AccelerateConfigurationTypeDef",
     {
         "Status": BucketAccelerateStatusType,
     },
     total=False,
 )
 
 OwnerTypeDef = TypedDict(
     "OwnerTypeDef",
     {
         "DisplayName": str,
         "ID": str,
     },
-    total=False,
 )
 
 AccessControlTranslationTypeDef = TypedDict(
     "AccessControlTranslationTypeDef",
     {
         "Owner": Literal["Destination"],
     },
@@ -526,35 +531,24 @@
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
-_RequiredAnalyticsS3BucketDestinationTypeDef = TypedDict(
-    "_RequiredAnalyticsS3BucketDestinationTypeDef",
+AnalyticsS3BucketDestinationTypeDef = TypedDict(
+    "AnalyticsS3BucketDestinationTypeDef",
     {
         "Format": Literal["CSV"],
-        "Bucket": str,
-    },
-)
-_OptionalAnalyticsS3BucketDestinationTypeDef = TypedDict(
-    "_OptionalAnalyticsS3BucketDestinationTypeDef",
-    {
         "BucketAccountId": str,
+        "Bucket": str,
         "Prefix": str,
     },
-    total=False,
 )
 
-class AnalyticsS3BucketDestinationTypeDef(
-    _RequiredAnalyticsS3BucketDestinationTypeDef, _OptionalAnalyticsS3BucketDestinationTypeDef
-):
-    pass
-
 _RequiredCopySourceTypeDef = TypedDict(
     "_RequiredCopySourceTypeDef",
     {
         "Bucket": str,
         "Key": str,
     },
 )
@@ -562,17 +556,19 @@
     "_OptionalCopySourceTypeDef",
     {
         "VersionId": str,
     },
     total=False,
 )
 
+
 class CopySourceTypeDef(_RequiredCopySourceTypeDef, _OptionalCopySourceTypeDef):
     pass
 
+
 _RequiredBucketDownloadFileRequestTypeDef = TypedDict(
     "_RequiredBucketDownloadFileRequestTypeDef",
     {
         "Key": str,
         "Filename": str,
     },
 )
@@ -582,19 +578,21 @@
         "ExtraArgs": Dict[str, Any],
         "Callback": Callable[..., Any],
         "Config": TransferConfig,
     },
     total=False,
 )
 
+
 class BucketDownloadFileRequestTypeDef(
     _RequiredBucketDownloadFileRequestTypeDef, _OptionalBucketDownloadFileRequestTypeDef
 ):
     pass
 
+
 _RequiredBucketDownloadFileobjRequestTypeDef = TypedDict(
     "_RequiredBucketDownloadFileobjRequestTypeDef",
     {
         "Key": str,
         "Fileobj": Union[IO[Any], StreamingBody],
     },
 )
@@ -604,26 +602,27 @@
         "ExtraArgs": Dict[str, Any],
         "Callback": Callable[..., Any],
         "Config": TransferConfig,
     },
     total=False,
 )
 
+
 class BucketDownloadFileobjRequestTypeDef(
     _RequiredBucketDownloadFileobjRequestTypeDef, _OptionalBucketDownloadFileobjRequestTypeDef
 ):
     pass
 
+
 BucketTypeDef = TypedDict(
     "BucketTypeDef",
     {
         "Name": str,
         "CreationDate": datetime,
     },
-    total=False,
 )
 
 _RequiredBucketUploadFileRequestTypeDef = TypedDict(
     "_RequiredBucketUploadFileRequestTypeDef",
     {
         "Filename": str,
         "Key": str,
@@ -635,19 +634,21 @@
         "ExtraArgs": Dict[str, Any],
         "Callback": Callable[..., Any],
         "Config": TransferConfig,
     },
     total=False,
 )
 
+
 class BucketUploadFileRequestTypeDef(
     _RequiredBucketUploadFileRequestTypeDef, _OptionalBucketUploadFileRequestTypeDef
 ):
     pass
 
+
 _RequiredBucketUploadFileobjRequestTypeDef = TypedDict(
     "_RequiredBucketUploadFileobjRequestTypeDef",
     {
         "Fileobj": Union[IO[Any], StreamingBody],
         "Key": str,
     },
 )
@@ -657,40 +658,33 @@
         "ExtraArgs": Dict[str, Any],
         "Callback": Callable[..., Any],
         "Config": TransferConfig,
     },
     total=False,
 )
 
+
 class BucketUploadFileobjRequestTypeDef(
     _RequiredBucketUploadFileobjRequestTypeDef, _OptionalBucketUploadFileobjRequestTypeDef
 ):
     pass
 
-_RequiredCORSRuleTypeDef = TypedDict(
-    "_RequiredCORSRuleTypeDef",
-    {
-        "AllowedMethods": List[str],
-        "AllowedOrigins": List[str],
-    },
-)
-_OptionalCORSRuleTypeDef = TypedDict(
-    "_OptionalCORSRuleTypeDef",
+
+CORSRuleTypeDef = TypedDict(
+    "CORSRuleTypeDef",
     {
         "ID": str,
         "AllowedHeaders": List[str],
+        "AllowedMethods": List[str],
+        "AllowedOrigins": List[str],
         "ExposeHeaders": List[str],
         "MaxAgeSeconds": int,
     },
-    total=False,
 )
 
-class CORSRuleTypeDef(_RequiredCORSRuleTypeDef, _OptionalCORSRuleTypeDef):
-    pass
-
 CSVInputTypeDef = TypedDict(
     "CSVInputTypeDef",
     {
         "FileHeaderInfo": FileHeaderInfoType,
         "Comments": str,
         "QuoteEscapeCharacter": str,
         "RecordDelimiter": str,
@@ -717,15 +711,14 @@
     "ChecksumTypeDef",
     {
         "ChecksumCRC32": str,
         "ChecksumCRC32C": str,
         "ChecksumSHA1": str,
         "ChecksumSHA256": str,
     },
-    total=False,
 )
 
 _RequiredClientDownloadFileRequestTypeDef = TypedDict(
     "_RequiredClientDownloadFileRequestTypeDef",
     {
         "Bucket": str,
         "Key": str,
@@ -738,19 +731,21 @@
         "ExtraArgs": Dict[str, Any],
         "Callback": Callable[..., Any],
         "Config": TransferConfig,
     },
     total=False,
 )
 
+
 class ClientDownloadFileRequestTypeDef(
     _RequiredClientDownloadFileRequestTypeDef, _OptionalClientDownloadFileRequestTypeDef
 ):
     pass
 
+
 _RequiredClientDownloadFileobjRequestTypeDef = TypedDict(
     "_RequiredClientDownloadFileobjRequestTypeDef",
     {
         "Bucket": str,
         "Key": str,
         "Fileobj": Union[IO[Any], StreamingBody],
     },
@@ -761,19 +756,21 @@
         "ExtraArgs": Dict[str, Any],
         "Callback": Callable[..., Any],
         "Config": TransferConfig,
     },
     total=False,
 )
 
+
 class ClientDownloadFileobjRequestTypeDef(
     _RequiredClientDownloadFileobjRequestTypeDef, _OptionalClientDownloadFileobjRequestTypeDef
 ):
     pass
 
+
 _RequiredClientGeneratePresignedPostRequestTypeDef = TypedDict(
     "_RequiredClientGeneratePresignedPostRequestTypeDef",
     {
         "Bucket": str,
         "Key": str,
     },
 )
@@ -783,20 +780,22 @@
         "Fields": Dict[str, Any],
         "Conditions": Union[List[Any], Dict[str, Any]],
         "ExpiresIn": int,
     },
     total=False,
 )
 
+
 class ClientGeneratePresignedPostRequestTypeDef(
     _RequiredClientGeneratePresignedPostRequestTypeDef,
     _OptionalClientGeneratePresignedPostRequestTypeDef,
 ):
     pass
 
+
 _RequiredClientUploadFileRequestTypeDef = TypedDict(
     "_RequiredClientUploadFileRequestTypeDef",
     {
         "Filename": str,
         "Bucket": str,
         "Key": str,
     },
@@ -807,19 +806,21 @@
         "ExtraArgs": Dict[str, Any],
         "Callback": Callable[..., Any],
         "Config": TransferConfig,
     },
     total=False,
 )
 
+
 class ClientUploadFileRequestTypeDef(
     _RequiredClientUploadFileRequestTypeDef, _OptionalClientUploadFileRequestTypeDef
 ):
     pass
 
+
 _RequiredClientUploadFileobjRequestTypeDef = TypedDict(
     "_RequiredClientUploadFileobjRequestTypeDef",
     {
         "Fileobj": Union[IO[Any], StreamingBody],
         "Bucket": str,
         "Key": str,
     },
@@ -830,58 +831,37 @@
         "ExtraArgs": Dict[str, Any],
         "Callback": Callable[..., Any],
         "Config": TransferConfig,
     },
     total=False,
 )
 
+
 class ClientUploadFileobjRequestTypeDef(
     _RequiredClientUploadFileobjRequestTypeDef, _OptionalClientUploadFileobjRequestTypeDef
 ):
     pass
 
+
 CloudFunctionConfigurationTypeDef = TypedDict(
     "CloudFunctionConfigurationTypeDef",
     {
         "Id": str,
         "Event": EventType,
         "Events": List[EventType],
         "CloudFunction": str,
         "InvocationRole": str,
     },
-    total=False,
 )
 
 CommonPrefixTypeDef = TypedDict(
     "CommonPrefixTypeDef",
     {
         "Prefix": str,
     },
-    total=False,
-)
-
-CompleteMultipartUploadOutputTypeDef = TypedDict(
-    "CompleteMultipartUploadOutputTypeDef",
-    {
-        "Location": str,
-        "Bucket": str,
-        "Key": str,
-        "Expiration": str,
-        "ETag": str,
-        "ChecksumCRC32": str,
-        "ChecksumCRC32C": str,
-        "ChecksumSHA1": str,
-        "ChecksumSHA256": str,
-        "ServerSideEncryption": ServerSideEncryptionType,
-        "VersionId": str,
-        "SSEKMSKeyId": str,
-        "BucketKeyEnabled": bool,
-        "RequestCharged": Literal["requester"],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
 )
 
 CompletedPartTypeDef = TypedDict(
     "CompletedPartTypeDef",
     {
         "ETag": str,
         "ChecksumCRC32": str,
@@ -895,28 +875,26 @@
 
 ConditionTypeDef = TypedDict(
     "ConditionTypeDef",
     {
         "HttpErrorCodeReturnedEquals": str,
         "KeyPrefixEquals": str,
     },
-    total=False,
 )
 
 CopyObjectResultTypeDef = TypedDict(
     "CopyObjectResultTypeDef",
     {
         "ETag": str,
         "LastModified": datetime,
         "ChecksumCRC32": str,
         "ChecksumCRC32C": str,
         "ChecksumSHA1": str,
         "ChecksumSHA256": str,
     },
-    total=False,
 )
 
 _RequiredCopyObjectRequestObjectCopyFromTypeDef = TypedDict(
     "_RequiredCopyObjectRequestObjectCopyFromTypeDef",
     {
         "CopySource": str,
     },
@@ -962,19 +940,21 @@
         "ObjectLockLegalHoldStatus": ObjectLockLegalHoldStatusType,
         "ExpectedBucketOwner": str,
         "ExpectedSourceBucketOwner": str,
     },
     total=False,
 )
 
+
 class CopyObjectRequestObjectCopyFromTypeDef(
     _RequiredCopyObjectRequestObjectCopyFromTypeDef, _OptionalCopyObjectRequestObjectCopyFromTypeDef
 ):
     pass
 
+
 _RequiredCopyObjectRequestObjectSummaryCopyFromTypeDef = TypedDict(
     "_RequiredCopyObjectRequestObjectSummaryCopyFromTypeDef",
     {
         "CopySource": str,
     },
 )
 _OptionalCopyObjectRequestObjectSummaryCopyFromTypeDef = TypedDict(
@@ -1018,69 +998,42 @@
         "ObjectLockLegalHoldStatus": ObjectLockLegalHoldStatusType,
         "ExpectedBucketOwner": str,
         "ExpectedSourceBucketOwner": str,
     },
     total=False,
 )
 
+
 class CopyObjectRequestObjectSummaryCopyFromTypeDef(
     _RequiredCopyObjectRequestObjectSummaryCopyFromTypeDef,
     _OptionalCopyObjectRequestObjectSummaryCopyFromTypeDef,
 ):
     pass
 
+
 CopyPartResultTypeDef = TypedDict(
     "CopyPartResultTypeDef",
     {
         "ETag": str,
         "LastModified": datetime,
         "ChecksumCRC32": str,
         "ChecksumCRC32C": str,
         "ChecksumSHA1": str,
         "ChecksumSHA256": str,
     },
-    total=False,
 )
 
 CreateBucketConfigurationTypeDef = TypedDict(
     "CreateBucketConfigurationTypeDef",
     {
         "LocationConstraint": BucketLocationConstraintType,
     },
     total=False,
 )
 
-CreateBucketOutputTypeDef = TypedDict(
-    "CreateBucketOutputTypeDef",
-    {
-        "Location": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateMultipartUploadOutputTypeDef = TypedDict(
-    "CreateMultipartUploadOutputTypeDef",
-    {
-        "AbortDate": datetime,
-        "AbortRuleId": str,
-        "Bucket": str,
-        "Key": str,
-        "UploadId": str,
-        "ServerSideEncryption": ServerSideEncryptionType,
-        "SSECustomerAlgorithm": str,
-        "SSECustomerKeyMD5": str,
-        "SSEKMSKeyId": str,
-        "SSEKMSEncryptionContext": str,
-        "BucketKeyEnabled": bool,
-        "RequestCharged": Literal["requester"],
-        "ChecksumAlgorithm": ChecksumAlgorithmType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CreateMultipartUploadRequestObjectInitiateMultipartUploadTypeDef = TypedDict(
     "CreateMultipartUploadRequestObjectInitiateMultipartUploadTypeDef",
     {
         "ACL": ObjectCannedACLType,
         "CacheControl": str,
         "ContentDisposition": str,
         "ContentEncoding": str,
@@ -1185,28 +1138,29 @@
         "ObjectLockLegalHoldStatus": ObjectLockLegalHoldStatusType,
         "ExpectedBucketOwner": str,
         "ChecksumAlgorithm": ChecksumAlgorithmType,
     },
     total=False,
 )
 
+
 class CreateMultipartUploadRequestRequestTypeDef(
     _RequiredCreateMultipartUploadRequestRequestTypeDef,
     _OptionalCreateMultipartUploadRequestRequestTypeDef,
 ):
     pass
 
+
 DefaultRetentionTypeDef = TypedDict(
     "DefaultRetentionTypeDef",
     {
         "Mode": ObjectLockRetentionModeType,
         "Days": int,
         "Years": int,
     },
-    total=False,
 )
 
 _RequiredDeleteBucketAnalyticsConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteBucketAnalyticsConfigurationRequestRequestTypeDef",
     {
         "Bucket": str,
         "Id": str,
@@ -1216,20 +1170,22 @@
     "_OptionalDeleteBucketAnalyticsConfigurationRequestRequestTypeDef",
     {
         "ExpectedBucketOwner": str,
     },
     total=False,
 )
 
+
 class DeleteBucketAnalyticsConfigurationRequestRequestTypeDef(
     _RequiredDeleteBucketAnalyticsConfigurationRequestRequestTypeDef,
     _OptionalDeleteBucketAnalyticsConfigurationRequestRequestTypeDef,
 ):
     pass
 
+
 DeleteBucketCorsRequestBucketCorsDeleteTypeDef = TypedDict(
     "DeleteBucketCorsRequestBucketCorsDeleteTypeDef",
     {
         "ExpectedBucketOwner": str,
     },
     total=False,
 )
@@ -1244,39 +1200,43 @@
     "_OptionalDeleteBucketCorsRequestRequestTypeDef",
     {
         "ExpectedBucketOwner": str,
     },
     total=False,
 )
 
+
 class DeleteBucketCorsRequestRequestTypeDef(
     _RequiredDeleteBucketCorsRequestRequestTypeDef, _OptionalDeleteBucketCorsRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredDeleteBucketEncryptionRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteBucketEncryptionRequestRequestTypeDef",
     {
         "Bucket": str,
     },
 )
 _OptionalDeleteBucketEncryptionRequestRequestTypeDef = TypedDict(
     "_OptionalDeleteBucketEncryptionRequestRequestTypeDef",
     {
         "ExpectedBucketOwner": str,
     },
     total=False,
 )
 
+
 class DeleteBucketEncryptionRequestRequestTypeDef(
     _RequiredDeleteBucketEncryptionRequestRequestTypeDef,
     _OptionalDeleteBucketEncryptionRequestRequestTypeDef,
 ):
     pass
 
+
 DeleteBucketIntelligentTieringConfigurationRequestRequestTypeDef = TypedDict(
     "DeleteBucketIntelligentTieringConfigurationRequestRequestTypeDef",
     {
         "Bucket": str,
         "Id": str,
     },
 )
@@ -1292,20 +1252,22 @@
     "_OptionalDeleteBucketInventoryConfigurationRequestRequestTypeDef",
     {
         "ExpectedBucketOwner": str,
     },
     total=False,
 )
 
+
 class DeleteBucketInventoryConfigurationRequestRequestTypeDef(
     _RequiredDeleteBucketInventoryConfigurationRequestRequestTypeDef,
     _OptionalDeleteBucketInventoryConfigurationRequestRequestTypeDef,
 ):
     pass
 
+
 DeleteBucketLifecycleRequestBucketLifecycleConfigurationDeleteTypeDef = TypedDict(
     "DeleteBucketLifecycleRequestBucketLifecycleConfigurationDeleteTypeDef",
     {
         "ExpectedBucketOwner": str,
     },
     total=False,
 )
@@ -1328,20 +1290,22 @@
     "_OptionalDeleteBucketLifecycleRequestRequestTypeDef",
     {
         "ExpectedBucketOwner": str,
     },
     total=False,
 )
 
+
 class DeleteBucketLifecycleRequestRequestTypeDef(
     _RequiredDeleteBucketLifecycleRequestRequestTypeDef,
     _OptionalDeleteBucketLifecycleRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredDeleteBucketMetricsConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteBucketMetricsConfigurationRequestRequestTypeDef",
     {
         "Bucket": str,
         "Id": str,
     },
 )
@@ -1349,40 +1313,44 @@
     "_OptionalDeleteBucketMetricsConfigurationRequestRequestTypeDef",
     {
         "ExpectedBucketOwner": str,
     },
     total=False,
 )
 
+
 class DeleteBucketMetricsConfigurationRequestRequestTypeDef(
     _RequiredDeleteBucketMetricsConfigurationRequestRequestTypeDef,
     _OptionalDeleteBucketMetricsConfigurationRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredDeleteBucketOwnershipControlsRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteBucketOwnershipControlsRequestRequestTypeDef",
     {
         "Bucket": str,
     },
 )
 _OptionalDeleteBucketOwnershipControlsRequestRequestTypeDef = TypedDict(
     "_OptionalDeleteBucketOwnershipControlsRequestRequestTypeDef",
     {
         "ExpectedBucketOwner": str,
     },
     total=False,
 )
 
+
 class DeleteBucketOwnershipControlsRequestRequestTypeDef(
     _RequiredDeleteBucketOwnershipControlsRequestRequestTypeDef,
     _OptionalDeleteBucketOwnershipControlsRequestRequestTypeDef,
 ):
     pass
 
+
 DeleteBucketPolicyRequestBucketPolicyDeleteTypeDef = TypedDict(
     "DeleteBucketPolicyRequestBucketPolicyDeleteTypeDef",
     {
         "ExpectedBucketOwner": str,
     },
     total=False,
 )
@@ -1397,40 +1365,44 @@
     "_OptionalDeleteBucketPolicyRequestRequestTypeDef",
     {
         "ExpectedBucketOwner": str,
     },
     total=False,
 )
 
+
 class DeleteBucketPolicyRequestRequestTypeDef(
     _RequiredDeleteBucketPolicyRequestRequestTypeDef,
     _OptionalDeleteBucketPolicyRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredDeleteBucketReplicationRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteBucketReplicationRequestRequestTypeDef",
     {
         "Bucket": str,
     },
 )
 _OptionalDeleteBucketReplicationRequestRequestTypeDef = TypedDict(
     "_OptionalDeleteBucketReplicationRequestRequestTypeDef",
     {
         "ExpectedBucketOwner": str,
     },
     total=False,
 )
 
+
 class DeleteBucketReplicationRequestRequestTypeDef(
     _RequiredDeleteBucketReplicationRequestRequestTypeDef,
     _OptionalDeleteBucketReplicationRequestRequestTypeDef,
 ):
     pass
 
+
 DeleteBucketRequestBucketDeleteTypeDef = TypedDict(
     "DeleteBucketRequestBucketDeleteTypeDef",
     {
         "ExpectedBucketOwner": str,
     },
     total=False,
 )
@@ -1445,19 +1417,21 @@
     "_OptionalDeleteBucketRequestRequestTypeDef",
     {
         "ExpectedBucketOwner": str,
     },
     total=False,
 )
 
+
 class DeleteBucketRequestRequestTypeDef(
     _RequiredDeleteBucketRequestRequestTypeDef, _OptionalDeleteBucketRequestRequestTypeDef
 ):
     pass
 
+
 DeleteBucketTaggingRequestBucketTaggingDeleteTypeDef = TypedDict(
     "DeleteBucketTaggingRequestBucketTaggingDeleteTypeDef",
     {
         "ExpectedBucketOwner": str,
     },
     total=False,
 )
@@ -1472,20 +1446,22 @@
     "_OptionalDeleteBucketTaggingRequestRequestTypeDef",
     {
         "ExpectedBucketOwner": str,
     },
     total=False,
 )
 
+
 class DeleteBucketTaggingRequestRequestTypeDef(
     _RequiredDeleteBucketTaggingRequestRequestTypeDef,
     _OptionalDeleteBucketTaggingRequestRequestTypeDef,
 ):
     pass
 
+
 DeleteBucketWebsiteRequestBucketWebsiteDeleteTypeDef = TypedDict(
     "DeleteBucketWebsiteRequestBucketWebsiteDeleteTypeDef",
     {
         "ExpectedBucketOwner": str,
     },
     total=False,
 )
@@ -1500,36 +1476,27 @@
     "_OptionalDeleteBucketWebsiteRequestRequestTypeDef",
     {
         "ExpectedBucketOwner": str,
     },
     total=False,
 )
 
+
 class DeleteBucketWebsiteRequestRequestTypeDef(
     _RequiredDeleteBucketWebsiteRequestRequestTypeDef,
     _OptionalDeleteBucketWebsiteRequestRequestTypeDef,
 ):
     pass
 
+
 DeleteMarkerReplicationTypeDef = TypedDict(
     "DeleteMarkerReplicationTypeDef",
     {
         "Status": DeleteMarkerReplicationStatusType,
     },
-    total=False,
-)
-
-DeleteObjectOutputTypeDef = TypedDict(
-    "DeleteObjectOutputTypeDef",
-    {
-        "DeleteMarker": bool,
-        "VersionId": str,
-        "RequestCharged": Literal["requester"],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
 )
 
 DeleteObjectRequestObjectDeleteTypeDef = TypedDict(
     "DeleteObjectRequestObjectDeleteTypeDef",
     {
         "MFA": str,
         "VersionId": str,
@@ -1578,26 +1545,20 @@
         "RequestPayer": Literal["requester"],
         "BypassGovernanceRetention": bool,
         "ExpectedBucketOwner": str,
     },
     total=False,
 )
 
+
 class DeleteObjectRequestRequestTypeDef(
     _RequiredDeleteObjectRequestRequestTypeDef, _OptionalDeleteObjectRequestRequestTypeDef
 ):
     pass
 
-DeleteObjectTaggingOutputTypeDef = TypedDict(
-    "DeleteObjectTaggingOutputTypeDef",
-    {
-        "VersionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 _RequiredDeleteObjectTaggingRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteObjectTaggingRequestRequestTypeDef",
     {
         "Bucket": str,
         "Key": str,
     },
@@ -1607,40 +1568,40 @@
     {
         "VersionId": str,
         "ExpectedBucketOwner": str,
     },
     total=False,
 )
 
+
 class DeleteObjectTaggingRequestRequestTypeDef(
     _RequiredDeleteObjectTaggingRequestRequestTypeDef,
     _OptionalDeleteObjectTaggingRequestRequestTypeDef,
 ):
     pass
 
+
 DeletedObjectTypeDef = TypedDict(
     "DeletedObjectTypeDef",
     {
         "Key": str,
         "VersionId": str,
         "DeleteMarker": bool,
         "DeleteMarkerVersionId": str,
     },
-    total=False,
 )
 
 ErrorTypeDef = TypedDict(
     "ErrorTypeDef",
     {
         "Key": str,
         "VersionId": str,
         "Code": str,
         "Message": str,
     },
-    total=False,
 )
 
 _RequiredDeletePublicAccessBlockRequestRequestTypeDef = TypedDict(
     "_RequiredDeletePublicAccessBlockRequestRequestTypeDef",
     {
         "Bucket": str,
     },
@@ -1649,50 +1610,46 @@
     "_OptionalDeletePublicAccessBlockRequestRequestTypeDef",
     {
         "ExpectedBucketOwner": str,
     },
     total=False,
 )
 
+
 class DeletePublicAccessBlockRequestRequestTypeDef(
     _RequiredDeletePublicAccessBlockRequestRequestTypeDef,
     _OptionalDeletePublicAccessBlockRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredObjectIdentifierTypeDef = TypedDict(
     "_RequiredObjectIdentifierTypeDef",
     {
         "Key": str,
     },
 )
 _OptionalObjectIdentifierTypeDef = TypedDict(
     "_OptionalObjectIdentifierTypeDef",
     {
         "VersionId": str,
     },
     total=False,
 )
 
+
 class ObjectIdentifierTypeDef(_RequiredObjectIdentifierTypeDef, _OptionalObjectIdentifierTypeDef):
     pass
 
+
 EncryptionConfigurationTypeDef = TypedDict(
     "EncryptionConfigurationTypeDef",
     {
         "ReplicaKmsKeyID": str,
     },
-    total=False,
-)
-
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
 )
 
 _RequiredEncryptionTypeDef = TypedDict(
     "_RequiredEncryptionTypeDef",
     {
         "EncryptionType": ServerSideEncryptionType,
     },
@@ -1702,24 +1659,18 @@
     {
         "KMSKeyId": str,
         "KMSContext": str,
     },
     total=False,
 )
 
+
 class EncryptionTypeDef(_RequiredEncryptionTypeDef, _OptionalEncryptionTypeDef):
     pass
 
-ErrorDocumentResponseMetadataTypeDef = TypedDict(
-    "ErrorDocumentResponseMetadataTypeDef",
-    {
-        "Key": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 ErrorDocumentTypeDef = TypedDict(
     "ErrorDocumentTypeDef",
     {
         "Key": str,
     },
 )
@@ -1733,24 +1684,14 @@
 
 FilterRuleTypeDef = TypedDict(
     "FilterRuleTypeDef",
     {
         "Name": FilterRuleNameType,
         "Value": str,
     },
-    total=False,
-)
-
-GetBucketAccelerateConfigurationOutputTypeDef = TypedDict(
-    "GetBucketAccelerateConfigurationOutputTypeDef",
-    {
-        "Status": BucketAccelerateStatusType,
-        "RequestCharged": Literal["requester"],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
 )
 
 _RequiredGetBucketAccelerateConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredGetBucketAccelerateConfigurationRequestRequestTypeDef",
     {
         "Bucket": str,
     },
@@ -1760,39 +1701,43 @@
     {
         "ExpectedBucketOwner": str,
         "RequestPayer": Literal["requester"],
     },
     total=False,
 )
 
+
 class GetBucketAccelerateConfigurationRequestRequestTypeDef(
     _RequiredGetBucketAccelerateConfigurationRequestRequestTypeDef,
     _OptionalGetBucketAccelerateConfigurationRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredGetBucketAclRequestRequestTypeDef = TypedDict(
     "_RequiredGetBucketAclRequestRequestTypeDef",
     {
         "Bucket": str,
     },
 )
 _OptionalGetBucketAclRequestRequestTypeDef = TypedDict(
     "_OptionalGetBucketAclRequestRequestTypeDef",
     {
         "ExpectedBucketOwner": str,
     },
     total=False,
 )
 
+
 class GetBucketAclRequestRequestTypeDef(
     _RequiredGetBucketAclRequestRequestTypeDef, _OptionalGetBucketAclRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredGetBucketAnalyticsConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredGetBucketAnalyticsConfigurationRequestRequestTypeDef",
     {
         "Bucket": str,
         "Id": str,
     },
 )
@@ -1800,59 +1745,65 @@
     "_OptionalGetBucketAnalyticsConfigurationRequestRequestTypeDef",
     {
         "ExpectedBucketOwner": str,
     },
     total=False,
 )
 
+
 class GetBucketAnalyticsConfigurationRequestRequestTypeDef(
     _RequiredGetBucketAnalyticsConfigurationRequestRequestTypeDef,
     _OptionalGetBucketAnalyticsConfigurationRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredGetBucketCorsRequestRequestTypeDef = TypedDict(
     "_RequiredGetBucketCorsRequestRequestTypeDef",
     {
         "Bucket": str,
     },
 )
 _OptionalGetBucketCorsRequestRequestTypeDef = TypedDict(
     "_OptionalGetBucketCorsRequestRequestTypeDef",
     {
         "ExpectedBucketOwner": str,
     },
     total=False,
 )
 
+
 class GetBucketCorsRequestRequestTypeDef(
     _RequiredGetBucketCorsRequestRequestTypeDef, _OptionalGetBucketCorsRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredGetBucketEncryptionRequestRequestTypeDef = TypedDict(
     "_RequiredGetBucketEncryptionRequestRequestTypeDef",
     {
         "Bucket": str,
     },
 )
 _OptionalGetBucketEncryptionRequestRequestTypeDef = TypedDict(
     "_OptionalGetBucketEncryptionRequestRequestTypeDef",
     {
         "ExpectedBucketOwner": str,
     },
     total=False,
 )
 
+
 class GetBucketEncryptionRequestRequestTypeDef(
     _RequiredGetBucketEncryptionRequestRequestTypeDef,
     _OptionalGetBucketEncryptionRequestRequestTypeDef,
 ):
     pass
 
+
 GetBucketIntelligentTieringConfigurationRequestRequestTypeDef = TypedDict(
     "GetBucketIntelligentTieringConfigurationRequestRequestTypeDef",
     {
         "Bucket": str,
         "Id": str,
     },
 )
@@ -1868,67 +1819,65 @@
     "_OptionalGetBucketInventoryConfigurationRequestRequestTypeDef",
     {
         "ExpectedBucketOwner": str,
     },
     total=False,
 )
 
+
 class GetBucketInventoryConfigurationRequestRequestTypeDef(
     _RequiredGetBucketInventoryConfigurationRequestRequestTypeDef,
     _OptionalGetBucketInventoryConfigurationRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredGetBucketLifecycleConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredGetBucketLifecycleConfigurationRequestRequestTypeDef",
     {
         "Bucket": str,
     },
 )
 _OptionalGetBucketLifecycleConfigurationRequestRequestTypeDef = TypedDict(
     "_OptionalGetBucketLifecycleConfigurationRequestRequestTypeDef",
     {
         "ExpectedBucketOwner": str,
     },
     total=False,
 )
 
+
 class GetBucketLifecycleConfigurationRequestRequestTypeDef(
     _RequiredGetBucketLifecycleConfigurationRequestRequestTypeDef,
     _OptionalGetBucketLifecycleConfigurationRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredGetBucketLifecycleRequestRequestTypeDef = TypedDict(
     "_RequiredGetBucketLifecycleRequestRequestTypeDef",
     {
         "Bucket": str,
     },
 )
 _OptionalGetBucketLifecycleRequestRequestTypeDef = TypedDict(
     "_OptionalGetBucketLifecycleRequestRequestTypeDef",
     {
         "ExpectedBucketOwner": str,
     },
     total=False,
 )
 
+
 class GetBucketLifecycleRequestRequestTypeDef(
     _RequiredGetBucketLifecycleRequestRequestTypeDef,
     _OptionalGetBucketLifecycleRequestRequestTypeDef,
 ):
     pass
 
-GetBucketLocationOutputTypeDef = TypedDict(
-    "GetBucketLocationOutputTypeDef",
-    {
-        "LocationConstraint": BucketLocationConstraintType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 _RequiredGetBucketLocationRequestRequestTypeDef = TypedDict(
     "_RequiredGetBucketLocationRequestRequestTypeDef",
     {
         "Bucket": str,
     },
 )
@@ -1936,38 +1885,42 @@
     "_OptionalGetBucketLocationRequestRequestTypeDef",
     {
         "ExpectedBucketOwner": str,
     },
     total=False,
 )
 
+
 class GetBucketLocationRequestRequestTypeDef(
     _RequiredGetBucketLocationRequestRequestTypeDef, _OptionalGetBucketLocationRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredGetBucketLoggingRequestRequestTypeDef = TypedDict(
     "_RequiredGetBucketLoggingRequestRequestTypeDef",
     {
         "Bucket": str,
     },
 )
 _OptionalGetBucketLoggingRequestRequestTypeDef = TypedDict(
     "_OptionalGetBucketLoggingRequestRequestTypeDef",
     {
         "ExpectedBucketOwner": str,
     },
     total=False,
 )
 
+
 class GetBucketLoggingRequestRequestTypeDef(
     _RequiredGetBucketLoggingRequestRequestTypeDef, _OptionalGetBucketLoggingRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredGetBucketMetricsConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredGetBucketMetricsConfigurationRequestRequestTypeDef",
     {
         "Bucket": str,
         "Id": str,
     },
 )
@@ -1975,67 +1928,65 @@
     "_OptionalGetBucketMetricsConfigurationRequestRequestTypeDef",
     {
         "ExpectedBucketOwner": str,
     },
     total=False,
 )
 
+
 class GetBucketMetricsConfigurationRequestRequestTypeDef(
     _RequiredGetBucketMetricsConfigurationRequestRequestTypeDef,
     _OptionalGetBucketMetricsConfigurationRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredGetBucketNotificationConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredGetBucketNotificationConfigurationRequestRequestTypeDef",
     {
         "Bucket": str,
     },
 )
 _OptionalGetBucketNotificationConfigurationRequestRequestTypeDef = TypedDict(
     "_OptionalGetBucketNotificationConfigurationRequestRequestTypeDef",
     {
         "ExpectedBucketOwner": str,
     },
     total=False,
 )
 
+
 class GetBucketNotificationConfigurationRequestRequestTypeDef(
     _RequiredGetBucketNotificationConfigurationRequestRequestTypeDef,
     _OptionalGetBucketNotificationConfigurationRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredGetBucketOwnershipControlsRequestRequestTypeDef = TypedDict(
     "_RequiredGetBucketOwnershipControlsRequestRequestTypeDef",
     {
         "Bucket": str,
     },
 )
 _OptionalGetBucketOwnershipControlsRequestRequestTypeDef = TypedDict(
     "_OptionalGetBucketOwnershipControlsRequestRequestTypeDef",
     {
         "ExpectedBucketOwner": str,
     },
     total=False,
 )
 
+
 class GetBucketOwnershipControlsRequestRequestTypeDef(
     _RequiredGetBucketOwnershipControlsRequestRequestTypeDef,
     _OptionalGetBucketOwnershipControlsRequestRequestTypeDef,
 ):
     pass
 
-GetBucketPolicyOutputTypeDef = TypedDict(
-    "GetBucketPolicyOutputTypeDef",
-    {
-        "Policy": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 _RequiredGetBucketPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredGetBucketPolicyRequestRequestTypeDef",
     {
         "Bucket": str,
     },
 )
@@ -2043,25 +1994,26 @@
     "_OptionalGetBucketPolicyRequestRequestTypeDef",
     {
         "ExpectedBucketOwner": str,
     },
     total=False,
 )
 
+
 class GetBucketPolicyRequestRequestTypeDef(
     _RequiredGetBucketPolicyRequestRequestTypeDef, _OptionalGetBucketPolicyRequestRequestTypeDef
 ):
     pass
 
+
 PolicyStatusTypeDef = TypedDict(
     "PolicyStatusTypeDef",
     {
         "IsPublic": bool,
     },
-    total=False,
 )
 
 _RequiredGetBucketPolicyStatusRequestRequestTypeDef = TypedDict(
     "_RequiredGetBucketPolicyStatusRequestRequestTypeDef",
     {
         "Bucket": str,
     },
@@ -2070,47 +2022,43 @@
     "_OptionalGetBucketPolicyStatusRequestRequestTypeDef",
     {
         "ExpectedBucketOwner": str,
     },
     total=False,
 )
 
+
 class GetBucketPolicyStatusRequestRequestTypeDef(
     _RequiredGetBucketPolicyStatusRequestRequestTypeDef,
     _OptionalGetBucketPolicyStatusRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredGetBucketReplicationRequestRequestTypeDef = TypedDict(
     "_RequiredGetBucketReplicationRequestRequestTypeDef",
     {
         "Bucket": str,
     },
 )
 _OptionalGetBucketReplicationRequestRequestTypeDef = TypedDict(
     "_OptionalGetBucketReplicationRequestRequestTypeDef",
     {
         "ExpectedBucketOwner": str,
     },
     total=False,
 )
 
+
 class GetBucketReplicationRequestRequestTypeDef(
     _RequiredGetBucketReplicationRequestRequestTypeDef,
     _OptionalGetBucketReplicationRequestRequestTypeDef,
 ):
     pass
 
-GetBucketRequestPaymentOutputTypeDef = TypedDict(
-    "GetBucketRequestPaymentOutputTypeDef",
-    {
-        "Payer": PayerType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 _RequiredGetBucketRequestPaymentRequestRequestTypeDef = TypedDict(
     "_RequiredGetBucketRequestPaymentRequestRequestTypeDef",
     {
         "Bucket": str,
     },
 )
@@ -2118,47 +2066,42 @@
     "_OptionalGetBucketRequestPaymentRequestRequestTypeDef",
     {
         "ExpectedBucketOwner": str,
     },
     total=False,
 )
 
+
 class GetBucketRequestPaymentRequestRequestTypeDef(
     _RequiredGetBucketRequestPaymentRequestRequestTypeDef,
     _OptionalGetBucketRequestPaymentRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredGetBucketTaggingRequestRequestTypeDef = TypedDict(
     "_RequiredGetBucketTaggingRequestRequestTypeDef",
     {
         "Bucket": str,
     },
 )
 _OptionalGetBucketTaggingRequestRequestTypeDef = TypedDict(
     "_OptionalGetBucketTaggingRequestRequestTypeDef",
     {
         "ExpectedBucketOwner": str,
     },
     total=False,
 )
 
+
 class GetBucketTaggingRequestRequestTypeDef(
     _RequiredGetBucketTaggingRequestRequestTypeDef, _OptionalGetBucketTaggingRequestRequestTypeDef
 ):
     pass
 
-GetBucketVersioningOutputTypeDef = TypedDict(
-    "GetBucketVersioningOutputTypeDef",
-    {
-        "Status": BucketVersioningStatusType,
-        "MFADelete": MFADeleteStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 _RequiredGetBucketVersioningRequestRequestTypeDef = TypedDict(
     "_RequiredGetBucketVersioningRequestRequestTypeDef",
     {
         "Bucket": str,
     },
 )
@@ -2166,65 +2109,58 @@
     "_OptionalGetBucketVersioningRequestRequestTypeDef",
     {
         "ExpectedBucketOwner": str,
     },
     total=False,
 )
 
+
 class GetBucketVersioningRequestRequestTypeDef(
     _RequiredGetBucketVersioningRequestRequestTypeDef,
     _OptionalGetBucketVersioningRequestRequestTypeDef,
 ):
     pass
 
+
 IndexDocumentTypeDef = TypedDict(
     "IndexDocumentTypeDef",
     {
         "Suffix": str,
     },
 )
 
-_RequiredRedirectAllRequestsToTypeDef = TypedDict(
-    "_RequiredRedirectAllRequestsToTypeDef",
+RedirectAllRequestsToTypeDef = TypedDict(
+    "RedirectAllRequestsToTypeDef",
     {
         "HostName": str,
-    },
-)
-_OptionalRedirectAllRequestsToTypeDef = TypedDict(
-    "_OptionalRedirectAllRequestsToTypeDef",
-    {
         "Protocol": ProtocolType,
     },
-    total=False,
 )
 
-class RedirectAllRequestsToTypeDef(
-    _RequiredRedirectAllRequestsToTypeDef, _OptionalRedirectAllRequestsToTypeDef
-):
-    pass
-
 _RequiredGetBucketWebsiteRequestRequestTypeDef = TypedDict(
     "_RequiredGetBucketWebsiteRequestRequestTypeDef",
     {
         "Bucket": str,
     },
 )
 _OptionalGetBucketWebsiteRequestRequestTypeDef = TypedDict(
     "_OptionalGetBucketWebsiteRequestRequestTypeDef",
     {
         "ExpectedBucketOwner": str,
     },
     total=False,
 )
 
+
 class GetBucketWebsiteRequestRequestTypeDef(
     _RequiredGetBucketWebsiteRequestRequestTypeDef, _OptionalGetBucketWebsiteRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredGetObjectAclRequestRequestTypeDef = TypedDict(
     "_RequiredGetObjectAclRequestRequestTypeDef",
     {
         "Bucket": str,
         "Key": str,
     },
 )
@@ -2234,30 +2170,31 @@
         "VersionId": str,
         "RequestPayer": Literal["requester"],
         "ExpectedBucketOwner": str,
     },
     total=False,
 )
 
+
 class GetObjectAclRequestRequestTypeDef(
     _RequiredGetObjectAclRequestRequestTypeDef, _OptionalGetObjectAclRequestRequestTypeDef
 ):
     pass
 
+
 ObjectPartTypeDef = TypedDict(
     "ObjectPartTypeDef",
     {
         "PartNumber": int,
         "Size": int,
         "ChecksumCRC32": str,
         "ChecksumCRC32C": str,
         "ChecksumSHA1": str,
         "ChecksumSHA256": str,
     },
-    total=False,
 )
 
 _RequiredGetObjectAttributesRequestRequestTypeDef = TypedDict(
     "_RequiredGetObjectAttributesRequestRequestTypeDef",
     {
         "Bucket": str,
         "Key": str,
@@ -2275,26 +2212,27 @@
         "SSECustomerKeyMD5": str,
         "RequestPayer": Literal["requester"],
         "ExpectedBucketOwner": str,
     },
     total=False,
 )
 
+
 class GetObjectAttributesRequestRequestTypeDef(
     _RequiredGetObjectAttributesRequestRequestTypeDef,
     _OptionalGetObjectAttributesRequestRequestTypeDef,
 ):
     pass
 
+
 ObjectLockLegalHoldTypeDef = TypedDict(
     "ObjectLockLegalHoldTypeDef",
     {
         "Status": ObjectLockLegalHoldStatusType,
     },
-    total=False,
 )
 
 _RequiredGetObjectLegalHoldRequestRequestTypeDef = TypedDict(
     "_RequiredGetObjectLegalHoldRequestRequestTypeDef",
     {
         "Bucket": str,
         "Key": str,
@@ -2306,82 +2244,43 @@
         "VersionId": str,
         "RequestPayer": Literal["requester"],
         "ExpectedBucketOwner": str,
     },
     total=False,
 )
 
+
 class GetObjectLegalHoldRequestRequestTypeDef(
     _RequiredGetObjectLegalHoldRequestRequestTypeDef,
     _OptionalGetObjectLegalHoldRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredGetObjectLockConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredGetObjectLockConfigurationRequestRequestTypeDef",
     {
         "Bucket": str,
     },
 )
 _OptionalGetObjectLockConfigurationRequestRequestTypeDef = TypedDict(
     "_OptionalGetObjectLockConfigurationRequestRequestTypeDef",
     {
         "ExpectedBucketOwner": str,
     },
     total=False,
 )
 
+
 class GetObjectLockConfigurationRequestRequestTypeDef(
     _RequiredGetObjectLockConfigurationRequestRequestTypeDef,
     _OptionalGetObjectLockConfigurationRequestRequestTypeDef,
 ):
     pass
 
-GetObjectOutputTypeDef = TypedDict(
-    "GetObjectOutputTypeDef",
-    {
-        "Body": StreamingBody,
-        "DeleteMarker": bool,
-        "AcceptRanges": str,
-        "Expiration": str,
-        "Restore": str,
-        "LastModified": datetime,
-        "ContentLength": int,
-        "ETag": str,
-        "ChecksumCRC32": str,
-        "ChecksumCRC32C": str,
-        "ChecksumSHA1": str,
-        "ChecksumSHA256": str,
-        "MissingMeta": int,
-        "VersionId": str,
-        "CacheControl": str,
-        "ContentDisposition": str,
-        "ContentEncoding": str,
-        "ContentLanguage": str,
-        "ContentRange": str,
-        "ContentType": str,
-        "Expires": datetime,
-        "WebsiteRedirectLocation": str,
-        "ServerSideEncryption": ServerSideEncryptionType,
-        "Metadata": Dict[str, str],
-        "SSECustomerAlgorithm": str,
-        "SSECustomerKeyMD5": str,
-        "SSEKMSKeyId": str,
-        "BucketKeyEnabled": bool,
-        "StorageClass": StorageClassType,
-        "RequestCharged": Literal["requester"],
-        "ReplicationStatus": ReplicationStatusType,
-        "PartsCount": int,
-        "TagCount": int,
-        "ObjectLockMode": ObjectLockModeType,
-        "ObjectLockRetainUntilDate": datetime,
-        "ObjectLockLegalHoldStatus": ObjectLockLegalHoldStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 GetObjectRequestObjectGetTypeDef = TypedDict(
     "GetObjectRequestObjectGetTypeDef",
     {
         "IfMatch": str,
         "IfModifiedSince": Union[datetime, str],
         "IfNoneMatch": str,
@@ -2485,26 +2384,27 @@
         "PartNumber": int,
         "ExpectedBucketOwner": str,
         "ChecksumMode": Literal["ENABLED"],
     },
     total=False,
 )
 
+
 class GetObjectRequestRequestTypeDef(
     _RequiredGetObjectRequestRequestTypeDef, _OptionalGetObjectRequestRequestTypeDef
 ):
     pass
 
+
 ObjectLockRetentionTypeDef = TypedDict(
     "ObjectLockRetentionTypeDef",
     {
         "Mode": ObjectLockRetentionModeType,
         "RetainUntilDate": datetime,
     },
-    total=False,
 )
 
 _RequiredGetObjectRetentionRequestRequestTypeDef = TypedDict(
     "_RequiredGetObjectRetentionRequestRequestTypeDef",
     {
         "Bucket": str,
         "Key": str,
@@ -2516,20 +2416,22 @@
         "VersionId": str,
         "RequestPayer": Literal["requester"],
         "ExpectedBucketOwner": str,
     },
     total=False,
 )
 
+
 class GetObjectRetentionRequestRequestTypeDef(
     _RequiredGetObjectRetentionRequestRequestTypeDef,
     _OptionalGetObjectRetentionRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredGetObjectTaggingRequestRequestTypeDef = TypedDict(
     "_RequiredGetObjectTaggingRequestRequestTypeDef",
     {
         "Bucket": str,
         "Key": str,
     },
 )
@@ -2539,27 +2441,20 @@
         "VersionId": str,
         "ExpectedBucketOwner": str,
         "RequestPayer": Literal["requester"],
     },
     total=False,
 )
 
+
 class GetObjectTaggingRequestRequestTypeDef(
     _RequiredGetObjectTaggingRequestRequestTypeDef, _OptionalGetObjectTaggingRequestRequestTypeDef
 ):
     pass
 
-GetObjectTorrentOutputTypeDef = TypedDict(
-    "GetObjectTorrentOutputTypeDef",
-    {
-        "Body": StreamingBody,
-        "RequestCharged": Literal["requester"],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 _RequiredGetObjectTorrentRequestRequestTypeDef = TypedDict(
     "_RequiredGetObjectTorrentRequestRequestTypeDef",
     {
         "Bucket": str,
         "Key": str,
     },
@@ -2569,28 +2464,29 @@
     {
         "RequestPayer": Literal["requester"],
         "ExpectedBucketOwner": str,
     },
     total=False,
 )
 
+
 class GetObjectTorrentRequestRequestTypeDef(
     _RequiredGetObjectTorrentRequestRequestTypeDef, _OptionalGetObjectTorrentRequestRequestTypeDef
 ):
     pass
 
+
 PublicAccessBlockConfigurationTypeDef = TypedDict(
     "PublicAccessBlockConfigurationTypeDef",
     {
         "BlockPublicAcls": bool,
         "IgnorePublicAcls": bool,
         "BlockPublicPolicy": bool,
         "RestrictPublicBuckets": bool,
     },
-    total=False,
 )
 
 _RequiredGetPublicAccessBlockRequestRequestTypeDef = TypedDict(
     "_RequiredGetPublicAccessBlockRequestRequestTypeDef",
     {
         "Bucket": str,
     },
@@ -2599,47 +2495,40 @@
     "_OptionalGetPublicAccessBlockRequestRequestTypeDef",
     {
         "ExpectedBucketOwner": str,
     },
     total=False,
 )
 
+
 class GetPublicAccessBlockRequestRequestTypeDef(
     _RequiredGetPublicAccessBlockRequestRequestTypeDef,
     _OptionalGetPublicAccessBlockRequestRequestTypeDef,
 ):
     pass
 
+
 GlacierJobParametersTypeDef = TypedDict(
     "GlacierJobParametersTypeDef",
     {
         "Tier": TierType,
     },
 )
 
-_RequiredGranteeTypeDef = TypedDict(
-    "_RequiredGranteeTypeDef",
-    {
-        "Type": TypeType,
-    },
-)
-_OptionalGranteeTypeDef = TypedDict(
-    "_OptionalGranteeTypeDef",
+GranteeTypeDef = TypedDict(
+    "GranteeTypeDef",
     {
         "DisplayName": str,
         "EmailAddress": str,
         "ID": str,
+        "Type": TypeType,
         "URI": str,
     },
-    total=False,
 )
 
-class GranteeTypeDef(_RequiredGranteeTypeDef, _OptionalGranteeTypeDef):
-    pass
-
 WaiterConfigTypeDef = TypedDict(
     "WaiterConfigTypeDef",
     {
         "Delay": int,
         "MaxAttempts": int,
     },
     total=False,
@@ -2655,59 +2544,20 @@
     "_OptionalHeadBucketRequestRequestTypeDef",
     {
         "ExpectedBucketOwner": str,
     },
     total=False,
 )
 
+
 class HeadBucketRequestRequestTypeDef(
     _RequiredHeadBucketRequestRequestTypeDef, _OptionalHeadBucketRequestRequestTypeDef
 ):
     pass
 
-HeadObjectOutputTypeDef = TypedDict(
-    "HeadObjectOutputTypeDef",
-    {
-        "DeleteMarker": bool,
-        "AcceptRanges": str,
-        "Expiration": str,
-        "Restore": str,
-        "ArchiveStatus": ArchiveStatusType,
-        "LastModified": datetime,
-        "ContentLength": int,
-        "ChecksumCRC32": str,
-        "ChecksumCRC32C": str,
-        "ChecksumSHA1": str,
-        "ChecksumSHA256": str,
-        "ETag": str,
-        "MissingMeta": int,
-        "VersionId": str,
-        "CacheControl": str,
-        "ContentDisposition": str,
-        "ContentEncoding": str,
-        "ContentLanguage": str,
-        "ContentType": str,
-        "Expires": datetime,
-        "WebsiteRedirectLocation": str,
-        "ServerSideEncryption": ServerSideEncryptionType,
-        "Metadata": Dict[str, str],
-        "SSECustomerAlgorithm": str,
-        "SSECustomerKeyMD5": str,
-        "SSEKMSKeyId": str,
-        "BucketKeyEnabled": bool,
-        "StorageClass": StorageClassType,
-        "RequestCharged": Literal["requester"],
-        "ReplicationStatus": ReplicationStatusType,
-        "PartsCount": int,
-        "ObjectLockMode": ObjectLockModeType,
-        "ObjectLockRetainUntilDate": datetime,
-        "ObjectLockLegalHoldStatus": ObjectLockLegalHoldStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 HeadObjectRequestObjectVersionHeadTypeDef = TypedDict(
     "HeadObjectRequestObjectVersionHeadTypeDef",
     {
         "IfMatch": str,
         "IfModifiedSince": Union[datetime, str],
         "IfNoneMatch": str,
@@ -2747,43 +2597,27 @@
         "PartNumber": int,
         "ExpectedBucketOwner": str,
         "ChecksumMode": Literal["ENABLED"],
     },
     total=False,
 )
 
+
 class HeadObjectRequestRequestTypeDef(
     _RequiredHeadObjectRequestRequestTypeDef, _OptionalHeadObjectRequestRequestTypeDef
 ):
     pass
 
-IndexDocumentResponseMetadataTypeDef = TypedDict(
-    "IndexDocumentResponseMetadataTypeDef",
-    {
-        "Suffix": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-InitiatorResponseMetadataTypeDef = TypedDict(
-    "InitiatorResponseMetadataTypeDef",
-    {
-        "ID": str,
-        "DisplayName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 InitiatorTypeDef = TypedDict(
     "InitiatorTypeDef",
     {
         "ID": str,
         "DisplayName": str,
     },
-    total=False,
 )
 
 JSONInputTypeDef = TypedDict(
     "JSONInputTypeDef",
     {
         "Type": JSONTypeType,
     },
@@ -2830,44 +2664,40 @@
 LifecycleExpirationTypeDef = TypedDict(
     "LifecycleExpirationTypeDef",
     {
         "Date": datetime,
         "Days": int,
         "ExpiredObjectDeleteMarker": bool,
     },
-    total=False,
 )
 
 NoncurrentVersionExpirationTypeDef = TypedDict(
     "NoncurrentVersionExpirationTypeDef",
     {
         "NoncurrentDays": int,
         "NewerNoncurrentVersions": int,
     },
-    total=False,
 )
 
 NoncurrentVersionTransitionTypeDef = TypedDict(
     "NoncurrentVersionTransitionTypeDef",
     {
         "NoncurrentDays": int,
         "StorageClass": TransitionStorageClassType,
         "NewerNoncurrentVersions": int,
     },
-    total=False,
 )
 
 TransitionTypeDef = TypedDict(
     "TransitionTypeDef",
     {
         "Date": datetime,
         "Days": int,
         "StorageClass": TransitionStorageClassType,
     },
-    total=False,
 )
 
 _RequiredListBucketAnalyticsConfigurationsRequestRequestTypeDef = TypedDict(
     "_RequiredListBucketAnalyticsConfigurationsRequestRequestTypeDef",
     {
         "Bucket": str,
     },
@@ -2877,40 +2707,44 @@
     {
         "ContinuationToken": str,
         "ExpectedBucketOwner": str,
     },
     total=False,
 )
 
+
 class ListBucketAnalyticsConfigurationsRequestRequestTypeDef(
     _RequiredListBucketAnalyticsConfigurationsRequestRequestTypeDef,
     _OptionalListBucketAnalyticsConfigurationsRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredListBucketIntelligentTieringConfigurationsRequestRequestTypeDef = TypedDict(
     "_RequiredListBucketIntelligentTieringConfigurationsRequestRequestTypeDef",
     {
         "Bucket": str,
     },
 )
 _OptionalListBucketIntelligentTieringConfigurationsRequestRequestTypeDef = TypedDict(
     "_OptionalListBucketIntelligentTieringConfigurationsRequestRequestTypeDef",
     {
         "ContinuationToken": str,
     },
     total=False,
 )
 
+
 class ListBucketIntelligentTieringConfigurationsRequestRequestTypeDef(
     _RequiredListBucketIntelligentTieringConfigurationsRequestRequestTypeDef,
     _OptionalListBucketIntelligentTieringConfigurationsRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredListBucketInventoryConfigurationsRequestRequestTypeDef = TypedDict(
     "_RequiredListBucketInventoryConfigurationsRequestRequestTypeDef",
     {
         "Bucket": str,
     },
 )
 _OptionalListBucketInventoryConfigurationsRequestRequestTypeDef = TypedDict(
@@ -2918,20 +2752,22 @@
     {
         "ContinuationToken": str,
         "ExpectedBucketOwner": str,
     },
     total=False,
 )
 
+
 class ListBucketInventoryConfigurationsRequestRequestTypeDef(
     _RequiredListBucketInventoryConfigurationsRequestRequestTypeDef,
     _OptionalListBucketInventoryConfigurationsRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredListBucketMetricsConfigurationsRequestRequestTypeDef = TypedDict(
     "_RequiredListBucketMetricsConfigurationsRequestRequestTypeDef",
     {
         "Bucket": str,
     },
 )
 _OptionalListBucketMetricsConfigurationsRequestRequestTypeDef = TypedDict(
@@ -2939,45 +2775,32 @@
     {
         "ContinuationToken": str,
         "ExpectedBucketOwner": str,
     },
     total=False,
 )
 
+
 class ListBucketMetricsConfigurationsRequestRequestTypeDef(
     _RequiredListBucketMetricsConfigurationsRequestRequestTypeDef,
     _OptionalListBucketMetricsConfigurationsRequestRequestTypeDef,
 ):
     pass
 
-_RequiredListMultipartUploadsRequestListMultipartUploadsPaginateTypeDef = TypedDict(
-    "_RequiredListMultipartUploadsRequestListMultipartUploadsPaginateTypeDef",
-    {
-        "Bucket": str,
-    },
-)
-_OptionalListMultipartUploadsRequestListMultipartUploadsPaginateTypeDef = TypedDict(
-    "_OptionalListMultipartUploadsRequestListMultipartUploadsPaginateTypeDef",
+
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "Delimiter": str,
-        "EncodingType": Literal["url"],
-        "Prefix": str,
-        "ExpectedBucketOwner": str,
-        "RequestPayer": Literal["requester"],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
-class ListMultipartUploadsRequestListMultipartUploadsPaginateTypeDef(
-    _RequiredListMultipartUploadsRequestListMultipartUploadsPaginateTypeDef,
-    _OptionalListMultipartUploadsRequestListMultipartUploadsPaginateTypeDef,
-):
-    pass
-
 _RequiredListMultipartUploadsRequestRequestTypeDef = TypedDict(
     "_RequiredListMultipartUploadsRequestRequestTypeDef",
     {
         "Bucket": str,
     },
 )
 _OptionalListMultipartUploadsRequestRequestTypeDef = TypedDict(
@@ -2991,45 +2814,21 @@
         "UploadIdMarker": str,
         "ExpectedBucketOwner": str,
         "RequestPayer": Literal["requester"],
     },
     total=False,
 )
 
+
 class ListMultipartUploadsRequestRequestTypeDef(
     _RequiredListMultipartUploadsRequestRequestTypeDef,
     _OptionalListMultipartUploadsRequestRequestTypeDef,
 ):
     pass
 
-_RequiredListObjectVersionsRequestListObjectVersionsPaginateTypeDef = TypedDict(
-    "_RequiredListObjectVersionsRequestListObjectVersionsPaginateTypeDef",
-    {
-        "Bucket": str,
-    },
-)
-_OptionalListObjectVersionsRequestListObjectVersionsPaginateTypeDef = TypedDict(
-    "_OptionalListObjectVersionsRequestListObjectVersionsPaginateTypeDef",
-    {
-        "Delimiter": str,
-        "EncodingType": Literal["url"],
-        "Prefix": str,
-        "ExpectedBucketOwner": str,
-        "RequestPayer": Literal["requester"],
-        "OptionalObjectAttributes": Sequence[Literal["RestoreStatus"]],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListObjectVersionsRequestListObjectVersionsPaginateTypeDef(
-    _RequiredListObjectVersionsRequestListObjectVersionsPaginateTypeDef,
-    _OptionalListObjectVersionsRequestListObjectVersionsPaginateTypeDef,
-):
-    pass
 
 _RequiredListObjectVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredListObjectVersionsRequestRequestTypeDef",
     {
         "Bucket": str,
     },
 )
@@ -3045,45 +2844,21 @@
         "ExpectedBucketOwner": str,
         "RequestPayer": Literal["requester"],
         "OptionalObjectAttributes": Sequence[Literal["RestoreStatus"]],
     },
     total=False,
 )
 
+
 class ListObjectVersionsRequestRequestTypeDef(
     _RequiredListObjectVersionsRequestRequestTypeDef,
     _OptionalListObjectVersionsRequestRequestTypeDef,
 ):
     pass
 
-_RequiredListObjectsRequestListObjectsPaginateTypeDef = TypedDict(
-    "_RequiredListObjectsRequestListObjectsPaginateTypeDef",
-    {
-        "Bucket": str,
-    },
-)
-_OptionalListObjectsRequestListObjectsPaginateTypeDef = TypedDict(
-    "_OptionalListObjectsRequestListObjectsPaginateTypeDef",
-    {
-        "Delimiter": str,
-        "EncodingType": Literal["url"],
-        "Prefix": str,
-        "RequestPayer": Literal["requester"],
-        "ExpectedBucketOwner": str,
-        "OptionalObjectAttributes": Sequence[Literal["RestoreStatus"]],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListObjectsRequestListObjectsPaginateTypeDef(
-    _RequiredListObjectsRequestListObjectsPaginateTypeDef,
-    _OptionalListObjectsRequestListObjectsPaginateTypeDef,
-):
-    pass
 
 _RequiredListObjectsRequestRequestTypeDef = TypedDict(
     "_RequiredListObjectsRequestRequestTypeDef",
     {
         "Bucket": str,
     },
 )
@@ -3098,46 +2873,20 @@
         "RequestPayer": Literal["requester"],
         "ExpectedBucketOwner": str,
         "OptionalObjectAttributes": Sequence[Literal["RestoreStatus"]],
     },
     total=False,
 )
 
+
 class ListObjectsRequestRequestTypeDef(
     _RequiredListObjectsRequestRequestTypeDef, _OptionalListObjectsRequestRequestTypeDef
 ):
     pass
 
-_RequiredListObjectsV2RequestListObjectsV2PaginateTypeDef = TypedDict(
-    "_RequiredListObjectsV2RequestListObjectsV2PaginateTypeDef",
-    {
-        "Bucket": str,
-    },
-)
-_OptionalListObjectsV2RequestListObjectsV2PaginateTypeDef = TypedDict(
-    "_OptionalListObjectsV2RequestListObjectsV2PaginateTypeDef",
-    {
-        "Delimiter": str,
-        "EncodingType": Literal["url"],
-        "Prefix": str,
-        "FetchOwner": bool,
-        "StartAfter": str,
-        "RequestPayer": Literal["requester"],
-        "ExpectedBucketOwner": str,
-        "OptionalObjectAttributes": Sequence[Literal["RestoreStatus"]],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListObjectsV2RequestListObjectsV2PaginateTypeDef(
-    _RequiredListObjectsV2RequestListObjectsV2PaginateTypeDef,
-    _OptionalListObjectsV2RequestListObjectsV2PaginateTypeDef,
-):
-    pass
 
 _RequiredListObjectsV2RequestRequestTypeDef = TypedDict(
     "_RequiredListObjectsV2RequestRequestTypeDef",
     {
         "Bucket": str,
     },
 )
@@ -3154,61 +2903,35 @@
         "RequestPayer": Literal["requester"],
         "ExpectedBucketOwner": str,
         "OptionalObjectAttributes": Sequence[Literal["RestoreStatus"]],
     },
     total=False,
 )
 
+
 class ListObjectsV2RequestRequestTypeDef(
     _RequiredListObjectsV2RequestRequestTypeDef, _OptionalListObjectsV2RequestRequestTypeDef
 ):
     pass
 
+
 PartTypeDef = TypedDict(
     "PartTypeDef",
     {
         "PartNumber": int,
         "LastModified": datetime,
         "ETag": str,
         "Size": int,
         "ChecksumCRC32": str,
         "ChecksumCRC32C": str,
         "ChecksumSHA1": str,
         "ChecksumSHA256": str,
     },
-    total=False,
 )
 
-_RequiredListPartsRequestListPartsPaginateTypeDef = TypedDict(
-    "_RequiredListPartsRequestListPartsPaginateTypeDef",
-    {
-        "Bucket": str,
-        "Key": str,
-        "UploadId": str,
-    },
-)
-_OptionalListPartsRequestListPartsPaginateTypeDef = TypedDict(
-    "_OptionalListPartsRequestListPartsPaginateTypeDef",
-    {
-        "RequestPayer": Literal["requester"],
-        "ExpectedBucketOwner": str,
-        "SSECustomerAlgorithm": str,
-        "SSECustomerKey": str,
-        "SSECustomerKeyMD5": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListPartsRequestListPartsPaginateTypeDef(
-    _RequiredListPartsRequestListPartsPaginateTypeDef,
-    _OptionalListPartsRequestListPartsPaginateTypeDef,
-):
-    pass
-
 _RequiredListPartsRequestRequestTypeDef = TypedDict(
     "_RequiredListPartsRequestRequestTypeDef",
     {
         "Bucket": str,
         "Key": str,
         "UploadId": str,
     },
@@ -3223,56 +2946,55 @@
         "SSECustomerAlgorithm": str,
         "SSECustomerKey": str,
         "SSECustomerKeyMD5": str,
     },
     total=False,
 )
 
+
 class ListPartsRequestRequestTypeDef(
     _RequiredListPartsRequestRequestTypeDef, _OptionalListPartsRequestRequestTypeDef
 ):
     pass
 
+
 MetadataEntryTypeDef = TypedDict(
     "MetadataEntryTypeDef",
     {
         "Name": str,
         "Value": str,
     },
     total=False,
 )
 
 ReplicationTimeValueTypeDef = TypedDict(
     "ReplicationTimeValueTypeDef",
     {
         "Minutes": int,
     },
-    total=False,
 )
 
 QueueConfigurationDeprecatedTypeDef = TypedDict(
     "QueueConfigurationDeprecatedTypeDef",
     {
         "Id": str,
         "Event": EventType,
         "Events": List[EventType],
         "Queue": str,
     },
-    total=False,
 )
 
 TopicConfigurationDeprecatedTypeDef = TypedDict(
     "TopicConfigurationDeprecatedTypeDef",
     {
         "Id": str,
         "Events": List[EventType],
         "Event": EventType,
         "Topic": str,
     },
-    total=False,
 )
 
 _RequiredObjectDownloadFileRequestTypeDef = TypedDict(
     "_RequiredObjectDownloadFileRequestTypeDef",
     {
         "Filename": str,
     },
@@ -3283,19 +3005,21 @@
         "ExtraArgs": Dict[str, Any],
         "Callback": Callable[..., Any],
         "Config": TransferConfig,
     },
     total=False,
 )
 
+
 class ObjectDownloadFileRequestTypeDef(
     _RequiredObjectDownloadFileRequestTypeDef, _OptionalObjectDownloadFileRequestTypeDef
 ):
     pass
 
+
 _RequiredObjectDownloadFileobjRequestTypeDef = TypedDict(
     "_RequiredObjectDownloadFileobjRequestTypeDef",
     {
         "Fileobj": Union[IO[Any], StreamingBody],
     },
 )
 _OptionalObjectDownloadFileobjRequestTypeDef = TypedDict(
@@ -3304,26 +3028,27 @@
         "ExtraArgs": Dict[str, Any],
         "Callback": Callable[..., Any],
         "Config": TransferConfig,
     },
     total=False,
 )
 
+
 class ObjectDownloadFileobjRequestTypeDef(
     _RequiredObjectDownloadFileobjRequestTypeDef, _OptionalObjectDownloadFileobjRequestTypeDef
 ):
     pass
 
+
 RestoreStatusTypeDef = TypedDict(
     "RestoreStatusTypeDef",
     {
         "IsRestoreInProgress": bool,
         "RestoreExpiryDate": datetime,
     },
-    total=False,
 )
 
 _RequiredObjectUploadFileRequestTypeDef = TypedDict(
     "_RequiredObjectUploadFileRequestTypeDef",
     {
         "Filename": str,
     },
@@ -3334,19 +3059,21 @@
         "ExtraArgs": Dict[str, Any],
         "Callback": Callable[..., Any],
         "Config": TransferConfig,
     },
     total=False,
 )
 
+
 class ObjectUploadFileRequestTypeDef(
     _RequiredObjectUploadFileRequestTypeDef, _OptionalObjectUploadFileRequestTypeDef
 ):
     pass
 
+
 _RequiredObjectUploadFileobjRequestTypeDef = TypedDict(
     "_RequiredObjectUploadFileobjRequestTypeDef",
     {
         "Fileobj": Union[IO[Any], StreamingBody],
     },
 )
 _OptionalObjectUploadFileobjRequestTypeDef = TypedDict(
@@ -3355,53 +3082,35 @@
         "ExtraArgs": Dict[str, Any],
         "Callback": Callable[..., Any],
         "Config": TransferConfig,
     },
     total=False,
 )
 
+
 class ObjectUploadFileobjRequestTypeDef(
     _RequiredObjectUploadFileobjRequestTypeDef, _OptionalObjectUploadFileobjRequestTypeDef
 ):
     pass
 
-OwnerResponseMetadataTypeDef = TypedDict(
-    "OwnerResponseMetadataTypeDef",
-    {
-        "DisplayName": str,
-        "ID": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 OwnershipControlsRuleTypeDef = TypedDict(
     "OwnershipControlsRuleTypeDef",
     {
         "ObjectOwnership": ObjectOwnershipType,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
-    {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
-    },
-    total=False,
-)
-
 ProgressTypeDef = TypedDict(
     "ProgressTypeDef",
     {
         "BytesScanned": int,
         "BytesProcessed": int,
         "BytesReturned": int,
     },
-    total=False,
 )
 
 _RequiredPutBucketPolicyRequestBucketPolicyPutTypeDef = TypedDict(
     "_RequiredPutBucketPolicyRequestBucketPolicyPutTypeDef",
     {
         "Policy": str,
     },
@@ -3412,20 +3121,22 @@
         "ChecksumAlgorithm": ChecksumAlgorithmType,
         "ConfirmRemoveSelfBucketAccess": bool,
         "ExpectedBucketOwner": str,
     },
     total=False,
 )
 
+
 class PutBucketPolicyRequestBucketPolicyPutTypeDef(
     _RequiredPutBucketPolicyRequestBucketPolicyPutTypeDef,
     _OptionalPutBucketPolicyRequestBucketPolicyPutTypeDef,
 ):
     pass
 
+
 _RequiredPutBucketPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredPutBucketPolicyRequestRequestTypeDef",
     {
         "Bucket": str,
         "Policy": str,
     },
 )
@@ -3435,19 +3146,21 @@
         "ChecksumAlgorithm": ChecksumAlgorithmType,
         "ConfirmRemoveSelfBucketAccess": bool,
         "ExpectedBucketOwner": str,
     },
     total=False,
 )
 
+
 class PutBucketPolicyRequestRequestTypeDef(
     _RequiredPutBucketPolicyRequestRequestTypeDef, _OptionalPutBucketPolicyRequestRequestTypeDef
 ):
     pass
 
+
 RequestPaymentConfigurationTypeDef = TypedDict(
     "RequestPaymentConfigurationTypeDef",
     {
         "Payer": PayerType,
     },
 )
 
@@ -3476,59 +3189,14 @@
         "ChecksumAlgorithm": ChecksumAlgorithmType,
         "MFA": str,
         "ExpectedBucketOwner": str,
     },
     total=False,
 )
 
-PutObjectAclOutputTypeDef = TypedDict(
-    "PutObjectAclOutputTypeDef",
-    {
-        "RequestCharged": Literal["requester"],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-PutObjectLegalHoldOutputTypeDef = TypedDict(
-    "PutObjectLegalHoldOutputTypeDef",
-    {
-        "RequestCharged": Literal["requester"],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-PutObjectLockConfigurationOutputTypeDef = TypedDict(
-    "PutObjectLockConfigurationOutputTypeDef",
-    {
-        "RequestCharged": Literal["requester"],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-PutObjectOutputTypeDef = TypedDict(
-    "PutObjectOutputTypeDef",
-    {
-        "Expiration": str,
-        "ETag": str,
-        "ChecksumCRC32": str,
-        "ChecksumCRC32C": str,
-        "ChecksumSHA1": str,
-        "ChecksumSHA256": str,
-        "ServerSideEncryption": ServerSideEncryptionType,
-        "VersionId": str,
-        "SSECustomerAlgorithm": str,
-        "SSECustomerKeyMD5": str,
-        "SSEKMSKeyId": str,
-        "SSEKMSEncryptionContext": str,
-        "BucketKeyEnabled": bool,
-        "RequestCharged": Literal["requester"],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredPutObjectRequestBucketPutObjectTypeDef = TypedDict(
     "_RequiredPutObjectRequestBucketPutObjectTypeDef",
     {
         "Key": str,
     },
 )
 _OptionalPutObjectRequestBucketPutObjectTypeDef = TypedDict(
@@ -3569,19 +3237,21 @@
         "ObjectLockRetainUntilDate": Union[datetime, str],
         "ObjectLockLegalHoldStatus": ObjectLockLegalHoldStatusType,
         "ExpectedBucketOwner": str,
     },
     total=False,
 )
 
+
 class PutObjectRequestBucketPutObjectTypeDef(
     _RequiredPutObjectRequestBucketPutObjectTypeDef, _OptionalPutObjectRequestBucketPutObjectTypeDef
 ):
     pass
 
+
 PutObjectRequestObjectPutTypeDef = TypedDict(
     "PutObjectRequestObjectPutTypeDef",
     {
         "ACL": ObjectCannedACLType,
         "Body": Union[str, bytes, IO[Any], StreamingBody],
         "CacheControl": str,
         "ContentDisposition": str,
@@ -3707,62 +3377,37 @@
         "ObjectLockRetainUntilDate": Union[datetime, str],
         "ObjectLockLegalHoldStatus": ObjectLockLegalHoldStatusType,
         "ExpectedBucketOwner": str,
     },
     total=False,
 )
 
+
 class PutObjectRequestRequestTypeDef(
     _RequiredPutObjectRequestRequestTypeDef, _OptionalPutObjectRequestRequestTypeDef
 ):
     pass
 
-PutObjectRetentionOutputTypeDef = TypedDict(
-    "PutObjectRetentionOutputTypeDef",
-    {
-        "RequestCharged": Literal["requester"],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-PutObjectTaggingOutputTypeDef = TypedDict(
-    "PutObjectTaggingOutputTypeDef",
-    {
-        "VersionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 RecordsEventTypeDef = TypedDict(
     "RecordsEventTypeDef",
     {
         "Payload": bytes,
     },
-    total=False,
-)
-
-RedirectAllRequestsToResponseMetadataTypeDef = TypedDict(
-    "RedirectAllRequestsToResponseMetadataTypeDef",
-    {
-        "HostName": str,
-        "Protocol": ProtocolType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
 )
 
 RedirectTypeDef = TypedDict(
     "RedirectTypeDef",
     {
         "HostName": str,
         "HttpRedirectCode": str,
         "Protocol": ProtocolType,
         "ReplaceKeyPrefixWith": str,
         "ReplaceKeyWith": str,
     },
-    total=False,
 )
 
 ReplicaModificationsTypeDef = TypedDict(
     "ReplicaModificationsTypeDef",
     {
         "Status": ReplicaModificationsStatusType,
     },
@@ -3772,104 +3417,45 @@
     "RequestProgressTypeDef",
     {
         "Enabled": bool,
     },
     total=False,
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
-RestoreObjectOutputTypeDef = TypedDict(
-    "RestoreObjectOutputTypeDef",
-    {
-        "RequestCharged": Literal["requester"],
-        "RestoreOutputPath": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-RestoreStatusResponseMetadataTypeDef = TypedDict(
-    "RestoreStatusResponseMetadataTypeDef",
-    {
-        "IsRestoreInProgress": bool,
-        "RestoreExpiryDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ScanRangeTypeDef = TypedDict(
     "ScanRangeTypeDef",
     {
         "Start": int,
         "End": int,
     },
     total=False,
 )
 
-_RequiredServerSideEncryptionByDefaultTypeDef = TypedDict(
-    "_RequiredServerSideEncryptionByDefaultTypeDef",
+ServerSideEncryptionByDefaultTypeDef = TypedDict(
+    "ServerSideEncryptionByDefaultTypeDef",
     {
         "SSEAlgorithm": ServerSideEncryptionType,
-    },
-)
-_OptionalServerSideEncryptionByDefaultTypeDef = TypedDict(
-    "_OptionalServerSideEncryptionByDefaultTypeDef",
-    {
         "KMSMasterKeyID": str,
     },
-    total=False,
 )
 
-class ServerSideEncryptionByDefaultTypeDef(
-    _RequiredServerSideEncryptionByDefaultTypeDef, _OptionalServerSideEncryptionByDefaultTypeDef
-):
-    pass
-
 SseKmsEncryptedObjectsTypeDef = TypedDict(
     "SseKmsEncryptedObjectsTypeDef",
     {
         "Status": SseKmsEncryptedObjectsStatusType,
     },
 )
 
 StatsTypeDef = TypedDict(
     "StatsTypeDef",
     {
         "BytesScanned": int,
         "BytesProcessed": int,
         "BytesReturned": int,
     },
-    total=False,
-)
-
-UploadPartOutputTypeDef = TypedDict(
-    "UploadPartOutputTypeDef",
-    {
-        "ServerSideEncryption": ServerSideEncryptionType,
-        "ETag": str,
-        "ChecksumCRC32": str,
-        "ChecksumCRC32C": str,
-        "ChecksumSHA1": str,
-        "ChecksumSHA256": str,
-        "SSECustomerAlgorithm": str,
-        "SSECustomerKeyMD5": str,
-        "SSEKMSKeyId": str,
-        "BucketKeyEnabled": bool,
-        "RequestCharged": Literal["requester"],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
 )
 
 UploadPartRequestMultipartUploadPartUploadTypeDef = TypedDict(
     "UploadPartRequestMultipartUploadPartUploadTypeDef",
     {
         "Body": Union[str, bytes, IO[Any], StreamingBody],
         "ContentLength": int,
@@ -3913,19 +3499,21 @@
         "SSECustomerKeyMD5": str,
         "RequestPayer": Literal["requester"],
         "ExpectedBucketOwner": str,
     },
     total=False,
 )
 
+
 class UploadPartRequestRequestTypeDef(
     _RequiredUploadPartRequestRequestTypeDef, _OptionalUploadPartRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredWriteGetObjectResponseRequestRequestTypeDef = TypedDict(
     "_RequiredWriteGetObjectResponseRequestRequestTypeDef",
     {
         "RequestRoute": str,
         "RequestToken": str,
     },
 )
@@ -3970,20 +3558,379 @@
         "TagCount": int,
         "VersionId": str,
         "BucketKeyEnabled": bool,
     },
     total=False,
 )
 
+
 class WriteGetObjectResponseRequestRequestTypeDef(
     _RequiredWriteGetObjectResponseRequestRequestTypeDef,
     _OptionalWriteGetObjectResponseRequestRequestTypeDef,
 ):
     pass
 
+
+AbortMultipartUploadOutputTypeDef = TypedDict(
+    "AbortMultipartUploadOutputTypeDef",
+    {
+        "RequestCharged": Literal["requester"],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CompleteMultipartUploadOutputTypeDef = TypedDict(
+    "CompleteMultipartUploadOutputTypeDef",
+    {
+        "Location": str,
+        "Bucket": str,
+        "Key": str,
+        "Expiration": str,
+        "ETag": str,
+        "ChecksumCRC32": str,
+        "ChecksumCRC32C": str,
+        "ChecksumSHA1": str,
+        "ChecksumSHA256": str,
+        "ServerSideEncryption": ServerSideEncryptionType,
+        "VersionId": str,
+        "SSEKMSKeyId": str,
+        "BucketKeyEnabled": bool,
+        "RequestCharged": Literal["requester"],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateBucketOutputTypeDef = TypedDict(
+    "CreateBucketOutputTypeDef",
+    {
+        "Location": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateMultipartUploadOutputTypeDef = TypedDict(
+    "CreateMultipartUploadOutputTypeDef",
+    {
+        "AbortDate": datetime,
+        "AbortRuleId": str,
+        "Bucket": str,
+        "Key": str,
+        "UploadId": str,
+        "ServerSideEncryption": ServerSideEncryptionType,
+        "SSECustomerAlgorithm": str,
+        "SSECustomerKeyMD5": str,
+        "SSEKMSKeyId": str,
+        "SSEKMSEncryptionContext": str,
+        "BucketKeyEnabled": bool,
+        "RequestCharged": Literal["requester"],
+        "ChecksumAlgorithm": ChecksumAlgorithmType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteObjectOutputTypeDef = TypedDict(
+    "DeleteObjectOutputTypeDef",
+    {
+        "DeleteMarker": bool,
+        "VersionId": str,
+        "RequestCharged": Literal["requester"],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteObjectTaggingOutputTypeDef = TypedDict(
+    "DeleteObjectTaggingOutputTypeDef",
+    {
+        "VersionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ErrorDocumentResponseMetadataTypeDef = TypedDict(
+    "ErrorDocumentResponseMetadataTypeDef",
+    {
+        "Key": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetBucketAccelerateConfigurationOutputTypeDef = TypedDict(
+    "GetBucketAccelerateConfigurationOutputTypeDef",
+    {
+        "Status": BucketAccelerateStatusType,
+        "RequestCharged": Literal["requester"],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetBucketLocationOutputTypeDef = TypedDict(
+    "GetBucketLocationOutputTypeDef",
+    {
+        "LocationConstraint": BucketLocationConstraintType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetBucketPolicyOutputTypeDef = TypedDict(
+    "GetBucketPolicyOutputTypeDef",
+    {
+        "Policy": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetBucketRequestPaymentOutputTypeDef = TypedDict(
+    "GetBucketRequestPaymentOutputTypeDef",
+    {
+        "Payer": PayerType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetBucketVersioningOutputTypeDef = TypedDict(
+    "GetBucketVersioningOutputTypeDef",
+    {
+        "Status": BucketVersioningStatusType,
+        "MFADelete": MFADeleteStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetObjectOutputTypeDef = TypedDict(
+    "GetObjectOutputTypeDef",
+    {
+        "Body": StreamingBody,
+        "DeleteMarker": bool,
+        "AcceptRanges": str,
+        "Expiration": str,
+        "Restore": str,
+        "LastModified": datetime,
+        "ContentLength": int,
+        "ETag": str,
+        "ChecksumCRC32": str,
+        "ChecksumCRC32C": str,
+        "ChecksumSHA1": str,
+        "ChecksumSHA256": str,
+        "MissingMeta": int,
+        "VersionId": str,
+        "CacheControl": str,
+        "ContentDisposition": str,
+        "ContentEncoding": str,
+        "ContentLanguage": str,
+        "ContentRange": str,
+        "ContentType": str,
+        "Expires": datetime,
+        "WebsiteRedirectLocation": str,
+        "ServerSideEncryption": ServerSideEncryptionType,
+        "Metadata": Dict[str, str],
+        "SSECustomerAlgorithm": str,
+        "SSECustomerKeyMD5": str,
+        "SSEKMSKeyId": str,
+        "BucketKeyEnabled": bool,
+        "StorageClass": StorageClassType,
+        "RequestCharged": Literal["requester"],
+        "ReplicationStatus": ReplicationStatusType,
+        "PartsCount": int,
+        "TagCount": int,
+        "ObjectLockMode": ObjectLockModeType,
+        "ObjectLockRetainUntilDate": datetime,
+        "ObjectLockLegalHoldStatus": ObjectLockLegalHoldStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetObjectTorrentOutputTypeDef = TypedDict(
+    "GetObjectTorrentOutputTypeDef",
+    {
+        "Body": StreamingBody,
+        "RequestCharged": Literal["requester"],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+HeadObjectOutputTypeDef = TypedDict(
+    "HeadObjectOutputTypeDef",
+    {
+        "DeleteMarker": bool,
+        "AcceptRanges": str,
+        "Expiration": str,
+        "Restore": str,
+        "ArchiveStatus": ArchiveStatusType,
+        "LastModified": datetime,
+        "ContentLength": int,
+        "ChecksumCRC32": str,
+        "ChecksumCRC32C": str,
+        "ChecksumSHA1": str,
+        "ChecksumSHA256": str,
+        "ETag": str,
+        "MissingMeta": int,
+        "VersionId": str,
+        "CacheControl": str,
+        "ContentDisposition": str,
+        "ContentEncoding": str,
+        "ContentLanguage": str,
+        "ContentType": str,
+        "Expires": datetime,
+        "WebsiteRedirectLocation": str,
+        "ServerSideEncryption": ServerSideEncryptionType,
+        "Metadata": Dict[str, str],
+        "SSECustomerAlgorithm": str,
+        "SSECustomerKeyMD5": str,
+        "SSEKMSKeyId": str,
+        "BucketKeyEnabled": bool,
+        "StorageClass": StorageClassType,
+        "RequestCharged": Literal["requester"],
+        "ReplicationStatus": ReplicationStatusType,
+        "PartsCount": int,
+        "ObjectLockMode": ObjectLockModeType,
+        "ObjectLockRetainUntilDate": datetime,
+        "ObjectLockLegalHoldStatus": ObjectLockLegalHoldStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+IndexDocumentResponseMetadataTypeDef = TypedDict(
+    "IndexDocumentResponseMetadataTypeDef",
+    {
+        "Suffix": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+InitiatorResponseMetadataTypeDef = TypedDict(
+    "InitiatorResponseMetadataTypeDef",
+    {
+        "ID": str,
+        "DisplayName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+OwnerResponseMetadataTypeDef = TypedDict(
+    "OwnerResponseMetadataTypeDef",
+    {
+        "DisplayName": str,
+        "ID": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutObjectAclOutputTypeDef = TypedDict(
+    "PutObjectAclOutputTypeDef",
+    {
+        "RequestCharged": Literal["requester"],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutObjectLegalHoldOutputTypeDef = TypedDict(
+    "PutObjectLegalHoldOutputTypeDef",
+    {
+        "RequestCharged": Literal["requester"],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutObjectLockConfigurationOutputTypeDef = TypedDict(
+    "PutObjectLockConfigurationOutputTypeDef",
+    {
+        "RequestCharged": Literal["requester"],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutObjectOutputTypeDef = TypedDict(
+    "PutObjectOutputTypeDef",
+    {
+        "Expiration": str,
+        "ETag": str,
+        "ChecksumCRC32": str,
+        "ChecksumCRC32C": str,
+        "ChecksumSHA1": str,
+        "ChecksumSHA256": str,
+        "ServerSideEncryption": ServerSideEncryptionType,
+        "VersionId": str,
+        "SSECustomerAlgorithm": str,
+        "SSECustomerKeyMD5": str,
+        "SSEKMSKeyId": str,
+        "SSEKMSEncryptionContext": str,
+        "BucketKeyEnabled": bool,
+        "RequestCharged": Literal["requester"],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutObjectRetentionOutputTypeDef = TypedDict(
+    "PutObjectRetentionOutputTypeDef",
+    {
+        "RequestCharged": Literal["requester"],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutObjectTaggingOutputTypeDef = TypedDict(
+    "PutObjectTaggingOutputTypeDef",
+    {
+        "VersionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RedirectAllRequestsToResponseMetadataTypeDef = TypedDict(
+    "RedirectAllRequestsToResponseMetadataTypeDef",
+    {
+        "HostName": str,
+        "Protocol": ProtocolType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RestoreObjectOutputTypeDef = TypedDict(
+    "RestoreObjectOutputTypeDef",
+    {
+        "RequestCharged": Literal["requester"],
+        "RestoreOutputPath": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RestoreStatusResponseMetadataTypeDef = TypedDict(
+    "RestoreStatusResponseMetadataTypeDef",
+    {
+        "IsRestoreInProgress": bool,
+        "RestoreExpiryDate": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UploadPartOutputTypeDef = TypedDict(
+    "UploadPartOutputTypeDef",
+    {
+        "ServerSideEncryption": ServerSideEncryptionType,
+        "ETag": str,
+        "ChecksumCRC32": str,
+        "ChecksumCRC32C": str,
+        "ChecksumSHA1": str,
+        "ChecksumSHA256": str,
+        "SSECustomerAlgorithm": str,
+        "SSECustomerKeyMD5": str,
+        "SSEKMSKeyId": str,
+        "BucketKeyEnabled": bool,
+        "RequestCharged": Literal["requester"],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredPutBucketAccelerateConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredPutBucketAccelerateConfigurationRequestRequestTypeDef",
     {
         "Bucket": str,
         "AccelerateConfiguration": AccelerateConfigurationTypeDef,
     },
 )
@@ -3992,95 +3939,91 @@
     {
         "ExpectedBucketOwner": str,
         "ChecksumAlgorithm": ChecksumAlgorithmType,
     },
     total=False,
 )
 
+
 class PutBucketAccelerateConfigurationRequestRequestTypeDef(
     _RequiredPutBucketAccelerateConfigurationRequestRequestTypeDef,
     _OptionalPutBucketAccelerateConfigurationRequestRequestTypeDef,
 ):
     pass
 
+
 DeleteMarkerEntryTypeDef = TypedDict(
     "DeleteMarkerEntryTypeDef",
     {
         "Owner": OwnerTypeDef,
         "Key": str,
         "VersionId": str,
         "IsLatest": bool,
         "LastModified": datetime,
     },
-    total=False,
 )
 
 AnalyticsAndOperatorTypeDef = TypedDict(
     "AnalyticsAndOperatorTypeDef",
     {
         "Prefix": str,
         "Tags": List[TagTypeDef],
     },
-    total=False,
 )
 
 GetBucketTaggingOutputTypeDef = TypedDict(
     "GetBucketTaggingOutputTypeDef",
     {
         "TagSet": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetObjectTaggingOutputTypeDef = TypedDict(
     "GetObjectTaggingOutputTypeDef",
     {
         "VersionId": str,
         "TagSet": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 IntelligentTieringAndOperatorTypeDef = TypedDict(
     "IntelligentTieringAndOperatorTypeDef",
     {
         "Prefix": str,
         "Tags": List[TagTypeDef],
     },
-    total=False,
 )
 
 LifecycleRuleAndOperatorTypeDef = TypedDict(
     "LifecycleRuleAndOperatorTypeDef",
     {
         "Prefix": str,
         "Tags": List[TagTypeDef],
         "ObjectSizeGreaterThan": int,
         "ObjectSizeLessThan": int,
     },
-    total=False,
 )
 
 MetricsAndOperatorTypeDef = TypedDict(
     "MetricsAndOperatorTypeDef",
     {
         "Prefix": str,
         "Tags": List[TagTypeDef],
         "AccessPointArn": str,
     },
-    total=False,
 )
 
 ReplicationRuleAndOperatorTypeDef = TypedDict(
     "ReplicationRuleAndOperatorTypeDef",
     {
         "Prefix": str,
         "Tags": List[TagTypeDef],
     },
-    total=False,
 )
 
 TaggingTypeDef = TypedDict(
     "TaggingTypeDef",
     {
         "TagSet": Sequence[TagTypeDef],
     },
@@ -4107,19 +4050,21 @@
         "Callback": Callable[..., Any],
         "SourceClient": BaseClient,
         "Config": TransferConfig,
     },
     total=False,
 )
 
+
 class BucketCopyRequestTypeDef(
     _RequiredBucketCopyRequestTypeDef, _OptionalBucketCopyRequestTypeDef
 ):
     pass
 
+
 _RequiredClientCopyRequestTypeDef = TypedDict(
     "_RequiredClientCopyRequestTypeDef",
     {
         "CopySource": CopySourceTypeDef,
         "Bucket": str,
         "Key": str,
     },
@@ -4131,19 +4076,21 @@
         "Callback": Callable[..., Any],
         "SourceClient": BaseClient,
         "Config": TransferConfig,
     },
     total=False,
 )
 
+
 class ClientCopyRequestTypeDef(
     _RequiredClientCopyRequestTypeDef, _OptionalClientCopyRequestTypeDef
 ):
     pass
 
+
 _RequiredCopyObjectRequestRequestTypeDef = TypedDict(
     "_RequiredCopyObjectRequestRequestTypeDef",
     {
         "Bucket": str,
         "CopySource": Union[str, CopySourceTypeDef],
         "Key": str,
     },
@@ -4189,19 +4136,21 @@
         "ObjectLockLegalHoldStatus": ObjectLockLegalHoldStatusType,
         "ExpectedBucketOwner": str,
         "ExpectedSourceBucketOwner": str,
     },
     total=False,
 )
 
+
 class CopyObjectRequestRequestTypeDef(
     _RequiredCopyObjectRequestRequestTypeDef, _OptionalCopyObjectRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredObjectCopyRequestTypeDef = TypedDict(
     "_RequiredObjectCopyRequestTypeDef",
     {
         "CopySource": CopySourceTypeDef,
     },
 )
 _OptionalObjectCopyRequestTypeDef = TypedDict(
@@ -4211,19 +4160,21 @@
         "Callback": Callable[..., Any],
         "SourceClient": BaseClient,
         "Config": TransferConfig,
     },
     total=False,
 )
 
+
 class ObjectCopyRequestTypeDef(
     _RequiredObjectCopyRequestTypeDef, _OptionalObjectCopyRequestTypeDef
 ):
     pass
 
+
 _RequiredUploadPartCopyRequestMultipartUploadPartCopyFromTypeDef = TypedDict(
     "_RequiredUploadPartCopyRequestMultipartUploadPartCopyFromTypeDef",
     {
         "CopySource": Union[str, CopySourceTypeDef],
     },
 )
 _OptionalUploadPartCopyRequestMultipartUploadPartCopyFromTypeDef = TypedDict(
@@ -4243,20 +4194,22 @@
         "RequestPayer": Literal["requester"],
         "ExpectedBucketOwner": str,
         "ExpectedSourceBucketOwner": str,
     },
     total=False,
 )
 
+
 class UploadPartCopyRequestMultipartUploadPartCopyFromTypeDef(
     _RequiredUploadPartCopyRequestMultipartUploadPartCopyFromTypeDef,
     _OptionalUploadPartCopyRequestMultipartUploadPartCopyFromTypeDef,
 ):
     pass
 
+
 _RequiredUploadPartCopyRequestRequestTypeDef = TypedDict(
     "_RequiredUploadPartCopyRequestRequestTypeDef",
     {
         "Bucket": str,
         "CopySource": Union[str, CopySourceTypeDef],
         "Key": str,
         "PartNumber": int,
@@ -4280,40 +4233,42 @@
         "RequestPayer": Literal["requester"],
         "ExpectedBucketOwner": str,
         "ExpectedSourceBucketOwner": str,
     },
     total=False,
 )
 
+
 class UploadPartCopyRequestRequestTypeDef(
     _RequiredUploadPartCopyRequestRequestTypeDef, _OptionalUploadPartCopyRequestRequestTypeDef
 ):
     pass
 
+
 ListBucketsOutputTypeDef = TypedDict(
     "ListBucketsOutputTypeDef",
     {
         "Buckets": List[BucketTypeDef],
         "Owner": OwnerTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CORSConfigurationTypeDef = TypedDict(
     "CORSConfigurationTypeDef",
     {
         "CORSRules": Sequence[CORSRuleTypeDef],
     },
 )
 
 GetBucketCorsOutputTypeDef = TypedDict(
     "GetBucketCorsOutputTypeDef",
     {
         "CORSRules": List[CORSRuleTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CompletedMultipartUploadTypeDef = TypedDict(
     "CompletedMultipartUploadTypeDef",
     {
         "Parts": Sequence[CompletedPartTypeDef],
@@ -4331,30 +4286,30 @@
         "ServerSideEncryption": ServerSideEncryptionType,
         "SSECustomerAlgorithm": str,
         "SSECustomerKeyMD5": str,
         "SSEKMSKeyId": str,
         "SSEKMSEncryptionContext": str,
         "BucketKeyEnabled": bool,
         "RequestCharged": Literal["requester"],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UploadPartCopyOutputTypeDef = TypedDict(
     "UploadPartCopyOutputTypeDef",
     {
         "CopySourceVersionId": str,
         "CopyPartResult": CopyPartResultTypeDef,
         "ServerSideEncryption": ServerSideEncryptionType,
         "SSECustomerAlgorithm": str,
         "SSECustomerKeyMD5": str,
         "SSEKMSKeyId": str,
         "BucketKeyEnabled": bool,
         "RequestCharged": Literal["requester"],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateBucketRequestBucketCreateTypeDef = TypedDict(
     "CreateBucketRequestBucketCreateTypeDef",
     {
         "ACL": BucketCannedACLType,
@@ -4388,19 +4343,21 @@
         "GrantWriteACP": str,
         "ObjectLockEnabledForBucket": bool,
         "ObjectOwnership": ObjectOwnershipType,
     },
     total=False,
 )
 
+
 class CreateBucketRequestRequestTypeDef(
     _RequiredCreateBucketRequestRequestTypeDef, _OptionalCreateBucketRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredCreateBucketRequestServiceResourceCreateBucketTypeDef = TypedDict(
     "_RequiredCreateBucketRequestServiceResourceCreateBucketTypeDef",
     {
         "Bucket": str,
     },
 )
 _OptionalCreateBucketRequestServiceResourceCreateBucketTypeDef = TypedDict(
@@ -4415,35 +4372,36 @@
         "GrantWriteACP": str,
         "ObjectLockEnabledForBucket": bool,
         "ObjectOwnership": ObjectOwnershipType,
     },
     total=False,
 )
 
+
 class CreateBucketRequestServiceResourceCreateBucketTypeDef(
     _RequiredCreateBucketRequestServiceResourceCreateBucketTypeDef,
     _OptionalCreateBucketRequestServiceResourceCreateBucketTypeDef,
 ):
     pass
 
+
 ObjectLockRuleTypeDef = TypedDict(
     "ObjectLockRuleTypeDef",
     {
         "DefaultRetention": DefaultRetentionTypeDef,
     },
-    total=False,
 )
 
 DeleteObjectsOutputTypeDef = TypedDict(
     "DeleteObjectsOutputTypeDef",
     {
         "Deleted": List[DeletedObjectTypeDef],
         "RequestCharged": Literal["requester"],
         "Errors": List[ErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredDeleteTypeDef = TypedDict(
     "_RequiredDeleteTypeDef",
     {
         "Objects": Sequence[ObjectIdentifierTypeDef],
@@ -4453,51 +4411,51 @@
     "_OptionalDeleteTypeDef",
     {
         "Quiet": bool,
     },
     total=False,
 )
 
+
 class DeleteTypeDef(_RequiredDeleteTypeDef, _OptionalDeleteTypeDef):
     pass
 
+
 S3KeyFilterTypeDef = TypedDict(
     "S3KeyFilterTypeDef",
     {
         "FilterRules": List[FilterRuleTypeDef],
     },
-    total=False,
 )
 
 GetBucketPolicyStatusOutputTypeDef = TypedDict(
     "GetBucketPolicyStatusOutputTypeDef",
     {
         "PolicyStatus": PolicyStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetObjectAttributesPartsTypeDef = TypedDict(
     "GetObjectAttributesPartsTypeDef",
     {
         "TotalPartsCount": int,
         "PartNumberMarker": int,
         "NextPartNumberMarker": int,
         "MaxParts": int,
         "IsTruncated": bool,
         "Parts": List[ObjectPartTypeDef],
     },
-    total=False,
 )
 
 GetObjectLegalHoldOutputTypeDef = TypedDict(
     "GetObjectLegalHoldOutputTypeDef",
     {
         "LegalHold": ObjectLockLegalHoldTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredPutObjectLegalHoldRequestRequestTypeDef = TypedDict(
     "_RequiredPutObjectLegalHoldRequestRequestTypeDef",
     {
         "Bucket": str,
@@ -4513,25 +4471,27 @@
         "ContentMD5": str,
         "ChecksumAlgorithm": ChecksumAlgorithmType,
         "ExpectedBucketOwner": str,
     },
     total=False,
 )
 
+
 class PutObjectLegalHoldRequestRequestTypeDef(
     _RequiredPutObjectLegalHoldRequestRequestTypeDef,
     _OptionalPutObjectLegalHoldRequestRequestTypeDef,
 ):
     pass
 
+
 GetObjectRetentionOutputTypeDef = TypedDict(
     "GetObjectRetentionOutputTypeDef",
     {
         "Retention": ObjectLockRetentionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredPutObjectRetentionRequestRequestTypeDef = TypedDict(
     "_RequiredPutObjectRetentionRequestRequestTypeDef",
     {
         "Bucket": str,
@@ -4548,25 +4508,27 @@
         "ContentMD5": str,
         "ChecksumAlgorithm": ChecksumAlgorithmType,
         "ExpectedBucketOwner": str,
     },
     total=False,
 )
 
+
 class PutObjectRetentionRequestRequestTypeDef(
     _RequiredPutObjectRetentionRequestRequestTypeDef,
     _OptionalPutObjectRetentionRequestRequestTypeDef,
 ):
     pass
 
+
 GetPublicAccessBlockOutputTypeDef = TypedDict(
     "GetPublicAccessBlockOutputTypeDef",
     {
         "PublicAccessBlockConfiguration": PublicAccessBlockConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredPutPublicAccessBlockRequestRequestTypeDef = TypedDict(
     "_RequiredPutPublicAccessBlockRequestRequestTypeDef",
     {
         "Bucket": str,
@@ -4579,36 +4541,36 @@
         "ContentMD5": str,
         "ChecksumAlgorithm": ChecksumAlgorithmType,
         "ExpectedBucketOwner": str,
     },
     total=False,
 )
 
+
 class PutPublicAccessBlockRequestRequestTypeDef(
     _RequiredPutPublicAccessBlockRequestRequestTypeDef,
     _OptionalPutPublicAccessBlockRequestRequestTypeDef,
 ):
     pass
 
+
 GrantTypeDef = TypedDict(
     "GrantTypeDef",
     {
         "Grantee": GranteeTypeDef,
         "Permission": PermissionType,
     },
-    total=False,
 )
 
 TargetGrantTypeDef = TypedDict(
     "TargetGrantTypeDef",
     {
         "Grantee": GranteeTypeDef,
         "Permission": BucketLogsPermissionType,
     },
-    total=False,
 )
 
 _RequiredHeadBucketRequestBucketExistsWaitTypeDef = TypedDict(
     "_RequiredHeadBucketRequestBucketExistsWaitTypeDef",
     {
         "Bucket": str,
     },
@@ -4618,20 +4580,22 @@
     {
         "ExpectedBucketOwner": str,
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
+
 class HeadBucketRequestBucketExistsWaitTypeDef(
     _RequiredHeadBucketRequestBucketExistsWaitTypeDef,
     _OptionalHeadBucketRequestBucketExistsWaitTypeDef,
 ):
     pass
 
+
 _RequiredHeadBucketRequestBucketNotExistsWaitTypeDef = TypedDict(
     "_RequiredHeadBucketRequestBucketNotExistsWaitTypeDef",
     {
         "Bucket": str,
     },
 )
 _OptionalHeadBucketRequestBucketNotExistsWaitTypeDef = TypedDict(
@@ -4639,20 +4603,22 @@
     {
         "ExpectedBucketOwner": str,
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
+
 class HeadBucketRequestBucketNotExistsWaitTypeDef(
     _RequiredHeadBucketRequestBucketNotExistsWaitTypeDef,
     _OptionalHeadBucketRequestBucketNotExistsWaitTypeDef,
 ):
     pass
 
+
 _RequiredHeadObjectRequestObjectExistsWaitTypeDef = TypedDict(
     "_RequiredHeadObjectRequestObjectExistsWaitTypeDef",
     {
         "Bucket": str,
         "Key": str,
     },
 )
@@ -4673,20 +4639,22 @@
         "ExpectedBucketOwner": str,
         "ChecksumMode": Literal["ENABLED"],
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
+
 class HeadObjectRequestObjectExistsWaitTypeDef(
     _RequiredHeadObjectRequestObjectExistsWaitTypeDef,
     _OptionalHeadObjectRequestObjectExistsWaitTypeDef,
 ):
     pass
 
+
 _RequiredHeadObjectRequestObjectNotExistsWaitTypeDef = TypedDict(
     "_RequiredHeadObjectRequestObjectNotExistsWaitTypeDef",
     {
         "Bucket": str,
         "Key": str,
     },
 )
@@ -4707,32 +4675,33 @@
         "ExpectedBucketOwner": str,
         "ChecksumMode": Literal["ENABLED"],
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
+
 class HeadObjectRequestObjectNotExistsWaitTypeDef(
     _RequiredHeadObjectRequestObjectNotExistsWaitTypeDef,
     _OptionalHeadObjectRequestObjectNotExistsWaitTypeDef,
 ):
     pass
 
+
 MultipartUploadTypeDef = TypedDict(
     "MultipartUploadTypeDef",
     {
         "UploadId": str,
         "Key": str,
         "Initiated": datetime,
         "StorageClass": StorageClassType,
         "Owner": OwnerTypeDef,
         "Initiator": InitiatorTypeDef,
         "ChecksumAlgorithm": ChecksumAlgorithmType,
     },
-    total=False,
 )
 
 InputSerializationTypeDef = TypedDict(
     "InputSerializationTypeDef",
     {
         "CSV": CSVInputTypeDef,
         "CompressionType": CompressionTypeType,
@@ -4744,49 +4713,181 @@
 
 InventoryEncryptionTypeDef = TypedDict(
     "InventoryEncryptionTypeDef",
     {
         "SSES3": Dict[str, Any],
         "SSEKMS": SSEKMSTypeDef,
     },
-    total=False,
 )
 
 OutputSerializationTypeDef = TypedDict(
     "OutputSerializationTypeDef",
     {
         "CSV": CSVOutputTypeDef,
         "JSON": JSONOutputTypeDef,
     },
     total=False,
 )
 
-_RequiredRuleTypeDef = TypedDict(
-    "_RequiredRuleTypeDef",
-    {
-        "Prefix": str,
-        "Status": ExpirationStatusType,
-    },
-)
-_OptionalRuleTypeDef = TypedDict(
-    "_OptionalRuleTypeDef",
+RuleTypeDef = TypedDict(
+    "RuleTypeDef",
     {
         "Expiration": LifecycleExpirationTypeDef,
         "ID": str,
+        "Prefix": str,
+        "Status": ExpirationStatusType,
         "Transition": TransitionTypeDef,
         "NoncurrentVersionTransition": NoncurrentVersionTransitionTypeDef,
         "NoncurrentVersionExpiration": NoncurrentVersionExpirationTypeDef,
         "AbortIncompleteMultipartUpload": AbortIncompleteMultipartUploadTypeDef,
     },
+)
+
+_RequiredListMultipartUploadsRequestListMultipartUploadsPaginateTypeDef = TypedDict(
+    "_RequiredListMultipartUploadsRequestListMultipartUploadsPaginateTypeDef",
+    {
+        "Bucket": str,
+    },
+)
+_OptionalListMultipartUploadsRequestListMultipartUploadsPaginateTypeDef = TypedDict(
+    "_OptionalListMultipartUploadsRequestListMultipartUploadsPaginateTypeDef",
+    {
+        "Delimiter": str,
+        "EncodingType": Literal["url"],
+        "Prefix": str,
+        "ExpectedBucketOwner": str,
+        "RequestPayer": Literal["requester"],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListMultipartUploadsRequestListMultipartUploadsPaginateTypeDef(
+    _RequiredListMultipartUploadsRequestListMultipartUploadsPaginateTypeDef,
+    _OptionalListMultipartUploadsRequestListMultipartUploadsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListObjectVersionsRequestListObjectVersionsPaginateTypeDef = TypedDict(
+    "_RequiredListObjectVersionsRequestListObjectVersionsPaginateTypeDef",
+    {
+        "Bucket": str,
+    },
+)
+_OptionalListObjectVersionsRequestListObjectVersionsPaginateTypeDef = TypedDict(
+    "_OptionalListObjectVersionsRequestListObjectVersionsPaginateTypeDef",
+    {
+        "Delimiter": str,
+        "EncodingType": Literal["url"],
+        "Prefix": str,
+        "ExpectedBucketOwner": str,
+        "RequestPayer": Literal["requester"],
+        "OptionalObjectAttributes": Sequence[Literal["RestoreStatus"]],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
     total=False,
 )
 
-class RuleTypeDef(_RequiredRuleTypeDef, _OptionalRuleTypeDef):
+
+class ListObjectVersionsRequestListObjectVersionsPaginateTypeDef(
+    _RequiredListObjectVersionsRequestListObjectVersionsPaginateTypeDef,
+    _OptionalListObjectVersionsRequestListObjectVersionsPaginateTypeDef,
+):
     pass
 
+
+_RequiredListObjectsRequestListObjectsPaginateTypeDef = TypedDict(
+    "_RequiredListObjectsRequestListObjectsPaginateTypeDef",
+    {
+        "Bucket": str,
+    },
+)
+_OptionalListObjectsRequestListObjectsPaginateTypeDef = TypedDict(
+    "_OptionalListObjectsRequestListObjectsPaginateTypeDef",
+    {
+        "Delimiter": str,
+        "EncodingType": Literal["url"],
+        "Prefix": str,
+        "RequestPayer": Literal["requester"],
+        "ExpectedBucketOwner": str,
+        "OptionalObjectAttributes": Sequence[Literal["RestoreStatus"]],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListObjectsRequestListObjectsPaginateTypeDef(
+    _RequiredListObjectsRequestListObjectsPaginateTypeDef,
+    _OptionalListObjectsRequestListObjectsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListObjectsV2RequestListObjectsV2PaginateTypeDef = TypedDict(
+    "_RequiredListObjectsV2RequestListObjectsV2PaginateTypeDef",
+    {
+        "Bucket": str,
+    },
+)
+_OptionalListObjectsV2RequestListObjectsV2PaginateTypeDef = TypedDict(
+    "_OptionalListObjectsV2RequestListObjectsV2PaginateTypeDef",
+    {
+        "Delimiter": str,
+        "EncodingType": Literal["url"],
+        "Prefix": str,
+        "FetchOwner": bool,
+        "StartAfter": str,
+        "RequestPayer": Literal["requester"],
+        "ExpectedBucketOwner": str,
+        "OptionalObjectAttributes": Sequence[Literal["RestoreStatus"]],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListObjectsV2RequestListObjectsV2PaginateTypeDef(
+    _RequiredListObjectsV2RequestListObjectsV2PaginateTypeDef,
+    _OptionalListObjectsV2RequestListObjectsV2PaginateTypeDef,
+):
+    pass
+
+
+_RequiredListPartsRequestListPartsPaginateTypeDef = TypedDict(
+    "_RequiredListPartsRequestListPartsPaginateTypeDef",
+    {
+        "Bucket": str,
+        "Key": str,
+        "UploadId": str,
+    },
+)
+_OptionalListPartsRequestListPartsPaginateTypeDef = TypedDict(
+    "_OptionalListPartsRequestListPartsPaginateTypeDef",
+    {
+        "RequestPayer": Literal["requester"],
+        "ExpectedBucketOwner": str,
+        "SSECustomerAlgorithm": str,
+        "SSECustomerKey": str,
+        "SSECustomerKeyMD5": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListPartsRequestListPartsPaginateTypeDef(
+    _RequiredListPartsRequestListPartsPaginateTypeDef,
+    _OptionalListPartsRequestListPartsPaginateTypeDef,
+):
+    pass
+
+
 ListPartsOutputTypeDef = TypedDict(
     "ListPartsOutputTypeDef",
     {
         "AbortDate": datetime,
         "AbortRuleId": str,
         "Bucket": str,
         "Key": str,
@@ -4797,50 +4898,41 @@
         "IsTruncated": bool,
         "Parts": List[PartTypeDef],
         "Initiator": InitiatorTypeDef,
         "Owner": OwnerTypeDef,
         "StorageClass": StorageClassType,
         "RequestCharged": Literal["requester"],
         "ChecksumAlgorithm": ChecksumAlgorithmType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredMetricsTypeDef = TypedDict(
-    "_RequiredMetricsTypeDef",
+MetricsTypeDef = TypedDict(
+    "MetricsTypeDef",
     {
         "Status": MetricsStatusType,
-    },
-)
-_OptionalMetricsTypeDef = TypedDict(
-    "_OptionalMetricsTypeDef",
-    {
         "EventThreshold": ReplicationTimeValueTypeDef,
     },
-    total=False,
 )
 
-class MetricsTypeDef(_RequiredMetricsTypeDef, _OptionalMetricsTypeDef):
-    pass
-
 ReplicationTimeTypeDef = TypedDict(
     "ReplicationTimeTypeDef",
     {
         "Status": ReplicationTimeStatusType,
         "Time": ReplicationTimeValueTypeDef,
     },
 )
 
 NotificationConfigurationDeprecatedResponseMetadataTypeDef = TypedDict(
     "NotificationConfigurationDeprecatedResponseMetadataTypeDef",
     {
         "TopicConfiguration": TopicConfigurationDeprecatedTypeDef,
         "QueueConfiguration": QueueConfigurationDeprecatedTypeDef,
         "CloudFunctionConfiguration": CloudFunctionConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 NotificationConfigurationDeprecatedTypeDef = TypedDict(
     "NotificationConfigurationDeprecatedTypeDef",
     {
         "TopicConfiguration": TopicConfigurationDeprecatedTypeDef,
@@ -4858,15 +4950,14 @@
         "ETag": str,
         "ChecksumAlgorithm": List[ChecksumAlgorithmType],
         "Size": int,
         "StorageClass": ObjectStorageClassType,
         "Owner": OwnerTypeDef,
         "RestoreStatus": RestoreStatusTypeDef,
     },
-    total=False,
 )
 
 ObjectVersionTypeDef = TypedDict(
     "ObjectVersionTypeDef",
     {
         "ETag": str,
         "ChecksumAlgorithm": List[ChecksumAlgorithmType],
@@ -4875,30 +4966,28 @@
         "Key": str,
         "VersionId": str,
         "IsLatest": bool,
         "LastModified": datetime,
         "Owner": OwnerTypeDef,
         "RestoreStatus": RestoreStatusTypeDef,
     },
-    total=False,
 )
 
 OwnershipControlsTypeDef = TypedDict(
     "OwnershipControlsTypeDef",
     {
         "Rules": List[OwnershipControlsRuleTypeDef],
     },
 )
 
 ProgressEventTypeDef = TypedDict(
     "ProgressEventTypeDef",
     {
         "Details": ProgressTypeDef,
     },
-    total=False,
 )
 
 _RequiredPutBucketRequestPaymentRequestBucketRequestPaymentPutTypeDef = TypedDict(
     "_RequiredPutBucketRequestPaymentRequestBucketRequestPaymentPutTypeDef",
     {
         "RequestPaymentConfiguration": RequestPaymentConfigurationTypeDef,
     },
@@ -4908,20 +4997,22 @@
     {
         "ChecksumAlgorithm": ChecksumAlgorithmType,
         "ExpectedBucketOwner": str,
     },
     total=False,
 )
 
+
 class PutBucketRequestPaymentRequestBucketRequestPaymentPutTypeDef(
     _RequiredPutBucketRequestPaymentRequestBucketRequestPaymentPutTypeDef,
     _OptionalPutBucketRequestPaymentRequestBucketRequestPaymentPutTypeDef,
 ):
     pass
 
+
 _RequiredPutBucketRequestPaymentRequestRequestTypeDef = TypedDict(
     "_RequiredPutBucketRequestPaymentRequestRequestTypeDef",
     {
         "Bucket": str,
         "RequestPaymentConfiguration": RequestPaymentConfigurationTypeDef,
     },
 )
@@ -4930,20 +5021,22 @@
     {
         "ChecksumAlgorithm": ChecksumAlgorithmType,
         "ExpectedBucketOwner": str,
     },
     total=False,
 )
 
+
 class PutBucketRequestPaymentRequestRequestTypeDef(
     _RequiredPutBucketRequestPaymentRequestRequestTypeDef,
     _OptionalPutBucketRequestPaymentRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredPutBucketVersioningRequestBucketVersioningPutTypeDef = TypedDict(
     "_RequiredPutBucketVersioningRequestBucketVersioningPutTypeDef",
     {
         "VersioningConfiguration": VersioningConfigurationTypeDef,
     },
 )
 _OptionalPutBucketVersioningRequestBucketVersioningPutTypeDef = TypedDict(
@@ -4952,20 +5045,22 @@
         "ChecksumAlgorithm": ChecksumAlgorithmType,
         "MFA": str,
         "ExpectedBucketOwner": str,
     },
     total=False,
 )
 
+
 class PutBucketVersioningRequestBucketVersioningPutTypeDef(
     _RequiredPutBucketVersioningRequestBucketVersioningPutTypeDef,
     _OptionalPutBucketVersioningRequestBucketVersioningPutTypeDef,
 ):
     pass
 
+
 _RequiredPutBucketVersioningRequestRequestTypeDef = TypedDict(
     "_RequiredPutBucketVersioningRequestRequestTypeDef",
     {
         "Bucket": str,
         "VersioningConfiguration": VersioningConfigurationTypeDef,
     },
 )
@@ -4975,114 +5070,99 @@
         "ChecksumAlgorithm": ChecksumAlgorithmType,
         "MFA": str,
         "ExpectedBucketOwner": str,
     },
     total=False,
 )
 
+
 class PutBucketVersioningRequestRequestTypeDef(
     _RequiredPutBucketVersioningRequestRequestTypeDef,
     _OptionalPutBucketVersioningRequestRequestTypeDef,
 ):
     pass
 
-_RequiredRoutingRuleTypeDef = TypedDict(
-    "_RequiredRoutingRuleTypeDef",
-    {
-        "Redirect": RedirectTypeDef,
-    },
-)
-_OptionalRoutingRuleTypeDef = TypedDict(
-    "_OptionalRoutingRuleTypeDef",
+
+RoutingRuleTypeDef = TypedDict(
+    "RoutingRuleTypeDef",
     {
         "Condition": ConditionTypeDef,
+        "Redirect": RedirectTypeDef,
     },
-    total=False,
 )
 
-class RoutingRuleTypeDef(_RequiredRoutingRuleTypeDef, _OptionalRoutingRuleTypeDef):
-    pass
-
 ServerSideEncryptionRuleTypeDef = TypedDict(
     "ServerSideEncryptionRuleTypeDef",
     {
         "ApplyServerSideEncryptionByDefault": ServerSideEncryptionByDefaultTypeDef,
         "BucketKeyEnabled": bool,
     },
-    total=False,
 )
 
 SourceSelectionCriteriaTypeDef = TypedDict(
     "SourceSelectionCriteriaTypeDef",
     {
         "SseKmsEncryptedObjects": SseKmsEncryptedObjectsTypeDef,
         "ReplicaModifications": ReplicaModificationsTypeDef,
     },
-    total=False,
 )
 
 StatsEventTypeDef = TypedDict(
     "StatsEventTypeDef",
     {
         "Details": StatsTypeDef,
     },
-    total=False,
 )
 
 AnalyticsFilterTypeDef = TypedDict(
     "AnalyticsFilterTypeDef",
     {
         "Prefix": str,
         "Tag": TagTypeDef,
         "And": AnalyticsAndOperatorTypeDef,
     },
-    total=False,
 )
 
 IntelligentTieringFilterTypeDef = TypedDict(
     "IntelligentTieringFilterTypeDef",
     {
         "Prefix": str,
         "Tag": TagTypeDef,
         "And": IntelligentTieringAndOperatorTypeDef,
     },
-    total=False,
 )
 
 LifecycleRuleFilterTypeDef = TypedDict(
     "LifecycleRuleFilterTypeDef",
     {
         "Prefix": str,
         "Tag": TagTypeDef,
         "ObjectSizeGreaterThan": int,
         "ObjectSizeLessThan": int,
         "And": LifecycleRuleAndOperatorTypeDef,
     },
-    total=False,
 )
 
 MetricsFilterTypeDef = TypedDict(
     "MetricsFilterTypeDef",
     {
         "Prefix": str,
         "Tag": TagTypeDef,
         "AccessPointArn": str,
         "And": MetricsAndOperatorTypeDef,
     },
-    total=False,
 )
 
 ReplicationRuleFilterTypeDef = TypedDict(
     "ReplicationRuleFilterTypeDef",
     {
         "Prefix": str,
         "Tag": TagTypeDef,
         "And": ReplicationRuleAndOperatorTypeDef,
     },
-    total=False,
 )
 
 _RequiredPutBucketTaggingRequestBucketTaggingPutTypeDef = TypedDict(
     "_RequiredPutBucketTaggingRequestBucketTaggingPutTypeDef",
     {
         "Tagging": TaggingTypeDef,
     },
@@ -5092,20 +5172,22 @@
     {
         "ChecksumAlgorithm": ChecksumAlgorithmType,
         "ExpectedBucketOwner": str,
     },
     total=False,
 )
 
+
 class PutBucketTaggingRequestBucketTaggingPutTypeDef(
     _RequiredPutBucketTaggingRequestBucketTaggingPutTypeDef,
     _OptionalPutBucketTaggingRequestBucketTaggingPutTypeDef,
 ):
     pass
 
+
 _RequiredPutBucketTaggingRequestRequestTypeDef = TypedDict(
     "_RequiredPutBucketTaggingRequestRequestTypeDef",
     {
         "Bucket": str,
         "Tagging": TaggingTypeDef,
     },
 )
@@ -5114,19 +5196,21 @@
     {
         "ChecksumAlgorithm": ChecksumAlgorithmType,
         "ExpectedBucketOwner": str,
     },
     total=False,
 )
 
+
 class PutBucketTaggingRequestRequestTypeDef(
     _RequiredPutBucketTaggingRequestRequestTypeDef, _OptionalPutBucketTaggingRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredPutObjectTaggingRequestRequestTypeDef = TypedDict(
     "_RequiredPutObjectTaggingRequestRequestTypeDef",
     {
         "Bucket": str,
         "Key": str,
         "Tagging": TaggingTypeDef,
     },
@@ -5139,19 +5223,21 @@
         "ChecksumAlgorithm": ChecksumAlgorithmType,
         "ExpectedBucketOwner": str,
         "RequestPayer": Literal["requester"],
     },
     total=False,
 )
 
+
 class PutObjectTaggingRequestRequestTypeDef(
     _RequiredPutObjectTaggingRequestRequestTypeDef, _OptionalPutObjectTaggingRequestRequestTypeDef
 ):
     pass
 
+
 StorageClassAnalysisDataExportTypeDef = TypedDict(
     "StorageClassAnalysisDataExportTypeDef",
     {
         "OutputSchemaVersion": Literal["V_1"],
         "Destination": AnalyticsExportDestinationTypeDef,
     },
 )
@@ -5167,20 +5253,22 @@
     {
         "ChecksumAlgorithm": ChecksumAlgorithmType,
         "ExpectedBucketOwner": str,
     },
     total=False,
 )
 
+
 class PutBucketCorsRequestBucketCorsPutTypeDef(
     _RequiredPutBucketCorsRequestBucketCorsPutTypeDef,
     _OptionalPutBucketCorsRequestBucketCorsPutTypeDef,
 ):
     pass
 
+
 _RequiredPutBucketCorsRequestRequestTypeDef = TypedDict(
     "_RequiredPutBucketCorsRequestRequestTypeDef",
     {
         "Bucket": str,
         "CORSConfiguration": CORSConfigurationTypeDef,
     },
 )
@@ -5189,19 +5277,21 @@
     {
         "ChecksumAlgorithm": ChecksumAlgorithmType,
         "ExpectedBucketOwner": str,
     },
     total=False,
 )
 
+
 class PutBucketCorsRequestRequestTypeDef(
     _RequiredPutBucketCorsRequestRequestTypeDef, _OptionalPutBucketCorsRequestRequestTypeDef
 ):
     pass
 
+
 CompleteMultipartUploadRequestMultipartUploadCompleteTypeDef = TypedDict(
     "CompleteMultipartUploadRequestMultipartUploadCompleteTypeDef",
     {
         "MultipartUpload": CompletedMultipartUploadTypeDef,
         "ChecksumCRC32": str,
         "ChecksumCRC32C": str,
         "ChecksumSHA1": str,
@@ -5236,27 +5326,28 @@
         "SSECustomerAlgorithm": str,
         "SSECustomerKey": str,
         "SSECustomerKeyMD5": str,
     },
     total=False,
 )
 
+
 class CompleteMultipartUploadRequestRequestTypeDef(
     _RequiredCompleteMultipartUploadRequestRequestTypeDef,
     _OptionalCompleteMultipartUploadRequestRequestTypeDef,
 ):
     pass
 
+
 ObjectLockConfigurationTypeDef = TypedDict(
     "ObjectLockConfigurationTypeDef",
     {
         "ObjectLockEnabled": Literal["Enabled"],
         "Rule": ObjectLockRuleTypeDef,
     },
-    total=False,
 )
 
 _RequiredDeleteObjectsRequestBucketDeleteObjectsTypeDef = TypedDict(
     "_RequiredDeleteObjectsRequestBucketDeleteObjectsTypeDef",
     {
         "Delete": DeleteTypeDef,
     },
@@ -5269,20 +5360,22 @@
         "BypassGovernanceRetention": bool,
         "ExpectedBucketOwner": str,
         "ChecksumAlgorithm": ChecksumAlgorithmType,
     },
     total=False,
 )
 
+
 class DeleteObjectsRequestBucketDeleteObjectsTypeDef(
     _RequiredDeleteObjectsRequestBucketDeleteObjectsTypeDef,
     _OptionalDeleteObjectsRequestBucketDeleteObjectsTypeDef,
 ):
     pass
 
+
 _RequiredDeleteObjectsRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteObjectsRequestRequestTypeDef",
     {
         "Bucket": str,
         "Delete": DeleteTypeDef,
     },
 )
@@ -5294,40 +5387,41 @@
         "BypassGovernanceRetention": bool,
         "ExpectedBucketOwner": str,
         "ChecksumAlgorithm": ChecksumAlgorithmType,
     },
     total=False,
 )
 
+
 class DeleteObjectsRequestRequestTypeDef(
     _RequiredDeleteObjectsRequestRequestTypeDef, _OptionalDeleteObjectsRequestRequestTypeDef
 ):
     pass
 
+
 NotificationConfigurationFilterTypeDef = TypedDict(
     "NotificationConfigurationFilterTypeDef",
     {
         "Key": S3KeyFilterTypeDef,
     },
-    total=False,
 )
 
 GetObjectAttributesOutputTypeDef = TypedDict(
     "GetObjectAttributesOutputTypeDef",
     {
         "DeleteMarker": bool,
         "LastModified": datetime,
         "VersionId": str,
         "RequestCharged": Literal["requester"],
         "ETag": str,
         "Checksum": ChecksumTypeDef,
         "ObjectParts": GetObjectAttributesPartsTypeDef,
         "StorageClass": StorageClassType,
         "ObjectSize": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AccessControlPolicyTypeDef = TypedDict(
     "AccessControlPolicyTypeDef",
     {
         "Grants": Sequence[GrantTypeDef],
@@ -5337,25 +5431,25 @@
 )
 
 GetBucketAclOutputTypeDef = TypedDict(
     "GetBucketAclOutputTypeDef",
     {
         "Owner": OwnerTypeDef,
         "Grants": List[GrantTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetObjectAclOutputTypeDef = TypedDict(
     "GetObjectAclOutputTypeDef",
     {
         "Owner": OwnerTypeDef,
         "Grants": List[GrantTypeDef],
         "RequestCharged": Literal["requester"],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredS3LocationTypeDef = TypedDict(
     "_RequiredS3LocationTypeDef",
     {
         "BucketName": str,
@@ -5371,45 +5465,38 @@
         "Tagging": TaggingTypeDef,
         "UserMetadata": Sequence[MetadataEntryTypeDef],
         "StorageClass": StorageClassType,
     },
     total=False,
 )
 
+
 class S3LocationTypeDef(_RequiredS3LocationTypeDef, _OptionalS3LocationTypeDef):
     pass
 
+
 LoggingEnabledResponseMetadataTypeDef = TypedDict(
     "LoggingEnabledResponseMetadataTypeDef",
     {
         "TargetBucket": str,
         "TargetGrants": List[TargetGrantTypeDef],
         "TargetPrefix": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredLoggingEnabledTypeDef = TypedDict(
-    "_RequiredLoggingEnabledTypeDef",
+LoggingEnabledTypeDef = TypedDict(
+    "LoggingEnabledTypeDef",
     {
         "TargetBucket": str,
-        "TargetPrefix": str,
-    },
-)
-_OptionalLoggingEnabledTypeDef = TypedDict(
-    "_OptionalLoggingEnabledTypeDef",
-    {
         "TargetGrants": List[TargetGrantTypeDef],
+        "TargetPrefix": str,
     },
-    total=False,
 )
 
-class LoggingEnabledTypeDef(_RequiredLoggingEnabledTypeDef, _OptionalLoggingEnabledTypeDef):
-    pass
-
 ListMultipartUploadsOutputTypeDef = TypedDict(
     "ListMultipartUploadsOutputTypeDef",
     {
         "Bucket": str,
         "KeyMarker": str,
         "UploadIdMarker": str,
         "NextKeyMarker": str,
@@ -5418,40 +5505,29 @@
         "NextUploadIdMarker": str,
         "MaxUploads": int,
         "IsTruncated": bool,
         "Uploads": List[MultipartUploadTypeDef],
         "CommonPrefixes": List[CommonPrefixTypeDef],
         "EncodingType": Literal["url"],
         "RequestCharged": Literal["requester"],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredInventoryS3BucketDestinationTypeDef = TypedDict(
-    "_RequiredInventoryS3BucketDestinationTypeDef",
+InventoryS3BucketDestinationTypeDef = TypedDict(
+    "InventoryS3BucketDestinationTypeDef",
     {
+        "AccountId": str,
         "Bucket": str,
         "Format": InventoryFormatType,
-    },
-)
-_OptionalInventoryS3BucketDestinationTypeDef = TypedDict(
-    "_OptionalInventoryS3BucketDestinationTypeDef",
-    {
-        "AccountId": str,
         "Prefix": str,
         "Encryption": InventoryEncryptionTypeDef,
     },
-    total=False,
 )
 
-class InventoryS3BucketDestinationTypeDef(
-    _RequiredInventoryS3BucketDestinationTypeDef, _OptionalInventoryS3BucketDestinationTypeDef
-):
-    pass
-
 _RequiredSelectObjectContentRequestRequestTypeDef = TypedDict(
     "_RequiredSelectObjectContentRequestRequestTypeDef",
     {
         "Bucket": str,
         "Key": str,
         "Expression": str,
         "ExpressionType": Literal["SQL"],
@@ -5468,67 +5544,60 @@
         "RequestProgress": RequestProgressTypeDef,
         "ScanRange": ScanRangeTypeDef,
         "ExpectedBucketOwner": str,
     },
     total=False,
 )
 
+
 class SelectObjectContentRequestRequestTypeDef(
     _RequiredSelectObjectContentRequestRequestTypeDef,
     _OptionalSelectObjectContentRequestRequestTypeDef,
 ):
     pass
 
+
 SelectParametersTypeDef = TypedDict(
     "SelectParametersTypeDef",
     {
         "InputSerialization": InputSerializationTypeDef,
         "ExpressionType": Literal["SQL"],
         "Expression": str,
         "OutputSerialization": OutputSerializationTypeDef,
     },
 )
 
 GetBucketLifecycleOutputTypeDef = TypedDict(
     "GetBucketLifecycleOutputTypeDef",
     {
         "Rules": List[RuleTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 LifecycleConfigurationTypeDef = TypedDict(
     "LifecycleConfigurationTypeDef",
     {
         "Rules": Sequence[RuleTypeDef],
     },
 )
 
-_RequiredDestinationTypeDef = TypedDict(
-    "_RequiredDestinationTypeDef",
+DestinationTypeDef = TypedDict(
+    "DestinationTypeDef",
     {
         "Bucket": str,
-    },
-)
-_OptionalDestinationTypeDef = TypedDict(
-    "_OptionalDestinationTypeDef",
-    {
         "Account": str,
         "StorageClass": StorageClassType,
         "AccessControlTranslation": AccessControlTranslationTypeDef,
         "EncryptionConfiguration": EncryptionConfigurationTypeDef,
         "ReplicationTime": ReplicationTimeTypeDef,
         "Metrics": MetricsTypeDef,
     },
-    total=False,
 )
 
-class DestinationTypeDef(_RequiredDestinationTypeDef, _OptionalDestinationTypeDef):
-    pass
-
 _RequiredPutBucketNotificationRequestRequestTypeDef = TypedDict(
     "_RequiredPutBucketNotificationRequestRequestTypeDef",
     {
         "Bucket": str,
         "NotificationConfiguration": NotificationConfigurationDeprecatedTypeDef,
     },
 )
@@ -5537,35 +5606,37 @@
     {
         "ChecksumAlgorithm": ChecksumAlgorithmType,
         "ExpectedBucketOwner": str,
     },
     total=False,
 )
 
+
 class PutBucketNotificationRequestRequestTypeDef(
     _RequiredPutBucketNotificationRequestRequestTypeDef,
     _OptionalPutBucketNotificationRequestRequestTypeDef,
 ):
     pass
 
+
 ListObjectsOutputTypeDef = TypedDict(
     "ListObjectsOutputTypeDef",
     {
         "IsTruncated": bool,
         "Marker": str,
         "NextMarker": str,
         "Contents": List[ObjectTypeDef],
         "Name": str,
         "Prefix": str,
         "Delimiter": str,
         "MaxKeys": int,
         "CommonPrefixes": List[CommonPrefixTypeDef],
         "EncodingType": Literal["url"],
         "RequestCharged": Literal["requester"],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListObjectsV2OutputTypeDef = TypedDict(
     "ListObjectsV2OutputTypeDef",
     {
         "IsTruncated": bool,
@@ -5577,15 +5648,15 @@
         "CommonPrefixes": List[CommonPrefixTypeDef],
         "EncodingType": Literal["url"],
         "KeyCount": int,
         "ContinuationToken": str,
         "NextContinuationToken": str,
         "StartAfter": str,
         "RequestCharged": Literal["requester"],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListObjectVersionsOutputTypeDef = TypedDict(
     "ListObjectVersionsOutputTypeDef",
     {
         "IsTruncated": bool,
@@ -5598,23 +5669,23 @@
         "Name": str,
         "Prefix": str,
         "Delimiter": str,
         "MaxKeys": int,
         "CommonPrefixes": List[CommonPrefixTypeDef],
         "EncodingType": Literal["url"],
         "RequestCharged": Literal["requester"],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetBucketOwnershipControlsOutputTypeDef = TypedDict(
     "GetBucketOwnershipControlsOutputTypeDef",
     {
         "OwnershipControls": OwnershipControlsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredPutBucketOwnershipControlsRequestRequestTypeDef = TypedDict(
     "_RequiredPutBucketOwnershipControlsRequestRequestTypeDef",
     {
         "Bucket": str,
@@ -5626,28 +5697,30 @@
     {
         "ContentMD5": str,
         "ExpectedBucketOwner": str,
     },
     total=False,
 )
 
+
 class PutBucketOwnershipControlsRequestRequestTypeDef(
     _RequiredPutBucketOwnershipControlsRequestRequestTypeDef,
     _OptionalPutBucketOwnershipControlsRequestRequestTypeDef,
 ):
     pass
 
+
 GetBucketWebsiteOutputTypeDef = TypedDict(
     "GetBucketWebsiteOutputTypeDef",
     {
         "RedirectAllRequestsTo": RedirectAllRequestsToTypeDef,
         "IndexDocument": IndexDocumentTypeDef,
         "ErrorDocument": ErrorDocumentTypeDef,
         "RoutingRules": List[RoutingRuleTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 WebsiteConfigurationTypeDef = TypedDict(
     "WebsiteConfigurationTypeDef",
     {
         "ErrorDocument": ErrorDocumentTypeDef,
@@ -5670,94 +5743,61 @@
     {
         "Records": RecordsEventTypeDef,
         "Stats": StatsEventTypeDef,
         "Progress": ProgressEventTypeDef,
         "Cont": Dict[str, Any],
         "End": Dict[str, Any],
     },
-    total=False,
 )
 
-_RequiredIntelligentTieringConfigurationTypeDef = TypedDict(
-    "_RequiredIntelligentTieringConfigurationTypeDef",
+IntelligentTieringConfigurationTypeDef = TypedDict(
+    "IntelligentTieringConfigurationTypeDef",
     {
         "Id": str,
+        "Filter": IntelligentTieringFilterTypeDef,
         "Status": IntelligentTieringStatusType,
         "Tierings": List[TieringTypeDef],
     },
 )
-_OptionalIntelligentTieringConfigurationTypeDef = TypedDict(
-    "_OptionalIntelligentTieringConfigurationTypeDef",
-    {
-        "Filter": IntelligentTieringFilterTypeDef,
-    },
-    total=False,
-)
-
-class IntelligentTieringConfigurationTypeDef(
-    _RequiredIntelligentTieringConfigurationTypeDef, _OptionalIntelligentTieringConfigurationTypeDef
-):
-    pass
 
-_RequiredLifecycleRuleTypeDef = TypedDict(
-    "_RequiredLifecycleRuleTypeDef",
-    {
-        "Status": ExpirationStatusType,
-    },
-)
-_OptionalLifecycleRuleTypeDef = TypedDict(
-    "_OptionalLifecycleRuleTypeDef",
+LifecycleRuleTypeDef = TypedDict(
+    "LifecycleRuleTypeDef",
     {
         "Expiration": LifecycleExpirationTypeDef,
         "ID": str,
         "Prefix": str,
         "Filter": LifecycleRuleFilterTypeDef,
+        "Status": ExpirationStatusType,
         "Transitions": List[TransitionTypeDef],
         "NoncurrentVersionTransitions": List[NoncurrentVersionTransitionTypeDef],
         "NoncurrentVersionExpiration": NoncurrentVersionExpirationTypeDef,
         "AbortIncompleteMultipartUpload": AbortIncompleteMultipartUploadTypeDef,
     },
-    total=False,
 )
 
-class LifecycleRuleTypeDef(_RequiredLifecycleRuleTypeDef, _OptionalLifecycleRuleTypeDef):
-    pass
-
-_RequiredMetricsConfigurationTypeDef = TypedDict(
-    "_RequiredMetricsConfigurationTypeDef",
+MetricsConfigurationTypeDef = TypedDict(
+    "MetricsConfigurationTypeDef",
     {
         "Id": str,
-    },
-)
-_OptionalMetricsConfigurationTypeDef = TypedDict(
-    "_OptionalMetricsConfigurationTypeDef",
-    {
         "Filter": MetricsFilterTypeDef,
     },
-    total=False,
 )
 
-class MetricsConfigurationTypeDef(
-    _RequiredMetricsConfigurationTypeDef, _OptionalMetricsConfigurationTypeDef
-):
-    pass
-
 StorageClassAnalysisTypeDef = TypedDict(
     "StorageClassAnalysisTypeDef",
     {
         "DataExport": StorageClassAnalysisDataExportTypeDef,
     },
-    total=False,
 )
 
 GetObjectLockConfigurationOutputTypeDef = TypedDict(
     "GetObjectLockConfigurationOutputTypeDef",
     {
         "ObjectLockConfiguration": ObjectLockConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredPutObjectLockConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredPutObjectLockConfigurationRequestRequestTypeDef",
     {
         "Bucket": str,
@@ -5772,83 +5812,52 @@
         "ContentMD5": str,
         "ChecksumAlgorithm": ChecksumAlgorithmType,
         "ExpectedBucketOwner": str,
     },
     total=False,
 )
 
+
 class PutObjectLockConfigurationRequestRequestTypeDef(
     _RequiredPutObjectLockConfigurationRequestRequestTypeDef,
     _OptionalPutObjectLockConfigurationRequestRequestTypeDef,
 ):
     pass
 
-_RequiredLambdaFunctionConfigurationTypeDef = TypedDict(
-    "_RequiredLambdaFunctionConfigurationTypeDef",
+
+LambdaFunctionConfigurationTypeDef = TypedDict(
+    "LambdaFunctionConfigurationTypeDef",
     {
+        "Id": str,
         "LambdaFunctionArn": str,
         "Events": List[EventType],
-    },
-)
-_OptionalLambdaFunctionConfigurationTypeDef = TypedDict(
-    "_OptionalLambdaFunctionConfigurationTypeDef",
-    {
-        "Id": str,
         "Filter": NotificationConfigurationFilterTypeDef,
     },
-    total=False,
 )
 
-class LambdaFunctionConfigurationTypeDef(
-    _RequiredLambdaFunctionConfigurationTypeDef, _OptionalLambdaFunctionConfigurationTypeDef
-):
-    pass
-
-_RequiredQueueConfigurationTypeDef = TypedDict(
-    "_RequiredQueueConfigurationTypeDef",
+QueueConfigurationTypeDef = TypedDict(
+    "QueueConfigurationTypeDef",
     {
+        "Id": str,
         "QueueArn": str,
         "Events": List[EventType],
-    },
-)
-_OptionalQueueConfigurationTypeDef = TypedDict(
-    "_OptionalQueueConfigurationTypeDef",
-    {
-        "Id": str,
         "Filter": NotificationConfigurationFilterTypeDef,
     },
-    total=False,
 )
 
-class QueueConfigurationTypeDef(
-    _RequiredQueueConfigurationTypeDef, _OptionalQueueConfigurationTypeDef
-):
-    pass
-
-_RequiredTopicConfigurationTypeDef = TypedDict(
-    "_RequiredTopicConfigurationTypeDef",
+TopicConfigurationTypeDef = TypedDict(
+    "TopicConfigurationTypeDef",
     {
+        "Id": str,
         "TopicArn": str,
         "Events": List[EventType],
-    },
-)
-_OptionalTopicConfigurationTypeDef = TypedDict(
-    "_OptionalTopicConfigurationTypeDef",
-    {
-        "Id": str,
         "Filter": NotificationConfigurationFilterTypeDef,
     },
-    total=False,
 )
 
-class TopicConfigurationTypeDef(
-    _RequiredTopicConfigurationTypeDef, _OptionalTopicConfigurationTypeDef
-):
-    pass
-
 PutBucketAclRequestBucketAclPutTypeDef = TypedDict(
     "PutBucketAclRequestBucketAclPutTypeDef",
     {
         "ACL": BucketCannedACLType,
         "AccessControlPolicy": AccessControlPolicyTypeDef,
         "ChecksumAlgorithm": ChecksumAlgorithmType,
         "GrantFullControl": str,
@@ -5879,19 +5888,21 @@
         "GrantWrite": str,
         "GrantWriteACP": str,
         "ExpectedBucketOwner": str,
     },
     total=False,
 )
 
+
 class PutBucketAclRequestRequestTypeDef(
     _RequiredPutBucketAclRequestRequestTypeDef, _OptionalPutBucketAclRequestRequestTypeDef
 ):
     pass
 
+
 PutObjectAclRequestObjectAclPutTypeDef = TypedDict(
     "PutObjectAclRequestObjectAclPutTypeDef",
     {
         "ACL": ObjectCannedACLType,
         "AccessControlPolicy": AccessControlPolicyTypeDef,
         "ChecksumAlgorithm": ChecksumAlgorithmType,
         "GrantFullControl": str,
@@ -5927,19 +5938,21 @@
         "RequestPayer": Literal["requester"],
         "VersionId": str,
         "ExpectedBucketOwner": str,
     },
     total=False,
 )
 
+
 class PutObjectAclRequestRequestTypeDef(
     _RequiredPutObjectAclRequestRequestTypeDef, _OptionalPutObjectAclRequestRequestTypeDef
 ):
     pass
 
+
 OutputLocationTypeDef = TypedDict(
     "OutputLocationTypeDef",
     {
         "S3": S3LocationTypeDef,
     },
     total=False,
 )
@@ -5952,15 +5965,15 @@
     total=False,
 )
 
 GetBucketLoggingOutputTypeDef = TypedDict(
     "GetBucketLoggingOutputTypeDef",
     {
         "LoggingEnabled": LoggingEnabledTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 InventoryDestinationTypeDef = TypedDict(
     "InventoryDestinationTypeDef",
     {
         "S3BucketDestination": InventoryS3BucketDestinationTypeDef,
@@ -5989,44 +6002,37 @@
         "ChecksumAlgorithm": ChecksumAlgorithmType,
         "LifecycleConfiguration": LifecycleConfigurationTypeDef,
         "ExpectedBucketOwner": str,
     },
     total=False,
 )
 
+
 class PutBucketLifecycleRequestRequestTypeDef(
     _RequiredPutBucketLifecycleRequestRequestTypeDef,
     _OptionalPutBucketLifecycleRequestRequestTypeDef,
 ):
     pass
 
-_RequiredReplicationRuleTypeDef = TypedDict(
-    "_RequiredReplicationRuleTypeDef",
-    {
-        "Status": ReplicationRuleStatusType,
-        "Destination": DestinationTypeDef,
-    },
-)
-_OptionalReplicationRuleTypeDef = TypedDict(
-    "_OptionalReplicationRuleTypeDef",
+
+ReplicationRuleTypeDef = TypedDict(
+    "ReplicationRuleTypeDef",
     {
         "ID": str,
         "Priority": int,
         "Prefix": str,
         "Filter": ReplicationRuleFilterTypeDef,
+        "Status": ReplicationRuleStatusType,
         "SourceSelectionCriteria": SourceSelectionCriteriaTypeDef,
         "ExistingObjectReplication": ExistingObjectReplicationTypeDef,
+        "Destination": DestinationTypeDef,
         "DeleteMarkerReplication": DeleteMarkerReplicationTypeDef,
     },
-    total=False,
 )
 
-class ReplicationRuleTypeDef(_RequiredReplicationRuleTypeDef, _OptionalReplicationRuleTypeDef):
-    pass
-
 _RequiredPutBucketWebsiteRequestBucketWebsitePutTypeDef = TypedDict(
     "_RequiredPutBucketWebsiteRequestBucketWebsitePutTypeDef",
     {
         "WebsiteConfiguration": WebsiteConfigurationTypeDef,
     },
 )
 _OptionalPutBucketWebsiteRequestBucketWebsitePutTypeDef = TypedDict(
@@ -6034,20 +6040,22 @@
     {
         "ChecksumAlgorithm": ChecksumAlgorithmType,
         "ExpectedBucketOwner": str,
     },
     total=False,
 )
 
+
 class PutBucketWebsiteRequestBucketWebsitePutTypeDef(
     _RequiredPutBucketWebsiteRequestBucketWebsitePutTypeDef,
     _OptionalPutBucketWebsiteRequestBucketWebsitePutTypeDef,
 ):
     pass
 
+
 _RequiredPutBucketWebsiteRequestRequestTypeDef = TypedDict(
     "_RequiredPutBucketWebsiteRequestRequestTypeDef",
     {
         "Bucket": str,
         "WebsiteConfiguration": WebsiteConfigurationTypeDef,
     },
 )
@@ -6056,24 +6064,26 @@
     {
         "ChecksumAlgorithm": ChecksumAlgorithmType,
         "ExpectedBucketOwner": str,
     },
     total=False,
 )
 
+
 class PutBucketWebsiteRequestRequestTypeDef(
     _RequiredPutBucketWebsiteRequestRequestTypeDef, _OptionalPutBucketWebsiteRequestRequestTypeDef
 ):
     pass
 
+
 GetBucketEncryptionOutputTypeDef = TypedDict(
     "GetBucketEncryptionOutputTypeDef",
     {
         "ServerSideEncryptionConfiguration": ServerSideEncryptionConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredPutBucketEncryptionRequestRequestTypeDef = TypedDict(
     "_RequiredPutBucketEncryptionRequestRequestTypeDef",
     {
         "Bucket": str,
@@ -6086,44 +6096,46 @@
         "ContentMD5": str,
         "ChecksumAlgorithm": ChecksumAlgorithmType,
         "ExpectedBucketOwner": str,
     },
     total=False,
 )
 
+
 class PutBucketEncryptionRequestRequestTypeDef(
     _RequiredPutBucketEncryptionRequestRequestTypeDef,
     _OptionalPutBucketEncryptionRequestRequestTypeDef,
 ):
     pass
 
+
 SelectObjectContentOutputTypeDef = TypedDict(
     "SelectObjectContentOutputTypeDef",
     {
-        "Payload": SelectObjectContentEventStreamTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Payload": "EventStream[SelectObjectContentEventStreamTypeDef]",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetBucketIntelligentTieringConfigurationOutputTypeDef = TypedDict(
     "GetBucketIntelligentTieringConfigurationOutputTypeDef",
     {
         "IntelligentTieringConfiguration": IntelligentTieringConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListBucketIntelligentTieringConfigurationsOutputTypeDef = TypedDict(
     "ListBucketIntelligentTieringConfigurationsOutputTypeDef",
     {
         "IsTruncated": bool,
         "ContinuationToken": str,
         "NextContinuationToken": str,
         "IntelligentTieringConfigurationList": List[IntelligentTieringConfigurationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutBucketIntelligentTieringConfigurationRequestRequestTypeDef = TypedDict(
     "PutBucketIntelligentTieringConfigurationRequestRequestTypeDef",
     {
         "Bucket": str,
@@ -6139,34 +6151,34 @@
     },
 )
 
 GetBucketLifecycleConfigurationOutputTypeDef = TypedDict(
     "GetBucketLifecycleConfigurationOutputTypeDef",
     {
         "Rules": List[LifecycleRuleTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetBucketMetricsConfigurationOutputTypeDef = TypedDict(
     "GetBucketMetricsConfigurationOutputTypeDef",
     {
         "MetricsConfiguration": MetricsConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListBucketMetricsConfigurationsOutputTypeDef = TypedDict(
     "ListBucketMetricsConfigurationsOutputTypeDef",
     {
         "IsTruncated": bool,
         "ContinuationToken": str,
         "NextContinuationToken": str,
         "MetricsConfigurationList": List[MetricsConfigurationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredPutBucketMetricsConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredPutBucketMetricsConfigurationRequestRequestTypeDef",
     {
         "Bucket": str,
@@ -6178,48 +6190,39 @@
     "_OptionalPutBucketMetricsConfigurationRequestRequestTypeDef",
     {
         "ExpectedBucketOwner": str,
     },
     total=False,
 )
 
+
 class PutBucketMetricsConfigurationRequestRequestTypeDef(
     _RequiredPutBucketMetricsConfigurationRequestRequestTypeDef,
     _OptionalPutBucketMetricsConfigurationRequestRequestTypeDef,
 ):
     pass
 
-_RequiredAnalyticsConfigurationTypeDef = TypedDict(
-    "_RequiredAnalyticsConfigurationTypeDef",
+
+AnalyticsConfigurationTypeDef = TypedDict(
+    "AnalyticsConfigurationTypeDef",
     {
         "Id": str,
-        "StorageClassAnalysis": StorageClassAnalysisTypeDef,
-    },
-)
-_OptionalAnalyticsConfigurationTypeDef = TypedDict(
-    "_OptionalAnalyticsConfigurationTypeDef",
-    {
         "Filter": AnalyticsFilterTypeDef,
+        "StorageClassAnalysis": StorageClassAnalysisTypeDef,
     },
-    total=False,
 )
 
-class AnalyticsConfigurationTypeDef(
-    _RequiredAnalyticsConfigurationTypeDef, _OptionalAnalyticsConfigurationTypeDef
-):
-    pass
-
 NotificationConfigurationResponseMetadataTypeDef = TypedDict(
     "NotificationConfigurationResponseMetadataTypeDef",
     {
         "TopicConfigurations": List[TopicConfigurationTypeDef],
         "QueueConfigurations": List[QueueConfigurationTypeDef],
         "LambdaFunctionConfigurations": List[LambdaFunctionConfigurationTypeDef],
         "EventBridgeConfiguration": Dict[str, Any],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 NotificationConfigurationTypeDef = TypedDict(
     "NotificationConfigurationTypeDef",
     {
         "TopicConfigurations": Sequence[TopicConfigurationTypeDef],
@@ -6255,20 +6258,22 @@
     {
         "ChecksumAlgorithm": ChecksumAlgorithmType,
         "ExpectedBucketOwner": str,
     },
     total=False,
 )
 
+
 class PutBucketLoggingRequestBucketLoggingPutTypeDef(
     _RequiredPutBucketLoggingRequestBucketLoggingPutTypeDef,
     _OptionalPutBucketLoggingRequestBucketLoggingPutTypeDef,
 ):
     pass
 
+
 _RequiredPutBucketLoggingRequestRequestTypeDef = TypedDict(
     "_RequiredPutBucketLoggingRequestRequestTypeDef",
     {
         "Bucket": str,
         "BucketLoggingStatus": BucketLoggingStatusTypeDef,
     },
 )
@@ -6277,43 +6282,34 @@
     {
         "ChecksumAlgorithm": ChecksumAlgorithmType,
         "ExpectedBucketOwner": str,
     },
     total=False,
 )
 
+
 class PutBucketLoggingRequestRequestTypeDef(
     _RequiredPutBucketLoggingRequestRequestTypeDef, _OptionalPutBucketLoggingRequestRequestTypeDef
 ):
     pass
 
-_RequiredInventoryConfigurationTypeDef = TypedDict(
-    "_RequiredInventoryConfigurationTypeDef",
+
+InventoryConfigurationTypeDef = TypedDict(
+    "InventoryConfigurationTypeDef",
     {
         "Destination": InventoryDestinationTypeDef,
         "IsEnabled": bool,
+        "Filter": InventoryFilterTypeDef,
         "Id": str,
         "IncludedObjectVersions": InventoryIncludedObjectVersionsType,
-        "Schedule": InventoryScheduleTypeDef,
-    },
-)
-_OptionalInventoryConfigurationTypeDef = TypedDict(
-    "_OptionalInventoryConfigurationTypeDef",
-    {
-        "Filter": InventoryFilterTypeDef,
         "OptionalFields": List[InventoryOptionalFieldType],
+        "Schedule": InventoryScheduleTypeDef,
     },
-    total=False,
 )
 
-class InventoryConfigurationTypeDef(
-    _RequiredInventoryConfigurationTypeDef, _OptionalInventoryConfigurationTypeDef
-):
-    pass
-
 ReplicationConfigurationTypeDef = TypedDict(
     "ReplicationConfigurationTypeDef",
     {
         "Role": str,
         "Rules": List[ReplicationRuleTypeDef],
     },
 )
@@ -6340,36 +6336,38 @@
         "ChecksumAlgorithm": ChecksumAlgorithmType,
         "LifecycleConfiguration": BucketLifecycleConfigurationTypeDef,
         "ExpectedBucketOwner": str,
     },
     total=False,
 )
 
+
 class PutBucketLifecycleConfigurationRequestRequestTypeDef(
     _RequiredPutBucketLifecycleConfigurationRequestRequestTypeDef,
     _OptionalPutBucketLifecycleConfigurationRequestRequestTypeDef,
 ):
     pass
 
+
 GetBucketAnalyticsConfigurationOutputTypeDef = TypedDict(
     "GetBucketAnalyticsConfigurationOutputTypeDef",
     {
         "AnalyticsConfiguration": AnalyticsConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListBucketAnalyticsConfigurationsOutputTypeDef = TypedDict(
     "ListBucketAnalyticsConfigurationsOutputTypeDef",
     {
         "IsTruncated": bool,
         "ContinuationToken": str,
         "NextContinuationToken": str,
         "AnalyticsConfigurationList": List[AnalyticsConfigurationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredPutBucketAnalyticsConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredPutBucketAnalyticsConfigurationRequestRequestTypeDef",
     {
         "Bucket": str,
@@ -6381,20 +6379,22 @@
     "_OptionalPutBucketAnalyticsConfigurationRequestRequestTypeDef",
     {
         "ExpectedBucketOwner": str,
     },
     total=False,
 )
 
+
 class PutBucketAnalyticsConfigurationRequestRequestTypeDef(
     _RequiredPutBucketAnalyticsConfigurationRequestRequestTypeDef,
     _OptionalPutBucketAnalyticsConfigurationRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredPutBucketNotificationConfigurationRequestBucketNotificationPutTypeDef = TypedDict(
     "_RequiredPutBucketNotificationConfigurationRequestBucketNotificationPutTypeDef",
     {
         "NotificationConfiguration": NotificationConfigurationTypeDef,
     },
 )
 _OptionalPutBucketNotificationConfigurationRequestBucketNotificationPutTypeDef = TypedDict(
@@ -6402,20 +6402,22 @@
     {
         "ExpectedBucketOwner": str,
         "SkipDestinationValidation": bool,
     },
     total=False,
 )
 
+
 class PutBucketNotificationConfigurationRequestBucketNotificationPutTypeDef(
     _RequiredPutBucketNotificationConfigurationRequestBucketNotificationPutTypeDef,
     _OptionalPutBucketNotificationConfigurationRequestBucketNotificationPutTypeDef,
 ):
     pass
 
+
 _RequiredPutBucketNotificationConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredPutBucketNotificationConfigurationRequestRequestTypeDef",
     {
         "Bucket": str,
         "NotificationConfiguration": NotificationConfigurationTypeDef,
     },
 )
@@ -6424,20 +6426,22 @@
     {
         "ExpectedBucketOwner": str,
         "SkipDestinationValidation": bool,
     },
     total=False,
 )
 
+
 class PutBucketNotificationConfigurationRequestRequestTypeDef(
     _RequiredPutBucketNotificationConfigurationRequestRequestTypeDef,
     _OptionalPutBucketNotificationConfigurationRequestRequestTypeDef,
 ):
     pass
 
+
 RestoreObjectRequestObjectRestoreObjectTypeDef = TypedDict(
     "RestoreObjectRequestObjectRestoreObjectTypeDef",
     {
         "VersionId": str,
         "RestoreRequest": RestoreRequestTypeDef,
         "RequestPayer": Literal["requester"],
         "ChecksumAlgorithm": ChecksumAlgorithmType,
@@ -6473,35 +6477,37 @@
         "RequestPayer": Literal["requester"],
         "ChecksumAlgorithm": ChecksumAlgorithmType,
         "ExpectedBucketOwner": str,
     },
     total=False,
 )
 
+
 class RestoreObjectRequestRequestTypeDef(
     _RequiredRestoreObjectRequestRequestTypeDef, _OptionalRestoreObjectRequestRequestTypeDef
 ):
     pass
 
+
 GetBucketInventoryConfigurationOutputTypeDef = TypedDict(
     "GetBucketInventoryConfigurationOutputTypeDef",
     {
         "InventoryConfiguration": InventoryConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListBucketInventoryConfigurationsOutputTypeDef = TypedDict(
     "ListBucketInventoryConfigurationsOutputTypeDef",
     {
         "ContinuationToken": str,
         "InventoryConfigurationList": List[InventoryConfigurationTypeDef],
         "IsTruncated": bool,
         "NextContinuationToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredPutBucketInventoryConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredPutBucketInventoryConfigurationRequestRequestTypeDef",
     {
         "Bucket": str,
@@ -6513,25 +6519,27 @@
     "_OptionalPutBucketInventoryConfigurationRequestRequestTypeDef",
     {
         "ExpectedBucketOwner": str,
     },
     total=False,
 )
 
+
 class PutBucketInventoryConfigurationRequestRequestTypeDef(
     _RequiredPutBucketInventoryConfigurationRequestRequestTypeDef,
     _OptionalPutBucketInventoryConfigurationRequestRequestTypeDef,
 ):
     pass
 
+
 GetBucketReplicationOutputTypeDef = TypedDict(
     "GetBucketReplicationOutputTypeDef",
     {
         "ReplicationConfiguration": ReplicationConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredPutBucketReplicationRequestRequestTypeDef = TypedDict(
     "_RequiredPutBucketReplicationRequestRequestTypeDef",
     {
         "Bucket": str,
@@ -6544,12 +6552,13 @@
         "ChecksumAlgorithm": ChecksumAlgorithmType,
         "Token": str,
         "ExpectedBucketOwner": str,
     },
     total=False,
 )
 
+
 class PutBucketReplicationRequestRequestTypeDef(
     _RequiredPutBucketReplicationRequestRequestTypeDef,
     _OptionalPutBucketReplicationRequestRequestTypeDef,
 ):
     pass
```

### Comparing `mypy-boto3-s3-1.28.0/mypy_boto3_s3/waiter.py` & `mypy-boto3-s3-1.28.2/mypy_boto3_s3/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-s3-1.28.0/mypy_boto3_s3/waiter.pyi` & `mypy-boto3-s3-1.28.2/mypy_boto3_s3/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-s3-1.28.0/mypy_boto3_s3.egg-info/PKG-INFO` & `mypy-boto3-s3-1.28.2/mypy_boto3_s3.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-s3
-Version: 1.28.0
-Summary: Type annotations for boto3.S3 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.2
+Summary: Type annotations for boto3.S3 1.28.2 service generated with mypy-boto3-builder 7.14.6
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-s3.svg?color=blue)](https://pypi.org/project/mypy-boto3-s3)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-s3?color=blue)](https://pypistats.org/packages/mypy-boto3-s3)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.S3 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3)
+[boto3.S3 1.28.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3)
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
 [mypy-boto3-s3 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/).
 
 See how it helps to find and fix potential bugs:
 
@@ -552,15 +552,15 @@
 
 `mypy_boto3_s3.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_s3.type_defs import (
     AbortIncompleteMultipartUploadTypeDef,
-    AbortMultipartUploadOutputTypeDef,
+    ResponseMetadataTypeDef,
     AbortMultipartUploadRequestMultipartUploadAbortTypeDef,
     AbortMultipartUploadRequestRequestTypeDef,
     AccelerateConfigurationTypeDef,
     OwnerTypeDef,
     AccessControlTranslationTypeDef,
     TagTypeDef,
     AnalyticsS3BucketDestinationTypeDef,
@@ -577,24 +577,21 @@
     ClientDownloadFileRequestTypeDef,
     ClientDownloadFileobjRequestTypeDef,
     ClientGeneratePresignedPostRequestTypeDef,
     ClientUploadFileRequestTypeDef,
     ClientUploadFileobjRequestTypeDef,
     CloudFunctionConfigurationTypeDef,
     CommonPrefixTypeDef,
-    CompleteMultipartUploadOutputTypeDef,
     CompletedPartTypeDef,
     ConditionTypeDef,
     CopyObjectResultTypeDef,
     CopyObjectRequestObjectCopyFromTypeDef,
     CopyObjectRequestObjectSummaryCopyFromTypeDef,
     CopyPartResultTypeDef,
     CreateBucketConfigurationTypeDef,
-    CreateBucketOutputTypeDef,
-    CreateMultipartUploadOutputTypeDef,
     CreateMultipartUploadRequestObjectInitiateMultipartUploadTypeDef,
     CreateMultipartUploadRequestObjectSummaryInitiateMultipartUploadTypeDef,
     CreateMultipartUploadRequestRequestTypeDef,
     DefaultRetentionTypeDef,
     DeleteBucketAnalyticsConfigurationRequestRequestTypeDef,
     DeleteBucketCorsRequestBucketCorsDeleteTypeDef,
     DeleteBucketCorsRequestRequestTypeDef,
@@ -612,88 +609,74 @@
     DeleteBucketRequestBucketDeleteTypeDef,
     DeleteBucketRequestRequestTypeDef,
     DeleteBucketTaggingRequestBucketTaggingDeleteTypeDef,
     DeleteBucketTaggingRequestRequestTypeDef,
     DeleteBucketWebsiteRequestBucketWebsiteDeleteTypeDef,
     DeleteBucketWebsiteRequestRequestTypeDef,
     DeleteMarkerReplicationTypeDef,
-    DeleteObjectOutputTypeDef,
     DeleteObjectRequestObjectDeleteTypeDef,
     DeleteObjectRequestObjectSummaryDeleteTypeDef,
     DeleteObjectRequestObjectVersionDeleteTypeDef,
     DeleteObjectRequestRequestTypeDef,
-    DeleteObjectTaggingOutputTypeDef,
     DeleteObjectTaggingRequestRequestTypeDef,
     DeletedObjectTypeDef,
     ErrorTypeDef,
     DeletePublicAccessBlockRequestRequestTypeDef,
     ObjectIdentifierTypeDef,
     EncryptionConfigurationTypeDef,
-    EmptyResponseMetadataTypeDef,
     EncryptionTypeDef,
-    ErrorDocumentResponseMetadataTypeDef,
     ErrorDocumentTypeDef,
     ExistingObjectReplicationTypeDef,
     FilterRuleTypeDef,
-    GetBucketAccelerateConfigurationOutputTypeDef,
     GetBucketAccelerateConfigurationRequestRequestTypeDef,
     GetBucketAclRequestRequestTypeDef,
     GetBucketAnalyticsConfigurationRequestRequestTypeDef,
     GetBucketCorsRequestRequestTypeDef,
     GetBucketEncryptionRequestRequestTypeDef,
     GetBucketIntelligentTieringConfigurationRequestRequestTypeDef,
     GetBucketInventoryConfigurationRequestRequestTypeDef,
     GetBucketLifecycleConfigurationRequestRequestTypeDef,
     GetBucketLifecycleRequestRequestTypeDef,
-    GetBucketLocationOutputTypeDef,
     GetBucketLocationRequestRequestTypeDef,
     GetBucketLoggingRequestRequestTypeDef,
     GetBucketMetricsConfigurationRequestRequestTypeDef,
     GetBucketNotificationConfigurationRequestRequestTypeDef,
     GetBucketOwnershipControlsRequestRequestTypeDef,
-    GetBucketPolicyOutputTypeDef,
     GetBucketPolicyRequestRequestTypeDef,
     PolicyStatusTypeDef,
     GetBucketPolicyStatusRequestRequestTypeDef,
     GetBucketReplicationRequestRequestTypeDef,
-    GetBucketRequestPaymentOutputTypeDef,
     GetBucketRequestPaymentRequestRequestTypeDef,
     GetBucketTaggingRequestRequestTypeDef,
-    GetBucketVersioningOutputTypeDef,
     GetBucketVersioningRequestRequestTypeDef,
     IndexDocumentTypeDef,
     RedirectAllRequestsToTypeDef,
     GetBucketWebsiteRequestRequestTypeDef,
     GetObjectAclRequestRequestTypeDef,
     ObjectPartTypeDef,
     GetObjectAttributesRequestRequestTypeDef,
     ObjectLockLegalHoldTypeDef,
     GetObjectLegalHoldRequestRequestTypeDef,
     GetObjectLockConfigurationRequestRequestTypeDef,
-    GetObjectOutputTypeDef,
     GetObjectRequestObjectGetTypeDef,
     GetObjectRequestObjectSummaryGetTypeDef,
     GetObjectRequestObjectVersionGetTypeDef,
     GetObjectRequestRequestTypeDef,
     ObjectLockRetentionTypeDef,
     GetObjectRetentionRequestRequestTypeDef,
     GetObjectTaggingRequestRequestTypeDef,
-    GetObjectTorrentOutputTypeDef,
     GetObjectTorrentRequestRequestTypeDef,
     PublicAccessBlockConfigurationTypeDef,
     GetPublicAccessBlockRequestRequestTypeDef,
     GlacierJobParametersTypeDef,
     GranteeTypeDef,
     WaiterConfigTypeDef,
     HeadBucketRequestRequestTypeDef,
-    HeadObjectOutputTypeDef,
     HeadObjectRequestObjectVersionHeadTypeDef,
     HeadObjectRequestRequestTypeDef,
-    IndexDocumentResponseMetadataTypeDef,
-    InitiatorResponseMetadataTypeDef,
     InitiatorTypeDef,
     JSONInputTypeDef,
     TieringTypeDef,
     InventoryFilterTypeDef,
     InventoryScheduleTypeDef,
     SSEKMSTypeDef,
     JSONOutputTypeDef,
@@ -701,70 +684,82 @@
     NoncurrentVersionExpirationTypeDef,
     NoncurrentVersionTransitionTypeDef,
     TransitionTypeDef,
     ListBucketAnalyticsConfigurationsRequestRequestTypeDef,
     ListBucketIntelligentTieringConfigurationsRequestRequestTypeDef,
     ListBucketInventoryConfigurationsRequestRequestTypeDef,
     ListBucketMetricsConfigurationsRequestRequestTypeDef,
-    ListMultipartUploadsRequestListMultipartUploadsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListMultipartUploadsRequestRequestTypeDef,
-    ListObjectVersionsRequestListObjectVersionsPaginateTypeDef,
     ListObjectVersionsRequestRequestTypeDef,
-    ListObjectsRequestListObjectsPaginateTypeDef,
     ListObjectsRequestRequestTypeDef,
-    ListObjectsV2RequestListObjectsV2PaginateTypeDef,
     ListObjectsV2RequestRequestTypeDef,
     PartTypeDef,
-    ListPartsRequestListPartsPaginateTypeDef,
     ListPartsRequestRequestTypeDef,
     MetadataEntryTypeDef,
     ReplicationTimeValueTypeDef,
     QueueConfigurationDeprecatedTypeDef,
     TopicConfigurationDeprecatedTypeDef,
     ObjectDownloadFileRequestTypeDef,
     ObjectDownloadFileobjRequestTypeDef,
     RestoreStatusTypeDef,
     ObjectUploadFileRequestTypeDef,
     ObjectUploadFileobjRequestTypeDef,
-    OwnerResponseMetadataTypeDef,
     OwnershipControlsRuleTypeDef,
-    PaginatorConfigTypeDef,
     ProgressTypeDef,
     PutBucketPolicyRequestBucketPolicyPutTypeDef,
     PutBucketPolicyRequestRequestTypeDef,
     RequestPaymentConfigurationTypeDef,
     PutBucketVersioningRequestBucketVersioningEnableTypeDef,
     VersioningConfigurationTypeDef,
     PutBucketVersioningRequestBucketVersioningSuspendTypeDef,
-    PutObjectAclOutputTypeDef,
-    PutObjectLegalHoldOutputTypeDef,
-    PutObjectLockConfigurationOutputTypeDef,
-    PutObjectOutputTypeDef,
     PutObjectRequestBucketPutObjectTypeDef,
     PutObjectRequestObjectPutTypeDef,
     PutObjectRequestObjectSummaryPutTypeDef,
     PutObjectRequestRequestTypeDef,
-    PutObjectRetentionOutputTypeDef,
-    PutObjectTaggingOutputTypeDef,
     RecordsEventTypeDef,
-    RedirectAllRequestsToResponseMetadataTypeDef,
     RedirectTypeDef,
     ReplicaModificationsTypeDef,
     RequestProgressTypeDef,
-    ResponseMetadataTypeDef,
-    RestoreObjectOutputTypeDef,
-    RestoreStatusResponseMetadataTypeDef,
     ScanRangeTypeDef,
     ServerSideEncryptionByDefaultTypeDef,
     SseKmsEncryptedObjectsTypeDef,
     StatsTypeDef,
-    UploadPartOutputTypeDef,
     UploadPartRequestMultipartUploadPartUploadTypeDef,
     UploadPartRequestRequestTypeDef,
     WriteGetObjectResponseRequestRequestTypeDef,
+    AbortMultipartUploadOutputTypeDef,
+    CompleteMultipartUploadOutputTypeDef,
+    CreateBucketOutputTypeDef,
+    CreateMultipartUploadOutputTypeDef,
+    DeleteObjectOutputTypeDef,
+    DeleteObjectTaggingOutputTypeDef,
+    EmptyResponseMetadataTypeDef,
+    ErrorDocumentResponseMetadataTypeDef,
+    GetBucketAccelerateConfigurationOutputTypeDef,
+    GetBucketLocationOutputTypeDef,
+    GetBucketPolicyOutputTypeDef,
+    GetBucketRequestPaymentOutputTypeDef,
+    GetBucketVersioningOutputTypeDef,
+    GetObjectOutputTypeDef,
+    GetObjectTorrentOutputTypeDef,
+    HeadObjectOutputTypeDef,
+    IndexDocumentResponseMetadataTypeDef,
+    InitiatorResponseMetadataTypeDef,
+    OwnerResponseMetadataTypeDef,
+    PutObjectAclOutputTypeDef,
+    PutObjectLegalHoldOutputTypeDef,
+    PutObjectLockConfigurationOutputTypeDef,
+    PutObjectOutputTypeDef,
+    PutObjectRetentionOutputTypeDef,
+    PutObjectTaggingOutputTypeDef,
+    RedirectAllRequestsToResponseMetadataTypeDef,
+    RestoreObjectOutputTypeDef,
+    RestoreStatusResponseMetadataTypeDef,
+    UploadPartOutputTypeDef,
     PutBucketAccelerateConfigurationRequestRequestTypeDef,
     DeleteMarkerEntryTypeDef,
     AnalyticsAndOperatorTypeDef,
     GetBucketTaggingOutputTypeDef,
     GetObjectTaggingOutputTypeDef,
     IntelligentTieringAndOperatorTypeDef,
     LifecycleRuleAndOperatorTypeDef,
@@ -806,14 +801,19 @@
     HeadObjectRequestObjectExistsWaitTypeDef,
     HeadObjectRequestObjectNotExistsWaitTypeDef,
     MultipartUploadTypeDef,
     InputSerializationTypeDef,
     InventoryEncryptionTypeDef,
     OutputSerializationTypeDef,
     RuleTypeDef,
+    ListMultipartUploadsRequestListMultipartUploadsPaginateTypeDef,
+    ListObjectVersionsRequestListObjectVersionsPaginateTypeDef,
+    ListObjectsRequestListObjectsPaginateTypeDef,
+    ListObjectsV2RequestListObjectsV2PaginateTypeDef,
+    ListPartsRequestListPartsPaginateTypeDef,
     ListPartsOutputTypeDef,
     MetricsTypeDef,
     ReplicationTimeTypeDef,
     NotificationConfigurationDeprecatedResponseMetadataTypeDef,
     NotificationConfigurationDeprecatedTypeDef,
     ObjectTypeDef,
     ObjectVersionTypeDef,
```

### Comparing `mypy-boto3-s3-1.28.0/mypy_boto3_s3.egg-info/SOURCES.txt` & `mypy-boto3-s3-1.28.2/mypy_boto3_s3.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-s3-1.28.0/setup.py` & `mypy-boto3-s3-1.28.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-s3",
-    version="1.28.0",
+    version="1.28.2",
     packages=["mypy_boto3_s3"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.S3 1.28.0 service generated with mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.S3 1.28.2 service generated with mypy-boto3-builder 7.14.6"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

