# Comparing `tmp/aie-sdk-3.0.2.tar.gz` & `tmp/aie-sdk-3.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aie-sdk-3.0.2.tar", last modified: Thu Jul 13 02:22:24 2023, max compression
+gzip compressed data, was "aie-sdk-3.0.3.tar", last modified: Thu Jul 13 08:32:40 2023, max compression
```

## Comparing `aie-sdk-3.0.2.tar` & `aie-sdk-3.0.3.tar`

### file list

```diff
@@ -1,13 +1,20 @@
-drwxr-xr-x   0 songci     (502) staff       (20)        0 2023-07-13 02:22:24.519428 aie-sdk-3.0.2/
--rw-r--r--   0 songci     (502) staff       (20)      454 2023-07-13 02:22:24.518832 aie-sdk-3.0.2/PKG-INFO
--rw-r--r--   0 songci     (502) staff       (20)      209 2022-11-21 06:06:45.000000 aie-sdk-3.0.2/README.md
-drwxr-xr-x   0 songci     (502) staff       (20)        0 2023-07-13 02:22:24.515124 aie-sdk-3.0.2/aie/
--rw-r--r--   0 songci     (502) staff       (20)      249 2023-07-13 02:21:40.000000 aie-sdk-3.0.2/aie/__init__.py
-drwxr-xr-x   0 songci     (502) staff       (20)        0 2023-07-13 02:22:24.518179 aie-sdk-3.0.2/aie_sdk.egg-info/
--rw-r--r--   0 songci     (502) staff       (20)      454 2023-07-13 02:22:24.000000 aie-sdk-3.0.2/aie_sdk.egg-info/PKG-INFO
--rw-r--r--   0 songci     (502) staff       (20)      188 2023-07-13 02:22:24.000000 aie-sdk-3.0.2/aie_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 songci     (502) staff       (20)        1 2023-07-13 02:22:24.000000 aie-sdk-3.0.2/aie_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 songci     (502) staff       (20)      248 2023-07-13 02:22:24.000000 aie-sdk-3.0.2/aie_sdk.egg-info/requires.txt
--rw-r--r--   0 songci     (502) staff       (20)        4 2023-07-13 02:22:24.000000 aie-sdk-3.0.2/aie_sdk.egg-info/top_level.txt
--rw-r--r--   0 songci     (502) staff       (20)       38 2023-07-13 02:22:24.519590 aie-sdk-3.0.2/setup.cfg
--rw-r--r--   0 songci     (502) staff       (20)     1103 2023-06-08 06:03:40.000000 aie-sdk-3.0.2/setup.py
+drwxr-xr-x   0 songci     (502) staff       (20)        0 2023-07-13 08:32:40.605948 aie-sdk-3.0.3/
+-rw-r--r--   0 songci     (502) staff       (20)      454 2023-07-13 08:32:40.605464 aie-sdk-3.0.3/PKG-INFO
+-rw-r--r--   0 songci     (502) staff       (20)      209 2022-11-21 06:06:45.000000 aie-sdk-3.0.3/README.md
+drwxr-xr-x   0 songci     (502) staff       (20)        0 2023-07-13 08:32:40.600265 aie-sdk-3.0.3/aie/
+-rw-r--r--   0 songci     (502) staff       (20)      249 2023-07-13 04:09:28.000000 aie-sdk-3.0.3/aie/__init__.py
+-rw-r--r--   0 songci     (502) staff       (20)       31 2023-07-13 04:09:28.000000 aie-sdk-3.0.3/aie/auth.py
+drwxr-xr-x   0 songci     (502) staff       (20)        0 2023-07-13 08:32:40.600883 aie-sdk-3.0.3/aie/client/
+-rw-r--r--   0 songci     (502) staff       (20)       35 2023-07-13 03:57:55.000000 aie-sdk-3.0.3/aie/client/__init__.py
+-rw-r--r--   0 songci     (502) staff       (20)       30 2023-07-13 04:09:28.000000 aie-sdk-3.0.3/aie/env.py
+drwxr-xr-x   0 songci     (502) staff       (20)        0 2023-07-13 08:32:40.601462 aie-sdk-3.0.3/aie/error/
+-rw-r--r--   0 songci     (502) staff       (20)       32 2023-07-13 03:58:55.000000 aie-sdk-3.0.3/aie/error/__init__.py
+-rw-r--r--   0 songci     (502) staff       (20)       32 2023-07-13 04:09:38.000000 aie-sdk-3.0.3/aie/g_var.py
+drwxr-xr-x   0 songci     (502) staff       (20)        0 2023-07-13 08:32:40.604627 aie-sdk-3.0.3/aie_sdk.egg-info/
+-rw-r--r--   0 songci     (502) staff       (20)      454 2023-07-13 08:32:40.000000 aie-sdk-3.0.3/aie_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 songci     (502) staff       (20)      269 2023-07-13 08:32:40.000000 aie-sdk-3.0.3/aie_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 songci     (502) staff       (20)        1 2023-07-13 08:32:40.000000 aie-sdk-3.0.3/aie_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 songci     (502) staff       (20)      248 2023-07-13 08:32:40.000000 aie-sdk-3.0.3/aie_sdk.egg-info/requires.txt
+-rw-r--r--   0 songci     (502) staff       (20)        4 2023-07-13 08:32:40.000000 aie-sdk-3.0.3/aie_sdk.egg-info/top_level.txt
+-rw-r--r--   0 songci     (502) staff       (20)       38 2023-07-13 08:32:40.606085 aie-sdk-3.0.3/setup.cfg
+-rw-r--r--   0 songci     (502) staff       (20)     1103 2023-06-08 06:03:40.000000 aie-sdk-3.0.3/setup.py
```

### Comparing `aie-sdk-3.0.2/setup.py` & `aie-sdk-3.0.3/setup.py`

 * *Files identical despite different names*

