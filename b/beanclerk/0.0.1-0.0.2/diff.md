# Comparing `tmp/beanclerk-0.0.1.tar.gz` & `tmp/beanclerk-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "beanclerk-0.0.1.tar", last modified: Mon May 15 19:30:12 2023, max compression
+gzip compressed data, was "beanclerk-0.0.2.tar", last modified: Thu Jul 13 15:01:01 2023, max compression
```

## Comparing `beanclerk-0.0.1.tar` & `beanclerk-0.0.2.tar`

### file list

```diff
@@ -1,25 +1,23 @@
-drwxr-xr-x   0 petr      (1000) petr      (1000)        0 2023-05-15 19:30:12.943777 beanclerk-0.0.1/
--rw-r--r--   0 petr      (1000) petr      (1000)     2579 2023-05-15 19:30:12.943777 beanclerk-0.0.1/PKG-INFO
--rw-r--r--   0 petr      (1000) petr      (1000)     2078 2023-05-15 19:11:00.000000 beanclerk-0.0.1/README.md
-drwxr-xr-x   0 petr      (1000) petr      (1000)        0 2023-05-15 19:30:12.942777 beanclerk-0.0.1/beanclerk/
--rw-r--r--   0 petr      (1000) petr      (1000)        0 2023-05-12 18:03:34.000000 beanclerk-0.0.1/beanclerk/__init__.py
-drwxr-xr-x   0 petr      (1000) petr      (1000)        0 2023-05-15 19:30:12.943777 beanclerk-0.0.1/beanclerk/apis/
--rw-r--r--   0 petr      (1000) petr      (1000)        0 2023-05-13 12:18:23.000000 beanclerk-0.0.1/beanclerk/apis/__init__.py
--rw-r--r--   0 petr      (1000) petr      (1000)     1029 2023-05-15 15:50:36.000000 beanclerk-0.0.1/beanclerk/apis/fio_banka.py
--rw-r--r--   0 petr      (1000) petr      (1000)     3096 2023-05-15 15:50:36.000000 beanclerk-0.0.1/beanclerk/bean_utils.py
--rw-r--r--   0 petr      (1000) petr      (1000)     1571 2023-05-15 14:25:04.000000 beanclerk-0.0.1/beanclerk/clerk.py
--rw-r--r--   0 petr      (1000) petr      (1000)     1095 2023-05-15 19:09:59.000000 beanclerk-0.0.1/beanclerk/cli.py
--rw-r--r--   0 petr      (1000) petr      (1000)       41 2023-05-15 14:14:55.000000 beanclerk-0.0.1/beanclerk/utils.py
-drwxr-xr-x   0 petr      (1000) petr      (1000)        0 2023-05-15 19:30:12.943777 beanclerk-0.0.1/beanclerk.egg-info/
--rw-r--r--   0 petr      (1000) petr      (1000)     2579 2023-05-15 19:30:12.000000 beanclerk-0.0.1/beanclerk.egg-info/PKG-INFO
--rw-r--r--   0 petr      (1000) petr      (1000)      443 2023-05-15 19:30:12.000000 beanclerk-0.0.1/beanclerk.egg-info/SOURCES.txt
--rw-r--r--   0 petr      (1000) petr      (1000)        1 2023-05-15 19:30:12.000000 beanclerk-0.0.1/beanclerk.egg-info/dependency_links.txt
--rw-r--r--   0 petr      (1000) petr      (1000)       49 2023-05-15 19:30:12.000000 beanclerk-0.0.1/beanclerk.egg-info/entry_points.txt
--rw-r--r--   0 petr      (1000) petr      (1000)      131 2023-05-15 19:30:12.000000 beanclerk-0.0.1/beanclerk.egg-info/requires.txt
--rw-r--r--   0 petr      (1000) petr      (1000)       10 2023-05-15 19:30:12.000000 beanclerk-0.0.1/beanclerk.egg-info/top_level.txt
--rw-r--r--   0 petr      (1000) petr      (1000)      909 2023-05-15 19:29:06.000000 beanclerk-0.0.1/pyproject.toml
--rw-r--r--   0 petr      (1000) petr      (1000)       38 2023-05-15 19:30:12.943777 beanclerk-0.0.1/setup.cfg
-drwxr-xr-x   0 petr      (1000) petr      (1000)        0 2023-05-15 19:30:12.943777 beanclerk-0.0.1/tests/
--rw-r--r--   0 petr      (1000) petr      (1000)     3963 2023-05-15 15:10:50.000000 beanclerk-0.0.1/tests/test_bean_utils.py
--rw-r--r--   0 petr      (1000) petr      (1000)     1125 2023-05-15 15:32:44.000000 beanclerk-0.0.1/tests/test_clerk.py
--rw-r--r--   0 petr      (1000) petr      (1000)     1716 2023-05-15 15:09:02.000000 beanclerk-0.0.1/tests/test_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:01:01.580780 beanclerk-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    18342 2023-07-13 15:00:47.000000 beanclerk-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    22394 2023-07-13 15:01:01.580780 beanclerk-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-07-13 15:00:47.000000 beanclerk-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:01:01.576780 beanclerk-0.0.2/beanclerk/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 15:00:47.000000 beanclerk-0.0.2/beanclerk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-07-13 15:00:47.000000 beanclerk-0.0.2/beanclerk/bean_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-07-13 15:00:47.000000 beanclerk-0.0.2/beanclerk/clerk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-07-13 15:00:47.000000 beanclerk-0.0.2/beanclerk/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-07-13 15:00:47.000000 beanclerk-0.0.2/beanclerk/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:01:01.580780 beanclerk-0.0.2/beanclerk/importers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-07-13 15:00:47.000000 beanclerk-0.0.2/beanclerk/importers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4649 2023-07-13 15:00:47.000000 beanclerk-0.0.2/beanclerk/importers/banka_creditas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2789 2023-07-13 15:00:47.000000 beanclerk-0.0.2/beanclerk/importers/fio_banka.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:01:01.580780 beanclerk-0.0.2/beanclerk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    22394 2023-07-13 15:01:01.000000 beanclerk-0.0.2/beanclerk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-07-13 15:01:01.000000 beanclerk-0.0.2/beanclerk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 15:01:01.000000 beanclerk-0.0.2/beanclerk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-13 15:01:01.000000 beanclerk-0.0.2/beanclerk.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-13 15:01:01.000000 beanclerk-0.0.2/beanclerk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-13 15:01:01.000000 beanclerk-0.0.2/beanclerk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-07-13 15:00:47.000000 beanclerk-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 15:01:01.580780 beanclerk-0.0.2/setup.cfg
```

