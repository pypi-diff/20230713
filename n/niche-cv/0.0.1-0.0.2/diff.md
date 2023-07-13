# Comparing `tmp/niche_cv-0.0.1.tar.gz` & `tmp/niche_cv-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "niche_cv-0.0.1.tar", last modified: Thu Jul 13 03:04:20 2023, max compression
+gzip compressed data, was "niche_cv-0.0.2.tar", last modified: Thu Jul 13 03:18:16 2023, max compression
```

## Comparing `niche_cv-0.0.1.tar` & `niche_cv-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,19 @@
-drwxr-xr-x   0 niche      (502) staff       (20)        0 2023-07-13 03:04:20.231789 niche_cv-0.0.1/
--rw-r--r--   0 niche      (502) staff       (20)        0 2023-07-13 03:01:41.000000 niche_cv-0.0.1/LICENSE
--rw-r--r--   0 niche      (502) staff       (20)        0 2023-07-13 03:01:46.000000 niche_cv-0.0.1/MANIFEST.in
--rw-r--r--   0 niche      (502) staff       (20)      224 2023-07-13 03:04:20.231378 niche_cv-0.0.1/PKG-INFO
-drwxr-xr-x   0 niche      (502) staff       (20)        0 2023-07-13 03:04:20.226512 niche_cv-0.0.1/niche_cv/
--rw-r--r--   0 niche      (502) staff       (20)        0 2023-07-13 03:03:11.000000 niche_cv-0.0.1/niche_cv/__init__.py
-drwxr-xr-x   0 niche      (502) staff       (20)        0 2023-07-13 03:04:20.229777 niche_cv-0.0.1/niche_cv/data/
--rw-r--r--   0 niche      (502) staff       (20)        0 2023-07-13 03:03:24.000000 niche_cv-0.0.1/niche_cv/data/__init__.py
-drwxr-xr-x   0 niche      (502) staff       (20)        0 2023-07-13 03:04:20.230580 niche_cv-0.0.1/niche_cv/models/
--rw-r--r--   0 niche      (502) staff       (20)        0 2023-07-13 03:03:16.000000 niche_cv-0.0.1/niche_cv/models/__init__.py
-drwxr-xr-x   0 niche      (502) staff       (20)        0 2023-07-13 03:04:20.229189 niche_cv-0.0.1/niche_cv.egg-info/
--rw-r--r--   0 niche      (502) staff       (20)      224 2023-07-13 03:04:20.000000 niche_cv-0.0.1/niche_cv.egg-info/PKG-INFO
--rw-r--r--   0 niche      (502) staff       (20)      231 2023-07-13 03:04:20.000000 niche_cv-0.0.1/niche_cv.egg-info/SOURCES.txt
--rw-r--r--   0 niche      (502) staff       (20)        1 2023-07-13 03:04:20.000000 niche_cv-0.0.1/niche_cv.egg-info/dependency_links.txt
--rw-r--r--   0 niche      (502) staff       (20)        9 2023-07-13 03:04:20.000000 niche_cv-0.0.1/niche_cv.egg-info/top_level.txt
--rw-r--r--   0 niche      (502) staff       (20)       38 2023-07-13 03:04:20.231861 niche_cv-0.0.1/setup.cfg
--rw-r--r--   0 niche      (502) staff       (20)      323 2023-07-13 03:01:12.000000 niche_cv-0.0.1/setup.py
+drwxr-xr-x   0 niche      (502) staff       (20)        0 2023-07-13 03:18:16.050017 niche_cv-0.0.2/
+-rw-r--r--   0 niche      (502) staff       (20)        0 2023-07-13 03:01:41.000000 niche_cv-0.0.2/LICENSE
+-rw-r--r--   0 niche      (502) staff       (20)        0 2023-07-13 03:01:46.000000 niche_cv-0.0.2/MANIFEST.in
+-rw-r--r--   0 niche      (502) staff       (20)      224 2023-07-13 03:18:16.048525 niche_cv-0.0.2/PKG-INFO
+drwxr-xr-x   0 niche      (502) staff       (20)        0 2023-07-13 03:18:16.045517 niche_cv-0.0.2/niche_cv/
+-rw-r--r--   0 niche      (502) staff       (20)        0 2023-07-13 03:03:11.000000 niche_cv-0.0.2/niche_cv/__init__.py
+drwxr-xr-x   0 niche      (502) staff       (20)        0 2023-07-13 03:18:16.047659 niche_cv-0.0.2/niche_cv/data/
+-rw-r--r--   0 niche      (502) staff       (20)        0 2023-07-13 03:03:24.000000 niche_cv-0.0.2/niche_cv/data/__init__.py
+drwxr-xr-x   0 niche      (502) staff       (20)        0 2023-07-13 03:18:16.047911 niche_cv-0.0.2/niche_cv/models/
+-rw-r--r--   0 niche      (502) staff       (20)        0 2023-07-13 03:03:16.000000 niche_cv-0.0.2/niche_cv/models/__init__.py
+-rw-r--r--   0 niche      (502) staff       (20)      289 2023-07-13 03:11:53.000000 niche_cv-0.0.2/niche_cv/show.py
+drwxr-xr-x   0 niche      (502) staff       (20)        0 2023-07-13 03:18:16.047358 niche_cv-0.0.2/niche_cv.egg-info/
+-rw-r--r--   0 niche      (502) staff       (20)      224 2023-07-13 03:18:15.000000 niche_cv-0.0.2/niche_cv.egg-info/PKG-INFO
+-rw-r--r--   0 niche      (502) staff       (20)      283 2023-07-13 03:18:15.000000 niche_cv-0.0.2/niche_cv.egg-info/SOURCES.txt
+-rw-r--r--   0 niche      (502) staff       (20)        1 2023-07-13 03:18:15.000000 niche_cv-0.0.2/niche_cv.egg-info/dependency_links.txt
+-rw-r--r--   0 niche      (502) staff       (20)       45 2023-07-13 03:18:15.000000 niche_cv-0.0.2/niche_cv.egg-info/entry_points.txt
+-rw-r--r--   0 niche      (502) staff       (20)        9 2023-07-13 03:18:15.000000 niche_cv-0.0.2/niche_cv.egg-info/top_level.txt
+-rw-r--r--   0 niche      (502) staff       (20)       38 2023-07-13 03:18:16.050124 niche_cv-0.0.2/setup.cfg
+-rw-r--r--   0 niche      (502) staff       (20)      391 2023-07-13 03:17:57.000000 niche_cv-0.0.2/setup.py
```

