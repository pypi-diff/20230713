# Comparing `tmp/understar-0.2.0.tar.gz` & `tmp/understar-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "understar-0.2.0.tar", last modified: Wed Jul 12 09:40:24 2023, max compression
+gzip compressed data, was "understar-0.2.3.tar", last modified: Thu Jul 13 00:38:08 2023, max compression
```

## Comparing `understar-0.2.0.tar` & `understar-0.2.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 maxence    (501) staff       (20)        0 2023-07-12 09:40:24.071028 understar-0.2.0/
--rw-r--r--   0 maxence    (501) staff       (20)     1188 2023-05-26 01:06:57.000000 understar-0.2.0/LICENSE.md
--rw-r--r--   0 maxence    (501) staff       (20)      591 2023-07-12 09:40:24.070913 understar-0.2.0/PKG-INFO
--rw-r--r--   0 maxence    (501) staff       (20)       45 2023-05-26 01:06:57.000000 understar-0.2.0/README.md
--rw-r--r--   0 maxence    (501) staff       (20)       38 2023-07-12 09:40:24.071075 understar-0.2.0/setup.cfg
--rw-r--r--   0 maxence    (501) staff       (20)     1222 2023-07-12 09:33:23.000000 understar-0.2.0/setup.py
-drwxr-xr-x   0 maxence    (501) staff       (20)        0 2023-07-12 09:40:24.067076 understar-0.2.0/understar/
--rw-r--r--   0 maxence    (501) staff       (20)       49 2023-07-12 03:28:50.000000 understar-0.2.0/understar/__init__.py
-drwxr-xr-x   0 maxence    (501) staff       (20)        0 2023-07-12 09:40:24.068136 understar-0.2.0/understar/system/
--rw-r--r--   0 maxence    (501) staff       (20)       17 2023-07-12 03:20:28.000000 understar-0.2.0/understar/system/__init__.py
-drwxr-xr-x   0 maxence    (501) staff       (20)        0 2023-07-12 09:40:24.070613 understar-0.2.0/understar/system/lib/
--rw-r--r--   0 maxence    (501) staff       (20)      149 2023-07-12 03:30:52.000000 understar-0.2.0/understar/system/lib/__init__.py
--rw-r--r--   0 maxence    (501) staff       (20)     5614 2023-07-12 03:35:46.000000 understar-0.2.0/understar/system/lib/app.py
--rw-r--r--   0 maxence    (501) staff       (20)     1015 2023-06-23 09:10:23.000000 understar-0.2.0/understar/system/lib/com.py
--rw-r--r--   0 maxence    (501) staff       (20)    11757 2023-06-19 00:59:20.000000 understar-0.2.0/understar/system/lib/event.py
--rw-r--r--   0 maxence    (501) staff       (20)     3784 2023-06-19 05:27:26.000000 understar-0.2.0/understar/system/lib/save.py
--rw-r--r--   0 maxence    (501) staff       (20)     2402 2023-06-25 03:39:17.000000 understar-0.2.0/understar/system/lib/store.py
--rw-r--r--   0 maxence    (501) staff       (20)      174 2023-06-23 09:10:04.000000 understar-0.2.0/understar/system/lib/types.py
--rw-r--r--   0 maxence    (501) staff       (20)     4978 2023-07-12 03:07:24.000000 understar-0.2.0/understar/system/lib/utils.py
--rw-r--r--   0 maxence    (501) staff       (20)    30889 2023-07-12 09:33:55.000000 understar-0.2.0/understar/understar.py
-drwxr-xr-x   0 maxence    (501) staff       (20)        0 2023-07-12 09:40:24.067945 understar-0.2.0/understar.egg-info/
--rw-r--r--   0 maxence    (501) staff       (20)      591 2023-07-12 09:40:24.000000 understar-0.2.0/understar.egg-info/PKG-INFO
--rw-r--r--   0 maxence    (501) staff       (20)      505 2023-07-12 09:40:24.000000 understar-0.2.0/understar.egg-info/SOURCES.txt
--rw-r--r--   0 maxence    (501) staff       (20)        1 2023-07-12 09:40:24.000000 understar-0.2.0/understar.egg-info/dependency_links.txt
--rw-r--r--   0 maxence    (501) staff       (20)       49 2023-07-12 09:40:24.000000 understar-0.2.0/understar.egg-info/requires.txt
--rw-r--r--   0 maxence    (501) staff       (20)       10 2023-07-12 09:40:24.000000 understar-0.2.0/understar.egg-info/top_level.txt
+drwxr-xr-x   0 maxence    (501) staff       (20)        0 2023-07-13 00:38:08.267398 understar-0.2.3/
+-rw-r--r--   0 maxence    (501) staff       (20)     1188 2023-05-26 01:06:57.000000 understar-0.2.3/LICENSE.md
+-rw-r--r--   0 maxence    (501) staff       (20)      591 2023-07-13 00:38:08.267279 understar-0.2.3/PKG-INFO
+-rw-r--r--   0 maxence    (501) staff       (20)       45 2023-05-26 01:06:57.000000 understar-0.2.3/README.md
+-rw-r--r--   0 maxence    (501) staff       (20)       38 2023-07-13 00:38:08.267448 understar-0.2.3/setup.cfg
+-rw-r--r--   0 maxence    (501) staff       (20)     1222 2023-07-13 00:34:17.000000 understar-0.2.3/setup.py
+drwxr-xr-x   0 maxence    (501) staff       (20)        0 2023-07-13 00:38:08.263443 understar-0.2.3/understar/
+-rw-r--r--   0 maxence    (501) staff       (20)       49 2023-07-12 03:28:50.000000 understar-0.2.3/understar/__init__.py
+drwxr-xr-x   0 maxence    (501) staff       (20)        0 2023-07-13 00:38:08.264497 understar-0.2.3/understar/system/
+-rw-r--r--   0 maxence    (501) staff       (20)       17 2023-07-12 03:20:28.000000 understar-0.2.3/understar/system/__init__.py
+drwxr-xr-x   0 maxence    (501) staff       (20)        0 2023-07-13 00:38:08.266995 understar-0.2.3/understar/system/lib/
+-rw-r--r--   0 maxence    (501) staff       (20)      149 2023-07-12 03:30:52.000000 understar-0.2.3/understar/system/lib/__init__.py
+-rw-r--r--   0 maxence    (501) staff       (20)     5614 2023-07-12 03:35:46.000000 understar-0.2.3/understar/system/lib/app.py
+-rw-r--r--   0 maxence    (501) staff       (20)     1015 2023-06-23 09:10:23.000000 understar-0.2.3/understar/system/lib/com.py
+-rw-r--r--   0 maxence    (501) staff       (20)    11757 2023-06-19 00:59:20.000000 understar-0.2.3/understar/system/lib/event.py
+-rw-r--r--   0 maxence    (501) staff       (20)     3784 2023-06-19 05:27:26.000000 understar-0.2.3/understar/system/lib/save.py
+-rw-r--r--   0 maxence    (501) staff       (20)     2402 2023-06-25 03:39:17.000000 understar-0.2.3/understar/system/lib/store.py
+-rw-r--r--   0 maxence    (501) staff       (20)      174 2023-06-23 09:10:04.000000 understar-0.2.3/understar/system/lib/types.py
+-rw-r--r--   0 maxence    (501) staff       (20)     4978 2023-07-12 03:07:24.000000 understar-0.2.3/understar/system/lib/utils.py
+-rw-r--r--   0 maxence    (501) staff       (20)    30889 2023-07-12 09:33:55.000000 understar-0.2.3/understar/understar.py
+drwxr-xr-x   0 maxence    (501) staff       (20)        0 2023-07-13 00:38:08.264336 understar-0.2.3/understar.egg-info/
+-rw-r--r--   0 maxence    (501) staff       (20)      591 2023-07-13 00:38:08.000000 understar-0.2.3/understar.egg-info/PKG-INFO
+-rw-r--r--   0 maxence    (501) staff       (20)      505 2023-07-13 00:38:08.000000 understar-0.2.3/understar.egg-info/SOURCES.txt
+-rw-r--r--   0 maxence    (501) staff       (20)        1 2023-07-13 00:38:08.000000 understar-0.2.3/understar.egg-info/dependency_links.txt
+-rw-r--r--   0 maxence    (501) staff       (20)       49 2023-07-13 00:38:08.000000 understar-0.2.3/understar.egg-info/requires.txt
+-rw-r--r--   0 maxence    (501) staff       (20)       10 2023-07-13 00:38:08.000000 understar-0.2.3/understar.egg-info/top_level.txt
```

### Comparing `understar-0.2.0/LICENSE.md` & `understar-0.2.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `understar-0.2.0/PKG-INFO` & `understar-0.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: understar
-Version: 0.2.0
+Version: 0.2.3
 Summary: A discord bot framewrok
 Home-page: https://github.com/GalTechDev/UnderStar-OS
 Download-URL: https://github.com/GalTechDev/UnderStar-OS/tarball/master
 Author: GalTech
 Author-email: poussigalitv@gmail.com
 License: MIT
 Keywords: discord,bot,discord.py,understar,os,framework
```

### Comparing `understar-0.2.0/setup.py` & `understar-0.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open("README.md", "r") as stream:
     long_description = stream.read()
 
 # long_description = "An universal wrapper (and useful tool) to make event / commands in python"
 
 setup(
     name='understar',
-    version="0.2.0",
+    version="0.2.3",
     url='https://github.com/GalTechDev/UnderStar-OS',
     download_url='https://github.com/GalTechDev/UnderStar-OS/tarball/master',
     license='MIT',
     author='GalTech',
     author_email='poussigalitv@gmail.com',
     description='A discord bot framewrok',
     long_description=long_description,
```

### Comparing `understar-0.2.0/understar/system/lib/app.py` & `understar-0.2.3/understar/system/lib/app.py`

 * *Files identical despite different names*

### Comparing `understar-0.2.0/understar/system/lib/com.py` & `understar-0.2.3/understar/system/lib/com.py`

 * *Files identical despite different names*

### Comparing `understar-0.2.0/understar/system/lib/event.py` & `understar-0.2.3/understar/system/lib/event.py`

 * *Files identical despite different names*

### Comparing `understar-0.2.0/understar/system/lib/save.py` & `understar-0.2.3/understar/system/lib/save.py`

 * *Files identical despite different names*

### Comparing `understar-0.2.0/understar/system/lib/store.py` & `understar-0.2.3/understar/system/lib/store.py`

 * *Files identical despite different names*

### Comparing `understar-0.2.0/understar/system/lib/utils.py` & `understar-0.2.3/understar/system/lib/utils.py`

 * *Files identical despite different names*

### Comparing `understar-0.2.0/understar/understar.py` & `understar-0.2.3/understar/understar.py`

 * *Files identical despite different names*

### Comparing `understar-0.2.0/understar.egg-info/PKG-INFO` & `understar-0.2.3/understar.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: understar
-Version: 0.2.0
+Version: 0.2.3
 Summary: A discord bot framewrok
 Home-page: https://github.com/GalTechDev/UnderStar-OS
 Download-URL: https://github.com/GalTechDev/UnderStar-OS/tarball/master
 Author: GalTech
 Author-email: poussigalitv@gmail.com
 License: MIT
 Keywords: discord,bot,discord.py,understar,os,framework
```

