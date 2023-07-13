# Comparing `tmp/evo-1.9.tar.gz` & `tmp/evo-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/evo-1.9.tar", last modified: Fri Jun  5 11:27:51 2020, max compression
+gzip compressed data, was "dist/evo-1.9.1.tar", last modified: Sun Jun 14 13:00:37 2020, max compression
```

## Comparing `evo-1.9.tar` & `evo-1.9.1.tar`

### file list

```diff
@@ -1,66 +1,59 @@
-drwxrwxr-x   0 grupp     (1000) grupp     (1000)        0 2020-06-05 11:27:51.000000 evo-1.9/
--rw-rw-r--   0 grupp     (1000) grupp     (1000)      102 2020-06-05 11:27:51.000000 evo-1.9/setup.cfg
--rw-rw-r--   0 grupp     (1000) grupp     (1000)    35147 2017-12-11 10:49:05.000000 evo-1.9/LICENSE
-drwxrwxr-x   0 grupp     (1000) grupp     (1000)        0 2020-06-05 11:27:51.000000 evo-1.9/evo.egg-info/
--rw-rw-r--   0 grupp     (1000) grupp     (1000)      267 2020-06-05 11:27:51.000000 evo-1.9/evo.egg-info/entry_points.txt
--rw-rw-r--   0 grupp     (1000) grupp     (1000)        1 2017-12-11 13:24:41.000000 evo-1.9/evo.egg-info/not-zip-safe
--rw-rw-r--   0 grupp     (1000) grupp     (1000)        4 2020-06-05 11:27:51.000000 evo-1.9/evo.egg-info/top_level.txt
--rw-rw-r--   0 grupp     (1000) grupp     (1000)      112 2020-06-05 11:27:51.000000 evo-1.9/evo.egg-info/requires.txt
--rw-rw-r--   0 grupp     (1000) grupp     (1000)        1 2020-06-05 11:27:51.000000 evo-1.9/evo.egg-info/dependency_links.txt
--rw-rw-r--   0 grupp     (1000) grupp     (1000)     1270 2020-06-05 11:27:51.000000 evo-1.9/evo.egg-info/SOURCES.txt
--rw-rw-r--   0 grupp     (1000) grupp     (1000)    14392 2020-06-05 11:27:51.000000 evo-1.9/evo.egg-info/PKG-INFO
-drwxrwxr-x   0 grupp     (1000) grupp     (1000)        0 2020-06-05 11:27:51.000000 evo-1.9/notebooks/
--rw-rw-r--   0 grupp     (1000) grupp     (1000)    10633 2020-01-16 15:45:53.000000 evo-1.9/notebooks/metrics_interactive.ipynb
--rw-rw-r--   0 grupp     (1000) grupp     (1000)     5598 2018-12-22 14:57:04.000000 evo-1.9/notebooks/pandas_bridge.ipynb
-drwxrwxr-x   0 grupp     (1000) grupp     (1000)        0 2020-06-05 11:27:51.000000 evo-1.9/notebooks/.ipynb_checkpoints/
--rw-rw-r--   0 grupp     (1000) grupp     (1000)    19833 2018-12-22 14:54:43.000000 evo-1.9/notebooks/.ipynb_checkpoints/metrics.py_API_Documentation-checkpoint.ipynb
--rw-rw-r--   0 grupp     (1000) grupp     (1000)    19964 2020-01-16 15:45:53.000000 evo-1.9/notebooks/metrics.py_API_Documentation.ipynb
--rw-rw-r--   0 grupp     (1000) grupp     (1000)      727 2019-02-07 10:21:13.000000 evo-1.9/notebooks/metrics_tutorial.ipynb
--rw-rw-r--   0 grupp     (1000) grupp     (1000)     3950 2019-09-09 16:29:57.000000 evo-1.9/fastentrypoints.py
-drwxrwxr-x   0 grupp     (1000) grupp     (1000)        0 2020-06-05 11:27:51.000000 evo-1.9/test/
--rwxrwxr-x   0 grupp     (1000) grupp     (1000)     2629 2019-04-10 08:29:43.000000 evo-1.9/test/test_result.py
--rwxrwxr-x   0 grupp     (1000) grupp     (1000)     8279 2020-02-13 09:05:29.000000 evo-1.9/test/test_trajectory.py
--rwxrwxr-x   0 grupp     (1000) grupp     (1000)     4929 2020-01-16 15:45:53.000000 evo-1.9/test/test_filters.py
--rwxrwxr-x   0 grupp     (1000) grupp     (1000)     7656 2020-06-02 13:58:51.000000 evo-1.9/test/test_file_interface.py
--rwxrwxr-x   0 grupp     (1000) grupp     (1000)     5950 2020-02-13 09:05:29.000000 evo-1.9/test/test_lie_algebra.py
--rwxrwxr-x   0 grupp     (1000) grupp     (1000)     3186 2019-09-09 16:31:22.000000 evo-1.9/test/test_sync.py
-drwxrwxr-x   0 grupp     (1000) grupp     (1000)        0 2020-06-05 11:27:51.000000 evo-1.9/evo/
--rw-rw-r--   0 grupp     (1000) grupp     (1000)     3727 2020-01-16 16:49:33.000000 evo-1.9/evo/entry_points.py
--rw-rw-r--   0 grupp     (1000) grupp     (1000)    35147 2017-12-11 10:49:05.000000 evo-1.9/evo/LICENSE
--rw-rw-r--   0 grupp     (1000) grupp     (1000)    11137 2019-09-09 16:31:22.000000 evo-1.9/evo/main_config.py
--rw-rw-r--   0 grupp     (1000) grupp     (1000)    13573 2019-10-15 13:04:50.000000 evo-1.9/evo/main_res.py
--rw-rw-r--   0 grupp     (1000) grupp     (1000)      614 2019-02-08 16:13:53.000000 evo-1.9/evo/__init__.py
--rw-rw-r--   0 grupp     (1000) grupp     (1000)     6865 2019-09-09 16:31:22.000000 evo-1.9/evo/main_evo.py
--rw-rw-r--   0 grupp     (1000) grupp     (1000)    23205 2019-02-07 10:21:13.000000 evo-1.9/evo/ipython_config.py
--rw-rw-r--   0 grupp     (1000) grupp     (1000)     6404 2020-05-29 09:17:36.000000 evo-1.9/evo/common_ape_rpe.py
--rwxrwxr-x   0 grupp     (1000) grupp     (1000)    11769 2020-01-29 09:04:34.000000 evo-1.9/evo/main_rpe.py
--rwxrwxr-x   0 grupp     (1000) grupp     (1000)    22869 2020-06-05 11:26:50.000000 evo-1.9/evo/main_traj.py
--rw-rw-r--   0 grupp     (1000) grupp     (1000)     2624 2019-09-09 16:31:22.000000 evo-1.9/evo/main_ipython.py
--rw-rw-r--   0 grupp     (1000) grupp     (1000)        5 2020-06-05 11:26:50.000000 evo-1.9/evo/version
--rw-rw-r--   0 grupp     (1000) grupp     (1000)     3631 2019-09-09 16:31:22.000000 evo-1.9/evo/main_fig.py
-drwxrwxr-x   0 grupp     (1000) grupp     (1000)        0 2020-06-05 11:27:51.000000 evo-1.9/evo/core/
--rw-rw-r--   0 grupp     (1000) grupp     (1000)     3219 2020-02-10 09:37:02.000000 evo-1.9/evo/core/geometry.py
--rw-rw-r--   0 grupp     (1000) grupp     (1000)    16401 2020-02-13 09:05:29.000000 evo-1.9/evo/core/trajectory.py
--rw-rw-r--   0 grupp     (1000) grupp     (1000)        0 2017-12-11 10:49:05.000000 evo-1.9/evo/core/__init__.py
--rw-rw-r--   0 grupp     (1000) grupp     (1000)     4231 2019-09-09 16:28:41.000000 evo-1.9/evo/core/sync.py
--rw-rw-r--   0 grupp     (1000) grupp     (1000)    13914 2019-09-09 16:31:22.000000 evo-1.9/evo/core/metrics.py
--rw-rw-r--   0 grupp     (1000) grupp     (1000)     5914 2020-02-13 09:05:29.000000 evo-1.9/evo/core/lie_algebra.py
--rw-rw-r--   0 grupp     (1000) grupp     (1000)     6746 2019-09-09 16:31:22.000000 evo-1.9/evo/core/filters.py
--rw-rw-r--   0 grupp     (1000) grupp     (1000)     4075 2019-04-10 08:29:43.000000 evo-1.9/evo/core/result.py
--rw-rw-r--   0 grupp     (1000) grupp     (1000)    66201 2019-09-09 16:31:22.000000 evo-1.9/evo/core/transformations.py
--rwxrwxr-x   0 grupp     (1000) grupp     (1000)    10197 2020-01-29 09:04:34.000000 evo-1.9/evo/main_ape.py
-drwxrwxr-x   0 grupp     (1000) grupp     (1000)        0 2020-06-05 11:27:51.000000 evo-1.9/evo/tools/
--rw-rw-r--   0 grupp     (1000) grupp     (1000)     4418 2019-09-09 16:31:22.000000 evo-1.9/evo/tools/settings.py
--rw-rw-r--   0 grupp     (1000) grupp     (1000)     1285 2018-01-04 10:04:08.000000 evo-1.9/evo/tools/compat.py
--rw-rw-r--   0 grupp     (1000) grupp     (1000)        0 2017-12-11 10:49:05.000000 evo-1.9/evo/tools/__init__.py
--rw-rw-r--   0 grupp     (1000) grupp     (1000)     3808 2020-01-16 16:22:35.000000 evo-1.9/evo/tools/log.py
--rw-rw-r--   0 grupp     (1000) grupp     (1000)     6418 2020-06-05 11:26:50.000000 evo-1.9/evo/tools/tf_cache.py
--rw-rw-r--   0 grupp     (1000) grupp     (1000)     2129 2020-06-05 11:26:50.000000 evo-1.9/evo/tools/pandas_bridge.py
--rw-rw-r--   0 grupp     (1000) grupp     (1000)    26662 2020-05-29 11:38:40.000000 evo-1.9/evo/tools/plot.py
--rw-rw-r--   0 grupp     (1000) grupp     (1000)     6335 2020-06-05 11:26:50.000000 evo-1.9/evo/tools/settings_template.py
--rw-rw-r--   0 grupp     (1000) grupp     (1000)     1322 2019-09-09 16:31:22.000000 evo-1.9/evo/tools/user.py
--rw-rw-r--   0 grupp     (1000) grupp     (1000)    16086 2020-06-05 11:26:50.000000 evo-1.9/evo/tools/file_interface.py
--rw-rw-r--   0 grupp     (1000) grupp     (1000)    14392 2020-06-05 11:27:51.000000 evo-1.9/PKG-INFO
--rw-rw-r--   0 grupp     (1000) grupp     (1000)      130 2018-10-19 11:00:43.000000 evo-1.9/MANIFEST.in
--rw-rw-r--   0 grupp     (1000) grupp     (1000)     3637 2020-01-29 09:04:34.000000 evo-1.9/setup.py
--rw-rw-r--   0 grupp     (1000) grupp     (1000)    11598 2020-06-05 11:26:50.000000 evo-1.9/README.md
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2020-06-14 13:00:37.830043 evo-1.9.1/
+-rw-r--r--   0 michael   (1000) michael   (1000)    35147 2019-12-21 12:57:46.000000 evo-1.9.1/LICENSE
+-rw-r--r--   0 michael   (1000) michael   (1000)      130 2019-12-21 12:57:46.000000 evo-1.9.1/MANIFEST.in
+-rw-rw-r--   0 michael   (1000) michael   (1000)    14394 2020-06-14 13:00:37.830043 evo-1.9.1/PKG-INFO
+-rw-rw-r--   0 michael   (1000) michael   (1000)    11598 2020-06-05 20:47:51.000000 evo-1.9.1/README.md
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2020-06-14 13:00:37.830043 evo-1.9.1/evo/
+-rw-r--r--   0 michael   (1000) michael   (1000)    35147 2019-12-21 12:57:46.000000 evo-1.9.1/evo/LICENSE
+-rw-r--r--   0 michael   (1000) michael   (1000)      614 2019-12-21 12:57:46.000000 evo-1.9.1/evo/__init__.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     6474 2020-06-14 11:50:34.000000 evo-1.9.1/evo/common_ape_rpe.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2020-06-14 13:00:37.830043 evo-1.9.1/evo/core/
+-rw-r--r--   0 michael   (1000) michael   (1000)        0 2019-12-21 12:57:46.000000 evo-1.9.1/evo/core/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     6746 2020-01-04 14:21:40.000000 evo-1.9.1/evo/core/filters.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     3219 2020-02-08 20:28:37.000000 evo-1.9.1/evo/core/geometry.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     5914 2020-02-12 23:32:21.000000 evo-1.9.1/evo/core/lie_algebra.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    13914 2019-12-27 11:22:20.000000 evo-1.9.1/evo/core/metrics.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     4075 2019-12-21 12:57:46.000000 evo-1.9.1/evo/core/result.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     4232 2020-06-14 11:50:34.000000 evo-1.9.1/evo/core/sync.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    16401 2020-02-12 23:32:21.000000 evo-1.9.1/evo/core/trajectory.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    66201 2019-12-21 12:57:46.000000 evo-1.9.1/evo/core/transformations.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     3745 2020-06-14 12:34:10.000000 evo-1.9.1/evo/entry_points.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    23205 2019-12-21 12:57:46.000000 evo-1.9.1/evo/ipython_config.py
+-rwxrwxr-x   0 michael   (1000) michael   (1000)    10165 2020-06-14 11:50:34.000000 evo-1.9.1/evo/main_ape.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    11137 2019-12-27 11:22:20.000000 evo-1.9.1/evo/main_config.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     6865 2019-12-27 11:22:20.000000 evo-1.9.1/evo/main_evo.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     3631 2019-12-27 11:22:20.000000 evo-1.9.1/evo/main_fig.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     2624 2019-12-21 12:57:46.000000 evo-1.9.1/evo/main_ipython.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    13573 2019-12-27 11:22:20.000000 evo-1.9.1/evo/main_res.py
+-rwxrwxr-x   0 michael   (1000) michael   (1000)    11737 2020-06-14 11:50:34.000000 evo-1.9.1/evo/main_rpe.py
+-rwxrwxr-x   0 michael   (1000) michael   (1000)    22922 2020-06-14 12:55:35.000000 evo-1.9.1/evo/main_traj.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2020-06-14 13:00:37.830043 evo-1.9.1/evo/tools/
+-rw-r--r--   0 michael   (1000) michael   (1000)        0 2019-12-21 12:57:46.000000 evo-1.9.1/evo/tools/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     1285 2019-12-21 12:57:46.000000 evo-1.9.1/evo/tools/compat.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)    16086 2020-06-05 20:47:51.000000 evo-1.9.1/evo/tools/file_interface.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     3808 2019-12-21 12:57:46.000000 evo-1.9.1/evo/tools/log.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     2129 2020-06-05 20:47:51.000000 evo-1.9.1/evo/tools/pandas_bridge.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    26662 2020-05-29 18:10:41.000000 evo-1.9.1/evo/tools/plot.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     4418 2019-12-27 11:22:20.000000 evo-1.9.1/evo/tools/settings.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     6335 2020-06-05 20:47:51.000000 evo-1.9.1/evo/tools/settings_template.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     6418 2020-06-05 20:47:51.000000 evo-1.9.1/evo/tools/tf_cache.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     1322 2019-12-21 12:57:46.000000 evo-1.9.1/evo/tools/user.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)        7 2020-06-14 12:57:45.000000 evo-1.9.1/evo/version
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2020-06-14 13:00:37.830043 evo-1.9.1/evo.egg-info/
+-rw-r--r--   0 michael   (1000) michael   (1000)    14394 2020-06-14 13:00:37.000000 evo-1.9.1/evo.egg-info/PKG-INFO
+-rw-r--r--   0 michael   (1000) michael   (1000)     1051 2020-06-14 13:00:37.000000 evo-1.9.1/evo.egg-info/SOURCES.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)        1 2020-06-14 13:00:37.000000 evo-1.9.1/evo.egg-info/dependency_links.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)      267 2020-06-14 13:00:37.000000 evo-1.9.1/evo.egg-info/entry_points.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)        1 2020-01-29 21:21:45.000000 evo-1.9.1/evo.egg-info/not-zip-safe
+-rw-r--r--   0 michael   (1000) michael   (1000)      105 2020-06-14 13:00:37.000000 evo-1.9.1/evo.egg-info/requires.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)        4 2020-06-14 13:00:37.000000 evo-1.9.1/evo.egg-info/top_level.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)     3950 2019-12-21 12:57:46.000000 evo-1.9.1/fastentrypoints.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      102 2020-06-14 13:00:37.830043 evo-1.9.1/setup.cfg
+-rw-r--r--   0 michael   (1000) michael   (1000)     3637 2020-01-28 22:09:44.000000 evo-1.9.1/setup.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2020-06-14 13:00:37.830043 evo-1.9.1/test/
+-rwxrwxr-x   0 michael   (1000) michael   (1000)     7656 2020-06-03 22:22:20.000000 evo-1.9.1/test/test_file_interface.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     4929 2020-01-04 15:19:32.000000 evo-1.9.1/test/test_filters.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     5950 2020-02-12 23:32:21.000000 evo-1.9.1/test/test_lie_algebra.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     2629 2019-12-21 12:57:46.000000 evo-1.9.1/test/test_result.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     3186 2019-12-21 12:57:46.000000 evo-1.9.1/test/test_sync.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     8279 2020-02-12 23:32:21.000000 evo-1.9.1/test/test_trajectory.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `evo-1.9/LICENSE` & `evo-1.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `evo-1.9/evo.egg-info/SOURCES.txt` & `evo-1.9.1/evo.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -40,18 +40,13 @@
 evo/tools/log.py
 evo/tools/pandas_bridge.py
 evo/tools/plot.py
 evo/tools/settings.py
 evo/tools/settings_template.py
 evo/tools/tf_cache.py
 evo/tools/user.py
-notebooks/metrics.py_API_Documentation.ipynb
-notebooks/metrics_interactive.ipynb
-notebooks/metrics_tutorial.ipynb
-notebooks/pandas_bridge.ipynb
-notebooks/.ipynb_checkpoints/metrics.py_API_Documentation-checkpoint.ipynb
 test/test_file_interface.py
 test/test_filters.py
 test/test_lie_algebra.py
 test/test_result.py
 test/test_sync.py
 test/test_trajectory.py
```

### Comparing `evo-1.9/evo.egg-info/PKG-INFO` & `evo-1.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: evo
-Version: 1.9
+Version: 1.9.1
 Summary: Python package for the evaluation of odometry and SLAM
 Home-page: https://github.com/MichaelGrupp/evo
 Author: Michael Grupp
 Author-email: michael.grupp@tum.de
 License: GPLv3
 Description: # evo
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: evo Version: 1.9 Summary: Python package for the
+Metadata-Version: 2.1 Name: evo Version: 1.9.1 Summary: Python package for the
 evaluation of odometry and SLAM Home-page: https://github.com/MichaelGrupp/evo
 Author: Michael Grupp Author-email: michael.grupp@tum.de License: GPLv3
 Description: # evo ***Python package for the evaluation of odometry and SLAM***
 | Linux / macOS / Windows / ROS | | :---: | | [![Build Status](https://
 dev.azure.com/michl2222/michl2222/_apis/build/status/
 MichaelGrupp.evo?branchName=master)](https://dev.azure.com/michl2222/michl2222/
 _build/latest?definitionId=1&branchName=master) | This package provides
```

### Comparing `evo-1.9/fastentrypoints.py` & `evo-1.9.1/fastentrypoints.py`

 * *Files identical despite different names*

### Comparing `evo-1.9/test/test_result.py` & `evo-1.9.1/test/test_result.py`

 * *Files identical despite different names*

### Comparing `evo-1.9/test/test_trajectory.py` & `evo-1.9.1/test/test_trajectory.py`

 * *Files identical despite different names*

### Comparing `evo-1.9/test/test_filters.py` & `evo-1.9.1/test/test_filters.py`

 * *Files identical despite different names*

### Comparing `evo-1.9/test/test_file_interface.py` & `evo-1.9.1/test/test_file_interface.py`

 * *Files identical despite different names*

### Comparing `evo-1.9/test/test_lie_algebra.py` & `evo-1.9.1/test/test_lie_algebra.py`

 * *Files identical despite different names*

### Comparing `evo-1.9/test/test_sync.py` & `evo-1.9.1/test/test_sync.py`

 * *Files identical despite different names*

### Comparing `evo-1.9/evo/entry_points.py` & `evo-1.9.1/evo/entry_points.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,16 +90,16 @@
     from evo import EvoException, NullHandler
     try:
         main_module.run(args)
     except KeyboardInterrupt:
         sys.exit(1)
     except SystemExit as e:
         sys.exit(e.code)
-    except EvoException as e:
-        logger.error(e.message)
+    except (EvoException, FileNotFoundError) as e:
+        logger.error(str(e))
         sys.exit(1)
     except Exception:
         base_logger = logging.getLogger("evo")
         if len(base_logger.handlers) == 0 or isinstance(
                 base_logger.handlers[0], NullHandler):
             # In case logging couldn't be configured, print & exit directly.
             import traceback
```

### Comparing `evo-1.9/evo/LICENSE` & `evo-1.9.1/evo/LICENSE`

 * *Files identical despite different names*

### Comparing `evo-1.9/evo/main_config.py` & `evo-1.9.1/evo/main_config.py`

 * *Files identical despite different names*

### Comparing `evo-1.9/evo/main_res.py` & `evo-1.9.1/evo/main_res.py`

 * *Files identical despite different names*

### Comparing `evo-1.9/evo/__init__.py` & `evo-1.9.1/evo/__init__.py`

 * *Files identical despite different names*

### Comparing `evo-1.9/evo/main_evo.py` & `evo-1.9.1/evo/main_evo.py`

 * *Files identical despite different names*

### Comparing `evo-1.9/evo/ipython_config.py` & `evo-1.9.1/evo/ipython_config.py`

 * *Files identical despite different names*

### Comparing `evo-1.9/evo/common_ape_rpe.py` & `evo-1.9.1/evo/common_ape_rpe.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,15 +87,15 @@
     elif args.delta_unit == "r":
         delta_unit = Unit.radians
     elif args.delta_unit == "m":
         delta_unit = Unit.meters
     return delta_unit
 
 
-def plot(args, result, traj_ref, traj_est):
+def plot(args, result, traj_ref, traj_est, traj_ref_full=None):
     from evo.tools import plot
     from evo.tools.settings import SETTINGS
 
     import matplotlib.pyplot as plt
     import numpy as np
 
     logger.debug(SEP)
@@ -119,15 +119,16 @@
 
     # Plot the values color-mapped onto the trajectory.
     fig2 = plt.figure(figsize=SETTINGS.plot_figsize)
     ax = plot.prepare_axis(fig2, plot_mode)
     if args.ros_map_yaml:
         plot.ros_map(ax, args.ros_map_yaml, plot_mode)
 
-    plot.traj(ax, plot_mode, traj_ref, style=SETTINGS.plot_reference_linestyle,
+    plot.traj(ax, plot_mode, traj_ref_full if traj_ref_full else traj_ref,
+              style=SETTINGS.plot_reference_linestyle,
               color=SETTINGS.plot_reference_color, label='reference',
               alpha=SETTINGS.plot_reference_alpha)
     plot.draw_coordinate_axes(ax, traj_ref, plot_mode,
                               SETTINGS.plot_axis_marker_scale)
 
     if args.plot_colormap_min is None:
         args.plot_colormap_min = result.stats["min"]
```

### Comparing `evo-1.9/evo/main_rpe.py` & `evo-1.9.1/evo/main_rpe.py`

 * *Files 1% similar despite different names*

```diff
@@ -273,17 +273,16 @@
         correct_scale=args.correct_scale,
         align_origin=args.align_origin,
         ref_name=ref_name,
         est_name=est_name,
     )
 
     if args.plot or args.save_plot or args.serialize_plot:
-        common.plot(args, result,
-                    traj_ref_full if args.plot_full_ref else traj_ref,
-                    result.trajectories[est_name])
+        common.plot(args, result, traj_ref, result.trajectories[est_name],
+                    traj_ref_full=traj_ref_full)
 
     if args.save_results:
         logger.debug(SEP)
         if not SETTINGS.save_traj_in_zip:
             del result.trajectories[ref_name]
             del result.trajectories[est_name]
         file_interface.save_res_file(args.save_results, result,
```

### Comparing `evo-1.9/evo/main_traj.py` & `evo-1.9.1/evo/main_traj.py`

 * *Files 1% similar despite different names*

```diff
@@ -201,14 +201,15 @@
     elif args.subcommand == "bag":
         if not (args.topics or args.all_topics):
             die("No topics used - specify topics or set --all_topics.")
         if not os.path.exists(args.bag):
             raise file_interface.FileInterfaceException(
                 "File doesn't exist: {}".format(args.bag))
         import rosbag
+        logger.debug("Opening bag file " + args.bag)
         bag = rosbag.Bag(args.bag)
         try:
             if args.all_topics:
                 topics = args.topics + file_interface.get_supported_topics(bag)
                 if args.ref in topics:
                     topics.remove(args.ref)
                 if len(topics) == 0:
```

### Comparing `evo-1.9/evo/main_ipython.py` & `evo-1.9.1/evo/main_ipython.py`

 * *Files identical despite different names*

### Comparing `evo-1.9/evo/main_fig.py` & `evo-1.9.1/evo/main_fig.py`

 * *Files identical despite different names*

### Comparing `evo-1.9/evo/core/geometry.py` & `evo-1.9.1/evo/core/geometry.py`

 * *Files identical despite different names*

### Comparing `evo-1.9/evo/core/trajectory.py` & `evo-1.9.1/evo/core/trajectory.py`

 * *Files identical despite different names*

### Comparing `evo-1.9/evo/core/sync.py` & `evo-1.9.1/evo/core/sync.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,15 +71,15 @@
     if not isinstance(traj_1, PoseTrajectory3D) \
         or not isinstance(traj_2, PoseTrajectory3D):
         raise SyncException("trajectories must be PoseTrajectory3D objects")
 
     snd_longer = len(traj_2.timestamps) > len(traj_1.timestamps)
     traj_long = copy.deepcopy(traj_2) if snd_longer else copy.deepcopy(traj_1)
     traj_short = copy.deepcopy(traj_1) if snd_longer else copy.deepcopy(traj_2)
-    max_pairs = len(traj_long.timestamps)
+    max_pairs = len(traj_short.timestamps)
 
     # First, match the timestamps of the shorter trajectory to the longer one.
     matching_indices = matching_time_indices(
         traj_short.timestamps, traj_long.timestamps, max_diff,
         offset_2 if snd_longer else -offset_2)
     traj_long.reduce_to_ids(matching_indices)
```

### Comparing `evo-1.9/evo/core/metrics.py` & `evo-1.9.1/evo/core/metrics.py`

 * *Files identical despite different names*

### Comparing `evo-1.9/evo/core/lie_algebra.py` & `evo-1.9.1/evo/core/lie_algebra.py`

 * *Files identical despite different names*

### Comparing `evo-1.9/evo/core/filters.py` & `evo-1.9.1/evo/core/filters.py`

 * *Files identical despite different names*

### Comparing `evo-1.9/evo/core/result.py` & `evo-1.9.1/evo/core/result.py`

 * *Files identical despite different names*

### Comparing `evo-1.9/evo/core/transformations.py` & `evo-1.9.1/evo/core/transformations.py`

 * *Files identical despite different names*

### Comparing `evo-1.9/evo/main_ape.py` & `evo-1.9.1/evo/main_ape.py`

 * *Files 4% similar despite different names*

```diff
@@ -239,17 +239,16 @@
         correct_scale=args.correct_scale,
         align_origin=args.align_origin,
         ref_name=ref_name,
         est_name=est_name,
     )
 
     if args.plot or args.save_plot or args.serialize_plot:
-        common.plot(args, result,
-                    traj_ref_full if args.plot_full_ref else traj_ref,
-                    result.trajectories[est_name])
+        common.plot(args, result, traj_ref, result.trajectories[est_name],
+                    traj_ref_full=traj_ref_full)
 
     if args.save_results:
         logger.debug(SEP)
         if not SETTINGS.save_traj_in_zip:
             del result.trajectories[ref_name]
             del result.trajectories[est_name]
         file_interface.save_res_file(args.save_results, result,
```

### Comparing `evo-1.9/evo/tools/settings.py` & `evo-1.9.1/evo/tools/settings.py`

 * *Files identical despite different names*

### Comparing `evo-1.9/evo/tools/compat.py` & `evo-1.9.1/evo/tools/compat.py`

 * *Files identical despite different names*

### Comparing `evo-1.9/evo/tools/log.py` & `evo-1.9.1/evo/tools/log.py`

 * *Files identical despite different names*

### Comparing `evo-1.9/evo/tools/tf_cache.py` & `evo-1.9.1/evo/tools/tf_cache.py`

 * *Files identical despite different names*

### Comparing `evo-1.9/evo/tools/pandas_bridge.py` & `evo-1.9.1/evo/tools/pandas_bridge.py`

 * *Files identical despite different names*

### Comparing `evo-1.9/evo/tools/plot.py` & `evo-1.9.1/evo/tools/plot.py`

 * *Files identical despite different names*

### Comparing `evo-1.9/evo/tools/settings_template.py` & `evo-1.9.1/evo/tools/settings_template.py`

 * *Files identical despite different names*

### Comparing `evo-1.9/evo/tools/user.py` & `evo-1.9.1/evo/tools/user.py`

 * *Files identical despite different names*

### Comparing `evo-1.9/evo/tools/file_interface.py` & `evo-1.9.1/evo/tools/file_interface.py`

 * *Files identical despite different names*

### Comparing `evo-1.9/PKG-INFO` & `evo-1.9.1/evo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: evo
-Version: 1.9
+Version: 1.9.1
 Summary: Python package for the evaluation of odometry and SLAM
 Home-page: https://github.com/MichaelGrupp/evo
 Author: Michael Grupp
 Author-email: michael.grupp@tum.de
 License: GPLv3
 Description: # evo
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: evo Version: 1.9 Summary: Python package for the
+Metadata-Version: 2.1 Name: evo Version: 1.9.1 Summary: Python package for the
 evaluation of odometry and SLAM Home-page: https://github.com/MichaelGrupp/evo
 Author: Michael Grupp Author-email: michael.grupp@tum.de License: GPLv3
 Description: # evo ***Python package for the evaluation of odometry and SLAM***
 | Linux / macOS / Windows / ROS | | :---: | | [![Build Status](https://
 dev.azure.com/michl2222/michl2222/_apis/build/status/
 MichaelGrupp.evo?branchName=master)](https://dev.azure.com/michl2222/michl2222/
 _build/latest?definitionId=1&branchName=master) | This package provides
```

### Comparing `evo-1.9/setup.py` & `evo-1.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `evo-1.9/README.md` & `evo-1.9.1/README.md`

 * *Files identical despite different names*

