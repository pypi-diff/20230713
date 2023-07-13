# Comparing `tmp/com-enovation-0.0.8.tar.gz` & `tmp/com-enovation-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "com-enovation-0.0.8.tar", last modified: Sun Sep 19 10:31:43 2021, max compression
+gzip compressed data, was "com-enovation-0.0.9.tar", last modified: Sun Sep 19 10:35:00 2021, max compression
```

## Comparing `com-enovation-0.0.8.tar` & `com-enovation-0.0.9.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 jsg        (501) staff       (20)        0 2021-09-19 10:31:43.522340 com-enovation-0.0.8/
--rw-r--r--   0 jsg        (501) staff       (20)      367 2021-05-30 14:38:00.000000 com-enovation-0.0.8/LICENSE
--rw-r--r--   0 jsg        (501) staff       (20)     3580 2021-09-19 10:31:43.522459 com-enovation-0.0.8/PKG-INFO
--rw-r--r--   0 jsg        (501) staff       (20)     2983 2021-09-19 07:24:01.000000 com-enovation-0.0.8/README.md
--rw-r--r--   0 jsg        (501) staff       (20)      103 2021-05-30 14:21:24.000000 com-enovation-0.0.8/pyproject.toml
--rw-r--r--   0 jsg        (501) staff       (20)      829 2021-09-19 10:31:43.523054 com-enovation-0.0.8/setup.cfg
-drwxr-xr-x   0 jsg        (501) staff       (20)        0 2021-09-19 10:31:43.506592 com-enovation-0.0.8/src/
-drwxr-xr-x   0 jsg        (501) staff       (20)        0 2021-09-19 10:31:43.508780 com-enovation-0.0.8/src/com/
--rw-r--r--   0 jsg        (501) staff       (20)        0 2021-05-30 14:19:10.000000 com-enovation-0.0.8/src/com/__init__.py
-drwxr-xr-x   0 jsg        (501) staff       (20)        0 2021-09-19 10:31:43.509302 com-enovation-0.0.8/src/com/enovation/
--rw-r--r--   0 jsg        (501) staff       (20)        0 2021-05-30 14:19:10.000000 com-enovation-0.0.8/src/com/enovation/__init__.py
--rw-r--r--   0 jsg        (501) staff       (20)     2274 2021-09-19 10:16:02.000000 com-enovation-0.0.8/src/com/enovation/enov.py
-drwxr-xr-x   0 jsg        (501) staff       (20)        0 2021-09-19 10:31:43.510509 com-enovation-0.0.8/src/com/enovation/helper/
--rw-r--r--   0 jsg        (501) staff       (20)        0 2021-06-13 09:02:23.000000 com-enovation-0.0.8/src/com/enovation/helper/__init__.py
-drwxr-xr-x   0 jsg        (501) staff       (20)        0 2021-09-19 10:31:43.513540 com-enovation-0.0.8/src/com/enovation/helper/click/
--rw-r--r--   0 jsg        (501) staff       (20)        0 2021-08-29 08:54:28.000000 com-enovation-0.0.8/src/com/enovation/helper/click/__init__.py
--rw-r--r--   0 jsg        (501) staff       (20)     4518 2021-09-05 07:48:59.000000 com-enovation-0.0.8/src/com/enovation/helper/click/df_load.py
--rw-r--r--   0 jsg        (501) staff       (20)     6280 2021-09-05 07:52:28.000000 com-enovation-0.0.8/src/com/enovation/helper/click/df_modify.py
--rw-r--r--   0 jsg        (501) staff       (20)     3113 2021-09-05 07:48:59.000000 com-enovation-0.0.8/src/com/enovation/helper/click/df_write.py
--rw-r--r--   0 jsg        (501) staff       (20)      521 2021-06-27 09:32:53.000000 com-enovation-0.0.8/src/com/enovation/helper/json_encoder.py
--rw-r--r--   0 jsg        (501) staff       (20)     4874 2021-08-30 08:55:58.000000 com-enovation-0.0.8/src/com/enovation/helper/pandas_dataframe_typer.py
-drwxr-xr-x   0 jsg        (501) staff       (20)        0 2021-09-19 10:31:43.514517 com-enovation-0.0.8/src/com/enovation/toolbox/
--rw-r--r--   0 jsg        (501) staff       (20)        0 2021-05-30 14:19:10.000000 com-enovation-0.0.8/src/com/enovation/toolbox/__init__.py
-drwxr-xr-x   0 jsg        (501) staff       (20)        0 2021-09-19 10:31:43.515018 com-enovation-0.0.8/src/com/enovation/toolbox/predictability/
--rw-r--r--   0 jsg        (501) staff       (20)        0 2021-08-16 14:31:44.000000 com-enovation-0.0.8/src/com/enovation/toolbox/predictability/__init__.py
--rw-r--r--   0 jsg        (501) staff       (20)     1179 2021-08-31 09:29:12.000000 com-enovation-0.0.8/src/com/enovation/toolbox/predictability/bean.py
-drwxr-xr-x   0 jsg        (501) staff       (20)        0 2021-09-19 10:31:43.517307 com-enovation-0.0.8/src/com/enovation/toolbox/predictability/click/
--rw-r--r--   0 jsg        (501) staff       (20)        0 2021-08-29 14:20:08.000000 com-enovation-0.0.8/src/com/enovation/toolbox/predictability/click/__init__.py
--rw-r--r--   0 jsg        (501) staff       (20)     2389 2021-09-05 14:20:53.000000 com-enovation-0.0.8/src/com/enovation/toolbox/predictability/click/compute.py
--rw-r--r--   0 jsg        (501) staff       (20)     1603 2021-09-05 14:57:44.000000 com-enovation-0.0.8/src/com/enovation/toolbox/predictability/click/graph.py
--rw-r--r--   0 jsg        (501) staff       (20)     2693 2021-09-18 14:29:29.000000 com-enovation-0.0.8/src/com/enovation/toolbox/predictability/click/persist.py
-drwxr-xr-x   0 jsg        (501) staff       (20)        0 2021-09-19 10:31:43.519989 com-enovation-0.0.8/src/com/enovation/toolbox/predictability/date_predictability/
--rw-r--r--   0 jsg        (501) staff       (20)        0 2021-08-17 16:01:08.000000 com-enovation-0.0.8/src/com/enovation/toolbox/predictability/date_predictability/__init__.py
--rw-r--r--   0 jsg        (501) staff       (20)    24040 2021-09-18 07:54:22.000000 com-enovation-0.0.8/src/com/enovation/toolbox/predictability/date_predictability/computer.py
--rw-r--r--   0 jsg        (501) staff       (20)     9922 2021-09-18 07:34:37.000000 com-enovation-0.0.8/src/com/enovation/toolbox/predictability/date_predictability/grapher.py
--rw-r--r--   0 jsg        (501) staff       (20)     9261 2021-09-18 14:24:48.000000 com-enovation-0.0.8/src/com/enovation/toolbox/predictability/date_predictability/persister.py
-drwxr-xr-x   0 jsg        (501) staff       (20)        0 2021-09-19 10:31:43.522101 com-enovation-0.0.8/src/com_enovation.egg-info/
--rw-r--r--   0 jsg        (501) staff       (20)     3580 2021-09-19 10:31:43.000000 com-enovation-0.0.8/src/com_enovation.egg-info/PKG-INFO
--rw-r--r--   0 jsg        (501) staff       (20)     1330 2021-09-19 10:31:43.000000 com-enovation-0.0.8/src/com_enovation.egg-info/SOURCES.txt
--rw-r--r--   0 jsg        (501) staff       (20)        1 2021-09-19 10:31:43.000000 com-enovation-0.0.8/src/com_enovation.egg-info/dependency_links.txt
--rw-r--r--   0 jsg        (501) staff       (20)       50 2021-09-19 10:31:43.000000 com-enovation-0.0.8/src/com_enovation.egg-info/entry_points.txt
--rw-r--r--   0 jsg        (501) staff       (20)       43 2021-09-19 10:31:43.000000 com-enovation-0.0.8/src/com_enovation.egg-info/requires.txt
--rw-r--r--   0 jsg        (501) staff       (20)        4 2021-09-19 10:31:43.000000 com-enovation-0.0.8/src/com_enovation.egg-info/top_level.txt
+drwxr-xr-x   0 jsg        (501) staff       (20)        0 2021-09-19 10:35:00.001765 com-enovation-0.0.9/
+-rw-r--r--   0 jsg        (501) staff       (20)      367 2021-05-30 14:38:00.000000 com-enovation-0.0.9/LICENSE
+-rw-r--r--   0 jsg        (501) staff       (20)     3580 2021-09-19 10:35:00.002014 com-enovation-0.0.9/PKG-INFO
+-rw-r--r--   0 jsg        (501) staff       (20)     2983 2021-09-19 07:24:01.000000 com-enovation-0.0.9/README.md
+-rw-r--r--   0 jsg        (501) staff       (20)      103 2021-05-30 14:21:24.000000 com-enovation-0.0.9/pyproject.toml
+-rw-r--r--   0 jsg        (501) staff       (20)      829 2021-09-19 10:35:00.003328 com-enovation-0.0.9/setup.cfg
+drwxr-xr-x   0 jsg        (501) staff       (20)        0 2021-09-19 10:34:59.988286 com-enovation-0.0.9/src/
+drwxr-xr-x   0 jsg        (501) staff       (20)        0 2021-09-19 10:34:59.990145 com-enovation-0.0.9/src/com/
+-rw-r--r--   0 jsg        (501) staff       (20)        0 2021-05-30 14:19:10.000000 com-enovation-0.0.9/src/com/__init__.py
+drwxr-xr-x   0 jsg        (501) staff       (20)        0 2021-09-19 10:34:59.990844 com-enovation-0.0.9/src/com/enovation/
+-rw-r--r--   0 jsg        (501) staff       (20)        0 2021-05-30 14:19:10.000000 com-enovation-0.0.9/src/com/enovation/__init__.py
+-rw-r--r--   0 jsg        (501) staff       (20)     2274 2021-09-19 10:16:02.000000 com-enovation-0.0.9/src/com/enovation/enov.py
+drwxr-xr-x   0 jsg        (501) staff       (20)        0 2021-09-19 10:34:59.992218 com-enovation-0.0.9/src/com/enovation/helper/
+-rw-r--r--   0 jsg        (501) staff       (20)        0 2021-06-13 09:02:23.000000 com-enovation-0.0.9/src/com/enovation/helper/__init__.py
+drwxr-xr-x   0 jsg        (501) staff       (20)        0 2021-09-19 10:34:59.993685 com-enovation-0.0.9/src/com/enovation/helper/click/
+-rw-r--r--   0 jsg        (501) staff       (20)        0 2021-08-29 08:54:28.000000 com-enovation-0.0.9/src/com/enovation/helper/click/__init__.py
+-rw-r--r--   0 jsg        (501) staff       (20)     4518 2021-09-05 07:48:59.000000 com-enovation-0.0.9/src/com/enovation/helper/click/df_load.py
+-rw-r--r--   0 jsg        (501) staff       (20)     6280 2021-09-05 07:52:28.000000 com-enovation-0.0.9/src/com/enovation/helper/click/df_modify.py
+-rw-r--r--   0 jsg        (501) staff       (20)     3113 2021-09-05 07:48:59.000000 com-enovation-0.0.9/src/com/enovation/helper/click/df_write.py
+-rw-r--r--   0 jsg        (501) staff       (20)      521 2021-06-27 09:32:53.000000 com-enovation-0.0.9/src/com/enovation/helper/json_encoder.py
+-rw-r--r--   0 jsg        (501) staff       (20)     4874 2021-08-30 08:55:58.000000 com-enovation-0.0.9/src/com/enovation/helper/pandas_dataframe_typer.py
+drwxr-xr-x   0 jsg        (501) staff       (20)        0 2021-09-19 10:34:59.994218 com-enovation-0.0.9/src/com/enovation/toolbox/
+-rw-r--r--   0 jsg        (501) staff       (20)        0 2021-05-30 14:19:10.000000 com-enovation-0.0.9/src/com/enovation/toolbox/__init__.py
+drwxr-xr-x   0 jsg        (501) staff       (20)        0 2021-09-19 10:34:59.994830 com-enovation-0.0.9/src/com/enovation/toolbox/predictability/
+-rw-r--r--   0 jsg        (501) staff       (20)        0 2021-08-16 14:31:44.000000 com-enovation-0.0.9/src/com/enovation/toolbox/predictability/__init__.py
+-rw-r--r--   0 jsg        (501) staff       (20)     1179 2021-08-31 09:29:12.000000 com-enovation-0.0.9/src/com/enovation/toolbox/predictability/bean.py
+drwxr-xr-x   0 jsg        (501) staff       (20)        0 2021-09-19 10:34:59.996501 com-enovation-0.0.9/src/com/enovation/toolbox/predictability/click/
+-rw-r--r--   0 jsg        (501) staff       (20)        0 2021-08-29 14:20:08.000000 com-enovation-0.0.9/src/com/enovation/toolbox/predictability/click/__init__.py
+-rw-r--r--   0 jsg        (501) staff       (20)     2389 2021-09-05 14:20:53.000000 com-enovation-0.0.9/src/com/enovation/toolbox/predictability/click/compute.py
+-rw-r--r--   0 jsg        (501) staff       (20)     1603 2021-09-05 14:57:44.000000 com-enovation-0.0.9/src/com/enovation/toolbox/predictability/click/graph.py
+-rw-r--r--   0 jsg        (501) staff       (20)     2693 2021-09-18 14:29:29.000000 com-enovation-0.0.9/src/com/enovation/toolbox/predictability/click/persist.py
+drwxr-xr-x   0 jsg        (501) staff       (20)        0 2021-09-19 10:34:59.998476 com-enovation-0.0.9/src/com/enovation/toolbox/predictability/date_predictability/
+-rw-r--r--   0 jsg        (501) staff       (20)        0 2021-08-17 16:01:08.000000 com-enovation-0.0.9/src/com/enovation/toolbox/predictability/date_predictability/__init__.py
+-rw-r--r--   0 jsg        (501) staff       (20)    24040 2021-09-18 07:54:22.000000 com-enovation-0.0.9/src/com/enovation/toolbox/predictability/date_predictability/computer.py
+-rw-r--r--   0 jsg        (501) staff       (20)     9922 2021-09-18 07:34:37.000000 com-enovation-0.0.9/src/com/enovation/toolbox/predictability/date_predictability/grapher.py
+-rw-r--r--   0 jsg        (501) staff       (20)     9261 2021-09-18 14:24:48.000000 com-enovation-0.0.9/src/com/enovation/toolbox/predictability/date_predictability/persister.py
+drwxr-xr-x   0 jsg        (501) staff       (20)        0 2021-09-19 10:35:00.001326 com-enovation-0.0.9/src/com_enovation.egg-info/
+-rw-r--r--   0 jsg        (501) staff       (20)     3580 2021-09-19 10:34:59.000000 com-enovation-0.0.9/src/com_enovation.egg-info/PKG-INFO
+-rw-r--r--   0 jsg        (501) staff       (20)     1330 2021-09-19 10:34:59.000000 com-enovation-0.0.9/src/com_enovation.egg-info/SOURCES.txt
+-rw-r--r--   0 jsg        (501) staff       (20)        1 2021-09-19 10:34:59.000000 com-enovation-0.0.9/src/com_enovation.egg-info/dependency_links.txt
+-rw-r--r--   0 jsg        (501) staff       (20)       50 2021-09-19 10:34:59.000000 com-enovation-0.0.9/src/com_enovation.egg-info/entry_points.txt
+-rw-r--r--   0 jsg        (501) staff       (20)       43 2021-09-19 10:34:59.000000 com-enovation-0.0.9/src/com_enovation.egg-info/requires.txt
+-rw-r--r--   0 jsg        (501) staff       (20)        4 2021-09-19 10:34:59.000000 com-enovation-0.0.9/src/com_enovation.egg-info/top_level.txt
```

### Comparing `com-enovation-0.0.8/PKG-INFO` & `com-enovation-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: com-enovation
-Version: 0.0.8
+Version: 0.0.9
 Summary: project management toolbox
 Home-page: https://jsebastien_Guillard@bitbucket.org/jsebastien_Guillard
 Author: jean-sebastien guillard
 Author-email: jsebastien.guillard@gmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://jsebastien_Guillard@bitbucket.org/jsebastien_Guillard
 Platform: UNKNOWN
```

### Comparing `com-enovation-0.0.8/README.md` & `com-enovation-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `com-enovation-0.0.8/setup.cfg` & `com-enovation-0.0.9/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = com-enovation
-version = 0.0.8
+version = 0.0.9
 author = jean-sebastien guillard
 author_email = jsebastien.guillard@gmail.com
 description = project management toolbox
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://jsebastien_Guillard@bitbucket.org/jsebastien_Guillard
 project_urls = 
@@ -28,13 +28,13 @@
 python_requires = >=3.6
 
 [options.packages.find]
 where = src
 
 [options.entry_points]
 console_scripts = 
-	enov = com.enovation.enov:main
+	enov = com.enovation.enov:enov
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `com-enovation-0.0.8/src/com/enovation/enov.py` & `com-enovation-0.0.9/src/com/enovation/enov.py`

 * *Files identical despite different names*

### Comparing `com-enovation-0.0.8/src/com/enovation/helper/click/df_load.py` & `com-enovation-0.0.9/src/com/enovation/helper/click/df_load.py`

 * *Files identical despite different names*

### Comparing `com-enovation-0.0.8/src/com/enovation/helper/click/df_modify.py` & `com-enovation-0.0.9/src/com/enovation/helper/click/df_modify.py`

 * *Files identical despite different names*

### Comparing `com-enovation-0.0.8/src/com/enovation/helper/click/df_write.py` & `com-enovation-0.0.9/src/com/enovation/helper/click/df_write.py`

 * *Files identical despite different names*

### Comparing `com-enovation-0.0.8/src/com/enovation/helper/json_encoder.py` & `com-enovation-0.0.9/src/com/enovation/helper/json_encoder.py`

 * *Files identical despite different names*

### Comparing `com-enovation-0.0.8/src/com/enovation/helper/pandas_dataframe_typer.py` & `com-enovation-0.0.9/src/com/enovation/helper/pandas_dataframe_typer.py`

 * *Files identical despite different names*

### Comparing `com-enovation-0.0.8/src/com/enovation/toolbox/predictability/bean.py` & `com-enovation-0.0.9/src/com/enovation/toolbox/predictability/bean.py`

 * *Files identical despite different names*

### Comparing `com-enovation-0.0.8/src/com/enovation/toolbox/predictability/click/compute.py` & `com-enovation-0.0.9/src/com/enovation/toolbox/predictability/click/compute.py`

 * *Files identical despite different names*

### Comparing `com-enovation-0.0.8/src/com/enovation/toolbox/predictability/click/graph.py` & `com-enovation-0.0.9/src/com/enovation/toolbox/predictability/click/graph.py`

 * *Files identical despite different names*

### Comparing `com-enovation-0.0.8/src/com/enovation/toolbox/predictability/click/persist.py` & `com-enovation-0.0.9/src/com/enovation/toolbox/predictability/click/persist.py`

 * *Files identical despite different names*

### Comparing `com-enovation-0.0.8/src/com/enovation/toolbox/predictability/date_predictability/computer.py` & `com-enovation-0.0.9/src/com/enovation/toolbox/predictability/date_predictability/computer.py`

 * *Files identical despite different names*

### Comparing `com-enovation-0.0.8/src/com/enovation/toolbox/predictability/date_predictability/grapher.py` & `com-enovation-0.0.9/src/com/enovation/toolbox/predictability/date_predictability/grapher.py`

 * *Files identical despite different names*

### Comparing `com-enovation-0.0.8/src/com/enovation/toolbox/predictability/date_predictability/persister.py` & `com-enovation-0.0.9/src/com/enovation/toolbox/predictability/date_predictability/persister.py`

 * *Files identical despite different names*

### Comparing `com-enovation-0.0.8/src/com_enovation.egg-info/PKG-INFO` & `com-enovation-0.0.9/src/com_enovation.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: com-enovation
-Version: 0.0.8
+Version: 0.0.9
 Summary: project management toolbox
 Home-page: https://jsebastien_Guillard@bitbucket.org/jsebastien_Guillard
 Author: jean-sebastien guillard
 Author-email: jsebastien.guillard@gmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://jsebastien_Guillard@bitbucket.org/jsebastien_Guillard
 Platform: UNKNOWN
```

### Comparing `com-enovation-0.0.8/src/com_enovation.egg-info/SOURCES.txt` & `com-enovation-0.0.9/src/com_enovation.egg-info/SOURCES.txt`

 * *Files identical despite different names*

