# Comparing `tmp/mypy-boto3-cognito-idp-1.28.2.tar.gz` & `tmp/mypy-boto3-cognito-idp-1.28.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-cognito-idp-1.28.2.tar", last modified: Tue Jul 11 06:09:51 2023, max compression
+gzip compressed data, was "mypy-boto3-cognito-idp-1.28.3.tar", last modified: Thu Jul 13 19:49:12 2023, max compression
```

## Comparing `mypy-boto3-cognito-idp-1.28.2.tar` & `mypy-boto3-cognito-idp-1.28.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 06:09:51.558497 mypy-boto3-cognito-idp-1.28.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-11 06:09:39.000000 mypy-boto3-cognito-idp-1.28.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    25178 2023-07-11 06:09:51.558497 mypy-boto3-cognito-idp-1.28.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    23665 2023-07-11 06:09:39.000000 mypy-boto3-cognito-idp-1.28.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 06:09:51.558497 mypy-boto3-cognito-idp-1.28.2/mypy_boto3_cognito_idp/
--rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-07-11 06:09:39.000000 mypy-boto3-cognito-idp-1.28.2/mypy_boto3_cognito_idp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-07-11 06:09:39.000000 mypy-boto3-cognito-idp-1.28.2/mypy_boto3_cognito_idp/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-07-11 06:09:39.000000 mypy-boto3-cognito-idp-1.28.2/mypy_boto3_cognito_idp/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    78755 2023-07-11 06:09:40.000000 mypy-boto3-cognito-idp-1.28.2/mypy_boto3_cognito_idp/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    78638 2023-07-11 06:09:39.000000 mypy-boto3-cognito-idp-1.28.2/mypy_boto3_cognito_idp/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13623 2023-07-11 06:09:40.000000 mypy-boto3-cognito-idp-1.28.2/mypy_boto3_cognito_idp/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    13621 2023-07-11 06:09:40.000000 mypy-boto3-cognito-idp-1.28.2/mypy_boto3_cognito_idp/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11048 2023-07-11 06:09:40.000000 mypy-boto3-cognito-idp-1.28.2/mypy_boto3_cognito_idp/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    11037 2023-07-11 06:09:40.000000 mypy-boto3-cognito-idp-1.28.2/mypy_boto3_cognito_idp/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 06:09:39.000000 mypy-boto3-cognito-idp-1.28.2/mypy_boto3_cognito_idp/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    97304 2023-07-11 06:09:42.000000 mypy-boto3-cognito-idp-1.28.2/mypy_boto3_cognito_idp/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    97165 2023-07-11 06:09:41.000000 mypy-boto3-cognito-idp-1.28.2/mypy_boto3_cognito_idp/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-11 06:09:39.000000 mypy-boto3-cognito-idp-1.28.2/mypy_boto3_cognito_idp/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 06:09:51.558497 mypy-boto3-cognito-idp-1.28.2/mypy_boto3_cognito_idp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    25178 2023-07-11 06:09:51.000000 mypy-boto3-cognito-idp-1.28.2/mypy_boto3_cognito_idp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-07-11 06:09:51.000000 mypy-boto3-cognito-idp-1.28.2/mypy_boto3_cognito_idp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 06:09:51.000000 mypy-boto3-cognito-idp-1.28.2/mypy_boto3_cognito_idp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 06:09:51.000000 mypy-boto3-cognito-idp-1.28.2/mypy_boto3_cognito_idp.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-11 06:09:51.000000 mypy-boto3-cognito-idp-1.28.2/mypy_boto3_cognito_idp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-11 06:09:51.000000 mypy-boto3-cognito-idp-1.28.2/mypy_boto3_cognito_idp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 06:09:51.558497 mypy-boto3-cognito-idp-1.28.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-07-11 06:09:39.000000 mypy-boto3-cognito-idp-1.28.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:49:12.673227 mypy-boto3-cognito-idp-1.28.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-13 19:46:55.000000 mypy-boto3-cognito-idp-1.28.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    25178 2023-07-13 19:49:12.665227 mypy-boto3-cognito-idp-1.28.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    23665 2023-07-13 19:46:55.000000 mypy-boto3-cognito-idp-1.28.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:49:12.657227 mypy-boto3-cognito-idp-1.28.3/mypy_boto3_cognito_idp/
+-rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-07-13 19:46:55.000000 mypy-boto3-cognito-idp-1.28.3/mypy_boto3_cognito_idp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-07-13 19:46:55.000000 mypy-boto3-cognito-idp-1.28.3/mypy_boto3_cognito_idp/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-07-13 19:46:55.000000 mypy-boto3-cognito-idp-1.28.3/mypy_boto3_cognito_idp/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    78755 2023-07-13 19:46:55.000000 mypy-boto3-cognito-idp-1.28.3/mypy_boto3_cognito_idp/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    78638 2023-07-13 19:46:55.000000 mypy-boto3-cognito-idp-1.28.3/mypy_boto3_cognito_idp/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13623 2023-07-13 19:46:56.000000 mypy-boto3-cognito-idp-1.28.3/mypy_boto3_cognito_idp/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13621 2023-07-13 19:46:56.000000 mypy-boto3-cognito-idp-1.28.3/mypy_boto3_cognito_idp/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11048 2023-07-13 19:46:55.000000 mypy-boto3-cognito-idp-1.28.3/mypy_boto3_cognito_idp/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11037 2023-07-13 19:46:55.000000 mypy-boto3-cognito-idp-1.28.3/mypy_boto3_cognito_idp/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 19:46:55.000000 mypy-boto3-cognito-idp-1.28.3/mypy_boto3_cognito_idp/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    95323 2023-07-13 19:46:58.000000 mypy-boto3-cognito-idp-1.28.3/mypy_boto3_cognito_idp/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    95194 2023-07-13 19:46:57.000000 mypy-boto3-cognito-idp-1.28.3/mypy_boto3_cognito_idp/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-13 19:46:55.000000 mypy-boto3-cognito-idp-1.28.3/mypy_boto3_cognito_idp/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:49:12.665227 mypy-boto3-cognito-idp-1.28.3/mypy_boto3_cognito_idp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    25178 2023-07-13 19:49:12.000000 mypy-boto3-cognito-idp-1.28.3/mypy_boto3_cognito_idp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-07-13 19:49:12.000000 mypy-boto3-cognito-idp-1.28.3/mypy_boto3_cognito_idp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 19:49:12.000000 mypy-boto3-cognito-idp-1.28.3/mypy_boto3_cognito_idp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 19:49:12.000000 mypy-boto3-cognito-idp-1.28.3/mypy_boto3_cognito_idp.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-13 19:49:12.000000 mypy-boto3-cognito-idp-1.28.3/mypy_boto3_cognito_idp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-13 19:49:12.000000 mypy-boto3-cognito-idp-1.28.3/mypy_boto3_cognito_idp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 19:49:12.673227 mypy-boto3-cognito-idp-1.28.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-07-13 19:46:54.000000 mypy-boto3-cognito-idp-1.28.3/setup.py
```

### Comparing `mypy-boto3-cognito-idp-1.28.2/LICENSE` & `mypy-boto3-cognito-idp-1.28.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cognito-idp-1.28.2/PKG-INFO` & `mypy-boto3-cognito-idp-1.28.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-cognito-idp
-Version: 1.28.2
-Summary: Type annotations for boto3.CognitoIdentityProvider 1.28.2 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.3
+Summary: Type annotations for boto3.CognitoIdentityProvider 1.28.3 service generated with mypy-boto3-builder 7.14.6
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cognito-idp.svg?color=blue)](https://pypi.org/project/mypy-boto3-cognito-idp)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-cognito-idp?color=blue)](https://pypistats.org/packages/mypy-boto3-cognito-idp)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CognitoIdentityProvider 1.28.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider)
+[boto3.CognitoIdentityProvider 1.28.3](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider)
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
 [mypy-boto3-cognito-idp docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-cognito-idp-1.28.2/README.md` & `mypy-boto3-cognito-idp-1.28.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cognito-idp.svg?color=blue)](https://pypi.org/project/mypy-boto3-cognito-idp)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-cognito-idp?color=blue)](https://pypistats.org/packages/mypy-boto3-cognito-idp)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CognitoIdentityProvider 1.28.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider)
+[boto3.CognitoIdentityProvider 1.28.3](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider)
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
 [mypy-boto3-cognito-idp docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-cognito-idp-1.28.2/mypy_boto3_cognito_idp/__init__.py` & `mypy-boto3-cognito-idp-1.28.3/mypy_boto3_cognito_idp/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cognito-idp-1.28.2/mypy_boto3_cognito_idp/__init__.pyi` & `mypy-boto3-cognito-idp-1.28.3/mypy_boto3_cognito_idp/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cognito-idp-1.28.2/mypy_boto3_cognito_idp/__main__.py` & `mypy-boto3-cognito-idp-1.28.3/mypy_boto3_cognito_idp/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.CognitoIdentityProvider 1.28.2\nVersion:        "
-        " 1.28.2\nBuilder version: 7.14.5\nDocs:           "
+        "Type annotations for boto3.CognitoIdentityProvider 1.28.3\nVersion:        "
+        " 1.28.3\nBuilder version: 7.14.6\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.28.2")
+    print("1.28.3")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-cognito-idp-1.28.2/mypy_boto3_cognito_idp/client.py` & `mypy-boto3-cognito-idp-1.28.3/mypy_boto3_cognito_idp/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cognito-idp-1.28.2/mypy_boto3_cognito_idp/client.pyi` & `mypy-boto3-cognito-idp-1.28.3/mypy_boto3_cognito_idp/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cognito-idp-1.28.2/mypy_boto3_cognito_idp/literals.py` & `mypy-boto3-cognito-idp-1.28.3/mypy_boto3_cognito_idp/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cognito-idp-1.28.2/mypy_boto3_cognito_idp/literals.pyi` & `mypy-boto3-cognito-idp-1.28.3/mypy_boto3_cognito_idp/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cognito-idp-1.28.2/mypy_boto3_cognito_idp/paginator.py` & `mypy-boto3-cognito-idp-1.28.3/mypy_boto3_cognito_idp/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cognito-idp-1.28.2/mypy_boto3_cognito_idp/paginator.pyi` & `mypy-boto3-cognito-idp-1.28.3/mypy_boto3_cognito_idp/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cognito-idp-1.28.2/mypy_boto3_cognito_idp/type_defs.py` & `mypy-boto3-cognito-idp-1.28.3/mypy_boto3_cognito_idp/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -465,15 +465,14 @@
 
 MFAOptionTypeTypeDef = TypedDict(
     "MFAOptionTypeTypeDef",
     {
         "DeliveryMedium": DeliveryMediumTypeType,
         "AttributeName": str,
     },
-    total=False,
 )
 
 AnalyticsMetadataTypeTypeDef = TypedDict(
     "AnalyticsMetadataTypeTypeDef",
     {
         "AnalyticsEndpointId": str,
     },
@@ -544,15 +543,14 @@
         "UserPoolId": str,
         "Description": str,
         "RoleArn": str,
         "Precedence": int,
         "LastModifiedDate": datetime,
         "CreationDate": datetime,
     },
-    total=False,
 )
 
 _RequiredAdminListUserAuthEventsRequestRequestTypeDef = TypedDict(
     "_RequiredAdminListUserAuthEventsRequestRequestTypeDef",
     {
         "UserPoolId": str,
         "Username": str,
@@ -714,68 +712,51 @@
 
 ChallengeResponseTypeTypeDef = TypedDict(
     "ChallengeResponseTypeTypeDef",
     {
         "ChallengeName": ChallengeNameType,
         "ChallengeResponse": ChallengeResponseType,
     },
-    total=False,
 )
 
 EventContextDataTypeTypeDef = TypedDict(
     "EventContextDataTypeTypeDef",
     {
         "IpAddress": str,
         "DeviceName": str,
         "Timezone": str,
         "City": str,
         "Country": str,
     },
-    total=False,
 )
 
-_RequiredEventFeedbackTypeTypeDef = TypedDict(
-    "_RequiredEventFeedbackTypeTypeDef",
+EventFeedbackTypeTypeDef = TypedDict(
+    "EventFeedbackTypeTypeDef",
     {
         "FeedbackValue": FeedbackValueTypeType,
         "Provider": str,
-    },
-)
-_OptionalEventFeedbackTypeTypeDef = TypedDict(
-    "_OptionalEventFeedbackTypeTypeDef",
-    {
         "FeedbackDate": datetime,
     },
-    total=False,
 )
 
-
-class EventFeedbackTypeTypeDef(
-    _RequiredEventFeedbackTypeTypeDef, _OptionalEventFeedbackTypeTypeDef
-):
-    pass
-
-
 EventRiskTypeTypeDef = TypedDict(
     "EventRiskTypeTypeDef",
     {
         "RiskDecision": RiskDecisionTypeType,
         "RiskLevel": RiskLevelTypeType,
         "CompromisedCredentialsDetected": bool,
     },
-    total=False,
 )
 
 NewDeviceMetadataTypeTypeDef = TypedDict(
     "NewDeviceMetadataTypeTypeDef",
     {
         "DeviceKey": str,
         "DeviceGroupKey": str,
     },
-    total=False,
 )
 
 ChangePasswordRequestRequestTypeDef = TypedDict(
     "ChangePasswordRequestRequestTypeDef",
     {
         "PreviousPassword": str,
         "ProposedPassword": str,
@@ -786,15 +767,14 @@
 CodeDeliveryDetailsTypeTypeDef = TypedDict(
     "CodeDeliveryDetailsTypeTypeDef",
     {
         "Destination": str,
         "DeliveryMedium": DeliveryMediumTypeType,
         "AttributeName": str,
     },
-    total=False,
 )
 
 CompromisedCredentialsActionsTypeTypeDef = TypedDict(
     "CompromisedCredentialsActionsTypeTypeDef",
     {
         "EventAction": CompromisedCredentialsEventActionTypeType,
     },
@@ -885,15 +865,14 @@
         "ProviderType": IdentityProviderTypeTypeType,
         "ProviderDetails": Dict[str, str],
         "AttributeMapping": Dict[str, str],
         "IdpIdentifiers": List[str],
         "LastModifiedDate": datetime,
         "CreationDate": datetime,
     },
-    total=False,
 )
 
 ResourceServerScopeTypeTypeDef = TypedDict(
     "ResourceServerScopeTypeTypeDef",
     {
         "ScopeName": str,
         "ScopeDescription": str,
@@ -922,15 +901,14 @@
         "Status": UserImportJobStatusTypeType,
         "CloudWatchLogsRoleArn": str,
         "ImportedUsers": int,
         "SkippedUsers": int,
         "FailedUsers": int,
         "CompletionMessage": str,
     },
-    total=False,
 )
 
 TokenValidityUnitsTypeTypeDef = TypedDict(
     "TokenValidityUnitsTypeTypeDef",
     {
         "AccessToken": TimeUnitsTypeType,
         "IdToken": TimeUnitsTypeType,
@@ -1271,15 +1249,14 @@
         "ClientId": str,
         "ImageUrl": str,
         "CSS": str,
         "CSSVersion": str,
         "LastModifiedDate": datetime,
         "CreationDate": datetime,
     },
-    total=False,
 )
 
 _RequiredGetUserAttributeVerificationCodeRequestRequestTypeDef = TypedDict(
     "_RequiredGetUserAttributeVerificationCodeRequestRequestTypeDef",
     {
         "AccessToken": str,
         "AttributeName": str,
@@ -1309,15 +1286,14 @@
 )
 
 SoftwareTokenMfaConfigTypeTypeDef = TypedDict(
     "SoftwareTokenMfaConfigTypeTypeDef",
     {
         "Enabled": bool,
     },
-    total=False,
 )
 
 GetUserRequestRequestTypeDef = TypedDict(
     "GetUserRequestRequestTypeDef",
     {
         "AccessToken": str,
     },
@@ -1401,15 +1377,14 @@
     "ProviderDescriptionTypeDef",
     {
         "ProviderName": str,
         "ProviderType": IdentityProviderTypeTypeType,
         "LastModifiedDate": datetime,
         "CreationDate": datetime,
     },
-    total=False,
 )
 
 _RequiredListResourceServersRequestRequestTypeDef = TypedDict(
     "_RequiredListResourceServersRequestRequestTypeDef",
     {
         "UserPoolId": str,
     },
@@ -1487,15 +1462,14 @@
 UserPoolClientDescriptionTypeDef = TypedDict(
     "UserPoolClientDescriptionTypeDef",
     {
         "ClientId": str,
         "UserPoolId": str,
         "ClientName": str,
     },
-    total=False,
 )
 
 _RequiredListUserPoolsRequestRequestTypeDef = TypedDict(
     "_RequiredListUserPoolsRequestRequestTypeDef",
     {
         "MaxResults": int,
     },
@@ -1558,34 +1532,23 @@
 
 class ListUsersRequestRequestTypeDef(
     _RequiredListUsersRequestRequestTypeDef, _OptionalListUsersRequestRequestTypeDef
 ):
     pass
 
 
-_RequiredNotifyEmailTypeTypeDef = TypedDict(
-    "_RequiredNotifyEmailTypeTypeDef",
+NotifyEmailTypeTypeDef = TypedDict(
+    "NotifyEmailTypeTypeDef",
     {
         "Subject": str,
-    },
-)
-_OptionalNotifyEmailTypeTypeDef = TypedDict(
-    "_OptionalNotifyEmailTypeTypeDef",
-    {
         "HtmlBody": str,
         "TextBody": str,
     },
-    total=False,
 )
 
-
-class NotifyEmailTypeTypeDef(_RequiredNotifyEmailTypeTypeDef, _OptionalNotifyEmailTypeTypeDef):
-    pass
-
-
 NumberAttributeConstraintsTypeTypeDef = TypedDict(
     "NumberAttributeConstraintsTypeTypeDef",
     {
         "MinValue": str,
         "MaxValue": str,
     },
     total=False,
@@ -1628,15 +1591,14 @@
 
 RiskExceptionConfigurationTypeTypeDef = TypedDict(
     "RiskExceptionConfigurationTypeTypeDef",
     {
         "BlockedIPRangeList": List[str],
         "SkippedIPRangeList": List[str],
     },
-    total=False,
 )
 
 StringAttributeConstraintsTypeTypeDef = TypedDict(
     "StringAttributeConstraintsTypeTypeDef",
     {
         "MinLength": str,
         "MaxLength": str,
@@ -1827,15 +1789,14 @@
 AccountTakeoverActionsTypeTypeDef = TypedDict(
     "AccountTakeoverActionsTypeTypeDef",
     {
         "LowAction": AccountTakeoverActionTypeTypeDef,
         "MediumAction": AccountTakeoverActionTypeTypeDef,
         "HighAction": AccountTakeoverActionTypeTypeDef,
     },
-    total=False,
 )
 
 AdminCreateUserConfigTypeTypeDef = TypedDict(
     "AdminCreateUserConfigTypeTypeDef",
     {
         "AllowAdminCreateUserOnly": bool,
         "UnusedAccountValidityDays": int,
@@ -1901,15 +1862,14 @@
     {
         "DeviceKey": str,
         "DeviceAttributes": List[AttributeTypeTypeDef],
         "DeviceCreateDate": datetime,
         "DeviceLastModifiedDate": datetime,
         "DeviceLastAuthenticatedDate": datetime,
     },
-    total=False,
 )
 
 _RequiredUpdateUserAttributesRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateUserAttributesRequestRequestTypeDef",
     {
         "UserAttributes": Sequence[AttributeTypeTypeDef],
         "AccessToken": str,
@@ -2074,15 +2034,14 @@
         "Attributes": List[AttributeTypeTypeDef],
         "UserCreateDate": datetime,
         "UserLastModifiedDate": datetime,
         "Enabled": bool,
         "UserStatus": UserStatusTypeType,
         "MFAOptions": List[MFAOptionTypeTypeDef],
     },
-    total=False,
 )
 
 _RequiredAdminListGroupsForUserRequestAdminListGroupsForUserPaginateTypeDef = TypedDict(
     "_RequiredAdminListGroupsForUserRequestAdminListGroupsForUserPaginateTypeDef",
     {
         "Username": str,
         "UserPoolId": str,
@@ -2367,28 +2326,26 @@
         "CreationDate": datetime,
         "EventResponse": EventResponseTypeType,
         "EventRisk": EventRiskTypeTypeDef,
         "ChallengeResponses": List[ChallengeResponseTypeTypeDef],
         "EventContextData": EventContextDataTypeTypeDef,
         "EventFeedback": EventFeedbackTypeTypeDef,
     },
-    total=False,
 )
 
 AuthenticationResultTypeTypeDef = TypedDict(
     "AuthenticationResultTypeTypeDef",
     {
         "AccessToken": str,
         "ExpiresIn": int,
         "TokenType": str,
         "RefreshToken": str,
         "IdToken": str,
         "NewDeviceMetadata": NewDeviceMetadataTypeTypeDef,
     },
-    total=False,
 )
 
 ForgotPasswordResponseTypeDef = TypedDict(
     "ForgotPasswordResponseTypeDef",
     {
         "CodeDeliveryDetails": CodeDeliveryDetailsTypeTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -2425,36 +2382,22 @@
     "UpdateUserAttributesResponseTypeDef",
     {
         "CodeDeliveryDetailsList": List[CodeDeliveryDetailsTypeTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredCompromisedCredentialsRiskConfigurationTypeTypeDef = TypedDict(
-    "_RequiredCompromisedCredentialsRiskConfigurationTypeTypeDef",
-    {
-        "Actions": CompromisedCredentialsActionsTypeTypeDef,
-    },
-)
-_OptionalCompromisedCredentialsRiskConfigurationTypeTypeDef = TypedDict(
-    "_OptionalCompromisedCredentialsRiskConfigurationTypeTypeDef",
+CompromisedCredentialsRiskConfigurationTypeTypeDef = TypedDict(
+    "CompromisedCredentialsRiskConfigurationTypeTypeDef",
     {
         "EventFilter": List[EventFilterTypeType],
+        "Actions": CompromisedCredentialsActionsTypeTypeDef,
     },
-    total=False,
 )
 
-
-class CompromisedCredentialsRiskConfigurationTypeTypeDef(
-    _RequiredCompromisedCredentialsRiskConfigurationTypeTypeDef,
-    _OptionalCompromisedCredentialsRiskConfigurationTypeTypeDef,
-):
-    pass
-
-
 _RequiredConfirmDeviceRequestRequestTypeDef = TypedDict(
     "_RequiredConfirmDeviceRequestRequestTypeDef",
     {
         "AccessToken": str,
         "DeviceKey": str,
     },
 )
@@ -2742,15 +2685,14 @@
     "ResourceServerTypeTypeDef",
     {
         "UserPoolId": str,
         "Identifier": str,
         "Name": str,
         "Scopes": List[ResourceServerScopeTypeTypeDef],
     },
-    total=False,
 )
 
 _RequiredUpdateResourceServerRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateResourceServerRequestRequestTypeDef",
     {
         "UserPoolId": str,
         "Identifier": str,
@@ -2923,15 +2865,14 @@
         "AllowedOAuthFlowsUserPoolClient": bool,
         "AnalyticsConfiguration": AnalyticsConfigurationTypeTypeDef,
         "PreventUserExistenceErrors": PreventUserExistenceErrorTypesType,
         "EnableTokenRevocation": bool,
         "EnablePropagateAdditionalUserContextData": bool,
         "AuthSessionValidity": int,
     },
-    total=False,
 )
 
 _RequiredCreateUserPoolDomainRequestRequestTypeDef = TypedDict(
     "_RequiredCreateUserPoolDomainRequestRequestTypeDef",
     {
         "Domain": str,
         "UserPoolId": str,
@@ -2961,15 +2902,14 @@
         "Domain": str,
         "S3Bucket": str,
         "CloudFrontDistribution": str,
         "Version": str,
         "Status": DomainStatusTypeType,
         "CustomDomainConfig": CustomDomainConfigTypeTypeDef,
     },
-    total=False,
 )
 
 UpdateUserPoolDomainRequestRequestTypeDef = TypedDict(
     "UpdateUserPoolDomainRequestRequestTypeDef",
     {
         "Domain": str,
         "UserPoolId": str,
@@ -2979,15 +2919,14 @@
 
 SmsMfaConfigTypeTypeDef = TypedDict(
     "SmsMfaConfigTypeTypeDef",
     {
         "SmsAuthenticationMessage": str,
         "SmsConfiguration": SmsConfigurationTypeTypeDef,
     },
-    total=False,
 )
 
 LambdaConfigTypeTypeDef = TypedDict(
     "LambdaConfigTypeTypeDef",
     {
         "PreSignUp": str,
         "CustomMessage": str,
@@ -3036,39 +2975,26 @@
     {
         "UserPoolClients": List[UserPoolClientDescriptionTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredNotifyConfigurationTypeTypeDef = TypedDict(
-    "_RequiredNotifyConfigurationTypeTypeDef",
-    {
-        "SourceArn": str,
-    },
-)
-_OptionalNotifyConfigurationTypeTypeDef = TypedDict(
-    "_OptionalNotifyConfigurationTypeTypeDef",
+NotifyConfigurationTypeTypeDef = TypedDict(
+    "NotifyConfigurationTypeTypeDef",
     {
         "From": str,
         "ReplyTo": str,
+        "SourceArn": str,
         "BlockEmail": NotifyEmailTypeTypeDef,
         "NoActionEmail": NotifyEmailTypeTypeDef,
         "MfaEmail": NotifyEmailTypeTypeDef,
     },
-    total=False,
 )
 
-
-class NotifyConfigurationTypeTypeDef(
-    _RequiredNotifyConfigurationTypeTypeDef, _OptionalNotifyConfigurationTypeTypeDef
-):
-    pass
-
-
 UserPoolPolicyTypeTypeDef = TypedDict(
     "UserPoolPolicyTypeTypeDef",
     {
         "PasswordPolicy": PasswordPolicyTypeTypeDef,
     },
     total=False,
 )
@@ -3369,39 +3295,24 @@
         "Id": str,
         "Name": str,
         "LambdaConfig": LambdaConfigTypeTypeDef,
         "Status": StatusTypeType,
         "LastModifiedDate": datetime,
         "CreationDate": datetime,
     },
-    total=False,
 )
 
-_RequiredAccountTakeoverRiskConfigurationTypeTypeDef = TypedDict(
-    "_RequiredAccountTakeoverRiskConfigurationTypeTypeDef",
-    {
-        "Actions": AccountTakeoverActionsTypeTypeDef,
-    },
-)
-_OptionalAccountTakeoverRiskConfigurationTypeTypeDef = TypedDict(
-    "_OptionalAccountTakeoverRiskConfigurationTypeTypeDef",
+AccountTakeoverRiskConfigurationTypeTypeDef = TypedDict(
+    "AccountTakeoverRiskConfigurationTypeTypeDef",
     {
         "NotifyConfiguration": NotifyConfigurationTypeTypeDef,
+        "Actions": AccountTakeoverActionsTypeTypeDef,
     },
-    total=False,
 )
 
-
-class AccountTakeoverRiskConfigurationTypeTypeDef(
-    _RequiredAccountTakeoverRiskConfigurationTypeTypeDef,
-    _OptionalAccountTakeoverRiskConfigurationTypeTypeDef,
-):
-    pass
-
-
 _RequiredUpdateUserPoolRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateUserPoolRequestRequestTypeDef",
     {
         "UserPoolId": str,
     },
 )
 _OptionalUpdateUserPoolRequestRequestTypeDef = TypedDict(
@@ -3519,15 +3430,14 @@
         "CustomDomain": str,
         "AdminCreateUserConfig": AdminCreateUserConfigTypeTypeDef,
         "UserPoolAddOns": UserPoolAddOnsTypeTypeDef,
         "UsernameConfiguration": UsernameConfigurationTypeTypeDef,
         "Arn": str,
         "AccountRecoverySetting": AccountRecoverySettingTypeTypeDef,
     },
-    total=False,
 )
 
 ListUserPoolsResponseTypeDef = TypedDict(
     "ListUserPoolsResponseTypeDef",
     {
         "UserPools": List[UserPoolDescriptionTypeTypeDef],
         "NextToken": str,
@@ -3543,15 +3453,14 @@
         "CompromisedCredentialsRiskConfiguration": (
             CompromisedCredentialsRiskConfigurationTypeTypeDef
         ),
         "AccountTakeoverRiskConfiguration": AccountTakeoverRiskConfigurationTypeTypeDef,
         "RiskExceptionConfiguration": RiskExceptionConfigurationTypeTypeDef,
         "LastModifiedDate": datetime,
     },
-    total=False,
 )
 
 _RequiredSetRiskConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredSetRiskConfigurationRequestRequestTypeDef",
     {
         "UserPoolId": str,
     },
```

### Comparing `mypy-boto3-cognito-idp-1.28.2/mypy_boto3_cognito_idp/type_defs.pyi` & `mypy-boto3-cognito-idp-1.28.3/mypy_boto3_cognito_idp/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -460,15 +460,14 @@
 
 MFAOptionTypeTypeDef = TypedDict(
     "MFAOptionTypeTypeDef",
     {
         "DeliveryMedium": DeliveryMediumTypeType,
         "AttributeName": str,
     },
-    total=False,
 )
 
 AnalyticsMetadataTypeTypeDef = TypedDict(
     "AnalyticsMetadataTypeTypeDef",
     {
         "AnalyticsEndpointId": str,
     },
@@ -535,15 +534,14 @@
         "UserPoolId": str,
         "Description": str,
         "RoleArn": str,
         "Precedence": int,
         "LastModifiedDate": datetime,
         "CreationDate": datetime,
     },
-    total=False,
 )
 
 _RequiredAdminListUserAuthEventsRequestRequestTypeDef = TypedDict(
     "_RequiredAdminListUserAuthEventsRequestRequestTypeDef",
     {
         "UserPoolId": str,
         "Username": str,
@@ -697,66 +695,51 @@
 
 ChallengeResponseTypeTypeDef = TypedDict(
     "ChallengeResponseTypeTypeDef",
     {
         "ChallengeName": ChallengeNameType,
         "ChallengeResponse": ChallengeResponseType,
     },
-    total=False,
 )
 
 EventContextDataTypeTypeDef = TypedDict(
     "EventContextDataTypeTypeDef",
     {
         "IpAddress": str,
         "DeviceName": str,
         "Timezone": str,
         "City": str,
         "Country": str,
     },
-    total=False,
 )
 
-_RequiredEventFeedbackTypeTypeDef = TypedDict(
-    "_RequiredEventFeedbackTypeTypeDef",
+EventFeedbackTypeTypeDef = TypedDict(
+    "EventFeedbackTypeTypeDef",
     {
         "FeedbackValue": FeedbackValueTypeType,
         "Provider": str,
-    },
-)
-_OptionalEventFeedbackTypeTypeDef = TypedDict(
-    "_OptionalEventFeedbackTypeTypeDef",
-    {
         "FeedbackDate": datetime,
     },
-    total=False,
 )
 
-class EventFeedbackTypeTypeDef(
-    _RequiredEventFeedbackTypeTypeDef, _OptionalEventFeedbackTypeTypeDef
-):
-    pass
-
 EventRiskTypeTypeDef = TypedDict(
     "EventRiskTypeTypeDef",
     {
         "RiskDecision": RiskDecisionTypeType,
         "RiskLevel": RiskLevelTypeType,
         "CompromisedCredentialsDetected": bool,
     },
-    total=False,
 )
 
 NewDeviceMetadataTypeTypeDef = TypedDict(
     "NewDeviceMetadataTypeTypeDef",
     {
         "DeviceKey": str,
         "DeviceGroupKey": str,
     },
-    total=False,
 )
 
 ChangePasswordRequestRequestTypeDef = TypedDict(
     "ChangePasswordRequestRequestTypeDef",
     {
         "PreviousPassword": str,
         "ProposedPassword": str,
@@ -767,15 +750,14 @@
 CodeDeliveryDetailsTypeTypeDef = TypedDict(
     "CodeDeliveryDetailsTypeTypeDef",
     {
         "Destination": str,
         "DeliveryMedium": DeliveryMediumTypeType,
         "AttributeName": str,
     },
-    total=False,
 )
 
 CompromisedCredentialsActionsTypeTypeDef = TypedDict(
     "CompromisedCredentialsActionsTypeTypeDef",
     {
         "EventAction": CompromisedCredentialsEventActionTypeType,
     },
@@ -862,15 +844,14 @@
         "ProviderType": IdentityProviderTypeTypeType,
         "ProviderDetails": Dict[str, str],
         "AttributeMapping": Dict[str, str],
         "IdpIdentifiers": List[str],
         "LastModifiedDate": datetime,
         "CreationDate": datetime,
     },
-    total=False,
 )
 
 ResourceServerScopeTypeTypeDef = TypedDict(
     "ResourceServerScopeTypeTypeDef",
     {
         "ScopeName": str,
         "ScopeDescription": str,
@@ -899,15 +880,14 @@
         "Status": UserImportJobStatusTypeType,
         "CloudWatchLogsRoleArn": str,
         "ImportedUsers": int,
         "SkippedUsers": int,
         "FailedUsers": int,
         "CompletionMessage": str,
     },
-    total=False,
 )
 
 TokenValidityUnitsTypeTypeDef = TypedDict(
     "TokenValidityUnitsTypeTypeDef",
     {
         "AccessToken": TimeUnitsTypeType,
         "IdToken": TimeUnitsTypeType,
@@ -1238,15 +1218,14 @@
         "ClientId": str,
         "ImageUrl": str,
         "CSS": str,
         "CSSVersion": str,
         "LastModifiedDate": datetime,
         "CreationDate": datetime,
     },
-    total=False,
 )
 
 _RequiredGetUserAttributeVerificationCodeRequestRequestTypeDef = TypedDict(
     "_RequiredGetUserAttributeVerificationCodeRequestRequestTypeDef",
     {
         "AccessToken": str,
         "AttributeName": str,
@@ -1274,15 +1253,14 @@
 )
 
 SoftwareTokenMfaConfigTypeTypeDef = TypedDict(
     "SoftwareTokenMfaConfigTypeTypeDef",
     {
         "Enabled": bool,
     },
-    total=False,
 )
 
 GetUserRequestRequestTypeDef = TypedDict(
     "GetUserRequestRequestTypeDef",
     {
         "AccessToken": str,
     },
@@ -1360,15 +1338,14 @@
     "ProviderDescriptionTypeDef",
     {
         "ProviderName": str,
         "ProviderType": IdentityProviderTypeTypeType,
         "LastModifiedDate": datetime,
         "CreationDate": datetime,
     },
-    total=False,
 )
 
 _RequiredListResourceServersRequestRequestTypeDef = TypedDict(
     "_RequiredListResourceServersRequestRequestTypeDef",
     {
         "UserPoolId": str,
     },
@@ -1440,15 +1417,14 @@
 UserPoolClientDescriptionTypeDef = TypedDict(
     "UserPoolClientDescriptionTypeDef",
     {
         "ClientId": str,
         "UserPoolId": str,
         "ClientName": str,
     },
-    total=False,
 )
 
 _RequiredListUserPoolsRequestRequestTypeDef = TypedDict(
     "_RequiredListUserPoolsRequestRequestTypeDef",
     {
         "MaxResults": int,
     },
@@ -1505,32 +1481,23 @@
 )
 
 class ListUsersRequestRequestTypeDef(
     _RequiredListUsersRequestRequestTypeDef, _OptionalListUsersRequestRequestTypeDef
 ):
     pass
 
-_RequiredNotifyEmailTypeTypeDef = TypedDict(
-    "_RequiredNotifyEmailTypeTypeDef",
+NotifyEmailTypeTypeDef = TypedDict(
+    "NotifyEmailTypeTypeDef",
     {
         "Subject": str,
-    },
-)
-_OptionalNotifyEmailTypeTypeDef = TypedDict(
-    "_OptionalNotifyEmailTypeTypeDef",
-    {
         "HtmlBody": str,
         "TextBody": str,
     },
-    total=False,
 )
 
-class NotifyEmailTypeTypeDef(_RequiredNotifyEmailTypeTypeDef, _OptionalNotifyEmailTypeTypeDef):
-    pass
-
 NumberAttributeConstraintsTypeTypeDef = TypedDict(
     "NumberAttributeConstraintsTypeTypeDef",
     {
         "MinValue": str,
         "MaxValue": str,
     },
     total=False,
@@ -1571,15 +1538,14 @@
 
 RiskExceptionConfigurationTypeTypeDef = TypedDict(
     "RiskExceptionConfigurationTypeTypeDef",
     {
         "BlockedIPRangeList": List[str],
         "SkippedIPRangeList": List[str],
     },
-    total=False,
 )
 
 StringAttributeConstraintsTypeTypeDef = TypedDict(
     "StringAttributeConstraintsTypeTypeDef",
     {
         "MinLength": str,
         "MaxLength": str,
@@ -1760,15 +1726,14 @@
 AccountTakeoverActionsTypeTypeDef = TypedDict(
     "AccountTakeoverActionsTypeTypeDef",
     {
         "LowAction": AccountTakeoverActionTypeTypeDef,
         "MediumAction": AccountTakeoverActionTypeTypeDef,
         "HighAction": AccountTakeoverActionTypeTypeDef,
     },
-    total=False,
 )
 
 AdminCreateUserConfigTypeTypeDef = TypedDict(
     "AdminCreateUserConfigTypeTypeDef",
     {
         "AllowAdminCreateUserOnly": bool,
         "UnusedAccountValidityDays": int,
@@ -1830,15 +1795,14 @@
     {
         "DeviceKey": str,
         "DeviceAttributes": List[AttributeTypeTypeDef],
         "DeviceCreateDate": datetime,
         "DeviceLastModifiedDate": datetime,
         "DeviceLastAuthenticatedDate": datetime,
     },
-    total=False,
 )
 
 _RequiredUpdateUserAttributesRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateUserAttributesRequestRequestTypeDef",
     {
         "UserAttributes": Sequence[AttributeTypeTypeDef],
         "AccessToken": str,
@@ -2001,15 +1965,14 @@
         "Attributes": List[AttributeTypeTypeDef],
         "UserCreateDate": datetime,
         "UserLastModifiedDate": datetime,
         "Enabled": bool,
         "UserStatus": UserStatusTypeType,
         "MFAOptions": List[MFAOptionTypeTypeDef],
     },
-    total=False,
 )
 
 _RequiredAdminListGroupsForUserRequestAdminListGroupsForUserPaginateTypeDef = TypedDict(
     "_RequiredAdminListGroupsForUserRequestAdminListGroupsForUserPaginateTypeDef",
     {
         "Username": str,
         "UserPoolId": str,
@@ -2274,28 +2237,26 @@
         "CreationDate": datetime,
         "EventResponse": EventResponseTypeType,
         "EventRisk": EventRiskTypeTypeDef,
         "ChallengeResponses": List[ChallengeResponseTypeTypeDef],
         "EventContextData": EventContextDataTypeTypeDef,
         "EventFeedback": EventFeedbackTypeTypeDef,
     },
-    total=False,
 )
 
 AuthenticationResultTypeTypeDef = TypedDict(
     "AuthenticationResultTypeTypeDef",
     {
         "AccessToken": str,
         "ExpiresIn": int,
         "TokenType": str,
         "RefreshToken": str,
         "IdToken": str,
         "NewDeviceMetadata": NewDeviceMetadataTypeTypeDef,
     },
-    total=False,
 )
 
 ForgotPasswordResponseTypeDef = TypedDict(
     "ForgotPasswordResponseTypeDef",
     {
         "CodeDeliveryDetails": CodeDeliveryDetailsTypeTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -2332,34 +2293,22 @@
     "UpdateUserAttributesResponseTypeDef",
     {
         "CodeDeliveryDetailsList": List[CodeDeliveryDetailsTypeTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredCompromisedCredentialsRiskConfigurationTypeTypeDef = TypedDict(
-    "_RequiredCompromisedCredentialsRiskConfigurationTypeTypeDef",
-    {
-        "Actions": CompromisedCredentialsActionsTypeTypeDef,
-    },
-)
-_OptionalCompromisedCredentialsRiskConfigurationTypeTypeDef = TypedDict(
-    "_OptionalCompromisedCredentialsRiskConfigurationTypeTypeDef",
+CompromisedCredentialsRiskConfigurationTypeTypeDef = TypedDict(
+    "CompromisedCredentialsRiskConfigurationTypeTypeDef",
     {
         "EventFilter": List[EventFilterTypeType],
+        "Actions": CompromisedCredentialsActionsTypeTypeDef,
     },
-    total=False,
 )
 
-class CompromisedCredentialsRiskConfigurationTypeTypeDef(
-    _RequiredCompromisedCredentialsRiskConfigurationTypeTypeDef,
-    _OptionalCompromisedCredentialsRiskConfigurationTypeTypeDef,
-):
-    pass
-
 _RequiredConfirmDeviceRequestRequestTypeDef = TypedDict(
     "_RequiredConfirmDeviceRequestRequestTypeDef",
     {
         "AccessToken": str,
         "DeviceKey": str,
     },
 )
@@ -2627,15 +2576,14 @@
     "ResourceServerTypeTypeDef",
     {
         "UserPoolId": str,
         "Identifier": str,
         "Name": str,
         "Scopes": List[ResourceServerScopeTypeTypeDef],
     },
-    total=False,
 )
 
 _RequiredUpdateResourceServerRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateResourceServerRequestRequestTypeDef",
     {
         "UserPoolId": str,
         "Identifier": str,
@@ -2802,15 +2750,14 @@
         "AllowedOAuthFlowsUserPoolClient": bool,
         "AnalyticsConfiguration": AnalyticsConfigurationTypeTypeDef,
         "PreventUserExistenceErrors": PreventUserExistenceErrorTypesType,
         "EnableTokenRevocation": bool,
         "EnablePropagateAdditionalUserContextData": bool,
         "AuthSessionValidity": int,
     },
-    total=False,
 )
 
 _RequiredCreateUserPoolDomainRequestRequestTypeDef = TypedDict(
     "_RequiredCreateUserPoolDomainRequestRequestTypeDef",
     {
         "Domain": str,
         "UserPoolId": str,
@@ -2838,15 +2785,14 @@
         "Domain": str,
         "S3Bucket": str,
         "CloudFrontDistribution": str,
         "Version": str,
         "Status": DomainStatusTypeType,
         "CustomDomainConfig": CustomDomainConfigTypeTypeDef,
     },
-    total=False,
 )
 
 UpdateUserPoolDomainRequestRequestTypeDef = TypedDict(
     "UpdateUserPoolDomainRequestRequestTypeDef",
     {
         "Domain": str,
         "UserPoolId": str,
@@ -2856,15 +2802,14 @@
 
 SmsMfaConfigTypeTypeDef = TypedDict(
     "SmsMfaConfigTypeTypeDef",
     {
         "SmsAuthenticationMessage": str,
         "SmsConfiguration": SmsConfigurationTypeTypeDef,
     },
-    total=False,
 )
 
 LambdaConfigTypeTypeDef = TypedDict(
     "LambdaConfigTypeTypeDef",
     {
         "PreSignUp": str,
         "CustomMessage": str,
@@ -2913,37 +2858,26 @@
     {
         "UserPoolClients": List[UserPoolClientDescriptionTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredNotifyConfigurationTypeTypeDef = TypedDict(
-    "_RequiredNotifyConfigurationTypeTypeDef",
-    {
-        "SourceArn": str,
-    },
-)
-_OptionalNotifyConfigurationTypeTypeDef = TypedDict(
-    "_OptionalNotifyConfigurationTypeTypeDef",
+NotifyConfigurationTypeTypeDef = TypedDict(
+    "NotifyConfigurationTypeTypeDef",
     {
         "From": str,
         "ReplyTo": str,
+        "SourceArn": str,
         "BlockEmail": NotifyEmailTypeTypeDef,
         "NoActionEmail": NotifyEmailTypeTypeDef,
         "MfaEmail": NotifyEmailTypeTypeDef,
     },
-    total=False,
 )
 
-class NotifyConfigurationTypeTypeDef(
-    _RequiredNotifyConfigurationTypeTypeDef, _OptionalNotifyConfigurationTypeTypeDef
-):
-    pass
-
 UserPoolPolicyTypeTypeDef = TypedDict(
     "UserPoolPolicyTypeTypeDef",
     {
         "PasswordPolicy": PasswordPolicyTypeTypeDef,
     },
     total=False,
 )
@@ -3238,37 +3172,24 @@
         "Id": str,
         "Name": str,
         "LambdaConfig": LambdaConfigTypeTypeDef,
         "Status": StatusTypeType,
         "LastModifiedDate": datetime,
         "CreationDate": datetime,
     },
-    total=False,
 )
 
-_RequiredAccountTakeoverRiskConfigurationTypeTypeDef = TypedDict(
-    "_RequiredAccountTakeoverRiskConfigurationTypeTypeDef",
-    {
-        "Actions": AccountTakeoverActionsTypeTypeDef,
-    },
-)
-_OptionalAccountTakeoverRiskConfigurationTypeTypeDef = TypedDict(
-    "_OptionalAccountTakeoverRiskConfigurationTypeTypeDef",
+AccountTakeoverRiskConfigurationTypeTypeDef = TypedDict(
+    "AccountTakeoverRiskConfigurationTypeTypeDef",
     {
         "NotifyConfiguration": NotifyConfigurationTypeTypeDef,
+        "Actions": AccountTakeoverActionsTypeTypeDef,
     },
-    total=False,
 )
 
-class AccountTakeoverRiskConfigurationTypeTypeDef(
-    _RequiredAccountTakeoverRiskConfigurationTypeTypeDef,
-    _OptionalAccountTakeoverRiskConfigurationTypeTypeDef,
-):
-    pass
-
 _RequiredUpdateUserPoolRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateUserPoolRequestRequestTypeDef",
     {
         "UserPoolId": str,
     },
 )
 _OptionalUpdateUserPoolRequestRequestTypeDef = TypedDict(
@@ -3382,15 +3303,14 @@
         "CustomDomain": str,
         "AdminCreateUserConfig": AdminCreateUserConfigTypeTypeDef,
         "UserPoolAddOns": UserPoolAddOnsTypeTypeDef,
         "UsernameConfiguration": UsernameConfigurationTypeTypeDef,
         "Arn": str,
         "AccountRecoverySetting": AccountRecoverySettingTypeTypeDef,
     },
-    total=False,
 )
 
 ListUserPoolsResponseTypeDef = TypedDict(
     "ListUserPoolsResponseTypeDef",
     {
         "UserPools": List[UserPoolDescriptionTypeTypeDef],
         "NextToken": str,
@@ -3406,15 +3326,14 @@
         "CompromisedCredentialsRiskConfiguration": (
             CompromisedCredentialsRiskConfigurationTypeTypeDef
         ),
         "AccountTakeoverRiskConfiguration": AccountTakeoverRiskConfigurationTypeTypeDef,
         "RiskExceptionConfiguration": RiskExceptionConfigurationTypeTypeDef,
         "LastModifiedDate": datetime,
     },
-    total=False,
 )
 
 _RequiredSetRiskConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredSetRiskConfigurationRequestRequestTypeDef",
     {
         "UserPoolId": str,
     },
```

### Comparing `mypy-boto3-cognito-idp-1.28.2/mypy_boto3_cognito_idp.egg-info/PKG-INFO` & `mypy-boto3-cognito-idp-1.28.3/mypy_boto3_cognito_idp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-cognito-idp
-Version: 1.28.2
-Summary: Type annotations for boto3.CognitoIdentityProvider 1.28.2 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.3
+Summary: Type annotations for boto3.CognitoIdentityProvider 1.28.3 service generated with mypy-boto3-builder 7.14.6
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cognito-idp.svg?color=blue)](https://pypi.org/project/mypy-boto3-cognito-idp)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-cognito-idp?color=blue)](https://pypistats.org/packages/mypy-boto3-cognito-idp)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CognitoIdentityProvider 1.28.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider)
+[boto3.CognitoIdentityProvider 1.28.3](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider)
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
 [mypy-boto3-cognito-idp docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-cognito-idp-1.28.2/mypy_boto3_cognito_idp.egg-info/SOURCES.txt` & `mypy-boto3-cognito-idp-1.28.3/mypy_boto3_cognito_idp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cognito-idp-1.28.2/setup.py` & `mypy-boto3-cognito-idp-1.28.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-cognito-idp",
-    version="1.28.2",
+    version="1.28.3",
     packages=["mypy_boto3_cognito_idp"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.CognitoIdentityProvider 1.28.2 service generated with"
-        " mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.CognitoIdentityProvider 1.28.3 service generated with"
+        " mypy-boto3-builder 7.14.6"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

