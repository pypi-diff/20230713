# Comparing `tmp/meteo_hr-0.9.0.tar.gz` & `tmp/meteo_hr-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meteo_hr-0.9.0.tar", last modified: Fri Feb 10 14:15:27 2023, max compression
+gzip compressed data, was "meteo_hr-1.0.0.tar", last modified: Thu Jul 13 16:02:13 2023, max compression
```

## Comparing `meteo_hr-0.9.0.tar` & `meteo_hr-1.0.0.tar`

### file list

```diff
@@ -1,18 +1,22 @@
-drwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)        0 2023-02-10 14:15:27.733982 meteo_hr-0.9.0/
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)    35149 2022-07-28 08:59:43.000000 meteo_hr-0.9.0/LICENSE
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)    41418 2023-02-10 14:15:27.733982 meteo_hr-0.9.0/PKG-INFO
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      359 2022-07-30 06:55:32.000000 meteo_hr-0.9.0/README.md
-drwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)        0 2023-02-10 14:15:27.732982 meteo_hr-0.9.0/meteo_hr/
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     6401 2023-02-10 14:12:44.000000 meteo_hr-0.9.0/meteo_hr/__init__.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)       30 2022-07-28 08:44:10.000000 meteo_hr-0.9.0/meteo_hr/__main__.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      830 2022-07-30 13:45:44.000000 meteo_hr-0.9.0/meteo_hr/cli.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)    13968 2022-07-30 13:46:13.000000 meteo_hr-0.9.0/meteo_hr/places.py
-drwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)        0 2023-02-10 14:15:27.733982 meteo_hr-0.9.0/meteo_hr.egg-info/
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)    41418 2023-02-10 14:15:27.000000 meteo_hr-0.9.0/meteo_hr.egg-info/PKG-INFO
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      303 2023-02-10 14:15:27.000000 meteo_hr-0.9.0/meteo_hr.egg-info/SOURCES.txt
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)        1 2023-02-10 14:15:27.000000 meteo_hr-0.9.0/meteo_hr.egg-info/dependency_links.txt
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)       44 2023-02-10 14:15:27.000000 meteo_hr-0.9.0/meteo_hr.egg-info/entry_points.txt
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)       44 2023-02-10 14:15:27.000000 meteo_hr-0.9.0/meteo_hr.egg-info/requires.txt
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)        9 2023-02-10 14:15:27.000000 meteo_hr-0.9.0/meteo_hr.egg-info/top_level.txt
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      772 2023-02-10 14:13:50.000000 meteo_hr-0.9.0/pyproject.toml
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)       38 2023-02-10 14:15:27.733982 meteo_hr-0.9.0/setup.cfg
+drwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)        0 2023-07-13 16:02:13.513414 meteo_hr-1.0.0/
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)    35149 2022-07-28 08:59:43.000000 meteo_hr-1.0.0/LICENSE
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)    41535 2023-07-13 16:02:13.512414 meteo_hr-1.0.0/PKG-INFO
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      476 2023-07-13 15:59:25.000000 meteo_hr-1.0.0/README.md
+drwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)        0 2023-07-13 16:02:13.512414 meteo_hr-1.0.0/meteo_hr/
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      201 2023-07-13 15:55:45.000000 meteo_hr-1.0.0/meteo_hr/__init__.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)       30 2022-07-28 08:44:10.000000 meteo_hr-1.0.0/meteo_hr/__main__.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     2158 2023-07-13 15:50:29.000000 meteo_hr-1.0.0/meteo_hr/api.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     1944 2023-07-13 15:50:29.000000 meteo_hr-1.0.0/meteo_hr/cache.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     1567 2023-07-13 15:52:58.000000 meteo_hr-1.0.0/meteo_hr/cli.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     4884 2023-07-13 16:00:46.000000 meteo_hr-1.0.0/meteo_hr/output.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     2129 2023-07-13 15:54:59.000000 meteo_hr-1.0.0/meteo_hr/parse.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      638 2023-07-13 15:50:29.000000 meteo_hr-1.0.0/meteo_hr/places.py
+drwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)        0 2023-07-13 16:02:13.512414 meteo_hr-1.0.0/meteo_hr.egg-info/
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)    41535 2023-07-13 16:02:13.000000 meteo_hr-1.0.0/meteo_hr.egg-info/PKG-INFO
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      374 2023-07-13 16:02:13.000000 meteo_hr-1.0.0/meteo_hr.egg-info/SOURCES.txt
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)        1 2023-07-13 16:02:13.000000 meteo_hr-1.0.0/meteo_hr.egg-info/dependency_links.txt
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)       44 2023-07-13 16:02:13.000000 meteo_hr-1.0.0/meteo_hr.egg-info/entry_points.txt
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)       44 2023-07-13 16:02:13.000000 meteo_hr-1.0.0/meteo_hr.egg-info/requires.txt
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)        9 2023-07-13 16:02:13.000000 meteo_hr-1.0.0/meteo_hr.egg-info/top_level.txt
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      772 2023-07-13 16:01:44.000000 meteo_hr-1.0.0/pyproject.toml
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)       38 2023-07-13 16:02:13.513414 meteo_hr-1.0.0/setup.cfg
```

### Comparing `meteo_hr-0.9.0/LICENSE` & `meteo_hr-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `meteo_hr-0.9.0/PKG-INFO` & `meteo_hr-1.0.0/meteo_hr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: meteo_hr
-Version: 0.9.0
+Name: meteo-hr
+Version: 1.0.0
 Summary: CLI for printing weather forecast from meteo.hr
 Author-email: Ivan Habunek <ivan@habunek.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -686,15 +686,15 @@
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 meteo.hr CLI
 ============
 
-Commandline tool for displaying the [three-day forecast from meteo.hr](http://meteo.hr/prognoze.php?section=prognoze_model&param=3d).
+Commandline tool for displaying the forecast from [meteo.hr](http://meteo.hr/prognoze.php?section=prognoze_model&param=3d).
 
 Install:
 
 ```
 pip install --user meteo_hr
 ```
 
@@ -708,12 +708,25 @@
 
 ```
 meteo zagreb
 ```
 
 ![Forecast for Zagreb](forecast.png)
 
-List available places:
+7 day forecast:
+
+```
+meteo zagreb -7
+```
+
+
+List available places for 3 day forecast:
+
+```
+meteo --list
+```
+
+List available places for 7 day forecast:
 
 ```
 meteo --list
 ```
```

### Comparing `meteo_hr-0.9.0/meteo_hr.egg-info/PKG-INFO` & `meteo_hr-1.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: meteo-hr
-Version: 0.9.0
+Name: meteo_hr
+Version: 1.0.0
 Summary: CLI for printing weather forecast from meteo.hr
 Author-email: Ivan Habunek <ivan@habunek.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -686,15 +686,15 @@
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 meteo.hr CLI
 ============
 
-Commandline tool for displaying the [three-day forecast from meteo.hr](http://meteo.hr/prognoze.php?section=prognoze_model&param=3d).
+Commandline tool for displaying the forecast from [meteo.hr](http://meteo.hr/prognoze.php?section=prognoze_model&param=3d).
 
 Install:
 
 ```
 pip install --user meteo_hr
 ```
 
@@ -708,12 +708,25 @@
 
 ```
 meteo zagreb
 ```
 
 ![Forecast for Zagreb](forecast.png)
 
-List available places:
+7 day forecast:
+
+```
+meteo zagreb -7
+```
+
+
+List available places for 3 day forecast:
+
+```
+meteo --list
+```
+
+List available places for 7 day forecast:
 
 ```
 meteo --list
 ```
```

### Comparing `meteo_hr-0.9.0/pyproject.toml` & `meteo_hr-1.0.0/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "meteo_hr"
-version = "0.9.0"
+version = "1.0.0"
 authors = [{ name="Ivan Habunek", email="ivan@habunek.com" }]
 description = "CLI for printing weather forecast from meteo.hr"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
```

