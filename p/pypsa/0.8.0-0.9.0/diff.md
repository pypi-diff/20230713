# Comparing `tmp/pypsa-0.8.0.tar.gz` & `tmp/pypsa-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pypsa-0.8.0.tar", last modified: Wed Jan 25 11:22:08 2017, max compression
+gzip compressed data, was "dist/pypsa-0.9.0.tar", last modified: Sat Apr 29 08:35:08 2017, max compression
```

## Comparing `pypsa-0.8.0.tar` & `pypsa-0.9.0.tar`

### file list

```diff
@@ -1,52 +1,53 @@
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2017-01-25 11:22:08.000000 pypsa-0.8.0/
--rw-rw-r--   0 tom       (1000) tom       (1000)     8664 2017-01-25 11:22:08.000000 pypsa-0.8.0/PKG-INFO
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2017-01-25 11:22:08.000000 pypsa-0.8.0/pypsa/
--rw-rw-r--   0 tom       (1000) tom       (1000)     6151 2017-01-23 15:48:29.000000 pypsa-0.8.0/pypsa/graph.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1385 2017-01-22 21:13:10.000000 pypsa-0.8.0/pypsa/components.csv
--rw-rw-r--   0 tom       (1000) tom       (1000)    10865 2017-01-23 15:50:06.000000 pypsa-0.8.0/pypsa/opt.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2017-01-25 11:22:08.000000 pypsa-0.8.0/pypsa/standard_types/
--rw-rw-r--   0 tom       (1000) tom       (1000)     4841 2017-01-25 09:56:01.000000 pypsa-0.8.0/pypsa/standard_types/line_types.csv
--rw-rw-r--   0 tom       (1000) tom       (1000)     2964 2017-01-24 14:13:47.000000 pypsa-0.8.0/pypsa/standard_types/transformer_types.csv
--rw-rw-r--   0 tom       (1000) tom       (1000)    22943 2017-01-25 08:33:44.000000 pypsa-0.8.0/pypsa/io.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1277 2017-01-25 11:12:31.000000 pypsa-0.8.0/pypsa/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)    36853 2017-01-25 08:31:25.000000 pypsa-0.8.0/pypsa/pf.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2017-01-25 11:22:08.000000 pypsa-0.8.0/pypsa/component_attrs/
--rw-rw-r--   0 tom       (1000) tom       (1000)     3155 2017-01-25 10:04:03.000000 pypsa-0.8.0/pypsa/component_attrs/storage_units.csv
--rw-rw-r--   0 tom       (1000) tom       (1000)     2722 2017-01-22 21:13:10.000000 pypsa-0.8.0/pypsa/component_attrs/networks.csv
--rw-rw-r--   0 tom       (1000) tom       (1000)     2271 2017-01-25 10:03:36.000000 pypsa-0.8.0/pypsa/component_attrs/generators.csv
--rw-rw-r--   0 tom       (1000) tom       (1000)      643 2017-01-22 21:13:10.000000 pypsa-0.8.0/pypsa/component_attrs/shunt_impedances.csv
--rw-rw-r--   0 tom       (1000) tom       (1000)      674 2017-01-22 21:13:10.000000 pypsa-0.8.0/pypsa/component_attrs/line_types.csv
--rw-rw-r--   0 tom       (1000) tom       (1000)     3685 2017-01-25 09:44:45.000000 pypsa-0.8.0/pypsa/component_attrs/lines.csv
--rw-rw-r--   0 tom       (1000) tom       (1000)     1877 2017-01-25 10:04:13.000000 pypsa-0.8.0/pypsa/component_attrs/stores.csv
--rw-rw-r--   0 tom       (1000) tom       (1000)      686 2017-01-25 10:04:29.000000 pypsa-0.8.0/pypsa/component_attrs/loads.csv
--rw-rw-r--   0 tom       (1000) tom       (1000)     4267 2017-01-25 10:02:41.000000 pypsa-0.8.0/pypsa/component_attrs/transformers.csv
--rw-rw-r--   0 tom       (1000) tom       (1000)     1314 2017-01-24 15:39:01.000000 pypsa-0.8.0/pypsa/component_attrs/transformer_types.csv
--rw-rw-r--   0 tom       (1000) tom       (1000)     1760 2017-01-25 10:03:22.000000 pypsa-0.8.0/pypsa/component_attrs/buses.csv
--rw-rw-r--   0 tom       (1000) tom       (1000)      384 2017-01-22 21:13:10.000000 pypsa-0.8.0/pypsa/component_attrs/sub_networks.csv
--rw-rw-r--   0 tom       (1000) tom       (1000)      254 2017-01-22 21:13:10.000000 pypsa-0.8.0/pypsa/component_attrs/carriers.csv
--rw-rw-r--   0 tom       (1000) tom       (1000)     2129 2017-01-25 10:03:51.000000 pypsa-0.8.0/pypsa/component_attrs/links.csv
--rw-rw-r--   0 tom       (1000) tom       (1000)     7584 2017-01-23 15:49:30.000000 pypsa-0.8.0/pypsa/plot.py
--rw-rw-r--   0 tom       (1000) tom       (1000)    26765 2017-01-23 16:33:03.000000 pypsa-0.8.0/pypsa/components.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     9210 2017-01-23 15:48:02.000000 pypsa-0.8.0/pypsa/contingency.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     6852 2017-01-23 15:48:11.000000 pypsa-0.8.0/pypsa/descriptors.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     3186 2017-01-23 15:48:22.000000 pypsa-0.8.0/pypsa/geo.py
--rw-rw-r--   0 tom       (1000) tom       (1000)    44622 2017-01-24 16:00:50.000000 pypsa-0.8.0/pypsa/opf.py
--rw-rw-r--   0 tom       (1000) tom       (1000)    19408 2017-01-23 15:48:46.000000 pypsa-0.8.0/pypsa/networkclustering.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     6629 2017-01-24 16:12:17.000000 pypsa-0.8.0/README.rst
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2017-01-25 11:22:08.000000 pypsa-0.8.0/pypsa.egg-info/
--rw-rw-r--   0 tom       (1000) tom       (1000)     8664 2017-01-25 11:22:08.000000 pypsa-0.8.0/pypsa.egg-info/PKG-INFO
--rw-rw-r--   0 tom       (1000) tom       (1000)     1194 2017-01-25 11:22:08.000000 pypsa-0.8.0/pypsa.egg-info/SOURCES.txt
--rw-rw-r--   0 tom       (1000) tom       (1000)        6 2017-01-25 11:22:08.000000 pypsa-0.8.0/pypsa.egg-info/top_level.txt
--rw-rw-r--   0 tom       (1000) tom       (1000)       48 2017-01-25 11:22:08.000000 pypsa-0.8.0/pypsa.egg-info/requires.txt
--rw-rw-r--   0 tom       (1000) tom       (1000)        1 2017-01-25 11:22:08.000000 pypsa-0.8.0/pypsa.egg-info/dependency_links.txt
--rw-rw-r--   0 tom       (1000) tom       (1000)      100 2017-01-25 11:08:46.000000 pypsa-0.8.0/MANIFEST.in
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2017-01-25 11:22:08.000000 pypsa-0.8.0/test/
--rw-rw-r--   0 tom       (1000) tom       (1000)     1614 2017-01-04 08:17:47.000000 pypsa-0.8.0/test/test_ac_dc_lopf.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     2639 2017-01-23 09:20:57.000000 pypsa-0.8.0/test/test_pf_against_pypower.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     2096 2016-10-05 19:51:08.000000 pypsa-0.8.0/test/test_lpf_against_pypower.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     2782 2017-01-23 10:47:06.000000 pypsa-0.8.0/test/test_pf_against_pandapower.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1147 2016-10-05 19:51:08.000000 pypsa-0.8.0/test/test_opf_storage.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1474 2016-11-20 21:44:18.000000 pypsa-0.8.0/test/test_sclopf_scigrid.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1279 2016-10-05 19:51:08.000000 pypsa-0.8.0/test/test_ac_dc_lpf.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1013 2017-01-25 11:12:18.000000 pypsa-0.8.0/setup.py
--rw-rw-r--   0 tom       (1000) tom       (1000)       88 2017-01-25 11:22:08.000000 pypsa-0.8.0/setup.cfg
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2017-04-29 08:35:08.000000 pypsa-0.9.0/
+-rw-rw-r--   0 tom       (1000) tom       (1000)     8724 2017-04-29 08:35:08.000000 pypsa-0.9.0/PKG-INFO
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2017-04-29 08:35:08.000000 pypsa-0.9.0/pypsa/
+-rw-rw-r--   0 tom       (1000) tom       (1000)     6536 2017-04-28 13:20:43.000000 pypsa-0.9.0/pypsa/graph.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1385 2017-04-28 13:20:43.000000 pypsa-0.9.0/pypsa/components.csv
+-rw-rw-r--   0 tom       (1000) tom       (1000)    10865 2017-04-28 13:20:43.000000 pypsa-0.9.0/pypsa/opt.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2017-04-29 08:35:08.000000 pypsa-0.9.0/pypsa/standard_types/
+-rw-rw-r--   0 tom       (1000) tom       (1000)     4841 2017-04-28 13:20:43.000000 pypsa-0.9.0/pypsa/standard_types/line_types.csv
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2964 2017-04-28 13:20:43.000000 pypsa-0.9.0/pypsa/standard_types/transformer_types.csv
+-rw-rw-r--   0 tom       (1000) tom       (1000)    23075 2017-04-29 08:33:58.000000 pypsa-0.9.0/pypsa/io.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1277 2017-04-29 08:33:58.000000 pypsa-0.9.0/pypsa/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)    36905 2017-04-29 08:33:58.000000 pypsa-0.9.0/pypsa/pf.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2017-04-29 08:35:08.000000 pypsa-0.9.0/pypsa/component_attrs/
+-rw-rw-r--   0 tom       (1000) tom       (1000)     3155 2017-04-28 13:20:43.000000 pypsa-0.9.0/pypsa/component_attrs/storage_units.csv
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2722 2017-04-28 13:20:43.000000 pypsa-0.9.0/pypsa/component_attrs/networks.csv
+-rw-rw-r--   0 tom       (1000) tom       (1000)     3819 2017-04-29 08:33:58.000000 pypsa-0.9.0/pypsa/component_attrs/generators.csv
+-rw-rw-r--   0 tom       (1000) tom       (1000)      643 2017-04-28 13:20:43.000000 pypsa-0.9.0/pypsa/component_attrs/shunt_impedances.csv
+-rw-rw-r--   0 tom       (1000) tom       (1000)      674 2017-04-28 13:20:43.000000 pypsa-0.9.0/pypsa/component_attrs/line_types.csv
+-rw-rw-r--   0 tom       (1000) tom       (1000)     3685 2017-04-28 13:20:43.000000 pypsa-0.9.0/pypsa/component_attrs/lines.csv
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1877 2017-04-28 13:20:43.000000 pypsa-0.9.0/pypsa/component_attrs/stores.csv
+-rw-rw-r--   0 tom       (1000) tom       (1000)      686 2017-04-28 13:20:43.000000 pypsa-0.9.0/pypsa/component_attrs/loads.csv
+-rw-rw-r--   0 tom       (1000) tom       (1000)     4267 2017-04-28 13:20:43.000000 pypsa-0.9.0/pypsa/component_attrs/transformers.csv
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1314 2017-04-28 13:20:43.000000 pypsa-0.9.0/pypsa/component_attrs/transformer_types.csv
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1760 2017-04-28 13:20:43.000000 pypsa-0.9.0/pypsa/component_attrs/buses.csv
+-rw-rw-r--   0 tom       (1000) tom       (1000)      384 2017-04-28 13:20:43.000000 pypsa-0.9.0/pypsa/component_attrs/sub_networks.csv
+-rw-rw-r--   0 tom       (1000) tom       (1000)      254 2017-04-28 13:20:43.000000 pypsa-0.9.0/pypsa/component_attrs/carriers.csv
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2129 2017-04-28 13:20:43.000000 pypsa-0.9.0/pypsa/component_attrs/links.csv
+-rw-rw-r--   0 tom       (1000) tom       (1000)     8975 2017-04-28 13:20:43.000000 pypsa-0.9.0/pypsa/plot.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)    28753 2017-04-29 08:33:58.000000 pypsa-0.9.0/pypsa/components.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     9108 2017-04-29 08:33:58.000000 pypsa-0.9.0/pypsa/contingency.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     6852 2017-04-28 13:20:43.000000 pypsa-0.9.0/pypsa/descriptors.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     3186 2017-04-28 13:20:43.000000 pypsa-0.9.0/pypsa/geo.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)    54619 2017-04-29 08:33:58.000000 pypsa-0.9.0/pypsa/opf.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)    18882 2017-04-29 08:33:58.000000 pypsa-0.9.0/pypsa/networkclustering.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     6689 2017-04-29 08:33:58.000000 pypsa-0.9.0/README.rst
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2017-04-29 08:35:08.000000 pypsa-0.9.0/pypsa.egg-info/
+-rw-rw-r--   0 tom       (1000) tom       (1000)     8724 2017-04-29 08:35:08.000000 pypsa-0.9.0/pypsa.egg-info/PKG-INFO
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1223 2017-04-29 08:35:08.000000 pypsa-0.9.0/pypsa.egg-info/SOURCES.txt
+-rw-rw-r--   0 tom       (1000) tom       (1000)        6 2017-04-29 08:35:08.000000 pypsa-0.9.0/pypsa.egg-info/top_level.txt
+-rw-rw-r--   0 tom       (1000) tom       (1000)       48 2017-04-29 08:35:08.000000 pypsa-0.9.0/pypsa.egg-info/requires.txt
+-rw-rw-r--   0 tom       (1000) tom       (1000)        1 2017-04-29 08:35:08.000000 pypsa-0.9.0/pypsa.egg-info/dependency_links.txt
+-rw-rw-r--   0 tom       (1000) tom       (1000)      100 2017-04-28 13:20:43.000000 pypsa-0.9.0/MANIFEST.in
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2017-04-29 08:35:08.000000 pypsa-0.9.0/test/
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1614 2017-01-04 08:17:47.000000 pypsa-0.9.0/test/test_ac_dc_lopf.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2615 2017-04-29 08:33:58.000000 pypsa-0.9.0/test/test_pf_against_pypower.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2084 2017-04-29 08:33:58.000000 pypsa-0.9.0/test/test_lpf_against_pypower.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2782 2017-04-29 08:33:58.000000 pypsa-0.9.0/test/test_pf_against_pandapower.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1147 2016-10-05 19:51:08.000000 pypsa-0.9.0/test/test_opf_storage.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     3260 2017-04-29 08:33:58.000000 pypsa-0.9.0/test/test_unit_commitment.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1476 2017-04-29 08:33:58.000000 pypsa-0.9.0/test/test_sclopf_scigrid.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1279 2016-10-05 19:51:08.000000 pypsa-0.9.0/test/test_ac_dc_lpf.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1013 2017-04-29 08:33:58.000000 pypsa-0.9.0/setup.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)       88 2017-04-29 08:35:08.000000 pypsa-0.9.0/setup.cfg
```

### Comparing `pypsa-0.8.0/PKG-INFO` & `pypsa-0.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pypsa
-Version: 0.8.0
+Version: 0.9.0
 Summary: Python for Power Systems Analysis
 Home-page: https://github.com/FRESNA/PyPSA
 Author: Tom Brown (FIAS), Jonas Hoersch (FIAS), David Schlachtberger (FIAS)
 Author-email: brown@fias.uni-frankfurt.de
 License: GPLv3
 Description: ################################
         Python for Power System Analysis
@@ -19,25 +19,26 @@
         =====
         
         PyPSA stands for "Python for Power System Analysis". It is pronounced "pipes-ah".
         
         PyPSA is a `free software
         <http://www.gnu.org/philosophy/free-sw.en.html>`_ toolbox for
         simulating and optimising modern power systems that include features
-        such as variable wind and solar generation, storage units, sector
-        coupling and mixed alternating and direct current networks. PyPSA is
-        designed to scale well with large networks and long time series.
+        such as conventional generators with unit commitment, variable wind
+        and solar generation, storage units, sector coupling and mixed
+        alternating and direct current networks. PyPSA is designed to scale
+        well with large networks and long time series.
         
         As of 2017 PyPSA is under heavy development and therefore it
         is recommended to use caution when using it in a production
         environment. Some APIs may change - those liable to be updated are
         listed in the `doc/todo.rst <doc/todo.rst>`_.
         
         PyPSA was initially developed by the `Renewable Energy Group
-        <https://fias.uni-frankfurt.de/physics/schramm/complex-renewable-energy-networks/>`_
+        <https://fias.uni-frankfurt.de/physics/schramm/renewable-energy-system-and-network-analysis/>`_
         at `FIAS <https://fias.uni-frankfurt.de/>`_ to carry out simulations
         for the `CoNDyNet project <http://condynet.de/>`_, financed by the
         `German Federal Ministry for Education and Research (BMBF) <https://www.bmbf.de/en/index.html>`_ as part of the `Stromnetze Research Initiative <http://forschung-stromnetze.info/projekte/grundlagen-und-konzepte-fuer-effiziente-dezentrale-stromnetze/>`_.
         
         
         Documentation
         =============
@@ -72,15 +73,15 @@
           the capacities of generation, storage and transmission)
         
         It has models for:
         
         * meshed multiply-connected AC and DC networks, with controllable
           converters between AC and DC networks
         * standard types for lines and transformers following the implementation in `pandapower <https://www.uni-kassel.de/eecs/fachgebiete/e2n/software/pandapower.html>`_
-        * conventional dispatchable generators
+        * conventional dispatchable generators with unit commitment
         * generators with time-varying power availability, such as
           wind and solar generators
         * storage units with efficiency losses
         * simple hydroelectricity with inflow and spillage
         * coupling with other energy carriers
         * basic components out of which more complicated assets can be built,
           such as Combined Heat and Power (CHP) units, heat pumps, resistive
@@ -97,15 +98,14 @@
         * Non-linear power flow solution using `analytic continuation
           <https://en.wikipedia.org/wiki/Holomorphic_embedding_load_flow_method>`_
           in the complex plane following `GridCal
           <https://github.com/SanPen/GridCal>`_
         
         Functionality that may be added in the future:
         
-        * Unit Commitment using MILP
         * Short-circuit current calculations
         * Dynamic RMS simulations
         * Small signal stability analysis
         * Interactive web-based GUI with SVG
         * OPF with the full non-linear network equations
         * Dynamic EMT simulations
         * Unbalanced load flow
@@ -130,15 +130,15 @@
         
         .. image:: http://www.pypsa.org/img/storage-scigrid.png
         
         .. image:: http://www.pypsa.org/img/scigrid-curtailment.png
         
         .. image:: http://www.pypsa.org/img/meshed-ac-dc.png
         
-        .. image:: http://www.pypsa.org/img/pre-4-network-181-LV-2.png
+        .. image:: http://www.pypsa.org/img/euro-pie-pre-7-branch_limit-1-256.png
         
         
         
         What PyPSA uses under the hood
         ===============================
         
         PyPSA is written and tested to be compatible with both Python 2.7 and
```

### Comparing `pypsa-0.8.0/pypsa/graph.py` & `pypsa-0.9.0/pypsa/graph.py`

 * *Files 3% similar despite different names*

```diff
@@ -48,26 +48,29 @@
                          for c in network.iterate_components(branch_components)
                          for branch in c.df.loc[slice(None)
                                                 if c.ind is None
                                                 else c.ind].itertuples())
 
     return graph
 
-def adjacency_matrix(network, branch_components=None, busorder=None):
+def adjacency_matrix(network, branch_components=None, busorder=None, weights=None):
     """
     Construct a sparse adjacency matrix (directed)
 
     Parameters
     ----------
     branch_components : iterable sublist of `branch_components`
        Buses connected by any of the selected branches are adjacent
        (default: branch_components (network) or passive_branch_components (sub_network))
     busorder : pd.Index subset of network.buses.index
        Basis to use for the matrix representation of the adjacency matrix
        (default: buses.index (network) or buses_i() (sub_network))
+    weights : pd.Series or None (default)
+       If given must provide a weight for each branch, multi-indexed
+       on branch_component name and branch name.
 
     Returns
     -------
     adjacency_matrix : sp.sparse.coo_matrix
        Directed adjacency matrix
     """
     from . import components
@@ -85,31 +88,36 @@
     else:
         raise TypeError(" must be called with a Network or a SubNetwork")
 
     no_buses = len(busorder)
     no_branches = 0
     bus0_inds = []
     bus1_inds = []
+    weight_vals = []
     for c in network.iterate_components(branch_components):
         if c.ind is None:
             sel = slice(None)
-            no_branches += len(c.df)
+            no_branches = len(c.df)
         else:
-            sel = c.ind
-            no_branches += len(c.ind)
+            sel = t.ind
+            no_branches = len(c.ind)
         bus0_inds.append(busorder.get_indexer(c.df.loc[sel, "bus0"]))
         bus1_inds.append(busorder.get_indexer(c.df.loc[sel, "bus1"]))
+        weight_vals.append(np.ones(no_branches)
+                           if weights is None
+                           else weights[c.name][sel].values)
 
     if no_branches == 0:
         return sp.sparse.coo_matrix((no_buses, no_buses))
 
     bus0_inds = np.concatenate(bus0_inds)
     bus1_inds = np.concatenate(bus1_inds)
+    weight_vals = np.concatenate(weight_vals)
 
-    return sp.sparse.coo_matrix((np.ones(no_branches), (bus0_inds, bus1_inds)),
+    return sp.sparse.coo_matrix((weight_vals, (bus0_inds, bus1_inds)),
                                 shape=(no_buses, no_buses))
 
 def incidence_matrix(network, branch_components=None, busorder=None):
     """
     Construct a sparse incidence matrix (directed)
 
     Parameters
```

### Comparing `pypsa-0.8.0/pypsa/components.csv` & `pypsa-0.9.0/pypsa/components.csv`

 * *Files identical despite different names*

### Comparing `pypsa-0.8.0/pypsa/opt.py` & `pypsa-0.9.0/pypsa/opt.py`

 * *Files identical despite different names*

### Comparing `pypsa-0.8.0/pypsa/standard_types/line_types.csv` & `pypsa-0.9.0/pypsa/standard_types/line_types.csv`

 * *Files identical despite different names*

### Comparing `pypsa-0.8.0/pypsa/standard_types/transformer_types.csv` & `pypsa-0.9.0/pypsa/standard_types/transformer_types.csv`

 * *Files identical despite different names*

### Comparing `pypsa-0.8.0/pypsa/io.py` & `pypsa-0.9.0/pypsa/io.py`

 * *Files 0% similar despite different names*

```diff
@@ -119,15 +119,17 @@
         col_export = []
         for col in df.columns:
             #do not export derived attributes
             if col in ["sub_network","r_pu","x_pu","g_pu","b_pu"]:
                 continue
             if col in attrs.index and pd.isnull(attrs.at[col,"default"]) and pd.isnull(df[col]).all():
                 continue
-            if col in attrs.index and (df[col] == attrs.at[col,"default"]).all():
+            if (col in attrs.index
+                and df[col].dtype == attrs.at[col, 'typ']
+                and (df[col] == attrs.at[col,"default"]).all()):
                 continue
 
             col_export.append(col)
 
         df[col_export].to_csv(os.path.join(csv_folder_name,list_name+".csv"),encoding=encoding)
 
 
@@ -213,17 +215,18 @@
             new_df.loc[:,k] = new_df.loc[:,k].astype(typ)
 
     setattr(network,network.components[cls_name]["list_name"],new_df)
 
     #check all the buses are well-defined
     for attr in ["bus","bus0","bus1"]:
         if attr in new_df.columns:
-            missing = new_df.index[pd.isnull(new_df[attr].map(network.buses.v_nom))]
+            missing = new_df.index[~new_df[attr].isin(network.buses.index)]
             if len(missing) > 0:
-                logger.warning("The following {} have buses which are not defined:\n{}".format(cls_name,missing))
+                logger.warning("The following %s have buses which are not defined:\n%s",
+                               cls_name, missing)
 
 
     #now deal with time-dependent properties
 
     pnl = network.pnl(cls_name)
 
     for k in set(non_static_attrs.index) & set(dataframe.columns):
@@ -312,15 +315,15 @@
             setattr(network,col,df[col][network.name])
 
     #if there is snapshots.csv, read in snapshot data
 
     file_name = os.path.join(csv_folder_name,"snapshots.csv")
 
     if os.path.isfile(file_name):
-        df = pd.read_csv(file_name,index_col=0,encoding=encoding)
+        df = pd.read_csv(file_name, index_col=0, encoding=encoding, parse_dates=True)
         network.set_snapshots(df.index)
         if "weightings" in df.columns:
             network.snapshot_weightings = df["weightings"].reindex(network.snapshots)
 
     #now read in other components; make sure buses and carriers come first
     for component in ["Bus", "Carrier"] + sorted(pypsa.components.all_components - {"Bus","Carrier","SubNetwork"}):
 
@@ -341,15 +344,15 @@
         df = pd.read_csv(file_name,index_col=0,encoding=encoding)
 
         import_components_from_dataframe(network,df,component)
 
         file_attrs = [n for n in os.listdir(csv_folder_name) if n.startswith(list_name+"-") and n.endswith(".csv")]
 
         for file_name in file_attrs:
-            df = pd.read_csv(os.path.join(csv_folder_name,file_name),index_col=0,encoding=encoding)
+            df = pd.read_csv(os.path.join(csv_folder_name,file_name), index_col=0, encoding=encoding, parse_dates=True)
             import_series_from_dataframe(network,df,component,file_name[len(list_name)+1:-4])
 
         logger.debug(getattr(network,list_name))
```

### Comparing `pypsa-0.8.0/pypsa/__init__.py` & `pypsa-0.9.0/pypsa/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -29,10 +29,10 @@
 from . import pf, opf, plot, networkclustering, io, contingency, geo
 
 from .components import Network, SubNetwork
 
 import logging
 logging.basicConfig(level=logging.INFO)
 
-__version__ = "0.8.0"
+__version__ = "0.9.0"
 __author__ = "Tom Brown (FIAS), Jonas Hoersch (FIAS), David Schlachtberger (FIAS)"
 __copyright__ = "Copyright 2015-2017 Tom Brown (FIAS), Jonas Hoersch (FIAS), David Schlachtberger (FIAS), GNU GPL 3"
```

### Comparing `pypsa-0.8.0/pypsa/pf.py` & `pypsa-0.9.0/pypsa/pf.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 from itertools import chain
 import time
 
 from .descriptors import get_switchable_as_dense, allocate_series_dataframes
 
 def _as_snapshots(network, snapshots):
     if snapshots is None:
-        snapshots = [network.now]
+        snapshots = network.snapshots
     if (isinstance(snapshots, six.string_types) or
         not isinstance(snapshots, (collections.Sequence, pd.Index))):
         return pd.Index([snapshots])
     else:
         return pd.Index(snapshots)
 
 
@@ -112,15 +112,15 @@
     """
     Full non-linear power flow for generic network.
 
     Parameters
     ----------
     snapshots : list-like|single snapshot
         A subset or an elements of network.snapshots on which to run
-        the power flow, defaults to [now]
+        the power flow, defaults to network.snapshots
     skip_pre: bool, default False
         Skip the preliminary steps of computing topology, calculating dependent values and finding bus controls.
     x_tol: float
         Tolerance for Newton-Raphson power flow.
     use_seed : bool, default False
         Use a seed for the initial guess for the Newton-Raphson algorithm.
 
@@ -167,15 +167,15 @@
     """
     Non-linear power flow for connected sub-network.
 
     Parameters
     ----------
     snapshots : list-like|single snapshot
         A subset or an elements of network.snapshots on which to run
-        the power flow, defaults to [now]
+        the power flow, defaults to network.snapshots
     skip_pre: bool, default False
         Skip the preliminary steps of computing topology, calculating dependent values and finding bus controls.
     x_tol: float
         Tolerance for Newton-Raphson power flow.
     use_seed : bool, default False
         Use a seed for the initial guess for the Newton-Raphson algorithm.
 
@@ -362,15 +362,15 @@
     """
     Linear power flow for generic network.
 
     Parameters
     ----------
     snapshots : list-like|single snapshot
         A subset or an elements of network.snapshots on which to run
-        the power flow, defaults to [now]
+        the power flow, defaults to network.snapshots
     skip_pre: bool, default False
         Skip the preliminary steps of computing topology, calculating
         dependent values and finding bus controls.
 
     Returns
     -------
     None
@@ -871,15 +871,15 @@
     """
     Linear power flow for connected sub-network.
 
     Parameters
     ----------
     snapshots : list-like|single snapshot
         A subset or an elements of network.snapshots on which to run
-        the power flow, defaults to [now]
+        the power flow, defaults to network.snapshots
     skip_pre: bool, default False
         Skip the preliminary steps of computing topology, calculating
         dependent values and finding bus controls.
 
     Returns
     -------
     None
```

### Comparing `pypsa-0.8.0/pypsa/component_attrs/storage_units.csv` & `pypsa-0.9.0/pypsa/component_attrs/storage_units.csv`

 * *Files identical despite different names*

### Comparing `pypsa-0.8.0/pypsa/component_attrs/networks.csv` & `pypsa-0.9.0/pypsa/component_attrs/networks.csv`

 * *Files identical despite different names*

### Comparing `pypsa-0.8.0/pypsa/component_attrs/generators.csv` & `pypsa-0.9.0/pypsa/component_attrs/links.csv`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 attribute,type,unit,default,description,status
 name,string,n/a,n/a,Unique name,Input (required)
-bus,string,n/a,n/a,name of bus to which generator is attached,Input (required)
-control,string,n/a,PQ,"P,Q,V control strategy for PF, must be ""PQ"", ""PV"" or ""Slack"".",Input (optional)
-type,string,n/a,n/a,"Placeholder for generator type. Not yet implemented.",Input (optional)
-p_nom,float,MW,0.,Nominal power for limits in OPF.,Input (optional)
+bus0,string,n/a,n/a,Name of first bus to which link is attached.,Input (required)
+bus1,string,n/a,n/a,Name of second bus to which link is attached.,Input (required)
+type,string,n/a,n/a,"Placeholder for link type. Not yet implemented.",Input (optional)
+efficiency,static or series,per unit,1.,Efficiency of power transfer from bus0 to bus1. (Can be time-dependent to represent temperature-dependent Coefficient of Performance of a heat pump from an electric to a heat bus.),Input (optional)
+p_nom,float,MVA,0.,Limit of active power which can pass through link.,Input (optional)
 p_nom_extendable,boolean,n/a,False,Switch to allow capacity p_nom to be extended in OPF.,Input (optional)
-p_nom_min,float,MW,0.,"If p_nom is extendable in OPF, set its minimum value.",Input (optional)
-p_nom_max,float,MW,inf,"If p_nom is extendable in OPF, set its maximum value (e.g. limited by technical potential).",Input (optional)
-p_min_pu,static or series,per unit,0.,"The minimum output for each snapshot per unit of p_nom for the OPF (e.g. for variable renewable generators this can change due to weather conditions and compulsory feed-in; for conventional generators it represents a minimal dispatch).",Input (optional)
-p_max_pu,static or series,per unit,1.,"The maximum output for each snapshot per unit of p_nom for the OPF (e.g. for varialbe renewable generators this can change due to weather conditions; for conventional generators it represents a maximum dispatch).",Input (optional)
-p_set,static or series,MW,0.,active power set point (for PF),Input (optional)
-q_set,static or series,MVar,0.,reactive power set point (for PF),Input (optional)
-sign,float,n/a,1.,power sign,Input (optional)
-carrier,string,n/a,n/a,"Prime mover energy carrier (e.g. coal, gas, wind, solar); required for CO2 calculation in OPF",Input (optional)
-marginal_cost,float,currency/MWh,0.,"Marginal cost of production of 1 MWh.",Input (optional)
+p_nom_min,float,MVA,0.,"If p_nom is extendable in OPF, set its minimum value.",Input (optional)
+p_nom_max,float,MVA,inf,"If p_nom is extendable in OPF, set its maximum value (e.g. limited by potential).",Input (optional)
+p_set,static or series,MW,0.,"The dispatch set point for p0 of the link in PF.",Input (optional)
+p_min_pu,static or series,per unit of p_nom,0.,"Minimal dispatch (can also be negative) per unit of p_nom for the link in OPF.",Input (optional)
+p_max_pu,static or series,per unit of p_nom,1.,"Maximal dispatch (can also be negative) per unit of p_nom for the link in OPF.",Input (optional)
 capital_cost,float,currency/MW,0.,"Capital cost of extending p_nom by 1 MW.",Input (optional)
-efficiency,float,per unit,1.,"Ratio between primary energy and electrical energy, e.g. takes value 0.4 MWh_elec/MWh_thermal for gas. This is important for determining CO2 emissions per MWh.",Input (optional)
-p,series,MW,0.,active power at bus (positive if net generation),Output
-q,series,MVar,0.,reactive power (positive if net generation),Output
-p_nom_opt,float,MW,0.,Optimised nominal power.,Output
+marginal_cost,float,currency/MWh,0.,"Marginal cost of transfering 1 MWh (before efficiency losses) from bus0 to bus1. NB: marginal cost only makes sense in OPF if p_max_pu >= 0.",Input (optional)
+length,float,km,0.,"Length of line, useful for calculating the capital cost.",Input (optional)
+terrain_factor,float,per unit,1.,"Terrain factor for increasing capital cost.",Input (optional)
+p0,series,MW,0.,Active power at bus0 (positive if branch is withdrawing power from bus0).,Output
+p1,series,MW,0.,Active power at bus1 (positive if branch is withdrawing power from bus1).,Output
+p_nom_opt,float,MVA,0.,Optimised capacity for active power.,Output
```

### Comparing `pypsa-0.8.0/pypsa/component_attrs/shunt_impedances.csv` & `pypsa-0.9.0/pypsa/component_attrs/shunt_impedances.csv`

 * *Files identical despite different names*

### Comparing `pypsa-0.8.0/pypsa/component_attrs/line_types.csv` & `pypsa-0.9.0/pypsa/component_attrs/line_types.csv`

 * *Files identical despite different names*

### Comparing `pypsa-0.8.0/pypsa/component_attrs/lines.csv` & `pypsa-0.9.0/pypsa/component_attrs/lines.csv`

 * *Files identical despite different names*

### Comparing `pypsa-0.8.0/pypsa/component_attrs/stores.csv` & `pypsa-0.9.0/pypsa/component_attrs/stores.csv`

 * *Files identical despite different names*

### Comparing `pypsa-0.8.0/pypsa/component_attrs/loads.csv` & `pypsa-0.9.0/pypsa/component_attrs/loads.csv`

 * *Files identical despite different names*

### Comparing `pypsa-0.8.0/pypsa/component_attrs/transformers.csv` & `pypsa-0.9.0/pypsa/component_attrs/transformers.csv`

 * *Files identical despite different names*

### Comparing `pypsa-0.8.0/pypsa/component_attrs/transformer_types.csv` & `pypsa-0.9.0/pypsa/component_attrs/transformer_types.csv`

 * *Files identical despite different names*

### Comparing `pypsa-0.8.0/pypsa/component_attrs/buses.csv` & `pypsa-0.9.0/pypsa/component_attrs/buses.csv`

 * *Files identical despite different names*

### Comparing `pypsa-0.8.0/pypsa/plot.py` & `pypsa-0.9.0/pypsa/plot.py`

 * *Files 7% similar despite different names*

```diff
@@ -32,15 +32,16 @@
 __author__ = "Tom Brown (FIAS), Jonas Hoersch (FIAS)"
 __copyright__ = "Copyright 2015-2017 Tom Brown (FIAS), Jonas Hoersch (FIAS), GNU GPL 3"
 
 
 plt_present = True
 try:
     import matplotlib.pyplot as plt
-    from matplotlib.collections import LineCollection
+    from matplotlib.patches import Wedge
+    from matplotlib.collections import LineCollection, PatchCollection
 except:
     plt_present = False
 
 basemap_present = True
 try:
     from mpl_toolkits.basemap import Basemap
 except:
@@ -127,23 +128,50 @@
         bmap.drawcountries()
         bmap.drawcoastlines()
 
         x, y = bmap(x.values, y.values)
         x = pd.Series(x, network.buses.index)
         y = pd.Series(y, network.buses.index)
 
-    c = pd.Series(bus_colors, index=network.buses.index)
-    if c.dtype == np.dtype('O'):
-        c.fillna("b", inplace=True)
-        c = list(c.values)
-    s = pd.Series(bus_sizes, index=network.buses.index, dtype="float").fillna(10)
-    bus_collection = ax.scatter(x, y, c=c, s=s, cmap=bus_cmap)
+    if isinstance(bus_sizes, pd.Series) and isinstance(bus_sizes.index, pd.MultiIndex):
+        # We are drawing pies to show all the different shares
+        assert len(network.buses.index.difference(bus_sizes.index.levels[0])) == 0, \
+            "The first MultiIndex level of bus_sizes must contain buses"
+        assert isinstance(bus_colors, dict) and set(bus_colors).issuperset(bus_sizes.index.levels[1]), \
+            "bus_colors must be a dictionary defining a color for each element " \
+            "in the second MultiIndex level of bus_sizes"
+
+        bus_sizes = bus_sizes.sort_index(level=0, sort_remaining=False)
+
+        patches = []
+        for b_i in bus_sizes.index.levels[0]:
+            s = bus_sizes.loc[b_i]
+            radius = s.sum()**0.5
+            ratios = s/s.sum()
+
+            start = 0.25
+            for i, ratio in ratios.iteritems():
+                patches.append(Wedge((x.at[b_i], y.at[b_i]), radius,
+                                     360*start, 360*(start+ratio),
+                                     facecolor=bus_colors[i]))
+                start += ratio
+        bus_collection = PatchCollection(patches, match_original=True)
+        ax.add_collection(bus_collection)
+    else:
+        c = pd.Series(bus_colors, index=network.buses.index)
+        if c.dtype == np.dtype('O'):
+            c.fillna("b", inplace=True)
+            c = list(c.values)
+        s = pd.Series(bus_sizes, index=network.buses.index, dtype="float").fillna(10)
+        bus_collection = ax.scatter(x, y, c=c, s=s, cmap=bus_cmap)
 
     def as_branch_series(ser):
-        if isinstance(ser, pd.Series):
+        if isinstance(ser, dict) and set(ser).issubset(branch_components):
+            return pd.Series(ser)
+        elif isinstance(ser, pd.Series):
             if isinstance(ser.index, pd.MultiIndex):
                 return ser
             index = ser.index
             ser = ser.values
         else:
             index = network.lines.index
         return pd.Series(ser,
@@ -157,24 +185,22 @@
         line_cmap = {'Line': line_cmap}
 
     branch_collections = []
     for c in network.iterate_components(branch_components):
         l_defaults = defaults_for_branches[c.name]
         l_widths = line_widths.get(c.name, l_defaults['width'])
         l_nums = None
-        if c.name in line_colors:
-            l_colors = line_colors[c.name]
+        l_colors = line_colors.get(c.name, l_defaults['color'])
 
+        if isinstance(l_colors, pd.Series):
             if issubclass(l_colors.dtype.type, np.number):
                 l_nums = l_colors
                 l_colors = None
             else:
                 l_colors.fillna(l_defaults['color'], inplace=True)
-        else:
-            l_colors = l_defaults['color']
 
         if not geometry:
             segments = (np.asarray(((c.df.bus0.map(x),
                                      c.df.bus0.map(y)),
                                     (c.df.bus1.map(x),
                                      c.df.bus1.map(y))))
                         .transpose(2, 0, 1))
```

### Comparing `pypsa-0.8.0/pypsa/components.py` & `pypsa-0.9.0/pypsa/components.py`

 * *Files 4% similar despite different names*

```diff
@@ -139,18 +139,14 @@
     Examples
     --------
     >>> nw = pypsa.Network(csv_folder_name=/my/folder,co2_limit=10e6)
 
     """
 
 
-
-    #the current scenario/time
-    now = "now"
-
     #limit of total co2-tonnes-equivalent emissions for period
     co2_limit = None
 
 
     #Spatial Reference System Identifier (SRID) for x,y - defaults to longitude and latitude
     srid = 4326
 
@@ -191,15 +187,15 @@
     adjacency_matrix = adjacency_matrix
 
     def __init__(self, csv_folder_name=None, name="", ignore_standard_types=False, **kwargs):
 
         Basic.__init__(self,name)
 
         #a list/index of scenarios/times
-        self.snapshots = pd.Index([self.now])
+        self.snapshots = pd.Index(["now"])
 
         #corresponds to number of hours represented by each snapshot
         self.snapshot_weightings = pd.Series(index=self.snapshots,data=1.)
 
         components = pd.read_csv(os.path.join(dir_name,
                                               "components.csv"),
                                  index_col=0)
@@ -346,17 +342,14 @@
             attrs = self.components[component]["attrs"]
 
             for k,default in attrs.default[attrs.varying].iteritems():
                 pnl[k] = pnl[k].reindex(self.snapshots).fillna(default)
 
         #NB: No need to rebind pnl to self, since haven't changed it
 
-        if self.now not in self.snapshots:
-            logger.warning("Attribute network.now is not in newly-defined snapshots. (network.now is only relevant if you call e.g. network.pf() without specifying snapshots.)")
-
 
 
     def add(self, class_name, name, **kwargs):
         """
         Add a single component to the network.
 
         Adds it to component DataFrame and Panel and creates object.
@@ -472,15 +465,15 @@
 
         Examples
         --------
         >>> network_copy = network.copy()
 
         """
 
-        network = Network(ignore_standard_types=ignore_standard_types)
+        network = self.__class__(ignore_standard_types=ignore_standard_types)
 
         for component in self.iterate_components(["Bus", "Carrier"] + sorted(all_components - {"Bus","Carrier"})):
             df = component.df
             #drop the standard types to avoid them being read in twice
             if not ignore_standard_types and component.name in standard_types:
                 df = component.df.drop(network.components[component.name]["standard_types"].index)
 
@@ -490,19 +483,91 @@
             network.set_snapshots(self.snapshots)
             for component in self.iterate_components():
                 pnl = getattr(network, component.list_name+"_t")
                 for k in iterkeys(component.pnl):
                     pnl[k] = component.pnl[k].copy()
 
         #catch all remaining attributes of network
-        for attr in ["name", "now", "co2_limit", "srid"]:
+        for attr in ["name", "co2_limit", "srid"]:
             setattr(network,attr,getattr(self,attr))
 
+        network.snapshot_weightings = self.snapshot_weightings.copy()
+
         return network
 
+    def __getitem__(self, key):
+        """
+        Returns a shallow slice of the Network object containing only
+        the selected buses and all the connected components.
+
+        Parameters
+        ----------
+        key : indexer or tuple of indexer
+            If only one indexer is provided it is used in the .ix
+            indexer of the buses dataframe (refer also to the help for
+            pd.DataFrame.ix). If a tuple of two indexers are provided,
+            the first one is used to slice snapshots and the second
+            one buses.
+
+        Returns
+        --------
+        network : pypsa.Network
+
+        Examples
+        --------
+        >>> sub_network_0 = network[network.buses.sub_network = "0"]
+
+        >>> sub_network_0_with_only_10_snapshots = network[:10, network.buses.sub_network = "0"]
+
+        """
+
+        if isinstance(key, tuple):
+            time_i, key = key
+        else:
+            time_i = slice(None)
+
+        n = self.__class__(ignore_standard_types=True)
+        n.import_components_from_dataframe(
+            pd.DataFrame(self.buses.ix[key]).assign(sub_network=""),
+            "Bus"
+        )
+        buses_i = n.buses.index
+
+        rest_components = all_components - one_port_components - branch_components
+        for c in rest_components - {"Bus", "SubNetwork"}:
+            n.import_components_from_dataframe(pd.DataFrame(self.df(c)), c)
+
+        for c in one_port_components:
+            df = self.df(c).loc[lambda df: df.bus.isin(buses_i)]
+            n.import_components_from_dataframe(pd.DataFrame(df), c)
+
+        for c in branch_components:
+            df = self.df(c).loc[lambda df: df.bus0.isin(buses_i) & df.bus1.isin(buses_i)]
+            n.import_components_from_dataframe(pd.DataFrame(df), c)
+
+        n.set_snapshots(self.snapshots[time_i])
+        for c in all_components:
+            i = n.df(c).index
+            try:
+                npnl = n.pnl(c)
+                pnl = self.pnl(c)
+
+                for k in pnl:
+                    npnl[k] = pnl[k].ix[time_i,i.intersection(pnl[k].columns)]
+            except AttributeError:
+                pass
+
+        # catch all remaining attributes of network
+        for attr in ["name", "co2_limit", "srid"]:
+            setattr(n,attr,getattr(self, attr))
+
+        n.snapshot_weightings = self.snapshot_weightings.ix[time_i]
+
+        return n
+
 
     #beware, this turns bools like s_nom_extendable into objects because of
     #presence of links without s_nom_extendable
     def branches(self):
         return pd.concat((self.df(c) for c in branch_components),
                          keys=branch_components)
 
@@ -574,61 +639,69 @@
         --------
         >>> network.consistency_check()
 
         """
 
 
         for c in self.iterate_components(one_port_components):
-            missing = c.df.index[pd.isnull(c.df.bus.map(self.buses.v_nom))]
+            missing = c.df.index[~c.df.bus.isin(self.buses.index)]
             if len(missing) > 0:
-                logger.warning("The following {} have buses which are not defined:\n{}".format(c.list_name,missing))
+                logger.warning("The following %s have buses which are not defined:\n%s",
+                               c.list_name, missing)
 
         for c in self.iterate_components(branch_components):
-            for end in ["0","1"]:
-                missing = c.df.index[pd.isnull(c.df["bus"+end].map(self.buses.v_nom))]
+            for attr in ["bus0","bus1"]:
+                missing = c.df.index[~c.df[attr].isin(self.buses.index)]
                 if len(missing) > 0:
-                    logger.warning("The following {} have bus {} which are not defined:\n{}".format(c.list_name,end,missing))
+                    logger.warning("The following %s have %s which are not defined:\n%s",
+                                   c.list_name, attr, missing)
 
 
         for c in self.iterate_components(passive_branch_components):
             for attr in ["x","r"]:
                 bad = c.df.index[c.df[attr] == 0.]
                 if len(bad) > 0:
-                    logger.warning("The following {} have zero {}, which could break the linear load flow:\n{}".format(c.list_name,attr,bad))
+                    logger.warning("The following %s have zero %s, which could break the linear load flow:\n%s",
+                                   c.list_name, attr, bad)
 
             bad = c.df.index[(c.df["x"] == 0.) & (c.df["r"] == 0.)]
             if len(bad) > 0:
-                logger.warning("The following {} have zero series impedance, which will break the load flow:\n{}".format(c.list_name,bad))
+                logger.warning("The following %s have zero series impedance, which will break the load flow:\n%s",
+                               c.list_name, bad)
 
 
         for c in self.iterate_components({"Transformer"}):
             bad = c.df.index[c.df["s_nom"] == 0.]
             if len(bad) > 0:
-                logger.warning("The following {} have zero s_nom, which is used to define the impedance and will thus break the load flow:\n{}".format(c.list_name,bad))
+                logger.warning("The following %s have zero s_nom, which is used to define the impedance and will thus break the load flow:\n%s",
+                               c.list_name, bad)
 
 
         for c in self.iterate_components(all_components):
             for attr in c.attrs.index[c.attrs.varying & c.attrs.static]:
                 attr_df = c.pnl[attr]
 
                 diff = attr_df.columns.difference(c.df.index)
                 if len(diff) > 0:
-                    logger.warning("The following {} have time series defined for attribute {} in network.{}_t, but are not defined in network.{}:\n{}".format(c.list_name,attr,c.list_name,c.list_name,diff))
+                    logger.warning("The following %s have time series defined for attribute %s in network.%s_t, but are not defined in network.%s:\n%s",
+                                   c.list_name, attr, c.list_name, c.list_name, diff)
 
                 diff = self.snapshots.difference(attr_df.index)
                 if len(diff) > 0:
-                    logger.warning("In the time-dependent Dataframe for attribute {} of network.{}_t the following snapshots are missing:\n{}".format(attr,c.list_name,diff))
+                    logger.warning("In the time-dependent Dataframe for attribute %s of network.%s_t the following snapshots are missing:\n%s",
+                                   attr, c.list_name, diff)
 
                 diff = attr_df.index.difference(self.snapshots)
                 if len(diff) > 0:
-                    logger.warning("In the time-dependent Dataframe for attribute {} of network.{}_t the following snapshots are defined which are not in network.snapshots:\n{}".format(attr,c.list_name,diff))
+                    logger.warning("In the time-dependent Dataframe for attribute %s of network.%s_t the following snapshots are defined which are not in network.snapshots:\n%s",
+                                   attr, c.list_name, diff)
 
 
 
-	#check all dtypes of component attributes
+        #check all dtypes of component attributes
 
         #this isn't strictly necessary (except for str)
         #since e.g. float == np.dtype("float64") is True
         #but we do it for easy reading of errors
         np_dtypes = {str : np.dtype("object"),
                      float : np.dtype("float64"),
                      int : np.dtype("int64"),
@@ -641,36 +714,42 @@
             types_soll = c.attrs["typ"][c.attrs["static"]].drop("name")
 
             dtypes_soll = types_soll.replace(np_dtypes)
 
             unmatched = (c.df.dtypes[dtypes_soll.index] != dtypes_soll)
 
             if unmatched.any():
-                logger.warning("The following attributes of the dataframe {} have the wrong dtype:\n{}\nThey are:\n{}\nbut should be:\n{}".format(c.list_name,
-                                                                                                                                         unmatched.index[unmatched],
-                                                                                                                                         c.df.dtypes[unmatched],
-                                                                                                                                         dtypes_soll[unmatched]))
+                logger.warning("The following attributes of the dataframe %s have the wrong dtype:\n%s\n"
+                               "They are:\n%s\n"
+                               "but should be:\n%s",
+                               c.list_name,
+                               unmatched.index[unmatched],
+                               c.df.dtypes[dtypes_soll.index[unmatched]],
+                               dtypes_soll[unmatched])
 
             #now check varying attributes
 
             types_soll = c.attrs["typ"][c.attrs["varying"]]
 
             dtypes_soll = types_soll.replace(np_dtypes)
 
             for attr, typ in dtypes_soll.iteritems():
                 if c.pnl[attr].empty:
                     continue
 
                 unmatched = (c.pnl[attr].dtypes != typ)
 
                 if unmatched.any():
-                    logger.warning("The following columns of time-varying attribute {} in {}_t have the wrong dtype:\n{}\nThey are:\n{}\nbut should be:\n{}".format(attr,c.list_name,
-                                                                                                                                  unmatched.index[unmatched],
-                                                                                                                                  c.pnl[attr].dtypes[unmatched],
-                                                                                                                                  typ))
+                    logger.warning("The following columns of time-varying attribute %s in %s_t have the wrong dtype:\n%s\n"
+                                   "They are:\n%s\n"
+                                   "but should be:\n%s",
+                                   attr,c.list_name,
+                                   unmatched.index[unmatched],
+                                   c.pnl[attr].dtypes[unmatched],
+                                   typ)
 
 
 
 class SubNetwork(Common):
     """
     Connected network of electric buses (AC or DC) with passive flows
     or isolated non-electric buses.
```

### Comparing `pypsa-0.8.0/pypsa/contingency.py` & `pypsa-0.9.0/pypsa/contingency.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 logger = logging.getLogger(__name__)
 
 import numpy as np
 import pandas as pd
 
 import collections
 
-from .pf import calculate_PTDF
+from .pf import calculate_PTDF, _as_snapshots
 
 from .opt import l_constraint
 
 
 def calculate_BODF(sub_network, skip_pre=False):
     """
     Calculate the Branch Outage Distribution Factor (BODF) for
@@ -86,35 +86,33 @@
     """
     Computes linear power flow for a selection of branch outages.
 
     Parameters
     ----------
     snapshots : list-like|single snapshot
         A subset or an elements of network.snapshots on which to run
-        the power flow, defaults to [now]
+        the power flow, defaults to network.snapshots
         NB: currently this only works for a single snapshot
     branch_outages : list-like
         A list of passive branches which are to be tested for outages.
         If None, it's take as all network.passive_branches_i()
-    now : object
-        Deprecated: A member of network.snapshots on which to run the
-        power flow, defaults to network.now
 
     Returns
     -------
     p0 : pandas.DataFrame
         num_passive_branch x num_branch_outages DataFrame of new power flows
 
     """
 
     from .components import passive_branch_components
 
     if snapshots is None:
-        snapshot = network.now
-    elif isinstance(snapshots, collections.Iterable):
+        snapshots = network.snapshots
+
+    if isinstance(snapshots, collections.Iterable):
         logger.warning("Apologies LPF contingency, this only works for single snapshots at the moment, taking the first snapshot.")
         snapshot = snapshots[0]
     else:
         snapshot = snapshots
 
     network.lpf(snapshot)
 
@@ -163,15 +161,15 @@
     Computes Security-Constrained Linear Optimal Power Flow (SCLOPF).
 
     This ensures that no branch is overloaded even given the branch outages.
 
     Parameters
     ----------
     snapshots : list or index slice
-        A list of snapshots to optimise, must be a subset of network.snapshots, defaults to network.now
+        A list of snapshots to optimise, must be a subset of network.snapshots, defaults to network.snapshots
     branch_outages : list-like
         A list of passive branches which are to be tested for outages.
         If None, it's take as all network.passive_branches_i()
     solver_name : string
         Must be a solver name that pyomo recognises and that is installed, e.g. "glpk", "gurobi"
     skip_pre: bool, default False
         Skip the preliminary steps of computing topology, calculating dependent values and finding bus controls.
@@ -189,16 +187,15 @@
     -------
     None
     """
 
     if not skip_pre:
         network.determine_network_topology()
 
-    if snapshots is None:
-        snapshots = [network.now]
+    snapshots = _as_snapshots(network, snapshots)
 
     passive_branches = network.passive_branches()
 
     if branch_outages is None:
         branch_outages = passive_branches.index
 
     #prepare the sub networks by calculating BODF and preparing helper DataFrames
```

### Comparing `pypsa-0.8.0/pypsa/descriptors.py` & `pypsa-0.9.0/pypsa/descriptors.py`

 * *Files identical despite different names*

### Comparing `pypsa-0.8.0/pypsa/geo.py` & `pypsa-0.9.0/pypsa/geo.py`

 * *Files identical despite different names*

### Comparing `pypsa-0.8.0/pypsa/opf.py` & `pypsa-0.9.0/pypsa/opf.py`

 * *Files 12% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 __copyright__ = "Copyright 2015-2017 Tom Brown (FIAS), Jonas Hoersch (FIAS), David Schlachtberger (FIAS), GNU GPL 3"
 
 import pandas as pd
 import numpy as np
 from scipy.sparse.linalg import spsolve
 from pyomo.environ import (ConcreteModel, Var, Objective,
                            NonNegativeReals, Constraint, Reals,
-                           Suffix, Expression)
+                           Suffix, Expression, Binary)
 from pyomo.opt import SolverFactory
 from itertools import chain
 
 import logging
 logger = logging.getLogger(__name__)
 
 
@@ -45,15 +45,15 @@
 try:
     _pd_version = StrictVersion(pd.__version__)
 except ValueError:
     _pd_version = LooseVersion(pd.__version__)
 
 from .pf import (calculate_dependent_values, find_slack_bus,
                  find_bus_controls, calculate_B_H, calculate_PTDF, find_tree,
-                 find_cycles)
+                 find_cycles, _as_snapshots)
 from .opt import (l_constraint, l_objective, LExpression, LConstraint,
                   patch_optsolver_free_model_before_solving,
                   patch_optsolver_record_memusage_before_solving,
                   empty_network)
 from .descriptors import get_switchable_as_dense, allocate_series_dataframes
 
 
@@ -64,23 +64,27 @@
     raise NotImplementedError("Non-linear optimal power flow not supported yet")
 
 
 
 def define_generator_variables_constraints(network,snapshots):
 
     extendable_gens_i = network.generators.index[network.generators.p_nom_extendable]
-    fixed_gens_i = network.generators.index[~ network.generators.p_nom_extendable]
+    fixed_gens_i = network.generators.index[~network.generators.p_nom_extendable & ~network.generators.committable]
+    fixed_committable_gens_i = network.generators.index[~network.generators.p_nom_extendable & network.generators.committable]
+
+    if (network.generators.p_nom_extendable & network.generators.committable).any():
+        logger.warning("The following generators have both investment optimisation and unit commitment:\n{}\nCurrently PyPSA cannot do both these functions, so PyPSA is choosing investment optimisation for these generators.".format(network.generators.index[network.generators.p_nom_extendable & network.generators.committable]))
 
     p_min_pu = get_switchable_as_dense(network, 'Generator', 'p_min_pu')
     p_max_pu = get_switchable_as_dense(network, 'Generator', 'p_max_pu')
 
     ## Define generator dispatch variables ##
 
     gen_p_bounds = {(gen,sn) : (None,None)
-                    for gen in extendable_gens_i
+                    for gen in extendable_gens_i | fixed_committable_gens_i
                     for sn in snapshots}
 
     if len(fixed_gens_i):
         var_lower = p_min_pu.loc[:,fixed_gens_i].multiply(network.generators.loc[fixed_gens_i, 'p_nom'])
         var_upper = p_max_pu.loc[:,fixed_gens_i].multiply(network.generators.loc[fixed_gens_i, 'p_nom'])
 
         gen_p_bounds.update({(gen,sn) : (var_lower[gen][sn],var_upper[gen][sn])
@@ -119,14 +123,191 @@
                       network.model.generator_p_nom[gen])],"<=",0.]
                    for gen in extendable_gens_i for sn in snapshots}
     l_constraint(network.model, "generator_p_upper", gen_p_upper,
                  list(extendable_gens_i), snapshots)
 
 
 
+    ## Define committable generator statuses ##
+
+    network.model.generator_status = Var(list(fixed_committable_gens_i), snapshots,
+                                         within=Binary)
+
+    var_lower = p_min_pu.loc[:,fixed_committable_gens_i].multiply(network.generators.loc[fixed_committable_gens_i, 'p_nom'])
+    var_upper = p_max_pu.loc[:,fixed_committable_gens_i].multiply(network.generators.loc[fixed_committable_gens_i, 'p_nom'])
+
+
+    committable_gen_p_lower = {(gen,sn) : LConstraint(LExpression([(var_lower[gen][sn],network.model.generator_status[gen,sn]),(-1.,network.model.generator_p[gen,sn])]),"<=") for gen in fixed_committable_gens_i for sn in snapshots}
+
+    l_constraint(network.model, "committable_gen_p_lower", committable_gen_p_lower,
+                 list(fixed_committable_gens_i), snapshots)
+
+
+    committable_gen_p_upper = {(gen,sn) : LConstraint(LExpression([(var_upper[gen][sn],network.model.generator_status[gen,sn]),(-1.,network.model.generator_p[gen,sn])]),">=") for gen in fixed_committable_gens_i for sn in snapshots}
+
+    l_constraint(network.model, "committable_gen_p_upper", committable_gen_p_upper,
+                 list(fixed_committable_gens_i), snapshots)
+
+
+    ## Deal with minimum up time ##
+
+    up_time_gens = fixed_committable_gens_i[network.generators.loc[fixed_committable_gens_i,"min_up_time"] > 0]
+
+    for gen_i, gen in enumerate(up_time_gens):
+
+        min_up_time = network.generators.loc[gen,"min_up_time"]
+        initial_status = network.generators.loc[gen,"initial_status"]
+
+        blocks = max(1,len(snapshots)-min_up_time+1)
+
+        gen_up_time = {}
+
+        for i in range(blocks):
+            lhs = LExpression([(1,network.model.generator_status[gen,snapshots[j]]) for j in range(i,i+min_up_time)])
+
+            if i == 0:
+                rhs = LExpression([(min_up_time,network.model.generator_status[gen,snapshots[i]])],-min_up_time*initial_status)
+            else:
+                rhs = LExpression([(min_up_time,network.model.generator_status[gen,snapshots[i]]),(-min_up_time,network.model.generator_status[gen,snapshots[i-1]])])
+
+            gen_up_time[i] = LConstraint(lhs,">=",rhs)
+
+        l_constraint(network.model, "gen_up_time_{}".format(gen_i), gen_up_time,
+                     range(blocks))
+
+
+
+    ## Deal with minimum down time ##
+
+    down_time_gens = fixed_committable_gens_i[network.generators.loc[fixed_committable_gens_i,"min_down_time"] > 0]
+
+    for gen_i, gen in enumerate(down_time_gens):
+
+        min_down_time = network.generators.loc[gen,"min_down_time"]
+        initial_status = network.generators.loc[gen,"initial_status"]
+
+        blocks = max(1,len(snapshots)-min_down_time+1)
+
+        gen_down_time = {}
+
+        for i in range(blocks):
+            #sum of 1-status
+            lhs = LExpression([(-1,network.model.generator_status[gen,snapshots[j]]) for j in range(i,i+min_down_time)],min_down_time)
+
+            if i == 0:
+                rhs = LExpression([(-min_down_time,network.model.generator_status[gen,snapshots[i]])],min_down_time*initial_status)
+            else:
+                rhs = LExpression([(-min_down_time,network.model.generator_status[gen,snapshots[i]]),(min_down_time,network.model.generator_status[gen,snapshots[i-1]])])
+
+            gen_down_time[i] = LConstraint(lhs,">=",rhs)
+
+        l_constraint(network.model, "gen_down_time_{}".format(gen_i), gen_down_time,
+                     range(blocks))
+
+    ## Deal with start up costs ##
+
+    suc_gens = fixed_committable_gens_i[network.generators.loc[fixed_committable_gens_i,"start_up_cost"] > 0]
+
+    network.model.generator_start_up_cost = Var(list(suc_gens),snapshots,
+                                                domain=NonNegativeReals)
+
+    sucs = {}
+
+    for gen in suc_gens:
+        suc = network.generators.loc[gen,"start_up_cost"]
+        initial_status = network.generators.loc[gen,"initial_status"]
+
+        for i,sn in enumerate(snapshots):
+
+            if i == 0:
+                rhs = LExpression([(suc, network.model.generator_status[gen,sn])],-suc*initial_status)
+            else:
+                rhs = LExpression([(suc, network.model.generator_status[gen,sn]),(-suc,network.model.generator_status[gen,snapshots[i-1]])])
+
+            lhs = LExpression([(1,network.model.generator_start_up_cost[gen,sn])])
+
+            sucs[gen,sn] = LConstraint(lhs,">=",rhs)
+
+    l_constraint(network.model, "generator_start_up", sucs, list(suc_gens), snapshots)
+
+
+
+    ## Deal with shut down costs ##
+
+    sdc_gens = fixed_committable_gens_i[network.generators.loc[fixed_committable_gens_i,"shut_down_cost"] > 0]
+
+    network.model.generator_shut_down_cost = Var(list(sdc_gens),snapshots,
+                                                domain=NonNegativeReals)
+
+    sdcs = {}
+
+    for gen in sdc_gens:
+        sdc = network.generators.loc[gen,"shut_down_cost"]
+        initial_status = network.generators.loc[gen,"initial_status"]
+
+        for i,sn in enumerate(snapshots):
+
+            if i == 0:
+                rhs = LExpression([(-sdc, network.model.generator_status[gen,sn])],sdc*initial_status)
+            else:
+                rhs = LExpression([(-sdc, network.model.generator_status[gen,sn]),(sdc,network.model.generator_status[gen,snapshots[i-1]])])
+
+            lhs = LExpression([(1,network.model.generator_shut_down_cost[gen,sn])])
+
+            sdcs[gen,sn] = LConstraint(lhs,">=",rhs)
+
+    l_constraint(network.model, "generator_shut_down", sdcs, list(sdc_gens), snapshots)
+
+
+
+    ## Deal with ramp limits without unit commitment ##
+
+    sns = snapshots[1:]
+
+    ru_gens = network.generators.index[~network.generators.ramp_limit_up.isnull()]
+
+    ru = {}
+
+    for gen in ru_gens:
+        for i,sn in enumerate(sns):
+            if network.generators.at[gen, "p_nom_extendable"]:
+                lhs = LExpression([(1, network.model.generator_p[gen,sn]), (-1, network.model.generator_p[gen,snapshots[i]]), (-network.generators.at[gen, "ramp_limit_up"], network.model.generator_p_nom[gen])])
+            elif not network.generators.at[gen, "committable"]:
+                lhs = LExpression([(1, network.model.generator_p[gen,sn]), (-1, network.model.generator_p[gen,snapshots[i]])], -network.generators.at[gen, "ramp_limit_up"]*network.generators.at[gen, "p_nom"])
+            else:
+                lhs = LExpression([(1, network.model.generator_p[gen,sn]), (-1, network.model.generator_p[gen,snapshots[i]]), ((network.generators.at[gen, "ramp_limit_start_up"] - network.generators.at[gen, "ramp_limit_up"])*network.generators.at[gen, "p_nom"], network.model.generator_status[gen,snapshots[i]]), (-network.generators.at[gen, "ramp_limit_start_up"]*network.generators.at[gen, "p_nom"], network.model.generator_status[gen,sn])])
+
+            ru[gen,sn] = LConstraint(lhs,"<=")
+
+    l_constraint(network.model, "ramp_up", ru, list(ru_gens), sns)
+
+
+
+    rd_gens = network.generators.index[~network.generators.ramp_limit_down.isnull()]
+
+    rd = {}
+
+
+    for gen in rd_gens:
+        for i,sn in enumerate(sns):
+            if network.generators.at[gen, "p_nom_extendable"]:
+                lhs = LExpression([(1, network.model.generator_p[gen,sn]), (-1, network.model.generator_p[gen,snapshots[i]]), (network.generators.at[gen, "ramp_limit_down"], network.model.generator_p_nom[gen])])
+            elif not network.generators.at[gen, "committable"]:
+                lhs = LExpression([(1, network.model.generator_p[gen,sn]), (-1, network.model.generator_p[gen,snapshots[i]])], network.generators.loc[gen, "ramp_limit_down"]*network.generators.at[gen, "p_nom"])
+            else:
+                lhs = LExpression([(1, network.model.generator_p[gen,sn]), (-1, network.model.generator_p[gen,snapshots[i]]), ((network.generators.at[gen, "ramp_limit_down"] - network.generators.at[gen, "ramp_limit_shut_down"])*network.generators.at[gen, "p_nom"], network.model.generator_status[gen,sn]), (network.generators.at[gen, "ramp_limit_shut_down"]*network.generators.at[gen, "p_nom"], network.model.generator_status[gen,snapshots[i]])])
+
+            rd[gen,sn] = LConstraint(lhs,">=")
+
+    l_constraint(network.model, "ramp_down", rd, list(rd_gens), sns)
+
+
+
+
+
 def define_storage_variables_constraints(network,snapshots):
 
     sus = network.storage_units
     ext_sus_i = sus.index[sus.p_nom_extendable]
     fix_sus_i = sus.index[~ sus.p_nom_extendable]
 
     model = network.model
@@ -783,14 +964,19 @@
 
     passive_branches = network.passive_branches()
 
     extendable_passive_branches = passive_branches[passive_branches.s_nom_extendable]
 
     extendable_links = network.links[network.links.p_nom_extendable]
 
+    suc_gens_i = network.generators.index[~network.generators.p_nom_extendable & network.generators.committable & (network.generators.start_up_cost > 0)]
+
+    sdc_gens_i = network.generators.index[~network.generators.p_nom_extendable & network.generators.committable & (network.generators.shut_down_cost > 0)]
+
+
     objective = LExpression()
 
 
     for sn in snapshots:
         weight = network.snapshot_weightings[sn]
         for gen in network.generators.index:
             coefficient = network.generators.at[gen, "marginal_cost"] * weight
@@ -827,16 +1013,23 @@
                                 for b in extendable_passive_branches.index])
     objective.constant -= (extendable_passive_branches.capital_cost * extendable_passive_branches.s_nom).sum()
 
     objective.variables.extend([(extendable_links.at[b,"capital_cost"], model.link_p_nom[b])
                                 for b in extendable_links.index])
     objective.constant -= (extendable_links.capital_cost * extendable_links.p_nom).sum()
 
-    l_objective(model,objective)
 
+    ## Unit commitment costs
+
+    objective.variables.extend([(1, model.generator_start_up_cost[gen,sn]) for gen in suc_gens_i for sn in snapshots])
+
+    objective.variables.extend([(1, model.generator_shut_down_cost[gen,sn]) for gen in sdc_gens_i for sn in snapshots])
+
+
+    l_objective(model,objective)
 
 def extract_optimisation_results(network, snapshots, formulation="angles"):
 
     from .components import \
         passive_branch_components, branch_components, controllable_one_port_components
 
     if isinstance(snapshots, pd.DatetimeIndex) and _pd_version < '0.18.0':
@@ -973,30 +1166,44 @@
 
     if network.co2_limit is not None:
         try:
             network.co2_price = - network.model.dual[network.model.co2_constraint]
         except (AttributeError, KeyError) as e:
             logger.warning("Could not read out co2_price, although a co2_limit was set")
 
+    #extract unit commitment statuses
+    if network.generators.committable.any():
+        allocate_series_dataframes(network, {'Generator': ['status']})
 
-def network_lopf(network, snapshots=None, solver_name="glpk",
+        fixed_committable_gens_i = network.generators.index[~network.generators.p_nom_extendable & network.generators.committable]
+
+        if len(fixed_committable_gens_i) > 0:
+            network.generators_t.status.loc[snapshots,fixed_committable_gens_i] = \
+                as_series(model.generator_status).unstack(0)
+
+
+
+def network_lopf(network, snapshots=None, solver_name="glpk", solver_io=None,
                  skip_pre=False, extra_functionality=None, solver_options={},
                  keep_files=False, formulation="angles", ptdf_tolerance=0.,
                  free_memory={}):
     """
     Linear optimal power flow for a group of snapshots.
 
     Parameters
     ----------
     snapshots : list or index slice
         A list of snapshots to optimise, must be a subset of
-        network.snapshots, defaults to network.now
+        network.snapshots, defaults to network.snapshots
     solver_name : string
         Must be a solver name that pyomo recognises and that is
         installed, e.g. "glpk", "gurobi"
+    solver_io : string, default None
+        Solver Input-Output option, e.g. "python" to use "gurobipy" for
+        solver_name="gurobi"
     skip_pre: bool, default False
         Skip the preliminary steps of computing topology, calculating
         dependent values and finding bus controls.
     extra_functionality : callable function
         This function must take two arguments
         `extra_functionality(network,snapshots)` and is called after
         the model building is complete, but before it is sent to the
@@ -1027,18 +1234,15 @@
         network.determine_network_topology()
         calculate_dependent_values(network)
         for sub_network in network.sub_networks.obj:
             find_slack_bus(sub_network)
         logger.info("Performed preliminary steps")
 
 
-
-    if snapshots is None:
-        snapshots = [network.now]
-
+    snapshots = _as_snapshots(network, snapshots)
 
     logger.info("Building pyomo model using `%s` formulation", formulation)
     network.model = ConcreteModel("Linear Optimal Power Flow")
 
 
     define_generator_variables_constraints(network,snapshots)
 
@@ -1073,15 +1277,15 @@
         extra_functionality(network,snapshots)
 
 
     #tidy up auxilliary expressions
     del network._p_balance
 
     logger.info("Solving model using %s", solver_name)
-    opt = SolverFactory(solver_name)
+    opt = SolverFactory(solver_name, solver_io=solver_io)
 
     patch_optsolver_record_memusage_before_solving(opt, network)
 
     if isinstance(free_memory, string_types):
         free_memory = {free_memory}
 
     if 'pyomo_hack' in free_memory:
```

### Comparing `pypsa-0.8.0/pypsa/networkclustering.py` & `pypsa-0.9.0/pypsa/networkclustering.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,113 +22,96 @@
 __copyright__ = "Copyright 2015-2017 Tom Brown (FIAS), Jonas Hoersch (FIAS), GNU GPL 3"
 
 import numpy as np
 import pandas as pd
 import networkx as nx
 from collections import OrderedDict, namedtuple
 from itertools import repeat
-from six.moves import zip, range
+from six.moves import map, zip, range
 from six import itervalues, iteritems
 import six
 
 import logging
 logger = logging.getLogger(__name__)
 
 
 from .descriptors import OrderedGraph
 from .components import Network
 
 from . import components, io
 
 
+def _flatten_multiindex(m, join=' '):
+    if m.nlevels <= 1: return m
+    levels = map(m.get_level_values, range(m.nlevels))
+    return reduce(lambda x, y: x+join+y, levels, next(levels))
 
 def _consense(x):
     v = x.iat[0]
     assert ((x == v).all() or x.isnull().all())
     return v
 
 def _haversine(coords):
     lon, lat = np.deg2rad(np.asarray(coords)).T
     a = np.sin((lat[1]-lat[0])/2.)**2 + np.cos(lat[0]) * np.cos(lat[1]) * np.sin((lon[0] - lon[1])/2.)**2
     return 6371.000 * 2 * np.arctan2( np.sqrt(a), np.sqrt(1-a) )
 
 def aggregategenerators(network, busmap, with_time=True):
     attrs = network.components["Generator"]["attrs"]
-    columns = set(attrs.index[~attrs.varying]) | {'weight'}
     generators = network.generators.assign(bus=lambda df: df.bus.map(busmap))
+    columns = (set(attrs.index[attrs.static]) | {'weight'}) & set(generators.columns)
     grouper = [generators.bus, generators.carrier]
 
     weighting = generators.weight.groupby(grouper, axis=0).transform(lambda x: (x/x.sum()).fillna(1.))
     generators['p_nom_max'] /= weighting
     strategies = {'p_nom_max': np.min, 'weight': np.sum, 'p_nom': np.sum}
     strategies.update(zip(columns.difference(strategies), repeat(_consense)))
     new_df = generators.groupby(grouper, axis=0).agg(strategies)
-
-    new_index = pd.Index([bus + ' ' + carrier
-                          for bus, carrier in new_df.index.get_values()])
+    new_df.index = _flatten_multiindex(new_df.index).rename("name")
 
     new_pnl = dict()
     if with_time:
         for attr, df in iteritems(network.generators_t):
             if not df.empty:
-                time_dependent_old_b, time_dependent_new_b = \
-                    ((generators[attr + '_t'], new_df[attr + '_t'])
-                     if attr + '_t' in generators
-                     else (slice(None), slice(None)))
-
                 if attr == 'p_max_pu':
-                    df = df.multiply(weighting.loc[time_dependent_old_b], axis=1)
-                pnl_df = df.groupby(grouper, axis=1).sum().reindex(columns=new_df.index[time_dependent_new_b])
-                pnl_df.columns = new_index[time_dependent_new_b]
+                    df = df.multiply(weighting.loc[df.columns], axis=1)
+                pnl_df = df.groupby(grouper, axis=1).sum()
+                pnl_df.columns = _flatten_multiindex(pnl_df.columns).rename("name")
                 new_pnl[attr] = pnl_df
 
-    new_df.set_index(new_index, inplace=True)
     return new_df, new_pnl
 
 def aggregateoneport(network, busmap, component, with_time=True):
-
     attrs = network.components[component]["attrs"]
-    columns = set(attrs.index[~attrs.varying])
-
     old_df = getattr(network, network.components[component]["list_name"]).assign(bus=lambda df: df.bus.map(busmap))
-    if 'carrier' in columns:
-        grouper = [old_df.bus, old_df.carrier]
-    else:
-        grouper = old_df.bus
+    columns = set(attrs.index[attrs.static]) & set(old_df.columns)
+    grouper = old_df.bus if 'carrier' not in columns else [old_df.bus, old_df.carrier]
+
     strategies = {attr: (np.sum
                          if attr in {'p', 'q', 'p_set', 'q_set',
                                      'p_nom', 'p_nom_max', 'p_nom_min'}
                          else _consense)
                   for attr in columns}
     new_df = old_df.groupby(grouper).agg(strategies)
-    if 'carrier' in columns:
-        new_index = pd.Index([bus + ' ' + carrier
-                              for bus, carrier in new_df.index.get_values()])
-    else:
-        new_index = new_df.index
+    new_df.index = _flatten_multiindex(new_df.index).rename("name")
 
     new_pnl = dict()
     if with_time:
         old_pnl = network.pnl(component)
         for attr, df in iteritems(old_pnl):
             if not df.empty:
                 pnl_df = df.groupby(grouper, axis=1).sum()
-                time_dependent_b  = (new_df[attr + '_t']
-                                     if attr + '_t' in new_df
-                                     else slice(None))
-                pnl_df = pnl_df.reindex(columns=new_df.index[time_dependent_b])
-                pnl_df.columns = new_index[time_dependent_b]
+                pnl_df.columns = _flatten_multiindex(pnl_df.columns).rename("name")
                 new_pnl[attr] = pnl_df
 
-    new_df.set_index(new_index, inplace=True)
     return new_df, new_pnl
 
 def aggregatebuses(network, busmap, custom_strategies=dict()):
     attrs = network.components["Bus"]["attrs"]
-    columns = set(attrs.index[~attrs.varying])
+    columns = set(attrs.index[attrs.static]) & set(network.buses.columns)
 
     strategies = dict(x=np.mean, y=np.mean,
                       v_nom=np.max,
                       v_mag_pu_max=np.min, v_mag_pu_min=np.max)
     strategies.update(zip(columns.difference(strategies), repeat(_consense)))
     strategies.update(custom_strategies)
 
@@ -143,24 +126,24 @@
     #make sure all lines have same bus ordering
     positive_order = interlines.bus0_s < interlines.bus1_s
     interlines_p = interlines[positive_order]
     interlines_n = interlines[~ positive_order].rename(columns={"bus0_s":"bus1_s", "bus1_s":"bus0_s"})
     interlines_c = pd.concat((interlines_p,interlines_n))
 
     attrs = network.components["Line"]["attrs"]
-    columns = set(attrs.index[~attrs.varying]).difference(('bus0', 'bus1'))
+    columns = set(attrs.index[attrs.static]).difference(('name', 'bus0', 'bus1'))
 
     def aggregatelinegroup(l):
 
         # l.name is a tuple of the groupby index (bus0_s, bus1_s)
         length_s = _haversine(buses.loc[list(l.name),['x', 'y']])*line_length_factor
         v_nom_s = _consense(buses.loc[list(l.name),'v_nom'])
 
         voltage_factor = (np.asarray(network.buses.loc[l.bus0,'v_nom'])/v_nom_s)**2
-        length_factor = length_s/l['length']
+        length_factor = (length_s/l['length'])
 
         data = dict(
             r=1./(voltage_factor/(length_factor * l['r'])).sum(),
             x=1./(voltage_factor/(length_factor * l['x'])).sum(),
             g=(voltage_factor * length_factor * l['g']).sum(),
             b=(voltage_factor * length_factor * l['b']).sum(),
             terrain_factor=l['terrain_factor'].mean(),
@@ -186,18 +169,16 @@
 
     return lines, linemap_p, linemap_n, linemap
 
 def get_buses_linemap_and_lines(network, busmap, line_length_factor=1.0, bus_strategies=dict()):
     # compute new buses
     buses = aggregatebuses(network, busmap, bus_strategies)
 
-    lines = network.lines
-
-    lines['bus0_s'] = lines.bus0.map(busmap)
-    lines['bus1_s'] = lines.bus1.map(busmap)
+    lines = network.lines.assign(bus0_s=lambda df: df.bus0.map(busmap),
+                                 bus1_s=lambda df: df.bus1.map(busmap))
 
     # lines between different clusters
     interlines = lines.loc[lines['bus0_s'] != lines['bus1_s']]
     lines, linemap_p, linemap_n, linemap = aggregatelines(network, buses, interlines, line_length_factor)
     return (buses,
             linemap,
             linemap_p,
@@ -492,15 +473,15 @@
         for u in graph.node:
             neighbours = list(graph.adj[u].keys())
             if len(neighbours) == 1:
                 neighbour = neighbours[0]
                 count +=1
                 lines = list(graph.adj[u][neighbour].keys())
                 for line in lines:
-                    network.remove("Line",line.name)
+                    network.remove(*line)
                 network.remove("Bus",u)
                 busmap[busmap==u] = neighbour
         logger.info("{} deleted".format(count))
         if old_count == count:
             break
     return busmap
```

### Comparing `pypsa-0.8.0/README.rst` & `pypsa-0.9.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -11,25 +11,26 @@
 =====
 
 PyPSA stands for "Python for Power System Analysis". It is pronounced "pipes-ah".
 
 PyPSA is a `free software
 <http://www.gnu.org/philosophy/free-sw.en.html>`_ toolbox for
 simulating and optimising modern power systems that include features
-such as variable wind and solar generation, storage units, sector
-coupling and mixed alternating and direct current networks. PyPSA is
-designed to scale well with large networks and long time series.
+such as conventional generators with unit commitment, variable wind
+and solar generation, storage units, sector coupling and mixed
+alternating and direct current networks. PyPSA is designed to scale
+well with large networks and long time series.
 
 As of 2017 PyPSA is under heavy development and therefore it
 is recommended to use caution when using it in a production
 environment. Some APIs may change - those liable to be updated are
 listed in the `doc/todo.rst <doc/todo.rst>`_.
 
 PyPSA was initially developed by the `Renewable Energy Group
-<https://fias.uni-frankfurt.de/physics/schramm/complex-renewable-energy-networks/>`_
+<https://fias.uni-frankfurt.de/physics/schramm/renewable-energy-system-and-network-analysis/>`_
 at `FIAS <https://fias.uni-frankfurt.de/>`_ to carry out simulations
 for the `CoNDyNet project <http://condynet.de/>`_, financed by the
 `German Federal Ministry for Education and Research (BMBF) <https://www.bmbf.de/en/index.html>`_ as part of the `Stromnetze Research Initiative <http://forschung-stromnetze.info/projekte/grundlagen-und-konzepte-fuer-effiziente-dezentrale-stromnetze/>`_.
 
 
 Documentation
 =============
@@ -64,15 +65,15 @@
   the capacities of generation, storage and transmission)
 
 It has models for:
 
 * meshed multiply-connected AC and DC networks, with controllable
   converters between AC and DC networks
 * standard types for lines and transformers following the implementation in `pandapower <https://www.uni-kassel.de/eecs/fachgebiete/e2n/software/pandapower.html>`_
-* conventional dispatchable generators
+* conventional dispatchable generators with unit commitment
 * generators with time-varying power availability, such as
   wind and solar generators
 * storage units with efficiency losses
 * simple hydroelectricity with inflow and spillage
 * coupling with other energy carriers
 * basic components out of which more complicated assets can be built,
   such as Combined Heat and Power (CHP) units, heat pumps, resistive
@@ -89,15 +90,14 @@
 * Non-linear power flow solution using `analytic continuation
   <https://en.wikipedia.org/wiki/Holomorphic_embedding_load_flow_method>`_
   in the complex plane following `GridCal
   <https://github.com/SanPen/GridCal>`_
 
 Functionality that may be added in the future:
 
-* Unit Commitment using MILP
 * Short-circuit current calculations
 * Dynamic RMS simulations
 * Small signal stability analysis
 * Interactive web-based GUI with SVG
 * OPF with the full non-linear network equations
 * Dynamic EMT simulations
 * Unbalanced load flow
@@ -122,15 +122,15 @@
 
 .. image:: http://www.pypsa.org/img/storage-scigrid.png
 
 .. image:: http://www.pypsa.org/img/scigrid-curtailment.png
 
 .. image:: http://www.pypsa.org/img/meshed-ac-dc.png
 
-.. image:: http://www.pypsa.org/img/pre-4-network-181-LV-2.png
+.. image:: http://www.pypsa.org/img/euro-pie-pre-7-branch_limit-1-256.png
 
 
 
 What PyPSA uses under the hood
 ===============================
 
 PyPSA is written and tested to be compatible with both Python 2.7 and
```

### Comparing `pypsa-0.8.0/pypsa.egg-info/PKG-INFO` & `pypsa-0.9.0/pypsa.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pypsa
-Version: 0.8.0
+Version: 0.9.0
 Summary: Python for Power Systems Analysis
 Home-page: https://github.com/FRESNA/PyPSA
 Author: Tom Brown (FIAS), Jonas Hoersch (FIAS), David Schlachtberger (FIAS)
 Author-email: brown@fias.uni-frankfurt.de
 License: GPLv3
 Description: ################################
         Python for Power System Analysis
@@ -19,25 +19,26 @@
         =====
         
         PyPSA stands for "Python for Power System Analysis". It is pronounced "pipes-ah".
         
         PyPSA is a `free software
         <http://www.gnu.org/philosophy/free-sw.en.html>`_ toolbox for
         simulating and optimising modern power systems that include features
-        such as variable wind and solar generation, storage units, sector
-        coupling and mixed alternating and direct current networks. PyPSA is
-        designed to scale well with large networks and long time series.
+        such as conventional generators with unit commitment, variable wind
+        and solar generation, storage units, sector coupling and mixed
+        alternating and direct current networks. PyPSA is designed to scale
+        well with large networks and long time series.
         
         As of 2017 PyPSA is under heavy development and therefore it
         is recommended to use caution when using it in a production
         environment. Some APIs may change - those liable to be updated are
         listed in the `doc/todo.rst <doc/todo.rst>`_.
         
         PyPSA was initially developed by the `Renewable Energy Group
-        <https://fias.uni-frankfurt.de/physics/schramm/complex-renewable-energy-networks/>`_
+        <https://fias.uni-frankfurt.de/physics/schramm/renewable-energy-system-and-network-analysis/>`_
         at `FIAS <https://fias.uni-frankfurt.de/>`_ to carry out simulations
         for the `CoNDyNet project <http://condynet.de/>`_, financed by the
         `German Federal Ministry for Education and Research (BMBF) <https://www.bmbf.de/en/index.html>`_ as part of the `Stromnetze Research Initiative <http://forschung-stromnetze.info/projekte/grundlagen-und-konzepte-fuer-effiziente-dezentrale-stromnetze/>`_.
         
         
         Documentation
         =============
@@ -72,15 +73,15 @@
           the capacities of generation, storage and transmission)
         
         It has models for:
         
         * meshed multiply-connected AC and DC networks, with controllable
           converters between AC and DC networks
         * standard types for lines and transformers following the implementation in `pandapower <https://www.uni-kassel.de/eecs/fachgebiete/e2n/software/pandapower.html>`_
-        * conventional dispatchable generators
+        * conventional dispatchable generators with unit commitment
         * generators with time-varying power availability, such as
           wind and solar generators
         * storage units with efficiency losses
         * simple hydroelectricity with inflow and spillage
         * coupling with other energy carriers
         * basic components out of which more complicated assets can be built,
           such as Combined Heat and Power (CHP) units, heat pumps, resistive
@@ -97,15 +98,14 @@
         * Non-linear power flow solution using `analytic continuation
           <https://en.wikipedia.org/wiki/Holomorphic_embedding_load_flow_method>`_
           in the complex plane following `GridCal
           <https://github.com/SanPen/GridCal>`_
         
         Functionality that may be added in the future:
         
-        * Unit Commitment using MILP
         * Short-circuit current calculations
         * Dynamic RMS simulations
         * Small signal stability analysis
         * Interactive web-based GUI with SVG
         * OPF with the full non-linear network equations
         * Dynamic EMT simulations
         * Unbalanced load flow
@@ -130,15 +130,15 @@
         
         .. image:: http://www.pypsa.org/img/storage-scigrid.png
         
         .. image:: http://www.pypsa.org/img/scigrid-curtailment.png
         
         .. image:: http://www.pypsa.org/img/meshed-ac-dc.png
         
-        .. image:: http://www.pypsa.org/img/pre-4-network-181-LV-2.png
+        .. image:: http://www.pypsa.org/img/euro-pie-pre-7-branch_limit-1-256.png
         
         
         
         What PyPSA uses under the hood
         ===============================
         
         PyPSA is written and tested to be compatible with both Python 2.7 and
```

### Comparing `pypsa-0.8.0/pypsa.egg-info/SOURCES.txt` & `pypsa-0.9.0/pypsa.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -38,8 +38,9 @@
 pypsa/standard_types/transformer_types.csv
 test/test_ac_dc_lopf.py
 test/test_ac_dc_lpf.py
 test/test_lpf_against_pypower.py
 test/test_opf_storage.py
 test/test_pf_against_pandapower.py
 test/test_pf_against_pypower.py
-test/test_sclopf_scigrid.py
+test/test_sclopf_scigrid.py
+test/test_unit_commitment.py
```

### Comparing `pypsa-0.8.0/test/test_ac_dc_lopf.py` & `pypsa-0.9.0/test/test_ac_dc_lopf.py`

 * *Files identical despite different names*

### Comparing `pypsa-0.8.0/test/test_pf_against_pypower.py` & `pypsa-0.9.0/test/test_pf_against_pypower.py`

 * *Files 10% similar despite different names*

```diff
@@ -53,30 +53,30 @@
     network.transformers.model = "pi"
 
     network.pf()
 
     #compare branch flows
     for c in network.iterate_components(pypsa.components.passive_branch_components):
         for si in ["p0","p1","q0","q1"]:
-            si_pypsa = getattr(c.pnl,si).loc[network.now].values
+            si_pypsa = getattr(c.pnl,si).loc["now"].values
             si_pypower = results_df['branch'][si][c.df.original_index].values
             np.testing.assert_array_almost_equal(si_pypsa,si_pypower)
 
 
     #compare generator dispatch
     for s in ["p","q"]:
-        s_pypsa = getattr(network.generators_t,s).loc[network.now].values
+        s_pypsa = getattr(network.generators_t,s).loc["now"].values
         s_pypower = results_df["gen"][s].values
         np.testing.assert_array_almost_equal(s_pypsa,s_pypower)
 
 
     #compare voltages
-    v_mag_pypsa = network.buses_t.v_mag_pu.loc[network.now]
+    v_mag_pypsa = network.buses_t.v_mag_pu.loc["now"]
     v_mag_pypower = results_df["bus"]["v_mag_pu"]
 
     np.testing.assert_array_almost_equal(v_mag_pypsa,v_mag_pypower)
 
-    v_ang_pypsa = network.buses_t.v_ang.loc[network.now]
+    v_ang_pypsa = network.buses_t.v_ang.loc["now"]
     pypower_slack_angle = results_df["bus"]["v_ang"][results_df["bus"]["type"] == 3].values[0]
     v_ang_pypower = (results_df["bus"]["v_ang"] - pypower_slack_angle)*np.pi/180.
 
     np.testing.assert_array_almost_equal(v_ang_pypsa,v_ang_pypower)
```

### Comparing `pypsa-0.8.0/test/test_lpf_against_pypower.py` & `pypsa-0.9.0/test/test_lpf_against_pypower.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,21 +51,21 @@
     network.import_from_pypower_ppc(ppc)
     network.lpf()
 
 
 
     #compare generator dispatch
 
-    p_pypsa = network.generators_t.p.loc[network.now].values
+    p_pypsa = network.generators_t.p.loc["now"].values
     p_pypower = results_df['gen']["p"].values
 
     np.testing.assert_array_almost_equal(p_pypsa,p_pypower)
 
     #compare branch flows
     for item in ["lines","transformers"]:
         df = getattr(network,item)
         pnl = getattr(network,item + "_t")
 
         for si in ["p0","p1"]:
-            si_pypsa = getattr(pnl,si).loc[network.now].values
+            si_pypsa = getattr(pnl,si).loc["now"].values
             si_pypower = results_df['branch'][si][df.original_index].values
             np.testing.assert_array_almost_equal(si_pypsa,si_pypower)
```

### Comparing `pypsa-0.8.0/test/test_pf_against_pandapower.py` & `pypsa-0.9.0/test/test_pf_against_pandapower.py`

 * *Files 14% similar despite different names*

```diff
@@ -48,28 +48,28 @@
     n.pf(use_seed=True)
 
     #use same index for everything
     net.res_bus.index = net.bus.name.values
     net.res_line.index = net.line.name.values
 
     #compare bus angles
-    np.testing.assert_array_almost_equal(n.buses_t.v_ang.loc[n.now]*180/np.pi,net.res_bus.va_degree)
+    np.testing.assert_array_almost_equal(n.buses_t.v_ang.loc["now"]*180/np.pi,net.res_bus.va_degree)
 
     #compare bus voltage magnitudes
-    np.testing.assert_array_almost_equal(n.buses_t.v_mag_pu.loc[n.now],net.res_bus.vm_pu)
+    np.testing.assert_array_almost_equal(n.buses_t.v_mag_pu.loc["now"],net.res_bus.vm_pu)
 
     #compare bus active power (NB: pandapower uses load signs)
-    np.testing.assert_array_almost_equal(n.buses_t.p.loc[n.now],-net.res_bus.p_kw/1e3)
+    np.testing.assert_array_almost_equal(n.buses_t.p.loc["now"],-net.res_bus.p_kw/1e3)
 
     #compare bus active power (NB: pandapower uses load signs)
-    np.testing.assert_array_almost_equal(n.buses_t.q.loc[n.now],-net.res_bus.q_kvar/1e3)
+    np.testing.assert_array_almost_equal(n.buses_t.q.loc["now"],-net.res_bus.q_kvar/1e3)
 
     #compare branch flows
-    np.testing.assert_array_almost_equal(n.lines_t.p0.loc[n.now],net.res_line.p_from_kw/1e3)
-    np.testing.assert_array_almost_equal(n.lines_t.p1.loc[n.now],net.res_line.p_to_kw/1e3)
-    np.testing.assert_array_almost_equal(n.lines_t.q0.loc[n.now],net.res_line.q_from_kvar/1e3)
-    np.testing.assert_array_almost_equal(n.lines_t.q1.loc[n.now],net.res_line.q_to_kvar/1e3)
-
-    np.testing.assert_array_almost_equal(n.transformers_t.p0.loc[n.now],net.res_trafo.p_hv_kw/1e3)
-    np.testing.assert_array_almost_equal(n.transformers_t.p1.loc[n.now],net.res_trafo.p_lv_kw/1e3)
-    np.testing.assert_array_almost_equal(n.transformers_t.q0.loc[n.now],net.res_trafo.q_hv_kvar/1e3)
-    np.testing.assert_array_almost_equal(n.transformers_t.q1.loc[n.now],net.res_trafo.q_lv_kvar/1e3)
+    np.testing.assert_array_almost_equal(n.lines_t.p0.loc["now"],net.res_line.p_from_kw/1e3)
+    np.testing.assert_array_almost_equal(n.lines_t.p1.loc["now"],net.res_line.p_to_kw/1e3)
+    np.testing.assert_array_almost_equal(n.lines_t.q0.loc["now"],net.res_line.q_from_kvar/1e3)
+    np.testing.assert_array_almost_equal(n.lines_t.q1.loc["now"],net.res_line.q_to_kvar/1e3)
+
+    np.testing.assert_array_almost_equal(n.transformers_t.p0.loc["now"],net.res_trafo.p_hv_kw/1e3)
+    np.testing.assert_array_almost_equal(n.transformers_t.p1.loc["now"],net.res_trafo.p_lv_kw/1e3)
+    np.testing.assert_array_almost_equal(n.transformers_t.q0.loc["now"],net.res_trafo.q_hv_kvar/1e3)
+    np.testing.assert_array_almost_equal(n.transformers_t.q1.loc["now"],net.res_trafo.q_lv_kvar/1e3)
```

### Comparing `pypsa-0.8.0/test/test_opf_storage.py` & `pypsa-0.9.0/test/test_opf_storage.py`

 * *Files identical despite different names*

### Comparing `pypsa-0.8.0/test/test_sclopf_scigrid.py` & `pypsa-0.9.0/test/test_sclopf_scigrid.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,32 +16,30 @@
     #test results were generated with GLPK and other solvers may differ
     solver_name = "glpk"
 
     #There are some infeasibilities without line extensions
     for line_name in ["316","527","602"]:
         network.lines.loc[line_name,"s_nom"] = 1200
 
-    network.now = network.snapshots[0]
-
     #choose the contingencies
     branch_outages = network.lines.index[:3]
 
     print("Performing security-constrained linear OPF:")
 
-    network.sclopf(branch_outages=branch_outages)
+    network.sclopf(network.snapshots[0],branch_outages=branch_outages)
 
     #For the PF, set the P to the optimised P
     network.generators_t.p_set = network.generators_t.p.copy()
     network.generators.loc[:,'p_set_t'] = True
     network.storage_units_t.p_set = network.storage_units_t.p.copy()
     network.storage_units.loc[:,'p_set_t'] = True
 
     #Check no lines are overloaded with the linear contingency analysis
 
-    p0_test = network.lpf_contingency(branch_outages=branch_outages)
+    p0_test = network.lpf_contingency(network.snapshots[0],branch_outages=branch_outages)
 
     #check loading as per unit of s_nom in each contingency
 
     max_loading = abs(p0_test.divide(network.passive_branches().s_nom,axis=0)).describe().loc["max"]
 
 
     np.testing.assert_array_almost_equal(max_loading,np.ones((len(max_loading))))
```

### Comparing `pypsa-0.8.0/test/test_ac_dc_lpf.py` & `pypsa-0.9.0/test/test_ac_dc_lpf.py`

 * *Files identical despite different names*

### Comparing `pypsa-0.8.0/setup.py` & `pypsa-0.9.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,24 +7,24 @@
 
 
 with open('README.rst', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='pypsa',
-    version='0.8.0',
+    version='0.9.0',
     author='Tom Brown (FIAS), Jonas Hoersch (FIAS), David Schlachtberger (FIAS)',
     author_email='brown@fias.uni-frankfurt.de',
     description='Python for Power Systems Analysis',
     long_description=long_description,
     url='https://github.com/FRESNA/PyPSA',
     license='GPLv3',
     packages=find_packages(exclude=['doc', 'test']),
     include_package_data=True,
-    install_requires=['numpy','pyomo','scipy','pandas>=0.17.1','networkx>=1.10'],
+    install_requires=['numpy','pyomo','scipy','pandas>=0.19.0','networkx>=1.10'],
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Environment :: Console',
         'Intended Audience :: Science/Research',
         'License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)',
         'Natural Language :: English',
         'Operating System :: OS Independent',
```

