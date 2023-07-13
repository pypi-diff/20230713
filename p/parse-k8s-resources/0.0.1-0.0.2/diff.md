# Comparing `tmp/parse-k8s-resources-0.0.1.tar.gz` & `tmp/parse-k8s-resources-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "parse-k8s-resources-0.0.1.tar", last modified: Thu Jul 13 08:04:42 2023, max compression
+gzip compressed data, was "parse-k8s-resources-0.0.2.tar", last modified: Thu Jul 13 08:16:06 2023, max compression
```

## Comparing `parse-k8s-resources-0.0.1.tar` & `parse-k8s-resources-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 weizheng   (501) staff       (20)        0 2023-07-13 08:04:42.646421 parse-k8s-resources-0.0.1/
--rw-r--r--   0 weizheng   (501) staff       (20)      132 2023-07-13 07:45:31.000000 parse-k8s-resources-0.0.1/MANIFEST.in
--rw-r--r--   0 weizheng   (501) staff       (20)      912 2023-07-13 08:04:42.646544 parse-k8s-resources-0.0.1/PKG-INFO
--rw-r--r--   0 weizheng   (501) staff       (20)        0 2023-07-13 07:50:02.000000 parse-k8s-resources-0.0.1/README.md
-drwxr-xr-x   0 weizheng   (501) staff       (20)        0 2023-07-13 08:04:42.644323 parse-k8s-resources-0.0.1/parse_k8s_resources/
--rw-r--r--   0 weizheng   (501) staff       (20)      169 2023-07-13 07:42:25.000000 parse-k8s-resources-0.0.1/parse_k8s_resources/__init__.py
--rw-r--r--   0 weizheng   (501) staff       (20)     5193 2023-07-13 08:00:27.000000 parse-k8s-resources-0.0.1/parse_k8s_resources/main.py
-drwxr-xr-x   0 weizheng   (501) staff       (20)        0 2023-07-13 08:04:42.646063 parse-k8s-resources-0.0.1/parse_k8s_resources.egg-info/
--rw-r--r--   0 weizheng   (501) staff       (20)      912 2023-07-13 08:04:42.000000 parse-k8s-resources-0.0.1/parse_k8s_resources.egg-info/PKG-INFO
--rw-r--r--   0 weizheng   (501) staff       (20)      377 2023-07-13 08:04:42.000000 parse-k8s-resources-0.0.1/parse_k8s_resources.egg-info/SOURCES.txt
--rw-r--r--   0 weizheng   (501) staff       (20)        1 2023-07-13 08:04:42.000000 parse-k8s-resources-0.0.1/parse_k8s_resources.egg-info/dependency_links.txt
--rw-r--r--   0 weizheng   (501) staff       (20)       70 2023-07-13 08:04:42.000000 parse-k8s-resources-0.0.1/parse_k8s_resources.egg-info/entry_points.txt
--rw-r--r--   0 weizheng   (501) staff       (20)       35 2023-07-13 08:04:42.000000 parse-k8s-resources-0.0.1/parse_k8s_resources.egg-info/requires.txt
--rw-r--r--   0 weizheng   (501) staff       (20)       20 2023-07-13 08:04:42.000000 parse-k8s-resources-0.0.1/parse_k8s_resources.egg-info/top_level.txt
--rw-r--r--   0 weizheng   (501) staff       (20)       34 2023-07-13 07:49:28.000000 parse-k8s-resources-0.0.1/requirements.txt
--rw-r--r--   0 weizheng   (501) staff       (20)      159 2023-07-13 08:04:42.646971 parse-k8s-resources-0.0.1/setup.cfg
--rw-r--r--   0 weizheng   (501) staff       (20)     2674 2023-07-13 08:04:08.000000 parse-k8s-resources-0.0.1/setup.py
+drwxr-xr-x   0 weizheng   (501) staff       (20)        0 2023-07-13 08:16:06.553757 parse-k8s-resources-0.0.2/
+-rw-r--r--   0 weizheng   (501) staff       (20)      132 2023-07-13 07:45:31.000000 parse-k8s-resources-0.0.2/MANIFEST.in
+-rw-r--r--   0 weizheng   (501) staff       (20)      912 2023-07-13 08:16:06.553900 parse-k8s-resources-0.0.2/PKG-INFO
+-rw-r--r--   0 weizheng   (501) staff       (20)        0 2023-07-13 07:50:02.000000 parse-k8s-resources-0.0.2/README.md
+drwxr-xr-x   0 weizheng   (501) staff       (20)        0 2023-07-13 08:16:06.551180 parse-k8s-resources-0.0.2/parse_k8s_resources/
+-rw-r--r--   0 weizheng   (501) staff       (20)      169 2023-07-13 08:16:03.000000 parse-k8s-resources-0.0.2/parse_k8s_resources/__init__.py
+-rw-r--r--   0 weizheng   (501) staff       (20)     5193 2023-07-13 08:00:27.000000 parse-k8s-resources-0.0.2/parse_k8s_resources/main.py
+drwxr-xr-x   0 weizheng   (501) staff       (20)        0 2023-07-13 08:16:06.553497 parse-k8s-resources-0.0.2/parse_k8s_resources.egg-info/
+-rw-r--r--   0 weizheng   (501) staff       (20)      912 2023-07-13 08:16:06.000000 parse-k8s-resources-0.0.2/parse_k8s_resources.egg-info/PKG-INFO
+-rw-r--r--   0 weizheng   (501) staff       (20)      377 2023-07-13 08:16:06.000000 parse-k8s-resources-0.0.2/parse_k8s_resources.egg-info/SOURCES.txt
+-rw-r--r--   0 weizheng   (501) staff       (20)        1 2023-07-13 08:16:06.000000 parse-k8s-resources-0.0.2/parse_k8s_resources.egg-info/dependency_links.txt
+-rw-r--r--   0 weizheng   (501) staff       (20)       70 2023-07-13 08:16:06.000000 parse-k8s-resources-0.0.2/parse_k8s_resources.egg-info/entry_points.txt
+-rw-r--r--   0 weizheng   (501) staff       (20)       35 2023-07-13 08:16:06.000000 parse-k8s-resources-0.0.2/parse_k8s_resources.egg-info/requires.txt
+-rw-r--r--   0 weizheng   (501) staff       (20)       20 2023-07-13 08:16:06.000000 parse-k8s-resources-0.0.2/parse_k8s_resources.egg-info/top_level.txt
+-rw-r--r--   0 weizheng   (501) staff       (20)       34 2023-07-13 08:15:34.000000 parse-k8s-resources-0.0.2/requirements.txt
+-rw-r--r--   0 weizheng   (501) staff       (20)      159 2023-07-13 08:16:06.554424 parse-k8s-resources-0.0.2/setup.cfg
+-rw-r--r--   0 weizheng   (501) staff       (20)     2674 2023-07-13 08:04:08.000000 parse-k8s-resources-0.0.2/setup.py
```

### Comparing `parse-k8s-resources-0.0.1/PKG-INFO` & `parse-k8s-resources-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: parse-k8s-resources
-Version: 0.0.1
+Version: 0.0.2
 Summary: parse k8s resource
 Home-page: 
 Author: harvey
 Author-email: harveyzhwei@gmail.com
 License: MIT
 Keywords: kubectl,Kubernetes
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `parse-k8s-resources-0.0.1/parse_k8s_resources/main.py` & `parse-k8s-resources-0.0.2/parse_k8s_resources/main.py`

 * *Files identical despite different names*

### Comparing `parse-k8s-resources-0.0.1/parse_k8s_resources.egg-info/PKG-INFO` & `parse-k8s-resources-0.0.2/parse_k8s_resources.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: parse-k8s-resources
-Version: 0.0.1
+Version: 0.0.2
 Summary: parse k8s resource
 Home-page: 
 Author: harvey
 Author-email: harveyzhwei@gmail.com
 License: MIT
 Keywords: kubectl,Kubernetes
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `parse-k8s-resources-0.0.1/setup.py` & `parse-k8s-resources-0.0.2/setup.py`

 * *Files identical despite different names*

