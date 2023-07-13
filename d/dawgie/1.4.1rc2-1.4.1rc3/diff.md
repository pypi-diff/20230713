# Comparing `tmp/dawgie-1.4.1rc2.tar.gz` & `tmp/dawgie-1.4.1rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dawgie-1.4.1rc2.tar", last modified: Thu Jul 13 15:26:01 2023, max compression
+gzip compressed data, was "dawgie-1.4.1rc3.tar", last modified: Thu Jul 13 16:38:32 2023, max compression
```

## Comparing `dawgie-1.4.1rc2.tar` & `dawgie-1.4.1rc3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-07-13 15:26:01.282250 dawgie-1.4.1rc2/
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     1615 2023-07-13 15:25:38.000000 dawgie-1.4.1rc2/LICENSE
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     9505 2023-07-13 15:26:01.282250 dawgie-1.4.1rc2/PKG-INFO
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     8906 2023-07-13 15:25:38.000000 dawgie-1.4.1rc2/README.md
-drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-07-13 15:26:01.282250 dawgie-1.4.1rc2/dawgie.egg-info/
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     9505 2023-07-13 15:26:01.000000 dawgie-1.4.1rc2/dawgie.egg-info/PKG-INFO
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     6384 2023-07-13 15:26:01.000000 dawgie-1.4.1rc2/dawgie.egg-info/SOURCES.txt
--rw-rw-r--   0 niessner  (1000) niessner  (1000)        1 2023-07-13 15:26:01.000000 dawgie-1.4.1rc2/dawgie.egg-info/dependency_links.txt
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      257 2023-07-13 15:26:01.000000 dawgie-1.4.1rc2/dawgie.egg-info/requires.txt
--rw-rw-r--   0 niessner  (1000) niessner  (1000)        7 2023-07-13 15:26:01.000000 dawgie-1.4.1rc2/dawgie.egg-info/top_level.txt
--rw-rw-r--   0 niessner  (1000) niessner  (1000)       38 2023-07-13 15:26:01.282250 dawgie-1.4.1rc2/setup.cfg
--rwxrwxr-x   0 niessner  (1000) niessner  (1000)     6368 2023-07-13 00:36:01.000000 dawgie-1.4.1rc2/setup.py
+drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-07-13 16:38:32.981605 dawgie-1.4.1rc3/
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     1615 2023-07-13 16:38:16.000000 dawgie-1.4.1rc3/LICENSE
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     9505 2023-07-13 16:38:32.981605 dawgie-1.4.1rc3/PKG-INFO
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     8906 2023-07-13 16:38:16.000000 dawgie-1.4.1rc3/README.md
+drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-07-13 16:38:32.981605 dawgie-1.4.1rc3/dawgie.egg-info/
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     9505 2023-07-13 16:38:32.000000 dawgie-1.4.1rc3/dawgie.egg-info/PKG-INFO
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     6384 2023-07-13 16:38:32.000000 dawgie-1.4.1rc3/dawgie.egg-info/SOURCES.txt
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)        1 2023-07-13 16:38:32.000000 dawgie-1.4.1rc3/dawgie.egg-info/dependency_links.txt
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      257 2023-07-13 16:38:32.000000 dawgie-1.4.1rc3/dawgie.egg-info/requires.txt
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)        7 2023-07-13 16:38:32.000000 dawgie-1.4.1rc3/dawgie.egg-info/top_level.txt
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)       38 2023-07-13 16:38:32.981605 dawgie-1.4.1rc3/setup.cfg
+-rwxrwxr-x   0 niessner  (1000) niessner  (1000)     6368 2023-07-13 16:26:52.000000 dawgie-1.4.1rc3/setup.py
```

### Comparing `dawgie-1.4.1rc2/LICENSE` & `dawgie-1.4.1rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `dawgie-1.4.1rc2/PKG-INFO` & `dawgie-1.4.1rc3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dawgie
-Version: 1.4.1rc2
+Version: 1.4.1rc3
 Summary: Data and Algorithm Work-flow Generation, Introspection, and Execution (DAWGIE)
 Home-page: https://github.com/al-niessner/DAWGIE
 Author: Al Niessner
 Author-email: Al.Niessner@jpl.nasa.gov
 License: see LICENSE file for details
 Keywords: adaptive pipeline
 Platform: UNKNOWN
```

### Comparing `dawgie-1.4.1rc2/README.md` & `dawgie-1.4.1rc3/README.md`

 * *Files identical despite different names*

### Comparing `dawgie-1.4.1rc2/dawgie.egg-info/PKG-INFO` & `dawgie-1.4.1rc3/dawgie.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dawgie
-Version: 1.4.1rc2
+Version: 1.4.1rc3
 Summary: Data and Algorithm Work-flow Generation, Introspection, and Execution (DAWGIE)
 Home-page: https://github.com/al-niessner/DAWGIE
 Author: Al Niessner
 Author-email: Al.Niessner@jpl.nasa.gov
 License: see LICENSE file for details
 Keywords: adaptive pipeline
 Platform: UNKNOWN
```

### Comparing `dawgie-1.4.1rc2/setup.py` & `dawgie-1.4.1rc3/setup.py`

 * *Files identical despite different names*

