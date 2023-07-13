# Comparing `tmp/entail-0.0.1.tar.gz` & `tmp/entail-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "entail-0.0.1.tar", last modified: Thu Jul 13 04:35:22 2023, max compression
+gzip compressed data, was "entail-0.1.0.tar", last modified: Wed Jul 12 18:30:58 2023, max compression
```

## Comparing `entail-0.0.1.tar` & `entail-0.1.0.tar`

### file list

```diff
@@ -1,22 +1,33 @@
-drwxr-xr-x   0 haowu4     (501) staff       (20)        0 2023-07-13 04:35:22.012404 entail-0.0.1/
--rw-r--r--   0 haowu4     (501) staff       (20)      147 2023-07-13 04:35:22.012304 entail-0.0.1/PKG-INFO
-drwxr-xr-x   0 haowu4     (501) staff       (20)        0 2023-07-13 04:35:22.010517 entail-0.0.1/entail/
--rw-r--r--   0 haowu4     (501) staff       (20)       87 2023-07-12 04:37:13.000000 entail-0.0.1/entail/__init__.py
--rw-r--r--   0 haowu4     (501) staff       (20)      117 2023-07-12 00:12:40.000000 entail-0.0.1/entail/chat.py
--rw-r--r--   0 haowu4     (501) staff       (20)     1858 2023-07-12 04:35:55.000000 entail-0.0.1/entail/config.py
--rw-r--r--   0 haowu4     (501) staff       (20)     4316 2023-07-12 05:29:43.000000 entail-0.0.1/entail/core.py
--rw-r--r--   0 haowu4     (501) staff       (20)     4520 2023-07-12 17:05:34.000000 entail-0.0.1/entail/env.py
--rw-r--r--   0 haowu4     (501) staff       (20)      625 2023-07-11 18:21:50.000000 entail-0.0.1/entail/main.py
--rw-r--r--   0 haowu4     (501) staff       (20)     2379 2023-07-12 18:38:59.000000 entail-0.0.1/entail/results.py
--rw-r--r--   0 haowu4     (501) staff       (20)     1321 2023-07-12 16:48:49.000000 entail-0.0.1/entail/utils.py
-drwxr-xr-x   0 haowu4     (501) staff       (20)        0 2023-07-13 04:35:22.011396 entail-0.0.1/entail.egg-info/
--rw-r--r--   0 haowu4     (501) staff       (20)      147 2023-07-13 04:35:22.000000 entail-0.0.1/entail.egg-info/PKG-INFO
--rw-r--r--   0 haowu4     (501) staff       (20)      325 2023-07-13 04:35:22.000000 entail-0.0.1/entail.egg-info/SOURCES.txt
--rw-r--r--   0 haowu4     (501) staff       (20)        1 2023-07-13 04:35:22.000000 entail-0.0.1/entail.egg-info/dependency_links.txt
--rw-r--r--   0 haowu4     (501) staff       (20)       39 2023-07-13 04:35:22.000000 entail-0.0.1/entail.egg-info/requires.txt
--rw-r--r--   0 haowu4     (501) staff       (20)        7 2023-07-13 04:35:22.000000 entail-0.0.1/entail.egg-info/top_level.txt
--rw-r--r--   0 haowu4     (501) staff       (20)       38 2023-07-13 04:35:22.012443 entail-0.0.1/setup.cfg
--rw-r--r--   0 haowu4     (501) staff       (20)      348 2023-07-13 04:35:16.000000 entail-0.0.1/setup.py
-drwxr-xr-x   0 haowu4     (501) staff       (20)        0 2023-07-13 04:35:22.011918 entail-0.0.1/tests/
--rw-r--r--   0 haowu4     (501) staff       (20)      191 2023-07-11 17:08:15.000000 entail-0.0.1/tests/test_e2e.py
--rw-r--r--   0 haowu4     (501) staff       (20)      195 2023-07-11 17:08:46.000000 entail-0.0.1/tests/test_loader.py
+drwxr-xr-x   0 haowu4     (501) wheel        (0)        0 2023-07-12 18:30:58.595476 entail-0.1.0/
+-rw-r--r--   0 haowu4     (501) wheel        (0)      148 2023-07-12 18:29:45.000000 entail-0.1.0/AUTHORS.rst
+-rw-r--r--   0 haowu4     (501) wheel        (0)     3506 2023-07-12 18:29:45.000000 entail-0.1.0/CONTRIBUTING.rst
+-rw-r--r--   0 haowu4     (501) wheel        (0)       89 2023-07-12 18:29:45.000000 entail-0.1.0/HISTORY.rst
+-rw-r--r--   0 haowu4     (501) wheel        (0)     1065 2023-07-12 18:29:45.000000 entail-0.1.0/LICENSE
+-rw-r--r--   0 haowu4     (501) wheel        (0)      262 2023-07-12 18:29:45.000000 entail-0.1.0/MANIFEST.in
+-rw-r--r--   0 haowu4     (501) wheel        (0)     1558 2023-07-12 18:30:58.595524 entail-0.1.0/PKG-INFO
+-rw-r--r--   0 haowu4     (501) wheel        (0)      815 2023-07-12 18:29:45.000000 entail-0.1.0/README.rst
+drwxr-xr-x   0 haowu4     (501) wheel        (0)        0 2023-07-12 18:30:58.594358 entail-0.1.0/docs/
+-rw-r--r--   0 haowu4     (501) wheel        (0)      607 2023-07-12 18:29:45.000000 entail-0.1.0/docs/Makefile
+-rw-r--r--   0 haowu4     (501) wheel        (0)       28 2023-07-12 18:29:45.000000 entail-0.1.0/docs/authors.rst
+-rwxr-xr-x   0 haowu4     (501) wheel        (0)     4747 2023-07-12 18:29:45.000000 entail-0.1.0/docs/conf.py
+-rw-r--r--   0 haowu4     (501) wheel        (0)       33 2023-07-12 18:29:45.000000 entail-0.1.0/docs/contributing.rst
+-rw-r--r--   0 haowu4     (501) wheel        (0)       28 2023-07-12 18:29:45.000000 entail-0.1.0/docs/history.rst
+-rw-r--r--   0 haowu4     (501) wheel        (0)      303 2023-07-12 18:29:45.000000 entail-0.1.0/docs/index.rst
+-rw-r--r--   0 haowu4     (501) wheel        (0)     1098 2023-07-12 18:29:45.000000 entail-0.1.0/docs/installation.rst
+-rw-r--r--   0 haowu4     (501) wheel        (0)      804 2023-07-12 18:29:45.000000 entail-0.1.0/docs/make.bat
+-rw-r--r--   0 haowu4     (501) wheel        (0)       27 2023-07-12 18:29:45.000000 entail-0.1.0/docs/readme.rst
+-rw-r--r--   0 haowu4     (501) wheel        (0)       67 2023-07-12 18:29:45.000000 entail-0.1.0/docs/usage.rst
+drwxr-xr-x   0 haowu4     (501) wheel        (0)        0 2023-07-12 18:30:58.594585 entail-0.1.0/entail/
+-rw-r--r--   0 haowu4     (501) wheel        (0)      116 2023-07-12 18:29:45.000000 entail-0.1.0/entail/__init__.py
+-rw-r--r--   0 haowu4     (501) wheel        (0)       19 2023-07-12 18:29:45.000000 entail-0.1.0/entail/entail.py
+drwxr-xr-x   0 haowu4     (501) wheel        (0)        0 2023-07-12 18:30:58.595147 entail-0.1.0/entail.egg-info/
+-rw-r--r--   0 haowu4     (501) wheel        (0)     1558 2023-07-12 18:30:58.000000 entail-0.1.0/entail.egg-info/PKG-INFO
+-rw-r--r--   0 haowu4     (501) wheel        (0)      479 2023-07-12 18:30:58.000000 entail-0.1.0/entail.egg-info/SOURCES.txt
+-rw-r--r--   0 haowu4     (501) wheel        (0)        1 2023-07-12 18:30:58.000000 entail-0.1.0/entail.egg-info/dependency_links.txt
+-rw-r--r--   0 haowu4     (501) wheel        (0)        1 2023-07-12 18:30:58.000000 entail-0.1.0/entail.egg-info/not-zip-safe
+-rw-r--r--   0 haowu4     (501) wheel        (0)        7 2023-07-12 18:30:58.000000 entail-0.1.0/entail.egg-info/top_level.txt
+-rw-r--r--   0 haowu4     (501) wheel        (0)      378 2023-07-12 18:30:58.595756 entail-0.1.0/setup.cfg
+-rw-r--r--   0 haowu4     (501) wheel        (0)     1202 2023-07-12 18:29:45.000000 entail-0.1.0/setup.py
+drwxr-xr-x   0 haowu4     (501) wheel        (0)        0 2023-07-12 18:30:58.595378 entail-0.1.0/tests/
+-rw-r--r--   0 haowu4     (501) wheel        (0)       36 2023-07-12 18:29:45.000000 entail-0.1.0/tests/__init__.py
+-rw-r--r--   0 haowu4     (501) wheel        (0)      382 2023-07-12 18:29:45.000000 entail-0.1.0/tests/test_entail.py
```

