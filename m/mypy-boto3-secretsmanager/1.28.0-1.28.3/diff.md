# Comparing `tmp/mypy-boto3-secretsmanager-1.28.0.tar.gz` & `tmp/mypy-boto3-secretsmanager-1.28.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-secretsmanager-1.28.0.tar", last modified: Thu Jul  6 21:00:35 2023, max compression
+gzip compressed data, was "mypy-boto3-secretsmanager-1.28.3.tar", last modified: Thu Jul 13 19:49:15 2023, max compression
```

## Comparing `mypy-boto3-secretsmanager-1.28.0.tar` & `mypy-boto3-secretsmanager-1.28.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:35.614427 mypy-boto3-secretsmanager-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:55:02.000000 mypy-boto3-secretsmanager-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15037 2023-07-06 21:00:35.610427 mypy-boto3-secretsmanager-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13524 2023-07-06 20:55:02.000000 mypy-boto3-secretsmanager-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:35.606427 mypy-boto3-secretsmanager-1.28.0/mypy_boto3_secretsmanager/
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-07-06 20:55:02.000000 mypy-boto3-secretsmanager-1.28.0/mypy_boto3_secretsmanager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-07-06 20:55:02.000000 mypy-boto3-secretsmanager-1.28.0/mypy_boto3_secretsmanager/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-07-06 20:55:02.000000 mypy-boto3-secretsmanager-1.28.0/mypy_boto3_secretsmanager/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18863 2023-07-06 20:55:02.000000 mypy-boto3-secretsmanager-1.28.0/mypy_boto3_secretsmanager/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    18833 2023-07-06 20:55:02.000000 mypy-boto3-secretsmanager-1.28.0/mypy_boto3_secretsmanager/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8578 2023-07-06 20:55:02.000000 mypy-boto3-secretsmanager-1.28.0/mypy_boto3_secretsmanager/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8576 2023-07-06 20:55:02.000000 mypy-boto3-secretsmanager-1.28.0/mypy_boto3_secretsmanager/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-07-06 20:55:02.000000 mypy-boto3-secretsmanager-1.28.0/mypy_boto3_secretsmanager/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-07-06 20:55:02.000000 mypy-boto3-secretsmanager-1.28.0/mypy_boto3_secretsmanager/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:55:02.000000 mypy-boto3-secretsmanager-1.28.0/mypy_boto3_secretsmanager/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    19641 2023-07-06 20:55:07.000000 mypy-boto3-secretsmanager-1.28.0/mypy_boto3_secretsmanager/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    19618 2023-07-06 20:55:06.000000 mypy-boto3-secretsmanager-1.28.0/mypy_boto3_secretsmanager/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:55:02.000000 mypy-boto3-secretsmanager-1.28.0/mypy_boto3_secretsmanager/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:35.610427 mypy-boto3-secretsmanager-1.28.0/mypy_boto3_secretsmanager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15037 2023-07-06 21:00:35.000000 mypy-boto3-secretsmanager-1.28.0/mypy_boto3_secretsmanager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-06 21:00:35.000000 mypy-boto3-secretsmanager-1.28.0/mypy_boto3_secretsmanager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:35.000000 mypy-boto3-secretsmanager-1.28.0/mypy_boto3_secretsmanager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:35.000000 mypy-boto3-secretsmanager-1.28.0/mypy_boto3_secretsmanager.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 21:00:35.000000 mypy-boto3-secretsmanager-1.28.0/mypy_boto3_secretsmanager.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-06 21:00:35.000000 mypy-boto3-secretsmanager-1.28.0/mypy_boto3_secretsmanager.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 21:00:35.614427 mypy-boto3-secretsmanager-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-07-06 20:55:02.000000 mypy-boto3-secretsmanager-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:49:15.173303 mypy-boto3-secretsmanager-1.28.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-13 19:49:00.000000 mypy-boto3-secretsmanager-1.28.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15037 2023-07-13 19:49:15.169303 mypy-boto3-secretsmanager-1.28.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13524 2023-07-13 19:49:00.000000 mypy-boto3-secretsmanager-1.28.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:49:15.165303 mypy-boto3-secretsmanager-1.28.3/mypy_boto3_secretsmanager/
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-07-13 19:49:00.000000 mypy-boto3-secretsmanager-1.28.3/mypy_boto3_secretsmanager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-07-13 19:49:00.000000 mypy-boto3-secretsmanager-1.28.3/mypy_boto3_secretsmanager/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-07-13 19:49:00.000000 mypy-boto3-secretsmanager-1.28.3/mypy_boto3_secretsmanager/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18863 2023-07-13 19:49:00.000000 mypy-boto3-secretsmanager-1.28.3/mypy_boto3_secretsmanager/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18833 2023-07-13 19:49:00.000000 mypy-boto3-secretsmanager-1.28.3/mypy_boto3_secretsmanager/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8578 2023-07-13 19:49:00.000000 mypy-boto3-secretsmanager-1.28.3/mypy_boto3_secretsmanager/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8576 2023-07-13 19:49:00.000000 mypy-boto3-secretsmanager-1.28.3/mypy_boto3_secretsmanager/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-07-13 19:49:00.000000 mypy-boto3-secretsmanager-1.28.3/mypy_boto3_secretsmanager/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-07-13 19:49:00.000000 mypy-boto3-secretsmanager-1.28.3/mypy_boto3_secretsmanager/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 19:49:00.000000 mypy-boto3-secretsmanager-1.28.3/mypy_boto3_secretsmanager/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    19556 2023-07-13 19:49:01.000000 mypy-boto3-secretsmanager-1.28.3/mypy_boto3_secretsmanager/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19533 2023-07-13 19:49:01.000000 mypy-boto3-secretsmanager-1.28.3/mypy_boto3_secretsmanager/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-13 19:49:00.000000 mypy-boto3-secretsmanager-1.28.3/mypy_boto3_secretsmanager/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:49:15.169303 mypy-boto3-secretsmanager-1.28.3/mypy_boto3_secretsmanager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15037 2023-07-13 19:49:15.000000 mypy-boto3-secretsmanager-1.28.3/mypy_boto3_secretsmanager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-13 19:49:15.000000 mypy-boto3-secretsmanager-1.28.3/mypy_boto3_secretsmanager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 19:49:15.000000 mypy-boto3-secretsmanager-1.28.3/mypy_boto3_secretsmanager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 19:49:15.000000 mypy-boto3-secretsmanager-1.28.3/mypy_boto3_secretsmanager.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-13 19:49:15.000000 mypy-boto3-secretsmanager-1.28.3/mypy_boto3_secretsmanager.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-13 19:49:15.000000 mypy-boto3-secretsmanager-1.28.3/mypy_boto3_secretsmanager.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 19:49:15.173303 mypy-boto3-secretsmanager-1.28.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-07-13 19:49:00.000000 mypy-boto3-secretsmanager-1.28.3/setup.py
```

### Comparing `mypy-boto3-secretsmanager-1.28.0/LICENSE` & `mypy-boto3-secretsmanager-1.28.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-secretsmanager-1.28.0/PKG-INFO` & `mypy-boto3-secretsmanager-1.28.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-secretsmanager
-Version: 1.28.0
-Summary: Type annotations for boto3.SecretsManager 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.3
+Summary: Type annotations for boto3.SecretsManager 1.28.3 service generated with mypy-boto3-builder 7.14.6
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_secretsmanager/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-secretsmanager.svg?color=blue)](https://pypi.org/project/mypy-boto3-secretsmanager)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_secretsmanager/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-secretsmanager?color=blue)](https://pypistats.org/packages/mypy-boto3-secretsmanager)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SecretsManager 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#SecretsManager)
+[boto3.SecretsManager 1.28.3](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#SecretsManager)
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
 [mypy-boto3-secretsmanager docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_secretsmanager/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-secretsmanager-1.28.0/README.md` & `mypy-boto3-secretsmanager-1.28.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-secretsmanager.svg?color=blue)](https://pypi.org/project/mypy-boto3-secretsmanager)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_secretsmanager/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-secretsmanager?color=blue)](https://pypistats.org/packages/mypy-boto3-secretsmanager)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SecretsManager 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#SecretsManager)
+[boto3.SecretsManager 1.28.3](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#SecretsManager)
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
 [mypy-boto3-secretsmanager docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_secretsmanager/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-secretsmanager-1.28.0/mypy_boto3_secretsmanager/__init__.py` & `mypy-boto3-secretsmanager-1.28.3/mypy_boto3_secretsmanager/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-secretsmanager-1.28.0/mypy_boto3_secretsmanager/__init__.pyi` & `mypy-boto3-secretsmanager-1.28.3/mypy_boto3_secretsmanager/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-secretsmanager-1.28.0/mypy_boto3_secretsmanager/__main__.py` & `mypy-boto3-secretsmanager-1.28.3/mypy_boto3_secretsmanager/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.SecretsManager 1.28.0\nVersion:         1.28.0\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for boto3.SecretsManager 1.28.3\nVersion:         1.28.3\nBuilder"
+        " version: 7.14.6\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_secretsmanager//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#SecretsManager\nOther"
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

### Comparing `mypy-boto3-secretsmanager-1.28.0/mypy_boto3_secretsmanager/client.py` & `mypy-boto3-secretsmanager-1.28.3/mypy_boto3_secretsmanager/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-secretsmanager-1.28.0/mypy_boto3_secretsmanager/client.pyi` & `mypy-boto3-secretsmanager-1.28.3/mypy_boto3_secretsmanager/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-secretsmanager-1.28.0/mypy_boto3_secretsmanager/literals.py` & `mypy-boto3-secretsmanager-1.28.3/mypy_boto3_secretsmanager/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-secretsmanager-1.28.0/mypy_boto3_secretsmanager/literals.pyi` & `mypy-boto3-secretsmanager-1.28.3/mypy_boto3_secretsmanager/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-secretsmanager-1.28.0/mypy_boto3_secretsmanager/paginator.py` & `mypy-boto3-secretsmanager-1.28.3/mypy_boto3_secretsmanager/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-secretsmanager-1.28.0/mypy_boto3_secretsmanager/paginator.pyi` & `mypy-boto3-secretsmanager-1.28.3/mypy_boto3_secretsmanager/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-secretsmanager-1.28.0/mypy_boto3_secretsmanager/type_defs.py` & `mypy-boto3-secretsmanager-1.28.3/mypy_boto3_secretsmanager/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -122,15 +122,14 @@
     {
         "Region": str,
         "KmsKeyId": str,
         "Status": StatusTypeType,
         "StatusMessage": str,
         "LastAccessedDate": datetime,
     },
-    total=False,
 )
 
 DeleteResourcePolicyRequestRequestTypeDef = TypedDict(
     "DeleteResourcePolicyRequestRequestTypeDef",
     {
         "SecretId": str,
     },
@@ -187,15 +186,14 @@
 RotationRulesTypeTypeDef = TypedDict(
     "RotationRulesTypeTypeDef",
     {
         "AutomaticallyAfterDays": int,
         "Duration": str,
         "ScheduleExpression": str,
     },
-    total=False,
 )
 
 EmptyResponseMetadataTypeDef = TypedDict(
     "EmptyResponseMetadataTypeDef",
     {
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -315,15 +313,14 @@
     {
         "VersionId": str,
         "VersionStages": List[str],
         "LastAccessedDate": datetime,
         "CreatedDate": datetime,
         "KmsKeyIds": List[str],
     },
-    total=False,
 )
 
 PaginatorConfigTypeDef = TypedDict(
     "PaginatorConfigTypeDef",
     {
         "MaxItems": int,
         "PageSize": int,
@@ -558,15 +555,14 @@
 
 ValidationErrorsEntryTypeDef = TypedDict(
     "ValidationErrorsEntryTypeDef",
     {
         "CheckName": str,
         "ErrorMessage": str,
     },
-    total=False,
 )
 
 _RequiredReplicateSecretToRegionsRequestRequestTypeDef = TypedDict(
     "_RequiredReplicateSecretToRegionsRequestRequestTypeDef",
     {
         "SecretId": str,
         "AddReplicaRegions": Sequence[ReplicaRegionTypeTypeDef],
@@ -719,15 +715,14 @@
         "NextRotationDate": datetime,
         "Tags": List[TagTypeDef],
         "SecretVersionsToStages": Dict[str, List[str]],
         "OwningService": str,
         "CreatedDate": datetime,
         "PrimaryRegion": str,
     },
-    total=False,
 )
 
 ListSecretsRequestListSecretsPaginateTypeDef = TypedDict(
     "ListSecretsRequestListSecretsPaginateTypeDef",
     {
         "IncludePlannedDeletion": bool,
         "Filters": Sequence[FilterTypeDef],
```

### Comparing `mypy-boto3-secretsmanager-1.28.0/mypy_boto3_secretsmanager/type_defs.pyi` & `mypy-boto3-secretsmanager-1.28.3/mypy_boto3_secretsmanager/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -121,15 +121,14 @@
     {
         "Region": str,
         "KmsKeyId": str,
         "Status": StatusTypeType,
         "StatusMessage": str,
         "LastAccessedDate": datetime,
     },
-    total=False,
 )
 
 DeleteResourcePolicyRequestRequestTypeDef = TypedDict(
     "DeleteResourcePolicyRequestRequestTypeDef",
     {
         "SecretId": str,
     },
@@ -184,15 +183,14 @@
 RotationRulesTypeTypeDef = TypedDict(
     "RotationRulesTypeTypeDef",
     {
         "AutomaticallyAfterDays": int,
         "Duration": str,
         "ScheduleExpression": str,
     },
-    total=False,
 )
 
 EmptyResponseMetadataTypeDef = TypedDict(
     "EmptyResponseMetadataTypeDef",
     {
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -308,15 +306,14 @@
     {
         "VersionId": str,
         "VersionStages": List[str],
         "LastAccessedDate": datetime,
         "CreatedDate": datetime,
         "KmsKeyIds": List[str],
     },
-    total=False,
 )
 
 PaginatorConfigTypeDef = TypedDict(
     "PaginatorConfigTypeDef",
     {
         "MaxItems": int,
         "PageSize": int,
@@ -541,15 +538,14 @@
 
 ValidationErrorsEntryTypeDef = TypedDict(
     "ValidationErrorsEntryTypeDef",
     {
         "CheckName": str,
         "ErrorMessage": str,
     },
-    total=False,
 )
 
 _RequiredReplicateSecretToRegionsRequestRequestTypeDef = TypedDict(
     "_RequiredReplicateSecretToRegionsRequestRequestTypeDef",
     {
         "SecretId": str,
         "AddReplicaRegions": Sequence[ReplicaRegionTypeTypeDef],
@@ -696,15 +692,14 @@
         "NextRotationDate": datetime,
         "Tags": List[TagTypeDef],
         "SecretVersionsToStages": Dict[str, List[str]],
         "OwningService": str,
         "CreatedDate": datetime,
         "PrimaryRegion": str,
     },
-    total=False,
 )
 
 ListSecretsRequestListSecretsPaginateTypeDef = TypedDict(
     "ListSecretsRequestListSecretsPaginateTypeDef",
     {
         "IncludePlannedDeletion": bool,
         "Filters": Sequence[FilterTypeDef],
```

### Comparing `mypy-boto3-secretsmanager-1.28.0/mypy_boto3_secretsmanager.egg-info/PKG-INFO` & `mypy-boto3-secretsmanager-1.28.3/mypy_boto3_secretsmanager.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-secretsmanager
-Version: 1.28.0
-Summary: Type annotations for boto3.SecretsManager 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.3
+Summary: Type annotations for boto3.SecretsManager 1.28.3 service generated with mypy-boto3-builder 7.14.6
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_secretsmanager/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-secretsmanager.svg?color=blue)](https://pypi.org/project/mypy-boto3-secretsmanager)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_secretsmanager/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-secretsmanager?color=blue)](https://pypistats.org/packages/mypy-boto3-secretsmanager)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SecretsManager 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#SecretsManager)
+[boto3.SecretsManager 1.28.3](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#SecretsManager)
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
 [mypy-boto3-secretsmanager docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_secretsmanager/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-secretsmanager-1.28.0/mypy_boto3_secretsmanager.egg-info/SOURCES.txt` & `mypy-boto3-secretsmanager-1.28.3/mypy_boto3_secretsmanager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-secretsmanager-1.28.0/setup.py` & `mypy-boto3-secretsmanager-1.28.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-secretsmanager",
-    version="1.28.0",
+    version="1.28.3",
     packages=["mypy_boto3_secretsmanager"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.SecretsManager 1.28.0 service generated with mypy-boto3-builder"
-        " 7.14.5"
+        "Type annotations for boto3.SecretsManager 1.28.3 service generated with mypy-boto3-builder"
+        " 7.14.6"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

