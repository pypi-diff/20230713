# Comparing `tmp/alibabacloud_ehpc20180412-1.14.8.tar.gz` & `tmp/alibabacloud_ehpc20180412-1.14.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_ehpc20180412-1.14.8.tar", last modified: Mon Oct 25 03:23:19 2021, max compression
+gzip compressed data, was "dist/alibabacloud_ehpc20180412-1.14.9.tar", last modified: Mon Oct 25 06:35:05 2021, max compression
```

## Comparing `alibabacloud_ehpc20180412-1.14.8.tar` & `alibabacloud_ehpc20180412-1.14.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-25 03:23:19.000000 alibabacloud_ehpc20180412-1.14.8/
--rw-r--r--   0 root         (0) root         (0)      165 2021-10-25 03:23:19.000000 alibabacloud_ehpc20180412-1.14.8/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2021-10-25 03:23:19.000000 alibabacloud_ehpc20180412-1.14.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2021-10-25 03:23:19.000000 alibabacloud_ehpc20180412-1.14.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2365 2021-10-25 03:23:19.000000 alibabacloud_ehpc20180412-1.14.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1025 2021-10-25 03:23:19.000000 alibabacloud_ehpc20180412-1.14.8/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1110 2021-10-25 03:23:19.000000 alibabacloud_ehpc20180412-1.14.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-25 03:23:19.000000 alibabacloud_ehpc20180412-1.14.8/alibabacloud_ehpc20180412/
--rw-r--r--   0 root         (0) root         (0)       22 2021-10-25 03:23:19.000000 alibabacloud_ehpc20180412-1.14.8/alibabacloud_ehpc20180412/__init__.py
--rw-r--r--   0 root         (0) root         (0)   217305 2021-10-25 03:23:19.000000 alibabacloud_ehpc20180412-1.14.8/alibabacloud_ehpc20180412/client.py
--rw-r--r--   0 root         (0) root         (0)   737630 2021-10-25 03:23:19.000000 alibabacloud_ehpc20180412-1.14.8/alibabacloud_ehpc20180412/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-25 03:23:19.000000 alibabacloud_ehpc20180412-1.14.8/alibabacloud_ehpc20180412.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2365 2021-10-25 03:23:19.000000 alibabacloud_ehpc20180412-1.14.8/alibabacloud_ehpc20180412.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      428 2021-10-25 03:23:19.000000 alibabacloud_ehpc20180412-1.14.8/alibabacloud_ehpc20180412.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-10-25 03:23:19.000000 alibabacloud_ehpc20180412-1.14.8/alibabacloud_ehpc20180412.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      156 2021-10-25 03:23:19.000000 alibabacloud_ehpc20180412-1.14.8/alibabacloud_ehpc20180412.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       26 2021-10-25 03:23:19.000000 alibabacloud_ehpc20180412-1.14.8/alibabacloud_ehpc20180412.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2021-10-25 03:23:19.000000 alibabacloud_ehpc20180412-1.14.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2645 2021-10-25 03:23:19.000000 alibabacloud_ehpc20180412-1.14.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-25 06:35:05.000000 alibabacloud_ehpc20180412-1.14.9/
+-rw-r--r--   0 root         (0) root         (0)      226 2021-10-25 06:35:05.000000 alibabacloud_ehpc20180412-1.14.9/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2021-10-25 06:35:05.000000 alibabacloud_ehpc20180412-1.14.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2021-10-25 06:35:05.000000 alibabacloud_ehpc20180412-1.14.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2365 2021-10-25 06:35:05.000000 alibabacloud_ehpc20180412-1.14.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1025 2021-10-25 06:35:05.000000 alibabacloud_ehpc20180412-1.14.9/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1110 2021-10-25 06:35:05.000000 alibabacloud_ehpc20180412-1.14.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-25 06:35:05.000000 alibabacloud_ehpc20180412-1.14.9/alibabacloud_ehpc20180412/
+-rw-r--r--   0 root         (0) root         (0)       22 2021-10-25 06:35:05.000000 alibabacloud_ehpc20180412-1.14.9/alibabacloud_ehpc20180412/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   217305 2021-10-25 06:35:05.000000 alibabacloud_ehpc20180412-1.14.9/alibabacloud_ehpc20180412/client.py
+-rw-r--r--   0 root         (0) root         (0)   737630 2021-10-25 06:35:05.000000 alibabacloud_ehpc20180412-1.14.9/alibabacloud_ehpc20180412/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-25 06:35:05.000000 alibabacloud_ehpc20180412-1.14.9/alibabacloud_ehpc20180412.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2365 2021-10-25 06:35:05.000000 alibabacloud_ehpc20180412-1.14.9/alibabacloud_ehpc20180412.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      428 2021-10-25 06:35:05.000000 alibabacloud_ehpc20180412-1.14.9/alibabacloud_ehpc20180412.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2021-10-25 06:35:05.000000 alibabacloud_ehpc20180412-1.14.9/alibabacloud_ehpc20180412.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      156 2021-10-25 06:35:05.000000 alibabacloud_ehpc20180412-1.14.9/alibabacloud_ehpc20180412.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       26 2021-10-25 06:35:05.000000 alibabacloud_ehpc20180412-1.14.9/alibabacloud_ehpc20180412.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2021-10-25 06:35:05.000000 alibabacloud_ehpc20180412-1.14.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2645 2021-10-25 06:35:05.000000 alibabacloud_ehpc20180412-1.14.9/setup.py
```

### Comparing `alibabacloud_ehpc20180412-1.14.8/LICENSE` & `alibabacloud_ehpc20180412-1.14.9/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_ehpc20180412-1.14.8/PKG-INFO` & `alibabacloud_ehpc20180412-1.14.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_ehpc20180412
-Version: 1.14.8
+Version: 1.14.9
 Summary: Alibaba Cloud Elastic High Performance Computing (20180412) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_ehpc20180412-1.14.8/README-CN.md` & `alibabacloud_ehpc20180412-1.14.9/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_ehpc20180412-1.14.8/README.md` & `alibabacloud_ehpc20180412-1.14.9/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_ehpc20180412-1.14.8/alibabacloud_ehpc20180412/client.py` & `alibabacloud_ehpc20180412-1.14.9/alibabacloud_ehpc20180412/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_ehpc20180412-1.14.8/alibabacloud_ehpc20180412/models.py` & `alibabacloud_ehpc20180412-1.14.9/alibabacloud_ehpc20180412/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_ehpc20180412-1.14.8/alibabacloud_ehpc20180412.egg-info/PKG-INFO` & `alibabacloud_ehpc20180412-1.14.9/alibabacloud_ehpc20180412.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-ehpc20180412
-Version: 1.14.8
+Version: 1.14.9
 Summary: Alibaba Cloud Elastic High Performance Computing (20180412) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_ehpc20180412-1.14.8/setup.py` & `alibabacloud_ehpc20180412-1.14.9/setup.py`

 * *Files identical despite different names*

