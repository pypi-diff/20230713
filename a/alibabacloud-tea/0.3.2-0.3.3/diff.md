# Comparing `tmp/alibabacloud-tea-0.3.2.tar.gz` & `tmp/alibabacloud-tea-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud-tea-0.3.2.tar", last modified: Thu May 11 02:51:44 2023, max compression
+gzip compressed data, was "dist/alibabacloud-tea-0.3.3.tar", last modified: Thu Jul 13 04:00:12 2023, max compression
```

## Comparing `alibabacloud-tea-0.3.2.tar` & `alibabacloud-tea-0.3.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 02:51:44.000000 alibabacloud-tea-0.3.2/
--rw-r--r--   0 root         (0) root         (0)     2244 2023-05-11 02:51:44.000000 alibabacloud-tea-0.3.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1189 2023-05-11 02:51:44.000000 alibabacloud-tea-0.3.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 02:51:44.000000 alibabacloud-tea-0.3.2/Tea/
--rw-r--r--   0 root         (0) root         (0)       23 2023-05-11 02:51:44.000000 alibabacloud-tea-0.3.2/Tea/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9895 2023-05-11 02:51:44.000000 alibabacloud-tea-0.3.2/Tea/core.py
--rw-r--r--   0 root         (0) root         (0)     1490 2023-05-11 02:51:44.000000 alibabacloud-tea-0.3.2/Tea/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     1542 2023-05-11 02:51:44.000000 alibabacloud-tea-0.3.2/Tea/model.py
--rw-r--r--   0 root         (0) root         (0)      849 2023-05-11 02:51:44.000000 alibabacloud-tea-0.3.2/Tea/request.py
--rw-r--r--   0 root         (0) root         (0)      149 2023-05-11 02:51:44.000000 alibabacloud-tea-0.3.2/Tea/response.py
--rw-r--r--   0 root         (0) root         (0)      892 2023-05-11 02:51:44.000000 alibabacloud-tea-0.3.2/Tea/stream.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 02:51:44.000000 alibabacloud-tea-0.3.2/alibabacloud_tea.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2244 2023-05-11 02:51:44.000000 alibabacloud-tea-0.3.2/alibabacloud_tea.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      321 2023-05-11 02:51:44.000000 alibabacloud-tea-0.3.2/alibabacloud_tea.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-11 02:51:44.000000 alibabacloud-tea-0.3.2/alibabacloud_tea.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       60 2023-05-11 02:51:44.000000 alibabacloud-tea-0.3.2/alibabacloud_tea.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2023-05-11 02:51:44.000000 alibabacloud-tea-0.3.2/alibabacloud_tea.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-11 02:51:44.000000 alibabacloud-tea-0.3.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2559 2023-05-11 02:51:44.000000 alibabacloud-tea-0.3.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 04:00:12.000000 alibabacloud-tea-0.3.3/
+-rw-r--r--   0 root         (0) root         (0)     2244 2023-07-13 04:00:12.000000 alibabacloud-tea-0.3.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1189 2023-07-13 04:00:12.000000 alibabacloud-tea-0.3.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 04:00:12.000000 alibabacloud-tea-0.3.3/Tea/
+-rw-r--r--   0 root         (0) root         (0)       23 2023-07-13 04:00:12.000000 alibabacloud-tea-0.3.3/Tea/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10093 2023-07-13 04:00:12.000000 alibabacloud-tea-0.3.3/Tea/core.py
+-rw-r--r--   0 root         (0) root         (0)     1490 2023-07-13 04:00:12.000000 alibabacloud-tea-0.3.3/Tea/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     1542 2023-07-13 04:00:12.000000 alibabacloud-tea-0.3.3/Tea/model.py
+-rw-r--r--   0 root         (0) root         (0)      849 2023-07-13 04:00:12.000000 alibabacloud-tea-0.3.3/Tea/request.py
+-rw-r--r--   0 root         (0) root         (0)      149 2023-07-13 04:00:12.000000 alibabacloud-tea-0.3.3/Tea/response.py
+-rw-r--r--   0 root         (0) root         (0)      892 2023-07-13 04:00:12.000000 alibabacloud-tea-0.3.3/Tea/stream.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 04:00:12.000000 alibabacloud-tea-0.3.3/alibabacloud_tea.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2244 2023-07-13 04:00:12.000000 alibabacloud-tea-0.3.3/alibabacloud_tea.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      321 2023-07-13 04:00:12.000000 alibabacloud-tea-0.3.3/alibabacloud_tea.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-13 04:00:12.000000 alibabacloud-tea-0.3.3/alibabacloud_tea.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       60 2023-07-13 04:00:12.000000 alibabacloud-tea-0.3.3/alibabacloud_tea.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-07-13 04:00:12.000000 alibabacloud-tea-0.3.3/alibabacloud_tea.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-13 04:00:12.000000 alibabacloud-tea-0.3.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2559 2023-07-13 04:00:12.000000 alibabacloud-tea-0.3.3/setup.py
```

### Comparing `alibabacloud-tea-0.3.2/PKG-INFO` & `alibabacloud-tea-0.3.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: alibabacloud-tea
-Version: 0.3.2
+Version: 0.3.3
 Summary: The tea module of alibabaCloud Python SDK.
 Home-page: https://github.com/aliyun/tea-python
 Author: Alibaba Cloud
 Author-email: alibaba-cloud-sdk-dev-team@list.alibaba-inc.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud-tea-0.3.2/README.md` & `alibabacloud-tea-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud-tea-0.3.2/Tea/core.py` & `alibabacloud-tea-0.3.3/Tea/core.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 
 from typing import Dict, Any, Optional
 
 DEFAULT_CONNECT_TIMEOUT = 5000
 DEFAULT_READ_TIMEOUT = 10000
 DEFAULT_POOL_SIZE = 10
 
-
 logger = logging.getLogger('alibabacloud-tea')
 logger.setLevel(logging.DEBUG)
 ch = logging.StreamHandler()
 logger.addHandler(ch)
 
 
 class TeaCore:
@@ -133,14 +132,16 @@
         async with aiohttp.ClientSession(
             connector=connector
         ) as s:
             body = b''
             if isinstance(request.body, BaseStream):
                 for content in request.body:
                     body += content
+            elif isinstance(request.body, str):
+                body = request.body.encode('utf-8')
             else:
                 body = request.body
             try:
                 async with s.request(request.method, url,
                                      data=body,
                                      headers=request.headers,
                                      ssl=verify,
@@ -174,14 +175,17 @@
         connect_timeout = connect_timeout if connect_timeout else DEFAULT_CONNECT_TIMEOUT
 
         read_timeout = runtime_option.get('readTimeout')
         read_timeout = read_timeout if read_timeout else DEFAULT_READ_TIMEOUT
 
         timeout = (int(connect_timeout) / 1000, int(read_timeout) / 1000)
 
+        if isinstance(request.body, str):
+            request.body = request.body.encode('utf-8')
+
         p = PreparedRequest()
         p.prepare(
             method=request.method.upper(),
             url=url,
             data=request.body,
             headers=request.headers,
         )
```

### Comparing `alibabacloud-tea-0.3.2/Tea/exceptions.py` & `alibabacloud-tea-0.3.3/Tea/exceptions.py`

 * *Files identical despite different names*

### Comparing `alibabacloud-tea-0.3.2/Tea/model.py` & `alibabacloud-tea-0.3.3/Tea/model.py`

 * *Files identical despite different names*

### Comparing `alibabacloud-tea-0.3.2/Tea/request.py` & `alibabacloud-tea-0.3.3/Tea/request.py`

 * *Files identical despite different names*

### Comparing `alibabacloud-tea-0.3.2/Tea/stream.py` & `alibabacloud-tea-0.3.3/Tea/stream.py`

 * *Files identical despite different names*

### Comparing `alibabacloud-tea-0.3.2/alibabacloud_tea.egg-info/PKG-INFO` & `alibabacloud-tea-0.3.3/alibabacloud_tea.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: alibabacloud-tea
-Version: 0.3.2
+Version: 0.3.3
 Summary: The tea module of alibabaCloud Python SDK.
 Home-page: https://github.com/aliyun/tea-python
 Author: Alibaba Cloud
 Author-email: alibaba-cloud-sdk-dev-team@list.alibaba-inc.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud-tea-0.3.2/setup.py` & `alibabacloud-tea-0.3.3/setup.py`

 * *Files identical despite different names*

