# Comparing `tmp/mypy-boto3-sagemaker-1.28.0.tar.gz` & `tmp/mypy-boto3-sagemaker-1.28.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-sagemaker-1.28.0.tar", last modified: Thu Jul  6 21:00:33 2023, max compression
+gzip compressed data, was "mypy-boto3-sagemaker-1.28.3.tar", last modified: Thu Jul 13 19:49:15 2023, max compression
```

## Comparing `mypy-boto3-sagemaker-1.28.0.tar` & `mypy-boto3-sagemaker-1.28.3.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:33.054422 mypy-boto3-sagemaker-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:54:18.000000 mypy-boto3-sagemaker-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    80735 2023-07-06 21:00:33.054422 mypy-boto3-sagemaker-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    79242 2023-07-06 20:54:18.000000 mypy-boto3-sagemaker-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:33.038422 mypy-boto3-sagemaker-1.28.0/mypy_boto3_sagemaker/
--rw-r--r--   0 runner    (1001) docker     (123)    18513 2023-07-06 20:54:18.000000 mypy-boto3-sagemaker-1.28.0/mypy_boto3_sagemaker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18512 2023-07-06 20:54:18.000000 mypy-boto3-sagemaker-1.28.0/mypy_boto3_sagemaker/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-07-06 20:54:18.000000 mypy-boto3-sagemaker-1.28.0/mypy_boto3_sagemaker/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)   262100 2023-07-06 20:54:24.000000 mypy-boto3-sagemaker-1.28.0/mypy_boto3_sagemaker/client.py
--rw-r--r--   0 runner    (1001) docker     (123)   261710 2023-07-06 20:54:23.000000 mypy-boto3-sagemaker-1.28.0/mypy_boto3_sagemaker/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    57365 2023-07-06 20:54:27.000000 mypy-boto3-sagemaker-1.28.0/mypy_boto3_sagemaker/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    57363 2023-07-06 20:54:26.000000 mypy-boto3-sagemaker-1.28.0/mypy_boto3_sagemaker/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    97555 2023-07-06 20:54:26.000000 mypy-boto3-sagemaker-1.28.0/mypy_boto3_sagemaker/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    97484 2023-07-06 20:54:25.000000 mypy-boto3-sagemaker-1.28.0/mypy_boto3_sagemaker/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:54:18.000000 mypy-boto3-sagemaker-1.28.0/mypy_boto3_sagemaker/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   495915 2023-07-06 20:54:47.000000 mypy-boto3-sagemaker-1.28.0/mypy_boto3_sagemaker/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   495286 2023-07-06 20:54:37.000000 mypy-boto3-sagemaker-1.28.0/mypy_boto3_sagemaker/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:54:18.000000 mypy-boto3-sagemaker-1.28.0/mypy_boto3_sagemaker/version.py
--rw-r--r--   0 runner    (1001) docker     (123)    13320 2023-07-06 20:54:26.000000 mypy-boto3-sagemaker-1.28.0/mypy_boto3_sagemaker/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)    13307 2023-07-06 20:54:26.000000 mypy-boto3-sagemaker-1.28.0/mypy_boto3_sagemaker/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:33.054422 mypy-boto3-sagemaker-1.28.0/mypy_boto3_sagemaker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    80735 2023-07-06 21:00:32.000000 mypy-boto3-sagemaker-1.28.0/mypy_boto3_sagemaker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-07-06 21:00:32.000000 mypy-boto3-sagemaker-1.28.0/mypy_boto3_sagemaker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:32.000000 mypy-boto3-sagemaker-1.28.0/mypy_boto3_sagemaker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:32.000000 mypy-boto3-sagemaker-1.28.0/mypy_boto3_sagemaker.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 21:00:32.000000 mypy-boto3-sagemaker-1.28.0/mypy_boto3_sagemaker.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-06 21:00:32.000000 mypy-boto3-sagemaker-1.28.0/mypy_boto3_sagemaker.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 21:00:33.054422 mypy-boto3-sagemaker-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-07-06 20:54:17.000000 mypy-boto3-sagemaker-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:49:15.193303 mypy-boto3-sagemaker-1.28.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-13 19:48:42.000000 mypy-boto3-sagemaker-1.28.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    80765 2023-07-13 19:49:15.193303 mypy-boto3-sagemaker-1.28.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    79272 2023-07-13 19:48:42.000000 mypy-boto3-sagemaker-1.28.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:49:15.193303 mypy-boto3-sagemaker-1.28.3/mypy_boto3_sagemaker/
+-rw-r--r--   0 runner    (1001) docker     (123)    18513 2023-07-13 19:48:43.000000 mypy-boto3-sagemaker-1.28.3/mypy_boto3_sagemaker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18512 2023-07-13 19:48:42.000000 mypy-boto3-sagemaker-1.28.3/mypy_boto3_sagemaker/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-07-13 19:48:43.000000 mypy-boto3-sagemaker-1.28.3/mypy_boto3_sagemaker/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   262100 2023-07-13 19:48:45.000000 mypy-boto3-sagemaker-1.28.3/mypy_boto3_sagemaker/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)   261710 2023-07-13 19:48:44.000000 mypy-boto3-sagemaker-1.28.3/mypy_boto3_sagemaker/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    57365 2023-07-13 19:48:48.000000 mypy-boto3-sagemaker-1.28.3/mypy_boto3_sagemaker/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57363 2023-07-13 19:48:48.000000 mypy-boto3-sagemaker-1.28.3/mypy_boto3_sagemaker/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    97555 2023-07-13 19:48:46.000000 mypy-boto3-sagemaker-1.28.3/mypy_boto3_sagemaker/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    97484 2023-07-13 19:48:46.000000 mypy-boto3-sagemaker-1.28.3/mypy_boto3_sagemaker/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 19:48:43.000000 mypy-boto3-sagemaker-1.28.3/mypy_boto3_sagemaker/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   474493 2023-07-13 19:49:00.000000 mypy-boto3-sagemaker-1.28.3/mypy_boto3_sagemaker/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   474008 2023-07-13 19:48:53.000000 mypy-boto3-sagemaker-1.28.3/mypy_boto3_sagemaker/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-13 19:48:42.000000 mypy-boto3-sagemaker-1.28.3/mypy_boto3_sagemaker/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13320 2023-07-13 19:48:46.000000 mypy-boto3-sagemaker-1.28.3/mypy_boto3_sagemaker/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13307 2023-07-13 19:48:46.000000 mypy-boto3-sagemaker-1.28.3/mypy_boto3_sagemaker/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:49:15.193303 mypy-boto3-sagemaker-1.28.3/mypy_boto3_sagemaker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    80765 2023-07-13 19:49:15.000000 mypy-boto3-sagemaker-1.28.3/mypy_boto3_sagemaker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-07-13 19:49:15.000000 mypy-boto3-sagemaker-1.28.3/mypy_boto3_sagemaker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 19:49:15.000000 mypy-boto3-sagemaker-1.28.3/mypy_boto3_sagemaker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 19:49:15.000000 mypy-boto3-sagemaker-1.28.3/mypy_boto3_sagemaker.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-13 19:49:15.000000 mypy-boto3-sagemaker-1.28.3/mypy_boto3_sagemaker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-13 19:49:15.000000 mypy-boto3-sagemaker-1.28.3/mypy_boto3_sagemaker.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 19:49:15.193303 mypy-boto3-sagemaker-1.28.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-07-13 19:48:42.000000 mypy-boto3-sagemaker-1.28.3/setup.py
```

### Comparing `mypy-boto3-sagemaker-1.28.0/LICENSE` & `mypy-boto3-sagemaker-1.28.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sagemaker-1.28.0/PKG-INFO` & `mypy-boto3-sagemaker-1.28.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-sagemaker
-Version: 1.28.0
-Summary: Type annotations for boto3.SageMaker 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.3
+Summary: Type annotations for boto3.SageMaker 1.28.3 service generated with mypy-boto3-builder 7.14.6
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-sagemaker.svg?color=blue)](https://pypi.org/project/mypy-boto3-sagemaker)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-sagemaker?color=blue)](https://pypistats.org/packages/mypy-boto3-sagemaker)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SageMaker 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker)
+[boto3.SageMaker 1.28.3](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker)
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
 [mypy-boto3-sagemaker docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker/).
 
 See how it helps to find and fix potential bugs:
 
@@ -962,14 +962,15 @@
     MetricsSourceTypeDef,
     CacheHitResultTypeDef,
     OutputParameterTypeDef,
     CandidateArtifactLocationsTypeDef,
     MetricDatumTypeDef,
     ModelRegisterSettingsTypeDef,
     TimeSeriesForecastingSettingsTypeDef,
+    WorkspaceSettingsTypeDef,
     CapacitySizeTypeDef,
     CaptureContentTypeHeaderTypeDef,
     CaptureOptionTypeDef,
     CategoricalParameterRangeSpecificationTypeDef,
     CategoricalParameterRangeTypeDef,
     CategoricalParameterTypeDef,
     ChannelSpecificationTypeDef,
```

### Comparing `mypy-boto3-sagemaker-1.28.0/README.md` & `mypy-boto3-sagemaker-1.28.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-sagemaker.svg?color=blue)](https://pypi.org/project/mypy-boto3-sagemaker)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-sagemaker?color=blue)](https://pypistats.org/packages/mypy-boto3-sagemaker)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SageMaker 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker)
+[boto3.SageMaker 1.28.3](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker)
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
 [mypy-boto3-sagemaker docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker/).
 
 See how it helps to find and fix potential bugs:
 
@@ -930,14 +930,15 @@
     MetricsSourceTypeDef,
     CacheHitResultTypeDef,
     OutputParameterTypeDef,
     CandidateArtifactLocationsTypeDef,
     MetricDatumTypeDef,
     ModelRegisterSettingsTypeDef,
     TimeSeriesForecastingSettingsTypeDef,
+    WorkspaceSettingsTypeDef,
     CapacitySizeTypeDef,
     CaptureContentTypeHeaderTypeDef,
     CaptureOptionTypeDef,
     CategoricalParameterRangeSpecificationTypeDef,
     CategoricalParameterRangeTypeDef,
     CategoricalParameterTypeDef,
     ChannelSpecificationTypeDef,
```

### Comparing `mypy-boto3-sagemaker-1.28.0/mypy_boto3_sagemaker/__init__.py` & `mypy-boto3-sagemaker-1.28.3/mypy_boto3_sagemaker/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sagemaker-1.28.0/mypy_boto3_sagemaker/__init__.pyi` & `mypy-boto3-sagemaker-1.28.3/mypy_boto3_sagemaker/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sagemaker-1.28.0/mypy_boto3_sagemaker/__main__.py` & `mypy-boto3-sagemaker-1.28.3/mypy_boto3_sagemaker/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.SageMaker 1.28.0\nVersion:         1.28.0\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.SageMaker 1.28.3\nVersion:         1.28.3\nBuilder version:"
+        " 7.14.6\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker\nOther"
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

### Comparing `mypy-boto3-sagemaker-1.28.0/mypy_boto3_sagemaker/client.py` & `mypy-boto3-sagemaker-1.28.3/mypy_boto3_sagemaker/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sagemaker-1.28.0/mypy_boto3_sagemaker/client.pyi` & `mypy-boto3-sagemaker-1.28.3/mypy_boto3_sagemaker/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sagemaker-1.28.0/mypy_boto3_sagemaker/literals.py` & `mypy-boto3-sagemaker-1.28.3/mypy_boto3_sagemaker/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sagemaker-1.28.0/mypy_boto3_sagemaker/literals.pyi` & `mypy-boto3-sagemaker-1.28.3/mypy_boto3_sagemaker/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sagemaker-1.28.0/mypy_boto3_sagemaker/paginator.py` & `mypy-boto3-sagemaker-1.28.3/mypy_boto3_sagemaker/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sagemaker-1.28.0/mypy_boto3_sagemaker/paginator.pyi` & `mypy-boto3-sagemaker-1.28.3/mypy_boto3_sagemaker/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sagemaker-1.28.0/mypy_boto3_sagemaker/type_defs.py` & `mypy-boto3-sagemaker-1.28.3/mypy_boto3_sagemaker/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -300,14 +300,15 @@
     "MetricsSourceTypeDef",
     "CacheHitResultTypeDef",
     "OutputParameterTypeDef",
     "CandidateArtifactLocationsTypeDef",
     "MetricDatumTypeDef",
     "ModelRegisterSettingsTypeDef",
     "TimeSeriesForecastingSettingsTypeDef",
+    "WorkspaceSettingsTypeDef",
     "CapacitySizeTypeDef",
     "CaptureContentTypeHeaderTypeDef",
     "CaptureOptionTypeDef",
     "CategoricalParameterRangeSpecificationTypeDef",
     "CategoricalParameterRangeTypeDef",
     "CategoricalParameterTypeDef",
     "ChannelSpecificationTypeDef",
@@ -1463,57 +1464,33 @@
     "MetricDefinitionTypeDef",
     {
         "Name": str,
         "Regex": str,
     },
 )
 
-_RequiredAlgorithmStatusItemTypeDef = TypedDict(
-    "_RequiredAlgorithmStatusItemTypeDef",
+AlgorithmStatusItemTypeDef = TypedDict(
+    "AlgorithmStatusItemTypeDef",
     {
         "Name": str,
         "Status": DetailedAlgorithmStatusType,
-    },
-)
-_OptionalAlgorithmStatusItemTypeDef = TypedDict(
-    "_OptionalAlgorithmStatusItemTypeDef",
-    {
         "FailureReason": str,
     },
-    total=False,
 )
 
-
-class AlgorithmStatusItemTypeDef(
-    _RequiredAlgorithmStatusItemTypeDef, _OptionalAlgorithmStatusItemTypeDef
-):
-    pass
-
-
-_RequiredAlgorithmSummaryTypeDef = TypedDict(
-    "_RequiredAlgorithmSummaryTypeDef",
+AlgorithmSummaryTypeDef = TypedDict(
+    "AlgorithmSummaryTypeDef",
     {
         "AlgorithmName": str,
         "AlgorithmArn": str,
+        "AlgorithmDescription": str,
         "CreationTime": datetime,
         "AlgorithmStatus": AlgorithmStatusType,
     },
 )
-_OptionalAlgorithmSummaryTypeDef = TypedDict(
-    "_OptionalAlgorithmSummaryTypeDef",
-    {
-        "AlgorithmDescription": str,
-    },
-    total=False,
-)
-
-
-class AlgorithmSummaryTypeDef(_RequiredAlgorithmSummaryTypeDef, _OptionalAlgorithmSummaryTypeDef):
-    pass
-
 
 AnnotationConsolidationConfigTypeDef = TypedDict(
     "AnnotationConsolidationConfigTypeDef",
     {
         "AnnotationConsolidationLambdaArn": str,
     },
 )
@@ -1525,15 +1502,14 @@
         "UserProfileName": str,
         "AppType": AppTypeType,
         "AppName": str,
         "Status": AppStatusType,
         "CreationTime": datetime,
         "SpaceName": str,
     },
-    total=False,
 )
 
 _RequiredAppSpecificationTypeDef = TypedDict(
     "_RequiredAppSpecificationTypeDef",
     {
         "ImageUri": str,
     },
@@ -1634,59 +1610,33 @@
     {
         "CandidateStepType": CandidateStepTypeType,
         "CandidateStepArn": str,
         "CandidateStepName": str,
     },
 )
 
-_RequiredAutoMLContainerDefinitionTypeDef = TypedDict(
-    "_RequiredAutoMLContainerDefinitionTypeDef",
+AutoMLContainerDefinitionTypeDef = TypedDict(
+    "AutoMLContainerDefinitionTypeDef",
     {
         "Image": str,
         "ModelDataUrl": str,
-    },
-)
-_OptionalAutoMLContainerDefinitionTypeDef = TypedDict(
-    "_OptionalAutoMLContainerDefinitionTypeDef",
-    {
         "Environment": Dict[str, str],
     },
-    total=False,
 )
 
-
-class AutoMLContainerDefinitionTypeDef(
-    _RequiredAutoMLContainerDefinitionTypeDef, _OptionalAutoMLContainerDefinitionTypeDef
-):
-    pass
-
-
-_RequiredFinalAutoMLJobObjectiveMetricTypeDef = TypedDict(
-    "_RequiredFinalAutoMLJobObjectiveMetricTypeDef",
+FinalAutoMLJobObjectiveMetricTypeDef = TypedDict(
+    "FinalAutoMLJobObjectiveMetricTypeDef",
     {
+        "Type": AutoMLJobObjectiveTypeType,
         "MetricName": AutoMLMetricEnumType,
         "Value": float,
-    },
-)
-_OptionalFinalAutoMLJobObjectiveMetricTypeDef = TypedDict(
-    "_OptionalFinalAutoMLJobObjectiveMetricTypeDef",
-    {
-        "Type": AutoMLJobObjectiveTypeType,
         "StandardMetricName": AutoMLMetricEnumType,
     },
-    total=False,
 )
 
-
-class FinalAutoMLJobObjectiveMetricTypeDef(
-    _RequiredFinalAutoMLJobObjectiveMetricTypeDef, _OptionalFinalAutoMLJobObjectiveMetricTypeDef
-):
-    pass
-
-
 AutoMLS3DataSourceTypeDef = TypedDict(
     "AutoMLS3DataSourceTypeDef",
     {
         "S3DataType": AutoMLS3DataTypeType,
         "S3Uri": str,
     },
 )
@@ -1701,15 +1651,14 @@
 
 AutoMLJobArtifactsTypeDef = TypedDict(
     "AutoMLJobArtifactsTypeDef",
     {
         "CandidateDefinitionNotebookLocation": str,
         "DataExplorationNotebookLocation": str,
     },
-    total=False,
 )
 
 AutoMLJobCompletionCriteriaTypeDef = TypedDict(
     "AutoMLJobCompletionCriteriaTypeDef",
     {
         "MaxCandidates": int,
         "MaxRuntimePerTrainingJobInSeconds": int,
@@ -1726,23 +1675,21 @@
 )
 
 AutoMLJobStepMetadataTypeDef = TypedDict(
     "AutoMLJobStepMetadataTypeDef",
     {
         "Arn": str,
     },
-    total=False,
 )
 
 AutoMLPartialFailureReasonTypeDef = TypedDict(
     "AutoMLPartialFailureReasonTypeDef",
     {
         "PartialFailureMessage": str,
     },
-    total=False,
 )
 
 _RequiredAutoMLOutputDataConfigTypeDef = TypedDict(
     "_RequiredAutoMLOutputDataConfigTypeDef",
     {
         "S3OutputPath": str,
     },
@@ -1763,15 +1710,14 @@
 
 
 TabularResolvedAttributesTypeDef = TypedDict(
     "TabularResolvedAttributesTypeDef",
     {
         "ProblemType": ProblemTypeType,
     },
-    total=False,
 )
 
 VpcConfigTypeDef = TypedDict(
     "VpcConfigTypeDef",
     {
         "SecurityGroupIds": Sequence[str],
         "Subnets": Sequence[str],
@@ -1859,56 +1805,41 @@
 
 
 CacheHitResultTypeDef = TypedDict(
     "CacheHitResultTypeDef",
     {
         "SourcePipelineExecutionArn": str,
     },
-    total=False,
 )
 
 OutputParameterTypeDef = TypedDict(
     "OutputParameterTypeDef",
     {
         "Name": str,
         "Value": str,
     },
 )
 
-_RequiredCandidateArtifactLocationsTypeDef = TypedDict(
-    "_RequiredCandidateArtifactLocationsTypeDef",
+CandidateArtifactLocationsTypeDef = TypedDict(
+    "CandidateArtifactLocationsTypeDef",
     {
         "Explainability": str,
-    },
-)
-_OptionalCandidateArtifactLocationsTypeDef = TypedDict(
-    "_OptionalCandidateArtifactLocationsTypeDef",
-    {
         "ModelInsights": str,
         "BacktestResults": str,
     },
-    total=False,
 )
 
-
-class CandidateArtifactLocationsTypeDef(
-    _RequiredCandidateArtifactLocationsTypeDef, _OptionalCandidateArtifactLocationsTypeDef
-):
-    pass
-
-
 MetricDatumTypeDef = TypedDict(
     "MetricDatumTypeDef",
     {
         "MetricName": AutoMLMetricEnumType,
         "Value": float,
         "Set": MetricSetSourceType,
         "StandardMetricName": AutoMLMetricExtendedEnumType,
     },
-    total=False,
 )
 
 ModelRegisterSettingsTypeDef = TypedDict(
     "ModelRegisterSettingsTypeDef",
     {
         "Status": FeatureStatusType,
         "CrossAccountModelRegisterRoleArn": str,
@@ -1921,14 +1852,23 @@
     {
         "Status": FeatureStatusType,
         "AmazonForecastRoleArn": str,
     },
     total=False,
 )
 
+WorkspaceSettingsTypeDef = TypedDict(
+    "WorkspaceSettingsTypeDef",
+    {
+        "S3ArtifactPath": str,
+        "S3KmsKeyId": str,
+    },
+    total=False,
+)
+
 CapacitySizeTypeDef = TypedDict(
     "CapacitySizeTypeDef",
     {
         "Type": CapacitySizeTypeType,
         "Value": int,
     },
 )
@@ -2031,15 +1971,14 @@
         "CalculatedBaselineConstraints": str,
         "ModelPackageGroupName": str,
         "ViolationReport": str,
         "CheckJobArn": str,
         "SkipCheck": bool,
         "RegisterNewBaseline": bool,
     },
-    total=False,
 )
 
 ClarifyInferenceConfigTypeDef = TypedDict(
     "ClarifyInferenceConfigTypeDef",
     {
         "FeaturesAttribute": str,
         "ContentTemplate": str,
@@ -2123,50 +2062,36 @@
     {
         "CollectionName": str,
         "CollectionParameters": Mapping[str, str],
     },
     total=False,
 )
 
-_RequiredCompilationJobSummaryTypeDef = TypedDict(
-    "_RequiredCompilationJobSummaryTypeDef",
+CompilationJobSummaryTypeDef = TypedDict(
+    "CompilationJobSummaryTypeDef",
     {
         "CompilationJobName": str,
         "CompilationJobArn": str,
         "CreationTime": datetime,
-        "CompilationJobStatus": CompilationJobStatusType,
-    },
-)
-_OptionalCompilationJobSummaryTypeDef = TypedDict(
-    "_OptionalCompilationJobSummaryTypeDef",
-    {
         "CompilationStartTime": datetime,
         "CompilationEndTime": datetime,
         "CompilationTargetDevice": TargetDeviceType,
         "CompilationTargetPlatformOs": TargetPlatformOsType,
         "CompilationTargetPlatformArch": TargetPlatformArchType,
         "CompilationTargetPlatformAccelerator": TargetPlatformAcceleratorType,
         "LastModifiedTime": datetime,
+        "CompilationJobStatus": CompilationJobStatusType,
     },
-    total=False,
 )
 
-
-class CompilationJobSummaryTypeDef(
-    _RequiredCompilationJobSummaryTypeDef, _OptionalCompilationJobSummaryTypeDef
-):
-    pass
-
-
 ConditionStepMetadataTypeDef = TypedDict(
     "ConditionStepMetadataTypeDef",
     {
         "Outcome": ConditionOutcomeType,
     },
-    total=False,
 )
 
 MultiModelConfigTypeDef = TypedDict(
     "MultiModelConfigTypeDef",
     {
         "ModelCacheSetting": ModelCacheSettingType,
     },
@@ -3496,15 +3421,14 @@
     {
         "RuleConfigurationName": str,
         "RuleEvaluationJobArn": str,
         "RuleEvaluationStatus": RuleEvaluationStatusType,
         "StatusDetails": str,
         "LastModifiedTime": datetime,
     },
-    total=False,
 )
 
 DeleteActionRequestRequestTypeDef = TypedDict(
     "DeleteActionRequestRequestTypeDef",
     {
         "ActionName": str,
     },
@@ -3938,39 +3862,25 @@
 DeployedImageTypeDef = TypedDict(
     "DeployedImageTypeDef",
     {
         "SpecifiedImage": str,
         "ResolvedImage": str,
         "ResolutionTime": datetime,
     },
-    total=False,
 )
 
-_RequiredRealTimeInferenceRecommendationTypeDef = TypedDict(
-    "_RequiredRealTimeInferenceRecommendationTypeDef",
+RealTimeInferenceRecommendationTypeDef = TypedDict(
+    "RealTimeInferenceRecommendationTypeDef",
     {
         "RecommendationId": str,
         "InstanceType": ProductionVariantInstanceTypeType,
-    },
-)
-_OptionalRealTimeInferenceRecommendationTypeDef = TypedDict(
-    "_OptionalRealTimeInferenceRecommendationTypeDef",
-    {
         "Environment": Dict[str, str],
     },
-    total=False,
 )
 
-
-class RealTimeInferenceRecommendationTypeDef(
-    _RequiredRealTimeInferenceRecommendationTypeDef, _OptionalRealTimeInferenceRecommendationTypeDef
-):
-    pass
-
-
 _RequiredDeviceSelectionConfigTypeDef = TypedDict(
     "_RequiredDeviceSelectionConfigTypeDef",
     {
         "DeviceSubsetType": DeviceSubsetTypeType,
     },
 )
 _OptionalDeviceSelectionConfigTypeDef = TypedDict(
@@ -3993,39 +3903,26 @@
 EdgeDeploymentConfigTypeDef = TypedDict(
     "EdgeDeploymentConfigTypeDef",
     {
         "FailureHandlingPolicy": FailureHandlingPolicyType,
     },
 )
 
-_RequiredEdgeDeploymentStatusTypeDef = TypedDict(
-    "_RequiredEdgeDeploymentStatusTypeDef",
+EdgeDeploymentStatusTypeDef = TypedDict(
+    "EdgeDeploymentStatusTypeDef",
     {
         "StageStatus": StageStatusType,
         "EdgeDeploymentSuccessInStage": int,
         "EdgeDeploymentPendingInStage": int,
         "EdgeDeploymentFailedInStage": int,
-    },
-)
-_OptionalEdgeDeploymentStatusTypeDef = TypedDict(
-    "_OptionalEdgeDeploymentStatusTypeDef",
-    {
         "EdgeDeploymentStatusMessage": str,
         "EdgeDeploymentStageStartTime": datetime,
     },
-    total=False,
 )
 
-
-class EdgeDeploymentStatusTypeDef(
-    _RequiredEdgeDeploymentStatusTypeDef, _OptionalEdgeDeploymentStatusTypeDef
-):
-    pass
-
-
 DeregisterDevicesRequestRequestTypeDef = TypedDict(
     "DeregisterDevicesRequestRequestTypeDef",
     {
         "DeviceFleetName": str,
         "DeviceNames": Sequence[str],
     },
 )
@@ -4090,15 +3987,14 @@
 )
 
 ModelDeployResultTypeDef = TypedDict(
     "ModelDeployResultTypeDef",
     {
         "EndpointName": str,
     },
-    total=False,
 )
 
 DescribeAutoMLJobV2RequestRequestTypeDef = TypedDict(
     "DescribeAutoMLJobV2RequestRequestTypeDef",
     {
         "AutoMLJobName": str,
     },
@@ -4126,15 +4022,14 @@
 )
 
 ModelDigestsTypeDef = TypedDict(
     "ModelDigestsTypeDef",
     {
         "ArtifactDigest": str,
     },
-    total=False,
 )
 
 DescribeContextRequestRequestTypeDef = TypedDict(
     "DescribeContextRequestRequestTypeDef",
     {
         "ContextName": str,
     },
@@ -4172,35 +4067,24 @@
 
 class DescribeDeviceRequestRequestTypeDef(
     _RequiredDescribeDeviceRequestRequestTypeDef, _OptionalDescribeDeviceRequestRequestTypeDef
 ):
     pass
 
 
-_RequiredEdgeModelTypeDef = TypedDict(
-    "_RequiredEdgeModelTypeDef",
+EdgeModelTypeDef = TypedDict(
+    "EdgeModelTypeDef",
     {
         "ModelName": str,
         "ModelVersion": str,
-    },
-)
-_OptionalEdgeModelTypeDef = TypedDict(
-    "_OptionalEdgeModelTypeDef",
-    {
         "LatestSampleTime": datetime,
         "LatestInference": datetime,
     },
-    total=False,
 )
 
-
-class EdgeModelTypeDef(_RequiredEdgeModelTypeDef, _OptionalEdgeModelTypeDef):
-    pass
-
-
 DescribeDomainRequestRequestTypeDef = TypedDict(
     "DescribeDomainRequestRequestTypeDef",
     {
         "DomainId": str,
     },
 )
 
@@ -4230,37 +4114,24 @@
 DescribeEdgePackagingJobRequestRequestTypeDef = TypedDict(
     "DescribeEdgePackagingJobRequestRequestTypeDef",
     {
         "EdgePackagingJobName": str,
     },
 )
 
-_RequiredEdgePresetDeploymentOutputTypeDef = TypedDict(
-    "_RequiredEdgePresetDeploymentOutputTypeDef",
+EdgePresetDeploymentOutputTypeDef = TypedDict(
+    "EdgePresetDeploymentOutputTypeDef",
     {
         "Type": Literal["GreengrassV2Component"],
-    },
-)
-_OptionalEdgePresetDeploymentOutputTypeDef = TypedDict(
-    "_OptionalEdgePresetDeploymentOutputTypeDef",
-    {
         "Artifact": str,
         "Status": EdgePresetDeploymentStatusType,
         "StatusMessage": str,
     },
-    total=False,
 )
 
-
-class EdgePresetDeploymentOutputTypeDef(
-    _RequiredEdgePresetDeploymentOutputTypeDef, _OptionalEdgePresetDeploymentOutputTypeDef
-):
-    pass
-
-
 DescribeEndpointConfigInputRequestTypeDef = TypedDict(
     "DescribeEndpointConfigInputRequestTypeDef",
     {
         "EndpointConfigName": str,
     },
 )
 
@@ -4283,33 +4154,22 @@
 DescribeExperimentRequestRequestTypeDef = TypedDict(
     "DescribeExperimentRequestRequestTypeDef",
     {
         "ExperimentName": str,
     },
 )
 
-_RequiredExperimentSourceTypeDef = TypedDict(
-    "_RequiredExperimentSourceTypeDef",
+ExperimentSourceTypeDef = TypedDict(
+    "ExperimentSourceTypeDef",
     {
         "SourceArn": str,
-    },
-)
-_OptionalExperimentSourceTypeDef = TypedDict(
-    "_OptionalExperimentSourceTypeDef",
-    {
         "SourceType": str,
     },
-    total=False,
 )
 
-
-class ExperimentSourceTypeDef(_RequiredExperimentSourceTypeDef, _OptionalExperimentSourceTypeDef):
-    pass
-
-
 _RequiredDescribeFeatureGroupRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeFeatureGroupRequestRequestTypeDef",
     {
         "FeatureGroupName": str,
     },
 )
 _OptionalDescribeFeatureGroupRequestRequestTypeDef = TypedDict(
@@ -4324,69 +4184,44 @@
 class DescribeFeatureGroupRequestRequestTypeDef(
     _RequiredDescribeFeatureGroupRequestRequestTypeDef,
     _OptionalDescribeFeatureGroupRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredLastUpdateStatusTypeDef = TypedDict(
-    "_RequiredLastUpdateStatusTypeDef",
+LastUpdateStatusTypeDef = TypedDict(
+    "LastUpdateStatusTypeDef",
     {
         "Status": LastUpdateStatusValueType,
-    },
-)
-_OptionalLastUpdateStatusTypeDef = TypedDict(
-    "_OptionalLastUpdateStatusTypeDef",
-    {
         "FailureReason": str,
     },
-    total=False,
 )
 
-
-class LastUpdateStatusTypeDef(_RequiredLastUpdateStatusTypeDef, _OptionalLastUpdateStatusTypeDef):
-    pass
-
-
-_RequiredOfflineStoreStatusTypeDef = TypedDict(
-    "_RequiredOfflineStoreStatusTypeDef",
+OfflineStoreStatusTypeDef = TypedDict(
+    "OfflineStoreStatusTypeDef",
     {
         "Status": OfflineStoreStatusValueType,
-    },
-)
-_OptionalOfflineStoreStatusTypeDef = TypedDict(
-    "_OptionalOfflineStoreStatusTypeDef",
-    {
         "BlockedReason": str,
     },
-    total=False,
 )
 
-
-class OfflineStoreStatusTypeDef(
-    _RequiredOfflineStoreStatusTypeDef, _OptionalOfflineStoreStatusTypeDef
-):
-    pass
-
-
 DescribeFeatureMetadataRequestRequestTypeDef = TypedDict(
     "DescribeFeatureMetadataRequestRequestTypeDef",
     {
         "FeatureGroupName": str,
         "FeatureName": str,
     },
 )
 
 FeatureParameterTypeDef = TypedDict(
     "FeatureParameterTypeDef",
     {
         "Key": str,
         "Value": str,
     },
-    total=False,
 )
 
 DescribeFlowDefinitionRequestRequestTypeDef = TypedDict(
     "DescribeFlowDefinitionRequestRequestTypeDef",
     {
         "FlowDefinitionName": str,
     },
@@ -4418,15 +4253,14 @@
 
 HubContentDependencyTypeDef = TypedDict(
     "HubContentDependencyTypeDef",
     {
         "DependencyOriginPath": str,
         "DependencyCopyPath": str,
     },
-    total=False,
 )
 
 DescribeHubRequestRequestTypeDef = TypedDict(
     "DescribeHubRequestRequestTypeDef",
     {
         "HubName": str,
     },
@@ -4441,15 +4275,14 @@
 
 UiTemplateInfoTypeDef = TypedDict(
     "UiTemplateInfoTypeDef",
     {
         "Url": str,
         "ContentSha256": str,
     },
-    total=False,
 )
 
 DescribeHyperParameterTuningJobRequestRequestTypeDef = TypedDict(
     "DescribeHyperParameterTuningJobRequestRequestTypeDef",
     {
         "HyperParameterTuningJobName": str,
     },
@@ -4457,45 +4290,41 @@
 
 HyperParameterTuningJobCompletionDetailsTypeDef = TypedDict(
     "HyperParameterTuningJobCompletionDetailsTypeDef",
     {
         "NumberOfTrainingJobsObjectiveNotImproving": int,
         "ConvergenceDetectedTime": datetime,
     },
-    total=False,
 )
 
 HyperParameterTuningJobConsumedResourcesTypeDef = TypedDict(
     "HyperParameterTuningJobConsumedResourcesTypeDef",
     {
         "RuntimeInSeconds": int,
     },
-    total=False,
 )
 
 ObjectiveStatusCountersTypeDef = TypedDict(
     "ObjectiveStatusCountersTypeDef",
     {
         "Succeeded": int,
         "Pending": int,
         "Failed": int,
     },
-    total=False,
 )
 
 TrainingJobStatusCountersTypeDef = TypedDict(
     "TrainingJobStatusCountersTypeDef",
     {
         "Completed": int,
         "InProgress": int,
         "RetryableError": int,
         "NonRetryableError": int,
         "Stopped": int,
     },
-    total=False,
 )
 
 DescribeImageRequestRequestTypeDef = TypedDict(
     "DescribeImageRequestRequestTypeDef",
     {
         "ImageName": str,
     },
@@ -4566,35 +4395,24 @@
 DescribeInferenceExperimentRequestRequestTypeDef = TypedDict(
     "DescribeInferenceExperimentRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
-_RequiredEndpointMetadataTypeDef = TypedDict(
-    "_RequiredEndpointMetadataTypeDef",
+EndpointMetadataTypeDef = TypedDict(
+    "EndpointMetadataTypeDef",
     {
         "EndpointName": str,
-    },
-)
-_OptionalEndpointMetadataTypeDef = TypedDict(
-    "_OptionalEndpointMetadataTypeDef",
-    {
         "EndpointConfigName": str,
         "EndpointStatus": EndpointStatusType,
         "FailureReason": str,
     },
-    total=False,
 )
 
-
-class EndpointMetadataTypeDef(_RequiredEndpointMetadataTypeDef, _OptionalEndpointMetadataTypeDef):
-    pass
-
-
 DescribeInferenceRecommendationsJobRequestRequestTypeDef = TypedDict(
     "DescribeInferenceRecommendationsJobRequestRequestTypeDef",
     {
         "JobName": str,
     },
 )
 
@@ -4610,38 +4428,24 @@
     {
         "TotalLabeled": int,
         "HumanLabeled": int,
         "MachineLabeled": int,
         "FailedNonRetryableError": int,
         "Unlabeled": int,
     },
-    total=False,
 )
 
-_RequiredLabelingJobOutputTypeDef = TypedDict(
-    "_RequiredLabelingJobOutputTypeDef",
+LabelingJobOutputTypeDef = TypedDict(
+    "LabelingJobOutputTypeDef",
     {
         "OutputDatasetS3Uri": str,
-    },
-)
-_OptionalLabelingJobOutputTypeDef = TypedDict(
-    "_OptionalLabelingJobOutputTypeDef",
-    {
         "FinalActiveLearningModelArn": str,
     },
-    total=False,
 )
 
-
-class LabelingJobOutputTypeDef(
-    _RequiredLabelingJobOutputTypeDef, _OptionalLabelingJobOutputTypeDef
-):
-    pass
-
-
 DescribeLineageGroupRequestRequestTypeDef = TypedDict(
     "DescribeLineageGroupRequestRequestTypeDef",
     {
         "LineageGroupName": str,
     },
 )
 
@@ -4725,43 +4529,30 @@
 DescribeMonitoringScheduleRequestRequestTypeDef = TypedDict(
     "DescribeMonitoringScheduleRequestRequestTypeDef",
     {
         "MonitoringScheduleName": str,
     },
 )
 
-_RequiredMonitoringExecutionSummaryTypeDef = TypedDict(
-    "_RequiredMonitoringExecutionSummaryTypeDef",
+MonitoringExecutionSummaryTypeDef = TypedDict(
+    "MonitoringExecutionSummaryTypeDef",
     {
         "MonitoringScheduleName": str,
         "ScheduledTime": datetime,
         "CreationTime": datetime,
         "LastModifiedTime": datetime,
         "MonitoringExecutionStatus": ExecutionStatusType,
-    },
-)
-_OptionalMonitoringExecutionSummaryTypeDef = TypedDict(
-    "_OptionalMonitoringExecutionSummaryTypeDef",
-    {
         "ProcessingJobArn": str,
         "EndpointName": str,
         "FailureReason": str,
         "MonitoringJobDefinitionName": str,
         "MonitoringType": MonitoringTypeType,
     },
-    total=False,
 )
 
-
-class MonitoringExecutionSummaryTypeDef(
-    _RequiredMonitoringExecutionSummaryTypeDef, _OptionalMonitoringExecutionSummaryTypeDef
-):
-    pass
-
-
 DescribeNotebookInstanceInputRequestTypeDef = TypedDict(
     "DescribeNotebookInstanceInputRequestTypeDef",
     {
         "NotebookInstanceName": str,
     },
 )
 
@@ -4797,15 +4588,14 @@
 
 PipelineExperimentConfigTypeDef = TypedDict(
     "PipelineExperimentConfigTypeDef",
     {
         "ExperimentName": str,
         "TrialName": str,
     },
-    total=False,
 )
 
 DescribePipelineRequestRequestTypeDef = TypedDict(
     "DescribePipelineRequestRequestTypeDef",
     {
         "PipelineName": str,
     },
@@ -4827,15 +4617,14 @@
 
 ServiceCatalogProvisionedProductDetailsTypeDef = TypedDict(
     "ServiceCatalogProvisionedProductDetailsTypeDef",
     {
         "ProvisionedProductId": str,
         "ProvisionedProductStatusMessage": str,
     },
-    total=False,
 )
 
 DescribeSpaceRequestRequestTypeDef = TypedDict(
     "DescribeSpaceRequestRequestTypeDef",
     {
         "DomainId": str,
         "SpaceName": str,
@@ -4865,110 +4654,71 @@
 DescribeSubscribedWorkteamRequestRequestTypeDef = TypedDict(
     "DescribeSubscribedWorkteamRequestRequestTypeDef",
     {
         "WorkteamArn": str,
     },
 )
 
-_RequiredSubscribedWorkteamTypeDef = TypedDict(
-    "_RequiredSubscribedWorkteamTypeDef",
+SubscribedWorkteamTypeDef = TypedDict(
+    "SubscribedWorkteamTypeDef",
     {
         "WorkteamArn": str,
-    },
-)
-_OptionalSubscribedWorkteamTypeDef = TypedDict(
-    "_OptionalSubscribedWorkteamTypeDef",
-    {
         "MarketplaceTitle": str,
         "SellerName": str,
         "MarketplaceDescription": str,
         "ListingId": str,
     },
-    total=False,
 )
 
-
-class SubscribedWorkteamTypeDef(
-    _RequiredSubscribedWorkteamTypeDef, _OptionalSubscribedWorkteamTypeDef
-):
-    pass
-
-
 DescribeTrainingJobRequestRequestTypeDef = TypedDict(
     "DescribeTrainingJobRequestRequestTypeDef",
     {
         "TrainingJobName": str,
     },
 )
 
 MetricDataTypeDef = TypedDict(
     "MetricDataTypeDef",
     {
         "MetricName": str,
         "Value": float,
         "Timestamp": datetime,
     },
-    total=False,
 )
 
 ProfilerRuleEvaluationStatusTypeDef = TypedDict(
     "ProfilerRuleEvaluationStatusTypeDef",
     {
         "RuleConfigurationName": str,
         "RuleEvaluationJobArn": str,
         "RuleEvaluationStatus": RuleEvaluationStatusType,
         "StatusDetails": str,
         "LastModifiedTime": datetime,
     },
-    total=False,
 )
 
-_RequiredSecondaryStatusTransitionTypeDef = TypedDict(
-    "_RequiredSecondaryStatusTransitionTypeDef",
+SecondaryStatusTransitionTypeDef = TypedDict(
+    "SecondaryStatusTransitionTypeDef",
     {
         "Status": SecondaryStatusType,
         "StartTime": datetime,
-    },
-)
-_OptionalSecondaryStatusTransitionTypeDef = TypedDict(
-    "_OptionalSecondaryStatusTransitionTypeDef",
-    {
         "EndTime": datetime,
         "StatusMessage": str,
     },
-    total=False,
 )
 
-
-class SecondaryStatusTransitionTypeDef(
-    _RequiredSecondaryStatusTransitionTypeDef, _OptionalSecondaryStatusTransitionTypeDef
-):
-    pass
-
-
-_RequiredWarmPoolStatusTypeDef = TypedDict(
-    "_RequiredWarmPoolStatusTypeDef",
+WarmPoolStatusTypeDef = TypedDict(
+    "WarmPoolStatusTypeDef",
     {
         "Status": WarmPoolResourceStatusType,
-    },
-)
-_OptionalWarmPoolStatusTypeDef = TypedDict(
-    "_OptionalWarmPoolStatusTypeDef",
-    {
         "ResourceRetainedBillableTimeInSeconds": int,
         "ReusedByJob": str,
     },
-    total=False,
 )
 
-
-class WarmPoolStatusTypeDef(_RequiredWarmPoolStatusTypeDef, _OptionalWarmPoolStatusTypeDef):
-    pass
-
-
 DescribeTransformJobRequestRequestTypeDef = TypedDict(
     "DescribeTransformJobRequestRequestTypeDef",
     {
         "TransformJobName": str,
     },
 )
 
@@ -4988,64 +4738,39 @@
         "Max": float,
         "Min": float,
         "Last": float,
         "Count": int,
         "Avg": float,
         "StdDev": float,
     },
-    total=False,
 )
 
-_RequiredTrialComponentSourceTypeDef = TypedDict(
-    "_RequiredTrialComponentSourceTypeDef",
+TrialComponentSourceTypeDef = TypedDict(
+    "TrialComponentSourceTypeDef",
     {
         "SourceArn": str,
-    },
-)
-_OptionalTrialComponentSourceTypeDef = TypedDict(
-    "_OptionalTrialComponentSourceTypeDef",
-    {
         "SourceType": str,
     },
-    total=False,
 )
 
-
-class TrialComponentSourceTypeDef(
-    _RequiredTrialComponentSourceTypeDef, _OptionalTrialComponentSourceTypeDef
-):
-    pass
-
-
 DescribeTrialRequestRequestTypeDef = TypedDict(
     "DescribeTrialRequestRequestTypeDef",
     {
         "TrialName": str,
     },
 )
 
-_RequiredTrialSourceTypeDef = TypedDict(
-    "_RequiredTrialSourceTypeDef",
+TrialSourceTypeDef = TypedDict(
+    "TrialSourceTypeDef",
     {
         "SourceArn": str,
-    },
-)
-_OptionalTrialSourceTypeDef = TypedDict(
-    "_OptionalTrialSourceTypeDef",
-    {
         "SourceType": str,
     },
-    total=False,
 )
 
-
-class TrialSourceTypeDef(_RequiredTrialSourceTypeDef, _OptionalTrialSourceTypeDef):
-    pass
-
-
 DescribeUserProfileRequestRequestTypeDef = TypedDict(
     "DescribeUserProfileRequestRequestTypeDef",
     {
         "DomainId": str,
         "UserProfileName": str,
     },
 )
@@ -5069,67 +4794,41 @@
     {
         "MaxConcurrency": int,
         "ProvisionedConcurrency": int,
     },
     total=False,
 )
 
-_RequiredDeviceDeploymentSummaryTypeDef = TypedDict(
-    "_RequiredDeviceDeploymentSummaryTypeDef",
+DeviceDeploymentSummaryTypeDef = TypedDict(
+    "DeviceDeploymentSummaryTypeDef",
     {
         "EdgeDeploymentPlanArn": str,
         "EdgeDeploymentPlanName": str,
         "StageName": str,
-        "DeviceName": str,
-        "DeviceArn": str,
-    },
-)
-_OptionalDeviceDeploymentSummaryTypeDef = TypedDict(
-    "_OptionalDeviceDeploymentSummaryTypeDef",
-    {
         "DeployedStageName": str,
         "DeviceFleetName": str,
+        "DeviceName": str,
+        "DeviceArn": str,
         "DeviceDeploymentStatus": DeviceDeploymentStatusType,
         "DeviceDeploymentStatusMessage": str,
         "Description": str,
         "DeploymentStartTime": datetime,
     },
-    total=False,
 )
 
-
-class DeviceDeploymentSummaryTypeDef(
-    _RequiredDeviceDeploymentSummaryTypeDef, _OptionalDeviceDeploymentSummaryTypeDef
-):
-    pass
-
-
-_RequiredDeviceFleetSummaryTypeDef = TypedDict(
-    "_RequiredDeviceFleetSummaryTypeDef",
+DeviceFleetSummaryTypeDef = TypedDict(
+    "DeviceFleetSummaryTypeDef",
     {
         "DeviceFleetArn": str,
         "DeviceFleetName": str,
-    },
-)
-_OptionalDeviceFleetSummaryTypeDef = TypedDict(
-    "_OptionalDeviceFleetSummaryTypeDef",
-    {
         "CreationTime": datetime,
         "LastModifiedTime": datetime,
     },
-    total=False,
 )
 
-
-class DeviceFleetSummaryTypeDef(
-    _RequiredDeviceFleetSummaryTypeDef, _OptionalDeviceFleetSummaryTypeDef
-):
-    pass
-
-
 DeviceStatsTypeDef = TypedDict(
     "DeviceStatsTypeDef",
     {
         "ConnectedDeviceCount": int,
         "RegisteredDeviceCount": int,
     },
 )
@@ -5186,15 +4885,14 @@
         "DomainId": str,
         "DomainName": str,
         "Status": DomainStatusType,
         "CreationTime": datetime,
         "LastModifiedTime": datetime,
         "Url": str,
     },
-    total=False,
 )
 
 _RequiredFileSourceTypeDef = TypedDict(
     "_RequiredFileSourceTypeDef",
     {
         "S3Uri": str,
     },
@@ -5217,91 +4915,63 @@
     "EMRStepMetadataTypeDef",
     {
         "ClusterId": str,
         "StepId": str,
         "StepName": str,
         "LogFilePath": str,
     },
-    total=False,
 )
 
-_RequiredEdgeDeploymentPlanSummaryTypeDef = TypedDict(
-    "_RequiredEdgeDeploymentPlanSummaryTypeDef",
+EdgeDeploymentPlanSummaryTypeDef = TypedDict(
+    "EdgeDeploymentPlanSummaryTypeDef",
     {
         "EdgeDeploymentPlanArn": str,
         "EdgeDeploymentPlanName": str,
         "DeviceFleetName": str,
         "EdgeDeploymentSuccess": int,
         "EdgeDeploymentPending": int,
         "EdgeDeploymentFailed": int,
-    },
-)
-_OptionalEdgeDeploymentPlanSummaryTypeDef = TypedDict(
-    "_OptionalEdgeDeploymentPlanSummaryTypeDef",
-    {
         "CreationTime": datetime,
         "LastModifiedTime": datetime,
     },
-    total=False,
 )
 
-
-class EdgeDeploymentPlanSummaryTypeDef(
-    _RequiredEdgeDeploymentPlanSummaryTypeDef, _OptionalEdgeDeploymentPlanSummaryTypeDef
-):
-    pass
-
-
 EdgeModelStatTypeDef = TypedDict(
     "EdgeModelStatTypeDef",
     {
         "ModelName": str,
         "ModelVersion": str,
         "OfflineDeviceCount": int,
         "ConnectedDeviceCount": int,
         "ActiveDeviceCount": int,
         "SamplingDeviceCount": int,
     },
 )
 
-_RequiredEdgePackagingJobSummaryTypeDef = TypedDict(
-    "_RequiredEdgePackagingJobSummaryTypeDef",
+EdgePackagingJobSummaryTypeDef = TypedDict(
+    "EdgePackagingJobSummaryTypeDef",
     {
         "EdgePackagingJobArn": str,
         "EdgePackagingJobName": str,
         "EdgePackagingJobStatus": EdgePackagingJobStatusType,
-    },
-)
-_OptionalEdgePackagingJobSummaryTypeDef = TypedDict(
-    "_OptionalEdgePackagingJobSummaryTypeDef",
-    {
         "CompilationJobName": str,
         "ModelName": str,
         "ModelVersion": str,
         "CreationTime": datetime,
         "LastModifiedTime": datetime,
     },
-    total=False,
 )
 
-
-class EdgePackagingJobSummaryTypeDef(
-    _RequiredEdgePackagingJobSummaryTypeDef, _OptionalEdgePackagingJobSummaryTypeDef
-):
-    pass
-
-
 EdgeTypeDef = TypedDict(
     "EdgeTypeDef",
     {
         "SourceArn": str,
         "DestinationArn": str,
         "AssociationType": AssociationEdgeTypeType,
     },
-    total=False,
 )
 
 EmptyResponseMetadataTypeDef = TypedDict(
     "EmptyResponseMetadataTypeDef",
     {
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -5375,15 +5045,14 @@
 )
 
 FailStepMetadataTypeDef = TypedDict(
     "FailStepMetadataTypeDef",
     {
         "ErrorMessage": str,
     },
-    total=False,
 )
 
 FileSystemConfigTypeDef = TypedDict(
     "FileSystemConfigTypeDef",
     {
         "MountPath": str,
         "DefaultUid": int,
@@ -5408,61 +5077,34 @@
 )
 
 
 class FilterTypeDef(_RequiredFilterTypeDef, _OptionalFilterTypeDef):
     pass
 
 
-_RequiredFinalHyperParameterTuningJobObjectiveMetricTypeDef = TypedDict(
-    "_RequiredFinalHyperParameterTuningJobObjectiveMetricTypeDef",
+FinalHyperParameterTuningJobObjectiveMetricTypeDef = TypedDict(
+    "FinalHyperParameterTuningJobObjectiveMetricTypeDef",
     {
+        "Type": HyperParameterTuningJobObjectiveTypeType,
         "MetricName": str,
         "Value": float,
     },
 )
-_OptionalFinalHyperParameterTuningJobObjectiveMetricTypeDef = TypedDict(
-    "_OptionalFinalHyperParameterTuningJobObjectiveMetricTypeDef",
-    {
-        "Type": HyperParameterTuningJobObjectiveTypeType,
-    },
-    total=False,
-)
-
-
-class FinalHyperParameterTuningJobObjectiveMetricTypeDef(
-    _RequiredFinalHyperParameterTuningJobObjectiveMetricTypeDef,
-    _OptionalFinalHyperParameterTuningJobObjectiveMetricTypeDef,
-):
-    pass
 
-
-_RequiredFlowDefinitionSummaryTypeDef = TypedDict(
-    "_RequiredFlowDefinitionSummaryTypeDef",
+FlowDefinitionSummaryTypeDef = TypedDict(
+    "FlowDefinitionSummaryTypeDef",
     {
         "FlowDefinitionName": str,
         "FlowDefinitionArn": str,
         "FlowDefinitionStatus": FlowDefinitionStatusType,
         "CreationTime": datetime,
-    },
-)
-_OptionalFlowDefinitionSummaryTypeDef = TypedDict(
-    "_OptionalFlowDefinitionSummaryTypeDef",
-    {
         "FailureReason": str,
     },
-    total=False,
 )
 
-
-class FlowDefinitionSummaryTypeDef(
-    _RequiredFlowDefinitionSummaryTypeDef, _OptionalFlowDefinitionSummaryTypeDef
-):
-    pass
-
-
 GetDeviceFleetReportRequestRequestTypeDef = TypedDict(
     "GetDeviceFleetReportRequestRequestTypeDef",
     {
         "DeviceFleetName": str,
     },
 )
 
@@ -5506,77 +5148,54 @@
 )
 
 PropertyNameSuggestionTypeDef = TypedDict(
     "PropertyNameSuggestionTypeDef",
     {
         "PropertyName": str,
     },
-    total=False,
 )
 
 GitConfigForUpdateTypeDef = TypedDict(
     "GitConfigForUpdateTypeDef",
     {
         "SecretArn": str,
     },
     total=False,
 )
 
-_RequiredHubContentInfoTypeDef = TypedDict(
-    "_RequiredHubContentInfoTypeDef",
+HubContentInfoTypeDef = TypedDict(
+    "HubContentInfoTypeDef",
     {
         "HubContentName": str,
         "HubContentArn": str,
         "HubContentVersion": str,
         "HubContentType": HubContentTypeType,
         "DocumentSchemaVersion": str,
-        "HubContentStatus": HubContentStatusType,
-        "CreationTime": datetime,
-    },
-)
-_OptionalHubContentInfoTypeDef = TypedDict(
-    "_OptionalHubContentInfoTypeDef",
-    {
         "HubContentDisplayName": str,
         "HubContentDescription": str,
         "HubContentSearchKeywords": List[str],
+        "HubContentStatus": HubContentStatusType,
+        "CreationTime": datetime,
     },
-    total=False,
 )
 
-
-class HubContentInfoTypeDef(_RequiredHubContentInfoTypeDef, _OptionalHubContentInfoTypeDef):
-    pass
-
-
-_RequiredHubInfoTypeDef = TypedDict(
-    "_RequiredHubInfoTypeDef",
+HubInfoTypeDef = TypedDict(
+    "HubInfoTypeDef",
     {
         "HubName": str,
         "HubArn": str,
-        "HubStatus": HubStatusType,
-        "CreationTime": datetime,
-        "LastModifiedTime": datetime,
-    },
-)
-_OptionalHubInfoTypeDef = TypedDict(
-    "_OptionalHubInfoTypeDef",
-    {
         "HubDisplayName": str,
         "HubDescription": str,
         "HubSearchKeywords": List[str],
+        "HubStatus": HubStatusType,
+        "CreationTime": datetime,
+        "LastModifiedTime": datetime,
     },
-    total=False,
 )
 
-
-class HubInfoTypeDef(_RequiredHubInfoTypeDef, _OptionalHubInfoTypeDef):
-    pass
-
-
 HumanLoopActivationConditionsConfigTypeDef = TypedDict(
     "HumanLoopActivationConditionsConfigTypeDef",
     {
         "HumanLoopActivationConditions": str,
     },
 )
 
@@ -5655,140 +5274,91 @@
 IamIdentityTypeDef = TypedDict(
     "IamIdentityTypeDef",
     {
         "Arn": str,
         "PrincipalId": str,
         "SourceIdentity": str,
     },
-    total=False,
 )
 
 RepositoryAuthConfigTypeDef = TypedDict(
     "RepositoryAuthConfigTypeDef",
     {
         "RepositoryCredentialsProviderArn": str,
     },
 )
 
-_RequiredImageTypeDef = TypedDict(
-    "_RequiredImageTypeDef",
+ImageTypeDef = TypedDict(
+    "ImageTypeDef",
     {
         "CreationTime": datetime,
+        "Description": str,
+        "DisplayName": str,
+        "FailureReason": str,
         "ImageArn": str,
         "ImageName": str,
         "ImageStatus": ImageStatusType,
         "LastModifiedTime": datetime,
     },
 )
-_OptionalImageTypeDef = TypedDict(
-    "_OptionalImageTypeDef",
-    {
-        "Description": str,
-        "DisplayName": str,
-        "FailureReason": str,
-    },
-    total=False,
-)
-
-
-class ImageTypeDef(_RequiredImageTypeDef, _OptionalImageTypeDef):
-    pass
-
 
-_RequiredImageVersionTypeDef = TypedDict(
-    "_RequiredImageVersionTypeDef",
+ImageVersionTypeDef = TypedDict(
+    "ImageVersionTypeDef",
     {
         "CreationTime": datetime,
+        "FailureReason": str,
         "ImageArn": str,
         "ImageVersionArn": str,
         "ImageVersionStatus": ImageVersionStatusType,
         "LastModifiedTime": datetime,
         "Version": int,
     },
 )
-_OptionalImageVersionTypeDef = TypedDict(
-    "_OptionalImageVersionTypeDef",
-    {
-        "FailureReason": str,
-    },
-    total=False,
-)
-
-
-class ImageVersionTypeDef(_RequiredImageVersionTypeDef, _OptionalImageVersionTypeDef):
-    pass
-
 
 ImportHubContentResponseTypeDef = TypedDict(
     "ImportHubContentResponseTypeDef",
     {
         "HubArn": str,
         "HubContentArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredRecommendationMetricsTypeDef = TypedDict(
-    "_RequiredRecommendationMetricsTypeDef",
+RecommendationMetricsTypeDef = TypedDict(
+    "RecommendationMetricsTypeDef",
     {
         "CostPerHour": float,
         "CostPerInference": float,
         "MaxInvocations": int,
         "ModelLatency": int,
-    },
-)
-_OptionalRecommendationMetricsTypeDef = TypedDict(
-    "_OptionalRecommendationMetricsTypeDef",
-    {
         "CpuUtilization": float,
         "MemoryUtilization": float,
         "ModelSetupTime": int,
     },
-    total=False,
 )
 
-
-class RecommendationMetricsTypeDef(
-    _RequiredRecommendationMetricsTypeDef, _OptionalRecommendationMetricsTypeDef
-):
-    pass
-
-
-_RequiredInferenceRecommendationsJobTypeDef = TypedDict(
-    "_RequiredInferenceRecommendationsJobTypeDef",
+InferenceRecommendationsJobTypeDef = TypedDict(
+    "InferenceRecommendationsJobTypeDef",
     {
         "JobName": str,
         "JobDescription": str,
         "JobType": RecommendationJobTypeType,
         "JobArn": str,
         "Status": RecommendationJobStatusType,
         "CreationTime": datetime,
+        "CompletionTime": datetime,
         "RoleArn": str,
         "LastModifiedTime": datetime,
-    },
-)
-_OptionalInferenceRecommendationsJobTypeDef = TypedDict(
-    "_OptionalInferenceRecommendationsJobTypeDef",
-    {
-        "CompletionTime": datetime,
         "FailureReason": str,
         "ModelName": str,
         "SamplePayloadUrl": str,
         "ModelPackageVersionArn": str,
     },
-    total=False,
 )
 
-
-class InferenceRecommendationsJobTypeDef(
-    _RequiredInferenceRecommendationsJobTypeDef, _OptionalInferenceRecommendationsJobTypeDef
-):
-    pass
-
-
 InstanceGroupTypeDef = TypedDict(
     "InstanceGroupTypeDef",
     {
         "InstanceType": TrainingInstanceTypeType,
         "InstanceCount": int,
         "InstanceGroupName": str,
     },
@@ -5847,15 +5417,14 @@
 LabelCountersForWorkteamTypeDef = TypedDict(
     "LabelCountersForWorkteamTypeDef",
     {
         "HumanLabeled": int,
         "PendingHuman": int,
         "Total": int,
     },
-    total=False,
 )
 
 LabelingJobDataAttributesTypeDef = TypedDict(
     "LabelingJobDataAttributesTypeDef",
     {
         "ContentClassifiers": Sequence[ContentClassifierType],
     },
@@ -5881,15 +5450,14 @@
     {
         "LineageGroupArn": str,
         "LineageGroupName": str,
         "DisplayName": str,
         "CreationTime": datetime,
         "LastModifiedTime": datetime,
     },
-    total=False,
 )
 
 ListActionsRequestListActionsPaginateTypeDef = TypedDict(
     "ListActionsRequestListActionsPaginateTypeDef",
     {
         "SourceUri": str,
         "ActionType": str,
@@ -7224,39 +6792,26 @@
 class ListModelCardVersionsRequestRequestTypeDef(
     _RequiredListModelCardVersionsRequestRequestTypeDef,
     _OptionalListModelCardVersionsRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredModelCardVersionSummaryTypeDef = TypedDict(
-    "_RequiredModelCardVersionSummaryTypeDef",
+ModelCardVersionSummaryTypeDef = TypedDict(
+    "ModelCardVersionSummaryTypeDef",
     {
         "ModelCardName": str,
         "ModelCardArn": str,
         "ModelCardStatus": ModelCardStatusType,
         "ModelCardVersion": int,
         "CreationTime": datetime,
-    },
-)
-_OptionalModelCardVersionSummaryTypeDef = TypedDict(
-    "_OptionalModelCardVersionSummaryTypeDef",
-    {
         "LastModifiedTime": datetime,
     },
-    total=False,
 )
 
-
-class ModelCardVersionSummaryTypeDef(
-    _RequiredModelCardVersionSummaryTypeDef, _OptionalModelCardVersionSummaryTypeDef
-):
-    pass
-
-
 ListModelCardsRequestListModelCardsPaginateTypeDef = TypedDict(
     "ListModelCardsRequestListModelCardsPaginateTypeDef",
     {
         "CreationTimeAfter": Union[datetime, str],
         "CreationTimeBefore": Union[datetime, str],
         "NameContains": str,
         "ModelCardStatus": ModelCardStatusType,
@@ -7278,36 +6833,25 @@
         "NextToken": str,
         "SortBy": ModelCardSortByType,
         "SortOrder": ModelCardSortOrderType,
     },
     total=False,
 )
 
-_RequiredModelCardSummaryTypeDef = TypedDict(
-    "_RequiredModelCardSummaryTypeDef",
+ModelCardSummaryTypeDef = TypedDict(
+    "ModelCardSummaryTypeDef",
     {
         "ModelCardName": str,
         "ModelCardArn": str,
         "ModelCardStatus": ModelCardStatusType,
         "CreationTime": datetime,
-    },
-)
-_OptionalModelCardSummaryTypeDef = TypedDict(
-    "_OptionalModelCardSummaryTypeDef",
-    {
         "LastModifiedTime": datetime,
     },
-    total=False,
 )
 
-
-class ModelCardSummaryTypeDef(_RequiredModelCardSummaryTypeDef, _OptionalModelCardSummaryTypeDef):
-    pass
-
-
 ListModelExplainabilityJobDefinitionsRequestListModelExplainabilityJobDefinitionsPaginateTypeDef = TypedDict(
     "ListModelExplainabilityJobDefinitionsRequestListModelExplainabilityJobDefinitionsPaginateTypeDef",
     {
         "EndpointName": str,
         "SortBy": MonitoringJobDefinitionSortKeyType,
         "SortOrder": SortOrderType,
         "NameContains": str,
@@ -7367,37 +6911,24 @@
         "NextToken": str,
         "SortBy": ModelPackageGroupSortByType,
         "SortOrder": SortOrderType,
     },
     total=False,
 )
 
-_RequiredModelPackageGroupSummaryTypeDef = TypedDict(
-    "_RequiredModelPackageGroupSummaryTypeDef",
+ModelPackageGroupSummaryTypeDef = TypedDict(
+    "ModelPackageGroupSummaryTypeDef",
     {
         "ModelPackageGroupName": str,
         "ModelPackageGroupArn": str,
+        "ModelPackageGroupDescription": str,
         "CreationTime": datetime,
         "ModelPackageGroupStatus": ModelPackageGroupStatusType,
     },
 )
-_OptionalModelPackageGroupSummaryTypeDef = TypedDict(
-    "_OptionalModelPackageGroupSummaryTypeDef",
-    {
-        "ModelPackageGroupDescription": str,
-    },
-    total=False,
-)
-
-
-class ModelPackageGroupSummaryTypeDef(
-    _RequiredModelPackageGroupSummaryTypeDef, _OptionalModelPackageGroupSummaryTypeDef
-):
-    pass
-
 
 ListModelPackagesInputListModelPackagesPaginateTypeDef = TypedDict(
     "ListModelPackagesInputListModelPackagesPaginateTypeDef",
     {
         "CreationTimeAfter": Union[datetime, str],
         "CreationTimeBefore": Union[datetime, str],
         "NameContains": str,
@@ -7424,41 +6955,28 @@
         "NextToken": str,
         "SortBy": ModelPackageSortByType,
         "SortOrder": SortOrderType,
     },
     total=False,
 )
 
-_RequiredModelPackageSummaryTypeDef = TypedDict(
-    "_RequiredModelPackageSummaryTypeDef",
+ModelPackageSummaryTypeDef = TypedDict(
+    "ModelPackageSummaryTypeDef",
     {
         "ModelPackageName": str,
-        "ModelPackageArn": str,
-        "CreationTime": datetime,
-        "ModelPackageStatus": ModelPackageStatusType,
-    },
-)
-_OptionalModelPackageSummaryTypeDef = TypedDict(
-    "_OptionalModelPackageSummaryTypeDef",
-    {
         "ModelPackageGroupName": str,
         "ModelPackageVersion": int,
+        "ModelPackageArn": str,
         "ModelPackageDescription": str,
+        "CreationTime": datetime,
+        "ModelPackageStatus": ModelPackageStatusType,
         "ModelApprovalStatus": ModelApprovalStatusType,
     },
-    total=False,
 )
 
-
-class ModelPackageSummaryTypeDef(
-    _RequiredModelPackageSummaryTypeDef, _OptionalModelPackageSummaryTypeDef
-):
-    pass
-
-
 ListModelQualityJobDefinitionsRequestListModelQualityJobDefinitionsPaginateTypeDef = TypedDict(
     "ListModelQualityJobDefinitionsRequestListModelQualityJobDefinitionsPaginateTypeDef",
     {
         "EndpointName": str,
         "SortBy": MonitoringJobDefinitionSortKeyType,
         "SortOrder": SortOrderType,
         "NameContains": str,
@@ -7684,41 +7202,28 @@
         "StatusEquals": ScheduleStatusType,
         "MonitoringJobDefinitionName": str,
         "MonitoringTypeEquals": MonitoringTypeType,
     },
     total=False,
 )
 
-_RequiredMonitoringScheduleSummaryTypeDef = TypedDict(
-    "_RequiredMonitoringScheduleSummaryTypeDef",
+MonitoringScheduleSummaryTypeDef = TypedDict(
+    "MonitoringScheduleSummaryTypeDef",
     {
         "MonitoringScheduleName": str,
         "MonitoringScheduleArn": str,
         "CreationTime": datetime,
         "LastModifiedTime": datetime,
         "MonitoringScheduleStatus": ScheduleStatusType,
-    },
-)
-_OptionalMonitoringScheduleSummaryTypeDef = TypedDict(
-    "_OptionalMonitoringScheduleSummaryTypeDef",
-    {
         "EndpointName": str,
         "MonitoringJobDefinitionName": str,
         "MonitoringType": MonitoringTypeType,
     },
-    total=False,
 )
 
-
-class MonitoringScheduleSummaryTypeDef(
-    _RequiredMonitoringScheduleSummaryTypeDef, _OptionalMonitoringScheduleSummaryTypeDef
-):
-    pass
-
-
 ListNotebookInstanceLifecycleConfigsInputListNotebookInstanceLifecycleConfigsPaginateTypeDef = TypedDict(
     "ListNotebookInstanceLifecycleConfigsInputListNotebookInstanceLifecycleConfigsPaginateTypeDef",
     {
         "SortBy": NotebookInstanceLifecycleConfigSortKeyType,
         "SortOrder": NotebookInstanceLifecycleConfigSortOrderType,
         "NameContains": str,
         "CreationTimeBefore": Union[datetime, str],
@@ -7742,38 +7247,24 @@
         "CreationTimeAfter": Union[datetime, str],
         "LastModifiedTimeBefore": Union[datetime, str],
         "LastModifiedTimeAfter": Union[datetime, str],
     },
     total=False,
 )
 
-_RequiredNotebookInstanceLifecycleConfigSummaryTypeDef = TypedDict(
-    "_RequiredNotebookInstanceLifecycleConfigSummaryTypeDef",
+NotebookInstanceLifecycleConfigSummaryTypeDef = TypedDict(
+    "NotebookInstanceLifecycleConfigSummaryTypeDef",
     {
         "NotebookInstanceLifecycleConfigName": str,
         "NotebookInstanceLifecycleConfigArn": str,
-    },
-)
-_OptionalNotebookInstanceLifecycleConfigSummaryTypeDef = TypedDict(
-    "_OptionalNotebookInstanceLifecycleConfigSummaryTypeDef",
-    {
         "CreationTime": datetime,
         "LastModifiedTime": datetime,
     },
-    total=False,
 )
 
-
-class NotebookInstanceLifecycleConfigSummaryTypeDef(
-    _RequiredNotebookInstanceLifecycleConfigSummaryTypeDef,
-    _OptionalNotebookInstanceLifecycleConfigSummaryTypeDef,
-):
-    pass
-
-
 ListNotebookInstancesInputListNotebookInstancesPaginateTypeDef = TypedDict(
     "ListNotebookInstancesInputListNotebookInstancesPaginateTypeDef",
     {
         "SortBy": NotebookInstanceSortKeyType,
         "SortOrder": NotebookInstanceSortOrderType,
         "NameContains": str,
         "CreationTimeBefore": Union[datetime, str],
@@ -7805,43 +7296,30 @@
         "NotebookInstanceLifecycleConfigNameContains": str,
         "DefaultCodeRepositoryContains": str,
         "AdditionalCodeRepositoryEquals": str,
     },
     total=False,
 )
 
-_RequiredNotebookInstanceSummaryTypeDef = TypedDict(
-    "_RequiredNotebookInstanceSummaryTypeDef",
+NotebookInstanceSummaryTypeDef = TypedDict(
+    "NotebookInstanceSummaryTypeDef",
     {
         "NotebookInstanceName": str,
         "NotebookInstanceArn": str,
-    },
-)
-_OptionalNotebookInstanceSummaryTypeDef = TypedDict(
-    "_OptionalNotebookInstanceSummaryTypeDef",
-    {
         "NotebookInstanceStatus": NotebookInstanceStatusType,
         "Url": str,
         "InstanceType": InstanceTypeType,
         "CreationTime": datetime,
         "LastModifiedTime": datetime,
         "NotebookInstanceLifecycleConfigName": str,
         "DefaultCodeRepository": str,
         "AdditionalCodeRepositories": List[str],
     },
-    total=False,
 )
 
-
-class NotebookInstanceSummaryTypeDef(
-    _RequiredNotebookInstanceSummaryTypeDef, _OptionalNotebookInstanceSummaryTypeDef
-):
-    pass
-
-
 ListPipelineExecutionStepsRequestListPipelineExecutionStepsPaginateTypeDef = TypedDict(
     "ListPipelineExecutionStepsRequestListPipelineExecutionStepsPaginateTypeDef",
     {
         "PipelineExecutionArn": str,
         "SortOrder": SortOrderType,
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
@@ -7918,15 +7396,14 @@
         "PipelineExecutionArn": str,
         "StartTime": datetime,
         "PipelineExecutionStatus": PipelineExecutionStatusType,
         "PipelineExecutionDescription": str,
         "PipelineExecutionDisplayName": str,
         "PipelineExecutionFailureReason": str,
     },
-    total=False,
 )
 
 _RequiredListPipelineParametersForExecutionRequestListPipelineParametersForExecutionPaginateTypeDef = TypedDict(
     "_RequiredListPipelineParametersForExecutionRequestListPipelineParametersForExecutionPaginateTypeDef",
     {
         "PipelineExecutionArn": str,
     },
@@ -8013,15 +7490,14 @@
         "PipelineDisplayName": str,
         "PipelineDescription": str,
         "RoleArn": str,
         "CreationTime": datetime,
         "LastModifiedTime": datetime,
         "LastExecutionTime": datetime,
     },
-    total=False,
 )
 
 ListProcessingJobsRequestListProcessingJobsPaginateTypeDef = TypedDict(
     "ListProcessingJobsRequestListProcessingJobsPaginateTypeDef",
     {
         "CreationTimeAfter": Union[datetime, str],
         "CreationTimeBefore": Union[datetime, str],
@@ -8049,77 +7525,53 @@
         "SortOrder": SortOrderType,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-_RequiredProcessingJobSummaryTypeDef = TypedDict(
-    "_RequiredProcessingJobSummaryTypeDef",
+ProcessingJobSummaryTypeDef = TypedDict(
+    "ProcessingJobSummaryTypeDef",
     {
         "ProcessingJobName": str,
         "ProcessingJobArn": str,
         "CreationTime": datetime,
-        "ProcessingJobStatus": ProcessingJobStatusType,
-    },
-)
-_OptionalProcessingJobSummaryTypeDef = TypedDict(
-    "_OptionalProcessingJobSummaryTypeDef",
-    {
         "ProcessingEndTime": datetime,
         "LastModifiedTime": datetime,
+        "ProcessingJobStatus": ProcessingJobStatusType,
         "FailureReason": str,
         "ExitMessage": str,
     },
-    total=False,
 )
 
-
-class ProcessingJobSummaryTypeDef(
-    _RequiredProcessingJobSummaryTypeDef, _OptionalProcessingJobSummaryTypeDef
-):
-    pass
-
-
 ListProjectsInputRequestTypeDef = TypedDict(
     "ListProjectsInputRequestTypeDef",
     {
         "CreationTimeAfter": Union[datetime, str],
         "CreationTimeBefore": Union[datetime, str],
         "MaxResults": int,
         "NameContains": str,
         "NextToken": str,
         "SortBy": ProjectSortByType,
         "SortOrder": ProjectSortOrderType,
     },
     total=False,
 )
 
-_RequiredProjectSummaryTypeDef = TypedDict(
-    "_RequiredProjectSummaryTypeDef",
+ProjectSummaryTypeDef = TypedDict(
+    "ProjectSummaryTypeDef",
     {
         "ProjectName": str,
+        "ProjectDescription": str,
         "ProjectArn": str,
         "ProjectId": str,
         "CreationTime": datetime,
         "ProjectStatus": ProjectStatusType,
     },
 )
-_OptionalProjectSummaryTypeDef = TypedDict(
-    "_OptionalProjectSummaryTypeDef",
-    {
-        "ProjectDescription": str,
-    },
-    total=False,
-)
-
-
-class ProjectSummaryTypeDef(_RequiredProjectSummaryTypeDef, _OptionalProjectSummaryTypeDef):
-    pass
-
 
 ListSpacesRequestListSpacesPaginateTypeDef = TypedDict(
     "ListSpacesRequestListSpacesPaginateTypeDef",
     {
         "SortOrder": SortOrderType,
         "SortBy": SpaceSortKeyType,
         "DomainIdEquals": str,
@@ -8147,15 +7599,14 @@
     {
         "DomainId": str,
         "SpaceName": str,
         "Status": SpaceStatusType,
         "CreationTime": datetime,
         "LastModifiedTime": datetime,
     },
-    total=False,
 )
 
 _RequiredListStageDevicesRequestListStageDevicesPaginateTypeDef = TypedDict(
     "_RequiredListStageDevicesRequestListStageDevicesPaginateTypeDef",
     {
         "EdgeDeploymentPlanName": str,
         "StageName": str,
@@ -8240,15 +7691,14 @@
     {
         "StudioLifecycleConfigArn": str,
         "StudioLifecycleConfigName": str,
         "CreationTime": datetime,
         "LastModifiedTime": datetime,
         "StudioLifecycleConfigAppType": StudioLifecycleConfigAppTypeType,
     },
-    total=False,
 )
 
 ListSubscribedWorkteamsRequestListSubscribedWorkteamsPaginateTypeDef = TypedDict(
     "ListSubscribedWorkteamsRequestListSubscribedWorkteamsPaginateTypeDef",
     {
         "NameContains": str,
         "PaginationConfig": "PaginatorConfigTypeDef",
@@ -8424,40 +7874,27 @@
         "SortOrder": SortOrderType,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-_RequiredTransformJobSummaryTypeDef = TypedDict(
-    "_RequiredTransformJobSummaryTypeDef",
+TransformJobSummaryTypeDef = TypedDict(
+    "TransformJobSummaryTypeDef",
     {
         "TransformJobName": str,
         "TransformJobArn": str,
         "CreationTime": datetime,
-        "TransformJobStatus": TransformJobStatusType,
-    },
-)
-_OptionalTransformJobSummaryTypeDef = TypedDict(
-    "_OptionalTransformJobSummaryTypeDef",
-    {
         "TransformEndTime": datetime,
         "LastModifiedTime": datetime,
+        "TransformJobStatus": TransformJobStatusType,
         "FailureReason": str,
     },
-    total=False,
 )
 
-
-class TransformJobSummaryTypeDef(
-    _RequiredTransformJobSummaryTypeDef, _OptionalTransformJobSummaryTypeDef
-):
-    pass
-
-
 ListTrialComponentsRequestListTrialComponentsPaginateTypeDef = TypedDict(
     "ListTrialComponentsRequestListTrialComponentsPaginateTypeDef",
     {
         "ExperimentName": str,
         "TrialName": str,
         "SourceArn": str,
         "CreatedAfter": Union[datetime, str],
@@ -8544,15 +7981,14 @@
     {
         "DomainId": str,
         "UserProfileName": str,
         "Status": UserProfileStatusType,
         "CreationTime": datetime,
         "LastModifiedTime": datetime,
     },
-    total=False,
 )
 
 ListWorkforcesRequestListWorkforcesPaginateTypeDef = TypedDict(
     "ListWorkforcesRequestListWorkforcesPaginateTypeDef",
     {
         "SortBy": ListWorkforcesSortByOptionsType,
         "SortOrder": SortOrderType,
@@ -8624,15 +8060,14 @@
 )
 
 ModelDashboardIndicatorActionTypeDef = TypedDict(
     "ModelDashboardIndicatorActionTypeDef",
     {
         "Enabled": bool,
     },
-    total=False,
 )
 
 S3ModelDataSourceTypeDef = TypedDict(
     "S3ModelDataSourceTypeDef",
     {
         "S3Uri": str,
         "S3DataType": S3ModelDataTypeType,
@@ -8668,42 +8103,28 @@
     "ModelMetadataFilterTypeDef",
     {
         "Name": ModelMetadataFilterTypeType,
         "Value": str,
     },
 )
 
-_RequiredModelPackageStatusItemTypeDef = TypedDict(
-    "_RequiredModelPackageStatusItemTypeDef",
+ModelPackageStatusItemTypeDef = TypedDict(
+    "ModelPackageStatusItemTypeDef",
     {
         "Name": str,
         "Status": DetailedModelPackageStatusType,
-    },
-)
-_OptionalModelPackageStatusItemTypeDef = TypedDict(
-    "_OptionalModelPackageStatusItemTypeDef",
-    {
         "FailureReason": str,
     },
-    total=False,
 )
 
-
-class ModelPackageStatusItemTypeDef(
-    _RequiredModelPackageStatusItemTypeDef, _OptionalModelPackageStatusItemTypeDef
-):
-    pass
-
-
 ModelStepMetadataTypeDef = TypedDict(
     "ModelStepMetadataTypeDef",
     {
         "Arn": str,
     },
-    total=False,
 )
 
 _RequiredMonitoringAppSpecificationTypeDef = TypedDict(
     "_RequiredMonitoringAppSpecificationTypeDef",
     {
         "ImageUri": str,
     },
@@ -8821,15 +8242,14 @@
         "Issuer": str,
         "AuthorizationEndpoint": str,
         "TokenEndpoint": str,
         "UserInfoEndpoint": str,
         "LogoutEndpoint": str,
         "JwksUri": str,
     },
-    total=False,
 )
 
 OnlineStoreSecurityConfigTypeDef = TypedDict(
     "OnlineStoreSecurityConfigTypeDef",
     {
         "KmsKeyId": str,
     },
@@ -8877,39 +8297,25 @@
 
 ParentTypeDef = TypedDict(
     "ParentTypeDef",
     {
         "TrialName": str,
         "ExperimentName": str,
     },
-    total=False,
 )
 
-_RequiredProductionVariantStatusTypeDef = TypedDict(
-    "_RequiredProductionVariantStatusTypeDef",
+ProductionVariantStatusTypeDef = TypedDict(
+    "ProductionVariantStatusTypeDef",
     {
         "Status": VariantStatusType,
-    },
-)
-_OptionalProductionVariantStatusTypeDef = TypedDict(
-    "_OptionalProductionVariantStatusTypeDef",
-    {
         "StatusMessage": str,
         "StartTime": datetime,
     },
-    total=False,
 )
 
-
-class ProductionVariantStatusTypeDef(
-    _RequiredProductionVariantStatusTypeDef, _OptionalProductionVariantStatusTypeDef
-):
-    pass
-
-
 PhaseTypeDef = TypedDict(
     "PhaseTypeDef",
     {
         "InitialNumberOfUsers": int,
         "SpawnRate": int,
         "DurationInSeconds": int,
     },
@@ -8917,15 +8323,14 @@
 )
 
 ProcessingJobStepMetadataTypeDef = TypedDict(
     "ProcessingJobStepMetadataTypeDef",
     {
         "Arn": str,
     },
-    total=False,
 )
 
 QualityCheckStepMetadataTypeDef = TypedDict(
     "QualityCheckStepMetadataTypeDef",
     {
         "CheckType": str,
         "BaselineUsedForDriftCheckStatistics": str,
@@ -8934,55 +8339,49 @@
         "CalculatedBaselineConstraints": str,
         "ModelPackageGroupName": str,
         "ViolationReport": str,
         "CheckJobArn": str,
         "SkipCheck": bool,
         "RegisterNewBaseline": bool,
     },
-    total=False,
 )
 
 RegisterModelStepMetadataTypeDef = TypedDict(
     "RegisterModelStepMetadataTypeDef",
     {
         "Arn": str,
     },
-    total=False,
 )
 
 TrainingJobStepMetadataTypeDef = TypedDict(
     "TrainingJobStepMetadataTypeDef",
     {
         "Arn": str,
     },
-    total=False,
 )
 
 TransformJobStepMetadataTypeDef = TypedDict(
     "TransformJobStepMetadataTypeDef",
     {
         "Arn": str,
     },
-    total=False,
 )
 
 TuningJobStepMetaDataTypeDef = TypedDict(
     "TuningJobStepMetaDataTypeDef",
     {
         "Arn": str,
     },
-    total=False,
 )
 
 SelectiveExecutionResultTypeDef = TypedDict(
     "SelectiveExecutionResultTypeDef",
     {
         "SourcePipelineExecutionArn": str,
     },
-    total=False,
 )
 
 _RequiredProcessingClusterConfigTypeDef = TypedDict(
     "_RequiredProcessingClusterConfigTypeDef",
     {
         "InstanceCount": int,
         "InstanceType": ProcessingInstanceTypeType,
@@ -9136,15 +8535,14 @@
 VertexTypeDef = TypedDict(
     "VertexTypeDef",
     {
         "Arn": str,
         "Type": str,
         "LineageType": LineageTypeType,
     },
-    total=False,
 )
 
 RStudioServerProAppSettingsTypeDef = TypedDict(
     "RStudioServerProAppSettingsTypeDef",
     {
         "AccessStatus": RStudioServerProAccessStatusType,
         "UserGroup": RStudioServerProUserGroupType,
@@ -9994,49 +9392,35 @@
     "UpdateUserProfileResponseTypeDef",
     {
         "UserProfileArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredWorkforceVpcConfigResponseTypeDef = TypedDict(
-    "_RequiredWorkforceVpcConfigResponseTypeDef",
+WorkforceVpcConfigResponseTypeDef = TypedDict(
+    "WorkforceVpcConfigResponseTypeDef",
     {
         "VpcId": str,
         "SecurityGroupIds": List[str],
         "Subnets": List[str],
-    },
-)
-_OptionalWorkforceVpcConfigResponseTypeDef = TypedDict(
-    "_OptionalWorkforceVpcConfigResponseTypeDef",
-    {
         "VpcEndpointId": str,
     },
-    total=False,
 )
 
-
-class WorkforceVpcConfigResponseTypeDef(
-    _RequiredWorkforceVpcConfigResponseTypeDef, _OptionalWorkforceVpcConfigResponseTypeDef
-):
-    pass
-
-
 ActionSummaryTypeDef = TypedDict(
     "ActionSummaryTypeDef",
     {
         "ActionArn": str,
         "ActionName": str,
         "Source": ActionSourceTypeDef,
         "ActionType": str,
         "Status": ActionStatusType,
         "CreationTime": datetime,
         "LastModifiedTime": datetime,
     },
-    total=False,
 )
 
 AddTagsInputRequestTypeDef = TypedDict(
     "AddTagsInputRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Sequence[TagTypeDef],
@@ -10218,15 +9602,14 @@
 
 AlgorithmStatusDetailsTypeDef = TypedDict(
     "AlgorithmStatusDetailsTypeDef",
     {
         "ValidationStatuses": List[AlgorithmStatusItemTypeDef],
         "ImageScanStatuses": List[AlgorithmStatusItemTypeDef],
     },
-    total=False,
 )
 
 ListAlgorithmsOutputTypeDef = TypedDict(
     "ListAlgorithmsOutputTypeDef",
     {
         "AlgorithmSummaryList": List[AlgorithmSummaryTypeDef],
         "NextToken": str,
@@ -10318,49 +9701,36 @@
 ResolvedAttributesTypeDef = TypedDict(
     "ResolvedAttributesTypeDef",
     {
         "AutoMLJobObjective": AutoMLJobObjectiveTypeDef,
         "ProblemType": ProblemTypeType,
         "CompletionCriteria": AutoMLJobCompletionCriteriaTypeDef,
     },
-    total=False,
 )
 
-_RequiredAutoMLJobSummaryTypeDef = TypedDict(
-    "_RequiredAutoMLJobSummaryTypeDef",
+AutoMLJobSummaryTypeDef = TypedDict(
+    "AutoMLJobSummaryTypeDef",
     {
         "AutoMLJobName": str,
         "AutoMLJobArn": str,
         "AutoMLJobStatus": AutoMLJobStatusType,
         "AutoMLJobSecondaryStatus": AutoMLJobSecondaryStatusType,
         "CreationTime": datetime,
-        "LastModifiedTime": datetime,
-    },
-)
-_OptionalAutoMLJobSummaryTypeDef = TypedDict(
-    "_OptionalAutoMLJobSummaryTypeDef",
-    {
         "EndTime": datetime,
+        "LastModifiedTime": datetime,
         "FailureReason": str,
         "PartialFailureReasons": List[AutoMLPartialFailureReasonTypeDef],
     },
-    total=False,
 )
 
-
-class AutoMLJobSummaryTypeDef(_RequiredAutoMLJobSummaryTypeDef, _OptionalAutoMLJobSummaryTypeDef):
-    pass
-
-
 AutoMLProblemTypeResolvedAttributesTypeDef = TypedDict(
     "AutoMLProblemTypeResolvedAttributesTypeDef",
     {
         "TabularResolvedAttributes": TabularResolvedAttributesTypeDef,
     },
-    total=False,
 )
 
 AutoMLSecurityConfigTypeDef = TypedDict(
     "AutoMLSecurityConfigTypeDef",
     {
         "VolumeKmsKeyId": str,
         "EnableInterContainerTrafficEncryption": bool,
@@ -10455,24 +9825,22 @@
 CallbackStepMetadataTypeDef = TypedDict(
     "CallbackStepMetadataTypeDef",
     {
         "CallbackToken": str,
         "SqsQueueUrl": str,
         "OutputParameters": List[OutputParameterTypeDef],
     },
-    total=False,
 )
 
 LambdaStepMetadataTypeDef = TypedDict(
     "LambdaStepMetadataTypeDef",
     {
         "Arn": str,
         "OutputParameters": List[OutputParameterTypeDef],
     },
-    total=False,
 )
 
 _RequiredSendPipelineExecutionStepSuccessRequestRequestTypeDef = TypedDict(
     "_RequiredSendPipelineExecutionStepSuccessRequestRequestTypeDef",
     {
         "CallbackToken": str,
     },
@@ -10496,22 +9864,22 @@
 
 CandidatePropertiesTypeDef = TypedDict(
     "CandidatePropertiesTypeDef",
     {
         "CandidateArtifactLocations": CandidateArtifactLocationsTypeDef,
         "CandidateMetrics": List[MetricDatumTypeDef],
     },
-    total=False,
 )
 
 CanvasAppSettingsTypeDef = TypedDict(
     "CanvasAppSettingsTypeDef",
     {
         "TimeSeriesForecastingSettings": TimeSeriesForecastingSettingsTypeDef,
         "ModelRegisterSettings": ModelRegisterSettingsTypeDef,
+        "WorkspaceSettings": WorkspaceSettingsTypeDef,
     },
     total=False,
 )
 
 _RequiredRollingUpdatePolicyTypeDef = TypedDict(
     "_RequiredRollingUpdatePolicyTypeDef",
     {
@@ -10634,38 +10002,25 @@
 
 class ClarifyShapConfigTypeDef(
     _RequiredClarifyShapConfigTypeDef, _OptionalClarifyShapConfigTypeDef
 ):
     pass
 
 
-_RequiredCodeRepositorySummaryTypeDef = TypedDict(
-    "_RequiredCodeRepositorySummaryTypeDef",
+CodeRepositorySummaryTypeDef = TypedDict(
+    "CodeRepositorySummaryTypeDef",
     {
         "CodeRepositoryName": str,
         "CodeRepositoryArn": str,
         "CreationTime": datetime,
         "LastModifiedTime": datetime,
-    },
-)
-_OptionalCodeRepositorySummaryTypeDef = TypedDict(
-    "_OptionalCodeRepositorySummaryTypeDef",
-    {
         "GitConfig": GitConfigTypeDef,
     },
-    total=False,
 )
 
-
-class CodeRepositorySummaryTypeDef(
-    _RequiredCodeRepositorySummaryTypeDef, _OptionalCodeRepositorySummaryTypeDef
-):
-    pass
-
-
 _RequiredCreateCodeRepositoryInputRequestTypeDef = TypedDict(
     "_RequiredCreateCodeRepositoryInputRequestTypeDef",
     {
         "CodeRepositoryName": str,
         "GitConfig": GitConfigTypeDef,
     },
 )
@@ -10733,15 +10088,14 @@
         "ContextArn": str,
         "ContextName": str,
         "Source": ContextSourceTypeDef,
         "ContextType": str,
         "CreationTime": datetime,
         "LastModifiedTime": datetime,
     },
-    total=False,
 )
 
 _RequiredCreateContextRequestRequestTypeDef = TypedDict(
     "_RequiredCreateContextRequestRequestTypeDef",
     {
         "ContextName": str,
         "Source": ContextSourceTypeDef,
@@ -11088,43 +10442,30 @@
 
 class CreateHumanTaskUiRequestRequestTypeDef(
     _RequiredCreateHumanTaskUiRequestRequestTypeDef, _OptionalCreateHumanTaskUiRequestRequestTypeDef
 ):
     pass
 
 
-_RequiredInferenceExperimentSummaryTypeDef = TypedDict(
-    "_RequiredInferenceExperimentSummaryTypeDef",
+InferenceExperimentSummaryTypeDef = TypedDict(
+    "InferenceExperimentSummaryTypeDef",
     {
         "Name": str,
         "Type": Literal["ShadowMode"],
-        "Status": InferenceExperimentStatusType,
-        "CreationTime": datetime,
-        "LastModifiedTime": datetime,
-    },
-)
-_OptionalInferenceExperimentSummaryTypeDef = TypedDict(
-    "_OptionalInferenceExperimentSummaryTypeDef",
-    {
         "Schedule": InferenceExperimentScheduleTypeDef,
+        "Status": InferenceExperimentStatusType,
         "StatusReason": str,
         "Description": str,
+        "CreationTime": datetime,
         "CompletionTime": datetime,
+        "LastModifiedTime": datetime,
         "RoleArn": str,
     },
-    total=False,
 )
 
-
-class InferenceExperimentSummaryTypeDef(
-    _RequiredInferenceExperimentSummaryTypeDef, _OptionalInferenceExperimentSummaryTypeDef
-):
-    pass
-
-
 _RequiredCreateModelCardExportJobRequestRequestTypeDef = TypedDict(
     "_RequiredCreateModelCardExportJobRequestRequestTypeDef",
     {
         "ModelCardName": str,
         "ModelCardExportJobName": str,
         "OutputConfig": ModelCardExportOutputConfigTypeDef,
     },
@@ -11641,35 +10982,22 @@
 
 class DeleteDomainRequestRequestTypeDef(
     _RequiredDeleteDomainRequestRequestTypeDef, _OptionalDeleteDomainRequestRequestTypeDef
 ):
     pass
 
 
-_RequiredDeploymentRecommendationTypeDef = TypedDict(
-    "_RequiredDeploymentRecommendationTypeDef",
+DeploymentRecommendationTypeDef = TypedDict(
+    "DeploymentRecommendationTypeDef",
     {
         "RecommendationStatus": RecommendationStatusType,
-    },
-)
-_OptionalDeploymentRecommendationTypeDef = TypedDict(
-    "_OptionalDeploymentRecommendationTypeDef",
-    {
         "RealTimeInferenceRecommendations": List[RealTimeInferenceRecommendationTypeDef],
     },
-    total=False,
 )
 
-
-class DeploymentRecommendationTypeDef(
-    _RequiredDeploymentRecommendationTypeDef, _OptionalDeploymentRecommendationTypeDef
-):
-    pass
-
-
 _RequiredDeploymentStageTypeDef = TypedDict(
     "_RequiredDeploymentStageTypeDef",
     {
         "StageName": str,
         "DeviceSelectionConfig": DeviceSelectionConfigTypeDef,
     },
 )
@@ -12032,41 +11360,27 @@
         "ExperimentArn": str,
         "ExperimentName": str,
         "DisplayName": str,
         "ExperimentSource": ExperimentSourceTypeDef,
         "CreationTime": datetime,
         "LastModifiedTime": datetime,
     },
-    total=False,
 )
 
-_RequiredFeatureGroupSummaryTypeDef = TypedDict(
-    "_RequiredFeatureGroupSummaryTypeDef",
+FeatureGroupSummaryTypeDef = TypedDict(
+    "FeatureGroupSummaryTypeDef",
     {
         "FeatureGroupName": str,
         "FeatureGroupArn": str,
         "CreationTime": datetime,
-    },
-)
-_OptionalFeatureGroupSummaryTypeDef = TypedDict(
-    "_OptionalFeatureGroupSummaryTypeDef",
-    {
         "FeatureGroupStatus": FeatureGroupStatusType,
         "OfflineStoreStatus": OfflineStoreStatusTypeDef,
     },
-    total=False,
 )
 
-
-class FeatureGroupSummaryTypeDef(
-    _RequiredFeatureGroupSummaryTypeDef, _OptionalFeatureGroupSummaryTypeDef
-):
-    pass
-
-
 DescribeFeatureMetadataResponseTypeDef = TypedDict(
     "DescribeFeatureMetadataResponseTypeDef",
     {
         "FeatureGroupArn": str,
         "FeatureGroupName": str,
         "FeatureName": str,
         "FeatureType": FeatureTypeType,
@@ -12086,15 +11400,14 @@
         "FeatureName": str,
         "FeatureType": FeatureTypeType,
         "CreationTime": datetime,
         "LastModifiedTime": datetime,
         "Description": str,
         "Parameters": List[FeatureParameterTypeDef],
     },
-    total=False,
 )
 
 _RequiredUpdateFeatureMetadataRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateFeatureMetadataRequestRequestTypeDef",
     {
         "FeatureGroupName": str,
         "FeatureName": str,
@@ -12192,51 +11505,37 @@
     {
         "SubscribedWorkteams": List[SubscribedWorkteamTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredTrainingJobSummaryTypeDef = TypedDict(
-    "_RequiredTrainingJobSummaryTypeDef",
+TrainingJobSummaryTypeDef = TypedDict(
+    "TrainingJobSummaryTypeDef",
     {
         "TrainingJobName": str,
         "TrainingJobArn": str,
         "CreationTime": datetime,
-        "TrainingJobStatus": TrainingJobStatusType,
-    },
-)
-_OptionalTrainingJobSummaryTypeDef = TypedDict(
-    "_OptionalTrainingJobSummaryTypeDef",
-    {
         "TrainingEndTime": datetime,
         "LastModifiedTime": datetime,
+        "TrainingJobStatus": TrainingJobStatusType,
         "WarmPoolStatus": WarmPoolStatusTypeDef,
     },
-    total=False,
 )
 
-
-class TrainingJobSummaryTypeDef(
-    _RequiredTrainingJobSummaryTypeDef, _OptionalTrainingJobSummaryTypeDef
-):
-    pass
-
-
 TrialSummaryTypeDef = TypedDict(
     "TrialSummaryTypeDef",
     {
         "TrialArn": str,
         "TrialName": str,
         "DisplayName": str,
         "TrialSource": TrialSourceTypeDef,
         "CreationTime": datetime,
         "LastModifiedTime": datetime,
     },
-    total=False,
 )
 
 _RequiredDesiredWeightAndCapacityTypeDef = TypedDict(
     "_RequiredDesiredWeightAndCapacityTypeDef",
     {
         "VariantName": str,
     },
@@ -12272,40 +11571,29 @@
     {
         "DeviceFleetSummaries": List[DeviceFleetSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredDeviceSummaryTypeDef = TypedDict(
-    "_RequiredDeviceSummaryTypeDef",
+DeviceSummaryTypeDef = TypedDict(
+    "DeviceSummaryTypeDef",
     {
         "DeviceName": str,
         "DeviceArn": str,
-    },
-)
-_OptionalDeviceSummaryTypeDef = TypedDict(
-    "_OptionalDeviceSummaryTypeDef",
-    {
         "Description": str,
         "DeviceFleetName": str,
         "IotThingName": str,
         "RegistrationTime": datetime,
         "LatestHeartbeat": datetime,
         "Models": List[EdgeModelSummaryTypeDef],
         "AgentVersion": str,
     },
-    total=False,
 )
 
-
-class DeviceSummaryTypeDef(_RequiredDeviceSummaryTypeDef, _OptionalDeviceSummaryTypeDef):
-    pass
-
-
 _RequiredRegisterDevicesRequestRequestTypeDef = TypedDict(
     "_RequiredRegisterDevicesRequestRequestTypeDef",
     {
         "DeviceFleetName": str,
         "Devices": Sequence[DeviceTypeDef],
     },
 )
@@ -12398,38 +11686,25 @@
     {
         "EndpointConfigs": List[EndpointConfigSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredEndpointOutputConfigurationTypeDef = TypedDict(
-    "_RequiredEndpointOutputConfigurationTypeDef",
+EndpointOutputConfigurationTypeDef = TypedDict(
+    "EndpointOutputConfigurationTypeDef",
     {
         "EndpointName": str,
         "VariantName": str,
-    },
-)
-_OptionalEndpointOutputConfigurationTypeDef = TypedDict(
-    "_OptionalEndpointOutputConfigurationTypeDef",
-    {
         "InstanceType": ProductionVariantInstanceTypeType,
         "InitialInstanceCount": int,
         "ServerlessConfig": ProductionVariantServerlessConfigTypeDef,
     },
-    total=False,
 )
 
-
-class EndpointOutputConfigurationTypeDef(
-    _RequiredEndpointOutputConfigurationTypeDef, _OptionalEndpointOutputConfigurationTypeDef
-):
-    pass
-
-
 EndpointPerformanceTypeDef = TypedDict(
     "EndpointPerformanceTypeDef",
     {
         "Metrics": InferenceMetricsTypeDef,
         "EndpointInfo": EndpointInfoTypeDef,
     },
 )
@@ -12446,59 +11721,44 @@
 ModelConfigurationTypeDef = TypedDict(
     "ModelConfigurationTypeDef",
     {
         "InferenceSpecificationName": str,
         "EnvironmentParameters": List[EnvironmentParameterTypeDef],
         "CompilationJobName": str,
     },
-    total=False,
 )
 
 NestedFiltersTypeDef = TypedDict(
     "NestedFiltersTypeDef",
     {
         "NestedPropertyName": str,
         "Filters": Sequence[FilterTypeDef],
     },
 )
 
-_RequiredHyperParameterTrainingJobSummaryTypeDef = TypedDict(
-    "_RequiredHyperParameterTrainingJobSummaryTypeDef",
+HyperParameterTrainingJobSummaryTypeDef = TypedDict(
+    "HyperParameterTrainingJobSummaryTypeDef",
     {
+        "TrainingJobDefinitionName": str,
         "TrainingJobName": str,
         "TrainingJobArn": str,
-        "CreationTime": datetime,
-        "TrainingJobStatus": TrainingJobStatusType,
-        "TunedHyperParameters": Dict[str, str],
-    },
-)
-_OptionalHyperParameterTrainingJobSummaryTypeDef = TypedDict(
-    "_OptionalHyperParameterTrainingJobSummaryTypeDef",
-    {
-        "TrainingJobDefinitionName": str,
         "TuningJobName": str,
+        "CreationTime": datetime,
         "TrainingStartTime": datetime,
         "TrainingEndTime": datetime,
+        "TrainingJobStatus": TrainingJobStatusType,
+        "TunedHyperParameters": Dict[str, str],
         "FailureReason": str,
         "FinalHyperParameterTuningJobObjectiveMetric": (
             FinalHyperParameterTuningJobObjectiveMetricTypeDef
         ),
         "ObjectiveStatus": ObjectiveStatusType,
     },
-    total=False,
 )
 
-
-class HyperParameterTrainingJobSummaryTypeDef(
-    _RequiredHyperParameterTrainingJobSummaryTypeDef,
-    _OptionalHyperParameterTrainingJobSummaryTypeDef,
-):
-    pass
-
-
 ListFlowDefinitionsResponseTypeDef = TypedDict(
     "ListFlowDefinitionsResponseTypeDef",
     {
         "FlowDefinitionSummaries": List[FlowDefinitionSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -12586,43 +11846,30 @@
         "VolumeKmsKeyId": str,
         "AllocationStrategy": Literal["Prioritized"],
         "InstanceConfigs": Sequence[HyperParameterTuningInstanceConfigTypeDef],
     },
     total=False,
 )
 
-_RequiredHyperParameterTuningJobSummaryTypeDef = TypedDict(
-    "_RequiredHyperParameterTuningJobSummaryTypeDef",
+HyperParameterTuningJobSummaryTypeDef = TypedDict(
+    "HyperParameterTuningJobSummaryTypeDef",
     {
         "HyperParameterTuningJobName": str,
         "HyperParameterTuningJobArn": str,
         "HyperParameterTuningJobStatus": HyperParameterTuningJobStatusType,
         "Strategy": HyperParameterTuningJobStrategyTypeType,
         "CreationTime": datetime,
-        "TrainingJobStatusCounters": TrainingJobStatusCountersTypeDef,
-        "ObjectiveStatusCounters": ObjectiveStatusCountersTypeDef,
-    },
-)
-_OptionalHyperParameterTuningJobSummaryTypeDef = TypedDict(
-    "_OptionalHyperParameterTuningJobSummaryTypeDef",
-    {
         "HyperParameterTuningEndTime": datetime,
         "LastModifiedTime": datetime,
+        "TrainingJobStatusCounters": TrainingJobStatusCountersTypeDef,
+        "ObjectiveStatusCounters": ObjectiveStatusCountersTypeDef,
         "ResourceLimits": ResourceLimitsTypeDef,
     },
-    total=False,
 )
 
-
-class HyperParameterTuningJobSummaryTypeDef(
-    _RequiredHyperParameterTuningJobSummaryTypeDef, _OptionalHyperParameterTuningJobSummaryTypeDef
-):
-    pass
-
-
 HyperParameterTuningJobStrategyConfigTypeDef = TypedDict(
     "HyperParameterTuningJobStrategyConfigTypeDef",
     {
         "HyperbandStrategyConfig": HyperbandStrategyConfigTypeDef,
     },
     total=False,
 )
@@ -12639,15 +11886,14 @@
     "UserContextTypeDef",
     {
         "UserProfileArn": str,
         "UserProfileName": str,
         "DomainId": str,
         "IamIdentity": IamIdentityTypeDef,
     },
-    total=False,
 )
 
 _RequiredImageConfigTypeDef = TypedDict(
     "_RequiredImageConfigTypeDef",
     {
         "RepositoryAccessMode": RepositoryAccessModeType,
     },
@@ -12753,39 +11999,26 @@
 
 class KernelGatewayImageConfigTypeDef(
     _RequiredKernelGatewayImageConfigTypeDef, _OptionalKernelGatewayImageConfigTypeDef
 ):
     pass
 
 
-_RequiredLabelingJobForWorkteamSummaryTypeDef = TypedDict(
-    "_RequiredLabelingJobForWorkteamSummaryTypeDef",
+LabelingJobForWorkteamSummaryTypeDef = TypedDict(
+    "LabelingJobForWorkteamSummaryTypeDef",
     {
+        "LabelingJobName": str,
         "JobReferenceCode": str,
         "WorkRequesterAccountId": str,
         "CreationTime": datetime,
-    },
-)
-_OptionalLabelingJobForWorkteamSummaryTypeDef = TypedDict(
-    "_OptionalLabelingJobForWorkteamSummaryTypeDef",
-    {
-        "LabelingJobName": str,
         "LabelCounters": LabelCountersForWorkteamTypeDef,
         "NumberOfHumanWorkersPerDataObject": int,
     },
-    total=False,
 )
 
-
-class LabelingJobForWorkteamSummaryTypeDef(
-    _RequiredLabelingJobForWorkteamSummaryTypeDef, _OptionalLabelingJobForWorkteamSummaryTypeDef
-):
-    pass
-
-
 LabelingJobDataSourceTypeDef = TypedDict(
     "LabelingJobDataSourceTypeDef",
     {
         "S3DataSource": LabelingJobS3DataSourceTypeDef,
         "SnsDataSource": LabelingJobSnsDataSourceTypeDef,
     },
     total=False,
@@ -13026,15 +12259,14 @@
 )
 
 MonitoringAlertActionsTypeDef = TypedDict(
     "MonitoringAlertActionsTypeDef",
     {
         "ModelDashboardIndicator": ModelDashboardIndicatorActionTypeDef,
     },
-    total=False,
 )
 
 ModelDataSourceTypeDef = TypedDict(
     "ModelDataSourceTypeDef",
     {
         "S3DataSource": S3ModelDataSourceTypeDef,
     },
@@ -13044,43 +12276,30 @@
     "ModelInfrastructureConfigTypeDef",
     {
         "InfrastructureType": Literal["RealTimeInference"],
         "RealTimeInferenceConfig": RealTimeInferenceConfigTypeDef,
     },
 )
 
-_RequiredModelPackageContainerDefinitionTypeDef = TypedDict(
-    "_RequiredModelPackageContainerDefinitionTypeDef",
-    {
-        "Image": str,
-    },
-)
-_OptionalModelPackageContainerDefinitionTypeDef = TypedDict(
-    "_OptionalModelPackageContainerDefinitionTypeDef",
+ModelPackageContainerDefinitionTypeDef = TypedDict(
+    "ModelPackageContainerDefinitionTypeDef",
     {
         "ContainerHostname": str,
+        "Image": str,
         "ImageDigest": str,
         "ModelDataUrl": str,
         "ProductId": str,
         "Environment": Dict[str, str],
         "ModelInput": ModelInputTypeDef,
         "Framework": str,
         "FrameworkVersion": str,
         "NearestModelName": str,
     },
-    total=False,
 )
 
-
-class ModelPackageContainerDefinitionTypeDef(
-    _RequiredModelPackageContainerDefinitionTypeDef, _OptionalModelPackageContainerDefinitionTypeDef
-):
-    pass
-
-
 RecommendationJobStoppingConditionsTypeDef = TypedDict(
     "RecommendationJobStoppingConditionsTypeDef",
     {
         "MaxInvocations": int,
         "ModelLatencyThresholds": Sequence[ModelLatencyThresholdTypeDef],
     },
     total=False,
@@ -13090,35 +12309,22 @@
     "ModelMetadataSearchExpressionTypeDef",
     {
         "Filters": Sequence[ModelMetadataFilterTypeDef],
     },
     total=False,
 )
 
-_RequiredModelPackageStatusDetailsTypeDef = TypedDict(
-    "_RequiredModelPackageStatusDetailsTypeDef",
+ModelPackageStatusDetailsTypeDef = TypedDict(
+    "ModelPackageStatusDetailsTypeDef",
     {
         "ValidationStatuses": List[ModelPackageStatusItemTypeDef],
-    },
-)
-_OptionalModelPackageStatusDetailsTypeDef = TypedDict(
-    "_OptionalModelPackageStatusDetailsTypeDef",
-    {
         "ImageScanStatuses": List[ModelPackageStatusItemTypeDef],
     },
-    total=False,
 )
 
-
-class ModelPackageStatusDetailsTypeDef(
-    _RequiredModelPackageStatusDetailsTypeDef, _OptionalModelPackageStatusDetailsTypeDef
-):
-    pass
-
-
 MonitoringResourcesTypeDef = TypedDict(
     "MonitoringResourcesTypeDef",
     {
         "ClusterConfig": MonitoringClusterConfigTypeDef,
     },
 )
 
@@ -13198,72 +12404,46 @@
 )
 
 
 class OutputConfigTypeDef(_RequiredOutputConfigTypeDef, _OptionalOutputConfigTypeDef):
     pass
 
 
-_RequiredPendingProductionVariantSummaryTypeDef = TypedDict(
-    "_RequiredPendingProductionVariantSummaryTypeDef",
+PendingProductionVariantSummaryTypeDef = TypedDict(
+    "PendingProductionVariantSummaryTypeDef",
     {
         "VariantName": str,
-    },
-)
-_OptionalPendingProductionVariantSummaryTypeDef = TypedDict(
-    "_OptionalPendingProductionVariantSummaryTypeDef",
-    {
         "DeployedImages": List[DeployedImageTypeDef],
         "CurrentWeight": float,
         "DesiredWeight": float,
         "CurrentInstanceCount": int,
         "DesiredInstanceCount": int,
         "InstanceType": ProductionVariantInstanceTypeType,
         "AcceleratorType": ProductionVariantAcceleratorTypeType,
         "VariantStatus": List[ProductionVariantStatusTypeDef],
         "CurrentServerlessConfig": ProductionVariantServerlessConfigTypeDef,
         "DesiredServerlessConfig": ProductionVariantServerlessConfigTypeDef,
     },
-    total=False,
 )
 
-
-class PendingProductionVariantSummaryTypeDef(
-    _RequiredPendingProductionVariantSummaryTypeDef, _OptionalPendingProductionVariantSummaryTypeDef
-):
-    pass
-
-
-_RequiredProductionVariantSummaryTypeDef = TypedDict(
-    "_RequiredProductionVariantSummaryTypeDef",
+ProductionVariantSummaryTypeDef = TypedDict(
+    "ProductionVariantSummaryTypeDef",
     {
         "VariantName": str,
-    },
-)
-_OptionalProductionVariantSummaryTypeDef = TypedDict(
-    "_OptionalProductionVariantSummaryTypeDef",
-    {
         "DeployedImages": List[DeployedImageTypeDef],
         "CurrentWeight": float,
         "DesiredWeight": float,
         "CurrentInstanceCount": int,
         "DesiredInstanceCount": int,
         "VariantStatus": List[ProductionVariantStatusTypeDef],
         "CurrentServerlessConfig": ProductionVariantServerlessConfigTypeDef,
         "DesiredServerlessConfig": ProductionVariantServerlessConfigTypeDef,
     },
-    total=False,
 )
 
-
-class ProductionVariantSummaryTypeDef(
-    _RequiredProductionVariantSummaryTypeDef, _OptionalProductionVariantSummaryTypeDef
-):
-    pass
-
-
 TrafficPatternTypeDef = TypedDict(
     "TrafficPatternTypeDef",
     {
         "TrafficType": Literal["PHASES"],
         "Phases": Sequence[PhaseTypeDef],
     },
     total=False,
@@ -13554,42 +12734,31 @@
 TransformDataSourceTypeDef = TypedDict(
     "TransformDataSourceTypeDef",
     {
         "S3DataSource": TransformS3DataSourceTypeDef,
     },
 )
 
-_RequiredWorkforceTypeDef = TypedDict(
-    "_RequiredWorkforceTypeDef",
+WorkforceTypeDef = TypedDict(
+    "WorkforceTypeDef",
     {
         "WorkforceName": str,
         "WorkforceArn": str,
-    },
-)
-_OptionalWorkforceTypeDef = TypedDict(
-    "_OptionalWorkforceTypeDef",
-    {
         "LastUpdatedDate": datetime,
         "SourceIpConfig": SourceIpConfigTypeDef,
         "SubDomain": str,
         "CognitoConfig": CognitoConfigTypeDef,
         "OidcConfig": OidcConfigForResponseTypeDef,
         "CreateDate": datetime,
         "WorkforceVpcConfig": WorkforceVpcConfigResponseTypeDef,
         "Status": WorkforceStatusType,
         "FailureReason": str,
     },
-    total=False,
 )
 
-
-class WorkforceTypeDef(_RequiredWorkforceTypeDef, _OptionalWorkforceTypeDef):
-    pass
-
-
 ListActionsResponseTypeDef = TypedDict(
     "ListActionsResponseTypeDef",
     {
         "ActionSummaries": List[ActionSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -13601,15 +12770,14 @@
         "ArtifactArn": str,
         "ArtifactName": str,
         "Source": ArtifactSourceTypeDef,
         "ArtifactType": str,
         "CreationTime": datetime,
         "LastModifiedTime": datetime,
     },
-    total=False,
 )
 
 _RequiredCreateArtifactRequestRequestTypeDef = TypedDict(
     "_RequiredCreateArtifactRequestRequestTypeDef",
     {
         "Source": ArtifactSourceTypeDef,
         "ArtifactType": str,
@@ -13734,15 +12902,14 @@
 AutoMLResolvedAttributesTypeDef = TypedDict(
     "AutoMLResolvedAttributesTypeDef",
     {
         "AutoMLJobObjective": AutoMLJobObjectiveTypeDef,
         "CompletionCriteria": AutoMLJobCompletionCriteriaTypeDef,
         "AutoMLProblemTypeResolvedAttributes": AutoMLProblemTypeResolvedAttributesTypeDef,
     },
-    total=False,
 )
 
 AutoMLJobConfigTypeDef = TypedDict(
     "AutoMLJobConfigTypeDef",
     {
         "CompletionCriteria": AutoMLJobCompletionCriteriaTypeDef,
         "SecurityConfig": AutoMLSecurityConfigTypeDef,
@@ -13800,48 +12967,36 @@
         "Lambda": LambdaStepMetadataTypeDef,
         "QualityCheck": QualityCheckStepMetadataTypeDef,
         "ClarifyCheck": ClarifyCheckStepMetadataTypeDef,
         "EMR": EMRStepMetadataTypeDef,
         "Fail": FailStepMetadataTypeDef,
         "AutoMLJob": AutoMLJobStepMetadataTypeDef,
     },
-    total=False,
 )
 
-_RequiredAutoMLCandidateTypeDef = TypedDict(
-    "_RequiredAutoMLCandidateTypeDef",
+AutoMLCandidateTypeDef = TypedDict(
+    "AutoMLCandidateTypeDef",
     {
         "CandidateName": str,
+        "FinalAutoMLJobObjectiveMetric": FinalAutoMLJobObjectiveMetricTypeDef,
         "ObjectiveStatus": ObjectiveStatusType,
         "CandidateSteps": List[AutoMLCandidateStepTypeDef],
         "CandidateStatus": CandidateStatusType,
-        "CreationTime": datetime,
-        "LastModifiedTime": datetime,
-    },
-)
-_OptionalAutoMLCandidateTypeDef = TypedDict(
-    "_OptionalAutoMLCandidateTypeDef",
-    {
-        "FinalAutoMLJobObjectiveMetric": FinalAutoMLJobObjectiveMetricTypeDef,
         "InferenceContainers": List[AutoMLContainerDefinitionTypeDef],
+        "CreationTime": datetime,
         "EndTime": datetime,
+        "LastModifiedTime": datetime,
         "FailureReason": str,
         "CandidateProperties": CandidatePropertiesTypeDef,
         "InferenceContainerDefinitions": Dict[
             AutoMLProcessingUnitType, List[AutoMLContainerDefinitionTypeDef]
         ],
     },
-    total=False,
 )
 
-
-class AutoMLCandidateTypeDef(_RequiredAutoMLCandidateTypeDef, _OptionalAutoMLCandidateTypeDef):
-    pass
-
-
 _RequiredBlueGreenUpdatePolicyTypeDef = TypedDict(
     "_RequiredBlueGreenUpdatePolicyTypeDef",
     {
         "TrafficRoutingConfiguration": TrafficRoutingConfigTypeDef,
     },
 )
 _OptionalBlueGreenUpdatePolicyTypeDef = TypedDict(
@@ -14132,66 +13287,39 @@
         "Explainability": DriftCheckExplainabilityTypeDef,
         "ModelQuality": DriftCheckModelQualityTypeDef,
         "ModelDataQuality": DriftCheckModelDataQualityTypeDef,
     },
     total=False,
 )
 
-_RequiredInferenceRecommendationTypeDef = TypedDict(
-    "_RequiredInferenceRecommendationTypeDef",
+InferenceRecommendationTypeDef = TypedDict(
+    "InferenceRecommendationTypeDef",
     {
         "Metrics": RecommendationMetricsTypeDef,
         "EndpointConfiguration": EndpointOutputConfigurationTypeDef,
         "ModelConfiguration": ModelConfigurationTypeDef,
-    },
-)
-_OptionalInferenceRecommendationTypeDef = TypedDict(
-    "_OptionalInferenceRecommendationTypeDef",
-    {
         "RecommendationId": str,
         "InvocationEndTime": datetime,
         "InvocationStartTime": datetime,
     },
-    total=False,
 )
 
-
-class InferenceRecommendationTypeDef(
-    _RequiredInferenceRecommendationTypeDef, _OptionalInferenceRecommendationTypeDef
-):
-    pass
-
-
-_RequiredRecommendationJobInferenceBenchmarkTypeDef = TypedDict(
-    "_RequiredRecommendationJobInferenceBenchmarkTypeDef",
-    {
-        "ModelConfiguration": ModelConfigurationTypeDef,
-    },
-)
-_OptionalRecommendationJobInferenceBenchmarkTypeDef = TypedDict(
-    "_OptionalRecommendationJobInferenceBenchmarkTypeDef",
+RecommendationJobInferenceBenchmarkTypeDef = TypedDict(
+    "RecommendationJobInferenceBenchmarkTypeDef",
     {
         "Metrics": RecommendationMetricsTypeDef,
         "EndpointConfiguration": EndpointOutputConfigurationTypeDef,
+        "ModelConfiguration": ModelConfigurationTypeDef,
         "FailureReason": str,
         "EndpointMetrics": InferenceMetricsTypeDef,
         "InvocationEndTime": datetime,
         "InvocationStartTime": datetime,
     },
-    total=False,
 )
 
-
-class RecommendationJobInferenceBenchmarkTypeDef(
-    _RequiredRecommendationJobInferenceBenchmarkTypeDef,
-    _OptionalRecommendationJobInferenceBenchmarkTypeDef,
-):
-    pass
-
-
 SearchExpressionTypeDef = TypedDict(
     "SearchExpressionTypeDef",
     {
         "Filters": Sequence[FilterTypeDef],
         "NestedFilters": Sequence[NestedFiltersTypeDef],
         "SubExpressions": Sequence[Dict[str, Any]],
         "Operator": BooleanOperatorType,
@@ -14226,15 +13354,14 @@
         "DestinationType": str,
         "AssociationType": AssociationEdgeTypeType,
         "SourceName": str,
         "DestinationName": str,
         "CreationTime": datetime,
         "CreatedBy": UserContextTypeDef,
     },
-    total=False,
 )
 
 DescribeActionResponseTypeDef = TypedDict(
     "DescribeActionResponseTypeDef",
     {
         "ActionName": str,
         "ActionArn": str,
@@ -14423,15 +13550,14 @@
         "Description": str,
         "CreationTime": datetime,
         "CreatedBy": UserContextTypeDef,
         "LastModifiedTime": datetime,
         "LastModifiedBy": UserContextTypeDef,
         "Tags": List[TagTypeDef],
     },
-    total=False,
 )
 
 ModelCardTypeDef = TypedDict(
     "ModelCardTypeDef",
     {
         "ModelCardArn": str,
         "ModelCardName": str,
@@ -14444,15 +13570,14 @@
         "LastModifiedTime": datetime,
         "LastModifiedBy": UserContextTypeDef,
         "Tags": List[TagTypeDef],
         "ModelId": str,
         "RiskRating": str,
         "ModelPackageGroupName": str,
     },
-    total=False,
 )
 
 ModelDashboardModelCardTypeDef = TypedDict(
     "ModelDashboardModelCardTypeDef",
     {
         "ModelCardArn": str,
         "ModelCardName": str,
@@ -14463,29 +13588,27 @@
         "CreatedBy": UserContextTypeDef,
         "LastModifiedTime": datetime,
         "LastModifiedBy": UserContextTypeDef,
         "Tags": List[TagTypeDef],
         "ModelId": str,
         "RiskRating": str,
     },
-    total=False,
 )
 
 ModelPackageGroupTypeDef = TypedDict(
     "ModelPackageGroupTypeDef",
     {
         "ModelPackageGroupName": str,
         "ModelPackageGroupArn": str,
         "ModelPackageGroupDescription": str,
         "CreationTime": datetime,
         "CreatedBy": UserContextTypeDef,
         "ModelPackageGroupStatus": ModelPackageGroupStatusType,
         "Tags": List[TagTypeDef],
     },
-    total=False,
 )
 
 PipelineTypeDef = TypedDict(
     "PipelineTypeDef",
     {
         "PipelineArn": str,
         "PipelineName": str,
@@ -14497,27 +13620,25 @@
         "LastModifiedTime": datetime,
         "LastRunTime": datetime,
         "CreatedBy": UserContextTypeDef,
         "LastModifiedBy": UserContextTypeDef,
         "ParallelismConfiguration": ParallelismConfigurationTypeDef,
         "Tags": List[TagTypeDef],
     },
-    total=False,
 )
 
 TrialComponentSimpleSummaryTypeDef = TypedDict(
     "TrialComponentSimpleSummaryTypeDef",
     {
         "TrialComponentName": str,
         "TrialComponentArn": str,
         "TrialComponentSource": TrialComponentSourceTypeDef,
         "CreationTime": datetime,
         "CreatedBy": UserContextTypeDef,
     },
-    total=False,
 )
 
 TrialComponentSummaryTypeDef = TypedDict(
     "TrialComponentSummaryTypeDef",
     {
         "TrialComponentName": str,
         "TrialComponentArn": str,
@@ -14527,15 +13648,14 @@
         "StartTime": datetime,
         "EndTime": datetime,
         "CreationTime": datetime,
         "CreatedBy": UserContextTypeDef,
         "LastModifiedTime": datetime,
         "LastModifiedBy": UserContextTypeDef,
     },
-    total=False,
 )
 
 _RequiredHyperParameterSpecificationTypeDef = TypedDict(
     "_RequiredHyperParameterSpecificationTypeDef",
     {
         "Name": str,
         "Type": ParameterTypeType,
@@ -14592,15 +13712,14 @@
     {
         "AppImageConfigArn": str,
         "AppImageConfigName": str,
         "CreationTime": datetime,
         "LastModifiedTime": datetime,
         "KernelGatewayImageConfig": KernelGatewayImageConfigTypeDef,
     },
-    total=False,
 )
 
 _RequiredCreateAppImageConfigRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAppImageConfigRequestRequestTypeDef",
     {
         "AppImageConfigName": str,
     },
@@ -14730,41 +13849,30 @@
 
 class UpdateWorkteamRequestRequestTypeDef(
     _RequiredUpdateWorkteamRequestRequestTypeDef, _OptionalUpdateWorkteamRequestRequestTypeDef
 ):
     pass
 
 
-_RequiredWorkteamTypeDef = TypedDict(
-    "_RequiredWorkteamTypeDef",
+WorkteamTypeDef = TypedDict(
+    "WorkteamTypeDef",
     {
         "WorkteamName": str,
         "MemberDefinitions": List[MemberDefinitionTypeDef],
         "WorkteamArn": str,
-        "Description": str,
-    },
-)
-_OptionalWorkteamTypeDef = TypedDict(
-    "_OptionalWorkteamTypeDef",
-    {
         "WorkforceArn": str,
         "ProductListingIds": List[str],
+        "Description": str,
         "SubDomain": str,
         "CreateDate": datetime,
         "LastUpdatedDate": datetime,
         "NotificationConfiguration": NotificationConfigurationTypeDef,
     },
-    total=False,
 )
 
-
-class WorkteamTypeDef(_RequiredWorkteamTypeDef, _OptionalWorkteamTypeDef):
-    pass
-
-
 MonitoringAlertSummaryTypeDef = TypedDict(
     "MonitoringAlertSummaryTypeDef",
     {
         "MonitoringAlertName": str,
         "CreationTime": datetime,
         "LastModifiedTime": datetime,
         "AlertStatus": MonitoringAlertStatusType,
@@ -14833,38 +13941,25 @@
 class AdditionalInferenceSpecificationDefinitionTypeDef(
     _RequiredAdditionalInferenceSpecificationDefinitionTypeDef,
     _OptionalAdditionalInferenceSpecificationDefinitionTypeDef,
 ):
     pass
 
 
-_RequiredInferenceSpecificationTypeDef = TypedDict(
-    "_RequiredInferenceSpecificationTypeDef",
+InferenceSpecificationTypeDef = TypedDict(
+    "InferenceSpecificationTypeDef",
     {
         "Containers": List[ModelPackageContainerDefinitionTypeDef],
-        "SupportedContentTypes": List[str],
-        "SupportedResponseMIMETypes": List[str],
-    },
-)
-_OptionalInferenceSpecificationTypeDef = TypedDict(
-    "_OptionalInferenceSpecificationTypeDef",
-    {
         "SupportedTransformInstanceTypes": List[TransformInstanceTypeType],
         "SupportedRealtimeInferenceInstanceTypes": List[ProductionVariantInstanceTypeType],
+        "SupportedContentTypes": List[str],
+        "SupportedResponseMIMETypes": List[str],
     },
-    total=False,
 )
 
-
-class InferenceSpecificationTypeDef(
-    _RequiredInferenceSpecificationTypeDef, _OptionalInferenceSpecificationTypeDef
-):
-    pass
-
-
 ListModelMetadataRequestListModelMetadataPaginateTypeDef = TypedDict(
     "ListModelMetadataRequestListModelMetadataPaginateTypeDef",
     {
         "SearchExpression": ModelMetadataSearchExpressionTypeDef,
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
@@ -15000,15 +14095,14 @@
         "FeatureGroupStatus": FeatureGroupStatusType,
         "OfflineStoreStatus": OfflineStoreStatusTypeDef,
         "LastUpdateStatus": LastUpdateStatusTypeDef,
         "FailureReason": str,
         "Description": str,
         "Tags": List[TagTypeDef],
     },
-    total=False,
 )
 
 _RequiredUpdateFeatureGroupRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateFeatureGroupRequestRequestTypeDef",
     {
         "FeatureGroupName": str,
     },
@@ -15078,37 +14172,24 @@
         "InputConfig": InputConfigTypeDef,
         "OutputConfig": OutputConfigTypeDef,
         "VpcConfig": NeoVpcConfigTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredPendingDeploymentSummaryTypeDef = TypedDict(
-    "_RequiredPendingDeploymentSummaryTypeDef",
+PendingDeploymentSummaryTypeDef = TypedDict(
+    "PendingDeploymentSummaryTypeDef",
     {
         "EndpointConfigName": str,
-    },
-)
-_OptionalPendingDeploymentSummaryTypeDef = TypedDict(
-    "_OptionalPendingDeploymentSummaryTypeDef",
-    {
         "ProductionVariants": List[PendingProductionVariantSummaryTypeDef],
         "StartTime": datetime,
         "ShadowProductionVariants": List[PendingProductionVariantSummaryTypeDef],
     },
-    total=False,
 )
 
-
-class PendingDeploymentSummaryTypeDef(
-    _RequiredPendingDeploymentSummaryTypeDef, _OptionalPendingDeploymentSummaryTypeDef
-):
-    pass
-
-
 _RequiredProcessingOutputConfigTypeDef = TypedDict(
     "_RequiredProcessingOutputConfigTypeDef",
     {
         "Outputs": Sequence[ProcessingOutputTypeDef],
     },
 )
 _OptionalProcessingOutputConfigTypeDef = TypedDict(
@@ -15201,15 +14282,14 @@
         "ProjectStatus": ProjectStatusType,
         "CreatedBy": UserContextTypeDef,
         "CreationTime": datetime,
         "Tags": List[TagTypeDef],
         "LastModifiedTime": datetime,
         "LastModifiedBy": UserContextTypeDef,
     },
-    total=False,
 )
 
 _RequiredUpdateProjectInputRequestTypeDef = TypedDict(
     "_RequiredUpdateProjectInputRequestTypeDef",
     {
         "ProjectName": str,
     },
@@ -15320,15 +14400,14 @@
         "LastModifiedTime": datetime,
         "CreatedBy": UserContextTypeDef,
         "LastModifiedBy": UserContextTypeDef,
         "ParallelismConfiguration": ParallelismConfigurationTypeDef,
         "PipelineParameters": List[ParameterTypeDef],
         "SelectiveExecutionConfig": SelectiveExecutionConfigTypeDef,
     },
-    total=False,
 )
 
 _RequiredStartPipelineExecutionRequestRequestTypeDef = TypedDict(
     "_RequiredStartPipelineExecutionRequestRequestTypeDef",
     {
         "PipelineName": str,
         "ClientRequestToken": str,
@@ -15487,15 +14566,14 @@
         "StepStatus": StepStatusType,
         "CacheHitResult": CacheHitResultTypeDef,
         "AttemptCount": int,
         "FailureReason": str,
         "Metadata": PipelineExecutionStepMetadataTypeDef,
         "SelectiveExecutionResult": SelectiveExecutionResultTypeDef,
     },
-    total=False,
 )
 
 DescribeAutoMLJobResponseTypeDef = TypedDict(
     "DescribeAutoMLJobResponseTypeDef",
     {
         "AutoMLJobName": str,
         "AutoMLJobArn": str,
@@ -15834,37 +14912,24 @@
 
 class TrainingJobDefinitionTypeDef(
     _RequiredTrainingJobDefinitionTypeDef, _OptionalTrainingJobDefinitionTypeDef
 ):
     pass
 
 
-_RequiredInferenceRecommendationsJobStepTypeDef = TypedDict(
-    "_RequiredInferenceRecommendationsJobStepTypeDef",
+InferenceRecommendationsJobStepTypeDef = TypedDict(
+    "InferenceRecommendationsJobStepTypeDef",
     {
         "StepType": Literal["BENCHMARK"],
         "JobName": str,
         "Status": RecommendationJobStatusType,
-    },
-)
-_OptionalInferenceRecommendationsJobStepTypeDef = TypedDict(
-    "_OptionalInferenceRecommendationsJobStepTypeDef",
-    {
         "InferenceBenchmark": RecommendationJobInferenceBenchmarkTypeDef,
     },
-    total=False,
 )
 
-
-class InferenceRecommendationsJobStepTypeDef(
-    _RequiredInferenceRecommendationsJobStepTypeDef, _OptionalInferenceRecommendationsJobStepTypeDef
-):
-    pass
-
-
 ListAssociationsResponseTypeDef = TypedDict(
     "ListAssociationsResponseTypeDef",
     {
         "AssociationSummaries": List[AssociationSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -15882,15 +14947,14 @@
         "CreatedBy": UserContextTypeDef,
         "LastModifiedTime": datetime,
         "LastModifiedBy": UserContextTypeDef,
         "MetadataProperties": MetadataPropertiesTypeDef,
         "Tags": List[TagTypeDef],
         "TrialComponentSummaries": List[TrialComponentSimpleSummaryTypeDef],
     },
-    total=False,
 )
 
 ListTrialComponentsResponseTypeDef = TypedDict(
     "ListTrialComponentsResponseTypeDef",
     {
         "TrialComponentSummaries": List[TrialComponentSummaryTypeDef],
         "NextToken": str,
@@ -15930,45 +14994,32 @@
     {
         "NextToken": str,
         "AppImageConfigs": List[AppImageConfigDetailsTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredLabelingJobSummaryTypeDef = TypedDict(
-    "_RequiredLabelingJobSummaryTypeDef",
+LabelingJobSummaryTypeDef = TypedDict(
+    "LabelingJobSummaryTypeDef",
     {
         "LabelingJobName": str,
         "LabelingJobArn": str,
         "CreationTime": datetime,
         "LastModifiedTime": datetime,
         "LabelingJobStatus": LabelingJobStatusType,
         "LabelCounters": LabelCountersTypeDef,
         "WorkteamArn": str,
         "PreHumanTaskLambdaArn": str,
-    },
-)
-_OptionalLabelingJobSummaryTypeDef = TypedDict(
-    "_OptionalLabelingJobSummaryTypeDef",
-    {
         "AnnotationConsolidationLambdaArn": str,
         "FailureReason": str,
         "LabelingJobOutput": LabelingJobOutputTypeDef,
         "InputConfig": LabelingJobInputConfigTypeDef,
     },
-    total=False,
 )
 
-
-class LabelingJobSummaryTypeDef(
-    _RequiredLabelingJobSummaryTypeDef, _OptionalLabelingJobSummaryTypeDef
-):
-    pass
-
-
 DescribeWorkteamResponseTypeDef = TypedDict(
     "DescribeWorkteamResponseTypeDef",
     {
         "Workteam": WorkteamTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -16054,15 +15105,14 @@
         "VpcConfig": VpcConfigTypeDef,
         "CreationTime": datetime,
         "ModelArn": str,
         "EnableNetworkIsolation": bool,
         "Tags": List[TagTypeDef],
         "DeploymentRecommendation": DeploymentRecommendationTypeDef,
     },
-    total=False,
 )
 
 DescribeInferenceExperimentResponseTypeDef = TypedDict(
     "DescribeInferenceExperimentResponseTypeDef",
     {
         "Arn": str,
         "Name": str,
@@ -16189,42 +15239,28 @@
 
 class UpdateModelPackageInputRequestTypeDef(
     _RequiredUpdateModelPackageInputRequestTypeDef, _OptionalUpdateModelPackageInputRequestTypeDef
 ):
     pass
 
 
-_RequiredBatchDescribeModelPackageSummaryTypeDef = TypedDict(
-    "_RequiredBatchDescribeModelPackageSummaryTypeDef",
+BatchDescribeModelPackageSummaryTypeDef = TypedDict(
+    "BatchDescribeModelPackageSummaryTypeDef",
     {
         "ModelPackageGroupName": str,
+        "ModelPackageVersion": int,
         "ModelPackageArn": str,
+        "ModelPackageDescription": str,
         "CreationTime": datetime,
         "InferenceSpecification": InferenceSpecificationTypeDef,
         "ModelPackageStatus": ModelPackageStatusType,
-    },
-)
-_OptionalBatchDescribeModelPackageSummaryTypeDef = TypedDict(
-    "_OptionalBatchDescribeModelPackageSummaryTypeDef",
-    {
-        "ModelPackageVersion": int,
-        "ModelPackageDescription": str,
         "ModelApprovalStatus": ModelApprovalStatusType,
     },
-    total=False,
 )
 
-
-class BatchDescribeModelPackageSummaryTypeDef(
-    _RequiredBatchDescribeModelPackageSummaryTypeDef,
-    _OptionalBatchDescribeModelPackageSummaryTypeDef,
-):
-    pass
-
-
 DataQualityJobInputTypeDef = TypedDict(
     "DataQualityJobInputTypeDef",
     {
         "EndpointInput": EndpointInputTypeDef,
         "BatchTransformInput": BatchTransformInputTypeDef,
     },
     total=False,
@@ -16373,15 +15409,14 @@
         "LastModifiedTime": datetime,
         "CreationTime": datetime,
         "MonitoringScheduleArn": str,
         "AutoMLJobArn": str,
         "TrainingJobArn": str,
         "Tags": List[TagTypeDef],
     },
-    total=False,
 )
 
 _RequiredCreateFlowDefinitionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateFlowDefinitionRequestRequestTypeDef",
     {
         "FlowDefinitionName": str,
         "HumanLoopConfig": HumanLoopConfigTypeDef,
@@ -16604,15 +15639,14 @@
         "DebugRuleConfigurations": List[DebugRuleConfigurationTypeDef],
         "TensorBoardOutputConfig": TensorBoardOutputConfigTypeDef,
         "DebugRuleEvaluationStatuses": List[DebugRuleEvaluationStatusTypeDef],
         "Environment": Dict[str, str],
         "RetryStrategy": RetryStrategyTypeDef,
         "Tags": List[TagTypeDef],
     },
-    total=False,
 )
 
 _RequiredCreateTransformJobRequestRequestTypeDef = TypedDict(
     "_RequiredCreateTransformJobRequestRequestTypeDef",
     {
         "TransformJobName": str,
         "ModelName": str,
@@ -16720,15 +15754,14 @@
         "TransformEndTime": datetime,
         "LabelingJobArn": str,
         "AutoMLJobArn": str,
         "DataProcessing": DataProcessingTypeDef,
         "ExperimentConfig": ExperimentConfigTypeDef,
         "Tags": List[TagTypeDef],
     },
-    total=False,
 )
 
 _RequiredCreateAutoMLJobV2RequestRequestTypeDef = TypedDict(
     "_RequiredCreateAutoMLJobV2RequestRequestTypeDef",
     {
         "AutoMLJobName": str,
         "AutoMLJobInputDataConfig": Sequence[AutoMLJobChannelTypeDef],
@@ -17026,15 +16059,14 @@
         "OverallBestTrainingJob": HyperParameterTrainingJobSummaryTypeDef,
         "WarmStartConfig": HyperParameterTuningJobWarmStartConfigTypeDef,
         "FailureReason": str,
         "Tags": List[TagTypeDef],
         "TuningJobCompletionDetails": HyperParameterTuningJobCompletionDetailsTypeDef,
         "ConsumedResources": HyperParameterTuningJobConsumedResourcesTypeDef,
     },
-    total=False,
 )
 
 ListInferenceRecommendationsJobStepsResponseTypeDef = TypedDict(
     "ListInferenceRecommendationsJobStepsResponseTypeDef",
     {
         "Steps": List[InferenceRecommendationsJobStepTypeDef],
         "NextToken": str,
@@ -17314,15 +16346,14 @@
     "TrialComponentSourceDetailTypeDef",
     {
         "SourceArn": str,
         "TrainingJob": TrainingJobTypeDef,
         "ProcessingJob": ProcessingJobTypeDef,
         "TransformJob": TransformJobTypeDef,
     },
-    total=False,
 )
 
 MonitoringScheduleConfigTypeDef = TypedDict(
     "MonitoringScheduleConfigTypeDef",
     {
         "ScheduleConfig": ScheduleConfigTypeDef,
         "MonitoringJobDefinition": MonitoringJobDefinitionTypeDef,
@@ -17369,15 +16400,14 @@
         "MetadataProperties": MetadataPropertiesTypeDef,
         "SourceDetail": TrialComponentSourceDetailTypeDef,
         "LineageGroupArn": str,
         "Tags": List[TagTypeDef],
         "Parents": List[ParentTypeDef],
         "RunName": str,
     },
-    total=False,
 )
 
 _RequiredCreateMonitoringScheduleRequestRequestTypeDef = TypedDict(
     "_RequiredCreateMonitoringScheduleRequestRequestTypeDef",
     {
         "MonitoringScheduleName": str,
         "MonitoringScheduleConfig": MonitoringScheduleConfigTypeDef,
@@ -17427,15 +16457,14 @@
         "CreationTime": datetime,
         "LastModifiedTime": datetime,
         "MonitoringScheduleConfig": MonitoringScheduleConfigTypeDef,
         "EndpointName": str,
         "MonitoringAlertSummaries": List[MonitoringAlertSummaryTypeDef],
         "LastMonitoringExecutionSummary": MonitoringExecutionSummaryTypeDef,
     },
-    total=False,
 )
 
 MonitoringScheduleTypeDef = TypedDict(
     "MonitoringScheduleTypeDef",
     {
         "MonitoringScheduleArn": str,
         "MonitoringScheduleName": str,
@@ -17445,15 +16474,14 @@
         "CreationTime": datetime,
         "LastModifiedTime": datetime,
         "MonitoringScheduleConfig": MonitoringScheduleConfigTypeDef,
         "EndpointName": str,
         "LastMonitoringExecutionSummary": MonitoringExecutionSummaryTypeDef,
         "Tags": List[TagTypeDef],
     },
-    total=False,
 )
 
 UpdateMonitoringScheduleRequestRequestTypeDef = TypedDict(
     "UpdateMonitoringScheduleRequestRequestTypeDef",
     {
         "MonitoringScheduleName": str,
         "MonitoringScheduleConfig": MonitoringScheduleConfigTypeDef,
@@ -17593,58 +16621,45 @@
         "AdditionalInferenceSpecifications": List[
             AdditionalInferenceSpecificationDefinitionTypeDef
         ],
         "Tags": List[TagTypeDef],
         "CustomerMetadataProperties": Dict[str, str],
         "DriftCheckBaselines": DriftCheckBaselinesTypeDef,
     },
-    total=False,
 )
 
 ModelDashboardModelTypeDef = TypedDict(
     "ModelDashboardModelTypeDef",
     {
         "Model": ModelTypeDef,
         "Endpoints": List[ModelDashboardEndpointTypeDef],
         "LastBatchTransformJob": TransformJobTypeDef,
         "MonitoringSchedules": List[ModelDashboardMonitoringScheduleTypeDef],
         "ModelCard": ModelDashboardModelCardTypeDef,
     },
-    total=False,
 )
 
-_RequiredEndpointTypeDef = TypedDict(
-    "_RequiredEndpointTypeDef",
+EndpointTypeDef = TypedDict(
+    "EndpointTypeDef",
     {
         "EndpointName": str,
         "EndpointArn": str,
         "EndpointConfigName": str,
-        "EndpointStatus": EndpointStatusType,
-        "CreationTime": datetime,
-        "LastModifiedTime": datetime,
-    },
-)
-_OptionalEndpointTypeDef = TypedDict(
-    "_OptionalEndpointTypeDef",
-    {
         "ProductionVariants": List[ProductionVariantSummaryTypeDef],
         "DataCaptureConfig": DataCaptureConfigSummaryTypeDef,
+        "EndpointStatus": EndpointStatusType,
         "FailureReason": str,
+        "CreationTime": datetime,
+        "LastModifiedTime": datetime,
         "MonitoringSchedules": List[MonitoringScheduleTypeDef],
         "Tags": List[TagTypeDef],
         "ShadowProductionVariants": List[ProductionVariantSummaryTypeDef],
     },
-    total=False,
 )
 
-
-class EndpointTypeDef(_RequiredEndpointTypeDef, _OptionalEndpointTypeDef):
-    pass
-
-
 SearchRecordTypeDef = TypedDict(
     "SearchRecordTypeDef",
     {
         "TrainingJob": TrainingJobTypeDef,
         "Experiment": ExperimentTypeDef,
         "Trial": TrialTypeDef,
         "TrialComponent": TrialComponentTypeDef,
@@ -17656,15 +16671,14 @@
         "FeatureGroup": FeatureGroupTypeDef,
         "Project": ProjectTypeDef,
         "FeatureMetadata": FeatureMetadataTypeDef,
         "HyperParameterTuningJob": HyperParameterTuningJobSearchEntityTypeDef,
         "Model": ModelDashboardModelTypeDef,
         "ModelCard": ModelCardTypeDef,
     },
-    total=False,
 )
 
 SearchResponseTypeDef = TypedDict(
     "SearchResponseTypeDef",
     {
         "Results": List[SearchRecordTypeDef],
         "NextToken": str,
```

### Comparing `mypy-boto3-sagemaker-1.28.0/mypy_boto3_sagemaker/type_defs.pyi` & `mypy-boto3-sagemaker-1.28.3/mypy_boto3_sagemaker/type_defs.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -299,14 +299,15 @@
     "MetricsSourceTypeDef",
     "CacheHitResultTypeDef",
     "OutputParameterTypeDef",
     "CandidateArtifactLocationsTypeDef",
     "MetricDatumTypeDef",
     "ModelRegisterSettingsTypeDef",
     "TimeSeriesForecastingSettingsTypeDef",
+    "WorkspaceSettingsTypeDef",
     "CapacitySizeTypeDef",
     "CaptureContentTypeHeaderTypeDef",
     "CaptureOptionTypeDef",
     "CategoricalParameterRangeSpecificationTypeDef",
     "CategoricalParameterRangeTypeDef",
     "CategoricalParameterTypeDef",
     "ChannelSpecificationTypeDef",
@@ -1458,53 +1459,33 @@
     "MetricDefinitionTypeDef",
     {
         "Name": str,
         "Regex": str,
     },
 )
 
-_RequiredAlgorithmStatusItemTypeDef = TypedDict(
-    "_RequiredAlgorithmStatusItemTypeDef",
+AlgorithmStatusItemTypeDef = TypedDict(
+    "AlgorithmStatusItemTypeDef",
     {
         "Name": str,
         "Status": DetailedAlgorithmStatusType,
-    },
-)
-_OptionalAlgorithmStatusItemTypeDef = TypedDict(
-    "_OptionalAlgorithmStatusItemTypeDef",
-    {
         "FailureReason": str,
     },
-    total=False,
 )
 
-class AlgorithmStatusItemTypeDef(
-    _RequiredAlgorithmStatusItemTypeDef, _OptionalAlgorithmStatusItemTypeDef
-):
-    pass
-
-_RequiredAlgorithmSummaryTypeDef = TypedDict(
-    "_RequiredAlgorithmSummaryTypeDef",
+AlgorithmSummaryTypeDef = TypedDict(
+    "AlgorithmSummaryTypeDef",
     {
         "AlgorithmName": str,
         "AlgorithmArn": str,
+        "AlgorithmDescription": str,
         "CreationTime": datetime,
         "AlgorithmStatus": AlgorithmStatusType,
     },
 )
-_OptionalAlgorithmSummaryTypeDef = TypedDict(
-    "_OptionalAlgorithmSummaryTypeDef",
-    {
-        "AlgorithmDescription": str,
-    },
-    total=False,
-)
-
-class AlgorithmSummaryTypeDef(_RequiredAlgorithmSummaryTypeDef, _OptionalAlgorithmSummaryTypeDef):
-    pass
 
 AnnotationConsolidationConfigTypeDef = TypedDict(
     "AnnotationConsolidationConfigTypeDef",
     {
         "AnnotationConsolidationLambdaArn": str,
     },
 )
@@ -1516,15 +1497,14 @@
         "UserProfileName": str,
         "AppType": AppTypeType,
         "AppName": str,
         "Status": AppStatusType,
         "CreationTime": datetime,
         "SpaceName": str,
     },
-    total=False,
 )
 
 _RequiredAppSpecificationTypeDef = TypedDict(
     "_RequiredAppSpecificationTypeDef",
     {
         "ImageUri": str,
     },
@@ -1621,55 +1601,33 @@
     {
         "CandidateStepType": CandidateStepTypeType,
         "CandidateStepArn": str,
         "CandidateStepName": str,
     },
 )
 
-_RequiredAutoMLContainerDefinitionTypeDef = TypedDict(
-    "_RequiredAutoMLContainerDefinitionTypeDef",
+AutoMLContainerDefinitionTypeDef = TypedDict(
+    "AutoMLContainerDefinitionTypeDef",
     {
         "Image": str,
         "ModelDataUrl": str,
-    },
-)
-_OptionalAutoMLContainerDefinitionTypeDef = TypedDict(
-    "_OptionalAutoMLContainerDefinitionTypeDef",
-    {
         "Environment": Dict[str, str],
     },
-    total=False,
 )
 
-class AutoMLContainerDefinitionTypeDef(
-    _RequiredAutoMLContainerDefinitionTypeDef, _OptionalAutoMLContainerDefinitionTypeDef
-):
-    pass
-
-_RequiredFinalAutoMLJobObjectiveMetricTypeDef = TypedDict(
-    "_RequiredFinalAutoMLJobObjectiveMetricTypeDef",
+FinalAutoMLJobObjectiveMetricTypeDef = TypedDict(
+    "FinalAutoMLJobObjectiveMetricTypeDef",
     {
+        "Type": AutoMLJobObjectiveTypeType,
         "MetricName": AutoMLMetricEnumType,
         "Value": float,
-    },
-)
-_OptionalFinalAutoMLJobObjectiveMetricTypeDef = TypedDict(
-    "_OptionalFinalAutoMLJobObjectiveMetricTypeDef",
-    {
-        "Type": AutoMLJobObjectiveTypeType,
         "StandardMetricName": AutoMLMetricEnumType,
     },
-    total=False,
 )
 
-class FinalAutoMLJobObjectiveMetricTypeDef(
-    _RequiredFinalAutoMLJobObjectiveMetricTypeDef, _OptionalFinalAutoMLJobObjectiveMetricTypeDef
-):
-    pass
-
 AutoMLS3DataSourceTypeDef = TypedDict(
     "AutoMLS3DataSourceTypeDef",
     {
         "S3DataType": AutoMLS3DataTypeType,
         "S3Uri": str,
     },
 )
@@ -1684,15 +1642,14 @@
 
 AutoMLJobArtifactsTypeDef = TypedDict(
     "AutoMLJobArtifactsTypeDef",
     {
         "CandidateDefinitionNotebookLocation": str,
         "DataExplorationNotebookLocation": str,
     },
-    total=False,
 )
 
 AutoMLJobCompletionCriteriaTypeDef = TypedDict(
     "AutoMLJobCompletionCriteriaTypeDef",
     {
         "MaxCandidates": int,
         "MaxRuntimePerTrainingJobInSeconds": int,
@@ -1709,23 +1666,21 @@
 )
 
 AutoMLJobStepMetadataTypeDef = TypedDict(
     "AutoMLJobStepMetadataTypeDef",
     {
         "Arn": str,
     },
-    total=False,
 )
 
 AutoMLPartialFailureReasonTypeDef = TypedDict(
     "AutoMLPartialFailureReasonTypeDef",
     {
         "PartialFailureMessage": str,
     },
-    total=False,
 )
 
 _RequiredAutoMLOutputDataConfigTypeDef = TypedDict(
     "_RequiredAutoMLOutputDataConfigTypeDef",
     {
         "S3OutputPath": str,
     },
@@ -1744,15 +1699,14 @@
     pass
 
 TabularResolvedAttributesTypeDef = TypedDict(
     "TabularResolvedAttributesTypeDef",
     {
         "ProblemType": ProblemTypeType,
     },
-    total=False,
 )
 
 VpcConfigTypeDef = TypedDict(
     "VpcConfigTypeDef",
     {
         "SecurityGroupIds": Sequence[str],
         "Subnets": Sequence[str],
@@ -1836,54 +1790,41 @@
     pass
 
 CacheHitResultTypeDef = TypedDict(
     "CacheHitResultTypeDef",
     {
         "SourcePipelineExecutionArn": str,
     },
-    total=False,
 )
 
 OutputParameterTypeDef = TypedDict(
     "OutputParameterTypeDef",
     {
         "Name": str,
         "Value": str,
     },
 )
 
-_RequiredCandidateArtifactLocationsTypeDef = TypedDict(
-    "_RequiredCandidateArtifactLocationsTypeDef",
+CandidateArtifactLocationsTypeDef = TypedDict(
+    "CandidateArtifactLocationsTypeDef",
     {
         "Explainability": str,
-    },
-)
-_OptionalCandidateArtifactLocationsTypeDef = TypedDict(
-    "_OptionalCandidateArtifactLocationsTypeDef",
-    {
         "ModelInsights": str,
         "BacktestResults": str,
     },
-    total=False,
 )
 
-class CandidateArtifactLocationsTypeDef(
-    _RequiredCandidateArtifactLocationsTypeDef, _OptionalCandidateArtifactLocationsTypeDef
-):
-    pass
-
 MetricDatumTypeDef = TypedDict(
     "MetricDatumTypeDef",
     {
         "MetricName": AutoMLMetricEnumType,
         "Value": float,
         "Set": MetricSetSourceType,
         "StandardMetricName": AutoMLMetricExtendedEnumType,
     },
-    total=False,
 )
 
 ModelRegisterSettingsTypeDef = TypedDict(
     "ModelRegisterSettingsTypeDef",
     {
         "Status": FeatureStatusType,
         "CrossAccountModelRegisterRoleArn": str,
@@ -1896,14 +1837,23 @@
     {
         "Status": FeatureStatusType,
         "AmazonForecastRoleArn": str,
     },
     total=False,
 )
 
+WorkspaceSettingsTypeDef = TypedDict(
+    "WorkspaceSettingsTypeDef",
+    {
+        "S3ArtifactPath": str,
+        "S3KmsKeyId": str,
+    },
+    total=False,
+)
+
 CapacitySizeTypeDef = TypedDict(
     "CapacitySizeTypeDef",
     {
         "Type": CapacitySizeTypeType,
         "Value": int,
     },
 )
@@ -2002,15 +1952,14 @@
         "CalculatedBaselineConstraints": str,
         "ModelPackageGroupName": str,
         "ViolationReport": str,
         "CheckJobArn": str,
         "SkipCheck": bool,
         "RegisterNewBaseline": bool,
     },
-    total=False,
 )
 
 ClarifyInferenceConfigTypeDef = TypedDict(
     "ClarifyInferenceConfigTypeDef",
     {
         "FeaturesAttribute": str,
         "ContentTemplate": str,
@@ -2092,48 +2041,36 @@
     {
         "CollectionName": str,
         "CollectionParameters": Mapping[str, str],
     },
     total=False,
 )
 
-_RequiredCompilationJobSummaryTypeDef = TypedDict(
-    "_RequiredCompilationJobSummaryTypeDef",
+CompilationJobSummaryTypeDef = TypedDict(
+    "CompilationJobSummaryTypeDef",
     {
         "CompilationJobName": str,
         "CompilationJobArn": str,
         "CreationTime": datetime,
-        "CompilationJobStatus": CompilationJobStatusType,
-    },
-)
-_OptionalCompilationJobSummaryTypeDef = TypedDict(
-    "_OptionalCompilationJobSummaryTypeDef",
-    {
         "CompilationStartTime": datetime,
         "CompilationEndTime": datetime,
         "CompilationTargetDevice": TargetDeviceType,
         "CompilationTargetPlatformOs": TargetPlatformOsType,
         "CompilationTargetPlatformArch": TargetPlatformArchType,
         "CompilationTargetPlatformAccelerator": TargetPlatformAcceleratorType,
         "LastModifiedTime": datetime,
+        "CompilationJobStatus": CompilationJobStatusType,
     },
-    total=False,
 )
 
-class CompilationJobSummaryTypeDef(
-    _RequiredCompilationJobSummaryTypeDef, _OptionalCompilationJobSummaryTypeDef
-):
-    pass
-
 ConditionStepMetadataTypeDef = TypedDict(
     "ConditionStepMetadataTypeDef",
     {
         "Outcome": ConditionOutcomeType,
     },
-    total=False,
 )
 
 MultiModelConfigTypeDef = TypedDict(
     "MultiModelConfigTypeDef",
     {
         "ModelCacheSetting": ModelCacheSettingType,
     },
@@ -3413,15 +3350,14 @@
     {
         "RuleConfigurationName": str,
         "RuleEvaluationJobArn": str,
         "RuleEvaluationStatus": RuleEvaluationStatusType,
         "StatusDetails": str,
         "LastModifiedTime": datetime,
     },
-    total=False,
 )
 
 DeleteActionRequestRequestTypeDef = TypedDict(
     "DeleteActionRequestRequestTypeDef",
     {
         "ActionName": str,
     },
@@ -3851,37 +3787,25 @@
 DeployedImageTypeDef = TypedDict(
     "DeployedImageTypeDef",
     {
         "SpecifiedImage": str,
         "ResolvedImage": str,
         "ResolutionTime": datetime,
     },
-    total=False,
 )
 
-_RequiredRealTimeInferenceRecommendationTypeDef = TypedDict(
-    "_RequiredRealTimeInferenceRecommendationTypeDef",
+RealTimeInferenceRecommendationTypeDef = TypedDict(
+    "RealTimeInferenceRecommendationTypeDef",
     {
         "RecommendationId": str,
         "InstanceType": ProductionVariantInstanceTypeType,
-    },
-)
-_OptionalRealTimeInferenceRecommendationTypeDef = TypedDict(
-    "_OptionalRealTimeInferenceRecommendationTypeDef",
-    {
         "Environment": Dict[str, str],
     },
-    total=False,
 )
 
-class RealTimeInferenceRecommendationTypeDef(
-    _RequiredRealTimeInferenceRecommendationTypeDef, _OptionalRealTimeInferenceRecommendationTypeDef
-):
-    pass
-
 _RequiredDeviceSelectionConfigTypeDef = TypedDict(
     "_RequiredDeviceSelectionConfigTypeDef",
     {
         "DeviceSubsetType": DeviceSubsetTypeType,
     },
 )
 _OptionalDeviceSelectionConfigTypeDef = TypedDict(
@@ -3902,37 +3826,26 @@
 EdgeDeploymentConfigTypeDef = TypedDict(
     "EdgeDeploymentConfigTypeDef",
     {
         "FailureHandlingPolicy": FailureHandlingPolicyType,
     },
 )
 
-_RequiredEdgeDeploymentStatusTypeDef = TypedDict(
-    "_RequiredEdgeDeploymentStatusTypeDef",
+EdgeDeploymentStatusTypeDef = TypedDict(
+    "EdgeDeploymentStatusTypeDef",
     {
         "StageStatus": StageStatusType,
         "EdgeDeploymentSuccessInStage": int,
         "EdgeDeploymentPendingInStage": int,
         "EdgeDeploymentFailedInStage": int,
-    },
-)
-_OptionalEdgeDeploymentStatusTypeDef = TypedDict(
-    "_OptionalEdgeDeploymentStatusTypeDef",
-    {
         "EdgeDeploymentStatusMessage": str,
         "EdgeDeploymentStageStartTime": datetime,
     },
-    total=False,
 )
 
-class EdgeDeploymentStatusTypeDef(
-    _RequiredEdgeDeploymentStatusTypeDef, _OptionalEdgeDeploymentStatusTypeDef
-):
-    pass
-
 DeregisterDevicesRequestRequestTypeDef = TypedDict(
     "DeregisterDevicesRequestRequestTypeDef",
     {
         "DeviceFleetName": str,
         "DeviceNames": Sequence[str],
     },
 )
@@ -3995,15 +3908,14 @@
 )
 
 ModelDeployResultTypeDef = TypedDict(
     "ModelDeployResultTypeDef",
     {
         "EndpointName": str,
     },
-    total=False,
 )
 
 DescribeAutoMLJobV2RequestRequestTypeDef = TypedDict(
     "DescribeAutoMLJobV2RequestRequestTypeDef",
     {
         "AutoMLJobName": str,
     },
@@ -4031,15 +3943,14 @@
 )
 
 ModelDigestsTypeDef = TypedDict(
     "ModelDigestsTypeDef",
     {
         "ArtifactDigest": str,
     },
-    total=False,
 )
 
 DescribeContextRequestRequestTypeDef = TypedDict(
     "DescribeContextRequestRequestTypeDef",
     {
         "ContextName": str,
     },
@@ -4075,33 +3986,24 @@
 )
 
 class DescribeDeviceRequestRequestTypeDef(
     _RequiredDescribeDeviceRequestRequestTypeDef, _OptionalDescribeDeviceRequestRequestTypeDef
 ):
     pass
 
-_RequiredEdgeModelTypeDef = TypedDict(
-    "_RequiredEdgeModelTypeDef",
+EdgeModelTypeDef = TypedDict(
+    "EdgeModelTypeDef",
     {
         "ModelName": str,
         "ModelVersion": str,
-    },
-)
-_OptionalEdgeModelTypeDef = TypedDict(
-    "_OptionalEdgeModelTypeDef",
-    {
         "LatestSampleTime": datetime,
         "LatestInference": datetime,
     },
-    total=False,
 )
 
-class EdgeModelTypeDef(_RequiredEdgeModelTypeDef, _OptionalEdgeModelTypeDef):
-    pass
-
 DescribeDomainRequestRequestTypeDef = TypedDict(
     "DescribeDomainRequestRequestTypeDef",
     {
         "DomainId": str,
     },
 )
 
@@ -4129,35 +4031,24 @@
 DescribeEdgePackagingJobRequestRequestTypeDef = TypedDict(
     "DescribeEdgePackagingJobRequestRequestTypeDef",
     {
         "EdgePackagingJobName": str,
     },
 )
 
-_RequiredEdgePresetDeploymentOutputTypeDef = TypedDict(
-    "_RequiredEdgePresetDeploymentOutputTypeDef",
+EdgePresetDeploymentOutputTypeDef = TypedDict(
+    "EdgePresetDeploymentOutputTypeDef",
     {
         "Type": Literal["GreengrassV2Component"],
-    },
-)
-_OptionalEdgePresetDeploymentOutputTypeDef = TypedDict(
-    "_OptionalEdgePresetDeploymentOutputTypeDef",
-    {
         "Artifact": str,
         "Status": EdgePresetDeploymentStatusType,
         "StatusMessage": str,
     },
-    total=False,
 )
 
-class EdgePresetDeploymentOutputTypeDef(
-    _RequiredEdgePresetDeploymentOutputTypeDef, _OptionalEdgePresetDeploymentOutputTypeDef
-):
-    pass
-
 DescribeEndpointConfigInputRequestTypeDef = TypedDict(
     "DescribeEndpointConfigInputRequestTypeDef",
     {
         "EndpointConfigName": str,
     },
 )
 
@@ -4180,31 +4071,22 @@
 DescribeExperimentRequestRequestTypeDef = TypedDict(
     "DescribeExperimentRequestRequestTypeDef",
     {
         "ExperimentName": str,
     },
 )
 
-_RequiredExperimentSourceTypeDef = TypedDict(
-    "_RequiredExperimentSourceTypeDef",
+ExperimentSourceTypeDef = TypedDict(
+    "ExperimentSourceTypeDef",
     {
         "SourceArn": str,
-    },
-)
-_OptionalExperimentSourceTypeDef = TypedDict(
-    "_OptionalExperimentSourceTypeDef",
-    {
         "SourceType": str,
     },
-    total=False,
 )
 
-class ExperimentSourceTypeDef(_RequiredExperimentSourceTypeDef, _OptionalExperimentSourceTypeDef):
-    pass
-
 _RequiredDescribeFeatureGroupRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeFeatureGroupRequestRequestTypeDef",
     {
         "FeatureGroupName": str,
     },
 )
 _OptionalDescribeFeatureGroupRequestRequestTypeDef = TypedDict(
@@ -4217,65 +4099,44 @@
 
 class DescribeFeatureGroupRequestRequestTypeDef(
     _RequiredDescribeFeatureGroupRequestRequestTypeDef,
     _OptionalDescribeFeatureGroupRequestRequestTypeDef,
 ):
     pass
 
-_RequiredLastUpdateStatusTypeDef = TypedDict(
-    "_RequiredLastUpdateStatusTypeDef",
+LastUpdateStatusTypeDef = TypedDict(
+    "LastUpdateStatusTypeDef",
     {
         "Status": LastUpdateStatusValueType,
-    },
-)
-_OptionalLastUpdateStatusTypeDef = TypedDict(
-    "_OptionalLastUpdateStatusTypeDef",
-    {
         "FailureReason": str,
     },
-    total=False,
 )
 
-class LastUpdateStatusTypeDef(_RequiredLastUpdateStatusTypeDef, _OptionalLastUpdateStatusTypeDef):
-    pass
-
-_RequiredOfflineStoreStatusTypeDef = TypedDict(
-    "_RequiredOfflineStoreStatusTypeDef",
+OfflineStoreStatusTypeDef = TypedDict(
+    "OfflineStoreStatusTypeDef",
     {
         "Status": OfflineStoreStatusValueType,
-    },
-)
-_OptionalOfflineStoreStatusTypeDef = TypedDict(
-    "_OptionalOfflineStoreStatusTypeDef",
-    {
         "BlockedReason": str,
     },
-    total=False,
 )
 
-class OfflineStoreStatusTypeDef(
-    _RequiredOfflineStoreStatusTypeDef, _OptionalOfflineStoreStatusTypeDef
-):
-    pass
-
 DescribeFeatureMetadataRequestRequestTypeDef = TypedDict(
     "DescribeFeatureMetadataRequestRequestTypeDef",
     {
         "FeatureGroupName": str,
         "FeatureName": str,
     },
 )
 
 FeatureParameterTypeDef = TypedDict(
     "FeatureParameterTypeDef",
     {
         "Key": str,
         "Value": str,
     },
-    total=False,
 )
 
 DescribeFlowDefinitionRequestRequestTypeDef = TypedDict(
     "DescribeFlowDefinitionRequestRequestTypeDef",
     {
         "FlowDefinitionName": str,
     },
@@ -4305,15 +4166,14 @@
 
 HubContentDependencyTypeDef = TypedDict(
     "HubContentDependencyTypeDef",
     {
         "DependencyOriginPath": str,
         "DependencyCopyPath": str,
     },
-    total=False,
 )
 
 DescribeHubRequestRequestTypeDef = TypedDict(
     "DescribeHubRequestRequestTypeDef",
     {
         "HubName": str,
     },
@@ -4328,15 +4188,14 @@
 
 UiTemplateInfoTypeDef = TypedDict(
     "UiTemplateInfoTypeDef",
     {
         "Url": str,
         "ContentSha256": str,
     },
-    total=False,
 )
 
 DescribeHyperParameterTuningJobRequestRequestTypeDef = TypedDict(
     "DescribeHyperParameterTuningJobRequestRequestTypeDef",
     {
         "HyperParameterTuningJobName": str,
     },
@@ -4344,45 +4203,41 @@
 
 HyperParameterTuningJobCompletionDetailsTypeDef = TypedDict(
     "HyperParameterTuningJobCompletionDetailsTypeDef",
     {
         "NumberOfTrainingJobsObjectiveNotImproving": int,
         "ConvergenceDetectedTime": datetime,
     },
-    total=False,
 )
 
 HyperParameterTuningJobConsumedResourcesTypeDef = TypedDict(
     "HyperParameterTuningJobConsumedResourcesTypeDef",
     {
         "RuntimeInSeconds": int,
     },
-    total=False,
 )
 
 ObjectiveStatusCountersTypeDef = TypedDict(
     "ObjectiveStatusCountersTypeDef",
     {
         "Succeeded": int,
         "Pending": int,
         "Failed": int,
     },
-    total=False,
 )
 
 TrainingJobStatusCountersTypeDef = TypedDict(
     "TrainingJobStatusCountersTypeDef",
     {
         "Completed": int,
         "InProgress": int,
         "RetryableError": int,
         "NonRetryableError": int,
         "Stopped": int,
     },
-    total=False,
 )
 
 DescribeImageRequestRequestTypeDef = TypedDict(
     "DescribeImageRequestRequestTypeDef",
     {
         "ImageName": str,
     },
@@ -4451,33 +4306,24 @@
 DescribeInferenceExperimentRequestRequestTypeDef = TypedDict(
     "DescribeInferenceExperimentRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
-_RequiredEndpointMetadataTypeDef = TypedDict(
-    "_RequiredEndpointMetadataTypeDef",
+EndpointMetadataTypeDef = TypedDict(
+    "EndpointMetadataTypeDef",
     {
         "EndpointName": str,
-    },
-)
-_OptionalEndpointMetadataTypeDef = TypedDict(
-    "_OptionalEndpointMetadataTypeDef",
-    {
         "EndpointConfigName": str,
         "EndpointStatus": EndpointStatusType,
         "FailureReason": str,
     },
-    total=False,
 )
 
-class EndpointMetadataTypeDef(_RequiredEndpointMetadataTypeDef, _OptionalEndpointMetadataTypeDef):
-    pass
-
 DescribeInferenceRecommendationsJobRequestRequestTypeDef = TypedDict(
     "DescribeInferenceRecommendationsJobRequestRequestTypeDef",
     {
         "JobName": str,
     },
 )
 
@@ -4493,36 +4339,24 @@
     {
         "TotalLabeled": int,
         "HumanLabeled": int,
         "MachineLabeled": int,
         "FailedNonRetryableError": int,
         "Unlabeled": int,
     },
-    total=False,
 )
 
-_RequiredLabelingJobOutputTypeDef = TypedDict(
-    "_RequiredLabelingJobOutputTypeDef",
+LabelingJobOutputTypeDef = TypedDict(
+    "LabelingJobOutputTypeDef",
     {
         "OutputDatasetS3Uri": str,
-    },
-)
-_OptionalLabelingJobOutputTypeDef = TypedDict(
-    "_OptionalLabelingJobOutputTypeDef",
-    {
         "FinalActiveLearningModelArn": str,
     },
-    total=False,
 )
 
-class LabelingJobOutputTypeDef(
-    _RequiredLabelingJobOutputTypeDef, _OptionalLabelingJobOutputTypeDef
-):
-    pass
-
 DescribeLineageGroupRequestRequestTypeDef = TypedDict(
     "DescribeLineageGroupRequestRequestTypeDef",
     {
         "LineageGroupName": str,
     },
 )
 
@@ -4604,41 +4438,30 @@
 DescribeMonitoringScheduleRequestRequestTypeDef = TypedDict(
     "DescribeMonitoringScheduleRequestRequestTypeDef",
     {
         "MonitoringScheduleName": str,
     },
 )
 
-_RequiredMonitoringExecutionSummaryTypeDef = TypedDict(
-    "_RequiredMonitoringExecutionSummaryTypeDef",
+MonitoringExecutionSummaryTypeDef = TypedDict(
+    "MonitoringExecutionSummaryTypeDef",
     {
         "MonitoringScheduleName": str,
         "ScheduledTime": datetime,
         "CreationTime": datetime,
         "LastModifiedTime": datetime,
         "MonitoringExecutionStatus": ExecutionStatusType,
-    },
-)
-_OptionalMonitoringExecutionSummaryTypeDef = TypedDict(
-    "_OptionalMonitoringExecutionSummaryTypeDef",
-    {
         "ProcessingJobArn": str,
         "EndpointName": str,
         "FailureReason": str,
         "MonitoringJobDefinitionName": str,
         "MonitoringType": MonitoringTypeType,
     },
-    total=False,
 )
 
-class MonitoringExecutionSummaryTypeDef(
-    _RequiredMonitoringExecutionSummaryTypeDef, _OptionalMonitoringExecutionSummaryTypeDef
-):
-    pass
-
 DescribeNotebookInstanceInputRequestTypeDef = TypedDict(
     "DescribeNotebookInstanceInputRequestTypeDef",
     {
         "NotebookInstanceName": str,
     },
 )
 
@@ -4674,15 +4497,14 @@
 
 PipelineExperimentConfigTypeDef = TypedDict(
     "PipelineExperimentConfigTypeDef",
     {
         "ExperimentName": str,
         "TrialName": str,
     },
-    total=False,
 )
 
 DescribePipelineRequestRequestTypeDef = TypedDict(
     "DescribePipelineRequestRequestTypeDef",
     {
         "PipelineName": str,
     },
@@ -4704,15 +4526,14 @@
 
 ServiceCatalogProvisionedProductDetailsTypeDef = TypedDict(
     "ServiceCatalogProvisionedProductDetailsTypeDef",
     {
         "ProvisionedProductId": str,
         "ProvisionedProductStatusMessage": str,
     },
-    total=False,
 )
 
 DescribeSpaceRequestRequestTypeDef = TypedDict(
     "DescribeSpaceRequestRequestTypeDef",
     {
         "DomainId": str,
         "SpaceName": str,
@@ -4742,104 +4563,71 @@
 DescribeSubscribedWorkteamRequestRequestTypeDef = TypedDict(
     "DescribeSubscribedWorkteamRequestRequestTypeDef",
     {
         "WorkteamArn": str,
     },
 )
 
-_RequiredSubscribedWorkteamTypeDef = TypedDict(
-    "_RequiredSubscribedWorkteamTypeDef",
+SubscribedWorkteamTypeDef = TypedDict(
+    "SubscribedWorkteamTypeDef",
     {
         "WorkteamArn": str,
-    },
-)
-_OptionalSubscribedWorkteamTypeDef = TypedDict(
-    "_OptionalSubscribedWorkteamTypeDef",
-    {
         "MarketplaceTitle": str,
         "SellerName": str,
         "MarketplaceDescription": str,
         "ListingId": str,
     },
-    total=False,
 )
 
-class SubscribedWorkteamTypeDef(
-    _RequiredSubscribedWorkteamTypeDef, _OptionalSubscribedWorkteamTypeDef
-):
-    pass
-
 DescribeTrainingJobRequestRequestTypeDef = TypedDict(
     "DescribeTrainingJobRequestRequestTypeDef",
     {
         "TrainingJobName": str,
     },
 )
 
 MetricDataTypeDef = TypedDict(
     "MetricDataTypeDef",
     {
         "MetricName": str,
         "Value": float,
         "Timestamp": datetime,
     },
-    total=False,
 )
 
 ProfilerRuleEvaluationStatusTypeDef = TypedDict(
     "ProfilerRuleEvaluationStatusTypeDef",
     {
         "RuleConfigurationName": str,
         "RuleEvaluationJobArn": str,
         "RuleEvaluationStatus": RuleEvaluationStatusType,
         "StatusDetails": str,
         "LastModifiedTime": datetime,
     },
-    total=False,
 )
 
-_RequiredSecondaryStatusTransitionTypeDef = TypedDict(
-    "_RequiredSecondaryStatusTransitionTypeDef",
+SecondaryStatusTransitionTypeDef = TypedDict(
+    "SecondaryStatusTransitionTypeDef",
     {
         "Status": SecondaryStatusType,
         "StartTime": datetime,
-    },
-)
-_OptionalSecondaryStatusTransitionTypeDef = TypedDict(
-    "_OptionalSecondaryStatusTransitionTypeDef",
-    {
         "EndTime": datetime,
         "StatusMessage": str,
     },
-    total=False,
 )
 
-class SecondaryStatusTransitionTypeDef(
-    _RequiredSecondaryStatusTransitionTypeDef, _OptionalSecondaryStatusTransitionTypeDef
-):
-    pass
-
-_RequiredWarmPoolStatusTypeDef = TypedDict(
-    "_RequiredWarmPoolStatusTypeDef",
+WarmPoolStatusTypeDef = TypedDict(
+    "WarmPoolStatusTypeDef",
     {
         "Status": WarmPoolResourceStatusType,
-    },
-)
-_OptionalWarmPoolStatusTypeDef = TypedDict(
-    "_OptionalWarmPoolStatusTypeDef",
-    {
         "ResourceRetainedBillableTimeInSeconds": int,
         "ReusedByJob": str,
     },
-    total=False,
 )
 
-class WarmPoolStatusTypeDef(_RequiredWarmPoolStatusTypeDef, _OptionalWarmPoolStatusTypeDef):
-    pass
-
 DescribeTransformJobRequestRequestTypeDef = TypedDict(
     "DescribeTransformJobRequestRequestTypeDef",
     {
         "TransformJobName": str,
     },
 )
 
@@ -4859,60 +4647,39 @@
         "Max": float,
         "Min": float,
         "Last": float,
         "Count": int,
         "Avg": float,
         "StdDev": float,
     },
-    total=False,
 )
 
-_RequiredTrialComponentSourceTypeDef = TypedDict(
-    "_RequiredTrialComponentSourceTypeDef",
+TrialComponentSourceTypeDef = TypedDict(
+    "TrialComponentSourceTypeDef",
     {
         "SourceArn": str,
-    },
-)
-_OptionalTrialComponentSourceTypeDef = TypedDict(
-    "_OptionalTrialComponentSourceTypeDef",
-    {
         "SourceType": str,
     },
-    total=False,
 )
 
-class TrialComponentSourceTypeDef(
-    _RequiredTrialComponentSourceTypeDef, _OptionalTrialComponentSourceTypeDef
-):
-    pass
-
 DescribeTrialRequestRequestTypeDef = TypedDict(
     "DescribeTrialRequestRequestTypeDef",
     {
         "TrialName": str,
     },
 )
 
-_RequiredTrialSourceTypeDef = TypedDict(
-    "_RequiredTrialSourceTypeDef",
+TrialSourceTypeDef = TypedDict(
+    "TrialSourceTypeDef",
     {
         "SourceArn": str,
-    },
-)
-_OptionalTrialSourceTypeDef = TypedDict(
-    "_OptionalTrialSourceTypeDef",
-    {
         "SourceType": str,
     },
-    total=False,
 )
 
-class TrialSourceTypeDef(_RequiredTrialSourceTypeDef, _OptionalTrialSourceTypeDef):
-    pass
-
 DescribeUserProfileRequestRequestTypeDef = TypedDict(
     "DescribeUserProfileRequestRequestTypeDef",
     {
         "DomainId": str,
         "UserProfileName": str,
     },
 )
@@ -4936,63 +4703,41 @@
     {
         "MaxConcurrency": int,
         "ProvisionedConcurrency": int,
     },
     total=False,
 )
 
-_RequiredDeviceDeploymentSummaryTypeDef = TypedDict(
-    "_RequiredDeviceDeploymentSummaryTypeDef",
+DeviceDeploymentSummaryTypeDef = TypedDict(
+    "DeviceDeploymentSummaryTypeDef",
     {
         "EdgeDeploymentPlanArn": str,
         "EdgeDeploymentPlanName": str,
         "StageName": str,
-        "DeviceName": str,
-        "DeviceArn": str,
-    },
-)
-_OptionalDeviceDeploymentSummaryTypeDef = TypedDict(
-    "_OptionalDeviceDeploymentSummaryTypeDef",
-    {
         "DeployedStageName": str,
         "DeviceFleetName": str,
+        "DeviceName": str,
+        "DeviceArn": str,
         "DeviceDeploymentStatus": DeviceDeploymentStatusType,
         "DeviceDeploymentStatusMessage": str,
         "Description": str,
         "DeploymentStartTime": datetime,
     },
-    total=False,
 )
 
-class DeviceDeploymentSummaryTypeDef(
-    _RequiredDeviceDeploymentSummaryTypeDef, _OptionalDeviceDeploymentSummaryTypeDef
-):
-    pass
-
-_RequiredDeviceFleetSummaryTypeDef = TypedDict(
-    "_RequiredDeviceFleetSummaryTypeDef",
+DeviceFleetSummaryTypeDef = TypedDict(
+    "DeviceFleetSummaryTypeDef",
     {
         "DeviceFleetArn": str,
         "DeviceFleetName": str,
-    },
-)
-_OptionalDeviceFleetSummaryTypeDef = TypedDict(
-    "_OptionalDeviceFleetSummaryTypeDef",
-    {
         "CreationTime": datetime,
         "LastModifiedTime": datetime,
     },
-    total=False,
 )
 
-class DeviceFleetSummaryTypeDef(
-    _RequiredDeviceFleetSummaryTypeDef, _OptionalDeviceFleetSummaryTypeDef
-):
-    pass
-
 DeviceStatsTypeDef = TypedDict(
     "DeviceStatsTypeDef",
     {
         "ConnectedDeviceCount": int,
         "RegisteredDeviceCount": int,
     },
 )
@@ -5047,15 +4792,14 @@
         "DomainId": str,
         "DomainName": str,
         "Status": DomainStatusType,
         "CreationTime": datetime,
         "LastModifiedTime": datetime,
         "Url": str,
     },
-    total=False,
 )
 
 _RequiredFileSourceTypeDef = TypedDict(
     "_RequiredFileSourceTypeDef",
     {
         "S3Uri": str,
     },
@@ -5076,87 +4820,63 @@
     "EMRStepMetadataTypeDef",
     {
         "ClusterId": str,
         "StepId": str,
         "StepName": str,
         "LogFilePath": str,
     },
-    total=False,
 )
 
-_RequiredEdgeDeploymentPlanSummaryTypeDef = TypedDict(
-    "_RequiredEdgeDeploymentPlanSummaryTypeDef",
+EdgeDeploymentPlanSummaryTypeDef = TypedDict(
+    "EdgeDeploymentPlanSummaryTypeDef",
     {
         "EdgeDeploymentPlanArn": str,
         "EdgeDeploymentPlanName": str,
         "DeviceFleetName": str,
         "EdgeDeploymentSuccess": int,
         "EdgeDeploymentPending": int,
         "EdgeDeploymentFailed": int,
-    },
-)
-_OptionalEdgeDeploymentPlanSummaryTypeDef = TypedDict(
-    "_OptionalEdgeDeploymentPlanSummaryTypeDef",
-    {
         "CreationTime": datetime,
         "LastModifiedTime": datetime,
     },
-    total=False,
 )
 
-class EdgeDeploymentPlanSummaryTypeDef(
-    _RequiredEdgeDeploymentPlanSummaryTypeDef, _OptionalEdgeDeploymentPlanSummaryTypeDef
-):
-    pass
-
 EdgeModelStatTypeDef = TypedDict(
     "EdgeModelStatTypeDef",
     {
         "ModelName": str,
         "ModelVersion": str,
         "OfflineDeviceCount": int,
         "ConnectedDeviceCount": int,
         "ActiveDeviceCount": int,
         "SamplingDeviceCount": int,
     },
 )
 
-_RequiredEdgePackagingJobSummaryTypeDef = TypedDict(
-    "_RequiredEdgePackagingJobSummaryTypeDef",
+EdgePackagingJobSummaryTypeDef = TypedDict(
+    "EdgePackagingJobSummaryTypeDef",
     {
         "EdgePackagingJobArn": str,
         "EdgePackagingJobName": str,
         "EdgePackagingJobStatus": EdgePackagingJobStatusType,
-    },
-)
-_OptionalEdgePackagingJobSummaryTypeDef = TypedDict(
-    "_OptionalEdgePackagingJobSummaryTypeDef",
-    {
         "CompilationJobName": str,
         "ModelName": str,
         "ModelVersion": str,
         "CreationTime": datetime,
         "LastModifiedTime": datetime,
     },
-    total=False,
 )
 
-class EdgePackagingJobSummaryTypeDef(
-    _RequiredEdgePackagingJobSummaryTypeDef, _OptionalEdgePackagingJobSummaryTypeDef
-):
-    pass
-
 EdgeTypeDef = TypedDict(
     "EdgeTypeDef",
     {
         "SourceArn": str,
         "DestinationArn": str,
         "AssociationType": AssociationEdgeTypeType,
     },
-    total=False,
 )
 
 EmptyResponseMetadataTypeDef = TypedDict(
     "EmptyResponseMetadataTypeDef",
     {
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -5228,15 +4948,14 @@
 )
 
 FailStepMetadataTypeDef = TypedDict(
     "FailStepMetadataTypeDef",
     {
         "ErrorMessage": str,
     },
-    total=False,
 )
 
 FileSystemConfigTypeDef = TypedDict(
     "FileSystemConfigTypeDef",
     {
         "MountPath": str,
         "DefaultUid": int,
@@ -5259,57 +4978,34 @@
     },
     total=False,
 )
 
 class FilterTypeDef(_RequiredFilterTypeDef, _OptionalFilterTypeDef):
     pass
 
-_RequiredFinalHyperParameterTuningJobObjectiveMetricTypeDef = TypedDict(
-    "_RequiredFinalHyperParameterTuningJobObjectiveMetricTypeDef",
+FinalHyperParameterTuningJobObjectiveMetricTypeDef = TypedDict(
+    "FinalHyperParameterTuningJobObjectiveMetricTypeDef",
     {
+        "Type": HyperParameterTuningJobObjectiveTypeType,
         "MetricName": str,
         "Value": float,
     },
 )
-_OptionalFinalHyperParameterTuningJobObjectiveMetricTypeDef = TypedDict(
-    "_OptionalFinalHyperParameterTuningJobObjectiveMetricTypeDef",
-    {
-        "Type": HyperParameterTuningJobObjectiveTypeType,
-    },
-    total=False,
-)
-
-class FinalHyperParameterTuningJobObjectiveMetricTypeDef(
-    _RequiredFinalHyperParameterTuningJobObjectiveMetricTypeDef,
-    _OptionalFinalHyperParameterTuningJobObjectiveMetricTypeDef,
-):
-    pass
 
-_RequiredFlowDefinitionSummaryTypeDef = TypedDict(
-    "_RequiredFlowDefinitionSummaryTypeDef",
+FlowDefinitionSummaryTypeDef = TypedDict(
+    "FlowDefinitionSummaryTypeDef",
     {
         "FlowDefinitionName": str,
         "FlowDefinitionArn": str,
         "FlowDefinitionStatus": FlowDefinitionStatusType,
         "CreationTime": datetime,
-    },
-)
-_OptionalFlowDefinitionSummaryTypeDef = TypedDict(
-    "_OptionalFlowDefinitionSummaryTypeDef",
-    {
         "FailureReason": str,
     },
-    total=False,
 )
 
-class FlowDefinitionSummaryTypeDef(
-    _RequiredFlowDefinitionSummaryTypeDef, _OptionalFlowDefinitionSummaryTypeDef
-):
-    pass
-
 GetDeviceFleetReportRequestRequestTypeDef = TypedDict(
     "GetDeviceFleetReportRequestRequestTypeDef",
     {
         "DeviceFleetName": str,
     },
 )
 
@@ -5353,73 +5049,54 @@
 )
 
 PropertyNameSuggestionTypeDef = TypedDict(
     "PropertyNameSuggestionTypeDef",
     {
         "PropertyName": str,
     },
-    total=False,
 )
 
 GitConfigForUpdateTypeDef = TypedDict(
     "GitConfigForUpdateTypeDef",
     {
         "SecretArn": str,
     },
     total=False,
 )
 
-_RequiredHubContentInfoTypeDef = TypedDict(
-    "_RequiredHubContentInfoTypeDef",
+HubContentInfoTypeDef = TypedDict(
+    "HubContentInfoTypeDef",
     {
         "HubContentName": str,
         "HubContentArn": str,
         "HubContentVersion": str,
         "HubContentType": HubContentTypeType,
         "DocumentSchemaVersion": str,
-        "HubContentStatus": HubContentStatusType,
-        "CreationTime": datetime,
-    },
-)
-_OptionalHubContentInfoTypeDef = TypedDict(
-    "_OptionalHubContentInfoTypeDef",
-    {
         "HubContentDisplayName": str,
         "HubContentDescription": str,
         "HubContentSearchKeywords": List[str],
+        "HubContentStatus": HubContentStatusType,
+        "CreationTime": datetime,
     },
-    total=False,
 )
 
-class HubContentInfoTypeDef(_RequiredHubContentInfoTypeDef, _OptionalHubContentInfoTypeDef):
-    pass
-
-_RequiredHubInfoTypeDef = TypedDict(
-    "_RequiredHubInfoTypeDef",
+HubInfoTypeDef = TypedDict(
+    "HubInfoTypeDef",
     {
         "HubName": str,
         "HubArn": str,
-        "HubStatus": HubStatusType,
-        "CreationTime": datetime,
-        "LastModifiedTime": datetime,
-    },
-)
-_OptionalHubInfoTypeDef = TypedDict(
-    "_OptionalHubInfoTypeDef",
-    {
         "HubDisplayName": str,
         "HubDescription": str,
         "HubSearchKeywords": List[str],
+        "HubStatus": HubStatusType,
+        "CreationTime": datetime,
+        "LastModifiedTime": datetime,
     },
-    total=False,
 )
 
-class HubInfoTypeDef(_RequiredHubInfoTypeDef, _OptionalHubInfoTypeDef):
-    pass
-
 HumanLoopActivationConditionsConfigTypeDef = TypedDict(
     "HumanLoopActivationConditionsConfigTypeDef",
     {
         "HumanLoopActivationConditions": str,
     },
 )
 
@@ -5496,132 +5173,91 @@
 IamIdentityTypeDef = TypedDict(
     "IamIdentityTypeDef",
     {
         "Arn": str,
         "PrincipalId": str,
         "SourceIdentity": str,
     },
-    total=False,
 )
 
 RepositoryAuthConfigTypeDef = TypedDict(
     "RepositoryAuthConfigTypeDef",
     {
         "RepositoryCredentialsProviderArn": str,
     },
 )
 
-_RequiredImageTypeDef = TypedDict(
-    "_RequiredImageTypeDef",
+ImageTypeDef = TypedDict(
+    "ImageTypeDef",
     {
         "CreationTime": datetime,
+        "Description": str,
+        "DisplayName": str,
+        "FailureReason": str,
         "ImageArn": str,
         "ImageName": str,
         "ImageStatus": ImageStatusType,
         "LastModifiedTime": datetime,
     },
 )
-_OptionalImageTypeDef = TypedDict(
-    "_OptionalImageTypeDef",
-    {
-        "Description": str,
-        "DisplayName": str,
-        "FailureReason": str,
-    },
-    total=False,
-)
-
-class ImageTypeDef(_RequiredImageTypeDef, _OptionalImageTypeDef):
-    pass
 
-_RequiredImageVersionTypeDef = TypedDict(
-    "_RequiredImageVersionTypeDef",
+ImageVersionTypeDef = TypedDict(
+    "ImageVersionTypeDef",
     {
         "CreationTime": datetime,
+        "FailureReason": str,
         "ImageArn": str,
         "ImageVersionArn": str,
         "ImageVersionStatus": ImageVersionStatusType,
         "LastModifiedTime": datetime,
         "Version": int,
     },
 )
-_OptionalImageVersionTypeDef = TypedDict(
-    "_OptionalImageVersionTypeDef",
-    {
-        "FailureReason": str,
-    },
-    total=False,
-)
-
-class ImageVersionTypeDef(_RequiredImageVersionTypeDef, _OptionalImageVersionTypeDef):
-    pass
 
 ImportHubContentResponseTypeDef = TypedDict(
     "ImportHubContentResponseTypeDef",
     {
         "HubArn": str,
         "HubContentArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredRecommendationMetricsTypeDef = TypedDict(
-    "_RequiredRecommendationMetricsTypeDef",
+RecommendationMetricsTypeDef = TypedDict(
+    "RecommendationMetricsTypeDef",
     {
         "CostPerHour": float,
         "CostPerInference": float,
         "MaxInvocations": int,
         "ModelLatency": int,
-    },
-)
-_OptionalRecommendationMetricsTypeDef = TypedDict(
-    "_OptionalRecommendationMetricsTypeDef",
-    {
         "CpuUtilization": float,
         "MemoryUtilization": float,
         "ModelSetupTime": int,
     },
-    total=False,
 )
 
-class RecommendationMetricsTypeDef(
-    _RequiredRecommendationMetricsTypeDef, _OptionalRecommendationMetricsTypeDef
-):
-    pass
-
-_RequiredInferenceRecommendationsJobTypeDef = TypedDict(
-    "_RequiredInferenceRecommendationsJobTypeDef",
+InferenceRecommendationsJobTypeDef = TypedDict(
+    "InferenceRecommendationsJobTypeDef",
     {
         "JobName": str,
         "JobDescription": str,
         "JobType": RecommendationJobTypeType,
         "JobArn": str,
         "Status": RecommendationJobStatusType,
         "CreationTime": datetime,
+        "CompletionTime": datetime,
         "RoleArn": str,
         "LastModifiedTime": datetime,
-    },
-)
-_OptionalInferenceRecommendationsJobTypeDef = TypedDict(
-    "_OptionalInferenceRecommendationsJobTypeDef",
-    {
-        "CompletionTime": datetime,
         "FailureReason": str,
         "ModelName": str,
         "SamplePayloadUrl": str,
         "ModelPackageVersionArn": str,
     },
-    total=False,
 )
 
-class InferenceRecommendationsJobTypeDef(
-    _RequiredInferenceRecommendationsJobTypeDef, _OptionalInferenceRecommendationsJobTypeDef
-):
-    pass
-
 InstanceGroupTypeDef = TypedDict(
     "InstanceGroupTypeDef",
     {
         "InstanceType": TrainingInstanceTypeType,
         "InstanceCount": int,
         "InstanceGroupName": str,
     },
@@ -5676,15 +5312,14 @@
 LabelCountersForWorkteamTypeDef = TypedDict(
     "LabelCountersForWorkteamTypeDef",
     {
         "HumanLabeled": int,
         "PendingHuman": int,
         "Total": int,
     },
-    total=False,
 )
 
 LabelingJobDataAttributesTypeDef = TypedDict(
     "LabelingJobDataAttributesTypeDef",
     {
         "ContentClassifiers": Sequence[ContentClassifierType],
     },
@@ -5710,15 +5345,14 @@
     {
         "LineageGroupArn": str,
         "LineageGroupName": str,
         "DisplayName": str,
         "CreationTime": datetime,
         "LastModifiedTime": datetime,
     },
-    total=False,
 )
 
 ListActionsRequestListActionsPaginateTypeDef = TypedDict(
     "ListActionsRequestListActionsPaginateTypeDef",
     {
         "SourceUri": str,
         "ActionType": str,
@@ -7021,37 +6655,26 @@
 
 class ListModelCardVersionsRequestRequestTypeDef(
     _RequiredListModelCardVersionsRequestRequestTypeDef,
     _OptionalListModelCardVersionsRequestRequestTypeDef,
 ):
     pass
 
-_RequiredModelCardVersionSummaryTypeDef = TypedDict(
-    "_RequiredModelCardVersionSummaryTypeDef",
+ModelCardVersionSummaryTypeDef = TypedDict(
+    "ModelCardVersionSummaryTypeDef",
     {
         "ModelCardName": str,
         "ModelCardArn": str,
         "ModelCardStatus": ModelCardStatusType,
         "ModelCardVersion": int,
         "CreationTime": datetime,
-    },
-)
-_OptionalModelCardVersionSummaryTypeDef = TypedDict(
-    "_OptionalModelCardVersionSummaryTypeDef",
-    {
         "LastModifiedTime": datetime,
     },
-    total=False,
 )
 
-class ModelCardVersionSummaryTypeDef(
-    _RequiredModelCardVersionSummaryTypeDef, _OptionalModelCardVersionSummaryTypeDef
-):
-    pass
-
 ListModelCardsRequestListModelCardsPaginateTypeDef = TypedDict(
     "ListModelCardsRequestListModelCardsPaginateTypeDef",
     {
         "CreationTimeAfter": Union[datetime, str],
         "CreationTimeBefore": Union[datetime, str],
         "NameContains": str,
         "ModelCardStatus": ModelCardStatusType,
@@ -7073,34 +6696,25 @@
         "NextToken": str,
         "SortBy": ModelCardSortByType,
         "SortOrder": ModelCardSortOrderType,
     },
     total=False,
 )
 
-_RequiredModelCardSummaryTypeDef = TypedDict(
-    "_RequiredModelCardSummaryTypeDef",
+ModelCardSummaryTypeDef = TypedDict(
+    "ModelCardSummaryTypeDef",
     {
         "ModelCardName": str,
         "ModelCardArn": str,
         "ModelCardStatus": ModelCardStatusType,
         "CreationTime": datetime,
-    },
-)
-_OptionalModelCardSummaryTypeDef = TypedDict(
-    "_OptionalModelCardSummaryTypeDef",
-    {
         "LastModifiedTime": datetime,
     },
-    total=False,
 )
 
-class ModelCardSummaryTypeDef(_RequiredModelCardSummaryTypeDef, _OptionalModelCardSummaryTypeDef):
-    pass
-
 ListModelExplainabilityJobDefinitionsRequestListModelExplainabilityJobDefinitionsPaginateTypeDef = TypedDict(
     "ListModelExplainabilityJobDefinitionsRequestListModelExplainabilityJobDefinitionsPaginateTypeDef",
     {
         "EndpointName": str,
         "SortBy": MonitoringJobDefinitionSortKeyType,
         "SortOrder": SortOrderType,
         "NameContains": str,
@@ -7160,35 +6774,24 @@
         "NextToken": str,
         "SortBy": ModelPackageGroupSortByType,
         "SortOrder": SortOrderType,
     },
     total=False,
 )
 
-_RequiredModelPackageGroupSummaryTypeDef = TypedDict(
-    "_RequiredModelPackageGroupSummaryTypeDef",
+ModelPackageGroupSummaryTypeDef = TypedDict(
+    "ModelPackageGroupSummaryTypeDef",
     {
         "ModelPackageGroupName": str,
         "ModelPackageGroupArn": str,
+        "ModelPackageGroupDescription": str,
         "CreationTime": datetime,
         "ModelPackageGroupStatus": ModelPackageGroupStatusType,
     },
 )
-_OptionalModelPackageGroupSummaryTypeDef = TypedDict(
-    "_OptionalModelPackageGroupSummaryTypeDef",
-    {
-        "ModelPackageGroupDescription": str,
-    },
-    total=False,
-)
-
-class ModelPackageGroupSummaryTypeDef(
-    _RequiredModelPackageGroupSummaryTypeDef, _OptionalModelPackageGroupSummaryTypeDef
-):
-    pass
 
 ListModelPackagesInputListModelPackagesPaginateTypeDef = TypedDict(
     "ListModelPackagesInputListModelPackagesPaginateTypeDef",
     {
         "CreationTimeAfter": Union[datetime, str],
         "CreationTimeBefore": Union[datetime, str],
         "NameContains": str,
@@ -7215,39 +6818,28 @@
         "NextToken": str,
         "SortBy": ModelPackageSortByType,
         "SortOrder": SortOrderType,
     },
     total=False,
 )
 
-_RequiredModelPackageSummaryTypeDef = TypedDict(
-    "_RequiredModelPackageSummaryTypeDef",
+ModelPackageSummaryTypeDef = TypedDict(
+    "ModelPackageSummaryTypeDef",
     {
         "ModelPackageName": str,
-        "ModelPackageArn": str,
-        "CreationTime": datetime,
-        "ModelPackageStatus": ModelPackageStatusType,
-    },
-)
-_OptionalModelPackageSummaryTypeDef = TypedDict(
-    "_OptionalModelPackageSummaryTypeDef",
-    {
         "ModelPackageGroupName": str,
         "ModelPackageVersion": int,
+        "ModelPackageArn": str,
         "ModelPackageDescription": str,
+        "CreationTime": datetime,
+        "ModelPackageStatus": ModelPackageStatusType,
         "ModelApprovalStatus": ModelApprovalStatusType,
     },
-    total=False,
 )
 
-class ModelPackageSummaryTypeDef(
-    _RequiredModelPackageSummaryTypeDef, _OptionalModelPackageSummaryTypeDef
-):
-    pass
-
 ListModelQualityJobDefinitionsRequestListModelQualityJobDefinitionsPaginateTypeDef = TypedDict(
     "ListModelQualityJobDefinitionsRequestListModelQualityJobDefinitionsPaginateTypeDef",
     {
         "EndpointName": str,
         "SortBy": MonitoringJobDefinitionSortKeyType,
         "SortOrder": SortOrderType,
         "NameContains": str,
@@ -7469,39 +7061,28 @@
         "StatusEquals": ScheduleStatusType,
         "MonitoringJobDefinitionName": str,
         "MonitoringTypeEquals": MonitoringTypeType,
     },
     total=False,
 )
 
-_RequiredMonitoringScheduleSummaryTypeDef = TypedDict(
-    "_RequiredMonitoringScheduleSummaryTypeDef",
+MonitoringScheduleSummaryTypeDef = TypedDict(
+    "MonitoringScheduleSummaryTypeDef",
     {
         "MonitoringScheduleName": str,
         "MonitoringScheduleArn": str,
         "CreationTime": datetime,
         "LastModifiedTime": datetime,
         "MonitoringScheduleStatus": ScheduleStatusType,
-    },
-)
-_OptionalMonitoringScheduleSummaryTypeDef = TypedDict(
-    "_OptionalMonitoringScheduleSummaryTypeDef",
-    {
         "EndpointName": str,
         "MonitoringJobDefinitionName": str,
         "MonitoringType": MonitoringTypeType,
     },
-    total=False,
 )
 
-class MonitoringScheduleSummaryTypeDef(
-    _RequiredMonitoringScheduleSummaryTypeDef, _OptionalMonitoringScheduleSummaryTypeDef
-):
-    pass
-
 ListNotebookInstanceLifecycleConfigsInputListNotebookInstanceLifecycleConfigsPaginateTypeDef = TypedDict(
     "ListNotebookInstanceLifecycleConfigsInputListNotebookInstanceLifecycleConfigsPaginateTypeDef",
     {
         "SortBy": NotebookInstanceLifecycleConfigSortKeyType,
         "SortOrder": NotebookInstanceLifecycleConfigSortOrderType,
         "NameContains": str,
         "CreationTimeBefore": Union[datetime, str],
@@ -7525,36 +7106,24 @@
         "CreationTimeAfter": Union[datetime, str],
         "LastModifiedTimeBefore": Union[datetime, str],
         "LastModifiedTimeAfter": Union[datetime, str],
     },
     total=False,
 )
 
-_RequiredNotebookInstanceLifecycleConfigSummaryTypeDef = TypedDict(
-    "_RequiredNotebookInstanceLifecycleConfigSummaryTypeDef",
+NotebookInstanceLifecycleConfigSummaryTypeDef = TypedDict(
+    "NotebookInstanceLifecycleConfigSummaryTypeDef",
     {
         "NotebookInstanceLifecycleConfigName": str,
         "NotebookInstanceLifecycleConfigArn": str,
-    },
-)
-_OptionalNotebookInstanceLifecycleConfigSummaryTypeDef = TypedDict(
-    "_OptionalNotebookInstanceLifecycleConfigSummaryTypeDef",
-    {
         "CreationTime": datetime,
         "LastModifiedTime": datetime,
     },
-    total=False,
 )
 
-class NotebookInstanceLifecycleConfigSummaryTypeDef(
-    _RequiredNotebookInstanceLifecycleConfigSummaryTypeDef,
-    _OptionalNotebookInstanceLifecycleConfigSummaryTypeDef,
-):
-    pass
-
 ListNotebookInstancesInputListNotebookInstancesPaginateTypeDef = TypedDict(
     "ListNotebookInstancesInputListNotebookInstancesPaginateTypeDef",
     {
         "SortBy": NotebookInstanceSortKeyType,
         "SortOrder": NotebookInstanceSortOrderType,
         "NameContains": str,
         "CreationTimeBefore": Union[datetime, str],
@@ -7586,41 +7155,30 @@
         "NotebookInstanceLifecycleConfigNameContains": str,
         "DefaultCodeRepositoryContains": str,
         "AdditionalCodeRepositoryEquals": str,
     },
     total=False,
 )
 
-_RequiredNotebookInstanceSummaryTypeDef = TypedDict(
-    "_RequiredNotebookInstanceSummaryTypeDef",
+NotebookInstanceSummaryTypeDef = TypedDict(
+    "NotebookInstanceSummaryTypeDef",
     {
         "NotebookInstanceName": str,
         "NotebookInstanceArn": str,
-    },
-)
-_OptionalNotebookInstanceSummaryTypeDef = TypedDict(
-    "_OptionalNotebookInstanceSummaryTypeDef",
-    {
         "NotebookInstanceStatus": NotebookInstanceStatusType,
         "Url": str,
         "InstanceType": InstanceTypeType,
         "CreationTime": datetime,
         "LastModifiedTime": datetime,
         "NotebookInstanceLifecycleConfigName": str,
         "DefaultCodeRepository": str,
         "AdditionalCodeRepositories": List[str],
     },
-    total=False,
 )
 
-class NotebookInstanceSummaryTypeDef(
-    _RequiredNotebookInstanceSummaryTypeDef, _OptionalNotebookInstanceSummaryTypeDef
-):
-    pass
-
 ListPipelineExecutionStepsRequestListPipelineExecutionStepsPaginateTypeDef = TypedDict(
     "ListPipelineExecutionStepsRequestListPipelineExecutionStepsPaginateTypeDef",
     {
         "PipelineExecutionArn": str,
         "SortOrder": SortOrderType,
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
@@ -7693,15 +7251,14 @@
         "PipelineExecutionArn": str,
         "StartTime": datetime,
         "PipelineExecutionStatus": PipelineExecutionStatusType,
         "PipelineExecutionDescription": str,
         "PipelineExecutionDisplayName": str,
         "PipelineExecutionFailureReason": str,
     },
-    total=False,
 )
 
 _RequiredListPipelineParametersForExecutionRequestListPipelineParametersForExecutionPaginateTypeDef = TypedDict(
     "_RequiredListPipelineParametersForExecutionRequestListPipelineParametersForExecutionPaginateTypeDef",
     {
         "PipelineExecutionArn": str,
     },
@@ -7784,15 +7341,14 @@
         "PipelineDisplayName": str,
         "PipelineDescription": str,
         "RoleArn": str,
         "CreationTime": datetime,
         "LastModifiedTime": datetime,
         "LastExecutionTime": datetime,
     },
-    total=False,
 )
 
 ListProcessingJobsRequestListProcessingJobsPaginateTypeDef = TypedDict(
     "ListProcessingJobsRequestListProcessingJobsPaginateTypeDef",
     {
         "CreationTimeAfter": Union[datetime, str],
         "CreationTimeBefore": Union[datetime, str],
@@ -7820,73 +7376,53 @@
         "SortOrder": SortOrderType,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-_RequiredProcessingJobSummaryTypeDef = TypedDict(
-    "_RequiredProcessingJobSummaryTypeDef",
+ProcessingJobSummaryTypeDef = TypedDict(
+    "ProcessingJobSummaryTypeDef",
     {
         "ProcessingJobName": str,
         "ProcessingJobArn": str,
         "CreationTime": datetime,
-        "ProcessingJobStatus": ProcessingJobStatusType,
-    },
-)
-_OptionalProcessingJobSummaryTypeDef = TypedDict(
-    "_OptionalProcessingJobSummaryTypeDef",
-    {
         "ProcessingEndTime": datetime,
         "LastModifiedTime": datetime,
+        "ProcessingJobStatus": ProcessingJobStatusType,
         "FailureReason": str,
         "ExitMessage": str,
     },
-    total=False,
 )
 
-class ProcessingJobSummaryTypeDef(
-    _RequiredProcessingJobSummaryTypeDef, _OptionalProcessingJobSummaryTypeDef
-):
-    pass
-
 ListProjectsInputRequestTypeDef = TypedDict(
     "ListProjectsInputRequestTypeDef",
     {
         "CreationTimeAfter": Union[datetime, str],
         "CreationTimeBefore": Union[datetime, str],
         "MaxResults": int,
         "NameContains": str,
         "NextToken": str,
         "SortBy": ProjectSortByType,
         "SortOrder": ProjectSortOrderType,
     },
     total=False,
 )
 
-_RequiredProjectSummaryTypeDef = TypedDict(
-    "_RequiredProjectSummaryTypeDef",
+ProjectSummaryTypeDef = TypedDict(
+    "ProjectSummaryTypeDef",
     {
         "ProjectName": str,
+        "ProjectDescription": str,
         "ProjectArn": str,
         "ProjectId": str,
         "CreationTime": datetime,
         "ProjectStatus": ProjectStatusType,
     },
 )
-_OptionalProjectSummaryTypeDef = TypedDict(
-    "_OptionalProjectSummaryTypeDef",
-    {
-        "ProjectDescription": str,
-    },
-    total=False,
-)
-
-class ProjectSummaryTypeDef(_RequiredProjectSummaryTypeDef, _OptionalProjectSummaryTypeDef):
-    pass
 
 ListSpacesRequestListSpacesPaginateTypeDef = TypedDict(
     "ListSpacesRequestListSpacesPaginateTypeDef",
     {
         "SortOrder": SortOrderType,
         "SortBy": SpaceSortKeyType,
         "DomainIdEquals": str,
@@ -7914,15 +7450,14 @@
     {
         "DomainId": str,
         "SpaceName": str,
         "Status": SpaceStatusType,
         "CreationTime": datetime,
         "LastModifiedTime": datetime,
     },
-    total=False,
 )
 
 _RequiredListStageDevicesRequestListStageDevicesPaginateTypeDef = TypedDict(
     "_RequiredListStageDevicesRequestListStageDevicesPaginateTypeDef",
     {
         "EdgeDeploymentPlanName": str,
         "StageName": str,
@@ -8003,15 +7538,14 @@
     {
         "StudioLifecycleConfigArn": str,
         "StudioLifecycleConfigName": str,
         "CreationTime": datetime,
         "LastModifiedTime": datetime,
         "StudioLifecycleConfigAppType": StudioLifecycleConfigAppTypeType,
     },
-    total=False,
 )
 
 ListSubscribedWorkteamsRequestListSubscribedWorkteamsPaginateTypeDef = TypedDict(
     "ListSubscribedWorkteamsRequestListSubscribedWorkteamsPaginateTypeDef",
     {
         "NameContains": str,
         "PaginationConfig": "PaginatorConfigTypeDef",
@@ -8179,38 +7713,27 @@
         "SortOrder": SortOrderType,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-_RequiredTransformJobSummaryTypeDef = TypedDict(
-    "_RequiredTransformJobSummaryTypeDef",
+TransformJobSummaryTypeDef = TypedDict(
+    "TransformJobSummaryTypeDef",
     {
         "TransformJobName": str,
         "TransformJobArn": str,
         "CreationTime": datetime,
-        "TransformJobStatus": TransformJobStatusType,
-    },
-)
-_OptionalTransformJobSummaryTypeDef = TypedDict(
-    "_OptionalTransformJobSummaryTypeDef",
-    {
         "TransformEndTime": datetime,
         "LastModifiedTime": datetime,
+        "TransformJobStatus": TransformJobStatusType,
         "FailureReason": str,
     },
-    total=False,
 )
 
-class TransformJobSummaryTypeDef(
-    _RequiredTransformJobSummaryTypeDef, _OptionalTransformJobSummaryTypeDef
-):
-    pass
-
 ListTrialComponentsRequestListTrialComponentsPaginateTypeDef = TypedDict(
     "ListTrialComponentsRequestListTrialComponentsPaginateTypeDef",
     {
         "ExperimentName": str,
         "TrialName": str,
         "SourceArn": str,
         "CreatedAfter": Union[datetime, str],
@@ -8297,15 +7820,14 @@
     {
         "DomainId": str,
         "UserProfileName": str,
         "Status": UserProfileStatusType,
         "CreationTime": datetime,
         "LastModifiedTime": datetime,
     },
-    total=False,
 )
 
 ListWorkforcesRequestListWorkforcesPaginateTypeDef = TypedDict(
     "ListWorkforcesRequestListWorkforcesPaginateTypeDef",
     {
         "SortBy": ListWorkforcesSortByOptionsType,
         "SortOrder": SortOrderType,
@@ -8377,15 +7899,14 @@
 )
 
 ModelDashboardIndicatorActionTypeDef = TypedDict(
     "ModelDashboardIndicatorActionTypeDef",
     {
         "Enabled": bool,
     },
-    total=False,
 )
 
 S3ModelDataSourceTypeDef = TypedDict(
     "S3ModelDataSourceTypeDef",
     {
         "S3Uri": str,
         "S3DataType": S3ModelDataTypeType,
@@ -8421,40 +7942,28 @@
     "ModelMetadataFilterTypeDef",
     {
         "Name": ModelMetadataFilterTypeType,
         "Value": str,
     },
 )
 
-_RequiredModelPackageStatusItemTypeDef = TypedDict(
-    "_RequiredModelPackageStatusItemTypeDef",
+ModelPackageStatusItemTypeDef = TypedDict(
+    "ModelPackageStatusItemTypeDef",
     {
         "Name": str,
         "Status": DetailedModelPackageStatusType,
-    },
-)
-_OptionalModelPackageStatusItemTypeDef = TypedDict(
-    "_OptionalModelPackageStatusItemTypeDef",
-    {
         "FailureReason": str,
     },
-    total=False,
 )
 
-class ModelPackageStatusItemTypeDef(
-    _RequiredModelPackageStatusItemTypeDef, _OptionalModelPackageStatusItemTypeDef
-):
-    pass
-
 ModelStepMetadataTypeDef = TypedDict(
     "ModelStepMetadataTypeDef",
     {
         "Arn": str,
     },
-    total=False,
 )
 
 _RequiredMonitoringAppSpecificationTypeDef = TypedDict(
     "_RequiredMonitoringAppSpecificationTypeDef",
     {
         "ImageUri": str,
     },
@@ -8564,15 +8073,14 @@
         "Issuer": str,
         "AuthorizationEndpoint": str,
         "TokenEndpoint": str,
         "UserInfoEndpoint": str,
         "LogoutEndpoint": str,
         "JwksUri": str,
     },
-    total=False,
 )
 
 OnlineStoreSecurityConfigTypeDef = TypedDict(
     "OnlineStoreSecurityConfigTypeDef",
     {
         "KmsKeyId": str,
     },
@@ -8618,37 +8126,25 @@
 
 ParentTypeDef = TypedDict(
     "ParentTypeDef",
     {
         "TrialName": str,
         "ExperimentName": str,
     },
-    total=False,
 )
 
-_RequiredProductionVariantStatusTypeDef = TypedDict(
-    "_RequiredProductionVariantStatusTypeDef",
+ProductionVariantStatusTypeDef = TypedDict(
+    "ProductionVariantStatusTypeDef",
     {
         "Status": VariantStatusType,
-    },
-)
-_OptionalProductionVariantStatusTypeDef = TypedDict(
-    "_OptionalProductionVariantStatusTypeDef",
-    {
         "StatusMessage": str,
         "StartTime": datetime,
     },
-    total=False,
 )
 
-class ProductionVariantStatusTypeDef(
-    _RequiredProductionVariantStatusTypeDef, _OptionalProductionVariantStatusTypeDef
-):
-    pass
-
 PhaseTypeDef = TypedDict(
     "PhaseTypeDef",
     {
         "InitialNumberOfUsers": int,
         "SpawnRate": int,
         "DurationInSeconds": int,
     },
@@ -8656,15 +8152,14 @@
 )
 
 ProcessingJobStepMetadataTypeDef = TypedDict(
     "ProcessingJobStepMetadataTypeDef",
     {
         "Arn": str,
     },
-    total=False,
 )
 
 QualityCheckStepMetadataTypeDef = TypedDict(
     "QualityCheckStepMetadataTypeDef",
     {
         "CheckType": str,
         "BaselineUsedForDriftCheckStatistics": str,
@@ -8673,55 +8168,49 @@
         "CalculatedBaselineConstraints": str,
         "ModelPackageGroupName": str,
         "ViolationReport": str,
         "CheckJobArn": str,
         "SkipCheck": bool,
         "RegisterNewBaseline": bool,
     },
-    total=False,
 )
 
 RegisterModelStepMetadataTypeDef = TypedDict(
     "RegisterModelStepMetadataTypeDef",
     {
         "Arn": str,
     },
-    total=False,
 )
 
 TrainingJobStepMetadataTypeDef = TypedDict(
     "TrainingJobStepMetadataTypeDef",
     {
         "Arn": str,
     },
-    total=False,
 )
 
 TransformJobStepMetadataTypeDef = TypedDict(
     "TransformJobStepMetadataTypeDef",
     {
         "Arn": str,
     },
-    total=False,
 )
 
 TuningJobStepMetaDataTypeDef = TypedDict(
     "TuningJobStepMetaDataTypeDef",
     {
         "Arn": str,
     },
-    total=False,
 )
 
 SelectiveExecutionResultTypeDef = TypedDict(
     "SelectiveExecutionResultTypeDef",
     {
         "SourcePipelineExecutionArn": str,
     },
-    total=False,
 )
 
 _RequiredProcessingClusterConfigTypeDef = TypedDict(
     "_RequiredProcessingClusterConfigTypeDef",
     {
         "InstanceCount": int,
         "InstanceType": ProcessingInstanceTypeType,
@@ -8869,15 +8358,14 @@
 VertexTypeDef = TypedDict(
     "VertexTypeDef",
     {
         "Arn": str,
         "Type": str,
         "LineageType": LineageTypeType,
     },
-    total=False,
 )
 
 RStudioServerProAppSettingsTypeDef = TypedDict(
     "RStudioServerProAppSettingsTypeDef",
     {
         "AccessStatus": RStudioServerProAccessStatusType,
         "UserGroup": RStudioServerProUserGroupType,
@@ -9699,47 +9187,35 @@
     "UpdateUserProfileResponseTypeDef",
     {
         "UserProfileArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredWorkforceVpcConfigResponseTypeDef = TypedDict(
-    "_RequiredWorkforceVpcConfigResponseTypeDef",
+WorkforceVpcConfigResponseTypeDef = TypedDict(
+    "WorkforceVpcConfigResponseTypeDef",
     {
         "VpcId": str,
         "SecurityGroupIds": List[str],
         "Subnets": List[str],
-    },
-)
-_OptionalWorkforceVpcConfigResponseTypeDef = TypedDict(
-    "_OptionalWorkforceVpcConfigResponseTypeDef",
-    {
         "VpcEndpointId": str,
     },
-    total=False,
 )
 
-class WorkforceVpcConfigResponseTypeDef(
-    _RequiredWorkforceVpcConfigResponseTypeDef, _OptionalWorkforceVpcConfigResponseTypeDef
-):
-    pass
-
 ActionSummaryTypeDef = TypedDict(
     "ActionSummaryTypeDef",
     {
         "ActionArn": str,
         "ActionName": str,
         "Source": ActionSourceTypeDef,
         "ActionType": str,
         "Status": ActionStatusType,
         "CreationTime": datetime,
         "LastModifiedTime": datetime,
     },
-    total=False,
 )
 
 AddTagsInputRequestTypeDef = TypedDict(
     "AddTagsInputRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Sequence[TagTypeDef],
@@ -9909,15 +9385,14 @@
 
 AlgorithmStatusDetailsTypeDef = TypedDict(
     "AlgorithmStatusDetailsTypeDef",
     {
         "ValidationStatuses": List[AlgorithmStatusItemTypeDef],
         "ImageScanStatuses": List[AlgorithmStatusItemTypeDef],
     },
-    total=False,
 )
 
 ListAlgorithmsOutputTypeDef = TypedDict(
     "ListAlgorithmsOutputTypeDef",
     {
         "AlgorithmSummaryList": List[AlgorithmSummaryTypeDef],
         "NextToken": str,
@@ -10007,47 +9482,36 @@
 ResolvedAttributesTypeDef = TypedDict(
     "ResolvedAttributesTypeDef",
     {
         "AutoMLJobObjective": AutoMLJobObjectiveTypeDef,
         "ProblemType": ProblemTypeType,
         "CompletionCriteria": AutoMLJobCompletionCriteriaTypeDef,
     },
-    total=False,
 )
 
-_RequiredAutoMLJobSummaryTypeDef = TypedDict(
-    "_RequiredAutoMLJobSummaryTypeDef",
+AutoMLJobSummaryTypeDef = TypedDict(
+    "AutoMLJobSummaryTypeDef",
     {
         "AutoMLJobName": str,
         "AutoMLJobArn": str,
         "AutoMLJobStatus": AutoMLJobStatusType,
         "AutoMLJobSecondaryStatus": AutoMLJobSecondaryStatusType,
         "CreationTime": datetime,
-        "LastModifiedTime": datetime,
-    },
-)
-_OptionalAutoMLJobSummaryTypeDef = TypedDict(
-    "_OptionalAutoMLJobSummaryTypeDef",
-    {
         "EndTime": datetime,
+        "LastModifiedTime": datetime,
         "FailureReason": str,
         "PartialFailureReasons": List[AutoMLPartialFailureReasonTypeDef],
     },
-    total=False,
 )
 
-class AutoMLJobSummaryTypeDef(_RequiredAutoMLJobSummaryTypeDef, _OptionalAutoMLJobSummaryTypeDef):
-    pass
-
 AutoMLProblemTypeResolvedAttributesTypeDef = TypedDict(
     "AutoMLProblemTypeResolvedAttributesTypeDef",
     {
         "TabularResolvedAttributes": TabularResolvedAttributesTypeDef,
     },
-    total=False,
 )
 
 AutoMLSecurityConfigTypeDef = TypedDict(
     "AutoMLSecurityConfigTypeDef",
     {
         "VolumeKmsKeyId": str,
         "EnableInterContainerTrafficEncryption": bool,
@@ -10142,24 +9606,22 @@
 CallbackStepMetadataTypeDef = TypedDict(
     "CallbackStepMetadataTypeDef",
     {
         "CallbackToken": str,
         "SqsQueueUrl": str,
         "OutputParameters": List[OutputParameterTypeDef],
     },
-    total=False,
 )
 
 LambdaStepMetadataTypeDef = TypedDict(
     "LambdaStepMetadataTypeDef",
     {
         "Arn": str,
         "OutputParameters": List[OutputParameterTypeDef],
     },
-    total=False,
 )
 
 _RequiredSendPipelineExecutionStepSuccessRequestRequestTypeDef = TypedDict(
     "_RequiredSendPipelineExecutionStepSuccessRequestRequestTypeDef",
     {
         "CallbackToken": str,
     },
@@ -10181,22 +9643,22 @@
 
 CandidatePropertiesTypeDef = TypedDict(
     "CandidatePropertiesTypeDef",
     {
         "CandidateArtifactLocations": CandidateArtifactLocationsTypeDef,
         "CandidateMetrics": List[MetricDatumTypeDef],
     },
-    total=False,
 )
 
 CanvasAppSettingsTypeDef = TypedDict(
     "CanvasAppSettingsTypeDef",
     {
         "TimeSeriesForecastingSettings": TimeSeriesForecastingSettingsTypeDef,
         "ModelRegisterSettings": ModelRegisterSettingsTypeDef,
+        "WorkspaceSettings": WorkspaceSettingsTypeDef,
     },
     total=False,
 )
 
 _RequiredRollingUpdatePolicyTypeDef = TypedDict(
     "_RequiredRollingUpdatePolicyTypeDef",
     {
@@ -10309,36 +9771,25 @@
 )
 
 class ClarifyShapConfigTypeDef(
     _RequiredClarifyShapConfigTypeDef, _OptionalClarifyShapConfigTypeDef
 ):
     pass
 
-_RequiredCodeRepositorySummaryTypeDef = TypedDict(
-    "_RequiredCodeRepositorySummaryTypeDef",
+CodeRepositorySummaryTypeDef = TypedDict(
+    "CodeRepositorySummaryTypeDef",
     {
         "CodeRepositoryName": str,
         "CodeRepositoryArn": str,
         "CreationTime": datetime,
         "LastModifiedTime": datetime,
-    },
-)
-_OptionalCodeRepositorySummaryTypeDef = TypedDict(
-    "_OptionalCodeRepositorySummaryTypeDef",
-    {
         "GitConfig": GitConfigTypeDef,
     },
-    total=False,
 )
 
-class CodeRepositorySummaryTypeDef(
-    _RequiredCodeRepositorySummaryTypeDef, _OptionalCodeRepositorySummaryTypeDef
-):
-    pass
-
 _RequiredCreateCodeRepositoryInputRequestTypeDef = TypedDict(
     "_RequiredCreateCodeRepositoryInputRequestTypeDef",
     {
         "CodeRepositoryName": str,
         "GitConfig": GitConfigTypeDef,
     },
 )
@@ -10402,15 +9853,14 @@
         "ContextArn": str,
         "ContextName": str,
         "Source": ContextSourceTypeDef,
         "ContextType": str,
         "CreationTime": datetime,
         "LastModifiedTime": datetime,
     },
-    total=False,
 )
 
 _RequiredCreateContextRequestRequestTypeDef = TypedDict(
     "_RequiredCreateContextRequestRequestTypeDef",
     {
         "ContextName": str,
         "Source": ContextSourceTypeDef,
@@ -10735,41 +10185,30 @@
 )
 
 class CreateHumanTaskUiRequestRequestTypeDef(
     _RequiredCreateHumanTaskUiRequestRequestTypeDef, _OptionalCreateHumanTaskUiRequestRequestTypeDef
 ):
     pass
 
-_RequiredInferenceExperimentSummaryTypeDef = TypedDict(
-    "_RequiredInferenceExperimentSummaryTypeDef",
+InferenceExperimentSummaryTypeDef = TypedDict(
+    "InferenceExperimentSummaryTypeDef",
     {
         "Name": str,
         "Type": Literal["ShadowMode"],
-        "Status": InferenceExperimentStatusType,
-        "CreationTime": datetime,
-        "LastModifiedTime": datetime,
-    },
-)
-_OptionalInferenceExperimentSummaryTypeDef = TypedDict(
-    "_OptionalInferenceExperimentSummaryTypeDef",
-    {
         "Schedule": InferenceExperimentScheduleTypeDef,
+        "Status": InferenceExperimentStatusType,
         "StatusReason": str,
         "Description": str,
+        "CreationTime": datetime,
         "CompletionTime": datetime,
+        "LastModifiedTime": datetime,
         "RoleArn": str,
     },
-    total=False,
 )
 
-class InferenceExperimentSummaryTypeDef(
-    _RequiredInferenceExperimentSummaryTypeDef, _OptionalInferenceExperimentSummaryTypeDef
-):
-    pass
-
 _RequiredCreateModelCardExportJobRequestRequestTypeDef = TypedDict(
     "_RequiredCreateModelCardExportJobRequestRequestTypeDef",
     {
         "ModelCardName": str,
         "ModelCardExportJobName": str,
         "OutputConfig": ModelCardExportOutputConfigTypeDef,
     },
@@ -11256,33 +10695,22 @@
 )
 
 class DeleteDomainRequestRequestTypeDef(
     _RequiredDeleteDomainRequestRequestTypeDef, _OptionalDeleteDomainRequestRequestTypeDef
 ):
     pass
 
-_RequiredDeploymentRecommendationTypeDef = TypedDict(
-    "_RequiredDeploymentRecommendationTypeDef",
+DeploymentRecommendationTypeDef = TypedDict(
+    "DeploymentRecommendationTypeDef",
     {
         "RecommendationStatus": RecommendationStatusType,
-    },
-)
-_OptionalDeploymentRecommendationTypeDef = TypedDict(
-    "_OptionalDeploymentRecommendationTypeDef",
-    {
         "RealTimeInferenceRecommendations": List[RealTimeInferenceRecommendationTypeDef],
     },
-    total=False,
 )
 
-class DeploymentRecommendationTypeDef(
-    _RequiredDeploymentRecommendationTypeDef, _OptionalDeploymentRecommendationTypeDef
-):
-    pass
-
 _RequiredDeploymentStageTypeDef = TypedDict(
     "_RequiredDeploymentStageTypeDef",
     {
         "StageName": str,
         "DeviceSelectionConfig": DeviceSelectionConfigTypeDef,
     },
 )
@@ -11617,39 +11045,27 @@
         "ExperimentArn": str,
         "ExperimentName": str,
         "DisplayName": str,
         "ExperimentSource": ExperimentSourceTypeDef,
         "CreationTime": datetime,
         "LastModifiedTime": datetime,
     },
-    total=False,
 )
 
-_RequiredFeatureGroupSummaryTypeDef = TypedDict(
-    "_RequiredFeatureGroupSummaryTypeDef",
+FeatureGroupSummaryTypeDef = TypedDict(
+    "FeatureGroupSummaryTypeDef",
     {
         "FeatureGroupName": str,
         "FeatureGroupArn": str,
         "CreationTime": datetime,
-    },
-)
-_OptionalFeatureGroupSummaryTypeDef = TypedDict(
-    "_OptionalFeatureGroupSummaryTypeDef",
-    {
         "FeatureGroupStatus": FeatureGroupStatusType,
         "OfflineStoreStatus": OfflineStoreStatusTypeDef,
     },
-    total=False,
 )
 
-class FeatureGroupSummaryTypeDef(
-    _RequiredFeatureGroupSummaryTypeDef, _OptionalFeatureGroupSummaryTypeDef
-):
-    pass
-
 DescribeFeatureMetadataResponseTypeDef = TypedDict(
     "DescribeFeatureMetadataResponseTypeDef",
     {
         "FeatureGroupArn": str,
         "FeatureGroupName": str,
         "FeatureName": str,
         "FeatureType": FeatureTypeType,
@@ -11669,15 +11085,14 @@
         "FeatureName": str,
         "FeatureType": FeatureTypeType,
         "CreationTime": datetime,
         "LastModifiedTime": datetime,
         "Description": str,
         "Parameters": List[FeatureParameterTypeDef],
     },
-    total=False,
 )
 
 _RequiredUpdateFeatureMetadataRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateFeatureMetadataRequestRequestTypeDef",
     {
         "FeatureGroupName": str,
         "FeatureName": str,
@@ -11773,49 +11188,37 @@
     {
         "SubscribedWorkteams": List[SubscribedWorkteamTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredTrainingJobSummaryTypeDef = TypedDict(
-    "_RequiredTrainingJobSummaryTypeDef",
+TrainingJobSummaryTypeDef = TypedDict(
+    "TrainingJobSummaryTypeDef",
     {
         "TrainingJobName": str,
         "TrainingJobArn": str,
         "CreationTime": datetime,
-        "TrainingJobStatus": TrainingJobStatusType,
-    },
-)
-_OptionalTrainingJobSummaryTypeDef = TypedDict(
-    "_OptionalTrainingJobSummaryTypeDef",
-    {
         "TrainingEndTime": datetime,
         "LastModifiedTime": datetime,
+        "TrainingJobStatus": TrainingJobStatusType,
         "WarmPoolStatus": WarmPoolStatusTypeDef,
     },
-    total=False,
 )
 
-class TrainingJobSummaryTypeDef(
-    _RequiredTrainingJobSummaryTypeDef, _OptionalTrainingJobSummaryTypeDef
-):
-    pass
-
 TrialSummaryTypeDef = TypedDict(
     "TrialSummaryTypeDef",
     {
         "TrialArn": str,
         "TrialName": str,
         "DisplayName": str,
         "TrialSource": TrialSourceTypeDef,
         "CreationTime": datetime,
         "LastModifiedTime": datetime,
     },
-    total=False,
 )
 
 _RequiredDesiredWeightAndCapacityTypeDef = TypedDict(
     "_RequiredDesiredWeightAndCapacityTypeDef",
     {
         "VariantName": str,
     },
@@ -11849,38 +11252,29 @@
     {
         "DeviceFleetSummaries": List[DeviceFleetSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredDeviceSummaryTypeDef = TypedDict(
-    "_RequiredDeviceSummaryTypeDef",
+DeviceSummaryTypeDef = TypedDict(
+    "DeviceSummaryTypeDef",
     {
         "DeviceName": str,
         "DeviceArn": str,
-    },
-)
-_OptionalDeviceSummaryTypeDef = TypedDict(
-    "_OptionalDeviceSummaryTypeDef",
-    {
         "Description": str,
         "DeviceFleetName": str,
         "IotThingName": str,
         "RegistrationTime": datetime,
         "LatestHeartbeat": datetime,
         "Models": List[EdgeModelSummaryTypeDef],
         "AgentVersion": str,
     },
-    total=False,
 )
 
-class DeviceSummaryTypeDef(_RequiredDeviceSummaryTypeDef, _OptionalDeviceSummaryTypeDef):
-    pass
-
 _RequiredRegisterDevicesRequestRequestTypeDef = TypedDict(
     "_RequiredRegisterDevicesRequestRequestTypeDef",
     {
         "DeviceFleetName": str,
         "Devices": Sequence[DeviceTypeDef],
     },
 )
@@ -11971,36 +11365,25 @@
     {
         "EndpointConfigs": List[EndpointConfigSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredEndpointOutputConfigurationTypeDef = TypedDict(
-    "_RequiredEndpointOutputConfigurationTypeDef",
+EndpointOutputConfigurationTypeDef = TypedDict(
+    "EndpointOutputConfigurationTypeDef",
     {
         "EndpointName": str,
         "VariantName": str,
-    },
-)
-_OptionalEndpointOutputConfigurationTypeDef = TypedDict(
-    "_OptionalEndpointOutputConfigurationTypeDef",
-    {
         "InstanceType": ProductionVariantInstanceTypeType,
         "InitialInstanceCount": int,
         "ServerlessConfig": ProductionVariantServerlessConfigTypeDef,
     },
-    total=False,
 )
 
-class EndpointOutputConfigurationTypeDef(
-    _RequiredEndpointOutputConfigurationTypeDef, _OptionalEndpointOutputConfigurationTypeDef
-):
-    pass
-
 EndpointPerformanceTypeDef = TypedDict(
     "EndpointPerformanceTypeDef",
     {
         "Metrics": InferenceMetricsTypeDef,
         "EndpointInfo": EndpointInfoTypeDef,
     },
 )
@@ -12017,57 +11400,44 @@
 ModelConfigurationTypeDef = TypedDict(
     "ModelConfigurationTypeDef",
     {
         "InferenceSpecificationName": str,
         "EnvironmentParameters": List[EnvironmentParameterTypeDef],
         "CompilationJobName": str,
     },
-    total=False,
 )
 
 NestedFiltersTypeDef = TypedDict(
     "NestedFiltersTypeDef",
     {
         "NestedPropertyName": str,
         "Filters": Sequence[FilterTypeDef],
     },
 )
 
-_RequiredHyperParameterTrainingJobSummaryTypeDef = TypedDict(
-    "_RequiredHyperParameterTrainingJobSummaryTypeDef",
+HyperParameterTrainingJobSummaryTypeDef = TypedDict(
+    "HyperParameterTrainingJobSummaryTypeDef",
     {
+        "TrainingJobDefinitionName": str,
         "TrainingJobName": str,
         "TrainingJobArn": str,
-        "CreationTime": datetime,
-        "TrainingJobStatus": TrainingJobStatusType,
-        "TunedHyperParameters": Dict[str, str],
-    },
-)
-_OptionalHyperParameterTrainingJobSummaryTypeDef = TypedDict(
-    "_OptionalHyperParameterTrainingJobSummaryTypeDef",
-    {
-        "TrainingJobDefinitionName": str,
         "TuningJobName": str,
+        "CreationTime": datetime,
         "TrainingStartTime": datetime,
         "TrainingEndTime": datetime,
+        "TrainingJobStatus": TrainingJobStatusType,
+        "TunedHyperParameters": Dict[str, str],
         "FailureReason": str,
         "FinalHyperParameterTuningJobObjectiveMetric": (
             FinalHyperParameterTuningJobObjectiveMetricTypeDef
         ),
         "ObjectiveStatus": ObjectiveStatusType,
     },
-    total=False,
 )
 
-class HyperParameterTrainingJobSummaryTypeDef(
-    _RequiredHyperParameterTrainingJobSummaryTypeDef,
-    _OptionalHyperParameterTrainingJobSummaryTypeDef,
-):
-    pass
-
 ListFlowDefinitionsResponseTypeDef = TypedDict(
     "ListFlowDefinitionsResponseTypeDef",
     {
         "FlowDefinitionSummaries": List[FlowDefinitionSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -12153,41 +11523,30 @@
         "VolumeKmsKeyId": str,
         "AllocationStrategy": Literal["Prioritized"],
         "InstanceConfigs": Sequence[HyperParameterTuningInstanceConfigTypeDef],
     },
     total=False,
 )
 
-_RequiredHyperParameterTuningJobSummaryTypeDef = TypedDict(
-    "_RequiredHyperParameterTuningJobSummaryTypeDef",
+HyperParameterTuningJobSummaryTypeDef = TypedDict(
+    "HyperParameterTuningJobSummaryTypeDef",
     {
         "HyperParameterTuningJobName": str,
         "HyperParameterTuningJobArn": str,
         "HyperParameterTuningJobStatus": HyperParameterTuningJobStatusType,
         "Strategy": HyperParameterTuningJobStrategyTypeType,
         "CreationTime": datetime,
-        "TrainingJobStatusCounters": TrainingJobStatusCountersTypeDef,
-        "ObjectiveStatusCounters": ObjectiveStatusCountersTypeDef,
-    },
-)
-_OptionalHyperParameterTuningJobSummaryTypeDef = TypedDict(
-    "_OptionalHyperParameterTuningJobSummaryTypeDef",
-    {
         "HyperParameterTuningEndTime": datetime,
         "LastModifiedTime": datetime,
+        "TrainingJobStatusCounters": TrainingJobStatusCountersTypeDef,
+        "ObjectiveStatusCounters": ObjectiveStatusCountersTypeDef,
         "ResourceLimits": ResourceLimitsTypeDef,
     },
-    total=False,
 )
 
-class HyperParameterTuningJobSummaryTypeDef(
-    _RequiredHyperParameterTuningJobSummaryTypeDef, _OptionalHyperParameterTuningJobSummaryTypeDef
-):
-    pass
-
 HyperParameterTuningJobStrategyConfigTypeDef = TypedDict(
     "HyperParameterTuningJobStrategyConfigTypeDef",
     {
         "HyperbandStrategyConfig": HyperbandStrategyConfigTypeDef,
     },
     total=False,
 )
@@ -12204,15 +11563,14 @@
     "UserContextTypeDef",
     {
         "UserProfileArn": str,
         "UserProfileName": str,
         "DomainId": str,
         "IamIdentity": IamIdentityTypeDef,
     },
-    total=False,
 )
 
 _RequiredImageConfigTypeDef = TypedDict(
     "_RequiredImageConfigTypeDef",
     {
         "RepositoryAccessMode": RepositoryAccessModeType,
     },
@@ -12312,37 +11670,26 @@
 )
 
 class KernelGatewayImageConfigTypeDef(
     _RequiredKernelGatewayImageConfigTypeDef, _OptionalKernelGatewayImageConfigTypeDef
 ):
     pass
 
-_RequiredLabelingJobForWorkteamSummaryTypeDef = TypedDict(
-    "_RequiredLabelingJobForWorkteamSummaryTypeDef",
+LabelingJobForWorkteamSummaryTypeDef = TypedDict(
+    "LabelingJobForWorkteamSummaryTypeDef",
     {
+        "LabelingJobName": str,
         "JobReferenceCode": str,
         "WorkRequesterAccountId": str,
         "CreationTime": datetime,
-    },
-)
-_OptionalLabelingJobForWorkteamSummaryTypeDef = TypedDict(
-    "_OptionalLabelingJobForWorkteamSummaryTypeDef",
-    {
-        "LabelingJobName": str,
         "LabelCounters": LabelCountersForWorkteamTypeDef,
         "NumberOfHumanWorkersPerDataObject": int,
     },
-    total=False,
 )
 
-class LabelingJobForWorkteamSummaryTypeDef(
-    _RequiredLabelingJobForWorkteamSummaryTypeDef, _OptionalLabelingJobForWorkteamSummaryTypeDef
-):
-    pass
-
 LabelingJobDataSourceTypeDef = TypedDict(
     "LabelingJobDataSourceTypeDef",
     {
         "S3DataSource": LabelingJobS3DataSourceTypeDef,
         "SnsDataSource": LabelingJobSnsDataSourceTypeDef,
     },
     total=False,
@@ -12583,15 +11930,14 @@
 )
 
 MonitoringAlertActionsTypeDef = TypedDict(
     "MonitoringAlertActionsTypeDef",
     {
         "ModelDashboardIndicator": ModelDashboardIndicatorActionTypeDef,
     },
-    total=False,
 )
 
 ModelDataSourceTypeDef = TypedDict(
     "ModelDataSourceTypeDef",
     {
         "S3DataSource": S3ModelDataSourceTypeDef,
     },
@@ -12601,41 +11947,30 @@
     "ModelInfrastructureConfigTypeDef",
     {
         "InfrastructureType": Literal["RealTimeInference"],
         "RealTimeInferenceConfig": RealTimeInferenceConfigTypeDef,
     },
 )
 
-_RequiredModelPackageContainerDefinitionTypeDef = TypedDict(
-    "_RequiredModelPackageContainerDefinitionTypeDef",
-    {
-        "Image": str,
-    },
-)
-_OptionalModelPackageContainerDefinitionTypeDef = TypedDict(
-    "_OptionalModelPackageContainerDefinitionTypeDef",
+ModelPackageContainerDefinitionTypeDef = TypedDict(
+    "ModelPackageContainerDefinitionTypeDef",
     {
         "ContainerHostname": str,
+        "Image": str,
         "ImageDigest": str,
         "ModelDataUrl": str,
         "ProductId": str,
         "Environment": Dict[str, str],
         "ModelInput": ModelInputTypeDef,
         "Framework": str,
         "FrameworkVersion": str,
         "NearestModelName": str,
     },
-    total=False,
 )
 
-class ModelPackageContainerDefinitionTypeDef(
-    _RequiredModelPackageContainerDefinitionTypeDef, _OptionalModelPackageContainerDefinitionTypeDef
-):
-    pass
-
 RecommendationJobStoppingConditionsTypeDef = TypedDict(
     "RecommendationJobStoppingConditionsTypeDef",
     {
         "MaxInvocations": int,
         "ModelLatencyThresholds": Sequence[ModelLatencyThresholdTypeDef],
     },
     total=False,
@@ -12645,33 +11980,22 @@
     "ModelMetadataSearchExpressionTypeDef",
     {
         "Filters": Sequence[ModelMetadataFilterTypeDef],
     },
     total=False,
 )
 
-_RequiredModelPackageStatusDetailsTypeDef = TypedDict(
-    "_RequiredModelPackageStatusDetailsTypeDef",
+ModelPackageStatusDetailsTypeDef = TypedDict(
+    "ModelPackageStatusDetailsTypeDef",
     {
         "ValidationStatuses": List[ModelPackageStatusItemTypeDef],
-    },
-)
-_OptionalModelPackageStatusDetailsTypeDef = TypedDict(
-    "_OptionalModelPackageStatusDetailsTypeDef",
-    {
         "ImageScanStatuses": List[ModelPackageStatusItemTypeDef],
     },
-    total=False,
 )
 
-class ModelPackageStatusDetailsTypeDef(
-    _RequiredModelPackageStatusDetailsTypeDef, _OptionalModelPackageStatusDetailsTypeDef
-):
-    pass
-
 MonitoringResourcesTypeDef = TypedDict(
     "MonitoringResourcesTypeDef",
     {
         "ClusterConfig": MonitoringClusterConfigTypeDef,
     },
 )
 
@@ -12747,68 +12071,46 @@
     },
     total=False,
 )
 
 class OutputConfigTypeDef(_RequiredOutputConfigTypeDef, _OptionalOutputConfigTypeDef):
     pass
 
-_RequiredPendingProductionVariantSummaryTypeDef = TypedDict(
-    "_RequiredPendingProductionVariantSummaryTypeDef",
+PendingProductionVariantSummaryTypeDef = TypedDict(
+    "PendingProductionVariantSummaryTypeDef",
     {
         "VariantName": str,
-    },
-)
-_OptionalPendingProductionVariantSummaryTypeDef = TypedDict(
-    "_OptionalPendingProductionVariantSummaryTypeDef",
-    {
         "DeployedImages": List[DeployedImageTypeDef],
         "CurrentWeight": float,
         "DesiredWeight": float,
         "CurrentInstanceCount": int,
         "DesiredInstanceCount": int,
         "InstanceType": ProductionVariantInstanceTypeType,
         "AcceleratorType": ProductionVariantAcceleratorTypeType,
         "VariantStatus": List[ProductionVariantStatusTypeDef],
         "CurrentServerlessConfig": ProductionVariantServerlessConfigTypeDef,
         "DesiredServerlessConfig": ProductionVariantServerlessConfigTypeDef,
     },
-    total=False,
 )
 
-class PendingProductionVariantSummaryTypeDef(
-    _RequiredPendingProductionVariantSummaryTypeDef, _OptionalPendingProductionVariantSummaryTypeDef
-):
-    pass
-
-_RequiredProductionVariantSummaryTypeDef = TypedDict(
-    "_RequiredProductionVariantSummaryTypeDef",
+ProductionVariantSummaryTypeDef = TypedDict(
+    "ProductionVariantSummaryTypeDef",
     {
         "VariantName": str,
-    },
-)
-_OptionalProductionVariantSummaryTypeDef = TypedDict(
-    "_OptionalProductionVariantSummaryTypeDef",
-    {
         "DeployedImages": List[DeployedImageTypeDef],
         "CurrentWeight": float,
         "DesiredWeight": float,
         "CurrentInstanceCount": int,
         "DesiredInstanceCount": int,
         "VariantStatus": List[ProductionVariantStatusTypeDef],
         "CurrentServerlessConfig": ProductionVariantServerlessConfigTypeDef,
         "DesiredServerlessConfig": ProductionVariantServerlessConfigTypeDef,
     },
-    total=False,
 )
 
-class ProductionVariantSummaryTypeDef(
-    _RequiredProductionVariantSummaryTypeDef, _OptionalProductionVariantSummaryTypeDef
-):
-    pass
-
 TrafficPatternTypeDef = TypedDict(
     "TrafficPatternTypeDef",
     {
         "TrafficType": Literal["PHASES"],
         "Phases": Sequence[PhaseTypeDef],
     },
     total=False,
@@ -13085,40 +12387,31 @@
 TransformDataSourceTypeDef = TypedDict(
     "TransformDataSourceTypeDef",
     {
         "S3DataSource": TransformS3DataSourceTypeDef,
     },
 )
 
-_RequiredWorkforceTypeDef = TypedDict(
-    "_RequiredWorkforceTypeDef",
+WorkforceTypeDef = TypedDict(
+    "WorkforceTypeDef",
     {
         "WorkforceName": str,
         "WorkforceArn": str,
-    },
-)
-_OptionalWorkforceTypeDef = TypedDict(
-    "_OptionalWorkforceTypeDef",
-    {
         "LastUpdatedDate": datetime,
         "SourceIpConfig": SourceIpConfigTypeDef,
         "SubDomain": str,
         "CognitoConfig": CognitoConfigTypeDef,
         "OidcConfig": OidcConfigForResponseTypeDef,
         "CreateDate": datetime,
         "WorkforceVpcConfig": WorkforceVpcConfigResponseTypeDef,
         "Status": WorkforceStatusType,
         "FailureReason": str,
     },
-    total=False,
 )
 
-class WorkforceTypeDef(_RequiredWorkforceTypeDef, _OptionalWorkforceTypeDef):
-    pass
-
 ListActionsResponseTypeDef = TypedDict(
     "ListActionsResponseTypeDef",
     {
         "ActionSummaries": List[ActionSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -13130,15 +12423,14 @@
         "ArtifactArn": str,
         "ArtifactName": str,
         "Source": ArtifactSourceTypeDef,
         "ArtifactType": str,
         "CreationTime": datetime,
         "LastModifiedTime": datetime,
     },
-    total=False,
 )
 
 _RequiredCreateArtifactRequestRequestTypeDef = TypedDict(
     "_RequiredCreateArtifactRequestRequestTypeDef",
     {
         "Source": ArtifactSourceTypeDef,
         "ArtifactType": str,
@@ -13255,15 +12547,14 @@
 AutoMLResolvedAttributesTypeDef = TypedDict(
     "AutoMLResolvedAttributesTypeDef",
     {
         "AutoMLJobObjective": AutoMLJobObjectiveTypeDef,
         "CompletionCriteria": AutoMLJobCompletionCriteriaTypeDef,
         "AutoMLProblemTypeResolvedAttributes": AutoMLProblemTypeResolvedAttributesTypeDef,
     },
-    total=False,
 )
 
 AutoMLJobConfigTypeDef = TypedDict(
     "AutoMLJobConfigTypeDef",
     {
         "CompletionCriteria": AutoMLJobCompletionCriteriaTypeDef,
         "SecurityConfig": AutoMLSecurityConfigTypeDef,
@@ -13319,46 +12610,36 @@
         "Lambda": LambdaStepMetadataTypeDef,
         "QualityCheck": QualityCheckStepMetadataTypeDef,
         "ClarifyCheck": ClarifyCheckStepMetadataTypeDef,
         "EMR": EMRStepMetadataTypeDef,
         "Fail": FailStepMetadataTypeDef,
         "AutoMLJob": AutoMLJobStepMetadataTypeDef,
     },
-    total=False,
 )
 
-_RequiredAutoMLCandidateTypeDef = TypedDict(
-    "_RequiredAutoMLCandidateTypeDef",
+AutoMLCandidateTypeDef = TypedDict(
+    "AutoMLCandidateTypeDef",
     {
         "CandidateName": str,
+        "FinalAutoMLJobObjectiveMetric": FinalAutoMLJobObjectiveMetricTypeDef,
         "ObjectiveStatus": ObjectiveStatusType,
         "CandidateSteps": List[AutoMLCandidateStepTypeDef],
         "CandidateStatus": CandidateStatusType,
-        "CreationTime": datetime,
-        "LastModifiedTime": datetime,
-    },
-)
-_OptionalAutoMLCandidateTypeDef = TypedDict(
-    "_OptionalAutoMLCandidateTypeDef",
-    {
-        "FinalAutoMLJobObjectiveMetric": FinalAutoMLJobObjectiveMetricTypeDef,
         "InferenceContainers": List[AutoMLContainerDefinitionTypeDef],
+        "CreationTime": datetime,
         "EndTime": datetime,
+        "LastModifiedTime": datetime,
         "FailureReason": str,
         "CandidateProperties": CandidatePropertiesTypeDef,
         "InferenceContainerDefinitions": Dict[
             AutoMLProcessingUnitType, List[AutoMLContainerDefinitionTypeDef]
         ],
     },
-    total=False,
 )
 
-class AutoMLCandidateTypeDef(_RequiredAutoMLCandidateTypeDef, _OptionalAutoMLCandidateTypeDef):
-    pass
-
 _RequiredBlueGreenUpdatePolicyTypeDef = TypedDict(
     "_RequiredBlueGreenUpdatePolicyTypeDef",
     {
         "TrafficRoutingConfiguration": TrafficRoutingConfigTypeDef,
     },
 )
 _OptionalBlueGreenUpdatePolicyTypeDef = TypedDict(
@@ -13639,62 +12920,39 @@
         "Explainability": DriftCheckExplainabilityTypeDef,
         "ModelQuality": DriftCheckModelQualityTypeDef,
         "ModelDataQuality": DriftCheckModelDataQualityTypeDef,
     },
     total=False,
 )
 
-_RequiredInferenceRecommendationTypeDef = TypedDict(
-    "_RequiredInferenceRecommendationTypeDef",
+InferenceRecommendationTypeDef = TypedDict(
+    "InferenceRecommendationTypeDef",
     {
         "Metrics": RecommendationMetricsTypeDef,
         "EndpointConfiguration": EndpointOutputConfigurationTypeDef,
         "ModelConfiguration": ModelConfigurationTypeDef,
-    },
-)
-_OptionalInferenceRecommendationTypeDef = TypedDict(
-    "_OptionalInferenceRecommendationTypeDef",
-    {
         "RecommendationId": str,
         "InvocationEndTime": datetime,
         "InvocationStartTime": datetime,
     },
-    total=False,
 )
 
-class InferenceRecommendationTypeDef(
-    _RequiredInferenceRecommendationTypeDef, _OptionalInferenceRecommendationTypeDef
-):
-    pass
-
-_RequiredRecommendationJobInferenceBenchmarkTypeDef = TypedDict(
-    "_RequiredRecommendationJobInferenceBenchmarkTypeDef",
-    {
-        "ModelConfiguration": ModelConfigurationTypeDef,
-    },
-)
-_OptionalRecommendationJobInferenceBenchmarkTypeDef = TypedDict(
-    "_OptionalRecommendationJobInferenceBenchmarkTypeDef",
+RecommendationJobInferenceBenchmarkTypeDef = TypedDict(
+    "RecommendationJobInferenceBenchmarkTypeDef",
     {
         "Metrics": RecommendationMetricsTypeDef,
         "EndpointConfiguration": EndpointOutputConfigurationTypeDef,
+        "ModelConfiguration": ModelConfigurationTypeDef,
         "FailureReason": str,
         "EndpointMetrics": InferenceMetricsTypeDef,
         "InvocationEndTime": datetime,
         "InvocationStartTime": datetime,
     },
-    total=False,
 )
 
-class RecommendationJobInferenceBenchmarkTypeDef(
-    _RequiredRecommendationJobInferenceBenchmarkTypeDef,
-    _OptionalRecommendationJobInferenceBenchmarkTypeDef,
-):
-    pass
-
 SearchExpressionTypeDef = TypedDict(
     "SearchExpressionTypeDef",
     {
         "Filters": Sequence[FilterTypeDef],
         "NestedFilters": Sequence[NestedFiltersTypeDef],
         "SubExpressions": Sequence[Dict[str, Any]],
         "Operator": BooleanOperatorType,
@@ -13729,15 +12987,14 @@
         "DestinationType": str,
         "AssociationType": AssociationEdgeTypeType,
         "SourceName": str,
         "DestinationName": str,
         "CreationTime": datetime,
         "CreatedBy": UserContextTypeDef,
     },
-    total=False,
 )
 
 DescribeActionResponseTypeDef = TypedDict(
     "DescribeActionResponseTypeDef",
     {
         "ActionName": str,
         "ActionArn": str,
@@ -13926,15 +13183,14 @@
         "Description": str,
         "CreationTime": datetime,
         "CreatedBy": UserContextTypeDef,
         "LastModifiedTime": datetime,
         "LastModifiedBy": UserContextTypeDef,
         "Tags": List[TagTypeDef],
     },
-    total=False,
 )
 
 ModelCardTypeDef = TypedDict(
     "ModelCardTypeDef",
     {
         "ModelCardArn": str,
         "ModelCardName": str,
@@ -13947,15 +13203,14 @@
         "LastModifiedTime": datetime,
         "LastModifiedBy": UserContextTypeDef,
         "Tags": List[TagTypeDef],
         "ModelId": str,
         "RiskRating": str,
         "ModelPackageGroupName": str,
     },
-    total=False,
 )
 
 ModelDashboardModelCardTypeDef = TypedDict(
     "ModelDashboardModelCardTypeDef",
     {
         "ModelCardArn": str,
         "ModelCardName": str,
@@ -13966,29 +13221,27 @@
         "CreatedBy": UserContextTypeDef,
         "LastModifiedTime": datetime,
         "LastModifiedBy": UserContextTypeDef,
         "Tags": List[TagTypeDef],
         "ModelId": str,
         "RiskRating": str,
     },
-    total=False,
 )
 
 ModelPackageGroupTypeDef = TypedDict(
     "ModelPackageGroupTypeDef",
     {
         "ModelPackageGroupName": str,
         "ModelPackageGroupArn": str,
         "ModelPackageGroupDescription": str,
         "CreationTime": datetime,
         "CreatedBy": UserContextTypeDef,
         "ModelPackageGroupStatus": ModelPackageGroupStatusType,
         "Tags": List[TagTypeDef],
     },
-    total=False,
 )
 
 PipelineTypeDef = TypedDict(
     "PipelineTypeDef",
     {
         "PipelineArn": str,
         "PipelineName": str,
@@ -14000,27 +13253,25 @@
         "LastModifiedTime": datetime,
         "LastRunTime": datetime,
         "CreatedBy": UserContextTypeDef,
         "LastModifiedBy": UserContextTypeDef,
         "ParallelismConfiguration": ParallelismConfigurationTypeDef,
         "Tags": List[TagTypeDef],
     },
-    total=False,
 )
 
 TrialComponentSimpleSummaryTypeDef = TypedDict(
     "TrialComponentSimpleSummaryTypeDef",
     {
         "TrialComponentName": str,
         "TrialComponentArn": str,
         "TrialComponentSource": TrialComponentSourceTypeDef,
         "CreationTime": datetime,
         "CreatedBy": UserContextTypeDef,
     },
-    total=False,
 )
 
 TrialComponentSummaryTypeDef = TypedDict(
     "TrialComponentSummaryTypeDef",
     {
         "TrialComponentName": str,
         "TrialComponentArn": str,
@@ -14030,15 +13281,14 @@
         "StartTime": datetime,
         "EndTime": datetime,
         "CreationTime": datetime,
         "CreatedBy": UserContextTypeDef,
         "LastModifiedTime": datetime,
         "LastModifiedBy": UserContextTypeDef,
     },
-    total=False,
 )
 
 _RequiredHyperParameterSpecificationTypeDef = TypedDict(
     "_RequiredHyperParameterSpecificationTypeDef",
     {
         "Name": str,
         "Type": ParameterTypeType,
@@ -14091,15 +13341,14 @@
     {
         "AppImageConfigArn": str,
         "AppImageConfigName": str,
         "CreationTime": datetime,
         "LastModifiedTime": datetime,
         "KernelGatewayImageConfig": KernelGatewayImageConfigTypeDef,
     },
-    total=False,
 )
 
 _RequiredCreateAppImageConfigRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAppImageConfigRequestRequestTypeDef",
     {
         "AppImageConfigName": str,
     },
@@ -14219,39 +13468,30 @@
 )
 
 class UpdateWorkteamRequestRequestTypeDef(
     _RequiredUpdateWorkteamRequestRequestTypeDef, _OptionalUpdateWorkteamRequestRequestTypeDef
 ):
     pass
 
-_RequiredWorkteamTypeDef = TypedDict(
-    "_RequiredWorkteamTypeDef",
+WorkteamTypeDef = TypedDict(
+    "WorkteamTypeDef",
     {
         "WorkteamName": str,
         "MemberDefinitions": List[MemberDefinitionTypeDef],
         "WorkteamArn": str,
-        "Description": str,
-    },
-)
-_OptionalWorkteamTypeDef = TypedDict(
-    "_OptionalWorkteamTypeDef",
-    {
         "WorkforceArn": str,
         "ProductListingIds": List[str],
+        "Description": str,
         "SubDomain": str,
         "CreateDate": datetime,
         "LastUpdatedDate": datetime,
         "NotificationConfiguration": NotificationConfigurationTypeDef,
     },
-    total=False,
 )
 
-class WorkteamTypeDef(_RequiredWorkteamTypeDef, _OptionalWorkteamTypeDef):
-    pass
-
 MonitoringAlertSummaryTypeDef = TypedDict(
     "MonitoringAlertSummaryTypeDef",
     {
         "MonitoringAlertName": str,
         "CreationTime": datetime,
         "LastModifiedTime": datetime,
         "AlertStatus": MonitoringAlertStatusType,
@@ -14318,36 +13558,25 @@
 
 class AdditionalInferenceSpecificationDefinitionTypeDef(
     _RequiredAdditionalInferenceSpecificationDefinitionTypeDef,
     _OptionalAdditionalInferenceSpecificationDefinitionTypeDef,
 ):
     pass
 
-_RequiredInferenceSpecificationTypeDef = TypedDict(
-    "_RequiredInferenceSpecificationTypeDef",
+InferenceSpecificationTypeDef = TypedDict(
+    "InferenceSpecificationTypeDef",
     {
         "Containers": List[ModelPackageContainerDefinitionTypeDef],
-        "SupportedContentTypes": List[str],
-        "SupportedResponseMIMETypes": List[str],
-    },
-)
-_OptionalInferenceSpecificationTypeDef = TypedDict(
-    "_OptionalInferenceSpecificationTypeDef",
-    {
         "SupportedTransformInstanceTypes": List[TransformInstanceTypeType],
         "SupportedRealtimeInferenceInstanceTypes": List[ProductionVariantInstanceTypeType],
+        "SupportedContentTypes": List[str],
+        "SupportedResponseMIMETypes": List[str],
     },
-    total=False,
 )
 
-class InferenceSpecificationTypeDef(
-    _RequiredInferenceSpecificationTypeDef, _OptionalInferenceSpecificationTypeDef
-):
-    pass
-
 ListModelMetadataRequestListModelMetadataPaginateTypeDef = TypedDict(
     "ListModelMetadataRequestListModelMetadataPaginateTypeDef",
     {
         "SearchExpression": ModelMetadataSearchExpressionTypeDef,
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
@@ -14477,15 +13706,14 @@
         "FeatureGroupStatus": FeatureGroupStatusType,
         "OfflineStoreStatus": OfflineStoreStatusTypeDef,
         "LastUpdateStatus": LastUpdateStatusTypeDef,
         "FailureReason": str,
         "Description": str,
         "Tags": List[TagTypeDef],
     },
-    total=False,
 )
 
 _RequiredUpdateFeatureGroupRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateFeatureGroupRequestRequestTypeDef",
     {
         "FeatureGroupName": str,
     },
@@ -14551,35 +13779,24 @@
         "InputConfig": InputConfigTypeDef,
         "OutputConfig": OutputConfigTypeDef,
         "VpcConfig": NeoVpcConfigTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredPendingDeploymentSummaryTypeDef = TypedDict(
-    "_RequiredPendingDeploymentSummaryTypeDef",
+PendingDeploymentSummaryTypeDef = TypedDict(
+    "PendingDeploymentSummaryTypeDef",
     {
         "EndpointConfigName": str,
-    },
-)
-_OptionalPendingDeploymentSummaryTypeDef = TypedDict(
-    "_OptionalPendingDeploymentSummaryTypeDef",
-    {
         "ProductionVariants": List[PendingProductionVariantSummaryTypeDef],
         "StartTime": datetime,
         "ShadowProductionVariants": List[PendingProductionVariantSummaryTypeDef],
     },
-    total=False,
 )
 
-class PendingDeploymentSummaryTypeDef(
-    _RequiredPendingDeploymentSummaryTypeDef, _OptionalPendingDeploymentSummaryTypeDef
-):
-    pass
-
 _RequiredProcessingOutputConfigTypeDef = TypedDict(
     "_RequiredProcessingOutputConfigTypeDef",
     {
         "Outputs": Sequence[ProcessingOutputTypeDef],
     },
 )
 _OptionalProcessingOutputConfigTypeDef = TypedDict(
@@ -14666,15 +13883,14 @@
         "ProjectStatus": ProjectStatusType,
         "CreatedBy": UserContextTypeDef,
         "CreationTime": datetime,
         "Tags": List[TagTypeDef],
         "LastModifiedTime": datetime,
         "LastModifiedBy": UserContextTypeDef,
     },
-    total=False,
 )
 
 _RequiredUpdateProjectInputRequestTypeDef = TypedDict(
     "_RequiredUpdateProjectInputRequestTypeDef",
     {
         "ProjectName": str,
     },
@@ -14779,15 +13995,14 @@
         "LastModifiedTime": datetime,
         "CreatedBy": UserContextTypeDef,
         "LastModifiedBy": UserContextTypeDef,
         "ParallelismConfiguration": ParallelismConfigurationTypeDef,
         "PipelineParameters": List[ParameterTypeDef],
         "SelectiveExecutionConfig": SelectiveExecutionConfigTypeDef,
     },
-    total=False,
 )
 
 _RequiredStartPipelineExecutionRequestRequestTypeDef = TypedDict(
     "_RequiredStartPipelineExecutionRequestRequestTypeDef",
     {
         "PipelineName": str,
         "ClientRequestToken": str,
@@ -14938,15 +14153,14 @@
         "StepStatus": StepStatusType,
         "CacheHitResult": CacheHitResultTypeDef,
         "AttemptCount": int,
         "FailureReason": str,
         "Metadata": PipelineExecutionStepMetadataTypeDef,
         "SelectiveExecutionResult": SelectiveExecutionResultTypeDef,
     },
-    total=False,
 )
 
 DescribeAutoMLJobResponseTypeDef = TypedDict(
     "DescribeAutoMLJobResponseTypeDef",
     {
         "AutoMLJobName": str,
         "AutoMLJobArn": str,
@@ -15269,35 +14483,24 @@
 )
 
 class TrainingJobDefinitionTypeDef(
     _RequiredTrainingJobDefinitionTypeDef, _OptionalTrainingJobDefinitionTypeDef
 ):
     pass
 
-_RequiredInferenceRecommendationsJobStepTypeDef = TypedDict(
-    "_RequiredInferenceRecommendationsJobStepTypeDef",
+InferenceRecommendationsJobStepTypeDef = TypedDict(
+    "InferenceRecommendationsJobStepTypeDef",
     {
         "StepType": Literal["BENCHMARK"],
         "JobName": str,
         "Status": RecommendationJobStatusType,
-    },
-)
-_OptionalInferenceRecommendationsJobStepTypeDef = TypedDict(
-    "_OptionalInferenceRecommendationsJobStepTypeDef",
-    {
         "InferenceBenchmark": RecommendationJobInferenceBenchmarkTypeDef,
     },
-    total=False,
 )
 
-class InferenceRecommendationsJobStepTypeDef(
-    _RequiredInferenceRecommendationsJobStepTypeDef, _OptionalInferenceRecommendationsJobStepTypeDef
-):
-    pass
-
 ListAssociationsResponseTypeDef = TypedDict(
     "ListAssociationsResponseTypeDef",
     {
         "AssociationSummaries": List[AssociationSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -15315,15 +14518,14 @@
         "CreatedBy": UserContextTypeDef,
         "LastModifiedTime": datetime,
         "LastModifiedBy": UserContextTypeDef,
         "MetadataProperties": MetadataPropertiesTypeDef,
         "Tags": List[TagTypeDef],
         "TrialComponentSummaries": List[TrialComponentSimpleSummaryTypeDef],
     },
-    total=False,
 )
 
 ListTrialComponentsResponseTypeDef = TypedDict(
     "ListTrialComponentsResponseTypeDef",
     {
         "TrialComponentSummaries": List[TrialComponentSummaryTypeDef],
         "NextToken": str,
@@ -15361,43 +14563,32 @@
     {
         "NextToken": str,
         "AppImageConfigs": List[AppImageConfigDetailsTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredLabelingJobSummaryTypeDef = TypedDict(
-    "_RequiredLabelingJobSummaryTypeDef",
+LabelingJobSummaryTypeDef = TypedDict(
+    "LabelingJobSummaryTypeDef",
     {
         "LabelingJobName": str,
         "LabelingJobArn": str,
         "CreationTime": datetime,
         "LastModifiedTime": datetime,
         "LabelingJobStatus": LabelingJobStatusType,
         "LabelCounters": LabelCountersTypeDef,
         "WorkteamArn": str,
         "PreHumanTaskLambdaArn": str,
-    },
-)
-_OptionalLabelingJobSummaryTypeDef = TypedDict(
-    "_OptionalLabelingJobSummaryTypeDef",
-    {
         "AnnotationConsolidationLambdaArn": str,
         "FailureReason": str,
         "LabelingJobOutput": LabelingJobOutputTypeDef,
         "InputConfig": LabelingJobInputConfigTypeDef,
     },
-    total=False,
 )
 
-class LabelingJobSummaryTypeDef(
-    _RequiredLabelingJobSummaryTypeDef, _OptionalLabelingJobSummaryTypeDef
-):
-    pass
-
 DescribeWorkteamResponseTypeDef = TypedDict(
     "DescribeWorkteamResponseTypeDef",
     {
         "Workteam": WorkteamTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -15481,15 +14672,14 @@
         "VpcConfig": VpcConfigTypeDef,
         "CreationTime": datetime,
         "ModelArn": str,
         "EnableNetworkIsolation": bool,
         "Tags": List[TagTypeDef],
         "DeploymentRecommendation": DeploymentRecommendationTypeDef,
     },
-    total=False,
 )
 
 DescribeInferenceExperimentResponseTypeDef = TypedDict(
     "DescribeInferenceExperimentResponseTypeDef",
     {
         "Arn": str,
         "Name": str,
@@ -15608,40 +14798,28 @@
 )
 
 class UpdateModelPackageInputRequestTypeDef(
     _RequiredUpdateModelPackageInputRequestTypeDef, _OptionalUpdateModelPackageInputRequestTypeDef
 ):
     pass
 
-_RequiredBatchDescribeModelPackageSummaryTypeDef = TypedDict(
-    "_RequiredBatchDescribeModelPackageSummaryTypeDef",
+BatchDescribeModelPackageSummaryTypeDef = TypedDict(
+    "BatchDescribeModelPackageSummaryTypeDef",
     {
         "ModelPackageGroupName": str,
+        "ModelPackageVersion": int,
         "ModelPackageArn": str,
+        "ModelPackageDescription": str,
         "CreationTime": datetime,
         "InferenceSpecification": InferenceSpecificationTypeDef,
         "ModelPackageStatus": ModelPackageStatusType,
-    },
-)
-_OptionalBatchDescribeModelPackageSummaryTypeDef = TypedDict(
-    "_OptionalBatchDescribeModelPackageSummaryTypeDef",
-    {
-        "ModelPackageVersion": int,
-        "ModelPackageDescription": str,
         "ModelApprovalStatus": ModelApprovalStatusType,
     },
-    total=False,
 )
 
-class BatchDescribeModelPackageSummaryTypeDef(
-    _RequiredBatchDescribeModelPackageSummaryTypeDef,
-    _OptionalBatchDescribeModelPackageSummaryTypeDef,
-):
-    pass
-
 DataQualityJobInputTypeDef = TypedDict(
     "DataQualityJobInputTypeDef",
     {
         "EndpointInput": EndpointInputTypeDef,
         "BatchTransformInput": BatchTransformInputTypeDef,
     },
     total=False,
@@ -15784,15 +14962,14 @@
         "LastModifiedTime": datetime,
         "CreationTime": datetime,
         "MonitoringScheduleArn": str,
         "AutoMLJobArn": str,
         "TrainingJobArn": str,
         "Tags": List[TagTypeDef],
     },
-    total=False,
 )
 
 _RequiredCreateFlowDefinitionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateFlowDefinitionRequestRequestTypeDef",
     {
         "FlowDefinitionName": str,
         "HumanLoopConfig": HumanLoopConfigTypeDef,
@@ -16009,15 +15186,14 @@
         "DebugRuleConfigurations": List[DebugRuleConfigurationTypeDef],
         "TensorBoardOutputConfig": TensorBoardOutputConfigTypeDef,
         "DebugRuleEvaluationStatuses": List[DebugRuleEvaluationStatusTypeDef],
         "Environment": Dict[str, str],
         "RetryStrategy": RetryStrategyTypeDef,
         "Tags": List[TagTypeDef],
     },
-    total=False,
 )
 
 _RequiredCreateTransformJobRequestRequestTypeDef = TypedDict(
     "_RequiredCreateTransformJobRequestRequestTypeDef",
     {
         "TransformJobName": str,
         "ModelName": str,
@@ -16121,15 +15297,14 @@
         "TransformEndTime": datetime,
         "LabelingJobArn": str,
         "AutoMLJobArn": str,
         "DataProcessing": DataProcessingTypeDef,
         "ExperimentConfig": ExperimentConfigTypeDef,
         "Tags": List[TagTypeDef],
     },
-    total=False,
 )
 
 _RequiredCreateAutoMLJobV2RequestRequestTypeDef = TypedDict(
     "_RequiredCreateAutoMLJobV2RequestRequestTypeDef",
     {
         "AutoMLJobName": str,
         "AutoMLJobInputDataConfig": Sequence[AutoMLJobChannelTypeDef],
@@ -16415,15 +15590,14 @@
         "OverallBestTrainingJob": HyperParameterTrainingJobSummaryTypeDef,
         "WarmStartConfig": HyperParameterTuningJobWarmStartConfigTypeDef,
         "FailureReason": str,
         "Tags": List[TagTypeDef],
         "TuningJobCompletionDetails": HyperParameterTuningJobCompletionDetailsTypeDef,
         "ConsumedResources": HyperParameterTuningJobConsumedResourcesTypeDef,
     },
-    total=False,
 )
 
 ListInferenceRecommendationsJobStepsResponseTypeDef = TypedDict(
     "ListInferenceRecommendationsJobStepsResponseTypeDef",
     {
         "Steps": List[InferenceRecommendationsJobStepTypeDef],
         "NextToken": str,
@@ -16691,15 +15865,14 @@
     "TrialComponentSourceDetailTypeDef",
     {
         "SourceArn": str,
         "TrainingJob": TrainingJobTypeDef,
         "ProcessingJob": ProcessingJobTypeDef,
         "TransformJob": TransformJobTypeDef,
     },
-    total=False,
 )
 
 MonitoringScheduleConfigTypeDef = TypedDict(
     "MonitoringScheduleConfigTypeDef",
     {
         "ScheduleConfig": ScheduleConfigTypeDef,
         "MonitoringJobDefinition": MonitoringJobDefinitionTypeDef,
@@ -16746,15 +15919,14 @@
         "MetadataProperties": MetadataPropertiesTypeDef,
         "SourceDetail": TrialComponentSourceDetailTypeDef,
         "LineageGroupArn": str,
         "Tags": List[TagTypeDef],
         "Parents": List[ParentTypeDef],
         "RunName": str,
     },
-    total=False,
 )
 
 _RequiredCreateMonitoringScheduleRequestRequestTypeDef = TypedDict(
     "_RequiredCreateMonitoringScheduleRequestRequestTypeDef",
     {
         "MonitoringScheduleName": str,
         "MonitoringScheduleConfig": MonitoringScheduleConfigTypeDef,
@@ -16802,15 +15974,14 @@
         "CreationTime": datetime,
         "LastModifiedTime": datetime,
         "MonitoringScheduleConfig": MonitoringScheduleConfigTypeDef,
         "EndpointName": str,
         "MonitoringAlertSummaries": List[MonitoringAlertSummaryTypeDef],
         "LastMonitoringExecutionSummary": MonitoringExecutionSummaryTypeDef,
     },
-    total=False,
 )
 
 MonitoringScheduleTypeDef = TypedDict(
     "MonitoringScheduleTypeDef",
     {
         "MonitoringScheduleArn": str,
         "MonitoringScheduleName": str,
@@ -16820,15 +15991,14 @@
         "CreationTime": datetime,
         "LastModifiedTime": datetime,
         "MonitoringScheduleConfig": MonitoringScheduleConfigTypeDef,
         "EndpointName": str,
         "LastMonitoringExecutionSummary": MonitoringExecutionSummaryTypeDef,
         "Tags": List[TagTypeDef],
     },
-    total=False,
 )
 
 UpdateMonitoringScheduleRequestRequestTypeDef = TypedDict(
     "UpdateMonitoringScheduleRequestRequestTypeDef",
     {
         "MonitoringScheduleName": str,
         "MonitoringScheduleConfig": MonitoringScheduleConfigTypeDef,
@@ -16966,56 +16136,45 @@
         "AdditionalInferenceSpecifications": List[
             AdditionalInferenceSpecificationDefinitionTypeDef
         ],
         "Tags": List[TagTypeDef],
         "CustomerMetadataProperties": Dict[str, str],
         "DriftCheckBaselines": DriftCheckBaselinesTypeDef,
     },
-    total=False,
 )
 
 ModelDashboardModelTypeDef = TypedDict(
     "ModelDashboardModelTypeDef",
     {
         "Model": ModelTypeDef,
         "Endpoints": List[ModelDashboardEndpointTypeDef],
         "LastBatchTransformJob": TransformJobTypeDef,
         "MonitoringSchedules": List[ModelDashboardMonitoringScheduleTypeDef],
         "ModelCard": ModelDashboardModelCardTypeDef,
     },
-    total=False,
 )
 
-_RequiredEndpointTypeDef = TypedDict(
-    "_RequiredEndpointTypeDef",
+EndpointTypeDef = TypedDict(
+    "EndpointTypeDef",
     {
         "EndpointName": str,
         "EndpointArn": str,
         "EndpointConfigName": str,
-        "EndpointStatus": EndpointStatusType,
-        "CreationTime": datetime,
-        "LastModifiedTime": datetime,
-    },
-)
-_OptionalEndpointTypeDef = TypedDict(
-    "_OptionalEndpointTypeDef",
-    {
         "ProductionVariants": List[ProductionVariantSummaryTypeDef],
         "DataCaptureConfig": DataCaptureConfigSummaryTypeDef,
+        "EndpointStatus": EndpointStatusType,
         "FailureReason": str,
+        "CreationTime": datetime,
+        "LastModifiedTime": datetime,
         "MonitoringSchedules": List[MonitoringScheduleTypeDef],
         "Tags": List[TagTypeDef],
         "ShadowProductionVariants": List[ProductionVariantSummaryTypeDef],
     },
-    total=False,
 )
 
-class EndpointTypeDef(_RequiredEndpointTypeDef, _OptionalEndpointTypeDef):
-    pass
-
 SearchRecordTypeDef = TypedDict(
     "SearchRecordTypeDef",
     {
         "TrainingJob": TrainingJobTypeDef,
         "Experiment": ExperimentTypeDef,
         "Trial": TrialTypeDef,
         "TrialComponent": TrialComponentTypeDef,
@@ -17027,15 +16186,14 @@
         "FeatureGroup": FeatureGroupTypeDef,
         "Project": ProjectTypeDef,
         "FeatureMetadata": FeatureMetadataTypeDef,
         "HyperParameterTuningJob": HyperParameterTuningJobSearchEntityTypeDef,
         "Model": ModelDashboardModelTypeDef,
         "ModelCard": ModelCardTypeDef,
     },
-    total=False,
 )
 
 SearchResponseTypeDef = TypedDict(
     "SearchResponseTypeDef",
     {
         "Results": List[SearchRecordTypeDef],
         "NextToken": str,
```

### Comparing `mypy-boto3-sagemaker-1.28.0/mypy_boto3_sagemaker/waiter.py` & `mypy-boto3-sagemaker-1.28.3/mypy_boto3_sagemaker/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sagemaker-1.28.0/mypy_boto3_sagemaker/waiter.pyi` & `mypy-boto3-sagemaker-1.28.3/mypy_boto3_sagemaker/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sagemaker-1.28.0/mypy_boto3_sagemaker.egg-info/PKG-INFO` & `mypy-boto3-sagemaker-1.28.3/mypy_boto3_sagemaker.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-sagemaker
-Version: 1.28.0
-Summary: Type annotations for boto3.SageMaker 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.3
+Summary: Type annotations for boto3.SageMaker 1.28.3 service generated with mypy-boto3-builder 7.14.6
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-sagemaker.svg?color=blue)](https://pypi.org/project/mypy-boto3-sagemaker)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-sagemaker?color=blue)](https://pypistats.org/packages/mypy-boto3-sagemaker)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SageMaker 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker)
+[boto3.SageMaker 1.28.3](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker)
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
 [mypy-boto3-sagemaker docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker/).
 
 See how it helps to find and fix potential bugs:
 
@@ -962,14 +962,15 @@
     MetricsSourceTypeDef,
     CacheHitResultTypeDef,
     OutputParameterTypeDef,
     CandidateArtifactLocationsTypeDef,
     MetricDatumTypeDef,
     ModelRegisterSettingsTypeDef,
     TimeSeriesForecastingSettingsTypeDef,
+    WorkspaceSettingsTypeDef,
     CapacitySizeTypeDef,
     CaptureContentTypeHeaderTypeDef,
     CaptureOptionTypeDef,
     CategoricalParameterRangeSpecificationTypeDef,
     CategoricalParameterRangeTypeDef,
     CategoricalParameterTypeDef,
     ChannelSpecificationTypeDef,
```

### Comparing `mypy-boto3-sagemaker-1.28.0/mypy_boto3_sagemaker.egg-info/SOURCES.txt` & `mypy-boto3-sagemaker-1.28.3/mypy_boto3_sagemaker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sagemaker-1.28.0/setup.py` & `mypy-boto3-sagemaker-1.28.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-sagemaker",
-    version="1.28.0",
+    version="1.28.3",
     packages=["mypy_boto3_sagemaker"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.SageMaker 1.28.0 service generated with mypy-boto3-builder"
-        " 7.14.5"
+        "Type annotations for boto3.SageMaker 1.28.3 service generated with mypy-boto3-builder"
+        " 7.14.6"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

