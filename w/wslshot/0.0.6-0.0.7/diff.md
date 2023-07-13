# Comparing `tmp/wslshot-0.0.6.tar.gz` & `tmp/wslshot-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wslshot-0.0.6.tar", last modified: Thu Jul 13 12:05:14 2023, max compression
+gzip compressed data, was "wslshot-0.0.7.tar", last modified: Thu Jul 13 12:07:41 2023, max compression
```

## Comparing `wslshot-0.0.6.tar` & `wslshot-0.0.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-07-13 12:05:14.497689 wslshot-0.0.6/
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)    11357 2023-07-07 11:34:57.000000 wslshot-0.0.6/LICENSE
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)     6782 2023-07-13 12:05:14.497689 wslshot-0.0.6/PKG-INFO
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)     6342 2023-07-13 11:15:32.000000 wslshot-0.0.6/README.md
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)       38 2023-07-13 12:05:14.497689 wslshot-0.0.6/setup.cfg
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      990 2023-07-13 12:04:39.000000 wslshot-0.0.6/setup.py
-drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-07-13 12:05:14.497689 wslshot-0.0.6/wslshot/
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)        0 2023-07-07 12:41:35.000000 wslshot-0.0.6/wslshot/__init__.py
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)    16184 2023-07-13 12:01:49.000000 wslshot-0.0.6/wslshot/cli.py
-drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-07-13 12:05:14.497689 wslshot-0.0.6/wslshot.egg-info/
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)     6782 2023-07-13 12:05:14.000000 wslshot-0.0.6/wslshot.egg-info/PKG-INFO
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      249 2023-07-13 12:05:14.000000 wslshot-0.0.6/wslshot.egg-info/SOURCES.txt
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)        1 2023-07-13 12:05:14.000000 wslshot-0.0.6/wslshot.egg-info/dependency_links.txt
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)       48 2023-07-13 12:05:14.000000 wslshot-0.0.6/wslshot.egg-info/entry_points.txt
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)        6 2023-07-13 12:05:14.000000 wslshot-0.0.6/wslshot.egg-info/requires.txt
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)        8 2023-07-13 12:05:14.000000 wslshot-0.0.6/wslshot.egg-info/top_level.txt
+drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-07-13 12:07:41.937688 wslshot-0.0.7/
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)    11357 2023-07-07 11:34:57.000000 wslshot-0.0.7/LICENSE
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)     6782 2023-07-13 12:07:41.937688 wslshot-0.0.7/PKG-INFO
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)     6342 2023-07-13 11:15:32.000000 wslshot-0.0.7/README.md
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)       38 2023-07-13 12:07:41.937688 wslshot-0.0.7/setup.cfg
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      990 2023-07-13 12:06:37.000000 wslshot-0.0.7/setup.py
+drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-07-13 12:07:41.937688 wslshot-0.0.7/wslshot/
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)        0 2023-07-07 12:41:35.000000 wslshot-0.0.7/wslshot/__init__.py
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)    16138 2023-07-13 12:06:28.000000 wslshot-0.0.7/wslshot/cli.py
+drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-07-13 12:07:41.937688 wslshot-0.0.7/wslshot.egg-info/
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)     6782 2023-07-13 12:07:41.000000 wslshot-0.0.7/wslshot.egg-info/PKG-INFO
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      249 2023-07-13 12:07:41.000000 wslshot-0.0.7/wslshot.egg-info/SOURCES.txt
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)        1 2023-07-13 12:07:41.000000 wslshot-0.0.7/wslshot.egg-info/dependency_links.txt
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)       48 2023-07-13 12:07:41.000000 wslshot-0.0.7/wslshot.egg-info/entry_points.txt
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)        6 2023-07-13 12:07:41.000000 wslshot-0.0.7/wslshot.egg-info/requires.txt
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)        8 2023-07-13 12:07:41.000000 wslshot-0.0.7/wslshot.egg-info/top_level.txt
```

### Comparing `wslshot-0.0.6/LICENSE` & `wslshot-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `wslshot-0.0.6/PKG-INFO` & `wslshot-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wslshot
-Version: 0.0.6
+Version: 0.0.7
 Home-page: https://github.com/sderev/wslshot
 Author: Sébastien De Revière
 License: Apache Licence, Version 2.0
 Project-URL: Documentation, https://github.com/sderev/wslshot
 Project-URL: Issues, http://github.com/sderev/wslshot/issues
 Project-URL: Changelog, https://github.com/sderev/wslshot/releases
 Requires-Python: >=3.8
```

### Comparing `wslshot-0.0.6/README.md` & `wslshot-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `wslshot-0.0.6/setup.py` & `wslshot-0.0.7/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 
 
-VERSION = "0.0.6"
+VERSION = "0.0.7"
 
 
 def read_requirements():
     with open("requirements.txt") as file:
         return list(file)
```

### Comparing `wslshot-0.0.6/wslshot/cli.py` & `wslshot-0.0.7/wslshot/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -112,15 +112,14 @@
 
     # Copy the screenshot(s) to the destination directory.
     source_screenshots = get_screenshots(source, count)
     copied_screenshots = copy_screenshots(source_screenshots, destination)
 
     # Automatically stage the screenshot(s) if the destination is a git repo.
     # But only if auto_stage is enabled in the config.
-    print(f"{config['auto_stage_enabled']=}")
     if is_git_repo() and bool(config["auto_stage_enabled"]):
         stage_screenshots(copied_screenshots)
         copied_screenshots = format_screenshots_path_for_git(copied_screenshots)
 
     # Print the screenshot(s)'s path in the specified format.
     print_formatted_path(output_format, copied_screenshots)
```

### Comparing `wslshot-0.0.6/wslshot.egg-info/PKG-INFO` & `wslshot-0.0.7/wslshot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wslshot
-Version: 0.0.6
+Version: 0.0.7
 Home-page: https://github.com/sderev/wslshot
 Author: Sébastien De Revière
 License: Apache Licence, Version 2.0
 Project-URL: Documentation, https://github.com/sderev/wslshot
 Project-URL: Issues, http://github.com/sderev/wslshot/issues
 Project-URL: Changelog, https://github.com/sderev/wslshot/releases
 Requires-Python: >=3.8
```

