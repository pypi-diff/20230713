# Comparing `tmp/mypy-boto3-iam-1.28.0.tar.gz` & `tmp/mypy-boto3-iam-1.28.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-iam-1.28.0.tar", last modified: Thu Jul  6 20:59:43 2023, max compression
+gzip compressed data, was "mypy-boto3-iam-1.28.3.tar", last modified: Thu Jul 13 19:49:12 2023, max compression
```

## Comparing `mypy-boto3-iam-1.28.0.tar` & `mypy-boto3-iam-1.28.3.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:43.474321 mypy-boto3-iam-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:42:40.000000 mypy-boto3-iam-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    41928 2023-07-06 20:59:43.474321 mypy-boto3-iam-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    40459 2023-07-06 20:42:40.000000 mypy-boto3-iam-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:43.474321 mypy-boto3-iam-1.28.0/mypy_boto3_iam/
--rw-r--r--   0 runner    (1001) docker     (123)     8785 2023-07-06 20:42:40.000000 mypy-boto3-iam-1.28.0/mypy_boto3_iam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8783 2023-07-06 20:42:40.000000 mypy-boto3-iam-1.28.0/mypy_boto3_iam/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-06 20:42:40.000000 mypy-boto3-iam-1.28.0/mypy_boto3_iam/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)   113198 2023-07-06 20:42:43.000000 mypy-boto3-iam-1.28.0/mypy_boto3_iam/client.py
--rw-r--r--   0 runner    (1001) docker     (123)   112994 2023-07-06 20:42:41.000000 mypy-boto3-iam-1.28.0/mypy_boto3_iam/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    15542 2023-07-06 20:42:45.000000 mypy-boto3-iam-1.28.0/mypy_boto3_iam/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    15540 2023-07-06 20:42:45.000000 mypy-boto3-iam-1.28.0/mypy_boto3_iam/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    38502 2023-07-06 20:42:44.000000 mypy-boto3-iam-1.28.0/mypy_boto3_iam/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    38466 2023-07-06 20:42:44.000000 mypy-boto3-iam-1.28.0/mypy_boto3_iam/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:42:40.000000 mypy-boto3-iam-1.28.0/mypy_boto3_iam/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   141689 2023-07-06 20:42:44.000000 mypy-boto3-iam-1.28.0/mypy_boto3_iam/service_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)   141336 2023-07-06 20:42:43.000000 mypy-boto3-iam-1.28.0/mypy_boto3_iam/service_resource.pyi
--rw-r--r--   0 runner    (1001) docker     (123)   146128 2023-07-06 20:42:50.000000 mypy-boto3-iam-1.28.0/mypy_boto3_iam/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   145913 2023-07-06 20:42:48.000000 mypy-boto3-iam-1.28.0/mypy_boto3_iam/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:42:40.000000 mypy-boto3-iam-1.28.0/mypy_boto3_iam/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-07-06 20:42:44.000000 mypy-boto3-iam-1.28.0/mypy_boto3_iam/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3908 2023-07-06 20:42:44.000000 mypy-boto3-iam-1.28.0/mypy_boto3_iam/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:43.474321 mypy-boto3-iam-1.28.0/mypy_boto3_iam.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    41928 2023-07-06 20:59:43.000000 mypy-boto3-iam-1.28.0/mypy_boto3_iam.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-07-06 20:59:43.000000 mypy-boto3-iam-1.28.0/mypy_boto3_iam.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:43.000000 mypy-boto3-iam-1.28.0/mypy_boto3_iam.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:43.000000 mypy-boto3-iam-1.28.0/mypy_boto3_iam.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 20:59:43.000000 mypy-boto3-iam-1.28.0/mypy_boto3_iam.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-06 20:59:43.000000 mypy-boto3-iam-1.28.0/mypy_boto3_iam.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 20:59:43.474321 mypy-boto3-iam-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-07-06 20:42:40.000000 mypy-boto3-iam-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:49:12.685228 mypy-boto3-iam-1.28.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-13 19:48:10.000000 mypy-boto3-iam-1.28.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    41928 2023-07-13 19:49:12.677227 mypy-boto3-iam-1.28.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    40459 2023-07-13 19:48:10.000000 mypy-boto3-iam-1.28.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:49:12.677227 mypy-boto3-iam-1.28.3/mypy_boto3_iam/
+-rw-r--r--   0 runner    (1001) docker     (123)     8785 2023-07-13 19:48:10.000000 mypy-boto3-iam-1.28.3/mypy_boto3_iam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8783 2023-07-13 19:48:10.000000 mypy-boto3-iam-1.28.3/mypy_boto3_iam/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-13 19:48:10.000000 mypy-boto3-iam-1.28.3/mypy_boto3_iam/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   113198 2023-07-13 19:48:11.000000 mypy-boto3-iam-1.28.3/mypy_boto3_iam/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)   112994 2023-07-13 19:48:10.000000 mypy-boto3-iam-1.28.3/mypy_boto3_iam/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    15542 2023-07-13 19:48:13.000000 mypy-boto3-iam-1.28.3/mypy_boto3_iam/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15540 2023-07-13 19:48:13.000000 mypy-boto3-iam-1.28.3/mypy_boto3_iam/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    38502 2023-07-13 19:48:12.000000 mypy-boto3-iam-1.28.3/mypy_boto3_iam/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38466 2023-07-13 19:48:12.000000 mypy-boto3-iam-1.28.3/mypy_boto3_iam/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 19:48:10.000000 mypy-boto3-iam-1.28.3/mypy_boto3_iam/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   141689 2023-07-13 19:48:12.000000 mypy-boto3-iam-1.28.3/mypy_boto3_iam/service_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)   141336 2023-07-13 19:48:11.000000 mypy-boto3-iam-1.28.3/mypy_boto3_iam/service_resource.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)   141573 2023-07-13 19:48:16.000000 mypy-boto3-iam-1.28.3/mypy_boto3_iam/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   141392 2023-07-13 19:48:15.000000 mypy-boto3-iam-1.28.3/mypy_boto3_iam/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-13 19:48:10.000000 mypy-boto3-iam-1.28.3/mypy_boto3_iam/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-07-13 19:48:12.000000 mypy-boto3-iam-1.28.3/mypy_boto3_iam/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3908 2023-07-13 19:48:12.000000 mypy-boto3-iam-1.28.3/mypy_boto3_iam/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:49:12.677227 mypy-boto3-iam-1.28.3/mypy_boto3_iam.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    41928 2023-07-13 19:49:12.000000 mypy-boto3-iam-1.28.3/mypy_boto3_iam.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-07-13 19:49:12.000000 mypy-boto3-iam-1.28.3/mypy_boto3_iam.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 19:49:12.000000 mypy-boto3-iam-1.28.3/mypy_boto3_iam.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 19:49:12.000000 mypy-boto3-iam-1.28.3/mypy_boto3_iam.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-13 19:49:12.000000 mypy-boto3-iam-1.28.3/mypy_boto3_iam.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-13 19:49:12.000000 mypy-boto3-iam-1.28.3/mypy_boto3_iam.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 19:49:12.685228 mypy-boto3-iam-1.28.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-07-13 19:48:10.000000 mypy-boto3-iam-1.28.3/setup.py
```

### Comparing `mypy-boto3-iam-1.28.0/LICENSE` & `mypy-boto3-iam-1.28.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iam-1.28.0/PKG-INFO` & `mypy-boto3-iam-1.28.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-iam
-Version: 1.28.0
-Summary: Type annotations for boto3.IAM 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.3
+Summary: Type annotations for boto3.IAM 1.28.3 service generated with mypy-boto3-builder 7.14.6
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iam.svg?color=blue)](https://pypi.org/project/mypy-boto3-iam)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-iam?color=blue)](https://pypistats.org/packages/mypy-boto3-iam)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IAM 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM)
+[boto3.IAM 1.28.3](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM)
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
 [mypy-boto3-iam docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-iam-1.28.0/README.md` & `mypy-boto3-iam-1.28.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iam.svg?color=blue)](https://pypi.org/project/mypy-boto3-iam)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-iam?color=blue)](https://pypistats.org/packages/mypy-boto3-iam)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IAM 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM)
+[boto3.IAM 1.28.3](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM)
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
 [mypy-boto3-iam docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-iam-1.28.0/mypy_boto3_iam/__init__.py` & `mypy-boto3-iam-1.28.3/mypy_boto3_iam/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iam-1.28.0/mypy_boto3_iam/__init__.pyi` & `mypy-boto3-iam-1.28.3/mypy_boto3_iam/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iam-1.28.0/mypy_boto3_iam/__main__.py` & `mypy-boto3-iam-1.28.3/mypy_boto3_iam/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.IAM 1.28.0\nVersion:         1.28.0\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.IAM 1.28.3\nVersion:         1.28.3\nBuilder version:"
+        " 7.14.6\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM\nOther"
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

### Comparing `mypy-boto3-iam-1.28.0/mypy_boto3_iam/client.py` & `mypy-boto3-iam-1.28.3/mypy_boto3_iam/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iam-1.28.0/mypy_boto3_iam/client.pyi` & `mypy-boto3-iam-1.28.3/mypy_boto3_iam/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iam-1.28.0/mypy_boto3_iam/literals.py` & `mypy-boto3-iam-1.28.3/mypy_boto3_iam/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iam-1.28.0/mypy_boto3_iam/literals.pyi` & `mypy-boto3-iam-1.28.3/mypy_boto3_iam/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iam-1.28.0/mypy_boto3_iam/paginator.py` & `mypy-boto3-iam-1.28.3/mypy_boto3_iam/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iam-1.28.0/mypy_boto3_iam/paginator.pyi` & `mypy-boto3-iam-1.28.3/mypy_boto3_iam/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iam-1.28.0/mypy_boto3_iam/service_resource.py` & `mypy-boto3-iam-1.28.3/mypy_boto3_iam/service_resource.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iam-1.28.0/mypy_boto3_iam/service_resource.pyi` & `mypy-boto3-iam-1.28.3/mypy_boto3_iam/service_resource.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iam-1.28.0/mypy_boto3_iam/type_defs.py` & `mypy-boto3-iam-1.28.3/mypy_boto3_iam/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -433,37 +433,26 @@
     "ListInstanceProfilesForRoleResponseTypeDef",
     "ListInstanceProfilesResponseTypeDef",
     "RoleDetailTypeDef",
     "SimulatePolicyResponseTypeDef",
     "GetAccountAuthorizationDetailsResponseTypeDef",
 )
 
-_RequiredAccessDetailTypeDef = TypedDict(
-    "_RequiredAccessDetailTypeDef",
+AccessDetailTypeDef = TypedDict(
+    "AccessDetailTypeDef",
     {
         "ServiceName": str,
         "ServiceNamespace": str,
-    },
-)
-_OptionalAccessDetailTypeDef = TypedDict(
-    "_OptionalAccessDetailTypeDef",
-    {
         "Region": str,
         "EntityPath": str,
         "LastAuthenticatedTime": datetime,
         "TotalAuthenticatedEntities": int,
     },
-    total=False,
 )
 
-
-class AccessDetailTypeDef(_RequiredAccessDetailTypeDef, _OptionalAccessDetailTypeDef):
-    pass
-
-
 AccessKeyLastUsedTypeDef = TypedDict(
     "AccessKeyLastUsedTypeDef",
     {
         "LastUsedDate": datetime,
         "ServiceName": str,
         "Region": str,
     },
@@ -473,39 +462,27 @@
     "AccessKeyMetadataTypeDef",
     {
         "UserName": str,
         "AccessKeyId": str,
         "Status": statusTypeType,
         "CreateDate": datetime,
     },
-    total=False,
 )
 
-_RequiredAccessKeyTypeDef = TypedDict(
-    "_RequiredAccessKeyTypeDef",
+AccessKeyTypeDef = TypedDict(
+    "AccessKeyTypeDef",
     {
         "UserName": str,
         "AccessKeyId": str,
         "Status": statusTypeType,
         "SecretAccessKey": str,
-    },
-)
-_OptionalAccessKeyTypeDef = TypedDict(
-    "_OptionalAccessKeyTypeDef",
-    {
         "CreateDate": datetime,
     },
-    total=False,
 )
 
-
-class AccessKeyTypeDef(_RequiredAccessKeyTypeDef, _OptionalAccessKeyTypeDef):
-    pass
-
-
 AddClientIDToOpenIDConnectProviderRequestRequestTypeDef = TypedDict(
     "AddClientIDToOpenIDConnectProviderRequestRequestTypeDef",
     {
         "OpenIDConnectProviderArn": str,
         "ClientID": str,
     },
 )
@@ -624,24 +601,22 @@
 
 AttachedPermissionsBoundaryTypeDef = TypedDict(
     "AttachedPermissionsBoundaryTypeDef",
     {
         "PermissionsBoundaryType": Literal["PermissionsBoundaryPolicy"],
         "PermissionsBoundaryArn": str,
     },
-    total=False,
 )
 
 AttachedPolicyTypeDef = TypedDict(
     "AttachedPolicyTypeDef",
     {
         "PolicyName": str,
         "PolicyArn": str,
     },
-    total=False,
 )
 
 ChangePasswordRequestRequestTypeDef = TypedDict(
     "ChangePasswordRequestRequestTypeDef",
     {
         "OldPassword": str,
         "NewPassword": str,
@@ -821,34 +796,23 @@
 class CreateLoginProfileRequestUserCreateLoginProfileTypeDef(
     _RequiredCreateLoginProfileRequestUserCreateLoginProfileTypeDef,
     _OptionalCreateLoginProfileRequestUserCreateLoginProfileTypeDef,
 ):
     pass
 
 
-_RequiredLoginProfileTypeDef = TypedDict(
-    "_RequiredLoginProfileTypeDef",
+LoginProfileTypeDef = TypedDict(
+    "LoginProfileTypeDef",
     {
         "UserName": str,
         "CreateDate": datetime,
-    },
-)
-_OptionalLoginProfileTypeDef = TypedDict(
-    "_OptionalLoginProfileTypeDef",
-    {
         "PasswordResetRequired": bool,
     },
-    total=False,
 )
 
-
-class LoginProfileTypeDef(_RequiredLoginProfileTypeDef, _OptionalLoginProfileTypeDef):
-    pass
-
-
 _RequiredCreatePolicyVersionRequestPolicyCreateVersionTypeDef = TypedDict(
     "_RequiredCreatePolicyVersionRequestPolicyCreateVersionTypeDef",
     {
         "PolicyDocument": str,
     },
 )
 _OptionalCreatePolicyVersionRequestPolicyCreateVersionTypeDef = TypedDict(
@@ -894,15 +858,14 @@
     "PolicyVersionTypeDef",
     {
         "Document": str,
         "VersionId": str,
         "IsDefaultVersion": bool,
         "CreateDate": datetime,
     },
-    total=False,
 )
 
 _RequiredCreateServiceLinkedRoleRequestRequestTypeDef = TypedDict(
     "_RequiredCreateServiceLinkedRoleRequestRequestTypeDef",
     {
         "AWSServiceName": str,
     },
@@ -1166,15 +1129,14 @@
 
 RoleUsageTypeTypeDef = TypedDict(
     "RoleUsageTypeTypeDef",
     {
         "Region": str,
         "Resources": List[str],
     },
-    total=False,
 )
 
 DetachGroupPolicyRequestGroupDetachPolicyTypeDef = TypedDict(
     "DetachGroupPolicyRequestGroupDetachPolicyTypeDef",
     {
         "PolicyArn": str,
     },
@@ -1269,58 +1231,45 @@
     {
         "SerialNumber": str,
         "AuthenticationCode1": str,
         "AuthenticationCode2": str,
     },
 )
 
-_RequiredEntityInfoTypeDef = TypedDict(
-    "_RequiredEntityInfoTypeDef",
+EntityInfoTypeDef = TypedDict(
+    "EntityInfoTypeDef",
     {
         "Arn": str,
         "Name": str,
         "Type": policyOwnerEntityTypeType,
         "Id": str,
-    },
-)
-_OptionalEntityInfoTypeDef = TypedDict(
-    "_OptionalEntityInfoTypeDef",
-    {
         "Path": str,
     },
-    total=False,
 )
 
-
-class EntityInfoTypeDef(_RequiredEntityInfoTypeDef, _OptionalEntityInfoTypeDef):
-    pass
-
-
 ErrorDetailsTypeDef = TypedDict(
     "ErrorDetailsTypeDef",
     {
         "Message": str,
         "Code": str,
     },
 )
 
 OrganizationsDecisionDetailTypeDef = TypedDict(
     "OrganizationsDecisionDetailTypeDef",
     {
         "AllowedByOrganizations": bool,
     },
-    total=False,
 )
 
 PermissionsBoundaryDecisionDetailTypeDef = TypedDict(
     "PermissionsBoundaryDecisionDetailTypeDef",
     {
         "AllowedByPermissionsBoundary": bool,
     },
-    total=False,
 )
 
 GenerateCredentialReportResponseTypeDef = TypedDict(
     "GenerateCredentialReportResponseTypeDef",
     {
         "State": ReportStateTypeType,
         "Description": str,
@@ -1424,15 +1373,14 @@
         "RequireLowercaseCharacters": bool,
         "AllowUsersToChangePassword": bool,
         "ExpirePasswords": bool,
         "MaxPasswordAge": int,
         "PasswordReusePrevention": int,
         "HardExpiry": bool,
     },
-    total=False,
 )
 
 GetAccountSummaryResponseTypeDef = TypedDict(
     "GetAccountSummaryResponseTypeDef",
     {
         "SummaryMap": Dict[summaryKeyTypeType, int],
         "ResponseMetadata": "ResponseMetadataTypeDef",
@@ -1685,37 +1633,26 @@
     {
         "UserName": str,
         "SSHPublicKeyId": str,
         "Encoding": encodingTypeType,
     },
 )
 
-_RequiredSSHPublicKeyTypeDef = TypedDict(
-    "_RequiredSSHPublicKeyTypeDef",
+SSHPublicKeyTypeDef = TypedDict(
+    "SSHPublicKeyTypeDef",
     {
         "UserName": str,
         "SSHPublicKeyId": str,
         "Fingerprint": str,
         "SSHPublicKeyBody": str,
         "Status": statusTypeType,
-    },
-)
-_OptionalSSHPublicKeyTypeDef = TypedDict(
-    "_OptionalSSHPublicKeyTypeDef",
-    {
         "UploadDate": datetime,
     },
-    total=False,
 )
 
-
-class SSHPublicKeyTypeDef(_RequiredSSHPublicKeyTypeDef, _OptionalSSHPublicKeyTypeDef):
-    pass
-
-
 GetServerCertificateRequestRequestTypeDef = TypedDict(
     "GetServerCertificateRequestRequestTypeDef",
     {
         "ServerCertificateName": str,
     },
 )
 
@@ -1801,15 +1738,14 @@
 
 PolicyDetailTypeDef = TypedDict(
     "PolicyDetailTypeDef",
     {
         "PolicyName": str,
         "PolicyDocument": str,
     },
-    total=False,
 )
 
 ListAccessKeysRequestListAccessKeysPaginateTypeDef = TypedDict(
     "ListAccessKeysRequestListAccessKeysPaginateTypeDef",
     {
         "UserName": str,
         "PaginationConfig": "PaginatorConfigTypeDef",
@@ -2048,33 +1984,30 @@
 
 PolicyGroupTypeDef = TypedDict(
     "PolicyGroupTypeDef",
     {
         "GroupName": str,
         "GroupId": str,
     },
-    total=False,
 )
 
 PolicyRoleTypeDef = TypedDict(
     "PolicyRoleTypeDef",
     {
         "RoleName": str,
         "RoleId": str,
     },
-    total=False,
 )
 
 PolicyUserTypeDef = TypedDict(
     "PolicyUserTypeDef",
     {
         "UserName": str,
         "UserId": str,
     },
-    total=False,
 )
 
 _RequiredListGroupPoliciesRequestListGroupPoliciesPaginateTypeDef = TypedDict(
     "_RequiredListGroupPoliciesRequestListGroupPoliciesPaginateTypeDef",
     {
         "GroupName": str,
     },
@@ -2421,41 +2354,27 @@
 
 
 OpenIDConnectProviderListEntryTypeDef = TypedDict(
     "OpenIDConnectProviderListEntryTypeDef",
     {
         "Arn": str,
     },
-    total=False,
 )
 
-_RequiredPolicyGrantingServiceAccessTypeDef = TypedDict(
-    "_RequiredPolicyGrantingServiceAccessTypeDef",
+PolicyGrantingServiceAccessTypeDef = TypedDict(
+    "PolicyGrantingServiceAccessTypeDef",
     {
         "PolicyName": str,
         "PolicyType": policyTypeType,
-    },
-)
-_OptionalPolicyGrantingServiceAccessTypeDef = TypedDict(
-    "_OptionalPolicyGrantingServiceAccessTypeDef",
-    {
         "PolicyArn": str,
         "EntityType": policyOwnerEntityTypeType,
         "EntityName": str,
     },
-    total=False,
 )
 
-
-class PolicyGrantingServiceAccessTypeDef(
-    _RequiredPolicyGrantingServiceAccessTypeDef, _OptionalPolicyGrantingServiceAccessTypeDef
-):
-    pass
-
-
 _RequiredListPoliciesGrantingServiceAccessRequestRequestTypeDef = TypedDict(
     "_RequiredListPoliciesGrantingServiceAccessRequestRequestTypeDef",
     {
         "Arn": str,
         "ServiceNamespaces": Sequence[str],
     },
 )
@@ -2754,15 +2673,14 @@
 SAMLProviderListEntryTypeDef = TypedDict(
     "SAMLProviderListEntryTypeDef",
     {
         "Arn": str,
         "ValidUntil": datetime,
         "CreateDate": datetime,
     },
-    total=False,
 )
 
 ListSSHPublicKeysRequestListSSHPublicKeysPaginateTypeDef = TypedDict(
     "ListSSHPublicKeysRequestListSSHPublicKeysPaginateTypeDef",
     {
         "UserName": str,
         "PaginationConfig": "PaginatorConfigTypeDef",
@@ -2850,39 +2768,26 @@
         "PathPrefix": str,
         "Marker": str,
         "MaxItems": int,
     },
     total=False,
 )
 
-_RequiredServerCertificateMetadataTypeDef = TypedDict(
-    "_RequiredServerCertificateMetadataTypeDef",
+ServerCertificateMetadataTypeDef = TypedDict(
+    "ServerCertificateMetadataTypeDef",
     {
         "Path": str,
         "ServerCertificateName": str,
         "ServerCertificateId": str,
         "Arn": str,
-    },
-)
-_OptionalServerCertificateMetadataTypeDef = TypedDict(
-    "_OptionalServerCertificateMetadataTypeDef",
-    {
         "UploadDate": datetime,
         "Expiration": datetime,
     },
-    total=False,
 )
 
-
-class ServerCertificateMetadataTypeDef(
-    _RequiredServerCertificateMetadataTypeDef, _OptionalServerCertificateMetadataTypeDef
-):
-    pass
-
-
 ListServiceSpecificCredentialsRequestRequestTypeDef = TypedDict(
     "ListServiceSpecificCredentialsRequestRequestTypeDef",
     {
         "UserName": str,
         "ServiceName": str,
     },
     total=False,
@@ -2915,38 +2820,25 @@
         "UserName": str,
         "Marker": str,
         "MaxItems": int,
     },
     total=False,
 )
 
-_RequiredSigningCertificateTypeDef = TypedDict(
-    "_RequiredSigningCertificateTypeDef",
+SigningCertificateTypeDef = TypedDict(
+    "SigningCertificateTypeDef",
     {
         "UserName": str,
         "CertificateId": str,
         "CertificateBody": str,
         "Status": statusTypeType,
-    },
-)
-_OptionalSigningCertificateTypeDef = TypedDict(
-    "_OptionalSigningCertificateTypeDef",
-    {
         "UploadDate": datetime,
     },
-    total=False,
 )
 
-
-class SigningCertificateTypeDef(
-    _RequiredSigningCertificateTypeDef, _OptionalSigningCertificateTypeDef
-):
-    pass
-
-
 _RequiredListUserPoliciesRequestListUserPoliciesPaginateTypeDef = TypedDict(
     "_RequiredListUserPoliciesRequestListUserPoliciesPaginateTypeDef",
     {
         "UserName": str,
     },
 )
 _OptionalListUserPoliciesRequestListUserPoliciesPaginateTypeDef = TypedDict(
@@ -3091,15 +2983,14 @@
 
 PositionTypeDef = TypedDict(
     "PositionTypeDef",
     {
         "Line": int,
         "Column": int,
     },
-    total=False,
 )
 
 PutGroupPolicyRequestGroupCreatePolicyTypeDef = TypedDict(
     "PutGroupPolicyRequestGroupCreatePolicyTypeDef",
     {
         "PolicyName": str,
         "PolicyDocument": str,
@@ -3276,15 +3167,14 @@
 
 RoleLastUsedTypeDef = TypedDict(
     "RoleLastUsedTypeDef",
     {
         "LastUsedDate": datetime,
         "Region": str,
     },
-    total=False,
 )
 
 RoleLastUsedResponseMetadataTypeDef = TypedDict(
     "RoleLastUsedResponseMetadataTypeDef",
     {
         "LastUsedDate": datetime,
         "Region": str,
@@ -3309,15 +3199,14 @@
     "TrackedActionLastAccessedTypeDef",
     {
         "ActionName": str,
         "LastAccessedEntity": str,
         "LastAccessedTime": datetime,
         "LastAccessedRegion": str,
     },
-    total=False,
 )
 
 SetDefaultPolicyVersionRequestRequestTypeDef = TypedDict(
     "SetDefaultPolicyVersionRequestRequestTypeDef",
     {
         "PolicyArn": str,
         "VersionId": str,
@@ -4485,15 +4374,14 @@
         "PermissionsBoundaryUsageCount": int,
         "IsAttachable": bool,
         "Description": str,
         "CreateDate": datetime,
         "UpdateDate": datetime,
         "Tags": List[TagTypeDef],
     },
-    total=False,
 )
 
 TagInstanceProfileRequestRequestTypeDef = TypedDict(
     "TagInstanceProfileRequestRequestTypeDef",
     {
         "InstanceProfileName": str,
         "Tags": Sequence[TagTypeDef],
@@ -4619,39 +4507,28 @@
         "PasswordLastUsed": datetime,
         "PermissionsBoundary": AttachedPermissionsBoundaryTypeDef,
         "Tags": List[TagTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredUserTypeDef = TypedDict(
-    "_RequiredUserTypeDef",
+UserTypeDef = TypedDict(
+    "UserTypeDef",
     {
         "Path": str,
         "UserName": str,
         "UserId": str,
         "Arn": str,
         "CreateDate": datetime,
-    },
-)
-_OptionalUserTypeDef = TypedDict(
-    "_OptionalUserTypeDef",
-    {
         "PasswordLastUsed": datetime,
         "PermissionsBoundary": AttachedPermissionsBoundaryTypeDef,
         "Tags": List[TagTypeDef],
     },
-    total=False,
 )
 
-
-class UserTypeDef(_RequiredUserTypeDef, _OptionalUserTypeDef):
-    pass
-
-
 CreateLoginProfileResponseTypeDef = TypedDict(
     "CreateLoginProfileResponseTypeDef",
     {
         "LoginProfile": LoginProfileTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -4702,15 +4579,14 @@
         "PermissionsBoundaryUsageCount": int,
         "IsAttachable": bool,
         "Description": str,
         "CreateDate": datetime,
         "UpdateDate": datetime,
         "PolicyVersionList": List[PolicyVersionTypeDef],
     },
-    total=False,
 )
 
 CreateServiceSpecificCredentialResponseTypeDef = TypedDict(
     "CreateServiceSpecificCredentialResponseTypeDef",
     {
         "ServiceSpecificCredential": ServiceSpecificCredentialTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
@@ -4727,36 +4603,24 @@
 
 DeletionTaskFailureReasonTypeTypeDef = TypedDict(
     "DeletionTaskFailureReasonTypeTypeDef",
     {
         "Reason": str,
         "RoleUsageList": List[RoleUsageTypeTypeDef],
     },
-    total=False,
 )
 
-_RequiredEntityDetailsTypeDef = TypedDict(
-    "_RequiredEntityDetailsTypeDef",
+EntityDetailsTypeDef = TypedDict(
+    "EntityDetailsTypeDef",
     {
         "EntityInfo": EntityInfoTypeDef,
-    },
-)
-_OptionalEntityDetailsTypeDef = TypedDict(
-    "_OptionalEntityDetailsTypeDef",
-    {
         "LastAuthenticated": datetime,
     },
-    total=False,
 )
 
-
-class EntityDetailsTypeDef(_RequiredEntityDetailsTypeDef, _OptionalEntityDetailsTypeDef):
-    pass
-
-
 GetOrganizationsAccessReportResponseTypeDef = TypedDict(
     "GetOrganizationsAccessReportResponseTypeDef",
     {
         "JobStatus": jobStatusTypeType,
         "JobCreationDate": datetime,
         "JobCompletionDate": datetime,
         "NumberOfServicesAccessible": int,
@@ -4874,15 +4738,14 @@
         "GroupName": str,
         "GroupId": str,
         "Arn": str,
         "CreateDate": datetime,
         "GroupPolicyList": List[PolicyDetailTypeDef],
         "AttachedManagedPolicies": List[AttachedPolicyTypeDef],
     },
-    total=False,
 )
 
 UserDetailTypeDef = TypedDict(
     "UserDetailTypeDef",
     {
         "Path": str,
         "UserName": str,
@@ -4891,15 +4754,14 @@
         "CreateDate": datetime,
         "UserPolicyList": List[PolicyDetailTypeDef],
         "GroupList": List[str],
         "AttachedManagedPolicies": List[AttachedPolicyTypeDef],
         "PermissionsBoundary": AttachedPermissionsBoundaryTypeDef,
         "Tags": List[TagTypeDef],
     },
-    total=False,
 )
 
 ListEntitiesForPolicyResponseTypeDef = TypedDict(
     "ListEntitiesForPolicyResponseTypeDef",
     {
         "PolicyGroups": List[PolicyGroupTypeDef],
         "PolicyUsers": List[PolicyUserTypeDef],
@@ -4930,15 +4792,14 @@
 
 ListPoliciesGrantingServiceAccessEntryTypeDef = TypedDict(
     "ListPoliciesGrantingServiceAccessEntryTypeDef",
     {
         "ServiceNamespace": str,
         "Policies": List[PolicyGrantingServiceAccessTypeDef],
     },
-    total=False,
 )
 
 ListSAMLProvidersResponseTypeDef = TypedDict(
     "ListSAMLProvidersResponseTypeDef",
     {
         "SAMLProviderList": List[SAMLProviderListEntryTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
@@ -4961,37 +4822,24 @@
         "ServerCertificateMetadataList": List[ServerCertificateMetadataTypeDef],
         "IsTruncated": bool,
         "Marker": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredServerCertificateTypeDef = TypedDict(
-    "_RequiredServerCertificateTypeDef",
+ServerCertificateTypeDef = TypedDict(
+    "ServerCertificateTypeDef",
     {
         "ServerCertificateMetadata": ServerCertificateMetadataTypeDef,
         "CertificateBody": str,
-    },
-)
-_OptionalServerCertificateTypeDef = TypedDict(
-    "_OptionalServerCertificateTypeDef",
-    {
         "CertificateChain": str,
         "Tags": List[TagTypeDef],
     },
-    total=False,
 )
 
-
-class ServerCertificateTypeDef(
-    _RequiredServerCertificateTypeDef, _OptionalServerCertificateTypeDef
-):
-    pass
-
-
 UploadServerCertificateResponseTypeDef = TypedDict(
     "UploadServerCertificateResponseTypeDef",
     {
         "ServerCertificateMetadata": ServerCertificateMetadataTypeDef,
         "Tags": List[TagTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -5027,71 +4875,46 @@
     "StatementTypeDef",
     {
         "SourcePolicyId": str,
         "SourcePolicyType": PolicySourceTypeType,
         "StartPosition": PositionTypeDef,
         "EndPosition": PositionTypeDef,
     },
-    total=False,
 )
 
-_RequiredRoleTypeDef = TypedDict(
-    "_RequiredRoleTypeDef",
+RoleTypeDef = TypedDict(
+    "RoleTypeDef",
     {
         "Path": str,
         "RoleName": str,
         "RoleId": str,
         "Arn": str,
         "CreateDate": datetime,
-    },
-)
-_OptionalRoleTypeDef = TypedDict(
-    "_OptionalRoleTypeDef",
-    {
         "AssumeRolePolicyDocument": str,
         "Description": str,
         "MaxSessionDuration": int,
         "PermissionsBoundary": AttachedPermissionsBoundaryTypeDef,
         "Tags": List[TagTypeDef],
         "RoleLastUsed": RoleLastUsedTypeDef,
     },
-    total=False,
 )
 
-
-class RoleTypeDef(_RequiredRoleTypeDef, _OptionalRoleTypeDef):
-    pass
-
-
-_RequiredServiceLastAccessedTypeDef = TypedDict(
-    "_RequiredServiceLastAccessedTypeDef",
+ServiceLastAccessedTypeDef = TypedDict(
+    "ServiceLastAccessedTypeDef",
     {
         "ServiceName": str,
-        "ServiceNamespace": str,
-    },
-)
-_OptionalServiceLastAccessedTypeDef = TypedDict(
-    "_OptionalServiceLastAccessedTypeDef",
-    {
         "LastAuthenticated": datetime,
+        "ServiceNamespace": str,
         "LastAuthenticatedEntity": str,
         "LastAuthenticatedRegion": str,
         "TotalAuthenticatedEntities": int,
         "TrackedActionsLastAccessed": List[TrackedActionLastAccessedTypeDef],
     },
-    total=False,
 )
 
-
-class ServiceLastAccessedTypeDef(
-    _RequiredServiceLastAccessedTypeDef, _OptionalServiceLastAccessedTypeDef
-):
-    pass
-
-
 CreatePolicyResponseTypeDef = TypedDict(
     "CreatePolicyResponseTypeDef",
     {
         "Policy": PolicyTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -5147,37 +4970,26 @@
         "Users": List[UserTypeDef],
         "IsTruncated": bool,
         "Marker": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredVirtualMFADeviceTypeDef = TypedDict(
-    "_RequiredVirtualMFADeviceTypeDef",
+VirtualMFADeviceTypeDef = TypedDict(
+    "VirtualMFADeviceTypeDef",
     {
         "SerialNumber": str,
-    },
-)
-_OptionalVirtualMFADeviceTypeDef = TypedDict(
-    "_OptionalVirtualMFADeviceTypeDef",
-    {
         "Base32StringSeed": bytes,
         "QRCodePNG": bytes,
         "User": UserTypeDef,
         "EnableDate": datetime,
         "Tags": List[TagTypeDef],
     },
-    total=False,
 )
 
-
-class VirtualMFADeviceTypeDef(_RequiredVirtualMFADeviceTypeDef, _OptionalVirtualMFADeviceTypeDef):
-    pass
-
-
 GetServiceLinkedRoleDeletionStatusResponseTypeDef = TypedDict(
     "GetServiceLinkedRoleDeletionStatusResponseTypeDef",
     {
         "Status": DeletionTaskStatusTypeType,
         "Reason": DeletionTaskFailureReasonTypeTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -5211,39 +5023,26 @@
     "GetServerCertificateResponseTypeDef",
     {
         "ServerCertificate": ServerCertificateTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredResourceSpecificResultTypeDef = TypedDict(
-    "_RequiredResourceSpecificResultTypeDef",
+ResourceSpecificResultTypeDef = TypedDict(
+    "ResourceSpecificResultTypeDef",
     {
         "EvalResourceName": str,
         "EvalResourceDecision": PolicyEvaluationDecisionTypeType,
-    },
-)
-_OptionalResourceSpecificResultTypeDef = TypedDict(
-    "_OptionalResourceSpecificResultTypeDef",
-    {
         "MatchedStatements": List[StatementTypeDef],
         "MissingContextValues": List[str],
         "EvalDecisionDetails": Dict[str, PolicyEvaluationDecisionTypeType],
         "PermissionsBoundaryDecisionDetail": PermissionsBoundaryDecisionDetailTypeDef,
     },
-    total=False,
 )
 
-
-class ResourceSpecificResultTypeDef(
-    _RequiredResourceSpecificResultTypeDef, _OptionalResourceSpecificResultTypeDef
-):
-    pass
-
-
 CreateRoleResponseTypeDef = TypedDict(
     "CreateRoleResponseTypeDef",
     {
         "Role": RoleTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -5260,38 +5059,27 @@
     "GetRoleResponseTypeDef",
     {
         "Role": RoleTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredInstanceProfileTypeDef = TypedDict(
-    "_RequiredInstanceProfileTypeDef",
+InstanceProfileTypeDef = TypedDict(
+    "InstanceProfileTypeDef",
     {
         "Path": str,
         "InstanceProfileName": str,
         "InstanceProfileId": str,
         "Arn": str,
         "CreateDate": datetime,
         "Roles": List[RoleTypeDef],
-    },
-)
-_OptionalInstanceProfileTypeDef = TypedDict(
-    "_OptionalInstanceProfileTypeDef",
-    {
         "Tags": List[TagTypeDef],
     },
-    total=False,
 )
 
-
-class InstanceProfileTypeDef(_RequiredInstanceProfileTypeDef, _OptionalInstanceProfileTypeDef):
-    pass
-
-
 ListRolesResponseTypeDef = TypedDict(
     "ListRolesResponseTypeDef",
     {
         "Roles": List[RoleTypeDef],
         "IsTruncated": bool,
         "Marker": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
@@ -5335,40 +5123,29 @@
         "VirtualMFADevices": List[VirtualMFADeviceTypeDef],
         "IsTruncated": bool,
         "Marker": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredEvaluationResultTypeDef = TypedDict(
-    "_RequiredEvaluationResultTypeDef",
+EvaluationResultTypeDef = TypedDict(
+    "EvaluationResultTypeDef",
     {
         "EvalActionName": str,
-        "EvalDecision": PolicyEvaluationDecisionTypeType,
-    },
-)
-_OptionalEvaluationResultTypeDef = TypedDict(
-    "_OptionalEvaluationResultTypeDef",
-    {
         "EvalResourceName": str,
+        "EvalDecision": PolicyEvaluationDecisionTypeType,
         "MatchedStatements": List[StatementTypeDef],
         "MissingContextValues": List[str],
         "OrganizationsDecisionDetail": OrganizationsDecisionDetailTypeDef,
         "PermissionsBoundaryDecisionDetail": PermissionsBoundaryDecisionDetailTypeDef,
         "EvalDecisionDetails": Dict[str, PolicyEvaluationDecisionTypeType],
         "ResourceSpecificResults": List[ResourceSpecificResultTypeDef],
     },
-    total=False,
 )
 
-
-class EvaluationResultTypeDef(_RequiredEvaluationResultTypeDef, _OptionalEvaluationResultTypeDef):
-    pass
-
-
 CreateInstanceProfileResponseTypeDef = TypedDict(
     "CreateInstanceProfileResponseTypeDef",
     {
         "InstanceProfile": InstanceProfileTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -5413,15 +5190,14 @@
         "InstanceProfileList": List[InstanceProfileTypeDef],
         "RolePolicyList": List[PolicyDetailTypeDef],
         "AttachedManagedPolicies": List[AttachedPolicyTypeDef],
         "PermissionsBoundary": AttachedPermissionsBoundaryTypeDef,
         "Tags": List[TagTypeDef],
         "RoleLastUsed": RoleLastUsedTypeDef,
     },
-    total=False,
 )
 
 SimulatePolicyResponseTypeDef = TypedDict(
     "SimulatePolicyResponseTypeDef",
     {
         "EvaluationResults": List[EvaluationResultTypeDef],
         "IsTruncated": bool,
```

### Comparing `mypy-boto3-iam-1.28.0/mypy_boto3_iam/type_defs.pyi` & `mypy-boto3-iam-1.28.3/mypy_boto3_iam/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -432,35 +432,26 @@
     "ListInstanceProfilesForRoleResponseTypeDef",
     "ListInstanceProfilesResponseTypeDef",
     "RoleDetailTypeDef",
     "SimulatePolicyResponseTypeDef",
     "GetAccountAuthorizationDetailsResponseTypeDef",
 )
 
-_RequiredAccessDetailTypeDef = TypedDict(
-    "_RequiredAccessDetailTypeDef",
+AccessDetailTypeDef = TypedDict(
+    "AccessDetailTypeDef",
     {
         "ServiceName": str,
         "ServiceNamespace": str,
-    },
-)
-_OptionalAccessDetailTypeDef = TypedDict(
-    "_OptionalAccessDetailTypeDef",
-    {
         "Region": str,
         "EntityPath": str,
         "LastAuthenticatedTime": datetime,
         "TotalAuthenticatedEntities": int,
     },
-    total=False,
 )
 
-class AccessDetailTypeDef(_RequiredAccessDetailTypeDef, _OptionalAccessDetailTypeDef):
-    pass
-
 AccessKeyLastUsedTypeDef = TypedDict(
     "AccessKeyLastUsedTypeDef",
     {
         "LastUsedDate": datetime,
         "ServiceName": str,
         "Region": str,
     },
@@ -470,37 +461,27 @@
     "AccessKeyMetadataTypeDef",
     {
         "UserName": str,
         "AccessKeyId": str,
         "Status": statusTypeType,
         "CreateDate": datetime,
     },
-    total=False,
 )
 
-_RequiredAccessKeyTypeDef = TypedDict(
-    "_RequiredAccessKeyTypeDef",
+AccessKeyTypeDef = TypedDict(
+    "AccessKeyTypeDef",
     {
         "UserName": str,
         "AccessKeyId": str,
         "Status": statusTypeType,
         "SecretAccessKey": str,
-    },
-)
-_OptionalAccessKeyTypeDef = TypedDict(
-    "_OptionalAccessKeyTypeDef",
-    {
         "CreateDate": datetime,
     },
-    total=False,
 )
 
-class AccessKeyTypeDef(_RequiredAccessKeyTypeDef, _OptionalAccessKeyTypeDef):
-    pass
-
 AddClientIDToOpenIDConnectProviderRequestRequestTypeDef = TypedDict(
     "AddClientIDToOpenIDConnectProviderRequestRequestTypeDef",
     {
         "OpenIDConnectProviderArn": str,
         "ClientID": str,
     },
 )
@@ -619,24 +600,22 @@
 
 AttachedPermissionsBoundaryTypeDef = TypedDict(
     "AttachedPermissionsBoundaryTypeDef",
     {
         "PermissionsBoundaryType": Literal["PermissionsBoundaryPolicy"],
         "PermissionsBoundaryArn": str,
     },
-    total=False,
 )
 
 AttachedPolicyTypeDef = TypedDict(
     "AttachedPolicyTypeDef",
     {
         "PolicyName": str,
         "PolicyArn": str,
     },
-    total=False,
 )
 
 ChangePasswordRequestRequestTypeDef = TypedDict(
     "ChangePasswordRequestRequestTypeDef",
     {
         "OldPassword": str,
         "NewPassword": str,
@@ -806,32 +785,23 @@
 
 class CreateLoginProfileRequestUserCreateLoginProfileTypeDef(
     _RequiredCreateLoginProfileRequestUserCreateLoginProfileTypeDef,
     _OptionalCreateLoginProfileRequestUserCreateLoginProfileTypeDef,
 ):
     pass
 
-_RequiredLoginProfileTypeDef = TypedDict(
-    "_RequiredLoginProfileTypeDef",
+LoginProfileTypeDef = TypedDict(
+    "LoginProfileTypeDef",
     {
         "UserName": str,
         "CreateDate": datetime,
-    },
-)
-_OptionalLoginProfileTypeDef = TypedDict(
-    "_OptionalLoginProfileTypeDef",
-    {
         "PasswordResetRequired": bool,
     },
-    total=False,
 )
 
-class LoginProfileTypeDef(_RequiredLoginProfileTypeDef, _OptionalLoginProfileTypeDef):
-    pass
-
 _RequiredCreatePolicyVersionRequestPolicyCreateVersionTypeDef = TypedDict(
     "_RequiredCreatePolicyVersionRequestPolicyCreateVersionTypeDef",
     {
         "PolicyDocument": str,
     },
 )
 _OptionalCreatePolicyVersionRequestPolicyCreateVersionTypeDef = TypedDict(
@@ -873,15 +843,14 @@
     "PolicyVersionTypeDef",
     {
         "Document": str,
         "VersionId": str,
         "IsDefaultVersion": bool,
         "CreateDate": datetime,
     },
-    total=False,
 )
 
 _RequiredCreateServiceLinkedRoleRequestRequestTypeDef = TypedDict(
     "_RequiredCreateServiceLinkedRoleRequestRequestTypeDef",
     {
         "AWSServiceName": str,
     },
@@ -1137,15 +1106,14 @@
 
 RoleUsageTypeTypeDef = TypedDict(
     "RoleUsageTypeTypeDef",
     {
         "Region": str,
         "Resources": List[str],
     },
-    total=False,
 )
 
 DetachGroupPolicyRequestGroupDetachPolicyTypeDef = TypedDict(
     "DetachGroupPolicyRequestGroupDetachPolicyTypeDef",
     {
         "PolicyArn": str,
     },
@@ -1240,56 +1208,45 @@
     {
         "SerialNumber": str,
         "AuthenticationCode1": str,
         "AuthenticationCode2": str,
     },
 )
 
-_RequiredEntityInfoTypeDef = TypedDict(
-    "_RequiredEntityInfoTypeDef",
+EntityInfoTypeDef = TypedDict(
+    "EntityInfoTypeDef",
     {
         "Arn": str,
         "Name": str,
         "Type": policyOwnerEntityTypeType,
         "Id": str,
-    },
-)
-_OptionalEntityInfoTypeDef = TypedDict(
-    "_OptionalEntityInfoTypeDef",
-    {
         "Path": str,
     },
-    total=False,
 )
 
-class EntityInfoTypeDef(_RequiredEntityInfoTypeDef, _OptionalEntityInfoTypeDef):
-    pass
-
 ErrorDetailsTypeDef = TypedDict(
     "ErrorDetailsTypeDef",
     {
         "Message": str,
         "Code": str,
     },
 )
 
 OrganizationsDecisionDetailTypeDef = TypedDict(
     "OrganizationsDecisionDetailTypeDef",
     {
         "AllowedByOrganizations": bool,
     },
-    total=False,
 )
 
 PermissionsBoundaryDecisionDetailTypeDef = TypedDict(
     "PermissionsBoundaryDecisionDetailTypeDef",
     {
         "AllowedByPermissionsBoundary": bool,
     },
-    total=False,
 )
 
 GenerateCredentialReportResponseTypeDef = TypedDict(
     "GenerateCredentialReportResponseTypeDef",
     {
         "State": ReportStateTypeType,
         "Description": str,
@@ -1389,15 +1346,14 @@
         "RequireLowercaseCharacters": bool,
         "AllowUsersToChangePassword": bool,
         "ExpirePasswords": bool,
         "MaxPasswordAge": int,
         "PasswordReusePrevention": int,
         "HardExpiry": bool,
     },
-    total=False,
 )
 
 GetAccountSummaryResponseTypeDef = TypedDict(
     "GetAccountSummaryResponseTypeDef",
     {
         "SummaryMap": Dict[summaryKeyTypeType, int],
         "ResponseMetadata": "ResponseMetadataTypeDef",
@@ -1640,35 +1596,26 @@
     {
         "UserName": str,
         "SSHPublicKeyId": str,
         "Encoding": encodingTypeType,
     },
 )
 
-_RequiredSSHPublicKeyTypeDef = TypedDict(
-    "_RequiredSSHPublicKeyTypeDef",
+SSHPublicKeyTypeDef = TypedDict(
+    "SSHPublicKeyTypeDef",
     {
         "UserName": str,
         "SSHPublicKeyId": str,
         "Fingerprint": str,
         "SSHPublicKeyBody": str,
         "Status": statusTypeType,
-    },
-)
-_OptionalSSHPublicKeyTypeDef = TypedDict(
-    "_OptionalSSHPublicKeyTypeDef",
-    {
         "UploadDate": datetime,
     },
-    total=False,
 )
 
-class SSHPublicKeyTypeDef(_RequiredSSHPublicKeyTypeDef, _OptionalSSHPublicKeyTypeDef):
-    pass
-
 GetServerCertificateRequestRequestTypeDef = TypedDict(
     "GetServerCertificateRequestRequestTypeDef",
     {
         "ServerCertificateName": str,
     },
 )
 
@@ -1750,15 +1697,14 @@
 
 PolicyDetailTypeDef = TypedDict(
     "PolicyDetailTypeDef",
     {
         "PolicyName": str,
         "PolicyDocument": str,
     },
-    total=False,
 )
 
 ListAccessKeysRequestListAccessKeysPaginateTypeDef = TypedDict(
     "ListAccessKeysRequestListAccessKeysPaginateTypeDef",
     {
         "UserName": str,
         "PaginationConfig": "PaginatorConfigTypeDef",
@@ -1981,33 +1927,30 @@
 
 PolicyGroupTypeDef = TypedDict(
     "PolicyGroupTypeDef",
     {
         "GroupName": str,
         "GroupId": str,
     },
-    total=False,
 )
 
 PolicyRoleTypeDef = TypedDict(
     "PolicyRoleTypeDef",
     {
         "RoleName": str,
         "RoleId": str,
     },
-    total=False,
 )
 
 PolicyUserTypeDef = TypedDict(
     "PolicyUserTypeDef",
     {
         "UserName": str,
         "UserId": str,
     },
-    total=False,
 )
 
 _RequiredListGroupPoliciesRequestListGroupPoliciesPaginateTypeDef = TypedDict(
     "_RequiredListGroupPoliciesRequestListGroupPoliciesPaginateTypeDef",
     {
         "GroupName": str,
     },
@@ -2330,39 +2273,27 @@
     pass
 
 OpenIDConnectProviderListEntryTypeDef = TypedDict(
     "OpenIDConnectProviderListEntryTypeDef",
     {
         "Arn": str,
     },
-    total=False,
 )
 
-_RequiredPolicyGrantingServiceAccessTypeDef = TypedDict(
-    "_RequiredPolicyGrantingServiceAccessTypeDef",
+PolicyGrantingServiceAccessTypeDef = TypedDict(
+    "PolicyGrantingServiceAccessTypeDef",
     {
         "PolicyName": str,
         "PolicyType": policyTypeType,
-    },
-)
-_OptionalPolicyGrantingServiceAccessTypeDef = TypedDict(
-    "_OptionalPolicyGrantingServiceAccessTypeDef",
-    {
         "PolicyArn": str,
         "EntityType": policyOwnerEntityTypeType,
         "EntityName": str,
     },
-    total=False,
 )
 
-class PolicyGrantingServiceAccessTypeDef(
-    _RequiredPolicyGrantingServiceAccessTypeDef, _OptionalPolicyGrantingServiceAccessTypeDef
-):
-    pass
-
 _RequiredListPoliciesGrantingServiceAccessRequestRequestTypeDef = TypedDict(
     "_RequiredListPoliciesGrantingServiceAccessRequestRequestTypeDef",
     {
         "Arn": str,
         "ServiceNamespaces": Sequence[str],
     },
 )
@@ -2639,15 +2570,14 @@
 SAMLProviderListEntryTypeDef = TypedDict(
     "SAMLProviderListEntryTypeDef",
     {
         "Arn": str,
         "ValidUntil": datetime,
         "CreateDate": datetime,
     },
-    total=False,
 )
 
 ListSSHPublicKeysRequestListSSHPublicKeysPaginateTypeDef = TypedDict(
     "ListSSHPublicKeysRequestListSSHPublicKeysPaginateTypeDef",
     {
         "UserName": str,
         "PaginationConfig": "PaginatorConfigTypeDef",
@@ -2731,37 +2661,26 @@
         "PathPrefix": str,
         "Marker": str,
         "MaxItems": int,
     },
     total=False,
 )
 
-_RequiredServerCertificateMetadataTypeDef = TypedDict(
-    "_RequiredServerCertificateMetadataTypeDef",
+ServerCertificateMetadataTypeDef = TypedDict(
+    "ServerCertificateMetadataTypeDef",
     {
         "Path": str,
         "ServerCertificateName": str,
         "ServerCertificateId": str,
         "Arn": str,
-    },
-)
-_OptionalServerCertificateMetadataTypeDef = TypedDict(
-    "_OptionalServerCertificateMetadataTypeDef",
-    {
         "UploadDate": datetime,
         "Expiration": datetime,
     },
-    total=False,
 )
 
-class ServerCertificateMetadataTypeDef(
-    _RequiredServerCertificateMetadataTypeDef, _OptionalServerCertificateMetadataTypeDef
-):
-    pass
-
 ListServiceSpecificCredentialsRequestRequestTypeDef = TypedDict(
     "ListServiceSpecificCredentialsRequestRequestTypeDef",
     {
         "UserName": str,
         "ServiceName": str,
     },
     total=False,
@@ -2794,36 +2713,25 @@
         "UserName": str,
         "Marker": str,
         "MaxItems": int,
     },
     total=False,
 )
 
-_RequiredSigningCertificateTypeDef = TypedDict(
-    "_RequiredSigningCertificateTypeDef",
+SigningCertificateTypeDef = TypedDict(
+    "SigningCertificateTypeDef",
     {
         "UserName": str,
         "CertificateId": str,
         "CertificateBody": str,
         "Status": statusTypeType,
-    },
-)
-_OptionalSigningCertificateTypeDef = TypedDict(
-    "_OptionalSigningCertificateTypeDef",
-    {
         "UploadDate": datetime,
     },
-    total=False,
 )
 
-class SigningCertificateTypeDef(
-    _RequiredSigningCertificateTypeDef, _OptionalSigningCertificateTypeDef
-):
-    pass
-
 _RequiredListUserPoliciesRequestListUserPoliciesPaginateTypeDef = TypedDict(
     "_RequiredListUserPoliciesRequestListUserPoliciesPaginateTypeDef",
     {
         "UserName": str,
     },
 )
 _OptionalListUserPoliciesRequestListUserPoliciesPaginateTypeDef = TypedDict(
@@ -2960,15 +2868,14 @@
 
 PositionTypeDef = TypedDict(
     "PositionTypeDef",
     {
         "Line": int,
         "Column": int,
     },
-    total=False,
 )
 
 PutGroupPolicyRequestGroupCreatePolicyTypeDef = TypedDict(
     "PutGroupPolicyRequestGroupCreatePolicyTypeDef",
     {
         "PolicyName": str,
         "PolicyDocument": str,
@@ -3143,15 +3050,14 @@
 
 RoleLastUsedTypeDef = TypedDict(
     "RoleLastUsedTypeDef",
     {
         "LastUsedDate": datetime,
         "Region": str,
     },
-    total=False,
 )
 
 RoleLastUsedResponseMetadataTypeDef = TypedDict(
     "RoleLastUsedResponseMetadataTypeDef",
     {
         "LastUsedDate": datetime,
         "Region": str,
@@ -3176,15 +3082,14 @@
     "TrackedActionLastAccessedTypeDef",
     {
         "ActionName": str,
         "LastAccessedEntity": str,
         "LastAccessedTime": datetime,
         "LastAccessedRegion": str,
     },
-    total=False,
 )
 
 SetDefaultPolicyVersionRequestRequestTypeDef = TypedDict(
     "SetDefaultPolicyVersionRequestRequestTypeDef",
     {
         "PolicyArn": str,
         "VersionId": str,
@@ -4298,15 +4203,14 @@
         "PermissionsBoundaryUsageCount": int,
         "IsAttachable": bool,
         "Description": str,
         "CreateDate": datetime,
         "UpdateDate": datetime,
         "Tags": List[TagTypeDef],
     },
-    total=False,
 )
 
 TagInstanceProfileRequestRequestTypeDef = TypedDict(
     "TagInstanceProfileRequestRequestTypeDef",
     {
         "InstanceProfileName": str,
         "Tags": Sequence[TagTypeDef],
@@ -4428,37 +4332,28 @@
         "PasswordLastUsed": datetime,
         "PermissionsBoundary": AttachedPermissionsBoundaryTypeDef,
         "Tags": List[TagTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredUserTypeDef = TypedDict(
-    "_RequiredUserTypeDef",
+UserTypeDef = TypedDict(
+    "UserTypeDef",
     {
         "Path": str,
         "UserName": str,
         "UserId": str,
         "Arn": str,
         "CreateDate": datetime,
-    },
-)
-_OptionalUserTypeDef = TypedDict(
-    "_OptionalUserTypeDef",
-    {
         "PasswordLastUsed": datetime,
         "PermissionsBoundary": AttachedPermissionsBoundaryTypeDef,
         "Tags": List[TagTypeDef],
     },
-    total=False,
 )
 
-class UserTypeDef(_RequiredUserTypeDef, _OptionalUserTypeDef):
-    pass
-
 CreateLoginProfileResponseTypeDef = TypedDict(
     "CreateLoginProfileResponseTypeDef",
     {
         "LoginProfile": LoginProfileTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -4509,15 +4404,14 @@
         "PermissionsBoundaryUsageCount": int,
         "IsAttachable": bool,
         "Description": str,
         "CreateDate": datetime,
         "UpdateDate": datetime,
         "PolicyVersionList": List[PolicyVersionTypeDef],
     },
-    total=False,
 )
 
 CreateServiceSpecificCredentialResponseTypeDef = TypedDict(
     "CreateServiceSpecificCredentialResponseTypeDef",
     {
         "ServiceSpecificCredential": ServiceSpecificCredentialTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
@@ -4534,34 +4428,24 @@
 
 DeletionTaskFailureReasonTypeTypeDef = TypedDict(
     "DeletionTaskFailureReasonTypeTypeDef",
     {
         "Reason": str,
         "RoleUsageList": List[RoleUsageTypeTypeDef],
     },
-    total=False,
 )
 
-_RequiredEntityDetailsTypeDef = TypedDict(
-    "_RequiredEntityDetailsTypeDef",
+EntityDetailsTypeDef = TypedDict(
+    "EntityDetailsTypeDef",
     {
         "EntityInfo": EntityInfoTypeDef,
-    },
-)
-_OptionalEntityDetailsTypeDef = TypedDict(
-    "_OptionalEntityDetailsTypeDef",
-    {
         "LastAuthenticated": datetime,
     },
-    total=False,
 )
 
-class EntityDetailsTypeDef(_RequiredEntityDetailsTypeDef, _OptionalEntityDetailsTypeDef):
-    pass
-
 GetOrganizationsAccessReportResponseTypeDef = TypedDict(
     "GetOrganizationsAccessReportResponseTypeDef",
     {
         "JobStatus": jobStatusTypeType,
         "JobCreationDate": datetime,
         "JobCompletionDate": datetime,
         "NumberOfServicesAccessible": int,
@@ -4673,15 +4557,14 @@
         "GroupName": str,
         "GroupId": str,
         "Arn": str,
         "CreateDate": datetime,
         "GroupPolicyList": List[PolicyDetailTypeDef],
         "AttachedManagedPolicies": List[AttachedPolicyTypeDef],
     },
-    total=False,
 )
 
 UserDetailTypeDef = TypedDict(
     "UserDetailTypeDef",
     {
         "Path": str,
         "UserName": str,
@@ -4690,15 +4573,14 @@
         "CreateDate": datetime,
         "UserPolicyList": List[PolicyDetailTypeDef],
         "GroupList": List[str],
         "AttachedManagedPolicies": List[AttachedPolicyTypeDef],
         "PermissionsBoundary": AttachedPermissionsBoundaryTypeDef,
         "Tags": List[TagTypeDef],
     },
-    total=False,
 )
 
 ListEntitiesForPolicyResponseTypeDef = TypedDict(
     "ListEntitiesForPolicyResponseTypeDef",
     {
         "PolicyGroups": List[PolicyGroupTypeDef],
         "PolicyUsers": List[PolicyUserTypeDef],
@@ -4729,15 +4611,14 @@
 
 ListPoliciesGrantingServiceAccessEntryTypeDef = TypedDict(
     "ListPoliciesGrantingServiceAccessEntryTypeDef",
     {
         "ServiceNamespace": str,
         "Policies": List[PolicyGrantingServiceAccessTypeDef],
     },
-    total=False,
 )
 
 ListSAMLProvidersResponseTypeDef = TypedDict(
     "ListSAMLProvidersResponseTypeDef",
     {
         "SAMLProviderList": List[SAMLProviderListEntryTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
@@ -4760,35 +4641,24 @@
         "ServerCertificateMetadataList": List[ServerCertificateMetadataTypeDef],
         "IsTruncated": bool,
         "Marker": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredServerCertificateTypeDef = TypedDict(
-    "_RequiredServerCertificateTypeDef",
+ServerCertificateTypeDef = TypedDict(
+    "ServerCertificateTypeDef",
     {
         "ServerCertificateMetadata": ServerCertificateMetadataTypeDef,
         "CertificateBody": str,
-    },
-)
-_OptionalServerCertificateTypeDef = TypedDict(
-    "_OptionalServerCertificateTypeDef",
-    {
         "CertificateChain": str,
         "Tags": List[TagTypeDef],
     },
-    total=False,
 )
 
-class ServerCertificateTypeDef(
-    _RequiredServerCertificateTypeDef, _OptionalServerCertificateTypeDef
-):
-    pass
-
 UploadServerCertificateResponseTypeDef = TypedDict(
     "UploadServerCertificateResponseTypeDef",
     {
         "ServerCertificateMetadata": ServerCertificateMetadataTypeDef,
         "Tags": List[TagTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -4824,67 +4694,46 @@
     "StatementTypeDef",
     {
         "SourcePolicyId": str,
         "SourcePolicyType": PolicySourceTypeType,
         "StartPosition": PositionTypeDef,
         "EndPosition": PositionTypeDef,
     },
-    total=False,
 )
 
-_RequiredRoleTypeDef = TypedDict(
-    "_RequiredRoleTypeDef",
+RoleTypeDef = TypedDict(
+    "RoleTypeDef",
     {
         "Path": str,
         "RoleName": str,
         "RoleId": str,
         "Arn": str,
         "CreateDate": datetime,
-    },
-)
-_OptionalRoleTypeDef = TypedDict(
-    "_OptionalRoleTypeDef",
-    {
         "AssumeRolePolicyDocument": str,
         "Description": str,
         "MaxSessionDuration": int,
         "PermissionsBoundary": AttachedPermissionsBoundaryTypeDef,
         "Tags": List[TagTypeDef],
         "RoleLastUsed": RoleLastUsedTypeDef,
     },
-    total=False,
 )
 
-class RoleTypeDef(_RequiredRoleTypeDef, _OptionalRoleTypeDef):
-    pass
-
-_RequiredServiceLastAccessedTypeDef = TypedDict(
-    "_RequiredServiceLastAccessedTypeDef",
+ServiceLastAccessedTypeDef = TypedDict(
+    "ServiceLastAccessedTypeDef",
     {
         "ServiceName": str,
-        "ServiceNamespace": str,
-    },
-)
-_OptionalServiceLastAccessedTypeDef = TypedDict(
-    "_OptionalServiceLastAccessedTypeDef",
-    {
         "LastAuthenticated": datetime,
+        "ServiceNamespace": str,
         "LastAuthenticatedEntity": str,
         "LastAuthenticatedRegion": str,
         "TotalAuthenticatedEntities": int,
         "TrackedActionsLastAccessed": List[TrackedActionLastAccessedTypeDef],
     },
-    total=False,
 )
 
-class ServiceLastAccessedTypeDef(
-    _RequiredServiceLastAccessedTypeDef, _OptionalServiceLastAccessedTypeDef
-):
-    pass
-
 CreatePolicyResponseTypeDef = TypedDict(
     "CreatePolicyResponseTypeDef",
     {
         "Policy": PolicyTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -4940,35 +4789,26 @@
         "Users": List[UserTypeDef],
         "IsTruncated": bool,
         "Marker": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredVirtualMFADeviceTypeDef = TypedDict(
-    "_RequiredVirtualMFADeviceTypeDef",
+VirtualMFADeviceTypeDef = TypedDict(
+    "VirtualMFADeviceTypeDef",
     {
         "SerialNumber": str,
-    },
-)
-_OptionalVirtualMFADeviceTypeDef = TypedDict(
-    "_OptionalVirtualMFADeviceTypeDef",
-    {
         "Base32StringSeed": bytes,
         "QRCodePNG": bytes,
         "User": UserTypeDef,
         "EnableDate": datetime,
         "Tags": List[TagTypeDef],
     },
-    total=False,
 )
 
-class VirtualMFADeviceTypeDef(_RequiredVirtualMFADeviceTypeDef, _OptionalVirtualMFADeviceTypeDef):
-    pass
-
 GetServiceLinkedRoleDeletionStatusResponseTypeDef = TypedDict(
     "GetServiceLinkedRoleDeletionStatusResponseTypeDef",
     {
         "Status": DeletionTaskStatusTypeType,
         "Reason": DeletionTaskFailureReasonTypeTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -5002,37 +4842,26 @@
     "GetServerCertificateResponseTypeDef",
     {
         "ServerCertificate": ServerCertificateTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredResourceSpecificResultTypeDef = TypedDict(
-    "_RequiredResourceSpecificResultTypeDef",
+ResourceSpecificResultTypeDef = TypedDict(
+    "ResourceSpecificResultTypeDef",
     {
         "EvalResourceName": str,
         "EvalResourceDecision": PolicyEvaluationDecisionTypeType,
-    },
-)
-_OptionalResourceSpecificResultTypeDef = TypedDict(
-    "_OptionalResourceSpecificResultTypeDef",
-    {
         "MatchedStatements": List[StatementTypeDef],
         "MissingContextValues": List[str],
         "EvalDecisionDetails": Dict[str, PolicyEvaluationDecisionTypeType],
         "PermissionsBoundaryDecisionDetail": PermissionsBoundaryDecisionDetailTypeDef,
     },
-    total=False,
 )
 
-class ResourceSpecificResultTypeDef(
-    _RequiredResourceSpecificResultTypeDef, _OptionalResourceSpecificResultTypeDef
-):
-    pass
-
 CreateRoleResponseTypeDef = TypedDict(
     "CreateRoleResponseTypeDef",
     {
         "Role": RoleTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -5049,36 +4878,27 @@
     "GetRoleResponseTypeDef",
     {
         "Role": RoleTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredInstanceProfileTypeDef = TypedDict(
-    "_RequiredInstanceProfileTypeDef",
+InstanceProfileTypeDef = TypedDict(
+    "InstanceProfileTypeDef",
     {
         "Path": str,
         "InstanceProfileName": str,
         "InstanceProfileId": str,
         "Arn": str,
         "CreateDate": datetime,
         "Roles": List[RoleTypeDef],
-    },
-)
-_OptionalInstanceProfileTypeDef = TypedDict(
-    "_OptionalInstanceProfileTypeDef",
-    {
         "Tags": List[TagTypeDef],
     },
-    total=False,
 )
 
-class InstanceProfileTypeDef(_RequiredInstanceProfileTypeDef, _OptionalInstanceProfileTypeDef):
-    pass
-
 ListRolesResponseTypeDef = TypedDict(
     "ListRolesResponseTypeDef",
     {
         "Roles": List[RoleTypeDef],
         "IsTruncated": bool,
         "Marker": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
@@ -5122,38 +4942,29 @@
         "VirtualMFADevices": List[VirtualMFADeviceTypeDef],
         "IsTruncated": bool,
         "Marker": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredEvaluationResultTypeDef = TypedDict(
-    "_RequiredEvaluationResultTypeDef",
+EvaluationResultTypeDef = TypedDict(
+    "EvaluationResultTypeDef",
     {
         "EvalActionName": str,
-        "EvalDecision": PolicyEvaluationDecisionTypeType,
-    },
-)
-_OptionalEvaluationResultTypeDef = TypedDict(
-    "_OptionalEvaluationResultTypeDef",
-    {
         "EvalResourceName": str,
+        "EvalDecision": PolicyEvaluationDecisionTypeType,
         "MatchedStatements": List[StatementTypeDef],
         "MissingContextValues": List[str],
         "OrganizationsDecisionDetail": OrganizationsDecisionDetailTypeDef,
         "PermissionsBoundaryDecisionDetail": PermissionsBoundaryDecisionDetailTypeDef,
         "EvalDecisionDetails": Dict[str, PolicyEvaluationDecisionTypeType],
         "ResourceSpecificResults": List[ResourceSpecificResultTypeDef],
     },
-    total=False,
 )
 
-class EvaluationResultTypeDef(_RequiredEvaluationResultTypeDef, _OptionalEvaluationResultTypeDef):
-    pass
-
 CreateInstanceProfileResponseTypeDef = TypedDict(
     "CreateInstanceProfileResponseTypeDef",
     {
         "InstanceProfile": InstanceProfileTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -5198,15 +5009,14 @@
         "InstanceProfileList": List[InstanceProfileTypeDef],
         "RolePolicyList": List[PolicyDetailTypeDef],
         "AttachedManagedPolicies": List[AttachedPolicyTypeDef],
         "PermissionsBoundary": AttachedPermissionsBoundaryTypeDef,
         "Tags": List[TagTypeDef],
         "RoleLastUsed": RoleLastUsedTypeDef,
     },
-    total=False,
 )
 
 SimulatePolicyResponseTypeDef = TypedDict(
     "SimulatePolicyResponseTypeDef",
     {
         "EvaluationResults": List[EvaluationResultTypeDef],
         "IsTruncated": bool,
```

### Comparing `mypy-boto3-iam-1.28.0/mypy_boto3_iam/waiter.py` & `mypy-boto3-iam-1.28.3/mypy_boto3_iam/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iam-1.28.0/mypy_boto3_iam/waiter.pyi` & `mypy-boto3-iam-1.28.3/mypy_boto3_iam/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iam-1.28.0/mypy_boto3_iam.egg-info/PKG-INFO` & `mypy-boto3-iam-1.28.3/mypy_boto3_iam.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-iam
-Version: 1.28.0
-Summary: Type annotations for boto3.IAM 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.3
+Summary: Type annotations for boto3.IAM 1.28.3 service generated with mypy-boto3-builder 7.14.6
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iam.svg?color=blue)](https://pypi.org/project/mypy-boto3-iam)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-iam?color=blue)](https://pypistats.org/packages/mypy-boto3-iam)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IAM 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM)
+[boto3.IAM 1.28.3](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM)
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
 [mypy-boto3-iam docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-iam-1.28.0/mypy_boto3_iam.egg-info/SOURCES.txt` & `mypy-boto3-iam-1.28.3/mypy_boto3_iam.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iam-1.28.0/setup.py` & `mypy-boto3-iam-1.28.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-iam",
-    version="1.28.0",
+    version="1.28.3",
     packages=["mypy_boto3_iam"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.IAM 1.28.0 service generated with mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.IAM 1.28.3 service generated with mypy-boto3-builder 7.14.6"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

