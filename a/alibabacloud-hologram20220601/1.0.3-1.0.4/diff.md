# Comparing `tmp/alibabacloud_hologram20220601-1.0.3.tar.gz` & `tmp/alibabacloud_hologram20220601-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_hologram20220601-1.0.3.tar", last modified: Wed May 17 03:56:22 2023, max compression
+gzip compressed data, was "dist/alibabacloud_hologram20220601-1.0.4.tar", last modified: Thu Jul 13 10:42:31 2023, max compression
```

## Comparing `alibabacloud_hologram20220601-1.0.3.tar` & `alibabacloud_hologram20220601-1.0.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:56:22.000000 alibabacloud_hologram20220601-1.0.3/
--rw-r--r--   0 root         (0) root         (0)      138 2023-05-17 03:56:22.000000 alibabacloud_hologram20220601-1.0.3/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2023-05-17 03:56:22.000000 alibabacloud_hologram20220601-1.0.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-05-17 03:56:22.000000 alibabacloud_hologram20220601-1.0.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2358 2023-05-17 03:56:22.000000 alibabacloud_hologram20220601-1.0.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1037 2023-05-17 03:56:22.000000 alibabacloud_hologram20220601-1.0.3/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1122 2023-05-17 03:56:22.000000 alibabacloud_hologram20220601-1.0.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:56:22.000000 alibabacloud_hologram20220601-1.0.3/alibabacloud_hologram20220601/
--rw-r--r--   0 root         (0) root         (0)       21 2023-05-17 03:56:22.000000 alibabacloud_hologram20220601-1.0.3/alibabacloud_hologram20220601/__init__.py
--rw-r--r--   0 root         (0) root         (0)    21136 2023-05-17 03:56:22.000000 alibabacloud_hologram20220601-1.0.3/alibabacloud_hologram20220601/client.py
--rw-r--r--   0 root         (0) root         (0)    47585 2023-05-17 03:56:22.000000 alibabacloud_hologram20220601-1.0.3/alibabacloud_hologram20220601/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:56:22.000000 alibabacloud_hologram20220601-1.0.3/alibabacloud_hologram20220601.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2358 2023-05-17 03:56:22.000000 alibabacloud_hologram20220601-1.0.3/alibabacloud_hologram20220601.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      460 2023-05-17 03:56:22.000000 alibabacloud_hologram20220601-1.0.3/alibabacloud_hologram20220601.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-17 03:56:22.000000 alibabacloud_hologram20220601-1.0.3/alibabacloud_hologram20220601.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      156 2023-05-17 03:56:22.000000 alibabacloud_hologram20220601-1.0.3/alibabacloud_hologram20220601.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       30 2023-05-17 03:56:22.000000 alibabacloud_hologram20220601-1.0.3/alibabacloud_hologram20220601.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-05-17 03:56:22.000000 alibabacloud_hologram20220601-1.0.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2635 2023-05-17 03:56:22.000000 alibabacloud_hologram20220601-1.0.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 10:42:31.000000 alibabacloud_hologram20220601-1.0.4/
+-rw-r--r--   0 root         (0) root         (0)      184 2023-07-13 10:42:31.000000 alibabacloud_hologram20220601-1.0.4/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2023-07-13 10:42:31.000000 alibabacloud_hologram20220601-1.0.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-07-13 10:42:31.000000 alibabacloud_hologram20220601-1.0.4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2358 2023-07-13 10:42:31.000000 alibabacloud_hologram20220601-1.0.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1037 2023-07-13 10:42:31.000000 alibabacloud_hologram20220601-1.0.4/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1122 2023-07-13 10:42:31.000000 alibabacloud_hologram20220601-1.0.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 10:42:31.000000 alibabacloud_hologram20220601-1.0.4/alibabacloud_hologram20220601/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-07-13 10:42:31.000000 alibabacloud_hologram20220601-1.0.4/alibabacloud_hologram20220601/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    37548 2023-07-13 10:42:31.000000 alibabacloud_hologram20220601-1.0.4/alibabacloud_hologram20220601/client.py
+-rw-r--r--   0 root         (0) root         (0)    89042 2023-07-13 10:42:31.000000 alibabacloud_hologram20220601-1.0.4/alibabacloud_hologram20220601/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 10:42:31.000000 alibabacloud_hologram20220601-1.0.4/alibabacloud_hologram20220601.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2358 2023-07-13 10:42:31.000000 alibabacloud_hologram20220601-1.0.4/alibabacloud_hologram20220601.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      460 2023-07-13 10:42:31.000000 alibabacloud_hologram20220601-1.0.4/alibabacloud_hologram20220601.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-13 10:42:31.000000 alibabacloud_hologram20220601-1.0.4/alibabacloud_hologram20220601.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      156 2023-07-13 10:42:31.000000 alibabacloud_hologram20220601-1.0.4/alibabacloud_hologram20220601.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       30 2023-07-13 10:42:31.000000 alibabacloud_hologram20220601-1.0.4/alibabacloud_hologram20220601.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-07-13 10:42:31.000000 alibabacloud_hologram20220601-1.0.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2635 2023-07-13 10:42:31.000000 alibabacloud_hologram20220601-1.0.4/setup.py
```

### Comparing `alibabacloud_hologram20220601-1.0.3/LICENSE` & `alibabacloud_hologram20220601-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_hologram20220601-1.0.3/PKG-INFO` & `alibabacloud_hologram20220601-1.0.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_hologram20220601
-Version: 1.0.3
+Version: 1.0.4
 Summary: Alibaba Cloud Hologres (20220601) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_hologram20220601-1.0.3/README-CN.md` & `alibabacloud_hologram20220601-1.0.4/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_hologram20220601-1.0.3/README.md` & `alibabacloud_hologram20220601-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_hologram20220601-1.0.3/alibabacloud_hologram20220601.egg-info/PKG-INFO` & `alibabacloud_hologram20220601-1.0.4/alibabacloud_hologram20220601.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-hologram20220601
-Version: 1.0.3
+Version: 1.0.4
 Summary: Alibaba Cloud Hologres (20220601) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_hologram20220601-1.0.3/setup.py` & `alibabacloud_hologram20220601-1.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,28 +20,28 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_hologram20220601.
 
-Created on 17/05/2023
+Created on 13/07/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_hologram20220601"
 NAME = "alibabacloud_hologram20220601" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Hologres (20220601) SDK Library for Python"
 AUTHOR = "Alibaba Cloud SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/aliyun/alibabacloud-python-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
-    "alibabacloud_tea_util>=0.3.8, <1.0.0",
+    "alibabacloud_tea_util>=0.3.9, <1.0.0",
     "alibabacloud_tea_openapi>=0.3.6, <1.0.0",
     "alibabacloud_openapi_util>=0.2.1, <1.0.0",
     "alibabacloud_endpoint_util>=0.0.3, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
 if os.path.exists('./README.md'):
```

