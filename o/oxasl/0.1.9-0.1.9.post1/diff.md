# Comparing `tmp/oxasl-0.1.9.tar.gz` & `tmp/oxasl-0.1.9.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/oxasl-0.1.9.tar", last modified: Mon May  4 11:10:26 2020, max compression
+gzip compressed data, was "dist/oxasl-0.1.9.post1.tar", last modified: Mon May  4 13:32:55 2020, max compression
```

## Comparing `oxasl-0.1.9.tar` & `oxasl-0.1.9.post1.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 ibmeuser  (1000) ibmeuser  (1000)        0 2020-05-04 11:10:26.000000 oxasl-0.1.9/
--rw-r--r--   0 ibmeuser  (1000) ibmeuser  (1000)     6243 2019-09-04 08:25:34.000000 oxasl-0.1.9/LICENSE
--rw-r--r--   0 ibmeuser  (1000) ibmeuser  (1000)       43 2019-10-02 14:00:31.000000 oxasl-0.1.9/MANIFEST.in
--rw-r--r--   0 ibmeuser  (1000) ibmeuser  (1000)      932 2020-05-04 11:10:26.000000 oxasl-0.1.9/PKG-INFO
--rw-r--r--   0 ibmeuser  (1000) ibmeuser  (1000)      118 2019-09-04 08:25:34.000000 oxasl-0.1.9/README.md
-drwxr-xr-x   0 ibmeuser  (1000) ibmeuser  (1000)        0 2020-05-04 11:10:26.000000 oxasl-0.1.9/oxasl/
--rw-r--r--   0 ibmeuser  (1000) ibmeuser  (1000)     4714 2019-09-04 08:24:55.000000 oxasl-0.1.9/oxasl/__init__.py
--rw-r--r--   0 ibmeuser  (1000) ibmeuser  (1000)       70 2020-05-04 11:10:26.000000 oxasl-0.1.9/oxasl/_version.py
--rw-r--r--   0 ibmeuser  (1000) ibmeuser  (1000)    29028 2020-05-04 10:50:06.000000 oxasl-0.1.9/oxasl/basil.py
--rw-r--r--   0 ibmeuser  (1000) ibmeuser  (1000)    20599 2019-09-04 08:24:55.000000 oxasl-0.1.9/oxasl/basil2.py
--rw-r--r--   0 ibmeuser  (1000) ibmeuser  (1000)      579 2019-09-04 08:24:55.000000 oxasl-0.1.9/oxasl/brain.py
--rwxr-xr-x   0 ibmeuser  (1000) ibmeuser  (1000)    32013 2020-04-02 15:54:16.000000 oxasl-0.1.9/oxasl/calib.py
--rw-r--r--   0 ibmeuser  (1000) ibmeuser  (1000)    27709 2019-11-12 10:15:04.000000 oxasl-0.1.9/oxasl/corrections.py
--rw-r--r--   0 ibmeuser  (1000) ibmeuser  (1000)     5824 2019-09-04 08:24:55.000000 oxasl-0.1.9/oxasl/epi_reg.py
-drwxr-xr-x   0 ibmeuser  (1000) ibmeuser  (1000)        0 2020-05-04 11:10:26.000000 oxasl-0.1.9/oxasl/gui/
--rw-r--r--   0 ibmeuser  (1000) ibmeuser  (1000)     3555 2019-10-02 14:00:31.000000 oxasl-0.1.9/oxasl/gui/__init__.py
--rw-r--r--   0 ibmeuser  (1000) ibmeuser  (1000)     3910 2019-09-04 08:26:35.000000 oxasl-0.1.9/oxasl/gui/analysis_tab.py
--rw-r--r--   0 ibmeuser  (1000) ibmeuser  (1000)    13308 2019-04-29 13:32:32.000000 oxasl-0.1.9/oxasl/gui/banner.png
--rw-r--r--   0 ibmeuser  (1000) ibmeuser  (1000)     5532 2019-09-04 08:26:35.000000 oxasl-0.1.9/oxasl/gui/calib_tab.py
--rw-r--r--   0 ibmeuser  (1000) ibmeuser  (1000)     3984 2019-09-04 08:26:35.000000 oxasl-0.1.9/oxasl/gui/dist_corr_tab.py
--rw-r--r--   0 ibmeuser  (1000) ibmeuser  (1000)     2020 2019-10-02 14:00:31.000000 oxasl-0.1.9/oxasl/gui/icon.png
--rw-r--r--   0 ibmeuser  (1000) ibmeuser  (1000)    11088 2019-09-04 08:26:35.000000 oxasl-0.1.9/oxasl/gui/input_tab.py
--rw-r--r--   0 ibmeuser  (1000) ibmeuser  (1000)     4652 2019-09-04 08:26:35.000000 oxasl-0.1.9/oxasl/gui/run_box.py
--rw-r--r--   0 ibmeuser  (1000) ibmeuser  (1000)     2837 2019-09-04 08:26:35.000000 oxasl-0.1.9/oxasl/gui/structure_tab.py
--rw-r--r--   0 ibmeuser  (1000) ibmeuser  (1000)    19555 2019-09-04 08:26:35.000000 oxasl-0.1.9/oxasl/gui/widgets.py
--rwxr-xr-x   0 ibmeuser  (1000) ibmeuser  (1000)    35918 2020-05-04 10:18:13.000000 oxasl-0.1.9/oxasl/image.py
--rw-r--r--   0 ibmeuser  (1000) ibmeuser  (1000)     4739 2019-10-02 14:00:31.000000 oxasl-0.1.9/oxasl/mask.py
--rw-r--r--   0 ibmeuser  (1000) ibmeuser  (1000)     8236 2019-09-04 08:27:46.000000 oxasl-0.1.9/oxasl/options.py
--rwxr-xr-x   0 ibmeuser  (1000) ibmeuser  (1000)    25086 2020-05-04 10:53:52.000000 oxasl-0.1.9/oxasl/oxford_asl.py
--rw-r--r--   0 ibmeuser  (1000) ibmeuser  (1000)      693 2019-10-02 14:00:31.000000 oxasl-0.1.9/oxasl/plugin.py
--rw-r--r--   0 ibmeuser  (1000) ibmeuser  (1000)     4009 2019-09-04 08:24:55.000000 oxasl-0.1.9/oxasl/preproc.py
--rw-r--r--   0 ibmeuser  (1000) ibmeuser  (1000)     2239 2019-10-02 14:00:31.000000 oxasl-0.1.9/oxasl/quasil.py
--rw-r--r--   0 ibmeuser  (1000) ibmeuser  (1000)    19773 2019-09-26 08:34:08.000000 oxasl-0.1.9/oxasl/reg.py
--rw-r--r--   0 ibmeuser  (1000) ibmeuser  (1000)    17350 2019-12-12 13:05:40.000000 oxasl-0.1.9/oxasl/reporting.py
--rw-r--r--   0 ibmeuser  (1000) ibmeuser  (1000)     7218 2019-11-12 10:15:04.000000 oxasl-0.1.9/oxasl/struc.py
-drwxr-xr-x   0 ibmeuser  (1000) ibmeuser  (1000)        0 2020-05-04 11:10:26.000000 oxasl-0.1.9/oxasl/test/
--rw-r--r--   0 ibmeuser  (1000) ibmeuser  (1000)        0 2019-09-04 08:26:40.000000 oxasl-0.1.9/oxasl/test/__init__.py
--rw-r--r--   0 ibmeuser  (1000) ibmeuser  (1000)    13141 2019-09-04 08:26:40.000000 oxasl-0.1.9/oxasl/test/test_basil.py
--rw-r--r--   0 ibmeuser  (1000) ibmeuser  (1000)    19985 2019-10-02 14:00:32.000000 oxasl-0.1.9/oxasl/test/test_calib.py
--rw-r--r--   0 ibmeuser  (1000) ibmeuser  (1000)    24735 2019-10-02 14:00:32.000000 oxasl-0.1.9/oxasl/test/test_image.py
--rw-r--r--   0 ibmeuser  (1000) ibmeuser  (1000)     3399 2019-09-04 08:26:40.000000 oxasl-0.1.9/oxasl/test/test_preproc.py
--rw-r--r--   0 ibmeuser  (1000) ibmeuser  (1000)     1863 2019-09-04 08:26:40.000000 oxasl-0.1.9/oxasl/test/test_reg.py
--rw-r--r--   0 ibmeuser  (1000) ibmeuser  (1000)    12803 2019-10-02 14:00:32.000000 oxasl-0.1.9/oxasl/test/test_workspace.py
--rw-r--r--   0 ibmeuser  (1000) ibmeuser  (1000)      830 2019-09-04 08:24:55.000000 oxasl-0.1.9/oxasl/utils.py
--rw-r--r--   0 ibmeuser  (1000) ibmeuser  (1000)    13616 2019-12-12 12:41:42.000000 oxasl-0.1.9/oxasl/workspace.py
-drwxr-xr-x   0 ibmeuser  (1000) ibmeuser  (1000)        0 2020-05-04 11:10:26.000000 oxasl-0.1.9/oxasl/wrappers/
--rw-r--r--   0 ibmeuser  (1000) ibmeuser  (1000)      270 2019-09-04 08:26:48.000000 oxasl-0.1.9/oxasl/wrappers/__init__.py
--rw-r--r--   0 ibmeuser  (1000) ibmeuser  (1000)      932 2019-09-04 08:26:48.000000 oxasl-0.1.9/oxasl/wrappers/avscale.py
--rw-r--r--   0 ibmeuser  (1000) ibmeuser  (1000)     1457 2019-09-04 08:26:48.000000 oxasl-0.1.9/oxasl/wrappers/epi_reg.py
--rw-r--r--   0 ibmeuser  (1000) ibmeuser  (1000)     6749 2019-10-02 14:00:32.000000 oxasl-0.1.9/oxasl/wrappers/fabber.py
--rw-r--r--   0 ibmeuser  (1000) ibmeuser  (1000)     1371 2019-09-04 08:26:48.000000 oxasl-0.1.9/oxasl/wrappers/fnirt_extra.py
-drwxr-xr-x   0 ibmeuser  (1000) ibmeuser  (1000)        0 2020-05-04 11:10:26.000000 oxasl-0.1.9/oxasl.egg-info/
--rw-r--r--   0 ibmeuser  (1000) ibmeuser  (1000)      932 2020-05-04 11:10:26.000000 oxasl-0.1.9/oxasl.egg-info/PKG-INFO
--rw-r--r--   0 ibmeuser  (1000) ibmeuser  (1000)     1103 2020-05-04 11:10:26.000000 oxasl-0.1.9/oxasl.egg-info/SOURCES.txt
--rw-r--r--   0 ibmeuser  (1000) ibmeuser  (1000)        1 2020-05-04 11:10:26.000000 oxasl-0.1.9/oxasl.egg-info/dependency_links.txt
--rw-r--r--   0 ibmeuser  (1000) ibmeuser  (1000)      244 2020-05-04 11:10:26.000000 oxasl-0.1.9/oxasl.egg-info/entry_points.txt
--rw-r--r--   0 ibmeuser  (1000) ibmeuser  (1000)       62 2020-05-04 11:10:26.000000 oxasl-0.1.9/oxasl.egg-info/requires.txt
--rw-r--r--   0 ibmeuser  (1000) ibmeuser  (1000)        6 2020-05-04 11:10:26.000000 oxasl-0.1.9/oxasl.egg-info/top_level.txt
--rw-r--r--   0 ibmeuser  (1000) ibmeuser  (1000)       62 2019-10-02 14:00:32.000000 oxasl-0.1.9/requirements.txt
--rw-r--r--   0 ibmeuser  (1000) ibmeuser  (1000)       38 2020-05-04 11:10:26.000000 oxasl-0.1.9/setup.cfg
--rw-r--r--   0 ibmeuser  (1000) ibmeuser  (1000)     4796 2019-10-02 14:00:32.000000 oxasl-0.1.9/setup.py
+drwxr-xr-x   0 ibmeuser  (1000) ibmeuser  (1000)        0 2020-05-04 13:32:55.000000 oxasl-0.1.9.post1/
+-rw-r--r--   0 ibmeuser  (1000) ibmeuser  (1000)     6243 2019-09-04 08:25:34.000000 oxasl-0.1.9.post1/LICENSE
+-rw-r--r--   0 ibmeuser  (1000) ibmeuser  (1000)       43 2019-10-02 14:00:31.000000 oxasl-0.1.9.post1/MANIFEST.in
+-rw-r--r--   0 ibmeuser  (1000) ibmeuser  (1000)      938 2020-05-04 13:32:55.000000 oxasl-0.1.9.post1/PKG-INFO
+-rw-r--r--   0 ibmeuser  (1000) ibmeuser  (1000)      118 2019-09-04 08:25:34.000000 oxasl-0.1.9.post1/README.md
+drwxr-xr-x   0 ibmeuser  (1000) ibmeuser  (1000)        0 2020-05-04 13:32:55.000000 oxasl-0.1.9.post1/oxasl/
+-rw-r--r--   0 ibmeuser  (1000) ibmeuser  (1000)     4714 2019-09-04 08:24:55.000000 oxasl-0.1.9.post1/oxasl/__init__.py
+-rw-r--r--   0 ibmeuser  (1000) ibmeuser  (1000)       76 2020-05-04 13:32:55.000000 oxasl-0.1.9.post1/oxasl/_version.py
+-rw-r--r--   0 ibmeuser  (1000) ibmeuser  (1000)    29028 2020-05-04 10:50:06.000000 oxasl-0.1.9.post1/oxasl/basil.py
+-rw-r--r--   0 ibmeuser  (1000) ibmeuser  (1000)    20599 2019-09-04 08:24:55.000000 oxasl-0.1.9.post1/oxasl/basil2.py
+-rw-r--r--   0 ibmeuser  (1000) ibmeuser  (1000)      579 2019-09-04 08:24:55.000000 oxasl-0.1.9.post1/oxasl/brain.py
+-rwxr-xr-x   0 ibmeuser  (1000) ibmeuser  (1000)    32013 2020-04-02 15:54:16.000000 oxasl-0.1.9.post1/oxasl/calib.py
+-rw-r--r--   0 ibmeuser  (1000) ibmeuser  (1000)    27709 2019-11-12 10:15:04.000000 oxasl-0.1.9.post1/oxasl/corrections.py
+-rw-r--r--   0 ibmeuser  (1000) ibmeuser  (1000)     5824 2019-09-04 08:24:55.000000 oxasl-0.1.9.post1/oxasl/epi_reg.py
+drwxr-xr-x   0 ibmeuser  (1000) ibmeuser  (1000)        0 2020-05-04 13:32:55.000000 oxasl-0.1.9.post1/oxasl/gui/
+-rw-r--r--   0 ibmeuser  (1000) ibmeuser  (1000)     3555 2019-10-02 14:00:31.000000 oxasl-0.1.9.post1/oxasl/gui/__init__.py
+-rw-r--r--   0 ibmeuser  (1000) ibmeuser  (1000)     3910 2019-09-04 08:26:35.000000 oxasl-0.1.9.post1/oxasl/gui/analysis_tab.py
+-rw-r--r--   0 ibmeuser  (1000) ibmeuser  (1000)    13308 2019-04-29 13:32:32.000000 oxasl-0.1.9.post1/oxasl/gui/banner.png
+-rw-r--r--   0 ibmeuser  (1000) ibmeuser  (1000)     5532 2019-09-04 08:26:35.000000 oxasl-0.1.9.post1/oxasl/gui/calib_tab.py
+-rw-r--r--   0 ibmeuser  (1000) ibmeuser  (1000)     3984 2019-09-04 08:26:35.000000 oxasl-0.1.9.post1/oxasl/gui/dist_corr_tab.py
+-rw-r--r--   0 ibmeuser  (1000) ibmeuser  (1000)     2020 2019-10-02 14:00:31.000000 oxasl-0.1.9.post1/oxasl/gui/icon.png
+-rw-r--r--   0 ibmeuser  (1000) ibmeuser  (1000)    11088 2019-09-04 08:26:35.000000 oxasl-0.1.9.post1/oxasl/gui/input_tab.py
+-rw-r--r--   0 ibmeuser  (1000) ibmeuser  (1000)     4652 2019-09-04 08:26:35.000000 oxasl-0.1.9.post1/oxasl/gui/run_box.py
+-rw-r--r--   0 ibmeuser  (1000) ibmeuser  (1000)     2837 2019-09-04 08:26:35.000000 oxasl-0.1.9.post1/oxasl/gui/structure_tab.py
+-rw-r--r--   0 ibmeuser  (1000) ibmeuser  (1000)    19555 2019-09-04 08:26:35.000000 oxasl-0.1.9.post1/oxasl/gui/widgets.py
+-rwxr-xr-x   0 ibmeuser  (1000) ibmeuser  (1000)    35918 2020-05-04 10:18:13.000000 oxasl-0.1.9.post1/oxasl/image.py
+-rw-r--r--   0 ibmeuser  (1000) ibmeuser  (1000)     4739 2019-10-02 14:00:31.000000 oxasl-0.1.9.post1/oxasl/mask.py
+-rw-r--r--   0 ibmeuser  (1000) ibmeuser  (1000)     8236 2019-09-04 08:27:46.000000 oxasl-0.1.9.post1/oxasl/options.py
+-rwxr-xr-x   0 ibmeuser  (1000) ibmeuser  (1000)    25303 2020-05-04 13:24:08.000000 oxasl-0.1.9.post1/oxasl/oxford_asl.py
+-rw-r--r--   0 ibmeuser  (1000) ibmeuser  (1000)      693 2019-10-02 14:00:31.000000 oxasl-0.1.9.post1/oxasl/plugin.py
+-rw-r--r--   0 ibmeuser  (1000) ibmeuser  (1000)     4009 2019-09-04 08:24:55.000000 oxasl-0.1.9.post1/oxasl/preproc.py
+-rw-r--r--   0 ibmeuser  (1000) ibmeuser  (1000)     2239 2019-10-02 14:00:31.000000 oxasl-0.1.9.post1/oxasl/quasil.py
+-rw-r--r--   0 ibmeuser  (1000) ibmeuser  (1000)    19773 2019-09-26 08:34:08.000000 oxasl-0.1.9.post1/oxasl/reg.py
+-rw-r--r--   0 ibmeuser  (1000) ibmeuser  (1000)    17350 2019-12-12 13:05:40.000000 oxasl-0.1.9.post1/oxasl/reporting.py
+-rw-r--r--   0 ibmeuser  (1000) ibmeuser  (1000)     7218 2019-11-12 10:15:04.000000 oxasl-0.1.9.post1/oxasl/struc.py
+drwxr-xr-x   0 ibmeuser  (1000) ibmeuser  (1000)        0 2020-05-04 13:32:55.000000 oxasl-0.1.9.post1/oxasl/test/
+-rw-r--r--   0 ibmeuser  (1000) ibmeuser  (1000)        0 2019-09-04 08:26:40.000000 oxasl-0.1.9.post1/oxasl/test/__init__.py
+-rw-r--r--   0 ibmeuser  (1000) ibmeuser  (1000)    13141 2019-09-04 08:26:40.000000 oxasl-0.1.9.post1/oxasl/test/test_basil.py
+-rw-r--r--   0 ibmeuser  (1000) ibmeuser  (1000)    19985 2019-10-02 14:00:32.000000 oxasl-0.1.9.post1/oxasl/test/test_calib.py
+-rw-r--r--   0 ibmeuser  (1000) ibmeuser  (1000)    24735 2019-10-02 14:00:32.000000 oxasl-0.1.9.post1/oxasl/test/test_image.py
+-rw-r--r--   0 ibmeuser  (1000) ibmeuser  (1000)     3399 2019-09-04 08:26:40.000000 oxasl-0.1.9.post1/oxasl/test/test_preproc.py
+-rw-r--r--   0 ibmeuser  (1000) ibmeuser  (1000)     1863 2019-09-04 08:26:40.000000 oxasl-0.1.9.post1/oxasl/test/test_reg.py
+-rw-r--r--   0 ibmeuser  (1000) ibmeuser  (1000)    12803 2019-10-02 14:00:32.000000 oxasl-0.1.9.post1/oxasl/test/test_workspace.py
+-rw-r--r--   0 ibmeuser  (1000) ibmeuser  (1000)      830 2019-09-04 08:24:55.000000 oxasl-0.1.9.post1/oxasl/utils.py
+-rw-r--r--   0 ibmeuser  (1000) ibmeuser  (1000)    13616 2019-12-12 12:41:42.000000 oxasl-0.1.9.post1/oxasl/workspace.py
+drwxr-xr-x   0 ibmeuser  (1000) ibmeuser  (1000)        0 2020-05-04 13:32:55.000000 oxasl-0.1.9.post1/oxasl/wrappers/
+-rw-r--r--   0 ibmeuser  (1000) ibmeuser  (1000)      270 2019-09-04 08:26:48.000000 oxasl-0.1.9.post1/oxasl/wrappers/__init__.py
+-rw-r--r--   0 ibmeuser  (1000) ibmeuser  (1000)      932 2019-09-04 08:26:48.000000 oxasl-0.1.9.post1/oxasl/wrappers/avscale.py
+-rw-r--r--   0 ibmeuser  (1000) ibmeuser  (1000)     1457 2019-09-04 08:26:48.000000 oxasl-0.1.9.post1/oxasl/wrappers/epi_reg.py
+-rw-r--r--   0 ibmeuser  (1000) ibmeuser  (1000)     6749 2019-10-02 14:00:32.000000 oxasl-0.1.9.post1/oxasl/wrappers/fabber.py
+-rw-r--r--   0 ibmeuser  (1000) ibmeuser  (1000)     1371 2019-09-04 08:26:48.000000 oxasl-0.1.9.post1/oxasl/wrappers/fnirt_extra.py
+drwxr-xr-x   0 ibmeuser  (1000) ibmeuser  (1000)        0 2020-05-04 13:32:55.000000 oxasl-0.1.9.post1/oxasl.egg-info/
+-rw-r--r--   0 ibmeuser  (1000) ibmeuser  (1000)      938 2020-05-04 13:32:55.000000 oxasl-0.1.9.post1/oxasl.egg-info/PKG-INFO
+-rw-r--r--   0 ibmeuser  (1000) ibmeuser  (1000)     1103 2020-05-04 13:32:55.000000 oxasl-0.1.9.post1/oxasl.egg-info/SOURCES.txt
+-rw-r--r--   0 ibmeuser  (1000) ibmeuser  (1000)        1 2020-05-04 13:32:55.000000 oxasl-0.1.9.post1/oxasl.egg-info/dependency_links.txt
+-rw-r--r--   0 ibmeuser  (1000) ibmeuser  (1000)      244 2020-05-04 13:32:55.000000 oxasl-0.1.9.post1/oxasl.egg-info/entry_points.txt
+-rw-r--r--   0 ibmeuser  (1000) ibmeuser  (1000)       62 2020-05-04 13:32:55.000000 oxasl-0.1.9.post1/oxasl.egg-info/requires.txt
+-rw-r--r--   0 ibmeuser  (1000) ibmeuser  (1000)        6 2020-05-04 13:32:55.000000 oxasl-0.1.9.post1/oxasl.egg-info/top_level.txt
+-rw-r--r--   0 ibmeuser  (1000) ibmeuser  (1000)       62 2019-10-02 14:00:32.000000 oxasl-0.1.9.post1/requirements.txt
+-rw-r--r--   0 ibmeuser  (1000) ibmeuser  (1000)       38 2020-05-04 13:32:55.000000 oxasl-0.1.9.post1/setup.cfg
+-rw-r--r--   0 ibmeuser  (1000) ibmeuser  (1000)     4796 2019-10-02 14:00:32.000000 oxasl-0.1.9.post1/setup.py
```

### Comparing `oxasl-0.1.9/LICENSE` & `oxasl-0.1.9.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `oxasl-0.1.9/PKG-INFO` & `oxasl-0.1.9.post1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oxasl
-Version: 0.1.9
+Version: 0.1.9.post1
 Summary: Python library for manipulating and modelling ASL data
 Home-page: https://oxasl.readthedocs.io/
 Author: Martin Craig
 Author-email: martin.craig@eng.ox.ac.uk
 License: License granted by University of Oxford for use by academics carrying out research and not for use by consumers or commercial businesses. See LICENSE file for more details
 Description: OXASL - FSL based ASL pipeline
         ==============================
```

### Comparing `oxasl-0.1.9/oxasl/__init__.py` & `oxasl-0.1.9.post1/oxasl/__init__.py`

 * *Files identical despite different names*

### Comparing `oxasl-0.1.9/oxasl/basil.py` & `oxasl-0.1.9.post1/oxasl/basil.py`

 * *Files identical despite different names*

### Comparing `oxasl-0.1.9/oxasl/basil2.py` & `oxasl-0.1.9.post1/oxasl/basil2.py`

 * *Files identical despite different names*

### Comparing `oxasl-0.1.9/oxasl/brain.py` & `oxasl-0.1.9.post1/oxasl/brain.py`

 * *Files identical despite different names*

### Comparing `oxasl-0.1.9/oxasl/calib.py` & `oxasl-0.1.9.post1/oxasl/calib.py`

 * *Files identical despite different names*

### Comparing `oxasl-0.1.9/oxasl/corrections.py` & `oxasl-0.1.9.post1/oxasl/corrections.py`

 * *Files identical despite different names*

### Comparing `oxasl-0.1.9/oxasl/epi_reg.py` & `oxasl-0.1.9.post1/oxasl/epi_reg.py`

 * *Files identical despite different names*

### Comparing `oxasl-0.1.9/oxasl/gui/__init__.py` & `oxasl-0.1.9.post1/oxasl/gui/__init__.py`

 * *Files identical despite different names*

### Comparing `oxasl-0.1.9/oxasl/gui/analysis_tab.py` & `oxasl-0.1.9.post1/oxasl/gui/analysis_tab.py`

 * *Files identical despite different names*

### Comparing `oxasl-0.1.9/oxasl/gui/banner.png` & `oxasl-0.1.9.post1/oxasl/gui/banner.png`

 * *Files identical despite different names*

### Comparing `oxasl-0.1.9/oxasl/gui/calib_tab.py` & `oxasl-0.1.9.post1/oxasl/gui/calib_tab.py`

 * *Files identical despite different names*

### Comparing `oxasl-0.1.9/oxasl/gui/dist_corr_tab.py` & `oxasl-0.1.9.post1/oxasl/gui/dist_corr_tab.py`

 * *Files identical despite different names*

### Comparing `oxasl-0.1.9/oxasl/gui/icon.png` & `oxasl-0.1.9.post1/oxasl/gui/icon.png`

 * *Files identical despite different names*

### Comparing `oxasl-0.1.9/oxasl/gui/input_tab.py` & `oxasl-0.1.9.post1/oxasl/gui/input_tab.py`

 * *Files identical despite different names*

### Comparing `oxasl-0.1.9/oxasl/gui/run_box.py` & `oxasl-0.1.9.post1/oxasl/gui/run_box.py`

 * *Files identical despite different names*

### Comparing `oxasl-0.1.9/oxasl/gui/structure_tab.py` & `oxasl-0.1.9.post1/oxasl/gui/structure_tab.py`

 * *Files identical despite different names*

### Comparing `oxasl-0.1.9/oxasl/gui/widgets.py` & `oxasl-0.1.9.post1/oxasl/gui/widgets.py`

 * *Files identical despite different names*

### Comparing `oxasl-0.1.9/oxasl/image.py` & `oxasl-0.1.9.post1/oxasl/image.py`

 * *Files identical despite different names*

### Comparing `oxasl-0.1.9/oxasl/mask.py` & `oxasl-0.1.9.post1/oxasl/mask.py`

 * *Files identical despite different names*

### Comparing `oxasl-0.1.9/oxasl/options.py` & `oxasl-0.1.9.post1/oxasl/options.py`

 * *Files identical despite different names*

### Comparing `oxasl-0.1.9/oxasl/oxford_asl.py` & `oxasl-0.1.9.post1/oxasl/oxford_asl.py`

 * *Files 2% similar despite different names*

```diff
@@ -421,14 +421,20 @@
     :param wsp: Workspace object. Output will be placed in a sub workspace named ``native``
     :param basil_wsp: Workspace in which Basil modelling has been run. The ``finalstep``
                       attribute is expected to point to the final output workspace
     """
     if not wsp.output_native: return
 
     wsp.sub("native")
+
+    # Output the differenced data averaged across repeats for kinetic curve comparison
+    # with the model
+    wsp.native.diffdata_mean = wsp.asldata.diff().mean_across_repeats()
+
+    # Output model fitting results
     prefixes = ["", "mean"]
     if wsp.output_stddev:
         prefixes.append("std")
     if wsp.output_var:
         prefixes.append("var")
     for fabber_name, oxasl_output in OUTPUT_ITEMS.items():
         for prefix in prefixes:
```

### Comparing `oxasl-0.1.9/oxasl/plugin.py` & `oxasl-0.1.9.post1/oxasl/plugin.py`

 * *Files identical despite different names*

### Comparing `oxasl-0.1.9/oxasl/preproc.py` & `oxasl-0.1.9.post1/oxasl/preproc.py`

 * *Files identical despite different names*

### Comparing `oxasl-0.1.9/oxasl/quasil.py` & `oxasl-0.1.9.post1/oxasl/quasil.py`

 * *Files identical despite different names*

### Comparing `oxasl-0.1.9/oxasl/reg.py` & `oxasl-0.1.9.post1/oxasl/reg.py`

 * *Files identical despite different names*

### Comparing `oxasl-0.1.9/oxasl/reporting.py` & `oxasl-0.1.9.post1/oxasl/reporting.py`

 * *Files identical despite different names*

### Comparing `oxasl-0.1.9/oxasl/struc.py` & `oxasl-0.1.9.post1/oxasl/struc.py`

 * *Files identical despite different names*

### Comparing `oxasl-0.1.9/oxasl/test/test_basil.py` & `oxasl-0.1.9.post1/oxasl/test/test_basil.py`

 * *Files identical despite different names*

### Comparing `oxasl-0.1.9/oxasl/test/test_calib.py` & `oxasl-0.1.9.post1/oxasl/test/test_calib.py`

 * *Files identical despite different names*

### Comparing `oxasl-0.1.9/oxasl/test/test_image.py` & `oxasl-0.1.9.post1/oxasl/test/test_image.py`

 * *Files identical despite different names*

### Comparing `oxasl-0.1.9/oxasl/test/test_preproc.py` & `oxasl-0.1.9.post1/oxasl/test/test_preproc.py`

 * *Files identical despite different names*

### Comparing `oxasl-0.1.9/oxasl/test/test_reg.py` & `oxasl-0.1.9.post1/oxasl/test/test_reg.py`

 * *Files identical despite different names*

### Comparing `oxasl-0.1.9/oxasl/test/test_workspace.py` & `oxasl-0.1.9.post1/oxasl/test/test_workspace.py`

 * *Files identical despite different names*

### Comparing `oxasl-0.1.9/oxasl/utils.py` & `oxasl-0.1.9.post1/oxasl/utils.py`

 * *Files identical despite different names*

### Comparing `oxasl-0.1.9/oxasl/workspace.py` & `oxasl-0.1.9.post1/oxasl/workspace.py`

 * *Files identical despite different names*

### Comparing `oxasl-0.1.9/oxasl/wrappers/avscale.py` & `oxasl-0.1.9.post1/oxasl/wrappers/avscale.py`

 * *Files identical despite different names*

### Comparing `oxasl-0.1.9/oxasl/wrappers/epi_reg.py` & `oxasl-0.1.9.post1/oxasl/wrappers/epi_reg.py`

 * *Files identical despite different names*

### Comparing `oxasl-0.1.9/oxasl/wrappers/fabber.py` & `oxasl-0.1.9.post1/oxasl/wrappers/fabber.py`

 * *Files identical despite different names*

### Comparing `oxasl-0.1.9/oxasl/wrappers/fnirt_extra.py` & `oxasl-0.1.9.post1/oxasl/wrappers/fnirt_extra.py`

 * *Files identical despite different names*

### Comparing `oxasl-0.1.9/oxasl.egg-info/PKG-INFO` & `oxasl-0.1.9.post1/oxasl.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oxasl
-Version: 0.1.9
+Version: 0.1.9.post1
 Summary: Python library for manipulating and modelling ASL data
 Home-page: https://oxasl.readthedocs.io/
 Author: Martin Craig
 Author-email: martin.craig@eng.ox.ac.uk
 License: License granted by University of Oxford for use by academics carrying out research and not for use by consumers or commercial businesses. See LICENSE file for more details
 Description: OXASL - FSL based ASL pipeline
         ==============================
```

### Comparing `oxasl-0.1.9/oxasl.egg-info/SOURCES.txt` & `oxasl-0.1.9.post1/oxasl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `oxasl-0.1.9/setup.py` & `oxasl-0.1.9.post1/setup.py`

 * *Files identical despite different names*

