# Comparing `tmp/index_calculator-0.7.6.tar.gz` & `tmp/index_calculator-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "index_calculator-0.7.6.tar", last modified: Mon Jun 19 13:04:11 2023, max compression
+gzip compressed data, was "index_calculator-0.8.0.tar", last modified: Thu Jul 13 13:27:22 2023, max compression
```

## Comparing `index_calculator-0.7.6.tar` & `index_calculator-0.8.0.tar`

### file list

```diff
@@ -1,79 +1,56 @@
-drwxr-xr-x   0 g300100  (25516) ch0636    (1303)        0 2023-06-19 13:04:11.000000 index_calculator-0.7.6/
--rw-r--r--   0 g300100  (25516) ch0636    (1303)      170 2023-06-14 13:50:23.000000 index_calculator-0.7.6/AUTHORS.rst
--rw-r--r--   0 g300100  (25516) ch0636    (1303)     3640 2023-06-14 13:50:23.000000 index_calculator-0.7.6/CONTRIBUTING.rst
--rw-r--r--   0 g300100  (25516) ch0636    (1303)     5753 2023-06-19 13:01:38.000000 index_calculator-0.7.6/HISTORY.rst
--rw-r--r--   0 g300100  (25516) ch0636    (1303)     1075 2023-06-14 13:50:23.000000 index_calculator-0.7.6/LICENSE
--rw-r--r--   0 g300100  (25516) ch0636    (1303)      262 2023-06-14 13:50:23.000000 index_calculator-0.7.6/MANIFEST.in
--rw-r--r--   0 g300100  (25516) ch0636    (1303)    11666 2023-06-19 13:04:11.000000 index_calculator-0.7.6/PKG-INFO
--rw-r--r--   0 g300100  (25516) ch0636    (1303)     5108 2023-06-14 13:50:23.000000 index_calculator-0.7.6/README.rst
-drwxr-xr-x   0 g300100  (25516) ch0636    (1303)        0 2023-06-19 13:04:11.000000 index_calculator-0.7.6/docs/
--rw-r--r--   0 g300100  (25516) ch0636    (1303)      617 2023-06-14 13:50:23.000000 index_calculator-0.7.6/docs/Makefile
--rw-r--r--   0 g300100  (25516) ch0636    (1303)      555 2023-06-14 13:50:23.000000 index_calculator-0.7.6/docs/api.rst
--rw-r--r--   0 g300100  (25516) ch0636    (1303)       28 2023-06-14 13:50:23.000000 index_calculator-0.7.6/docs/authors.rst
--rwxr-xr-x   0 g300100  (25516) ch0636    (1303)     7680 2023-06-14 13:50:23.000000 index_calculator-0.7.6/docs/conf.py
--rw-r--r--   0 g300100  (25516) ch0636    (1303)       33 2023-06-14 13:50:23.000000 index_calculator-0.7.6/docs/contributing.rst
--rw-r--r--   0 g300100  (25516) ch0636    (1303)       28 2023-06-14 13:50:23.000000 index_calculator-0.7.6/docs/history.rst
--rw-r--r--   0 g300100  (25516) ch0636    (1303)      351 2023-06-14 13:50:23.000000 index_calculator-0.7.6/docs/index.rst
--rw-r--r--   0 g300100  (25516) ch0636    (1303)      174 2023-06-14 13:50:23.000000 index_calculator-0.7.6/docs/indices.rst
--rw-r--r--   0 g300100  (25516) ch0636    (1303)     1218 2023-06-14 13:50:23.000000 index_calculator-0.7.6/docs/installation.rst
--rw-r--r--   0 g300100  (25516) ch0636    (1303)      778 2023-06-14 13:50:23.000000 index_calculator-0.7.6/docs/make.bat
--rw-r--r--   0 g300100  (25516) ch0636    (1303)       27 2023-06-14 13:50:23.000000 index_calculator-0.7.6/docs/readme.rst
--rw-r--r--   0 g300100  (25516) ch0636    (1303)       87 2023-06-14 13:50:23.000000 index_calculator-0.7.6/docs/usage.rst
-drwxr-xr-x   0 g300100  (25516) ch0636    (1303)        0 2023-06-19 13:04:11.000000 index_calculator-0.7.6/index_calculator/
--rw-r--r--   0 g300100  (25516) ch0636    (1303)     1039 2023-06-19 13:01:53.000000 index_calculator-0.7.6/index_calculator/__init__.py
--rw-r--r--   0 g300100  (25516) ch0636    (1303)     4645 2023-06-14 13:50:23.000000 index_calculator-0.7.6/index_calculator/_ci_netcdfattrs.py
--rw-r--r--   0 g300100  (25516) ch0636    (1303)      805 2023-06-15 09:02:15.000000 index_calculator-0.7.6/index_calculator/_consts.py
--rw-r--r--   0 g300100  (25516) ch0636    (1303)    76343 2023-06-16 07:57:47.000000 index_calculator-0.7.6/index_calculator/_indices.py
--rw-r--r--   0 g300100  (25516) ch0636    (1303)     5213 2023-06-14 13:50:23.000000 index_calculator-0.7.6/index_calculator/_outputwriter.py
--rw-r--r--   0 g300100  (25516) ch0636    (1303)     5385 2023-06-15 09:02:15.000000 index_calculator-0.7.6/index_calculator/_postprocessing.py
--rw-r--r--   0 g300100  (25516) ch0636    (1303)     4800 2023-06-15 09:02:15.000000 index_calculator-0.7.6/index_calculator/_preprocessing.py
--rw-r--r--   0 g300100  (25516) ch0636    (1303)     7707 2023-06-19 08:01:38.000000 index_calculator-0.7.6/index_calculator/_processing.py
--rw-r--r--   0 g300100  (25516) ch0636    (1303)      643 2023-06-15 09:02:15.000000 index_calculator-0.7.6/index_calculator/_tables.py
--rw-r--r--   0 g300100  (25516) ch0636    (1303)     1988 2023-06-14 13:50:23.000000 index_calculator-0.7.6/index_calculator/_utils.py
--rw-r--r--   0 g300100  (25516) ch0636    (1303)     2147 2023-06-14 13:50:23.000000 index_calculator-0.7.6/index_calculator/cli.py
--rw-r--r--   0 g300100  (25516) ch0636    (1303)     2427 2023-06-14 13:50:24.000000 index_calculator-0.7.6/index_calculator/index_calculator.py
-drwxr-xr-x   0 g300100  (25516) ch0636    (1303)        0 2023-06-19 13:04:11.000000 index_calculator-0.7.6/index_calculator/tables/
--rw-r--r--   0 g300100  (25516) ch0636    (1303)      323 2023-06-15 09:02:16.000000 index_calculator-0.7.6/index_calculator/tables/cf_conversion.json
--rw-r--r--   0 g300100  (25516) ch0636    (1303)      369 2023-06-15 09:02:16.000000 index_calculator-0.7.6/index_calculator/tables/convert_to_frequencies.json
--rw-r--r--   0 g300100  (25516) ch0636    (1303)     1507 2023-06-16 07:57:47.000000 index_calculator-0.7.6/index_calculator/tables/input_vars.json
--rw-r--r--   0 g300100  (25516) ch0636    (1303)    19310 2023-06-16 07:57:47.000000 index_calculator-0.7.6/index_calculator/tables/metadata.json
--rw-r--r--   0 g300100  (25516) ch0636    (1303)     3085 2023-06-14 13:50:24.000000 index_calculator-0.7.6/index_calculator/tables/projects.json
--rw-r--r--   0 g300100  (25516) ch0636    (1303)     1191 2023-06-14 13:50:24.000000 index_calculator-0.7.6/index_calculator/tables/xcalc.json
-drwxr-xr-x   0 g300100  (25516) ch0636    (1303)        0 2023-06-19 13:04:11.000000 index_calculator-0.7.6/index_calculator.egg-info/
--rw-r--r--   0 g300100  (25516) ch0636    (1303)    11666 2023-06-19 13:04:10.000000 index_calculator-0.7.6/index_calculator.egg-info/PKG-INFO
--rw-r--r--   0 g300100  (25516) ch0636    (1303)     1704 2023-06-19 13:04:11.000000 index_calculator-0.7.6/index_calculator.egg-info/SOURCES.txt
--rw-r--r--   0 g300100  (25516) ch0636    (1303)        1 2023-06-19 13:04:10.000000 index_calculator-0.7.6/index_calculator.egg-info/dependency_links.txt
--rw-r--r--   0 g300100  (25516) ch0636    (1303)       63 2023-06-19 13:04:10.000000 index_calculator-0.7.6/index_calculator.egg-info/entry_points.txt
--rw-r--r--   0 g300100  (25516) ch0636    (1303)        1 2023-06-19 13:04:10.000000 index_calculator-0.7.6/index_calculator.egg-info/not-zip-safe
--rw-r--r--   0 g300100  (25516) ch0636    (1303)       78 2023-06-19 13:04:10.000000 index_calculator-0.7.6/index_calculator.egg-info/requires.txt
--rw-r--r--   0 g300100  (25516) ch0636    (1303)       17 2023-06-19 13:04:10.000000 index_calculator-0.7.6/index_calculator.egg-info/top_level.txt
--rw-r--r--   0 g300100  (25516) ch0636    (1303)       38 2023-06-19 13:04:11.000000 index_calculator-0.7.6/setup.cfg
--rw-r--r--   0 g300100  (25516) ch0636    (1303)     2103 2023-06-14 13:50:24.000000 index_calculator-0.7.6/setup.py
-drwxr-xr-x   0 g300100  (25516) ch0636    (1303)        0 2023-06-19 13:04:11.000000 index_calculator-0.7.6/tests/
--rw-r--r--   0 g300100  (25516) ch0636    (1303)       46 2023-06-14 13:50:24.000000 index_calculator-0.7.6/tests/__init__.py
--rw-r--r--   0 g300100  (25516) ch0636    (1303)     8385 2023-06-19 12:56:16.000000 index_calculator-0.7.6/tests/conftest.py
-drwxr-xr-x   0 g300100  (25516) ch0636    (1303)        0 2023-06-19 13:04:11.000000 index_calculator-0.7.6/tests/cordex/
-drwxr-xr-x   0 g300100  (25516) ch0636    (1303)        0 2023-06-19 13:04:11.000000 index_calculator-0.7.6/tests/cordex/EUR-11/
-drwxr-xr-x   0 g300100  (25516) ch0636    (1303)        0 2023-06-19 13:04:11.000000 index_calculator-0.7.6/tests/cordex/EUR-11/TEST/
-drwxr-xr-x   0 g300100  (25516) ch0636    (1303)        0 2023-06-19 13:04:11.000000 index_calculator-0.7.6/tests/cordex/EUR-11/TEST/GERICS/
-drwxr-xr-x   0 g300100  (25516) ch0636    (1303)        0 2023-06-19 13:04:11.000000 index_calculator-0.7.6/tests/cordex/EUR-11/TEST/GERICS/MPI-M-MPI-ESM-LR/
-drwxr-xr-x   0 g300100  (25516) ch0636    (1303)        0 2023-06-19 13:04:11.000000 index_calculator-0.7.6/tests/cordex/EUR-11/TEST/GERICS/MPI-M-MPI-ESM-LR/historical/
-drwxr-xr-x   0 g300100  (25516) ch0636    (1303)        0 2023-06-19 13:04:11.000000 index_calculator-0.7.6/tests/cordex/EUR-11/TEST/GERICS/MPI-M-MPI-ESM-LR/historical/r3i1p1/
-drwxr-xr-x   0 g300100  (25516) ch0636    (1303)        0 2023-06-19 13:04:11.000000 index_calculator-0.7.6/tests/cordex/EUR-11/TEST/GERICS/MPI-M-MPI-ESM-LR/historical/r3i1p1/GERICS-REMO2015/
-drwxr-xr-x   0 g300100  (25516) ch0636    (1303)        0 2023-06-19 13:04:11.000000 index_calculator-0.7.6/tests/cordex/EUR-11/TEST/GERICS/MPI-M-MPI-ESM-LR/historical/r3i1p1/GERICS-REMO2015/v1/
-drwxr-xr-x   0 g300100  (25516) ch0636    (1303)        0 2023-06-19 13:04:11.000000 index_calculator-0.7.6/tests/cordex/EUR-11/TEST/GERICS/MPI-M-MPI-ESM-LR/historical/r3i1p1/GERICS-REMO2015/v1/week/
-drwxr-xr-x   0 g300100  (25516) ch0636    (1303)        0 2023-06-19 13:04:11.000000 index_calculator-0.7.6/tests/cordex/EUR-11/TEST/GERICS/MPI-M-MPI-ESM-LR/historical/r3i1p1/GERICS-REMO2015/v1/week/TG/
-drwxr-xr-x   0 g300100  (25516) ch0636    (1303)        0 2023-06-19 13:04:11.000000 index_calculator-0.7.6/tests/cordex/EUR-11/TEST/GERICS/MPI-M-MPI-ESM-LR/historical/r3i1p1/GERICS-REMO2015/v1/week/TG/xcalc_0.7.5/
--rw-r--r--   0 g300100  (25516) ch0636    (1303)  7745308 2023-06-19 12:13:10.000000 index_calculator-0.7.6/tests/cordex/EUR-11/TEST/GERICS/MPI-M-MPI-ESM-LR/historical/r3i1p1/GERICS-REMO2015/v1/week/TG/xcalc_0.7.5/TG_EUR-11_MPI-M-MPI-ESM-LR_historical_r3i1p1_GERICS-REMO2015_v1_day_TEST_week_20010101-20010101.nc
-drwxr-xr-x   0 g300100  (25516) ch0636    (1303)        0 2023-06-19 13:04:11.000000 index_calculator-0.7.6/tests/cordex/EUR-11/TEST/GERICS/MPI-M-MPI-ESM-LR/rcp85/
-drwxr-xr-x   0 g300100  (25516) ch0636    (1303)        0 2023-06-19 13:04:11.000000 index_calculator-0.7.6/tests/cordex/EUR-11/TEST/GERICS/MPI-M-MPI-ESM-LR/rcp85/r3i1p1/
-drwxr-xr-x   0 g300100  (25516) ch0636    (1303)        0 2023-06-19 13:04:11.000000 index_calculator-0.7.6/tests/cordex/EUR-11/TEST/GERICS/MPI-M-MPI-ESM-LR/rcp85/r3i1p1/GERICS-REMO2015/
-drwxr-xr-x   0 g300100  (25516) ch0636    (1303)        0 2023-06-19 13:04:11.000000 index_calculator-0.7.6/tests/cordex/EUR-11/TEST/GERICS/MPI-M-MPI-ESM-LR/rcp85/r3i1p1/GERICS-REMO2015/v1/
-drwxr-xr-x   0 g300100  (25516) ch0636    (1303)        0 2023-06-19 13:04:11.000000 index_calculator-0.7.6/tests/cordex/EUR-11/TEST/GERICS/MPI-M-MPI-ESM-LR/rcp85/r3i1p1/GERICS-REMO2015/v1/week/
-drwxr-xr-x   0 g300100  (25516) ch0636    (1303)        0 2023-06-19 13:04:11.000000 index_calculator-0.7.6/tests/cordex/EUR-11/TEST/GERICS/MPI-M-MPI-ESM-LR/rcp85/r3i1p1/GERICS-REMO2015/v1/week/TG/
-drwxr-xr-x   0 g300100  (25516) ch0636    (1303)        0 2023-06-19 13:04:11.000000 index_calculator-0.7.6/tests/cordex/EUR-11/TEST/GERICS/MPI-M-MPI-ESM-LR/rcp85/r3i1p1/GERICS-REMO2015/v1/week/TG/xcalc_0.7.5/
--rw-r--r--   0 g300100  (25516) ch0636    (1303)  2196580 2023-06-19 12:50:45.000000 index_calculator-0.7.6/tests/cordex/EUR-11/TEST/GERICS/MPI-M-MPI-ESM-LR/rcp85/r3i1p1/GERICS-REMO2015/v1/week/TG/xcalc_0.7.5/TG_EUR-11_MPI-M-MPI-ESM-LR_rcp85_r3i1p1_GERICS-REMO2015_v1_1hr_TEST_week_20070101-20070101.nc
--rw-r--r--   0 g300100  (25516) ch0636    (1303)      365 2023-06-19 12:51:50.000000 index_calculator-0.7.6/tests/test_cli.py
--rw-r--r--   0 g300100  (25516) ch0636    (1303)      532 2023-06-14 13:50:24.000000 index_calculator-0.7.6/tests/test_index_calculator.py
--rw-r--r--   0 g300100  (25516) ch0636    (1303)    16193 2023-06-16 07:57:47.000000 index_calculator-0.7.6/tests/test_indices.py
--rw-r--r--   0 g300100  (25516) ch0636    (1303)     2645 2023-06-19 12:51:50.000000 index_calculator-0.7.6/tests/test_xcalc.py
+drwxr-xr-x   0 g300100  (25516) ch0636    (1303)        0 2023-07-13 13:27:22.000000 index_calculator-0.8.0/
+-rw-r--r--   0 g300100  (25516) ch0636    (1303)      170 2023-06-30 09:38:29.000000 index_calculator-0.8.0/AUTHORS.rst
+-rw-r--r--   0 g300100  (25516) ch0636    (1303)     3640 2023-06-30 09:38:29.000000 index_calculator-0.8.0/CONTRIBUTING.rst
+-rw-r--r--   0 g300100  (25516) ch0636    (1303)     6418 2023-07-13 13:23:24.000000 index_calculator-0.8.0/HISTORY.rst
+-rw-r--r--   0 g300100  (25516) ch0636    (1303)     1075 2023-06-30 09:38:29.000000 index_calculator-0.8.0/LICENSE
+-rw-r--r--   0 g300100  (25516) ch0636    (1303)      262 2023-06-30 09:38:29.000000 index_calculator-0.8.0/MANIFEST.in
+-rw-r--r--   0 g300100  (25516) ch0636    (1303)    12331 2023-07-13 13:27:22.000000 index_calculator-0.8.0/PKG-INFO
+-rw-r--r--   0 g300100  (25516) ch0636    (1303)     5108 2023-06-30 09:38:29.000000 index_calculator-0.8.0/README.rst
+drwxr-xr-x   0 g300100  (25516) ch0636    (1303)        0 2023-07-13 13:27:22.000000 index_calculator-0.8.0/docs/
+-rw-r--r--   0 g300100  (25516) ch0636    (1303)      617 2023-06-30 09:38:29.000000 index_calculator-0.8.0/docs/Makefile
+-rw-r--r--   0 g300100  (25516) ch0636    (1303)      555 2023-06-30 09:38:29.000000 index_calculator-0.8.0/docs/api.rst
+-rw-r--r--   0 g300100  (25516) ch0636    (1303)       28 2023-06-30 09:38:29.000000 index_calculator-0.8.0/docs/authors.rst
+-rwxr-xr-x   0 g300100  (25516) ch0636    (1303)     7680 2023-06-30 09:38:29.000000 index_calculator-0.8.0/docs/conf.py
+-rw-r--r--   0 g300100  (25516) ch0636    (1303)       33 2023-06-30 09:38:29.000000 index_calculator-0.8.0/docs/contributing.rst
+-rw-r--r--   0 g300100  (25516) ch0636    (1303)       28 2023-06-30 09:38:29.000000 index_calculator-0.8.0/docs/history.rst
+-rw-r--r--   0 g300100  (25516) ch0636    (1303)      351 2023-06-30 09:38:29.000000 index_calculator-0.8.0/docs/index.rst
+-rw-r--r--   0 g300100  (25516) ch0636    (1303)      174 2023-06-30 09:38:29.000000 index_calculator-0.8.0/docs/indices.rst
+-rw-r--r--   0 g300100  (25516) ch0636    (1303)     1218 2023-06-30 09:38:29.000000 index_calculator-0.8.0/docs/installation.rst
+-rw-r--r--   0 g300100  (25516) ch0636    (1303)      778 2023-06-30 09:38:29.000000 index_calculator-0.8.0/docs/make.bat
+-rw-r--r--   0 g300100  (25516) ch0636    (1303)       27 2023-06-30 09:38:29.000000 index_calculator-0.8.0/docs/readme.rst
+-rw-r--r--   0 g300100  (25516) ch0636    (1303)       87 2023-06-30 09:38:29.000000 index_calculator-0.8.0/docs/usage.rst
+drwxr-xr-x   0 g300100  (25516) ch0636    (1303)        0 2023-07-13 13:27:22.000000 index_calculator-0.8.0/index_calculator/
+-rw-r--r--   0 g300100  (25516) ch0636    (1303)      968 2023-07-13 13:23:47.000000 index_calculator-0.8.0/index_calculator/__init__.py
+-rw-r--r--   0 g300100  (25516) ch0636    (1303)     4645 2023-06-30 09:38:29.000000 index_calculator-0.8.0/index_calculator/_ci_netcdfattrs.py
+-rw-r--r--   0 g300100  (25516) ch0636    (1303)      805 2023-06-30 09:38:29.000000 index_calculator-0.8.0/index_calculator/_consts.py
+-rw-r--r--   0 g300100  (25516) ch0636    (1303)    84925 2023-06-30 12:12:52.000000 index_calculator-0.8.0/index_calculator/_indices.py
+-rw-r--r--   0 g300100  (25516) ch0636    (1303)     5231 2023-06-30 12:12:52.000000 index_calculator-0.8.0/index_calculator/_outputwriter.py
+-rw-r--r--   0 g300100  (25516) ch0636    (1303)     5385 2023-06-30 09:38:29.000000 index_calculator-0.8.0/index_calculator/_postprocessing.py
+-rw-r--r--   0 g300100  (25516) ch0636    (1303)     3666 2023-07-13 13:16:21.000000 index_calculator-0.8.0/index_calculator/_preprocessing.py
+-rw-r--r--   0 g300100  (25516) ch0636    (1303)     7860 2023-06-30 12:12:52.000000 index_calculator-0.8.0/index_calculator/_processing.py
+-rw-r--r--   0 g300100  (25516) ch0636    (1303)      529 2023-07-13 13:16:21.000000 index_calculator-0.8.0/index_calculator/_tables.py
+-rw-r--r--   0 g300100  (25516) ch0636    (1303)     1988 2023-06-30 09:38:29.000000 index_calculator-0.8.0/index_calculator/_utils.py
+-rw-r--r--   0 g300100  (25516) ch0636    (1303)     2147 2023-06-30 09:38:29.000000 index_calculator-0.8.0/index_calculator/cli.py
+-rw-r--r--   0 g300100  (25516) ch0636    (1303)     2427 2023-06-30 09:38:29.000000 index_calculator-0.8.0/index_calculator/index_calculator.py
+drwxr-xr-x   0 g300100  (25516) ch0636    (1303)        0 2023-07-13 13:27:22.000000 index_calculator-0.8.0/index_calculator/tables/
+-rw-r--r--   0 g300100  (25516) ch0636    (1303)     1631 2023-06-30 12:12:52.000000 index_calculator-0.8.0/index_calculator/tables/input_vars.json
+-rw-r--r--   0 g300100  (25516) ch0636    (1303)    21402 2023-06-30 12:12:52.000000 index_calculator-0.8.0/index_calculator/tables/metadata.json
+-rw-r--r--   0 g300100  (25516) ch0636    (1303)     3099 2023-06-30 12:12:52.000000 index_calculator-0.8.0/index_calculator/tables/projects.json
+-rw-r--r--   0 g300100  (25516) ch0636    (1303)     1191 2023-06-30 09:38:29.000000 index_calculator-0.8.0/index_calculator/tables/xcalc.json
+drwxr-xr-x   0 g300100  (25516) ch0636    (1303)        0 2023-07-13 13:27:22.000000 index_calculator-0.8.0/index_calculator.egg-info/
+-rw-r--r--   0 g300100  (25516) ch0636    (1303)    12331 2023-07-13 13:27:21.000000 index_calculator-0.8.0/index_calculator.egg-info/PKG-INFO
+-rw-r--r--   0 g300100  (25516) ch0636    (1303)     1209 2023-07-13 13:27:22.000000 index_calculator-0.8.0/index_calculator.egg-info/SOURCES.txt
+-rw-r--r--   0 g300100  (25516) ch0636    (1303)        1 2023-07-13 13:27:21.000000 index_calculator-0.8.0/index_calculator.egg-info/dependency_links.txt
+-rw-r--r--   0 g300100  (25516) ch0636    (1303)       63 2023-07-13 13:27:21.000000 index_calculator-0.8.0/index_calculator.egg-info/entry_points.txt
+-rw-r--r--   0 g300100  (25516) ch0636    (1303)        1 2023-07-13 13:27:21.000000 index_calculator-0.8.0/index_calculator.egg-info/not-zip-safe
+-rw-r--r--   0 g300100  (25516) ch0636    (1303)       78 2023-07-13 13:27:21.000000 index_calculator-0.8.0/index_calculator.egg-info/requires.txt
+-rw-r--r--   0 g300100  (25516) ch0636    (1303)       17 2023-07-13 13:27:21.000000 index_calculator-0.8.0/index_calculator.egg-info/top_level.txt
+-rw-r--r--   0 g300100  (25516) ch0636    (1303)       38 2023-07-13 13:27:22.000000 index_calculator-0.8.0/setup.cfg
+-rw-r--r--   0 g300100  (25516) ch0636    (1303)     2103 2023-06-30 09:38:29.000000 index_calculator-0.8.0/setup.py
+drwxr-xr-x   0 g300100  (25516) ch0636    (1303)        0 2023-07-13 13:27:22.000000 index_calculator-0.8.0/tests/
+-rw-r--r--   0 g300100  (25516) ch0636    (1303)       46 2023-06-30 09:38:29.000000 index_calculator-0.8.0/tests/__init__.py
+-rw-r--r--   0 g300100  (25516) ch0636    (1303)     7453 2023-07-13 13:16:21.000000 index_calculator-0.8.0/tests/conftest.py
+-rw-r--r--   0 g300100  (25516) ch0636    (1303)      365 2023-06-30 09:38:29.000000 index_calculator-0.8.0/tests/test_cli.py
+-rw-r--r--   0 g300100  (25516) ch0636    (1303)      532 2023-06-30 09:38:29.000000 index_calculator-0.8.0/tests/test_index_calculator.py
+-rw-r--r--   0 g300100  (25516) ch0636    (1303)    17552 2023-06-30 12:12:52.000000 index_calculator-0.8.0/tests/test_indices.py
+-rw-r--r--   0 g300100  (25516) ch0636    (1303)     2259 2023-07-13 13:16:21.000000 index_calculator-0.8.0/tests/test_xcalc.py
```

### Comparing `index_calculator-0.7.6/CONTRIBUTING.rst` & `index_calculator-0.8.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `index_calculator-0.7.6/HISTORY.rst` & `index_calculator-0.8.0/HISTORY.rst`

 * *Files 9% similar despite different names*

```diff
@@ -69,14 +69,15 @@
 * restructuring time encoding
 * properties removed
 
 0.5.0 (2023-01-04)
 ------------------
 
 * new indices:
+
   * CSf (Number of cold spells)
   * HSf (Number of hot spells)
   * HSx (Maximum length of hot spells)
   * SD (Number od snow days)
   * SCD (Snow cover duration)
   * Sint (Snowfall intensity)
   * Sfreq (Snowfall freqeuncy)
@@ -118,21 +119,23 @@
 
 * time controlling to pyhomogenize
 
 0.6.0 (2023-03-03)
 ------------------
 
 * new indices:
+
   * HW: maximum length of heat waves
   * GSS: start of growing season
   * GSE: end of growing season
   * FFS: start of frost-free season
   * FFE: end of frost-free season
   * RRm: mean daily precipitation
   * RRYYp: precipitation percentile value
+
 * rename RYYp to RYYpABS and RDYYP to RYYp according to ICCLIM
 * optional argument perc woth percentile indicators
 
 0.6.1 (2023-03-09)
 ------------------
 
 * some metadata corrections
@@ -183,14 +186,15 @@
 
 * calculating percentile indices with non-standard calendar
 
 0.7.2 (2023-05-10)
 ------------------
 
 * new indicators implemented:
+
   * FG (mean daily wind speed)
   * FGn (minimum od mean daily wind speed)
   * FGx (maximum of mean daily wind speed)
   * FX (mean of maximum daily wind speed)
   * FXn (minimum of daily maximum wind speed)
   * FXx (maximum of daily maximum wind speed)
 
@@ -222,7 +226,25 @@
 * calcualte climate indicators for ERA5 data
 * input variable for WI is tasmin not tas
 
 0.7.6 (2023-06-20)
 ------------------
 
 * outsourcing test data to github repository https://github.com/ludwiglierhammer/test_data
+
+0.8.0 (2023-07-13)
+------------------
+* optionally: calculate SCD with water equivalent input
+* replace '.' with '-' in directory structure and output file names
+* new climate indicators:
+
+  * DSn: total number of days in dry spells
+  * WSn: total number of days in wet spells
+  * CSx: maximum length of cold spell
+  * CSn: total number of days in cold spells
+  * HSn: total number of days in hot spells
+  * HWn: total number of days in heat waves
+  * LFD: number of late frost days
+
+* metadata: set mm/day to mm
+* fixing v0.7.3 and v0.7.4 with xclim>=0.44
+* redo v0.7.5 (if dataset frequency is not equal input frequency, convert it; adding hourly test data)
```

### Comparing `index_calculator-0.7.6/LICENSE` & `index_calculator-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `index_calculator-0.7.6/PKG-INFO` & `index_calculator-0.8.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: index_calculator
-Version: 0.7.6
+Version: 0.8.0
 Summary: Python index-calculator is an xclim wrapperto calculate climate indices from CMORized netCDF files.
 Home-page: https://github.com/ludwiglierhammer/index_calculator
 Author: Ludwig Lierhammer
 Author-email: ludwig.lierhammer@hereon.de
 License: MIT license
 Keywords: index_calculator
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -227,14 +227,15 @@
 * restructuring time encoding
 * properties removed
 
 0.5.0 (2023-01-04)
 ------------------
 
 * new indices:
+
   * CSf (Number of cold spells)
   * HSf (Number of hot spells)
   * HSx (Maximum length of hot spells)
   * SD (Number od snow days)
   * SCD (Snow cover duration)
   * Sint (Snowfall intensity)
   * Sfreq (Snowfall freqeuncy)
@@ -276,21 +277,23 @@
 
 * time controlling to pyhomogenize
 
 0.6.0 (2023-03-03)
 ------------------
 
 * new indices:
+
   * HW: maximum length of heat waves
   * GSS: start of growing season
   * GSE: end of growing season
   * FFS: start of frost-free season
   * FFE: end of frost-free season
   * RRm: mean daily precipitation
   * RRYYp: precipitation percentile value
+
 * rename RYYp to RYYpABS and RDYYP to RYYp according to ICCLIM
 * optional argument perc woth percentile indicators
 
 0.6.1 (2023-03-09)
 ------------------
 
 * some metadata corrections
@@ -341,14 +344,15 @@
 
 * calculating percentile indices with non-standard calendar
 
 0.7.2 (2023-05-10)
 ------------------
 
 * new indicators implemented:
+
   * FG (mean daily wind speed)
   * FGn (minimum od mean daily wind speed)
   * FGx (maximum of mean daily wind speed)
   * FX (mean of maximum daily wind speed)
   * FXn (minimum of daily maximum wind speed)
   * FXx (maximum of daily maximum wind speed)
 
@@ -380,7 +384,25 @@
 * calcualte climate indicators for ERA5 data
 * input variable for WI is tasmin not tas
 
 0.7.6 (2023-06-20)
 ------------------
 
 * outsourcing test data to github repository https://github.com/ludwiglierhammer/test_data
+
+0.8.0 (2023-07-13)
+------------------
+* optionally: calculate SCD with water equivalent input
+* replace '.' with '-' in directory structure and output file names
+* new climate indicators:
+
+  * DSn: total number of days in dry spells
+  * WSn: total number of days in wet spells
+  * CSx: maximum length of cold spell
+  * CSn: total number of days in cold spells
+  * HSn: total number of days in hot spells
+  * HWn: total number of days in heat waves
+  * LFD: number of late frost days
+
+* metadata: set mm/day to mm
+* fixing v0.7.3 and v0.7.4 with xclim>=0.44
+* redo v0.7.5 (if dataset frequency is not equal input frequency, convert it; adding hourly test data)
```

### Comparing `index_calculator-0.7.6/README.rst` & `index_calculator-0.8.0/README.rst`

 * *Files identical despite different names*

### Comparing `index_calculator-0.7.6/docs/Makefile` & `index_calculator-0.8.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `index_calculator-0.7.6/docs/api.rst` & `index_calculator-0.8.0/docs/api.rst`

 * *Files identical despite different names*

### Comparing `index_calculator-0.7.6/docs/conf.py` & `index_calculator-0.8.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `index_calculator-0.7.6/docs/installation.rst` & `index_calculator-0.8.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `index_calculator-0.7.6/docs/make.bat` & `index_calculator-0.8.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `index_calculator-0.7.6/index_calculator/__init__.py` & `index_calculator-0.8.0/index_calculator/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 """Top-level package for index_calculator."""
 
 __author__ = """Ludwig Lierhammer"""
 __email__ = "ludwig.lierhammer@hereon.de"
-__version__ = "0.7.6"
+__version__ = "0.8.0"
 
 from ._outputwriter import OutputWriter as outputwriter
 from ._postprocessing import PostProcessing as postprocessing
 from ._preprocessing import PreProcessing as preprocessing
 from ._processing import Processing as processing
-from ._tables import cfjson  # noqa
-from ._tables import cjson  # noqa
 from ._tables import mjson  # noqa
 from ._tables import pjson  # noqa
 from ._tables import vjson  # noqa
 from ._tables import xjson  # noqa
 from .index_calculator import IndexCalculator as index_calculator
 
 preprocessing.__module__ = __name__
```

### Comparing `index_calculator-0.7.6/index_calculator/_ci_netcdfattrs.py` & `index_calculator-0.8.0/index_calculator/_ci_netcdfattrs.py`

 * *Files identical despite different names*

### Comparing `index_calculator-0.7.6/index_calculator/_consts.py` & `index_calculator-0.8.0/index_calculator/_consts.py`

 * *Files identical despite different names*

### Comparing `index_calculator-0.7.6/index_calculator/_indices.py` & `index_calculator-0.8.0/index_calculator/_indices.py`

 * *Files 5% similar despite different names*

```diff
@@ -929,3844 +929,4380 @@
 00003a00: 746d 6f73 2e64 7279 5f73 7065 6c6c 5f6d  tmos.dry_spell_m
 00003a10: 6178 5f6c 656e 6774 6828 0a20 2020 2020  ax_length(.     
 00003a20: 2020 2020 2020 2074 6872 6573 683d 7468         thresh=th
 00003a30: 7265 7368 2c0a 2020 2020 2020 2020 2020  resh,.          
 00003a40: 2020 7769 6e64 6f77 3d77 696e 646f 772c    window=window,
 00003a50: 0a20 2020 2020 2020 2020 2020 202a 2a70  .            **p
 00003a60: 6172 616d 732c 0a20 2020 2020 2020 2029  arams,.        )
-00003a70: 0a0a 0a63 6c61 7373 2057 5366 3a0a 2020  ...class WSf:.  
-00003a80: 2020 2222 224e 756d 6265 7220 6f66 2077    """Number of w
-00003a90: 6574 2073 7065 6c6c 7320 2870 7229 2e22  et spells (pr)."
-00003aa0: 2222 0a0a 2020 2020 7468 7265 7368 203d  ""..    thresh =
-00003ab0: 2031 0a20 2020 2077 696e 646f 7720 3d20   1.    window = 
-00003ac0: 350a 0a20 2020 2064 6566 2063 6f6d 7075  5..    def compu
-00003ad0: 7465 2874 6872 6573 683d 7468 7265 7368  te(thresh=thresh
-00003ae0: 2c20 7769 6e64 6f77 3d77 696e 646f 772c  , window=window,
-00003af0: 202a 2a70 6172 616d 7329 3a0a 2020 2020   **params):.    
-00003b00: 2020 2020 2222 2243 616c 6375 6c61 7465      """Calculate
-00003b10: 206e 756d 6265 7220 6f66 2077 6574 2073   number of wet s
-00003b20: 7065 6c6c 732e 0a0a 2020 2020 2020 2020  pells...        
-00003b30: 5061 7261 6d65 7465 7273 0a20 2020 2020  Parameters.     
-00003b40: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020     ----------.  
-00003b50: 2020 2020 2020 7468 7265 7368 3a20 696e        thresh: in
-00003b60: 7420 6f72 2073 7472 696e 670a 2020 2020  t or string.    
-00003b70: 2020 2020 2020 2020 5468 7265 7368 6f6c          Threshol
-00003b80: 6420 7072 6563 6970 6974 6174 696f 6e20  d precipitation 
-00003b90: 6162 6f76 6520 7768 6963 6820 6120 6461  above which a da
-00003ba0: 7920 6973 2063 6f6e 7369 6465 7265 640a  y is considered.
-00003bb0: 2020 2020 2020 2020 2020 2020 6173 2061              as a
-00003bc0: 2077 6574 2064 6179 2028 6465 6661 756c   wet day (defaul
-00003bd0: 743a 2031 206d 6d29 2e0a 2020 2020 2020  t: 1 mm)..      
-00003be0: 2020 2020 2020 4966 2074 7970 6520 6f66        If type of
-00003bf0: 2074 6872 6573 686f 6c64 2069 7320 616e   threshold is an
-00003c00: 2069 6e74 6567 6572 2074 6865 2075 6e69   integer the uni
-00003c10: 7420 6973 2073 6574 2074 6f20 6d6d 2e0a  t is set to mm..
-00003c20: 2020 2020 2020 2020 7769 6e64 6f77 3a20          window: 
-00003c30: 696e 740a 2020 2020 2020 2020 2020 2020  int.            
-00003c40: 4d69 6e69 6d75 6d20 6e75 6d62 6572 206f  Minimum number o
-00003c50: 6620 6461 7973 2077 6974 6820 7072 6563  f days with prec
-00003c60: 6970 6974 6174 696f 6e20 6162 6f76 6520  ipitation above 
-00003c70: 7468 7265 7368 6f6c 640a 2020 2020 2020  threshold.      
-00003c80: 2020 2020 2020 746f 2071 7561 6c69 6679        to qualify
-00003c90: 2061 7320 6120 7765 7420 7370 656c 6c20   as a wet spell 
-00003ca0: 2864 6566 6175 6c74 3a20 3529 2e0a 0a20  (default: 5)... 
-00003cb0: 2020 2020 2020 2052 6574 7572 6e73 0a20         Returns. 
-00003cc0: 2020 2020 2020 202d 2d2d 2d2d 2d2d 0a20         -------. 
-00003cd0: 2020 2020 2020 2078 6172 7261 792e 4461         xarray.Da
-00003ce0: 7461 4172 7261 790a 2020 2020 2020 2020  taArray.        
-00003cf0: 2020 2020 4e75 6d62 6572 206f 6620 7765      Number of we
-00003d00: 7420 7065 7269 6f64 7320 6f66 206d 696e  t periods of min
-00003d10: 696d 756d 207b 7769 6e64 6f77 7d20 6461  imum {window} da
-00003d20: 7973 2028 7072 203e 3d20 7b74 6872 6573  ys (pr >= {thres
-00003d30: 687d 292e 0a0a 2020 2020 2020 2020 4e6f  h})...        No
-00003d40: 7465 730a 2020 2020 2020 2020 2d2d 2d2d  tes.        ----
-00003d50: 2d0a 2020 2020 2020 2020 466f 7220 6d6f  -.        For mo
-00003d60: 7265 2069 6e66 6f72 6d61 7469 6f6e 206f  re information o
-00003d70: 6e20 7468 6520 696e 7075 7420 7061 7261  n the input para
-00003d80: 6d65 7465 7273 2073 6565 3a0a 2020 2020  meters see:.    
-00003d90: 2020 2020 2020 2020 6874 7470 733a 2f2f          https://
-00003da0: 7863 6c69 6d2e 7265 6164 7468 6564 6f63  xclim.readthedoc
-00003db0: 732e 696f 2f65 6e2f 7374 6162 6c65 2f61  s.io/en/stable/a
-00003dc0: 7069 2e68 746d 6c23 7863 6c69 6d2e 696e  pi.html#xclim.in
-00003dd0: 6469 6361 746f 7273 2e61 746d 6f73 2e77  dicators.atmos.w
-00003de0: 6574 5f73 7065 6c6c 5f66 7265 7175 656e  et_spell_frequen
-00003df0: 6379 0a20 2020 2020 2020 2022 2222 0a20  cy.        """. 
-00003e00: 2020 2020 2020 2074 6872 6573 6820 3d20         thresh = 
-00003e10: 5f74 6872 6573 685f 7374 7269 6e67 2874  _thresh_string(t
-00003e20: 6872 6573 682c 2022 6d6d 2229 0a20 2020  hresh, "mm").   
-00003e30: 2020 2020 2072 6574 7572 6e20 7863 2e61       return xc.a
-00003e40: 746d 6f73 2e77 6574 5f73 7065 6c6c 5f66  tmos.wet_spell_f
-00003e50: 7265 7175 656e 6379 280a 2020 2020 2020  requency(.      
-00003e60: 2020 2020 2020 7468 7265 7368 3d74 6872        thresh=thr
-00003e70: 6573 682c 0a20 2020 2020 2020 2020 2020  esh,.           
-00003e80: 2077 696e 646f 773d 7769 6e64 6f77 2c0a   window=window,.
-00003e90: 2020 2020 2020 2020 2020 2020 2a2a 7061              **pa
-00003ea0: 7261 6d73 2c0a 2020 2020 2020 2020 290a  rams,.        ).
-00003eb0: 0a0a 636c 6173 7320 5753 783a 0a20 2020  ..class WSx:.   
-00003ec0: 2022 2222 4d61 7869 6d75 6d20 6c65 6e67   """Maximum leng
-00003ed0: 7468 206f 6620 7765 7420 7370 656c 6c73  th of wet spells
-00003ee0: 2028 7072 292e 2222 220a 0a20 2020 2074   (pr)."""..    t
-00003ef0: 6872 6573 6820 3d20 310a 2020 2020 7769  hresh = 1.    wi
-00003f00: 6e64 6f77 203d 2031 0a0a 2020 2020 6465  ndow = 1..    de
-00003f10: 6620 636f 6d70 7574 6528 7468 7265 7368  f compute(thresh
-00003f20: 3d74 6872 6573 682c 2077 696e 646f 773d  =thresh, window=
-00003f30: 7769 6e64 6f77 2c20 2a2a 7061 7261 6d73  window, **params
-00003f40: 293a 0a20 2020 2020 2020 2022 2222 4361  ):.        """Ca
-00003f50: 6c63 756c 6174 6520 6d61 7869 6d75 6d20  lculate maximum 
-00003f60: 6c65 6e67 7468 206f 6620 7765 7420 7370  length of wet sp
-00003f70: 656c 6c73 2e0a 0a20 2020 2020 2020 2050  ells...        P
-00003f80: 6172 616d 6574 6572 730a 2020 2020 2020  arameters.      
-00003f90: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020    ----------.   
-00003fa0: 2020 2020 2074 6872 6573 683a 2069 6e74       thresh: int
-00003fb0: 206f 7220 7374 7269 6e67 0a20 2020 2020   or string.     
-00003fc0: 2020 2020 2020 2054 6872 6573 686f 6c64         Threshold
-00003fd0: 2070 7265 6369 7069 7461 7469 6f6e 2061   precipitation a
-00003fe0: 626f 7665 2077 6869 6368 2061 2064 6179  bove which a day
-00003ff0: 2069 7320 636f 6e73 6964 6572 6564 0a20   is considered. 
-00004000: 2020 2020 2020 2020 2020 2061 7320 6120             as a 
-00004010: 7765 7420 6461 7920 2864 6566 6175 6c74  wet day (default
-00004020: 3a20 3120 6d6d 292e 0a20 2020 2020 2020  : 1 mm)..       
-00004030: 2020 2020 2049 6620 7479 7065 206f 6620       If type of 
-00004040: 7468 7265 7368 6f6c 6420 6973 2061 6e20  threshold is an 
-00004050: 696e 7465 6765 7220 7468 6520 756e 6974  integer the unit
-00004060: 2069 7320 7365 7420 746f 206d 6d2e 0a20   is set to mm.. 
-00004070: 2020 2020 2020 2077 696e 646f 773a 2069         window: i
-00004080: 6e74 0a20 2020 2020 2020 2020 2020 204d  nt.            M
-00004090: 696e 696d 756d 206e 756d 6265 7220 6f66  inimum number of
-000040a0: 2064 6179 7320 7769 7468 2070 7265 6369   days with preci
-000040b0: 7069 7461 7469 6f6e 2061 626f 7665 2074  pitation above t
-000040c0: 6872 6573 686f 6c64 0a20 2020 2020 2020  hreshold.       
-000040d0: 2020 2020 2074 6f20 7175 616c 6966 7920       to qualify 
-000040e0: 6173 2061 2077 6574 2073 7065 6c6c 2028  as a wet spell (
-000040f0: 6465 6661 756c 743a 2031 292e 0a0a 2020  default: 1)...  
-00004100: 2020 2020 2020 5265 7475 726e 730a 2020        Returns.  
-00004110: 2020 2020 2020 2d2d 2d2d 2d2d 2d0a 2020        -------.  
-00004120: 2020 2020 2020 7861 7272 6179 2e44 6174        xarray.Dat
-00004130: 6141 7272 6179 0a20 2020 2020 2020 2020  aArray.         
-00004140: 2020 204d 6178 696d 756d 206c 656e 6774     Maximum lengt
-00004150: 6820 6f66 2077 6574 2073 7065 6c6c 7320  h of wet spells 
-00004160: 6f66 2061 7420 6c65 6173 7420 7b77 696e  of at least {win
-00004170: 646f 777d 2063 6f6e 7365 6375 7469 7665  dow} consecutive
-00004180: 2064 6179 730a 2020 2020 2020 2020 2020   days.          
-00004190: 2020 7769 7468 2070 7265 6369 7069 7461    with precipita
-000041a0: 7469 6f6e 2061 626f 7665 207b 7468 7265  tion above {thre
-000041b0: 7368 7d2e 0a0a 2020 2020 2020 2020 4e6f  sh}...        No
-000041c0: 7465 730a 2020 2020 2020 2020 2d2d 2d2d  tes.        ----
-000041d0: 2d0a 2020 2020 2020 2020 466f 7220 6d6f  -.        For mo
-000041e0: 7265 2069 6e66 6f72 6d61 7469 6f6e 206f  re information o
-000041f0: 6e20 7468 6520 696e 7075 7420 7061 7261  n the input para
-00004200: 6d65 7465 7273 2073 6565 3a0a 2020 2020  meters see:.    
-00004210: 2020 2020 2020 2020 6874 7470 733a 2f2f          https://
-00004220: 7863 6c69 6d2e 7265 6164 7468 6564 6f63  xclim.readthedoc
-00004230: 732e 696f 2f65 6e2f 7374 6162 6c65 2f61  s.io/en/stable/a
-00004240: 7069 2e68 746d 6c23 7863 6c69 6d2e 696e  pi.html#xclim.in
-00004250: 6469 6361 746f 7273 2e61 746d 6f73 2e77  dicators.atmos.w
-00004260: 6574 5f73 7065 6c6c 5f6d 6178 5f6c 656e  et_spell_max_len
-00004270: 6774 680a 2020 2020 2020 2020 2222 220a  gth.        """.
-00004280: 2020 2020 2020 2020 7468 7265 7368 203d          thresh =
-00004290: 205f 7468 7265 7368 5f73 7472 696e 6728   _thresh_string(
-000042a0: 7468 7265 7368 2c20 226d 6d22 290a 2020  thresh, "mm").  
-000042b0: 2020 2020 2020 7265 7475 726e 2078 632e        return xc.
-000042c0: 6174 6d6f 732e 7765 745f 7370 656c 6c5f  atmos.wet_spell_
-000042d0: 6d61 785f 6c65 6e67 7468 280a 2020 2020  max_length(.    
-000042e0: 2020 2020 2020 2020 7468 7265 7368 3d74          thresh=t
-000042f0: 6872 6573 682c 0a20 2020 2020 2020 2020  hresh,.         
-00004300: 2020 2077 696e 646f 773d 7769 6e64 6f77     window=window
-00004310: 2c0a 2020 2020 2020 2020 2020 2020 2a2a  ,.            **
-00004320: 7061 7261 6d73 2c0a 2020 2020 2020 2020  params,.        
-00004330: 290a 0a0a 636c 6173 7320 4454 523a 0a20  )...class DTR:. 
-00004340: 2020 2022 2222 4d65 616e 2074 656d 7065     """Mean tempe
-00004350: 7261 7475 7265 2072 6e61 6765 2028 7461  rature rnage (ta
-00004360: 736d 6178 2c20 7461 736d 696e 292e 2222  smax, tasmin).""
-00004370: 220a 0a20 2020 2064 6566 2063 6f6d 7075  "..    def compu
-00004380: 7465 282a 2a70 6172 616d 7329 3a0a 2020  te(**params):.  
-00004390: 2020 2020 2020 2222 2243 616c 6375 6c61        """Calcula
-000043a0: 7465 206d 6561 6e20 6f66 2064 6169 6c79  te mean of daily
-000043b0: 2074 656d 7065 7261 7475 7265 2072 616e   temperature ran
-000043c0: 6765 2e0a 0a20 2020 2020 2020 2052 6574  ge...        Ret
-000043d0: 7572 6e73 0a20 2020 2020 2020 202d 2d2d  urns.        ---
-000043e0: 2d2d 2d2d 0a20 2020 2020 2020 2078 6172  ----.        xar
-000043f0: 7261 792e 4461 7461 4172 7261 790a 2020  ray.DataArray.  
-00004400: 2020 2020 2020 2020 2020 4d65 616e 206f            Mean o
-00004410: 6620 6461 696c 7920 7465 6d70 6572 6174  f daily temperat
-00004420: 7572 6520 7261 6e67 652e 0a0a 2020 2020  ure range...    
-00004430: 2020 2020 4e6f 7465 730a 2020 2020 2020      Notes.      
-00004440: 2020 2d2d 2d2d 2d0a 2020 2020 2020 2020    -----.        
-00004450: 466f 7220 696e 666f 726d 6174 696f 6e20  For information 
-00004460: 6f6e 2074 6865 2069 6e70 7574 2070 6172  on the input par
-00004470: 616d 6574 6572 7320 7365 653a 0a20 2020  ameters see:.   
-00004480: 2020 2020 2020 2020 2068 7474 7073 3a2f           https:/
-00004490: 2f78 636c 696d 2e72 6561 6474 6865 646f  /xclim.readthedo
-000044a0: 6373 2e69 6f2f 656e 2f73 7461 626c 652f  cs.io/en/stable/
-000044b0: 6170 692e 6874 6d6c 2378 636c 696d 2e69  api.html#xclim.i
-000044c0: 6e64 6963 6174 6f72 732e 6174 6d6f 732e  ndicators.atmos.
-000044d0: 6461 696c 795f 7465 6d70 6572 6174 7572  daily_temperatur
-000044e0: 655f 7261 6e67 650a 2020 2020 2020 2020  e_range.        
-000044f0: 2222 220a 2020 2020 2020 2020 7265 7475  """.        retu
-00004500: 726e 2078 632e 6174 6d6f 732e 6461 696c  rn xc.atmos.dail
-00004510: 795f 7465 6d70 6572 6174 7572 655f 7261  y_temperature_ra
-00004520: 6e67 6528 2a2a 7061 7261 6d73 290a 0a0a  nge(**params)...
-00004530: 636c 6173 7320 4644 3a0a 2020 2020 2222  class FD:.    ""
-00004540: 224e 756d 6265 7220 6f66 2066 726f 7374  "Number of frost
-00004550: 2064 6179 7320 2874 6173 6d69 6e29 2e22   days (tasmin)."
-00004560: 2222 0a0a 2020 2020 6465 6620 636f 6d70  ""..    def comp
-00004570: 7574 6528 2a2a 7061 7261 6d73 293a 0a20  ute(**params):. 
-00004580: 2020 2020 2020 2022 2222 4361 6c63 756c         """Calcul
-00004590: 6174 6520 6e75 6d62 6572 206f 6620 6672  ate number of fr
-000045a0: 6f73 7420 6461 7973 2028 7461 736d 696e  ost days (tasmin
-000045b0: 203c 2030 2e30 2064 6567 4329 2e0a 0a20   < 0.0 degC)... 
-000045c0: 2020 2020 2020 2052 6574 7572 6e73 0a20         Returns. 
-000045d0: 2020 2020 2020 202d 2d2d 2d2d 2d2d 0a20         -------. 
-000045e0: 2020 2020 2020 2078 6172 7261 792e 4461         xarray.Da
-000045f0: 7461 4172 7261 790a 2020 2020 2020 2020  taArray.        
-00004600: 2020 2020 4e75 6d62 6572 206f 6620 6672      Number of fr
-00004610: 6f73 7420 6461 7973 2028 7461 736d 696e  ost days (tasmin
-00004620: 203c 2030 2e30 2064 6567 4329 2e0a 0a20   < 0.0 degC)... 
-00004630: 2020 2020 2020 204e 6f74 6573 0a20 2020         Notes.   
-00004640: 2020 2020 202d 2d2d 2d2d 0a20 2020 2020       -----.     
-00004650: 2020 2046 6f72 2069 6e66 6f72 6d61 7469     For informati
-00004660: 6f6e 206f 6e20 7468 6520 696e 7075 7420  on on the input 
-00004670: 7061 7261 6d65 7465 7273 2073 6565 3a0a  parameters see:.
-00004680: 2020 2020 2020 2020 2020 2020 6874 7470              http
-00004690: 733a 2f2f 7863 6c69 6d2e 7265 6164 7468  s://xclim.readth
-000046a0: 6564 6f63 732e 696f 2f65 6e2f 7374 6162  edocs.io/en/stab
-000046b0: 6c65 2f61 7069 2e68 746d 6c23 7863 6c69  le/api.html#xcli
-000046c0: 6d2e 696e 6469 6361 746f 7273 2e61 746d  m.indicators.atm
-000046d0: 6f73 2e66 726f 7374 5f64 6179 730a 2020  os.frost_days.  
-000046e0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-000046f0: 2020 7265 7475 726e 2078 632e 6174 6d6f    return xc.atmo
-00004700: 732e 6672 6f73 745f 6461 7973 282a 2a70  s.frost_days(**p
-00004710: 6172 616d 7329 0a0a 0a63 6c61 7373 2049  arams)...class I
-00004720: 443a 0a20 2020 2022 2222 4e75 6d62 6572  D:.    """Number
-00004730: 206f 6620 6963 6520 6461 7973 2028 7461   of ice days (ta
-00004740: 736d 6178 292e 2222 220a 0a20 2020 2064  smax)."""..    d
-00004750: 6566 2063 6f6d 7075 7465 282a 2a70 6172  ef compute(**par
-00004760: 616d 7329 3a0a 2020 2020 2020 2020 2222  ams):.        ""
-00004770: 2243 616c 6375 6c61 7465 206e 756d 6265  "Calculate numbe
-00004780: 7220 6f66 2069 6365 2064 6179 7320 2874  r of ice days (t
-00004790: 6173 6d61 7820 3c20 302e 3020 6465 6743  asmax < 0.0 degC
-000047a0: 292e 0a0a 2020 2020 2020 2020 5061 7261  )...        Para
-000047b0: 6d65 7465 7273 0a20 2020 2020 2020 202d  meters.        -
-000047c0: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 2020  ---------.      
-000047d0: 2020 466f 7220 696e 666f 726d 6174 696f    For informatio
-000047e0: 6e20 6f6e 2074 6865 2069 6e70 7574 2070  n on the input p
-000047f0: 6172 616d 6574 6572 7320 7365 653a 0a20  arameters see:. 
-00004800: 2020 2020 2020 2020 2020 2068 7474 7073             https
-00004810: 3a2f 2f78 636c 696d 2e72 6561 6474 6865  ://xclim.readthe
-00004820: 646f 6373 2e69 6f2f 656e 2f73 7461 626c  docs.io/en/stabl
-00004830: 652f 6170 692e 6874 6d6c 2378 636c 696d  e/api.html#xclim
-00004840: 2e69 6e64 6963 6174 6f72 732e 6174 6d6f  .indicators.atmo
-00004850: 732e 6963 655f 6461 7973 0a0a 2020 2020  s.ice_days..    
-00004860: 2020 2020 5265 7475 726e 730a 2020 2020      Returns.    
-00004870: 2020 2020 2d2d 2d2d 2d2d 2d0a 2020 2020      -------.    
-00004880: 2020 2020 7861 7272 6179 2e44 6174 6141      xarray.DataA
-00004890: 7272 6179 0a20 2020 2020 2020 2020 2020  rray.           
-000048a0: 204e 756d 6265 7220 6f66 2069 6365 2064   Number of ice d
-000048b0: 6179 7320 2874 6173 6d61 7820 3c20 302e  ays (tasmax < 0.
-000048c0: 3020 6465 6743 292e 0a20 2020 2020 2020  0 degC)..       
-000048d0: 2022 2222 0a20 2020 2020 2020 2072 6574   """.        ret
-000048e0: 7572 6e20 7863 2e61 746d 6f73 2e69 6365  urn xc.atmos.ice
-000048f0: 5f64 6179 7328 2a2a 7061 7261 6d73 290a  _days(**params).
-00004900: 0a0a 636c 6173 7320 4744 3a0a 2020 2020  ..class GD:.    
-00004910: 2222 2243 756d 756c 6174 6976 6520 6772  """Cumulative gr
-00004920: 6f77 696e 6720 6465 6772 6565 2064 6179  owing degree day
-00004930: 7320 2874 6173 292e 2222 220a 0a20 2020  s (tas)."""..   
-00004940: 2074 6872 6573 6820 3d20 340a 0a20 2020   thresh = 4..   
-00004950: 2064 6566 2063 6f6d 7075 7465 2874 6872   def compute(thr
-00004960: 6573 683d 7468 7265 7368 2c20 2a2a 7061  esh=thresh, **pa
-00004970: 7261 6d73 293a 0a20 2020 2020 2020 2022  rams):.        "
-00004980: 2222 4361 6c63 756c 6174 6520 6375 6d75  ""Calculate cumu
-00004990: 6c61 7469 7665 2067 726f 7769 6e67 2064  lative growing d
-000049a0: 6567 7265 6520 6461 7973 2028 7461 7320  egree days (tas 
-000049b0: 3e20 7468 7265 7368 292e 0a0a 2020 2020  > thresh)...    
-000049c0: 2020 2020 5061 7261 6d65 7465 7273 0a20      Parameters. 
-000049d0: 2020 2020 2020 202d 2d2d 2d2d 2d2d 2d2d         ---------
-000049e0: 2d0a 2020 2020 2020 2020 7468 7265 7368  -.        thresh
-000049f0: 3a20 696e 7420 6f72 2073 7472 696e 670a  : int or string.
-00004a00: 2020 2020 2020 2020 2020 2020 5468 7265              Thre
-00004a10: 7368 6f6c 6420 7465 6d70 6572 6174 7572  shold temperatur
-00004a20: 6520 6162 6f76 6520 7768 6963 6820 7468  e above which th
-00004a30: 6520 6461 696c 7920 7465 6d70 6572 6174  e daily temperat
-00004a40: 7572 6520 7769 6c6c 0a20 2020 2020 2020  ure will.       
-00004a50: 2020 2020 2062 6520 6164 6465 6420 746f       be added to
-00004a60: 2074 6865 2063 756d 756c 6174 6976 6520   the cumulative 
-00004a70: 7375 6d20 6f66 2074 656d 7065 7261 7475  sum of temperatu
-00004a80: 7265 2064 6567 7265 6573 2e0a 0a20 2020  re degrees...   
-00004a90: 2020 2020 2052 6574 7572 6e73 0a20 2020       Returns.   
-00004aa0: 2020 2020 202d 2d2d 2d2d 2d2d 0a20 2020       -------.   
-00004ab0: 2020 2020 2078 6172 7261 792e 4461 7461       xarray.Data
-00004ac0: 4172 7261 790a 2020 2020 2020 2020 2020  Array.          
-00004ad0: 2020 4375 6d75 6c61 7469 7665 2067 726f    Cumulative gro
-00004ae0: 7769 6e67 2064 6567 7265 6520 6461 7973  wing degree days
-00004af0: 2028 7461 7320 3e20 7b74 6872 6573 687d   (tas > {thresh}
-00004b00: 292e 0a0a 2020 2020 2020 2020 4e6f 7465  )...        Note
-00004b10: 730a 2020 2020 2020 2020 2d2d 2d2d 2d0a  s.        -----.
-00004b20: 2020 2020 2020 2020 466f 7220 6d6f 7265          For more
-00004b30: 2069 6e66 6f72 6d61 7469 6f6e 206f 6e20   information on 
-00004b40: 7468 6520 696e 7075 7420 7061 7261 6d65  the input parame
-00004b50: 7465 7273 2073 6565 3a0a 2020 2020 2020  ters see:.      
-00004b60: 2020 2020 2020 6874 7470 733a 2f2f 7863        https://xc
-00004b70: 6c69 6d2e 7265 6164 7468 6564 6f63 732e  lim.readthedocs.
-00004b80: 696f 2f65 6e2f 7374 6162 6c65 2f61 7069  io/en/stable/api
-00004b90: 2e68 746d 6c23 7863 6c69 6d2e 696e 6469  .html#xclim.indi
-00004ba0: 6361 746f 7273 2e61 746d 6f73 2e67 726f  cators.atmos.gro
-00004bb0: 7769 6e67 5f64 6567 7265 655f 6461 7973  wing_degree_days
-00004bc0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00004bd0: 2020 2020 2074 6872 6573 6820 3d20 5f74       thresh = _t
-00004be0: 6872 6573 685f 7374 7269 6e67 2874 6872  hresh_string(thr
-00004bf0: 6573 682c 2022 6465 6743 2229 0a20 2020  esh, "degC").   
-00004c00: 2020 2020 2072 6574 7572 6e20 7863 2e61       return xc.a
-00004c10: 746d 6f73 2e67 726f 7769 6e67 5f64 6567  tmos.growing_deg
-00004c20: 7265 655f 6461 7973 280a 2020 2020 2020  ree_days(.      
-00004c30: 2020 2020 2020 7468 7265 7368 3d74 6872        thresh=thr
-00004c40: 6573 682c 0a20 2020 2020 2020 2020 2020  esh,.           
-00004c50: 202a 2a70 6172 616d 732c 0a20 2020 2020   **params,.     
-00004c60: 2020 2029 0a0a 0a63 6c61 7373 2048 4431     )...class HD1
-00004c70: 373a 0a20 2020 2022 2222 4375 6d75 6c61  7:.    """Cumula
-00004c80: 7469 7665 2068 6561 7469 6e67 2064 6567  tive heating deg
-00004c90: 7265 6520 6461 7973 2028 7461 7329 2e22  ree days (tas)."
-00004ca0: 2222 0a0a 2020 2020 6465 6620 636f 6d70  ""..    def comp
-00004cb0: 7574 6528 2a2a 7061 7261 6d73 293a 0a20  ute(**params):. 
-00004cc0: 2020 2020 2020 2022 2222 4361 6c63 756c         """Calcul
-00004cd0: 6174 6520 6375 6d75 6c61 7469 7665 2068  ate cumulative h
-00004ce0: 6561 7469 6e67 2064 6567 7265 6520 6461  eating degree da
-00004cf0: 7973 2028 7461 7320 3c20 3137 2064 6567  ys (tas < 17 deg
-00004d00: 4329 2e0a 0a20 2020 2020 2020 2052 6574  C)...        Ret
-00004d10: 7572 6e73 0a20 2020 2020 2020 202d 2d2d  urns.        ---
-00004d20: 2d2d 2d2d 0a20 2020 2020 2020 2078 6172  ----.        xar
-00004d30: 7261 792e 4461 7461 4172 7261 790a 2020  ray.DataArray.  
-00004d40: 2020 2020 2020 2020 2020 4375 6d75 6c61            Cumula
-00004d50: 7469 7665 2068 6561 7469 6e67 2064 6567  tive heating deg
-00004d60: 7265 6520 6461 7973 2028 7461 7320 3e20  ree days (tas > 
-00004d70: 3137 2064 6567 4329 2e0a 0a20 2020 2020  17 degC)...     
-00004d80: 2020 204e 6f74 6573 0a20 2020 2020 2020     Notes.       
-00004d90: 202d 2d2d 2d2d 0a20 2020 2020 2020 2046   -----.        F
-00004da0: 6f72 2069 6e66 6f72 6d61 7469 6f6e 206f  or information o
-00004db0: 6e20 7468 6520 696e 7075 7420 7061 7261  n the input para
-00004dc0: 6d65 7465 7273 2073 6565 3a0a 2020 2020  meters see:.    
-00004dd0: 2020 2020 2020 2020 6874 7470 733a 2f2f          https://
-00004de0: 7863 6c69 6d2e 7265 6164 7468 6564 6f63  xclim.readthedoc
-00004df0: 732e 696f 2f65 6e2f 7374 6162 6c65 2f61  s.io/en/stable/a
-00004e00: 7069 2e68 746d 6c23 7863 6c69 6d2e 696e  pi.html#xclim.in
-00004e10: 6469 6361 746f 7273 2e61 746d 6f73 2e68  dicators.atmos.h
-00004e20: 6561 7469 6e67 5f64 6567 7265 655f 6461  eating_degree_da
-00004e30: 7973 0a20 2020 2020 2020 2022 2222 0a20  ys.        """. 
-00004e40: 2020 2020 2020 2072 6574 7572 6e20 7863         return xc
-00004e50: 2e61 746d 6f73 2e68 6561 7469 6e67 5f64  .atmos.heating_d
-00004e60: 6567 7265 655f 6461 7973 280a 2020 2020  egree_days(.    
-00004e70: 2020 2020 2020 2020 2a2a 7061 7261 6d73          **params
-00004e80: 2c0a 2020 2020 2020 2020 290a 0a0a 636c  ,.        )...cl
-00004e90: 6173 7320 5052 4350 544f 543a 0a20 2020  ass PRCPTOT:.   
-00004ea0: 2022 2222 546f 7461 6c20 7072 6563 6970   """Total precip
-00004eb0: 6974 6174 696f 6e20 616d 6f75 6e74 2028  itation amount (
-00004ec0: 7072 292e 2222 220a 0a20 2020 2074 6872  pr)."""..    thr
-00004ed0: 6573 6820 3d20 310a 0a20 2020 2064 6566  esh = 1..    def
-00004ee0: 2063 6f6d 7075 7465 2874 6872 6573 683d   compute(thresh=
-00004ef0: 7468 7265 7368 2c20 2a2a 7061 7261 6d73  thresh, **params
-00004f00: 293a 0a20 2020 2020 2020 2022 2222 4361  ):.        """Ca
-00004f10: 6c63 756c 6174 6520 746f 7461 6c20 7072  lculate total pr
-00004f20: 6563 6970 6974 6174 696f 6e20 616d 6f75  ecipitation amou
-00004f30: 6e74 2e0a 0a20 2020 2020 2020 2050 6172  nt...        Par
-00004f40: 616d 6574 6572 730a 2020 2020 2020 2020  ameters.        
-00004f50: 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020  ----------.     
-00004f60: 2020 2074 6872 6573 683a 2069 6e74 206f     thresh: int o
-00004f70: 7220 7374 7269 6e67 0a20 2020 2020 2020  r string.       
-00004f80: 2020 2020 2054 6872 6573 686f 6c64 2070       Threshold p
-00004f90: 7265 6369 7069 7461 7469 6f6e 2061 626f  recipitation abo
-00004fa0: 7665 2077 6869 6368 2061 2064 6179 2069  ve which a day i
-00004fb0: 7320 636f 6e73 6964 6572 6564 0a20 2020  s considered.   
-00004fc0: 2020 2020 2020 2020 2061 7320 6120 7765           as a we
-00004fd0: 7420 6461 7920 2864 6566 6175 6c74 3a20  t day (default: 
-00004fe0: 3120 6d6d 2f64 6179 292e 0a20 2020 2020  1 mm/day)..     
-00004ff0: 2020 2020 2020 2049 6620 7479 7065 206f         If type o
-00005000: 6620 7468 7265 7368 6f6c 6420 6973 2061  f threshold is a
-00005010: 6e20 696e 7465 6765 7220 7468 6520 756e  n integer the un
-00005020: 6974 2069 7320 7365 7420 746f 206d 6d2f  it is set to mm/
-00005030: 6461 792e 0a0a 2020 2020 2020 2020 5265  day...        Re
-00005040: 7475 726e 730a 2020 2020 2020 2020 2d2d  turns.        --
-00005050: 2d2d 2d2d 2d0a 2020 2020 2020 2020 7861  -----.        xa
-00005060: 7272 6179 2e44 6174 6141 7272 6179 0a20  rray.DataArray. 
-00005070: 2020 2020 2020 2020 2020 2054 6f74 616c             Total
-00005080: 2070 7265 6369 7069 7461 7469 6f6e 2061   precipitation a
-00005090: 6d6f 756e 7420 6f66 2077 6574 2064 6179  mount of wet day
-000050a0: 7320 2870 7265 6369 7020 3e20 7b74 6872  s (precip > {thr
-000050b0: 6573 687d 290a 0a20 2020 2020 2020 204e  esh})..        N
-000050c0: 6f74 6573 0a20 2020 2020 2020 202d 2d2d  otes.        ---
-000050d0: 2d2d 0a20 2020 2020 2020 2046 6f72 206d  --.        For m
-000050e0: 6f72 6520 696e 666f 726d 6174 696f 6e20  ore information 
-000050f0: 6f6e 2074 6865 2069 6e70 7574 2070 6172  on the input par
-00005100: 616d 6574 6572 7320 7365 653a 0a20 2020  ameters see:.   
-00005110: 2020 2020 2020 2020 2068 7474 7073 3a2f           https:/
-00005120: 2f78 636c 696d 2e72 6561 6474 6865 646f  /xclim.readthedo
-00005130: 6373 2e69 6f2f 656e 2f73 7461 626c 652f  cs.io/en/stable/
-00005140: 6170 692e 6874 6d6c 2378 636c 696d 2e69  api.html#xclim.i
-00005150: 6e64 6963 6174 6f72 732e 6174 6d6f 732e  ndicators.atmos.
-00005160: 7765 745f 7072 6563 6970 5f61 6363 756d  wet_precip_accum
-00005170: 756c 6174 696f 6e0a 2020 2020 2020 2020  ulation.        
-00005180: 2222 220a 2020 2020 2020 2020 7468 7265  """.        thre
-00005190: 7368 203d 205f 7468 7265 7368 5f73 7472  sh = _thresh_str
-000051a0: 696e 6728 7468 7265 7368 2c20 226d 6d2f  ing(thresh, "mm/
-000051b0: 6461 7922 290a 2020 2020 2020 2020 7265  day").        re
-000051c0: 7475 726e 2078 632e 6174 6d6f 732e 7765  turn xc.atmos.we
-000051d0: 745f 7072 6563 6970 5f61 6363 756d 756c  t_precip_accumul
-000051e0: 6174 696f 6e28 0a20 2020 2020 2020 2020  ation(.         
-000051f0: 2020 2074 6872 6573 683d 7468 7265 7368     thresh=thresh
-00005200: 2c0a 2020 2020 2020 2020 2020 2020 2a2a  ,.            **
-00005210: 7061 7261 6d73 2c0a 2020 2020 2020 2020  params,.        
-00005220: 290a 0a0a 636c 6173 7320 5252 3a0a 2020  )...class RR:.  
-00005230: 2020 2222 2254 6f74 616c 2070 7265 6369    """Total preci
-00005240: 7069 7461 7469 6f6e 2028 7072 292e 2222  pitation (pr).""
-00005250: 220a 0a20 2020 2064 6566 2063 6f6d 7075  "..    def compu
-00005260: 7465 282a 2a70 6172 616d 7329 3a0a 2020  te(**params):.  
-00005270: 2020 2020 2020 2222 2243 616c 6375 6c61        """Calcula
-00005280: 7465 2074 6f74 616c 2070 7265 6369 7069  te total precipi
-00005290: 7461 7469 6f6e 2e0a 0a20 2020 2020 2020  tation...       
-000052a0: 2052 6574 7572 6e73 0a20 2020 2020 2020   Returns.       
-000052b0: 202d 2d2d 2d2d 2d2d 0a20 2020 2020 2020   -------.       
-000052c0: 2078 6172 7261 792e 4461 7461 4172 7261   xarray.DataArra
-000052d0: 790a 2020 2020 2020 2020 2020 2020 546f  y.            To
-000052e0: 7461 6c20 7072 6563 6970 6974 6174 696f  tal precipitatio
-000052f0: 6e2e 0a0a 2020 2020 2020 2020 4e6f 7465  n...        Note
-00005300: 730a 2020 2020 2020 2020 2d2d 2d2d 2d0a  s.        -----.
-00005310: 2020 2020 2020 2020 466f 7220 696e 666f          For info
-00005320: 726d 6174 696f 6e20 6f6e 2074 6865 2069  rmation on the i
-00005330: 6e70 7574 2070 6172 616d 6574 6572 7320  nput parameters 
-00005340: 7365 653a 0a20 2020 2020 2020 2020 2020  see:.           
-00005350: 2068 7474 7073 3a2f 2f78 636c 696d 2e72   https://xclim.r
-00005360: 6561 6474 6865 646f 6373 2e69 6f2f 656e  eadthedocs.io/en
-00005370: 2f73 7461 626c 652f 6170 692e 6874 6d6c  /stable/api.html
-00005380: 2378 636c 696d 2e69 6e64 6963 6174 6f72  #xclim.indicator
-00005390: 732e 6174 6d6f 732e 7072 6563 6970 5f61  s.atmos.precip_a
-000053a0: 6363 756d 756c 6174 696f 6e0a 2020 2020  ccumulation.    
-000053b0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-000053c0: 7265 7475 726e 2078 632e 6174 6d6f 732e  return xc.atmos.
-000053d0: 7072 6563 6970 5f61 6363 756d 756c 6174  precip_accumulat
-000053e0: 696f 6e28 2a2a 7061 7261 6d73 290a 0a0a  ion(**params)...
-000053f0: 636c 6173 7320 5252 6d3a 0a20 2020 2022  class RRm:.    "
-00005400: 2222 4d65 616e 2064 6169 6c79 2070 7265  ""Mean daily pre
-00005410: 6369 7069 7461 7469 6f6e 2028 7072 292e  cipitation (pr).
-00005420: 2222 220a 0a20 2020 2064 6566 2063 6f6d  """..    def com
-00005430: 7075 7465 282a 2a70 6172 616d 7329 3a0a  pute(**params):.
-00005440: 2020 2020 2020 2020 2222 2243 616c 6375          """Calcu
-00005450: 6c61 7465 206d 6561 6e20 6461 696c 7920  late mean daily 
-00005460: 7072 6563 6970 6974 6174 696f 6e2e 0a0a  precipitation...
-00005470: 2020 2020 2020 2020 5265 7475 726e 730a          Returns.
-00005480: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d0a          -------.
-00005490: 2020 2020 2020 2020 7861 7272 6179 2e44          xarray.D
-000054a0: 6174 6141 7272 6179 0a20 2020 2020 2020  ataArray.       
-000054b0: 2020 2020 204d 6561 6e20 6461 696c 7920       Mean daily 
-000054c0: 7072 6563 6970 6974 6174 696f 6e2e 0a0a  precipitation...
-000054d0: 2020 2020 2020 2020 4e6f 7465 730a 2020          Notes.  
-000054e0: 2020 2020 2020 2d2d 2d2d 2d0a 2020 2020        -----.    
-000054f0: 2020 2020 466f 7220 696e 666f 726d 6174      For informat
-00005500: 696f 6e20 6f6e 2074 6865 2069 6e70 7574  ion on the input
-00005510: 2070 6172 616d 6574 6572 7320 7365 653a   parameters see:
-00005520: 0a20 2020 2020 2020 2020 2020 2068 7474  .            htt
-00005530: 7073 3a2f 2f78 636c 696d 2e72 6561 6474  ps://xclim.readt
-00005540: 6865 646f 6373 2e69 6f2f 656e 2f73 7461  hedocs.io/en/sta
-00005550: 626c 652f 6170 692e 6874 6d6c 2378 636c  ble/api.html#xcl
-00005560: 696d 2e69 6e64 6963 6174 6f72 732e 6174  im.indicators.at
-00005570: 6d6f 732e 7072 6563 6970 5f61 7665 7261  mos.precip_avera
-00005580: 6765 0a20 2020 2020 2020 2022 2222 0a20  ge.        """. 
-00005590: 2020 2020 2020 2072 6574 7572 6e20 7863         return xc
-000055a0: 2e61 746d 6f73 2e70 7265 6369 705f 6176  .atmos.precip_av
-000055b0: 6572 6167 6528 2a2a 7061 7261 6d73 290a  erage(**params).
-000055c0: 0a0a 636c 6173 7320 5252 313a 0a20 2020  ..class RR1:.   
-000055d0: 2022 2222 4e75 6d62 6572 206f 6620 7765   """Number of we
-000055e0: 7420 6461 7973 2028 7072 292e 2222 220a  t days (pr).""".
-000055f0: 0a20 2020 2064 6566 2063 6f6d 7075 7465  .    def compute
-00005600: 282a 2a70 6172 616d 7329 3a0a 2020 2020  (**params):.    
-00005610: 2020 2020 2222 2243 616c 6375 6c61 7465      """Calculate
-00005620: 206e 756d 6265 7220 6f66 2077 6574 2064   number of wet d
-00005630: 6179 7320 2870 7220 3e3d 2031 206d 6d2f  ays (pr >= 1 mm/
-00005640: 6461 7929 2e0a 0a20 2020 2020 2020 2052  day)...        R
-00005650: 6574 7572 6e73 0a20 2020 2020 2020 202d  eturns.        -
-00005660: 2d2d 2d2d 2d2d 0a20 2020 2020 2020 2078  ------.        x
-00005670: 6172 7261 792e 4461 7461 4172 7261 790a  array.DataArray.
-00005680: 2020 2020 2020 2020 2020 2020 4e75 6d62              Numb
-00005690: 6572 206f 6620 7765 7420 6461 7973 2028  er of wet days (
-000056a0: 7072 203e 3d20 3120 6d6d 2f64 6179 292e  pr >= 1 mm/day).
-000056b0: 0a0a 2020 2020 2020 2020 4e6f 7465 730a  ..        Notes.
-000056c0: 2020 2020 2020 2020 2d2d 2d2d 2d0a 2020          -----.  
-000056d0: 2020 2020 2020 466f 7220 696e 666f 726d        For inform
-000056e0: 6174 696f 6e20 6f6e 2074 6865 2069 6e70  ation on the inp
-000056f0: 7574 2070 6172 616d 6574 6572 7320 7365  ut parameters se
-00005700: 653a 0a20 2020 2020 2020 2020 2020 2068  e:.            h
-00005710: 7474 7073 3a2f 2f78 636c 696d 2e72 6561  ttps://xclim.rea
-00005720: 6474 6865 646f 6373 2e69 6f2f 656e 2f73  dthedocs.io/en/s
-00005730: 7461 626c 652f 6170 692e 6874 6d6c 2378  table/api.html#x
-00005740: 636c 696d 2e69 6e64 6963 6174 6f72 732e  clim.indicators.
-00005750: 6174 6d6f 732e 7765 7464 6179 730a 2020  atmos.wetdays.  
-00005760: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-00005770: 2020 7265 7475 726e 2078 632e 6174 6d6f    return xc.atmo
-00005780: 732e 7765 7464 6179 7328 0a20 2020 2020  s.wetdays(.     
-00005790: 2020 2020 2020 2074 6872 6573 683d 2231         thresh="1
-000057a0: 206d 6d2f 6461 7922 2c0a 2020 2020 2020   mm/day",.      
-000057b0: 2020 2020 2020 2a2a 7061 7261 6d73 2c0a        **params,.
-000057c0: 2020 2020 2020 2020 290a 0a0a 636c 6173          )...clas
-000057d0: 7320 5231 306d 6d3a 0a20 2020 2022 2222  s R10mm:.    """
-000057e0: 4e75 6d62 6572 206f 6620 6865 6176 7920  Number of heavy 
-000057f0: 7072 6563 6970 6974 6174 696f 6e20 6461  precipitation da
-00005800: 7973 2028 7072 292e 2222 220a 0a20 2020  ys (pr)."""..   
-00005810: 2064 6566 2063 6f6d 7075 7465 282a 2a70   def compute(**p
-00005820: 6172 616d 7329 3a0a 2020 2020 2020 2020  arams):.        
-00005830: 2222 2243 616c 6375 6c61 7465 206e 756d  """Calculate num
-00005840: 6265 7220 6f66 2077 6574 2064 6179 7320  ber of wet days 
-00005850: 2870 7220 3e3d 2031 3020 6d6d 2f64 6179  (pr >= 10 mm/day
-00005860: 292e 0a0a 2020 2020 2020 2020 5265 7475  )...        Retu
-00005870: 726e 730a 2020 2020 2020 2020 2d2d 2d2d  rns.        ----
-00005880: 2d2d 2d0a 2020 2020 2020 2020 7861 7272  ---.        xarr
-00005890: 6179 2e44 6174 6141 7272 6179 0a20 2020  ay.DataArray.   
-000058a0: 2020 2020 2020 2020 204e 756d 6265 7220           Number 
-000058b0: 6f66 2077 6574 2064 6179 7320 2870 7220  of wet days (pr 
-000058c0: 3e3d 2031 3020 6d6d 2f64 6179 292e 0a0a  >= 10 mm/day)...
-000058d0: 2020 2020 2020 2020 4e6f 7465 730a 2020          Notes.  
-000058e0: 2020 2020 2020 2d2d 2d2d 2d0a 2020 2020        -----.    
-000058f0: 2020 2020 466f 7220 696e 666f 726d 6174      For informat
-00005900: 696f 6e20 6f6e 2074 6865 2069 6e70 7574  ion on the input
-00005910: 2070 6172 616d 6574 6572 7320 7365 653a   parameters see:
-00005920: 0a20 2020 2020 2020 2020 2020 2068 7474  .            htt
-00005930: 7073 3a2f 2f78 636c 696d 2e72 6561 6474  ps://xclim.readt
-00005940: 6865 646f 6373 2e69 6f2f 656e 2f73 7461  hedocs.io/en/sta
-00005950: 626c 652f 6170 692e 6874 6d6c 2378 636c  ble/api.html#xcl
-00005960: 696d 2e69 6e64 6963 6174 6f72 732e 6174  im.indicators.at
-00005970: 6d6f 732e 7765 7464 6179 730a 2020 2020  mos.wetdays.    
-00005980: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-00005990: 7265 7475 726e 2078 632e 6174 6d6f 732e  return xc.atmos.
-000059a0: 7765 7464 6179 7328 0a20 2020 2020 2020  wetdays(.       
-000059b0: 2020 2020 2074 6872 6573 683d 2231 3020       thresh="10 
-000059c0: 6d6d 2f64 6179 222c 0a20 2020 2020 2020  mm/day",.       
-000059d0: 2020 2020 202a 2a70 6172 616d 732c 0a20       **params,. 
-000059e0: 2020 2020 2020 2029 0a0a 0a63 6c61 7373         )...class
-000059f0: 2052 3230 6d6d 3a0a 2020 2020 2222 224e   R20mm:.    """N
-00005a00: 756d 6265 7220 6f66 2076 6572 7920 6865  umber of very he
-00005a10: 6176 7920 7072 6563 6970 6974 6174 696f  avy precipitatio
-00005a20: 6e20 6461 7973 2028 7072 292e 2222 220a  n days (pr).""".
-00005a30: 0a20 2020 2064 6566 2063 6f6d 7075 7465  .    def compute
-00005a40: 282a 2a70 6172 616d 7329 3a0a 2020 2020  (**params):.    
-00005a50: 2020 2020 2222 2243 616c 6375 6c61 7465      """Calculate
-00005a60: 206e 756d 6265 7220 6f66 2077 6574 2064   number of wet d
-00005a70: 6179 7320 2870 7220 3e3d 2032 3020 6d6d  ays (pr >= 20 mm
-00005a80: 2f64 6179 292e 0a0a 2020 2020 2020 2020  /day)...        
-00005a90: 5265 7475 726e 730a 2020 2020 2020 2020  Returns.        
-00005aa0: 2d2d 2d2d 2d2d 2d0a 2020 2020 2020 2020  -------.        
-00005ab0: 7861 7272 6179 2e44 6174 6141 7272 6179  xarray.DataArray
-00005ac0: 0a20 2020 2020 2020 2020 2020 204e 756d  .            Num
-00005ad0: 6265 7220 6f66 2077 6574 2064 6179 7320  ber of wet days 
-00005ae0: 2870 7220 3e3d 2032 3020 6d6d 2f64 6179  (pr >= 20 mm/day
-00005af0: 292e 0a0a 2020 2020 2020 2020 4e6f 7465  )...        Note
-00005b00: 730a 2020 2020 2020 2020 2d2d 2d2d 2d0a  s.        -----.
-00005b10: 2020 2020 2020 2020 466f 7220 696e 666f          For info
-00005b20: 726d 6174 696f 6e20 6f6e 2074 6865 2069  rmation on the i
-00005b30: 6e70 7574 2070 6172 616d 6574 6572 7320  nput parameters 
-00005b40: 7365 653a 0a20 2020 2020 2020 2020 2020  see:.           
-00005b50: 2068 7474 7073 3a2f 2f78 636c 696d 2e72   https://xclim.r
-00005b60: 6561 6474 6865 646f 6373 2e69 6f2f 656e  eadthedocs.io/en
-00005b70: 2f73 7461 626c 652f 6170 692e 6874 6d6c  /stable/api.html
-00005b80: 2378 636c 696d 2e69 6e64 6963 6174 6f72  #xclim.indicator
-00005b90: 732e 6174 6d6f 732e 7765 7464 6179 730a  s.atmos.wetdays.
-00005ba0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00005bb0: 2020 2020 7265 7475 726e 2078 632e 6174      return xc.at
-00005bc0: 6d6f 732e 7765 7464 6179 7328 0a20 2020  mos.wetdays(.   
-00005bd0: 2020 2020 2020 2020 2074 6872 6573 683d           thresh=
-00005be0: 2232 3020 6d6d 2f64 6179 222c 0a20 2020  "20 mm/day",.   
-00005bf0: 2020 2020 2020 2020 202a 2a70 6172 616d           **param
-00005c00: 732c 0a20 2020 2020 2020 2029 0a0a 0a63  s,.        )...c
-00005c10: 6c61 7373 2052 3235 6d6d 3a0a 2020 2020  lass R25mm:.    
-00005c20: 2222 224e 756d 6265 7220 6f66 2073 7570  """Number of sup
-00005c30: 6572 2068 6561 7679 2070 7265 6369 7069  er heavy precipi
-00005c40: 7461 7469 6f6e 2064 6179 7320 2870 7229  tation days (pr)
-00005c50: 2e22 2222 0a0a 2020 2020 6465 6620 636f  ."""..    def co
-00005c60: 6d70 7574 6528 2a2a 7061 7261 6d73 293a  mpute(**params):
-00005c70: 0a20 2020 2020 2020 2022 2222 4361 6c63  .        """Calc
-00005c80: 756c 6174 6520 6e75 6d62 6572 206f 6620  ulate number of 
-00005c90: 7765 7420 6461 7973 2028 7072 203e 3d20  wet days (pr >= 
-00005ca0: 3235 206d 6d2f 6461 7929 2e0a 0a20 2020  25 mm/day)...   
-00005cb0: 2020 2020 2052 6574 7572 6e73 0a20 2020       Returns.   
-00005cc0: 2020 2020 202d 2d2d 2d2d 2d2d 0a20 2020       -------.   
-00005cd0: 2020 2020 2078 6172 7261 792e 4461 7461       xarray.Data
-00005ce0: 4172 7261 790a 2020 2020 2020 2020 2020  Array.          
-00005cf0: 2020 4e75 6d62 6572 206f 6620 7765 7420    Number of wet 
-00005d00: 6461 7973 2028 7072 203e 3d20 3235 206d  days (pr >= 25 m
-00005d10: 6d2f 6461 7929 2e0a 0a20 2020 2020 2020  m/day)...       
-00005d20: 204e 6f74 6573 0a20 2020 2020 2020 202d   Notes.        -
-00005d30: 2d2d 2d2d 0a20 2020 2020 2020 2046 6f72  ----.        For
-00005d40: 2069 6e66 6f72 6d61 7469 6f6e 206f 6e20   information on 
-00005d50: 7468 6520 696e 7075 7420 7061 7261 6d65  the input parame
-00005d60: 7465 7273 2073 6565 3a0a 2020 2020 2020  ters see:.      
-00005d70: 2020 2020 2020 6874 7470 733a 2f2f 7863        https://xc
-00005d80: 6c69 6d2e 7265 6164 7468 6564 6f63 732e  lim.readthedocs.
-00005d90: 696f 2f65 6e2f 7374 6162 6c65 2f61 7069  io/en/stable/api
-00005da0: 2e68 746d 6c23 7863 6c69 6d2e 696e 6469  .html#xclim.indi
-00005db0: 6361 746f 7273 2e61 746d 6f73 2e77 6574  cators.atmos.wet
-00005dc0: 6461 7973 0a20 2020 2020 2020 2022 2222  days.        """
-00005dd0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00005de0: 7863 2e61 746d 6f73 2e77 6574 6461 7973  xc.atmos.wetdays
-00005df0: 280a 2020 2020 2020 2020 2020 2020 7468  (.            th
-00005e00: 7265 7368 3d22 3235 206d 6d2f 6461 7922  resh="25 mm/day"
-00005e10: 2c0a 2020 2020 2020 2020 2020 2020 2a2a  ,.            **
-00005e20: 7061 7261 6d73 2c0a 2020 2020 2020 2020  params,.        
-00005e30: 290a 0a0a 636c 6173 7320 5252 5959 703a  )...class RRYYp:
-00005e40: 0a20 2020 2022 2222 5072 6563 6970 2070  .    """Precip p
-00005e50: 6572 6365 6e74 696c 2076 616c 7565 2066  ercentil value f
-00005e60: 6f72 2077 6574 2064 6179 7320 2870 7229  or wet days (pr)
-00005e70: 2e22 2222 0a0a 2020 2020 7065 7220 3d20  ."""..    per = 
-00005e80: 3735 0a20 2020 2074 6872 6573 6820 3d20  75.    thresh = 
-00005e90: 310a 2020 2020 6261 7365 5f70 6572 696f  1.    base_perio
-00005ea0: 645f 7469 6d65 5f72 616e 6765 203d 2042  d_time_range = B
-00005eb0: 4153 455f 5045 5249 4f44 0a0a 2020 2020  ASE_PERIOD..    
-00005ec0: 6465 6620 636f 6d70 7574 6528 0a20 2020  def compute(.   
-00005ed0: 2020 2020 2070 6572 3d70 6572 2c0a 2020       per=per,.  
-00005ee0: 2020 2020 2020 7468 7265 7368 3d74 6872        thresh=thr
-00005ef0: 6573 682c 0a20 2020 2020 2020 2062 6173  esh,.        bas
-00005f00: 655f 7065 7269 6f64 5f74 696d 655f 7261  e_period_time_ra
-00005f10: 6e67 653d 6261 7365 5f70 6572 696f 645f  nge=base_period_
-00005f20: 7469 6d65 5f72 616e 6765 2c0a 2020 2020  time_range,.    
-00005f30: 2020 2020 2a2a 7061 7261 6d73 2c0a 2020      **params,.  
-00005f40: 2020 293a 0a20 2020 2020 2020 2022 2222    ):.        """
-00005f50: 4361 6c63 756c 6174 6520 7072 6563 6970  Calculate precip
-00005f60: 2070 6572 6365 6e74 696c 6520 7265 6665   percentile refe
-00005f70: 7265 6e63 6520 7661 6c75 650a 2020 2020  rence value.    
-00005f80: 2020 2020 666f 7220 7765 7420 6461 7973      for wet days
-00005f90: 2028 7072 203e 2074 6872 6573 6829 2e0a   (pr > thresh)..
-00005fa0: 0a20 2020 2020 2020 2050 6172 616d 6574  .        Paramet
-00005fb0: 6572 730a 2020 2020 2020 2020 2d2d 2d2d  ers.        ----
-00005fc0: 2d2d 2d2d 2d2d 0a20 2020 2020 2020 2070  ------.        p
-00005fd0: 6572 3a20 696e 740a 2020 2020 2020 2020  er: int.        
-00005fe0: 2020 2020 5065 7263 656e 7469 6c65 2076      Percentile v
-00005ff0: 616c 7565 2e0a 2020 2020 2020 2020 7468  alue..        th
-00006000: 7265 7368 3a20 696e 7420 6f72 2073 7472  resh: int or str
-00006010: 696e 670a 2020 2020 2020 2020 2020 2020  ing.            
-00006020: 5468 7265 7368 6f6c 6420 7072 6563 6970  Threshold precip
-00006030: 6974 6174 696f 6e20 6162 6f76 6520 7768  itation above wh
-00006040: 6963 6820 6120 6461 7920 6973 2063 6f6e  ich a day is con
-00006050: 7369 6465 7265 640a 2020 2020 2020 2020  sidered.        
-00006060: 2020 2020 6173 2061 2077 6574 2064 6179      as a wet day
-00006070: 2028 6465 6661 756c 743a 2031 206d 6d2f   (default: 1 mm/
-00006080: 6461 7929 2e0a 2020 2020 2020 2020 2020  day)..          
-00006090: 2020 4966 2074 7970 6520 6f66 2074 6872    If type of thr
-000060a0: 6573 686f 6c64 2069 7320 616e 2069 6e74  eshold is an int
-000060b0: 6567 6572 2074 6865 2075 6e69 7420 6973  eger the unit is
-000060c0: 2073 6574 2074 6f20 6d6d 2f64 6179 2e0a   set to mm/day..
-000060d0: 2020 2020 2020 2020 6261 7365 5f70 6572          base_per
-000060e0: 696f 645f 7469 6d65 5f72 616e 6765 3a20  iod_time_range: 
-000060f0: 6c69 7374 0a20 2020 2020 2020 2020 2020  list.           
-00006100: 204c 6973 7420 7769 7468 206c 6566 7420   List with left 
-00006110: 626f 756e 6420 6973 2073 7461 7274 2079  bound is start y
-00006120: 6561 7220 7374 7269 6e67 2061 6e64 2072  ear string and r
-00006130: 6967 6874 2062 6f75 6e64 0a20 2020 2020  ight bound.     
-00006140: 2020 2020 2020 2069 7320 656e 6420 7965         is end ye
-00006150: 6172 2073 7472 696e 6720 666f 7220 6361  ar string for ca
-00006160: 6c63 756c 6174 696e 6720 7468 6520 7072  lculating the pr
-00006170: 6563 6970 2070 6572 6365 6e74 696c 650a  ecip percentile.
-00006180: 2020 2020 2020 2020 2020 2020 7265 6665              refe
-00006190: 7265 6e63 6520 7661 6c75 652e 0a0a 2020  rence value...  
-000061a0: 2020 2020 2020 5265 7475 726e 730a 2020        Returns.  
-000061b0: 2020 2020 2020 2d2d 2d2d 2d2d 2d0a 2020        -------.  
-000061c0: 2020 2020 2020 7861 7272 6179 2e44 6174        xarray.Dat
-000061d0: 6141 7272 6179 0a20 2020 2020 2020 2020  aArray.         
-000061e0: 2020 2050 7265 6369 7020 7b70 6572 7d74     Precip {per}t
-000061f0: 6820 7065 7263 656e 7469 6c20 7265 6665  h percentil refe
-00006200: 7265 6e63 6520 7661 6c75 650a 2020 2020  rence value.    
-00006210: 2020 2020 2020 2020 666f 7220 7765 7420          for wet 
-00006220: 6461 7973 2028 7072 203e 207b 7468 7265  days (pr > {thre
-00006230: 7368 7d29 2e0a 2020 2020 2020 2020 2222  sh})..        ""
-00006240: 220a 2020 2020 2020 2020 7468 7265 7368  ".        thresh
-00006250: 203d 205f 7468 7265 7368 5f73 7472 696e   = _thresh_strin
-00006260: 6728 7468 7265 7368 2c20 226d 6d2f 6461  g(thresh, "mm/da
-00006270: 7922 290a 2020 2020 2020 2020 6461 203d  y").        da =
-00006280: 205f 6765 745f 6461 2870 6172 616d 732c   _get_da(params,
-00006290: 2022 7072 2229 0a20 2020 2020 2020 2064   "pr").        d
-000062a0: 6120 3d20 5f66 696c 7465 725f 6f75 745f  a = _filter_out_
-000062b0: 736d 616c 6c5f 7661 6c75 6573 2864 612c  small_values(da,
-000062c0: 2074 6872 6573 682c 2063 6f6e 7465 7874   thresh, context
-000062d0: 3d22 6879 6472 6f22 290a 2020 2020 2020  ="hydro").      
-000062e0: 2020 7265 7475 726e 205f 6765 745f 7065    return _get_pe
-000062f0: 7263 656e 7469 6c65 280a 2020 2020 2020  rcentile(.      
-00006300: 2020 2020 2020 6461 3d64 612c 0a20 2020        da=da,.   
-00006310: 2020 2020 2020 2020 2070 6572 3d70 6572           per=per
-00006320: 2c0a 2020 2020 2020 2020 2020 2020 6261  ,.            ba
-00006330: 7365 5f70 6572 696f 645f 7469 6d65 5f72  se_period_time_r
-00006340: 616e 6765 3d62 6173 655f 7065 7269 6f64  ange=base_period
-00006350: 5f74 696d 655f 7261 6e67 652c 0a20 2020  _time_range,.   
-00006360: 2020 2020 2029 0a0a 0a63 6c61 7373 2052       )...class R
-00006370: 5959 703a 0a20 2020 2022 2222 4e75 6d62  YYp:.    """Numb
-00006380: 6572 206f 6620 7765 7420 6461 7973 2077  er of wet days w
-00006390: 6974 6820 7072 6563 6970 206f 7665 7220  ith precip over 
-000063a0: 6120 6769 7665 6e20 7065 7263 656e 7469  a given percenti
-000063b0: 6c65 2028 7072 292e 2222 220a 0a20 2020  le (pr)."""..   
-000063c0: 2070 6572 203d 2037 350a 2020 2020 7468   per = 75.    th
-000063d0: 7265 7368 203d 2031 0a20 2020 2062 6173  resh = 1.    bas
-000063e0: 655f 7065 7269 6f64 5f74 696d 655f 7261  e_period_time_ra
-000063f0: 6e67 6520 3d20 4241 5345 5f50 4552 494f  nge = BASE_PERIO
-00006400: 440a 0a20 2020 2064 6566 2063 6f6d 7075  D..    def compu
-00006410: 7465 280a 2020 2020 2020 2020 7065 723d  te(.        per=
-00006420: 7065 722c 0a20 2020 2020 2020 2074 6872  per,.        thr
-00006430: 6573 683d 7468 7265 7368 2c0a 2020 2020  esh=thresh,.    
-00006440: 2020 2020 6261 7365 5f70 6572 696f 645f      base_period_
-00006450: 7469 6d65 5f72 616e 6765 3d62 6173 655f  time_range=base_
-00006460: 7065 7269 6f64 5f74 696d 655f 7261 6e67  period_time_rang
-00006470: 652c 0a20 2020 2020 2020 202a 2a70 6172  e,.        **par
-00006480: 616d 732c 0a20 2020 2029 3a0a 2020 2020  ams,.    ):.    
-00006490: 2020 2020 2222 2243 616c 6375 6c61 7465      """Calculate
-000064a0: 206e 756d 6265 7220 6f66 2077 6574 2064   number of wet d
-000064b0: 6179 7320 2870 7220 3e20 7468 7265 7368  ays (pr > thresh
-000064c0: 290a 2020 2020 2020 2020 7769 7468 2070  ).        with p
-000064d0: 7265 6369 7020 6f76 6572 2061 2067 6976  recip over a giv
-000064e0: 656e 2070 6572 6365 6e74 696c 652e 0a0a  en percentile...
-000064f0: 2020 2020 2020 2020 5061 7261 6d65 7465          Paramete
-00006500: 7273 0a20 2020 2020 2020 202d 2d2d 2d2d  rs.        -----
-00006510: 2d2d 2d2d 2d0a 2020 2020 2020 2020 7065  -----.        pe
-00006520: 723a 2069 6e74 0a20 2020 2020 2020 2020  r: int.         
-00006530: 2020 2050 7265 6369 7069 7461 7469 6f6e     Precipitation
-00006540: 2070 6572 6365 6e74 696c 6520 7661 6c75   percentile valu
-00006550: 652e 0a20 2020 2020 2020 2074 6872 6573  e..        thres
-00006560: 683a 2069 6e74 206f 7220 7374 7269 6e67  h: int or string
-00006570: 0a20 2020 2020 2020 2020 2020 2054 6872  .            Thr
-00006580: 6573 686f 6c64 2070 7265 6369 7069 7461  eshold precipita
-00006590: 7469 6f6e 2061 626f 7665 2077 6869 6368  tion above which
-000065a0: 2061 2064 6179 2069 7320 636f 6e73 6964   a day is consid
-000065b0: 6572 6564 0a20 2020 2020 2020 2020 2020  ered.           
-000065c0: 2061 7320 6120 7765 7420 6461 7920 2864   as a wet day (d
-000065d0: 6566 6175 6c74 3a20 3120 6d6d 2f64 6179  efault: 1 mm/day
-000065e0: 292e 0a20 2020 2020 2020 2020 2020 2049  )..            I
-000065f0: 6620 7479 7065 206f 6620 7468 7265 7368  f type of thresh
-00006600: 6f6c 6420 6973 2061 6e20 696e 7465 6765  old is an intege
-00006610: 7220 7468 6520 756e 6974 2069 7320 7365  r the unit is se
-00006620: 7420 746f 206d 6d2f 6461 792e 0a20 2020  t to mm/day..   
-00006630: 2020 2020 2062 6173 655f 7065 7269 6f64       base_period
-00006640: 5f74 696d 655f 7261 6e67 653a 206c 6973  _time_range: lis
-00006650: 740a 2020 2020 2020 2020 2020 2020 4c69  t.            Li
-00006660: 7374 2077 6974 6820 6c65 6674 2062 6f75  st with left bou
-00006670: 6e64 2069 7320 7374 6172 7420 7965 6172  nd is start year
-00006680: 2073 7472 696e 6720 616e 6420 7269 6768   string and righ
-00006690: 7420 626f 756e 640a 2020 2020 2020 2020  t bound.        
-000066a0: 2020 2020 6973 2065 6e64 2079 6561 7220      is end year 
-000066b0: 7374 7269 6e67 2066 6f72 2063 616c 6375  string for calcu
-000066c0: 6c61 7469 6e67 2074 6865 2070 7265 6369  lating the preci
-000066d0: 700a 2020 2020 2020 2020 2020 2020 7065  p.            pe
-000066e0: 7263 656e 7469 6c65 2072 6566 6572 656e  rcentile referen
-000066f0: 6365 2076 616c 7565 2e0a 0a20 2020 2020  ce value...     
-00006700: 2020 2052 6574 7572 6e73 0a20 2020 2020     Returns.     
-00006710: 2020 202d 2d2d 2d2d 2d2d 0a20 2020 2020     -------.     
-00006720: 2020 2078 6172 7261 792e 4461 7461 4172     xarray.DataAr
-00006730: 7261 790a 2020 2020 2020 2020 2020 2020  ray.            
-00006740: 4e75 6d62 6572 206f 6620 7765 7420 6461  Number of wet da
-00006750: 7973 2028 7079 7220 3e20 7b74 6872 6573  ys (pyr > {thres
-00006760: 687d 2920 6f76 6572 2061 207b 7065 727d  h}) over a {per}
-00006770: 7468 2070 6572 6365 6e74 696c 652e 0a0a  th percentile...
-00006780: 2020 2020 2020 2020 4e6f 7465 730a 2020          Notes.  
-00006790: 2020 2020 2020 2d2d 2d2d 2d0a 2020 2020        -----.    
-000067a0: 2020 2020 466f 7220 6d6f 7265 2069 6e66      For more inf
-000067b0: 6f72 6d61 7469 6f6e 206f 6e20 7468 6520  ormation on the 
-000067c0: 696e 7075 7420 7061 7261 6d65 7465 7273  input parameters
-000067d0: 2073 6565 3a0a 2020 2020 2020 2020 2020   see:.          
-000067e0: 2020 6874 7470 733a 2f2f 7863 6c69 6d2e    https://xclim.
-000067f0: 7265 6164 7468 6564 6f63 732e 696f 2f65  readthedocs.io/e
-00006800: 6e2f 7374 6162 6c65 2f61 7069 2e68 746d  n/stable/api.htm
-00006810: 6c23 7863 6c69 6d2e 696e 6469 6361 746f  l#xclim.indicato
-00006820: 7273 2e61 746d 6f73 2e64 6179 735f 6f76  rs.atmos.days_ov
-00006830: 6572 5f70 7265 6369 705f 646f 795f 7468  er_precip_doy_th
-00006840: 7265 7368 0a20 2020 2020 2020 2022 2222  resh.        """
-00006850: 0a20 2020 2020 2020 2074 6872 6573 6820  .        thresh 
-00006860: 3d20 5f74 6872 6573 685f 7374 7269 6e67  = _thresh_string
-00006870: 2874 6872 6573 682c 2022 6d6d 2f64 6179  (thresh, "mm/day
-00006880: 2229 0a20 2020 2020 2020 2064 6120 3d20  ").        da = 
-00006890: 5f67 6574 5f64 6128 7061 7261 6d73 2c20  _get_da(params, 
-000068a0: 2270 7222 290a 2020 2020 2020 2020 6461  "pr").        da
-000068b0: 5f70 7220 3d20 5f66 696c 7465 725f 6f75  _pr = _filter_ou
-000068c0: 745f 736d 616c 6c5f 7661 6c75 6573 2864  t_small_values(d
-000068d0: 612c 2074 6872 6573 682c 2063 6f6e 7465  a, thresh, conte
-000068e0: 7874 3d22 6879 6472 6f22 290a 2020 2020  xt="hydro").    
-000068f0: 2020 2020 7072 5f70 6572 203d 205f 6765      pr_per = _ge
-00006900: 745f 7065 7263 656e 7469 6c65 280a 2020  t_percentile(.  
-00006910: 2020 2020 2020 2020 2020 6461 3d64 615f            da=da_
-00006920: 7072 2c0a 2020 2020 2020 2020 2020 2020  pr,.            
-00006930: 7065 723d 7065 722c 0a20 2020 2020 2020  per=per,.       
-00006940: 2020 2020 2062 6173 655f 7065 7269 6f64       base_period
-00006950: 5f74 696d 655f 7261 6e67 653d 6261 7365  _time_range=base
-00006960: 5f70 6572 696f 645f 7469 6d65 5f72 616e  _period_time_ran
-00006970: 6765 2c0a 2020 2020 2020 2020 290a 2020  ge,.        ).  
-00006980: 2020 2020 2020 7265 7475 726e 2078 632e        return xc.
-00006990: 6174 6d6f 732e 6461 7973 5f6f 7665 725f  atmos.days_over_
-000069a0: 7072 6563 6970 5f64 6f79 5f74 6872 6573  precip_doy_thres
-000069b0: 6828 0a20 2020 2020 2020 2020 2020 2070  h(.            p
-000069c0: 725f 7065 723d 7072 5f70 6572 2c0a 2020  r_per=pr_per,.  
-000069d0: 2020 2020 2020 2020 2020 2a2a 7061 7261            **para
-000069e0: 6d73 2c0a 2020 2020 2020 2020 290a 0a0a  ms,.        )...
-000069f0: 636c 6173 7320 5259 596d 6d3a 0a20 2020  class RYYmm:.   
-00006a00: 2022 2222 4e75 6d62 6572 206f 6620 6461   """Number of da
-00006a10: 7973 2077 6974 6820 7072 6563 6970 206f  ys with precip o
-00006a20: 7665 7220 7468 7265 7368 6f6c 6420 2870  ver threshold (p
-00006a30: 7229 2e22 2222 0a0a 2020 2020 7468 7265  r)."""..    thre
-00006a40: 7368 203d 2032 350a 0a20 2020 2064 6566  sh = 25..    def
-00006a50: 2063 6f6d 7075 7465 2874 6872 6573 683d   compute(thresh=
-00006a60: 7468 7265 7368 2c20 2a2a 7061 7261 6d73  thresh, **params
-00006a70: 293a 0a20 2020 2020 2020 2022 2222 4361  ):.        """Ca
-00006a80: 6c63 756c 6174 6520 6e75 6d62 6572 206f  lculate number o
-00006a90: 6620 7765 7420 6461 7973 2e0a 0a20 2020  f wet days...   
-00006aa0: 2020 2020 2050 6172 616d 6574 6572 730a       Parameters.
-00006ab0: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d2d          --------
-00006ac0: 2d2d 0a20 2020 2020 2020 2074 6872 6573  --.        thres
-00006ad0: 683a 0a20 2020 2020 2020 2054 6872 6573  h:.        Thres
-00006ae0: 686f 6c64 2070 7265 6369 7069 7461 7469  hold precipitati
-00006af0: 6f6e 2061 626f 7665 2077 6869 6368 2061  on above which a
-00006b00: 2064 6179 2069 7320 636f 6e73 6964 6572   day is consider
-00006b10: 6564 0a20 2020 2020 2020 2020 2020 2061  ed.            a
-00006b20: 7320 6120 7765 7420 6461 7928 6465 6661  s a wet day(defa
-00006b30: 756c 743a 2032 3520 6d6d 2f64 6179 292e  ult: 25 mm/day).
-00006b40: 0a20 2020 2020 2020 2020 2020 2049 6620  .            If 
-00006b50: 7479 7065 206f 6620 7468 7265 7368 6f6c  type of threshol
-00006b60: 6420 6973 2061 6e20 696e 7465 6765 7220  d is an integer 
-00006b70: 7468 6520 756e 6974 2069 7320 7365 7420  the unit is set 
-00006b80: 746f 206d 6d2f 6461 792e 0a0a 2020 2020  to mm/day...    
-00006b90: 2020 2020 5265 7475 726e 730a 2020 2020      Returns.    
-00006ba0: 2020 2020 2d2d 2d2d 2d2d 2d0a 2020 2020      -------.    
-00006bb0: 2020 2020 7861 7272 6179 2e44 6174 6141      xarray.DataA
-00006bc0: 7272 6179 0a20 2020 2020 2020 2020 2020  rray.           
-00006bd0: 204e 756d 6265 7220 6f66 2077 6574 2064   Number of wet d
-00006be0: 6179 7320 2870 7220 3e20 7b74 6872 6573  ays (pr > {thres
-00006bf0: 687d 292e 0a0a 2020 2020 2020 2020 4e6f  h})...        No
-00006c00: 7465 730a 2020 2020 2020 2020 2d2d 2d2d  tes.        ----
-00006c10: 2d0a 2020 2020 2020 2020 466f 7220 6d6f  -.        For mo
-00006c20: 7265 2069 6e66 6f72 6d61 7469 6f6e 206f  re information o
-00006c30: 6e20 7468 6520 696e 7075 7420 7061 7261  n the input para
-00006c40: 6d65 7465 7273 2073 6565 3a0a 2020 2020  meters see:.    
-00006c50: 2020 2020 2020 2020 6874 7470 733a 2f2f          https://
-00006c60: 7863 6c69 6d2e 7265 6164 7468 6564 6f63  xclim.readthedoc
-00006c70: 732e 696f 2f65 6e2f 7374 6162 6c65 2f61  s.io/en/stable/a
-00006c80: 7069 2e68 746d 6c23 7863 6c69 6d2e 696e  pi.html#xclim.in
-00006c90: 6469 6361 746f 7273 2e61 746d 6f73 2e77  dicators.atmos.w
-00006ca0: 6574 6461 7973 0a20 2020 2020 2020 2022  etdays.        "
-00006cb0: 2222 0a20 2020 2020 2020 2074 6872 6573  "".        thres
-00006cc0: 6820 3d20 5f74 6872 6573 685f 7374 7269  h = _thresh_stri
-00006cd0: 6e67 2874 6872 6573 682c 2022 6d6d 2f64  ng(thresh, "mm/d
-00006ce0: 6179 2229 0a20 2020 2020 2020 2072 6574  ay").        ret
-00006cf0: 7572 6e20 7863 2e61 746d 6f73 2e77 6574  urn xc.atmos.wet
-00006d00: 6461 7973 280a 2020 2020 2020 2020 2020  days(.          
-00006d10: 2020 7468 7265 7368 3d74 6872 6573 682c    thresh=thresh,
-00006d20: 0a20 2020 2020 2020 2020 2020 202a 2a70  .            **p
-00006d30: 6172 616d 732c 0a20 2020 2020 2020 2029  arams,.        )
-00006d40: 0a0a 0a63 6c61 7373 2052 5831 6461 793a  ...class RX1day:
-00006d50: 0a20 2020 2022 2222 4d61 7869 6d75 6d20  .    """Maximum 
-00006d60: 312d 6461 7920 746f 7461 6c20 7072 6563  1-day total prec
-00006d70: 6970 6974 6174 696f 6e20 2870 7229 2e22  ipitation (pr)."
-00006d80: 2222 0a0a 2020 2020 6465 6620 636f 6d70  ""..    def comp
-00006d90: 7574 6528 2a2a 7061 7261 6d73 293a 0a20  ute(**params):. 
-00006da0: 2020 2020 2020 2022 2222 4361 6c63 756c         """Calcul
-00006db0: 6174 6520 6d61 7869 6d75 6d20 312d 6461  ate maximum 1-da
-00006dc0: 7920 746f 7461 6c20 7072 6563 6970 6974  y total precipit
-00006dd0: 6174 696f 6e2e 0a0a 2020 2020 2020 2020  ation...        
-00006de0: 5265 7475 726e 730a 2020 2020 2020 2020  Returns.        
-00006df0: 2d2d 2d2d 2d2d 2d0a 2020 2020 2020 2020  -------.        
-00006e00: 7861 7272 6179 2e44 6174 6141 7272 6179  xarray.DataArray
-00006e10: 0a20 2020 2020 2020 2020 2020 204d 6178  .            Max
-00006e20: 696d 756d 2031 2d64 6179 2074 6f74 616c  imum 1-day total
-00006e30: 2070 7265 6369 7069 7461 7469 6f6e 2e0a   precipitation..
-00006e40: 0a20 2020 2020 2020 204e 6f74 6573 0a20  .        Notes. 
-00006e50: 2020 2020 2020 202d 2d2d 2d2d 0a20 2020         -----.   
-00006e60: 2020 2020 2046 6f72 2069 6e66 6f72 6d61       For informa
-00006e70: 7469 6f6e 206f 6e20 7468 6520 696e 7075  tion on the inpu
-00006e80: 7420 7061 7261 6d65 7465 7273 2073 6565  t parameters see
-00006e90: 3a0a 2020 2020 2020 2020 2020 2020 6874  :.            ht
-00006ea0: 7470 733a 2f2f 7863 6c69 6d2e 7265 6164  tps://xclim.read
-00006eb0: 7468 6564 6f63 732e 696f 2f65 6e2f 7374  thedocs.io/en/st
-00006ec0: 6162 6c65 2f61 7069 2e68 746d 6c23 7863  able/api.html#xc
-00006ed0: 6c69 6d2e 696e 6469 6361 746f 7273 2e61  lim.indicators.a
-00006ee0: 746d 6f73 2e6d 6178 5f31 6461 795f 7072  tmos.max_1day_pr
-00006ef0: 6563 6970 6974 6174 696f 6e5f 616d 6f75  ecipitation_amou
-00006f00: 6e74 0a20 2020 2020 2020 2022 2222 0a20  nt.        """. 
-00006f10: 2020 2020 2020 2072 6574 7572 6e20 7863         return xc
-00006f20: 2e61 746d 6f73 2e6d 6178 5f31 6461 795f  .atmos.max_1day_
-00006f30: 7072 6563 6970 6974 6174 696f 6e5f 616d  precipitation_am
-00006f40: 6f75 6e74 282a 2a70 6172 616d 7329 0a0a  ount(**params)..
-00006f50: 0a63 6c61 7373 2052 5859 5964 6179 3a0a  .class RXYYday:.
-00006f60: 2020 2020 2222 224d 6178 696d 756d 206e      """Maximum n
-00006f70: 2d64 6179 2074 6f74 616c 2070 7265 6369  -day total preci
-00006f80: 7069 7461 7469 6f6e 2028 7072 292e 2222  pitation (pr).""
-00006f90: 220a 0a20 2020 2077 696e 646f 7720 3d20  "..    window = 
-00006fa0: 350a 0a20 2020 2064 6566 2063 6f6d 7075  5..    def compu
-00006fb0: 7465 2877 696e 646f 773d 7769 6e64 6f77  te(window=window
-00006fc0: 2c20 2a2a 7061 7261 6d73 293a 0a20 2020  , **params):.   
-00006fd0: 2020 2020 2022 2222 4361 6c63 756c 6174       """Calculat
-00006fe0: 6520 6d61 7869 6d75 6d20 7b77 696e 646f  e maximum {windo
-00006ff0: 777d 2d64 6179 2074 6f74 616c 2070 7265  w}-day total pre
-00007000: 6369 7069 7461 7469 6f6e 2e0a 0a20 2020  cipitation...   
-00007010: 2020 2020 2050 6172 616d 6574 6572 730a       Parameters.
-00007020: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d2d          --------
-00007030: 2d2d 0a20 2020 2020 2020 2077 696e 646f  --.        windo
-00007040: 773a 2069 6e74 0a20 2020 2020 2020 2020  w: int.         
-00007050: 2020 2057 696e 646f 7720 7369 7a65 2069     Window size i
-00007060: 6e20 6461 7973 2e0a 0a20 2020 2020 2020  n days...       
-00007070: 2052 6574 7572 6e73 0a20 2020 2020 2020   Returns.       
-00007080: 202d 2d2d 2d2d 2d2d 0a20 2020 2020 2020   -------.       
-00007090: 2078 6172 7261 792e 4461 7461 4172 7261   xarray.DataArra
-000070a0: 790a 2020 2020 2020 2020 2020 2020 4d61  y.            Ma
-000070b0: 7869 6d75 6d20 7b77 696e 646f 777d 2d64  ximum {window}-d
-000070c0: 6179 2074 6f74 616c 2070 7265 6369 7069  ay total precipi
-000070d0: 7461 7469 6f6e 2e0a 0a20 2020 2020 2020  tation...       
-000070e0: 204e 6f74 6573 0a20 2020 2020 2020 202d   Notes.        -
-000070f0: 2d2d 2d2d 0a20 2020 2020 2020 2046 6f72  ----.        For
-00007100: 206d 6f72 6520 696e 666f 726d 6174 696f   more informatio
-00007110: 6e20 6f6e 2074 6865 2069 6e70 7574 2070  n on the input p
-00007120: 6172 616d 6574 6572 7320 7365 653a 0a20  arameters see:. 
-00007130: 2020 2020 2020 2020 2020 2068 7474 7073             https
-00007140: 3a2f 2f78 636c 696d 2e72 6561 6474 6865  ://xclim.readthe
-00007150: 646f 6373 2e69 6f2f 656e 2f73 7461 626c  docs.io/en/stabl
-00007160: 652f 6170 692e 6874 6d6c 2378 636c 696d  e/api.html#xclim
-00007170: 2e69 6e64 6963 6174 6f72 732e 6174 6d6f  .indicators.atmo
-00007180: 732e 6d61 785f 6e5f 6461 795f 7072 6563  s.max_n_day_prec
-00007190: 6970 6974 6174 696f 6e5f 616d 6f75 6e74  ipitation_amount
-000071a0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-000071b0: 2020 2020 2072 6574 7572 6e20 7863 2e61       return xc.a
-000071c0: 746d 6f73 2e6d 6178 5f6e 5f64 6179 5f70  tmos.max_n_day_p
-000071d0: 7265 6369 7069 7461 7469 6f6e 5f61 6d6f  recipitation_amo
-000071e0: 756e 7428 0a20 2020 2020 2020 2020 2020  unt(.           
-000071f0: 2077 696e 646f 773d 7769 6e64 6f77 2c0a   window=window,.
-00007200: 2020 2020 2020 2020 2020 2020 2a2a 7061              **pa
-00007210: 7261 6d73 2c0a 2020 2020 2020 2020 290a  rams,.        ).
-00007220: 0a0a 636c 6173 7320 5259 5970 4142 533a  ..class RYYpABS:
-00007230: 0a20 2020 2022 2222 546f 7461 6c20 7072  .    """Total pr
-00007240: 6563 6970 6974 6174 696f 6e20 616d 6f75  ecipitation amou
-00007250: 6e74 2077 6974 6820 7072 6563 6970 2061  nt with precip a
-00007260: 626f 7665 2070 6572 6365 6e74 696c 650a  bove percentile.
-00007270: 2020 2020 6f6e 2077 6574 2064 6179 7320      on wet days 
-00007280: 2870 7229 2e22 2222 0a0a 2020 2020 7065  (pr)."""..    pe
-00007290: 7220 3d20 3735 0a20 2020 2074 6872 6573  r = 75.    thres
-000072a0: 6820 3d20 310a 2020 2020 6261 7365 5f70  h = 1.    base_p
-000072b0: 6572 696f 645f 7469 6d65 5f72 616e 6765  eriod_time_range
-000072c0: 203d 2042 4153 455f 5045 5249 4f44 0a0a   = BASE_PERIOD..
-000072d0: 2020 2020 6465 6620 636f 6d70 7574 6528      def compute(
-000072e0: 0a20 2020 2020 2020 2070 6572 3d70 6572  .        per=per
-000072f0: 2c0a 2020 2020 2020 2020 7468 7265 7368  ,.        thresh
-00007300: 3d74 6872 6573 682c 0a20 2020 2020 2020  =thresh,.       
-00007310: 2062 6173 655f 7065 7269 6f64 5f74 696d   base_period_tim
-00007320: 655f 7261 6e67 653d 6261 7365 5f70 6572  e_range=base_per
-00007330: 696f 645f 7469 6d65 5f72 616e 6765 2c0a  iod_time_range,.
-00007340: 2020 2020 2020 2020 2a2a 7061 7261 6d73          **params
-00007350: 2c0a 2020 2020 293a 0a20 2020 2020 2020  ,.    ):.       
-00007360: 2022 2222 4361 6c63 756c 6174 6520 746f   """Calculate to
-00007370: 7461 6c20 7072 6563 6970 6974 6174 696f  tal precipitatio
-00007380: 6e20 616d 6f75 6e74 2077 6974 680a 2020  n amount with.  
-00007390: 2020 2020 2020 7072 6563 6970 203e 207b        precip > {
-000073a0: 7065 7263 7d74 6820 7065 7263 656e 7469  perc}th percenti
-000073b0: 6c65 206f 6e20 7765 7420 6461 7973 2028  le on wet days (
-000073c0: 7072 203e 2074 6872 6573 6829 2e0a 0a20  pr > thresh)... 
-000073d0: 2020 2020 2020 2050 6172 616d 6574 6572         Parameter
-000073e0: 730a 2020 2020 2020 2020 2d2d 2d2d 2d2d  s.        ------
-000073f0: 2d2d 2d2d 0a20 2020 2020 2020 2070 6572  ----.        per
-00007400: 3a20 696e 740a 2020 2020 2020 2020 2020  : int.          
-00007410: 2020 5065 7263 656e 7469 6c65 2076 616c    Percentile val
-00007420: 7565 2e0a 2020 2020 2020 2020 7468 7265  ue..        thre
-00007430: 7368 3a20 696e 7420 6f72 2073 7472 696e  sh: int or strin
-00007440: 670a 2020 2020 2020 2020 2020 2020 5468  g.            Th
-00007450: 7265 7368 6f6c 6420 7072 6563 6970 6974  reshold precipit
-00007460: 6174 696f 6e20 6162 6f76 6520 7768 6963  ation above whic
-00007470: 6820 6120 6461 7920 6973 2063 6f6e 7369  h a day is consi
-00007480: 6465 7265 640a 2020 2020 2020 2020 2020  dered.          
-00007490: 2020 6173 2061 2077 6574 2064 6179 2028    as a wet day (
-000074a0: 6465 6661 756c 743a 2031 206d 6d2f 6461  default: 1 mm/da
-000074b0: 7929 2e0a 2020 2020 2020 2020 2020 2020  y)..            
-000074c0: 4966 2074 7970 6520 6f66 2074 6872 6573  If type of thres
-000074d0: 686f 6c64 2069 7320 616e 2069 6e74 6567  hold is an integ
-000074e0: 6572 2074 6865 2075 6e69 7420 6973 2073  er the unit is s
-000074f0: 6574 2074 6f20 6d6d 2f64 6179 2e0a 2020  et to mm/day..  
-00007500: 2020 2020 2020 6261 7365 5f70 6572 696f        base_perio
-00007510: 645f 7469 6d65 5f72 616e 6765 3a20 6c69  d_time_range: li
-00007520: 7374 0a20 2020 2020 2020 2020 2020 204c  st.            L
-00007530: 6973 7420 7769 7468 206c 6566 7420 626f  ist with left bo
-00007540: 756e 6420 6973 2073 7461 7274 2079 6561  und is start yea
-00007550: 7220 7374 7269 6e67 2061 6e64 2072 6967  r string and rig
-00007560: 6874 2062 6f75 6e64 0a20 2020 2020 2020  ht bound.       
-00007570: 2020 2020 2069 7320 656e 6420 7965 6172       is end year
-00007580: 2073 7472 696e 6720 666f 7220 6361 6c75   string for calu
-00007590: 6c61 7469 6e67 2074 6865 2070 7265 6369  lating the preci
-000075a0: 7020 7065 7263 656e 7469 6c65 0a20 2020  p percentile.   
-000075b0: 2020 2020 2020 2020 2072 6566 6572 656e           referen
-000075c0: 6365 2076 616c 7565 2e0a 0a20 2020 2020  ce value...     
-000075d0: 2020 2052 6574 7572 6e73 0a20 2020 2020     Returns.     
-000075e0: 2020 202d 2d2d 2d2d 2d2d 0a20 2020 2020     -------.     
-000075f0: 2020 2078 6172 7261 792e 4461 7461 4172     xarray.DataAr
-00007600: 7261 790a 2020 2020 2020 2020 2020 2020  ray.            
-00007610: 5072 6563 6970 6974 6174 696f 6e20 6672  Precipitation fr
-00007620: 6163 7469 6f6e 2077 6974 6820 7072 6563  action with prec
-00007630: 6970 203e 207b 7065 7263 7d74 6820 7065  ip > {perc}th pe
-00007640: 7263 656e 7469 6c65 0a20 2020 2020 2020  rcentile.       
-00007650: 2020 2020 206f 6e20 7765 7420 6461 7973       on wet days
-00007660: 2028 7072 203e 207b 7468 7265 7368 7d29   (pr > {thresh})
-00007670: 2e0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
-00007680: 2020 2020 2020 7468 7265 7368 203d 205f        thresh = _
-00007690: 7468 7265 7368 5f73 7472 696e 6728 7468  thresh_string(th
-000076a0: 7265 7368 2c20 226d 6d2f 6461 7922 290a  resh, "mm/day").
-000076b0: 2020 2020 2020 2020 6461 203d 205f 6765          da = _ge
-000076c0: 745f 6461 2870 6172 616d 732c 2022 7072  t_da(params, "pr
-000076d0: 2229 0a20 2020 2020 2020 2064 615f 7072  ").        da_pr
-000076e0: 203d 205f 6669 6c74 6572 5f6f 7574 5f73   = _filter_out_s
-000076f0: 6d61 6c6c 5f76 616c 7565 7328 6461 2c20  mall_values(da, 
-00007700: 7468 7265 7368 2c20 636f 6e74 6578 743d  thresh, context=
-00007710: 2268 7964 726f 2229 0a20 2020 2020 2020  "hydro").       
-00007720: 2070 725f 7065 7220 3d20 5f67 6574 5f70   pr_per = _get_p
-00007730: 6572 6365 6e74 696c 6528 0a20 2020 2020  ercentile(.     
-00007740: 2020 2020 2020 2064 613d 6461 5f70 722c         da=da_pr,
-00007750: 0a20 2020 2020 2020 2020 2020 2070 6572  .            per
-00007760: 3d70 6572 2c0a 2020 2020 2020 2020 2020  =per,.          
-00007770: 2020 6261 7365 5f70 6572 696f 645f 7469    base_period_ti
-00007780: 6d65 5f72 616e 6765 3d62 6173 655f 7065  me_range=base_pe
-00007790: 7269 6f64 5f74 696d 655f 7261 6e67 652c  riod_time_range,
-000077a0: 0a20 2020 2020 2020 2029 0a20 2020 2020  .        ).     
-000077b0: 2020 2077 6974 6820 6461 736b 2e63 6f6e     with dask.con
-000077c0: 6669 672e 7365 7428 2a2a 7b22 6172 7261  fig.set(**{"arra
-000077d0: 792e 736c 6963 696e 672e 7370 6c69 745f  y.slicing.split_
-000077e0: 6c61 7267 655f 6368 756e 6b73 223a 2046  large_chunks": F
-000077f0: 616c 7365 7d29 3a0a 2020 2020 2020 2020  alse}):.        
-00007800: 2020 2020 7072 5f70 6572 203d 2063 6f6e      pr_per = con
-00007810: 7665 7274 5f75 6e69 7473 5f74 6f28 7072  vert_units_to(pr
-00007820: 5f70 6572 2c20 6461 2c20 636f 6e74 6578  _per, da, contex
-00007830: 743d 2268 7964 726f 2229 0a20 2020 2020  t="hydro").     
-00007840: 2020 2020 2020 2074 6872 6573 6820 3d20         thresh = 
-00007850: 636f 6e76 6572 745f 756e 6974 735f 746f  convert_units_to
-00007860: 2874 6872 6573 682c 2064 612c 2063 6f6e  (thresh, da, con
-00007870: 7465 7874 3d22 6879 6472 6f22 290a 0a20  text="hydro").. 
-00007880: 2020 2020 2020 2020 2020 2074 7020 3d20             tp = 
-00007890: 7072 5f70 6572 2e77 6865 7265 2870 725f  pr_per.where(pr_
-000078a0: 7065 7220 3e20 7468 7265 7368 2c20 7468  per > thresh, th
-000078b0: 7265 7368 290a 2020 2020 2020 2020 2020  resh).          
-000078c0: 2020 6966 2022 6461 796f 6679 6561 7222    if "dayofyear"
-000078d0: 2069 6e20 7072 5f70 6572 2e63 6f6f 7264   in pr_per.coord
-000078e0: 733a 0a20 2020 2020 2020 2020 2020 2020  s:.             
-000078f0: 2020 2023 2043 7265 6174 6520 7469 6d65     # Create time
-00007900: 2073 6572 6965 7320 6f75 7420 6f66 2064   series out of d
-00007910: 6f79 2076 616c 7565 732e 0a20 2020 2020  oy values..     
-00007920: 2020 2020 2020 2020 2020 2074 7020 3d20             tp = 
-00007930: 7265 7361 6d70 6c65 5f64 6f79 2874 702c  resample_doy(tp,
-00007940: 2064 6129 0a0a 2020 2020 2020 2020 2020   da)..          
-00007950: 2020 636f 6e73 7472 6169 6e20 3d20 2822    constrain = ("
-00007960: 3e22 2c20 223e 3d22 290a 0a20 2020 2020  >", ">=")..     
-00007970: 2020 2020 2020 2023 2043 6f6d 7075 7465         # Compute
-00007980: 2074 6865 2064 6179 7320 7768 656e 2070   the days when p
-00007990: 7265 6369 7020 6973 2062 6f74 6820 6f76  recip is both ov
-000079a0: 6572 2074 6865 2077 6574 2064 6179 2074  er the wet day t
-000079b0: 6872 6573 686f 6c64 0a20 2020 2020 2020  hreshold.       
-000079c0: 2020 2020 2023 2061 6e64 2074 6865 2070       # and the p
-000079d0: 6572 6365 6e74 696c 6520 7468 7265 7368  ercentile thresh
-000079e0: 6f6c 642e 0a20 2020 2020 2020 2020 2020  old..           
-000079f0: 206f 7665 7220 3d20 280a 2020 2020 2020   over = (.      
-00007a00: 2020 2020 2020 2020 2020 6461 2e77 6865            da.whe
-00007a10: 7265 2863 6f6d 7061 7265 2864 612c 2022  re(compare(da, "
-00007a20: 3e22 2c20 7470 2c20 636f 6e73 7472 6169  >", tp, constrai
-00007a30: 6e29 290a 2020 2020 2020 2020 2020 2020  n)).            
-00007a40: 2020 2020 2e72 6573 616d 706c 6528 7469      .resample(ti
-00007a50: 6d65 3d70 6172 616d 735b 2266 7265 7122  me=params["freq"
-00007a60: 5d29 0a20 2020 2020 2020 2020 2020 2020  ]).             
-00007a70: 2020 202e 7375 6d28 6469 6d3d 2274 696d     .sum(dim="tim
-00007a80: 6522 290a 2020 2020 2020 2020 2020 2020  e").            
-00007a90: 290a 2020 2020 2020 2020 2020 2020 6f75  ).            ou
-00007aa0: 7420 3d20 636f 6e76 6572 745f 756e 6974  t = convert_unit
-00007ab0: 735f 746f 286f 7665 722c 2022 6d6d 2f64  s_to(over, "mm/d
-00007ac0: 6179 2229 0a20 2020 2020 2020 2020 2020  ay").           
-00007ad0: 206f 7574 2e61 7474 7273 5b22 756e 6974   out.attrs["unit
-00007ae0: 7322 5d20 3d20 226d 6d22 0a20 2020 2020  s"] = "mm".     
-00007af0: 2020 2020 2020 2072 6574 7572 6e20 6f75         return ou
-00007b00: 740a 0a0a 636c 6173 7320 5259 5970 544f  t...class RYYpTO
-00007b10: 543a 0a20 2020 2022 2222 5072 6563 6970  T:.    """Precip
-00007b20: 6974 6174 696f 6e20 6672 6163 7469 6f6e  itation fraction
-00007b30: 2077 6974 6820 7072 6563 6970 2061 626f   with precip abo
-00007b40: 7665 2070 6572 6365 6e74 696c 6520 6f6e  ve percentile on
-00007b50: 2077 6574 2064 6179 7320 2870 7229 2e22   wet days (pr)."
-00007b60: 2222 0a0a 2020 2020 7065 7220 3d20 3735  ""..    per = 75
-00007b70: 0a20 2020 2074 6872 6573 6820 3d20 310a  .    thresh = 1.
-00007b80: 2020 2020 6261 7365 5f70 6572 696f 645f      base_period_
-00007b90: 7469 6d65 5f72 616e 6765 203d 2042 4153  time_range = BAS
-00007ba0: 455f 5045 5249 4f44 0a0a 2020 2020 6465  E_PERIOD..    de
-00007bb0: 6620 636f 6d70 7574 6528 0a20 2020 2020  f compute(.     
-00007bc0: 2020 2070 6572 3d70 6572 2c0a 2020 2020     per=per,.    
-00007bd0: 2020 2020 7468 7265 7368 3d74 6872 6573      thresh=thres
-00007be0: 682c 0a20 2020 2020 2020 2062 6173 655f  h,.        base_
-00007bf0: 7065 7269 6f64 5f74 696d 655f 7261 6e67  period_time_rang
-00007c00: 653d 6261 7365 5f70 6572 696f 645f 7469  e=base_period_ti
-00007c10: 6d65 5f72 616e 6765 2c0a 2020 2020 2020  me_range,.      
-00007c20: 2020 2a2a 7061 7261 6d73 2c0a 2020 2020    **params,.    
-00007c30: 293a 0a20 2020 2020 2020 2022 2222 4361  ):.        """Ca
-00007c40: 6c63 756c 6174 6520 7072 6563 6970 6974  lculate precipit
-00007c50: 6174 696f 6e20 6672 6163 7469 6f6e 2077  ation fraction w
-00007c60: 6974 6820 7072 6563 6970 2061 626f 7665  ith precip above
-00007c70: 2070 6572 6365 6e74 696c 650a 2020 2020   percentile.    
-00007c80: 2020 2020 6f6e 2077 6574 2064 6179 7320      on wet days 
-00007c90: 2870 7220 3e20 7468 7265 7368 292e 0a0a  (pr > thresh)...
-00007ca0: 2020 2020 2020 2020 5061 7261 6d65 7465          Paramete
-00007cb0: 7273 0a20 2020 2020 2020 202d 2d2d 2d2d  rs.        -----
-00007cc0: 2d2d 2d2d 2d0a 2020 2020 2020 2020 7065  -----.        pe
-00007cd0: 723a 2069 6e74 0a20 2020 2020 2020 2020  r: int.         
-00007ce0: 2020 2050 6572 6365 6e74 696c 6520 7661     Percentile va
-00007cf0: 6c75 652e 0a20 2020 2020 2020 2074 6872  lue..        thr
-00007d00: 6573 683a 2069 6e74 206f 7220 7374 7269  esh: int or stri
-00007d10: 6e67 0a20 2020 2020 2020 2020 2020 2054  ng.            T
-00007d20: 6872 6573 686f 6c64 2070 7265 6369 7069  hreshold precipi
-00007d30: 7461 7469 6f6e 2061 626f 7665 2077 6869  tation above whi
-00007d40: 6368 2061 2064 6179 2069 7320 636f 6e73  ch a day is cons
-00007d50: 6964 6572 6564 0a20 2020 2020 2020 2020  idered.         
-00007d60: 2020 2061 7320 6120 7765 7420 6461 7920     as a wet day 
-00007d70: 2864 6566 6175 6c74 3a20 3120 6d6d 2f64  (default: 1 mm/d
-00007d80: 6179 292e 0a20 2020 2020 2020 2020 2020  ay)..           
-00007d90: 2049 6620 7479 7065 206f 6620 7468 7265   If type of thre
-00007da0: 7368 6f6c 6420 6973 2061 6e20 696e 7465  shold is an inte
-00007db0: 6765 7220 7468 6520 756e 6974 2069 7320  ger the unit is 
-00007dc0: 7365 7420 746f 206d 6d2f 6461 792e 0a20  set to mm/day.. 
-00007dd0: 2020 2020 2020 2062 6173 655f 7065 7269         base_peri
-00007de0: 6f64 5f74 696d 655f 7261 6e67 653a 206c  od_time_range: l
-00007df0: 6973 740a 2020 2020 2020 2020 2020 2020  ist.            
-00007e00: 4c69 7374 2077 6974 6820 6c65 6674 2062  List with left b
-00007e10: 6f75 6e64 2069 7320 7374 6172 7420 7965  ound is start ye
-00007e20: 6172 2073 7472 696e 6720 616e 6420 7269  ar string and ri
-00007e30: 6768 7420 626f 756e 640a 2020 2020 2020  ght bound.      
-00007e40: 2020 2020 2020 6973 2065 6e64 2079 6561        is end yea
-00007e50: 7220 7374 7269 6e67 2066 6f72 2063 616c  r string for cal
-00007e60: 756c 6174 696e 6720 7468 6520 7072 6563  ulating the prec
-00007e70: 6970 2070 6572 6365 6e74 696c 650a 2020  ip percentile.  
-00007e80: 2020 2020 2020 2020 2020 7265 6665 7265            refere
-00007e90: 6e63 6520 7661 6c75 652e 0a0a 2020 2020  nce value...    
-00007ea0: 2020 2020 5265 7475 726e 730a 2020 2020      Returns.    
-00007eb0: 2020 2020 2d2d 2d2d 2d2d 2d0a 2020 2020      -------.    
-00007ec0: 2020 2020 7861 7272 6179 2e44 6174 6141      xarray.DataA
-00007ed0: 7272 6179 0a20 2020 2020 2020 2020 2020  rray.           
-00007ee0: 2050 7265 6369 7069 7461 7469 6f6e 2066   Precipitation f
-00007ef0: 7261 6374 696f 6e20 7769 7468 2070 7265  raction with pre
-00007f00: 6369 7020 3e20 7b70 6572 637d 7468 2070  cip > {perc}th p
-00007f10: 6572 6365 6e74 696c 650a 2020 2020 2020  ercentile.      
-00007f20: 2020 2020 2020 6f6e 2077 6574 2064 6179        on wet day
-00007f30: 7320 2870 7220 3e20 7b74 6872 6573 687d  s (pr > {thresh}
-00007f40: 292e 0a0a 2020 2020 2020 2020 4e6f 7465  )...        Note
-00007f50: 730a 2020 2020 2020 2020 2d2d 2d2d 2d0a  s.        -----.
-00007f60: 2020 2020 2020 2020 466f 7220 6d6f 7265          For more
-00007f70: 2069 6e66 6f72 6d61 7469 6f6e 206f 6e20   information on 
-00007f80: 7468 6520 696e 7075 7420 7061 7261 6d65  the input parame
-00007f90: 7465 7273 2073 6565 3a0a 2020 2020 2020  ters see:.      
-00007fa0: 2020 2020 2020 6874 7470 733a 2f2f 7863        https://xc
-00007fb0: 6c69 6d2e 7265 6164 7468 6564 6f63 732e  lim.readthedocs.
-00007fc0: 696f 2f65 6e2f 7374 6162 6c65 2f61 7069  io/en/stable/api
-00007fd0: 2e68 746d 6c23 7863 6c69 6d2e 696e 6469  .html#xclim.indi
-00007fe0: 6361 746f 7273 2e61 746d 6f73 2e66 7261  cators.atmos.fra
-00007ff0: 6374 696f 6e5f 6f76 6572 5f70 7265 6369  ction_over_preci
-00008000: 705f 7468 7265 7368 0a20 2020 2020 2020  p_thresh.       
-00008010: 2022 2222 0a20 2020 2020 2020 2074 6872   """.        thr
-00008020: 6573 6820 3d20 5f74 6872 6573 685f 7374  esh = _thresh_st
-00008030: 7269 6e67 2874 6872 6573 682c 2022 6d6d  ring(thresh, "mm
-00008040: 2f64 6179 2229 0a20 2020 2020 2020 2064  /day").        d
-00008050: 6120 3d20 5f67 6574 5f64 6128 7061 7261  a = _get_da(para
-00008060: 6d73 2c20 2270 7222 290a 2020 2020 2020  ms, "pr").      
-00008070: 2020 6461 5f70 7220 3d20 5f66 696c 7465    da_pr = _filte
-00008080: 725f 6f75 745f 736d 616c 6c5f 7661 6c75  r_out_small_valu
-00008090: 6573 2864 612c 2074 6872 6573 682c 2063  es(da, thresh, c
-000080a0: 6f6e 7465 7874 3d22 6879 6472 6f22 290a  ontext="hydro").
-000080b0: 2020 2020 2020 2020 7072 5f70 6572 203d          pr_per =
-000080c0: 205f 6765 745f 7065 7263 656e 7469 6c65   _get_percentile
-000080d0: 280a 2020 2020 2020 2020 2020 2020 6461  (.            da
-000080e0: 3d64 615f 7072 2c0a 2020 2020 2020 2020  =da_pr,.        
-000080f0: 2020 2020 7065 723d 7065 722c 0a20 2020      per=per,.   
-00008100: 2020 2020 2020 2020 2062 6173 655f 7065           base_pe
-00008110: 7269 6f64 5f74 696d 655f 7261 6e67 653d  riod_time_range=
-00008120: 6261 7365 5f70 6572 696f 645f 7469 6d65  base_period_time
-00008130: 5f72 616e 6765 2c0a 2020 2020 2020 2020  _range,.        
-00008140: 290a 2020 2020 2020 2020 7769 7468 2064  ).        with d
-00008150: 6173 6b2e 636f 6e66 6967 2e73 6574 282a  ask.config.set(*
-00008160: 2a7b 2261 7272 6179 2e73 6c69 6369 6e67  *{"array.slicing
-00008170: 2e73 706c 6974 5f6c 6172 6765 5f63 6875  .split_large_chu
-00008180: 6e6b 7322 3a20 4661 6c73 657d 293a 0a20  nks": False}):. 
-00008190: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-000081a0: 6e20 7863 2e61 746d 6f73 2e66 7261 6374  n xc.atmos.fract
-000081b0: 696f 6e5f 6f76 6572 5f70 7265 6369 705f  ion_over_precip_
-000081c0: 7468 7265 7368 280a 2020 2020 2020 2020  thresh(.        
-000081d0: 2020 2020 2020 2020 7072 5f70 6572 3d70          pr_per=p
-000081e0: 725f 7065 722c 0a20 2020 2020 2020 2020  r_per,.         
-000081f0: 2020 2020 2020 202a 2a70 6172 616d 732c         **params,
-00008200: 0a20 2020 2020 2020 2020 2020 2029 0a0a  .            )..
-00008210: 0a63 6c61 7373 2053 4449 493a 0a20 2020  .class SDII:.   
-00008220: 2022 2222 4176 6572 6167 6520 7072 6563   """Average prec
-00008230: 6970 6974 6174 696f 6e20 6475 7269 6e67  ipitation during
-00008240: 2077 6574 2064 6179 7320 2870 7229 2e22   wet days (pr)."
-00008250: 2222 0a0a 2020 2020 7468 7265 7368 203d  ""..    thresh =
-00008260: 2031 0a0a 2020 2020 6465 6620 636f 6d70   1..    def comp
-00008270: 7574 6528 7468 7265 7368 3d74 6872 6573  ute(thresh=thres
-00008280: 682c 202a 2a70 6172 616d 7329 3a0a 2020  h, **params):.  
-00008290: 2020 2020 2020 2222 2243 616c 6375 6c61        """Calcula
-000082a0: 7465 2061 7665 7261 6765 2070 7265 6369  te average preci
-000082b0: 7069 7461 7469 6f6e 2064 7572 696e 6720  pitation during 
-000082c0: 7765 7420 6461 7973 2e0a 0a20 2020 2020  wet days...     
-000082d0: 2020 2050 6172 616d 6574 6572 730a 2020     Parameters.  
-000082e0: 2020 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d        ----------
-000082f0: 0a20 2020 2020 2020 2074 6872 6573 683a  .        thresh:
-00008300: 2069 6e74 206f 7220 7374 7269 6e67 0a20   int or string. 
-00008310: 2020 2020 2020 2020 2020 2054 6872 6573             Thres
-00008320: 686f 6c64 2070 7265 6369 7069 7461 7469  hold precipitati
-00008330: 6f6e 2061 626f 7665 2077 6869 6368 2061  on above which a
-00008340: 2064 6179 2069 7320 636f 6e73 6964 6572   day is consider
-00008350: 6564 0a20 2020 2020 2020 2020 2020 2061  ed.            a
-00008360: 7320 6120 7765 7420 6461 7920 2864 6566  s a wet day (def
-00008370: 6175 6c74 3a20 3120 6d6d 2f64 6179 292e  ault: 1 mm/day).
-00008380: 0a20 2020 2020 2020 2020 2020 2049 6620  .            If 
-00008390: 7479 7065 206f 6620 7468 7265 7368 6f6c  type of threshol
-000083a0: 6420 6973 2061 6e20 696e 7465 6765 7220  d is an integer 
-000083b0: 7468 6520 756e 6974 2069 7320 7365 7420  the unit is set 
-000083c0: 746f 206d 6d2f 6461 792e 0a0a 2020 2020  to mm/day...    
-000083d0: 2020 2020 5265 7475 726e 730a 2020 2020      Returns.    
-000083e0: 2020 2020 2d2d 2d2d 2d2d 2d0a 2020 2020      -------.    
-000083f0: 2020 2020 7861 7272 6179 2e44 6174 6141      xarray.DataA
-00008400: 7272 6179 0a20 2020 2020 2020 2020 2020  rray.           
-00008410: 2041 7665 7261 6765 2070 7265 6369 7069   Average precipi
-00008420: 7461 7469 6f6e 2064 7572 696e 6720 7765  tation during we
-00008430: 7420 6461 7973 2e0a 0a20 2020 2020 2020  t days...       
-00008440: 204e 6f74 6573 0a20 2020 2020 2020 202d   Notes.        -
-00008450: 2d2d 2d2d 0a20 2020 2020 2020 2046 6f72  ----.        For
-00008460: 206d 6f72 6520 696e 666f 726d 6174 696f   more informatio
-00008470: 6e20 6f6e 2074 6865 2069 6e70 7574 2070  n on the input p
-00008480: 6172 616d 6574 6572 7320 7365 653a 0a20  arameters see:. 
-00008490: 2020 2020 2020 2020 2020 2068 7474 7073             https
-000084a0: 3a2f 2f78 636c 696d 2e72 6561 6474 6865  ://xclim.readthe
-000084b0: 646f 6373 2e69 6f2f 656e 2f73 7461 626c  docs.io/en/stabl
-000084c0: 652f 6170 692e 6874 6d6c 2378 636c 696d  e/api.html#xclim
-000084d0: 2e69 6e64 6963 6174 6f72 732e 6174 6d6f  .indicators.atmo
-000084e0: 732e 6461 696c 795f 7072 5f69 6e74 656e  s.daily_pr_inten
-000084f0: 7369 7479 0a20 2020 2020 2020 2022 2222  sity.        """
-00008500: 0a20 2020 2020 2020 2074 6872 6573 6820  .        thresh 
-00008510: 3d20 5f74 6872 6573 685f 7374 7269 6e67  = _thresh_string
-00008520: 2831 2c20 226d 6d2f 6461 7922 290a 2020  (1, "mm/day").  
-00008530: 2020 2020 2020 7265 7475 726e 2078 632e        return xc.
-00008540: 6174 6d6f 732e 6461 696c 795f 7072 5f69  atmos.daily_pr_i
-00008550: 6e74 656e 7369 7479 280a 2020 2020 2020  ntensity(.      
-00008560: 2020 2020 2020 7468 7265 7368 3d74 6872        thresh=thr
-00008570: 6573 682c 0a20 2020 2020 2020 2020 2020  esh,.           
-00008580: 202a 2a70 6172 616d 732c 0a20 2020 2020   **params,.     
-00008590: 2020 2029 0a0a 0a63 6c61 7373 2053 553a     )...class SU:
-000085a0: 0a20 2020 2022 2222 4e75 6d62 6572 206f  .    """Number o
-000085b0: 6620 7375 6d6d 6572 2064 6179 7320 2874  f summer days (t
-000085c0: 6173 6d61 7829 2e22 2222 0a0a 2020 2020  asmax)."""..    
-000085d0: 7468 7265 7368 203d 2032 350a 0a20 2020  thresh = 25..   
-000085e0: 2064 6566 2063 6f6d 7075 7465 2874 6872   def compute(thr
-000085f0: 6573 683d 7468 7265 7368 2c20 2a2a 7061  esh=thresh, **pa
-00008600: 7261 6d73 293a 0a20 2020 2020 2020 2022  rams):.        "
-00008610: 2222 4361 6c63 756c 6174 6520 6e75 6d62  ""Calculate numb
-00008620: 6572 206f 6620 7375 6d6d 6572 2064 6179  er of summer day
-00008630: 732e 0a0a 2020 2020 2020 2020 5061 7261  s...        Para
-00008640: 6d65 7465 7273 0a20 2020 2020 2020 202d  meters.        -
-00008650: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 2020  ---------.      
-00008660: 2020 7468 7265 7368 3a20 696e 7420 6f72    thresh: int or
-00008670: 2073 7472 696e 670a 2020 2020 2020 2020   string.        
-00008680: 2020 2020 5468 7265 7368 6f6c 6420 6d61      Threshold ma
-00008690: 7869 6d75 6d20 7465 6d70 6572 6174 7572  ximum temperatur
-000086a0: 6520 6162 6f76 6520 7768 6963 6820 746f  e above which to
-000086b0: 2064 6179 2069 7320 636f 6e73 6964 6572   day is consider
-000086c0: 6564 0a20 2020 2020 2020 2020 2020 2061  ed.            a
-000086d0: 7320 6120 7375 6d6d 6572 2064 6179 2028  s a summer day (
-000086e0: 6465 6661 756c 743a 2032 3520 6465 6743  default: 25 degC
-000086f0: 292e 0a20 2020 2020 2020 2020 2020 2049  )..            I
-00008700: 6620 7479 7065 206f 6620 7468 7265 7368  f type of thresh
-00008710: 6f6c 6420 6973 2061 6e20 696e 7465 6765  old is an intege
-00008720: 7220 7468 6520 756e 6974 2069 7320 7365  r the unit is se
-00008730: 7420 746f 2064 6567 432e 0a0a 2020 2020  t to degC...    
-00008740: 2020 2020 5265 7475 726e 730a 2020 2020      Returns.    
-00008750: 2020 2020 2d2d 2d2d 2d2d 2d0a 2020 2020      -------.    
-00008760: 2020 2020 7861 7272 6179 2e44 6174 6141      xarray.DataA
-00008770: 7272 6179 0a20 2020 2020 2020 2020 2020  rray.           
-00008780: 204e 756d 6265 7220 6f66 2073 756d 6d65   Number of summe
-00008790: 7220 6461 7973 2028 7478 203e 207b 7468  r days (tx > {th
-000087a0: 7265 7368 7d29 2e0a 0a20 2020 2020 2020  resh})...       
-000087b0: 204e 6f74 6573 0a20 2020 2020 2020 202d   Notes.        -
-000087c0: 2d2d 2d2d 0a20 2020 2020 2020 2046 6f72  ----.        For
-000087d0: 206d 6f72 6520 696e 666f 726d 6174 696f   more informatio
-000087e0: 6e20 6f6e 2074 6865 2069 6e70 7574 2070  n on the input p
-000087f0: 6172 616d 6574 6572 7320 7365 653a 0a20  arameters see:. 
-00008800: 2020 2020 2020 2020 2020 2068 7474 7073             https
-00008810: 3a2f 2f78 636c 696d 2e72 6561 6474 6865  ://xclim.readthe
-00008820: 646f 6373 2e69 6f2f 656e 2f73 7461 626c  docs.io/en/stabl
-00008830: 652f 6170 692e 6874 6d6c 2378 636c 696d  e/api.html#xclim
-00008840: 2e69 6e64 6963 6174 6f72 732e 6174 6d6f  .indicators.atmo
-00008850: 732e 7478 5f64 6179 735f 6162 6f76 650a  s.tx_days_above.
-00008860: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00008870: 2020 2020 7468 7265 7368 203d 205f 7468      thresh = _th
-00008880: 7265 7368 5f73 7472 696e 6728 7468 7265  resh_string(thre
-00008890: 7368 2c20 2264 6567 4322 290a 2020 2020  sh, "degC").    
-000088a0: 2020 2020 7265 7475 726e 2078 632e 6174      return xc.at
-000088b0: 6d6f 732e 7478 5f64 6179 735f 6162 6f76  mos.tx_days_abov
-000088c0: 6528 0a20 2020 2020 2020 2020 2020 2074  e(.            t
-000088d0: 6872 6573 683d 7468 7265 7368 2c0a 2020  hresh=thresh,.  
-000088e0: 2020 2020 2020 2020 2020 2a2a 7061 7261            **para
-000088f0: 6d73 2c0a 2020 2020 2020 2020 290a 0a0a  ms,.        )...
-00008900: 636c 6173 7320 5351 493a 0a20 2020 2022  class SQI:.    "
-00008910: 2222 4e75 6d62 6572 206f 6620 756e 636f  ""Number of unco
-00008920: 6d66 6f72 7461 626c 6520 736c 6565 7020  mfortable sleep 
-00008930: 6576 656e 7473 2028 7461 736d 696e 292e  events (tasmin).
-00008940: 2222 220a 0a20 2020 2074 6872 6573 6820  """..    thresh 
-00008950: 3d20 3138 0a0a 2020 2020 6465 6620 636f  = 18..    def co
-00008960: 6d70 7574 6528 7468 7265 7368 3d74 6872  mpute(thresh=thr
-00008970: 6573 682c 202a 2a70 6172 616d 7329 3a0a  esh, **params):.
-00008980: 2020 2020 2020 2020 2222 2243 616c 6375          """Calcu
-00008990: 6c61 7465 206e 756d 6265 7220 6f66 2075  late number of u
-000089a0: 6e63 6f6d 666f 7274 6162 6c65 2073 6c65  ncomfortable sle
-000089b0: 6570 2065 7665 6e74 732e 0a0a 2020 2020  ep events...    
-000089c0: 2020 2020 5061 7261 6d65 7465 7273 0a20      Parameters. 
-000089d0: 2020 2020 2020 202d 2d2d 2d2d 2d2d 2d2d         ---------
-000089e0: 2d0a 2020 2020 2020 2020 7468 7265 7368  -.        thresh
-000089f0: 3a20 696e 7420 6f72 2073 7472 696e 670a  : int or string.
-00008a00: 2020 2020 2020 2020 2020 2020 5468 7265              Thre
-00008a10: 7368 6f6c 6420 6d69 6e69 6d75 6d20 7465  shold minimum te
-00008a20: 6d70 6572 6174 7572 6520 6265 6c6f 7720  mperature below 
-00008a30: 7768 6963 6820 6120 6461 7920 6861 730a  which a day has.
-00008a40: 2020 2020 2020 2020 2020 2020 6120 756e              a un
-00008a50: 636f 6d66 6f72 7461 626c 6520 736c 6565  comfortable slee
-00008a60: 7020 6576 656e 7420 2864 6566 6175 6c74  p event (default
-00008a70: 3a20 3138 2064 6567 4329 2e0a 2020 2020  : 18 degC)..    
-00008a80: 2020 2020 2020 2020 4966 2074 7970 6520          If type 
-00008a90: 6f66 2074 6872 6573 686f 6c64 2069 7320  of threshold is 
-00008aa0: 616e 2069 6e74 6567 6572 2074 6865 2075  an integer the u
-00008ab0: 6e69 7420 6973 2073 6574 2074 6f20 6465  nit is set to de
-00008ac0: 6743 2e0a 0a20 2020 2020 2020 2052 6574  gC...        Ret
-00008ad0: 7572 6e73 0a20 2020 2020 2020 202d 2d2d  urns.        ---
-00008ae0: 2d2d 2d2d 0a20 2020 2020 2020 2078 6172  ----.        xar
-00008af0: 7261 792e 4461 7461 4172 7261 790a 2020  ray.DataArray.  
-00008b00: 2020 2020 2020 2020 2020 4e75 6d62 6572            Number
-00008b10: 206f 6620 756e 636f 6d66 6f72 7461 626c   of uncomfortabl
-00008b20: 6520 736c 6565 7020 6576 656e 7473 2028  e sleep events (
-00008b30: 746e 203c 207b 7468 7265 7368 7d29 2e0a  tn < {thresh})..
-00008b40: 0a20 2020 2020 2020 204e 6f74 6573 0a20  .        Notes. 
-00008b50: 2020 2020 2020 202d 2d2d 2d2d 0a20 2020         -----.   
-00008b60: 2020 2020 2046 6f72 206d 6f72 6520 696e       For more in
-00008b70: 666f 726d 6174 696f 6e20 6f6e 2074 6865  formation on the
-00008b80: 2069 6e70 7574 2070 6172 616d 6574 6572   input parameter
-00008b90: 7320 7365 653a 0a20 2020 2020 2020 2020  s see:.         
-00008ba0: 2020 2068 7474 7073 3a2f 2f78 636c 696d     https://xclim
-00008bb0: 2e72 6561 6474 6865 646f 6373 2e69 6f2f  .readthedocs.io/
-00008bc0: 656e 2f73 7461 626c 652f 6170 692e 6874  en/stable/api.ht
-00008bd0: 6d6c 2378 636c 696d 2e69 6e64 6963 6174  ml#xclim.indicat
-00008be0: 6f72 732e 6174 6d6f 732e 746e 5f64 6179  ors.atmos.tn_day
-00008bf0: 735f 6162 6f76 650a 2020 2020 2020 2020  s_above.        
-00008c00: 2222 220a 2020 2020 2020 2020 7468 7265  """.        thre
-00008c10: 7368 203d 205f 7468 7265 7368 5f73 7472  sh = _thresh_str
-00008c20: 696e 6728 7468 7265 7368 2c20 2264 6567  ing(thresh, "deg
-00008c30: 4322 290a 2020 2020 2020 2020 7265 7475  C").        retu
-00008c40: 726e 2078 632e 6174 6d6f 732e 746e 5f64  rn xc.atmos.tn_d
-00008c50: 6179 735f 6162 6f76 6528 0a20 2020 2020  ays_above(.     
-00008c60: 2020 2020 2020 2074 6872 6573 683d 7468         thresh=th
-00008c70: 7265 7368 2c0a 2020 2020 2020 2020 2020  resh,.          
-00008c80: 2020 2a2a 7061 7261 6d73 2c0a 2020 2020    **params,.    
-00008c90: 2020 2020 290a 0a0a 636c 6173 7320 5447      )...class TG
-00008ca0: 3a0a 2020 2020 2222 224d 6561 6e20 6d65  :.    """Mean me
-00008cb0: 616e 2074 656d 7065 7261 7475 7265 2028  an temperature (
-00008cc0: 7461 7329 2e22 2222 0a0a 2020 2020 6465  tas)."""..    de
-00008cd0: 6620 636f 6d70 7574 6528 2a2a 7061 7261  f compute(**para
-00008ce0: 6d73 293a 0a20 2020 2020 2020 2022 2222  ms):.        """
-00008cf0: 4361 6c63 756c 6174 6520 6d65 616e 2064  Calculate mean d
-00008d00: 6169 6c79 206d 6561 6e20 7465 6d70 6572  aily mean temper
-00008d10: 6174 7572 652e 0a0a 2020 2020 2020 2020  ature...        
-00008d20: 5265 7475 726e 730a 2020 2020 2020 2020  Returns.        
-00008d30: 2d2d 2d2d 2d2d 2d0a 2020 2020 2020 2020  -------.        
-00008d40: 7861 7272 6179 2e44 6174 6141 7272 6179  xarray.DataArray
-00008d50: 0a20 2020 2020 2020 2020 2020 204d 6561  .            Mea
-00008d60: 6e20 6461 696c 7920 6d65 616e 2074 656d  n daily mean tem
-00008d70: 7065 7261 7475 7265 2e0a 0a20 2020 2020  perature...     
-00008d80: 2020 204e 6f74 6573 0a20 2020 2020 2020     Notes.       
-00008d90: 202d 2d2d 2d2d 0a20 2020 2020 2020 2046   -----.        F
-00008da0: 6f72 2069 6e66 6f72 6d61 7469 6f6e 206f  or information o
-00008db0: 6e20 7468 6520 696e 7075 7420 7061 7261  n the input para
-00008dc0: 6d65 7465 7273 2073 6565 3a0a 2020 2020  meters see:.    
-00008dd0: 2020 2020 2020 2020 6874 7470 733a 2f2f          https://
-00008de0: 7863 6c69 6d2e 7265 6164 7468 6564 6f63  xclim.readthedoc
-00008df0: 732e 696f 2f65 6e2f 7374 6162 6c65 2f61  s.io/en/stable/a
-00008e00: 7069 2e68 746d 6c23 7863 6c69 6d2e 696e  pi.html#xclim.in
-00008e10: 6469 6361 746f 7273 2e61 746d 6f73 2e74  dicators.atmos.t
-00008e20: 675f 6d65 616e 0a20 2020 2020 2020 2022  g_mean.        "
-00008e30: 2222 0a20 2020 2020 2020 2072 6574 7572  "".        retur
-00008e40: 6e20 7863 2e61 746d 6f73 2e74 675f 6d65  n xc.atmos.tg_me
-00008e50: 616e 282a 2a70 6172 616d 7329 0a0a 0a63  an(**params)...c
-00008e60: 6c61 7373 2054 4731 3070 3a0a 2020 2020  lass TG10p:.    
-00008e70: 2222 2246 7261 6374 696f 6e20 6f66 2064  """Fraction of d
-00008e80: 6179 7320 7769 7468 206d 6561 6e20 7465  ays with mean te
-00008e90: 6d70 6572 6174 7572 6520 3c20 3130 7468  mperature < 10th
-00008ea0: 2070 6572 6365 6e74 696c 6520 2874 6173   percentile (tas
-00008eb0: 292e 2222 220a 0a20 2020 2074 6173 5f70  )."""..    tas_p
-00008ec0: 6572 203d 204e 6f6e 650a 2020 2020 6261  er = None.    ba
-00008ed0: 7365 5f70 6572 696f 645f 7469 6d65 5f72  se_period_time_r
-00008ee0: 616e 6765 203d 2042 4153 455f 5045 5249  ange = BASE_PERI
-00008ef0: 4f44 0a0a 2020 2020 6465 6620 636f 6d70  OD..    def comp
-00008f00: 7574 6528 0a20 2020 2020 2020 2062 6173  ute(.        bas
-00008f10: 655f 7065 7269 6f64 5f74 696d 655f 7261  e_period_time_ra
-00008f20: 6e67 653d 6261 7365 5f70 6572 696f 645f  nge=base_period_
-00008f30: 7469 6d65 5f72 616e 6765 2c0a 2020 2020  time_range,.    
-00008f40: 2020 2020 7461 735f 7065 723d 7461 735f      tas_per=tas_
-00008f50: 7065 722c 0a20 2020 2020 2020 202a 2a70  per,.        **p
-00008f60: 6172 616d 732c 0a20 2020 2029 3a0a 2020  arams,.    ):.  
-00008f70: 2020 2020 2020 2222 2243 616c 6375 6c61        """Calcula
-00008f80: 7465 2066 7261 6374 696f 6e20 6f66 2064  te fraction of d
-00008f90: 6179 7320 7769 7468 206d 6561 6e20 7465  ays with mean te
-00008fa0: 6d70 6572 6174 7572 6520 3c20 3130 7468  mperature < 10th
-00008fb0: 2070 6572 6365 6e74 696c 652e 0a0a 2020   percentile...  
-00008fc0: 2020 2020 2020 5061 7261 6d65 7465 7273        Parameters
-00008fd0: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
-00008fe0: 2d2d 2d0a 2020 2020 2020 2020 7461 735f  ---.        tas_
-00008ff0: 7065 723a 2078 722e 4461 7461 4172 7261  per: xr.DataArra
-00009000: 792c 206f 7074 696f 6e61 6c0a 2020 2020  y, optional.    
-00009010: 2020 2020 2020 2020 5465 6d70 6572 6174          Temperat
-00009020: 7572 6520 3130 7468 2070 6572 6365 6e74  ure 10th percent
-00009030: 696c 6520 7265 6665 7265 6e63 6520 7661  ile reference va
-00009040: 6c75 652e 0a20 2020 2020 2020 2062 6173  lue..        bas
-00009050: 655f 7065 7269 6f64 5f74 696d 655f 7261  e_period_time_ra
-00009060: 6e67 653a 206c 6973 740a 2020 2020 2020  nge: list.      
-00009070: 2020 2020 2020 4c69 7374 2077 6974 6820        List with 
-00009080: 6c65 6674 2062 6f75 6e64 2069 7320 7374  left bound is st
-00009090: 6172 7420 7965 6172 2073 7472 696e 6720  art year string 
-000090a0: 616e 6420 7269 6768 7420 626f 756e 6420  and right bound 
-000090b0: 6973 0a20 2020 2020 2020 2020 2020 2065  is.            e
-000090c0: 6e64 2079 6561 7220 7374 7269 6e67 2066  nd year string f
-000090d0: 6f72 2063 616c 6375 6c61 7469 6e67 2060  or calculating `
-000090e0: 7461 735f 7065 7260 2e0a 2020 2020 2020  tas_per`..      
-000090f0: 2020 2020 2020 5468 6973 2077 696c 6c20        This will 
-00009100: 6265 2075 7365 6420 6f6e 6c79 2069 6620  be used only if 
-00009110: 6074 6173 5f70 6572 6020 6973 204e 6f6e  `tas_per` is Non
-00009120: 652e 0a0a 2020 2020 2020 2020 5265 7475  e...        Retu
-00009130: 726e 730a 2020 2020 2020 2020 2d2d 2d2d  rns.        ----
-00009140: 2d2d 2d0a 2020 2020 2020 2020 7861 7272  ---.        xarr
-00009150: 6179 2e44 6174 6141 7272 6179 0a20 2020  ay.DataArray.   
-00009160: 2020 2020 2020 2020 2046 7261 6374 696f           Fractio
-00009170: 6e20 6f66 2064 6179 7320 7769 7468 206d  n of days with m
-00009180: 6561 6e20 7465 6d70 6572 6174 7572 6520  ean temperature 
-00009190: 3c20 3130 7468 2070 6572 6365 6e74 696c  < 10th percentil
-000091a0: 6522 2e0a 0a20 2020 2020 2020 204e 6f74  e"...        Not
-000091b0: 6573 0a20 2020 2020 2020 202d 2d2d 2d2d  es.        -----
-000091c0: 0a20 2020 2020 2020 2046 6f72 206d 6f72  .        For mor
-000091d0: 6520 696e 666f 726d 6174 696f 6e20 6f6e  e information on
-000091e0: 2074 6865 2069 6e70 7574 2070 6172 616d   the input param
-000091f0: 6574 6572 7320 7365 653a 0a20 2020 2020  eters see:.     
-00009200: 2020 2020 2020 2068 7474 7073 3a2f 2f78         https://x
-00009210: 636c 696d 2e72 6561 6474 6865 646f 6373  clim.readthedocs
-00009220: 2e69 6f2f 656e 2f73 7461 626c 652f 6170  .io/en/stable/ap
-00009230: 692e 6874 6d6c 2378 636c 696d 2e69 6e64  i.html#xclim.ind
-00009240: 6963 6174 6f72 732e 6174 6d6f 732e 7467  icators.atmos.tg
-00009250: 3130 700a 2020 2020 2020 2020 2222 220a  10p.        """.
-00009260: 2020 2020 2020 2020 6461 203d 205f 6765          da = _ge
-00009270: 745f 6461 2870 6172 616d 732c 2022 7461  t_da(params, "ta
-00009280: 7322 290a 2020 2020 2020 2020 6966 2074  s").        if t
-00009290: 6173 5f70 6572 2069 7320 4e6f 6e65 3a0a  as_per is None:.
-000092a0: 2020 2020 2020 2020 2020 2020 7461 735f              tas_
-000092b0: 7065 7220 3d20 5f67 6574 5f70 6572 6365  per = _get_perce
-000092c0: 6e74 696c 6528 0a20 2020 2020 2020 2020  ntile(.         
-000092d0: 2020 2020 2020 2064 613d 6461 2c0a 2020         da=da,.  
-000092e0: 2020 2020 2020 2020 2020 2020 2020 7065                pe
-000092f0: 723d 3130 2c0a 2020 2020 2020 2020 2020  r=10,.          
-00009300: 2020 2020 2020 6261 7365 5f70 6572 696f        base_perio
-00009310: 645f 7469 6d65 5f72 616e 6765 3d62 6173  d_time_range=bas
-00009320: 655f 7065 7269 6f64 5f74 696d 655f 7261  e_period_time_ra
-00009330: 6e67 652c 0a20 2020 2020 2020 2020 2020  nge,.           
-00009340: 2029 0a20 2020 2020 2020 2077 6974 6820   ).        with 
-00009350: 6461 736b 2e63 6f6e 6669 672e 7365 7428  dask.config.set(
-00009360: 2a2a 7b22 6172 7261 792e 736c 6963 696e  **{"array.slicin
-00009370: 672e 7370 6c69 745f 6c61 7267 655f 6368  g.split_large_ch
-00009380: 756e 6b73 223a 2046 616c 7365 7d29 3a0a  unks": False}):.
-00009390: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-000093a0: 726e 2078 632e 6174 6d6f 732e 7467 3130  rn xc.atmos.tg10
-000093b0: 7028 0a20 2020 2020 2020 2020 2020 2020  p(.             
-000093c0: 2020 2074 6173 5f70 6572 3d74 6173 5f70     tas_per=tas_p
-000093d0: 6572 2c0a 2020 2020 2020 2020 2020 2020  er,.            
-000093e0: 2020 2020 2a2a 7061 7261 6d73 2c0a 2020      **params,.  
-000093f0: 2020 2020 2020 2020 2020 290a 0a0a 636c            )...cl
-00009400: 6173 7320 5447 3930 703a 0a20 2020 2022  ass TG90p:.    "
-00009410: 2222 4672 6163 7469 6f6e 206f 6620 6461  ""Fraction of da
-00009420: 7973 2077 6974 6820 6d65 616e 2074 656d  ys with mean tem
-00009430: 7065 7261 7475 7265 203e 2039 3074 6820  perature > 90th 
-00009440: 7065 7263 656e 7469 6c65 2028 7461 7329  percentile (tas)
-00009450: 2e22 2222 0a0a 2020 2020 7461 735f 7065  ."""..    tas_pe
-00009460: 7220 3d20 4e6f 6e65 0a20 2020 2062 6173  r = None.    bas
-00009470: 655f 7065 7269 6f64 5f74 696d 655f 7261  e_period_time_ra
-00009480: 6e67 6520 3d20 4241 5345 5f50 4552 494f  nge = BASE_PERIO
-00009490: 440a 0a20 2020 2064 6566 2063 6f6d 7075  D..    def compu
-000094a0: 7465 280a 2020 2020 2020 2020 6261 7365  te(.        base
-000094b0: 5f70 6572 696f 645f 7469 6d65 5f72 616e  _period_time_ran
-000094c0: 6765 3d62 6173 655f 7065 7269 6f64 5f74  ge=base_period_t
-000094d0: 696d 655f 7261 6e67 652c 0a20 2020 2020  ime_range,.     
-000094e0: 2020 2074 6173 5f70 6572 3d74 6173 5f70     tas_per=tas_p
-000094f0: 6572 2c0a 2020 2020 2020 2020 2a2a 7061  er,.        **pa
-00009500: 7261 6d73 2c0a 2020 2020 293a 0a20 2020  rams,.    ):.   
-00009510: 2020 2020 2022 2222 4361 6c63 756c 6174       """Calculat
-00009520: 6520 6672 6163 7469 6f6e 206f 6620 6461  e fraction of da
-00009530: 7973 2077 6974 6820 6d65 616e 2074 656d  ys with mean tem
-00009540: 7065 7261 7475 7265 203e 2039 3074 6820  perature > 90th 
-00009550: 7065 7263 656e 7469 6c65 222e 0a0a 2020  percentile"...  
-00009560: 2020 2020 2020 5061 7261 6d65 7465 7273        Parameters
-00009570: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
-00009580: 2d2d 2d0a 2020 2020 2020 2020 7461 735f  ---.        tas_
-00009590: 7065 723a 2078 722e 4461 7461 4172 7261  per: xr.DataArra
-000095a0: 792c 206f 7074 696f 6e61 6c0a 2020 2020  y, optional.    
-000095b0: 2020 2020 2020 2020 5465 6d70 6572 6174          Temperat
-000095c0: 7572 6520 3930 7468 2070 6572 6365 6e74  ure 90th percent
-000095d0: 696c 6520 7265 6665 7265 6e63 6520 7661  ile reference va
-000095e0: 6c75 652e 0a20 2020 2020 2020 2062 6173  lue..        bas
-000095f0: 655f 7065 7269 6f64 5f74 696d 655f 7261  e_period_time_ra
-00009600: 6e67 653a 206c 6973 740a 2020 2020 2020  nge: list.      
-00009610: 2020 2020 2020 4c69 7374 2077 6974 6820        List with 
-00009620: 6c65 6674 2062 6f75 6e64 2069 7320 7374  left bound is st
-00009630: 6172 7420 7965 6172 2073 7472 696e 6720  art year string 
-00009640: 616e 6420 7269 6768 7420 626f 756e 640a  and right bound.
-00009650: 2020 2020 2020 2020 2020 2020 6973 2065              is e
-00009660: 6e64 2079 6561 7220 7374 7269 6e67 2066  nd year string f
-00009670: 6f72 2063 616c 6375 6c61 7469 6e67 2060  or calculating `
-00009680: 7461 735f 7065 7260 2e0a 2020 2020 2020  tas_per`..      
-00009690: 2020 2020 2020 5468 6973 2077 696c 6c20        This will 
-000096a0: 6265 2075 7365 6420 6f6e 6c79 2069 6620  be used only if 
-000096b0: 6074 6173 5f70 6572 6020 6973 204e 6f6e  `tas_per` is Non
-000096c0: 652e 0a0a 2020 2020 2020 2020 5265 7475  e...        Retu
-000096d0: 726e 730a 2020 2020 2020 2020 2d2d 2d2d  rns.        ----
-000096e0: 2d2d 2d0a 2020 2020 2020 2020 7861 7272  ---.        xarr
-000096f0: 6179 2e44 6174 6141 7272 6179 0a20 2020  ay.DataArray.   
-00009700: 2020 2020 2020 2020 2046 7261 6374 696f           Fractio
-00009710: 6e20 6f66 2064 6179 7320 7769 7468 206d  n of days with m
-00009720: 6561 6e20 7465 6d70 6572 6174 7572 6520  ean temperature 
-00009730: 3e20 3930 7468 2070 6572 6365 6e74 696c  > 90th percentil
-00009740: 6522 2e0a 0a20 2020 2020 2020 204e 6f74  e"...        Not
-00009750: 6573 0a20 2020 2020 2020 202d 2d2d 2d2d  es.        -----
-00009760: 0a20 2020 2020 2020 2046 6f72 206d 6f72  .        For mor
-00009770: 6520 696e 666f 726d 6174 696f 6e20 6f6e  e information on
-00009780: 2074 6865 2069 6e70 7574 2070 6172 616d   the input param
-00009790: 6574 6572 7320 7365 653a 0a20 2020 2020  eters see:.     
-000097a0: 2020 2020 2020 2068 7474 7073 3a2f 2f78         https://x
-000097b0: 636c 696d 2e72 6561 6474 6865 646f 6373  clim.readthedocs
-000097c0: 2e69 6f2f 656e 2f73 7461 626c 652f 6170  .io/en/stable/ap
-000097d0: 692e 6874 6d6c 2378 636c 696d 2e69 6e64  i.html#xclim.ind
-000097e0: 6963 6174 6f72 732e 6174 6d6f 732e 7467  icators.atmos.tg
-000097f0: 3930 700a 2020 2020 2020 2020 2222 220a  90p.        """.
-00009800: 2020 2020 2020 2020 6461 203d 205f 6765          da = _ge
-00009810: 745f 6461 2870 6172 616d 732c 2022 7461  t_da(params, "ta
-00009820: 7322 290a 2020 2020 2020 2020 6966 2074  s").        if t
-00009830: 6173 5f70 6572 2069 7320 4e6f 6e65 3a0a  as_per is None:.
-00009840: 2020 2020 2020 2020 2020 2020 7461 735f              tas_
-00009850: 7065 7220 3d20 5f67 6574 5f70 6572 6365  per = _get_perce
-00009860: 6e74 696c 6528 0a20 2020 2020 2020 2020  ntile(.         
-00009870: 2020 2020 2020 2064 613d 6461 2c0a 2020         da=da,.  
-00009880: 2020 2020 2020 2020 2020 2020 2020 7065                pe
-00009890: 723d 3930 2c0a 2020 2020 2020 2020 2020  r=90,.          
-000098a0: 2020 2020 2020 6261 7365 5f70 6572 696f        base_perio
-000098b0: 645f 7469 6d65 5f72 616e 6765 3d62 6173  d_time_range=bas
-000098c0: 655f 7065 7269 6f64 5f74 696d 655f 7261  e_period_time_ra
-000098d0: 6e67 652c 0a20 2020 2020 2020 2020 2020  nge,.           
-000098e0: 2029 0a20 2020 2020 2020 2077 6974 6820   ).        with 
-000098f0: 6461 736b 2e63 6f6e 6669 672e 7365 7428  dask.config.set(
-00009900: 2a2a 7b22 6172 7261 792e 736c 6963 696e  **{"array.slicin
-00009910: 672e 7370 6c69 745f 6c61 7267 655f 6368  g.split_large_ch
-00009920: 756e 6b73 223a 2046 616c 7365 7d29 3a0a  unks": False}):.
-00009930: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00009940: 726e 2078 632e 6174 6d6f 732e 7467 3930  rn xc.atmos.tg90
-00009950: 7028 0a20 2020 2020 2020 2020 2020 2020  p(.             
-00009960: 2020 2074 6173 5f70 6572 3d74 6173 5f70     tas_per=tas_p
-00009970: 6572 2c0a 2020 2020 2020 2020 2020 2020  er,.            
-00009980: 2020 2020 2a2a 7061 7261 6d73 2c0a 2020      **params,.  
-00009990: 2020 2020 2020 2020 2020 290a 0a0a 636c            )...cl
-000099a0: 6173 7320 5452 3a0a 2020 2020 2222 224e  ass TR:.    """N
-000099b0: 756d 6265 7220 6f66 2074 726f 7069 6361  umber of tropica
-000099c0: 6c20 6e69 6768 7473 2028 7461 736d 696e  l nights (tasmin
-000099d0: 292e 2222 220a 0a20 2020 2074 6872 6573  )."""..    thres
-000099e0: 6820 3d20 3230 0a0a 2020 2020 6465 6620  h = 20..    def 
-000099f0: 636f 6d70 7574 6528 7468 7265 7368 3d74  compute(thresh=t
-00009a00: 6872 6573 682c 202a 2a70 6172 616d 7329  hresh, **params)
-00009a10: 3a0a 2020 2020 2020 2020 2222 2243 616c  :.        """Cal
-00009a20: 6375 6c61 7465 206e 756d 6265 7220 6f66  culate number of
-00009a30: 2074 726f 7069 6361 6c20 6e69 6768 7473   tropical nights
-00009a40: 2e0a 0a20 2020 2020 2020 2050 6172 616d  ...        Param
-00009a50: 6574 6572 730a 2020 2020 2020 2020 2d2d  eters.        --
-00009a60: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020 2020  --------.       
-00009a70: 2074 6872 6573 683a 2069 6e74 206f 7220   thresh: int or 
-00009a80: 7374 7269 6e67 0a20 2020 2020 2020 2020  string.         
-00009a90: 2020 2054 6872 6573 686f 6c64 206d 696e     Threshold min
-00009aa0: 696d 756d 2074 656d 7065 7261 7475 7265  imum temperature
-00009ab0: 206f 6e20 7768 6963 6820 6120 6461 790a   on which a day.
-00009ac0: 2020 2020 2020 2020 2020 2020 6861 7320              has 
-00009ad0: 6120 7472 6f70 6963 616c 206e 6967 6874  a tropical night
-00009ae0: 2028 6465 6661 756c 743a 2032 3020 6465   (default: 20 de
-00009af0: 6743 292e 0a20 2020 2020 2020 2020 2020  gC)..           
-00009b00: 2049 6620 7479 7065 206f 6620 7468 7265   If type of thre
-00009b10: 7368 6f6c 6420 6973 2061 6e20 696e 7465  shold is an inte
-00009b20: 6765 7220 7468 6520 756e 6974 2069 7320  ger the unit is 
-00009b30: 7365 7420 746f 2064 6567 432e 0a0a 2020  set to degC...  
-00009b40: 2020 2020 2020 5265 7475 726e 730a 2020        Returns.  
-00009b50: 2020 2020 2020 2d2d 2d2d 2d2d 2d0a 2020        -------.  
-00009b60: 2020 2020 2020 7861 7272 6179 2e44 6174        xarray.Dat
-00009b70: 6141 7272 6179 0a20 2020 2020 2020 2020  aArray.         
-00009b80: 2020 204e 756d 6265 7220 6f66 2074 726f     Number of tro
-00009b90: 7069 6361 6c20 6e69 6768 7473 2028 746e  pical nights (tn
-00009ba0: 203e 207b 7468 7265 7368 7d2e 0a0a 2020   > {thresh}...  
-00009bb0: 2020 2020 2020 4e6f 7465 730a 2020 2020        Notes.    
-00009bc0: 2020 2020 2d2d 2d2d 2d0a 2020 2020 2020      -----.      
-00009bd0: 2020 466f 7220 6d6f 7265 2069 6e66 6f72    For more infor
-00009be0: 6d61 7469 6f6e 206f 6e20 7468 6520 696e  mation on the in
-00009bf0: 7075 7420 7061 7261 6d65 7465 7273 2073  put parameters s
-00009c00: 6565 3a0a 2020 2020 2020 2020 2020 2020  ee:.            
-00009c10: 6874 7470 733a 2f2f 7863 6c69 6d2e 7265  https://xclim.re
-00009c20: 6164 7468 6564 6f63 732e 696f 2f65 6e2f  adthedocs.io/en/
-00009c30: 7374 6162 6c65 2f61 7069 2e68 746d 6c23  stable/api.html#
-00009c40: 7863 6c69 6d2e 696e 6469 6361 746f 7273  xclim.indicators
-00009c50: 2e61 746d 6f73 2e74 6e5f 6461 7973 5f61  .atmos.tn_days_a
-00009c60: 626f 7665 0a20 2020 2020 2020 2022 2222  bove.        """
-00009c70: 0a20 2020 2020 2020 2074 6872 6573 6820  .        thresh 
-00009c80: 3d20 5f74 6872 6573 685f 7374 7269 6e67  = _thresh_string
-00009c90: 2874 6872 6573 682c 2022 6465 6743 2229  (thresh, "degC")
-00009ca0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00009cb0: 7863 2e61 746d 6f73 2e74 6e5f 6461 7973  xc.atmos.tn_days
-00009cc0: 5f61 626f 7665 280a 2020 2020 2020 2020  _above(.        
-00009cd0: 2020 2020 7468 7265 7368 3d74 6872 6573      thresh=thres
-00009ce0: 682c 0a20 2020 2020 2020 2020 2020 202a  h,.            *
-00009cf0: 2a70 6172 616d 732c 0a20 2020 2020 2020  *params,.       
-00009d00: 2029 0a0a 0a63 6c61 7373 2054 583a 0a20   )...class TX:. 
-00009d10: 2020 2022 2222 4d65 616e 206d 6178 696d     """Mean maxim
-00009d20: 756d 2074 656d 7065 7261 7475 7265 2028  um temperature (
-00009d30: 7461 736d 6178 292e 2222 220a 0a20 2020  tasmax)."""..   
-00009d40: 2064 6566 2063 6f6d 7075 7465 282a 2a70   def compute(**p
-00009d50: 6172 616d 7329 3a0a 2020 2020 2020 2020  arams):.        
-00009d60: 2222 2243 616c 6375 6c61 7465 206d 6561  """Calculate mea
-00009d70: 6e20 6461 696c 7920 6d61 7869 6d75 6d20  n daily maximum 
-00009d80: 7465 6d70 6572 6174 7572 652e 0a0a 2020  temperature...  
-00009d90: 2020 2020 2020 5265 7475 726e 730a 2020        Returns.  
-00009da0: 2020 2020 2020 2d2d 2d2d 2d2d 2d0a 2020        -------.  
-00009db0: 2020 2020 2020 7861 7272 6179 2e44 6174        xarray.Dat
-00009dc0: 6141 7272 6179 0a20 2020 2020 2020 2020  aArray.         
-00009dd0: 2020 204d 6561 6e20 6461 696c 7920 6d61     Mean daily ma
-00009de0: 7869 6d75 6d20 7465 6d70 6572 6174 7572  ximum temperatur
-00009df0: 652e 0a0a 2020 2020 2020 2020 4e6f 7465  e...        Note
-00009e00: 730a 2020 2020 2020 2020 2d2d 2d2d 2d0a  s.        -----.
-00009e10: 2020 2020 2020 2020 466f 7220 696e 666f          For info
-00009e20: 726d 6174 696f 6e20 6f6e 2074 6865 2069  rmation on the i
-00009e30: 6e70 7574 2070 6172 616d 6574 6572 7320  nput parameters 
-00009e40: 7365 653a 0a20 2020 2020 2020 2020 2020  see:.           
-00009e50: 2068 7474 7073 3a2f 2f78 636c 696d 2e72   https://xclim.r
-00009e60: 6561 6474 6865 646f 6373 2e69 6f2f 656e  eadthedocs.io/en
-00009e70: 2f73 7461 626c 652f 6170 692e 6874 6d6c  /stable/api.html
-00009e80: 2378 636c 696d 2e69 6e64 6963 6174 6f72  #xclim.indicator
-00009e90: 732e 6174 6d6f 732e 7478 5f6d 6561 6e0a  s.atmos.tx_mean.
-00009ea0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00009eb0: 2020 2020 7265 7475 726e 2078 632e 6174      return xc.at
-00009ec0: 6d6f 732e 7478 5f6d 6561 6e28 2a2a 7061  mos.tx_mean(**pa
-00009ed0: 7261 6d73 290a 0a0a 636c 6173 7320 5458  rams)...class TX
-00009ee0: 3130 703a 0a20 2020 2022 2222 4672 6163  10p:.    """Frac
-00009ef0: 7469 6f6e 206f 6620 6461 7973 2077 6974  tion of days wit
-00009f00: 6820 6d61 7820 7465 6d70 6572 6174 7572  h max temperatur
-00009f10: 6520 3c20 3130 7468 2070 6572 6365 6e74  e < 10th percent
-00009f20: 696c 6520 2874 6173 6d61 7829 2e22 2222  ile (tasmax)."""
-00009f30: 0a0a 2020 2020 7461 736d 6178 5f70 6572  ..    tasmax_per
-00009f40: 203d 204e 6f6e 650a 2020 2020 6261 7365   = None.    base
-00009f50: 5f70 6572 696f 645f 7469 6d65 5f72 616e  _period_time_ran
-00009f60: 6765 203d 2042 4153 455f 5045 5249 4f44  ge = BASE_PERIOD
-00009f70: 0a0a 2020 2020 6465 6620 636f 6d70 7574  ..    def comput
-00009f80: 6528 0a20 2020 2020 2020 2062 6173 655f  e(.        base_
-00009f90: 7065 7269 6f64 5f74 696d 655f 7261 6e67  period_time_rang
-00009fa0: 653d 6261 7365 5f70 6572 696f 645f 7469  e=base_period_ti
-00009fb0: 6d65 5f72 616e 6765 2c0a 2020 2020 2020  me_range,.      
-00009fc0: 2020 7461 736d 6178 5f70 6572 3d74 6173    tasmax_per=tas
-00009fd0: 6d61 785f 7065 722c 0a20 2020 2020 2020  max_per,.       
-00009fe0: 202a 2a70 6172 616d 732c 0a20 2020 2029   **params,.    )
-00009ff0: 3a0a 2020 2020 2020 2020 2222 2243 616c  :.        """Cal
-0000a000: 6375 6c61 7465 2066 7261 6374 696f 6e20  culate fraction 
-0000a010: 6f66 2064 6179 7320 7769 7468 206d 6178  of days with max
-0000a020: 2074 656d 7065 7261 7475 7265 203c 2031   temperature < 1
-0000a030: 3074 6820 7065 7263 656e 7469 6c65 2e0a  0th percentile..
-0000a040: 0a20 2020 2020 2020 2050 6172 616d 6574  .        Paramet
-0000a050: 6572 730a 2020 2020 2020 2020 2d2d 2d2d  ers.        ----
-0000a060: 2d2d 2d2d 2d2d 0a20 2020 2020 2020 2074  ------.        t
-0000a070: 6173 6d61 785f 7065 723a 2078 722e 4461  asmax_per: xr.Da
-0000a080: 7461 4172 7261 792c 206f 7074 696f 6e61  taArray, optiona
-0000a090: 6c0a 2020 2020 2020 2020 2020 2020 4d61  l.            Ma
-0000a0a0: 7869 6d75 6d20 7465 6d70 6572 6174 7572  ximum temperatur
-0000a0b0: 6520 3130 7468 2070 6572 6365 6e74 696c  e 10th percentil
-0000a0c0: 6520 7265 6665 7265 6e63 6520 7661 6c75  e reference valu
-0000a0d0: 652e 0a20 2020 2020 2020 2062 6173 655f  e..        base_
-0000a0e0: 7065 7269 6f64 5f74 696d 655f 7261 6e67  period_time_rang
-0000a0f0: 653a 206c 6973 740a 2020 2020 2020 2020  e: list.        
-0000a100: 2020 2020 4c69 7374 2077 6974 6820 6c65      List with le
-0000a110: 6674 2062 6f75 6e64 2069 7320 7374 6172  ft bound is star
-0000a120: 7420 7965 6172 2073 7472 696e 6720 616e  t year string an
-0000a130: 6420 7269 6768 7420 626f 756e 640a 2020  d right bound.  
-0000a140: 2020 2020 2020 2020 2020 6973 2065 6e64            is end
-0000a150: 2079 6561 7220 7374 7269 6e67 2066 6f72   year string for
-0000a160: 2063 616c 6375 6c61 7469 6e67 2060 7461   calculating `ta
-0000a170: 736d 6178 5f70 6572 602e 0a20 2020 2020  smax_per`..     
-0000a180: 2020 2020 2020 2054 6869 7320 7769 6c6c         This will
-0000a190: 2062 6520 7573 6564 206f 6e6c 7920 6966   be used only if
-0000a1a0: 2060 7461 736d 6178 5f70 6572 6020 6973   `tasmax_per` is
-0000a1b0: 204e 6f6e 652e 0a0a 2020 2020 2020 2020   None...        
-0000a1c0: 5265 7475 726e 730a 2020 2020 2020 2020  Returns.        
-0000a1d0: 2d2d 2d2d 2d2d 2d0a 2020 2020 2020 2020  -------.        
-0000a1e0: 7861 7272 6179 2e44 6174 6141 7272 6179  xarray.DataArray
-0000a1f0: 0a20 2020 2020 2020 2020 2020 2046 7261  .            Fra
-0000a200: 6374 696f 6e20 6f66 2064 6179 7320 7769  ction of days wi
-0000a210: 7468 206d 6178 696d 756d 2074 656d 7065  th maximum tempe
-0000a220: 7261 7475 7265 203c 2031 3074 6820 7065  rature < 10th pe
-0000a230: 7263 656e 7469 6c65 222e 0a0a 2020 2020  rcentile"...    
-0000a240: 2020 2020 4e6f 7465 730a 2020 2020 2020      Notes.      
-0000a250: 2020 2d2d 2d2d 2d0a 2020 2020 2020 2020    -----.        
-0000a260: 466f 7220 6d6f 7265 2069 6e66 6f72 6d61  For more informa
-0000a270: 7469 6f6e 206f 6e20 7468 6520 696e 7075  tion on the inpu
-0000a280: 7420 7061 7261 6d65 7465 7273 2073 6565  t parameters see
-0000a290: 3a0a 2020 2020 2020 2020 2020 2020 6874  :.            ht
-0000a2a0: 7470 733a 2f2f 7863 6c69 6d2e 7265 6164  tps://xclim.read
-0000a2b0: 7468 6564 6f63 732e 696f 2f65 6e2f 7374  thedocs.io/en/st
-0000a2c0: 6162 6c65 2f61 7069 2e68 746d 6c23 7863  able/api.html#xc
-0000a2d0: 6c69 6d2e 696e 6469 6361 746f 7273 2e61  lim.indicators.a
-0000a2e0: 746d 6f73 2e74 7831 3070 0a20 2020 2020  tmos.tx10p.     
-0000a2f0: 2020 2022 2222 0a20 2020 2020 2020 2064     """.        d
-0000a300: 6120 3d20 5f67 6574 5f64 6128 7061 7261  a = _get_da(para
-0000a310: 6d73 2c20 2274 6173 6d61 7822 290a 2020  ms, "tasmax").  
-0000a320: 2020 2020 2020 6966 2074 6173 6d61 785f        if tasmax_
-0000a330: 7065 7220 6973 204e 6f6e 653a 0a20 2020  per is None:.   
-0000a340: 2020 2020 2020 2020 2074 6173 6d61 785f           tasmax_
-0000a350: 7065 7220 3d20 5f67 6574 5f70 6572 6365  per = _get_perce
-0000a360: 6e74 696c 6528 0a20 2020 2020 2020 2020  ntile(.         
-0000a370: 2020 2020 2020 2064 613d 6461 2c0a 2020         da=da,.  
-0000a380: 2020 2020 2020 2020 2020 2020 2020 7065                pe
-0000a390: 723d 3130 2c0a 2020 2020 2020 2020 2020  r=10,.          
-0000a3a0: 2020 2020 2020 6261 7365 5f70 6572 696f        base_perio
-0000a3b0: 645f 7469 6d65 5f72 616e 6765 3d62 6173  d_time_range=bas
-0000a3c0: 655f 7065 7269 6f64 5f74 696d 655f 7261  e_period_time_ra
-0000a3d0: 6e67 652c 0a20 2020 2020 2020 2020 2020  nge,.           
-0000a3e0: 2029 0a20 2020 2020 2020 2077 6974 6820   ).        with 
-0000a3f0: 6461 736b 2e63 6f6e 6669 672e 7365 7428  dask.config.set(
-0000a400: 2a2a 7b22 6172 7261 792e 736c 6963 696e  **{"array.slicin
-0000a410: 672e 7370 6c69 745f 6c61 7267 655f 6368  g.split_large_ch
-0000a420: 756e 6b73 223a 2046 616c 7365 7d29 3a0a  unks": False}):.
-0000a430: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-0000a440: 726e 2078 632e 6174 6d6f 732e 7478 3130  rn xc.atmos.tx10
-0000a450: 7028 0a20 2020 2020 2020 2020 2020 2020  p(.             
-0000a460: 2020 2074 6173 6d61 785f 7065 723d 7461     tasmax_per=ta
-0000a470: 736d 6178 5f70 6572 2c0a 2020 2020 2020  smax_per,.      
-0000a480: 2020 2020 2020 2020 2020 2a2a 7061 7261            **para
-0000a490: 6d73 2c0a 2020 2020 2020 2020 2020 2020  ms,.            
-0000a4a0: 290a 0a0a 636c 6173 7320 5458 3930 703a  )...class TX90p:
-0000a4b0: 0a20 2020 2022 2222 4672 6163 7469 6f6e  .    """Fraction
-0000a4c0: 206f 6620 6461 7973 2077 6974 6820 6d61   of days with ma
-0000a4d0: 7820 7465 6d70 6572 6174 7572 6520 3e20  x temperature > 
-0000a4e0: 3930 7468 2070 6572 6365 6e74 696c 6520  90th percentile 
-0000a4f0: 2874 6173 6d61 7829 2e22 2222 0a0a 2020  (tasmax)."""..  
-0000a500: 2020 7461 736d 6178 5f70 6572 203d 204e    tasmax_per = N
-0000a510: 6f6e 650a 2020 2020 6261 7365 5f70 6572  one.    base_per
-0000a520: 696f 645f 7469 6d65 5f72 616e 6765 203d  iod_time_range =
-0000a530: 2042 4153 455f 5045 5249 4f44 0a0a 2020   BASE_PERIOD..  
-0000a540: 2020 6465 6620 636f 6d70 7574 6528 0a20    def compute(. 
-0000a550: 2020 2020 2020 2062 6173 655f 7065 7269         base_peri
-0000a560: 6f64 5f74 696d 655f 7261 6e67 653d 6261  od_time_range=ba
-0000a570: 7365 5f70 6572 696f 645f 7469 6d65 5f72  se_period_time_r
-0000a580: 616e 6765 2c0a 2020 2020 2020 2020 7461  ange,.        ta
-0000a590: 736d 6178 5f70 6572 3d74 6173 6d61 785f  smax_per=tasmax_
-0000a5a0: 7065 722c 0a20 2020 2020 2020 202a 2a70  per,.        **p
-0000a5b0: 6172 616d 732c 0a20 2020 2029 3a0a 2020  arams,.    ):.  
-0000a5c0: 2020 2020 2020 2222 2243 616c 6375 6c61        """Calcula
-0000a5d0: 7465 2066 7261 6374 696f 6e20 6f66 2064  te fraction of d
-0000a5e0: 6179 7320 7769 7468 206d 6178 2074 656d  ays with max tem
-0000a5f0: 7065 7261 7475 7265 203e 2039 3074 6820  perature > 90th 
-0000a600: 7065 7263 656e 7469 6c65 2e0a 0a20 2020  percentile...   
-0000a610: 2020 2020 2050 6172 616d 6574 6572 730a       Parameters.
-0000a620: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d2d          --------
-0000a630: 2d2d 0a20 2020 2020 2020 2074 6173 6d61  --.        tasma
-0000a640: 785f 7065 723a 2078 722e 4461 7461 4172  x_per: xr.DataAr
-0000a650: 7261 792c 206f 7074 696f 6e61 6c0a 2020  ray, optional.  
-0000a660: 2020 2020 2020 2020 2020 4d61 7869 6d75            Maximu
-0000a670: 6d20 7465 6d70 6572 6174 7572 6520 3930  m temperature 90
-0000a680: 7468 2070 6572 6365 6e74 696c 6520 7265  th percentile re
-0000a690: 6665 7265 6e63 6520 7661 6c75 652e 0a20  ference value.. 
-0000a6a0: 2020 2020 2020 2062 6173 655f 7065 7269         base_peri
-0000a6b0: 6f64 5f74 696d 655f 7261 6e67 653a 206c  od_time_range: l
-0000a6c0: 6973 740a 2020 2020 2020 2020 2020 2020  ist.            
-0000a6d0: 4c69 7374 2077 6974 6820 6c65 6674 2062  List with left b
-0000a6e0: 6f75 6e64 2069 7320 7374 6172 7420 7965  ound is start ye
-0000a6f0: 6172 2073 7472 696e 6720 616e 6420 7269  ar string and ri
-0000a700: 6768 7420 626f 756e 640a 2020 2020 2020  ght bound.      
-0000a710: 2020 2020 2020 6973 2065 6e64 2079 6561        is end yea
-0000a720: 7220 7374 7269 6e67 2066 6f72 2063 616c  r string for cal
-0000a730: 6375 6c61 7469 6e67 2060 7461 736d 6178  culating `tasmax
-0000a740: 5f70 6572 602e 0a20 2020 2020 2020 2020  _per`..         
-0000a750: 2020 2054 6869 7320 7769 6c6c 2062 6520     This will be 
-0000a760: 7573 6564 206f 6e6c 7920 6966 2060 7461  used only if `ta
-0000a770: 736d 6178 5f70 6572 6020 6973 204e 6f6e  smax_per` is Non
-0000a780: 652e 0a0a 2020 2020 2020 2020 5265 7475  e...        Retu
-0000a790: 726e 730a 2020 2020 2020 2020 2d2d 2d2d  rns.        ----
-0000a7a0: 2d2d 2d0a 2020 2020 2020 2020 7861 7272  ---.        xarr
-0000a7b0: 6179 2e44 6174 6141 7272 6179 0a20 2020  ay.DataArray.   
-0000a7c0: 2020 2020 2020 2020 2046 7261 6374 696f           Fractio
-0000a7d0: 6e20 6f66 2064 6179 7320 7769 7468 206d  n of days with m
-0000a7e0: 6178 696d 756d 2074 656d 7065 7261 7475  aximum temperatu
-0000a7f0: 7265 203e 2039 3074 6820 7065 7263 656e  re > 90th percen
-0000a800: 7469 6c65 222e 0a0a 2020 2020 2020 2020  tile"...        
-0000a810: 4e6f 7465 730a 2020 2020 2020 2020 2d2d  Notes.        --
-0000a820: 2d2d 2d0a 2020 2020 2020 2020 466f 7220  ---.        For 
-0000a830: 6d6f 7265 2069 6e66 6f72 6d61 7469 6f6e  more information
-0000a840: 206f 6e20 7468 6520 696e 7075 7420 7061   on the input pa
-0000a850: 7261 6d65 7465 7273 2073 6565 3a0a 2020  rameters see:.  
-0000a860: 2020 2020 2020 2020 2020 6874 7470 733a            https:
-0000a870: 2f2f 7863 6c69 6d2e 7265 6164 7468 6564  //xclim.readthed
-0000a880: 6f63 732e 696f 2f65 6e2f 7374 6162 6c65  ocs.io/en/stable
-0000a890: 2f61 7069 2e68 746d 6c23 7863 6c69 6d2e  /api.html#xclim.
-0000a8a0: 696e 6469 6361 746f 7273 2e61 746d 6f73  indicators.atmos
-0000a8b0: 2e74 7839 3070 0a20 2020 2020 2020 2022  .tx90p.        "
-0000a8c0: 2222 0a20 2020 2020 2020 2064 6120 3d20  "".        da = 
-0000a8d0: 5f67 6574 5f64 6128 7061 7261 6d73 2c20  _get_da(params, 
-0000a8e0: 2274 6173 6d61 7822 290a 2020 2020 2020  "tasmax").      
-0000a8f0: 2020 6966 2074 6173 6d61 785f 7065 7220    if tasmax_per 
-0000a900: 6973 204e 6f6e 653a 0a20 2020 2020 2020  is None:.       
-0000a910: 2020 2020 2074 6173 6d61 785f 7065 7220       tasmax_per 
-0000a920: 3d20 5f67 6574 5f70 6572 6365 6e74 696c  = _get_percentil
-0000a930: 6528 0a20 2020 2020 2020 2020 2020 2020  e(.             
-0000a940: 2020 2064 613d 6461 2c0a 2020 2020 2020     da=da,.      
-0000a950: 2020 2020 2020 2020 2020 7065 723d 3930            per=90
-0000a960: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0000a970: 2020 6261 7365 5f70 6572 696f 645f 7469    base_period_ti
-0000a980: 6d65 5f72 616e 6765 3d62 6173 655f 7065  me_range=base_pe
-0000a990: 7269 6f64 5f74 696d 655f 7261 6e67 652c  riod_time_range,
-0000a9a0: 0a20 2020 2020 2020 2020 2020 2029 0a20  .            ). 
-0000a9b0: 2020 2020 2020 2077 6974 6820 6461 736b         with dask
-0000a9c0: 2e63 6f6e 6669 672e 7365 7428 2a2a 7b22  .config.set(**{"
-0000a9d0: 6172 7261 792e 736c 6963 696e 672e 7370  array.slicing.sp
-0000a9e0: 6c69 745f 6c61 7267 655f 6368 756e 6b73  lit_large_chunks
-0000a9f0: 223a 2046 616c 7365 7d29 3a0a 2020 2020  ": False}):.    
-0000aa00: 2020 2020 2020 2020 7265 7475 726e 2078          return x
-0000aa10: 632e 6174 6d6f 732e 7478 3930 7028 0a20  c.atmos.tx90p(. 
-0000aa20: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-0000aa30: 6173 6d61 785f 7065 723d 7461 736d 6178  asmax_per=tasmax
-0000aa40: 5f70 6572 2c0a 2020 2020 2020 2020 2020  _per,.          
-0000aa50: 2020 2020 2020 2a2a 7061 7261 6d73 2c0a        **params,.
-0000aa60: 2020 2020 2020 2020 2020 2020 290a 0a0a              )...
-0000aa70: 636c 6173 7320 5458 6e3a 0a20 2020 2022  class TXn:.    "
-0000aa80: 2222 4d69 6e69 6d75 6d20 6d61 7869 6d75  ""Minimum maximu
-0000aa90: 6d20 7465 6d70 6572 6174 7572 6520 2874  m temperature (t
-0000aaa0: 6173 6d61 7829 2e22 2222 0a0a 2020 2020  asmax)."""..    
-0000aab0: 6465 6620 636f 6d70 7574 6528 2a2a 7061  def compute(**pa
-0000aac0: 7261 6d73 293a 0a20 2020 2020 2020 2022  rams):.        "
-0000aad0: 2222 4361 6c63 756c 6174 6520 6d69 6e69  ""Calculate mini
-0000aae0: 6d75 6d20 6461 696c 7920 6d61 7869 6d75  mum daily maximu
-0000aaf0: 6d20 7465 6d70 6572 6174 7572 652e 0a0a  m temperature...
-0000ab00: 2020 2020 2020 2020 5265 7475 726e 730a          Returns.
-0000ab10: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d0a          -------.
-0000ab20: 2020 2020 2020 2020 7861 7272 6179 2e44          xarray.D
-0000ab30: 6174 6141 7272 6179 0a20 2020 2020 2020  ataArray.       
-0000ab40: 2020 2020 204d 696e 696d 756d 2064 6169       Minimum dai
-0000ab50: 6c79 206d 6178 696d 756d 2074 656d 7065  ly maximum tempe
-0000ab60: 7261 7475 7265 2e0a 0a20 2020 2020 2020  rature...       
-0000ab70: 204e 6f74 6573 0a20 2020 2020 2020 202d   Notes.        -
-0000ab80: 2d2d 2d2d 0a20 2020 2020 2020 2046 6f72  ----.        For
-0000ab90: 2069 6e66 6f72 6d61 7469 6f6e 206f 6e20   information on 
-0000aba0: 7468 6520 696e 7075 7420 7061 7261 6d65  the input parame
-0000abb0: 7465 7273 2073 6565 3a0a 2020 2020 2020  ters see:.      
-0000abc0: 2020 2020 2020 6874 7470 733a 2f2f 7863        https://xc
-0000abd0: 6c69 6d2e 7265 6164 7468 6564 6f63 732e  lim.readthedocs.
-0000abe0: 696f 2f65 6e2f 7374 6162 6c65 2f61 7069  io/en/stable/api
-0000abf0: 2e68 746d 6c23 7863 6c69 6d2e 696e 6469  .html#xclim.indi
-0000ac00: 6361 746f 7273 2e61 746d 6f73 2e74 785f  cators.atmos.tx_
-0000ac10: 6d69 6e0a 2020 2020 2020 2020 2222 220a  min.        """.
-0000ac20: 2020 2020 2020 2020 7265 7475 726e 2078          return x
-0000ac30: 632e 6174 6d6f 732e 7478 5f6d 696e 282a  c.atmos.tx_min(*
-0000ac40: 2a70 6172 616d 7329 0a0a 0a63 6c61 7373  *params)...class
-0000ac50: 2054 5878 3a0a 2020 2020 2222 224d 6178   TXx:.    """Max
-0000ac60: 696d 756d 206d 6178 696d 756d 2074 656d  imum maximum tem
-0000ac70: 7065 7261 7475 7265 2028 7461 736d 6178  perature (tasmax
-0000ac80: 292e 2222 220a 0a20 2020 2064 6566 2063  )."""..    def c
-0000ac90: 6f6d 7075 7465 282a 2a70 6172 616d 7329  ompute(**params)
-0000aca0: 3a0a 2020 2020 2020 2020 2222 2243 616c  :.        """Cal
-0000acb0: 6375 6c61 7465 206d 6178 696d 756d 2064  culate maximum d
-0000acc0: 6169 6c79 206d 6178 696d 756d 2074 656d  aily maximum tem
-0000acd0: 7065 7261 7475 7265 2e0a 0a20 2020 2020  perature...     
-0000ace0: 2020 2052 6574 7572 6e73 0a20 2020 2020     Returns.     
-0000acf0: 2020 202d 2d2d 2d2d 2d2d 0a20 2020 2020     -------.     
-0000ad00: 2020 2078 6172 7261 792e 4461 7461 4172     xarray.DataAr
-0000ad10: 7261 790a 2020 2020 2020 2020 2020 2020  ray.            
-0000ad20: 4d61 7869 6d75 6d20 6461 696c 7920 6d61  Maximum daily ma
-0000ad30: 7869 6d75 6d20 7465 6d70 6572 6174 7572  ximum temperatur
-0000ad40: 652e 0a0a 2020 2020 2020 2020 4e6f 7465  e...        Note
-0000ad50: 730a 2020 2020 2020 2020 2d2d 2d2d 2d0a  s.        -----.
-0000ad60: 2020 2020 2020 2020 466f 7220 696e 666f          For info
-0000ad70: 726d 6174 696f 6e20 6f6e 2074 6865 2069  rmation on the i
-0000ad80: 6e70 7574 2070 6172 616d 6574 6572 7320  nput parameters 
-0000ad90: 7365 653a 0a20 2020 2020 2020 2020 2020  see:.           
-0000ada0: 2068 7474 7073 3a2f 2f78 636c 696d 2e72   https://xclim.r
-0000adb0: 6561 6474 6865 646f 6373 2e69 6f2f 656e  eadthedocs.io/en
-0000adc0: 2f73 7461 626c 652f 6170 692e 6874 6d6c  /stable/api.html
-0000add0: 2378 636c 696d 2e69 6e64 6963 6174 6f72  #xclim.indicator
-0000ade0: 732e 6174 6d6f 732e 7478 5f6d 6178 0a20  s.atmos.tx_max. 
-0000adf0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-0000ae00: 2020 2072 6574 7572 6e20 7863 2e61 746d     return xc.atm
-0000ae10: 6f73 2e74 785f 6d61 7828 2a2a 7061 7261  os.tx_max(**para
-0000ae20: 6d73 290a 0a0a 636c 6173 7320 544e 3a0a  ms)...class TN:.
-0000ae30: 2020 2020 2222 224d 6561 6e20 6d69 6e69      """Mean mini
-0000ae40: 6d75 6d20 7465 6d70 6572 6174 7572 6520  mum temperature 
-0000ae50: 2874 6173 6d69 6e29 2e22 2222 0a0a 2020  (tasmin)."""..  
-0000ae60: 2020 6465 6620 636f 6d70 7574 6528 2a2a    def compute(**
-0000ae70: 7061 7261 6d73 293a 0a20 2020 2020 2020  params):.       
-0000ae80: 2022 2222 4361 6c63 756c 6174 6520 6d65   """Calculate me
-0000ae90: 616e 2064 6169 6c79 206d 696e 696d 756d  an daily minimum
-0000aea0: 2074 656d 7065 7261 7475 7265 2e0a 0a20   temperature... 
-0000aeb0: 2020 2020 2020 2052 6574 7572 6e73 0a20         Returns. 
-0000aec0: 2020 2020 2020 202d 2d2d 2d2d 2d2d 0a20         -------. 
-0000aed0: 2020 2020 2020 2078 6172 7261 792e 4461         xarray.Da
-0000aee0: 7461 4172 7261 790a 2020 2020 2020 2020  taArray.        
-0000aef0: 2020 2020 4d65 616e 2064 6169 6c79 206d      Mean daily m
-0000af00: 696e 696d 756d 2074 656d 7065 7261 7475  inimum temperatu
-0000af10: 7265 2e0a 0a20 2020 2020 2020 204e 6f74  re...        Not
-0000af20: 6573 0a20 2020 2020 2020 202d 2d2d 2d2d  es.        -----
-0000af30: 0a20 2020 2020 2020 2046 6f72 2069 6e66  .        For inf
-0000af40: 6f72 6d61 7469 6f6e 206f 6e20 7468 6520  ormation on the 
-0000af50: 696e 7075 7420 7061 7261 6d65 7465 7273  input parameters
-0000af60: 2073 6565 3a0a 2020 2020 2020 2020 2020   see:.          
-0000af70: 2020 6874 7470 733a 2f2f 7863 6c69 6d2e    https://xclim.
-0000af80: 7265 6164 7468 6564 6f63 732e 696f 2f65  readthedocs.io/e
-0000af90: 6e2f 7374 6162 6c65 2f61 7069 2e68 746d  n/stable/api.htm
-0000afa0: 6c23 7863 6c69 6d2e 696e 6469 6361 746f  l#xclim.indicato
-0000afb0: 7273 2e61 746d 6f73 2e74 6e5f 6d65 616e  rs.atmos.tn_mean
-0000afc0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-0000afd0: 2020 2020 2072 6574 7572 6e20 7863 2e61       return xc.a
-0000afe0: 746d 6f73 2e74 6e5f 6d65 616e 282a 2a70  tmos.tn_mean(**p
-0000aff0: 6172 616d 7329 0a0a 0a63 6c61 7373 2054  arams)...class T
-0000b000: 4e31 3070 3a0a 2020 2020 2222 2246 7261  N10p:.    """Fra
-0000b010: 6374 696f 6e20 6f66 2064 6179 7320 7769  ction of days wi
-0000b020: 7468 206d 696e 2074 656d 7065 7261 7475  th min temperatu
-0000b030: 7265 203c 2031 3074 6820 7065 7263 656e  re < 10th percen
-0000b040: 7469 6c65 2e22 2222 0a0a 2020 2020 7461  tile."""..    ta
-0000b050: 736d 696e 5f70 6572 203d 204e 6f6e 650a  smin_per = None.
+00003a70: 0a0a 0a63 6c61 7373 2044 536e 3a0a 2020  ...class DSn:.  
+00003a80: 2020 2222 2254 6f74 616c 206e 756d 6265    """Total numbe
+00003a90: 7220 6f66 2064 6179 7320 696e 2064 7279  r of days in dry
+00003aa0: 2073 7065 6c6c 7320 2870 7229 2e22 2222   spells (pr)."""
+00003ab0: 0a0a 2020 2020 7468 7265 7368 203d 2031  ..    thresh = 1
+00003ac0: 0a20 2020 2077 696e 646f 7720 3d20 350a  .    window = 5.
+00003ad0: 0a20 2020 2064 6566 2063 6f6d 7075 7465  .    def compute
+00003ae0: 2874 6872 6573 683d 7468 7265 7368 2c20  (thresh=thresh, 
+00003af0: 7769 6e64 6f77 3d77 696e 646f 772c 202a  window=window, *
+00003b00: 2a70 6172 616d 7329 3a0a 2020 2020 2020  *params):.      
+00003b10: 2020 2222 2243 616c 6375 6c61 7465 2074    """Calculate t
+00003b20: 6f74 616c 206e 756d 6265 7220 6f66 2064  otal number of d
+00003b30: 6179 7320 696e 2064 7279 2073 7065 6c6c  ays in dry spell
+00003b40: 732e 0a0a 2020 2020 2020 2020 5061 7261  s...        Para
+00003b50: 6d65 7465 7273 0a20 2020 2020 2020 202d  meters.        -
+00003b60: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 2020  ---------.      
+00003b70: 2020 7468 7265 7368 3a20 696e 7420 6f72    thresh: int or
+00003b80: 2073 7472 696e 670a 2020 2020 2020 2020   string.        
+00003b90: 2020 2020 5468 7265 7368 6f6c 6420 7072      Threshold pr
+00003ba0: 6563 6970 6974 6174 696f 6e20 6265 6c6f  ecipitation belo
+00003bb0: 7720 7768 6963 6820 6120 6461 7920 6973  w which a day is
+00003bc0: 2063 6f6e 7369 6465 7265 640a 2020 2020   considered.    
+00003bd0: 2020 2020 2020 2020 6173 2061 2064 7279          as a dry
+00003be0: 2064 6179 2028 6465 6661 756c 743a 2031   day (default: 1
+00003bf0: 206d 6d29 2e0a 2020 2020 2020 2020 2020   mm)..          
+00003c00: 2020 4966 2074 7970 6520 6f66 2074 6872    If type of thr
+00003c10: 6573 686f 6c64 2069 7320 616e 2069 6e74  eshold is an int
+00003c20: 6567 6572 2074 6865 2075 6e69 7420 6973  eger the unit is
+00003c30: 2073 6574 2074 6f20 6d6d 2e0a 2020 2020   set to mm..    
+00003c40: 2020 2020 7769 6e64 6f77 3a20 696e 740a      window: int.
+00003c50: 2020 2020 2020 2020 2020 2020 4d69 6e69              Mini
+00003c60: 6d75 6d20 6e75 6d62 6572 206f 6620 6461  mum number of da
+00003c70: 7973 2077 6974 6820 7072 6563 6970 6974  ys with precipit
+00003c80: 6174 696f 6e20 6265 6c6f 7720 7468 7265  ation below thre
+00003c90: 7368 6f6c 640a 2020 2020 2020 2020 2020  shold.          
+00003ca0: 2020 746f 2071 7561 6c69 6679 2061 7320    to qualify as 
+00003cb0: 6120 6472 7920 7370 656c 6c20 2864 6566  a dry spell (def
+00003cc0: 6175 6c74 3a20 3529 2e0a 0a20 2020 2020  ault: 5)...     
+00003cd0: 2020 2052 6574 7572 6e73 0a20 2020 2020     Returns.     
+00003ce0: 2020 202d 2d2d 2d2d 2d2d 0a20 2020 2020     -------.     
+00003cf0: 2020 2078 6172 7261 792e 4461 7461 4172     xarray.DataAr
+00003d00: 7261 790a 2020 2020 2020 2020 2020 2020  ray.            
+00003d10: 546f 7461 6c20 6e75 6d62 6572 206f 6620  Total number of 
+00003d20: 6461 7973 2069 6e20 6472 7920 7370 656c  days in dry spel
+00003d30: 6c73 206f 6620 6174 206c 6561 7374 207b  ls of at least {
+00003d40: 7769 6e64 6f77 7d0a 2020 2020 2020 2020  window}.        
+00003d50: 2020 2020 636f 6e73 6563 7574 6976 6520      consecutive 
+00003d60: 6461 7973 2077 6974 6820 7072 6563 6970  days with precip
+00003d70: 6974 6174 696f 6e20 6265 6c6f 7720 7b74  itation below {t
+00003d80: 6872 6573 687d 2e0a 0a20 2020 2020 2020  hresh}...       
+00003d90: 204e 6f74 6573 0a20 2020 2020 2020 202d   Notes.        -
+00003da0: 2d2d 2d2d 0a20 2020 2020 2020 2046 6f72  ----.        For
+00003db0: 206d 6f72 6520 696e 666f 726d 6174 696f   more informatio
+00003dc0: 6e20 6f6e 2074 6865 2069 6e70 7574 2070  n on the input p
+00003dd0: 6172 616d 6574 6572 7320 7365 653a 0a20  arameters see:. 
+00003de0: 2020 2020 2020 2020 2020 2068 7474 7073             https
+00003df0: 3a2f 2f78 636c 696d 2e72 6561 6474 6865  ://xclim.readthe
+00003e00: 646f 6373 2e69 6f2f 656e 2f73 7461 626c  docs.io/en/stabl
+00003e10: 652f 6170 692e 6874 6d6c 2378 636c 696d  e/api.html#xclim
+00003e20: 2e69 6e64 6963 6174 6f72 732e 6174 6d6f  .indicators.atmo
+00003e30: 732e 6472 795f 7370 656c 6c5f 746f 7461  s.dry_spell_tota
+00003e40: 6c5f 6c65 6e67 7468 0a20 2020 2020 2020  l_length.       
+00003e50: 2022 2222 0a20 2020 2020 2020 2074 6872   """.        thr
+00003e60: 6573 6820 3d20 5f74 6872 6573 685f 7374  esh = _thresh_st
+00003e70: 7269 6e67 2874 6872 6573 682c 2022 6d6d  ring(thresh, "mm
+00003e80: 2229 0a20 2020 2020 2020 2072 6574 7572  ").        retur
+00003e90: 6e20 7863 2e61 746d 6f73 2e64 7279 5f73  n xc.atmos.dry_s
+00003ea0: 7065 6c6c 5f74 6f74 616c 5f6c 656e 6774  pell_total_lengt
+00003eb0: 6828 0a20 2020 2020 2020 2020 2020 2074  h(.            t
+00003ec0: 6872 6573 683d 7468 7265 7368 2c0a 2020  hresh=thresh,.  
+00003ed0: 2020 2020 2020 2020 2020 7769 6e64 6f77            window
+00003ee0: 3d77 696e 646f 772c 0a20 2020 2020 2020  =window,.       
+00003ef0: 2020 2020 202a 2a70 6172 616d 732c 0a20       **params,. 
+00003f00: 2020 2020 2020 2029 0a0a 0a63 6c61 7373         )...class
+00003f10: 2057 5366 3a0a 2020 2020 2222 224e 756d   WSf:.    """Num
+00003f20: 6265 7220 6f66 2077 6574 2073 7065 6c6c  ber of wet spell
+00003f30: 7320 2870 7229 2e22 2222 0a0a 2020 2020  s (pr)."""..    
+00003f40: 7468 7265 7368 203d 2031 0a20 2020 2077  thresh = 1.    w
+00003f50: 696e 646f 7720 3d20 350a 0a20 2020 2064  indow = 5..    d
+00003f60: 6566 2063 6f6d 7075 7465 2874 6872 6573  ef compute(thres
+00003f70: 683d 7468 7265 7368 2c20 7769 6e64 6f77  h=thresh, window
+00003f80: 3d77 696e 646f 772c 202a 2a70 6172 616d  =window, **param
+00003f90: 7329 3a0a 2020 2020 2020 2020 2222 2243  s):.        """C
+00003fa0: 616c 6375 6c61 7465 206e 756d 6265 7220  alculate number 
+00003fb0: 6f66 2077 6574 2073 7065 6c6c 732e 0a0a  of wet spells...
+00003fc0: 2020 2020 2020 2020 5061 7261 6d65 7465          Paramete
+00003fd0: 7273 0a20 2020 2020 2020 202d 2d2d 2d2d  rs.        -----
+00003fe0: 2d2d 2d2d 2d0a 2020 2020 2020 2020 7468  -----.        th
+00003ff0: 7265 7368 3a20 696e 7420 6f72 2073 7472  resh: int or str
+00004000: 696e 670a 2020 2020 2020 2020 2020 2020  ing.            
+00004010: 5468 7265 7368 6f6c 6420 7072 6563 6970  Threshold precip
+00004020: 6974 6174 696f 6e20 6162 6f76 6520 7768  itation above wh
+00004030: 6963 6820 6120 6461 7920 6973 2063 6f6e  ich a day is con
+00004040: 7369 6465 7265 640a 2020 2020 2020 2020  sidered.        
+00004050: 2020 2020 6173 2061 2077 6574 2064 6179      as a wet day
+00004060: 2028 6465 6661 756c 743a 2031 206d 6d29   (default: 1 mm)
+00004070: 2e0a 2020 2020 2020 2020 2020 2020 4966  ..            If
+00004080: 2074 7970 6520 6f66 2074 6872 6573 686f   type of thresho
+00004090: 6c64 2069 7320 616e 2069 6e74 6567 6572  ld is an integer
+000040a0: 2074 6865 2075 6e69 7420 6973 2073 6574   the unit is set
+000040b0: 2074 6f20 6d6d 2e0a 2020 2020 2020 2020   to mm..        
+000040c0: 7769 6e64 6f77 3a20 696e 740a 2020 2020  window: int.    
+000040d0: 2020 2020 2020 2020 4d69 6e69 6d75 6d20          Minimum 
+000040e0: 6e75 6d62 6572 206f 6620 6461 7973 2077  number of days w
+000040f0: 6974 6820 7072 6563 6970 6974 6174 696f  ith precipitatio
+00004100: 6e20 6162 6f76 6520 7468 7265 7368 6f6c  n above threshol
+00004110: 640a 2020 2020 2020 2020 2020 2020 746f  d.            to
+00004120: 2071 7561 6c69 6679 2061 7320 6120 7765   qualify as a we
+00004130: 7420 7370 656c 6c20 2864 6566 6175 6c74  t spell (default
+00004140: 3a20 3529 2e0a 0a20 2020 2020 2020 2052  : 5)...        R
+00004150: 6574 7572 6e73 0a20 2020 2020 2020 202d  eturns.        -
+00004160: 2d2d 2d2d 2d2d 0a20 2020 2020 2020 2078  ------.        x
+00004170: 6172 7261 792e 4461 7461 4172 7261 790a  array.DataArray.
+00004180: 2020 2020 2020 2020 2020 2020 4e75 6d62              Numb
+00004190: 6572 206f 6620 7765 7420 7065 7269 6f64  er of wet period
+000041a0: 7320 6f66 206d 696e 696d 756d 207b 7769  s of minimum {wi
+000041b0: 6e64 6f77 7d20 6461 7973 2028 7072 203e  ndow} days (pr >
+000041c0: 3d20 7b74 6872 6573 687d 292e 0a0a 2020  = {thresh})...  
+000041d0: 2020 2020 2020 4e6f 7465 730a 2020 2020        Notes.    
+000041e0: 2020 2020 2d2d 2d2d 2d0a 2020 2020 2020      -----.      
+000041f0: 2020 466f 7220 6d6f 7265 2069 6e66 6f72    For more infor
+00004200: 6d61 7469 6f6e 206f 6e20 7468 6520 696e  mation on the in
+00004210: 7075 7420 7061 7261 6d65 7465 7273 2073  put parameters s
+00004220: 6565 3a0a 2020 2020 2020 2020 2020 2020  ee:.            
+00004230: 6874 7470 733a 2f2f 7863 6c69 6d2e 7265  https://xclim.re
+00004240: 6164 7468 6564 6f63 732e 696f 2f65 6e2f  adthedocs.io/en/
+00004250: 7374 6162 6c65 2f61 7069 2e68 746d 6c23  stable/api.html#
+00004260: 7863 6c69 6d2e 696e 6469 6361 746f 7273  xclim.indicators
+00004270: 2e61 746d 6f73 2e77 6574 5f73 7065 6c6c  .atmos.wet_spell
+00004280: 5f66 7265 7175 656e 6379 0a20 2020 2020  _frequency.     
+00004290: 2020 2022 2222 0a20 2020 2020 2020 2074     """.        t
+000042a0: 6872 6573 6820 3d20 5f74 6872 6573 685f  hresh = _thresh_
+000042b0: 7374 7269 6e67 2874 6872 6573 682c 2022  string(thresh, "
+000042c0: 6d6d 2229 0a20 2020 2020 2020 2072 6574  mm").        ret
+000042d0: 7572 6e20 7863 2e61 746d 6f73 2e77 6574  urn xc.atmos.wet
+000042e0: 5f73 7065 6c6c 5f66 7265 7175 656e 6379  _spell_frequency
+000042f0: 280a 2020 2020 2020 2020 2020 2020 7468  (.            th
+00004300: 7265 7368 3d74 6872 6573 682c 0a20 2020  resh=thresh,.   
+00004310: 2020 2020 2020 2020 2077 696e 646f 773d           window=
+00004320: 7769 6e64 6f77 2c0a 2020 2020 2020 2020  window,.        
+00004330: 2020 2020 2a2a 7061 7261 6d73 2c0a 2020      **params,.  
+00004340: 2020 2020 2020 290a 0a0a 636c 6173 7320        )...class 
+00004350: 5753 783a 0a20 2020 2022 2222 4d61 7869  WSx:.    """Maxi
+00004360: 6d75 6d20 6c65 6e67 7468 206f 6620 7765  mum length of we
+00004370: 7420 7370 656c 6c73 2028 7072 292e 2222  t spells (pr).""
+00004380: 220a 0a20 2020 2074 6872 6573 6820 3d20  "..    thresh = 
+00004390: 310a 2020 2020 7769 6e64 6f77 203d 2031  1.    window = 1
+000043a0: 0a0a 2020 2020 6465 6620 636f 6d70 7574  ..    def comput
+000043b0: 6528 7468 7265 7368 3d74 6872 6573 682c  e(thresh=thresh,
+000043c0: 2077 696e 646f 773d 7769 6e64 6f77 2c20   window=window, 
+000043d0: 2a2a 7061 7261 6d73 293a 0a20 2020 2020  **params):.     
+000043e0: 2020 2022 2222 4361 6c63 756c 6174 6520     """Calculate 
+000043f0: 6d61 7869 6d75 6d20 6c65 6e67 7468 206f  maximum length o
+00004400: 6620 7765 7420 7370 656c 6c73 2e0a 0a20  f wet spells... 
+00004410: 2020 2020 2020 2050 6172 616d 6574 6572         Parameter
+00004420: 730a 2020 2020 2020 2020 2d2d 2d2d 2d2d  s.        ------
+00004430: 2d2d 2d2d 0a20 2020 2020 2020 2074 6872  ----.        thr
+00004440: 6573 683a 2069 6e74 206f 7220 7374 7269  esh: int or stri
+00004450: 6e67 0a20 2020 2020 2020 2020 2020 2054  ng.            T
+00004460: 6872 6573 686f 6c64 2070 7265 6369 7069  hreshold precipi
+00004470: 7461 7469 6f6e 2061 626f 7665 2077 6869  tation above whi
+00004480: 6368 2061 2064 6179 2069 7320 636f 6e73  ch a day is cons
+00004490: 6964 6572 6564 0a20 2020 2020 2020 2020  idered.         
+000044a0: 2020 2061 7320 6120 7765 7420 6461 7920     as a wet day 
+000044b0: 2864 6566 6175 6c74 3a20 3120 6d6d 292e  (default: 1 mm).
+000044c0: 0a20 2020 2020 2020 2020 2020 2049 6620  .            If 
+000044d0: 7479 7065 206f 6620 7468 7265 7368 6f6c  type of threshol
+000044e0: 6420 6973 2061 6e20 696e 7465 6765 7220  d is an integer 
+000044f0: 7468 6520 756e 6974 2069 7320 7365 7420  the unit is set 
+00004500: 746f 206d 6d2e 0a20 2020 2020 2020 2077  to mm..        w
+00004510: 696e 646f 773a 2069 6e74 0a20 2020 2020  indow: int.     
+00004520: 2020 2020 2020 204d 696e 696d 756d 206e         Minimum n
+00004530: 756d 6265 7220 6f66 2064 6179 7320 7769  umber of days wi
+00004540: 7468 2070 7265 6369 7069 7461 7469 6f6e  th precipitation
+00004550: 2061 626f 7665 2074 6872 6573 686f 6c64   above threshold
+00004560: 0a20 2020 2020 2020 2020 2020 2074 6f20  .            to 
+00004570: 7175 616c 6966 7920 6173 2061 2077 6574  qualify as a wet
+00004580: 2073 7065 6c6c 2028 6465 6661 756c 743a   spell (default:
+00004590: 2031 292e 0a0a 2020 2020 2020 2020 5265   1)...        Re
+000045a0: 7475 726e 730a 2020 2020 2020 2020 2d2d  turns.        --
+000045b0: 2d2d 2d2d 2d0a 2020 2020 2020 2020 7861  -----.        xa
+000045c0: 7272 6179 2e44 6174 6141 7272 6179 0a20  rray.DataArray. 
+000045d0: 2020 2020 2020 2020 2020 204d 6178 696d             Maxim
+000045e0: 756d 206c 656e 6774 6820 6f66 2077 6574  um length of wet
+000045f0: 2073 7065 6c6c 7320 6f66 2061 7420 6c65   spells of at le
+00004600: 6173 7420 7b77 696e 646f 777d 2063 6f6e  ast {window} con
+00004610: 7365 6375 7469 7665 2064 6179 730a 2020  secutive days.  
+00004620: 2020 2020 2020 2020 2020 7769 7468 2070            with p
+00004630: 7265 6369 7069 7461 7469 6f6e 2061 626f  recipitation abo
+00004640: 7665 207b 7468 7265 7368 7d2e 0a0a 2020  ve {thresh}...  
+00004650: 2020 2020 2020 4e6f 7465 730a 2020 2020        Notes.    
+00004660: 2020 2020 2d2d 2d2d 2d0a 2020 2020 2020      -----.      
+00004670: 2020 466f 7220 6d6f 7265 2069 6e66 6f72    For more infor
+00004680: 6d61 7469 6f6e 206f 6e20 7468 6520 696e  mation on the in
+00004690: 7075 7420 7061 7261 6d65 7465 7273 2073  put parameters s
+000046a0: 6565 3a0a 2020 2020 2020 2020 2020 2020  ee:.            
+000046b0: 6874 7470 733a 2f2f 7863 6c69 6d2e 7265  https://xclim.re
+000046c0: 6164 7468 6564 6f63 732e 696f 2f65 6e2f  adthedocs.io/en/
+000046d0: 7374 6162 6c65 2f61 7069 2e68 746d 6c23  stable/api.html#
+000046e0: 7863 6c69 6d2e 696e 6469 6361 746f 7273  xclim.indicators
+000046f0: 2e61 746d 6f73 2e77 6574 5f73 7065 6c6c  .atmos.wet_spell
+00004700: 5f6d 6178 5f6c 656e 6774 680a 2020 2020  _max_length.    
+00004710: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00004720: 7468 7265 7368 203d 205f 7468 7265 7368  thresh = _thresh
+00004730: 5f73 7472 696e 6728 7468 7265 7368 2c20  _string(thresh, 
+00004740: 226d 6d22 290a 2020 2020 2020 2020 7265  "mm").        re
+00004750: 7475 726e 2078 632e 6174 6d6f 732e 7765  turn xc.atmos.we
+00004760: 745f 7370 656c 6c5f 6d61 785f 6c65 6e67  t_spell_max_leng
+00004770: 7468 280a 2020 2020 2020 2020 2020 2020  th(.            
+00004780: 7468 7265 7368 3d74 6872 6573 682c 0a20  thresh=thresh,. 
+00004790: 2020 2020 2020 2020 2020 2077 696e 646f             windo
+000047a0: 773d 7769 6e64 6f77 2c0a 2020 2020 2020  w=window,.      
+000047b0: 2020 2020 2020 2a2a 7061 7261 6d73 2c0a        **params,.
+000047c0: 2020 2020 2020 2020 290a 0a0a 636c 6173          )...clas
+000047d0: 7320 5753 6e3a 0a20 2020 2022 2222 546f  s WSn:.    """To
+000047e0: 7461 6c20 6e75 6d62 6572 206f 6620 6461  tal number of da
+000047f0: 7973 2069 6e20 7765 7420 7370 656c 6c73  ys in wet spells
+00004800: 2028 7072 292e 2222 220a 0a20 2020 2074   (pr)."""..    t
+00004810: 6872 6573 6820 3d20 310a 2020 2020 7769  hresh = 1.    wi
+00004820: 6e64 6f77 203d 2035 0a0a 2020 2020 6465  ndow = 5..    de
+00004830: 6620 636f 6d70 7574 6528 7468 7265 7368  f compute(thresh
+00004840: 3d74 6872 6573 682c 2077 696e 646f 773d  =thresh, window=
+00004850: 7769 6e64 6f77 2c20 2a2a 7061 7261 6d73  window, **params
+00004860: 293a 0a20 2020 2020 2020 2022 2222 4361  ):.        """Ca
+00004870: 6c63 756c 6174 6520 746f 7461 6c20 6e75  lculate total nu
+00004880: 6d62 6572 206f 6620 6461 7973 2069 6e20  mber of days in 
+00004890: 7765 7420 7370 656c 6c73 2e0a 0a20 2020  wet spells...   
+000048a0: 2020 2020 2050 6172 616d 6574 6572 730a       Parameters.
+000048b0: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d2d          --------
+000048c0: 2d2d 0a20 2020 2020 2020 2074 6872 6573  --.        thres
+000048d0: 683a 2069 6e74 206f 7220 7374 7269 6e67  h: int or string
+000048e0: 0a20 2020 2020 2020 2020 2020 2054 6872  .            Thr
+000048f0: 6573 686f 6c64 2070 7265 6369 7069 7461  eshold precipita
+00004900: 7469 6f6e 2061 626f 7665 2077 6869 6368  tion above which
+00004910: 2061 2064 6179 2069 7320 636f 6e73 6964   a day is consid
+00004920: 6572 6564 0a20 2020 2020 2020 2020 2020  ered.           
+00004930: 2061 7320 6120 7765 7420 6461 7920 2864   as a wet day (d
+00004940: 6566 6175 6c74 3a20 3120 6d6d 292e 0a20  efault: 1 mm).. 
+00004950: 2020 2020 2020 2020 2020 2049 6620 7479             If ty
+00004960: 7065 206f 6620 7468 7265 7368 6f6c 6420  pe of threshold 
+00004970: 6973 2061 6e20 696e 7465 6765 7220 7468  is an integer th
+00004980: 6520 756e 6974 2069 7320 7365 7420 746f  e unit is set to
+00004990: 206d 6d2e 0a20 2020 2020 2020 2077 696e   mm..        win
+000049a0: 646f 773a 2069 6e74 0a20 2020 2020 2020  dow: int.       
+000049b0: 2020 2020 204d 696e 696d 756d 206e 756d       Minimum num
+000049c0: 6265 7220 6f66 2064 6179 7320 7769 7468  ber of days with
+000049d0: 2070 7265 6369 7069 7461 7469 6f6e 2061   precipitation a
+000049e0: 626f 7665 2074 6872 6573 686f 6c64 0a20  bove threshold. 
+000049f0: 2020 2020 2020 2020 2020 2074 6f20 7175             to qu
+00004a00: 616c 6966 7920 6173 2061 2077 6574 2073  alify as a wet s
+00004a10: 7065 6c6c 2028 6465 6661 756c 743a 2035  pell (default: 5
+00004a20: 292e 0a0a 2020 2020 2020 2020 5265 7475  )...        Retu
+00004a30: 726e 730a 2020 2020 2020 2020 2d2d 2d2d  rns.        ----
+00004a40: 2d2d 2d0a 2020 2020 2020 2020 7861 7272  ---.        xarr
+00004a50: 6179 2e44 6174 6141 7272 6179 0a20 2020  ay.DataArray.   
+00004a60: 2020 2020 2020 2020 2054 6f74 616c 206e           Total n
+00004a70: 756d 6572 206f 6620 6461 7973 2069 6e20  umer of days in 
+00004a80: 7765 7420 7370 656c 6c73 206f 6620 6174  wet spells of at
+00004a90: 206c 6561 7374 207b 7769 6e64 6f77 7d0a   least {window}.
+00004aa0: 2020 2020 2020 2020 2020 2020 636f 6e73              cons
+00004ab0: 6563 7574 6976 6520 6461 7973 2077 6974  ecutive days wit
+00004ac0: 6820 7072 6563 6970 6974 6174 696f 6e20  h precipitation 
+00004ad0: 6162 6f76 6520 7b74 6872 6573 687d 2e0a  above {thresh}..
+00004ae0: 0a20 2020 2020 2020 204e 6f74 6573 0a20  .        Notes. 
+00004af0: 2020 2020 2020 202d 2d2d 2d2d 0a20 2020         -----.   
+00004b00: 2020 2020 2046 6f72 206d 6f72 6520 696e       For more in
+00004b10: 666f 726d 6174 696f 6e20 6f6e 2074 6865  formation on the
+00004b20: 2069 6e70 7574 2070 6172 616d 6574 6572   input parameter
+00004b30: 7320 7365 653a 0a20 2020 2020 2020 2020  s see:.         
+00004b40: 2020 2068 7474 7073 3a2f 2f78 636c 696d     https://xclim
+00004b50: 2e72 6561 6474 6865 646f 6373 2e69 6f2f  .readthedocs.io/
+00004b60: 656e 2f73 7461 626c 652f 6170 692e 6874  en/stable/api.ht
+00004b70: 6d6c 2378 636c 696d 2e69 6e64 6963 6174  ml#xclim.indicat
+00004b80: 6f72 732e 6174 6d6f 732e 7765 745f 7370  ors.atmos.wet_sp
+00004b90: 656c 6c5f 746f 7461 6c5f 6c65 6e67 7468  ell_total_length
+00004ba0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00004bb0: 2020 2020 2074 6872 6573 6820 3d20 5f74       thresh = _t
+00004bc0: 6872 6573 685f 7374 7269 6e67 2874 6872  hresh_string(thr
+00004bd0: 6573 682c 2022 6d6d 2229 0a20 2020 2020  esh, "mm").     
+00004be0: 2020 2072 6574 7572 6e20 7863 2e61 746d     return xc.atm
+00004bf0: 6f73 2e77 6574 5f73 7065 6c6c 5f74 6f74  os.wet_spell_tot
+00004c00: 616c 5f6c 656e 6774 6828 0a20 2020 2020  al_length(.     
+00004c10: 2020 2020 2020 2074 6872 6573 683d 7468         thresh=th
+00004c20: 7265 7368 2c0a 2020 2020 2020 2020 2020  resh,.          
+00004c30: 2020 7769 6e64 6f77 3d77 696e 646f 772c    window=window,
+00004c40: 0a20 2020 2020 2020 2020 2020 202a 2a70  .            **p
+00004c50: 6172 616d 732c 0a20 2020 2020 2020 2029  arams,.        )
+00004c60: 0a0a 0a63 6c61 7373 2044 5452 3a0a 2020  ...class DTR:.  
+00004c70: 2020 2222 224d 6561 6e20 7465 6d70 6572    """Mean temper
+00004c80: 6174 7572 6520 726e 6167 6520 2874 6173  ature rnage (tas
+00004c90: 6d61 782c 2074 6173 6d69 6e29 2e22 2222  max, tasmin)."""
+00004ca0: 0a0a 2020 2020 6465 6620 636f 6d70 7574  ..    def comput
+00004cb0: 6528 2a2a 7061 7261 6d73 293a 0a20 2020  e(**params):.   
+00004cc0: 2020 2020 2022 2222 4361 6c63 756c 6174       """Calculat
+00004cd0: 6520 6d65 616e 206f 6620 6461 696c 7920  e mean of daily 
+00004ce0: 7465 6d70 6572 6174 7572 6520 7261 6e67  temperature rang
+00004cf0: 652e 0a0a 2020 2020 2020 2020 5265 7475  e...        Retu
+00004d00: 726e 730a 2020 2020 2020 2020 2d2d 2d2d  rns.        ----
+00004d10: 2d2d 2d0a 2020 2020 2020 2020 7861 7272  ---.        xarr
+00004d20: 6179 2e44 6174 6141 7272 6179 0a20 2020  ay.DataArray.   
+00004d30: 2020 2020 2020 2020 204d 6561 6e20 6f66           Mean of
+00004d40: 2064 6169 6c79 2074 656d 7065 7261 7475   daily temperatu
+00004d50: 7265 2072 616e 6765 2e0a 0a20 2020 2020  re range...     
+00004d60: 2020 204e 6f74 6573 0a20 2020 2020 2020     Notes.       
+00004d70: 202d 2d2d 2d2d 0a20 2020 2020 2020 2046   -----.        F
+00004d80: 6f72 2069 6e66 6f72 6d61 7469 6f6e 206f  or information o
+00004d90: 6e20 7468 6520 696e 7075 7420 7061 7261  n the input para
+00004da0: 6d65 7465 7273 2073 6565 3a0a 2020 2020  meters see:.    
+00004db0: 2020 2020 2020 2020 6874 7470 733a 2f2f          https://
+00004dc0: 7863 6c69 6d2e 7265 6164 7468 6564 6f63  xclim.readthedoc
+00004dd0: 732e 696f 2f65 6e2f 7374 6162 6c65 2f61  s.io/en/stable/a
+00004de0: 7069 2e68 746d 6c23 7863 6c69 6d2e 696e  pi.html#xclim.in
+00004df0: 6469 6361 746f 7273 2e61 746d 6f73 2e64  dicators.atmos.d
+00004e00: 6169 6c79 5f74 656d 7065 7261 7475 7265  aily_temperature
+00004e10: 5f72 616e 6765 0a20 2020 2020 2020 2022  _range.        "
+00004e20: 2222 0a20 2020 2020 2020 2072 6574 7572  "".        retur
+00004e30: 6e20 7863 2e61 746d 6f73 2e64 6169 6c79  n xc.atmos.daily
+00004e40: 5f74 656d 7065 7261 7475 7265 5f72 616e  _temperature_ran
+00004e50: 6765 282a 2a70 6172 616d 7329 0a0a 0a63  ge(**params)...c
+00004e60: 6c61 7373 2046 443a 0a20 2020 2022 2222  lass FD:.    """
+00004e70: 4e75 6d62 6572 206f 6620 6672 6f73 7420  Number of frost 
+00004e80: 6461 7973 2028 7461 736d 696e 292e 2222  days (tasmin).""
+00004e90: 220a 0a20 2020 2064 6566 2063 6f6d 7075  "..    def compu
+00004ea0: 7465 282a 2a70 6172 616d 7329 3a0a 2020  te(**params):.  
+00004eb0: 2020 2020 2020 2222 2243 616c 6375 6c61        """Calcula
+00004ec0: 7465 206e 756d 6265 7220 6f66 2066 726f  te number of fro
+00004ed0: 7374 2064 6179 7320 2874 6173 6d69 6e20  st days (tasmin 
+00004ee0: 3c20 302e 3020 6465 6743 292e 0a0a 2020  < 0.0 degC)...  
+00004ef0: 2020 2020 2020 5265 7475 726e 730a 2020        Returns.  
+00004f00: 2020 2020 2020 2d2d 2d2d 2d2d 2d0a 2020        -------.  
+00004f10: 2020 2020 2020 7861 7272 6179 2e44 6174        xarray.Dat
+00004f20: 6141 7272 6179 0a20 2020 2020 2020 2020  aArray.         
+00004f30: 2020 204e 756d 6265 7220 6f66 2066 726f     Number of fro
+00004f40: 7374 2064 6179 7320 2874 6173 6d69 6e20  st days (tasmin 
+00004f50: 3c20 302e 3020 6465 6743 292e 0a0a 2020  < 0.0 degC)...  
+00004f60: 2020 2020 2020 4e6f 7465 730a 2020 2020        Notes.    
+00004f70: 2020 2020 2d2d 2d2d 2d0a 2020 2020 2020      -----.      
+00004f80: 2020 466f 7220 696e 666f 726d 6174 696f    For informatio
+00004f90: 6e20 6f6e 2074 6865 2069 6e70 7574 2070  n on the input p
+00004fa0: 6172 616d 6574 6572 7320 7365 653a 0a20  arameters see:. 
+00004fb0: 2020 2020 2020 2020 2020 2068 7474 7073             https
+00004fc0: 3a2f 2f78 636c 696d 2e72 6561 6474 6865  ://xclim.readthe
+00004fd0: 646f 6373 2e69 6f2f 656e 2f73 7461 626c  docs.io/en/stabl
+00004fe0: 652f 6170 692e 6874 6d6c 2378 636c 696d  e/api.html#xclim
+00004ff0: 2e69 6e64 6963 6174 6f72 732e 6174 6d6f  .indicators.atmo
+00005000: 732e 6672 6f73 745f 6461 7973 0a20 2020  s.frost_days.   
+00005010: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+00005020: 2072 6574 7572 6e20 7863 2e61 746d 6f73   return xc.atmos
+00005030: 2e66 726f 7374 5f64 6179 7328 2a2a 7061  .frost_days(**pa
+00005040: 7261 6d73 290a 0a0a 636c 6173 7320 4c46  rams)...class LF
+00005050: 443a 0a20 2020 2022 2222 4e75 6d62 6572  D:.    """Number
+00005060: 206f 6620 6c61 7465 2066 726f 7374 2064   of late frost d
+00005070: 6179 7320 2874 6173 6d69 6e29 2e22 2222  ays (tasmin)."""
+00005080: 0a0a 2020 2020 7374 6172 745f 6461 7465  ..    start_date
+00005090: 203d 2022 3034 2d30 3122 0a20 2020 2065   = "04-01".    e
+000050a0: 6e64 5f64 6174 6520 3d20 2230 362d 3330  nd_date = "06-30
+000050b0: 220a 0a20 2020 2064 6566 2063 6f6d 7075  "..    def compu
+000050c0: 7465 2873 7461 7274 5f64 6174 653d 7374  te(start_date=st
+000050d0: 6172 745f 6461 7465 2c20 656e 645f 6461  art_date, end_da
+000050e0: 7465 3d65 6e64 5f64 6174 652c 202a 2a70  te=end_date, **p
+000050f0: 6172 616d 7329 3a0a 2020 2020 2020 2020  arams):.        
+00005100: 2222 2243 616c 6375 6c61 7465 206e 756d  """Calculate num
+00005110: 6265 7220 6f66 206c 6174 6520 6672 6f73  ber of late fros
+00005120: 7420 6461 7973 2028 7461 736d 696e 203c  t days (tasmin <
+00005130: 2030 2e30 2064 6567 4329 2e0a 0a20 2020   0.0 degC)...   
+00005140: 2020 2020 2050 6172 616d 6574 6572 730a       Parameters.
+00005150: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d2d          --------
+00005160: 2d2d 0a20 2020 2020 2020 2073 7461 7274  --.        start
+00005170: 5f64 6174 653a 2073 7472 0a20 2020 2020  _date: str.     
+00005180: 2020 2020 2020 204c 6566 7420 626f 756e         Left boun
+00005190: 6420 6f66 2074 6865 2070 6572 696f 6420  d of the period 
+000051a0: 746f 2062 6520 636f 6e73 6964 6572 6564  to be considered
+000051b0: 2e0a 2020 2020 2020 2020 656e 645f 6461  ..        end_da
+000051c0: 7465 3a20 7374 720a 2020 2020 2020 2020  te: str.        
+000051d0: 2020 2020 5269 6768 7420 626f 756e 6420      Right bound 
+000051e0: 6f66 2074 6865 2070 6572 696f 6420 746f  of the period to
+000051f0: 2062 6520 636f 6e73 6964 6572 6564 2e0a   be considered..
+00005200: 0a20 2020 2020 2020 2052 6574 7572 6e73  .        Returns
+00005210: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
+00005220: 0a20 2020 2020 2020 2078 6172 7261 792e  .        xarray.
+00005230: 4461 7461 4172 7261 790a 2020 2020 2020  DataArray.      
+00005240: 2020 2020 2020 4e75 6d62 6572 206f 6620        Number of 
+00005250: 6672 6f73 7420 6461 7973 2028 7461 736d  frost days (tasm
+00005260: 696e 203c 2030 2e30 290a 2020 2020 2020  in < 0.0).      
+00005270: 2020 2020 2020 6265 7477 6565 6e20 7b73        between {s
+00005280: 7461 7274 5f64 6174 657d 2061 6e64 207b  tart_date} and {
+00005290: 656e 645f 6461 7465 7d2e 0a0a 2020 2020  end_date}...    
+000052a0: 2020 2020 4e6f 7465 730a 2020 2020 2020      Notes.      
+000052b0: 2020 2d2d 2d2d 2d0a 2020 2020 2020 2020    -----.        
+000052c0: 466f 7220 696e 666f 726d 6174 696f 6e20  For information 
+000052d0: 6f6e 2074 6865 2069 6e70 7574 2070 6172  on the input par
+000052e0: 616d 6574 6572 7320 7365 653a 0a20 2020  ameters see:.   
+000052f0: 2020 2020 2020 2020 2068 7474 7073 3a2f           https:/
+00005300: 2f78 636c 696d 2e72 6561 6474 6865 646f  /xclim.readthedo
+00005310: 6373 2e69 6f2f 656e 2f73 7461 626c 652f  cs.io/en/stable/
+00005320: 6170 692e 6874 6d6c 2378 636c 696d 2e69  api.html#xclim.i
+00005330: 6e64 6963 6174 6f72 732e 6174 6d6f 732e  ndicators.atmos.
+00005340: 6c61 7465 5f66 726f 7374 5f64 6179 730a  late_frost_days.
+00005350: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00005360: 2020 2020 7265 7475 726e 2078 632e 6174      return xc.at
+00005370: 6d6f 732e 6c61 7465 5f66 726f 7374 5f64  mos.late_frost_d
+00005380: 6179 7328 0a20 2020 2020 2020 2020 2020  ays(.           
+00005390: 2064 6174 655f 626f 756e 6473 3d28 7374   date_bounds=(st
+000053a0: 6172 745f 6461 7465 2c20 656e 645f 6461  art_date, end_da
+000053b0: 7465 292c 0a20 2020 2020 2020 2020 2020  te),.           
+000053c0: 202a 2a70 6172 616d 732c 0a20 2020 2020   **params,.     
+000053d0: 2020 2029 0a0a 0a63 6c61 7373 2049 443a     )...class ID:
+000053e0: 0a20 2020 2022 2222 4e75 6d62 6572 206f  .    """Number o
+000053f0: 6620 6963 6520 6461 7973 2028 7461 736d  f ice days (tasm
+00005400: 6178 292e 2222 220a 0a20 2020 2064 6566  ax)."""..    def
+00005410: 2063 6f6d 7075 7465 282a 2a70 6172 616d   compute(**param
+00005420: 7329 3a0a 2020 2020 2020 2020 2222 2243  s):.        """C
+00005430: 616c 6375 6c61 7465 206e 756d 6265 7220  alculate number 
+00005440: 6f66 2069 6365 2064 6179 7320 2874 6173  of ice days (tas
+00005450: 6d61 7820 3c20 302e 3020 6465 6743 292e  max < 0.0 degC).
+00005460: 0a0a 2020 2020 2020 2020 5061 7261 6d65  ..        Parame
+00005470: 7465 7273 0a20 2020 2020 2020 202d 2d2d  ters.        ---
+00005480: 2d2d 2d2d 2d2d 2d0a 2020 2020 2020 2020  -------.        
+00005490: 466f 7220 696e 666f 726d 6174 696f 6e20  For information 
+000054a0: 6f6e 2074 6865 2069 6e70 7574 2070 6172  on the input par
+000054b0: 616d 6574 6572 7320 7365 653a 0a20 2020  ameters see:.   
+000054c0: 2020 2020 2020 2020 2068 7474 7073 3a2f           https:/
+000054d0: 2f78 636c 696d 2e72 6561 6474 6865 646f  /xclim.readthedo
+000054e0: 6373 2e69 6f2f 656e 2f73 7461 626c 652f  cs.io/en/stable/
+000054f0: 6170 692e 6874 6d6c 2378 636c 696d 2e69  api.html#xclim.i
+00005500: 6e64 6963 6174 6f72 732e 6174 6d6f 732e  ndicators.atmos.
+00005510: 6963 655f 6461 7973 0a0a 2020 2020 2020  ice_days..      
+00005520: 2020 5265 7475 726e 730a 2020 2020 2020    Returns.      
+00005530: 2020 2d2d 2d2d 2d2d 2d0a 2020 2020 2020    -------.      
+00005540: 2020 7861 7272 6179 2e44 6174 6141 7272    xarray.DataArr
+00005550: 6179 0a20 2020 2020 2020 2020 2020 204e  ay.            N
+00005560: 756d 6265 7220 6f66 2069 6365 2064 6179  umber of ice day
+00005570: 7320 2874 6173 6d61 7820 3c20 302e 3020  s (tasmax < 0.0 
+00005580: 6465 6743 292e 0a20 2020 2020 2020 2022  degC)..        "
+00005590: 2222 0a20 2020 2020 2020 2072 6574 7572  "".        retur
+000055a0: 6e20 7863 2e61 746d 6f73 2e69 6365 5f64  n xc.atmos.ice_d
+000055b0: 6179 7328 2a2a 7061 7261 6d73 290a 0a0a  ays(**params)...
+000055c0: 636c 6173 7320 4744 3a0a 2020 2020 2222  class GD:.    ""
+000055d0: 2243 756d 756c 6174 6976 6520 6772 6f77  "Cumulative grow
+000055e0: 696e 6720 6465 6772 6565 2064 6179 7320  ing degree days 
+000055f0: 2874 6173 292e 2222 220a 0a20 2020 2074  (tas)."""..    t
+00005600: 6872 6573 6820 3d20 340a 0a20 2020 2064  hresh = 4..    d
+00005610: 6566 2063 6f6d 7075 7465 2874 6872 6573  ef compute(thres
+00005620: 683d 7468 7265 7368 2c20 2a2a 7061 7261  h=thresh, **para
+00005630: 6d73 293a 0a20 2020 2020 2020 2022 2222  ms):.        """
+00005640: 4361 6c63 756c 6174 6520 6375 6d75 6c61  Calculate cumula
+00005650: 7469 7665 2067 726f 7769 6e67 2064 6567  tive growing deg
+00005660: 7265 6520 6461 7973 2028 7461 7320 3e20  ree days (tas > 
+00005670: 7468 7265 7368 292e 0a0a 2020 2020 2020  thresh)...      
+00005680: 2020 5061 7261 6d65 7465 7273 0a20 2020    Parameters.   
+00005690: 2020 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a       ----------.
+000056a0: 2020 2020 2020 2020 7468 7265 7368 3a20          thresh: 
+000056b0: 696e 7420 6f72 2073 7472 696e 670a 2020  int or string.  
+000056c0: 2020 2020 2020 2020 2020 5468 7265 7368            Thresh
+000056d0: 6f6c 6420 7465 6d70 6572 6174 7572 6520  old temperature 
+000056e0: 6162 6f76 6520 7768 6963 6820 7468 6520  above which the 
+000056f0: 6461 696c 7920 7465 6d70 6572 6174 7572  daily temperatur
+00005700: 6520 7769 6c6c 0a20 2020 2020 2020 2020  e will.         
+00005710: 2020 2062 6520 6164 6465 6420 746f 2074     be added to t
+00005720: 6865 2063 756d 756c 6174 6976 6520 7375  he cumulative su
+00005730: 6d20 6f66 2074 656d 7065 7261 7475 7265  m of temperature
+00005740: 2064 6567 7265 6573 2e0a 0a20 2020 2020   degrees...     
+00005750: 2020 2052 6574 7572 6e73 0a20 2020 2020     Returns.     
+00005760: 2020 202d 2d2d 2d2d 2d2d 0a20 2020 2020     -------.     
+00005770: 2020 2078 6172 7261 792e 4461 7461 4172     xarray.DataAr
+00005780: 7261 790a 2020 2020 2020 2020 2020 2020  ray.            
+00005790: 4375 6d75 6c61 7469 7665 2067 726f 7769  Cumulative growi
+000057a0: 6e67 2064 6567 7265 6520 6461 7973 2028  ng degree days (
+000057b0: 7461 7320 3e20 7b74 6872 6573 687d 292e  tas > {thresh}).
+000057c0: 0a0a 2020 2020 2020 2020 4e6f 7465 730a  ..        Notes.
+000057d0: 2020 2020 2020 2020 2d2d 2d2d 2d0a 2020          -----.  
+000057e0: 2020 2020 2020 466f 7220 6d6f 7265 2069        For more i
+000057f0: 6e66 6f72 6d61 7469 6f6e 206f 6e20 7468  nformation on th
+00005800: 6520 696e 7075 7420 7061 7261 6d65 7465  e input paramete
+00005810: 7273 2073 6565 3a0a 2020 2020 2020 2020  rs see:.        
+00005820: 2020 2020 6874 7470 733a 2f2f 7863 6c69      https://xcli
+00005830: 6d2e 7265 6164 7468 6564 6f63 732e 696f  m.readthedocs.io
+00005840: 2f65 6e2f 7374 6162 6c65 2f61 7069 2e68  /en/stable/api.h
+00005850: 746d 6c23 7863 6c69 6d2e 696e 6469 6361  tml#xclim.indica
+00005860: 746f 7273 2e61 746d 6f73 2e67 726f 7769  tors.atmos.growi
+00005870: 6e67 5f64 6567 7265 655f 6461 7973 0a20  ng_degree_days. 
+00005880: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00005890: 2020 2074 6872 6573 6820 3d20 5f74 6872     thresh = _thr
+000058a0: 6573 685f 7374 7269 6e67 2874 6872 6573  esh_string(thres
+000058b0: 682c 2022 6465 6743 2229 0a20 2020 2020  h, "degC").     
+000058c0: 2020 2072 6574 7572 6e20 7863 2e61 746d     return xc.atm
+000058d0: 6f73 2e67 726f 7769 6e67 5f64 6567 7265  os.growing_degre
+000058e0: 655f 6461 7973 280a 2020 2020 2020 2020  e_days(.        
+000058f0: 2020 2020 7468 7265 7368 3d74 6872 6573      thresh=thres
+00005900: 682c 0a20 2020 2020 2020 2020 2020 202a  h,.            *
+00005910: 2a70 6172 616d 732c 0a20 2020 2020 2020  *params,.       
+00005920: 2029 0a0a 0a63 6c61 7373 2048 4431 373a   )...class HD17:
+00005930: 0a20 2020 2022 2222 4375 6d75 6c61 7469  .    """Cumulati
+00005940: 7665 2068 6561 7469 6e67 2064 6567 7265  ve heating degre
+00005950: 6520 6461 7973 2028 7461 7329 2e22 2222  e days (tas)."""
+00005960: 0a0a 2020 2020 6465 6620 636f 6d70 7574  ..    def comput
+00005970: 6528 2a2a 7061 7261 6d73 293a 0a20 2020  e(**params):.   
+00005980: 2020 2020 2022 2222 4361 6c63 756c 6174       """Calculat
+00005990: 6520 6375 6d75 6c61 7469 7665 2068 6561  e cumulative hea
+000059a0: 7469 6e67 2064 6567 7265 6520 6461 7973  ting degree days
+000059b0: 2028 7461 7320 3c20 3137 2064 6567 4329   (tas < 17 degC)
+000059c0: 2e0a 0a20 2020 2020 2020 2052 6574 7572  ...        Retur
+000059d0: 6e73 0a20 2020 2020 2020 202d 2d2d 2d2d  ns.        -----
+000059e0: 2d2d 0a20 2020 2020 2020 2078 6172 7261  --.        xarra
+000059f0: 792e 4461 7461 4172 7261 790a 2020 2020  y.DataArray.    
+00005a00: 2020 2020 2020 2020 4375 6d75 6c61 7469          Cumulati
+00005a10: 7665 2068 6561 7469 6e67 2064 6567 7265  ve heating degre
+00005a20: 6520 6461 7973 2028 7461 7320 3e20 3137  e days (tas > 17
+00005a30: 2064 6567 4329 2e0a 0a20 2020 2020 2020   degC)...       
+00005a40: 204e 6f74 6573 0a20 2020 2020 2020 202d   Notes.        -
+00005a50: 2d2d 2d2d 0a20 2020 2020 2020 2046 6f72  ----.        For
+00005a60: 2069 6e66 6f72 6d61 7469 6f6e 206f 6e20   information on 
+00005a70: 7468 6520 696e 7075 7420 7061 7261 6d65  the input parame
+00005a80: 7465 7273 2073 6565 3a0a 2020 2020 2020  ters see:.      
+00005a90: 2020 2020 2020 6874 7470 733a 2f2f 7863        https://xc
+00005aa0: 6c69 6d2e 7265 6164 7468 6564 6f63 732e  lim.readthedocs.
+00005ab0: 696f 2f65 6e2f 7374 6162 6c65 2f61 7069  io/en/stable/api
+00005ac0: 2e68 746d 6c23 7863 6c69 6d2e 696e 6469  .html#xclim.indi
+00005ad0: 6361 746f 7273 2e61 746d 6f73 2e68 6561  cators.atmos.hea
+00005ae0: 7469 6e67 5f64 6567 7265 655f 6461 7973  ting_degree_days
+00005af0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00005b00: 2020 2020 2072 6574 7572 6e20 7863 2e61       return xc.a
+00005b10: 746d 6f73 2e68 6561 7469 6e67 5f64 6567  tmos.heating_deg
+00005b20: 7265 655f 6461 7973 280a 2020 2020 2020  ree_days(.      
+00005b30: 2020 2020 2020 2a2a 7061 7261 6d73 2c0a        **params,.
+00005b40: 2020 2020 2020 2020 290a 0a0a 636c 6173          )...clas
+00005b50: 7320 5052 4350 544f 543a 0a20 2020 2022  s PRCPTOT:.    "
+00005b60: 2222 546f 7461 6c20 7072 6563 6970 6974  ""Total precipit
+00005b70: 6174 696f 6e20 616d 6f75 6e74 2028 7072  ation amount (pr
+00005b80: 292e 2222 220a 0a20 2020 2074 6872 6573  )."""..    thres
+00005b90: 6820 3d20 310a 0a20 2020 2064 6566 2063  h = 1..    def c
+00005ba0: 6f6d 7075 7465 2874 6872 6573 683d 7468  ompute(thresh=th
+00005bb0: 7265 7368 2c20 2a2a 7061 7261 6d73 293a  resh, **params):
+00005bc0: 0a20 2020 2020 2020 2022 2222 4361 6c63  .        """Calc
+00005bd0: 756c 6174 6520 746f 7461 6c20 7072 6563  ulate total prec
+00005be0: 6970 6974 6174 696f 6e20 616d 6f75 6e74  ipitation amount
+00005bf0: 2e0a 0a20 2020 2020 2020 2050 6172 616d  ...        Param
+00005c00: 6574 6572 730a 2020 2020 2020 2020 2d2d  eters.        --
+00005c10: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020 2020  --------.       
+00005c20: 2074 6872 6573 683a 2069 6e74 206f 7220   thresh: int or 
+00005c30: 7374 7269 6e67 0a20 2020 2020 2020 2020  string.         
+00005c40: 2020 2054 6872 6573 686f 6c64 2070 7265     Threshold pre
+00005c50: 6369 7069 7461 7469 6f6e 2061 626f 7665  cipitation above
+00005c60: 2077 6869 6368 2061 2064 6179 2069 7320   which a day is 
+00005c70: 636f 6e73 6964 6572 6564 0a20 2020 2020  considered.     
+00005c80: 2020 2020 2020 2061 7320 6120 7765 7420         as a wet 
+00005c90: 6461 7920 2864 6566 6175 6c74 3a20 3120  day (default: 1 
+00005ca0: 6d6d 2f64 6179 292e 0a20 2020 2020 2020  mm/day)..       
+00005cb0: 2020 2020 2049 6620 7479 7065 206f 6620       If type of 
+00005cc0: 7468 7265 7368 6f6c 6420 6973 2061 6e20  threshold is an 
+00005cd0: 696e 7465 6765 7220 7468 6520 756e 6974  integer the unit
+00005ce0: 2069 7320 7365 7420 746f 206d 6d2f 6461   is set to mm/da
+00005cf0: 792e 0a0a 2020 2020 2020 2020 5265 7475  y...        Retu
+00005d00: 726e 730a 2020 2020 2020 2020 2d2d 2d2d  rns.        ----
+00005d10: 2d2d 2d0a 2020 2020 2020 2020 7861 7272  ---.        xarr
+00005d20: 6179 2e44 6174 6141 7272 6179 0a20 2020  ay.DataArray.   
+00005d30: 2020 2020 2020 2020 2054 6f74 616c 2070           Total p
+00005d40: 7265 6369 7069 7461 7469 6f6e 2061 6d6f  recipitation amo
+00005d50: 756e 7420 6f66 2077 6574 2064 6179 7320  unt of wet days 
+00005d60: 2870 7265 6369 7020 3e20 7b74 6872 6573  (precip > {thres
+00005d70: 687d 290a 0a20 2020 2020 2020 204e 6f74  h})..        Not
+00005d80: 6573 0a20 2020 2020 2020 202d 2d2d 2d2d  es.        -----
+00005d90: 0a20 2020 2020 2020 2046 6f72 206d 6f72  .        For mor
+00005da0: 6520 696e 666f 726d 6174 696f 6e20 6f6e  e information on
+00005db0: 2074 6865 2069 6e70 7574 2070 6172 616d   the input param
+00005dc0: 6574 6572 7320 7365 653a 0a20 2020 2020  eters see:.     
+00005dd0: 2020 2020 2020 2068 7474 7073 3a2f 2f78         https://x
+00005de0: 636c 696d 2e72 6561 6474 6865 646f 6373  clim.readthedocs
+00005df0: 2e69 6f2f 656e 2f73 7461 626c 652f 6170  .io/en/stable/ap
+00005e00: 692e 6874 6d6c 2378 636c 696d 2e69 6e64  i.html#xclim.ind
+00005e10: 6963 6174 6f72 732e 6174 6d6f 732e 7765  icators.atmos.we
+00005e20: 745f 7072 6563 6970 5f61 6363 756d 756c  t_precip_accumul
+00005e30: 6174 696f 6e0a 2020 2020 2020 2020 2222  ation.        ""
+00005e40: 220a 2020 2020 2020 2020 7468 7265 7368  ".        thresh
+00005e50: 203d 205f 7468 7265 7368 5f73 7472 696e   = _thresh_strin
+00005e60: 6728 7468 7265 7368 2c20 226d 6d2f 6461  g(thresh, "mm/da
+00005e70: 7922 290a 2020 2020 2020 2020 7265 7475  y").        retu
+00005e80: 726e 2078 632e 6174 6d6f 732e 7765 745f  rn xc.atmos.wet_
+00005e90: 7072 6563 6970 5f61 6363 756d 756c 6174  precip_accumulat
+00005ea0: 696f 6e28 0a20 2020 2020 2020 2020 2020  ion(.           
+00005eb0: 2074 6872 6573 683d 7468 7265 7368 2c0a   thresh=thresh,.
+00005ec0: 2020 2020 2020 2020 2020 2020 2a2a 7061              **pa
+00005ed0: 7261 6d73 2c0a 2020 2020 2020 2020 290a  rams,.        ).
+00005ee0: 0a0a 636c 6173 7320 5252 3a0a 2020 2020  ..class RR:.    
+00005ef0: 2222 2254 6f74 616c 2070 7265 6369 7069  """Total precipi
+00005f00: 7461 7469 6f6e 2028 7072 292e 2222 220a  tation (pr).""".
+00005f10: 0a20 2020 2064 6566 2063 6f6d 7075 7465  .    def compute
+00005f20: 282a 2a70 6172 616d 7329 3a0a 2020 2020  (**params):.    
+00005f30: 2020 2020 2222 2243 616c 6375 6c61 7465      """Calculate
+00005f40: 2074 6f74 616c 2070 7265 6369 7069 7461   total precipita
+00005f50: 7469 6f6e 2e0a 0a20 2020 2020 2020 2052  tion...        R
+00005f60: 6574 7572 6e73 0a20 2020 2020 2020 202d  eturns.        -
+00005f70: 2d2d 2d2d 2d2d 0a20 2020 2020 2020 2078  ------.        x
+00005f80: 6172 7261 792e 4461 7461 4172 7261 790a  array.DataArray.
+00005f90: 2020 2020 2020 2020 2020 2020 546f 7461              Tota
+00005fa0: 6c20 7072 6563 6970 6974 6174 696f 6e2e  l precipitation.
+00005fb0: 0a0a 2020 2020 2020 2020 4e6f 7465 730a  ..        Notes.
+00005fc0: 2020 2020 2020 2020 2d2d 2d2d 2d0a 2020          -----.  
+00005fd0: 2020 2020 2020 466f 7220 696e 666f 726d        For inform
+00005fe0: 6174 696f 6e20 6f6e 2074 6865 2069 6e70  ation on the inp
+00005ff0: 7574 2070 6172 616d 6574 6572 7320 7365  ut parameters se
+00006000: 653a 0a20 2020 2020 2020 2020 2020 2068  e:.            h
+00006010: 7474 7073 3a2f 2f78 636c 696d 2e72 6561  ttps://xclim.rea
+00006020: 6474 6865 646f 6373 2e69 6f2f 656e 2f73  dthedocs.io/en/s
+00006030: 7461 626c 652f 6170 692e 6874 6d6c 2378  table/api.html#x
+00006040: 636c 696d 2e69 6e64 6963 6174 6f72 732e  clim.indicators.
+00006050: 6174 6d6f 732e 7072 6563 6970 5f61 6363  atmos.precip_acc
+00006060: 756d 756c 6174 696f 6e0a 2020 2020 2020  umulation.      
+00006070: 2020 2222 220a 2020 2020 2020 2020 7265    """.        re
+00006080: 7475 726e 2078 632e 6174 6d6f 732e 7072  turn xc.atmos.pr
+00006090: 6563 6970 5f61 6363 756d 756c 6174 696f  ecip_accumulatio
+000060a0: 6e28 2a2a 7061 7261 6d73 290a 0a0a 636c  n(**params)...cl
+000060b0: 6173 7320 5252 6d3a 0a20 2020 2022 2222  ass RRm:.    """
+000060c0: 4d65 616e 2064 6169 6c79 2070 7265 6369  Mean daily preci
+000060d0: 7069 7461 7469 6f6e 2028 7072 292e 2222  pitation (pr).""
+000060e0: 220a 0a20 2020 2064 6566 2063 6f6d 7075  "..    def compu
+000060f0: 7465 282a 2a70 6172 616d 7329 3a0a 2020  te(**params):.  
+00006100: 2020 2020 2020 2222 2243 616c 6375 6c61        """Calcula
+00006110: 7465 206d 6561 6e20 6461 696c 7920 7072  te mean daily pr
+00006120: 6563 6970 6974 6174 696f 6e2e 0a0a 2020  ecipitation...  
+00006130: 2020 2020 2020 5265 7475 726e 730a 2020        Returns.  
+00006140: 2020 2020 2020 2d2d 2d2d 2d2d 2d0a 2020        -------.  
+00006150: 2020 2020 2020 7861 7272 6179 2e44 6174        xarray.Dat
+00006160: 6141 7272 6179 0a20 2020 2020 2020 2020  aArray.         
+00006170: 2020 204d 6561 6e20 6461 696c 7920 7072     Mean daily pr
+00006180: 6563 6970 6974 6174 696f 6e2e 0a0a 2020  ecipitation...  
+00006190: 2020 2020 2020 4e6f 7465 730a 2020 2020        Notes.    
+000061a0: 2020 2020 2d2d 2d2d 2d0a 2020 2020 2020      -----.      
+000061b0: 2020 466f 7220 696e 666f 726d 6174 696f    For informatio
+000061c0: 6e20 6f6e 2074 6865 2069 6e70 7574 2070  n on the input p
+000061d0: 6172 616d 6574 6572 7320 7365 653a 0a20  arameters see:. 
+000061e0: 2020 2020 2020 2020 2020 2068 7474 7073             https
+000061f0: 3a2f 2f78 636c 696d 2e72 6561 6474 6865  ://xclim.readthe
+00006200: 646f 6373 2e69 6f2f 656e 2f73 7461 626c  docs.io/en/stabl
+00006210: 652f 6170 692e 6874 6d6c 2378 636c 696d  e/api.html#xclim
+00006220: 2e69 6e64 6963 6174 6f72 732e 6174 6d6f  .indicators.atmo
+00006230: 732e 7072 6563 6970 5f61 7665 7261 6765  s.precip_average
+00006240: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00006250: 2020 2020 2072 6574 7572 6e20 7863 2e61       return xc.a
+00006260: 746d 6f73 2e70 7265 6369 705f 6176 6572  tmos.precip_aver
+00006270: 6167 6528 2a2a 7061 7261 6d73 290a 0a0a  age(**params)...
+00006280: 636c 6173 7320 5252 313a 0a20 2020 2022  class RR1:.    "
+00006290: 2222 4e75 6d62 6572 206f 6620 7765 7420  ""Number of wet 
+000062a0: 6461 7973 2028 7072 292e 2222 220a 0a20  days (pr).""".. 
+000062b0: 2020 2064 6566 2063 6f6d 7075 7465 282a     def compute(*
+000062c0: 2a70 6172 616d 7329 3a0a 2020 2020 2020  *params):.      
+000062d0: 2020 2222 2243 616c 6375 6c61 7465 206e    """Calculate n
+000062e0: 756d 6265 7220 6f66 2077 6574 2064 6179  umber of wet day
+000062f0: 7320 2870 7220 3e3d 2031 206d 6d2f 6461  s (pr >= 1 mm/da
+00006300: 7929 2e0a 0a20 2020 2020 2020 2052 6574  y)...        Ret
+00006310: 7572 6e73 0a20 2020 2020 2020 202d 2d2d  urns.        ---
+00006320: 2d2d 2d2d 0a20 2020 2020 2020 2078 6172  ----.        xar
+00006330: 7261 792e 4461 7461 4172 7261 790a 2020  ray.DataArray.  
+00006340: 2020 2020 2020 2020 2020 4e75 6d62 6572            Number
+00006350: 206f 6620 7765 7420 6461 7973 2028 7072   of wet days (pr
+00006360: 203e 3d20 3120 6d6d 2f64 6179 292e 0a0a   >= 1 mm/day)...
+00006370: 2020 2020 2020 2020 4e6f 7465 730a 2020          Notes.  
+00006380: 2020 2020 2020 2d2d 2d2d 2d0a 2020 2020        -----.    
+00006390: 2020 2020 466f 7220 696e 666f 726d 6174      For informat
+000063a0: 696f 6e20 6f6e 2074 6865 2069 6e70 7574  ion on the input
+000063b0: 2070 6172 616d 6574 6572 7320 7365 653a   parameters see:
+000063c0: 0a20 2020 2020 2020 2020 2020 2068 7474  .            htt
+000063d0: 7073 3a2f 2f78 636c 696d 2e72 6561 6474  ps://xclim.readt
+000063e0: 6865 646f 6373 2e69 6f2f 656e 2f73 7461  hedocs.io/en/sta
+000063f0: 626c 652f 6170 692e 6874 6d6c 2378 636c  ble/api.html#xcl
+00006400: 696d 2e69 6e64 6963 6174 6f72 732e 6174  im.indicators.at
+00006410: 6d6f 732e 7765 7464 6179 730a 2020 2020  mos.wetdays.    
+00006420: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00006430: 7265 7475 726e 2078 632e 6174 6d6f 732e  return xc.atmos.
+00006440: 7765 7464 6179 7328 0a20 2020 2020 2020  wetdays(.       
+00006450: 2020 2020 2074 6872 6573 683d 2231 206d       thresh="1 m
+00006460: 6d2f 6461 7922 2c0a 2020 2020 2020 2020  m/day",.        
+00006470: 2020 2020 2a2a 7061 7261 6d73 2c0a 2020      **params,.  
+00006480: 2020 2020 2020 290a 0a0a 636c 6173 7320        )...class 
+00006490: 5231 306d 6d3a 0a20 2020 2022 2222 4e75  R10mm:.    """Nu
+000064a0: 6d62 6572 206f 6620 6865 6176 7920 7072  mber of heavy pr
+000064b0: 6563 6970 6974 6174 696f 6e20 6461 7973  ecipitation days
+000064c0: 2028 7072 292e 2222 220a 0a20 2020 2064   (pr)."""..    d
+000064d0: 6566 2063 6f6d 7075 7465 282a 2a70 6172  ef compute(**par
+000064e0: 616d 7329 3a0a 2020 2020 2020 2020 2222  ams):.        ""
+000064f0: 2243 616c 6375 6c61 7465 206e 756d 6265  "Calculate numbe
+00006500: 7220 6f66 2077 6574 2064 6179 7320 2870  r of wet days (p
+00006510: 7220 3e3d 2031 3020 6d6d 2f64 6179 292e  r >= 10 mm/day).
+00006520: 0a0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
+00006530: 730a 2020 2020 2020 2020 2d2d 2d2d 2d2d  s.        ------
+00006540: 2d0a 2020 2020 2020 2020 7861 7272 6179  -.        xarray
+00006550: 2e44 6174 6141 7272 6179 0a20 2020 2020  .DataArray.     
+00006560: 2020 2020 2020 204e 756d 6265 7220 6f66         Number of
+00006570: 2077 6574 2064 6179 7320 2870 7220 3e3d   wet days (pr >=
+00006580: 2031 3020 6d6d 2f64 6179 292e 0a0a 2020   10 mm/day)...  
+00006590: 2020 2020 2020 4e6f 7465 730a 2020 2020        Notes.    
+000065a0: 2020 2020 2d2d 2d2d 2d0a 2020 2020 2020      -----.      
+000065b0: 2020 466f 7220 696e 666f 726d 6174 696f    For informatio
+000065c0: 6e20 6f6e 2074 6865 2069 6e70 7574 2070  n on the input p
+000065d0: 6172 616d 6574 6572 7320 7365 653a 0a20  arameters see:. 
+000065e0: 2020 2020 2020 2020 2020 2068 7474 7073             https
+000065f0: 3a2f 2f78 636c 696d 2e72 6561 6474 6865  ://xclim.readthe
+00006600: 646f 6373 2e69 6f2f 656e 2f73 7461 626c  docs.io/en/stabl
+00006610: 652f 6170 692e 6874 6d6c 2378 636c 696d  e/api.html#xclim
+00006620: 2e69 6e64 6963 6174 6f72 732e 6174 6d6f  .indicators.atmo
+00006630: 732e 7765 7464 6179 730a 2020 2020 2020  s.wetdays.      
+00006640: 2020 2222 220a 2020 2020 2020 2020 7265    """.        re
+00006650: 7475 726e 2078 632e 6174 6d6f 732e 7765  turn xc.atmos.we
+00006660: 7464 6179 7328 0a20 2020 2020 2020 2020  tdays(.         
+00006670: 2020 2074 6872 6573 683d 2231 3020 6d6d     thresh="10 mm
+00006680: 2f64 6179 222c 0a20 2020 2020 2020 2020  /day",.         
+00006690: 2020 202a 2a70 6172 616d 732c 0a20 2020     **params,.   
+000066a0: 2020 2020 2029 0a0a 0a63 6c61 7373 2052       )...class R
+000066b0: 3230 6d6d 3a0a 2020 2020 2222 224e 756d  20mm:.    """Num
+000066c0: 6265 7220 6f66 2076 6572 7920 6865 6176  ber of very heav
+000066d0: 7920 7072 6563 6970 6974 6174 696f 6e20  y precipitation 
+000066e0: 6461 7973 2028 7072 292e 2222 220a 0a20  days (pr).""".. 
+000066f0: 2020 2064 6566 2063 6f6d 7075 7465 282a     def compute(*
+00006700: 2a70 6172 616d 7329 3a0a 2020 2020 2020  *params):.      
+00006710: 2020 2222 2243 616c 6375 6c61 7465 206e    """Calculate n
+00006720: 756d 6265 7220 6f66 2077 6574 2064 6179  umber of wet day
+00006730: 7320 2870 7220 3e3d 2032 3020 6d6d 2f64  s (pr >= 20 mm/d
+00006740: 6179 292e 0a0a 2020 2020 2020 2020 5265  ay)...        Re
+00006750: 7475 726e 730a 2020 2020 2020 2020 2d2d  turns.        --
+00006760: 2d2d 2d2d 2d0a 2020 2020 2020 2020 7861  -----.        xa
+00006770: 7272 6179 2e44 6174 6141 7272 6179 0a20  rray.DataArray. 
+00006780: 2020 2020 2020 2020 2020 204e 756d 6265             Numbe
+00006790: 7220 6f66 2077 6574 2064 6179 7320 2870  r of wet days (p
+000067a0: 7220 3e3d 2032 3020 6d6d 2f64 6179 292e  r >= 20 mm/day).
+000067b0: 0a0a 2020 2020 2020 2020 4e6f 7465 730a  ..        Notes.
+000067c0: 2020 2020 2020 2020 2d2d 2d2d 2d0a 2020          -----.  
+000067d0: 2020 2020 2020 466f 7220 696e 666f 726d        For inform
+000067e0: 6174 696f 6e20 6f6e 2074 6865 2069 6e70  ation on the inp
+000067f0: 7574 2070 6172 616d 6574 6572 7320 7365  ut parameters se
+00006800: 653a 0a20 2020 2020 2020 2020 2020 2068  e:.            h
+00006810: 7474 7073 3a2f 2f78 636c 696d 2e72 6561  ttps://xclim.rea
+00006820: 6474 6865 646f 6373 2e69 6f2f 656e 2f73  dthedocs.io/en/s
+00006830: 7461 626c 652f 6170 692e 6874 6d6c 2378  table/api.html#x
+00006840: 636c 696d 2e69 6e64 6963 6174 6f72 732e  clim.indicators.
+00006850: 6174 6d6f 732e 7765 7464 6179 730a 2020  atmos.wetdays.  
+00006860: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+00006870: 2020 7265 7475 726e 2078 632e 6174 6d6f    return xc.atmo
+00006880: 732e 7765 7464 6179 7328 0a20 2020 2020  s.wetdays(.     
+00006890: 2020 2020 2020 2074 6872 6573 683d 2232         thresh="2
+000068a0: 3020 6d6d 2f64 6179 222c 0a20 2020 2020  0 mm/day",.     
+000068b0: 2020 2020 2020 202a 2a70 6172 616d 732c         **params,
+000068c0: 0a20 2020 2020 2020 2029 0a0a 0a63 6c61  .        )...cla
+000068d0: 7373 2052 3235 6d6d 3a0a 2020 2020 2222  ss R25mm:.    ""
+000068e0: 224e 756d 6265 7220 6f66 2073 7570 6572  "Number of super
+000068f0: 2068 6561 7679 2070 7265 6369 7069 7461   heavy precipita
+00006900: 7469 6f6e 2064 6179 7320 2870 7229 2e22  tion days (pr)."
+00006910: 2222 0a0a 2020 2020 6465 6620 636f 6d70  ""..    def comp
+00006920: 7574 6528 2a2a 7061 7261 6d73 293a 0a20  ute(**params):. 
+00006930: 2020 2020 2020 2022 2222 4361 6c63 756c         """Calcul
+00006940: 6174 6520 6e75 6d62 6572 206f 6620 7765  ate number of we
+00006950: 7420 6461 7973 2028 7072 203e 3d20 3235  t days (pr >= 25
+00006960: 206d 6d2f 6461 7929 2e0a 0a20 2020 2020   mm/day)...     
+00006970: 2020 2052 6574 7572 6e73 0a20 2020 2020     Returns.     
+00006980: 2020 202d 2d2d 2d2d 2d2d 0a20 2020 2020     -------.     
+00006990: 2020 2078 6172 7261 792e 4461 7461 4172     xarray.DataAr
+000069a0: 7261 790a 2020 2020 2020 2020 2020 2020  ray.            
+000069b0: 4e75 6d62 6572 206f 6620 7765 7420 6461  Number of wet da
+000069c0: 7973 2028 7072 203e 3d20 3235 206d 6d2f  ys (pr >= 25 mm/
+000069d0: 6461 7929 2e0a 0a20 2020 2020 2020 204e  day)...        N
+000069e0: 6f74 6573 0a20 2020 2020 2020 202d 2d2d  otes.        ---
+000069f0: 2d2d 0a20 2020 2020 2020 2046 6f72 2069  --.        For i
+00006a00: 6e66 6f72 6d61 7469 6f6e 206f 6e20 7468  nformation on th
+00006a10: 6520 696e 7075 7420 7061 7261 6d65 7465  e input paramete
+00006a20: 7273 2073 6565 3a0a 2020 2020 2020 2020  rs see:.        
+00006a30: 2020 2020 6874 7470 733a 2f2f 7863 6c69      https://xcli
+00006a40: 6d2e 7265 6164 7468 6564 6f63 732e 696f  m.readthedocs.io
+00006a50: 2f65 6e2f 7374 6162 6c65 2f61 7069 2e68  /en/stable/api.h
+00006a60: 746d 6c23 7863 6c69 6d2e 696e 6469 6361  tml#xclim.indica
+00006a70: 746f 7273 2e61 746d 6f73 2e77 6574 6461  tors.atmos.wetda
+00006a80: 7973 0a20 2020 2020 2020 2022 2222 0a20  ys.        """. 
+00006a90: 2020 2020 2020 2072 6574 7572 6e20 7863         return xc
+00006aa0: 2e61 746d 6f73 2e77 6574 6461 7973 280a  .atmos.wetdays(.
+00006ab0: 2020 2020 2020 2020 2020 2020 7468 7265              thre
+00006ac0: 7368 3d22 3235 206d 6d2f 6461 7922 2c0a  sh="25 mm/day",.
+00006ad0: 2020 2020 2020 2020 2020 2020 2a2a 7061              **pa
+00006ae0: 7261 6d73 2c0a 2020 2020 2020 2020 290a  rams,.        ).
+00006af0: 0a0a 636c 6173 7320 5252 5959 703a 0a20  ..class RRYYp:. 
+00006b00: 2020 2022 2222 5072 6563 6970 2070 6572     """Precip per
+00006b10: 6365 6e74 696c 2076 616c 7565 2066 6f72  centil value for
+00006b20: 2077 6574 2064 6179 7320 2870 7229 2e22   wet days (pr)."
+00006b30: 2222 0a0a 2020 2020 7065 7220 3d20 3735  ""..    per = 75
+00006b40: 0a20 2020 2074 6872 6573 6820 3d20 310a  .    thresh = 1.
+00006b50: 2020 2020 6261 7365 5f70 6572 696f 645f      base_period_
+00006b60: 7469 6d65 5f72 616e 6765 203d 2042 4153  time_range = BAS
+00006b70: 455f 5045 5249 4f44 0a0a 2020 2020 6465  E_PERIOD..    de
+00006b80: 6620 636f 6d70 7574 6528 0a20 2020 2020  f compute(.     
+00006b90: 2020 2070 6572 3d70 6572 2c0a 2020 2020     per=per,.    
+00006ba0: 2020 2020 7468 7265 7368 3d74 6872 6573      thresh=thres
+00006bb0: 682c 0a20 2020 2020 2020 2062 6173 655f  h,.        base_
+00006bc0: 7065 7269 6f64 5f74 696d 655f 7261 6e67  period_time_rang
+00006bd0: 653d 6261 7365 5f70 6572 696f 645f 7469  e=base_period_ti
+00006be0: 6d65 5f72 616e 6765 2c0a 2020 2020 2020  me_range,.      
+00006bf0: 2020 2a2a 7061 7261 6d73 2c0a 2020 2020    **params,.    
+00006c00: 293a 0a20 2020 2020 2020 2022 2222 4361  ):.        """Ca
+00006c10: 6c63 756c 6174 6520 7072 6563 6970 2070  lculate precip p
+00006c20: 6572 6365 6e74 696c 6520 7265 6665 7265  ercentile refere
+00006c30: 6e63 6520 7661 6c75 650a 2020 2020 2020  nce value.      
+00006c40: 2020 666f 7220 7765 7420 6461 7973 2028    for wet days (
+00006c50: 7072 203e 2074 6872 6573 6829 2e0a 0a20  pr > thresh)... 
+00006c60: 2020 2020 2020 2050 6172 616d 6574 6572         Parameter
+00006c70: 730a 2020 2020 2020 2020 2d2d 2d2d 2d2d  s.        ------
+00006c80: 2d2d 2d2d 0a20 2020 2020 2020 2070 6572  ----.        per
+00006c90: 3a20 696e 740a 2020 2020 2020 2020 2020  : int.          
+00006ca0: 2020 5065 7263 656e 7469 6c65 2076 616c    Percentile val
+00006cb0: 7565 2e0a 2020 2020 2020 2020 7468 7265  ue..        thre
+00006cc0: 7368 3a20 696e 7420 6f72 2073 7472 696e  sh: int or strin
+00006cd0: 670a 2020 2020 2020 2020 2020 2020 5468  g.            Th
+00006ce0: 7265 7368 6f6c 6420 7072 6563 6970 6974  reshold precipit
+00006cf0: 6174 696f 6e20 6162 6f76 6520 7768 6963  ation above whic
+00006d00: 6820 6120 6461 7920 6973 2063 6f6e 7369  h a day is consi
+00006d10: 6465 7265 640a 2020 2020 2020 2020 2020  dered.          
+00006d20: 2020 6173 2061 2077 6574 2064 6179 2028    as a wet day (
+00006d30: 6465 6661 756c 743a 2031 206d 6d2f 6461  default: 1 mm/da
+00006d40: 7929 2e0a 2020 2020 2020 2020 2020 2020  y)..            
+00006d50: 4966 2074 7970 6520 6f66 2074 6872 6573  If type of thres
+00006d60: 686f 6c64 2069 7320 616e 2069 6e74 6567  hold is an integ
+00006d70: 6572 2074 6865 2075 6e69 7420 6973 2073  er the unit is s
+00006d80: 6574 2074 6f20 6d6d 2f64 6179 2e0a 2020  et to mm/day..  
+00006d90: 2020 2020 2020 6261 7365 5f70 6572 696f        base_perio
+00006da0: 645f 7469 6d65 5f72 616e 6765 3a20 6c69  d_time_range: li
+00006db0: 7374 0a20 2020 2020 2020 2020 2020 204c  st.            L
+00006dc0: 6973 7420 7769 7468 206c 6566 7420 626f  ist with left bo
+00006dd0: 756e 6420 6973 2073 7461 7274 2079 6561  und is start yea
+00006de0: 7220 7374 7269 6e67 2061 6e64 2072 6967  r string and rig
+00006df0: 6874 2062 6f75 6e64 0a20 2020 2020 2020  ht bound.       
+00006e00: 2020 2020 2069 7320 656e 6420 7965 6172       is end year
+00006e10: 2073 7472 696e 6720 666f 7220 6361 6c63   string for calc
+00006e20: 756c 6174 696e 6720 7468 6520 7072 6563  ulating the prec
+00006e30: 6970 2070 6572 6365 6e74 696c 650a 2020  ip percentile.  
+00006e40: 2020 2020 2020 2020 2020 7265 6665 7265            refere
+00006e50: 6e63 6520 7661 6c75 652e 0a0a 2020 2020  nce value...    
+00006e60: 2020 2020 5265 7475 726e 730a 2020 2020      Returns.    
+00006e70: 2020 2020 2d2d 2d2d 2d2d 2d0a 2020 2020      -------.    
+00006e80: 2020 2020 7861 7272 6179 2e44 6174 6141      xarray.DataA
+00006e90: 7272 6179 0a20 2020 2020 2020 2020 2020  rray.           
+00006ea0: 2050 7265 6369 7020 7b70 6572 7d74 6820   Precip {per}th 
+00006eb0: 7065 7263 656e 7469 6c20 7265 6665 7265  percentil refere
+00006ec0: 6e63 6520 7661 6c75 650a 2020 2020 2020  nce value.      
+00006ed0: 2020 2020 2020 666f 7220 7765 7420 6461        for wet da
+00006ee0: 7973 2028 7072 203e 207b 7468 7265 7368  ys (pr > {thresh
+00006ef0: 7d29 2e0a 2020 2020 2020 2020 2222 220a  })..        """.
+00006f00: 2020 2020 2020 2020 7468 7265 7368 203d          thresh =
+00006f10: 205f 7468 7265 7368 5f73 7472 696e 6728   _thresh_string(
+00006f20: 7468 7265 7368 2c20 226d 6d2f 6461 7922  thresh, "mm/day"
+00006f30: 290a 2020 2020 2020 2020 6461 203d 205f  ).        da = _
+00006f40: 6765 745f 6461 2870 6172 616d 732c 2022  get_da(params, "
+00006f50: 7072 2229 0a20 2020 2020 2020 2064 6120  pr").        da 
+00006f60: 3d20 5f66 696c 7465 725f 6f75 745f 736d  = _filter_out_sm
+00006f70: 616c 6c5f 7661 6c75 6573 2864 612c 2074  all_values(da, t
+00006f80: 6872 6573 682c 2063 6f6e 7465 7874 3d22  hresh, context="
+00006f90: 6879 6472 6f22 290a 2020 2020 2020 2020  hydro").        
+00006fa0: 7265 7475 726e 205f 6765 745f 7065 7263  return _get_perc
+00006fb0: 656e 7469 6c65 280a 2020 2020 2020 2020  entile(.        
+00006fc0: 2020 2020 6461 3d64 612c 0a20 2020 2020      da=da,.     
+00006fd0: 2020 2020 2020 2070 6572 3d70 6572 2c0a         per=per,.
+00006fe0: 2020 2020 2020 2020 2020 2020 6261 7365              base
+00006ff0: 5f70 6572 696f 645f 7469 6d65 5f72 616e  _period_time_ran
+00007000: 6765 3d62 6173 655f 7065 7269 6f64 5f74  ge=base_period_t
+00007010: 696d 655f 7261 6e67 652c 0a20 2020 2020  ime_range,.     
+00007020: 2020 2029 0a0a 0a63 6c61 7373 2052 5959     )...class RYY
+00007030: 703a 0a20 2020 2022 2222 4e75 6d62 6572  p:.    """Number
+00007040: 206f 6620 7765 7420 6461 7973 2077 6974   of wet days wit
+00007050: 6820 7072 6563 6970 206f 7665 7220 6120  h precip over a 
+00007060: 6769 7665 6e20 7065 7263 656e 7469 6c65  given percentile
+00007070: 2028 7072 292e 2222 220a 0a20 2020 2070   (pr)."""..    p
+00007080: 6572 203d 2037 350a 2020 2020 7468 7265  er = 75.    thre
+00007090: 7368 203d 2031 0a20 2020 2062 6173 655f  sh = 1.    base_
+000070a0: 7065 7269 6f64 5f74 696d 655f 7261 6e67  period_time_rang
+000070b0: 6520 3d20 4241 5345 5f50 4552 494f 440a  e = BASE_PERIOD.
+000070c0: 0a20 2020 2064 6566 2063 6f6d 7075 7465  .    def compute
+000070d0: 280a 2020 2020 2020 2020 7065 723d 7065  (.        per=pe
+000070e0: 722c 0a20 2020 2020 2020 2074 6872 6573  r,.        thres
+000070f0: 683d 7468 7265 7368 2c0a 2020 2020 2020  h=thresh,.      
+00007100: 2020 6261 7365 5f70 6572 696f 645f 7469    base_period_ti
+00007110: 6d65 5f72 616e 6765 3d62 6173 655f 7065  me_range=base_pe
+00007120: 7269 6f64 5f74 696d 655f 7261 6e67 652c  riod_time_range,
+00007130: 0a20 2020 2020 2020 202a 2a70 6172 616d  .        **param
+00007140: 732c 0a20 2020 2029 3a0a 2020 2020 2020  s,.    ):.      
+00007150: 2020 2222 2243 616c 6375 6c61 7465 206e    """Calculate n
+00007160: 756d 6265 7220 6f66 2077 6574 2064 6179  umber of wet day
+00007170: 7320 2870 7220 3e20 7468 7265 7368 290a  s (pr > thresh).
+00007180: 2020 2020 2020 2020 7769 7468 2070 7265          with pre
+00007190: 6369 7020 6f76 6572 2061 2067 6976 656e  cip over a given
+000071a0: 2070 6572 6365 6e74 696c 652e 0a0a 2020   percentile...  
+000071b0: 2020 2020 2020 5061 7261 6d65 7465 7273        Parameters
+000071c0: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
+000071d0: 2d2d 2d0a 2020 2020 2020 2020 7065 723a  ---.        per:
+000071e0: 2069 6e74 0a20 2020 2020 2020 2020 2020   int.           
+000071f0: 2050 7265 6369 7069 7461 7469 6f6e 2070   Precipitation p
+00007200: 6572 6365 6e74 696c 6520 7661 6c75 652e  ercentile value.
+00007210: 0a20 2020 2020 2020 2074 6872 6573 683a  .        thresh:
+00007220: 2069 6e74 206f 7220 7374 7269 6e67 0a20   int or string. 
+00007230: 2020 2020 2020 2020 2020 2054 6872 6573             Thres
+00007240: 686f 6c64 2070 7265 6369 7069 7461 7469  hold precipitati
+00007250: 6f6e 2061 626f 7665 2077 6869 6368 2061  on above which a
+00007260: 2064 6179 2069 7320 636f 6e73 6964 6572   day is consider
+00007270: 6564 0a20 2020 2020 2020 2020 2020 2061  ed.            a
+00007280: 7320 6120 7765 7420 6461 7920 2864 6566  s a wet day (def
+00007290: 6175 6c74 3a20 3120 6d6d 2f64 6179 292e  ault: 1 mm/day).
+000072a0: 0a20 2020 2020 2020 2020 2020 2049 6620  .            If 
+000072b0: 7479 7065 206f 6620 7468 7265 7368 6f6c  type of threshol
+000072c0: 6420 6973 2061 6e20 696e 7465 6765 7220  d is an integer 
+000072d0: 7468 6520 756e 6974 2069 7320 7365 7420  the unit is set 
+000072e0: 746f 206d 6d2f 6461 792e 0a20 2020 2020  to mm/day..     
+000072f0: 2020 2062 6173 655f 7065 7269 6f64 5f74     base_period_t
+00007300: 696d 655f 7261 6e67 653a 206c 6973 740a  ime_range: list.
+00007310: 2020 2020 2020 2020 2020 2020 4c69 7374              List
+00007320: 2077 6974 6820 6c65 6674 2062 6f75 6e64   with left bound
+00007330: 2069 7320 7374 6172 7420 7965 6172 2073   is start year s
+00007340: 7472 696e 6720 616e 6420 7269 6768 7420  tring and right 
+00007350: 626f 756e 640a 2020 2020 2020 2020 2020  bound.          
+00007360: 2020 6973 2065 6e64 2079 6561 7220 7374    is end year st
+00007370: 7269 6e67 2066 6f72 2063 616c 6375 6c61  ring for calcula
+00007380: 7469 6e67 2074 6865 2070 7265 6369 700a  ting the precip.
+00007390: 2020 2020 2020 2020 2020 2020 7065 7263              perc
+000073a0: 656e 7469 6c65 2072 6566 6572 656e 6365  entile reference
+000073b0: 2076 616c 7565 2e0a 0a20 2020 2020 2020   value...       
+000073c0: 2052 6574 7572 6e73 0a20 2020 2020 2020   Returns.       
+000073d0: 202d 2d2d 2d2d 2d2d 0a20 2020 2020 2020   -------.       
+000073e0: 2078 6172 7261 792e 4461 7461 4172 7261   xarray.DataArra
+000073f0: 790a 2020 2020 2020 2020 2020 2020 4e75  y.            Nu
+00007400: 6d62 6572 206f 6620 7765 7420 6461 7973  mber of wet days
+00007410: 2028 7079 7220 3e20 7b74 6872 6573 687d   (pyr > {thresh}
+00007420: 2920 6f76 6572 2061 207b 7065 727d 7468  ) over a {per}th
+00007430: 2070 6572 6365 6e74 696c 652e 0a0a 2020   percentile...  
+00007440: 2020 2020 2020 4e6f 7465 730a 2020 2020        Notes.    
+00007450: 2020 2020 2d2d 2d2d 2d0a 2020 2020 2020      -----.      
+00007460: 2020 466f 7220 6d6f 7265 2069 6e66 6f72    For more infor
+00007470: 6d61 7469 6f6e 206f 6e20 7468 6520 696e  mation on the in
+00007480: 7075 7420 7061 7261 6d65 7465 7273 2073  put parameters s
+00007490: 6565 3a0a 2020 2020 2020 2020 2020 2020  ee:.            
+000074a0: 6874 7470 733a 2f2f 7863 6c69 6d2e 7265  https://xclim.re
+000074b0: 6164 7468 6564 6f63 732e 696f 2f65 6e2f  adthedocs.io/en/
+000074c0: 7374 6162 6c65 2f61 7069 2e68 746d 6c23  stable/api.html#
+000074d0: 7863 6c69 6d2e 696e 6469 6361 746f 7273  xclim.indicators
+000074e0: 2e61 746d 6f73 2e64 6179 735f 6f76 6572  .atmos.days_over
+000074f0: 5f70 7265 6369 705f 646f 795f 7468 7265  _precip_doy_thre
+00007500: 7368 0a20 2020 2020 2020 2022 2222 0a20  sh.        """. 
+00007510: 2020 2020 2020 2074 6872 6573 6820 3d20         thresh = 
+00007520: 5f74 6872 6573 685f 7374 7269 6e67 2874  _thresh_string(t
+00007530: 6872 6573 682c 2022 6d6d 2f64 6179 2229  hresh, "mm/day")
+00007540: 0a20 2020 2020 2020 2064 6120 3d20 5f67  .        da = _g
+00007550: 6574 5f64 6128 7061 7261 6d73 2c20 2270  et_da(params, "p
+00007560: 7222 290a 2020 2020 2020 2020 6461 5f70  r").        da_p
+00007570: 7220 3d20 5f66 696c 7465 725f 6f75 745f  r = _filter_out_
+00007580: 736d 616c 6c5f 7661 6c75 6573 2864 612c  small_values(da,
+00007590: 2074 6872 6573 682c 2063 6f6e 7465 7874   thresh, context
+000075a0: 3d22 6879 6472 6f22 290a 2020 2020 2020  ="hydro").      
+000075b0: 2020 7072 5f70 6572 203d 205f 6765 745f    pr_per = _get_
+000075c0: 7065 7263 656e 7469 6c65 280a 2020 2020  percentile(.    
+000075d0: 2020 2020 2020 2020 6461 3d64 615f 7072          da=da_pr
+000075e0: 2c0a 2020 2020 2020 2020 2020 2020 7065  ,.            pe
+000075f0: 723d 7065 722c 0a20 2020 2020 2020 2020  r=per,.         
+00007600: 2020 2062 6173 655f 7065 7269 6f64 5f74     base_period_t
+00007610: 696d 655f 7261 6e67 653d 6261 7365 5f70  ime_range=base_p
+00007620: 6572 696f 645f 7469 6d65 5f72 616e 6765  eriod_time_range
+00007630: 2c0a 2020 2020 2020 2020 290a 2020 2020  ,.        ).    
+00007640: 2020 2020 7265 7475 726e 2078 632e 6174      return xc.at
+00007650: 6d6f 732e 6461 7973 5f6f 7665 725f 7072  mos.days_over_pr
+00007660: 6563 6970 5f64 6f79 5f74 6872 6573 6828  ecip_doy_thresh(
+00007670: 0a20 2020 2020 2020 2020 2020 2070 725f  .            pr_
+00007680: 7065 723d 7072 5f70 6572 2c0a 2020 2020  per=pr_per,.    
+00007690: 2020 2020 2020 2020 2a2a 7061 7261 6d73          **params
+000076a0: 2c0a 2020 2020 2020 2020 290a 0a0a 636c  ,.        )...cl
+000076b0: 6173 7320 5259 596d 6d3a 0a20 2020 2022  ass RYYmm:.    "
+000076c0: 2222 4e75 6d62 6572 206f 6620 6461 7973  ""Number of days
+000076d0: 2077 6974 6820 7072 6563 6970 206f 7665   with precip ove
+000076e0: 7220 7468 7265 7368 6f6c 6420 2870 7229  r threshold (pr)
+000076f0: 2e22 2222 0a0a 2020 2020 7468 7265 7368  ."""..    thresh
+00007700: 203d 2032 350a 0a20 2020 2064 6566 2063   = 25..    def c
+00007710: 6f6d 7075 7465 2874 6872 6573 683d 7468  ompute(thresh=th
+00007720: 7265 7368 2c20 2a2a 7061 7261 6d73 293a  resh, **params):
+00007730: 0a20 2020 2020 2020 2022 2222 4361 6c63  .        """Calc
+00007740: 756c 6174 6520 6e75 6d62 6572 206f 6620  ulate number of 
+00007750: 7765 7420 6461 7973 2e0a 0a20 2020 2020  wet days...     
+00007760: 2020 2050 6172 616d 6574 6572 730a 2020     Parameters.  
+00007770: 2020 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d        ----------
+00007780: 0a20 2020 2020 2020 2074 6872 6573 683a  .        thresh:
+00007790: 0a20 2020 2020 2020 2054 6872 6573 686f  .        Thresho
+000077a0: 6c64 2070 7265 6369 7069 7461 7469 6f6e  ld precipitation
+000077b0: 2061 626f 7665 2077 6869 6368 2061 2064   above which a d
+000077c0: 6179 2069 7320 636f 6e73 6964 6572 6564  ay is considered
+000077d0: 0a20 2020 2020 2020 2020 2020 2061 7320  .            as 
+000077e0: 6120 7765 7420 6461 7928 6465 6661 756c  a wet day(defaul
+000077f0: 743a 2032 3520 6d6d 2f64 6179 292e 0a20  t: 25 mm/day).. 
+00007800: 2020 2020 2020 2020 2020 2049 6620 7479             If ty
+00007810: 7065 206f 6620 7468 7265 7368 6f6c 6420  pe of threshold 
+00007820: 6973 2061 6e20 696e 7465 6765 7220 7468  is an integer th
+00007830: 6520 756e 6974 2069 7320 7365 7420 746f  e unit is set to
+00007840: 206d 6d2f 6461 792e 0a0a 2020 2020 2020   mm/day...      
+00007850: 2020 5265 7475 726e 730a 2020 2020 2020    Returns.      
+00007860: 2020 2d2d 2d2d 2d2d 2d0a 2020 2020 2020    -------.      
+00007870: 2020 7861 7272 6179 2e44 6174 6141 7272    xarray.DataArr
+00007880: 6179 0a20 2020 2020 2020 2020 2020 204e  ay.            N
+00007890: 756d 6265 7220 6f66 2077 6574 2064 6179  umber of wet day
+000078a0: 7320 2870 7220 3e20 7b74 6872 6573 687d  s (pr > {thresh}
+000078b0: 292e 0a0a 2020 2020 2020 2020 4e6f 7465  )...        Note
+000078c0: 730a 2020 2020 2020 2020 2d2d 2d2d 2d0a  s.        -----.
+000078d0: 2020 2020 2020 2020 466f 7220 6d6f 7265          For more
+000078e0: 2069 6e66 6f72 6d61 7469 6f6e 206f 6e20   information on 
+000078f0: 7468 6520 696e 7075 7420 7061 7261 6d65  the input parame
+00007900: 7465 7273 2073 6565 3a0a 2020 2020 2020  ters see:.      
+00007910: 2020 2020 2020 6874 7470 733a 2f2f 7863        https://xc
+00007920: 6c69 6d2e 7265 6164 7468 6564 6f63 732e  lim.readthedocs.
+00007930: 696f 2f65 6e2f 7374 6162 6c65 2f61 7069  io/en/stable/api
+00007940: 2e68 746d 6c23 7863 6c69 6d2e 696e 6469  .html#xclim.indi
+00007950: 6361 746f 7273 2e61 746d 6f73 2e77 6574  cators.atmos.wet
+00007960: 6461 7973 0a20 2020 2020 2020 2022 2222  days.        """
+00007970: 0a20 2020 2020 2020 2074 6872 6573 6820  .        thresh 
+00007980: 3d20 5f74 6872 6573 685f 7374 7269 6e67  = _thresh_string
+00007990: 2874 6872 6573 682c 2022 6d6d 2f64 6179  (thresh, "mm/day
+000079a0: 2229 0a20 2020 2020 2020 2072 6574 7572  ").        retur
+000079b0: 6e20 7863 2e61 746d 6f73 2e77 6574 6461  n xc.atmos.wetda
+000079c0: 7973 280a 2020 2020 2020 2020 2020 2020  ys(.            
+000079d0: 7468 7265 7368 3d74 6872 6573 682c 0a20  thresh=thresh,. 
+000079e0: 2020 2020 2020 2020 2020 202a 2a70 6172             **par
+000079f0: 616d 732c 0a20 2020 2020 2020 2029 0a0a  ams,.        )..
+00007a00: 0a63 6c61 7373 2052 5831 6461 793a 0a20  .class RX1day:. 
+00007a10: 2020 2022 2222 4d61 7869 6d75 6d20 312d     """Maximum 1-
+00007a20: 6461 7920 746f 7461 6c20 7072 6563 6970  day total precip
+00007a30: 6974 6174 696f 6e20 2870 7229 2e22 2222  itation (pr)."""
+00007a40: 0a0a 2020 2020 6465 6620 636f 6d70 7574  ..    def comput
+00007a50: 6528 2a2a 7061 7261 6d73 293a 0a20 2020  e(**params):.   
+00007a60: 2020 2020 2022 2222 4361 6c63 756c 6174       """Calculat
+00007a70: 6520 6d61 7869 6d75 6d20 312d 6461 7920  e maximum 1-day 
+00007a80: 746f 7461 6c20 7072 6563 6970 6974 6174  total precipitat
+00007a90: 696f 6e2e 0a0a 2020 2020 2020 2020 5265  ion...        Re
+00007aa0: 7475 726e 730a 2020 2020 2020 2020 2d2d  turns.        --
+00007ab0: 2d2d 2d2d 2d0a 2020 2020 2020 2020 7861  -----.        xa
+00007ac0: 7272 6179 2e44 6174 6141 7272 6179 0a20  rray.DataArray. 
+00007ad0: 2020 2020 2020 2020 2020 204d 6178 696d             Maxim
+00007ae0: 756d 2031 2d64 6179 2074 6f74 616c 2070  um 1-day total p
+00007af0: 7265 6369 7069 7461 7469 6f6e 2e0a 0a20  recipitation... 
+00007b00: 2020 2020 2020 204e 6f74 6573 0a20 2020         Notes.   
+00007b10: 2020 2020 202d 2d2d 2d2d 0a20 2020 2020       -----.     
+00007b20: 2020 2046 6f72 2069 6e66 6f72 6d61 7469     For informati
+00007b30: 6f6e 206f 6e20 7468 6520 696e 7075 7420  on on the input 
+00007b40: 7061 7261 6d65 7465 7273 2073 6565 3a0a  parameters see:.
+00007b50: 2020 2020 2020 2020 2020 2020 6874 7470              http
+00007b60: 733a 2f2f 7863 6c69 6d2e 7265 6164 7468  s://xclim.readth
+00007b70: 6564 6f63 732e 696f 2f65 6e2f 7374 6162  edocs.io/en/stab
+00007b80: 6c65 2f61 7069 2e68 746d 6c23 7863 6c69  le/api.html#xcli
+00007b90: 6d2e 696e 6469 6361 746f 7273 2e61 746d  m.indicators.atm
+00007ba0: 6f73 2e6d 6178 5f31 6461 795f 7072 6563  os.max_1day_prec
+00007bb0: 6970 6974 6174 696f 6e5f 616d 6f75 6e74  ipitation_amount
+00007bc0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00007bd0: 2020 2020 2072 6574 7572 6e20 7863 2e61       return xc.a
+00007be0: 746d 6f73 2e6d 6178 5f31 6461 795f 7072  tmos.max_1day_pr
+00007bf0: 6563 6970 6974 6174 696f 6e5f 616d 6f75  ecipitation_amou
+00007c00: 6e74 282a 2a70 6172 616d 7329 0a0a 0a63  nt(**params)...c
+00007c10: 6c61 7373 2052 5859 5964 6179 3a0a 2020  lass RXYYday:.  
+00007c20: 2020 2222 224d 6178 696d 756d 206e 2d64    """Maximum n-d
+00007c30: 6179 2074 6f74 616c 2070 7265 6369 7069  ay total precipi
+00007c40: 7461 7469 6f6e 2028 7072 292e 2222 220a  tation (pr).""".
+00007c50: 0a20 2020 2077 696e 646f 7720 3d20 350a  .    window = 5.
+00007c60: 0a20 2020 2064 6566 2063 6f6d 7075 7465  .    def compute
+00007c70: 2877 696e 646f 773d 7769 6e64 6f77 2c20  (window=window, 
+00007c80: 2a2a 7061 7261 6d73 293a 0a20 2020 2020  **params):.     
+00007c90: 2020 2022 2222 4361 6c63 756c 6174 6520     """Calculate 
+00007ca0: 6d61 7869 6d75 6d20 7b77 696e 646f 777d  maximum {window}
+00007cb0: 2d64 6179 2074 6f74 616c 2070 7265 6369  -day total preci
+00007cc0: 7069 7461 7469 6f6e 2e0a 0a20 2020 2020  pitation...     
+00007cd0: 2020 2050 6172 616d 6574 6572 730a 2020     Parameters.  
+00007ce0: 2020 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d        ----------
+00007cf0: 0a20 2020 2020 2020 2077 696e 646f 773a  .        window:
+00007d00: 2069 6e74 0a20 2020 2020 2020 2020 2020   int.           
+00007d10: 2057 696e 646f 7720 7369 7a65 2069 6e20   Window size in 
+00007d20: 6461 7973 2e0a 0a20 2020 2020 2020 2052  days...        R
+00007d30: 6574 7572 6e73 0a20 2020 2020 2020 202d  eturns.        -
+00007d40: 2d2d 2d2d 2d2d 0a20 2020 2020 2020 2078  ------.        x
+00007d50: 6172 7261 792e 4461 7461 4172 7261 790a  array.DataArray.
+00007d60: 2020 2020 2020 2020 2020 2020 4d61 7869              Maxi
+00007d70: 6d75 6d20 7b77 696e 646f 777d 2d64 6179  mum {window}-day
+00007d80: 2074 6f74 616c 2070 7265 6369 7069 7461   total precipita
+00007d90: 7469 6f6e 2e0a 0a20 2020 2020 2020 204e  tion...        N
+00007da0: 6f74 6573 0a20 2020 2020 2020 202d 2d2d  otes.        ---
+00007db0: 2d2d 0a20 2020 2020 2020 2046 6f72 206d  --.        For m
+00007dc0: 6f72 6520 696e 666f 726d 6174 696f 6e20  ore information 
+00007dd0: 6f6e 2074 6865 2069 6e70 7574 2070 6172  on the input par
+00007de0: 616d 6574 6572 7320 7365 653a 0a20 2020  ameters see:.   
+00007df0: 2020 2020 2020 2020 2068 7474 7073 3a2f           https:/
+00007e00: 2f78 636c 696d 2e72 6561 6474 6865 646f  /xclim.readthedo
+00007e10: 6373 2e69 6f2f 656e 2f73 7461 626c 652f  cs.io/en/stable/
+00007e20: 6170 692e 6874 6d6c 2378 636c 696d 2e69  api.html#xclim.i
+00007e30: 6e64 6963 6174 6f72 732e 6174 6d6f 732e  ndicators.atmos.
+00007e40: 6d61 785f 6e5f 6461 795f 7072 6563 6970  max_n_day_precip
+00007e50: 6974 6174 696f 6e5f 616d 6f75 6e74 0a20  itation_amount. 
+00007e60: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00007e70: 2020 2072 6574 7572 6e20 7863 2e61 746d     return xc.atm
+00007e80: 6f73 2e6d 6178 5f6e 5f64 6179 5f70 7265  os.max_n_day_pre
+00007e90: 6369 7069 7461 7469 6f6e 5f61 6d6f 756e  cipitation_amoun
+00007ea0: 7428 0a20 2020 2020 2020 2020 2020 2077  t(.            w
+00007eb0: 696e 646f 773d 7769 6e64 6f77 2c0a 2020  indow=window,.  
+00007ec0: 2020 2020 2020 2020 2020 2a2a 7061 7261            **para
+00007ed0: 6d73 2c0a 2020 2020 2020 2020 290a 0a0a  ms,.        )...
+00007ee0: 636c 6173 7320 5259 5970 4142 533a 0a20  class RYYpABS:. 
+00007ef0: 2020 2022 2222 546f 7461 6c20 7072 6563     """Total prec
+00007f00: 6970 6974 6174 696f 6e20 616d 6f75 6e74  ipitation amount
+00007f10: 2077 6974 6820 7072 6563 6970 2061 626f   with precip abo
+00007f20: 7665 2070 6572 6365 6e74 696c 650a 2020  ve percentile.  
+00007f30: 2020 6f6e 2077 6574 2064 6179 7320 2870    on wet days (p
+00007f40: 7229 2e22 2222 0a0a 2020 2020 7065 7220  r)."""..    per 
+00007f50: 3d20 3735 0a20 2020 2074 6872 6573 6820  = 75.    thresh 
+00007f60: 3d20 310a 2020 2020 6261 7365 5f70 6572  = 1.    base_per
+00007f70: 696f 645f 7469 6d65 5f72 616e 6765 203d  iod_time_range =
+00007f80: 2042 4153 455f 5045 5249 4f44 0a0a 2020   BASE_PERIOD..  
+00007f90: 2020 6465 6620 636f 6d70 7574 6528 0a20    def compute(. 
+00007fa0: 2020 2020 2020 2070 6572 3d70 6572 2c0a         per=per,.
+00007fb0: 2020 2020 2020 2020 7468 7265 7368 3d74          thresh=t
+00007fc0: 6872 6573 682c 0a20 2020 2020 2020 2062  hresh,.        b
+00007fd0: 6173 655f 7065 7269 6f64 5f74 696d 655f  ase_period_time_
+00007fe0: 7261 6e67 653d 6261 7365 5f70 6572 696f  range=base_perio
+00007ff0: 645f 7469 6d65 5f72 616e 6765 2c0a 2020  d_time_range,.  
+00008000: 2020 2020 2020 2a2a 7061 7261 6d73 2c0a        **params,.
+00008010: 2020 2020 293a 0a20 2020 2020 2020 2022      ):.        "
+00008020: 2222 4361 6c63 756c 6174 6520 746f 7461  ""Calculate tota
+00008030: 6c20 7072 6563 6970 6974 6174 696f 6e20  l precipitation 
+00008040: 616d 6f75 6e74 2077 6974 680a 2020 2020  amount with.    
+00008050: 2020 2020 7072 6563 6970 203e 207b 7065      precip > {pe
+00008060: 7263 7d74 6820 7065 7263 656e 7469 6c65  rc}th percentile
+00008070: 206f 6e20 7765 7420 6461 7973 2028 7072   on wet days (pr
+00008080: 203e 2074 6872 6573 6829 2e0a 0a20 2020   > thresh)...   
+00008090: 2020 2020 2050 6172 616d 6574 6572 730a       Parameters.
+000080a0: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d2d          --------
+000080b0: 2d2d 0a20 2020 2020 2020 2070 6572 3a20  --.        per: 
+000080c0: 696e 740a 2020 2020 2020 2020 2020 2020  int.            
+000080d0: 5065 7263 656e 7469 6c65 2076 616c 7565  Percentile value
+000080e0: 2e0a 2020 2020 2020 2020 7468 7265 7368  ..        thresh
+000080f0: 3a20 696e 7420 6f72 2073 7472 696e 670a  : int or string.
+00008100: 2020 2020 2020 2020 2020 2020 5468 7265              Thre
+00008110: 7368 6f6c 6420 7072 6563 6970 6974 6174  shold precipitat
+00008120: 696f 6e20 6162 6f76 6520 7768 6963 6820  ion above which 
+00008130: 6120 6461 7920 6973 2063 6f6e 7369 6465  a day is conside
+00008140: 7265 640a 2020 2020 2020 2020 2020 2020  red.            
+00008150: 6173 2061 2077 6574 2064 6179 2028 6465  as a wet day (de
+00008160: 6661 756c 743a 2031 206d 6d2f 6461 7929  fault: 1 mm/day)
+00008170: 2e0a 2020 2020 2020 2020 2020 2020 4966  ..            If
+00008180: 2074 7970 6520 6f66 2074 6872 6573 686f   type of thresho
+00008190: 6c64 2069 7320 616e 2069 6e74 6567 6572  ld is an integer
+000081a0: 2074 6865 2075 6e69 7420 6973 2073 6574   the unit is set
+000081b0: 2074 6f20 6d6d 2f64 6179 2e0a 2020 2020   to mm/day..    
+000081c0: 2020 2020 6261 7365 5f70 6572 696f 645f      base_period_
+000081d0: 7469 6d65 5f72 616e 6765 3a20 6c69 7374  time_range: list
+000081e0: 0a20 2020 2020 2020 2020 2020 204c 6973  .            Lis
+000081f0: 7420 7769 7468 206c 6566 7420 626f 756e  t with left boun
+00008200: 6420 6973 2073 7461 7274 2079 6561 7220  d is start year 
+00008210: 7374 7269 6e67 2061 6e64 2072 6967 6874  string and right
+00008220: 2062 6f75 6e64 0a20 2020 2020 2020 2020   bound.         
+00008230: 2020 2069 7320 656e 6420 7965 6172 2073     is end year s
+00008240: 7472 696e 6720 666f 7220 6361 6c75 6c61  tring for calula
+00008250: 7469 6e67 2074 6865 2070 7265 6369 7020  ting the precip 
+00008260: 7065 7263 656e 7469 6c65 0a20 2020 2020  percentile.     
+00008270: 2020 2020 2020 2072 6566 6572 656e 6365         reference
+00008280: 2076 616c 7565 2e0a 0a20 2020 2020 2020   value...       
+00008290: 2052 6574 7572 6e73 0a20 2020 2020 2020   Returns.       
+000082a0: 202d 2d2d 2d2d 2d2d 0a20 2020 2020 2020   -------.       
+000082b0: 2078 6172 7261 792e 4461 7461 4172 7261   xarray.DataArra
+000082c0: 790a 2020 2020 2020 2020 2020 2020 5072  y.            Pr
+000082d0: 6563 6970 6974 6174 696f 6e20 6672 6163  ecipitation frac
+000082e0: 7469 6f6e 2077 6974 6820 7072 6563 6970  tion with precip
+000082f0: 203e 207b 7065 7263 7d74 6820 7065 7263   > {perc}th perc
+00008300: 656e 7469 6c65 0a20 2020 2020 2020 2020  entile.         
+00008310: 2020 206f 6e20 7765 7420 6461 7973 2028     on wet days (
+00008320: 7072 203e 207b 7468 7265 7368 7d29 2e0a  pr > {thresh})..
+00008330: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00008340: 2020 2020 7468 7265 7368 203d 205f 7468      thresh = _th
+00008350: 7265 7368 5f73 7472 696e 6728 7468 7265  resh_string(thre
+00008360: 7368 2c20 226d 6d2f 6461 7922 290a 2020  sh, "mm/day").  
+00008370: 2020 2020 2020 6461 203d 205f 6765 745f        da = _get_
+00008380: 6461 2870 6172 616d 732c 2022 7072 2229  da(params, "pr")
+00008390: 0a20 2020 2020 2020 2064 615f 7072 203d  .        da_pr =
+000083a0: 205f 6669 6c74 6572 5f6f 7574 5f73 6d61   _filter_out_sma
+000083b0: 6c6c 5f76 616c 7565 7328 6461 2c20 7468  ll_values(da, th
+000083c0: 7265 7368 2c20 636f 6e74 6578 743d 2268  resh, context="h
+000083d0: 7964 726f 2229 0a20 2020 2020 2020 2070  ydro").        p
+000083e0: 725f 7065 7220 3d20 5f67 6574 5f70 6572  r_per = _get_per
+000083f0: 6365 6e74 696c 6528 0a20 2020 2020 2020  centile(.       
+00008400: 2020 2020 2064 613d 6461 5f70 722c 0a20       da=da_pr,. 
+00008410: 2020 2020 2020 2020 2020 2070 6572 3d70             per=p
+00008420: 6572 2c0a 2020 2020 2020 2020 2020 2020  er,.            
+00008430: 6261 7365 5f70 6572 696f 645f 7469 6d65  base_period_time
+00008440: 5f72 616e 6765 3d62 6173 655f 7065 7269  _range=base_peri
+00008450: 6f64 5f74 696d 655f 7261 6e67 652c 0a20  od_time_range,. 
+00008460: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+00008470: 2077 6974 6820 6461 736b 2e63 6f6e 6669   with dask.confi
+00008480: 672e 7365 7428 2a2a 7b22 6172 7261 792e  g.set(**{"array.
+00008490: 736c 6963 696e 672e 7370 6c69 745f 6c61  slicing.split_la
+000084a0: 7267 655f 6368 756e 6b73 223a 2046 616c  rge_chunks": Fal
+000084b0: 7365 7d29 3a0a 2020 2020 2020 2020 2020  se}):.          
+000084c0: 2020 7072 5f70 6572 203d 2063 6f6e 7665    pr_per = conve
+000084d0: 7274 5f75 6e69 7473 5f74 6f28 7072 5f70  rt_units_to(pr_p
+000084e0: 6572 2c20 6461 2c20 636f 6e74 6578 743d  er, da, context=
+000084f0: 2268 7964 726f 2229 0a20 2020 2020 2020  "hydro").       
+00008500: 2020 2020 2074 6872 6573 6820 3d20 636f       thresh = co
+00008510: 6e76 6572 745f 756e 6974 735f 746f 2874  nvert_units_to(t
+00008520: 6872 6573 682c 2064 612c 2063 6f6e 7465  hresh, da, conte
+00008530: 7874 3d22 6879 6472 6f22 290a 0a20 2020  xt="hydro")..   
+00008540: 2020 2020 2020 2020 2074 7020 3d20 7072           tp = pr
+00008550: 5f70 6572 2e77 6865 7265 2870 725f 7065  _per.where(pr_pe
+00008560: 7220 3e20 7468 7265 7368 2c20 7468 7265  r > thresh, thre
+00008570: 7368 290a 2020 2020 2020 2020 2020 2020  sh).            
+00008580: 6966 2022 6461 796f 6679 6561 7222 2069  if "dayofyear" i
+00008590: 6e20 7072 5f70 6572 2e63 6f6f 7264 733a  n pr_per.coords:
+000085a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000085b0: 2023 2043 7265 6174 6520 7469 6d65 2073   # Create time s
+000085c0: 6572 6965 7320 6f75 7420 6f66 2064 6f79  eries out of doy
+000085d0: 2076 616c 7565 732e 0a20 2020 2020 2020   values..       
+000085e0: 2020 2020 2020 2020 2074 7020 3d20 7265           tp = re
+000085f0: 7361 6d70 6c65 5f64 6f79 2874 702c 2064  sample_doy(tp, d
+00008600: 6129 0a0a 2020 2020 2020 2020 2020 2020  a)..            
+00008610: 636f 6e73 7472 6169 6e20 3d20 2822 3e22  constrain = (">"
+00008620: 2c20 223e 3d22 290a 0a20 2020 2020 2020  , ">=")..       
+00008630: 2020 2020 2023 2043 6f6d 7075 7465 2074       # Compute t
+00008640: 6865 2064 6179 7320 7768 656e 2070 7265  he days when pre
+00008650: 6369 7020 6973 2062 6f74 6820 6f76 6572  cip is both over
+00008660: 2074 6865 2077 6574 2064 6179 2074 6872   the wet day thr
+00008670: 6573 686f 6c64 0a20 2020 2020 2020 2020  eshold.         
+00008680: 2020 2023 2061 6e64 2074 6865 2070 6572     # and the per
+00008690: 6365 6e74 696c 6520 7468 7265 7368 6f6c  centile threshol
+000086a0: 642e 0a20 2020 2020 2020 2020 2020 206f  d..            o
+000086b0: 7665 7220 3d20 280a 2020 2020 2020 2020  ver = (.        
+000086c0: 2020 2020 2020 2020 6461 2e77 6865 7265          da.where
+000086d0: 2863 6f6d 7061 7265 2864 612c 2022 3e22  (compare(da, ">"
+000086e0: 2c20 7470 2c20 636f 6e73 7472 6169 6e29  , tp, constrain)
+000086f0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00008700: 2020 2e72 6573 616d 706c 6528 7469 6d65    .resample(time
+00008710: 3d70 6172 616d 735b 2266 7265 7122 5d29  =params["freq"])
+00008720: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00008730: 202e 7375 6d28 6469 6d3d 2274 696d 6522   .sum(dim="time"
+00008740: 290a 2020 2020 2020 2020 2020 2020 290a  ).            ).
+00008750: 2020 2020 2020 2020 2020 2020 6f75 7420              out 
+00008760: 3d20 636f 6e76 6572 745f 756e 6974 735f  = convert_units_
+00008770: 746f 286f 7665 722c 2022 6d6d 2f64 6179  to(over, "mm/day
+00008780: 2229 0a20 2020 2020 2020 2020 2020 206f  ").            o
+00008790: 7574 2e61 7474 7273 5b22 756e 6974 7322  ut.attrs["units"
+000087a0: 5d20 3d20 226d 6d22 0a20 2020 2020 2020  ] = "mm".       
+000087b0: 2020 2020 2072 6574 7572 6e20 6f75 740a       return out.
+000087c0: 0a0a 636c 6173 7320 5259 5970 544f 543a  ..class RYYpTOT:
+000087d0: 0a20 2020 2022 2222 5072 6563 6970 6974  .    """Precipit
+000087e0: 6174 696f 6e20 6672 6163 7469 6f6e 2077  ation fraction w
+000087f0: 6974 6820 7072 6563 6970 2061 626f 7665  ith precip above
+00008800: 2070 6572 6365 6e74 696c 6520 6f6e 2077   percentile on w
+00008810: 6574 2064 6179 7320 2870 7229 2e22 2222  et days (pr)."""
+00008820: 0a0a 2020 2020 7065 7220 3d20 3735 0a20  ..    per = 75. 
+00008830: 2020 2074 6872 6573 6820 3d20 310a 2020     thresh = 1.  
+00008840: 2020 6261 7365 5f70 6572 696f 645f 7469    base_period_ti
+00008850: 6d65 5f72 616e 6765 203d 2042 4153 455f  me_range = BASE_
+00008860: 5045 5249 4f44 0a0a 2020 2020 6465 6620  PERIOD..    def 
+00008870: 636f 6d70 7574 6528 0a20 2020 2020 2020  compute(.       
+00008880: 2070 6572 3d70 6572 2c0a 2020 2020 2020   per=per,.      
+00008890: 2020 7468 7265 7368 3d74 6872 6573 682c    thresh=thresh,
+000088a0: 0a20 2020 2020 2020 2062 6173 655f 7065  .        base_pe
+000088b0: 7269 6f64 5f74 696d 655f 7261 6e67 653d  riod_time_range=
+000088c0: 6261 7365 5f70 6572 696f 645f 7469 6d65  base_period_time
+000088d0: 5f72 616e 6765 2c0a 2020 2020 2020 2020  _range,.        
+000088e0: 2a2a 7061 7261 6d73 2c0a 2020 2020 293a  **params,.    ):
+000088f0: 0a20 2020 2020 2020 2022 2222 4361 6c63  .        """Calc
+00008900: 756c 6174 6520 7072 6563 6970 6974 6174  ulate precipitat
+00008910: 696f 6e20 6672 6163 7469 6f6e 2077 6974  ion fraction wit
+00008920: 6820 7072 6563 6970 2061 626f 7665 2070  h precip above p
+00008930: 6572 6365 6e74 696c 650a 2020 2020 2020  ercentile.      
+00008940: 2020 6f6e 2077 6574 2064 6179 7320 2870    on wet days (p
+00008950: 7220 3e20 7468 7265 7368 292e 0a0a 2020  r > thresh)...  
+00008960: 2020 2020 2020 5061 7261 6d65 7465 7273        Parameters
+00008970: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
+00008980: 2d2d 2d0a 2020 2020 2020 2020 7065 723a  ---.        per:
+00008990: 2069 6e74 0a20 2020 2020 2020 2020 2020   int.           
+000089a0: 2050 6572 6365 6e74 696c 6520 7661 6c75   Percentile valu
+000089b0: 652e 0a20 2020 2020 2020 2074 6872 6573  e..        thres
+000089c0: 683a 2069 6e74 206f 7220 7374 7269 6e67  h: int or string
+000089d0: 0a20 2020 2020 2020 2020 2020 2054 6872  .            Thr
+000089e0: 6573 686f 6c64 2070 7265 6369 7069 7461  eshold precipita
+000089f0: 7469 6f6e 2061 626f 7665 2077 6869 6368  tion above which
+00008a00: 2061 2064 6179 2069 7320 636f 6e73 6964   a day is consid
+00008a10: 6572 6564 0a20 2020 2020 2020 2020 2020  ered.           
+00008a20: 2061 7320 6120 7765 7420 6461 7920 2864   as a wet day (d
+00008a30: 6566 6175 6c74 3a20 3120 6d6d 2f64 6179  efault: 1 mm/day
+00008a40: 292e 0a20 2020 2020 2020 2020 2020 2049  )..            I
+00008a50: 6620 7479 7065 206f 6620 7468 7265 7368  f type of thresh
+00008a60: 6f6c 6420 6973 2061 6e20 696e 7465 6765  old is an intege
+00008a70: 7220 7468 6520 756e 6974 2069 7320 7365  r the unit is se
+00008a80: 7420 746f 206d 6d2f 6461 792e 0a20 2020  t to mm/day..   
+00008a90: 2020 2020 2062 6173 655f 7065 7269 6f64       base_period
+00008aa0: 5f74 696d 655f 7261 6e67 653a 206c 6973  _time_range: lis
+00008ab0: 740a 2020 2020 2020 2020 2020 2020 4c69  t.            Li
+00008ac0: 7374 2077 6974 6820 6c65 6674 2062 6f75  st with left bou
+00008ad0: 6e64 2069 7320 7374 6172 7420 7965 6172  nd is start year
+00008ae0: 2073 7472 696e 6720 616e 6420 7269 6768   string and righ
+00008af0: 7420 626f 756e 640a 2020 2020 2020 2020  t bound.        
+00008b00: 2020 2020 6973 2065 6e64 2079 6561 7220      is end year 
+00008b10: 7374 7269 6e67 2066 6f72 2063 616c 756c  string for calul
+00008b20: 6174 696e 6720 7468 6520 7072 6563 6970  ating the precip
+00008b30: 2070 6572 6365 6e74 696c 650a 2020 2020   percentile.    
+00008b40: 2020 2020 2020 2020 7265 6665 7265 6e63          referenc
+00008b50: 6520 7661 6c75 652e 0a0a 2020 2020 2020  e value...      
+00008b60: 2020 5265 7475 726e 730a 2020 2020 2020    Returns.      
+00008b70: 2020 2d2d 2d2d 2d2d 2d0a 2020 2020 2020    -------.      
+00008b80: 2020 7861 7272 6179 2e44 6174 6141 7272    xarray.DataArr
+00008b90: 6179 0a20 2020 2020 2020 2020 2020 2050  ay.            P
+00008ba0: 7265 6369 7069 7461 7469 6f6e 2066 7261  recipitation fra
+00008bb0: 6374 696f 6e20 7769 7468 2070 7265 6369  ction with preci
+00008bc0: 7020 3e20 7b70 6572 637d 7468 2070 6572  p > {perc}th per
+00008bd0: 6365 6e74 696c 650a 2020 2020 2020 2020  centile.        
+00008be0: 2020 2020 6f6e 2077 6574 2064 6179 7320      on wet days 
+00008bf0: 2870 7220 3e20 7b74 6872 6573 687d 292e  (pr > {thresh}).
+00008c00: 0a0a 2020 2020 2020 2020 4e6f 7465 730a  ..        Notes.
+00008c10: 2020 2020 2020 2020 2d2d 2d2d 2d0a 2020          -----.  
+00008c20: 2020 2020 2020 466f 7220 6d6f 7265 2069        For more i
+00008c30: 6e66 6f72 6d61 7469 6f6e 206f 6e20 7468  nformation on th
+00008c40: 6520 696e 7075 7420 7061 7261 6d65 7465  e input paramete
+00008c50: 7273 2073 6565 3a0a 2020 2020 2020 2020  rs see:.        
+00008c60: 2020 2020 6874 7470 733a 2f2f 7863 6c69      https://xcli
+00008c70: 6d2e 7265 6164 7468 6564 6f63 732e 696f  m.readthedocs.io
+00008c80: 2f65 6e2f 7374 6162 6c65 2f61 7069 2e68  /en/stable/api.h
+00008c90: 746d 6c23 7863 6c69 6d2e 696e 6469 6361  tml#xclim.indica
+00008ca0: 746f 7273 2e61 746d 6f73 2e66 7261 6374  tors.atmos.fract
+00008cb0: 696f 6e5f 6f76 6572 5f70 7265 6369 705f  ion_over_precip_
+00008cc0: 7468 7265 7368 0a20 2020 2020 2020 2022  thresh.        "
+00008cd0: 2222 0a20 2020 2020 2020 2074 6872 6573  "".        thres
+00008ce0: 6820 3d20 5f74 6872 6573 685f 7374 7269  h = _thresh_stri
+00008cf0: 6e67 2874 6872 6573 682c 2022 6d6d 2f64  ng(thresh, "mm/d
+00008d00: 6179 2229 0a20 2020 2020 2020 2064 6120  ay").        da 
+00008d10: 3d20 5f67 6574 5f64 6128 7061 7261 6d73  = _get_da(params
+00008d20: 2c20 2270 7222 290a 2020 2020 2020 2020  , "pr").        
+00008d30: 6461 5f70 7220 3d20 5f66 696c 7465 725f  da_pr = _filter_
+00008d40: 6f75 745f 736d 616c 6c5f 7661 6c75 6573  out_small_values
+00008d50: 2864 612c 2074 6872 6573 682c 2063 6f6e  (da, thresh, con
+00008d60: 7465 7874 3d22 6879 6472 6f22 290a 2020  text="hydro").  
+00008d70: 2020 2020 2020 7072 5f70 6572 203d 205f        pr_per = _
+00008d80: 6765 745f 7065 7263 656e 7469 6c65 280a  get_percentile(.
+00008d90: 2020 2020 2020 2020 2020 2020 6461 3d64              da=d
+00008da0: 615f 7072 2c0a 2020 2020 2020 2020 2020  a_pr,.          
+00008db0: 2020 7065 723d 7065 722c 0a20 2020 2020    per=per,.     
+00008dc0: 2020 2020 2020 2062 6173 655f 7065 7269         base_peri
+00008dd0: 6f64 5f74 696d 655f 7261 6e67 653d 6261  od_time_range=ba
+00008de0: 7365 5f70 6572 696f 645f 7469 6d65 5f72  se_period_time_r
+00008df0: 616e 6765 2c0a 2020 2020 2020 2020 290a  ange,.        ).
+00008e00: 2020 2020 2020 2020 7769 7468 2064 6173          with das
+00008e10: 6b2e 636f 6e66 6967 2e73 6574 282a 2a7b  k.config.set(**{
+00008e20: 2261 7272 6179 2e73 6c69 6369 6e67 2e73  "array.slicing.s
+00008e30: 706c 6974 5f6c 6172 6765 5f63 6875 6e6b  plit_large_chunk
+00008e40: 7322 3a20 4661 6c73 657d 293a 0a20 2020  s": False}):.   
+00008e50: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00008e60: 7863 2e61 746d 6f73 2e66 7261 6374 696f  xc.atmos.fractio
+00008e70: 6e5f 6f76 6572 5f70 7265 6369 705f 7468  n_over_precip_th
+00008e80: 7265 7368 280a 2020 2020 2020 2020 2020  resh(.          
+00008e90: 2020 2020 2020 7072 5f70 6572 3d70 725f        pr_per=pr_
+00008ea0: 7065 722c 0a20 2020 2020 2020 2020 2020  per,.           
+00008eb0: 2020 2020 202a 2a70 6172 616d 732c 0a20       **params,. 
+00008ec0: 2020 2020 2020 2020 2020 2029 0a0a 0a63             )...c
+00008ed0: 6c61 7373 2053 4449 493a 0a20 2020 2022  lass SDII:.    "
+00008ee0: 2222 4176 6572 6167 6520 7072 6563 6970  ""Average precip
+00008ef0: 6974 6174 696f 6e20 6475 7269 6e67 2077  itation during w
+00008f00: 6574 2064 6179 7320 2870 7229 2e22 2222  et days (pr)."""
+00008f10: 0a0a 2020 2020 7468 7265 7368 203d 2031  ..    thresh = 1
+00008f20: 0a0a 2020 2020 6465 6620 636f 6d70 7574  ..    def comput
+00008f30: 6528 7468 7265 7368 3d74 6872 6573 682c  e(thresh=thresh,
+00008f40: 202a 2a70 6172 616d 7329 3a0a 2020 2020   **params):.    
+00008f50: 2020 2020 2222 2243 616c 6375 6c61 7465      """Calculate
+00008f60: 2061 7665 7261 6765 2070 7265 6369 7069   average precipi
+00008f70: 7461 7469 6f6e 2064 7572 696e 6720 7765  tation during we
+00008f80: 7420 6461 7973 2e0a 0a20 2020 2020 2020  t days...       
+00008f90: 2050 6172 616d 6574 6572 730a 2020 2020   Parameters.    
+00008fa0: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20      ----------. 
+00008fb0: 2020 2020 2020 2074 6872 6573 683a 2069         thresh: i
+00008fc0: 6e74 206f 7220 7374 7269 6e67 0a20 2020  nt or string.   
+00008fd0: 2020 2020 2020 2020 2054 6872 6573 686f           Thresho
+00008fe0: 6c64 2070 7265 6369 7069 7461 7469 6f6e  ld precipitation
+00008ff0: 2061 626f 7665 2077 6869 6368 2061 2064   above which a d
+00009000: 6179 2069 7320 636f 6e73 6964 6572 6564  ay is considered
+00009010: 0a20 2020 2020 2020 2020 2020 2061 7320  .            as 
+00009020: 6120 7765 7420 6461 7920 2864 6566 6175  a wet day (defau
+00009030: 6c74 3a20 3120 6d6d 2f64 6179 292e 0a20  lt: 1 mm/day).. 
+00009040: 2020 2020 2020 2020 2020 2049 6620 7479             If ty
+00009050: 7065 206f 6620 7468 7265 7368 6f6c 6420  pe of threshold 
+00009060: 6973 2061 6e20 696e 7465 6765 7220 7468  is an integer th
+00009070: 6520 756e 6974 2069 7320 7365 7420 746f  e unit is set to
+00009080: 206d 6d2f 6461 792e 0a0a 2020 2020 2020   mm/day...      
+00009090: 2020 5265 7475 726e 730a 2020 2020 2020    Returns.      
+000090a0: 2020 2d2d 2d2d 2d2d 2d0a 2020 2020 2020    -------.      
+000090b0: 2020 7861 7272 6179 2e44 6174 6141 7272    xarray.DataArr
+000090c0: 6179 0a20 2020 2020 2020 2020 2020 2041  ay.            A
+000090d0: 7665 7261 6765 2070 7265 6369 7069 7461  verage precipita
+000090e0: 7469 6f6e 2064 7572 696e 6720 7765 7420  tion during wet 
+000090f0: 6461 7973 2e0a 0a20 2020 2020 2020 204e  days...        N
+00009100: 6f74 6573 0a20 2020 2020 2020 202d 2d2d  otes.        ---
+00009110: 2d2d 0a20 2020 2020 2020 2046 6f72 206d  --.        For m
+00009120: 6f72 6520 696e 666f 726d 6174 696f 6e20  ore information 
+00009130: 6f6e 2074 6865 2069 6e70 7574 2070 6172  on the input par
+00009140: 616d 6574 6572 7320 7365 653a 0a20 2020  ameters see:.   
+00009150: 2020 2020 2020 2020 2068 7474 7073 3a2f           https:/
+00009160: 2f78 636c 696d 2e72 6561 6474 6865 646f  /xclim.readthedo
+00009170: 6373 2e69 6f2f 656e 2f73 7461 626c 652f  cs.io/en/stable/
+00009180: 6170 692e 6874 6d6c 2378 636c 696d 2e69  api.html#xclim.i
+00009190: 6e64 6963 6174 6f72 732e 6174 6d6f 732e  ndicators.atmos.
+000091a0: 6461 696c 795f 7072 5f69 6e74 656e 7369  daily_pr_intensi
+000091b0: 7479 0a20 2020 2020 2020 2022 2222 0a20  ty.        """. 
+000091c0: 2020 2020 2020 2074 6872 6573 6820 3d20         thresh = 
+000091d0: 5f74 6872 6573 685f 7374 7269 6e67 2831  _thresh_string(1
+000091e0: 2c20 226d 6d2f 6461 7922 290a 2020 2020  , "mm/day").    
+000091f0: 2020 2020 7265 7475 726e 2078 632e 6174      return xc.at
+00009200: 6d6f 732e 6461 696c 795f 7072 5f69 6e74  mos.daily_pr_int
+00009210: 656e 7369 7479 280a 2020 2020 2020 2020  ensity(.        
+00009220: 2020 2020 7468 7265 7368 3d74 6872 6573      thresh=thres
+00009230: 682c 0a20 2020 2020 2020 2020 2020 202a  h,.            *
+00009240: 2a70 6172 616d 732c 0a20 2020 2020 2020  *params,.       
+00009250: 2029 0a0a 0a63 6c61 7373 2053 553a 0a20   )...class SU:. 
+00009260: 2020 2022 2222 4e75 6d62 6572 206f 6620     """Number of 
+00009270: 7375 6d6d 6572 2064 6179 7320 2874 6173  summer days (tas
+00009280: 6d61 7829 2e22 2222 0a0a 2020 2020 7468  max)."""..    th
+00009290: 7265 7368 203d 2032 350a 0a20 2020 2064  resh = 25..    d
+000092a0: 6566 2063 6f6d 7075 7465 2874 6872 6573  ef compute(thres
+000092b0: 683d 7468 7265 7368 2c20 2a2a 7061 7261  h=thresh, **para
+000092c0: 6d73 293a 0a20 2020 2020 2020 2022 2222  ms):.        """
+000092d0: 4361 6c63 756c 6174 6520 6e75 6d62 6572  Calculate number
+000092e0: 206f 6620 7375 6d6d 6572 2064 6179 732e   of summer days.
+000092f0: 0a0a 2020 2020 2020 2020 5061 7261 6d65  ..        Parame
+00009300: 7465 7273 0a20 2020 2020 2020 202d 2d2d  ters.        ---
+00009310: 2d2d 2d2d 2d2d 2d0a 2020 2020 2020 2020  -------.        
+00009320: 7468 7265 7368 3a20 696e 7420 6f72 2073  thresh: int or s
+00009330: 7472 696e 670a 2020 2020 2020 2020 2020  tring.          
+00009340: 2020 5468 7265 7368 6f6c 6420 6d61 7869    Threshold maxi
+00009350: 6d75 6d20 7465 6d70 6572 6174 7572 6520  mum temperature 
+00009360: 6162 6f76 6520 7768 6963 6820 746f 2064  above which to d
+00009370: 6179 2069 7320 636f 6e73 6964 6572 6564  ay is considered
+00009380: 0a20 2020 2020 2020 2020 2020 2061 7320  .            as 
+00009390: 6120 7375 6d6d 6572 2064 6179 2028 6465  a summer day (de
+000093a0: 6661 756c 743a 2032 3520 6465 6743 292e  fault: 25 degC).
+000093b0: 0a20 2020 2020 2020 2020 2020 2049 6620  .            If 
+000093c0: 7479 7065 206f 6620 7468 7265 7368 6f6c  type of threshol
+000093d0: 6420 6973 2061 6e20 696e 7465 6765 7220  d is an integer 
+000093e0: 7468 6520 756e 6974 2069 7320 7365 7420  the unit is set 
+000093f0: 746f 2064 6567 432e 0a0a 2020 2020 2020  to degC...      
+00009400: 2020 5265 7475 726e 730a 2020 2020 2020    Returns.      
+00009410: 2020 2d2d 2d2d 2d2d 2d0a 2020 2020 2020    -------.      
+00009420: 2020 7861 7272 6179 2e44 6174 6141 7272    xarray.DataArr
+00009430: 6179 0a20 2020 2020 2020 2020 2020 204e  ay.            N
+00009440: 756d 6265 7220 6f66 2073 756d 6d65 7220  umber of summer 
+00009450: 6461 7973 2028 7478 203e 207b 7468 7265  days (tx > {thre
+00009460: 7368 7d29 2e0a 0a20 2020 2020 2020 204e  sh})...        N
+00009470: 6f74 6573 0a20 2020 2020 2020 202d 2d2d  otes.        ---
+00009480: 2d2d 0a20 2020 2020 2020 2046 6f72 206d  --.        For m
+00009490: 6f72 6520 696e 666f 726d 6174 696f 6e20  ore information 
+000094a0: 6f6e 2074 6865 2069 6e70 7574 2070 6172  on the input par
+000094b0: 616d 6574 6572 7320 7365 653a 0a20 2020  ameters see:.   
+000094c0: 2020 2020 2020 2020 2068 7474 7073 3a2f           https:/
+000094d0: 2f78 636c 696d 2e72 6561 6474 6865 646f  /xclim.readthedo
+000094e0: 6373 2e69 6f2f 656e 2f73 7461 626c 652f  cs.io/en/stable/
+000094f0: 6170 692e 6874 6d6c 2378 636c 696d 2e69  api.html#xclim.i
+00009500: 6e64 6963 6174 6f72 732e 6174 6d6f 732e  ndicators.atmos.
+00009510: 7478 5f64 6179 735f 6162 6f76 650a 2020  tx_days_above.  
+00009520: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+00009530: 2020 7468 7265 7368 203d 205f 7468 7265    thresh = _thre
+00009540: 7368 5f73 7472 696e 6728 7468 7265 7368  sh_string(thresh
+00009550: 2c20 2264 6567 4322 290a 2020 2020 2020  , "degC").      
+00009560: 2020 7265 7475 726e 2078 632e 6174 6d6f    return xc.atmo
+00009570: 732e 7478 5f64 6179 735f 6162 6f76 6528  s.tx_days_above(
+00009580: 0a20 2020 2020 2020 2020 2020 2074 6872  .            thr
+00009590: 6573 683d 7468 7265 7368 2c0a 2020 2020  esh=thresh,.    
+000095a0: 2020 2020 2020 2020 2a2a 7061 7261 6d73          **params
+000095b0: 2c0a 2020 2020 2020 2020 290a 0a0a 636c  ,.        )...cl
+000095c0: 6173 7320 5351 493a 0a20 2020 2022 2222  ass SQI:.    """
+000095d0: 4e75 6d62 6572 206f 6620 756e 636f 6d66  Number of uncomf
+000095e0: 6f72 7461 626c 6520 736c 6565 7020 6576  ortable sleep ev
+000095f0: 656e 7473 2028 7461 736d 696e 292e 2222  ents (tasmin).""
+00009600: 220a 0a20 2020 2074 6872 6573 6820 3d20  "..    thresh = 
+00009610: 3138 0a0a 2020 2020 6465 6620 636f 6d70  18..    def comp
+00009620: 7574 6528 7468 7265 7368 3d74 6872 6573  ute(thresh=thres
+00009630: 682c 202a 2a70 6172 616d 7329 3a0a 2020  h, **params):.  
+00009640: 2020 2020 2020 2222 2243 616c 6375 6c61        """Calcula
+00009650: 7465 206e 756d 6265 7220 6f66 2075 6e63  te number of unc
+00009660: 6f6d 666f 7274 6162 6c65 2073 6c65 6570  omfortable sleep
+00009670: 2065 7665 6e74 732e 0a0a 2020 2020 2020   events...      
+00009680: 2020 5061 7261 6d65 7465 7273 0a20 2020    Parameters.   
+00009690: 2020 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a       ----------.
+000096a0: 2020 2020 2020 2020 7468 7265 7368 3a20          thresh: 
+000096b0: 696e 7420 6f72 2073 7472 696e 670a 2020  int or string.  
+000096c0: 2020 2020 2020 2020 2020 5468 7265 7368            Thresh
+000096d0: 6f6c 6420 6d69 6e69 6d75 6d20 7465 6d70  old minimum temp
+000096e0: 6572 6174 7572 6520 6265 6c6f 7720 7768  erature below wh
+000096f0: 6963 6820 6120 6461 7920 6861 730a 2020  ich a day has.  
+00009700: 2020 2020 2020 2020 2020 6120 756e 636f            a unco
+00009710: 6d66 6f72 7461 626c 6520 736c 6565 7020  mfortable sleep 
+00009720: 6576 656e 7420 2864 6566 6175 6c74 3a20  event (default: 
+00009730: 3138 2064 6567 4329 2e0a 2020 2020 2020  18 degC)..      
+00009740: 2020 2020 2020 4966 2074 7970 6520 6f66        If type of
+00009750: 2074 6872 6573 686f 6c64 2069 7320 616e   threshold is an
+00009760: 2069 6e74 6567 6572 2074 6865 2075 6e69   integer the uni
+00009770: 7420 6973 2073 6574 2074 6f20 6465 6743  t is set to degC
+00009780: 2e0a 0a20 2020 2020 2020 2052 6574 7572  ...        Retur
+00009790: 6e73 0a20 2020 2020 2020 202d 2d2d 2d2d  ns.        -----
+000097a0: 2d2d 0a20 2020 2020 2020 2078 6172 7261  --.        xarra
+000097b0: 792e 4461 7461 4172 7261 790a 2020 2020  y.DataArray.    
+000097c0: 2020 2020 2020 2020 4e75 6d62 6572 206f          Number o
+000097d0: 6620 756e 636f 6d66 6f72 7461 626c 6520  f uncomfortable 
+000097e0: 736c 6565 7020 6576 656e 7473 2028 746e  sleep events (tn
+000097f0: 203c 207b 7468 7265 7368 7d29 2e0a 0a20   < {thresh})... 
+00009800: 2020 2020 2020 204e 6f74 6573 0a20 2020         Notes.   
+00009810: 2020 2020 202d 2d2d 2d2d 0a20 2020 2020       -----.     
+00009820: 2020 2046 6f72 206d 6f72 6520 696e 666f     For more info
+00009830: 726d 6174 696f 6e20 6f6e 2074 6865 2069  rmation on the i
+00009840: 6e70 7574 2070 6172 616d 6574 6572 7320  nput parameters 
+00009850: 7365 653a 0a20 2020 2020 2020 2020 2020  see:.           
+00009860: 2068 7474 7073 3a2f 2f78 636c 696d 2e72   https://xclim.r
+00009870: 6561 6474 6865 646f 6373 2e69 6f2f 656e  eadthedocs.io/en
+00009880: 2f73 7461 626c 652f 6170 692e 6874 6d6c  /stable/api.html
+00009890: 2378 636c 696d 2e69 6e64 6963 6174 6f72  #xclim.indicator
+000098a0: 732e 6174 6d6f 732e 746e 5f64 6179 735f  s.atmos.tn_days_
+000098b0: 6162 6f76 650a 2020 2020 2020 2020 2222  above.        ""
+000098c0: 220a 2020 2020 2020 2020 7468 7265 7368  ".        thresh
+000098d0: 203d 205f 7468 7265 7368 5f73 7472 696e   = _thresh_strin
+000098e0: 6728 7468 7265 7368 2c20 2264 6567 4322  g(thresh, "degC"
+000098f0: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
+00009900: 2078 632e 6174 6d6f 732e 746e 5f64 6179   xc.atmos.tn_day
+00009910: 735f 6162 6f76 6528 0a20 2020 2020 2020  s_above(.       
+00009920: 2020 2020 2074 6872 6573 683d 7468 7265       thresh=thre
+00009930: 7368 2c0a 2020 2020 2020 2020 2020 2020  sh,.            
+00009940: 2a2a 7061 7261 6d73 2c0a 2020 2020 2020  **params,.      
+00009950: 2020 290a 0a0a 636c 6173 7320 5447 3a0a    )...class TG:.
+00009960: 2020 2020 2222 224d 6561 6e20 6d65 616e      """Mean mean
+00009970: 2074 656d 7065 7261 7475 7265 2028 7461   temperature (ta
+00009980: 7329 2e22 2222 0a0a 2020 2020 6465 6620  s)."""..    def 
+00009990: 636f 6d70 7574 6528 2a2a 7061 7261 6d73  compute(**params
+000099a0: 293a 0a20 2020 2020 2020 2022 2222 4361  ):.        """Ca
+000099b0: 6c63 756c 6174 6520 6d65 616e 2064 6169  lculate mean dai
+000099c0: 6c79 206d 6561 6e20 7465 6d70 6572 6174  ly mean temperat
+000099d0: 7572 652e 0a0a 2020 2020 2020 2020 5265  ure...        Re
+000099e0: 7475 726e 730a 2020 2020 2020 2020 2d2d  turns.        --
+000099f0: 2d2d 2d2d 2d0a 2020 2020 2020 2020 7861  -----.        xa
+00009a00: 7272 6179 2e44 6174 6141 7272 6179 0a20  rray.DataArray. 
+00009a10: 2020 2020 2020 2020 2020 204d 6561 6e20             Mean 
+00009a20: 6461 696c 7920 6d65 616e 2074 656d 7065  daily mean tempe
+00009a30: 7261 7475 7265 2e0a 0a20 2020 2020 2020  rature...       
+00009a40: 204e 6f74 6573 0a20 2020 2020 2020 202d   Notes.        -
+00009a50: 2d2d 2d2d 0a20 2020 2020 2020 2046 6f72  ----.        For
+00009a60: 2069 6e66 6f72 6d61 7469 6f6e 206f 6e20   information on 
+00009a70: 7468 6520 696e 7075 7420 7061 7261 6d65  the input parame
+00009a80: 7465 7273 2073 6565 3a0a 2020 2020 2020  ters see:.      
+00009a90: 2020 2020 2020 6874 7470 733a 2f2f 7863        https://xc
+00009aa0: 6c69 6d2e 7265 6164 7468 6564 6f63 732e  lim.readthedocs.
+00009ab0: 696f 2f65 6e2f 7374 6162 6c65 2f61 7069  io/en/stable/api
+00009ac0: 2e68 746d 6c23 7863 6c69 6d2e 696e 6469  .html#xclim.indi
+00009ad0: 6361 746f 7273 2e61 746d 6f73 2e74 675f  cators.atmos.tg_
+00009ae0: 6d65 616e 0a20 2020 2020 2020 2022 2222  mean.        """
+00009af0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00009b00: 7863 2e61 746d 6f73 2e74 675f 6d65 616e  xc.atmos.tg_mean
+00009b10: 282a 2a70 6172 616d 7329 0a0a 0a63 6c61  (**params)...cla
+00009b20: 7373 2054 4731 3070 3a0a 2020 2020 2222  ss TG10p:.    ""
+00009b30: 2246 7261 6374 696f 6e20 6f66 2064 6179  "Fraction of day
+00009b40: 7320 7769 7468 206d 6561 6e20 7465 6d70  s with mean temp
+00009b50: 6572 6174 7572 6520 3c20 3130 7468 2070  erature < 10th p
+00009b60: 6572 6365 6e74 696c 6520 2874 6173 292e  ercentile (tas).
+00009b70: 2222 220a 0a20 2020 2074 6173 5f70 6572  """..    tas_per
+00009b80: 203d 204e 6f6e 650a 2020 2020 6261 7365   = None.    base
+00009b90: 5f70 6572 696f 645f 7469 6d65 5f72 616e  _period_time_ran
+00009ba0: 6765 203d 2042 4153 455f 5045 5249 4f44  ge = BASE_PERIOD
+00009bb0: 0a0a 2020 2020 6465 6620 636f 6d70 7574  ..    def comput
+00009bc0: 6528 0a20 2020 2020 2020 2062 6173 655f  e(.        base_
+00009bd0: 7065 7269 6f64 5f74 696d 655f 7261 6e67  period_time_rang
+00009be0: 653d 6261 7365 5f70 6572 696f 645f 7469  e=base_period_ti
+00009bf0: 6d65 5f72 616e 6765 2c0a 2020 2020 2020  me_range,.      
+00009c00: 2020 7461 735f 7065 723d 7461 735f 7065    tas_per=tas_pe
+00009c10: 722c 0a20 2020 2020 2020 202a 2a70 6172  r,.        **par
+00009c20: 616d 732c 0a20 2020 2029 3a0a 2020 2020  ams,.    ):.    
+00009c30: 2020 2020 2222 2243 616c 6375 6c61 7465      """Calculate
+00009c40: 2066 7261 6374 696f 6e20 6f66 2064 6179   fraction of day
+00009c50: 7320 7769 7468 206d 6561 6e20 7465 6d70  s with mean temp
+00009c60: 6572 6174 7572 6520 3c20 3130 7468 2070  erature < 10th p
+00009c70: 6572 6365 6e74 696c 652e 0a0a 2020 2020  ercentile...    
+00009c80: 2020 2020 5061 7261 6d65 7465 7273 0a20      Parameters. 
+00009c90: 2020 2020 2020 202d 2d2d 2d2d 2d2d 2d2d         ---------
+00009ca0: 2d0a 2020 2020 2020 2020 7461 735f 7065  -.        tas_pe
+00009cb0: 723a 2078 722e 4461 7461 4172 7261 792c  r: xr.DataArray,
+00009cc0: 206f 7074 696f 6e61 6c0a 2020 2020 2020   optional.      
+00009cd0: 2020 2020 2020 5465 6d70 6572 6174 7572        Temperatur
+00009ce0: 6520 3130 7468 2070 6572 6365 6e74 696c  e 10th percentil
+00009cf0: 6520 7265 6665 7265 6e63 6520 7661 6c75  e reference valu
+00009d00: 652e 0a20 2020 2020 2020 2062 6173 655f  e..        base_
+00009d10: 7065 7269 6f64 5f74 696d 655f 7261 6e67  period_time_rang
+00009d20: 653a 206c 6973 740a 2020 2020 2020 2020  e: list.        
+00009d30: 2020 2020 4c69 7374 2077 6974 6820 6c65      List with le
+00009d40: 6674 2062 6f75 6e64 2069 7320 7374 6172  ft bound is star
+00009d50: 7420 7965 6172 2073 7472 696e 6720 616e  t year string an
+00009d60: 6420 7269 6768 7420 626f 756e 6420 6973  d right bound is
+00009d70: 0a20 2020 2020 2020 2020 2020 2065 6e64  .            end
+00009d80: 2079 6561 7220 7374 7269 6e67 2066 6f72   year string for
+00009d90: 2063 616c 6375 6c61 7469 6e67 2060 7461   calculating `ta
+00009da0: 735f 7065 7260 2e0a 2020 2020 2020 2020  s_per`..        
+00009db0: 2020 2020 5468 6973 2077 696c 6c20 6265      This will be
+00009dc0: 2075 7365 6420 6f6e 6c79 2069 6620 6074   used only if `t
+00009dd0: 6173 5f70 6572 6020 6973 204e 6f6e 652e  as_per` is None.
+00009de0: 0a0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
+00009df0: 730a 2020 2020 2020 2020 2d2d 2d2d 2d2d  s.        ------
+00009e00: 2d0a 2020 2020 2020 2020 7861 7272 6179  -.        xarray
+00009e10: 2e44 6174 6141 7272 6179 0a20 2020 2020  .DataArray.     
+00009e20: 2020 2020 2020 2046 7261 6374 696f 6e20         Fraction 
+00009e30: 6f66 2064 6179 7320 7769 7468 206d 6561  of days with mea
+00009e40: 6e20 7465 6d70 6572 6174 7572 6520 3c20  n temperature < 
+00009e50: 3130 7468 2070 6572 6365 6e74 696c 6522  10th percentile"
+00009e60: 2e0a 0a20 2020 2020 2020 204e 6f74 6573  ...        Notes
+00009e70: 0a20 2020 2020 2020 202d 2d2d 2d2d 0a20  .        -----. 
+00009e80: 2020 2020 2020 2046 6f72 206d 6f72 6520         For more 
+00009e90: 696e 666f 726d 6174 696f 6e20 6f6e 2074  information on t
+00009ea0: 6865 2069 6e70 7574 2070 6172 616d 6574  he input paramet
+00009eb0: 6572 7320 7365 653a 0a20 2020 2020 2020  ers see:.       
+00009ec0: 2020 2020 2068 7474 7073 3a2f 2f78 636c       https://xcl
+00009ed0: 696d 2e72 6561 6474 6865 646f 6373 2e69  im.readthedocs.i
+00009ee0: 6f2f 656e 2f73 7461 626c 652f 6170 692e  o/en/stable/api.
+00009ef0: 6874 6d6c 2378 636c 696d 2e69 6e64 6963  html#xclim.indic
+00009f00: 6174 6f72 732e 6174 6d6f 732e 7467 3130  ators.atmos.tg10
+00009f10: 700a 2020 2020 2020 2020 2222 220a 2020  p.        """.  
+00009f20: 2020 2020 2020 6461 203d 205f 6765 745f        da = _get_
+00009f30: 6461 2870 6172 616d 732c 2022 7461 7322  da(params, "tas"
+00009f40: 290a 2020 2020 2020 2020 6966 2074 6173  ).        if tas
+00009f50: 5f70 6572 2069 7320 4e6f 6e65 3a0a 2020  _per is None:.  
+00009f60: 2020 2020 2020 2020 2020 7461 735f 7065            tas_pe
+00009f70: 7220 3d20 5f67 6574 5f70 6572 6365 6e74  r = _get_percent
+00009f80: 696c 6528 0a20 2020 2020 2020 2020 2020  ile(.           
+00009f90: 2020 2020 2064 613d 6461 2c0a 2020 2020       da=da,.    
+00009fa0: 2020 2020 2020 2020 2020 2020 7065 723d              per=
+00009fb0: 3130 2c0a 2020 2020 2020 2020 2020 2020  10,.            
+00009fc0: 2020 2020 6261 7365 5f70 6572 696f 645f      base_period_
+00009fd0: 7469 6d65 5f72 616e 6765 3d62 6173 655f  time_range=base_
+00009fe0: 7065 7269 6f64 5f74 696d 655f 7261 6e67  period_time_rang
+00009ff0: 652c 0a20 2020 2020 2020 2020 2020 2029  e,.            )
+0000a000: 0a20 2020 2020 2020 2077 6974 6820 6461  .        with da
+0000a010: 736b 2e63 6f6e 6669 672e 7365 7428 2a2a  sk.config.set(**
+0000a020: 7b22 6172 7261 792e 736c 6963 696e 672e  {"array.slicing.
+0000a030: 7370 6c69 745f 6c61 7267 655f 6368 756e  split_large_chun
+0000a040: 6b73 223a 2046 616c 7365 7d29 3a0a 2020  ks": False}):.  
+0000a050: 2020 2020 2020 2020 2020 7265 7475 726e            return
+0000a060: 2078 632e 6174 6d6f 732e 7467 3130 7028   xc.atmos.tg10p(
+0000a070: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000a080: 2074 6173 5f70 6572 3d74 6173 5f70 6572   tas_per=tas_per
+0000a090: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0000a0a0: 2020 2a2a 7061 7261 6d73 2c0a 2020 2020    **params,.    
+0000a0b0: 2020 2020 2020 2020 290a 0a0a 636c 6173          )...clas
+0000a0c0: 7320 5447 3930 703a 0a20 2020 2022 2222  s TG90p:.    """
+0000a0d0: 4672 6163 7469 6f6e 206f 6620 6461 7973  Fraction of days
+0000a0e0: 2077 6974 6820 6d65 616e 2074 656d 7065   with mean tempe
+0000a0f0: 7261 7475 7265 203e 2039 3074 6820 7065  rature > 90th pe
+0000a100: 7263 656e 7469 6c65 2028 7461 7329 2e22  rcentile (tas)."
+0000a110: 2222 0a0a 2020 2020 7461 735f 7065 7220  ""..    tas_per 
+0000a120: 3d20 4e6f 6e65 0a20 2020 2062 6173 655f  = None.    base_
+0000a130: 7065 7269 6f64 5f74 696d 655f 7261 6e67  period_time_rang
+0000a140: 6520 3d20 4241 5345 5f50 4552 494f 440a  e = BASE_PERIOD.
+0000a150: 0a20 2020 2064 6566 2063 6f6d 7075 7465  .    def compute
+0000a160: 280a 2020 2020 2020 2020 6261 7365 5f70  (.        base_p
+0000a170: 6572 696f 645f 7469 6d65 5f72 616e 6765  eriod_time_range
+0000a180: 3d62 6173 655f 7065 7269 6f64 5f74 696d  =base_period_tim
+0000a190: 655f 7261 6e67 652c 0a20 2020 2020 2020  e_range,.       
+0000a1a0: 2074 6173 5f70 6572 3d74 6173 5f70 6572   tas_per=tas_per
+0000a1b0: 2c0a 2020 2020 2020 2020 2a2a 7061 7261  ,.        **para
+0000a1c0: 6d73 2c0a 2020 2020 293a 0a20 2020 2020  ms,.    ):.     
+0000a1d0: 2020 2022 2222 4361 6c63 756c 6174 6520     """Calculate 
+0000a1e0: 6672 6163 7469 6f6e 206f 6620 6461 7973  fraction of days
+0000a1f0: 2077 6974 6820 6d65 616e 2074 656d 7065   with mean tempe
+0000a200: 7261 7475 7265 203e 2039 3074 6820 7065  rature > 90th pe
+0000a210: 7263 656e 7469 6c65 222e 0a0a 2020 2020  rcentile"...    
+0000a220: 2020 2020 5061 7261 6d65 7465 7273 0a20      Parameters. 
+0000a230: 2020 2020 2020 202d 2d2d 2d2d 2d2d 2d2d         ---------
+0000a240: 2d0a 2020 2020 2020 2020 7461 735f 7065  -.        tas_pe
+0000a250: 723a 2078 722e 4461 7461 4172 7261 792c  r: xr.DataArray,
+0000a260: 206f 7074 696f 6e61 6c0a 2020 2020 2020   optional.      
+0000a270: 2020 2020 2020 5465 6d70 6572 6174 7572        Temperatur
+0000a280: 6520 3930 7468 2070 6572 6365 6e74 696c  e 90th percentil
+0000a290: 6520 7265 6665 7265 6e63 6520 7661 6c75  e reference valu
+0000a2a0: 652e 0a20 2020 2020 2020 2062 6173 655f  e..        base_
+0000a2b0: 7065 7269 6f64 5f74 696d 655f 7261 6e67  period_time_rang
+0000a2c0: 653a 206c 6973 740a 2020 2020 2020 2020  e: list.        
+0000a2d0: 2020 2020 4c69 7374 2077 6974 6820 6c65      List with le
+0000a2e0: 6674 2062 6f75 6e64 2069 7320 7374 6172  ft bound is star
+0000a2f0: 7420 7965 6172 2073 7472 696e 6720 616e  t year string an
+0000a300: 6420 7269 6768 7420 626f 756e 640a 2020  d right bound.  
+0000a310: 2020 2020 2020 2020 2020 6973 2065 6e64            is end
+0000a320: 2079 6561 7220 7374 7269 6e67 2066 6f72   year string for
+0000a330: 2063 616c 6375 6c61 7469 6e67 2060 7461   calculating `ta
+0000a340: 735f 7065 7260 2e0a 2020 2020 2020 2020  s_per`..        
+0000a350: 2020 2020 5468 6973 2077 696c 6c20 6265      This will be
+0000a360: 2075 7365 6420 6f6e 6c79 2069 6620 6074   used only if `t
+0000a370: 6173 5f70 6572 6020 6973 204e 6f6e 652e  as_per` is None.
+0000a380: 0a0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
+0000a390: 730a 2020 2020 2020 2020 2d2d 2d2d 2d2d  s.        ------
+0000a3a0: 2d0a 2020 2020 2020 2020 7861 7272 6179  -.        xarray
+0000a3b0: 2e44 6174 6141 7272 6179 0a20 2020 2020  .DataArray.     
+0000a3c0: 2020 2020 2020 2046 7261 6374 696f 6e20         Fraction 
+0000a3d0: 6f66 2064 6179 7320 7769 7468 206d 6561  of days with mea
+0000a3e0: 6e20 7465 6d70 6572 6174 7572 6520 3e20  n temperature > 
+0000a3f0: 3930 7468 2070 6572 6365 6e74 696c 6522  90th percentile"
+0000a400: 2e0a 0a20 2020 2020 2020 204e 6f74 6573  ...        Notes
+0000a410: 0a20 2020 2020 2020 202d 2d2d 2d2d 0a20  .        -----. 
+0000a420: 2020 2020 2020 2046 6f72 206d 6f72 6520         For more 
+0000a430: 696e 666f 726d 6174 696f 6e20 6f6e 2074  information on t
+0000a440: 6865 2069 6e70 7574 2070 6172 616d 6574  he input paramet
+0000a450: 6572 7320 7365 653a 0a20 2020 2020 2020  ers see:.       
+0000a460: 2020 2020 2068 7474 7073 3a2f 2f78 636c       https://xcl
+0000a470: 696d 2e72 6561 6474 6865 646f 6373 2e69  im.readthedocs.i
+0000a480: 6f2f 656e 2f73 7461 626c 652f 6170 692e  o/en/stable/api.
+0000a490: 6874 6d6c 2378 636c 696d 2e69 6e64 6963  html#xclim.indic
+0000a4a0: 6174 6f72 732e 6174 6d6f 732e 7467 3930  ators.atmos.tg90
+0000a4b0: 700a 2020 2020 2020 2020 2222 220a 2020  p.        """.  
+0000a4c0: 2020 2020 2020 6461 203d 205f 6765 745f        da = _get_
+0000a4d0: 6461 2870 6172 616d 732c 2022 7461 7322  da(params, "tas"
+0000a4e0: 290a 2020 2020 2020 2020 6966 2074 6173  ).        if tas
+0000a4f0: 5f70 6572 2069 7320 4e6f 6e65 3a0a 2020  _per is None:.  
+0000a500: 2020 2020 2020 2020 2020 7461 735f 7065            tas_pe
+0000a510: 7220 3d20 5f67 6574 5f70 6572 6365 6e74  r = _get_percent
+0000a520: 696c 6528 0a20 2020 2020 2020 2020 2020  ile(.           
+0000a530: 2020 2020 2064 613d 6461 2c0a 2020 2020       da=da,.    
+0000a540: 2020 2020 2020 2020 2020 2020 7065 723d              per=
+0000a550: 3930 2c0a 2020 2020 2020 2020 2020 2020  90,.            
+0000a560: 2020 2020 6261 7365 5f70 6572 696f 645f      base_period_
+0000a570: 7469 6d65 5f72 616e 6765 3d62 6173 655f  time_range=base_
+0000a580: 7065 7269 6f64 5f74 696d 655f 7261 6e67  period_time_rang
+0000a590: 652c 0a20 2020 2020 2020 2020 2020 2029  e,.            )
+0000a5a0: 0a20 2020 2020 2020 2077 6974 6820 6461  .        with da
+0000a5b0: 736b 2e63 6f6e 6669 672e 7365 7428 2a2a  sk.config.set(**
+0000a5c0: 7b22 6172 7261 792e 736c 6963 696e 672e  {"array.slicing.
+0000a5d0: 7370 6c69 745f 6c61 7267 655f 6368 756e  split_large_chun
+0000a5e0: 6b73 223a 2046 616c 7365 7d29 3a0a 2020  ks": False}):.  
+0000a5f0: 2020 2020 2020 2020 2020 7265 7475 726e            return
+0000a600: 2078 632e 6174 6d6f 732e 7467 3930 7028   xc.atmos.tg90p(
+0000a610: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000a620: 2074 6173 5f70 6572 3d74 6173 5f70 6572   tas_per=tas_per
+0000a630: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0000a640: 2020 2a2a 7061 7261 6d73 2c0a 2020 2020    **params,.    
+0000a650: 2020 2020 2020 2020 290a 0a0a 636c 6173          )...clas
+0000a660: 7320 5452 3a0a 2020 2020 2222 224e 756d  s TR:.    """Num
+0000a670: 6265 7220 6f66 2074 726f 7069 6361 6c20  ber of tropical 
+0000a680: 6e69 6768 7473 2028 7461 736d 696e 292e  nights (tasmin).
+0000a690: 2222 220a 0a20 2020 2074 6872 6573 6820  """..    thresh 
+0000a6a0: 3d20 3230 0a0a 2020 2020 6465 6620 636f  = 20..    def co
+0000a6b0: 6d70 7574 6528 7468 7265 7368 3d74 6872  mpute(thresh=thr
+0000a6c0: 6573 682c 202a 2a70 6172 616d 7329 3a0a  esh, **params):.
+0000a6d0: 2020 2020 2020 2020 2222 2243 616c 6375          """Calcu
+0000a6e0: 6c61 7465 206e 756d 6265 7220 6f66 2074  late number of t
+0000a6f0: 726f 7069 6361 6c20 6e69 6768 7473 2e0a  ropical nights..
+0000a700: 0a20 2020 2020 2020 2050 6172 616d 6574  .        Paramet
+0000a710: 6572 730a 2020 2020 2020 2020 2d2d 2d2d  ers.        ----
+0000a720: 2d2d 2d2d 2d2d 0a20 2020 2020 2020 2074  ------.        t
+0000a730: 6872 6573 683a 2069 6e74 206f 7220 7374  hresh: int or st
+0000a740: 7269 6e67 0a20 2020 2020 2020 2020 2020  ring.           
+0000a750: 2054 6872 6573 686f 6c64 206d 696e 696d   Threshold minim
+0000a760: 756d 2074 656d 7065 7261 7475 7265 206f  um temperature o
+0000a770: 6e20 7768 6963 6820 6120 6461 790a 2020  n which a day.  
+0000a780: 2020 2020 2020 2020 2020 6861 7320 6120            has a 
+0000a790: 7472 6f70 6963 616c 206e 6967 6874 2028  tropical night (
+0000a7a0: 6465 6661 756c 743a 2032 3020 6465 6743  default: 20 degC
+0000a7b0: 292e 0a20 2020 2020 2020 2020 2020 2049  )..            I
+0000a7c0: 6620 7479 7065 206f 6620 7468 7265 7368  f type of thresh
+0000a7d0: 6f6c 6420 6973 2061 6e20 696e 7465 6765  old is an intege
+0000a7e0: 7220 7468 6520 756e 6974 2069 7320 7365  r the unit is se
+0000a7f0: 7420 746f 2064 6567 432e 0a0a 2020 2020  t to degC...    
+0000a800: 2020 2020 5265 7475 726e 730a 2020 2020      Returns.    
+0000a810: 2020 2020 2d2d 2d2d 2d2d 2d0a 2020 2020      -------.    
+0000a820: 2020 2020 7861 7272 6179 2e44 6174 6141      xarray.DataA
+0000a830: 7272 6179 0a20 2020 2020 2020 2020 2020  rray.           
+0000a840: 204e 756d 6265 7220 6f66 2074 726f 7069   Number of tropi
+0000a850: 6361 6c20 6e69 6768 7473 2028 746e 203e  cal nights (tn >
+0000a860: 207b 7468 7265 7368 7d2e 0a0a 2020 2020   {thresh}...    
+0000a870: 2020 2020 4e6f 7465 730a 2020 2020 2020      Notes.      
+0000a880: 2020 2d2d 2d2d 2d0a 2020 2020 2020 2020    -----.        
+0000a890: 466f 7220 6d6f 7265 2069 6e66 6f72 6d61  For more informa
+0000a8a0: 7469 6f6e 206f 6e20 7468 6520 696e 7075  tion on the inpu
+0000a8b0: 7420 7061 7261 6d65 7465 7273 2073 6565  t parameters see
+0000a8c0: 3a0a 2020 2020 2020 2020 2020 2020 6874  :.            ht
+0000a8d0: 7470 733a 2f2f 7863 6c69 6d2e 7265 6164  tps://xclim.read
+0000a8e0: 7468 6564 6f63 732e 696f 2f65 6e2f 7374  thedocs.io/en/st
+0000a8f0: 6162 6c65 2f61 7069 2e68 746d 6c23 7863  able/api.html#xc
+0000a900: 6c69 6d2e 696e 6469 6361 746f 7273 2e61  lim.indicators.a
+0000a910: 746d 6f73 2e74 6e5f 6461 7973 5f61 626f  tmos.tn_days_abo
+0000a920: 7665 0a20 2020 2020 2020 2022 2222 0a20  ve.        """. 
+0000a930: 2020 2020 2020 2074 6872 6573 6820 3d20         thresh = 
+0000a940: 5f74 6872 6573 685f 7374 7269 6e67 2874  _thresh_string(t
+0000a950: 6872 6573 682c 2022 6465 6743 2229 0a20  hresh, "degC"). 
+0000a960: 2020 2020 2020 2072 6574 7572 6e20 7863         return xc
+0000a970: 2e61 746d 6f73 2e74 6e5f 6461 7973 5f61  .atmos.tn_days_a
+0000a980: 626f 7665 280a 2020 2020 2020 2020 2020  bove(.          
+0000a990: 2020 7468 7265 7368 3d74 6872 6573 682c    thresh=thresh,
+0000a9a0: 0a20 2020 2020 2020 2020 2020 202a 2a70  .            **p
+0000a9b0: 6172 616d 732c 0a20 2020 2020 2020 2029  arams,.        )
+0000a9c0: 0a0a 0a63 6c61 7373 2054 583a 0a20 2020  ...class TX:.   
+0000a9d0: 2022 2222 4d65 616e 206d 6178 696d 756d   """Mean maximum
+0000a9e0: 2074 656d 7065 7261 7475 7265 2028 7461   temperature (ta
+0000a9f0: 736d 6178 292e 2222 220a 0a20 2020 2064  smax)."""..    d
+0000aa00: 6566 2063 6f6d 7075 7465 282a 2a70 6172  ef compute(**par
+0000aa10: 616d 7329 3a0a 2020 2020 2020 2020 2222  ams):.        ""
+0000aa20: 2243 616c 6375 6c61 7465 206d 6561 6e20  "Calculate mean 
+0000aa30: 6461 696c 7920 6d61 7869 6d75 6d20 7465  daily maximum te
+0000aa40: 6d70 6572 6174 7572 652e 0a0a 2020 2020  mperature...    
+0000aa50: 2020 2020 5265 7475 726e 730a 2020 2020      Returns.    
+0000aa60: 2020 2020 2d2d 2d2d 2d2d 2d0a 2020 2020      -------.    
+0000aa70: 2020 2020 7861 7272 6179 2e44 6174 6141      xarray.DataA
+0000aa80: 7272 6179 0a20 2020 2020 2020 2020 2020  rray.           
+0000aa90: 204d 6561 6e20 6461 696c 7920 6d61 7869   Mean daily maxi
+0000aaa0: 6d75 6d20 7465 6d70 6572 6174 7572 652e  mum temperature.
+0000aab0: 0a0a 2020 2020 2020 2020 4e6f 7465 730a  ..        Notes.
+0000aac0: 2020 2020 2020 2020 2d2d 2d2d 2d0a 2020          -----.  
+0000aad0: 2020 2020 2020 466f 7220 696e 666f 726d        For inform
+0000aae0: 6174 696f 6e20 6f6e 2074 6865 2069 6e70  ation on the inp
+0000aaf0: 7574 2070 6172 616d 6574 6572 7320 7365  ut parameters se
+0000ab00: 653a 0a20 2020 2020 2020 2020 2020 2068  e:.            h
+0000ab10: 7474 7073 3a2f 2f78 636c 696d 2e72 6561  ttps://xclim.rea
+0000ab20: 6474 6865 646f 6373 2e69 6f2f 656e 2f73  dthedocs.io/en/s
+0000ab30: 7461 626c 652f 6170 692e 6874 6d6c 2378  table/api.html#x
+0000ab40: 636c 696d 2e69 6e64 6963 6174 6f72 732e  clim.indicators.
+0000ab50: 6174 6d6f 732e 7478 5f6d 6561 6e0a 2020  atmos.tx_mean.  
+0000ab60: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+0000ab70: 2020 7265 7475 726e 2078 632e 6174 6d6f    return xc.atmo
+0000ab80: 732e 7478 5f6d 6561 6e28 2a2a 7061 7261  s.tx_mean(**para
+0000ab90: 6d73 290a 0a0a 636c 6173 7320 5458 3130  ms)...class TX10
+0000aba0: 703a 0a20 2020 2022 2222 4672 6163 7469  p:.    """Fracti
+0000abb0: 6f6e 206f 6620 6461 7973 2077 6974 6820  on of days with 
+0000abc0: 6d61 7820 7465 6d70 6572 6174 7572 6520  max temperature 
+0000abd0: 3c20 3130 7468 2070 6572 6365 6e74 696c  < 10th percentil
+0000abe0: 6520 2874 6173 6d61 7829 2e22 2222 0a0a  e (tasmax)."""..
+0000abf0: 2020 2020 7461 736d 6178 5f70 6572 203d      tasmax_per =
+0000ac00: 204e 6f6e 650a 2020 2020 6261 7365 5f70   None.    base_p
+0000ac10: 6572 696f 645f 7469 6d65 5f72 616e 6765  eriod_time_range
+0000ac20: 203d 2042 4153 455f 5045 5249 4f44 0a0a   = BASE_PERIOD..
+0000ac30: 2020 2020 6465 6620 636f 6d70 7574 6528      def compute(
+0000ac40: 0a20 2020 2020 2020 2062 6173 655f 7065  .        base_pe
+0000ac50: 7269 6f64 5f74 696d 655f 7261 6e67 653d  riod_time_range=
+0000ac60: 6261 7365 5f70 6572 696f 645f 7469 6d65  base_period_time
+0000ac70: 5f72 616e 6765 2c0a 2020 2020 2020 2020  _range,.        
+0000ac80: 7461 736d 6178 5f70 6572 3d74 6173 6d61  tasmax_per=tasma
+0000ac90: 785f 7065 722c 0a20 2020 2020 2020 202a  x_per,.        *
+0000aca0: 2a70 6172 616d 732c 0a20 2020 2029 3a0a  *params,.    ):.
+0000acb0: 2020 2020 2020 2020 2222 2243 616c 6375          """Calcu
+0000acc0: 6c61 7465 2066 7261 6374 696f 6e20 6f66  late fraction of
+0000acd0: 2064 6179 7320 7769 7468 206d 6178 2074   days with max t
+0000ace0: 656d 7065 7261 7475 7265 203c 2031 3074  emperature < 10t
+0000acf0: 6820 7065 7263 656e 7469 6c65 2e0a 0a20  h percentile... 
+0000ad00: 2020 2020 2020 2050 6172 616d 6574 6572         Parameter
+0000ad10: 730a 2020 2020 2020 2020 2d2d 2d2d 2d2d  s.        ------
+0000ad20: 2d2d 2d2d 0a20 2020 2020 2020 2074 6173  ----.        tas
+0000ad30: 6d61 785f 7065 723a 2078 722e 4461 7461  max_per: xr.Data
+0000ad40: 4172 7261 792c 206f 7074 696f 6e61 6c0a  Array, optional.
+0000ad50: 2020 2020 2020 2020 2020 2020 4d61 7869              Maxi
+0000ad60: 6d75 6d20 7465 6d70 6572 6174 7572 6520  mum temperature 
+0000ad70: 3130 7468 2070 6572 6365 6e74 696c 6520  10th percentile 
+0000ad80: 7265 6665 7265 6e63 6520 7661 6c75 652e  reference value.
+0000ad90: 0a20 2020 2020 2020 2062 6173 655f 7065  .        base_pe
+0000ada0: 7269 6f64 5f74 696d 655f 7261 6e67 653a  riod_time_range:
+0000adb0: 206c 6973 740a 2020 2020 2020 2020 2020   list.          
+0000adc0: 2020 4c69 7374 2077 6974 6820 6c65 6674    List with left
+0000add0: 2062 6f75 6e64 2069 7320 7374 6172 7420   bound is start 
+0000ade0: 7965 6172 2073 7472 696e 6720 616e 6420  year string and 
+0000adf0: 7269 6768 7420 626f 756e 640a 2020 2020  right bound.    
+0000ae00: 2020 2020 2020 2020 6973 2065 6e64 2079          is end y
+0000ae10: 6561 7220 7374 7269 6e67 2066 6f72 2063  ear string for c
+0000ae20: 616c 6375 6c61 7469 6e67 2060 7461 736d  alculating `tasm
+0000ae30: 6178 5f70 6572 602e 0a20 2020 2020 2020  ax_per`..       
+0000ae40: 2020 2020 2054 6869 7320 7769 6c6c 2062       This will b
+0000ae50: 6520 7573 6564 206f 6e6c 7920 6966 2060  e used only if `
+0000ae60: 7461 736d 6178 5f70 6572 6020 6973 204e  tasmax_per` is N
+0000ae70: 6f6e 652e 0a0a 2020 2020 2020 2020 5265  one...        Re
+0000ae80: 7475 726e 730a 2020 2020 2020 2020 2d2d  turns.        --
+0000ae90: 2d2d 2d2d 2d0a 2020 2020 2020 2020 7861  -----.        xa
+0000aea0: 7272 6179 2e44 6174 6141 7272 6179 0a20  rray.DataArray. 
+0000aeb0: 2020 2020 2020 2020 2020 2046 7261 6374             Fract
+0000aec0: 696f 6e20 6f66 2064 6179 7320 7769 7468  ion of days with
+0000aed0: 206d 6178 696d 756d 2074 656d 7065 7261   maximum tempera
+0000aee0: 7475 7265 203c 2031 3074 6820 7065 7263  ture < 10th perc
+0000aef0: 656e 7469 6c65 222e 0a0a 2020 2020 2020  entile"...      
+0000af00: 2020 4e6f 7465 730a 2020 2020 2020 2020    Notes.        
+0000af10: 2d2d 2d2d 2d0a 2020 2020 2020 2020 466f  -----.        Fo
+0000af20: 7220 6d6f 7265 2069 6e66 6f72 6d61 7469  r more informati
+0000af30: 6f6e 206f 6e20 7468 6520 696e 7075 7420  on on the input 
+0000af40: 7061 7261 6d65 7465 7273 2073 6565 3a0a  parameters see:.
+0000af50: 2020 2020 2020 2020 2020 2020 6874 7470              http
+0000af60: 733a 2f2f 7863 6c69 6d2e 7265 6164 7468  s://xclim.readth
+0000af70: 6564 6f63 732e 696f 2f65 6e2f 7374 6162  edocs.io/en/stab
+0000af80: 6c65 2f61 7069 2e68 746d 6c23 7863 6c69  le/api.html#xcli
+0000af90: 6d2e 696e 6469 6361 746f 7273 2e61 746d  m.indicators.atm
+0000afa0: 6f73 2e74 7831 3070 0a20 2020 2020 2020  os.tx10p.       
+0000afb0: 2022 2222 0a20 2020 2020 2020 2064 6120   """.        da 
+0000afc0: 3d20 5f67 6574 5f64 6128 7061 7261 6d73  = _get_da(params
+0000afd0: 2c20 2274 6173 6d61 7822 290a 2020 2020  , "tasmax").    
+0000afe0: 2020 2020 6966 2074 6173 6d61 785f 7065      if tasmax_pe
+0000aff0: 7220 6973 204e 6f6e 653a 0a20 2020 2020  r is None:.     
+0000b000: 2020 2020 2020 2074 6173 6d61 785f 7065         tasmax_pe
+0000b010: 7220 3d20 5f67 6574 5f70 6572 6365 6e74  r = _get_percent
+0000b020: 696c 6528 0a20 2020 2020 2020 2020 2020  ile(.           
+0000b030: 2020 2020 2064 613d 6461 2c0a 2020 2020       da=da,.    
+0000b040: 2020 2020 2020 2020 2020 2020 7065 723d              per=
+0000b050: 3130 2c0a 2020 2020 2020 2020 2020 2020  10,.            
 0000b060: 2020 2020 6261 7365 5f70 6572 696f 645f      base_period_
-0000b070: 7469 6d65 5f72 616e 6765 203d 2042 4153  time_range = BAS
-0000b080: 455f 5045 5249 4f44 0a0a 2020 2020 6465  E_PERIOD..    de
-0000b090: 6620 636f 6d70 7574 6528 0a20 2020 2020  f compute(.     
-0000b0a0: 2020 2062 6173 655f 7065 7269 6f64 5f74     base_period_t
-0000b0b0: 696d 655f 7261 6e67 653d 6261 7365 5f70  ime_range=base_p
-0000b0c0: 6572 696f 645f 7469 6d65 5f72 616e 6765  eriod_time_range
-0000b0d0: 2c0a 2020 2020 2020 2020 7461 736d 696e  ,.        tasmin
-0000b0e0: 5f70 6572 3d74 6173 6d69 6e5f 7065 722c  _per=tasmin_per,
-0000b0f0: 0a20 2020 2020 2020 202a 2a70 6172 616d  .        **param
-0000b100: 732c 0a20 2020 2029 3a0a 2020 2020 2020  s,.    ):.      
-0000b110: 2020 2222 2243 616c 6375 6c61 7465 2066    """Calculate f
-0000b120: 7261 6374 696f 6e20 6f66 2064 6179 7320  raction of days 
-0000b130: 7769 7468 206d 696e 2074 656d 7065 7261  with min tempera
-0000b140: 7475 7265 203c 2031 3074 6820 7065 7263  ture < 10th perc
-0000b150: 656e 7469 6c65 2e0a 0a20 2020 2020 2020  entile...       
-0000b160: 2050 6172 616d 6574 6572 730a 2020 2020   Parameters.    
-0000b170: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20      ----------. 
-0000b180: 2020 2020 2020 2074 6173 6d69 6e5f 7065         tasmin_pe
-0000b190: 723a 2078 722e 4461 7461 4172 7261 792c  r: xr.DataArray,
-0000b1a0: 206f 7074 696f 6e61 6c0a 2020 2020 2020   optional.      
-0000b1b0: 2020 2020 2020 4d69 6e69 6d75 6d20 7465        Minimum te
-0000b1c0: 6d70 6572 6174 7572 6520 3130 7468 2070  mperature 10th p
-0000b1d0: 6572 6365 6e74 696c 6520 7265 6665 7265  ercentile refere
-0000b1e0: 6e63 6520 7661 6c75 652e 0a20 2020 2020  nce value..     
-0000b1f0: 2020 2062 6173 655f 7065 7269 6f64 5f74     base_period_t
-0000b200: 696d 655f 7261 6e67 653a 206c 6973 740a  ime_range: list.
-0000b210: 2020 2020 2020 2020 2020 2020 4c69 7374              List
-0000b220: 2077 6974 6820 6c65 6674 2062 6f75 6e64   with left bound
-0000b230: 2069 7320 7374 6172 7420 7965 6172 2073   is start year s
-0000b240: 7472 696e 6720 616e 6420 7269 6768 7420  tring and right 
-0000b250: 626f 756e 640a 2020 2020 2020 2020 2020  bound.          
-0000b260: 2020 6973 2065 6e64 2079 6561 7220 7374    is end year st
-0000b270: 7269 6e67 2066 6f72 2063 616c 6375 6c61  ring for calcula
-0000b280: 7469 6e67 2060 7461 736d 696e 5f70 6572  ting `tasmin_per
-0000b290: 602e 0a20 2020 2020 2020 2020 2020 2054  `..            T
-0000b2a0: 6869 7320 7769 6c6c 2062 6520 7573 6564  his will be used
-0000b2b0: 206f 6e6c 7920 6966 2060 7461 736d 696e   only if `tasmin
-0000b2c0: 5f70 6572 6020 6973 204e 6f6e 652e 0a0a  _per` is None...
-0000b2d0: 2020 2020 2020 2020 5265 7475 726e 730a          Returns.
-0000b2e0: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d0a          -------.
-0000b2f0: 2020 2020 2020 2020 7861 7272 6179 2e44          xarray.D
-0000b300: 6174 6141 7272 6179 0a20 2020 2020 2020  ataArray.       
-0000b310: 2020 2020 2046 7261 6374 696f 6e20 6f66       Fraction of
-0000b320: 2064 6179 7320 7769 7468 206d 696e 696d   days with minim
-0000b330: 756d 2074 656d 7065 7261 7475 7265 203c  um temperature <
-0000b340: 2031 3074 6820 7065 7263 656e 7469 6c65   10th percentile
-0000b350: 222e 0a0a 2020 2020 2020 2020 4e6f 7465  "...        Note
-0000b360: 730a 2020 2020 2020 2020 2d2d 2d2d 2d0a  s.        -----.
-0000b370: 2020 2020 2020 2020 466f 7220 6d6f 7265          For more
-0000b380: 2069 6e66 6f72 6d61 7469 6f6e 206f 6e20   information on 
-0000b390: 7468 6520 696e 7075 7420 7061 7261 6d65  the input parame
-0000b3a0: 7465 7273 2073 6565 3a0a 2020 2020 2020  ters see:.      
-0000b3b0: 2020 2020 2020 6874 7470 733a 2f2f 7863        https://xc
-0000b3c0: 6c69 6d2e 7265 6164 7468 6564 6f63 732e  lim.readthedocs.
-0000b3d0: 696f 2f65 6e2f 7374 6162 6c65 2f61 7069  io/en/stable/api
-0000b3e0: 2e68 746d 6c23 7863 6c69 6d2e 696e 6469  .html#xclim.indi
-0000b3f0: 6361 746f 7273 2e61 746d 6f73 2e74 6e31  cators.atmos.tn1
-0000b400: 3070 0a20 2020 2020 2020 2022 2222 0a20  0p.        """. 
-0000b410: 2020 2020 2020 2064 6120 3d20 5f67 6574         da = _get
-0000b420: 5f64 6128 7061 7261 6d73 2c20 2274 6173  _da(params, "tas
-0000b430: 6d69 6e22 290a 2020 2020 2020 2020 6966  min").        if
-0000b440: 2074 6173 6d69 6e5f 7065 7220 6973 204e   tasmin_per is N
-0000b450: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-0000b460: 2074 6173 6d69 6e5f 7065 7220 3d20 5f67   tasmin_per = _g
-0000b470: 6574 5f70 6572 6365 6e74 696c 6528 0a20  et_percentile(. 
-0000b480: 2020 2020 2020 2020 2020 2020 2020 2064                 d
-0000b490: 613d 6461 2c0a 2020 2020 2020 2020 2020  a=da,.          
-0000b4a0: 2020 2020 2020 7065 723d 3130 2c0a 2020        per=10,.  
-0000b4b0: 2020 2020 2020 2020 2020 2020 2020 6261                ba
-0000b4c0: 7365 5f70 6572 696f 645f 7469 6d65 5f72  se_period_time_r
-0000b4d0: 616e 6765 3d62 6173 655f 7065 7269 6f64  ange=base_period
-0000b4e0: 5f74 696d 655f 7261 6e67 652c 0a20 2020  _time_range,.   
-0000b4f0: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
-0000b500: 2020 2077 6974 6820 6461 736b 2e63 6f6e     with dask.con
-0000b510: 6669 672e 7365 7428 2a2a 7b22 6172 7261  fig.set(**{"arra
-0000b520: 792e 736c 6963 696e 672e 7370 6c69 745f  y.slicing.split_
-0000b530: 6c61 7267 655f 6368 756e 6b73 223a 2046  large_chunks": F
-0000b540: 616c 7365 7d29 3a0a 2020 2020 2020 2020  alse}):.        
-0000b550: 2020 2020 7265 7475 726e 2078 632e 6174      return xc.at
-0000b560: 6d6f 732e 746e 3130 7028 0a20 2020 2020  mos.tn10p(.     
-0000b570: 2020 2020 2020 2020 2020 2074 6173 6d69             tasmi
-0000b580: 6e5f 7065 723d 7461 736d 696e 5f70 6572  n_per=tasmin_per
-0000b590: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0000b5a0: 2020 2a2a 7061 7261 6d73 2c0a 2020 2020    **params,.    
-0000b5b0: 2020 2020 2020 2020 290a 0a0a 636c 6173          )...clas
-0000b5c0: 7320 544e 3930 703a 0a20 2020 2022 2222  s TN90p:.    """
-0000b5d0: 4672 6163 7469 6f6e 206f 6620 6461 7973  Fraction of days
-0000b5e0: 2077 6974 6820 6d69 6e20 7465 6d70 6572   with min temper
-0000b5f0: 6174 7572 6520 3e20 3930 7468 2070 6572  ature > 90th per
-0000b600: 6365 6e74 696c 652e 2222 220a 0a20 2020  centile."""..   
-0000b610: 2074 6173 6d69 6e5f 7065 7220 3d20 4e6f   tasmin_per = No
-0000b620: 6e65 0a20 2020 2062 6173 655f 7065 7269  ne.    base_peri
-0000b630: 6f64 5f74 696d 655f 7261 6e67 6520 3d20  od_time_range = 
-0000b640: 4241 5345 5f50 4552 494f 440a 0a20 2020  BASE_PERIOD..   
-0000b650: 2064 6566 2063 6f6d 7075 7465 280a 2020   def compute(.  
-0000b660: 2020 2020 2020 6261 7365 5f70 6572 696f        base_perio
-0000b670: 645f 7469 6d65 5f72 616e 6765 3d62 6173  d_time_range=bas
-0000b680: 655f 7065 7269 6f64 5f74 696d 655f 7261  e_period_time_ra
-0000b690: 6e67 652c 0a20 2020 2020 2020 2074 6173  nge,.        tas
-0000b6a0: 6d69 6e5f 7065 723d 7461 736d 696e 5f70  min_per=tasmin_p
-0000b6b0: 6572 2c0a 2020 2020 2020 2020 2a2a 7061  er,.        **pa
-0000b6c0: 7261 6d73 2c0a 2020 2020 293a 0a20 2020  rams,.    ):.   
-0000b6d0: 2020 2020 2022 2222 4361 6c63 756c 6174       """Calculat
-0000b6e0: 6520 6672 6163 7469 6f6e 206f 6620 6461  e fraction of da
-0000b6f0: 7973 2077 6974 6820 6d69 6e20 7465 6d70  ys with min temp
-0000b700: 6572 6174 7572 6520 3e20 3930 7468 2070  erature > 90th p
-0000b710: 6572 6365 6e74 696c 652e 0a0a 2020 2020  ercentile...    
-0000b720: 2020 2020 5061 7261 6d65 7465 7273 0a20      Parameters. 
-0000b730: 2020 2020 2020 202d 2d2d 2d2d 2d2d 2d2d         ---------
-0000b740: 2d0a 2020 2020 2020 2020 7461 736d 696e  -.        tasmin
-0000b750: 5f70 6572 3a20 7872 2e44 6174 6141 7272  _per: xr.DataArr
-0000b760: 6179 2c20 6f70 7469 6f6e 616c 0a20 2020  ay, optional.   
-0000b770: 2020 2020 2020 2020 204d 696e 696d 756d           Minimum
-0000b780: 2074 656d 7065 7261 7475 7265 2039 3074   temperature 90t
-0000b790: 6820 7065 7263 656e 7469 6c65 2072 6566  h percentile ref
-0000b7a0: 6572 656e 6365 2076 616c 7565 2e0a 2020  erence value..  
-0000b7b0: 2020 2020 2020 6261 7365 5f70 6572 696f        base_perio
-0000b7c0: 645f 7469 6d65 5f72 616e 6765 3a20 6c69  d_time_range: li
-0000b7d0: 7374 0a20 2020 2020 2020 2020 2020 204c  st.            L
-0000b7e0: 6973 7420 7769 7468 206c 6566 7420 626f  ist with left bo
-0000b7f0: 756e 6420 6973 2073 7461 7274 2079 6561  und is start yea
-0000b800: 7220 7374 7269 6e67 2061 6e64 2072 6967  r string and rig
-0000b810: 6874 2062 6f75 6e64 0a20 2020 2020 2020  ht bound.       
-0000b820: 2020 2020 2069 7320 656e 6420 7965 6172       is end year
-0000b830: 2073 7472 696e 6720 666f 7220 6361 6c63   string for calc
-0000b840: 756c 6174 696e 6720 6074 6173 6d69 6e5f  ulating `tasmin_
-0000b850: 7065 7260 2e0a 2020 2020 2020 2020 2020  per`..          
-0000b860: 2020 5468 6973 2077 696c 6c20 6265 2075    This will be u
-0000b870: 7365 6420 6f6e 6c79 2069 6620 6074 6173  sed only if `tas
-0000b880: 6d69 6e5f 7065 7260 2069 7320 4e6f 6e65  min_per` is None
-0000b890: 2e0a 0a20 2020 2020 2020 2052 6574 7572  ...        Retur
-0000b8a0: 6e73 0a20 2020 2020 2020 202d 2d2d 2d2d  ns.        -----
-0000b8b0: 2d2d 0a20 2020 2020 2020 2078 6172 7261  --.        xarra
-0000b8c0: 792e 4461 7461 4172 7261 790a 2020 2020  y.DataArray.    
-0000b8d0: 2020 2020 2020 2020 4672 6163 7469 6f6e          Fraction
-0000b8e0: 206f 6620 6461 7973 2077 6974 6820 6d69   of days with mi
-0000b8f0: 6e69 6d75 6d20 7465 6d70 6572 6174 7572  nimum temperatur
-0000b900: 6520 3e20 3930 7468 2070 6572 6365 6e74  e > 90th percent
-0000b910: 696c 6522 2e0a 0a20 2020 2020 2020 204e  ile"...        N
-0000b920: 6f74 6573 0a20 2020 2020 2020 202d 2d2d  otes.        ---
-0000b930: 2d2d 0a20 2020 2020 2020 2046 6f72 206d  --.        For m
-0000b940: 6f72 6520 696e 666f 726d 6174 696f 6e20  ore information 
-0000b950: 6f6e 2074 6865 2069 6e70 7574 2070 6172  on the input par
-0000b960: 616d 6574 6572 7320 7365 653a 0a20 2020  ameters see:.   
-0000b970: 2020 2020 2020 2020 2068 7474 7073 3a2f           https:/
-0000b980: 2f78 636c 696d 2e72 6561 6474 6865 646f  /xclim.readthedo
-0000b990: 6373 2e69 6f2f 656e 2f73 7461 626c 652f  cs.io/en/stable/
-0000b9a0: 6170 692e 6874 6d6c 2378 636c 696d 2e69  api.html#xclim.i
-0000b9b0: 6e64 6963 6174 6f72 732e 6174 6d6f 732e  ndicators.atmos.
-0000b9c0: 7478 3930 700a 2020 2020 2020 2020 2222  tx90p.        ""
-0000b9d0: 220a 2020 2020 2020 2020 6461 203d 205f  ".        da = _
-0000b9e0: 6765 745f 6461 2870 6172 616d 732c 2022  get_da(params, "
-0000b9f0: 7461 736d 696e 2229 0a20 2020 2020 2020  tasmin").       
-0000ba00: 2069 6620 7461 736d 696e 5f70 6572 2069   if tasmin_per i
-0000ba10: 7320 4e6f 6e65 3a0a 2020 2020 2020 2020  s None:.        
-0000ba20: 2020 2020 7461 736d 696e 5f70 6572 203d      tasmin_per =
-0000ba30: 205f 6765 745f 7065 7263 656e 7469 6c65   _get_percentile
-0000ba40: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-0000ba50: 2020 6461 3d64 612c 0a20 2020 2020 2020    da=da,.       
-0000ba60: 2020 2020 2020 2020 2070 6572 3d39 302c           per=90,
-0000ba70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000ba80: 2062 6173 655f 7065 7269 6f64 5f74 696d   base_period_tim
-0000ba90: 655f 7261 6e67 653d 6261 7365 5f70 6572  e_range=base_per
-0000baa0: 696f 645f 7469 6d65 5f72 616e 6765 2c0a  iod_time_range,.
-0000bab0: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-0000bac0: 2020 2020 2020 7769 7468 2064 6173 6b2e        with dask.
-0000bad0: 636f 6e66 6967 2e73 6574 282a 2a7b 2261  config.set(**{"a
-0000bae0: 7272 6179 2e73 6c69 6369 6e67 2e73 706c  rray.slicing.spl
-0000baf0: 6974 5f6c 6172 6765 5f63 6875 6e6b 7322  it_large_chunks"
-0000bb00: 3a20 4661 6c73 657d 293a 0a20 2020 2020  : False}):.     
-0000bb10: 2020 2020 2020 2072 6574 7572 6e20 7863         return xc
-0000bb20: 2e61 746d 6f73 2e74 6e39 3070 280a 2020  .atmos.tn90p(.  
-0000bb30: 2020 2020 2020 2020 2020 2020 2020 7461                ta
-0000bb40: 736d 696e 5f70 6572 3d74 6173 6d69 6e5f  smin_per=tasmin_
-0000bb50: 7065 722c 0a20 2020 2020 2020 2020 2020  per,.           
-0000bb60: 2020 2020 202a 2a70 6172 616d 732c 0a20       **params,. 
-0000bb70: 2020 2020 2020 2020 2020 2029 0a0a 0a63             )...c
-0000bb80: 6c61 7373 2054 4e6e 3a0a 2020 2020 2222  lass TNn:.    ""
-0000bb90: 224d 696e 696d 756d 206d 696e 696d 756d  "Minimum minimum
-0000bba0: 2074 656d 7065 7261 7475 7265 2028 7461   temperature (ta
-0000bbb0: 736d 696e 292e 2222 220a 0a20 2020 2064  smin)."""..    d
-0000bbc0: 6566 2063 6f6d 7075 7465 282a 2a70 6172  ef compute(**par
-0000bbd0: 616d 7329 3a0a 2020 2020 2020 2020 2222  ams):.        ""
-0000bbe0: 2243 616c 6375 6c61 7465 206d 696e 696d  "Calculate minim
-0000bbf0: 756d 2064 6169 6c79 206d 696e 696d 756d  um daily minimum
-0000bc00: 2074 656d 7065 7261 7475 7265 2e0a 0a20   temperature... 
-0000bc10: 2020 2020 2020 2052 6574 7572 6e73 0a20         Returns. 
-0000bc20: 2020 2020 2020 202d 2d2d 2d2d 2d2d 0a20         -------. 
-0000bc30: 2020 2020 2020 2078 6172 7261 792e 4461         xarray.Da
-0000bc40: 7461 4172 7261 790a 2020 2020 2020 2020  taArray.        
-0000bc50: 2020 2020 4d69 6e69 6d75 6d20 6461 696c      Minimum dail
-0000bc60: 7920 6d69 6e69 6d75 6d20 7465 6d70 6572  y minimum temper
-0000bc70: 6174 7572 652e 0a0a 2020 2020 2020 2020  ature...        
-0000bc80: 4e6f 7465 730a 2020 2020 2020 2020 2d2d  Notes.        --
-0000bc90: 2d2d 2d0a 2020 2020 2020 2020 466f 7220  ---.        For 
-0000bca0: 696e 666f 726d 6174 696f 6e20 6f6e 2074  information on t
-0000bcb0: 6865 2069 6e70 7574 2070 6172 616d 6574  he input paramet
-0000bcc0: 6572 7320 7365 653a 0a20 2020 2020 2020  ers see:.       
-0000bcd0: 2020 2020 2068 7474 7073 3a2f 2f78 636c       https://xcl
-0000bce0: 696d 2e72 6561 6474 6865 646f 6373 2e69  im.readthedocs.i
-0000bcf0: 6f2f 656e 2f73 7461 626c 652f 6170 692e  o/en/stable/api.
-0000bd00: 6874 6d6c 2378 636c 696d 2e69 6e64 6963  html#xclim.indic
-0000bd10: 6174 6f72 732e 6174 6d6f 732e 746e 5f6d  ators.atmos.tn_m
-0000bd20: 696e 0a20 2020 2020 2020 2022 2222 0a20  in.        """. 
-0000bd30: 2020 2020 2020 2072 6574 7572 6e20 7863         return xc
-0000bd40: 2e61 746d 6f73 2e74 6e5f 6d69 6e28 2a2a  .atmos.tn_min(**
-0000bd50: 7061 7261 6d73 290a 0a0a 636c 6173 7320  params)...class 
-0000bd60: 544e 783a 0a20 2020 2022 2222 4d61 7869  TNx:.    """Maxi
-0000bd70: 6d75 6d20 6d69 6e69 6d75 6d20 7465 6d70  mum minimum temp
-0000bd80: 6572 6174 7572 6520 2874 6173 6d69 6e29  erature (tasmin)
-0000bd90: 2e22 2222 0a0a 2020 2020 6465 6620 636f  ."""..    def co
-0000bda0: 6d70 7574 6528 2a2a 7061 7261 6d73 293a  mpute(**params):
-0000bdb0: 0a20 2020 2020 2020 2022 2222 4361 6c63  .        """Calc
-0000bdc0: 756c 6174 6520 6d61 7869 6d75 6d20 6461  ulate maximum da
-0000bdd0: 696c 7920 6d69 6e69 6d75 6d20 7465 6d70  ily minimum temp
-0000bde0: 6572 6174 7572 652e 0a0a 2020 2020 2020  erature...      
-0000bdf0: 2020 5265 7475 726e 730a 2020 2020 2020    Returns.      
-0000be00: 2020 2d2d 2d2d 2d2d 2d0a 2020 2020 2020    -------.      
-0000be10: 2020 7861 7272 6179 2e44 6174 6141 7272    xarray.DataArr
-0000be20: 6179 0a20 2020 2020 2020 2020 2020 204d  ay.            M
-0000be30: 6178 696d 756d 2064 6169 6c79 206d 696e  aximum daily min
-0000be40: 696d 756d 2074 656d 7065 7261 7475 7265  imum temperature
-0000be50: 2e0a 0a20 2020 2020 2020 204e 6f74 6573  ...        Notes
-0000be60: 0a20 2020 2020 2020 202d 2d2d 2d2d 0a20  .        -----. 
-0000be70: 2020 2020 2020 2046 6f72 2069 6e66 6f72         For infor
-0000be80: 6d61 7469 6f6e 206f 6e20 7468 6520 696e  mation on the in
-0000be90: 7075 7420 7061 7261 6d65 7465 7273 2073  put parameters s
-0000bea0: 6565 3a0a 2020 2020 2020 2020 2020 2020  ee:.            
-0000beb0: 6874 7470 733a 2f2f 7863 6c69 6d2e 7265  https://xclim.re
-0000bec0: 6164 7468 6564 6f63 732e 696f 2f65 6e2f  adthedocs.io/en/
-0000bed0: 7374 6162 6c65 2f61 7069 2e68 746d 6c23  stable/api.html#
-0000bee0: 7863 6c69 6d2e 696e 6469 6361 746f 7273  xclim.indicators
-0000bef0: 2e61 746d 6f73 2e74 6e5f 6d61 780a 2020  .atmos.tn_max.  
-0000bf00: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-0000bf10: 2020 7265 7475 726e 2078 632e 6174 6d6f    return xc.atmo
-0000bf20: 732e 746e 5f6d 6178 282a 2a70 6172 616d  s.tn_max(**param
-0000bf30: 7329 0a0a 0a63 6c61 7373 2057 443a 0a20  s)...class WD:. 
-0000bf40: 2020 2022 2222 4e75 6d62 6572 206f 6620     """Number of 
-0000bf50: 7761 726d 2061 6e64 2064 7279 2064 6179  warm and dry day
-0000bf60: 7320 2874 6173 2c20 7072 292e 2222 220a  s (tas, pr).""".
-0000bf70: 0a20 2020 2074 6173 5f70 6572 203d 204e  .    tas_per = N
-0000bf80: 6f6e 650a 2020 2020 7072 5f70 6572 203d  one.    pr_per =
-0000bf90: 204e 6f6e 650a 2020 2020 6261 7365 5f70   None.    base_p
-0000bfa0: 6572 696f 645f 7469 6d65 5f72 616e 6765  eriod_time_range
-0000bfb0: 203d 2042 4153 455f 5045 5249 4f44 0a0a   = BASE_PERIOD..
-0000bfc0: 2020 2020 6465 6620 636f 6d70 7574 6528      def compute(
-0000bfd0: 0a20 2020 2020 2020 2062 6173 655f 7065  .        base_pe
-0000bfe0: 7269 6f64 5f74 696d 655f 7261 6e67 653d  riod_time_range=
-0000bff0: 6261 7365 5f70 6572 696f 645f 7469 6d65  base_period_time
-0000c000: 5f72 616e 6765 2c0a 2020 2020 2020 2020  _range,.        
-0000c010: 7461 735f 7065 723d 7461 735f 7065 722c  tas_per=tas_per,
-0000c020: 0a20 2020 2020 2020 2070 725f 7065 723d  .        pr_per=
-0000c030: 7072 5f70 6572 2c0a 2020 2020 2020 2020  pr_per,.        
-0000c040: 2a2a 7061 7261 6d73 2c0a 2020 2020 293a  **params,.    ):
-0000c050: 0a20 2020 2020 2020 2022 2222 4361 6c63  .        """Calc
-0000c060: 756c 6174 6520 6e75 6d62 6572 206f 6620  ulate number of 
-0000c070: 7761 726d 2061 6e64 2064 7279 2064 6179  warm and dry day
-0000c080: 732e 0a0a 2020 2020 2020 2020 5061 7261  s...        Para
-0000c090: 6d65 7465 7273 0a20 2020 2020 2020 202d  meters.        -
-0000c0a0: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 2020  ---------.      
-0000c0b0: 2020 7461 735f 7065 723a 2078 722e 4461    tas_per: xr.Da
-0000c0c0: 7461 4172 7261 792c 206f 7074 696f 6e61  taArray, optiona
-0000c0d0: 6c0a 2020 2020 2020 2020 2020 2020 4d65  l.            Me
-0000c0e0: 616e 2074 656d 7065 7261 7475 7265 2037  an temperature 7
-0000c0f0: 3574 6820 7065 7263 656e 7469 6c65 2072  5th percentile r
-0000c100: 6566 6572 656e 6365 2076 616c 7565 2061  eference value a
-0000c110: 626f 7665 2077 6869 6368 0a20 2020 2020  bove which.     
-0000c120: 2020 2020 2020 2061 2064 6179 2069 7320         a day is 
-0000c130: 636f 6e73 6964 6572 6564 2061 7320 6120  considered as a 
-0000c140: 7761 726d 2064 6179 2e0a 2020 2020 2020  warm day..      
-0000c150: 2020 7072 5f70 6572 3a20 7872 2e44 6174    pr_per: xr.Dat
-0000c160: 6141 7272 6179 2c20 6f70 7469 6f6e 616c  aArray, optional
-0000c170: 0a20 2020 2020 2020 2020 2020 2050 7265  .            Pre
-0000c180: 6369 7069 7461 7469 6f6e 2032 3574 6820  cipitation 25th 
-0000c190: 7065 7263 656e 7469 6c65 2072 6566 6572  percentile refer
-0000c1a0: 656e 6365 2076 616c 7565 2062 656c 6f77  ence value below
-0000c1b0: 2077 6869 6368 0a20 2020 2020 2020 2020   which.         
-0000c1c0: 2020 2061 2064 6179 2069 7320 636f 6e73     a day is cons
-0000c1d0: 6964 6572 6564 2061 7320 6120 6472 7920  idered as a dry 
-0000c1e0: 6461 792e 0a20 2020 2020 2020 2062 6173  day..        bas
-0000c1f0: 655f 7065 7269 6f64 5f74 696d 655f 7261  e_period_time_ra
-0000c200: 6e67 653a 206c 6973 740a 2020 2020 2020  nge: list.      
-0000c210: 2020 2020 2020 4c69 7374 2077 6974 6820        List with 
-0000c220: 6c65 6674 2062 6f75 6e64 2069 7320 7374  left bound is st
-0000c230: 6172 7420 7965 6172 2073 7472 696e 6720  art year string 
-0000c240: 616e 6420 7269 6768 7420 626f 756e 640a  and right bound.
-0000c250: 2020 2020 2020 2020 2020 2020 6973 2065              is e
-0000c260: 6e64 2079 6561 7220 7374 7269 6e67 2066  nd year string f
-0000c270: 6f72 2063 616c 6375 6c61 7469 6e67 2060  or calculating `
-0000c280: 7461 735f 7065 7260 2061 6e64 2f6f 7220  tas_per` and/or 
-0000c290: 6070 725f 7065 7260 2e0a 2020 2020 2020  `pr_per`..      
-0000c2a0: 2020 2020 2020 5468 6973 2077 696c 6c20        This will 
-0000c2b0: 6265 2075 7365 6420 6f6e 6c79 2069 6620  be used only if 
-0000c2c0: 6074 6173 5f70 6572 6020 616e 642f 6f72  `tas_per` and/or
-0000c2d0: 2060 7072 5f70 6572 6020 6973 204e 6f6e   `pr_per` is Non
-0000c2e0: 652e 0a0a 2020 2020 2020 2020 5265 7475  e...        Retu
-0000c2f0: 726e 730a 2020 2020 2020 2020 2d2d 2d2d  rns.        ----
-0000c300: 2d2d 2d0a 2020 2020 2020 2020 7861 7272  ---.        xarr
-0000c310: 6179 2e44 6174 6141 7272 6179 3a0a 2020  ay.DataArray:.  
-0000c320: 2020 2020 2020 2020 2020 4e75 6d62 6572            Number
-0000c330: 206f 6620 6461 7973 2077 6865 7265 2077   of days where w
-0000c340: 6172 6d20 616e 6420 6472 7920 636f 6e64  arm and dry cond
-0000c350: 6974 696f 6e73 2063 6f69 6e63 6964 652e  itions coincide.
-0000c360: 0a20 2020 2020 2020 2020 2020 2049 6620  .            If 
-0000c370: 7465 6d70 6572 6174 7572 6520 6973 2061  temperature is a
-0000c380: 626f 7665 207b 7461 735f 7065 727d 2061  bove {tas_per} a
-0000c390: 2064 6179 2069 7320 636f 6e73 6964 6572   day is consider
-0000c3a0: 6564 2061 7320 610a 2020 2020 2020 2020  ed as a.        
-0000c3b0: 2020 2020 7761 726d 2064 6179 2e0a 2020      warm day..  
-0000c3c0: 2020 2020 2020 2020 2020 4966 2070 7265            If pre
-0000c3d0: 6369 7069 7461 7469 6f6e 2069 7320 6265  cipitation is be
-0000c3e0: 6c6f 7720 7b70 725f 7065 727d 2061 2064  low {pr_per} a d
-0000c3f0: 6179 2069 7320 636f 6e73 6964 6572 6564  ay is considered
-0000c400: 2061 7320 610a 2020 2020 2020 2020 2020   as a.          
-0000c410: 2020 6472 7920 6461 792e 0a0a 2020 2020    dry day...    
-0000c420: 2020 2020 4e6f 7465 730a 2020 2020 2020      Notes.      
-0000c430: 2020 2d2d 2d2d 2d0a 2020 2020 2020 2020    -----.        
-0000c440: 466f 7220 6d6f 7265 2069 6e66 6f72 6d61  For more informa
-0000c450: 7469 6f6e 206f 6e20 7468 6520 696e 7075  tion on the inpu
-0000c460: 7420 7061 7261 6d65 7465 7273 2073 6565  t parameters see
-0000c470: 3a0a 2020 2020 2020 2020 2020 2020 6874  :.            ht
-0000c480: 7470 733a 2f2f 7863 6c69 6d2e 7265 6164  tps://xclim.read
-0000c490: 7468 6564 6f63 732e 696f 2f65 6e2f 7374  thedocs.io/en/st
-0000c4a0: 6162 6c65 2f61 7069 2e68 746d 6c23 7863  able/api.html#xc
-0000c4b0: 6c69 6d2e 696e 6469 6361 746f 7273 2e61  lim.indicators.a
-0000c4c0: 746d 6f73 2e77 6172 6d5f 616e 645f 6472  tmos.warm_and_dr
-0000c4d0: 795f 6461 7973 0a20 2020 2020 2020 2022  y_days.        "
-0000c4e0: 2222 0a20 2020 2020 2020 2064 615f 7461  "".        da_ta
-0000c4f0: 7320 3d20 5f67 6574 5f64 6128 7061 7261  s = _get_da(para
-0000c500: 6d73 2c20 2274 6173 2229 0a20 2020 2020  ms, "tas").     
-0000c510: 2020 2064 615f 7072 203d 205f 6765 745f     da_pr = _get_
-0000c520: 6461 2870 6172 616d 732c 2022 7072 2229  da(params, "pr")
-0000c530: 0a20 2020 2020 2020 2069 6620 7461 735f  .        if tas_
-0000c540: 7065 7220 6973 204e 6f6e 653a 0a20 2020  per is None:.   
-0000c550: 2020 2020 2020 2020 2074 6173 5f70 6572           tas_per
-0000c560: 203d 205f 6765 745f 7065 7263 656e 7469   = _get_percenti
-0000c570: 6c65 280a 2020 2020 2020 2020 2020 2020  le(.            
-0000c580: 2020 2020 6461 3d64 615f 7461 732c 0a20      da=da_tas,. 
-0000c590: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-0000c5a0: 6572 3d37 352c 0a20 2020 2020 2020 2020  er=75,.         
-0000c5b0: 2020 2020 2020 2062 6173 655f 7065 7269         base_peri
-0000c5c0: 6f64 5f74 696d 655f 7261 6e67 653d 6261  od_time_range=ba
-0000c5d0: 7365 5f70 6572 696f 645f 7469 6d65 5f72  se_period_time_r
-0000c5e0: 616e 6765 2c0a 2020 2020 2020 2020 2020  ange,.          
-0000c5f0: 2020 290a 2020 2020 2020 2020 6966 2070    ).        if p
-0000c600: 725f 7065 7220 6973 204e 6f6e 653a 0a20  r_per is None:. 
-0000c610: 2020 2020 2020 2020 2020 2064 615f 7072             da_pr
-0000c620: 5f66 203d 205f 6669 6c74 6572 5f6f 7574  _f = _filter_out
-0000c630: 5f73 6d61 6c6c 5f76 616c 7565 7328 0a20  _small_values(. 
-0000c640: 2020 2020 2020 2020 2020 2020 2020 2064                 d
-0000c650: 615f 7072 2c0a 2020 2020 2020 2020 2020  a_pr,.          
-0000c660: 2020 2020 2020 2231 206d 6d2f 6461 7922        "1 mm/day"
-0000c670: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0000c680: 2020 636f 6e74 6578 743d 2268 7964 726f    context="hydro
-0000c690: 222c 0a20 2020 2020 2020 2020 2020 2029  ",.            )
-0000c6a0: 0a20 2020 2020 2020 2020 2020 2070 725f  .            pr_
-0000c6b0: 7065 7220 3d20 5f67 6574 5f70 6572 6365  per = _get_perce
-0000c6c0: 6e74 696c 6528 0a20 2020 2020 2020 2020  ntile(.         
-0000c6d0: 2020 2020 2020 2064 613d 6461 5f70 725f         da=da_pr_
-0000c6e0: 662c 0a20 2020 2020 2020 2020 2020 2020  f,.             
-0000c6f0: 2020 2070 6572 3d32 352c 0a20 2020 2020     per=25,.     
-0000c700: 2020 2020 2020 2020 2020 2062 6173 655f             base_
-0000c710: 7065 7269 6f64 5f74 696d 655f 7261 6e67  period_time_rang
-0000c720: 653d 6261 7365 5f70 6572 696f 645f 7469  e=base_period_ti
-0000c730: 6d65 5f72 616e 6765 2c0a 2020 2020 2020  me_range,.      
-0000c740: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-0000c750: 7769 7468 2064 6173 6b2e 636f 6e66 6967  with dask.config
-0000c760: 2e73 6574 282a 2a7b 2261 7272 6179 2e73  .set(**{"array.s
-0000c770: 6c69 6369 6e67 2e73 706c 6974 5f6c 6172  licing.split_lar
-0000c780: 6765 5f63 6875 6e6b 7322 3a20 4661 6c73  ge_chunks": Fals
-0000c790: 657d 293a 0a20 2020 2020 2020 2020 2020  e}):.           
-0000c7a0: 2072 6574 7572 6e20 7863 2e61 746d 6f73   return xc.atmos
-0000c7b0: 2e77 6172 6d5f 616e 645f 6472 795f 6461  .warm_and_dry_da
-0000c7c0: 7973 280a 2020 2020 2020 2020 2020 2020  ys(.            
-0000c7d0: 2020 2020 7461 735f 7065 723d 7461 735f      tas_per=tas_
-0000c7e0: 7065 722c 0a20 2020 2020 2020 2020 2020  per,.           
-0000c7f0: 2020 2020 2070 725f 7065 723d 7072 5f70       pr_per=pr_p
-0000c800: 6572 2c0a 2020 2020 2020 2020 2020 2020  er,.            
-0000c810: 2020 2020 2a2a 7061 7261 6d73 2c0a 2020      **params,.  
-0000c820: 2020 2020 2020 2020 2020 290a 0a0a 636c            )...cl
-0000c830: 6173 7320 5753 4449 3a0a 2020 2020 2222  ass WSDI:.    ""
-0000c840: 2257 6172 6d20 7370 656c 6c20 6475 7261  "Warm spell dura
-0000c850: 7469 6f6e 2069 6e64 6578 2028 7461 736d  tion index (tasm
-0000c860: 6178 292e 2222 220a 0a20 2020 2077 696e  ax)."""..    win
-0000c870: 646f 7720 3d20 360a 2020 2020 7461 736d  dow = 6.    tasm
-0000c880: 6178 5f70 6572 203d 204e 6f6e 650a 2020  ax_per = None.  
-0000c890: 2020 6261 7365 5f70 6572 696f 645f 7469    base_period_ti
-0000c8a0: 6d65 5f72 616e 6765 203d 2042 4153 455f  me_range = BASE_
-0000c8b0: 5045 5249 4f44 0a0a 2020 2020 6465 6620  PERIOD..    def 
-0000c8c0: 636f 6d70 7574 6528 0a20 2020 2020 2020  compute(.       
-0000c8d0: 2077 696e 646f 773d 7769 6e64 6f77 2c0a   window=window,.
-0000c8e0: 2020 2020 2020 2020 6261 7365 5f70 6572          base_per
-0000c8f0: 696f 645f 7469 6d65 5f72 616e 6765 3d62  iod_time_range=b
-0000c900: 6173 655f 7065 7269 6f64 5f74 696d 655f  ase_period_time_
-0000c910: 7261 6e67 652c 0a20 2020 2020 2020 2074  range,.        t
-0000c920: 6173 6d61 785f 7065 723d 7461 736d 6178  asmax_per=tasmax
-0000c930: 5f70 6572 2c0a 2020 2020 2020 2020 2a2a  _per,.        **
-0000c940: 7061 7261 6d73 2c0a 2020 2020 293a 0a20  params,.    ):. 
-0000c950: 2020 2020 2020 2022 2222 4361 6c63 756c         """Calcul
-0000c960: 6174 6520 7761 726d 2073 7065 6c6c 2064  ate warm spell d
-0000c970: 7572 6174 696f 6e20 696e 6465 782e 0a0a  uration index...
-0000c980: 2020 2020 2020 2020 5061 7261 6d65 7465          Paramete
-0000c990: 7273 0a20 2020 2020 2020 202d 2d2d 2d2d  rs.        -----
-0000c9a0: 2d2d 2d2d 2d0a 2020 2020 2020 2020 7769  -----.        wi
-0000c9b0: 6e64 6f77 3a20 696e 740a 2020 2020 2020  ndow: int.      
-0000c9c0: 2020 2020 2020 4d69 6e69 6d75 6d20 6e75        Minimum nu
-0000c9d0: 6d62 6572 206f 6620 6461 7973 2077 6974  mber of days wit
-0000c9e0: 6820 7465 6d70 6572 6174 7572 6520 6162  h temperature ab
-0000c9f0: 6f76 6520 6074 6173 6d61 785f 7065 7260  ove `tasmax_per`
-0000ca00: 0a20 2020 2020 2020 2020 2020 2074 6f20  .            to 
-0000ca10: 7175 616c 6966 7920 6173 2061 2077 6172  qualify as a war
-0000ca20: 6d20 7370 656c 6c20 2864 6566 6175 6c74  m spell (default
-0000ca30: 3a20 3629 2e0a 2020 2020 2020 2020 7461  : 6)..        ta
-0000ca40: 736d 696e 5f70 6572 3a20 7872 2e44 6174  smin_per: xr.Dat
-0000ca50: 6141 7272 6179 2c20 6f70 7469 6f6e 616c  aArray, optional
-0000ca60: 0a20 2020 2020 2020 2020 2020 204d 6178  .            Max
-0000ca70: 696d 756d 2074 656d 7065 7261 7475 7265  imum temperature
-0000ca80: 2039 3074 6820 7065 7263 656e 7469 6c65   90th percentile
-0000ca90: 2072 6566 6572 656e 6365 2076 616c 7565   reference value
-0000caa0: 2e0a 2020 2020 2020 2020 6261 7365 5f70  ..        base_p
-0000cab0: 6572 696f 645f 7469 6d65 5f72 616e 6765  eriod_time_range
-0000cac0: 3a20 6c69 7374 0a20 2020 2020 2020 2020  : list.         
-0000cad0: 2020 204c 6973 7420 7769 7468 206c 6566     List with lef
-0000cae0: 7420 626f 756e 6420 6973 2073 7461 7274  t bound is start
-0000caf0: 2079 6561 7220 7374 7269 6e67 2061 6e64   year string and
-0000cb00: 2072 6967 6874 2062 6f75 6e64 0a20 2020   right bound.   
-0000cb10: 2020 2020 2020 2020 2069 7320 656e 6420           is end 
-0000cb20: 7965 6172 2073 7472 696e 6720 666f 7220  year string for 
-0000cb30: 6361 6c63 756c 6174 696e 6720 6074 6173  calculating `tas
-0000cb40: 6d61 785f 7065 7260 2e0a 2020 2020 2020  max_per`..      
-0000cb50: 2020 2020 2020 5468 6973 2077 696c 6c20        This will 
-0000cb60: 6265 2075 7365 6420 6f6e 6c79 2069 6620  be used only if 
-0000cb70: 6074 6173 6d61 785f 7065 7260 2069 7320  `tasmax_per` is 
-0000cb80: 4e6f 6e65 2e0a 0a20 2020 2020 2020 2052  None...        R
-0000cb90: 6574 7572 6e73 0a20 2020 2020 2020 202d  eturns.        -
-0000cba0: 2d2d 2d2d 2d2d 0a20 2020 2020 2020 2078  ------.        x
-0000cbb0: 6172 7261 792e 4461 7461 4172 7261 790a  array.DataArray.
-0000cbc0: 2020 2020 2020 2020 2020 2020 4e75 6d62              Numb
-0000cbd0: 6572 206f 6620 6461 7973 2070 6172 7420  er of days part 
-0000cbe0: 6f66 2061 2039 3074 6820 7065 7263 656e  of a 90th percen
-0000cbf0: 7469 6c65 2077 6172 6d20 7370 656c 6c2e  tile warm spell.
-0000cc00: 0a20 2020 2020 2020 2020 2020 2041 7420  .            At 
-0000cc10: 6c65 6173 7420 7b77 696e 646f 777d 2063  least {window} c
-0000cc20: 6f6e 7365 6375 7469 7665 2064 6179 732e  onsecutive days.
-0000cc30: 0a0a 2020 2020 2020 2020 4e6f 7465 730a  ..        Notes.
-0000cc40: 2020 2020 2020 2020 2d2d 2d2d 2d0a 2020          -----.  
-0000cc50: 2020 2020 2020 466f 7220 6d6f 7265 2069        For more i
-0000cc60: 6e66 6f72 6d61 7469 6f6e 206f 6e20 7468  nformation on th
-0000cc70: 6520 696e 7075 7420 7061 7261 6d65 7465  e input paramete
-0000cc80: 7273 2073 6565 3a0a 2020 2020 2020 2020  rs see:.        
-0000cc90: 2020 2020 6874 7470 733a 2f2f 7863 6c69      https://xcli
-0000cca0: 6d2e 7265 6164 7468 6564 6f63 732e 696f  m.readthedocs.io
-0000ccb0: 2f65 6e2f 7374 6162 6c65 2f61 7069 2e68  /en/stable/api.h
-0000ccc0: 746d 6c23 7863 6c69 6d2e 696e 6469 6361  tml#xclim.indica
-0000ccd0: 746f 7273 2e61 746d 6f73 2e77 6172 6d5f  tors.atmos.warm_
-0000cce0: 7370 656c 6c5f 6475 7261 7469 6f6e 5f69  spell_duration_i
-0000ccf0: 6e64 6578 0a20 2020 2020 2020 2022 2222  ndex.        """
-0000cd00: 0a20 2020 2020 2020 2064 6120 3d20 5f67  .        da = _g
-0000cd10: 6574 5f64 6128 7061 7261 6d73 2c20 2274  et_da(params, "t
-0000cd20: 6173 6d61 7822 290a 2020 2020 2020 2020  asmax").        
-0000cd30: 6966 2074 6173 6d61 785f 7065 7220 6973  if tasmax_per is
-0000cd40: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-0000cd50: 2020 2074 6173 6d61 785f 7065 7220 3d20     tasmax_per = 
-0000cd60: 5f67 6574 5f70 6572 6365 6e74 696c 6528  _get_percentile(
-0000cd70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000cd80: 2064 613d 6461 2c0a 2020 2020 2020 2020   da=da,.        
-0000cd90: 2020 2020 2020 2020 7065 723d 3930 2c0a          per=90,.
-0000cda0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cdb0: 6261 7365 5f70 6572 696f 645f 7469 6d65  base_period_time
-0000cdc0: 5f72 616e 6765 3d62 6173 655f 7065 7269  _range=base_peri
-0000cdd0: 6f64 5f74 696d 655f 7261 6e67 652c 0a20  od_time_range,. 
-0000cde0: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
-0000cdf0: 2020 2020 2077 6974 6820 6461 736b 2e63       with dask.c
-0000ce00: 6f6e 6669 672e 7365 7428 2a2a 7b22 6172  onfig.set(**{"ar
-0000ce10: 7261 792e 736c 6963 696e 672e 7370 6c69  ray.slicing.spli
-0000ce20: 745f 6c61 7267 655f 6368 756e 6b73 223a  t_large_chunks":
-0000ce30: 2046 616c 7365 7d29 3a0a 2020 2020 2020   False}):.      
-0000ce40: 2020 2020 2020 7265 7475 726e 2078 632e        return xc.
-0000ce50: 6174 6d6f 732e 7761 726d 5f73 7065 6c6c  atmos.warm_spell
-0000ce60: 5f64 7572 6174 696f 6e5f 696e 6465 7828  _duration_index(
-0000ce70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000ce80: 2074 6173 6d61 785f 7065 723d 7461 736d   tasmax_per=tasm
-0000ce90: 6178 5f70 6572 2c0a 2020 2020 2020 2020  ax_per,.        
-0000cea0: 2020 2020 2020 2020 7769 6e64 6f77 3d77          window=w
-0000ceb0: 696e 646f 772c 0a20 2020 2020 2020 2020  indow,.         
-0000cec0: 2020 2020 2020 202a 2a70 6172 616d 732c         **params,
-0000ced0: 0a20 2020 2020 2020 2020 2020 2029 0a0a  .            )..
-0000cee0: 0a63 6c61 7373 2057 573a 0a20 2020 2022  .class WW:.    "
-0000cef0: 2222 4e75 6d62 6572 206f 6620 7761 726d  ""Number of warm
-0000cf00: 2061 6e64 2077 6574 2064 6179 7320 2874   and wet days (t
-0000cf10: 6173 2c20 7072 292e 2222 220a 0a20 2020  as, pr)."""..   
-0000cf20: 2074 6173 5f70 6572 203d 204e 6f6e 650a   tas_per = None.
-0000cf30: 2020 2020 7072 5f70 6572 203d 204e 6f6e      pr_per = Non
-0000cf40: 650a 2020 2020 6261 7365 5f70 6572 696f  e.    base_perio
-0000cf50: 645f 7469 6d65 5f72 616e 6765 203d 2042  d_time_range = B
-0000cf60: 4153 455f 5045 5249 4f44 0a0a 2020 2020  ASE_PERIOD..    
-0000cf70: 6465 6620 636f 6d70 7574 6528 0a20 2020  def compute(.   
-0000cf80: 2020 2020 2062 6173 655f 7065 7269 6f64       base_period
-0000cf90: 5f74 696d 655f 7261 6e67 653d 6261 7365  _time_range=base
-0000cfa0: 5f70 6572 696f 645f 7469 6d65 5f72 616e  _period_time_ran
-0000cfb0: 6765 2c0a 2020 2020 2020 2020 7461 735f  ge,.        tas_
-0000cfc0: 7065 723d 7461 735f 7065 722c 0a20 2020  per=tas_per,.   
-0000cfd0: 2020 2020 2070 725f 7065 723d 7072 5f70       pr_per=pr_p
-0000cfe0: 6572 2c0a 2020 2020 2020 2020 2a2a 7061  er,.        **pa
-0000cff0: 7261 6d73 2c0a 2020 2020 293a 0a20 2020  rams,.    ):.   
-0000d000: 2020 2020 2022 2222 4361 6c63 756c 6174       """Calculat
-0000d010: 6520 6e75 6d62 6572 206f 6620 7761 726d  e number of warm
-0000d020: 2061 6e64 2077 6574 2064 6179 732e 0a0a   and wet days...
-0000d030: 2020 2020 2020 2020 5061 7261 6d65 7465          Paramete
-0000d040: 7273 0a20 2020 2020 2020 202d 2d2d 2d2d  rs.        -----
-0000d050: 2d2d 2d2d 2d0a 2020 2020 2020 2020 7461  -----.        ta
-0000d060: 735f 7065 723a 2078 722e 4461 7461 4172  s_per: xr.DataAr
-0000d070: 7261 792c 206f 7074 696f 6e61 6c0a 2020  ray, optional.  
-0000d080: 2020 2020 2020 2020 2020 4d65 616e 2074            Mean t
-0000d090: 656d 7065 7261 7475 7265 2037 3574 6820  emperature 75th 
-0000d0a0: 7065 7263 656e 7469 6c65 2072 6566 6572  percentile refer
-0000d0b0: 656e 6365 2076 616c 7565 2061 626f 7665  ence value above
-0000d0c0: 2077 6869 6368 0a20 2020 2020 2020 2020   which.         
-0000d0d0: 2020 2061 2064 6179 2069 7320 636f 6e73     a day is cons
-0000d0e0: 6964 6572 6564 2061 7320 6120 7761 726d  idered as a warm
-0000d0f0: 2064 6179 2e0a 2020 2020 2020 2020 7072   day..        pr
-0000d100: 5f70 6572 3a20 7872 2e44 6174 6141 7272  _per: xr.DataArr
-0000d110: 6179 2c20 6f70 7469 6f6e 616c 0a20 2020  ay, optional.   
-0000d120: 2020 2020 2020 2020 2050 7265 6369 7069           Precipi
-0000d130: 7461 7469 6f6e 2037 3574 6820 7065 7263  tation 75th perc
-0000d140: 656e 7469 6c65 2072 6566 6572 656e 6365  entile reference
-0000d150: 2076 616c 7565 2061 626f 7665 2077 6869   value above whi
-0000d160: 6368 0a20 2020 2020 2020 2020 2020 2061  ch.            a
-0000d170: 2064 6179 2069 7320 636f 6e73 6964 6572   day is consider
-0000d180: 6564 2061 7320 6120 7765 7420 6461 792e  ed as a wet day.
-0000d190: 0a20 2020 2020 2020 2062 6173 655f 7065  .        base_pe
-0000d1a0: 7269 6f64 5f74 696d 655f 7261 6e67 653a  riod_time_range:
-0000d1b0: 206c 6973 740a 2020 2020 2020 2020 2020   list.          
-0000d1c0: 2020 4c69 7374 2077 6974 6820 6c65 6674    List with left
-0000d1d0: 2062 6f75 6e64 2069 7320 7374 6172 7420   bound is start 
-0000d1e0: 7965 6172 2073 7472 696e 6720 616e 6420  year string and 
-0000d1f0: 7269 6768 7420 626f 756e 640a 2020 2020  right bound.    
-0000d200: 2020 2020 2020 2020 6973 2065 6e64 2079          is end y
-0000d210: 6561 7220 7374 7269 6e67 2066 6f72 2063  ear string for c
-0000d220: 616c 6375 6c61 7469 6e67 2060 7461 735f  alculating `tas_
-0000d230: 7065 7260 2061 6e64 2f6f 7220 6070 725f  per` and/or `pr_
-0000d240: 7065 7260 2e0a 2020 2020 2020 2020 2020  per`..          
-0000d250: 2020 5468 6973 2077 696c 6c20 6265 2075    This will be u
-0000d260: 7365 6420 6f6e 6c79 2069 6620 6074 6173  sed only if `tas
-0000d270: 5f70 6572 6020 616e 642f 6f72 2060 7072  _per` and/or `pr
-0000d280: 5f70 6572 6020 6973 204e 6f6e 652e 0a0a  _per` is None...
-0000d290: 2020 2020 2020 2020 5265 7475 726e 730a          Returns.
-0000d2a0: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d0a          -------.
-0000d2b0: 2020 2020 2020 2020 7861 7272 6179 2e44          xarray.D
-0000d2c0: 6174 6141 7272 6179 3a0a 2020 2020 2020  ataArray:.      
-0000d2d0: 2020 2020 2020 4e75 6d62 6572 206f 6620        Number of 
-0000d2e0: 6461 7973 2077 6865 7265 2077 6172 6d20  days where warm 
-0000d2f0: 616e 6420 7765 7420 636f 6e64 6974 696f  and wet conditio
-0000d300: 6e73 2063 6f69 6e63 6964 652e 0a20 2020  ns coincide..   
-0000d310: 2020 2020 2020 2020 2049 6620 7465 6d70           If temp
-0000d320: 6572 6174 7572 6520 6973 2061 626f 7665  erature is above
-0000d330: 207b 7461 735f 7065 727d 2061 2064 6179   {tas_per} a day
-0000d340: 2069 7320 636f 6e73 6964 6572 6564 2061   is considered a
-0000d350: 7320 610a 2020 2020 2020 2020 2020 2020  s a.            
-0000d360: 7761 726d 2064 6179 2e0a 2020 2020 2020  warm day..      
-0000d370: 2020 2020 2020 4966 2070 7265 6369 7069        If precipi
-0000d380: 7461 7469 6f6e 2069 7320 6162 6f76 6520  tation is above 
-0000d390: 7b70 725f 7065 727d 2061 2064 6179 2069  {pr_per} a day i
-0000d3a0: 7320 636f 6e73 6964 6572 6564 2061 7320  s considered as 
-0000d3b0: 610a 2020 2020 2020 2020 2020 2020 7765  a.            we
-0000d3c0: 7420 6461 792e 0a0a 2020 2020 2020 2020  t day...        
-0000d3d0: 4e6f 7465 730a 2020 2020 2020 2020 2d2d  Notes.        --
-0000d3e0: 2d2d 2d0a 2020 2020 2020 2020 466f 7220  ---.        For 
-0000d3f0: 6d6f 7265 2069 6e66 6f72 6d61 7469 6f6e  more information
-0000d400: 206f 6e20 7468 6520 696e 7075 7420 7061   on the input pa
-0000d410: 7261 6d65 7465 7273 2073 6565 3a0a 2020  rameters see:.  
-0000d420: 2020 2020 2020 2020 2020 6874 7470 733a            https:
-0000d430: 2f2f 7863 6c69 6d2e 7265 6164 7468 6564  //xclim.readthed
-0000d440: 6f63 732e 696f 2f65 6e2f 7374 6162 6c65  ocs.io/en/stable
-0000d450: 2f61 7069 2e68 746d 6c23 7863 6c69 6d2e  /api.html#xclim.
-0000d460: 696e 6469 6361 746f 7273 2e61 746d 6f73  indicators.atmos
-0000d470: 2e77 6172 6d5f 616e 645f 7765 745f 6461  .warm_and_wet_da
-0000d480: 7973 0a20 2020 2020 2020 2022 2222 0a20  ys.        """. 
-0000d490: 2020 2020 2020 2064 615f 7461 7320 3d20         da_tas = 
-0000d4a0: 5f67 6574 5f64 6128 7061 7261 6d73 2c20  _get_da(params, 
-0000d4b0: 2274 6173 2229 0a20 2020 2020 2020 2064  "tas").        d
-0000d4c0: 615f 7072 203d 205f 6765 745f 6461 2870  a_pr = _get_da(p
-0000d4d0: 6172 616d 732c 2022 7072 2229 0a20 2020  arams, "pr").   
-0000d4e0: 2020 2020 2069 6620 7461 735f 7065 7220       if tas_per 
-0000d4f0: 6973 204e 6f6e 653a 0a20 2020 2020 2020  is None:.       
-0000d500: 2020 2020 2074 6173 5f70 6572 203d 205f       tas_per = _
-0000d510: 6765 745f 7065 7263 656e 7469 6c65 280a  get_percentile(.
-0000d520: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d530: 6461 3d64 615f 7461 732c 0a20 2020 2020  da=da_tas,.     
-0000d540: 2020 2020 2020 2020 2020 2070 6572 3d37             per=7
-0000d550: 352c 0a20 2020 2020 2020 2020 2020 2020  5,.             
-0000d560: 2020 2062 6173 655f 7065 7269 6f64 5f74     base_period_t
-0000d570: 696d 655f 7261 6e67 653d 6261 7365 5f70  ime_range=base_p
-0000d580: 6572 696f 645f 7469 6d65 5f72 616e 6765  eriod_time_range
-0000d590: 2c0a 2020 2020 2020 2020 2020 2020 290a  ,.            ).
-0000d5a0: 2020 2020 2020 2020 6966 2070 725f 7065          if pr_pe
-0000d5b0: 7220 6973 204e 6f6e 653a 0a20 2020 2020  r is None:.     
-0000d5c0: 2020 2020 2020 2064 615f 7072 5f66 203d         da_pr_f =
-0000d5d0: 205f 6669 6c74 6572 5f6f 7574 5f73 6d61   _filter_out_sma
-0000d5e0: 6c6c 5f76 616c 7565 7328 0a20 2020 2020  ll_values(.     
-0000d5f0: 2020 2020 2020 2020 2020 2064 615f 7072             da_pr
-0000d600: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0000d610: 2020 2231 206d 6d2f 6461 7922 2c0a 2020    "1 mm/day",.  
-0000d620: 2020 2020 2020 2020 2020 2020 2020 636f                co
-0000d630: 6e74 6578 743d 2268 7964 726f 222c 0a20  ntext="hydro",. 
-0000d640: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
-0000d650: 2020 2020 2020 2020 2070 725f 7065 7220           pr_per 
-0000d660: 3d20 5f67 6574 5f70 6572 6365 6e74 696c  = _get_percentil
-0000d670: 6528 0a20 2020 2020 2020 2020 2020 2020  e(.             
-0000d680: 2020 2064 613d 6461 5f70 725f 662c 0a20     da=da_pr_f,. 
-0000d690: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-0000d6a0: 6572 3d37 352c 0a20 2020 2020 2020 2020  er=75,.         
-0000d6b0: 2020 2020 2020 2062 6173 655f 7065 7269         base_peri
-0000d6c0: 6f64 5f74 696d 655f 7261 6e67 653d 6261  od_time_range=ba
-0000d6d0: 7365 5f70 6572 696f 645f 7469 6d65 5f72  se_period_time_r
-0000d6e0: 616e 6765 2c0a 2020 2020 2020 2020 2020  ange,.          
-0000d6f0: 2020 290a 2020 2020 2020 2020 7769 7468    ).        with
-0000d700: 2064 6173 6b2e 636f 6e66 6967 2e73 6574   dask.config.set
-0000d710: 282a 2a7b 2261 7272 6179 2e73 6c69 6369  (**{"array.slici
-0000d720: 6e67 2e73 706c 6974 5f6c 6172 6765 5f63  ng.split_large_c
-0000d730: 6875 6e6b 7322 3a20 4661 6c73 657d 293a  hunks": False}):
-0000d740: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-0000d750: 7572 6e20 7863 2e61 746d 6f73 2e77 6172  urn xc.atmos.war
-0000d760: 6d5f 616e 645f 7765 745f 6461 7973 280a  m_and_wet_days(.
-0000d770: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d780: 7461 735f 7065 723d 7461 735f 7065 722c  tas_per=tas_per,
-0000d790: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000d7a0: 2070 725f 7065 723d 7072 5f70 6572 2c0a   pr_per=pr_per,.
-0000d7b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d7c0: 2a2a 7061 7261 6d73 2c0a 2020 2020 2020  **params,.      
-0000d7d0: 2020 2020 2020 290a 0a0a 636c 6173 7320        )...class 
-0000d7e0: 4353 663a 0a20 2020 2022 2222 4e75 6d62  CSf:.    """Numb
-0000d7f0: 6572 206f 6620 636f 6c64 2073 7065 6c6c  er of cold spell
-0000d800: 7320 2874 6173 292e 2222 220a 0a20 2020  s (tas)."""..   
-0000d810: 2074 6872 6573 6820 3d20 2d31 300a 2020   thresh = -10.  
-0000d820: 2020 7769 6e64 6f77 203d 2033 0a0a 2020    window = 3..  
-0000d830: 2020 6465 6620 636f 6d70 7574 6528 7468    def compute(th
-0000d840: 7265 7368 3d74 6872 6573 682c 2077 696e  resh=thresh, win
-0000d850: 646f 773d 7769 6e64 6f77 2c20 2a2a 7061  dow=window, **pa
-0000d860: 7261 6d73 293a 0a20 2020 2020 2020 2022  rams):.        "
-0000d870: 2222 4361 6c63 756c 6174 6520 6e75 6d62  ""Calculate numb
-0000d880: 6572 206f 6620 636f 6c64 2073 7065 6c6c  er of cold spell
-0000d890: 732e 0a0a 2020 2020 2020 2020 5061 7261  s...        Para
-0000d8a0: 6d65 7465 7273 0a20 2020 2020 2020 202d  meters.        -
-0000d8b0: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 2020  ---------.      
-0000d8c0: 2020 7468 7265 7368 3a20 696e 7420 6f72    thresh: int or
-0000d8d0: 2073 7472 696e 670a 2020 2020 2020 2020   string.        
-0000d8e0: 2020 2020 5468 7265 7368 6f6c 6420 7465      Threshold te
-0000d8f0: 6d70 6572 6174 7572 6520 6265 6c6f 7720  mperature below 
-0000d900: 7768 6963 6820 6120 6461 7920 6973 2063  which a day is c
-0000d910: 6f6e 7369 6465 7265 640a 2020 2020 2020  onsidered.      
-0000d920: 2020 2020 2020 6173 2061 2063 6f6c 6420        as a cold 
-0000d930: 6461 7920 2864 6566 6175 6c74 3a20 2d31  day (default: -1
-0000d940: 3020 6465 6743 292e 0a20 2020 2020 2020  0 degC)..       
-0000d950: 2020 2020 2049 6620 7479 7065 206f 6620       If type of 
-0000d960: 7468 7265 7368 6f6c 6420 6973 2061 6e20  threshold is an 
-0000d970: 696e 7465 6765 7220 7468 6520 756e 6974  integer the unit
-0000d980: 2069 7320 7365 7420 746f 2064 6567 432e   is set to degC.
-0000d990: 0a20 2020 2020 2020 2077 696e 646f 773a  .        window:
-0000d9a0: 2069 6e74 0a20 2020 2020 2020 2020 2020   int.           
-0000d9b0: 204d 696e 696d 756d 206e 756d 6265 7220   Minimum number 
-0000d9c0: 6f66 2064 6179 7320 7769 7468 2074 656d  of days with tem
-0000d9d0: 7065 7261 7475 7265 2062 656c 6f77 2074  perature below t
-0000d9e0: 6872 6573 680a 2020 2020 2020 2020 2020  hresh.          
-0000d9f0: 2020 746f 2071 7561 6c69 6679 2061 7320    to qualify as 
-0000da00: 6120 636f 6c64 2073 7065 6c6c 2028 6465  a cold spell (de
-0000da10: 6661 756c 743a 2033 292e 0a0a 2020 2020  fault: 3)...    
-0000da20: 2020 2020 5265 7475 726e 730a 2020 2020      Returns.    
-0000da30: 2020 2020 2d2d 2d2d 2d2d 2d0a 2020 2020      -------.    
-0000da40: 2020 2020 7861 7272 6179 2e44 6174 6141      xarray.DataA
-0000da50: 7272 6179 0a20 2020 2020 2020 2020 2020  rray.           
-0000da60: 204e 756d 6265 7220 6f66 2063 6f6c 6420   Number of cold 
-0000da70: 7370 656c 6c73 206f 6620 6174 206c 6561  spells of at lea
-0000da80: 7374 207b 7769 6e64 6f77 7d20 636f 6e73  st {window} cons
-0000da90: 6563 7574 6976 6520 6461 7973 0a20 2020  ecutive days.   
-0000daa0: 2020 2020 2020 2020 2077 6974 6820 7465           with te
-0000dab0: 6d70 6572 6174 7572 6520 6265 6c6f 7720  mperature below 
-0000dac0: 7b74 6872 6573 687d 2e0a 0a20 2020 2020  {thresh}...     
-0000dad0: 2020 204e 6f74 6573 0a20 2020 2020 2020     Notes.       
-0000dae0: 202d 2d2d 2d2d 0a20 2020 2020 2020 2046   -----.        F
-0000daf0: 6f72 206d 6f72 6520 696e 666f 726d 6174  or more informat
-0000db00: 696f 6e20 6f6e 2074 6865 2069 6e70 7574  ion on the input
-0000db10: 2070 6172 616d 6574 6572 7320 7365 653a   parameters see:
-0000db20: 0a20 2020 2020 2020 2020 2020 2068 7474  .            htt
-0000db30: 7073 3a2f 2f78 636c 696d 2e72 6561 6474  ps://xclim.readt
-0000db40: 6865 646f 6373 2e69 6f2f 656e 2f73 7461  hedocs.io/en/sta
-0000db50: 626c 652f 6170 692e 6874 6d6c 2378 636c  ble/api.html#xcl
-0000db60: 696d 2e69 6e64 6963 6174 6f72 732e 6174  im.indicators.at
-0000db70: 6d6f 732e 636f 6c64 5f73 7065 6c6c 5f66  mos.cold_spell_f
-0000db80: 7265 7175 656e 6379 0a20 2020 2020 2020  requency.       
-0000db90: 2022 2222 0a20 2020 2020 2020 2074 6872   """.        thr
-0000dba0: 6573 6820 3d20 5f74 6872 6573 685f 7374  esh = _thresh_st
-0000dbb0: 7269 6e67 2874 6872 6573 682c 2022 6465  ring(thresh, "de
-0000dbc0: 6743 2229 0a20 2020 2020 2020 2072 6574  gC").        ret
-0000dbd0: 7572 6e20 7863 2e61 746d 6f73 2e63 6f6c  urn xc.atmos.col
-0000dbe0: 645f 7370 656c 6c5f 6672 6571 7565 6e63  d_spell_frequenc
-0000dbf0: 7928 0a20 2020 2020 2020 2020 2020 2074  y(.            t
-0000dc00: 6872 6573 683d 7468 7265 7368 2c0a 2020  hresh=thresh,.  
-0000dc10: 2020 2020 2020 2020 2020 7769 6e64 6f77            window
-0000dc20: 3d77 696e 646f 772c 0a20 2020 2020 2020  =window,.       
-0000dc30: 2020 2020 202a 2a70 6172 616d 732c 0a20       **params,. 
-0000dc40: 2020 2020 2020 2029 0a0a 0a63 6c61 7373         )...class
-0000dc50: 2048 5366 3a0a 2020 2020 2222 224e 756d   HSf:.    """Num
-0000dc60: 6265 7220 6f66 2068 6f74 2073 7065 6c6c  ber of hot spell
-0000dc70: 7320 2874 6173 6d61 7829 2e22 2222 0a0a  s (tasmax)."""..
-0000dc80: 2020 2020 7468 7265 7368 203d 2033 350a      thresh = 35.
-0000dc90: 2020 2020 7769 6e64 6f77 203d 2033 0a0a      window = 3..
-0000dca0: 2020 2020 6465 6620 636f 6d70 7574 6528      def compute(
-0000dcb0: 7468 7265 7368 3d74 6872 6573 682c 2077  thresh=thresh, w
-0000dcc0: 696e 646f 773d 7769 6e64 6f77 2c20 2a2a  indow=window, **
-0000dcd0: 7061 7261 6d73 293a 0a20 2020 2020 2020  params):.       
-0000dce0: 2022 2222 4361 6c63 756c 6174 6520 6e75   """Calculate nu
-0000dcf0: 6d62 6572 206f 6620 686f 7420 7370 656c  mber of hot spel
-0000dd00: 6c73 2e0a 0a20 2020 2020 2020 2050 6172  ls...        Par
-0000dd10: 616d 6574 6572 730a 2020 2020 2020 2020  ameters.        
-0000dd20: 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020  ----------.     
-0000dd30: 2020 2074 6872 6573 683a 2069 6e74 206f     thresh: int o
-0000dd40: 7220 7374 7269 6e67 0a20 2020 2020 2020  r string.       
-0000dd50: 2020 2020 2054 6872 6573 686f 6c64 206d       Threshold m
-0000dd60: 6178 696d 756d 2074 656d 7065 7261 7475  aximum temperatu
-0000dd70: 7265 2061 626f 7665 2077 6869 6368 2061  re above which a
-0000dd80: 2064 6179 2069 7320 636f 6e73 6964 6572   day is consider
-0000dd90: 6564 0a20 2020 2020 2020 2020 2020 2061  ed.            a
-0000dda0: 7320 6120 686f 7420 6461 7920 2864 6566  s a hot day (def
-0000ddb0: 6175 6c74 3a20 3335 2064 6567 4329 2e0a  ault: 35 degC)..
-0000ddc0: 2020 2020 2020 2020 2020 2020 4966 2074              If t
-0000ddd0: 7970 6520 6f66 2074 6872 6573 686f 6c64  ype of threshold
-0000dde0: 2069 7320 616e 2069 6e74 6567 6572 2074   is an integer t
-0000ddf0: 6865 2075 6e69 7420 6973 2073 6574 2074  he unit is set t
-0000de00: 6f20 6465 6743 2e0a 2020 2020 2020 2020  o degC..        
-0000de10: 7769 6e64 6f77 3a20 696e 740a 2020 2020  window: int.    
-0000de20: 2020 2020 2020 2020 4d69 6e69 6d75 6d20          Minimum 
-0000de30: 6e75 6d62 6572 206f 6620 6461 7973 2077  number of days w
-0000de40: 6974 6820 7465 6d70 6572 6174 7572 6520  ith temperature 
-0000de50: 6162 6f76 6520 7468 7265 7368 0a20 2020  above thresh.   
-0000de60: 2020 2020 2020 2020 2074 6f20 7175 616c           to qual
-0000de70: 6966 7920 6173 2061 2068 6f74 2073 7065  ify as a hot spe
-0000de80: 6c6c 2028 6465 6661 756c 743a 2033 292e  ll (default: 3).
-0000de90: 0a0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
-0000dea0: 730a 2020 2020 2020 2020 2d2d 2d2d 2d2d  s.        ------
-0000deb0: 2d0a 2020 2020 2020 2020 7861 7272 6179  -.        xarray
-0000dec0: 2e44 6174 6141 7272 6179 0a20 2020 2020  .DataArray.     
-0000ded0: 2020 2020 2020 204e 756d 6265 7220 6f66         Number of
-0000dee0: 2068 6f74 2073 7065 6c6c 7320 6f66 2061   hot spells of a
-0000def0: 7420 6c65 6173 7420 7b77 696e 646f 777d  t least {window}
-0000df00: 2063 6f6e 7365 6375 7469 7665 2064 6179   consecutive day
-0000df10: 730a 2020 2020 2020 2020 2020 2020 7769  s.            wi
-0000df20: 7468 206d 6178 696d 756d 2074 656d 7065  th maximum tempe
-0000df30: 7261 7475 7265 2061 626f 7665 207b 7468  rature above {th
-0000df40: 7265 7368 7d2e 0a0a 2020 2020 2020 2020  resh}...        
-0000df50: 4e6f 7465 730a 2020 2020 2020 2020 2d2d  Notes.        --
-0000df60: 2d2d 2d0a 2020 2020 2020 2020 466f 7220  ---.        For 
-0000df70: 6d6f 7265 2069 6e66 6f72 6d61 7469 6f6e  more information
-0000df80: 206f 6e20 7468 6520 696e 7075 7420 7061   on the input pa
-0000df90: 7261 6d65 7465 7273 2073 6565 3a0a 2020  rameters see:.  
-0000dfa0: 2020 2020 2020 2020 2020 6874 7470 733a            https:
-0000dfb0: 2f2f 7863 6c69 6d2e 7265 6164 7468 6564  //xclim.readthed
-0000dfc0: 6f63 732e 696f 2f65 6e2f 7374 6162 6c65  ocs.io/en/stable
-0000dfd0: 2f61 7069 2e68 746d 6c23 7863 6c69 6d2e  /api.html#xclim.
-0000dfe0: 696e 6469 6361 746f 7273 2e61 746d 6f73  indicators.atmos
-0000dff0: 2e68 6f74 5f73 7065 6c6c 5f66 7265 7175  .hot_spell_frequ
-0000e000: 656e 6379 0a20 2020 2020 2020 2022 2222  ency.        """
-0000e010: 0a20 2020 2020 2020 2074 6872 6573 6820  .        thresh 
-0000e020: 3d20 5f74 6872 6573 685f 7374 7269 6e67  = _thresh_string
-0000e030: 2874 6872 6573 682c 2022 6465 6743 2229  (thresh, "degC")
-0000e040: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-0000e050: 7863 2e61 746d 6f73 2e68 6f74 5f73 7065  xc.atmos.hot_spe
-0000e060: 6c6c 5f66 7265 7175 656e 6379 280a 2020  ll_frequency(.  
-0000e070: 2020 2020 2020 2020 2020 7468 7265 7368            thresh
-0000e080: 3d74 6872 6573 682c 0a20 2020 2020 2020  =thresh,.       
-0000e090: 2020 2020 2077 696e 646f 773d 7769 6e64       window=wind
-0000e0a0: 6f77 2c0a 2020 2020 2020 2020 2020 2020  ow,.            
-0000e0b0: 2a2a 7061 7261 6d73 2c0a 2020 2020 2020  **params,.      
-0000e0c0: 2020 290a 0a0a 636c 6173 7320 4853 783a    )...class HSx:
-0000e0d0: 0a20 2020 2022 2222 4d61 7869 6d75 6d20  .    """Maximum 
-0000e0e0: 6c65 6e67 6874 206f 6620 686f 7420 7370  lenght of hot sp
-0000e0f0: 656c 6c73 2028 7461 736d 6178 292e 2222  ells (tasmax).""
-0000e100: 220a 0a20 2020 2074 6872 6573 6820 3d20  "..    thresh = 
-0000e110: 3335 0a20 2020 2077 696e 646f 7720 3d20  35.    window = 
-0000e120: 310a 0a20 2020 2064 6566 2063 6f6d 7075  1..    def compu
-0000e130: 7465 2874 6872 6573 683d 7468 7265 7368  te(thresh=thresh
-0000e140: 2c20 7769 6e64 6f77 3d77 696e 646f 772c  , window=window,
-0000e150: 202a 2a70 6172 616d 7329 3a0a 2020 2020   **params):.    
-0000e160: 2020 2020 2222 2243 616c 6375 6c61 7465      """Calculate
-0000e170: 206d 6178 696d 756d 206c 656e 6768 7420   maximum lenght 
-0000e180: 6f66 2068 6f74 2073 7065 6c6c 732e 0a0a  of hot spells...
-0000e190: 2020 2020 2020 2020 5061 7261 6d65 7465          Paramete
-0000e1a0: 7273 0a20 2020 2020 2020 202d 2d2d 2d2d  rs.        -----
-0000e1b0: 2d2d 2d2d 2d0a 2020 2020 2020 2020 7468  -----.        th
-0000e1c0: 7265 7368 3a20 696e 7420 6f72 2073 7472  resh: int or str
-0000e1d0: 696e 670a 2020 2020 2020 2020 2020 2020  ing.            
-0000e1e0: 5468 7265 7368 6f6c 6420 6d61 7869 6d75  Threshold maximu
-0000e1f0: 6d20 7465 6d70 6572 6174 7572 6520 6162  m temperature ab
-0000e200: 6f76 6520 7768 6963 6820 6120 6461 7920  ove which a day 
-0000e210: 6973 2063 6f6e 7369 6465 7265 640a 2020  is considered.  
-0000e220: 2020 2020 2020 2020 2020 6173 2061 2068            as a h
-0000e230: 6f74 2064 6179 2028 6465 6661 756c 743a  ot day (default:
-0000e240: 2033 3520 6465 6743 292e 0a20 2020 2020   35 degC)..     
-0000e250: 2020 2020 2020 2049 6620 7479 7065 206f         If type o
-0000e260: 6620 7468 7265 7368 6f6c 6420 6973 2061  f threshold is a
-0000e270: 6e20 696e 7465 6765 7220 7468 6520 756e  n integer the un
-0000e280: 6974 2069 7320 7365 7420 746f 2064 6567  it is set to deg
-0000e290: 432e 0a20 2020 2020 2020 2077 696e 646f  C..        windo
-0000e2a0: 773a 2069 6e74 0a20 2020 2020 2020 2020  w: int.         
-0000e2b0: 2020 204d 696e 696d 756d 206e 756d 6265     Minimum numbe
-0000e2c0: 7220 6f66 2064 6179 7320 7769 7468 2074  r of days with t
-0000e2d0: 656d 7065 7261 7475 7265 2061 626f 7665  emperature above
-0000e2e0: 2074 6872 6573 680a 2020 2020 2020 2020   thresh.        
-0000e2f0: 2020 2020 746f 2071 7561 6c69 6679 2061      to qualify a
-0000e300: 7320 6120 686f 7420 7370 656c 6c20 2864  s a hot spell (d
-0000e310: 6566 6175 6c74 3a20 3129 2e0a 0a20 2020  efault: 1)...   
-0000e320: 2020 2020 2052 6574 7572 6e73 0a20 2020       Returns.   
-0000e330: 2020 2020 202d 2d2d 2d2d 2d2d 0a20 2020       -------.   
-0000e340: 2020 2020 2078 6172 7261 792e 4461 7461       xarray.Data
-0000e350: 4172 7261 790a 2020 2020 2020 2020 2020  Array.          
-0000e360: 2020 4d61 7869 6d75 6d20 6c65 6e67 7468    Maximum length
-0000e370: 206f 6620 686f 7420 7370 656c 6c73 206f   of hot spells o
-0000e380: 6620 6174 206c 6561 7374 207b 7769 6e64  f at least {wind
-0000e390: 6f77 7d20 636f 6e73 6563 7574 6976 6520  ow} consecutive 
-0000e3a0: 6461 7973 0a20 2020 2020 2020 2020 2020  days.           
-0000e3b0: 2077 6974 6820 6d61 7869 6d75 6d20 7465   with maximum te
-0000e3c0: 6d70 6572 6174 7572 6520 6162 6f76 6520  mperature above 
-0000e3d0: 7b74 6872 6573 687d 2e0a 0a20 2020 2020  {thresh}...     
-0000e3e0: 2020 204e 6f74 6573 0a20 2020 2020 2020     Notes.       
-0000e3f0: 202d 2d2d 2d2d 0a20 2020 2020 2020 2046   -----.        F
-0000e400: 6f72 206d 6f72 6520 696e 666f 726d 6174  or more informat
-0000e410: 696f 6e20 6f6e 2074 6865 2069 6e70 7574  ion on the input
-0000e420: 2070 6172 616d 6574 6572 7320 7365 653a   parameters see:
-0000e430: 0a20 2020 2020 2020 2020 2020 2068 7474  .            htt
-0000e440: 7073 3a2f 2f78 636c 696d 2e72 6561 6474  ps://xclim.readt
-0000e450: 6865 646f 6373 2e69 6f2f 656e 2f73 7461  hedocs.io/en/sta
-0000e460: 626c 652f 6170 692e 6874 6d6c 2378 636c  ble/api.html#xcl
-0000e470: 696d 2e69 6e64 6963 6174 6f72 732e 6174  im.indicators.at
-0000e480: 6d6f 732e 686f 745f 7370 656c 6c5f 6d61  mos.hot_spell_ma
-0000e490: 785f 6c65 6e67 7468 0a20 2020 2020 2020  x_length.       
-0000e4a0: 2022 2222 0a20 2020 2020 2020 2074 6872   """.        thr
-0000e4b0: 6573 6820 3d20 5f74 6872 6573 685f 7374  esh = _thresh_st
-0000e4c0: 7269 6e67 2874 6872 6573 682c 2022 6465  ring(thresh, "de
-0000e4d0: 6743 2229 0a20 2020 2020 2020 2072 6574  gC").        ret
-0000e4e0: 7572 6e20 7863 2e61 746d 6f73 2e68 6f74  urn xc.atmos.hot
-0000e4f0: 5f73 7065 6c6c 5f6d 6178 5f6c 656e 6774  _spell_max_lengt
-0000e500: 6828 0a20 2020 2020 2020 2020 2020 2074  h(.            t
-0000e510: 6872 6573 683d 7468 7265 7368 2c0a 2020  hresh=thresh,.  
-0000e520: 2020 2020 2020 2020 2020 7769 6e64 6f77            window
-0000e530: 3d77 696e 646f 772c 0a20 2020 2020 2020  =window,.       
-0000e540: 2020 2020 202a 2a70 6172 616d 732c 0a20       **params,. 
-0000e550: 2020 2020 2020 2029 0a0a 0a63 6c61 7373         )...class
-0000e560: 2053 443a 0a20 2020 2022 2222 4e75 6d62   SD:.    """Numb
-0000e570: 6572 206f 6620 736e 6f77 2064 6179 732e  er of snow days.
-0000e580: 2222 220a 0a20 2020 2074 6872 6573 6820  """..    thresh 
-0000e590: 3d20 310a 0a20 2020 2064 6566 2063 6f6d  = 1..    def com
-0000e5a0: 7075 7465 2874 6872 6573 683d 7468 7265  pute(thresh=thre
-0000e5b0: 7368 2c20 2a2a 7061 7261 6d73 293a 0a20  sh, **params):. 
-0000e5c0: 2020 2020 2020 2022 2222 4361 6c63 756c         """Calcul
-0000e5d0: 6174 6520 6e75 6d62 6572 206f 6620 736e  ate number of sn
-0000e5e0: 6f77 2064 6179 732e 0a0a 2020 2020 2020  ow days...      
-0000e5f0: 2020 5061 7261 6d65 7465 7273 0a20 2020    Parameters.   
-0000e600: 2020 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a       ----------.
-0000e610: 2020 2020 2020 2020 7468 7265 7368 3a20          thresh: 
-0000e620: 696e 7420 6f72 2073 7472 696e 670a 2020  int or string.  
-0000e630: 2020 2020 2020 2020 2020 4c69 7175 6964            Liquid
-0000e640: 2077 6174 6572 2065 7175 6976 616c 656e   water equivalen
-0000e650: 7420 736e 6f77 6661 6c6c 2072 6174 6520  t snowfall rate 
-0000e660: 6162 6f76 6520 7768 6963 6820 6120 6461  above which a da
-0000e670: 7920 6973 0a20 2020 2020 2020 2020 2020  y is.           
-0000e680: 2063 6f6e 7369 6465 7265 6420 6173 2061   considered as a
-0000e690: 2073 6e6f 7720 6461 7920 2864 6566 6175   snow day (defau
-0000e6a0: 6c74 3a20 3120 6d6d 2f64 6179 2920 2e0a  lt: 1 mm/day) ..
-0000e6b0: 2020 2020 2020 2020 2020 2020 4966 2074              If t
-0000e6c0: 7970 6520 6f66 2074 6872 6573 686f 6c64  ype of threshold
-0000e6d0: 2069 7320 616e 2069 6e74 6567 6572 2074   is an integer t
-0000e6e0: 6865 2075 6e69 7420 6973 2073 6574 2074  he unit is set t
-0000e6f0: 6f20 6d6d 2f64 6179 2e0a 0a20 2020 2020  o mm/day...     
-0000e700: 2020 2052 6574 7572 6e73 0a20 2020 2020     Returns.     
-0000e710: 2020 202d 2d2d 2d2d 2d2d 0a20 2020 2020     -------.     
-0000e720: 2020 2078 6172 7261 792e 4461 7461 4172     xarray.DataAr
-0000e730: 7261 790a 2020 2020 2020 2020 2020 2020  ray.            
-0000e740: 4e75 6d62 6572 206f 6620 6461 7973 2077  Number of days w
-0000e750: 6974 6820 736f 6c69 6420 7072 6563 6970  ith solid precip
-0000e760: 6974 6174 696f 6e20 666c 7578 0a20 2020  itation flux.   
-0000e770: 2020 2020 2020 2020 2061 626f 7665 207b           above {
-0000e780: 7468 7265 7368 7d20 7468 7265 7368 6f6c  thresh} threshol
-0000e790: 642e 0a0a 2020 2020 2020 2020 4e6f 7465  d...        Note
-0000e7a0: 730a 2020 2020 2020 2020 2d2d 2d2d 2d0a  s.        -----.
-0000e7b0: 2020 2020 2020 2020 466f 7220 6d6f 7265          For more
-0000e7c0: 2069 6e66 6f72 6d61 7469 6f6e 206f 6e20   information on 
-0000e7d0: 7468 6520 696e 7075 7420 7061 7261 6d65  the input parame
-0000e7e0: 7465 7273 2073 6565 3a0a 2020 2020 2020  ters see:.      
-0000e7f0: 2020 2020 2020 6874 7470 733a 2f2f 7863        https://xc
-0000e800: 6c69 6d2e 7265 6164 7468 6564 6f63 732e  lim.readthedocs.
-0000e810: 696f 2f65 6e2f 7374 6162 6c65 2f61 7069  io/en/stable/api
-0000e820: 2e68 746d 6c23 7863 6c69 6d2e 696e 6469  .html#xclim.indi
-0000e830: 6361 746f 7273 2e61 746d 6f73 2e64 6179  cators.atmos.day
-0000e840: 735f 7769 7468 5f73 6e6f 770a 2020 2020  s_with_snow.    
-0000e850: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-0000e860: 7468 7265 7368 203d 205f 7468 7265 7368  thresh = _thresh
-0000e870: 5f73 7472 696e 6728 7468 7265 7368 2c20  _string(thresh, 
-0000e880: 226d 6d2f 6461 7922 290a 2020 2020 2020  "mm/day").      
-0000e890: 2020 7265 7475 726e 2078 632e 6174 6d6f    return xc.atmo
-0000e8a0: 732e 6461 7973 5f77 6974 685f 736e 6f77  s.days_with_snow
-0000e8b0: 280a 2020 2020 2020 2020 2020 2020 6c6f  (.            lo
-0000e8c0: 773d 7468 7265 7368 2c0a 2020 2020 2020  w=thresh,.      
-0000e8d0: 2020 2020 2020 2a2a 7061 7261 6d73 2c0a        **params,.
-0000e8e0: 2020 2020 2020 2020 290a 0a0a 636c 6173          )...clas
-0000e8f0: 7320 5343 443a 0a20 2020 2022 2222 536e  s SCD:.    """Sn
-0000e900: 6f77 2063 6f76 6572 2064 7572 6174 696f  ow cover duratio
-0000e910: 6e2e 2222 220a 0a20 2020 2074 6872 6573  n."""..    thres
-0000e920: 6820 3d20 310a 2020 2020 7761 7465 725f  h = 1.    water_
-0000e930: 6571 7569 7661 6c65 6e74 203d 2046 616c  equivalent = Fal
-0000e940: 7365 0a0a 2020 2020 6465 6620 636f 6d70  se..    def comp
-0000e950: 7574 6528 7468 7265 7368 3d74 6872 6573  ute(thresh=thres
-0000e960: 682c 2077 6174 6572 5f65 7175 6976 616c  h, water_equival
-0000e970: 656e 743d 7761 7465 725f 6571 7569 7661  ent=water_equiva
-0000e980: 6c65 6e74 2c20 2a2a 7061 7261 6d73 293a  lent, **params):
-0000e990: 0a20 2020 2020 2020 2022 2222 4361 6c63  .        """Calc
-0000e9a0: 756c 6174 6520 736e 6f77 2063 6f76 6572  ulate snow cover
-0000e9b0: 2064 7572 6174 696f 6e2e 0a0a 2020 2020   duration...    
-0000e9c0: 2020 2020 5061 7261 6d65 7465 7273 0a20      Parameters. 
-0000e9d0: 2020 2020 2020 202d 2d2d 2d2d 2d2d 2d2d         ---------
-0000e9e0: 2d0a 2020 2020 2020 2020 7468 7265 7368  -.        thresh
-0000e9f0: 3a20 696e 7420 6f72 2073 7472 696e 670a  : int or string.
-0000ea00: 2020 2020 2020 2020 2020 2020 5468 7265              Thre
-0000ea10: 7368 6f6c 6420 736e 6f77 2074 6869 636b  shold snow thick
-0000ea20: 6e65 7373 2061 626f 7665 2077 6869 6368  ness above which
-0000ea30: 2061 2064 6179 2069 7320 636f 6e73 6964   a day is consid
-0000ea40: 6572 6564 0a20 2020 2020 2020 2020 2020  ered.           
-0000ea50: 2061 7320 6120 736e 6f77 2064 6179 2028   as a snow day (
-0000ea60: 6465 6661 756c 743a 2031 2063 6d29 2e0a  default: 1 cm)..
-0000ea70: 2020 2020 2020 2020 2020 2020 4966 2074              If t
-0000ea80: 7970 6520 6f66 2074 6872 6573 686f 6c64  ype of threshold
-0000ea90: 2069 7320 616e 2069 6e74 6567 6572 2074   is an integer t
-0000eaa0: 6865 2075 6e69 7420 6973 2073 6574 2074  he unit is set t
-0000eab0: 6f20 636d 2e0a 0a20 2020 2020 2020 2052  o cm...        R
-0000eac0: 6574 7572 6e73 0a20 2020 2020 2020 202d  eturns.        -
-0000ead0: 2d2d 2d2d 2d2d 0a20 2020 2020 2020 2078  ------.        x
-0000eae0: 6172 7261 792e 4461 7461 4172 7261 790a  array.DataArray.
-0000eaf0: 2020 2020 2020 2020 2020 2020 4e75 6d62              Numb
-0000eb00: 6572 206f 6620 6461 7973 2077 6974 6820  er of days with 
-0000eb10: 736e 6f77 2063 6f76 6572 2061 626f 7665  snow cover above
-0000eb20: 207b 7468 7265 7368 7d20 7468 7265 7368   {thresh} thresh
-0000eb30: 6f6c 642e 0a0a 2020 2020 2020 2020 4e6f  old...        No
-0000eb40: 7465 730a 2020 2020 2020 2020 2d2d 2d2d  tes.        ----
-0000eb50: 2d0a 2020 2020 2020 2020 466f 7220 6d6f  -.        For mo
-0000eb60: 7265 2069 6e66 6f72 6d61 7469 6f6e 206f  re information o
-0000eb70: 6e20 7468 6520 696e 7075 7420 7061 7261  n the input para
-0000eb80: 6d65 7465 7273 2073 6565 3a0a 2020 2020  meters see:.    
-0000eb90: 2020 2020 2020 2020 6874 7470 733a 2f2f          https://
-0000eba0: 7863 6c69 6d2e 7265 6164 7468 6564 6f63  xclim.readthedoc
-0000ebb0: 732e 696f 2f65 6e2f 7374 6162 6c65 2f61  s.io/en/stable/a
-0000ebc0: 7069 2e68 746d 6c23 7863 6c69 6d2e 696e  pi.html#xclim.in
-0000ebd0: 6469 6361 746f 7273 2e6c 616e 642e 736e  dicators.land.sn
-0000ebe0: 6f77 5f63 6f76 6572 5f64 7572 6174 696f  ow_cover_duratio
-0000ebf0: 6e0a 2020 2020 2020 2020 2222 220a 2020  n.        """.  
-0000ec00: 2020 2020 2020 6966 2077 6174 6572 5f65        if water_e
-0000ec10: 7175 6976 616c 656e 7420 6973 2054 7275  quivalent is Tru
-0000ec20: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
-0000ec30: 6e77 203d 2078 632e 6c61 6e64 2e73 6e64  nw = xc.land.snd
-0000ec40: 5f74 6f5f 736e 7728 6473 3d70 6172 616d  _to_snw(ds=param
-0000ec50: 735b 2264 7322 5d29 0a20 2020 2020 2020  s["ds"]).       
-0000ec60: 2020 2020 2073 6e64 203d 2063 6f6e 7665       snd = conve
-0000ec70: 7274 5f75 6e69 7473 5f74 6f28 736e 772c  rt_units_to(snw,
-0000ec80: 2022 6d6d 222c 2063 6f6e 7465 7874 3d22   "mm", context="
-0000ec90: 6879 6472 6f22 290a 2020 2020 2020 2020  hydro").        
-0000eca0: 2020 2020 736e 642e 6174 7472 7320 3d20      snd.attrs = 
-0000ecb0: 7061 7261 6d73 5b22 6473 225d 5b22 736e  params["ds"]["sn
-0000ecc0: 6422 5d2e 6174 7472 730a 2020 2020 2020  d"].attrs.      
-0000ecd0: 2020 2020 2020 7061 7261 6d73 5b22 6473        params["ds
-0000ece0: 225d 5b22 736e 6422 5d20 3d20 736e 640a  "]["snd"] = snd.
-0000ecf0: 2020 2020 2020 2020 7468 7265 7368 203d          thresh =
-0000ed00: 205f 7468 7265 7368 5f73 7472 696e 6728   _thresh_string(
-0000ed10: 7468 7265 7368 2c20 2263 6d22 290a 2020  thresh, "cm").  
-0000ed20: 2020 2020 2020 7265 7475 726e 2078 632e        return xc.
-0000ed30: 6c61 6e64 2e73 6e64 5f73 6561 736f 6e5f  land.snd_season_
-0000ed40: 6c65 6e67 7468 280a 2020 2020 2020 2020  length(.        
-0000ed50: 2020 2020 7468 7265 7368 3d74 6872 6573      thresh=thres
-0000ed60: 682c 0a20 2020 2020 2020 2020 2020 202a  h,.            *
-0000ed70: 2a70 6172 616d 732c 0a20 2020 2020 2020  *params,.       
-0000ed80: 2029 0a0a 0a63 6c61 7373 2053 696e 743a   )...class Sint:
-0000ed90: 0a20 2020 2022 2222 536e 6f77 6661 6c6c  .    """Snowfall
-0000eda0: 2069 6e74 656e 7369 7479 2e22 2222 0a0a   intensity."""..
-0000edb0: 2020 2020 7468 7265 7368 203d 2031 0a0a      thresh = 1..
-0000edc0: 2020 2020 6465 6620 636f 6d70 7574 6528      def compute(
-0000edd0: 7468 7265 7368 3d74 6872 6573 682c 202a  thresh=thresh, *
-0000ede0: 2a70 6172 616d 7329 3a0a 2020 2020 2020  *params):.      
-0000edf0: 2020 2222 2243 616c 6375 6c61 7465 2073    """Calculate s
-0000ee00: 6e6f 7766 616c 6c20 696e 7465 6e73 6974  nowfall intensit
-0000ee10: 792e 0a0a 2020 2020 2020 2020 5061 7261  y...        Para
-0000ee20: 6d65 7465 7273 0a20 2020 2020 2020 202d  meters.        -
-0000ee30: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 2020  ---------.      
-0000ee40: 2020 7468 7265 7368 3a20 696e 7420 6f72    thresh: int or
-0000ee50: 2073 7472 696e 670a 2020 2020 2020 2020   string.        
-0000ee60: 2020 2020 4c69 7175 6964 2077 6174 6572      Liquid water
-0000ee70: 2065 7175 6976 616c 656e 7420 736e 6f77   equivalent snow
-0000ee80: 6661 6c6c 2072 6174 6520 6162 6f76 6520  fall rate above 
-0000ee90: 7768 6963 6820 6120 6461 7920 6973 0a20  which a day is. 
-0000eea0: 2020 2020 2020 2020 2020 2063 6f6e 7369             consi
-0000eeb0: 6465 7265 6420 6173 2061 2073 6e6f 7720  dered as a snow 
-0000eec0: 6461 7920 2864 6566 6175 6c74 3a20 3120  day (default: 1 
-0000eed0: 6d6d 2f64 6179 2920 2e0a 2020 2020 2020  mm/day) ..      
-0000eee0: 2020 2020 2020 4966 2074 7970 6520 6f66        If type of
-0000eef0: 2074 6872 6573 686f 6c64 2069 7320 616e   threshold is an
-0000ef00: 2069 6e74 6567 6572 2074 6865 2075 6e69   integer the uni
-0000ef10: 7420 6973 2073 6574 2074 6f20 6d6d 2f64  t is set to mm/d
-0000ef20: 6179 2e0a 0a20 2020 2020 2020 2052 6574  ay...        Ret
-0000ef30: 7572 6e73 0a20 2020 2020 2020 202d 2d2d  urns.        ---
-0000ef40: 2d2d 2d2d 0a20 2020 2020 2020 2078 6172  ----.        xar
-0000ef50: 7261 792e 4461 7461 4172 7261 790a 2020  ray.DataArray.  
-0000ef60: 2020 2020 2020 2020 2020 4d65 616e 2064            Mean d
-0000ef70: 6169 6c79 2073 6e6f 7766 616c 6c20 6475  aily snowfall du
-0000ef80: 7269 6e67 2064 6179 7320 7769 7468 2073  ring days with s
-0000ef90: 6e6f 7766 616c 6c20 3e20 7b74 6872 6573  nowfall > {thres
-0000efa0: 687d 2e0a 0a20 2020 2020 2020 204e 6f74  h}...        Not
-0000efb0: 6573 0a20 2020 2020 2020 202d 2d2d 2d2d  es.        -----
-0000efc0: 0a20 2020 2020 2020 2046 6f72 206d 6f72  .        For mor
-0000efd0: 6520 696e 666f 726d 6174 696f 6e20 6f6e  e information on
-0000efe0: 2074 6865 2069 6e70 7574 2070 6172 616d   the input param
-0000eff0: 6574 6572 7320 7365 653a 0a20 2020 2020  eters see:.     
-0000f000: 2020 2020 2020 2068 7474 7073 3a2f 2f78         https://x
-0000f010: 636c 696d 2e72 6561 6474 6865 646f 6373  clim.readthedocs
-0000f020: 2e69 6f2f 656e 2f73 7461 626c 652f 6170  .io/en/stable/ap
-0000f030: 692e 6874 6d6c 2378 636c 696d 2e69 6e64  i.html#xclim.ind
-0000f040: 6963 6174 6f72 732e 6174 6d6f 732e 736e  icators.atmos.sn
-0000f050: 6f77 6661 6c6c 5f69 6e74 656e 7369 7479  owfall_intensity
-0000f060: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-0000f070: 2020 2020 2074 6872 6573 6820 3d20 5f74       thresh = _t
-0000f080: 6872 6573 685f 7374 7269 6e67 2874 6872  hresh_string(thr
-0000f090: 6573 682c 2022 6d6d 2f64 6179 2229 0a20  esh, "mm/day"). 
-0000f0a0: 2020 2020 2020 2072 6574 7572 6e20 7863         return xc
-0000f0b0: 2e61 746d 6f73 2e73 6e6f 7766 616c 6c5f  .atmos.snowfall_
-0000f0c0: 696e 7465 6e73 6974 7928 0a20 2020 2020  intensity(.     
-0000f0d0: 2020 2020 2020 2074 6872 6573 683d 7468         thresh=th
-0000f0e0: 7265 7368 2c0a 2020 2020 2020 2020 2020  resh,.          
-0000f0f0: 2020 2a2a 7061 7261 6d73 2c0a 2020 2020    **params,.    
-0000f100: 2020 2020 290a 0a0a 636c 6173 7320 5366      )...class Sf
-0000f110: 7265 713a 0a20 2020 2022 2222 536e 6f77  req:.    """Snow
-0000f120: 6661 6c6c 2066 7265 7175 656e 6379 2e22  fall frequency."
-0000f130: 2222 0a0a 2020 2020 7468 7265 7368 203d  ""..    thresh =
-0000f140: 2031 0a0a 2020 2020 6465 6620 636f 6d70   1..    def comp
-0000f150: 7574 6528 7468 7265 7368 3d74 6872 6573  ute(thresh=thres
-0000f160: 682c 202a 2a70 6172 616d 7329 3a0a 2020  h, **params):.  
-0000f170: 2020 2020 2020 2222 2243 616c 6375 6c61        """Calcula
-0000f180: 7465 2073 6e6f 7766 616c 6c20 6672 6571  te snowfall freq
-0000f190: 7565 6e63 792e 0a0a 2020 2020 2020 2020  uency...        
-0000f1a0: 5061 7261 6d65 7465 7273 0a20 2020 2020  Parameters.     
-0000f1b0: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020     ----------.  
-0000f1c0: 2020 2020 2020 7468 7265 7368 3a20 696e        thresh: in
-0000f1d0: 7420 6f72 2073 7472 696e 670a 2020 2020  t or string.    
-0000f1e0: 2020 2020 2020 2020 4c69 7175 6964 2077          Liquid w
-0000f1f0: 6174 6572 2065 7175 6976 616c 656e 7420  ater equivalent 
-0000f200: 736e 6f77 6661 6c6c 2072 6174 6520 6162  snowfall rate ab
-0000f210: 6f76 6520 7768 6963 6820 6120 6461 7920  ove which a day 
-0000f220: 6973 0a20 2020 2020 2020 2020 2020 2063  is.            c
-0000f230: 6f6e 7369 6465 7265 6420 6173 2061 2073  onsidered as a s
-0000f240: 6e6f 7720 6461 7920 2864 6566 6175 6c74  now day (default
-0000f250: 3a20 3120 6d6d 2f64 6179 2920 2e0a 2020  : 1 mm/day) ..  
-0000f260: 2020 2020 2020 2020 2020 4966 2074 7970            If typ
-0000f270: 6520 6f66 2074 6872 6573 686f 6c64 2069  e of threshold i
-0000f280: 7320 616e 2069 6e74 6567 6572 2074 6865  s an integer the
-0000f290: 2075 6e69 7420 6973 2073 6574 2074 6f20   unit is set to 
-0000f2a0: 6d6d 2f64 6179 2e0a 0a20 2020 2020 2020  mm/day...       
-0000f2b0: 2052 6574 7572 6e73 0a20 2020 2020 2020   Returns.       
-0000f2c0: 202d 2d2d 2d2d 2d2d 0a20 2020 2020 2020   -------.       
-0000f2d0: 2078 6172 7261 792e 4461 7461 4172 7261   xarray.DataArra
-0000f2e0: 790a 2020 2020 2020 2020 2020 2020 5065  y.            Pe
-0000f2f0: 7263 656e 7461 6765 206f 6620 6461 7973  rcentage of days
-0000f300: 2077 6974 6820 736e 6f77 6661 6c6c 203e   with snowfall >
-0000f310: 207b 7468 7265 7368 7d2e 0a0a 2020 2020   {thresh}...    
-0000f320: 2020 2020 4e6f 7465 730a 2020 2020 2020      Notes.      
-0000f330: 2020 2d2d 2d2d 2d0a 2020 2020 2020 2020    -----.        
-0000f340: 466f 7220 6d6f 7265 2069 6e66 6f72 6d61  For more informa
-0000f350: 7469 6f6e 206f 6e20 7468 6520 696e 7075  tion on the inpu
-0000f360: 7420 7061 7261 6d65 7465 7273 2073 6565  t parameters see
-0000f370: 3a0a 2020 2020 2020 2020 2020 2020 6874  :.            ht
-0000f380: 7470 733a 2f2f 7863 6c69 6d2e 7265 6164  tps://xclim.read
-0000f390: 7468 6564 6f63 732e 696f 2f65 6e2f 7374  thedocs.io/en/st
-0000f3a0: 6162 6c65 2f61 7069 2e68 746d 6c23 7863  able/api.html#xc
-0000f3b0: 6c69 6d2e 696e 6469 6361 746f 7273 2e61  lim.indicators.a
-0000f3c0: 746d 6f73 2e73 6e6f 7766 616c 6c5f 6672  tmos.snowfall_fr
-0000f3d0: 6571 7565 6e63 790a 2020 2020 2020 2020  equency.        
-0000f3e0: 2222 220a 2020 2020 2020 2020 7468 7265  """.        thre
-0000f3f0: 7368 203d 205f 7468 7265 7368 5f73 7472  sh = _thresh_str
-0000f400: 696e 6728 7468 7265 7368 2c20 226d 6d2f  ing(thresh, "mm/
-0000f410: 6461 7922 290a 2020 2020 2020 2020 7265  day").        re
-0000f420: 7475 726e 2078 632e 6174 6d6f 732e 736e  turn xc.atmos.sn
-0000f430: 6f77 6661 6c6c 5f66 7265 7175 656e 6379  owfall_frequency
-0000f440: 280a 2020 2020 2020 2020 2020 2020 7468  (.            th
-0000f450: 7265 7368 3d74 6872 6573 682c 0a20 2020  resh=thresh,.   
-0000f460: 2020 2020 2020 2020 202a 2a70 6172 616d           **param
-0000f470: 732c 0a20 2020 2020 2020 2029 0a0a 0a63  s,.        )...c
-0000f480: 6c61 7373 2055 5443 493a 0a20 2020 2022  lass UTCI:.    "
-0000f490: 2222 556e 6976 6572 7361 6c20 7468 6572  ""Universal ther
-0000f4a0: 6d61 6c20 636c 696d 6174 6520 696e 6465  mal climate inde
-0000f4b0: 782e 2222 220a 0a20 2020 2073 7461 7420  x."""..    stat 
-0000f4c0: 3d20 2261 7665 7261 6765 220a 2020 2020  = "average".    
-0000f4d0: 6d61 736b 5f69 6e76 616c 6964 203d 2054  mask_invalid = T
-0000f4e0: 7275 650a 0a20 2020 2064 6566 2063 6f6d  rue..    def com
-0000f4f0: 7075 7465 2873 7461 743d 7374 6174 2c20  pute(stat=stat, 
-0000f500: 6d61 736b 5f69 6e76 616c 6964 3d6d 6173  mask_invalid=mas
-0000f510: 6b5f 696e 7661 6c69 642c 202a 2a70 6172  k_invalid, **par
-0000f520: 616d 7329 3a0a 2020 2020 2020 2020 2222  ams):.        ""
-0000f530: 2243 616c 6375 6c61 7465 2075 6e69 7665  "Calculate unive
-0000f540: 7273 616c 2074 6865 726d 616c 2063 6c69  rsal thermal cli
-0000f550: 6d61 7465 2069 6e64 6578 2e0a 0a20 2020  mate index...   
-0000f560: 2020 2020 2050 6172 616d 6574 6572 730a       Parameters.
-0000f570: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d2d          --------
-0000f580: 2d2d 0a20 2020 2020 2020 2073 7461 743a  --.        stat:
-0000f590: 207b e280 9861 7665 7261 6765 e280 992c   {...average...,
-0000f5a0: 20e2 8098 7375 6e6c 6974 e280 992c 20e2   ...sunlit..., .
-0000f5b0: 8098 696e 7374 616e 74e2 8099 7d0a 2020  ..instant...}.  
-0000f5c0: 2020 2020 2020 2020 2020 5768 6963 6820            Which 
-0000f5d0: 7374 6174 6973 7469 6320 746f 2061 7070  statistic to app
-0000f5e0: 6c79 2e20 4966 20e2 809c 6176 6572 6167  ly. If ...averag
-0000f5f0: 65e2 809d 2c20 7468 6520 6176 6572 6167  e..., the averag
-0000f600: 6520 6f66 2074 6865 2063 6f73 696e 650a  e of the cosine.
-0000f610: 2020 2020 2020 2020 2020 2020 6f66 2074              of t
-0000f620: 6865 2073 6f6c 6172 207a 656e 6974 6820  he solar zenith 
-0000f630: 616e 676c 6520 6973 2063 616c 6375 6c61  angle is calcula
-0000f640: 7465 642e 0a20 2020 2020 2020 2020 2020  ted..           
-0000f650: 2049 6620 e280 9c69 6e73 7461 6e74 e280   If ...instant..
-0000f660: 9d2c 2074 6865 2069 6e73 7461 6e74 616e  ., the instantan
-0000f670: 656f 7573 2063 6f73 696e 6520 6f66 2074  eous cosine of t
-0000f680: 6865 2073 6f6c 6172 207a 656e 6974 6820  he solar zenith 
-0000f690: 616e 676c 6520 6973 0a20 2020 2020 2020  angle is.       
-0000f6a0: 2020 2020 2063 616c 6375 6c61 7465 642e       calculated.
-0000f6b0: 0a20 2020 2020 2020 2020 2020 2049 6620  .            If 
-0000f6c0: e280 9c73 756e 6c69 74e2 809d 2c20 7468  ...sunlit..., th
-0000f6d0: 6520 636f 7369 6e65 206f 6620 7468 6520  e cosine of the 
-0000f6e0: 736f 6c61 7220 7a65 6e69 7468 2061 6e67  solar zenith ang
-0000f6f0: 6c65 2069 7320 6361 6c63 756c 6174 6564  le is calculated
-0000f700: 0a20 2020 2020 2020 2020 2020 2064 7572  .            dur
-0000f710: 696e 6720 7468 6520 7375 6e6c 6974 2070  ing the sunlit p
-0000f720: 6572 696f 6420 6f66 2065 6163 6820 696e  eriod of each in
-0000f730: 7465 7276 616c 2e0a 2020 2020 2020 2020  terval..        
-0000f740: 2020 2020 4966 20e2 809c 696e 7374 616e      If ...instan
-0000f750: 74e2 809d 2c20 7468 6520 696e 7374 616e  t..., the instan
-0000f760: 7461 6e65 6f75 7320 636f 7369 6e65 206f  taneous cosine o
-0000f770: 6620 7468 6520 736f 6c61 7220 7a65 6e69  f the solar zeni
-0000f780: 7468 2061 6e67 6c65 2069 730a 2020 2020  th angle is.    
-0000f790: 2020 2020 2020 2020 6361 6c63 756c 6174          calculat
-0000f7a0: 6564 2e0a 2020 2020 2020 2020 2020 2020  ed..            
-0000f7b0: 5468 6973 2069 7320 6e65 6365 7373 6172  This is necessar
-0000f7c0: 7920 6966 206d 7274 2069 7320 6e6f 7420  y if mrt is not 
-0000f7d0: 4e6f 6e65 2028 6465 6661 756c 743a 2061  None (default: a
-0000f7e0: 7665 7261 6765 292e 0a20 2020 2020 2020  verage)..       
-0000f7f0: 206d 6173 6b5f 7661 6c69 643a 2062 6f6f   mask_valid: boo
-0000f800: 6c0a 2020 2020 2020 2020 2020 2020 4966  l.            If
-0000f810: 2054 7275 652c 2055 5443 4920 7661 6c75   True, UTCI valu
-0000f820: 6573 2061 7265 204e 614e 2077 6865 7265  es are NaN where
-0000f830: 2061 6e79 206f 6620 7468 6520 696e 7075   any of the inpu
-0000f840: 7473 2061 7265 206f 7574 7369 6465 0a20  ts are outside. 
-0000f850: 2020 2020 2020 2020 2020 2074 6865 6972             their
-0000f860: 2076 616c 6964 6974 7920 7261 6e67 6573   validity ranges
-0000f870: 3a0a 2020 2020 2020 2020 2020 2020 2d35  :.            -5
-0000f880: 30c2 b043 203c 2074 6173 203c 2035 30c2  0..C < tas < 50.
-0000f890: b043 2c0a 2020 2020 2020 2020 2020 2020  .C,.            
-0000f8a0: 2d33 30c2 b043 203c 2074 6173 202d 206d  -30..C < tas - m
-0000f8b0: 7274 203c 2033 30c2 b043 0a20 2020 2020  rt < 30..C.     
-0000f8c0: 2020 2020 2020 2030 2e35 206d 2f73 203c         0.5 m/s <
-0000f8d0: 2073 6663 5769 6e64 203c 2031 372e 3020   sfcWind < 17.0 
-0000f8e0: 6d2f 730a 2020 2020 2020 2020 2020 2020  m/s.            
-0000f8f0: 2864 6566 6175 6c74 3a20 5472 7565 292e  (default: True).
-0000f900: 0a0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
-0000f910: 730a 2020 2020 2020 2020 2d2d 2d2d 2d2d  s.        ------
-0000f920: 2d0a 2020 2020 2020 2020 7861 7272 6179  -.        xarray
-0000f930: 2e44 6174 6141 7272 6179 0a20 2020 2020  .DataArray.     
-0000f940: 2020 2020 2020 2055 6e69 7665 7273 616c         Universal
-0000f950: 2054 6865 726d 616c 2043 6c69 6d61 7465   Thermal Climate
-0000f960: 2049 6e64 6578 2e0a 0a20 2020 2020 2020   Index...       
-0000f970: 204e 6f74 6573 0a20 2020 2020 2020 202d   Notes.        -
-0000f980: 2d2d 2d2d 0a20 2020 2020 2020 2046 6f72  ----.        For
-0000f990: 206d 6f72 6520 696e 666f 726d 6174 696f   more informatio
-0000f9a0: 6e20 6f6e 2074 6865 2069 6e70 7574 2070  n on the input p
-0000f9b0: 6172 616d 6574 6572 7320 7365 653a 0a20  arameters see:. 
-0000f9c0: 2020 2020 2020 2020 2020 2068 7474 7073             https
-0000f9d0: 3a2f 2f78 636c 696d 2e72 6561 6474 6865  ://xclim.readthe
-0000f9e0: 646f 6373 2e69 6f2f 656e 2f73 7461 626c  docs.io/en/stabl
-0000f9f0: 652f 6170 692e 6874 6d6c 2378 636c 696d  e/api.html#xclim
-0000fa00: 2e69 6e64 6963 6174 6f72 732e 6174 6d6f  .indicators.atmo
-0000fa10: 732e 756e 6976 6572 7361 6c5f 7468 6572  s.universal_ther
-0000fa20: 6d61 6c5f 636c 696d 6174 655f 696e 6465  mal_climate_inde
-0000fa30: 780a 2020 2020 2020 2020 2222 220a 2020  x.        """.  
-0000fa40: 2020 2020 2020 7265 7475 726e 2078 632e        return xc.
-0000fa50: 6174 6d6f 732e 756e 6976 6572 7361 6c5f  atmos.universal_
-0000fa60: 7468 6572 6d61 6c5f 636c 696d 6174 655f  thermal_climate_
-0000fa70: 696e 6465 7828 0a20 2020 2020 2020 2020  index(.         
-0000fa80: 2020 2073 7461 743d 7374 6174 2c0a 2020     stat=stat,.  
-0000fa90: 2020 2020 2020 2020 2020 6d61 736b 5f69            mask_i
-0000faa0: 6e76 616c 6964 3d6d 6173 6b5f 696e 7661  nvalid=mask_inva
-0000fab0: 6c69 642c 0a20 2020 2020 2020 2020 2020  lid,.           
-0000fac0: 202a 2a70 6172 616d 732c 0a20 2020 2020   **params,.     
-0000fad0: 2020 2029 0a0a 0a63 6c61 7373 2057 493a     )...class WI:
-0000fae0: 0a20 2020 2022 2222 4e75 6d62 6572 206f  .    """Number o
-0000faf0: 6620 7769 6e74 6572 2064 6179 7320 2874  f winter days (t
-0000fb00: 6173 6d69 6e29 2e22 2222 0a0a 2020 2020  asmin)."""..    
-0000fb10: 7468 7265 7368 203d 202d 3130 0a0a 2020  thresh = -10..  
-0000fb20: 2020 6465 6620 636f 6d70 7574 6528 7468    def compute(th
-0000fb30: 7265 7368 3d74 6872 6573 682c 202a 2a70  resh=thresh, **p
-0000fb40: 6172 616d 7329 3a0a 2020 2020 2020 2020  arams):.        
-0000fb50: 2222 2243 616c 6375 6c61 7465 206e 756d  """Calculate num
-0000fb60: 6265 7220 6f66 2077 696e 7465 7220 6461  ber of winter da
-0000fb70: 7973 2e0a 0a20 2020 2020 2020 2050 6172  ys...        Par
-0000fb80: 616d 6574 6572 730a 2020 2020 2020 2020  ameters.        
-0000fb90: 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020  ----------.     
-0000fba0: 2020 2074 6872 6573 683a 2069 6e74 206f     thresh: int o
-0000fbb0: 7220 7374 7269 6e67 0a20 2020 2020 2020  r string.       
-0000fbc0: 2020 2020 2054 6872 6573 686f 6c64 206d       Threshold m
-0000fbd0: 696e 696d 756d 2074 656d 7065 7261 7475  inimum temperatu
-0000fbe0: 7265 2062 656c 6f77 2077 6869 6368 2061  re below which a
-0000fbf0: 2064 6179 2069 7320 636f 6e73 6964 6572   day is consider
-0000fc00: 6564 0a20 2020 2020 2020 2020 2020 2061  ed.            a
-0000fc10: 7320 6120 7769 6e74 6572 2064 6179 2028  s a winter day (
-0000fc20: 6465 6661 756c 743a 202d 3130 2064 6567  default: -10 deg
-0000fc30: 4329 2e0a 2020 2020 2020 2020 2020 2020  C)..            
-0000fc40: 4966 2074 7970 6520 6f66 2074 6872 6573  If type of thres
-0000fc50: 686f 6c64 2069 7320 616e 2069 6e74 6567  hold is an integ
-0000fc60: 6572 2074 6865 2075 6e69 7420 6973 2073  er the unit is s
-0000fc70: 6574 2074 6f20 6465 6743 2e0a 0a20 2020  et to degC...   
-0000fc80: 2020 2020 2052 6574 7572 6e73 0a20 2020       Returns.   
-0000fc90: 2020 2020 202d 2d2d 2d2d 2d2d 0a20 2020       -------.   
-0000fca0: 2020 2020 2078 6172 7261 792e 4461 7461       xarray.Data
-0000fcb0: 4172 7261 790a 2020 2020 2020 2020 2020  Array.          
-0000fcc0: 2020 4e75 6d62 6572 206f 6620 7769 6e74    Number of wint
-0000fcd0: 6572 2064 6179 732e 0a0a 2020 2020 2020  er days...      
-0000fce0: 2020 4e6f 7465 730a 2020 2020 2020 2020    Notes.        
-0000fcf0: 2d2d 2d2d 2d0a 2020 2020 2020 2020 466f  -----.        Fo
-0000fd00: 7220 6d6f 7265 2069 6e66 6f72 6d61 7469  r more informati
-0000fd10: 6f6e 206f 6e20 7468 6520 696e 7075 7420  on on the input 
-0000fd20: 7061 7261 6d65 7465 7273 2073 6565 3a0a  parameters see:.
-0000fd30: 2020 2020 2020 2020 2020 2020 6874 7470              http
-0000fd40: 733a 2f2f 7863 6c69 6d2e 7265 6164 7468  s://xclim.readth
-0000fd50: 6564 6f63 732e 696f 2f65 6e2f 7374 6162  edocs.io/en/stab
-0000fd60: 6c65 2f61 7069 2e68 746d 6c23 7863 6c69  le/api.html#xcli
-0000fd70: 6d2e 696e 6469 6361 746f 7273 2e61 746d  m.indicators.atm
-0000fd80: 6f73 2e74 6e5f 6461 7973 5f62 656c 6f77  os.tn_days_below
-0000fd90: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-0000fda0: 2020 2020 2074 6872 6573 6820 3d20 5f74       thresh = _t
-0000fdb0: 6872 6573 685f 7374 7269 6e67 2874 6872  hresh_string(thr
-0000fdc0: 6573 682c 2022 6465 6743 2229 0a20 2020  esh, "degC").   
-0000fdd0: 2020 2020 2072 6574 7572 6e20 7863 2e61       return xc.a
-0000fde0: 746d 6f73 2e74 6e5f 6461 7973 5f62 656c  tmos.tn_days_bel
-0000fdf0: 6f77 280a 2020 2020 2020 2020 2020 2020  ow(.            
-0000fe00: 7468 7265 7368 3d74 6872 6573 682c 0a20  thresh=thresh,. 
-0000fe10: 2020 2020 2020 2020 2020 202a 2a70 6172             **par
-0000fe20: 616d 732c 0a20 2020 2020 2020 2029 0a0a  ams,.        )..
-0000fe30: 0a63 6c61 7373 2048 5766 3a0a 2020 2020  .class HWf:.    
-0000fe40: 2222 224e 756d 6265 7220 6f66 2068 6561  """Number of hea
-0000fe50: 7420 7761 7665 7320 2874 6173 6d61 782c  t waves (tasmax,
-0000fe60: 2074 6173 6d69 6e29 2e22 2222 0a0a 2020   tasmin)."""..  
-0000fe70: 2020 7468 7265 7368 5f74 6173 6d69 6e20    thresh_tasmin 
-0000fe80: 3d20 3232 0a20 2020 2074 6872 6573 685f  = 22.    thresh_
-0000fe90: 7461 736d 6178 203d 2033 300a 2020 2020  tasmax = 30.    
-0000fea0: 7769 6e64 6f77 203d 2033 0a0a 2020 2020  window = 3..    
-0000feb0: 6465 6620 636f 6d70 7574 6528 0a20 2020  def compute(.   
-0000fec0: 2020 2020 2074 6872 6573 685f 7461 736d       thresh_tasm
-0000fed0: 696e 3d74 6872 6573 685f 7461 736d 696e  in=thresh_tasmin
-0000fee0: 2c0a 2020 2020 2020 2020 7468 7265 7368  ,.        thresh
-0000fef0: 5f74 6173 6d61 783d 7468 7265 7368 5f74  _tasmax=thresh_t
-0000ff00: 6173 6d61 782c 0a20 2020 2020 2020 2077  asmax,.        w
-0000ff10: 696e 646f 773d 7769 6e64 6f77 2c0a 2020  indow=window,.  
-0000ff20: 2020 2020 2020 2a2a 7061 7261 6d73 2c0a        **params,.
-0000ff30: 2020 2020 293a 0a20 2020 2020 2020 2022      ):.        "
-0000ff40: 2222 4361 6c63 756c 6174 6520 6e75 6d62  ""Calculate numb
-0000ff50: 6572 206f 6620 6865 6174 2077 6176 6573  er of heat waves
-0000ff60: 2e0a 0a20 2020 2020 2020 2050 6172 616d  ...        Param
-0000ff70: 6574 6572 730a 2020 2020 2020 2020 2d2d  eters.        --
-0000ff80: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020 2020  --------.       
-0000ff90: 2074 6872 6573 685f 7461 736d 696e 3a20   thresh_tasmin: 
-0000ffa0: 696e 7420 6f72 2073 7472 696e 670a 2020  int or string.  
-0000ffb0: 2020 2020 2020 2020 2020 5468 7265 7368            Thresh
-0000ffc0: 6f6c 6420 6d69 6e69 6d75 6d20 7465 6d70  old minimum temp
-0000ffd0: 6572 6174 7572 6520 6162 6f76 6520 7768  erature above wh
-0000ffe0: 6963 6820 6120 6461 7920 6973 2063 6f6e  ich a day is con
-0000fff0: 7369 6465 7265 640a 2020 2020 2020 2020  sidered.        
-00010000: 2020 2020 6173 2061 2068 6561 7420 6461      as a heat da
-00010010: 7920 2864 6566 6175 6c74 3a20 3232 2064  y (default: 22 d
-00010020: 6567 4329 2e0a 2020 2020 2020 2020 2020  egC)..          
-00010030: 2020 4966 2074 7970 6520 6f66 2074 6872    If type of thr
-00010040: 6573 686f 6c64 2069 7320 616e 2069 6e74  eshold is an int
-00010050: 6567 6572 2074 6865 2075 6e69 7420 6973  eger the unit is
-00010060: 2073 6574 2074 6f20 6465 6743 2e0a 2020   set to degC..  
-00010070: 2020 2020 2020 7468 7265 7368 5f74 6173        thresh_tas
-00010080: 6d61 783a 2069 6e74 206f 7220 7374 7269  max: int or stri
-00010090: 6e67 0a20 2020 2020 2020 2020 2020 2054  ng.            T
-000100a0: 6872 6573 686f 6c64 206d 6178 696d 756d  hreshold maximum
-000100b0: 2074 656d 7065 7261 7475 7265 2061 626f   temperature abo
-000100c0: 7665 2077 6869 6368 2061 2064 6179 2069  ve which a day i
-000100d0: 7320 636f 6e73 6964 6572 6564 0a20 2020  s considered.   
-000100e0: 2020 2020 2020 2020 2061 7320 6120 7769           as a wi
-000100f0: 6e74 6572 2064 6179 2028 6465 6661 756c  nter day (defaul
-00010100: 743a 2033 3020 6465 6743 292e 0a20 2020  t: 30 degC)..   
-00010110: 2020 2020 2020 2020 2049 6620 7479 7065           If type
-00010120: 206f 6620 7468 7265 7368 6f6c 6420 6973   of threshold is
-00010130: 2061 6e20 696e 7465 6765 7220 7468 6520   an integer the 
-00010140: 756e 6974 2069 7320 7365 7420 746f 2064  unit is set to d
-00010150: 6567 432e 0a20 2020 2020 2020 2077 696e  egC..        win
-00010160: 646f 773a 2069 6e74 0a20 2020 2020 2020  dow: int.       
-00010170: 2020 2020 204d 696e 696d 756d 206e 756d       Minimum num
-00010180: 6265 7220 6f66 2064 6179 7320 7769 7468  ber of days with
-00010190: 2074 656d 7065 7261 7475 7265 2061 626f   temperature abo
-000101a0: 7665 2074 6872 6573 680a 2020 2020 2020  ve thresh.      
-000101b0: 2020 2020 2020 746f 2071 7561 6c69 6679        to qualify
-000101c0: 2061 7320 6120 686f 7420 7370 656c 6c20   as a hot spell 
-000101d0: 2864 6566 6175 6c74 3a20 3329 2e0a 0a20  (default: 3)... 
-000101e0: 2020 2020 2020 2052 6574 7572 6e73 0a20         Returns. 
-000101f0: 2020 2020 2020 202d 2d2d 2d2d 2d2d 0a20         -------. 
-00010200: 2020 2020 2020 2078 6172 7261 792e 4461         xarray.Da
-00010210: 7461 4172 7261 790a 2020 2020 2020 2020  taArray.        
-00010220: 2020 2020 4e75 6d62 6572 206f 6620 6865      Number of he
-00010230: 6174 2077 6176 6573 206f 6620 6174 206c  at waves of at l
-00010240: 6561 7374 207b 7769 6e64 6f77 7d20 636f  east {window} co
-00010250: 6e73 6563 7574 6976 6520 6461 7973 0a20  nsecutive days. 
-00010260: 2020 2020 2020 2020 2020 2077 6974 6820             with 
-00010270: 6d61 7869 6d75 6d20 7465 6d70 6572 6174  maximum temperat
-00010280: 7572 6520 6162 6f76 6520 7b74 6872 6573  ure above {thres
-00010290: 685f 7461 736d 6178 7d20 616e 640a 2020  h_tasmax} and.  
-000102a0: 2020 2020 2020 2020 2020 6d69 6e69 6d75            minimu
-000102b0: 6d20 7465 6d70 6572 6174 7572 6520 6162  m temperature ab
-000102c0: 6f76 6520 7b74 6872 6573 685f 7461 736d  ove {thresh_tasm
-000102d0: 696e 7d2e 0a0a 2020 2020 2020 2020 4e6f  in}...        No
-000102e0: 7465 730a 2020 2020 2020 2020 2d2d 2d2d  tes.        ----
-000102f0: 2d0a 2020 2020 2020 2020 466f 7220 6d6f  -.        For mo
-00010300: 7265 2069 6e66 6f72 6d61 7469 6f6e 206f  re information o
-00010310: 6e20 7468 6520 696e 7075 7420 7061 7261  n the input para
-00010320: 6d65 7465 7273 2073 6565 3a0a 2020 2020  meters see:.    
-00010330: 2020 2020 2020 2020 6874 7470 733a 2f2f          https://
-00010340: 7863 6c69 6d2e 7265 6164 7468 6564 6f63  xclim.readthedoc
-00010350: 732e 696f 2f65 6e2f 7374 6162 6c65 2f61  s.io/en/stable/a
-00010360: 7069 2e68 746d 6c23 7863 6c69 6d2e 696e  pi.html#xclim.in
-00010370: 6469 6361 746f 7273 2e61 746d 6f73 2e68  dicators.atmos.h
-00010380: 6f74 5f73 7065 6c6c 5f66 7265 7175 656e  ot_spell_frequen
-00010390: 6379 0a20 2020 2020 2020 2022 2222 0a20  cy.        """. 
-000103a0: 2020 2020 2020 2074 6872 6573 685f 7461         thresh_ta
-000103b0: 736d 6178 203d 205f 7468 7265 7368 5f73  smax = _thresh_s
-000103c0: 7472 696e 6728 7468 7265 7368 5f74 6173  tring(thresh_tas
-000103d0: 6d61 782c 2022 6465 6743 2229 0a20 2020  max, "degC").   
-000103e0: 2020 2020 2074 6872 6573 685f 7461 736d       thresh_tasm
-000103f0: 696e 203d 205f 7468 7265 7368 5f73 7472  in = _thresh_str
-00010400: 696e 6728 7468 7265 7368 5f74 6173 6d69  ing(thresh_tasmi
-00010410: 6e2c 2022 6465 6743 2229 0a20 2020 2020  n, "degC").     
-00010420: 2020 2072 6574 7572 6e20 7863 2e61 746d     return xc.atm
-00010430: 6f73 2e68 6561 745f 7761 7665 5f66 7265  os.heat_wave_fre
-00010440: 7175 656e 6379 280a 2020 2020 2020 2020  quency(.        
-00010450: 2020 2020 7468 7265 7368 5f74 6173 6d61      thresh_tasma
-00010460: 783d 7468 7265 7368 5f74 6173 6d61 782c  x=thresh_tasmax,
-00010470: 0a20 2020 2020 2020 2020 2020 2074 6872  .            thr
-00010480: 6573 685f 7461 736d 696e 3d74 6872 6573  esh_tasmin=thres
-00010490: 685f 7461 736d 696e 2c0a 2020 2020 2020  h_tasmin,.      
-000104a0: 2020 2020 2020 7769 6e64 6f77 3d77 696e        window=win
-000104b0: 646f 772c 0a20 2020 2020 2020 2020 2020  dow,.           
-000104c0: 202a 2a70 6172 616d 732c 0a20 2020 2020   **params,.     
-000104d0: 2020 2029 0a0a 0a63 6c61 7373 2048 5778     )...class HWx
-000104e0: 3a0a 2020 2020 2222 224d 6178 696d 756d  :.    """Maximum
-000104f0: 206c 656e 6774 6820 6f66 2068 6561 7420   length of heat 
-00010500: 7761 7665 7320 2874 6173 6d61 782c 2074  waves (tasmax, t
-00010510: 6173 6d69 6e29 2e22 2222 0a0a 2020 2020  asmin)."""..    
-00010520: 7468 7265 7368 5f74 6173 6d69 6e20 3d20  thresh_tasmin = 
-00010530: 3232 0a20 2020 2074 6872 6573 685f 7461  22.    thresh_ta
-00010540: 736d 6178 203d 2033 300a 2020 2020 7769  smax = 30.    wi
-00010550: 6e64 6f77 203d 2031 0a0a 2020 2020 6465  ndow = 1..    de
-00010560: 6620 636f 6d70 7574 6528 0a20 2020 2020  f compute(.     
-00010570: 2020 2074 6872 6573 685f 7461 736d 6178     thresh_tasmax
-00010580: 3d74 6872 6573 685f 7461 736d 6178 2c0a  =thresh_tasmax,.
-00010590: 2020 2020 2020 2020 7468 7265 7368 5f74          thresh_t
-000105a0: 6173 6d69 6e3d 7468 7265 7368 5f74 6173  asmin=thresh_tas
-000105b0: 6d69 6e2c 0a20 2020 2020 2020 2077 696e  min,.        win
-000105c0: 646f 773d 7769 6e64 6f77 2c0a 2020 2020  dow=window,.    
-000105d0: 2020 2020 2a2a 7061 7261 6d73 2c0a 2020      **params,.  
-000105e0: 2020 293a 0a20 2020 2020 2020 2022 2222    ):.        """
-000105f0: 4361 6c63 756c 6174 6520 6d61 7869 6d75  Calculate maximu
-00010600: 6d20 6e75 6d62 6572 206f 6620 6865 6174  m number of heat
-00010610: 2077 6176 6573 2e0a 0a20 2020 2020 2020   waves...       
-00010620: 2050 6172 616d 6574 6572 730a 2020 2020   Parameters.    
-00010630: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20      ----------. 
-00010640: 2020 2020 2020 2074 6872 6573 685f 7461         thresh_ta
-00010650: 736d 696e 3a20 696e 7420 6f72 2073 7472  smin: int or str
-00010660: 696e 670a 2020 2020 2020 2020 2020 2020  ing.            
-00010670: 5468 7265 7368 6f6c 6420 6d69 6e69 6d75  Threshold minimu
-00010680: 6d20 7465 6d70 6572 6174 7572 6520 6162  m temperature ab
-00010690: 6f76 6520 7768 6963 6820 6120 6461 7920  ove which a day 
-000106a0: 6973 2063 6f6e 7369 6465 7265 640a 2020  is considered.  
-000106b0: 2020 2020 2020 2020 2020 6173 2061 2068            as a h
-000106c0: 6561 7420 6461 7920 2864 6566 6175 6c74  eat day (default
-000106d0: 3a20 3232 2064 6567 4329 2e0a 2020 2020  : 22 degC)..    
-000106e0: 2020 2020 2020 2020 4966 2074 7970 6520          If type 
-000106f0: 6f66 2074 6872 6573 686f 6c64 2069 7320  of threshold is 
-00010700: 616e 2069 6e74 6567 6572 2074 6865 2075  an integer the u
-00010710: 6e69 7420 6973 2073 6574 2074 6f20 6465  nit is set to de
-00010720: 6743 2e0a 2020 2020 2020 2020 7468 7265  gC..        thre
-00010730: 7368 5f74 6173 6d61 783a 2069 6e74 206f  sh_tasmax: int o
-00010740: 7220 7374 7269 6e67 0a20 2020 2020 2020  r string.       
-00010750: 2020 2020 2054 6872 6573 686f 6c64 206d       Threshold m
-00010760: 6178 696d 756d 2074 656d 7065 7261 7475  aximum temperatu
-00010770: 7265 2061 626f 7665 2077 6869 6368 2061  re above which a
-00010780: 2064 6179 2069 7320 636f 6e73 6964 6572   day is consider
-00010790: 6564 0a20 2020 2020 2020 2020 2020 2061  ed.            a
-000107a0: 7320 6120 7769 6e74 6572 2064 6179 2028  s a winter day (
-000107b0: 6465 6661 756c 743a 2033 3020 6465 6743  default: 30 degC
-000107c0: 292e 0a20 2020 2020 2020 2020 2020 2049  )..            I
-000107d0: 6620 7479 7065 206f 6620 7468 7265 7368  f type of thresh
-000107e0: 6f6c 6420 6973 2061 6e20 696e 7465 6765  old is an intege
-000107f0: 7220 7468 6520 756e 6974 2069 7320 7365  r the unit is se
-00010800: 7420 746f 2064 6567 432e 0a20 2020 2020  t to degC..     
-00010810: 2020 2077 696e 646f 773a 2069 6e74 0a20     window: int. 
-00010820: 2020 2020 2020 2020 2020 204d 696e 696d             Minim
-00010830: 756d 206e 756d 6265 7220 6f66 2064 6179  um number of day
-00010840: 7320 7769 7468 2074 656d 7065 7261 7475  s with temperatu
-00010850: 7265 2061 626f 7665 2074 6872 6573 680a  re above thresh.
-00010860: 2020 2020 2020 2020 2020 2020 746f 2071              to q
-00010870: 7561 6c69 6679 2061 7320 6120 686f 7420  ualify as a hot 
-00010880: 7370 656c 6c20 2864 6566 6175 6c74 3a20  spell (default: 
-00010890: 3129 2e0a 0a20 2020 2020 2020 2052 6574  1)...        Ret
-000108a0: 7572 6e73 0a20 2020 2020 2020 202d 2d2d  urns.        ---
-000108b0: 2d2d 2d2d 0a20 2020 2020 2020 2078 6172  ----.        xar
-000108c0: 7261 792e 4461 7461 4172 7261 790a 2020  ray.DataArray.  
-000108d0: 2020 2020 2020 2020 2020 4d61 7869 6d75            Maximu
-000108e0: 6d20 6c65 6e67 7468 206f 6620 6865 6174  m length of heat
-000108f0: 2077 6176 6573 206f 6620 6174 206c 6561   waves of at lea
-00010900: 7374 207b 7769 6e64 6f77 7d20 636f 6e73  st {window} cons
-00010910: 6563 7574 6976 6520 6461 7973 0a20 2020  ecutive days.   
-00010920: 2020 2020 2020 2020 2077 6974 6820 6d61           with ma
-00010930: 7869 6d75 6d20 7465 6d70 6572 6174 7572  ximum temperatur
-00010940: 6520 6162 6f76 6520 7b74 6872 6573 685f  e above {thresh_
-00010950: 7461 736d 6178 7d20 616e 640a 2020 2020  tasmax} and.    
-00010960: 2020 2020 2020 2020 6d69 6e69 6d75 6d20          minimum 
-00010970: 7465 6d70 6572 6174 7572 6520 6162 6f76  temperature abov
-00010980: 6520 7b74 6872 6573 685f 7461 736d 696e  e {thresh_tasmin
-00010990: 7d2e 0a0a 2020 2020 2020 2020 4e6f 7465  }...        Note
-000109a0: 730a 2020 2020 2020 2020 2d2d 2d2d 2d0a  s.        -----.
-000109b0: 2020 2020 2020 2020 466f 7220 6d6f 7265          For more
-000109c0: 2069 6e66 6f72 6d61 7469 6f6e 206f 6e20   information on 
-000109d0: 7468 6520 696e 7075 7420 7061 7261 6d65  the input parame
-000109e0: 7465 7273 2073 6565 3a0a 2020 2020 2020  ters see:.      
-000109f0: 2020 2020 2020 6874 7470 733a 2f2f 7863        https://xc
-00010a00: 6c69 6d2e 7265 6164 7468 6564 6f63 732e  lim.readthedocs.
-00010a10: 696f 2f65 6e2f 7374 6162 6c65 2f61 7069  io/en/stable/api
-00010a20: 2e68 746d 6c23 7863 6c69 6d2e 696e 6469  .html#xclim.indi
-00010a30: 6361 746f 7273 2e61 746d 6f73 2e68 6561  cators.atmos.hea
-00010a40: 745f 7761 7665 5f6d 6178 5f6c 656e 6774  t_wave_max_lengt
-00010a50: 680a 2020 2020 2020 2020 2222 220a 2020  h.        """.  
-00010a60: 2020 2020 2020 7468 7265 7368 5f74 6173        thresh_tas
-00010a70: 6d61 7820 3d20 5f74 6872 6573 685f 7374  max = _thresh_st
-00010a80: 7269 6e67 2874 6872 6573 685f 7461 736d  ring(thresh_tasm
-00010a90: 6178 2c20 2264 6567 4322 290a 2020 2020  ax, "degC").    
-00010aa0: 2020 2020 7468 7265 7368 5f74 6173 6d69      thresh_tasmi
-00010ab0: 6e20 3d20 5f74 6872 6573 685f 7374 7269  n = _thresh_stri
-00010ac0: 6e67 2874 6872 6573 685f 7461 736d 696e  ng(thresh_tasmin
-00010ad0: 2c20 2264 6567 4322 290a 2020 2020 2020  , "degC").      
-00010ae0: 2020 7265 7475 726e 2078 632e 6174 6d6f    return xc.atmo
-00010af0: 732e 6865 6174 5f77 6176 655f 6d61 785f  s.heat_wave_max_
-00010b00: 6c65 6e67 7468 280a 2020 2020 2020 2020  length(.        
-00010b10: 2020 2020 7468 7265 7368 5f74 6173 6d61      thresh_tasma
-00010b20: 783d 7468 7265 7368 5f74 6173 6d61 782c  x=thresh_tasmax,
-00010b30: 0a20 2020 2020 2020 2020 2020 2074 6872  .            thr
-00010b40: 6573 685f 7461 736d 696e 3d74 6872 6573  esh_tasmin=thres
-00010b50: 685f 7461 736d 696e 2c0a 2020 2020 2020  h_tasmin,.      
-00010b60: 2020 2020 2020 7769 6e64 6f77 3d77 696e        window=win
-00010b70: 646f 772c 0a20 2020 2020 2020 2020 2020  dow,.           
-00010b80: 202a 2a70 6172 616d 732c 0a20 2020 2020   **params,.     
-00010b90: 2020 2029 0a0a 0a63 6c61 7373 2047 5353     )...class GSS
-00010ba0: 3a0a 2020 2020 2222 2247 726f 7769 6e67  :.    """Growing
-00010bb0: 2073 6561 736f 6e20 7374 6172 7420 2874   season start (t
-00010bc0: 6173 292e 2222 220a 0a20 2020 2074 6872  as)."""..    thr
-00010bd0: 6573 6820 3d20 350a 2020 2020 7769 6e64  esh = 5.    wind
-00010be0: 6f77 203d 2035 0a0a 2020 2020 6465 6620  ow = 5..    def 
-00010bf0: 636f 6d70 7574 6528 7468 7265 7368 3d74  compute(thresh=t
-00010c00: 6872 6573 682c 2077 696e 646f 773d 7769  hresh, window=wi
-00010c10: 6e64 6f77 2c20 2a2a 7061 7261 6d73 293a  ndow, **params):
-00010c20: 0a20 2020 2020 2020 2022 2222 4361 6c63  .        """Calc
-00010c30: 756c 6174 6520 6772 6f77 696e 6720 7365  ulate growing se
-00010c40: 6173 6f6e 2073 7461 7274 2e0a 0a20 2020  ason start...   
-00010c50: 2020 2020 2050 6172 616d 6574 6572 730a       Parameters.
-00010c60: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d2d          --------
-00010c70: 2d2d 0a20 2020 2020 2020 2074 6872 6573  --.        thres
-00010c80: 683a 2069 6e74 206f 7220 7374 7269 6e67  h: int or string
-00010c90: 0a20 2020 2020 2020 2020 2020 2054 6872  .            Thr
-00010ca0: 6573 686f 6c64 2074 656d 7065 7261 7475  eshold temperatu
-00010cb0: 7265 2061 626f 7665 2077 6869 6368 2074  re above which t
-00010cc0: 6865 2067 726f 7769 6e67 2073 6561 736f  he growing seaso
-00010cd0: 6e20 7374 6172 7473 0a20 2020 2020 2020  n starts.       
-00010ce0: 2020 2020 2028 6465 6661 756c 743a 2035       (default: 5
-00010cf0: 2064 6567 4329 2e0a 2020 2020 2020 2020   degC)..        
-00010d00: 2020 2020 4966 2074 7970 6520 6f66 2074      If type of t
-00010d10: 6872 6573 686f 6c64 2069 7320 616e 2069  hreshold is an i
-00010d20: 6e74 6567 6572 2074 6865 2075 6e69 7420  nteger the unit 
-00010d30: 6973 2073 6574 2074 6f20 6465 6743 2e0a  is set to degC..
-00010d40: 2020 2020 2020 2020 7769 6e64 6f77 3a20          window: 
-00010d50: 696e 740a 2020 2020 2020 2020 2020 2020  int.            
-00010d60: 4d69 6e69 6d75 6d20 6e75 6d62 6572 206f  Minimum number o
-00010d70: 6620 6461 7973 2077 6974 6820 7465 6d70  f days with temp
-00010d80: 6572 6174 7572 6520 6162 6f76 6520 7468  erature above th
-00010d90: 7265 7368 6f6c 640a 2020 2020 2020 2020  reshold.        
-00010da0: 2020 2020 6e65 6564 6564 2066 6f72 2065      needed for e
-00010db0: 7661 6c75 6174 696f 6e20 2864 6566 6175  valuation (defau
-00010dc0: 6c74 3a20 3529 2e0a 0a20 2020 2020 2020  lt: 5)...       
-00010dd0: 2052 6574 7572 6e73 0a20 2020 2020 2020   Returns.       
-00010de0: 202d 2d2d 2d2d 2d2d 0a20 2020 2020 2020   -------.       
-00010df0: 2078 6172 7261 792e 4461 7461 4172 7261   xarray.DataArra
-00010e00: 790a 2020 2020 2020 2020 2020 2020 4772  y.            Gr
-00010e10: 6f77 696e 6720 7365 6173 6f6e 2073 7461  owing season sta
-00010e20: 7274 2e0a 0a20 2020 2020 2020 204e 6f74  rt...        Not
-00010e30: 6573 0a20 2020 2020 2020 202d 2d2d 2d2d  es.        -----
-00010e40: 0a20 2020 2020 2020 2046 6f72 206d 6f72  .        For mor
-00010e50: 6520 696e 666f 726d 6174 696f 6e20 6f6e  e information on
-00010e60: 2074 6865 2069 6e70 7574 2070 6172 616d   the input param
-00010e70: 6574 6572 7320 7365 653a 0a20 2020 2020  eters see:.     
-00010e80: 2020 2020 2020 2068 7474 7073 3a2f 2f78         https://x
-00010e90: 636c 696d 2e72 6561 6474 6865 646f 6373  clim.readthedocs
-00010ea0: 2e69 6f2f 656e 2f73 7461 626c 652f 6170  .io/en/stable/ap
-00010eb0: 692e 6874 6d6c 2378 636c 696d 2e69 6e64  i.html#xclim.ind
-00010ec0: 6963 6174 6f72 732e 6174 6d6f 732e 6772  icators.atmos.gr
-00010ed0: 6f77 696e 675f 7365 6173 6f6e 5f73 7461  owing_season_sta
-00010ee0: 7274 0a20 2020 2020 2020 2022 2222 0a20  rt.        """. 
-00010ef0: 2020 2020 2020 2074 6872 6573 6820 3d20         thresh = 
-00010f00: 5f74 6872 6573 685f 7374 7269 6e67 2874  _thresh_string(t
-00010f10: 6872 6573 682c 2022 6465 6743 2229 0a20  hresh, "degC"). 
-00010f20: 2020 2020 2020 2072 6574 7572 6e20 7863         return xc
-00010f30: 2e61 746d 6f73 2e67 726f 7769 6e67 5f73  .atmos.growing_s
-00010f40: 6561 736f 6e5f 7374 6172 7428 0a20 2020  eason_start(.   
-00010f50: 2020 2020 2020 2020 2074 6872 6573 683d           thresh=
-00010f60: 7468 7265 7368 2c0a 2020 2020 2020 2020  thresh,.        
-00010f70: 2020 2020 7769 6e64 6f77 3d77 696e 646f      window=windo
-00010f80: 772c 0a20 2020 2020 2020 2020 2020 202a  w,.            *
-00010f90: 2a70 6172 616d 732c 0a20 2020 2020 2020  *params,.       
-00010fa0: 2029 0a0a 0a63 6c61 7373 2047 5345 3a0a   )...class GSE:.
-00010fb0: 2020 2020 2222 2247 726f 7769 6e67 2073      """Growing s
-00010fc0: 6561 736f 6e20 656e 6420 2874 6173 292e  eason end (tas).
-00010fd0: 2222 220a 0a20 2020 2074 6872 6573 6820  """..    thresh 
-00010fe0: 3d20 350a 2020 2020 7769 6e64 6f77 203d  = 5.    window =
-00010ff0: 2035 0a0a 2020 2020 6465 6620 636f 6d70   5..    def comp
-00011000: 7574 6528 7468 7265 7368 3d74 6872 6573  ute(thresh=thres
-00011010: 682c 2077 696e 646f 773d 7769 6e64 6f77  h, window=window
-00011020: 2c20 2a2a 7061 7261 6d73 293a 0a20 2020  , **params):.   
-00011030: 2020 2020 2022 2222 4361 6c63 756c 6174       """Calculat
-00011040: 6520 6772 6f77 696e 6720 7365 6173 6f6e  e growing season
-00011050: 2065 6e64 2e0a 0a20 2020 2020 2020 2050   end...        P
-00011060: 6172 616d 6574 6572 730a 2020 2020 2020  arameters.      
-00011070: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020    ----------.   
-00011080: 2020 2020 2074 6872 6573 683a 2069 6e74       thresh: int
-00011090: 206f 7220 7374 7269 6e67 0a20 2020 2020   or string.     
-000110a0: 2020 2020 2020 2054 6872 6573 686f 6c64         Threshold
-000110b0: 2074 656d 7065 7261 7475 7265 2062 656c   temperature bel
-000110c0: 6f77 2077 6869 6368 2074 6865 2067 726f  ow which the gro
-000110d0: 7769 6e67 2073 6561 736f 6e20 656e 6473  wing season ends
-000110e0: 0a20 2020 2020 2020 2020 2020 2028 6465  .            (de
-000110f0: 6661 756c 743a 2035 2064 6567 4329 2e0a  fault: 5 degC)..
-00011100: 2020 2020 2020 2020 2020 2020 4966 2074              If t
-00011110: 7970 6520 6f66 2074 6872 6573 686f 6c64  ype of threshold
-00011120: 2069 7320 616e 2069 6e74 6567 6572 2074   is an integer t
-00011130: 6865 2075 6e69 7420 6973 2073 6574 2074  he unit is set t
-00011140: 6f20 6465 6743 2e0a 2020 2020 2020 2020  o degC..        
-00011150: 7769 6e64 6f77 3a20 696e 740a 2020 2020  window: int.    
-00011160: 2020 2020 2020 2020 4d69 6e69 6d75 6d20          Minimum 
-00011170: 6e75 6d62 6572 206f 6620 6461 7973 2077  number of days w
-00011180: 6974 6820 7465 6d70 6572 6174 7572 6520  ith temperature 
-00011190: 6265 6c6f 7720 7468 7265 7368 6f6c 640a  below threshold.
-000111a0: 2020 2020 2020 2020 2020 2020 6e65 6564              need
-000111b0: 6564 2066 6f72 2065 7661 6c75 6174 696f  ed for evaluatio
-000111c0: 6e20 2864 6566 6175 6c74 3a20 3529 2e0a  n (default: 5)..
-000111d0: 0a20 2020 2020 2020 2052 6574 7572 6e73  .        Returns
-000111e0: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
-000111f0: 0a20 2020 2020 2020 2078 6172 7261 792e  .        xarray.
-00011200: 4461 7461 4172 7261 790a 2020 2020 2020  DataArray.      
-00011210: 2020 2020 2020 4772 6f77 696e 6720 7365        Growing se
-00011220: 6173 6f6e 2065 6e64 2e0a 0a20 2020 2020  ason end...     
-00011230: 2020 204e 6f74 6573 0a20 2020 2020 2020     Notes.       
-00011240: 202d 2d2d 2d2d 0a20 2020 2020 2020 2046   -----.        F
-00011250: 6f72 206d 6f72 6520 696e 666f 726d 6174  or more informat
-00011260: 696f 6e20 6f6e 2074 6865 2069 6e70 7574  ion on the input
-00011270: 2070 6172 616d 6574 6572 7320 7365 653a   parameters see:
-00011280: 0a20 2020 2020 2020 2020 2020 2068 7474  .            htt
-00011290: 7073 3a2f 2f78 636c 696d 2e72 6561 6474  ps://xclim.readt
-000112a0: 6865 646f 6373 2e69 6f2f 656e 2f73 7461  hedocs.io/en/sta
-000112b0: 626c 652f 6170 692e 6874 6d6c 2378 636c  ble/api.html#xcl
-000112c0: 696d 2e69 6e64 6963 6174 6f72 732e 6174  im.indicators.at
-000112d0: 6d6f 732e 6772 6f77 696e 675f 7365 6173  mos.growing_seas
-000112e0: 6f6e 5f65 6e64 0a20 2020 2020 2020 2022  on_end.        "
-000112f0: 2222 0a20 2020 2020 2020 2074 6872 6573  "".        thres
-00011300: 6820 3d20 5f74 6872 6573 685f 7374 7269  h = _thresh_stri
-00011310: 6e67 2874 6872 6573 682c 2022 6465 6743  ng(thresh, "degC
-00011320: 2229 0a20 2020 2020 2020 2072 6574 7572  ").        retur
-00011330: 6e20 7863 2e61 746d 6f73 2e67 726f 7769  n xc.atmos.growi
-00011340: 6e67 5f73 6561 736f 6e5f 656e 6428 0a20  ng_season_end(. 
-00011350: 2020 2020 2020 2020 2020 2074 6872 6573             thres
-00011360: 683d 7468 7265 7368 2c0a 2020 2020 2020  h=thresh,.      
-00011370: 2020 2020 2020 7769 6e64 6f77 3d77 696e        window=win
-00011380: 646f 772c 0a20 2020 2020 2020 2020 2020  dow,.           
-00011390: 202a 2a70 6172 616d 732c 0a20 2020 2020   **params,.     
-000113a0: 2020 2029 0a0a 0a63 6c61 7373 2046 4653     )...class FFS
-000113b0: 3a0a 2020 2020 2222 2246 726f 7374 2066  :.    """Frost f
-000113c0: 7265 6520 7365 6173 6f6e 2073 7461 7274  ree season start
-000113d0: 2028 7461 736d 696e 292e 2222 220a 0a20   (tasmin).""".. 
-000113e0: 2020 2074 6872 6573 6820 3d20 300a 2020     thresh = 0.  
-000113f0: 2020 7769 6e64 6f77 203d 2035 0a0a 2020    window = 5..  
-00011400: 2020 6465 6620 636f 6d70 7574 6528 7468    def compute(th
-00011410: 7265 7368 3d74 6872 6573 682c 2077 696e  resh=thresh, win
-00011420: 646f 773d 7769 6e64 6f77 2c20 2a2a 7061  dow=window, **pa
-00011430: 7261 6d73 293a 0a20 2020 2020 2020 2022  rams):.        "
-00011440: 2222 4361 6c63 756c 6174 6520 6672 6f73  ""Calculate fros
-00011450: 7420 6672 6565 2073 6561 736f 6e20 7374  t free season st
-00011460: 6172 742e 0a0a 2020 2020 2020 2020 5061  art...        Pa
-00011470: 7261 6d65 7465 7273 0a20 2020 2020 2020  rameters.       
-00011480: 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020   ----------.    
-00011490: 2020 2020 7468 7265 7368 3a20 696e 7420      thresh: int 
-000114a0: 6f72 2073 7472 696e 670a 2020 2020 2020  or string.      
-000114b0: 2020 2020 2020 5468 7265 7368 6f6c 6420        Threshold 
-000114c0: 6d69 6e69 6d75 6d20 7465 6d70 6572 6174  minimum temperat
-000114d0: 7572 6520 6162 6f76 6520 7768 6963 6820  ure above which 
-000114e0: 7468 6520 6672 6f73 7420 6672 6565 2073  the frost free s
-000114f0: 6561 736f 6e0a 2020 2020 2020 2020 2020  eason.          
-00011500: 2020 7374 6172 7473 2028 6465 6661 756c    starts (defaul
-00011510: 743a 2030 2064 6567 4329 2e0a 2020 2020  t: 0 degC)..    
-00011520: 2020 2020 2020 2020 4966 2074 7970 6520          If type 
-00011530: 6f66 2074 6872 6573 686f 6c64 2069 7320  of threshold is 
-00011540: 616e 2069 6e74 6567 6572 2074 6865 2075  an integer the u
-00011550: 6e69 7420 6973 2073 6574 2074 6f20 6465  nit is set to de
-00011560: 6743 2e0a 2020 2020 2020 2020 7769 6e64  gC..        wind
-00011570: 6f77 3a20 696e 740a 2020 2020 2020 2020  ow: int.        
-00011580: 2020 2020 4d69 6e69 6d75 6d20 6e75 6d62      Minimum numb
-00011590: 6572 206f 6620 6461 7973 2077 6974 6820  er of days with 
-000115a0: 7465 6d70 6572 6174 7572 6520 6162 6f76  temperature abov
-000115b0: 6520 7468 7265 7368 6f6c 640a 2020 2020  e threshold.    
-000115c0: 2020 2020 2020 2020 6e65 6564 6564 2066          needed f
-000115d0: 6f72 2065 7661 6c75 6174 696f 6e20 2864  or evaluation (d
-000115e0: 6566 6175 6c74 3a20 3529 2e0a 0a20 2020  efault: 5)...   
-000115f0: 2020 2020 2052 6574 7572 6e73 0a20 2020       Returns.   
-00011600: 2020 2020 202d 2d2d 2d2d 2d2d 0a20 2020       -------.   
-00011610: 2020 2020 2078 6172 7261 792e 4461 7461       xarray.Data
-00011620: 4172 7261 790a 2020 2020 2020 2020 2020  Array.          
-00011630: 2020 4672 6f73 7420 6672 6565 2073 6561    Frost free sea
-00011640: 736f 6e20 7374 6172 742e 0a0a 2020 2020  son start...    
-00011650: 2020 2020 4e6f 7465 730a 2020 2020 2020      Notes.      
-00011660: 2020 2d2d 2d2d 2d0a 2020 2020 2020 2020    -----.        
-00011670: 466f 7220 6d6f 7265 2069 6e66 6f72 6d61  For more informa
-00011680: 7469 6f6e 206f 6e20 7468 6520 696e 7075  tion on the inpu
-00011690: 7420 7061 7261 6d65 7465 7273 2073 6565  t parameters see
-000116a0: 3a0a 2020 2020 2020 2020 2020 2020 6874  :.            ht
-000116b0: 7470 733a 2f2f 7863 6c69 6d2e 7265 6164  tps://xclim.read
-000116c0: 7468 6564 6f63 732e 696f 2f65 6e2f 7374  thedocs.io/en/st
-000116d0: 6162 6c65 2f61 7069 2e68 746d 6c23 7863  able/api.html#xc
-000116e0: 6c69 6d2e 696e 6469 6361 746f 7273 2e61  lim.indicators.a
-000116f0: 746d 6f73 2e66 726f 7374 5f66 7265 655f  tmos.frost_free_
-00011700: 7365 6173 6f6e 5f73 7461 7274 0a20 2020  season_start.   
-00011710: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-00011720: 2074 6872 6573 6820 3d20 5f74 6872 6573   thresh = _thres
-00011730: 685f 7374 7269 6e67 2874 6872 6573 682c  h_string(thresh,
-00011740: 2022 6465 6743 2229 0a20 2020 2020 2020   "degC").       
-00011750: 2072 6574 7572 6e20 7863 2e61 746d 6f73   return xc.atmos
-00011760: 2e66 726f 7374 5f66 7265 655f 7365 6173  .frost_free_seas
-00011770: 6f6e 5f73 7461 7274 280a 2020 2020 2020  on_start(.      
-00011780: 2020 2020 2020 7468 7265 7368 3d74 6872        thresh=thr
-00011790: 6573 682c 0a20 2020 2020 2020 2020 2020  esh,.           
-000117a0: 2077 696e 646f 773d 7769 6e64 6f77 2c0a   window=window,.
-000117b0: 2020 2020 2020 2020 2020 2020 2a2a 7061              **pa
-000117c0: 7261 6d73 2c0a 2020 2020 2020 2020 290a  rams,.        ).
-000117d0: 0a0a 636c 6173 7320 4646 453a 0a20 2020  ..class FFE:.   
-000117e0: 2022 2222 4672 6f73 7420 6672 6565 2073   """Frost free s
-000117f0: 6561 736f 6e20 656e 6420 2874 6173 6d69  eason end (tasmi
-00011800: 6e29 2e22 2222 0a0a 2020 2020 7468 7265  n)."""..    thre
-00011810: 7368 203d 2030 0a20 2020 2077 696e 646f  sh = 0.    windo
-00011820: 7720 3d20 350a 0a20 2020 2064 6566 2063  w = 5..    def c
-00011830: 6f6d 7075 7465 2874 6872 6573 683d 7468  ompute(thresh=th
-00011840: 7265 7368 2c20 7769 6e64 6f77 3d77 696e  resh, window=win
-00011850: 646f 772c 202a 2a70 6172 616d 7329 3a0a  dow, **params):.
-00011860: 2020 2020 2020 2020 2222 2243 616c 6375          """Calcu
-00011870: 6c61 7465 2066 726f 7374 2066 7265 6520  late frost free 
-00011880: 7365 6173 6f6e 2065 6e64 2e0a 0a20 2020  season end...   
-00011890: 2020 2020 2050 6172 616d 6574 6572 730a       Parameters.
-000118a0: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d2d          --------
-000118b0: 2d2d 0a20 2020 2020 2020 2074 6872 6573  --.        thres
-000118c0: 683a 2069 6e74 206f 7220 7374 7269 6e67  h: int or string
-000118d0: 0a20 2020 2020 2020 2020 2020 2054 6872  .            Thr
-000118e0: 6573 686f 6c64 206d 696e 696d 756d 2074  eshold minimum t
-000118f0: 656d 7065 7261 7475 7265 2062 656c 6f77  emperature below
-00011900: 2077 6869 6368 2074 6865 2066 726f 7374   which the frost
-00011910: 2066 7265 6520 7365 6173 6f6e 0a20 2020   free season.   
-00011920: 2020 2020 2020 2020 2065 6e64 7320 2864           ends (d
-00011930: 6566 6175 6c74 3a20 3020 6465 6743 292e  efault: 0 degC).
-00011940: 0a20 2020 2020 2020 2020 2020 2049 6620  .            If 
-00011950: 7479 7065 206f 6620 7468 7265 7368 6f6c  type of threshol
-00011960: 6420 6973 2061 6e20 696e 7465 6765 7220  d is an integer 
-00011970: 7468 6520 756e 6974 2069 7320 7365 7420  the unit is set 
-00011980: 746f 2064 6567 432e 0a20 2020 2020 2020  to degC..       
-00011990: 2077 696e 646f 773a 2069 6e74 0a20 2020   window: int.   
-000119a0: 2020 2020 2020 2020 204d 696e 696d 756d           Minimum
-000119b0: 206e 756d 6265 7220 6f66 2064 6179 7320   number of days 
-000119c0: 7769 7468 2074 656d 7065 7261 7475 7265  with temperature
-000119d0: 2062 656c 6f77 2074 6872 6573 686f 6c64   below threshold
-000119e0: 0a20 2020 2020 2020 2020 2020 206e 6565  .            nee
-000119f0: 6465 6420 666f 7220 6576 616c 7561 7469  ded for evaluati
-00011a00: 6f6e 2028 6465 6661 756c 743a 2035 292e  on (default: 5).
-00011a10: 0a0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
-00011a20: 730a 2020 2020 2020 2020 2d2d 2d2d 2d2d  s.        ------
-00011a30: 2d0a 2020 2020 2020 2020 7861 7272 6179  -.        xarray
-00011a40: 2e44 6174 6141 7272 6179 0a20 2020 2020  .DataArray.     
-00011a50: 2020 2020 2020 2046 726f 7374 2066 7265         Frost fre
-00011a60: 6520 7365 6173 6f6e 2065 6e64 2e0a 0a20  e season end... 
-00011a70: 2020 2020 2020 204e 6f74 6573 0a20 2020         Notes.   
-00011a80: 2020 2020 202d 2d2d 2d2d 0a20 2020 2020       -----.     
-00011a90: 2020 2046 6f72 206d 6f72 6520 696e 666f     For more info
-00011aa0: 726d 6174 696f 6e20 6f6e 2074 6865 2069  rmation on the i
-00011ab0: 6e70 7574 2070 6172 616d 6574 6572 7320  nput parameters 
-00011ac0: 7365 653a 0a20 2020 2020 2020 2020 2020  see:.           
-00011ad0: 2068 7474 7073 3a2f 2f78 636c 696d 2e72   https://xclim.r
-00011ae0: 6561 6474 6865 646f 6373 2e69 6f2f 656e  eadthedocs.io/en
-00011af0: 2f73 7461 626c 652f 6170 692e 6874 6d6c  /stable/api.html
-00011b00: 2378 636c 696d 2e69 6e64 6963 6174 6f72  #xclim.indicator
-00011b10: 732e 6174 6d6f 732e 6672 6f73 745f 6672  s.atmos.frost_fr
-00011b20: 6565 5f73 6561 736f 6e5f 656e 640a 2020  ee_season_end.  
-00011b30: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-00011b40: 2020 7468 7265 7368 203d 205f 7468 7265    thresh = _thre
-00011b50: 7368 5f73 7472 696e 6728 7468 7265 7368  sh_string(thresh
-00011b60: 2c20 2264 6567 4322 290a 2020 2020 2020  , "degC").      
-00011b70: 2020 7265 7475 726e 2078 632e 6174 6d6f    return xc.atmo
-00011b80: 732e 6672 6f73 745f 6672 6565 5f73 6561  s.frost_free_sea
-00011b90: 736f 6e5f 656e 6428 0a20 2020 2020 2020  son_end(.       
-00011ba0: 2020 2020 2074 6872 6573 683d 7468 7265       thresh=thre
-00011bb0: 7368 2c0a 2020 2020 2020 2020 2020 2020  sh,.            
-00011bc0: 7769 6e64 6f77 3d77 696e 646f 772c 0a20  window=window,. 
-00011bd0: 2020 2020 2020 2020 2020 202a 2a70 6172             **par
-00011be0: 616d 732c 0a20 2020 2020 2020 2029 0a0a  ams,.        )..
-00011bf0: 0a63 6c61 7373 2046 473a 0a20 2020 2022  .class FG:.    "
-00011c00: 2222 4d65 616e 2064 6169 6c79 206d 6561  ""Mean daily mea
-00011c10: 6e20 7769 6e64 2073 7065 6564 2e22 2222  n wind speed."""
-00011c20: 0a0a 2020 2020 6465 6620 636f 6d70 7574  ..    def comput
-00011c30: 6528 2a2a 7061 7261 6d73 293a 0a20 2020  e(**params):.   
-00011c40: 2020 2020 2022 2222 4361 6c63 756c 6174       """Calculat
-00011c50: 6520 6d65 616e 2064 6169 6c79 206d 6561  e mean daily mea
-00011c60: 6e20 7769 6e64 2073 7065 6564 2e0a 0a20  n wind speed... 
-00011c70: 2020 2020 2020 2052 6574 7572 6e73 0a20         Returns. 
-00011c80: 2020 2020 2020 202d 2d2d 2d2d 2d2d 0a20         -------. 
-00011c90: 2020 2020 2020 2078 6172 7261 792e 4461         xarray.Da
-00011ca0: 7461 4172 7261 790a 2020 2020 2020 2020  taArray.        
-00011cb0: 2020 2020 4d65 616e 2064 6169 6c79 206d      Mean daily m
-00011cc0: 6561 6e20 7769 6e64 2073 7065 6564 2e0a  ean wind speed..
-00011cd0: 0a20 2020 2020 2020 204e 6f74 6573 0a20  .        Notes. 
-00011ce0: 2020 2020 2020 202d 2d2d 2d2d 0a20 2020         -----.   
-00011cf0: 2020 2020 2049 6620 7366 6357 696e 6420       If sfcWind 
-00011d00: 6973 206e 6f74 2070 726f 7669 6465 6420  is not provided 
-00011d10: 696e 2060 6473 6020 7366 6357 696e 6420  in `ds` sfcWind 
-00011d20: 636f 756c 6420 6265 2063 6f6d 7075 7465  could be compute
-00011d30: 640a 2020 2020 2020 2020 6672 6f6d 2060  d.        from `
-00011d40: 6473 602e 7561 7320 616e 6420 6064 7360  ds`.uas and `ds`
-00011d50: 2e76 6173 2e0a 0a20 2020 2020 2020 2046  .vas...        F
-00011d60: 6f72 2069 6e66 6f72 6d61 7469 6f6e 206f  or information o
-00011d70: 6e20 7468 6520 696e 7075 7420 7061 7261  n the input para
-00011d80: 6d65 7465 7273 2073 6565 3a0a 2020 2020  meters see:.    
-00011d90: 2020 2020 2020 2020 6874 7470 733a 2f2f          https://
-00011da0: 7863 6c69 6d2e 7265 6164 7468 6564 6f63  xclim.readthedoc
-00011db0: 732e 696f 2f65 6e2f 7374 6162 6c65 2f61  s.io/en/stable/a
-00011dc0: 7069 2e68 746d 6c23 7863 6c69 6d2e 696e  pi.html#xclim.in
-00011dd0: 6469 6361 746f 7273 2e61 746d 6f73 2e73  dicators.atmos.s
-00011de0: 6663 5769 6e64 5f6d 6561 6e0a 2020 2020  fcWind_mean.    
-00011df0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-00011e00: 6966 2022 7366 6357 696e 6422 206e 6f74  if "sfcWind" not
-00011e10: 2069 6e20 7061 7261 6d73 5b22 6473 225d   in params["ds"]
-00011e20: 3a0a 2020 2020 2020 2020 2020 2020 7061  :.            pa
-00011e30: 7261 6d73 5b22 6473 225d 5b22 7366 6357  rams["ds"]["sfcW
-00011e40: 696e 6422 5d20 3d20 7863 2e61 746d 6f73  ind"] = xc.atmos
-00011e50: 2e77 696e 645f 7370 6565 645f 6672 6f6d  .wind_speed_from
-00011e60: 5f76 6563 746f 7228 0a20 2020 2020 2020  _vector(.       
-00011e70: 2020 2020 2020 2020 2064 733d 7061 7261           ds=para
-00011e80: 6d73 5b22 6473 225d 2c0a 2020 2020 2020  ms["ds"],.      
-00011e90: 2020 2020 2020 295b 305d 0a20 2020 2020        )[0].     
-00011ea0: 2020 2072 6574 7572 6e20 7863 2e61 746d     return xc.atm
-00011eb0: 6f73 2e73 6663 5769 6e64 5f6d 6561 6e28  os.sfcWind_mean(
-00011ec0: 2a2a 7061 7261 6d73 290a 0a0a 636c 6173  **params)...clas
-00011ed0: 7320 4647 6e3a 0a20 2020 2022 2222 4d69  s FGn:.    """Mi
-00011ee0: 6e69 6d75 6d20 6461 696c 7920 6d65 616e  nimum daily mean
-00011ef0: 2077 696e 6420 7370 6565 642e 2222 220a   wind speed.""".
-00011f00: 0a20 2020 2064 6566 2063 6f6d 7075 7465  .    def compute
-00011f10: 282a 2a70 6172 616d 7329 3a0a 2020 2020  (**params):.    
-00011f20: 2020 2020 2222 2243 616c 6375 6c61 7465      """Calculate
-00011f30: 206d 696e 696d 756d 2064 6169 6c79 206d   minimum daily m
-00011f40: 6561 6e20 7769 6e64 2073 7065 6564 2e0a  ean wind speed..
-00011f50: 0a20 2020 2020 2020 2052 6574 7572 6e73  .        Returns
-00011f60: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
-00011f70: 0a20 2020 2020 2020 2078 6172 7261 792e  .        xarray.
-00011f80: 4461 7461 4172 7261 790a 2020 2020 2020  DataArray.      
-00011f90: 2020 2020 2020 4d69 6e69 6d75 6d20 6461        Minimum da
-00011fa0: 696c 7920 6d65 616e 2077 696e 6420 7370  ily mean wind sp
-00011fb0: 6565 642e 0a0a 2020 2020 2020 2020 4e6f  eed...        No
-00011fc0: 7465 730a 2020 2020 2020 2020 2d2d 2d2d  tes.        ----
-00011fd0: 2d0a 2020 2020 2020 2020 4966 2073 6663  -.        If sfc
-00011fe0: 5769 6e64 2069 7320 6e6f 7420 7072 6f76  Wind is not prov
-00011ff0: 6964 6564 2069 6e20 6064 7360 2073 6663  ided in `ds` sfc
-00012000: 5769 6e64 2063 6f75 6c64 2062 6520 636f  Wind could be co
-00012010: 6d70 7574 6564 0a20 2020 2020 2020 2066  mputed.        f
-00012020: 726f 6d20 6064 7360 2e75 6173 2061 6e64  rom `ds`.uas and
-00012030: 2060 6473 602e 7661 732e 0a0a 2020 2020   `ds`.vas...    
-00012040: 2020 2020 466f 7220 696e 666f 726d 6174      For informat
-00012050: 696f 6e20 6f6e 2074 6865 2069 6e70 7574  ion on the input
-00012060: 2070 6172 616d 6574 6572 7320 7365 653a   parameters see:
-00012070: 0a20 2020 2020 2020 2020 2020 2068 7474  .            htt
-00012080: 7073 3a2f 2f78 636c 696d 2e72 6561 6474  ps://xclim.readt
-00012090: 6865 646f 6373 2e69 6f2f 656e 2f73 7461  hedocs.io/en/sta
-000120a0: 626c 652f 6170 692e 6874 6d6c 2378 636c  ble/api.html#xcl
-000120b0: 696d 2e69 6e64 6963 6174 6f72 732e 6174  im.indicators.at
-000120c0: 6d6f 732e 7366 6357 696e 645f 6d69 6e0a  mos.sfcWind_min.
-000120d0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-000120e0: 2020 2020 6966 2022 7366 6357 696e 6422      if "sfcWind"
-000120f0: 206e 6f74 2069 6e20 7061 7261 6d73 5b22   not in params["
-00012100: 6473 225d 3a0a 2020 2020 2020 2020 2020  ds"]:.          
-00012110: 2020 7061 7261 6d73 5b22 6473 225d 5b22    params["ds"]["
-00012120: 7366 6357 696e 6422 5d20 3d20 7863 2e61  sfcWind"] = xc.a
-00012130: 746d 6f73 2e77 696e 645f 7370 6565 645f  tmos.wind_speed_
-00012140: 6672 6f6d 5f76 6563 746f 7228 0a20 2020  from_vector(.   
-00012150: 2020 2020 2020 2020 2020 2020 2064 733d               ds=
-00012160: 7061 7261 6d73 5b22 6473 225d 2c0a 2020  params["ds"],.  
-00012170: 2020 2020 2020 2020 2020 295b 305d 0a20            )[0]. 
-00012180: 2020 2020 2020 2072 6574 7572 6e20 7863         return xc
-00012190: 2e61 746d 6f73 2e73 6663 5769 6e64 5f6d  .atmos.sfcWind_m
-000121a0: 696e 282a 2a70 6172 616d 7329 0a0a 0a63  in(**params)...c
-000121b0: 6c61 7373 2046 4778 3a0a 2020 2020 2222  lass FGx:.    ""
-000121c0: 224d 6178 696d 756d 2064 6169 6c79 206d  "Maximum daily m
-000121d0: 6561 6e20 7769 6e64 2073 7065 6564 2e22  ean wind speed."
-000121e0: 2222 0a0a 2020 2020 6465 6620 636f 6d70  ""..    def comp
-000121f0: 7574 6528 2a2a 7061 7261 6d73 293a 0a20  ute(**params):. 
-00012200: 2020 2020 2020 2022 2222 4361 6c63 756c         """Calcul
-00012210: 6174 6520 6d61 7869 6d75 6d20 6461 696c  ate maximum dail
-00012220: 7920 6d65 616e 2077 696e 6420 7370 6565  y mean wind spee
-00012230: 642e 0a0a 2020 2020 2020 2020 5265 7475  d...        Retu
-00012240: 726e 730a 2020 2020 2020 2020 2d2d 2d2d  rns.        ----
-00012250: 2d2d 2d0a 2020 2020 2020 2020 7861 7272  ---.        xarr
-00012260: 6179 2e44 6174 6141 7272 6179 0a20 2020  ay.DataArray.   
-00012270: 2020 2020 2020 2020 204d 6178 696d 756d           Maximum
-00012280: 2064 6169 6c79 206d 6561 6e20 7769 6e64   daily mean wind
-00012290: 2073 7065 6564 2e0a 0a20 2020 2020 2020   speed...       
-000122a0: 204e 6f74 6573 0a20 2020 2020 2020 202d   Notes.        -
-000122b0: 2d2d 2d2d 0a20 2020 2020 2020 2049 6620  ----.        If 
-000122c0: 7366 6357 696e 6420 6973 206e 6f74 2070  sfcWind is not p
-000122d0: 726f 7669 6465 6420 696e 2060 6473 6020  rovided in `ds` 
-000122e0: 7366 6357 696e 6420 636f 756c 6420 6265  sfcWind could be
-000122f0: 2063 6f6d 7075 7465 640a 2020 2020 2020   computed.      
-00012300: 2020 6672 6f6d 2060 6473 602e 7561 7320    from `ds`.uas 
-00012310: 616e 6420 6064 7360 2e76 6173 2e0a 0a20  and `ds`.vas... 
-00012320: 2020 2020 2020 2046 6f72 2069 6e66 6f72         For infor
-00012330: 6d61 7469 6f6e 206f 6e20 7468 6520 696e  mation on the in
-00012340: 7075 7420 7061 7261 6d65 7465 7273 2073  put parameters s
-00012350: 6565 3a0a 2020 2020 2020 2020 2020 2020  ee:.            
-00012360: 6874 7470 733a 2f2f 7863 6c69 6d2e 7265  https://xclim.re
-00012370: 6164 7468 6564 6f63 732e 696f 2f65 6e2f  adthedocs.io/en/
-00012380: 7374 6162 6c65 2f61 7069 2e68 746d 6c23  stable/api.html#
-00012390: 7863 6c69 6d2e 696e 6469 6361 746f 7273  xclim.indicators
-000123a0: 2e61 746d 6f73 2e73 6663 5769 6e64 5f6d  .atmos.sfcWind_m
-000123b0: 6178 0a20 2020 2020 2020 2022 2222 0a20  ax.        """. 
-000123c0: 2020 2020 2020 2069 6620 2273 6663 5769         if "sfcWi
-000123d0: 6e64 2220 6e6f 7420 696e 2070 6172 616d  nd" not in param
-000123e0: 735b 2264 7322 5d3a 0a20 2020 2020 2020  s["ds"]:.       
-000123f0: 2020 2020 2070 6172 616d 735b 2264 7322       params["ds"
-00012400: 5d5b 2273 6663 5769 6e64 225d 203d 2078  ]["sfcWind"] = x
-00012410: 632e 6174 6d6f 732e 7769 6e64 5f73 7065  c.atmos.wind_spe
-00012420: 6564 5f66 726f 6d5f 7665 6374 6f72 280a  ed_from_vector(.
-00012430: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012440: 6473 3d70 6172 616d 735b 2264 7322 5d2c  ds=params["ds"],
-00012450: 0a20 2020 2020 2020 2020 2020 2029 5b30  .            )[0
-00012460: 5d0a 2020 2020 2020 2020 7265 7475 726e  ].        return
-00012470: 2078 632e 6174 6d6f 732e 7366 6357 696e   xc.atmos.sfcWin
-00012480: 645f 6d61 7828 2a2a 7061 7261 6d73 290a  d_max(**params).
-00012490: 0a0a 636c 6173 7320 4658 3a0a 2020 2020  ..class FX:.    
-000124a0: 2222 224d 6561 6e20 6461 696c 7920 6d61  """Mean daily ma
-000124b0: 7869 6d75 6d20 7769 6e64 2073 7065 6564  ximum wind speed
-000124c0: 2e22 2222 0a0a 2020 2020 6465 6620 636f  ."""..    def co
-000124d0: 6d70 7574 6528 2a2a 7061 7261 6d73 293a  mpute(**params):
-000124e0: 0a20 2020 2020 2020 2022 2222 4361 6c63  .        """Calc
-000124f0: 756c 6174 6520 6d65 616e 2064 6169 6c79  ulate mean daily
-00012500: 206d 6178 696d 756d 2077 696e 6420 7370   maximum wind sp
-00012510: 6565 642e 0a0a 2020 2020 2020 2020 5265  eed...        Re
-00012520: 7475 726e 730a 2020 2020 2020 2020 2d2d  turns.        --
-00012530: 2d2d 2d2d 2d0a 2020 2020 2020 2020 7861  -----.        xa
-00012540: 7272 6179 2e44 6174 6141 7272 6179 0a20  rray.DataArray. 
-00012550: 2020 2020 2020 2020 2020 204d 6561 6e20             Mean 
-00012560: 6461 696c 7920 6d61 7869 6d75 6d20 7769  daily maximum wi
-00012570: 6e64 2073 7065 6564 2e0a 0a20 2020 2020  nd speed...     
-00012580: 2020 204e 6f74 6573 0a20 2020 2020 2020     Notes.       
-00012590: 202d 2d2d 2d2d 0a20 2020 2020 2020 2046   -----.        F
-000125a0: 6f72 2069 6e66 6f72 6d61 7469 6f6e 206f  or information o
-000125b0: 6e20 7468 6520 696e 7075 7420 7061 7261  n the input para
-000125c0: 6d65 7465 7273 2073 6565 3a0a 2020 2020  meters see:.    
-000125d0: 2020 2020 2020 2020 6874 7470 733a 2f2f          https://
-000125e0: 7863 6c69 6d2e 7265 6164 7468 6564 6f63  xclim.readthedoc
-000125f0: 732e 696f 2f65 6e2f 7374 6162 6c65 2f61  s.io/en/stable/a
-00012600: 7069 2e68 746d 6c23 7863 6c69 6d2e 696e  pi.html#xclim.in
-00012610: 6469 6361 746f 7273 2e61 746d 6f73 2e73  dicators.atmos.s
-00012620: 6663 5769 6e64 6d61 785f 6d65 616e 0a20  fcWindmax_mean. 
-00012630: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-00012640: 2020 2072 6574 7572 6e20 7863 2e61 746d     return xc.atm
-00012650: 6f73 2e73 6663 5769 6e64 6d61 785f 6d65  os.sfcWindmax_me
-00012660: 616e 282a 2a70 6172 616d 7329 0a0a 0a63  an(**params)...c
-00012670: 6c61 7373 2046 586e 3a0a 2020 2020 2222  lass FXn:.    ""
-00012680: 224d 696e 696d 756d 2064 6169 6c79 206d  "Minimum daily m
-00012690: 6178 696d 756d 2077 696e 6420 7370 6565  aximum wind spee
-000126a0: 642e 2222 220a 0a20 2020 2064 6566 2063  d."""..    def c
-000126b0: 6f6d 7075 7465 282a 2a70 6172 616d 7329  ompute(**params)
-000126c0: 3a0a 2020 2020 2020 2020 2222 2243 616c  :.        """Cal
-000126d0: 6375 6c61 7465 206d 696e 696d 756d 2064  culate minimum d
-000126e0: 6169 6c79 206d 6178 696d 756d 2077 696e  aily maximum win
-000126f0: 6420 7370 6565 642e 0a0a 2020 2020 2020  d speed...      
-00012700: 2020 5265 7475 726e 730a 2020 2020 2020    Returns.      
-00012710: 2020 2d2d 2d2d 2d2d 2d0a 2020 2020 2020    -------.      
-00012720: 2020 7861 7272 6179 2e44 6174 6141 7272    xarray.DataArr
-00012730: 6179 0a20 2020 2020 2020 2020 2020 204d  ay.            M
-00012740: 696e 696d 756d 2064 6169 6c79 206d 6178  inimum daily max
-00012750: 696d 756d 2077 696e 6420 7370 6565 642e  imum wind speed.
-00012760: 0a0a 2020 2020 2020 2020 4e6f 7465 730a  ..        Notes.
-00012770: 2020 2020 2020 2020 2d2d 2d2d 2d0a 2020          -----.  
-00012780: 2020 2020 2020 466f 7220 696e 666f 726d        For inform
-00012790: 6174 696f 6e20 6f6e 2074 6865 2069 6e70  ation on the inp
-000127a0: 7574 2070 6172 616d 6574 6572 7320 7365  ut parameters se
-000127b0: 653a 0a20 2020 2020 2020 2020 2020 2068  e:.            h
-000127c0: 7474 7073 3a2f 2f78 636c 696d 2e72 6561  ttps://xclim.rea
-000127d0: 6474 6865 646f 6373 2e69 6f2f 656e 2f73  dthedocs.io/en/s
-000127e0: 7461 626c 652f 6170 692e 6874 6d6c 2378  table/api.html#x
-000127f0: 636c 696d 2e69 6e64 6963 6174 6f72 732e  clim.indicators.
-00012800: 6174 6d6f 732e 7366 6357 696e 646d 6178  atmos.sfcWindmax
-00012810: 5f6d 696e 0a20 2020 2020 2020 2022 2222  _min.        """
-00012820: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00012830: 7863 2e61 746d 6f73 2e73 6663 5769 6e64  xc.atmos.sfcWind
-00012840: 6d61 785f 6d69 6e28 2a2a 7061 7261 6d73  max_min(**params
-00012850: 290a 0a0a 636c 6173 7320 4658 783a 0a20  )...class FXx:. 
-00012860: 2020 2022 2222 4d61 7869 6d75 6d20 6461     """Maximum da
-00012870: 696c 7920 6d61 7869 6d75 6d20 7769 6e64  ily maximum wind
-00012880: 2073 7065 6564 2e22 2222 0a0a 2020 2020   speed."""..    
-00012890: 6465 6620 636f 6d70 7574 6528 2a2a 7061  def compute(**pa
-000128a0: 7261 6d73 293a 0a20 2020 2020 2020 2022  rams):.        "
-000128b0: 2222 4361 6c63 756c 6174 6520 6d61 7869  ""Calculate maxi
-000128c0: 6d75 6d20 6461 696c 7920 6d61 7869 6d75  mum daily maximu
-000128d0: 6d20 7769 6e64 2073 7065 6564 2e0a 0a20  m wind speed... 
-000128e0: 2020 2020 2020 2052 6574 7572 6e73 0a20         Returns. 
-000128f0: 2020 2020 2020 202d 2d2d 2d2d 2d2d 0a20         -------. 
-00012900: 2020 2020 2020 2078 6172 7261 792e 4461         xarray.Da
-00012910: 7461 4172 7261 790a 2020 2020 2020 2020  taArray.        
-00012920: 2020 2020 4d61 7869 6d75 6d20 6461 696c      Maximum dail
-00012930: 7920 6d61 7869 6d75 6d20 7769 6e64 2073  y maximum wind s
-00012940: 7065 6564 2e0a 0a20 2020 2020 2020 204e  peed...        N
-00012950: 6f74 6573 0a20 2020 2020 2020 202d 2d2d  otes.        ---
-00012960: 2d2d 0a20 2020 2020 2020 2046 6f72 2069  --.        For i
-00012970: 6e66 6f72 6d61 7469 6f6e 206f 6e20 7468  nformation on th
-00012980: 6520 696e 7075 7420 7061 7261 6d65 7465  e input paramete
-00012990: 7273 2073 6565 3a0a 2020 2020 2020 2020  rs see:.        
-000129a0: 2020 2020 6874 7470 733a 2f2f 7863 6c69      https://xcli
-000129b0: 6d2e 7265 6164 7468 6564 6f63 732e 696f  m.readthedocs.io
-000129c0: 2f65 6e2f 7374 6162 6c65 2f61 7069 2e68  /en/stable/api.h
-000129d0: 746d 6c23 7863 6c69 6d2e 696e 6469 6361  tml#xclim.indica
-000129e0: 746f 7273 2e61 746d 6f73 2e73 6663 5769  tors.atmos.sfcWi
-000129f0: 6e64 6d61 785f 6d61 780a 2020 2020 2020  ndmax_max.      
-00012a00: 2020 2222 220a 2020 2020 2020 2020 7265    """.        re
-00012a10: 7475 726e 2078 632e 6174 6d6f 732e 7366  turn xc.atmos.sf
-00012a20: 6357 696e 646d 6178 5f6d 6178 282a 2a70  cWindmax_max(**p
-00012a30: 6172 616d 7329 0a                        arams).
+0000b070: 7469 6d65 5f72 616e 6765 3d62 6173 655f  time_range=base_
+0000b080: 7065 7269 6f64 5f74 696d 655f 7261 6e67  period_time_rang
+0000b090: 652c 0a20 2020 2020 2020 2020 2020 2029  e,.            )
+0000b0a0: 0a20 2020 2020 2020 2077 6974 6820 6461  .        with da
+0000b0b0: 736b 2e63 6f6e 6669 672e 7365 7428 2a2a  sk.config.set(**
+0000b0c0: 7b22 6172 7261 792e 736c 6963 696e 672e  {"array.slicing.
+0000b0d0: 7370 6c69 745f 6c61 7267 655f 6368 756e  split_large_chun
+0000b0e0: 6b73 223a 2046 616c 7365 7d29 3a0a 2020  ks": False}):.  
+0000b0f0: 2020 2020 2020 2020 2020 7265 7475 726e            return
+0000b100: 2078 632e 6174 6d6f 732e 7478 3130 7028   xc.atmos.tx10p(
+0000b110: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000b120: 2074 6173 6d61 785f 7065 723d 7461 736d   tasmax_per=tasm
+0000b130: 6178 5f70 6572 2c0a 2020 2020 2020 2020  ax_per,.        
+0000b140: 2020 2020 2020 2020 2a2a 7061 7261 6d73          **params
+0000b150: 2c0a 2020 2020 2020 2020 2020 2020 290a  ,.            ).
+0000b160: 0a0a 636c 6173 7320 5458 3930 703a 0a20  ..class TX90p:. 
+0000b170: 2020 2022 2222 4672 6163 7469 6f6e 206f     """Fraction o
+0000b180: 6620 6461 7973 2077 6974 6820 6d61 7820  f days with max 
+0000b190: 7465 6d70 6572 6174 7572 6520 3e20 3930  temperature > 90
+0000b1a0: 7468 2070 6572 6365 6e74 696c 6520 2874  th percentile (t
+0000b1b0: 6173 6d61 7829 2e22 2222 0a0a 2020 2020  asmax)."""..    
+0000b1c0: 7461 736d 6178 5f70 6572 203d 204e 6f6e  tasmax_per = Non
+0000b1d0: 650a 2020 2020 6261 7365 5f70 6572 696f  e.    base_perio
+0000b1e0: 645f 7469 6d65 5f72 616e 6765 203d 2042  d_time_range = B
+0000b1f0: 4153 455f 5045 5249 4f44 0a0a 2020 2020  ASE_PERIOD..    
+0000b200: 6465 6620 636f 6d70 7574 6528 0a20 2020  def compute(.   
+0000b210: 2020 2020 2062 6173 655f 7065 7269 6f64       base_period
+0000b220: 5f74 696d 655f 7261 6e67 653d 6261 7365  _time_range=base
+0000b230: 5f70 6572 696f 645f 7469 6d65 5f72 616e  _period_time_ran
+0000b240: 6765 2c0a 2020 2020 2020 2020 7461 736d  ge,.        tasm
+0000b250: 6178 5f70 6572 3d74 6173 6d61 785f 7065  ax_per=tasmax_pe
+0000b260: 722c 0a20 2020 2020 2020 202a 2a70 6172  r,.        **par
+0000b270: 616d 732c 0a20 2020 2029 3a0a 2020 2020  ams,.    ):.    
+0000b280: 2020 2020 2222 2243 616c 6375 6c61 7465      """Calculate
+0000b290: 2066 7261 6374 696f 6e20 6f66 2064 6179   fraction of day
+0000b2a0: 7320 7769 7468 206d 6178 2074 656d 7065  s with max tempe
+0000b2b0: 7261 7475 7265 203e 2039 3074 6820 7065  rature > 90th pe
+0000b2c0: 7263 656e 7469 6c65 2e0a 0a20 2020 2020  rcentile...     
+0000b2d0: 2020 2050 6172 616d 6574 6572 730a 2020     Parameters.  
+0000b2e0: 2020 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d        ----------
+0000b2f0: 0a20 2020 2020 2020 2074 6173 6d61 785f  .        tasmax_
+0000b300: 7065 723a 2078 722e 4461 7461 4172 7261  per: xr.DataArra
+0000b310: 792c 206f 7074 696f 6e61 6c0a 2020 2020  y, optional.    
+0000b320: 2020 2020 2020 2020 4d61 7869 6d75 6d20          Maximum 
+0000b330: 7465 6d70 6572 6174 7572 6520 3930 7468  temperature 90th
+0000b340: 2070 6572 6365 6e74 696c 6520 7265 6665   percentile refe
+0000b350: 7265 6e63 6520 7661 6c75 652e 0a20 2020  rence value..   
+0000b360: 2020 2020 2062 6173 655f 7065 7269 6f64       base_period
+0000b370: 5f74 696d 655f 7261 6e67 653a 206c 6973  _time_range: lis
+0000b380: 740a 2020 2020 2020 2020 2020 2020 4c69  t.            Li
+0000b390: 7374 2077 6974 6820 6c65 6674 2062 6f75  st with left bou
+0000b3a0: 6e64 2069 7320 7374 6172 7420 7965 6172  nd is start year
+0000b3b0: 2073 7472 696e 6720 616e 6420 7269 6768   string and righ
+0000b3c0: 7420 626f 756e 640a 2020 2020 2020 2020  t bound.        
+0000b3d0: 2020 2020 6973 2065 6e64 2079 6561 7220      is end year 
+0000b3e0: 7374 7269 6e67 2066 6f72 2063 616c 6375  string for calcu
+0000b3f0: 6c61 7469 6e67 2060 7461 736d 6178 5f70  lating `tasmax_p
+0000b400: 6572 602e 0a20 2020 2020 2020 2020 2020  er`..           
+0000b410: 2054 6869 7320 7769 6c6c 2062 6520 7573   This will be us
+0000b420: 6564 206f 6e6c 7920 6966 2060 7461 736d  ed only if `tasm
+0000b430: 6178 5f70 6572 6020 6973 204e 6f6e 652e  ax_per` is None.
+0000b440: 0a0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
+0000b450: 730a 2020 2020 2020 2020 2d2d 2d2d 2d2d  s.        ------
+0000b460: 2d0a 2020 2020 2020 2020 7861 7272 6179  -.        xarray
+0000b470: 2e44 6174 6141 7272 6179 0a20 2020 2020  .DataArray.     
+0000b480: 2020 2020 2020 2046 7261 6374 696f 6e20         Fraction 
+0000b490: 6f66 2064 6179 7320 7769 7468 206d 6178  of days with max
+0000b4a0: 696d 756d 2074 656d 7065 7261 7475 7265  imum temperature
+0000b4b0: 203e 2039 3074 6820 7065 7263 656e 7469   > 90th percenti
+0000b4c0: 6c65 222e 0a0a 2020 2020 2020 2020 4e6f  le"...        No
+0000b4d0: 7465 730a 2020 2020 2020 2020 2d2d 2d2d  tes.        ----
+0000b4e0: 2d0a 2020 2020 2020 2020 466f 7220 6d6f  -.        For mo
+0000b4f0: 7265 2069 6e66 6f72 6d61 7469 6f6e 206f  re information o
+0000b500: 6e20 7468 6520 696e 7075 7420 7061 7261  n the input para
+0000b510: 6d65 7465 7273 2073 6565 3a0a 2020 2020  meters see:.    
+0000b520: 2020 2020 2020 2020 6874 7470 733a 2f2f          https://
+0000b530: 7863 6c69 6d2e 7265 6164 7468 6564 6f63  xclim.readthedoc
+0000b540: 732e 696f 2f65 6e2f 7374 6162 6c65 2f61  s.io/en/stable/a
+0000b550: 7069 2e68 746d 6c23 7863 6c69 6d2e 696e  pi.html#xclim.in
+0000b560: 6469 6361 746f 7273 2e61 746d 6f73 2e74  dicators.atmos.t
+0000b570: 7839 3070 0a20 2020 2020 2020 2022 2222  x90p.        """
+0000b580: 0a20 2020 2020 2020 2064 6120 3d20 5f67  .        da = _g
+0000b590: 6574 5f64 6128 7061 7261 6d73 2c20 2274  et_da(params, "t
+0000b5a0: 6173 6d61 7822 290a 2020 2020 2020 2020  asmax").        
+0000b5b0: 6966 2074 6173 6d61 785f 7065 7220 6973  if tasmax_per is
+0000b5c0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+0000b5d0: 2020 2074 6173 6d61 785f 7065 7220 3d20     tasmax_per = 
+0000b5e0: 5f67 6574 5f70 6572 6365 6e74 696c 6528  _get_percentile(
+0000b5f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000b600: 2064 613d 6461 2c0a 2020 2020 2020 2020   da=da,.        
+0000b610: 2020 2020 2020 2020 7065 723d 3930 2c0a          per=90,.
+0000b620: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b630: 6261 7365 5f70 6572 696f 645f 7469 6d65  base_period_time
+0000b640: 5f72 616e 6765 3d62 6173 655f 7065 7269  _range=base_peri
+0000b650: 6f64 5f74 696d 655f 7261 6e67 652c 0a20  od_time_range,. 
+0000b660: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+0000b670: 2020 2020 2077 6974 6820 6461 736b 2e63       with dask.c
+0000b680: 6f6e 6669 672e 7365 7428 2a2a 7b22 6172  onfig.set(**{"ar
+0000b690: 7261 792e 736c 6963 696e 672e 7370 6c69  ray.slicing.spli
+0000b6a0: 745f 6c61 7267 655f 6368 756e 6b73 223a  t_large_chunks":
+0000b6b0: 2046 616c 7365 7d29 3a0a 2020 2020 2020   False}):.      
+0000b6c0: 2020 2020 2020 7265 7475 726e 2078 632e        return xc.
+0000b6d0: 6174 6d6f 732e 7478 3930 7028 0a20 2020  atmos.tx90p(.   
+0000b6e0: 2020 2020 2020 2020 2020 2020 2074 6173               tas
+0000b6f0: 6d61 785f 7065 723d 7461 736d 6178 5f70  max_per=tasmax_p
+0000b700: 6572 2c0a 2020 2020 2020 2020 2020 2020  er,.            
+0000b710: 2020 2020 2a2a 7061 7261 6d73 2c0a 2020      **params,.  
+0000b720: 2020 2020 2020 2020 2020 290a 0a0a 636c            )...cl
+0000b730: 6173 7320 5458 6e3a 0a20 2020 2022 2222  ass TXn:.    """
+0000b740: 4d69 6e69 6d75 6d20 6d61 7869 6d75 6d20  Minimum maximum 
+0000b750: 7465 6d70 6572 6174 7572 6520 2874 6173  temperature (tas
+0000b760: 6d61 7829 2e22 2222 0a0a 2020 2020 6465  max)."""..    de
+0000b770: 6620 636f 6d70 7574 6528 2a2a 7061 7261  f compute(**para
+0000b780: 6d73 293a 0a20 2020 2020 2020 2022 2222  ms):.        """
+0000b790: 4361 6c63 756c 6174 6520 6d69 6e69 6d75  Calculate minimu
+0000b7a0: 6d20 6461 696c 7920 6d61 7869 6d75 6d20  m daily maximum 
+0000b7b0: 7465 6d70 6572 6174 7572 652e 0a0a 2020  temperature...  
+0000b7c0: 2020 2020 2020 5265 7475 726e 730a 2020        Returns.  
+0000b7d0: 2020 2020 2020 2d2d 2d2d 2d2d 2d0a 2020        -------.  
+0000b7e0: 2020 2020 2020 7861 7272 6179 2e44 6174        xarray.Dat
+0000b7f0: 6141 7272 6179 0a20 2020 2020 2020 2020  aArray.         
+0000b800: 2020 204d 696e 696d 756d 2064 6169 6c79     Minimum daily
+0000b810: 206d 6178 696d 756d 2074 656d 7065 7261   maximum tempera
+0000b820: 7475 7265 2e0a 0a20 2020 2020 2020 204e  ture...        N
+0000b830: 6f74 6573 0a20 2020 2020 2020 202d 2d2d  otes.        ---
+0000b840: 2d2d 0a20 2020 2020 2020 2046 6f72 2069  --.        For i
+0000b850: 6e66 6f72 6d61 7469 6f6e 206f 6e20 7468  nformation on th
+0000b860: 6520 696e 7075 7420 7061 7261 6d65 7465  e input paramete
+0000b870: 7273 2073 6565 3a0a 2020 2020 2020 2020  rs see:.        
+0000b880: 2020 2020 6874 7470 733a 2f2f 7863 6c69      https://xcli
+0000b890: 6d2e 7265 6164 7468 6564 6f63 732e 696f  m.readthedocs.io
+0000b8a0: 2f65 6e2f 7374 6162 6c65 2f61 7069 2e68  /en/stable/api.h
+0000b8b0: 746d 6c23 7863 6c69 6d2e 696e 6469 6361  tml#xclim.indica
+0000b8c0: 746f 7273 2e61 746d 6f73 2e74 785f 6d69  tors.atmos.tx_mi
+0000b8d0: 6e0a 2020 2020 2020 2020 2222 220a 2020  n.        """.  
+0000b8e0: 2020 2020 2020 7265 7475 726e 2078 632e        return xc.
+0000b8f0: 6174 6d6f 732e 7478 5f6d 696e 282a 2a70  atmos.tx_min(**p
+0000b900: 6172 616d 7329 0a0a 0a63 6c61 7373 2054  arams)...class T
+0000b910: 5878 3a0a 2020 2020 2222 224d 6178 696d  Xx:.    """Maxim
+0000b920: 756d 206d 6178 696d 756d 2074 656d 7065  um maximum tempe
+0000b930: 7261 7475 7265 2028 7461 736d 6178 292e  rature (tasmax).
+0000b940: 2222 220a 0a20 2020 2064 6566 2063 6f6d  """..    def com
+0000b950: 7075 7465 282a 2a70 6172 616d 7329 3a0a  pute(**params):.
+0000b960: 2020 2020 2020 2020 2222 2243 616c 6375          """Calcu
+0000b970: 6c61 7465 206d 6178 696d 756d 2064 6169  late maximum dai
+0000b980: 6c79 206d 6178 696d 756d 2074 656d 7065  ly maximum tempe
+0000b990: 7261 7475 7265 2e0a 0a20 2020 2020 2020  rature...       
+0000b9a0: 2052 6574 7572 6e73 0a20 2020 2020 2020   Returns.       
+0000b9b0: 202d 2d2d 2d2d 2d2d 0a20 2020 2020 2020   -------.       
+0000b9c0: 2078 6172 7261 792e 4461 7461 4172 7261   xarray.DataArra
+0000b9d0: 790a 2020 2020 2020 2020 2020 2020 4d61  y.            Ma
+0000b9e0: 7869 6d75 6d20 6461 696c 7920 6d61 7869  ximum daily maxi
+0000b9f0: 6d75 6d20 7465 6d70 6572 6174 7572 652e  mum temperature.
+0000ba00: 0a0a 2020 2020 2020 2020 4e6f 7465 730a  ..        Notes.
+0000ba10: 2020 2020 2020 2020 2d2d 2d2d 2d0a 2020          -----.  
+0000ba20: 2020 2020 2020 466f 7220 696e 666f 726d        For inform
+0000ba30: 6174 696f 6e20 6f6e 2074 6865 2069 6e70  ation on the inp
+0000ba40: 7574 2070 6172 616d 6574 6572 7320 7365  ut parameters se
+0000ba50: 653a 0a20 2020 2020 2020 2020 2020 2068  e:.            h
+0000ba60: 7474 7073 3a2f 2f78 636c 696d 2e72 6561  ttps://xclim.rea
+0000ba70: 6474 6865 646f 6373 2e69 6f2f 656e 2f73  dthedocs.io/en/s
+0000ba80: 7461 626c 652f 6170 692e 6874 6d6c 2378  table/api.html#x
+0000ba90: 636c 696d 2e69 6e64 6963 6174 6f72 732e  clim.indicators.
+0000baa0: 6174 6d6f 732e 7478 5f6d 6178 0a20 2020  atmos.tx_max.   
+0000bab0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+0000bac0: 2072 6574 7572 6e20 7863 2e61 746d 6f73   return xc.atmos
+0000bad0: 2e74 785f 6d61 7828 2a2a 7061 7261 6d73  .tx_max(**params
+0000bae0: 290a 0a0a 636c 6173 7320 544e 3a0a 2020  )...class TN:.  
+0000baf0: 2020 2222 224d 6561 6e20 6d69 6e69 6d75    """Mean minimu
+0000bb00: 6d20 7465 6d70 6572 6174 7572 6520 2874  m temperature (t
+0000bb10: 6173 6d69 6e29 2e22 2222 0a0a 2020 2020  asmin)."""..    
+0000bb20: 6465 6620 636f 6d70 7574 6528 2a2a 7061  def compute(**pa
+0000bb30: 7261 6d73 293a 0a20 2020 2020 2020 2022  rams):.        "
+0000bb40: 2222 4361 6c63 756c 6174 6520 6d65 616e  ""Calculate mean
+0000bb50: 2064 6169 6c79 206d 696e 696d 756d 2074   daily minimum t
+0000bb60: 656d 7065 7261 7475 7265 2e0a 0a20 2020  emperature...   
+0000bb70: 2020 2020 2052 6574 7572 6e73 0a20 2020       Returns.   
+0000bb80: 2020 2020 202d 2d2d 2d2d 2d2d 0a20 2020       -------.   
+0000bb90: 2020 2020 2078 6172 7261 792e 4461 7461       xarray.Data
+0000bba0: 4172 7261 790a 2020 2020 2020 2020 2020  Array.          
+0000bbb0: 2020 4d65 616e 2064 6169 6c79 206d 696e    Mean daily min
+0000bbc0: 696d 756d 2074 656d 7065 7261 7475 7265  imum temperature
+0000bbd0: 2e0a 0a20 2020 2020 2020 204e 6f74 6573  ...        Notes
+0000bbe0: 0a20 2020 2020 2020 202d 2d2d 2d2d 0a20  .        -----. 
+0000bbf0: 2020 2020 2020 2046 6f72 2069 6e66 6f72         For infor
+0000bc00: 6d61 7469 6f6e 206f 6e20 7468 6520 696e  mation on the in
+0000bc10: 7075 7420 7061 7261 6d65 7465 7273 2073  put parameters s
+0000bc20: 6565 3a0a 2020 2020 2020 2020 2020 2020  ee:.            
+0000bc30: 6874 7470 733a 2f2f 7863 6c69 6d2e 7265  https://xclim.re
+0000bc40: 6164 7468 6564 6f63 732e 696f 2f65 6e2f  adthedocs.io/en/
+0000bc50: 7374 6162 6c65 2f61 7069 2e68 746d 6c23  stable/api.html#
+0000bc60: 7863 6c69 6d2e 696e 6469 6361 746f 7273  xclim.indicators
+0000bc70: 2e61 746d 6f73 2e74 6e5f 6d65 616e 0a20  .atmos.tn_mean. 
+0000bc80: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+0000bc90: 2020 2072 6574 7572 6e20 7863 2e61 746d     return xc.atm
+0000bca0: 6f73 2e74 6e5f 6d65 616e 282a 2a70 6172  os.tn_mean(**par
+0000bcb0: 616d 7329 0a0a 0a63 6c61 7373 2054 4e31  ams)...class TN1
+0000bcc0: 3070 3a0a 2020 2020 2222 2246 7261 6374  0p:.    """Fract
+0000bcd0: 696f 6e20 6f66 2064 6179 7320 7769 7468  ion of days with
+0000bce0: 206d 696e 2074 656d 7065 7261 7475 7265   min temperature
+0000bcf0: 203c 2031 3074 6820 7065 7263 656e 7469   < 10th percenti
+0000bd00: 6c65 2e22 2222 0a0a 2020 2020 7461 736d  le."""..    tasm
+0000bd10: 696e 5f70 6572 203d 204e 6f6e 650a 2020  in_per = None.  
+0000bd20: 2020 6261 7365 5f70 6572 696f 645f 7469    base_period_ti
+0000bd30: 6d65 5f72 616e 6765 203d 2042 4153 455f  me_range = BASE_
+0000bd40: 5045 5249 4f44 0a0a 2020 2020 6465 6620  PERIOD..    def 
+0000bd50: 636f 6d70 7574 6528 0a20 2020 2020 2020  compute(.       
+0000bd60: 2062 6173 655f 7065 7269 6f64 5f74 696d   base_period_tim
+0000bd70: 655f 7261 6e67 653d 6261 7365 5f70 6572  e_range=base_per
+0000bd80: 696f 645f 7469 6d65 5f72 616e 6765 2c0a  iod_time_range,.
+0000bd90: 2020 2020 2020 2020 7461 736d 696e 5f70          tasmin_p
+0000bda0: 6572 3d74 6173 6d69 6e5f 7065 722c 0a20  er=tasmin_per,. 
+0000bdb0: 2020 2020 2020 202a 2a70 6172 616d 732c         **params,
+0000bdc0: 0a20 2020 2029 3a0a 2020 2020 2020 2020  .    ):.        
+0000bdd0: 2222 2243 616c 6375 6c61 7465 2066 7261  """Calculate fra
+0000bde0: 6374 696f 6e20 6f66 2064 6179 7320 7769  ction of days wi
+0000bdf0: 7468 206d 696e 2074 656d 7065 7261 7475  th min temperatu
+0000be00: 7265 203c 2031 3074 6820 7065 7263 656e  re < 10th percen
+0000be10: 7469 6c65 2e0a 0a20 2020 2020 2020 2050  tile...        P
+0000be20: 6172 616d 6574 6572 730a 2020 2020 2020  arameters.      
+0000be30: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020    ----------.   
+0000be40: 2020 2020 2074 6173 6d69 6e5f 7065 723a       tasmin_per:
+0000be50: 2078 722e 4461 7461 4172 7261 792c 206f   xr.DataArray, o
+0000be60: 7074 696f 6e61 6c0a 2020 2020 2020 2020  ptional.        
+0000be70: 2020 2020 4d69 6e69 6d75 6d20 7465 6d70      Minimum temp
+0000be80: 6572 6174 7572 6520 3130 7468 2070 6572  erature 10th per
+0000be90: 6365 6e74 696c 6520 7265 6665 7265 6e63  centile referenc
+0000bea0: 6520 7661 6c75 652e 0a20 2020 2020 2020  e value..       
+0000beb0: 2062 6173 655f 7065 7269 6f64 5f74 696d   base_period_tim
+0000bec0: 655f 7261 6e67 653a 206c 6973 740a 2020  e_range: list.  
+0000bed0: 2020 2020 2020 2020 2020 4c69 7374 2077            List w
+0000bee0: 6974 6820 6c65 6674 2062 6f75 6e64 2069  ith left bound i
+0000bef0: 7320 7374 6172 7420 7965 6172 2073 7472  s start year str
+0000bf00: 696e 6720 616e 6420 7269 6768 7420 626f  ing and right bo
+0000bf10: 756e 640a 2020 2020 2020 2020 2020 2020  und.            
+0000bf20: 6973 2065 6e64 2079 6561 7220 7374 7269  is end year stri
+0000bf30: 6e67 2066 6f72 2063 616c 6375 6c61 7469  ng for calculati
+0000bf40: 6e67 2060 7461 736d 696e 5f70 6572 602e  ng `tasmin_per`.
+0000bf50: 0a20 2020 2020 2020 2020 2020 2054 6869  .            Thi
+0000bf60: 7320 7769 6c6c 2062 6520 7573 6564 206f  s will be used o
+0000bf70: 6e6c 7920 6966 2060 7461 736d 696e 5f70  nly if `tasmin_p
+0000bf80: 6572 6020 6973 204e 6f6e 652e 0a0a 2020  er` is None...  
+0000bf90: 2020 2020 2020 5265 7475 726e 730a 2020        Returns.  
+0000bfa0: 2020 2020 2020 2d2d 2d2d 2d2d 2d0a 2020        -------.  
+0000bfb0: 2020 2020 2020 7861 7272 6179 2e44 6174        xarray.Dat
+0000bfc0: 6141 7272 6179 0a20 2020 2020 2020 2020  aArray.         
+0000bfd0: 2020 2046 7261 6374 696f 6e20 6f66 2064     Fraction of d
+0000bfe0: 6179 7320 7769 7468 206d 696e 696d 756d  ays with minimum
+0000bff0: 2074 656d 7065 7261 7475 7265 203c 2031   temperature < 1
+0000c000: 3074 6820 7065 7263 656e 7469 6c65 222e  0th percentile".
+0000c010: 0a0a 2020 2020 2020 2020 4e6f 7465 730a  ..        Notes.
+0000c020: 2020 2020 2020 2020 2d2d 2d2d 2d0a 2020          -----.  
+0000c030: 2020 2020 2020 466f 7220 6d6f 7265 2069        For more i
+0000c040: 6e66 6f72 6d61 7469 6f6e 206f 6e20 7468  nformation on th
+0000c050: 6520 696e 7075 7420 7061 7261 6d65 7465  e input paramete
+0000c060: 7273 2073 6565 3a0a 2020 2020 2020 2020  rs see:.        
+0000c070: 2020 2020 6874 7470 733a 2f2f 7863 6c69      https://xcli
+0000c080: 6d2e 7265 6164 7468 6564 6f63 732e 696f  m.readthedocs.io
+0000c090: 2f65 6e2f 7374 6162 6c65 2f61 7069 2e68  /en/stable/api.h
+0000c0a0: 746d 6c23 7863 6c69 6d2e 696e 6469 6361  tml#xclim.indica
+0000c0b0: 746f 7273 2e61 746d 6f73 2e74 6e31 3070  tors.atmos.tn10p
+0000c0c0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+0000c0d0: 2020 2020 2064 6120 3d20 5f67 6574 5f64       da = _get_d
+0000c0e0: 6128 7061 7261 6d73 2c20 2274 6173 6d69  a(params, "tasmi
+0000c0f0: 6e22 290a 2020 2020 2020 2020 6966 2074  n").        if t
+0000c100: 6173 6d69 6e5f 7065 7220 6973 204e 6f6e  asmin_per is Non
+0000c110: 653a 0a20 2020 2020 2020 2020 2020 2074  e:.            t
+0000c120: 6173 6d69 6e5f 7065 7220 3d20 5f67 6574  asmin_per = _get
+0000c130: 5f70 6572 6365 6e74 696c 6528 0a20 2020  _percentile(.   
+0000c140: 2020 2020 2020 2020 2020 2020 2064 613d               da=
+0000c150: 6461 2c0a 2020 2020 2020 2020 2020 2020  da,.            
+0000c160: 2020 2020 7065 723d 3130 2c0a 2020 2020      per=10,.    
+0000c170: 2020 2020 2020 2020 2020 2020 6261 7365              base
+0000c180: 5f70 6572 696f 645f 7469 6d65 5f72 616e  _period_time_ran
+0000c190: 6765 3d62 6173 655f 7065 7269 6f64 5f74  ge=base_period_t
+0000c1a0: 696d 655f 7261 6e67 652c 0a20 2020 2020  ime_range,.     
+0000c1b0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+0000c1c0: 2077 6974 6820 6461 736b 2e63 6f6e 6669   with dask.confi
+0000c1d0: 672e 7365 7428 2a2a 7b22 6172 7261 792e  g.set(**{"array.
+0000c1e0: 736c 6963 696e 672e 7370 6c69 745f 6c61  slicing.split_la
+0000c1f0: 7267 655f 6368 756e 6b73 223a 2046 616c  rge_chunks": Fal
+0000c200: 7365 7d29 3a0a 2020 2020 2020 2020 2020  se}):.          
+0000c210: 2020 7265 7475 726e 2078 632e 6174 6d6f    return xc.atmo
+0000c220: 732e 746e 3130 7028 0a20 2020 2020 2020  s.tn10p(.       
+0000c230: 2020 2020 2020 2020 2074 6173 6d69 6e5f           tasmin_
+0000c240: 7065 723d 7461 736d 696e 5f70 6572 2c0a  per=tasmin_per,.
+0000c250: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c260: 2a2a 7061 7261 6d73 2c0a 2020 2020 2020  **params,.      
+0000c270: 2020 2020 2020 290a 0a0a 636c 6173 7320        )...class 
+0000c280: 544e 3930 703a 0a20 2020 2022 2222 4672  TN90p:.    """Fr
+0000c290: 6163 7469 6f6e 206f 6620 6461 7973 2077  action of days w
+0000c2a0: 6974 6820 6d69 6e20 7465 6d70 6572 6174  ith min temperat
+0000c2b0: 7572 6520 3e20 3930 7468 2070 6572 6365  ure > 90th perce
+0000c2c0: 6e74 696c 652e 2222 220a 0a20 2020 2074  ntile."""..    t
+0000c2d0: 6173 6d69 6e5f 7065 7220 3d20 4e6f 6e65  asmin_per = None
+0000c2e0: 0a20 2020 2062 6173 655f 7065 7269 6f64  .    base_period
+0000c2f0: 5f74 696d 655f 7261 6e67 6520 3d20 4241  _time_range = BA
+0000c300: 5345 5f50 4552 494f 440a 0a20 2020 2064  SE_PERIOD..    d
+0000c310: 6566 2063 6f6d 7075 7465 280a 2020 2020  ef compute(.    
+0000c320: 2020 2020 6261 7365 5f70 6572 696f 645f      base_period_
+0000c330: 7469 6d65 5f72 616e 6765 3d62 6173 655f  time_range=base_
+0000c340: 7065 7269 6f64 5f74 696d 655f 7261 6e67  period_time_rang
+0000c350: 652c 0a20 2020 2020 2020 2074 6173 6d69  e,.        tasmi
+0000c360: 6e5f 7065 723d 7461 736d 696e 5f70 6572  n_per=tasmin_per
+0000c370: 2c0a 2020 2020 2020 2020 2a2a 7061 7261  ,.        **para
+0000c380: 6d73 2c0a 2020 2020 293a 0a20 2020 2020  ms,.    ):.     
+0000c390: 2020 2022 2222 4361 6c63 756c 6174 6520     """Calculate 
+0000c3a0: 6672 6163 7469 6f6e 206f 6620 6461 7973  fraction of days
+0000c3b0: 2077 6974 6820 6d69 6e20 7465 6d70 6572   with min temper
+0000c3c0: 6174 7572 6520 3e20 3930 7468 2070 6572  ature > 90th per
+0000c3d0: 6365 6e74 696c 652e 0a0a 2020 2020 2020  centile...      
+0000c3e0: 2020 5061 7261 6d65 7465 7273 0a20 2020    Parameters.   
+0000c3f0: 2020 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a       ----------.
+0000c400: 2020 2020 2020 2020 7461 736d 696e 5f70          tasmin_p
+0000c410: 6572 3a20 7872 2e44 6174 6141 7272 6179  er: xr.DataArray
+0000c420: 2c20 6f70 7469 6f6e 616c 0a20 2020 2020  , optional.     
+0000c430: 2020 2020 2020 204d 696e 696d 756d 2074         Minimum t
+0000c440: 656d 7065 7261 7475 7265 2039 3074 6820  emperature 90th 
+0000c450: 7065 7263 656e 7469 6c65 2072 6566 6572  percentile refer
+0000c460: 656e 6365 2076 616c 7565 2e0a 2020 2020  ence value..    
+0000c470: 2020 2020 6261 7365 5f70 6572 696f 645f      base_period_
+0000c480: 7469 6d65 5f72 616e 6765 3a20 6c69 7374  time_range: list
+0000c490: 0a20 2020 2020 2020 2020 2020 204c 6973  .            Lis
+0000c4a0: 7420 7769 7468 206c 6566 7420 626f 756e  t with left boun
+0000c4b0: 6420 6973 2073 7461 7274 2079 6561 7220  d is start year 
+0000c4c0: 7374 7269 6e67 2061 6e64 2072 6967 6874  string and right
+0000c4d0: 2062 6f75 6e64 0a20 2020 2020 2020 2020   bound.         
+0000c4e0: 2020 2069 7320 656e 6420 7965 6172 2073     is end year s
+0000c4f0: 7472 696e 6720 666f 7220 6361 6c63 756c  tring for calcul
+0000c500: 6174 696e 6720 6074 6173 6d69 6e5f 7065  ating `tasmin_pe
+0000c510: 7260 2e0a 2020 2020 2020 2020 2020 2020  r`..            
+0000c520: 5468 6973 2077 696c 6c20 6265 2075 7365  This will be use
+0000c530: 6420 6f6e 6c79 2069 6620 6074 6173 6d69  d only if `tasmi
+0000c540: 6e5f 7065 7260 2069 7320 4e6f 6e65 2e0a  n_per` is None..
+0000c550: 0a20 2020 2020 2020 2052 6574 7572 6e73  .        Returns
+0000c560: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
+0000c570: 0a20 2020 2020 2020 2078 6172 7261 792e  .        xarray.
+0000c580: 4461 7461 4172 7261 790a 2020 2020 2020  DataArray.      
+0000c590: 2020 2020 2020 4672 6163 7469 6f6e 206f        Fraction o
+0000c5a0: 6620 6461 7973 2077 6974 6820 6d69 6e69  f days with mini
+0000c5b0: 6d75 6d20 7465 6d70 6572 6174 7572 6520  mum temperature 
+0000c5c0: 3e20 3930 7468 2070 6572 6365 6e74 696c  > 90th percentil
+0000c5d0: 6522 2e0a 0a20 2020 2020 2020 204e 6f74  e"...        Not
+0000c5e0: 6573 0a20 2020 2020 2020 202d 2d2d 2d2d  es.        -----
+0000c5f0: 0a20 2020 2020 2020 2046 6f72 206d 6f72  .        For mor
+0000c600: 6520 696e 666f 726d 6174 696f 6e20 6f6e  e information on
+0000c610: 2074 6865 2069 6e70 7574 2070 6172 616d   the input param
+0000c620: 6574 6572 7320 7365 653a 0a20 2020 2020  eters see:.     
+0000c630: 2020 2020 2020 2068 7474 7073 3a2f 2f78         https://x
+0000c640: 636c 696d 2e72 6561 6474 6865 646f 6373  clim.readthedocs
+0000c650: 2e69 6f2f 656e 2f73 7461 626c 652f 6170  .io/en/stable/ap
+0000c660: 692e 6874 6d6c 2378 636c 696d 2e69 6e64  i.html#xclim.ind
+0000c670: 6963 6174 6f72 732e 6174 6d6f 732e 7478  icators.atmos.tx
+0000c680: 3930 700a 2020 2020 2020 2020 2222 220a  90p.        """.
+0000c690: 2020 2020 2020 2020 6461 203d 205f 6765          da = _ge
+0000c6a0: 745f 6461 2870 6172 616d 732c 2022 7461  t_da(params, "ta
+0000c6b0: 736d 696e 2229 0a20 2020 2020 2020 2069  smin").        i
+0000c6c0: 6620 7461 736d 696e 5f70 6572 2069 7320  f tasmin_per is 
+0000c6d0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+0000c6e0: 2020 7461 736d 696e 5f70 6572 203d 205f    tasmin_per = _
+0000c6f0: 6765 745f 7065 7263 656e 7469 6c65 280a  get_percentile(.
+0000c700: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c710: 6461 3d64 612c 0a20 2020 2020 2020 2020  da=da,.         
+0000c720: 2020 2020 2020 2070 6572 3d39 302c 0a20         per=90,. 
+0000c730: 2020 2020 2020 2020 2020 2020 2020 2062                 b
+0000c740: 6173 655f 7065 7269 6f64 5f74 696d 655f  ase_period_time_
+0000c750: 7261 6e67 653d 6261 7365 5f70 6572 696f  range=base_perio
+0000c760: 645f 7469 6d65 5f72 616e 6765 2c0a 2020  d_time_range,.  
+0000c770: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
+0000c780: 2020 2020 7769 7468 2064 6173 6b2e 636f      with dask.co
+0000c790: 6e66 6967 2e73 6574 282a 2a7b 2261 7272  nfig.set(**{"arr
+0000c7a0: 6179 2e73 6c69 6369 6e67 2e73 706c 6974  ay.slicing.split
+0000c7b0: 5f6c 6172 6765 5f63 6875 6e6b 7322 3a20  _large_chunks": 
+0000c7c0: 4661 6c73 657d 293a 0a20 2020 2020 2020  False}):.       
+0000c7d0: 2020 2020 2072 6574 7572 6e20 7863 2e61       return xc.a
+0000c7e0: 746d 6f73 2e74 6e39 3070 280a 2020 2020  tmos.tn90p(.    
+0000c7f0: 2020 2020 2020 2020 2020 2020 7461 736d              tasm
+0000c800: 696e 5f70 6572 3d74 6173 6d69 6e5f 7065  in_per=tasmin_pe
+0000c810: 722c 0a20 2020 2020 2020 2020 2020 2020  r,.             
+0000c820: 2020 202a 2a70 6172 616d 732c 0a20 2020     **params,.   
+0000c830: 2020 2020 2020 2020 2029 0a0a 0a63 6c61           )...cla
+0000c840: 7373 2054 4e6e 3a0a 2020 2020 2222 224d  ss TNn:.    """M
+0000c850: 696e 696d 756d 206d 696e 696d 756d 2074  inimum minimum t
+0000c860: 656d 7065 7261 7475 7265 2028 7461 736d  emperature (tasm
+0000c870: 696e 292e 2222 220a 0a20 2020 2064 6566  in)."""..    def
+0000c880: 2063 6f6d 7075 7465 282a 2a70 6172 616d   compute(**param
+0000c890: 7329 3a0a 2020 2020 2020 2020 2222 2243  s):.        """C
+0000c8a0: 616c 6375 6c61 7465 206d 696e 696d 756d  alculate minimum
+0000c8b0: 2064 6169 6c79 206d 696e 696d 756d 2074   daily minimum t
+0000c8c0: 656d 7065 7261 7475 7265 2e0a 0a20 2020  emperature...   
+0000c8d0: 2020 2020 2052 6574 7572 6e73 0a20 2020       Returns.   
+0000c8e0: 2020 2020 202d 2d2d 2d2d 2d2d 0a20 2020       -------.   
+0000c8f0: 2020 2020 2078 6172 7261 792e 4461 7461       xarray.Data
+0000c900: 4172 7261 790a 2020 2020 2020 2020 2020  Array.          
+0000c910: 2020 4d69 6e69 6d75 6d20 6461 696c 7920    Minimum daily 
+0000c920: 6d69 6e69 6d75 6d20 7465 6d70 6572 6174  minimum temperat
+0000c930: 7572 652e 0a0a 2020 2020 2020 2020 4e6f  ure...        No
+0000c940: 7465 730a 2020 2020 2020 2020 2d2d 2d2d  tes.        ----
+0000c950: 2d0a 2020 2020 2020 2020 466f 7220 696e  -.        For in
+0000c960: 666f 726d 6174 696f 6e20 6f6e 2074 6865  formation on the
+0000c970: 2069 6e70 7574 2070 6172 616d 6574 6572   input parameter
+0000c980: 7320 7365 653a 0a20 2020 2020 2020 2020  s see:.         
+0000c990: 2020 2068 7474 7073 3a2f 2f78 636c 696d     https://xclim
+0000c9a0: 2e72 6561 6474 6865 646f 6373 2e69 6f2f  .readthedocs.io/
+0000c9b0: 656e 2f73 7461 626c 652f 6170 692e 6874  en/stable/api.ht
+0000c9c0: 6d6c 2378 636c 696d 2e69 6e64 6963 6174  ml#xclim.indicat
+0000c9d0: 6f72 732e 6174 6d6f 732e 746e 5f6d 696e  ors.atmos.tn_min
+0000c9e0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+0000c9f0: 2020 2020 2072 6574 7572 6e20 7863 2e61       return xc.a
+0000ca00: 746d 6f73 2e74 6e5f 6d69 6e28 2a2a 7061  tmos.tn_min(**pa
+0000ca10: 7261 6d73 290a 0a0a 636c 6173 7320 544e  rams)...class TN
+0000ca20: 783a 0a20 2020 2022 2222 4d61 7869 6d75  x:.    """Maximu
+0000ca30: 6d20 6d69 6e69 6d75 6d20 7465 6d70 6572  m minimum temper
+0000ca40: 6174 7572 6520 2874 6173 6d69 6e29 2e22  ature (tasmin)."
+0000ca50: 2222 0a0a 2020 2020 6465 6620 636f 6d70  ""..    def comp
+0000ca60: 7574 6528 2a2a 7061 7261 6d73 293a 0a20  ute(**params):. 
+0000ca70: 2020 2020 2020 2022 2222 4361 6c63 756c         """Calcul
+0000ca80: 6174 6520 6d61 7869 6d75 6d20 6461 696c  ate maximum dail
+0000ca90: 7920 6d69 6e69 6d75 6d20 7465 6d70 6572  y minimum temper
+0000caa0: 6174 7572 652e 0a0a 2020 2020 2020 2020  ature...        
+0000cab0: 5265 7475 726e 730a 2020 2020 2020 2020  Returns.        
+0000cac0: 2d2d 2d2d 2d2d 2d0a 2020 2020 2020 2020  -------.        
+0000cad0: 7861 7272 6179 2e44 6174 6141 7272 6179  xarray.DataArray
+0000cae0: 0a20 2020 2020 2020 2020 2020 204d 6178  .            Max
+0000caf0: 696d 756d 2064 6169 6c79 206d 696e 696d  imum daily minim
+0000cb00: 756d 2074 656d 7065 7261 7475 7265 2e0a  um temperature..
+0000cb10: 0a20 2020 2020 2020 204e 6f74 6573 0a20  .        Notes. 
+0000cb20: 2020 2020 2020 202d 2d2d 2d2d 0a20 2020         -----.   
+0000cb30: 2020 2020 2046 6f72 2069 6e66 6f72 6d61       For informa
+0000cb40: 7469 6f6e 206f 6e20 7468 6520 696e 7075  tion on the inpu
+0000cb50: 7420 7061 7261 6d65 7465 7273 2073 6565  t parameters see
+0000cb60: 3a0a 2020 2020 2020 2020 2020 2020 6874  :.            ht
+0000cb70: 7470 733a 2f2f 7863 6c69 6d2e 7265 6164  tps://xclim.read
+0000cb80: 7468 6564 6f63 732e 696f 2f65 6e2f 7374  thedocs.io/en/st
+0000cb90: 6162 6c65 2f61 7069 2e68 746d 6c23 7863  able/api.html#xc
+0000cba0: 6c69 6d2e 696e 6469 6361 746f 7273 2e61  lim.indicators.a
+0000cbb0: 746d 6f73 2e74 6e5f 6d61 780a 2020 2020  tmos.tn_max.    
+0000cbc0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+0000cbd0: 7265 7475 726e 2078 632e 6174 6d6f 732e  return xc.atmos.
+0000cbe0: 746e 5f6d 6178 282a 2a70 6172 616d 7329  tn_max(**params)
+0000cbf0: 0a0a 0a63 6c61 7373 2057 443a 0a20 2020  ...class WD:.   
+0000cc00: 2022 2222 4e75 6d62 6572 206f 6620 7761   """Number of wa
+0000cc10: 726d 2061 6e64 2064 7279 2064 6179 7320  rm and dry days 
+0000cc20: 2874 6173 2c20 7072 292e 2222 220a 0a20  (tas, pr).""".. 
+0000cc30: 2020 2074 6173 5f70 6572 203d 204e 6f6e     tas_per = Non
+0000cc40: 650a 2020 2020 7072 5f70 6572 203d 204e  e.    pr_per = N
+0000cc50: 6f6e 650a 2020 2020 6261 7365 5f70 6572  one.    base_per
+0000cc60: 696f 645f 7469 6d65 5f72 616e 6765 203d  iod_time_range =
+0000cc70: 2042 4153 455f 5045 5249 4f44 0a0a 2020   BASE_PERIOD..  
+0000cc80: 2020 6465 6620 636f 6d70 7574 6528 0a20    def compute(. 
+0000cc90: 2020 2020 2020 2062 6173 655f 7065 7269         base_peri
+0000cca0: 6f64 5f74 696d 655f 7261 6e67 653d 6261  od_time_range=ba
+0000ccb0: 7365 5f70 6572 696f 645f 7469 6d65 5f72  se_period_time_r
+0000ccc0: 616e 6765 2c0a 2020 2020 2020 2020 7461  ange,.        ta
+0000ccd0: 735f 7065 723d 7461 735f 7065 722c 0a20  s_per=tas_per,. 
+0000cce0: 2020 2020 2020 2070 725f 7065 723d 7072         pr_per=pr
+0000ccf0: 5f70 6572 2c0a 2020 2020 2020 2020 2a2a  _per,.        **
+0000cd00: 7061 7261 6d73 2c0a 2020 2020 293a 0a20  params,.    ):. 
+0000cd10: 2020 2020 2020 2022 2222 4361 6c63 756c         """Calcul
+0000cd20: 6174 6520 6e75 6d62 6572 206f 6620 7761  ate number of wa
+0000cd30: 726d 2061 6e64 2064 7279 2064 6179 732e  rm and dry days.
+0000cd40: 0a0a 2020 2020 2020 2020 5061 7261 6d65  ..        Parame
+0000cd50: 7465 7273 0a20 2020 2020 2020 202d 2d2d  ters.        ---
+0000cd60: 2d2d 2d2d 2d2d 2d0a 2020 2020 2020 2020  -------.        
+0000cd70: 7461 735f 7065 723a 2078 722e 4461 7461  tas_per: xr.Data
+0000cd80: 4172 7261 792c 206f 7074 696f 6e61 6c0a  Array, optional.
+0000cd90: 2020 2020 2020 2020 2020 2020 4d65 616e              Mean
+0000cda0: 2074 656d 7065 7261 7475 7265 2037 3574   temperature 75t
+0000cdb0: 6820 7065 7263 656e 7469 6c65 2072 6566  h percentile ref
+0000cdc0: 6572 656e 6365 2076 616c 7565 2061 626f  erence value abo
+0000cdd0: 7665 2077 6869 6368 0a20 2020 2020 2020  ve which.       
+0000cde0: 2020 2020 2061 2064 6179 2069 7320 636f       a day is co
+0000cdf0: 6e73 6964 6572 6564 2061 7320 6120 7761  nsidered as a wa
+0000ce00: 726d 2064 6179 2e0a 2020 2020 2020 2020  rm day..        
+0000ce10: 7072 5f70 6572 3a20 7872 2e44 6174 6141  pr_per: xr.DataA
+0000ce20: 7272 6179 2c20 6f70 7469 6f6e 616c 0a20  rray, optional. 
+0000ce30: 2020 2020 2020 2020 2020 2050 7265 6369             Preci
+0000ce40: 7069 7461 7469 6f6e 2032 3574 6820 7065  pitation 25th pe
+0000ce50: 7263 656e 7469 6c65 2072 6566 6572 656e  rcentile referen
+0000ce60: 6365 2076 616c 7565 2062 656c 6f77 2077  ce value below w
+0000ce70: 6869 6368 0a20 2020 2020 2020 2020 2020  hich.           
+0000ce80: 2061 2064 6179 2069 7320 636f 6e73 6964   a day is consid
+0000ce90: 6572 6564 2061 7320 6120 6472 7920 6461  ered as a dry da
+0000cea0: 792e 0a20 2020 2020 2020 2062 6173 655f  y..        base_
+0000ceb0: 7065 7269 6f64 5f74 696d 655f 7261 6e67  period_time_rang
+0000cec0: 653a 206c 6973 740a 2020 2020 2020 2020  e: list.        
+0000ced0: 2020 2020 4c69 7374 2077 6974 6820 6c65      List with le
+0000cee0: 6674 2062 6f75 6e64 2069 7320 7374 6172  ft bound is star
+0000cef0: 7420 7965 6172 2073 7472 696e 6720 616e  t year string an
+0000cf00: 6420 7269 6768 7420 626f 756e 640a 2020  d right bound.  
+0000cf10: 2020 2020 2020 2020 2020 6973 2065 6e64            is end
+0000cf20: 2079 6561 7220 7374 7269 6e67 2066 6f72   year string for
+0000cf30: 2063 616c 6375 6c61 7469 6e67 2060 7461   calculating `ta
+0000cf40: 735f 7065 7260 2061 6e64 2f6f 7220 6070  s_per` and/or `p
+0000cf50: 725f 7065 7260 2e0a 2020 2020 2020 2020  r_per`..        
+0000cf60: 2020 2020 5468 6973 2077 696c 6c20 6265      This will be
+0000cf70: 2075 7365 6420 6f6e 6c79 2069 6620 6074   used only if `t
+0000cf80: 6173 5f70 6572 6020 616e 642f 6f72 2060  as_per` and/or `
+0000cf90: 7072 5f70 6572 6020 6973 204e 6f6e 652e  pr_per` is None.
+0000cfa0: 0a0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
+0000cfb0: 730a 2020 2020 2020 2020 2d2d 2d2d 2d2d  s.        ------
+0000cfc0: 2d0a 2020 2020 2020 2020 7861 7272 6179  -.        xarray
+0000cfd0: 2e44 6174 6141 7272 6179 3a0a 2020 2020  .DataArray:.    
+0000cfe0: 2020 2020 2020 2020 4e75 6d62 6572 206f          Number o
+0000cff0: 6620 6461 7973 2077 6865 7265 2077 6172  f days where war
+0000d000: 6d20 616e 6420 6472 7920 636f 6e64 6974  m and dry condit
+0000d010: 696f 6e73 2063 6f69 6e63 6964 652e 0a20  ions coincide.. 
+0000d020: 2020 2020 2020 2020 2020 2049 6620 7465             If te
+0000d030: 6d70 6572 6174 7572 6520 6973 2061 626f  mperature is abo
+0000d040: 7665 207b 7461 735f 7065 727d 2061 2064  ve {tas_per} a d
+0000d050: 6179 2069 7320 636f 6e73 6964 6572 6564  ay is considered
+0000d060: 2061 7320 610a 2020 2020 2020 2020 2020   as a.          
+0000d070: 2020 7761 726d 2064 6179 2e0a 2020 2020    warm day..    
+0000d080: 2020 2020 2020 2020 4966 2070 7265 6369          If preci
+0000d090: 7069 7461 7469 6f6e 2069 7320 6265 6c6f  pitation is belo
+0000d0a0: 7720 7b70 725f 7065 727d 2061 2064 6179  w {pr_per} a day
+0000d0b0: 2069 7320 636f 6e73 6964 6572 6564 2061   is considered a
+0000d0c0: 7320 610a 2020 2020 2020 2020 2020 2020  s a.            
+0000d0d0: 6472 7920 6461 792e 0a0a 2020 2020 2020  dry day...      
+0000d0e0: 2020 4e6f 7465 730a 2020 2020 2020 2020    Notes.        
+0000d0f0: 2d2d 2d2d 2d0a 2020 2020 2020 2020 466f  -----.        Fo
+0000d100: 7220 6d6f 7265 2069 6e66 6f72 6d61 7469  r more informati
+0000d110: 6f6e 206f 6e20 7468 6520 696e 7075 7420  on on the input 
+0000d120: 7061 7261 6d65 7465 7273 2073 6565 3a0a  parameters see:.
+0000d130: 2020 2020 2020 2020 2020 2020 6874 7470              http
+0000d140: 733a 2f2f 7863 6c69 6d2e 7265 6164 7468  s://xclim.readth
+0000d150: 6564 6f63 732e 696f 2f65 6e2f 7374 6162  edocs.io/en/stab
+0000d160: 6c65 2f61 7069 2e68 746d 6c23 7863 6c69  le/api.html#xcli
+0000d170: 6d2e 696e 6469 6361 746f 7273 2e61 746d  m.indicators.atm
+0000d180: 6f73 2e77 6172 6d5f 616e 645f 6472 795f  os.warm_and_dry_
+0000d190: 6461 7973 0a20 2020 2020 2020 2022 2222  days.        """
+0000d1a0: 0a20 2020 2020 2020 2064 615f 7461 7320  .        da_tas 
+0000d1b0: 3d20 5f67 6574 5f64 6128 7061 7261 6d73  = _get_da(params
+0000d1c0: 2c20 2274 6173 2229 0a20 2020 2020 2020  , "tas").       
+0000d1d0: 2064 615f 7072 203d 205f 6765 745f 6461   da_pr = _get_da
+0000d1e0: 2870 6172 616d 732c 2022 7072 2229 0a20  (params, "pr"). 
+0000d1f0: 2020 2020 2020 2069 6620 7461 735f 7065         if tas_pe
+0000d200: 7220 6973 204e 6f6e 653a 0a20 2020 2020  r is None:.     
+0000d210: 2020 2020 2020 2074 6173 5f70 6572 203d         tas_per =
+0000d220: 205f 6765 745f 7065 7263 656e 7469 6c65   _get_percentile
+0000d230: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+0000d240: 2020 6461 3d64 615f 7461 732c 0a20 2020    da=da_tas,.   
+0000d250: 2020 2020 2020 2020 2020 2020 2070 6572               per
+0000d260: 3d37 352c 0a20 2020 2020 2020 2020 2020  =75,.           
+0000d270: 2020 2020 2062 6173 655f 7065 7269 6f64       base_period
+0000d280: 5f74 696d 655f 7261 6e67 653d 6261 7365  _time_range=base
+0000d290: 5f70 6572 696f 645f 7469 6d65 5f72 616e  _period_time_ran
+0000d2a0: 6765 2c0a 2020 2020 2020 2020 2020 2020  ge,.            
+0000d2b0: 290a 2020 2020 2020 2020 6966 2070 725f  ).        if pr_
+0000d2c0: 7065 7220 6973 204e 6f6e 653a 0a20 2020  per is None:.   
+0000d2d0: 2020 2020 2020 2020 2064 615f 7072 5f66           da_pr_f
+0000d2e0: 203d 205f 6669 6c74 6572 5f6f 7574 5f73   = _filter_out_s
+0000d2f0: 6d61 6c6c 5f76 616c 7565 7328 0a20 2020  mall_values(.   
+0000d300: 2020 2020 2020 2020 2020 2020 2064 615f               da_
+0000d310: 7072 2c0a 2020 2020 2020 2020 2020 2020  pr,.            
+0000d320: 2020 2020 2231 206d 6d2f 6461 7922 2c0a      "1 mm/day",.
+0000d330: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d340: 636f 6e74 6578 743d 2268 7964 726f 222c  context="hydro",
+0000d350: 0a20 2020 2020 2020 2020 2020 2029 0a20  .            ). 
+0000d360: 2020 2020 2020 2020 2020 2070 725f 7065             pr_pe
+0000d370: 7220 3d20 5f67 6574 5f70 6572 6365 6e74  r = _get_percent
+0000d380: 696c 6528 0a20 2020 2020 2020 2020 2020  ile(.           
+0000d390: 2020 2020 2064 613d 6461 5f70 725f 662c       da=da_pr_f,
+0000d3a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000d3b0: 2070 6572 3d32 352c 0a20 2020 2020 2020   per=25,.       
+0000d3c0: 2020 2020 2020 2020 2062 6173 655f 7065           base_pe
+0000d3d0: 7269 6f64 5f74 696d 655f 7261 6e67 653d  riod_time_range=
+0000d3e0: 6261 7365 5f70 6572 696f 645f 7469 6d65  base_period_time
+0000d3f0: 5f72 616e 6765 2c0a 2020 2020 2020 2020  _range,.        
+0000d400: 2020 2020 290a 2020 2020 2020 2020 7769      ).        wi
+0000d410: 7468 2064 6173 6b2e 636f 6e66 6967 2e73  th dask.config.s
+0000d420: 6574 282a 2a7b 2261 7272 6179 2e73 6c69  et(**{"array.sli
+0000d430: 6369 6e67 2e73 706c 6974 5f6c 6172 6765  cing.split_large
+0000d440: 5f63 6875 6e6b 7322 3a20 4661 6c73 657d  _chunks": False}
+0000d450: 293a 0a20 2020 2020 2020 2020 2020 2072  ):.            r
+0000d460: 6574 7572 6e20 7863 2e61 746d 6f73 2e77  eturn xc.atmos.w
+0000d470: 6172 6d5f 616e 645f 6472 795f 6461 7973  arm_and_dry_days
+0000d480: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+0000d490: 2020 7461 735f 7065 723d 7461 735f 7065    tas_per=tas_pe
+0000d4a0: 722c 0a20 2020 2020 2020 2020 2020 2020  r,.             
+0000d4b0: 2020 2070 725f 7065 723d 7072 5f70 6572     pr_per=pr_per
+0000d4c0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0000d4d0: 2020 2a2a 7061 7261 6d73 2c0a 2020 2020    **params,.    
+0000d4e0: 2020 2020 2020 2020 290a 0a0a 636c 6173          )...clas
+0000d4f0: 7320 5753 4449 3a0a 2020 2020 2222 2257  s WSDI:.    """W
+0000d500: 6172 6d20 7370 656c 6c20 6475 7261 7469  arm spell durati
+0000d510: 6f6e 2069 6e64 6578 2028 7461 736d 6178  on index (tasmax
+0000d520: 292e 2222 220a 0a20 2020 2077 696e 646f  )."""..    windo
+0000d530: 7720 3d20 360a 2020 2020 7461 736d 6178  w = 6.    tasmax
+0000d540: 5f70 6572 203d 204e 6f6e 650a 2020 2020  _per = None.    
+0000d550: 6261 7365 5f70 6572 696f 645f 7469 6d65  base_period_time
+0000d560: 5f72 616e 6765 203d 2042 4153 455f 5045  _range = BASE_PE
+0000d570: 5249 4f44 0a0a 2020 2020 6465 6620 636f  RIOD..    def co
+0000d580: 6d70 7574 6528 0a20 2020 2020 2020 2077  mpute(.        w
+0000d590: 696e 646f 773d 7769 6e64 6f77 2c0a 2020  indow=window,.  
+0000d5a0: 2020 2020 2020 6261 7365 5f70 6572 696f        base_perio
+0000d5b0: 645f 7469 6d65 5f72 616e 6765 3d62 6173  d_time_range=bas
+0000d5c0: 655f 7065 7269 6f64 5f74 696d 655f 7261  e_period_time_ra
+0000d5d0: 6e67 652c 0a20 2020 2020 2020 2074 6173  nge,.        tas
+0000d5e0: 6d61 785f 7065 723d 7461 736d 6178 5f70  max_per=tasmax_p
+0000d5f0: 6572 2c0a 2020 2020 2020 2020 2a2a 7061  er,.        **pa
+0000d600: 7261 6d73 2c0a 2020 2020 293a 0a20 2020  rams,.    ):.   
+0000d610: 2020 2020 2022 2222 4361 6c63 756c 6174       """Calculat
+0000d620: 6520 7761 726d 2073 7065 6c6c 2064 7572  e warm spell dur
+0000d630: 6174 696f 6e20 696e 6465 782e 0a0a 2020  ation index...  
+0000d640: 2020 2020 2020 5061 7261 6d65 7465 7273        Parameters
+0000d650: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
+0000d660: 2d2d 2d0a 2020 2020 2020 2020 7769 6e64  ---.        wind
+0000d670: 6f77 3a20 696e 740a 2020 2020 2020 2020  ow: int.        
+0000d680: 2020 2020 4d69 6e69 6d75 6d20 6e75 6d62      Minimum numb
+0000d690: 6572 206f 6620 6461 7973 2077 6974 6820  er of days with 
+0000d6a0: 7465 6d70 6572 6174 7572 6520 6162 6f76  temperature abov
+0000d6b0: 6520 6074 6173 6d61 785f 7065 7260 0a20  e `tasmax_per`. 
+0000d6c0: 2020 2020 2020 2020 2020 2074 6f20 7175             to qu
+0000d6d0: 616c 6966 7920 6173 2061 2077 6172 6d20  alify as a warm 
+0000d6e0: 7370 656c 6c20 2864 6566 6175 6c74 3a20  spell (default: 
+0000d6f0: 3629 2e0a 2020 2020 2020 2020 7461 736d  6)..        tasm
+0000d700: 696e 5f70 6572 3a20 7872 2e44 6174 6141  in_per: xr.DataA
+0000d710: 7272 6179 2c20 6f70 7469 6f6e 616c 0a20  rray, optional. 
+0000d720: 2020 2020 2020 2020 2020 204d 6178 696d             Maxim
+0000d730: 756d 2074 656d 7065 7261 7475 7265 2039  um temperature 9
+0000d740: 3074 6820 7065 7263 656e 7469 6c65 2072  0th percentile r
+0000d750: 6566 6572 656e 6365 2076 616c 7565 2e0a  eference value..
+0000d760: 2020 2020 2020 2020 6261 7365 5f70 6572          base_per
+0000d770: 696f 645f 7469 6d65 5f72 616e 6765 3a20  iod_time_range: 
+0000d780: 6c69 7374 0a20 2020 2020 2020 2020 2020  list.           
+0000d790: 204c 6973 7420 7769 7468 206c 6566 7420   List with left 
+0000d7a0: 626f 756e 6420 6973 2073 7461 7274 2079  bound is start y
+0000d7b0: 6561 7220 7374 7269 6e67 2061 6e64 2072  ear string and r
+0000d7c0: 6967 6874 2062 6f75 6e64 0a20 2020 2020  ight bound.     
+0000d7d0: 2020 2020 2020 2069 7320 656e 6420 7965         is end ye
+0000d7e0: 6172 2073 7472 696e 6720 666f 7220 6361  ar string for ca
+0000d7f0: 6c63 756c 6174 696e 6720 6074 6173 6d61  lculating `tasma
+0000d800: 785f 7065 7260 2e0a 2020 2020 2020 2020  x_per`..        
+0000d810: 2020 2020 5468 6973 2077 696c 6c20 6265      This will be
+0000d820: 2075 7365 6420 6f6e 6c79 2069 6620 6074   used only if `t
+0000d830: 6173 6d61 785f 7065 7260 2069 7320 4e6f  asmax_per` is No
+0000d840: 6e65 2e0a 0a20 2020 2020 2020 2052 6574  ne...        Ret
+0000d850: 7572 6e73 0a20 2020 2020 2020 202d 2d2d  urns.        ---
+0000d860: 2d2d 2d2d 0a20 2020 2020 2020 2078 6172  ----.        xar
+0000d870: 7261 792e 4461 7461 4172 7261 790a 2020  ray.DataArray.  
+0000d880: 2020 2020 2020 2020 2020 4e75 6d62 6572            Number
+0000d890: 206f 6620 6461 7973 2070 6172 7420 6f66   of days part of
+0000d8a0: 2061 2039 3074 6820 7065 7263 656e 7469   a 90th percenti
+0000d8b0: 6c65 2077 6172 6d20 7370 656c 6c2e 0a20  le warm spell.. 
+0000d8c0: 2020 2020 2020 2020 2020 2041 7420 6c65             At le
+0000d8d0: 6173 7420 7b77 696e 646f 777d 2063 6f6e  ast {window} con
+0000d8e0: 7365 6375 7469 7665 2064 6179 732e 0a0a  secutive days...
+0000d8f0: 2020 2020 2020 2020 4e6f 7465 730a 2020          Notes.  
+0000d900: 2020 2020 2020 2d2d 2d2d 2d0a 2020 2020        -----.    
+0000d910: 2020 2020 466f 7220 6d6f 7265 2069 6e66      For more inf
+0000d920: 6f72 6d61 7469 6f6e 206f 6e20 7468 6520  ormation on the 
+0000d930: 696e 7075 7420 7061 7261 6d65 7465 7273  input parameters
+0000d940: 2073 6565 3a0a 2020 2020 2020 2020 2020   see:.          
+0000d950: 2020 6874 7470 733a 2f2f 7863 6c69 6d2e    https://xclim.
+0000d960: 7265 6164 7468 6564 6f63 732e 696f 2f65  readthedocs.io/e
+0000d970: 6e2f 7374 6162 6c65 2f61 7069 2e68 746d  n/stable/api.htm
+0000d980: 6c23 7863 6c69 6d2e 696e 6469 6361 746f  l#xclim.indicato
+0000d990: 7273 2e61 746d 6f73 2e77 6172 6d5f 7370  rs.atmos.warm_sp
+0000d9a0: 656c 6c5f 6475 7261 7469 6f6e 5f69 6e64  ell_duration_ind
+0000d9b0: 6578 0a20 2020 2020 2020 2022 2222 0a20  ex.        """. 
+0000d9c0: 2020 2020 2020 2064 6120 3d20 5f67 6574         da = _get
+0000d9d0: 5f64 6128 7061 7261 6d73 2c20 2274 6173  _da(params, "tas
+0000d9e0: 6d61 7822 290a 2020 2020 2020 2020 6966  max").        if
+0000d9f0: 2074 6173 6d61 785f 7065 7220 6973 204e   tasmax_per is N
+0000da00: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+0000da10: 2074 6173 6d61 785f 7065 7220 3d20 5f67   tasmax_per = _g
+0000da20: 6574 5f70 6572 6365 6e74 696c 6528 0a20  et_percentile(. 
+0000da30: 2020 2020 2020 2020 2020 2020 2020 2064                 d
+0000da40: 613d 6461 2c0a 2020 2020 2020 2020 2020  a=da,.          
+0000da50: 2020 2020 2020 7065 723d 3930 2c0a 2020        per=90,.  
+0000da60: 2020 2020 2020 2020 2020 2020 2020 6261                ba
+0000da70: 7365 5f70 6572 696f 645f 7469 6d65 5f72  se_period_time_r
+0000da80: 616e 6765 3d62 6173 655f 7065 7269 6f64  ange=base_period
+0000da90: 5f74 696d 655f 7261 6e67 652c 0a20 2020  _time_range,.   
+0000daa0: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
+0000dab0: 2020 2077 6974 6820 6461 736b 2e63 6f6e     with dask.con
+0000dac0: 6669 672e 7365 7428 2a2a 7b22 6172 7261  fig.set(**{"arra
+0000dad0: 792e 736c 6963 696e 672e 7370 6c69 745f  y.slicing.split_
+0000dae0: 6c61 7267 655f 6368 756e 6b73 223a 2046  large_chunks": F
+0000daf0: 616c 7365 7d29 3a0a 2020 2020 2020 2020  alse}):.        
+0000db00: 2020 2020 7265 7475 726e 2078 632e 6174      return xc.at
+0000db10: 6d6f 732e 7761 726d 5f73 7065 6c6c 5f64  mos.warm_spell_d
+0000db20: 7572 6174 696f 6e5f 696e 6465 7828 0a20  uration_index(. 
+0000db30: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+0000db40: 6173 6d61 785f 7065 723d 7461 736d 6178  asmax_per=tasmax
+0000db50: 5f70 6572 2c0a 2020 2020 2020 2020 2020  _per,.          
+0000db60: 2020 2020 2020 7769 6e64 6f77 3d77 696e        window=win
+0000db70: 646f 772c 0a20 2020 2020 2020 2020 2020  dow,.           
+0000db80: 2020 2020 202a 2a70 6172 616d 732c 0a20       **params,. 
+0000db90: 2020 2020 2020 2020 2020 2029 0a0a 0a63             )...c
+0000dba0: 6c61 7373 2057 573a 0a20 2020 2022 2222  lass WW:.    """
+0000dbb0: 4e75 6d62 6572 206f 6620 7761 726d 2061  Number of warm a
+0000dbc0: 6e64 2077 6574 2064 6179 7320 2874 6173  nd wet days (tas
+0000dbd0: 2c20 7072 292e 2222 220a 0a20 2020 2074  , pr)."""..    t
+0000dbe0: 6173 5f70 6572 203d 204e 6f6e 650a 2020  as_per = None.  
+0000dbf0: 2020 7072 5f70 6572 203d 204e 6f6e 650a    pr_per = None.
+0000dc00: 2020 2020 6261 7365 5f70 6572 696f 645f      base_period_
+0000dc10: 7469 6d65 5f72 616e 6765 203d 2042 4153  time_range = BAS
+0000dc20: 455f 5045 5249 4f44 0a0a 2020 2020 6465  E_PERIOD..    de
+0000dc30: 6620 636f 6d70 7574 6528 0a20 2020 2020  f compute(.     
+0000dc40: 2020 2062 6173 655f 7065 7269 6f64 5f74     base_period_t
+0000dc50: 696d 655f 7261 6e67 653d 6261 7365 5f70  ime_range=base_p
+0000dc60: 6572 696f 645f 7469 6d65 5f72 616e 6765  eriod_time_range
+0000dc70: 2c0a 2020 2020 2020 2020 7461 735f 7065  ,.        tas_pe
+0000dc80: 723d 7461 735f 7065 722c 0a20 2020 2020  r=tas_per,.     
+0000dc90: 2020 2070 725f 7065 723d 7072 5f70 6572     pr_per=pr_per
+0000dca0: 2c0a 2020 2020 2020 2020 2a2a 7061 7261  ,.        **para
+0000dcb0: 6d73 2c0a 2020 2020 293a 0a20 2020 2020  ms,.    ):.     
+0000dcc0: 2020 2022 2222 4361 6c63 756c 6174 6520     """Calculate 
+0000dcd0: 6e75 6d62 6572 206f 6620 7761 726d 2061  number of warm a
+0000dce0: 6e64 2077 6574 2064 6179 732e 0a0a 2020  nd wet days...  
+0000dcf0: 2020 2020 2020 5061 7261 6d65 7465 7273        Parameters
+0000dd00: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
+0000dd10: 2d2d 2d0a 2020 2020 2020 2020 7461 735f  ---.        tas_
+0000dd20: 7065 723a 2078 722e 4461 7461 4172 7261  per: xr.DataArra
+0000dd30: 792c 206f 7074 696f 6e61 6c0a 2020 2020  y, optional.    
+0000dd40: 2020 2020 2020 2020 4d65 616e 2074 656d          Mean tem
+0000dd50: 7065 7261 7475 7265 2037 3574 6820 7065  perature 75th pe
+0000dd60: 7263 656e 7469 6c65 2072 6566 6572 656e  rcentile referen
+0000dd70: 6365 2076 616c 7565 2061 626f 7665 2077  ce value above w
+0000dd80: 6869 6368 0a20 2020 2020 2020 2020 2020  hich.           
+0000dd90: 2061 2064 6179 2069 7320 636f 6e73 6964   a day is consid
+0000dda0: 6572 6564 2061 7320 6120 7761 726d 2064  ered as a warm d
+0000ddb0: 6179 2e0a 2020 2020 2020 2020 7072 5f70  ay..        pr_p
+0000ddc0: 6572 3a20 7872 2e44 6174 6141 7272 6179  er: xr.DataArray
+0000ddd0: 2c20 6f70 7469 6f6e 616c 0a20 2020 2020  , optional.     
+0000dde0: 2020 2020 2020 2050 7265 6369 7069 7461         Precipita
+0000ddf0: 7469 6f6e 2037 3574 6820 7065 7263 656e  tion 75th percen
+0000de00: 7469 6c65 2072 6566 6572 656e 6365 2076  tile reference v
+0000de10: 616c 7565 2061 626f 7665 2077 6869 6368  alue above which
+0000de20: 0a20 2020 2020 2020 2020 2020 2061 2064  .            a d
+0000de30: 6179 2069 7320 636f 6e73 6964 6572 6564  ay is considered
+0000de40: 2061 7320 6120 7765 7420 6461 792e 0a20   as a wet day.. 
+0000de50: 2020 2020 2020 2062 6173 655f 7065 7269         base_peri
+0000de60: 6f64 5f74 696d 655f 7261 6e67 653a 206c  od_time_range: l
+0000de70: 6973 740a 2020 2020 2020 2020 2020 2020  ist.            
+0000de80: 4c69 7374 2077 6974 6820 6c65 6674 2062  List with left b
+0000de90: 6f75 6e64 2069 7320 7374 6172 7420 7965  ound is start ye
+0000dea0: 6172 2073 7472 696e 6720 616e 6420 7269  ar string and ri
+0000deb0: 6768 7420 626f 756e 640a 2020 2020 2020  ght bound.      
+0000dec0: 2020 2020 2020 6973 2065 6e64 2079 6561        is end yea
+0000ded0: 7220 7374 7269 6e67 2066 6f72 2063 616c  r string for cal
+0000dee0: 6375 6c61 7469 6e67 2060 7461 735f 7065  culating `tas_pe
+0000def0: 7260 2061 6e64 2f6f 7220 6070 725f 7065  r` and/or `pr_pe
+0000df00: 7260 2e0a 2020 2020 2020 2020 2020 2020  r`..            
+0000df10: 5468 6973 2077 696c 6c20 6265 2075 7365  This will be use
+0000df20: 6420 6f6e 6c79 2069 6620 6074 6173 5f70  d only if `tas_p
+0000df30: 6572 6020 616e 642f 6f72 2060 7072 5f70  er` and/or `pr_p
+0000df40: 6572 6020 6973 204e 6f6e 652e 0a0a 2020  er` is None...  
+0000df50: 2020 2020 2020 5265 7475 726e 730a 2020        Returns.  
+0000df60: 2020 2020 2020 2d2d 2d2d 2d2d 2d0a 2020        -------.  
+0000df70: 2020 2020 2020 7861 7272 6179 2e44 6174        xarray.Dat
+0000df80: 6141 7272 6179 3a0a 2020 2020 2020 2020  aArray:.        
+0000df90: 2020 2020 4e75 6d62 6572 206f 6620 6461      Number of da
+0000dfa0: 7973 2077 6865 7265 2077 6172 6d20 616e  ys where warm an
+0000dfb0: 6420 7765 7420 636f 6e64 6974 696f 6e73  d wet conditions
+0000dfc0: 2063 6f69 6e63 6964 652e 0a20 2020 2020   coincide..     
+0000dfd0: 2020 2020 2020 2049 6620 7465 6d70 6572         If temper
+0000dfe0: 6174 7572 6520 6973 2061 626f 7665 207b  ature is above {
+0000dff0: 7461 735f 7065 727d 2061 2064 6179 2069  tas_per} a day i
+0000e000: 7320 636f 6e73 6964 6572 6564 2061 7320  s considered as 
+0000e010: 610a 2020 2020 2020 2020 2020 2020 7761  a.            wa
+0000e020: 726d 2064 6179 2e0a 2020 2020 2020 2020  rm day..        
+0000e030: 2020 2020 4966 2070 7265 6369 7069 7461      If precipita
+0000e040: 7469 6f6e 2069 7320 6162 6f76 6520 7b70  tion is above {p
+0000e050: 725f 7065 727d 2061 2064 6179 2069 7320  r_per} a day is 
+0000e060: 636f 6e73 6964 6572 6564 2061 7320 610a  considered as a.
+0000e070: 2020 2020 2020 2020 2020 2020 7765 7420              wet 
+0000e080: 6461 792e 0a0a 2020 2020 2020 2020 4e6f  day...        No
+0000e090: 7465 730a 2020 2020 2020 2020 2d2d 2d2d  tes.        ----
+0000e0a0: 2d0a 2020 2020 2020 2020 466f 7220 6d6f  -.        For mo
+0000e0b0: 7265 2069 6e66 6f72 6d61 7469 6f6e 206f  re information o
+0000e0c0: 6e20 7468 6520 696e 7075 7420 7061 7261  n the input para
+0000e0d0: 6d65 7465 7273 2073 6565 3a0a 2020 2020  meters see:.    
+0000e0e0: 2020 2020 2020 2020 6874 7470 733a 2f2f          https://
+0000e0f0: 7863 6c69 6d2e 7265 6164 7468 6564 6f63  xclim.readthedoc
+0000e100: 732e 696f 2f65 6e2f 7374 6162 6c65 2f61  s.io/en/stable/a
+0000e110: 7069 2e68 746d 6c23 7863 6c69 6d2e 696e  pi.html#xclim.in
+0000e120: 6469 6361 746f 7273 2e61 746d 6f73 2e77  dicators.atmos.w
+0000e130: 6172 6d5f 616e 645f 7765 745f 6461 7973  arm_and_wet_days
+0000e140: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+0000e150: 2020 2020 2064 615f 7461 7320 3d20 5f67       da_tas = _g
+0000e160: 6574 5f64 6128 7061 7261 6d73 2c20 2274  et_da(params, "t
+0000e170: 6173 2229 0a20 2020 2020 2020 2064 615f  as").        da_
+0000e180: 7072 203d 205f 6765 745f 6461 2870 6172  pr = _get_da(par
+0000e190: 616d 732c 2022 7072 2229 0a20 2020 2020  ams, "pr").     
+0000e1a0: 2020 2069 6620 7461 735f 7065 7220 6973     if tas_per is
+0000e1b0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+0000e1c0: 2020 2074 6173 5f70 6572 203d 205f 6765     tas_per = _ge
+0000e1d0: 745f 7065 7263 656e 7469 6c65 280a 2020  t_percentile(.  
+0000e1e0: 2020 2020 2020 2020 2020 2020 2020 6461                da
+0000e1f0: 3d64 615f 7461 732c 0a20 2020 2020 2020  =da_tas,.       
+0000e200: 2020 2020 2020 2020 2070 6572 3d37 352c           per=75,
+0000e210: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000e220: 2062 6173 655f 7065 7269 6f64 5f74 696d   base_period_tim
+0000e230: 655f 7261 6e67 653d 6261 7365 5f70 6572  e_range=base_per
+0000e240: 696f 645f 7469 6d65 5f72 616e 6765 2c0a  iod_time_range,.
+0000e250: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
+0000e260: 2020 2020 2020 6966 2070 725f 7065 7220        if pr_per 
+0000e270: 6973 204e 6f6e 653a 0a20 2020 2020 2020  is None:.       
+0000e280: 2020 2020 2064 615f 7072 5f66 203d 205f       da_pr_f = _
+0000e290: 6669 6c74 6572 5f6f 7574 5f73 6d61 6c6c  filter_out_small
+0000e2a0: 5f76 616c 7565 7328 0a20 2020 2020 2020  _values(.       
+0000e2b0: 2020 2020 2020 2020 2064 615f 7072 2c0a           da_pr,.
+0000e2c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e2d0: 2231 206d 6d2f 6461 7922 2c0a 2020 2020  "1 mm/day",.    
+0000e2e0: 2020 2020 2020 2020 2020 2020 636f 6e74              cont
+0000e2f0: 6578 743d 2268 7964 726f 222c 0a20 2020  ext="hydro",.   
+0000e300: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
+0000e310: 2020 2020 2020 2070 725f 7065 7220 3d20         pr_per = 
+0000e320: 5f67 6574 5f70 6572 6365 6e74 696c 6528  _get_percentile(
+0000e330: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000e340: 2064 613d 6461 5f70 725f 662c 0a20 2020   da=da_pr_f,.   
+0000e350: 2020 2020 2020 2020 2020 2020 2070 6572               per
+0000e360: 3d37 352c 0a20 2020 2020 2020 2020 2020  =75,.           
+0000e370: 2020 2020 2062 6173 655f 7065 7269 6f64       base_period
+0000e380: 5f74 696d 655f 7261 6e67 653d 6261 7365  _time_range=base
+0000e390: 5f70 6572 696f 645f 7469 6d65 5f72 616e  _period_time_ran
+0000e3a0: 6765 2c0a 2020 2020 2020 2020 2020 2020  ge,.            
+0000e3b0: 290a 2020 2020 2020 2020 7769 7468 2064  ).        with d
+0000e3c0: 6173 6b2e 636f 6e66 6967 2e73 6574 282a  ask.config.set(*
+0000e3d0: 2a7b 2261 7272 6179 2e73 6c69 6369 6e67  *{"array.slicing
+0000e3e0: 2e73 706c 6974 5f6c 6172 6765 5f63 6875  .split_large_chu
+0000e3f0: 6e6b 7322 3a20 4661 6c73 657d 293a 0a20  nks": False}):. 
+0000e400: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+0000e410: 6e20 7863 2e61 746d 6f73 2e77 6172 6d5f  n xc.atmos.warm_
+0000e420: 616e 645f 7765 745f 6461 7973 280a 2020  and_wet_days(.  
+0000e430: 2020 2020 2020 2020 2020 2020 2020 7461                ta
+0000e440: 735f 7065 723d 7461 735f 7065 722c 0a20  s_per=tas_per,. 
+0000e450: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+0000e460: 725f 7065 723d 7072 5f70 6572 2c0a 2020  r_per=pr_per,.  
+0000e470: 2020 2020 2020 2020 2020 2020 2020 2a2a                **
+0000e480: 7061 7261 6d73 2c0a 2020 2020 2020 2020  params,.        
+0000e490: 2020 2020 290a 0a0a 636c 6173 7320 4353      )...class CS
+0000e4a0: 663a 0a20 2020 2022 2222 4e75 6d62 6572  f:.    """Number
+0000e4b0: 206f 6620 636f 6c64 2073 7065 6c6c 7320   of cold spells 
+0000e4c0: 2874 6173 292e 2222 220a 0a20 2020 2074  (tas)."""..    t
+0000e4d0: 6872 6573 6820 3d20 2d31 300a 2020 2020  hresh = -10.    
+0000e4e0: 7769 6e64 6f77 203d 2033 0a0a 2020 2020  window = 3..    
+0000e4f0: 6465 6620 636f 6d70 7574 6528 7468 7265  def compute(thre
+0000e500: 7368 3d74 6872 6573 682c 2077 696e 646f  sh=thresh, windo
+0000e510: 773d 7769 6e64 6f77 2c20 2a2a 7061 7261  w=window, **para
+0000e520: 6d73 293a 0a20 2020 2020 2020 2022 2222  ms):.        """
+0000e530: 4361 6c63 756c 6174 6520 6e75 6d62 6572  Calculate number
+0000e540: 206f 6620 636f 6c64 2073 7065 6c6c 732e   of cold spells.
+0000e550: 0a0a 2020 2020 2020 2020 5061 7261 6d65  ..        Parame
+0000e560: 7465 7273 0a20 2020 2020 2020 202d 2d2d  ters.        ---
+0000e570: 2d2d 2d2d 2d2d 2d0a 2020 2020 2020 2020  -------.        
+0000e580: 7468 7265 7368 3a20 696e 7420 6f72 2073  thresh: int or s
+0000e590: 7472 696e 670a 2020 2020 2020 2020 2020  tring.          
+0000e5a0: 2020 5468 7265 7368 6f6c 6420 7465 6d70    Threshold temp
+0000e5b0: 6572 6174 7572 6520 6265 6c6f 7720 7768  erature below wh
+0000e5c0: 6963 6820 6120 6461 7920 6973 2063 6f6e  ich a day is con
+0000e5d0: 7369 6465 7265 640a 2020 2020 2020 2020  sidered.        
+0000e5e0: 2020 2020 6173 2061 2063 6f6c 6420 6461      as a cold da
+0000e5f0: 7920 2864 6566 6175 6c74 3a20 2d31 3020  y (default: -10 
+0000e600: 6465 6743 292e 0a20 2020 2020 2020 2020  degC)..         
+0000e610: 2020 2049 6620 7479 7065 206f 6620 7468     If type of th
+0000e620: 7265 7368 6f6c 6420 6973 2061 6e20 696e  reshold is an in
+0000e630: 7465 6765 7220 7468 6520 756e 6974 2069  teger the unit i
+0000e640: 7320 7365 7420 746f 2064 6567 432e 0a20  s set to degC.. 
+0000e650: 2020 2020 2020 2077 696e 646f 773a 2069         window: i
+0000e660: 6e74 0a20 2020 2020 2020 2020 2020 204d  nt.            M
+0000e670: 696e 696d 756d 206e 756d 6265 7220 6f66  inimum number of
+0000e680: 2064 6179 7320 7769 7468 2074 656d 7065   days with tempe
+0000e690: 7261 7475 7265 2062 656c 6f77 2074 6872  rature below thr
+0000e6a0: 6573 680a 2020 2020 2020 2020 2020 2020  esh.            
+0000e6b0: 746f 2071 7561 6c69 6679 2061 7320 6120  to qualify as a 
+0000e6c0: 636f 6c64 2073 7065 6c6c 2028 6465 6661  cold spell (defa
+0000e6d0: 756c 743a 2033 292e 0a0a 2020 2020 2020  ult: 3)...      
+0000e6e0: 2020 5265 7475 726e 730a 2020 2020 2020    Returns.      
+0000e6f0: 2020 2d2d 2d2d 2d2d 2d0a 2020 2020 2020    -------.      
+0000e700: 2020 7861 7272 6179 2e44 6174 6141 7272    xarray.DataArr
+0000e710: 6179 0a20 2020 2020 2020 2020 2020 204e  ay.            N
+0000e720: 756d 6265 7220 6f66 2063 6f6c 6420 7370  umber of cold sp
+0000e730: 656c 6c73 206f 6620 6174 206c 6561 7374  ells of at least
+0000e740: 207b 7769 6e64 6f77 7d20 636f 6e73 6563   {window} consec
+0000e750: 7574 6976 6520 6461 7973 0a20 2020 2020  utive days.     
+0000e760: 2020 2020 2020 2077 6974 6820 7465 6d70         with temp
+0000e770: 6572 6174 7572 6520 6265 6c6f 7720 7b74  erature below {t
+0000e780: 6872 6573 687d 2e0a 0a20 2020 2020 2020  hresh}...       
+0000e790: 204e 6f74 6573 0a20 2020 2020 2020 202d   Notes.        -
+0000e7a0: 2d2d 2d2d 0a20 2020 2020 2020 2046 6f72  ----.        For
+0000e7b0: 206d 6f72 6520 696e 666f 726d 6174 696f   more informatio
+0000e7c0: 6e20 6f6e 2074 6865 2069 6e70 7574 2070  n on the input p
+0000e7d0: 6172 616d 6574 6572 7320 7365 653a 0a20  arameters see:. 
+0000e7e0: 2020 2020 2020 2020 2020 2068 7474 7073             https
+0000e7f0: 3a2f 2f78 636c 696d 2e72 6561 6474 6865  ://xclim.readthe
+0000e800: 646f 6373 2e69 6f2f 656e 2f73 7461 626c  docs.io/en/stabl
+0000e810: 652f 6170 692e 6874 6d6c 2378 636c 696d  e/api.html#xclim
+0000e820: 2e69 6e64 6963 6174 6f72 732e 6174 6d6f  .indicators.atmo
+0000e830: 732e 636f 6c64 5f73 7065 6c6c 5f66 7265  s.cold_spell_fre
+0000e840: 7175 656e 6379 0a20 2020 2020 2020 2022  quency.        "
+0000e850: 2222 0a20 2020 2020 2020 2074 6872 6573  "".        thres
+0000e860: 6820 3d20 5f74 6872 6573 685f 7374 7269  h = _thresh_stri
+0000e870: 6e67 2874 6872 6573 682c 2022 6465 6743  ng(thresh, "degC
+0000e880: 2229 0a20 2020 2020 2020 2072 6574 7572  ").        retur
+0000e890: 6e20 7863 2e61 746d 6f73 2e63 6f6c 645f  n xc.atmos.cold_
+0000e8a0: 7370 656c 6c5f 6672 6571 7565 6e63 7928  spell_frequency(
+0000e8b0: 0a20 2020 2020 2020 2020 2020 2074 6872  .            thr
+0000e8c0: 6573 683d 7468 7265 7368 2c0a 2020 2020  esh=thresh,.    
+0000e8d0: 2020 2020 2020 2020 7769 6e64 6f77 3d77          window=w
+0000e8e0: 696e 646f 772c 0a20 2020 2020 2020 2020  indow,.         
+0000e8f0: 2020 202a 2a70 6172 616d 732c 0a20 2020     **params,.   
+0000e900: 2020 2020 2029 0a0a 0a63 6c61 7373 2043       )...class C
+0000e910: 5378 3a0a 2020 2020 2222 224d 6178 696d  Sx:.    """Maxim
+0000e920: 756d 206c 656e 6774 6820 6f66 2063 6f6c  um length of col
+0000e930: 6420 7370 656c 6c73 2028 7461 7329 2e22  d spells (tas)."
+0000e940: 2222 0a0a 2020 2020 7468 7265 7368 203d  ""..    thresh =
+0000e950: 202d 3130 0a20 2020 2077 696e 646f 7720   -10.    window 
+0000e960: 3d20 310a 0a20 2020 2064 6566 2063 6f6d  = 1..    def com
+0000e970: 7075 7465 2874 6872 6573 683d 7468 7265  pute(thresh=thre
+0000e980: 7368 2c20 7769 6e64 6f77 3d77 696e 646f  sh, window=windo
+0000e990: 772c 202a 2a70 6172 616d 7329 3a0a 2020  w, **params):.  
+0000e9a0: 2020 2020 2020 2222 2243 616c 6375 6c61        """Calcula
+0000e9b0: 7465 206d 6178 696d 756d 206c 656e 6774  te maximum lengt
+0000e9c0: 6820 6f66 2063 6f6c 6420 7370 656c 6c73  h of cold spells
+0000e9d0: 2e0a 0a20 2020 2020 2020 2050 6172 616d  ...        Param
+0000e9e0: 6574 6572 730a 2020 2020 2020 2020 2d2d  eters.        --
+0000e9f0: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020 2020  --------.       
+0000ea00: 2074 6872 6573 683a 2069 6e74 206f 7220   thresh: int or 
+0000ea10: 7374 7269 6e67 0a20 2020 2020 2020 2020  string.         
+0000ea20: 2020 2054 6872 6573 686f 6c64 2074 656d     Threshold tem
+0000ea30: 7065 7261 7475 7265 2062 656c 6f77 2077  perature below w
+0000ea40: 6869 6368 2061 2064 6179 2069 7320 636f  hich a day is co
+0000ea50: 6e73 6964 6572 6564 0a20 2020 2020 2020  nsidered.       
+0000ea60: 2020 2020 2061 7320 6120 636f 6c64 2064       as a cold d
+0000ea70: 6179 2028 6465 6661 756c 743a 202d 3130  ay (default: -10
+0000ea80: 2064 6567 4329 2e0a 2020 2020 2020 2020   degC)..        
+0000ea90: 2020 2020 4966 2074 7970 6520 6f66 2074      If type of t
+0000eaa0: 6872 6573 686f 6c64 2069 7320 616e 2069  hreshold is an i
+0000eab0: 6e74 6567 6572 2074 6865 2075 6e69 7420  nteger the unit 
+0000eac0: 6973 2073 6574 2074 6f20 6465 6743 2e0a  is set to degC..
+0000ead0: 2020 2020 2020 2020 7769 6e64 6f77 3a20          window: 
+0000eae0: 696e 740a 2020 2020 2020 2020 2020 2020  int.            
+0000eaf0: 4d69 6e69 6d75 6d20 6e75 6d62 6572 206f  Minimum number o
+0000eb00: 6620 6461 7973 2077 6974 6820 7465 6d70  f days with temp
+0000eb10: 6572 6174 7572 6520 6265 6c6f 7720 7468  erature below th
+0000eb20: 7265 7368 0a20 2020 2020 2020 2020 2020  resh.           
+0000eb30: 2074 6f20 7175 616c 6966 7920 6173 2061   to qualify as a
+0000eb40: 2063 6f6c 6420 7370 656c 6c20 2864 6566   cold spell (def
+0000eb50: 6175 6c74 3a20 3129 2e0a 0a20 2020 2020  ault: 1)...     
+0000eb60: 2020 2052 6574 7572 6e73 0a20 2020 2020     Returns.     
+0000eb70: 2020 202d 2d2d 2d2d 2d2d 0a20 2020 2020     -------.     
+0000eb80: 2020 2078 6172 7261 792e 4461 7461 4172     xarray.DataAr
+0000eb90: 7261 790a 2020 2020 2020 2020 2020 2020  ray.            
+0000eba0: 4e75 6d62 6572 206f 6620 636f 6c64 2073  Number of cold s
+0000ebb0: 7065 6c6c 7320 6f66 2061 7420 6c65 6173  pells of at leas
+0000ebc0: 7420 7b77 696e 646f 777d 2063 6f6e 7365  t {window} conse
+0000ebd0: 6375 7469 7665 2064 6179 730a 2020 2020  cutive days.    
+0000ebe0: 2020 2020 2020 2020 7769 7468 2074 656d          with tem
+0000ebf0: 7065 7261 7475 7265 2062 656c 6f77 207b  perature below {
+0000ec00: 7468 7265 7368 7d2e 0a0a 2020 2020 2020  thresh}...      
+0000ec10: 2020 4e6f 7465 730a 2020 2020 2020 2020    Notes.        
+0000ec20: 2d2d 2d2d 2d0a 2020 2020 2020 2020 466f  -----.        Fo
+0000ec30: 7220 6d6f 7265 2069 6e66 6f72 6d61 7469  r more informati
+0000ec40: 6f6e 206f 6e20 7468 6520 696e 7075 7420  on on the input 
+0000ec50: 7061 7261 6d65 7465 7273 2073 6565 3a0a  parameters see:.
+0000ec60: 2020 2020 2020 2020 2020 2020 6874 7470              http
+0000ec70: 733a 2f2f 7863 6c69 6d2e 7265 6164 7468  s://xclim.readth
+0000ec80: 6564 6f63 732e 696f 2f65 6e2f 7374 6162  edocs.io/en/stab
+0000ec90: 6c65 2f61 7069 2e68 746d 6c23 7863 6c69  le/api.html#xcli
+0000eca0: 6d2e 696e 6469 6361 746f 7273 2e61 746d  m.indicators.atm
+0000ecb0: 6f73 2e63 6f6c 645f 7370 656c 6c5f 6d61  os.cold_spell_ma
+0000ecc0: 785f 6c65 6e67 7468 0a20 2020 2020 2020  x_length.       
+0000ecd0: 2022 2222 0a20 2020 2020 2020 2074 6872   """.        thr
+0000ece0: 6573 6820 3d20 5f74 6872 6573 685f 7374  esh = _thresh_st
+0000ecf0: 7269 6e67 2874 6872 6573 682c 2022 6465  ring(thresh, "de
+0000ed00: 6743 2229 0a20 2020 2020 2020 2072 6574  gC").        ret
+0000ed10: 7572 6e20 7863 2e61 746d 6f73 2e63 6f6c  urn xc.atmos.col
+0000ed20: 645f 7370 656c 6c5f 6d61 785f 6c65 6e67  d_spell_max_leng
+0000ed30: 7468 280a 2020 2020 2020 2020 2020 2020  th(.            
+0000ed40: 7468 7265 7368 3d74 6872 6573 682c 0a20  thresh=thresh,. 
+0000ed50: 2020 2020 2020 2020 2020 2077 696e 646f             windo
+0000ed60: 773d 7769 6e64 6f77 2c0a 2020 2020 2020  w=window,.      
+0000ed70: 2020 2020 2020 2a2a 7061 7261 6d73 2c0a        **params,.
+0000ed80: 2020 2020 2020 2020 290a 0a0a 636c 6173          )...clas
+0000ed90: 7320 4353 6e3a 0a20 2020 2022 2222 546f  s CSn:.    """To
+0000eda0: 7461 6c20 6e75 6d62 6572 206f 6620 6461  tal number of da
+0000edb0: 7973 2069 6e20 636f 6c64 2073 7065 6c6c  ys in cold spell
+0000edc0: 7320 2874 6173 292e 2222 220a 0a20 2020  s (tas)."""..   
+0000edd0: 2074 6872 6573 6820 3d20 2d31 300a 2020   thresh = -10.  
+0000ede0: 2020 7769 6e64 6f77 203d 2033 0a0a 2020    window = 3..  
+0000edf0: 2020 6465 6620 636f 6d70 7574 6528 7468    def compute(th
+0000ee00: 7265 7368 3d74 6872 6573 682c 2077 696e  resh=thresh, win
+0000ee10: 646f 773d 7769 6e64 6f77 2c20 2a2a 7061  dow=window, **pa
+0000ee20: 7261 6d73 293a 0a20 2020 2020 2020 2022  rams):.        "
+0000ee30: 2222 4361 6c63 756c 6174 6520 746f 7461  ""Calculate tota
+0000ee40: 6c20 6e75 6d62 6572 206f 6620 6461 7973  l number of days
+0000ee50: 2069 6e20 636f 6c64 2073 7065 6c6c 732e   in cold spells.
+0000ee60: 0a0a 2020 2020 2020 2020 5061 7261 6d65  ..        Parame
+0000ee70: 7465 7273 0a20 2020 2020 2020 202d 2d2d  ters.        ---
+0000ee80: 2d2d 2d2d 2d2d 2d0a 2020 2020 2020 2020  -------.        
+0000ee90: 7468 7265 7368 3a20 696e 7420 6f72 2073  thresh: int or s
+0000eea0: 7472 696e 670a 2020 2020 2020 2020 2020  tring.          
+0000eeb0: 2020 5468 7265 7368 6f6c 6420 7465 6d70    Threshold temp
+0000eec0: 6572 6174 7572 6520 6265 6c6f 7720 7768  erature below wh
+0000eed0: 6963 6820 6120 6461 7920 6973 2063 6f6e  ich a day is con
+0000eee0: 7369 6465 7265 640a 2020 2020 2020 2020  sidered.        
+0000eef0: 2020 2020 6173 2061 2063 6f6c 6420 6461      as a cold da
+0000ef00: 7920 2864 6566 6175 6c74 3a20 2d31 3020  y (default: -10 
+0000ef10: 6465 6743 292e 0a20 2020 2020 2020 2020  degC)..         
+0000ef20: 2020 2049 6620 7479 7065 206f 6620 7468     If type of th
+0000ef30: 7265 7368 6f6c 6420 6973 2061 6e20 696e  reshold is an in
+0000ef40: 7465 6765 7220 7468 6520 756e 6974 2069  teger the unit i
+0000ef50: 7320 7365 7420 746f 2064 6567 432e 0a20  s set to degC.. 
+0000ef60: 2020 2020 2020 2077 696e 646f 773a 2069         window: i
+0000ef70: 6e74 0a20 2020 2020 2020 2020 2020 204d  nt.            M
+0000ef80: 696e 696d 756d 206e 756d 6265 7220 6f66  inimum number of
+0000ef90: 2064 6179 7320 7769 7468 2074 656d 7065   days with tempe
+0000efa0: 7261 7475 7265 2062 656c 6f77 2074 6872  rature below thr
+0000efb0: 6573 680a 2020 2020 2020 2020 2020 2020  esh.            
+0000efc0: 746f 2071 7561 6c69 6679 2061 7320 6120  to qualify as a 
+0000efd0: 636f 6c64 2073 7065 6c6c 2028 6465 6661  cold spell (defa
+0000efe0: 756c 743a 2033 292e 0a0a 2020 2020 2020  ult: 3)...      
+0000eff0: 2020 5265 7475 726e 730a 2020 2020 2020    Returns.      
+0000f000: 2020 2d2d 2d2d 2d2d 2d0a 2020 2020 2020    -------.      
+0000f010: 2020 7861 7272 6179 2e44 6174 6141 7272    xarray.DataArr
+0000f020: 6179 0a20 2020 2020 2020 2020 2020 2054  ay.            T
+0000f030: 6f74 616c 206e 756d 6265 7220 6f66 2064  otal number of d
+0000f040: 6179 7320 696e 2063 6f6c 6420 7370 656c  ays in cold spel
+0000f050: 6c73 206f 6620 6174 206c 6561 7374 207b  ls of at least {
+0000f060: 7769 6e64 6f77 7d0a 2020 2020 2020 2020  window}.        
+0000f070: 2020 2020 636f 6e73 6563 7574 6976 6520      consecutive 
+0000f080: 6461 7973 2077 6974 6820 7465 6d70 6572  days with temper
+0000f090: 6174 7572 6520 6265 6c6f 7720 7b74 6872  ature below {thr
+0000f0a0: 6573 687d 2e0a 0a20 2020 2020 2020 204e  esh}...        N
+0000f0b0: 6f74 6573 0a20 2020 2020 2020 202d 2d2d  otes.        ---
+0000f0c0: 2d2d 0a20 2020 2020 2020 2046 6f72 206d  --.        For m
+0000f0d0: 6f72 6520 696e 666f 726d 6174 696f 6e20  ore information 
+0000f0e0: 6f6e 2074 6865 2069 6e70 7574 2070 6172  on the input par
+0000f0f0: 616d 6574 6572 7320 7365 653a 0a20 2020  ameters see:.   
+0000f100: 2020 2020 2020 2020 2068 7474 7073 3a2f           https:/
+0000f110: 2f78 636c 696d 2e72 6561 6474 6865 646f  /xclim.readthedo
+0000f120: 6373 2e69 6f2f 656e 2f73 7461 626c 652f  cs.io/en/stable/
+0000f130: 6170 692e 6874 6d6c 2378 636c 696d 2e69  api.html#xclim.i
+0000f140: 6e64 6963 6174 6f72 732e 6174 6d6f 732e  ndicators.atmos.
+0000f150: 636f 6c64 5f73 7065 6c6c 5f74 6f74 616c  cold_spell_total
+0000f160: 5f6c 656e 6774 680a 2020 2020 2020 2020  _length.        
+0000f170: 2222 220a 2020 2020 2020 2020 7468 7265  """.        thre
+0000f180: 7368 203d 205f 7468 7265 7368 5f73 7472  sh = _thresh_str
+0000f190: 696e 6728 7468 7265 7368 2c20 2264 6567  ing(thresh, "deg
+0000f1a0: 4322 290a 2020 2020 2020 2020 7265 7475  C").        retu
+0000f1b0: 726e 2078 632e 6174 6d6f 732e 636f 6c64  rn xc.atmos.cold
+0000f1c0: 5f73 7065 6c6c 5f74 6f74 616c 5f6c 656e  _spell_total_len
+0000f1d0: 6774 6828 0a20 2020 2020 2020 2020 2020  gth(.           
+0000f1e0: 2074 6872 6573 683d 7468 7265 7368 2c0a   thresh=thresh,.
+0000f1f0: 2020 2020 2020 2020 2020 2020 7769 6e64              wind
+0000f200: 6f77 3d77 696e 646f 772c 0a20 2020 2020  ow=window,.     
+0000f210: 2020 2020 2020 202a 2a70 6172 616d 732c         **params,
+0000f220: 0a20 2020 2020 2020 2029 0a0a 0a63 6c61  .        )...cla
+0000f230: 7373 2048 5366 3a0a 2020 2020 2222 224e  ss HSf:.    """N
+0000f240: 756d 6265 7220 6f66 2068 6f74 2073 7065  umber of hot spe
+0000f250: 6c6c 7320 2874 6173 6d61 7829 2e22 2222  lls (tasmax)."""
+0000f260: 0a0a 2020 2020 7468 7265 7368 203d 2033  ..    thresh = 3
+0000f270: 350a 2020 2020 7769 6e64 6f77 203d 2033  5.    window = 3
+0000f280: 0a0a 2020 2020 6465 6620 636f 6d70 7574  ..    def comput
+0000f290: 6528 7468 7265 7368 3d74 6872 6573 682c  e(thresh=thresh,
+0000f2a0: 2077 696e 646f 773d 7769 6e64 6f77 2c20   window=window, 
+0000f2b0: 2a2a 7061 7261 6d73 293a 0a20 2020 2020  **params):.     
+0000f2c0: 2020 2022 2222 4361 6c63 756c 6174 6520     """Calculate 
+0000f2d0: 6e75 6d62 6572 206f 6620 686f 7420 7370  number of hot sp
+0000f2e0: 656c 6c73 2e0a 0a20 2020 2020 2020 2050  ells...        P
+0000f2f0: 6172 616d 6574 6572 730a 2020 2020 2020  arameters.      
+0000f300: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020    ----------.   
+0000f310: 2020 2020 2074 6872 6573 683a 2069 6e74       thresh: int
+0000f320: 206f 7220 7374 7269 6e67 0a20 2020 2020   or string.     
+0000f330: 2020 2020 2020 2054 6872 6573 686f 6c64         Threshold
+0000f340: 206d 6178 696d 756d 2074 656d 7065 7261   maximum tempera
+0000f350: 7475 7265 2061 626f 7665 2077 6869 6368  ture above which
+0000f360: 2061 2064 6179 2069 7320 636f 6e73 6964   a day is consid
+0000f370: 6572 6564 0a20 2020 2020 2020 2020 2020  ered.           
+0000f380: 2061 7320 6120 686f 7420 6461 7920 2864   as a hot day (d
+0000f390: 6566 6175 6c74 3a20 3335 2064 6567 4329  efault: 35 degC)
+0000f3a0: 2e0a 2020 2020 2020 2020 2020 2020 4966  ..            If
+0000f3b0: 2074 7970 6520 6f66 2074 6872 6573 686f   type of thresho
+0000f3c0: 6c64 2069 7320 616e 2069 6e74 6567 6572  ld is an integer
+0000f3d0: 2074 6865 2075 6e69 7420 6973 2073 6574   the unit is set
+0000f3e0: 2074 6f20 6465 6743 2e0a 2020 2020 2020   to degC..      
+0000f3f0: 2020 7769 6e64 6f77 3a20 696e 740a 2020    window: int.  
+0000f400: 2020 2020 2020 2020 2020 4d69 6e69 6d75            Minimu
+0000f410: 6d20 6e75 6d62 6572 206f 6620 6461 7973  m number of days
+0000f420: 2077 6974 6820 7465 6d70 6572 6174 7572   with temperatur
+0000f430: 6520 6162 6f76 6520 7468 7265 7368 0a20  e above thresh. 
+0000f440: 2020 2020 2020 2020 2020 2074 6f20 7175             to qu
+0000f450: 616c 6966 7920 6173 2061 2068 6f74 2073  alify as a hot s
+0000f460: 7065 6c6c 2028 6465 6661 756c 743a 2033  pell (default: 3
+0000f470: 292e 0a0a 2020 2020 2020 2020 5265 7475  )...        Retu
+0000f480: 726e 730a 2020 2020 2020 2020 2d2d 2d2d  rns.        ----
+0000f490: 2d2d 2d0a 2020 2020 2020 2020 7861 7272  ---.        xarr
+0000f4a0: 6179 2e44 6174 6141 7272 6179 0a20 2020  ay.DataArray.   
+0000f4b0: 2020 2020 2020 2020 204e 756d 6265 7220           Number 
+0000f4c0: 6f66 2068 6f74 2073 7065 6c6c 7320 6f66  of hot spells of
+0000f4d0: 2061 7420 6c65 6173 7420 7b77 696e 646f   at least {windo
+0000f4e0: 777d 2063 6f6e 7365 6375 7469 7665 2064  w} consecutive d
+0000f4f0: 6179 730a 2020 2020 2020 2020 2020 2020  ays.            
+0000f500: 7769 7468 206d 6178 696d 756d 2074 656d  with maximum tem
+0000f510: 7065 7261 7475 7265 2061 626f 7665 207b  perature above {
+0000f520: 7468 7265 7368 7d2e 0a0a 2020 2020 2020  thresh}...      
+0000f530: 2020 4e6f 7465 730a 2020 2020 2020 2020    Notes.        
+0000f540: 2d2d 2d2d 2d0a 2020 2020 2020 2020 466f  -----.        Fo
+0000f550: 7220 6d6f 7265 2069 6e66 6f72 6d61 7469  r more informati
+0000f560: 6f6e 206f 6e20 7468 6520 696e 7075 7420  on on the input 
+0000f570: 7061 7261 6d65 7465 7273 2073 6565 3a0a  parameters see:.
+0000f580: 2020 2020 2020 2020 2020 2020 6874 7470              http
+0000f590: 733a 2f2f 7863 6c69 6d2e 7265 6164 7468  s://xclim.readth
+0000f5a0: 6564 6f63 732e 696f 2f65 6e2f 7374 6162  edocs.io/en/stab
+0000f5b0: 6c65 2f61 7069 2e68 746d 6c23 7863 6c69  le/api.html#xcli
+0000f5c0: 6d2e 696e 6469 6361 746f 7273 2e61 746d  m.indicators.atm
+0000f5d0: 6f73 2e68 6f74 5f73 7065 6c6c 5f66 7265  os.hot_spell_fre
+0000f5e0: 7175 656e 6379 0a20 2020 2020 2020 2022  quency.        "
+0000f5f0: 2222 0a20 2020 2020 2020 2074 6872 6573  "".        thres
+0000f600: 6820 3d20 5f74 6872 6573 685f 7374 7269  h = _thresh_stri
+0000f610: 6e67 2874 6872 6573 682c 2022 6465 6743  ng(thresh, "degC
+0000f620: 2229 0a20 2020 2020 2020 2072 6574 7572  ").        retur
+0000f630: 6e20 7863 2e61 746d 6f73 2e68 6f74 5f73  n xc.atmos.hot_s
+0000f640: 7065 6c6c 5f66 7265 7175 656e 6379 280a  pell_frequency(.
+0000f650: 2020 2020 2020 2020 2020 2020 7468 7265              thre
+0000f660: 7368 3d74 6872 6573 682c 0a20 2020 2020  sh=thresh,.     
+0000f670: 2020 2020 2020 2077 696e 646f 773d 7769         window=wi
+0000f680: 6e64 6f77 2c0a 2020 2020 2020 2020 2020  ndow,.          
+0000f690: 2020 2a2a 7061 7261 6d73 2c0a 2020 2020    **params,.    
+0000f6a0: 2020 2020 290a 0a0a 636c 6173 7320 4853      )...class HS
+0000f6b0: 783a 0a20 2020 2022 2222 4d61 7869 6d75  x:.    """Maximu
+0000f6c0: 6d20 6c65 6e67 6874 206f 6620 686f 7420  m lenght of hot 
+0000f6d0: 7370 656c 6c73 2028 7461 736d 6178 292e  spells (tasmax).
+0000f6e0: 2222 220a 0a20 2020 2074 6872 6573 6820  """..    thresh 
+0000f6f0: 3d20 3335 0a20 2020 2077 696e 646f 7720  = 35.    window 
+0000f700: 3d20 310a 0a20 2020 2064 6566 2063 6f6d  = 1..    def com
+0000f710: 7075 7465 2874 6872 6573 683d 7468 7265  pute(thresh=thre
+0000f720: 7368 2c20 7769 6e64 6f77 3d77 696e 646f  sh, window=windo
+0000f730: 772c 202a 2a70 6172 616d 7329 3a0a 2020  w, **params):.  
+0000f740: 2020 2020 2020 2222 2243 616c 6375 6c61        """Calcula
+0000f750: 7465 206d 6178 696d 756d 206c 656e 6768  te maximum lengh
+0000f760: 7420 6f66 2068 6f74 2073 7065 6c6c 732e  t of hot spells.
+0000f770: 0a0a 2020 2020 2020 2020 5061 7261 6d65  ..        Parame
+0000f780: 7465 7273 0a20 2020 2020 2020 202d 2d2d  ters.        ---
+0000f790: 2d2d 2d2d 2d2d 2d0a 2020 2020 2020 2020  -------.        
+0000f7a0: 7468 7265 7368 3a20 696e 7420 6f72 2073  thresh: int or s
+0000f7b0: 7472 696e 670a 2020 2020 2020 2020 2020  tring.          
+0000f7c0: 2020 5468 7265 7368 6f6c 6420 6d61 7869    Threshold maxi
+0000f7d0: 6d75 6d20 7465 6d70 6572 6174 7572 6520  mum temperature 
+0000f7e0: 6162 6f76 6520 7768 6963 6820 6120 6461  above which a da
+0000f7f0: 7920 6973 2063 6f6e 7369 6465 7265 640a  y is considered.
+0000f800: 2020 2020 2020 2020 2020 2020 6173 2061              as a
+0000f810: 2068 6f74 2064 6179 2028 6465 6661 756c   hot day (defaul
+0000f820: 743a 2033 3520 6465 6743 292e 0a20 2020  t: 35 degC)..   
+0000f830: 2020 2020 2020 2020 2049 6620 7479 7065           If type
+0000f840: 206f 6620 7468 7265 7368 6f6c 6420 6973   of threshold is
+0000f850: 2061 6e20 696e 7465 6765 7220 7468 6520   an integer the 
+0000f860: 756e 6974 2069 7320 7365 7420 746f 2064  unit is set to d
+0000f870: 6567 432e 0a20 2020 2020 2020 2077 696e  egC..        win
+0000f880: 646f 773a 2069 6e74 0a20 2020 2020 2020  dow: int.       
+0000f890: 2020 2020 204d 696e 696d 756d 206e 756d       Minimum num
+0000f8a0: 6265 7220 6f66 2064 6179 7320 7769 7468  ber of days with
+0000f8b0: 2074 656d 7065 7261 7475 7265 2061 626f   temperature abo
+0000f8c0: 7665 2074 6872 6573 680a 2020 2020 2020  ve thresh.      
+0000f8d0: 2020 2020 2020 746f 2071 7561 6c69 6679        to qualify
+0000f8e0: 2061 7320 6120 686f 7420 7370 656c 6c20   as a hot spell 
+0000f8f0: 2864 6566 6175 6c74 3a20 3129 2e0a 0a20  (default: 1)... 
+0000f900: 2020 2020 2020 2052 6574 7572 6e73 0a20         Returns. 
+0000f910: 2020 2020 2020 202d 2d2d 2d2d 2d2d 0a20         -------. 
+0000f920: 2020 2020 2020 2078 6172 7261 792e 4461         xarray.Da
+0000f930: 7461 4172 7261 790a 2020 2020 2020 2020  taArray.        
+0000f940: 2020 2020 4d61 7869 6d75 6d20 6c65 6e67      Maximum leng
+0000f950: 7468 206f 6620 686f 7420 7370 656c 6c73  th of hot spells
+0000f960: 206f 6620 6174 206c 6561 7374 207b 7769   of at least {wi
+0000f970: 6e64 6f77 7d0a 2020 2020 2020 2020 2020  ndow}.          
+0000f980: 2020 636f 6e73 6563 7574 6976 6520 6461    consecutive da
+0000f990: 7973 2077 6974 6820 6d61 7869 6d75 6d20  ys with maximum 
+0000f9a0: 7465 6d70 6572 6174 7572 6520 6162 6f76  temperature abov
+0000f9b0: 6520 7b74 6872 6573 687d 2e0a 0a20 2020  e {thresh}...   
+0000f9c0: 2020 2020 204e 6f74 6573 0a20 2020 2020       Notes.     
+0000f9d0: 2020 202d 2d2d 2d2d 0a20 2020 2020 2020     -----.       
+0000f9e0: 2046 6f72 206d 6f72 6520 696e 666f 726d   For more inform
+0000f9f0: 6174 696f 6e20 6f6e 2074 6865 2069 6e70  ation on the inp
+0000fa00: 7574 2070 6172 616d 6574 6572 7320 7365  ut parameters se
+0000fa10: 653a 0a20 2020 2020 2020 2020 2020 2068  e:.            h
+0000fa20: 7474 7073 3a2f 2f78 636c 696d 2e72 6561  ttps://xclim.rea
+0000fa30: 6474 6865 646f 6373 2e69 6f2f 656e 2f73  dthedocs.io/en/s
+0000fa40: 7461 626c 652f 6170 692e 6874 6d6c 2378  table/api.html#x
+0000fa50: 636c 696d 2e69 6e64 6963 6174 6f72 732e  clim.indicators.
+0000fa60: 6174 6d6f 732e 686f 745f 7370 656c 6c5f  atmos.hot_spell_
+0000fa70: 6d61 785f 6c65 6e67 7468 0a20 2020 2020  max_length.     
+0000fa80: 2020 2022 2222 0a20 2020 2020 2020 2074     """.        t
+0000fa90: 6872 6573 6820 3d20 5f74 6872 6573 685f  hresh = _thresh_
+0000faa0: 7374 7269 6e67 2874 6872 6573 682c 2022  string(thresh, "
+0000fab0: 6465 6743 2229 0a20 2020 2020 2020 2072  degC").        r
+0000fac0: 6574 7572 6e20 7863 2e61 746d 6f73 2e68  eturn xc.atmos.h
+0000fad0: 6f74 5f73 7065 6c6c 5f6d 6178 5f6c 656e  ot_spell_max_len
+0000fae0: 6774 6828 0a20 2020 2020 2020 2020 2020  gth(.           
+0000faf0: 2074 6872 6573 683d 7468 7265 7368 2c0a   thresh=thresh,.
+0000fb00: 2020 2020 2020 2020 2020 2020 7769 6e64              wind
+0000fb10: 6f77 3d77 696e 646f 772c 0a20 2020 2020  ow=window,.     
+0000fb20: 2020 2020 2020 202a 2a70 6172 616d 732c         **params,
+0000fb30: 0a20 2020 2020 2020 2029 0a0a 0a63 6c61  .        )...cla
+0000fb40: 7373 2048 536e 3a0a 2020 2020 2222 2254  ss HSn:.    """T
+0000fb50: 6f74 616c 206e 756d 6265 7220 6f66 2064  otal number of d
+0000fb60: 6179 7320 696e 2068 6f74 2073 7065 6c6c  ays in hot spell
+0000fb70: 7320 2874 6173 6d61 7829 2e22 2222 0a0a  s (tasmax)."""..
+0000fb80: 2020 2020 7468 7265 7368 203d 2033 350a      thresh = 35.
+0000fb90: 2020 2020 7769 6e64 6f77 203d 2033 0a0a      window = 3..
+0000fba0: 2020 2020 6465 6620 636f 6d70 7574 6528      def compute(
+0000fbb0: 7468 7265 7368 3d74 6872 6573 682c 2077  thresh=thresh, w
+0000fbc0: 696e 646f 773d 7769 6e64 6f77 2c20 2a2a  indow=window, **
+0000fbd0: 7061 7261 6d73 293a 0a20 2020 2020 2020  params):.       
+0000fbe0: 2022 2222 4361 6c63 756c 6174 6520 746f   """Calculate to
+0000fbf0: 7461 6c20 6e75 6d62 6572 206f 6620 6461  tal number of da
+0000fc00: 7973 2069 6e20 686f 7420 7370 656c 6c73  ys in hot spells
+0000fc10: 2e0a 0a20 2020 2020 2020 2050 6172 616d  ...        Param
+0000fc20: 6574 6572 730a 2020 2020 2020 2020 2d2d  eters.        --
+0000fc30: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020 2020  --------.       
+0000fc40: 2074 6872 6573 683a 2069 6e74 206f 7220   thresh: int or 
+0000fc50: 7374 7269 6e67 0a20 2020 2020 2020 2020  string.         
+0000fc60: 2020 2054 6872 6573 686f 6c64 206d 6178     Threshold max
+0000fc70: 696d 756d 2074 656d 7065 7261 7475 7265  imum temperature
+0000fc80: 2061 626f 7665 2077 6869 6368 2061 2064   above which a d
+0000fc90: 6179 2069 7320 636f 6e73 6964 6572 6564  ay is considered
+0000fca0: 0a20 2020 2020 2020 2020 2020 2061 7320  .            as 
+0000fcb0: 6120 686f 7420 6461 7920 2864 6566 6175  a hot day (defau
+0000fcc0: 6c74 3a20 3335 2064 6567 4329 2e0a 2020  lt: 35 degC)..  
+0000fcd0: 2020 2020 2020 2020 2020 4966 2074 7970            If typ
+0000fce0: 6520 6f66 2074 6872 6573 686f 6c64 2069  e of threshold i
+0000fcf0: 7320 616e 2069 6e74 6567 6572 2074 6865  s an integer the
+0000fd00: 2075 6e69 7420 6973 2073 6574 2074 6f20   unit is set to 
+0000fd10: 6465 6743 2e0a 2020 2020 2020 2020 7769  degC..        wi
+0000fd20: 6e64 6f77 3a20 696e 740a 2020 2020 2020  ndow: int.      
+0000fd30: 2020 2020 2020 4d69 6e69 6d75 6d20 6e75        Minimum nu
+0000fd40: 6d62 6572 206f 6620 6461 7973 2077 6974  mber of days wit
+0000fd50: 6820 7465 6d70 6572 6174 7572 6520 6162  h temperature ab
+0000fd60: 6f76 6520 7468 7265 7368 0a20 2020 2020  ove thresh.     
+0000fd70: 2020 2020 2020 2074 6f20 7175 616c 6966         to qualif
+0000fd80: 7920 6173 2061 2068 6f74 2073 7065 6c6c  y as a hot spell
+0000fd90: 2028 6465 6661 756c 743a 2033 292e 0a0a   (default: 3)...
+0000fda0: 2020 2020 2020 2020 5265 7475 726e 730a          Returns.
+0000fdb0: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d0a          -------.
+0000fdc0: 2020 2020 2020 2020 7861 7272 6179 2e44          xarray.D
+0000fdd0: 6174 6141 7272 6179 0a20 2020 2020 2020  ataArray.       
+0000fde0: 2020 2020 2054 6f74 616c 206e 756d 6265       Total numbe
+0000fdf0: 7220 6f66 2020 6461 7973 2069 6e20 686f  r of  days in ho
+0000fe00: 7420 7370 656c 6c73 206f 6620 6174 206c  t spells of at l
+0000fe10: 6561 7374 207b 7769 6e64 6f77 7d0a 2020  east {window}.  
+0000fe20: 2020 2020 2020 2020 2020 636f 6e73 6563            consec
+0000fe30: 7574 6976 6520 6461 7973 2077 6974 6820  utive days with 
+0000fe40: 6d61 7869 6d75 6d20 7465 6d70 6572 6174  maximum temperat
+0000fe50: 7572 6520 6162 6f76 6520 7b74 6872 6573  ure above {thres
+0000fe60: 687d 2e0a 0a20 2020 2020 2020 204e 6f74  h}...        Not
+0000fe70: 6573 0a20 2020 2020 2020 202d 2d2d 2d2d  es.        -----
+0000fe80: 0a20 2020 2020 2020 2046 6f72 206d 6f72  .        For mor
+0000fe90: 6520 696e 666f 726d 6174 696f 6e20 6f6e  e information on
+0000fea0: 2074 6865 2069 6e70 7574 2070 6172 616d   the input param
+0000feb0: 6574 6572 7320 7365 653a 0a20 2020 2020  eters see:.     
+0000fec0: 2020 2020 2020 2068 7474 7073 3a2f 2f78         https://x
+0000fed0: 636c 696d 2e72 6561 6474 6865 646f 6373  clim.readthedocs
+0000fee0: 2e69 6f2f 656e 2f73 7461 626c 652f 6170  .io/en/stable/ap
+0000fef0: 692e 6874 6d6c 2378 636c 696d 2e69 6e64  i.html#xclim.ind
+0000ff00: 6963 6174 6f72 732e 6174 6d6f 732e 686f  icators.atmos.ho
+0000ff10: 745f 7370 656c 6c5f 746f 7461 6c5f 6c65  t_spell_total_le
+0000ff20: 6e67 7468 0a20 2020 2020 2020 2022 2222  ngth.        """
+0000ff30: 0a20 2020 2020 2020 2074 6872 6573 6820  .        thresh 
+0000ff40: 3d20 5f74 6872 6573 685f 7374 7269 6e67  = _thresh_string
+0000ff50: 2874 6872 6573 682c 2022 6465 6743 2229  (thresh, "degC")
+0000ff60: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+0000ff70: 7863 2e61 746d 6f73 2e68 6f74 5f73 7065  xc.atmos.hot_spe
+0000ff80: 6c6c 5f74 6f74 616c 5f6c 656e 6774 6828  ll_total_length(
+0000ff90: 0a20 2020 2020 2020 2020 2020 2074 6872  .            thr
+0000ffa0: 6573 683d 7468 7265 7368 2c0a 2020 2020  esh=thresh,.    
+0000ffb0: 2020 2020 2020 2020 7769 6e64 6f77 3d77          window=w
+0000ffc0: 696e 646f 772c 0a20 2020 2020 2020 2020  indow,.         
+0000ffd0: 2020 202a 2a70 6172 616d 732c 0a20 2020     **params,.   
+0000ffe0: 2020 2020 2029 0a0a 0a63 6c61 7373 2053       )...class S
+0000fff0: 443a 0a20 2020 2022 2222 4e75 6d62 6572  D:.    """Number
+00010000: 206f 6620 736e 6f77 2064 6179 732e 2222   of snow days.""
+00010010: 220a 0a20 2020 2074 6872 6573 6820 3d20  "..    thresh = 
+00010020: 310a 0a20 2020 2064 6566 2063 6f6d 7075  1..    def compu
+00010030: 7465 2874 6872 6573 683d 7468 7265 7368  te(thresh=thresh
+00010040: 2c20 2a2a 7061 7261 6d73 293a 0a20 2020  , **params):.   
+00010050: 2020 2020 2022 2222 4361 6c63 756c 6174       """Calculat
+00010060: 6520 6e75 6d62 6572 206f 6620 736e 6f77  e number of snow
+00010070: 2064 6179 732e 0a0a 2020 2020 2020 2020   days...        
+00010080: 5061 7261 6d65 7465 7273 0a20 2020 2020  Parameters.     
+00010090: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020     ----------.  
+000100a0: 2020 2020 2020 7468 7265 7368 3a20 696e        thresh: in
+000100b0: 7420 6f72 2073 7472 696e 670a 2020 2020  t or string.    
+000100c0: 2020 2020 2020 2020 4c69 7175 6964 2077          Liquid w
+000100d0: 6174 6572 2065 7175 6976 616c 656e 7420  ater equivalent 
+000100e0: 736e 6f77 6661 6c6c 2072 6174 6520 6162  snowfall rate ab
+000100f0: 6f76 6520 7768 6963 6820 6120 6461 7920  ove which a day 
+00010100: 6973 0a20 2020 2020 2020 2020 2020 2063  is.            c
+00010110: 6f6e 7369 6465 7265 6420 6173 2061 2073  onsidered as a s
+00010120: 6e6f 7720 6461 7920 2864 6566 6175 6c74  now day (default
+00010130: 3a20 3120 6d6d 2f64 6179 2920 2e0a 2020  : 1 mm/day) ..  
+00010140: 2020 2020 2020 2020 2020 4966 2074 7970            If typ
+00010150: 6520 6f66 2074 6872 6573 686f 6c64 2069  e of threshold i
+00010160: 7320 616e 2069 6e74 6567 6572 2074 6865  s an integer the
+00010170: 2075 6e69 7420 6973 2073 6574 2074 6f20   unit is set to 
+00010180: 6d6d 2f64 6179 2e0a 0a20 2020 2020 2020  mm/day...       
+00010190: 2052 6574 7572 6e73 0a20 2020 2020 2020   Returns.       
+000101a0: 202d 2d2d 2d2d 2d2d 0a20 2020 2020 2020   -------.       
+000101b0: 2078 6172 7261 792e 4461 7461 4172 7261   xarray.DataArra
+000101c0: 790a 2020 2020 2020 2020 2020 2020 4e75  y.            Nu
+000101d0: 6d62 6572 206f 6620 6461 7973 2077 6974  mber of days wit
+000101e0: 6820 736f 6c69 6420 7072 6563 6970 6974  h solid precipit
+000101f0: 6174 696f 6e20 666c 7578 0a20 2020 2020  ation flux.     
+00010200: 2020 2020 2020 2061 626f 7665 207b 7468         above {th
+00010210: 7265 7368 7d20 7468 7265 7368 6f6c 642e  resh} threshold.
+00010220: 0a0a 2020 2020 2020 2020 4e6f 7465 730a  ..        Notes.
+00010230: 2020 2020 2020 2020 2d2d 2d2d 2d0a 2020          -----.  
+00010240: 2020 2020 2020 466f 7220 6d6f 7265 2069        For more i
+00010250: 6e66 6f72 6d61 7469 6f6e 206f 6e20 7468  nformation on th
+00010260: 6520 696e 7075 7420 7061 7261 6d65 7465  e input paramete
+00010270: 7273 2073 6565 3a0a 2020 2020 2020 2020  rs see:.        
+00010280: 2020 2020 6874 7470 733a 2f2f 7863 6c69      https://xcli
+00010290: 6d2e 7265 6164 7468 6564 6f63 732e 696f  m.readthedocs.io
+000102a0: 2f65 6e2f 7374 6162 6c65 2f61 7069 2e68  /en/stable/api.h
+000102b0: 746d 6c23 7863 6c69 6d2e 696e 6469 6361  tml#xclim.indica
+000102c0: 746f 7273 2e61 746d 6f73 2e64 6179 735f  tors.atmos.days_
+000102d0: 7769 7468 5f73 6e6f 770a 2020 2020 2020  with_snow.      
+000102e0: 2020 2222 220a 2020 2020 2020 2020 7468    """.        th
+000102f0: 7265 7368 203d 205f 7468 7265 7368 5f73  resh = _thresh_s
+00010300: 7472 696e 6728 7468 7265 7368 2c20 226d  tring(thresh, "m
+00010310: 6d2f 6461 7922 290a 2020 2020 2020 2020  m/day").        
+00010320: 7265 7475 726e 2078 632e 6174 6d6f 732e  return xc.atmos.
+00010330: 6461 7973 5f77 6974 685f 736e 6f77 280a  days_with_snow(.
+00010340: 2020 2020 2020 2020 2020 2020 6c6f 773d              low=
+00010350: 7468 7265 7368 2c0a 2020 2020 2020 2020  thresh,.        
+00010360: 2020 2020 2a2a 7061 7261 6d73 2c0a 2020      **params,.  
+00010370: 2020 2020 2020 290a 0a0a 636c 6173 7320        )...class 
+00010380: 5343 443a 0a20 2020 2022 2222 536e 6f77  SCD:.    """Snow
+00010390: 2063 6f76 6572 2064 7572 6174 696f 6e2e   cover duration.
+000103a0: 2222 220a 0a20 2020 2074 6872 6573 6820  """..    thresh 
+000103b0: 3d20 310a 2020 2020 7761 7465 725f 6571  = 1.    water_eq
+000103c0: 7569 7661 6c65 6e74 203d 2046 616c 7365  uivalent = False
+000103d0: 0a0a 2020 2020 6465 6620 636f 6d70 7574  ..    def comput
+000103e0: 6528 7468 7265 7368 3d74 6872 6573 682c  e(thresh=thresh,
+000103f0: 2077 6174 6572 5f65 7175 6976 616c 656e   water_equivalen
+00010400: 743d 7761 7465 725f 6571 7569 7661 6c65  t=water_equivale
+00010410: 6e74 2c20 2a2a 7061 7261 6d73 293a 0a20  nt, **params):. 
+00010420: 2020 2020 2020 2022 2222 4361 6c63 756c         """Calcul
+00010430: 6174 6520 736e 6f77 2063 6f76 6572 2064  ate snow cover d
+00010440: 7572 6174 696f 6e2e 0a0a 2020 2020 2020  uration...      
+00010450: 2020 5061 7261 6d65 7465 7273 0a20 2020    Parameters.   
+00010460: 2020 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a       ----------.
+00010470: 2020 2020 2020 2020 7468 7265 7368 3a20          thresh: 
+00010480: 696e 7420 6f72 2073 7472 696e 670a 2020  int or string.  
+00010490: 2020 2020 2020 2020 2020 5468 7265 7368            Thresh
+000104a0: 6f6c 6420 736e 6f77 2074 6869 636b 6e65  old snow thickne
+000104b0: 7373 2061 626f 7665 2077 6869 6368 2061  ss above which a
+000104c0: 2064 6179 2069 7320 636f 6e73 6964 6572   day is consider
+000104d0: 6564 0a20 2020 2020 2020 2020 2020 2061  ed.            a
+000104e0: 7320 6120 736e 6f77 2064 6179 2028 6465  s a snow day (de
+000104f0: 6661 756c 743a 2031 2063 6d29 2e0a 2020  fault: 1 cm)..  
+00010500: 2020 2020 2020 2020 2020 4966 2074 7970            If typ
+00010510: 6520 6f66 2074 6872 6573 686f 6c64 2069  e of threshold i
+00010520: 7320 616e 2069 6e74 6567 6572 2074 6865  s an integer the
+00010530: 2075 6e69 7420 6973 2073 6574 2074 6f20   unit is set to 
+00010540: 636d 2e0a 0a20 2020 2020 2020 2052 6574  cm...        Ret
+00010550: 7572 6e73 0a20 2020 2020 2020 202d 2d2d  urns.        ---
+00010560: 2d2d 2d2d 0a20 2020 2020 2020 2078 6172  ----.        xar
+00010570: 7261 792e 4461 7461 4172 7261 790a 2020  ray.DataArray.  
+00010580: 2020 2020 2020 2020 2020 4e75 6d62 6572            Number
+00010590: 206f 6620 6461 7973 2077 6974 6820 736e   of days with sn
+000105a0: 6f77 2063 6f76 6572 2061 626f 7665 207b  ow cover above {
+000105b0: 7468 7265 7368 7d20 7468 7265 7368 6f6c  thresh} threshol
+000105c0: 642e 0a0a 2020 2020 2020 2020 4e6f 7465  d...        Note
+000105d0: 730a 2020 2020 2020 2020 2d2d 2d2d 2d0a  s.        -----.
+000105e0: 2020 2020 2020 2020 466f 7220 6d6f 7265          For more
+000105f0: 2069 6e66 6f72 6d61 7469 6f6e 206f 6e20   information on 
+00010600: 7468 6520 696e 7075 7420 7061 7261 6d65  the input parame
+00010610: 7465 7273 2073 6565 3a0a 2020 2020 2020  ters see:.      
+00010620: 2020 2020 2020 6874 7470 733a 2f2f 7863        https://xc
+00010630: 6c69 6d2e 7265 6164 7468 6564 6f63 732e  lim.readthedocs.
+00010640: 696f 2f65 6e2f 7374 6162 6c65 2f61 7069  io/en/stable/api
+00010650: 2e68 746d 6c23 7863 6c69 6d2e 696e 6469  .html#xclim.indi
+00010660: 6361 746f 7273 2e6c 616e 642e 736e 6f77  cators.land.snow
+00010670: 5f63 6f76 6572 5f64 7572 6174 696f 6e0a  _cover_duration.
+00010680: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00010690: 2020 2020 6966 2077 6174 6572 5f65 7175      if water_equ
+000106a0: 6976 616c 656e 7420 6973 2054 7275 653a  ivalent is True:
+000106b0: 0a20 2020 2020 2020 2020 2020 2073 6e77  .            snw
+000106c0: 203d 2078 632e 6c61 6e64 2e73 6e64 5f74   = xc.land.snd_t
+000106d0: 6f5f 736e 7728 0a20 2020 2020 2020 2020  o_snw(.         
+000106e0: 2020 2020 2020 2073 6e64 3d70 6172 616d         snd=param
+000106f0: 735b 2264 7322 5d5b 2273 6e64 225d 2c0a  s["ds"]["snd"],.
+00010700: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010710: 636f 6e73 743d 2231 3030 3020 6b67 206d  const="1000 kg m
+00010720: 2d33 222c 0a20 2020 2020 2020 2020 2020  -3",.           
+00010730: 2029 0a20 2020 2020 2020 2020 2020 2073   ).            s
+00010740: 6e64 203d 2078 632e 6c61 6e64 2e73 6e77  nd = xc.land.snw
+00010750: 5f74 6f5f 736e 6428 736e 773d 736e 772c  _to_snd(snw=snw,
+00010760: 2073 6e72 3d70 6172 616d 735b 2264 7322   snr=params["ds"
+00010770: 5d5b 2273 6e72 225d 290a 2020 2020 2020  ]["snr"]).      
+00010780: 2020 2020 2020 7061 7261 6d73 5b22 6473        params["ds
+00010790: 225d 5b22 736e 6422 5d20 3d20 736e 640a  "]["snd"] = snd.
+000107a0: 2020 2020 2020 2020 7468 7265 7368 203d          thresh =
+000107b0: 205f 7468 7265 7368 5f73 7472 696e 6728   _thresh_string(
+000107c0: 7468 7265 7368 2c20 2263 6d22 290a 2020  thresh, "cm").  
+000107d0: 2020 2020 2020 7265 7475 726e 2078 632e        return xc.
+000107e0: 6c61 6e64 2e73 6e64 5f73 6561 736f 6e5f  land.snd_season_
+000107f0: 6c65 6e67 7468 280a 2020 2020 2020 2020  length(.        
+00010800: 2020 2020 7468 7265 7368 3d74 6872 6573      thresh=thres
+00010810: 682c 0a20 2020 2020 2020 2020 2020 202a  h,.            *
+00010820: 2a70 6172 616d 732c 0a20 2020 2020 2020  *params,.       
+00010830: 2029 0a0a 0a63 6c61 7373 2053 696e 743a   )...class Sint:
+00010840: 0a20 2020 2022 2222 536e 6f77 6661 6c6c  .    """Snowfall
+00010850: 2069 6e74 656e 7369 7479 2e22 2222 0a0a   intensity."""..
+00010860: 2020 2020 7468 7265 7368 203d 2031 0a0a      thresh = 1..
+00010870: 2020 2020 6465 6620 636f 6d70 7574 6528      def compute(
+00010880: 7468 7265 7368 3d74 6872 6573 682c 202a  thresh=thresh, *
+00010890: 2a70 6172 616d 7329 3a0a 2020 2020 2020  *params):.      
+000108a0: 2020 2222 2243 616c 6375 6c61 7465 2073    """Calculate s
+000108b0: 6e6f 7766 616c 6c20 696e 7465 6e73 6974  nowfall intensit
+000108c0: 792e 0a0a 2020 2020 2020 2020 5061 7261  y...        Para
+000108d0: 6d65 7465 7273 0a20 2020 2020 2020 202d  meters.        -
+000108e0: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 2020  ---------.      
+000108f0: 2020 7468 7265 7368 3a20 696e 7420 6f72    thresh: int or
+00010900: 2073 7472 696e 670a 2020 2020 2020 2020   string.        
+00010910: 2020 2020 4c69 7175 6964 2077 6174 6572      Liquid water
+00010920: 2065 7175 6976 616c 656e 7420 736e 6f77   equivalent snow
+00010930: 6661 6c6c 2072 6174 6520 6162 6f76 6520  fall rate above 
+00010940: 7768 6963 6820 6120 6461 7920 6973 0a20  which a day is. 
+00010950: 2020 2020 2020 2020 2020 2063 6f6e 7369             consi
+00010960: 6465 7265 6420 6173 2061 2073 6e6f 7720  dered as a snow 
+00010970: 6461 7920 2864 6566 6175 6c74 3a20 3120  day (default: 1 
+00010980: 6d6d 2f64 6179 2920 2e0a 2020 2020 2020  mm/day) ..      
+00010990: 2020 2020 2020 4966 2074 7970 6520 6f66        If type of
+000109a0: 2074 6872 6573 686f 6c64 2069 7320 616e   threshold is an
+000109b0: 2069 6e74 6567 6572 2074 6865 2075 6e69   integer the uni
+000109c0: 7420 6973 2073 6574 2074 6f20 6d6d 2f64  t is set to mm/d
+000109d0: 6179 2e0a 0a20 2020 2020 2020 2052 6574  ay...        Ret
+000109e0: 7572 6e73 0a20 2020 2020 2020 202d 2d2d  urns.        ---
+000109f0: 2d2d 2d2d 0a20 2020 2020 2020 2078 6172  ----.        xar
+00010a00: 7261 792e 4461 7461 4172 7261 790a 2020  ray.DataArray.  
+00010a10: 2020 2020 2020 2020 2020 4d65 616e 2064            Mean d
+00010a20: 6169 6c79 2073 6e6f 7766 616c 6c20 6475  aily snowfall du
+00010a30: 7269 6e67 2064 6179 7320 7769 7468 2073  ring days with s
+00010a40: 6e6f 7766 616c 6c20 3e20 7b74 6872 6573  nowfall > {thres
+00010a50: 687d 2e0a 0a20 2020 2020 2020 204e 6f74  h}...        Not
+00010a60: 6573 0a20 2020 2020 2020 202d 2d2d 2d2d  es.        -----
+00010a70: 0a20 2020 2020 2020 2046 6f72 206d 6f72  .        For mor
+00010a80: 6520 696e 666f 726d 6174 696f 6e20 6f6e  e information on
+00010a90: 2074 6865 2069 6e70 7574 2070 6172 616d   the input param
+00010aa0: 6574 6572 7320 7365 653a 0a20 2020 2020  eters see:.     
+00010ab0: 2020 2020 2020 2068 7474 7073 3a2f 2f78         https://x
+00010ac0: 636c 696d 2e72 6561 6474 6865 646f 6373  clim.readthedocs
+00010ad0: 2e69 6f2f 656e 2f73 7461 626c 652f 6170  .io/en/stable/ap
+00010ae0: 692e 6874 6d6c 2378 636c 696d 2e69 6e64  i.html#xclim.ind
+00010af0: 6963 6174 6f72 732e 6174 6d6f 732e 736e  icators.atmos.sn
+00010b00: 6f77 6661 6c6c 5f69 6e74 656e 7369 7479  owfall_intensity
+00010b10: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00010b20: 2020 2020 2074 6872 6573 6820 3d20 5f74       thresh = _t
+00010b30: 6872 6573 685f 7374 7269 6e67 2874 6872  hresh_string(thr
+00010b40: 6573 682c 2022 6d6d 2f64 6179 2229 0a20  esh, "mm/day"). 
+00010b50: 2020 2020 2020 2072 6574 7572 6e20 7863         return xc
+00010b60: 2e61 746d 6f73 2e73 6e6f 7766 616c 6c5f  .atmos.snowfall_
+00010b70: 696e 7465 6e73 6974 7928 0a20 2020 2020  intensity(.     
+00010b80: 2020 2020 2020 2074 6872 6573 683d 7468         thresh=th
+00010b90: 7265 7368 2c0a 2020 2020 2020 2020 2020  resh,.          
+00010ba0: 2020 2a2a 7061 7261 6d73 2c0a 2020 2020    **params,.    
+00010bb0: 2020 2020 290a 0a0a 636c 6173 7320 5366      )...class Sf
+00010bc0: 7265 713a 0a20 2020 2022 2222 536e 6f77  req:.    """Snow
+00010bd0: 6661 6c6c 2066 7265 7175 656e 6379 2e22  fall frequency."
+00010be0: 2222 0a0a 2020 2020 7468 7265 7368 203d  ""..    thresh =
+00010bf0: 2031 0a0a 2020 2020 6465 6620 636f 6d70   1..    def comp
+00010c00: 7574 6528 7468 7265 7368 3d74 6872 6573  ute(thresh=thres
+00010c10: 682c 202a 2a70 6172 616d 7329 3a0a 2020  h, **params):.  
+00010c20: 2020 2020 2020 2222 2243 616c 6375 6c61        """Calcula
+00010c30: 7465 2073 6e6f 7766 616c 6c20 6672 6571  te snowfall freq
+00010c40: 7565 6e63 792e 0a0a 2020 2020 2020 2020  uency...        
+00010c50: 5061 7261 6d65 7465 7273 0a20 2020 2020  Parameters.     
+00010c60: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020     ----------.  
+00010c70: 2020 2020 2020 7468 7265 7368 3a20 696e        thresh: in
+00010c80: 7420 6f72 2073 7472 696e 670a 2020 2020  t or string.    
+00010c90: 2020 2020 2020 2020 4c69 7175 6964 2077          Liquid w
+00010ca0: 6174 6572 2065 7175 6976 616c 656e 7420  ater equivalent 
+00010cb0: 736e 6f77 6661 6c6c 2072 6174 6520 6162  snowfall rate ab
+00010cc0: 6f76 6520 7768 6963 6820 6120 6461 7920  ove which a day 
+00010cd0: 6973 0a20 2020 2020 2020 2020 2020 2063  is.            c
+00010ce0: 6f6e 7369 6465 7265 6420 6173 2061 2073  onsidered as a s
+00010cf0: 6e6f 7720 6461 7920 2864 6566 6175 6c74  now day (default
+00010d00: 3a20 3120 6d6d 2f64 6179 2920 2e0a 2020  : 1 mm/day) ..  
+00010d10: 2020 2020 2020 2020 2020 4966 2074 7970            If typ
+00010d20: 6520 6f66 2074 6872 6573 686f 6c64 2069  e of threshold i
+00010d30: 7320 616e 2069 6e74 6567 6572 2074 6865  s an integer the
+00010d40: 2075 6e69 7420 6973 2073 6574 2074 6f20   unit is set to 
+00010d50: 6d6d 2f64 6179 2e0a 0a20 2020 2020 2020  mm/day...       
+00010d60: 2052 6574 7572 6e73 0a20 2020 2020 2020   Returns.       
+00010d70: 202d 2d2d 2d2d 2d2d 0a20 2020 2020 2020   -------.       
+00010d80: 2078 6172 7261 792e 4461 7461 4172 7261   xarray.DataArra
+00010d90: 790a 2020 2020 2020 2020 2020 2020 5065  y.            Pe
+00010da0: 7263 656e 7461 6765 206f 6620 6461 7973  rcentage of days
+00010db0: 2077 6974 6820 736e 6f77 6661 6c6c 203e   with snowfall >
+00010dc0: 207b 7468 7265 7368 7d2e 0a0a 2020 2020   {thresh}...    
+00010dd0: 2020 2020 4e6f 7465 730a 2020 2020 2020      Notes.      
+00010de0: 2020 2d2d 2d2d 2d0a 2020 2020 2020 2020    -----.        
+00010df0: 466f 7220 6d6f 7265 2069 6e66 6f72 6d61  For more informa
+00010e00: 7469 6f6e 206f 6e20 7468 6520 696e 7075  tion on the inpu
+00010e10: 7420 7061 7261 6d65 7465 7273 2073 6565  t parameters see
+00010e20: 3a0a 2020 2020 2020 2020 2020 2020 6874  :.            ht
+00010e30: 7470 733a 2f2f 7863 6c69 6d2e 7265 6164  tps://xclim.read
+00010e40: 7468 6564 6f63 732e 696f 2f65 6e2f 7374  thedocs.io/en/st
+00010e50: 6162 6c65 2f61 7069 2e68 746d 6c23 7863  able/api.html#xc
+00010e60: 6c69 6d2e 696e 6469 6361 746f 7273 2e61  lim.indicators.a
+00010e70: 746d 6f73 2e73 6e6f 7766 616c 6c5f 6672  tmos.snowfall_fr
+00010e80: 6571 7565 6e63 790a 2020 2020 2020 2020  equency.        
+00010e90: 2222 220a 2020 2020 2020 2020 7468 7265  """.        thre
+00010ea0: 7368 203d 205f 7468 7265 7368 5f73 7472  sh = _thresh_str
+00010eb0: 696e 6728 7468 7265 7368 2c20 226d 6d2f  ing(thresh, "mm/
+00010ec0: 6461 7922 290a 2020 2020 2020 2020 7265  day").        re
+00010ed0: 7475 726e 2078 632e 6174 6d6f 732e 736e  turn xc.atmos.sn
+00010ee0: 6f77 6661 6c6c 5f66 7265 7175 656e 6379  owfall_frequency
+00010ef0: 280a 2020 2020 2020 2020 2020 2020 7468  (.            th
+00010f00: 7265 7368 3d74 6872 6573 682c 0a20 2020  resh=thresh,.   
+00010f10: 2020 2020 2020 2020 202a 2a70 6172 616d           **param
+00010f20: 732c 0a20 2020 2020 2020 2029 0a0a 0a63  s,.        )...c
+00010f30: 6c61 7373 2055 5443 493a 0a20 2020 2022  lass UTCI:.    "
+00010f40: 2222 556e 6976 6572 7361 6c20 7468 6572  ""Universal ther
+00010f50: 6d61 6c20 636c 696d 6174 6520 696e 6465  mal climate inde
+00010f60: 782e 2222 220a 0a20 2020 2073 7461 7420  x."""..    stat 
+00010f70: 3d20 2261 7665 7261 6765 220a 2020 2020  = "average".    
+00010f80: 6d61 736b 5f69 6e76 616c 6964 203d 2054  mask_invalid = T
+00010f90: 7275 650a 0a20 2020 2064 6566 2063 6f6d  rue..    def com
+00010fa0: 7075 7465 2873 7461 743d 7374 6174 2c20  pute(stat=stat, 
+00010fb0: 6d61 736b 5f69 6e76 616c 6964 3d6d 6173  mask_invalid=mas
+00010fc0: 6b5f 696e 7661 6c69 642c 202a 2a70 6172  k_invalid, **par
+00010fd0: 616d 7329 3a0a 2020 2020 2020 2020 2222  ams):.        ""
+00010fe0: 2243 616c 6375 6c61 7465 2075 6e69 7665  "Calculate unive
+00010ff0: 7273 616c 2074 6865 726d 616c 2063 6c69  rsal thermal cli
+00011000: 6d61 7465 2069 6e64 6578 2e0a 0a20 2020  mate index...   
+00011010: 2020 2020 2050 6172 616d 6574 6572 730a       Parameters.
+00011020: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d2d          --------
+00011030: 2d2d 0a20 2020 2020 2020 2073 7461 743a  --.        stat:
+00011040: 207b e280 9861 7665 7261 6765 e280 992c   {...average...,
+00011050: 20e2 8098 7375 6e6c 6974 e280 992c 20e2   ...sunlit..., .
+00011060: 8098 696e 7374 616e 74e2 8099 7d0a 2020  ..instant...}.  
+00011070: 2020 2020 2020 2020 2020 5768 6963 6820            Which 
+00011080: 7374 6174 6973 7469 6320 746f 2061 7070  statistic to app
+00011090: 6c79 2e20 4966 20e2 809c 6176 6572 6167  ly. If ...averag
+000110a0: 65e2 809d 2c20 7468 6520 6176 6572 6167  e..., the averag
+000110b0: 6520 6f66 2074 6865 2063 6f73 696e 650a  e of the cosine.
+000110c0: 2020 2020 2020 2020 2020 2020 6f66 2074              of t
+000110d0: 6865 2073 6f6c 6172 207a 656e 6974 6820  he solar zenith 
+000110e0: 616e 676c 6520 6973 2063 616c 6375 6c61  angle is calcula
+000110f0: 7465 642e 0a20 2020 2020 2020 2020 2020  ted..           
+00011100: 2049 6620 e280 9c69 6e73 7461 6e74 e280   If ...instant..
+00011110: 9d2c 2074 6865 2069 6e73 7461 6e74 616e  ., the instantan
+00011120: 656f 7573 2063 6f73 696e 6520 6f66 2074  eous cosine of t
+00011130: 6865 2073 6f6c 6172 207a 656e 6974 6820  he solar zenith 
+00011140: 616e 676c 6520 6973 0a20 2020 2020 2020  angle is.       
+00011150: 2020 2020 2063 616c 6375 6c61 7465 642e       calculated.
+00011160: 0a20 2020 2020 2020 2020 2020 2049 6620  .            If 
+00011170: e280 9c73 756e 6c69 74e2 809d 2c20 7468  ...sunlit..., th
+00011180: 6520 636f 7369 6e65 206f 6620 7468 6520  e cosine of the 
+00011190: 736f 6c61 7220 7a65 6e69 7468 2061 6e67  solar zenith ang
+000111a0: 6c65 2069 7320 6361 6c63 756c 6174 6564  le is calculated
+000111b0: 0a20 2020 2020 2020 2020 2020 2064 7572  .            dur
+000111c0: 696e 6720 7468 6520 7375 6e6c 6974 2070  ing the sunlit p
+000111d0: 6572 696f 6420 6f66 2065 6163 6820 696e  eriod of each in
+000111e0: 7465 7276 616c 2e0a 2020 2020 2020 2020  terval..        
+000111f0: 2020 2020 4966 20e2 809c 696e 7374 616e      If ...instan
+00011200: 74e2 809d 2c20 7468 6520 696e 7374 616e  t..., the instan
+00011210: 7461 6e65 6f75 7320 636f 7369 6e65 206f  taneous cosine o
+00011220: 6620 7468 6520 736f 6c61 7220 7a65 6e69  f the solar zeni
+00011230: 7468 2061 6e67 6c65 2069 730a 2020 2020  th angle is.    
+00011240: 2020 2020 2020 2020 6361 6c63 756c 6174          calculat
+00011250: 6564 2e0a 2020 2020 2020 2020 2020 2020  ed..            
+00011260: 5468 6973 2069 7320 6e65 6365 7373 6172  This is necessar
+00011270: 7920 6966 206d 7274 2069 7320 6e6f 7420  y if mrt is not 
+00011280: 4e6f 6e65 2028 6465 6661 756c 743a 2061  None (default: a
+00011290: 7665 7261 6765 292e 0a20 2020 2020 2020  verage)..       
+000112a0: 206d 6173 6b5f 7661 6c69 643a 2062 6f6f   mask_valid: boo
+000112b0: 6c0a 2020 2020 2020 2020 2020 2020 4966  l.            If
+000112c0: 2054 7275 652c 2055 5443 4920 7661 6c75   True, UTCI valu
+000112d0: 6573 2061 7265 204e 614e 2077 6865 7265  es are NaN where
+000112e0: 2061 6e79 206f 6620 7468 6520 696e 7075   any of the inpu
+000112f0: 7473 2061 7265 206f 7574 7369 6465 0a20  ts are outside. 
+00011300: 2020 2020 2020 2020 2020 2074 6865 6972             their
+00011310: 2076 616c 6964 6974 7920 7261 6e67 6573   validity ranges
+00011320: 3a0a 2020 2020 2020 2020 2020 2020 2d35  :.            -5
+00011330: 30c2 b043 203c 2074 6173 203c 2035 30c2  0..C < tas < 50.
+00011340: b043 2c0a 2020 2020 2020 2020 2020 2020  .C,.            
+00011350: 2d33 30c2 b043 203c 2074 6173 202d 206d  -30..C < tas - m
+00011360: 7274 203c 2033 30c2 b043 0a20 2020 2020  rt < 30..C.     
+00011370: 2020 2020 2020 2030 2e35 206d 2f73 203c         0.5 m/s <
+00011380: 2073 6663 5769 6e64 203c 2031 372e 3020   sfcWind < 17.0 
+00011390: 6d2f 730a 2020 2020 2020 2020 2020 2020  m/s.            
+000113a0: 2864 6566 6175 6c74 3a20 5472 7565 292e  (default: True).
+000113b0: 0a0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
+000113c0: 730a 2020 2020 2020 2020 2d2d 2d2d 2d2d  s.        ------
+000113d0: 2d0a 2020 2020 2020 2020 7861 7272 6179  -.        xarray
+000113e0: 2e44 6174 6141 7272 6179 0a20 2020 2020  .DataArray.     
+000113f0: 2020 2020 2020 2055 6e69 7665 7273 616c         Universal
+00011400: 2054 6865 726d 616c 2043 6c69 6d61 7465   Thermal Climate
+00011410: 2049 6e64 6578 2e0a 0a20 2020 2020 2020   Index...       
+00011420: 204e 6f74 6573 0a20 2020 2020 2020 202d   Notes.        -
+00011430: 2d2d 2d2d 0a20 2020 2020 2020 2046 6f72  ----.        For
+00011440: 206d 6f72 6520 696e 666f 726d 6174 696f   more informatio
+00011450: 6e20 6f6e 2074 6865 2069 6e70 7574 2070  n on the input p
+00011460: 6172 616d 6574 6572 7320 7365 653a 0a20  arameters see:. 
+00011470: 2020 2020 2020 2020 2020 2068 7474 7073             https
+00011480: 3a2f 2f78 636c 696d 2e72 6561 6474 6865  ://xclim.readthe
+00011490: 646f 6373 2e69 6f2f 656e 2f73 7461 626c  docs.io/en/stabl
+000114a0: 652f 6170 692e 6874 6d6c 2378 636c 696d  e/api.html#xclim
+000114b0: 2e69 6e64 6963 6174 6f72 732e 6174 6d6f  .indicators.atmo
+000114c0: 732e 756e 6976 6572 7361 6c5f 7468 6572  s.universal_ther
+000114d0: 6d61 6c5f 636c 696d 6174 655f 696e 6465  mal_climate_inde
+000114e0: 780a 2020 2020 2020 2020 2222 220a 2020  x.        """.  
+000114f0: 2020 2020 2020 7265 7475 726e 2078 632e        return xc.
+00011500: 6174 6d6f 732e 756e 6976 6572 7361 6c5f  atmos.universal_
+00011510: 7468 6572 6d61 6c5f 636c 696d 6174 655f  thermal_climate_
+00011520: 696e 6465 7828 0a20 2020 2020 2020 2020  index(.         
+00011530: 2020 2073 7461 743d 7374 6174 2c0a 2020     stat=stat,.  
+00011540: 2020 2020 2020 2020 2020 6d61 736b 5f69            mask_i
+00011550: 6e76 616c 6964 3d6d 6173 6b5f 696e 7661  nvalid=mask_inva
+00011560: 6c69 642c 0a20 2020 2020 2020 2020 2020  lid,.           
+00011570: 202a 2a70 6172 616d 732c 0a20 2020 2020   **params,.     
+00011580: 2020 2029 0a0a 0a63 6c61 7373 2057 493a     )...class WI:
+00011590: 0a20 2020 2022 2222 4e75 6d62 6572 206f  .    """Number o
+000115a0: 6620 7769 6e74 6572 2064 6179 7320 2874  f winter days (t
+000115b0: 6173 6d69 6e29 2e22 2222 0a0a 2020 2020  asmin)."""..    
+000115c0: 7468 7265 7368 203d 202d 3130 0a0a 2020  thresh = -10..  
+000115d0: 2020 6465 6620 636f 6d70 7574 6528 7468    def compute(th
+000115e0: 7265 7368 3d74 6872 6573 682c 202a 2a70  resh=thresh, **p
+000115f0: 6172 616d 7329 3a0a 2020 2020 2020 2020  arams):.        
+00011600: 2222 2243 616c 6375 6c61 7465 206e 756d  """Calculate num
+00011610: 6265 7220 6f66 2077 696e 7465 7220 6461  ber of winter da
+00011620: 7973 2e0a 0a20 2020 2020 2020 2050 6172  ys...        Par
+00011630: 616d 6574 6572 730a 2020 2020 2020 2020  ameters.        
+00011640: 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020  ----------.     
+00011650: 2020 2074 6872 6573 683a 2069 6e74 206f     thresh: int o
+00011660: 7220 7374 7269 6e67 0a20 2020 2020 2020  r string.       
+00011670: 2020 2020 2054 6872 6573 686f 6c64 206d       Threshold m
+00011680: 696e 696d 756d 2074 656d 7065 7261 7475  inimum temperatu
+00011690: 7265 2062 656c 6f77 2077 6869 6368 2061  re below which a
+000116a0: 2064 6179 2069 7320 636f 6e73 6964 6572   day is consider
+000116b0: 6564 0a20 2020 2020 2020 2020 2020 2061  ed.            a
+000116c0: 7320 6120 7769 6e74 6572 2064 6179 2028  s a winter day (
+000116d0: 6465 6661 756c 743a 202d 3130 2064 6567  default: -10 deg
+000116e0: 4329 2e0a 2020 2020 2020 2020 2020 2020  C)..            
+000116f0: 4966 2074 7970 6520 6f66 2074 6872 6573  If type of thres
+00011700: 686f 6c64 2069 7320 616e 2069 6e74 6567  hold is an integ
+00011710: 6572 2074 6865 2075 6e69 7420 6973 2073  er the unit is s
+00011720: 6574 2074 6f20 6465 6743 2e0a 0a20 2020  et to degC...   
+00011730: 2020 2020 2052 6574 7572 6e73 0a20 2020       Returns.   
+00011740: 2020 2020 202d 2d2d 2d2d 2d2d 0a20 2020       -------.   
+00011750: 2020 2020 2078 6172 7261 792e 4461 7461       xarray.Data
+00011760: 4172 7261 790a 2020 2020 2020 2020 2020  Array.          
+00011770: 2020 4e75 6d62 6572 206f 6620 7769 6e74    Number of wint
+00011780: 6572 2064 6179 732e 0a0a 2020 2020 2020  er days...      
+00011790: 2020 4e6f 7465 730a 2020 2020 2020 2020    Notes.        
+000117a0: 2d2d 2d2d 2d0a 2020 2020 2020 2020 466f  -----.        Fo
+000117b0: 7220 6d6f 7265 2069 6e66 6f72 6d61 7469  r more informati
+000117c0: 6f6e 206f 6e20 7468 6520 696e 7075 7420  on on the input 
+000117d0: 7061 7261 6d65 7465 7273 2073 6565 3a0a  parameters see:.
+000117e0: 2020 2020 2020 2020 2020 2020 6874 7470              http
+000117f0: 733a 2f2f 7863 6c69 6d2e 7265 6164 7468  s://xclim.readth
+00011800: 6564 6f63 732e 696f 2f65 6e2f 7374 6162  edocs.io/en/stab
+00011810: 6c65 2f61 7069 2e68 746d 6c23 7863 6c69  le/api.html#xcli
+00011820: 6d2e 696e 6469 6361 746f 7273 2e61 746d  m.indicators.atm
+00011830: 6f73 2e74 6e5f 6461 7973 5f62 656c 6f77  os.tn_days_below
+00011840: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00011850: 2020 2020 2074 6872 6573 6820 3d20 5f74       thresh = _t
+00011860: 6872 6573 685f 7374 7269 6e67 2874 6872  hresh_string(thr
+00011870: 6573 682c 2022 6465 6743 2229 0a20 2020  esh, "degC").   
+00011880: 2020 2020 2072 6574 7572 6e20 7863 2e61       return xc.a
+00011890: 746d 6f73 2e74 6e5f 6461 7973 5f62 656c  tmos.tn_days_bel
+000118a0: 6f77 280a 2020 2020 2020 2020 2020 2020  ow(.            
+000118b0: 7468 7265 7368 3d74 6872 6573 682c 0a20  thresh=thresh,. 
+000118c0: 2020 2020 2020 2020 2020 202a 2a70 6172             **par
+000118d0: 616d 732c 0a20 2020 2020 2020 2029 0a0a  ams,.        )..
+000118e0: 0a63 6c61 7373 2048 5766 3a0a 2020 2020  .class HWf:.    
+000118f0: 2222 224e 756d 6265 7220 6f66 2068 6561  """Number of hea
+00011900: 7420 7761 7665 7320 2874 6173 6d61 782c  t waves (tasmax,
+00011910: 2074 6173 6d69 6e29 2e22 2222 0a0a 2020   tasmin)."""..  
+00011920: 2020 7468 7265 7368 5f74 6173 6d69 6e20    thresh_tasmin 
+00011930: 3d20 3232 0a20 2020 2074 6872 6573 685f  = 22.    thresh_
+00011940: 7461 736d 6178 203d 2033 300a 2020 2020  tasmax = 30.    
+00011950: 7769 6e64 6f77 203d 2033 0a0a 2020 2020  window = 3..    
+00011960: 6465 6620 636f 6d70 7574 6528 0a20 2020  def compute(.   
+00011970: 2020 2020 2074 6872 6573 685f 7461 736d       thresh_tasm
+00011980: 696e 3d74 6872 6573 685f 7461 736d 696e  in=thresh_tasmin
+00011990: 2c0a 2020 2020 2020 2020 7468 7265 7368  ,.        thresh
+000119a0: 5f74 6173 6d61 783d 7468 7265 7368 5f74  _tasmax=thresh_t
+000119b0: 6173 6d61 782c 0a20 2020 2020 2020 2077  asmax,.        w
+000119c0: 696e 646f 773d 7769 6e64 6f77 2c0a 2020  indow=window,.  
+000119d0: 2020 2020 2020 2a2a 7061 7261 6d73 2c0a        **params,.
+000119e0: 2020 2020 293a 0a20 2020 2020 2020 2022      ):.        "
+000119f0: 2222 4361 6c63 756c 6174 6520 6e75 6d62  ""Calculate numb
+00011a00: 6572 206f 6620 6865 6174 2077 6176 6573  er of heat waves
+00011a10: 2e0a 0a20 2020 2020 2020 2050 6172 616d  ...        Param
+00011a20: 6574 6572 730a 2020 2020 2020 2020 2d2d  eters.        --
+00011a30: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020 2020  --------.       
+00011a40: 2074 6872 6573 685f 7461 736d 696e 3a20   thresh_tasmin: 
+00011a50: 696e 7420 6f72 2073 7472 696e 670a 2020  int or string.  
+00011a60: 2020 2020 2020 2020 2020 5468 7265 7368            Thresh
+00011a70: 6f6c 6420 6d69 6e69 6d75 6d20 7465 6d70  old minimum temp
+00011a80: 6572 6174 7572 6520 6162 6f76 6520 7768  erature above wh
+00011a90: 6963 6820 6120 6461 7920 6973 2063 6f6e  ich a day is con
+00011aa0: 7369 6465 7265 640a 2020 2020 2020 2020  sidered.        
+00011ab0: 2020 2020 6173 2061 2068 6561 7420 6461      as a heat da
+00011ac0: 7920 2864 6566 6175 6c74 3a20 3232 2064  y (default: 22 d
+00011ad0: 6567 4329 2e0a 2020 2020 2020 2020 2020  egC)..          
+00011ae0: 2020 4966 2074 7970 6520 6f66 2074 6872    If type of thr
+00011af0: 6573 686f 6c64 2069 7320 616e 2069 6e74  eshold is an int
+00011b00: 6567 6572 2074 6865 2075 6e69 7420 6973  eger the unit is
+00011b10: 2073 6574 2074 6f20 6465 6743 2e0a 2020   set to degC..  
+00011b20: 2020 2020 2020 7468 7265 7368 5f74 6173        thresh_tas
+00011b30: 6d61 783a 2069 6e74 206f 7220 7374 7269  max: int or stri
+00011b40: 6e67 0a20 2020 2020 2020 2020 2020 2054  ng.            T
+00011b50: 6872 6573 686f 6c64 206d 6178 696d 756d  hreshold maximum
+00011b60: 2074 656d 7065 7261 7475 7265 2061 626f   temperature abo
+00011b70: 7665 2077 6869 6368 2061 2064 6179 2069  ve which a day i
+00011b80: 7320 636f 6e73 6964 6572 6564 0a20 2020  s considered.   
+00011b90: 2020 2020 2020 2020 2061 7320 6120 7769           as a wi
+00011ba0: 6e74 6572 2064 6179 2028 6465 6661 756c  nter day (defaul
+00011bb0: 743a 2033 3020 6465 6743 292e 0a20 2020  t: 30 degC)..   
+00011bc0: 2020 2020 2020 2020 2049 6620 7479 7065           If type
+00011bd0: 206f 6620 7468 7265 7368 6f6c 6420 6973   of threshold is
+00011be0: 2061 6e20 696e 7465 6765 7220 7468 6520   an integer the 
+00011bf0: 756e 6974 2069 7320 7365 7420 746f 2064  unit is set to d
+00011c00: 6567 432e 0a20 2020 2020 2020 2077 696e  egC..        win
+00011c10: 646f 773a 2069 6e74 0a20 2020 2020 2020  dow: int.       
+00011c20: 2020 2020 204d 696e 696d 756d 206e 756d       Minimum num
+00011c30: 6265 7220 6f66 2064 6179 7320 7769 7468  ber of days with
+00011c40: 2074 656d 7065 7261 7475 7265 2061 626f   temperature abo
+00011c50: 7665 2074 6872 6573 680a 2020 2020 2020  ve thresh.      
+00011c60: 2020 2020 2020 746f 2071 7561 6c69 6679        to qualify
+00011c70: 2061 7320 6120 686f 7420 7370 656c 6c20   as a hot spell 
+00011c80: 2864 6566 6175 6c74 3a20 3329 2e0a 0a20  (default: 3)... 
+00011c90: 2020 2020 2020 2052 6574 7572 6e73 0a20         Returns. 
+00011ca0: 2020 2020 2020 202d 2d2d 2d2d 2d2d 0a20         -------. 
+00011cb0: 2020 2020 2020 2078 6172 7261 792e 4461         xarray.Da
+00011cc0: 7461 4172 7261 790a 2020 2020 2020 2020  taArray.        
+00011cd0: 2020 2020 4e75 6d62 6572 206f 6620 6865      Number of he
+00011ce0: 6174 2077 6176 6573 206f 6620 6174 206c  at waves of at l
+00011cf0: 6561 7374 207b 7769 6e64 6f77 7d20 636f  east {window} co
+00011d00: 6e73 6563 7574 6976 6520 6461 7973 0a20  nsecutive days. 
+00011d10: 2020 2020 2020 2020 2020 2077 6974 6820             with 
+00011d20: 6d61 7869 6d75 6d20 7465 6d70 6572 6174  maximum temperat
+00011d30: 7572 6520 6162 6f76 6520 7b74 6872 6573  ure above {thres
+00011d40: 685f 7461 736d 6178 7d20 616e 640a 2020  h_tasmax} and.  
+00011d50: 2020 2020 2020 2020 2020 6d69 6e69 6d75            minimu
+00011d60: 6d20 7465 6d70 6572 6174 7572 6520 6162  m temperature ab
+00011d70: 6f76 6520 7b74 6872 6573 685f 7461 736d  ove {thresh_tasm
+00011d80: 696e 7d2e 0a0a 2020 2020 2020 2020 4e6f  in}...        No
+00011d90: 7465 730a 2020 2020 2020 2020 2d2d 2d2d  tes.        ----
+00011da0: 2d0a 2020 2020 2020 2020 466f 7220 6d6f  -.        For mo
+00011db0: 7265 2069 6e66 6f72 6d61 7469 6f6e 206f  re information o
+00011dc0: 6e20 7468 6520 696e 7075 7420 7061 7261  n the input para
+00011dd0: 6d65 7465 7273 2073 6565 3a0a 2020 2020  meters see:.    
+00011de0: 2020 2020 2020 2020 6874 7470 733a 2f2f          https://
+00011df0: 7863 6c69 6d2e 7265 6164 7468 6564 6f63  xclim.readthedoc
+00011e00: 732e 696f 2f65 6e2f 7374 6162 6c65 2f61  s.io/en/stable/a
+00011e10: 7069 2e68 746d 6c23 7863 6c69 6d2e 696e  pi.html#xclim.in
+00011e20: 6469 6361 746f 7273 2e61 746d 6f73 2e68  dicators.atmos.h
+00011e30: 6f74 5f73 7065 6c6c 5f66 7265 7175 656e  ot_spell_frequen
+00011e40: 6379 0a20 2020 2020 2020 2022 2222 0a20  cy.        """. 
+00011e50: 2020 2020 2020 2074 6872 6573 685f 7461         thresh_ta
+00011e60: 736d 6178 203d 205f 7468 7265 7368 5f73  smax = _thresh_s
+00011e70: 7472 696e 6728 7468 7265 7368 5f74 6173  tring(thresh_tas
+00011e80: 6d61 782c 2022 6465 6743 2229 0a20 2020  max, "degC").   
+00011e90: 2020 2020 2074 6872 6573 685f 7461 736d       thresh_tasm
+00011ea0: 696e 203d 205f 7468 7265 7368 5f73 7472  in = _thresh_str
+00011eb0: 696e 6728 7468 7265 7368 5f74 6173 6d69  ing(thresh_tasmi
+00011ec0: 6e2c 2022 6465 6743 2229 0a20 2020 2020  n, "degC").     
+00011ed0: 2020 2072 6574 7572 6e20 7863 2e61 746d     return xc.atm
+00011ee0: 6f73 2e68 6561 745f 7761 7665 5f66 7265  os.heat_wave_fre
+00011ef0: 7175 656e 6379 280a 2020 2020 2020 2020  quency(.        
+00011f00: 2020 2020 7468 7265 7368 5f74 6173 6d61      thresh_tasma
+00011f10: 783d 7468 7265 7368 5f74 6173 6d61 782c  x=thresh_tasmax,
+00011f20: 0a20 2020 2020 2020 2020 2020 2074 6872  .            thr
+00011f30: 6573 685f 7461 736d 696e 3d74 6872 6573  esh_tasmin=thres
+00011f40: 685f 7461 736d 696e 2c0a 2020 2020 2020  h_tasmin,.      
+00011f50: 2020 2020 2020 7769 6e64 6f77 3d77 696e        window=win
+00011f60: 646f 772c 0a20 2020 2020 2020 2020 2020  dow,.           
+00011f70: 202a 2a70 6172 616d 732c 0a20 2020 2020   **params,.     
+00011f80: 2020 2029 0a0a 0a63 6c61 7373 2048 5778     )...class HWx
+00011f90: 3a0a 2020 2020 2222 224d 6178 696d 756d  :.    """Maximum
+00011fa0: 206c 656e 6774 6820 6f66 2068 6561 7420   length of heat 
+00011fb0: 7761 7665 7320 2874 6173 6d61 782c 2074  waves (tasmax, t
+00011fc0: 6173 6d69 6e29 2e22 2222 0a0a 2020 2020  asmin)."""..    
+00011fd0: 7468 7265 7368 5f74 6173 6d69 6e20 3d20  thresh_tasmin = 
+00011fe0: 3232 0a20 2020 2074 6872 6573 685f 7461  22.    thresh_ta
+00011ff0: 736d 6178 203d 2033 300a 2020 2020 7769  smax = 30.    wi
+00012000: 6e64 6f77 203d 2031 0a0a 2020 2020 6465  ndow = 1..    de
+00012010: 6620 636f 6d70 7574 6528 0a20 2020 2020  f compute(.     
+00012020: 2020 2074 6872 6573 685f 7461 736d 6178     thresh_tasmax
+00012030: 3d74 6872 6573 685f 7461 736d 6178 2c0a  =thresh_tasmax,.
+00012040: 2020 2020 2020 2020 7468 7265 7368 5f74          thresh_t
+00012050: 6173 6d69 6e3d 7468 7265 7368 5f74 6173  asmin=thresh_tas
+00012060: 6d69 6e2c 0a20 2020 2020 2020 2077 696e  min,.        win
+00012070: 646f 773d 7769 6e64 6f77 2c0a 2020 2020  dow=window,.    
+00012080: 2020 2020 2a2a 7061 7261 6d73 2c0a 2020      **params,.  
+00012090: 2020 293a 0a20 2020 2020 2020 2022 2222    ):.        """
+000120a0: 4361 6c63 756c 6174 6520 6d61 7869 6d75  Calculate maximu
+000120b0: 6d20 6e75 6d62 6572 206f 6620 6865 6174  m number of heat
+000120c0: 2077 6176 6573 2e0a 0a20 2020 2020 2020   waves...       
+000120d0: 2050 6172 616d 6574 6572 730a 2020 2020   Parameters.    
+000120e0: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20      ----------. 
+000120f0: 2020 2020 2020 2074 6872 6573 685f 7461         thresh_ta
+00012100: 736d 696e 3a20 696e 7420 6f72 2073 7472  smin: int or str
+00012110: 696e 670a 2020 2020 2020 2020 2020 2020  ing.            
+00012120: 5468 7265 7368 6f6c 6420 6d69 6e69 6d75  Threshold minimu
+00012130: 6d20 7465 6d70 6572 6174 7572 6520 6162  m temperature ab
+00012140: 6f76 6520 7768 6963 6820 6120 6461 7920  ove which a day 
+00012150: 6973 2063 6f6e 7369 6465 7265 640a 2020  is considered.  
+00012160: 2020 2020 2020 2020 2020 6173 2061 2068            as a h
+00012170: 6561 7420 6461 7920 2864 6566 6175 6c74  eat day (default
+00012180: 3a20 3232 2064 6567 4329 2e0a 2020 2020  : 22 degC)..    
+00012190: 2020 2020 2020 2020 4966 2074 7970 6520          If type 
+000121a0: 6f66 2074 6872 6573 686f 6c64 2069 7320  of threshold is 
+000121b0: 616e 2069 6e74 6567 6572 2074 6865 2075  an integer the u
+000121c0: 6e69 7420 6973 2073 6574 2074 6f20 6465  nit is set to de
+000121d0: 6743 2e0a 2020 2020 2020 2020 7468 7265  gC..        thre
+000121e0: 7368 5f74 6173 6d61 783a 2069 6e74 206f  sh_tasmax: int o
+000121f0: 7220 7374 7269 6e67 0a20 2020 2020 2020  r string.       
+00012200: 2020 2020 2054 6872 6573 686f 6c64 206d       Threshold m
+00012210: 6178 696d 756d 2074 656d 7065 7261 7475  aximum temperatu
+00012220: 7265 2061 626f 7665 2077 6869 6368 2061  re above which a
+00012230: 2064 6179 2069 7320 636f 6e73 6964 6572   day is consider
+00012240: 6564 0a20 2020 2020 2020 2020 2020 2061  ed.            a
+00012250: 7320 6120 7769 6e74 6572 2064 6179 2028  s a winter day (
+00012260: 6465 6661 756c 743a 2033 3020 6465 6743  default: 30 degC
+00012270: 292e 0a20 2020 2020 2020 2020 2020 2049  )..            I
+00012280: 6620 7479 7065 206f 6620 7468 7265 7368  f type of thresh
+00012290: 6f6c 6420 6973 2061 6e20 696e 7465 6765  old is an intege
+000122a0: 7220 7468 6520 756e 6974 2069 7320 7365  r the unit is se
+000122b0: 7420 746f 2064 6567 432e 0a20 2020 2020  t to degC..     
+000122c0: 2020 2077 696e 646f 773a 2069 6e74 0a20     window: int. 
+000122d0: 2020 2020 2020 2020 2020 204d 696e 696d             Minim
+000122e0: 756d 206e 756d 6265 7220 6f66 2064 6179  um number of day
+000122f0: 7320 7769 7468 2074 656d 7065 7261 7475  s with temperatu
+00012300: 7265 2061 626f 7665 2074 6872 6573 680a  re above thresh.
+00012310: 2020 2020 2020 2020 2020 2020 746f 2071              to q
+00012320: 7561 6c69 6679 2061 7320 6120 686f 7420  ualify as a hot 
+00012330: 7370 656c 6c20 2864 6566 6175 6c74 3a20  spell (default: 
+00012340: 3129 2e0a 0a20 2020 2020 2020 2052 6574  1)...        Ret
+00012350: 7572 6e73 0a20 2020 2020 2020 202d 2d2d  urns.        ---
+00012360: 2d2d 2d2d 0a20 2020 2020 2020 2078 6172  ----.        xar
+00012370: 7261 792e 4461 7461 4172 7261 790a 2020  ray.DataArray.  
+00012380: 2020 2020 2020 2020 2020 4d61 7869 6d75            Maximu
+00012390: 6d20 6c65 6e67 7468 206f 6620 6865 6174  m length of heat
+000123a0: 2077 6176 6573 206f 6620 6174 206c 6561   waves of at lea
+000123b0: 7374 207b 7769 6e64 6f77 7d20 636f 6e73  st {window} cons
+000123c0: 6563 7574 6976 6520 6461 7973 0a20 2020  ecutive days.   
+000123d0: 2020 2020 2020 2020 2077 6974 6820 6d61           with ma
+000123e0: 7869 6d75 6d20 7465 6d70 6572 6174 7572  ximum temperatur
+000123f0: 6520 6162 6f76 6520 7b74 6872 6573 685f  e above {thresh_
+00012400: 7461 736d 6178 7d20 616e 640a 2020 2020  tasmax} and.    
+00012410: 2020 2020 2020 2020 6d69 6e69 6d75 6d20          minimum 
+00012420: 7465 6d70 6572 6174 7572 6520 6162 6f76  temperature abov
+00012430: 6520 7b74 6872 6573 685f 7461 736d 696e  e {thresh_tasmin
+00012440: 7d2e 0a0a 2020 2020 2020 2020 4e6f 7465  }...        Note
+00012450: 730a 2020 2020 2020 2020 2d2d 2d2d 2d0a  s.        -----.
+00012460: 2020 2020 2020 2020 466f 7220 6d6f 7265          For more
+00012470: 2069 6e66 6f72 6d61 7469 6f6e 206f 6e20   information on 
+00012480: 7468 6520 696e 7075 7420 7061 7261 6d65  the input parame
+00012490: 7465 7273 2073 6565 3a0a 2020 2020 2020  ters see:.      
+000124a0: 2020 2020 2020 6874 7470 733a 2f2f 7863        https://xc
+000124b0: 6c69 6d2e 7265 6164 7468 6564 6f63 732e  lim.readthedocs.
+000124c0: 696f 2f65 6e2f 7374 6162 6c65 2f61 7069  io/en/stable/api
+000124d0: 2e68 746d 6c23 7863 6c69 6d2e 696e 6469  .html#xclim.indi
+000124e0: 6361 746f 7273 2e61 746d 6f73 2e68 6561  cators.atmos.hea
+000124f0: 745f 7761 7665 5f6d 6178 5f6c 656e 6774  t_wave_max_lengt
+00012500: 680a 2020 2020 2020 2020 2222 220a 2020  h.        """.  
+00012510: 2020 2020 2020 7468 7265 7368 5f74 6173        thresh_tas
+00012520: 6d61 7820 3d20 5f74 6872 6573 685f 7374  max = _thresh_st
+00012530: 7269 6e67 2874 6872 6573 685f 7461 736d  ring(thresh_tasm
+00012540: 6178 2c20 2264 6567 4322 290a 2020 2020  ax, "degC").    
+00012550: 2020 2020 7468 7265 7368 5f74 6173 6d69      thresh_tasmi
+00012560: 6e20 3d20 5f74 6872 6573 685f 7374 7269  n = _thresh_stri
+00012570: 6e67 2874 6872 6573 685f 7461 736d 696e  ng(thresh_tasmin
+00012580: 2c20 2264 6567 4322 290a 2020 2020 2020  , "degC").      
+00012590: 2020 7265 7475 726e 2078 632e 6174 6d6f    return xc.atmo
+000125a0: 732e 6865 6174 5f77 6176 655f 6d61 785f  s.heat_wave_max_
+000125b0: 6c65 6e67 7468 280a 2020 2020 2020 2020  length(.        
+000125c0: 2020 2020 7468 7265 7368 5f74 6173 6d61      thresh_tasma
+000125d0: 783d 7468 7265 7368 5f74 6173 6d61 782c  x=thresh_tasmax,
+000125e0: 0a20 2020 2020 2020 2020 2020 2074 6872  .            thr
+000125f0: 6573 685f 7461 736d 696e 3d74 6872 6573  esh_tasmin=thres
+00012600: 685f 7461 736d 696e 2c0a 2020 2020 2020  h_tasmin,.      
+00012610: 2020 2020 2020 7769 6e64 6f77 3d77 696e        window=win
+00012620: 646f 772c 0a20 2020 2020 2020 2020 2020  dow,.           
+00012630: 202a 2a70 6172 616d 732c 0a20 2020 2020   **params,.     
+00012640: 2020 2029 0a0a 0a63 6c61 7373 2048 576e     )...class HWn
+00012650: 3a0a 2020 2020 2222 2254 6f74 616c 206e  :.    """Total n
+00012660: 756d 6265 7220 6f66 2064 6179 7320 696e  umber of days in
+00012670: 2068 6561 7420 7761 7665 7320 2874 6173   heat waves (tas
+00012680: 6d61 782c 2074 6173 6d69 6e29 2e22 2222  max, tasmin)."""
+00012690: 0a0a 2020 2020 7468 7265 7368 5f74 6173  ..    thresh_tas
+000126a0: 6d69 6e20 3d20 3232 0a20 2020 2074 6872  min = 22.    thr
+000126b0: 6573 685f 7461 736d 6178 203d 2033 300a  esh_tasmax = 30.
+000126c0: 2020 2020 7769 6e64 6f77 203d 2033 0a0a      window = 3..
+000126d0: 2020 2020 6465 6620 636f 6d70 7574 6528      def compute(
+000126e0: 0a20 2020 2020 2020 2074 6872 6573 685f  .        thresh_
+000126f0: 7461 736d 696e 3d74 6872 6573 685f 7461  tasmin=thresh_ta
+00012700: 736d 696e 2c0a 2020 2020 2020 2020 7468  smin,.        th
+00012710: 7265 7368 5f74 6173 6d61 783d 7468 7265  resh_tasmax=thre
+00012720: 7368 5f74 6173 6d61 782c 0a20 2020 2020  sh_tasmax,.     
+00012730: 2020 2077 696e 646f 773d 7769 6e64 6f77     window=window
+00012740: 2c0a 2020 2020 2020 2020 2a2a 7061 7261  ,.        **para
+00012750: 6d73 2c0a 2020 2020 293a 0a20 2020 2020  ms,.    ):.     
+00012760: 2020 2022 2222 4361 6c63 756c 6174 6520     """Calculate 
+00012770: 746f 7461 6c20 6e75 6d62 6572 206f 6620  total number of 
+00012780: 6461 7973 2069 6e20 6865 6174 2077 6176  days in heat wav
+00012790: 6573 2e0a 0a20 2020 2020 2020 2050 6172  es...        Par
+000127a0: 616d 6574 6572 730a 2020 2020 2020 2020  ameters.        
+000127b0: 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020  ----------.     
+000127c0: 2020 2074 6872 6573 685f 7461 736d 696e     thresh_tasmin
+000127d0: 3a20 696e 7420 6f72 2073 7472 696e 670a  : int or string.
+000127e0: 2020 2020 2020 2020 2020 2020 5468 7265              Thre
+000127f0: 7368 6f6c 6420 6d69 6e69 6d75 6d20 7465  shold minimum te
+00012800: 6d70 6572 6174 7572 6520 6162 6f76 6520  mperature above 
+00012810: 7768 6963 6820 6120 6461 7920 6973 2063  which a day is c
+00012820: 6f6e 7369 6465 7265 640a 2020 2020 2020  onsidered.      
+00012830: 2020 2020 2020 6173 2061 2068 6561 7420        as a heat 
+00012840: 6461 7920 2864 6566 6175 6c74 3a20 3232  day (default: 22
+00012850: 2064 6567 4329 2e0a 2020 2020 2020 2020   degC)..        
+00012860: 2020 2020 4966 2074 7970 6520 6f66 2074      If type of t
+00012870: 6872 6573 686f 6c64 2069 7320 616e 2069  hreshold is an i
+00012880: 6e74 6567 6572 2074 6865 2075 6e69 7420  nteger the unit 
+00012890: 6973 2073 6574 2074 6f20 6465 6743 2e0a  is set to degC..
+000128a0: 2020 2020 2020 2020 7468 7265 7368 5f74          thresh_t
+000128b0: 6173 6d61 783a 2069 6e74 206f 7220 7374  asmax: int or st
+000128c0: 7269 6e67 0a20 2020 2020 2020 2020 2020  ring.           
+000128d0: 2054 6872 6573 686f 6c64 206d 6178 696d   Threshold maxim
+000128e0: 756d 2074 656d 7065 7261 7475 7265 2061  um temperature a
+000128f0: 626f 7665 2077 6869 6368 2061 2064 6179  bove which a day
+00012900: 2069 7320 636f 6e73 6964 6572 6564 0a20   is considered. 
+00012910: 2020 2020 2020 2020 2020 2061 7320 6120             as a 
+00012920: 7769 6e74 6572 2064 6179 2028 6465 6661  winter day (defa
+00012930: 756c 743a 2033 3020 6465 6743 292e 0a20  ult: 30 degC).. 
+00012940: 2020 2020 2020 2020 2020 2049 6620 7479             If ty
+00012950: 7065 206f 6620 7468 7265 7368 6f6c 6420  pe of threshold 
+00012960: 6973 2061 6e20 696e 7465 6765 7220 7468  is an integer th
+00012970: 6520 756e 6974 2069 7320 7365 7420 746f  e unit is set to
+00012980: 2064 6567 432e 0a20 2020 2020 2020 2077   degC..        w
+00012990: 696e 646f 773a 2069 6e74 0a20 2020 2020  indow: int.     
+000129a0: 2020 2020 2020 204d 696e 696d 756d 206e         Minimum n
+000129b0: 756d 6265 7220 6f66 2064 6179 7320 7769  umber of days wi
+000129c0: 7468 2074 656d 7065 7261 7475 7265 2061  th temperature a
+000129d0: 626f 7665 2074 6872 6573 680a 2020 2020  bove thresh.    
+000129e0: 2020 2020 2020 2020 746f 2071 7561 6c69          to quali
+000129f0: 6679 2061 7320 6120 686f 7420 7370 656c  fy as a hot spel
+00012a00: 6c20 2864 6566 6175 6c74 3a20 3329 2e0a  l (default: 3)..
+00012a10: 0a20 2020 2020 2020 2052 6574 7572 6e73  .        Returns
+00012a20: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
+00012a30: 0a20 2020 2020 2020 2078 6172 7261 792e  .        xarray.
+00012a40: 4461 7461 4172 7261 790a 2020 2020 2020  DataArray.      
+00012a50: 2020 2020 2020 546f 7461 6c20 6e75 6d62        Total numb
+00012a60: 6572 206f 6620 6461 7973 2069 6e20 6865  er of days in he
+00012a70: 6174 2077 6176 6573 206f 6620 6174 206c  at waves of at l
+00012a80: 6561 7374 207b 7769 6e64 6f77 7d0a 2020  east {window}.  
+00012a90: 2020 2020 2020 2020 2020 636f 6e73 6563            consec
+00012aa0: 7574 6976 6520 6461 7973 2077 6974 6820  utive days with 
+00012ab0: 6d61 7869 6d75 6d20 7465 6d70 6572 6174  maximum temperat
+00012ac0: 7572 6520 6162 6f76 6520 7b74 6872 6573  ure above {thres
+00012ad0: 685f 7461 736d 6178 7d0a 2020 2020 2020  h_tasmax}.      
+00012ae0: 2020 2020 2020 616e 6420 6d69 6e69 6d75        and minimu
+00012af0: 6d20 7465 6d70 6572 6174 7572 6520 6162  m temperature ab
+00012b00: 6f76 6520 7b74 6872 6573 685f 7461 736d  ove {thresh_tasm
+00012b10: 696e 7d2e 0a0a 2020 2020 2020 2020 4e6f  in}...        No
+00012b20: 7465 730a 2020 2020 2020 2020 2d2d 2d2d  tes.        ----
+00012b30: 2d0a 2020 2020 2020 2020 466f 7220 6d6f  -.        For mo
+00012b40: 7265 2069 6e66 6f72 6d61 7469 6f6e 206f  re information o
+00012b50: 6e20 7468 6520 696e 7075 7420 7061 7261  n the input para
+00012b60: 6d65 7465 7273 2073 6565 3a0a 2020 2020  meters see:.    
+00012b70: 2020 2020 2020 2020 6874 7470 733a 2f2f          https://
+00012b80: 7863 6c69 6d2e 7265 6164 7468 6564 6f63  xclim.readthedoc
+00012b90: 732e 696f 2f65 6e2f 7374 6162 6c65 2f61  s.io/en/stable/a
+00012ba0: 7069 2e68 746d 6c23 7863 6c69 6d2e 696e  pi.html#xclim.in
+00012bb0: 6469 6361 746f 7273 2e61 746d 6f73 2e68  dicators.atmos.h
+00012bc0: 6f74 5f73 7065 6c6c 5f74 6f74 616c 5f6c  ot_spell_total_l
+00012bd0: 656e 6774 680a 2020 2020 2020 2020 2222  ength.        ""
+00012be0: 220a 2020 2020 2020 2020 7468 7265 7368  ".        thresh
+00012bf0: 5f74 6173 6d61 7820 3d20 5f74 6872 6573  _tasmax = _thres
+00012c00: 685f 7374 7269 6e67 2874 6872 6573 685f  h_string(thresh_
+00012c10: 7461 736d 6178 2c20 2264 6567 4322 290a  tasmax, "degC").
+00012c20: 2020 2020 2020 2020 7468 7265 7368 5f74          thresh_t
+00012c30: 6173 6d69 6e20 3d20 5f74 6872 6573 685f  asmin = _thresh_
+00012c40: 7374 7269 6e67 2874 6872 6573 685f 7461  string(thresh_ta
+00012c50: 736d 696e 2c20 2264 6567 4322 290a 2020  smin, "degC").  
+00012c60: 2020 2020 2020 7265 7475 726e 2078 632e        return xc.
+00012c70: 6174 6d6f 732e 6865 6174 5f77 6176 655f  atmos.heat_wave_
+00012c80: 746f 7461 6c5f 6c65 6e67 7468 280a 2020  total_length(.  
+00012c90: 2020 2020 2020 2020 2020 7468 7265 7368            thresh
+00012ca0: 5f74 6173 6d61 783d 7468 7265 7368 5f74  _tasmax=thresh_t
+00012cb0: 6173 6d61 782c 0a20 2020 2020 2020 2020  asmax,.         
+00012cc0: 2020 2074 6872 6573 685f 7461 736d 696e     thresh_tasmin
+00012cd0: 3d74 6872 6573 685f 7461 736d 696e 2c0a  =thresh_tasmin,.
+00012ce0: 2020 2020 2020 2020 2020 2020 7769 6e64              wind
+00012cf0: 6f77 3d77 696e 646f 772c 0a20 2020 2020  ow=window,.     
+00012d00: 2020 2020 2020 202a 2a70 6172 616d 732c         **params,
+00012d10: 0a20 2020 2020 2020 2029 0a0a 0a63 6c61  .        )...cla
+00012d20: 7373 2047 5353 3a0a 2020 2020 2222 2247  ss GSS:.    """G
+00012d30: 726f 7769 6e67 2073 6561 736f 6e20 7374  rowing season st
+00012d40: 6172 7420 2874 6173 292e 2222 220a 0a20  art (tas).""".. 
+00012d50: 2020 2074 6872 6573 6820 3d20 350a 2020     thresh = 5.  
+00012d60: 2020 7769 6e64 6f77 203d 2035 0a0a 2020    window = 5..  
+00012d70: 2020 6465 6620 636f 6d70 7574 6528 7468    def compute(th
+00012d80: 7265 7368 3d74 6872 6573 682c 2077 696e  resh=thresh, win
+00012d90: 646f 773d 7769 6e64 6f77 2c20 2a2a 7061  dow=window, **pa
+00012da0: 7261 6d73 293a 0a20 2020 2020 2020 2022  rams):.        "
+00012db0: 2222 4361 6c63 756c 6174 6520 6772 6f77  ""Calculate grow
+00012dc0: 696e 6720 7365 6173 6f6e 2073 7461 7274  ing season start
+00012dd0: 2e0a 0a20 2020 2020 2020 2050 6172 616d  ...        Param
+00012de0: 6574 6572 730a 2020 2020 2020 2020 2d2d  eters.        --
+00012df0: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020 2020  --------.       
+00012e00: 2074 6872 6573 683a 2069 6e74 206f 7220   thresh: int or 
+00012e10: 7374 7269 6e67 0a20 2020 2020 2020 2020  string.         
+00012e20: 2020 2054 6872 6573 686f 6c64 2074 656d     Threshold tem
+00012e30: 7065 7261 7475 7265 2061 626f 7665 2077  perature above w
+00012e40: 6869 6368 2074 6865 2067 726f 7769 6e67  hich the growing
+00012e50: 2073 6561 736f 6e20 7374 6172 7473 0a20   season starts. 
+00012e60: 2020 2020 2020 2020 2020 2028 6465 6661             (defa
+00012e70: 756c 743a 2035 2064 6567 4329 2e0a 2020  ult: 5 degC)..  
+00012e80: 2020 2020 2020 2020 2020 4966 2074 7970            If typ
+00012e90: 6520 6f66 2074 6872 6573 686f 6c64 2069  e of threshold i
+00012ea0: 7320 616e 2069 6e74 6567 6572 2074 6865  s an integer the
+00012eb0: 2075 6e69 7420 6973 2073 6574 2074 6f20   unit is set to 
+00012ec0: 6465 6743 2e0a 2020 2020 2020 2020 7769  degC..        wi
+00012ed0: 6e64 6f77 3a20 696e 740a 2020 2020 2020  ndow: int.      
+00012ee0: 2020 2020 2020 4d69 6e69 6d75 6d20 6e75        Minimum nu
+00012ef0: 6d62 6572 206f 6620 6461 7973 2077 6974  mber of days wit
+00012f00: 6820 7465 6d70 6572 6174 7572 6520 6162  h temperature ab
+00012f10: 6f76 6520 7468 7265 7368 6f6c 640a 2020  ove threshold.  
+00012f20: 2020 2020 2020 2020 2020 6e65 6564 6564            needed
+00012f30: 2066 6f72 2065 7661 6c75 6174 696f 6e20   for evaluation 
+00012f40: 2864 6566 6175 6c74 3a20 3529 2e0a 0a20  (default: 5)... 
+00012f50: 2020 2020 2020 2052 6574 7572 6e73 0a20         Returns. 
+00012f60: 2020 2020 2020 202d 2d2d 2d2d 2d2d 0a20         -------. 
+00012f70: 2020 2020 2020 2078 6172 7261 792e 4461         xarray.Da
+00012f80: 7461 4172 7261 790a 2020 2020 2020 2020  taArray.        
+00012f90: 2020 2020 4772 6f77 696e 6720 7365 6173      Growing seas
+00012fa0: 6f6e 2073 7461 7274 2e0a 0a20 2020 2020  on start...     
+00012fb0: 2020 204e 6f74 6573 0a20 2020 2020 2020     Notes.       
+00012fc0: 202d 2d2d 2d2d 0a20 2020 2020 2020 2046   -----.        F
+00012fd0: 6f72 206d 6f72 6520 696e 666f 726d 6174  or more informat
+00012fe0: 696f 6e20 6f6e 2074 6865 2069 6e70 7574  ion on the input
+00012ff0: 2070 6172 616d 6574 6572 7320 7365 653a   parameters see:
+00013000: 0a20 2020 2020 2020 2020 2020 2068 7474  .            htt
+00013010: 7073 3a2f 2f78 636c 696d 2e72 6561 6474  ps://xclim.readt
+00013020: 6865 646f 6373 2e69 6f2f 656e 2f73 7461  hedocs.io/en/sta
+00013030: 626c 652f 6170 692e 6874 6d6c 2378 636c  ble/api.html#xcl
+00013040: 696d 2e69 6e64 6963 6174 6f72 732e 6174  im.indicators.at
+00013050: 6d6f 732e 6772 6f77 696e 675f 7365 6173  mos.growing_seas
+00013060: 6f6e 5f73 7461 7274 0a20 2020 2020 2020  on_start.       
+00013070: 2022 2222 0a20 2020 2020 2020 2074 6872   """.        thr
+00013080: 6573 6820 3d20 5f74 6872 6573 685f 7374  esh = _thresh_st
+00013090: 7269 6e67 2874 6872 6573 682c 2022 6465  ring(thresh, "de
+000130a0: 6743 2229 0a20 2020 2020 2020 2072 6574  gC").        ret
+000130b0: 7572 6e20 7863 2e61 746d 6f73 2e67 726f  urn xc.atmos.gro
+000130c0: 7769 6e67 5f73 6561 736f 6e5f 7374 6172  wing_season_star
+000130d0: 7428 0a20 2020 2020 2020 2020 2020 2074  t(.            t
+000130e0: 6872 6573 683d 7468 7265 7368 2c0a 2020  hresh=thresh,.  
+000130f0: 2020 2020 2020 2020 2020 7769 6e64 6f77            window
+00013100: 3d77 696e 646f 772c 0a20 2020 2020 2020  =window,.       
+00013110: 2020 2020 202a 2a70 6172 616d 732c 0a20       **params,. 
+00013120: 2020 2020 2020 2029 0a0a 0a63 6c61 7373         )...class
+00013130: 2047 5345 3a0a 2020 2020 2222 2247 726f   GSE:.    """Gro
+00013140: 7769 6e67 2073 6561 736f 6e20 656e 6420  wing season end 
+00013150: 2874 6173 292e 2222 220a 0a20 2020 2074  (tas)."""..    t
+00013160: 6872 6573 6820 3d20 350a 2020 2020 7769  hresh = 5.    wi
+00013170: 6e64 6f77 203d 2035 0a0a 2020 2020 6465  ndow = 5..    de
+00013180: 6620 636f 6d70 7574 6528 7468 7265 7368  f compute(thresh
+00013190: 3d74 6872 6573 682c 2077 696e 646f 773d  =thresh, window=
+000131a0: 7769 6e64 6f77 2c20 2a2a 7061 7261 6d73  window, **params
+000131b0: 293a 0a20 2020 2020 2020 2022 2222 4361  ):.        """Ca
+000131c0: 6c63 756c 6174 6520 6772 6f77 696e 6720  lculate growing 
+000131d0: 7365 6173 6f6e 2065 6e64 2e0a 0a20 2020  season end...   
+000131e0: 2020 2020 2050 6172 616d 6574 6572 730a       Parameters.
+000131f0: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d2d          --------
+00013200: 2d2d 0a20 2020 2020 2020 2074 6872 6573  --.        thres
+00013210: 683a 2069 6e74 206f 7220 7374 7269 6e67  h: int or string
+00013220: 0a20 2020 2020 2020 2020 2020 2054 6872  .            Thr
+00013230: 6573 686f 6c64 2074 656d 7065 7261 7475  eshold temperatu
+00013240: 7265 2062 656c 6f77 2077 6869 6368 2074  re below which t
+00013250: 6865 2067 726f 7769 6e67 2073 6561 736f  he growing seaso
+00013260: 6e20 656e 6473 0a20 2020 2020 2020 2020  n ends.         
+00013270: 2020 2028 6465 6661 756c 743a 2035 2064     (default: 5 d
+00013280: 6567 4329 2e0a 2020 2020 2020 2020 2020  egC)..          
+00013290: 2020 4966 2074 7970 6520 6f66 2074 6872    If type of thr
+000132a0: 6573 686f 6c64 2069 7320 616e 2069 6e74  eshold is an int
+000132b0: 6567 6572 2074 6865 2075 6e69 7420 6973  eger the unit is
+000132c0: 2073 6574 2074 6f20 6465 6743 2e0a 2020   set to degC..  
+000132d0: 2020 2020 2020 7769 6e64 6f77 3a20 696e        window: in
+000132e0: 740a 2020 2020 2020 2020 2020 2020 4d69  t.            Mi
+000132f0: 6e69 6d75 6d20 6e75 6d62 6572 206f 6620  nimum number of 
+00013300: 6461 7973 2077 6974 6820 7465 6d70 6572  days with temper
+00013310: 6174 7572 6520 6265 6c6f 7720 7468 7265  ature below thre
+00013320: 7368 6f6c 640a 2020 2020 2020 2020 2020  shold.          
+00013330: 2020 6e65 6564 6564 2066 6f72 2065 7661    needed for eva
+00013340: 6c75 6174 696f 6e20 2864 6566 6175 6c74  luation (default
+00013350: 3a20 3529 2e0a 0a20 2020 2020 2020 2052  : 5)...        R
+00013360: 6574 7572 6e73 0a20 2020 2020 2020 202d  eturns.        -
+00013370: 2d2d 2d2d 2d2d 0a20 2020 2020 2020 2078  ------.        x
+00013380: 6172 7261 792e 4461 7461 4172 7261 790a  array.DataArray.
+00013390: 2020 2020 2020 2020 2020 2020 4772 6f77              Grow
+000133a0: 696e 6720 7365 6173 6f6e 2065 6e64 2e0a  ing season end..
+000133b0: 0a20 2020 2020 2020 204e 6f74 6573 0a20  .        Notes. 
+000133c0: 2020 2020 2020 202d 2d2d 2d2d 0a20 2020         -----.   
+000133d0: 2020 2020 2046 6f72 206d 6f72 6520 696e       For more in
+000133e0: 666f 726d 6174 696f 6e20 6f6e 2074 6865  formation on the
+000133f0: 2069 6e70 7574 2070 6172 616d 6574 6572   input parameter
+00013400: 7320 7365 653a 0a20 2020 2020 2020 2020  s see:.         
+00013410: 2020 2068 7474 7073 3a2f 2f78 636c 696d     https://xclim
+00013420: 2e72 6561 6474 6865 646f 6373 2e69 6f2f  .readthedocs.io/
+00013430: 656e 2f73 7461 626c 652f 6170 692e 6874  en/stable/api.ht
+00013440: 6d6c 2378 636c 696d 2e69 6e64 6963 6174  ml#xclim.indicat
+00013450: 6f72 732e 6174 6d6f 732e 6772 6f77 696e  ors.atmos.growin
+00013460: 675f 7365 6173 6f6e 5f65 6e64 0a20 2020  g_season_end.   
+00013470: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+00013480: 2074 6872 6573 6820 3d20 5f74 6872 6573   thresh = _thres
+00013490: 685f 7374 7269 6e67 2874 6872 6573 682c  h_string(thresh,
+000134a0: 2022 6465 6743 2229 0a20 2020 2020 2020   "degC").       
+000134b0: 2072 6574 7572 6e20 7863 2e61 746d 6f73   return xc.atmos
+000134c0: 2e67 726f 7769 6e67 5f73 6561 736f 6e5f  .growing_season_
+000134d0: 656e 6428 0a20 2020 2020 2020 2020 2020  end(.           
+000134e0: 2074 6872 6573 683d 7468 7265 7368 2c0a   thresh=thresh,.
+000134f0: 2020 2020 2020 2020 2020 2020 7769 6e64              wind
+00013500: 6f77 3d77 696e 646f 772c 0a20 2020 2020  ow=window,.     
+00013510: 2020 2020 2020 202a 2a70 6172 616d 732c         **params,
+00013520: 0a20 2020 2020 2020 2029 0a0a 0a63 6c61  .        )...cla
+00013530: 7373 2046 4653 3a0a 2020 2020 2222 2246  ss FFS:.    """F
+00013540: 726f 7374 2066 7265 6520 7365 6173 6f6e  rost free season
+00013550: 2073 7461 7274 2028 7461 736d 696e 292e   start (tasmin).
+00013560: 2222 220a 0a20 2020 2074 6872 6573 6820  """..    thresh 
+00013570: 3d20 300a 2020 2020 7769 6e64 6f77 203d  = 0.    window =
+00013580: 2035 0a0a 2020 2020 6465 6620 636f 6d70   5..    def comp
+00013590: 7574 6528 7468 7265 7368 3d74 6872 6573  ute(thresh=thres
+000135a0: 682c 2077 696e 646f 773d 7769 6e64 6f77  h, window=window
+000135b0: 2c20 2a2a 7061 7261 6d73 293a 0a20 2020  , **params):.   
+000135c0: 2020 2020 2022 2222 4361 6c63 756c 6174       """Calculat
+000135d0: 6520 6672 6f73 7420 6672 6565 2073 6561  e frost free sea
+000135e0: 736f 6e20 7374 6172 742e 0a0a 2020 2020  son start...    
+000135f0: 2020 2020 5061 7261 6d65 7465 7273 0a20      Parameters. 
+00013600: 2020 2020 2020 202d 2d2d 2d2d 2d2d 2d2d         ---------
+00013610: 2d0a 2020 2020 2020 2020 7468 7265 7368  -.        thresh
+00013620: 3a20 696e 7420 6f72 2073 7472 696e 670a  : int or string.
+00013630: 2020 2020 2020 2020 2020 2020 5468 7265              Thre
+00013640: 7368 6f6c 6420 6d69 6e69 6d75 6d20 7465  shold minimum te
+00013650: 6d70 6572 6174 7572 6520 6162 6f76 6520  mperature above 
+00013660: 7768 6963 6820 7468 6520 6672 6f73 7420  which the frost 
+00013670: 6672 6565 2073 6561 736f 6e0a 2020 2020  free season.    
+00013680: 2020 2020 2020 2020 7374 6172 7473 2028          starts (
+00013690: 6465 6661 756c 743a 2030 2064 6567 4329  default: 0 degC)
+000136a0: 2e0a 2020 2020 2020 2020 2020 2020 4966  ..            If
+000136b0: 2074 7970 6520 6f66 2074 6872 6573 686f   type of thresho
+000136c0: 6c64 2069 7320 616e 2069 6e74 6567 6572  ld is an integer
+000136d0: 2074 6865 2075 6e69 7420 6973 2073 6574   the unit is set
+000136e0: 2074 6f20 6465 6743 2e0a 2020 2020 2020   to degC..      
+000136f0: 2020 7769 6e64 6f77 3a20 696e 740a 2020    window: int.  
+00013700: 2020 2020 2020 2020 2020 4d69 6e69 6d75            Minimu
+00013710: 6d20 6e75 6d62 6572 206f 6620 6461 7973  m number of days
+00013720: 2077 6974 6820 7465 6d70 6572 6174 7572   with temperatur
+00013730: 6520 6162 6f76 6520 7468 7265 7368 6f6c  e above threshol
+00013740: 640a 2020 2020 2020 2020 2020 2020 6e65  d.            ne
+00013750: 6564 6564 2066 6f72 2065 7661 6c75 6174  eded for evaluat
+00013760: 696f 6e20 2864 6566 6175 6c74 3a20 3529  ion (default: 5)
+00013770: 2e0a 0a20 2020 2020 2020 2052 6574 7572  ...        Retur
+00013780: 6e73 0a20 2020 2020 2020 202d 2d2d 2d2d  ns.        -----
+00013790: 2d2d 0a20 2020 2020 2020 2078 6172 7261  --.        xarra
+000137a0: 792e 4461 7461 4172 7261 790a 2020 2020  y.DataArray.    
+000137b0: 2020 2020 2020 2020 4672 6f73 7420 6672          Frost fr
+000137c0: 6565 2073 6561 736f 6e20 7374 6172 742e  ee season start.
+000137d0: 0a0a 2020 2020 2020 2020 4e6f 7465 730a  ..        Notes.
+000137e0: 2020 2020 2020 2020 2d2d 2d2d 2d0a 2020          -----.  
+000137f0: 2020 2020 2020 466f 7220 6d6f 7265 2069        For more i
+00013800: 6e66 6f72 6d61 7469 6f6e 206f 6e20 7468  nformation on th
+00013810: 6520 696e 7075 7420 7061 7261 6d65 7465  e input paramete
+00013820: 7273 2073 6565 3a0a 2020 2020 2020 2020  rs see:.        
+00013830: 2020 2020 6874 7470 733a 2f2f 7863 6c69      https://xcli
+00013840: 6d2e 7265 6164 7468 6564 6f63 732e 696f  m.readthedocs.io
+00013850: 2f65 6e2f 7374 6162 6c65 2f61 7069 2e68  /en/stable/api.h
+00013860: 746d 6c23 7863 6c69 6d2e 696e 6469 6361  tml#xclim.indica
+00013870: 746f 7273 2e61 746d 6f73 2e66 726f 7374  tors.atmos.frost
+00013880: 5f66 7265 655f 7365 6173 6f6e 5f73 7461  _free_season_sta
+00013890: 7274 0a20 2020 2020 2020 2022 2222 0a20  rt.        """. 
+000138a0: 2020 2020 2020 2074 6872 6573 6820 3d20         thresh = 
+000138b0: 5f74 6872 6573 685f 7374 7269 6e67 2874  _thresh_string(t
+000138c0: 6872 6573 682c 2022 6465 6743 2229 0a20  hresh, "degC"). 
+000138d0: 2020 2020 2020 2072 6574 7572 6e20 7863         return xc
+000138e0: 2e61 746d 6f73 2e66 726f 7374 5f66 7265  .atmos.frost_fre
+000138f0: 655f 7365 6173 6f6e 5f73 7461 7274 280a  e_season_start(.
+00013900: 2020 2020 2020 2020 2020 2020 7468 7265              thre
+00013910: 7368 3d74 6872 6573 682c 0a20 2020 2020  sh=thresh,.     
+00013920: 2020 2020 2020 2077 696e 646f 773d 7769         window=wi
+00013930: 6e64 6f77 2c0a 2020 2020 2020 2020 2020  ndow,.          
+00013940: 2020 2a2a 7061 7261 6d73 2c0a 2020 2020    **params,.    
+00013950: 2020 2020 290a 0a0a 636c 6173 7320 4646      )...class FF
+00013960: 453a 0a20 2020 2022 2222 4672 6f73 7420  E:.    """Frost 
+00013970: 6672 6565 2073 6561 736f 6e20 656e 6420  free season end 
+00013980: 2874 6173 6d69 6e29 2e22 2222 0a0a 2020  (tasmin)."""..  
+00013990: 2020 7468 7265 7368 203d 2030 0a20 2020    thresh = 0.   
+000139a0: 2077 696e 646f 7720 3d20 350a 0a20 2020   window = 5..   
+000139b0: 2064 6566 2063 6f6d 7075 7465 2874 6872   def compute(thr
+000139c0: 6573 683d 7468 7265 7368 2c20 7769 6e64  esh=thresh, wind
+000139d0: 6f77 3d77 696e 646f 772c 202a 2a70 6172  ow=window, **par
+000139e0: 616d 7329 3a0a 2020 2020 2020 2020 2222  ams):.        ""
+000139f0: 2243 616c 6375 6c61 7465 2066 726f 7374  "Calculate frost
+00013a00: 2066 7265 6520 7365 6173 6f6e 2065 6e64   free season end
+00013a10: 2e0a 0a20 2020 2020 2020 2050 6172 616d  ...        Param
+00013a20: 6574 6572 730a 2020 2020 2020 2020 2d2d  eters.        --
+00013a30: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020 2020  --------.       
+00013a40: 2074 6872 6573 683a 2069 6e74 206f 7220   thresh: int or 
+00013a50: 7374 7269 6e67 0a20 2020 2020 2020 2020  string.         
+00013a60: 2020 2054 6872 6573 686f 6c64 206d 696e     Threshold min
+00013a70: 696d 756d 2074 656d 7065 7261 7475 7265  imum temperature
+00013a80: 2062 656c 6f77 2077 6869 6368 2074 6865   below which the
+00013a90: 2066 726f 7374 2066 7265 6520 7365 6173   frost free seas
+00013aa0: 6f6e 0a20 2020 2020 2020 2020 2020 2065  on.            e
+00013ab0: 6e64 7320 2864 6566 6175 6c74 3a20 3020  nds (default: 0 
+00013ac0: 6465 6743 292e 0a20 2020 2020 2020 2020  degC)..         
+00013ad0: 2020 2049 6620 7479 7065 206f 6620 7468     If type of th
+00013ae0: 7265 7368 6f6c 6420 6973 2061 6e20 696e  reshold is an in
+00013af0: 7465 6765 7220 7468 6520 756e 6974 2069  teger the unit i
+00013b00: 7320 7365 7420 746f 2064 6567 432e 0a20  s set to degC.. 
+00013b10: 2020 2020 2020 2077 696e 646f 773a 2069         window: i
+00013b20: 6e74 0a20 2020 2020 2020 2020 2020 204d  nt.            M
+00013b30: 696e 696d 756d 206e 756d 6265 7220 6f66  inimum number of
+00013b40: 2064 6179 7320 7769 7468 2074 656d 7065   days with tempe
+00013b50: 7261 7475 7265 2062 656c 6f77 2074 6872  rature below thr
+00013b60: 6573 686f 6c64 0a20 2020 2020 2020 2020  eshold.         
+00013b70: 2020 206e 6565 6465 6420 666f 7220 6576     needed for ev
+00013b80: 616c 7561 7469 6f6e 2028 6465 6661 756c  aluation (defaul
+00013b90: 743a 2035 292e 0a0a 2020 2020 2020 2020  t: 5)...        
+00013ba0: 5265 7475 726e 730a 2020 2020 2020 2020  Returns.        
+00013bb0: 2d2d 2d2d 2d2d 2d0a 2020 2020 2020 2020  -------.        
+00013bc0: 7861 7272 6179 2e44 6174 6141 7272 6179  xarray.DataArray
+00013bd0: 0a20 2020 2020 2020 2020 2020 2046 726f  .            Fro
+00013be0: 7374 2066 7265 6520 7365 6173 6f6e 2065  st free season e
+00013bf0: 6e64 2e0a 0a20 2020 2020 2020 204e 6f74  nd...        Not
+00013c00: 6573 0a20 2020 2020 2020 202d 2d2d 2d2d  es.        -----
+00013c10: 0a20 2020 2020 2020 2046 6f72 206d 6f72  .        For mor
+00013c20: 6520 696e 666f 726d 6174 696f 6e20 6f6e  e information on
+00013c30: 2074 6865 2069 6e70 7574 2070 6172 616d   the input param
+00013c40: 6574 6572 7320 7365 653a 0a20 2020 2020  eters see:.     
+00013c50: 2020 2020 2020 2068 7474 7073 3a2f 2f78         https://x
+00013c60: 636c 696d 2e72 6561 6474 6865 646f 6373  clim.readthedocs
+00013c70: 2e69 6f2f 656e 2f73 7461 626c 652f 6170  .io/en/stable/ap
+00013c80: 692e 6874 6d6c 2378 636c 696d 2e69 6e64  i.html#xclim.ind
+00013c90: 6963 6174 6f72 732e 6174 6d6f 732e 6672  icators.atmos.fr
+00013ca0: 6f73 745f 6672 6565 5f73 6561 736f 6e5f  ost_free_season_
+00013cb0: 656e 640a 2020 2020 2020 2020 2222 220a  end.        """.
+00013cc0: 2020 2020 2020 2020 7468 7265 7368 203d          thresh =
+00013cd0: 205f 7468 7265 7368 5f73 7472 696e 6728   _thresh_string(
+00013ce0: 7468 7265 7368 2c20 2264 6567 4322 290a  thresh, "degC").
+00013cf0: 2020 2020 2020 2020 7265 7475 726e 2078          return x
+00013d00: 632e 6174 6d6f 732e 6672 6f73 745f 6672  c.atmos.frost_fr
+00013d10: 6565 5f73 6561 736f 6e5f 656e 6428 0a20  ee_season_end(. 
+00013d20: 2020 2020 2020 2020 2020 2074 6872 6573             thres
+00013d30: 683d 7468 7265 7368 2c0a 2020 2020 2020  h=thresh,.      
+00013d40: 2020 2020 2020 7769 6e64 6f77 3d77 696e        window=win
+00013d50: 646f 772c 0a20 2020 2020 2020 2020 2020  dow,.           
+00013d60: 202a 2a70 6172 616d 732c 0a20 2020 2020   **params,.     
+00013d70: 2020 2029 0a0a 0a63 6c61 7373 2046 473a     )...class FG:
+00013d80: 0a20 2020 2022 2222 4d65 616e 2064 6169  .    """Mean dai
+00013d90: 6c79 206d 6561 6e20 7769 6e64 2073 7065  ly mean wind spe
+00013da0: 6564 2e22 2222 0a0a 2020 2020 6465 6620  ed."""..    def 
+00013db0: 636f 6d70 7574 6528 2a2a 7061 7261 6d73  compute(**params
+00013dc0: 293a 0a20 2020 2020 2020 2022 2222 4361  ):.        """Ca
+00013dd0: 6c63 756c 6174 6520 6d65 616e 2064 6169  lculate mean dai
+00013de0: 6c79 206d 6561 6e20 7769 6e64 2073 7065  ly mean wind spe
+00013df0: 6564 2e0a 0a20 2020 2020 2020 2052 6574  ed...        Ret
+00013e00: 7572 6e73 0a20 2020 2020 2020 202d 2d2d  urns.        ---
+00013e10: 2d2d 2d2d 0a20 2020 2020 2020 2078 6172  ----.        xar
+00013e20: 7261 792e 4461 7461 4172 7261 790a 2020  ray.DataArray.  
+00013e30: 2020 2020 2020 2020 2020 4d65 616e 2064            Mean d
+00013e40: 6169 6c79 206d 6561 6e20 7769 6e64 2073  aily mean wind s
+00013e50: 7065 6564 2e0a 0a20 2020 2020 2020 204e  peed...        N
+00013e60: 6f74 6573 0a20 2020 2020 2020 202d 2d2d  otes.        ---
+00013e70: 2d2d 0a20 2020 2020 2020 2049 6620 7366  --.        If sf
+00013e80: 6357 696e 6420 6973 206e 6f74 2070 726f  cWind is not pro
+00013e90: 7669 6465 6420 696e 2060 6473 6020 7366  vided in `ds` sf
+00013ea0: 6357 696e 6420 636f 756c 6420 6265 2063  cWind could be c
+00013eb0: 6f6d 7075 7465 640a 2020 2020 2020 2020  omputed.        
+00013ec0: 6672 6f6d 2060 6473 602e 7561 7320 616e  from `ds`.uas an
+00013ed0: 6420 6064 7360 2e76 6173 2e0a 0a20 2020  d `ds`.vas...   
+00013ee0: 2020 2020 2046 6f72 2069 6e66 6f72 6d61       For informa
+00013ef0: 7469 6f6e 206f 6e20 7468 6520 696e 7075  tion on the inpu
+00013f00: 7420 7061 7261 6d65 7465 7273 2073 6565  t parameters see
+00013f10: 3a0a 2020 2020 2020 2020 2020 2020 6874  :.            ht
+00013f20: 7470 733a 2f2f 7863 6c69 6d2e 7265 6164  tps://xclim.read
+00013f30: 7468 6564 6f63 732e 696f 2f65 6e2f 7374  thedocs.io/en/st
+00013f40: 6162 6c65 2f61 7069 2e68 746d 6c23 7863  able/api.html#xc
+00013f50: 6c69 6d2e 696e 6469 6361 746f 7273 2e61  lim.indicators.a
+00013f60: 746d 6f73 2e73 6663 5769 6e64 5f6d 6561  tmos.sfcWind_mea
+00013f70: 6e0a 2020 2020 2020 2020 2222 220a 2020  n.        """.  
+00013f80: 2020 2020 2020 6966 2022 7366 6357 696e        if "sfcWin
+00013f90: 6422 206e 6f74 2069 6e20 7061 7261 6d73  d" not in params
+00013fa0: 5b22 6473 225d 3a0a 2020 2020 2020 2020  ["ds"]:.        
+00013fb0: 2020 2020 7061 7261 6d73 5b22 6473 225d      params["ds"]
+00013fc0: 5b22 7366 6357 696e 6422 5d20 3d20 7863  ["sfcWind"] = xc
+00013fd0: 2e61 746d 6f73 2e77 696e 645f 7370 6565  .atmos.wind_spee
+00013fe0: 645f 6672 6f6d 5f76 6563 746f 7228 0a20  d_from_vector(. 
+00013ff0: 2020 2020 2020 2020 2020 2020 2020 2064                 d
+00014000: 733d 7061 7261 6d73 5b22 6473 225d 2c0a  s=params["ds"],.
+00014010: 2020 2020 2020 2020 2020 2020 295b 305d              )[0]
+00014020: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00014030: 7863 2e61 746d 6f73 2e73 6663 5769 6e64  xc.atmos.sfcWind
+00014040: 5f6d 6561 6e28 2a2a 7061 7261 6d73 290a  _mean(**params).
+00014050: 0a0a 636c 6173 7320 4647 6e3a 0a20 2020  ..class FGn:.   
+00014060: 2022 2222 4d69 6e69 6d75 6d20 6461 696c   """Minimum dail
+00014070: 7920 6d65 616e 2077 696e 6420 7370 6565  y mean wind spee
+00014080: 642e 2222 220a 0a20 2020 2064 6566 2063  d."""..    def c
+00014090: 6f6d 7075 7465 282a 2a70 6172 616d 7329  ompute(**params)
+000140a0: 3a0a 2020 2020 2020 2020 2222 2243 616c  :.        """Cal
+000140b0: 6375 6c61 7465 206d 696e 696d 756d 2064  culate minimum d
+000140c0: 6169 6c79 206d 6561 6e20 7769 6e64 2073  aily mean wind s
+000140d0: 7065 6564 2e0a 0a20 2020 2020 2020 2052  peed...        R
+000140e0: 6574 7572 6e73 0a20 2020 2020 2020 202d  eturns.        -
+000140f0: 2d2d 2d2d 2d2d 0a20 2020 2020 2020 2078  ------.        x
+00014100: 6172 7261 792e 4461 7461 4172 7261 790a  array.DataArray.
+00014110: 2020 2020 2020 2020 2020 2020 4d69 6e69              Mini
+00014120: 6d75 6d20 6461 696c 7920 6d65 616e 2077  mum daily mean w
+00014130: 696e 6420 7370 6565 642e 0a0a 2020 2020  ind speed...    
+00014140: 2020 2020 4e6f 7465 730a 2020 2020 2020      Notes.      
+00014150: 2020 2d2d 2d2d 2d0a 2020 2020 2020 2020    -----.        
+00014160: 4966 2073 6663 5769 6e64 2069 7320 6e6f  If sfcWind is no
+00014170: 7420 7072 6f76 6964 6564 2069 6e20 6064  t provided in `d
+00014180: 7360 2073 6663 5769 6e64 2063 6f75 6c64  s` sfcWind could
+00014190: 2062 6520 636f 6d70 7574 6564 0a20 2020   be computed.   
+000141a0: 2020 2020 2066 726f 6d20 6064 7360 2e75       from `ds`.u
+000141b0: 6173 2061 6e64 2060 6473 602e 7661 732e  as and `ds`.vas.
+000141c0: 0a0a 2020 2020 2020 2020 466f 7220 696e  ..        For in
+000141d0: 666f 726d 6174 696f 6e20 6f6e 2074 6865  formation on the
+000141e0: 2069 6e70 7574 2070 6172 616d 6574 6572   input parameter
+000141f0: 7320 7365 653a 0a20 2020 2020 2020 2020  s see:.         
+00014200: 2020 2068 7474 7073 3a2f 2f78 636c 696d     https://xclim
+00014210: 2e72 6561 6474 6865 646f 6373 2e69 6f2f  .readthedocs.io/
+00014220: 656e 2f73 7461 626c 652f 6170 692e 6874  en/stable/api.ht
+00014230: 6d6c 2378 636c 696d 2e69 6e64 6963 6174  ml#xclim.indicat
+00014240: 6f72 732e 6174 6d6f 732e 7366 6357 696e  ors.atmos.sfcWin
+00014250: 645f 6d69 6e0a 2020 2020 2020 2020 2222  d_min.        ""
+00014260: 220a 2020 2020 2020 2020 6966 2022 7366  ".        if "sf
+00014270: 6357 696e 6422 206e 6f74 2069 6e20 7061  cWind" not in pa
+00014280: 7261 6d73 5b22 6473 225d 3a0a 2020 2020  rams["ds"]:.    
+00014290: 2020 2020 2020 2020 7061 7261 6d73 5b22          params["
+000142a0: 6473 225d 5b22 7366 6357 696e 6422 5d20  ds"]["sfcWind"] 
+000142b0: 3d20 7863 2e61 746d 6f73 2e77 696e 645f  = xc.atmos.wind_
+000142c0: 7370 6565 645f 6672 6f6d 5f76 6563 746f  speed_from_vecto
+000142d0: 7228 0a20 2020 2020 2020 2020 2020 2020  r(.             
+000142e0: 2020 2064 733d 7061 7261 6d73 5b22 6473     ds=params["ds
+000142f0: 225d 2c0a 2020 2020 2020 2020 2020 2020  "],.            
+00014300: 295b 305d 0a20 2020 2020 2020 2072 6574  )[0].        ret
+00014310: 7572 6e20 7863 2e61 746d 6f73 2e73 6663  urn xc.atmos.sfc
+00014320: 5769 6e64 5f6d 696e 282a 2a70 6172 616d  Wind_min(**param
+00014330: 7329 0a0a 0a63 6c61 7373 2046 4778 3a0a  s)...class FGx:.
+00014340: 2020 2020 2222 224d 6178 696d 756d 2064      """Maximum d
+00014350: 6169 6c79 206d 6561 6e20 7769 6e64 2073  aily mean wind s
+00014360: 7065 6564 2e22 2222 0a0a 2020 2020 6465  peed."""..    de
+00014370: 6620 636f 6d70 7574 6528 2a2a 7061 7261  f compute(**para
+00014380: 6d73 293a 0a20 2020 2020 2020 2022 2222  ms):.        """
+00014390: 4361 6c63 756c 6174 6520 6d61 7869 6d75  Calculate maximu
+000143a0: 6d20 6461 696c 7920 6d65 616e 2077 696e  m daily mean win
+000143b0: 6420 7370 6565 642e 0a0a 2020 2020 2020  d speed...      
+000143c0: 2020 5265 7475 726e 730a 2020 2020 2020    Returns.      
+000143d0: 2020 2d2d 2d2d 2d2d 2d0a 2020 2020 2020    -------.      
+000143e0: 2020 7861 7272 6179 2e44 6174 6141 7272    xarray.DataArr
+000143f0: 6179 0a20 2020 2020 2020 2020 2020 204d  ay.            M
+00014400: 6178 696d 756d 2064 6169 6c79 206d 6561  aximum daily mea
+00014410: 6e20 7769 6e64 2073 7065 6564 2e0a 0a20  n wind speed... 
+00014420: 2020 2020 2020 204e 6f74 6573 0a20 2020         Notes.   
+00014430: 2020 2020 202d 2d2d 2d2d 0a20 2020 2020       -----.     
+00014440: 2020 2049 6620 7366 6357 696e 6420 6973     If sfcWind is
+00014450: 206e 6f74 2070 726f 7669 6465 6420 696e   not provided in
+00014460: 2060 6473 6020 7366 6357 696e 6420 636f   `ds` sfcWind co
+00014470: 756c 6420 6265 2063 6f6d 7075 7465 640a  uld be computed.
+00014480: 2020 2020 2020 2020 6672 6f6d 2060 6473          from `ds
+00014490: 602e 7561 7320 616e 6420 6064 7360 2e76  `.uas and `ds`.v
+000144a0: 6173 2e0a 0a20 2020 2020 2020 2046 6f72  as...        For
+000144b0: 2069 6e66 6f72 6d61 7469 6f6e 206f 6e20   information on 
+000144c0: 7468 6520 696e 7075 7420 7061 7261 6d65  the input parame
+000144d0: 7465 7273 2073 6565 3a0a 2020 2020 2020  ters see:.      
+000144e0: 2020 2020 2020 6874 7470 733a 2f2f 7863        https://xc
+000144f0: 6c69 6d2e 7265 6164 7468 6564 6f63 732e  lim.readthedocs.
+00014500: 696f 2f65 6e2f 7374 6162 6c65 2f61 7069  io/en/stable/api
+00014510: 2e68 746d 6c23 7863 6c69 6d2e 696e 6469  .html#xclim.indi
+00014520: 6361 746f 7273 2e61 746d 6f73 2e73 6663  cators.atmos.sfc
+00014530: 5769 6e64 5f6d 6178 0a20 2020 2020 2020  Wind_max.       
+00014540: 2022 2222 0a20 2020 2020 2020 2069 6620   """.        if 
+00014550: 2273 6663 5769 6e64 2220 6e6f 7420 696e  "sfcWind" not in
+00014560: 2070 6172 616d 735b 2264 7322 5d3a 0a20   params["ds"]:. 
+00014570: 2020 2020 2020 2020 2020 2070 6172 616d             param
+00014580: 735b 2264 7322 5d5b 2273 6663 5769 6e64  s["ds"]["sfcWind
+00014590: 225d 203d 2078 632e 6174 6d6f 732e 7769  "] = xc.atmos.wi
+000145a0: 6e64 5f73 7065 6564 5f66 726f 6d5f 7665  nd_speed_from_ve
+000145b0: 6374 6f72 280a 2020 2020 2020 2020 2020  ctor(.          
+000145c0: 2020 2020 2020 6473 3d70 6172 616d 735b        ds=params[
+000145d0: 2264 7322 5d2c 0a20 2020 2020 2020 2020  "ds"],.         
+000145e0: 2020 2029 5b30 5d0a 2020 2020 2020 2020     )[0].        
+000145f0: 7265 7475 726e 2078 632e 6174 6d6f 732e  return xc.atmos.
+00014600: 7366 6357 696e 645f 6d61 7828 2a2a 7061  sfcWind_max(**pa
+00014610: 7261 6d73 290a 0a0a 636c 6173 7320 4658  rams)...class FX
+00014620: 3a0a 2020 2020 2222 224d 6561 6e20 6461  :.    """Mean da
+00014630: 696c 7920 6d61 7869 6d75 6d20 7769 6e64  ily maximum wind
+00014640: 2073 7065 6564 2e22 2222 0a0a 2020 2020   speed."""..    
+00014650: 6465 6620 636f 6d70 7574 6528 2a2a 7061  def compute(**pa
+00014660: 7261 6d73 293a 0a20 2020 2020 2020 2022  rams):.        "
+00014670: 2222 4361 6c63 756c 6174 6520 6d65 616e  ""Calculate mean
+00014680: 2064 6169 6c79 206d 6178 696d 756d 2077   daily maximum w
+00014690: 696e 6420 7370 6565 642e 0a0a 2020 2020  ind speed...    
+000146a0: 2020 2020 5265 7475 726e 730a 2020 2020      Returns.    
+000146b0: 2020 2020 2d2d 2d2d 2d2d 2d0a 2020 2020      -------.    
+000146c0: 2020 2020 7861 7272 6179 2e44 6174 6141      xarray.DataA
+000146d0: 7272 6179 0a20 2020 2020 2020 2020 2020  rray.           
+000146e0: 204d 6561 6e20 6461 696c 7920 6d61 7869   Mean daily maxi
+000146f0: 6d75 6d20 7769 6e64 2073 7065 6564 2e0a  mum wind speed..
+00014700: 0a20 2020 2020 2020 204e 6f74 6573 0a20  .        Notes. 
+00014710: 2020 2020 2020 202d 2d2d 2d2d 0a20 2020         -----.   
+00014720: 2020 2020 2046 6f72 2069 6e66 6f72 6d61       For informa
+00014730: 7469 6f6e 206f 6e20 7468 6520 696e 7075  tion on the inpu
+00014740: 7420 7061 7261 6d65 7465 7273 2073 6565  t parameters see
+00014750: 3a0a 2020 2020 2020 2020 2020 2020 6874  :.            ht
+00014760: 7470 733a 2f2f 7863 6c69 6d2e 7265 6164  tps://xclim.read
+00014770: 7468 6564 6f63 732e 696f 2f65 6e2f 7374  thedocs.io/en/st
+00014780: 6162 6c65 2f61 7069 2e68 746d 6c23 7863  able/api.html#xc
+00014790: 6c69 6d2e 696e 6469 6361 746f 7273 2e61  lim.indicators.a
+000147a0: 746d 6f73 2e73 6663 5769 6e64 6d61 785f  tmos.sfcWindmax_
+000147b0: 6d65 616e 0a20 2020 2020 2020 2022 2222  mean.        """
+000147c0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+000147d0: 7863 2e61 746d 6f73 2e73 6663 5769 6e64  xc.atmos.sfcWind
+000147e0: 6d61 785f 6d65 616e 282a 2a70 6172 616d  max_mean(**param
+000147f0: 7329 0a0a 0a63 6c61 7373 2046 586e 3a0a  s)...class FXn:.
+00014800: 2020 2020 2222 224d 696e 696d 756d 2064      """Minimum d
+00014810: 6169 6c79 206d 6178 696d 756d 2077 696e  aily maximum win
+00014820: 6420 7370 6565 642e 2222 220a 0a20 2020  d speed."""..   
+00014830: 2064 6566 2063 6f6d 7075 7465 282a 2a70   def compute(**p
+00014840: 6172 616d 7329 3a0a 2020 2020 2020 2020  arams):.        
+00014850: 2222 2243 616c 6375 6c61 7465 206d 696e  """Calculate min
+00014860: 696d 756d 2064 6169 6c79 206d 6178 696d  imum daily maxim
+00014870: 756d 2077 696e 6420 7370 6565 642e 0a0a  um wind speed...
+00014880: 2020 2020 2020 2020 5265 7475 726e 730a          Returns.
+00014890: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d0a          -------.
+000148a0: 2020 2020 2020 2020 7861 7272 6179 2e44          xarray.D
+000148b0: 6174 6141 7272 6179 0a20 2020 2020 2020  ataArray.       
+000148c0: 2020 2020 204d 696e 696d 756d 2064 6169       Minimum dai
+000148d0: 6c79 206d 6178 696d 756d 2077 696e 6420  ly maximum wind 
+000148e0: 7370 6565 642e 0a0a 2020 2020 2020 2020  speed...        
+000148f0: 4e6f 7465 730a 2020 2020 2020 2020 2d2d  Notes.        --
+00014900: 2d2d 2d0a 2020 2020 2020 2020 466f 7220  ---.        For 
+00014910: 696e 666f 726d 6174 696f 6e20 6f6e 2074  information on t
+00014920: 6865 2069 6e70 7574 2070 6172 616d 6574  he input paramet
+00014930: 6572 7320 7365 653a 0a20 2020 2020 2020  ers see:.       
+00014940: 2020 2020 2068 7474 7073 3a2f 2f78 636c       https://xcl
+00014950: 696d 2e72 6561 6474 6865 646f 6373 2e69  im.readthedocs.i
+00014960: 6f2f 656e 2f73 7461 626c 652f 6170 692e  o/en/stable/api.
+00014970: 6874 6d6c 2378 636c 696d 2e69 6e64 6963  html#xclim.indic
+00014980: 6174 6f72 732e 6174 6d6f 732e 7366 6357  ators.atmos.sfcW
+00014990: 696e 646d 6178 5f6d 696e 0a20 2020 2020  indmax_min.     
+000149a0: 2020 2022 2222 0a20 2020 2020 2020 2072     """.        r
+000149b0: 6574 7572 6e20 7863 2e61 746d 6f73 2e73  eturn xc.atmos.s
+000149c0: 6663 5769 6e64 6d61 785f 6d69 6e28 2a2a  fcWindmax_min(**
+000149d0: 7061 7261 6d73 290a 0a0a 636c 6173 7320  params)...class 
+000149e0: 4658 783a 0a20 2020 2022 2222 4d61 7869  FXx:.    """Maxi
+000149f0: 6d75 6d20 6461 696c 7920 6d61 7869 6d75  mum daily maximu
+00014a00: 6d20 7769 6e64 2073 7065 6564 2e22 2222  m wind speed."""
+00014a10: 0a0a 2020 2020 6465 6620 636f 6d70 7574  ..    def comput
+00014a20: 6528 2a2a 7061 7261 6d73 293a 0a20 2020  e(**params):.   
+00014a30: 2020 2020 2022 2222 4361 6c63 756c 6174       """Calculat
+00014a40: 6520 6d61 7869 6d75 6d20 6461 696c 7920  e maximum daily 
+00014a50: 6d61 7869 6d75 6d20 7769 6e64 2073 7065  maximum wind spe
+00014a60: 6564 2e0a 0a20 2020 2020 2020 2052 6574  ed...        Ret
+00014a70: 7572 6e73 0a20 2020 2020 2020 202d 2d2d  urns.        ---
+00014a80: 2d2d 2d2d 0a20 2020 2020 2020 2078 6172  ----.        xar
+00014a90: 7261 792e 4461 7461 4172 7261 790a 2020  ray.DataArray.  
+00014aa0: 2020 2020 2020 2020 2020 4d61 7869 6d75            Maximu
+00014ab0: 6d20 6461 696c 7920 6d61 7869 6d75 6d20  m daily maximum 
+00014ac0: 7769 6e64 2073 7065 6564 2e0a 0a20 2020  wind speed...   
+00014ad0: 2020 2020 204e 6f74 6573 0a20 2020 2020       Notes.     
+00014ae0: 2020 202d 2d2d 2d2d 0a20 2020 2020 2020     -----.       
+00014af0: 2046 6f72 2069 6e66 6f72 6d61 7469 6f6e   For information
+00014b00: 206f 6e20 7468 6520 696e 7075 7420 7061   on the input pa
+00014b10: 7261 6d65 7465 7273 2073 6565 3a0a 2020  rameters see:.  
+00014b20: 2020 2020 2020 2020 2020 6874 7470 733a            https:
+00014b30: 2f2f 7863 6c69 6d2e 7265 6164 7468 6564  //xclim.readthed
+00014b40: 6f63 732e 696f 2f65 6e2f 7374 6162 6c65  ocs.io/en/stable
+00014b50: 2f61 7069 2e68 746d 6c23 7863 6c69 6d2e  /api.html#xclim.
+00014b60: 696e 6469 6361 746f 7273 2e61 746d 6f73  indicators.atmos
+00014b70: 2e73 6663 5769 6e64 6d61 785f 6d61 780a  .sfcWindmax_max.
+00014b80: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00014b90: 2020 2020 7265 7475 726e 2078 632e 6174      return xc.at
+00014ba0: 6d6f 732e 7366 6357 696e 646d 6178 5f6d  mos.sfcWindmax_m
+00014bb0: 6178 282a 2a70 6172 616d 7329 0a         ax(**params).
```

### Comparing `index_calculator-0.7.6/index_calculator/_outputwriter.py` & `index_calculator-0.8.0/index_calculator/_outputwriter.py`

 * *Files 5% similar despite different names*

```diff
@@ -93,15 +93,15 @@
                 print("Could not write output.")
                 continue
             outputname = Path(os.path.join(output_dir, output_name)).resolve()
             ds_dict[output_name] = self._to_netcdf(ds_, outputname)
 
     def _parse_components_to_format(self, ds, out_components, out_format):
         def test_ocomp(ocomp):
-            return ocomp.replace("/", "").replace(" ", "")
+            return ocomp.replace("/", "").replace(" ", "").replace(".", "-")
 
         ocomps = []
         for comp in out_components:
             if hasattr(ds, comp):
                 ocomps.append(test_ocomp(getattr(ds, comp)))
             elif hasattr(self.proc, comp):
                 ocomps.append(test_ocomp(getattr(self.proc, comp)))
```

### Comparing `index_calculator-0.7.6/index_calculator/_postprocessing.py` & `index_calculator-0.8.0/index_calculator/_postprocessing.py`

 * *Files identical despite different names*

### Comparing `index_calculator-0.7.6/index_calculator/_processing.py` & `index_calculator-0.8.0/index_calculator/_processing.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,14 +99,16 @@
                     continue
                 replacement[attr] = numb_name
             else:
                 replacement[attr] = getattr(obj, attr)
             if isinstance(replacement[attr], list):
                 continue
             if isinstance(replacement[attr], str):
+                if not replacement[attr].isnumeric():
+                    continue
                 if replacement[attr][0] == "0":
                     replacement[attr] = float(
                         "{}.{}".format(
                             replacement[attr][0],
                             replacement[attr][1:],
                         )
                     )
@@ -126,14 +128,16 @@
             if k in defaults and k in self.kwargs.keys():
                 if "YY" in self.CIname:
                     self.CIname = self.CIname.replace("YY", str(v))
                 elif isinstance(v, list):
                     continue
                 elif isinstance(v, bool):
                     continue
+                elif isinstance(v, str):
+                    continue
                 elif numb_name is not None:
                     self.CIname = self.CIname.replace(
                         numb_name,
                         v,
                     )
                 elif str(v) not in self.CIname:
                     self.CIname = "{}{}".format(self.CIname, str(v))
```

### Comparing `index_calculator-0.7.6/index_calculator/_tables.py` & `index_calculator-0.8.0/index_calculator/_tables.py`

 * *Files 22% similar despite different names*

```diff
@@ -20,9 +20,7 @@
         return json.load(f)
 
 
 mjson = read_from_json("tables/metadata.json")
 xjson = read_from_json("tables/xcalc.json")
 pjson = read_from_json("tables/projects.json")
 vjson = read_from_json("tables/input_vars.json")
-cfjson = read_from_json("tables/cf_conversion.json")
-cjson = read_from_json("tables/convert_to_frequencies.json")
```

### Comparing `index_calculator-0.7.6/index_calculator/_utils.py` & `index_calculator-0.8.0/index_calculator/_utils.py`

 * *Files identical despite different names*

### Comparing `index_calculator-0.7.6/index_calculator/cli.py` & `index_calculator-0.8.0/index_calculator/cli.py`

 * *Files identical despite different names*

### Comparing `index_calculator-0.7.6/index_calculator/index_calculator.py` & `index_calculator-0.8.0/index_calculator/index_calculator.py`

 * *Files identical despite different names*

### Comparing `index_calculator-0.7.6/index_calculator/tables/input_vars.json` & `index_calculator-0.8.0/index_calculator/tables/input_vars.json`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9783950617283951%*

 * *Differences: {"'default'": "{'LFD': 'tasmin', 'DSn': 'pr', 'WSn': 'pr', 'HSn': 'tasmax', 'CSx': 'tas', 'CSn': "*

 * *              "'tas', 'HWn': ['tasmax', 'tasmin']}"}*

```diff
@@ -24,21 +24,24 @@
         ],
         "CDD": "pr",
         "CFD": "tasmin",
         "CHDYYx": "tasmax",
         "CSDI": "tasmin",
         "CSU": "tasmax",
         "CSf": "tas",
+        "CSn": "tas",
+        "CSx": "tas",
         "CW": [
             "tas",
             "pr"
         ],
         "CWD": "pr",
         "DD": "pr",
         "DSf": "pr",
+        "DSn": "pr",
         "DSx": "pr",
         "DTR": [
             "tasmax",
             "tasmin"
         ],
         "FD": "tasmin",
         "FFE": "tasmin",
@@ -50,24 +53,30 @@
         "FXn": "sfcWindmax",
         "FXx": "sfcWindmax",
         "GD": "tas",
         "GSE": "tas",
         "GSS": "tas",
         "HD17": "tas",
         "HSf": "tasmax",
+        "HSn": "tasmax",
         "HSx": "tasmax",
         "HWf": [
             "tasmax",
             "tasmin"
         ],
+        "HWn": [
+            "tasmax",
+            "tasmin"
+        ],
         "HWx": [
             "tasmax",
             "tasmin"
         ],
         "ID": "tasmax",
+        "LFD": "tasmin",
         "PRCPTOT": "pr",
         "R10mm": "pr",
         "R20mm": "pr",
         "R25mm": "pr",
         "RDYYp": "pr",
         "RR": "pr",
         "RR1": "pr",
@@ -112,14 +121,15 @@
         "WD": [
             "tas",
             "pr"
         ],
         "WI": "tasmin",
         "WSDI": "tasmax",
         "WSf": "pr",
+        "WSn": "pr",
         "WSx": "pr",
         "WW": [
             "tas",
             "pr"
         ]
     }
 }
```

### Comparing `index_calculator-0.7.6/index_calculator/tables/metadata.json` & `index_calculator-0.8.0/index_calculator/tables/metadata.json`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9015625%*

 * *Differences: {"'CSU'": "{'long_name': 'Maximum number of consecutive summer days (maximum temperature > "*

 * *          "{thresh} degC)', 'description': 'Maximum count of consecutive days with daily maximum "*

 * *          "temperature above {thresh} degC.'}",*

 * * "'CSf'": "{'description': 'Total number of series of at least {window} consecutive days with "*

 * *          "temperature below {thresh} degC.'}",*

 * * "'CSn'": "OrderedDict([('standard_name', 'cold_spell_days'), ('long_name', 'Total number of days "*

 * *          "in cold spells (t […]*

```diff
@@ -26,25 +26,37 @@
     "CSDI": {
         "description": "Number of days within periods of at least {window} consecutive days with minimum temperature below the 10th percentile.",
         "long_name": "Cold spell duration index (days within periods >= {window} consecutive days with minimum temperature < 10th percentile)",
         "standard_name": "consecutive_days_with_air_temperature_below_threshold",
         "units": "days"
     },
     "CSU": {
-        "description": "Maximum count of consecutive days with daily maximum temperature above {tresh} degC.",
-        "long_name": "Maximum number of consecutive summer days (maximum temperature > {threh} degC)",
+        "description": "Maximum count of consecutive days with daily maximum temperature above {thresh} degC.",
+        "long_name": "Maximum number of consecutive summer days (maximum temperature > {thresh} degC)",
         "standard_name": "consecutive_days_with_air_temperature_above_threshold",
         "units": "days"
     },
     "CSf": {
-        "description": "Total number of series of at least {window} consecutive days with temperature below {thresh}.",
+        "description": "Total number of series of at least {window} consecutive days with temperature below {thresh} degC.",
         "long_name": "Number of cold spells (temperature < {thresh} degC)",
         "standard_name": "cold_spell_frequency",
         "units": ""
     },
+    "CSn": {
+        "description": "Total number of days in series of at least {window} consecutive days with temperature below {thresh} degC.",
+        "long_name": "Total number of days in cold spells (temperature < {thresh} degC)",
+        "standard_name": "cold_spell_days",
+        "units": "days"
+    },
+    "CSx": {
+        "description": "Longest series of at least {window} consecutive days with temperature below {thresh} degC.",
+        "long_name": "Maximum length of cold spells (temperature < {thresh} degC)",
+        "standard_name": "cold_spell_duration",
+        "units": "days"
+    },
     "CW": {
         "description": "Number of days with daily mean temperature below the 25th percentile and total daily precipitation amount above the 75th percentile.",
         "long_name": "Number of cold and wet days",
         "standard_name": "cold_and_wet_days",
         "units": "days"
     },
     "CWD": {
@@ -56,22 +68,28 @@
     "DD": {
         "description": "Number of days with daily total precipitation below {thresh} mm.",
         "long_name": "Number of dry days (precipitation < {thresh} mm)",
         "standard_name": "days_with_precipitation_amount_below_threshold",
         "units": "days"
     },
     "DSf": {
-        "description": "Total number of series of at least {window} consecutive days with precipitation below {thresh} mm/day.",
-        "long_name": "Number of dry spells (precipitation < {thresh} mm/day)",
+        "description": "Total number of series of at least {window} consecutive days with precipitation below {thresh} mm.",
+        "long_name": "Number of dry spells (precipitation < {thresh} mm)",
         "standard_name": "dry_spell_frequency",
         "units": ""
     },
+    "DSn": {
+        "description": "Total number of days in series of at least {window} consecutive days with precipitation below {thresh} mm.",
+        "long_name": "Total number of days in dry spells (precipitation < {thresh} mm)",
+        "standard_name": "dry_spell_days",
+        "units": "days"
+    },
     "DSx": {
-        "description": "Longest series of at least {window} consecutive days with precipitation below {thresh} mm/day.",
-        "long_name": "Maximum lenght of dry spells (precipitation < {thresh} mm/day)",
+        "description": "Longest series of at least {window} consecutive days with precipitation below {thresh} mm.",
+        "long_name": "Maximum lenght of dry spells (precipitation < {thresh} mm)",
         "standard_name": "dry_spell_duration",
         "units": "days"
     },
     "DTR": {
         "description": "Mean diurnal temperature range (difference between daily maximum temperature and daily minimum temperature).",
         "long_name": "Mean diurnal temperature range (difference between maximum and minimum temperature)",
         "standard_name": "air_temperature",
@@ -152,43 +170,61 @@
     "HD17": {
         "description": "Cumulative sum of temperature degrees for daily mean temperature below 17 degC.",
         "long_name": "Cumulative heating degree days (mean temperature < 17 degC)",
         "standard_name": "degree_days_for_days_with_air_temperature_below_threshold",
         "units": "degree_day"
     },
     "HSf": {
-        "description": "Total number of series of at least {window} consecutive days with maximum temperature above {thresh}.",
+        "description": "Total number of series of at least {window} consecutive days with maximum temperature above {thresh} degC.",
         "long_name": "Number of hot spells (maximum temperature > {thresh} degC)",
         "standard_name": "hot_spell_frequency",
         "units": ""
     },
+    "HSn": {
+        "description": "Total number of days in series of at least {window} consecutive days with maximum temperature above {thresh} degC.",
+        "long_name": "Total number of days in hot spells (maximum temperature > {thresh} degC)",
+        "standard_name": "hot_spell_days",
+        "units": "days"
+    },
     "HSx": {
-        "description": "Longest series of at least {window} consecutive days with maximum temperature above {thresh}.",
+        "description": "Longest series of at least {window} consecutive days with maximum temperature above {thresh} degC.",
         "long_name": "Maximum length of hot spells (maximum temperature > {thresh} degC)",
         "standard_name": "hot_spell_duration",
         "units": "days"
     },
     "HWf": {
         "description": "Total number of serires of at least {window} consecutive days with maximum temperature above {thresh_tasmax} degC and minimum temperature above {thresh_tasmin} degC).",
         "long_name": "Number of heat waves (maximum temperature > {thresh_tasmax} degC and minimum temperature > {thresh_tasmin} degC)",
         "standard_name": "heat_wave_frequency",
         "units": ""
     },
+    "HWn": {
+        "description": "Total number of days in series of at least {window} consecutive days with maximum temperature above {thresh_tasmax} degC and minimum temperature above {thresh_tasmin} degC).",
+        "long_name": "Total number of days in heat waves (maximum temperature > {thresh_tasmax} degC and minimum temperature > {thresh_tasmin} degC)",
+        "standard_name": "heat_wave_days",
+        "units": "days"
+    },
     "HWx": {
         "description": "Longest series of at least {window} consecutive days with maximum temperature above {thresh_tasmax} degC and minimum temperature above {thresh_tasmin} degC).",
         "long_name": "Maximum length of heat waves (maximum temperature > {thresh_tasmax} degC and minimum temperature > {thresh_tasmin} degC)",
         "standard_name": "heat_wave_duration",
         "units": "days"
     },
     "ID": {
         "description": "Number of days with daily maximum temperature below 0 degC.",
         "long_name": "Number of ice days (maximum temperature < 0 degC)",
         "standard_name": "days_with_air_temperature_below_threshold",
         "units": "days"
     },
+    "LFD": {
+        "description": "Number of days with daily minimum temperature below 0 degC between {start_date} and {end_date}.",
+        "long_name": "Number of late frost days (minimum temperature < 0 degC)",
+        "standard_name": "days_with_air_temperature_below_threshold",
+        "units": "days"
+    },
     "PRCPTOT": {
         "description": "Sum of daily total precipitation amount on days with total precipitation above or equal {thresh} mm).",
         "long_name": "Total precipitation amount of wet days (precipitation >= {thresh} mm)",
         "standard_name": "precipitation",
         "units": "mm"
     },
     "R10mm": {
@@ -297,15 +333,15 @@
         "description": "Number of days with daily maximum temperature above {thresh} degC.",
         "long_name": "Number of summer days (maximum temperature > {thresh} degC)",
         "standard_name": "days_with_air_temperature_above_or_equal_threshold",
         "units": "days"
     },
     "Sfreq": {
         "description": "Snowfall intensity is derived by dividing the total number of days with snowfall > {thresh} mm (liquid water equivalent) by the total number of days within the analysed time period.",
-        "long_name": "Percentage of days with snowfall flux > {thresh} mm/day",
+        "long_name": "Percentage of days with snowfall flux > {thresh} mm",
         "standard_name": "snowfall_frequency",
         "units": "%"
     },
     "Sint": {
         "description": "Mean snowfall flux above {thresh} mm (liquid water equivalent).",
         "long_name": "Mean snowfall during days with snowfall > {thresh} mm",
         "standard_name": "snowfall_intensity",
@@ -416,22 +452,28 @@
     "WSDI": {
         "description": "Number of days within periods of at least {window} consecutive days with maximum temperature above the 90th percentile.",
         "long_name": "Warm spell duration index (days within periods >= {window} consecutive days with minimum temperature > 90th percentile)",
         "standard_name": "consecutive_days_with_air_temperature_above_threshold",
         "units": "days"
     },
     "WSf": {
-        "description": "Total number of series of at least {window} consecutive days with precipitation above {thresh} mm/day.",
-        "long_name": "Number of wet spells (precipitation >= {thresh} mm/day)",
+        "description": "Total number of series of at least {window} consecutive days with precipitation above {thresh} mm.",
+        "long_name": "Number of wet spells (precipitation >= {thresh} mm)",
         "standard_name": "wet_spell_frequency",
         "units": ""
     },
+    "WSn": {
+        "description": "Total number of days in series of at least {window} consecutive days with precipitation above {thresh} mm.",
+        "long_name": "Total number of days in wet spells (precipitation >= {thresh} mm)",
+        "standard_name": "wet_spell_days",
+        "units": "days"
+    },
     "WSx": {
-        "description": "Longest series of at least {window} consecutive days with precipitation above {thresh} mm/day.",
-        "long_name": "Maximum lenght of wet spells (precipitation >= {thresh} mm/day)",
+        "description": "Longest series of at least {window} consecutive days with precipitation above {thresh} mm.",
+        "long_name": "Maximum lenght of wet spells (precipitation >= {thresh} mm)",
         "standard_name": "wet_spell_duration",
         "units": "days"
     },
     "WW": {
         "description": "Number of days with daily mean temperature above the 75th percentile and total daily precipitation amount above the 75th percentile.",
         "long_name": "Number of warm & wet days",
         "standard_name": "warm_and_wet_days",
```

### Comparing `index_calculator-0.7.6/index_calculator/tables/projects.json` & `index_calculator-0.8.0/index_calculator/tables/projects.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9791666666666666%*

 * *Differences: {"'EOBS'": "{'iformat': '{}_ens_mean_0-1deg_reg_v{}.nc'}",*

 * * "'ERA5'": "{'icomponents': 'era_level, frequency, timerange, variable_id', 'iformat': "*

 * *           "'{}_{}_{}_{}.nc'}"}*

```diff
@@ -25,23 +25,23 @@
     },
     "EOBS": {
         "components": "ci_name, E-OBS_version, ci_institute_id, ci_frequency, ci_timerange_index",
         "drs_components": "ci_institute_id, E-OBS_version, ci_frequency, ci_name, ci_package_reference",
         "drs_format": "eobs/{}/0.1deg/{}/{}/{}/{}",
         "format": "{}_ens_mean_0.1deg_reg_v{}_{}_{}_{}.nc",
         "icomponents": "variable_id, resolution, E-OBS_version",
-        "iformat": "{}_ens_mean_0.1deg_reg_v{}.nc"
+        "iformat": "{}_ens_mean_0-1deg_reg_v{}.nc"
     },
     "ERA5": {
         "components": "ci_name, frequency, ci_institute_id, ci_frequency, ci_timerange_index",
         "drs_components": "ci_institute_id, ci_frequency, ci_name, ci_package_reference",
         "drs_format": "era5/{}/{}/{}/{}",
         "format": "{}_era5_{}_{}_{}_{}.nc",
-        "icomponents": "variable_id, frequency, date",
-        "iformat": "{}_era5_{}_{}.nc"
+        "icomponents": "era_level, frequency, timerange, variable_id",
+        "iformat": "{}_{}_{}_{}.nc"
     },
     "HYRAS": {
         "components": "ci_name, horizontal_resolution, realization, ci_frequency, ci_timerange_index",
         "drs_components": "ci_institute_id, realization, horizontal_resolution, ci_frequency, ci_name, ci_package_reference",
         "drs_format": "hyras/{}/{}/{}/{}/{}/{}",
         "format": "{}_hyras_{}_{}_{}_de_{}.nc",
         "icomponents": "variable_id, horizontal_resolution, year, realization",
```

### Comparing `index_calculator-0.7.6/index_calculator/tables/xcalc.json` & `index_calculator-0.8.0/index_calculator/tables/xcalc.json`

 * *Files identical despite different names*

### Comparing `index_calculator-0.7.6/index_calculator.egg-info/PKG-INFO` & `index_calculator-0.8.0/index_calculator.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: index-calculator
-Version: 0.7.6
+Version: 0.8.0
 Summary: Python index-calculator is an xclim wrapperto calculate climate indices from CMORized netCDF files.
 Home-page: https://github.com/ludwiglierhammer/index_calculator
 Author: Ludwig Lierhammer
 Author-email: ludwig.lierhammer@hereon.de
 License: MIT license
 Keywords: index_calculator
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -227,14 +227,15 @@
 * restructuring time encoding
 * properties removed
 
 0.5.0 (2023-01-04)
 ------------------
 
 * new indices:
+
   * CSf (Number of cold spells)
   * HSf (Number of hot spells)
   * HSx (Maximum length of hot spells)
   * SD (Number od snow days)
   * SCD (Snow cover duration)
   * Sint (Snowfall intensity)
   * Sfreq (Snowfall freqeuncy)
@@ -276,21 +277,23 @@
 
 * time controlling to pyhomogenize
 
 0.6.0 (2023-03-03)
 ------------------
 
 * new indices:
+
   * HW: maximum length of heat waves
   * GSS: start of growing season
   * GSE: end of growing season
   * FFS: start of frost-free season
   * FFE: end of frost-free season
   * RRm: mean daily precipitation
   * RRYYp: precipitation percentile value
+
 * rename RYYp to RYYpABS and RDYYP to RYYp according to ICCLIM
 * optional argument perc woth percentile indicators
 
 0.6.1 (2023-03-09)
 ------------------
 
 * some metadata corrections
@@ -341,14 +344,15 @@
 
 * calculating percentile indices with non-standard calendar
 
 0.7.2 (2023-05-10)
 ------------------
 
 * new indicators implemented:
+
   * FG (mean daily wind speed)
   * FGn (minimum od mean daily wind speed)
   * FGx (maximum of mean daily wind speed)
   * FX (mean of maximum daily wind speed)
   * FXn (minimum of daily maximum wind speed)
   * FXx (maximum of daily maximum wind speed)
 
@@ -380,7 +384,25 @@
 * calcualte climate indicators for ERA5 data
 * input variable for WI is tasmin not tas
 
 0.7.6 (2023-06-20)
 ------------------
 
 * outsourcing test data to github repository https://github.com/ludwiglierhammer/test_data
+
+0.8.0 (2023-07-13)
+------------------
+* optionally: calculate SCD with water equivalent input
+* replace '.' with '-' in directory structure and output file names
+* new climate indicators:
+
+  * DSn: total number of days in dry spells
+  * WSn: total number of days in wet spells
+  * CSx: maximum length of cold spell
+  * CSn: total number of days in cold spells
+  * HSn: total number of days in hot spells
+  * HWn: total number of days in heat waves
+  * LFD: number of late frost days
+
+* metadata: set mm/day to mm
+* fixing v0.7.3 and v0.7.4 with xclim>=0.44
+* redo v0.7.5 (if dataset frequency is not equal input frequency, convert it; adding hourly test data)
```

### Comparing `index_calculator-0.7.6/setup.py` & `index_calculator-0.8.0/setup.py`

 * *Files identical despite different names*

### Comparing `index_calculator-0.7.6/tests/test_index_calculator.py` & `index_calculator-0.8.0/tests/test_index_calculator.py`

 * *Files identical despite different names*

### Comparing `index_calculator-0.7.6/tests/test_indices.py` & `index_calculator-0.8.0/tests/test_indices.py`

 * *Files 1% similar despite different names*

```diff
@@ -180,14 +180,24 @@
 
 
 def test_FD():
     result = indices.FD.compute(tasmin=tasmin_xarray(), freq="7D")
     np.testing.assert_allclose(result, 5, rtol=1e-03)
 
 
+def test_LFD():
+    result = indices.LFD.compute(
+        tasmin=tasmin_xarray(),
+        freq="7D",
+        start_date="01-04",
+        end_date="01-07",
+    )
+    np.testing.assert_allclose(result, 2, rtol=1e-03)
+
+
 def test_ID():
     result = indices.ID.compute(tasmax=tasmax_xarray(), freq="7D")
     np.testing.assert_allclose(result, 3, rtol=1e-03)
 
 
 def test_TX():
     result = indices.TX.compute(tasmax=tasmax_xarray(), freq="7D")
@@ -262,30 +272,40 @@
 
 def test_CSU():
     result = indices.CSU.compute(tasmax=tasmax_xarray(), freq="7D")
     np.testing.assert_allclose(result, 1, rtol=1e-03)
 
 
 def test_DSf():
-    result = indices.DSf.compute(pr=pr_xarray(), freq="7D")
+    result = indices.DSf.compute(pr=pr_xarray(), window=2, freq="7D")
     np.testing.assert_allclose(result, 0, rtol=1e-03)
 
 
 def test_DSx():
-    result = indices.DSx.compute(pr=pr_xarray(), freq="7D")
+    result = indices.DSx.compute(pr=pr_xarray(), window=1, freq="7D")
     np.testing.assert_allclose(result, 1, rtol=1e-03)
 
 
-def test_WSf():
-    result = indices.WSf.compute(pr=pr_xarray(), freq="7D")
+def test_DSn():
+    result = indices.DSn.compute(pr=pr_xarray(), window=1, freq="7D")
     np.testing.assert_allclose(result, 1, rtol=1e-03)
 
 
+def test_WSf():
+    result = indices.WSf.compute(pr=pr_xarray(), window=1, freq="7D")
+    np.testing.assert_allclose(result, 2, rtol=1e-03)
+
+
 def test_WSx():
-    result = indices.WSx.compute(pr=pr_xarray(), freq="7D")
+    result = indices.WSx.compute(pr=pr_xarray(), window=1, freq="7D")
+    np.testing.assert_allclose(result, 1, rtol=1e-03)
+
+
+def test_WSn():
+    result = indices.WSn.compute(pr=pr_xarray(), window=1, freq="7D")
     np.testing.assert_allclose(result, 1, rtol=1e-03)
 
 
 def test_RYYp():
     result = indices.RYYp.compute(
         pr=pr_xarray(),
         freq="7D",
@@ -478,14 +498,33 @@
         freq="7D",
         thresh=-10,
         window=1,
     )
     np.testing.assert_allclose(result, 2, rtol=1e-03)
 
 
+def test_CSx():
+    result = indices.CSx.compute(
+        tas=tas_c_xarray(),
+        freq="7D",
+        thresh=-10,
+    )
+    np.testing.assert_allclose(result, 2, rtol=1e-03)
+
+
+def test_CSn():
+    result = indices.CSn.compute(
+        tas=tas_c_xarray(),
+        freq="7D",
+        thresh=-10,
+        window=1,
+    )
+    np.testing.assert_allclose(result, 3, rtol=1e-03)
+
+
 def test_HSf():
     result = indices.HSf.compute(
         tasmax=tasmax_xarray(),
         freq="7D",
         thresh=27,
         window=1,
     )
@@ -493,27 +532,35 @@
 
 
 def test_HSx():
     result = indices.HSx.compute(
         tasmax=tasmax_xarray(),
         freq="7D",
         thresh=27,
+    )
+    np.testing.assert_allclose(result, 1, rtol=1e-03)
+
+
+def test_HSn():
+    result = indices.HSn.compute(
+        tasmax=tasmax_xarray(),
+        freq="7D",
+        thresh=27,
         window=1,
     )
     np.testing.assert_allclose(result, 1, rtol=1e-03)
 
 
 def test_HWx():
     result = indices.HWx.compute(
         tasmax=tasmax_xarray(),
         tasmin=tasmin_xarray(),
         freq="7D",
         thresh_tasmax=27,
         thresh_tasmin=25,
-        window=1,
     )
     np.testing.assert_allclose(result, 0, rtol=1e-03)
 
 
 def test_HWf():
     result = indices.HWf.compute(
         tasmax=tasmax_xarray(),
@@ -522,14 +569,26 @@
         thresh_tasmax=27,
         thresh_tasmin=25,
         window=1,
     )
     np.testing.assert_allclose(result, 0, rtol=1e-03)
 
 
+def test_HWn():
+    result = indices.HWn.compute(
+        tasmax=tasmax_xarray(),
+        tasmin=tasmin_xarray(),
+        freq="7D",
+        thresh_tasmax=27,
+        thresh_tasmin=25,
+        window=1,
+    )
+    np.testing.assert_allclose(result, 0, rtol=1e-03)
+
+
 def test_SD():
     result = indices.SD.compute(
         prsn=prsn_xarray(),
         freq="7D",
     )
     np.testing.assert_allclose(result, 4, rtol=1e-03)
 
@@ -660,7 +719,10 @@
 
 def FXx():
     result = indices.FGx.compute(
         sfcWindmax=sfcWind_xarray(),
         freq="7D",
     )
     np.testing.assert_allclose(result, [23], rtol=1e-03)
+
+
+test_LFD()
```

### Comparing `index_calculator-0.7.6/tests/test_xcalc.py` & `index_calculator-0.8.0/tests/test_xcalc.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pytest  # noqa
 from pyhomogenize import open_xrdataset
 
 import index_calculator as xcalc
 
-from .conftest import pr_day_netcdf, tas_1hr_netcdf, tas_day_netcdf
+from .conftest import pr_day_netcdf, tas_day_netcdf
 
 
 def test_processing():
     data = tas_day_netcdf()
     tas_ds = open_xrdataset(data)
     preproc = xcalc.preprocessing(
         tas_ds,
@@ -88,23 +88,7 @@
         freq="week",
         index="R95p",
         crop_time_axis=False,
         project="CORDEX",
         institution_id="TEST",
         base_period_time_range=["2001-01-01", "2001-01-07"],
     )
-
-
-def test_index_calculator_1hr():
-    data = tas_1hr_netcdf()
-    tas_ds = open_xrdataset(data)
-    xcalc.index_calculator(
-        ds=tas_ds,
-        freq="week",
-        index="TG",
-        crop_time_axis=False,
-        project="CORDEX",
-        institution="test institution",
-        institution_id="TEST",
-        contact="test@test.de",
-        write=True,
-    )
```

