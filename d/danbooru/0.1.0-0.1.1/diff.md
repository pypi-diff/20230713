# Comparing `tmp/danbooru-0.1.0.tar.gz` & `tmp/danbooru-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "danbooru-0.1.0.tar", last modified: Thu Jul 13 03:55:36 2023, max compression
+gzip compressed data, was "danbooru-0.1.1.tar", last modified: Thu Jul 13 04:47:26 2023, max compression
```

## Comparing `danbooru-0.1.0.tar` & `danbooru-0.1.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 sayu      (1000) sayu      (1000)        0 2023-07-13 03:55:36.293065 danbooru-0.1.0/
--rw-rw-r--   0 sayu      (1000) sayu      (1000)     1066 2023-07-13 03:34:40.000000 danbooru-0.1.0/LICENSE
--rw-rw-r--   0 sayu      (1000) sayu      (1000)     1850 2023-07-13 03:55:36.289065 danbooru-0.1.0/PKG-INFO
--rw-rw-r--   0 sayu      (1000) sayu      (1000)     1492 2023-07-13 03:34:40.000000 danbooru-0.1.0/README.md
-drwxrwxr-x   0 sayu      (1000) sayu      (1000)        0 2023-07-13 03:55:36.289065 danbooru-0.1.0/danbooru/
--rw-rw-r--   0 sayu      (1000) sayu      (1000)       74 2023-07-13 03:34:40.000000 danbooru-0.1.0/danbooru/__init__.py
--rw-rw-r--   0 sayu      (1000) sayu      (1000)      197 2023-07-13 03:51:53.000000 danbooru-0.1.0/danbooru/__vars__.py
--rw-rw-r--   0 sayu      (1000) sayu      (1000)    11445 2023-07-13 03:44:58.000000 danbooru-0.1.0/danbooru/booru.py
--rw-rw-r--   0 sayu      (1000) sayu      (1000)      946 2023-07-13 03:34:40.000000 danbooru-0.1.0/danbooru/exceptions.py
-drwxrwxr-x   0 sayu      (1000) sayu      (1000)        0 2023-07-13 03:55:36.289065 danbooru-0.1.0/danbooru/types/
--rw-rw-r--   0 sayu      (1000) sayu      (1000)    20045 2023-07-13 03:38:20.000000 danbooru-0.1.0/danbooru/types/Danbooru_API.py
--rw-rw-r--   0 sayu      (1000) sayu      (1000)     2555 2023-07-13 03:34:40.000000 danbooru-0.1.0/danbooru/types/Danbooru_Types.py
--rw-rw-r--   0 sayu      (1000) sayu      (1000)        0 2023-07-13 03:34:40.000000 danbooru-0.1.0/danbooru/types/__init__.py
-drwxrwxr-x   0 sayu      (1000) sayu      (1000)        0 2023-07-13 03:55:36.289065 danbooru-0.1.0/danbooru.egg-info/
--rw-rw-r--   0 sayu      (1000) sayu      (1000)     1850 2023-07-13 03:55:36.000000 danbooru-0.1.0/danbooru.egg-info/PKG-INFO
--rw-rw-r--   0 sayu      (1000) sayu      (1000)      359 2023-07-13 03:55:36.000000 danbooru-0.1.0/danbooru.egg-info/SOURCES.txt
--rw-rw-r--   0 sayu      (1000) sayu      (1000)        1 2023-07-13 03:55:36.000000 danbooru-0.1.0/danbooru.egg-info/dependency_links.txt
--rw-rw-r--   0 sayu      (1000) sayu      (1000)       28 2023-07-13 03:55:36.000000 danbooru-0.1.0/danbooru.egg-info/requires.txt
--rw-rw-r--   0 sayu      (1000) sayu      (1000)        9 2023-07-13 03:55:36.000000 danbooru-0.1.0/danbooru.egg-info/top_level.txt
--rw-rw-r--   0 sayu      (1000) sayu      (1000)       38 2023-07-13 03:55:36.293065 danbooru-0.1.0/setup.cfg
--rw-rw-r--   0 sayu      (1000) sayu      (1000)      654 2023-07-13 03:34:40.000000 danbooru-0.1.0/setup.py
+drwxrwxr-x   0 sayu      (1000) sayu      (1000)        0 2023-07-13 04:47:26.607671 danbooru-0.1.1/
+-rw-rw-r--   0 sayu      (1000) sayu      (1000)     1066 2023-07-13 03:34:40.000000 danbooru-0.1.1/LICENSE
+-rw-rw-r--   0 sayu      (1000) sayu      (1000)     1850 2023-07-13 04:47:26.607671 danbooru-0.1.1/PKG-INFO
+-rw-rw-r--   0 sayu      (1000) sayu      (1000)     1492 2023-07-13 03:34:40.000000 danbooru-0.1.1/README.md
+drwxrwxr-x   0 sayu      (1000) sayu      (1000)        0 2023-07-13 04:47:26.603671 danbooru-0.1.1/danbooru/
+-rw-rw-r--   0 sayu      (1000) sayu      (1000)       74 2023-07-13 04:47:09.000000 danbooru-0.1.1/danbooru/__init__.py
+-rw-rw-r--   0 sayu      (1000) sayu      (1000)      197 2023-07-13 04:43:55.000000 danbooru-0.1.1/danbooru/__vars__.py
+-rw-rw-r--   0 sayu      (1000) sayu      (1000)    11445 2023-07-13 04:42:41.000000 danbooru-0.1.1/danbooru/booru.py
+-rw-rw-r--   0 sayu      (1000) sayu      (1000)      946 2023-07-13 03:34:40.000000 danbooru-0.1.1/danbooru/exceptions.py
+drwxrwxr-x   0 sayu      (1000) sayu      (1000)        0 2023-07-13 04:47:26.607671 danbooru-0.1.1/danbooru/types/
+-rw-rw-r--   0 sayu      (1000) sayu      (1000)    20045 2023-07-13 03:38:20.000000 danbooru-0.1.1/danbooru/types/Danbooru_API.py
+-rw-rw-r--   0 sayu      (1000) sayu      (1000)     2555 2023-07-13 03:34:40.000000 danbooru-0.1.1/danbooru/types/Danbooru_Types.py
+-rw-rw-r--   0 sayu      (1000) sayu      (1000)        0 2023-07-13 03:34:40.000000 danbooru-0.1.1/danbooru/types/__init__.py
+drwxrwxr-x   0 sayu      (1000) sayu      (1000)        0 2023-07-13 04:47:26.607671 danbooru-0.1.1/danbooru.egg-info/
+-rw-rw-r--   0 sayu      (1000) sayu      (1000)     1850 2023-07-13 04:47:26.000000 danbooru-0.1.1/danbooru.egg-info/PKG-INFO
+-rw-rw-r--   0 sayu      (1000) sayu      (1000)      359 2023-07-13 04:47:26.000000 danbooru-0.1.1/danbooru.egg-info/SOURCES.txt
+-rw-rw-r--   0 sayu      (1000) sayu      (1000)        1 2023-07-13 04:47:26.000000 danbooru-0.1.1/danbooru.egg-info/dependency_links.txt
+-rw-rw-r--   0 sayu      (1000) sayu      (1000)       28 2023-07-13 04:47:26.000000 danbooru-0.1.1/danbooru.egg-info/requires.txt
+-rw-rw-r--   0 sayu      (1000) sayu      (1000)        9 2023-07-13 04:47:26.000000 danbooru-0.1.1/danbooru.egg-info/top_level.txt
+-rw-rw-r--   0 sayu      (1000) sayu      (1000)       38 2023-07-13 04:47:26.607671 danbooru-0.1.1/setup.cfg
+-rw-rw-r--   0 sayu      (1000) sayu      (1000)      654 2023-07-13 03:34:40.000000 danbooru-0.1.1/setup.py
```

### Comparing `danbooru-0.1.0/LICENSE` & `danbooru-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `danbooru-0.1.0/PKG-INFO` & `danbooru-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: danbooru
-Version: 0.1.0
+Version: 0.1.1
 Summary: Unofficial https://danbooru.donmai.us Package
 Home-page: https://github.com/TaprisSugarbell/Danbooru
 Author: SayuOgiwara
 Author-email: anonesayu@gmail.com
 Project-URL: Issue tracker, https://github.com/TaprisSugarbell/Danbooru/issues
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `danbooru-0.1.0/README.md` & `danbooru-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `danbooru-0.1.0/danbooru/booru.py` & `danbooru-0.1.1/danbooru/booru.py`

 * *Files identical despite different names*

### Comparing `danbooru-0.1.0/danbooru/exceptions.py` & `danbooru-0.1.1/danbooru/exceptions.py`

 * *Files identical despite different names*

### Comparing `danbooru-0.1.0/danbooru/types/Danbooru_API.py` & `danbooru-0.1.1/danbooru/types/Danbooru_API.py`

 * *Files identical despite different names*

### Comparing `danbooru-0.1.0/danbooru/types/Danbooru_Types.py` & `danbooru-0.1.1/danbooru/types/Danbooru_Types.py`

 * *Files identical despite different names*

### Comparing `danbooru-0.1.0/danbooru.egg-info/PKG-INFO` & `danbooru-0.1.1/danbooru.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: danbooru
-Version: 0.1.0
+Version: 0.1.1
 Summary: Unofficial https://danbooru.donmai.us Package
 Home-page: https://github.com/TaprisSugarbell/Danbooru
 Author: SayuOgiwara
 Author-email: anonesayu@gmail.com
 Project-URL: Issue tracker, https://github.com/TaprisSugarbell/Danbooru/issues
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `danbooru-0.1.0/setup.py` & `danbooru-0.1.1/setup.py`

 * *Files identical despite different names*

