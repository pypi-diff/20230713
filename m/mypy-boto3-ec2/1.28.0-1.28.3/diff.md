# Comparing `tmp/mypy-boto3-ec2-1.28.0.tar.gz` & `tmp/mypy-boto3-ec2-1.28.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-ec2-1.28.0.tar", last modified: Thu Jul  6 20:59:29 2023, max compression
+gzip compressed data, was "mypy-boto3-ec2-1.28.3.tar", last modified: Thu Jul 13 19:49:12 2023, max compression
```

## Comparing `mypy-boto3-ec2-1.28.0.tar` & `mypy-boto3-ec2-1.28.3.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:29.514290 mypy-boto3-ec2-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:38:52.000000 mypy-boto3-ec2-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)   170472 2023-07-06 20:59:29.502290 mypy-boto3-ec2-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)   169003 2023-07-06 20:38:52.000000 mypy-boto3-ec2-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:29.490290 mypy-boto3-ec2-1.28.0/mypy_boto3_ec2/
--rw-r--r--   0 runner    (1001) docker     (123)    46235 2023-07-06 20:38:52.000000 mypy-boto3-ec2-1.28.0/mypy_boto3_ec2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    46233 2023-07-06 20:38:52.000000 mypy-boto3-ec2-1.28.0/mypy_boto3_ec2/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-06 20:38:52.000000 mypy-boto3-ec2-1.28.0/mypy_boto3_ec2/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)   519979 2023-07-06 20:39:01.000000 mypy-boto3-ec2-1.28.0/mypy_boto3_ec2/client.py
--rw-r--r--   0 runner    (1001) docker     (123)   519205 2023-07-06 20:38:56.000000 mypy-boto3-ec2-1.28.0/mypy_boto3_ec2/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    89678 2023-07-06 20:39:11.000000 mypy-boto3-ec2-1.28.0/mypy_boto3_ec2/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    89676 2023-07-06 20:39:10.000000 mypy-boto3-ec2-1.28.0/mypy_boto3_ec2/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)   182527 2023-07-06 20:39:07.000000 mypy-boto3-ec2-1.28.0/mypy_boto3_ec2/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)   182386 2023-07-06 20:39:06.000000 mypy-boto3-ec2-1.28.0/mypy_boto3_ec2/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:38:52.000000 mypy-boto3-ec2-1.28.0/mypy_boto3_ec2/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   269571 2023-07-06 20:39:05.000000 mypy-boto3-ec2-1.28.0/mypy_boto3_ec2/service_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)   269106 2023-07-06 20:39:04.000000 mypy-boto3-ec2-1.28.0/mypy_boto3_ec2/service_resource.pyi
--rw-r--r--   0 runner    (1001) docker     (123)   954716 2023-07-06 20:39:45.000000 mypy-boto3-ec2-1.28.0/mypy_boto3_ec2/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   953709 2023-07-06 20:39:28.000000 mypy-boto3-ec2-1.28.0/mypy_boto3_ec2/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:38:52.000000 mypy-boto3-ec2-1.28.0/mypy_boto3_ec2/version.py
--rw-r--r--   0 runner    (1001) docker     (123)    38527 2023-07-06 20:39:09.000000 mypy-boto3-ec2-1.28.0/mypy_boto3_ec2/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)    38492 2023-07-06 20:39:09.000000 mypy-boto3-ec2-1.28.0/mypy_boto3_ec2/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:29.502290 mypy-boto3-ec2-1.28.0/mypy_boto3_ec2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)   170472 2023-07-06 20:59:29.000000 mypy-boto3-ec2-1.28.0/mypy_boto3_ec2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-07-06 20:59:29.000000 mypy-boto3-ec2-1.28.0/mypy_boto3_ec2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:29.000000 mypy-boto3-ec2-1.28.0/mypy_boto3_ec2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:29.000000 mypy-boto3-ec2-1.28.0/mypy_boto3_ec2.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 20:59:29.000000 mypy-boto3-ec2-1.28.0/mypy_boto3_ec2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-06 20:59:29.000000 mypy-boto3-ec2-1.28.0/mypy_boto3_ec2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 20:59:29.514290 mypy-boto3-ec2-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-07-06 20:38:51.000000 mypy-boto3-ec2-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:49:12.685228 mypy-boto3-ec2-1.28.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-13 19:47:28.000000 mypy-boto3-ec2-1.28.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)   170472 2023-07-13 19:49:12.685228 mypy-boto3-ec2-1.28.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)   169003 2023-07-13 19:47:28.000000 mypy-boto3-ec2-1.28.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:49:12.685228 mypy-boto3-ec2-1.28.3/mypy_boto3_ec2/
+-rw-r--r--   0 runner    (1001) docker     (123)    46235 2023-07-13 19:47:28.000000 mypy-boto3-ec2-1.28.3/mypy_boto3_ec2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46233 2023-07-13 19:47:28.000000 mypy-boto3-ec2-1.28.3/mypy_boto3_ec2/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-13 19:47:28.000000 mypy-boto3-ec2-1.28.3/mypy_boto3_ec2/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   519979 2023-07-13 19:47:34.000000 mypy-boto3-ec2-1.28.3/mypy_boto3_ec2/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)   519205 2023-07-13 19:47:31.000000 mypy-boto3-ec2-1.28.3/mypy_boto3_ec2/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    89900 2023-07-13 19:47:41.000000 mypy-boto3-ec2-1.28.3/mypy_boto3_ec2/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    89898 2023-07-13 19:47:39.000000 mypy-boto3-ec2-1.28.3/mypy_boto3_ec2/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)   182527 2023-07-13 19:47:38.000000 mypy-boto3-ec2-1.28.3/mypy_boto3_ec2/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)   182386 2023-07-13 19:47:38.000000 mypy-boto3-ec2-1.28.3/mypy_boto3_ec2/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 19:47:28.000000 mypy-boto3-ec2-1.28.3/mypy_boto3_ec2/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   269571 2023-07-13 19:47:36.000000 mypy-boto3-ec2-1.28.3/mypy_boto3_ec2/service_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)   269106 2023-07-13 19:47:35.000000 mypy-boto3-ec2-1.28.3/mypy_boto3_ec2/service_resource.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)   945658 2023-07-13 19:48:02.000000 mypy-boto3-ec2-1.28.3/mypy_boto3_ec2/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   944653 2023-07-13 19:47:51.000000 mypy-boto3-ec2-1.28.3/mypy_boto3_ec2/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-13 19:47:28.000000 mypy-boto3-ec2-1.28.3/mypy_boto3_ec2/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38527 2023-07-13 19:47:39.000000 mypy-boto3-ec2-1.28.3/mypy_boto3_ec2/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38492 2023-07-13 19:47:38.000000 mypy-boto3-ec2-1.28.3/mypy_boto3_ec2/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:49:12.685228 mypy-boto3-ec2-1.28.3/mypy_boto3_ec2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)   170472 2023-07-13 19:49:12.000000 mypy-boto3-ec2-1.28.3/mypy_boto3_ec2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-07-13 19:49:12.000000 mypy-boto3-ec2-1.28.3/mypy_boto3_ec2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 19:49:12.000000 mypy-boto3-ec2-1.28.3/mypy_boto3_ec2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 19:49:12.000000 mypy-boto3-ec2-1.28.3/mypy_boto3_ec2.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-13 19:49:12.000000 mypy-boto3-ec2-1.28.3/mypy_boto3_ec2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-13 19:49:12.000000 mypy-boto3-ec2-1.28.3/mypy_boto3_ec2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 19:49:12.685228 mypy-boto3-ec2-1.28.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-07-13 19:47:27.000000 mypy-boto3-ec2-1.28.3/setup.py
```

### Comparing `mypy-boto3-ec2-1.28.0/LICENSE` & `mypy-boto3-ec2-1.28.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ec2-1.28.0/PKG-INFO` & `mypy-boto3-ec2-1.28.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-ec2
-Version: 1.28.0
-Summary: Type annotations for boto3.EC2 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.3
+Summary: Type annotations for boto3.EC2 1.28.3 service generated with mypy-boto3-builder 7.14.6
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ec2.svg?color=blue)](https://pypi.org/project/mypy-boto3-ec2)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-ec2?color=blue)](https://pypistats.org/packages/mypy-boto3-ec2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.EC2 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2)
+[boto3.EC2 1.28.3](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2)
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
 [mypy-boto3-ec2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-ec2-1.28.0/README.md` & `mypy-boto3-ec2-1.28.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ec2.svg?color=blue)](https://pypi.org/project/mypy-boto3-ec2)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-ec2?color=blue)](https://pypistats.org/packages/mypy-boto3-ec2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.EC2 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2)
+[boto3.EC2 1.28.3](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2)
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
 [mypy-boto3-ec2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-ec2-1.28.0/mypy_boto3_ec2/__init__.py` & `mypy-boto3-ec2-1.28.3/mypy_boto3_ec2/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ec2-1.28.0/mypy_boto3_ec2/__init__.pyi` & `mypy-boto3-ec2-1.28.3/mypy_boto3_ec2/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ec2-1.28.0/mypy_boto3_ec2/__main__.py` & `mypy-boto3-ec2-1.28.3/mypy_boto3_ec2/__main__.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.EC2 1.28.0\nVersion:         1.28.0\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.EC2 1.28.3\nVersion:         1.28.3\nBuilder version:"
+        " 7.14.6\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2\nOther"
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

### Comparing `mypy-boto3-ec2-1.28.0/mypy_boto3_ec2/client.py` & `mypy-boto3-ec2-1.28.3/mypy_boto3_ec2/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ec2-1.28.0/mypy_boto3_ec2/client.pyi` & `mypy-boto3-ec2-1.28.3/mypy_boto3_ec2/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ec2-1.28.0/mypy_boto3_ec2/literals.py` & `mypy-boto3-ec2-1.28.3/mypy_boto3_ec2/literals.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "AcceleratorManufacturerType",
     "AcceleratorNameType",
     "AcceleratorTypeType",
     "AccountAttributeNameType",
     "ActivityStatusType",
     "AddressAttributeNameType",
@@ -506,15 +505,14 @@
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "WaiterName",
     "RegionName",
 )
 
-
 AcceleratorManufacturerType = Literal["amazon-web-services", "amd", "nvidia", "xilinx"]
 AcceleratorNameType = Literal[
     "a100", "inferentia", "k520", "k80", "m60", "radeon-pro-v520", "t4", "v100", "vu9p"
 ]
 AcceleratorTypeType = Literal["fpga", "gpu", "inference"]
 AccountAttributeNameType = Literal["default-vpc", "supported-platforms"]
 ActivityStatusType = Literal["error", "fulfilled", "pending_fulfillment", "pending_termination"]
@@ -1126,14 +1124,22 @@
     "c7g.2xlarge",
     "c7g.4xlarge",
     "c7g.8xlarge",
     "c7g.large",
     "c7g.medium",
     "c7g.metal",
     "c7g.xlarge",
+    "c7gn.12xlarge",
+    "c7gn.16xlarge",
+    "c7gn.2xlarge",
+    "c7gn.4xlarge",
+    "c7gn.8xlarge",
+    "c7gn.large",
+    "c7gn.medium",
+    "c7gn.xlarge",
     "cc1.4xlarge",
     "cc2.8xlarge",
     "cg1.4xlarge",
     "cr1.8xlarge",
     "d2.2xlarge",
     "d2.4xlarge",
     "d2.8xlarge",
@@ -1187,14 +1193,17 @@
     "h1.16xlarge",
     "h1.2xlarge",
     "h1.4xlarge",
     "h1.8xlarge",
     "hi1.4xlarge",
     "hpc6a.48xlarge",
     "hpc6id.32xlarge",
+    "hpc7g.16xlarge",
+    "hpc7g.4xlarge",
+    "hpc7g.8xlarge",
     "hs1.8xlarge",
     "i2.2xlarge",
     "i2.4xlarge",
     "i2.8xlarge",
     "i2.xlarge",
     "i3.16xlarge",
     "i3.2xlarge",
```

### Comparing `mypy-boto3-ec2-1.28.0/mypy_boto3_ec2/literals.pyi` & `mypy-boto3-ec2-1.28.3/mypy_boto3_ec2/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = (
     "AcceleratorManufacturerType",
     "AcceleratorNameType",
     "AcceleratorTypeType",
     "AccountAttributeNameType",
     "ActivityStatusType",
     "AddressAttributeNameType",
@@ -505,14 +506,15 @@
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "WaiterName",
     "RegionName",
 )
 
+
 AcceleratorManufacturerType = Literal["amazon-web-services", "amd", "nvidia", "xilinx"]
 AcceleratorNameType = Literal[
     "a100", "inferentia", "k520", "k80", "m60", "radeon-pro-v520", "t4", "v100", "vu9p"
 ]
 AcceleratorTypeType = Literal["fpga", "gpu", "inference"]
 AccountAttributeNameType = Literal["default-vpc", "supported-platforms"]
 ActivityStatusType = Literal["error", "fulfilled", "pending_fulfillment", "pending_termination"]
@@ -1124,14 +1126,22 @@
     "c7g.2xlarge",
     "c7g.4xlarge",
     "c7g.8xlarge",
     "c7g.large",
     "c7g.medium",
     "c7g.metal",
     "c7g.xlarge",
+    "c7gn.12xlarge",
+    "c7gn.16xlarge",
+    "c7gn.2xlarge",
+    "c7gn.4xlarge",
+    "c7gn.8xlarge",
+    "c7gn.large",
+    "c7gn.medium",
+    "c7gn.xlarge",
     "cc1.4xlarge",
     "cc2.8xlarge",
     "cg1.4xlarge",
     "cr1.8xlarge",
     "d2.2xlarge",
     "d2.4xlarge",
     "d2.8xlarge",
@@ -1185,14 +1195,17 @@
     "h1.16xlarge",
     "h1.2xlarge",
     "h1.4xlarge",
     "h1.8xlarge",
     "hi1.4xlarge",
     "hpc6a.48xlarge",
     "hpc6id.32xlarge",
+    "hpc7g.16xlarge",
+    "hpc7g.4xlarge",
+    "hpc7g.8xlarge",
     "hs1.8xlarge",
     "i2.2xlarge",
     "i2.4xlarge",
     "i2.8xlarge",
     "i2.xlarge",
     "i3.16xlarge",
     "i3.2xlarge",
```

### Comparing `mypy-boto3-ec2-1.28.0/mypy_boto3_ec2/paginator.py` & `mypy-boto3-ec2-1.28.3/mypy_boto3_ec2/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ec2-1.28.0/mypy_boto3_ec2/paginator.pyi` & `mypy-boto3-ec2-1.28.3/mypy_boto3_ec2/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ec2-1.28.0/mypy_boto3_ec2/service_resource.py` & `mypy-boto3-ec2-1.28.3/mypy_boto3_ec2/service_resource.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ec2-1.28.0/mypy_boto3_ec2/service_resource.pyi` & `mypy-boto3-ec2-1.28.3/mypy_boto3_ec2/service_resource.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ec2-1.28.0/mypy_boto3_ec2/type_defs.py` & `mypy-boto3-ec2-1.28.3/mypy_boto3_ec2/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -2468,15 +2468,14 @@
 
 AcceleratorCountTypeDef = TypedDict(
     "AcceleratorCountTypeDef",
     {
         "Min": int,
         "Max": int,
     },
-    total=False,
 )
 
 AcceleratorTotalMemoryMiBRequestTypeDef = TypedDict(
     "AcceleratorTotalMemoryMiBRequestTypeDef",
     {
         "Min": int,
         "Max": int,
@@ -2486,28 +2485,26 @@
 
 AcceleratorTotalMemoryMiBTypeDef = TypedDict(
     "AcceleratorTotalMemoryMiBTypeDef",
     {
         "Min": int,
         "Max": int,
     },
-    total=False,
 )
 
 AddressTransferTypeDef = TypedDict(
     "AddressTransferTypeDef",
     {
         "PublicIp": str,
         "AllocationId": str,
         "TransferAccountId": str,
         "TransferOfferExpirationTimestamp": datetime,
         "TransferOfferAcceptedTimestamp": datetime,
         "AddressTransferStatus": AddressTransferStatusType,
     },
-    total=False,
 )
 
 _RequiredTargetConfigurationRequestTypeDef = TypedDict(
     "_RequiredTargetConfigurationRequestTypeDef",
     {
         "OfferingId": str,
     },
@@ -2644,26 +2641,24 @@
 )
 
 AccountAttributeValueTypeDef = TypedDict(
     "AccountAttributeValueTypeDef",
     {
         "AttributeValue": str,
     },
-    total=False,
 )
 
 ActiveInstanceTypeDef = TypedDict(
     "ActiveInstanceTypeDef",
     {
         "InstanceId": str,
         "InstanceType": str,
         "SpotInstanceRequestId": str,
         "InstanceHealth": InstanceHealthStatusType,
     },
-    total=False,
 )
 
 AddIpamOperatingRegionTypeDef = TypedDict(
     "AddIpamOperatingRegionTypeDef",
     {
         "RegionName": str,
     },
@@ -2695,53 +2690,48 @@
     "AddedPrincipalTypeDef",
     {
         "PrincipalType": PrincipalTypeType,
         "Principal": str,
         "ServicePermissionId": str,
         "ServiceId": str,
     },
-    total=False,
 )
 
 AnalysisComponentTypeDef = TypedDict(
     "AnalysisComponentTypeDef",
     {
         "Id": str,
         "Arn": str,
         "Name": str,
     },
-    total=False,
 )
 
 RuleGroupTypePairTypeDef = TypedDict(
     "RuleGroupTypePairTypeDef",
     {
         "RuleGroupArn": str,
         "RuleGroupType": str,
     },
-    total=False,
 )
 
 RuleOptionTypeDef = TypedDict(
     "RuleOptionTypeDef",
     {
         "Keyword": str,
         "Settings": List[str],
     },
-    total=False,
 )
 
 PtrUpdateStatusTypeDef = TypedDict(
     "PtrUpdateStatusTypeDef",
     {
         "Value": str,
         "Status": str,
         "Reason": str,
     },
-    total=False,
 )
 
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
@@ -2775,15 +2765,14 @@
     "ByoipCidrTypeDef",
     {
         "Cidr": str,
         "Description": str,
         "StatusMessage": str,
         "State": ByoipCidrStateType,
     },
-    total=False,
 )
 
 AllocateAddressResultTypeDef = TypedDict(
     "AllocateAddressResultTypeDef",
     {
         "PublicIp": str,
         "AllocationId": str,
@@ -2840,42 +2829,38 @@
         "IpamPoolAllocationId": str,
         "Description": str,
         "ResourceId": str,
         "ResourceType": IpamPoolAllocationResourceTypeType,
         "ResourceRegion": str,
         "ResourceOwner": str,
     },
-    total=False,
 )
 
 AlternatePathHintTypeDef = TypedDict(
     "AlternatePathHintTypeDef",
     {
         "ComponentId": str,
         "ComponentArn": str,
     },
-    total=False,
 )
 
 PortRangeTypeDef = TypedDict(
     "PortRangeTypeDef",
     {
         "From": int,
         "To": int,
     },
-    total=False,
 )
 
 AnalysisLoadBalancerListenerTypeDef = TypedDict(
     "AnalysisLoadBalancerListenerTypeDef",
     {
         "LoadBalancerPort": int,
         "InstancePort": int,
     },
-    total=False,
 )
 
 AnalysisRouteTableRouteTypeDef = TypedDict(
     "AnalysisRouteTableRouteTypeDef",
     {
         "DestinationCidr": str,
         "DestinationPrefixListId": str,
@@ -2888,15 +2873,14 @@
         "TransitGatewayId": str,
         "VpcPeeringConnectionId": str,
         "State": str,
         "CarrierGatewayId": str,
         "CoreNetworkArn": str,
         "LocalGatewayId": str,
     },
-    total=False,
 )
 
 _RequiredApplySecurityGroupsToClientVpnTargetNetworkRequestRequestTypeDef = TypedDict(
     "_RequiredApplySecurityGroupsToClientVpnTargetNetworkRequestRequestTypeDef",
     {
         "ClientVpnEndpointId": str,
         "VpcId": str,
@@ -3001,23 +2985,21 @@
 
 
 AssignedPrivateIpAddressTypeDef = TypedDict(
     "AssignedPrivateIpAddressTypeDef",
     {
         "PrivateIpAddress": str,
     },
-    total=False,
 )
 
 Ipv4PrefixSpecificationTypeDef = TypedDict(
     "Ipv4PrefixSpecificationTypeDef",
     {
         "Ipv4Prefix": str,
     },
-    total=False,
 )
 
 _RequiredAssignPrivateNatGatewayAddressRequestRequestTypeDef = TypedDict(
     "_RequiredAssignPrivateNatGatewayAddressRequestRequestTypeDef",
     {
         "NatGatewayId": str,
     },
@@ -3048,15 +3030,14 @@
         "PrivateIp": str,
         "PublicIp": str,
         "AssociationId": str,
         "IsPrimary": bool,
         "FailureMessage": str,
         "Status": NatGatewayAddressStatusType,
     },
-    total=False,
 )
 
 AssociateAddressRequestClassicAddressAssociateTypeDef = TypedDict(
     "AssociateAddressRequestClassicAddressAssociateTypeDef",
     {
         "AllocationId": str,
         "InstanceId": str,
@@ -3129,15 +3110,14 @@
 
 AssociationStatusTypeDef = TypedDict(
     "AssociationStatusTypeDef",
     {
         "Code": AssociationStatusCodeType,
         "Message": str,
     },
-    total=False,
 )
 
 _RequiredAssociateDhcpOptionsRequestDhcpOptionsAssociateWithVpcTypeDef = TypedDict(
     "_RequiredAssociateDhcpOptionsRequestDhcpOptionsAssociateWithVpcTypeDef",
     {
         "VpcId": str,
     },
@@ -3305,15 +3285,14 @@
 
 RouteTableAssociationStateTypeDef = TypedDict(
     "RouteTableAssociationStateTypeDef",
     {
         "State": RouteTableAssociationStateCodeType,
         "StatusMessage": str,
     },
-    total=False,
 )
 
 AssociateSubnetCidrBlockRequestRequestTypeDef = TypedDict(
     "AssociateSubnetCidrBlockRequestRequestTypeDef",
     {
         "Ipv6CidrBlock": str,
         "SubnetId": str,
@@ -3372,15 +3351,14 @@
     {
         "TransitGatewayPolicyTableId": str,
         "TransitGatewayAttachmentId": str,
         "ResourceId": str,
         "ResourceType": TransitGatewayAttachmentResourceTypeType,
         "State": TransitGatewayAssociationStateType,
     },
-    total=False,
 )
 
 _RequiredAssociateTransitGatewayRouteTableRequestRequestTypeDef = TypedDict(
     "_RequiredAssociateTransitGatewayRouteTableRequestRequestTypeDef",
     {
         "TransitGatewayRouteTableId": str,
         "TransitGatewayAttachmentId": str,
@@ -3407,15 +3385,14 @@
     {
         "TransitGatewayRouteTableId": str,
         "TransitGatewayAttachmentId": str,
         "ResourceId": str,
         "ResourceType": TransitGatewayAttachmentResourceTypeType,
         "State": TransitGatewayAssociationStateType,
     },
-    total=False,
 )
 
 _RequiredAssociateTrunkInterfaceRequestRequestTypeDef = TypedDict(
     "_RequiredAssociateTrunkInterfaceRequestRequestTypeDef",
     {
         "BranchInterfaceId": str,
         "TrunkInterfaceId": str,
@@ -3474,24 +3451,22 @@
     "AssociatedRoleTypeDef",
     {
         "AssociatedRoleArn": str,
         "CertificateS3BucketName": str,
         "CertificateS3ObjectKey": str,
         "EncryptionKmsKeyId": str,
     },
-    total=False,
 )
 
 AssociatedTargetNetworkTypeDef = TypedDict(
     "AssociatedTargetNetworkTypeDef",
     {
         "NetworkId": str,
         "NetworkType": Literal["vpc"],
     },
-    total=False,
 )
 
 _RequiredAthenaIntegrationTypeDef = TypedDict(
     "_RequiredAthenaIntegrationTypeDef",
     {
         "IntegrationResultS3DestinationArn": str,
         "PartitionLoadFrequency": PartitionLoadFrequencyType,
@@ -3784,48 +3759,43 @@
 
 VpcAttachmentTypeDef = TypedDict(
     "VpcAttachmentTypeDef",
     {
         "State": AttachmentStatusType,
         "VpcId": str,
     },
-    total=False,
 )
 
 AttachmentEnaSrdUdpSpecificationTypeDef = TypedDict(
     "AttachmentEnaSrdUdpSpecificationTypeDef",
     {
         "EnaSrdUdpEnabled": bool,
     },
-    total=False,
 )
 
 AttributeBooleanValueTypeDef = TypedDict(
     "AttributeBooleanValueTypeDef",
     {
         "Value": bool,
     },
-    total=False,
 )
 
 AttributeValueTypeDef = TypedDict(
     "AttributeValueTypeDef",
     {
         "Value": str,
     },
-    total=False,
 )
 
 ClientVpnAuthorizationRuleStatusTypeDef = TypedDict(
     "ClientVpnAuthorizationRuleStatusTypeDef",
     {
         "Code": ClientVpnAuthorizationRuleStatusCodeType,
         "Message": str,
     },
-    total=False,
 )
 
 _RequiredAuthorizeClientVpnIngressRequestRequestTypeDef = TypedDict(
     "_RequiredAuthorizeClientVpnIngressRequestRequestTypeDef",
     {
         "ClientVpnEndpointId": str,
         "TargetNetworkCidr": str,
@@ -3852,25 +3822,23 @@
 
 
 AvailabilityZoneMessageTypeDef = TypedDict(
     "AvailabilityZoneMessageTypeDef",
     {
         "Message": str,
     },
-    total=False,
 )
 
 InstanceCapacityTypeDef = TypedDict(
     "InstanceCapacityTypeDef",
     {
         "AvailableCapacity": int,
         "InstanceType": str,
         "TotalCapacity": int,
     },
-    total=False,
 )
 
 BaselineEbsBandwidthMbpsRequestTypeDef = TypedDict(
     "BaselineEbsBandwidthMbpsRequestTypeDef",
     {
         "Min": int,
         "Max": int,
@@ -3880,15 +3848,14 @@
 
 BaselineEbsBandwidthMbpsTypeDef = TypedDict(
     "BaselineEbsBandwidthMbpsTypeDef",
     {
         "Min": int,
         "Max": int,
     },
-    total=False,
 )
 
 BlobAttributeValueTypeDef = TypedDict(
     "BlobAttributeValueTypeDef",
     {
         "Value": Union[str, bytes, IO[Any], StreamingBody],
     },
@@ -3913,15 +3880,14 @@
 
 BundleTaskErrorTypeDef = TypedDict(
     "BundleTaskErrorTypeDef",
     {
         "Code": str,
         "Message": str,
     },
-    total=False,
 )
 
 _RequiredCancelBundleTaskRequestRequestTypeDef = TypedDict(
     "_RequiredCancelBundleTaskRequestRequestTypeDef",
     {
         "BundleId": str,
     },
@@ -3943,15 +3909,14 @@
 
 CancelCapacityReservationFleetErrorTypeDef = TypedDict(
     "CancelCapacityReservationFleetErrorTypeDef",
     {
         "Code": str,
         "Message": str,
     },
-    total=False,
 )
 
 _RequiredCancelCapacityReservationFleetsRequestRequestTypeDef = TypedDict(
     "_RequiredCancelCapacityReservationFleetsRequestRequestTypeDef",
     {
         "CapacityReservationFleetIds": Sequence[str],
     },
@@ -3975,15 +3940,14 @@
 CapacityReservationFleetCancellationStateTypeDef = TypedDict(
     "CapacityReservationFleetCancellationStateTypeDef",
     {
         "CurrentFleetState": CapacityReservationFleetStateType,
         "PreviousFleetState": CapacityReservationFleetStateType,
         "CapacityReservationFleetId": str,
     },
-    total=False,
 )
 
 _RequiredCancelCapacityReservationRequestRequestTypeDef = TypedDict(
     "_RequiredCancelCapacityReservationRequestRequestTypeDef",
     {
         "CapacityReservationId": str,
     },
@@ -4100,15 +4064,14 @@
 
 CancelSpotFleetRequestsErrorTypeDef = TypedDict(
     "CancelSpotFleetRequestsErrorTypeDef",
     {
         "Code": CancelBatchErrorCodeType,
         "Message": str,
     },
-    total=False,
 )
 
 _RequiredCancelSpotFleetRequestsRequestRequestTypeDef = TypedDict(
     "_RequiredCancelSpotFleetRequestsRequestRequestTypeDef",
     {
         "SpotFleetRequestIds": Sequence[str],
         "TerminateInstances": bool,
@@ -4133,15 +4096,14 @@
 CancelSpotFleetRequestsSuccessItemTypeDef = TypedDict(
     "CancelSpotFleetRequestsSuccessItemTypeDef",
     {
         "CurrentSpotFleetRequestState": BatchStateType,
         "PreviousSpotFleetRequestState": BatchStateType,
         "SpotFleetRequestId": str,
     },
-    total=False,
 )
 
 _RequiredCancelSpotInstanceRequestsRequestRequestTypeDef = TypedDict(
     "_RequiredCancelSpotInstanceRequestsRequestRequestTypeDef",
     {
         "SpotInstanceRequestIds": Sequence[str],
     },
@@ -4164,24 +4126,22 @@
 
 CancelledSpotInstanceRequestTypeDef = TypedDict(
     "CancelledSpotInstanceRequestTypeDef",
     {
         "SpotInstanceRequestId": str,
         "State": CancelSpotInstanceRequestStateType,
     },
-    total=False,
 )
 
 CapacityAllocationTypeDef = TypedDict(
     "CapacityAllocationTypeDef",
     {
         "AllocationType": Literal["used"],
         "Count": int,
     },
-    total=False,
 )
 
 FleetCapacityReservationTypeDef = TypedDict(
     "FleetCapacityReservationTypeDef",
     {
         "CapacityReservationId": str,
         "AvailabilityZoneId": str,
@@ -4191,24 +4151,22 @@
         "TotalInstanceCount": int,
         "FulfilledCapacity": float,
         "EbsOptimized": bool,
         "CreateDate": datetime,
         "Weight": float,
         "Priority": int,
     },
-    total=False,
 )
 
 CapacityReservationGroupTypeDef = TypedDict(
     "CapacityReservationGroupTypeDef",
     {
         "GroupArn": str,
         "OwnerId": str,
     },
-    total=False,
 )
 
 CapacityReservationOptionsRequestTypeDef = TypedDict(
     "CapacityReservationOptionsRequestTypeDef",
     {
         "UsageStrategy": Literal["use-capacity-reservations-first"],
     },
@@ -4216,24 +4174,22 @@
 )
 
 CapacityReservationOptionsTypeDef = TypedDict(
     "CapacityReservationOptionsTypeDef",
     {
         "UsageStrategy": Literal["use-capacity-reservations-first"],
     },
-    total=False,
 )
 
 CapacityReservationTargetResponseTypeDef = TypedDict(
     "CapacityReservationTargetResponseTypeDef",
     {
         "CapacityReservationId": str,
         "CapacityReservationResourceGroupArn": str,
     },
-    total=False,
 )
 
 CapacityReservationTargetTypeDef = TypedDict(
     "CapacityReservationTargetTypeDef",
     {
         "CapacityReservationId": str,
         "CapacityReservationResourceGroupArn": str,
@@ -4250,15 +4206,14 @@
 )
 
 CertificateAuthenticationTypeDef = TypedDict(
     "CertificateAuthenticationTypeDef",
     {
         "ClientRootCertificateChain": str,
     },
-    total=False,
 )
 
 CidrAuthorizationContextTypeDef = TypedDict(
     "CidrAuthorizationContextTypeDef",
     {
         "Message": str,
         "Signature": str,
@@ -4266,50 +4221,45 @@
 )
 
 CidrBlockTypeDef = TypedDict(
     "CidrBlockTypeDef",
     {
         "CidrBlock": str,
     },
-    total=False,
 )
 
 ClassicLinkDnsSupportTypeDef = TypedDict(
     "ClassicLinkDnsSupportTypeDef",
     {
         "ClassicLinkDnsSupported": bool,
         "VpcId": str,
     },
-    total=False,
 )
 
 GroupIdentifierTypeDef = TypedDict(
     "GroupIdentifierTypeDef",
     {
         "GroupName": str,
         "GroupId": str,
     },
-    total=False,
 )
 
 ClassicLoadBalancerTypeDef = TypedDict(
     "ClassicLoadBalancerTypeDef",
     {
         "Name": str,
     },
-    total=False,
 )
 
 ClientCertificateRevocationListStatusTypeDef = TypedDict(
     "ClientCertificateRevocationListStatusTypeDef",
     {
         "Code": ClientCertificateRevocationListStatusCodeType,
         "Message": str,
     },
-    total=False,
 )
 
 ClientConnectOptionsTypeDef = TypedDict(
     "ClientConnectOptionsTypeDef",
     {
         "Enabled": bool,
         "LambdaFunctionArn": str,
@@ -4319,15 +4269,14 @@
 
 ClientVpnEndpointAttributeStatusTypeDef = TypedDict(
     "ClientVpnEndpointAttributeStatusTypeDef",
     {
         "Code": ClientVpnEndpointAttributeStatusCodeType,
         "Message": str,
     },
-    total=False,
 )
 
 ClientDataTypeDef = TypedDict(
     "ClientDataTypeDef",
     {
         "Comment": str,
         "UploadEnd": Union[datetime, str],
@@ -4348,15 +4297,14 @@
 
 ClientLoginBannerResponseOptionsTypeDef = TypedDict(
     "ClientLoginBannerResponseOptionsTypeDef",
     {
         "Enabled": bool,
         "BannerText": str,
     },
-    total=False,
 )
 
 DirectoryServiceAuthenticationRequestTypeDef = TypedDict(
     "DirectoryServiceAuthenticationRequestTypeDef",
     {
         "DirectoryId": str,
     },
@@ -4373,61 +4321,55 @@
 )
 
 DirectoryServiceAuthenticationTypeDef = TypedDict(
     "DirectoryServiceAuthenticationTypeDef",
     {
         "DirectoryId": str,
     },
-    total=False,
 )
 
 FederatedAuthenticationTypeDef = TypedDict(
     "FederatedAuthenticationTypeDef",
     {
         "SamlProviderArn": str,
         "SelfServiceSamlProviderArn": str,
     },
-    total=False,
 )
 
 ClientVpnConnectionStatusTypeDef = TypedDict(
     "ClientVpnConnectionStatusTypeDef",
     {
         "Code": ClientVpnConnectionStatusCodeType,
         "Message": str,
     },
-    total=False,
 )
 
 ClientVpnEndpointStatusTypeDef = TypedDict(
     "ClientVpnEndpointStatusTypeDef",
     {
         "Code": ClientVpnEndpointStatusCodeType,
         "Message": str,
     },
-    total=False,
 )
 
 ConnectionLogResponseOptionsTypeDef = TypedDict(
     "ConnectionLogResponseOptionsTypeDef",
     {
         "Enabled": bool,
         "CloudwatchLogGroup": str,
         "CloudwatchLogStream": str,
     },
-    total=False,
 )
 
 ClientVpnRouteStatusTypeDef = TypedDict(
     "ClientVpnRouteStatusTypeDef",
     {
         "Code": ClientVpnRouteStatusCodeType,
         "Message": str,
     },
-    total=False,
 )
 
 CloudWatchLogOptionsSpecificationTypeDef = TypedDict(
     "CloudWatchLogOptionsSpecificationTypeDef",
     {
         "LogEnabled": bool,
         "LogGroupArn": str,
@@ -4439,36 +4381,33 @@
 CloudWatchLogOptionsTypeDef = TypedDict(
     "CloudWatchLogOptionsTypeDef",
     {
         "LogEnabled": bool,
         "LogGroupArn": str,
         "LogOutputFormat": str,
     },
-    total=False,
 )
 
 CoipAddressUsageTypeDef = TypedDict(
     "CoipAddressUsageTypeDef",
     {
         "AllocationId": str,
         "AwsAccountId": str,
         "AwsService": str,
         "CoIp": str,
     },
-    total=False,
 )
 
 CoipCidrTypeDef = TypedDict(
     "CoipCidrTypeDef",
     {
         "Cidr": str,
         "CoipPoolId": str,
         "LocalGatewayRouteTableId": str,
     },
-    total=False,
 )
 
 _RequiredConfirmProductInstanceRequestRequestTypeDef = TypedDict(
     "_RequiredConfirmProductInstanceRequestRequestTypeDef",
     {
         "InstanceId": str,
         "ProductCode": str,
@@ -4516,15 +4455,14 @@
         "ServiceId": str,
         "VpcEndpointId": str,
         "ConnectionNotificationType": Literal["Topic"],
         "ConnectionNotificationArn": str,
         "ConnectionEvents": List[str],
         "ConnectionNotificationState": ConnectionNotificationStateType,
     },
-    total=False,
 )
 
 _RequiredCopyFpgaImageRequestRequestTypeDef = TypedDict(
     "_RequiredCopyFpgaImageRequestRequestTypeDef",
     {
         "SourceFpgaImageId": str,
         "SourceRegion": str,
@@ -4616,15 +4554,14 @@
 CpuOptionsTypeDef = TypedDict(
     "CpuOptionsTypeDef",
     {
         "CoreCount": int,
         "ThreadsPerCore": int,
         "AmdSevSnp": AmdSevSnpSpecificationType,
     },
-    total=False,
 )
 
 ReservationFleetInstanceSpecificationTypeDef = TypedDict(
     "ReservationFleetInstanceSpecificationTypeDef",
     {
         "InstanceType": InstanceTypeType,
         "InstancePlatform": CapacityReservationInstancePlatformType,
@@ -4854,24 +4791,22 @@
         "LocalGatewayRouteTableArn": str,
         "OwnerId": str,
         "SubnetId": str,
         "CoipPoolId": str,
         "NetworkInterfaceId": str,
         "DestinationPrefixListId": str,
     },
-    total=False,
 )
 
 IcmpTypeCodeTypeDef = TypedDict(
     "IcmpTypeCodeTypeDef",
     {
         "Code": int,
         "Type": int,
     },
-    total=False,
 )
 
 _RequiredCreateNetworkInterfacePermissionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateNetworkInterfacePermissionRequestRequestTypeDef",
     {
         "NetworkInterfaceId": str,
         "Permission": InterfacePermissionTypeType,
@@ -4896,15 +4831,14 @@
 
 
 InstanceIpv6AddressTypeDef = TypedDict(
     "InstanceIpv6AddressTypeDef",
     {
         "Ipv6Address": str,
     },
-    total=False,
 )
 
 Ipv4PrefixSpecificationRequestTypeDef = TypedDict(
     "Ipv4PrefixSpecificationRequestTypeDef",
     {
         "Ipv4Prefix": str,
     },
@@ -5243,15 +5177,14 @@
 
 CreateVolumePermissionTypeDef = TypedDict(
     "CreateVolumePermissionTypeDef",
     {
         "Group": Literal["all"],
         "UserId": str,
     },
-    total=False,
 )
 
 _RequiredCreateVpcEndpointConnectionNotificationRequestRequestTypeDef = TypedDict(
     "_RequiredCreateVpcEndpointConnectionNotificationRequestRequestTypeDef",
     {
         "ConnectionNotificationArn": str,
         "ConnectionEvents": Sequence[str],
@@ -5301,15 +5234,14 @@
 )
 
 CreditSpecificationTypeDef = TypedDict(
     "CreditSpecificationTypeDef",
     {
         "CpuCredits": str,
     },
-    total=False,
 )
 
 DataQueryTypeDef = TypedDict(
     "DataQueryTypeDef",
     {
         "Id": str,
         "Source": str,
@@ -5325,15 +5257,14 @@
     "MetricPointTypeDef",
     {
         "StartDate": datetime,
         "EndDate": datetime,
         "Value": float,
         "Status": str,
     },
-    total=False,
 )
 
 _RequiredDeleteCarrierGatewayRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteCarrierGatewayRequestRequestTypeDef",
     {
         "CarrierGatewayId": str,
     },
@@ -5526,25 +5457,23 @@
 
 DeleteFleetErrorTypeDef = TypedDict(
     "DeleteFleetErrorTypeDef",
     {
         "Code": DeleteFleetErrorCodeType,
         "Message": str,
     },
-    total=False,
 )
 
 DeleteFleetSuccessItemTypeDef = TypedDict(
     "DeleteFleetSuccessItemTypeDef",
     {
         "CurrentFleetState": FleetStateCodeType,
         "PreviousFleetState": FleetStateCodeType,
         "FleetId": str,
     },
-    total=False,
 )
 
 _RequiredDeleteFleetsRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteFleetsRequestRequestTypeDef",
     {
         "FleetIds": Sequence[str],
         "TerminateInstances": bool,
@@ -5662,15 +5591,14 @@
 
 InstanceEventWindowStateChangeTypeDef = TypedDict(
     "InstanceEventWindowStateChangeTypeDef",
     {
         "InstanceEventWindowId": str,
         "State": InstanceEventWindowStateType,
     },
-    total=False,
 )
 
 DeleteInternetGatewayRequestInternetGatewayDeleteTypeDef = TypedDict(
     "DeleteInternetGatewayRequestInternetGatewayDeleteTypeDef",
     {
         "DryRun": bool,
     },
@@ -5849,25 +5777,23 @@
 
 ResponseErrorTypeDef = TypedDict(
     "ResponseErrorTypeDef",
     {
         "Code": LaunchTemplateErrorCodeType,
         "Message": str,
     },
-    total=False,
 )
 
 DeleteLaunchTemplateVersionsResponseSuccessItemTypeDef = TypedDict(
     "DeleteLaunchTemplateVersionsResponseSuccessItemTypeDef",
     {
         "LaunchTemplateId": str,
         "LaunchTemplateName": str,
         "VersionNumber": int,
     },
-    total=False,
 )
 
 _RequiredDeleteLocalGatewayRouteRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteLocalGatewayRouteRequestRequestTypeDef",
     {
         "LocalGatewayRouteTableId": str,
     },
@@ -6326,15 +6252,14 @@
 
 DeleteQueuedReservedInstancesErrorTypeDef = TypedDict(
     "DeleteQueuedReservedInstancesErrorTypeDef",
     {
         "Code": DeleteQueuedReservedInstancesErrorCodeType,
         "Message": str,
     },
-    total=False,
 )
 
 _RequiredDeleteQueuedReservedInstancesRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteQueuedReservedInstancesRequestRequestTypeDef",
     {
         "ReservedInstancesIds": Sequence[str],
     },
@@ -6356,15 +6281,14 @@
 
 
 SuccessfulQueuedPurchaseDeletionTypeDef = TypedDict(
     "SuccessfulQueuedPurchaseDeletionTypeDef",
     {
         "ReservedInstancesId": str,
     },
-    total=False,
 )
 
 _RequiredDeleteRouteRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteRouteRequestRequestTypeDef",
     {
         "RouteTableId": str,
     },
@@ -7327,15 +7251,14 @@
 
 InstanceTagNotificationAttributeTypeDef = TypedDict(
     "InstanceTagNotificationAttributeTypeDef",
     {
         "InstanceTagKeys": List[str],
         "IncludeAllTagsOfInstance": bool,
     },
-    total=False,
 )
 
 DeregisterTransitGatewayMulticastGroupMembersRequestRequestTypeDef = TypedDict(
     "DeregisterTransitGatewayMulticastGroupMembersRequestRequestTypeDef",
     {
         "TransitGatewayMulticastDomainId": str,
         "GroupIpAddress": str,
@@ -7348,15 +7271,14 @@
 TransitGatewayMulticastDeregisteredGroupMembersTypeDef = TypedDict(
     "TransitGatewayMulticastDeregisteredGroupMembersTypeDef",
     {
         "TransitGatewayMulticastDomainId": str,
         "DeregisteredNetworkInterfaceIds": List[str],
         "GroupIpAddress": str,
     },
-    total=False,
 )
 
 DeregisterTransitGatewayMulticastGroupSourcesRequestRequestTypeDef = TypedDict(
     "DeregisterTransitGatewayMulticastGroupSourcesRequestRequestTypeDef",
     {
         "TransitGatewayMulticastDomainId": str,
         "GroupIpAddress": str,
@@ -7369,15 +7291,14 @@
 TransitGatewayMulticastDeregisteredGroupSourcesTypeDef = TypedDict(
     "TransitGatewayMulticastDeregisteredGroupSourcesTypeDef",
     {
         "TransitGatewayMulticastDomainId": str,
         "DeregisteredNetworkInterfaceIds": List[str],
         "GroupIpAddress": str,
     },
-    total=False,
 )
 
 DescribeAccountAttributesRequestRequestTypeDef = TypedDict(
     "DescribeAccountAttributesRequestRequestTypeDef",
     {
         "AttributeNames": Sequence[AccountAttributeNameType],
         "DryRun": bool,
@@ -7449,27 +7370,25 @@
 IdFormatTypeDef = TypedDict(
     "IdFormatTypeDef",
     {
         "Deadline": datetime,
         "Resource": str,
         "UseLongIds": bool,
     },
-    total=False,
 )
 
 SubscriptionTypeDef = TypedDict(
     "SubscriptionTypeDef",
     {
         "Source": str,
         "Destination": str,
         "Metric": Literal["aggregate-latency"],
         "Statistic": Literal["p50"],
         "Period": PeriodTypeType,
     },
-    total=False,
 )
 
 WaiterConfigTypeDef = TypedDict(
     "WaiterConfigTypeDef",
     {
         "Delay": int,
         "MaxAttempts": int,
@@ -7521,23 +7440,21 @@
 FastLaunchLaunchTemplateSpecificationResponseTypeDef = TypedDict(
     "FastLaunchLaunchTemplateSpecificationResponseTypeDef",
     {
         "LaunchTemplateId": str,
         "LaunchTemplateName": str,
         "Version": str,
     },
-    total=False,
 )
 
 FastLaunchSnapshotConfigurationResponseTypeDef = TypedDict(
     "FastLaunchSnapshotConfigurationResponseTypeDef",
     {
         "TargetResourceCount": int,
     },
-    total=False,
 )
 
 DescribeFastSnapshotRestoreSuccessItemTypeDef = TypedDict(
     "DescribeFastSnapshotRestoreSuccessItemTypeDef",
     {
         "SnapshotId": str,
         "AvailabilityZone": str,
@@ -7547,15 +7464,14 @@
         "OwnerAlias": str,
         "EnablingTime": datetime,
         "OptimizingTime": datetime,
         "EnabledTime": datetime,
         "DisablingTime": datetime,
         "DisabledTime": datetime,
     },
-    total=False,
 )
 
 _RequiredDescribeFleetHistoryRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeFleetHistoryRequestRequestTypeDef",
     {
         "FleetId": str,
         "StartTime": Union[datetime, str],
@@ -7610,15 +7526,14 @@
         "Duration": int,
         "HourlyPrice": str,
         "InstanceFamily": str,
         "OfferingId": str,
         "PaymentOption": PaymentOptionType,
         "UpfrontPrice": str,
     },
-    total=False,
 )
 
 DescribeIdFormatRequestRequestTypeDef = TypedDict(
     "DescribeIdFormatRequestRequestTypeDef",
     {
         "Resource": str,
     },
@@ -7739,15 +7654,14 @@
 
 InstanceCreditSpecificationTypeDef = TypedDict(
     "InstanceCreditSpecificationTypeDef",
     {
         "InstanceId": str,
         "CpuCredits": str,
     },
-    total=False,
 )
 
 DescribeInstanceEventNotificationAttributesRequestRequestTypeDef = TypedDict(
     "DescribeInstanceEventNotificationAttributesRequestRequestTypeDef",
     {
         "DryRun": bool,
     },
@@ -7757,24 +7671,22 @@
 InstanceTypeOfferingTypeDef = TypedDict(
     "InstanceTypeOfferingTypeDef",
     {
         "InstanceType": InstanceTypeType,
         "LocationType": LocationTypeType,
         "Location": str,
     },
-    total=False,
 )
 
 MovingAddressStatusTypeDef = TypedDict(
     "MovingAddressStatusTypeDef",
     {
         "MoveStatus": MoveStatusType,
         "PublicIp": str,
     },
-    total=False,
 )
 
 DescribeNetworkInterfaceAttributeRequestNetworkInterfaceDescribeAttributeTypeDef = TypedDict(
     "DescribeNetworkInterfaceAttributeRequestNetworkInterfaceDescribeAttributeTypeDef",
     {
         "Attribute": NetworkInterfaceAttributeType,
         "DryRun": bool,
@@ -7808,15 +7720,14 @@
 PrefixListTypeDef = TypedDict(
     "PrefixListTypeDef",
     {
         "Cidrs": List[str],
         "PrefixListId": str,
         "PrefixListName": str,
     },
-    total=False,
 )
 
 DescribePrincipalIdFormatRequestDescribePrincipalIdFormatPaginateTypeDef = TypedDict(
     "DescribePrincipalIdFormatRequestDescribePrincipalIdFormatPaginateTypeDef",
     {
         "DryRun": bool,
         "Resources": Sequence[str],
@@ -7839,15 +7750,14 @@
 RegionTypeDef = TypedDict(
     "RegionTypeDef",
     {
         "Endpoint": str,
         "RegionName": str,
         "OptInStatus": str,
     },
-    total=False,
 )
 
 ScheduledInstanceRecurrenceRequestTypeDef = TypedDict(
     "ScheduledInstanceRecurrenceRequestTypeDef",
     {
         "Frequency": str,
         "Interval": int,
@@ -7900,15 +7810,14 @@
 SecurityGroupReferenceTypeDef = TypedDict(
     "SecurityGroupReferenceTypeDef",
     {
         "GroupId": str,
         "ReferencingVpcId": str,
         "VpcPeeringConnectionId": str,
     },
-    total=False,
 )
 
 _RequiredDescribeSnapshotAttributeRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeSnapshotAttributeRequestRequestTypeDef",
     {
         "Attribute": SnapshotAttributeNameType,
         "SnapshotId": str,
@@ -7954,15 +7863,14 @@
 
 ProductCodeTypeDef = TypedDict(
     "ProductCodeTypeDef",
     {
         "ProductCodeId": str,
         "ProductCodeType": ProductCodeValuesType,
     },
-    total=False,
 )
 
 DescribeSpotDatafeedSubscriptionRequestRequestTypeDef = TypedDict(
     "DescribeSpotDatafeedSubscriptionRequestRequestTypeDef",
     {
         "DryRun": bool,
     },
@@ -8068,15 +7976,14 @@
     {
         "AvailabilityZone": str,
         "InstanceType": InstanceTypeType,
         "ProductDescription": RIProductDescriptionType,
         "SpotPrice": str,
         "Timestamp": datetime,
     },
-    total=False,
 )
 
 _RequiredDescribeStaleSecurityGroupsRequestDescribeStaleSecurityGroupsPaginateTypeDef = TypedDict(
     "_RequiredDescribeStaleSecurityGroupsRequestDescribeStaleSecurityGroupsPaginateTypeDef",
     {
         "VpcId": str,
     },
@@ -8129,26 +8036,24 @@
         "TaskStartTime": datetime,
         "Bucket": str,
         "S3objectKey": str,
         "ProgressPercentage": int,
         "StoreTaskState": str,
         "StoreTaskFailureReason": str,
     },
-    total=False,
 )
 
 TagDescriptionTypeDef = TypedDict(
     "TagDescriptionTypeDef",
     {
         "Key": str,
         "ResourceId": str,
         "ResourceType": ResourceTypeType,
         "Value": str,
     },
-    total=False,
 )
 
 _RequiredDescribeVolumeAttributeRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeVolumeAttributeRequestRequestTypeDef",
     {
         "Attribute": VolumeAttributeNameType,
         "VolumeId": str,
@@ -8208,15 +8113,14 @@
         "OriginalVolumeType": VolumeTypeType,
         "OriginalThroughput": int,
         "OriginalMultiAttachEnabled": bool,
         "Progress": int,
         "StartTime": datetime,
         "EndTime": datetime,
     },
-    total=False,
 )
 
 _RequiredDescribeVpcAttributeRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeVpcAttributeRequestRequestTypeDef",
     {
         "Attribute": VpcAttributeNameType,
         "VpcId": str,
@@ -8282,15 +8186,14 @@
 DestinationOptionsResponseTypeDef = TypedDict(
     "DestinationOptionsResponseTypeDef",
     {
         "FileFormat": DestinationFileFormatType,
         "HiveCompatiblePartitions": bool,
         "PerHourPartition": bool,
     },
-    total=False,
 )
 
 _RequiredDetachClassicLinkVpcRequestInstanceDetachClassicLinkVpcTypeDef = TypedDict(
     "_RequiredDetachClassicLinkVpcRequestInstanceDetachClassicLinkVpcTypeDef",
     {
         "VpcId": str,
     },
@@ -8583,15 +8486,14 @@
 
 
 DeviceOptionsTypeDef = TypedDict(
     "DeviceOptionsTypeDef",
     {
         "TenantId": str,
     },
-    total=False,
 )
 
 _RequiredDisableAddressTransferRequestRequestTypeDef = TypedDict(
     "_RequiredDisableAddressTransferRequestRequestTypeDef",
     {
         "AllocationId": str,
     },
@@ -8672,15 +8574,14 @@
 
 DisableFastSnapshotRestoreStateErrorTypeDef = TypedDict(
     "DisableFastSnapshotRestoreStateErrorTypeDef",
     {
         "Code": str,
         "Message": str,
     },
-    total=False,
 )
 
 DisableFastSnapshotRestoreSuccessItemTypeDef = TypedDict(
     "DisableFastSnapshotRestoreSuccessItemTypeDef",
     {
         "SnapshotId": str,
         "AvailabilityZone": str,
@@ -8690,15 +8591,14 @@
         "OwnerAlias": str,
         "EnablingTime": datetime,
         "OptimizingTime": datetime,
         "EnabledTime": datetime,
         "DisablingTime": datetime,
         "DisabledTime": datetime,
     },
-    total=False,
 )
 
 _RequiredDisableFastSnapshotRestoresRequestRequestTypeDef = TypedDict(
     "_RequiredDisableFastSnapshotRestoresRequestRequestTypeDef",
     {
         "AvailabilityZones": Sequence[str],
         "SourceSnapshotIds": Sequence[str],
@@ -8826,15 +8726,14 @@
         "TransitGatewayAttachmentId": str,
         "ResourceId": str,
         "ResourceType": TransitGatewayAttachmentResourceTypeType,
         "TransitGatewayRouteTableId": str,
         "State": TransitGatewayPropagationStateType,
         "TransitGatewayRouteTableAnnouncementId": str,
     },
-    total=False,
 )
 
 _RequiredDisableVgwRoutePropagationRequestRequestTypeDef = TypedDict(
     "_RequiredDisableVgwRoutePropagationRequestRequestTypeDef",
     {
         "GatewayId": str,
         "RouteTableId": str,
@@ -9218,15 +9117,14 @@
     "DiskImageDescriptionTypeDef",
     {
         "Checksum": str,
         "Format": DiskImageFormatType,
         "ImportManifestUrl": str,
         "Size": int,
     },
-    total=False,
 )
 
 DiskImageDetailTypeDef = TypedDict(
     "DiskImageDetailTypeDef",
     {
         "Bytes": int,
         "Format": DiskImageFormatType,
@@ -9243,43 +9141,39 @@
 
 DiskImageVolumeDescriptionTypeDef = TypedDict(
     "DiskImageVolumeDescriptionTypeDef",
     {
         "Id": str,
         "Size": int,
     },
-    total=False,
 )
 
 DiskInfoTypeDef = TypedDict(
     "DiskInfoTypeDef",
     {
         "SizeInGB": int,
         "Count": int,
         "Type": DiskTypeType,
     },
-    total=False,
 )
 
 DnsEntryTypeDef = TypedDict(
     "DnsEntryTypeDef",
     {
         "DnsName": str,
         "HostedZoneId": str,
     },
-    total=False,
 )
 
 DnsOptionsTypeDef = TypedDict(
     "DnsOptionsTypeDef",
     {
         "DnsRecordIpType": DnsRecordIpTypeType,
         "PrivateDnsOnlyForInboundResolverEndpoint": bool,
     },
-    total=False,
 )
 
 DnsServersOptionsModifyStructureTypeDef = TypedDict(
     "DnsServersOptionsModifyStructureTypeDef",
     {
         "CustomDnsServers": Sequence[str],
         "Enabled": bool,
@@ -9293,15 +9187,14 @@
         "BaselineBandwidthInMbps": int,
         "BaselineThroughputInMBps": float,
         "BaselineIops": int,
         "MaximumBandwidthInMbps": int,
         "MaximumThroughputInMBps": float,
         "MaximumIops": int,
     },
-    total=False,
 )
 
 EbsInstanceBlockDeviceSpecificationTypeDef = TypedDict(
     "EbsInstanceBlockDeviceSpecificationTypeDef",
     {
         "DeleteOnTermination": bool,
         "VolumeId": str,
@@ -9313,59 +9206,53 @@
     "EbsInstanceBlockDeviceTypeDef",
     {
         "AttachTime": datetime,
         "DeleteOnTermination": bool,
         "Status": AttachmentStatusType,
         "VolumeId": str,
     },
-    total=False,
 )
 
 EfaInfoTypeDef = TypedDict(
     "EfaInfoTypeDef",
     {
         "MaximumEfaInterfaces": int,
     },
-    total=False,
 )
 
 InternetGatewayAttachmentTypeDef = TypedDict(
     "InternetGatewayAttachmentTypeDef",
     {
         "State": AttachmentStatusType,
         "VpcId": str,
     },
-    total=False,
 )
 
 ElasticGpuAssociationTypeDef = TypedDict(
     "ElasticGpuAssociationTypeDef",
     {
         "ElasticGpuId": str,
         "ElasticGpuAssociationId": str,
         "ElasticGpuAssociationState": str,
         "ElasticGpuAssociationTime": str,
     },
-    total=False,
 )
 
 ElasticGpuHealthTypeDef = TypedDict(
     "ElasticGpuHealthTypeDef",
     {
         "Status": ElasticGpuStatusType,
     },
-    total=False,
 )
 
 ElasticGpuSpecificationResponseTypeDef = TypedDict(
     "ElasticGpuSpecificationResponseTypeDef",
     {
         "Type": str,
     },
-    total=False,
 )
 
 ElasticGpuSpecificationTypeDef = TypedDict(
     "ElasticGpuSpecificationTypeDef",
     {
         "Type": str,
     },
@@ -9375,15 +9262,14 @@
     "ElasticInferenceAcceleratorAssociationTypeDef",
     {
         "ElasticInferenceAcceleratorArn": str,
         "ElasticInferenceAcceleratorAssociationId": str,
         "ElasticInferenceAcceleratorAssociationState": str,
         "ElasticInferenceAcceleratorAssociationTime": datetime,
     },
-    total=False,
 )
 
 _RequiredElasticInferenceAcceleratorTypeDef = TypedDict(
     "_RequiredElasticInferenceAcceleratorTypeDef",
     {
         "Type": str,
     },
@@ -9510,15 +9396,14 @@
 
 EnableFastSnapshotRestoreStateErrorTypeDef = TypedDict(
     "EnableFastSnapshotRestoreStateErrorTypeDef",
     {
         "Code": str,
         "Message": str,
     },
-    total=False,
 )
 
 EnableFastSnapshotRestoreSuccessItemTypeDef = TypedDict(
     "EnableFastSnapshotRestoreSuccessItemTypeDef",
     {
         "SnapshotId": str,
         "AvailabilityZone": str,
@@ -9528,15 +9413,14 @@
         "OwnerAlias": str,
         "EnablingTime": datetime,
         "OptimizingTime": datetime,
         "EnabledTime": datetime,
         "DisablingTime": datetime,
         "DisabledTime": datetime,
     },
-    total=False,
 )
 
 _RequiredEnableFastSnapshotRestoresRequestRequestTypeDef = TypedDict(
     "_RequiredEnableFastSnapshotRestoresRequestRequestTypeDef",
     {
         "AvailabilityZones": Sequence[str],
         "SourceSnapshotIds": Sequence[str],
@@ -9798,39 +9682,36 @@
 )
 
 EnclaveOptionsTypeDef = TypedDict(
     "EnclaveOptionsTypeDef",
     {
         "Enabled": bool,
     },
-    total=False,
 )
 
 EventInformationTypeDef = TypedDict(
     "EventInformationTypeDef",
     {
         "EventDescription": str,
         "EventSubType": str,
         "InstanceId": str,
     },
-    total=False,
 )
 
 TransitGatewayRouteTableRouteTypeDef = TypedDict(
     "TransitGatewayRouteTableRouteTypeDef",
     {
         "DestinationCidr": str,
         "State": str,
         "RouteOrigin": str,
         "PrefixListId": str,
         "AttachmentId": str,
         "ResourceId": str,
         "ResourceType": str,
     },
-    total=False,
 )
 
 _RequiredExportClientVpnClientCertificateRevocationListRequestRequestTypeDef = TypedDict(
     "_RequiredExportClientVpnClientCertificateRevocationListRequestRequestTypeDef",
     {
         "ClientVpnEndpointId": str,
     },
@@ -9904,35 +9785,32 @@
 
 ExportTaskS3LocationTypeDef = TypedDict(
     "ExportTaskS3LocationTypeDef",
     {
         "S3Bucket": str,
         "S3Prefix": str,
     },
-    total=False,
 )
 
 ExportToS3TaskTypeDef = TypedDict(
     "ExportToS3TaskTypeDef",
     {
         "ContainerFormat": Literal["ova"],
         "DiskImageFormat": DiskImageFormatType,
         "S3Bucket": str,
         "S3Key": str,
     },
-    total=False,
 )
 
 InstanceExportDetailsTypeDef = TypedDict(
     "InstanceExportDetailsTypeDef",
     {
         "InstanceId": str,
         "TargetEnvironment": ExportEnvironmentType,
     },
-    total=False,
 )
 
 ExportTransitGatewayRoutesResultTypeDef = TypedDict(
     "ExportTransitGatewayRoutesResultTypeDef",
     {
         "S3Location": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
@@ -9941,27 +9819,25 @@
 
 FilterPortRangeTypeDef = TypedDict(
     "FilterPortRangeTypeDef",
     {
         "FromPort": int,
         "ToPort": int,
     },
-    total=False,
 )
 
 TargetCapacitySpecificationTypeDef = TypedDict(
     "TargetCapacitySpecificationTypeDef",
     {
         "TotalTargetCapacity": int,
         "OnDemandTargetCapacity": int,
         "SpotTargetCapacity": int,
         "DefaultTargetCapacityType": DefaultTargetCapacityTypeType,
         "TargetCapacityUnitType": TargetCapacityUnitTypeType,
     },
-    total=False,
 )
 
 FleetLaunchTemplateSpecificationRequestTypeDef = TypedDict(
     "FleetLaunchTemplateSpecificationRequestTypeDef",
     {
         "LaunchTemplateId": str,
         "LaunchTemplateName": str,
@@ -9973,15 +9849,14 @@
 FleetLaunchTemplateSpecificationTypeDef = TypedDict(
     "FleetLaunchTemplateSpecificationTypeDef",
     {
         "LaunchTemplateId": str,
         "LaunchTemplateName": str,
         "Version": str,
     },
-    total=False,
 )
 
 PlacementTypeDef = TypedDict(
     "PlacementTypeDef",
     {
         "AvailabilityZone": str,
         "Affinity": str,
@@ -9997,15 +9872,14 @@
 )
 
 PlacementResponseTypeDef = TypedDict(
     "PlacementResponseTypeDef",
     {
         "GroupName": str,
     },
-    total=False,
 )
 
 FleetSpotCapacityRebalanceRequestTypeDef = TypedDict(
     "FleetSpotCapacityRebalanceRequestTypeDef",
     {
         "ReplacementStrategy": FleetReplacementStrategyType,
         "TerminationDelay": int,
@@ -10015,52 +9889,47 @@
 
 FleetSpotCapacityRebalanceTypeDef = TypedDict(
     "FleetSpotCapacityRebalanceTypeDef",
     {
         "ReplacementStrategy": FleetReplacementStrategyType,
         "TerminationDelay": int,
     },
-    total=False,
 )
 
 FpgaDeviceMemoryInfoTypeDef = TypedDict(
     "FpgaDeviceMemoryInfoTypeDef",
     {
         "SizeInMiB": int,
     },
-    total=False,
 )
 
 LoadPermissionTypeDef = TypedDict(
     "LoadPermissionTypeDef",
     {
         "UserId": str,
         "Group": Literal["all"],
     },
-    total=False,
 )
 
 FpgaImageStateTypeDef = TypedDict(
     "FpgaImageStateTypeDef",
     {
         "Code": FpgaImageStateCodeType,
         "Message": str,
     },
-    total=False,
 )
 
 PciIdTypeDef = TypedDict(
     "PciIdTypeDef",
     {
         "DeviceId": str,
         "VendorId": str,
         "SubsystemId": str,
         "SubsystemVendorId": str,
     },
-    total=False,
 )
 
 _RequiredGetAssociatedEnclaveCertificateIamRolesRequestRequestTypeDef = TypedDict(
     "_RequiredGetAssociatedEnclaveCertificateIamRolesRequestRequestTypeDef",
     {
         "CertificateArn": str,
     },
@@ -10130,15 +9999,14 @@
 
 Ipv6CidrAssociationTypeDef = TypedDict(
     "Ipv6CidrAssociationTypeDef",
     {
         "Ipv6Cidr": str,
         "AssociatedResource": str,
     },
-    total=False,
 )
 
 _RequiredGetCapacityReservationUsageRequestRequestTypeDef = TypedDict(
     "_RequiredGetCapacityReservationUsageRequestRequestTypeDef",
     {
         "CapacityReservationId": str,
     },
@@ -10163,15 +10031,14 @@
 
 InstanceUsageTypeDef = TypedDict(
     "InstanceUsageTypeDef",
     {
         "AccountId": str,
         "UsedInstanceCount": int,
     },
-    total=False,
 )
 
 GetConsoleOutputRequestInstanceConsoleOutputTypeDef = TypedDict(
     "GetConsoleOutputRequestInstanceConsoleOutputTypeDef",
     {
         "DryRun": bool,
         "Latest": bool,
@@ -10267,15 +10134,14 @@
 
 InstanceFamilyCreditSpecificationTypeDef = TypedDict(
     "InstanceFamilyCreditSpecificationTypeDef",
     {
         "InstanceFamily": UnlimitedSupportedInstanceFamilyType,
         "CpuCredits": str,
     },
-    total=False,
 )
 
 GetEbsDefaultKmsKeyIdRequestRequestTypeDef = TypedDict(
     "GetEbsDefaultKmsKeyIdRequestRequestTypeDef",
     {
         "DryRun": bool,
     },
@@ -10377,23 +10243,21 @@
         "HostIdSet": List[str],
         "HostReservationId": str,
         "HourlyPrice": str,
         "InstanceFamily": str,
         "PaymentOption": PaymentOptionType,
         "UpfrontPrice": str,
     },
-    total=False,
 )
 
 InstanceTypeInfoFromInstanceRequirementsTypeDef = TypedDict(
     "InstanceTypeInfoFromInstanceRequirementsTypeDef",
     {
         "InstanceType": str,
     },
-    total=False,
 )
 
 _RequiredGetInstanceUefiDataRequestRequestTypeDef = TypedDict(
     "_RequiredGetInstanceUefiDataRequestRequestTypeDef",
     {
         "InstanceId": str,
     },
@@ -10489,15 +10353,14 @@
         "ResourceName": str,
         "ResourceComplianceStatus": IpamComplianceStatusType,
         "ResourceOverlapStatus": IpamOverlapStatusType,
         "VpcId": str,
         "SampledStartTime": datetime,
         "SampledEndTime": datetime,
     },
-    total=False,
 )
 
 _RequiredGetLaunchTemplateDataRequestRequestTypeDef = TypedDict(
     "_RequiredGetLaunchTemplateDataRequestRequestTypeDef",
     {
         "InstanceId": str,
     },
@@ -10567,15 +10430,14 @@
 
 PrefixListAssociationTypeDef = TypedDict(
     "PrefixListAssociationTypeDef",
     {
         "ResourceId": str,
         "ResourceOwner": str,
     },
-    total=False,
 )
 
 _RequiredGetManagedPrefixListEntriesRequestGetManagedPrefixListEntriesPaginateTypeDef = TypedDict(
     "_RequiredGetManagedPrefixListEntriesRequestGetManagedPrefixListEntriesPaginateTypeDef",
     {
         "PrefixListId": str,
     },
@@ -10625,15 +10487,14 @@
 
 PrefixListEntryTypeDef = TypedDict(
     "PrefixListEntryTypeDef",
     {
         "Cidr": str,
         "Description": str,
     },
-    total=False,
 )
 
 _RequiredGetNetworkInsightsAccessScopeAnalysisFindingsRequestGetNetworkInsightsAccessScopeAnalysisFindingsPaginateTypeDef = TypedDict(
     "_RequiredGetNetworkInsightsAccessScopeAnalysisFindingsRequestGetNetworkInsightsAccessScopeAnalysisFindingsPaginateTypeDef",
     {
         "NetworkInsightsAccessScopeAnalysisId": str,
     },
@@ -10743,15 +10604,14 @@
 ReservationValueTypeDef = TypedDict(
     "ReservationValueTypeDef",
     {
         "HourlyPrice": str,
         "RemainingTotalValue": str,
         "RemainingUpfrontValue": str,
     },
-    total=False,
 )
 
 GetSerialConsoleAccessStatusRequestRequestTypeDef = TypedDict(
     "GetSerialConsoleAccessStatusRequestRequestTypeDef",
     {
         "DryRun": bool,
     },
@@ -10769,47 +10629,43 @@
 SpotPlacementScoreTypeDef = TypedDict(
     "SpotPlacementScoreTypeDef",
     {
         "Region": str,
         "AvailabilityZoneId": str,
         "Score": int,
     },
-    total=False,
 )
 
 TransitGatewayAttachmentPropagationTypeDef = TypedDict(
     "TransitGatewayAttachmentPropagationTypeDef",
     {
         "TransitGatewayRouteTableId": str,
         "State": TransitGatewayPropagationStateType,
     },
-    total=False,
 )
 
 TransitGatewayRouteTableAssociationTypeDef = TypedDict(
     "TransitGatewayRouteTableAssociationTypeDef",
     {
         "TransitGatewayAttachmentId": str,
         "ResourceId": str,
         "ResourceType": TransitGatewayAttachmentResourceTypeType,
         "State": TransitGatewayAssociationStateType,
     },
-    total=False,
 )
 
 TransitGatewayRouteTablePropagationTypeDef = TypedDict(
     "TransitGatewayRouteTablePropagationTypeDef",
     {
         "TransitGatewayAttachmentId": str,
         "ResourceId": str,
         "ResourceType": TransitGatewayAttachmentResourceTypeType,
         "State": TransitGatewayPropagationStateType,
         "TransitGatewayRouteTableAnnouncementId": str,
     },
-    total=False,
 )
 
 _RequiredGetVerifiedAccessEndpointPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredGetVerifiedAccessEndpointPolicyRequestRequestTypeDef",
     {
         "VerifiedAccessEndpointId": str,
     },
@@ -10925,15 +10781,14 @@
     "VpnConnectionDeviceTypeTypeDef",
     {
         "VpnConnectionDeviceTypeId": str,
         "Vendor": str,
         "Platform": str,
         "Software": str,
     },
-    total=False,
 )
 
 _RequiredGetVpnTunnelReplacementStatusRequestRequestTypeDef = TypedDict(
     "_RequiredGetVpnTunnelReplacementStatusRequestRequestTypeDef",
     {
         "VpnConnectionId": str,
         "VpnTunnelOutsideIpAddress": str,
@@ -10958,23 +10813,21 @@
 MaintenanceDetailsTypeDef = TypedDict(
     "MaintenanceDetailsTypeDef",
     {
         "PendingMaintenance": str,
         "MaintenanceAutoAppliedAfter": datetime,
         "LastMaintenanceApplied": datetime,
     },
-    total=False,
 )
 
 GpuDeviceMemoryInfoTypeDef = TypedDict(
     "GpuDeviceMemoryInfoTypeDef",
     {
         "SizeInMiB": int,
     },
-    total=False,
 )
 
 HibernationOptionsRequestTypeDef = TypedDict(
     "HibernationOptionsRequestTypeDef",
     {
         "Configured": bool,
     },
@@ -10990,45 +10843,41 @@
 )
 
 HibernationOptionsTypeDef = TypedDict(
     "HibernationOptionsTypeDef",
     {
         "Configured": bool,
     },
-    total=False,
 )
 
 HostInstanceTypeDef = TypedDict(
     "HostInstanceTypeDef",
     {
         "InstanceId": str,
         "InstanceType": str,
         "OwnerId": str,
     },
-    total=False,
 )
 
 HostPropertiesTypeDef = TypedDict(
     "HostPropertiesTypeDef",
     {
         "Cores": int,
         "InstanceType": str,
         "InstanceFamily": str,
         "Sockets": int,
         "TotalVCpus": int,
     },
-    total=False,
 )
 
 IKEVersionsListValueTypeDef = TypedDict(
     "IKEVersionsListValueTypeDef",
     {
         "Value": str,
     },
-    total=False,
 )
 
 IKEVersionsRequestListValueTypeDef = TypedDict(
     "IKEVersionsRequestListValueTypeDef",
     {
         "Value": str,
     },
@@ -11037,15 +10886,14 @@
 
 IamInstanceProfileTypeDef = TypedDict(
     "IamInstanceProfileTypeDef",
     {
         "Arn": str,
         "Id": str,
     },
-    total=False,
 )
 
 IamInstanceProfileResponseMetadataTypeDef = TypedDict(
     "IamInstanceProfileResponseMetadataTypeDef",
     {
         "Arn": str,
         "Id": str,
@@ -11057,15 +10905,14 @@
     "LaunchPermissionTypeDef",
     {
         "Group": Literal["all"],
         "UserId": str,
         "OrganizationArn": str,
         "OrganizationalUnitArn": str,
     },
-    total=False,
 )
 
 UserBucketTypeDef = TypedDict(
     "UserBucketTypeDef",
     {
         "S3Bucket": str,
         "S3Key": str,
@@ -11078,24 +10925,22 @@
     {
         "ImageId": str,
         "Name": str,
         "Description": str,
         "RecycleBinEnterTime": datetime,
         "RecycleBinExitTime": datetime,
     },
-    total=False,
 )
 
 StateReasonTypeDef = TypedDict(
     "StateReasonTypeDef",
     {
         "Code": str,
         "Message": str,
     },
-    total=False,
 )
 
 _RequiredImportClientVpnClientCertificateRevocationListRequestRequestTypeDef = TypedDict(
     "_RequiredImportClientVpnClientCertificateRevocationListRequestRequestTypeDef",
     {
         "ClientVpnEndpointId": str,
         "CertificateRevocationList": str,
@@ -11134,15 +10979,14 @@
 )
 
 ImportImageLicenseConfigurationResponseTypeDef = TypedDict(
     "ImportImageLicenseConfigurationResponseTypeDef",
     {
         "LicenseConfigurationArn": str,
     },
-    total=False,
 )
 
 UserDataTypeDef = TypedDict(
     "UserDataTypeDef",
     {
         "Data": str,
     },
@@ -11152,24 +10996,22 @@
 InferenceDeviceInfoTypeDef = TypedDict(
     "InferenceDeviceInfoTypeDef",
     {
         "Count": int,
         "Name": str,
         "Manufacturer": str,
     },
-    total=False,
 )
 
 InstanceCountTypeDef = TypedDict(
     "InstanceCountTypeDef",
     {
         "InstanceCount": int,
         "State": ListingStateType,
     },
-    total=False,
 )
 
 _RequiredInstanceCreditSpecificationRequestTypeDef = TypedDict(
     "_RequiredInstanceCreditSpecificationRequestTypeDef",
     {
         "InstanceId": str,
     },
@@ -11194,23 +11036,21 @@
     "InstanceEventWindowTimeRangeTypeDef",
     {
         "StartWeekDay": WeekDayType,
         "StartHour": int,
         "EndWeekDay": WeekDayType,
         "EndHour": int,
     },
-    total=False,
 )
 
 InstanceIpv4PrefixTypeDef = TypedDict(
     "InstanceIpv4PrefixTypeDef",
     {
         "Ipv4Prefix": str,
     },
-    total=False,
 )
 
 InstanceIpv6AddressRequestTypeDef = TypedDict(
     "InstanceIpv6AddressRequestTypeDef",
     {
         "Ipv6Address": str,
     },
@@ -11218,15 +11058,14 @@
 )
 
 InstanceIpv6PrefixTypeDef = TypedDict(
     "InstanceIpv6PrefixTypeDef",
     {
         "Ipv6Prefix": str,
     },
-    total=False,
 )
 
 InstanceMaintenanceOptionsRequestTypeDef = TypedDict(
     "InstanceMaintenanceOptionsRequestTypeDef",
     {
         "AutoRecovery": InstanceAutoRecoveryStateType,
     },
@@ -11242,15 +11081,14 @@
 )
 
 InstanceMaintenanceOptionsTypeDef = TypedDict(
     "InstanceMaintenanceOptionsTypeDef",
     {
         "AutoRecovery": InstanceAutoRecoveryStateType,
     },
-    total=False,
 )
 
 SpotMarketOptionsTypeDef = TypedDict(
     "SpotMarketOptionsTypeDef",
     {
         "MaxPrice": str,
         "SpotInstanceType": SpotInstanceTypeType,
@@ -11292,48 +11130,44 @@
         "State": InstanceMetadataOptionsStateType,
         "HttpTokens": HttpTokensStateType,
         "HttpPutResponseHopLimit": int,
         "HttpEndpoint": InstanceMetadataEndpointStateType,
         "HttpProtocolIpv6": InstanceMetadataProtocolStateType,
         "InstanceMetadataTags": InstanceMetadataTagsStateType,
     },
-    total=False,
 )
 
 MonitoringTypeDef = TypedDict(
     "MonitoringTypeDef",
     {
         "State": MonitoringStateType,
     },
-    total=False,
 )
 
 InstanceNetworkInterfaceAssociationTypeDef = TypedDict(
     "InstanceNetworkInterfaceAssociationTypeDef",
     {
         "CarrierIp": str,
         "CustomerOwnedIp": str,
         "IpOwnerId": str,
         "PublicDnsName": str,
         "PublicIp": str,
     },
-    total=False,
 )
 
 InstanceNetworkInterfaceAttachmentTypeDef = TypedDict(
     "InstanceNetworkInterfaceAttachmentTypeDef",
     {
         "AttachTime": datetime,
         "AttachmentId": str,
         "DeleteOnTermination": bool,
         "DeviceIndex": int,
         "Status": AttachmentStatusType,
         "NetworkCardIndex": int,
     },
-    total=False,
 )
 
 MemoryGiBPerVCpuRequestTypeDef = TypedDict(
     "MemoryGiBPerVCpuRequestTypeDef",
     {
         "Min": float,
         "Max": float,
@@ -11410,69 +11244,62 @@
 
 MemoryGiBPerVCpuTypeDef = TypedDict(
     "MemoryGiBPerVCpuTypeDef",
     {
         "Min": float,
         "Max": float,
     },
-    total=False,
 )
 
 MemoryMiBTypeDef = TypedDict(
     "MemoryMiBTypeDef",
     {
         "Min": int,
         "Max": int,
     },
-    total=False,
 )
 
 NetworkBandwidthGbpsTypeDef = TypedDict(
     "NetworkBandwidthGbpsTypeDef",
     {
         "Min": float,
         "Max": float,
     },
-    total=False,
 )
 
 NetworkInterfaceCountTypeDef = TypedDict(
     "NetworkInterfaceCountTypeDef",
     {
         "Min": int,
         "Max": int,
     },
-    total=False,
 )
 
 TotalLocalStorageGBTypeDef = TypedDict(
     "TotalLocalStorageGBTypeDef",
     {
         "Min": float,
         "Max": float,
     },
-    total=False,
 )
 
 VCpuCountRangeTypeDef = TypedDict(
     "VCpuCountRangeTypeDef",
     {
         "Min": int,
         "Max": int,
     },
-    total=False,
 )
 
 InstanceStateTypeDef = TypedDict(
     "InstanceStateTypeDef",
     {
         "Code": int,
         "Name": InstanceStateNameType,
     },
-    total=False,
 )
 
 InstanceStateResponseMetadataTypeDef = TypedDict(
     "InstanceStateResponseMetadataTypeDef",
     {
         "Code": int,
         "Name": InstanceStateNameType,
@@ -11483,84 +11310,76 @@
 InstanceStatusDetailsTypeDef = TypedDict(
     "InstanceStatusDetailsTypeDef",
     {
         "ImpairedSince": datetime,
         "Name": Literal["reachability"],
         "Status": StatusTypeType,
     },
-    total=False,
 )
 
 InstanceStatusEventTypeDef = TypedDict(
     "InstanceStatusEventTypeDef",
     {
         "InstanceEventId": str,
         "Code": EventCodeType,
         "Description": str,
         "NotAfter": datetime,
         "NotBefore": datetime,
         "NotBeforeDeadline": datetime,
     },
-    total=False,
 )
 
 LicenseConfigurationTypeDef = TypedDict(
     "LicenseConfigurationTypeDef",
     {
         "LicenseConfigurationArn": str,
     },
-    total=False,
 )
 
 PrivateDnsNameOptionsResponseTypeDef = TypedDict(
     "PrivateDnsNameOptionsResponseTypeDef",
     {
         "HostnameType": HostnameTypeType,
         "EnableResourceNameDnsARecord": bool,
         "EnableResourceNameDnsAAAARecord": bool,
     },
-    total=False,
 )
 
 MemoryInfoTypeDef = TypedDict(
     "MemoryInfoTypeDef",
     {
         "SizeInMiB": int,
     },
-    total=False,
 )
 
 PlacementGroupInfoTypeDef = TypedDict(
     "PlacementGroupInfoTypeDef",
     {
         "SupportedStrategies": List[PlacementGroupStrategyType],
     },
-    total=False,
 )
 
 ProcessorInfoTypeDef = TypedDict(
     "ProcessorInfoTypeDef",
     {
         "SupportedArchitectures": List[ArchitectureTypeType],
         "SustainedClockSpeedInGhz": float,
         "SupportedFeatures": List[Literal["amd-sev-snp"]],
     },
-    total=False,
 )
 
 VCpuInfoTypeDef = TypedDict(
     "VCpuInfoTypeDef",
     {
         "DefaultVCpus": int,
         "DefaultCores": int,
         "DefaultThreadsPerCore": int,
         "ValidCores": List[int],
         "ValidThreadsPerCore": List[int],
     },
-    total=False,
 )
 
 IpRangeTypeDef = TypedDict(
     "IpRangeTypeDef",
     {
         "CidrIp": str,
         "Description": str,
@@ -11611,90 +11430,80 @@
 
 IpamDiscoveryFailureReasonTypeDef = TypedDict(
     "IpamDiscoveryFailureReasonTypeDef",
     {
         "Code": IpamDiscoveryFailureCodeType,
         "Message": str,
     },
-    total=False,
 )
 
 IpamResourceTagTypeDef = TypedDict(
     "IpamResourceTagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
-    total=False,
 )
 
 IpamOperatingRegionTypeDef = TypedDict(
     "IpamOperatingRegionTypeDef",
     {
         "RegionName": str,
     },
-    total=False,
 )
 
 IpamPoolCidrFailureReasonTypeDef = TypedDict(
     "IpamPoolCidrFailureReasonTypeDef",
     {
         "Code": IpamPoolCidrFailureCodeType,
         "Message": str,
     },
-    total=False,
 )
 
 Ipv4PrefixSpecificationResponseTypeDef = TypedDict(
     "Ipv4PrefixSpecificationResponseTypeDef",
     {
         "Ipv4Prefix": str,
     },
-    total=False,
 )
 
 Ipv6CidrBlockTypeDef = TypedDict(
     "Ipv6CidrBlockTypeDef",
     {
         "Ipv6CidrBlock": str,
     },
-    total=False,
 )
 
 PoolCidrBlockTypeDef = TypedDict(
     "PoolCidrBlockTypeDef",
     {
         "Cidr": str,
     },
-    total=False,
 )
 
 Ipv6PrefixSpecificationResponseTypeDef = TypedDict(
     "Ipv6PrefixSpecificationResponseTypeDef",
     {
         "Ipv6Prefix": str,
     },
-    total=False,
 )
 
 Ipv6PrefixSpecificationTypeDef = TypedDict(
     "Ipv6PrefixSpecificationTypeDef",
     {
         "Ipv6Prefix": str,
     },
-    total=False,
 )
 
 LastErrorTypeDef = TypedDict(
     "LastErrorTypeDef",
     {
         "Message": str,
         "Code": str,
     },
-    total=False,
 )
 
 RunInstancesMonitoringEnabledTypeDef = TypedDict(
     "RunInstancesMonitoringEnabledTypeDef",
     {
         "Enabled": bool,
     },
@@ -11703,15 +11512,14 @@
 SpotPlacementTypeDef = TypedDict(
     "SpotPlacementTypeDef",
     {
         "AvailabilityZone": str,
         "GroupName": str,
         "Tenancy": TenancyType,
     },
-    total=False,
 )
 
 LaunchTemplateEbsBlockDeviceRequestTypeDef = TypedDict(
     "LaunchTemplateEbsBlockDeviceRequestTypeDef",
     {
         "Encrypted": bool,
         "DeleteOnTermination": bool,
@@ -11733,15 +11541,14 @@
         "Iops": int,
         "KmsKeyId": str,
         "SnapshotId": str,
         "VolumeSize": int,
         "VolumeType": VolumeTypeType,
         "Throughput": int,
     },
-    total=False,
 )
 
 LaunchTemplateCpuOptionsRequestTypeDef = TypedDict(
     "LaunchTemplateCpuOptionsRequestTypeDef",
     {
         "CoreCount": int,
         "ThreadsPerCore": int,
@@ -11753,24 +11560,22 @@
 LaunchTemplateCpuOptionsTypeDef = TypedDict(
     "LaunchTemplateCpuOptionsTypeDef",
     {
         "CoreCount": int,
         "ThreadsPerCore": int,
         "AmdSevSnp": AmdSevSnpSpecificationType,
     },
-    total=False,
 )
 
 LaunchTemplateElasticInferenceAcceleratorResponseTypeDef = TypedDict(
     "LaunchTemplateElasticInferenceAcceleratorResponseTypeDef",
     {
         "Type": str,
         "Count": int,
     },
-    total=False,
 )
 
 _RequiredLaunchTemplateElasticInferenceAcceleratorTypeDef = TypedDict(
     "_RequiredLaunchTemplateElasticInferenceAcceleratorTypeDef",
     {
         "Type": str,
     },
@@ -11800,15 +11605,14 @@
 )
 
 LaunchTemplateEnclaveOptionsTypeDef = TypedDict(
     "LaunchTemplateEnclaveOptionsTypeDef",
     {
         "Enabled": bool,
     },
-    total=False,
 )
 
 LaunchTemplateHibernationOptionsRequestTypeDef = TypedDict(
     "LaunchTemplateHibernationOptionsRequestTypeDef",
     {
         "Configured": bool,
     },
@@ -11816,15 +11620,14 @@
 )
 
 LaunchTemplateHibernationOptionsTypeDef = TypedDict(
     "LaunchTemplateHibernationOptionsTypeDef",
     {
         "Configured": bool,
     },
-    total=False,
 )
 
 LaunchTemplateIamInstanceProfileSpecificationRequestTypeDef = TypedDict(
     "LaunchTemplateIamInstanceProfileSpecificationRequestTypeDef",
     {
         "Arn": str,
         "Name": str,
@@ -11834,15 +11637,14 @@
 
 LaunchTemplateIamInstanceProfileSpecificationTypeDef = TypedDict(
     "LaunchTemplateIamInstanceProfileSpecificationTypeDef",
     {
         "Arn": str,
         "Name": str,
     },
-    total=False,
 )
 
 LaunchTemplateInstanceMaintenanceOptionsRequestTypeDef = TypedDict(
     "LaunchTemplateInstanceMaintenanceOptionsRequestTypeDef",
     {
         "AutoRecovery": LaunchTemplateAutoRecoveryStateType,
     },
@@ -11850,15 +11652,14 @@
 )
 
 LaunchTemplateInstanceMaintenanceOptionsTypeDef = TypedDict(
     "LaunchTemplateInstanceMaintenanceOptionsTypeDef",
     {
         "AutoRecovery": LaunchTemplateAutoRecoveryStateType,
     },
-    total=False,
 )
 
 LaunchTemplateSpotMarketOptionsRequestTypeDef = TypedDict(
     "LaunchTemplateSpotMarketOptionsRequestTypeDef",
     {
         "MaxPrice": str,
         "SpotInstanceType": SpotInstanceTypeType,
@@ -11874,15 +11675,14 @@
     {
         "MaxPrice": str,
         "SpotInstanceType": SpotInstanceTypeType,
         "BlockDurationMinutes": int,
         "ValidUntil": datetime,
         "InstanceInterruptionBehavior": InstanceInterruptionBehaviorType,
     },
-    total=False,
 )
 
 LaunchTemplateInstanceMetadataOptionsRequestTypeDef = TypedDict(
     "LaunchTemplateInstanceMetadataOptionsRequestTypeDef",
     {
         "HttpTokens": LaunchTemplateHttpTokensStateType,
         "HttpPutResponseHopLimit": int,
@@ -11899,15 +11699,14 @@
         "State": LaunchTemplateInstanceMetadataOptionsStateType,
         "HttpTokens": LaunchTemplateHttpTokensStateType,
         "HttpPutResponseHopLimit": int,
         "HttpEndpoint": LaunchTemplateInstanceMetadataEndpointStateType,
         "HttpProtocolIpv6": LaunchTemplateInstanceMetadataProtocolIpv6Type,
         "InstanceMetadataTags": LaunchTemplateInstanceMetadataTagsStateType,
     },
-    total=False,
 )
 
 LaunchTemplateLicenseConfigurationRequestTypeDef = TypedDict(
     "LaunchTemplateLicenseConfigurationRequestTypeDef",
     {
         "LicenseConfigurationArn": str,
     },
@@ -11915,15 +11714,14 @@
 )
 
 LaunchTemplateLicenseConfigurationTypeDef = TypedDict(
     "LaunchTemplateLicenseConfigurationTypeDef",
     {
         "LicenseConfigurationArn": str,
     },
-    total=False,
 )
 
 LaunchTemplatePlacementRequestTypeDef = TypedDict(
     "LaunchTemplatePlacementRequestTypeDef",
     {
         "AvailabilityZone": str,
         "Affinity": str,
@@ -11947,15 +11745,14 @@
         "HostId": str,
         "Tenancy": TenancyType,
         "SpreadDomain": str,
         "HostResourceGroupArn": str,
         "PartitionNumber": int,
         "GroupId": str,
     },
-    total=False,
 )
 
 LaunchTemplatePrivateDnsNameOptionsRequestTypeDef = TypedDict(
     "LaunchTemplatePrivateDnsNameOptionsRequestTypeDef",
     {
         "HostnameType": HostnameTypeType,
         "EnableResourceNameDnsARecord": bool,
@@ -11967,15 +11764,14 @@
 LaunchTemplatePrivateDnsNameOptionsTypeDef = TypedDict(
     "LaunchTemplatePrivateDnsNameOptionsTypeDef",
     {
         "HostnameType": HostnameTypeType,
         "EnableResourceNameDnsARecord": bool,
         "EnableResourceNameDnsAAAARecord": bool,
     },
-    total=False,
 )
 
 LaunchTemplateSpecificationTypeDef = TypedDict(
     "LaunchTemplateSpecificationTypeDef",
     {
         "LaunchTemplateId": str,
         "LaunchTemplateName": str,
@@ -11993,15 +11789,14 @@
 )
 
 LaunchTemplatesMonitoringTypeDef = TypedDict(
     "LaunchTemplatesMonitoringTypeDef",
     {
         "Enabled": bool,
     },
-    total=False,
 )
 
 LicenseConfigurationRequestTypeDef = TypedDict(
     "LicenseConfigurationRequestTypeDef",
     {
         "LicenseConfigurationArn": str,
     },
@@ -12055,15 +11850,14 @@
     {
         "SnapshotId": str,
         "RecycleBinEnterTime": datetime,
         "RecycleBinExitTime": datetime,
         "Description": str,
         "VolumeId": str,
     },
-    total=False,
 )
 
 LoadPermissionRequestTypeDef = TypedDict(
     "LoadPermissionRequestTypeDef",
     {
         "Group": Literal["all"],
         "UserId": str,
@@ -12313,15 +12107,14 @@
 )
 
 SuccessfulInstanceCreditSpecificationItemTypeDef = TypedDict(
     "SuccessfulInstanceCreditSpecificationItemTypeDef",
     {
         "InstanceId": str,
     },
-    total=False,
 )
 
 _RequiredModifyInstanceEventStartTimeRequestRequestTypeDef = TypedDict(
     "_RequiredModifyInstanceEventStartTimeRequestRequestTypeDef",
     {
         "InstanceId": str,
         "InstanceEventId": str,
@@ -12588,15 +12381,14 @@
     {
         "AvailabilityZone": str,
         "InstanceCount": int,
         "InstanceType": InstanceTypeType,
         "Platform": str,
         "Scope": scopeType,
     },
-    total=False,
 )
 
 ModifyReservedInstancesResultTypeDef = TypedDict(
     "ModifyReservedInstancesResultTypeDef",
     {
         "ReservedInstancesModificationId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
@@ -13079,15 +12871,14 @@
 PeeringConnectionOptionsTypeDef = TypedDict(
     "PeeringConnectionOptionsTypeDef",
     {
         "AllowDnsResolutionFromRemoteVpc": bool,
         "AllowEgressFromLocalClassicLinkToRemoteVpc": bool,
         "AllowEgressFromLocalVpcToRemoteClassicLink": bool,
     },
-    total=False,
 )
 
 _RequiredModifyVpcTenancyRequestRequestTypeDef = TypedDict(
     "_RequiredModifyVpcTenancyRequestRequestTypeDef",
     {
         "VpcId": str,
         "InstanceTenancy": Literal["default"],
@@ -13334,35 +13125,32 @@
     {
         "ProvisionTime": datetime,
         "Provisioned": str,
         "RequestTime": datetime,
         "Requested": str,
         "Status": str,
     },
-    total=False,
 )
 
 NetworkAclAssociationTypeDef = TypedDict(
     "NetworkAclAssociationTypeDef",
     {
         "NetworkAclAssociationId": str,
         "NetworkAclId": str,
         "SubnetId": str,
     },
-    total=False,
 )
 
 NetworkCardInfoTypeDef = TypedDict(
     "NetworkCardInfoTypeDef",
     {
         "NetworkCardIndex": int,
         "NetworkPerformance": str,
         "MaximumNetworkInterfaces": int,
     },
-    total=False,
 )
 
 NetworkInterfaceAssociationResponseMetadataTypeDef = TypedDict(
     "NetworkInterfaceAssociationResponseMetadataTypeDef",
     {
         "AllocationId": str,
         "AssociationId": str,
@@ -13382,46 +13170,42 @@
         "AssociationId": str,
         "IpOwnerId": str,
         "PublicDnsName": str,
         "PublicIp": str,
         "CustomerOwnedIp": str,
         "CarrierIp": str,
     },
-    total=False,
 )
 
 NetworkInterfaceIpv6AddressTypeDef = TypedDict(
     "NetworkInterfaceIpv6AddressTypeDef",
     {
         "Ipv6Address": str,
     },
-    total=False,
 )
 
 NetworkInterfacePermissionStateTypeDef = TypedDict(
     "NetworkInterfacePermissionStateTypeDef",
     {
         "State": NetworkInterfacePermissionStateCodeType,
         "StatusMessage": str,
     },
-    total=False,
 )
 
 OidcOptionsTypeDef = TypedDict(
     "OidcOptionsTypeDef",
     {
         "Issuer": str,
         "AuthorizationEndpoint": str,
         "TokenEndpoint": str,
         "UserInfoEndpoint": str,
         "ClientId": str,
         "ClientSecret": str,
         "Scope": str,
     },
-    total=False,
 )
 
 PacketHeaderStatementRequestTypeDef = TypedDict(
     "PacketHeaderStatementRequestTypeDef",
     {
         "SourceAddresses": Sequence[str],
         "DestinationAddresses": Sequence[str],
@@ -13441,15 +13225,14 @@
         "DestinationAddresses": List[str],
         "SourcePorts": List[str],
         "DestinationPorts": List[str],
         "SourcePrefixLists": List[str],
         "DestinationPrefixLists": List[str],
         "Protocols": List[ProtocolType],
     },
-    total=False,
 )
 
 PaginatorConfigTypeDef = TypedDict(
     "PaginatorConfigTypeDef",
     {
         "MaxItems": int,
         "PageSize": int,
@@ -13478,83 +13261,74 @@
 
 ResourceStatementTypeDef = TypedDict(
     "ResourceStatementTypeDef",
     {
         "Resources": List[str],
         "ResourceTypes": List[str],
     },
-    total=False,
 )
 
 PeeringAttachmentStatusTypeDef = TypedDict(
     "PeeringAttachmentStatusTypeDef",
     {
         "Code": str,
         "Message": str,
     },
-    total=False,
 )
 
 PeeringTgwInfoTypeDef = TypedDict(
     "PeeringTgwInfoTypeDef",
     {
         "TransitGatewayId": str,
         "CoreNetworkId": str,
         "OwnerId": str,
         "Region": str,
     },
-    total=False,
 )
 
 Phase1DHGroupNumbersListValueTypeDef = TypedDict(
     "Phase1DHGroupNumbersListValueTypeDef",
     {
         "Value": int,
     },
-    total=False,
 )
 
 Phase1EncryptionAlgorithmsListValueTypeDef = TypedDict(
     "Phase1EncryptionAlgorithmsListValueTypeDef",
     {
         "Value": str,
     },
-    total=False,
 )
 
 Phase1IntegrityAlgorithmsListValueTypeDef = TypedDict(
     "Phase1IntegrityAlgorithmsListValueTypeDef",
     {
         "Value": str,
     },
-    total=False,
 )
 
 Phase2DHGroupNumbersListValueTypeDef = TypedDict(
     "Phase2DHGroupNumbersListValueTypeDef",
     {
         "Value": int,
     },
-    total=False,
 )
 
 Phase2EncryptionAlgorithmsListValueTypeDef = TypedDict(
     "Phase2EncryptionAlgorithmsListValueTypeDef",
     {
         "Value": str,
     },
-    total=False,
 )
 
 Phase2IntegrityAlgorithmsListValueTypeDef = TypedDict(
     "Phase2IntegrityAlgorithmsListValueTypeDef",
     {
         "Value": str,
     },
-    total=False,
 )
 
 PlacementResponseMetadataTypeDef = TypedDict(
     "PlacementResponseMetadataTypeDef",
     {
         "AvailabilityZone": str,
         "Affinity": str,
@@ -13573,43 +13347,39 @@
     "PriceScheduleTypeDef",
     {
         "Active": bool,
         "CurrencyCode": Literal["USD"],
         "Price": float,
         "Term": int,
     },
-    total=False,
 )
 
 PricingDetailTypeDef = TypedDict(
     "PricingDetailTypeDef",
     {
         "Count": int,
         "Price": float,
     },
-    total=False,
 )
 
 PrivateDnsDetailsTypeDef = TypedDict(
     "PrivateDnsDetailsTypeDef",
     {
         "PrivateDnsName": str,
     },
-    total=False,
 )
 
 PrivateDnsNameConfigurationTypeDef = TypedDict(
     "PrivateDnsNameConfigurationTypeDef",
     {
         "State": DnsNameStateType,
         "Type": str,
         "Value": str,
         "Name": str,
     },
-    total=False,
 )
 
 PrivateDnsNameOptionsOnLaunchResponseMetadataTypeDef = TypedDict(
     "PrivateDnsNameOptionsOnLaunchResponseMetadataTypeDef",
     {
         "HostnameType": HostnameTypeType,
         "EnableResourceNameDnsARecord": bool,
@@ -13621,15 +13391,14 @@
 PrivateDnsNameOptionsOnLaunchTypeDef = TypedDict(
     "PrivateDnsNameOptionsOnLaunchTypeDef",
     {
         "HostnameType": HostnameTypeType,
         "EnableResourceNameDnsARecord": bool,
         "EnableResourceNameDnsAAAARecord": bool,
     },
-    total=False,
 )
 
 PrivateDnsNameOptionsRequestTypeDef = TypedDict(
     "PrivateDnsNameOptionsRequestTypeDef",
     {
         "HostnameType": HostnameTypeType,
         "EnableResourceNameDnsARecord": bool,
@@ -13649,15 +13418,14 @@
 )
 
 PropagatingVgwTypeDef = TypedDict(
     "PropagatingVgwTypeDef",
     {
         "GatewayId": str,
     },
-    total=False,
 )
 
 _RequiredProvisionPublicIpv4PoolCidrRequestRequestTypeDef = TypedDict(
     "_RequiredProvisionPublicIpv4PoolCidrRequestRequestTypeDef",
     {
         "IpamPoolId": str,
         "PoolId": str,
@@ -13684,15 +13452,14 @@
     "PublicIpv4PoolRangeTypeDef",
     {
         "FirstAddress": str,
         "LastAddress": str,
         "AddressCount": int,
         "AvailableAddressCount": int,
     },
-    total=False,
 )
 
 PurchaseRequestTypeDef = TypedDict(
     "PurchaseRequestTypeDef",
     {
         "InstanceCount": int,
         "PurchaseToken": str,
@@ -13747,27 +13514,25 @@
 
 RecurringChargeTypeDef = TypedDict(
     "RecurringChargeTypeDef",
     {
         "Amount": float,
         "Frequency": Literal["Hourly"],
     },
-    total=False,
 )
 
 ReferencedSecurityGroupTypeDef = TypedDict(
     "ReferencedSecurityGroupTypeDef",
     {
         "GroupId": str,
         "PeeringStatus": str,
         "UserId": str,
         "VpcId": str,
         "VpcPeeringConnectionId": str,
     },
-    total=False,
 )
 
 RegisterImageResultTypeDef = TypedDict(
     "RegisterImageResultTypeDef",
     {
         "ImageId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
@@ -13810,15 +13575,14 @@
 TransitGatewayMulticastRegisteredGroupMembersTypeDef = TypedDict(
     "TransitGatewayMulticastRegisteredGroupMembersTypeDef",
     {
         "TransitGatewayMulticastDomainId": str,
         "RegisteredNetworkInterfaceIds": List[str],
         "GroupIpAddress": str,
     },
-    total=False,
 )
 
 _RequiredRegisterTransitGatewayMulticastGroupSourcesRequestRequestTypeDef = TypedDict(
     "_RequiredRegisterTransitGatewayMulticastGroupSourcesRequestRequestTypeDef",
     {
         "TransitGatewayMulticastDomainId": str,
         "NetworkInterfaceIds": Sequence[str],
@@ -13844,15 +13608,14 @@
 TransitGatewayMulticastRegisteredGroupSourcesTypeDef = TypedDict(
     "TransitGatewayMulticastRegisteredGroupSourcesTypeDef",
     {
         "TransitGatewayMulticastDomainId": str,
         "RegisteredNetworkInterfaceIds": List[str],
         "GroupIpAddress": str,
     },
-    total=False,
 )
 
 RejectTransitGatewayMulticastDomainAssociationsRequestRequestTypeDef = TypedDict(
     "RejectTransitGatewayMulticastDomainAssociationsRequestRequestTypeDef",
     {
         "TransitGatewayMulticastDomainId": str,
         "TransitGatewayAttachmentId": str,
@@ -14313,15 +14076,14 @@
 )
 
 ReservedInstancesIdTypeDef = TypedDict(
     "ReservedInstancesIdTypeDef",
     {
         "ReservedInstancesId": str,
     },
-    total=False,
 )
 
 _RequiredResetAddressAttributeRequestRequestTypeDef = TypedDict(
     "_RequiredResetAddressAttributeRequestRequestTypeDef",
     {
         "AllocationId": str,
         "Attribute": Literal["domain-name"],
@@ -14804,15 +14566,14 @@
         "CarrierGatewayId": str,
         "NetworkInterfaceId": str,
         "Origin": RouteOriginType,
         "State": RouteStateType,
         "VpcPeeringConnectionId": str,
         "CoreNetworkArn": str,
     },
-    total=False,
 )
 
 RunScheduledInstancesResultTypeDef = TypedDict(
     "RunScheduledInstancesResultTypeDef",
     {
         "InstanceIdSet": List[str],
         "ResponseMetadata": "ResponseMetadataTypeDef",
@@ -14836,15 +14597,14 @@
     {
         "Frequency": str,
         "Interval": int,
         "OccurrenceDaySet": List[int],
         "OccurrenceRelativeToEnd": bool,
         "OccurrenceUnit": str,
     },
-    total=False,
 )
 
 ScheduledInstancesEbsTypeDef = TypedDict(
     "ScheduledInstancesEbsTypeDef",
     {
         "DeleteOnTermination": bool,
         "Encrypted": bool,
@@ -14910,24 +14670,22 @@
         "ResourceOwnerId": str,
         "NetworkInterfaceId": str,
         "GroupMember": bool,
         "GroupSource": bool,
         "MemberType": MembershipTypeType,
         "SourceType": MembershipTypeType,
     },
-    total=False,
 )
 
 SecurityGroupIdentifierTypeDef = TypedDict(
     "SecurityGroupIdentifierTypeDef",
     {
         "GroupId": str,
         "GroupName": str,
     },
-    total=False,
 )
 
 SecurityGroupRuleDescriptionTypeDef = TypedDict(
     "SecurityGroupRuleDescriptionTypeDef",
     {
         "SecurityGroupRuleId": str,
         "Description": str,
@@ -14973,60 +14731,54 @@
 
 
 ServiceTypeDetailTypeDef = TypedDict(
     "ServiceTypeDetailTypeDef",
     {
         "ServiceType": ServiceTypeType,
     },
-    total=False,
 )
 
 UserBucketDetailsTypeDef = TypedDict(
     "UserBucketDetailsTypeDef",
     {
         "S3Bucket": str,
         "S3Key": str,
     },
-    total=False,
 )
 
 SpotCapacityRebalanceTypeDef = TypedDict(
     "SpotCapacityRebalanceTypeDef",
     {
         "ReplacementStrategy": ReplacementStrategyType,
         "TerminationDelay": int,
     },
-    total=False,
 )
 
 SpotInstanceStateFaultTypeDef = TypedDict(
     "SpotInstanceStateFaultTypeDef",
     {
         "Code": str,
         "Message": str,
     },
-    total=False,
 )
 
 SpotFleetMonitoringTypeDef = TypedDict(
     "SpotFleetMonitoringTypeDef",
     {
         "Enabled": bool,
     },
-    total=False,
 )
 
 SpotInstanceStatusTypeDef = TypedDict(
     "SpotInstanceStatusTypeDef",
     {
         "Code": str,
         "Message": str,
         "UpdateTime": datetime,
     },
-    total=False,
 )
 
 StartInstancesRequestInstanceStartTypeDef = TypedDict(
     "StartInstancesRequestInstanceStartTypeDef",
     {
         "AdditionalInfo": str,
         "DryRun": bool,
@@ -15130,41 +14882,37 @@
 
 SubnetAssociationTypeDef = TypedDict(
     "SubnetAssociationTypeDef",
     {
         "SubnetId": str,
         "State": TransitGatewayMulitcastDomainAssociationStateType,
     },
-    total=False,
 )
 
 SubnetCidrBlockStateTypeDef = TypedDict(
     "SubnetCidrBlockStateTypeDef",
     {
         "State": SubnetCidrBlockStateCodeType,
         "StatusMessage": str,
     },
-    total=False,
 )
 
 TargetConfigurationTypeDef = TypedDict(
     "TargetConfigurationTypeDef",
     {
         "InstanceCount": int,
         "OfferingId": str,
     },
-    total=False,
 )
 
 TargetGroupTypeDef = TypedDict(
     "TargetGroupTypeDef",
     {
         "Arn": str,
     },
-    total=False,
 )
 
 _RequiredTerminateClientVpnConnectionsRequestRequestTypeDef = TypedDict(
     "_RequiredTerminateClientVpnConnectionsRequestRequestTypeDef",
     {
         "ClientVpnEndpointId": str,
     },
@@ -15219,54 +14967,49 @@
 
 TrafficMirrorPortRangeTypeDef = TypedDict(
     "TrafficMirrorPortRangeTypeDef",
     {
         "FromPort": int,
         "ToPort": int,
     },
-    total=False,
 )
 
 TransitGatewayAttachmentAssociationTypeDef = TypedDict(
     "TransitGatewayAttachmentAssociationTypeDef",
     {
         "TransitGatewayRouteTableId": str,
         "State": TransitGatewayAssociationStateType,
     },
-    total=False,
 )
 
 TransitGatewayAttachmentBgpConfigurationTypeDef = TypedDict(
     "TransitGatewayAttachmentBgpConfigurationTypeDef",
     {
         "TransitGatewayAsn": int,
         "PeerAsn": int,
         "TransitGatewayAddress": str,
         "PeerAddress": str,
         "BgpStatus": BgpStatusType,
     },
-    total=False,
 )
 
 TransitGatewayConnectOptionsTypeDef = TypedDict(
     "TransitGatewayConnectOptionsTypeDef",
     {
         "Protocol": Literal["gre"],
     },
-    total=False,
 )
 
 TransitGatewayMulticastDomainOptionsTypeDef = TypedDict(
     "TransitGatewayMulticastDomainOptionsTypeDef",
     {
         "Igmpv2Support": Igmpv2SupportValueType,
         "StaticSourcesSupport": StaticSourcesSupportValueType,
         "AutoAcceptSharedAssociations": AutoAcceptSharedAssociationsValueType,
     },
-    total=False,
 )
 
 TransitGatewayOptionsTypeDef = TypedDict(
     "TransitGatewayOptionsTypeDef",
     {
         "AmazonSideAsn": int,
         "TransitGatewayCidrBlocks": List[str],
@@ -15275,62 +15018,56 @@
         "AssociationDefaultRouteTableId": str,
         "DefaultRouteTablePropagation": DefaultRouteTablePropagationValueType,
         "PropagationDefaultRouteTableId": str,
         "VpnEcmpSupport": VpnEcmpSupportValueType,
         "DnsSupport": DnsSupportValueType,
         "MulticastSupport": MulticastSupportValueType,
     },
-    total=False,
 )
 
 TransitGatewayPeeringAttachmentOptionsTypeDef = TypedDict(
     "TransitGatewayPeeringAttachmentOptionsTypeDef",
     {
         "DynamicRouting": DynamicRoutingValueType,
     },
-    total=False,
 )
 
 TransitGatewayPolicyRuleMetaDataTypeDef = TypedDict(
     "TransitGatewayPolicyRuleMetaDataTypeDef",
     {
         "MetaDataKey": str,
         "MetaDataValue": str,
     },
-    total=False,
 )
 
 TransitGatewayPrefixListAttachmentTypeDef = TypedDict(
     "TransitGatewayPrefixListAttachmentTypeDef",
     {
         "TransitGatewayAttachmentId": str,
         "ResourceType": TransitGatewayAttachmentResourceTypeType,
         "ResourceId": str,
     },
-    total=False,
 )
 
 TransitGatewayRouteAttachmentTypeDef = TypedDict(
     "TransitGatewayRouteAttachmentTypeDef",
     {
         "ResourceId": str,
         "TransitGatewayAttachmentId": str,
         "ResourceType": TransitGatewayAttachmentResourceTypeType,
     },
-    total=False,
 )
 
 TransitGatewayVpcAttachmentOptionsTypeDef = TypedDict(
     "TransitGatewayVpcAttachmentOptionsTypeDef",
     {
         "DnsSupport": DnsSupportValueType,
         "Ipv6Support": Ipv6SupportValueType,
         "ApplianceModeSupport": ApplianceModeSupportValueType,
     },
-    total=False,
 )
 
 _RequiredUnassignIpv6AddressesRequestRequestTypeDef = TypedDict(
     "_RequiredUnassignIpv6AddressesRequestRequestTypeDef",
     {
         "NetworkInterfaceId": str,
     },
@@ -15450,24 +15187,22 @@
 
 UnsuccessfulInstanceCreditSpecificationItemErrorTypeDef = TypedDict(
     "UnsuccessfulInstanceCreditSpecificationItemErrorTypeDef",
     {
         "Code": UnsuccessfulInstanceCreditSpecificationErrorCodeType,
         "Message": str,
     },
-    total=False,
 )
 
 UnsuccessfulItemErrorTypeDef = TypedDict(
     "UnsuccessfulItemErrorTypeDef",
     {
         "Code": str,
         "Message": str,
     },
-    total=False,
 )
 
 UpdateSecurityGroupRuleDescriptionsEgressResultTypeDef = TypedDict(
     "UpdateSecurityGroupRuleDescriptionsEgressResultTypeDef",
     {
         "Return": bool,
         "ResponseMetadata": "ResponseMetadataTypeDef",
@@ -15484,57 +15219,52 @@
 
 ValidationErrorTypeDef = TypedDict(
     "ValidationErrorTypeDef",
     {
         "Code": str,
         "Message": str,
     },
-    total=False,
 )
 
 VerifiedAccessEndpointEniOptionsTypeDef = TypedDict(
     "VerifiedAccessEndpointEniOptionsTypeDef",
     {
         "NetworkInterfaceId": str,
         "Protocol": VerifiedAccessEndpointProtocolType,
         "Port": int,
     },
-    total=False,
 )
 
 VerifiedAccessEndpointLoadBalancerOptionsTypeDef = TypedDict(
     "VerifiedAccessEndpointLoadBalancerOptionsTypeDef",
     {
         "Protocol": VerifiedAccessEndpointProtocolType,
         "Port": int,
         "LoadBalancerArn": str,
         "SubnetIds": List[str],
     },
-    total=False,
 )
 
 VerifiedAccessEndpointStatusTypeDef = TypedDict(
     "VerifiedAccessEndpointStatusTypeDef",
     {
         "Code": VerifiedAccessEndpointStatusCodeType,
         "Message": str,
     },
-    total=False,
 )
 
 VerifiedAccessTrustProviderCondensedTypeDef = TypedDict(
     "VerifiedAccessTrustProviderCondensedTypeDef",
     {
         "VerifiedAccessTrustProviderId": str,
         "Description": str,
         "TrustProviderType": TrustProviderTypeType,
         "UserTrustProviderType": UserTrustProviderTypeType,
         "DeviceTrustProviderType": DeviceTrustProviderTypeType,
     },
-    total=False,
 )
 
 _RequiredVerifiedAccessLogCloudWatchLogsDestinationOptionsTypeDef = TypedDict(
     "_RequiredVerifiedAccessLogCloudWatchLogsDestinationOptionsTypeDef",
     {
         "Enabled": bool,
     },
@@ -15557,15 +15287,14 @@
 
 VerifiedAccessLogDeliveryStatusTypeDef = TypedDict(
     "VerifiedAccessLogDeliveryStatusTypeDef",
     {
         "Code": VerifiedAccessLogDeliveryStatusCodeType,
         "Message": str,
     },
-    total=False,
 )
 
 _RequiredVerifiedAccessLogKinesisDataFirehoseDestinationOptionsTypeDef = TypedDict(
     "_RequiredVerifiedAccessLogKinesisDataFirehoseDestinationOptionsTypeDef",
     {
         "Enabled": bool,
     },
@@ -15616,15 +15345,14 @@
         "AcceptedRouteCount": int,
         "LastStatusChange": datetime,
         "OutsideIpAddress": str,
         "Status": TelemetryStatusType,
         "StatusMessage": str,
         "CertificateArn": str,
     },
-    total=False,
 )
 
 VolumeAttachmentResponseMetadataTypeDef = TypedDict(
     "VolumeAttachmentResponseMetadataTypeDef",
     {
         "AttachTime": datetime,
         "Device": str,
@@ -15642,76 +15370,69 @@
         "AttachTime": datetime,
         "Device": str,
         "InstanceId": str,
         "State": VolumeAttachmentStateType,
         "VolumeId": str,
         "DeleteOnTermination": bool,
     },
-    total=False,
 )
 
 VolumeStatusActionTypeDef = TypedDict(
     "VolumeStatusActionTypeDef",
     {
         "Code": str,
         "Description": str,
         "EventId": str,
         "EventType": str,
     },
-    total=False,
 )
 
 VolumeStatusAttachmentStatusTypeDef = TypedDict(
     "VolumeStatusAttachmentStatusTypeDef",
     {
         "IoPerformance": str,
         "InstanceId": str,
     },
-    total=False,
 )
 
 VolumeStatusDetailsTypeDef = TypedDict(
     "VolumeStatusDetailsTypeDef",
     {
         "Name": VolumeStatusNameType,
         "Status": str,
     },
-    total=False,
 )
 
 VolumeStatusEventTypeDef = TypedDict(
     "VolumeStatusEventTypeDef",
     {
         "Description": str,
         "EventId": str,
         "EventType": str,
         "NotAfter": datetime,
         "NotBefore": datetime,
         "InstanceId": str,
     },
-    total=False,
 )
 
 VpcCidrBlockStateTypeDef = TypedDict(
     "VpcCidrBlockStateTypeDef",
     {
         "State": VpcCidrBlockStateCodeType,
         "StatusMessage": str,
     },
-    total=False,
 )
 
 VpcPeeringConnectionOptionsDescriptionTypeDef = TypedDict(
     "VpcPeeringConnectionOptionsDescriptionTypeDef",
     {
         "AllowDnsResolutionFromRemoteVpc": bool,
         "AllowEgressFromLocalClassicLinkToRemoteVpc": bool,
         "AllowEgressFromLocalVpcToRemoteClassicLink": bool,
     },
-    total=False,
 )
 
 VpcPeeringConnectionStateReasonResponseMetadataTypeDef = TypedDict(
     "VpcPeeringConnectionStateReasonResponseMetadataTypeDef",
     {
         "Code": VpcPeeringConnectionStateReasonCodeType,
         "Message": str,
@@ -15721,25 +15442,23 @@
 
 VpcPeeringConnectionStateReasonTypeDef = TypedDict(
     "VpcPeeringConnectionStateReasonTypeDef",
     {
         "Code": VpcPeeringConnectionStateReasonCodeType,
         "Message": str,
     },
-    total=False,
 )
 
 VpnStaticRouteTypeDef = TypedDict(
     "VpnStaticRouteTypeDef",
     {
         "DestinationCidrBlock": str,
         "Source": Literal["Static"],
         "State": VpnStateType,
     },
-    total=False,
 )
 
 _RequiredWithdrawByoipCidrRequestRequestTypeDef = TypedDict(
     "_RequiredWithdrawByoipCidrRequestRequestTypeDef",
     {
         "Cidr": str,
     },
@@ -15840,15 +15559,14 @@
 
 AccountAttributeTypeDef = TypedDict(
     "AccountAttributeTypeDef",
     {
         "AttributeName": str,
         "AttributeValues": List[AccountAttributeValueTypeDef],
     },
-    total=False,
 )
 
 DescribeFleetInstancesResultTypeDef = TypedDict(
     "DescribeFleetInstancesResultTypeDef",
     {
         "ActiveInstances": List[ActiveInstanceTypeDef],
         "NextToken": str,
@@ -15880,35 +15598,32 @@
     "AnalysisLoadBalancerTargetTypeDef",
     {
         "Address": str,
         "AvailabilityZone": str,
         "Instance": AnalysisComponentTypeDef,
         "Port": int,
     },
-    total=False,
 )
 
 RuleGroupRuleOptionsPairTypeDef = TypedDict(
     "RuleGroupRuleOptionsPairTypeDef",
     {
         "RuleGroupArn": str,
         "RuleOptions": List[RuleOptionTypeDef],
     },
-    total=False,
 )
 
 AddressAttributeTypeDef = TypedDict(
     "AddressAttributeTypeDef",
     {
         "PublicIp": str,
         "AllocationId": str,
         "PtrRecord": str,
         "PtrRecordUpdate": PtrUpdateStatusTypeDef,
     },
-    total=False,
 )
 
 AddressTypeDef = TypedDict(
     "AddressTypeDef",
     {
         "InstanceId": str,
         "PublicIp": str,
@@ -15921,39 +15636,36 @@
         "Tags": List[TagTypeDef],
         "PublicIpv4Pool": str,
         "NetworkBorderGroup": str,
         "CustomerOwnedIp": str,
         "CustomerOwnedIpv4Pool": str,
         "CarrierIp": str,
     },
-    total=False,
 )
 
 AllowedPrincipalTypeDef = TypedDict(
     "AllowedPrincipalTypeDef",
     {
         "PrincipalType": PrincipalTypeType,
         "Principal": str,
         "ServicePermissionId": str,
         "Tags": List[TagTypeDef],
         "ServiceId": str,
     },
-    total=False,
 )
 
 CarrierGatewayTypeDef = TypedDict(
     "CarrierGatewayTypeDef",
     {
         "CarrierGatewayId": str,
         "VpcId": str,
         "State": CarrierGatewayStateType,
         "OwnerId": str,
         "Tags": List[TagTypeDef],
     },
-    total=False,
 )
 
 _RequiredClientCreateTagsRequestTypeDef = TypedDict(
     "_RequiredClientCreateTagsRequestTypeDef",
     {
         "Resources": Sequence[str],
         "Tags": Sequence[TagTypeDef],
@@ -16001,15 +15713,14 @@
     {
         "PoolId": str,
         "PoolCidrs": List[str],
         "LocalGatewayRouteTableId": str,
         "Tags": List[TagTypeDef],
         "PoolArn": str,
     },
-    total=False,
 )
 
 CopySnapshotResultTypeDef = TypedDict(
     "CopySnapshotResultTypeDef",
     {
         "SnapshotId": str,
         "Tags": List[TagTypeDef],
@@ -16057,15 +15768,14 @@
         "IpAddress": str,
         "CertificateArn": str,
         "State": str,
         "Type": str,
         "DeviceName": str,
         "Tags": List[TagTypeDef],
     },
-    total=False,
 )
 
 Ec2InstanceConnectEndpointTypeDef = TypedDict(
     "Ec2InstanceConnectEndpointTypeDef",
     {
         "OwnerId": str,
         "InstanceConnectEndpointId": str,
@@ -16079,15 +15789,14 @@
         "AvailabilityZone": str,
         "CreatedAt": datetime,
         "SubnetId": str,
         "PreserveClientIp": bool,
         "SecurityGroupIds": List[str],
         "Tags": List[TagTypeDef],
     },
-    total=False,
 )
 
 HostReservationTypeDef = TypedDict(
     "HostReservationTypeDef",
     {
         "Count": int,
         "CurrencyCode": Literal["USD"],
@@ -16100,15 +15809,14 @@
         "OfferingId": str,
         "PaymentOption": PaymentOptionType,
         "Start": datetime,
         "State": ReservationStateType,
         "UpfrontPrice": str,
         "Tags": List[TagTypeDef],
     },
-    total=False,
 )
 
 ImportKeyPairResultTypeDef = TypedDict(
     "ImportKeyPairResultTypeDef",
     {
         "KeyFingerprint": str,
         "KeyName": str,
@@ -16161,15 +15869,14 @@
 InstanceEventWindowAssociationTargetTypeDef = TypedDict(
     "InstanceEventWindowAssociationTargetTypeDef",
     {
         "InstanceIds": List[str],
         "Tags": List[TagTypeDef],
         "DedicatedHostIds": List[str],
     },
-    total=False,
 )
 
 InstanceEventWindowDisassociationRequestTypeDef = TypedDict(
     "InstanceEventWindowDisassociationRequestTypeDef",
     {
         "InstanceIds": Sequence[str],
         "InstanceTags": Sequence[TagTypeDef],
@@ -16189,15 +15896,14 @@
         "IpamArn": str,
         "IpamRegion": str,
         "IsDefault": bool,
         "ResourceDiscoveryStatus": IpamAssociatedResourceDiscoveryStatusType,
         "State": IpamResourceDiscoveryAssociationStateType,
         "Tags": List[TagTypeDef],
     },
-    total=False,
 )
 
 IpamScopeTypeDef = TypedDict(
     "IpamScopeTypeDef",
     {
         "OwnerId": str,
         "IpamScopeId": str,
@@ -16207,29 +15913,27 @@
         "IpamScopeType": IpamScopeTypeType,
         "IsDefault": bool,
         "Description": str,
         "PoolCount": int,
         "State": IpamScopeStateType,
         "Tags": List[TagTypeDef],
     },
-    total=False,
 )
 
 KeyPairInfoTypeDef = TypedDict(
     "KeyPairInfoTypeDef",
     {
         "KeyPairId": str,
         "KeyFingerprint": str,
         "KeyName": str,
         "KeyType": KeyTypeType,
         "Tags": List[TagTypeDef],
         "PublicKey": str,
         "CreateTime": datetime,
     },
-    total=False,
 )
 
 KeyPairTypeDef = TypedDict(
     "KeyPairTypeDef",
     {
         "KeyFingerprint": str,
         "KeyMaterial": str,
@@ -16251,83 +15955,77 @@
 
 LaunchTemplateTagSpecificationTypeDef = TypedDict(
     "LaunchTemplateTagSpecificationTypeDef",
     {
         "ResourceType": ResourceTypeType,
         "Tags": List[TagTypeDef],
     },
-    total=False,
 )
 
 LaunchTemplateTypeDef = TypedDict(
     "LaunchTemplateTypeDef",
     {
         "LaunchTemplateId": str,
         "LaunchTemplateName": str,
         "CreateTime": datetime,
         "CreatedBy": str,
         "DefaultVersionNumber": int,
         "LatestVersionNumber": int,
         "Tags": List[TagTypeDef],
     },
-    total=False,
 )
 
 LocalGatewayRouteTableVirtualInterfaceGroupAssociationTypeDef = TypedDict(
     "LocalGatewayRouteTableVirtualInterfaceGroupAssociationTypeDef",
     {
         "LocalGatewayRouteTableVirtualInterfaceGroupAssociationId": str,
         "LocalGatewayVirtualInterfaceGroupId": str,
         "LocalGatewayId": str,
         "LocalGatewayRouteTableId": str,
         "LocalGatewayRouteTableArn": str,
         "OwnerId": str,
         "State": str,
         "Tags": List[TagTypeDef],
     },
-    total=False,
 )
 
 LocalGatewayRouteTableVpcAssociationTypeDef = TypedDict(
     "LocalGatewayRouteTableVpcAssociationTypeDef",
     {
         "LocalGatewayRouteTableVpcAssociationId": str,
         "LocalGatewayRouteTableId": str,
         "LocalGatewayRouteTableArn": str,
         "LocalGatewayId": str,
         "VpcId": str,
         "OwnerId": str,
         "State": str,
         "Tags": List[TagTypeDef],
     },
-    total=False,
 )
 
 LocalGatewayTypeDef = TypedDict(
     "LocalGatewayTypeDef",
     {
         "LocalGatewayId": str,
         "OutpostArn": str,
         "OwnerId": str,
         "State": str,
         "Tags": List[TagTypeDef],
     },
-    total=False,
 )
 
 LocalGatewayVirtualInterfaceGroupTypeDef = TypedDict(
     "LocalGatewayVirtualInterfaceGroupTypeDef",
     {
         "LocalGatewayVirtualInterfaceGroupId": str,
         "LocalGatewayVirtualInterfaceIds": List[str],
         "LocalGatewayId": str,
         "OwnerId": str,
         "Tags": List[TagTypeDef],
     },
-    total=False,
 )
 
 LocalGatewayVirtualInterfaceTypeDef = TypedDict(
     "LocalGatewayVirtualInterfaceTypeDef",
     {
         "LocalGatewayVirtualInterfaceId": str,
         "LocalGatewayId": str,
@@ -16335,15 +16033,14 @@
         "LocalAddress": str,
         "PeerAddress": str,
         "LocalBgpAsn": int,
         "PeerBgpAsn": int,
         "OwnerId": str,
         "Tags": List[TagTypeDef],
     },
-    total=False,
 )
 
 ManagedPrefixListTypeDef = TypedDict(
     "ManagedPrefixListTypeDef",
     {
         "PrefixListId": str,
         "AddressFamily": str,
@@ -16352,15 +16049,14 @@
         "PrefixListArn": str,
         "PrefixListName": str,
         "MaxEntries": int,
         "Version": int,
         "Tags": List[TagTypeDef],
         "OwnerId": str,
     },
-    total=False,
 )
 
 NetworkInsightsAccessScopeAnalysisTypeDef = TypedDict(
     "NetworkInsightsAccessScopeAnalysisTypeDef",
     {
         "NetworkInsightsAccessScopeAnalysisId": str,
         "NetworkInsightsAccessScopeAnalysisArn": str,
@@ -16370,42 +16066,39 @@
         "WarningMessage": str,
         "StartDate": datetime,
         "EndDate": datetime,
         "FindingsFound": FindingsFoundType,
         "AnalyzedEniCount": int,
         "Tags": List[TagTypeDef],
     },
-    total=False,
 )
 
 NetworkInsightsAccessScopeTypeDef = TypedDict(
     "NetworkInsightsAccessScopeTypeDef",
     {
         "NetworkInsightsAccessScopeId": str,
         "NetworkInsightsAccessScopeArn": str,
         "CreatedDate": datetime,
         "UpdatedDate": datetime,
         "Tags": List[TagTypeDef],
     },
-    total=False,
 )
 
 PlacementGroupTypeDef = TypedDict(
     "PlacementGroupTypeDef",
     {
         "GroupName": str,
         "State": PlacementGroupStateType,
         "Strategy": PlacementStrategyType,
         "PartitionCount": int,
         "GroupId": str,
         "Tags": List[TagTypeDef],
         "GroupArn": str,
         "SpreadLevel": SpreadLevelType,
     },
-    total=False,
 )
 
 ReplaceRootVolumeTaskTypeDef = TypedDict(
     "ReplaceRootVolumeTaskTypeDef",
     {
         "ReplaceRootVolumeTaskId": str,
         "InstanceId": str,
@@ -16413,15 +16106,14 @@
         "StartTime": str,
         "CompleteTime": str,
         "Tags": List[TagTypeDef],
         "ImageId": str,
         "SnapshotId": str,
         "DeleteReplacedRootVolume": bool,
     },
-    total=False,
 )
 
 SnapshotInfoTypeDef = TypedDict(
     "SnapshotInfoTypeDef",
     {
         "Description": str,
         "Tags": List[TagTypeDef],
@@ -16431,15 +16123,14 @@
         "VolumeSize": int,
         "StartTime": datetime,
         "Progress": str,
         "OwnerId": str,
         "SnapshotId": str,
         "OutpostArn": str,
     },
-    total=False,
 )
 
 SnapshotResponseMetadataTypeDef = TypedDict(
     "SnapshotResponseMetadataTypeDef",
     {
         "DataEncryptionKeyId": str,
         "Description": str,
@@ -16474,15 +16165,14 @@
         "LastTieringStartTime": datetime,
         "LastTieringProgress": int,
         "LastTieringOperationStatus": TieringOperationStatusType,
         "LastTieringOperationStatusDetail": str,
         "ArchivalCompleteTime": datetime,
         "RestoreExpiryTime": datetime,
     },
-    total=False,
 )
 
 SnapshotTypeDef = TypedDict(
     "SnapshotTypeDef",
     {
         "DataEncryptionKeyId": str,
         "Description": str,
@@ -16498,38 +16188,35 @@
         "VolumeSize": int,
         "OwnerAlias": str,
         "OutpostArn": str,
         "Tags": List[TagTypeDef],
         "StorageTier": StorageTierType,
         "RestoreExpiryTime": datetime,
     },
-    total=False,
 )
 
 SpotFleetTagSpecificationTypeDef = TypedDict(
     "SpotFleetTagSpecificationTypeDef",
     {
         "ResourceType": ResourceTypeType,
         "Tags": List[TagTypeDef],
     },
-    total=False,
 )
 
 SubnetCidrReservationTypeDef = TypedDict(
     "SubnetCidrReservationTypeDef",
     {
         "SubnetCidrReservationId": str,
         "SubnetId": str,
         "Cidr": str,
         "ReservationType": SubnetCidrReservationTypeType,
         "OwnerId": str,
         "Description": str,
         "Tags": List[TagTypeDef],
     },
-    total=False,
 )
 
 TagSpecificationTypeDef = TypedDict(
     "TagSpecificationTypeDef",
     {
         "ResourceType": ResourceTypeType,
         "Tags": Sequence[TagTypeDef],
@@ -16547,42 +16234,39 @@
         "OwnerId": str,
         "PacketLength": int,
         "SessionNumber": int,
         "VirtualNetworkId": int,
         "Description": str,
         "Tags": List[TagTypeDef],
     },
-    total=False,
 )
 
 TrafficMirrorTargetTypeDef = TypedDict(
     "TrafficMirrorTargetTypeDef",
     {
         "TrafficMirrorTargetId": str,
         "NetworkInterfaceId": str,
         "NetworkLoadBalancerArn": str,
         "Type": TrafficMirrorTargetTypeType,
         "Description": str,
         "OwnerId": str,
         "Tags": List[TagTypeDef],
         "GatewayLoadBalancerEndpointId": str,
     },
-    total=False,
 )
 
 TransitGatewayPolicyTableTypeDef = TypedDict(
     "TransitGatewayPolicyTableTypeDef",
     {
         "TransitGatewayPolicyTableId": str,
         "TransitGatewayId": str,
         "State": TransitGatewayPolicyTableStateType,
         "CreationTime": datetime,
         "Tags": List[TagTypeDef],
     },
-    total=False,
 )
 
 TransitGatewayRouteTableAnnouncementTypeDef = TypedDict(
     "TransitGatewayRouteTableAnnouncementTypeDef",
     {
         "TransitGatewayRouteTableAnnouncementId": str,
         "TransitGatewayId": str,
@@ -16592,43 +16276,40 @@
         "PeeringAttachmentId": str,
         "AnnouncementDirection": TransitGatewayRouteTableAnnouncementDirectionType,
         "TransitGatewayRouteTableId": str,
         "State": TransitGatewayRouteTableAnnouncementStateType,
         "CreationTime": datetime,
         "Tags": List[TagTypeDef],
     },
-    total=False,
 )
 
 TransitGatewayRouteTableTypeDef = TypedDict(
     "TransitGatewayRouteTableTypeDef",
     {
         "TransitGatewayRouteTableId": str,
         "TransitGatewayId": str,
         "State": TransitGatewayRouteTableStateType,
         "DefaultAssociationRouteTable": bool,
         "DefaultPropagationRouteTable": bool,
         "CreationTime": datetime,
         "Tags": List[TagTypeDef],
     },
-    total=False,
 )
 
 TrunkInterfaceAssociationTypeDef = TypedDict(
     "TrunkInterfaceAssociationTypeDef",
     {
         "AssociationId": str,
         "BranchInterfaceId": str,
         "TrunkInterfaceId": str,
         "InterfaceProtocol": InterfaceProtocolTypeType,
         "VlanId": int,
         "GreKey": int,
         "Tags": List[TagTypeDef],
     },
-    total=False,
 )
 
 VerifiedAccessGroupTypeDef = TypedDict(
     "VerifiedAccessGroupTypeDef",
     {
         "VerifiedAccessGroupId": str,
         "VerifiedAccessInstanceId": str,
@@ -16636,25 +16317,23 @@
         "Owner": str,
         "VerifiedAccessGroupArn": str,
         "CreationTime": str,
         "LastUpdatedTime": str,
         "DeletionTime": str,
         "Tags": List[TagTypeDef],
     },
-    total=False,
 )
 
 VpcClassicLinkTypeDef = TypedDict(
     "VpcClassicLinkTypeDef",
     {
         "ClassicLinkEnabled": bool,
         "Tags": List[TagTypeDef],
         "VpcId": str,
     },
-    total=False,
 )
 
 _RequiredVpcCreateTagsRequestTypeDef = TypedDict(
     "_RequiredVpcCreateTagsRequestTypeDef",
     {
         "Tags": Sequence[TagTypeDef],
     },
@@ -16746,70 +16425,65 @@
         "Cidr": str,
         "Egress": bool,
         "PortRange": PortRangeTypeDef,
         "Protocol": str,
         "RuleAction": str,
         "RuleNumber": int,
     },
-    total=False,
 )
 
 AnalysisPacketHeaderTypeDef = TypedDict(
     "AnalysisPacketHeaderTypeDef",
     {
         "DestinationAddresses": List[str],
         "DestinationPortRanges": List[PortRangeTypeDef],
         "Protocol": str,
         "SourceAddresses": List[str],
         "SourcePortRanges": List[PortRangeTypeDef],
     },
-    total=False,
 )
 
 AnalysisSecurityGroupRuleTypeDef = TypedDict(
     "AnalysisSecurityGroupRuleTypeDef",
     {
         "Cidr": str,
         "Direction": str,
         "SecurityGroupId": str,
         "PortRange": PortRangeTypeDef,
         "PrefixListId": str,
         "Protocol": str,
     },
-    total=False,
 )
 
 FirewallStatefulRuleTypeDef = TypedDict(
     "FirewallStatefulRuleTypeDef",
     {
         "RuleGroupArn": str,
         "Sources": List[str],
         "Destinations": List[str],
         "SourcePorts": List[PortRangeTypeDef],
         "DestinationPorts": List[PortRangeTypeDef],
         "Protocol": str,
         "RuleAction": str,
         "Direction": str,
     },
-    total=False,
 )
 
 FirewallStatelessRuleTypeDef = TypedDict(
     "FirewallStatelessRuleTypeDef",
     {
         "RuleGroupArn": str,
         "Sources": List[str],
         "Destinations": List[str],
         "SourcePorts": List[PortRangeTypeDef],
         "DestinationPorts": List[PortRangeTypeDef],
         "Protocols": List[int],
         "RuleAction": str,
         "Priority": int,
     },
-    total=False,
 )
 
 AssignPrivateIpAddressesResultTypeDef = TypedDict(
     "AssignPrivateIpAddressesResultTypeDef",
     {
         "NetworkInterfaceId": str,
         "AssignedPrivateIpAddresses": List[AssignedPrivateIpAddressTypeDef],
@@ -16878,15 +16552,14 @@
         "AssociationId": str,
         "VpcId": str,
         "TargetNetworkId": str,
         "ClientVpnEndpointId": str,
         "Status": AssociationStatusTypeDef,
         "SecurityGroups": List[str],
     },
-    total=False,
 )
 
 AssociateIamInstanceProfileRequestRequestTypeDef = TypedDict(
     "AssociateIamInstanceProfileRequestRequestTypeDef",
     {
         "IamInstanceProfile": IamInstanceProfileSpecificationTypeDef,
         "InstanceId": str,
@@ -16925,15 +16598,14 @@
         "Main": bool,
         "RouteTableAssociationId": str,
         "RouteTableId": str,
         "SubnetId": str,
         "GatewayId": str,
         "AssociationState": RouteTableAssociationStateTypeDef,
     },
-    total=False,
 )
 
 AssociateTransitGatewayPolicyTableResultTypeDef = TypedDict(
     "AssociateTransitGatewayPolicyTableResultTypeDef",
     {
         "Association": TransitGatewayPolicyTableAssociationTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
@@ -17004,24 +16676,22 @@
         "State": VpnStateType,
         "Type": Literal["ipsec.1"],
         "VpcAttachments": List[VpcAttachmentTypeDef],
         "VpnGatewayId": str,
         "AmazonSideAsn": int,
         "Tags": List[TagTypeDef],
     },
-    total=False,
 )
 
 AttachmentEnaSrdSpecificationTypeDef = TypedDict(
     "AttachmentEnaSrdSpecificationTypeDef",
     {
         "EnaSrdEnabled": bool,
         "EnaSrdUdpSpecification": AttachmentEnaSrdUdpSpecificationTypeDef,
     },
-    total=False,
 )
 
 DescribeVpcAttributeResultTypeDef = TypedDict(
     "DescribeVpcAttributeResultTypeDef",
     {
         "VpcId": str,
         "EnableDnsHostnames": AttributeBooleanValueTypeDef,
@@ -17130,28 +16800,26 @@
 
 DhcpConfigurationTypeDef = TypedDict(
     "DhcpConfigurationTypeDef",
     {
         "Key": str,
         "Values": List[AttributeValueTypeDef],
     },
-    total=False,
 )
 
 AuthorizationRuleTypeDef = TypedDict(
     "AuthorizationRuleTypeDef",
     {
         "ClientVpnEndpointId": str,
         "Description": str,
         "GroupId": str,
         "AccessAll": bool,
         "DestinationCidr": str,
         "Status": ClientVpnAuthorizationRuleStatusTypeDef,
     },
-    total=False,
 )
 
 AuthorizeClientVpnIngressResultTypeDef = TypedDict(
     "AuthorizeClientVpnIngressResultTypeDef",
     {
         "Status": ClientVpnAuthorizationRuleStatusTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
@@ -17177,24 +16845,22 @@
         "ZoneId": str,
         "GroupName": str,
         "NetworkBorderGroup": str,
         "ZoneType": str,
         "ParentZoneName": str,
         "ParentZoneId": str,
     },
-    total=False,
 )
 
 AvailableCapacityTypeDef = TypedDict(
     "AvailableCapacityTypeDef",
     {
         "AvailableInstanceCapacity": List[InstanceCapacityTypeDef],
         "AvailableVCpus": int,
     },
-    total=False,
 )
 
 BlockDeviceMappingTypeDef = TypedDict(
     "BlockDeviceMappingTypeDef",
     {
         "DeviceName": str,
         "VirtualName": str,
@@ -17206,24 +16872,22 @@
 
 FailedCapacityReservationFleetCancellationResultTypeDef = TypedDict(
     "FailedCapacityReservationFleetCancellationResultTypeDef",
     {
         "CapacityReservationFleetId": str,
         "CancelCapacityReservationFleetError": CancelCapacityReservationFleetErrorTypeDef,
     },
-    total=False,
 )
 
 CancelSpotFleetRequestsErrorItemTypeDef = TypedDict(
     "CancelSpotFleetRequestsErrorItemTypeDef",
     {
         "Error": CancelSpotFleetRequestsErrorTypeDef,
         "SpotFleetRequestId": str,
     },
-    total=False,
 )
 
 CancelSpotInstanceRequestsResultTypeDef = TypedDict(
     "CancelSpotInstanceRequestsResultTypeDef",
     {
         "CancelledSpotInstanceRequests": List[CancelledSpotInstanceRequestTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
@@ -17253,15 +16917,14 @@
         "CreateDate": datetime,
         "Tags": List[TagTypeDef],
         "OutpostArn": str,
         "CapacityReservationFleetId": str,
         "PlacementGroupArn": str,
         "CapacityAllocations": List[CapacityAllocationTypeDef],
     },
-    total=False,
 )
 
 CapacityReservationFleetTypeDef = TypedDict(
     "CapacityReservationFleetTypeDef",
     {
         "CapacityReservationFleetId": str,
         "CapacityReservationFleetArn": str,
@@ -17272,15 +16935,14 @@
         "EndDate": datetime,
         "CreateTime": datetime,
         "InstanceMatchCriteria": Literal["open"],
         "AllocationStrategy": str,
         "InstanceTypeSpecifications": List[FleetCapacityReservationTypeDef],
         "Tags": List[TagTypeDef],
     },
-    total=False,
 )
 
 CreateCapacityReservationFleetResultTypeDef = TypedDict(
     "CreateCapacityReservationFleetResultTypeDef",
     {
         "CapacityReservationFleetId": str,
         "State": CapacityReservationFleetStateType,
@@ -17325,15 +16987,14 @@
         "AllocationStrategy": FleetOnDemandAllocationStrategyType,
         "CapacityReservationOptions": CapacityReservationOptionsTypeDef,
         "SingleInstanceType": bool,
         "SingleAvailabilityZone": bool,
         "MinTargetCapacity": int,
         "MaxTotalPrice": str,
     },
-    total=False,
 )
 
 CapacityReservationSpecificationResponseResponseMetadataTypeDef = TypedDict(
     "CapacityReservationSpecificationResponseResponseMetadataTypeDef",
     {
         "CapacityReservationPreference": CapacityReservationPreferenceType,
         "CapacityReservationTarget": CapacityReservationTargetResponseTypeDef,
@@ -17343,24 +17004,22 @@
 
 CapacityReservationSpecificationResponseTypeDef = TypedDict(
     "CapacityReservationSpecificationResponseTypeDef",
     {
         "CapacityReservationPreference": CapacityReservationPreferenceType,
         "CapacityReservationTarget": CapacityReservationTargetResponseTypeDef,
     },
-    total=False,
 )
 
 LaunchTemplateCapacityReservationSpecificationResponseTypeDef = TypedDict(
     "LaunchTemplateCapacityReservationSpecificationResponseTypeDef",
     {
         "CapacityReservationPreference": CapacityReservationPreferenceType,
         "CapacityReservationTarget": CapacityReservationTargetResponseTypeDef,
     },
-    total=False,
 )
 
 CapacityReservationSpecificationTypeDef = TypedDict(
     "CapacityReservationSpecificationTypeDef",
     {
         "CapacityReservationPreference": CapacityReservationPreferenceType,
         "CapacityReservationTarget": CapacityReservationTargetTypeDef,
@@ -17390,23 +17049,21 @@
     "ClassicLinkInstanceTypeDef",
     {
         "Groups": List[GroupIdentifierTypeDef],
         "InstanceId": str,
         "Tags": List[TagTypeDef],
         "VpcId": str,
     },
-    total=False,
 )
 
 ClassicLoadBalancersConfigTypeDef = TypedDict(
     "ClassicLoadBalancersConfigTypeDef",
     {
         "ClassicLoadBalancers": List[ClassicLoadBalancerTypeDef],
     },
-    total=False,
 )
 
 ExportClientVpnClientCertificateRevocationListResultTypeDef = TypedDict(
     "ExportClientVpnClientCertificateRevocationListResultTypeDef",
     {
         "CertificateRevocationList": str,
         "Status": ClientCertificateRevocationListStatusTypeDef,
@@ -17417,15 +17074,14 @@
 ClientConnectResponseOptionsTypeDef = TypedDict(
     "ClientConnectResponseOptionsTypeDef",
     {
         "Enabled": bool,
         "LambdaFunctionArn": str,
         "Status": ClientVpnEndpointAttributeStatusTypeDef,
     },
-    total=False,
 )
 
 ClientVpnAuthenticationRequestTypeDef = TypedDict(
     "ClientVpnAuthenticationRequestTypeDef",
     {
         "Type": ClientVpnAuthenticationTypeType,
         "ActiveDirectory": DirectoryServiceAuthenticationRequestTypeDef,
@@ -17439,15 +17095,14 @@
     "ClientVpnAuthenticationTypeDef",
     {
         "Type": ClientVpnAuthenticationTypeType,
         "ActiveDirectory": DirectoryServiceAuthenticationTypeDef,
         "MutualAuthentication": CertificateAuthenticationTypeDef,
         "FederatedAuthentication": FederatedAuthenticationTypeDef,
     },
-    total=False,
 )
 
 ClientVpnConnectionTypeDef = TypedDict(
     "ClientVpnConnectionTypeDef",
     {
         "ClientVpnEndpointId": str,
         "Timestamp": str,
@@ -17460,25 +17115,23 @@
         "EgressPackets": str,
         "ClientIp": str,
         "CommonName": str,
         "Status": ClientVpnConnectionStatusTypeDef,
         "ConnectionEndTime": str,
         "PostureComplianceStatuses": List[str],
     },
-    total=False,
 )
 
 TerminateConnectionStatusTypeDef = TypedDict(
     "TerminateConnectionStatusTypeDef",
     {
         "ConnectionId": str,
         "PreviousStatus": ClientVpnConnectionStatusTypeDef,
         "CurrentStatus": ClientVpnConnectionStatusTypeDef,
     },
-    total=False,
 )
 
 CreateClientVpnEndpointResultTypeDef = TypedDict(
     "CreateClientVpnEndpointResultTypeDef",
     {
         "ClientVpnEndpointId": str,
         "Status": ClientVpnEndpointStatusTypeDef,
@@ -17502,15 +17155,14 @@
         "DestinationCidr": str,
         "TargetSubnet": str,
         "Type": str,
         "Origin": str,
         "Status": ClientVpnRouteStatusTypeDef,
         "Description": str,
     },
-    total=False,
 )
 
 CreateClientVpnRouteResultTypeDef = TypedDict(
     "CreateClientVpnRouteResultTypeDef",
     {
         "Status": ClientVpnRouteStatusTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
@@ -17534,15 +17186,14 @@
 )
 
 VpnTunnelLogOptionsTypeDef = TypedDict(
     "VpnTunnelLogOptionsTypeDef",
     {
         "CloudWatchLogOptions": CloudWatchLogOptionsTypeDef,
     },
-    total=False,
 )
 
 GetCoipPoolUsageResultTypeDef = TypedDict(
     "GetCoipPoolUsageResultTypeDef",
     {
         "CoipPoolId": str,
         "CoipAddressUsages": List[CoipAddressUsageTypeDef],
@@ -17739,15 +17390,14 @@
         "IcmpTypeCode": IcmpTypeCodeTypeDef,
         "Ipv6CidrBlock": str,
         "PortRange": PortRangeTypeDef,
         "Protocol": str,
         "RuleAction": RuleActionType,
         "RuleNumber": int,
     },
-    total=False,
 )
 
 _RequiredReplaceNetworkAclEntryRequestNetworkAclReplaceEntryTypeDef = TypedDict(
     "_RequiredReplaceNetworkAclEntryRequestNetworkAclReplaceEntryTypeDef",
     {
         "Egress": bool,
         "Protocol": str,
@@ -17824,15 +17474,14 @@
         "InterfaceType": str,
         "NetworkCardIndex": int,
         "Ipv4Prefixes": List[Ipv4PrefixSpecificationRequestTypeDef],
         "Ipv4PrefixCount": int,
         "Ipv6Prefixes": List[Ipv6PrefixSpecificationRequestTypeDef],
         "Ipv6PrefixCount": int,
     },
-    total=False,
 )
 
 CreateReservedInstancesListingRequestRequestTypeDef = TypedDict(
     "CreateReservedInstancesListingRequestRequestTypeDef",
     {
         "ClientToken": str,
         "InstanceCount": int,
@@ -18002,24 +17651,22 @@
         "Source": str,
         "Destination": str,
         "Metric": Literal["aggregate-latency"],
         "Statistic": Literal["p50"],
         "Period": PeriodTypeType,
         "MetricPoints": List[MetricPointTypeDef],
     },
-    total=False,
 )
 
 DeleteFleetErrorItemTypeDef = TypedDict(
     "DeleteFleetErrorItemTypeDef",
     {
         "Error": DeleteFleetErrorTypeDef,
         "FleetId": str,
     },
-    total=False,
 )
 
 DeleteInstanceEventWindowResultTypeDef = TypedDict(
     "DeleteInstanceEventWindowResultTypeDef",
     {
         "InstanceEventWindowState": InstanceEventWindowStateChangeTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
@@ -18030,24 +17677,22 @@
     "DeleteLaunchTemplateVersionsResponseErrorItemTypeDef",
     {
         "LaunchTemplateId": str,
         "LaunchTemplateName": str,
         "VersionNumber": int,
         "ResponseError": ResponseErrorTypeDef,
     },
-    total=False,
 )
 
 FailedQueuedPurchaseDeletionTypeDef = TypedDict(
     "FailedQueuedPurchaseDeletionTypeDef",
     {
         "Error": DeleteQueuedReservedInstancesErrorTypeDef,
         "ReservedInstancesId": str,
     },
-    total=False,
 )
 
 _RequiredDeregisterInstanceEventNotificationAttributesRequestRequestTypeDef = TypedDict(
     "_RequiredDeregisterInstanceEventNotificationAttributesRequestRequestTypeDef",
     {
         "InstanceTagAttribute": DeregisterInstanceTagAttributeRequestTypeDef,
     },
@@ -21655,15 +21300,14 @@
 
 PrincipalIdFormatTypeDef = TypedDict(
     "PrincipalIdFormatTypeDef",
     {
         "Arn": str,
         "Statuses": List[IdFormatTypeDef],
     },
-    total=False,
 )
 
 DescribeAwsNetworkPerformanceMetricSubscriptionsResultTypeDef = TypedDict(
     "DescribeAwsNetworkPerformanceMetricSubscriptionsResultTypeDef",
     {
         "NextToken": str,
         "Subscriptions": List[SubscriptionTypeDef],
@@ -22133,15 +21777,14 @@
         "LaunchTemplate": FastLaunchLaunchTemplateSpecificationResponseTypeDef,
         "MaxParallelLaunches": int,
         "OwnerId": str,
         "State": FastLaunchStateCodeType,
         "StateTransitionReason": str,
         "StateTransitionTime": datetime,
     },
-    total=False,
 )
 
 DisableFastLaunchResultTypeDef = TypedDict(
     "DisableFastLaunchResultTypeDef",
     {
         "ImageId": str,
         "ResourceType": Literal["snapshot"],
@@ -22402,24 +22045,22 @@
         "LogDestinationType": LogDestinationTypeType,
         "LogDestination": str,
         "LogFormat": str,
         "Tags": List[TagTypeDef],
         "MaxAggregationInterval": int,
         "DestinationOptions": DestinationOptionsResponseTypeDef,
     },
-    total=False,
 )
 
 DisableFastSnapshotRestoreStateErrorItemTypeDef = TypedDict(
     "DisableFastSnapshotRestoreStateErrorItemTypeDef",
     {
         "AvailabilityZone": str,
         "Error": DisableFastSnapshotRestoreStateErrorTypeDef,
     },
-    total=False,
 )
 
 DisableTransitGatewayRouteTablePropagationResultTypeDef = TypedDict(
     "DisableTransitGatewayRouteTablePropagationResultTypeDef",
     {
         "Propagation": TransitGatewayPropagationTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
@@ -22475,38 +22116,35 @@
         "BytesConverted": int,
         "Description": str,
         "Image": DiskImageDescriptionTypeDef,
         "Status": str,
         "StatusMessage": str,
         "Volume": DiskImageVolumeDescriptionTypeDef,
     },
-    total=False,
 )
 
 ImportVolumeTaskDetailsTypeDef = TypedDict(
     "ImportVolumeTaskDetailsTypeDef",
     {
         "AvailabilityZone": str,
         "BytesConverted": int,
         "Description": str,
         "Image": DiskImageDescriptionTypeDef,
         "Volume": DiskImageVolumeDescriptionTypeDef,
     },
-    total=False,
 )
 
 InstanceStorageInfoTypeDef = TypedDict(
     "InstanceStorageInfoTypeDef",
     {
         "TotalSizeInGB": int,
         "Disks": List[DiskInfoTypeDef],
         "NvmeSupport": EphemeralNvmeSupportType,
         "EncryptionSupport": InstanceStorageEncryptionSupportType,
     },
-    total=False,
 )
 
 VpcEndpointConnectionTypeDef = TypedDict(
     "VpcEndpointConnectionTypeDef",
     {
         "ServiceId": str,
         "VpcEndpointId": str,
@@ -22516,15 +22154,14 @@
         "DnsEntries": List[DnsEntryTypeDef],
         "NetworkLoadBalancerArns": List[str],
         "GatewayLoadBalancerArns": List[str],
         "IpAddressType": IpAddressTypeType,
         "VpcEndpointConnectionId": str,
         "Tags": List[TagTypeDef],
     },
-    total=False,
 )
 
 _RequiredModifyClientVpnEndpointRequestRequestTypeDef = TypedDict(
     "_RequiredModifyClientVpnEndpointRequestRequestTypeDef",
     {
         "ClientVpnEndpointId": str,
     },
@@ -22561,15 +22198,14 @@
     "EbsInfoTypeDef",
     {
         "EbsOptimizedSupport": EbsOptimizedSupportType,
         "EncryptionSupport": EbsEncryptionSupportType,
         "EbsOptimizedInfo": EbsOptimizedInfoTypeDef,
         "NvmeSupport": EbsNvmeSupportType,
     },
-    total=False,
 )
 
 InstanceBlockDeviceMappingSpecificationTypeDef = TypedDict(
     "InstanceBlockDeviceMappingSpecificationTypeDef",
     {
         "DeviceName": str,
         "Ebs": EbsInstanceBlockDeviceSpecificationTypeDef,
@@ -22581,50 +22217,46 @@
 
 InstanceBlockDeviceMappingTypeDef = TypedDict(
     "InstanceBlockDeviceMappingTypeDef",
     {
         "DeviceName": str,
         "Ebs": EbsInstanceBlockDeviceTypeDef,
     },
-    total=False,
 )
 
 EgressOnlyInternetGatewayTypeDef = TypedDict(
     "EgressOnlyInternetGatewayTypeDef",
     {
         "Attachments": List[InternetGatewayAttachmentTypeDef],
         "EgressOnlyInternetGatewayId": str,
         "Tags": List[TagTypeDef],
     },
-    total=False,
 )
 
 InternetGatewayTypeDef = TypedDict(
     "InternetGatewayTypeDef",
     {
         "Attachments": List[InternetGatewayAttachmentTypeDef],
         "InternetGatewayId": str,
         "OwnerId": str,
         "Tags": List[TagTypeDef],
     },
-    total=False,
 )
 
 ElasticGpusTypeDef = TypedDict(
     "ElasticGpusTypeDef",
     {
         "ElasticGpuId": str,
         "AvailabilityZone": str,
         "ElasticGpuType": str,
         "ElasticGpuHealth": ElasticGpuHealthTypeDef,
         "ElasticGpuState": Literal["ATTACHED"],
         "InstanceId": str,
         "Tags": List[TagTypeDef],
     },
-    total=False,
 )
 
 EnaSrdSpecificationTypeDef = TypedDict(
     "EnaSrdSpecificationTypeDef",
     {
         "EnaSrdEnabled": bool,
         "EnaSrdUdpSpecification": EnaSrdUdpSpecificationTypeDef,
@@ -22659,35 +22291,32 @@
 
 EnableFastSnapshotRestoreStateErrorItemTypeDef = TypedDict(
     "EnableFastSnapshotRestoreStateErrorItemTypeDef",
     {
         "AvailabilityZone": str,
         "Error": EnableFastSnapshotRestoreStateErrorTypeDef,
     },
-    total=False,
 )
 
 HistoryRecordEntryTypeDef = TypedDict(
     "HistoryRecordEntryTypeDef",
     {
         "EventInformation": EventInformationTypeDef,
         "EventType": FleetEventTypeType,
         "Timestamp": datetime,
     },
-    total=False,
 )
 
 HistoryRecordTypeDef = TypedDict(
     "HistoryRecordTypeDef",
     {
         "EventInformation": EventInformationTypeDef,
         "EventType": EventTypeType,
         "Timestamp": datetime,
     },
-    total=False,
 )
 
 ExportImageResultTypeDef = TypedDict(
     "ExportImageResultTypeDef",
     {
         "Description": str,
         "DiskImageFormat": DiskImageFormatType,
@@ -22711,40 +22340,37 @@
         "ImageId": str,
         "Progress": str,
         "S3ExportLocation": ExportTaskS3LocationTypeDef,
         "Status": str,
         "StatusMessage": str,
         "Tags": List[TagTypeDef],
     },
-    total=False,
 )
 
 ExportTaskTypeDef = TypedDict(
     "ExportTaskTypeDef",
     {
         "Description": str,
         "ExportTaskId": str,
         "ExportToS3Task": ExportToS3TaskTypeDef,
         "InstanceExportDetails": InstanceExportDetailsTypeDef,
         "State": ExportTaskStateType,
         "StatusMessage": str,
         "Tags": List[TagTypeDef],
     },
-    total=False,
 )
 
 PathFilterTypeDef = TypedDict(
     "PathFilterTypeDef",
     {
         "SourceAddress": str,
         "SourcePortRange": FilterPortRangeTypeDef,
         "DestinationAddress": str,
         "DestinationPortRange": FilterPortRangeTypeDef,
     },
-    total=False,
 )
 
 FleetSpotMaintenanceStrategiesRequestTypeDef = TypedDict(
     "FleetSpotMaintenanceStrategiesRequestTypeDef",
     {
         "CapacityRebalance": FleetSpotCapacityRebalanceRequestTypeDef,
     },
@@ -22752,38 +22378,35 @@
 )
 
 FleetSpotMaintenanceStrategiesTypeDef = TypedDict(
     "FleetSpotMaintenanceStrategiesTypeDef",
     {
         "CapacityRebalance": FleetSpotCapacityRebalanceTypeDef,
     },
-    total=False,
 )
 
 FpgaDeviceInfoTypeDef = TypedDict(
     "FpgaDeviceInfoTypeDef",
     {
         "Name": str,
         "Manufacturer": str,
         "Count": int,
         "MemoryInfo": FpgaDeviceMemoryInfoTypeDef,
     },
-    total=False,
 )
 
 FpgaImageAttributeTypeDef = TypedDict(
     "FpgaImageAttributeTypeDef",
     {
         "FpgaImageId": str,
         "Name": str,
         "Description": str,
         "LoadPermissions": List[LoadPermissionTypeDef],
         "ProductCodes": List[ProductCodeTypeDef],
     },
-    total=False,
 )
 
 FpgaImageTypeDef = TypedDict(
     "FpgaImageTypeDef",
     {
         "FpgaImageId": str,
         "FpgaImageGlobalId": str,
@@ -22798,15 +22421,14 @@
         "OwnerAlias": str,
         "ProductCodes": List[ProductCodeTypeDef],
         "Tags": List[TagTypeDef],
         "Public": bool,
         "DataRetentionSupport": bool,
         "InstanceTypes": List[str],
     },
-    total=False,
 )
 
 GetAssociatedIpv6PoolCidrsResultTypeDef = TypedDict(
     "GetAssociatedIpv6PoolCidrsResultTypeDef",
     {
         "Ipv6CidrAssociations": List[Ipv6CidrAssociationTypeDef],
         "NextToken": str,
@@ -22905,15 +22527,14 @@
 
 ReservedInstanceReservationValueTypeDef = TypedDict(
     "ReservedInstanceReservationValueTypeDef",
     {
         "ReservationValue": ReservationValueTypeDef,
         "ReservedInstanceId": str,
     },
-    total=False,
 )
 
 GetSpotPlacementScoresResultTypeDef = TypedDict(
     "GetSpotPlacementScoresResultTypeDef",
     {
         "SpotPlacementScores": List[SpotPlacementScoreTypeDef],
         "NextToken": str,
@@ -22974,27 +22595,25 @@
     "GpuDeviceInfoTypeDef",
     {
         "Name": str,
         "Manufacturer": str,
         "Count": int,
         "MemoryInfo": GpuDeviceMemoryInfoTypeDef,
     },
-    total=False,
 )
 
 IamInstanceProfileAssociationTypeDef = TypedDict(
     "IamInstanceProfileAssociationTypeDef",
     {
         "AssociationId": str,
         "InstanceId": str,
         "IamInstanceProfile": IamInstanceProfileTypeDef,
         "State": IamInstanceProfileAssociationStateType,
         "Timestamp": datetime,
     },
-    total=False,
 )
 
 LaunchPermissionModificationsTypeDef = TypedDict(
     "LaunchPermissionModificationsTypeDef",
     {
         "Add": Sequence[LaunchPermissionTypeDef],
         "Remove": Sequence[LaunchPermissionTypeDef],
@@ -23044,15 +22663,14 @@
         "OutpostArn": str,
         "OwnerId": str,
         "State": str,
         "Tags": List[TagTypeDef],
         "Mode": LocalGatewayRouteTableModeType,
         "StateReason": StateReasonTypeDef,
     },
-    total=False,
 )
 
 ImportInstanceLaunchSpecificationTypeDef = TypedDict(
     "ImportInstanceLaunchSpecificationTypeDef",
     {
         "AdditionalInfo": str,
         "Architecture": ArchitectureValuesType,
@@ -23070,15 +22688,14 @@
 )
 
 InferenceAcceleratorInfoTypeDef = TypedDict(
     "InferenceAcceleratorInfoTypeDef",
     {
         "Accelerators": List[InferenceDeviceInfoTypeDef],
     },
-    total=False,
 )
 
 _RequiredModifyInstanceCreditSpecificationRequestRequestTypeDef = TypedDict(
     "_RequiredModifyInstanceCreditSpecificationRequestRequestTypeDef",
     {
         "InstanceCreditSpecifications": Sequence[InstanceCreditSpecificationRequestTypeDef],
     },
@@ -23146,26 +22763,24 @@
 
 InstanceMonitoringTypeDef = TypedDict(
     "InstanceMonitoringTypeDef",
     {
         "InstanceId": str,
         "Monitoring": MonitoringTypeDef,
     },
-    total=False,
 )
 
 InstancePrivateIpAddressTypeDef = TypedDict(
     "InstancePrivateIpAddressTypeDef",
     {
         "Association": InstanceNetworkInterfaceAssociationTypeDef,
         "Primary": bool,
         "PrivateDnsName": str,
         "PrivateIpAddress": str,
     },
-    total=False,
 )
 
 _RequiredInstanceRequirementsRequestTypeDef = TypedDict(
     "_RequiredInstanceRequirementsRequestTypeDef",
     {
         "VCpuCount": VCpuCountRangeRequestTypeDef,
         "MemoryMiB": MemoryMiBRequestTypeDef,
@@ -23229,34 +22844,31 @@
         "AcceleratorCount": AcceleratorCountTypeDef,
         "AcceleratorManufacturers": List[AcceleratorManufacturerType],
         "AcceleratorNames": List[AcceleratorNameType],
         "AcceleratorTotalMemoryMiB": AcceleratorTotalMemoryMiBTypeDef,
         "NetworkBandwidthGbps": NetworkBandwidthGbpsTypeDef,
         "AllowedInstanceTypes": List[str],
     },
-    total=False,
 )
 
 InstanceStateChangeTypeDef = TypedDict(
     "InstanceStateChangeTypeDef",
     {
         "CurrentState": InstanceStateTypeDef,
         "InstanceId": str,
         "PreviousState": InstanceStateTypeDef,
     },
-    total=False,
 )
 
 InstanceStatusSummaryTypeDef = TypedDict(
     "InstanceStatusSummaryTypeDef",
     {
         "Details": List[InstanceStatusDetailsTypeDef],
         "Status": SummaryStatusType,
     },
-    total=False,
 )
 
 ModifyInstanceEventStartTimeResultTypeDef = TypedDict(
     "ModifyInstanceEventStartTimeResultTypeDef",
     {
         "Event": InstanceStatusEventTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
@@ -23283,15 +22895,14 @@
         "FromPort": int,
         "IpProtocol": str,
         "IpRanges": List[str],
         "PrefixListIds": List[str],
         "ToPort": int,
         "UserIdGroupPairs": List[UserIdGroupPairTypeDef],
     },
-    total=False,
 )
 
 _RequiredProvisionIpamPoolCidrRequestRequestTypeDef = TypedDict(
     "_RequiredProvisionIpamPoolCidrRequestRequestTypeDef",
     {
         "IpamPoolId": str,
     },
@@ -23321,15 +22932,14 @@
     {
         "AccountId": str,
         "DiscoveryRegion": str,
         "FailureReason": IpamDiscoveryFailureReasonTypeDef,
         "LastAttemptedDiscoveryTime": datetime,
         "LastSuccessfulDiscoveryTime": datetime,
     },
-    total=False,
 )
 
 IpamDiscoveredResourceCidrTypeDef = TypedDict(
     "IpamDiscoveredResourceCidrTypeDef",
     {
         "IpamResourceDiscoveryId": str,
         "ResourceRegion": str,
@@ -23338,15 +22948,14 @@
         "ResourceCidr": str,
         "ResourceType": IpamResourceTypeType,
         "ResourceTags": List[IpamResourceTagTypeDef],
         "IpUsage": float,
         "VpcId": str,
         "SampleTime": datetime,
     },
-    total=False,
 )
 
 IpamPoolTypeDef = TypedDict(
     "IpamPoolTypeDef",
     {
         "OwnerId": str,
         "IpamPoolId": str,
@@ -23368,15 +22977,14 @@
         "AllocationMaxNetmaskLength": int,
         "AllocationDefaultNetmaskLength": int,
         "AllocationResourceTags": List[IpamResourceTagTypeDef],
         "Tags": List[TagTypeDef],
         "AwsService": Literal["ec2"],
         "PublicIpSource": IpamPoolPublicIpSourceType,
     },
-    total=False,
 )
 
 IpamResourceCidrTypeDef = TypedDict(
     "IpamResourceCidrTypeDef",
     {
         "IpamId": str,
         "IpamScopeId": str,
@@ -23390,15 +22998,14 @@
         "ResourceTags": List[IpamResourceTagTypeDef],
         "IpUsage": float,
         "ComplianceStatus": IpamComplianceStatusType,
         "ManagementState": IpamManagementStateType,
         "OverlapStatus": IpamOverlapStatusType,
         "VpcId": str,
     },
-    total=False,
 )
 
 IpamResourceDiscoveryTypeDef = TypedDict(
     "IpamResourceDiscoveryTypeDef",
     {
         "OwnerId": str,
         "IpamResourceDiscoveryId": str,
@@ -23406,15 +23013,14 @@
         "IpamResourceDiscoveryRegion": str,
         "Description": str,
         "OperatingRegions": List[IpamOperatingRegionTypeDef],
         "IsDefault": bool,
         "State": IpamResourceDiscoveryStateType,
         "Tags": List[TagTypeDef],
     },
-    total=False,
 )
 
 IpamTypeDef = TypedDict(
     "IpamTypeDef",
     {
         "OwnerId": str,
         "IpamId": str,
@@ -23427,38 +23033,35 @@
         "OperatingRegions": List[IpamOperatingRegionTypeDef],
         "State": IpamStateType,
         "Tags": List[TagTypeDef],
         "DefaultResourceDiscoveryId": str,
         "DefaultResourceDiscoveryAssociationId": str,
         "ResourceDiscoveryAssociationCount": int,
     },
-    total=False,
 )
 
 IpamPoolCidrTypeDef = TypedDict(
     "IpamPoolCidrTypeDef",
     {
         "Cidr": str,
         "State": IpamPoolCidrStateType,
         "FailureReason": IpamPoolCidrFailureReasonTypeDef,
         "IpamPoolCidrId": str,
         "NetmaskLength": int,
     },
-    total=False,
 )
 
 Ipv6PoolTypeDef = TypedDict(
     "Ipv6PoolTypeDef",
     {
         "PoolId": str,
         "Description": str,
         "PoolCidrBlocks": List[PoolCidrBlockTypeDef],
         "Tags": List[TagTypeDef],
     },
-    total=False,
 )
 
 LaunchTemplateInstanceNetworkInterfaceSpecificationTypeDef = TypedDict(
     "LaunchTemplateInstanceNetworkInterfaceSpecificationTypeDef",
     {
         "AssociateCarrierIpAddress": bool,
         "AssociatePublicIpAddress": bool,
@@ -23476,15 +23079,14 @@
         "SubnetId": str,
         "NetworkCardIndex": int,
         "Ipv4Prefixes": List[Ipv4PrefixSpecificationResponseTypeDef],
         "Ipv4PrefixCount": int,
         "Ipv6Prefixes": List[Ipv6PrefixSpecificationResponseTypeDef],
         "Ipv6PrefixCount": int,
     },
-    total=False,
 )
 
 LaunchTemplateBlockDeviceMappingRequestTypeDef = TypedDict(
     "LaunchTemplateBlockDeviceMappingRequestTypeDef",
     {
         "DeviceName": str,
         "VirtualName": str,
@@ -23498,15 +23100,14 @@
     "LaunchTemplateBlockDeviceMappingTypeDef",
     {
         "DeviceName": str,
         "VirtualName": str,
         "Ebs": LaunchTemplateEbsBlockDeviceTypeDef,
         "NoDevice": str,
     },
-    total=False,
 )
 
 LaunchTemplateInstanceMarketOptionsRequestTypeDef = TypedDict(
     "LaunchTemplateInstanceMarketOptionsRequestTypeDef",
     {
         "MarketType": Literal["spot"],
         "SpotOptions": LaunchTemplateSpotMarketOptionsRequestTypeDef,
@@ -23516,15 +23117,14 @@
 
 LaunchTemplateInstanceMarketOptionsTypeDef = TypedDict(
     "LaunchTemplateInstanceMarketOptionsTypeDef",
     {
         "MarketType": Literal["spot"],
         "SpotOptions": LaunchTemplateSpotMarketOptionsTypeDef,
     },
-    total=False,
 )
 
 ListSnapshotsInRecycleBinResultTypeDef = TypedDict(
     "ListSnapshotsInRecycleBinResultTypeDef",
     {
         "Snapshots": List[SnapshotRecycleBinInfoTypeDef],
         "NextToken": str,
@@ -23642,15 +23242,14 @@
 
 ReservedInstancesModificationResultTypeDef = TypedDict(
     "ReservedInstancesModificationResultTypeDef",
     {
         "ReservedInstancesId": str,
         "TargetConfiguration": ReservedInstancesConfigurationTypeDef,
     },
-    total=False,
 )
 
 _RequiredModifyTransitGatewayRequestRequestTypeDef = TypedDict(
     "_RequiredModifyTransitGatewayRequestRequestTypeDef",
     {
         "TransitGatewayId": str,
     },
@@ -23795,15 +23394,14 @@
         "ProvisionedBandwidth": ProvisionedBandwidthTypeDef,
         "State": NatGatewayStateType,
         "SubnetId": str,
         "VpcId": str,
         "Tags": List[TagTypeDef],
         "ConnectivityType": ConnectivityTypeType,
     },
-    total=False,
 )
 
 NetworkInfoTypeDef = TypedDict(
     "NetworkInfoTypeDef",
     {
         "NetworkPerformance": str,
         "MaximumNetworkInterfaces": int,
@@ -23815,39 +23413,36 @@
         "Ipv6Supported": bool,
         "EnaSupport": EnaSupportType,
         "EfaSupported": bool,
         "EfaInfo": EfaInfoTypeDef,
         "EncryptionInTransitSupported": bool,
         "EnaSrdSupported": bool,
     },
-    total=False,
 )
 
 NetworkInterfacePrivateIpAddressTypeDef = TypedDict(
     "NetworkInterfacePrivateIpAddressTypeDef",
     {
         "Association": NetworkInterfaceAssociationTypeDef,
         "Primary": bool,
         "PrivateDnsName": str,
         "PrivateIpAddress": str,
     },
-    total=False,
 )
 
 NetworkInterfacePermissionTypeDef = TypedDict(
     "NetworkInterfacePermissionTypeDef",
     {
         "NetworkInterfacePermissionId": str,
         "NetworkInterfaceId": str,
         "AwsAccountId": str,
         "AwsService": str,
         "Permission": InterfacePermissionTypeType,
         "PermissionState": NetworkInterfacePermissionStateTypeDef,
     },
-    total=False,
 )
 
 VerifiedAccessTrustProviderTypeDef = TypedDict(
     "VerifiedAccessTrustProviderTypeDef",
     {
         "VerifiedAccessTrustProviderId": str,
         "Description": str,
@@ -23857,15 +23452,14 @@
         "OidcOptions": OidcOptionsTypeDef,
         "DeviceOptions": DeviceOptionsTypeDef,
         "PolicyReferenceName": str,
         "CreationTime": str,
         "LastUpdatedTime": str,
         "Tags": List[TagTypeDef],
     },
-    total=False,
 )
 
 PathRequestFilterTypeDef = TypedDict(
     "PathRequestFilterTypeDef",
     {
         "SourceAddress": str,
         "SourcePortRange": RequestFilterPortRangeTypeDef,
@@ -23894,23 +23488,21 @@
 
 PathStatementTypeDef = TypedDict(
     "PathStatementTypeDef",
     {
         "PacketHeaderStatement": PacketHeaderStatementTypeDef,
         "ResourceStatement": ResourceStatementTypeDef,
     },
-    total=False,
 )
 
 ThroughResourcesStatementTypeDef = TypedDict(
     "ThroughResourcesStatementTypeDef",
     {
         "ResourceStatement": ResourceStatementTypeDef,
     },
-    total=False,
 )
 
 ReservedInstancesListingTypeDef = TypedDict(
     "ReservedInstancesListingTypeDef",
     {
         "ClientToken": str,
         "CreateDate": datetime,
@@ -23919,15 +23511,14 @@
         "ReservedInstancesId": str,
         "ReservedInstancesListingId": str,
         "Status": ListingStatusType,
         "StatusMessage": str,
         "Tags": List[TagTypeDef],
         "UpdateDate": datetime,
     },
-    total=False,
 )
 
 ProvisionPublicIpv4PoolCidrResultTypeDef = TypedDict(
     "ProvisionPublicIpv4PoolCidrResultTypeDef",
     {
         "PoolId": str,
         "PoolAddressRange": PublicIpv4PoolRangeTypeDef,
@@ -23942,15 +23533,14 @@
         "Description": str,
         "PoolAddressRanges": List[PublicIpv4PoolRangeTypeDef],
         "TotalAddressCount": int,
         "TotalAvailableAddressCount": int,
         "NetworkBorderGroup": str,
         "Tags": List[TagTypeDef],
     },
-    total=False,
 )
 
 _RequiredPurchaseScheduledInstancesRequestRequestTypeDef = TypedDict(
     "_RequiredPurchaseScheduledInstancesRequestRequestTypeDef",
     {
         "PurchaseRequests": Sequence[PurchaseRequestTypeDef],
     },
@@ -24012,15 +23602,14 @@
         "Marketplace": bool,
         "OfferingClass": OfferingClassTypeType,
         "OfferingType": OfferingTypeValuesType,
         "PricingDetails": List[PricingDetailTypeDef],
         "RecurringCharges": List[RecurringChargeTypeDef],
         "Scope": scopeType,
     },
-    total=False,
 )
 
 ReservedInstancesTypeDef = TypedDict(
     "ReservedInstancesTypeDef",
     {
         "AvailabilityZone": str,
         "Duration": int,
@@ -24037,15 +23626,14 @@
         "InstanceTenancy": TenancyType,
         "OfferingClass": OfferingClassTypeType,
         "OfferingType": OfferingTypeValuesType,
         "RecurringCharges": List[RecurringChargeTypeDef],
         "Scope": scopeType,
         "Tags": List[TagTypeDef],
     },
-    total=False,
 )
 
 SecurityGroupRuleTypeDef = TypedDict(
     "SecurityGroupRuleTypeDef",
     {
         "SecurityGroupRuleId": str,
         "GroupId": str,
@@ -24057,15 +23645,14 @@
         "CidrIpv4": str,
         "CidrIpv6": str,
         "PrefixListId": str,
         "ReferencedGroupInfo": ReferencedSecurityGroupTypeDef,
         "Description": str,
         "Tags": List[TagTypeDef],
     },
-    total=False,
 )
 
 _RequiredRegisterInstanceEventNotificationAttributesRequestRequestTypeDef = TypedDict(
     "_RequiredRegisterInstanceEventNotificationAttributesRequestRequestTypeDef",
     {
         "InstanceTagAttribute": RegisterInstanceTagAttributeRequestTypeDef,
     },
@@ -24123,15 +23710,14 @@
         "NetworkPlatform": str,
         "Platform": str,
         "PurchaseToken": str,
         "Recurrence": ScheduledInstanceRecurrenceTypeDef,
         "SlotDurationInHours": int,
         "TotalScheduledInstanceHours": int,
     },
-    total=False,
 )
 
 ScheduledInstanceTypeDef = TypedDict(
     "ScheduledInstanceTypeDef",
     {
         "AvailabilityZone": str,
         "CreateDate": datetime,
@@ -24145,15 +23731,14 @@
         "Recurrence": ScheduledInstanceRecurrenceTypeDef,
         "ScheduledInstanceId": str,
         "SlotDurationInHours": int,
         "TermEndDate": datetime,
         "TermStartDate": datetime,
         "TotalScheduledInstanceHours": int,
     },
-    total=False,
 )
 
 ScheduledInstancesBlockDeviceMappingTypeDef = TypedDict(
     "ScheduledInstancesBlockDeviceMappingTypeDef",
     {
         "DeviceName": str,
         "Ebs": ScheduledInstancesEbsTypeDef,
@@ -24210,15 +23795,14 @@
         "NetworkInterfaceIds": List[str],
         "DnsEntries": List[DnsEntryTypeDef],
         "CreationTimestamp": datetime,
         "Tags": List[TagTypeDef],
         "OwnerId": str,
         "LastError": LastErrorTypeDef,
     },
-    total=False,
 )
 
 _RequiredSecurityGroupRuleUpdateTypeDef = TypedDict(
     "_RequiredSecurityGroupRuleUpdateTypeDef",
     {
         "SecurityGroupRuleId": str,
     },
@@ -24253,15 +23837,14 @@
         "SupportedIpAddressTypes": List[ServiceConnectivityTypeType],
         "BaseEndpointDnsNames": List[str],
         "PrivateDnsName": str,
         "PrivateDnsNameConfiguration": PrivateDnsNameConfigurationTypeDef,
         "PayerResponsibility": Literal["ServiceOwner"],
         "Tags": List[TagTypeDef],
     },
-    total=False,
 )
 
 ServiceDetailTypeDef = TypedDict(
     "ServiceDetailTypeDef",
     {
         "ServiceName": str,
         "ServiceId": str,
@@ -24275,15 +23858,14 @@
         "AcceptanceRequired": bool,
         "ManagesVpcEndpoints": bool,
         "PayerResponsibility": Literal["ServiceOwner"],
         "Tags": List[TagTypeDef],
         "PrivateDnsNameVerificationState": DnsNameStateType,
         "SupportedIpAddressTypes": List[ServiceConnectivityTypeType],
     },
-    total=False,
 )
 
 SnapshotDetailTypeDef = TypedDict(
     "SnapshotDetailTypeDef",
     {
         "Description": str,
         "DeviceName": str,
@@ -24292,15 +23874,14 @@
         "Progress": str,
         "SnapshotId": str,
         "Status": str,
         "StatusMessage": str,
         "Url": str,
         "UserBucket": UserBucketDetailsTypeDef,
     },
-    total=False,
 )
 
 SnapshotTaskDetailTypeDef = TypedDict(
     "SnapshotTaskDetailTypeDef",
     {
         "Description": str,
         "DiskImageSize": float,
@@ -24310,87 +23891,79 @@
         "Progress": str,
         "SnapshotId": str,
         "Status": str,
         "StatusMessage": str,
         "Url": str,
         "UserBucket": UserBucketDetailsTypeDef,
     },
-    total=False,
 )
 
 SpotMaintenanceStrategiesTypeDef = TypedDict(
     "SpotMaintenanceStrategiesTypeDef",
     {
         "CapacityRebalance": SpotCapacityRebalanceTypeDef,
     },
-    total=False,
 )
 
 SpotDatafeedSubscriptionTypeDef = TypedDict(
     "SpotDatafeedSubscriptionTypeDef",
     {
         "Bucket": str,
         "Fault": SpotInstanceStateFaultTypeDef,
         "OwnerId": str,
         "Prefix": str,
         "State": DatafeedSubscriptionStateType,
     },
-    total=False,
 )
 
 TransitGatewayMulticastDomainAssociationTypeDef = TypedDict(
     "TransitGatewayMulticastDomainAssociationTypeDef",
     {
         "TransitGatewayAttachmentId": str,
         "ResourceId": str,
         "ResourceType": TransitGatewayAttachmentResourceTypeType,
         "ResourceOwnerId": str,
         "Subnet": SubnetAssociationTypeDef,
     },
-    total=False,
 )
 
 TransitGatewayMulticastDomainAssociationsTypeDef = TypedDict(
     "TransitGatewayMulticastDomainAssociationsTypeDef",
     {
         "TransitGatewayMulticastDomainId": str,
         "TransitGatewayAttachmentId": str,
         "ResourceId": str,
         "ResourceType": TransitGatewayAttachmentResourceTypeType,
         "ResourceOwnerId": str,
         "Subnets": List[SubnetAssociationTypeDef],
     },
-    total=False,
 )
 
 SubnetIpv6CidrBlockAssociationTypeDef = TypedDict(
     "SubnetIpv6CidrBlockAssociationTypeDef",
     {
         "AssociationId": str,
         "Ipv6CidrBlock": str,
         "Ipv6CidrBlockState": SubnetCidrBlockStateTypeDef,
     },
-    total=False,
 )
 
 TargetReservationValueTypeDef = TypedDict(
     "TargetReservationValueTypeDef",
     {
         "ReservationValue": ReservationValueTypeDef,
         "TargetConfiguration": TargetConfigurationTypeDef,
     },
-    total=False,
 )
 
 TargetGroupsConfigTypeDef = TypedDict(
     "TargetGroupsConfigTypeDef",
     {
         "TargetGroups": List[TargetGroupTypeDef],
     },
-    total=False,
 )
 
 TrafficMirrorFilterRuleTypeDef = TypedDict(
     "TrafficMirrorFilterRuleTypeDef",
     {
         "TrafficMirrorFilterRuleId": str,
         "TrafficMirrorFilterId": str,
@@ -24400,15 +23973,14 @@
         "Protocol": int,
         "DestinationPortRange": TrafficMirrorPortRangeTypeDef,
         "SourcePortRange": TrafficMirrorPortRangeTypeDef,
         "DestinationCidrBlock": str,
         "SourceCidrBlock": str,
         "Description": str,
     },
-    total=False,
 )
 
 TransitGatewayAttachmentTypeDef = TypedDict(
     "TransitGatewayAttachmentTypeDef",
     {
         "TransitGatewayAttachmentId": str,
         "TransitGatewayId": str,
@@ -24417,71 +23989,66 @@
         "ResourceType": TransitGatewayAttachmentResourceTypeType,
         "ResourceId": str,
         "State": TransitGatewayAttachmentStateType,
         "Association": TransitGatewayAttachmentAssociationTypeDef,
         "CreationTime": datetime,
         "Tags": List[TagTypeDef],
     },
-    total=False,
 )
 
 TransitGatewayConnectPeerConfigurationTypeDef = TypedDict(
     "TransitGatewayConnectPeerConfigurationTypeDef",
     {
         "TransitGatewayAddress": str,
         "PeerAddress": str,
         "InsideCidrBlocks": List[str],
         "Protocol": Literal["gre"],
         "BgpConfigurations": List[TransitGatewayAttachmentBgpConfigurationTypeDef],
     },
-    total=False,
 )
 
 TransitGatewayConnectTypeDef = TypedDict(
     "TransitGatewayConnectTypeDef",
     {
         "TransitGatewayAttachmentId": str,
         "TransportTransitGatewayAttachmentId": str,
         "TransitGatewayId": str,
         "State": TransitGatewayAttachmentStateType,
         "CreationTime": datetime,
         "Options": TransitGatewayConnectOptionsTypeDef,
         "Tags": List[TagTypeDef],
     },
-    total=False,
 )
 
 TransitGatewayMulticastDomainTypeDef = TypedDict(
     "TransitGatewayMulticastDomainTypeDef",
     {
         "TransitGatewayMulticastDomainId": str,
         "TransitGatewayId": str,
         "TransitGatewayMulticastDomainArn": str,
         "OwnerId": str,
         "Options": TransitGatewayMulticastDomainOptionsTypeDef,
         "State": TransitGatewayMulticastDomainStateType,
         "CreationTime": datetime,
         "Tags": List[TagTypeDef],
     },
-    total=False,
 )
 
 TransitGatewayTypeDef = TypedDict(
     "TransitGatewayTypeDef",
     {
         "TransitGatewayId": str,
         "TransitGatewayArn": str,
         "State": TransitGatewayStateType,
         "OwnerId": str,
         "Description": str,
         "CreationTime": datetime,
         "Options": TransitGatewayOptionsTypeDef,
         "Tags": List[TagTypeDef],
     },
-    total=False,
 )
 
 TransitGatewayPeeringAttachmentTypeDef = TypedDict(
     "TransitGatewayPeeringAttachmentTypeDef",
     {
         "TransitGatewayAttachmentId": str,
         "AccepterTransitGatewayAttachmentId": str,
@@ -24489,54 +24056,50 @@
         "AccepterTgwInfo": PeeringTgwInfoTypeDef,
         "Options": TransitGatewayPeeringAttachmentOptionsTypeDef,
         "Status": PeeringAttachmentStatusTypeDef,
         "State": TransitGatewayAttachmentStateType,
         "CreationTime": datetime,
         "Tags": List[TagTypeDef],
     },
-    total=False,
 )
 
 TransitGatewayPolicyRuleTypeDef = TypedDict(
     "TransitGatewayPolicyRuleTypeDef",
     {
         "SourceCidrBlock": str,
         "SourcePortRange": str,
         "DestinationCidrBlock": str,
         "DestinationPortRange": str,
         "Protocol": str,
         "MetaData": TransitGatewayPolicyRuleMetaDataTypeDef,
     },
-    total=False,
 )
 
 TransitGatewayPrefixListReferenceTypeDef = TypedDict(
     "TransitGatewayPrefixListReferenceTypeDef",
     {
         "TransitGatewayRouteTableId": str,
         "PrefixListId": str,
         "PrefixListOwnerId": str,
         "State": TransitGatewayPrefixListReferenceStateType,
         "Blackhole": bool,
         "TransitGatewayAttachment": TransitGatewayPrefixListAttachmentTypeDef,
     },
-    total=False,
 )
 
 TransitGatewayRouteTypeDef = TypedDict(
     "TransitGatewayRouteTypeDef",
     {
         "DestinationCidrBlock": str,
         "PrefixListId": str,
         "TransitGatewayRouteTableAnnouncementId": str,
         "TransitGatewayAttachments": List[TransitGatewayRouteAttachmentTypeDef],
         "Type": TransitGatewayRouteTypeType,
         "State": TransitGatewayRouteStateType,
     },
-    total=False,
 )
 
 TransitGatewayVpcAttachmentTypeDef = TypedDict(
     "TransitGatewayVpcAttachmentTypeDef",
     {
         "TransitGatewayAttachmentId": str,
         "TransitGatewayId": str,
@@ -24544,41 +24107,37 @@
         "VpcOwnerId": str,
         "State": TransitGatewayAttachmentStateType,
         "SubnetIds": List[str],
         "CreationTime": datetime,
         "Options": TransitGatewayVpcAttachmentOptionsTypeDef,
         "Tags": List[TagTypeDef],
     },
-    total=False,
 )
 
 UnsuccessfulInstanceCreditSpecificationItemTypeDef = TypedDict(
     "UnsuccessfulInstanceCreditSpecificationItemTypeDef",
     {
         "InstanceId": str,
         "Error": UnsuccessfulInstanceCreditSpecificationItemErrorTypeDef,
     },
-    total=False,
 )
 
 UnsuccessfulItemTypeDef = TypedDict(
     "UnsuccessfulItemTypeDef",
     {
         "Error": UnsuccessfulItemErrorTypeDef,
         "ResourceId": str,
     },
-    total=False,
 )
 
 ValidationWarningTypeDef = TypedDict(
     "ValidationWarningTypeDef",
     {
         "Errors": List[ValidationErrorTypeDef],
     },
-    total=False,
 )
 
 VerifiedAccessEndpointTypeDef = TypedDict(
     "VerifiedAccessEndpointTypeDef",
     {
         "VerifiedAccessInstanceId": str,
         "VerifiedAccessGroupId": str,
@@ -24595,60 +24154,55 @@
         "Status": VerifiedAccessEndpointStatusTypeDef,
         "Description": str,
         "CreationTime": str,
         "LastUpdatedTime": str,
         "DeletionTime": str,
         "Tags": List[TagTypeDef],
     },
-    total=False,
 )
 
 VerifiedAccessInstanceTypeDef = TypedDict(
     "VerifiedAccessInstanceTypeDef",
     {
         "VerifiedAccessInstanceId": str,
         "Description": str,
         "VerifiedAccessTrustProviders": List[VerifiedAccessTrustProviderCondensedTypeDef],
         "CreationTime": str,
         "LastUpdatedTime": str,
         "Tags": List[TagTypeDef],
     },
-    total=False,
 )
 
 VerifiedAccessLogCloudWatchLogsDestinationTypeDef = TypedDict(
     "VerifiedAccessLogCloudWatchLogsDestinationTypeDef",
     {
         "Enabled": bool,
         "DeliveryStatus": VerifiedAccessLogDeliveryStatusTypeDef,
         "LogGroup": str,
     },
-    total=False,
 )
 
 VerifiedAccessLogKinesisDataFirehoseDestinationTypeDef = TypedDict(
     "VerifiedAccessLogKinesisDataFirehoseDestinationTypeDef",
     {
         "Enabled": bool,
         "DeliveryStatus": VerifiedAccessLogDeliveryStatusTypeDef,
         "DeliveryStream": str,
     },
-    total=False,
 )
 
 VerifiedAccessLogS3DestinationTypeDef = TypedDict(
     "VerifiedAccessLogS3DestinationTypeDef",
     {
         "Enabled": bool,
         "DeliveryStatus": VerifiedAccessLogDeliveryStatusTypeDef,
         "BucketName": str,
         "Prefix": str,
         "BucketOwner": str,
     },
-    total=False,
 )
 
 VerifiedAccessLogOptionsTypeDef = TypedDict(
     "VerifiedAccessLogOptionsTypeDef",
     {
         "S3": VerifiedAccessLogS3DestinationOptionsTypeDef,
         "CloudWatchLogs": VerifiedAccessLogCloudWatchLogsDestinationOptionsTypeDef,
@@ -24698,46 +24252,42 @@
         "Iops": int,
         "Tags": List[TagTypeDef],
         "VolumeType": VolumeTypeType,
         "FastRestored": bool,
         "MultiAttachEnabled": bool,
         "Throughput": int,
     },
-    total=False,
 )
 
 VolumeStatusInfoTypeDef = TypedDict(
     "VolumeStatusInfoTypeDef",
     {
         "Details": List[VolumeStatusDetailsTypeDef],
         "Status": VolumeStatusInfoStatusType,
     },
-    total=False,
 )
 
 VpcCidrBlockAssociationTypeDef = TypedDict(
     "VpcCidrBlockAssociationTypeDef",
     {
         "AssociationId": str,
         "CidrBlock": str,
         "CidrBlockState": VpcCidrBlockStateTypeDef,
     },
-    total=False,
 )
 
 VpcIpv6CidrBlockAssociationTypeDef = TypedDict(
     "VpcIpv6CidrBlockAssociationTypeDef",
     {
         "AssociationId": str,
         "Ipv6CidrBlock": str,
         "Ipv6CidrBlockState": VpcCidrBlockStateTypeDef,
         "NetworkBorderGroup": str,
         "Ipv6Pool": str,
     },
-    total=False,
 )
 
 VpcPeeringConnectionVpcInfoResponseMetadataTypeDef = TypedDict(
     "VpcPeeringConnectionVpcInfoResponseMetadataTypeDef",
     {
         "CidrBlock": str,
         "Ipv6CidrBlockSet": List[Ipv6CidrBlockTypeDef],
@@ -24757,15 +24307,14 @@
         "Ipv6CidrBlockSet": List[Ipv6CidrBlockTypeDef],
         "CidrBlockSet": List[CidrBlockTypeDef],
         "OwnerId": str,
         "PeeringOptions": VpcPeeringConnectionOptionsDescriptionTypeDef,
         "VpcId": str,
         "Region": str,
     },
-    total=False,
 )
 
 DescribeAccountAttributesResultTypeDef = TypedDict(
     "DescribeAccountAttributesResultTypeDef",
     {
         "AccountAttributes": List[AccountAttributeTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
@@ -24780,15 +24329,14 @@
         "VpcEndpointService": AnalysisComponentTypeDef,
         "RuleOptions": List[RuleOptionTypeDef],
         "RuleGroupTypePairs": List[RuleGroupTypePairTypeDef],
         "RuleGroupRuleOptionsPairs": List[RuleGroupRuleOptionsPairTypeDef],
         "ServiceName": str,
         "LoadBalancers": List[AnalysisComponentTypeDef],
     },
-    total=False,
 )
 
 DescribeAddressesAttributeResultTypeDef = TypedDict(
     "DescribeAddressesAttributeResultTypeDef",
     {
         "Addresses": List[AddressAttributeTypeDef],
         "NextToken": str,
@@ -24960,15 +24508,14 @@
         "TimeRanges": List[InstanceEventWindowTimeRangeTypeDef],
         "Name": str,
         "CronExpression": str,
         "AssociationTarget": InstanceEventWindowAssociationTargetTypeDef,
         "State": InstanceEventWindowStateType,
         "Tags": List[TagTypeDef],
     },
-    total=False,
 )
 
 _RequiredDisassociateInstanceEventWindowRequestRequestTypeDef = TypedDict(
     "_RequiredDisassociateInstanceEventWindowRequestRequestTypeDef",
     {
         "InstanceEventWindowId": str,
         "AssociationTarget": InstanceEventWindowDisassociationRequestTypeDef,
@@ -27630,15 +27177,14 @@
         "TransitGatewayRouteTableRoute": TransitGatewayRouteTableRouteTypeDef,
         "TransitGatewayAttachment": AnalysisComponentTypeDef,
         "ComponentAccount": str,
         "ComponentRegion": str,
         "FirewallStatelessRule": FirewallStatelessRuleTypeDef,
         "FirewallStatefulRule": FirewallStatefulRuleTypeDef,
     },
-    total=False,
 )
 
 DescribeClientVpnTargetNetworksResultTypeDef = TypedDict(
     "DescribeClientVpnTargetNetworksResultTypeDef",
     {
         "ClientVpnTargetNetworks": List[TargetNetworkTypeDef],
         "NextToken": str,
@@ -27653,15 +27199,14 @@
         "PropagatingVgws": List[PropagatingVgwTypeDef],
         "RouteTableId": str,
         "Routes": List[RouteTypeDef],
         "Tags": List[TagTypeDef],
         "VpcId": str,
         "OwnerId": str,
     },
-    total=False,
 )
 
 _RequiredGetFlowLogsIntegrationTemplateRequestRequestTypeDef = TypedDict(
     "_RequiredGetFlowLogsIntegrationTemplateRequestRequestTypeDef",
     {
         "FlowLogId": str,
         "ConfigDeliveryS3DestinationArn": str,
@@ -27725,26 +27270,24 @@
         "DeviceIndex": int,
         "NetworkCardIndex": int,
         "InstanceId": str,
         "InstanceOwnerId": str,
         "Status": AttachmentStatusType,
         "EnaSrdSpecification": AttachmentEnaSrdSpecificationTypeDef,
     },
-    total=False,
 )
 
 DhcpOptionsTypeDef = TypedDict(
     "DhcpOptionsTypeDef",
     {
         "DhcpConfigurations": List[DhcpConfigurationTypeDef],
         "DhcpOptionsId": str,
         "OwnerId": str,
         "Tags": List[TagTypeDef],
     },
-    total=False,
 )
 
 DescribeClientVpnAuthorizationRulesResultTypeDef = TypedDict(
     "DescribeClientVpnAuthorizationRulesResultTypeDef",
     {
         "AuthorizationRules": List[AuthorizationRuleTypeDef],
         "NextToken": str,
@@ -27780,15 +27323,14 @@
         "OwnerId": str,
         "AvailabilityZoneId": str,
         "MemberOfServiceLinkedResourceGroup": bool,
         "OutpostArn": str,
         "HostMaintenance": HostMaintenanceType,
         "AssetId": str,
     },
-    total=False,
 )
 
 _RequiredCreateImageRequestInstanceCreateImageTypeDef = TypedDict(
     "_RequiredCreateImageRequestInstanceCreateImageTypeDef",
     {
         "Name": str,
     },
@@ -27889,15 +27431,14 @@
         "Tags": List[TagTypeDef],
         "VirtualizationType": VirtualizationTypeType,
         "BootMode": BootModeValuesType,
         "TpmSupport": Literal["v2.0"],
         "DeprecationTime": str,
         "ImdsSupport": Literal["v2.0"],
     },
-    total=False,
 )
 
 _RequiredRegisterImageRequestRequestTypeDef = TypedDict(
     "_RequiredRegisterImageRequestRequestTypeDef",
     {
         "Name": str,
     },
@@ -28106,15 +27647,14 @@
         "SecurityGroupIds": List[str],
         "VpcId": str,
         "SelfServicePortalUrl": str,
         "ClientConnectOptions": ClientConnectResponseOptionsTypeDef,
         "SessionTimeoutHours": int,
         "ClientLoginBannerOptions": ClientLoginBannerResponseOptionsTypeDef,
     },
-    total=False,
 )
 
 DescribeClientVpnConnectionsResultTypeDef = TypedDict(
     "DescribeClientVpnConnectionsResultTypeDef",
     {
         "Connections": List[ClientVpnConnectionTypeDef],
         "NextToken": str,
@@ -28216,29 +27756,27 @@
         "Phase1DHGroupNumbers": List[Phase1DHGroupNumbersListValueTypeDef],
         "Phase2DHGroupNumbers": List[Phase2DHGroupNumbersListValueTypeDef],
         "IkeVersions": List[IKEVersionsListValueTypeDef],
         "StartupAction": str,
         "LogOptions": VpnTunnelLogOptionsTypeDef,
         "EnableTunnelLifecycleControl": bool,
     },
-    total=False,
 )
 
 NetworkAclTypeDef = TypedDict(
     "NetworkAclTypeDef",
     {
         "Associations": List[NetworkAclAssociationTypeDef],
         "Entries": List[NetworkAclEntryTypeDef],
         "IsDefault": bool,
         "NetworkAclId": str,
         "Tags": List[TagTypeDef],
         "VpcId": str,
         "OwnerId": str,
     },
-    total=False,
 )
 
 LaunchSpecificationTypeDef = TypedDict(
     "LaunchSpecificationTypeDef",
     {
         "UserData": str,
         "SecurityGroups": List[GroupIdentifierTypeDef],
@@ -28252,15 +27790,14 @@
         "KeyName": str,
         "NetworkInterfaces": List[InstanceNetworkInterfaceSpecificationTypeDef],
         "Placement": SpotPlacementTypeDef,
         "RamdiskId": str,
         "SubnetId": str,
         "Monitoring": RunInstancesMonitoringEnabledTypeDef,
     },
-    total=False,
 )
 
 RequestSpotLaunchSpecificationTypeDef = TypedDict(
     "RequestSpotLaunchSpecificationTypeDef",
     {
         "SecurityGroupIds": Sequence[str],
         "SecurityGroups": Sequence[str],
@@ -28391,26 +27928,24 @@
 
 DisableFastSnapshotRestoreErrorItemTypeDef = TypedDict(
     "DisableFastSnapshotRestoreErrorItemTypeDef",
     {
         "SnapshotId": str,
         "FastSnapshotRestoreStateErrors": List[DisableFastSnapshotRestoreStateErrorItemTypeDef],
     },
-    total=False,
 )
 
 ImportInstanceTaskDetailsTypeDef = TypedDict(
     "ImportInstanceTaskDetailsTypeDef",
     {
         "Description": str,
         "InstanceId": str,
         "Platform": Literal["Windows"],
         "Volumes": List[ImportInstanceVolumeDetailItemTypeDef],
     },
-    total=False,
 )
 
 DescribeVpcEndpointConnectionsResultTypeDef = TypedDict(
     "DescribeVpcEndpointConnectionsResultTypeDef",
     {
         "VpcEndpointConnections": List[VpcEndpointConnectionTypeDef],
         "NextToken": str,
@@ -28640,15 +28175,14 @@
 
 EnableFastSnapshotRestoreErrorItemTypeDef = TypedDict(
     "EnableFastSnapshotRestoreErrorItemTypeDef",
     {
         "SnapshotId": str,
         "FastSnapshotRestoreStateErrors": List[EnableFastSnapshotRestoreStateErrorItemTypeDef],
     },
-    total=False,
 )
 
 DescribeFleetHistoryResultTypeDef = TypedDict(
     "DescribeFleetHistoryResultTypeDef",
     {
         "HistoryRecords": List[HistoryRecordEntryTypeDef],
         "LastEvaluatedTime": datetime,
@@ -28710,15 +28244,14 @@
         "DestinationIp": str,
         "Protocol": ProtocolType,
         "DestinationPort": int,
         "Tags": List[TagTypeDef],
         "FilterAtSource": PathFilterTypeDef,
         "FilterAtDestination": PathFilterTypeDef,
     },
-    total=False,
 )
 
 SpotOptionsRequestTypeDef = TypedDict(
     "SpotOptionsRequestTypeDef",
     {
         "AllocationStrategy": SpotAllocationStrategyType,
         "MaintenanceStrategies": FleetSpotMaintenanceStrategiesRequestTypeDef,
@@ -28740,24 +28273,22 @@
         "InstanceInterruptionBehavior": SpotInstanceInterruptionBehaviorType,
         "InstancePoolsToUseCount": int,
         "SingleInstanceType": bool,
         "SingleAvailabilityZone": bool,
         "MinTargetCapacity": int,
         "MaxTotalPrice": str,
     },
-    total=False,
 )
 
 FpgaInfoTypeDef = TypedDict(
     "FpgaInfoTypeDef",
     {
         "Fpgas": List[FpgaDeviceInfoTypeDef],
         "TotalFpgaMemoryInMiB": int,
     },
-    total=False,
 )
 
 DescribeFpgaImageAttributeResultTypeDef = TypedDict(
     "DescribeFpgaImageAttributeResultTypeDef",
     {
         "FpgaImageAttribute": FpgaImageAttributeTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
@@ -28783,15 +28314,14 @@
 
 GpuInfoTypeDef = TypedDict(
     "GpuInfoTypeDef",
     {
         "Gpus": List[GpuDeviceInfoTypeDef],
         "TotalGpuMemoryInMiB": int,
     },
-    total=False,
 )
 
 AssociateIamInstanceProfileResultTypeDef = TypedDict(
     "AssociateIamInstanceProfileResultTypeDef",
     {
         "IamInstanceProfileAssociation": IamInstanceProfileAssociationTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
@@ -29175,15 +28705,14 @@
         "Status": NetworkInterfaceStatusType,
         "SubnetId": str,
         "VpcId": str,
         "InterfaceType": str,
         "Ipv4Prefixes": List[InstanceIpv4PrefixTypeDef],
         "Ipv6Prefixes": List[InstanceIpv6PrefixTypeDef],
     },
-    total=False,
 )
 
 FleetLaunchTemplateOverridesRequestTypeDef = TypedDict(
     "FleetLaunchTemplateOverridesRequestTypeDef",
     {
         "InstanceType": InstanceTypeType,
         "MaxPrice": str,
@@ -29268,29 +28797,27 @@
         "AvailabilityZone": str,
         "WeightedCapacity": float,
         "Priority": float,
         "Placement": PlacementResponseTypeDef,
         "InstanceRequirements": InstanceRequirementsTypeDef,
         "ImageId": str,
     },
-    total=False,
 )
 
 LaunchTemplateOverridesTypeDef = TypedDict(
     "LaunchTemplateOverridesTypeDef",
     {
         "InstanceType": InstanceTypeType,
         "SpotPrice": str,
         "SubnetId": str,
         "AvailabilityZone": str,
         "WeightedCapacity": float,
         "Priority": float,
         "InstanceRequirements": InstanceRequirementsTypeDef,
     },
-    total=False,
 )
 
 SpotFleetLaunchSpecificationTypeDef = TypedDict(
     "SpotFleetLaunchSpecificationTypeDef",
     {
         "SecurityGroups": List[GroupIdentifierTypeDef],
         "AddressingType": str,
@@ -29308,15 +28835,14 @@
         "SpotPrice": str,
         "SubnetId": str,
         "UserData": str,
         "WeightedCapacity": float,
         "TagSpecifications": List[SpotFleetTagSpecificationTypeDef],
         "InstanceRequirements": InstanceRequirementsTypeDef,
     },
-    total=False,
 )
 
 StartInstancesResultTypeDef = TypedDict(
     "StartInstancesResultTypeDef",
     {
         "StartingInstances": List[InstanceStateChangeTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
@@ -29346,15 +28872,14 @@
         "OutpostArn": str,
         "Events": List[InstanceStatusEventTypeDef],
         "InstanceId": str,
         "InstanceState": InstanceStateTypeDef,
         "InstanceStatus": InstanceStatusSummaryTypeDef,
         "SystemStatus": InstanceStatusSummaryTypeDef,
     },
-    total=False,
 )
 
 _RequiredAuthorizeSecurityGroupEgressRequestRequestTypeDef = TypedDict(
     "_RequiredAuthorizeSecurityGroupEgressRequestRequestTypeDef",
     {
         "GroupId": str,
     },
@@ -29541,15 +29066,14 @@
         "IpPermissions": List[IpPermissionTypeDef],
         "OwnerId": str,
         "GroupId": str,
         "IpPermissionsEgress": List[IpPermissionTypeDef],
         "Tags": List[TagTypeDef],
         "VpcId": str,
     },
-    total=False,
 )
 
 UpdateSecurityGroupRuleDescriptionsEgressRequestRequestTypeDef = TypedDict(
     "UpdateSecurityGroupRuleDescriptionsEgressRequestRequestTypeDef",
     {
         "DryRun": bool,
         "GroupId": str,
@@ -29578,15 +29102,14 @@
         "Description": str,
         "GroupId": str,
         "GroupName": str,
         "StaleIpPermissions": List[StaleIpPermissionTypeDef],
         "StaleIpPermissionsEgress": List[StaleIpPermissionTypeDef],
         "VpcId": str,
     },
-    total=False,
 )
 
 GetIpamDiscoveredAccountsResultTypeDef = TypedDict(
     "GetIpamDiscoveredAccountsResultTypeDef",
     {
         "IpamDiscoveredAccounts": List[IpamDiscoveredAccountTypeDef],
         "NextToken": str,
@@ -29830,15 +29353,14 @@
         "MetadataOptions": LaunchTemplateInstanceMetadataOptionsTypeDef,
         "EnclaveOptions": LaunchTemplateEnclaveOptionsTypeDef,
         "InstanceRequirements": InstanceRequirementsTypeDef,
         "PrivateDnsNameOptions": LaunchTemplatePrivateDnsNameOptionsTypeDef,
         "MaintenanceOptions": LaunchTemplateInstanceMaintenanceOptionsTypeDef,
         "DisableApiStop": bool,
     },
-    total=False,
 )
 
 _RequiredModifyFpgaImageAttributeRequestRequestTypeDef = TypedDict(
     "_RequiredModifyFpgaImageAttributeRequestRequestTypeDef",
     {
         "FpgaImageId": str,
     },
@@ -29876,15 +29398,14 @@
         "ModificationResults": List[ReservedInstancesModificationResultTypeDef],
         "ReservedInstancesIds": List[ReservedInstancesIdTypeDef],
         "ReservedInstancesModificationId": str,
         "Status": str,
         "StatusMessage": str,
         "UpdateDate": datetime,
     },
-    total=False,
 )
 
 CreateNatGatewayResultTypeDef = TypedDict(
     "CreateNatGatewayResultTypeDef",
     {
         "ClientToken": str,
         "NatGateway": NatGatewayTypeDef,
@@ -29995,15 +29516,14 @@
 AccessScopePathTypeDef = TypedDict(
     "AccessScopePathTypeDef",
     {
         "Source": PathStatementTypeDef,
         "Destination": PathStatementTypeDef,
         "ThroughResources": List[ThroughResourcesStatementTypeDef],
     },
-    total=False,
 )
 
 CancelReservedInstancesListingResultTypeDef = TypedDict(
     "CancelReservedInstancesListingResultTypeDef",
     {
         "ReservedInstancesListings": List[ReservedInstancesListingTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
@@ -30109,15 +29629,14 @@
         "InstanceId": str,
         "Progress": str,
         "StartTime": datetime,
         "State": BundleTaskStateType,
         "Storage": StorageTypeDef,
         "UpdateTime": datetime,
     },
-    total=False,
 )
 
 DescribeScheduledInstanceAvailabilityResultTypeDef = TypedDict(
     "DescribeScheduledInstanceAvailabilityResultTypeDef",
     {
         "NextToken": str,
         "ScheduledInstanceAvailabilitySet": List[ScheduledInstanceAvailabilityTypeDef],
@@ -30285,15 +29804,14 @@
         "Status": str,
         "StatusMessage": str,
         "Tags": List[TagTypeDef],
         "LicenseSpecifications": List[ImportImageLicenseConfigurationResponseTypeDef],
         "UsageOperation": str,
         "BootMode": BootModeValuesType,
     },
-    total=False,
 )
 
 ImportSnapshotResultTypeDef = TypedDict(
     "ImportSnapshotResultTypeDef",
     {
         "Description": str,
         "ImportTaskId": str,
@@ -30307,15 +29825,14 @@
     "ImportSnapshotTaskTypeDef",
     {
         "Description": str,
         "ImportTaskId": str,
         "SnapshotTaskDetail": SnapshotTaskDetailTypeDef,
         "Tags": List[TagTypeDef],
     },
-    total=False,
 )
 
 CreateSpotDatafeedSubscriptionResultTypeDef = TypedDict(
     "CreateSpotDatafeedSubscriptionResultTypeDef",
     {
         "SpotDatafeedSubscription": SpotDatafeedSubscriptionTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
@@ -30410,15 +29927,14 @@
         "Tags": List[TagTypeDef],
         "SubnetArn": str,
         "OutpostArn": str,
         "EnableDns64": bool,
         "Ipv6Native": bool,
         "PrivateDnsNameOptionsOnLaunch": PrivateDnsNameOptionsOnLaunchTypeDef,
     },
-    total=False,
 )
 
 GetReservedInstancesExchangeQuoteResultTypeDef = TypedDict(
     "GetReservedInstancesExchangeQuoteResultTypeDef",
     {
         "CurrencyCode": str,
         "IsValidExchange": bool,
@@ -30435,15 +29951,14 @@
 
 LoadBalancersConfigTypeDef = TypedDict(
     "LoadBalancersConfigTypeDef",
     {
         "ClassicLoadBalancersConfig": ClassicLoadBalancersConfigTypeDef,
         "TargetGroupsConfig": TargetGroupsConfigTypeDef,
     },
-    total=False,
 )
 
 CreateTrafficMirrorFilterRuleResultTypeDef = TypedDict(
     "CreateTrafficMirrorFilterRuleResultTypeDef",
     {
         "TrafficMirrorFilterRule": TrafficMirrorFilterRuleTypeDef,
         "ClientToken": str,
@@ -30465,15 +29980,14 @@
         "TrafficMirrorFilterId": str,
         "IngressFilterRules": List[TrafficMirrorFilterRuleTypeDef],
         "EgressFilterRules": List[TrafficMirrorFilterRuleTypeDef],
         "NetworkServices": List[Literal["amazon-dns"]],
         "Description": str,
         "Tags": List[TagTypeDef],
     },
-    total=False,
 )
 
 DescribeTransitGatewayAttachmentsResultTypeDef = TypedDict(
     "DescribeTransitGatewayAttachmentsResultTypeDef",
     {
         "TransitGatewayAttachments": List[TransitGatewayAttachmentTypeDef],
         "NextToken": str,
@@ -30487,15 +30001,14 @@
         "TransitGatewayAttachmentId": str,
         "TransitGatewayConnectPeerId": str,
         "State": TransitGatewayConnectPeerStateType,
         "CreationTime": datetime,
         "ConnectPeerConfiguration": TransitGatewayConnectPeerConfigurationTypeDef,
         "Tags": List[TagTypeDef],
     },
-    total=False,
 )
 
 CreateTransitGatewayConnectResultTypeDef = TypedDict(
     "CreateTransitGatewayConnectResultTypeDef",
     {
         "TransitGatewayConnect": TransitGatewayConnectTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
@@ -30621,15 +30134,14 @@
 TransitGatewayPolicyTableEntryTypeDef = TypedDict(
     "TransitGatewayPolicyTableEntryTypeDef",
     {
         "PolicyRuleNumber": str,
         "PolicyRule": TransitGatewayPolicyRuleTypeDef,
         "TargetRouteTableId": str,
     },
-    total=False,
 )
 
 CreateTransitGatewayPrefixListReferenceResultTypeDef = TypedDict(
     "CreateTransitGatewayPrefixListReferenceResultTypeDef",
     {
         "TransitGatewayPrefixListReference": TransitGatewayPrefixListReferenceTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
@@ -30930,15 +30442,14 @@
     {
         "S3": VerifiedAccessLogS3DestinationTypeDef,
         "CloudWatchLogs": VerifiedAccessLogCloudWatchLogsDestinationTypeDef,
         "KinesisDataFirehose": VerifiedAccessLogKinesisDataFirehoseDestinationTypeDef,
         "LogVersion": str,
         "IncludeTrustContext": bool,
     },
-    total=False,
 )
 
 _RequiredModifyVerifiedAccessInstanceLoggingConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredModifyVerifiedAccessInstanceLoggingConfigurationRequestRequestTypeDef",
     {
         "VerifiedAccessInstanceId": str,
         "AccessLogs": VerifiedAccessLogOptionsTypeDef,
@@ -30977,15 +30488,14 @@
         "AvailabilityZone": str,
         "OutpostArn": str,
         "Events": List[VolumeStatusEventTypeDef],
         "VolumeId": str,
         "VolumeStatus": VolumeStatusInfoTypeDef,
         "AttachmentStatuses": List[VolumeStatusAttachmentStatusTypeDef],
     },
-    total=False,
 )
 
 AssociateVpcCidrBlockResultTypeDef = TypedDict(
     "AssociateVpcCidrBlockResultTypeDef",
     {
         "Ipv6CidrBlockAssociation": VpcIpv6CidrBlockAssociationTypeDef,
         "CidrBlockAssociation": VpcCidrBlockAssociationTypeDef,
@@ -31014,28 +30524,26 @@
         "OwnerId": str,
         "InstanceTenancy": TenancyType,
         "Ipv6CidrBlockAssociationSet": List[VpcIpv6CidrBlockAssociationTypeDef],
         "CidrBlockAssociationSet": List[VpcCidrBlockAssociationTypeDef],
         "IsDefault": bool,
         "Tags": List[TagTypeDef],
     },
-    total=False,
 )
 
 VpcPeeringConnectionTypeDef = TypedDict(
     "VpcPeeringConnectionTypeDef",
     {
         "AccepterVpcInfo": VpcPeeringConnectionVpcInfoTypeDef,
         "ExpirationTime": datetime,
         "RequesterVpcInfo": VpcPeeringConnectionVpcInfoTypeDef,
         "Status": VpcPeeringConnectionStateReasonTypeDef,
         "Tags": List[TagTypeDef],
         "VpcPeeringConnectionId": str,
     },
-    total=False,
 )
 
 AssociateInstanceEventWindowResultTypeDef = TypedDict(
     "AssociateInstanceEventWindowResultTypeDef",
     {
         "InstanceEventWindow": InstanceEventWindowTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
@@ -31095,15 +30603,14 @@
         "TransitGatewayRouteTableRoute": TransitGatewayRouteTableRouteTypeDef,
         "Explanations": List[ExplanationTypeDef],
         "ElasticLoadBalancerListener": AnalysisComponentTypeDef,
         "FirewallStatelessRule": FirewallStatelessRuleTypeDef,
         "FirewallStatefulRule": FirewallStatefulRuleTypeDef,
         "ServiceName": str,
     },
-    total=False,
 )
 
 CreateRouteTableResultTypeDef = TypedDict(
     "CreateRouteTableResultTypeDef",
     {
         "RouteTable": RouteTableTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
@@ -31157,15 +30664,14 @@
         "SubnetId": str,
         "TagSet": List[TagTypeDef],
         "VpcId": str,
         "DenyAllIgwTraffic": bool,
         "Ipv6Native": bool,
         "Ipv6Address": str,
     },
-    total=False,
 )
 
 CreateDhcpOptionsResultTypeDef = TypedDict(
     "CreateDhcpOptionsResultTypeDef",
     {
         "DhcpOptions": DhcpOptionsTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
@@ -31260,15 +30766,14 @@
         "LocalIpv6NetworkCidr": str,
         "RemoteIpv6NetworkCidr": str,
         "OutsideIpAddressType": str,
         "TransportTransitGatewayAttachmentId": str,
         "TunnelInsideIpVersion": TunnelInsideIpVersionType,
         "TunnelOptions": List[TunnelOptionTypeDef],
     },
-    total=False,
 )
 
 CreateNetworkAclResultTypeDef = TypedDict(
     "CreateNetworkAclResultTypeDef",
     {
         "NetworkAcl": NetworkAclTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
@@ -31303,15 +30808,14 @@
         "Status": SpotInstanceStatusTypeDef,
         "Tags": List[TagTypeDef],
         "Type": SpotInstanceTypeType,
         "ValidFrom": datetime,
         "ValidUntil": datetime,
         "InstanceInterruptionBehavior": InstanceInterruptionBehaviorType,
     },
-    total=False,
 )
 
 RequestSpotInstancesRequestRequestTypeDef = TypedDict(
     "RequestSpotInstancesRequestRequestTypeDef",
     {
         "AvailabilityZoneGroup": str,
         "BlockDurationMinutes": int,
@@ -31346,15 +30850,14 @@
         "ExpirationTime": str,
         "ImportInstance": ImportInstanceTaskDetailsTypeDef,
         "ImportVolume": ImportVolumeTaskDetailsTypeDef,
         "State": ConversionTaskStateType,
         "StatusMessage": str,
         "Tags": List[TagTypeDef],
     },
-    total=False,
 )
 
 EnableFastSnapshotRestoresResultTypeDef = TypedDict(
     "EnableFastSnapshotRestoresResultTypeDef",
     {
         "Successful": List[EnableFastSnapshotRestoreSuccessItemTypeDef],
         "Unsuccessful": List[EnableFastSnapshotRestoreErrorItemTypeDef],
@@ -31404,15 +30907,14 @@
         "HibernationSupported": bool,
         "BurstablePerformanceSupported": bool,
         "DedicatedHostsSupported": bool,
         "AutoRecoverySupported": bool,
         "SupportedBootModes": List[BootModeTypeType],
         "NitroEnclavesSupport": NitroEnclavesSupportType,
     },
-    total=False,
 )
 
 InstanceTypeDef = TypedDict(
     "InstanceTypeDef",
     {
         "AmiLaunchIndex": int,
         "ImageId": str,
@@ -31470,15 +30972,14 @@
         "UsageOperationUpdateTime": datetime,
         "PrivateDnsNameOptions": PrivateDnsNameOptionsResponseTypeDef,
         "Ipv6Address": str,
         "TpmSupport": str,
         "MaintenanceOptions": InstanceMaintenanceOptionsTypeDef,
         "CurrentInstanceBootMode": InstanceBootModeValuesType,
     },
-    total=False,
 )
 
 FleetLaunchTemplateConfigRequestTypeDef = TypedDict(
     "FleetLaunchTemplateConfigRequestTypeDef",
     {
         "LaunchTemplateSpecification": FleetLaunchTemplateSpecificationRequestTypeDef,
         "Overrides": Sequence[FleetLaunchTemplateOverridesRequestTypeDef],
@@ -31545,33 +31046,30 @@
 
 FleetLaunchTemplateConfigTypeDef = TypedDict(
     "FleetLaunchTemplateConfigTypeDef",
     {
         "LaunchTemplateSpecification": FleetLaunchTemplateSpecificationTypeDef,
         "Overrides": List[FleetLaunchTemplateOverridesTypeDef],
     },
-    total=False,
 )
 
 LaunchTemplateAndOverridesResponseTypeDef = TypedDict(
     "LaunchTemplateAndOverridesResponseTypeDef",
     {
         "LaunchTemplateSpecification": FleetLaunchTemplateSpecificationTypeDef,
         "Overrides": FleetLaunchTemplateOverridesTypeDef,
     },
-    total=False,
 )
 
 LaunchTemplateConfigTypeDef = TypedDict(
     "LaunchTemplateConfigTypeDef",
     {
         "LaunchTemplateSpecification": FleetLaunchTemplateSpecificationTypeDef,
         "Overrides": List[LaunchTemplateOverridesTypeDef],
     },
-    total=False,
 )
 
 DescribeInstanceStatusResultTypeDef = TypedDict(
     "DescribeInstanceStatusResultTypeDef",
     {
         "InstanceStatuses": List[InstanceStatusTypeDef],
         "NextToken": str,
@@ -31667,15 +31165,14 @@
         "VersionNumber": int,
         "VersionDescription": str,
         "CreateTime": datetime,
         "CreatedBy": str,
         "DefaultVersion": bool,
         "LaunchTemplateData": ResponseLaunchTemplateDataTypeDef,
     },
-    total=False,
 )
 
 DescribeReservedInstancesModificationsResultTypeDef = TypedDict(
     "DescribeReservedInstancesModificationsResultTypeDef",
     {
         "NextToken": str,
         "ReservedInstancesModifications": List[ReservedInstancesModificationTypeDef],
@@ -31711,15 +31208,14 @@
 NetworkInsightsAccessScopeContentTypeDef = TypedDict(
     "NetworkInsightsAccessScopeContentTypeDef",
     {
         "NetworkInsightsAccessScopeId": str,
         "MatchPaths": List[AccessScopePathTypeDef],
         "ExcludePaths": List[AccessScopePathTypeDef],
     },
-    total=False,
 )
 
 BundleInstanceResultTypeDef = TypedDict(
     "BundleInstanceResultTypeDef",
     {
         "BundleTask": BundleTaskTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
@@ -31871,15 +31367,14 @@
 
 VerifiedAccessInstanceLoggingConfigurationTypeDef = TypedDict(
     "VerifiedAccessInstanceLoggingConfigurationTypeDef",
     {
         "VerifiedAccessInstanceId": str,
         "AccessLogs": VerifiedAccessLogsTypeDef,
     },
-    total=False,
 )
 
 DescribeVolumeStatusResultTypeDef = TypedDict(
     "DescribeVolumeStatusResultTypeDef",
     {
         "NextToken": str,
         "VolumeStatuses": List[VolumeStatusItemTypeDef],
@@ -31941,15 +31436,14 @@
     "AccessScopeAnalysisFindingTypeDef",
     {
         "NetworkInsightsAccessScopeAnalysisId": str,
         "NetworkInsightsAccessScopeId": str,
         "FindingId": str,
         "FindingComponents": List[PathComponentTypeDef],
     },
-    total=False,
 )
 
 NetworkInsightsAnalysisTypeDef = TypedDict(
     "NetworkInsightsAnalysisTypeDef",
     {
         "NetworkInsightsAnalysisId": str,
         "NetworkInsightsAnalysisArn": str,
@@ -31964,15 +31458,14 @@
         "ForwardPathComponents": List[PathComponentTypeDef],
         "ReturnPathComponents": List[PathComponentTypeDef],
         "Explanations": List[ExplanationTypeDef],
         "AlternatePathHints": List[AlternatePathHintTypeDef],
         "SuggestedAccounts": List[str],
         "Tags": List[TagTypeDef],
     },
-    total=False,
 )
 
 CreateNetworkInterfaceResultTypeDef = TypedDict(
     "CreateNetworkInterfaceResultTypeDef",
     {
         "NetworkInterface": NetworkInterfaceTypeDef,
         "ClientToken": str,
@@ -32031,15 +31524,14 @@
         "CoreNetworkAttachmentArn": str,
         "GatewayAssociationState": GatewayAssociationStateType,
         "Options": VpnConnectionOptionsTypeDef,
         "Routes": List[VpnStaticRouteTypeDef],
         "Tags": List[TagTypeDef],
         "VgwTelemetry": List[VgwTelemetryTypeDef],
     },
-    total=False,
 )
 
 DescribeSpotInstanceRequestsResultTypeDef = TypedDict(
     "DescribeSpotInstanceRequestsResultTypeDef",
     {
         "SpotInstanceRequests": List[SpotInstanceRequestTypeDef],
         "NextToken": str,
@@ -32105,15 +31597,14 @@
     {
         "Groups": List[GroupIdentifierTypeDef],
         "Instances": List[InstanceTypeDef],
         "OwnerId": str,
         "RequesterId": str,
         "ReservationId": str,
     },
-    total=False,
 )
 
 _RequiredCreateFleetRequestRequestTypeDef = TypedDict(
     "_RequiredCreateFleetRequestRequestTypeDef",
     {
         "LaunchTemplateConfigs": Sequence[FleetLaunchTemplateConfigRequestTypeDef],
         "TargetCapacitySpecification": TargetCapacitySpecificationRequestTypeDef,
@@ -32174,50 +31665,46 @@
     "CreateFleetErrorTypeDef",
     {
         "LaunchTemplateAndOverrides": LaunchTemplateAndOverridesResponseTypeDef,
         "Lifecycle": InstanceLifecycleType,
         "ErrorCode": str,
         "ErrorMessage": str,
     },
-    total=False,
 )
 
 CreateFleetInstanceTypeDef = TypedDict(
     "CreateFleetInstanceTypeDef",
     {
         "LaunchTemplateAndOverrides": LaunchTemplateAndOverridesResponseTypeDef,
         "Lifecycle": InstanceLifecycleType,
         "InstanceIds": List[str],
         "InstanceType": InstanceTypeType,
         "Platform": Literal["Windows"],
     },
-    total=False,
 )
 
 DescribeFleetErrorTypeDef = TypedDict(
     "DescribeFleetErrorTypeDef",
     {
         "LaunchTemplateAndOverrides": LaunchTemplateAndOverridesResponseTypeDef,
         "Lifecycle": InstanceLifecycleType,
         "ErrorCode": str,
         "ErrorMessage": str,
     },
-    total=False,
 )
 
 DescribeFleetsInstancesTypeDef = TypedDict(
     "DescribeFleetsInstancesTypeDef",
     {
         "LaunchTemplateAndOverrides": LaunchTemplateAndOverridesResponseTypeDef,
         "Lifecycle": InstanceLifecycleType,
         "InstanceIds": List[str],
         "InstanceType": InstanceTypeType,
         "Platform": Literal["Windows"],
     },
-    total=False,
 )
 
 _RequiredModifySpotFleetRequestRequestRequestTypeDef = TypedDict(
     "_RequiredModifySpotFleetRequestRequestRequestTypeDef",
     {
         "SpotFleetRequestId": str,
     },
@@ -32238,34 +31725,29 @@
 class ModifySpotFleetRequestRequestRequestTypeDef(
     _RequiredModifySpotFleetRequestRequestRequestTypeDef,
     _OptionalModifySpotFleetRequestRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredSpotFleetRequestConfigDataTypeDef = TypedDict(
-    "_RequiredSpotFleetRequestConfigDataTypeDef",
-    {
-        "IamFleetRole": str,
-        "TargetCapacity": int,
-    },
-)
-_OptionalSpotFleetRequestConfigDataTypeDef = TypedDict(
-    "_OptionalSpotFleetRequestConfigDataTypeDef",
+SpotFleetRequestConfigDataTypeDef = TypedDict(
+    "SpotFleetRequestConfigDataTypeDef",
     {
         "AllocationStrategy": AllocationStrategyType,
         "OnDemandAllocationStrategy": OnDemandAllocationStrategyType,
         "SpotMaintenanceStrategies": SpotMaintenanceStrategiesTypeDef,
         "ClientToken": str,
         "ExcessCapacityTerminationPolicy": ExcessCapacityTerminationPolicyType,
         "FulfilledCapacity": float,
         "OnDemandFulfilledCapacity": float,
+        "IamFleetRole": str,
         "LaunchSpecifications": List[SpotFleetLaunchSpecificationTypeDef],
         "LaunchTemplateConfigs": List[LaunchTemplateConfigTypeDef],
         "SpotPrice": str,
+        "TargetCapacity": int,
         "OnDemandTargetCapacity": int,
         "OnDemandMaxTotalPrice": str,
         "SpotMaxTotalPrice": str,
         "TerminateInstancesWithExpiration": bool,
         "Type": FleetTypeType,
         "ValidFrom": datetime,
         "ValidUntil": datetime,
@@ -32273,24 +31755,16 @@
         "InstanceInterruptionBehavior": InstanceInterruptionBehaviorType,
         "LoadBalancersConfig": LoadBalancersConfigTypeDef,
         "InstancePoolsToUseCount": int,
         "Context": str,
         "TargetCapacityUnitType": TargetCapacityUnitTypeType,
         "TagSpecifications": List[TagSpecificationTypeDef],
     },
-    total=False,
 )
 
-
-class SpotFleetRequestConfigDataTypeDef(
-    _RequiredSpotFleetRequestConfigDataTypeDef, _OptionalSpotFleetRequestConfigDataTypeDef
-):
-    pass
-
-
 CreateLaunchTemplateVersionResultTypeDef = TypedDict(
     "CreateLaunchTemplateVersionResultTypeDef",
     {
         "LaunchTemplateVersion": LaunchTemplateVersionTypeDef,
         "Warning": ValidationWarningTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -32455,15 +31929,14 @@
         "SpotOptions": SpotOptionsTypeDef,
         "OnDemandOptions": OnDemandOptionsTypeDef,
         "Tags": List[TagTypeDef],
         "Errors": List[DescribeFleetErrorTypeDef],
         "Instances": List[DescribeFleetsInstancesTypeDef],
         "Context": str,
     },
-    total=False,
 )
 
 _RequiredRequestSpotFleetRequestRequestTypeDef = TypedDict(
     "_RequiredRequestSpotFleetRequestRequestTypeDef",
     {
         "SpotFleetRequestConfig": SpotFleetRequestConfigDataTypeDef,
     },
@@ -32489,15 +31962,14 @@
         "ActivityStatus": ActivityStatusType,
         "CreateTime": datetime,
         "SpotFleetRequestConfig": SpotFleetRequestConfigDataTypeDef,
         "SpotFleetRequestId": str,
         "SpotFleetRequestState": BatchStateType,
         "Tags": List[TagTypeDef],
     },
-    total=False,
 )
 
 DescribeFleetsResultTypeDef = TypedDict(
     "DescribeFleetsResultTypeDef",
     {
         "NextToken": str,
         "Fleets": List[FleetDataTypeDef],
```

### Comparing `mypy-boto3-ec2-1.28.0/mypy_boto3_ec2/type_defs.pyi` & `mypy-boto3-ec2-1.28.3/mypy_boto3_ec2/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -2467,15 +2467,14 @@
 
 AcceleratorCountTypeDef = TypedDict(
     "AcceleratorCountTypeDef",
     {
         "Min": int,
         "Max": int,
     },
-    total=False,
 )
 
 AcceleratorTotalMemoryMiBRequestTypeDef = TypedDict(
     "AcceleratorTotalMemoryMiBRequestTypeDef",
     {
         "Min": int,
         "Max": int,
@@ -2485,28 +2484,26 @@
 
 AcceleratorTotalMemoryMiBTypeDef = TypedDict(
     "AcceleratorTotalMemoryMiBTypeDef",
     {
         "Min": int,
         "Max": int,
     },
-    total=False,
 )
 
 AddressTransferTypeDef = TypedDict(
     "AddressTransferTypeDef",
     {
         "PublicIp": str,
         "AllocationId": str,
         "TransferAccountId": str,
         "TransferOfferExpirationTimestamp": datetime,
         "TransferOfferAcceptedTimestamp": datetime,
         "AddressTransferStatus": AddressTransferStatusType,
     },
-    total=False,
 )
 
 _RequiredTargetConfigurationRequestTypeDef = TypedDict(
     "_RequiredTargetConfigurationRequestTypeDef",
     {
         "OfferingId": str,
     },
@@ -2633,26 +2630,24 @@
 )
 
 AccountAttributeValueTypeDef = TypedDict(
     "AccountAttributeValueTypeDef",
     {
         "AttributeValue": str,
     },
-    total=False,
 )
 
 ActiveInstanceTypeDef = TypedDict(
     "ActiveInstanceTypeDef",
     {
         "InstanceId": str,
         "InstanceType": str,
         "SpotInstanceRequestId": str,
         "InstanceHealth": InstanceHealthStatusType,
     },
-    total=False,
 )
 
 AddIpamOperatingRegionTypeDef = TypedDict(
     "AddIpamOperatingRegionTypeDef",
     {
         "RegionName": str,
     },
@@ -2682,53 +2677,48 @@
     "AddedPrincipalTypeDef",
     {
         "PrincipalType": PrincipalTypeType,
         "Principal": str,
         "ServicePermissionId": str,
         "ServiceId": str,
     },
-    total=False,
 )
 
 AnalysisComponentTypeDef = TypedDict(
     "AnalysisComponentTypeDef",
     {
         "Id": str,
         "Arn": str,
         "Name": str,
     },
-    total=False,
 )
 
 RuleGroupTypePairTypeDef = TypedDict(
     "RuleGroupTypePairTypeDef",
     {
         "RuleGroupArn": str,
         "RuleGroupType": str,
     },
-    total=False,
 )
 
 RuleOptionTypeDef = TypedDict(
     "RuleOptionTypeDef",
     {
         "Keyword": str,
         "Settings": List[str],
     },
-    total=False,
 )
 
 PtrUpdateStatusTypeDef = TypedDict(
     "PtrUpdateStatusTypeDef",
     {
         "Value": str,
         "Status": str,
         "Reason": str,
     },
-    total=False,
 )
 
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
@@ -2760,15 +2750,14 @@
     "ByoipCidrTypeDef",
     {
         "Cidr": str,
         "Description": str,
         "StatusMessage": str,
         "State": ByoipCidrStateType,
     },
-    total=False,
 )
 
 AllocateAddressResultTypeDef = TypedDict(
     "AllocateAddressResultTypeDef",
     {
         "PublicIp": str,
         "AllocationId": str,
@@ -2823,42 +2812,38 @@
         "IpamPoolAllocationId": str,
         "Description": str,
         "ResourceId": str,
         "ResourceType": IpamPoolAllocationResourceTypeType,
         "ResourceRegion": str,
         "ResourceOwner": str,
     },
-    total=False,
 )
 
 AlternatePathHintTypeDef = TypedDict(
     "AlternatePathHintTypeDef",
     {
         "ComponentId": str,
         "ComponentArn": str,
     },
-    total=False,
 )
 
 PortRangeTypeDef = TypedDict(
     "PortRangeTypeDef",
     {
         "From": int,
         "To": int,
     },
-    total=False,
 )
 
 AnalysisLoadBalancerListenerTypeDef = TypedDict(
     "AnalysisLoadBalancerListenerTypeDef",
     {
         "LoadBalancerPort": int,
         "InstancePort": int,
     },
-    total=False,
 )
 
 AnalysisRouteTableRouteTypeDef = TypedDict(
     "AnalysisRouteTableRouteTypeDef",
     {
         "DestinationCidr": str,
         "DestinationPrefixListId": str,
@@ -2871,15 +2856,14 @@
         "TransitGatewayId": str,
         "VpcPeeringConnectionId": str,
         "State": str,
         "CarrierGatewayId": str,
         "CoreNetworkArn": str,
         "LocalGatewayId": str,
     },
-    total=False,
 )
 
 _RequiredApplySecurityGroupsToClientVpnTargetNetworkRequestRequestTypeDef = TypedDict(
     "_RequiredApplySecurityGroupsToClientVpnTargetNetworkRequestRequestTypeDef",
     {
         "ClientVpnEndpointId": str,
         "VpcId": str,
@@ -2978,23 +2962,21 @@
     pass
 
 AssignedPrivateIpAddressTypeDef = TypedDict(
     "AssignedPrivateIpAddressTypeDef",
     {
         "PrivateIpAddress": str,
     },
-    total=False,
 )
 
 Ipv4PrefixSpecificationTypeDef = TypedDict(
     "Ipv4PrefixSpecificationTypeDef",
     {
         "Ipv4Prefix": str,
     },
-    total=False,
 )
 
 _RequiredAssignPrivateNatGatewayAddressRequestRequestTypeDef = TypedDict(
     "_RequiredAssignPrivateNatGatewayAddressRequestRequestTypeDef",
     {
         "NatGatewayId": str,
     },
@@ -3023,15 +3005,14 @@
         "PrivateIp": str,
         "PublicIp": str,
         "AssociationId": str,
         "IsPrimary": bool,
         "FailureMessage": str,
         "Status": NatGatewayAddressStatusType,
     },
-    total=False,
 )
 
 AssociateAddressRequestClassicAddressAssociateTypeDef = TypedDict(
     "AssociateAddressRequestClassicAddressAssociateTypeDef",
     {
         "AllocationId": str,
         "InstanceId": str,
@@ -3102,15 +3083,14 @@
 
 AssociationStatusTypeDef = TypedDict(
     "AssociationStatusTypeDef",
     {
         "Code": AssociationStatusCodeType,
         "Message": str,
     },
-    total=False,
 )
 
 _RequiredAssociateDhcpOptionsRequestDhcpOptionsAssociateWithVpcTypeDef = TypedDict(
     "_RequiredAssociateDhcpOptionsRequestDhcpOptionsAssociateWithVpcTypeDef",
     {
         "VpcId": str,
     },
@@ -3266,15 +3246,14 @@
 
 RouteTableAssociationStateTypeDef = TypedDict(
     "RouteTableAssociationStateTypeDef",
     {
         "State": RouteTableAssociationStateCodeType,
         "StatusMessage": str,
     },
-    total=False,
 )
 
 AssociateSubnetCidrBlockRequestRequestTypeDef = TypedDict(
     "AssociateSubnetCidrBlockRequestRequestTypeDef",
     {
         "Ipv6CidrBlock": str,
         "SubnetId": str,
@@ -3329,15 +3308,14 @@
     {
         "TransitGatewayPolicyTableId": str,
         "TransitGatewayAttachmentId": str,
         "ResourceId": str,
         "ResourceType": TransitGatewayAttachmentResourceTypeType,
         "State": TransitGatewayAssociationStateType,
     },
-    total=False,
 )
 
 _RequiredAssociateTransitGatewayRouteTableRequestRequestTypeDef = TypedDict(
     "_RequiredAssociateTransitGatewayRouteTableRequestRequestTypeDef",
     {
         "TransitGatewayRouteTableId": str,
         "TransitGatewayAttachmentId": str,
@@ -3362,15 +3340,14 @@
     {
         "TransitGatewayRouteTableId": str,
         "TransitGatewayAttachmentId": str,
         "ResourceId": str,
         "ResourceType": TransitGatewayAttachmentResourceTypeType,
         "State": TransitGatewayAssociationStateType,
     },
-    total=False,
 )
 
 _RequiredAssociateTrunkInterfaceRequestRequestTypeDef = TypedDict(
     "_RequiredAssociateTrunkInterfaceRequestRequestTypeDef",
     {
         "BranchInterfaceId": str,
         "TrunkInterfaceId": str,
@@ -3425,24 +3402,22 @@
     "AssociatedRoleTypeDef",
     {
         "AssociatedRoleArn": str,
         "CertificateS3BucketName": str,
         "CertificateS3ObjectKey": str,
         "EncryptionKmsKeyId": str,
     },
-    total=False,
 )
 
 AssociatedTargetNetworkTypeDef = TypedDict(
     "AssociatedTargetNetworkTypeDef",
     {
         "NetworkId": str,
         "NetworkType": Literal["vpc"],
     },
-    total=False,
 )
 
 _RequiredAthenaIntegrationTypeDef = TypedDict(
     "_RequiredAthenaIntegrationTypeDef",
     {
         "IntegrationResultS3DestinationArn": str,
         "PartitionLoadFrequency": PartitionLoadFrequencyType,
@@ -3711,48 +3686,43 @@
 
 VpcAttachmentTypeDef = TypedDict(
     "VpcAttachmentTypeDef",
     {
         "State": AttachmentStatusType,
         "VpcId": str,
     },
-    total=False,
 )
 
 AttachmentEnaSrdUdpSpecificationTypeDef = TypedDict(
     "AttachmentEnaSrdUdpSpecificationTypeDef",
     {
         "EnaSrdUdpEnabled": bool,
     },
-    total=False,
 )
 
 AttributeBooleanValueTypeDef = TypedDict(
     "AttributeBooleanValueTypeDef",
     {
         "Value": bool,
     },
-    total=False,
 )
 
 AttributeValueTypeDef = TypedDict(
     "AttributeValueTypeDef",
     {
         "Value": str,
     },
-    total=False,
 )
 
 ClientVpnAuthorizationRuleStatusTypeDef = TypedDict(
     "ClientVpnAuthorizationRuleStatusTypeDef",
     {
         "Code": ClientVpnAuthorizationRuleStatusCodeType,
         "Message": str,
     },
-    total=False,
 )
 
 _RequiredAuthorizeClientVpnIngressRequestRequestTypeDef = TypedDict(
     "_RequiredAuthorizeClientVpnIngressRequestRequestTypeDef",
     {
         "ClientVpnEndpointId": str,
         "TargetNetworkCidr": str,
@@ -3777,25 +3747,23 @@
     pass
 
 AvailabilityZoneMessageTypeDef = TypedDict(
     "AvailabilityZoneMessageTypeDef",
     {
         "Message": str,
     },
-    total=False,
 )
 
 InstanceCapacityTypeDef = TypedDict(
     "InstanceCapacityTypeDef",
     {
         "AvailableCapacity": int,
         "InstanceType": str,
         "TotalCapacity": int,
     },
-    total=False,
 )
 
 BaselineEbsBandwidthMbpsRequestTypeDef = TypedDict(
     "BaselineEbsBandwidthMbpsRequestTypeDef",
     {
         "Min": int,
         "Max": int,
@@ -3805,15 +3773,14 @@
 
 BaselineEbsBandwidthMbpsTypeDef = TypedDict(
     "BaselineEbsBandwidthMbpsTypeDef",
     {
         "Min": int,
         "Max": int,
     },
-    total=False,
 )
 
 BlobAttributeValueTypeDef = TypedDict(
     "BlobAttributeValueTypeDef",
     {
         "Value": Union[str, bytes, IO[Any], StreamingBody],
     },
@@ -3838,15 +3805,14 @@
 
 BundleTaskErrorTypeDef = TypedDict(
     "BundleTaskErrorTypeDef",
     {
         "Code": str,
         "Message": str,
     },
-    total=False,
 )
 
 _RequiredCancelBundleTaskRequestRequestTypeDef = TypedDict(
     "_RequiredCancelBundleTaskRequestRequestTypeDef",
     {
         "BundleId": str,
     },
@@ -3866,15 +3832,14 @@
 
 CancelCapacityReservationFleetErrorTypeDef = TypedDict(
     "CancelCapacityReservationFleetErrorTypeDef",
     {
         "Code": str,
         "Message": str,
     },
-    total=False,
 )
 
 _RequiredCancelCapacityReservationFleetsRequestRequestTypeDef = TypedDict(
     "_RequiredCancelCapacityReservationFleetsRequestRequestTypeDef",
     {
         "CapacityReservationFleetIds": Sequence[str],
     },
@@ -3896,15 +3861,14 @@
 CapacityReservationFleetCancellationStateTypeDef = TypedDict(
     "CapacityReservationFleetCancellationStateTypeDef",
     {
         "CurrentFleetState": CapacityReservationFleetStateType,
         "PreviousFleetState": CapacityReservationFleetStateType,
         "CapacityReservationFleetId": str,
     },
-    total=False,
 )
 
 _RequiredCancelCapacityReservationRequestRequestTypeDef = TypedDict(
     "_RequiredCancelCapacityReservationRequestRequestTypeDef",
     {
         "CapacityReservationId": str,
     },
@@ -4015,15 +3979,14 @@
 
 CancelSpotFleetRequestsErrorTypeDef = TypedDict(
     "CancelSpotFleetRequestsErrorTypeDef",
     {
         "Code": CancelBatchErrorCodeType,
         "Message": str,
     },
-    total=False,
 )
 
 _RequiredCancelSpotFleetRequestsRequestRequestTypeDef = TypedDict(
     "_RequiredCancelSpotFleetRequestsRequestRequestTypeDef",
     {
         "SpotFleetRequestIds": Sequence[str],
         "TerminateInstances": bool,
@@ -4046,15 +4009,14 @@
 CancelSpotFleetRequestsSuccessItemTypeDef = TypedDict(
     "CancelSpotFleetRequestsSuccessItemTypeDef",
     {
         "CurrentSpotFleetRequestState": BatchStateType,
         "PreviousSpotFleetRequestState": BatchStateType,
         "SpotFleetRequestId": str,
     },
-    total=False,
 )
 
 _RequiredCancelSpotInstanceRequestsRequestRequestTypeDef = TypedDict(
     "_RequiredCancelSpotInstanceRequestsRequestRequestTypeDef",
     {
         "SpotInstanceRequestIds": Sequence[str],
     },
@@ -4075,24 +4037,22 @@
 
 CancelledSpotInstanceRequestTypeDef = TypedDict(
     "CancelledSpotInstanceRequestTypeDef",
     {
         "SpotInstanceRequestId": str,
         "State": CancelSpotInstanceRequestStateType,
     },
-    total=False,
 )
 
 CapacityAllocationTypeDef = TypedDict(
     "CapacityAllocationTypeDef",
     {
         "AllocationType": Literal["used"],
         "Count": int,
     },
-    total=False,
 )
 
 FleetCapacityReservationTypeDef = TypedDict(
     "FleetCapacityReservationTypeDef",
     {
         "CapacityReservationId": str,
         "AvailabilityZoneId": str,
@@ -4102,24 +4062,22 @@
         "TotalInstanceCount": int,
         "FulfilledCapacity": float,
         "EbsOptimized": bool,
         "CreateDate": datetime,
         "Weight": float,
         "Priority": int,
     },
-    total=False,
 )
 
 CapacityReservationGroupTypeDef = TypedDict(
     "CapacityReservationGroupTypeDef",
     {
         "GroupArn": str,
         "OwnerId": str,
     },
-    total=False,
 )
 
 CapacityReservationOptionsRequestTypeDef = TypedDict(
     "CapacityReservationOptionsRequestTypeDef",
     {
         "UsageStrategy": Literal["use-capacity-reservations-first"],
     },
@@ -4127,24 +4085,22 @@
 )
 
 CapacityReservationOptionsTypeDef = TypedDict(
     "CapacityReservationOptionsTypeDef",
     {
         "UsageStrategy": Literal["use-capacity-reservations-first"],
     },
-    total=False,
 )
 
 CapacityReservationTargetResponseTypeDef = TypedDict(
     "CapacityReservationTargetResponseTypeDef",
     {
         "CapacityReservationId": str,
         "CapacityReservationResourceGroupArn": str,
     },
-    total=False,
 )
 
 CapacityReservationTargetTypeDef = TypedDict(
     "CapacityReservationTargetTypeDef",
     {
         "CapacityReservationId": str,
         "CapacityReservationResourceGroupArn": str,
@@ -4161,15 +4117,14 @@
 )
 
 CertificateAuthenticationTypeDef = TypedDict(
     "CertificateAuthenticationTypeDef",
     {
         "ClientRootCertificateChain": str,
     },
-    total=False,
 )
 
 CidrAuthorizationContextTypeDef = TypedDict(
     "CidrAuthorizationContextTypeDef",
     {
         "Message": str,
         "Signature": str,
@@ -4177,50 +4132,45 @@
 )
 
 CidrBlockTypeDef = TypedDict(
     "CidrBlockTypeDef",
     {
         "CidrBlock": str,
     },
-    total=False,
 )
 
 ClassicLinkDnsSupportTypeDef = TypedDict(
     "ClassicLinkDnsSupportTypeDef",
     {
         "ClassicLinkDnsSupported": bool,
         "VpcId": str,
     },
-    total=False,
 )
 
 GroupIdentifierTypeDef = TypedDict(
     "GroupIdentifierTypeDef",
     {
         "GroupName": str,
         "GroupId": str,
     },
-    total=False,
 )
 
 ClassicLoadBalancerTypeDef = TypedDict(
     "ClassicLoadBalancerTypeDef",
     {
         "Name": str,
     },
-    total=False,
 )
 
 ClientCertificateRevocationListStatusTypeDef = TypedDict(
     "ClientCertificateRevocationListStatusTypeDef",
     {
         "Code": ClientCertificateRevocationListStatusCodeType,
         "Message": str,
     },
-    total=False,
 )
 
 ClientConnectOptionsTypeDef = TypedDict(
     "ClientConnectOptionsTypeDef",
     {
         "Enabled": bool,
         "LambdaFunctionArn": str,
@@ -4230,15 +4180,14 @@
 
 ClientVpnEndpointAttributeStatusTypeDef = TypedDict(
     "ClientVpnEndpointAttributeStatusTypeDef",
     {
         "Code": ClientVpnEndpointAttributeStatusCodeType,
         "Message": str,
     },
-    total=False,
 )
 
 ClientDataTypeDef = TypedDict(
     "ClientDataTypeDef",
     {
         "Comment": str,
         "UploadEnd": Union[datetime, str],
@@ -4259,15 +4208,14 @@
 
 ClientLoginBannerResponseOptionsTypeDef = TypedDict(
     "ClientLoginBannerResponseOptionsTypeDef",
     {
         "Enabled": bool,
         "BannerText": str,
     },
-    total=False,
 )
 
 DirectoryServiceAuthenticationRequestTypeDef = TypedDict(
     "DirectoryServiceAuthenticationRequestTypeDef",
     {
         "DirectoryId": str,
     },
@@ -4284,61 +4232,55 @@
 )
 
 DirectoryServiceAuthenticationTypeDef = TypedDict(
     "DirectoryServiceAuthenticationTypeDef",
     {
         "DirectoryId": str,
     },
-    total=False,
 )
 
 FederatedAuthenticationTypeDef = TypedDict(
     "FederatedAuthenticationTypeDef",
     {
         "SamlProviderArn": str,
         "SelfServiceSamlProviderArn": str,
     },
-    total=False,
 )
 
 ClientVpnConnectionStatusTypeDef = TypedDict(
     "ClientVpnConnectionStatusTypeDef",
     {
         "Code": ClientVpnConnectionStatusCodeType,
         "Message": str,
     },
-    total=False,
 )
 
 ClientVpnEndpointStatusTypeDef = TypedDict(
     "ClientVpnEndpointStatusTypeDef",
     {
         "Code": ClientVpnEndpointStatusCodeType,
         "Message": str,
     },
-    total=False,
 )
 
 ConnectionLogResponseOptionsTypeDef = TypedDict(
     "ConnectionLogResponseOptionsTypeDef",
     {
         "Enabled": bool,
         "CloudwatchLogGroup": str,
         "CloudwatchLogStream": str,
     },
-    total=False,
 )
 
 ClientVpnRouteStatusTypeDef = TypedDict(
     "ClientVpnRouteStatusTypeDef",
     {
         "Code": ClientVpnRouteStatusCodeType,
         "Message": str,
     },
-    total=False,
 )
 
 CloudWatchLogOptionsSpecificationTypeDef = TypedDict(
     "CloudWatchLogOptionsSpecificationTypeDef",
     {
         "LogEnabled": bool,
         "LogGroupArn": str,
@@ -4350,36 +4292,33 @@
 CloudWatchLogOptionsTypeDef = TypedDict(
     "CloudWatchLogOptionsTypeDef",
     {
         "LogEnabled": bool,
         "LogGroupArn": str,
         "LogOutputFormat": str,
     },
-    total=False,
 )
 
 CoipAddressUsageTypeDef = TypedDict(
     "CoipAddressUsageTypeDef",
     {
         "AllocationId": str,
         "AwsAccountId": str,
         "AwsService": str,
         "CoIp": str,
     },
-    total=False,
 )
 
 CoipCidrTypeDef = TypedDict(
     "CoipCidrTypeDef",
     {
         "Cidr": str,
         "CoipPoolId": str,
         "LocalGatewayRouteTableId": str,
     },
-    total=False,
 )
 
 _RequiredConfirmProductInstanceRequestRequestTypeDef = TypedDict(
     "_RequiredConfirmProductInstanceRequestRequestTypeDef",
     {
         "InstanceId": str,
         "ProductCode": str,
@@ -4425,15 +4364,14 @@
         "ServiceId": str,
         "VpcEndpointId": str,
         "ConnectionNotificationType": Literal["Topic"],
         "ConnectionNotificationArn": str,
         "ConnectionEvents": List[str],
         "ConnectionNotificationState": ConnectionNotificationStateType,
     },
-    total=False,
 )
 
 _RequiredCopyFpgaImageRequestRequestTypeDef = TypedDict(
     "_RequiredCopyFpgaImageRequestRequestTypeDef",
     {
         "SourceFpgaImageId": str,
         "SourceRegion": str,
@@ -4521,15 +4459,14 @@
 CpuOptionsTypeDef = TypedDict(
     "CpuOptionsTypeDef",
     {
         "CoreCount": int,
         "ThreadsPerCore": int,
         "AmdSevSnp": AmdSevSnpSpecificationType,
     },
-    total=False,
 )
 
 ReservationFleetInstanceSpecificationTypeDef = TypedDict(
     "ReservationFleetInstanceSpecificationTypeDef",
     {
         "InstanceType": InstanceTypeType,
         "InstancePlatform": CapacityReservationInstancePlatformType,
@@ -4749,24 +4686,22 @@
         "LocalGatewayRouteTableArn": str,
         "OwnerId": str,
         "SubnetId": str,
         "CoipPoolId": str,
         "NetworkInterfaceId": str,
         "DestinationPrefixListId": str,
     },
-    total=False,
 )
 
 IcmpTypeCodeTypeDef = TypedDict(
     "IcmpTypeCodeTypeDef",
     {
         "Code": int,
         "Type": int,
     },
-    total=False,
 )
 
 _RequiredCreateNetworkInterfacePermissionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateNetworkInterfacePermissionRequestRequestTypeDef",
     {
         "NetworkInterfaceId": str,
         "Permission": InterfacePermissionTypeType,
@@ -4789,15 +4724,14 @@
     pass
 
 InstanceIpv6AddressTypeDef = TypedDict(
     "InstanceIpv6AddressTypeDef",
     {
         "Ipv6Address": str,
     },
-    total=False,
 )
 
 Ipv4PrefixSpecificationRequestTypeDef = TypedDict(
     "Ipv4PrefixSpecificationRequestTypeDef",
     {
         "Ipv4Prefix": str,
     },
@@ -5126,15 +5060,14 @@
 
 CreateVolumePermissionTypeDef = TypedDict(
     "CreateVolumePermissionTypeDef",
     {
         "Group": Literal["all"],
         "UserId": str,
     },
-    total=False,
 )
 
 _RequiredCreateVpcEndpointConnectionNotificationRequestRequestTypeDef = TypedDict(
     "_RequiredCreateVpcEndpointConnectionNotificationRequestRequestTypeDef",
     {
         "ConnectionNotificationArn": str,
         "ConnectionEvents": Sequence[str],
@@ -5182,15 +5115,14 @@
 )
 
 CreditSpecificationTypeDef = TypedDict(
     "CreditSpecificationTypeDef",
     {
         "CpuCredits": str,
     },
-    total=False,
 )
 
 DataQueryTypeDef = TypedDict(
     "DataQueryTypeDef",
     {
         "Id": str,
         "Source": str,
@@ -5206,15 +5138,14 @@
     "MetricPointTypeDef",
     {
         "StartDate": datetime,
         "EndDate": datetime,
         "Value": float,
         "Status": str,
     },
-    total=False,
 )
 
 _RequiredDeleteCarrierGatewayRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteCarrierGatewayRequestRequestTypeDef",
     {
         "CarrierGatewayId": str,
     },
@@ -5391,25 +5322,23 @@
 
 DeleteFleetErrorTypeDef = TypedDict(
     "DeleteFleetErrorTypeDef",
     {
         "Code": DeleteFleetErrorCodeType,
         "Message": str,
     },
-    total=False,
 )
 
 DeleteFleetSuccessItemTypeDef = TypedDict(
     "DeleteFleetSuccessItemTypeDef",
     {
         "CurrentFleetState": FleetStateCodeType,
         "PreviousFleetState": FleetStateCodeType,
         "FleetId": str,
     },
-    total=False,
 )
 
 _RequiredDeleteFleetsRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteFleetsRequestRequestTypeDef",
     {
         "FleetIds": Sequence[str],
         "TerminateInstances": bool,
@@ -5517,15 +5446,14 @@
 
 InstanceEventWindowStateChangeTypeDef = TypedDict(
     "InstanceEventWindowStateChangeTypeDef",
     {
         "InstanceEventWindowId": str,
         "State": InstanceEventWindowStateType,
     },
-    total=False,
 )
 
 DeleteInternetGatewayRequestInternetGatewayDeleteTypeDef = TypedDict(
     "DeleteInternetGatewayRequestInternetGatewayDeleteTypeDef",
     {
         "DryRun": bool,
     },
@@ -5692,25 +5620,23 @@
 
 ResponseErrorTypeDef = TypedDict(
     "ResponseErrorTypeDef",
     {
         "Code": LaunchTemplateErrorCodeType,
         "Message": str,
     },
-    total=False,
 )
 
 DeleteLaunchTemplateVersionsResponseSuccessItemTypeDef = TypedDict(
     "DeleteLaunchTemplateVersionsResponseSuccessItemTypeDef",
     {
         "LaunchTemplateId": str,
         "LaunchTemplateName": str,
         "VersionNumber": int,
     },
-    total=False,
 )
 
 _RequiredDeleteLocalGatewayRouteRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteLocalGatewayRouteRequestRequestTypeDef",
     {
         "LocalGatewayRouteTableId": str,
     },
@@ -6135,15 +6061,14 @@
 
 DeleteQueuedReservedInstancesErrorTypeDef = TypedDict(
     "DeleteQueuedReservedInstancesErrorTypeDef",
     {
         "Code": DeleteQueuedReservedInstancesErrorCodeType,
         "Message": str,
     },
-    total=False,
 )
 
 _RequiredDeleteQueuedReservedInstancesRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteQueuedReservedInstancesRequestRequestTypeDef",
     {
         "ReservedInstancesIds": Sequence[str],
     },
@@ -6163,15 +6088,14 @@
     pass
 
 SuccessfulQueuedPurchaseDeletionTypeDef = TypedDict(
     "SuccessfulQueuedPurchaseDeletionTypeDef",
     {
         "ReservedInstancesId": str,
     },
-    total=False,
 )
 
 _RequiredDeleteRouteRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteRouteRequestRequestTypeDef",
     {
         "RouteTableId": str,
     },
@@ -7062,15 +6986,14 @@
 
 InstanceTagNotificationAttributeTypeDef = TypedDict(
     "InstanceTagNotificationAttributeTypeDef",
     {
         "InstanceTagKeys": List[str],
         "IncludeAllTagsOfInstance": bool,
     },
-    total=False,
 )
 
 DeregisterTransitGatewayMulticastGroupMembersRequestRequestTypeDef = TypedDict(
     "DeregisterTransitGatewayMulticastGroupMembersRequestRequestTypeDef",
     {
         "TransitGatewayMulticastDomainId": str,
         "GroupIpAddress": str,
@@ -7083,15 +7006,14 @@
 TransitGatewayMulticastDeregisteredGroupMembersTypeDef = TypedDict(
     "TransitGatewayMulticastDeregisteredGroupMembersTypeDef",
     {
         "TransitGatewayMulticastDomainId": str,
         "DeregisteredNetworkInterfaceIds": List[str],
         "GroupIpAddress": str,
     },
-    total=False,
 )
 
 DeregisterTransitGatewayMulticastGroupSourcesRequestRequestTypeDef = TypedDict(
     "DeregisterTransitGatewayMulticastGroupSourcesRequestRequestTypeDef",
     {
         "TransitGatewayMulticastDomainId": str,
         "GroupIpAddress": str,
@@ -7104,15 +7026,14 @@
 TransitGatewayMulticastDeregisteredGroupSourcesTypeDef = TypedDict(
     "TransitGatewayMulticastDeregisteredGroupSourcesTypeDef",
     {
         "TransitGatewayMulticastDomainId": str,
         "DeregisteredNetworkInterfaceIds": List[str],
         "GroupIpAddress": str,
     },
-    total=False,
 )
 
 DescribeAccountAttributesRequestRequestTypeDef = TypedDict(
     "DescribeAccountAttributesRequestRequestTypeDef",
     {
         "AttributeNames": Sequence[AccountAttributeNameType],
         "DryRun": bool,
@@ -7184,27 +7105,25 @@
 IdFormatTypeDef = TypedDict(
     "IdFormatTypeDef",
     {
         "Deadline": datetime,
         "Resource": str,
         "UseLongIds": bool,
     },
-    total=False,
 )
 
 SubscriptionTypeDef = TypedDict(
     "SubscriptionTypeDef",
     {
         "Source": str,
         "Destination": str,
         "Metric": Literal["aggregate-latency"],
         "Statistic": Literal["p50"],
         "Period": PeriodTypeType,
     },
-    total=False,
 )
 
 WaiterConfigTypeDef = TypedDict(
     "WaiterConfigTypeDef",
     {
         "Delay": int,
         "MaxAttempts": int,
@@ -7254,23 +7173,21 @@
 FastLaunchLaunchTemplateSpecificationResponseTypeDef = TypedDict(
     "FastLaunchLaunchTemplateSpecificationResponseTypeDef",
     {
         "LaunchTemplateId": str,
         "LaunchTemplateName": str,
         "Version": str,
     },
-    total=False,
 )
 
 FastLaunchSnapshotConfigurationResponseTypeDef = TypedDict(
     "FastLaunchSnapshotConfigurationResponseTypeDef",
     {
         "TargetResourceCount": int,
     },
-    total=False,
 )
 
 DescribeFastSnapshotRestoreSuccessItemTypeDef = TypedDict(
     "DescribeFastSnapshotRestoreSuccessItemTypeDef",
     {
         "SnapshotId": str,
         "AvailabilityZone": str,
@@ -7280,15 +7197,14 @@
         "OwnerAlias": str,
         "EnablingTime": datetime,
         "OptimizingTime": datetime,
         "EnabledTime": datetime,
         "DisablingTime": datetime,
         "DisabledTime": datetime,
     },
-    total=False,
 )
 
 _RequiredDescribeFleetHistoryRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeFleetHistoryRequestRequestTypeDef",
     {
         "FleetId": str,
         "StartTime": Union[datetime, str],
@@ -7339,15 +7255,14 @@
         "Duration": int,
         "HourlyPrice": str,
         "InstanceFamily": str,
         "OfferingId": str,
         "PaymentOption": PaymentOptionType,
         "UpfrontPrice": str,
     },
-    total=False,
 )
 
 DescribeIdFormatRequestRequestTypeDef = TypedDict(
     "DescribeIdFormatRequestRequestTypeDef",
     {
         "Resource": str,
     },
@@ -7458,15 +7373,14 @@
 
 InstanceCreditSpecificationTypeDef = TypedDict(
     "InstanceCreditSpecificationTypeDef",
     {
         "InstanceId": str,
         "CpuCredits": str,
     },
-    total=False,
 )
 
 DescribeInstanceEventNotificationAttributesRequestRequestTypeDef = TypedDict(
     "DescribeInstanceEventNotificationAttributesRequestRequestTypeDef",
     {
         "DryRun": bool,
     },
@@ -7476,24 +7390,22 @@
 InstanceTypeOfferingTypeDef = TypedDict(
     "InstanceTypeOfferingTypeDef",
     {
         "InstanceType": InstanceTypeType,
         "LocationType": LocationTypeType,
         "Location": str,
     },
-    total=False,
 )
 
 MovingAddressStatusTypeDef = TypedDict(
     "MovingAddressStatusTypeDef",
     {
         "MoveStatus": MoveStatusType,
         "PublicIp": str,
     },
-    total=False,
 )
 
 DescribeNetworkInterfaceAttributeRequestNetworkInterfaceDescribeAttributeTypeDef = TypedDict(
     "DescribeNetworkInterfaceAttributeRequestNetworkInterfaceDescribeAttributeTypeDef",
     {
         "Attribute": NetworkInterfaceAttributeType,
         "DryRun": bool,
@@ -7525,15 +7437,14 @@
 PrefixListTypeDef = TypedDict(
     "PrefixListTypeDef",
     {
         "Cidrs": List[str],
         "PrefixListId": str,
         "PrefixListName": str,
     },
-    total=False,
 )
 
 DescribePrincipalIdFormatRequestDescribePrincipalIdFormatPaginateTypeDef = TypedDict(
     "DescribePrincipalIdFormatRequestDescribePrincipalIdFormatPaginateTypeDef",
     {
         "DryRun": bool,
         "Resources": Sequence[str],
@@ -7556,15 +7467,14 @@
 RegionTypeDef = TypedDict(
     "RegionTypeDef",
     {
         "Endpoint": str,
         "RegionName": str,
         "OptInStatus": str,
     },
-    total=False,
 )
 
 ScheduledInstanceRecurrenceRequestTypeDef = TypedDict(
     "ScheduledInstanceRecurrenceRequestTypeDef",
     {
         "Frequency": str,
         "Interval": int,
@@ -7615,15 +7525,14 @@
 SecurityGroupReferenceTypeDef = TypedDict(
     "SecurityGroupReferenceTypeDef",
     {
         "GroupId": str,
         "ReferencingVpcId": str,
         "VpcPeeringConnectionId": str,
     },
-    total=False,
 )
 
 _RequiredDescribeSnapshotAttributeRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeSnapshotAttributeRequestRequestTypeDef",
     {
         "Attribute": SnapshotAttributeNameType,
         "SnapshotId": str,
@@ -7665,15 +7574,14 @@
 
 ProductCodeTypeDef = TypedDict(
     "ProductCodeTypeDef",
     {
         "ProductCodeId": str,
         "ProductCodeType": ProductCodeValuesType,
     },
-    total=False,
 )
 
 DescribeSpotDatafeedSubscriptionRequestRequestTypeDef = TypedDict(
     "DescribeSpotDatafeedSubscriptionRequestRequestTypeDef",
     {
         "DryRun": bool,
     },
@@ -7773,15 +7681,14 @@
     {
         "AvailabilityZone": str,
         "InstanceType": InstanceTypeType,
         "ProductDescription": RIProductDescriptionType,
         "SpotPrice": str,
         "Timestamp": datetime,
     },
-    total=False,
 )
 
 _RequiredDescribeStaleSecurityGroupsRequestDescribeStaleSecurityGroupsPaginateTypeDef = TypedDict(
     "_RequiredDescribeStaleSecurityGroupsRequestDescribeStaleSecurityGroupsPaginateTypeDef",
     {
         "VpcId": str,
     },
@@ -7830,26 +7737,24 @@
         "TaskStartTime": datetime,
         "Bucket": str,
         "S3objectKey": str,
         "ProgressPercentage": int,
         "StoreTaskState": str,
         "StoreTaskFailureReason": str,
     },
-    total=False,
 )
 
 TagDescriptionTypeDef = TypedDict(
     "TagDescriptionTypeDef",
     {
         "Key": str,
         "ResourceId": str,
         "ResourceType": ResourceTypeType,
         "Value": str,
     },
-    total=False,
 )
 
 _RequiredDescribeVolumeAttributeRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeVolumeAttributeRequestRequestTypeDef",
     {
         "Attribute": VolumeAttributeNameType,
         "VolumeId": str,
@@ -7905,15 +7810,14 @@
         "OriginalVolumeType": VolumeTypeType,
         "OriginalThroughput": int,
         "OriginalMultiAttachEnabled": bool,
         "Progress": int,
         "StartTime": datetime,
         "EndTime": datetime,
     },
-    total=False,
 )
 
 _RequiredDescribeVpcAttributeRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeVpcAttributeRequestRequestTypeDef",
     {
         "Attribute": VpcAttributeNameType,
         "VpcId": str,
@@ -7975,15 +7879,14 @@
 DestinationOptionsResponseTypeDef = TypedDict(
     "DestinationOptionsResponseTypeDef",
     {
         "FileFormat": DestinationFileFormatType,
         "HiveCompatiblePartitions": bool,
         "PerHourPartition": bool,
     },
-    total=False,
 )
 
 _RequiredDetachClassicLinkVpcRequestInstanceDetachClassicLinkVpcTypeDef = TypedDict(
     "_RequiredDetachClassicLinkVpcRequestInstanceDetachClassicLinkVpcTypeDef",
     {
         "VpcId": str,
     },
@@ -8252,15 +8155,14 @@
     pass
 
 DeviceOptionsTypeDef = TypedDict(
     "DeviceOptionsTypeDef",
     {
         "TenantId": str,
     },
-    total=False,
 )
 
 _RequiredDisableAddressTransferRequestRequestTypeDef = TypedDict(
     "_RequiredDisableAddressTransferRequestRequestTypeDef",
     {
         "AllocationId": str,
     },
@@ -8337,15 +8239,14 @@
 
 DisableFastSnapshotRestoreStateErrorTypeDef = TypedDict(
     "DisableFastSnapshotRestoreStateErrorTypeDef",
     {
         "Code": str,
         "Message": str,
     },
-    total=False,
 )
 
 DisableFastSnapshotRestoreSuccessItemTypeDef = TypedDict(
     "DisableFastSnapshotRestoreSuccessItemTypeDef",
     {
         "SnapshotId": str,
         "AvailabilityZone": str,
@@ -8355,15 +8256,14 @@
         "OwnerAlias": str,
         "EnablingTime": datetime,
         "OptimizingTime": datetime,
         "EnabledTime": datetime,
         "DisablingTime": datetime,
         "DisabledTime": datetime,
     },
-    total=False,
 )
 
 _RequiredDisableFastSnapshotRestoresRequestRequestTypeDef = TypedDict(
     "_RequiredDisableFastSnapshotRestoresRequestRequestTypeDef",
     {
         "AvailabilityZones": Sequence[str],
         "SourceSnapshotIds": Sequence[str],
@@ -8483,15 +8383,14 @@
         "TransitGatewayAttachmentId": str,
         "ResourceId": str,
         "ResourceType": TransitGatewayAttachmentResourceTypeType,
         "TransitGatewayRouteTableId": str,
         "State": TransitGatewayPropagationStateType,
         "TransitGatewayRouteTableAnnouncementId": str,
     },
-    total=False,
 )
 
 _RequiredDisableVgwRoutePropagationRequestRequestTypeDef = TypedDict(
     "_RequiredDisableVgwRoutePropagationRequestRequestTypeDef",
     {
         "GatewayId": str,
         "RouteTableId": str,
@@ -8851,15 +8750,14 @@
     "DiskImageDescriptionTypeDef",
     {
         "Checksum": str,
         "Format": DiskImageFormatType,
         "ImportManifestUrl": str,
         "Size": int,
     },
-    total=False,
 )
 
 DiskImageDetailTypeDef = TypedDict(
     "DiskImageDetailTypeDef",
     {
         "Bytes": int,
         "Format": DiskImageFormatType,
@@ -8876,43 +8774,39 @@
 
 DiskImageVolumeDescriptionTypeDef = TypedDict(
     "DiskImageVolumeDescriptionTypeDef",
     {
         "Id": str,
         "Size": int,
     },
-    total=False,
 )
 
 DiskInfoTypeDef = TypedDict(
     "DiskInfoTypeDef",
     {
         "SizeInGB": int,
         "Count": int,
         "Type": DiskTypeType,
     },
-    total=False,
 )
 
 DnsEntryTypeDef = TypedDict(
     "DnsEntryTypeDef",
     {
         "DnsName": str,
         "HostedZoneId": str,
     },
-    total=False,
 )
 
 DnsOptionsTypeDef = TypedDict(
     "DnsOptionsTypeDef",
     {
         "DnsRecordIpType": DnsRecordIpTypeType,
         "PrivateDnsOnlyForInboundResolverEndpoint": bool,
     },
-    total=False,
 )
 
 DnsServersOptionsModifyStructureTypeDef = TypedDict(
     "DnsServersOptionsModifyStructureTypeDef",
     {
         "CustomDnsServers": Sequence[str],
         "Enabled": bool,
@@ -8926,15 +8820,14 @@
         "BaselineBandwidthInMbps": int,
         "BaselineThroughputInMBps": float,
         "BaselineIops": int,
         "MaximumBandwidthInMbps": int,
         "MaximumThroughputInMBps": float,
         "MaximumIops": int,
     },
-    total=False,
 )
 
 EbsInstanceBlockDeviceSpecificationTypeDef = TypedDict(
     "EbsInstanceBlockDeviceSpecificationTypeDef",
     {
         "DeleteOnTermination": bool,
         "VolumeId": str,
@@ -8946,59 +8839,53 @@
     "EbsInstanceBlockDeviceTypeDef",
     {
         "AttachTime": datetime,
         "DeleteOnTermination": bool,
         "Status": AttachmentStatusType,
         "VolumeId": str,
     },
-    total=False,
 )
 
 EfaInfoTypeDef = TypedDict(
     "EfaInfoTypeDef",
     {
         "MaximumEfaInterfaces": int,
     },
-    total=False,
 )
 
 InternetGatewayAttachmentTypeDef = TypedDict(
     "InternetGatewayAttachmentTypeDef",
     {
         "State": AttachmentStatusType,
         "VpcId": str,
     },
-    total=False,
 )
 
 ElasticGpuAssociationTypeDef = TypedDict(
     "ElasticGpuAssociationTypeDef",
     {
         "ElasticGpuId": str,
         "ElasticGpuAssociationId": str,
         "ElasticGpuAssociationState": str,
         "ElasticGpuAssociationTime": str,
     },
-    total=False,
 )
 
 ElasticGpuHealthTypeDef = TypedDict(
     "ElasticGpuHealthTypeDef",
     {
         "Status": ElasticGpuStatusType,
     },
-    total=False,
 )
 
 ElasticGpuSpecificationResponseTypeDef = TypedDict(
     "ElasticGpuSpecificationResponseTypeDef",
     {
         "Type": str,
     },
-    total=False,
 )
 
 ElasticGpuSpecificationTypeDef = TypedDict(
     "ElasticGpuSpecificationTypeDef",
     {
         "Type": str,
     },
@@ -9008,15 +8895,14 @@
     "ElasticInferenceAcceleratorAssociationTypeDef",
     {
         "ElasticInferenceAcceleratorArn": str,
         "ElasticInferenceAcceleratorAssociationId": str,
         "ElasticInferenceAcceleratorAssociationState": str,
         "ElasticInferenceAcceleratorAssociationTime": datetime,
     },
-    total=False,
 )
 
 _RequiredElasticInferenceAcceleratorTypeDef = TypedDict(
     "_RequiredElasticInferenceAcceleratorTypeDef",
     {
         "Type": str,
     },
@@ -9137,15 +9023,14 @@
 
 EnableFastSnapshotRestoreStateErrorTypeDef = TypedDict(
     "EnableFastSnapshotRestoreStateErrorTypeDef",
     {
         "Code": str,
         "Message": str,
     },
-    total=False,
 )
 
 EnableFastSnapshotRestoreSuccessItemTypeDef = TypedDict(
     "EnableFastSnapshotRestoreSuccessItemTypeDef",
     {
         "SnapshotId": str,
         "AvailabilityZone": str,
@@ -9155,15 +9040,14 @@
         "OwnerAlias": str,
         "EnablingTime": datetime,
         "OptimizingTime": datetime,
         "EnabledTime": datetime,
         "DisablingTime": datetime,
         "DisabledTime": datetime,
     },
-    total=False,
 )
 
 _RequiredEnableFastSnapshotRestoresRequestRequestTypeDef = TypedDict(
     "_RequiredEnableFastSnapshotRestoresRequestRequestTypeDef",
     {
         "AvailabilityZones": Sequence[str],
         "SourceSnapshotIds": Sequence[str],
@@ -9411,39 +9295,36 @@
 )
 
 EnclaveOptionsTypeDef = TypedDict(
     "EnclaveOptionsTypeDef",
     {
         "Enabled": bool,
     },
-    total=False,
 )
 
 EventInformationTypeDef = TypedDict(
     "EventInformationTypeDef",
     {
         "EventDescription": str,
         "EventSubType": str,
         "InstanceId": str,
     },
-    total=False,
 )
 
 TransitGatewayRouteTableRouteTypeDef = TypedDict(
     "TransitGatewayRouteTableRouteTypeDef",
     {
         "DestinationCidr": str,
         "State": str,
         "RouteOrigin": str,
         "PrefixListId": str,
         "AttachmentId": str,
         "ResourceId": str,
         "ResourceType": str,
     },
-    total=False,
 )
 
 _RequiredExportClientVpnClientCertificateRevocationListRequestRequestTypeDef = TypedDict(
     "_RequiredExportClientVpnClientCertificateRevocationListRequestRequestTypeDef",
     {
         "ClientVpnEndpointId": str,
     },
@@ -9511,35 +9392,32 @@
 
 ExportTaskS3LocationTypeDef = TypedDict(
     "ExportTaskS3LocationTypeDef",
     {
         "S3Bucket": str,
         "S3Prefix": str,
     },
-    total=False,
 )
 
 ExportToS3TaskTypeDef = TypedDict(
     "ExportToS3TaskTypeDef",
     {
         "ContainerFormat": Literal["ova"],
         "DiskImageFormat": DiskImageFormatType,
         "S3Bucket": str,
         "S3Key": str,
     },
-    total=False,
 )
 
 InstanceExportDetailsTypeDef = TypedDict(
     "InstanceExportDetailsTypeDef",
     {
         "InstanceId": str,
         "TargetEnvironment": ExportEnvironmentType,
     },
-    total=False,
 )
 
 ExportTransitGatewayRoutesResultTypeDef = TypedDict(
     "ExportTransitGatewayRoutesResultTypeDef",
     {
         "S3Location": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
@@ -9548,27 +9426,25 @@
 
 FilterPortRangeTypeDef = TypedDict(
     "FilterPortRangeTypeDef",
     {
         "FromPort": int,
         "ToPort": int,
     },
-    total=False,
 )
 
 TargetCapacitySpecificationTypeDef = TypedDict(
     "TargetCapacitySpecificationTypeDef",
     {
         "TotalTargetCapacity": int,
         "OnDemandTargetCapacity": int,
         "SpotTargetCapacity": int,
         "DefaultTargetCapacityType": DefaultTargetCapacityTypeType,
         "TargetCapacityUnitType": TargetCapacityUnitTypeType,
     },
-    total=False,
 )
 
 FleetLaunchTemplateSpecificationRequestTypeDef = TypedDict(
     "FleetLaunchTemplateSpecificationRequestTypeDef",
     {
         "LaunchTemplateId": str,
         "LaunchTemplateName": str,
@@ -9580,15 +9456,14 @@
 FleetLaunchTemplateSpecificationTypeDef = TypedDict(
     "FleetLaunchTemplateSpecificationTypeDef",
     {
         "LaunchTemplateId": str,
         "LaunchTemplateName": str,
         "Version": str,
     },
-    total=False,
 )
 
 PlacementTypeDef = TypedDict(
     "PlacementTypeDef",
     {
         "AvailabilityZone": str,
         "Affinity": str,
@@ -9604,15 +9479,14 @@
 )
 
 PlacementResponseTypeDef = TypedDict(
     "PlacementResponseTypeDef",
     {
         "GroupName": str,
     },
-    total=False,
 )
 
 FleetSpotCapacityRebalanceRequestTypeDef = TypedDict(
     "FleetSpotCapacityRebalanceRequestTypeDef",
     {
         "ReplacementStrategy": FleetReplacementStrategyType,
         "TerminationDelay": int,
@@ -9622,52 +9496,47 @@
 
 FleetSpotCapacityRebalanceTypeDef = TypedDict(
     "FleetSpotCapacityRebalanceTypeDef",
     {
         "ReplacementStrategy": FleetReplacementStrategyType,
         "TerminationDelay": int,
     },
-    total=False,
 )
 
 FpgaDeviceMemoryInfoTypeDef = TypedDict(
     "FpgaDeviceMemoryInfoTypeDef",
     {
         "SizeInMiB": int,
     },
-    total=False,
 )
 
 LoadPermissionTypeDef = TypedDict(
     "LoadPermissionTypeDef",
     {
         "UserId": str,
         "Group": Literal["all"],
     },
-    total=False,
 )
 
 FpgaImageStateTypeDef = TypedDict(
     "FpgaImageStateTypeDef",
     {
         "Code": FpgaImageStateCodeType,
         "Message": str,
     },
-    total=False,
 )
 
 PciIdTypeDef = TypedDict(
     "PciIdTypeDef",
     {
         "DeviceId": str,
         "VendorId": str,
         "SubsystemId": str,
         "SubsystemVendorId": str,
     },
-    total=False,
 )
 
 _RequiredGetAssociatedEnclaveCertificateIamRolesRequestRequestTypeDef = TypedDict(
     "_RequiredGetAssociatedEnclaveCertificateIamRolesRequestRequestTypeDef",
     {
         "CertificateArn": str,
     },
@@ -9731,15 +9600,14 @@
 
 Ipv6CidrAssociationTypeDef = TypedDict(
     "Ipv6CidrAssociationTypeDef",
     {
         "Ipv6Cidr": str,
         "AssociatedResource": str,
     },
-    total=False,
 )
 
 _RequiredGetCapacityReservationUsageRequestRequestTypeDef = TypedDict(
     "_RequiredGetCapacityReservationUsageRequestRequestTypeDef",
     {
         "CapacityReservationId": str,
     },
@@ -9762,15 +9630,14 @@
 
 InstanceUsageTypeDef = TypedDict(
     "InstanceUsageTypeDef",
     {
         "AccountId": str,
         "UsedInstanceCount": int,
     },
-    total=False,
 )
 
 GetConsoleOutputRequestInstanceConsoleOutputTypeDef = TypedDict(
     "GetConsoleOutputRequestInstanceConsoleOutputTypeDef",
     {
         "DryRun": bool,
         "Latest": bool,
@@ -9860,15 +9727,14 @@
 
 InstanceFamilyCreditSpecificationTypeDef = TypedDict(
     "InstanceFamilyCreditSpecificationTypeDef",
     {
         "InstanceFamily": UnlimitedSupportedInstanceFamilyType,
         "CpuCredits": str,
     },
-    total=False,
 )
 
 GetEbsDefaultKmsKeyIdRequestRequestTypeDef = TypedDict(
     "GetEbsDefaultKmsKeyIdRequestRequestTypeDef",
     {
         "DryRun": bool,
     },
@@ -9966,23 +9832,21 @@
         "HostIdSet": List[str],
         "HostReservationId": str,
         "HourlyPrice": str,
         "InstanceFamily": str,
         "PaymentOption": PaymentOptionType,
         "UpfrontPrice": str,
     },
-    total=False,
 )
 
 InstanceTypeInfoFromInstanceRequirementsTypeDef = TypedDict(
     "InstanceTypeInfoFromInstanceRequirementsTypeDef",
     {
         "InstanceType": str,
     },
-    total=False,
 )
 
 _RequiredGetInstanceUefiDataRequestRequestTypeDef = TypedDict(
     "_RequiredGetInstanceUefiDataRequestRequestTypeDef",
     {
         "InstanceId": str,
     },
@@ -10072,15 +9936,14 @@
         "ResourceName": str,
         "ResourceComplianceStatus": IpamComplianceStatusType,
         "ResourceOverlapStatus": IpamOverlapStatusType,
         "VpcId": str,
         "SampledStartTime": datetime,
         "SampledEndTime": datetime,
     },
-    total=False,
 )
 
 _RequiredGetLaunchTemplateDataRequestRequestTypeDef = TypedDict(
     "_RequiredGetLaunchTemplateDataRequestRequestTypeDef",
     {
         "InstanceId": str,
     },
@@ -10144,15 +10007,14 @@
 
 PrefixListAssociationTypeDef = TypedDict(
     "PrefixListAssociationTypeDef",
     {
         "ResourceId": str,
         "ResourceOwner": str,
     },
-    total=False,
 )
 
 _RequiredGetManagedPrefixListEntriesRequestGetManagedPrefixListEntriesPaginateTypeDef = TypedDict(
     "_RequiredGetManagedPrefixListEntriesRequestGetManagedPrefixListEntriesPaginateTypeDef",
     {
         "PrefixListId": str,
     },
@@ -10198,15 +10060,14 @@
 
 PrefixListEntryTypeDef = TypedDict(
     "PrefixListEntryTypeDef",
     {
         "Cidr": str,
         "Description": str,
     },
-    total=False,
 )
 
 _RequiredGetNetworkInsightsAccessScopeAnalysisFindingsRequestGetNetworkInsightsAccessScopeAnalysisFindingsPaginateTypeDef = TypedDict(
     "_RequiredGetNetworkInsightsAccessScopeAnalysisFindingsRequestGetNetworkInsightsAccessScopeAnalysisFindingsPaginateTypeDef",
     {
         "NetworkInsightsAccessScopeAnalysisId": str,
     },
@@ -10308,15 +10169,14 @@
 ReservationValueTypeDef = TypedDict(
     "ReservationValueTypeDef",
     {
         "HourlyPrice": str,
         "RemainingTotalValue": str,
         "RemainingUpfrontValue": str,
     },
-    total=False,
 )
 
 GetSerialConsoleAccessStatusRequestRequestTypeDef = TypedDict(
     "GetSerialConsoleAccessStatusRequestRequestTypeDef",
     {
         "DryRun": bool,
     },
@@ -10334,47 +10194,43 @@
 SpotPlacementScoreTypeDef = TypedDict(
     "SpotPlacementScoreTypeDef",
     {
         "Region": str,
         "AvailabilityZoneId": str,
         "Score": int,
     },
-    total=False,
 )
 
 TransitGatewayAttachmentPropagationTypeDef = TypedDict(
     "TransitGatewayAttachmentPropagationTypeDef",
     {
         "TransitGatewayRouteTableId": str,
         "State": TransitGatewayPropagationStateType,
     },
-    total=False,
 )
 
 TransitGatewayRouteTableAssociationTypeDef = TypedDict(
     "TransitGatewayRouteTableAssociationTypeDef",
     {
         "TransitGatewayAttachmentId": str,
         "ResourceId": str,
         "ResourceType": TransitGatewayAttachmentResourceTypeType,
         "State": TransitGatewayAssociationStateType,
     },
-    total=False,
 )
 
 TransitGatewayRouteTablePropagationTypeDef = TypedDict(
     "TransitGatewayRouteTablePropagationTypeDef",
     {
         "TransitGatewayAttachmentId": str,
         "ResourceId": str,
         "ResourceType": TransitGatewayAttachmentResourceTypeType,
         "State": TransitGatewayPropagationStateType,
         "TransitGatewayRouteTableAnnouncementId": str,
     },
-    total=False,
 )
 
 _RequiredGetVerifiedAccessEndpointPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredGetVerifiedAccessEndpointPolicyRequestRequestTypeDef",
     {
         "VerifiedAccessEndpointId": str,
     },
@@ -10484,15 +10340,14 @@
     "VpnConnectionDeviceTypeTypeDef",
     {
         "VpnConnectionDeviceTypeId": str,
         "Vendor": str,
         "Platform": str,
         "Software": str,
     },
-    total=False,
 )
 
 _RequiredGetVpnTunnelReplacementStatusRequestRequestTypeDef = TypedDict(
     "_RequiredGetVpnTunnelReplacementStatusRequestRequestTypeDef",
     {
         "VpnConnectionId": str,
         "VpnTunnelOutsideIpAddress": str,
@@ -10515,23 +10370,21 @@
 MaintenanceDetailsTypeDef = TypedDict(
     "MaintenanceDetailsTypeDef",
     {
         "PendingMaintenance": str,
         "MaintenanceAutoAppliedAfter": datetime,
         "LastMaintenanceApplied": datetime,
     },
-    total=False,
 )
 
 GpuDeviceMemoryInfoTypeDef = TypedDict(
     "GpuDeviceMemoryInfoTypeDef",
     {
         "SizeInMiB": int,
     },
-    total=False,
 )
 
 HibernationOptionsRequestTypeDef = TypedDict(
     "HibernationOptionsRequestTypeDef",
     {
         "Configured": bool,
     },
@@ -10547,45 +10400,41 @@
 )
 
 HibernationOptionsTypeDef = TypedDict(
     "HibernationOptionsTypeDef",
     {
         "Configured": bool,
     },
-    total=False,
 )
 
 HostInstanceTypeDef = TypedDict(
     "HostInstanceTypeDef",
     {
         "InstanceId": str,
         "InstanceType": str,
         "OwnerId": str,
     },
-    total=False,
 )
 
 HostPropertiesTypeDef = TypedDict(
     "HostPropertiesTypeDef",
     {
         "Cores": int,
         "InstanceType": str,
         "InstanceFamily": str,
         "Sockets": int,
         "TotalVCpus": int,
     },
-    total=False,
 )
 
 IKEVersionsListValueTypeDef = TypedDict(
     "IKEVersionsListValueTypeDef",
     {
         "Value": str,
     },
-    total=False,
 )
 
 IKEVersionsRequestListValueTypeDef = TypedDict(
     "IKEVersionsRequestListValueTypeDef",
     {
         "Value": str,
     },
@@ -10594,15 +10443,14 @@
 
 IamInstanceProfileTypeDef = TypedDict(
     "IamInstanceProfileTypeDef",
     {
         "Arn": str,
         "Id": str,
     },
-    total=False,
 )
 
 IamInstanceProfileResponseMetadataTypeDef = TypedDict(
     "IamInstanceProfileResponseMetadataTypeDef",
     {
         "Arn": str,
         "Id": str,
@@ -10614,15 +10462,14 @@
     "LaunchPermissionTypeDef",
     {
         "Group": Literal["all"],
         "UserId": str,
         "OrganizationArn": str,
         "OrganizationalUnitArn": str,
     },
-    total=False,
 )
 
 UserBucketTypeDef = TypedDict(
     "UserBucketTypeDef",
     {
         "S3Bucket": str,
         "S3Key": str,
@@ -10635,24 +10482,22 @@
     {
         "ImageId": str,
         "Name": str,
         "Description": str,
         "RecycleBinEnterTime": datetime,
         "RecycleBinExitTime": datetime,
     },
-    total=False,
 )
 
 StateReasonTypeDef = TypedDict(
     "StateReasonTypeDef",
     {
         "Code": str,
         "Message": str,
     },
-    total=False,
 )
 
 _RequiredImportClientVpnClientCertificateRevocationListRequestRequestTypeDef = TypedDict(
     "_RequiredImportClientVpnClientCertificateRevocationListRequestRequestTypeDef",
     {
         "ClientVpnEndpointId": str,
         "CertificateRevocationList": str,
@@ -10689,15 +10534,14 @@
 )
 
 ImportImageLicenseConfigurationResponseTypeDef = TypedDict(
     "ImportImageLicenseConfigurationResponseTypeDef",
     {
         "LicenseConfigurationArn": str,
     },
-    total=False,
 )
 
 UserDataTypeDef = TypedDict(
     "UserDataTypeDef",
     {
         "Data": str,
     },
@@ -10707,24 +10551,22 @@
 InferenceDeviceInfoTypeDef = TypedDict(
     "InferenceDeviceInfoTypeDef",
     {
         "Count": int,
         "Name": str,
         "Manufacturer": str,
     },
-    total=False,
 )
 
 InstanceCountTypeDef = TypedDict(
     "InstanceCountTypeDef",
     {
         "InstanceCount": int,
         "State": ListingStateType,
     },
-    total=False,
 )
 
 _RequiredInstanceCreditSpecificationRequestTypeDef = TypedDict(
     "_RequiredInstanceCreditSpecificationRequestTypeDef",
     {
         "InstanceId": str,
     },
@@ -10747,23 +10589,21 @@
     "InstanceEventWindowTimeRangeTypeDef",
     {
         "StartWeekDay": WeekDayType,
         "StartHour": int,
         "EndWeekDay": WeekDayType,
         "EndHour": int,
     },
-    total=False,
 )
 
 InstanceIpv4PrefixTypeDef = TypedDict(
     "InstanceIpv4PrefixTypeDef",
     {
         "Ipv4Prefix": str,
     },
-    total=False,
 )
 
 InstanceIpv6AddressRequestTypeDef = TypedDict(
     "InstanceIpv6AddressRequestTypeDef",
     {
         "Ipv6Address": str,
     },
@@ -10771,15 +10611,14 @@
 )
 
 InstanceIpv6PrefixTypeDef = TypedDict(
     "InstanceIpv6PrefixTypeDef",
     {
         "Ipv6Prefix": str,
     },
-    total=False,
 )
 
 InstanceMaintenanceOptionsRequestTypeDef = TypedDict(
     "InstanceMaintenanceOptionsRequestTypeDef",
     {
         "AutoRecovery": InstanceAutoRecoveryStateType,
     },
@@ -10795,15 +10634,14 @@
 )
 
 InstanceMaintenanceOptionsTypeDef = TypedDict(
     "InstanceMaintenanceOptionsTypeDef",
     {
         "AutoRecovery": InstanceAutoRecoveryStateType,
     },
-    total=False,
 )
 
 SpotMarketOptionsTypeDef = TypedDict(
     "SpotMarketOptionsTypeDef",
     {
         "MaxPrice": str,
         "SpotInstanceType": SpotInstanceTypeType,
@@ -10845,48 +10683,44 @@
         "State": InstanceMetadataOptionsStateType,
         "HttpTokens": HttpTokensStateType,
         "HttpPutResponseHopLimit": int,
         "HttpEndpoint": InstanceMetadataEndpointStateType,
         "HttpProtocolIpv6": InstanceMetadataProtocolStateType,
         "InstanceMetadataTags": InstanceMetadataTagsStateType,
     },
-    total=False,
 )
 
 MonitoringTypeDef = TypedDict(
     "MonitoringTypeDef",
     {
         "State": MonitoringStateType,
     },
-    total=False,
 )
 
 InstanceNetworkInterfaceAssociationTypeDef = TypedDict(
     "InstanceNetworkInterfaceAssociationTypeDef",
     {
         "CarrierIp": str,
         "CustomerOwnedIp": str,
         "IpOwnerId": str,
         "PublicDnsName": str,
         "PublicIp": str,
     },
-    total=False,
 )
 
 InstanceNetworkInterfaceAttachmentTypeDef = TypedDict(
     "InstanceNetworkInterfaceAttachmentTypeDef",
     {
         "AttachTime": datetime,
         "AttachmentId": str,
         "DeleteOnTermination": bool,
         "DeviceIndex": int,
         "Status": AttachmentStatusType,
         "NetworkCardIndex": int,
     },
-    total=False,
 )
 
 MemoryGiBPerVCpuRequestTypeDef = TypedDict(
     "MemoryGiBPerVCpuRequestTypeDef",
     {
         "Min": float,
         "Max": float,
@@ -10959,69 +10793,62 @@
 
 MemoryGiBPerVCpuTypeDef = TypedDict(
     "MemoryGiBPerVCpuTypeDef",
     {
         "Min": float,
         "Max": float,
     },
-    total=False,
 )
 
 MemoryMiBTypeDef = TypedDict(
     "MemoryMiBTypeDef",
     {
         "Min": int,
         "Max": int,
     },
-    total=False,
 )
 
 NetworkBandwidthGbpsTypeDef = TypedDict(
     "NetworkBandwidthGbpsTypeDef",
     {
         "Min": float,
         "Max": float,
     },
-    total=False,
 )
 
 NetworkInterfaceCountTypeDef = TypedDict(
     "NetworkInterfaceCountTypeDef",
     {
         "Min": int,
         "Max": int,
     },
-    total=False,
 )
 
 TotalLocalStorageGBTypeDef = TypedDict(
     "TotalLocalStorageGBTypeDef",
     {
         "Min": float,
         "Max": float,
     },
-    total=False,
 )
 
 VCpuCountRangeTypeDef = TypedDict(
     "VCpuCountRangeTypeDef",
     {
         "Min": int,
         "Max": int,
     },
-    total=False,
 )
 
 InstanceStateTypeDef = TypedDict(
     "InstanceStateTypeDef",
     {
         "Code": int,
         "Name": InstanceStateNameType,
     },
-    total=False,
 )
 
 InstanceStateResponseMetadataTypeDef = TypedDict(
     "InstanceStateResponseMetadataTypeDef",
     {
         "Code": int,
         "Name": InstanceStateNameType,
@@ -11032,84 +10859,76 @@
 InstanceStatusDetailsTypeDef = TypedDict(
     "InstanceStatusDetailsTypeDef",
     {
         "ImpairedSince": datetime,
         "Name": Literal["reachability"],
         "Status": StatusTypeType,
     },
-    total=False,
 )
 
 InstanceStatusEventTypeDef = TypedDict(
     "InstanceStatusEventTypeDef",
     {
         "InstanceEventId": str,
         "Code": EventCodeType,
         "Description": str,
         "NotAfter": datetime,
         "NotBefore": datetime,
         "NotBeforeDeadline": datetime,
     },
-    total=False,
 )
 
 LicenseConfigurationTypeDef = TypedDict(
     "LicenseConfigurationTypeDef",
     {
         "LicenseConfigurationArn": str,
     },
-    total=False,
 )
 
 PrivateDnsNameOptionsResponseTypeDef = TypedDict(
     "PrivateDnsNameOptionsResponseTypeDef",
     {
         "HostnameType": HostnameTypeType,
         "EnableResourceNameDnsARecord": bool,
         "EnableResourceNameDnsAAAARecord": bool,
     },
-    total=False,
 )
 
 MemoryInfoTypeDef = TypedDict(
     "MemoryInfoTypeDef",
     {
         "SizeInMiB": int,
     },
-    total=False,
 )
 
 PlacementGroupInfoTypeDef = TypedDict(
     "PlacementGroupInfoTypeDef",
     {
         "SupportedStrategies": List[PlacementGroupStrategyType],
     },
-    total=False,
 )
 
 ProcessorInfoTypeDef = TypedDict(
     "ProcessorInfoTypeDef",
     {
         "SupportedArchitectures": List[ArchitectureTypeType],
         "SustainedClockSpeedInGhz": float,
         "SupportedFeatures": List[Literal["amd-sev-snp"]],
     },
-    total=False,
 )
 
 VCpuInfoTypeDef = TypedDict(
     "VCpuInfoTypeDef",
     {
         "DefaultVCpus": int,
         "DefaultCores": int,
         "DefaultThreadsPerCore": int,
         "ValidCores": List[int],
         "ValidThreadsPerCore": List[int],
     },
-    total=False,
 )
 
 IpRangeTypeDef = TypedDict(
     "IpRangeTypeDef",
     {
         "CidrIp": str,
         "Description": str,
@@ -11160,90 +10979,80 @@
 
 IpamDiscoveryFailureReasonTypeDef = TypedDict(
     "IpamDiscoveryFailureReasonTypeDef",
     {
         "Code": IpamDiscoveryFailureCodeType,
         "Message": str,
     },
-    total=False,
 )
 
 IpamResourceTagTypeDef = TypedDict(
     "IpamResourceTagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
-    total=False,
 )
 
 IpamOperatingRegionTypeDef = TypedDict(
     "IpamOperatingRegionTypeDef",
     {
         "RegionName": str,
     },
-    total=False,
 )
 
 IpamPoolCidrFailureReasonTypeDef = TypedDict(
     "IpamPoolCidrFailureReasonTypeDef",
     {
         "Code": IpamPoolCidrFailureCodeType,
         "Message": str,
     },
-    total=False,
 )
 
 Ipv4PrefixSpecificationResponseTypeDef = TypedDict(
     "Ipv4PrefixSpecificationResponseTypeDef",
     {
         "Ipv4Prefix": str,
     },
-    total=False,
 )
 
 Ipv6CidrBlockTypeDef = TypedDict(
     "Ipv6CidrBlockTypeDef",
     {
         "Ipv6CidrBlock": str,
     },
-    total=False,
 )
 
 PoolCidrBlockTypeDef = TypedDict(
     "PoolCidrBlockTypeDef",
     {
         "Cidr": str,
     },
-    total=False,
 )
 
 Ipv6PrefixSpecificationResponseTypeDef = TypedDict(
     "Ipv6PrefixSpecificationResponseTypeDef",
     {
         "Ipv6Prefix": str,
     },
-    total=False,
 )
 
 Ipv6PrefixSpecificationTypeDef = TypedDict(
     "Ipv6PrefixSpecificationTypeDef",
     {
         "Ipv6Prefix": str,
     },
-    total=False,
 )
 
 LastErrorTypeDef = TypedDict(
     "LastErrorTypeDef",
     {
         "Message": str,
         "Code": str,
     },
-    total=False,
 )
 
 RunInstancesMonitoringEnabledTypeDef = TypedDict(
     "RunInstancesMonitoringEnabledTypeDef",
     {
         "Enabled": bool,
     },
@@ -11252,15 +11061,14 @@
 SpotPlacementTypeDef = TypedDict(
     "SpotPlacementTypeDef",
     {
         "AvailabilityZone": str,
         "GroupName": str,
         "Tenancy": TenancyType,
     },
-    total=False,
 )
 
 LaunchTemplateEbsBlockDeviceRequestTypeDef = TypedDict(
     "LaunchTemplateEbsBlockDeviceRequestTypeDef",
     {
         "Encrypted": bool,
         "DeleteOnTermination": bool,
@@ -11282,15 +11090,14 @@
         "Iops": int,
         "KmsKeyId": str,
         "SnapshotId": str,
         "VolumeSize": int,
         "VolumeType": VolumeTypeType,
         "Throughput": int,
     },
-    total=False,
 )
 
 LaunchTemplateCpuOptionsRequestTypeDef = TypedDict(
     "LaunchTemplateCpuOptionsRequestTypeDef",
     {
         "CoreCount": int,
         "ThreadsPerCore": int,
@@ -11302,24 +11109,22 @@
 LaunchTemplateCpuOptionsTypeDef = TypedDict(
     "LaunchTemplateCpuOptionsTypeDef",
     {
         "CoreCount": int,
         "ThreadsPerCore": int,
         "AmdSevSnp": AmdSevSnpSpecificationType,
     },
-    total=False,
 )
 
 LaunchTemplateElasticInferenceAcceleratorResponseTypeDef = TypedDict(
     "LaunchTemplateElasticInferenceAcceleratorResponseTypeDef",
     {
         "Type": str,
         "Count": int,
     },
-    total=False,
 )
 
 _RequiredLaunchTemplateElasticInferenceAcceleratorTypeDef = TypedDict(
     "_RequiredLaunchTemplateElasticInferenceAcceleratorTypeDef",
     {
         "Type": str,
     },
@@ -11347,15 +11152,14 @@
 )
 
 LaunchTemplateEnclaveOptionsTypeDef = TypedDict(
     "LaunchTemplateEnclaveOptionsTypeDef",
     {
         "Enabled": bool,
     },
-    total=False,
 )
 
 LaunchTemplateHibernationOptionsRequestTypeDef = TypedDict(
     "LaunchTemplateHibernationOptionsRequestTypeDef",
     {
         "Configured": bool,
     },
@@ -11363,15 +11167,14 @@
 )
 
 LaunchTemplateHibernationOptionsTypeDef = TypedDict(
     "LaunchTemplateHibernationOptionsTypeDef",
     {
         "Configured": bool,
     },
-    total=False,
 )
 
 LaunchTemplateIamInstanceProfileSpecificationRequestTypeDef = TypedDict(
     "LaunchTemplateIamInstanceProfileSpecificationRequestTypeDef",
     {
         "Arn": str,
         "Name": str,
@@ -11381,15 +11184,14 @@
 
 LaunchTemplateIamInstanceProfileSpecificationTypeDef = TypedDict(
     "LaunchTemplateIamInstanceProfileSpecificationTypeDef",
     {
         "Arn": str,
         "Name": str,
     },
-    total=False,
 )
 
 LaunchTemplateInstanceMaintenanceOptionsRequestTypeDef = TypedDict(
     "LaunchTemplateInstanceMaintenanceOptionsRequestTypeDef",
     {
         "AutoRecovery": LaunchTemplateAutoRecoveryStateType,
     },
@@ -11397,15 +11199,14 @@
 )
 
 LaunchTemplateInstanceMaintenanceOptionsTypeDef = TypedDict(
     "LaunchTemplateInstanceMaintenanceOptionsTypeDef",
     {
         "AutoRecovery": LaunchTemplateAutoRecoveryStateType,
     },
-    total=False,
 )
 
 LaunchTemplateSpotMarketOptionsRequestTypeDef = TypedDict(
     "LaunchTemplateSpotMarketOptionsRequestTypeDef",
     {
         "MaxPrice": str,
         "SpotInstanceType": SpotInstanceTypeType,
@@ -11421,15 +11222,14 @@
     {
         "MaxPrice": str,
         "SpotInstanceType": SpotInstanceTypeType,
         "BlockDurationMinutes": int,
         "ValidUntil": datetime,
         "InstanceInterruptionBehavior": InstanceInterruptionBehaviorType,
     },
-    total=False,
 )
 
 LaunchTemplateInstanceMetadataOptionsRequestTypeDef = TypedDict(
     "LaunchTemplateInstanceMetadataOptionsRequestTypeDef",
     {
         "HttpTokens": LaunchTemplateHttpTokensStateType,
         "HttpPutResponseHopLimit": int,
@@ -11446,15 +11246,14 @@
         "State": LaunchTemplateInstanceMetadataOptionsStateType,
         "HttpTokens": LaunchTemplateHttpTokensStateType,
         "HttpPutResponseHopLimit": int,
         "HttpEndpoint": LaunchTemplateInstanceMetadataEndpointStateType,
         "HttpProtocolIpv6": LaunchTemplateInstanceMetadataProtocolIpv6Type,
         "InstanceMetadataTags": LaunchTemplateInstanceMetadataTagsStateType,
     },
-    total=False,
 )
 
 LaunchTemplateLicenseConfigurationRequestTypeDef = TypedDict(
     "LaunchTemplateLicenseConfigurationRequestTypeDef",
     {
         "LicenseConfigurationArn": str,
     },
@@ -11462,15 +11261,14 @@
 )
 
 LaunchTemplateLicenseConfigurationTypeDef = TypedDict(
     "LaunchTemplateLicenseConfigurationTypeDef",
     {
         "LicenseConfigurationArn": str,
     },
-    total=False,
 )
 
 LaunchTemplatePlacementRequestTypeDef = TypedDict(
     "LaunchTemplatePlacementRequestTypeDef",
     {
         "AvailabilityZone": str,
         "Affinity": str,
@@ -11494,15 +11292,14 @@
         "HostId": str,
         "Tenancy": TenancyType,
         "SpreadDomain": str,
         "HostResourceGroupArn": str,
         "PartitionNumber": int,
         "GroupId": str,
     },
-    total=False,
 )
 
 LaunchTemplatePrivateDnsNameOptionsRequestTypeDef = TypedDict(
     "LaunchTemplatePrivateDnsNameOptionsRequestTypeDef",
     {
         "HostnameType": HostnameTypeType,
         "EnableResourceNameDnsARecord": bool,
@@ -11514,15 +11311,14 @@
 LaunchTemplatePrivateDnsNameOptionsTypeDef = TypedDict(
     "LaunchTemplatePrivateDnsNameOptionsTypeDef",
     {
         "HostnameType": HostnameTypeType,
         "EnableResourceNameDnsARecord": bool,
         "EnableResourceNameDnsAAAARecord": bool,
     },
-    total=False,
 )
 
 LaunchTemplateSpecificationTypeDef = TypedDict(
     "LaunchTemplateSpecificationTypeDef",
     {
         "LaunchTemplateId": str,
         "LaunchTemplateName": str,
@@ -11540,15 +11336,14 @@
 )
 
 LaunchTemplatesMonitoringTypeDef = TypedDict(
     "LaunchTemplatesMonitoringTypeDef",
     {
         "Enabled": bool,
     },
-    total=False,
 )
 
 LicenseConfigurationRequestTypeDef = TypedDict(
     "LicenseConfigurationRequestTypeDef",
     {
         "LicenseConfigurationArn": str,
     },
@@ -11602,15 +11397,14 @@
     {
         "SnapshotId": str,
         "RecycleBinEnterTime": datetime,
         "RecycleBinExitTime": datetime,
         "Description": str,
         "VolumeId": str,
     },
-    total=False,
 )
 
 LoadPermissionRequestTypeDef = TypedDict(
     "LoadPermissionRequestTypeDef",
     {
         "Group": Literal["all"],
         "UserId": str,
@@ -11846,15 +11640,14 @@
 )
 
 SuccessfulInstanceCreditSpecificationItemTypeDef = TypedDict(
     "SuccessfulInstanceCreditSpecificationItemTypeDef",
     {
         "InstanceId": str,
     },
-    total=False,
 )
 
 _RequiredModifyInstanceEventStartTimeRequestRequestTypeDef = TypedDict(
     "_RequiredModifyInstanceEventStartTimeRequestRequestTypeDef",
     {
         "InstanceId": str,
         "InstanceEventId": str,
@@ -12105,15 +11898,14 @@
     {
         "AvailabilityZone": str,
         "InstanceCount": int,
         "InstanceType": InstanceTypeType,
         "Platform": str,
         "Scope": scopeType,
     },
-    total=False,
 )
 
 ModifyReservedInstancesResultTypeDef = TypedDict(
     "ModifyReservedInstancesResultTypeDef",
     {
         "ReservedInstancesModificationId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
@@ -12570,15 +12362,14 @@
 PeeringConnectionOptionsTypeDef = TypedDict(
     "PeeringConnectionOptionsTypeDef",
     {
         "AllowDnsResolutionFromRemoteVpc": bool,
         "AllowEgressFromLocalClassicLinkToRemoteVpc": bool,
         "AllowEgressFromLocalVpcToRemoteClassicLink": bool,
     },
-    total=False,
 )
 
 _RequiredModifyVpcTenancyRequestRequestTypeDef = TypedDict(
     "_RequiredModifyVpcTenancyRequestRequestTypeDef",
     {
         "VpcId": str,
         "InstanceTenancy": Literal["default"],
@@ -12811,35 +12602,32 @@
     {
         "ProvisionTime": datetime,
         "Provisioned": str,
         "RequestTime": datetime,
         "Requested": str,
         "Status": str,
     },
-    total=False,
 )
 
 NetworkAclAssociationTypeDef = TypedDict(
     "NetworkAclAssociationTypeDef",
     {
         "NetworkAclAssociationId": str,
         "NetworkAclId": str,
         "SubnetId": str,
     },
-    total=False,
 )
 
 NetworkCardInfoTypeDef = TypedDict(
     "NetworkCardInfoTypeDef",
     {
         "NetworkCardIndex": int,
         "NetworkPerformance": str,
         "MaximumNetworkInterfaces": int,
     },
-    total=False,
 )
 
 NetworkInterfaceAssociationResponseMetadataTypeDef = TypedDict(
     "NetworkInterfaceAssociationResponseMetadataTypeDef",
     {
         "AllocationId": str,
         "AssociationId": str,
@@ -12859,46 +12647,42 @@
         "AssociationId": str,
         "IpOwnerId": str,
         "PublicDnsName": str,
         "PublicIp": str,
         "CustomerOwnedIp": str,
         "CarrierIp": str,
     },
-    total=False,
 )
 
 NetworkInterfaceIpv6AddressTypeDef = TypedDict(
     "NetworkInterfaceIpv6AddressTypeDef",
     {
         "Ipv6Address": str,
     },
-    total=False,
 )
 
 NetworkInterfacePermissionStateTypeDef = TypedDict(
     "NetworkInterfacePermissionStateTypeDef",
     {
         "State": NetworkInterfacePermissionStateCodeType,
         "StatusMessage": str,
     },
-    total=False,
 )
 
 OidcOptionsTypeDef = TypedDict(
     "OidcOptionsTypeDef",
     {
         "Issuer": str,
         "AuthorizationEndpoint": str,
         "TokenEndpoint": str,
         "UserInfoEndpoint": str,
         "ClientId": str,
         "ClientSecret": str,
         "Scope": str,
     },
-    total=False,
 )
 
 PacketHeaderStatementRequestTypeDef = TypedDict(
     "PacketHeaderStatementRequestTypeDef",
     {
         "SourceAddresses": Sequence[str],
         "DestinationAddresses": Sequence[str],
@@ -12918,15 +12702,14 @@
         "DestinationAddresses": List[str],
         "SourcePorts": List[str],
         "DestinationPorts": List[str],
         "SourcePrefixLists": List[str],
         "DestinationPrefixLists": List[str],
         "Protocols": List[ProtocolType],
     },
-    total=False,
 )
 
 PaginatorConfigTypeDef = TypedDict(
     "PaginatorConfigTypeDef",
     {
         "MaxItems": int,
         "PageSize": int,
@@ -12955,83 +12738,74 @@
 
 ResourceStatementTypeDef = TypedDict(
     "ResourceStatementTypeDef",
     {
         "Resources": List[str],
         "ResourceTypes": List[str],
     },
-    total=False,
 )
 
 PeeringAttachmentStatusTypeDef = TypedDict(
     "PeeringAttachmentStatusTypeDef",
     {
         "Code": str,
         "Message": str,
     },
-    total=False,
 )
 
 PeeringTgwInfoTypeDef = TypedDict(
     "PeeringTgwInfoTypeDef",
     {
         "TransitGatewayId": str,
         "CoreNetworkId": str,
         "OwnerId": str,
         "Region": str,
     },
-    total=False,
 )
 
 Phase1DHGroupNumbersListValueTypeDef = TypedDict(
     "Phase1DHGroupNumbersListValueTypeDef",
     {
         "Value": int,
     },
-    total=False,
 )
 
 Phase1EncryptionAlgorithmsListValueTypeDef = TypedDict(
     "Phase1EncryptionAlgorithmsListValueTypeDef",
     {
         "Value": str,
     },
-    total=False,
 )
 
 Phase1IntegrityAlgorithmsListValueTypeDef = TypedDict(
     "Phase1IntegrityAlgorithmsListValueTypeDef",
     {
         "Value": str,
     },
-    total=False,
 )
 
 Phase2DHGroupNumbersListValueTypeDef = TypedDict(
     "Phase2DHGroupNumbersListValueTypeDef",
     {
         "Value": int,
     },
-    total=False,
 )
 
 Phase2EncryptionAlgorithmsListValueTypeDef = TypedDict(
     "Phase2EncryptionAlgorithmsListValueTypeDef",
     {
         "Value": str,
     },
-    total=False,
 )
 
 Phase2IntegrityAlgorithmsListValueTypeDef = TypedDict(
     "Phase2IntegrityAlgorithmsListValueTypeDef",
     {
         "Value": str,
     },
-    total=False,
 )
 
 PlacementResponseMetadataTypeDef = TypedDict(
     "PlacementResponseMetadataTypeDef",
     {
         "AvailabilityZone": str,
         "Affinity": str,
@@ -13050,43 +12824,39 @@
     "PriceScheduleTypeDef",
     {
         "Active": bool,
         "CurrencyCode": Literal["USD"],
         "Price": float,
         "Term": int,
     },
-    total=False,
 )
 
 PricingDetailTypeDef = TypedDict(
     "PricingDetailTypeDef",
     {
         "Count": int,
         "Price": float,
     },
-    total=False,
 )
 
 PrivateDnsDetailsTypeDef = TypedDict(
     "PrivateDnsDetailsTypeDef",
     {
         "PrivateDnsName": str,
     },
-    total=False,
 )
 
 PrivateDnsNameConfigurationTypeDef = TypedDict(
     "PrivateDnsNameConfigurationTypeDef",
     {
         "State": DnsNameStateType,
         "Type": str,
         "Value": str,
         "Name": str,
     },
-    total=False,
 )
 
 PrivateDnsNameOptionsOnLaunchResponseMetadataTypeDef = TypedDict(
     "PrivateDnsNameOptionsOnLaunchResponseMetadataTypeDef",
     {
         "HostnameType": HostnameTypeType,
         "EnableResourceNameDnsARecord": bool,
@@ -13098,15 +12868,14 @@
 PrivateDnsNameOptionsOnLaunchTypeDef = TypedDict(
     "PrivateDnsNameOptionsOnLaunchTypeDef",
     {
         "HostnameType": HostnameTypeType,
         "EnableResourceNameDnsARecord": bool,
         "EnableResourceNameDnsAAAARecord": bool,
     },
-    total=False,
 )
 
 PrivateDnsNameOptionsRequestTypeDef = TypedDict(
     "PrivateDnsNameOptionsRequestTypeDef",
     {
         "HostnameType": HostnameTypeType,
         "EnableResourceNameDnsARecord": bool,
@@ -13126,15 +12895,14 @@
 )
 
 PropagatingVgwTypeDef = TypedDict(
     "PropagatingVgwTypeDef",
     {
         "GatewayId": str,
     },
-    total=False,
 )
 
 _RequiredProvisionPublicIpv4PoolCidrRequestRequestTypeDef = TypedDict(
     "_RequiredProvisionPublicIpv4PoolCidrRequestRequestTypeDef",
     {
         "IpamPoolId": str,
         "PoolId": str,
@@ -13159,15 +12927,14 @@
     "PublicIpv4PoolRangeTypeDef",
     {
         "FirstAddress": str,
         "LastAddress": str,
         "AddressCount": int,
         "AvailableAddressCount": int,
     },
-    total=False,
 )
 
 PurchaseRequestTypeDef = TypedDict(
     "PurchaseRequestTypeDef",
     {
         "InstanceCount": int,
         "PurchaseToken": str,
@@ -13220,27 +12987,25 @@
 
 RecurringChargeTypeDef = TypedDict(
     "RecurringChargeTypeDef",
     {
         "Amount": float,
         "Frequency": Literal["Hourly"],
     },
-    total=False,
 )
 
 ReferencedSecurityGroupTypeDef = TypedDict(
     "ReferencedSecurityGroupTypeDef",
     {
         "GroupId": str,
         "PeeringStatus": str,
         "UserId": str,
         "VpcId": str,
         "VpcPeeringConnectionId": str,
     },
-    total=False,
 )
 
 RegisterImageResultTypeDef = TypedDict(
     "RegisterImageResultTypeDef",
     {
         "ImageId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
@@ -13281,15 +13046,14 @@
 TransitGatewayMulticastRegisteredGroupMembersTypeDef = TypedDict(
     "TransitGatewayMulticastRegisteredGroupMembersTypeDef",
     {
         "TransitGatewayMulticastDomainId": str,
         "RegisteredNetworkInterfaceIds": List[str],
         "GroupIpAddress": str,
     },
-    total=False,
 )
 
 _RequiredRegisterTransitGatewayMulticastGroupSourcesRequestRequestTypeDef = TypedDict(
     "_RequiredRegisterTransitGatewayMulticastGroupSourcesRequestRequestTypeDef",
     {
         "TransitGatewayMulticastDomainId": str,
         "NetworkInterfaceIds": Sequence[str],
@@ -13313,15 +13077,14 @@
 TransitGatewayMulticastRegisteredGroupSourcesTypeDef = TypedDict(
     "TransitGatewayMulticastRegisteredGroupSourcesTypeDef",
     {
         "TransitGatewayMulticastDomainId": str,
         "RegisteredNetworkInterfaceIds": List[str],
         "GroupIpAddress": str,
     },
-    total=False,
 )
 
 RejectTransitGatewayMulticastDomainAssociationsRequestRequestTypeDef = TypedDict(
     "RejectTransitGatewayMulticastDomainAssociationsRequestRequestTypeDef",
     {
         "TransitGatewayMulticastDomainId": str,
         "TransitGatewayAttachmentId": str,
@@ -13754,15 +13517,14 @@
 )
 
 ReservedInstancesIdTypeDef = TypedDict(
     "ReservedInstancesIdTypeDef",
     {
         "ReservedInstancesId": str,
     },
-    total=False,
 )
 
 _RequiredResetAddressAttributeRequestRequestTypeDef = TypedDict(
     "_RequiredResetAddressAttributeRequestRequestTypeDef",
     {
         "AllocationId": str,
         "Attribute": Literal["domain-name"],
@@ -14215,15 +13977,14 @@
         "CarrierGatewayId": str,
         "NetworkInterfaceId": str,
         "Origin": RouteOriginType,
         "State": RouteStateType,
         "VpcPeeringConnectionId": str,
         "CoreNetworkArn": str,
     },
-    total=False,
 )
 
 RunScheduledInstancesResultTypeDef = TypedDict(
     "RunScheduledInstancesResultTypeDef",
     {
         "InstanceIdSet": List[str],
         "ResponseMetadata": "ResponseMetadataTypeDef",
@@ -14247,15 +14008,14 @@
     {
         "Frequency": str,
         "Interval": int,
         "OccurrenceDaySet": List[int],
         "OccurrenceRelativeToEnd": bool,
         "OccurrenceUnit": str,
     },
-    total=False,
 )
 
 ScheduledInstancesEbsTypeDef = TypedDict(
     "ScheduledInstancesEbsTypeDef",
     {
         "DeleteOnTermination": bool,
         "Encrypted": bool,
@@ -14321,24 +14081,22 @@
         "ResourceOwnerId": str,
         "NetworkInterfaceId": str,
         "GroupMember": bool,
         "GroupSource": bool,
         "MemberType": MembershipTypeType,
         "SourceType": MembershipTypeType,
     },
-    total=False,
 )
 
 SecurityGroupIdentifierTypeDef = TypedDict(
     "SecurityGroupIdentifierTypeDef",
     {
         "GroupId": str,
         "GroupName": str,
     },
-    total=False,
 )
 
 SecurityGroupRuleDescriptionTypeDef = TypedDict(
     "SecurityGroupRuleDescriptionTypeDef",
     {
         "SecurityGroupRuleId": str,
         "Description": str,
@@ -14382,60 +14140,54 @@
     pass
 
 ServiceTypeDetailTypeDef = TypedDict(
     "ServiceTypeDetailTypeDef",
     {
         "ServiceType": ServiceTypeType,
     },
-    total=False,
 )
 
 UserBucketDetailsTypeDef = TypedDict(
     "UserBucketDetailsTypeDef",
     {
         "S3Bucket": str,
         "S3Key": str,
     },
-    total=False,
 )
 
 SpotCapacityRebalanceTypeDef = TypedDict(
     "SpotCapacityRebalanceTypeDef",
     {
         "ReplacementStrategy": ReplacementStrategyType,
         "TerminationDelay": int,
     },
-    total=False,
 )
 
 SpotInstanceStateFaultTypeDef = TypedDict(
     "SpotInstanceStateFaultTypeDef",
     {
         "Code": str,
         "Message": str,
     },
-    total=False,
 )
 
 SpotFleetMonitoringTypeDef = TypedDict(
     "SpotFleetMonitoringTypeDef",
     {
         "Enabled": bool,
     },
-    total=False,
 )
 
 SpotInstanceStatusTypeDef = TypedDict(
     "SpotInstanceStatusTypeDef",
     {
         "Code": str,
         "Message": str,
         "UpdateTime": datetime,
     },
-    total=False,
 )
 
 StartInstancesRequestInstanceStartTypeDef = TypedDict(
     "StartInstancesRequestInstanceStartTypeDef",
     {
         "AdditionalInfo": str,
         "DryRun": bool,
@@ -14533,41 +14285,37 @@
 
 SubnetAssociationTypeDef = TypedDict(
     "SubnetAssociationTypeDef",
     {
         "SubnetId": str,
         "State": TransitGatewayMulitcastDomainAssociationStateType,
     },
-    total=False,
 )
 
 SubnetCidrBlockStateTypeDef = TypedDict(
     "SubnetCidrBlockStateTypeDef",
     {
         "State": SubnetCidrBlockStateCodeType,
         "StatusMessage": str,
     },
-    total=False,
 )
 
 TargetConfigurationTypeDef = TypedDict(
     "TargetConfigurationTypeDef",
     {
         "InstanceCount": int,
         "OfferingId": str,
     },
-    total=False,
 )
 
 TargetGroupTypeDef = TypedDict(
     "TargetGroupTypeDef",
     {
         "Arn": str,
     },
-    total=False,
 )
 
 _RequiredTerminateClientVpnConnectionsRequestRequestTypeDef = TypedDict(
     "_RequiredTerminateClientVpnConnectionsRequestRequestTypeDef",
     {
         "ClientVpnEndpointId": str,
     },
@@ -14618,54 +14366,49 @@
 
 TrafficMirrorPortRangeTypeDef = TypedDict(
     "TrafficMirrorPortRangeTypeDef",
     {
         "FromPort": int,
         "ToPort": int,
     },
-    total=False,
 )
 
 TransitGatewayAttachmentAssociationTypeDef = TypedDict(
     "TransitGatewayAttachmentAssociationTypeDef",
     {
         "TransitGatewayRouteTableId": str,
         "State": TransitGatewayAssociationStateType,
     },
-    total=False,
 )
 
 TransitGatewayAttachmentBgpConfigurationTypeDef = TypedDict(
     "TransitGatewayAttachmentBgpConfigurationTypeDef",
     {
         "TransitGatewayAsn": int,
         "PeerAsn": int,
         "TransitGatewayAddress": str,
         "PeerAddress": str,
         "BgpStatus": BgpStatusType,
     },
-    total=False,
 )
 
 TransitGatewayConnectOptionsTypeDef = TypedDict(
     "TransitGatewayConnectOptionsTypeDef",
     {
         "Protocol": Literal["gre"],
     },
-    total=False,
 )
 
 TransitGatewayMulticastDomainOptionsTypeDef = TypedDict(
     "TransitGatewayMulticastDomainOptionsTypeDef",
     {
         "Igmpv2Support": Igmpv2SupportValueType,
         "StaticSourcesSupport": StaticSourcesSupportValueType,
         "AutoAcceptSharedAssociations": AutoAcceptSharedAssociationsValueType,
     },
-    total=False,
 )
 
 TransitGatewayOptionsTypeDef = TypedDict(
     "TransitGatewayOptionsTypeDef",
     {
         "AmazonSideAsn": int,
         "TransitGatewayCidrBlocks": List[str],
@@ -14674,62 +14417,56 @@
         "AssociationDefaultRouteTableId": str,
         "DefaultRouteTablePropagation": DefaultRouteTablePropagationValueType,
         "PropagationDefaultRouteTableId": str,
         "VpnEcmpSupport": VpnEcmpSupportValueType,
         "DnsSupport": DnsSupportValueType,
         "MulticastSupport": MulticastSupportValueType,
     },
-    total=False,
 )
 
 TransitGatewayPeeringAttachmentOptionsTypeDef = TypedDict(
     "TransitGatewayPeeringAttachmentOptionsTypeDef",
     {
         "DynamicRouting": DynamicRoutingValueType,
     },
-    total=False,
 )
 
 TransitGatewayPolicyRuleMetaDataTypeDef = TypedDict(
     "TransitGatewayPolicyRuleMetaDataTypeDef",
     {
         "MetaDataKey": str,
         "MetaDataValue": str,
     },
-    total=False,
 )
 
 TransitGatewayPrefixListAttachmentTypeDef = TypedDict(
     "TransitGatewayPrefixListAttachmentTypeDef",
     {
         "TransitGatewayAttachmentId": str,
         "ResourceType": TransitGatewayAttachmentResourceTypeType,
         "ResourceId": str,
     },
-    total=False,
 )
 
 TransitGatewayRouteAttachmentTypeDef = TypedDict(
     "TransitGatewayRouteAttachmentTypeDef",
     {
         "ResourceId": str,
         "TransitGatewayAttachmentId": str,
         "ResourceType": TransitGatewayAttachmentResourceTypeType,
     },
-    total=False,
 )
 
 TransitGatewayVpcAttachmentOptionsTypeDef = TypedDict(
     "TransitGatewayVpcAttachmentOptionsTypeDef",
     {
         "DnsSupport": DnsSupportValueType,
         "Ipv6Support": Ipv6SupportValueType,
         "ApplianceModeSupport": ApplianceModeSupportValueType,
     },
-    total=False,
 )
 
 _RequiredUnassignIpv6AddressesRequestRequestTypeDef = TypedDict(
     "_RequiredUnassignIpv6AddressesRequestRequestTypeDef",
     {
         "NetworkInterfaceId": str,
     },
@@ -14841,24 +14578,22 @@
 
 UnsuccessfulInstanceCreditSpecificationItemErrorTypeDef = TypedDict(
     "UnsuccessfulInstanceCreditSpecificationItemErrorTypeDef",
     {
         "Code": UnsuccessfulInstanceCreditSpecificationErrorCodeType,
         "Message": str,
     },
-    total=False,
 )
 
 UnsuccessfulItemErrorTypeDef = TypedDict(
     "UnsuccessfulItemErrorTypeDef",
     {
         "Code": str,
         "Message": str,
     },
-    total=False,
 )
 
 UpdateSecurityGroupRuleDescriptionsEgressResultTypeDef = TypedDict(
     "UpdateSecurityGroupRuleDescriptionsEgressResultTypeDef",
     {
         "Return": bool,
         "ResponseMetadata": "ResponseMetadataTypeDef",
@@ -14875,57 +14610,52 @@
 
 ValidationErrorTypeDef = TypedDict(
     "ValidationErrorTypeDef",
     {
         "Code": str,
         "Message": str,
     },
-    total=False,
 )
 
 VerifiedAccessEndpointEniOptionsTypeDef = TypedDict(
     "VerifiedAccessEndpointEniOptionsTypeDef",
     {
         "NetworkInterfaceId": str,
         "Protocol": VerifiedAccessEndpointProtocolType,
         "Port": int,
     },
-    total=False,
 )
 
 VerifiedAccessEndpointLoadBalancerOptionsTypeDef = TypedDict(
     "VerifiedAccessEndpointLoadBalancerOptionsTypeDef",
     {
         "Protocol": VerifiedAccessEndpointProtocolType,
         "Port": int,
         "LoadBalancerArn": str,
         "SubnetIds": List[str],
     },
-    total=False,
 )
 
 VerifiedAccessEndpointStatusTypeDef = TypedDict(
     "VerifiedAccessEndpointStatusTypeDef",
     {
         "Code": VerifiedAccessEndpointStatusCodeType,
         "Message": str,
     },
-    total=False,
 )
 
 VerifiedAccessTrustProviderCondensedTypeDef = TypedDict(
     "VerifiedAccessTrustProviderCondensedTypeDef",
     {
         "VerifiedAccessTrustProviderId": str,
         "Description": str,
         "TrustProviderType": TrustProviderTypeType,
         "UserTrustProviderType": UserTrustProviderTypeType,
         "DeviceTrustProviderType": DeviceTrustProviderTypeType,
     },
-    total=False,
 )
 
 _RequiredVerifiedAccessLogCloudWatchLogsDestinationOptionsTypeDef = TypedDict(
     "_RequiredVerifiedAccessLogCloudWatchLogsDestinationOptionsTypeDef",
     {
         "Enabled": bool,
     },
@@ -14946,15 +14676,14 @@
 
 VerifiedAccessLogDeliveryStatusTypeDef = TypedDict(
     "VerifiedAccessLogDeliveryStatusTypeDef",
     {
         "Code": VerifiedAccessLogDeliveryStatusCodeType,
         "Message": str,
     },
-    total=False,
 )
 
 _RequiredVerifiedAccessLogKinesisDataFirehoseDestinationOptionsTypeDef = TypedDict(
     "_RequiredVerifiedAccessLogKinesisDataFirehoseDestinationOptionsTypeDef",
     {
         "Enabled": bool,
     },
@@ -15001,15 +14730,14 @@
         "AcceptedRouteCount": int,
         "LastStatusChange": datetime,
         "OutsideIpAddress": str,
         "Status": TelemetryStatusType,
         "StatusMessage": str,
         "CertificateArn": str,
     },
-    total=False,
 )
 
 VolumeAttachmentResponseMetadataTypeDef = TypedDict(
     "VolumeAttachmentResponseMetadataTypeDef",
     {
         "AttachTime": datetime,
         "Device": str,
@@ -15027,76 +14755,69 @@
         "AttachTime": datetime,
         "Device": str,
         "InstanceId": str,
         "State": VolumeAttachmentStateType,
         "VolumeId": str,
         "DeleteOnTermination": bool,
     },
-    total=False,
 )
 
 VolumeStatusActionTypeDef = TypedDict(
     "VolumeStatusActionTypeDef",
     {
         "Code": str,
         "Description": str,
         "EventId": str,
         "EventType": str,
     },
-    total=False,
 )
 
 VolumeStatusAttachmentStatusTypeDef = TypedDict(
     "VolumeStatusAttachmentStatusTypeDef",
     {
         "IoPerformance": str,
         "InstanceId": str,
     },
-    total=False,
 )
 
 VolumeStatusDetailsTypeDef = TypedDict(
     "VolumeStatusDetailsTypeDef",
     {
         "Name": VolumeStatusNameType,
         "Status": str,
     },
-    total=False,
 )
 
 VolumeStatusEventTypeDef = TypedDict(
     "VolumeStatusEventTypeDef",
     {
         "Description": str,
         "EventId": str,
         "EventType": str,
         "NotAfter": datetime,
         "NotBefore": datetime,
         "InstanceId": str,
     },
-    total=False,
 )
 
 VpcCidrBlockStateTypeDef = TypedDict(
     "VpcCidrBlockStateTypeDef",
     {
         "State": VpcCidrBlockStateCodeType,
         "StatusMessage": str,
     },
-    total=False,
 )
 
 VpcPeeringConnectionOptionsDescriptionTypeDef = TypedDict(
     "VpcPeeringConnectionOptionsDescriptionTypeDef",
     {
         "AllowDnsResolutionFromRemoteVpc": bool,
         "AllowEgressFromLocalClassicLinkToRemoteVpc": bool,
         "AllowEgressFromLocalVpcToRemoteClassicLink": bool,
     },
-    total=False,
 )
 
 VpcPeeringConnectionStateReasonResponseMetadataTypeDef = TypedDict(
     "VpcPeeringConnectionStateReasonResponseMetadataTypeDef",
     {
         "Code": VpcPeeringConnectionStateReasonCodeType,
         "Message": str,
@@ -15106,25 +14827,23 @@
 
 VpcPeeringConnectionStateReasonTypeDef = TypedDict(
     "VpcPeeringConnectionStateReasonTypeDef",
     {
         "Code": VpcPeeringConnectionStateReasonCodeType,
         "Message": str,
     },
-    total=False,
 )
 
 VpnStaticRouteTypeDef = TypedDict(
     "VpnStaticRouteTypeDef",
     {
         "DestinationCidrBlock": str,
         "Source": Literal["Static"],
         "State": VpnStateType,
     },
-    total=False,
 )
 
 _RequiredWithdrawByoipCidrRequestRequestTypeDef = TypedDict(
     "_RequiredWithdrawByoipCidrRequestRequestTypeDef",
     {
         "Cidr": str,
     },
@@ -15219,15 +14938,14 @@
 
 AccountAttributeTypeDef = TypedDict(
     "AccountAttributeTypeDef",
     {
         "AttributeName": str,
         "AttributeValues": List[AccountAttributeValueTypeDef],
     },
-    total=False,
 )
 
 DescribeFleetInstancesResultTypeDef = TypedDict(
     "DescribeFleetInstancesResultTypeDef",
     {
         "ActiveInstances": List[ActiveInstanceTypeDef],
         "NextToken": str,
@@ -15259,35 +14977,32 @@
     "AnalysisLoadBalancerTargetTypeDef",
     {
         "Address": str,
         "AvailabilityZone": str,
         "Instance": AnalysisComponentTypeDef,
         "Port": int,
     },
-    total=False,
 )
 
 RuleGroupRuleOptionsPairTypeDef = TypedDict(
     "RuleGroupRuleOptionsPairTypeDef",
     {
         "RuleGroupArn": str,
         "RuleOptions": List[RuleOptionTypeDef],
     },
-    total=False,
 )
 
 AddressAttributeTypeDef = TypedDict(
     "AddressAttributeTypeDef",
     {
         "PublicIp": str,
         "AllocationId": str,
         "PtrRecord": str,
         "PtrRecordUpdate": PtrUpdateStatusTypeDef,
     },
-    total=False,
 )
 
 AddressTypeDef = TypedDict(
     "AddressTypeDef",
     {
         "InstanceId": str,
         "PublicIp": str,
@@ -15300,39 +15015,36 @@
         "Tags": List[TagTypeDef],
         "PublicIpv4Pool": str,
         "NetworkBorderGroup": str,
         "CustomerOwnedIp": str,
         "CustomerOwnedIpv4Pool": str,
         "CarrierIp": str,
     },
-    total=False,
 )
 
 AllowedPrincipalTypeDef = TypedDict(
     "AllowedPrincipalTypeDef",
     {
         "PrincipalType": PrincipalTypeType,
         "Principal": str,
         "ServicePermissionId": str,
         "Tags": List[TagTypeDef],
         "ServiceId": str,
     },
-    total=False,
 )
 
 CarrierGatewayTypeDef = TypedDict(
     "CarrierGatewayTypeDef",
     {
         "CarrierGatewayId": str,
         "VpcId": str,
         "State": CarrierGatewayStateType,
         "OwnerId": str,
         "Tags": List[TagTypeDef],
     },
-    total=False,
 )
 
 _RequiredClientCreateTagsRequestTypeDef = TypedDict(
     "_RequiredClientCreateTagsRequestTypeDef",
     {
         "Resources": Sequence[str],
         "Tags": Sequence[TagTypeDef],
@@ -15376,15 +15088,14 @@
     {
         "PoolId": str,
         "PoolCidrs": List[str],
         "LocalGatewayRouteTableId": str,
         "Tags": List[TagTypeDef],
         "PoolArn": str,
     },
-    total=False,
 )
 
 CopySnapshotResultTypeDef = TypedDict(
     "CopySnapshotResultTypeDef",
     {
         "SnapshotId": str,
         "Tags": List[TagTypeDef],
@@ -15430,15 +15141,14 @@
         "IpAddress": str,
         "CertificateArn": str,
         "State": str,
         "Type": str,
         "DeviceName": str,
         "Tags": List[TagTypeDef],
     },
-    total=False,
 )
 
 Ec2InstanceConnectEndpointTypeDef = TypedDict(
     "Ec2InstanceConnectEndpointTypeDef",
     {
         "OwnerId": str,
         "InstanceConnectEndpointId": str,
@@ -15452,15 +15162,14 @@
         "AvailabilityZone": str,
         "CreatedAt": datetime,
         "SubnetId": str,
         "PreserveClientIp": bool,
         "SecurityGroupIds": List[str],
         "Tags": List[TagTypeDef],
     },
-    total=False,
 )
 
 HostReservationTypeDef = TypedDict(
     "HostReservationTypeDef",
     {
         "Count": int,
         "CurrencyCode": Literal["USD"],
@@ -15473,15 +15182,14 @@
         "OfferingId": str,
         "PaymentOption": PaymentOptionType,
         "Start": datetime,
         "State": ReservationStateType,
         "UpfrontPrice": str,
         "Tags": List[TagTypeDef],
     },
-    total=False,
 )
 
 ImportKeyPairResultTypeDef = TypedDict(
     "ImportKeyPairResultTypeDef",
     {
         "KeyFingerprint": str,
         "KeyName": str,
@@ -15532,15 +15240,14 @@
 InstanceEventWindowAssociationTargetTypeDef = TypedDict(
     "InstanceEventWindowAssociationTargetTypeDef",
     {
         "InstanceIds": List[str],
         "Tags": List[TagTypeDef],
         "DedicatedHostIds": List[str],
     },
-    total=False,
 )
 
 InstanceEventWindowDisassociationRequestTypeDef = TypedDict(
     "InstanceEventWindowDisassociationRequestTypeDef",
     {
         "InstanceIds": Sequence[str],
         "InstanceTags": Sequence[TagTypeDef],
@@ -15560,15 +15267,14 @@
         "IpamArn": str,
         "IpamRegion": str,
         "IsDefault": bool,
         "ResourceDiscoveryStatus": IpamAssociatedResourceDiscoveryStatusType,
         "State": IpamResourceDiscoveryAssociationStateType,
         "Tags": List[TagTypeDef],
     },
-    total=False,
 )
 
 IpamScopeTypeDef = TypedDict(
     "IpamScopeTypeDef",
     {
         "OwnerId": str,
         "IpamScopeId": str,
@@ -15578,29 +15284,27 @@
         "IpamScopeType": IpamScopeTypeType,
         "IsDefault": bool,
         "Description": str,
         "PoolCount": int,
         "State": IpamScopeStateType,
         "Tags": List[TagTypeDef],
     },
-    total=False,
 )
 
 KeyPairInfoTypeDef = TypedDict(
     "KeyPairInfoTypeDef",
     {
         "KeyPairId": str,
         "KeyFingerprint": str,
         "KeyName": str,
         "KeyType": KeyTypeType,
         "Tags": List[TagTypeDef],
         "PublicKey": str,
         "CreateTime": datetime,
     },
-    total=False,
 )
 
 KeyPairTypeDef = TypedDict(
     "KeyPairTypeDef",
     {
         "KeyFingerprint": str,
         "KeyMaterial": str,
@@ -15622,83 +15326,77 @@
 
 LaunchTemplateTagSpecificationTypeDef = TypedDict(
     "LaunchTemplateTagSpecificationTypeDef",
     {
         "ResourceType": ResourceTypeType,
         "Tags": List[TagTypeDef],
     },
-    total=False,
 )
 
 LaunchTemplateTypeDef = TypedDict(
     "LaunchTemplateTypeDef",
     {
         "LaunchTemplateId": str,
         "LaunchTemplateName": str,
         "CreateTime": datetime,
         "CreatedBy": str,
         "DefaultVersionNumber": int,
         "LatestVersionNumber": int,
         "Tags": List[TagTypeDef],
     },
-    total=False,
 )
 
 LocalGatewayRouteTableVirtualInterfaceGroupAssociationTypeDef = TypedDict(
     "LocalGatewayRouteTableVirtualInterfaceGroupAssociationTypeDef",
     {
         "LocalGatewayRouteTableVirtualInterfaceGroupAssociationId": str,
         "LocalGatewayVirtualInterfaceGroupId": str,
         "LocalGatewayId": str,
         "LocalGatewayRouteTableId": str,
         "LocalGatewayRouteTableArn": str,
         "OwnerId": str,
         "State": str,
         "Tags": List[TagTypeDef],
     },
-    total=False,
 )
 
 LocalGatewayRouteTableVpcAssociationTypeDef = TypedDict(
     "LocalGatewayRouteTableVpcAssociationTypeDef",
     {
         "LocalGatewayRouteTableVpcAssociationId": str,
         "LocalGatewayRouteTableId": str,
         "LocalGatewayRouteTableArn": str,
         "LocalGatewayId": str,
         "VpcId": str,
         "OwnerId": str,
         "State": str,
         "Tags": List[TagTypeDef],
     },
-    total=False,
 )
 
 LocalGatewayTypeDef = TypedDict(
     "LocalGatewayTypeDef",
     {
         "LocalGatewayId": str,
         "OutpostArn": str,
         "OwnerId": str,
         "State": str,
         "Tags": List[TagTypeDef],
     },
-    total=False,
 )
 
 LocalGatewayVirtualInterfaceGroupTypeDef = TypedDict(
     "LocalGatewayVirtualInterfaceGroupTypeDef",
     {
         "LocalGatewayVirtualInterfaceGroupId": str,
         "LocalGatewayVirtualInterfaceIds": List[str],
         "LocalGatewayId": str,
         "OwnerId": str,
         "Tags": List[TagTypeDef],
     },
-    total=False,
 )
 
 LocalGatewayVirtualInterfaceTypeDef = TypedDict(
     "LocalGatewayVirtualInterfaceTypeDef",
     {
         "LocalGatewayVirtualInterfaceId": str,
         "LocalGatewayId": str,
@@ -15706,15 +15404,14 @@
         "LocalAddress": str,
         "PeerAddress": str,
         "LocalBgpAsn": int,
         "PeerBgpAsn": int,
         "OwnerId": str,
         "Tags": List[TagTypeDef],
     },
-    total=False,
 )
 
 ManagedPrefixListTypeDef = TypedDict(
     "ManagedPrefixListTypeDef",
     {
         "PrefixListId": str,
         "AddressFamily": str,
@@ -15723,15 +15420,14 @@
         "PrefixListArn": str,
         "PrefixListName": str,
         "MaxEntries": int,
         "Version": int,
         "Tags": List[TagTypeDef],
         "OwnerId": str,
     },
-    total=False,
 )
 
 NetworkInsightsAccessScopeAnalysisTypeDef = TypedDict(
     "NetworkInsightsAccessScopeAnalysisTypeDef",
     {
         "NetworkInsightsAccessScopeAnalysisId": str,
         "NetworkInsightsAccessScopeAnalysisArn": str,
@@ -15741,42 +15437,39 @@
         "WarningMessage": str,
         "StartDate": datetime,
         "EndDate": datetime,
         "FindingsFound": FindingsFoundType,
         "AnalyzedEniCount": int,
         "Tags": List[TagTypeDef],
     },
-    total=False,
 )
 
 NetworkInsightsAccessScopeTypeDef = TypedDict(
     "NetworkInsightsAccessScopeTypeDef",
     {
         "NetworkInsightsAccessScopeId": str,
         "NetworkInsightsAccessScopeArn": str,
         "CreatedDate": datetime,
         "UpdatedDate": datetime,
         "Tags": List[TagTypeDef],
     },
-    total=False,
 )
 
 PlacementGroupTypeDef = TypedDict(
     "PlacementGroupTypeDef",
     {
         "GroupName": str,
         "State": PlacementGroupStateType,
         "Strategy": PlacementStrategyType,
         "PartitionCount": int,
         "GroupId": str,
         "Tags": List[TagTypeDef],
         "GroupArn": str,
         "SpreadLevel": SpreadLevelType,
     },
-    total=False,
 )
 
 ReplaceRootVolumeTaskTypeDef = TypedDict(
     "ReplaceRootVolumeTaskTypeDef",
     {
         "ReplaceRootVolumeTaskId": str,
         "InstanceId": str,
@@ -15784,15 +15477,14 @@
         "StartTime": str,
         "CompleteTime": str,
         "Tags": List[TagTypeDef],
         "ImageId": str,
         "SnapshotId": str,
         "DeleteReplacedRootVolume": bool,
     },
-    total=False,
 )
 
 SnapshotInfoTypeDef = TypedDict(
     "SnapshotInfoTypeDef",
     {
         "Description": str,
         "Tags": List[TagTypeDef],
@@ -15802,15 +15494,14 @@
         "VolumeSize": int,
         "StartTime": datetime,
         "Progress": str,
         "OwnerId": str,
         "SnapshotId": str,
         "OutpostArn": str,
     },
-    total=False,
 )
 
 SnapshotResponseMetadataTypeDef = TypedDict(
     "SnapshotResponseMetadataTypeDef",
     {
         "DataEncryptionKeyId": str,
         "Description": str,
@@ -15845,15 +15536,14 @@
         "LastTieringStartTime": datetime,
         "LastTieringProgress": int,
         "LastTieringOperationStatus": TieringOperationStatusType,
         "LastTieringOperationStatusDetail": str,
         "ArchivalCompleteTime": datetime,
         "RestoreExpiryTime": datetime,
     },
-    total=False,
 )
 
 SnapshotTypeDef = TypedDict(
     "SnapshotTypeDef",
     {
         "DataEncryptionKeyId": str,
         "Description": str,
@@ -15869,38 +15559,35 @@
         "VolumeSize": int,
         "OwnerAlias": str,
         "OutpostArn": str,
         "Tags": List[TagTypeDef],
         "StorageTier": StorageTierType,
         "RestoreExpiryTime": datetime,
     },
-    total=False,
 )
 
 SpotFleetTagSpecificationTypeDef = TypedDict(
     "SpotFleetTagSpecificationTypeDef",
     {
         "ResourceType": ResourceTypeType,
         "Tags": List[TagTypeDef],
     },
-    total=False,
 )
 
 SubnetCidrReservationTypeDef = TypedDict(
     "SubnetCidrReservationTypeDef",
     {
         "SubnetCidrReservationId": str,
         "SubnetId": str,
         "Cidr": str,
         "ReservationType": SubnetCidrReservationTypeType,
         "OwnerId": str,
         "Description": str,
         "Tags": List[TagTypeDef],
     },
-    total=False,
 )
 
 TagSpecificationTypeDef = TypedDict(
     "TagSpecificationTypeDef",
     {
         "ResourceType": ResourceTypeType,
         "Tags": Sequence[TagTypeDef],
@@ -15918,42 +15605,39 @@
         "OwnerId": str,
         "PacketLength": int,
         "SessionNumber": int,
         "VirtualNetworkId": int,
         "Description": str,
         "Tags": List[TagTypeDef],
     },
-    total=False,
 )
 
 TrafficMirrorTargetTypeDef = TypedDict(
     "TrafficMirrorTargetTypeDef",
     {
         "TrafficMirrorTargetId": str,
         "NetworkInterfaceId": str,
         "NetworkLoadBalancerArn": str,
         "Type": TrafficMirrorTargetTypeType,
         "Description": str,
         "OwnerId": str,
         "Tags": List[TagTypeDef],
         "GatewayLoadBalancerEndpointId": str,
     },
-    total=False,
 )
 
 TransitGatewayPolicyTableTypeDef = TypedDict(
     "TransitGatewayPolicyTableTypeDef",
     {
         "TransitGatewayPolicyTableId": str,
         "TransitGatewayId": str,
         "State": TransitGatewayPolicyTableStateType,
         "CreationTime": datetime,
         "Tags": List[TagTypeDef],
     },
-    total=False,
 )
 
 TransitGatewayRouteTableAnnouncementTypeDef = TypedDict(
     "TransitGatewayRouteTableAnnouncementTypeDef",
     {
         "TransitGatewayRouteTableAnnouncementId": str,
         "TransitGatewayId": str,
@@ -15963,43 +15647,40 @@
         "PeeringAttachmentId": str,
         "AnnouncementDirection": TransitGatewayRouteTableAnnouncementDirectionType,
         "TransitGatewayRouteTableId": str,
         "State": TransitGatewayRouteTableAnnouncementStateType,
         "CreationTime": datetime,
         "Tags": List[TagTypeDef],
     },
-    total=False,
 )
 
 TransitGatewayRouteTableTypeDef = TypedDict(
     "TransitGatewayRouteTableTypeDef",
     {
         "TransitGatewayRouteTableId": str,
         "TransitGatewayId": str,
         "State": TransitGatewayRouteTableStateType,
         "DefaultAssociationRouteTable": bool,
         "DefaultPropagationRouteTable": bool,
         "CreationTime": datetime,
         "Tags": List[TagTypeDef],
     },
-    total=False,
 )
 
 TrunkInterfaceAssociationTypeDef = TypedDict(
     "TrunkInterfaceAssociationTypeDef",
     {
         "AssociationId": str,
         "BranchInterfaceId": str,
         "TrunkInterfaceId": str,
         "InterfaceProtocol": InterfaceProtocolTypeType,
         "VlanId": int,
         "GreKey": int,
         "Tags": List[TagTypeDef],
     },
-    total=False,
 )
 
 VerifiedAccessGroupTypeDef = TypedDict(
     "VerifiedAccessGroupTypeDef",
     {
         "VerifiedAccessGroupId": str,
         "VerifiedAccessInstanceId": str,
@@ -16007,25 +15688,23 @@
         "Owner": str,
         "VerifiedAccessGroupArn": str,
         "CreationTime": str,
         "LastUpdatedTime": str,
         "DeletionTime": str,
         "Tags": List[TagTypeDef],
     },
-    total=False,
 )
 
 VpcClassicLinkTypeDef = TypedDict(
     "VpcClassicLinkTypeDef",
     {
         "ClassicLinkEnabled": bool,
         "Tags": List[TagTypeDef],
         "VpcId": str,
     },
-    total=False,
 )
 
 _RequiredVpcCreateTagsRequestTypeDef = TypedDict(
     "_RequiredVpcCreateTagsRequestTypeDef",
     {
         "Tags": Sequence[TagTypeDef],
     },
@@ -16115,70 +15794,65 @@
         "Cidr": str,
         "Egress": bool,
         "PortRange": PortRangeTypeDef,
         "Protocol": str,
         "RuleAction": str,
         "RuleNumber": int,
     },
-    total=False,
 )
 
 AnalysisPacketHeaderTypeDef = TypedDict(
     "AnalysisPacketHeaderTypeDef",
     {
         "DestinationAddresses": List[str],
         "DestinationPortRanges": List[PortRangeTypeDef],
         "Protocol": str,
         "SourceAddresses": List[str],
         "SourcePortRanges": List[PortRangeTypeDef],
     },
-    total=False,
 )
 
 AnalysisSecurityGroupRuleTypeDef = TypedDict(
     "AnalysisSecurityGroupRuleTypeDef",
     {
         "Cidr": str,
         "Direction": str,
         "SecurityGroupId": str,
         "PortRange": PortRangeTypeDef,
         "PrefixListId": str,
         "Protocol": str,
     },
-    total=False,
 )
 
 FirewallStatefulRuleTypeDef = TypedDict(
     "FirewallStatefulRuleTypeDef",
     {
         "RuleGroupArn": str,
         "Sources": List[str],
         "Destinations": List[str],
         "SourcePorts": List[PortRangeTypeDef],
         "DestinationPorts": List[PortRangeTypeDef],
         "Protocol": str,
         "RuleAction": str,
         "Direction": str,
     },
-    total=False,
 )
 
 FirewallStatelessRuleTypeDef = TypedDict(
     "FirewallStatelessRuleTypeDef",
     {
         "RuleGroupArn": str,
         "Sources": List[str],
         "Destinations": List[str],
         "SourcePorts": List[PortRangeTypeDef],
         "DestinationPorts": List[PortRangeTypeDef],
         "Protocols": List[int],
         "RuleAction": str,
         "Priority": int,
     },
-    total=False,
 )
 
 AssignPrivateIpAddressesResultTypeDef = TypedDict(
     "AssignPrivateIpAddressesResultTypeDef",
     {
         "NetworkInterfaceId": str,
         "AssignedPrivateIpAddresses": List[AssignedPrivateIpAddressTypeDef],
@@ -16247,15 +15921,14 @@
         "AssociationId": str,
         "VpcId": str,
         "TargetNetworkId": str,
         "ClientVpnEndpointId": str,
         "Status": AssociationStatusTypeDef,
         "SecurityGroups": List[str],
     },
-    total=False,
 )
 
 AssociateIamInstanceProfileRequestRequestTypeDef = TypedDict(
     "AssociateIamInstanceProfileRequestRequestTypeDef",
     {
         "IamInstanceProfile": IamInstanceProfileSpecificationTypeDef,
         "InstanceId": str,
@@ -16294,15 +15967,14 @@
         "Main": bool,
         "RouteTableAssociationId": str,
         "RouteTableId": str,
         "SubnetId": str,
         "GatewayId": str,
         "AssociationState": RouteTableAssociationStateTypeDef,
     },
-    total=False,
 )
 
 AssociateTransitGatewayPolicyTableResultTypeDef = TypedDict(
     "AssociateTransitGatewayPolicyTableResultTypeDef",
     {
         "Association": TransitGatewayPolicyTableAssociationTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
@@ -16373,24 +16045,22 @@
         "State": VpnStateType,
         "Type": Literal["ipsec.1"],
         "VpcAttachments": List[VpcAttachmentTypeDef],
         "VpnGatewayId": str,
         "AmazonSideAsn": int,
         "Tags": List[TagTypeDef],
     },
-    total=False,
 )
 
 AttachmentEnaSrdSpecificationTypeDef = TypedDict(
     "AttachmentEnaSrdSpecificationTypeDef",
     {
         "EnaSrdEnabled": bool,
         "EnaSrdUdpSpecification": AttachmentEnaSrdUdpSpecificationTypeDef,
     },
-    total=False,
 )
 
 DescribeVpcAttributeResultTypeDef = TypedDict(
     "DescribeVpcAttributeResultTypeDef",
     {
         "VpcId": str,
         "EnableDnsHostnames": AttributeBooleanValueTypeDef,
@@ -16493,28 +16163,26 @@
 
 DhcpConfigurationTypeDef = TypedDict(
     "DhcpConfigurationTypeDef",
     {
         "Key": str,
         "Values": List[AttributeValueTypeDef],
     },
-    total=False,
 )
 
 AuthorizationRuleTypeDef = TypedDict(
     "AuthorizationRuleTypeDef",
     {
         "ClientVpnEndpointId": str,
         "Description": str,
         "GroupId": str,
         "AccessAll": bool,
         "DestinationCidr": str,
         "Status": ClientVpnAuthorizationRuleStatusTypeDef,
     },
-    total=False,
 )
 
 AuthorizeClientVpnIngressResultTypeDef = TypedDict(
     "AuthorizeClientVpnIngressResultTypeDef",
     {
         "Status": ClientVpnAuthorizationRuleStatusTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
@@ -16540,24 +16208,22 @@
         "ZoneId": str,
         "GroupName": str,
         "NetworkBorderGroup": str,
         "ZoneType": str,
         "ParentZoneName": str,
         "ParentZoneId": str,
     },
-    total=False,
 )
 
 AvailableCapacityTypeDef = TypedDict(
     "AvailableCapacityTypeDef",
     {
         "AvailableInstanceCapacity": List[InstanceCapacityTypeDef],
         "AvailableVCpus": int,
     },
-    total=False,
 )
 
 BlockDeviceMappingTypeDef = TypedDict(
     "BlockDeviceMappingTypeDef",
     {
         "DeviceName": str,
         "VirtualName": str,
@@ -16569,24 +16235,22 @@
 
 FailedCapacityReservationFleetCancellationResultTypeDef = TypedDict(
     "FailedCapacityReservationFleetCancellationResultTypeDef",
     {
         "CapacityReservationFleetId": str,
         "CancelCapacityReservationFleetError": CancelCapacityReservationFleetErrorTypeDef,
     },
-    total=False,
 )
 
 CancelSpotFleetRequestsErrorItemTypeDef = TypedDict(
     "CancelSpotFleetRequestsErrorItemTypeDef",
     {
         "Error": CancelSpotFleetRequestsErrorTypeDef,
         "SpotFleetRequestId": str,
     },
-    total=False,
 )
 
 CancelSpotInstanceRequestsResultTypeDef = TypedDict(
     "CancelSpotInstanceRequestsResultTypeDef",
     {
         "CancelledSpotInstanceRequests": List[CancelledSpotInstanceRequestTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
@@ -16616,15 +16280,14 @@
         "CreateDate": datetime,
         "Tags": List[TagTypeDef],
         "OutpostArn": str,
         "CapacityReservationFleetId": str,
         "PlacementGroupArn": str,
         "CapacityAllocations": List[CapacityAllocationTypeDef],
     },
-    total=False,
 )
 
 CapacityReservationFleetTypeDef = TypedDict(
     "CapacityReservationFleetTypeDef",
     {
         "CapacityReservationFleetId": str,
         "CapacityReservationFleetArn": str,
@@ -16635,15 +16298,14 @@
         "EndDate": datetime,
         "CreateTime": datetime,
         "InstanceMatchCriteria": Literal["open"],
         "AllocationStrategy": str,
         "InstanceTypeSpecifications": List[FleetCapacityReservationTypeDef],
         "Tags": List[TagTypeDef],
     },
-    total=False,
 )
 
 CreateCapacityReservationFleetResultTypeDef = TypedDict(
     "CreateCapacityReservationFleetResultTypeDef",
     {
         "CapacityReservationFleetId": str,
         "State": CapacityReservationFleetStateType,
@@ -16688,15 +16350,14 @@
         "AllocationStrategy": FleetOnDemandAllocationStrategyType,
         "CapacityReservationOptions": CapacityReservationOptionsTypeDef,
         "SingleInstanceType": bool,
         "SingleAvailabilityZone": bool,
         "MinTargetCapacity": int,
         "MaxTotalPrice": str,
     },
-    total=False,
 )
 
 CapacityReservationSpecificationResponseResponseMetadataTypeDef = TypedDict(
     "CapacityReservationSpecificationResponseResponseMetadataTypeDef",
     {
         "CapacityReservationPreference": CapacityReservationPreferenceType,
         "CapacityReservationTarget": CapacityReservationTargetResponseTypeDef,
@@ -16706,24 +16367,22 @@
 
 CapacityReservationSpecificationResponseTypeDef = TypedDict(
     "CapacityReservationSpecificationResponseTypeDef",
     {
         "CapacityReservationPreference": CapacityReservationPreferenceType,
         "CapacityReservationTarget": CapacityReservationTargetResponseTypeDef,
     },
-    total=False,
 )
 
 LaunchTemplateCapacityReservationSpecificationResponseTypeDef = TypedDict(
     "LaunchTemplateCapacityReservationSpecificationResponseTypeDef",
     {
         "CapacityReservationPreference": CapacityReservationPreferenceType,
         "CapacityReservationTarget": CapacityReservationTargetResponseTypeDef,
     },
-    total=False,
 )
 
 CapacityReservationSpecificationTypeDef = TypedDict(
     "CapacityReservationSpecificationTypeDef",
     {
         "CapacityReservationPreference": CapacityReservationPreferenceType,
         "CapacityReservationTarget": CapacityReservationTargetTypeDef,
@@ -16753,23 +16412,21 @@
     "ClassicLinkInstanceTypeDef",
     {
         "Groups": List[GroupIdentifierTypeDef],
         "InstanceId": str,
         "Tags": List[TagTypeDef],
         "VpcId": str,
     },
-    total=False,
 )
 
 ClassicLoadBalancersConfigTypeDef = TypedDict(
     "ClassicLoadBalancersConfigTypeDef",
     {
         "ClassicLoadBalancers": List[ClassicLoadBalancerTypeDef],
     },
-    total=False,
 )
 
 ExportClientVpnClientCertificateRevocationListResultTypeDef = TypedDict(
     "ExportClientVpnClientCertificateRevocationListResultTypeDef",
     {
         "CertificateRevocationList": str,
         "Status": ClientCertificateRevocationListStatusTypeDef,
@@ -16780,15 +16437,14 @@
 ClientConnectResponseOptionsTypeDef = TypedDict(
     "ClientConnectResponseOptionsTypeDef",
     {
         "Enabled": bool,
         "LambdaFunctionArn": str,
         "Status": ClientVpnEndpointAttributeStatusTypeDef,
     },
-    total=False,
 )
 
 ClientVpnAuthenticationRequestTypeDef = TypedDict(
     "ClientVpnAuthenticationRequestTypeDef",
     {
         "Type": ClientVpnAuthenticationTypeType,
         "ActiveDirectory": DirectoryServiceAuthenticationRequestTypeDef,
@@ -16802,15 +16458,14 @@
     "ClientVpnAuthenticationTypeDef",
     {
         "Type": ClientVpnAuthenticationTypeType,
         "ActiveDirectory": DirectoryServiceAuthenticationTypeDef,
         "MutualAuthentication": CertificateAuthenticationTypeDef,
         "FederatedAuthentication": FederatedAuthenticationTypeDef,
     },
-    total=False,
 )
 
 ClientVpnConnectionTypeDef = TypedDict(
     "ClientVpnConnectionTypeDef",
     {
         "ClientVpnEndpointId": str,
         "Timestamp": str,
@@ -16823,25 +16478,23 @@
         "EgressPackets": str,
         "ClientIp": str,
         "CommonName": str,
         "Status": ClientVpnConnectionStatusTypeDef,
         "ConnectionEndTime": str,
         "PostureComplianceStatuses": List[str],
     },
-    total=False,
 )
 
 TerminateConnectionStatusTypeDef = TypedDict(
     "TerminateConnectionStatusTypeDef",
     {
         "ConnectionId": str,
         "PreviousStatus": ClientVpnConnectionStatusTypeDef,
         "CurrentStatus": ClientVpnConnectionStatusTypeDef,
     },
-    total=False,
 )
 
 CreateClientVpnEndpointResultTypeDef = TypedDict(
     "CreateClientVpnEndpointResultTypeDef",
     {
         "ClientVpnEndpointId": str,
         "Status": ClientVpnEndpointStatusTypeDef,
@@ -16865,15 +16518,14 @@
         "DestinationCidr": str,
         "TargetSubnet": str,
         "Type": str,
         "Origin": str,
         "Status": ClientVpnRouteStatusTypeDef,
         "Description": str,
     },
-    total=False,
 )
 
 CreateClientVpnRouteResultTypeDef = TypedDict(
     "CreateClientVpnRouteResultTypeDef",
     {
         "Status": ClientVpnRouteStatusTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
@@ -16897,15 +16549,14 @@
 )
 
 VpnTunnelLogOptionsTypeDef = TypedDict(
     "VpnTunnelLogOptionsTypeDef",
     {
         "CloudWatchLogOptions": CloudWatchLogOptionsTypeDef,
     },
-    total=False,
 )
 
 GetCoipPoolUsageResultTypeDef = TypedDict(
     "GetCoipPoolUsageResultTypeDef",
     {
         "CoipPoolId": str,
         "CoipAddressUsages": List[CoipAddressUsageTypeDef],
@@ -17094,15 +16745,14 @@
         "IcmpTypeCode": IcmpTypeCodeTypeDef,
         "Ipv6CidrBlock": str,
         "PortRange": PortRangeTypeDef,
         "Protocol": str,
         "RuleAction": RuleActionType,
         "RuleNumber": int,
     },
-    total=False,
 )
 
 _RequiredReplaceNetworkAclEntryRequestNetworkAclReplaceEntryTypeDef = TypedDict(
     "_RequiredReplaceNetworkAclEntryRequestNetworkAclReplaceEntryTypeDef",
     {
         "Egress": bool,
         "Protocol": str,
@@ -17175,15 +16825,14 @@
         "InterfaceType": str,
         "NetworkCardIndex": int,
         "Ipv4Prefixes": List[Ipv4PrefixSpecificationRequestTypeDef],
         "Ipv4PrefixCount": int,
         "Ipv6Prefixes": List[Ipv6PrefixSpecificationRequestTypeDef],
         "Ipv6PrefixCount": int,
     },
-    total=False,
 )
 
 CreateReservedInstancesListingRequestRequestTypeDef = TypedDict(
     "CreateReservedInstancesListingRequestRequestTypeDef",
     {
         "ClientToken": str,
         "InstanceCount": int,
@@ -17345,24 +16994,22 @@
         "Source": str,
         "Destination": str,
         "Metric": Literal["aggregate-latency"],
         "Statistic": Literal["p50"],
         "Period": PeriodTypeType,
         "MetricPoints": List[MetricPointTypeDef],
     },
-    total=False,
 )
 
 DeleteFleetErrorItemTypeDef = TypedDict(
     "DeleteFleetErrorItemTypeDef",
     {
         "Error": DeleteFleetErrorTypeDef,
         "FleetId": str,
     },
-    total=False,
 )
 
 DeleteInstanceEventWindowResultTypeDef = TypedDict(
     "DeleteInstanceEventWindowResultTypeDef",
     {
         "InstanceEventWindowState": InstanceEventWindowStateChangeTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
@@ -17373,24 +17020,22 @@
     "DeleteLaunchTemplateVersionsResponseErrorItemTypeDef",
     {
         "LaunchTemplateId": str,
         "LaunchTemplateName": str,
         "VersionNumber": int,
         "ResponseError": ResponseErrorTypeDef,
     },
-    total=False,
 )
 
 FailedQueuedPurchaseDeletionTypeDef = TypedDict(
     "FailedQueuedPurchaseDeletionTypeDef",
     {
         "Error": DeleteQueuedReservedInstancesErrorTypeDef,
         "ReservedInstancesId": str,
     },
-    total=False,
 )
 
 _RequiredDeregisterInstanceEventNotificationAttributesRequestRequestTypeDef = TypedDict(
     "_RequiredDeregisterInstanceEventNotificationAttributesRequestRequestTypeDef",
     {
         "InstanceTagAttribute": DeregisterInstanceTagAttributeRequestTypeDef,
     },
@@ -20912,15 +20557,14 @@
 
 PrincipalIdFormatTypeDef = TypedDict(
     "PrincipalIdFormatTypeDef",
     {
         "Arn": str,
         "Statuses": List[IdFormatTypeDef],
     },
-    total=False,
 )
 
 DescribeAwsNetworkPerformanceMetricSubscriptionsResultTypeDef = TypedDict(
     "DescribeAwsNetworkPerformanceMetricSubscriptionsResultTypeDef",
     {
         "NextToken": str,
         "Subscriptions": List[SubscriptionTypeDef],
@@ -21388,15 +21032,14 @@
         "LaunchTemplate": FastLaunchLaunchTemplateSpecificationResponseTypeDef,
         "MaxParallelLaunches": int,
         "OwnerId": str,
         "State": FastLaunchStateCodeType,
         "StateTransitionReason": str,
         "StateTransitionTime": datetime,
     },
-    total=False,
 )
 
 DisableFastLaunchResultTypeDef = TypedDict(
     "DisableFastLaunchResultTypeDef",
     {
         "ImageId": str,
         "ResourceType": Literal["snapshot"],
@@ -21653,24 +21296,22 @@
         "LogDestinationType": LogDestinationTypeType,
         "LogDestination": str,
         "LogFormat": str,
         "Tags": List[TagTypeDef],
         "MaxAggregationInterval": int,
         "DestinationOptions": DestinationOptionsResponseTypeDef,
     },
-    total=False,
 )
 
 DisableFastSnapshotRestoreStateErrorItemTypeDef = TypedDict(
     "DisableFastSnapshotRestoreStateErrorItemTypeDef",
     {
         "AvailabilityZone": str,
         "Error": DisableFastSnapshotRestoreStateErrorTypeDef,
     },
-    total=False,
 )
 
 DisableTransitGatewayRouteTablePropagationResultTypeDef = TypedDict(
     "DisableTransitGatewayRouteTablePropagationResultTypeDef",
     {
         "Propagation": TransitGatewayPropagationTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
@@ -21724,38 +21365,35 @@
         "BytesConverted": int,
         "Description": str,
         "Image": DiskImageDescriptionTypeDef,
         "Status": str,
         "StatusMessage": str,
         "Volume": DiskImageVolumeDescriptionTypeDef,
     },
-    total=False,
 )
 
 ImportVolumeTaskDetailsTypeDef = TypedDict(
     "ImportVolumeTaskDetailsTypeDef",
     {
         "AvailabilityZone": str,
         "BytesConverted": int,
         "Description": str,
         "Image": DiskImageDescriptionTypeDef,
         "Volume": DiskImageVolumeDescriptionTypeDef,
     },
-    total=False,
 )
 
 InstanceStorageInfoTypeDef = TypedDict(
     "InstanceStorageInfoTypeDef",
     {
         "TotalSizeInGB": int,
         "Disks": List[DiskInfoTypeDef],
         "NvmeSupport": EphemeralNvmeSupportType,
         "EncryptionSupport": InstanceStorageEncryptionSupportType,
     },
-    total=False,
 )
 
 VpcEndpointConnectionTypeDef = TypedDict(
     "VpcEndpointConnectionTypeDef",
     {
         "ServiceId": str,
         "VpcEndpointId": str,
@@ -21765,15 +21403,14 @@
         "DnsEntries": List[DnsEntryTypeDef],
         "NetworkLoadBalancerArns": List[str],
         "GatewayLoadBalancerArns": List[str],
         "IpAddressType": IpAddressTypeType,
         "VpcEndpointConnectionId": str,
         "Tags": List[TagTypeDef],
     },
-    total=False,
 )
 
 _RequiredModifyClientVpnEndpointRequestRequestTypeDef = TypedDict(
     "_RequiredModifyClientVpnEndpointRequestRequestTypeDef",
     {
         "ClientVpnEndpointId": str,
     },
@@ -21808,15 +21445,14 @@
     "EbsInfoTypeDef",
     {
         "EbsOptimizedSupport": EbsOptimizedSupportType,
         "EncryptionSupport": EbsEncryptionSupportType,
         "EbsOptimizedInfo": EbsOptimizedInfoTypeDef,
         "NvmeSupport": EbsNvmeSupportType,
     },
-    total=False,
 )
 
 InstanceBlockDeviceMappingSpecificationTypeDef = TypedDict(
     "InstanceBlockDeviceMappingSpecificationTypeDef",
     {
         "DeviceName": str,
         "Ebs": EbsInstanceBlockDeviceSpecificationTypeDef,
@@ -21828,50 +21464,46 @@
 
 InstanceBlockDeviceMappingTypeDef = TypedDict(
     "InstanceBlockDeviceMappingTypeDef",
     {
         "DeviceName": str,
         "Ebs": EbsInstanceBlockDeviceTypeDef,
     },
-    total=False,
 )
 
 EgressOnlyInternetGatewayTypeDef = TypedDict(
     "EgressOnlyInternetGatewayTypeDef",
     {
         "Attachments": List[InternetGatewayAttachmentTypeDef],
         "EgressOnlyInternetGatewayId": str,
         "Tags": List[TagTypeDef],
     },
-    total=False,
 )
 
 InternetGatewayTypeDef = TypedDict(
     "InternetGatewayTypeDef",
     {
         "Attachments": List[InternetGatewayAttachmentTypeDef],
         "InternetGatewayId": str,
         "OwnerId": str,
         "Tags": List[TagTypeDef],
     },
-    total=False,
 )
 
 ElasticGpusTypeDef = TypedDict(
     "ElasticGpusTypeDef",
     {
         "ElasticGpuId": str,
         "AvailabilityZone": str,
         "ElasticGpuType": str,
         "ElasticGpuHealth": ElasticGpuHealthTypeDef,
         "ElasticGpuState": Literal["ATTACHED"],
         "InstanceId": str,
         "Tags": List[TagTypeDef],
     },
-    total=False,
 )
 
 EnaSrdSpecificationTypeDef = TypedDict(
     "EnaSrdSpecificationTypeDef",
     {
         "EnaSrdEnabled": bool,
         "EnaSrdUdpSpecification": EnaSrdUdpSpecificationTypeDef,
@@ -21904,35 +21536,32 @@
 
 EnableFastSnapshotRestoreStateErrorItemTypeDef = TypedDict(
     "EnableFastSnapshotRestoreStateErrorItemTypeDef",
     {
         "AvailabilityZone": str,
         "Error": EnableFastSnapshotRestoreStateErrorTypeDef,
     },
-    total=False,
 )
 
 HistoryRecordEntryTypeDef = TypedDict(
     "HistoryRecordEntryTypeDef",
     {
         "EventInformation": EventInformationTypeDef,
         "EventType": FleetEventTypeType,
         "Timestamp": datetime,
     },
-    total=False,
 )
 
 HistoryRecordTypeDef = TypedDict(
     "HistoryRecordTypeDef",
     {
         "EventInformation": EventInformationTypeDef,
         "EventType": EventTypeType,
         "Timestamp": datetime,
     },
-    total=False,
 )
 
 ExportImageResultTypeDef = TypedDict(
     "ExportImageResultTypeDef",
     {
         "Description": str,
         "DiskImageFormat": DiskImageFormatType,
@@ -21956,40 +21585,37 @@
         "ImageId": str,
         "Progress": str,
         "S3ExportLocation": ExportTaskS3LocationTypeDef,
         "Status": str,
         "StatusMessage": str,
         "Tags": List[TagTypeDef],
     },
-    total=False,
 )
 
 ExportTaskTypeDef = TypedDict(
     "ExportTaskTypeDef",
     {
         "Description": str,
         "ExportTaskId": str,
         "ExportToS3Task": ExportToS3TaskTypeDef,
         "InstanceExportDetails": InstanceExportDetailsTypeDef,
         "State": ExportTaskStateType,
         "StatusMessage": str,
         "Tags": List[TagTypeDef],
     },
-    total=False,
 )
 
 PathFilterTypeDef = TypedDict(
     "PathFilterTypeDef",
     {
         "SourceAddress": str,
         "SourcePortRange": FilterPortRangeTypeDef,
         "DestinationAddress": str,
         "DestinationPortRange": FilterPortRangeTypeDef,
     },
-    total=False,
 )
 
 FleetSpotMaintenanceStrategiesRequestTypeDef = TypedDict(
     "FleetSpotMaintenanceStrategiesRequestTypeDef",
     {
         "CapacityRebalance": FleetSpotCapacityRebalanceRequestTypeDef,
     },
@@ -21997,38 +21623,35 @@
 )
 
 FleetSpotMaintenanceStrategiesTypeDef = TypedDict(
     "FleetSpotMaintenanceStrategiesTypeDef",
     {
         "CapacityRebalance": FleetSpotCapacityRebalanceTypeDef,
     },
-    total=False,
 )
 
 FpgaDeviceInfoTypeDef = TypedDict(
     "FpgaDeviceInfoTypeDef",
     {
         "Name": str,
         "Manufacturer": str,
         "Count": int,
         "MemoryInfo": FpgaDeviceMemoryInfoTypeDef,
     },
-    total=False,
 )
 
 FpgaImageAttributeTypeDef = TypedDict(
     "FpgaImageAttributeTypeDef",
     {
         "FpgaImageId": str,
         "Name": str,
         "Description": str,
         "LoadPermissions": List[LoadPermissionTypeDef],
         "ProductCodes": List[ProductCodeTypeDef],
     },
-    total=False,
 )
 
 FpgaImageTypeDef = TypedDict(
     "FpgaImageTypeDef",
     {
         "FpgaImageId": str,
         "FpgaImageGlobalId": str,
@@ -22043,15 +21666,14 @@
         "OwnerAlias": str,
         "ProductCodes": List[ProductCodeTypeDef],
         "Tags": List[TagTypeDef],
         "Public": bool,
         "DataRetentionSupport": bool,
         "InstanceTypes": List[str],
     },
-    total=False,
 )
 
 GetAssociatedIpv6PoolCidrsResultTypeDef = TypedDict(
     "GetAssociatedIpv6PoolCidrsResultTypeDef",
     {
         "Ipv6CidrAssociations": List[Ipv6CidrAssociationTypeDef],
         "NextToken": str,
@@ -22150,15 +21772,14 @@
 
 ReservedInstanceReservationValueTypeDef = TypedDict(
     "ReservedInstanceReservationValueTypeDef",
     {
         "ReservationValue": ReservationValueTypeDef,
         "ReservedInstanceId": str,
     },
-    total=False,
 )
 
 GetSpotPlacementScoresResultTypeDef = TypedDict(
     "GetSpotPlacementScoresResultTypeDef",
     {
         "SpotPlacementScores": List[SpotPlacementScoreTypeDef],
         "NextToken": str,
@@ -22219,27 +21840,25 @@
     "GpuDeviceInfoTypeDef",
     {
         "Name": str,
         "Manufacturer": str,
         "Count": int,
         "MemoryInfo": GpuDeviceMemoryInfoTypeDef,
     },
-    total=False,
 )
 
 IamInstanceProfileAssociationTypeDef = TypedDict(
     "IamInstanceProfileAssociationTypeDef",
     {
         "AssociationId": str,
         "InstanceId": str,
         "IamInstanceProfile": IamInstanceProfileTypeDef,
         "State": IamInstanceProfileAssociationStateType,
         "Timestamp": datetime,
     },
-    total=False,
 )
 
 LaunchPermissionModificationsTypeDef = TypedDict(
     "LaunchPermissionModificationsTypeDef",
     {
         "Add": Sequence[LaunchPermissionTypeDef],
         "Remove": Sequence[LaunchPermissionTypeDef],
@@ -22289,15 +21908,14 @@
         "OutpostArn": str,
         "OwnerId": str,
         "State": str,
         "Tags": List[TagTypeDef],
         "Mode": LocalGatewayRouteTableModeType,
         "StateReason": StateReasonTypeDef,
     },
-    total=False,
 )
 
 ImportInstanceLaunchSpecificationTypeDef = TypedDict(
     "ImportInstanceLaunchSpecificationTypeDef",
     {
         "AdditionalInfo": str,
         "Architecture": ArchitectureValuesType,
@@ -22315,15 +21933,14 @@
 )
 
 InferenceAcceleratorInfoTypeDef = TypedDict(
     "InferenceAcceleratorInfoTypeDef",
     {
         "Accelerators": List[InferenceDeviceInfoTypeDef],
     },
-    total=False,
 )
 
 _RequiredModifyInstanceCreditSpecificationRequestRequestTypeDef = TypedDict(
     "_RequiredModifyInstanceCreditSpecificationRequestRequestTypeDef",
     {
         "InstanceCreditSpecifications": Sequence[InstanceCreditSpecificationRequestTypeDef],
     },
@@ -22389,26 +22006,24 @@
 
 InstanceMonitoringTypeDef = TypedDict(
     "InstanceMonitoringTypeDef",
     {
         "InstanceId": str,
         "Monitoring": MonitoringTypeDef,
     },
-    total=False,
 )
 
 InstancePrivateIpAddressTypeDef = TypedDict(
     "InstancePrivateIpAddressTypeDef",
     {
         "Association": InstanceNetworkInterfaceAssociationTypeDef,
         "Primary": bool,
         "PrivateDnsName": str,
         "PrivateIpAddress": str,
     },
-    total=False,
 )
 
 _RequiredInstanceRequirementsRequestTypeDef = TypedDict(
     "_RequiredInstanceRequirementsRequestTypeDef",
     {
         "VCpuCount": VCpuCountRangeRequestTypeDef,
         "MemoryMiB": MemoryMiBRequestTypeDef,
@@ -22470,34 +22085,31 @@
         "AcceleratorCount": AcceleratorCountTypeDef,
         "AcceleratorManufacturers": List[AcceleratorManufacturerType],
         "AcceleratorNames": List[AcceleratorNameType],
         "AcceleratorTotalMemoryMiB": AcceleratorTotalMemoryMiBTypeDef,
         "NetworkBandwidthGbps": NetworkBandwidthGbpsTypeDef,
         "AllowedInstanceTypes": List[str],
     },
-    total=False,
 )
 
 InstanceStateChangeTypeDef = TypedDict(
     "InstanceStateChangeTypeDef",
     {
         "CurrentState": InstanceStateTypeDef,
         "InstanceId": str,
         "PreviousState": InstanceStateTypeDef,
     },
-    total=False,
 )
 
 InstanceStatusSummaryTypeDef = TypedDict(
     "InstanceStatusSummaryTypeDef",
     {
         "Details": List[InstanceStatusDetailsTypeDef],
         "Status": SummaryStatusType,
     },
-    total=False,
 )
 
 ModifyInstanceEventStartTimeResultTypeDef = TypedDict(
     "ModifyInstanceEventStartTimeResultTypeDef",
     {
         "Event": InstanceStatusEventTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
@@ -22524,15 +22136,14 @@
         "FromPort": int,
         "IpProtocol": str,
         "IpRanges": List[str],
         "PrefixListIds": List[str],
         "ToPort": int,
         "UserIdGroupPairs": List[UserIdGroupPairTypeDef],
     },
-    total=False,
 )
 
 _RequiredProvisionIpamPoolCidrRequestRequestTypeDef = TypedDict(
     "_RequiredProvisionIpamPoolCidrRequestRequestTypeDef",
     {
         "IpamPoolId": str,
     },
@@ -22560,15 +22171,14 @@
     {
         "AccountId": str,
         "DiscoveryRegion": str,
         "FailureReason": IpamDiscoveryFailureReasonTypeDef,
         "LastAttemptedDiscoveryTime": datetime,
         "LastSuccessfulDiscoveryTime": datetime,
     },
-    total=False,
 )
 
 IpamDiscoveredResourceCidrTypeDef = TypedDict(
     "IpamDiscoveredResourceCidrTypeDef",
     {
         "IpamResourceDiscoveryId": str,
         "ResourceRegion": str,
@@ -22577,15 +22187,14 @@
         "ResourceCidr": str,
         "ResourceType": IpamResourceTypeType,
         "ResourceTags": List[IpamResourceTagTypeDef],
         "IpUsage": float,
         "VpcId": str,
         "SampleTime": datetime,
     },
-    total=False,
 )
 
 IpamPoolTypeDef = TypedDict(
     "IpamPoolTypeDef",
     {
         "OwnerId": str,
         "IpamPoolId": str,
@@ -22607,15 +22216,14 @@
         "AllocationMaxNetmaskLength": int,
         "AllocationDefaultNetmaskLength": int,
         "AllocationResourceTags": List[IpamResourceTagTypeDef],
         "Tags": List[TagTypeDef],
         "AwsService": Literal["ec2"],
         "PublicIpSource": IpamPoolPublicIpSourceType,
     },
-    total=False,
 )
 
 IpamResourceCidrTypeDef = TypedDict(
     "IpamResourceCidrTypeDef",
     {
         "IpamId": str,
         "IpamScopeId": str,
@@ -22629,15 +22237,14 @@
         "ResourceTags": List[IpamResourceTagTypeDef],
         "IpUsage": float,
         "ComplianceStatus": IpamComplianceStatusType,
         "ManagementState": IpamManagementStateType,
         "OverlapStatus": IpamOverlapStatusType,
         "VpcId": str,
     },
-    total=False,
 )
 
 IpamResourceDiscoveryTypeDef = TypedDict(
     "IpamResourceDiscoveryTypeDef",
     {
         "OwnerId": str,
         "IpamResourceDiscoveryId": str,
@@ -22645,15 +22252,14 @@
         "IpamResourceDiscoveryRegion": str,
         "Description": str,
         "OperatingRegions": List[IpamOperatingRegionTypeDef],
         "IsDefault": bool,
         "State": IpamResourceDiscoveryStateType,
         "Tags": List[TagTypeDef],
     },
-    total=False,
 )
 
 IpamTypeDef = TypedDict(
     "IpamTypeDef",
     {
         "OwnerId": str,
         "IpamId": str,
@@ -22666,38 +22272,35 @@
         "OperatingRegions": List[IpamOperatingRegionTypeDef],
         "State": IpamStateType,
         "Tags": List[TagTypeDef],
         "DefaultResourceDiscoveryId": str,
         "DefaultResourceDiscoveryAssociationId": str,
         "ResourceDiscoveryAssociationCount": int,
     },
-    total=False,
 )
 
 IpamPoolCidrTypeDef = TypedDict(
     "IpamPoolCidrTypeDef",
     {
         "Cidr": str,
         "State": IpamPoolCidrStateType,
         "FailureReason": IpamPoolCidrFailureReasonTypeDef,
         "IpamPoolCidrId": str,
         "NetmaskLength": int,
     },
-    total=False,
 )
 
 Ipv6PoolTypeDef = TypedDict(
     "Ipv6PoolTypeDef",
     {
         "PoolId": str,
         "Description": str,
         "PoolCidrBlocks": List[PoolCidrBlockTypeDef],
         "Tags": List[TagTypeDef],
     },
-    total=False,
 )
 
 LaunchTemplateInstanceNetworkInterfaceSpecificationTypeDef = TypedDict(
     "LaunchTemplateInstanceNetworkInterfaceSpecificationTypeDef",
     {
         "AssociateCarrierIpAddress": bool,
         "AssociatePublicIpAddress": bool,
@@ -22715,15 +22318,14 @@
         "SubnetId": str,
         "NetworkCardIndex": int,
         "Ipv4Prefixes": List[Ipv4PrefixSpecificationResponseTypeDef],
         "Ipv4PrefixCount": int,
         "Ipv6Prefixes": List[Ipv6PrefixSpecificationResponseTypeDef],
         "Ipv6PrefixCount": int,
     },
-    total=False,
 )
 
 LaunchTemplateBlockDeviceMappingRequestTypeDef = TypedDict(
     "LaunchTemplateBlockDeviceMappingRequestTypeDef",
     {
         "DeviceName": str,
         "VirtualName": str,
@@ -22737,15 +22339,14 @@
     "LaunchTemplateBlockDeviceMappingTypeDef",
     {
         "DeviceName": str,
         "VirtualName": str,
         "Ebs": LaunchTemplateEbsBlockDeviceTypeDef,
         "NoDevice": str,
     },
-    total=False,
 )
 
 LaunchTemplateInstanceMarketOptionsRequestTypeDef = TypedDict(
     "LaunchTemplateInstanceMarketOptionsRequestTypeDef",
     {
         "MarketType": Literal["spot"],
         "SpotOptions": LaunchTemplateSpotMarketOptionsRequestTypeDef,
@@ -22755,15 +22356,14 @@
 
 LaunchTemplateInstanceMarketOptionsTypeDef = TypedDict(
     "LaunchTemplateInstanceMarketOptionsTypeDef",
     {
         "MarketType": Literal["spot"],
         "SpotOptions": LaunchTemplateSpotMarketOptionsTypeDef,
     },
-    total=False,
 )
 
 ListSnapshotsInRecycleBinResultTypeDef = TypedDict(
     "ListSnapshotsInRecycleBinResultTypeDef",
     {
         "Snapshots": List[SnapshotRecycleBinInfoTypeDef],
         "NextToken": str,
@@ -22873,15 +22473,14 @@
 
 ReservedInstancesModificationResultTypeDef = TypedDict(
     "ReservedInstancesModificationResultTypeDef",
     {
         "ReservedInstancesId": str,
         "TargetConfiguration": ReservedInstancesConfigurationTypeDef,
     },
-    total=False,
 )
 
 _RequiredModifyTransitGatewayRequestRequestTypeDef = TypedDict(
     "_RequiredModifyTransitGatewayRequestRequestTypeDef",
     {
         "TransitGatewayId": str,
     },
@@ -23016,15 +22615,14 @@
         "ProvisionedBandwidth": ProvisionedBandwidthTypeDef,
         "State": NatGatewayStateType,
         "SubnetId": str,
         "VpcId": str,
         "Tags": List[TagTypeDef],
         "ConnectivityType": ConnectivityTypeType,
     },
-    total=False,
 )
 
 NetworkInfoTypeDef = TypedDict(
     "NetworkInfoTypeDef",
     {
         "NetworkPerformance": str,
         "MaximumNetworkInterfaces": int,
@@ -23036,39 +22634,36 @@
         "Ipv6Supported": bool,
         "EnaSupport": EnaSupportType,
         "EfaSupported": bool,
         "EfaInfo": EfaInfoTypeDef,
         "EncryptionInTransitSupported": bool,
         "EnaSrdSupported": bool,
     },
-    total=False,
 )
 
 NetworkInterfacePrivateIpAddressTypeDef = TypedDict(
     "NetworkInterfacePrivateIpAddressTypeDef",
     {
         "Association": NetworkInterfaceAssociationTypeDef,
         "Primary": bool,
         "PrivateDnsName": str,
         "PrivateIpAddress": str,
     },
-    total=False,
 )
 
 NetworkInterfacePermissionTypeDef = TypedDict(
     "NetworkInterfacePermissionTypeDef",
     {
         "NetworkInterfacePermissionId": str,
         "NetworkInterfaceId": str,
         "AwsAccountId": str,
         "AwsService": str,
         "Permission": InterfacePermissionTypeType,
         "PermissionState": NetworkInterfacePermissionStateTypeDef,
     },
-    total=False,
 )
 
 VerifiedAccessTrustProviderTypeDef = TypedDict(
     "VerifiedAccessTrustProviderTypeDef",
     {
         "VerifiedAccessTrustProviderId": str,
         "Description": str,
@@ -23078,15 +22673,14 @@
         "OidcOptions": OidcOptionsTypeDef,
         "DeviceOptions": DeviceOptionsTypeDef,
         "PolicyReferenceName": str,
         "CreationTime": str,
         "LastUpdatedTime": str,
         "Tags": List[TagTypeDef],
     },
-    total=False,
 )
 
 PathRequestFilterTypeDef = TypedDict(
     "PathRequestFilterTypeDef",
     {
         "SourceAddress": str,
         "SourcePortRange": RequestFilterPortRangeTypeDef,
@@ -23115,23 +22709,21 @@
 
 PathStatementTypeDef = TypedDict(
     "PathStatementTypeDef",
     {
         "PacketHeaderStatement": PacketHeaderStatementTypeDef,
         "ResourceStatement": ResourceStatementTypeDef,
     },
-    total=False,
 )
 
 ThroughResourcesStatementTypeDef = TypedDict(
     "ThroughResourcesStatementTypeDef",
     {
         "ResourceStatement": ResourceStatementTypeDef,
     },
-    total=False,
 )
 
 ReservedInstancesListingTypeDef = TypedDict(
     "ReservedInstancesListingTypeDef",
     {
         "ClientToken": str,
         "CreateDate": datetime,
@@ -23140,15 +22732,14 @@
         "ReservedInstancesId": str,
         "ReservedInstancesListingId": str,
         "Status": ListingStatusType,
         "StatusMessage": str,
         "Tags": List[TagTypeDef],
         "UpdateDate": datetime,
     },
-    total=False,
 )
 
 ProvisionPublicIpv4PoolCidrResultTypeDef = TypedDict(
     "ProvisionPublicIpv4PoolCidrResultTypeDef",
     {
         "PoolId": str,
         "PoolAddressRange": PublicIpv4PoolRangeTypeDef,
@@ -23163,15 +22754,14 @@
         "Description": str,
         "PoolAddressRanges": List[PublicIpv4PoolRangeTypeDef],
         "TotalAddressCount": int,
         "TotalAvailableAddressCount": int,
         "NetworkBorderGroup": str,
         "Tags": List[TagTypeDef],
     },
-    total=False,
 )
 
 _RequiredPurchaseScheduledInstancesRequestRequestTypeDef = TypedDict(
     "_RequiredPurchaseScheduledInstancesRequestRequestTypeDef",
     {
         "PurchaseRequests": Sequence[PurchaseRequestTypeDef],
     },
@@ -23229,15 +22819,14 @@
         "Marketplace": bool,
         "OfferingClass": OfferingClassTypeType,
         "OfferingType": OfferingTypeValuesType,
         "PricingDetails": List[PricingDetailTypeDef],
         "RecurringCharges": List[RecurringChargeTypeDef],
         "Scope": scopeType,
     },
-    total=False,
 )
 
 ReservedInstancesTypeDef = TypedDict(
     "ReservedInstancesTypeDef",
     {
         "AvailabilityZone": str,
         "Duration": int,
@@ -23254,15 +22843,14 @@
         "InstanceTenancy": TenancyType,
         "OfferingClass": OfferingClassTypeType,
         "OfferingType": OfferingTypeValuesType,
         "RecurringCharges": List[RecurringChargeTypeDef],
         "Scope": scopeType,
         "Tags": List[TagTypeDef],
     },
-    total=False,
 )
 
 SecurityGroupRuleTypeDef = TypedDict(
     "SecurityGroupRuleTypeDef",
     {
         "SecurityGroupRuleId": str,
         "GroupId": str,
@@ -23274,15 +22862,14 @@
         "CidrIpv4": str,
         "CidrIpv6": str,
         "PrefixListId": str,
         "ReferencedGroupInfo": ReferencedSecurityGroupTypeDef,
         "Description": str,
         "Tags": List[TagTypeDef],
     },
-    total=False,
 )
 
 _RequiredRegisterInstanceEventNotificationAttributesRequestRequestTypeDef = TypedDict(
     "_RequiredRegisterInstanceEventNotificationAttributesRequestRequestTypeDef",
     {
         "InstanceTagAttribute": RegisterInstanceTagAttributeRequestTypeDef,
     },
@@ -23338,15 +22925,14 @@
         "NetworkPlatform": str,
         "Platform": str,
         "PurchaseToken": str,
         "Recurrence": ScheduledInstanceRecurrenceTypeDef,
         "SlotDurationInHours": int,
         "TotalScheduledInstanceHours": int,
     },
-    total=False,
 )
 
 ScheduledInstanceTypeDef = TypedDict(
     "ScheduledInstanceTypeDef",
     {
         "AvailabilityZone": str,
         "CreateDate": datetime,
@@ -23360,15 +22946,14 @@
         "Recurrence": ScheduledInstanceRecurrenceTypeDef,
         "ScheduledInstanceId": str,
         "SlotDurationInHours": int,
         "TermEndDate": datetime,
         "TermStartDate": datetime,
         "TotalScheduledInstanceHours": int,
     },
-    total=False,
 )
 
 ScheduledInstancesBlockDeviceMappingTypeDef = TypedDict(
     "ScheduledInstancesBlockDeviceMappingTypeDef",
     {
         "DeviceName": str,
         "Ebs": ScheduledInstancesEbsTypeDef,
@@ -23425,15 +23010,14 @@
         "NetworkInterfaceIds": List[str],
         "DnsEntries": List[DnsEntryTypeDef],
         "CreationTimestamp": datetime,
         "Tags": List[TagTypeDef],
         "OwnerId": str,
         "LastError": LastErrorTypeDef,
     },
-    total=False,
 )
 
 _RequiredSecurityGroupRuleUpdateTypeDef = TypedDict(
     "_RequiredSecurityGroupRuleUpdateTypeDef",
     {
         "SecurityGroupRuleId": str,
     },
@@ -23466,15 +23050,14 @@
         "SupportedIpAddressTypes": List[ServiceConnectivityTypeType],
         "BaseEndpointDnsNames": List[str],
         "PrivateDnsName": str,
         "PrivateDnsNameConfiguration": PrivateDnsNameConfigurationTypeDef,
         "PayerResponsibility": Literal["ServiceOwner"],
         "Tags": List[TagTypeDef],
     },
-    total=False,
 )
 
 ServiceDetailTypeDef = TypedDict(
     "ServiceDetailTypeDef",
     {
         "ServiceName": str,
         "ServiceId": str,
@@ -23488,15 +23071,14 @@
         "AcceptanceRequired": bool,
         "ManagesVpcEndpoints": bool,
         "PayerResponsibility": Literal["ServiceOwner"],
         "Tags": List[TagTypeDef],
         "PrivateDnsNameVerificationState": DnsNameStateType,
         "SupportedIpAddressTypes": List[ServiceConnectivityTypeType],
     },
-    total=False,
 )
 
 SnapshotDetailTypeDef = TypedDict(
     "SnapshotDetailTypeDef",
     {
         "Description": str,
         "DeviceName": str,
@@ -23505,15 +23087,14 @@
         "Progress": str,
         "SnapshotId": str,
         "Status": str,
         "StatusMessage": str,
         "Url": str,
         "UserBucket": UserBucketDetailsTypeDef,
     },
-    total=False,
 )
 
 SnapshotTaskDetailTypeDef = TypedDict(
     "SnapshotTaskDetailTypeDef",
     {
         "Description": str,
         "DiskImageSize": float,
@@ -23523,87 +23104,79 @@
         "Progress": str,
         "SnapshotId": str,
         "Status": str,
         "StatusMessage": str,
         "Url": str,
         "UserBucket": UserBucketDetailsTypeDef,
     },
-    total=False,
 )
 
 SpotMaintenanceStrategiesTypeDef = TypedDict(
     "SpotMaintenanceStrategiesTypeDef",
     {
         "CapacityRebalance": SpotCapacityRebalanceTypeDef,
     },
-    total=False,
 )
 
 SpotDatafeedSubscriptionTypeDef = TypedDict(
     "SpotDatafeedSubscriptionTypeDef",
     {
         "Bucket": str,
         "Fault": SpotInstanceStateFaultTypeDef,
         "OwnerId": str,
         "Prefix": str,
         "State": DatafeedSubscriptionStateType,
     },
-    total=False,
 )
 
 TransitGatewayMulticastDomainAssociationTypeDef = TypedDict(
     "TransitGatewayMulticastDomainAssociationTypeDef",
     {
         "TransitGatewayAttachmentId": str,
         "ResourceId": str,
         "ResourceType": TransitGatewayAttachmentResourceTypeType,
         "ResourceOwnerId": str,
         "Subnet": SubnetAssociationTypeDef,
     },
-    total=False,
 )
 
 TransitGatewayMulticastDomainAssociationsTypeDef = TypedDict(
     "TransitGatewayMulticastDomainAssociationsTypeDef",
     {
         "TransitGatewayMulticastDomainId": str,
         "TransitGatewayAttachmentId": str,
         "ResourceId": str,
         "ResourceType": TransitGatewayAttachmentResourceTypeType,
         "ResourceOwnerId": str,
         "Subnets": List[SubnetAssociationTypeDef],
     },
-    total=False,
 )
 
 SubnetIpv6CidrBlockAssociationTypeDef = TypedDict(
     "SubnetIpv6CidrBlockAssociationTypeDef",
     {
         "AssociationId": str,
         "Ipv6CidrBlock": str,
         "Ipv6CidrBlockState": SubnetCidrBlockStateTypeDef,
     },
-    total=False,
 )
 
 TargetReservationValueTypeDef = TypedDict(
     "TargetReservationValueTypeDef",
     {
         "ReservationValue": ReservationValueTypeDef,
         "TargetConfiguration": TargetConfigurationTypeDef,
     },
-    total=False,
 )
 
 TargetGroupsConfigTypeDef = TypedDict(
     "TargetGroupsConfigTypeDef",
     {
         "TargetGroups": List[TargetGroupTypeDef],
     },
-    total=False,
 )
 
 TrafficMirrorFilterRuleTypeDef = TypedDict(
     "TrafficMirrorFilterRuleTypeDef",
     {
         "TrafficMirrorFilterRuleId": str,
         "TrafficMirrorFilterId": str,
@@ -23613,15 +23186,14 @@
         "Protocol": int,
         "DestinationPortRange": TrafficMirrorPortRangeTypeDef,
         "SourcePortRange": TrafficMirrorPortRangeTypeDef,
         "DestinationCidrBlock": str,
         "SourceCidrBlock": str,
         "Description": str,
     },
-    total=False,
 )
 
 TransitGatewayAttachmentTypeDef = TypedDict(
     "TransitGatewayAttachmentTypeDef",
     {
         "TransitGatewayAttachmentId": str,
         "TransitGatewayId": str,
@@ -23630,71 +23202,66 @@
         "ResourceType": TransitGatewayAttachmentResourceTypeType,
         "ResourceId": str,
         "State": TransitGatewayAttachmentStateType,
         "Association": TransitGatewayAttachmentAssociationTypeDef,
         "CreationTime": datetime,
         "Tags": List[TagTypeDef],
     },
-    total=False,
 )
 
 TransitGatewayConnectPeerConfigurationTypeDef = TypedDict(
     "TransitGatewayConnectPeerConfigurationTypeDef",
     {
         "TransitGatewayAddress": str,
         "PeerAddress": str,
         "InsideCidrBlocks": List[str],
         "Protocol": Literal["gre"],
         "BgpConfigurations": List[TransitGatewayAttachmentBgpConfigurationTypeDef],
     },
-    total=False,
 )
 
 TransitGatewayConnectTypeDef = TypedDict(
     "TransitGatewayConnectTypeDef",
     {
         "TransitGatewayAttachmentId": str,
         "TransportTransitGatewayAttachmentId": str,
         "TransitGatewayId": str,
         "State": TransitGatewayAttachmentStateType,
         "CreationTime": datetime,
         "Options": TransitGatewayConnectOptionsTypeDef,
         "Tags": List[TagTypeDef],
     },
-    total=False,
 )
 
 TransitGatewayMulticastDomainTypeDef = TypedDict(
     "TransitGatewayMulticastDomainTypeDef",
     {
         "TransitGatewayMulticastDomainId": str,
         "TransitGatewayId": str,
         "TransitGatewayMulticastDomainArn": str,
         "OwnerId": str,
         "Options": TransitGatewayMulticastDomainOptionsTypeDef,
         "State": TransitGatewayMulticastDomainStateType,
         "CreationTime": datetime,
         "Tags": List[TagTypeDef],
     },
-    total=False,
 )
 
 TransitGatewayTypeDef = TypedDict(
     "TransitGatewayTypeDef",
     {
         "TransitGatewayId": str,
         "TransitGatewayArn": str,
         "State": TransitGatewayStateType,
         "OwnerId": str,
         "Description": str,
         "CreationTime": datetime,
         "Options": TransitGatewayOptionsTypeDef,
         "Tags": List[TagTypeDef],
     },
-    total=False,
 )
 
 TransitGatewayPeeringAttachmentTypeDef = TypedDict(
     "TransitGatewayPeeringAttachmentTypeDef",
     {
         "TransitGatewayAttachmentId": str,
         "AccepterTransitGatewayAttachmentId": str,
@@ -23702,54 +23269,50 @@
         "AccepterTgwInfo": PeeringTgwInfoTypeDef,
         "Options": TransitGatewayPeeringAttachmentOptionsTypeDef,
         "Status": PeeringAttachmentStatusTypeDef,
         "State": TransitGatewayAttachmentStateType,
         "CreationTime": datetime,
         "Tags": List[TagTypeDef],
     },
-    total=False,
 )
 
 TransitGatewayPolicyRuleTypeDef = TypedDict(
     "TransitGatewayPolicyRuleTypeDef",
     {
         "SourceCidrBlock": str,
         "SourcePortRange": str,
         "DestinationCidrBlock": str,
         "DestinationPortRange": str,
         "Protocol": str,
         "MetaData": TransitGatewayPolicyRuleMetaDataTypeDef,
     },
-    total=False,
 )
 
 TransitGatewayPrefixListReferenceTypeDef = TypedDict(
     "TransitGatewayPrefixListReferenceTypeDef",
     {
         "TransitGatewayRouteTableId": str,
         "PrefixListId": str,
         "PrefixListOwnerId": str,
         "State": TransitGatewayPrefixListReferenceStateType,
         "Blackhole": bool,
         "TransitGatewayAttachment": TransitGatewayPrefixListAttachmentTypeDef,
     },
-    total=False,
 )
 
 TransitGatewayRouteTypeDef = TypedDict(
     "TransitGatewayRouteTypeDef",
     {
         "DestinationCidrBlock": str,
         "PrefixListId": str,
         "TransitGatewayRouteTableAnnouncementId": str,
         "TransitGatewayAttachments": List[TransitGatewayRouteAttachmentTypeDef],
         "Type": TransitGatewayRouteTypeType,
         "State": TransitGatewayRouteStateType,
     },
-    total=False,
 )
 
 TransitGatewayVpcAttachmentTypeDef = TypedDict(
     "TransitGatewayVpcAttachmentTypeDef",
     {
         "TransitGatewayAttachmentId": str,
         "TransitGatewayId": str,
@@ -23757,41 +23320,37 @@
         "VpcOwnerId": str,
         "State": TransitGatewayAttachmentStateType,
         "SubnetIds": List[str],
         "CreationTime": datetime,
         "Options": TransitGatewayVpcAttachmentOptionsTypeDef,
         "Tags": List[TagTypeDef],
     },
-    total=False,
 )
 
 UnsuccessfulInstanceCreditSpecificationItemTypeDef = TypedDict(
     "UnsuccessfulInstanceCreditSpecificationItemTypeDef",
     {
         "InstanceId": str,
         "Error": UnsuccessfulInstanceCreditSpecificationItemErrorTypeDef,
     },
-    total=False,
 )
 
 UnsuccessfulItemTypeDef = TypedDict(
     "UnsuccessfulItemTypeDef",
     {
         "Error": UnsuccessfulItemErrorTypeDef,
         "ResourceId": str,
     },
-    total=False,
 )
 
 ValidationWarningTypeDef = TypedDict(
     "ValidationWarningTypeDef",
     {
         "Errors": List[ValidationErrorTypeDef],
     },
-    total=False,
 )
 
 VerifiedAccessEndpointTypeDef = TypedDict(
     "VerifiedAccessEndpointTypeDef",
     {
         "VerifiedAccessInstanceId": str,
         "VerifiedAccessGroupId": str,
@@ -23808,60 +23367,55 @@
         "Status": VerifiedAccessEndpointStatusTypeDef,
         "Description": str,
         "CreationTime": str,
         "LastUpdatedTime": str,
         "DeletionTime": str,
         "Tags": List[TagTypeDef],
     },
-    total=False,
 )
 
 VerifiedAccessInstanceTypeDef = TypedDict(
     "VerifiedAccessInstanceTypeDef",
     {
         "VerifiedAccessInstanceId": str,
         "Description": str,
         "VerifiedAccessTrustProviders": List[VerifiedAccessTrustProviderCondensedTypeDef],
         "CreationTime": str,
         "LastUpdatedTime": str,
         "Tags": List[TagTypeDef],
     },
-    total=False,
 )
 
 VerifiedAccessLogCloudWatchLogsDestinationTypeDef = TypedDict(
     "VerifiedAccessLogCloudWatchLogsDestinationTypeDef",
     {
         "Enabled": bool,
         "DeliveryStatus": VerifiedAccessLogDeliveryStatusTypeDef,
         "LogGroup": str,
     },
-    total=False,
 )
 
 VerifiedAccessLogKinesisDataFirehoseDestinationTypeDef = TypedDict(
     "VerifiedAccessLogKinesisDataFirehoseDestinationTypeDef",
     {
         "Enabled": bool,
         "DeliveryStatus": VerifiedAccessLogDeliveryStatusTypeDef,
         "DeliveryStream": str,
     },
-    total=False,
 )
 
 VerifiedAccessLogS3DestinationTypeDef = TypedDict(
     "VerifiedAccessLogS3DestinationTypeDef",
     {
         "Enabled": bool,
         "DeliveryStatus": VerifiedAccessLogDeliveryStatusTypeDef,
         "BucketName": str,
         "Prefix": str,
         "BucketOwner": str,
     },
-    total=False,
 )
 
 VerifiedAccessLogOptionsTypeDef = TypedDict(
     "VerifiedAccessLogOptionsTypeDef",
     {
         "S3": VerifiedAccessLogS3DestinationOptionsTypeDef,
         "CloudWatchLogs": VerifiedAccessLogCloudWatchLogsDestinationOptionsTypeDef,
@@ -23911,46 +23465,42 @@
         "Iops": int,
         "Tags": List[TagTypeDef],
         "VolumeType": VolumeTypeType,
         "FastRestored": bool,
         "MultiAttachEnabled": bool,
         "Throughput": int,
     },
-    total=False,
 )
 
 VolumeStatusInfoTypeDef = TypedDict(
     "VolumeStatusInfoTypeDef",
     {
         "Details": List[VolumeStatusDetailsTypeDef],
         "Status": VolumeStatusInfoStatusType,
     },
-    total=False,
 )
 
 VpcCidrBlockAssociationTypeDef = TypedDict(
     "VpcCidrBlockAssociationTypeDef",
     {
         "AssociationId": str,
         "CidrBlock": str,
         "CidrBlockState": VpcCidrBlockStateTypeDef,
     },
-    total=False,
 )
 
 VpcIpv6CidrBlockAssociationTypeDef = TypedDict(
     "VpcIpv6CidrBlockAssociationTypeDef",
     {
         "AssociationId": str,
         "Ipv6CidrBlock": str,
         "Ipv6CidrBlockState": VpcCidrBlockStateTypeDef,
         "NetworkBorderGroup": str,
         "Ipv6Pool": str,
     },
-    total=False,
 )
 
 VpcPeeringConnectionVpcInfoResponseMetadataTypeDef = TypedDict(
     "VpcPeeringConnectionVpcInfoResponseMetadataTypeDef",
     {
         "CidrBlock": str,
         "Ipv6CidrBlockSet": List[Ipv6CidrBlockTypeDef],
@@ -23970,15 +23520,14 @@
         "Ipv6CidrBlockSet": List[Ipv6CidrBlockTypeDef],
         "CidrBlockSet": List[CidrBlockTypeDef],
         "OwnerId": str,
         "PeeringOptions": VpcPeeringConnectionOptionsDescriptionTypeDef,
         "VpcId": str,
         "Region": str,
     },
-    total=False,
 )
 
 DescribeAccountAttributesResultTypeDef = TypedDict(
     "DescribeAccountAttributesResultTypeDef",
     {
         "AccountAttributes": List[AccountAttributeTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
@@ -23993,15 +23542,14 @@
         "VpcEndpointService": AnalysisComponentTypeDef,
         "RuleOptions": List[RuleOptionTypeDef],
         "RuleGroupTypePairs": List[RuleGroupTypePairTypeDef],
         "RuleGroupRuleOptionsPairs": List[RuleGroupRuleOptionsPairTypeDef],
         "ServiceName": str,
         "LoadBalancers": List[AnalysisComponentTypeDef],
     },
-    total=False,
 )
 
 DescribeAddressesAttributeResultTypeDef = TypedDict(
     "DescribeAddressesAttributeResultTypeDef",
     {
         "Addresses": List[AddressAttributeTypeDef],
         "NextToken": str,
@@ -24171,15 +23719,14 @@
         "TimeRanges": List[InstanceEventWindowTimeRangeTypeDef],
         "Name": str,
         "CronExpression": str,
         "AssociationTarget": InstanceEventWindowAssociationTargetTypeDef,
         "State": InstanceEventWindowStateType,
         "Tags": List[TagTypeDef],
     },
-    total=False,
 )
 
 _RequiredDisassociateInstanceEventWindowRequestRequestTypeDef = TypedDict(
     "_RequiredDisassociateInstanceEventWindowRequestRequestTypeDef",
     {
         "InstanceEventWindowId": str,
         "AssociationTarget": InstanceEventWindowDisassociationRequestTypeDef,
@@ -26703,15 +26250,14 @@
         "TransitGatewayRouteTableRoute": TransitGatewayRouteTableRouteTypeDef,
         "TransitGatewayAttachment": AnalysisComponentTypeDef,
         "ComponentAccount": str,
         "ComponentRegion": str,
         "FirewallStatelessRule": FirewallStatelessRuleTypeDef,
         "FirewallStatefulRule": FirewallStatefulRuleTypeDef,
     },
-    total=False,
 )
 
 DescribeClientVpnTargetNetworksResultTypeDef = TypedDict(
     "DescribeClientVpnTargetNetworksResultTypeDef",
     {
         "ClientVpnTargetNetworks": List[TargetNetworkTypeDef],
         "NextToken": str,
@@ -26726,15 +26272,14 @@
         "PropagatingVgws": List[PropagatingVgwTypeDef],
         "RouteTableId": str,
         "Routes": List[RouteTypeDef],
         "Tags": List[TagTypeDef],
         "VpcId": str,
         "OwnerId": str,
     },
-    total=False,
 )
 
 _RequiredGetFlowLogsIntegrationTemplateRequestRequestTypeDef = TypedDict(
     "_RequiredGetFlowLogsIntegrationTemplateRequestRequestTypeDef",
     {
         "FlowLogId": str,
         "ConfigDeliveryS3DestinationArn": str,
@@ -26796,26 +26341,24 @@
         "DeviceIndex": int,
         "NetworkCardIndex": int,
         "InstanceId": str,
         "InstanceOwnerId": str,
         "Status": AttachmentStatusType,
         "EnaSrdSpecification": AttachmentEnaSrdSpecificationTypeDef,
     },
-    total=False,
 )
 
 DhcpOptionsTypeDef = TypedDict(
     "DhcpOptionsTypeDef",
     {
         "DhcpConfigurations": List[DhcpConfigurationTypeDef],
         "DhcpOptionsId": str,
         "OwnerId": str,
         "Tags": List[TagTypeDef],
     },
-    total=False,
 )
 
 DescribeClientVpnAuthorizationRulesResultTypeDef = TypedDict(
     "DescribeClientVpnAuthorizationRulesResultTypeDef",
     {
         "AuthorizationRules": List[AuthorizationRuleTypeDef],
         "NextToken": str,
@@ -26851,15 +26394,14 @@
         "OwnerId": str,
         "AvailabilityZoneId": str,
         "MemberOfServiceLinkedResourceGroup": bool,
         "OutpostArn": str,
         "HostMaintenance": HostMaintenanceType,
         "AssetId": str,
     },
-    total=False,
 )
 
 _RequiredCreateImageRequestInstanceCreateImageTypeDef = TypedDict(
     "_RequiredCreateImageRequestInstanceCreateImageTypeDef",
     {
         "Name": str,
     },
@@ -26956,15 +26498,14 @@
         "Tags": List[TagTypeDef],
         "VirtualizationType": VirtualizationTypeType,
         "BootMode": BootModeValuesType,
         "TpmSupport": Literal["v2.0"],
         "DeprecationTime": str,
         "ImdsSupport": Literal["v2.0"],
     },
-    total=False,
 )
 
 _RequiredRegisterImageRequestRequestTypeDef = TypedDict(
     "_RequiredRegisterImageRequestRequestTypeDef",
     {
         "Name": str,
     },
@@ -27165,15 +26706,14 @@
         "SecurityGroupIds": List[str],
         "VpcId": str,
         "SelfServicePortalUrl": str,
         "ClientConnectOptions": ClientConnectResponseOptionsTypeDef,
         "SessionTimeoutHours": int,
         "ClientLoginBannerOptions": ClientLoginBannerResponseOptionsTypeDef,
     },
-    total=False,
 )
 
 DescribeClientVpnConnectionsResultTypeDef = TypedDict(
     "DescribeClientVpnConnectionsResultTypeDef",
     {
         "Connections": List[ClientVpnConnectionTypeDef],
         "NextToken": str,
@@ -27275,29 +26815,27 @@
         "Phase1DHGroupNumbers": List[Phase1DHGroupNumbersListValueTypeDef],
         "Phase2DHGroupNumbers": List[Phase2DHGroupNumbersListValueTypeDef],
         "IkeVersions": List[IKEVersionsListValueTypeDef],
         "StartupAction": str,
         "LogOptions": VpnTunnelLogOptionsTypeDef,
         "EnableTunnelLifecycleControl": bool,
     },
-    total=False,
 )
 
 NetworkAclTypeDef = TypedDict(
     "NetworkAclTypeDef",
     {
         "Associations": List[NetworkAclAssociationTypeDef],
         "Entries": List[NetworkAclEntryTypeDef],
         "IsDefault": bool,
         "NetworkAclId": str,
         "Tags": List[TagTypeDef],
         "VpcId": str,
         "OwnerId": str,
     },
-    total=False,
 )
 
 LaunchSpecificationTypeDef = TypedDict(
     "LaunchSpecificationTypeDef",
     {
         "UserData": str,
         "SecurityGroups": List[GroupIdentifierTypeDef],
@@ -27311,15 +26849,14 @@
         "KeyName": str,
         "NetworkInterfaces": List[InstanceNetworkInterfaceSpecificationTypeDef],
         "Placement": SpotPlacementTypeDef,
         "RamdiskId": str,
         "SubnetId": str,
         "Monitoring": RunInstancesMonitoringEnabledTypeDef,
     },
-    total=False,
 )
 
 RequestSpotLaunchSpecificationTypeDef = TypedDict(
     "RequestSpotLaunchSpecificationTypeDef",
     {
         "SecurityGroupIds": Sequence[str],
         "SecurityGroups": Sequence[str],
@@ -27448,26 +26985,24 @@
 
 DisableFastSnapshotRestoreErrorItemTypeDef = TypedDict(
     "DisableFastSnapshotRestoreErrorItemTypeDef",
     {
         "SnapshotId": str,
         "FastSnapshotRestoreStateErrors": List[DisableFastSnapshotRestoreStateErrorItemTypeDef],
     },
-    total=False,
 )
 
 ImportInstanceTaskDetailsTypeDef = TypedDict(
     "ImportInstanceTaskDetailsTypeDef",
     {
         "Description": str,
         "InstanceId": str,
         "Platform": Literal["Windows"],
         "Volumes": List[ImportInstanceVolumeDetailItemTypeDef],
     },
-    total=False,
 )
 
 DescribeVpcEndpointConnectionsResultTypeDef = TypedDict(
     "DescribeVpcEndpointConnectionsResultTypeDef",
     {
         "VpcEndpointConnections": List[VpcEndpointConnectionTypeDef],
         "NextToken": str,
@@ -27689,15 +27224,14 @@
 
 EnableFastSnapshotRestoreErrorItemTypeDef = TypedDict(
     "EnableFastSnapshotRestoreErrorItemTypeDef",
     {
         "SnapshotId": str,
         "FastSnapshotRestoreStateErrors": List[EnableFastSnapshotRestoreStateErrorItemTypeDef],
     },
-    total=False,
 )
 
 DescribeFleetHistoryResultTypeDef = TypedDict(
     "DescribeFleetHistoryResultTypeDef",
     {
         "HistoryRecords": List[HistoryRecordEntryTypeDef],
         "LastEvaluatedTime": datetime,
@@ -27759,15 +27293,14 @@
         "DestinationIp": str,
         "Protocol": ProtocolType,
         "DestinationPort": int,
         "Tags": List[TagTypeDef],
         "FilterAtSource": PathFilterTypeDef,
         "FilterAtDestination": PathFilterTypeDef,
     },
-    total=False,
 )
 
 SpotOptionsRequestTypeDef = TypedDict(
     "SpotOptionsRequestTypeDef",
     {
         "AllocationStrategy": SpotAllocationStrategyType,
         "MaintenanceStrategies": FleetSpotMaintenanceStrategiesRequestTypeDef,
@@ -27789,24 +27322,22 @@
         "InstanceInterruptionBehavior": SpotInstanceInterruptionBehaviorType,
         "InstancePoolsToUseCount": int,
         "SingleInstanceType": bool,
         "SingleAvailabilityZone": bool,
         "MinTargetCapacity": int,
         "MaxTotalPrice": str,
     },
-    total=False,
 )
 
 FpgaInfoTypeDef = TypedDict(
     "FpgaInfoTypeDef",
     {
         "Fpgas": List[FpgaDeviceInfoTypeDef],
         "TotalFpgaMemoryInMiB": int,
     },
-    total=False,
 )
 
 DescribeFpgaImageAttributeResultTypeDef = TypedDict(
     "DescribeFpgaImageAttributeResultTypeDef",
     {
         "FpgaImageAttribute": FpgaImageAttributeTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
@@ -27832,15 +27363,14 @@
 
 GpuInfoTypeDef = TypedDict(
     "GpuInfoTypeDef",
     {
         "Gpus": List[GpuDeviceInfoTypeDef],
         "TotalGpuMemoryInMiB": int,
     },
-    total=False,
 )
 
 AssociateIamInstanceProfileResultTypeDef = TypedDict(
     "AssociateIamInstanceProfileResultTypeDef",
     {
         "IamInstanceProfileAssociation": IamInstanceProfileAssociationTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
@@ -28214,15 +27744,14 @@
         "Status": NetworkInterfaceStatusType,
         "SubnetId": str,
         "VpcId": str,
         "InterfaceType": str,
         "Ipv4Prefixes": List[InstanceIpv4PrefixTypeDef],
         "Ipv6Prefixes": List[InstanceIpv6PrefixTypeDef],
     },
-    total=False,
 )
 
 FleetLaunchTemplateOverridesRequestTypeDef = TypedDict(
     "FleetLaunchTemplateOverridesRequestTypeDef",
     {
         "InstanceType": InstanceTypeType,
         "MaxPrice": str,
@@ -28303,29 +27832,27 @@
         "AvailabilityZone": str,
         "WeightedCapacity": float,
         "Priority": float,
         "Placement": PlacementResponseTypeDef,
         "InstanceRequirements": InstanceRequirementsTypeDef,
         "ImageId": str,
     },
-    total=False,
 )
 
 LaunchTemplateOverridesTypeDef = TypedDict(
     "LaunchTemplateOverridesTypeDef",
     {
         "InstanceType": InstanceTypeType,
         "SpotPrice": str,
         "SubnetId": str,
         "AvailabilityZone": str,
         "WeightedCapacity": float,
         "Priority": float,
         "InstanceRequirements": InstanceRequirementsTypeDef,
     },
-    total=False,
 )
 
 SpotFleetLaunchSpecificationTypeDef = TypedDict(
     "SpotFleetLaunchSpecificationTypeDef",
     {
         "SecurityGroups": List[GroupIdentifierTypeDef],
         "AddressingType": str,
@@ -28343,15 +27870,14 @@
         "SpotPrice": str,
         "SubnetId": str,
         "UserData": str,
         "WeightedCapacity": float,
         "TagSpecifications": List[SpotFleetTagSpecificationTypeDef],
         "InstanceRequirements": InstanceRequirementsTypeDef,
     },
-    total=False,
 )
 
 StartInstancesResultTypeDef = TypedDict(
     "StartInstancesResultTypeDef",
     {
         "StartingInstances": List[InstanceStateChangeTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
@@ -28381,15 +27907,14 @@
         "OutpostArn": str,
         "Events": List[InstanceStatusEventTypeDef],
         "InstanceId": str,
         "InstanceState": InstanceStateTypeDef,
         "InstanceStatus": InstanceStatusSummaryTypeDef,
         "SystemStatus": InstanceStatusSummaryTypeDef,
     },
-    total=False,
 )
 
 _RequiredAuthorizeSecurityGroupEgressRequestRequestTypeDef = TypedDict(
     "_RequiredAuthorizeSecurityGroupEgressRequestRequestTypeDef",
     {
         "GroupId": str,
     },
@@ -28572,15 +28097,14 @@
         "IpPermissions": List[IpPermissionTypeDef],
         "OwnerId": str,
         "GroupId": str,
         "IpPermissionsEgress": List[IpPermissionTypeDef],
         "Tags": List[TagTypeDef],
         "VpcId": str,
     },
-    total=False,
 )
 
 UpdateSecurityGroupRuleDescriptionsEgressRequestRequestTypeDef = TypedDict(
     "UpdateSecurityGroupRuleDescriptionsEgressRequestRequestTypeDef",
     {
         "DryRun": bool,
         "GroupId": str,
@@ -28609,15 +28133,14 @@
         "Description": str,
         "GroupId": str,
         "GroupName": str,
         "StaleIpPermissions": List[StaleIpPermissionTypeDef],
         "StaleIpPermissionsEgress": List[StaleIpPermissionTypeDef],
         "VpcId": str,
     },
-    total=False,
 )
 
 GetIpamDiscoveredAccountsResultTypeDef = TypedDict(
     "GetIpamDiscoveredAccountsResultTypeDef",
     {
         "IpamDiscoveredAccounts": List[IpamDiscoveredAccountTypeDef],
         "NextToken": str,
@@ -28861,15 +28384,14 @@
         "MetadataOptions": LaunchTemplateInstanceMetadataOptionsTypeDef,
         "EnclaveOptions": LaunchTemplateEnclaveOptionsTypeDef,
         "InstanceRequirements": InstanceRequirementsTypeDef,
         "PrivateDnsNameOptions": LaunchTemplatePrivateDnsNameOptionsTypeDef,
         "MaintenanceOptions": LaunchTemplateInstanceMaintenanceOptionsTypeDef,
         "DisableApiStop": bool,
     },
-    total=False,
 )
 
 _RequiredModifyFpgaImageAttributeRequestRequestTypeDef = TypedDict(
     "_RequiredModifyFpgaImageAttributeRequestRequestTypeDef",
     {
         "FpgaImageId": str,
     },
@@ -28905,15 +28427,14 @@
         "ModificationResults": List[ReservedInstancesModificationResultTypeDef],
         "ReservedInstancesIds": List[ReservedInstancesIdTypeDef],
         "ReservedInstancesModificationId": str,
         "Status": str,
         "StatusMessage": str,
         "UpdateDate": datetime,
     },
-    total=False,
 )
 
 CreateNatGatewayResultTypeDef = TypedDict(
     "CreateNatGatewayResultTypeDef",
     {
         "ClientToken": str,
         "NatGateway": NatGatewayTypeDef,
@@ -29022,15 +28543,14 @@
 AccessScopePathTypeDef = TypedDict(
     "AccessScopePathTypeDef",
     {
         "Source": PathStatementTypeDef,
         "Destination": PathStatementTypeDef,
         "ThroughResources": List[ThroughResourcesStatementTypeDef],
     },
-    total=False,
 )
 
 CancelReservedInstancesListingResultTypeDef = TypedDict(
     "CancelReservedInstancesListingResultTypeDef",
     {
         "ReservedInstancesListings": List[ReservedInstancesListingTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
@@ -29134,15 +28654,14 @@
         "InstanceId": str,
         "Progress": str,
         "StartTime": datetime,
         "State": BundleTaskStateType,
         "Storage": StorageTypeDef,
         "UpdateTime": datetime,
     },
-    total=False,
 )
 
 DescribeScheduledInstanceAvailabilityResultTypeDef = TypedDict(
     "DescribeScheduledInstanceAvailabilityResultTypeDef",
     {
         "NextToken": str,
         "ScheduledInstanceAvailabilitySet": List[ScheduledInstanceAvailabilityTypeDef],
@@ -29306,15 +28825,14 @@
         "Status": str,
         "StatusMessage": str,
         "Tags": List[TagTypeDef],
         "LicenseSpecifications": List[ImportImageLicenseConfigurationResponseTypeDef],
         "UsageOperation": str,
         "BootMode": BootModeValuesType,
     },
-    total=False,
 )
 
 ImportSnapshotResultTypeDef = TypedDict(
     "ImportSnapshotResultTypeDef",
     {
         "Description": str,
         "ImportTaskId": str,
@@ -29328,15 +28846,14 @@
     "ImportSnapshotTaskTypeDef",
     {
         "Description": str,
         "ImportTaskId": str,
         "SnapshotTaskDetail": SnapshotTaskDetailTypeDef,
         "Tags": List[TagTypeDef],
     },
-    total=False,
 )
 
 CreateSpotDatafeedSubscriptionResultTypeDef = TypedDict(
     "CreateSpotDatafeedSubscriptionResultTypeDef",
     {
         "SpotDatafeedSubscription": SpotDatafeedSubscriptionTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
@@ -29431,15 +28948,14 @@
         "Tags": List[TagTypeDef],
         "SubnetArn": str,
         "OutpostArn": str,
         "EnableDns64": bool,
         "Ipv6Native": bool,
         "PrivateDnsNameOptionsOnLaunch": PrivateDnsNameOptionsOnLaunchTypeDef,
     },
-    total=False,
 )
 
 GetReservedInstancesExchangeQuoteResultTypeDef = TypedDict(
     "GetReservedInstancesExchangeQuoteResultTypeDef",
     {
         "CurrencyCode": str,
         "IsValidExchange": bool,
@@ -29456,15 +28972,14 @@
 
 LoadBalancersConfigTypeDef = TypedDict(
     "LoadBalancersConfigTypeDef",
     {
         "ClassicLoadBalancersConfig": ClassicLoadBalancersConfigTypeDef,
         "TargetGroupsConfig": TargetGroupsConfigTypeDef,
     },
-    total=False,
 )
 
 CreateTrafficMirrorFilterRuleResultTypeDef = TypedDict(
     "CreateTrafficMirrorFilterRuleResultTypeDef",
     {
         "TrafficMirrorFilterRule": TrafficMirrorFilterRuleTypeDef,
         "ClientToken": str,
@@ -29486,15 +29001,14 @@
         "TrafficMirrorFilterId": str,
         "IngressFilterRules": List[TrafficMirrorFilterRuleTypeDef],
         "EgressFilterRules": List[TrafficMirrorFilterRuleTypeDef],
         "NetworkServices": List[Literal["amazon-dns"]],
         "Description": str,
         "Tags": List[TagTypeDef],
     },
-    total=False,
 )
 
 DescribeTransitGatewayAttachmentsResultTypeDef = TypedDict(
     "DescribeTransitGatewayAttachmentsResultTypeDef",
     {
         "TransitGatewayAttachments": List[TransitGatewayAttachmentTypeDef],
         "NextToken": str,
@@ -29508,15 +29022,14 @@
         "TransitGatewayAttachmentId": str,
         "TransitGatewayConnectPeerId": str,
         "State": TransitGatewayConnectPeerStateType,
         "CreationTime": datetime,
         "ConnectPeerConfiguration": TransitGatewayConnectPeerConfigurationTypeDef,
         "Tags": List[TagTypeDef],
     },
-    total=False,
 )
 
 CreateTransitGatewayConnectResultTypeDef = TypedDict(
     "CreateTransitGatewayConnectResultTypeDef",
     {
         "TransitGatewayConnect": TransitGatewayConnectTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
@@ -29642,15 +29155,14 @@
 TransitGatewayPolicyTableEntryTypeDef = TypedDict(
     "TransitGatewayPolicyTableEntryTypeDef",
     {
         "PolicyRuleNumber": str,
         "PolicyRule": TransitGatewayPolicyRuleTypeDef,
         "TargetRouteTableId": str,
     },
-    total=False,
 )
 
 CreateTransitGatewayPrefixListReferenceResultTypeDef = TypedDict(
     "CreateTransitGatewayPrefixListReferenceResultTypeDef",
     {
         "TransitGatewayPrefixListReference": TransitGatewayPrefixListReferenceTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
@@ -29951,15 +29463,14 @@
     {
         "S3": VerifiedAccessLogS3DestinationTypeDef,
         "CloudWatchLogs": VerifiedAccessLogCloudWatchLogsDestinationTypeDef,
         "KinesisDataFirehose": VerifiedAccessLogKinesisDataFirehoseDestinationTypeDef,
         "LogVersion": str,
         "IncludeTrustContext": bool,
     },
-    total=False,
 )
 
 _RequiredModifyVerifiedAccessInstanceLoggingConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredModifyVerifiedAccessInstanceLoggingConfigurationRequestRequestTypeDef",
     {
         "VerifiedAccessInstanceId": str,
         "AccessLogs": VerifiedAccessLogOptionsTypeDef,
@@ -29996,15 +29507,14 @@
         "AvailabilityZone": str,
         "OutpostArn": str,
         "Events": List[VolumeStatusEventTypeDef],
         "VolumeId": str,
         "VolumeStatus": VolumeStatusInfoTypeDef,
         "AttachmentStatuses": List[VolumeStatusAttachmentStatusTypeDef],
     },
-    total=False,
 )
 
 AssociateVpcCidrBlockResultTypeDef = TypedDict(
     "AssociateVpcCidrBlockResultTypeDef",
     {
         "Ipv6CidrBlockAssociation": VpcIpv6CidrBlockAssociationTypeDef,
         "CidrBlockAssociation": VpcCidrBlockAssociationTypeDef,
@@ -30033,28 +29543,26 @@
         "OwnerId": str,
         "InstanceTenancy": TenancyType,
         "Ipv6CidrBlockAssociationSet": List[VpcIpv6CidrBlockAssociationTypeDef],
         "CidrBlockAssociationSet": List[VpcCidrBlockAssociationTypeDef],
         "IsDefault": bool,
         "Tags": List[TagTypeDef],
     },
-    total=False,
 )
 
 VpcPeeringConnectionTypeDef = TypedDict(
     "VpcPeeringConnectionTypeDef",
     {
         "AccepterVpcInfo": VpcPeeringConnectionVpcInfoTypeDef,
         "ExpirationTime": datetime,
         "RequesterVpcInfo": VpcPeeringConnectionVpcInfoTypeDef,
         "Status": VpcPeeringConnectionStateReasonTypeDef,
         "Tags": List[TagTypeDef],
         "VpcPeeringConnectionId": str,
     },
-    total=False,
 )
 
 AssociateInstanceEventWindowResultTypeDef = TypedDict(
     "AssociateInstanceEventWindowResultTypeDef",
     {
         "InstanceEventWindow": InstanceEventWindowTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
@@ -30114,15 +29622,14 @@
         "TransitGatewayRouteTableRoute": TransitGatewayRouteTableRouteTypeDef,
         "Explanations": List[ExplanationTypeDef],
         "ElasticLoadBalancerListener": AnalysisComponentTypeDef,
         "FirewallStatelessRule": FirewallStatelessRuleTypeDef,
         "FirewallStatefulRule": FirewallStatefulRuleTypeDef,
         "ServiceName": str,
     },
-    total=False,
 )
 
 CreateRouteTableResultTypeDef = TypedDict(
     "CreateRouteTableResultTypeDef",
     {
         "RouteTable": RouteTableTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
@@ -30176,15 +29683,14 @@
         "SubnetId": str,
         "TagSet": List[TagTypeDef],
         "VpcId": str,
         "DenyAllIgwTraffic": bool,
         "Ipv6Native": bool,
         "Ipv6Address": str,
     },
-    total=False,
 )
 
 CreateDhcpOptionsResultTypeDef = TypedDict(
     "CreateDhcpOptionsResultTypeDef",
     {
         "DhcpOptions": DhcpOptionsTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
@@ -30277,15 +29783,14 @@
         "LocalIpv6NetworkCidr": str,
         "RemoteIpv6NetworkCidr": str,
         "OutsideIpAddressType": str,
         "TransportTransitGatewayAttachmentId": str,
         "TunnelInsideIpVersion": TunnelInsideIpVersionType,
         "TunnelOptions": List[TunnelOptionTypeDef],
     },
-    total=False,
 )
 
 CreateNetworkAclResultTypeDef = TypedDict(
     "CreateNetworkAclResultTypeDef",
     {
         "NetworkAcl": NetworkAclTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
@@ -30320,15 +29825,14 @@
         "Status": SpotInstanceStatusTypeDef,
         "Tags": List[TagTypeDef],
         "Type": SpotInstanceTypeType,
         "ValidFrom": datetime,
         "ValidUntil": datetime,
         "InstanceInterruptionBehavior": InstanceInterruptionBehaviorType,
     },
-    total=False,
 )
 
 RequestSpotInstancesRequestRequestTypeDef = TypedDict(
     "RequestSpotInstancesRequestRequestTypeDef",
     {
         "AvailabilityZoneGroup": str,
         "BlockDurationMinutes": int,
@@ -30363,15 +29867,14 @@
         "ExpirationTime": str,
         "ImportInstance": ImportInstanceTaskDetailsTypeDef,
         "ImportVolume": ImportVolumeTaskDetailsTypeDef,
         "State": ConversionTaskStateType,
         "StatusMessage": str,
         "Tags": List[TagTypeDef],
     },
-    total=False,
 )
 
 EnableFastSnapshotRestoresResultTypeDef = TypedDict(
     "EnableFastSnapshotRestoresResultTypeDef",
     {
         "Successful": List[EnableFastSnapshotRestoreSuccessItemTypeDef],
         "Unsuccessful": List[EnableFastSnapshotRestoreErrorItemTypeDef],
@@ -30421,15 +29924,14 @@
         "HibernationSupported": bool,
         "BurstablePerformanceSupported": bool,
         "DedicatedHostsSupported": bool,
         "AutoRecoverySupported": bool,
         "SupportedBootModes": List[BootModeTypeType],
         "NitroEnclavesSupport": NitroEnclavesSupportType,
     },
-    total=False,
 )
 
 InstanceTypeDef = TypedDict(
     "InstanceTypeDef",
     {
         "AmiLaunchIndex": int,
         "ImageId": str,
@@ -30487,15 +29989,14 @@
         "UsageOperationUpdateTime": datetime,
         "PrivateDnsNameOptions": PrivateDnsNameOptionsResponseTypeDef,
         "Ipv6Address": str,
         "TpmSupport": str,
         "MaintenanceOptions": InstanceMaintenanceOptionsTypeDef,
         "CurrentInstanceBootMode": InstanceBootModeValuesType,
     },
-    total=False,
 )
 
 FleetLaunchTemplateConfigRequestTypeDef = TypedDict(
     "FleetLaunchTemplateConfigRequestTypeDef",
     {
         "LaunchTemplateSpecification": FleetLaunchTemplateSpecificationRequestTypeDef,
         "Overrides": Sequence[FleetLaunchTemplateOverridesRequestTypeDef],
@@ -30558,33 +30059,30 @@
 
 FleetLaunchTemplateConfigTypeDef = TypedDict(
     "FleetLaunchTemplateConfigTypeDef",
     {
         "LaunchTemplateSpecification": FleetLaunchTemplateSpecificationTypeDef,
         "Overrides": List[FleetLaunchTemplateOverridesTypeDef],
     },
-    total=False,
 )
 
 LaunchTemplateAndOverridesResponseTypeDef = TypedDict(
     "LaunchTemplateAndOverridesResponseTypeDef",
     {
         "LaunchTemplateSpecification": FleetLaunchTemplateSpecificationTypeDef,
         "Overrides": FleetLaunchTemplateOverridesTypeDef,
     },
-    total=False,
 )
 
 LaunchTemplateConfigTypeDef = TypedDict(
     "LaunchTemplateConfigTypeDef",
     {
         "LaunchTemplateSpecification": FleetLaunchTemplateSpecificationTypeDef,
         "Overrides": List[LaunchTemplateOverridesTypeDef],
     },
-    total=False,
 )
 
 DescribeInstanceStatusResultTypeDef = TypedDict(
     "DescribeInstanceStatusResultTypeDef",
     {
         "InstanceStatuses": List[InstanceStatusTypeDef],
         "NextToken": str,
@@ -30676,15 +30174,14 @@
         "VersionNumber": int,
         "VersionDescription": str,
         "CreateTime": datetime,
         "CreatedBy": str,
         "DefaultVersion": bool,
         "LaunchTemplateData": ResponseLaunchTemplateDataTypeDef,
     },
-    total=False,
 )
 
 DescribeReservedInstancesModificationsResultTypeDef = TypedDict(
     "DescribeReservedInstancesModificationsResultTypeDef",
     {
         "NextToken": str,
         "ReservedInstancesModifications": List[ReservedInstancesModificationTypeDef],
@@ -30718,15 +30215,14 @@
 NetworkInsightsAccessScopeContentTypeDef = TypedDict(
     "NetworkInsightsAccessScopeContentTypeDef",
     {
         "NetworkInsightsAccessScopeId": str,
         "MatchPaths": List[AccessScopePathTypeDef],
         "ExcludePaths": List[AccessScopePathTypeDef],
     },
-    total=False,
 )
 
 BundleInstanceResultTypeDef = TypedDict(
     "BundleInstanceResultTypeDef",
     {
         "BundleTask": BundleTaskTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
@@ -30876,15 +30372,14 @@
 
 VerifiedAccessInstanceLoggingConfigurationTypeDef = TypedDict(
     "VerifiedAccessInstanceLoggingConfigurationTypeDef",
     {
         "VerifiedAccessInstanceId": str,
         "AccessLogs": VerifiedAccessLogsTypeDef,
     },
-    total=False,
 )
 
 DescribeVolumeStatusResultTypeDef = TypedDict(
     "DescribeVolumeStatusResultTypeDef",
     {
         "NextToken": str,
         "VolumeStatuses": List[VolumeStatusItemTypeDef],
@@ -30946,15 +30441,14 @@
     "AccessScopeAnalysisFindingTypeDef",
     {
         "NetworkInsightsAccessScopeAnalysisId": str,
         "NetworkInsightsAccessScopeId": str,
         "FindingId": str,
         "FindingComponents": List[PathComponentTypeDef],
     },
-    total=False,
 )
 
 NetworkInsightsAnalysisTypeDef = TypedDict(
     "NetworkInsightsAnalysisTypeDef",
     {
         "NetworkInsightsAnalysisId": str,
         "NetworkInsightsAnalysisArn": str,
@@ -30969,15 +30463,14 @@
         "ForwardPathComponents": List[PathComponentTypeDef],
         "ReturnPathComponents": List[PathComponentTypeDef],
         "Explanations": List[ExplanationTypeDef],
         "AlternatePathHints": List[AlternatePathHintTypeDef],
         "SuggestedAccounts": List[str],
         "Tags": List[TagTypeDef],
     },
-    total=False,
 )
 
 CreateNetworkInterfaceResultTypeDef = TypedDict(
     "CreateNetworkInterfaceResultTypeDef",
     {
         "NetworkInterface": NetworkInterfaceTypeDef,
         "ClientToken": str,
@@ -31034,15 +30527,14 @@
         "CoreNetworkAttachmentArn": str,
         "GatewayAssociationState": GatewayAssociationStateType,
         "Options": VpnConnectionOptionsTypeDef,
         "Routes": List[VpnStaticRouteTypeDef],
         "Tags": List[TagTypeDef],
         "VgwTelemetry": List[VgwTelemetryTypeDef],
     },
-    total=False,
 )
 
 DescribeSpotInstanceRequestsResultTypeDef = TypedDict(
     "DescribeSpotInstanceRequestsResultTypeDef",
     {
         "SpotInstanceRequests": List[SpotInstanceRequestTypeDef],
         "NextToken": str,
@@ -31108,15 +30600,14 @@
     {
         "Groups": List[GroupIdentifierTypeDef],
         "Instances": List[InstanceTypeDef],
         "OwnerId": str,
         "RequesterId": str,
         "ReservationId": str,
     },
-    total=False,
 )
 
 _RequiredCreateFleetRequestRequestTypeDef = TypedDict(
     "_RequiredCreateFleetRequestRequestTypeDef",
     {
         "LaunchTemplateConfigs": Sequence[FleetLaunchTemplateConfigRequestTypeDef],
         "TargetCapacitySpecification": TargetCapacitySpecificationRequestTypeDef,
@@ -31173,50 +30664,46 @@
     "CreateFleetErrorTypeDef",
     {
         "LaunchTemplateAndOverrides": LaunchTemplateAndOverridesResponseTypeDef,
         "Lifecycle": InstanceLifecycleType,
         "ErrorCode": str,
         "ErrorMessage": str,
     },
-    total=False,
 )
 
 CreateFleetInstanceTypeDef = TypedDict(
     "CreateFleetInstanceTypeDef",
     {
         "LaunchTemplateAndOverrides": LaunchTemplateAndOverridesResponseTypeDef,
         "Lifecycle": InstanceLifecycleType,
         "InstanceIds": List[str],
         "InstanceType": InstanceTypeType,
         "Platform": Literal["Windows"],
     },
-    total=False,
 )
 
 DescribeFleetErrorTypeDef = TypedDict(
     "DescribeFleetErrorTypeDef",
     {
         "LaunchTemplateAndOverrides": LaunchTemplateAndOverridesResponseTypeDef,
         "Lifecycle": InstanceLifecycleType,
         "ErrorCode": str,
         "ErrorMessage": str,
     },
-    total=False,
 )
 
 DescribeFleetsInstancesTypeDef = TypedDict(
     "DescribeFleetsInstancesTypeDef",
     {
         "LaunchTemplateAndOverrides": LaunchTemplateAndOverridesResponseTypeDef,
         "Lifecycle": InstanceLifecycleType,
         "InstanceIds": List[str],
         "InstanceType": InstanceTypeType,
         "Platform": Literal["Windows"],
     },
-    total=False,
 )
 
 _RequiredModifySpotFleetRequestRequestRequestTypeDef = TypedDict(
     "_RequiredModifySpotFleetRequestRequestRequestTypeDef",
     {
         "SpotFleetRequestId": str,
     },
@@ -31235,34 +30722,29 @@
 
 class ModifySpotFleetRequestRequestRequestTypeDef(
     _RequiredModifySpotFleetRequestRequestRequestTypeDef,
     _OptionalModifySpotFleetRequestRequestRequestTypeDef,
 ):
     pass
 
-_RequiredSpotFleetRequestConfigDataTypeDef = TypedDict(
-    "_RequiredSpotFleetRequestConfigDataTypeDef",
-    {
-        "IamFleetRole": str,
-        "TargetCapacity": int,
-    },
-)
-_OptionalSpotFleetRequestConfigDataTypeDef = TypedDict(
-    "_OptionalSpotFleetRequestConfigDataTypeDef",
+SpotFleetRequestConfigDataTypeDef = TypedDict(
+    "SpotFleetRequestConfigDataTypeDef",
     {
         "AllocationStrategy": AllocationStrategyType,
         "OnDemandAllocationStrategy": OnDemandAllocationStrategyType,
         "SpotMaintenanceStrategies": SpotMaintenanceStrategiesTypeDef,
         "ClientToken": str,
         "ExcessCapacityTerminationPolicy": ExcessCapacityTerminationPolicyType,
         "FulfilledCapacity": float,
         "OnDemandFulfilledCapacity": float,
+        "IamFleetRole": str,
         "LaunchSpecifications": List[SpotFleetLaunchSpecificationTypeDef],
         "LaunchTemplateConfigs": List[LaunchTemplateConfigTypeDef],
         "SpotPrice": str,
+        "TargetCapacity": int,
         "OnDemandTargetCapacity": int,
         "OnDemandMaxTotalPrice": str,
         "SpotMaxTotalPrice": str,
         "TerminateInstancesWithExpiration": bool,
         "Type": FleetTypeType,
         "ValidFrom": datetime,
         "ValidUntil": datetime,
@@ -31270,22 +30752,16 @@
         "InstanceInterruptionBehavior": InstanceInterruptionBehaviorType,
         "LoadBalancersConfig": LoadBalancersConfigTypeDef,
         "InstancePoolsToUseCount": int,
         "Context": str,
         "TargetCapacityUnitType": TargetCapacityUnitTypeType,
         "TagSpecifications": List[TagSpecificationTypeDef],
     },
-    total=False,
 )
 
-class SpotFleetRequestConfigDataTypeDef(
-    _RequiredSpotFleetRequestConfigDataTypeDef, _OptionalSpotFleetRequestConfigDataTypeDef
-):
-    pass
-
 CreateLaunchTemplateVersionResultTypeDef = TypedDict(
     "CreateLaunchTemplateVersionResultTypeDef",
     {
         "LaunchTemplateVersion": LaunchTemplateVersionTypeDef,
         "Warning": ValidationWarningTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -31450,15 +30926,14 @@
         "SpotOptions": SpotOptionsTypeDef,
         "OnDemandOptions": OnDemandOptionsTypeDef,
         "Tags": List[TagTypeDef],
         "Errors": List[DescribeFleetErrorTypeDef],
         "Instances": List[DescribeFleetsInstancesTypeDef],
         "Context": str,
     },
-    total=False,
 )
 
 _RequiredRequestSpotFleetRequestRequestTypeDef = TypedDict(
     "_RequiredRequestSpotFleetRequestRequestTypeDef",
     {
         "SpotFleetRequestConfig": SpotFleetRequestConfigDataTypeDef,
     },
@@ -31482,15 +30957,14 @@
         "ActivityStatus": ActivityStatusType,
         "CreateTime": datetime,
         "SpotFleetRequestConfig": SpotFleetRequestConfigDataTypeDef,
         "SpotFleetRequestId": str,
         "SpotFleetRequestState": BatchStateType,
         "Tags": List[TagTypeDef],
     },
-    total=False,
 )
 
 DescribeFleetsResultTypeDef = TypedDict(
     "DescribeFleetsResultTypeDef",
     {
         "NextToken": str,
         "Fleets": List[FleetDataTypeDef],
```

### Comparing `mypy-boto3-ec2-1.28.0/mypy_boto3_ec2/waiter.py` & `mypy-boto3-ec2-1.28.3/mypy_boto3_ec2/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ec2-1.28.0/mypy_boto3_ec2/waiter.pyi` & `mypy-boto3-ec2-1.28.3/mypy_boto3_ec2/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ec2-1.28.0/mypy_boto3_ec2.egg-info/PKG-INFO` & `mypy-boto3-ec2-1.28.3/mypy_boto3_ec2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-ec2
-Version: 1.28.0
-Summary: Type annotations for boto3.EC2 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.3
+Summary: Type annotations for boto3.EC2 1.28.3 service generated with mypy-boto3-builder 7.14.6
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ec2.svg?color=blue)](https://pypi.org/project/mypy-boto3-ec2)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-ec2?color=blue)](https://pypistats.org/packages/mypy-boto3-ec2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.EC2 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2)
+[boto3.EC2 1.28.3](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2)
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
 [mypy-boto3-ec2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-ec2-1.28.0/mypy_boto3_ec2.egg-info/SOURCES.txt` & `mypy-boto3-ec2-1.28.3/mypy_boto3_ec2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ec2-1.28.0/setup.py` & `mypy-boto3-ec2-1.28.3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-ec2",
-    version="1.28.0",
+    version="1.28.3",
     packages=["mypy_boto3_ec2"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.EC2 1.28.0 service generated with mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.EC2 1.28.3 service generated with mypy-boto3-builder 7.14.6"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

