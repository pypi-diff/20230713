# Comparing `tmp/pyOpenHaptics-0.0.2.tar.gz` & `tmp/pyOpenHaptics-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyOpenHaptics-0.0.2.tar", last modified: Wed Jul 12 16:05:21 2023, max compression
+gzip compressed data, was "pyOpenHaptics-0.0.3.tar", last modified: Thu Jul 13 08:25:43 2023, max compression
```

## Comparing `pyOpenHaptics-0.0.2.tar` & `pyOpenHaptics-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 hammerlab  (1001) hammerlab  (1001)        0 2023-07-12 16:05:21.060695 pyOpenHaptics-0.0.2/
--rw-rw-r--   0 hammerlab  (1001) hammerlab  (1001)      481 2023-07-12 16:05:21.060695 pyOpenHaptics-0.0.2/PKG-INFO
--rw-rw-r--   0 hammerlab  (1001) hammerlab  (1001)      128 2023-07-12 15:54:52.000000 pyOpenHaptics-0.0.2/README.md
-drwxrwxr-x   0 hammerlab  (1001) hammerlab  (1001)        0 2023-07-12 16:05:21.056695 pyOpenHaptics-0.0.2/pyOpenHaptics.egg-info/
--rw-rw-r--   0 hammerlab  (1001) hammerlab  (1001)      481 2023-07-12 16:05:21.000000 pyOpenHaptics-0.0.2/pyOpenHaptics.egg-info/PKG-INFO
--rw-rw-r--   0 hammerlab  (1001) hammerlab  (1001)      245 2023-07-12 16:05:21.000000 pyOpenHaptics-0.0.2/pyOpenHaptics.egg-info/SOURCES.txt
--rw-rw-r--   0 hammerlab  (1001) hammerlab  (1001)        1 2023-07-12 16:05:21.000000 pyOpenHaptics-0.0.2/pyOpenHaptics.egg-info/dependency_links.txt
--rw-rw-r--   0 hammerlab  (1001) hammerlab  (1001)        4 2023-07-12 16:05:21.000000 pyOpenHaptics-0.0.2/pyOpenHaptics.egg-info/top_level.txt
--rw-rw-r--   0 hammerlab  (1001) hammerlab  (1001)       38 2023-07-12 16:05:21.060695 pyOpenHaptics-0.0.2/setup.cfg
--rw-rw-r--   0 hammerlab  (1001) hammerlab  (1001)      730 2023-07-12 16:04:51.000000 pyOpenHaptics-0.0.2/setup.py
-drwxrwxr-x   0 hammerlab  (1001) hammerlab  (1001)        0 2023-07-12 16:05:21.060695 pyOpenHaptics-0.0.2/src/
--rw-rw-r--   0 hammerlab  (1001) hammerlab  (1001)       18 2023-07-12 13:33:26.000000 pyOpenHaptics-0.0.2/src/__init__.py
--rw-rw-r--   0 hammerlab  (1001) hammerlab  (1001)      623 2023-07-12 13:33:26.000000 pyOpenHaptics-0.0.2/src/exceptions.py
--rw-rw-r--   0 hammerlab  (1001) hammerlab  (1001)     3658 2023-07-12 13:33:26.000000 pyOpenHaptics-0.0.2/src/hd.py
--rw-rw-r--   0 hammerlab  (1001) hammerlab  (1001)     5292 2023-07-12 13:33:26.000000 pyOpenHaptics-0.0.2/src/hd_define.py
--rw-rw-r--   0 hammerlab  (1001) hammerlab  (1001)       82 2023-07-12 13:33:26.000000 pyOpenHaptics-0.0.2/src/hdu_matrix.py
+drwxrwxr-x   0 hammerlab  (1001) hammerlab  (1001)        0 2023-07-13 08:25:43.272190 pyOpenHaptics-0.0.3/
+-rw-rw-r--   0 hammerlab  (1001) hammerlab  (1001)      481 2023-07-13 08:25:43.272190 pyOpenHaptics-0.0.3/PKG-INFO
+-rw-rw-r--   0 hammerlab  (1001) hammerlab  (1001)      128 2023-07-12 15:54:52.000000 pyOpenHaptics-0.0.3/README.md
+drwxrwxr-x   0 hammerlab  (1001) hammerlab  (1001)        0 2023-07-13 08:25:43.272190 pyOpenHaptics-0.0.3/pyOpenHaptics.egg-info/
+-rw-rw-r--   0 hammerlab  (1001) hammerlab  (1001)      481 2023-07-13 08:25:43.000000 pyOpenHaptics-0.0.3/pyOpenHaptics.egg-info/PKG-INFO
+-rw-rw-r--   0 hammerlab  (1001) hammerlab  (1001)      245 2023-07-13 08:25:43.000000 pyOpenHaptics-0.0.3/pyOpenHaptics.egg-info/SOURCES.txt
+-rw-rw-r--   0 hammerlab  (1001) hammerlab  (1001)        1 2023-07-13 08:25:43.000000 pyOpenHaptics-0.0.3/pyOpenHaptics.egg-info/dependency_links.txt
+-rw-rw-r--   0 hammerlab  (1001) hammerlab  (1001)        4 2023-07-13 08:25:43.000000 pyOpenHaptics-0.0.3/pyOpenHaptics.egg-info/top_level.txt
+-rw-rw-r--   0 hammerlab  (1001) hammerlab  (1001)       38 2023-07-13 08:25:43.272190 pyOpenHaptics-0.0.3/setup.cfg
+-rw-rw-r--   0 hammerlab  (1001) hammerlab  (1001)      730 2023-07-13 08:25:36.000000 pyOpenHaptics-0.0.3/setup.py
+drwxrwxr-x   0 hammerlab  (1001) hammerlab  (1001)        0 2023-07-13 08:25:43.272190 pyOpenHaptics-0.0.3/src/
+-rw-rw-r--   0 hammerlab  (1001) hammerlab  (1001)       18 2023-07-12 13:33:26.000000 pyOpenHaptics-0.0.3/src/__init__.py
+-rw-rw-r--   0 hammerlab  (1001) hammerlab  (1001)      623 2023-07-12 13:33:26.000000 pyOpenHaptics-0.0.3/src/exceptions.py
+-rw-rw-r--   0 hammerlab  (1001) hammerlab  (1001)     3658 2023-07-12 13:33:26.000000 pyOpenHaptics-0.0.3/src/hd.py
+-rw-rw-r--   0 hammerlab  (1001) hammerlab  (1001)     5292 2023-07-12 13:33:26.000000 pyOpenHaptics-0.0.3/src/hd_define.py
+-rw-rw-r--   0 hammerlab  (1001) hammerlab  (1001)       82 2023-07-12 13:33:26.000000 pyOpenHaptics-0.0.3/src/hdu_matrix.py
```

### Comparing `pyOpenHaptics-0.0.2/setup.py` & `pyOpenHaptics-0.0.3/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION="0.0.2"
+VERSION="0.0.3"
 DESCRIPTION="Python binding for OpenHaptics"
 LONG_DESCRIPTION="Basic functions to mimic the OpenHaptics library on C++. Written into a more Python friendly language"
 
 setup(
     name="pyOpenHaptics",
     version=VERSION,
     author="Mikel De Iturrate Reyzabal",
```

### Comparing `pyOpenHaptics-0.0.2/src/exceptions.py` & `pyOpenHaptics-0.0.3/src/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyOpenHaptics-0.0.2/src/hd.py` & `pyOpenHaptics-0.0.3/src/hd.py`

 * *Files identical despite different names*

### Comparing `pyOpenHaptics-0.0.2/src/hd_define.py` & `pyOpenHaptics-0.0.3/src/hd_define.py`

 * *Files identical despite different names*

