# Comparing `tmp/py_ballisticcalc-1.0.4.tar.gz` & `tmp/py_ballisticcalc-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_ballisticcalc-1.0.4.tar", last modified: Wed Jul  6 06:59:35 2022, max compression
+gzip compressed data, was "py_ballisticcalc-1.0.9.tar", last modified: Thu Sep  1 19:54:35 2022, max compression
```

## Comparing `py_ballisticcalc-1.0.4.tar` & `py_ballisticcalc-1.0.9.tar`

### file list

```diff
@@ -1,52 +1,64 @@
-drwxrwxrwx   0        0        0        0 2022-07-06 06:59:34.999605 py_ballisticcalc-1.0.4/
--rw-rw-rw-   0        0        0     7817 2022-06-30 10:48:36.000000 py_ballisticcalc-1.0.4/LICENSE
--rw-rw-rw-   0        0        0     7440 2022-07-06 06:59:34.998604 py_ballisticcalc-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     7046 2022-07-06 06:46:08.000000 py_ballisticcalc-1.0.4/README.md
-drwxrwxrwx   0        0        0        0 2022-07-06 06:59:34.923950 py_ballisticcalc-1.0.4/py_ballisticcalc/
--rw-rw-rw-   0        0        0      259 2022-07-06 06:59:18.000000 py_ballisticcalc-1.0.4/py_ballisticcalc/__init__.py
--rw-rw-rw-   0        0        0     6300 2022-07-04 07:01:41.000000 py_ballisticcalc-1.0.4/py_ballisticcalc/atmosphere.py
-drwxrwxrwx   0        0        0        0 2022-07-06 06:59:34.947636 py_ballisticcalc-1.0.4/py_ballisticcalc/bmath/
--rw-rw-rw-   0        0        0       49 2022-06-30 10:48:36.000000 py_ballisticcalc-1.0.4/py_ballisticcalc/bmath/__init__.py
-drwxrwxrwx   0        0        0        0 2022-07-06 06:59:34.969626 py_ballisticcalc-1.0.4/py_ballisticcalc/bmath/unit/
--rw-rw-rw-   0        0        0      173 2022-06-30 10:48:36.000000 py_ballisticcalc-1.0.4/py_ballisticcalc/bmath/unit/__init__.py
--rw-rw-rw-   0        0        0     1914 2022-07-05 10:13:24.000000 py_ballisticcalc-1.0.4/py_ballisticcalc/bmath/unit/angular.py
--rw-rw-rw-   0        0        0     3650 2022-06-30 11:35:01.000000 py_ballisticcalc-1.0.4/py_ballisticcalc/bmath/unit/convertor.py
--rw-rw-rw-   0        0        0     2134 2022-06-30 10:48:36.000000 py_ballisticcalc-1.0.4/py_ballisticcalc/bmath/unit/distance.py
--rw-rw-rw-   0        0        0      623 2022-06-30 10:48:36.000000 py_ballisticcalc-1.0.4/py_ballisticcalc/bmath/unit/energy.py
--rw-rw-rw-   0        0        0     1169 2022-06-30 10:48:36.000000 py_ballisticcalc-1.0.4/py_ballisticcalc/bmath/unit/pressure.py
--rw-rw-rw-   0        0        0     1117 2022-06-30 10:48:36.000000 py_ballisticcalc-1.0.4/py_ballisticcalc/bmath/unit/temperature.py
--rw-rw-rw-   0        0        0     3862 2022-06-30 10:48:36.000000 py_ballisticcalc-1.0.4/py_ballisticcalc/bmath/unit/unit_test.py
--rw-rw-rw-   0        0        0     1133 2022-06-30 10:48:36.000000 py_ballisticcalc-1.0.4/py_ballisticcalc/bmath/unit/velocity.py
--rw-rw-rw-   0        0        0     2609 2022-06-30 10:48:36.000000 py_ballisticcalc-1.0.4/py_ballisticcalc/bmath/unit/weight.py
-drwxrwxrwx   0        0        0        0 2022-07-06 06:59:34.977619 py_ballisticcalc-1.0.4/py_ballisticcalc/bmath/vector/
--rw-rw-rw-   0        0        0       28 2022-06-30 10:48:36.000000 py_ballisticcalc-1.0.4/py_ballisticcalc/bmath/vector/__init__.py
--rw-rw-rw-   0        0        0     2789 2022-06-30 10:48:36.000000 py_ballisticcalc-1.0.4/py_ballisticcalc/bmath/vector/vector.py
--rw-rw-rw-   0        0        0     1502 2022-06-30 10:48:36.000000 py_ballisticcalc-1.0.4/py_ballisticcalc/bmath/vector/vector_test.py
--rw-rw-rw-   0        0        0    27645 2022-07-04 08:14:35.000000 py_ballisticcalc-1.0.4/py_ballisticcalc/drag.py
-drwxrwxrwx   0        0        0        0 2022-07-06 06:59:34.988613 py_ballisticcalc-1.0.4/py_ballisticcalc/extended/
--rw-rw-rw-   0        0        0      178 2022-07-04 12:41:43.000000 py_ballisticcalc-1.0.4/py_ballisticcalc/extended/__init__.py
--rw-rw-rw-   0        0        0     4736 2022-07-05 09:12:58.000000 py_ballisticcalc-1.0.4/py_ballisticcalc/extended/drag_extended.py
--rw-rw-rw-   0        0        0     3157 2022-07-06 06:49:09.000000 py_ballisticcalc-1.0.4/py_ballisticcalc/extended/extended_test.py
--rw-rw-rw-   0        0        0     5822 2022-07-06 06:21:08.000000 py_ballisticcalc-1.0.4/py_ballisticcalc/extended/multiple_ballistic_coefficient.py
--rw-rw-rw-   0        0        0     5148 2022-07-06 06:21:08.000000 py_ballisticcalc-1.0.4/py_ballisticcalc/extended/profile_extended.py
--rw-rw-rw-   0        0        0     5337 2022-07-05 12:59:44.000000 py_ballisticcalc-1.0.4/py_ballisticcalc/profile.py
--rw-rw-rw-   0        0        0     3415 2022-07-04 08:10:36.000000 py_ballisticcalc-1.0.4/py_ballisticcalc/projectile.py
--rw-rw-rw-   0        0        0     7532 2022-06-30 10:48:36.000000 py_ballisticcalc-1.0.4/py_ballisticcalc/py_ballisticcalc_test.py
--rw-rw-rw-   0        0        0     2107 2022-06-30 10:48:36.000000 py_ballisticcalc-1.0.4/py_ballisticcalc/shot_parameters.py
-drwxrwxrwx   0        0        0        0 2022-07-06 06:59:34.995607 py_ballisticcalc-1.0.4/py_ballisticcalc/tools/
--rw-rw-rw-   0        0        0      123 2022-07-06 06:21:08.000000 py_ballisticcalc-1.0.4/py_ballisticcalc/tools/__init__.py
--rw-rw-rw-   0        0        0     3112 2022-07-06 06:21:08.000000 py_ballisticcalc-1.0.4/py_ballisticcalc/tools/cramer_speed_of_sound.py
--rw-rw-rw-   0        0        0     8516 2022-07-06 06:21:08.000000 py_ballisticcalc-1.0.4/py_ballisticcalc/tools/pejsa_trajectory_calculator.py
--rw-rw-rw-   0        0        0      864 2022-07-06 06:21:08.000000 py_ballisticcalc-1.0.4/py_ballisticcalc/tools/tools_test.py
--rw-rw-rw-   0        0        0    13964 2022-07-04 07:01:41.000000 py_ballisticcalc-1.0.4/py_ballisticcalc/trajectory_calculator.py
--rw-rw-rw-   0        0        0     4056 2022-06-30 10:48:36.000000 py_ballisticcalc-1.0.4/py_ballisticcalc/trajectory_data.py
--rw-rw-rw-   0        0        0     6794 2022-06-30 10:48:36.000000 py_ballisticcalc-1.0.4/py_ballisticcalc/weapon.py
--rw-rw-rw-   0        0        0     3128 2022-06-30 10:53:05.000000 py_ballisticcalc-1.0.4/py_ballisticcalc/wind.py
-drwxrwxrwx   0        0        0        0 2022-07-06 06:59:34.945637 py_ballisticcalc-1.0.4/py_ballisticcalc.egg-info/
--rw-rw-rw-   0        0        0     7440 2022-07-06 06:59:33.000000 py_ballisticcalc-1.0.4/py_ballisticcalc.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1539 2022-07-06 06:59:34.000000 py_ballisticcalc-1.0.4/py_ballisticcalc.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-07-06 06:59:33.000000 py_ballisticcalc-1.0.4/py_ballisticcalc.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2022-07-06 06:59:34.000000 py_ballisticcalc-1.0.4/py_ballisticcalc.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2022-07-06 06:59:33.000000 py_ballisticcalc-1.0.4/py_ballisticcalc.egg-info/zip-safe
--rw-rw-rw-   0        0        0       42 2022-07-06 06:59:35.000604 py_ballisticcalc-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0      717 2022-06-30 10:48:36.000000 py_ballisticcalc-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2022-09-01 19:54:35.415370 py_ballisticcalc-1.0.9/
+-rw-rw-rw-   0        0        0     7817 2022-06-30 20:14:12.000000 py_ballisticcalc-1.0.9/LICENSE
+-rw-rw-rw-   0        0        0       40 2022-09-01 19:32:07.000000 py_ballisticcalc-1.0.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     7730 2022-09-01 19:54:35.415370 py_ballisticcalc-1.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     7313 2022-08-12 18:58:30.000000 py_ballisticcalc-1.0.9/README.md
+drwxrwxrwx   0        0        0        0 2022-09-01 19:54:35.149763 py_ballisticcalc-1.0.9/py_ballisticcalc/
+-rw-rw-rw-   0        0        0    20480 2022-09-01 19:45:18.000000 py_ballisticcalc-1.0.9/py_ballisticcalc/__init__.cp39-win_amd64.pyd
+-rw-rw-rw-   0        0        0      296 2022-09-01 19:37:15.000000 py_ballisticcalc-1.0.9/py_ballisticcalc/__init__.py
+-rw-rw-rw-   0        0        0   565470 2022-09-01 19:31:18.000000 py_ballisticcalc-1.0.9/py_ballisticcalc/atmosphere.c
+-rw-rw-rw-   0        0        0    92160 2022-09-01 19:50:42.000000 py_ballisticcalc-1.0.9/py_ballisticcalc/atmosphere.cp39-win_amd64.pyd
+-rw-rw-rw-   0        0        0    15883 2022-09-01 19:27:15.000000 py_ballisticcalc-1.0.9/py_ballisticcalc/bin_test.py
+drwxrwxrwx   0        0        0        0 2022-09-01 19:54:35.196636 py_ballisticcalc-1.0.9/py_ballisticcalc/bmath/
+-rw-rw-rw-   0        0        0       44 2022-09-01 19:27:15.000000 py_ballisticcalc-1.0.9/py_ballisticcalc/bmath/__init__.py
+drwxrwxrwx   0        0        0        0 2022-09-01 19:54:35.384121 py_ballisticcalc-1.0.9/py_ballisticcalc/bmath/unit/
+-rw-rw-rw-   0        0        0    22016 2022-09-01 19:45:19.000000 py_ballisticcalc-1.0.9/py_ballisticcalc/bmath/unit/__init__.cp39-win_amd64.pyd
+-rw-rw-rw-   0        0        0      173 2022-09-01 19:27:15.000000 py_ballisticcalc-1.0.9/py_ballisticcalc/bmath/unit/__init__.py
+-rw-rw-rw-   0        0        0   454073 2022-09-01 19:31:16.000000 py_ballisticcalc-1.0.9/py_ballisticcalc/bmath/unit/angular.c
+-rw-rw-rw-   0        0        0    69632 2022-09-01 19:51:03.000000 py_ballisticcalc-1.0.9/py_ballisticcalc/bmath/unit/angular.cp39-win_amd64.pyd
+-rw-rw-rw-   0        0        0   466575 2022-09-01 19:31:16.000000 py_ballisticcalc-1.0.9/py_ballisticcalc/bmath/unit/distance.c
+-rw-rw-rw-   0        0        0    71680 2022-09-01 19:51:05.000000 py_ballisticcalc-1.0.9/py_ballisticcalc/bmath/unit/distance.cp39-win_amd64.pyd
+-rw-rw-rw-   0        0        0   413689 2022-09-01 19:31:16.000000 py_ballisticcalc-1.0.9/py_ballisticcalc/bmath/unit/energy.c
+-rw-rw-rw-   0        0        0    64000 2022-09-01 19:51:06.000000 py_ballisticcalc-1.0.9/py_ballisticcalc/bmath/unit/energy.cp39-win_amd64.pyd
+-rw-rw-rw-   0        0        0   434628 2022-09-01 19:31:16.000000 py_ballisticcalc-1.0.9/py_ballisticcalc/bmath/unit/pressure.c
+-rw-rw-rw-   0        0        0    67072 2022-09-01 19:51:07.000000 py_ballisticcalc-1.0.9/py_ballisticcalc/bmath/unit/pressure.cp39-win_amd64.pyd
+-rw-rw-rw-   0        0        0   432651 2022-09-01 19:31:16.000000 py_ballisticcalc-1.0.9/py_ballisticcalc/bmath/unit/temperature.c
+-rw-rw-rw-   0        0        0    66560 2022-09-01 19:51:09.000000 py_ballisticcalc-1.0.9/py_ballisticcalc/bmath/unit/temperature.cp39-win_amd64.pyd
+-rw-rw-rw-   0        0        0     3563 2022-09-01 19:27:15.000000 py_ballisticcalc-1.0.9/py_ballisticcalc/bmath/unit/unit_test.py
+-rw-rw-rw-   0        0        0   434101 2022-09-01 19:31:17.000000 py_ballisticcalc-1.0.9/py_ballisticcalc/bmath/unit/velocity.c
+-rw-rw-rw-   0        0        0    67072 2022-09-01 19:51:10.000000 py_ballisticcalc-1.0.9/py_ballisticcalc/bmath/unit/velocity.cp39-win_amd64.pyd
+-rw-rw-rw-   0        0        0   438572 2022-09-01 19:31:17.000000 py_ballisticcalc-1.0.9/py_ballisticcalc/bmath/unit/weight.c
+-rw-rw-rw-   0        0        0    68096 2022-09-01 19:51:11.000000 py_ballisticcalc-1.0.9/py_ballisticcalc/bmath/unit/weight.cp39-win_amd64.pyd
+drwxrwxrwx   0        0        0        0 2022-09-01 19:54:35.415370 py_ballisticcalc-1.0.9/py_ballisticcalc/bmath/vector/
+-rw-rw-rw-   0        0        0    20992 2022-09-01 19:45:19.000000 py_ballisticcalc-1.0.9/py_ballisticcalc/bmath/vector/__init__.cp39-win_amd64.pyd
+-rw-rw-rw-   0        0        0       23 2022-09-01 19:27:15.000000 py_ballisticcalc-1.0.9/py_ballisticcalc/bmath/vector/__init__.py
+-rw-rw-rw-   0        0        0   476301 2022-09-01 19:31:17.000000 py_ballisticcalc-1.0.9/py_ballisticcalc/bmath/vector/vector.c
+-rw-rw-rw-   0        0        0    72192 2022-09-01 19:51:12.000000 py_ballisticcalc-1.0.9/py_ballisticcalc/bmath/vector/vector.cp39-win_amd64.pyd
+-rw-rw-rw-   0        0        0     2198 2022-09-01 19:27:15.000000 py_ballisticcalc-1.0.9/py_ballisticcalc/bmath/vector/vectot_test.py
+-rw-rw-rw-   0        0        0   796985 2022-09-01 19:31:18.000000 py_ballisticcalc-1.0.9/py_ballisticcalc/drag.c
+-rw-rw-rw-   0        0        0   127488 2022-09-01 19:50:45.000000 py_ballisticcalc-1.0.9/py_ballisticcalc/drag.cp39-win_amd64.pyd
+-rw-rw-rw-   0        0        0    20123 2022-09-01 19:27:15.000000 py_ballisticcalc-1.0.9/py_ballisticcalc/drag_tables.py
+-rw-rw-rw-   0        0        0   595993 2022-09-01 19:31:19.000000 py_ballisticcalc-1.0.9/py_ballisticcalc/multiple_bc.c
+-rw-rw-rw-   0        0        0    98816 2022-09-01 19:50:47.000000 py_ballisticcalc-1.0.9/py_ballisticcalc/multiple_bc.cp39-win_amd64.pyd
+-rw-rw-rw-   0        0        0  1126644 2022-09-01 19:31:20.000000 py_ballisticcalc-1.0.9/py_ballisticcalc/profile.c
+-rw-rw-rw-   0        0        0   177152 2022-09-01 19:50:51.000000 py_ballisticcalc-1.0.9/py_ballisticcalc/profile.cp39-win_amd64.pyd
+-rw-rw-rw-   0        0        0   545967 2022-09-01 19:31:21.000000 py_ballisticcalc-1.0.9/py_ballisticcalc/projectile.c
+-rw-rw-rw-   0        0        0    80896 2022-09-01 19:50:52.000000 py_ballisticcalc-1.0.9/py_ballisticcalc/projectile.cp39-win_amd64.pyd
+-rw-rw-rw-   0        0        0   467748 2022-09-01 19:31:21.000000 py_ballisticcalc-1.0.9/py_ballisticcalc/shot_parameters.c
+-rw-rw-rw-   0        0        0    71680 2022-09-01 19:50:53.000000 py_ballisticcalc-1.0.9/py_ballisticcalc/shot_parameters.cp39-win_amd64.pyd
+-rw-rw-rw-   0        0        0   740036 2022-09-01 19:31:21.000000 py_ballisticcalc-1.0.9/py_ballisticcalc/trajectory_calculator.c
+-rw-rw-rw-   0        0        0   137216 2022-09-01 19:50:58.000000 py_ballisticcalc-1.0.9/py_ballisticcalc/trajectory_calculator.cp39-win_amd64.pyd
+-rw-rw-rw-   0        0        0   550566 2022-09-01 19:31:22.000000 py_ballisticcalc-1.0.9/py_ballisticcalc/trajectory_data.c
+-rw-rw-rw-   0        0        0    82432 2022-09-01 19:50:59.000000 py_ballisticcalc-1.0.9/py_ballisticcalc/trajectory_data.cp39-win_amd64.pyd
+-rw-rw-rw-   0        0        0   953531 2022-09-01 19:31:22.000000 py_ballisticcalc-1.0.9/py_ballisticcalc/weapon.c
+-rw-rw-rw-   0        0        0   133632 2022-09-01 19:51:01.000000 py_ballisticcalc-1.0.9/py_ballisticcalc/weapon.cp39-win_amd64.pyd
+-rw-rw-rw-   0        0        0   401975 2022-09-01 19:31:23.000000 py_ballisticcalc-1.0.9/py_ballisticcalc/wind.c
+-rw-rw-rw-   0        0        0    62976 2022-09-01 19:51:02.000000 py_ballisticcalc-1.0.9/py_ballisticcalc/wind.cp39-win_amd64.pyd
+drwxrwxrwx   0        0        0        0 2022-09-01 19:54:35.165385 py_ballisticcalc-1.0.9/py_ballisticcalc.egg-info/
+-rw-rw-rw-   0        0        0     7730 2022-09-01 19:54:34.000000 py_ballisticcalc-1.0.9/py_ballisticcalc.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2527 2022-09-01 19:54:34.000000 py_ballisticcalc-1.0.9/py_ballisticcalc.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-09-01 19:54:34.000000 py_ballisticcalc-1.0.9/py_ballisticcalc.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2022-09-01 19:54:34.000000 py_ballisticcalc-1.0.9/py_ballisticcalc.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2022-09-01 19:51:39.000000 py_ballisticcalc-1.0.9/py_ballisticcalc.egg-info/zip-safe
+-rw-rw-rw-   0        0        0       42 2022-09-01 19:54:35.415370 py_ballisticcalc-1.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1226 2022-09-01 19:51:37.000000 py_ballisticcalc-1.0.9/setup.py
```

### Comparing `py_ballisticcalc-1.0.4/LICENSE` & `py_ballisticcalc-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `py_ballisticcalc-1.0.4/PKG-INFO` & `py_ballisticcalc-1.0.9/py_ballisticcalc.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,42 @@
 Metadata-Version: 2.1
-Name: py_ballisticcalc
-Version: 1.0.4
+Name: py-ballisticcalc
+Version: 1.0.9
 Summary: LGPL library for small arms ballistic calculations (Python 3)
 Home-page: https://github.com/o-murphy/py_ballisticcalc
-Download-URL: http://pypi.python.org/pypi/py_ballisticcalc/
 Author: o-murphy
 Author-email: thehelixpg@gmail.com
 License: LGPL-3.0
+Download-URL: http://pypi.python.org/pypi/py_ballisticcalc/
+Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # BallisticCalculator
 LGPL library for small arms ballistic calculations (Python 3)
 
 Installation
 ------------
 **Stable release from pypi**
+(Contains c-extensions which offer higher performance)
 ```commandline
 pip install py-ballisticcalc
 ```
-**Latest release, may contain some issues**
+**Latest (only pure python) release, may contain some issues**
 ```commandline
 pip install git+https://github.com/o-murphy/py_ballisticcalc
 ```    
 
+**Also use `git clone` to build your own package**
+(Contains cython files to build your own c-extensions)
+```commandline
+git clone https://github.com/o-murphy/py_ballisticcalc
+```   
+
+
 Usage
 -----
 
 ### Simple start
 ```python
 from py_ballisticcalc.profile import Profile
 from py_ballisticcalc.bmath import unit
@@ -169,7 +178,9 @@
 The current status of the project is ALPHA version.
 
 RISK NOTICE
 
 The library performs very limited simulation of a complex physical process and so it performs a lot of approximations. Therefore the calculation results MUST NOT be considered as completely and reliably reflecting actual behavior or characteristics of projectiles. While these results may be used for educational purpose, they must NOT be considered as reliable for the areas where incorrect calculation may cause making a wrong decision, financial harm, or can put a human life at risk.
 
 THE CODE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE MATERIALS OR THE USE OR OTHER DEALINGS IN THE MATERIALS.
+
+
```

### Comparing `py_ballisticcalc-1.0.4/README.md` & `py_ballisticcalc-1.0.9/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,29 @@
 # BallisticCalculator
 LGPL library for small arms ballistic calculations (Python 3)
 
 Installation
 ------------
 **Stable release from pypi**
+(Contains c-extensions which offer higher performance)
 ```commandline
 pip install py-ballisticcalc
 ```
-**Latest release, may contain some issues**
+**Latest (only pure python) release, may contain some issues**
 ```commandline
 pip install git+https://github.com/o-murphy/py_ballisticcalc
 ```    
 
+**Also use `git clone` to build your own package**
+(Contains cython files to build your own c-extensions)
+```commandline
+git clone https://github.com/o-murphy/py_ballisticcalc
+```   
+
+
 Usage
 -----
 
 ### Simple start
 ```python
 from py_ballisticcalc.profile import Profile
 from py_ballisticcalc.bmath import unit
```

### Comparing `py_ballisticcalc-1.0.4/py_ballisticcalc/bmath/vector/vector_test.py` & `py_ballisticcalc-1.0.9/py_ballisticcalc/bmath/vector/vectot_test.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,49 +1,75 @@
-import math
+import timeit
 import unittest
-from py_ballisticcalc.bmath import Vector
+import pyximport
+import math
+pyximport.install()
+from py_ballisticcalc.bmath.vector import Vector
+
+
+class TestVector(unittest.TestCase):
+
+    def test_create(self):
+        v = Vector(1, 2, 3)
+        mag = v.magnitude()
+        mc = v.multiply_by_const(10)
+
+        b = Vector(1, 2, 3)
+        mv = v.multiply_by_vector(b)
+        a = v.add(b)
+        s = v.subtract(b)
+        neg = v.negate()
+        norm = v.normalize()
+        # print('\n'.join([str(i) for i in [mag, mc, mv, a, s, neg, norm]]))
+        x = v.x
+
+    # @unittest.SkipTest
+    def test_time(self):
+        t = timeit.timeit(self.test_create, number=50000)
+        print(t)
 
 
 class TestVectorCreation(unittest.TestCase):
 
     def test_create(self):
         v = Vector(1, 2, 3)
 
         self.assertTrue(v.x == 1 and v.y == 2 and v.z == 3, "Create failed")
 
-        c = v.__copy__()
+        c = v.copy()
         self.assertTrue(c.x == 1 and c.y == 2 and c.z == 3, "Copy failed")
 
 
 class TestUnary(unittest.TestCase):
 
     def test_unary(self):
         v1 = Vector(1, 2, 3)
 
         self.assertFalse(math.fabs(v1.magnitude() - 3.74165738677) > 1e-7, "Magnitude failed")
 
         v2 = v1.negate()
-        self.assertTrue(v2.x == -1 and v2.y == -2 and v2.z == -3, "Negate failed")
+        self.assertTrue(v2.x() == -1.0 and v2.y() == -2.0 and v2.z() == -3.0, "Negate failed")
 
         v2 = v1.normalize()
-        self.assertFalse(v2.x > 1 or v2.y > 1 or v2.z > 1, "Normalize failed")
+        self.assertFalse(v2.x() > 1.0 or v2.y() > 1.0 or v2.z() > 1.0, "Normalize failed")
 
         v1 = Vector(0, 0, 0)
         v2 = v1.normalize()
-        self.assertFalse(v2.x != 0 or v2.y != 0 or v2.z != 0, "Normalize failed")
+
+        self.assertFalse(v2.x() != 0.0 or v2.y() != 0.0 or v2.z() != 0.0, "Normalize failed")
 
 
 class TestBinary(unittest.TestCase):
 
     def test_binary(self):
         v1 = Vector(1, 2, 3)
 
-        v2 = v1.add(v1.__copy__())
-        self.assertFalse(v2.x != 2 or v2.y != 4 or v2.z != 6, "Add failed")
+        v2 = v1.add(v1.copy())
+        self.assertFalse(v2.x() != 2.0 or v2.y() != 4.0 or v2.z() != 6.0, "Add failed")
 
         v2 = v1.subtract(v2)
-        self.assertFalse(v2.x != -1 or v2.y != -2 or v2.z != -3, "Subtract failed")
+        self.assertFalse(v2.x() != -1.0 or v2.y() != -2.0 or v2.z() != -3.0, "Subtract failed")
 
-        self.assertFalse(v1.multiply_by_vector(v1.__copy__()) != (1 + 4 + 9), "MultiplyByVector failed")
+        self.assertFalse(v1.multiply_by_vector(v1.copy()) != float(1 + 4 + 9), "MultiplyByVector failed")
 
         v2 = v1.multiply_by_const(3)
-        self.assertFalse(v2.x != 3 or v2.y != 6 or v2.z != 9, "MultiplyByConst failed")
+        self.assertFalse(v2.x() != 3.0 or v2.y() != 6.0 or v2.z() != 9.0, "MultiplyByConst failed")
```

### Comparing `py_ballisticcalc-1.0.4/py_ballisticcalc.egg-info/PKG-INFO` & `py_ballisticcalc-1.0.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,42 @@
 Metadata-Version: 2.1
-Name: py-ballisticcalc
-Version: 1.0.4
+Name: py_ballisticcalc
+Version: 1.0.9
 Summary: LGPL library for small arms ballistic calculations (Python 3)
 Home-page: https://github.com/o-murphy/py_ballisticcalc
-Download-URL: http://pypi.python.org/pypi/py_ballisticcalc/
 Author: o-murphy
 Author-email: thehelixpg@gmail.com
 License: LGPL-3.0
+Download-URL: http://pypi.python.org/pypi/py_ballisticcalc/
+Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # BallisticCalculator
 LGPL library for small arms ballistic calculations (Python 3)
 
 Installation
 ------------
 **Stable release from pypi**
+(Contains c-extensions which offer higher performance)
 ```commandline
 pip install py-ballisticcalc
 ```
-**Latest release, may contain some issues**
+**Latest (only pure python) release, may contain some issues**
 ```commandline
 pip install git+https://github.com/o-murphy/py_ballisticcalc
 ```    
 
+**Also use `git clone` to build your own package**
+(Contains cython files to build your own c-extensions)
+```commandline
+git clone https://github.com/o-murphy/py_ballisticcalc
+```   
+
+
 Usage
 -----
 
 ### Simple start
 ```python
 from py_ballisticcalc.profile import Profile
 from py_ballisticcalc.bmath import unit
@@ -169,7 +178,9 @@
 The current status of the project is ALPHA version.
 
 RISK NOTICE
 
 The library performs very limited simulation of a complex physical process and so it performs a lot of approximations. Therefore the calculation results MUST NOT be considered as completely and reliably reflecting actual behavior or characteristics of projectiles. While these results may be used for educational purpose, they must NOT be considered as reliable for the areas where incorrect calculation may cause making a wrong decision, financial harm, or can put a human life at risk.
 
 THE CODE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE MATERIALS OR THE USE OR OTHER DEALINGS IN THE MATERIALS.
+
+
```

