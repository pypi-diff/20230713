# Comparing `tmp/siman-1.3.4.tar.gz` & `tmp/siman-1.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/siman-1.3.4.tar", last modified: Wed Jul 12 15:48:56 2023, max compression
+gzip compressed data, was "dist/siman-1.3.5.tar", last modified: Thu Jul 13 11:06:53 2023, max compression
```

## Comparing `siman-1.3.4.tar` & `siman-1.3.5.tar`

### file list

```diff
@@ -1,84 +1,84 @@
-drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2023-07-12 15:48:56.846702 siman-1.3.4/
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    18047 2021-02-17 13:28:25.000000 siman-1.3.4/LICENSE
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)       98 2021-02-17 13:28:25.000000 siman-1.3.4/MANIFEST.in
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)      935 2023-07-12 15:48:56.846702 siman-1.3.4/PKG-INFO
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)      409 2021-02-17 13:28:25.000000 siman-1.3.4/README.md
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)       38 2023-07-12 15:48:56.846702 siman-1.3.4/setup.cfg
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)      989 2023-07-12 15:48:51.000000 siman-1.3.4/setup.py
-drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2023-07-12 15:48:56.844702 siman-1.3.4/siman/
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     2473 2022-03-05 17:22:57.000000 siman-1.3.4/siman/3d_plot.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     3140 2022-03-05 17:22:57.000000 siman-1.3.4/siman/SSHTools.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)       32 2021-02-17 13:28:25.000000 siman-1.3.4/siman/__init__.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    49648 2023-07-12 15:40:54.000000 siman-1.3.4/siman/analysis.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    26024 2022-03-05 17:22:57.000000 siman-1.3.4/siman/analysis_functions.py
-drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2023-07-12 15:48:56.844702 siman-1.3.4/siman/analyze/
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)        0 2022-09-20 15:22:50.000000 siman-1.3.4/siman/analyze/__init__.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    10970 2022-09-20 15:22:50.000000 siman-1.3.4/siman/analyze/segregation.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     1160 2022-03-05 17:22:57.000000 siman-1.3.4/siman/approximation.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    16329 2022-03-05 17:22:57.000000 siman-1.3.4/siman/bands.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)   122152 2023-07-12 15:40:43.000000 siman-1.3.4/siman/calc_manage.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)   127097 2023-07-12 15:40:43.000000 siman-1.3.4/siman/calc_manage_AB.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     1085 2022-03-05 17:22:57.000000 siman-1.3.4/siman/calcul.py
-drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2023-07-12 15:48:56.845702 siman-1.3.4/siman/calculators/
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)        0 2022-09-20 15:22:50.000000 siman-1.3.4/siman/calculators/__init__.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     3685 2022-09-20 15:22:50.000000 siman-1.3.4/siman/calculators/aims.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     8718 2022-09-20 15:22:50.000000 siman-1.3.4/siman/calculators/gaussian.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     3769 2022-09-20 15:22:50.000000 siman-1.3.4/siman/calculators/qe.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    56510 2023-07-12 15:40:54.000000 siman-1.3.4/siman/calculators/vasp.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    38832 2022-09-20 15:22:50.000000 siman-1.3.4/siman/calculators/vasp_old.py
-drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2023-07-12 15:48:56.845702 siman-1.3.4/siman/chg/
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)        0 2021-02-17 13:28:25.000000 siman-1.3.4/siman/chg/__init__.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     6771 2021-02-17 13:28:25.000000 siman-1.3.4/siman/chg/chg_func.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     3718 2021-02-17 13:28:25.000000 siman-1.3.4/siman/chg/vasputil_chgarith_module.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    11072 2023-07-12 15:40:54.000000 siman-1.3.4/siman/classes.py
-drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2023-07-12 15:48:56.846702 siman-1.3.4/siman/core/
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)        0 2022-09-20 15:22:50.000000 siman-1.3.4/siman/core/__init__.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    53311 2023-07-12 15:40:54.000000 siman-1.3.4/siman/core/calculation.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    45277 2022-09-20 15:22:50.000000 siman-1.3.4/siman/core/calculation_old.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    33337 2023-07-12 15:40:54.000000 siman-1.3.4/siman/core/cluster_batch_script.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     3698 2022-09-20 15:22:50.000000 siman-1.3.4/siman/core/cluster_run_script.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     2127 2022-09-20 15:22:50.000000 siman-1.3.4/siman/core/molecule.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)   118466 2023-07-12 08:46:06.000000 siman-1.3.4/siman/core/structure.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    20203 2023-07-12 08:46:06.000000 siman-1.3.4/siman/database.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     3192 2022-03-05 17:22:57.000000 siman-1.3.4/siman/default_project_conf.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    10776 2022-03-05 17:22:57.000000 siman-1.3.4/siman/dev_functions.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    32406 2023-07-12 15:40:54.000000 siman-1.3.4/siman/dos_functions.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     9424 2022-03-05 17:22:57.000000 siman-1.3.4/siman/fit_hex.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    28048 2023-07-12 08:46:06.000000 siman-1.3.4/siman/functions.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)   113841 2023-07-12 15:40:54.000000 siman-1.3.4/siman/geo.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    14530 2023-07-12 15:40:54.000000 siman-1.3.4/siman/header.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)      286 2022-03-05 17:22:57.000000 siman-1.3.4/siman/helper_for_writing_beatiful_code.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    40223 2023-07-12 15:40:54.000000 siman-1.3.4/siman/impurity.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    86006 2023-07-12 15:40:43.000000 siman-1.3.4/siman/inout.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     4642 2022-03-05 17:22:57.000000 siman-1.3.4/siman/kpoints_functions.py
-drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2023-07-12 15:48:56.846702 siman-1.3.4/siman/mat_prop/
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)        0 2022-09-20 15:22:50.000000 siman-1.3.4/siman/mat_prop/__init__.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     1574 2022-09-20 15:22:50.000000 siman-1.3.4/siman/mat_prop/mat_prop.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    45055 2023-07-12 15:40:54.000000 siman-1.3.4/siman/matproj_functions.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    17009 2022-09-20 15:22:50.000000 siman-1.3.4/siman/monte.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)      980 2022-03-05 17:22:57.000000 siman-1.3.4/siman/monte_functions.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    31643 2022-09-20 15:22:50.000000 siman-1.3.4/siman/neb.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    44420 2021-02-17 13:28:25.000000 siman-1.3.4/siman/pairs.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    49712 2023-07-12 08:46:06.000000 siman-1.3.4/siman/picture_functions.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    25262 2022-03-05 17:22:57.000000 siman-1.3.4/siman/plot_functions.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     5224 2023-07-12 08:46:06.000000 siman-1.3.4/siman/polaron.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     2406 2022-03-05 17:22:57.000000 siman-1.3.4/siman/polaron_hop.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     3772 2022-09-29 10:57:16.000000 siman-1.3.4/siman/polaron_mod.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)   194580 2022-09-29 10:57:16.000000 siman-1.3.4/siman/project_funcs.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    22880 2022-03-05 17:22:57.000000 siman-1.3.4/siman/properties_2d.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     1114 2022-03-05 17:22:57.000000 siman-1.3.4/siman/properties_energy.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     1091 2022-03-05 17:22:57.000000 siman-1.3.4/siman/properties_lattice.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    30666 2023-07-12 15:40:54.000000 siman-1.3.4/siman/set_functions.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     1352 2022-03-05 17:22:57.000000 siman-1.3.4/siman/simanrc.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)      174 2022-03-05 17:22:57.000000 siman-1.3.4/siman/small_classes.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     6565 2022-09-29 10:57:16.000000 siman-1.3.4/siman/small_functions.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     8328 2022-03-05 17:22:57.000000 siman-1.3.4/siman/structure_functions.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     8854 2022-03-05 17:22:57.000000 siman-1.3.4/siman/table_functions.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     2780 2022-03-05 17:22:57.000000 siman-1.3.4/siman/thermo.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    18673 2022-03-05 17:22:57.000000 siman-1.3.4/siman/workflow_utilities.py
-drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2023-07-12 15:48:56.844702 siman-1.3.4/siman.egg-info/
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)      935 2023-07-12 15:48:56.000000 siman-1.3.4/siman.egg-info/PKG-INFO
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     1701 2023-07-12 15:48:56.000000 siman-1.3.4/siman.egg-info/SOURCES.txt
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)        1 2023-07-12 15:48:56.000000 siman-1.3.4/siman.egg-info/dependency_links.txt
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)       76 2023-07-12 15:48:56.000000 siman-1.3.4/siman.egg-info/requires.txt
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)        6 2023-07-12 15:48:56.000000 siman-1.3.4/siman.egg-info/top_level.txt
+drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2023-07-13 11:06:53.475451 siman-1.3.5/
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    18047 2021-02-17 13:28:25.000000 siman-1.3.5/LICENSE
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)       98 2021-02-17 13:28:25.000000 siman-1.3.5/MANIFEST.in
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)      935 2023-07-13 11:06:53.475451 siman-1.3.5/PKG-INFO
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)      409 2021-02-17 13:28:25.000000 siman-1.3.5/README.md
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)       38 2023-07-13 11:06:53.475451 siman-1.3.5/setup.cfg
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)      989 2023-07-13 11:06:51.000000 siman-1.3.5/setup.py
+drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2023-07-13 11:06:53.473451 siman-1.3.5/siman/
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     2473 2022-03-05 17:22:57.000000 siman-1.3.5/siman/3d_plot.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     3140 2022-03-05 17:22:57.000000 siman-1.3.5/siman/SSHTools.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)       32 2021-02-17 13:28:25.000000 siman-1.3.5/siman/__init__.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    50660 2023-07-13 11:06:22.000000 siman-1.3.5/siman/analysis.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    26024 2022-03-05 17:22:57.000000 siman-1.3.5/siman/analysis_functions.py
+drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2023-07-13 11:06:53.474451 siman-1.3.5/siman/analyze/
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)        0 2022-09-20 15:22:50.000000 siman-1.3.5/siman/analyze/__init__.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    10970 2022-09-20 15:22:50.000000 siman-1.3.5/siman/analyze/segregation.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     1160 2022-03-05 17:22:57.000000 siman-1.3.5/siman/approximation.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    16329 2022-03-05 17:22:57.000000 siman-1.3.5/siman/bands.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)   122152 2023-07-12 15:40:43.000000 siman-1.3.5/siman/calc_manage.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)   127097 2023-07-12 15:40:43.000000 siman-1.3.5/siman/calc_manage_AB.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     1085 2022-03-05 17:22:57.000000 siman-1.3.5/siman/calcul.py
+drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2023-07-13 11:06:53.474451 siman-1.3.5/siman/calculators/
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)        0 2022-09-20 15:22:50.000000 siman-1.3.5/siman/calculators/__init__.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     3685 2022-09-20 15:22:50.000000 siman-1.3.5/siman/calculators/aims.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     8718 2022-09-20 15:22:50.000000 siman-1.3.5/siman/calculators/gaussian.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     3769 2022-09-20 15:22:50.000000 siman-1.3.5/siman/calculators/qe.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    56510 2023-07-13 11:06:22.000000 siman-1.3.5/siman/calculators/vasp.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    38832 2022-09-20 15:22:50.000000 siman-1.3.5/siman/calculators/vasp_old.py
+drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2023-07-13 11:06:53.474451 siman-1.3.5/siman/chg/
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)        0 2021-02-17 13:28:25.000000 siman-1.3.5/siman/chg/__init__.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     6771 2021-02-17 13:28:25.000000 siman-1.3.5/siman/chg/chg_func.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     3718 2021-02-17 13:28:25.000000 siman-1.3.5/siman/chg/vasputil_chgarith_module.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    11072 2023-07-13 11:06:22.000000 siman-1.3.5/siman/classes.py
+drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2023-07-13 11:06:53.475451 siman-1.3.5/siman/core/
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)        0 2022-09-20 15:22:50.000000 siman-1.3.5/siman/core/__init__.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    53311 2023-07-13 11:06:22.000000 siman-1.3.5/siman/core/calculation.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    45277 2022-09-20 15:22:50.000000 siman-1.3.5/siman/core/calculation_old.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    33337 2023-07-13 11:06:22.000000 siman-1.3.5/siman/core/cluster_batch_script.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     3698 2022-09-20 15:22:50.000000 siman-1.3.5/siman/core/cluster_run_script.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     2127 2022-09-20 15:22:50.000000 siman-1.3.5/siman/core/molecule.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)   118466 2023-07-12 08:46:06.000000 siman-1.3.5/siman/core/structure.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    20203 2023-07-12 08:46:06.000000 siman-1.3.5/siman/database.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     3192 2022-03-05 17:22:57.000000 siman-1.3.5/siman/default_project_conf.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    10776 2022-03-05 17:22:57.000000 siman-1.3.5/siman/dev_functions.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    32406 2023-07-13 11:06:22.000000 siman-1.3.5/siman/dos_functions.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     9424 2022-03-05 17:22:57.000000 siman-1.3.5/siman/fit_hex.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    28048 2023-07-12 08:46:06.000000 siman-1.3.5/siman/functions.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)   113841 2023-07-13 11:06:22.000000 siman-1.3.5/siman/geo.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    14530 2023-07-13 11:06:22.000000 siman-1.3.5/siman/header.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)      286 2022-03-05 17:22:57.000000 siman-1.3.5/siman/helper_for_writing_beatiful_code.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    40223 2023-07-13 11:06:22.000000 siman-1.3.5/siman/impurity.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    86006 2023-07-12 15:40:43.000000 siman-1.3.5/siman/inout.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     4642 2022-03-05 17:22:57.000000 siman-1.3.5/siman/kpoints_functions.py
+drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2023-07-13 11:06:53.475451 siman-1.3.5/siman/mat_prop/
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)        0 2022-09-20 15:22:50.000000 siman-1.3.5/siman/mat_prop/__init__.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     1574 2022-09-20 15:22:50.000000 siman-1.3.5/siman/mat_prop/mat_prop.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    45055 2023-07-13 11:06:22.000000 siman-1.3.5/siman/matproj_functions.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    17009 2022-09-20 15:22:50.000000 siman-1.3.5/siman/monte.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)      980 2022-03-05 17:22:57.000000 siman-1.3.5/siman/monte_functions.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    31643 2022-09-20 15:22:50.000000 siman-1.3.5/siman/neb.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    44420 2021-02-17 13:28:25.000000 siman-1.3.5/siman/pairs.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    49712 2023-07-12 08:46:06.000000 siman-1.3.5/siman/picture_functions.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    25262 2022-03-05 17:22:57.000000 siman-1.3.5/siman/plot_functions.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     5224 2023-07-12 08:46:06.000000 siman-1.3.5/siman/polaron.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     2406 2022-03-05 17:22:57.000000 siman-1.3.5/siman/polaron_hop.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     3772 2022-09-29 10:57:16.000000 siman-1.3.5/siman/polaron_mod.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)   194580 2022-09-29 10:57:16.000000 siman-1.3.5/siman/project_funcs.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    22880 2022-03-05 17:22:57.000000 siman-1.3.5/siman/properties_2d.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     1114 2022-03-05 17:22:57.000000 siman-1.3.5/siman/properties_energy.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     1091 2022-03-05 17:22:57.000000 siman-1.3.5/siman/properties_lattice.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    30666 2023-07-13 11:06:22.000000 siman-1.3.5/siman/set_functions.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     1352 2022-03-05 17:22:57.000000 siman-1.3.5/siman/simanrc.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)      174 2022-03-05 17:22:57.000000 siman-1.3.5/siman/small_classes.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     6565 2022-09-29 10:57:16.000000 siman-1.3.5/siman/small_functions.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     8328 2022-03-05 17:22:57.000000 siman-1.3.5/siman/structure_functions.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     8854 2022-03-05 17:22:57.000000 siman-1.3.5/siman/table_functions.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     2780 2022-03-05 17:22:57.000000 siman-1.3.5/siman/thermo.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    18673 2022-03-05 17:22:57.000000 siman-1.3.5/siman/workflow_utilities.py
+drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2023-07-13 11:06:53.474451 siman-1.3.5/siman.egg-info/
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)      935 2023-07-13 11:06:53.000000 siman-1.3.5/siman.egg-info/PKG-INFO
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     1701 2023-07-13 11:06:53.000000 siman-1.3.5/siman.egg-info/SOURCES.txt
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)        1 2023-07-13 11:06:53.000000 siman-1.3.5/siman.egg-info/dependency_links.txt
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)       76 2023-07-13 11:06:53.000000 siman-1.3.5/siman.egg-info/requires.txt
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)        6 2023-07-13 11:06:53.000000 siman-1.3.5/siman.egg-info/top_level.txt
```

### Comparing `siman-1.3.4/LICENSE` & `siman-1.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `siman-1.3.4/PKG-INFO` & `siman-1.3.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: siman
-Version: 1.3.4
+Version: 1.3.5
 Summary: Manager for DFT calculations
 Home-page: https://github.com/dimonaks/siman
 Author: Dmitry Aksenov
 Author-email: dimonaks@gmail.com
 License: GPL
 Keywords: DFT VASP Density Functional Theory NEB DFT+U PAW GGA Monte-Carlo
 Platform: UNKNOWN
```

### Comparing `siman-1.3.4/setup.py` & `siman-1.3.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools, os
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="siman",
-    version="1.3.4",
+    version="1.3.5",
     author="Dmitry Aksenov",
     author_email="dimonaks@gmail.com",
     description="Manager for DFT calculations",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/dimonaks/siman",
     license = 'GPL',
```

### Comparing `siman-1.3.4/siman/3d_plot.py` & `siman-1.3.5/siman/3d_plot.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.4/siman/SSHTools.py` & `siman-1.3.5/siman/SSHTools.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.4/siman/analysis.py` & `siman-1.3.5/siman/analysis.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,15 +69,15 @@
 
 def calc_oxidation_states(cl = None, st = None, silent = 1):
 
     #only use if charges are full charges from bader 
     if cl:
         st = cl.end
         ch = cl.charges
-    if st:
+    elif st:
         ch  = st.charges
     
     # print(st.get_elements() )
     # print(ch)
 
     z_vals = []
     for j, z_val, el in zip(range(st.natom), st.get_elements_zval(), st.get_elements()):
@@ -681,16 +681,21 @@
         vlist.append(cl.end.vol)
         magn1.append(cl.magn1)
         magn2.append(cl.magn2)
         alpha, beta, gamma = st.get_angles()
         alphas.append(alpha)
         print('alpha, energy: {:4.2f}, {:6.3f}'.format(alpha, cl.energy_sigma0))
 
+    if header.SIMAN_WEB:
+        path_l = cl.path['output'].replace('100.OUTCAR','')
+    else:
+        path_l = 'figs/'
+
     fit_and_plot(U1 = (alphas, etotlist, 'o-r'), 
-        image_name = 'figs/angle', ylabel = 'Total energy, eV', xlabel = 'Angle, deg', xlim = (89, 92.6))
+        image_name = f'{path_l}/angle', ylabel = 'Total energy, eV', xlabel = 'Angle, deg', xlim = (89, 92.6))
 
     if ase_flag:
         if 'angle' in analysis_type:
             eos = EquationOfState(alphas, etotlist, eos = 'sjeos')
         else:
             eos = EquationOfState(vlist, etotlist, eos = 'sjeos')
         # import inspect
@@ -702,15 +707,16 @@
             #print "c = ", clist[2]
             printlog( '''
             v0 = {0} A^3
             a0 = {1} A
             E0 = {2} eV
             B  = {3} eV/A^3'''.format(v0, v0**(1./3), e0, B), imp = 'Y'  )
 
-            savedpath = 'figs/'+cl.name+'.png'
+            
+            savedpath = f'{path_l}{cl.name}.png'
             makedir(savedpath)
 
 
             cl.B = B*160.218
             # plt.close()
             # plt.clf()
             # plt.close('all')
@@ -1663,14 +1669,53 @@
     gamma = e/2/A*header.eV_A_to_J_m
 
     if printlog:
             print('Surface energy = {:3.2f} J/m2   | {:}  \n\n'.format(gamma, cl_surf.id))
     return gamma
 
 
+
+def gb_en_ideal(cl_gb, cl_bulk, n_gbs = 2):
+
+    """
+    Calculate grain boundary energy of a pure material
+    GB is assumed to be normal to R3! The stoichiometry should be the same!
+
+    INPUT:
+    
+    - cl_gb (Calculation class object) - slab or cell with grain boundary
+    - cl_bulk (Calculation class object) - bulk cell 
+    - n_gbs (int) - number of grain boundaries in the system (Default - 2)
+
+    RETURN:
+        e_gb (float) - grain boundary energy in J/m2
+
+    AUTHOR: Boev A.
+
+    """
+
+    import numpy as np
+
+    st1 = cl_gb.end
+    st2 = cl_bulk.end
+
+    e1 = cl_gb.e0
+    n1 = st1.natom
+    e2 = cl_bulk.e0
+    n2 = st2.natom
+
+
+    A = st1.get_surface_area()
+
+
+    e_gb = (e1 - e2*n1/n2)/2/A * header.eV_A_to_J_m
+    print('E_gb = {} J/m2; Check manually that stoichiometry is the same in cl_gb and cl_bulk'.format(round(e_gb, 2)))
+    return e_gb
+
+
 def ads_en(cl_slab_ads, cl_slab, ads_at = 'O'):
 
     # ads_at_dic = {'O':-1.52, 'H':-1.07}
     ads_at_dic = {'O':-4.22, 'H':-1.07, 'Li': -1.91, 'LCO':-5.7241 } # half E of A2 mol    -1.36 per O2 mol overestimate error
     e_ads_at = ads_at_dic[ads_at]
     if ads_at == 'LCO':
         e_ads_at = ads_at_dic['LCO']*4 - ads_at_dic['Li'] - ads_at_dic['O']*2
```

### Comparing `siman-1.3.4/siman/analysis_functions.py` & `siman-1.3.5/siman/analysis_functions.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.4/siman/analyze/segregation.py` & `siman-1.3.5/siman/analyze/segregation.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.4/siman/approximation.py` & `siman-1.3.5/siman/approximation.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.4/siman/bands.py` & `siman-1.3.5/siman/bands.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.4/siman/calc_manage.py` & `siman-1.3.5/siman/calc_manage.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.4/siman/calc_manage_AB.py` & `siman-1.3.5/siman/calc_manage_AB.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.4/siman/calcul.py` & `siman-1.3.5/siman/calcul.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.4/siman/calculators/aims.py` & `siman-1.3.5/siman/calculators/aims.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.4/siman/calculators/gaussian.py` & `siman-1.3.5/siman/calculators/gaussian.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.4/siman/calculators/qe.py` & `siman-1.3.5/siman/calculators/qe.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.4/siman/calculators/vasp.py` & `siman-1.3.5/siman/calculators/vasp.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.4/siman/calculators/vasp_old.py` & `siman-1.3.5/siman/calculators/vasp_old.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.4/siman/chg/chg_func.py` & `siman-1.3.5/siman/chg/chg_func.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.4/siman/chg/vasputil_chgarith_module.py` & `siman-1.3.5/siman/chg/vasputil_chgarith_module.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.4/siman/classes.py` & `siman-1.3.5/siman/classes.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.4/siman/core/calculation.py` & `siman-1.3.5/siman/core/calculation.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.4/siman/core/calculation_old.py` & `siman-1.3.5/siman/core/calculation_old.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.4/siman/core/cluster_batch_script.py` & `siman-1.3.5/siman/core/cluster_batch_script.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.4/siman/core/cluster_run_script.py` & `siman-1.3.5/siman/core/cluster_run_script.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.4/siman/core/molecule.py` & `siman-1.3.5/siman/core/molecule.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.4/siman/core/structure.py` & `siman-1.3.5/siman/core/structure.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.4/siman/database.py` & `siman-1.3.5/siman/database.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.4/siman/default_project_conf.py` & `siman-1.3.5/siman/default_project_conf.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.4/siman/dev_functions.py` & `siman-1.3.5/siman/dev_functions.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.4/siman/dos_functions.py` & `siman-1.3.5/siman/dos_functions.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.4/siman/fit_hex.py` & `siman-1.3.5/siman/fit_hex.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.4/siman/functions.py` & `siman-1.3.5/siman/functions.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.4/siman/geo.py` & `siman-1.3.5/siman/geo.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.4/siman/header.py` & `siman-1.3.5/siman/header.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.4/siman/impurity.py` & `siman-1.3.5/siman/impurity.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.4/siman/inout.py` & `siman-1.3.5/siman/inout.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.4/siman/kpoints_functions.py` & `siman-1.3.5/siman/kpoints_functions.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.4/siman/mat_prop/mat_prop.py` & `siman-1.3.5/siman/mat_prop/mat_prop.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.4/siman/matproj_functions.py` & `siman-1.3.5/siman/matproj_functions.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.4/siman/monte.py` & `siman-1.3.5/siman/monte.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.4/siman/monte_functions.py` & `siman-1.3.5/siman/monte_functions.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.4/siman/neb.py` & `siman-1.3.5/siman/neb.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.4/siman/pairs.py` & `siman-1.3.5/siman/pairs.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.4/siman/picture_functions.py` & `siman-1.3.5/siman/picture_functions.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.4/siman/plot_functions.py` & `siman-1.3.5/siman/plot_functions.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.4/siman/polaron.py` & `siman-1.3.5/siman/polaron.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.4/siman/polaron_hop.py` & `siman-1.3.5/siman/polaron_hop.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.4/siman/polaron_mod.py` & `siman-1.3.5/siman/polaron_mod.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.4/siman/project_funcs.py` & `siman-1.3.5/siman/project_funcs.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.4/siman/properties_2d.py` & `siman-1.3.5/siman/properties_2d.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.4/siman/properties_energy.py` & `siman-1.3.5/siman/properties_energy.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.4/siman/properties_lattice.py` & `siman-1.3.5/siman/properties_lattice.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.4/siman/set_functions.py` & `siman-1.3.5/siman/set_functions.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.4/siman/simanrc.py` & `siman-1.3.5/siman/simanrc.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.4/siman/small_functions.py` & `siman-1.3.5/siman/small_functions.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.4/siman/structure_functions.py` & `siman-1.3.5/siman/structure_functions.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.4/siman/table_functions.py` & `siman-1.3.5/siman/table_functions.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.4/siman/thermo.py` & `siman-1.3.5/siman/thermo.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.4/siman/workflow_utilities.py` & `siman-1.3.5/siman/workflow_utilities.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.4/siman.egg-info/PKG-INFO` & `siman-1.3.5/siman.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: siman
-Version: 1.3.4
+Version: 1.3.5
 Summary: Manager for DFT calculations
 Home-page: https://github.com/dimonaks/siman
 Author: Dmitry Aksenov
 Author-email: dimonaks@gmail.com
 License: GPL
 Keywords: DFT VASP Density Functional Theory NEB DFT+U PAW GGA Monte-Carlo
 Platform: UNKNOWN
```

### Comparing `siman-1.3.4/siman.egg-info/SOURCES.txt` & `siman-1.3.5/siman.egg-info/SOURCES.txt`

 * *Files identical despite different names*

