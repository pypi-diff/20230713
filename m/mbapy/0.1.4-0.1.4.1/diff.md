# Comparing `tmp/mbapy-0.1.4.tar.gz` & `tmp/mbapy-0.1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mbapy-0.1.4.tar", last modified: Wed Jul 12 13:32:37 2023, max compression
+gzip compressed data, was "mbapy-0.1.4.1.tar", last modified: Thu Jul 13 11:14:15 2023, max compression
```

## Comparing `mbapy-0.1.4.tar` & `mbapy-0.1.4.1.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxrwxrwx   0        0        0        0 2023-07-12 13:32:37.088689 mbapy-0.1.4/
--rw-rw-rw-   0        0        0     1085 2022-10-19 14:16:22.000000 mbapy-0.1.4/LICENSE
--rw-rw-rw-   0        0        0     2747 2023-07-12 13:32:37.086689 mbapy-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     1921 2023-06-29 14:51:48.000000 mbapy-0.1.4/README.md
-drwxrwxrwx   0        0        0        0 2023-07-12 13:32:37.013340 mbapy-0.1.4/mbapy/
--rw-rw-rw-   0        0        0      862 2023-07-11 16:18:10.000000 mbapy-0.1.4/mbapy/__init__.py
--rw-rw-rw-   0        0        0      402 2023-07-12 13:12:09.000000 mbapy-0.1.4/mbapy/__version__.py
--rw-rw-rw-   0        0        0    12020 2023-07-11 14:33:25.000000 mbapy-0.1.4/mbapy/base.py
-drwxrwxrwx   0        0        0        0 2023-07-12 13:32:37.031676 mbapy-0.1.4/mbapy/dl_torch/
--rw-rw-rw-   0        0        0      363 2023-05-25 14:57:15.000000 mbapy-0.1.4/mbapy/dl_torch/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-12 13:32:37.033676 mbapy-0.1.4/mbapy/dl_torch/arch/
-drwxrwxrwx   0        0        0        0 2023-07-12 13:32:37.048679 mbapy-0.1.4/mbapy/dl_torch/arch/CL/
--rw-rw-rw-   0        0        0       34 2023-06-06 15:50:53.000000 mbapy-0.1.4/mbapy/dl_torch/arch/CL/__init__.py
--rw-rw-rw-   0        0        0    16561 2023-06-07 03:36:12.000000 mbapy-0.1.4/mbapy/dl_torch/arch/CL/builder.py
--rw-rw-rw-   0        0        0     2419 2023-06-07 03:14:56.000000 mbapy-0.1.4/mbapy/dl_torch/arch/CL/trainer.py
-drwxrwxrwx   0        0        0        0 2023-07-12 13:32:37.053682 mbapy-0.1.4/mbapy/dl_torch/arch/CLIP/
--rw-rw-rw-   0        0        0       32 2023-06-06 15:37:25.000000 mbapy-0.1.4/mbapy/dl_torch/arch/CLIP/__init__.py
--rw-rw-rw-   0        0        0        0 2023-06-06 15:35:10.000000 mbapy-0.1.4/mbapy/dl_torch/arch/CLIP/builder.py
--rw-rw-rw-   0        0        0        0 2023-06-06 15:35:17.000000 mbapy-0.1.4/mbapy/dl_torch/arch/CLIP/trainer.py
--rw-rw-rw-   0        0        0      203 2023-06-06 15:38:23.000000 mbapy-0.1.4/mbapy/dl_torch/arch/__init__.py
--rw-rw-rw-   0        0        0    22606 2023-06-02 01:55:22.000000 mbapy-0.1.4/mbapy/dl_torch/bb.py
--rw-rw-rw-   0        0        0     6379 2023-06-30 02:27:21.000000 mbapy-0.1.4/mbapy/dl_torch/data.py
--rw-rw-rw-   0        0        0     1052 2023-05-01 12:18:06.000000 mbapy-0.1.4/mbapy/dl_torch/hyper_search.py
--rw-rw-rw-   0        0        0     4113 2023-03-20 16:36:17.000000 mbapy-0.1.4/mbapy/dl_torch/loss.py
--rw-rw-rw-   0        0        0    13193 2023-06-02 01:55:22.000000 mbapy-0.1.4/mbapy/dl_torch/m.py
--rw-rw-rw-   0        0        0     3877 2023-06-02 01:55:22.000000 mbapy-0.1.4/mbapy/dl_torch/optim.py
-drwxrwxrwx   0        0        0        0 2023-07-12 13:32:37.055680 mbapy-0.1.4/mbapy/dl_torch/paper/
--rw-rw-rw-   0        0        0       18 2023-05-04 14:59:39.000000 mbapy-0.1.4/mbapy/dl_torch/paper/__init__.py
--rw-rw-rw-   0        0        0     2947 2023-05-25 14:57:15.000000 mbapy-0.1.4/mbapy/dl_torch/paper/bb.py
--rw-rw-rw-   0        0        0    11474 2023-06-15 14:59:22.000000 mbapy-0.1.4/mbapy/dl_torch/utils.py
--rw-rw-rw-   0        0        0    10373 2023-07-10 14:50:19.000000 mbapy-0.1.4/mbapy/file.py
--rw-rw-rw-   0        0        0    16575 2023-07-12 13:05:45.000000 mbapy-0.1.4/mbapy/paper.py
--rw-rw-rw-   0        0        0    14968 2023-07-10 12:49:19.000000 mbapy-0.1.4/mbapy/plot.py
-drwxrwxrwx   0        0        0        0 2023-07-12 13:32:37.060683 mbapy-0.1.4/mbapy/stats/
--rw-rw-rw-   0        0        0      539 2023-04-19 11:56:16.000000 mbapy-0.1.4/mbapy/stats/__init__.py
--rw-rw-rw-   0        0        0    12351 2023-07-10 12:49:19.000000 mbapy-0.1.4/mbapy/stats/df.py
--rw-rw-rw-   0        0        0    19333 2022-12-05 10:10:18.000000 mbapy-0.1.4/mbapy/stats/geography.py
--rw-rw-rw-   0        0        0     1281 2023-06-15 15:01:10.000000 mbapy-0.1.4/mbapy/stats/reg.py
--rw-rw-rw-   0        0        0    12735 2023-07-10 12:49:19.000000 mbapy-0.1.4/mbapy/stats/test.py
-drwxrwxrwx   0        0        0        0 2023-07-12 13:32:37.081686 mbapy-0.1.4/mbapy/storage/
--rw-rw-rw-   0        0        0    86016 2023-07-06 15:23:54.000000 mbapy-0.1.4/mbapy/storage/stats.dll
--rw-rw-rw-   0        0        0    16243 2023-07-12 13:29:22.000000 mbapy-0.1.4/mbapy/web.py
-drwxrwxrwx   0        0        0        0 2023-07-12 13:32:37.023343 mbapy-0.1.4/mbapy.egg-info/
--rw-rw-rw-   0        0        0     2747 2023-07-12 13:32:36.000000 mbapy-0.1.4/mbapy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      941 2023-07-12 13:32:36.000000 mbapy-0.1.4/mbapy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-12 13:32:36.000000 mbapy-0.1.4/mbapy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      432 2023-07-12 13:32:36.000000 mbapy-0.1.4/mbapy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-07-12 13:32:36.000000 mbapy-0.1.4/mbapy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-12 13:32:37.088689 mbapy-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0     2485 2023-07-11 16:18:10.000000 mbapy-0.1.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-12 13:32:37.084687 mbapy-0.1.4/test/
--rw-rw-rw-   0        0        0     1998 2023-07-12 13:19:31.000000 mbapy-0.1.4/test/test_base.py
--rw-rw-rw-   0        0        0     1740 2023-07-12 13:29:09.000000 mbapy-0.1.4/test/test_web.py
+drwxrwxrwx   0        0        0        0 2023-07-13 11:14:15.068061 mbapy-0.1.4.1/
+-rw-rw-rw-   0        0        0     1085 2022-10-19 14:16:22.000000 mbapy-0.1.4.1/LICENSE
+-rw-rw-rw-   0        0        0     3252 2023-07-13 11:14:15.067063 mbapy-0.1.4.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2424 2023-07-12 14:06:22.000000 mbapy-0.1.4.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-13 11:14:15.019053 mbapy-0.1.4.1/mbapy/
+-rw-rw-rw-   0        0        0      862 2023-07-11 16:18:10.000000 mbapy-0.1.4.1/mbapy/__init__.py
+-rw-rw-rw-   0        0        0      421 2023-07-13 11:13:59.000000 mbapy-0.1.4.1/mbapy/__version__.py
+-rw-rw-rw-   0        0        0    12020 2023-07-11 14:33:25.000000 mbapy-0.1.4.1/mbapy/base.py
+drwxrwxrwx   0        0        0        0 2023-07-13 11:14:15.046058 mbapy-0.1.4.1/mbapy/dl_torch/
+-rw-rw-rw-   0        0        0      363 2023-05-25 14:57:15.000000 mbapy-0.1.4.1/mbapy/dl_torch/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-13 11:14:15.048058 mbapy-0.1.4.1/mbapy/dl_torch/arch/
+drwxrwxrwx   0        0        0        0 2023-07-13 11:14:15.050059 mbapy-0.1.4.1/mbapy/dl_torch/arch/CL/
+-rw-rw-rw-   0        0        0       34 2023-06-06 15:50:53.000000 mbapy-0.1.4.1/mbapy/dl_torch/arch/CL/__init__.py
+-rw-rw-rw-   0        0        0    16561 2023-06-07 03:36:12.000000 mbapy-0.1.4.1/mbapy/dl_torch/arch/CL/builder.py
+-rw-rw-rw-   0        0        0     2419 2023-06-07 03:14:56.000000 mbapy-0.1.4.1/mbapy/dl_torch/arch/CL/trainer.py
+drwxrwxrwx   0        0        0        0 2023-07-13 11:14:15.054063 mbapy-0.1.4.1/mbapy/dl_torch/arch/CLIP/
+-rw-rw-rw-   0        0        0       32 2023-06-06 15:37:25.000000 mbapy-0.1.4.1/mbapy/dl_torch/arch/CLIP/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-06-06 15:35:10.000000 mbapy-0.1.4.1/mbapy/dl_torch/arch/CLIP/builder.py
+-rw-rw-rw-   0        0        0        0 2023-06-06 15:35:17.000000 mbapy-0.1.4.1/mbapy/dl_torch/arch/CLIP/trainer.py
+-rw-rw-rw-   0        0        0      203 2023-06-06 15:38:23.000000 mbapy-0.1.4.1/mbapy/dl_torch/arch/__init__.py
+-rw-rw-rw-   0        0        0    22606 2023-06-02 01:55:22.000000 mbapy-0.1.4.1/mbapy/dl_torch/bb.py
+-rw-rw-rw-   0        0        0     6379 2023-06-30 02:27:21.000000 mbapy-0.1.4.1/mbapy/dl_torch/data.py
+-rw-rw-rw-   0        0        0     1052 2023-05-01 12:18:06.000000 mbapy-0.1.4.1/mbapy/dl_torch/hyper_search.py
+-rw-rw-rw-   0        0        0     4113 2023-03-20 16:36:17.000000 mbapy-0.1.4.1/mbapy/dl_torch/loss.py
+-rw-rw-rw-   0        0        0    13193 2023-06-02 01:55:22.000000 mbapy-0.1.4.1/mbapy/dl_torch/m.py
+-rw-rw-rw-   0        0        0     3877 2023-06-02 01:55:22.000000 mbapy-0.1.4.1/mbapy/dl_torch/optim.py
+drwxrwxrwx   0        0        0        0 2023-07-13 11:14:15.057061 mbapy-0.1.4.1/mbapy/dl_torch/paper/
+-rw-rw-rw-   0        0        0       18 2023-05-04 14:59:39.000000 mbapy-0.1.4.1/mbapy/dl_torch/paper/__init__.py
+-rw-rw-rw-   0        0        0     2947 2023-05-25 14:57:15.000000 mbapy-0.1.4.1/mbapy/dl_torch/paper/bb.py
+-rw-rw-rw-   0        0        0    11474 2023-06-15 14:59:22.000000 mbapy-0.1.4.1/mbapy/dl_torch/utils.py
+-rw-rw-rw-   0        0        0    10373 2023-07-10 14:50:19.000000 mbapy-0.1.4.1/mbapy/file.py
+-rw-rw-rw-   0        0        0    16575 2023-07-12 13:05:45.000000 mbapy-0.1.4.1/mbapy/paper.py
+-rw-rw-rw-   0        0        0    14968 2023-07-10 12:49:19.000000 mbapy-0.1.4.1/mbapy/plot.py
+drwxrwxrwx   0        0        0        0 2023-07-13 11:14:15.063062 mbapy-0.1.4.1/mbapy/stats/
+-rw-rw-rw-   0        0        0      539 2023-04-19 11:56:16.000000 mbapy-0.1.4.1/mbapy/stats/__init__.py
+-rw-rw-rw-   0        0        0    12351 2023-07-10 12:49:19.000000 mbapy-0.1.4.1/mbapy/stats/df.py
+-rw-rw-rw-   0        0        0    19333 2022-12-05 10:10:18.000000 mbapy-0.1.4.1/mbapy/stats/geography.py
+-rw-rw-rw-   0        0        0     1281 2023-06-15 15:01:10.000000 mbapy-0.1.4.1/mbapy/stats/reg.py
+-rw-rw-rw-   0        0        0    12735 2023-07-10 12:49:19.000000 mbapy-0.1.4.1/mbapy/stats/test.py
+drwxrwxrwx   0        0        0        0 2023-07-13 11:14:15.064062 mbapy-0.1.4.1/mbapy/storage/
+-rw-rw-rw-   0        0        0    86016 2023-07-06 15:23:54.000000 mbapy-0.1.4.1/mbapy/storage/stats.dll
+-rw-rw-rw-   0        0        0    16243 2023-07-12 13:29:22.000000 mbapy-0.1.4.1/mbapy/web.py
+drwxrwxrwx   0        0        0        0 2023-07-13 11:14:15.036065 mbapy-0.1.4.1/mbapy.egg-info/
+-rw-rw-rw-   0        0        0     3252 2023-07-13 11:14:14.000000 mbapy-0.1.4.1/mbapy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      941 2023-07-13 11:14:14.000000 mbapy-0.1.4.1/mbapy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-13 11:14:14.000000 mbapy-0.1.4.1/mbapy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      432 2023-07-13 11:14:14.000000 mbapy-0.1.4.1/mbapy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-13 11:14:14.000000 mbapy-0.1.4.1/mbapy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-13 11:14:15.068061 mbapy-0.1.4.1/setup.cfg
+-rw-rw-rw-   0        0        0     3092 2023-07-13 11:11:54.000000 mbapy-0.1.4.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-13 11:14:15.066062 mbapy-0.1.4.1/test/
+-rw-rw-rw-   0        0        0     1998 2023-07-12 13:19:31.000000 mbapy-0.1.4.1/test/test_base.py
+-rw-rw-rw-   0        0        0     1740 2023-07-12 13:29:09.000000 mbapy-0.1.4.1/test/test_web.py
```

### Comparing `mbapy-0.1.4/LICENSE` & `mbapy-0.1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mbapy-0.1.4/PKG-INFO` & `mbapy-0.1.4.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mbapy
-Version: 0.1.4
+Version: 0.1.4.1
 Summary: MyBA in Python
 Home-page: https://github.com/BHM-Bob/BA_PY
 Author: BHM-Bob G
 Author-email: bhmfly@foxmail.com
 License: MIT Licence
 Keywords: mbapy,Utilities,plot
 Platform: any
@@ -21,21 +21,27 @@
 Requires-Python: >=3.7, <3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <!--
  * @Author: BHM-Bob 2262029386@qq.com
  * @Date: 2022-10-19 22:16:22
- * @LastEditors: BHM-Bob G 2262029386@qq.com
- * @LastEditTime: 2023-06-23 09:38:02
+ * @LastEditors: BHM-Bob 2262029386@qq.com
+ * @LastEditTime: 2023-07-12 22:06:01
  * @Description: 
 -->
 # BA_PY
 [![Downloads](https://static.pepy.tech/badge/mbapy)](https://pepy.tech/project/mbapy) ![PyPI - Downloads](https://img.shields.io/pypi/dm/mbapy) ![GitHub all releases](https://img.shields.io/github/downloads/BHM-Bob/BA_PY/total?label=GitHub%20all%20releases%20downloads)
 
+![GitHub repo size](https://img.shields.io/github/repo-size/BHM-Bob/BA_PY) ![GitHub code size in bytes](https://img.shields.io/github/languages/code-size/BHM-Bob/BA_PY) [![GitHub Commit Activity](https://img.shields.io/github/commit-activity/m/BHM-Bob/BA_PY)](https://github.com/BHM-Bob/BA_PY/pulse)
+
+![PyPI - Status](https://img.shields.io/pypi/status/mbapy?label=PyPI%20Status) ![PyPI](https://img.shields.io/pypi/v/mbapy)
+ ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mbapy)
+
+
 ![GitHub](https://img.shields.io/github/license/BHM-Bob/BA_PY)
 
 some helpful python scripts. (Basic for All in Python)
 Mainly contains sci-plot, stats, web-crawler and deeplearing-torch.
 
 ## get start
```

### Comparing `mbapy-0.1.4/README.md` & `mbapy-0.1.4.1/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,17 +1,23 @@
 <!--
  * @Author: BHM-Bob 2262029386@qq.com
  * @Date: 2022-10-19 22:16:22
- * @LastEditors: BHM-Bob G 2262029386@qq.com
- * @LastEditTime: 2023-06-23 09:38:02
+ * @LastEditors: BHM-Bob 2262029386@qq.com
+ * @LastEditTime: 2023-07-12 22:06:01
  * @Description: 
 -->
 # BA_PY
 [![Downloads](https://static.pepy.tech/badge/mbapy)](https://pepy.tech/project/mbapy) ![PyPI - Downloads](https://img.shields.io/pypi/dm/mbapy) ![GitHub all releases](https://img.shields.io/github/downloads/BHM-Bob/BA_PY/total?label=GitHub%20all%20releases%20downloads)
 
+![GitHub repo size](https://img.shields.io/github/repo-size/BHM-Bob/BA_PY) ![GitHub code size in bytes](https://img.shields.io/github/languages/code-size/BHM-Bob/BA_PY) [![GitHub Commit Activity](https://img.shields.io/github/commit-activity/m/BHM-Bob/BA_PY)](https://github.com/BHM-Bob/BA_PY/pulse)
+
+![PyPI - Status](https://img.shields.io/pypi/status/mbapy?label=PyPI%20Status) ![PyPI](https://img.shields.io/pypi/v/mbapy)
+ ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mbapy)
+
+
 ![GitHub](https://img.shields.io/github/license/BHM-Bob/BA_PY)
 
 some helpful python scripts. (Basic for All in Python)
 Mainly contains sci-plot, stats, web-crawler and deeplearing-torch.
 
 ## get start
```

### Comparing `mbapy-0.1.4/mbapy/__init__.py` & `mbapy-0.1.4.1/mbapy/__init__.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.1.4/mbapy/base.py` & `mbapy-0.1.4.1/mbapy/base.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.1.4/mbapy/dl_torch/arch/CL/builder.py` & `mbapy-0.1.4.1/mbapy/dl_torch/arch/CL/builder.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.1.4/mbapy/dl_torch/arch/CL/trainer.py` & `mbapy-0.1.4.1/mbapy/dl_torch/arch/CL/trainer.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.1.4/mbapy/dl_torch/bb.py` & `mbapy-0.1.4.1/mbapy/dl_torch/bb.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.1.4/mbapy/dl_torch/data.py` & `mbapy-0.1.4.1/mbapy/dl_torch/data.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.1.4/mbapy/dl_torch/hyper_search.py` & `mbapy-0.1.4.1/mbapy/dl_torch/hyper_search.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.1.4/mbapy/dl_torch/loss.py` & `mbapy-0.1.4.1/mbapy/dl_torch/loss.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.1.4/mbapy/dl_torch/m.py` & `mbapy-0.1.4.1/mbapy/dl_torch/m.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.1.4/mbapy/dl_torch/optim.py` & `mbapy-0.1.4.1/mbapy/dl_torch/optim.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.1.4/mbapy/dl_torch/paper/bb.py` & `mbapy-0.1.4.1/mbapy/dl_torch/paper/bb.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.1.4/mbapy/dl_torch/utils.py` & `mbapy-0.1.4.1/mbapy/dl_torch/utils.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.1.4/mbapy/file.py` & `mbapy-0.1.4.1/mbapy/file.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.1.4/mbapy/paper.py` & `mbapy-0.1.4.1/mbapy/paper.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.1.4/mbapy/plot.py` & `mbapy-0.1.4.1/mbapy/plot.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.1.4/mbapy/stats/__init__.py` & `mbapy-0.1.4.1/mbapy/stats/__init__.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.1.4/mbapy/stats/df.py` & `mbapy-0.1.4.1/mbapy/stats/df.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.1.4/mbapy/stats/geography.py` & `mbapy-0.1.4.1/mbapy/stats/geography.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.1.4/mbapy/stats/reg.py` & `mbapy-0.1.4.1/mbapy/stats/reg.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.1.4/mbapy/stats/test.py` & `mbapy-0.1.4.1/mbapy/stats/test.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.1.4/mbapy/storage/stats.dll` & `mbapy-0.1.4.1/mbapy/storage/stats.dll`

 * *Files identical despite different names*

### Comparing `mbapy-0.1.4/mbapy/web.py` & `mbapy-0.1.4.1/mbapy/web.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.1.4/mbapy.egg-info/PKG-INFO` & `mbapy-0.1.4.1/mbapy.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mbapy
-Version: 0.1.4
+Version: 0.1.4.1
 Summary: MyBA in Python
 Home-page: https://github.com/BHM-Bob/BA_PY
 Author: BHM-Bob G
 Author-email: bhmfly@foxmail.com
 License: MIT Licence
 Keywords: mbapy,Utilities,plot
 Platform: any
@@ -21,21 +21,27 @@
 Requires-Python: >=3.7, <3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <!--
  * @Author: BHM-Bob 2262029386@qq.com
  * @Date: 2022-10-19 22:16:22
- * @LastEditors: BHM-Bob G 2262029386@qq.com
- * @LastEditTime: 2023-06-23 09:38:02
+ * @LastEditors: BHM-Bob 2262029386@qq.com
+ * @LastEditTime: 2023-07-12 22:06:01
  * @Description: 
 -->
 # BA_PY
 [![Downloads](https://static.pepy.tech/badge/mbapy)](https://pepy.tech/project/mbapy) ![PyPI - Downloads](https://img.shields.io/pypi/dm/mbapy) ![GitHub all releases](https://img.shields.io/github/downloads/BHM-Bob/BA_PY/total?label=GitHub%20all%20releases%20downloads)
 
+![GitHub repo size](https://img.shields.io/github/repo-size/BHM-Bob/BA_PY) ![GitHub code size in bytes](https://img.shields.io/github/languages/code-size/BHM-Bob/BA_PY) [![GitHub Commit Activity](https://img.shields.io/github/commit-activity/m/BHM-Bob/BA_PY)](https://github.com/BHM-Bob/BA_PY/pulse)
+
+![PyPI - Status](https://img.shields.io/pypi/status/mbapy?label=PyPI%20Status) ![PyPI](https://img.shields.io/pypi/v/mbapy)
+ ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mbapy)
+
+
 ![GitHub](https://img.shields.io/github/license/BHM-Bob/BA_PY)
 
 some helpful python scripts. (Basic for All in Python)
 Mainly contains sci-plot, stats, web-crawler and deeplearing-torch.
 
 ## get start
```

### Comparing `mbapy-0.1.4/mbapy.egg-info/SOURCES.txt` & `mbapy-0.1.4.1/mbapy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mbapy-0.1.4/setup.py` & `mbapy-0.1.4.1/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 '''
 Author: BHM-Bob 2262029386@qq.com
 Date: 2022-11-01 18:30:01
 LastEditors: BHM-Bob 2262029386@qq.com
-LastEditTime: 2023-07-10 16:55:48
+LastEditTime: 2023-07-13 19:11:41
 Description: 
 '''
 """
 something is from https://github.com/pypa/sampleproject
 thanks to https://zetcode.com/python/package/
 """
 
@@ -32,15 +32,45 @@
     if '__author_email__' in line:
         __author_email__ = line[line.find('"')+1:-1]
     if '__author__' in line:
         __author__ = line[line.find('"')+1:-1]
     if '__url__' in line:
         __url__ = line[line.find('"')+1:-1]
 
-requires = (here / "requirements.txt").read_text(encoding="utf-8")
+requires = [
+    "beautifulsoup4>=4.11.1",
+    "bokeh>=2.4.3",
+    "chardet>=5.0.0",
+    "cn2an>=0.5.17",
+    "holoviews>=1.15.1",
+    "imageio>=2.22.2",
+    "importlib-metadata>=4.12.0",
+    "jieba>=0.42.1",
+    "Markdown>=3.4.1",
+    "matplotlib>=3.5.3",
+    "multiprocess>=0.70.13",
+    "numpy>=1.20.3",
+    "pandas>=1.4.3",
+    "pathtools>=0.1.2",
+    "pdfkit>=1.0.0",
+    "Pillow>=9.2.0",
+    "plotly>=5.10.0",
+    "requests>=2.28.1",
+    "scikit-learn>=1.1.2",
+    "scipy>=1.9.1",
+    "seaborn>=0.11.2",
+    "selenium>=4.5.0",
+    "urllib3>=1.26.12",
+    "openpyxl",
+    "statsmodels",
+    "scikit_posthocs",
+    "PyPDF2",
+    "lxml",
+]
+
 
 setup(
     name = "mbapy",
     version = __version__,
 
     classifiers=[
         "Development Status :: 4 - Beta",
```

### Comparing `mbapy-0.1.4/test/test_base.py` & `mbapy-0.1.4.1/test/test_base.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.1.4/test/test_web.py` & `mbapy-0.1.4.1/test/test_web.py`

 * *Files identical despite different names*

