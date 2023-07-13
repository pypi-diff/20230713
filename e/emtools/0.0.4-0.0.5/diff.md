# Comparing `tmp/emtools-0.0.4.tar.gz` & `tmp/emtools-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emtools-0.0.4.tar", last modified: Thu Feb  9 15:51:17 2023, max compression
+gzip compressed data, was "emtools-0.0.5.tar", last modified: Thu Jul 13 20:36:25 2023, max compression
```

## Comparing `emtools-0.0.4.tar` & `emtools-0.0.5.tar`

### file list

```diff
@@ -1,52 +1,64 @@
-drwxr-xr-x   0 jdela80  (97711) domain users (76937)        0 2023-02-09 15:51:17.998030 emtools-0.0.4/
--rw-r--r--   0 jdela80  (97711) domain users (76937)        0 2022-10-20 16:56:38.000000 emtools-0.0.4/CHANGES.txt
--rw-r--r--   0 jdela80  (97711) domain users (76937)    35147 2022-10-20 16:56:38.000000 emtools-0.0.4/LICENSE
--rw-r--r--   0 jdela80  (97711) domain users (76937)       44 2022-10-20 16:56:38.000000 emtools-0.0.4/MANIFEST.in
--rw-r--r--   0 jdela80  (97711) domain users (76937)     1341 2023-02-09 15:51:17.997030 emtools-0.0.4/PKG-INFO
--rw-r--r--   0 jdela80  (97711) domain users (76937)      693 2022-11-12 18:34:50.000000 emtools-0.0.4/README.rst
-drwxr-xr-x   0 jdela80  (97711) domain users (76937)        0 2023-02-09 15:51:17.995030 emtools-0.0.4/emtools/
--rw-r--r--   0 jdela80  (97711) domain users (76937)     1162 2023-02-09 15:50:42.000000 emtools-0.0.4/emtools/__init__.py
-drwxr-xr-x   0 jdela80  (97711) domain users (76937)        0 2023-02-09 15:51:17.996030 emtools-0.0.4/emtools/hpc/
--rw-r--r--   0 jdela80  (97711) domain users (76937)        0 2022-10-20 18:13:47.000000 emtools-0.0.4/emtools/hpc/__init__.py
--rw-r--r--   0 jdela80  (97711) domain users (76937)     1332 2022-10-21 20:08:01.000000 emtools-0.0.4/emtools/hpc/__main__.py
--rwxr-xr-x   0 jdela80  (97711) domain users (76937)     4884 2022-12-13 04:30:54.000000 emtools-0.0.4/emtools/hpc/lsf.py
--rw-r--r--   0 jdela80  (97711) domain users (76937)      520 2022-11-03 18:27:09.000000 emtools-0.0.4/emtools/hpc/submit.py
-drwxr-xr-x   0 jdela80  (97711) domain users (76937)        0 2023-02-09 15:51:17.996030 emtools-0.0.4/emtools/image/
--rw-r--r--   0 jdela80  (97711) domain users (76937)     1173 2022-10-20 16:56:38.000000 emtools-0.0.4/emtools/image/__init__.py
--rw-r--r--   0 jdela80  (97711) domain users (76937)     4178 2022-11-10 20:11:42.000000 emtools-0.0.4/emtools/image/thumbnail.py
-drwxr-xr-x   0 jdela80  (97711) domain users (76937)        0 2023-02-09 15:51:17.996030 emtools-0.0.4/emtools/metadata/
--rw-r--r--   0 jdela80  (97711) domain users (76937)      841 2023-01-11 17:34:36.000000 emtools-0.0.4/emtools/metadata/__init__.py
--rw-r--r--   0 jdela80  (97711) domain users (76937)     4029 2023-02-08 17:23:42.000000 emtools-0.0.4/emtools/metadata/epu.py
--rw-r--r--   0 jdela80  (97711) domain users (76937)    12983 2023-02-09 15:43:06.000000 emtools-0.0.4/emtools/metadata/starfile.py
--rw-r--r--   0 jdela80  (97711) domain users (76937)    10719 2022-11-12 17:51:25.000000 emtools-0.0.4/emtools/metadata/table.py
-drwxr-xr-x   0 jdela80  (97711) domain users (76937)        0 2023-02-09 15:51:17.996030 emtools-0.0.4/emtools/processing/
--rw-r--r--   0 jdela80  (97711) domain users (76937)      744 2022-12-27 15:12:49.000000 emtools-0.0.4/emtools/processing/__init__.py
--rwxr-xr-x   0 jdela80  (97711) domain users (76937)     1271 2022-12-27 15:12:49.000000 emtools-0.0.4/emtools/processing/__main__.py
--rwxr-xr-x   0 jdela80  (97711) domain users (76937)     6700 2022-12-27 15:12:49.000000 emtools-0.0.4/emtools/processing/motioncor.py
-drwxr-xr-x   0 jdela80  (97711) domain users (76937)        0 2023-02-09 15:51:17.996030 emtools-0.0.4/emtools/pwx/
--rw-r--r--   0 jdela80  (97711) domain users (76937)      791 2022-12-27 15:12:49.000000 emtools-0.0.4/emtools/pwx/__init__.py
--rw-r--r--   0 jdela80  (97711) domain users (76937)     4868 2022-12-27 15:12:49.000000 emtools-0.0.4/emtools/pwx/monitors.py
-drwxr-xr-x   0 jdela80  (97711) domain users (76937)        0 2023-02-09 15:51:17.997030 emtools-0.0.4/emtools/tests/
--rw-r--r--   0 jdela80  (97711) domain users (76937)      281 2022-11-12 17:41:46.000000 emtools-0.0.4/emtools/tests/__init__.py
--rw-r--r--   0 jdela80  (97711) domain users (76937)     6205 2023-01-11 17:48:29.000000 emtools-0.0.4/emtools/tests/test_metadata.py
--rw-r--r--   0 jdela80  (97711) domain users (76937)     2374 2022-11-30 04:05:23.000000 emtools-0.0.4/emtools/tests/test_pipeline.py
--rw-r--r--   0 jdela80  (97711) domain users (76937)     1487 2022-12-13 04:30:54.000000 emtools-0.0.4/emtools/tests/test_utils.py
-drwxr-xr-x   0 jdela80  (97711) domain users (76937)        0 2023-02-09 15:51:17.997030 emtools-0.0.4/emtools/utils/
--rw-r--r--   0 jdela80  (97711) domain users (76937)      979 2022-12-27 21:29:36.000000 emtools-0.0.4/emtools/utils/__init__.py
--rwxr-xr-x   0 jdela80  (97711) domain users (76937)     1195 2022-12-27 15:12:49.000000 emtools-0.0.4/emtools/utils/__main__.py
--rw-r--r--   0 jdela80  (97711) domain users (76937)     1235 2023-01-11 17:07:06.000000 emtools-0.0.4/emtools/utils/color.py
--rw-r--r--   0 jdela80  (97711) domain users (76937)    10200 2023-02-08 17:37:42.000000 emtools-0.0.4/emtools/utils/path.py
--rw-r--r--   0 jdela80  (97711) domain users (76937)     5951 2023-01-11 17:07:06.000000 emtools-0.0.4/emtools/utils/pipeline.py
--rw-r--r--   0 jdela80  (97711) domain users (76937)     2584 2023-01-11 17:07:30.000000 emtools-0.0.4/emtools/utils/pretty.py
--rw-r--r--   0 jdela80  (97711) domain users (76937)     2133 2023-01-13 20:19:15.000000 emtools-0.0.4/emtools/utils/process.py
--rw-r--r--   0 jdela80  (97711) domain users (76937)     4056 2023-01-12 19:46:32.000000 emtools-0.0.4/emtools/utils/server.py
--rw-r--r--   0 jdela80  (97711) domain users (76937)     2229 2022-12-13 04:30:54.000000 emtools-0.0.4/emtools/utils/system.py
--rw-r--r--   0 jdela80  (97711) domain users (76937)     1398 2022-12-27 15:12:49.000000 emtools-0.0.4/emtools/utils/time.py
-drwxr-xr-x   0 jdela80  (97711) domain users (76937)        0 2023-02-09 15:51:17.996030 emtools-0.0.4/emtools.egg-info/
--rw-r--r--   0 jdela80  (97711) domain users (76937)     1341 2023-02-09 15:51:17.000000 emtools-0.0.4/emtools.egg-info/PKG-INFO
--rw-r--r--   0 jdela80  (97711) domain users (76937)      962 2023-02-09 15:51:17.000000 emtools-0.0.4/emtools.egg-info/SOURCES.txt
--rw-r--r--   0 jdela80  (97711) domain users (76937)        1 2023-02-09 15:51:17.000000 emtools-0.0.4/emtools.egg-info/dependency_links.txt
--rw-r--r--   0 jdela80  (97711) domain users (76937)        8 2023-02-09 15:51:17.000000 emtools-0.0.4/emtools.egg-info/top_level.txt
--rw-r--r--   0 jdela80  (97711) domain users (76937)       44 2023-01-24 14:54:56.000000 emtools-0.0.4/requirements.txt
--rw-r--r--   0 jdela80  (97711) domain users (76937)       38 2023-02-09 15:51:17.998030 emtools-0.0.4/setup.cfg
--rw-r--r--   0 jdela80  (97711) domain users (76937)     2675 2022-10-20 17:17:42.000000 emtools-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:36:25.673262 emtools-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 20:36:12.000000 emtools-0.0.5/CHANGES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-07-13 20:36:12.000000 emtools-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-13 20:36:12.000000 emtools-0.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-07-13 20:36:25.673262 emtools-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-07-13 20:36:12.000000 emtools-0.0.5/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:36:25.669261 emtools-0.0.5/emtools/
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-07-13 20:36:12.000000 emtools-0.0.5/emtools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:36:25.669261 emtools-0.0.5/emtools/hpc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 20:36:12.000000 emtools-0.0.5/emtools/hpc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-07-13 20:36:12.000000 emtools-0.0.5/emtools/hpc/__main__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4884 2023-07-13 20:36:12.000000 emtools-0.0.5/emtools/hpc/lsf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-07-13 20:36:12.000000 emtools-0.0.5/emtools/hpc/submit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:36:25.669261 emtools-0.0.5/emtools/image/
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-07-13 20:36:12.000000 emtools-0.0.5/emtools/image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4178 2023-07-13 20:36:12.000000 emtools-0.0.5/emtools/image/thumbnail.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:36:25.669261 emtools-0.0.5/emtools/metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-07-13 20:36:12.000000 emtools-0.0.5/emtools/metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10903 2023-07-13 20:36:12.000000 emtools-0.0.5/emtools/metadata/epu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-07-13 20:36:12.000000 emtools-0.0.5/emtools/metadata/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5482 2023-07-13 20:36:12.000000 emtools-0.0.5/emtools/metadata/sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13079 2023-07-13 20:36:12.000000 emtools-0.0.5/emtools/metadata/starfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9227 2023-07-13 20:36:12.000000 emtools-0.0.5/emtools/metadata/table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:36:25.669261 emtools-0.0.5/emtools/processing/
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-07-13 20:36:12.000000 emtools-0.0.5/emtools/processing/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1271 2023-07-13 20:36:12.000000 emtools-0.0.5/emtools/processing/__main__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6682 2023-07-13 20:36:12.000000 emtools-0.0.5/emtools/processing/motioncor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:36:25.669261 emtools-0.0.5/emtools/pwx/
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-07-13 20:36:12.000000 emtools-0.0.5/emtools/pwx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4868 2023-07-13 20:36:12.000000 emtools-0.0.5/emtools/pwx/monitors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-07-13 20:36:12.000000 emtools-0.0.5/emtools/pwx/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:36:25.669261 emtools-0.0.5/emtools/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 20:36:12.000000 emtools-0.0.5/emtools/scripts/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4774 2023-07-13 20:36:12.000000 emtools-0.0.5/emtools/scripts/emt-beamshifts.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2393 2023-07-13 20:36:12.000000 emtools-0.0.5/emtools/scripts/emt-change-optics.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1562 2023-07-13 20:36:12.000000 emtools-0.0.5/emtools/scripts/emt-epu-parse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4186 2023-07-13 20:36:12.000000 emtools-0.0.5/emtools/scripts/emt-files.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3539 2023-07-13 20:36:12.000000 emtools-0.0.5/emtools/scripts/emt-frames.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1888 2023-07-13 20:36:12.000000 emtools-0.0.5/emtools/scripts/emt-ps.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    21289 2023-07-13 20:36:12.000000 emtools-0.0.5/emtools/scripts/emt-scipion-otf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:36:25.673262 emtools-0.0.5/emtools/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-07-13 20:36:12.000000 emtools-0.0.5/emtools/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9443 2023-07-13 20:36:12.000000 emtools-0.0.5/emtools/tests/test_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-07-13 20:36:12.000000 emtools-0.0.5/emtools/tests/test_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-07-13 20:36:12.000000 emtools-0.0.5/emtools/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:36:25.673262 emtools-0.0.5/emtools/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-07-13 20:36:12.000000 emtools-0.0.5/emtools/utils/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1195 2023-07-13 20:36:12.000000 emtools-0.0.5/emtools/utils/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-07-13 20:36:12.000000 emtools-0.0.5/emtools/utils/color.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11307 2023-07-13 20:36:12.000000 emtools-0.0.5/emtools/utils/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5951 2023-07-13 20:36:12.000000 emtools-0.0.5/emtools/utils/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-07-13 20:36:12.000000 emtools-0.0.5/emtools/utils/pretty.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4375 2023-07-13 20:36:12.000000 emtools-0.0.5/emtools/utils/process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4022 2023-07-13 20:36:12.000000 emtools-0.0.5/emtools/utils/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3138 2023-07-13 20:36:12.000000 emtools-0.0.5/emtools/utils/system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-07-13 20:36:12.000000 emtools-0.0.5/emtools/utils/time.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:36:25.669261 emtools-0.0.5/emtools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-07-13 20:36:25.000000 emtools-0.0.5/emtools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-07-13 20:36:25.000000 emtools-0.0.5/emtools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 20:36:25.000000 emtools-0.0.5/emtools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-13 20:36:25.000000 emtools-0.0.5/emtools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-13 20:36:12.000000 emtools-0.0.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 20:36:25.673262 emtools-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2675 2023-07-13 20:36:12.000000 emtools-0.0.5/setup.py
```

### Comparing `emtools-0.0.4/LICENSE` & `emtools-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `emtools-0.0.4/emtools/__init__.py` & `emtools-0.0.5/emtools/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -20,9 +20,8 @@
 # * 02111-1307  USA
 # *
 # *  All comments concerning this program package may be sent to the
 # *  e-mail address 'delarosatrevin@scilifelab.se'
 # *
 # **************************************************************************
 
-
-__version__ = '0.0.4'
+__version__ = '0.0.5'
```

### Comparing `emtools-0.0.4/emtools/hpc/__main__.py` & `emtools-0.0.5/emtools/hpc/__main__.py`

 * *Files identical despite different names*

### Comparing `emtools-0.0.4/emtools/hpc/lsf.py` & `emtools-0.0.5/emtools/hpc/lsf.py`

 * *Files identical despite different names*

### Comparing `emtools-0.0.4/emtools/hpc/submit.py` & `emtools-0.0.5/emtools/hpc/submit.py`

 * *Files identical despite different names*

### Comparing `emtools-0.0.4/emtools/image/__init__.py` & `emtools-0.0.5/emtools/image/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -21,8 +21,11 @@
 # *
 # *  All comments concerning this program package may be sent to the
 # *  e-mail address 'delarosatrevin@scilifelab.se'
 # *
 # **************************************************************************
 
 
-from .thumbnail import Thumbnail
+from .thumbnail import Thumbnail
+
+
+__all__ = [Thumbnail]
```

### Comparing `emtools-0.0.4/emtools/image/thumbnail.py` & `emtools-0.0.5/emtools/image/thumbnail.py`

 * *Files identical despite different names*

### Comparing `emtools-0.0.4/emtools/metadata/__init__.py` & `emtools-0.0.5/emtools/processing/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,10 +10,7 @@
 # * This program is distributed in the hope that it will be useful,
 # * but WITHOUT ANY WARRANTY; without even the implied warranty of
 # * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # * GNU General Public License for more details.
 # *
 # **************************************************************************
 
-from .table import Column, ColumnList, Table
-from .starfile import StarFile
-from .epu import EPU
```

### Comparing `emtools-0.0.4/emtools/metadata/starfile.py` & `emtools-0.0.5/emtools/metadata/starfile.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,19 +17,15 @@
 # * Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA
 # * 02111-1307  USA
 # *
 # **************************************************************************
 
 __author__ = 'Jose Miguel de la Rosa Trevin, Grigory Sharov'
 
-
-import os
 import sys
-import argparse
-from collections import OrderedDict, namedtuple
 from contextlib import AbstractContextManager
 
 from .table import ColumnList, Table
 
 
 class StarFile(AbstractContextManager):
     """
@@ -131,38 +127,48 @@
         if self._singleRow:
             return 1
         else:
             return sum(1 for line in self._iterRowLines())
 
     def getTableInfo(self, tableName, **kwargs):
         """ Similar to getTable(), but it will not parse the data rows.
-        Only the colums will be read into the Table instance.
+        Only the columns will be read into the Table instance.
         """
         self.__createTable(tableName, **kwargs)
         return self._table
 
     def iterTable(self, tableName, **kwargs):
-        """ Only iterate over the table's rows and do no create
+        """ Only iterate over the table's rows and do not create
         a Table in memory to store all rows.
+        Kwargs:
+            start: starting index, first one is 0
+            limit: limit to this number of elements
         """
-        start = kwargs.get('start', 1) - 1
-        limit = kwargs.get('limit', 0)
+        start = kwargs.get('start', 0)
+        limit = kwargs.get('limit', None)
 
         self.__createTable(tableName, **kwargs)
         if self._singleRow:
             yield self.__rowFromValues(self._values)
         else:
             c = 0
             for i, line in enumerate(self._iterRowLines()):
                 if i >= start:
                     c += 1
                     yield self.__rowFromValues(line.split())
                 if limit and c == limit:
                     break
 
+    def getTableRow(self, tableName, rowIndex, **kwargs):
+        """ Get a given row by index. Extra args are passed to iterTable. """
+        kwargs['start'] = rowIndex
+        kwargs['limit'] = 1
+        for row in self.iterTable(tableName, **kwargs):
+            return row
+
     def __loadFile(self, inputFile, mode):
         return open(inputFile, mode) if isinstance(inputFile, str) else inputFile
 
     def _loadTableInfo(self, tableName):
         self._findDataLine(tableName)
 
         # Find first column line and parse all columns
@@ -270,32 +276,35 @@
 
     def close(self):
         if getattr(self, '_file', None):
             self._file.close()
             self._file = None
 
     # ---------------------- Writer functions --------------------------------
+    def writeLine(self, line):
+        self._file.write(f"{line}\n")
+
     def _writeTableName(self, tableName):
         self._file.write("\ndata_%s\n\n" % (tableName or ''))
 
     def writeSingleRow(self, tableName, row):
         self._writeTableName(tableName)
         m = max([len(c) for c in row._fields]) + 5
         format = "_{:<%d} {:>10}\n" % m
         for col, value in row._asdict().items():
             self._file.write(format.format(col, value))
         self._file.write('\n\n')
 
-    def writeHeader(self, tableName, columns):
+    def writeHeader(self, tableName, table):
         self._format = None  # clear format for writing new table
         self._writeTableName(tableName)
         self._file.write("loop_\n")
-        self._columns = columns
+        self._columns = table.getColumns()
         # Write column names
-        for col in columns:
+        for col in self._columns:
             self._file.write("_%s \n" % col.getName())
 
     def _writeRowValues(self, values):
         """ Write to file a line for these row values.
         Order should be ensured that is the same of the expected columns.
         """
         if not self._format:
@@ -336,41 +345,25 @@
             table: Table that is going to be written
             singleRow: If True, don't write loop_, just label - value pairs.
         """
         if table.size():
             if singleRow:
                 self.writeSingleRow(tableName, table[0])
             else:
-                self.writeHeader(tableName, table.getColumns())
+                self.writeHeader(tableName, table)
                 for row in table:
                     self.writeRow(row)
 
             self._writeNewline()
         else:
             # Only write the table name
             self._writeTableName(tableName)
 
 
 # --------- Helper functions  ------------------------
-def _guessType(strValue):
-    try:
-        int(strValue)
-        return int
-    except ValueError:
-        try:
-            float(strValue)
-            return float
-        except ValueError:
-            return str
-
-
-def _guessTypesFromLine(line):
-    return [_guessType(v) for v in line.split()]
-
-
 def _formatValue(v):
     return '%0.6f' % v if isinstance(v, float) else str(v)
 
 
 def _getFormatStr(v):
     return '.6f' if isinstance(v, float) else ''
```

### Comparing `emtools-0.0.4/emtools/metadata/table.py` & `emtools-0.0.5/emtools/metadata/table.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,17 +18,14 @@
 # * 02111-1307  USA
 # *
 # **************************************************************************
 
 __author__ = 'Jose Miguel de la Rosa Trevin, Grigory Sharov'
 
 
-import os
-import sys
-import argparse
 from collections import OrderedDict, namedtuple
 
 
 class Column:
     def __init__(self, name, type=None):
         self._name = name
         self._type = type or str
@@ -157,15 +154,17 @@
 
     def addRow(self, row):
         """ Add a new Row. """
         self._rows.append(row)
 
     def addRowValues(self, *args, **kwargs):
         """ Append a new Row from the given values. """
-        self._rows.append(self.Row(*args, **kwargs))
+        row = self.Row(*args, **kwargs)
+        self._rows.append(row)
+        return row
 
     def size(self):
         return len(self._rows)
 
     def addColumns(self, *args):
         """ Add one or many columns.
 
@@ -251,56 +250,22 @@
         if colName not in self._columns:
             raise Exception("Not existing column: %s" % colName)
         return [getattr(row, colName) for row in self._rows]
 
     def sort(self, key, reverse=False):
         """ Sort the table in place using the provided key.
         If key is a string, it should be the name of one column. """
-        keyFunc = lambda r: getattr(r, key) if isinstance(key, str) else key
+        def keyFunc(r):
+            return getattr(r, key) if isinstance(key, str) else key
         self._rows.sort(key=keyFunc, reverse=reverse)
 
     def print(self, formatStr=None):
         for row in self._rows:
             print(formatStr.format(**row._asdict()))
 
-    @staticmethod
-    def iterRows(fileName, key=None, reverse=False, **kwargs):
-        """
-        Convenience method to iterate over the rows of a given table.
-
-        Args:
-            fileName: the input star filename, it might contain the '@'
-                to specify the tableName
-            key: key function to sort elements, it can also be a string that
-                will be used to retrieve the value of the column with that name.
-            reverse: If true reverse the sort order.
-            **kwargs:
-                tableName: can be used explicit instead of @ in the filename.
-                types: It can be a dictionary {columnName: columnType} pairs that
-                    allows to specify types for certain columns in the internal reader
-        """
-        if '@' in fileName:
-            tableName, fileName = fileName.split('@')
-        else:
-            tableName = kwargs.pop('tableName', None)
-
-        # Create a table iterator
-        with open(fileName) as f:
-            reader = _Reader(f, tableName, **kwargs)
-            if key is None:
-                for row in reader:
-                    yield row
-            else:
-                if isinstance(key, str):
-                    keyFunc = lambda r: getattr(r, key)
-                else:
-                    keyFunc = key
-                for row in sorted(reader, key=keyFunc, reverse=reverse):
-                    yield row
-
     def __len__(self):
         return self.size()
 
     def __iter__(self):
         return iter(self._rows)
 
     def __getitem__(self, item):
@@ -320,19 +285,13 @@
         try:
             float(strValue)
             return float
         except ValueError:
             return str
 
 
-def _guessTypesFromLine(line):
-    return [_guessType(v) for v in line.split()]
-
-
 def _formatValue(v):
     return '%0.6f' % v if isinstance(v, float) else str(v)
 
 
 def _getFormatStr(v):
     return '.6f' if isinstance(v, float) else ''
-
-
```

### Comparing `emtools-0.0.4/emtools/processing/__main__.py` & `emtools-0.0.5/emtools/processing/__main__.py`

 * *Files identical despite different names*

### Comparing `emtools-0.0.4/emtools/processing/motioncor.py` & `emtools-0.0.5/emtools/processing/motioncor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 #!/usr/bin/env python
 
 import os
-import sys
 import argparse
 import threading
 from glob import glob
 from uuid import uuid4
 
-from emtools.utils import Timer, Color, Pipeline
+from emtools.utils import Timer, Pipeline
 from emtools.metadata import StarFile
 
 
 class McPipeline(Pipeline):
     """ Pipeline specific to Motioncor processing. """
     def __init__(self, generateInputFunc, gpuList, outputDir, threads=1, **kwargs):
         Pipeline.__init__(self, **kwargs)
```

### Comparing `emtools-0.0.4/emtools/pwx/__init__.py` & `emtools-0.0.5/emtools/utils/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,8 +10,20 @@
 # * This program is distributed in the hope that it will be useful,
 # * but WITHOUT ANY WARRANTY; without even the implied warranty of
 # * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # * GNU General Public License for more details.
 # *
 # **************************************************************************
 
-from .monitors import ProtocolMonitor, SetDict
+from .color import Color
+from .process import Process
+from .pretty import Pretty
+from .path import Path
+from .time import Timer
+from .pipeline import Pipeline
+from .system import System
+from .server import JsonTCPServer, JsonTCPClient
+
+
+__all__ = [Color, Process, Pretty, Path, Timer, Pipeline, System,
+           JsonTCPServer, JsonTCPClient]
+
```

### Comparing `emtools-0.0.4/emtools/pwx/monitors.py` & `emtools-0.0.5/emtools/pwx/monitors.py`

 * *Files identical despite different names*

### Comparing `emtools-0.0.4/emtools/tests/test_pipeline.py` & `emtools-0.0.5/emtools/tests/test_pipeline.py`

 * *Files 10% similar despite different names*

```diff
@@ -50,19 +50,19 @@
         pipeline = Pipeline(debug=False)
 
         g = pipeline.addGenerator(generate,
                             name='GENERATOR')
 
         f1 = pipeline.addProcessor(g.outputQueue, filter,
                              name='FILTER-1')
-        f2 = pipeline.addProcessor(g.outputQueue, filter,
-                             name='FILTER-2',
-                             outputQueue=f1.outputQueue)
-        f3 = pipeline.addProcessor(g.outputQueue, filter,
-                                   name='FILTER-3',
-                                   outputQueue=f1.outputQueue)
-        p = pipeline.addProcessor(f1.outputQueue, picking,
-                            name='PICKING')
+        pipeline.addProcessor(g.outputQueue, filter,
+                              name='FILTER-2',
+                              outputQueue=f1.outputQueue)
+        pipeline.addProcessor(g.outputQueue, filter,
+                              name='FILTER-3',
+                              outputQueue=f1.outputQueue)
+        pipeline.addProcessor(f1.outputQueue, picking,
+                              name='PICKING')
 
         pipeline.run()
 
         print("PROCESSING DONE!!!")
```

### Comparing `emtools-0.0.4/emtools/tests/test_utils.py` & `emtools-0.0.5/emtools/scripts/emt-ps.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,46 +1,52 @@
+#!/usr/bin/env python
 # **************************************************************************
 # *
-# * Authors:  J. M. de la Rosa Trevin (delarosatrevin@gmail.com)
+# * Authors:     J.M. de la Rosa Trevin (delarosatrevin@gmail.com)
 # *
 # * This program is free software; you can redistribute it and/or modify
 # * it under the terms of the GNU General Public License as published by
 # * the Free Software Foundation; either version 3 of the License, or
 # * (at your option) any later version.
 # *
 # * This program is distributed in the hope that it will be useful,
 # * but WITHOUT ANY WARRANTY; without even the implied warranty of
 # * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # * GNU General Public License for more details.
 # *
-# * You should have received a copy of the GNU General Public License
-# * along with this program; if not, write to the Free Software
-# * Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA
-# * 02111-1307  USA
-# *
-# *  All comments concerning this program package may be sent to the
-# *  e-mail address 'delarosatrevin@gmail.com'
-# *
 # **************************************************************************
 
-import unittest
-import time
-from pprint import pprint
-
-from emtools.utils import Timer, System
-
+import os
+import argparse
 
-class TestTimer(unittest.TestCase):
+from emtools.utils import Process, Color
 
-    def test_basics(self):
-        t = Timer()
-        time.sleep(1)
-        t.toc()
 
-        with Timer('Time in context:') as t2:
-            time.sleep(2)
+if __name__ == '__main__':
+    p = argparse.ArgumentParser(prog='emt-ps')
+    p.add_argument('program', default='', nargs='?',
+                   help="Program name to check running processes")
+    p.add_argument('--folder', '-f',
+                   help='Folder to check where the processes are running')
+    p.add_argument('--kill', '-k', action='store_true',
+                   help='Kill matching processes')
+    args = p.parse_args()
+
+    kill = args.kill
+    folderPath = os.path.abspath(args.folder) if args.folder else args.folder
+    print('path', folderPath)
+    processes = Process.ps(args.program, workingDir=folderPath)
+
+    color = Color.red if kill else Color.bold
+
+    for folder, procs in processes.items():
+        print(f"{Color.warn(folder)}")
+        prefix = 'Killing' if kill else ''
+        for p in procs:
+            print(f"   {p.info['username']} - {prefix} {color(p.info['name']):<30} {p.cmdline()}")
+            if kill:
+                try:
+                    p.kill()
+                except:
+                    pass
 
 
-class TestSystem(unittest.TestCase):
-    def test_gpus(self):
-        gpus = System.gpus()
-        pprint(gpus)
```

### Comparing `emtools-0.0.4/emtools/utils/__init__.py` & `emtools-0.0.5/emtools/pwx/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 # * This program is distributed in the hope that it will be useful,
 # * but WITHOUT ANY WARRANTY; without even the implied warranty of
 # * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # * GNU General Public License for more details.
 # *
 # **************************************************************************
 
-from .color import Color
-from .process import Process
-from .pretty import Pretty
-from .path import Path
-from .time import Timer
-from .pipeline import Pipeline
-from .system import System
-from .server import JsonTCPServer, JsonTCPClient
+# This emtools submodule need Scipion environment
+
+from .monitors import ProtocolMonitor, SetDict
+from .workflow import Workflow
+
+
+__all__ = [ProtocolMonitor, SetDict, Workflow]
```

### Comparing `emtools-0.0.4/emtools/utils/__main__.py` & `emtools-0.0.5/emtools/utils/__main__.py`

 * *Files identical despite different names*

### Comparing `emtools-0.0.4/emtools/utils/color.py` & `emtools-0.0.5/emtools/utils/color.py`

 * *Files identical despite different names*

### Comparing `emtools-0.0.4/emtools/utils/path.py` & `emtools-0.0.5/emtools/utils/path.py`

 * *Files 14% similar despite different names*

```diff
@@ -58,16 +58,17 @@
             return sum(v['count'] for v in self.values())
 
     @staticmethod
     def splitall(path):
         return os.path.normpath(path).split(os.path.sep)
 
     @staticmethod
-    def checkDirs(dir1, dir2, verbose=False):
-        """ Use rsync as a subprocess to check if the two directories
+    def inSync(dir1, dir2, verbose=False):
+        """ Return True if both dir1 and dir2 are synchronized (i.e. same content)
+        Use rsync as a subprocess to check if the two directories
         are synchronized. Both directories must exist.
         """
         if not dir1.endswith('/'):
             dir1 += '/'
         if not dir2.endswith('/'):
             dir2 += '/'
 
@@ -106,40 +107,73 @@
                 while rbytes := f1.read(bufsize):
                     f2.write(rbytes)
                     if sleep:
                         time.sleep(sleep)
         #Process.system(f'cp {file1} {file2}')
 
     @staticmethod
-    def copyDir(dir1, dir2, copyFileFunc=None, **kwargs):
+    def copyDir(dir1, dir2, copyFileFunc=None, pl=None, **kwargs):
         """ This is a test method to copy a whole directory and control
         the speed of the copy and how files appear in the destination.
         A custom copyFileFunc can be passed to copy files. If None,
         Path.copyFile will be used.
         **kwargs will be passed to copyFile
         """
+        pl = pl or Process
+
         _copy = copyFileFunc or Path.copyFile
 
         def _mkdir(d):
             if not os.path.exists(d):
-                Process.system(f"mkdir {d}")
+                pl.system(f"mkdir {d}")
 
         if not os.path.exists(dir1):
             raise Exception(f"Source directory must exits")
 
         _mkdir(dir2)
 
         for root, dirs, files in os.walk(dir1):
             root2 = root.replace(dir1, dir2)
             for d in dirs:
                 _mkdir(os.path.join(root2, d))
             for f in files:
                 _copy(os.path.join(root, f), os.path.join(root2, f), **kwargs)
 
 
+    @staticmethod
+    def replaceExt(filename, newExt):
+        """ Replace the current path extension(from last .)
+        with a new one. The new one should not contains the ."""
+        return Path.removeExt(filename) + '.' + newExt
+
+    @staticmethod
+    def replaceBaseExt(filename, newExt):
+        """ Replace the current basename extension(from last .)
+        with a new one. The new one should not contains the .
+        """
+        return Path.replaceExt(os.path.basename(filename), newExt)
+
+    @staticmethod
+    def removeBaseExt(filename):
+        """Take the basename of the filename and remove extension"""
+        return Path.removeExt(os.path.basename(filename))
+
+    @staticmethod
+    def removeExt(filename):
+        """ Remove extension from basename """
+        return os.path.splitext(filename)[0]
+
+    @staticmethod
+    def exists(path):
+        """ Just avoid empty or None path to raise exception
+        from os.path.exists.
+        """
+        return path and os.path.exists(path)
+
+
 class Main:
     @staticmethod
     def add_arguments(parser):
         g = parser.add_mutually_exclusive_group()
         g.add_argument('--stats', metavar='PATTERN_OR_FOLDER',
                        help="Statistics of some files given a pattern or from "
                             "a folder.")
@@ -167,15 +201,15 @@
             if os.path.exists(pattern) and os.path.isdir(pattern):
                 statsDir(pattern, args.sort)
             else:
                 stats(pattern, args.bin, args.plot)
         elif dirs := args.copy_dir:
             Path.copyDir(dirs[0], dirs[1], sleep=args.delay)
         elif dirs := args.check_dirs:
-            sync = Path.checkDirs(dirs[0], dirs[1], verbose=True)
+            sync = Path.inSync(dirs[0], dirs[1], verbose=True)
             s = Color.green('in SYNC') if sync else Color.red('NOT in SYNC')
             print(f"Dirs are {s}")
 
 
 def statsDir(folder, sort):
     folders = 0
     ed = Path.ExtDict()
@@ -265,15 +299,15 @@
                 last_date = start
             else:
                 labels.append('')
         _addDt(bins[-1])
         values = [b['count'] for b in bins]
         fig, ax = plt.subplots(figsize=(24, 8))
         w = width * 0.9
-        rects1 = ax.bar(x + w / 2, values, w, label='Men')
+        ax.bar(x + w / 2, values, w, label='Men')
         # Add some text for labels, title and custom x-axis tick labels, etc.
         ax.set_ylabel('Files')
         ax.set_title(f'Files generated every {bin} minutes')
         ax.set_xticks(x)
         ax.set_xticklabels(labels)
         last_i = None
         annot = ax.annotate("", xy=(0, 0), xytext=(5, 5), textcoords="offset points")
```

### Comparing `emtools-0.0.4/emtools/utils/pipeline.py` & `emtools-0.0.5/emtools/utils/pipeline.py`

 * *Files identical despite different names*

### Comparing `emtools-0.0.4/emtools/utils/pretty.py` & `emtools-0.0.5/emtools/utils/pretty.py`

 * *Files identical despite different names*

### Comparing `emtools-0.0.4/emtools/utils/server.py` & `emtools-0.0.5/emtools/utils/server.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,23 +12,20 @@
 # * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # * GNU General Public License for more details.
 # *
 # **************************************************************************
 
 import sys
 import json
-import time
+from datetime import datetime
 import traceback
-import threading
 import socket
 from socketserver import BaseRequestHandler, ThreadingTCPServer
-from datetime import datetime
 
 from .pretty import Pretty
-from .color import Color
 
 
 def send_object(s, obj):
     """ Send an object serialized as json. """
     objstr = json.dumps(obj)
     return s.sendall(bytes(objstr, encoding='utf-8'))
 
@@ -64,15 +61,15 @@
             method = obj['method']
             args = obj.get('args', [])
             kwargs = obj.get('kwargs', {})
             function = getattr(self.server, method)
             result = function(*args, **kwargs) or {}
             r = {'result': result}
         except Exception as e:
-
+            print(e)
             print(traceback.format_exc())
             r = {'error': 'Wrong input object'}
         send_object(self.request, r)
 
 
 class JsonTCPServer(ThreadingTCPServer):
     def __init__(self, address):
```

### Comparing `emtools-0.0.4/emtools/utils/system.py` & `emtools-0.0.5/emtools/utils/system.py`

 * *Files 24% similar despite different names*

```diff
@@ -16,43 +16,72 @@
 
 """
 index, name, driver_version, temperature.gpu, utilization.gpu [%], utilization.memory [%], memory.total [MiB], memory.used [MiB]
 0, NVIDIA GeForce RTX 3090, 515.65.01, 42, 1 %, 13 %, 24576 MiB, 963 MiB
 1, NVIDIA GeForce RTX 3090, 515.65.01, 37, 0 %, 0 %, 24576 MiB, 1 MiB
 """
 
+import socket
+import platform
 from .process import Process
 
 
 class System:
     NVIDIA_SMI_QUERY = ['nvidia-smi', '--query-gpu=index,name,driver_version,'
                         'temperature.gpu,utilization.gpu,utilization.memory,'
                         'memory.total,memory.used', '--format=csv']
 
     @staticmethod
     def gpus():
-        query = Process(System.NVIDIA_SMI_QUERY[0],
-                        *System.NVIDIA_SMI_QUERY[1:])
         gpus = []
-        for i, line in enumerate(query.lines()):
-            # Use first line as keywords since it is the header
-            if line.strip():
-                if i == 0:
-                    keys = line.split(',')
-                else:
-                    values = line.split(',')
-                    gpus.append({k.strip().split()[0]: v.strip()
-                                 for k, v in zip(keys, values)})
-                print(i)
+        query = Process(System.NVIDIA_SMI_QUERY[0],
+                        *System.NVIDIA_SMI_QUERY[1:], doRaise=False)
+
+        if query.returncode == 0:   # no error
+            for i, line in enumerate(query.lines()):
+                # Use first line as keywords since it is the header
+                if line.strip():
+                    if i == 0:
+                        keys = line.split(',')
+                    else:
+                        values = line.split(',')
+                        gpus.append({k.strip().split()[0]: v.strip()
+                                     for k, v in zip(keys, values)})
         return gpus
 
     @staticmethod
     def cpus():
         """ Return number of CPUs in the system, None if can't figure it out."""
-        lscpu = Process('lscpu')
-        cpus = None
+        system = platform.system()
+        cpus = 0
 
-        for line in lscpu.lines():
-            if line.startswith('CPU(s):'):
-                cpus = int(line.split()[1].strip())
+        if system == 'Linux':
+            for line in Process('lscpu').lines():
+                if line.startswith('CPU(s):'):
+                    cpus = int(line.split()[1].strip())
+
+        elif system == 'Darwin':
+            for line in Process('sysctl', '-a').lines():
+                if line.startswith('hw.ncpu:'):
+                    cpus = int(line.split()[1])
 
         return cpus
+
+    @staticmethod
+    def specs():
+        """ Make an informative summary of the system specs. """
+        gpuDict = {}
+        for gpu in System.gpus():
+            name = gpu['name']
+            if name not in gpuDict:
+                gpuDict[name] = {
+                    'count': 1,
+                    'memory': gpu['memory.total']
+                }
+            else:
+                gpuDict[name]['count'] += 1
+        return {'CPUs': System.cpus(),
+                'GPUs': gpuDict}
+
+    @staticmethod
+    def hostname():
+        return socket.gethostname()
```

### Comparing `emtools-0.0.4/emtools/utils/time.py` & `emtools-0.0.5/emtools/utils/time.py`

 * *Files 15% similar despite different names*

```diff
@@ -18,28 +18,34 @@
 
 from .pretty import Pretty
 
 
 class Timer(object):
     """ Simple Timer base in datetime.now and timedelta. """
 
-    def __init__(self, message=""):
-        self._message = message
+    def __init__(self, message="Elapsed:"):
+        self.message = message
         self.tic()
 
     def tic(self):
         self._dt = datetime.now()
 
     def getElapsedTime(self):
         return datetime.now() - self._dt
 
-    def toc(self, message='Elapsed:'):
-        print(f"{message} {str(self.getElapsedTime())}")
+    def toc(self, message=None, pretty=False):
+        print(self.getToc(message=message, pretty=pretty))
 
-    def getToc(self):
-        return Pretty.delta(self.getElapsedTime())
+    def getToc(self, message=None, pretty=False):
+        if message:
+            self.message = message
+
+        elapsed = self.getElapsedTime()
+        elapsedStr = Pretty.delta(elapsed) if pretty else str(elapsed)
+
+        return f"{self.message} {elapsedStr}"
 
     def __enter__(self):
         return self
 
     def __exit__(self, type, value, traceback):
-        self.toc(self._message)
+        self.toc(self.message)
```

### Comparing `emtools-0.0.4/emtools.egg-info/SOURCES.txt` & `emtools-0.0.5/emtools.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -13,21 +13,32 @@
 emtools/hpc/__main__.py
 emtools/hpc/lsf.py
 emtools/hpc/submit.py
 emtools/image/__init__.py
 emtools/image/thumbnail.py
 emtools/metadata/__init__.py
 emtools/metadata/epu.py
+emtools/metadata/misc.py
+emtools/metadata/sqlite.py
 emtools/metadata/starfile.py
 emtools/metadata/table.py
 emtools/processing/__init__.py
 emtools/processing/__main__.py
 emtools/processing/motioncor.py
 emtools/pwx/__init__.py
 emtools/pwx/monitors.py
+emtools/pwx/workflow.py
+emtools/scripts/__init__.py
+emtools/scripts/emt-beamshifts.py
+emtools/scripts/emt-change-optics.py
+emtools/scripts/emt-epu-parse.py
+emtools/scripts/emt-files.py
+emtools/scripts/emt-frames.py
+emtools/scripts/emt-ps.py
+emtools/scripts/emt-scipion-otf.py
 emtools/tests/__init__.py
 emtools/tests/test_metadata.py
 emtools/tests/test_pipeline.py
 emtools/tests/test_utils.py
 emtools/utils/__init__.py
 emtools/utils/__main__.py
 emtools/utils/color.py
```

### Comparing `emtools-0.0.4/setup.py` & `emtools-0.0.5/setup.py`

 * *Files identical despite different names*

