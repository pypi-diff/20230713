# Comparing `tmp/multi-vector-simulator-1.0.6rc8.tar.gz` & `tmp/multi-vector-simulator-1.0.6rc9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multi-vector-simulator-1.0.6rc8.tar", last modified: Sun Oct 16 14:18:04 2022, max compression
+gzip compressed data, was "multi-vector-simulator-1.0.6rc9.tar", last modified: Sun Oct 16 14:39:14 2022, max compression
```

## Comparing `multi-vector-simulator-1.0.6rc8.tar` & `multi-vector-simulator-1.0.6rc9.tar`

### file list

```diff
@@ -1,85 +1,86 @@
-drwxrwxr-x   0 pierre-francois  (1000) pierre-francois  (1000)        0 2022-10-16 14:18:04.273596 multi-vector-simulator-1.0.6rc8/
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    18092 2022-01-27 11:19:42.000000 multi-vector-simulator-1.0.6rc8/LICENSE.md
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)       45 2022-01-27 11:19:42.000000 multi-vector-simulator-1.0.6rc8/MANIFEST.in
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    12138 2022-10-16 14:18:04.273596 multi-vector-simulator-1.0.6rc8/PKG-INFO
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    10994 2022-09-23 09:43:57.000000 multi-vector-simulator-1.0.6rc8/README.rst
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)       38 2022-10-16 14:18:04.273596 multi-vector-simulator-1.0.6rc8/setup.cfg
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)     9653 2022-09-23 09:34:10.000000 multi-vector-simulator-1.0.6rc8/setup.py
-drwxrwxr-x   0 pierre-francois  (1000) pierre-francois  (1000)        0 2022-10-16 14:18:04.269596 multi-vector-simulator-1.0.6rc8/src/
-drwxrwxr-x   0 pierre-francois  (1000) pierre-francois  (1000)        0 2022-10-16 14:18:04.269596 multi-vector-simulator-1.0.6rc8/src/multi_vector_simulator/
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    16860 2022-09-23 09:34:10.000000 multi-vector-simulator-1.0.6rc8/src/multi_vector_simulator/A0_initialization.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    27429 2022-10-16 14:16:22.000000 multi-vector-simulator-1.0.6rc8/src/multi_vector_simulator/A1_csv_to_json.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    11661 2022-09-23 09:34:10.000000 multi-vector-simulator-1.0.6rc8/src/multi_vector_simulator/B0_data_input_json.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    69516 2022-09-23 09:43:57.000000 multi-vector-simulator-1.0.6rc8/src/multi_vector_simulator/C0_data_processing.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    38672 2022-10-16 14:16:22.000000 multi-vector-simulator-1.0.6rc8/src/multi_vector_simulator/C1_verification.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    17720 2022-10-12 07:18:56.000000 multi-vector-simulator-1.0.6rc8/src/multi_vector_simulator/C2_economic_functions.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    14667 2022-10-16 14:16:22.000000 multi-vector-simulator-1.0.6rc8/src/multi_vector_simulator/D0_modelling_and_optimization.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    50103 2022-10-16 14:16:22.000000 multi-vector-simulator-1.0.6rc8/src/multi_vector_simulator/D1_model_components.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    28678 2022-09-23 09:34:10.000000 multi-vector-simulator-1.0.6rc8/src/multi_vector_simulator/D2_model_constraints.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    12133 2022-09-23 09:43:57.000000 multi-vector-simulator-1.0.6rc8/src/multi_vector_simulator/E0_evaluation.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    40926 2022-09-29 13:39:25.000000 multi-vector-simulator-1.0.6rc8/src/multi_vector_simulator/E1_process_results.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    17837 2022-09-29 13:39:25.000000 multi-vector-simulator-1.0.6rc8/src/multi_vector_simulator/E2_economics.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    44187 2022-09-23 09:43:57.000000 multi-vector-simulator-1.0.6rc8/src/multi_vector_simulator/E3_indicator_calculation.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)     9281 2022-01-27 11:19:42.000000 multi-vector-simulator-1.0.6rc8/src/multi_vector_simulator/E4_verification.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)     9543 2022-01-27 11:19:42.000000 multi-vector-simulator-1.0.6rc8/src/multi_vector_simulator/F0_output.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    36870 2022-10-16 14:16:22.000000 multi-vector-simulator-1.0.6rc8/src/multi_vector_simulator/F1_plotting.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    38813 2022-09-23 09:43:57.000000 multi-vector-simulator-1.0.6rc8/src/multi_vector_simulator/F2_autoreport.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    11637 2022-08-24 10:15:04.000000 multi-vector-simulator-1.0.6rc8/src/multi_vector_simulator/F3_debug.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)        0 2022-01-27 11:19:42.000000 multi-vector-simulator-1.0.6rc8/src/multi_vector_simulator/__init__.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    10258 2022-09-23 09:34:10.000000 multi-vector-simulator-1.0.6rc8/src/multi_vector_simulator/cli.py
-drwxrwxr-x   0 pierre-francois  (1000) pierre-francois  (1000)        0 2022-10-16 14:18:04.269596 multi-vector-simulator-1.0.6rc8/src/multi_vector_simulator/package_data/
-drwxrwxr-x   0 pierre-francois  (1000) pierre-francois  (1000)        0 2022-10-16 14:18:04.273596 multi-vector-simulator-1.0.6rc8/src/multi_vector_simulator/package_data/assets/
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)   168697 2022-01-27 11:19:42.000000 multi-vector-simulator-1.0.6rc8/src/multi_vector_simulator/package_data/assets/logo-eland-original.jpg
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)     6128 2022-01-27 11:19:42.000000 multi-vector-simulator-1.0.6rc8/src/multi_vector_simulator/package_data/assets/styles.css
-drwxrwxr-x   0 pierre-francois  (1000) pierre-francois  (1000)        0 2022-10-16 14:18:04.269596 multi-vector-simulator-1.0.6rc8/src/multi_vector_simulator/package_data/input_template/
-drwxrwxr-x   0 pierre-francois  (1000) pierre-francois  (1000)        0 2022-10-16 14:18:04.273596 multi-vector-simulator-1.0.6rc8/src/multi_vector_simulator/package_data/input_template/csv_elements/
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      132 2022-01-27 11:19:42.000000 multi-vector-simulator-1.0.6rc8/src/multi_vector_simulator/package_data/input_template/csv_elements/constraints.csv
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)       92 2022-01-27 11:19:42.000000 multi-vector-simulator-1.0.6rc8/src/multi_vector_simulator/package_data/input_template/csv_elements/economic_data.csv
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)       22 2022-01-27 11:19:42.000000 multi-vector-simulator-1.0.6rc8/src/multi_vector_simulator/package_data/input_template/csv_elements/energyBusses.csv
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)       81 2022-01-27 11:19:42.000000 multi-vector-simulator-1.0.6rc8/src/multi_vector_simulator/package_data/input_template/csv_elements/energyConsumption.csv
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      332 2022-01-27 11:19:42.000000 multi-vector-simulator-1.0.6rc8/src/multi_vector_simulator/package_data/input_template/csv_elements/energyConversion.csv
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      355 2022-01-27 11:19:42.000000 multi-vector-simulator-1.0.6rc8/src/multi_vector_simulator/package_data/input_template/csv_elements/energyProduction.csv
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      312 2022-01-27 11:19:42.000000 multi-vector-simulator-1.0.6rc8/src/multi_vector_simulator/package_data/input_template/csv_elements/energyProviders.csv
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      150 2022-01-27 11:19:42.000000 multi-vector-simulator-1.0.6rc8/src/multi_vector_simulator/package_data/input_template/csv_elements/energyStorage.csv
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      121 2022-01-27 11:19:42.000000 multi-vector-simulator-1.0.6rc8/src/multi_vector_simulator/package_data/input_template/csv_elements/fixcost.csv
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      156 2022-01-27 11:19:42.000000 multi-vector-simulator-1.0.6rc8/src/multi_vector_simulator/package_data/input_template/csv_elements/project_data.csv
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      105 2022-01-27 11:19:42.000000 multi-vector-simulator-1.0.6rc8/src/multi_vector_simulator/package_data/input_template/csv_elements/simulation_settings.csv
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      404 2022-01-27 11:19:42.000000 multi-vector-simulator-1.0.6rc8/src/multi_vector_simulator/package_data/input_template/csv_elements/storage_01.csv
-drwxrwxr-x   0 pierre-francois  (1000) pierre-francois  (1000)        0 2022-10-16 14:18:04.273596 multi-vector-simulator-1.0.6rc8/src/multi_vector_simulator/package_data/input_template/time_series/
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)       16 2022-01-27 11:19:42.000000 multi-vector-simulator-1.0.6rc8/src/multi_vector_simulator/package_data/input_template/time_series/blank
-drwxrwxr-x   0 pierre-francois  (1000) pierre-francois  (1000)        0 2022-10-16 14:18:04.273596 multi-vector-simulator-1.0.6rc8/src/multi_vector_simulator/package_data/inputs/
-drwxrwxr-x   0 pierre-francois  (1000) pierre-francois  (1000)        0 2022-10-16 14:18:04.273596 multi-vector-simulator-1.0.6rc8/src/multi_vector_simulator/package_data/inputs/csv_elements/
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      156 2022-01-27 11:19:42.000000 multi-vector-simulator-1.0.6rc8/src/multi_vector_simulator/package_data/inputs/csv_elements/constraints.csv
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      105 2022-01-27 11:19:42.000000 multi-vector-simulator-1.0.6rc8/src/multi_vector_simulator/package_data/inputs/csv_elements/economic_data.csv
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      154 2022-01-27 11:19:42.000000 multi-vector-simulator-1.0.6rc8/src/multi_vector_simulator/package_data/inputs/csv_elements/energyBusses.csv
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      179 2022-01-27 11:19:42.000000 multi-vector-simulator-1.0.6rc8/src/multi_vector_simulator/package_data/inputs/csv_elements/energyConsumption.csv
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)     1068 2022-01-27 11:19:42.000000 multi-vector-simulator-1.0.6rc8/src/multi_vector_simulator/package_data/inputs/csv_elements/energyConversion.csv
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      562 2022-01-27 11:19:42.000000 multi-vector-simulator-1.0.6rc8/src/multi_vector_simulator/package_data/inputs/csv_elements/energyProduction.csv
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      410 2022-01-27 11:19:42.000000 multi-vector-simulator-1.0.6rc8/src/multi_vector_simulator/package_data/inputs/csv_elements/energyProviders.csv
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      221 2022-01-27 11:19:42.000000 multi-vector-simulator-1.0.6rc8/src/multi_vector_simulator/package_data/inputs/csv_elements/energyStorage.csv
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      200 2022-01-27 11:19:42.000000 multi-vector-simulator-1.0.6rc8/src/multi_vector_simulator/package_data/inputs/csv_elements/fixcost.csv
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      249 2022-01-27 11:19:42.000000 multi-vector-simulator-1.0.6rc8/src/multi_vector_simulator/package_data/inputs/csv_elements/project_data.csv
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      130 2022-01-27 11:19:42.000000 multi-vector-simulator-1.0.6rc8/src/multi_vector_simulator/package_data/inputs/csv_elements/simulation_settings.csv
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      491 2022-01-27 11:19:42.000000 multi-vector-simulator-1.0.6rc8/src/multi_vector_simulator/package_data/inputs/csv_elements/storage_01.csv
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    23516 2022-01-27 11:19:42.000000 multi-vector-simulator-1.0.6rc8/src/multi_vector_simulator/package_data/inputs/mvs_config.json
-drwxrwxr-x   0 pierre-francois  (1000) pierre-francois  (1000)        0 2022-10-16 14:18:04.273596 multi-vector-simulator-1.0.6rc8/src/multi_vector_simulator/package_data/inputs/time_series/
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    78842 2022-01-27 11:19:42.000000 multi-vector-simulator-1.0.6rc8/src/multi_vector_simulator/package_data/inputs/time_series/demand.csv
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    34217 2022-01-27 11:19:42.000000 multi-vector-simulator-1.0.6rc8/src/multi_vector_simulator/package_data/inputs/time_series/pv_gen_merra2_2014_eff1_tilt40_az180.csv
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)     8301 2022-09-30 07:27:51.000000 multi-vector-simulator-1.0.6rc8/src/multi_vector_simulator/server.py
-drwxrwxr-x   0 pierre-francois  (1000) pierre-francois  (1000)        0 2022-10-16 14:18:04.273596 multi-vector-simulator-1.0.6rc8/src/multi_vector_simulator/utils/
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    24860 2022-10-16 14:16:22.000000 multi-vector-simulator-1.0.6rc8/src/multi_vector_simulator/utils/__init__.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)     3404 2022-03-30 10:59:56.000000 multi-vector-simulator-1.0.6rc8/src/multi_vector_simulator/utils/analysis.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    11844 2022-10-14 18:19:58.000000 multi-vector-simulator-1.0.6rc8/src/multi_vector_simulator/utils/constants.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)     8505 2022-10-16 14:16:22.000000 multi-vector-simulator-1.0.6rc8/src/multi_vector_simulator/utils/constants_json_strings.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)     1495 2022-01-27 11:19:42.000000 multi-vector-simulator-1.0.6rc8/src/multi_vector_simulator/utils/constants_output.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    27222 2022-10-14 18:20:23.000000 multi-vector-simulator-1.0.6rc8/src/multi_vector_simulator/utils/data_parser.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)     1594 2022-01-27 11:19:42.000000 multi-vector-simulator-1.0.6rc8/src/multi_vector_simulator/utils/exceptions.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)     2821 2022-10-14 10:17:55.000000 multi-vector-simulator-1.0.6rc8/src/multi_vector_simulator/utils/helpers.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      144 2022-10-16 14:17:37.000000 multi-vector-simulator-1.0.6rc8/src/multi_vector_simulator/version.py
-drwxrwxr-x   0 pierre-francois  (1000) pierre-francois  (1000)        0 2022-10-16 14:18:04.273596 multi-vector-simulator-1.0.6rc8/src/multi_vector_simulator.egg-info/
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    12138 2022-10-16 14:18:04.000000 multi-vector-simulator-1.0.6rc8/src/multi_vector_simulator.egg-info/PKG-INFO
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)     4144 2022-10-16 14:18:04.000000 multi-vector-simulator-1.0.6rc8/src/multi_vector_simulator.egg-info/SOURCES.txt
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)        1 2022-10-16 14:18:04.000000 multi-vector-simulator-1.0.6rc8/src/multi_vector_simulator.egg-info/dependency_links.txt
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      192 2022-10-16 14:18:04.000000 multi-vector-simulator-1.0.6rc8/src/multi_vector_simulator.egg-info/entry_points.txt
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      475 2022-10-16 14:18:04.000000 multi-vector-simulator-1.0.6rc8/src/multi_vector_simulator.egg-info/requires.txt
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)       23 2022-10-16 14:18:04.000000 multi-vector-simulator-1.0.6rc8/src/multi_vector_simulator.egg-info/top_level.txt
+drwxrwxr-x   0 pierre-francois  (1000) pierre-francois  (1000)        0 2022-10-16 14:39:14.037323 multi-vector-simulator-1.0.6rc9/
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    18092 2022-01-27 11:19:42.000000 multi-vector-simulator-1.0.6rc9/LICENSE.md
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)       45 2022-01-27 11:19:42.000000 multi-vector-simulator-1.0.6rc9/MANIFEST.in
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    12138 2022-10-16 14:39:14.037323 multi-vector-simulator-1.0.6rc9/PKG-INFO
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    10994 2022-09-23 09:43:57.000000 multi-vector-simulator-1.0.6rc9/README.rst
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)       38 2022-10-16 14:39:14.037323 multi-vector-simulator-1.0.6rc9/setup.cfg
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)     9653 2022-09-23 09:34:10.000000 multi-vector-simulator-1.0.6rc9/setup.py
+drwxrwxr-x   0 pierre-francois  (1000) pierre-francois  (1000)        0 2022-10-16 14:39:14.029323 multi-vector-simulator-1.0.6rc9/src/
+drwxrwxr-x   0 pierre-francois  (1000) pierre-francois  (1000)        0 2022-10-16 14:39:14.033323 multi-vector-simulator-1.0.6rc9/src/multi_vector_simulator/
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    16860 2022-09-23 09:34:10.000000 multi-vector-simulator-1.0.6rc9/src/multi_vector_simulator/A0_initialization.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    27429 2022-10-16 14:16:22.000000 multi-vector-simulator-1.0.6rc9/src/multi_vector_simulator/A1_csv_to_json.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    11661 2022-09-23 09:34:10.000000 multi-vector-simulator-1.0.6rc9/src/multi_vector_simulator/B0_data_input_json.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    69516 2022-09-23 09:43:57.000000 multi-vector-simulator-1.0.6rc9/src/multi_vector_simulator/C0_data_processing.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    38672 2022-10-16 14:16:22.000000 multi-vector-simulator-1.0.6rc9/src/multi_vector_simulator/C1_verification.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    17720 2022-10-12 07:18:56.000000 multi-vector-simulator-1.0.6rc9/src/multi_vector_simulator/C2_economic_functions.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    14667 2022-10-16 14:16:22.000000 multi-vector-simulator-1.0.6rc9/src/multi_vector_simulator/D0_modelling_and_optimization.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    50103 2022-10-16 14:16:22.000000 multi-vector-simulator-1.0.6rc9/src/multi_vector_simulator/D1_model_components.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    28678 2022-09-23 09:34:10.000000 multi-vector-simulator-1.0.6rc9/src/multi_vector_simulator/D2_model_constraints.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    12133 2022-09-23 09:43:57.000000 multi-vector-simulator-1.0.6rc9/src/multi_vector_simulator/E0_evaluation.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    40926 2022-09-29 13:39:25.000000 multi-vector-simulator-1.0.6rc9/src/multi_vector_simulator/E1_process_results.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    17837 2022-09-29 13:39:25.000000 multi-vector-simulator-1.0.6rc9/src/multi_vector_simulator/E2_economics.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    44187 2022-09-23 09:43:57.000000 multi-vector-simulator-1.0.6rc9/src/multi_vector_simulator/E3_indicator_calculation.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)     9281 2022-01-27 11:19:42.000000 multi-vector-simulator-1.0.6rc9/src/multi_vector_simulator/E4_verification.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)     9543 2022-01-27 11:19:42.000000 multi-vector-simulator-1.0.6rc9/src/multi_vector_simulator/F0_output.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    36870 2022-10-16 14:16:22.000000 multi-vector-simulator-1.0.6rc9/src/multi_vector_simulator/F1_plotting.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    38813 2022-09-23 09:43:57.000000 multi-vector-simulator-1.0.6rc9/src/multi_vector_simulator/F2_autoreport.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    11637 2022-08-24 10:15:04.000000 multi-vector-simulator-1.0.6rc9/src/multi_vector_simulator/F3_debug.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)        0 2022-01-27 11:19:42.000000 multi-vector-simulator-1.0.6rc9/src/multi_vector_simulator/__init__.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    10258 2022-09-23 09:34:10.000000 multi-vector-simulator-1.0.6rc9/src/multi_vector_simulator/cli.py
+drwxrwxr-x   0 pierre-francois  (1000) pierre-francois  (1000)        0 2022-10-16 14:39:14.033323 multi-vector-simulator-1.0.6rc9/src/multi_vector_simulator/package_data/
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    14348 2022-10-16 14:39:13.000000 multi-vector-simulator-1.0.6rc9/src/multi_vector_simulator/package_data/MVS_parameters_list.csv
+drwxrwxr-x   0 pierre-francois  (1000) pierre-francois  (1000)        0 2022-10-16 14:39:14.033323 multi-vector-simulator-1.0.6rc9/src/multi_vector_simulator/package_data/assets/
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)   168697 2022-01-27 11:19:42.000000 multi-vector-simulator-1.0.6rc9/src/multi_vector_simulator/package_data/assets/logo-eland-original.jpg
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)     6128 2022-01-27 11:19:42.000000 multi-vector-simulator-1.0.6rc9/src/multi_vector_simulator/package_data/assets/styles.css
+drwxrwxr-x   0 pierre-francois  (1000) pierre-francois  (1000)        0 2022-10-16 14:39:14.029323 multi-vector-simulator-1.0.6rc9/src/multi_vector_simulator/package_data/input_template/
+drwxrwxr-x   0 pierre-francois  (1000) pierre-francois  (1000)        0 2022-10-16 14:39:14.033323 multi-vector-simulator-1.0.6rc9/src/multi_vector_simulator/package_data/input_template/csv_elements/
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      132 2022-01-27 11:19:42.000000 multi-vector-simulator-1.0.6rc9/src/multi_vector_simulator/package_data/input_template/csv_elements/constraints.csv
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)       92 2022-01-27 11:19:42.000000 multi-vector-simulator-1.0.6rc9/src/multi_vector_simulator/package_data/input_template/csv_elements/economic_data.csv
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)       22 2022-01-27 11:19:42.000000 multi-vector-simulator-1.0.6rc9/src/multi_vector_simulator/package_data/input_template/csv_elements/energyBusses.csv
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)       81 2022-01-27 11:19:42.000000 multi-vector-simulator-1.0.6rc9/src/multi_vector_simulator/package_data/input_template/csv_elements/energyConsumption.csv
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      332 2022-01-27 11:19:42.000000 multi-vector-simulator-1.0.6rc9/src/multi_vector_simulator/package_data/input_template/csv_elements/energyConversion.csv
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      355 2022-01-27 11:19:42.000000 multi-vector-simulator-1.0.6rc9/src/multi_vector_simulator/package_data/input_template/csv_elements/energyProduction.csv
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      312 2022-01-27 11:19:42.000000 multi-vector-simulator-1.0.6rc9/src/multi_vector_simulator/package_data/input_template/csv_elements/energyProviders.csv
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      150 2022-01-27 11:19:42.000000 multi-vector-simulator-1.0.6rc9/src/multi_vector_simulator/package_data/input_template/csv_elements/energyStorage.csv
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      121 2022-01-27 11:19:42.000000 multi-vector-simulator-1.0.6rc9/src/multi_vector_simulator/package_data/input_template/csv_elements/fixcost.csv
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      156 2022-01-27 11:19:42.000000 multi-vector-simulator-1.0.6rc9/src/multi_vector_simulator/package_data/input_template/csv_elements/project_data.csv
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      105 2022-01-27 11:19:42.000000 multi-vector-simulator-1.0.6rc9/src/multi_vector_simulator/package_data/input_template/csv_elements/simulation_settings.csv
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      404 2022-01-27 11:19:42.000000 multi-vector-simulator-1.0.6rc9/src/multi_vector_simulator/package_data/input_template/csv_elements/storage_01.csv
+drwxrwxr-x   0 pierre-francois  (1000) pierre-francois  (1000)        0 2022-10-16 14:39:14.033323 multi-vector-simulator-1.0.6rc9/src/multi_vector_simulator/package_data/input_template/time_series/
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)       16 2022-01-27 11:19:42.000000 multi-vector-simulator-1.0.6rc9/src/multi_vector_simulator/package_data/input_template/time_series/blank
+drwxrwxr-x   0 pierre-francois  (1000) pierre-francois  (1000)        0 2022-10-16 14:39:14.033323 multi-vector-simulator-1.0.6rc9/src/multi_vector_simulator/package_data/inputs/
+drwxrwxr-x   0 pierre-francois  (1000) pierre-francois  (1000)        0 2022-10-16 14:39:14.037323 multi-vector-simulator-1.0.6rc9/src/multi_vector_simulator/package_data/inputs/csv_elements/
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      156 2022-01-27 11:19:42.000000 multi-vector-simulator-1.0.6rc9/src/multi_vector_simulator/package_data/inputs/csv_elements/constraints.csv
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      105 2022-01-27 11:19:42.000000 multi-vector-simulator-1.0.6rc9/src/multi_vector_simulator/package_data/inputs/csv_elements/economic_data.csv
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      154 2022-01-27 11:19:42.000000 multi-vector-simulator-1.0.6rc9/src/multi_vector_simulator/package_data/inputs/csv_elements/energyBusses.csv
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      179 2022-01-27 11:19:42.000000 multi-vector-simulator-1.0.6rc9/src/multi_vector_simulator/package_data/inputs/csv_elements/energyConsumption.csv
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)     1068 2022-01-27 11:19:42.000000 multi-vector-simulator-1.0.6rc9/src/multi_vector_simulator/package_data/inputs/csv_elements/energyConversion.csv
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      562 2022-01-27 11:19:42.000000 multi-vector-simulator-1.0.6rc9/src/multi_vector_simulator/package_data/inputs/csv_elements/energyProduction.csv
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      410 2022-01-27 11:19:42.000000 multi-vector-simulator-1.0.6rc9/src/multi_vector_simulator/package_data/inputs/csv_elements/energyProviders.csv
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      221 2022-01-27 11:19:42.000000 multi-vector-simulator-1.0.6rc9/src/multi_vector_simulator/package_data/inputs/csv_elements/energyStorage.csv
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      200 2022-01-27 11:19:42.000000 multi-vector-simulator-1.0.6rc9/src/multi_vector_simulator/package_data/inputs/csv_elements/fixcost.csv
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      249 2022-01-27 11:19:42.000000 multi-vector-simulator-1.0.6rc9/src/multi_vector_simulator/package_data/inputs/csv_elements/project_data.csv
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      130 2022-01-27 11:19:42.000000 multi-vector-simulator-1.0.6rc9/src/multi_vector_simulator/package_data/inputs/csv_elements/simulation_settings.csv
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      491 2022-01-27 11:19:42.000000 multi-vector-simulator-1.0.6rc9/src/multi_vector_simulator/package_data/inputs/csv_elements/storage_01.csv
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    23516 2022-01-27 11:19:42.000000 multi-vector-simulator-1.0.6rc9/src/multi_vector_simulator/package_data/inputs/mvs_config.json
+drwxrwxr-x   0 pierre-francois  (1000) pierre-francois  (1000)        0 2022-10-16 14:39:14.037323 multi-vector-simulator-1.0.6rc9/src/multi_vector_simulator/package_data/inputs/time_series/
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    78842 2022-01-27 11:19:42.000000 multi-vector-simulator-1.0.6rc9/src/multi_vector_simulator/package_data/inputs/time_series/demand.csv
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    34217 2022-01-27 11:19:42.000000 multi-vector-simulator-1.0.6rc9/src/multi_vector_simulator/package_data/inputs/time_series/pv_gen_merra2_2014_eff1_tilt40_az180.csv
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)     8301 2022-09-30 07:27:51.000000 multi-vector-simulator-1.0.6rc9/src/multi_vector_simulator/server.py
+drwxrwxr-x   0 pierre-francois  (1000) pierre-francois  (1000)        0 2022-10-16 14:39:14.037323 multi-vector-simulator-1.0.6rc9/src/multi_vector_simulator/utils/
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    24860 2022-10-16 14:16:22.000000 multi-vector-simulator-1.0.6rc9/src/multi_vector_simulator/utils/__init__.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)     3404 2022-03-30 10:59:56.000000 multi-vector-simulator-1.0.6rc9/src/multi_vector_simulator/utils/analysis.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    11844 2022-10-14 18:19:58.000000 multi-vector-simulator-1.0.6rc9/src/multi_vector_simulator/utils/constants.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)     8505 2022-10-16 14:16:22.000000 multi-vector-simulator-1.0.6rc9/src/multi_vector_simulator/utils/constants_json_strings.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)     1495 2022-01-27 11:19:42.000000 multi-vector-simulator-1.0.6rc9/src/multi_vector_simulator/utils/constants_output.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    27222 2022-10-14 18:20:23.000000 multi-vector-simulator-1.0.6rc9/src/multi_vector_simulator/utils/data_parser.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)     1594 2022-01-27 11:19:42.000000 multi-vector-simulator-1.0.6rc9/src/multi_vector_simulator/utils/exceptions.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)     2821 2022-10-14 10:17:55.000000 multi-vector-simulator-1.0.6rc9/src/multi_vector_simulator/utils/helpers.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      144 2022-10-16 14:38:43.000000 multi-vector-simulator-1.0.6rc9/src/multi_vector_simulator/version.py
+drwxrwxr-x   0 pierre-francois  (1000) pierre-francois  (1000)        0 2022-10-16 14:39:14.033323 multi-vector-simulator-1.0.6rc9/src/multi_vector_simulator.egg-info/
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    12138 2022-10-16 14:39:13.000000 multi-vector-simulator-1.0.6rc9/src/multi_vector_simulator.egg-info/PKG-INFO
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)     4208 2022-10-16 14:39:13.000000 multi-vector-simulator-1.0.6rc9/src/multi_vector_simulator.egg-info/SOURCES.txt
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)        1 2022-10-16 14:39:13.000000 multi-vector-simulator-1.0.6rc9/src/multi_vector_simulator.egg-info/dependency_links.txt
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      192 2022-10-16 14:39:13.000000 multi-vector-simulator-1.0.6rc9/src/multi_vector_simulator.egg-info/entry_points.txt
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      475 2022-10-16 14:39:13.000000 multi-vector-simulator-1.0.6rc9/src/multi_vector_simulator.egg-info/requires.txt
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)       23 2022-10-16 14:39:13.000000 multi-vector-simulator-1.0.6rc9/src/multi_vector_simulator.egg-info/top_level.txt
```

### Comparing `multi-vector-simulator-1.0.6rc8/LICENSE.md` & `multi-vector-simulator-1.0.6rc9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `multi-vector-simulator-1.0.6rc8/PKG-INFO` & `multi-vector-simulator-1.0.6rc9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multi-vector-simulator
-Version: 1.0.6rc8
+Version: 1.0.6rc9
 Summary: Multi-vector Simulation Tool assessing and optimizing Local Energy Systems (LES) for the E-LAND project
 Home-page: https://github.com/rl-institut/multi-vector-simulator
 Author: Reiner Lemoine Institut
 Author-email: pypi@rl-institut.de
 Project-URL: Bug Reports, https://github.com/rl-institut/multi-vector-simulator/issues
 Project-URL: Source, https://github.com/rl-institut/multi-vector-simulator
 Keywords: multi-vector local-energy-systems
```

### Comparing `multi-vector-simulator-1.0.6rc8/README.rst` & `multi-vector-simulator-1.0.6rc9/README.rst`

 * *Files identical despite different names*

### Comparing `multi-vector-simulator-1.0.6rc8/setup.py` & `multi-vector-simulator-1.0.6rc9/setup.py`

 * *Files identical despite different names*

### Comparing `multi-vector-simulator-1.0.6rc8/src/multi_vector_simulator/A0_initialization.py` & `multi-vector-simulator-1.0.6rc9/src/multi_vector_simulator/A0_initialization.py`

 * *Files identical despite different names*

### Comparing `multi-vector-simulator-1.0.6rc8/src/multi_vector_simulator/A1_csv_to_json.py` & `multi-vector-simulator-1.0.6rc9/src/multi_vector_simulator/A1_csv_to_json.py`

 * *Files identical despite different names*

### Comparing `multi-vector-simulator-1.0.6rc8/src/multi_vector_simulator/B0_data_input_json.py` & `multi-vector-simulator-1.0.6rc9/src/multi_vector_simulator/B0_data_input_json.py`

 * *Files identical despite different names*

### Comparing `multi-vector-simulator-1.0.6rc8/src/multi_vector_simulator/C0_data_processing.py` & `multi-vector-simulator-1.0.6rc9/src/multi_vector_simulator/C0_data_processing.py`

 * *Files identical despite different names*

### Comparing `multi-vector-simulator-1.0.6rc8/src/multi_vector_simulator/C1_verification.py` & `multi-vector-simulator-1.0.6rc9/src/multi_vector_simulator/C1_verification.py`

 * *Files identical despite different names*

### Comparing `multi-vector-simulator-1.0.6rc8/src/multi_vector_simulator/C2_economic_functions.py` & `multi-vector-simulator-1.0.6rc9/src/multi_vector_simulator/C2_economic_functions.py`

 * *Files identical despite different names*

### Comparing `multi-vector-simulator-1.0.6rc8/src/multi_vector_simulator/D0_modelling_and_optimization.py` & `multi-vector-simulator-1.0.6rc9/src/multi_vector_simulator/D0_modelling_and_optimization.py`

 * *Files identical despite different names*

### Comparing `multi-vector-simulator-1.0.6rc8/src/multi_vector_simulator/D1_model_components.py` & `multi-vector-simulator-1.0.6rc9/src/multi_vector_simulator/D1_model_components.py`

 * *Files identical despite different names*

### Comparing `multi-vector-simulator-1.0.6rc8/src/multi_vector_simulator/D2_model_constraints.py` & `multi-vector-simulator-1.0.6rc9/src/multi_vector_simulator/D2_model_constraints.py`

 * *Files identical despite different names*

### Comparing `multi-vector-simulator-1.0.6rc8/src/multi_vector_simulator/E0_evaluation.py` & `multi-vector-simulator-1.0.6rc9/src/multi_vector_simulator/E0_evaluation.py`

 * *Files identical despite different names*

### Comparing `multi-vector-simulator-1.0.6rc8/src/multi_vector_simulator/E1_process_results.py` & `multi-vector-simulator-1.0.6rc9/src/multi_vector_simulator/E1_process_results.py`

 * *Files identical despite different names*

### Comparing `multi-vector-simulator-1.0.6rc8/src/multi_vector_simulator/E2_economics.py` & `multi-vector-simulator-1.0.6rc9/src/multi_vector_simulator/E2_economics.py`

 * *Files identical despite different names*

### Comparing `multi-vector-simulator-1.0.6rc8/src/multi_vector_simulator/E3_indicator_calculation.py` & `multi-vector-simulator-1.0.6rc9/src/multi_vector_simulator/E3_indicator_calculation.py`

 * *Files identical despite different names*

### Comparing `multi-vector-simulator-1.0.6rc8/src/multi_vector_simulator/E4_verification.py` & `multi-vector-simulator-1.0.6rc9/src/multi_vector_simulator/E4_verification.py`

 * *Files identical despite different names*

### Comparing `multi-vector-simulator-1.0.6rc8/src/multi_vector_simulator/F0_output.py` & `multi-vector-simulator-1.0.6rc9/src/multi_vector_simulator/F0_output.py`

 * *Files identical despite different names*

### Comparing `multi-vector-simulator-1.0.6rc8/src/multi_vector_simulator/F1_plotting.py` & `multi-vector-simulator-1.0.6rc9/src/multi_vector_simulator/F1_plotting.py`

 * *Files identical despite different names*

### Comparing `multi-vector-simulator-1.0.6rc8/src/multi_vector_simulator/F2_autoreport.py` & `multi-vector-simulator-1.0.6rc9/src/multi_vector_simulator/F2_autoreport.py`

 * *Files identical despite different names*

### Comparing `multi-vector-simulator-1.0.6rc8/src/multi_vector_simulator/F3_debug.py` & `multi-vector-simulator-1.0.6rc9/src/multi_vector_simulator/F3_debug.py`

 * *Files identical despite different names*

### Comparing `multi-vector-simulator-1.0.6rc8/src/multi_vector_simulator/cli.py` & `multi-vector-simulator-1.0.6rc9/src/multi_vector_simulator/cli.py`

 * *Files identical despite different names*

### Comparing `multi-vector-simulator-1.0.6rc8/src/multi_vector_simulator/package_data/assets/logo-eland-original.jpg` & `multi-vector-simulator-1.0.6rc9/src/multi_vector_simulator/package_data/assets/logo-eland-original.jpg`

 * *Files identical despite different names*

### Comparing `multi-vector-simulator-1.0.6rc8/src/multi_vector_simulator/package_data/assets/styles.css` & `multi-vector-simulator-1.0.6rc9/src/multi_vector_simulator/package_data/assets/styles.css`

 * *Files identical despite different names*

### Comparing `multi-vector-simulator-1.0.6rc8/src/multi_vector_simulator/package_data/inputs/csv_elements/energyConversion.csv` & `multi-vector-simulator-1.0.6rc9/src/multi_vector_simulator/package_data/inputs/csv_elements/energyConversion.csv`

 * *Files identical despite different names*

### Comparing `multi-vector-simulator-1.0.6rc8/src/multi_vector_simulator/package_data/inputs/csv_elements/energyProduction.csv` & `multi-vector-simulator-1.0.6rc9/src/multi_vector_simulator/package_data/inputs/csv_elements/energyProduction.csv`

 * *Files identical despite different names*

### Comparing `multi-vector-simulator-1.0.6rc8/src/multi_vector_simulator/package_data/inputs/mvs_config.json` & `multi-vector-simulator-1.0.6rc9/src/multi_vector_simulator/package_data/inputs/mvs_config.json`

 * *Files identical despite different names*

### Comparing `multi-vector-simulator-1.0.6rc8/src/multi_vector_simulator/package_data/inputs/time_series/demand.csv` & `multi-vector-simulator-1.0.6rc9/src/multi_vector_simulator/package_data/inputs/time_series/demand.csv`

 * *Files identical despite different names*

### Comparing `multi-vector-simulator-1.0.6rc8/src/multi_vector_simulator/package_data/inputs/time_series/pv_gen_merra2_2014_eff1_tilt40_az180.csv` & `multi-vector-simulator-1.0.6rc9/src/multi_vector_simulator/package_data/inputs/time_series/pv_gen_merra2_2014_eff1_tilt40_az180.csv`

 * *Files identical despite different names*

### Comparing `multi-vector-simulator-1.0.6rc8/src/multi_vector_simulator/server.py` & `multi-vector-simulator-1.0.6rc9/src/multi_vector_simulator/server.py`

 * *Files identical despite different names*

### Comparing `multi-vector-simulator-1.0.6rc8/src/multi_vector_simulator/utils/__init__.py` & `multi-vector-simulator-1.0.6rc9/src/multi_vector_simulator/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `multi-vector-simulator-1.0.6rc8/src/multi_vector_simulator/utils/analysis.py` & `multi-vector-simulator-1.0.6rc9/src/multi_vector_simulator/utils/analysis.py`

 * *Files identical despite different names*

### Comparing `multi-vector-simulator-1.0.6rc8/src/multi_vector_simulator/utils/constants.py` & `multi-vector-simulator-1.0.6rc9/src/multi_vector_simulator/utils/constants.py`

 * *Files identical despite different names*

### Comparing `multi-vector-simulator-1.0.6rc8/src/multi_vector_simulator/utils/constants_json_strings.py` & `multi-vector-simulator-1.0.6rc9/src/multi_vector_simulator/utils/constants_json_strings.py`

 * *Files identical despite different names*

### Comparing `multi-vector-simulator-1.0.6rc8/src/multi_vector_simulator/utils/constants_output.py` & `multi-vector-simulator-1.0.6rc9/src/multi_vector_simulator/utils/constants_output.py`

 * *Files identical despite different names*

### Comparing `multi-vector-simulator-1.0.6rc8/src/multi_vector_simulator/utils/data_parser.py` & `multi-vector-simulator-1.0.6rc9/src/multi_vector_simulator/utils/data_parser.py`

 * *Files identical despite different names*

### Comparing `multi-vector-simulator-1.0.6rc8/src/multi_vector_simulator/utils/exceptions.py` & `multi-vector-simulator-1.0.6rc9/src/multi_vector_simulator/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `multi-vector-simulator-1.0.6rc8/src/multi_vector_simulator/utils/helpers.py` & `multi-vector-simulator-1.0.6rc9/src/multi_vector_simulator/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `multi-vector-simulator-1.0.6rc8/src/multi_vector_simulator.egg-info/PKG-INFO` & `multi-vector-simulator-1.0.6rc9/src/multi_vector_simulator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multi-vector-simulator
-Version: 1.0.6rc8
+Version: 1.0.6rc9
 Summary: Multi-vector Simulation Tool assessing and optimizing Local Energy Systems (LES) for the E-LAND project
 Home-page: https://github.com/rl-institut/multi-vector-simulator
 Author: Reiner Lemoine Institut
 Author-email: pypi@rl-institut.de
 Project-URL: Bug Reports, https://github.com/rl-institut/multi-vector-simulator/issues
 Project-URL: Source, https://github.com/rl-institut/multi-vector-simulator
 Keywords: multi-vector local-energy-systems
```

### Comparing `multi-vector-simulator-1.0.6rc8/src/multi_vector_simulator.egg-info/SOURCES.txt` & `multi-vector-simulator-1.0.6rc9/src/multi_vector_simulator.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 src/multi_vector_simulator/version.py
 src/multi_vector_simulator.egg-info/PKG-INFO
 src/multi_vector_simulator.egg-info/SOURCES.txt
 src/multi_vector_simulator.egg-info/dependency_links.txt
 src/multi_vector_simulator.egg-info/entry_points.txt
 src/multi_vector_simulator.egg-info/requires.txt
 src/multi_vector_simulator.egg-info/top_level.txt
+src/multi_vector_simulator/package_data/MVS_parameters_list.csv
 src/multi_vector_simulator/package_data/assets/logo-eland-original.jpg
 src/multi_vector_simulator/package_data/assets/styles.css
 src/multi_vector_simulator/package_data/input_template/csv_elements/constraints.csv
 src/multi_vector_simulator/package_data/input_template/csv_elements/economic_data.csv
 src/multi_vector_simulator/package_data/input_template/csv_elements/energyBusses.csv
 src/multi_vector_simulator/package_data/input_template/csv_elements/energyConsumption.csv
 src/multi_vector_simulator/package_data/input_template/csv_elements/energyConversion.csv
```

