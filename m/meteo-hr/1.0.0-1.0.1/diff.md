# Comparing `tmp/meteo_hr-1.0.0.tar.gz` & `tmp/meteo_hr-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meteo_hr-1.0.0.tar", last modified: Thu Jul 13 16:02:13 2023, max compression
+gzip compressed data, was "meteo_hr-1.0.1.tar", last modified: Thu Jul 13 16:05:38 2023, max compression
```

## Comparing `meteo_hr-1.0.0.tar` & `meteo_hr-1.0.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)        0 2023-07-13 16:02:13.513414 meteo_hr-1.0.0/
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)    35149 2022-07-28 08:59:43.000000 meteo_hr-1.0.0/LICENSE
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)    41535 2023-07-13 16:02:13.512414 meteo_hr-1.0.0/PKG-INFO
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      476 2023-07-13 15:59:25.000000 meteo_hr-1.0.0/README.md
-drwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)        0 2023-07-13 16:02:13.512414 meteo_hr-1.0.0/meteo_hr/
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      201 2023-07-13 15:55:45.000000 meteo_hr-1.0.0/meteo_hr/__init__.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)       30 2022-07-28 08:44:10.000000 meteo_hr-1.0.0/meteo_hr/__main__.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     2158 2023-07-13 15:50:29.000000 meteo_hr-1.0.0/meteo_hr/api.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     1944 2023-07-13 15:50:29.000000 meteo_hr-1.0.0/meteo_hr/cache.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     1567 2023-07-13 15:52:58.000000 meteo_hr-1.0.0/meteo_hr/cli.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     4884 2023-07-13 16:00:46.000000 meteo_hr-1.0.0/meteo_hr/output.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     2129 2023-07-13 15:54:59.000000 meteo_hr-1.0.0/meteo_hr/parse.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      638 2023-07-13 15:50:29.000000 meteo_hr-1.0.0/meteo_hr/places.py
-drwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)        0 2023-07-13 16:02:13.512414 meteo_hr-1.0.0/meteo_hr.egg-info/
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)    41535 2023-07-13 16:02:13.000000 meteo_hr-1.0.0/meteo_hr.egg-info/PKG-INFO
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      374 2023-07-13 16:02:13.000000 meteo_hr-1.0.0/meteo_hr.egg-info/SOURCES.txt
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)        1 2023-07-13 16:02:13.000000 meteo_hr-1.0.0/meteo_hr.egg-info/dependency_links.txt
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)       44 2023-07-13 16:02:13.000000 meteo_hr-1.0.0/meteo_hr.egg-info/entry_points.txt
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)       44 2023-07-13 16:02:13.000000 meteo_hr-1.0.0/meteo_hr.egg-info/requires.txt
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)        9 2023-07-13 16:02:13.000000 meteo_hr-1.0.0/meteo_hr.egg-info/top_level.txt
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      772 2023-07-13 16:01:44.000000 meteo_hr-1.0.0/pyproject.toml
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)       38 2023-07-13 16:02:13.513414 meteo_hr-1.0.0/setup.cfg
+drwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)        0 2023-07-13 16:05:38.669741 meteo_hr-1.0.1/
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)    35149 2022-07-28 08:59:43.000000 meteo_hr-1.0.1/LICENSE
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)    41535 2023-07-13 16:05:38.668741 meteo_hr-1.0.1/PKG-INFO
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      476 2023-07-13 15:59:25.000000 meteo_hr-1.0.1/README.md
+drwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)        0 2023-07-13 16:05:38.668741 meteo_hr-1.0.1/meteo_hr/
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      201 2023-07-13 15:55:45.000000 meteo_hr-1.0.1/meteo_hr/__init__.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)       30 2022-07-28 08:44:10.000000 meteo_hr-1.0.1/meteo_hr/__main__.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     2158 2023-07-13 15:50:29.000000 meteo_hr-1.0.1/meteo_hr/api.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     1944 2023-07-13 15:50:29.000000 meteo_hr-1.0.1/meteo_hr/cache.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     1567 2023-07-13 15:52:58.000000 meteo_hr-1.0.1/meteo_hr/cli.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     4979 2023-07-13 16:03:32.000000 meteo_hr-1.0.1/meteo_hr/output.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     2129 2023-07-13 15:54:59.000000 meteo_hr-1.0.1/meteo_hr/parse.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      638 2023-07-13 15:50:29.000000 meteo_hr-1.0.1/meteo_hr/places.py
+drwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)        0 2023-07-13 16:05:38.668741 meteo_hr-1.0.1/meteo_hr.egg-info/
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)    41535 2023-07-13 16:05:38.000000 meteo_hr-1.0.1/meteo_hr.egg-info/PKG-INFO
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      374 2023-07-13 16:05:38.000000 meteo_hr-1.0.1/meteo_hr.egg-info/SOURCES.txt
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)        1 2023-07-13 16:05:38.000000 meteo_hr-1.0.1/meteo_hr.egg-info/dependency_links.txt
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)       44 2023-07-13 16:05:38.000000 meteo_hr-1.0.1/meteo_hr.egg-info/entry_points.txt
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)       44 2023-07-13 16:05:38.000000 meteo_hr-1.0.1/meteo_hr.egg-info/requires.txt
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)        9 2023-07-13 16:05:38.000000 meteo_hr-1.0.1/meteo_hr.egg-info/top_level.txt
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      772 2023-07-13 16:05:06.000000 meteo_hr-1.0.1/pyproject.toml
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)       38 2023-07-13 16:05:38.669741 meteo_hr-1.0.1/setup.cfg
```

### Comparing `meteo_hr-1.0.0/LICENSE` & `meteo_hr-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `meteo_hr-1.0.0/PKG-INFO` & `meteo_hr-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meteo_hr
-Version: 1.0.0
+Version: 1.0.1
 Summary: CLI for printing weather forecast from meteo.hr
 Author-email: Ivan Habunek <ivan@habunek.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `meteo_hr-1.0.0/meteo_hr/api.py` & `meteo_hr-1.0.1/meteo_hr/api.py`

 * *Files identical despite different names*

### Comparing `meteo_hr-1.0.0/meteo_hr/cache.py` & `meteo_hr-1.0.1/meteo_hr/cache.py`

 * *Files identical despite different names*

### Comparing `meteo_hr-1.0.0/meteo_hr/cli.py` & `meteo_hr-1.0.1/meteo_hr/cli.py`

 * *Files identical despite different names*

### Comparing `meteo_hr-1.0.0/meteo_hr/output.py` & `meteo_hr-1.0.1/meteo_hr/output.py`

 * *Files 1% similar despite different names*

```diff
@@ -104,16 +104,17 @@
 
 
 WEATHER_ICONS = {
     "magla, malo do umjereno oblačno": "\N{fog}\N{fog}",
     "magla, nebo vedro": "\N{fog}\uFE0F",
     "malo oblačno, danju sunčano": "\N{white sun with small cloud}\uFE0F",
     "oblačno i maglovito": "\N{cloud}\uFE0F",
-    "oblačno uz malu količinu kiše": "\N{white sun behind cloud with rain}\uFE0F",
     "oblačno uz malu količinu kiše te moguću grmljavinu": "\N{white sun behind cloud with rain}\uFE0F",
+    "oblačno uz malu količinu kiše": "\N{white sun behind cloud with rain}\uFE0F",
+    "oblačno uz umjerenu količinu kiše te moguću grmljavinu": "\N{cloud with rain}\uFE0F",
     "oblačno uz umjerenu količinu kiše": "\N{cloud with rain}\uFE0F",
     "oblačno uz znatnu količinu kiše te moguću grmljavinu": "\N{thunder cloud and rain}\uFE0F",
     "oblačno uz znatnu količinu kiše": "\N{cloud with rain}\uFE0F",
     "oblačno": "\N{cloud}\uFE0F",
     "pretežno oblačno": "\N{cloud}\uFE0F",
     "promjenljivo oblačno uz malu količinu kiše": "\N{white sun behind cloud with rain}\uFE0F",
     "promjenljivo oblačno uz moguću grmljavinu": "\N{cloud with lightning}\uFE0F",
```

### Comparing `meteo_hr-1.0.0/meteo_hr/parse.py` & `meteo_hr-1.0.1/meteo_hr/parse.py`

 * *Files identical despite different names*

### Comparing `meteo_hr-1.0.0/meteo_hr/places.py` & `meteo_hr-1.0.1/meteo_hr/places.py`

 * *Files identical despite different names*

### Comparing `meteo_hr-1.0.0/meteo_hr.egg-info/PKG-INFO` & `meteo_hr-1.0.1/meteo_hr.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meteo-hr
-Version: 1.0.0
+Version: 1.0.1
 Summary: CLI for printing weather forecast from meteo.hr
 Author-email: Ivan Habunek <ivan@habunek.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `meteo_hr-1.0.0/pyproject.toml` & `meteo_hr-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "meteo_hr"
-version = "1.0.0"
+version = "1.0.1"
 authors = [{ name="Ivan Habunek", email="ivan@habunek.com" }]
 description = "CLI for printing weather forecast from meteo.hr"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
```

