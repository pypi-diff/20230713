# Comparing `tmp/zitan-0.1.1.tar.gz` & `tmp/zitan-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\zitan-0.1.1.tar", last modified: Thu Jul 13 09:44:46 2023, max compression
+gzip compressed data, was "dist\zitan-0.1.2.tar", last modified: Thu Jul 13 09:55:51 2023, max compression
```

## Comparing `zitan-0.1.1.tar` & `zitan-0.1.2.tar`

### file list

```diff
@@ -1,11 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-07-13 09:44:46.000000 zitan-0.1.1/
--rw-rw-rw-   0        0        0      707 2023-07-13 09:44:46.000000 zitan-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0       11 2023-07-12 11:42:42.000000 zitan-0.1.1/README.txt
--rw-rw-rw-   0        0        0       78 2023-07-12 09:34:05.000000 zitan-0.1.1/main.py
--rw-rw-rw-   0        0        0       42 2023-07-13 09:44:46.000000 zitan-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0     4164 2023-07-13 09:43:51.000000 zitan-0.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-13 09:44:46.000000 zitan-0.1.1/zitan.egg-info/
--rw-rw-rw-   0        0        0      707 2023-07-13 09:44:46.000000 zitan-0.1.1/zitan.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      143 2023-07-13 09:44:46.000000 zitan-0.1.1/zitan.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-13 09:44:46.000000 zitan-0.1.1/zitan.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-13 09:44:46.000000 zitan-0.1.1/zitan.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-13 09:55:51.000000 zitan-0.1.2/
+-rw-rw-rw-   0        0        0     1088 2023-07-12 11:41:48.000000 zitan-0.1.2/LICENSE.txt
+-rw-rw-rw-   0        0        0      704 2023-07-13 09:55:51.000000 zitan-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0       11 2023-07-12 11:42:42.000000 zitan-0.1.2/README.txt
+-rw-rw-rw-   0        0        0       78 2023-07-12 09:34:05.000000 zitan-0.1.2/main.py
+-rw-rw-rw-   0        0        0       42 2023-07-13 09:55:51.000000 zitan-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     4164 2023-07-13 09:54:48.000000 zitan-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-13 09:55:51.000000 zitan-0.1.2/zitan.egg-info/
+-rw-rw-rw-   0        0        0      704 2023-07-13 09:55:50.000000 zitan-0.1.2/zitan.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      155 2023-07-13 09:55:50.000000 zitan-0.1.2/zitan.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-13 09:55:50.000000 zitan-0.1.2/zitan.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-13 09:55:50.000000 zitan-0.1.2/zitan.egg-info/top_level.txt
```

### Comparing `zitan-0.1.1/PKG-INFO` & `zitan-0.1.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: zitan
-Version: 0.1.1
+Version: 0.1.2
 Summary: This project is used to display ...
 Home-page: https://github.com/你的github账户/test(项目文件夹名称)
 Author: xxx
 Author-email: xxx@gmail.com
 License: MIT
-Description: This project is used to display ...
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+This project is used to display ...
```

### Comparing `zitan-0.1.1/setup.py` & `zitan-0.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 # Package meta-data.
 NAME = 'zitan'  # 项目的名称，即包的分发名称
 DESCRIPTION = 'This project is used to display ...'  # 项目的简短描述
 URL = 'https://github.com/你的github账户/test(项目文件夹名称)'
 EMAIL = 'xxx@gmail.com'  # 项目作者的邮件
 AUTHOR = 'xxx'  # 项目作者的名字
 REQUIRES_PYTHON = '>=3.6.0'  # 项目支持的版本
-VERSION = '0.1.1'  # 项目的版本,如果后续代码有了任何更改，再次上传需要增加版本号
+VERSION = '0.1.2'  # 项目的版本,如果后续代码有了任何更改，再次上传需要增加版本号
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     # 'requests', 'maya', 'records',
 ]
 
 # What packages are optional?
```

### Comparing `zitan-0.1.1/zitan.egg-info/PKG-INFO` & `zitan-0.1.2/zitan.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: zitan
-Version: 0.1.1
+Version: 0.1.2
 Summary: This project is used to display ...
 Home-page: https://github.com/你的github账户/test(项目文件夹名称)
 Author: xxx
 Author-email: xxx@gmail.com
 License: MIT
-Description: This project is used to display ...
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+This project is used to display ...
```

