# Comparing `tmp/mypy-boto3-proton-1.28.0.tar.gz` & `tmp/mypy-boto3-proton-1.28.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-proton-1.28.0.tar", last modified: Thu Jul  6 21:00:22 2023, max compression
+gzip compressed data, was "mypy-boto3-proton-1.28.3.tar", last modified: Thu Jul 13 19:49:15 2023, max compression
```

## Comparing `mypy-boto3-proton-1.28.0.tar` & `mypy-boto3-proton-1.28.3.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:21.998399 mypy-boto3-proton-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:49:48.000000 mypy-boto3-proton-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    30630 2023-07-06 21:00:21.998399 mypy-boto3-proton-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    29149 2023-07-06 20:49:48.000000 mypy-boto3-proton-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:21.994399 mypy-boto3-proton-1.28.0/mypy_boto3_proton/
--rw-r--r--   0 runner    (1001) docker     (123)     7753 2023-07-06 20:49:48.000000 mypy-boto3-proton-1.28.0/mypy_boto3_proton/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7752 2023-07-06 20:49:48.000000 mypy-boto3-proton-1.28.0/mypy_boto3_proton/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-07-06 20:49:48.000000 mypy-boto3-proton-1.28.0/mypy_boto3_proton/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    72051 2023-07-06 20:49:51.000000 mypy-boto3-proton-1.28.0/mypy_boto3_proton/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    71930 2023-07-06 20:49:48.000000 mypy-boto3-proton-1.28.0/mypy_boto3_proton/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    15579 2023-07-06 20:49:52.000000 mypy-boto3-proton-1.28.0/mypy_boto3_proton/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    15577 2023-07-06 20:49:51.000000 mypy-boto3-proton-1.28.0/mypy_boto3_proton/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    25141 2023-07-06 20:49:51.000000 mypy-boto3-proton-1.28.0/mypy_boto3_proton/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    25119 2023-07-06 20:49:51.000000 mypy-boto3-proton-1.28.0/mypy_boto3_proton/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:49:48.000000 mypy-boto3-proton-1.28.0/mypy_boto3_proton/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   105724 2023-07-06 20:49:54.000000 mypy-boto3-proton-1.28.0/mypy_boto3_proton/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   105551 2023-07-06 20:49:53.000000 mypy-boto3-proton-1.28.0/mypy_boto3_proton/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:49:48.000000 mypy-boto3-proton-1.28.0/mypy_boto3_proton/version.py
--rw-r--r--   0 runner    (1001) docker     (123)    10159 2023-07-06 20:49:51.000000 mypy-boto3-proton-1.28.0/mypy_boto3_proton/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)    10149 2023-07-06 20:49:51.000000 mypy-boto3-proton-1.28.0/mypy_boto3_proton/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:21.998399 mypy-boto3-proton-1.28.0/mypy_boto3_proton.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    30630 2023-07-06 21:00:21.000000 mypy-boto3-proton-1.28.0/mypy_boto3_proton.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-06 21:00:21.000000 mypy-boto3-proton-1.28.0/mypy_boto3_proton.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:21.000000 mypy-boto3-proton-1.28.0/mypy_boto3_proton.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:21.000000 mypy-boto3-proton-1.28.0/mypy_boto3_proton.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 21:00:21.000000 mypy-boto3-proton-1.28.0/mypy_boto3_proton.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-06 21:00:21.000000 mypy-boto3-proton-1.28.0/mypy_boto3_proton.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 21:00:21.998399 mypy-boto3-proton-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-07-06 20:49:47.000000 mypy-boto3-proton-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:49:15.197303 mypy-boto3-proton-1.28.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-13 19:48:23.000000 mypy-boto3-proton-1.28.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    31307 2023-07-13 19:49:15.197303 mypy-boto3-proton-1.28.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    29826 2023-07-13 19:48:23.000000 mypy-boto3-proton-1.28.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:49:15.197303 mypy-boto3-proton-1.28.3/mypy_boto3_proton/
+-rw-r--r--   0 runner    (1001) docker     (123)     7949 2023-07-13 19:48:23.000000 mypy-boto3-proton-1.28.3/mypy_boto3_proton/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7948 2023-07-13 19:48:23.000000 mypy-boto3-proton-1.28.3/mypy_boto3_proton/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-07-13 19:48:23.000000 mypy-boto3-proton-1.28.3/mypy_boto3_proton/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    74390 2023-07-13 19:48:23.000000 mypy-boto3-proton-1.28.3/mypy_boto3_proton/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    74265 2023-07-13 19:48:23.000000 mypy-boto3-proton-1.28.3/mypy_boto3_proton/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    15855 2023-07-13 19:48:25.000000 mypy-boto3-proton-1.28.3/mypy_boto3_proton/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15853 2023-07-13 19:48:24.000000 mypy-boto3-proton-1.28.3/mypy_boto3_proton/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    26520 2023-07-13 19:48:24.000000 mypy-boto3-proton-1.28.3/mypy_boto3_proton/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26497 2023-07-13 19:48:23.000000 mypy-boto3-proton-1.28.3/mypy_boto3_proton/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 19:48:23.000000 mypy-boto3-proton-1.28.3/mypy_boto3_proton/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   104634 2023-07-13 19:48:26.000000 mypy-boto3-proton-1.28.3/mypy_boto3_proton/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   104511 2023-07-13 19:48:26.000000 mypy-boto3-proton-1.28.3/mypy_boto3_proton/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-13 19:48:23.000000 mypy-boto3-proton-1.28.3/mypy_boto3_proton/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10159 2023-07-13 19:48:24.000000 mypy-boto3-proton-1.28.3/mypy_boto3_proton/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10149 2023-07-13 19:48:24.000000 mypy-boto3-proton-1.28.3/mypy_boto3_proton/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:49:15.197303 mypy-boto3-proton-1.28.3/mypy_boto3_proton.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    31307 2023-07-13 19:49:15.000000 mypy-boto3-proton-1.28.3/mypy_boto3_proton.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-13 19:49:15.000000 mypy-boto3-proton-1.28.3/mypy_boto3_proton.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 19:49:15.000000 mypy-boto3-proton-1.28.3/mypy_boto3_proton.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 19:49:15.000000 mypy-boto3-proton-1.28.3/mypy_boto3_proton.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-13 19:49:15.000000 mypy-boto3-proton-1.28.3/mypy_boto3_proton.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-13 19:49:15.000000 mypy-boto3-proton-1.28.3/mypy_boto3_proton.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 19:49:15.197303 mypy-boto3-proton-1.28.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-07-13 19:48:23.000000 mypy-boto3-proton-1.28.3/setup.py
```

### Comparing `mypy-boto3-proton-1.28.0/LICENSE` & `mypy-boto3-proton-1.28.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-proton-1.28.0/PKG-INFO` & `mypy-boto3-proton-1.28.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-proton
-Version: 1.28.0
-Summary: Type annotations for boto3.Proton 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.3
+Summary: Type annotations for boto3.Proton 1.28.3 service generated with mypy-boto3-builder 7.14.6
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-proton.svg?color=blue)](https://pypi.org/project/mypy-boto3-proton)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-proton?color=blue)](https://pypistats.org/packages/mypy-boto3-proton)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Proton 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton)
+[boto3.Proton 1.28.3](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton)
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
 [mypy-boto3-proton docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/).
 
 See how it helps to find and fix potential bugs:
 
@@ -283,14 +283,15 @@
 from boto3.session import Session
 
 from mypy_boto3_proton import ProtonClient
 from mypy_boto3_proton.paginator import (
     ListComponentOutputsPaginator,
     ListComponentProvisionedResourcesPaginator,
     ListComponentsPaginator,
+    ListDeploymentsPaginator,
     ListEnvironmentAccountConnectionsPaginator,
     ListEnvironmentOutputsPaginator,
     ListEnvironmentProvisionedResourcesPaginator,
     ListEnvironmentTemplateVersionsPaginator,
     ListEnvironmentTemplatesPaginator,
     ListEnvironmentsPaginator,
     ListRepositoriesPaginator,
@@ -313,14 +314,15 @@
 list_component_outputs_paginator: ListComponentOutputsPaginator = client.get_paginator(
     "list_component_outputs"
 )
 list_component_provisioned_resources_paginator: ListComponentProvisionedResourcesPaginator = (
     client.get_paginator("list_component_provisioned_resources")
 )
 list_components_paginator: ListComponentsPaginator = client.get_paginator("list_components")
+list_deployments_paginator: ListDeploymentsPaginator = client.get_paginator("list_deployments")
 list_environment_account_connections_paginator: ListEnvironmentAccountConnectionsPaginator = (
     client.get_paginator("list_environment_account_connections")
 )
 list_environment_outputs_paginator: ListEnvironmentOutputsPaginator = client.get_paginator(
     "list_environment_outputs"
 )
 list_environment_provisioned_resources_paginator: ListEnvironmentProvisionedResourcesPaginator = (
@@ -422,22 +424,24 @@
 from mypy_boto3_proton.literals import (
     BlockerStatusType,
     BlockerTypeType,
     ComponentDeletedWaiterName,
     ComponentDeployedWaiterName,
     ComponentDeploymentUpdateTypeType,
     DeploymentStatusType,
+    DeploymentTargetResourceTypeType,
     DeploymentUpdateTypeType,
     EnvironmentAccountConnectionRequesterAccountTypeType,
     EnvironmentAccountConnectionStatusType,
     EnvironmentDeployedWaiterName,
     EnvironmentTemplateVersionRegisteredWaiterName,
     ListComponentOutputsPaginatorName,
     ListComponentProvisionedResourcesPaginatorName,
     ListComponentsPaginatorName,
+    ListDeploymentsPaginatorName,
     ListEnvironmentAccountConnectionsPaginatorName,
     ListEnvironmentOutputsPaginatorName,
     ListEnvironmentProvisionedResourcesPaginatorName,
     ListEnvironmentTemplateVersionsPaginatorName,
     ListEnvironmentTemplatesPaginatorName,
     ListEnvironmentsPaginatorName,
     ListRepositoriesPaginatorName,
@@ -501,44 +505,51 @@
     CancelEnvironmentDeploymentInputRequestTypeDef,
     CancelServiceInstanceDeploymentInputRequestTypeDef,
     ServiceInstanceTypeDef,
     CancelServicePipelineDeploymentInputRequestTypeDef,
     ServicePipelineTypeDef,
     CompatibleEnvironmentTemplateInputTypeDef,
     CompatibleEnvironmentTemplateTypeDef,
+    ComponentStateTypeDef,
     ComponentSummaryTypeDef,
     ResourceCountsSummaryTypeDef,
     TagTypeDef,
     RepositoryBranchInputTypeDef,
     EnvironmentTemplateTypeDef,
     EnvironmentTemplateVersionTypeDef,
     RepositoryTypeDef,
     CreateServiceSyncConfigInputRequestTypeDef,
     ServiceSyncConfigTypeDef,
     ServiceTemplateTypeDef,
     CreateTemplateSyncConfigInputRequestTypeDef,
     TemplateSyncConfigTypeDef,
     DeleteComponentInputRequestTypeDef,
+    DeleteDeploymentInputRequestTypeDef,
     DeleteEnvironmentAccountConnectionInputRequestTypeDef,
     DeleteEnvironmentInputRequestTypeDef,
     DeleteEnvironmentTemplateInputRequestTypeDef,
     DeleteEnvironmentTemplateVersionInputRequestTypeDef,
     DeleteRepositoryInputRequestTypeDef,
     DeleteServiceInputRequestTypeDef,
     DeleteServiceSyncConfigInputRequestTypeDef,
     DeleteServiceTemplateInputRequestTypeDef,
     DeleteServiceTemplateVersionInputRequestTypeDef,
     DeleteTemplateSyncConfigInputRequestTypeDef,
+    EnvironmentStateTypeDef,
+    ServiceInstanceStateTypeDef,
+    ServicePipelineStateTypeDef,
+    DeploymentSummaryTypeDef,
     EnvironmentAccountConnectionSummaryTypeDef,
     EnvironmentSummaryTypeDef,
     EnvironmentTemplateFilterTypeDef,
     EnvironmentTemplateSummaryTypeDef,
     EnvironmentTemplateVersionSummaryTypeDef,
     WaiterConfigTypeDef,
     GetComponentInputRequestTypeDef,
+    GetDeploymentInputRequestTypeDef,
     GetEnvironmentAccountConnectionInputRequestTypeDef,
     GetEnvironmentInputRequestTypeDef,
     GetEnvironmentTemplateInputRequestTypeDef,
     GetEnvironmentTemplateVersionInputRequestTypeDef,
     GetRepositoryInputRequestTypeDef,
     GetRepositorySyncStatusInputRequestTypeDef,
     GetServiceInputRequestTypeDef,
@@ -555,14 +566,16 @@
     ListComponentOutputsInputRequestTypeDef,
     OutputTypeDef,
     ListComponentProvisionedResourcesInputListComponentProvisionedResourcesPaginateTypeDef,
     ListComponentProvisionedResourcesInputRequestTypeDef,
     ProvisionedResourceTypeDef,
     ListComponentsInputListComponentsPaginateTypeDef,
     ListComponentsInputRequestTypeDef,
+    ListDeploymentsInputListDeploymentsPaginateTypeDef,
+    ListDeploymentsInputRequestTypeDef,
     ListEnvironmentAccountConnectionsInputListEnvironmentAccountConnectionsPaginateTypeDef,
     ListEnvironmentAccountConnectionsInputRequestTypeDef,
     ListEnvironmentOutputsInputListEnvironmentOutputsPaginateTypeDef,
     ListEnvironmentOutputsInputRequestTypeDef,
     ListEnvironmentProvisionedResourcesInputListEnvironmentProvisionedResourcesPaginateTypeDef,
     ListEnvironmentProvisionedResourcesInputRequestTypeDef,
     ListEnvironmentTemplateVersionsInputListEnvironmentTemplateVersionsPaginateTypeDef,
@@ -670,14 +683,16 @@
     DeleteServiceTemplateOutputTypeDef,
     GetServiceTemplateOutputTypeDef,
     UpdateServiceTemplateOutputTypeDef,
     CreateTemplateSyncConfigOutputTypeDef,
     DeleteTemplateSyncConfigOutputTypeDef,
     GetTemplateSyncConfigOutputTypeDef,
     UpdateTemplateSyncConfigOutputTypeDef,
+    DeploymentStateTypeDef,
+    ListDeploymentsOutputTypeDef,
     ListEnvironmentAccountConnectionsOutputTypeDef,
     ListEnvironmentsOutputTypeDef,
     ListEnvironmentsInputListEnvironmentsPaginateTypeDef,
     ListEnvironmentsInputRequestTypeDef,
     ListEnvironmentTemplatesOutputTypeDef,
     ListEnvironmentTemplateVersionsOutputTypeDef,
     GetComponentInputComponentDeletedWaitTypeDef,
@@ -723,21 +738,24 @@
     GetServiceOutputTypeDef,
     UpdateServiceOutputTypeDef,
     CreateServiceTemplateVersionOutputTypeDef,
     DeleteServiceTemplateVersionOutputTypeDef,
     GetServiceTemplateVersionOutputTypeDef,
     UpdateServiceTemplateVersionOutputTypeDef,
     GetResourcesSummaryOutputTypeDef,
+    DeploymentTypeDef,
     GetRepositorySyncStatusOutputTypeDef,
     GetServiceInstanceSyncStatusOutputTypeDef,
     GetTemplateSyncStatusOutputTypeDef,
     CreateEnvironmentTemplateVersionInputRequestTypeDef,
     CreateServiceTemplateVersionInputRequestTypeDef,
     ServiceSyncBlockerSummaryTypeDef,
     UpdateServiceSyncBlockerOutputTypeDef,
+    DeleteDeploymentOutputTypeDef,
+    GetDeploymentOutputTypeDef,
     GetServiceSyncBlockerSummaryOutputTypeDef,
 )
 
 
 def get_structure() -> AcceptEnvironmentAccountConnectionInputRequestTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-proton-1.28.0/README.md` & `mypy-boto3-proton-1.28.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-proton.svg?color=blue)](https://pypi.org/project/mypy-boto3-proton)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-proton?color=blue)](https://pypistats.org/packages/mypy-boto3-proton)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Proton 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton)
+[boto3.Proton 1.28.3](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton)
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
 [mypy-boto3-proton docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/).
 
 See how it helps to find and fix potential bugs:
 
@@ -251,14 +251,15 @@
 from boto3.session import Session
 
 from mypy_boto3_proton import ProtonClient
 from mypy_boto3_proton.paginator import (
     ListComponentOutputsPaginator,
     ListComponentProvisionedResourcesPaginator,
     ListComponentsPaginator,
+    ListDeploymentsPaginator,
     ListEnvironmentAccountConnectionsPaginator,
     ListEnvironmentOutputsPaginator,
     ListEnvironmentProvisionedResourcesPaginator,
     ListEnvironmentTemplateVersionsPaginator,
     ListEnvironmentTemplatesPaginator,
     ListEnvironmentsPaginator,
     ListRepositoriesPaginator,
@@ -281,14 +282,15 @@
 list_component_outputs_paginator: ListComponentOutputsPaginator = client.get_paginator(
     "list_component_outputs"
 )
 list_component_provisioned_resources_paginator: ListComponentProvisionedResourcesPaginator = (
     client.get_paginator("list_component_provisioned_resources")
 )
 list_components_paginator: ListComponentsPaginator = client.get_paginator("list_components")
+list_deployments_paginator: ListDeploymentsPaginator = client.get_paginator("list_deployments")
 list_environment_account_connections_paginator: ListEnvironmentAccountConnectionsPaginator = (
     client.get_paginator("list_environment_account_connections")
 )
 list_environment_outputs_paginator: ListEnvironmentOutputsPaginator = client.get_paginator(
     "list_environment_outputs"
 )
 list_environment_provisioned_resources_paginator: ListEnvironmentProvisionedResourcesPaginator = (
@@ -390,22 +392,24 @@
 from mypy_boto3_proton.literals import (
     BlockerStatusType,
     BlockerTypeType,
     ComponentDeletedWaiterName,
     ComponentDeployedWaiterName,
     ComponentDeploymentUpdateTypeType,
     DeploymentStatusType,
+    DeploymentTargetResourceTypeType,
     DeploymentUpdateTypeType,
     EnvironmentAccountConnectionRequesterAccountTypeType,
     EnvironmentAccountConnectionStatusType,
     EnvironmentDeployedWaiterName,
     EnvironmentTemplateVersionRegisteredWaiterName,
     ListComponentOutputsPaginatorName,
     ListComponentProvisionedResourcesPaginatorName,
     ListComponentsPaginatorName,
+    ListDeploymentsPaginatorName,
     ListEnvironmentAccountConnectionsPaginatorName,
     ListEnvironmentOutputsPaginatorName,
     ListEnvironmentProvisionedResourcesPaginatorName,
     ListEnvironmentTemplateVersionsPaginatorName,
     ListEnvironmentTemplatesPaginatorName,
     ListEnvironmentsPaginatorName,
     ListRepositoriesPaginatorName,
@@ -469,44 +473,51 @@
     CancelEnvironmentDeploymentInputRequestTypeDef,
     CancelServiceInstanceDeploymentInputRequestTypeDef,
     ServiceInstanceTypeDef,
     CancelServicePipelineDeploymentInputRequestTypeDef,
     ServicePipelineTypeDef,
     CompatibleEnvironmentTemplateInputTypeDef,
     CompatibleEnvironmentTemplateTypeDef,
+    ComponentStateTypeDef,
     ComponentSummaryTypeDef,
     ResourceCountsSummaryTypeDef,
     TagTypeDef,
     RepositoryBranchInputTypeDef,
     EnvironmentTemplateTypeDef,
     EnvironmentTemplateVersionTypeDef,
     RepositoryTypeDef,
     CreateServiceSyncConfigInputRequestTypeDef,
     ServiceSyncConfigTypeDef,
     ServiceTemplateTypeDef,
     CreateTemplateSyncConfigInputRequestTypeDef,
     TemplateSyncConfigTypeDef,
     DeleteComponentInputRequestTypeDef,
+    DeleteDeploymentInputRequestTypeDef,
     DeleteEnvironmentAccountConnectionInputRequestTypeDef,
     DeleteEnvironmentInputRequestTypeDef,
     DeleteEnvironmentTemplateInputRequestTypeDef,
     DeleteEnvironmentTemplateVersionInputRequestTypeDef,
     DeleteRepositoryInputRequestTypeDef,
     DeleteServiceInputRequestTypeDef,
     DeleteServiceSyncConfigInputRequestTypeDef,
     DeleteServiceTemplateInputRequestTypeDef,
     DeleteServiceTemplateVersionInputRequestTypeDef,
     DeleteTemplateSyncConfigInputRequestTypeDef,
+    EnvironmentStateTypeDef,
+    ServiceInstanceStateTypeDef,
+    ServicePipelineStateTypeDef,
+    DeploymentSummaryTypeDef,
     EnvironmentAccountConnectionSummaryTypeDef,
     EnvironmentSummaryTypeDef,
     EnvironmentTemplateFilterTypeDef,
     EnvironmentTemplateSummaryTypeDef,
     EnvironmentTemplateVersionSummaryTypeDef,
     WaiterConfigTypeDef,
     GetComponentInputRequestTypeDef,
+    GetDeploymentInputRequestTypeDef,
     GetEnvironmentAccountConnectionInputRequestTypeDef,
     GetEnvironmentInputRequestTypeDef,
     GetEnvironmentTemplateInputRequestTypeDef,
     GetEnvironmentTemplateVersionInputRequestTypeDef,
     GetRepositoryInputRequestTypeDef,
     GetRepositorySyncStatusInputRequestTypeDef,
     GetServiceInputRequestTypeDef,
@@ -523,14 +534,16 @@
     ListComponentOutputsInputRequestTypeDef,
     OutputTypeDef,
     ListComponentProvisionedResourcesInputListComponentProvisionedResourcesPaginateTypeDef,
     ListComponentProvisionedResourcesInputRequestTypeDef,
     ProvisionedResourceTypeDef,
     ListComponentsInputListComponentsPaginateTypeDef,
     ListComponentsInputRequestTypeDef,
+    ListDeploymentsInputListDeploymentsPaginateTypeDef,
+    ListDeploymentsInputRequestTypeDef,
     ListEnvironmentAccountConnectionsInputListEnvironmentAccountConnectionsPaginateTypeDef,
     ListEnvironmentAccountConnectionsInputRequestTypeDef,
     ListEnvironmentOutputsInputListEnvironmentOutputsPaginateTypeDef,
     ListEnvironmentOutputsInputRequestTypeDef,
     ListEnvironmentProvisionedResourcesInputListEnvironmentProvisionedResourcesPaginateTypeDef,
     ListEnvironmentProvisionedResourcesInputRequestTypeDef,
     ListEnvironmentTemplateVersionsInputListEnvironmentTemplateVersionsPaginateTypeDef,
@@ -638,14 +651,16 @@
     DeleteServiceTemplateOutputTypeDef,
     GetServiceTemplateOutputTypeDef,
     UpdateServiceTemplateOutputTypeDef,
     CreateTemplateSyncConfigOutputTypeDef,
     DeleteTemplateSyncConfigOutputTypeDef,
     GetTemplateSyncConfigOutputTypeDef,
     UpdateTemplateSyncConfigOutputTypeDef,
+    DeploymentStateTypeDef,
+    ListDeploymentsOutputTypeDef,
     ListEnvironmentAccountConnectionsOutputTypeDef,
     ListEnvironmentsOutputTypeDef,
     ListEnvironmentsInputListEnvironmentsPaginateTypeDef,
     ListEnvironmentsInputRequestTypeDef,
     ListEnvironmentTemplatesOutputTypeDef,
     ListEnvironmentTemplateVersionsOutputTypeDef,
     GetComponentInputComponentDeletedWaitTypeDef,
@@ -691,21 +706,24 @@
     GetServiceOutputTypeDef,
     UpdateServiceOutputTypeDef,
     CreateServiceTemplateVersionOutputTypeDef,
     DeleteServiceTemplateVersionOutputTypeDef,
     GetServiceTemplateVersionOutputTypeDef,
     UpdateServiceTemplateVersionOutputTypeDef,
     GetResourcesSummaryOutputTypeDef,
+    DeploymentTypeDef,
     GetRepositorySyncStatusOutputTypeDef,
     GetServiceInstanceSyncStatusOutputTypeDef,
     GetTemplateSyncStatusOutputTypeDef,
     CreateEnvironmentTemplateVersionInputRequestTypeDef,
     CreateServiceTemplateVersionInputRequestTypeDef,
     ServiceSyncBlockerSummaryTypeDef,
     UpdateServiceSyncBlockerOutputTypeDef,
+    DeleteDeploymentOutputTypeDef,
+    GetDeploymentOutputTypeDef,
     GetServiceSyncBlockerSummaryOutputTypeDef,
 )
 
 
 def get_structure() -> AcceptEnvironmentAccountConnectionInputRequestTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-proton-1.28.0/mypy_boto3_proton/__init__.py` & `mypy-boto3-proton-1.28.3/mypy_boto3_proton/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
         ComponentDeletedWaiter,
         ComponentDeployedWaiter,
         EnvironmentDeployedWaiter,
         EnvironmentTemplateVersionRegisteredWaiter,
         ListComponentOutputsPaginator,
         ListComponentProvisionedResourcesPaginator,
         ListComponentsPaginator,
+        ListDeploymentsPaginator,
         ListEnvironmentAccountConnectionsPaginator,
         ListEnvironmentOutputsPaginator,
         ListEnvironmentProvisionedResourcesPaginator,
         ListEnvironmentTemplateVersionsPaginator,
         ListEnvironmentTemplatesPaginator,
         ListEnvironmentsPaginator,
         ListRepositoriesPaginator,
@@ -53,14 +54,15 @@
     service_pipeline_deployed_waiter: ServicePipelineDeployedWaiter = client.get_waiter("service_pipeline_deployed")
     service_template_version_registered_waiter: ServiceTemplateVersionRegisteredWaiter = client.get_waiter("service_template_version_registered")
     service_updated_waiter: ServiceUpdatedWaiter = client.get_waiter("service_updated")
 
     list_component_outputs_paginator: ListComponentOutputsPaginator = client.get_paginator("list_component_outputs")
     list_component_provisioned_resources_paginator: ListComponentProvisionedResourcesPaginator = client.get_paginator("list_component_provisioned_resources")
     list_components_paginator: ListComponentsPaginator = client.get_paginator("list_components")
+    list_deployments_paginator: ListDeploymentsPaginator = client.get_paginator("list_deployments")
     list_environment_account_connections_paginator: ListEnvironmentAccountConnectionsPaginator = client.get_paginator("list_environment_account_connections")
     list_environment_outputs_paginator: ListEnvironmentOutputsPaginator = client.get_paginator("list_environment_outputs")
     list_environment_provisioned_resources_paginator: ListEnvironmentProvisionedResourcesPaginator = client.get_paginator("list_environment_provisioned_resources")
     list_environment_template_versions_paginator: ListEnvironmentTemplateVersionsPaginator = client.get_paginator("list_environment_template_versions")
     list_environment_templates_paginator: ListEnvironmentTemplatesPaginator = client.get_paginator("list_environment_templates")
     list_environments_paginator: ListEnvironmentsPaginator = client.get_paginator("list_environments")
     list_repositories_paginator: ListRepositoriesPaginator = client.get_paginator("list_repositories")
@@ -77,14 +79,15 @@
     ```
 """
 from .client import ProtonClient
 from .paginator import (
     ListComponentOutputsPaginator,
     ListComponentProvisionedResourcesPaginator,
     ListComponentsPaginator,
+    ListDeploymentsPaginator,
     ListEnvironmentAccountConnectionsPaginator,
     ListEnvironmentOutputsPaginator,
     ListEnvironmentProvisionedResourcesPaginator,
     ListEnvironmentsPaginator,
     ListEnvironmentTemplatesPaginator,
     ListEnvironmentTemplateVersionsPaginator,
     ListRepositoriesPaginator,
@@ -120,14 +123,15 @@
     "ComponentDeletedWaiter",
     "ComponentDeployedWaiter",
     "EnvironmentDeployedWaiter",
     "EnvironmentTemplateVersionRegisteredWaiter",
     "ListComponentOutputsPaginator",
     "ListComponentProvisionedResourcesPaginator",
     "ListComponentsPaginator",
+    "ListDeploymentsPaginator",
     "ListEnvironmentAccountConnectionsPaginator",
     "ListEnvironmentOutputsPaginator",
     "ListEnvironmentProvisionedResourcesPaginator",
     "ListEnvironmentTemplateVersionsPaginator",
     "ListEnvironmentTemplatesPaginator",
     "ListEnvironmentsPaginator",
     "ListRepositoriesPaginator",
```

### Comparing `mypy-boto3-proton-1.28.0/mypy_boto3_proton/__init__.pyi` & `mypy-boto3-proton-1.28.3/mypy_boto3_proton/__init__.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
         ComponentDeletedWaiter,
         ComponentDeployedWaiter,
         EnvironmentDeployedWaiter,
         EnvironmentTemplateVersionRegisteredWaiter,
         ListComponentOutputsPaginator,
         ListComponentProvisionedResourcesPaginator,
         ListComponentsPaginator,
+        ListDeploymentsPaginator,
         ListEnvironmentAccountConnectionsPaginator,
         ListEnvironmentOutputsPaginator,
         ListEnvironmentProvisionedResourcesPaginator,
         ListEnvironmentTemplateVersionsPaginator,
         ListEnvironmentTemplatesPaginator,
         ListEnvironmentsPaginator,
         ListRepositoriesPaginator,
@@ -53,14 +54,15 @@
     service_pipeline_deployed_waiter: ServicePipelineDeployedWaiter = client.get_waiter("service_pipeline_deployed")
     service_template_version_registered_waiter: ServiceTemplateVersionRegisteredWaiter = client.get_waiter("service_template_version_registered")
     service_updated_waiter: ServiceUpdatedWaiter = client.get_waiter("service_updated")
 
     list_component_outputs_paginator: ListComponentOutputsPaginator = client.get_paginator("list_component_outputs")
     list_component_provisioned_resources_paginator: ListComponentProvisionedResourcesPaginator = client.get_paginator("list_component_provisioned_resources")
     list_components_paginator: ListComponentsPaginator = client.get_paginator("list_components")
+    list_deployments_paginator: ListDeploymentsPaginator = client.get_paginator("list_deployments")
     list_environment_account_connections_paginator: ListEnvironmentAccountConnectionsPaginator = client.get_paginator("list_environment_account_connections")
     list_environment_outputs_paginator: ListEnvironmentOutputsPaginator = client.get_paginator("list_environment_outputs")
     list_environment_provisioned_resources_paginator: ListEnvironmentProvisionedResourcesPaginator = client.get_paginator("list_environment_provisioned_resources")
     list_environment_template_versions_paginator: ListEnvironmentTemplateVersionsPaginator = client.get_paginator("list_environment_template_versions")
     list_environment_templates_paginator: ListEnvironmentTemplatesPaginator = client.get_paginator("list_environment_templates")
     list_environments_paginator: ListEnvironmentsPaginator = client.get_paginator("list_environments")
     list_repositories_paginator: ListRepositoriesPaginator = client.get_paginator("list_repositories")
@@ -77,14 +79,15 @@
     ```
 """
 from .client import ProtonClient
 from .paginator import (
     ListComponentOutputsPaginator,
     ListComponentProvisionedResourcesPaginator,
     ListComponentsPaginator,
+    ListDeploymentsPaginator,
     ListEnvironmentAccountConnectionsPaginator,
     ListEnvironmentOutputsPaginator,
     ListEnvironmentProvisionedResourcesPaginator,
     ListEnvironmentsPaginator,
     ListEnvironmentTemplatesPaginator,
     ListEnvironmentTemplateVersionsPaginator,
     ListRepositoriesPaginator,
@@ -119,14 +122,15 @@
     "ComponentDeletedWaiter",
     "ComponentDeployedWaiter",
     "EnvironmentDeployedWaiter",
     "EnvironmentTemplateVersionRegisteredWaiter",
     "ListComponentOutputsPaginator",
     "ListComponentProvisionedResourcesPaginator",
     "ListComponentsPaginator",
+    "ListDeploymentsPaginator",
     "ListEnvironmentAccountConnectionsPaginator",
     "ListEnvironmentOutputsPaginator",
     "ListEnvironmentProvisionedResourcesPaginator",
     "ListEnvironmentTemplateVersionsPaginator",
     "ListEnvironmentTemplatesPaginator",
     "ListEnvironmentsPaginator",
     "ListRepositoriesPaginator",
```

### Comparing `mypy-boto3-proton-1.28.0/mypy_boto3_proton/__main__.py` & `mypy-boto3-proton-1.28.3/mypy_boto3_proton/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Proton 1.28.0\nVersion:         1.28.0\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.Proton 1.28.3\nVersion:         1.28.3\nBuilder version:"
+        " 7.14.6\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton\nOther"
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

### Comparing `mypy-boto3-proton-1.28.0/mypy_boto3_proton/client.py` & `mypy-boto3-proton-1.28.3/mypy_boto3_proton/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,14 +31,15 @@
     TemplateTypeType,
     TemplateVersionStatusType,
 )
 from .paginator import (
     ListComponentOutputsPaginator,
     ListComponentProvisionedResourcesPaginator,
     ListComponentsPaginator,
+    ListDeploymentsPaginator,
     ListEnvironmentAccountConnectionsPaginator,
     ListEnvironmentOutputsPaginator,
     ListEnvironmentProvisionedResourcesPaginator,
     ListEnvironmentsPaginator,
     ListEnvironmentTemplatesPaginator,
     ListEnvironmentTemplateVersionsPaginator,
     ListRepositoriesPaginator,
@@ -69,27 +70,29 @@
     CreateServiceInstanceOutputTypeDef,
     CreateServiceOutputTypeDef,
     CreateServiceSyncConfigOutputTypeDef,
     CreateServiceTemplateOutputTypeDef,
     CreateServiceTemplateVersionOutputTypeDef,
     CreateTemplateSyncConfigOutputTypeDef,
     DeleteComponentOutputTypeDef,
+    DeleteDeploymentOutputTypeDef,
     DeleteEnvironmentAccountConnectionOutputTypeDef,
     DeleteEnvironmentOutputTypeDef,
     DeleteEnvironmentTemplateOutputTypeDef,
     DeleteEnvironmentTemplateVersionOutputTypeDef,
     DeleteRepositoryOutputTypeDef,
     DeleteServiceOutputTypeDef,
     DeleteServiceSyncConfigOutputTypeDef,
     DeleteServiceTemplateOutputTypeDef,
     DeleteServiceTemplateVersionOutputTypeDef,
     DeleteTemplateSyncConfigOutputTypeDef,
     EnvironmentTemplateFilterTypeDef,
     GetAccountSettingsOutputTypeDef,
     GetComponentOutputTypeDef,
+    GetDeploymentOutputTypeDef,
     GetEnvironmentAccountConnectionOutputTypeDef,
     GetEnvironmentOutputTypeDef,
     GetEnvironmentTemplateOutputTypeDef,
     GetEnvironmentTemplateVersionOutputTypeDef,
     GetRepositoryOutputTypeDef,
     GetRepositorySyncStatusOutputTypeDef,
     GetResourcesSummaryOutputTypeDef,
@@ -101,14 +104,15 @@
     GetServiceTemplateOutputTypeDef,
     GetServiceTemplateVersionOutputTypeDef,
     GetTemplateSyncConfigOutputTypeDef,
     GetTemplateSyncStatusOutputTypeDef,
     ListComponentOutputsOutputTypeDef,
     ListComponentProvisionedResourcesOutputTypeDef,
     ListComponentsOutputTypeDef,
+    ListDeploymentsOutputTypeDef,
     ListEnvironmentAccountConnectionsOutputTypeDef,
     ListEnvironmentOutputsOutputTypeDef,
     ListEnvironmentProvisionedResourcesOutputTypeDef,
     ListEnvironmentsOutputTypeDef,
     ListEnvironmentTemplatesOutputTypeDef,
     ListEnvironmentTemplateVersionsOutputTypeDef,
     ListRepositoriesOutputTypeDef,
@@ -498,14 +502,22 @@
         """
         Delete an Proton component resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.delete_component)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#delete_component)
         """
 
+    def delete_deployment(self, *, id: str) -> DeleteDeploymentOutputTypeDef:
+        """
+        Delete the deployment.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.delete_deployment)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#delete_deployment)
+        """
+
     def delete_environment(self, *, name: str) -> DeleteEnvironmentOutputTypeDef:
         """
         Delete an environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.delete_environment)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#delete_environment)
         """
@@ -624,14 +636,30 @@
         """
         Get detailed data for a component.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_component)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_component)
         """
 
+    def get_deployment(
+        self,
+        *,
+        id: str,
+        componentName: str = ...,
+        environmentName: str = ...,
+        serviceInstanceName: str = ...,
+        serviceName: str = ...
+    ) -> GetDeploymentOutputTypeDef:
+        """
+        Get detailed data for a deployment.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_deployment)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_deployment)
+        """
+
     def get_environment(self, *, name: str) -> GetEnvironmentOutputTypeDef:
         """
         Get detailed data for an environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_environment)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_environment)
         """
@@ -779,15 +807,15 @@
         Get the status of a template sync.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_template_sync_status)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_template_sync_status)
         """
 
     def list_component_outputs(
-        self, *, componentName: str, nextToken: str = ...
+        self, *, componentName: str, deploymentId: str = ..., nextToken: str = ...
     ) -> ListComponentOutputsOutputTypeDef:
         """
         Get a list of component Infrastructure as Code (IaC) outputs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_component_outputs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#list_component_outputs)
         """
@@ -814,14 +842,31 @@
         """
         List components with summary data.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_components)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#list_components)
         """
 
+    def list_deployments(
+        self,
+        *,
+        componentName: str = ...,
+        environmentName: str = ...,
+        maxResults: int = ...,
+        nextToken: str = ...,
+        serviceInstanceName: str = ...,
+        serviceName: str = ...
+    ) -> ListDeploymentsOutputTypeDef:
+        """
+        List deployments.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_deployments)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#list_deployments)
+        """
+
     def list_environment_account_connections(
         self,
         *,
         requestedBy: EnvironmentAccountConnectionRequesterAccountTypeType,
         environmentName: str = ...,
         maxResults: int = ...,
         nextToken: str = ...,
@@ -831,15 +876,15 @@
         View a list of environment account connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_environment_account_connections)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#list_environment_account_connections)
         """
 
     def list_environment_outputs(
-        self, *, environmentName: str, nextToken: str = ...
+        self, *, environmentName: str, deploymentId: str = ..., nextToken: str = ...
     ) -> ListEnvironmentOutputsOutputTypeDef:
         """
         List the infrastructure as code outputs for your environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_environment_outputs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#list_environment_outputs)
         """
@@ -915,15 +960,20 @@
         List repository sync definitions with detail data.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_repository_sync_definitions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#list_repository_sync_definitions)
         """
 
     def list_service_instance_outputs(
-        self, *, serviceInstanceName: str, serviceName: str, nextToken: str = ...
+        self,
+        *,
+        serviceInstanceName: str,
+        serviceName: str,
+        deploymentId: str = ...,
+        nextToken: str = ...
     ) -> ListServiceInstanceOutputsOutputTypeDef:
         """
         Get a list service of instance Infrastructure as Code (IaC) outputs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_service_instance_outputs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#list_service_instance_outputs)
         """
@@ -952,15 +1002,15 @@
         List service instances with summary data.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_service_instances)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#list_service_instances)
         """
 
     def list_service_pipeline_outputs(
-        self, *, serviceName: str, nextToken: str = ...
+        self, *, serviceName: str, deploymentId: str = ..., nextToken: str = ...
     ) -> ListServicePipelineOutputsOutputTypeDef:
         """
         Get a list of service pipeline Infrastructure as Code (IaC) outputs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_service_pipeline_outputs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#list_service_pipeline_outputs)
         """
@@ -1302,14 +1352,23 @@
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_paginator)
         """
 
     @overload
     def get_paginator(
+        self, operation_name: Literal["list_deployments"]
+    ) -> ListDeploymentsPaginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_paginator)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_paginator)
+        """
+
+    @overload
+    def get_paginator(
         self, operation_name: Literal["list_environment_account_connections"]
     ) -> ListEnvironmentAccountConnectionsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_paginator)
         """
```

### Comparing `mypy-boto3-proton-1.28.0/mypy_boto3_proton/client.pyi` & `mypy-boto3-proton-1.28.3/mypy_boto3_proton/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -31,14 +31,15 @@
     TemplateTypeType,
     TemplateVersionStatusType,
 )
 from .paginator import (
     ListComponentOutputsPaginator,
     ListComponentProvisionedResourcesPaginator,
     ListComponentsPaginator,
+    ListDeploymentsPaginator,
     ListEnvironmentAccountConnectionsPaginator,
     ListEnvironmentOutputsPaginator,
     ListEnvironmentProvisionedResourcesPaginator,
     ListEnvironmentsPaginator,
     ListEnvironmentTemplatesPaginator,
     ListEnvironmentTemplateVersionsPaginator,
     ListRepositoriesPaginator,
@@ -69,27 +70,29 @@
     CreateServiceInstanceOutputTypeDef,
     CreateServiceOutputTypeDef,
     CreateServiceSyncConfigOutputTypeDef,
     CreateServiceTemplateOutputTypeDef,
     CreateServiceTemplateVersionOutputTypeDef,
     CreateTemplateSyncConfigOutputTypeDef,
     DeleteComponentOutputTypeDef,
+    DeleteDeploymentOutputTypeDef,
     DeleteEnvironmentAccountConnectionOutputTypeDef,
     DeleteEnvironmentOutputTypeDef,
     DeleteEnvironmentTemplateOutputTypeDef,
     DeleteEnvironmentTemplateVersionOutputTypeDef,
     DeleteRepositoryOutputTypeDef,
     DeleteServiceOutputTypeDef,
     DeleteServiceSyncConfigOutputTypeDef,
     DeleteServiceTemplateOutputTypeDef,
     DeleteServiceTemplateVersionOutputTypeDef,
     DeleteTemplateSyncConfigOutputTypeDef,
     EnvironmentTemplateFilterTypeDef,
     GetAccountSettingsOutputTypeDef,
     GetComponentOutputTypeDef,
+    GetDeploymentOutputTypeDef,
     GetEnvironmentAccountConnectionOutputTypeDef,
     GetEnvironmentOutputTypeDef,
     GetEnvironmentTemplateOutputTypeDef,
     GetEnvironmentTemplateVersionOutputTypeDef,
     GetRepositoryOutputTypeDef,
     GetRepositorySyncStatusOutputTypeDef,
     GetResourcesSummaryOutputTypeDef,
@@ -101,14 +104,15 @@
     GetServiceTemplateOutputTypeDef,
     GetServiceTemplateVersionOutputTypeDef,
     GetTemplateSyncConfigOutputTypeDef,
     GetTemplateSyncStatusOutputTypeDef,
     ListComponentOutputsOutputTypeDef,
     ListComponentProvisionedResourcesOutputTypeDef,
     ListComponentsOutputTypeDef,
+    ListDeploymentsOutputTypeDef,
     ListEnvironmentAccountConnectionsOutputTypeDef,
     ListEnvironmentOutputsOutputTypeDef,
     ListEnvironmentProvisionedResourcesOutputTypeDef,
     ListEnvironmentsOutputTypeDef,
     ListEnvironmentTemplatesOutputTypeDef,
     ListEnvironmentTemplateVersionsOutputTypeDef,
     ListRepositoriesOutputTypeDef,
@@ -473,14 +477,21 @@
     def delete_component(self, *, name: str) -> DeleteComponentOutputTypeDef:
         """
         Delete an Proton component resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.delete_component)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#delete_component)
         """
+    def delete_deployment(self, *, id: str) -> DeleteDeploymentOutputTypeDef:
+        """
+        Delete the deployment.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.delete_deployment)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#delete_deployment)
+        """
     def delete_environment(self, *, name: str) -> DeleteEnvironmentOutputTypeDef:
         """
         Delete an environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.delete_environment)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#delete_environment)
         """
@@ -586,14 +597,29 @@
     def get_component(self, *, name: str) -> GetComponentOutputTypeDef:
         """
         Get detailed data for a component.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_component)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_component)
         """
+    def get_deployment(
+        self,
+        *,
+        id: str,
+        componentName: str = ...,
+        environmentName: str = ...,
+        serviceInstanceName: str = ...,
+        serviceName: str = ...
+    ) -> GetDeploymentOutputTypeDef:
+        """
+        Get detailed data for a deployment.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_deployment)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_deployment)
+        """
     def get_environment(self, *, name: str) -> GetEnvironmentOutputTypeDef:
         """
         Get detailed data for an environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_environment)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_environment)
         """
@@ -725,15 +751,15 @@
         """
         Get the status of a template sync.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_template_sync_status)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_template_sync_status)
         """
     def list_component_outputs(
-        self, *, componentName: str, nextToken: str = ...
+        self, *, componentName: str, deploymentId: str = ..., nextToken: str = ...
     ) -> ListComponentOutputsOutputTypeDef:
         """
         Get a list of component Infrastructure as Code (IaC) outputs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_component_outputs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#list_component_outputs)
         """
@@ -757,14 +783,30 @@
     ) -> ListComponentsOutputTypeDef:
         """
         List components with summary data.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_components)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#list_components)
         """
+    def list_deployments(
+        self,
+        *,
+        componentName: str = ...,
+        environmentName: str = ...,
+        maxResults: int = ...,
+        nextToken: str = ...,
+        serviceInstanceName: str = ...,
+        serviceName: str = ...
+    ) -> ListDeploymentsOutputTypeDef:
+        """
+        List deployments.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_deployments)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#list_deployments)
+        """
     def list_environment_account_connections(
         self,
         *,
         requestedBy: EnvironmentAccountConnectionRequesterAccountTypeType,
         environmentName: str = ...,
         maxResults: int = ...,
         nextToken: str = ...,
@@ -773,15 +815,15 @@
         """
         View a list of environment account connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_environment_account_connections)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#list_environment_account_connections)
         """
     def list_environment_outputs(
-        self, *, environmentName: str, nextToken: str = ...
+        self, *, environmentName: str, deploymentId: str = ..., nextToken: str = ...
     ) -> ListEnvironmentOutputsOutputTypeDef:
         """
         List the infrastructure as code outputs for your environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_environment_outputs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#list_environment_outputs)
         """
@@ -850,15 +892,20 @@
         """
         List repository sync definitions with detail data.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_repository_sync_definitions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#list_repository_sync_definitions)
         """
     def list_service_instance_outputs(
-        self, *, serviceInstanceName: str, serviceName: str, nextToken: str = ...
+        self,
+        *,
+        serviceInstanceName: str,
+        serviceName: str,
+        deploymentId: str = ...,
+        nextToken: str = ...
     ) -> ListServiceInstanceOutputsOutputTypeDef:
         """
         Get a list service of instance Infrastructure as Code (IaC) outputs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_service_instance_outputs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#list_service_instance_outputs)
         """
@@ -884,15 +931,15 @@
         """
         List service instances with summary data.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_service_instances)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#list_service_instances)
         """
     def list_service_pipeline_outputs(
-        self, *, serviceName: str, nextToken: str = ...
+        self, *, serviceName: str, deploymentId: str = ..., nextToken: str = ...
     ) -> ListServicePipelineOutputsOutputTypeDef:
         """
         Get a list of service pipeline Infrastructure as Code (IaC) outputs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_service_pipeline_outputs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#list_service_pipeline_outputs)
         """
@@ -1207,14 +1254,22 @@
     def get_paginator(self, operation_name: Literal["list_components"]) -> ListComponentsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_paginator)
         """
     @overload
     def get_paginator(
+        self, operation_name: Literal["list_deployments"]
+    ) -> ListDeploymentsPaginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_paginator)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_paginator)
+        """
+    @overload
+    def get_paginator(
         self, operation_name: Literal["list_environment_account_connections"]
     ) -> ListEnvironmentAccountConnectionsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/client/#get_paginator)
         """
     @overload
```

### Comparing `mypy-boto3-proton-1.28.0/mypy_boto3_proton/literals.py` & `mypy-boto3-proton-1.28.3/mypy_boto3_proton/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,22 +22,24 @@
 __all__ = (
     "BlockerStatusType",
     "BlockerTypeType",
     "ComponentDeletedWaiterName",
     "ComponentDeployedWaiterName",
     "ComponentDeploymentUpdateTypeType",
     "DeploymentStatusType",
+    "DeploymentTargetResourceTypeType",
     "DeploymentUpdateTypeType",
     "EnvironmentAccountConnectionRequesterAccountTypeType",
     "EnvironmentAccountConnectionStatusType",
     "EnvironmentDeployedWaiterName",
     "EnvironmentTemplateVersionRegisteredWaiterName",
     "ListComponentOutputsPaginatorName",
     "ListComponentProvisionedResourcesPaginatorName",
     "ListComponentsPaginatorName",
+    "ListDeploymentsPaginatorName",
     "ListEnvironmentAccountConnectionsPaginatorName",
     "ListEnvironmentOutputsPaginatorName",
     "ListEnvironmentProvisionedResourcesPaginatorName",
     "ListEnvironmentTemplateVersionsPaginatorName",
     "ListEnvironmentTemplatesPaginatorName",
     "ListEnvironmentsPaginatorName",
     "ListRepositoriesPaginatorName",
@@ -91,24 +93,28 @@
     "DELETE_COMPLETE",
     "DELETE_FAILED",
     "DELETE_IN_PROGRESS",
     "FAILED",
     "IN_PROGRESS",
     "SUCCEEDED",
 ]
+DeploymentTargetResourceTypeType = Literal[
+    "COMPONENT", "ENVIRONMENT", "SERVICE_INSTANCE", "SERVICE_PIPELINE"
+]
 DeploymentUpdateTypeType = Literal["CURRENT_VERSION", "MAJOR_VERSION", "MINOR_VERSION", "NONE"]
 EnvironmentAccountConnectionRequesterAccountTypeType = Literal[
     "ENVIRONMENT_ACCOUNT", "MANAGEMENT_ACCOUNT"
 ]
 EnvironmentAccountConnectionStatusType = Literal["CONNECTED", "PENDING", "REJECTED"]
 EnvironmentDeployedWaiterName = Literal["environment_deployed"]
 EnvironmentTemplateVersionRegisteredWaiterName = Literal["environment_template_version_registered"]
 ListComponentOutputsPaginatorName = Literal["list_component_outputs"]
 ListComponentProvisionedResourcesPaginatorName = Literal["list_component_provisioned_resources"]
 ListComponentsPaginatorName = Literal["list_components"]
+ListDeploymentsPaginatorName = Literal["list_deployments"]
 ListEnvironmentAccountConnectionsPaginatorName = Literal["list_environment_account_connections"]
 ListEnvironmentOutputsPaginatorName = Literal["list_environment_outputs"]
 ListEnvironmentProvisionedResourcesPaginatorName = Literal["list_environment_provisioned_resources"]
 ListEnvironmentTemplateVersionsPaginatorName = Literal["list_environment_template_versions"]
 ListEnvironmentTemplatesPaginatorName = Literal["list_environment_templates"]
 ListEnvironmentsPaginatorName = Literal["list_environments"]
 ListRepositoriesPaginatorName = Literal["list_repositories"]
@@ -547,14 +553,15 @@
     "sns",
     "sqs",
 ]
 PaginatorName = Literal[
     "list_component_outputs",
     "list_component_provisioned_resources",
     "list_components",
+    "list_deployments",
     "list_environment_account_connections",
     "list_environment_outputs",
     "list_environment_provisioned_resources",
     "list_environment_template_versions",
     "list_environment_templates",
     "list_environments",
     "list_repositories",
```

### Comparing `mypy-boto3-proton-1.28.0/mypy_boto3_proton/literals.pyi` & `mypy-boto3-proton-1.28.3/mypy_boto3_proton/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -21,22 +21,24 @@
 __all__ = (
     "BlockerStatusType",
     "BlockerTypeType",
     "ComponentDeletedWaiterName",
     "ComponentDeployedWaiterName",
     "ComponentDeploymentUpdateTypeType",
     "DeploymentStatusType",
+    "DeploymentTargetResourceTypeType",
     "DeploymentUpdateTypeType",
     "EnvironmentAccountConnectionRequesterAccountTypeType",
     "EnvironmentAccountConnectionStatusType",
     "EnvironmentDeployedWaiterName",
     "EnvironmentTemplateVersionRegisteredWaiterName",
     "ListComponentOutputsPaginatorName",
     "ListComponentProvisionedResourcesPaginatorName",
     "ListComponentsPaginatorName",
+    "ListDeploymentsPaginatorName",
     "ListEnvironmentAccountConnectionsPaginatorName",
     "ListEnvironmentOutputsPaginatorName",
     "ListEnvironmentProvisionedResourcesPaginatorName",
     "ListEnvironmentTemplateVersionsPaginatorName",
     "ListEnvironmentTemplatesPaginatorName",
     "ListEnvironmentsPaginatorName",
     "ListRepositoriesPaginatorName",
@@ -89,24 +91,28 @@
     "DELETE_COMPLETE",
     "DELETE_FAILED",
     "DELETE_IN_PROGRESS",
     "FAILED",
     "IN_PROGRESS",
     "SUCCEEDED",
 ]
+DeploymentTargetResourceTypeType = Literal[
+    "COMPONENT", "ENVIRONMENT", "SERVICE_INSTANCE", "SERVICE_PIPELINE"
+]
 DeploymentUpdateTypeType = Literal["CURRENT_VERSION", "MAJOR_VERSION", "MINOR_VERSION", "NONE"]
 EnvironmentAccountConnectionRequesterAccountTypeType = Literal[
     "ENVIRONMENT_ACCOUNT", "MANAGEMENT_ACCOUNT"
 ]
 EnvironmentAccountConnectionStatusType = Literal["CONNECTED", "PENDING", "REJECTED"]
 EnvironmentDeployedWaiterName = Literal["environment_deployed"]
 EnvironmentTemplateVersionRegisteredWaiterName = Literal["environment_template_version_registered"]
 ListComponentOutputsPaginatorName = Literal["list_component_outputs"]
 ListComponentProvisionedResourcesPaginatorName = Literal["list_component_provisioned_resources"]
 ListComponentsPaginatorName = Literal["list_components"]
+ListDeploymentsPaginatorName = Literal["list_deployments"]
 ListEnvironmentAccountConnectionsPaginatorName = Literal["list_environment_account_connections"]
 ListEnvironmentOutputsPaginatorName = Literal["list_environment_outputs"]
 ListEnvironmentProvisionedResourcesPaginatorName = Literal["list_environment_provisioned_resources"]
 ListEnvironmentTemplateVersionsPaginatorName = Literal["list_environment_template_versions"]
 ListEnvironmentTemplatesPaginatorName = Literal["list_environment_templates"]
 ListEnvironmentsPaginatorName = Literal["list_environments"]
 ListRepositoriesPaginatorName = Literal["list_repositories"]
@@ -545,14 +551,15 @@
     "sns",
     "sqs",
 ]
 PaginatorName = Literal[
     "list_component_outputs",
     "list_component_provisioned_resources",
     "list_components",
+    "list_deployments",
     "list_environment_account_connections",
     "list_environment_outputs",
     "list_environment_provisioned_resources",
     "list_environment_template_versions",
     "list_environment_templates",
     "list_environments",
     "list_repositories",
```

### Comparing `mypy-boto3-proton-1.28.0/mypy_boto3_proton/paginator.py` & `mypy-boto3-proton-1.28.3/mypy_boto3_proton/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
     from boto3.session import Session
 
     from mypy_boto3_proton.client import ProtonClient
     from mypy_boto3_proton.paginator import (
         ListComponentOutputsPaginator,
         ListComponentProvisionedResourcesPaginator,
         ListComponentsPaginator,
+        ListDeploymentsPaginator,
         ListEnvironmentAccountConnectionsPaginator,
         ListEnvironmentOutputsPaginator,
         ListEnvironmentProvisionedResourcesPaginator,
         ListEnvironmentTemplateVersionsPaginator,
         ListEnvironmentTemplatesPaginator,
         ListEnvironmentsPaginator,
         ListRepositoriesPaginator,
@@ -34,14 +35,15 @@
 
     session = Session()
     client: ProtonClient = session.client("proton")
 
     list_component_outputs_paginator: ListComponentOutputsPaginator = client.get_paginator("list_component_outputs")
     list_component_provisioned_resources_paginator: ListComponentProvisionedResourcesPaginator = client.get_paginator("list_component_provisioned_resources")
     list_components_paginator: ListComponentsPaginator = client.get_paginator("list_components")
+    list_deployments_paginator: ListDeploymentsPaginator = client.get_paginator("list_deployments")
     list_environment_account_connections_paginator: ListEnvironmentAccountConnectionsPaginator = client.get_paginator("list_environment_account_connections")
     list_environment_outputs_paginator: ListEnvironmentOutputsPaginator = client.get_paginator("list_environment_outputs")
     list_environment_provisioned_resources_paginator: ListEnvironmentProvisionedResourcesPaginator = client.get_paginator("list_environment_provisioned_resources")
     list_environment_template_versions_paginator: ListEnvironmentTemplateVersionsPaginator = client.get_paginator("list_environment_template_versions")
     list_environment_templates_paginator: ListEnvironmentTemplatesPaginator = client.get_paginator("list_environment_templates")
     list_environments_paginator: ListEnvironmentsPaginator = client.get_paginator("list_environments")
     list_repositories_paginator: ListRepositoriesPaginator = client.get_paginator("list_repositories")
@@ -70,14 +72,15 @@
     SyncTypeType,
 )
 from .type_defs import (
     EnvironmentTemplateFilterTypeDef,
     ListComponentOutputsOutputTypeDef,
     ListComponentProvisionedResourcesOutputTypeDef,
     ListComponentsOutputTypeDef,
+    ListDeploymentsOutputTypeDef,
     ListEnvironmentAccountConnectionsOutputTypeDef,
     ListEnvironmentOutputsOutputTypeDef,
     ListEnvironmentProvisionedResourcesOutputTypeDef,
     ListEnvironmentsOutputTypeDef,
     ListEnvironmentTemplatesOutputTypeDef,
     ListEnvironmentTemplateVersionsOutputTypeDef,
     ListRepositoriesOutputTypeDef,
@@ -95,14 +98,15 @@
     PaginatorConfigTypeDef,
 )
 
 __all__ = (
     "ListComponentOutputsPaginator",
     "ListComponentProvisionedResourcesPaginator",
     "ListComponentsPaginator",
+    "ListDeploymentsPaginator",
     "ListEnvironmentAccountConnectionsPaginator",
     "ListEnvironmentOutputsPaginator",
     "ListEnvironmentProvisionedResourcesPaginator",
     "ListEnvironmentTemplateVersionsPaginator",
     "ListEnvironmentTemplatesPaginator",
     "ListEnvironmentsPaginator",
     "ListRepositoriesPaginator",
@@ -132,15 +136,19 @@
 class ListComponentOutputsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListComponentOutputs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listcomponentoutputspaginator)
     """
 
     def paginate(
-        self, *, componentName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self,
+        *,
+        componentName: str,
+        deploymentId: str = ...,
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListComponentOutputsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListComponentOutputs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listcomponentoutputspaginator)
         """
 
 
@@ -175,14 +183,35 @@
     ) -> _PageIterator[ListComponentsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListComponents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listcomponentspaginator)
         """
 
 
+class ListDeploymentsPaginator(Paginator):
+    """
+    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListDeployments)
+    [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listdeploymentspaginator)
+    """
+
+    def paginate(
+        self,
+        *,
+        componentName: str = ...,
+        environmentName: str = ...,
+        serviceInstanceName: str = ...,
+        serviceName: str = ...,
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
+    ) -> _PageIterator[ListDeploymentsOutputTypeDef]:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListDeployments.paginate)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listdeploymentspaginator)
+        """
+
+
 class ListEnvironmentAccountConnectionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListEnvironmentAccountConnections)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listenvironmentaccountconnectionspaginator)
     """
 
     def paginate(
@@ -202,15 +231,19 @@
 class ListEnvironmentOutputsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListEnvironmentOutputs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listenvironmentoutputspaginator)
     """
 
     def paginate(
-        self, *, environmentName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self,
+        *,
+        environmentName: str,
+        deploymentId: str = ...,
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListEnvironmentOutputsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListEnvironmentOutputs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listenvironmentoutputspaginator)
         """
 
 
@@ -323,14 +356,15 @@
     """
 
     def paginate(
         self,
         *,
         serviceInstanceName: str,
         serviceName: str,
+        deploymentId: str = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListServiceInstanceOutputsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListServiceInstanceOutputs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listserviceinstanceoutputspaginator)
         """
 
@@ -378,15 +412,19 @@
 class ListServicePipelineOutputsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListServicePipelineOutputs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listservicepipelineoutputspaginator)
     """
 
     def paginate(
-        self, *, serviceName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self,
+        *,
+        serviceName: str,
+        deploymentId: str = ...,
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListServicePipelineOutputsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListServicePipelineOutputs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listservicepipelineoutputspaginator)
         """
```

### Comparing `mypy-boto3-proton-1.28.0/mypy_boto3_proton/paginator.pyi` & `mypy-boto3-proton-1.28.3/mypy_boto3_proton/paginator.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -9,14 +9,15 @@
     from boto3.session import Session
 
     from mypy_boto3_proton.client import ProtonClient
     from mypy_boto3_proton.paginator import (
         ListComponentOutputsPaginator,
         ListComponentProvisionedResourcesPaginator,
         ListComponentsPaginator,
+        ListDeploymentsPaginator,
         ListEnvironmentAccountConnectionsPaginator,
         ListEnvironmentOutputsPaginator,
         ListEnvironmentProvisionedResourcesPaginator,
         ListEnvironmentTemplateVersionsPaginator,
         ListEnvironmentTemplatesPaginator,
         ListEnvironmentsPaginator,
         ListRepositoriesPaginator,
@@ -34,14 +35,15 @@
 
     session = Session()
     client: ProtonClient = session.client("proton")
 
     list_component_outputs_paginator: ListComponentOutputsPaginator = client.get_paginator("list_component_outputs")
     list_component_provisioned_resources_paginator: ListComponentProvisionedResourcesPaginator = client.get_paginator("list_component_provisioned_resources")
     list_components_paginator: ListComponentsPaginator = client.get_paginator("list_components")
+    list_deployments_paginator: ListDeploymentsPaginator = client.get_paginator("list_deployments")
     list_environment_account_connections_paginator: ListEnvironmentAccountConnectionsPaginator = client.get_paginator("list_environment_account_connections")
     list_environment_outputs_paginator: ListEnvironmentOutputsPaginator = client.get_paginator("list_environment_outputs")
     list_environment_provisioned_resources_paginator: ListEnvironmentProvisionedResourcesPaginator = client.get_paginator("list_environment_provisioned_resources")
     list_environment_template_versions_paginator: ListEnvironmentTemplateVersionsPaginator = client.get_paginator("list_environment_template_versions")
     list_environment_templates_paginator: ListEnvironmentTemplatesPaginator = client.get_paginator("list_environment_templates")
     list_environments_paginator: ListEnvironmentsPaginator = client.get_paginator("list_environments")
     list_repositories_paginator: ListRepositoriesPaginator = client.get_paginator("list_repositories")
@@ -70,14 +72,15 @@
     SyncTypeType,
 )
 from .type_defs import (
     EnvironmentTemplateFilterTypeDef,
     ListComponentOutputsOutputTypeDef,
     ListComponentProvisionedResourcesOutputTypeDef,
     ListComponentsOutputTypeDef,
+    ListDeploymentsOutputTypeDef,
     ListEnvironmentAccountConnectionsOutputTypeDef,
     ListEnvironmentOutputsOutputTypeDef,
     ListEnvironmentProvisionedResourcesOutputTypeDef,
     ListEnvironmentsOutputTypeDef,
     ListEnvironmentTemplatesOutputTypeDef,
     ListEnvironmentTemplateVersionsOutputTypeDef,
     ListRepositoriesOutputTypeDef,
@@ -95,14 +98,15 @@
     PaginatorConfigTypeDef,
 )
 
 __all__ = (
     "ListComponentOutputsPaginator",
     "ListComponentProvisionedResourcesPaginator",
     "ListComponentsPaginator",
+    "ListDeploymentsPaginator",
     "ListEnvironmentAccountConnectionsPaginator",
     "ListEnvironmentOutputsPaginator",
     "ListEnvironmentProvisionedResourcesPaginator",
     "ListEnvironmentTemplateVersionsPaginator",
     "ListEnvironmentTemplatesPaginator",
     "ListEnvironmentsPaginator",
     "ListRepositoriesPaginator",
@@ -129,15 +133,19 @@
 class ListComponentOutputsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListComponentOutputs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listcomponentoutputspaginator)
     """
 
     def paginate(
-        self, *, componentName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self,
+        *,
+        componentName: str,
+        deploymentId: str = ...,
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListComponentOutputsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListComponentOutputs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listcomponentoutputspaginator)
         """
 
 class ListComponentProvisionedResourcesPaginator(Paginator):
@@ -169,14 +177,34 @@
         PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListComponentsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListComponents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listcomponentspaginator)
         """
 
+class ListDeploymentsPaginator(Paginator):
+    """
+    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListDeployments)
+    [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listdeploymentspaginator)
+    """
+
+    def paginate(
+        self,
+        *,
+        componentName: str = ...,
+        environmentName: str = ...,
+        serviceInstanceName: str = ...,
+        serviceName: str = ...,
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
+    ) -> _PageIterator[ListDeploymentsOutputTypeDef]:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListDeployments.paginate)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listdeploymentspaginator)
+        """
+
 class ListEnvironmentAccountConnectionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListEnvironmentAccountConnections)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listenvironmentaccountconnectionspaginator)
     """
 
     def paginate(
@@ -195,15 +223,19 @@
 class ListEnvironmentOutputsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListEnvironmentOutputs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listenvironmentoutputspaginator)
     """
 
     def paginate(
-        self, *, environmentName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self,
+        *,
+        environmentName: str,
+        deploymentId: str = ...,
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListEnvironmentOutputsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListEnvironmentOutputs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listenvironmentoutputspaginator)
         """
 
 class ListEnvironmentProvisionedResourcesPaginator(Paginator):
@@ -309,14 +341,15 @@
     """
 
     def paginate(
         self,
         *,
         serviceInstanceName: str,
         serviceName: str,
+        deploymentId: str = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListServiceInstanceOutputsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListServiceInstanceOutputs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listserviceinstanceoutputspaginator)
         """
 
@@ -361,15 +394,19 @@
 class ListServicePipelineOutputsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListServicePipelineOutputs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listservicepipelineoutputspaginator)
     """
 
     def paginate(
-        self, *, serviceName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self,
+        *,
+        serviceName: str,
+        deploymentId: str = ...,
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListServicePipelineOutputsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListServicePipelineOutputs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/paginators/#listservicepipelineoutputspaginator)
         """
 
 class ListServicePipelineProvisionedResourcesPaginator(Paginator):
```

### Comparing `mypy-boto3-proton-1.28.0/mypy_boto3_proton/type_defs.py` & `mypy-boto3-proton-1.28.3/mypy_boto3_proton/type_defs.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 from datetime import datetime
 from typing import Dict, List, Sequence
 
 from .literals import (
     BlockerStatusType,
     ComponentDeploymentUpdateTypeType,
     DeploymentStatusType,
+    DeploymentTargetResourceTypeType,
     DeploymentUpdateTypeType,
     EnvironmentAccountConnectionRequesterAccountTypeType,
     EnvironmentAccountConnectionStatusType,
     ListServiceInstancesFilterByType,
     ListServiceInstancesSortByType,
     ProvisionedResourceEngineType,
     RepositoryProviderType,
@@ -55,44 +56,51 @@
     "CancelEnvironmentDeploymentInputRequestTypeDef",
     "CancelServiceInstanceDeploymentInputRequestTypeDef",
     "ServiceInstanceTypeDef",
     "CancelServicePipelineDeploymentInputRequestTypeDef",
     "ServicePipelineTypeDef",
     "CompatibleEnvironmentTemplateInputTypeDef",
     "CompatibleEnvironmentTemplateTypeDef",
+    "ComponentStateTypeDef",
     "ComponentSummaryTypeDef",
     "ResourceCountsSummaryTypeDef",
     "TagTypeDef",
     "RepositoryBranchInputTypeDef",
     "EnvironmentTemplateTypeDef",
     "EnvironmentTemplateVersionTypeDef",
     "RepositoryTypeDef",
     "CreateServiceSyncConfigInputRequestTypeDef",
     "ServiceSyncConfigTypeDef",
     "ServiceTemplateTypeDef",
     "CreateTemplateSyncConfigInputRequestTypeDef",
     "TemplateSyncConfigTypeDef",
     "DeleteComponentInputRequestTypeDef",
+    "DeleteDeploymentInputRequestTypeDef",
     "DeleteEnvironmentAccountConnectionInputRequestTypeDef",
     "DeleteEnvironmentInputRequestTypeDef",
     "DeleteEnvironmentTemplateInputRequestTypeDef",
     "DeleteEnvironmentTemplateVersionInputRequestTypeDef",
     "DeleteRepositoryInputRequestTypeDef",
     "DeleteServiceInputRequestTypeDef",
     "DeleteServiceSyncConfigInputRequestTypeDef",
     "DeleteServiceTemplateInputRequestTypeDef",
     "DeleteServiceTemplateVersionInputRequestTypeDef",
     "DeleteTemplateSyncConfigInputRequestTypeDef",
+    "EnvironmentStateTypeDef",
+    "ServiceInstanceStateTypeDef",
+    "ServicePipelineStateTypeDef",
+    "DeploymentSummaryTypeDef",
     "EnvironmentAccountConnectionSummaryTypeDef",
     "EnvironmentSummaryTypeDef",
     "EnvironmentTemplateFilterTypeDef",
     "EnvironmentTemplateSummaryTypeDef",
     "EnvironmentTemplateVersionSummaryTypeDef",
     "WaiterConfigTypeDef",
     "GetComponentInputRequestTypeDef",
+    "GetDeploymentInputRequestTypeDef",
     "GetEnvironmentAccountConnectionInputRequestTypeDef",
     "GetEnvironmentInputRequestTypeDef",
     "GetEnvironmentTemplateInputRequestTypeDef",
     "GetEnvironmentTemplateVersionInputRequestTypeDef",
     "GetRepositoryInputRequestTypeDef",
     "GetRepositorySyncStatusInputRequestTypeDef",
     "GetServiceInputRequestTypeDef",
@@ -109,14 +117,16 @@
     "ListComponentOutputsInputRequestTypeDef",
     "OutputTypeDef",
     "ListComponentProvisionedResourcesInputListComponentProvisionedResourcesPaginateTypeDef",
     "ListComponentProvisionedResourcesInputRequestTypeDef",
     "ProvisionedResourceTypeDef",
     "ListComponentsInputListComponentsPaginateTypeDef",
     "ListComponentsInputRequestTypeDef",
+    "ListDeploymentsInputListDeploymentsPaginateTypeDef",
+    "ListDeploymentsInputRequestTypeDef",
     "ListEnvironmentAccountConnectionsInputListEnvironmentAccountConnectionsPaginateTypeDef",
     "ListEnvironmentAccountConnectionsInputRequestTypeDef",
     "ListEnvironmentOutputsInputListEnvironmentOutputsPaginateTypeDef",
     "ListEnvironmentOutputsInputRequestTypeDef",
     "ListEnvironmentProvisionedResourcesInputListEnvironmentProvisionedResourcesPaginateTypeDef",
     "ListEnvironmentProvisionedResourcesInputRequestTypeDef",
     "ListEnvironmentTemplateVersionsInputListEnvironmentTemplateVersionsPaginateTypeDef",
@@ -224,14 +234,16 @@
     "DeleteServiceTemplateOutputTypeDef",
     "GetServiceTemplateOutputTypeDef",
     "UpdateServiceTemplateOutputTypeDef",
     "CreateTemplateSyncConfigOutputTypeDef",
     "DeleteTemplateSyncConfigOutputTypeDef",
     "GetTemplateSyncConfigOutputTypeDef",
     "UpdateTemplateSyncConfigOutputTypeDef",
+    "DeploymentStateTypeDef",
+    "ListDeploymentsOutputTypeDef",
     "ListEnvironmentAccountConnectionsOutputTypeDef",
     "ListEnvironmentsOutputTypeDef",
     "ListEnvironmentsInputListEnvironmentsPaginateTypeDef",
     "ListEnvironmentsInputRequestTypeDef",
     "ListEnvironmentTemplatesOutputTypeDef",
     "ListEnvironmentTemplateVersionsOutputTypeDef",
     "GetComponentInputComponentDeletedWaitTypeDef",
@@ -277,60 +289,50 @@
     "GetServiceOutputTypeDef",
     "UpdateServiceOutputTypeDef",
     "CreateServiceTemplateVersionOutputTypeDef",
     "DeleteServiceTemplateVersionOutputTypeDef",
     "GetServiceTemplateVersionOutputTypeDef",
     "UpdateServiceTemplateVersionOutputTypeDef",
     "GetResourcesSummaryOutputTypeDef",
+    "DeploymentTypeDef",
     "GetRepositorySyncStatusOutputTypeDef",
     "GetServiceInstanceSyncStatusOutputTypeDef",
     "GetTemplateSyncStatusOutputTypeDef",
     "CreateEnvironmentTemplateVersionInputRequestTypeDef",
     "CreateServiceTemplateVersionInputRequestTypeDef",
     "ServiceSyncBlockerSummaryTypeDef",
     "UpdateServiceSyncBlockerOutputTypeDef",
+    "DeleteDeploymentOutputTypeDef",
+    "GetDeploymentOutputTypeDef",
     "GetServiceSyncBlockerSummaryOutputTypeDef",
 )
 
 AcceptEnvironmentAccountConnectionInputRequestTypeDef = TypedDict(
     "AcceptEnvironmentAccountConnectionInputRequestTypeDef",
     {
         "id": str,
     },
 )
 
-_RequiredEnvironmentAccountConnectionTypeDef = TypedDict(
-    "_RequiredEnvironmentAccountConnectionTypeDef",
+EnvironmentAccountConnectionTypeDef = TypedDict(
+    "EnvironmentAccountConnectionTypeDef",
     {
         "arn": str,
+        "codebuildRoleArn": str,
+        "componentRoleArn": str,
         "environmentAccountId": str,
         "environmentName": str,
         "id": str,
         "lastModifiedAt": datetime,
         "managementAccountId": str,
         "requestedAt": datetime,
         "roleArn": str,
         "status": EnvironmentAccountConnectionStatusType,
     },
 )
-_OptionalEnvironmentAccountConnectionTypeDef = TypedDict(
-    "_OptionalEnvironmentAccountConnectionTypeDef",
-    {
-        "codebuildRoleArn": str,
-        "componentRoleArn": str,
-    },
-    total=False,
-)
-
-
-class EnvironmentAccountConnectionTypeDef(
-    _RequiredEnvironmentAccountConnectionTypeDef, _OptionalEnvironmentAccountConnectionTypeDef
-):
-    pass
-
 
 RepositoryBranchTypeDef = TypedDict(
     "RepositoryBranchTypeDef",
     {
         "arn": str,
         "branch": str,
         "name": str,
@@ -341,45 +343,36 @@
 CancelComponentDeploymentInputRequestTypeDef = TypedDict(
     "CancelComponentDeploymentInputRequestTypeDef",
     {
         "componentName": str,
     },
 )
 
-_RequiredComponentTypeDef = TypedDict(
-    "_RequiredComponentTypeDef",
+ComponentTypeDef = TypedDict(
+    "ComponentTypeDef",
     {
         "arn": str,
         "createdAt": datetime,
         "deploymentStatus": DeploymentStatusType,
-        "environmentName": str,
-        "lastModifiedAt": datetime,
-        "name": str,
-    },
-)
-_OptionalComponentTypeDef = TypedDict(
-    "_OptionalComponentTypeDef",
-    {
         "deploymentStatusMessage": str,
         "description": str,
+        "environmentName": str,
+        "lastAttemptedDeploymentId": str,
         "lastClientRequestToken": str,
         "lastDeploymentAttemptedAt": datetime,
         "lastDeploymentSucceededAt": datetime,
+        "lastModifiedAt": datetime,
+        "lastSucceededDeploymentId": str,
+        "name": str,
         "serviceInstanceName": str,
         "serviceName": str,
         "serviceSpec": str,
     },
-    total=False,
 )
 
-
-class ComponentTypeDef(_RequiredComponentTypeDef, _OptionalComponentTypeDef):
-    pass
-
-
 CancelEnvironmentDeploymentInputRequestTypeDef = TypedDict(
     "CancelEnvironmentDeploymentInputRequestTypeDef",
     {
         "environmentName": str,
     },
 )
 
@@ -387,78 +380,60 @@
     "CancelServiceInstanceDeploymentInputRequestTypeDef",
     {
         "serviceInstanceName": str,
         "serviceName": str,
     },
 )
 
-_RequiredServiceInstanceTypeDef = TypedDict(
-    "_RequiredServiceInstanceTypeDef",
+ServiceInstanceTypeDef = TypedDict(
+    "ServiceInstanceTypeDef",
     {
         "arn": str,
         "createdAt": datetime,
         "deploymentStatus": DeploymentStatusType,
+        "deploymentStatusMessage": str,
         "environmentName": str,
+        "lastAttemptedDeploymentId": str,
+        "lastClientRequestToken": str,
         "lastDeploymentAttemptedAt": datetime,
         "lastDeploymentSucceededAt": datetime,
+        "lastSucceededDeploymentId": str,
         "name": str,
         "serviceName": str,
+        "spec": str,
         "templateMajorVersion": str,
         "templateMinorVersion": str,
         "templateName": str,
     },
 )
-_OptionalServiceInstanceTypeDef = TypedDict(
-    "_OptionalServiceInstanceTypeDef",
-    {
-        "deploymentStatusMessage": str,
-        "lastClientRequestToken": str,
-        "spec": str,
-    },
-    total=False,
-)
-
-
-class ServiceInstanceTypeDef(_RequiredServiceInstanceTypeDef, _OptionalServiceInstanceTypeDef):
-    pass
-
 
 CancelServicePipelineDeploymentInputRequestTypeDef = TypedDict(
     "CancelServicePipelineDeploymentInputRequestTypeDef",
     {
         "serviceName": str,
     },
 )
 
-_RequiredServicePipelineTypeDef = TypedDict(
-    "_RequiredServicePipelineTypeDef",
+ServicePipelineTypeDef = TypedDict(
+    "ServicePipelineTypeDef",
     {
         "arn": str,
         "createdAt": datetime,
         "deploymentStatus": DeploymentStatusType,
+        "deploymentStatusMessage": str,
+        "lastAttemptedDeploymentId": str,
         "lastDeploymentAttemptedAt": datetime,
         "lastDeploymentSucceededAt": datetime,
+        "lastSucceededDeploymentId": str,
+        "spec": str,
         "templateMajorVersion": str,
         "templateMinorVersion": str,
         "templateName": str,
     },
 )
-_OptionalServicePipelineTypeDef = TypedDict(
-    "_OptionalServicePipelineTypeDef",
-    {
-        "deploymentStatusMessage": str,
-        "spec": str,
-    },
-    total=False,
-)
-
-
-class ServicePipelineTypeDef(_RequiredServicePipelineTypeDef, _OptionalServicePipelineTypeDef):
-    pass
-
 
 CompatibleEnvironmentTemplateInputTypeDef = TypedDict(
     "CompatibleEnvironmentTemplateInputTypeDef",
     {
         "majorVersion": str,
         "templateName": str,
     },
@@ -468,66 +443,54 @@
     "CompatibleEnvironmentTemplateTypeDef",
     {
         "majorVersion": str,
         "templateName": str,
     },
 )
 
-_RequiredComponentSummaryTypeDef = TypedDict(
-    "_RequiredComponentSummaryTypeDef",
+ComponentStateTypeDef = TypedDict(
+    "ComponentStateTypeDef",
     {
-        "arn": str,
-        "createdAt": datetime,
-        "deploymentStatus": DeploymentStatusType,
-        "environmentName": str,
-        "lastModifiedAt": datetime,
-        "name": str,
+        "serviceInstanceName": str,
+        "serviceName": str,
+        "serviceSpec": str,
+        "templateFile": str,
     },
 )
-_OptionalComponentSummaryTypeDef = TypedDict(
-    "_OptionalComponentSummaryTypeDef",
+
+ComponentSummaryTypeDef = TypedDict(
+    "ComponentSummaryTypeDef",
     {
+        "arn": str,
+        "createdAt": datetime,
+        "deploymentStatus": DeploymentStatusType,
         "deploymentStatusMessage": str,
+        "environmentName": str,
+        "lastAttemptedDeploymentId": str,
         "lastDeploymentAttemptedAt": datetime,
         "lastDeploymentSucceededAt": datetime,
+        "lastModifiedAt": datetime,
+        "lastSucceededDeploymentId": str,
+        "name": str,
         "serviceInstanceName": str,
         "serviceName": str,
     },
-    total=False,
 )
 
-
-class ComponentSummaryTypeDef(_RequiredComponentSummaryTypeDef, _OptionalComponentSummaryTypeDef):
-    pass
-
-
-_RequiredResourceCountsSummaryTypeDef = TypedDict(
-    "_RequiredResourceCountsSummaryTypeDef",
-    {
-        "total": int,
-    },
-)
-_OptionalResourceCountsSummaryTypeDef = TypedDict(
-    "_OptionalResourceCountsSummaryTypeDef",
+ResourceCountsSummaryTypeDef = TypedDict(
+    "ResourceCountsSummaryTypeDef",
     {
         "behindMajor": int,
         "behindMinor": int,
         "failed": int,
+        "total": int,
         "upToDate": int,
     },
-    total=False,
 )
 
-
-class ResourceCountsSummaryTypeDef(
-    _RequiredResourceCountsSummaryTypeDef, _OptionalResourceCountsSummaryTypeDef
-):
-    pass
-
-
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "key": str,
         "value": str,
     },
 )
@@ -537,93 +500,56 @@
     {
         "branch": str,
         "name": str,
         "provider": RepositoryProviderType,
     },
 )
 
-_RequiredEnvironmentTemplateTypeDef = TypedDict(
-    "_RequiredEnvironmentTemplateTypeDef",
+EnvironmentTemplateTypeDef = TypedDict(
+    "EnvironmentTemplateTypeDef",
     {
         "arn": str,
         "createdAt": datetime,
-        "lastModifiedAt": datetime,
-        "name": str,
-    },
-)
-_OptionalEnvironmentTemplateTypeDef = TypedDict(
-    "_OptionalEnvironmentTemplateTypeDef",
-    {
         "description": str,
         "displayName": str,
         "encryptionKey": str,
+        "lastModifiedAt": datetime,
+        "name": str,
         "provisioning": Literal["CUSTOMER_MANAGED"],
         "recommendedVersion": str,
     },
-    total=False,
 )
 
-
-class EnvironmentTemplateTypeDef(
-    _RequiredEnvironmentTemplateTypeDef, _OptionalEnvironmentTemplateTypeDef
-):
-    pass
-
-
-_RequiredEnvironmentTemplateVersionTypeDef = TypedDict(
-    "_RequiredEnvironmentTemplateVersionTypeDef",
+EnvironmentTemplateVersionTypeDef = TypedDict(
+    "EnvironmentTemplateVersionTypeDef",
     {
         "arn": str,
         "createdAt": datetime,
+        "description": str,
         "lastModifiedAt": datetime,
         "majorVersion": str,
         "minorVersion": str,
-        "status": TemplateVersionStatusType,
-        "templateName": str,
-    },
-)
-_OptionalEnvironmentTemplateVersionTypeDef = TypedDict(
-    "_OptionalEnvironmentTemplateVersionTypeDef",
-    {
-        "description": str,
         "recommendedMinorVersion": str,
         "schema": str,
+        "status": TemplateVersionStatusType,
         "statusMessage": str,
+        "templateName": str,
     },
-    total=False,
 )
 
-
-class EnvironmentTemplateVersionTypeDef(
-    _RequiredEnvironmentTemplateVersionTypeDef, _OptionalEnvironmentTemplateVersionTypeDef
-):
-    pass
-
-
-_RequiredRepositoryTypeDef = TypedDict(
-    "_RequiredRepositoryTypeDef",
+RepositoryTypeDef = TypedDict(
+    "RepositoryTypeDef",
     {
         "arn": str,
         "connectionArn": str,
+        "encryptionKey": str,
         "name": str,
         "provider": RepositoryProviderType,
     },
 )
-_OptionalRepositoryTypeDef = TypedDict(
-    "_OptionalRepositoryTypeDef",
-    {
-        "encryptionKey": str,
-    },
-    total=False,
-)
-
-
-class RepositoryTypeDef(_RequiredRepositoryTypeDef, _OptionalRepositoryTypeDef):
-    pass
-
 
 CreateServiceSyncConfigInputRequestTypeDef = TypedDict(
     "CreateServiceSyncConfigInputRequestTypeDef",
     {
         "branch": str,
         "filePath": str,
         "repositoryName": str,
@@ -639,40 +565,29 @@
         "filePath": str,
         "repositoryName": str,
         "repositoryProvider": RepositoryProviderType,
         "serviceName": str,
     },
 )
 
-_RequiredServiceTemplateTypeDef = TypedDict(
-    "_RequiredServiceTemplateTypeDef",
+ServiceTemplateTypeDef = TypedDict(
+    "ServiceTemplateTypeDef",
     {
         "arn": str,
         "createdAt": datetime,
-        "lastModifiedAt": datetime,
-        "name": str,
-    },
-)
-_OptionalServiceTemplateTypeDef = TypedDict(
-    "_OptionalServiceTemplateTypeDef",
-    {
         "description": str,
         "displayName": str,
         "encryptionKey": str,
+        "lastModifiedAt": datetime,
+        "name": str,
         "pipelineProvisioning": Literal["CUSTOMER_MANAGED"],
         "recommendedVersion": str,
     },
-    total=False,
 )
 
-
-class ServiceTemplateTypeDef(_RequiredServiceTemplateTypeDef, _OptionalServiceTemplateTypeDef):
-    pass
-
-
 _RequiredCreateTemplateSyncConfigInputRequestTypeDef = TypedDict(
     "_RequiredCreateTemplateSyncConfigInputRequestTypeDef",
     {
         "branch": str,
         "repositoryName": str,
         "repositoryProvider": RepositoryProviderType,
         "templateName": str,
@@ -691,46 +606,40 @@
 class CreateTemplateSyncConfigInputRequestTypeDef(
     _RequiredCreateTemplateSyncConfigInputRequestTypeDef,
     _OptionalCreateTemplateSyncConfigInputRequestTypeDef,
 ):
     pass
 
 
-_RequiredTemplateSyncConfigTypeDef = TypedDict(
-    "_RequiredTemplateSyncConfigTypeDef",
+TemplateSyncConfigTypeDef = TypedDict(
+    "TemplateSyncConfigTypeDef",
     {
         "branch": str,
         "repositoryName": str,
         "repositoryProvider": RepositoryProviderType,
+        "subdirectory": str,
         "templateName": str,
         "templateType": TemplateTypeType,
     },
 )
-_OptionalTemplateSyncConfigTypeDef = TypedDict(
-    "_OptionalTemplateSyncConfigTypeDef",
-    {
-        "subdirectory": str,
-    },
-    total=False,
-)
-
-
-class TemplateSyncConfigTypeDef(
-    _RequiredTemplateSyncConfigTypeDef, _OptionalTemplateSyncConfigTypeDef
-):
-    pass
-
 
 DeleteComponentInputRequestTypeDef = TypedDict(
     "DeleteComponentInputRequestTypeDef",
     {
         "name": str,
     },
 )
 
+DeleteDeploymentInputRequestTypeDef = TypedDict(
+    "DeleteDeploymentInputRequestTypeDef",
+    {
+        "id": str,
+    },
+)
+
 DeleteEnvironmentAccountConnectionInputRequestTypeDef = TypedDict(
     "DeleteEnvironmentAccountConnectionInputRequestTypeDef",
     {
         "id": str,
     },
 )
 
@@ -799,144 +708,146 @@
     "DeleteTemplateSyncConfigInputRequestTypeDef",
     {
         "templateName": str,
         "templateType": TemplateTypeType,
     },
 )
 
-_RequiredEnvironmentAccountConnectionSummaryTypeDef = TypedDict(
-    "_RequiredEnvironmentAccountConnectionSummaryTypeDef",
+EnvironmentStateTypeDef = TypedDict(
+    "EnvironmentStateTypeDef",
+    {
+        "spec": str,
+        "templateMajorVersion": str,
+        "templateMinorVersion": str,
+        "templateName": str,
+    },
+)
+
+ServiceInstanceStateTypeDef = TypedDict(
+    "ServiceInstanceStateTypeDef",
+    {
+        "lastSuccessfulComponentDeploymentIds": List[str],
+        "lastSuccessfulEnvironmentDeploymentId": str,
+        "lastSuccessfulServicePipelineDeploymentId": str,
+        "spec": str,
+        "templateMajorVersion": str,
+        "templateMinorVersion": str,
+        "templateName": str,
+    },
+)
+
+ServicePipelineStateTypeDef = TypedDict(
+    "ServicePipelineStateTypeDef",
+    {
+        "spec": str,
+        "templateMajorVersion": str,
+        "templateMinorVersion": str,
+        "templateName": str,
+    },
+)
+
+DeploymentSummaryTypeDef = TypedDict(
+    "DeploymentSummaryTypeDef",
     {
         "arn": str,
+        "completedAt": datetime,
+        "componentName": str,
+        "createdAt": datetime,
+        "deploymentStatus": DeploymentStatusType,
+        "environmentName": str,
+        "id": str,
+        "lastAttemptedDeploymentId": str,
+        "lastModifiedAt": datetime,
+        "lastSucceededDeploymentId": str,
+        "serviceInstanceName": str,
+        "serviceName": str,
+        "targetArn": str,
+        "targetResourceCreatedAt": datetime,
+        "targetResourceType": DeploymentTargetResourceTypeType,
+    },
+)
+
+EnvironmentAccountConnectionSummaryTypeDef = TypedDict(
+    "EnvironmentAccountConnectionSummaryTypeDef",
+    {
+        "arn": str,
+        "componentRoleArn": str,
         "environmentAccountId": str,
         "environmentName": str,
         "id": str,
         "lastModifiedAt": datetime,
         "managementAccountId": str,
         "requestedAt": datetime,
         "roleArn": str,
         "status": EnvironmentAccountConnectionStatusType,
     },
 )
-_OptionalEnvironmentAccountConnectionSummaryTypeDef = TypedDict(
-    "_OptionalEnvironmentAccountConnectionSummaryTypeDef",
-    {
-        "componentRoleArn": str,
-    },
-    total=False,
-)
-
-
-class EnvironmentAccountConnectionSummaryTypeDef(
-    _RequiredEnvironmentAccountConnectionSummaryTypeDef,
-    _OptionalEnvironmentAccountConnectionSummaryTypeDef,
-):
-    pass
 
-
-_RequiredEnvironmentSummaryTypeDef = TypedDict(
-    "_RequiredEnvironmentSummaryTypeDef",
+EnvironmentSummaryTypeDef = TypedDict(
+    "EnvironmentSummaryTypeDef",
     {
         "arn": str,
+        "componentRoleArn": str,
         "createdAt": datetime,
         "deploymentStatus": DeploymentStatusType,
-        "lastDeploymentAttemptedAt": datetime,
-        "lastDeploymentSucceededAt": datetime,
-        "name": str,
-        "templateMajorVersion": str,
-        "templateMinorVersion": str,
-        "templateName": str,
-    },
-)
-_OptionalEnvironmentSummaryTypeDef = TypedDict(
-    "_OptionalEnvironmentSummaryTypeDef",
-    {
-        "componentRoleArn": str,
         "deploymentStatusMessage": str,
         "description": str,
         "environmentAccountConnectionId": str,
         "environmentAccountId": str,
+        "lastAttemptedDeploymentId": str,
+        "lastDeploymentAttemptedAt": datetime,
+        "lastDeploymentSucceededAt": datetime,
+        "lastSucceededDeploymentId": str,
+        "name": str,
         "protonServiceRoleArn": str,
         "provisioning": Literal["CUSTOMER_MANAGED"],
+        "templateMajorVersion": str,
+        "templateMinorVersion": str,
+        "templateName": str,
     },
-    total=False,
 )
 
-
-class EnvironmentSummaryTypeDef(
-    _RequiredEnvironmentSummaryTypeDef, _OptionalEnvironmentSummaryTypeDef
-):
-    pass
-
-
 EnvironmentTemplateFilterTypeDef = TypedDict(
     "EnvironmentTemplateFilterTypeDef",
     {
         "majorVersion": str,
         "templateName": str,
     },
 )
 
-_RequiredEnvironmentTemplateSummaryTypeDef = TypedDict(
-    "_RequiredEnvironmentTemplateSummaryTypeDef",
+EnvironmentTemplateSummaryTypeDef = TypedDict(
+    "EnvironmentTemplateSummaryTypeDef",
     {
         "arn": str,
         "createdAt": datetime,
-        "lastModifiedAt": datetime,
-        "name": str,
-    },
-)
-_OptionalEnvironmentTemplateSummaryTypeDef = TypedDict(
-    "_OptionalEnvironmentTemplateSummaryTypeDef",
-    {
         "description": str,
         "displayName": str,
+        "lastModifiedAt": datetime,
+        "name": str,
         "provisioning": Literal["CUSTOMER_MANAGED"],
         "recommendedVersion": str,
     },
-    total=False,
 )
 
-
-class EnvironmentTemplateSummaryTypeDef(
-    _RequiredEnvironmentTemplateSummaryTypeDef, _OptionalEnvironmentTemplateSummaryTypeDef
-):
-    pass
-
-
-_RequiredEnvironmentTemplateVersionSummaryTypeDef = TypedDict(
-    "_RequiredEnvironmentTemplateVersionSummaryTypeDef",
+EnvironmentTemplateVersionSummaryTypeDef = TypedDict(
+    "EnvironmentTemplateVersionSummaryTypeDef",
     {
         "arn": str,
         "createdAt": datetime,
+        "description": str,
         "lastModifiedAt": datetime,
         "majorVersion": str,
         "minorVersion": str,
-        "status": TemplateVersionStatusType,
-        "templateName": str,
-    },
-)
-_OptionalEnvironmentTemplateVersionSummaryTypeDef = TypedDict(
-    "_OptionalEnvironmentTemplateVersionSummaryTypeDef",
-    {
-        "description": str,
         "recommendedMinorVersion": str,
+        "status": TemplateVersionStatusType,
         "statusMessage": str,
+        "templateName": str,
     },
-    total=False,
 )
 
-
-class EnvironmentTemplateVersionSummaryTypeDef(
-    _RequiredEnvironmentTemplateVersionSummaryTypeDef,
-    _OptionalEnvironmentTemplateVersionSummaryTypeDef,
-):
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
@@ -945,14 +856,38 @@
 GetComponentInputRequestTypeDef = TypedDict(
     "GetComponentInputRequestTypeDef",
     {
         "name": str,
     },
 )
 
+_RequiredGetDeploymentInputRequestTypeDef = TypedDict(
+    "_RequiredGetDeploymentInputRequestTypeDef",
+    {
+        "id": str,
+    },
+)
+_OptionalGetDeploymentInputRequestTypeDef = TypedDict(
+    "_OptionalGetDeploymentInputRequestTypeDef",
+    {
+        "componentName": str,
+        "environmentName": str,
+        "serviceInstanceName": str,
+        "serviceName": str,
+    },
+    total=False,
+)
+
+
+class GetDeploymentInputRequestTypeDef(
+    _RequiredGetDeploymentInputRequestTypeDef, _OptionalGetDeploymentInputRequestTypeDef
+):
+    pass
+
+
 GetEnvironmentAccountConnectionInputRequestTypeDef = TypedDict(
     "GetEnvironmentAccountConnectionInputRequestTypeDef",
     {
         "id": str,
     },
 )
 
@@ -1098,14 +1033,15 @@
     {
         "componentName": str,
     },
 )
 _OptionalListComponentOutputsInputListComponentOutputsPaginateTypeDef = TypedDict(
     "_OptionalListComponentOutputsInputListComponentOutputsPaginateTypeDef",
     {
+        "deploymentId": str,
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 
 class ListComponentOutputsInputListComponentOutputsPaginateTypeDef(
@@ -1120,14 +1056,15 @@
     {
         "componentName": str,
     },
 )
 _OptionalListComponentOutputsInputRequestTypeDef = TypedDict(
     "_OptionalListComponentOutputsInputRequestTypeDef",
     {
+        "deploymentId": str,
         "nextToken": str,
     },
     total=False,
 )
 
 
 class ListComponentOutputsInputRequestTypeDef(
@@ -1139,15 +1076,14 @@
 
 OutputTypeDef = TypedDict(
     "OutputTypeDef",
     {
         "key": str,
         "valueString": str,
     },
-    total=False,
 )
 
 _RequiredListComponentProvisionedResourcesInputListComponentProvisionedResourcesPaginateTypeDef = TypedDict(
     "_RequiredListComponentProvisionedResourcesInputListComponentProvisionedResourcesPaginateTypeDef",
     {
         "componentName": str,
     },
@@ -1193,15 +1129,14 @@
 ProvisionedResourceTypeDef = TypedDict(
     "ProvisionedResourceTypeDef",
     {
         "identifier": str,
         "name": str,
         "provisioningEngine": ProvisionedResourceEngineType,
     },
-    total=False,
 )
 
 ListComponentsInputListComponentsPaginateTypeDef = TypedDict(
     "ListComponentsInputListComponentsPaginateTypeDef",
     {
         "environmentName": str,
         "serviceInstanceName": str,
@@ -1219,14 +1154,39 @@
         "nextToken": str,
         "serviceInstanceName": str,
         "serviceName": str,
     },
     total=False,
 )
 
+ListDeploymentsInputListDeploymentsPaginateTypeDef = TypedDict(
+    "ListDeploymentsInputListDeploymentsPaginateTypeDef",
+    {
+        "componentName": str,
+        "environmentName": str,
+        "serviceInstanceName": str,
+        "serviceName": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+ListDeploymentsInputRequestTypeDef = TypedDict(
+    "ListDeploymentsInputRequestTypeDef",
+    {
+        "componentName": str,
+        "environmentName": str,
+        "maxResults": int,
+        "nextToken": str,
+        "serviceInstanceName": str,
+        "serviceName": str,
+    },
+    total=False,
+)
+
 _RequiredListEnvironmentAccountConnectionsInputListEnvironmentAccountConnectionsPaginateTypeDef = TypedDict(
     "_RequiredListEnvironmentAccountConnectionsInputListEnvironmentAccountConnectionsPaginateTypeDef",
     {
         "requestedBy": EnvironmentAccountConnectionRequesterAccountTypeType,
     },
 )
 _OptionalListEnvironmentAccountConnectionsInputListEnvironmentAccountConnectionsPaginateTypeDef = TypedDict(
@@ -1277,14 +1237,15 @@
     {
         "environmentName": str,
     },
 )
 _OptionalListEnvironmentOutputsInputListEnvironmentOutputsPaginateTypeDef = TypedDict(
     "_OptionalListEnvironmentOutputsInputListEnvironmentOutputsPaginateTypeDef",
     {
+        "deploymentId": str,
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 
 class ListEnvironmentOutputsInputListEnvironmentOutputsPaginateTypeDef(
@@ -1299,14 +1260,15 @@
     {
         "environmentName": str,
     },
 )
 _OptionalListEnvironmentOutputsInputRequestTypeDef = TypedDict(
     "_OptionalListEnvironmentOutputsInputRequestTypeDef",
     {
+        "deploymentId": str,
         "nextToken": str,
     },
     total=False,
 )
 
 
 class ListEnvironmentOutputsInputRequestTypeDef(
@@ -1515,14 +1477,15 @@
         "serviceInstanceName": str,
         "serviceName": str,
     },
 )
 _OptionalListServiceInstanceOutputsInputListServiceInstanceOutputsPaginateTypeDef = TypedDict(
     "_OptionalListServiceInstanceOutputsInputListServiceInstanceOutputsPaginateTypeDef",
     {
+        "deploymentId": str,
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 
 class ListServiceInstanceOutputsInputListServiceInstanceOutputsPaginateTypeDef(
@@ -1538,14 +1501,15 @@
         "serviceInstanceName": str,
         "serviceName": str,
     },
 )
 _OptionalListServiceInstanceOutputsInputRequestTypeDef = TypedDict(
     "_OptionalListServiceInstanceOutputsInputRequestTypeDef",
     {
+        "deploymentId": str,
         "nextToken": str,
     },
     total=False,
 )
 
 
 class ListServiceInstanceOutputsInputRequestTypeDef(
@@ -1606,54 +1570,44 @@
     {
         "key": ListServiceInstancesFilterByType,
         "value": str,
     },
     total=False,
 )
 
-_RequiredServiceInstanceSummaryTypeDef = TypedDict(
-    "_RequiredServiceInstanceSummaryTypeDef",
+ServiceInstanceSummaryTypeDef = TypedDict(
+    "ServiceInstanceSummaryTypeDef",
     {
         "arn": str,
         "createdAt": datetime,
         "deploymentStatus": DeploymentStatusType,
+        "deploymentStatusMessage": str,
         "environmentName": str,
+        "lastAttemptedDeploymentId": str,
         "lastDeploymentAttemptedAt": datetime,
         "lastDeploymentSucceededAt": datetime,
+        "lastSucceededDeploymentId": str,
         "name": str,
         "serviceName": str,
         "templateMajorVersion": str,
         "templateMinorVersion": str,
         "templateName": str,
     },
 )
-_OptionalServiceInstanceSummaryTypeDef = TypedDict(
-    "_OptionalServiceInstanceSummaryTypeDef",
-    {
-        "deploymentStatusMessage": str,
-    },
-    total=False,
-)
-
-
-class ServiceInstanceSummaryTypeDef(
-    _RequiredServiceInstanceSummaryTypeDef, _OptionalServiceInstanceSummaryTypeDef
-):
-    pass
-
 
 _RequiredListServicePipelineOutputsInputListServicePipelineOutputsPaginateTypeDef = TypedDict(
     "_RequiredListServicePipelineOutputsInputListServicePipelineOutputsPaginateTypeDef",
     {
         "serviceName": str,
     },
 )
 _OptionalListServicePipelineOutputsInputListServicePipelineOutputsPaginateTypeDef = TypedDict(
     "_OptionalListServicePipelineOutputsInputListServicePipelineOutputsPaginateTypeDef",
     {
+        "deploymentId": str,
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 
 class ListServicePipelineOutputsInputListServicePipelineOutputsPaginateTypeDef(
@@ -1668,14 +1622,15 @@
     {
         "serviceName": str,
     },
 )
 _OptionalListServicePipelineOutputsInputRequestTypeDef = TypedDict(
     "_OptionalListServicePipelineOutputsInputRequestTypeDef",
     {
+        "deploymentId": str,
         "nextToken": str,
     },
     total=False,
 )
 
 
 class ListServicePipelineOutputsInputRequestTypeDef(
@@ -1772,43 +1727,30 @@
 class ListServiceTemplateVersionsInputRequestTypeDef(
     _RequiredListServiceTemplateVersionsInputRequestTypeDef,
     _OptionalListServiceTemplateVersionsInputRequestTypeDef,
 ):
     pass
 
 
-_RequiredServiceTemplateVersionSummaryTypeDef = TypedDict(
-    "_RequiredServiceTemplateVersionSummaryTypeDef",
+ServiceTemplateVersionSummaryTypeDef = TypedDict(
+    "ServiceTemplateVersionSummaryTypeDef",
     {
         "arn": str,
         "createdAt": datetime,
+        "description": str,
         "lastModifiedAt": datetime,
         "majorVersion": str,
         "minorVersion": str,
-        "status": TemplateVersionStatusType,
-        "templateName": str,
-    },
-)
-_OptionalServiceTemplateVersionSummaryTypeDef = TypedDict(
-    "_OptionalServiceTemplateVersionSummaryTypeDef",
-    {
-        "description": str,
         "recommendedMinorVersion": str,
+        "status": TemplateVersionStatusType,
         "statusMessage": str,
+        "templateName": str,
     },
-    total=False,
 )
 
-
-class ServiceTemplateVersionSummaryTypeDef(
-    _RequiredServiceTemplateVersionSummaryTypeDef, _OptionalServiceTemplateVersionSummaryTypeDef
-):
-    pass
-
-
 ListServiceTemplatesInputListServiceTemplatesPaginateTypeDef = TypedDict(
     "ListServiceTemplatesInputListServiceTemplatesPaginateTypeDef",
     {
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
@@ -1818,41 +1760,28 @@
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-_RequiredServiceTemplateSummaryTypeDef = TypedDict(
-    "_RequiredServiceTemplateSummaryTypeDef",
+ServiceTemplateSummaryTypeDef = TypedDict(
+    "ServiceTemplateSummaryTypeDef",
     {
         "arn": str,
         "createdAt": datetime,
-        "lastModifiedAt": datetime,
-        "name": str,
-    },
-)
-_OptionalServiceTemplateSummaryTypeDef = TypedDict(
-    "_OptionalServiceTemplateSummaryTypeDef",
-    {
         "description": str,
         "displayName": str,
+        "lastModifiedAt": datetime,
+        "name": str,
         "pipelineProvisioning": Literal["CUSTOMER_MANAGED"],
         "recommendedVersion": str,
     },
-    total=False,
 )
 
-
-class ServiceTemplateSummaryTypeDef(
-    _RequiredServiceTemplateSummaryTypeDef, _OptionalServiceTemplateSummaryTypeDef
-):
-    pass
-
-
 ListServicesInputListServicesPaginateTypeDef = TypedDict(
     "ListServicesInputListServicesPaginateTypeDef",
     {
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
@@ -1862,39 +1791,28 @@
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-_RequiredServiceSummaryTypeDef = TypedDict(
-    "_RequiredServiceSummaryTypeDef",
+ServiceSummaryTypeDef = TypedDict(
+    "ServiceSummaryTypeDef",
     {
         "arn": str,
         "createdAt": datetime,
+        "description": str,
         "lastModifiedAt": datetime,
         "name": str,
         "status": ServiceStatusType,
-        "templateName": str,
-    },
-)
-_OptionalServiceSummaryTypeDef = TypedDict(
-    "_OptionalServiceSummaryTypeDef",
-    {
-        "description": str,
         "statusMessage": str,
+        "templateName": str,
     },
-    total=False,
 )
 
-
-class ServiceSummaryTypeDef(_RequiredServiceSummaryTypeDef, _OptionalServiceSummaryTypeDef):
-    pass
-
-
 _RequiredListTagsForResourceInputListTagsForResourcePaginateTypeDef = TypedDict(
     "_RequiredListTagsForResourceInputListTagsForResourcePaginateTypeDef",
     {
         "resourceArn": str,
     },
 )
 _OptionalListTagsForResourceInputListTagsForResourcePaginateTypeDef = TypedDict(
@@ -1948,59 +1866,33 @@
 RejectEnvironmentAccountConnectionInputRequestTypeDef = TypedDict(
     "RejectEnvironmentAccountConnectionInputRequestTypeDef",
     {
         "id": str,
     },
 )
 
-_RequiredRepositorySyncEventTypeDef = TypedDict(
-    "_RequiredRepositorySyncEventTypeDef",
+RepositorySyncEventTypeDef = TypedDict(
+    "RepositorySyncEventTypeDef",
     {
         "event": str,
+        "externalId": str,
         "time": datetime,
         "type": str,
     },
 )
-_OptionalRepositorySyncEventTypeDef = TypedDict(
-    "_OptionalRepositorySyncEventTypeDef",
-    {
-        "externalId": str,
-    },
-    total=False,
-)
-
-
-class RepositorySyncEventTypeDef(
-    _RequiredRepositorySyncEventTypeDef, _OptionalRepositorySyncEventTypeDef
-):
-    pass
-
 
-_RequiredResourceSyncEventTypeDef = TypedDict(
-    "_RequiredResourceSyncEventTypeDef",
+ResourceSyncEventTypeDef = TypedDict(
+    "ResourceSyncEventTypeDef",
     {
         "event": str,
+        "externalId": str,
         "time": datetime,
         "type": str,
     },
 )
-_OptionalResourceSyncEventTypeDef = TypedDict(
-    "_OptionalResourceSyncEventTypeDef",
-    {
-        "externalId": str,
-    },
-    total=False,
-)
-
-
-class ResourceSyncEventTypeDef(
-    _RequiredResourceSyncEventTypeDef, _OptionalResourceSyncEventTypeDef
-):
-    pass
-
 
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
         "HTTPStatusCode": int,
@@ -2325,53 +2217,43 @@
 AccountSettingsTypeDef = TypedDict(
     "AccountSettingsTypeDef",
     {
         "pipelineCodebuildRoleArn": str,
         "pipelineProvisioningRepository": RepositoryBranchTypeDef,
         "pipelineServiceRoleArn": str,
     },
-    total=False,
 )
 
-_RequiredEnvironmentTypeDef = TypedDict(
-    "_RequiredEnvironmentTypeDef",
+EnvironmentTypeDef = TypedDict(
+    "EnvironmentTypeDef",
     {
         "arn": str,
-        "createdAt": datetime,
-        "deploymentStatus": DeploymentStatusType,
-        "lastDeploymentAttemptedAt": datetime,
-        "lastDeploymentSucceededAt": datetime,
-        "name": str,
-        "templateMajorVersion": str,
-        "templateMinorVersion": str,
-        "templateName": str,
-    },
-)
-_OptionalEnvironmentTypeDef = TypedDict(
-    "_OptionalEnvironmentTypeDef",
-    {
         "codebuildRoleArn": str,
         "componentRoleArn": str,
+        "createdAt": datetime,
+        "deploymentStatus": DeploymentStatusType,
         "deploymentStatusMessage": str,
         "description": str,
         "environmentAccountConnectionId": str,
         "environmentAccountId": str,
+        "lastAttemptedDeploymentId": str,
+        "lastDeploymentAttemptedAt": datetime,
+        "lastDeploymentSucceededAt": datetime,
+        "lastSucceededDeploymentId": str,
+        "name": str,
         "protonServiceRoleArn": str,
         "provisioning": Literal["CUSTOMER_MANAGED"],
         "provisioningRepository": RepositoryBranchTypeDef,
         "spec": str,
+        "templateMajorVersion": str,
+        "templateMinorVersion": str,
+        "templateName": str,
     },
-    total=False,
 )
 
-
-class EnvironmentTypeDef(_RequiredEnvironmentTypeDef, _OptionalEnvironmentTypeDef):
-    pass
-
-
 CancelComponentDeploymentOutputTypeDef = TypedDict(
     "CancelComponentDeploymentOutputTypeDef",
     {
         "component": ComponentTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -2444,44 +2326,33 @@
     "CancelServicePipelineDeploymentOutputTypeDef",
     {
         "pipeline": ServicePipelineTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredServiceTypeDef = TypedDict(
-    "_RequiredServiceTypeDef",
+ServiceTypeDef = TypedDict(
+    "ServiceTypeDef",
     {
         "arn": str,
+        "branchName": str,
         "createdAt": datetime,
+        "description": str,
         "lastModifiedAt": datetime,
         "name": str,
-        "spec": str,
-        "status": ServiceStatusType,
-        "templateName": str,
-    },
-)
-_OptionalServiceTypeDef = TypedDict(
-    "_OptionalServiceTypeDef",
-    {
-        "branchName": str,
-        "description": str,
         "pipeline": ServicePipelineTypeDef,
         "repositoryConnectionArn": str,
         "repositoryId": str,
+        "spec": str,
+        "status": ServiceStatusType,
         "statusMessage": str,
+        "templateName": str,
     },
-    total=False,
 )
 
-
-class ServiceTypeDef(_RequiredServiceTypeDef, _OptionalServiceTypeDef):
-    pass
-
-
 UpdateServicePipelineOutputTypeDef = TypedDict(
     "UpdateServicePipelineOutputTypeDef",
     {
         "pipeline": ServicePipelineTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -2509,46 +2380,33 @@
 class UpdateServiceTemplateVersionInputRequestTypeDef(
     _RequiredUpdateServiceTemplateVersionInputRequestTypeDef,
     _OptionalUpdateServiceTemplateVersionInputRequestTypeDef,
 ):
     pass
 
 
-_RequiredServiceTemplateVersionTypeDef = TypedDict(
-    "_RequiredServiceTemplateVersionTypeDef",
+ServiceTemplateVersionTypeDef = TypedDict(
+    "ServiceTemplateVersionTypeDef",
     {
         "arn": str,
         "compatibleEnvironmentTemplates": List[CompatibleEnvironmentTemplateTypeDef],
         "createdAt": datetime,
+        "description": str,
         "lastModifiedAt": datetime,
         "majorVersion": str,
         "minorVersion": str,
-        "status": TemplateVersionStatusType,
-        "templateName": str,
-    },
-)
-_OptionalServiceTemplateVersionTypeDef = TypedDict(
-    "_OptionalServiceTemplateVersionTypeDef",
-    {
-        "description": str,
         "recommendedMinorVersion": str,
         "schema": str,
+        "status": TemplateVersionStatusType,
         "statusMessage": str,
         "supportedComponentSources": List[Literal["DIRECTLY_DEFINED"]],
+        "templateName": str,
     },
-    total=False,
 )
 
-
-class ServiceTemplateVersionTypeDef(
-    _RequiredServiceTemplateVersionTypeDef, _OptionalServiceTemplateVersionTypeDef
-):
-    pass
-
-
 ListComponentsOutputTypeDef = TypedDict(
     "ListComponentsOutputTypeDef",
     {
         "components": List[ComponentSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -2561,15 +2419,14 @@
         "environmentTemplates": ResourceCountsSummaryTypeDef,
         "environments": ResourceCountsSummaryTypeDef,
         "pipelines": ResourceCountsSummaryTypeDef,
         "serviceInstances": ResourceCountsSummaryTypeDef,
         "serviceTemplates": ResourceCountsSummaryTypeDef,
         "services": ResourceCountsSummaryTypeDef,
     },
-    total=False,
 )
 
 _RequiredCreateComponentInputRequestTypeDef = TypedDict(
     "_RequiredCreateComponentInputRequestTypeDef",
     {
         "manifest": str,
         "name": str,
@@ -3025,14 +2882,33 @@
     "UpdateTemplateSyncConfigOutputTypeDef",
     {
         "templateSyncConfig": TemplateSyncConfigTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+DeploymentStateTypeDef = TypedDict(
+    "DeploymentStateTypeDef",
+    {
+        "component": ComponentStateTypeDef,
+        "environment": EnvironmentStateTypeDef,
+        "serviceInstance": ServiceInstanceStateTypeDef,
+        "servicePipeline": ServicePipelineStateTypeDef,
+    },
+)
+
+ListDeploymentsOutputTypeDef = TypedDict(
+    "ListDeploymentsOutputTypeDef",
+    {
+        "deployments": List[DeploymentSummaryTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ListEnvironmentAccountConnectionsOutputTypeDef = TypedDict(
     "ListEnvironmentAccountConnectionsOutputTypeDef",
     {
         "environmentAccountConnections": List[EnvironmentAccountConnectionSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -3510,39 +3386,28 @@
     "TemplateVersionSourceInputTypeDef",
     {
         "s3": S3ObjectSourceTypeDef,
     },
     total=False,
 )
 
-_RequiredSyncBlockerTypeDef = TypedDict(
-    "_RequiredSyncBlockerTypeDef",
+SyncBlockerTypeDef = TypedDict(
+    "SyncBlockerTypeDef",
     {
+        "contexts": List[SyncBlockerContextTypeDef],
         "createdAt": datetime,
         "createdReason": str,
         "id": str,
-        "status": BlockerStatusType,
-        "type": Literal["AUTOMATED"],
-    },
-)
-_OptionalSyncBlockerTypeDef = TypedDict(
-    "_OptionalSyncBlockerTypeDef",
-    {
-        "contexts": List[SyncBlockerContextTypeDef],
         "resolvedAt": datetime,
         "resolvedReason": str,
+        "status": BlockerStatusType,
+        "type": Literal["AUTOMATED"],
     },
-    total=False,
 )
 
-
-class SyncBlockerTypeDef(_RequiredSyncBlockerTypeDef, _OptionalSyncBlockerTypeDef):
-    pass
-
-
 GetAccountSettingsOutputTypeDef = TypedDict(
     "GetAccountSettingsOutputTypeDef",
     {
         "accountSettings": AccountSettingsTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -3663,14 +3528,38 @@
     "GetResourcesSummaryOutputTypeDef",
     {
         "counts": CountsSummaryTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+DeploymentTypeDef = TypedDict(
+    "DeploymentTypeDef",
+    {
+        "arn": str,
+        "completedAt": datetime,
+        "componentName": str,
+        "createdAt": datetime,
+        "deploymentStatus": DeploymentStatusType,
+        "deploymentStatusMessage": str,
+        "environmentName": str,
+        "id": str,
+        "initialState": DeploymentStateTypeDef,
+        "lastAttemptedDeploymentId": str,
+        "lastModifiedAt": datetime,
+        "lastSucceededDeploymentId": str,
+        "serviceInstanceName": str,
+        "serviceName": str,
+        "targetArn": str,
+        "targetResourceCreatedAt": datetime,
+        "targetResourceType": DeploymentTargetResourceTypeType,
+        "targetState": DeploymentStateTypeDef,
+    },
+)
+
 GetRepositorySyncStatusOutputTypeDef = TypedDict(
     "GetRepositorySyncStatusOutputTypeDef",
     {
         "latestSync": RepositorySyncAttemptTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -3745,46 +3634,49 @@
 class CreateServiceTemplateVersionInputRequestTypeDef(
     _RequiredCreateServiceTemplateVersionInputRequestTypeDef,
     _OptionalCreateServiceTemplateVersionInputRequestTypeDef,
 ):
     pass
 
 
-_RequiredServiceSyncBlockerSummaryTypeDef = TypedDict(
-    "_RequiredServiceSyncBlockerSummaryTypeDef",
-    {
-        "serviceName": str,
-    },
-)
-_OptionalServiceSyncBlockerSummaryTypeDef = TypedDict(
-    "_OptionalServiceSyncBlockerSummaryTypeDef",
+ServiceSyncBlockerSummaryTypeDef = TypedDict(
+    "ServiceSyncBlockerSummaryTypeDef",
     {
         "latestBlockers": List[SyncBlockerTypeDef],
         "serviceInstanceName": str,
+        "serviceName": str,
     },
-    total=False,
 )
 
-
-class ServiceSyncBlockerSummaryTypeDef(
-    _RequiredServiceSyncBlockerSummaryTypeDef, _OptionalServiceSyncBlockerSummaryTypeDef
-):
-    pass
-
-
 UpdateServiceSyncBlockerOutputTypeDef = TypedDict(
     "UpdateServiceSyncBlockerOutputTypeDef",
     {
         "serviceInstanceName": str,
         "serviceName": str,
         "serviceSyncBlocker": SyncBlockerTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+DeleteDeploymentOutputTypeDef = TypedDict(
+    "DeleteDeploymentOutputTypeDef",
+    {
+        "deployment": DeploymentTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+GetDeploymentOutputTypeDef = TypedDict(
+    "GetDeploymentOutputTypeDef",
+    {
+        "deployment": DeploymentTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetServiceSyncBlockerSummaryOutputTypeDef = TypedDict(
     "GetServiceSyncBlockerSummaryOutputTypeDef",
     {
         "serviceSyncBlockerSummary": ServiceSyncBlockerSummaryTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-proton-1.28.0/mypy_boto3_proton/type_defs.pyi` & `mypy-boto3-proton-1.28.3/mypy_boto3_proton/type_defs.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 from datetime import datetime
 from typing import Dict, List, Sequence
 
 from .literals import (
     BlockerStatusType,
     ComponentDeploymentUpdateTypeType,
     DeploymentStatusType,
+    DeploymentTargetResourceTypeType,
     DeploymentUpdateTypeType,
     EnvironmentAccountConnectionRequesterAccountTypeType,
     EnvironmentAccountConnectionStatusType,
     ListServiceInstancesFilterByType,
     ListServiceInstancesSortByType,
     ProvisionedResourceEngineType,
     RepositoryProviderType,
@@ -54,44 +55,51 @@
     "CancelEnvironmentDeploymentInputRequestTypeDef",
     "CancelServiceInstanceDeploymentInputRequestTypeDef",
     "ServiceInstanceTypeDef",
     "CancelServicePipelineDeploymentInputRequestTypeDef",
     "ServicePipelineTypeDef",
     "CompatibleEnvironmentTemplateInputTypeDef",
     "CompatibleEnvironmentTemplateTypeDef",
+    "ComponentStateTypeDef",
     "ComponentSummaryTypeDef",
     "ResourceCountsSummaryTypeDef",
     "TagTypeDef",
     "RepositoryBranchInputTypeDef",
     "EnvironmentTemplateTypeDef",
     "EnvironmentTemplateVersionTypeDef",
     "RepositoryTypeDef",
     "CreateServiceSyncConfigInputRequestTypeDef",
     "ServiceSyncConfigTypeDef",
     "ServiceTemplateTypeDef",
     "CreateTemplateSyncConfigInputRequestTypeDef",
     "TemplateSyncConfigTypeDef",
     "DeleteComponentInputRequestTypeDef",
+    "DeleteDeploymentInputRequestTypeDef",
     "DeleteEnvironmentAccountConnectionInputRequestTypeDef",
     "DeleteEnvironmentInputRequestTypeDef",
     "DeleteEnvironmentTemplateInputRequestTypeDef",
     "DeleteEnvironmentTemplateVersionInputRequestTypeDef",
     "DeleteRepositoryInputRequestTypeDef",
     "DeleteServiceInputRequestTypeDef",
     "DeleteServiceSyncConfigInputRequestTypeDef",
     "DeleteServiceTemplateInputRequestTypeDef",
     "DeleteServiceTemplateVersionInputRequestTypeDef",
     "DeleteTemplateSyncConfigInputRequestTypeDef",
+    "EnvironmentStateTypeDef",
+    "ServiceInstanceStateTypeDef",
+    "ServicePipelineStateTypeDef",
+    "DeploymentSummaryTypeDef",
     "EnvironmentAccountConnectionSummaryTypeDef",
     "EnvironmentSummaryTypeDef",
     "EnvironmentTemplateFilterTypeDef",
     "EnvironmentTemplateSummaryTypeDef",
     "EnvironmentTemplateVersionSummaryTypeDef",
     "WaiterConfigTypeDef",
     "GetComponentInputRequestTypeDef",
+    "GetDeploymentInputRequestTypeDef",
     "GetEnvironmentAccountConnectionInputRequestTypeDef",
     "GetEnvironmentInputRequestTypeDef",
     "GetEnvironmentTemplateInputRequestTypeDef",
     "GetEnvironmentTemplateVersionInputRequestTypeDef",
     "GetRepositoryInputRequestTypeDef",
     "GetRepositorySyncStatusInputRequestTypeDef",
     "GetServiceInputRequestTypeDef",
@@ -108,14 +116,16 @@
     "ListComponentOutputsInputRequestTypeDef",
     "OutputTypeDef",
     "ListComponentProvisionedResourcesInputListComponentProvisionedResourcesPaginateTypeDef",
     "ListComponentProvisionedResourcesInputRequestTypeDef",
     "ProvisionedResourceTypeDef",
     "ListComponentsInputListComponentsPaginateTypeDef",
     "ListComponentsInputRequestTypeDef",
+    "ListDeploymentsInputListDeploymentsPaginateTypeDef",
+    "ListDeploymentsInputRequestTypeDef",
     "ListEnvironmentAccountConnectionsInputListEnvironmentAccountConnectionsPaginateTypeDef",
     "ListEnvironmentAccountConnectionsInputRequestTypeDef",
     "ListEnvironmentOutputsInputListEnvironmentOutputsPaginateTypeDef",
     "ListEnvironmentOutputsInputRequestTypeDef",
     "ListEnvironmentProvisionedResourcesInputListEnvironmentProvisionedResourcesPaginateTypeDef",
     "ListEnvironmentProvisionedResourcesInputRequestTypeDef",
     "ListEnvironmentTemplateVersionsInputListEnvironmentTemplateVersionsPaginateTypeDef",
@@ -223,14 +233,16 @@
     "DeleteServiceTemplateOutputTypeDef",
     "GetServiceTemplateOutputTypeDef",
     "UpdateServiceTemplateOutputTypeDef",
     "CreateTemplateSyncConfigOutputTypeDef",
     "DeleteTemplateSyncConfigOutputTypeDef",
     "GetTemplateSyncConfigOutputTypeDef",
     "UpdateTemplateSyncConfigOutputTypeDef",
+    "DeploymentStateTypeDef",
+    "ListDeploymentsOutputTypeDef",
     "ListEnvironmentAccountConnectionsOutputTypeDef",
     "ListEnvironmentsOutputTypeDef",
     "ListEnvironmentsInputListEnvironmentsPaginateTypeDef",
     "ListEnvironmentsInputRequestTypeDef",
     "ListEnvironmentTemplatesOutputTypeDef",
     "ListEnvironmentTemplateVersionsOutputTypeDef",
     "GetComponentInputComponentDeletedWaitTypeDef",
@@ -276,58 +288,50 @@
     "GetServiceOutputTypeDef",
     "UpdateServiceOutputTypeDef",
     "CreateServiceTemplateVersionOutputTypeDef",
     "DeleteServiceTemplateVersionOutputTypeDef",
     "GetServiceTemplateVersionOutputTypeDef",
     "UpdateServiceTemplateVersionOutputTypeDef",
     "GetResourcesSummaryOutputTypeDef",
+    "DeploymentTypeDef",
     "GetRepositorySyncStatusOutputTypeDef",
     "GetServiceInstanceSyncStatusOutputTypeDef",
     "GetTemplateSyncStatusOutputTypeDef",
     "CreateEnvironmentTemplateVersionInputRequestTypeDef",
     "CreateServiceTemplateVersionInputRequestTypeDef",
     "ServiceSyncBlockerSummaryTypeDef",
     "UpdateServiceSyncBlockerOutputTypeDef",
+    "DeleteDeploymentOutputTypeDef",
+    "GetDeploymentOutputTypeDef",
     "GetServiceSyncBlockerSummaryOutputTypeDef",
 )
 
 AcceptEnvironmentAccountConnectionInputRequestTypeDef = TypedDict(
     "AcceptEnvironmentAccountConnectionInputRequestTypeDef",
     {
         "id": str,
     },
 )
 
-_RequiredEnvironmentAccountConnectionTypeDef = TypedDict(
-    "_RequiredEnvironmentAccountConnectionTypeDef",
+EnvironmentAccountConnectionTypeDef = TypedDict(
+    "EnvironmentAccountConnectionTypeDef",
     {
         "arn": str,
+        "codebuildRoleArn": str,
+        "componentRoleArn": str,
         "environmentAccountId": str,
         "environmentName": str,
         "id": str,
         "lastModifiedAt": datetime,
         "managementAccountId": str,
         "requestedAt": datetime,
         "roleArn": str,
         "status": EnvironmentAccountConnectionStatusType,
     },
 )
-_OptionalEnvironmentAccountConnectionTypeDef = TypedDict(
-    "_OptionalEnvironmentAccountConnectionTypeDef",
-    {
-        "codebuildRoleArn": str,
-        "componentRoleArn": str,
-    },
-    total=False,
-)
-
-class EnvironmentAccountConnectionTypeDef(
-    _RequiredEnvironmentAccountConnectionTypeDef, _OptionalEnvironmentAccountConnectionTypeDef
-):
-    pass
 
 RepositoryBranchTypeDef = TypedDict(
     "RepositoryBranchTypeDef",
     {
         "arn": str,
         "branch": str,
         "name": str,
@@ -338,43 +342,36 @@
 CancelComponentDeploymentInputRequestTypeDef = TypedDict(
     "CancelComponentDeploymentInputRequestTypeDef",
     {
         "componentName": str,
     },
 )
 
-_RequiredComponentTypeDef = TypedDict(
-    "_RequiredComponentTypeDef",
+ComponentTypeDef = TypedDict(
+    "ComponentTypeDef",
     {
         "arn": str,
         "createdAt": datetime,
         "deploymentStatus": DeploymentStatusType,
-        "environmentName": str,
-        "lastModifiedAt": datetime,
-        "name": str,
-    },
-)
-_OptionalComponentTypeDef = TypedDict(
-    "_OptionalComponentTypeDef",
-    {
         "deploymentStatusMessage": str,
         "description": str,
+        "environmentName": str,
+        "lastAttemptedDeploymentId": str,
         "lastClientRequestToken": str,
         "lastDeploymentAttemptedAt": datetime,
         "lastDeploymentSucceededAt": datetime,
+        "lastModifiedAt": datetime,
+        "lastSucceededDeploymentId": str,
+        "name": str,
         "serviceInstanceName": str,
         "serviceName": str,
         "serviceSpec": str,
     },
-    total=False,
 )
 
-class ComponentTypeDef(_RequiredComponentTypeDef, _OptionalComponentTypeDef):
-    pass
-
 CancelEnvironmentDeploymentInputRequestTypeDef = TypedDict(
     "CancelEnvironmentDeploymentInputRequestTypeDef",
     {
         "environmentName": str,
     },
 )
 
@@ -382,74 +379,60 @@
     "CancelServiceInstanceDeploymentInputRequestTypeDef",
     {
         "serviceInstanceName": str,
         "serviceName": str,
     },
 )
 
-_RequiredServiceInstanceTypeDef = TypedDict(
-    "_RequiredServiceInstanceTypeDef",
+ServiceInstanceTypeDef = TypedDict(
+    "ServiceInstanceTypeDef",
     {
         "arn": str,
         "createdAt": datetime,
         "deploymentStatus": DeploymentStatusType,
+        "deploymentStatusMessage": str,
         "environmentName": str,
+        "lastAttemptedDeploymentId": str,
+        "lastClientRequestToken": str,
         "lastDeploymentAttemptedAt": datetime,
         "lastDeploymentSucceededAt": datetime,
+        "lastSucceededDeploymentId": str,
         "name": str,
         "serviceName": str,
+        "spec": str,
         "templateMajorVersion": str,
         "templateMinorVersion": str,
         "templateName": str,
     },
 )
-_OptionalServiceInstanceTypeDef = TypedDict(
-    "_OptionalServiceInstanceTypeDef",
-    {
-        "deploymentStatusMessage": str,
-        "lastClientRequestToken": str,
-        "spec": str,
-    },
-    total=False,
-)
-
-class ServiceInstanceTypeDef(_RequiredServiceInstanceTypeDef, _OptionalServiceInstanceTypeDef):
-    pass
 
 CancelServicePipelineDeploymentInputRequestTypeDef = TypedDict(
     "CancelServicePipelineDeploymentInputRequestTypeDef",
     {
         "serviceName": str,
     },
 )
 
-_RequiredServicePipelineTypeDef = TypedDict(
-    "_RequiredServicePipelineTypeDef",
+ServicePipelineTypeDef = TypedDict(
+    "ServicePipelineTypeDef",
     {
         "arn": str,
         "createdAt": datetime,
         "deploymentStatus": DeploymentStatusType,
+        "deploymentStatusMessage": str,
+        "lastAttemptedDeploymentId": str,
         "lastDeploymentAttemptedAt": datetime,
         "lastDeploymentSucceededAt": datetime,
+        "lastSucceededDeploymentId": str,
+        "spec": str,
         "templateMajorVersion": str,
         "templateMinorVersion": str,
         "templateName": str,
     },
 )
-_OptionalServicePipelineTypeDef = TypedDict(
-    "_OptionalServicePipelineTypeDef",
-    {
-        "deploymentStatusMessage": str,
-        "spec": str,
-    },
-    total=False,
-)
-
-class ServicePipelineTypeDef(_RequiredServicePipelineTypeDef, _OptionalServicePipelineTypeDef):
-    pass
 
 CompatibleEnvironmentTemplateInputTypeDef = TypedDict(
     "CompatibleEnvironmentTemplateInputTypeDef",
     {
         "majorVersion": str,
         "templateName": str,
     },
@@ -459,62 +442,54 @@
     "CompatibleEnvironmentTemplateTypeDef",
     {
         "majorVersion": str,
         "templateName": str,
     },
 )
 
-_RequiredComponentSummaryTypeDef = TypedDict(
-    "_RequiredComponentSummaryTypeDef",
+ComponentStateTypeDef = TypedDict(
+    "ComponentStateTypeDef",
     {
-        "arn": str,
-        "createdAt": datetime,
-        "deploymentStatus": DeploymentStatusType,
-        "environmentName": str,
-        "lastModifiedAt": datetime,
-        "name": str,
+        "serviceInstanceName": str,
+        "serviceName": str,
+        "serviceSpec": str,
+        "templateFile": str,
     },
 )
-_OptionalComponentSummaryTypeDef = TypedDict(
-    "_OptionalComponentSummaryTypeDef",
+
+ComponentSummaryTypeDef = TypedDict(
+    "ComponentSummaryTypeDef",
     {
+        "arn": str,
+        "createdAt": datetime,
+        "deploymentStatus": DeploymentStatusType,
         "deploymentStatusMessage": str,
+        "environmentName": str,
+        "lastAttemptedDeploymentId": str,
         "lastDeploymentAttemptedAt": datetime,
         "lastDeploymentSucceededAt": datetime,
+        "lastModifiedAt": datetime,
+        "lastSucceededDeploymentId": str,
+        "name": str,
         "serviceInstanceName": str,
         "serviceName": str,
     },
-    total=False,
 )
 
-class ComponentSummaryTypeDef(_RequiredComponentSummaryTypeDef, _OptionalComponentSummaryTypeDef):
-    pass
-
-_RequiredResourceCountsSummaryTypeDef = TypedDict(
-    "_RequiredResourceCountsSummaryTypeDef",
-    {
-        "total": int,
-    },
-)
-_OptionalResourceCountsSummaryTypeDef = TypedDict(
-    "_OptionalResourceCountsSummaryTypeDef",
+ResourceCountsSummaryTypeDef = TypedDict(
+    "ResourceCountsSummaryTypeDef",
     {
         "behindMajor": int,
         "behindMinor": int,
         "failed": int,
+        "total": int,
         "upToDate": int,
     },
-    total=False,
 )
 
-class ResourceCountsSummaryTypeDef(
-    _RequiredResourceCountsSummaryTypeDef, _OptionalResourceCountsSummaryTypeDef
-):
-    pass
-
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "key": str,
         "value": str,
     },
 )
@@ -524,87 +499,56 @@
     {
         "branch": str,
         "name": str,
         "provider": RepositoryProviderType,
     },
 )
 
-_RequiredEnvironmentTemplateTypeDef = TypedDict(
-    "_RequiredEnvironmentTemplateTypeDef",
+EnvironmentTemplateTypeDef = TypedDict(
+    "EnvironmentTemplateTypeDef",
     {
         "arn": str,
         "createdAt": datetime,
-        "lastModifiedAt": datetime,
-        "name": str,
-    },
-)
-_OptionalEnvironmentTemplateTypeDef = TypedDict(
-    "_OptionalEnvironmentTemplateTypeDef",
-    {
         "description": str,
         "displayName": str,
         "encryptionKey": str,
+        "lastModifiedAt": datetime,
+        "name": str,
         "provisioning": Literal["CUSTOMER_MANAGED"],
         "recommendedVersion": str,
     },
-    total=False,
 )
 
-class EnvironmentTemplateTypeDef(
-    _RequiredEnvironmentTemplateTypeDef, _OptionalEnvironmentTemplateTypeDef
-):
-    pass
-
-_RequiredEnvironmentTemplateVersionTypeDef = TypedDict(
-    "_RequiredEnvironmentTemplateVersionTypeDef",
+EnvironmentTemplateVersionTypeDef = TypedDict(
+    "EnvironmentTemplateVersionTypeDef",
     {
         "arn": str,
         "createdAt": datetime,
+        "description": str,
         "lastModifiedAt": datetime,
         "majorVersion": str,
         "minorVersion": str,
-        "status": TemplateVersionStatusType,
-        "templateName": str,
-    },
-)
-_OptionalEnvironmentTemplateVersionTypeDef = TypedDict(
-    "_OptionalEnvironmentTemplateVersionTypeDef",
-    {
-        "description": str,
         "recommendedMinorVersion": str,
         "schema": str,
+        "status": TemplateVersionStatusType,
         "statusMessage": str,
+        "templateName": str,
     },
-    total=False,
 )
 
-class EnvironmentTemplateVersionTypeDef(
-    _RequiredEnvironmentTemplateVersionTypeDef, _OptionalEnvironmentTemplateVersionTypeDef
-):
-    pass
-
-_RequiredRepositoryTypeDef = TypedDict(
-    "_RequiredRepositoryTypeDef",
+RepositoryTypeDef = TypedDict(
+    "RepositoryTypeDef",
     {
         "arn": str,
         "connectionArn": str,
+        "encryptionKey": str,
         "name": str,
         "provider": RepositoryProviderType,
     },
 )
-_OptionalRepositoryTypeDef = TypedDict(
-    "_OptionalRepositoryTypeDef",
-    {
-        "encryptionKey": str,
-    },
-    total=False,
-)
-
-class RepositoryTypeDef(_RequiredRepositoryTypeDef, _OptionalRepositoryTypeDef):
-    pass
 
 CreateServiceSyncConfigInputRequestTypeDef = TypedDict(
     "CreateServiceSyncConfigInputRequestTypeDef",
     {
         "branch": str,
         "filePath": str,
         "repositoryName": str,
@@ -620,38 +564,29 @@
         "filePath": str,
         "repositoryName": str,
         "repositoryProvider": RepositoryProviderType,
         "serviceName": str,
     },
 )
 
-_RequiredServiceTemplateTypeDef = TypedDict(
-    "_RequiredServiceTemplateTypeDef",
+ServiceTemplateTypeDef = TypedDict(
+    "ServiceTemplateTypeDef",
     {
         "arn": str,
         "createdAt": datetime,
-        "lastModifiedAt": datetime,
-        "name": str,
-    },
-)
-_OptionalServiceTemplateTypeDef = TypedDict(
-    "_OptionalServiceTemplateTypeDef",
-    {
         "description": str,
         "displayName": str,
         "encryptionKey": str,
+        "lastModifiedAt": datetime,
+        "name": str,
         "pipelineProvisioning": Literal["CUSTOMER_MANAGED"],
         "recommendedVersion": str,
     },
-    total=False,
 )
 
-class ServiceTemplateTypeDef(_RequiredServiceTemplateTypeDef, _OptionalServiceTemplateTypeDef):
-    pass
-
 _RequiredCreateTemplateSyncConfigInputRequestTypeDef = TypedDict(
     "_RequiredCreateTemplateSyncConfigInputRequestTypeDef",
     {
         "branch": str,
         "repositoryName": str,
         "repositoryProvider": RepositoryProviderType,
         "templateName": str,
@@ -668,44 +603,40 @@
 
 class CreateTemplateSyncConfigInputRequestTypeDef(
     _RequiredCreateTemplateSyncConfigInputRequestTypeDef,
     _OptionalCreateTemplateSyncConfigInputRequestTypeDef,
 ):
     pass
 
-_RequiredTemplateSyncConfigTypeDef = TypedDict(
-    "_RequiredTemplateSyncConfigTypeDef",
+TemplateSyncConfigTypeDef = TypedDict(
+    "TemplateSyncConfigTypeDef",
     {
         "branch": str,
         "repositoryName": str,
         "repositoryProvider": RepositoryProviderType,
+        "subdirectory": str,
         "templateName": str,
         "templateType": TemplateTypeType,
     },
 )
-_OptionalTemplateSyncConfigTypeDef = TypedDict(
-    "_OptionalTemplateSyncConfigTypeDef",
-    {
-        "subdirectory": str,
-    },
-    total=False,
-)
-
-class TemplateSyncConfigTypeDef(
-    _RequiredTemplateSyncConfigTypeDef, _OptionalTemplateSyncConfigTypeDef
-):
-    pass
 
 DeleteComponentInputRequestTypeDef = TypedDict(
     "DeleteComponentInputRequestTypeDef",
     {
         "name": str,
     },
 )
 
+DeleteDeploymentInputRequestTypeDef = TypedDict(
+    "DeleteDeploymentInputRequestTypeDef",
+    {
+        "id": str,
+    },
+)
+
 DeleteEnvironmentAccountConnectionInputRequestTypeDef = TypedDict(
     "DeleteEnvironmentAccountConnectionInputRequestTypeDef",
     {
         "id": str,
     },
 )
 
@@ -774,135 +705,145 @@
     "DeleteTemplateSyncConfigInputRequestTypeDef",
     {
         "templateName": str,
         "templateType": TemplateTypeType,
     },
 )
 
-_RequiredEnvironmentAccountConnectionSummaryTypeDef = TypedDict(
-    "_RequiredEnvironmentAccountConnectionSummaryTypeDef",
+EnvironmentStateTypeDef = TypedDict(
+    "EnvironmentStateTypeDef",
+    {
+        "spec": str,
+        "templateMajorVersion": str,
+        "templateMinorVersion": str,
+        "templateName": str,
+    },
+)
+
+ServiceInstanceStateTypeDef = TypedDict(
+    "ServiceInstanceStateTypeDef",
+    {
+        "lastSuccessfulComponentDeploymentIds": List[str],
+        "lastSuccessfulEnvironmentDeploymentId": str,
+        "lastSuccessfulServicePipelineDeploymentId": str,
+        "spec": str,
+        "templateMajorVersion": str,
+        "templateMinorVersion": str,
+        "templateName": str,
+    },
+)
+
+ServicePipelineStateTypeDef = TypedDict(
+    "ServicePipelineStateTypeDef",
+    {
+        "spec": str,
+        "templateMajorVersion": str,
+        "templateMinorVersion": str,
+        "templateName": str,
+    },
+)
+
+DeploymentSummaryTypeDef = TypedDict(
+    "DeploymentSummaryTypeDef",
+    {
+        "arn": str,
+        "completedAt": datetime,
+        "componentName": str,
+        "createdAt": datetime,
+        "deploymentStatus": DeploymentStatusType,
+        "environmentName": str,
+        "id": str,
+        "lastAttemptedDeploymentId": str,
+        "lastModifiedAt": datetime,
+        "lastSucceededDeploymentId": str,
+        "serviceInstanceName": str,
+        "serviceName": str,
+        "targetArn": str,
+        "targetResourceCreatedAt": datetime,
+        "targetResourceType": DeploymentTargetResourceTypeType,
+    },
+)
+
+EnvironmentAccountConnectionSummaryTypeDef = TypedDict(
+    "EnvironmentAccountConnectionSummaryTypeDef",
     {
         "arn": str,
+        "componentRoleArn": str,
         "environmentAccountId": str,
         "environmentName": str,
         "id": str,
         "lastModifiedAt": datetime,
         "managementAccountId": str,
         "requestedAt": datetime,
         "roleArn": str,
         "status": EnvironmentAccountConnectionStatusType,
     },
 )
-_OptionalEnvironmentAccountConnectionSummaryTypeDef = TypedDict(
-    "_OptionalEnvironmentAccountConnectionSummaryTypeDef",
-    {
-        "componentRoleArn": str,
-    },
-    total=False,
-)
 
-class EnvironmentAccountConnectionSummaryTypeDef(
-    _RequiredEnvironmentAccountConnectionSummaryTypeDef,
-    _OptionalEnvironmentAccountConnectionSummaryTypeDef,
-):
-    pass
-
-_RequiredEnvironmentSummaryTypeDef = TypedDict(
-    "_RequiredEnvironmentSummaryTypeDef",
+EnvironmentSummaryTypeDef = TypedDict(
+    "EnvironmentSummaryTypeDef",
     {
         "arn": str,
+        "componentRoleArn": str,
         "createdAt": datetime,
         "deploymentStatus": DeploymentStatusType,
-        "lastDeploymentAttemptedAt": datetime,
-        "lastDeploymentSucceededAt": datetime,
-        "name": str,
-        "templateMajorVersion": str,
-        "templateMinorVersion": str,
-        "templateName": str,
-    },
-)
-_OptionalEnvironmentSummaryTypeDef = TypedDict(
-    "_OptionalEnvironmentSummaryTypeDef",
-    {
-        "componentRoleArn": str,
         "deploymentStatusMessage": str,
         "description": str,
         "environmentAccountConnectionId": str,
         "environmentAccountId": str,
+        "lastAttemptedDeploymentId": str,
+        "lastDeploymentAttemptedAt": datetime,
+        "lastDeploymentSucceededAt": datetime,
+        "lastSucceededDeploymentId": str,
+        "name": str,
         "protonServiceRoleArn": str,
         "provisioning": Literal["CUSTOMER_MANAGED"],
+        "templateMajorVersion": str,
+        "templateMinorVersion": str,
+        "templateName": str,
     },
-    total=False,
 )
 
-class EnvironmentSummaryTypeDef(
-    _RequiredEnvironmentSummaryTypeDef, _OptionalEnvironmentSummaryTypeDef
-):
-    pass
-
 EnvironmentTemplateFilterTypeDef = TypedDict(
     "EnvironmentTemplateFilterTypeDef",
     {
         "majorVersion": str,
         "templateName": str,
     },
 )
 
-_RequiredEnvironmentTemplateSummaryTypeDef = TypedDict(
-    "_RequiredEnvironmentTemplateSummaryTypeDef",
+EnvironmentTemplateSummaryTypeDef = TypedDict(
+    "EnvironmentTemplateSummaryTypeDef",
     {
         "arn": str,
         "createdAt": datetime,
-        "lastModifiedAt": datetime,
-        "name": str,
-    },
-)
-_OptionalEnvironmentTemplateSummaryTypeDef = TypedDict(
-    "_OptionalEnvironmentTemplateSummaryTypeDef",
-    {
         "description": str,
         "displayName": str,
+        "lastModifiedAt": datetime,
+        "name": str,
         "provisioning": Literal["CUSTOMER_MANAGED"],
         "recommendedVersion": str,
     },
-    total=False,
 )
 
-class EnvironmentTemplateSummaryTypeDef(
-    _RequiredEnvironmentTemplateSummaryTypeDef, _OptionalEnvironmentTemplateSummaryTypeDef
-):
-    pass
-
-_RequiredEnvironmentTemplateVersionSummaryTypeDef = TypedDict(
-    "_RequiredEnvironmentTemplateVersionSummaryTypeDef",
+EnvironmentTemplateVersionSummaryTypeDef = TypedDict(
+    "EnvironmentTemplateVersionSummaryTypeDef",
     {
         "arn": str,
         "createdAt": datetime,
+        "description": str,
         "lastModifiedAt": datetime,
         "majorVersion": str,
         "minorVersion": str,
+        "recommendedMinorVersion": str,
         "status": TemplateVersionStatusType,
+        "statusMessage": str,
         "templateName": str,
     },
 )
-_OptionalEnvironmentTemplateVersionSummaryTypeDef = TypedDict(
-    "_OptionalEnvironmentTemplateVersionSummaryTypeDef",
-    {
-        "description": str,
-        "recommendedMinorVersion": str,
-        "statusMessage": str,
-    },
-    total=False,
-)
-
-class EnvironmentTemplateVersionSummaryTypeDef(
-    _RequiredEnvironmentTemplateVersionSummaryTypeDef,
-    _OptionalEnvironmentTemplateVersionSummaryTypeDef,
-):
-    pass
 
 WaiterConfigTypeDef = TypedDict(
     "WaiterConfigTypeDef",
     {
         "Delay": int,
         "MaxAttempts": int,
     },
@@ -912,14 +853,36 @@
 GetComponentInputRequestTypeDef = TypedDict(
     "GetComponentInputRequestTypeDef",
     {
         "name": str,
     },
 )
 
+_RequiredGetDeploymentInputRequestTypeDef = TypedDict(
+    "_RequiredGetDeploymentInputRequestTypeDef",
+    {
+        "id": str,
+    },
+)
+_OptionalGetDeploymentInputRequestTypeDef = TypedDict(
+    "_OptionalGetDeploymentInputRequestTypeDef",
+    {
+        "componentName": str,
+        "environmentName": str,
+        "serviceInstanceName": str,
+        "serviceName": str,
+    },
+    total=False,
+)
+
+class GetDeploymentInputRequestTypeDef(
+    _RequiredGetDeploymentInputRequestTypeDef, _OptionalGetDeploymentInputRequestTypeDef
+):
+    pass
+
 GetEnvironmentAccountConnectionInputRequestTypeDef = TypedDict(
     "GetEnvironmentAccountConnectionInputRequestTypeDef",
     {
         "id": str,
     },
 )
 
@@ -1063,14 +1026,15 @@
     {
         "componentName": str,
     },
 )
 _OptionalListComponentOutputsInputListComponentOutputsPaginateTypeDef = TypedDict(
     "_OptionalListComponentOutputsInputListComponentOutputsPaginateTypeDef",
     {
+        "deploymentId": str,
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 class ListComponentOutputsInputListComponentOutputsPaginateTypeDef(
     _RequiredListComponentOutputsInputListComponentOutputsPaginateTypeDef,
@@ -1083,14 +1047,15 @@
     {
         "componentName": str,
     },
 )
 _OptionalListComponentOutputsInputRequestTypeDef = TypedDict(
     "_OptionalListComponentOutputsInputRequestTypeDef",
     {
+        "deploymentId": str,
         "nextToken": str,
     },
     total=False,
 )
 
 class ListComponentOutputsInputRequestTypeDef(
     _RequiredListComponentOutputsInputRequestTypeDef,
@@ -1100,15 +1065,14 @@
 
 OutputTypeDef = TypedDict(
     "OutputTypeDef",
     {
         "key": str,
         "valueString": str,
     },
-    total=False,
 )
 
 _RequiredListComponentProvisionedResourcesInputListComponentProvisionedResourcesPaginateTypeDef = TypedDict(
     "_RequiredListComponentProvisionedResourcesInputListComponentProvisionedResourcesPaginateTypeDef",
     {
         "componentName": str,
     },
@@ -1150,15 +1114,14 @@
 ProvisionedResourceTypeDef = TypedDict(
     "ProvisionedResourceTypeDef",
     {
         "identifier": str,
         "name": str,
         "provisioningEngine": ProvisionedResourceEngineType,
     },
-    total=False,
 )
 
 ListComponentsInputListComponentsPaginateTypeDef = TypedDict(
     "ListComponentsInputListComponentsPaginateTypeDef",
     {
         "environmentName": str,
         "serviceInstanceName": str,
@@ -1176,14 +1139,39 @@
         "nextToken": str,
         "serviceInstanceName": str,
         "serviceName": str,
     },
     total=False,
 )
 
+ListDeploymentsInputListDeploymentsPaginateTypeDef = TypedDict(
+    "ListDeploymentsInputListDeploymentsPaginateTypeDef",
+    {
+        "componentName": str,
+        "environmentName": str,
+        "serviceInstanceName": str,
+        "serviceName": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+ListDeploymentsInputRequestTypeDef = TypedDict(
+    "ListDeploymentsInputRequestTypeDef",
+    {
+        "componentName": str,
+        "environmentName": str,
+        "maxResults": int,
+        "nextToken": str,
+        "serviceInstanceName": str,
+        "serviceName": str,
+    },
+    total=False,
+)
+
 _RequiredListEnvironmentAccountConnectionsInputListEnvironmentAccountConnectionsPaginateTypeDef = TypedDict(
     "_RequiredListEnvironmentAccountConnectionsInputListEnvironmentAccountConnectionsPaginateTypeDef",
     {
         "requestedBy": EnvironmentAccountConnectionRequesterAccountTypeType,
     },
 )
 _OptionalListEnvironmentAccountConnectionsInputListEnvironmentAccountConnectionsPaginateTypeDef = TypedDict(
@@ -1230,14 +1218,15 @@
     {
         "environmentName": str,
     },
 )
 _OptionalListEnvironmentOutputsInputListEnvironmentOutputsPaginateTypeDef = TypedDict(
     "_OptionalListEnvironmentOutputsInputListEnvironmentOutputsPaginateTypeDef",
     {
+        "deploymentId": str,
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 class ListEnvironmentOutputsInputListEnvironmentOutputsPaginateTypeDef(
     _RequiredListEnvironmentOutputsInputListEnvironmentOutputsPaginateTypeDef,
@@ -1250,14 +1239,15 @@
     {
         "environmentName": str,
     },
 )
 _OptionalListEnvironmentOutputsInputRequestTypeDef = TypedDict(
     "_OptionalListEnvironmentOutputsInputRequestTypeDef",
     {
+        "deploymentId": str,
         "nextToken": str,
     },
     total=False,
 )
 
 class ListEnvironmentOutputsInputRequestTypeDef(
     _RequiredListEnvironmentOutputsInputRequestTypeDef,
@@ -1452,14 +1442,15 @@
         "serviceInstanceName": str,
         "serviceName": str,
     },
 )
 _OptionalListServiceInstanceOutputsInputListServiceInstanceOutputsPaginateTypeDef = TypedDict(
     "_OptionalListServiceInstanceOutputsInputListServiceInstanceOutputsPaginateTypeDef",
     {
+        "deploymentId": str,
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 class ListServiceInstanceOutputsInputListServiceInstanceOutputsPaginateTypeDef(
     _RequiredListServiceInstanceOutputsInputListServiceInstanceOutputsPaginateTypeDef,
@@ -1473,14 +1464,15 @@
         "serviceInstanceName": str,
         "serviceName": str,
     },
 )
 _OptionalListServiceInstanceOutputsInputRequestTypeDef = TypedDict(
     "_OptionalListServiceInstanceOutputsInputRequestTypeDef",
     {
+        "deploymentId": str,
         "nextToken": str,
     },
     total=False,
 )
 
 class ListServiceInstanceOutputsInputRequestTypeDef(
     _RequiredListServiceInstanceOutputsInputRequestTypeDef,
@@ -1535,52 +1527,44 @@
     {
         "key": ListServiceInstancesFilterByType,
         "value": str,
     },
     total=False,
 )
 
-_RequiredServiceInstanceSummaryTypeDef = TypedDict(
-    "_RequiredServiceInstanceSummaryTypeDef",
+ServiceInstanceSummaryTypeDef = TypedDict(
+    "ServiceInstanceSummaryTypeDef",
     {
         "arn": str,
         "createdAt": datetime,
         "deploymentStatus": DeploymentStatusType,
+        "deploymentStatusMessage": str,
         "environmentName": str,
+        "lastAttemptedDeploymentId": str,
         "lastDeploymentAttemptedAt": datetime,
         "lastDeploymentSucceededAt": datetime,
+        "lastSucceededDeploymentId": str,
         "name": str,
         "serviceName": str,
         "templateMajorVersion": str,
         "templateMinorVersion": str,
         "templateName": str,
     },
 )
-_OptionalServiceInstanceSummaryTypeDef = TypedDict(
-    "_OptionalServiceInstanceSummaryTypeDef",
-    {
-        "deploymentStatusMessage": str,
-    },
-    total=False,
-)
-
-class ServiceInstanceSummaryTypeDef(
-    _RequiredServiceInstanceSummaryTypeDef, _OptionalServiceInstanceSummaryTypeDef
-):
-    pass
 
 _RequiredListServicePipelineOutputsInputListServicePipelineOutputsPaginateTypeDef = TypedDict(
     "_RequiredListServicePipelineOutputsInputListServicePipelineOutputsPaginateTypeDef",
     {
         "serviceName": str,
     },
 )
 _OptionalListServicePipelineOutputsInputListServicePipelineOutputsPaginateTypeDef = TypedDict(
     "_OptionalListServicePipelineOutputsInputListServicePipelineOutputsPaginateTypeDef",
     {
+        "deploymentId": str,
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 class ListServicePipelineOutputsInputListServicePipelineOutputsPaginateTypeDef(
     _RequiredListServicePipelineOutputsInputListServicePipelineOutputsPaginateTypeDef,
@@ -1593,14 +1577,15 @@
     {
         "serviceName": str,
     },
 )
 _OptionalListServicePipelineOutputsInputRequestTypeDef = TypedDict(
     "_OptionalListServicePipelineOutputsInputRequestTypeDef",
     {
+        "deploymentId": str,
         "nextToken": str,
     },
     total=False,
 )
 
 class ListServicePipelineOutputsInputRequestTypeDef(
     _RequiredListServicePipelineOutputsInputRequestTypeDef,
@@ -1687,41 +1672,30 @@
 
 class ListServiceTemplateVersionsInputRequestTypeDef(
     _RequiredListServiceTemplateVersionsInputRequestTypeDef,
     _OptionalListServiceTemplateVersionsInputRequestTypeDef,
 ):
     pass
 
-_RequiredServiceTemplateVersionSummaryTypeDef = TypedDict(
-    "_RequiredServiceTemplateVersionSummaryTypeDef",
+ServiceTemplateVersionSummaryTypeDef = TypedDict(
+    "ServiceTemplateVersionSummaryTypeDef",
     {
         "arn": str,
         "createdAt": datetime,
+        "description": str,
         "lastModifiedAt": datetime,
         "majorVersion": str,
         "minorVersion": str,
-        "status": TemplateVersionStatusType,
-        "templateName": str,
-    },
-)
-_OptionalServiceTemplateVersionSummaryTypeDef = TypedDict(
-    "_OptionalServiceTemplateVersionSummaryTypeDef",
-    {
-        "description": str,
         "recommendedMinorVersion": str,
+        "status": TemplateVersionStatusType,
         "statusMessage": str,
+        "templateName": str,
     },
-    total=False,
 )
 
-class ServiceTemplateVersionSummaryTypeDef(
-    _RequiredServiceTemplateVersionSummaryTypeDef, _OptionalServiceTemplateVersionSummaryTypeDef
-):
-    pass
-
 ListServiceTemplatesInputListServiceTemplatesPaginateTypeDef = TypedDict(
     "ListServiceTemplatesInputListServiceTemplatesPaginateTypeDef",
     {
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
@@ -1731,39 +1705,28 @@
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-_RequiredServiceTemplateSummaryTypeDef = TypedDict(
-    "_RequiredServiceTemplateSummaryTypeDef",
+ServiceTemplateSummaryTypeDef = TypedDict(
+    "ServiceTemplateSummaryTypeDef",
     {
         "arn": str,
         "createdAt": datetime,
-        "lastModifiedAt": datetime,
-        "name": str,
-    },
-)
-_OptionalServiceTemplateSummaryTypeDef = TypedDict(
-    "_OptionalServiceTemplateSummaryTypeDef",
-    {
         "description": str,
         "displayName": str,
+        "lastModifiedAt": datetime,
+        "name": str,
         "pipelineProvisioning": Literal["CUSTOMER_MANAGED"],
         "recommendedVersion": str,
     },
-    total=False,
 )
 
-class ServiceTemplateSummaryTypeDef(
-    _RequiredServiceTemplateSummaryTypeDef, _OptionalServiceTemplateSummaryTypeDef
-):
-    pass
-
 ListServicesInputListServicesPaginateTypeDef = TypedDict(
     "ListServicesInputListServicesPaginateTypeDef",
     {
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
@@ -1773,36 +1736,27 @@
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-_RequiredServiceSummaryTypeDef = TypedDict(
-    "_RequiredServiceSummaryTypeDef",
+ServiceSummaryTypeDef = TypedDict(
+    "ServiceSummaryTypeDef",
     {
         "arn": str,
         "createdAt": datetime,
+        "description": str,
         "lastModifiedAt": datetime,
         "name": str,
         "status": ServiceStatusType,
+        "statusMessage": str,
         "templateName": str,
     },
 )
-_OptionalServiceSummaryTypeDef = TypedDict(
-    "_OptionalServiceSummaryTypeDef",
-    {
-        "description": str,
-        "statusMessage": str,
-    },
-    total=False,
-)
-
-class ServiceSummaryTypeDef(_RequiredServiceSummaryTypeDef, _OptionalServiceSummaryTypeDef):
-    pass
 
 _RequiredListTagsForResourceInputListTagsForResourcePaginateTypeDef = TypedDict(
     "_RequiredListTagsForResourceInputListTagsForResourcePaginateTypeDef",
     {
         "resourceArn": str,
     },
 )
@@ -1853,55 +1807,33 @@
 RejectEnvironmentAccountConnectionInputRequestTypeDef = TypedDict(
     "RejectEnvironmentAccountConnectionInputRequestTypeDef",
     {
         "id": str,
     },
 )
 
-_RequiredRepositorySyncEventTypeDef = TypedDict(
-    "_RequiredRepositorySyncEventTypeDef",
+RepositorySyncEventTypeDef = TypedDict(
+    "RepositorySyncEventTypeDef",
     {
         "event": str,
+        "externalId": str,
         "time": datetime,
         "type": str,
     },
 )
-_OptionalRepositorySyncEventTypeDef = TypedDict(
-    "_OptionalRepositorySyncEventTypeDef",
-    {
-        "externalId": str,
-    },
-    total=False,
-)
 
-class RepositorySyncEventTypeDef(
-    _RequiredRepositorySyncEventTypeDef, _OptionalRepositorySyncEventTypeDef
-):
-    pass
-
-_RequiredResourceSyncEventTypeDef = TypedDict(
-    "_RequiredResourceSyncEventTypeDef",
+ResourceSyncEventTypeDef = TypedDict(
+    "ResourceSyncEventTypeDef",
     {
         "event": str,
+        "externalId": str,
         "time": datetime,
         "type": str,
     },
 )
-_OptionalResourceSyncEventTypeDef = TypedDict(
-    "_OptionalResourceSyncEventTypeDef",
-    {
-        "externalId": str,
-    },
-    total=False,
-)
-
-class ResourceSyncEventTypeDef(
-    _RequiredResourceSyncEventTypeDef, _OptionalResourceSyncEventTypeDef
-):
-    pass
 
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
         "HTTPStatusCode": int,
@@ -2208,51 +2140,43 @@
 AccountSettingsTypeDef = TypedDict(
     "AccountSettingsTypeDef",
     {
         "pipelineCodebuildRoleArn": str,
         "pipelineProvisioningRepository": RepositoryBranchTypeDef,
         "pipelineServiceRoleArn": str,
     },
-    total=False,
 )
 
-_RequiredEnvironmentTypeDef = TypedDict(
-    "_RequiredEnvironmentTypeDef",
+EnvironmentTypeDef = TypedDict(
+    "EnvironmentTypeDef",
     {
         "arn": str,
-        "createdAt": datetime,
-        "deploymentStatus": DeploymentStatusType,
-        "lastDeploymentAttemptedAt": datetime,
-        "lastDeploymentSucceededAt": datetime,
-        "name": str,
-        "templateMajorVersion": str,
-        "templateMinorVersion": str,
-        "templateName": str,
-    },
-)
-_OptionalEnvironmentTypeDef = TypedDict(
-    "_OptionalEnvironmentTypeDef",
-    {
         "codebuildRoleArn": str,
         "componentRoleArn": str,
+        "createdAt": datetime,
+        "deploymentStatus": DeploymentStatusType,
         "deploymentStatusMessage": str,
         "description": str,
         "environmentAccountConnectionId": str,
         "environmentAccountId": str,
+        "lastAttemptedDeploymentId": str,
+        "lastDeploymentAttemptedAt": datetime,
+        "lastDeploymentSucceededAt": datetime,
+        "lastSucceededDeploymentId": str,
+        "name": str,
         "protonServiceRoleArn": str,
         "provisioning": Literal["CUSTOMER_MANAGED"],
         "provisioningRepository": RepositoryBranchTypeDef,
         "spec": str,
+        "templateMajorVersion": str,
+        "templateMinorVersion": str,
+        "templateName": str,
     },
-    total=False,
 )
 
-class EnvironmentTypeDef(_RequiredEnvironmentTypeDef, _OptionalEnvironmentTypeDef):
-    pass
-
 CancelComponentDeploymentOutputTypeDef = TypedDict(
     "CancelComponentDeploymentOutputTypeDef",
     {
         "component": ComponentTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -2325,42 +2249,33 @@
     "CancelServicePipelineDeploymentOutputTypeDef",
     {
         "pipeline": ServicePipelineTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredServiceTypeDef = TypedDict(
-    "_RequiredServiceTypeDef",
+ServiceTypeDef = TypedDict(
+    "ServiceTypeDef",
     {
         "arn": str,
+        "branchName": str,
         "createdAt": datetime,
+        "description": str,
         "lastModifiedAt": datetime,
         "name": str,
-        "spec": str,
-        "status": ServiceStatusType,
-        "templateName": str,
-    },
-)
-_OptionalServiceTypeDef = TypedDict(
-    "_OptionalServiceTypeDef",
-    {
-        "branchName": str,
-        "description": str,
         "pipeline": ServicePipelineTypeDef,
         "repositoryConnectionArn": str,
         "repositoryId": str,
+        "spec": str,
+        "status": ServiceStatusType,
         "statusMessage": str,
+        "templateName": str,
     },
-    total=False,
 )
 
-class ServiceTypeDef(_RequiredServiceTypeDef, _OptionalServiceTypeDef):
-    pass
-
 UpdateServicePipelineOutputTypeDef = TypedDict(
     "UpdateServicePipelineOutputTypeDef",
     {
         "pipeline": ServicePipelineTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -2386,44 +2301,33 @@
 
 class UpdateServiceTemplateVersionInputRequestTypeDef(
     _RequiredUpdateServiceTemplateVersionInputRequestTypeDef,
     _OptionalUpdateServiceTemplateVersionInputRequestTypeDef,
 ):
     pass
 
-_RequiredServiceTemplateVersionTypeDef = TypedDict(
-    "_RequiredServiceTemplateVersionTypeDef",
+ServiceTemplateVersionTypeDef = TypedDict(
+    "ServiceTemplateVersionTypeDef",
     {
         "arn": str,
         "compatibleEnvironmentTemplates": List[CompatibleEnvironmentTemplateTypeDef],
         "createdAt": datetime,
+        "description": str,
         "lastModifiedAt": datetime,
         "majorVersion": str,
         "minorVersion": str,
-        "status": TemplateVersionStatusType,
-        "templateName": str,
-    },
-)
-_OptionalServiceTemplateVersionTypeDef = TypedDict(
-    "_OptionalServiceTemplateVersionTypeDef",
-    {
-        "description": str,
         "recommendedMinorVersion": str,
         "schema": str,
+        "status": TemplateVersionStatusType,
         "statusMessage": str,
         "supportedComponentSources": List[Literal["DIRECTLY_DEFINED"]],
+        "templateName": str,
     },
-    total=False,
 )
 
-class ServiceTemplateVersionTypeDef(
-    _RequiredServiceTemplateVersionTypeDef, _OptionalServiceTemplateVersionTypeDef
-):
-    pass
-
 ListComponentsOutputTypeDef = TypedDict(
     "ListComponentsOutputTypeDef",
     {
         "components": List[ComponentSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -2436,15 +2340,14 @@
         "environmentTemplates": ResourceCountsSummaryTypeDef,
         "environments": ResourceCountsSummaryTypeDef,
         "pipelines": ResourceCountsSummaryTypeDef,
         "serviceInstances": ResourceCountsSummaryTypeDef,
         "serviceTemplates": ResourceCountsSummaryTypeDef,
         "services": ResourceCountsSummaryTypeDef,
     },
-    total=False,
 )
 
 _RequiredCreateComponentInputRequestTypeDef = TypedDict(
     "_RequiredCreateComponentInputRequestTypeDef",
     {
         "manifest": str,
         "name": str,
@@ -2882,14 +2785,33 @@
     "UpdateTemplateSyncConfigOutputTypeDef",
     {
         "templateSyncConfig": TemplateSyncConfigTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+DeploymentStateTypeDef = TypedDict(
+    "DeploymentStateTypeDef",
+    {
+        "component": ComponentStateTypeDef,
+        "environment": EnvironmentStateTypeDef,
+        "serviceInstance": ServiceInstanceStateTypeDef,
+        "servicePipeline": ServicePipelineStateTypeDef,
+    },
+)
+
+ListDeploymentsOutputTypeDef = TypedDict(
+    "ListDeploymentsOutputTypeDef",
+    {
+        "deployments": List[DeploymentSummaryTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ListEnvironmentAccountConnectionsOutputTypeDef = TypedDict(
     "ListEnvironmentAccountConnectionsOutputTypeDef",
     {
         "environmentAccountConnections": List[EnvironmentAccountConnectionSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -3345,37 +3267,28 @@
     "TemplateVersionSourceInputTypeDef",
     {
         "s3": S3ObjectSourceTypeDef,
     },
     total=False,
 )
 
-_RequiredSyncBlockerTypeDef = TypedDict(
-    "_RequiredSyncBlockerTypeDef",
+SyncBlockerTypeDef = TypedDict(
+    "SyncBlockerTypeDef",
     {
+        "contexts": List[SyncBlockerContextTypeDef],
         "createdAt": datetime,
         "createdReason": str,
         "id": str,
-        "status": BlockerStatusType,
-        "type": Literal["AUTOMATED"],
-    },
-)
-_OptionalSyncBlockerTypeDef = TypedDict(
-    "_OptionalSyncBlockerTypeDef",
-    {
-        "contexts": List[SyncBlockerContextTypeDef],
         "resolvedAt": datetime,
         "resolvedReason": str,
+        "status": BlockerStatusType,
+        "type": Literal["AUTOMATED"],
     },
-    total=False,
 )
 
-class SyncBlockerTypeDef(_RequiredSyncBlockerTypeDef, _OptionalSyncBlockerTypeDef):
-    pass
-
 GetAccountSettingsOutputTypeDef = TypedDict(
     "GetAccountSettingsOutputTypeDef",
     {
         "accountSettings": AccountSettingsTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -3496,14 +3409,38 @@
     "GetResourcesSummaryOutputTypeDef",
     {
         "counts": CountsSummaryTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+DeploymentTypeDef = TypedDict(
+    "DeploymentTypeDef",
+    {
+        "arn": str,
+        "completedAt": datetime,
+        "componentName": str,
+        "createdAt": datetime,
+        "deploymentStatus": DeploymentStatusType,
+        "deploymentStatusMessage": str,
+        "environmentName": str,
+        "id": str,
+        "initialState": DeploymentStateTypeDef,
+        "lastAttemptedDeploymentId": str,
+        "lastModifiedAt": datetime,
+        "lastSucceededDeploymentId": str,
+        "serviceInstanceName": str,
+        "serviceName": str,
+        "targetArn": str,
+        "targetResourceCreatedAt": datetime,
+        "targetResourceType": DeploymentTargetResourceTypeType,
+        "targetState": DeploymentStateTypeDef,
+    },
+)
+
 GetRepositorySyncStatusOutputTypeDef = TypedDict(
     "GetRepositorySyncStatusOutputTypeDef",
     {
         "latestSync": RepositorySyncAttemptTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -3574,44 +3511,49 @@
 
 class CreateServiceTemplateVersionInputRequestTypeDef(
     _RequiredCreateServiceTemplateVersionInputRequestTypeDef,
     _OptionalCreateServiceTemplateVersionInputRequestTypeDef,
 ):
     pass
 
-_RequiredServiceSyncBlockerSummaryTypeDef = TypedDict(
-    "_RequiredServiceSyncBlockerSummaryTypeDef",
-    {
-        "serviceName": str,
-    },
-)
-_OptionalServiceSyncBlockerSummaryTypeDef = TypedDict(
-    "_OptionalServiceSyncBlockerSummaryTypeDef",
+ServiceSyncBlockerSummaryTypeDef = TypedDict(
+    "ServiceSyncBlockerSummaryTypeDef",
     {
         "latestBlockers": List[SyncBlockerTypeDef],
         "serviceInstanceName": str,
+        "serviceName": str,
     },
-    total=False,
 )
 
-class ServiceSyncBlockerSummaryTypeDef(
-    _RequiredServiceSyncBlockerSummaryTypeDef, _OptionalServiceSyncBlockerSummaryTypeDef
-):
-    pass
-
 UpdateServiceSyncBlockerOutputTypeDef = TypedDict(
     "UpdateServiceSyncBlockerOutputTypeDef",
     {
         "serviceInstanceName": str,
         "serviceName": str,
         "serviceSyncBlocker": SyncBlockerTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+DeleteDeploymentOutputTypeDef = TypedDict(
+    "DeleteDeploymentOutputTypeDef",
+    {
+        "deployment": DeploymentTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+GetDeploymentOutputTypeDef = TypedDict(
+    "GetDeploymentOutputTypeDef",
+    {
+        "deployment": DeploymentTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetServiceSyncBlockerSummaryOutputTypeDef = TypedDict(
     "GetServiceSyncBlockerSummaryOutputTypeDef",
     {
         "serviceSyncBlockerSummary": ServiceSyncBlockerSummaryTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-proton-1.28.0/mypy_boto3_proton/waiter.py` & `mypy-boto3-proton-1.28.3/mypy_boto3_proton/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-proton-1.28.0/mypy_boto3_proton/waiter.pyi` & `mypy-boto3-proton-1.28.3/mypy_boto3_proton/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-proton-1.28.0/mypy_boto3_proton.egg-info/PKG-INFO` & `mypy-boto3-proton-1.28.3/mypy_boto3_proton.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-proton
-Version: 1.28.0
-Summary: Type annotations for boto3.Proton 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.3
+Summary: Type annotations for boto3.Proton 1.28.3 service generated with mypy-boto3-builder 7.14.6
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-proton.svg?color=blue)](https://pypi.org/project/mypy-boto3-proton)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-proton?color=blue)](https://pypistats.org/packages/mypy-boto3-proton)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Proton 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton)
+[boto3.Proton 1.28.3](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton)
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
 [mypy-boto3-proton docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_proton/).
 
 See how it helps to find and fix potential bugs:
 
@@ -283,14 +283,15 @@
 from boto3.session import Session
 
 from mypy_boto3_proton import ProtonClient
 from mypy_boto3_proton.paginator import (
     ListComponentOutputsPaginator,
     ListComponentProvisionedResourcesPaginator,
     ListComponentsPaginator,
+    ListDeploymentsPaginator,
     ListEnvironmentAccountConnectionsPaginator,
     ListEnvironmentOutputsPaginator,
     ListEnvironmentProvisionedResourcesPaginator,
     ListEnvironmentTemplateVersionsPaginator,
     ListEnvironmentTemplatesPaginator,
     ListEnvironmentsPaginator,
     ListRepositoriesPaginator,
@@ -313,14 +314,15 @@
 list_component_outputs_paginator: ListComponentOutputsPaginator = client.get_paginator(
     "list_component_outputs"
 )
 list_component_provisioned_resources_paginator: ListComponentProvisionedResourcesPaginator = (
     client.get_paginator("list_component_provisioned_resources")
 )
 list_components_paginator: ListComponentsPaginator = client.get_paginator("list_components")
+list_deployments_paginator: ListDeploymentsPaginator = client.get_paginator("list_deployments")
 list_environment_account_connections_paginator: ListEnvironmentAccountConnectionsPaginator = (
     client.get_paginator("list_environment_account_connections")
 )
 list_environment_outputs_paginator: ListEnvironmentOutputsPaginator = client.get_paginator(
     "list_environment_outputs"
 )
 list_environment_provisioned_resources_paginator: ListEnvironmentProvisionedResourcesPaginator = (
@@ -422,22 +424,24 @@
 from mypy_boto3_proton.literals import (
     BlockerStatusType,
     BlockerTypeType,
     ComponentDeletedWaiterName,
     ComponentDeployedWaiterName,
     ComponentDeploymentUpdateTypeType,
     DeploymentStatusType,
+    DeploymentTargetResourceTypeType,
     DeploymentUpdateTypeType,
     EnvironmentAccountConnectionRequesterAccountTypeType,
     EnvironmentAccountConnectionStatusType,
     EnvironmentDeployedWaiterName,
     EnvironmentTemplateVersionRegisteredWaiterName,
     ListComponentOutputsPaginatorName,
     ListComponentProvisionedResourcesPaginatorName,
     ListComponentsPaginatorName,
+    ListDeploymentsPaginatorName,
     ListEnvironmentAccountConnectionsPaginatorName,
     ListEnvironmentOutputsPaginatorName,
     ListEnvironmentProvisionedResourcesPaginatorName,
     ListEnvironmentTemplateVersionsPaginatorName,
     ListEnvironmentTemplatesPaginatorName,
     ListEnvironmentsPaginatorName,
     ListRepositoriesPaginatorName,
@@ -501,44 +505,51 @@
     CancelEnvironmentDeploymentInputRequestTypeDef,
     CancelServiceInstanceDeploymentInputRequestTypeDef,
     ServiceInstanceTypeDef,
     CancelServicePipelineDeploymentInputRequestTypeDef,
     ServicePipelineTypeDef,
     CompatibleEnvironmentTemplateInputTypeDef,
     CompatibleEnvironmentTemplateTypeDef,
+    ComponentStateTypeDef,
     ComponentSummaryTypeDef,
     ResourceCountsSummaryTypeDef,
     TagTypeDef,
     RepositoryBranchInputTypeDef,
     EnvironmentTemplateTypeDef,
     EnvironmentTemplateVersionTypeDef,
     RepositoryTypeDef,
     CreateServiceSyncConfigInputRequestTypeDef,
     ServiceSyncConfigTypeDef,
     ServiceTemplateTypeDef,
     CreateTemplateSyncConfigInputRequestTypeDef,
     TemplateSyncConfigTypeDef,
     DeleteComponentInputRequestTypeDef,
+    DeleteDeploymentInputRequestTypeDef,
     DeleteEnvironmentAccountConnectionInputRequestTypeDef,
     DeleteEnvironmentInputRequestTypeDef,
     DeleteEnvironmentTemplateInputRequestTypeDef,
     DeleteEnvironmentTemplateVersionInputRequestTypeDef,
     DeleteRepositoryInputRequestTypeDef,
     DeleteServiceInputRequestTypeDef,
     DeleteServiceSyncConfigInputRequestTypeDef,
     DeleteServiceTemplateInputRequestTypeDef,
     DeleteServiceTemplateVersionInputRequestTypeDef,
     DeleteTemplateSyncConfigInputRequestTypeDef,
+    EnvironmentStateTypeDef,
+    ServiceInstanceStateTypeDef,
+    ServicePipelineStateTypeDef,
+    DeploymentSummaryTypeDef,
     EnvironmentAccountConnectionSummaryTypeDef,
     EnvironmentSummaryTypeDef,
     EnvironmentTemplateFilterTypeDef,
     EnvironmentTemplateSummaryTypeDef,
     EnvironmentTemplateVersionSummaryTypeDef,
     WaiterConfigTypeDef,
     GetComponentInputRequestTypeDef,
+    GetDeploymentInputRequestTypeDef,
     GetEnvironmentAccountConnectionInputRequestTypeDef,
     GetEnvironmentInputRequestTypeDef,
     GetEnvironmentTemplateInputRequestTypeDef,
     GetEnvironmentTemplateVersionInputRequestTypeDef,
     GetRepositoryInputRequestTypeDef,
     GetRepositorySyncStatusInputRequestTypeDef,
     GetServiceInputRequestTypeDef,
@@ -555,14 +566,16 @@
     ListComponentOutputsInputRequestTypeDef,
     OutputTypeDef,
     ListComponentProvisionedResourcesInputListComponentProvisionedResourcesPaginateTypeDef,
     ListComponentProvisionedResourcesInputRequestTypeDef,
     ProvisionedResourceTypeDef,
     ListComponentsInputListComponentsPaginateTypeDef,
     ListComponentsInputRequestTypeDef,
+    ListDeploymentsInputListDeploymentsPaginateTypeDef,
+    ListDeploymentsInputRequestTypeDef,
     ListEnvironmentAccountConnectionsInputListEnvironmentAccountConnectionsPaginateTypeDef,
     ListEnvironmentAccountConnectionsInputRequestTypeDef,
     ListEnvironmentOutputsInputListEnvironmentOutputsPaginateTypeDef,
     ListEnvironmentOutputsInputRequestTypeDef,
     ListEnvironmentProvisionedResourcesInputListEnvironmentProvisionedResourcesPaginateTypeDef,
     ListEnvironmentProvisionedResourcesInputRequestTypeDef,
     ListEnvironmentTemplateVersionsInputListEnvironmentTemplateVersionsPaginateTypeDef,
@@ -670,14 +683,16 @@
     DeleteServiceTemplateOutputTypeDef,
     GetServiceTemplateOutputTypeDef,
     UpdateServiceTemplateOutputTypeDef,
     CreateTemplateSyncConfigOutputTypeDef,
     DeleteTemplateSyncConfigOutputTypeDef,
     GetTemplateSyncConfigOutputTypeDef,
     UpdateTemplateSyncConfigOutputTypeDef,
+    DeploymentStateTypeDef,
+    ListDeploymentsOutputTypeDef,
     ListEnvironmentAccountConnectionsOutputTypeDef,
     ListEnvironmentsOutputTypeDef,
     ListEnvironmentsInputListEnvironmentsPaginateTypeDef,
     ListEnvironmentsInputRequestTypeDef,
     ListEnvironmentTemplatesOutputTypeDef,
     ListEnvironmentTemplateVersionsOutputTypeDef,
     GetComponentInputComponentDeletedWaitTypeDef,
@@ -723,21 +738,24 @@
     GetServiceOutputTypeDef,
     UpdateServiceOutputTypeDef,
     CreateServiceTemplateVersionOutputTypeDef,
     DeleteServiceTemplateVersionOutputTypeDef,
     GetServiceTemplateVersionOutputTypeDef,
     UpdateServiceTemplateVersionOutputTypeDef,
     GetResourcesSummaryOutputTypeDef,
+    DeploymentTypeDef,
     GetRepositorySyncStatusOutputTypeDef,
     GetServiceInstanceSyncStatusOutputTypeDef,
     GetTemplateSyncStatusOutputTypeDef,
     CreateEnvironmentTemplateVersionInputRequestTypeDef,
     CreateServiceTemplateVersionInputRequestTypeDef,
     ServiceSyncBlockerSummaryTypeDef,
     UpdateServiceSyncBlockerOutputTypeDef,
+    DeleteDeploymentOutputTypeDef,
+    GetDeploymentOutputTypeDef,
     GetServiceSyncBlockerSummaryOutputTypeDef,
 )
 
 
 def get_structure() -> AcceptEnvironmentAccountConnectionInputRequestTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-proton-1.28.0/mypy_boto3_proton.egg-info/SOURCES.txt` & `mypy-boto3-proton-1.28.3/mypy_boto3_proton.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-proton-1.28.0/setup.py` & `mypy-boto3-proton-1.28.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-proton",
-    version="1.28.0",
+    version="1.28.3",
     packages=["mypy_boto3_proton"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Proton 1.28.0 service generated with mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.Proton 1.28.3 service generated with mypy-boto3-builder 7.14.6"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

