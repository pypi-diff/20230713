# Comparing `tmp/pillow-stackblur-0.1.0.tar.gz` & `tmp/pillow-stackblur-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pillow-stackblur-0.1.0.tar", last modified: Wed Jul 15 11:29:57 2020, max compression
+gzip compressed data, was "pillow-stackblur-0.1.1.tar", last modified: Thu Jul 13 12:29:38 2023, max compression
```

## Comparing `pillow-stackblur-0.1.0.tar` & `pillow-stackblur-0.1.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 jon       (1000) jon       (1000)        0 2020-07-15 11:29:57.000000 pillow-stackblur-0.1.0/
-drwxrwxr-x   0 jon       (1000) jon       (1000)        0 2020-07-15 11:29:57.000000 pillow-stackblur-0.1.0/pillow_stackblur.egg-info/
--rw-rw-r--   0 jon       (1000) jon       (1000)       21 2020-07-15 11:29:57.000000 pillow-stackblur-0.1.0/pillow_stackblur.egg-info/top_level.txt
--rw-rw-r--   0 jon       (1000) jon       (1000)        1 2020-07-15 11:29:57.000000 pillow-stackblur-0.1.0/pillow_stackblur.egg-info/dependency_links.txt
--rw-rw-r--   0 jon       (1000) jon       (1000)     1422 2020-07-15 11:29:57.000000 pillow-stackblur-0.1.0/pillow_stackblur.egg-info/PKG-INFO
--rw-rw-r--   0 jon       (1000) jon       (1000)      243 2020-07-15 11:29:57.000000 pillow-stackblur-0.1.0/pillow_stackblur.egg-info/SOURCES.txt
--rw-rw-r--   0 jon       (1000) jon       (1000)       19 2020-07-15 11:29:57.000000 pillow-stackblur-0.1.0/pillow_stackblur.egg-info/requires.txt
--rw-rw-r--   0 jon       (1000) jon       (1000)      480 2020-07-15 11:17:23.000000 pillow-stackblur-0.1.0/stackblur.py
--rw-rw-r--   0 jon       (1000) jon       (1000)     9878 2020-07-15 11:17:23.000000 pillow-stackblur-0.1.0/cstackblur.c
--rw-rw-r--   0 jon       (1000) jon       (1000)     1422 2020-07-15 11:29:57.000000 pillow-stackblur-0.1.0/PKG-INFO
--rw-rw-r--   0 jon       (1000) jon       (1000)     3044 2020-07-15 11:21:41.000000 pillow-stackblur-0.1.0/setup.py
--rw-rw-r--   0 jon       (1000) jon       (1000)       59 2020-07-15 11:29:57.000000 pillow-stackblur-0.1.0/setup.cfg
--rw-rw-r--   0 jon       (1000) jon       (1000)      877 2020-07-15 11:17:23.000000 pillow-stackblur-0.1.0/README.md
+drwxrwxr-x   0 jon       (1000) jon       (1000)        0 2023-07-13 12:29:38.703898 pillow-stackblur-0.1.1/
+-rw-rw-r--   0 jon       (1000) jon       (1000)     1192 2023-07-13 12:29:38.703898 pillow-stackblur-0.1.1/PKG-INFO
+-rw-rw-r--   0 jon       (1000) jon       (1000)      877 2023-07-13 12:23:00.000000 pillow-stackblur-0.1.1/README.md
+-rw-rw-r--   0 jon       (1000) jon       (1000)     9878 2023-07-13 12:23:00.000000 pillow-stackblur-0.1.1/cstackblur.c
+drwxrwxr-x   0 jon       (1000) jon       (1000)        0 2023-07-13 12:29:38.703898 pillow-stackblur-0.1.1/pillow_stackblur.egg-info/
+-rw-rw-r--   0 jon       (1000) jon       (1000)     1192 2023-07-13 12:29:38.000000 pillow-stackblur-0.1.1/pillow_stackblur.egg-info/PKG-INFO
+-rw-rw-r--   0 jon       (1000) jon       (1000)      243 2023-07-13 12:29:38.000000 pillow-stackblur-0.1.1/pillow_stackblur.egg-info/SOURCES.txt
+-rw-rw-r--   0 jon       (1000) jon       (1000)        1 2023-07-13 12:29:38.000000 pillow-stackblur-0.1.1/pillow_stackblur.egg-info/dependency_links.txt
+-rw-rw-r--   0 jon       (1000) jon       (1000)       19 2023-07-13 12:29:38.000000 pillow-stackblur-0.1.1/pillow_stackblur.egg-info/requires.txt
+-rw-rw-r--   0 jon       (1000) jon       (1000)       21 2023-07-13 12:29:38.000000 pillow-stackblur-0.1.1/pillow_stackblur.egg-info/top_level.txt
+-rw-rw-r--   0 jon       (1000) jon       (1000)       38 2023-07-13 12:29:38.703898 pillow-stackblur-0.1.1/setup.cfg
+-rw-rw-r--   0 jon       (1000) jon       (1000)     3044 2023-07-13 12:25:18.000000 pillow-stackblur-0.1.1/setup.py
+-rw-rw-r--   0 jon       (1000) jon       (1000)      480 2023-07-13 12:23:00.000000 pillow-stackblur-0.1.1/stackblur.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pillow-stackblur-0.1.0/cstackblur.c` & `pillow-stackblur-0.1.1/cstackblur.c`

 * *Files identical despite different names*

### Comparing `pillow-stackblur-0.1.0/setup.py` & `pillow-stackblur-0.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = 'pillow-stackblur'
 DESCRIPTION = 'The Pillow filter for Stack Blur.'
 URL = 'https://github.com/dldevinc/pillow-stackblur'
 EMAIL = 'duguschi@gmail.com'
 AUTHOR = 'Jones Chi'
 REQUIRES_PYTHON = '>=3.5.0'
-VERSION = '0.1.0'
+VERSION = '0.1.1'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     'pillow',
 ]
 
 # What packages are optional?
```

### Comparing `pillow-stackblur-0.1.0/README.md` & `pillow-stackblur-0.1.1/README.md`

 * *Files identical despite different names*

