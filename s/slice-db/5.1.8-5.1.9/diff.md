# Comparing `tmp/slice-db-5.1.8.tar.gz` & `tmp/slice-db-5.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slice-db-5.1.8.tar", last modified: Thu Dec 29 21:16:48 2022, max compression
+gzip compressed data, was "slice-db-5.1.9.tar", last modified: Wed Jul 12 20:59:26 2023, max compression
```

## Comparing `slice-db-5.1.8.tar` & `slice-db-5.1.9.tar`

### file list

```diff
@@ -1,92 +1,93 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-12-29 21:16:48.076065 slice-db-5.1.8/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6093 2022-12-29 21:16:48.076065 slice-db-5.1.8/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4059 2022-11-10 18:04:52.000000 slice-db-5.1.8/README.md
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2022-12-29 21:16:48.076065 slice-db-5.1.8/setup.cfg
--rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)     1470 2022-12-29 20:33:18.000000 slice-db-5.1.8/setup.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-12-29 21:16:48.068065 slice-db-5.1.8/slice_db/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       33 2022-08-26 15:16:26.000000 slice-db-5.1.8/slice_db/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-12-29 21:16:48.072065 slice-db-5.1.8/slice_db/cli/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2022-08-26 15:16:26.000000 slice-db-5.1.8/slice_db/cli/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      563 2022-08-26 15:16:26.000000 slice-db-5.1.8/slice_db/cli/common.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1829 2022-12-29 20:33:18.000000 slice-db-5.1.8/slice_db/cli/dump.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7951 2022-08-26 15:16:26.000000 slice-db-5.1.8/slice_db/cli/main.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      869 2022-08-26 15:16:26.000000 slice-db-5.1.8/slice_db/cli/restore.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      467 2022-08-26 15:16:26.000000 slice-db-5.1.8/slice_db/cli/schema.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1302 2022-08-26 15:16:26.000000 slice-db-5.1.8/slice_db/cli/schema_filter.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       35 2022-08-26 15:16:26.000000 slice-db-5.1.8/slice_db/cli/transform.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      568 2022-08-26 15:16:26.000000 slice-db-5.1.8/slice_db/cli/transform_field.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-12-29 21:16:48.072065 slice-db-5.1.8/slice_db/collection/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2022-08-26 15:16:26.000000 slice-db-5.1.8/slice_db/collection/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      294 2022-08-26 15:16:26.000000 slice-db-5.1.8/slice_db/collection/dict.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      731 2022-08-26 15:16:26.000000 slice-db-5.1.8/slice_db/collection/set.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      301 2022-08-26 15:16:26.000000 slice-db-5.1.8/slice_db/common.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-12-29 21:16:48.072065 slice-db-5.1.8/slice_db/concurrent/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      611 2022-08-26 15:16:26.000000 slice-db-5.1.8/slice_db/concurrent/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1461 2022-08-26 15:16:26.000000 slice-db-5.1.8/slice_db/concurrent/graph.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1053 2022-08-26 15:16:26.000000 slice-db-5.1.8/slice_db/concurrent/lock.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1270 2022-08-26 15:16:26.000000 slice-db-5.1.8/slice_db/concurrent/queue.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-12-29 21:16:48.072065 slice-db-5.1.8/slice_db/data/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2022-08-26 15:16:26.000000 slice-db-5.1.8/slice_db/data/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10023 2022-08-26 15:16:26.000000 slice-db-5.1.8/slice_db/data/city.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13073 2022-08-26 15:16:26.000000 slice-db-5.1.8/slice_db/data/given-name.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   827195 2022-08-26 15:16:26.000000 slice-db-5.1.8/slice_db/data/street.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    73498 2022-08-26 15:16:26.000000 slice-db-5.1.8/slice_db/data/surname.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      168 2022-08-26 15:16:26.000000 slice-db-5.1.8/slice_db/data/us-state-abbr.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      565 2022-08-26 15:16:26.000000 slice-db-5.1.8/slice_db/data/us-state.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    75153 2022-08-26 15:16:26.000000 slice-db-5.1.8/slice_db/data/word.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   198726 2022-08-26 15:16:26.000000 slice-db-5.1.8/slice_db/data/zip.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    17775 2022-12-08 23:26:12.000000 slice-db-5.1.8/slice_db/dump.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11580 2022-08-26 15:16:26.000000 slice-db-5.1.8/slice_db/dump_memory.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10732 2022-12-29 20:33:18.000000 slice-db-5.1.8/slice_db/dump_temp_table.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-12-29 21:16:48.076065 slice-db-5.1.8/slice_db/formats/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2022-08-26 15:16:26.000000 slice-db-5.1.8/slice_db/formats/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3239 2022-08-26 15:16:26.000000 slice-db-5.1.8/slice_db/formats/dump.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1724 2022-08-26 15:16:26.000000 slice-db-5.1.8/slice_db/formats/dump.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2901 2022-08-26 15:16:26.000000 slice-db-5.1.8/slice_db/formats/manifest.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1517 2022-08-26 15:16:26.000000 slice-db-5.1.8/slice_db/formats/manifest.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1745 2022-08-26 15:16:26.000000 slice-db-5.1.8/slice_db/formats/transform.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      925 2022-08-26 15:16:26.000000 slice-db-5.1.8/slice_db/formats/transform.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-12-29 21:16:48.076065 slice-db-5.1.8/slice_db/graph/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1031 2022-08-26 15:16:26.000000 slice-db-5.1.8/slice_db/graph/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-12-29 21:16:48.076065 slice-db-5.1.8/slice_db/json/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1849 2022-08-26 15:16:26.000000 slice-db-5.1.8/slice_db/json/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       10 2022-08-26 15:16:26.000000 slice-db-5.1.8/slice_db/log.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-12-29 21:16:48.076065 slice-db-5.1.8/slice_db/pg/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1286 2022-08-26 15:16:26.000000 slice-db-5.1.8/slice_db/pg/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1574 2022-08-26 15:16:26.000000 slice-db-5.1.8/slice_db/pg/copy.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2076 2022-08-26 15:16:26.000000 slice-db-5.1.8/slice_db/pg/token.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-12-29 21:16:48.076065 slice-db-5.1.8/slice_db/resource/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      194 2022-08-26 15:16:26.000000 slice-db-5.1.8/slice_db/resource/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8351 2022-08-26 15:16:26.000000 slice-db-5.1.8/slice_db/restore.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4898 2022-08-26 15:16:26.000000 slice-db-5.1.8/slice_db/schema.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2639 2022-08-26 15:16:26.000000 slice-db-5.1.8/slice_db/slice.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1410 2022-08-26 15:16:26.000000 slice-db-5.1.8/slice_db/sql.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3728 2022-08-26 15:16:26.000000 slice-db-5.1.8/slice_db/transform.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-12-29 21:16:48.076065 slice-db-5.1.8/slice_db/transforms/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      127 2022-08-26 15:16:26.000000 slice-db-5.1.8/slice_db/transforms/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4784 2022-08-26 15:16:26.000000 slice-db-5.1.8/slice_db/transforms/address.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1383 2022-08-26 15:16:26.000000 slice-db-5.1.8/slice_db/transforms/common.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      854 2022-08-26 15:16:26.000000 slice-db-5.1.8/slice_db/transforms/date.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1354 2022-12-29 21:12:30.000000 slice-db-5.1.8/slice_db/transforms/json.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1292 2022-08-26 15:16:26.000000 slice-db-5.1.8/slice_db/transforms/person.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5933 2022-08-26 15:16:26.000000 slice-db-5.1.8/slice_db/transforms/text.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       22 2022-12-29 21:15:58.000000 slice-db-5.1.8/slice_db/version.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-12-29 21:16:48.068065 slice-db-5.1.8/slice_db.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6093 2022-12-29 21:16:47.000000 slice-db-5.1.8/slice_db.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1916 2022-12-29 21:16:47.000000 slice-db-5.1.8/slice_db.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2022-12-29 21:16:47.000000 slice-db-5.1.8/slice_db.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       52 2022-12-29 21:16:47.000000 slice-db-5.1.8/slice_db.egg-info/entry_points.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      138 2022-12-29 21:16:47.000000 slice-db-5.1.8/slice_db.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        9 2022-12-29 21:16:47.000000 slice-db-5.1.8/slice_db.egg-info/top_level.txt
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-12-29 21:16:48.076065 slice-db-5.1.8/test/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      484 2022-08-26 15:16:26.000000 slice-db-5.1.8/test/test_copy.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3617 2022-08-26 15:16:26.000000 slice-db-5.1.8/test/test_defer.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4192 2022-08-26 21:21:27.000000 slice-db-5.1.8/test/test_dump.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1871 2022-08-26 15:16:26.000000 slice-db-5.1.8/test/test_dump_sequence.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3054 2022-08-26 15:16:26.000000 slice-db-5.1.8/test/test_dump_sql.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3093 2022-08-26 15:16:26.000000 slice-db-5.1.8/test/test_dump_transform.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      689 2022-08-26 15:16:26.000000 slice-db-5.1.8/test/test_schema.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      691 2022-08-26 15:16:26.000000 slice-db-5.1.8/test/test_schema_empty.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      767 2022-08-26 15:16:26.000000 slice-db-5.1.8/test/test_set.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      256 2022-08-26 15:16:26.000000 slice-db-5.1.8/test/test_token.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5659 2022-12-29 21:13:13.000000 slice-db-5.1.8/test/test_transform_field.py
+drwxrwxr-x   0 captkirk  (1000) captkirk  (1000)        0 2023-07-12 20:59:26.878477 slice-db-5.1.9/
+-rw-rw-r--   0 captkirk  (1000) captkirk  (1000)     1062 2023-07-12 20:19:39.000000 slice-db-5.1.9/LICENSE.txt
+-rw-rw-r--   0 captkirk  (1000) captkirk  (1000)     4692 2023-07-12 20:59:26.874477 slice-db-5.1.9/PKG-INFO
+-rw-rw-r--   0 captkirk  (1000) captkirk  (1000)     4059 2023-07-12 20:19:39.000000 slice-db-5.1.9/README.md
+-rw-rw-r--   0 captkirk  (1000) captkirk  (1000)       38 2023-07-12 20:59:26.878477 slice-db-5.1.9/setup.cfg
+-rwxrwxr-x   0 captkirk  (1000) captkirk  (1000)     1470 2023-07-12 20:19:39.000000 slice-db-5.1.9/setup.py
+drwxrwxr-x   0 captkirk  (1000) captkirk  (1000)        0 2023-07-12 20:59:26.866477 slice-db-5.1.9/slice_db/
+-rw-rw-r--   0 captkirk  (1000) captkirk  (1000)       33 2023-07-12 20:19:39.000000 slice-db-5.1.9/slice_db/__init__.py
+drwxrwxr-x   0 captkirk  (1000) captkirk  (1000)        0 2023-07-12 20:59:26.866477 slice-db-5.1.9/slice_db/cli/
+-rw-rw-r--   0 captkirk  (1000) captkirk  (1000)        0 2023-07-12 20:19:39.000000 slice-db-5.1.9/slice_db/cli/__init__.py
+-rw-rw-r--   0 captkirk  (1000) captkirk  (1000)      563 2023-07-12 20:19:39.000000 slice-db-5.1.9/slice_db/cli/common.py
+-rw-rw-r--   0 captkirk  (1000) captkirk  (1000)     1938 2023-07-12 20:42:47.000000 slice-db-5.1.9/slice_db/cli/dump.py
+-rw-rw-r--   0 captkirk  (1000) captkirk  (1000)     7951 2023-07-12 20:19:39.000000 slice-db-5.1.9/slice_db/cli/main.py
+-rw-rw-r--   0 captkirk  (1000) captkirk  (1000)      869 2023-07-12 20:19:39.000000 slice-db-5.1.9/slice_db/cli/restore.py
+-rw-rw-r--   0 captkirk  (1000) captkirk  (1000)      467 2023-07-12 20:19:39.000000 slice-db-5.1.9/slice_db/cli/schema.py
+-rw-rw-r--   0 captkirk  (1000) captkirk  (1000)     1302 2023-07-12 20:19:39.000000 slice-db-5.1.9/slice_db/cli/schema_filter.py
+-rw-rw-r--   0 captkirk  (1000) captkirk  (1000)       35 2023-07-12 20:19:39.000000 slice-db-5.1.9/slice_db/cli/transform.py
+-rw-rw-r--   0 captkirk  (1000) captkirk  (1000)      568 2023-07-12 20:19:39.000000 slice-db-5.1.9/slice_db/cli/transform_field.py
+drwxrwxr-x   0 captkirk  (1000) captkirk  (1000)        0 2023-07-12 20:59:26.866477 slice-db-5.1.9/slice_db/collection/
+-rw-rw-r--   0 captkirk  (1000) captkirk  (1000)        0 2023-07-12 20:19:39.000000 slice-db-5.1.9/slice_db/collection/__init__.py
+-rw-rw-r--   0 captkirk  (1000) captkirk  (1000)      294 2023-07-12 20:19:39.000000 slice-db-5.1.9/slice_db/collection/dict.py
+-rw-rw-r--   0 captkirk  (1000) captkirk  (1000)      731 2023-07-12 20:19:39.000000 slice-db-5.1.9/slice_db/collection/set.py
+-rw-rw-r--   0 captkirk  (1000) captkirk  (1000)      301 2023-07-12 20:19:39.000000 slice-db-5.1.9/slice_db/common.py
+drwxrwxr-x   0 captkirk  (1000) captkirk  (1000)        0 2023-07-12 20:59:26.866477 slice-db-5.1.9/slice_db/concurrent/
+-rw-rw-r--   0 captkirk  (1000) captkirk  (1000)      611 2023-07-12 20:19:39.000000 slice-db-5.1.9/slice_db/concurrent/__init__.py
+-rw-rw-r--   0 captkirk  (1000) captkirk  (1000)     1461 2023-07-12 20:19:39.000000 slice-db-5.1.9/slice_db/concurrent/graph.py
+-rw-rw-r--   0 captkirk  (1000) captkirk  (1000)     1053 2023-07-12 20:19:39.000000 slice-db-5.1.9/slice_db/concurrent/lock.py
+-rw-rw-r--   0 captkirk  (1000) captkirk  (1000)     1270 2023-07-12 20:19:39.000000 slice-db-5.1.9/slice_db/concurrent/queue.py
+drwxrwxr-x   0 captkirk  (1000) captkirk  (1000)        0 2023-07-12 20:59:26.870477 slice-db-5.1.9/slice_db/data/
+-rw-rw-r--   0 captkirk  (1000) captkirk  (1000)        0 2023-07-12 20:19:39.000000 slice-db-5.1.9/slice_db/data/__init__.py
+-rw-rw-r--   0 captkirk  (1000) captkirk  (1000)    10023 2023-07-12 20:19:39.000000 slice-db-5.1.9/slice_db/data/city.txt
+-rw-rw-r--   0 captkirk  (1000) captkirk  (1000)    13073 2023-07-12 20:19:39.000000 slice-db-5.1.9/slice_db/data/given-name.txt
+-rw-rw-r--   0 captkirk  (1000) captkirk  (1000)   827195 2023-07-12 20:19:39.000000 slice-db-5.1.9/slice_db/data/street.txt
+-rw-rw-r--   0 captkirk  (1000) captkirk  (1000)    73498 2023-07-12 20:19:39.000000 slice-db-5.1.9/slice_db/data/surname.txt
+-rw-rw-r--   0 captkirk  (1000) captkirk  (1000)      168 2023-07-12 20:19:39.000000 slice-db-5.1.9/slice_db/data/us-state-abbr.txt
+-rw-rw-r--   0 captkirk  (1000) captkirk  (1000)      565 2023-07-12 20:19:39.000000 slice-db-5.1.9/slice_db/data/us-state.txt
+-rw-rw-r--   0 captkirk  (1000) captkirk  (1000)    75153 2023-07-12 20:19:39.000000 slice-db-5.1.9/slice_db/data/word.txt
+-rw-rw-r--   0 captkirk  (1000) captkirk  (1000)   198726 2023-07-12 20:19:39.000000 slice-db-5.1.9/slice_db/data/zip.txt
+-rw-rw-r--   0 captkirk  (1000) captkirk  (1000)    17775 2023-07-12 20:19:39.000000 slice-db-5.1.9/slice_db/dump.py
+-rw-rw-r--   0 captkirk  (1000) captkirk  (1000)    11580 2023-07-12 20:19:39.000000 slice-db-5.1.9/slice_db/dump_memory.py
+-rw-rw-r--   0 captkirk  (1000) captkirk  (1000)    10848 2023-07-12 20:47:22.000000 slice-db-5.1.9/slice_db/dump_temp_table.py
+drwxrwxr-x   0 captkirk  (1000) captkirk  (1000)        0 2023-07-12 20:59:26.870477 slice-db-5.1.9/slice_db/formats/
+-rw-rw-r--   0 captkirk  (1000) captkirk  (1000)        0 2023-07-12 20:19:39.000000 slice-db-5.1.9/slice_db/formats/__init__.py
+-rw-rw-r--   0 captkirk  (1000) captkirk  (1000)     3239 2023-07-12 20:19:39.000000 slice-db-5.1.9/slice_db/formats/dump.json
+-rw-rw-r--   0 captkirk  (1000) captkirk  (1000)     1724 2023-07-12 20:19:39.000000 slice-db-5.1.9/slice_db/formats/dump.py
+-rw-rw-r--   0 captkirk  (1000) captkirk  (1000)     2901 2023-07-12 20:19:39.000000 slice-db-5.1.9/slice_db/formats/manifest.json
+-rw-rw-r--   0 captkirk  (1000) captkirk  (1000)     1517 2023-07-12 20:19:39.000000 slice-db-5.1.9/slice_db/formats/manifest.py
+-rw-rw-r--   0 captkirk  (1000) captkirk  (1000)     1745 2023-07-12 20:19:39.000000 slice-db-5.1.9/slice_db/formats/transform.json
+-rw-rw-r--   0 captkirk  (1000) captkirk  (1000)      925 2023-07-12 20:19:39.000000 slice-db-5.1.9/slice_db/formats/transform.py
+drwxrwxr-x   0 captkirk  (1000) captkirk  (1000)        0 2023-07-12 20:59:26.870477 slice-db-5.1.9/slice_db/graph/
+-rw-rw-r--   0 captkirk  (1000) captkirk  (1000)     1031 2023-07-12 20:19:39.000000 slice-db-5.1.9/slice_db/graph/__init__.py
+drwxrwxr-x   0 captkirk  (1000) captkirk  (1000)        0 2023-07-12 20:59:26.874477 slice-db-5.1.9/slice_db/json/
+-rw-rw-r--   0 captkirk  (1000) captkirk  (1000)     1849 2023-07-12 20:19:39.000000 slice-db-5.1.9/slice_db/json/__init__.py
+-rw-rw-r--   0 captkirk  (1000) captkirk  (1000)       10 2023-07-12 20:19:39.000000 slice-db-5.1.9/slice_db/log.py
+drwxrwxr-x   0 captkirk  (1000) captkirk  (1000)        0 2023-07-12 20:59:26.874477 slice-db-5.1.9/slice_db/pg/
+-rw-rw-r--   0 captkirk  (1000) captkirk  (1000)     1286 2023-07-12 20:19:39.000000 slice-db-5.1.9/slice_db/pg/__init__.py
+-rw-rw-r--   0 captkirk  (1000) captkirk  (1000)     1574 2023-07-12 20:19:39.000000 slice-db-5.1.9/slice_db/pg/copy.py
+-rw-rw-r--   0 captkirk  (1000) captkirk  (1000)     2076 2023-07-12 20:19:39.000000 slice-db-5.1.9/slice_db/pg/token.py
+drwxrwxr-x   0 captkirk  (1000) captkirk  (1000)        0 2023-07-12 20:59:26.874477 slice-db-5.1.9/slice_db/resource/
+-rw-rw-r--   0 captkirk  (1000) captkirk  (1000)      194 2023-07-12 20:19:39.000000 slice-db-5.1.9/slice_db/resource/__init__.py
+-rw-rw-r--   0 captkirk  (1000) captkirk  (1000)     8351 2023-07-12 20:19:39.000000 slice-db-5.1.9/slice_db/restore.py
+-rw-rw-r--   0 captkirk  (1000) captkirk  (1000)     4898 2023-07-12 20:19:39.000000 slice-db-5.1.9/slice_db/schema.py
+-rw-rw-r--   0 captkirk  (1000) captkirk  (1000)     2639 2023-07-12 20:19:39.000000 slice-db-5.1.9/slice_db/slice.py
+-rw-rw-r--   0 captkirk  (1000) captkirk  (1000)     1410 2023-07-12 20:19:39.000000 slice-db-5.1.9/slice_db/sql.py
+-rw-rw-r--   0 captkirk  (1000) captkirk  (1000)     3728 2023-07-12 20:19:39.000000 slice-db-5.1.9/slice_db/transform.py
+drwxrwxr-x   0 captkirk  (1000) captkirk  (1000)        0 2023-07-12 20:59:26.874477 slice-db-5.1.9/slice_db/transforms/
+-rw-rw-r--   0 captkirk  (1000) captkirk  (1000)      127 2023-07-12 20:19:39.000000 slice-db-5.1.9/slice_db/transforms/__init__.py
+-rw-rw-r--   0 captkirk  (1000) captkirk  (1000)     4784 2023-07-12 20:19:39.000000 slice-db-5.1.9/slice_db/transforms/address.py
+-rw-rw-r--   0 captkirk  (1000) captkirk  (1000)     1383 2023-07-12 20:19:39.000000 slice-db-5.1.9/slice_db/transforms/common.py
+-rw-rw-r--   0 captkirk  (1000) captkirk  (1000)      854 2023-07-12 20:19:39.000000 slice-db-5.1.9/slice_db/transforms/date.py
+-rw-rw-r--   0 captkirk  (1000) captkirk  (1000)     1354 2023-07-12 20:19:39.000000 slice-db-5.1.9/slice_db/transforms/json.py
+-rw-rw-r--   0 captkirk  (1000) captkirk  (1000)     1292 2023-07-12 20:19:39.000000 slice-db-5.1.9/slice_db/transforms/person.py
+-rw-rw-r--   0 captkirk  (1000) captkirk  (1000)     5933 2023-07-12 20:19:39.000000 slice-db-5.1.9/slice_db/transforms/text.py
+-rw-rw-r--   0 captkirk  (1000) captkirk  (1000)       22 2023-07-12 20:38:34.000000 slice-db-5.1.9/slice_db/version.py
+drwxrwxr-x   0 captkirk  (1000) captkirk  (1000)        0 2023-07-12 20:59:26.866477 slice-db-5.1.9/slice_db.egg-info/
+-rw-rw-r--   0 captkirk  (1000) captkirk  (1000)     4692 2023-07-12 20:59:26.000000 slice-db-5.1.9/slice_db.egg-info/PKG-INFO
+-rw-rw-r--   0 captkirk  (1000) captkirk  (1000)     1928 2023-07-12 20:59:26.000000 slice-db-5.1.9/slice_db.egg-info/SOURCES.txt
+-rw-rw-r--   0 captkirk  (1000) captkirk  (1000)        1 2023-07-12 20:59:26.000000 slice-db-5.1.9/slice_db.egg-info/dependency_links.txt
+-rw-rw-r--   0 captkirk  (1000) captkirk  (1000)       52 2023-07-12 20:59:26.000000 slice-db-5.1.9/slice_db.egg-info/entry_points.txt
+-rw-rw-r--   0 captkirk  (1000) captkirk  (1000)      138 2023-07-12 20:59:26.000000 slice-db-5.1.9/slice_db.egg-info/requires.txt
+-rw-rw-r--   0 captkirk  (1000) captkirk  (1000)        9 2023-07-12 20:59:26.000000 slice-db-5.1.9/slice_db.egg-info/top_level.txt
+drwxrwxr-x   0 captkirk  (1000) captkirk  (1000)        0 2023-07-12 20:59:26.874477 slice-db-5.1.9/test/
+-rw-rw-r--   0 captkirk  (1000) captkirk  (1000)      484 2023-07-12 20:19:39.000000 slice-db-5.1.9/test/test_copy.py
+-rw-rw-r--   0 captkirk  (1000) captkirk  (1000)     3617 2023-07-12 20:19:39.000000 slice-db-5.1.9/test/test_defer.py
+-rw-rw-r--   0 captkirk  (1000) captkirk  (1000)     4192 2023-07-12 20:19:39.000000 slice-db-5.1.9/test/test_dump.py
+-rw-rw-r--   0 captkirk  (1000) captkirk  (1000)     1870 2023-07-12 20:42:47.000000 slice-db-5.1.9/test/test_dump_sequence.py
+-rw-rw-r--   0 captkirk  (1000) captkirk  (1000)     3054 2023-07-12 20:19:39.000000 slice-db-5.1.9/test/test_dump_sql.py
+-rw-rw-r--   0 captkirk  (1000) captkirk  (1000)     3093 2023-07-12 20:19:39.000000 slice-db-5.1.9/test/test_dump_transform.py
+-rw-rw-r--   0 captkirk  (1000) captkirk  (1000)      689 2023-07-12 20:19:39.000000 slice-db-5.1.9/test/test_schema.py
+-rw-rw-r--   0 captkirk  (1000) captkirk  (1000)      691 2023-07-12 20:19:39.000000 slice-db-5.1.9/test/test_schema_empty.py
+-rw-rw-r--   0 captkirk  (1000) captkirk  (1000)      767 2023-07-12 20:19:39.000000 slice-db-5.1.9/test/test_set.py
+-rw-rw-r--   0 captkirk  (1000) captkirk  (1000)      256 2023-07-12 20:19:39.000000 slice-db-5.1.9/test/test_token.py
+-rw-rw-r--   0 captkirk  (1000) captkirk  (1000)     5659 2023-07-12 20:19:39.000000 slice-db-5.1.9/test/test_transform_field.py
```

### Comparing `slice-db-5.1.8/README.md` & `slice-db-5.1.9/README.md`

 * *Files identical despite different names*

### Comparing `slice-db-5.1.8/setup.py` & `slice-db-5.1.9/setup.py`

 * *Files identical despite different names*

### Comparing `slice-db-5.1.8/slice_db/cli/common.py` & `slice-db-5.1.9/slice_db/cli/common.py`

 * *Files identical despite different names*

### Comparing `slice-db-5.1.8/slice_db/cli/dump.py` & `slice-db-5.1.9/slice_db/cli/dump.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import asyncio
 import logging
 import secrets
+import traceback
 
 import asyncpg
 
 from ..common import setup_connection
 from ..dump import DumpIo, DumpParams, OutputType, dump
 from ..dump_temp_table import TempTableStrategy
 from ..formats.dump import DumpRoot
@@ -51,14 +52,17 @@
             parallelism=args.jobs,
             output_type=output_type,
             pepper=pepper,
             strategy=strategy,
         )
 
         await dump(roots, io, params)
+    except:
+        print("Exception caught in cli/dump.py:")
+        traceback.print_exc()
     finally:
         await pool.close()
 
 
 async def _init_connection(conn):
     await set_tid_codec(conn)
     await setup_connection(conn)
```

### Comparing `slice-db-5.1.8/slice_db/cli/main.py` & `slice-db-5.1.9/slice_db/cli/main.py`

 * *Files identical despite different names*

### Comparing `slice-db-5.1.8/slice_db/cli/restore.py` & `slice-db-5.1.9/slice_db/cli/restore.py`

 * *Files identical despite different names*

### Comparing `slice-db-5.1.8/slice_db/cli/schema_filter.py` & `slice-db-5.1.9/slice_db/cli/schema_filter.py`

 * *Files identical despite different names*

### Comparing `slice-db-5.1.8/slice_db/cli/transform_field.py` & `slice-db-5.1.9/slice_db/cli/transform_field.py`

 * *Files identical despite different names*

### Comparing `slice-db-5.1.8/slice_db/collection/set.py` & `slice-db-5.1.9/slice_db/collection/set.py`

 * *Files identical despite different names*

### Comparing `slice-db-5.1.8/slice_db/concurrent/__init__.py` & `slice-db-5.1.9/slice_db/concurrent/__init__.py`

 * *Files identical despite different names*

### Comparing `slice-db-5.1.8/slice_db/concurrent/graph.py` & `slice-db-5.1.9/slice_db/concurrent/graph.py`

 * *Files identical despite different names*

### Comparing `slice-db-5.1.8/slice_db/concurrent/lock.py` & `slice-db-5.1.9/slice_db/concurrent/lock.py`

 * *Files identical despite different names*

### Comparing `slice-db-5.1.8/slice_db/concurrent/queue.py` & `slice-db-5.1.9/slice_db/concurrent/queue.py`

 * *Files identical despite different names*

### Comparing `slice-db-5.1.8/slice_db/data/city.txt` & `slice-db-5.1.9/slice_db/data/city.txt`

 * *Files identical despite different names*

### Comparing `slice-db-5.1.8/slice_db/data/given-name.txt` & `slice-db-5.1.9/slice_db/data/given-name.txt`

 * *Files identical despite different names*

### Comparing `slice-db-5.1.8/slice_db/data/street.txt` & `slice-db-5.1.9/slice_db/data/street.txt`

 * *Files identical despite different names*

### Comparing `slice-db-5.1.8/slice_db/data/surname.txt` & `slice-db-5.1.9/slice_db/data/surname.txt`

 * *Files identical despite different names*

### Comparing `slice-db-5.1.8/slice_db/data/us-state.txt` & `slice-db-5.1.9/slice_db/data/us-state.txt`

 * *Files identical despite different names*

### Comparing `slice-db-5.1.8/slice_db/data/word.txt` & `slice-db-5.1.9/slice_db/data/word.txt`

 * *Files identical despite different names*

### Comparing `slice-db-5.1.8/slice_db/data/zip.txt` & `slice-db-5.1.9/slice_db/data/zip.txt`

 * *Files identical despite different names*

### Comparing `slice-db-5.1.8/slice_db/dump.py` & `slice-db-5.1.9/slice_db/dump.py`

 * *Files identical despite different names*

### Comparing `slice-db-5.1.8/slice_db/dump_memory.py` & `slice-db-5.1.9/slice_db/dump_memory.py`

 * *Files identical despite different names*

### Comparing `slice-db-5.1.8/slice_db/dump_temp_table.py` & `slice-db-5.1.9/slice_db/dump_temp_table.py`

 * *Files 2% similar despite different names*

```diff
@@ -118,15 +118,15 @@
                 for reference in sorted(
                     self.segment.table.reverse_references,
                     key=lambda r: r.table.row_count,
                 ):
                     await self._process_reference(
                         conn, reference, DumpReferenceDirection.REVERSE
                     )
-
+                await conn.execute("SET statement_timeout TO 0")
                 await _dump_data(conn, self.segment.table, self.segment.row_ids, tmp)
 
             tmp.seek(0)
             try:
                 transformer = self.dump.transformers[self.segment.table.id]
             except KeyError:
                 # copy file without tranformation
@@ -191,14 +191,15 @@
 ) -> typing.List[Tid]:
     """
     Discover, using root
     """
     logging.log(TRACE, f"Finding rows from table %s", table.id)
     start = time.perf_counter()
 
+    await conn.execute("SET statement_timeout TO 0")
     query = f"""
         SELECT ctid
         FROM {table.sql}
         WHERE {condition}
         ORDER BY 1
     """
     found_ids = [id_ for id_, in await conn.fetch(query)]
@@ -252,15 +253,14 @@
 async def _discover_reference(
     conn: asyncpg.Connection,
     segment: TableSegment,
     reference: Reference,
     direction: DumpReferenceDirection,
     result,
 ) -> typing.List[Tid]:
-
     """
     Discover, using reference
     """
     if direction == DumpReferenceDirection.FORWARD:
         from_columns = reference.columns
         from_table = reference.table
         to_columns = reference.reference_columns
```

### Comparing `slice-db-5.1.8/slice_db/formats/dump.json` & `slice-db-5.1.9/slice_db/formats/dump.json`

 * *Files identical despite different names*

### Comparing `slice-db-5.1.8/slice_db/formats/dump.py` & `slice-db-5.1.9/slice_db/formats/dump.py`

 * *Files identical despite different names*

### Comparing `slice-db-5.1.8/slice_db/formats/manifest.json` & `slice-db-5.1.9/slice_db/formats/manifest.json`

 * *Files identical despite different names*

### Comparing `slice-db-5.1.8/slice_db/formats/manifest.py` & `slice-db-5.1.9/slice_db/formats/manifest.py`

 * *Files identical despite different names*

### Comparing `slice-db-5.1.8/slice_db/formats/transform.json` & `slice-db-5.1.9/slice_db/formats/transform.json`

 * *Files identical despite different names*

### Comparing `slice-db-5.1.8/slice_db/formats/transform.py` & `slice-db-5.1.9/slice_db/formats/transform.py`

 * *Files identical despite different names*

### Comparing `slice-db-5.1.8/slice_db/graph/__init__.py` & `slice-db-5.1.9/slice_db/graph/__init__.py`

 * *Files identical despite different names*

### Comparing `slice-db-5.1.8/slice_db/json/__init__.py` & `slice-db-5.1.9/slice_db/json/__init__.py`

 * *Files identical despite different names*

### Comparing `slice-db-5.1.8/slice_db/pg/__init__.py` & `slice-db-5.1.9/slice_db/pg/__init__.py`

 * *Files identical despite different names*

### Comparing `slice-db-5.1.8/slice_db/pg/copy.py` & `slice-db-5.1.9/slice_db/pg/copy.py`

 * *Files identical despite different names*

### Comparing `slice-db-5.1.8/slice_db/pg/token.py` & `slice-db-5.1.9/slice_db/pg/token.py`

 * *Files identical despite different names*

### Comparing `slice-db-5.1.8/slice_db/restore.py` & `slice-db-5.1.9/slice_db/restore.py`

 * *Files identical despite different names*

### Comparing `slice-db-5.1.8/slice_db/schema.py` & `slice-db-5.1.9/slice_db/schema.py`

 * *Files identical despite different names*

### Comparing `slice-db-5.1.8/slice_db/slice.py` & `slice-db-5.1.9/slice_db/slice.py`

 * *Files identical despite different names*

### Comparing `slice-db-5.1.8/slice_db/sql.py` & `slice-db-5.1.9/slice_db/sql.py`

 * *Files identical despite different names*

### Comparing `slice-db-5.1.8/slice_db/transform.py` & `slice-db-5.1.9/slice_db/transform.py`

 * *Files identical despite different names*

### Comparing `slice-db-5.1.8/slice_db/transforms/address.py` & `slice-db-5.1.9/slice_db/transforms/address.py`

 * *Files identical despite different names*

### Comparing `slice-db-5.1.8/slice_db/transforms/common.py` & `slice-db-5.1.9/slice_db/transforms/common.py`

 * *Files identical despite different names*

### Comparing `slice-db-5.1.8/slice_db/transforms/date.py` & `slice-db-5.1.9/slice_db/transforms/date.py`

 * *Files identical despite different names*

### Comparing `slice-db-5.1.8/slice_db/transforms/json.py` & `slice-db-5.1.9/slice_db/transforms/json.py`

 * *Files identical despite different names*

### Comparing `slice-db-5.1.8/slice_db/transforms/person.py` & `slice-db-5.1.9/slice_db/transforms/person.py`

 * *Files identical despite different names*

### Comparing `slice-db-5.1.8/slice_db/transforms/text.py` & `slice-db-5.1.9/slice_db/transforms/text.py`

 * *Files identical despite different names*

### Comparing `slice-db-5.1.8/slice_db.egg-info/SOURCES.txt` & `slice-db-5.1.9/slice_db.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE.txt
 README.md
 setup.py
 slice_db/__init__.py
 slice_db/common.py
 slice_db/dump.py
 slice_db/dump_memory.py
 slice_db/dump_temp_table.py
```

### Comparing `slice-db-5.1.8/test/test_defer.py` & `slice-db-5.1.9/test/test_defer.py`

 * *Files identical despite different names*

### Comparing `slice-db-5.1.8/test/test_dump.py` & `slice-db-5.1.9/test/test_dump.py`

 * *Files identical despite different names*

### Comparing `slice-db-5.1.8/test/test_dump_sequence.py` & `slice-db-5.1.9/test/test_dump_sequence.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,15 +11,14 @@
         id serial PRIMARY KEY,
         color text NOT NULL
     );
 """
 
 
 def test_dump_sequence(pg_database, snapshot):
-
     with temp_file("schema-") as schema_file, temp_file("output-") as output_file:
         with connection("") as conn, transaction(conn) as cur:
             cur.execute(_SCHEMA_SQL)
 
             cur.execute(
                 """
                     INSERT INTO datum (color) VALUES ('blue'), ('yellow'), ('red')
```

### Comparing `slice-db-5.1.8/test/test_dump_sql.py` & `slice-db-5.1.9/test/test_dump_sql.py`

 * *Files identical despite different names*

### Comparing `slice-db-5.1.8/test/test_dump_transform.py` & `slice-db-5.1.9/test/test_dump_transform.py`

 * *Files identical despite different names*

### Comparing `slice-db-5.1.8/test/test_schema.py` & `slice-db-5.1.9/test/test_schema.py`

 * *Files identical despite different names*

### Comparing `slice-db-5.1.8/test/test_schema_empty.py` & `slice-db-5.1.9/test/test_schema_empty.py`

 * *Files identical despite different names*

### Comparing `slice-db-5.1.8/test/test_set.py` & `slice-db-5.1.9/test/test_set.py`

 * *Files identical despite different names*

### Comparing `slice-db-5.1.8/test/test_transform_field.py` & `slice-db-5.1.9/test/test_transform_field.py`

 * *Files identical despite different names*

