# Comparing `tmp/niche_cv-0.0.10.tar.gz` & `tmp/niche_cv-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "niche_cv-0.0.10.tar", last modified: Thu Jul 13 04:56:01 2023, max compression
+gzip compressed data, was "niche_cv-0.0.2.tar", last modified: Thu Jul 13 03:18:16 2023, max compression
```

## Comparing `niche_cv-0.0.10.tar` & `niche_cv-0.0.2.tar`

### file list

```diff
@@ -1,21 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 04:56:01.707477 niche_cv-0.0.10/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 04:55:50.000000 niche_cv-0.0.10/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 04:55:50.000000 niche_cv-0.0.10/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-07-13 04:56:01.707477 niche_cv-0.0.10/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-13 04:55:50.000000 niche_cv-0.0.10/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 04:56:01.707477 niche_cv-0.0.10/niche_cv/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 04:55:50.000000 niche_cv-0.0.10/niche_cv/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 04:56:01.707477 niche_cv-0.0.10/niche_cv/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 04:55:50.000000 niche_cv-0.0.10/niche_cv/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-07-13 04:55:50.000000 niche_cv-0.0.10/niche_cv/data/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 04:56:01.707477 niche_cv-0.0.10/niche_cv/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 04:55:50.000000 niche_cv-0.0.10/niche_cv/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-07-13 04:55:50.000000 niche_cv-0.0.10/niche_cv/show.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 04:56:01.707477 niche_cv-0.0.10/niche_cv.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-07-13 04:56:01.000000 niche_cv-0.0.10/niche_cv.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-13 04:56:01.000000 niche_cv-0.0.10/niche_cv.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 04:56:01.000000 niche_cv-0.0.10/niche_cv.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-13 04:56:01.000000 niche_cv-0.0.10/niche_cv.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-13 04:56:01.000000 niche_cv-0.0.10/niche_cv.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 04:56:01.707477 niche_cv-0.0.10/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-13 04:55:50.000000 niche_cv-0.0.10/setup.py
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

