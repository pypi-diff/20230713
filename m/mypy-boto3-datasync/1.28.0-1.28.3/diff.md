# Comparing `tmp/mypy-boto3-datasync-1.28.0.tar.gz` & `tmp/mypy-boto3-datasync-1.28.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-datasync-1.28.0.tar", last modified: Thu Jul  6 20:59:22 2023, max compression
+gzip compressed data, was "mypy-boto3-datasync-1.28.3.tar", last modified: Thu Jul 13 19:49:12 2023, max compression
```

## Comparing `mypy-boto3-datasync-1.28.0.tar` & `mypy-boto3-datasync-1.28.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:22.918275 mypy-boto3-datasync-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:37:31.000000 mypy-boto3-datasync-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    20467 2023-07-06 20:59:22.918275 mypy-boto3-datasync-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18978 2023-07-06 20:37:31.000000 mypy-boto3-datasync-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:22.918275 mypy-boto3-datasync-1.28.0/mypy_boto3_datasync/
--rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-07-06 20:37:31.000000 mypy-boto3-datasync-1.28.0/mypy_boto3_datasync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-07-06 20:37:31.000000 mypy-boto3-datasync-1.28.0/mypy_boto3_datasync/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-07-06 20:37:31.000000 mypy-boto3-datasync-1.28.0/mypy_boto3_datasync/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    45375 2023-07-06 20:37:32.000000 mypy-boto3-datasync-1.28.0/mypy_boto3_datasync/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    45303 2023-07-06 20:37:31.000000 mypy-boto3-datasync-1.28.0/mypy_boto3_datasync/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12831 2023-07-06 20:37:32.000000 mypy-boto3-datasync-1.28.0/mypy_boto3_datasync/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    12829 2023-07-06 20:37:32.000000 mypy-boto3-datasync-1.28.0/mypy_boto3_datasync/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9911 2023-07-06 20:37:32.000000 mypy-boto3-datasync-1.28.0/mypy_boto3_datasync/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9901 2023-07-06 20:37:32.000000 mypy-boto3-datasync-1.28.0/mypy_boto3_datasync/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:37:31.000000 mypy-boto3-datasync-1.28.0/mypy_boto3_datasync/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    55433 2023-07-06 20:37:34.000000 mypy-boto3-datasync-1.28.0/mypy_boto3_datasync/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    55372 2023-07-06 20:37:33.000000 mypy-boto3-datasync-1.28.0/mypy_boto3_datasync/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:37:31.000000 mypy-boto3-datasync-1.28.0/mypy_boto3_datasync/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:22.918275 mypy-boto3-datasync-1.28.0/mypy_boto3_datasync.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20467 2023-07-06 20:59:22.000000 mypy-boto3-datasync-1.28.0/mypy_boto3_datasync.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-06 20:59:22.000000 mypy-boto3-datasync-1.28.0/mypy_boto3_datasync.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:22.000000 mypy-boto3-datasync-1.28.0/mypy_boto3_datasync.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:22.000000 mypy-boto3-datasync-1.28.0/mypy_boto3_datasync.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 20:59:22.000000 mypy-boto3-datasync-1.28.0/mypy_boto3_datasync.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-06 20:59:22.000000 mypy-boto3-datasync-1.28.0/mypy_boto3_datasync.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 20:59:22.918275 mypy-boto3-datasync-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-07-06 20:37:31.000000 mypy-boto3-datasync-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:49:12.653227 mypy-boto3-datasync-1.28.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-13 19:47:08.000000 mypy-boto3-datasync-1.28.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    20467 2023-07-13 19:49:12.653227 mypy-boto3-datasync-1.28.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18978 2023-07-13 19:47:08.000000 mypy-boto3-datasync-1.28.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:49:12.653227 mypy-boto3-datasync-1.28.3/mypy_boto3_datasync/
+-rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-07-13 19:47:08.000000 mypy-boto3-datasync-1.28.3/mypy_boto3_datasync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-07-13 19:47:08.000000 mypy-boto3-datasync-1.28.3/mypy_boto3_datasync/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-07-13 19:47:08.000000 mypy-boto3-datasync-1.28.3/mypy_boto3_datasync/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45373 2023-07-13 19:47:09.000000 mypy-boto3-datasync-1.28.3/mypy_boto3_datasync/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45301 2023-07-13 19:47:09.000000 mypy-boto3-datasync-1.28.3/mypy_boto3_datasync/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12831 2023-07-13 19:47:09.000000 mypy-boto3-datasync-1.28.3/mypy_boto3_datasync/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12829 2023-07-13 19:47:09.000000 mypy-boto3-datasync-1.28.3/mypy_boto3_datasync/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9911 2023-07-13 19:47:09.000000 mypy-boto3-datasync-1.28.3/mypy_boto3_datasync/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9901 2023-07-13 19:47:09.000000 mypy-boto3-datasync-1.28.3/mypy_boto3_datasync/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 19:47:08.000000 mypy-boto3-datasync-1.28.3/mypy_boto3_datasync/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    55168 2023-07-13 19:47:11.000000 mypy-boto3-datasync-1.28.3/mypy_boto3_datasync/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55107 2023-07-13 19:47:10.000000 mypy-boto3-datasync-1.28.3/mypy_boto3_datasync/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-13 19:47:08.000000 mypy-boto3-datasync-1.28.3/mypy_boto3_datasync/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:49:12.653227 mypy-boto3-datasync-1.28.3/mypy_boto3_datasync.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20467 2023-07-13 19:49:12.000000 mypy-boto3-datasync-1.28.3/mypy_boto3_datasync.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-13 19:49:12.000000 mypy-boto3-datasync-1.28.3/mypy_boto3_datasync.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 19:49:12.000000 mypy-boto3-datasync-1.28.3/mypy_boto3_datasync.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 19:49:12.000000 mypy-boto3-datasync-1.28.3/mypy_boto3_datasync.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-13 19:49:12.000000 mypy-boto3-datasync-1.28.3/mypy_boto3_datasync.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-13 19:49:12.000000 mypy-boto3-datasync-1.28.3/mypy_boto3_datasync.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 19:49:12.653227 mypy-boto3-datasync-1.28.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-07-13 19:47:08.000000 mypy-boto3-datasync-1.28.3/setup.py
```

### Comparing `mypy-boto3-datasync-1.28.0/LICENSE` & `mypy-boto3-datasync-1.28.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-datasync-1.28.0/PKG-INFO` & `mypy-boto3-datasync-1.28.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-datasync
-Version: 1.28.0
-Summary: Type annotations for boto3.DataSync 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.3
+Summary: Type annotations for boto3.DataSync 1.28.3 service generated with mypy-boto3-builder 7.14.6
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-datasync.svg?color=blue)](https://pypi.org/project/mypy-boto3-datasync)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-datasync?color=blue)](https://pypistats.org/packages/mypy-boto3-datasync)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.DataSync 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync)
+[boto3.DataSync 1.28.3](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync)
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
 [mypy-boto3-datasync docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-datasync-1.28.0/README.md` & `mypy-boto3-datasync-1.28.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-datasync.svg?color=blue)](https://pypi.org/project/mypy-boto3-datasync)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-datasync?color=blue)](https://pypistats.org/packages/mypy-boto3-datasync)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.DataSync 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync)
+[boto3.DataSync 1.28.3](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync)
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
 [mypy-boto3-datasync docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-datasync-1.28.0/mypy_boto3_datasync/__init__.py` & `mypy-boto3-datasync-1.28.3/mypy_boto3_datasync/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-datasync-1.28.0/mypy_boto3_datasync/__init__.pyi` & `mypy-boto3-datasync-1.28.3/mypy_boto3_datasync/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-datasync-1.28.0/mypy_boto3_datasync/client.py` & `mypy-boto3-datasync-1.28.3/mypy_boto3_datasync/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -186,15 +186,15 @@
         AgentName: str = ...,
         Tags: Sequence[TagListEntryTypeDef] = ...,
         VpcEndpointId: str = ...,
         SubnetArns: Sequence[str] = ...,
         SecurityGroupArns: Sequence[str] = ...
     ) -> CreateAgentResponseTypeDef:
         """
-        Activates an DataSync agent that you have deployed in your storage environment.
+        Activates an DataSync agent that you've deployed in your storage environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.create_agent)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#create_agent)
         """
 
     def create_location_efs(
         self,
```

### Comparing `mypy-boto3-datasync-1.28.0/mypy_boto3_datasync/client.pyi` & `mypy-boto3-datasync-1.28.3/mypy_boto3_datasync/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -177,15 +177,15 @@
         AgentName: str = ...,
         Tags: Sequence[TagListEntryTypeDef] = ...,
         VpcEndpointId: str = ...,
         SubnetArns: Sequence[str] = ...,
         SecurityGroupArns: Sequence[str] = ...
     ) -> CreateAgentResponseTypeDef:
         """
-        Activates an DataSync agent that you have deployed in your storage environment.
+        Activates an DataSync agent that you've deployed in your storage environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.create_agent)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#create_agent)
         """
     def create_location_efs(
         self,
         *,
```

### Comparing `mypy-boto3-datasync-1.28.0/mypy_boto3_datasync/literals.py` & `mypy-boto3-datasync-1.28.3/mypy_boto3_datasync/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-datasync-1.28.0/mypy_boto3_datasync/literals.pyi` & `mypy-boto3-datasync-1.28.3/mypy_boto3_datasync/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-datasync-1.28.0/mypy_boto3_datasync/paginator.py` & `mypy-boto3-datasync-1.28.3/mypy_boto3_datasync/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-datasync-1.28.0/mypy_boto3_datasync/paginator.pyi` & `mypy-boto3-datasync-1.28.3/mypy_boto3_datasync/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-datasync-1.28.0/mypy_boto3_datasync/type_defs.py` & `mypy-boto3-datasync-1.28.3/mypy_boto3_datasync/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -270,15 +270,14 @@
 AgentListEntryTypeDef = TypedDict(
     "AgentListEntryTypeDef",
     {
         "AgentArn": str,
         "Name": str,
         "Status": AgentStatusType,
     },
-    total=False,
 )
 
 CancelTaskExecutionRequestRequestTypeDef = TypedDict(
     "CancelTaskExecutionRequestRequestTypeDef",
     {
         "TaskExecutionArn": str,
     },
@@ -287,15 +286,14 @@
 CapacityTypeDef = TypedDict(
     "CapacityTypeDef",
     {
         "Used": int,
         "Provisioned": int,
         "LogicalUsed": int,
     },
-    total=False,
 )
 
 CreateAgentResponseTypeDef = TypedDict(
     "CreateAgentResponseTypeDef",
     {
         "AgentArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
@@ -515,15 +513,14 @@
     "PrivateLinkConfigTypeDef",
     {
         "VpcEndpointId": str,
         "PrivateLinkEndpoint": str,
         "SubnetArns": List[str],
         "SecurityGroupArns": List[str],
     },
-    total=False,
 )
 
 DescribeDiscoveryJobRequestRequestTypeDef = TypedDict(
     "DescribeDiscoveryJobRequestRequestTypeDef",
     {
         "DiscoveryJobArn": str,
     },
@@ -753,15 +750,14 @@
         "TransferDuration": int,
         "TransferStatus": PhaseStatusType,
         "VerifyDuration": int,
         "VerifyStatus": PhaseStatusType,
         "ErrorCode": str,
         "ErrorDetail": str,
     },
-    total=False,
 )
 
 DescribeTaskRequestRequestTypeDef = TypedDict(
     "DescribeTaskRequestRequestTypeDef",
     {
         "TaskArn": str,
     },
@@ -769,15 +765,14 @@
 
 DiscoveryJobListEntryTypeDef = TypedDict(
     "DiscoveryJobListEntryTypeDef",
     {
         "DiscoveryJobArn": str,
         "Status": DiscoveryJobStatusType,
     },
-    total=False,
 )
 
 GenerateRecommendationsRequestRequestTypeDef = TypedDict(
     "GenerateRecommendationsRequestRequestTypeDef",
     {
         "DiscoveryJobArn": str,
         "ResourceIds": Sequence[str],
@@ -789,25 +784,23 @@
     "IOPSTypeDef",
     {
         "Read": float,
         "Write": float,
         "Other": float,
         "Total": float,
     },
-    total=False,
 )
 
 LatencyTypeDef = TypedDict(
     "LatencyTypeDef",
     {
         "Read": float,
         "Write": float,
         "Other": float,
     },
-    total=False,
 )
 
 ListAgentsRequestListAgentsPaginateTypeDef = TypedDict(
     "ListAgentsRequestListAgentsPaginateTypeDef",
     {
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
@@ -853,15 +846,14 @@
 
 LocationListEntryTypeDef = TypedDict(
     "LocationListEntryTypeDef",
     {
         "LocationArn": str,
         "LocationUri": str,
     },
-    total=False,
 )
 
 ListStorageSystemsRequestListStorageSystemsPaginateTypeDef = TypedDict(
     "ListStorageSystemsRequestListStorageSystemsPaginateTypeDef",
     {
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
@@ -879,15 +871,14 @@
 
 StorageSystemListEntryTypeDef = TypedDict(
     "StorageSystemListEntryTypeDef",
     {
         "StorageSystemArn": str,
         "Name": str,
     },
-    total=False,
 )
 
 _RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
     "_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     {
         "ResourceArn": str,
     },
@@ -952,15 +943,14 @@
 
 TaskExecutionListEntryTypeDef = TypedDict(
     "TaskExecutionListEntryTypeDef",
     {
         "TaskExecutionArn": str,
         "Status": TaskExecutionStatusType,
     },
-    total=False,
 )
 
 TaskFilterTypeDef = TypedDict(
     "TaskFilterTypeDef",
     {
         "Name": TaskFilterNameType,
         "Values": Sequence[str],
@@ -971,15 +961,14 @@
 TaskListEntryTypeDef = TypedDict(
     "TaskListEntryTypeDef",
     {
         "TaskArn": str,
         "Status": TaskStatusType,
         "Name": str,
     },
-    total=False,
 )
 
 MaxP95PerformanceTypeDef = TypedDict(
     "MaxP95PerformanceTypeDef",
     {
         "IopsRead": float,
         "IopsWrite": float,
@@ -989,36 +978,33 @@
         "ThroughputWrite": float,
         "ThroughputOther": float,
         "ThroughputTotal": float,
         "LatencyRead": float,
         "LatencyWrite": float,
         "LatencyOther": float,
     },
-    total=False,
 )
 
 RecommendationTypeDef = TypedDict(
     "RecommendationTypeDef",
     {
         "StorageType": str,
         "StorageConfiguration": Dict[str, str],
         "EstimatedMonthlyStorageCost": str,
     },
-    total=False,
 )
 
 ThroughputTypeDef = TypedDict(
     "ThroughputTypeDef",
     {
         "Read": float,
         "Write": float,
         "Other": float,
         "Total": float,
     },
-    total=False,
 )
 
 PaginatorConfigTypeDef = TypedDict(
     "PaginatorConfigTypeDef",
     {
         "MaxItems": int,
         "PageSize": int,
@@ -1912,16 +1898,16 @@
         "ClusterName": str,
         "MaxP95Performance": MaxP95PerformanceTypeDef,
         "ClusterBlockStorageSize": int,
         "ClusterBlockStorageUsed": int,
         "ClusterBlockStorageLogicalUsed": int,
         "Recommendations": List[RecommendationTypeDef],
         "RecommendationStatus": RecommendationStatusType,
+        "LunCount": int,
     },
-    total=False,
 )
 
 NetAppONTAPSVMTypeDef = TypedDict(
     "NetAppONTAPSVMTypeDef",
     {
         "ClusterUuid": str,
         "ResourceId": str,
@@ -1932,16 +1918,16 @@
         "TotalCapacityProvisioned": int,
         "TotalLogicalCapacityUsed": int,
         "MaxP95Performance": MaxP95PerformanceTypeDef,
         "Recommendations": List[RecommendationTypeDef],
         "NfsExportedVolumes": int,
         "RecommendationStatus": RecommendationStatusType,
         "TotalSnapshotCapacityUsed": int,
+        "LunCount": int,
     },
-    total=False,
 )
 
 NetAppONTAPVolumeTypeDef = TypedDict(
     "NetAppONTAPVolumeTypeDef",
     {
         "VolumeName": str,
         "ResourceId": str,
@@ -1953,26 +1939,25 @@
         "CapacityProvisioned": int,
         "LogicalCapacityUsed": int,
         "NfsExported": bool,
         "SnapshotCapacityUsed": int,
         "MaxP95Performance": MaxP95PerformanceTypeDef,
         "Recommendations": List[RecommendationTypeDef],
         "RecommendationStatus": RecommendationStatusType,
+        "LunCount": int,
     },
-    total=False,
 )
 
 P95MetricsTypeDef = TypedDict(
     "P95MetricsTypeDef",
     {
         "IOPS": IOPSTypeDef,
         "Throughput": ThroughputTypeDef,
         "Latency": LatencyTypeDef,
     },
-    total=False,
 )
 
 FsxProtocolTypeDef = TypedDict(
     "FsxProtocolTypeDef",
     {
         "NFS": FsxProtocolNfsTypeDef,
         "SMB": FsxProtocolSmbTypeDef,
@@ -1983,27 +1968,25 @@
 ResourceDetailsTypeDef = TypedDict(
     "ResourceDetailsTypeDef",
     {
         "NetAppONTAPSVMs": List[NetAppONTAPSVMTypeDef],
         "NetAppONTAPVolumes": List[NetAppONTAPVolumeTypeDef],
         "NetAppONTAPClusters": List[NetAppONTAPClusterTypeDef],
     },
-    total=False,
 )
 
 ResourceMetricsTypeDef = TypedDict(
     "ResourceMetricsTypeDef",
     {
         "Timestamp": datetime,
         "P95Metrics": P95MetricsTypeDef,
         "Capacity": CapacityTypeDef,
         "ResourceId": str,
         "ResourceType": DiscoveryResourceTypeType,
     },
-    total=False,
 )
 
 _RequiredCreateLocationFsxOntapRequestRequestTypeDef = TypedDict(
     "_RequiredCreateLocationFsxOntapRequestRequestTypeDef",
     {
         "Protocol": FsxProtocolTypeDef,
         "SecurityGroupArns": Sequence[str],
```

### Comparing `mypy-boto3-datasync-1.28.0/mypy_boto3_datasync/type_defs.pyi` & `mypy-boto3-datasync-1.28.3/mypy_boto3_datasync/type_defs.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -265,15 +265,14 @@
 AgentListEntryTypeDef = TypedDict(
     "AgentListEntryTypeDef",
     {
         "AgentArn": str,
         "Name": str,
         "Status": AgentStatusType,
     },
-    total=False,
 )
 
 CancelTaskExecutionRequestRequestTypeDef = TypedDict(
     "CancelTaskExecutionRequestRequestTypeDef",
     {
         "TaskExecutionArn": str,
     },
@@ -282,15 +281,14 @@
 CapacityTypeDef = TypedDict(
     "CapacityTypeDef",
     {
         "Used": int,
         "Provisioned": int,
         "LogicalUsed": int,
     },
-    total=False,
 )
 
 CreateAgentResponseTypeDef = TypedDict(
     "CreateAgentResponseTypeDef",
     {
         "AgentArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
@@ -510,15 +508,14 @@
     "PrivateLinkConfigTypeDef",
     {
         "VpcEndpointId": str,
         "PrivateLinkEndpoint": str,
         "SubnetArns": List[str],
         "SecurityGroupArns": List[str],
     },
-    total=False,
 )
 
 DescribeDiscoveryJobRequestRequestTypeDef = TypedDict(
     "DescribeDiscoveryJobRequestRequestTypeDef",
     {
         "DiscoveryJobArn": str,
     },
@@ -742,15 +739,14 @@
         "TransferDuration": int,
         "TransferStatus": PhaseStatusType,
         "VerifyDuration": int,
         "VerifyStatus": PhaseStatusType,
         "ErrorCode": str,
         "ErrorDetail": str,
     },
-    total=False,
 )
 
 DescribeTaskRequestRequestTypeDef = TypedDict(
     "DescribeTaskRequestRequestTypeDef",
     {
         "TaskArn": str,
     },
@@ -758,15 +754,14 @@
 
 DiscoveryJobListEntryTypeDef = TypedDict(
     "DiscoveryJobListEntryTypeDef",
     {
         "DiscoveryJobArn": str,
         "Status": DiscoveryJobStatusType,
     },
-    total=False,
 )
 
 GenerateRecommendationsRequestRequestTypeDef = TypedDict(
     "GenerateRecommendationsRequestRequestTypeDef",
     {
         "DiscoveryJobArn": str,
         "ResourceIds": Sequence[str],
@@ -778,25 +773,23 @@
     "IOPSTypeDef",
     {
         "Read": float,
         "Write": float,
         "Other": float,
         "Total": float,
     },
-    total=False,
 )
 
 LatencyTypeDef = TypedDict(
     "LatencyTypeDef",
     {
         "Read": float,
         "Write": float,
         "Other": float,
     },
-    total=False,
 )
 
 ListAgentsRequestListAgentsPaginateTypeDef = TypedDict(
     "ListAgentsRequestListAgentsPaginateTypeDef",
     {
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
@@ -842,15 +835,14 @@
 
 LocationListEntryTypeDef = TypedDict(
     "LocationListEntryTypeDef",
     {
         "LocationArn": str,
         "LocationUri": str,
     },
-    total=False,
 )
 
 ListStorageSystemsRequestListStorageSystemsPaginateTypeDef = TypedDict(
     "ListStorageSystemsRequestListStorageSystemsPaginateTypeDef",
     {
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
@@ -868,15 +860,14 @@
 
 StorageSystemListEntryTypeDef = TypedDict(
     "StorageSystemListEntryTypeDef",
     {
         "StorageSystemArn": str,
         "Name": str,
     },
-    total=False,
 )
 
 _RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
     "_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     {
         "ResourceArn": str,
     },
@@ -937,15 +928,14 @@
 
 TaskExecutionListEntryTypeDef = TypedDict(
     "TaskExecutionListEntryTypeDef",
     {
         "TaskExecutionArn": str,
         "Status": TaskExecutionStatusType,
     },
-    total=False,
 )
 
 TaskFilterTypeDef = TypedDict(
     "TaskFilterTypeDef",
     {
         "Name": TaskFilterNameType,
         "Values": Sequence[str],
@@ -956,15 +946,14 @@
 TaskListEntryTypeDef = TypedDict(
     "TaskListEntryTypeDef",
     {
         "TaskArn": str,
         "Status": TaskStatusType,
         "Name": str,
     },
-    total=False,
 )
 
 MaxP95PerformanceTypeDef = TypedDict(
     "MaxP95PerformanceTypeDef",
     {
         "IopsRead": float,
         "IopsWrite": float,
@@ -974,36 +963,33 @@
         "ThroughputWrite": float,
         "ThroughputOther": float,
         "ThroughputTotal": float,
         "LatencyRead": float,
         "LatencyWrite": float,
         "LatencyOther": float,
     },
-    total=False,
 )
 
 RecommendationTypeDef = TypedDict(
     "RecommendationTypeDef",
     {
         "StorageType": str,
         "StorageConfiguration": Dict[str, str],
         "EstimatedMonthlyStorageCost": str,
     },
-    total=False,
 )
 
 ThroughputTypeDef = TypedDict(
     "ThroughputTypeDef",
     {
         "Read": float,
         "Write": float,
         "Other": float,
         "Total": float,
     },
-    total=False,
 )
 
 PaginatorConfigTypeDef = TypedDict(
     "PaginatorConfigTypeDef",
     {
         "MaxItems": int,
         "PageSize": int,
@@ -1855,16 +1841,16 @@
         "ClusterName": str,
         "MaxP95Performance": MaxP95PerformanceTypeDef,
         "ClusterBlockStorageSize": int,
         "ClusterBlockStorageUsed": int,
         "ClusterBlockStorageLogicalUsed": int,
         "Recommendations": List[RecommendationTypeDef],
         "RecommendationStatus": RecommendationStatusType,
+        "LunCount": int,
     },
-    total=False,
 )
 
 NetAppONTAPSVMTypeDef = TypedDict(
     "NetAppONTAPSVMTypeDef",
     {
         "ClusterUuid": str,
         "ResourceId": str,
@@ -1875,16 +1861,16 @@
         "TotalCapacityProvisioned": int,
         "TotalLogicalCapacityUsed": int,
         "MaxP95Performance": MaxP95PerformanceTypeDef,
         "Recommendations": List[RecommendationTypeDef],
         "NfsExportedVolumes": int,
         "RecommendationStatus": RecommendationStatusType,
         "TotalSnapshotCapacityUsed": int,
+        "LunCount": int,
     },
-    total=False,
 )
 
 NetAppONTAPVolumeTypeDef = TypedDict(
     "NetAppONTAPVolumeTypeDef",
     {
         "VolumeName": str,
         "ResourceId": str,
@@ -1896,26 +1882,25 @@
         "CapacityProvisioned": int,
         "LogicalCapacityUsed": int,
         "NfsExported": bool,
         "SnapshotCapacityUsed": int,
         "MaxP95Performance": MaxP95PerformanceTypeDef,
         "Recommendations": List[RecommendationTypeDef],
         "RecommendationStatus": RecommendationStatusType,
+        "LunCount": int,
     },
-    total=False,
 )
 
 P95MetricsTypeDef = TypedDict(
     "P95MetricsTypeDef",
     {
         "IOPS": IOPSTypeDef,
         "Throughput": ThroughputTypeDef,
         "Latency": LatencyTypeDef,
     },
-    total=False,
 )
 
 FsxProtocolTypeDef = TypedDict(
     "FsxProtocolTypeDef",
     {
         "NFS": FsxProtocolNfsTypeDef,
         "SMB": FsxProtocolSmbTypeDef,
@@ -1926,27 +1911,25 @@
 ResourceDetailsTypeDef = TypedDict(
     "ResourceDetailsTypeDef",
     {
         "NetAppONTAPSVMs": List[NetAppONTAPSVMTypeDef],
         "NetAppONTAPVolumes": List[NetAppONTAPVolumeTypeDef],
         "NetAppONTAPClusters": List[NetAppONTAPClusterTypeDef],
     },
-    total=False,
 )
 
 ResourceMetricsTypeDef = TypedDict(
     "ResourceMetricsTypeDef",
     {
         "Timestamp": datetime,
         "P95Metrics": P95MetricsTypeDef,
         "Capacity": CapacityTypeDef,
         "ResourceId": str,
         "ResourceType": DiscoveryResourceTypeType,
     },
-    total=False,
 )
 
 _RequiredCreateLocationFsxOntapRequestRequestTypeDef = TypedDict(
     "_RequiredCreateLocationFsxOntapRequestRequestTypeDef",
     {
         "Protocol": FsxProtocolTypeDef,
         "SecurityGroupArns": Sequence[str],
```

### Comparing `mypy-boto3-datasync-1.28.0/mypy_boto3_datasync.egg-info/PKG-INFO` & `mypy-boto3-datasync-1.28.3/mypy_boto3_datasync.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-datasync
-Version: 1.28.0
-Summary: Type annotations for boto3.DataSync 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.3
+Summary: Type annotations for boto3.DataSync 1.28.3 service generated with mypy-boto3-builder 7.14.6
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-datasync.svg?color=blue)](https://pypi.org/project/mypy-boto3-datasync)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-datasync?color=blue)](https://pypistats.org/packages/mypy-boto3-datasync)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.DataSync 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync)
+[boto3.DataSync 1.28.3](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync)
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
 [mypy-boto3-datasync docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-datasync-1.28.0/mypy_boto3_datasync.egg-info/SOURCES.txt` & `mypy-boto3-datasync-1.28.3/mypy_boto3_datasync.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-datasync-1.28.0/setup.py` & `mypy-boto3-datasync-1.28.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-datasync",
-    version="1.28.0",
+    version="1.28.3",
     packages=["mypy_boto3_datasync"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.DataSync 1.28.0 service generated with mypy-boto3-builder"
-        " 7.14.5"
+        "Type annotations for boto3.DataSync 1.28.3 service generated with mypy-boto3-builder"
+        " 7.14.6"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

