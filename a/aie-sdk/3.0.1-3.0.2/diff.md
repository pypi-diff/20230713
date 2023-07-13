# Comparing `tmp/aie-sdk-3.0.1.tar.gz` & `tmp/aie-sdk-3.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aie-sdk-3.0.1.tar", last modified: Thu Jun  8 06:03:53 2023, max compression
+gzip compressed data, was "aie-sdk-3.0.2.tar", last modified: Thu Jul 13 02:22:24 2023, max compression
```

## Comparing `aie-sdk-3.0.1.tar` & `aie-sdk-3.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 songci     (502) staff       (20)        0 2023-06-08 06:03:53.916916 aie-sdk-3.0.1/
--rw-r--r--   0 songci     (502) staff       (20)      454 2023-06-08 06:03:53.916441 aie-sdk-3.0.1/PKG-INFO
--rw-r--r--   0 songci     (502) staff       (20)      209 2022-11-21 06:06:45.000000 aie-sdk-3.0.1/README.md
-drwxr-xr-x   0 songci     (502) staff       (20)        0 2023-06-08 06:03:53.912358 aie-sdk-3.0.1/aie/
--rw-r--r--   0 songci     (502) staff       (20)      214 2023-06-06 06:51:25.000000 aie-sdk-3.0.1/aie/__init__.py
-drwxr-xr-x   0 songci     (502) staff       (20)        0 2023-06-08 06:03:53.915461 aie-sdk-3.0.1/aie_sdk.egg-info/
--rw-r--r--   0 songci     (502) staff       (20)      454 2023-06-08 06:03:53.000000 aie-sdk-3.0.1/aie_sdk.egg-info/PKG-INFO
--rw-r--r--   0 songci     (502) staff       (20)      188 2023-06-08 06:03:53.000000 aie-sdk-3.0.1/aie_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 songci     (502) staff       (20)        1 2023-06-08 06:03:53.000000 aie-sdk-3.0.1/aie_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 songci     (502) staff       (20)      248 2023-06-08 06:03:53.000000 aie-sdk-3.0.1/aie_sdk.egg-info/requires.txt
--rw-r--r--   0 songci     (502) staff       (20)        4 2023-06-08 06:03:53.000000 aie-sdk-3.0.1/aie_sdk.egg-info/top_level.txt
--rw-r--r--   0 songci     (502) staff       (20)       38 2023-06-08 06:03:53.917051 aie-sdk-3.0.1/setup.cfg
--rw-r--r--   0 songci     (502) staff       (20)     1103 2023-06-08 06:03:40.000000 aie-sdk-3.0.1/setup.py
+drwxr-xr-x   0 songci     (502) staff       (20)        0 2023-07-13 02:22:24.519428 aie-sdk-3.0.2/
+-rw-r--r--   0 songci     (502) staff       (20)      454 2023-07-13 02:22:24.518832 aie-sdk-3.0.2/PKG-INFO
+-rw-r--r--   0 songci     (502) staff       (20)      209 2022-11-21 06:06:45.000000 aie-sdk-3.0.2/README.md
+drwxr-xr-x   0 songci     (502) staff       (20)        0 2023-07-13 02:22:24.515124 aie-sdk-3.0.2/aie/
+-rw-r--r--   0 songci     (502) staff       (20)      249 2023-07-13 02:21:40.000000 aie-sdk-3.0.2/aie/__init__.py
+drwxr-xr-x   0 songci     (502) staff       (20)        0 2023-07-13 02:22:24.518179 aie-sdk-3.0.2/aie_sdk.egg-info/
+-rw-r--r--   0 songci     (502) staff       (20)      454 2023-07-13 02:22:24.000000 aie-sdk-3.0.2/aie_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 songci     (502) staff       (20)      188 2023-07-13 02:22:24.000000 aie-sdk-3.0.2/aie_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 songci     (502) staff       (20)        1 2023-07-13 02:22:24.000000 aie-sdk-3.0.2/aie_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 songci     (502) staff       (20)      248 2023-07-13 02:22:24.000000 aie-sdk-3.0.2/aie_sdk.egg-info/requires.txt
+-rw-r--r--   0 songci     (502) staff       (20)        4 2023-07-13 02:22:24.000000 aie-sdk-3.0.2/aie_sdk.egg-info/top_level.txt
+-rw-r--r--   0 songci     (502) staff       (20)       38 2023-07-13 02:22:24.519590 aie-sdk-3.0.2/setup.cfg
+-rw-r--r--   0 songci     (502) staff       (20)     1103 2023-06-08 06:03:40.000000 aie-sdk-3.0.2/setup.py
```

### Comparing `aie-sdk-3.0.1/setup.py` & `aie-sdk-3.0.2/setup.py`

 * *Files identical despite different names*

