# Comparing `tmp/bank-of-ghana-fx-rates-0.1.8.tar.gz` & `tmp/bank-of-ghana-fx-rates-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/bank-of-ghana-fx-rates-0.1.8.tar", last modified: Thu Jul 13 21:36:38 2023, max compression
+gzip compressed data, was "bank-of-ghana-fx-rates-1.0.1.tar", last modified: Sun Aug  7 00:15:54 2022, max compression
```

## Comparing `bank-of-ghana-fx-rates-0.1.8.tar` & `bank-of-ghana-fx-rates-1.0.1.tar`

### file list

```diff
@@ -1,19 +1,15 @@
-drwxr-xr-x   0 tsiameh    (501) staff       (20)        0 2023-07-13 21:36:38.000000 bank-of-ghana-fx-rates-0.1.8/
--rw-r--r--   0 tsiameh    (501) staff       (20)     1074 2021-01-13 02:45:22.000000 bank-of-ghana-fx-rates-0.1.8/LICENSE
--rw-r--r--   0 tsiameh    (501) staff       (20)     3515 2023-07-13 21:36:38.000000 bank-of-ghana-fx-rates-0.1.8/PKG-INFO
--rw-r--r--   0 tsiameh    (501) staff       (20)     1783 2023-07-13 20:24:44.000000 bank-of-ghana-fx-rates-0.1.8/README.md
-drwxr-xr-x   0 tsiameh    (501) staff       (20)        0 2023-07-13 21:36:38.000000 bank-of-ghana-fx-rates-0.1.8/bank_of_ghana_fx_rates.egg-info/
--rw-r--r--   0 tsiameh    (501) staff       (20)     3515 2023-07-13 21:36:38.000000 bank-of-ghana-fx-rates-0.1.8/bank_of_ghana_fx_rates.egg-info/PKG-INFO
--rw-r--r--   0 tsiameh    (501) staff       (20)      362 2023-07-13 21:36:38.000000 bank-of-ghana-fx-rates-0.1.8/bank_of_ghana_fx_rates.egg-info/SOURCES.txt
--rw-r--r--   0 tsiameh    (501) staff       (20)        1 2023-07-13 21:36:38.000000 bank-of-ghana-fx-rates-0.1.8/bank_of_ghana_fx_rates.egg-info/dependency_links.txt
--rw-r--r--   0 tsiameh    (501) staff       (20)       44 2023-07-13 21:36:38.000000 bank-of-ghana-fx-rates-0.1.8/bank_of_ghana_fx_rates.egg-info/entry_points.txt
--rw-r--r--   0 tsiameh    (501) staff       (20)       48 2023-07-13 21:36:38.000000 bank-of-ghana-fx-rates-0.1.8/bank_of_ghana_fx_rates.egg-info/requires.txt
--rw-r--r--   0 tsiameh    (501) staff       (20)        4 2023-07-13 21:36:38.000000 bank-of-ghana-fx-rates-0.1.8/bank_of_ghana_fx_rates.egg-info/top_level.txt
-drwxr-xr-x   0 tsiameh    (501) staff       (20)        0 2023-07-13 21:36:38.000000 bank-of-ghana-fx-rates-0.1.8/bog/
--rw-r--r--   0 tsiameh    (501) staff       (20)        0 2021-01-13 02:45:22.000000 bank-of-ghana-fx-rates-0.1.8/bog/__init__.py
--rw-r--r--   0 tsiameh    (501) staff       (20)      986 2023-07-13 20:05:34.000000 bank-of-ghana-fx-rates-0.1.8/bog/scraper.py
--rw-r--r--   0 tsiameh    (501) staff       (20)     5587 2023-07-13 21:17:20.000000 bank-of-ghana-fx-rates-0.1.8/bog/utils.py
--rw-r--r--   0 tsiameh    (501) staff       (20)       38 2023-07-13 21:36:38.000000 bank-of-ghana-fx-rates-0.1.8/setup.cfg
--rw-r--r--   0 tsiameh    (501) staff       (20)     1902 2023-07-13 20:18:46.000000 bank-of-ghana-fx-rates-0.1.8/setup.py
-drwxr-xr-x   0 tsiameh    (501) staff       (20)        0 2023-07-13 21:36:38.000000 bank-of-ghana-fx-rates-0.1.8/tests/
--rw-r--r--   0 tsiameh    (501) staff       (20)     4878 2023-07-12 20:28:00.000000 bank-of-ghana-fx-rates-0.1.8/tests/test.py
+drwxr-xr-x   0 tsiameh    (501) staff       (20)        0 2022-08-07 00:15:54.357895 bank-of-ghana-fx-rates-1.0.1/
+-rw-r--r--   0 tsiameh    (501) staff       (20)     1074 2021-01-13 02:45:22.000000 bank-of-ghana-fx-rates-1.0.1/LICENSE
+-rw-r--r--   0 tsiameh    (501) staff       (20)     2540 2022-08-07 00:15:54.357608 bank-of-ghana-fx-rates-1.0.1/PKG-INFO
+-rw-r--r--   0 tsiameh    (501) staff       (20)     1448 2022-08-07 00:15:30.000000 bank-of-ghana-fx-rates-1.0.1/README.md
+drwxr-xr-x   0 tsiameh    (501) staff       (20)        0 2022-08-07 00:15:54.356610 bank-of-ghana-fx-rates-1.0.1/bank_of_ghana_fx_rates.egg-info/
+-rw-r--r--   0 tsiameh    (501) staff       (20)     2540 2022-08-07 00:15:54.000000 bank-of-ghana-fx-rates-1.0.1/bank_of_ghana_fx_rates.egg-info/PKG-INFO
+-rw-r--r--   0 tsiameh    (501) staff       (20)      286 2022-08-07 00:15:54.000000 bank-of-ghana-fx-rates-1.0.1/bank_of_ghana_fx_rates.egg-info/SOURCES.txt
+-rw-r--r--   0 tsiameh    (501) staff       (20)        1 2022-08-07 00:15:54.000000 bank-of-ghana-fx-rates-1.0.1/bank_of_ghana_fx_rates.egg-info/dependency_links.txt
+-rw-r--r--   0 tsiameh    (501) staff       (20)       48 2022-08-07 00:15:54.000000 bank-of-ghana-fx-rates-1.0.1/bank_of_ghana_fx_rates.egg-info/requires.txt
+-rw-r--r--   0 tsiameh    (501) staff       (20)        4 2022-08-07 00:15:54.000000 bank-of-ghana-fx-rates-1.0.1/bank_of_ghana_fx_rates.egg-info/top_level.txt
+drwxr-xr-x   0 tsiameh    (501) staff       (20)        0 2022-08-07 00:15:54.357195 bank-of-ghana-fx-rates-1.0.1/bog/
+-rw-r--r--   0 tsiameh    (501) staff       (20)        0 2021-01-13 02:45:22.000000 bank-of-ghana-fx-rates-1.0.1/bog/__init__.py
+-rw-r--r--   0 tsiameh    (501) staff       (20)     5540 2022-08-07 00:15:30.000000 bank-of-ghana-fx-rates-1.0.1/bog/scraper.py
+-rw-r--r--   0 tsiameh    (501) staff       (20)       38 2022-08-07 00:15:54.358003 bank-of-ghana-fx-rates-1.0.1/setup.cfg
+-rw-r--r--   0 tsiameh    (501) staff       (20)     3613 2022-08-07 00:15:30.000000 bank-of-ghana-fx-rates-1.0.1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `bank-of-ghana-fx-rates-0.1.8/LICENSE` & `bank-of-ghana-fx-rates-1.0.1/LICENSE`

 * *Files identical despite different names*

