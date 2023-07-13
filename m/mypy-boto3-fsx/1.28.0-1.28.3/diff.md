# Comparing `tmp/mypy-boto3-fsx-1.28.0.tar.gz` & `tmp/mypy-boto3-fsx-1.28.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-fsx-1.28.0.tar", last modified: Thu Jul  6 20:59:37 2023, max compression
+gzip compressed data, was "mypy-boto3-fsx-1.28.3.tar", last modified: Thu Jul 13 19:49:12 2023, max compression
```

## Comparing `mypy-boto3-fsx-1.28.0.tar` & `mypy-boto3-fsx-1.28.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:37.854308 mypy-boto3-fsx-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:41:28.000000 mypy-boto3-fsx-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    21970 2023-07-06 20:59:37.854308 mypy-boto3-fsx-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    20501 2023-07-06 20:41:28.000000 mypy-boto3-fsx-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:37.846308 mypy-boto3-fsx-1.28.0/mypy_boto3_fsx/
--rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-07-06 20:41:28.000000 mypy-boto3-fsx-1.28.0/mypy_boto3_fsx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-07-06 20:41:28.000000 mypy-boto3-fsx-1.28.0/mypy_boto3_fsx/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-06 20:41:28.000000 mypy-boto3-fsx-1.28.0/mypy_boto3_fsx/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    38786 2023-07-06 20:41:28.000000 mypy-boto3-fsx-1.28.0/mypy_boto3_fsx/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    38733 2023-07-06 20:41:28.000000 mypy-boto3-fsx-1.28.0/mypy_boto3_fsx/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    14867 2023-07-06 20:41:31.000000 mypy-boto3-fsx-1.28.0/mypy_boto3_fsx/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    14865 2023-07-06 20:41:29.000000 mypy-boto3-fsx-1.28.0/mypy_boto3_fsx/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6619 2023-07-06 20:41:29.000000 mypy-boto3-fsx-1.28.0/mypy_boto3_fsx/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6612 2023-07-06 20:41:29.000000 mypy-boto3-fsx-1.28.0/mypy_boto3_fsx/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:41:28.000000 mypy-boto3-fsx-1.28.0/mypy_boto3_fsx/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    79400 2023-07-06 20:41:33.000000 mypy-boto3-fsx-1.28.0/mypy_boto3_fsx/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    79303 2023-07-06 20:41:32.000000 mypy-boto3-fsx-1.28.0/mypy_boto3_fsx/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:41:28.000000 mypy-boto3-fsx-1.28.0/mypy_boto3_fsx/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:37.854308 mypy-boto3-fsx-1.28.0/mypy_boto3_fsx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21970 2023-07-06 20:59:37.000000 mypy-boto3-fsx-1.28.0/mypy_boto3_fsx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-06 20:59:37.000000 mypy-boto3-fsx-1.28.0/mypy_boto3_fsx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:37.000000 mypy-boto3-fsx-1.28.0/mypy_boto3_fsx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:37.000000 mypy-boto3-fsx-1.28.0/mypy_boto3_fsx.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 20:59:37.000000 mypy-boto3-fsx-1.28.0/mypy_boto3_fsx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-06 20:59:37.000000 mypy-boto3-fsx-1.28.0/mypy_boto3_fsx.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 20:59:37.854308 mypy-boto3-fsx-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-07-06 20:41:28.000000 mypy-boto3-fsx-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:49:12.653227 mypy-boto3-fsx-1.28.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-13 19:48:05.000000 mypy-boto3-fsx-1.28.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    22284 2023-07-13 19:49:12.649227 mypy-boto3-fsx-1.28.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    20815 2023-07-13 19:48:05.000000 mypy-boto3-fsx-1.28.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:49:12.645227 mypy-boto3-fsx-1.28.3/mypy_boto3_fsx/
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-07-13 19:48:05.000000 mypy-boto3-fsx-1.28.3/mypy_boto3_fsx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-07-13 19:48:05.000000 mypy-boto3-fsx-1.28.3/mypy_boto3_fsx/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-13 19:48:05.000000 mypy-boto3-fsx-1.28.3/mypy_boto3_fsx/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38786 2023-07-13 19:48:06.000000 mypy-boto3-fsx-1.28.3/mypy_boto3_fsx/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38733 2023-07-13 19:48:06.000000 mypy-boto3-fsx-1.28.3/mypy_boto3_fsx/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    15330 2023-07-13 19:48:06.000000 mypy-boto3-fsx-1.28.3/mypy_boto3_fsx/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15328 2023-07-13 19:48:06.000000 mypy-boto3-fsx-1.28.3/mypy_boto3_fsx/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6619 2023-07-13 19:48:06.000000 mypy-boto3-fsx-1.28.3/mypy_boto3_fsx/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6612 2023-07-13 19:48:06.000000 mypy-boto3-fsx-1.28.3/mypy_boto3_fsx/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 19:48:05.000000 mypy-boto3-fsx-1.28.3/mypy_boto3_fsx/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    79886 2023-07-13 19:48:08.000000 mypy-boto3-fsx-1.28.3/mypy_boto3_fsx/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79797 2023-07-13 19:48:07.000000 mypy-boto3-fsx-1.28.3/mypy_boto3_fsx/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-13 19:48:05.000000 mypy-boto3-fsx-1.28.3/mypy_boto3_fsx/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:49:12.649227 mypy-boto3-fsx-1.28.3/mypy_boto3_fsx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    22284 2023-07-13 19:49:12.000000 mypy-boto3-fsx-1.28.3/mypy_boto3_fsx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-13 19:49:12.000000 mypy-boto3-fsx-1.28.3/mypy_boto3_fsx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 19:49:12.000000 mypy-boto3-fsx-1.28.3/mypy_boto3_fsx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 19:49:12.000000 mypy-boto3-fsx-1.28.3/mypy_boto3_fsx.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-13 19:49:12.000000 mypy-boto3-fsx-1.28.3/mypy_boto3_fsx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-13 19:49:12.000000 mypy-boto3-fsx-1.28.3/mypy_boto3_fsx.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 19:49:12.653227 mypy-boto3-fsx-1.28.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-07-13 19:48:05.000000 mypy-boto3-fsx-1.28.3/setup.py
```

### Comparing `mypy-boto3-fsx-1.28.0/LICENSE` & `mypy-boto3-fsx-1.28.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-fsx-1.28.0/PKG-INFO` & `mypy-boto3-fsx-1.28.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-fsx
-Version: 1.28.0
-Summary: Type annotations for boto3.FSx 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.3
+Summary: Type annotations for boto3.FSx 1.28.3 service generated with mypy-boto3-builder 7.14.6
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-fsx.svg?color=blue)](https://pypi.org/project/mypy-boto3-fsx)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-fsx?color=blue)](https://pypistats.org/packages/mypy-boto3-fsx)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.FSx 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx)
+[boto3.FSx 1.28.3](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx)
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
 [mypy-boto3-fsx docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/).
 
 See how it helps to find and fix potential bugs:
 
@@ -314,14 +314,15 @@
 can be used in user code for type checking.
 
 ```python
 from mypy_boto3_fsx.literals import (
     AdministrativeActionTypeType,
     AliasLifecycleType,
     AutoImportPolicyTypeType,
+    AutocommitPeriodTypeType,
     BackupLifecycleType,
     BackupTypeType,
     DataCompressionTypeType,
     DataRepositoryLifecycleType,
     DataRepositoryTaskFilterNameType,
     DataRepositoryTaskLifecycleType,
     DataRepositoryTaskTypeType,
@@ -349,19 +350,22 @@
     NfsVersionType,
     OntapDeploymentTypeType,
     OntapVolumeTypeType,
     OpenZFSCopyStrategyType,
     OpenZFSDataCompressionTypeType,
     OpenZFSDeploymentTypeType,
     OpenZFSQuotaTypeType,
+    PrivilegedDeleteType,
     ReportFormatType,
     ReportScopeType,
     ResourceTypeType,
     RestoreOpenZFSVolumeOptionType,
+    RetentionPeriodTypeType,
     SecurityStyleType,
+    SnaplockTypeType,
     SnapshotFilterNameType,
     SnapshotLifecycleType,
     StatusType,
     StorageTypeType,
     StorageVirtualMachineFilterNameType,
     StorageVirtualMachineLifecycleType,
     StorageVirtualMachineRootVolumeSecurityStyleType,
@@ -395,14 +399,15 @@
 from mypy_boto3_fsx.type_defs import (
     ActiveDirectoryBackupAttributesTypeDef,
     AdministrativeActionFailureDetailsTypeDef,
     AliasTypeDef,
     AssociateFileSystemAliasesRequestRequestTypeDef,
     AutoExportPolicyTypeDef,
     AutoImportPolicyTypeDef,
+    AutocommitPeriodTypeDef,
     BackupFailureDetailsTypeDef,
     TagTypeDef,
     CancelDataRepositoryTaskRequestRequestTypeDef,
     CancelDataRepositoryTaskResponseTypeDef,
     CompletionReportTypeDef,
     FileCacheLustreMetadataConfigurationTypeDef,
     CreateFileSystemFromBackupResponseTypeDef,
@@ -452,14 +457,15 @@
     OpenZFSOriginSnapshotConfigurationTypeDef,
     PaginatorConfigTypeDef,
     ReleaseFileSystemNfsV3LocksRequestRequestTypeDef,
     ReleaseFileSystemNfsV3LocksResponseTypeDef,
     ResponseMetadataTypeDef,
     RestoreVolumeFromSnapshotRequestRequestTypeDef,
     RestoreVolumeFromSnapshotResponseTypeDef,
+    RetentionPeriodTypeDef,
     SelfManagedActiveDirectoryAttributesTypeDef,
     SelfManagedActiveDirectoryConfigurationUpdatesTypeDef,
     SvmEndpointTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateFileCacheLustreConfigurationTypeDef,
     UpdateFileSystemResponseTypeDef,
     UpdateSnapshotRequestRequestTypeDef,
@@ -488,17 +494,14 @@
     UpdateFileSystemLustreConfigurationTypeDef,
     CreateFileSystemOntapConfigurationTypeDef,
     OpenZFSFileSystemConfigurationTypeDef,
     UpdateFileSystemOntapConfigurationTypeDef,
     UpdateFileSystemOpenZFSConfigurationTypeDef,
     CreateSvmActiveDirectoryConfigurationTypeDef,
     CreateFileSystemWindowsConfigurationTypeDef,
-    CreateOntapVolumeConfigurationTypeDef,
-    OntapVolumeConfigurationTypeDef,
-    UpdateOntapVolumeConfigurationTypeDef,
     DataRepositoryConfigurationTypeDef,
     DescribeDataRepositoryTasksRequestRequestTypeDef,
     DataRepositoryTaskTypeDef,
     DescribeBackupsRequestDescribeBackupsPaginateTypeDef,
     DescribeBackupsRequestRequestTypeDef,
     DescribeDataRepositoryAssociationsRequestRequestTypeDef,
     DescribeSnapshotsRequestRequestTypeDef,
@@ -507,62 +510,69 @@
     DescribeVolumesRequestDescribeVolumesPaginateTypeDef,
     DescribeVolumesRequestRequestTypeDef,
     FileCacheDataRepositoryAssociationTypeDef,
     FileCacheLustreConfigurationTypeDef,
     FileSystemEndpointsTypeDef,
     SnapshotTypeDef,
     OpenZFSNfsExportTypeDef,
+    SnaplockRetentionPeriodTypeDef,
     SvmActiveDirectoryConfigurationTypeDef,
     UpdateFileSystemWindowsConfigurationTypeDef,
     UpdateSvmActiveDirectoryConfigurationTypeDef,
     SvmEndpointsTypeDef,
     UpdateFileCacheRequestRequestTypeDef,
     WindowsFileSystemConfigurationTypeDef,
     CreateDataRepositoryAssociationRequestRequestTypeDef,
     DataRepositoryAssociationTypeDef,
     UpdateDataRepositoryAssociationRequestRequestTypeDef,
     DeleteFileSystemRequestRequestTypeDef,
     DeleteFileSystemResponseTypeDef,
     DeleteVolumeRequestRequestTypeDef,
     DeleteVolumeResponseTypeDef,
     CreateStorageVirtualMachineRequestRequestTypeDef,
-    CreateVolumeFromBackupRequestRequestTypeDef,
     LustreFileSystemConfigurationTypeDef,
     CreateDataRepositoryTaskResponseTypeDef,
     DescribeDataRepositoryTasksResponseTypeDef,
     CreateFileCacheRequestRequestTypeDef,
     FileCacheCreatingTypeDef,
     FileCacheTypeDef,
     OntapFileSystemConfigurationTypeDef,
     CreateSnapshotResponseTypeDef,
     DescribeSnapshotsResponseTypeDef,
     UpdateSnapshotResponseTypeDef,
     CreateOpenZFSVolumeConfigurationTypeDef,
     OpenZFSCreateRootVolumeConfigurationTypeDef,
     OpenZFSVolumeConfigurationTypeDef,
     UpdateOpenZFSVolumeConfigurationTypeDef,
+    CreateSnaplockConfigurationTypeDef,
+    SnaplockConfigurationTypeDef,
+    UpdateSnaplockConfigurationTypeDef,
     UpdateFileSystemRequestRequestTypeDef,
     UpdateStorageVirtualMachineRequestRequestTypeDef,
     StorageVirtualMachineTypeDef,
     CreateDataRepositoryAssociationResponseTypeDef,
     DescribeDataRepositoryAssociationsResponseTypeDef,
     UpdateDataRepositoryAssociationResponseTypeDef,
     CreateFileCacheResponseTypeDef,
     DescribeFileCachesResponseTypeDef,
     UpdateFileCacheResponseTypeDef,
     FileSystemTypeDef,
-    CreateVolumeRequestRequestTypeDef,
     CreateFileSystemOpenZFSConfigurationTypeDef,
-    VolumeTypeDef,
-    UpdateVolumeRequestRequestTypeDef,
+    CreateOntapVolumeConfigurationTypeDef,
+    OntapVolumeConfigurationTypeDef,
+    UpdateOntapVolumeConfigurationTypeDef,
     CreateStorageVirtualMachineResponseTypeDef,
     DescribeStorageVirtualMachinesResponseTypeDef,
     UpdateStorageVirtualMachineResponseTypeDef,
     CreateFileSystemFromBackupRequestRequestTypeDef,
     CreateFileSystemRequestRequestTypeDef,
+    CreateVolumeFromBackupRequestRequestTypeDef,
+    CreateVolumeRequestRequestTypeDef,
+    VolumeTypeDef,
+    UpdateVolumeRequestRequestTypeDef,
     AdministrativeActionTypeDef,
     BackupTypeDef,
     CreateVolumeFromBackupResponseTypeDef,
     CreateVolumeResponseTypeDef,
     DescribeVolumesResponseTypeDef,
     UpdateVolumeResponseTypeDef,
     CopyBackupResponseTypeDef,
```

### Comparing `mypy-boto3-fsx-1.28.0/README.md` & `mypy-boto3-fsx-1.28.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-fsx.svg?color=blue)](https://pypi.org/project/mypy-boto3-fsx)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-fsx?color=blue)](https://pypistats.org/packages/mypy-boto3-fsx)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.FSx 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx)
+[boto3.FSx 1.28.3](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx)
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
 [mypy-boto3-fsx docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/).
 
 See how it helps to find and fix potential bugs:
 
@@ -282,14 +282,15 @@
 can be used in user code for type checking.
 
 ```python
 from mypy_boto3_fsx.literals import (
     AdministrativeActionTypeType,
     AliasLifecycleType,
     AutoImportPolicyTypeType,
+    AutocommitPeriodTypeType,
     BackupLifecycleType,
     BackupTypeType,
     DataCompressionTypeType,
     DataRepositoryLifecycleType,
     DataRepositoryTaskFilterNameType,
     DataRepositoryTaskLifecycleType,
     DataRepositoryTaskTypeType,
@@ -317,19 +318,22 @@
     NfsVersionType,
     OntapDeploymentTypeType,
     OntapVolumeTypeType,
     OpenZFSCopyStrategyType,
     OpenZFSDataCompressionTypeType,
     OpenZFSDeploymentTypeType,
     OpenZFSQuotaTypeType,
+    PrivilegedDeleteType,
     ReportFormatType,
     ReportScopeType,
     ResourceTypeType,
     RestoreOpenZFSVolumeOptionType,
+    RetentionPeriodTypeType,
     SecurityStyleType,
+    SnaplockTypeType,
     SnapshotFilterNameType,
     SnapshotLifecycleType,
     StatusType,
     StorageTypeType,
     StorageVirtualMachineFilterNameType,
     StorageVirtualMachineLifecycleType,
     StorageVirtualMachineRootVolumeSecurityStyleType,
@@ -363,14 +367,15 @@
 from mypy_boto3_fsx.type_defs import (
     ActiveDirectoryBackupAttributesTypeDef,
     AdministrativeActionFailureDetailsTypeDef,
     AliasTypeDef,
     AssociateFileSystemAliasesRequestRequestTypeDef,
     AutoExportPolicyTypeDef,
     AutoImportPolicyTypeDef,
+    AutocommitPeriodTypeDef,
     BackupFailureDetailsTypeDef,
     TagTypeDef,
     CancelDataRepositoryTaskRequestRequestTypeDef,
     CancelDataRepositoryTaskResponseTypeDef,
     CompletionReportTypeDef,
     FileCacheLustreMetadataConfigurationTypeDef,
     CreateFileSystemFromBackupResponseTypeDef,
@@ -420,14 +425,15 @@
     OpenZFSOriginSnapshotConfigurationTypeDef,
     PaginatorConfigTypeDef,
     ReleaseFileSystemNfsV3LocksRequestRequestTypeDef,
     ReleaseFileSystemNfsV3LocksResponseTypeDef,
     ResponseMetadataTypeDef,
     RestoreVolumeFromSnapshotRequestRequestTypeDef,
     RestoreVolumeFromSnapshotResponseTypeDef,
+    RetentionPeriodTypeDef,
     SelfManagedActiveDirectoryAttributesTypeDef,
     SelfManagedActiveDirectoryConfigurationUpdatesTypeDef,
     SvmEndpointTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateFileCacheLustreConfigurationTypeDef,
     UpdateFileSystemResponseTypeDef,
     UpdateSnapshotRequestRequestTypeDef,
@@ -456,17 +462,14 @@
     UpdateFileSystemLustreConfigurationTypeDef,
     CreateFileSystemOntapConfigurationTypeDef,
     OpenZFSFileSystemConfigurationTypeDef,
     UpdateFileSystemOntapConfigurationTypeDef,
     UpdateFileSystemOpenZFSConfigurationTypeDef,
     CreateSvmActiveDirectoryConfigurationTypeDef,
     CreateFileSystemWindowsConfigurationTypeDef,
-    CreateOntapVolumeConfigurationTypeDef,
-    OntapVolumeConfigurationTypeDef,
-    UpdateOntapVolumeConfigurationTypeDef,
     DataRepositoryConfigurationTypeDef,
     DescribeDataRepositoryTasksRequestRequestTypeDef,
     DataRepositoryTaskTypeDef,
     DescribeBackupsRequestDescribeBackupsPaginateTypeDef,
     DescribeBackupsRequestRequestTypeDef,
     DescribeDataRepositoryAssociationsRequestRequestTypeDef,
     DescribeSnapshotsRequestRequestTypeDef,
@@ -475,62 +478,69 @@
     DescribeVolumesRequestDescribeVolumesPaginateTypeDef,
     DescribeVolumesRequestRequestTypeDef,
     FileCacheDataRepositoryAssociationTypeDef,
     FileCacheLustreConfigurationTypeDef,
     FileSystemEndpointsTypeDef,
     SnapshotTypeDef,
     OpenZFSNfsExportTypeDef,
+    SnaplockRetentionPeriodTypeDef,
     SvmActiveDirectoryConfigurationTypeDef,
     UpdateFileSystemWindowsConfigurationTypeDef,
     UpdateSvmActiveDirectoryConfigurationTypeDef,
     SvmEndpointsTypeDef,
     UpdateFileCacheRequestRequestTypeDef,
     WindowsFileSystemConfigurationTypeDef,
     CreateDataRepositoryAssociationRequestRequestTypeDef,
     DataRepositoryAssociationTypeDef,
     UpdateDataRepositoryAssociationRequestRequestTypeDef,
     DeleteFileSystemRequestRequestTypeDef,
     DeleteFileSystemResponseTypeDef,
     DeleteVolumeRequestRequestTypeDef,
     DeleteVolumeResponseTypeDef,
     CreateStorageVirtualMachineRequestRequestTypeDef,
-    CreateVolumeFromBackupRequestRequestTypeDef,
     LustreFileSystemConfigurationTypeDef,
     CreateDataRepositoryTaskResponseTypeDef,
     DescribeDataRepositoryTasksResponseTypeDef,
     CreateFileCacheRequestRequestTypeDef,
     FileCacheCreatingTypeDef,
     FileCacheTypeDef,
     OntapFileSystemConfigurationTypeDef,
     CreateSnapshotResponseTypeDef,
     DescribeSnapshotsResponseTypeDef,
     UpdateSnapshotResponseTypeDef,
     CreateOpenZFSVolumeConfigurationTypeDef,
     OpenZFSCreateRootVolumeConfigurationTypeDef,
     OpenZFSVolumeConfigurationTypeDef,
     UpdateOpenZFSVolumeConfigurationTypeDef,
+    CreateSnaplockConfigurationTypeDef,
+    SnaplockConfigurationTypeDef,
+    UpdateSnaplockConfigurationTypeDef,
     UpdateFileSystemRequestRequestTypeDef,
     UpdateStorageVirtualMachineRequestRequestTypeDef,
     StorageVirtualMachineTypeDef,
     CreateDataRepositoryAssociationResponseTypeDef,
     DescribeDataRepositoryAssociationsResponseTypeDef,
     UpdateDataRepositoryAssociationResponseTypeDef,
     CreateFileCacheResponseTypeDef,
     DescribeFileCachesResponseTypeDef,
     UpdateFileCacheResponseTypeDef,
     FileSystemTypeDef,
-    CreateVolumeRequestRequestTypeDef,
     CreateFileSystemOpenZFSConfigurationTypeDef,
-    VolumeTypeDef,
-    UpdateVolumeRequestRequestTypeDef,
+    CreateOntapVolumeConfigurationTypeDef,
+    OntapVolumeConfigurationTypeDef,
+    UpdateOntapVolumeConfigurationTypeDef,
     CreateStorageVirtualMachineResponseTypeDef,
     DescribeStorageVirtualMachinesResponseTypeDef,
     UpdateStorageVirtualMachineResponseTypeDef,
     CreateFileSystemFromBackupRequestRequestTypeDef,
     CreateFileSystemRequestRequestTypeDef,
+    CreateVolumeFromBackupRequestRequestTypeDef,
+    CreateVolumeRequestRequestTypeDef,
+    VolumeTypeDef,
+    UpdateVolumeRequestRequestTypeDef,
     AdministrativeActionTypeDef,
     BackupTypeDef,
     CreateVolumeFromBackupResponseTypeDef,
     CreateVolumeResponseTypeDef,
     DescribeVolumesResponseTypeDef,
     UpdateVolumeResponseTypeDef,
     CopyBackupResponseTypeDef,
```

### Comparing `mypy-boto3-fsx-1.28.0/mypy_boto3_fsx/__init__.py` & `mypy-boto3-fsx-1.28.3/mypy_boto3_fsx/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-fsx-1.28.0/mypy_boto3_fsx/__init__.pyi` & `mypy-boto3-fsx-1.28.3/mypy_boto3_fsx/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-fsx-1.28.0/mypy_boto3_fsx/__main__.py` & `mypy-boto3-fsx-1.28.3/mypy_boto3_fsx/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.FSx 1.28.0\nVersion:         1.28.0\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.FSx 1.28.3\nVersion:         1.28.3\nBuilder version:"
+        " 7.14.6\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx\nOther"
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

### Comparing `mypy-boto3-fsx-1.28.0/mypy_boto3_fsx/client.py` & `mypy-boto3-fsx-1.28.3/mypy_boto3_fsx/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-fsx-1.28.0/mypy_boto3_fsx/client.pyi` & `mypy-boto3-fsx-1.28.3/mypy_boto3_fsx/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-fsx-1.28.0/mypy_boto3_fsx/literals.py` & `mypy-boto3-fsx-1.28.3/mypy_boto3_fsx/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,15 @@
     from typing_extensions import Literal
 
 
 __all__ = (
     "AdministrativeActionTypeType",
     "AliasLifecycleType",
     "AutoImportPolicyTypeType",
+    "AutocommitPeriodTypeType",
     "BackupLifecycleType",
     "BackupTypeType",
     "DataCompressionTypeType",
     "DataRepositoryLifecycleType",
     "DataRepositoryTaskFilterNameType",
     "DataRepositoryTaskLifecycleType",
     "DataRepositoryTaskTypeType",
@@ -54,19 +55,22 @@
     "NfsVersionType",
     "OntapDeploymentTypeType",
     "OntapVolumeTypeType",
     "OpenZFSCopyStrategyType",
     "OpenZFSDataCompressionTypeType",
     "OpenZFSDeploymentTypeType",
     "OpenZFSQuotaTypeType",
+    "PrivilegedDeleteType",
     "ReportFormatType",
     "ReportScopeType",
     "ResourceTypeType",
     "RestoreOpenZFSVolumeOptionType",
+    "RetentionPeriodTypeType",
     "SecurityStyleType",
+    "SnaplockTypeType",
     "SnapshotFilterNameType",
     "SnapshotLifecycleType",
     "StatusType",
     "StorageTypeType",
     "StorageVirtualMachineFilterNameType",
     "StorageVirtualMachineLifecycleType",
     "StorageVirtualMachineRootVolumeSecurityStyleType",
@@ -93,14 +97,15 @@
     "SNAPSHOT_UPDATE",
     "STORAGE_OPTIMIZATION",
     "VOLUME_RESTORE",
     "VOLUME_UPDATE",
 ]
 AliasLifecycleType = Literal["AVAILABLE", "CREATE_FAILED", "CREATING", "DELETE_FAILED", "DELETING"]
 AutoImportPolicyTypeType = Literal["NEW", "NEW_CHANGED", "NEW_CHANGED_DELETED", "NONE"]
+AutocommitPeriodTypeType = Literal["DAYS", "HOURS", "MINUTES", "MONTHS", "NONE", "YEARS"]
 BackupLifecycleType = Literal[
     "AVAILABLE", "COPYING", "CREATING", "DELETED", "FAILED", "PENDING", "TRANSFERRING"
 ]
 BackupTypeType = Literal["AUTOMATIC", "AWS_BACKUP", "USER_INITIATED"]
 DataCompressionTypeType = Literal["LZ4", "NONE"]
 DataRepositoryLifecycleType = Literal[
     "AVAILABLE", "CREATING", "DELETING", "FAILED", "MISCONFIGURED", "UPDATING"
@@ -157,19 +162,24 @@
 NfsVersionType = Literal["NFS3"]
 OntapDeploymentTypeType = Literal["MULTI_AZ_1", "SINGLE_AZ_1"]
 OntapVolumeTypeType = Literal["DP", "LS", "RW"]
 OpenZFSCopyStrategyType = Literal["CLONE", "FULL_COPY"]
 OpenZFSDataCompressionTypeType = Literal["LZ4", "NONE", "ZSTD"]
 OpenZFSDeploymentTypeType = Literal["SINGLE_AZ_1", "SINGLE_AZ_2"]
 OpenZFSQuotaTypeType = Literal["GROUP", "USER"]
+PrivilegedDeleteType = Literal["DISABLED", "ENABLED", "PERMANENTLY_DISABLED"]
 ReportFormatType = Literal["REPORT_CSV_20191124"]
 ReportScopeType = Literal["FAILED_FILES_ONLY"]
 ResourceTypeType = Literal["FILE_SYSTEM", "VOLUME"]
 RestoreOpenZFSVolumeOptionType = Literal["DELETE_CLONED_VOLUMES", "DELETE_INTERMEDIATE_SNAPSHOTS"]
+RetentionPeriodTypeType = Literal[
+    "DAYS", "HOURS", "INFINITE", "MINUTES", "MONTHS", "SECONDS", "UNSPECIFIED", "YEARS"
+]
 SecurityStyleType = Literal["MIXED", "NTFS", "UNIX"]
+SnaplockTypeType = Literal["COMPLIANCE", "ENTERPRISE"]
 SnapshotFilterNameType = Literal["file-system-id", "volume-id"]
 SnapshotLifecycleType = Literal["AVAILABLE", "CREATING", "DELETING", "PENDING"]
 StatusType = Literal["COMPLETED", "FAILED", "IN_PROGRESS", "PENDING", "UPDATED_OPTIMIZING"]
 StorageTypeType = Literal["HDD", "SSD"]
 StorageVirtualMachineFilterNameType = Literal["file-system-id"]
 StorageVirtualMachineLifecycleType = Literal[
     "CREATED", "CREATING", "DELETING", "FAILED", "MISCONFIGURED", "PENDING"
```

### Comparing `mypy-boto3-fsx-1.28.0/mypy_boto3_fsx/literals.pyi` & `mypy-boto3-fsx-1.28.3/mypy_boto3_fsx/literals.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 else:
     from typing_extensions import Literal
 
 __all__ = (
     "AdministrativeActionTypeType",
     "AliasLifecycleType",
     "AutoImportPolicyTypeType",
+    "AutocommitPeriodTypeType",
     "BackupLifecycleType",
     "BackupTypeType",
     "DataCompressionTypeType",
     "DataRepositoryLifecycleType",
     "DataRepositoryTaskFilterNameType",
     "DataRepositoryTaskLifecycleType",
     "DataRepositoryTaskTypeType",
@@ -53,19 +54,22 @@
     "NfsVersionType",
     "OntapDeploymentTypeType",
     "OntapVolumeTypeType",
     "OpenZFSCopyStrategyType",
     "OpenZFSDataCompressionTypeType",
     "OpenZFSDeploymentTypeType",
     "OpenZFSQuotaTypeType",
+    "PrivilegedDeleteType",
     "ReportFormatType",
     "ReportScopeType",
     "ResourceTypeType",
     "RestoreOpenZFSVolumeOptionType",
+    "RetentionPeriodTypeType",
     "SecurityStyleType",
+    "SnaplockTypeType",
     "SnapshotFilterNameType",
     "SnapshotLifecycleType",
     "StatusType",
     "StorageTypeType",
     "StorageVirtualMachineFilterNameType",
     "StorageVirtualMachineLifecycleType",
     "StorageVirtualMachineRootVolumeSecurityStyleType",
@@ -91,14 +95,15 @@
     "SNAPSHOT_UPDATE",
     "STORAGE_OPTIMIZATION",
     "VOLUME_RESTORE",
     "VOLUME_UPDATE",
 ]
 AliasLifecycleType = Literal["AVAILABLE", "CREATE_FAILED", "CREATING", "DELETE_FAILED", "DELETING"]
 AutoImportPolicyTypeType = Literal["NEW", "NEW_CHANGED", "NEW_CHANGED_DELETED", "NONE"]
+AutocommitPeriodTypeType = Literal["DAYS", "HOURS", "MINUTES", "MONTHS", "NONE", "YEARS"]
 BackupLifecycleType = Literal[
     "AVAILABLE", "COPYING", "CREATING", "DELETED", "FAILED", "PENDING", "TRANSFERRING"
 ]
 BackupTypeType = Literal["AUTOMATIC", "AWS_BACKUP", "USER_INITIATED"]
 DataCompressionTypeType = Literal["LZ4", "NONE"]
 DataRepositoryLifecycleType = Literal[
     "AVAILABLE", "CREATING", "DELETING", "FAILED", "MISCONFIGURED", "UPDATING"
@@ -155,19 +160,24 @@
 NfsVersionType = Literal["NFS3"]
 OntapDeploymentTypeType = Literal["MULTI_AZ_1", "SINGLE_AZ_1"]
 OntapVolumeTypeType = Literal["DP", "LS", "RW"]
 OpenZFSCopyStrategyType = Literal["CLONE", "FULL_COPY"]
 OpenZFSDataCompressionTypeType = Literal["LZ4", "NONE", "ZSTD"]
 OpenZFSDeploymentTypeType = Literal["SINGLE_AZ_1", "SINGLE_AZ_2"]
 OpenZFSQuotaTypeType = Literal["GROUP", "USER"]
+PrivilegedDeleteType = Literal["DISABLED", "ENABLED", "PERMANENTLY_DISABLED"]
 ReportFormatType = Literal["REPORT_CSV_20191124"]
 ReportScopeType = Literal["FAILED_FILES_ONLY"]
 ResourceTypeType = Literal["FILE_SYSTEM", "VOLUME"]
 RestoreOpenZFSVolumeOptionType = Literal["DELETE_CLONED_VOLUMES", "DELETE_INTERMEDIATE_SNAPSHOTS"]
+RetentionPeriodTypeType = Literal[
+    "DAYS", "HOURS", "INFINITE", "MINUTES", "MONTHS", "SECONDS", "UNSPECIFIED", "YEARS"
+]
 SecurityStyleType = Literal["MIXED", "NTFS", "UNIX"]
+SnaplockTypeType = Literal["COMPLIANCE", "ENTERPRISE"]
 SnapshotFilterNameType = Literal["file-system-id", "volume-id"]
 SnapshotLifecycleType = Literal["AVAILABLE", "CREATING", "DELETING", "PENDING"]
 StatusType = Literal["COMPLETED", "FAILED", "IN_PROGRESS", "PENDING", "UPDATED_OPTIMIZING"]
 StorageTypeType = Literal["HDD", "SSD"]
 StorageVirtualMachineFilterNameType = Literal["file-system-id"]
 StorageVirtualMachineLifecycleType = Literal[
     "CREATED", "CREATING", "DELETING", "FAILED", "MISCONFIGURED", "PENDING"
```

### Comparing `mypy-boto3-fsx-1.28.0/mypy_boto3_fsx/paginator.py` & `mypy-boto3-fsx-1.28.3/mypy_boto3_fsx/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-fsx-1.28.0/mypy_boto3_fsx/paginator.pyi` & `mypy-boto3-fsx-1.28.3/mypy_boto3_fsx/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-fsx-1.28.0/mypy_boto3_fsx/type_defs.py` & `mypy-boto3-fsx-1.28.3/mypy_boto3_fsx/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 import sys
 from datetime import datetime
 from typing import Any, Dict, List, Sequence
 
 from .literals import (
     AdministrativeActionTypeType,
     AliasLifecycleType,
+    AutocommitPeriodTypeType,
     AutoImportPolicyTypeType,
     BackupLifecycleType,
     BackupTypeType,
     DataCompressionTypeType,
     DataRepositoryLifecycleType,
     DataRepositoryTaskFilterNameType,
     DataRepositoryTaskLifecycleType,
@@ -40,17 +41,20 @@
     LustreDeploymentTypeType,
     OntapDeploymentTypeType,
     OntapVolumeTypeType,
     OpenZFSCopyStrategyType,
     OpenZFSDataCompressionTypeType,
     OpenZFSDeploymentTypeType,
     OpenZFSQuotaTypeType,
+    PrivilegedDeleteType,
     ResourceTypeType,
     RestoreOpenZFSVolumeOptionType,
+    RetentionPeriodTypeType,
     SecurityStyleType,
+    SnaplockTypeType,
     SnapshotFilterNameType,
     SnapshotLifecycleType,
     StatusType,
     StorageTypeType,
     StorageVirtualMachineLifecycleType,
     StorageVirtualMachineRootVolumeSecurityStyleType,
     StorageVirtualMachineSubtypeType,
@@ -75,14 +79,15 @@
 __all__ = (
     "ActiveDirectoryBackupAttributesTypeDef",
     "AdministrativeActionFailureDetailsTypeDef",
     "AliasTypeDef",
     "AssociateFileSystemAliasesRequestRequestTypeDef",
     "AutoExportPolicyTypeDef",
     "AutoImportPolicyTypeDef",
+    "AutocommitPeriodTypeDef",
     "BackupFailureDetailsTypeDef",
     "TagTypeDef",
     "CancelDataRepositoryTaskRequestRequestTypeDef",
     "CancelDataRepositoryTaskResponseTypeDef",
     "CompletionReportTypeDef",
     "FileCacheLustreMetadataConfigurationTypeDef",
     "CreateFileSystemFromBackupResponseTypeDef",
@@ -132,14 +137,15 @@
     "OpenZFSOriginSnapshotConfigurationTypeDef",
     "PaginatorConfigTypeDef",
     "ReleaseFileSystemNfsV3LocksRequestRequestTypeDef",
     "ReleaseFileSystemNfsV3LocksResponseTypeDef",
     "ResponseMetadataTypeDef",
     "RestoreVolumeFromSnapshotRequestRequestTypeDef",
     "RestoreVolumeFromSnapshotResponseTypeDef",
+    "RetentionPeriodTypeDef",
     "SelfManagedActiveDirectoryAttributesTypeDef",
     "SelfManagedActiveDirectoryConfigurationUpdatesTypeDef",
     "SvmEndpointTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateFileCacheLustreConfigurationTypeDef",
     "UpdateFileSystemResponseTypeDef",
     "UpdateSnapshotRequestRequestTypeDef",
@@ -168,17 +174,14 @@
     "UpdateFileSystemLustreConfigurationTypeDef",
     "CreateFileSystemOntapConfigurationTypeDef",
     "OpenZFSFileSystemConfigurationTypeDef",
     "UpdateFileSystemOntapConfigurationTypeDef",
     "UpdateFileSystemOpenZFSConfigurationTypeDef",
     "CreateSvmActiveDirectoryConfigurationTypeDef",
     "CreateFileSystemWindowsConfigurationTypeDef",
-    "CreateOntapVolumeConfigurationTypeDef",
-    "OntapVolumeConfigurationTypeDef",
-    "UpdateOntapVolumeConfigurationTypeDef",
     "DataRepositoryConfigurationTypeDef",
     "DescribeDataRepositoryTasksRequestRequestTypeDef",
     "DataRepositoryTaskTypeDef",
     "DescribeBackupsRequestDescribeBackupsPaginateTypeDef",
     "DescribeBackupsRequestRequestTypeDef",
     "DescribeDataRepositoryAssociationsRequestRequestTypeDef",
     "DescribeSnapshotsRequestRequestTypeDef",
@@ -187,62 +190,69 @@
     "DescribeVolumesRequestDescribeVolumesPaginateTypeDef",
     "DescribeVolumesRequestRequestTypeDef",
     "FileCacheDataRepositoryAssociationTypeDef",
     "FileCacheLustreConfigurationTypeDef",
     "FileSystemEndpointsTypeDef",
     "SnapshotTypeDef",
     "OpenZFSNfsExportTypeDef",
+    "SnaplockRetentionPeriodTypeDef",
     "SvmActiveDirectoryConfigurationTypeDef",
     "UpdateFileSystemWindowsConfigurationTypeDef",
     "UpdateSvmActiveDirectoryConfigurationTypeDef",
     "SvmEndpointsTypeDef",
     "UpdateFileCacheRequestRequestTypeDef",
     "WindowsFileSystemConfigurationTypeDef",
     "CreateDataRepositoryAssociationRequestRequestTypeDef",
     "DataRepositoryAssociationTypeDef",
     "UpdateDataRepositoryAssociationRequestRequestTypeDef",
     "DeleteFileSystemRequestRequestTypeDef",
     "DeleteFileSystemResponseTypeDef",
     "DeleteVolumeRequestRequestTypeDef",
     "DeleteVolumeResponseTypeDef",
     "CreateStorageVirtualMachineRequestRequestTypeDef",
-    "CreateVolumeFromBackupRequestRequestTypeDef",
     "LustreFileSystemConfigurationTypeDef",
     "CreateDataRepositoryTaskResponseTypeDef",
     "DescribeDataRepositoryTasksResponseTypeDef",
     "CreateFileCacheRequestRequestTypeDef",
     "FileCacheCreatingTypeDef",
     "FileCacheTypeDef",
     "OntapFileSystemConfigurationTypeDef",
     "CreateSnapshotResponseTypeDef",
     "DescribeSnapshotsResponseTypeDef",
     "UpdateSnapshotResponseTypeDef",
     "CreateOpenZFSVolumeConfigurationTypeDef",
     "OpenZFSCreateRootVolumeConfigurationTypeDef",
     "OpenZFSVolumeConfigurationTypeDef",
     "UpdateOpenZFSVolumeConfigurationTypeDef",
+    "CreateSnaplockConfigurationTypeDef",
+    "SnaplockConfigurationTypeDef",
+    "UpdateSnaplockConfigurationTypeDef",
     "UpdateFileSystemRequestRequestTypeDef",
     "UpdateStorageVirtualMachineRequestRequestTypeDef",
     "StorageVirtualMachineTypeDef",
     "CreateDataRepositoryAssociationResponseTypeDef",
     "DescribeDataRepositoryAssociationsResponseTypeDef",
     "UpdateDataRepositoryAssociationResponseTypeDef",
     "CreateFileCacheResponseTypeDef",
     "DescribeFileCachesResponseTypeDef",
     "UpdateFileCacheResponseTypeDef",
     "FileSystemTypeDef",
-    "CreateVolumeRequestRequestTypeDef",
     "CreateFileSystemOpenZFSConfigurationTypeDef",
-    "VolumeTypeDef",
-    "UpdateVolumeRequestRequestTypeDef",
+    "CreateOntapVolumeConfigurationTypeDef",
+    "OntapVolumeConfigurationTypeDef",
+    "UpdateOntapVolumeConfigurationTypeDef",
     "CreateStorageVirtualMachineResponseTypeDef",
     "DescribeStorageVirtualMachinesResponseTypeDef",
     "UpdateStorageVirtualMachineResponseTypeDef",
     "CreateFileSystemFromBackupRequestRequestTypeDef",
     "CreateFileSystemRequestRequestTypeDef",
+    "CreateVolumeFromBackupRequestRequestTypeDef",
+    "CreateVolumeRequestRequestTypeDef",
+    "VolumeTypeDef",
+    "UpdateVolumeRequestRequestTypeDef",
     "AdministrativeActionTypeDef",
     "BackupTypeDef",
     "CreateVolumeFromBackupResponseTypeDef",
     "CreateVolumeResponseTypeDef",
     "DescribeVolumesResponseTypeDef",
     "UpdateVolumeResponseTypeDef",
     "CopyBackupResponseTypeDef",
@@ -253,32 +263,29 @@
 ActiveDirectoryBackupAttributesTypeDef = TypedDict(
     "ActiveDirectoryBackupAttributesTypeDef",
     {
         "DomainName": str,
         "ActiveDirectoryId": str,
         "ResourceARN": str,
     },
-    total=False,
 )
 
 AdministrativeActionFailureDetailsTypeDef = TypedDict(
     "AdministrativeActionFailureDetailsTypeDef",
     {
         "Message": str,
     },
-    total=False,
 )
 
 AliasTypeDef = TypedDict(
     "AliasTypeDef",
     {
         "Name": str,
         "Lifecycle": AliasLifecycleType,
     },
-    total=False,
 )
 
 _RequiredAssociateFileSystemAliasesRequestRequestTypeDef = TypedDict(
     "_RequiredAssociateFileSystemAliasesRequestRequestTypeDef",
     {
         "FileSystemId": str,
         "Aliases": Sequence[str],
@@ -312,20 +319,27 @@
     "AutoImportPolicyTypeDef",
     {
         "Events": Sequence[EventTypeType],
     },
     total=False,
 )
 
+AutocommitPeriodTypeDef = TypedDict(
+    "AutocommitPeriodTypeDef",
+    {
+        "Type": AutocommitPeriodTypeType,
+        "Value": int,
+    },
+)
+
 BackupFailureDetailsTypeDef = TypedDict(
     "BackupFailureDetailsTypeDef",
     {
         "Message": str,
     },
-    total=False,
 )
 
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
@@ -407,24 +421,22 @@
 
 LustreRootSquashConfigurationTypeDef = TypedDict(
     "LustreRootSquashConfigurationTypeDef",
     {
         "RootSquash": str,
         "NoSquashNids": List[str],
     },
-    total=False,
 )
 
 DiskIopsConfigurationTypeDef = TypedDict(
     "DiskIopsConfigurationTypeDef",
     {
         "Mode": DiskIopsConfigurationModeType,
         "Iops": int,
     },
-    total=False,
 )
 
 CreateFileSystemResponseTypeDef = TypedDict(
     "CreateFileSystemResponseTypeDef",
     {
         "FileSystem": "FileSystemTypeDef",
         "ResponseMetadata": "ResponseMetadataTypeDef",
@@ -482,15 +494,14 @@
 
 TieringPolicyTypeDef = TypedDict(
     "TieringPolicyTypeDef",
     {
         "CoolingPeriod": int,
         "Name": TieringPolicyNameType,
     },
-    total=False,
 )
 
 CreateOpenZFSOriginSnapshotConfigurationTypeDef = TypedDict(
     "CreateOpenZFSOriginSnapshotConfigurationTypeDef",
     {
         "SnapshotARN": str,
         "CopyStrategy": OpenZFSCopyStrategyType,
@@ -507,23 +518,21 @@
 )
 
 DataRepositoryFailureDetailsTypeDef = TypedDict(
     "DataRepositoryFailureDetailsTypeDef",
     {
         "Message": str,
     },
-    total=False,
 )
 
 DataRepositoryTaskFailureDetailsTypeDef = TypedDict(
     "DataRepositoryTaskFailureDetailsTypeDef",
     {
         "Message": str,
     },
-    total=False,
 )
 
 DataRepositoryTaskFilterTypeDef = TypedDict(
     "DataRepositoryTaskFilterTypeDef",
     {
         "Name": DataRepositoryTaskFilterNameType,
         "Values": Sequence[str],
@@ -536,15 +545,14 @@
     {
         "TotalCount": int,
         "SucceededCount": int,
         "FailedCount": int,
         "LastUpdatedTime": datetime,
         "ReleasedCapacity": int,
     },
-    total=False,
 )
 
 _RequiredDeleteBackupRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteBackupRequestRequestTypeDef",
     {
         "BackupId": str,
     },
@@ -827,15 +835,14 @@
 
 
 FileCacheFailureDetailsTypeDef = TypedDict(
     "FileCacheFailureDetailsTypeDef",
     {
         "Message": str,
     },
-    total=False,
 )
 
 _RequiredFileCacheNFSConfigurationTypeDef = TypedDict(
     "_RequiredFileCacheNFSConfigurationTypeDef",
     {
         "Version": Literal["NFS3"],
     },
@@ -851,58 +858,42 @@
 
 class FileCacheNFSConfigurationTypeDef(
     _RequiredFileCacheNFSConfigurationTypeDef, _OptionalFileCacheNFSConfigurationTypeDef
 ):
     pass
 
 
-_RequiredLustreLogConfigurationTypeDef = TypedDict(
-    "_RequiredLustreLogConfigurationTypeDef",
+LustreLogConfigurationTypeDef = TypedDict(
+    "LustreLogConfigurationTypeDef",
     {
         "Level": LustreAccessAuditLogLevelType,
-    },
-)
-_OptionalLustreLogConfigurationTypeDef = TypedDict(
-    "_OptionalLustreLogConfigurationTypeDef",
-    {
         "Destination": str,
     },
-    total=False,
 )
 
-
-class LustreLogConfigurationTypeDef(
-    _RequiredLustreLogConfigurationTypeDef, _OptionalLustreLogConfigurationTypeDef
-):
-    pass
-
-
 FileSystemEndpointTypeDef = TypedDict(
     "FileSystemEndpointTypeDef",
     {
         "DNSName": str,
         "IpAddresses": List[str],
     },
-    total=False,
 )
 
 FileSystemFailureDetailsTypeDef = TypedDict(
     "FileSystemFailureDetailsTypeDef",
     {
         "Message": str,
     },
-    total=False,
 )
 
 LifecycleTransitionReasonTypeDef = TypedDict(
     "LifecycleTransitionReasonTypeDef",
     {
         "Message": str,
     },
-    total=False,
 )
 
 _RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
     "_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     {
         "ResourceARN": str,
     },
@@ -956,15 +947,14 @@
 
 OpenZFSOriginSnapshotConfigurationTypeDef = TypedDict(
     "OpenZFSOriginSnapshotConfigurationTypeDef",
     {
         "SnapshotARN": str,
         "CopyStrategy": OpenZFSCopyStrategyType,
     },
-    total=False,
 )
 
 PaginatorConfigTypeDef = TypedDict(
     "PaginatorConfigTypeDef",
     {
         "MaxItems": int,
         "PageSize": int,
@@ -1044,24 +1034,31 @@
         "VolumeId": str,
         "Lifecycle": VolumeLifecycleType,
         "AdministrativeActions": List["AdministrativeActionTypeDef"],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+RetentionPeriodTypeDef = TypedDict(
+    "RetentionPeriodTypeDef",
+    {
+        "Type": RetentionPeriodTypeType,
+        "Value": int,
+    },
+)
+
 SelfManagedActiveDirectoryAttributesTypeDef = TypedDict(
     "SelfManagedActiveDirectoryAttributesTypeDef",
     {
         "DomainName": str,
         "OrganizationalUnitDistinguishedName": str,
         "FileSystemAdministratorsGroup": str,
         "UserName": str,
         "DnsIps": List[str],
     },
-    total=False,
 )
 
 SelfManagedActiveDirectoryConfigurationUpdatesTypeDef = TypedDict(
     "SelfManagedActiveDirectoryConfigurationUpdatesTypeDef",
     {
         "UserName": str,
         "Password": str,
@@ -1075,15 +1072,14 @@
 
 SvmEndpointTypeDef = TypedDict(
     "SvmEndpointTypeDef",
     {
         "DNSName": str,
         "IpAddresses": List[str],
     },
-    total=False,
 )
 
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
         "TagKeys": Sequence[str],
@@ -1124,36 +1120,23 @@
 
 class UpdateSnapshotRequestRequestTypeDef(
     _RequiredUpdateSnapshotRequestRequestTypeDef, _OptionalUpdateSnapshotRequestRequestTypeDef
 ):
     pass
 
 
-_RequiredWindowsAuditLogConfigurationTypeDef = TypedDict(
-    "_RequiredWindowsAuditLogConfigurationTypeDef",
+WindowsAuditLogConfigurationTypeDef = TypedDict(
+    "WindowsAuditLogConfigurationTypeDef",
     {
         "FileAccessAuditLogLevel": WindowsAccessAuditLogLevelType,
         "FileShareAccessAuditLogLevel": WindowsAccessAuditLogLevelType,
-    },
-)
-_OptionalWindowsAuditLogConfigurationTypeDef = TypedDict(
-    "_OptionalWindowsAuditLogConfigurationTypeDef",
-    {
         "AuditLogDestination": str,
     },
-    total=False,
 )
 
-
-class WindowsAuditLogConfigurationTypeDef(
-    _RequiredWindowsAuditLogConfigurationTypeDef, _OptionalWindowsAuditLogConfigurationTypeDef
-):
-    pass
-
-
 AssociateFileSystemAliasesResponseTypeDef = TypedDict(
     "AssociateFileSystemAliasesResponseTypeDef",
     {
         "Aliases": List[AliasTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -1171,36 +1154,23 @@
     "DisassociateFileSystemAliasesResponseTypeDef",
     {
         "Aliases": List[AliasTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredNFSDataRepositoryConfigurationTypeDef = TypedDict(
-    "_RequiredNFSDataRepositoryConfigurationTypeDef",
+NFSDataRepositoryConfigurationTypeDef = TypedDict(
+    "NFSDataRepositoryConfigurationTypeDef",
     {
         "Version": Literal["NFS3"],
-    },
-)
-_OptionalNFSDataRepositoryConfigurationTypeDef = TypedDict(
-    "_OptionalNFSDataRepositoryConfigurationTypeDef",
-    {
         "DnsIps": List[str],
         "AutoExportPolicy": AutoExportPolicyTypeDef,
     },
-    total=False,
 )
 
-
-class NFSDataRepositoryConfigurationTypeDef(
-    _RequiredNFSDataRepositoryConfigurationTypeDef, _OptionalNFSDataRepositoryConfigurationTypeDef
-):
-    pass
-
-
 S3DataRepositoryConfigurationTypeDef = TypedDict(
     "S3DataRepositoryConfigurationTypeDef",
     {
         "AutoImportPolicy": AutoImportPolicyTypeDef,
         "AutoExportPolicy": AutoExportPolicyTypeDef,
     },
     total=False,
@@ -1276,15 +1246,14 @@
 
 DeleteFileSystemLustreResponseTypeDef = TypedDict(
     "DeleteFileSystemLustreResponseTypeDef",
     {
         "FinalBackupId": str,
         "FinalBackupTags": List[TagTypeDef],
     },
-    total=False,
 )
 
 DeleteFileSystemOpenZFSConfigurationTypeDef = TypedDict(
     "DeleteFileSystemOpenZFSConfigurationTypeDef",
     {
         "SkipFinalBackup": bool,
         "FinalBackupTags": Sequence[TagTypeDef],
@@ -1295,15 +1264,14 @@
 
 DeleteFileSystemOpenZFSResponseTypeDef = TypedDict(
     "DeleteFileSystemOpenZFSResponseTypeDef",
     {
         "FinalBackupId": str,
         "FinalBackupTags": List[TagTypeDef],
     },
-    total=False,
 )
 
 DeleteFileSystemWindowsConfigurationTypeDef = TypedDict(
     "DeleteFileSystemWindowsConfigurationTypeDef",
     {
         "SkipFinalBackup": bool,
         "FinalBackupTags": Sequence[TagTypeDef],
@@ -1313,33 +1281,32 @@
 
 DeleteFileSystemWindowsResponseTypeDef = TypedDict(
     "DeleteFileSystemWindowsResponseTypeDef",
     {
         "FinalBackupId": str,
         "FinalBackupTags": List[TagTypeDef],
     },
-    total=False,
 )
 
 DeleteVolumeOntapConfigurationTypeDef = TypedDict(
     "DeleteVolumeOntapConfigurationTypeDef",
     {
         "SkipFinalBackup": bool,
         "FinalBackupTags": Sequence[TagTypeDef],
+        "BypassSnaplockEnterpriseRetention": bool,
     },
     total=False,
 )
 
 DeleteVolumeOntapResponseTypeDef = TypedDict(
     "DeleteVolumeOntapResponseTypeDef",
     {
         "FinalBackupId": str,
         "FinalBackupTags": List[TagTypeDef],
     },
-    total=False,
 )
 
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "Tags": List[TagTypeDef],
         "NextToken": str,
@@ -1480,15 +1447,14 @@
         "DailyAutomaticBackupStartTime": str,
         "DeploymentType": OpenZFSDeploymentTypeType,
         "ThroughputCapacity": int,
         "WeeklyMaintenanceStartTime": str,
         "DiskIopsConfiguration": DiskIopsConfigurationTypeDef,
         "RootVolumeId": str,
     },
-    total=False,
 )
 
 UpdateFileSystemOntapConfigurationTypeDef = TypedDict(
     "UpdateFileSystemOntapConfigurationTypeDef",
     {
         "AutomaticBackupRetentionDays": int,
         "DailyAutomaticBackupStartTime": str,
@@ -1565,133 +1531,58 @@
 class CreateFileSystemWindowsConfigurationTypeDef(
     _RequiredCreateFileSystemWindowsConfigurationTypeDef,
     _OptionalCreateFileSystemWindowsConfigurationTypeDef,
 ):
     pass
 
 
-_RequiredCreateOntapVolumeConfigurationTypeDef = TypedDict(
-    "_RequiredCreateOntapVolumeConfigurationTypeDef",
-    {
-        "SizeInMegabytes": int,
-        "StorageVirtualMachineId": str,
-    },
-)
-_OptionalCreateOntapVolumeConfigurationTypeDef = TypedDict(
-    "_OptionalCreateOntapVolumeConfigurationTypeDef",
-    {
-        "JunctionPath": str,
-        "SecurityStyle": SecurityStyleType,
-        "StorageEfficiencyEnabled": bool,
-        "TieringPolicy": TieringPolicyTypeDef,
-        "OntapVolumeType": InputOntapVolumeTypeType,
-        "SnapshotPolicy": str,
-        "CopyTagsToBackups": bool,
-    },
-    total=False,
-)
-
-
-class CreateOntapVolumeConfigurationTypeDef(
-    _RequiredCreateOntapVolumeConfigurationTypeDef, _OptionalCreateOntapVolumeConfigurationTypeDef
-):
-    pass
-
-
-OntapVolumeConfigurationTypeDef = TypedDict(
-    "OntapVolumeConfigurationTypeDef",
-    {
-        "FlexCacheEndpointType": FlexCacheEndpointTypeType,
-        "JunctionPath": str,
-        "SecurityStyle": SecurityStyleType,
-        "SizeInMegabytes": int,
-        "StorageEfficiencyEnabled": bool,
-        "StorageVirtualMachineId": str,
-        "StorageVirtualMachineRoot": bool,
-        "TieringPolicy": TieringPolicyTypeDef,
-        "UUID": str,
-        "OntapVolumeType": OntapVolumeTypeType,
-        "SnapshotPolicy": str,
-        "CopyTagsToBackups": bool,
-    },
-    total=False,
-)
-
-UpdateOntapVolumeConfigurationTypeDef = TypedDict(
-    "UpdateOntapVolumeConfigurationTypeDef",
-    {
-        "JunctionPath": str,
-        "SecurityStyle": SecurityStyleType,
-        "SizeInMegabytes": int,
-        "StorageEfficiencyEnabled": bool,
-        "TieringPolicy": TieringPolicyTypeDef,
-        "SnapshotPolicy": str,
-        "CopyTagsToBackups": bool,
-    },
-    total=False,
-)
-
 DataRepositoryConfigurationTypeDef = TypedDict(
     "DataRepositoryConfigurationTypeDef",
     {
         "Lifecycle": DataRepositoryLifecycleType,
         "ImportPath": str,
         "ExportPath": str,
         "ImportedFileChunkSize": int,
         "AutoImportPolicy": AutoImportPolicyTypeType,
         "FailureDetails": DataRepositoryFailureDetailsTypeDef,
     },
-    total=False,
 )
 
 DescribeDataRepositoryTasksRequestRequestTypeDef = TypedDict(
     "DescribeDataRepositoryTasksRequestRequestTypeDef",
     {
         "TaskIds": Sequence[str],
         "Filters": Sequence[DataRepositoryTaskFilterTypeDef],
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-_RequiredDataRepositoryTaskTypeDef = TypedDict(
-    "_RequiredDataRepositoryTaskTypeDef",
+DataRepositoryTaskTypeDef = TypedDict(
+    "DataRepositoryTaskTypeDef",
     {
         "TaskId": str,
         "Lifecycle": DataRepositoryTaskLifecycleType,
         "Type": DataRepositoryTaskTypeType,
         "CreationTime": datetime,
-    },
-)
-_OptionalDataRepositoryTaskTypeDef = TypedDict(
-    "_OptionalDataRepositoryTaskTypeDef",
-    {
         "StartTime": datetime,
         "EndTime": datetime,
         "ResourceARN": str,
         "Tags": List[TagTypeDef],
         "FileSystemId": str,
         "Paths": List[str],
         "FailureDetails": DataRepositoryTaskFailureDetailsTypeDef,
         "Status": DataRepositoryTaskStatusTypeDef,
         "Report": CompletionReportTypeDef,
         "CapacityToRelease": int,
         "FileCacheId": str,
     },
-    total=False,
 )
 
-
-class DataRepositoryTaskTypeDef(
-    _RequiredDataRepositoryTaskTypeDef, _OptionalDataRepositoryTaskTypeDef
-):
-    pass
-
-
 DescribeBackupsRequestDescribeBackupsPaginateTypeDef = TypedDict(
     "DescribeBackupsRequestDescribeBackupsPaginateTypeDef",
     {
         "BackupIds": Sequence[str],
         "Filters": Sequence[FilterTypeDef],
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
@@ -1803,24 +1694,22 @@
         "PerUnitStorageThroughput": int,
         "DeploymentType": Literal["CACHE_1"],
         "MountName": str,
         "WeeklyMaintenanceStartTime": str,
         "MetadataConfiguration": FileCacheLustreMetadataConfigurationTypeDef,
         "LogConfiguration": LustreLogConfigurationTypeDef,
     },
-    total=False,
 )
 
 FileSystemEndpointsTypeDef = TypedDict(
     "FileSystemEndpointsTypeDef",
     {
         "Intercluster": FileSystemEndpointTypeDef,
         "Management": FileSystemEndpointTypeDef,
     },
-    total=False,
 )
 
 SnapshotTypeDef = TypedDict(
     "SnapshotTypeDef",
     {
         "ResourceARN": str,
         "SnapshotId": str,
@@ -1828,31 +1717,38 @@
         "VolumeId": str,
         "CreationTime": datetime,
         "Lifecycle": SnapshotLifecycleType,
         "LifecycleTransitionReason": LifecycleTransitionReasonTypeDef,
         "Tags": List[TagTypeDef],
         "AdministrativeActions": List["AdministrativeActionTypeDef"],
     },
-    total=False,
 )
 
 OpenZFSNfsExportTypeDef = TypedDict(
     "OpenZFSNfsExportTypeDef",
     {
         "ClientConfigurations": List[OpenZFSClientConfigurationTypeDef],
     },
 )
 
+SnaplockRetentionPeriodTypeDef = TypedDict(
+    "SnaplockRetentionPeriodTypeDef",
+    {
+        "DefaultRetention": RetentionPeriodTypeDef,
+        "MinimumRetention": RetentionPeriodTypeDef,
+        "MaximumRetention": RetentionPeriodTypeDef,
+    },
+)
+
 SvmActiveDirectoryConfigurationTypeDef = TypedDict(
     "SvmActiveDirectoryConfigurationTypeDef",
     {
         "NetBiosName": str,
         "SelfManagedActiveDirectoryConfiguration": SelfManagedActiveDirectoryAttributesTypeDef,
     },
-    total=False,
 )
 
 UpdateFileSystemWindowsConfigurationTypeDef = TypedDict(
     "UpdateFileSystemWindowsConfigurationTypeDef",
     {
         "WeeklyMaintenanceStartTime": str,
         "DailyAutomaticBackupStartTime": str,
@@ -1881,15 +1777,14 @@
     "SvmEndpointsTypeDef",
     {
         "Iscsi": SvmEndpointTypeDef,
         "Management": SvmEndpointTypeDef,
         "Nfs": SvmEndpointTypeDef,
         "Smb": SvmEndpointTypeDef,
     },
-    total=False,
 )
 
 _RequiredUpdateFileCacheRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateFileCacheRequestRequestTypeDef",
     {
         "FileCacheId": str,
     },
@@ -1924,15 +1819,14 @@
         "WeeklyMaintenanceStartTime": str,
         "DailyAutomaticBackupStartTime": str,
         "AutomaticBackupRetentionDays": int,
         "CopyTagsToBackups": bool,
         "Aliases": List[AliasTypeDef],
         "AuditLogConfiguration": WindowsAuditLogConfigurationTypeDef,
     },
-    total=False,
 )
 
 _RequiredCreateDataRepositoryAssociationRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDataRepositoryAssociationRequestRequestTypeDef",
     {
         "FileSystemId": str,
         "DataRepositoryPath": str,
@@ -1975,15 +1869,14 @@
         "Tags": List[TagTypeDef],
         "CreationTime": datetime,
         "FileCacheId": str,
         "FileCachePath": str,
         "DataRepositorySubdirectories": List[str],
         "NFS": NFSDataRepositoryConfigurationTypeDef,
     },
-    total=False,
 )
 
 _RequiredUpdateDataRepositoryAssociationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateDataRepositoryAssociationRequestRequestTypeDef",
     {
         "AssociationId": str,
     },
@@ -2098,39 +1991,14 @@
 class CreateStorageVirtualMachineRequestRequestTypeDef(
     _RequiredCreateStorageVirtualMachineRequestRequestTypeDef,
     _OptionalCreateStorageVirtualMachineRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredCreateVolumeFromBackupRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateVolumeFromBackupRequestRequestTypeDef",
-    {
-        "BackupId": str,
-        "Name": str,
-    },
-)
-_OptionalCreateVolumeFromBackupRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateVolumeFromBackupRequestRequestTypeDef",
-    {
-        "ClientRequestToken": str,
-        "OntapConfiguration": CreateOntapVolumeConfigurationTypeDef,
-        "Tags": Sequence[TagTypeDef],
-    },
-    total=False,
-)
-
-
-class CreateVolumeFromBackupRequestRequestTypeDef(
-    _RequiredCreateVolumeFromBackupRequestRequestTypeDef,
-    _OptionalCreateVolumeFromBackupRequestRequestTypeDef,
-):
-    pass
-
-
 LustreFileSystemConfigurationTypeDef = TypedDict(
     "LustreFileSystemConfigurationTypeDef",
     {
         "WeeklyMaintenanceStartTime": str,
         "DataRepositoryConfiguration": DataRepositoryConfigurationTypeDef,
         "DeploymentType": LustreDeploymentTypeType,
         "PerUnitStorageThroughput": int,
@@ -2139,15 +2007,14 @@
         "AutomaticBackupRetentionDays": int,
         "CopyTagsToBackups": bool,
         "DriveCacheType": DriveCacheTypeType,
         "DataCompressionType": DataCompressionTypeType,
         "LogConfiguration": LustreLogConfigurationTypeDef,
         "RootSquashConfiguration": LustreRootSquashConfigurationTypeDef,
     },
-    total=False,
 )
 
 CreateDataRepositoryTaskResponseTypeDef = TypedDict(
     "CreateDataRepositoryTaskResponseTypeDef",
     {
         "DataRepositoryTask": DataRepositoryTaskTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
@@ -2211,15 +2078,14 @@
         "KmsKeyId": str,
         "ResourceARN": str,
         "Tags": List[TagTypeDef],
         "CopyTagsToDataRepositoryAssociations": bool,
         "LustreConfiguration": FileCacheLustreConfigurationTypeDef,
         "DataRepositoryAssociationIds": List[str],
     },
-    total=False,
 )
 
 FileCacheTypeDef = TypedDict(
     "FileCacheTypeDef",
     {
         "OwnerId": str,
         "CreationTime": datetime,
@@ -2234,15 +2100,14 @@
         "NetworkInterfaceIds": List[str],
         "DNSName": str,
         "KmsKeyId": str,
         "ResourceARN": str,
         "LustreConfiguration": FileCacheLustreConfigurationTypeDef,
         "DataRepositoryAssociationIds": List[str],
     },
-    total=False,
 )
 
 OntapFileSystemConfigurationTypeDef = TypedDict(
     "OntapFileSystemConfigurationTypeDef",
     {
         "AutomaticBackupRetentionDays": int,
         "DailyAutomaticBackupStartTime": str,
@@ -2252,15 +2117,14 @@
         "DiskIopsConfiguration": DiskIopsConfigurationTypeDef,
         "PreferredSubnetId": str,
         "RouteTableIds": List[str],
         "ThroughputCapacity": int,
         "WeeklyMaintenanceStartTime": str,
         "FsxAdminPassword": str,
     },
-    total=False,
 )
 
 CreateSnapshotResponseTypeDef = TypedDict(
     "CreateSnapshotResponseTypeDef",
     {
         "Snapshot": SnapshotTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
@@ -2341,15 +2205,14 @@
         "ReadOnly": bool,
         "NfsExports": List[OpenZFSNfsExportTypeDef],
         "UserAndGroupQuotas": List[OpenZFSUserOrGroupQuotaTypeDef],
         "RestoreToSnapshot": str,
         "DeleteIntermediateSnaphots": bool,
         "DeleteClonedVolumes": bool,
     },
-    total=False,
 )
 
 UpdateOpenZFSVolumeConfigurationTypeDef = TypedDict(
     "UpdateOpenZFSVolumeConfigurationTypeDef",
     {
         "StorageCapacityReservationGiB": int,
         "StorageCapacityQuotaGiB": int,
@@ -2358,14 +2221,63 @@
         "NfsExports": Sequence[OpenZFSNfsExportTypeDef],
         "UserAndGroupQuotas": Sequence[OpenZFSUserOrGroupQuotaTypeDef],
         "ReadOnly": bool,
     },
     total=False,
 )
 
+_RequiredCreateSnaplockConfigurationTypeDef = TypedDict(
+    "_RequiredCreateSnaplockConfigurationTypeDef",
+    {
+        "SnaplockType": SnaplockTypeType,
+    },
+)
+_OptionalCreateSnaplockConfigurationTypeDef = TypedDict(
+    "_OptionalCreateSnaplockConfigurationTypeDef",
+    {
+        "AuditLogVolume": bool,
+        "AutocommitPeriod": AutocommitPeriodTypeDef,
+        "PrivilegedDelete": PrivilegedDeleteType,
+        "RetentionPeriod": SnaplockRetentionPeriodTypeDef,
+        "VolumeAppendModeEnabled": bool,
+    },
+    total=False,
+)
+
+
+class CreateSnaplockConfigurationTypeDef(
+    _RequiredCreateSnaplockConfigurationTypeDef, _OptionalCreateSnaplockConfigurationTypeDef
+):
+    pass
+
+
+SnaplockConfigurationTypeDef = TypedDict(
+    "SnaplockConfigurationTypeDef",
+    {
+        "AuditLogVolume": bool,
+        "AutocommitPeriod": AutocommitPeriodTypeDef,
+        "PrivilegedDelete": PrivilegedDeleteType,
+        "RetentionPeriod": SnaplockRetentionPeriodTypeDef,
+        "SnaplockType": SnaplockTypeType,
+        "VolumeAppendModeEnabled": bool,
+    },
+)
+
+UpdateSnaplockConfigurationTypeDef = TypedDict(
+    "UpdateSnaplockConfigurationTypeDef",
+    {
+        "AuditLogVolume": bool,
+        "AutocommitPeriod": AutocommitPeriodTypeDef,
+        "PrivilegedDelete": PrivilegedDeleteType,
+        "RetentionPeriod": SnaplockRetentionPeriodTypeDef,
+        "VolumeAppendModeEnabled": bool,
+    },
+    total=False,
+)
+
 _RequiredUpdateFileSystemRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateFileSystemRequestRequestTypeDef",
     {
         "FileSystemId": str,
     },
 )
 _OptionalUpdateFileSystemRequestRequestTypeDef = TypedDict(
@@ -2425,15 +2337,14 @@
         "StorageVirtualMachineId": str,
         "Subtype": StorageVirtualMachineSubtypeType,
         "UUID": str,
         "Tags": List[TagTypeDef],
         "LifecycleTransitionReason": LifecycleTransitionReasonTypeDef,
         "RootVolumeSecurityStyle": StorageVirtualMachineRootVolumeSecurityStyleType,
     },
-    total=False,
 )
 
 CreateDataRepositoryAssociationResponseTypeDef = TypedDict(
     "CreateDataRepositoryAssociationResponseTypeDef",
     {
         "Association": DataRepositoryAssociationTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
@@ -2503,42 +2414,16 @@
         "WindowsConfiguration": WindowsFileSystemConfigurationTypeDef,
         "LustreConfiguration": LustreFileSystemConfigurationTypeDef,
         "AdministrativeActions": List["AdministrativeActionTypeDef"],
         "OntapConfiguration": OntapFileSystemConfigurationTypeDef,
         "FileSystemTypeVersion": str,
         "OpenZFSConfiguration": OpenZFSFileSystemConfigurationTypeDef,
     },
-    total=False,
 )
 
-_RequiredCreateVolumeRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateVolumeRequestRequestTypeDef",
-    {
-        "VolumeType": VolumeTypeType,
-        "Name": str,
-    },
-)
-_OptionalCreateVolumeRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateVolumeRequestRequestTypeDef",
-    {
-        "ClientRequestToken": str,
-        "OntapConfiguration": CreateOntapVolumeConfigurationTypeDef,
-        "Tags": Sequence[TagTypeDef],
-        "OpenZFSConfiguration": CreateOpenZFSVolumeConfigurationTypeDef,
-    },
-    total=False,
-)
-
-
-class CreateVolumeRequestRequestTypeDef(
-    _RequiredCreateVolumeRequestRequestTypeDef, _OptionalCreateVolumeRequestRequestTypeDef
-):
-    pass
-
-
 _RequiredCreateFileSystemOpenZFSConfigurationTypeDef = TypedDict(
     "_RequiredCreateFileSystemOpenZFSConfigurationTypeDef",
     {
         "DeploymentType": OpenZFSDeploymentTypeType,
         "ThroughputCapacity": int,
     },
 )
@@ -2560,57 +2445,77 @@
 class CreateFileSystemOpenZFSConfigurationTypeDef(
     _RequiredCreateFileSystemOpenZFSConfigurationTypeDef,
     _OptionalCreateFileSystemOpenZFSConfigurationTypeDef,
 ):
     pass
 
 
-VolumeTypeDef = TypedDict(
-    "VolumeTypeDef",
-    {
-        "CreationTime": datetime,
-        "FileSystemId": str,
-        "Lifecycle": VolumeLifecycleType,
-        "Name": str,
-        "OntapConfiguration": OntapVolumeConfigurationTypeDef,
-        "ResourceARN": str,
-        "Tags": List[TagTypeDef],
-        "VolumeId": str,
-        "VolumeType": VolumeTypeType,
-        "LifecycleTransitionReason": LifecycleTransitionReasonTypeDef,
-        "AdministrativeActions": List[Dict[str, Any]],
-        "OpenZFSConfiguration": OpenZFSVolumeConfigurationTypeDef,
-    },
-    total=False,
-)
-
-_RequiredUpdateVolumeRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateVolumeRequestRequestTypeDef",
+_RequiredCreateOntapVolumeConfigurationTypeDef = TypedDict(
+    "_RequiredCreateOntapVolumeConfigurationTypeDef",
     {
-        "VolumeId": str,
+        "SizeInMegabytes": int,
+        "StorageVirtualMachineId": str,
     },
 )
-_OptionalUpdateVolumeRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateVolumeRequestRequestTypeDef",
+_OptionalCreateOntapVolumeConfigurationTypeDef = TypedDict(
+    "_OptionalCreateOntapVolumeConfigurationTypeDef",
     {
-        "ClientRequestToken": str,
-        "OntapConfiguration": UpdateOntapVolumeConfigurationTypeDef,
-        "Name": str,
-        "OpenZFSConfiguration": UpdateOpenZFSVolumeConfigurationTypeDef,
+        "JunctionPath": str,
+        "SecurityStyle": SecurityStyleType,
+        "StorageEfficiencyEnabled": bool,
+        "TieringPolicy": TieringPolicyTypeDef,
+        "OntapVolumeType": InputOntapVolumeTypeType,
+        "SnapshotPolicy": str,
+        "CopyTagsToBackups": bool,
+        "SnaplockConfiguration": CreateSnaplockConfigurationTypeDef,
     },
     total=False,
 )
 
 
-class UpdateVolumeRequestRequestTypeDef(
-    _RequiredUpdateVolumeRequestRequestTypeDef, _OptionalUpdateVolumeRequestRequestTypeDef
+class CreateOntapVolumeConfigurationTypeDef(
+    _RequiredCreateOntapVolumeConfigurationTypeDef, _OptionalCreateOntapVolumeConfigurationTypeDef
 ):
     pass
 
 
+OntapVolumeConfigurationTypeDef = TypedDict(
+    "OntapVolumeConfigurationTypeDef",
+    {
+        "FlexCacheEndpointType": FlexCacheEndpointTypeType,
+        "JunctionPath": str,
+        "SecurityStyle": SecurityStyleType,
+        "SizeInMegabytes": int,
+        "StorageEfficiencyEnabled": bool,
+        "StorageVirtualMachineId": str,
+        "StorageVirtualMachineRoot": bool,
+        "TieringPolicy": TieringPolicyTypeDef,
+        "UUID": str,
+        "OntapVolumeType": OntapVolumeTypeType,
+        "SnapshotPolicy": str,
+        "CopyTagsToBackups": bool,
+        "SnaplockConfiguration": SnaplockConfigurationTypeDef,
+    },
+)
+
+UpdateOntapVolumeConfigurationTypeDef = TypedDict(
+    "UpdateOntapVolumeConfigurationTypeDef",
+    {
+        "JunctionPath": str,
+        "SecurityStyle": SecurityStyleType,
+        "SizeInMegabytes": int,
+        "StorageEfficiencyEnabled": bool,
+        "TieringPolicy": TieringPolicyTypeDef,
+        "SnapshotPolicy": str,
+        "CopyTagsToBackups": bool,
+        "SnaplockConfiguration": UpdateSnaplockConfigurationTypeDef,
+    },
+    total=False,
+)
+
 CreateStorageVirtualMachineResponseTypeDef = TypedDict(
     "CreateStorageVirtualMachineResponseTypeDef",
     {
         "StorageVirtualMachine": StorageVirtualMachineTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -2692,62 +2597,142 @@
 
 class CreateFileSystemRequestRequestTypeDef(
     _RequiredCreateFileSystemRequestRequestTypeDef, _OptionalCreateFileSystemRequestRequestTypeDef
 ):
     pass
 
 
+_RequiredCreateVolumeFromBackupRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateVolumeFromBackupRequestRequestTypeDef",
+    {
+        "BackupId": str,
+        "Name": str,
+    },
+)
+_OptionalCreateVolumeFromBackupRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateVolumeFromBackupRequestRequestTypeDef",
+    {
+        "ClientRequestToken": str,
+        "OntapConfiguration": CreateOntapVolumeConfigurationTypeDef,
+        "Tags": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
+
+class CreateVolumeFromBackupRequestRequestTypeDef(
+    _RequiredCreateVolumeFromBackupRequestRequestTypeDef,
+    _OptionalCreateVolumeFromBackupRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredCreateVolumeRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateVolumeRequestRequestTypeDef",
+    {
+        "VolumeType": VolumeTypeType,
+        "Name": str,
+    },
+)
+_OptionalCreateVolumeRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateVolumeRequestRequestTypeDef",
+    {
+        "ClientRequestToken": str,
+        "OntapConfiguration": CreateOntapVolumeConfigurationTypeDef,
+        "Tags": Sequence[TagTypeDef],
+        "OpenZFSConfiguration": CreateOpenZFSVolumeConfigurationTypeDef,
+    },
+    total=False,
+)
+
+
+class CreateVolumeRequestRequestTypeDef(
+    _RequiredCreateVolumeRequestRequestTypeDef, _OptionalCreateVolumeRequestRequestTypeDef
+):
+    pass
+
+
+VolumeTypeDef = TypedDict(
+    "VolumeTypeDef",
+    {
+        "CreationTime": datetime,
+        "FileSystemId": str,
+        "Lifecycle": VolumeLifecycleType,
+        "Name": str,
+        "OntapConfiguration": OntapVolumeConfigurationTypeDef,
+        "ResourceARN": str,
+        "Tags": List[TagTypeDef],
+        "VolumeId": str,
+        "VolumeType": VolumeTypeType,
+        "LifecycleTransitionReason": LifecycleTransitionReasonTypeDef,
+        "AdministrativeActions": List[Dict[str, Any]],
+        "OpenZFSConfiguration": OpenZFSVolumeConfigurationTypeDef,
+    },
+)
+
+_RequiredUpdateVolumeRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateVolumeRequestRequestTypeDef",
+    {
+        "VolumeId": str,
+    },
+)
+_OptionalUpdateVolumeRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateVolumeRequestRequestTypeDef",
+    {
+        "ClientRequestToken": str,
+        "OntapConfiguration": UpdateOntapVolumeConfigurationTypeDef,
+        "Name": str,
+        "OpenZFSConfiguration": UpdateOpenZFSVolumeConfigurationTypeDef,
+    },
+    total=False,
+)
+
+
+class UpdateVolumeRequestRequestTypeDef(
+    _RequiredUpdateVolumeRequestRequestTypeDef, _OptionalUpdateVolumeRequestRequestTypeDef
+):
+    pass
+
+
 AdministrativeActionTypeDef = TypedDict(
     "AdministrativeActionTypeDef",
     {
         "AdministrativeActionType": AdministrativeActionTypeType,
         "ProgressPercent": int,
         "RequestTime": datetime,
         "Status": StatusType,
         "TargetFileSystemValues": Dict[str, Any],
         "FailureDetails": AdministrativeActionFailureDetailsTypeDef,
         "TargetVolumeValues": Dict[str, Any],
         "TargetSnapshotValues": Dict[str, Any],
     },
-    total=False,
 )
 
-_RequiredBackupTypeDef = TypedDict(
-    "_RequiredBackupTypeDef",
+BackupTypeDef = TypedDict(
+    "BackupTypeDef",
     {
         "BackupId": str,
         "Lifecycle": BackupLifecycleType,
-        "Type": BackupTypeType,
-        "CreationTime": datetime,
-        "FileSystem": "FileSystemTypeDef",
-    },
-)
-_OptionalBackupTypeDef = TypedDict(
-    "_OptionalBackupTypeDef",
-    {
         "FailureDetails": BackupFailureDetailsTypeDef,
+        "Type": BackupTypeType,
         "ProgressPercent": int,
+        "CreationTime": datetime,
         "KmsKeyId": str,
         "ResourceARN": str,
         "Tags": List[TagTypeDef],
+        "FileSystem": "FileSystemTypeDef",
         "DirectoryInformation": ActiveDirectoryBackupAttributesTypeDef,
         "OwnerId": str,
         "SourceBackupId": str,
         "SourceBackupRegion": str,
         "ResourceType": ResourceTypeType,
         "Volume": VolumeTypeDef,
     },
-    total=False,
 )
 
-
-class BackupTypeDef(_RequiredBackupTypeDef, _OptionalBackupTypeDef):
-    pass
-
-
 CreateVolumeFromBackupResponseTypeDef = TypedDict(
     "CreateVolumeFromBackupResponseTypeDef",
     {
         "Volume": VolumeTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-fsx-1.28.0/mypy_boto3_fsx/type_defs.pyi` & `mypy-boto3-fsx-1.28.3/mypy_boto3_fsx/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 import sys
 from datetime import datetime
 from typing import Any, Dict, List, Sequence
 
 from .literals import (
     AdministrativeActionTypeType,
     AliasLifecycleType,
+    AutocommitPeriodTypeType,
     AutoImportPolicyTypeType,
     BackupLifecycleType,
     BackupTypeType,
     DataCompressionTypeType,
     DataRepositoryLifecycleType,
     DataRepositoryTaskFilterNameType,
     DataRepositoryTaskLifecycleType,
@@ -40,17 +41,20 @@
     LustreDeploymentTypeType,
     OntapDeploymentTypeType,
     OntapVolumeTypeType,
     OpenZFSCopyStrategyType,
     OpenZFSDataCompressionTypeType,
     OpenZFSDeploymentTypeType,
     OpenZFSQuotaTypeType,
+    PrivilegedDeleteType,
     ResourceTypeType,
     RestoreOpenZFSVolumeOptionType,
+    RetentionPeriodTypeType,
     SecurityStyleType,
+    SnaplockTypeType,
     SnapshotFilterNameType,
     SnapshotLifecycleType,
     StatusType,
     StorageTypeType,
     StorageVirtualMachineLifecycleType,
     StorageVirtualMachineRootVolumeSecurityStyleType,
     StorageVirtualMachineSubtypeType,
@@ -74,14 +78,15 @@
 __all__ = (
     "ActiveDirectoryBackupAttributesTypeDef",
     "AdministrativeActionFailureDetailsTypeDef",
     "AliasTypeDef",
     "AssociateFileSystemAliasesRequestRequestTypeDef",
     "AutoExportPolicyTypeDef",
     "AutoImportPolicyTypeDef",
+    "AutocommitPeriodTypeDef",
     "BackupFailureDetailsTypeDef",
     "TagTypeDef",
     "CancelDataRepositoryTaskRequestRequestTypeDef",
     "CancelDataRepositoryTaskResponseTypeDef",
     "CompletionReportTypeDef",
     "FileCacheLustreMetadataConfigurationTypeDef",
     "CreateFileSystemFromBackupResponseTypeDef",
@@ -131,14 +136,15 @@
     "OpenZFSOriginSnapshotConfigurationTypeDef",
     "PaginatorConfigTypeDef",
     "ReleaseFileSystemNfsV3LocksRequestRequestTypeDef",
     "ReleaseFileSystemNfsV3LocksResponseTypeDef",
     "ResponseMetadataTypeDef",
     "RestoreVolumeFromSnapshotRequestRequestTypeDef",
     "RestoreVolumeFromSnapshotResponseTypeDef",
+    "RetentionPeriodTypeDef",
     "SelfManagedActiveDirectoryAttributesTypeDef",
     "SelfManagedActiveDirectoryConfigurationUpdatesTypeDef",
     "SvmEndpointTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateFileCacheLustreConfigurationTypeDef",
     "UpdateFileSystemResponseTypeDef",
     "UpdateSnapshotRequestRequestTypeDef",
@@ -167,17 +173,14 @@
     "UpdateFileSystemLustreConfigurationTypeDef",
     "CreateFileSystemOntapConfigurationTypeDef",
     "OpenZFSFileSystemConfigurationTypeDef",
     "UpdateFileSystemOntapConfigurationTypeDef",
     "UpdateFileSystemOpenZFSConfigurationTypeDef",
     "CreateSvmActiveDirectoryConfigurationTypeDef",
     "CreateFileSystemWindowsConfigurationTypeDef",
-    "CreateOntapVolumeConfigurationTypeDef",
-    "OntapVolumeConfigurationTypeDef",
-    "UpdateOntapVolumeConfigurationTypeDef",
     "DataRepositoryConfigurationTypeDef",
     "DescribeDataRepositoryTasksRequestRequestTypeDef",
     "DataRepositoryTaskTypeDef",
     "DescribeBackupsRequestDescribeBackupsPaginateTypeDef",
     "DescribeBackupsRequestRequestTypeDef",
     "DescribeDataRepositoryAssociationsRequestRequestTypeDef",
     "DescribeSnapshotsRequestRequestTypeDef",
@@ -186,62 +189,69 @@
     "DescribeVolumesRequestDescribeVolumesPaginateTypeDef",
     "DescribeVolumesRequestRequestTypeDef",
     "FileCacheDataRepositoryAssociationTypeDef",
     "FileCacheLustreConfigurationTypeDef",
     "FileSystemEndpointsTypeDef",
     "SnapshotTypeDef",
     "OpenZFSNfsExportTypeDef",
+    "SnaplockRetentionPeriodTypeDef",
     "SvmActiveDirectoryConfigurationTypeDef",
     "UpdateFileSystemWindowsConfigurationTypeDef",
     "UpdateSvmActiveDirectoryConfigurationTypeDef",
     "SvmEndpointsTypeDef",
     "UpdateFileCacheRequestRequestTypeDef",
     "WindowsFileSystemConfigurationTypeDef",
     "CreateDataRepositoryAssociationRequestRequestTypeDef",
     "DataRepositoryAssociationTypeDef",
     "UpdateDataRepositoryAssociationRequestRequestTypeDef",
     "DeleteFileSystemRequestRequestTypeDef",
     "DeleteFileSystemResponseTypeDef",
     "DeleteVolumeRequestRequestTypeDef",
     "DeleteVolumeResponseTypeDef",
     "CreateStorageVirtualMachineRequestRequestTypeDef",
-    "CreateVolumeFromBackupRequestRequestTypeDef",
     "LustreFileSystemConfigurationTypeDef",
     "CreateDataRepositoryTaskResponseTypeDef",
     "DescribeDataRepositoryTasksResponseTypeDef",
     "CreateFileCacheRequestRequestTypeDef",
     "FileCacheCreatingTypeDef",
     "FileCacheTypeDef",
     "OntapFileSystemConfigurationTypeDef",
     "CreateSnapshotResponseTypeDef",
     "DescribeSnapshotsResponseTypeDef",
     "UpdateSnapshotResponseTypeDef",
     "CreateOpenZFSVolumeConfigurationTypeDef",
     "OpenZFSCreateRootVolumeConfigurationTypeDef",
     "OpenZFSVolumeConfigurationTypeDef",
     "UpdateOpenZFSVolumeConfigurationTypeDef",
+    "CreateSnaplockConfigurationTypeDef",
+    "SnaplockConfigurationTypeDef",
+    "UpdateSnaplockConfigurationTypeDef",
     "UpdateFileSystemRequestRequestTypeDef",
     "UpdateStorageVirtualMachineRequestRequestTypeDef",
     "StorageVirtualMachineTypeDef",
     "CreateDataRepositoryAssociationResponseTypeDef",
     "DescribeDataRepositoryAssociationsResponseTypeDef",
     "UpdateDataRepositoryAssociationResponseTypeDef",
     "CreateFileCacheResponseTypeDef",
     "DescribeFileCachesResponseTypeDef",
     "UpdateFileCacheResponseTypeDef",
     "FileSystemTypeDef",
-    "CreateVolumeRequestRequestTypeDef",
     "CreateFileSystemOpenZFSConfigurationTypeDef",
-    "VolumeTypeDef",
-    "UpdateVolumeRequestRequestTypeDef",
+    "CreateOntapVolumeConfigurationTypeDef",
+    "OntapVolumeConfigurationTypeDef",
+    "UpdateOntapVolumeConfigurationTypeDef",
     "CreateStorageVirtualMachineResponseTypeDef",
     "DescribeStorageVirtualMachinesResponseTypeDef",
     "UpdateStorageVirtualMachineResponseTypeDef",
     "CreateFileSystemFromBackupRequestRequestTypeDef",
     "CreateFileSystemRequestRequestTypeDef",
+    "CreateVolumeFromBackupRequestRequestTypeDef",
+    "CreateVolumeRequestRequestTypeDef",
+    "VolumeTypeDef",
+    "UpdateVolumeRequestRequestTypeDef",
     "AdministrativeActionTypeDef",
     "BackupTypeDef",
     "CreateVolumeFromBackupResponseTypeDef",
     "CreateVolumeResponseTypeDef",
     "DescribeVolumesResponseTypeDef",
     "UpdateVolumeResponseTypeDef",
     "CopyBackupResponseTypeDef",
@@ -252,32 +262,29 @@
 ActiveDirectoryBackupAttributesTypeDef = TypedDict(
     "ActiveDirectoryBackupAttributesTypeDef",
     {
         "DomainName": str,
         "ActiveDirectoryId": str,
         "ResourceARN": str,
     },
-    total=False,
 )
 
 AdministrativeActionFailureDetailsTypeDef = TypedDict(
     "AdministrativeActionFailureDetailsTypeDef",
     {
         "Message": str,
     },
-    total=False,
 )
 
 AliasTypeDef = TypedDict(
     "AliasTypeDef",
     {
         "Name": str,
         "Lifecycle": AliasLifecycleType,
     },
-    total=False,
 )
 
 _RequiredAssociateFileSystemAliasesRequestRequestTypeDef = TypedDict(
     "_RequiredAssociateFileSystemAliasesRequestRequestTypeDef",
     {
         "FileSystemId": str,
         "Aliases": Sequence[str],
@@ -309,20 +316,27 @@
     "AutoImportPolicyTypeDef",
     {
         "Events": Sequence[EventTypeType],
     },
     total=False,
 )
 
+AutocommitPeriodTypeDef = TypedDict(
+    "AutocommitPeriodTypeDef",
+    {
+        "Type": AutocommitPeriodTypeType,
+        "Value": int,
+    },
+)
+
 BackupFailureDetailsTypeDef = TypedDict(
     "BackupFailureDetailsTypeDef",
     {
         "Message": str,
     },
-    total=False,
 )
 
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
@@ -400,24 +414,22 @@
 
 LustreRootSquashConfigurationTypeDef = TypedDict(
     "LustreRootSquashConfigurationTypeDef",
     {
         "RootSquash": str,
         "NoSquashNids": List[str],
     },
-    total=False,
 )
 
 DiskIopsConfigurationTypeDef = TypedDict(
     "DiskIopsConfigurationTypeDef",
     {
         "Mode": DiskIopsConfigurationModeType,
         "Iops": int,
     },
-    total=False,
 )
 
 CreateFileSystemResponseTypeDef = TypedDict(
     "CreateFileSystemResponseTypeDef",
     {
         "FileSystem": "FileSystemTypeDef",
         "ResponseMetadata": "ResponseMetadataTypeDef",
@@ -471,15 +483,14 @@
 
 TieringPolicyTypeDef = TypedDict(
     "TieringPolicyTypeDef",
     {
         "CoolingPeriod": int,
         "Name": TieringPolicyNameType,
     },
-    total=False,
 )
 
 CreateOpenZFSOriginSnapshotConfigurationTypeDef = TypedDict(
     "CreateOpenZFSOriginSnapshotConfigurationTypeDef",
     {
         "SnapshotARN": str,
         "CopyStrategy": OpenZFSCopyStrategyType,
@@ -496,23 +507,21 @@
 )
 
 DataRepositoryFailureDetailsTypeDef = TypedDict(
     "DataRepositoryFailureDetailsTypeDef",
     {
         "Message": str,
     },
-    total=False,
 )
 
 DataRepositoryTaskFailureDetailsTypeDef = TypedDict(
     "DataRepositoryTaskFailureDetailsTypeDef",
     {
         "Message": str,
     },
-    total=False,
 )
 
 DataRepositoryTaskFilterTypeDef = TypedDict(
     "DataRepositoryTaskFilterTypeDef",
     {
         "Name": DataRepositoryTaskFilterNameType,
         "Values": Sequence[str],
@@ -525,15 +534,14 @@
     {
         "TotalCount": int,
         "SucceededCount": int,
         "FailedCount": int,
         "LastUpdatedTime": datetime,
         "ReleasedCapacity": int,
     },
-    total=False,
 )
 
 _RequiredDeleteBackupRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteBackupRequestRequestTypeDef",
     {
         "BackupId": str,
     },
@@ -802,15 +810,14 @@
     pass
 
 FileCacheFailureDetailsTypeDef = TypedDict(
     "FileCacheFailureDetailsTypeDef",
     {
         "Message": str,
     },
-    total=False,
 )
 
 _RequiredFileCacheNFSConfigurationTypeDef = TypedDict(
     "_RequiredFileCacheNFSConfigurationTypeDef",
     {
         "Version": Literal["NFS3"],
     },
@@ -824,56 +831,42 @@
 )
 
 class FileCacheNFSConfigurationTypeDef(
     _RequiredFileCacheNFSConfigurationTypeDef, _OptionalFileCacheNFSConfigurationTypeDef
 ):
     pass
 
-_RequiredLustreLogConfigurationTypeDef = TypedDict(
-    "_RequiredLustreLogConfigurationTypeDef",
+LustreLogConfigurationTypeDef = TypedDict(
+    "LustreLogConfigurationTypeDef",
     {
         "Level": LustreAccessAuditLogLevelType,
-    },
-)
-_OptionalLustreLogConfigurationTypeDef = TypedDict(
-    "_OptionalLustreLogConfigurationTypeDef",
-    {
         "Destination": str,
     },
-    total=False,
 )
 
-class LustreLogConfigurationTypeDef(
-    _RequiredLustreLogConfigurationTypeDef, _OptionalLustreLogConfigurationTypeDef
-):
-    pass
-
 FileSystemEndpointTypeDef = TypedDict(
     "FileSystemEndpointTypeDef",
     {
         "DNSName": str,
         "IpAddresses": List[str],
     },
-    total=False,
 )
 
 FileSystemFailureDetailsTypeDef = TypedDict(
     "FileSystemFailureDetailsTypeDef",
     {
         "Message": str,
     },
-    total=False,
 )
 
 LifecycleTransitionReasonTypeDef = TypedDict(
     "LifecycleTransitionReasonTypeDef",
     {
         "Message": str,
     },
-    total=False,
 )
 
 _RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
     "_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     {
         "ResourceARN": str,
     },
@@ -923,15 +916,14 @@
 
 OpenZFSOriginSnapshotConfigurationTypeDef = TypedDict(
     "OpenZFSOriginSnapshotConfigurationTypeDef",
     {
         "SnapshotARN": str,
         "CopyStrategy": OpenZFSCopyStrategyType,
     },
-    total=False,
 )
 
 PaginatorConfigTypeDef = TypedDict(
     "PaginatorConfigTypeDef",
     {
         "MaxItems": int,
         "PageSize": int,
@@ -1007,24 +999,31 @@
         "VolumeId": str,
         "Lifecycle": VolumeLifecycleType,
         "AdministrativeActions": List["AdministrativeActionTypeDef"],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+RetentionPeriodTypeDef = TypedDict(
+    "RetentionPeriodTypeDef",
+    {
+        "Type": RetentionPeriodTypeType,
+        "Value": int,
+    },
+)
+
 SelfManagedActiveDirectoryAttributesTypeDef = TypedDict(
     "SelfManagedActiveDirectoryAttributesTypeDef",
     {
         "DomainName": str,
         "OrganizationalUnitDistinguishedName": str,
         "FileSystemAdministratorsGroup": str,
         "UserName": str,
         "DnsIps": List[str],
     },
-    total=False,
 )
 
 SelfManagedActiveDirectoryConfigurationUpdatesTypeDef = TypedDict(
     "SelfManagedActiveDirectoryConfigurationUpdatesTypeDef",
     {
         "UserName": str,
         "Password": str,
@@ -1038,15 +1037,14 @@
 
 SvmEndpointTypeDef = TypedDict(
     "SvmEndpointTypeDef",
     {
         "DNSName": str,
         "IpAddresses": List[str],
     },
-    total=False,
 )
 
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
         "TagKeys": Sequence[str],
@@ -1085,34 +1083,23 @@
 )
 
 class UpdateSnapshotRequestRequestTypeDef(
     _RequiredUpdateSnapshotRequestRequestTypeDef, _OptionalUpdateSnapshotRequestRequestTypeDef
 ):
     pass
 
-_RequiredWindowsAuditLogConfigurationTypeDef = TypedDict(
-    "_RequiredWindowsAuditLogConfigurationTypeDef",
+WindowsAuditLogConfigurationTypeDef = TypedDict(
+    "WindowsAuditLogConfigurationTypeDef",
     {
         "FileAccessAuditLogLevel": WindowsAccessAuditLogLevelType,
         "FileShareAccessAuditLogLevel": WindowsAccessAuditLogLevelType,
-    },
-)
-_OptionalWindowsAuditLogConfigurationTypeDef = TypedDict(
-    "_OptionalWindowsAuditLogConfigurationTypeDef",
-    {
         "AuditLogDestination": str,
     },
-    total=False,
 )
 
-class WindowsAuditLogConfigurationTypeDef(
-    _RequiredWindowsAuditLogConfigurationTypeDef, _OptionalWindowsAuditLogConfigurationTypeDef
-):
-    pass
-
 AssociateFileSystemAliasesResponseTypeDef = TypedDict(
     "AssociateFileSystemAliasesResponseTypeDef",
     {
         "Aliases": List[AliasTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -1130,34 +1117,23 @@
     "DisassociateFileSystemAliasesResponseTypeDef",
     {
         "Aliases": List[AliasTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredNFSDataRepositoryConfigurationTypeDef = TypedDict(
-    "_RequiredNFSDataRepositoryConfigurationTypeDef",
+NFSDataRepositoryConfigurationTypeDef = TypedDict(
+    "NFSDataRepositoryConfigurationTypeDef",
     {
         "Version": Literal["NFS3"],
-    },
-)
-_OptionalNFSDataRepositoryConfigurationTypeDef = TypedDict(
-    "_OptionalNFSDataRepositoryConfigurationTypeDef",
-    {
         "DnsIps": List[str],
         "AutoExportPolicy": AutoExportPolicyTypeDef,
     },
-    total=False,
 )
 
-class NFSDataRepositoryConfigurationTypeDef(
-    _RequiredNFSDataRepositoryConfigurationTypeDef, _OptionalNFSDataRepositoryConfigurationTypeDef
-):
-    pass
-
 S3DataRepositoryConfigurationTypeDef = TypedDict(
     "S3DataRepositoryConfigurationTypeDef",
     {
         "AutoImportPolicy": AutoImportPolicyTypeDef,
         "AutoExportPolicy": AutoExportPolicyTypeDef,
     },
     total=False,
@@ -1229,15 +1205,14 @@
 
 DeleteFileSystemLustreResponseTypeDef = TypedDict(
     "DeleteFileSystemLustreResponseTypeDef",
     {
         "FinalBackupId": str,
         "FinalBackupTags": List[TagTypeDef],
     },
-    total=False,
 )
 
 DeleteFileSystemOpenZFSConfigurationTypeDef = TypedDict(
     "DeleteFileSystemOpenZFSConfigurationTypeDef",
     {
         "SkipFinalBackup": bool,
         "FinalBackupTags": Sequence[TagTypeDef],
@@ -1248,15 +1223,14 @@
 
 DeleteFileSystemOpenZFSResponseTypeDef = TypedDict(
     "DeleteFileSystemOpenZFSResponseTypeDef",
     {
         "FinalBackupId": str,
         "FinalBackupTags": List[TagTypeDef],
     },
-    total=False,
 )
 
 DeleteFileSystemWindowsConfigurationTypeDef = TypedDict(
     "DeleteFileSystemWindowsConfigurationTypeDef",
     {
         "SkipFinalBackup": bool,
         "FinalBackupTags": Sequence[TagTypeDef],
@@ -1266,33 +1240,32 @@
 
 DeleteFileSystemWindowsResponseTypeDef = TypedDict(
     "DeleteFileSystemWindowsResponseTypeDef",
     {
         "FinalBackupId": str,
         "FinalBackupTags": List[TagTypeDef],
     },
-    total=False,
 )
 
 DeleteVolumeOntapConfigurationTypeDef = TypedDict(
     "DeleteVolumeOntapConfigurationTypeDef",
     {
         "SkipFinalBackup": bool,
         "FinalBackupTags": Sequence[TagTypeDef],
+        "BypassSnaplockEnterpriseRetention": bool,
     },
     total=False,
 )
 
 DeleteVolumeOntapResponseTypeDef = TypedDict(
     "DeleteVolumeOntapResponseTypeDef",
     {
         "FinalBackupId": str,
         "FinalBackupTags": List[TagTypeDef],
     },
-    total=False,
 )
 
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "Tags": List[TagTypeDef],
         "NextToken": str,
@@ -1427,15 +1400,14 @@
         "DailyAutomaticBackupStartTime": str,
         "DeploymentType": OpenZFSDeploymentTypeType,
         "ThroughputCapacity": int,
         "WeeklyMaintenanceStartTime": str,
         "DiskIopsConfiguration": DiskIopsConfigurationTypeDef,
         "RootVolumeId": str,
     },
-    total=False,
 )
 
 UpdateFileSystemOntapConfigurationTypeDef = TypedDict(
     "UpdateFileSystemOntapConfigurationTypeDef",
     {
         "AutomaticBackupRetentionDays": int,
         "DailyAutomaticBackupStartTime": str,
@@ -1508,129 +1480,58 @@
 
 class CreateFileSystemWindowsConfigurationTypeDef(
     _RequiredCreateFileSystemWindowsConfigurationTypeDef,
     _OptionalCreateFileSystemWindowsConfigurationTypeDef,
 ):
     pass
 
-_RequiredCreateOntapVolumeConfigurationTypeDef = TypedDict(
-    "_RequiredCreateOntapVolumeConfigurationTypeDef",
-    {
-        "SizeInMegabytes": int,
-        "StorageVirtualMachineId": str,
-    },
-)
-_OptionalCreateOntapVolumeConfigurationTypeDef = TypedDict(
-    "_OptionalCreateOntapVolumeConfigurationTypeDef",
-    {
-        "JunctionPath": str,
-        "SecurityStyle": SecurityStyleType,
-        "StorageEfficiencyEnabled": bool,
-        "TieringPolicy": TieringPolicyTypeDef,
-        "OntapVolumeType": InputOntapVolumeTypeType,
-        "SnapshotPolicy": str,
-        "CopyTagsToBackups": bool,
-    },
-    total=False,
-)
-
-class CreateOntapVolumeConfigurationTypeDef(
-    _RequiredCreateOntapVolumeConfigurationTypeDef, _OptionalCreateOntapVolumeConfigurationTypeDef
-):
-    pass
-
-OntapVolumeConfigurationTypeDef = TypedDict(
-    "OntapVolumeConfigurationTypeDef",
-    {
-        "FlexCacheEndpointType": FlexCacheEndpointTypeType,
-        "JunctionPath": str,
-        "SecurityStyle": SecurityStyleType,
-        "SizeInMegabytes": int,
-        "StorageEfficiencyEnabled": bool,
-        "StorageVirtualMachineId": str,
-        "StorageVirtualMachineRoot": bool,
-        "TieringPolicy": TieringPolicyTypeDef,
-        "UUID": str,
-        "OntapVolumeType": OntapVolumeTypeType,
-        "SnapshotPolicy": str,
-        "CopyTagsToBackups": bool,
-    },
-    total=False,
-)
-
-UpdateOntapVolumeConfigurationTypeDef = TypedDict(
-    "UpdateOntapVolumeConfigurationTypeDef",
-    {
-        "JunctionPath": str,
-        "SecurityStyle": SecurityStyleType,
-        "SizeInMegabytes": int,
-        "StorageEfficiencyEnabled": bool,
-        "TieringPolicy": TieringPolicyTypeDef,
-        "SnapshotPolicy": str,
-        "CopyTagsToBackups": bool,
-    },
-    total=False,
-)
-
 DataRepositoryConfigurationTypeDef = TypedDict(
     "DataRepositoryConfigurationTypeDef",
     {
         "Lifecycle": DataRepositoryLifecycleType,
         "ImportPath": str,
         "ExportPath": str,
         "ImportedFileChunkSize": int,
         "AutoImportPolicy": AutoImportPolicyTypeType,
         "FailureDetails": DataRepositoryFailureDetailsTypeDef,
     },
-    total=False,
 )
 
 DescribeDataRepositoryTasksRequestRequestTypeDef = TypedDict(
     "DescribeDataRepositoryTasksRequestRequestTypeDef",
     {
         "TaskIds": Sequence[str],
         "Filters": Sequence[DataRepositoryTaskFilterTypeDef],
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-_RequiredDataRepositoryTaskTypeDef = TypedDict(
-    "_RequiredDataRepositoryTaskTypeDef",
+DataRepositoryTaskTypeDef = TypedDict(
+    "DataRepositoryTaskTypeDef",
     {
         "TaskId": str,
         "Lifecycle": DataRepositoryTaskLifecycleType,
         "Type": DataRepositoryTaskTypeType,
         "CreationTime": datetime,
-    },
-)
-_OptionalDataRepositoryTaskTypeDef = TypedDict(
-    "_OptionalDataRepositoryTaskTypeDef",
-    {
         "StartTime": datetime,
         "EndTime": datetime,
         "ResourceARN": str,
         "Tags": List[TagTypeDef],
         "FileSystemId": str,
         "Paths": List[str],
         "FailureDetails": DataRepositoryTaskFailureDetailsTypeDef,
         "Status": DataRepositoryTaskStatusTypeDef,
         "Report": CompletionReportTypeDef,
         "CapacityToRelease": int,
         "FileCacheId": str,
     },
-    total=False,
 )
 
-class DataRepositoryTaskTypeDef(
-    _RequiredDataRepositoryTaskTypeDef, _OptionalDataRepositoryTaskTypeDef
-):
-    pass
-
 DescribeBackupsRequestDescribeBackupsPaginateTypeDef = TypedDict(
     "DescribeBackupsRequestDescribeBackupsPaginateTypeDef",
     {
         "BackupIds": Sequence[str],
         "Filters": Sequence[FilterTypeDef],
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
@@ -1740,24 +1641,22 @@
         "PerUnitStorageThroughput": int,
         "DeploymentType": Literal["CACHE_1"],
         "MountName": str,
         "WeeklyMaintenanceStartTime": str,
         "MetadataConfiguration": FileCacheLustreMetadataConfigurationTypeDef,
         "LogConfiguration": LustreLogConfigurationTypeDef,
     },
-    total=False,
 )
 
 FileSystemEndpointsTypeDef = TypedDict(
     "FileSystemEndpointsTypeDef",
     {
         "Intercluster": FileSystemEndpointTypeDef,
         "Management": FileSystemEndpointTypeDef,
     },
-    total=False,
 )
 
 SnapshotTypeDef = TypedDict(
     "SnapshotTypeDef",
     {
         "ResourceARN": str,
         "SnapshotId": str,
@@ -1765,31 +1664,38 @@
         "VolumeId": str,
         "CreationTime": datetime,
         "Lifecycle": SnapshotLifecycleType,
         "LifecycleTransitionReason": LifecycleTransitionReasonTypeDef,
         "Tags": List[TagTypeDef],
         "AdministrativeActions": List["AdministrativeActionTypeDef"],
     },
-    total=False,
 )
 
 OpenZFSNfsExportTypeDef = TypedDict(
     "OpenZFSNfsExportTypeDef",
     {
         "ClientConfigurations": List[OpenZFSClientConfigurationTypeDef],
     },
 )
 
+SnaplockRetentionPeriodTypeDef = TypedDict(
+    "SnaplockRetentionPeriodTypeDef",
+    {
+        "DefaultRetention": RetentionPeriodTypeDef,
+        "MinimumRetention": RetentionPeriodTypeDef,
+        "MaximumRetention": RetentionPeriodTypeDef,
+    },
+)
+
 SvmActiveDirectoryConfigurationTypeDef = TypedDict(
     "SvmActiveDirectoryConfigurationTypeDef",
     {
         "NetBiosName": str,
         "SelfManagedActiveDirectoryConfiguration": SelfManagedActiveDirectoryAttributesTypeDef,
     },
-    total=False,
 )
 
 UpdateFileSystemWindowsConfigurationTypeDef = TypedDict(
     "UpdateFileSystemWindowsConfigurationTypeDef",
     {
         "WeeklyMaintenanceStartTime": str,
         "DailyAutomaticBackupStartTime": str,
@@ -1818,15 +1724,14 @@
     "SvmEndpointsTypeDef",
     {
         "Iscsi": SvmEndpointTypeDef,
         "Management": SvmEndpointTypeDef,
         "Nfs": SvmEndpointTypeDef,
         "Smb": SvmEndpointTypeDef,
     },
-    total=False,
 )
 
 _RequiredUpdateFileCacheRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateFileCacheRequestRequestTypeDef",
     {
         "FileCacheId": str,
     },
@@ -1859,15 +1764,14 @@
         "WeeklyMaintenanceStartTime": str,
         "DailyAutomaticBackupStartTime": str,
         "AutomaticBackupRetentionDays": int,
         "CopyTagsToBackups": bool,
         "Aliases": List[AliasTypeDef],
         "AuditLogConfiguration": WindowsAuditLogConfigurationTypeDef,
     },
-    total=False,
 )
 
 _RequiredCreateDataRepositoryAssociationRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDataRepositoryAssociationRequestRequestTypeDef",
     {
         "FileSystemId": str,
         "DataRepositoryPath": str,
@@ -1908,15 +1812,14 @@
         "Tags": List[TagTypeDef],
         "CreationTime": datetime,
         "FileCacheId": str,
         "FileCachePath": str,
         "DataRepositorySubdirectories": List[str],
         "NFS": NFSDataRepositoryConfigurationTypeDef,
     },
-    total=False,
 )
 
 _RequiredUpdateDataRepositoryAssociationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateDataRepositoryAssociationRequestRequestTypeDef",
     {
         "AssociationId": str,
     },
@@ -2023,37 +1926,14 @@
 
 class CreateStorageVirtualMachineRequestRequestTypeDef(
     _RequiredCreateStorageVirtualMachineRequestRequestTypeDef,
     _OptionalCreateStorageVirtualMachineRequestRequestTypeDef,
 ):
     pass
 
-_RequiredCreateVolumeFromBackupRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateVolumeFromBackupRequestRequestTypeDef",
-    {
-        "BackupId": str,
-        "Name": str,
-    },
-)
-_OptionalCreateVolumeFromBackupRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateVolumeFromBackupRequestRequestTypeDef",
-    {
-        "ClientRequestToken": str,
-        "OntapConfiguration": CreateOntapVolumeConfigurationTypeDef,
-        "Tags": Sequence[TagTypeDef],
-    },
-    total=False,
-)
-
-class CreateVolumeFromBackupRequestRequestTypeDef(
-    _RequiredCreateVolumeFromBackupRequestRequestTypeDef,
-    _OptionalCreateVolumeFromBackupRequestRequestTypeDef,
-):
-    pass
-
 LustreFileSystemConfigurationTypeDef = TypedDict(
     "LustreFileSystemConfigurationTypeDef",
     {
         "WeeklyMaintenanceStartTime": str,
         "DataRepositoryConfiguration": DataRepositoryConfigurationTypeDef,
         "DeploymentType": LustreDeploymentTypeType,
         "PerUnitStorageThroughput": int,
@@ -2062,15 +1942,14 @@
         "AutomaticBackupRetentionDays": int,
         "CopyTagsToBackups": bool,
         "DriveCacheType": DriveCacheTypeType,
         "DataCompressionType": DataCompressionTypeType,
         "LogConfiguration": LustreLogConfigurationTypeDef,
         "RootSquashConfiguration": LustreRootSquashConfigurationTypeDef,
     },
-    total=False,
 )
 
 CreateDataRepositoryTaskResponseTypeDef = TypedDict(
     "CreateDataRepositoryTaskResponseTypeDef",
     {
         "DataRepositoryTask": DataRepositoryTaskTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
@@ -2132,15 +2011,14 @@
         "KmsKeyId": str,
         "ResourceARN": str,
         "Tags": List[TagTypeDef],
         "CopyTagsToDataRepositoryAssociations": bool,
         "LustreConfiguration": FileCacheLustreConfigurationTypeDef,
         "DataRepositoryAssociationIds": List[str],
     },
-    total=False,
 )
 
 FileCacheTypeDef = TypedDict(
     "FileCacheTypeDef",
     {
         "OwnerId": str,
         "CreationTime": datetime,
@@ -2155,15 +2033,14 @@
         "NetworkInterfaceIds": List[str],
         "DNSName": str,
         "KmsKeyId": str,
         "ResourceARN": str,
         "LustreConfiguration": FileCacheLustreConfigurationTypeDef,
         "DataRepositoryAssociationIds": List[str],
     },
-    total=False,
 )
 
 OntapFileSystemConfigurationTypeDef = TypedDict(
     "OntapFileSystemConfigurationTypeDef",
     {
         "AutomaticBackupRetentionDays": int,
         "DailyAutomaticBackupStartTime": str,
@@ -2173,15 +2050,14 @@
         "DiskIopsConfiguration": DiskIopsConfigurationTypeDef,
         "PreferredSubnetId": str,
         "RouteTableIds": List[str],
         "ThroughputCapacity": int,
         "WeeklyMaintenanceStartTime": str,
         "FsxAdminPassword": str,
     },
-    total=False,
 )
 
 CreateSnapshotResponseTypeDef = TypedDict(
     "CreateSnapshotResponseTypeDef",
     {
         "Snapshot": SnapshotTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
@@ -2260,15 +2136,14 @@
         "ReadOnly": bool,
         "NfsExports": List[OpenZFSNfsExportTypeDef],
         "UserAndGroupQuotas": List[OpenZFSUserOrGroupQuotaTypeDef],
         "RestoreToSnapshot": str,
         "DeleteIntermediateSnaphots": bool,
         "DeleteClonedVolumes": bool,
     },
-    total=False,
 )
 
 UpdateOpenZFSVolumeConfigurationTypeDef = TypedDict(
     "UpdateOpenZFSVolumeConfigurationTypeDef",
     {
         "StorageCapacityReservationGiB": int,
         "StorageCapacityQuotaGiB": int,
@@ -2277,14 +2152,61 @@
         "NfsExports": Sequence[OpenZFSNfsExportTypeDef],
         "UserAndGroupQuotas": Sequence[OpenZFSUserOrGroupQuotaTypeDef],
         "ReadOnly": bool,
     },
     total=False,
 )
 
+_RequiredCreateSnaplockConfigurationTypeDef = TypedDict(
+    "_RequiredCreateSnaplockConfigurationTypeDef",
+    {
+        "SnaplockType": SnaplockTypeType,
+    },
+)
+_OptionalCreateSnaplockConfigurationTypeDef = TypedDict(
+    "_OptionalCreateSnaplockConfigurationTypeDef",
+    {
+        "AuditLogVolume": bool,
+        "AutocommitPeriod": AutocommitPeriodTypeDef,
+        "PrivilegedDelete": PrivilegedDeleteType,
+        "RetentionPeriod": SnaplockRetentionPeriodTypeDef,
+        "VolumeAppendModeEnabled": bool,
+    },
+    total=False,
+)
+
+class CreateSnaplockConfigurationTypeDef(
+    _RequiredCreateSnaplockConfigurationTypeDef, _OptionalCreateSnaplockConfigurationTypeDef
+):
+    pass
+
+SnaplockConfigurationTypeDef = TypedDict(
+    "SnaplockConfigurationTypeDef",
+    {
+        "AuditLogVolume": bool,
+        "AutocommitPeriod": AutocommitPeriodTypeDef,
+        "PrivilegedDelete": PrivilegedDeleteType,
+        "RetentionPeriod": SnaplockRetentionPeriodTypeDef,
+        "SnaplockType": SnaplockTypeType,
+        "VolumeAppendModeEnabled": bool,
+    },
+)
+
+UpdateSnaplockConfigurationTypeDef = TypedDict(
+    "UpdateSnaplockConfigurationTypeDef",
+    {
+        "AuditLogVolume": bool,
+        "AutocommitPeriod": AutocommitPeriodTypeDef,
+        "PrivilegedDelete": PrivilegedDeleteType,
+        "RetentionPeriod": SnaplockRetentionPeriodTypeDef,
+        "VolumeAppendModeEnabled": bool,
+    },
+    total=False,
+)
+
 _RequiredUpdateFileSystemRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateFileSystemRequestRequestTypeDef",
     {
         "FileSystemId": str,
     },
 )
 _OptionalUpdateFileSystemRequestRequestTypeDef = TypedDict(
@@ -2340,15 +2262,14 @@
         "StorageVirtualMachineId": str,
         "Subtype": StorageVirtualMachineSubtypeType,
         "UUID": str,
         "Tags": List[TagTypeDef],
         "LifecycleTransitionReason": LifecycleTransitionReasonTypeDef,
         "RootVolumeSecurityStyle": StorageVirtualMachineRootVolumeSecurityStyleType,
     },
-    total=False,
 )
 
 CreateDataRepositoryAssociationResponseTypeDef = TypedDict(
     "CreateDataRepositoryAssociationResponseTypeDef",
     {
         "Association": DataRepositoryAssociationTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
@@ -2418,40 +2339,16 @@
         "WindowsConfiguration": WindowsFileSystemConfigurationTypeDef,
         "LustreConfiguration": LustreFileSystemConfigurationTypeDef,
         "AdministrativeActions": List["AdministrativeActionTypeDef"],
         "OntapConfiguration": OntapFileSystemConfigurationTypeDef,
         "FileSystemTypeVersion": str,
         "OpenZFSConfiguration": OpenZFSFileSystemConfigurationTypeDef,
     },
-    total=False,
 )
 
-_RequiredCreateVolumeRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateVolumeRequestRequestTypeDef",
-    {
-        "VolumeType": VolumeTypeType,
-        "Name": str,
-    },
-)
-_OptionalCreateVolumeRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateVolumeRequestRequestTypeDef",
-    {
-        "ClientRequestToken": str,
-        "OntapConfiguration": CreateOntapVolumeConfigurationTypeDef,
-        "Tags": Sequence[TagTypeDef],
-        "OpenZFSConfiguration": CreateOpenZFSVolumeConfigurationTypeDef,
-    },
-    total=False,
-)
-
-class CreateVolumeRequestRequestTypeDef(
-    _RequiredCreateVolumeRequestRequestTypeDef, _OptionalCreateVolumeRequestRequestTypeDef
-):
-    pass
-
 _RequiredCreateFileSystemOpenZFSConfigurationTypeDef = TypedDict(
     "_RequiredCreateFileSystemOpenZFSConfigurationTypeDef",
     {
         "DeploymentType": OpenZFSDeploymentTypeType,
         "ThroughputCapacity": int,
     },
 )
@@ -2471,55 +2368,75 @@
 
 class CreateFileSystemOpenZFSConfigurationTypeDef(
     _RequiredCreateFileSystemOpenZFSConfigurationTypeDef,
     _OptionalCreateFileSystemOpenZFSConfigurationTypeDef,
 ):
     pass
 
-VolumeTypeDef = TypedDict(
-    "VolumeTypeDef",
+_RequiredCreateOntapVolumeConfigurationTypeDef = TypedDict(
+    "_RequiredCreateOntapVolumeConfigurationTypeDef",
     {
-        "CreationTime": datetime,
-        "FileSystemId": str,
-        "Lifecycle": VolumeLifecycleType,
-        "Name": str,
-        "OntapConfiguration": OntapVolumeConfigurationTypeDef,
-        "ResourceARN": str,
-        "Tags": List[TagTypeDef],
-        "VolumeId": str,
-        "VolumeType": VolumeTypeType,
-        "LifecycleTransitionReason": LifecycleTransitionReasonTypeDef,
-        "AdministrativeActions": List[Dict[str, Any]],
-        "OpenZFSConfiguration": OpenZFSVolumeConfigurationTypeDef,
+        "SizeInMegabytes": int,
+        "StorageVirtualMachineId": str,
+    },
+)
+_OptionalCreateOntapVolumeConfigurationTypeDef = TypedDict(
+    "_OptionalCreateOntapVolumeConfigurationTypeDef",
+    {
+        "JunctionPath": str,
+        "SecurityStyle": SecurityStyleType,
+        "StorageEfficiencyEnabled": bool,
+        "TieringPolicy": TieringPolicyTypeDef,
+        "OntapVolumeType": InputOntapVolumeTypeType,
+        "SnapshotPolicy": str,
+        "CopyTagsToBackups": bool,
+        "SnaplockConfiguration": CreateSnaplockConfigurationTypeDef,
     },
     total=False,
 )
 
-_RequiredUpdateVolumeRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateVolumeRequestRequestTypeDef",
+class CreateOntapVolumeConfigurationTypeDef(
+    _RequiredCreateOntapVolumeConfigurationTypeDef, _OptionalCreateOntapVolumeConfigurationTypeDef
+):
+    pass
+
+OntapVolumeConfigurationTypeDef = TypedDict(
+    "OntapVolumeConfigurationTypeDef",
     {
-        "VolumeId": str,
+        "FlexCacheEndpointType": FlexCacheEndpointTypeType,
+        "JunctionPath": str,
+        "SecurityStyle": SecurityStyleType,
+        "SizeInMegabytes": int,
+        "StorageEfficiencyEnabled": bool,
+        "StorageVirtualMachineId": str,
+        "StorageVirtualMachineRoot": bool,
+        "TieringPolicy": TieringPolicyTypeDef,
+        "UUID": str,
+        "OntapVolumeType": OntapVolumeTypeType,
+        "SnapshotPolicy": str,
+        "CopyTagsToBackups": bool,
+        "SnaplockConfiguration": SnaplockConfigurationTypeDef,
     },
 )
-_OptionalUpdateVolumeRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateVolumeRequestRequestTypeDef",
+
+UpdateOntapVolumeConfigurationTypeDef = TypedDict(
+    "UpdateOntapVolumeConfigurationTypeDef",
     {
-        "ClientRequestToken": str,
-        "OntapConfiguration": UpdateOntapVolumeConfigurationTypeDef,
-        "Name": str,
-        "OpenZFSConfiguration": UpdateOpenZFSVolumeConfigurationTypeDef,
+        "JunctionPath": str,
+        "SecurityStyle": SecurityStyleType,
+        "SizeInMegabytes": int,
+        "StorageEfficiencyEnabled": bool,
+        "TieringPolicy": TieringPolicyTypeDef,
+        "SnapshotPolicy": str,
+        "CopyTagsToBackups": bool,
+        "SnaplockConfiguration": UpdateSnaplockConfigurationTypeDef,
     },
     total=False,
 )
 
-class UpdateVolumeRequestRequestTypeDef(
-    _RequiredUpdateVolumeRequestRequestTypeDef, _OptionalUpdateVolumeRequestRequestTypeDef
-):
-    pass
-
 CreateStorageVirtualMachineResponseTypeDef = TypedDict(
     "CreateStorageVirtualMachineResponseTypeDef",
     {
         "StorageVirtualMachine": StorageVirtualMachineTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -2597,60 +2514,136 @@
 )
 
 class CreateFileSystemRequestRequestTypeDef(
     _RequiredCreateFileSystemRequestRequestTypeDef, _OptionalCreateFileSystemRequestRequestTypeDef
 ):
     pass
 
+_RequiredCreateVolumeFromBackupRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateVolumeFromBackupRequestRequestTypeDef",
+    {
+        "BackupId": str,
+        "Name": str,
+    },
+)
+_OptionalCreateVolumeFromBackupRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateVolumeFromBackupRequestRequestTypeDef",
+    {
+        "ClientRequestToken": str,
+        "OntapConfiguration": CreateOntapVolumeConfigurationTypeDef,
+        "Tags": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
+class CreateVolumeFromBackupRequestRequestTypeDef(
+    _RequiredCreateVolumeFromBackupRequestRequestTypeDef,
+    _OptionalCreateVolumeFromBackupRequestRequestTypeDef,
+):
+    pass
+
+_RequiredCreateVolumeRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateVolumeRequestRequestTypeDef",
+    {
+        "VolumeType": VolumeTypeType,
+        "Name": str,
+    },
+)
+_OptionalCreateVolumeRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateVolumeRequestRequestTypeDef",
+    {
+        "ClientRequestToken": str,
+        "OntapConfiguration": CreateOntapVolumeConfigurationTypeDef,
+        "Tags": Sequence[TagTypeDef],
+        "OpenZFSConfiguration": CreateOpenZFSVolumeConfigurationTypeDef,
+    },
+    total=False,
+)
+
+class CreateVolumeRequestRequestTypeDef(
+    _RequiredCreateVolumeRequestRequestTypeDef, _OptionalCreateVolumeRequestRequestTypeDef
+):
+    pass
+
+VolumeTypeDef = TypedDict(
+    "VolumeTypeDef",
+    {
+        "CreationTime": datetime,
+        "FileSystemId": str,
+        "Lifecycle": VolumeLifecycleType,
+        "Name": str,
+        "OntapConfiguration": OntapVolumeConfigurationTypeDef,
+        "ResourceARN": str,
+        "Tags": List[TagTypeDef],
+        "VolumeId": str,
+        "VolumeType": VolumeTypeType,
+        "LifecycleTransitionReason": LifecycleTransitionReasonTypeDef,
+        "AdministrativeActions": List[Dict[str, Any]],
+        "OpenZFSConfiguration": OpenZFSVolumeConfigurationTypeDef,
+    },
+)
+
+_RequiredUpdateVolumeRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateVolumeRequestRequestTypeDef",
+    {
+        "VolumeId": str,
+    },
+)
+_OptionalUpdateVolumeRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateVolumeRequestRequestTypeDef",
+    {
+        "ClientRequestToken": str,
+        "OntapConfiguration": UpdateOntapVolumeConfigurationTypeDef,
+        "Name": str,
+        "OpenZFSConfiguration": UpdateOpenZFSVolumeConfigurationTypeDef,
+    },
+    total=False,
+)
+
+class UpdateVolumeRequestRequestTypeDef(
+    _RequiredUpdateVolumeRequestRequestTypeDef, _OptionalUpdateVolumeRequestRequestTypeDef
+):
+    pass
+
 AdministrativeActionTypeDef = TypedDict(
     "AdministrativeActionTypeDef",
     {
         "AdministrativeActionType": AdministrativeActionTypeType,
         "ProgressPercent": int,
         "RequestTime": datetime,
         "Status": StatusType,
         "TargetFileSystemValues": Dict[str, Any],
         "FailureDetails": AdministrativeActionFailureDetailsTypeDef,
         "TargetVolumeValues": Dict[str, Any],
         "TargetSnapshotValues": Dict[str, Any],
     },
-    total=False,
 )
 
-_RequiredBackupTypeDef = TypedDict(
-    "_RequiredBackupTypeDef",
+BackupTypeDef = TypedDict(
+    "BackupTypeDef",
     {
         "BackupId": str,
         "Lifecycle": BackupLifecycleType,
-        "Type": BackupTypeType,
-        "CreationTime": datetime,
-        "FileSystem": "FileSystemTypeDef",
-    },
-)
-_OptionalBackupTypeDef = TypedDict(
-    "_OptionalBackupTypeDef",
-    {
         "FailureDetails": BackupFailureDetailsTypeDef,
+        "Type": BackupTypeType,
         "ProgressPercent": int,
+        "CreationTime": datetime,
         "KmsKeyId": str,
         "ResourceARN": str,
         "Tags": List[TagTypeDef],
+        "FileSystem": "FileSystemTypeDef",
         "DirectoryInformation": ActiveDirectoryBackupAttributesTypeDef,
         "OwnerId": str,
         "SourceBackupId": str,
         "SourceBackupRegion": str,
         "ResourceType": ResourceTypeType,
         "Volume": VolumeTypeDef,
     },
-    total=False,
 )
 
-class BackupTypeDef(_RequiredBackupTypeDef, _OptionalBackupTypeDef):
-    pass
-
 CreateVolumeFromBackupResponseTypeDef = TypedDict(
     "CreateVolumeFromBackupResponseTypeDef",
     {
         "Volume": VolumeTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-fsx-1.28.0/mypy_boto3_fsx.egg-info/PKG-INFO` & `mypy-boto3-fsx-1.28.3/mypy_boto3_fsx.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-fsx
-Version: 1.28.0
-Summary: Type annotations for boto3.FSx 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.3
+Summary: Type annotations for boto3.FSx 1.28.3 service generated with mypy-boto3-builder 7.14.6
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-fsx.svg?color=blue)](https://pypi.org/project/mypy-boto3-fsx)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-fsx?color=blue)](https://pypistats.org/packages/mypy-boto3-fsx)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.FSx 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx)
+[boto3.FSx 1.28.3](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx)
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
 [mypy-boto3-fsx docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/).
 
 See how it helps to find and fix potential bugs:
 
@@ -314,14 +314,15 @@
 can be used in user code for type checking.
 
 ```python
 from mypy_boto3_fsx.literals import (
     AdministrativeActionTypeType,
     AliasLifecycleType,
     AutoImportPolicyTypeType,
+    AutocommitPeriodTypeType,
     BackupLifecycleType,
     BackupTypeType,
     DataCompressionTypeType,
     DataRepositoryLifecycleType,
     DataRepositoryTaskFilterNameType,
     DataRepositoryTaskLifecycleType,
     DataRepositoryTaskTypeType,
@@ -349,19 +350,22 @@
     NfsVersionType,
     OntapDeploymentTypeType,
     OntapVolumeTypeType,
     OpenZFSCopyStrategyType,
     OpenZFSDataCompressionTypeType,
     OpenZFSDeploymentTypeType,
     OpenZFSQuotaTypeType,
+    PrivilegedDeleteType,
     ReportFormatType,
     ReportScopeType,
     ResourceTypeType,
     RestoreOpenZFSVolumeOptionType,
+    RetentionPeriodTypeType,
     SecurityStyleType,
+    SnaplockTypeType,
     SnapshotFilterNameType,
     SnapshotLifecycleType,
     StatusType,
     StorageTypeType,
     StorageVirtualMachineFilterNameType,
     StorageVirtualMachineLifecycleType,
     StorageVirtualMachineRootVolumeSecurityStyleType,
@@ -395,14 +399,15 @@
 from mypy_boto3_fsx.type_defs import (
     ActiveDirectoryBackupAttributesTypeDef,
     AdministrativeActionFailureDetailsTypeDef,
     AliasTypeDef,
     AssociateFileSystemAliasesRequestRequestTypeDef,
     AutoExportPolicyTypeDef,
     AutoImportPolicyTypeDef,
+    AutocommitPeriodTypeDef,
     BackupFailureDetailsTypeDef,
     TagTypeDef,
     CancelDataRepositoryTaskRequestRequestTypeDef,
     CancelDataRepositoryTaskResponseTypeDef,
     CompletionReportTypeDef,
     FileCacheLustreMetadataConfigurationTypeDef,
     CreateFileSystemFromBackupResponseTypeDef,
@@ -452,14 +457,15 @@
     OpenZFSOriginSnapshotConfigurationTypeDef,
     PaginatorConfigTypeDef,
     ReleaseFileSystemNfsV3LocksRequestRequestTypeDef,
     ReleaseFileSystemNfsV3LocksResponseTypeDef,
     ResponseMetadataTypeDef,
     RestoreVolumeFromSnapshotRequestRequestTypeDef,
     RestoreVolumeFromSnapshotResponseTypeDef,
+    RetentionPeriodTypeDef,
     SelfManagedActiveDirectoryAttributesTypeDef,
     SelfManagedActiveDirectoryConfigurationUpdatesTypeDef,
     SvmEndpointTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateFileCacheLustreConfigurationTypeDef,
     UpdateFileSystemResponseTypeDef,
     UpdateSnapshotRequestRequestTypeDef,
@@ -488,17 +494,14 @@
     UpdateFileSystemLustreConfigurationTypeDef,
     CreateFileSystemOntapConfigurationTypeDef,
     OpenZFSFileSystemConfigurationTypeDef,
     UpdateFileSystemOntapConfigurationTypeDef,
     UpdateFileSystemOpenZFSConfigurationTypeDef,
     CreateSvmActiveDirectoryConfigurationTypeDef,
     CreateFileSystemWindowsConfigurationTypeDef,
-    CreateOntapVolumeConfigurationTypeDef,
-    OntapVolumeConfigurationTypeDef,
-    UpdateOntapVolumeConfigurationTypeDef,
     DataRepositoryConfigurationTypeDef,
     DescribeDataRepositoryTasksRequestRequestTypeDef,
     DataRepositoryTaskTypeDef,
     DescribeBackupsRequestDescribeBackupsPaginateTypeDef,
     DescribeBackupsRequestRequestTypeDef,
     DescribeDataRepositoryAssociationsRequestRequestTypeDef,
     DescribeSnapshotsRequestRequestTypeDef,
@@ -507,62 +510,69 @@
     DescribeVolumesRequestDescribeVolumesPaginateTypeDef,
     DescribeVolumesRequestRequestTypeDef,
     FileCacheDataRepositoryAssociationTypeDef,
     FileCacheLustreConfigurationTypeDef,
     FileSystemEndpointsTypeDef,
     SnapshotTypeDef,
     OpenZFSNfsExportTypeDef,
+    SnaplockRetentionPeriodTypeDef,
     SvmActiveDirectoryConfigurationTypeDef,
     UpdateFileSystemWindowsConfigurationTypeDef,
     UpdateSvmActiveDirectoryConfigurationTypeDef,
     SvmEndpointsTypeDef,
     UpdateFileCacheRequestRequestTypeDef,
     WindowsFileSystemConfigurationTypeDef,
     CreateDataRepositoryAssociationRequestRequestTypeDef,
     DataRepositoryAssociationTypeDef,
     UpdateDataRepositoryAssociationRequestRequestTypeDef,
     DeleteFileSystemRequestRequestTypeDef,
     DeleteFileSystemResponseTypeDef,
     DeleteVolumeRequestRequestTypeDef,
     DeleteVolumeResponseTypeDef,
     CreateStorageVirtualMachineRequestRequestTypeDef,
-    CreateVolumeFromBackupRequestRequestTypeDef,
     LustreFileSystemConfigurationTypeDef,
     CreateDataRepositoryTaskResponseTypeDef,
     DescribeDataRepositoryTasksResponseTypeDef,
     CreateFileCacheRequestRequestTypeDef,
     FileCacheCreatingTypeDef,
     FileCacheTypeDef,
     OntapFileSystemConfigurationTypeDef,
     CreateSnapshotResponseTypeDef,
     DescribeSnapshotsResponseTypeDef,
     UpdateSnapshotResponseTypeDef,
     CreateOpenZFSVolumeConfigurationTypeDef,
     OpenZFSCreateRootVolumeConfigurationTypeDef,
     OpenZFSVolumeConfigurationTypeDef,
     UpdateOpenZFSVolumeConfigurationTypeDef,
+    CreateSnaplockConfigurationTypeDef,
+    SnaplockConfigurationTypeDef,
+    UpdateSnaplockConfigurationTypeDef,
     UpdateFileSystemRequestRequestTypeDef,
     UpdateStorageVirtualMachineRequestRequestTypeDef,
     StorageVirtualMachineTypeDef,
     CreateDataRepositoryAssociationResponseTypeDef,
     DescribeDataRepositoryAssociationsResponseTypeDef,
     UpdateDataRepositoryAssociationResponseTypeDef,
     CreateFileCacheResponseTypeDef,
     DescribeFileCachesResponseTypeDef,
     UpdateFileCacheResponseTypeDef,
     FileSystemTypeDef,
-    CreateVolumeRequestRequestTypeDef,
     CreateFileSystemOpenZFSConfigurationTypeDef,
-    VolumeTypeDef,
-    UpdateVolumeRequestRequestTypeDef,
+    CreateOntapVolumeConfigurationTypeDef,
+    OntapVolumeConfigurationTypeDef,
+    UpdateOntapVolumeConfigurationTypeDef,
     CreateStorageVirtualMachineResponseTypeDef,
     DescribeStorageVirtualMachinesResponseTypeDef,
     UpdateStorageVirtualMachineResponseTypeDef,
     CreateFileSystemFromBackupRequestRequestTypeDef,
     CreateFileSystemRequestRequestTypeDef,
+    CreateVolumeFromBackupRequestRequestTypeDef,
+    CreateVolumeRequestRequestTypeDef,
+    VolumeTypeDef,
+    UpdateVolumeRequestRequestTypeDef,
     AdministrativeActionTypeDef,
     BackupTypeDef,
     CreateVolumeFromBackupResponseTypeDef,
     CreateVolumeResponseTypeDef,
     DescribeVolumesResponseTypeDef,
     UpdateVolumeResponseTypeDef,
     CopyBackupResponseTypeDef,
```

### Comparing `mypy-boto3-fsx-1.28.0/mypy_boto3_fsx.egg-info/SOURCES.txt` & `mypy-boto3-fsx-1.28.3/mypy_boto3_fsx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-fsx-1.28.0/setup.py` & `mypy-boto3-fsx-1.28.3/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-fsx",
-    version="1.28.0",
+    version="1.28.3",
     packages=["mypy_boto3_fsx"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.FSx 1.28.0 service generated with mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.FSx 1.28.3 service generated with mypy-boto3-builder 7.14.6"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

