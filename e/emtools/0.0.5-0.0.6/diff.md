# Comparing `tmp/emtools-0.0.5.tar.gz` & `tmp/emtools-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emtools-0.0.5.tar", last modified: Thu Jul 13 20:36:25 2023, max compression
+gzip compressed data, was "emtools-0.0.6.tar", last modified: Thu Jul 13 20:58:46 2023, max compression
```

## Comparing `emtools-0.0.5.tar` & `emtools-0.0.6.tar`

### file list

```diff
@@ -1,64 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:36:25.673262 emtools-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 20:36:12.000000 emtools-0.0.5/CHANGES.txt
--rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-07-13 20:36:12.000000 emtools-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-13 20:36:12.000000 emtools-0.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-07-13 20:36:25.673262 emtools-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-07-13 20:36:12.000000 emtools-0.0.5/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:36:25.669261 emtools-0.0.5/emtools/
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-07-13 20:36:12.000000 emtools-0.0.5/emtools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:36:25.669261 emtools-0.0.5/emtools/hpc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 20:36:12.000000 emtools-0.0.5/emtools/hpc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-07-13 20:36:12.000000 emtools-0.0.5/emtools/hpc/__main__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4884 2023-07-13 20:36:12.000000 emtools-0.0.5/emtools/hpc/lsf.py
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-07-13 20:36:12.000000 emtools-0.0.5/emtools/hpc/submit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:36:25.669261 emtools-0.0.5/emtools/image/
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-07-13 20:36:12.000000 emtools-0.0.5/emtools/image/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4178 2023-07-13 20:36:12.000000 emtools-0.0.5/emtools/image/thumbnail.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:36:25.669261 emtools-0.0.5/emtools/metadata/
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-07-13 20:36:12.000000 emtools-0.0.5/emtools/metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10903 2023-07-13 20:36:12.000000 emtools-0.0.5/emtools/metadata/epu.py
--rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-07-13 20:36:12.000000 emtools-0.0.5/emtools/metadata/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5482 2023-07-13 20:36:12.000000 emtools-0.0.5/emtools/metadata/sqlite.py
--rw-r--r--   0 runner    (1001) docker     (123)    13079 2023-07-13 20:36:12.000000 emtools-0.0.5/emtools/metadata/starfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     9227 2023-07-13 20:36:12.000000 emtools-0.0.5/emtools/metadata/table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:36:25.669261 emtools-0.0.5/emtools/processing/
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-07-13 20:36:12.000000 emtools-0.0.5/emtools/processing/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1271 2023-07-13 20:36:12.000000 emtools-0.0.5/emtools/processing/__main__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6682 2023-07-13 20:36:12.000000 emtools-0.0.5/emtools/processing/motioncor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:36:25.669261 emtools-0.0.5/emtools/pwx/
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-07-13 20:36:12.000000 emtools-0.0.5/emtools/pwx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4868 2023-07-13 20:36:12.000000 emtools-0.0.5/emtools/pwx/monitors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-07-13 20:36:12.000000 emtools-0.0.5/emtools/pwx/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:36:25.669261 emtools-0.0.5/emtools/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 20:36:12.000000 emtools-0.0.5/emtools/scripts/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4774 2023-07-13 20:36:12.000000 emtools-0.0.5/emtools/scripts/emt-beamshifts.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2393 2023-07-13 20:36:12.000000 emtools-0.0.5/emtools/scripts/emt-change-optics.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1562 2023-07-13 20:36:12.000000 emtools-0.0.5/emtools/scripts/emt-epu-parse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4186 2023-07-13 20:36:12.000000 emtools-0.0.5/emtools/scripts/emt-files.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3539 2023-07-13 20:36:12.000000 emtools-0.0.5/emtools/scripts/emt-frames.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1888 2023-07-13 20:36:12.000000 emtools-0.0.5/emtools/scripts/emt-ps.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    21289 2023-07-13 20:36:12.000000 emtools-0.0.5/emtools/scripts/emt-scipion-otf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:36:25.673262 emtools-0.0.5/emtools/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-07-13 20:36:12.000000 emtools-0.0.5/emtools/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9443 2023-07-13 20:36:12.000000 emtools-0.0.5/emtools/tests/test_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-07-13 20:36:12.000000 emtools-0.0.5/emtools/tests/test_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-07-13 20:36:12.000000 emtools-0.0.5/emtools/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:36:25.673262 emtools-0.0.5/emtools/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-07-13 20:36:12.000000 emtools-0.0.5/emtools/utils/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1195 2023-07-13 20:36:12.000000 emtools-0.0.5/emtools/utils/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-07-13 20:36:12.000000 emtools-0.0.5/emtools/utils/color.py
--rw-r--r--   0 runner    (1001) docker     (123)    11307 2023-07-13 20:36:12.000000 emtools-0.0.5/emtools/utils/path.py
--rw-r--r--   0 runner    (1001) docker     (123)     5951 2023-07-13 20:36:12.000000 emtools-0.0.5/emtools/utils/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-07-13 20:36:12.000000 emtools-0.0.5/emtools/utils/pretty.py
--rw-r--r--   0 runner    (1001) docker     (123)     4375 2023-07-13 20:36:12.000000 emtools-0.0.5/emtools/utils/process.py
--rw-r--r--   0 runner    (1001) docker     (123)     4022 2023-07-13 20:36:12.000000 emtools-0.0.5/emtools/utils/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     3138 2023-07-13 20:36:12.000000 emtools-0.0.5/emtools/utils/system.py
--rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-07-13 20:36:12.000000 emtools-0.0.5/emtools/utils/time.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:36:25.669261 emtools-0.0.5/emtools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-07-13 20:36:25.000000 emtools-0.0.5/emtools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-07-13 20:36:25.000000 emtools-0.0.5/emtools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 20:36:25.000000 emtools-0.0.5/emtools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-13 20:36:25.000000 emtools-0.0.5/emtools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-13 20:36:12.000000 emtools-0.0.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 20:36:25.673262 emtools-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2675 2023-07-13 20:36:12.000000 emtools-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:58:46.915201 emtools-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 20:58:36.000000 emtools-0.0.6/CHANGES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-07-13 20:58:36.000000 emtools-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-13 20:58:36.000000 emtools-0.0.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-07-13 20:58:46.915201 emtools-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-07-13 20:58:36.000000 emtools-0.0.6/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:58:46.907201 emtools-0.0.6/emtools/
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-07-13 20:58:36.000000 emtools-0.0.6/emtools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:58:46.911201 emtools-0.0.6/emtools/hpc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 20:58:36.000000 emtools-0.0.6/emtools/hpc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-07-13 20:58:36.000000 emtools-0.0.6/emtools/hpc/__main__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4884 2023-07-13 20:58:36.000000 emtools-0.0.6/emtools/hpc/lsf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-07-13 20:58:36.000000 emtools-0.0.6/emtools/hpc/submit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:58:46.911201 emtools-0.0.6/emtools/image/
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-07-13 20:58:36.000000 emtools-0.0.6/emtools/image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4178 2023-07-13 20:58:36.000000 emtools-0.0.6/emtools/image/thumbnail.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:58:46.911201 emtools-0.0.6/emtools/metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-07-13 20:58:36.000000 emtools-0.0.6/emtools/metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10903 2023-07-13 20:58:36.000000 emtools-0.0.6/emtools/metadata/epu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-07-13 20:58:36.000000 emtools-0.0.6/emtools/metadata/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5482 2023-07-13 20:58:36.000000 emtools-0.0.6/emtools/metadata/sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13079 2023-07-13 20:58:36.000000 emtools-0.0.6/emtools/metadata/starfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9227 2023-07-13 20:58:36.000000 emtools-0.0.6/emtools/metadata/table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:58:46.911201 emtools-0.0.6/emtools/processing/
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-07-13 20:58:36.000000 emtools-0.0.6/emtools/processing/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1271 2023-07-13 20:58:36.000000 emtools-0.0.6/emtools/processing/__main__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6682 2023-07-13 20:58:36.000000 emtools-0.0.6/emtools/processing/motioncor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:58:46.911201 emtools-0.0.6/emtools/pwx/
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-07-13 20:58:36.000000 emtools-0.0.6/emtools/pwx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4868 2023-07-13 20:58:36.000000 emtools-0.0.6/emtools/pwx/monitors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-07-13 20:58:36.000000 emtools-0.0.6/emtools/pwx/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:58:46.911201 emtools-0.0.6/emtools/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 20:58:36.000000 emtools-0.0.6/emtools/scripts/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4774 2023-07-13 20:58:36.000000 emtools-0.0.6/emtools/scripts/emt-beamshifts.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2393 2023-07-13 20:58:36.000000 emtools-0.0.6/emtools/scripts/emt-change-optics.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1562 2023-07-13 20:58:36.000000 emtools-0.0.6/emtools/scripts/emt-epu-parse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4186 2023-07-13 20:58:36.000000 emtools-0.0.6/emtools/scripts/emt-files.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3539 2023-07-13 20:58:36.000000 emtools-0.0.6/emtools/scripts/emt-frames.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1888 2023-07-13 20:58:36.000000 emtools-0.0.6/emtools/scripts/emt-ps.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    21289 2023-07-13 20:58:36.000000 emtools-0.0.6/emtools/scripts/emt-scipion-otf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:58:46.911201 emtools-0.0.6/emtools/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-07-13 20:58:36.000000 emtools-0.0.6/emtools/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9443 2023-07-13 20:58:36.000000 emtools-0.0.6/emtools/tests/test_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-07-13 20:58:36.000000 emtools-0.0.6/emtools/tests/test_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-07-13 20:58:36.000000 emtools-0.0.6/emtools/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:58:46.915201 emtools-0.0.6/emtools/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-07-13 20:58:36.000000 emtools-0.0.6/emtools/utils/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1195 2023-07-13 20:58:36.000000 emtools-0.0.6/emtools/utils/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-07-13 20:58:36.000000 emtools-0.0.6/emtools/utils/color.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11307 2023-07-13 20:58:36.000000 emtools-0.0.6/emtools/utils/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5951 2023-07-13 20:58:36.000000 emtools-0.0.6/emtools/utils/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-07-13 20:58:36.000000 emtools-0.0.6/emtools/utils/pretty.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4375 2023-07-13 20:58:36.000000 emtools-0.0.6/emtools/utils/process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4022 2023-07-13 20:58:36.000000 emtools-0.0.6/emtools/utils/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3138 2023-07-13 20:58:36.000000 emtools-0.0.6/emtools/utils/system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-07-13 20:58:36.000000 emtools-0.0.6/emtools/utils/time.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:58:46.911201 emtools-0.0.6/emtools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-07-13 20:58:46.000000 emtools-0.0.6/emtools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-07-13 20:58:46.000000 emtools-0.0.6/emtools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 20:58:46.000000 emtools-0.0.6/emtools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-13 20:58:46.000000 emtools-0.0.6/emtools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-13 20:58:46.000000 emtools-0.0.6/emtools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-13 20:58:36.000000 emtools-0.0.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 20:58:46.915201 emtools-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-07-13 20:58:36.000000 emtools-0.0.6/setup.py
```

### Comparing `emtools-0.0.5/LICENSE` & `emtools-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `emtools-0.0.5/PKG-INFO` & `emtools-0.0.6/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 1.2
 Name: emtools
-Version: 0.0.5
-Summary: Basic utilities for CryoEM data manipulation
+Version: 0.0.6
+Summary: Utilities for CryoEM data manipulation
 Home-page: https://github.com/3dem/emtools
 Author: J.M. De la Rosa Trevin, Grigory Sharov
 Author-email: delarosatrevin@gmail.com, gsharov@mrc-lmb.cam.ac.uk
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/3dem/emtools/issues
 Project-URL: Source, https://github.com/3dem/emtools
 Description: =======
@@ -13,21 +13,22 @@
         =======
         
         Utilities for CryoEM data manipulation.
         
         Installation
         ------------
         
-        ``pip install emtools``
+        .. code-block:: bash
+        
+            pip install emtools
         
         Or for development:
         
         .. code-block:: bash
         
-            # Or for development
             git clone git@github.com:3dem/emtools.git
             cd emtools
             pip install -e .
         
         Usage
         -----
         
@@ -55,10 +56,10 @@
         
         
         
         
         
 Keywords: electron-microscopy cryo-em structural-biology image-processing
 Platform: UNKNOWN
-Classifier: Development Status :: 1 - Planning
+Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
```

### Comparing `emtools-0.0.5/README.rst` & `emtools-0.0.6/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -3,21 +3,22 @@
 =======
 
 Utilities for CryoEM data manipulation.
 
 Installation
 ------------
 
-``pip install emtools``
+.. code-block:: bash
+
+    pip install emtools
 
 Or for development:
 
 .. code-block:: bash
 
-    # Or for development
     git clone git@github.com:3dem/emtools.git
     cd emtools
     pip install -e .
 
 Usage
 -----
```

### Comparing `emtools-0.0.5/emtools/__init__.py` & `emtools-0.0.6/emtools/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,8 +20,8 @@
 # * 02111-1307  USA
 # *
 # *  All comments concerning this program package may be sent to the
 # *  e-mail address 'delarosatrevin@scilifelab.se'
 # *
 # **************************************************************************
 
-__version__ = '0.0.5'
+__version__ = '0.0.6'
```

### Comparing `emtools-0.0.5/emtools/hpc/__main__.py` & `emtools-0.0.6/emtools/hpc/__main__.py`

 * *Files identical despite different names*

### Comparing `emtools-0.0.5/emtools/hpc/lsf.py` & `emtools-0.0.6/emtools/hpc/lsf.py`

 * *Files identical despite different names*

### Comparing `emtools-0.0.5/emtools/hpc/submit.py` & `emtools-0.0.6/emtools/hpc/submit.py`

 * *Files identical despite different names*

### Comparing `emtools-0.0.5/emtools/image/__init__.py` & `emtools-0.0.6/emtools/image/__init__.py`

 * *Files identical despite different names*

### Comparing `emtools-0.0.5/emtools/image/thumbnail.py` & `emtools-0.0.6/emtools/image/thumbnail.py`

 * *Files identical despite different names*

### Comparing `emtools-0.0.5/emtools/metadata/__init__.py` & `emtools-0.0.6/emtools/metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `emtools-0.0.5/emtools/metadata/epu.py` & `emtools-0.0.6/emtools/metadata/epu.py`

 * *Files identical despite different names*

### Comparing `emtools-0.0.5/emtools/metadata/misc.py` & `emtools-0.0.6/emtools/metadata/misc.py`

 * *Files identical despite different names*

### Comparing `emtools-0.0.5/emtools/metadata/sqlite.py` & `emtools-0.0.6/emtools/metadata/sqlite.py`

 * *Files identical despite different names*

### Comparing `emtools-0.0.5/emtools/metadata/starfile.py` & `emtools-0.0.6/emtools/metadata/starfile.py`

 * *Files identical despite different names*

### Comparing `emtools-0.0.5/emtools/metadata/table.py` & `emtools-0.0.6/emtools/metadata/table.py`

 * *Files identical despite different names*

### Comparing `emtools-0.0.5/emtools/processing/__init__.py` & `emtools-0.0.6/emtools/processing/__init__.py`

 * *Files identical despite different names*

### Comparing `emtools-0.0.5/emtools/processing/__main__.py` & `emtools-0.0.6/emtools/processing/__main__.py`

 * *Files identical despite different names*

### Comparing `emtools-0.0.5/emtools/processing/motioncor.py` & `emtools-0.0.6/emtools/processing/motioncor.py`

 * *Files identical despite different names*

### Comparing `emtools-0.0.5/emtools/pwx/__init__.py` & `emtools-0.0.6/emtools/pwx/__init__.py`

 * *Files identical despite different names*

### Comparing `emtools-0.0.5/emtools/pwx/monitors.py` & `emtools-0.0.6/emtools/pwx/monitors.py`

 * *Files identical despite different names*

### Comparing `emtools-0.0.5/emtools/pwx/workflow.py` & `emtools-0.0.6/emtools/pwx/workflow.py`

 * *Files identical despite different names*

### Comparing `emtools-0.0.5/emtools/scripts/emt-beamshifts.py` & `emtools-0.0.6/emtools/scripts/emt-beamshifts.py`

 * *Files identical despite different names*

### Comparing `emtools-0.0.5/emtools/scripts/emt-change-optics.py` & `emtools-0.0.6/emtools/scripts/emt-change-optics.py`

 * *Files identical despite different names*

### Comparing `emtools-0.0.5/emtools/scripts/emt-epu-parse.py` & `emtools-0.0.6/emtools/scripts/emt-epu-parse.py`

 * *Files identical despite different names*

### Comparing `emtools-0.0.5/emtools/scripts/emt-files.py` & `emtools-0.0.6/emtools/scripts/emt-files.py`

 * *Files identical despite different names*

### Comparing `emtools-0.0.5/emtools/scripts/emt-frames.py` & `emtools-0.0.6/emtools/scripts/emt-frames.py`

 * *Files identical despite different names*

### Comparing `emtools-0.0.5/emtools/scripts/emt-ps.py` & `emtools-0.0.6/emtools/scripts/emt-ps.py`

 * *Files identical despite different names*

### Comparing `emtools-0.0.5/emtools/scripts/emt-scipion-otf.py` & `emtools-0.0.6/emtools/scripts/emt-scipion-otf.py`

 * *Files identical despite different names*

### Comparing `emtools-0.0.5/emtools/tests/test_metadata.py` & `emtools-0.0.6/emtools/tests/test_metadata.py`

 * *Files identical despite different names*

### Comparing `emtools-0.0.5/emtools/tests/test_pipeline.py` & `emtools-0.0.6/emtools/tests/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `emtools-0.0.5/emtools/tests/test_utils.py` & `emtools-0.0.6/emtools/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `emtools-0.0.5/emtools/utils/__init__.py` & `emtools-0.0.6/emtools/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `emtools-0.0.5/emtools/utils/__main__.py` & `emtools-0.0.6/emtools/utils/__main__.py`

 * *Files identical despite different names*

### Comparing `emtools-0.0.5/emtools/utils/color.py` & `emtools-0.0.6/emtools/utils/color.py`

 * *Files identical despite different names*

### Comparing `emtools-0.0.5/emtools/utils/path.py` & `emtools-0.0.6/emtools/utils/path.py`

 * *Files identical despite different names*

### Comparing `emtools-0.0.5/emtools/utils/pipeline.py` & `emtools-0.0.6/emtools/utils/pipeline.py`

 * *Files identical despite different names*

### Comparing `emtools-0.0.5/emtools/utils/pretty.py` & `emtools-0.0.6/emtools/utils/pretty.py`

 * *Files identical despite different names*

### Comparing `emtools-0.0.5/emtools/utils/process.py` & `emtools-0.0.6/emtools/utils/process.py`

 * *Files identical despite different names*

### Comparing `emtools-0.0.5/emtools/utils/server.py` & `emtools-0.0.6/emtools/utils/server.py`

 * *Files identical despite different names*

### Comparing `emtools-0.0.5/emtools/utils/system.py` & `emtools-0.0.6/emtools/utils/system.py`

 * *Files identical despite different names*

### Comparing `emtools-0.0.5/emtools/utils/time.py` & `emtools-0.0.6/emtools/utils/time.py`

 * *Files identical despite different names*

### Comparing `emtools-0.0.5/emtools.egg-info/PKG-INFO` & `emtools-0.0.6/emtools.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 1.2
 Name: emtools
-Version: 0.0.5
-Summary: Basic utilities for CryoEM data manipulation
+Version: 0.0.6
+Summary: Utilities for CryoEM data manipulation
 Home-page: https://github.com/3dem/emtools
 Author: J.M. De la Rosa Trevin, Grigory Sharov
 Author-email: delarosatrevin@gmail.com, gsharov@mrc-lmb.cam.ac.uk
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/3dem/emtools/issues
 Project-URL: Source, https://github.com/3dem/emtools
 Description: =======
@@ -13,21 +13,22 @@
         =======
         
         Utilities for CryoEM data manipulation.
         
         Installation
         ------------
         
-        ``pip install emtools``
+        .. code-block:: bash
+        
+            pip install emtools
         
         Or for development:
         
         .. code-block:: bash
         
-            # Or for development
             git clone git@github.com:3dem/emtools.git
             cd emtools
             pip install -e .
         
         Usage
         -----
         
@@ -55,10 +56,10 @@
         
         
         
         
         
 Keywords: electron-microscopy cryo-em structural-biology image-processing
 Platform: UNKNOWN
-Classifier: Development Status :: 1 - Planning
+Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
```

### Comparing `emtools-0.0.5/emtools.egg-info/SOURCES.txt` & `emtools-0.0.6/emtools.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 README.rst
 requirements.txt
 setup.py
 emtools/__init__.py
 emtools.egg-info/PKG-INFO
 emtools.egg-info/SOURCES.txt
 emtools.egg-info/dependency_links.txt
+emtools.egg-info/requires.txt
 emtools.egg-info/top_level.txt
 emtools/hpc/__init__.py
 emtools/hpc/__main__.py
 emtools/hpc/lsf.py
 emtools/hpc/submit.py
 emtools/image/__init__.py
 emtools/image/thumbnail.py
```

### Comparing `emtools-0.0.5/setup.py` & `emtools-0.0.6/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -25,43 +25,50 @@
 
 """A setuptools based setup module.
 See:
 https://packaging.python.org/en/latest/distributing.html
 https://github.com/pypa/sampleproject
 """
 
+import os
 # Always prefer setuptools over distutils
 from setuptools import setup, find_packages
 # To use a consistent encoding
 from codecs import open
 from os import path
 import emtools
 
 here = path.abspath(path.dirname(__file__))
 
 # Get the long description from the README file
 with open(path.join(here, 'README.rst'), encoding='utf-8') as f:
     long_description = f.read()
 
+# Read requirements.txt
+with open(os.path.join(here, 'requirements.txt')) as f:
+    requirements = f.read().splitlines()
+
 # Arguments marked as "Required" below must be included for upload to PyPI.
 # Fields marked as "Optional" may be commented out.
 
 setup(
     name='emtools',  # Required
     version=emtools.__version__,  # Required
-    description='Basic utilities for CryoEM data manipulation',  # Required
+    description='Utilities for CryoEM data manipulation',  # Required
     long_description=long_description,  # Optional
     url='https://github.com/3dem/emtools',  # Optional
     author='J.M. De la Rosa Trevin, Grigory Sharov',  # Optional
     author_email='delarosatrevin@gmail.com, gsharov@mrc-lmb.cam.ac.uk',  # Optional
     classifiers=[  # Optional
-        'Development Status :: 1 - Planning',
+        'Development Status :: 3 - Alpha',
         'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
         'Programming Language :: Python :: 3'
     ],
     keywords='electron-microscopy cryo-em structural-biology image-processing',  # Optional
     packages=find_packages(),
     project_urls={  # Optional
         'Bug Reports': 'https://github.com/3dem/emtools/issues',
         'Source': 'https://github.com/3dem/emtools',
     },
+    include_package_data=True,
+    install_requires=requirements
 )
```

