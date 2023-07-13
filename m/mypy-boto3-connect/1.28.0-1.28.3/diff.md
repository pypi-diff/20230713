# Comparing `tmp/mypy-boto3-connect-1.28.0.tar.gz` & `tmp/mypy-boto3-connect-1.28.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-connect-1.28.0.tar", last modified: Thu Jul  6 20:59:19 2023, max compression
+gzip compressed data, was "mypy-boto3-connect-1.28.3.tar", last modified: Thu Jul 13 19:49:12 2023, max compression
```

## Comparing `mypy-boto3-connect-1.28.0.tar` & `mypy-boto3-connect-1.28.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:19.570267 mypy-boto3-connect-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:36:53.000000 mypy-boto3-connect-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    45299 2023-07-06 20:59:19.566267 mypy-boto3-connect-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    43814 2023-07-06 20:36:53.000000 mypy-boto3-connect-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:19.562267 mypy-boto3-connect-1.28.0/mypy_boto3_connect/
--rw-r--r--   0 runner    (1001) docker     (123)    10262 2023-07-06 20:36:53.000000 mypy-boto3-connect-1.28.0/mypy_boto3_connect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10261 2023-07-06 20:36:53.000000 mypy-boto3-connect-1.28.0/mypy_boto3_connect/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-07-06 20:36:53.000000 mypy-boto3-connect-1.28.0/mypy_boto3_connect/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)   150407 2023-07-06 20:36:56.000000 mypy-boto3-connect-1.28.0/mypy_boto3_connect/client.py
--rw-r--r--   0 runner    (1001) docker     (123)   150161 2023-07-06 20:36:54.000000 mypy-boto3-connect-1.28.0/mypy_boto3_connect/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    25344 2023-07-06 20:36:57.000000 mypy-boto3-connect-1.28.0/mypy_boto3_connect/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    25342 2023-07-06 20:36:57.000000 mypy-boto3-connect-1.28.0/mypy_boto3_connect/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    54314 2023-07-06 20:36:56.000000 mypy-boto3-connect-1.28.0/mypy_boto3_connect/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    54267 2023-07-06 20:36:56.000000 mypy-boto3-connect-1.28.0/mypy_boto3_connect/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:36:53.000000 mypy-boto3-connect-1.28.0/mypy_boto3_connect/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   218168 2023-07-06 20:37:05.000000 mypy-boto3-connect-1.28.0/mypy_boto3_connect/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   217837 2023-07-06 20:37:01.000000 mypy-boto3-connect-1.28.0/mypy_boto3_connect/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:36:53.000000 mypy-boto3-connect-1.28.0/mypy_boto3_connect/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:19.566267 mypy-boto3-connect-1.28.0/mypy_boto3_connect.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    45299 2023-07-06 20:59:19.000000 mypy-boto3-connect-1.28.0/mypy_boto3_connect.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-07-06 20:59:19.000000 mypy-boto3-connect-1.28.0/mypy_boto3_connect.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:19.000000 mypy-boto3-connect-1.28.0/mypy_boto3_connect.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:19.000000 mypy-boto3-connect-1.28.0/mypy_boto3_connect.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 20:59:19.000000 mypy-boto3-connect-1.28.0/mypy_boto3_connect.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-06 20:59:19.000000 mypy-boto3-connect-1.28.0/mypy_boto3_connect.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 20:59:19.570267 mypy-boto3-connect-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-07-06 20:36:53.000000 mypy-boto3-connect-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:49:12.665227 mypy-boto3-connect-1.28.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-13 19:47:00.000000 mypy-boto3-connect-1.28.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    45384 2023-07-13 19:49:12.665227 mypy-boto3-connect-1.28.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    43899 2023-07-13 19:47:00.000000 mypy-boto3-connect-1.28.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:49:12.653227 mypy-boto3-connect-1.28.3/mypy_boto3_connect/
+-rw-r--r--   0 runner    (1001) docker     (123)    10262 2023-07-13 19:47:00.000000 mypy-boto3-connect-1.28.3/mypy_boto3_connect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10261 2023-07-13 19:47:00.000000 mypy-boto3-connect-1.28.3/mypy_boto3_connect/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-07-13 19:47:00.000000 mypy-boto3-connect-1.28.3/mypy_boto3_connect/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   151314 2023-07-13 19:47:01.000000 mypy-boto3-connect-1.28.3/mypy_boto3_connect/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)   151066 2023-07-13 19:47:00.000000 mypy-boto3-connect-1.28.3/mypy_boto3_connect/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    25344 2023-07-13 19:47:02.000000 mypy-boto3-connect-1.28.3/mypy_boto3_connect/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25342 2023-07-13 19:47:02.000000 mypy-boto3-connect-1.28.3/mypy_boto3_connect/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    54314 2023-07-13 19:47:02.000000 mypy-boto3-connect-1.28.3/mypy_boto3_connect/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54267 2023-07-13 19:47:02.000000 mypy-boto3-connect-1.28.3/mypy_boto3_connect/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 19:47:00.000000 mypy-boto3-connect-1.28.3/mypy_boto3_connect/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   215088 2023-07-13 19:47:08.000000 mypy-boto3-connect-1.28.3/mypy_boto3_connect/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   214775 2023-07-13 19:47:05.000000 mypy-boto3-connect-1.28.3/mypy_boto3_connect/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-13 19:47:00.000000 mypy-boto3-connect-1.28.3/mypy_boto3_connect/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:49:12.665227 mypy-boto3-connect-1.28.3/mypy_boto3_connect.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    45384 2023-07-13 19:49:12.000000 mypy-boto3-connect-1.28.3/mypy_boto3_connect.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-07-13 19:49:12.000000 mypy-boto3-connect-1.28.3/mypy_boto3_connect.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 19:49:12.000000 mypy-boto3-connect-1.28.3/mypy_boto3_connect.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 19:49:12.000000 mypy-boto3-connect-1.28.3/mypy_boto3_connect.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-13 19:49:12.000000 mypy-boto3-connect-1.28.3/mypy_boto3_connect.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-13 19:49:12.000000 mypy-boto3-connect-1.28.3/mypy_boto3_connect.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 19:49:12.665227 mypy-boto3-connect-1.28.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-07-13 19:47:00.000000 mypy-boto3-connect-1.28.3/setup.py
```

### Comparing `mypy-boto3-connect-1.28.0/LICENSE` & `mypy-boto3-connect-1.28.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-connect-1.28.0/PKG-INFO` & `mypy-boto3-connect-1.28.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-connect
-Version: 1.28.0
-Summary: Type annotations for boto3.Connect 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.3
+Summary: Type annotations for boto3.Connect 1.28.3 service generated with mypy-boto3-builder 7.14.6
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-connect.svg?color=blue)](https://pypi.org/project/mypy-boto3-connect)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-connect?color=blue)](https://pypistats.org/packages/mypy-boto3-connect)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Connect 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect)
+[boto3.Connect 1.28.3](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect)
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
 [mypy-boto3-connect docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/).
 
 See how it helps to find and fix potential bugs:
 
@@ -673,15 +673,17 @@
     DeleteContactFlowModuleRequestRequestTypeDef,
     DeleteContactFlowRequestRequestTypeDef,
     DeleteEvaluationFormRequestRequestTypeDef,
     DeleteHoursOfOperationRequestRequestTypeDef,
     DeleteInstanceRequestRequestTypeDef,
     DeleteIntegrationAssociationRequestRequestTypeDef,
     DeletePromptRequestRequestTypeDef,
+    DeleteQueueRequestRequestTypeDef,
     DeleteQuickConnectRequestRequestTypeDef,
+    DeleteRoutingProfileRequestRequestTypeDef,
     DeleteRuleRequestRequestTypeDef,
     DeleteSecurityProfileRequestRequestTypeDef,
     DeleteTaskTemplateRequestRequestTypeDef,
     DeleteTrafficDistributionGroupRequestRequestTypeDef,
     DeleteUseCaseRequestRequestTypeDef,
     DeleteUserHierarchyGroupRequestRequestTypeDef,
     DeleteUserRequestRequestTypeDef,
```

### Comparing `mypy-boto3-connect-1.28.0/README.md` & `mypy-boto3-connect-1.28.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-connect.svg?color=blue)](https://pypi.org/project/mypy-boto3-connect)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-connect?color=blue)](https://pypistats.org/packages/mypy-boto3-connect)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Connect 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect)
+[boto3.Connect 1.28.3](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect)
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
 [mypy-boto3-connect docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/).
 
 See how it helps to find and fix potential bugs:
 
@@ -641,15 +641,17 @@
     DeleteContactFlowModuleRequestRequestTypeDef,
     DeleteContactFlowRequestRequestTypeDef,
     DeleteEvaluationFormRequestRequestTypeDef,
     DeleteHoursOfOperationRequestRequestTypeDef,
     DeleteInstanceRequestRequestTypeDef,
     DeleteIntegrationAssociationRequestRequestTypeDef,
     DeletePromptRequestRequestTypeDef,
+    DeleteQueueRequestRequestTypeDef,
     DeleteQuickConnectRequestRequestTypeDef,
+    DeleteRoutingProfileRequestRequestTypeDef,
     DeleteRuleRequestRequestTypeDef,
     DeleteSecurityProfileRequestRequestTypeDef,
     DeleteTaskTemplateRequestRequestTypeDef,
     DeleteTrafficDistributionGroupRequestRequestTypeDef,
     DeleteUseCaseRequestRequestTypeDef,
     DeleteUserHierarchyGroupRequestRequestTypeDef,
     DeleteUserRequestRequestTypeDef,
```

### Comparing `mypy-boto3-connect-1.28.0/mypy_boto3_connect/__init__.py` & `mypy-boto3-connect-1.28.3/mypy_boto3_connect/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-connect-1.28.0/mypy_boto3_connect/__init__.pyi` & `mypy-boto3-connect-1.28.3/mypy_boto3_connect/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-connect-1.28.0/mypy_boto3_connect/__main__.py` & `mypy-boto3-connect-1.28.3/mypy_boto3_connect/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Connect 1.28.0\nVersion:         1.28.0\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.Connect 1.28.3\nVersion:         1.28.3\nBuilder version:"
+        " 7.14.6\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect\nOther"
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

### Comparing `mypy-boto3-connect-1.28.0/mypy_boto3_connect/client.py` & `mypy-boto3-connect-1.28.3/mypy_boto3_connect/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -900,24 +900,42 @@
         """
         Deletes a prompt.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.delete_prompt)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#delete_prompt)
         """
 
+    def delete_queue(self, *, InstanceId: str, QueueId: str) -> EmptyResponseMetadataTypeDef:
+        """
+        Deletes a queue.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.delete_queue)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#delete_queue)
+        """
+
     def delete_quick_connect(
         self, *, InstanceId: str, QuickConnectId: str
     ) -> EmptyResponseMetadataTypeDef:
         """
         Deletes a quick connect.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.delete_quick_connect)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#delete_quick_connect)
         """
 
+    def delete_routing_profile(
+        self, *, InstanceId: str, RoutingProfileId: str
+    ) -> EmptyResponseMetadataTypeDef:
+        """
+        Deletes a routing profile.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.delete_routing_profile)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#delete_routing_profile)
+        """
+
     def delete_rule(self, *, InstanceId: str, RuleId: str) -> EmptyResponseMetadataTypeDef:
         """
         Deletes a rule for the specified Amazon Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.delete_rule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#delete_rule)
         """
```

### Comparing `mypy-boto3-connect-1.28.0/mypy_boto3_connect/client.pyi` & `mypy-boto3-connect-1.28.3/mypy_boto3_connect/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -852,23 +852,39 @@
     def delete_prompt(self, *, InstanceId: str, PromptId: str) -> EmptyResponseMetadataTypeDef:
         """
         Deletes a prompt.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.delete_prompt)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#delete_prompt)
         """
+    def delete_queue(self, *, InstanceId: str, QueueId: str) -> EmptyResponseMetadataTypeDef:
+        """
+        Deletes a queue.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.delete_queue)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#delete_queue)
+        """
     def delete_quick_connect(
         self, *, InstanceId: str, QuickConnectId: str
     ) -> EmptyResponseMetadataTypeDef:
         """
         Deletes a quick connect.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.delete_quick_connect)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#delete_quick_connect)
         """
+    def delete_routing_profile(
+        self, *, InstanceId: str, RoutingProfileId: str
+    ) -> EmptyResponseMetadataTypeDef:
+        """
+        Deletes a routing profile.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.delete_routing_profile)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#delete_routing_profile)
+        """
     def delete_rule(self, *, InstanceId: str, RuleId: str) -> EmptyResponseMetadataTypeDef:
         """
         Deletes a rule for the specified Amazon Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.delete_rule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/client/#delete_rule)
         """
```

### Comparing `mypy-boto3-connect-1.28.0/mypy_boto3_connect/literals.py` & `mypy-boto3-connect-1.28.3/mypy_boto3_connect/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-connect-1.28.0/mypy_boto3_connect/literals.pyi` & `mypy-boto3-connect-1.28.3/mypy_boto3_connect/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-connect-1.28.0/mypy_boto3_connect/paginator.py` & `mypy-boto3-connect-1.28.3/mypy_boto3_connect/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-connect-1.28.0/mypy_boto3_connect/paginator.pyi` & `mypy-boto3-connect-1.28.3/mypy_boto3_connect/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-connect-1.28.0/mypy_boto3_connect/type_defs.py` & `mypy-boto3-connect-1.28.3/mypy_boto3_connect/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -180,15 +180,17 @@
     "DeleteContactFlowModuleRequestRequestTypeDef",
     "DeleteContactFlowRequestRequestTypeDef",
     "DeleteEvaluationFormRequestRequestTypeDef",
     "DeleteHoursOfOperationRequestRequestTypeDef",
     "DeleteInstanceRequestRequestTypeDef",
     "DeleteIntegrationAssociationRequestRequestTypeDef",
     "DeletePromptRequestRequestTypeDef",
+    "DeleteQueueRequestRequestTypeDef",
     "DeleteQuickConnectRequestRequestTypeDef",
+    "DeleteRoutingProfileRequestRequestTypeDef",
     "DeleteRuleRequestRequestTypeDef",
     "DeleteSecurityProfileRequestRequestTypeDef",
     "DeleteTaskTemplateRequestRequestTypeDef",
     "DeleteTrafficDistributionGroupRequestRequestTypeDef",
     "DeleteUseCaseRequestRequestTypeDef",
     "DeleteUserHierarchyGroupRequestRequestTypeDef",
     "DeleteUserRequestRequestTypeDef",
@@ -670,60 +672,55 @@
         "Channel": ChannelType,
         "InitiationMethod": ContactInitiationMethodType,
         "AgentContactState": ContactStateType,
         "StateStartTimestamp": datetime,
         "ConnectedToAgentTimestamp": datetime,
         "Queue": "QueueReferenceTypeDef",
     },
-    total=False,
 )
 
 AgentInfoTypeDef = TypedDict(
     "AgentInfoTypeDef",
     {
         "Id": str,
         "ConnectedToAgentTimestamp": datetime,
     },
-    total=False,
 )
 
 AgentStatusReferenceTypeDef = TypedDict(
     "AgentStatusReferenceTypeDef",
     {
         "StatusStartTimestamp": datetime,
         "StatusArn": str,
         "StatusName": str,
     },
-    total=False,
 )
 
 AgentStatusSummaryTypeDef = TypedDict(
     "AgentStatusSummaryTypeDef",
     {
         "Id": str,
         "Arn": str,
         "Name": str,
         "Type": AgentStatusTypeType,
     },
-    total=False,
 )
 
 AgentStatusTypeDef = TypedDict(
     "AgentStatusTypeDef",
     {
         "AgentStatusARN": str,
         "AgentStatusId": str,
         "Name": str,
         "Description": str,
         "Type": AgentStatusTypeType,
         "DisplayOrder": int,
         "State": AgentStatusStateType,
         "Tags": Dict[str, str],
     },
-    total=False,
 )
 
 AnswerMachineDetectionConfigTypeDef = TypedDict(
     "AnswerMachineDetectionConfigTypeDef",
     {
         "EnableAnswerMachineDetection": bool,
         "AwaitAnswerMachinePrompt": bool,
@@ -863,34 +860,31 @@
 AttachmentReferenceTypeDef = TypedDict(
     "AttachmentReferenceTypeDef",
     {
         "Name": str,
         "Value": str,
         "Status": ReferenceStatusType,
     },
-    total=False,
 )
 
 AttributeTypeDef = TypedDict(
     "AttributeTypeDef",
     {
         "AttributeType": InstanceAttributeTypeType,
         "Value": str,
     },
-    total=False,
 )
 
 AvailableNumberSummaryTypeDef = TypedDict(
     "AvailableNumberSummaryTypeDef",
     {
         "PhoneNumber": str,
         "PhoneNumberCountryCode": PhoneNumberCountryCodeType,
         "PhoneNumberType": PhoneNumberTypeType,
     },
-    total=False,
 )
 
 ChatMessageTypeDef = TypedDict(
     "ChatMessageTypeDef",
     {
         "ContentType": str,
         "Content": str,
@@ -953,15 +947,14 @@
         "PhoneNumberCountryCode": PhoneNumberCountryCodeType,
         "PhoneNumberType": PhoneNumberTypeType,
         "PhoneNumberDescription": str,
         "TargetArn": str,
         "Tags": Dict[str, str],
         "PhoneNumberStatus": "PhoneNumberStatusTypeDef",
     },
-    total=False,
 )
 
 ContactFilterTypeDef = TypedDict(
     "ContactFilterTypeDef",
     {
         "ContactStates": Sequence[ContactStateType],
     },
@@ -972,57 +965,53 @@
     "ContactFlowModuleSummaryTypeDef",
     {
         "Id": str,
         "Arn": str,
         "Name": str,
         "State": ContactFlowModuleStateType,
     },
-    total=False,
 )
 
 ContactFlowModuleTypeDef = TypedDict(
     "ContactFlowModuleTypeDef",
     {
         "Arn": str,
         "Id": str,
         "Name": str,
         "Content": str,
         "Description": str,
         "State": ContactFlowModuleStateType,
         "Status": ContactFlowModuleStatusType,
         "Tags": Dict[str, str],
     },
-    total=False,
 )
 
 ContactFlowSummaryTypeDef = TypedDict(
     "ContactFlowSummaryTypeDef",
     {
         "Id": str,
         "Arn": str,
         "Name": str,
         "ContactFlowType": ContactFlowTypeType,
         "ContactFlowState": ContactFlowStateType,
     },
-    total=False,
 )
 
 ContactFlowTypeDef = TypedDict(
     "ContactFlowTypeDef",
     {
         "Arn": str,
         "Id": str,
         "Name": str,
         "Type": ContactFlowTypeType,
         "State": ContactFlowStateType,
         "Description": str,
         "Content": str,
         "Tags": Dict[str, str],
     },
-    total=False,
 )
 
 ContactTypeDef = TypedDict(
     "ContactTypeDef",
     {
         "Arn": str,
         "Id": str,
@@ -1037,15 +1026,14 @@
         "InitiationTimestamp": datetime,
         "DisconnectTimestamp": datetime,
         "LastUpdateTimestamp": datetime,
         "ScheduledTimestamp": datetime,
         "RelatedContactId": str,
         "WisdomInfo": "WisdomInfoTypeDef",
     },
-    total=False,
 )
 
 ControlPlaneTagFilterTypeDef = TypedDict(
     "ControlPlaneTagFilterTypeDef",
     {
         "OrConditions": Sequence[Sequence["TagConditionTypeDef"]],
         "AndConditions": Sequence["TagConditionTypeDef"],
@@ -1753,15 +1741,14 @@
     "CredentialsTypeDef",
     {
         "AccessToken": str,
         "AccessTokenExpiration": datetime,
         "RefreshToken": str,
         "RefreshTokenExpiration": datetime,
     },
-    total=False,
 )
 
 CrossChannelBehaviorTypeDef = TypedDict(
     "CrossChannelBehaviorTypeDef",
     {
         "BehaviorType": BehaviorTypeType,
     },
@@ -1769,24 +1756,22 @@
 
 CurrentMetricDataTypeDef = TypedDict(
     "CurrentMetricDataTypeDef",
     {
         "Metric": "CurrentMetricTypeDef",
         "Value": float,
     },
-    total=False,
 )
 
 CurrentMetricResultTypeDef = TypedDict(
     "CurrentMetricResultTypeDef",
     {
         "Dimensions": "DimensionsTypeDef",
         "Collections": List["CurrentMetricDataTypeDef"],
     },
-    total=False,
 )
 
 CurrentMetricSortCriteriaTypeDef = TypedDict(
     "CurrentMetricSortCriteriaTypeDef",
     {
         "SortByMetric": CurrentMetricNameType,
         "SortOrder": SortOrderType,
@@ -1805,15 +1790,14 @@
 
 DateReferenceTypeDef = TypedDict(
     "DateReferenceTypeDef",
     {
         "Name": str,
         "Value": str,
     },
-    total=False,
 )
 
 DeactivateEvaluationFormRequestRequestTypeDef = TypedDict(
     "DeactivateEvaluationFormRequestRequestTypeDef",
     {
         "InstanceId": str,
         "EvaluationFormId": str,
@@ -1915,22 +1899,38 @@
     "DeletePromptRequestRequestTypeDef",
     {
         "InstanceId": str,
         "PromptId": str,
     },
 )
 
+DeleteQueueRequestRequestTypeDef = TypedDict(
+    "DeleteQueueRequestRequestTypeDef",
+    {
+        "InstanceId": str,
+        "QueueId": str,
+    },
+)
+
 DeleteQuickConnectRequestRequestTypeDef = TypedDict(
     "DeleteQuickConnectRequestRequestTypeDef",
     {
         "InstanceId": str,
         "QuickConnectId": str,
     },
 )
 
+DeleteRoutingProfileRequestRequestTypeDef = TypedDict(
+    "DeleteRoutingProfileRequestRequestTypeDef",
+    {
+        "InstanceId": str,
+        "RoutingProfileId": str,
+    },
+)
+
 DeleteRuleRequestRequestTypeDef = TypedDict(
     "DeleteRuleRequestRequestTypeDef",
     {
         "InstanceId": str,
         "RuleId": str,
     },
 )
@@ -2369,15 +2369,14 @@
 DimensionsTypeDef = TypedDict(
     "DimensionsTypeDef",
     {
         "Queue": "QueueReferenceTypeDef",
         "Channel": ChannelType,
         "RoutingProfile": "RoutingProfileReferenceTypeDef",
     },
-    total=False,
 )
 
 DisassociateApprovedOriginRequestRequestTypeDef = TypedDict(
     "DisassociateApprovedOriginRequestRequestTypeDef",
     {
         "InstanceId": str,
         "Origin": str,
@@ -2485,15 +2484,14 @@
 
 EmailReferenceTypeDef = TypedDict(
     "EmailReferenceTypeDef",
     {
         "Name": str,
         "Value": str,
     },
-    total=False,
 )
 
 EmptyResponseMetadataTypeDef = TypedDict(
     "EmptyResponseMetadataTypeDef",
     {
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -2510,15 +2508,14 @@
 EvaluationAnswerDataTypeDef = TypedDict(
     "EvaluationAnswerDataTypeDef",
     {
         "StringValue": str,
         "NumericValue": float,
         "NotApplicable": bool,
     },
-    total=False,
 )
 
 EvaluationAnswerInputTypeDef = TypedDict(
     "EvaluationAnswerInputTypeDef",
     {
         "Value": "EvaluationAnswerDataTypeDef",
     },
@@ -2527,43 +2524,29 @@
 
 EvaluationAnswerOutputTypeDef = TypedDict(
     "EvaluationAnswerOutputTypeDef",
     {
         "Value": "EvaluationAnswerDataTypeDef",
         "SystemSuggestedValue": "EvaluationAnswerDataTypeDef",
     },
-    total=False,
 )
 
-_RequiredEvaluationFormContentTypeDef = TypedDict(
-    "_RequiredEvaluationFormContentTypeDef",
+EvaluationFormContentTypeDef = TypedDict(
+    "EvaluationFormContentTypeDef",
     {
         "EvaluationFormVersion": int,
         "EvaluationFormId": str,
         "EvaluationFormArn": str,
         "Title": str,
-        "Items": List["EvaluationFormItemTypeDef"],
-    },
-)
-_OptionalEvaluationFormContentTypeDef = TypedDict(
-    "_OptionalEvaluationFormContentTypeDef",
-    {
         "Description": str,
+        "Items": List["EvaluationFormItemTypeDef"],
         "ScoringStrategy": "EvaluationFormScoringStrategyTypeDef",
     },
-    total=False,
 )
 
-
-class EvaluationFormContentTypeDef(
-    _RequiredEvaluationFormContentTypeDef, _OptionalEvaluationFormContentTypeDef
-):
-    pass
-
-
 EvaluationFormItemTypeDef = TypedDict(
     "EvaluationFormItemTypeDef",
     {
         "Section": Dict[str, Any],
         "Question": "EvaluationFormQuestionTypeDef",
     },
     total=False,
@@ -2765,75 +2748,51 @@
 class EvaluationFormSingleSelectQuestionPropertiesTypeDef(
     _RequiredEvaluationFormSingleSelectQuestionPropertiesTypeDef,
     _OptionalEvaluationFormSingleSelectQuestionPropertiesTypeDef,
 ):
     pass
 
 
-_RequiredEvaluationFormSummaryTypeDef = TypedDict(
-    "_RequiredEvaluationFormSummaryTypeDef",
+EvaluationFormSummaryTypeDef = TypedDict(
+    "EvaluationFormSummaryTypeDef",
     {
         "EvaluationFormId": str,
         "EvaluationFormArn": str,
         "Title": str,
         "CreatedTime": datetime,
         "CreatedBy": str,
         "LastModifiedTime": datetime,
         "LastModifiedBy": str,
-        "LatestVersion": int,
-    },
-)
-_OptionalEvaluationFormSummaryTypeDef = TypedDict(
-    "_OptionalEvaluationFormSummaryTypeDef",
-    {
         "LastActivatedTime": datetime,
         "LastActivatedBy": str,
+        "LatestVersion": int,
         "ActiveVersion": int,
     },
-    total=False,
 )
 
-
-class EvaluationFormSummaryTypeDef(
-    _RequiredEvaluationFormSummaryTypeDef, _OptionalEvaluationFormSummaryTypeDef
-):
-    pass
-
-
-_RequiredEvaluationFormTypeDef = TypedDict(
-    "_RequiredEvaluationFormTypeDef",
+EvaluationFormTypeDef = TypedDict(
+    "EvaluationFormTypeDef",
     {
         "EvaluationFormId": str,
         "EvaluationFormVersion": int,
         "Locked": bool,
         "EvaluationFormArn": str,
         "Title": str,
+        "Description": str,
         "Status": EvaluationFormVersionStatusType,
         "Items": List["EvaluationFormItemTypeDef"],
+        "ScoringStrategy": "EvaluationFormScoringStrategyTypeDef",
         "CreatedTime": datetime,
         "CreatedBy": str,
         "LastModifiedTime": datetime,
         "LastModifiedBy": str,
-    },
-)
-_OptionalEvaluationFormTypeDef = TypedDict(
-    "_OptionalEvaluationFormTypeDef",
-    {
-        "Description": str,
-        "ScoringStrategy": "EvaluationFormScoringStrategyTypeDef",
         "Tags": Dict[str, str],
     },
-    total=False,
 )
 
-
-class EvaluationFormTypeDef(_RequiredEvaluationFormTypeDef, _OptionalEvaluationFormTypeDef):
-    pass
-
-
 EvaluationFormVersionSummaryTypeDef = TypedDict(
     "EvaluationFormVersionSummaryTypeDef",
     {
         "EvaluationFormArn": str,
         "EvaluationFormId": str,
         "EvaluationFormVersion": int,
         "Locked": bool,
@@ -2841,110 +2800,71 @@
         "CreatedTime": datetime,
         "CreatedBy": str,
         "LastModifiedTime": datetime,
         "LastModifiedBy": str,
     },
 )
 
-_RequiredEvaluationMetadataTypeDef = TypedDict(
-    "_RequiredEvaluationMetadataTypeDef",
+EvaluationMetadataTypeDef = TypedDict(
+    "EvaluationMetadataTypeDef",
     {
         "ContactId": str,
         "EvaluatorArn": str,
-    },
-)
-_OptionalEvaluationMetadataTypeDef = TypedDict(
-    "_OptionalEvaluationMetadataTypeDef",
-    {
         "ContactAgentId": str,
         "Score": "EvaluationScoreTypeDef",
     },
-    total=False,
 )
 
-
-class EvaluationMetadataTypeDef(
-    _RequiredEvaluationMetadataTypeDef, _OptionalEvaluationMetadataTypeDef
-):
-    pass
-
-
 EvaluationNoteTypeDef = TypedDict(
     "EvaluationNoteTypeDef",
     {
         "Value": str,
     },
-    total=False,
 )
 
 EvaluationScoreTypeDef = TypedDict(
     "EvaluationScoreTypeDef",
     {
         "Percentage": float,
         "NotApplicable": bool,
         "AutomaticFail": bool,
     },
-    total=False,
 )
 
-_RequiredEvaluationSummaryTypeDef = TypedDict(
-    "_RequiredEvaluationSummaryTypeDef",
+EvaluationSummaryTypeDef = TypedDict(
+    "EvaluationSummaryTypeDef",
     {
         "EvaluationId": str,
         "EvaluationArn": str,
         "EvaluationFormTitle": str,
         "EvaluationFormId": str,
         "Status": EvaluationStatusType,
         "EvaluatorArn": str,
+        "Score": "EvaluationScoreTypeDef",
         "CreatedTime": datetime,
         "LastModifiedTime": datetime,
     },
 )
-_OptionalEvaluationSummaryTypeDef = TypedDict(
-    "_OptionalEvaluationSummaryTypeDef",
-    {
-        "Score": "EvaluationScoreTypeDef",
-    },
-    total=False,
-)
-
-
-class EvaluationSummaryTypeDef(
-    _RequiredEvaluationSummaryTypeDef, _OptionalEvaluationSummaryTypeDef
-):
-    pass
 
-
-_RequiredEvaluationTypeDef = TypedDict(
-    "_RequiredEvaluationTypeDef",
+EvaluationTypeDef = TypedDict(
+    "EvaluationTypeDef",
     {
         "EvaluationId": str,
         "EvaluationArn": str,
         "Metadata": "EvaluationMetadataTypeDef",
         "Answers": Dict[str, "EvaluationAnswerOutputTypeDef"],
         "Notes": Dict[str, "EvaluationNoteTypeDef"],
         "Status": EvaluationStatusType,
+        "Scores": Dict[str, "EvaluationScoreTypeDef"],
         "CreatedTime": datetime,
         "LastModifiedTime": datetime,
-    },
-)
-_OptionalEvaluationTypeDef = TypedDict(
-    "_OptionalEvaluationTypeDef",
-    {
-        "Scores": Dict[str, "EvaluationScoreTypeDef"],
         "Tags": Dict[str, str],
     },
-    total=False,
 )
 
-
-class EvaluationTypeDef(_RequiredEvaluationTypeDef, _OptionalEvaluationTypeDef):
-    pass
-
-
 EventBridgeActionDefinitionTypeDef = TypedDict(
     "EventBridgeActionDefinitionTypeDef",
     {
         "Name": str,
     },
 )
 
@@ -3258,48 +3178,44 @@
 
 HierarchyGroupSummaryReferenceTypeDef = TypedDict(
     "HierarchyGroupSummaryReferenceTypeDef",
     {
         "Id": str,
         "Arn": str,
     },
-    total=False,
 )
 
 HierarchyGroupSummaryTypeDef = TypedDict(
     "HierarchyGroupSummaryTypeDef",
     {
         "Id": str,
         "Arn": str,
         "Name": str,
     },
-    total=False,
 )
 
 HierarchyGroupTypeDef = TypedDict(
     "HierarchyGroupTypeDef",
     {
         "Id": str,
         "Arn": str,
         "Name": str,
         "LevelId": str,
         "HierarchyPath": "HierarchyPathTypeDef",
         "Tags": Dict[str, str],
     },
-    total=False,
 )
 
 HierarchyLevelTypeDef = TypedDict(
     "HierarchyLevelTypeDef",
     {
         "Id": str,
         "Arn": str,
         "Name": str,
     },
-    total=False,
 )
 
 HierarchyLevelUpdateTypeDef = TypedDict(
     "HierarchyLevelUpdateTypeDef",
     {
         "Name": str,
     },
@@ -3310,39 +3226,36 @@
     {
         "LevelOne": "HierarchyGroupSummaryReferenceTypeDef",
         "LevelTwo": "HierarchyGroupSummaryReferenceTypeDef",
         "LevelThree": "HierarchyGroupSummaryReferenceTypeDef",
         "LevelFour": "HierarchyGroupSummaryReferenceTypeDef",
         "LevelFive": "HierarchyGroupSummaryReferenceTypeDef",
     },
-    total=False,
 )
 
 HierarchyPathTypeDef = TypedDict(
     "HierarchyPathTypeDef",
     {
         "LevelOne": "HierarchyGroupSummaryTypeDef",
         "LevelTwo": "HierarchyGroupSummaryTypeDef",
         "LevelThree": "HierarchyGroupSummaryTypeDef",
         "LevelFour": "HierarchyGroupSummaryTypeDef",
         "LevelFive": "HierarchyGroupSummaryTypeDef",
     },
-    total=False,
 )
 
 HierarchyStructureTypeDef = TypedDict(
     "HierarchyStructureTypeDef",
     {
         "LevelOne": "HierarchyLevelTypeDef",
         "LevelTwo": "HierarchyLevelTypeDef",
         "LevelThree": "HierarchyLevelTypeDef",
         "LevelFour": "HierarchyLevelTypeDef",
         "LevelFive": "HierarchyLevelTypeDef",
     },
-    total=False,
 )
 
 HierarchyStructureUpdateTypeDef = TypedDict(
     "HierarchyStructureUpdateTypeDef",
     {
         "LevelOne": "HierarchyLevelUpdateTypeDef",
         "LevelTwo": "HierarchyLevelUpdateTypeDef",
@@ -3355,24 +3268,22 @@
 
 HistoricalMetricDataTypeDef = TypedDict(
     "HistoricalMetricDataTypeDef",
     {
         "Metric": "HistoricalMetricTypeDef",
         "Value": float,
     },
-    total=False,
 )
 
 HistoricalMetricResultTypeDef = TypedDict(
     "HistoricalMetricResultTypeDef",
     {
         "Dimensions": "DimensionsTypeDef",
         "Collections": List["HistoricalMetricDataTypeDef"],
     },
-    total=False,
 )
 
 HistoricalMetricTypeDef = TypedDict(
     "HistoricalMetricTypeDef",
     {
         "Name": HistoricalMetricNameType,
         "Threshold": "ThresholdTypeDef",
@@ -3412,15 +3323,14 @@
 HoursOfOperationSummaryTypeDef = TypedDict(
     "HoursOfOperationSummaryTypeDef",
     {
         "Id": str,
         "Arn": str,
         "Name": str,
     },
-    total=False,
 )
 
 HoursOfOperationTimeSliceTypeDef = TypedDict(
     "HoursOfOperationTimeSliceTypeDef",
     {
         "Hours": int,
         "Minutes": int,
@@ -3434,23 +3344,21 @@
         "HoursOfOperationArn": str,
         "Name": str,
         "Description": str,
         "TimeZone": str,
         "Config": List["HoursOfOperationConfigTypeDef"],
         "Tags": Dict[str, str],
     },
-    total=False,
 )
 
 InstanceStatusReasonTypeDef = TypedDict(
     "InstanceStatusReasonTypeDef",
     {
         "Message": str,
     },
-    total=False,
 )
 
 _RequiredInstanceStorageConfigTypeDef = TypedDict(
     "_RequiredInstanceStorageConfigTypeDef",
     {
         "StorageType": StorageTypeType,
     },
@@ -3484,15 +3392,14 @@
         "CreatedTime": datetime,
         "ServiceRole": str,
         "InstanceStatus": InstanceStatusType,
         "InboundCallsEnabled": bool,
         "OutboundCallsEnabled": bool,
         "InstanceAccessUrl": str,
     },
-    total=False,
 )
 
 InstanceTypeDef = TypedDict(
     "InstanceTypeDef",
     {
         "Id": str,
         "Arn": str,
@@ -3502,30 +3409,28 @@
         "ServiceRole": str,
         "InstanceStatus": InstanceStatusType,
         "StatusReason": "InstanceStatusReasonTypeDef",
         "InboundCallsEnabled": bool,
         "OutboundCallsEnabled": bool,
         "InstanceAccessUrl": str,
     },
-    total=False,
 )
 
 IntegrationAssociationSummaryTypeDef = TypedDict(
     "IntegrationAssociationSummaryTypeDef",
     {
         "IntegrationAssociationId": str,
         "IntegrationAssociationArn": str,
         "InstanceId": str,
         "IntegrationType": IntegrationTypeType,
         "IntegrationArn": str,
         "SourceApplicationUrl": str,
         "SourceApplicationName": str,
         "SourceType": SourceTypeType,
     },
-    total=False,
 )
 
 InvisibleFieldInfoTypeDef = TypedDict(
     "InvisibleFieldInfoTypeDef",
     {
         "Id": "TaskTemplateFieldIdentifierTypeDef",
     },
@@ -3557,15 +3462,14 @@
 
 LexBotConfigTypeDef = TypedDict(
     "LexBotConfigTypeDef",
     {
         "LexBot": "LexBotTypeDef",
         "LexV2Bot": "LexV2BotTypeDef",
     },
-    total=False,
 )
 
 LexBotTypeDef = TypedDict(
     "LexBotTypeDef",
     {
         "Name": str,
         "LexRegion": str,
@@ -4548,15 +4452,14 @@
         "PhoneNumberId": str,
         "PhoneNumberArn": str,
         "PhoneNumber": str,
         "PhoneNumberCountryCode": PhoneNumberCountryCodeType,
         "PhoneNumberType": PhoneNumberTypeType,
         "TargetArn": str,
     },
-    total=False,
 )
 
 ListPhoneNumbersV2RequestListPhoneNumbersV2PaginateTypeDef = TypedDict(
     "ListPhoneNumbersV2RequestListPhoneNumbersV2PaginateTypeDef",
     {
         "TargetArn": str,
         "PhoneNumberCountryCodes": Sequence[PhoneNumberCountryCodeType],
@@ -5422,15 +5325,14 @@
 
 MetricDataV2TypeDef = TypedDict(
     "MetricDataV2TypeDef",
     {
         "Metric": "MetricV2TypeDef",
         "Value": float,
     },
-    total=False,
 )
 
 MetricFilterV2TypeDef = TypedDict(
     "MetricFilterV2TypeDef",
     {
         "MetricFilterKey": str,
         "MetricFilterValues": Sequence[str],
@@ -5440,15 +5342,14 @@
 
 MetricResultV2TypeDef = TypedDict(
     "MetricResultV2TypeDef",
     {
         "Dimensions": Dict[str, str],
         "Collections": List["MetricDataV2TypeDef"],
     },
-    total=False,
 )
 
 MetricV2TypeDef = TypedDict(
     "MetricV2TypeDef",
     {
         "Name": str,
         "Threshold": Sequence["ThresholdV2TypeDef"],
@@ -5501,15 +5402,14 @@
 
 NumberReferenceTypeDef = TypedDict(
     "NumberReferenceTypeDef",
     {
         "Name": str,
         "Value": str,
     },
-    total=False,
 )
 
 NumericQuestionPropertyValueAutomationTypeDef = TypedDict(
     "NumericQuestionPropertyValueAutomationTypeDef",
     {
         "Label": NumericQuestionPropertyAutomationLabelType,
     },
@@ -5571,15 +5471,14 @@
 
 ParticipantTokenCredentialsTypeDef = TypedDict(
     "ParticipantTokenCredentialsTypeDef",
     {
         "ParticipantToken": str,
         "Expiry": str,
     },
-    total=False,
 )
 
 PersistentChatTypeDef = TypedDict(
     "PersistentChatTypeDef",
     {
         "RehydrationType": RehydrationTypeType,
         "SourceContactId": str,
@@ -5596,27 +5495,25 @@
 
 PhoneNumberStatusTypeDef = TypedDict(
     "PhoneNumberStatusTypeDef",
     {
         "Status": PhoneNumberWorkflowStatusType,
         "Message": str,
     },
-    total=False,
 )
 
 PhoneNumberSummaryTypeDef = TypedDict(
     "PhoneNumberSummaryTypeDef",
     {
         "Id": str,
         "Arn": str,
         "PhoneNumber": str,
         "PhoneNumberType": PhoneNumberTypeType,
         "PhoneNumberCountryCode": PhoneNumberCountryCodeType,
     },
-    total=False,
 )
 
 PromptSearchCriteriaTypeDef = TypedDict(
     "PromptSearchCriteriaTypeDef",
     {
         "OrConditions": Sequence[Dict[str, Any]],
         "AndConditions": Sequence[Dict[str, Any]],
@@ -5636,27 +5533,25 @@
 PromptSummaryTypeDef = TypedDict(
     "PromptSummaryTypeDef",
     {
         "Id": str,
         "Arn": str,
         "Name": str,
     },
-    total=False,
 )
 
 PromptTypeDef = TypedDict(
     "PromptTypeDef",
     {
         "PromptARN": str,
         "PromptId": str,
         "Name": str,
         "Description": str,
         "Tags": Dict[str, str],
     },
-    total=False,
 )
 
 PutUserStatusRequestRequestTypeDef = TypedDict(
     "PutUserStatusRequestRequestTypeDef",
     {
         "UserId": str,
         "InstanceId": str,
@@ -5666,15 +5561,14 @@
 
 QueueInfoTypeDef = TypedDict(
     "QueueInfoTypeDef",
     {
         "Id": str,
         "EnqueueTimestamp": datetime,
     },
-    total=False,
 )
 
 QueueQuickConnectConfigTypeDef = TypedDict(
     "QueueQuickConnectConfigTypeDef",
     {
         "QueueId": str,
         "ContactFlowId": str,
@@ -5683,15 +5577,14 @@
 
 QueueReferenceTypeDef = TypedDict(
     "QueueReferenceTypeDef",
     {
         "Id": str,
         "Arn": str,
     },
-    total=False,
 )
 
 QueueSearchCriteriaTypeDef = TypedDict(
     "QueueSearchCriteriaTypeDef",
     {
         "OrConditions": Sequence[Dict[str, Any]],
         "AndConditions": Sequence[Dict[str, Any]],
@@ -5713,15 +5606,14 @@
     "QueueSummaryTypeDef",
     {
         "Id": str,
         "Arn": str,
         "Name": str,
         "QueueType": QueueTypeType,
     },
-    total=False,
 )
 
 QueueTypeDef = TypedDict(
     "QueueTypeDef",
     {
         "Name": str,
         "QueueArn": str,
@@ -5729,15 +5621,14 @@
         "Description": str,
         "OutboundCallerConfig": "OutboundCallerConfigTypeDef",
         "HoursOfOperationId": str,
         "MaxContacts": int,
         "Status": QueueStatusType,
         "Tags": Dict[str, str],
     },
-    total=False,
 )
 
 _RequiredQuickConnectConfigTypeDef = TypedDict(
     "_RequiredQuickConnectConfigTypeDef",
     {
         "QuickConnectType": QuickConnectTypeType,
     },
@@ -5781,28 +5672,26 @@
     "QuickConnectSummaryTypeDef",
     {
         "Id": str,
         "Arn": str,
         "Name": str,
         "QuickConnectType": QuickConnectTypeType,
     },
-    total=False,
 )
 
 QuickConnectTypeDef = TypedDict(
     "QuickConnectTypeDef",
     {
         "QuickConnectARN": str,
         "QuickConnectId": str,
         "Name": str,
         "Description": str,
         "QuickConnectConfig": "QuickConnectConfigTypeDef",
         "Tags": Dict[str, str],
     },
-    total=False,
 )
 
 ReadOnlyFieldInfoTypeDef = TypedDict(
     "ReadOnlyFieldInfoTypeDef",
     {
         "Id": "TaskTemplateFieldIdentifierTypeDef",
     },
@@ -5815,15 +5704,14 @@
         "Url": "UrlReferenceTypeDef",
         "Attachment": "AttachmentReferenceTypeDef",
         "String": "StringReferenceTypeDef",
         "Number": "NumberReferenceTypeDef",
         "Date": "DateReferenceTypeDef",
         "Email": "EmailReferenceTypeDef",
     },
-    total=False,
 )
 
 ReferenceTypeDef = TypedDict(
     "ReferenceTypeDef",
     {
         "Value": str,
         "Type": ReferenceTypeType,
@@ -5951,15 +5839,14 @@
 
 RoutingProfileReferenceTypeDef = TypedDict(
     "RoutingProfileReferenceTypeDef",
     {
         "Id": str,
         "Arn": str,
     },
-    total=False,
 )
 
 RoutingProfileSearchCriteriaTypeDef = TypedDict(
     "RoutingProfileSearchCriteriaTypeDef",
     {
         "OrConditions": Sequence[Dict[str, Any]],
         "AndConditions": Sequence[Dict[str, Any]],
@@ -5979,15 +5866,14 @@
 RoutingProfileSummaryTypeDef = TypedDict(
     "RoutingProfileSummaryTypeDef",
     {
         "Id": str,
         "Arn": str,
         "Name": str,
     },
-    total=False,
 )
 
 RoutingProfileTypeDef = TypedDict(
     "RoutingProfileTypeDef",
     {
         "InstanceId": str,
         "Name": str,
@@ -5996,15 +5882,14 @@
         "Description": str,
         "MediaConcurrencies": List["MediaConcurrencyTypeDef"],
         "DefaultOutboundQueueId": str,
         "Tags": Dict[str, str],
         "NumberOfAssociatedQueues": int,
         "NumberOfAssociatedUsers": int,
     },
-    total=False,
 )
 
 _RequiredRuleActionTypeDef = TypedDict(
     "_RequiredRuleActionTypeDef",
     {
         "ActionType": ActionTypeType,
     },
@@ -6056,42 +5941,31 @@
 
 class RuleTriggerEventSourceTypeDef(
     _RequiredRuleTriggerEventSourceTypeDef, _OptionalRuleTriggerEventSourceTypeDef
 ):
     pass
 
 
-_RequiredRuleTypeDef = TypedDict(
-    "_RequiredRuleTypeDef",
+RuleTypeDef = TypedDict(
+    "RuleTypeDef",
     {
         "Name": str,
         "RuleId": str,
         "RuleArn": str,
         "TriggerEventSource": "RuleTriggerEventSourceTypeDef",
         "Function": str,
         "Actions": List["RuleActionTypeDef"],
         "PublishStatus": RulePublishStatusType,
         "CreatedTime": datetime,
         "LastUpdatedTime": datetime,
         "LastUpdatedBy": str,
-    },
-)
-_OptionalRuleTypeDef = TypedDict(
-    "_OptionalRuleTypeDef",
-    {
         "Tags": Dict[str, str],
     },
-    total=False,
 )
 
-
-class RuleTypeDef(_RequiredRuleTypeDef, _OptionalRuleTypeDef):
-    pass
-
-
 _RequiredS3ConfigTypeDef = TypedDict(
     "_RequiredS3ConfigTypeDef",
     {
         "BucketName": str,
         "BucketPrefix": str,
     },
 )
@@ -6674,15 +6548,14 @@
 SecurityKeyTypeDef = TypedDict(
     "SecurityKeyTypeDef",
     {
         "AssociationId": str,
         "Key": str,
         "CreationTime": datetime,
     },
-    total=False,
 )
 
 SecurityProfileSearchCriteriaTypeDef = TypedDict(
     "SecurityProfileSearchCriteriaTypeDef",
     {
         "OrConditions": Sequence[Dict[str, Any]],
         "AndConditions": Sequence[Dict[str, Any]],
@@ -6697,40 +6570,37 @@
         "Id": str,
         "OrganizationResourceId": str,
         "Arn": str,
         "SecurityProfileName": str,
         "Description": str,
         "Tags": Dict[str, str],
     },
-    total=False,
 )
 
 SecurityProfileSummaryTypeDef = TypedDict(
     "SecurityProfileSummaryTypeDef",
     {
         "Id": str,
         "Arn": str,
         "Name": str,
     },
-    total=False,
 )
 
 SecurityProfileTypeDef = TypedDict(
     "SecurityProfileTypeDef",
     {
         "Id": str,
         "OrganizationResourceId": str,
         "Arn": str,
         "SecurityProfileName": str,
         "Description": str,
         "Tags": Dict[str, str],
         "AllowedAccessControlTags": Dict[str, str],
         "TagRestrictedResources": List[str],
     },
-    total=False,
 )
 
 SecurityProfilesSearchFilterTypeDef = TypedDict(
     "SecurityProfilesSearchFilterTypeDef",
     {
         "TagFilter": "ControlPlaneTagFilterTypeDef",
     },
@@ -6987,15 +6857,14 @@
 
 StringReferenceTypeDef = TypedDict(
     "StringReferenceTypeDef",
     {
         "Name": str,
         "Value": str,
     },
-    total=False,
 )
 
 _RequiredSubmitContactEvaluationRequestRequestTypeDef = TypedDict(
     "_RequiredSubmitContactEvaluationRequestRequestTypeDef",
     {
         "InstanceId": str,
         "EvaluationId": str,
@@ -7066,15 +6935,14 @@
 
 TagSetTypeDef = TypedDict(
     "TagSetTypeDef",
     {
         "key": str,
         "value": str,
     },
-    total=False,
 )
 
 _RequiredTaskActionDefinitionTypeDef = TypedDict(
     "_RequiredTaskActionDefinitionTypeDef",
     {
         "Name": str,
         "ContactFlowId": str,
@@ -7161,15 +7029,14 @@
         "Arn": str,
         "Name": str,
         "Description": str,
         "Status": TaskTemplateStatusType,
         "LastModifiedTime": datetime,
         "CreatedTime": datetime,
     },
-    total=False,
 )
 
 TelephonyConfigTypeDef = TypedDict(
     "TelephonyConfigTypeDef",
     {
         "Distributions": List["DistributionTypeDef"],
     },
@@ -7198,29 +7065,27 @@
     {
         "Id": str,
         "Arn": str,
         "Name": str,
         "InstanceArn": str,
         "Status": TrafficDistributionGroupStatusType,
     },
-    total=False,
 )
 
 TrafficDistributionGroupTypeDef = TypedDict(
     "TrafficDistributionGroupTypeDef",
     {
         "Id": str,
         "Arn": str,
         "Name": str,
         "Description": str,
         "InstanceArn": str,
         "Status": TrafficDistributionGroupStatusType,
         "Tags": Dict[str, str],
     },
-    total=False,
 )
 
 _RequiredTransferContactRequestRequestTypeDef = TypedDict(
     "_RequiredTransferContactRequestRequestTypeDef",
     {
         "InstanceId": str,
         "ContactId": str,
@@ -7962,25 +7827,23 @@
 
 UrlReferenceTypeDef = TypedDict(
     "UrlReferenceTypeDef",
     {
         "Name": str,
         "Value": str,
     },
-    total=False,
 )
 
 UseCaseTypeDef = TypedDict(
     "UseCaseTypeDef",
     {
         "UseCaseId": str,
         "UseCaseArn": str,
         "UseCaseType": UseCaseTypeType,
     },
-    total=False,
 )
 
 UserDataFiltersTypeDef = TypedDict(
     "UserDataFiltersTypeDef",
     {
         "Queues": Sequence[str],
         "ContactFilter": "ContactFilterTypeDef",
@@ -8000,24 +7863,22 @@
         "Status": "AgentStatusReferenceTypeDef",
         "AvailableSlotsByChannel": Dict[ChannelType, int],
         "MaxSlotsByChannel": Dict[ChannelType, int],
         "ActiveSlotsByChannel": Dict[ChannelType, int],
         "Contacts": List["AgentContactReferenceTypeDef"],
         "NextStatus": str,
     },
-    total=False,
 )
 
 UserIdentityInfoLiteTypeDef = TypedDict(
     "UserIdentityInfoLiteTypeDef",
     {
         "FirstName": str,
         "LastName": str,
     },
-    total=False,
 )
 
 UserIdentityInfoTypeDef = TypedDict(
     "UserIdentityInfoTypeDef",
     {
         "FirstName": str,
         "LastName": str,
@@ -8059,15 +7920,14 @@
 
 UserReferenceTypeDef = TypedDict(
     "UserReferenceTypeDef",
     {
         "Id": str,
         "Arn": str,
     },
-    total=False,
 )
 
 UserSearchCriteriaTypeDef = TypedDict(
     "UserSearchCriteriaTypeDef",
     {
         "OrConditions": Sequence[Dict[str, Any]],
         "AndConditions": Sequence[Dict[str, Any]],
@@ -8095,25 +7955,23 @@
         "IdentityInfo": "UserIdentityInfoLiteTypeDef",
         "PhoneConfig": "UserPhoneConfigTypeDef",
         "RoutingProfileId": str,
         "SecurityProfileIds": List[str],
         "Tags": Dict[str, str],
         "Username": str,
     },
-    total=False,
 )
 
 UserSummaryTypeDef = TypedDict(
     "UserSummaryTypeDef",
     {
         "Id": str,
         "Arn": str,
         "Username": str,
     },
-    total=False,
 )
 
 UserTypeDef = TypedDict(
     "UserTypeDef",
     {
         "Id": str,
         "Arn": str,
@@ -8122,77 +7980,51 @@
         "PhoneConfig": "UserPhoneConfigTypeDef",
         "DirectoryUserId": str,
         "SecurityProfileIds": List[str],
         "RoutingProfileId": str,
         "HierarchyGroupId": str,
         "Tags": Dict[str, str],
     },
-    total=False,
 )
 
-_RequiredVocabularySummaryTypeDef = TypedDict(
-    "_RequiredVocabularySummaryTypeDef",
+VocabularySummaryTypeDef = TypedDict(
+    "VocabularySummaryTypeDef",
     {
         "Name": str,
         "Id": str,
         "Arn": str,
         "LanguageCode": VocabularyLanguageCodeType,
         "State": VocabularyStateType,
         "LastModifiedTime": datetime,
-    },
-)
-_OptionalVocabularySummaryTypeDef = TypedDict(
-    "_OptionalVocabularySummaryTypeDef",
-    {
         "FailureReason": str,
     },
-    total=False,
 )
 
-
-class VocabularySummaryTypeDef(
-    _RequiredVocabularySummaryTypeDef, _OptionalVocabularySummaryTypeDef
-):
-    pass
-
-
-_RequiredVocabularyTypeDef = TypedDict(
-    "_RequiredVocabularyTypeDef",
+VocabularyTypeDef = TypedDict(
+    "VocabularyTypeDef",
     {
         "Name": str,
         "Id": str,
         "Arn": str,
         "LanguageCode": VocabularyLanguageCodeType,
         "State": VocabularyStateType,
         "LastModifiedTime": datetime,
-    },
-)
-_OptionalVocabularyTypeDef = TypedDict(
-    "_OptionalVocabularyTypeDef",
-    {
         "FailureReason": str,
         "Content": str,
         "Tags": Dict[str, str],
     },
-    total=False,
 )
 
-
-class VocabularyTypeDef(_RequiredVocabularyTypeDef, _OptionalVocabularyTypeDef):
-    pass
-
-
 VoiceRecordingConfigurationTypeDef = TypedDict(
     "VoiceRecordingConfigurationTypeDef",
     {
         "VoiceRecordingTrack": VoiceRecordingTrackType,
     },
     total=False,
 )
 
 WisdomInfoTypeDef = TypedDict(
     "WisdomInfoTypeDef",
     {
         "SessionArn": str,
     },
-    total=False,
 )
```

### Comparing `mypy-boto3-connect-1.28.0/mypy_boto3_connect/type_defs.pyi` & `mypy-boto3-connect-1.28.3/mypy_boto3_connect/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -179,15 +179,17 @@
     "DeleteContactFlowModuleRequestRequestTypeDef",
     "DeleteContactFlowRequestRequestTypeDef",
     "DeleteEvaluationFormRequestRequestTypeDef",
     "DeleteHoursOfOperationRequestRequestTypeDef",
     "DeleteInstanceRequestRequestTypeDef",
     "DeleteIntegrationAssociationRequestRequestTypeDef",
     "DeletePromptRequestRequestTypeDef",
+    "DeleteQueueRequestRequestTypeDef",
     "DeleteQuickConnectRequestRequestTypeDef",
+    "DeleteRoutingProfileRequestRequestTypeDef",
     "DeleteRuleRequestRequestTypeDef",
     "DeleteSecurityProfileRequestRequestTypeDef",
     "DeleteTaskTemplateRequestRequestTypeDef",
     "DeleteTrafficDistributionGroupRequestRequestTypeDef",
     "DeleteUseCaseRequestRequestTypeDef",
     "DeleteUserHierarchyGroupRequestRequestTypeDef",
     "DeleteUserRequestRequestTypeDef",
@@ -669,60 +671,55 @@
         "Channel": ChannelType,
         "InitiationMethod": ContactInitiationMethodType,
         "AgentContactState": ContactStateType,
         "StateStartTimestamp": datetime,
         "ConnectedToAgentTimestamp": datetime,
         "Queue": "QueueReferenceTypeDef",
     },
-    total=False,
 )
 
 AgentInfoTypeDef = TypedDict(
     "AgentInfoTypeDef",
     {
         "Id": str,
         "ConnectedToAgentTimestamp": datetime,
     },
-    total=False,
 )
 
 AgentStatusReferenceTypeDef = TypedDict(
     "AgentStatusReferenceTypeDef",
     {
         "StatusStartTimestamp": datetime,
         "StatusArn": str,
         "StatusName": str,
     },
-    total=False,
 )
 
 AgentStatusSummaryTypeDef = TypedDict(
     "AgentStatusSummaryTypeDef",
     {
         "Id": str,
         "Arn": str,
         "Name": str,
         "Type": AgentStatusTypeType,
     },
-    total=False,
 )
 
 AgentStatusTypeDef = TypedDict(
     "AgentStatusTypeDef",
     {
         "AgentStatusARN": str,
         "AgentStatusId": str,
         "Name": str,
         "Description": str,
         "Type": AgentStatusTypeType,
         "DisplayOrder": int,
         "State": AgentStatusStateType,
         "Tags": Dict[str, str],
     },
-    total=False,
 )
 
 AnswerMachineDetectionConfigTypeDef = TypedDict(
     "AnswerMachineDetectionConfigTypeDef",
     {
         "EnableAnswerMachineDetection": bool,
         "AwaitAnswerMachinePrompt": bool,
@@ -858,34 +855,31 @@
 AttachmentReferenceTypeDef = TypedDict(
     "AttachmentReferenceTypeDef",
     {
         "Name": str,
         "Value": str,
         "Status": ReferenceStatusType,
     },
-    total=False,
 )
 
 AttributeTypeDef = TypedDict(
     "AttributeTypeDef",
     {
         "AttributeType": InstanceAttributeTypeType,
         "Value": str,
     },
-    total=False,
 )
 
 AvailableNumberSummaryTypeDef = TypedDict(
     "AvailableNumberSummaryTypeDef",
     {
         "PhoneNumber": str,
         "PhoneNumberCountryCode": PhoneNumberCountryCodeType,
         "PhoneNumberType": PhoneNumberTypeType,
     },
-    total=False,
 )
 
 ChatMessageTypeDef = TypedDict(
     "ChatMessageTypeDef",
     {
         "ContentType": str,
         "Content": str,
@@ -946,15 +940,14 @@
         "PhoneNumberCountryCode": PhoneNumberCountryCodeType,
         "PhoneNumberType": PhoneNumberTypeType,
         "PhoneNumberDescription": str,
         "TargetArn": str,
         "Tags": Dict[str, str],
         "PhoneNumberStatus": "PhoneNumberStatusTypeDef",
     },
-    total=False,
 )
 
 ContactFilterTypeDef = TypedDict(
     "ContactFilterTypeDef",
     {
         "ContactStates": Sequence[ContactStateType],
     },
@@ -965,57 +958,53 @@
     "ContactFlowModuleSummaryTypeDef",
     {
         "Id": str,
         "Arn": str,
         "Name": str,
         "State": ContactFlowModuleStateType,
     },
-    total=False,
 )
 
 ContactFlowModuleTypeDef = TypedDict(
     "ContactFlowModuleTypeDef",
     {
         "Arn": str,
         "Id": str,
         "Name": str,
         "Content": str,
         "Description": str,
         "State": ContactFlowModuleStateType,
         "Status": ContactFlowModuleStatusType,
         "Tags": Dict[str, str],
     },
-    total=False,
 )
 
 ContactFlowSummaryTypeDef = TypedDict(
     "ContactFlowSummaryTypeDef",
     {
         "Id": str,
         "Arn": str,
         "Name": str,
         "ContactFlowType": ContactFlowTypeType,
         "ContactFlowState": ContactFlowStateType,
     },
-    total=False,
 )
 
 ContactFlowTypeDef = TypedDict(
     "ContactFlowTypeDef",
     {
         "Arn": str,
         "Id": str,
         "Name": str,
         "Type": ContactFlowTypeType,
         "State": ContactFlowStateType,
         "Description": str,
         "Content": str,
         "Tags": Dict[str, str],
     },
-    total=False,
 )
 
 ContactTypeDef = TypedDict(
     "ContactTypeDef",
     {
         "Arn": str,
         "Id": str,
@@ -1030,15 +1019,14 @@
         "InitiationTimestamp": datetime,
         "DisconnectTimestamp": datetime,
         "LastUpdateTimestamp": datetime,
         "ScheduledTimestamp": datetime,
         "RelatedContactId": str,
         "WisdomInfo": "WisdomInfoTypeDef",
     },
-    total=False,
 )
 
 ControlPlaneTagFilterTypeDef = TypedDict(
     "ControlPlaneTagFilterTypeDef",
     {
         "OrConditions": Sequence[Sequence["TagConditionTypeDef"]],
         "AndConditions": Sequence["TagConditionTypeDef"],
@@ -1706,15 +1694,14 @@
     "CredentialsTypeDef",
     {
         "AccessToken": str,
         "AccessTokenExpiration": datetime,
         "RefreshToken": str,
         "RefreshTokenExpiration": datetime,
     },
-    total=False,
 )
 
 CrossChannelBehaviorTypeDef = TypedDict(
     "CrossChannelBehaviorTypeDef",
     {
         "BehaviorType": BehaviorTypeType,
     },
@@ -1722,24 +1709,22 @@
 
 CurrentMetricDataTypeDef = TypedDict(
     "CurrentMetricDataTypeDef",
     {
         "Metric": "CurrentMetricTypeDef",
         "Value": float,
     },
-    total=False,
 )
 
 CurrentMetricResultTypeDef = TypedDict(
     "CurrentMetricResultTypeDef",
     {
         "Dimensions": "DimensionsTypeDef",
         "Collections": List["CurrentMetricDataTypeDef"],
     },
-    total=False,
 )
 
 CurrentMetricSortCriteriaTypeDef = TypedDict(
     "CurrentMetricSortCriteriaTypeDef",
     {
         "SortByMetric": CurrentMetricNameType,
         "SortOrder": SortOrderType,
@@ -1758,15 +1743,14 @@
 
 DateReferenceTypeDef = TypedDict(
     "DateReferenceTypeDef",
     {
         "Name": str,
         "Value": str,
     },
-    total=False,
 )
 
 DeactivateEvaluationFormRequestRequestTypeDef = TypedDict(
     "DeactivateEvaluationFormRequestRequestTypeDef",
     {
         "InstanceId": str,
         "EvaluationFormId": str,
@@ -1866,22 +1850,38 @@
     "DeletePromptRequestRequestTypeDef",
     {
         "InstanceId": str,
         "PromptId": str,
     },
 )
 
+DeleteQueueRequestRequestTypeDef = TypedDict(
+    "DeleteQueueRequestRequestTypeDef",
+    {
+        "InstanceId": str,
+        "QueueId": str,
+    },
+)
+
 DeleteQuickConnectRequestRequestTypeDef = TypedDict(
     "DeleteQuickConnectRequestRequestTypeDef",
     {
         "InstanceId": str,
         "QuickConnectId": str,
     },
 )
 
+DeleteRoutingProfileRequestRequestTypeDef = TypedDict(
+    "DeleteRoutingProfileRequestRequestTypeDef",
+    {
+        "InstanceId": str,
+        "RoutingProfileId": str,
+    },
+)
+
 DeleteRuleRequestRequestTypeDef = TypedDict(
     "DeleteRuleRequestRequestTypeDef",
     {
         "InstanceId": str,
         "RuleId": str,
     },
 )
@@ -2318,15 +2318,14 @@
 DimensionsTypeDef = TypedDict(
     "DimensionsTypeDef",
     {
         "Queue": "QueueReferenceTypeDef",
         "Channel": ChannelType,
         "RoutingProfile": "RoutingProfileReferenceTypeDef",
     },
-    total=False,
 )
 
 DisassociateApprovedOriginRequestRequestTypeDef = TypedDict(
     "DisassociateApprovedOriginRequestRequestTypeDef",
     {
         "InstanceId": str,
         "Origin": str,
@@ -2432,15 +2431,14 @@
 
 EmailReferenceTypeDef = TypedDict(
     "EmailReferenceTypeDef",
     {
         "Name": str,
         "Value": str,
     },
-    total=False,
 )
 
 EmptyResponseMetadataTypeDef = TypedDict(
     "EmptyResponseMetadataTypeDef",
     {
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -2457,15 +2455,14 @@
 EvaluationAnswerDataTypeDef = TypedDict(
     "EvaluationAnswerDataTypeDef",
     {
         "StringValue": str,
         "NumericValue": float,
         "NotApplicable": bool,
     },
-    total=False,
 )
 
 EvaluationAnswerInputTypeDef = TypedDict(
     "EvaluationAnswerInputTypeDef",
     {
         "Value": "EvaluationAnswerDataTypeDef",
     },
@@ -2474,41 +2471,29 @@
 
 EvaluationAnswerOutputTypeDef = TypedDict(
     "EvaluationAnswerOutputTypeDef",
     {
         "Value": "EvaluationAnswerDataTypeDef",
         "SystemSuggestedValue": "EvaluationAnswerDataTypeDef",
     },
-    total=False,
 )
 
-_RequiredEvaluationFormContentTypeDef = TypedDict(
-    "_RequiredEvaluationFormContentTypeDef",
+EvaluationFormContentTypeDef = TypedDict(
+    "EvaluationFormContentTypeDef",
     {
         "EvaluationFormVersion": int,
         "EvaluationFormId": str,
         "EvaluationFormArn": str,
         "Title": str,
-        "Items": List["EvaluationFormItemTypeDef"],
-    },
-)
-_OptionalEvaluationFormContentTypeDef = TypedDict(
-    "_OptionalEvaluationFormContentTypeDef",
-    {
         "Description": str,
+        "Items": List["EvaluationFormItemTypeDef"],
         "ScoringStrategy": "EvaluationFormScoringStrategyTypeDef",
     },
-    total=False,
 )
 
-class EvaluationFormContentTypeDef(
-    _RequiredEvaluationFormContentTypeDef, _OptionalEvaluationFormContentTypeDef
-):
-    pass
-
 EvaluationFormItemTypeDef = TypedDict(
     "EvaluationFormItemTypeDef",
     {
         "Section": Dict[str, Any],
         "Question": "EvaluationFormQuestionTypeDef",
     },
     total=False,
@@ -2696,71 +2681,51 @@
 
 class EvaluationFormSingleSelectQuestionPropertiesTypeDef(
     _RequiredEvaluationFormSingleSelectQuestionPropertiesTypeDef,
     _OptionalEvaluationFormSingleSelectQuestionPropertiesTypeDef,
 ):
     pass
 
-_RequiredEvaluationFormSummaryTypeDef = TypedDict(
-    "_RequiredEvaluationFormSummaryTypeDef",
+EvaluationFormSummaryTypeDef = TypedDict(
+    "EvaluationFormSummaryTypeDef",
     {
         "EvaluationFormId": str,
         "EvaluationFormArn": str,
         "Title": str,
         "CreatedTime": datetime,
         "CreatedBy": str,
         "LastModifiedTime": datetime,
         "LastModifiedBy": str,
-        "LatestVersion": int,
-    },
-)
-_OptionalEvaluationFormSummaryTypeDef = TypedDict(
-    "_OptionalEvaluationFormSummaryTypeDef",
-    {
         "LastActivatedTime": datetime,
         "LastActivatedBy": str,
+        "LatestVersion": int,
         "ActiveVersion": int,
     },
-    total=False,
 )
 
-class EvaluationFormSummaryTypeDef(
-    _RequiredEvaluationFormSummaryTypeDef, _OptionalEvaluationFormSummaryTypeDef
-):
-    pass
-
-_RequiredEvaluationFormTypeDef = TypedDict(
-    "_RequiredEvaluationFormTypeDef",
+EvaluationFormTypeDef = TypedDict(
+    "EvaluationFormTypeDef",
     {
         "EvaluationFormId": str,
         "EvaluationFormVersion": int,
         "Locked": bool,
         "EvaluationFormArn": str,
         "Title": str,
+        "Description": str,
         "Status": EvaluationFormVersionStatusType,
         "Items": List["EvaluationFormItemTypeDef"],
+        "ScoringStrategy": "EvaluationFormScoringStrategyTypeDef",
         "CreatedTime": datetime,
         "CreatedBy": str,
         "LastModifiedTime": datetime,
         "LastModifiedBy": str,
-    },
-)
-_OptionalEvaluationFormTypeDef = TypedDict(
-    "_OptionalEvaluationFormTypeDef",
-    {
-        "Description": str,
-        "ScoringStrategy": "EvaluationFormScoringStrategyTypeDef",
         "Tags": Dict[str, str],
     },
-    total=False,
 )
 
-class EvaluationFormTypeDef(_RequiredEvaluationFormTypeDef, _OptionalEvaluationFormTypeDef):
-    pass
-
 EvaluationFormVersionSummaryTypeDef = TypedDict(
     "EvaluationFormVersionSummaryTypeDef",
     {
         "EvaluationFormArn": str,
         "EvaluationFormId": str,
         "EvaluationFormVersion": int,
         "Locked": bool,
@@ -2768,104 +2733,71 @@
         "CreatedTime": datetime,
         "CreatedBy": str,
         "LastModifiedTime": datetime,
         "LastModifiedBy": str,
     },
 )
 
-_RequiredEvaluationMetadataTypeDef = TypedDict(
-    "_RequiredEvaluationMetadataTypeDef",
+EvaluationMetadataTypeDef = TypedDict(
+    "EvaluationMetadataTypeDef",
     {
         "ContactId": str,
         "EvaluatorArn": str,
-    },
-)
-_OptionalEvaluationMetadataTypeDef = TypedDict(
-    "_OptionalEvaluationMetadataTypeDef",
-    {
         "ContactAgentId": str,
         "Score": "EvaluationScoreTypeDef",
     },
-    total=False,
 )
 
-class EvaluationMetadataTypeDef(
-    _RequiredEvaluationMetadataTypeDef, _OptionalEvaluationMetadataTypeDef
-):
-    pass
-
 EvaluationNoteTypeDef = TypedDict(
     "EvaluationNoteTypeDef",
     {
         "Value": str,
     },
-    total=False,
 )
 
 EvaluationScoreTypeDef = TypedDict(
     "EvaluationScoreTypeDef",
     {
         "Percentage": float,
         "NotApplicable": bool,
         "AutomaticFail": bool,
     },
-    total=False,
 )
 
-_RequiredEvaluationSummaryTypeDef = TypedDict(
-    "_RequiredEvaluationSummaryTypeDef",
+EvaluationSummaryTypeDef = TypedDict(
+    "EvaluationSummaryTypeDef",
     {
         "EvaluationId": str,
         "EvaluationArn": str,
         "EvaluationFormTitle": str,
         "EvaluationFormId": str,
         "Status": EvaluationStatusType,
         "EvaluatorArn": str,
+        "Score": "EvaluationScoreTypeDef",
         "CreatedTime": datetime,
         "LastModifiedTime": datetime,
     },
 )
-_OptionalEvaluationSummaryTypeDef = TypedDict(
-    "_OptionalEvaluationSummaryTypeDef",
-    {
-        "Score": "EvaluationScoreTypeDef",
-    },
-    total=False,
-)
-
-class EvaluationSummaryTypeDef(
-    _RequiredEvaluationSummaryTypeDef, _OptionalEvaluationSummaryTypeDef
-):
-    pass
 
-_RequiredEvaluationTypeDef = TypedDict(
-    "_RequiredEvaluationTypeDef",
+EvaluationTypeDef = TypedDict(
+    "EvaluationTypeDef",
     {
         "EvaluationId": str,
         "EvaluationArn": str,
         "Metadata": "EvaluationMetadataTypeDef",
         "Answers": Dict[str, "EvaluationAnswerOutputTypeDef"],
         "Notes": Dict[str, "EvaluationNoteTypeDef"],
         "Status": EvaluationStatusType,
+        "Scores": Dict[str, "EvaluationScoreTypeDef"],
         "CreatedTime": datetime,
         "LastModifiedTime": datetime,
-    },
-)
-_OptionalEvaluationTypeDef = TypedDict(
-    "_OptionalEvaluationTypeDef",
-    {
-        "Scores": Dict[str, "EvaluationScoreTypeDef"],
         "Tags": Dict[str, str],
     },
-    total=False,
 )
 
-class EvaluationTypeDef(_RequiredEvaluationTypeDef, _OptionalEvaluationTypeDef):
-    pass
-
 EventBridgeActionDefinitionTypeDef = TypedDict(
     "EventBridgeActionDefinitionTypeDef",
     {
         "Name": str,
     },
 )
 
@@ -3167,48 +3099,44 @@
 
 HierarchyGroupSummaryReferenceTypeDef = TypedDict(
     "HierarchyGroupSummaryReferenceTypeDef",
     {
         "Id": str,
         "Arn": str,
     },
-    total=False,
 )
 
 HierarchyGroupSummaryTypeDef = TypedDict(
     "HierarchyGroupSummaryTypeDef",
     {
         "Id": str,
         "Arn": str,
         "Name": str,
     },
-    total=False,
 )
 
 HierarchyGroupTypeDef = TypedDict(
     "HierarchyGroupTypeDef",
     {
         "Id": str,
         "Arn": str,
         "Name": str,
         "LevelId": str,
         "HierarchyPath": "HierarchyPathTypeDef",
         "Tags": Dict[str, str],
     },
-    total=False,
 )
 
 HierarchyLevelTypeDef = TypedDict(
     "HierarchyLevelTypeDef",
     {
         "Id": str,
         "Arn": str,
         "Name": str,
     },
-    total=False,
 )
 
 HierarchyLevelUpdateTypeDef = TypedDict(
     "HierarchyLevelUpdateTypeDef",
     {
         "Name": str,
     },
@@ -3219,39 +3147,36 @@
     {
         "LevelOne": "HierarchyGroupSummaryReferenceTypeDef",
         "LevelTwo": "HierarchyGroupSummaryReferenceTypeDef",
         "LevelThree": "HierarchyGroupSummaryReferenceTypeDef",
         "LevelFour": "HierarchyGroupSummaryReferenceTypeDef",
         "LevelFive": "HierarchyGroupSummaryReferenceTypeDef",
     },
-    total=False,
 )
 
 HierarchyPathTypeDef = TypedDict(
     "HierarchyPathTypeDef",
     {
         "LevelOne": "HierarchyGroupSummaryTypeDef",
         "LevelTwo": "HierarchyGroupSummaryTypeDef",
         "LevelThree": "HierarchyGroupSummaryTypeDef",
         "LevelFour": "HierarchyGroupSummaryTypeDef",
         "LevelFive": "HierarchyGroupSummaryTypeDef",
     },
-    total=False,
 )
 
 HierarchyStructureTypeDef = TypedDict(
     "HierarchyStructureTypeDef",
     {
         "LevelOne": "HierarchyLevelTypeDef",
         "LevelTwo": "HierarchyLevelTypeDef",
         "LevelThree": "HierarchyLevelTypeDef",
         "LevelFour": "HierarchyLevelTypeDef",
         "LevelFive": "HierarchyLevelTypeDef",
     },
-    total=False,
 )
 
 HierarchyStructureUpdateTypeDef = TypedDict(
     "HierarchyStructureUpdateTypeDef",
     {
         "LevelOne": "HierarchyLevelUpdateTypeDef",
         "LevelTwo": "HierarchyLevelUpdateTypeDef",
@@ -3264,24 +3189,22 @@
 
 HistoricalMetricDataTypeDef = TypedDict(
     "HistoricalMetricDataTypeDef",
     {
         "Metric": "HistoricalMetricTypeDef",
         "Value": float,
     },
-    total=False,
 )
 
 HistoricalMetricResultTypeDef = TypedDict(
     "HistoricalMetricResultTypeDef",
     {
         "Dimensions": "DimensionsTypeDef",
         "Collections": List["HistoricalMetricDataTypeDef"],
     },
-    total=False,
 )
 
 HistoricalMetricTypeDef = TypedDict(
     "HistoricalMetricTypeDef",
     {
         "Name": HistoricalMetricNameType,
         "Threshold": "ThresholdTypeDef",
@@ -3321,15 +3244,14 @@
 HoursOfOperationSummaryTypeDef = TypedDict(
     "HoursOfOperationSummaryTypeDef",
     {
         "Id": str,
         "Arn": str,
         "Name": str,
     },
-    total=False,
 )
 
 HoursOfOperationTimeSliceTypeDef = TypedDict(
     "HoursOfOperationTimeSliceTypeDef",
     {
         "Hours": int,
         "Minutes": int,
@@ -3343,23 +3265,21 @@
         "HoursOfOperationArn": str,
         "Name": str,
         "Description": str,
         "TimeZone": str,
         "Config": List["HoursOfOperationConfigTypeDef"],
         "Tags": Dict[str, str],
     },
-    total=False,
 )
 
 InstanceStatusReasonTypeDef = TypedDict(
     "InstanceStatusReasonTypeDef",
     {
         "Message": str,
     },
-    total=False,
 )
 
 _RequiredInstanceStorageConfigTypeDef = TypedDict(
     "_RequiredInstanceStorageConfigTypeDef",
     {
         "StorageType": StorageTypeType,
     },
@@ -3391,15 +3311,14 @@
         "CreatedTime": datetime,
         "ServiceRole": str,
         "InstanceStatus": InstanceStatusType,
         "InboundCallsEnabled": bool,
         "OutboundCallsEnabled": bool,
         "InstanceAccessUrl": str,
     },
-    total=False,
 )
 
 InstanceTypeDef = TypedDict(
     "InstanceTypeDef",
     {
         "Id": str,
         "Arn": str,
@@ -3409,30 +3328,28 @@
         "ServiceRole": str,
         "InstanceStatus": InstanceStatusType,
         "StatusReason": "InstanceStatusReasonTypeDef",
         "InboundCallsEnabled": bool,
         "OutboundCallsEnabled": bool,
         "InstanceAccessUrl": str,
     },
-    total=False,
 )
 
 IntegrationAssociationSummaryTypeDef = TypedDict(
     "IntegrationAssociationSummaryTypeDef",
     {
         "IntegrationAssociationId": str,
         "IntegrationAssociationArn": str,
         "InstanceId": str,
         "IntegrationType": IntegrationTypeType,
         "IntegrationArn": str,
         "SourceApplicationUrl": str,
         "SourceApplicationName": str,
         "SourceType": SourceTypeType,
     },
-    total=False,
 )
 
 InvisibleFieldInfoTypeDef = TypedDict(
     "InvisibleFieldInfoTypeDef",
     {
         "Id": "TaskTemplateFieldIdentifierTypeDef",
     },
@@ -3464,15 +3381,14 @@
 
 LexBotConfigTypeDef = TypedDict(
     "LexBotConfigTypeDef",
     {
         "LexBot": "LexBotTypeDef",
         "LexV2Bot": "LexV2BotTypeDef",
     },
-    total=False,
 )
 
 LexBotTypeDef = TypedDict(
     "LexBotTypeDef",
     {
         "Name": str,
         "LexRegion": str,
@@ -4387,15 +4303,14 @@
         "PhoneNumberId": str,
         "PhoneNumberArn": str,
         "PhoneNumber": str,
         "PhoneNumberCountryCode": PhoneNumberCountryCodeType,
         "PhoneNumberType": PhoneNumberTypeType,
         "TargetArn": str,
     },
-    total=False,
 )
 
 ListPhoneNumbersV2RequestListPhoneNumbersV2PaginateTypeDef = TypedDict(
     "ListPhoneNumbersV2RequestListPhoneNumbersV2PaginateTypeDef",
     {
         "TargetArn": str,
         "PhoneNumberCountryCodes": Sequence[PhoneNumberCountryCodeType],
@@ -5203,15 +5118,14 @@
 
 MetricDataV2TypeDef = TypedDict(
     "MetricDataV2TypeDef",
     {
         "Metric": "MetricV2TypeDef",
         "Value": float,
     },
-    total=False,
 )
 
 MetricFilterV2TypeDef = TypedDict(
     "MetricFilterV2TypeDef",
     {
         "MetricFilterKey": str,
         "MetricFilterValues": Sequence[str],
@@ -5221,15 +5135,14 @@
 
 MetricResultV2TypeDef = TypedDict(
     "MetricResultV2TypeDef",
     {
         "Dimensions": Dict[str, str],
         "Collections": List["MetricDataV2TypeDef"],
     },
-    total=False,
 )
 
 MetricV2TypeDef = TypedDict(
     "MetricV2TypeDef",
     {
         "Name": str,
         "Threshold": Sequence["ThresholdV2TypeDef"],
@@ -5280,15 +5193,14 @@
 
 NumberReferenceTypeDef = TypedDict(
     "NumberReferenceTypeDef",
     {
         "Name": str,
         "Value": str,
     },
-    total=False,
 )
 
 NumericQuestionPropertyValueAutomationTypeDef = TypedDict(
     "NumericQuestionPropertyValueAutomationTypeDef",
     {
         "Label": NumericQuestionPropertyAutomationLabelType,
     },
@@ -5350,15 +5262,14 @@
 
 ParticipantTokenCredentialsTypeDef = TypedDict(
     "ParticipantTokenCredentialsTypeDef",
     {
         "ParticipantToken": str,
         "Expiry": str,
     },
-    total=False,
 )
 
 PersistentChatTypeDef = TypedDict(
     "PersistentChatTypeDef",
     {
         "RehydrationType": RehydrationTypeType,
         "SourceContactId": str,
@@ -5375,27 +5286,25 @@
 
 PhoneNumberStatusTypeDef = TypedDict(
     "PhoneNumberStatusTypeDef",
     {
         "Status": PhoneNumberWorkflowStatusType,
         "Message": str,
     },
-    total=False,
 )
 
 PhoneNumberSummaryTypeDef = TypedDict(
     "PhoneNumberSummaryTypeDef",
     {
         "Id": str,
         "Arn": str,
         "PhoneNumber": str,
         "PhoneNumberType": PhoneNumberTypeType,
         "PhoneNumberCountryCode": PhoneNumberCountryCodeType,
     },
-    total=False,
 )
 
 PromptSearchCriteriaTypeDef = TypedDict(
     "PromptSearchCriteriaTypeDef",
     {
         "OrConditions": Sequence[Dict[str, Any]],
         "AndConditions": Sequence[Dict[str, Any]],
@@ -5415,27 +5324,25 @@
 PromptSummaryTypeDef = TypedDict(
     "PromptSummaryTypeDef",
     {
         "Id": str,
         "Arn": str,
         "Name": str,
     },
-    total=False,
 )
 
 PromptTypeDef = TypedDict(
     "PromptTypeDef",
     {
         "PromptARN": str,
         "PromptId": str,
         "Name": str,
         "Description": str,
         "Tags": Dict[str, str],
     },
-    total=False,
 )
 
 PutUserStatusRequestRequestTypeDef = TypedDict(
     "PutUserStatusRequestRequestTypeDef",
     {
         "UserId": str,
         "InstanceId": str,
@@ -5445,15 +5352,14 @@
 
 QueueInfoTypeDef = TypedDict(
     "QueueInfoTypeDef",
     {
         "Id": str,
         "EnqueueTimestamp": datetime,
     },
-    total=False,
 )
 
 QueueQuickConnectConfigTypeDef = TypedDict(
     "QueueQuickConnectConfigTypeDef",
     {
         "QueueId": str,
         "ContactFlowId": str,
@@ -5462,15 +5368,14 @@
 
 QueueReferenceTypeDef = TypedDict(
     "QueueReferenceTypeDef",
     {
         "Id": str,
         "Arn": str,
     },
-    total=False,
 )
 
 QueueSearchCriteriaTypeDef = TypedDict(
     "QueueSearchCriteriaTypeDef",
     {
         "OrConditions": Sequence[Dict[str, Any]],
         "AndConditions": Sequence[Dict[str, Any]],
@@ -5492,15 +5397,14 @@
     "QueueSummaryTypeDef",
     {
         "Id": str,
         "Arn": str,
         "Name": str,
         "QueueType": QueueTypeType,
     },
-    total=False,
 )
 
 QueueTypeDef = TypedDict(
     "QueueTypeDef",
     {
         "Name": str,
         "QueueArn": str,
@@ -5508,15 +5412,14 @@
         "Description": str,
         "OutboundCallerConfig": "OutboundCallerConfigTypeDef",
         "HoursOfOperationId": str,
         "MaxContacts": int,
         "Status": QueueStatusType,
         "Tags": Dict[str, str],
     },
-    total=False,
 )
 
 _RequiredQuickConnectConfigTypeDef = TypedDict(
     "_RequiredQuickConnectConfigTypeDef",
     {
         "QuickConnectType": QuickConnectTypeType,
     },
@@ -5558,28 +5461,26 @@
     "QuickConnectSummaryTypeDef",
     {
         "Id": str,
         "Arn": str,
         "Name": str,
         "QuickConnectType": QuickConnectTypeType,
     },
-    total=False,
 )
 
 QuickConnectTypeDef = TypedDict(
     "QuickConnectTypeDef",
     {
         "QuickConnectARN": str,
         "QuickConnectId": str,
         "Name": str,
         "Description": str,
         "QuickConnectConfig": "QuickConnectConfigTypeDef",
         "Tags": Dict[str, str],
     },
-    total=False,
 )
 
 ReadOnlyFieldInfoTypeDef = TypedDict(
     "ReadOnlyFieldInfoTypeDef",
     {
         "Id": "TaskTemplateFieldIdentifierTypeDef",
     },
@@ -5592,15 +5493,14 @@
         "Url": "UrlReferenceTypeDef",
         "Attachment": "AttachmentReferenceTypeDef",
         "String": "StringReferenceTypeDef",
         "Number": "NumberReferenceTypeDef",
         "Date": "DateReferenceTypeDef",
         "Email": "EmailReferenceTypeDef",
     },
-    total=False,
 )
 
 ReferenceTypeDef = TypedDict(
     "ReferenceTypeDef",
     {
         "Value": str,
         "Type": ReferenceTypeType,
@@ -5724,15 +5624,14 @@
 
 RoutingProfileReferenceTypeDef = TypedDict(
     "RoutingProfileReferenceTypeDef",
     {
         "Id": str,
         "Arn": str,
     },
-    total=False,
 )
 
 RoutingProfileSearchCriteriaTypeDef = TypedDict(
     "RoutingProfileSearchCriteriaTypeDef",
     {
         "OrConditions": Sequence[Dict[str, Any]],
         "AndConditions": Sequence[Dict[str, Any]],
@@ -5752,15 +5651,14 @@
 RoutingProfileSummaryTypeDef = TypedDict(
     "RoutingProfileSummaryTypeDef",
     {
         "Id": str,
         "Arn": str,
         "Name": str,
     },
-    total=False,
 )
 
 RoutingProfileTypeDef = TypedDict(
     "RoutingProfileTypeDef",
     {
         "InstanceId": str,
         "Name": str,
@@ -5769,15 +5667,14 @@
         "Description": str,
         "MediaConcurrencies": List["MediaConcurrencyTypeDef"],
         "DefaultOutboundQueueId": str,
         "Tags": Dict[str, str],
         "NumberOfAssociatedQueues": int,
         "NumberOfAssociatedUsers": int,
     },
-    total=False,
 )
 
 _RequiredRuleActionTypeDef = TypedDict(
     "_RequiredRuleActionTypeDef",
     {
         "ActionType": ActionTypeType,
     },
@@ -5825,40 +5722,31 @@
 )
 
 class RuleTriggerEventSourceTypeDef(
     _RequiredRuleTriggerEventSourceTypeDef, _OptionalRuleTriggerEventSourceTypeDef
 ):
     pass
 
-_RequiredRuleTypeDef = TypedDict(
-    "_RequiredRuleTypeDef",
+RuleTypeDef = TypedDict(
+    "RuleTypeDef",
     {
         "Name": str,
         "RuleId": str,
         "RuleArn": str,
         "TriggerEventSource": "RuleTriggerEventSourceTypeDef",
         "Function": str,
         "Actions": List["RuleActionTypeDef"],
         "PublishStatus": RulePublishStatusType,
         "CreatedTime": datetime,
         "LastUpdatedTime": datetime,
         "LastUpdatedBy": str,
-    },
-)
-_OptionalRuleTypeDef = TypedDict(
-    "_OptionalRuleTypeDef",
-    {
         "Tags": Dict[str, str],
     },
-    total=False,
 )
 
-class RuleTypeDef(_RequiredRuleTypeDef, _OptionalRuleTypeDef):
-    pass
-
 _RequiredS3ConfigTypeDef = TypedDict(
     "_RequiredS3ConfigTypeDef",
     {
         "BucketName": str,
         "BucketPrefix": str,
     },
 )
@@ -6403,15 +6291,14 @@
 SecurityKeyTypeDef = TypedDict(
     "SecurityKeyTypeDef",
     {
         "AssociationId": str,
         "Key": str,
         "CreationTime": datetime,
     },
-    total=False,
 )
 
 SecurityProfileSearchCriteriaTypeDef = TypedDict(
     "SecurityProfileSearchCriteriaTypeDef",
     {
         "OrConditions": Sequence[Dict[str, Any]],
         "AndConditions": Sequence[Dict[str, Any]],
@@ -6426,40 +6313,37 @@
         "Id": str,
         "OrganizationResourceId": str,
         "Arn": str,
         "SecurityProfileName": str,
         "Description": str,
         "Tags": Dict[str, str],
     },
-    total=False,
 )
 
 SecurityProfileSummaryTypeDef = TypedDict(
     "SecurityProfileSummaryTypeDef",
     {
         "Id": str,
         "Arn": str,
         "Name": str,
     },
-    total=False,
 )
 
 SecurityProfileTypeDef = TypedDict(
     "SecurityProfileTypeDef",
     {
         "Id": str,
         "OrganizationResourceId": str,
         "Arn": str,
         "SecurityProfileName": str,
         "Description": str,
         "Tags": Dict[str, str],
         "AllowedAccessControlTags": Dict[str, str],
         "TagRestrictedResources": List[str],
     },
-    total=False,
 )
 
 SecurityProfilesSearchFilterTypeDef = TypedDict(
     "SecurityProfilesSearchFilterTypeDef",
     {
         "TagFilter": "ControlPlaneTagFilterTypeDef",
     },
@@ -6706,15 +6590,14 @@
 
 StringReferenceTypeDef = TypedDict(
     "StringReferenceTypeDef",
     {
         "Name": str,
         "Value": str,
     },
-    total=False,
 )
 
 _RequiredSubmitContactEvaluationRequestRequestTypeDef = TypedDict(
     "_RequiredSubmitContactEvaluationRequestRequestTypeDef",
     {
         "InstanceId": str,
         "EvaluationId": str,
@@ -6783,15 +6666,14 @@
 
 TagSetTypeDef = TypedDict(
     "TagSetTypeDef",
     {
         "key": str,
         "value": str,
     },
-    total=False,
 )
 
 _RequiredTaskActionDefinitionTypeDef = TypedDict(
     "_RequiredTaskActionDefinitionTypeDef",
     {
         "Name": str,
         "ContactFlowId": str,
@@ -6874,15 +6756,14 @@
         "Arn": str,
         "Name": str,
         "Description": str,
         "Status": TaskTemplateStatusType,
         "LastModifiedTime": datetime,
         "CreatedTime": datetime,
     },
-    total=False,
 )
 
 TelephonyConfigTypeDef = TypedDict(
     "TelephonyConfigTypeDef",
     {
         "Distributions": List["DistributionTypeDef"],
     },
@@ -6911,29 +6792,27 @@
     {
         "Id": str,
         "Arn": str,
         "Name": str,
         "InstanceArn": str,
         "Status": TrafficDistributionGroupStatusType,
     },
-    total=False,
 )
 
 TrafficDistributionGroupTypeDef = TypedDict(
     "TrafficDistributionGroupTypeDef",
     {
         "Id": str,
         "Arn": str,
         "Name": str,
         "Description": str,
         "InstanceArn": str,
         "Status": TrafficDistributionGroupStatusType,
         "Tags": Dict[str, str],
     },
-    total=False,
 )
 
 _RequiredTransferContactRequestRequestTypeDef = TypedDict(
     "_RequiredTransferContactRequestRequestTypeDef",
     {
         "InstanceId": str,
         "ContactId": str,
@@ -7637,25 +7516,23 @@
 
 UrlReferenceTypeDef = TypedDict(
     "UrlReferenceTypeDef",
     {
         "Name": str,
         "Value": str,
     },
-    total=False,
 )
 
 UseCaseTypeDef = TypedDict(
     "UseCaseTypeDef",
     {
         "UseCaseId": str,
         "UseCaseArn": str,
         "UseCaseType": UseCaseTypeType,
     },
-    total=False,
 )
 
 UserDataFiltersTypeDef = TypedDict(
     "UserDataFiltersTypeDef",
     {
         "Queues": Sequence[str],
         "ContactFilter": "ContactFilterTypeDef",
@@ -7675,24 +7552,22 @@
         "Status": "AgentStatusReferenceTypeDef",
         "AvailableSlotsByChannel": Dict[ChannelType, int],
         "MaxSlotsByChannel": Dict[ChannelType, int],
         "ActiveSlotsByChannel": Dict[ChannelType, int],
         "Contacts": List["AgentContactReferenceTypeDef"],
         "NextStatus": str,
     },
-    total=False,
 )
 
 UserIdentityInfoLiteTypeDef = TypedDict(
     "UserIdentityInfoLiteTypeDef",
     {
         "FirstName": str,
         "LastName": str,
     },
-    total=False,
 )
 
 UserIdentityInfoTypeDef = TypedDict(
     "UserIdentityInfoTypeDef",
     {
         "FirstName": str,
         "LastName": str,
@@ -7732,15 +7607,14 @@
 
 UserReferenceTypeDef = TypedDict(
     "UserReferenceTypeDef",
     {
         "Id": str,
         "Arn": str,
     },
-    total=False,
 )
 
 UserSearchCriteriaTypeDef = TypedDict(
     "UserSearchCriteriaTypeDef",
     {
         "OrConditions": Sequence[Dict[str, Any]],
         "AndConditions": Sequence[Dict[str, Any]],
@@ -7768,25 +7642,23 @@
         "IdentityInfo": "UserIdentityInfoLiteTypeDef",
         "PhoneConfig": "UserPhoneConfigTypeDef",
         "RoutingProfileId": str,
         "SecurityProfileIds": List[str],
         "Tags": Dict[str, str],
         "Username": str,
     },
-    total=False,
 )
 
 UserSummaryTypeDef = TypedDict(
     "UserSummaryTypeDef",
     {
         "Id": str,
         "Arn": str,
         "Username": str,
     },
-    total=False,
 )
 
 UserTypeDef = TypedDict(
     "UserTypeDef",
     {
         "Id": str,
         "Arn": str,
@@ -7795,73 +7667,51 @@
         "PhoneConfig": "UserPhoneConfigTypeDef",
         "DirectoryUserId": str,
         "SecurityProfileIds": List[str],
         "RoutingProfileId": str,
         "HierarchyGroupId": str,
         "Tags": Dict[str, str],
     },
-    total=False,
 )
 
-_RequiredVocabularySummaryTypeDef = TypedDict(
-    "_RequiredVocabularySummaryTypeDef",
+VocabularySummaryTypeDef = TypedDict(
+    "VocabularySummaryTypeDef",
     {
         "Name": str,
         "Id": str,
         "Arn": str,
         "LanguageCode": VocabularyLanguageCodeType,
         "State": VocabularyStateType,
         "LastModifiedTime": datetime,
-    },
-)
-_OptionalVocabularySummaryTypeDef = TypedDict(
-    "_OptionalVocabularySummaryTypeDef",
-    {
         "FailureReason": str,
     },
-    total=False,
 )
 
-class VocabularySummaryTypeDef(
-    _RequiredVocabularySummaryTypeDef, _OptionalVocabularySummaryTypeDef
-):
-    pass
-
-_RequiredVocabularyTypeDef = TypedDict(
-    "_RequiredVocabularyTypeDef",
+VocabularyTypeDef = TypedDict(
+    "VocabularyTypeDef",
     {
         "Name": str,
         "Id": str,
         "Arn": str,
         "LanguageCode": VocabularyLanguageCodeType,
         "State": VocabularyStateType,
         "LastModifiedTime": datetime,
-    },
-)
-_OptionalVocabularyTypeDef = TypedDict(
-    "_OptionalVocabularyTypeDef",
-    {
         "FailureReason": str,
         "Content": str,
         "Tags": Dict[str, str],
     },
-    total=False,
 )
 
-class VocabularyTypeDef(_RequiredVocabularyTypeDef, _OptionalVocabularyTypeDef):
-    pass
-
 VoiceRecordingConfigurationTypeDef = TypedDict(
     "VoiceRecordingConfigurationTypeDef",
     {
         "VoiceRecordingTrack": VoiceRecordingTrackType,
     },
     total=False,
 )
 
 WisdomInfoTypeDef = TypedDict(
     "WisdomInfoTypeDef",
     {
         "SessionArn": str,
     },
-    total=False,
 )
```

### Comparing `mypy-boto3-connect-1.28.0/mypy_boto3_connect.egg-info/PKG-INFO` & `mypy-boto3-connect-1.28.3/mypy_boto3_connect.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-connect
-Version: 1.28.0
-Summary: Type annotations for boto3.Connect 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.3
+Summary: Type annotations for boto3.Connect 1.28.3 service generated with mypy-boto3-builder 7.14.6
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-connect.svg?color=blue)](https://pypi.org/project/mypy-boto3-connect)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-connect?color=blue)](https://pypistats.org/packages/mypy-boto3-connect)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Connect 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect)
+[boto3.Connect 1.28.3](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect)
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
 [mypy-boto3-connect docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/).
 
 See how it helps to find and fix potential bugs:
 
@@ -673,15 +673,17 @@
     DeleteContactFlowModuleRequestRequestTypeDef,
     DeleteContactFlowRequestRequestTypeDef,
     DeleteEvaluationFormRequestRequestTypeDef,
     DeleteHoursOfOperationRequestRequestTypeDef,
     DeleteInstanceRequestRequestTypeDef,
     DeleteIntegrationAssociationRequestRequestTypeDef,
     DeletePromptRequestRequestTypeDef,
+    DeleteQueueRequestRequestTypeDef,
     DeleteQuickConnectRequestRequestTypeDef,
+    DeleteRoutingProfileRequestRequestTypeDef,
     DeleteRuleRequestRequestTypeDef,
     DeleteSecurityProfileRequestRequestTypeDef,
     DeleteTaskTemplateRequestRequestTypeDef,
     DeleteTrafficDistributionGroupRequestRequestTypeDef,
     DeleteUseCaseRequestRequestTypeDef,
     DeleteUserHierarchyGroupRequestRequestTypeDef,
     DeleteUserRequestRequestTypeDef,
```

### Comparing `mypy-boto3-connect-1.28.0/mypy_boto3_connect.egg-info/SOURCES.txt` & `mypy-boto3-connect-1.28.3/mypy_boto3_connect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-connect-1.28.0/setup.py` & `mypy-boto3-connect-1.28.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-connect",
-    version="1.28.0",
+    version="1.28.3",
     packages=["mypy_boto3_connect"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Connect 1.28.0 service generated with mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.Connect 1.28.3 service generated with mypy-boto3-builder 7.14.6"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

