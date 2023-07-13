# Comparing `tmp/dreem-0.1.8.tar.gz` & `tmp/dreem-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dreem-0.1.8.tar", last modified: Wed Apr 26 03:43:48 2023, max compression
+gzip compressed data, was "dreem-0.1.9.tar", last modified: Wed May 10 03:22:49 2023, max compression
```

## Comparing `dreem-0.1.8.tar` & `dreem-0.1.9.tar`

### file list

```diff
@@ -1,81 +1,82 @@
-drwxr-xr-x   0 ymdt       (501) staff       (20)        0 2023-04-26 03:43:48.445230 dreem-0.1.8/
--rw-r--r--   0 ymdt       (501) staff       (20)     1227 2023-03-27 06:57:46.000000 dreem-0.1.8/LICENSE
--rw-r--r--   0 ymdt       (501) staff       (20)      131 2023-04-19 20:17:44.000000 dreem-0.1.8/MANIFEST.in
--rw-r--r--   0 ymdt       (501) staff       (20)     1195 2023-04-26 03:43:48.445064 dreem-0.1.8/PKG-INFO
--rw-r--r--   0 ymdt       (501) staff       (20)      916 2023-04-22 00:57:35.000000 dreem-0.1.8/README.md
-drwxr-xr-x   0 ymdt       (501) staff       (20)        0 2023-04-26 03:43:48.433334 dreem-0.1.8/dreem/
--rw-r--r--   0 ymdt       (501) staff       (20)      177 2023-04-19 20:17:44.000000 dreem-0.1.8/dreem/__init__.py
-drwxr-xr-x   0 ymdt       (501) staff       (20)        0 2023-04-26 03:43:48.435462 dreem-0.1.8/dreem/aggregate/
--rw-r--r--   0 ymdt       (501) staff       (20)       35 2023-03-27 06:57:46.000000 dreem-0.1.8/dreem/aggregate/__init__.py
--rw-r--r--   0 ymdt       (501) staff       (20)     2651 2023-03-02 22:29:36.000000 dreem-0.1.8/dreem/aggregate/library.py
--rw-r--r--   0 ymdt       (501) staff       (20)     1976 2023-03-27 06:57:46.000000 dreem-0.1.8/dreem/aggregate/library_samples.py
--rw-r--r--   0 ymdt       (501) staff       (20)     6714 2023-04-19 20:17:44.000000 dreem-0.1.8/dreem/aggregate/main.py
--rw-r--r--   0 ymdt       (501) staff       (20)     3388 2023-04-19 20:17:44.000000 dreem-0.1.8/dreem/aggregate/mutation_count.py
-drwxr-xr-x   0 ymdt       (501) staff       (20)        0 2023-04-26 03:43:48.436492 dreem-0.1.8/dreem/align/
--rw-r--r--   0 ymdt       (501) staff       (20)       35 2023-03-06 17:48:28.000000 dreem-0.1.8/dreem/align/__init__.py
--rw-r--r--   0 ymdt       (501) staff       (20)    21882 2023-04-11 18:17:48.000000 dreem-0.1.8/dreem/align/fq2bam.py
--rwxr-xr-x   0 ymdt       (501) staff       (20)    25001 2023-04-11 18:17:48.000000 dreem-0.1.8/dreem/align/fqs.py
--rw-r--r--   0 ymdt       (501) staff       (20)     7100 2023-04-19 20:17:44.000000 dreem-0.1.8/dreem/align/main.py
--rwxr-xr-x   0 ymdt       (501) staff       (20)     9982 2023-04-19 20:17:44.000000 dreem-0.1.8/dreem/align/xams.py
-drwxr-xr-x   0 ymdt       (501) staff       (20)        0 2023-04-26 03:43:48.437423 dreem-0.1.8/dreem/cluster/
--rw-r--r--   0 ymdt       (501) staff       (20)    13117 2023-04-04 22:14:41.000000 dreem-0.1.8/dreem/cluster/EMclustering.py
--rw-r--r--   0 ymdt       (501) staff       (20)       35 2023-04-04 22:14:41.000000 dreem-0.1.8/dreem/cluster/__init__.py
--rw-r--r--   0 ymdt       (501) staff       (20)     8800 2023-04-19 20:17:44.000000 dreem-0.1.8/dreem/cluster/bitvector.py
--rw-r--r--   0 ymdt       (501) staff       (20)     6503 2023-04-19 20:17:44.000000 dreem-0.1.8/dreem/cluster/clusteringAnalysis.py
--rw-r--r--   0 ymdt       (501) staff       (20)     3628 2023-04-19 20:17:44.000000 dreem-0.1.8/dreem/cluster/main.py
-drwxr-xr-x   0 ymdt       (501) staff       (20)        0 2023-04-26 03:43:48.438014 dreem-0.1.8/dreem/demultiplex/
--rw-r--r--   0 ymdt       (501) staff       (20)       35 2023-03-27 06:57:46.000000 dreem-0.1.8/dreem/demultiplex/__init__.py
--rw-r--r--   0 ymdt       (501) staff       (20)    38971 2023-04-19 20:17:44.000000 dreem-0.1.8/dreem/demultiplex/demultiplex.py
--rw-r--r--   0 ymdt       (501) staff       (20)     1819 2023-04-21 17:32:54.000000 dreem-0.1.8/dreem/demultiplex/main.py
-drwxr-xr-x   0 ymdt       (501) staff       (20)        0 2023-04-26 03:43:48.439322 dreem-0.1.8/dreem/draw/
--rw-r--r--   0 ymdt       (501) staff       (20)      315 2023-04-04 22:14:41.000000 dreem-0.1.8/dreem/draw/__init__.py
--rw-r--r--   0 ymdt       (501) staff       (20)      225 2023-03-02 22:29:36.000000 dreem-0.1.8/dreem/draw/load_dataset.py
--rw-r--r--   0 ymdt       (501) staff       (20)     5995 2023-04-19 20:17:44.000000 dreem-0.1.8/dreem/draw/main.py
--rw-r--r--   0 ymdt       (501) staff       (20)     6655 2023-04-04 22:14:41.000000 dreem-0.1.8/dreem/draw/manipulator.py
--rw-r--r--   0 ymdt       (501) staff       (20)    22424 2023-04-21 23:08:14.000000 dreem-0.1.8/dreem/draw/plotter.py
-drwxr-xr-x   0 ymdt       (501) staff       (20)        0 2023-04-26 03:43:48.439512 dreem-0.1.8/dreem/draw/resources/
--rw-r--r--   0 ymdt       (501) staff       (20)  1615050 2023-03-02 22:29:36.000000 dreem-0.1.8/dreem/draw/resources/my_dataset.feather
--rw-r--r--   0 ymdt       (501) staff       (20)    16796 2023-04-21 22:52:06.000000 dreem-0.1.8/dreem/draw/study.py
--rw-r--r--   0 ymdt       (501) staff       (20)    11285 2023-03-04 01:28:54.000000 dreem-0.1.8/dreem/draw/util.py
--rw-r--r--   0 ymdt       (501) staff       (20)      766 2023-04-24 02:55:28.000000 dreem-0.1.8/dreem/env.yml
--rw-r--r--   0 ymdt       (501) staff       (20)    10067 2023-04-19 20:17:44.000000 dreem-0.1.8/dreem/main.py
--rw-r--r--   0 ymdt       (501) staff       (20)     2501 2023-04-19 20:17:44.000000 dreem-0.1.8/dreem/requirements.txt
-drwxr-xr-x   0 ymdt       (501) staff       (20)        0 2023-04-26 03:43:48.440691 dreem-0.1.8/dreem/resources/
--rw-r--r--   0 ymdt       (501) staff       (20)        0 2023-02-28 01:36:53.000000 dreem-0.1.8/dreem/resources/__init__.py
--rw-r--r--   0 ymdt       (501) staff       (20)      475 2023-02-28 01:36:53.000000 dreem-0.1.8/dreem/resources/get_attributes.py
-drwxr-xr-x   0 ymdt       (501) staff       (20)        0 2023-04-26 03:43:48.443463 dreem-0.1.8/dreem/util/
--rw-r--r--   0 ymdt       (501) staff       (20)        0 2023-02-28 01:36:53.000000 dreem-0.1.8/dreem/util/__init__.py
--rw-r--r--   0 ymdt       (501) staff       (20)      163 2023-04-11 18:17:48.000000 dreem-0.1.8/dreem/util/artxt.py
--rw-r--r--   0 ymdt       (501) staff       (20)    25083 2023-04-21 17:32:54.000000 dreem-0.1.8/dreem/util/cli.py
--rw-r--r--   0 ymdt       (501) staff       (20)     7279 2023-04-19 20:17:44.000000 dreem-0.1.8/dreem/util/dependencies.py
--rw-r--r--   0 ymdt       (501) staff       (20)     4365 2023-02-28 01:36:53.000000 dreem-0.1.8/dreem/util/dms.py
--rw-r--r--   0 ymdt       (501) staff       (20)     6867 2023-04-04 22:14:41.000000 dreem-0.1.8/dreem/util/docdef.py
--rw-r--r--   0 ymdt       (501) staff       (20)     2264 2023-03-02 22:29:36.000000 dreem-0.1.8/dreem/util/docstring.py
--rw-r--r--   0 ymdt       (501) staff       (20)     1911 2023-03-02 22:29:36.000000 dreem-0.1.8/dreem/util/dump.py
--rw-r--r--   0 ymdt       (501) staff       (20)    13411 2023-04-19 20:17:44.000000 dreem-0.1.8/dreem/util/files_sanity.py
--rw-r--r--   0 ymdt       (501) staff       (20)     3682 2023-04-19 20:17:44.000000 dreem-0.1.8/dreem/util/logs.py
--rw-r--r--   0 ymdt       (501) staff       (20)     5530 2023-04-11 18:17:48.000000 dreem-0.1.8/dreem/util/parallel.py
--rw-r--r--   0 ymdt       (501) staff       (20)    58372 2023-04-21 17:36:14.000000 dreem-0.1.8/dreem/util/path.py
--rw-r--r--   0 ymdt       (501) staff       (20)     7376 2023-04-19 20:17:44.000000 dreem-0.1.8/dreem/util/rnastructure.py
--rw-r--r--   0 ymdt       (501) staff       (20)     8030 2023-04-19 20:17:44.000000 dreem-0.1.8/dreem/util/seq.py
--rw-r--r--   0 ymdt       (501) staff       (20)      859 2023-04-11 18:17:48.000000 dreem-0.1.8/dreem/util/shell.py
--rw-r--r--   0 ymdt       (501) staff       (20)     6024 2023-04-11 18:17:48.000000 dreem-0.1.8/dreem/util/util.py
-drwxr-xr-x   0 ymdt       (501) staff       (20)        0 2023-04-26 03:43:48.444277 dreem-0.1.8/dreem/vector/
--rw-r--r--   0 ymdt       (501) staff       (20)       35 2023-03-06 17:48:28.000000 dreem-0.1.8/dreem/vector/__init__.py
--rw-r--r--   0 ymdt       (501) staff       (20)     6621 2023-04-19 20:17:44.000000 dreem-0.1.8/dreem/vector/main.py
--rw-r--r--   0 ymdt       (501) staff       (20)    71580 2023-04-19 20:17:44.000000 dreem-0.1.8/dreem/vector/profile.py
--rw-r--r--   0 ymdt       (501) staff       (20)    15683 2023-04-19 20:17:44.000000 dreem-0.1.8/dreem/vector/samread.py
--rw-r--r--   0 ymdt       (501) staff       (20)    38492 2023-04-19 20:17:44.000000 dreem-0.1.8/dreem/vector/vector.py
-drwxr-xr-x   0 ymdt       (501) staff       (20)        0 2023-04-26 03:43:48.434490 dreem-0.1.8/dreem.egg-info/
--rw-r--r--   0 ymdt       (501) staff       (20)     1195 2023-04-26 03:43:48.000000 dreem-0.1.8/dreem.egg-info/PKG-INFO
--rw-r--r--   0 ymdt       (501) staff       (20)     1548 2023-04-26 03:43:48.000000 dreem-0.1.8/dreem.egg-info/SOURCES.txt
--rw-r--r--   0 ymdt       (501) staff       (20)        1 2023-04-26 03:43:48.000000 dreem-0.1.8/dreem.egg-info/dependency_links.txt
--rw-r--r--   0 ymdt       (501) staff       (20)       43 2023-04-26 03:43:48.000000 dreem-0.1.8/dreem.egg-info/entry_points.txt
--rw-r--r--   0 ymdt       (501) staff       (20)     2501 2023-04-26 03:43:48.000000 dreem-0.1.8/dreem.egg-info/requires.txt
--rw-r--r--   0 ymdt       (501) staff       (20)        6 2023-04-26 03:43:48.000000 dreem-0.1.8/dreem.egg-info/top_level.txt
--rw-r--r--   0 ymdt       (501) staff       (20)      648 2023-04-03 01:51:29.000000 dreem-0.1.8/pyproject.toml
--rw-r--r--   0 ymdt       (501) staff       (20)       38 2023-04-26 03:43:48.445291 dreem-0.1.8/setup.cfg
--rw-r--r--   0 ymdt       (501) staff       (20)      971 2023-04-26 03:43:01.000000 dreem-0.1.8/setup.py
-drwxr-xr-x   0 ymdt       (501) staff       (20)        0 2023-04-26 03:43:48.444818 dreem-0.1.8/test/
--rw-r--r--   0 ymdt       (501) staff       (20)     2001 2023-04-24 02:55:28.000000 dreem-0.1.8/test/test_demultiplexing.py
--rw-r--r--   0 ymdt       (501) staff       (20)     7167 2023-04-19 20:17:44.000000 dreem-0.1.8/test/test_pipeline.py
+drwxr-xr-x   0 ymdt       (501) staff       (20)        0 2023-05-10 03:22:49.432646 dreem-0.1.9/
+-rw-r--r--   0 ymdt       (501) staff       (20)     1227 2023-03-27 06:57:46.000000 dreem-0.1.9/LICENSE
+-rw-r--r--   0 ymdt       (501) staff       (20)      131 2023-04-19 20:17:44.000000 dreem-0.1.9/MANIFEST.in
+-rw-r--r--   0 ymdt       (501) staff       (20)     1195 2023-05-10 03:22:49.432476 dreem-0.1.9/PKG-INFO
+-rw-r--r--   0 ymdt       (501) staff       (20)      916 2023-04-22 00:57:35.000000 dreem-0.1.9/README.md
+drwxr-xr-x   0 ymdt       (501) staff       (20)        0 2023-05-10 03:22:49.408028 dreem-0.1.9/dreem/
+-rw-r--r--   0 ymdt       (501) staff       (20)      177 2023-04-19 20:17:44.000000 dreem-0.1.9/dreem/__init__.py
+drwxr-xr-x   0 ymdt       (501) staff       (20)        0 2023-05-10 03:22:49.411225 dreem-0.1.9/dreem/aggregate/
+-rw-r--r--   0 ymdt       (501) staff       (20)       35 2023-03-27 06:57:46.000000 dreem-0.1.9/dreem/aggregate/__init__.py
+-rw-r--r--   0 ymdt       (501) staff       (20)     2651 2023-03-02 22:29:36.000000 dreem-0.1.9/dreem/aggregate/library.py
+-rw-r--r--   0 ymdt       (501) staff       (20)     1976 2023-03-27 06:57:46.000000 dreem-0.1.9/dreem/aggregate/library_samples.py
+-rw-r--r--   0 ymdt       (501) staff       (20)     6714 2023-04-19 20:17:44.000000 dreem-0.1.9/dreem/aggregate/main.py
+-rw-r--r--   0 ymdt       (501) staff       (20)     3388 2023-04-19 20:17:44.000000 dreem-0.1.9/dreem/aggregate/mutation_count.py
+drwxr-xr-x   0 ymdt       (501) staff       (20)        0 2023-05-10 03:22:49.413080 dreem-0.1.9/dreem/align/
+-rw-r--r--   0 ymdt       (501) staff       (20)       35 2023-03-06 17:48:28.000000 dreem-0.1.9/dreem/align/__init__.py
+-rw-r--r--   0 ymdt       (501) staff       (20)    21882 2023-04-11 18:17:48.000000 dreem-0.1.9/dreem/align/fq2bam.py
+-rwxr-xr-x   0 ymdt       (501) staff       (20)    25001 2023-04-11 18:17:48.000000 dreem-0.1.9/dreem/align/fqs.py
+-rw-r--r--   0 ymdt       (501) staff       (20)     7100 2023-04-19 20:17:44.000000 dreem-0.1.9/dreem/align/main.py
+-rwxr-xr-x   0 ymdt       (501) staff       (20)     9982 2023-04-19 20:17:44.000000 dreem-0.1.9/dreem/align/xams.py
+drwxr-xr-x   0 ymdt       (501) staff       (20)        0 2023-05-10 03:22:49.414763 dreem-0.1.9/dreem/cluster/
+-rw-r--r--   0 ymdt       (501) staff       (20)    13117 2023-04-04 22:14:41.000000 dreem-0.1.9/dreem/cluster/EMclustering.py
+-rw-r--r--   0 ymdt       (501) staff       (20)       35 2023-04-04 22:14:41.000000 dreem-0.1.9/dreem/cluster/__init__.py
+-rw-r--r--   0 ymdt       (501) staff       (20)     8800 2023-04-19 20:17:44.000000 dreem-0.1.9/dreem/cluster/bitvector.py
+-rw-r--r--   0 ymdt       (501) staff       (20)     6503 2023-04-19 20:17:44.000000 dreem-0.1.9/dreem/cluster/clusteringAnalysis.py
+-rw-r--r--   0 ymdt       (501) staff       (20)     3628 2023-04-19 20:17:44.000000 dreem-0.1.9/dreem/cluster/main.py
+drwxr-xr-x   0 ymdt       (501) staff       (20)        0 2023-05-10 03:22:49.416043 dreem-0.1.9/dreem/demultiplex/
+-rw-r--r--   0 ymdt       (501) staff       (20)       35 2023-03-27 06:57:46.000000 dreem-0.1.9/dreem/demultiplex/__init__.py
+-rw-r--r--   0 ymdt       (501) staff       (20)    39590 2023-04-28 18:15:16.000000 dreem-0.1.9/dreem/demultiplex/demultiplex.py
+-rw-r--r--   0 ymdt       (501) staff       (20)     1819 2023-04-21 17:32:54.000000 dreem-0.1.9/dreem/demultiplex/main.py
+-rw-r--r--   0 ymdt       (501) staff       (20)     5514 2023-04-28 18:15:16.000000 dreem-0.1.9/dreem/demultiplex/slurm_dispatch.py
+drwxr-xr-x   0 ymdt       (501) staff       (20)        0 2023-05-10 03:22:49.418300 dreem-0.1.9/dreem/draw/
+-rw-r--r--   0 ymdt       (501) staff       (20)      315 2023-04-04 22:14:41.000000 dreem-0.1.9/dreem/draw/__init__.py
+-rw-r--r--   0 ymdt       (501) staff       (20)      225 2023-03-02 22:29:36.000000 dreem-0.1.9/dreem/draw/load_dataset.py
+-rw-r--r--   0 ymdt       (501) staff       (20)     5995 2023-04-19 20:17:44.000000 dreem-0.1.9/dreem/draw/main.py
+-rw-r--r--   0 ymdt       (501) staff       (20)     6682 2023-05-10 03:21:59.000000 dreem-0.1.9/dreem/draw/manipulator.py
+-rw-r--r--   0 ymdt       (501) staff       (20)    22424 2023-04-21 23:08:14.000000 dreem-0.1.9/dreem/draw/plotter.py
+drwxr-xr-x   0 ymdt       (501) staff       (20)        0 2023-05-10 03:22:49.418660 dreem-0.1.9/dreem/draw/resources/
+-rw-r--r--   0 ymdt       (501) staff       (20)  1615050 2023-03-02 22:29:36.000000 dreem-0.1.9/dreem/draw/resources/my_dataset.feather
+-rw-r--r--   0 ymdt       (501) staff       (20)    16817 2023-04-27 20:53:41.000000 dreem-0.1.9/dreem/draw/study.py
+-rw-r--r--   0 ymdt       (501) staff       (20)    11285 2023-03-04 01:28:54.000000 dreem-0.1.9/dreem/draw/util.py
+-rw-r--r--   0 ymdt       (501) staff       (20)      766 2023-04-24 02:55:28.000000 dreem-0.1.9/dreem/env.yml
+-rw-r--r--   0 ymdt       (501) staff       (20)    10067 2023-04-19 20:17:44.000000 dreem-0.1.9/dreem/main.py
+-rw-r--r--   0 ymdt       (501) staff       (20)     2501 2023-04-19 20:17:44.000000 dreem-0.1.9/dreem/requirements.txt
+drwxr-xr-x   0 ymdt       (501) staff       (20)        0 2023-05-10 03:22:49.421299 dreem-0.1.9/dreem/resources/
+-rw-r--r--   0 ymdt       (501) staff       (20)        0 2023-02-28 01:36:53.000000 dreem-0.1.9/dreem/resources/__init__.py
+-rw-r--r--   0 ymdt       (501) staff       (20)      475 2023-02-28 01:36:53.000000 dreem-0.1.9/dreem/resources/get_attributes.py
+drwxr-xr-x   0 ymdt       (501) staff       (20)        0 2023-05-10 03:22:49.429715 dreem-0.1.9/dreem/util/
+-rw-r--r--   0 ymdt       (501) staff       (20)        0 2023-02-28 01:36:53.000000 dreem-0.1.9/dreem/util/__init__.py
+-rw-r--r--   0 ymdt       (501) staff       (20)      163 2023-04-11 18:17:48.000000 dreem-0.1.9/dreem/util/artxt.py
+-rw-r--r--   0 ymdt       (501) staff       (20)    25083 2023-04-21 17:32:54.000000 dreem-0.1.9/dreem/util/cli.py
+-rw-r--r--   0 ymdt       (501) staff       (20)     7279 2023-04-19 20:17:44.000000 dreem-0.1.9/dreem/util/dependencies.py
+-rw-r--r--   0 ymdt       (501) staff       (20)     4365 2023-02-28 01:36:53.000000 dreem-0.1.9/dreem/util/dms.py
+-rw-r--r--   0 ymdt       (501) staff       (20)     6867 2023-04-04 22:14:41.000000 dreem-0.1.9/dreem/util/docdef.py
+-rw-r--r--   0 ymdt       (501) staff       (20)     2264 2023-03-02 22:29:36.000000 dreem-0.1.9/dreem/util/docstring.py
+-rw-r--r--   0 ymdt       (501) staff       (20)     1911 2023-03-02 22:29:36.000000 dreem-0.1.9/dreem/util/dump.py
+-rw-r--r--   0 ymdt       (501) staff       (20)    13411 2023-04-19 20:17:44.000000 dreem-0.1.9/dreem/util/files_sanity.py
+-rw-r--r--   0 ymdt       (501) staff       (20)     3682 2023-04-19 20:17:44.000000 dreem-0.1.9/dreem/util/logs.py
+-rw-r--r--   0 ymdt       (501) staff       (20)     5530 2023-04-11 18:17:48.000000 dreem-0.1.9/dreem/util/parallel.py
+-rw-r--r--   0 ymdt       (501) staff       (20)    58372 2023-04-21 17:36:14.000000 dreem-0.1.9/dreem/util/path.py
+-rw-r--r--   0 ymdt       (501) staff       (20)     7376 2023-04-19 20:17:44.000000 dreem-0.1.9/dreem/util/rnastructure.py
+-rw-r--r--   0 ymdt       (501) staff       (20)     8030 2023-04-19 20:17:44.000000 dreem-0.1.9/dreem/util/seq.py
+-rw-r--r--   0 ymdt       (501) staff       (20)      859 2023-04-11 18:17:48.000000 dreem-0.1.9/dreem/util/shell.py
+-rw-r--r--   0 ymdt       (501) staff       (20)     6024 2023-04-11 18:17:48.000000 dreem-0.1.9/dreem/util/util.py
+drwxr-xr-x   0 ymdt       (501) staff       (20)        0 2023-05-10 03:22:49.431599 dreem-0.1.9/dreem/vector/
+-rw-r--r--   0 ymdt       (501) staff       (20)       35 2023-03-06 17:48:28.000000 dreem-0.1.9/dreem/vector/__init__.py
+-rw-r--r--   0 ymdt       (501) staff       (20)     6621 2023-04-19 20:17:44.000000 dreem-0.1.9/dreem/vector/main.py
+-rw-r--r--   0 ymdt       (501) staff       (20)    71580 2023-04-19 20:17:44.000000 dreem-0.1.9/dreem/vector/profile.py
+-rw-r--r--   0 ymdt       (501) staff       (20)    15683 2023-04-19 20:17:44.000000 dreem-0.1.9/dreem/vector/samread.py
+-rw-r--r--   0 ymdt       (501) staff       (20)    38492 2023-04-19 20:17:44.000000 dreem-0.1.9/dreem/vector/vector.py
+drwxr-xr-x   0 ymdt       (501) staff       (20)        0 2023-05-10 03:22:49.409414 dreem-0.1.9/dreem.egg-info/
+-rw-r--r--   0 ymdt       (501) staff       (20)     1195 2023-05-10 03:22:49.000000 dreem-0.1.9/dreem.egg-info/PKG-INFO
+-rw-r--r--   0 ymdt       (501) staff       (20)     1584 2023-05-10 03:22:49.000000 dreem-0.1.9/dreem.egg-info/SOURCES.txt
+-rw-r--r--   0 ymdt       (501) staff       (20)        1 2023-05-10 03:22:49.000000 dreem-0.1.9/dreem.egg-info/dependency_links.txt
+-rw-r--r--   0 ymdt       (501) staff       (20)       43 2023-05-10 03:22:49.000000 dreem-0.1.9/dreem.egg-info/entry_points.txt
+-rw-r--r--   0 ymdt       (501) staff       (20)     2501 2023-05-10 03:22:49.000000 dreem-0.1.9/dreem.egg-info/requires.txt
+-rw-r--r--   0 ymdt       (501) staff       (20)        6 2023-05-10 03:22:49.000000 dreem-0.1.9/dreem.egg-info/top_level.txt
+-rw-r--r--   0 ymdt       (501) staff       (20)      648 2023-04-03 01:51:29.000000 dreem-0.1.9/pyproject.toml
+-rw-r--r--   0 ymdt       (501) staff       (20)       38 2023-05-10 03:22:49.432699 dreem-0.1.9/setup.cfg
+-rw-r--r--   0 ymdt       (501) staff       (20)      971 2023-05-10 03:22:25.000000 dreem-0.1.9/setup.py
+drwxr-xr-x   0 ymdt       (501) staff       (20)        0 2023-05-10 03:22:49.432065 dreem-0.1.9/test/
+-rw-r--r--   0 ymdt       (501) staff       (20)     5805 2023-04-28 18:15:16.000000 dreem-0.1.9/test/test_demultiplexing.py
+-rw-r--r--   0 ymdt       (501) staff       (20)     7167 2023-04-19 20:17:44.000000 dreem-0.1.9/test/test_pipeline.py
```

### Comparing `dreem-0.1.8/LICENSE` & `dreem-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `dreem-0.1.8/PKG-INFO` & `dreem-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dreem
-Version: 0.1.8
+Version: 0.1.9
 Summary: DREEM solves RNA structure ensembles using chemical probing data
 Home-page: https://github.com/rouskinlab/dreem
 Author: Silvi Rouskin Lab
 Author-email: silvi@hms.harvard.edu
 Requires-Python: >=3.10
 License-File: LICENSE
```

### Comparing `dreem-0.1.8/README.md` & `dreem-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `dreem-0.1.8/dreem/aggregate/library.py` & `dreem-0.1.9/dreem/aggregate/library.py`

 * *Files identical despite different names*

### Comparing `dreem-0.1.8/dreem/aggregate/library_samples.py` & `dreem-0.1.9/dreem/aggregate/library_samples.py`

 * *Files identical despite different names*

### Comparing `dreem-0.1.8/dreem/aggregate/main.py` & `dreem-0.1.9/dreem/aggregate/main.py`

 * *Files identical despite different names*

### Comparing `dreem-0.1.8/dreem/aggregate/mutation_count.py` & `dreem-0.1.9/dreem/aggregate/mutation_count.py`

 * *Files identical despite different names*

### Comparing `dreem-0.1.8/dreem/align/fq2bam.py` & `dreem-0.1.9/dreem/align/fq2bam.py`

 * *Files identical despite different names*

### Comparing `dreem-0.1.8/dreem/align/fqs.py` & `dreem-0.1.9/dreem/align/fqs.py`

 * *Files identical despite different names*

### Comparing `dreem-0.1.8/dreem/align/main.py` & `dreem-0.1.9/dreem/align/main.py`

 * *Files identical despite different names*

### Comparing `dreem-0.1.8/dreem/align/xams.py` & `dreem-0.1.9/dreem/align/xams.py`

 * *Files identical despite different names*

### Comparing `dreem-0.1.8/dreem/cluster/EMclustering.py` & `dreem-0.1.9/dreem/cluster/EMclustering.py`

 * *Files identical despite different names*

### Comparing `dreem-0.1.8/dreem/cluster/bitvector.py` & `dreem-0.1.9/dreem/cluster/bitvector.py`

 * *Files identical despite different names*

### Comparing `dreem-0.1.8/dreem/cluster/clusteringAnalysis.py` & `dreem-0.1.9/dreem/cluster/clusteringAnalysis.py`

 * *Files identical despite different names*

### Comparing `dreem-0.1.8/dreem/cluster/main.py` & `dreem-0.1.9/dreem/cluster/main.py`

 * *Files identical despite different names*

### Comparing `dreem-0.1.8/dreem/demultiplex/demultiplex.py` & `dreem-0.1.9/dreem/demultiplex/demultiplex.py`

 * *Files 2% similar despite different names*

```diff
@@ -428,25 +428,26 @@
     """
     1 indexed? 
     
     """
     append_char=">>" if append_bool else ">"
 
     if(search_start_ind -tolerance<0):
-        search_start_ind =0
+        search_start_ind = 0
     else:
-        search_start_ind-=tolerance
-    search_end_index+=tolerance
+        search_start_ind -= tolerance
+    #search_end_index+=tolerance
     if(search_start_ind<1):
-        search_end_index+=abs(search_start_ind)+1
+        search_end_index+=abs(search_start_ind)
         search_start_ind=1
+    print(f"")
     cmd=f'seqkit --threads {threads} grep -s -R {search_start_ind}:{search_end_index+tolerance} -p "{pattern}" -m {mismatch_threshhold} -P {fastq_to_search} > {fastq_to_write}'
     print(cmd)#debug-
     return_code=os.system(cmd)#debug
-    if (delete_fq):
+    if (delete_fq): 
         os.remove(fastq_to_write)
     return (set(makes_dict_from_fastq(fastq_to_write).keys()))
 
 
 
 
 
@@ -479,14 +480,15 @@
 
 
 """
 def make_sequence_objects_from_csv(input_csv,barcode_start,barcode_length,fasta,fastq1_path,fastq2_path,paired,workspace) -> dict:
     
     sequence_object_dict={}
     fasta_dict=make_dict_from_fasta(fasta)
+    #barcode_start-=1
     if (input_csv==""):
 
         for name in fasta_dict.keys():
 
             seq=fasta_dict[name]
             rev_seq=reverse_compliment(seq)
             bc=seq[barcode_start :barcode_start+barcode_length]
@@ -521,40 +523,45 @@
         df=pd.read_csv(input_csv)
 
         
         #fasta_dict=make_dict_from_fasta(fasta)
 
         #sequence_object_dict={}
         cols=set(df.columns)
-
-        if(barcode_start==barcode_length) and ("barcode_start" not in cols):
+        #(barcode_start==0 and barcode_length==0) is the case that barcode info is not given as an argument
+        if(barcode_start==0 and barcode_length==0) and ("barcode_start" not in cols):
             raise Exception("no barcode info given")
         
             
         for x in df.index:
 
             name=df.at[x,"reference"]
             seq=fasta_dict[name]
             rev_seq=reverse_compliment(seq)
 
-            
-            if(barcode_start==barcode_length):
+
+            #print(f"{barcode_start}=={barcode_length}")
+            if(barcode_start==0 and barcode_length==0):
                 barcode_start=df.at[x,"barcode_start"]
                 barcode_length=df.at[x,"barcode_length"]
-                bc=seq[barcode_start :barcode_start+barcode_length]
+                bc=seq[barcode_start -1:barcode_start-1+barcode_length]
+                #print(f"barcode: {bc}")
             else:
-                bc=seq[barcode_start:barcode_start+barcode_length]
+                bc=seq[barcode_start-1:barcode_start-1+barcode_length]
+
             rev_barcode=reverse_compliment(bc)
             rev_bc_start=rev_seq.index(rev_barcode)
             rev_bc_end=rev_bc_start+len(rev_barcode)
-            print("\nhere"+str(cols))
+            #print("\nhere"+str(cols))
             if("secondary_signature_start" in cols ):
+                
                 secondary_sign_start=df.at[x,"secondary_signature_start"]
+                #secondary_sign_start-=1
                 secondary_sign_end=secondary_sign_start+df.at[x,"secondary_signature_length"]
-                secondary_sign=fasta_dict[name][secondary_sign_start:secondary_sign_end]
+                secondary_sign=fasta_dict[name][secondary_sign_start-1:secondary_sign_end-1]
 
                 rev_sec_sign=reverse_compliment(secondary_sign)
                 rev_sec_sign_start = rev_seq.index(rev_sec_sign)
                 rev_sec_sign_end= rev_sec_sign_start +len(rev_sec_sign)
 
 
             else:
@@ -606,17 +613,19 @@
 index tolerence can only apply to the initial but there are cases where that could false 
 """
 def run_multi_greps(read_id_dict:dict,clipped:int,index_tolerence:int,delete_fastqs:bool,mismatches_allowed:int,pattern_type:str,pattern:str,pattern_start:int,pattern_end:int,fastq:str,seq_folder:str,front:bool=False):
     #debug#print("running multi_greps for ", pattern_type)
     new_reads_dict={}
     folder=seq_folder
     #file_name_start=
+    print(f"pattern start: {pattern_start} pattern end: {pattern_end}")
     new_reads_dict["init_"+pattern_type]=run_seqkit_grep_function(pattern=pattern,search_start_ind=pattern_start,search_end_index=pattern_end,fastq_to_search=fastq,fastq_to_write=seq_folder+"init_"+pattern_type+".fastq",mismatch_threshhold=mismatches_allowed,tolerance=index_tolerence)
     #if(len(pattern)-pattern_end)<clipped:
     append_these=[seq_folder+"init_"+pattern_type+".fastq"]
+    print("index tolerence: "+ str(index_tolerence))
     clipped+=1
     #print("initial grep run")#debug
     if not front:
         for x in range(1,clipped):
             
             append_these.append(seq_folder+pattern_type+"_clipped_"+str(x)+".fastq")
             new_reads_dict[pattern_type+"_clipped_"+str(x)]=run_seqkit_grep_function(pattern=pattern[:len(pattern)-x],search_start_ind=pattern_start+x,search_end_index=pattern_end,fastq_to_search=fastq,fastq_to_write=seq_folder+pattern_type+"_clipped_"+str(x)+".fastq",mismatch_threshhold=0,tolerance=0)
@@ -678,14 +687,15 @@
     fastq_rev_sec_filtered=fastq_folder + "rev_sec_filtered.fastq"
     
     fastq_filtered=fastq_folder + "filtered_out.fastq"
 
     read_ids={}
     bc_fastq=run_multi_greps(read_id_dict=read_ids,clipped=clipped,index_tolerence=index_tolerence,delete_fastqs=delete_fastqs,mismatches_allowed=mismatches_allowed,pattern_type="barcode",pattern=sequence_object.barcode,pattern_start=sequence_object.barcode_start,pattern_end=sequence_object.barcode_end,fastq=fastq,seq_folder=fastq_folder)
     #debug#print("first_multi_run")
+    print("index tolerence: "+ str(index_tolerence))
     rev_bc_fastq=run_multi_greps(read_id_dict=read_ids,clipped=0,index_tolerence=index_tolerence,delete_fastqs=delete_fastqs,mismatches_allowed=mismatches_allowed,pattern_type="rev_barcode",pattern=sequence_object.rev_barcode,pattern_start=sequence_object.rev_barcode_start,pattern_end=sequence_object.rev_barcode_end,fastq=fastq,seq_folder=fastq_folder)
 
     append_files([bc_fastq,rev_bc_fastq],fastq_unfiltered)
     read_ids["unfiltered"]=set(makes_dict_from_fastq(fastq_unfiltered).keys())
 
     
     complete_set=set()
@@ -705,18 +715,20 @@
         secondary_sign_mismatches=v_threshold#TODO hardcoded :(
 
 
         read_ids["sec_filter"]=run_seqkit_grep_function(pattern=sequence_object.secondary_signature,search_start_ind=sequence_object.secondary_signature_start,search_end_index=sequence_object.secondary_signature_end,fastq_to_search=fastq_unfiltered,fastq_to_write=fastq_sec_filtered,mismatch_threshhold=secondary_sign_mismatches,tolerance=2)
         read_ids["rev_sec_filter"]=run_seqkit_grep_function(pattern=sequence_object.rev_secondary_signature,search_start_ind=sequence_object.rev_secondary_signature_start,search_end_index=sequence_object.rev_secondary_signature_end,fastq_to_search=fastq_unfiltered,fastq_to_write=fastq_rev_sec_filtered,mismatch_threshhold=secondary_sign_mismatches,tolerance=2)
         complete_set=read_ids["sec_filter"].union(read_ids["rev_sec_filter"])
         read_ids["reads_lost_to_filter"]=read_ids["unfiltered"]-complete_set
+        read_ids["pre_union"]=complete_set
         #complete_set=read_ids["sec_filter"].union(read_ids["rev_sec_filter"])
     else:
         complete_set=read_ids["unfiltered"]
     #here the sets need to be compared in order to identify which ids were unique to which search
+    read_ids
     #TODO
     
     #print(vars(sequence_object))
     #complete_set=read_ids["sec_filter"].union(read_ids["rev_sec_filter"])
 
     complete_set_pickle=fastq_folder+"complete_set_of_reads.p"
     pickle.dump(complete_set,open(complete_set_pickle,"wb"))
@@ -995,16 +1007,16 @@
 
     for k in dict_of_lists.keys():
         df[k]=dict_of_lists[k]
     print("len: mixed: ",len(mixed_total_dict[FQS[0]]))
     print("len: mixed: ",len(mixed_total_dict[FQS[0]])," / ",orginal_len[FQS[0]]," = ",len(mixed_total_dict[FQS[0]])/orginal_len[FQS[0]])
     len_col=[" "]*len(sequence_objects.keys())
     len_col[0]=len(mixed_total_dict[FQS[0]])
-    df["percent_reads_used"]=[(1-(len(mixed_total_dict[FQS[0]])/orginal_len[FQS[0]]))*100]*len(sequence_objects.keys())
-    df["total_read_count"]=len_col
+    df["percent_reads_unused"]=[(1-(len(mixed_total_dict[FQS[0]])/orginal_len[FQS[0]]))*100]*len(sequence_objects.keys())
+    df["orginal_fq_total_read_count"]=orginal_len[FQS[0]]
 
     print(working_directory+"demultiplex_info.csv")
     df.to_csv(working_directory+"demultiplex_info.csv",index=False)
 
 
 
 """
@@ -1045,15 +1057,17 @@
         barcode_length=barcode_length,
         fasta=fasta,
         fastq1_path=mixed_fastq1,
         fastq2_path=mixed_fastq2,
         paired=True,
         workspace=seq_data_folder)
 
-    #print("\nhere:\n"+(sequence_objects))
+    for k in sequence_objects.keys():
+
+        print(vars(sequence_objects[k]))
     #print("workspace: ",vars(sequence_objects["3042-O-flank_1=hp1-DB"]))
     #demultiplex_workspace=demulti_workspace#"demultiplexed_sequences/"
     """
     makes a super fastq for memory efficent access to fastq reads
 
     checks values of ids to verify that the two fastq provided contain matching paired end reads
     """
```

### Comparing `dreem-0.1.8/dreem/demultiplex/main.py` & `dreem-0.1.9/dreem/demultiplex/main.py`

 * *Files identical despite different names*

### Comparing `dreem-0.1.8/dreem/draw/main.py` & `dreem-0.1.9/dreem/draw/main.py`

 * *Files identical despite different names*

### Comparing `dreem-0.1.8/dreem/draw/manipulator.py` & `dreem-0.1.9/dreem/draw/manipulator.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,14 +21,17 @@
     if base_type is not ['A','C','G','T']:
         index = list(set(index) & set(__find_base_in_sequence(row['sequence'], base_type)))
     
     if base_pairing is not None:
         base_pairing_switch = lambda idx, base, pairing: idx if (base=='.' and not pairing) or (base in ['(',')'] and pairing) else None 
         structure = [base_pairing_switch(i,base,base_pairing) for i, base in enumerate(row['structure'])]
         index = list(set(index) & set([i for i in structure if i is not None]))
+        
+    index.sort()
+
     return index
 
 
 def get_df(df, sample=None, reference=None, section=None, cluster=None, min_cov=0, base_index=None, base_type=['A','C','G','T'], base_pairing=None, 
            RNAstructure_use_DMS=False, RNAstructure_use_temp=False, unique_id = False, index_selected=False, **kwargs)->pd.DataFrame:
     """Get a dataframe with filtered data
```

### Comparing `dreem-0.1.8/dreem/draw/plotter.py` & `dreem-0.1.9/dreem/draw/plotter.py`

 * *Files identical despite different names*

### Comparing `dreem-0.1.8/dreem/draw/resources/my_dataset.feather` & `dreem-0.1.9/dreem/draw/resources/my_dataset.feather`

 * *Files identical despite different names*

### Comparing `dreem-0.1.8/dreem/draw/study.py` & `dreem-0.1.9/dreem/draw/study.py`

 * *Files 1% similar despite different names*

```diff
@@ -117,15 +117,15 @@
                                 **{k:v for k,v in kwargs.items() if k in extract_args(func)})
 
     
     def default_arguments_per_base(self):
         """Default arguments for the plot functions.
         
         Args:
-            base_index (list[int], list[str], optional): Filter per-base attributes (sub_rate, sequence, etc) by base index. Can be a unique sequence in the row's sequence, a list of indexes or a single index. Defaults to None.
+            base_index (list, int, str, optional): Filter per-base attributes (sub_rate, sequence, etc) by base index, using 1-indexing. Can be a unique sequence in the row's sequence, a list of indexes or a single index. Gives a  Defaults to None.
             base_type (list, str, optional): Filter per-base attributes (sub_rate, sequence, etc) by base type. Defaults to ``['A','C','G','T']``.
             base_pairing (bool, optional): Filter per-base attributes (sub_rate, sequence, etc) by expected base pairing. True will keep only base pairs, False will keep only non-base pairs. Defaults to None.
             **kwargs: Additional arguments to pass to filter rows by. Ex: ``flank='flank_1'`` will keep only rows with ``flank==flank_1``. 
 
         Returns:
             dict: {``'fig'``: a plotly figure, ``'data'``: a pandas dataframe}
```

### Comparing `dreem-0.1.8/dreem/draw/util.py` & `dreem-0.1.9/dreem/draw/util.py`

 * *Files identical despite different names*

### Comparing `dreem-0.1.8/dreem/env.yml` & `dreem-0.1.9/dreem/env.yml`

 * *Files identical despite different names*

### Comparing `dreem-0.1.8/dreem/main.py` & `dreem-0.1.9/dreem/main.py`

 * *Files identical despite different names*

### Comparing `dreem-0.1.8/dreem/requirements.txt` & `dreem-0.1.9/dreem/requirements.txt`

 * *Files identical despite different names*

### Comparing `dreem-0.1.8/dreem/util/cli.py` & `dreem-0.1.9/dreem/util/cli.py`

 * *Files identical despite different names*

### Comparing `dreem-0.1.8/dreem/util/dependencies.py` & `dreem-0.1.9/dreem/util/dependencies.py`

 * *Files identical despite different names*

### Comparing `dreem-0.1.8/dreem/util/dms.py` & `dreem-0.1.9/dreem/util/dms.py`

 * *Files identical despite different names*

### Comparing `dreem-0.1.8/dreem/util/docdef.py` & `dreem-0.1.9/dreem/util/docdef.py`

 * *Files identical despite different names*

### Comparing `dreem-0.1.8/dreem/util/docstring.py` & `dreem-0.1.9/dreem/util/docstring.py`

 * *Files identical despite different names*

### Comparing `dreem-0.1.8/dreem/util/dump.py` & `dreem-0.1.9/dreem/util/dump.py`

 * *Files identical despite different names*

### Comparing `dreem-0.1.8/dreem/util/files_sanity.py` & `dreem-0.1.9/dreem/util/files_sanity.py`

 * *Files identical despite different names*

### Comparing `dreem-0.1.8/dreem/util/logs.py` & `dreem-0.1.9/dreem/util/logs.py`

 * *Files identical despite different names*

### Comparing `dreem-0.1.8/dreem/util/parallel.py` & `dreem-0.1.9/dreem/util/parallel.py`

 * *Files identical despite different names*

### Comparing `dreem-0.1.8/dreem/util/path.py` & `dreem-0.1.9/dreem/util/path.py`

 * *Files identical despite different names*

### Comparing `dreem-0.1.8/dreem/util/rnastructure.py` & `dreem-0.1.9/dreem/util/rnastructure.py`

 * *Files identical despite different names*

### Comparing `dreem-0.1.8/dreem/util/seq.py` & `dreem-0.1.9/dreem/util/seq.py`

 * *Files identical despite different names*

### Comparing `dreem-0.1.8/dreem/util/shell.py` & `dreem-0.1.9/dreem/util/shell.py`

 * *Files identical despite different names*

### Comparing `dreem-0.1.8/dreem/util/util.py` & `dreem-0.1.9/dreem/util/util.py`

 * *Files identical despite different names*

### Comparing `dreem-0.1.8/dreem/vector/main.py` & `dreem-0.1.9/dreem/vector/main.py`

 * *Files identical despite different names*

### Comparing `dreem-0.1.8/dreem/vector/profile.py` & `dreem-0.1.9/dreem/vector/profile.py`

 * *Files identical despite different names*

### Comparing `dreem-0.1.8/dreem/vector/samread.py` & `dreem-0.1.9/dreem/vector/samread.py`

 * *Files identical despite different names*

### Comparing `dreem-0.1.8/dreem/vector/vector.py` & `dreem-0.1.9/dreem/vector/vector.py`

 * *Files identical despite different names*

### Comparing `dreem-0.1.8/dreem.egg-info/PKG-INFO` & `dreem-0.1.9/dreem.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dreem
-Version: 0.1.8
+Version: 0.1.9
 Summary: DREEM solves RNA structure ensembles using chemical probing data
 Home-page: https://github.com/rouskinlab/dreem
 Author: Silvi Rouskin Lab
 Author-email: silvi@hms.harvard.edu
 Requires-Python: >=3.10
 License-File: LICENSE
```

### Comparing `dreem-0.1.8/dreem.egg-info/SOURCES.txt` & `dreem-0.1.9/dreem.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 dreem/cluster/__init__.py
 dreem/cluster/bitvector.py
 dreem/cluster/clusteringAnalysis.py
 dreem/cluster/main.py
 dreem/demultiplex/__init__.py
 dreem/demultiplex/demultiplex.py
 dreem/demultiplex/main.py
+dreem/demultiplex/slurm_dispatch.py
 dreem/draw/__init__.py
 dreem/draw/load_dataset.py
 dreem/draw/main.py
 dreem/draw/manipulator.py
 dreem/draw/plotter.py
 dreem/draw/study.py
 dreem/draw/util.py
```

### Comparing `dreem-0.1.8/dreem.egg-info/requires.txt` & `dreem-0.1.9/dreem.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `dreem-0.1.8/pyproject.toml` & `dreem-0.1.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dreem-0.1.8/setup.py` & `dreem-0.1.9/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # if sys.version_info < PYTHON_VERSION:
 #    sys.exit(f"Python >= {PYTHON_VERSION[0]}.{PYTHON_VERSION[1]} required.")
 
 readme = open('README.md').read()
 
 setup(
     name="dreem",
-    version='0.1.8',
+    version='0.1.9',
     description="DREEM solves RNA structure ensembles using chemical probing data",
     long_description=readme,
     author="Silvi Rouskin Lab",
     author_email="silvi@hms.harvard.edu",
     url="https://github.com/rouskinlab/dreem",
     packages=find_packages(),
     package_dir={'dreem': 'dreem'},
```

### Comparing `dreem-0.1.8/test/test_pipeline.py` & `dreem-0.1.9/test/test_pipeline.py`

 * *Files identical despite different names*

