# Comparing `tmp/zoviz-0.4.98.tar.gz` & `tmp/zoviz-0.4.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/zoviz-0.4.98.tar", last modified: Thu Oct  1 07:07:10 2020, max compression
+gzip compressed data, was "dist/zoviz-0.4.99.tar", last modified: Thu Oct  8 07:07:11 2020, max compression
```

## Comparing `zoviz-0.4.98.tar` & `zoviz-0.4.99.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-01 07:07:10.000000 zoviz-0.4.98/
--rw-r--r--   0 root         (0) root         (0)      910 2020-10-01 07:07:10.000000 zoviz-0.4.98/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      373 2020-10-01 07:05:46.000000 zoviz-0.4.98/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2020-10-01 07:07:10.000000 zoviz-0.4.98/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      894 2020-10-01 07:05:46.000000 zoviz-0.4.98/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-01 07:07:10.000000 zoviz-0.4.98/zoviz/
--rw-rw-rw-   0 root         (0) root         (0)      184 2020-10-01 07:05:46.000000 zoviz-0.4.98/zoviz/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6476 2020-10-01 07:05:46.000000 zoviz-0.4.98/zoviz/database.py
--rw-rw-rw-   0 root         (0) root         (0)      230 2020-10-01 07:06:28.000000 zoviz-0.4.98/zoviz/metadata.py
--rw-rw-rw-   0 root         (0) root         (0)     2817 2020-10-01 07:05:46.000000 zoviz-0.4.98/zoviz/visualization.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-01 07:07:10.000000 zoviz-0.4.98/zoviz.egg-info/
--rw-r--r--   0 root         (0) root         (0)      910 2020-10-01 07:07:09.000000 zoviz-0.4.98/zoviz.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      239 2020-10-01 07:07:10.000000 zoviz-0.4.98/zoviz.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2020-10-01 07:07:09.000000 zoviz-0.4.98/zoviz.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       35 2020-10-01 07:07:09.000000 zoviz-0.4.98/zoviz.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2020-10-01 07:07:09.000000 zoviz-0.4.98/zoviz.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-08 07:07:11.000000 zoviz-0.4.99/
+-rw-r--r--   0 root         (0) root         (0)      910 2020-10-08 07:07:11.000000 zoviz-0.4.99/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      373 2020-10-08 07:05:50.000000 zoviz-0.4.99/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2020-10-08 07:07:11.000000 zoviz-0.4.99/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      894 2020-10-08 07:05:50.000000 zoviz-0.4.99/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-08 07:07:11.000000 zoviz-0.4.99/zoviz/
+-rw-rw-rw-   0 root         (0) root         (0)      184 2020-10-08 07:05:50.000000 zoviz-0.4.99/zoviz/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6476 2020-10-08 07:05:50.000000 zoviz-0.4.99/zoviz/database.py
+-rw-rw-rw-   0 root         (0) root         (0)      230 2020-10-08 07:06:28.000000 zoviz-0.4.99/zoviz/metadata.py
+-rw-rw-rw-   0 root         (0) root         (0)     2817 2020-10-08 07:05:50.000000 zoviz-0.4.99/zoviz/visualization.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-08 07:07:11.000000 zoviz-0.4.99/zoviz.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      910 2020-10-08 07:07:11.000000 zoviz-0.4.99/zoviz.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      239 2020-10-08 07:07:11.000000 zoviz-0.4.99/zoviz.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2020-10-08 07:07:11.000000 zoviz-0.4.99/zoviz.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       35 2020-10-08 07:07:11.000000 zoviz-0.4.99/zoviz.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2020-10-08 07:07:11.000000 zoviz-0.4.99/zoviz.egg-info/top_level.txt
```

### Comparing `zoviz-0.4.98/PKG-INFO` & `zoviz-0.4.99/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zoviz
-Version: 0.4.98
+Version: 0.4.99
 Summary: Unaffiliated visualization helper for Zotero data
 Home-page: https://gitlab.com/jlogan03/zoviz
 Author: James Logan
 Author-email: jlogan03@gmail.com
 License: UNKNOWN
 Description: Zoviz is an unaffiliated library for accessing and visualizing Zotero data.
```

### Comparing `zoviz-0.4.98/setup.py` & `zoviz-0.4.99/setup.py`

 * *Files identical despite different names*

### Comparing `zoviz-0.4.98/zoviz/database.py` & `zoviz-0.4.99/zoviz/database.py`

 * *Files identical despite different names*

### Comparing `zoviz-0.4.98/zoviz/visualization.py` & `zoviz-0.4.99/zoviz/visualization.py`

 * *Files identical despite different names*

### Comparing `zoviz-0.4.98/zoviz.egg-info/PKG-INFO` & `zoviz-0.4.99/zoviz.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zoviz
-Version: 0.4.98
+Version: 0.4.99
 Summary: Unaffiliated visualization helper for Zotero data
 Home-page: https://gitlab.com/jlogan03/zoviz
 Author: James Logan
 Author-email: jlogan03@gmail.com
 License: UNKNOWN
 Description: Zoviz is an unaffiliated library for accessing and visualizing Zotero data.
```

