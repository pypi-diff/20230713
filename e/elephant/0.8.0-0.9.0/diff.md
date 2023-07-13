# Comparing `tmp/elephant-0.8.0.tar.gz` & `tmp/elephant-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/elephant-0.8.0.tar", last modified: Fri Aug  7 12:55:55 2020, max compression
+gzip compressed data, was "dist/elephant-0.9.0.tar", last modified: Fri Nov 13 11:41:46 2020, max compression
```

## Comparing `elephant-0.8.0.tar` & `elephant-0.9.0.tar`

### file list

```diff
@@ -1,157 +1,172 @@
-drwxrwxr-x   0 ulianych  (1001) ulianych  (1001)        0 2020-08-07 12:55:55.517376 elephant-0.8.0/
--rw-rw-r--   0 ulianych  (1001) ulianych  (1001)     1506 2019-07-01 07:26:01.000000 elephant-0.8.0/LICENSE.txt
--rw-rw-r--   0 ulianych  (1001) ulianych  (1001)      562 2020-08-04 13:50:24.000000 elephant-0.8.0/MANIFEST.in
--rw-rw-r--   0 ulianych  (1001) ulianych  (1001)     2200 2020-08-07 12:55:55.517376 elephant-0.8.0/PKG-INFO
--rw-rw-r--   0 ulianych  (1001) ulianych  (1001)     1173 2020-08-07 12:55:31.000000 elephant-0.8.0/README.md
-drwxrwxr-x   0 ulianych  (1001) ulianych  (1001)        0 2020-08-07 12:55:55.469375 elephant-0.8.0/doc/
--rw-rw-r--   0 ulianych  (1001) ulianych  (1001)     5572 2019-05-15 09:32:00.000000 elephant-0.8.0/doc/Makefile
--rw-rw-r--   0 ulianych  (1001) ulianych  (1001)      333 2020-08-04 13:50:24.000000 elephant-0.8.0/doc/acknowledgments.rst
--rw-rw-r--   0 ulianych  (1001) ulianych  (1001)     2380 2020-08-04 13:50:24.000000 elephant-0.8.0/doc/authors.rst
-drwxrwxr-x   0 ulianych  (1001) ulianych  (1001)        0 2020-08-07 12:55:55.469375 elephant-0.8.0/doc/bib/
--rw-rw-r--   0 ulianych  (1001) ulianych  (1001)     2263 2020-08-04 13:50:24.000000 elephant-0.8.0/doc/bib/elephant.bib
--rw-rw-r--   0 ulianych  (1001) ulianych  (1001)    11515 2020-08-04 13:50:24.000000 elephant-0.8.0/doc/conf.py
--rw-rw-r--   0 ulianych  (1001) ulianych  (1001)     2392 2020-08-04 13:50:24.000000 elephant-0.8.0/doc/developers_guide.rst
--rw-rw-r--   0 ulianych  (1001) ulianych  (1001)     1248 2020-08-04 13:50:24.000000 elephant-0.8.0/doc/documentation_guide.rst
--rw-rw-r--   0 ulianych  (1001) ulianych  (1001)     1075 2020-08-04 13:50:24.000000 elephant-0.8.0/doc/get_in_touch.rst
-drwxrwxr-x   0 ulianych  (1001) ulianych  (1001)        0 2020-08-07 12:55:55.469375 elephant-0.8.0/doc/images/
--rw-rw-r--   0 ulianych  (1001) ulianych  (1001)     2238 2019-05-15 09:32:00.000000 elephant-0.8.0/doc/images/elephant_favicon.ico
--rw-rw-r--   0 ulianych  (1001) ulianych  (1001)   116686 2019-05-15 09:32:00.000000 elephant-0.8.0/doc/images/elephant_logo.png
--rw-rw-r--   0 ulianych  (1001) ulianych  (1001)    12239 2019-05-15 09:32:00.000000 elephant-0.8.0/doc/images/elephant_logo_sidebar.png
--rw-rw-r--   0 ulianych  (1001) ulianych  (1001)     1774 2020-08-04 13:50:24.000000 elephant-0.8.0/doc/index.rst
--rw-rw-r--   0 ulianych  (1001) ulianych  (1001)     3964 2020-08-04 13:50:24.000000 elephant-0.8.0/doc/install.rst
--rw-rw-r--   0 ulianych  (1001) ulianych  (1001)     4710 2020-08-04 13:50:24.000000 elephant-0.8.0/doc/maintainers_guide.rst
--rw-rw-r--   0 ulianych  (1001) ulianych  (1001)     5100 2019-05-15 09:32:00.000000 elephant-0.8.0/doc/make.bat
--rw-rw-r--   0 ulianych  (1001) ulianych  (1001)      756 2020-08-04 13:50:24.000000 elephant-0.8.0/doc/modules.rst
-drwxrwxr-x   0 ulianych  (1001) ulianych  (1001)        0 2020-08-07 12:55:55.473375 elephant-0.8.0/doc/reference/
--rw-rw-r--   0 ulianych  (1001) ulianych  (1001)      310 2020-08-04 13:50:24.000000 elephant-0.8.0/doc/reference/asset.rst
--rw-rw-r--   0 ulianych  (1001) ulianych  (1001)      159 2020-08-04 13:50:24.000000 elephant-0.8.0/doc/reference/cell_assembly_detection.rst
--rw-rw-r--   0 ulianych  (1001) ulianych  (1001)      176 2020-08-04 13:50:24.000000 elephant-0.8.0/doc/reference/change_point_detection.rst
--rw-rw-r--   0 ulianych  (1001) ulianych  (1001)      140 2020-08-04 13:50:24.000000 elephant-0.8.0/doc/reference/conversion.rst
--rw-rw-r--   0 ulianych  (1001) ulianych  (1001)      228 2020-08-04 13:50:24.000000 elephant-0.8.0/doc/reference/cubic.rst
--rw-rw-r--   0 ulianych  (1001) ulianych  (1001)      158 2020-08-04 13:50:24.000000 elephant-0.8.0/doc/reference/current_source_density.rst
--rw-rw-r--   0 ulianych  (1001) ulianych  (1001)      407 2020-08-04 13:50:24.000000 elephant-0.8.0/doc/reference/gpfa.rst
--rw-rw-r--   0 ulianych  (1001) ulianych  (1001)       58 2020-08-04 13:50:24.000000 elephant-0.8.0/doc/reference/kernels.rst
--rw-rw-r--   0 ulianych  (1001) ulianych  (1001)      115 2020-08-04 13:50:24.000000 elephant-0.8.0/doc/reference/neo_tools.rst
--rw-rw-r--   0 ulianych  (1001) ulianych  (1001)      140 2020-08-04 13:50:24.000000 elephant-0.8.0/doc/reference/pandas_bridge.rst
--rw-rw-r--   0 ulianych  (1001) ulianych  (1001)       62 2020-08-04 13:50:24.000000 elephant-0.8.0/doc/reference/parallel.rst
--rw-rw-r--   0 ulianych  (1001) ulianych  (1001)      132 2020-08-04 13:50:24.000000 elephant-0.8.0/doc/reference/phase_analysis.rst
--rw-rw-r--   0 ulianych  (1001) ulianych  (1001)      249 2020-08-04 13:50:24.000000 elephant-0.8.0/doc/reference/signal_processing.rst
--rw-rw-r--   0 ulianych  (1001) ulianych  (1001)      186 2020-08-04 13:50:24.000000 elephant-0.8.0/doc/reference/spade.rst
--rw-rw-r--   0 ulianych  (1001) ulianych  (1001)      102 2020-08-04 13:50:24.000000 elephant-0.8.0/doc/reference/spectral.rst
--rw-rw-r--   0 ulianych  (1001) ulianych  (1001)      277 2020-08-04 13:50:24.000000 elephant-0.8.0/doc/reference/spike_train_correlation.rst
--rw-rw-r--   0 ulianych  (1001) ulianych  (1001)      187 2020-08-04 13:50:24.000000 elephant-0.8.0/doc/reference/spike_train_dissimilarity.rst
--rw-rw-r--   0 ulianych  (1001) ulianych  (1001)      284 2020-08-04 13:50:24.000000 elephant-0.8.0/doc/reference/spike_train_generation.rst
--rw-rw-r--   0 ulianych  (1001) ulianych  (1001)      278 2020-08-04 13:50:24.000000 elephant-0.8.0/doc/reference/spike_train_surrogates.rst
--rw-rw-r--   0 ulianych  (1001) ulianych  (1001)      115 2020-08-04 13:50:24.000000 elephant-0.8.0/doc/reference/sta.rst
--rw-rw-r--   0 ulianych  (1001) ulianych  (1001)      118 2020-08-04 13:50:24.000000 elephant-0.8.0/doc/reference/statistics.rst
-drwxrwxr-x   0 ulianych  (1001) ulianych  (1001)        0 2020-08-07 12:55:55.461375 elephant-0.8.0/doc/reference/toctree/
-drwxrwxr-x   0 ulianych  (1001) ulianych  (1001)        0 2020-08-07 12:55:55.473375 elephant-0.8.0/doc/reference/toctree/kernels/
--rw-rw-r--   0 ulianych  (1001) ulianych  (1001)      508 2020-08-04 13:50:24.000000 elephant-0.8.0/doc/reference/toctree/kernels/elephant.kernels.AlphaKernel.rst
--rw-rw-r--   0 ulianych  (1001) ulianych  (1001)      615 2020-08-04 13:50:24.000000 elephant-0.8.0/doc/reference/toctree/kernels/elephant.kernels.EpanechnikovLikeKernel.rst
--rw-rw-r--   0 ulianych  (1001) ulianych  (1001)      568 2020-08-04 13:50:24.000000 elephant-0.8.0/doc/reference/toctree/kernels/elephant.kernels.ExponentialKernel.rst
--rw-rw-r--   0 ulianych  (1001) ulianych  (1001)      538 2020-08-04 13:50:24.000000 elephant-0.8.0/doc/reference/toctree/kernels/elephant.kernels.GaussianKernel.rst
--rw-rw-r--   0 ulianych  (1001) ulianych  (1001)      548 2020-08-04 13:50:24.000000 elephant-0.8.0/doc/reference/toctree/kernels/elephant.kernels.LaplacianKernel.rst
--rw-rw-r--   0 ulianych  (1001) ulianych  (1001)      568 2020-08-04 13:50:24.000000 elephant-0.8.0/doc/reference/toctree/kernels/elephant.kernels.RectangularKernel.rst
--rw-rw-r--   0 ulianych  (1001) ulianych  (1001)      558 2020-08-04 13:50:24.000000 elephant-0.8.0/doc/reference/toctree/kernels/elephant.kernels.TriangularKernel.rst
--rw-rw-r--   0 ulianych  (1001) ulianych  (1001)      421 2020-08-04 13:50:24.000000 elephant-0.8.0/doc/reference/unitary_event_analysis.rst
--rw-rw-r--   0 ulianych  (1001) ulianych  (1001)      111 2020-08-04 13:50:24.000000 elephant-0.8.0/doc/reference/waveform_features.rst
--rw-rw-r--   0 ulianych  (1001) ulianych  (1001)    14695 2020-08-07 12:55:31.000000 elephant-0.8.0/doc/release_notes.rst
--rw-rw-r--   0 ulianych  (1001) ulianych  (1001)    29332 2020-08-07 12:33:53.000000 elephant-0.8.0/doc/style_guide.rst
-drwxrwxr-x   0 ulianych  (1001) ulianych  (1001)        0 2020-08-07 12:55:55.509375 elephant-0.8.0/doc/tutorials/
--rw-rw-r--   0 ulianych  (1001) ulianych  (1001)   334256 2020-08-07 12:55:31.000000 elephant-0.8.0/doc/tutorials/asset.ipynb
--rw-rw-r--   0 ulianych  (1001) ulianych  (1001) 44142233 2020-05-25 13:44:04.000000 elephant-0.8.0/doc/tutorials/asset_showcase_500.nix
--rw-rw-r--   0 ulianych  (1001) ulianych  (1001)  1578043 2020-08-05 09:48:24.000000 elephant-0.8.0/doc/tutorials/gpfa.ipynb
--rw-rw-r--   0 ulianych  (1001) ulianych  (1001)    13125 2020-08-07 12:33:53.000000 elephant-0.8.0/doc/tutorials/parallel.ipynb
--rw-rw-r--   0 ulianych  (1001) ulianych  (1001)    19837 2020-08-05 09:48:24.000000 elephant-0.8.0/doc/tutorials/statistics.ipynb
--rw-rw-r--   0 ulianych  (1001) ulianych  (1001)    15339 2020-08-07 12:33:53.000000 elephant-0.8.0/doc/tutorials/unitary_event_analysis.ipynb
--rw-rw-r--   0 ulianych  (1001) ulianych  (1001)     2256 2020-08-05 09:48:24.000000 elephant-0.8.0/doc/tutorials.rst
-drwxrwxr-x   0 ulianych  (1001) ulianych  (1001)        0 2020-08-07 12:55:55.509375 elephant-0.8.0/elephant/
--rw-rw-r--   0 ulianych  (1001) ulianych  (1001)        5 2020-08-07 12:55:31.000000 elephant-0.8.0/elephant/VERSION
--rw-rw-r--   0 ulianych  (1001) ulianych  (1001)     1394 2020-08-07 10:14:09.000000 elephant-0.8.0/elephant/__init__.py
--rw-rw-r--   0 ulianych  (1001) ulianych  (1001)    72460 2020-08-07 12:33:53.000000 elephant-0.8.0/elephant/asset.py
--rw-rw-r--   0 ulianych  (1001) ulianych  (1001)    49208 2020-08-07 12:33:53.000000 elephant-0.8.0/elephant/cell_assembly_detection.py
--rw-rw-r--   0 ulianych  (1001) ulianych  (1001)    18505 2020-08-07 12:33:53.000000 elephant-0.8.0/elephant/change_point_detection.py
--rw-rw-r--   0 ulianych  (1001) ulianych  (1001)    37204 2020-08-07 12:33:53.000000 elephant-0.8.0/elephant/conversion.py
--rw-rw-r--   0 ulianych  (1001) ulianych  (1001)     6950 2020-08-07 12:33:53.000000 elephant-0.8.0/elephant/cubic.py
--rw-rw-r--   0 ulianych  (1001) ulianych  (1001)    14122 2020-08-07 12:33:53.000000 elephant-0.8.0/elephant/current_source_density.py
-drwxrwxr-x   0 ulianych  (1001) ulianych  (1001)        0 2020-08-07 12:55:55.513376 elephant-0.8.0/elephant/current_source_density_src/
--rw-rw-r--   0 ulianych  (1001) ulianych  (1001)    42718 2020-08-04 13:50:24.000000 elephant-0.8.0/elephant/current_source_density_src/KCSD.py
--rw-rw-r--   0 ulianych  (1001) ulianych  (1001)     4060 2019-05-15 09:32:00.000000 elephant-0.8.0/elephant/current_source_density_src/README.md
--rw-rw-r--   0 ulianych  (1001) ulianych  (1001)       62 2020-02-19 12:59:34.000000 elephant-0.8.0/elephant/current_source_density_src/__init__.py
--rw-rw-r--   0 ulianych  (1001) ulianych  (1001)     4939 2020-02-19 12:59:34.000000 elephant-0.8.0/elephant/current_source_density_src/basis_functions.py
--rw-rw-r--   0 ulianych  (1001) ulianych  (1001)    35175 2020-02-19 12:59:34.000000 elephant-0.8.0/elephant/current_source_density_src/icsd.py
--rw-rw-r--   0 ulianych  (1001) ulianych  (1001)    65926 2019-05-15 09:32:00.000000 elephant-0.8.0/elephant/current_source_density_src/test_data.mat
--rw-rw-r--   0 ulianych  (1001) ulianych  (1001)    11986 2020-08-04 13:50:24.000000 elephant-0.8.0/elephant/current_source_density_src/utility_functions.py
-drwxrwxr-x   0 ulianych  (1001) ulianych  (1001)        0 2020-08-07 12:55:55.513376 elephant-0.8.0/elephant/gpfa/
--rw-rw-r--   0 ulianych  (1001) ulianych  (1001)      127 2020-08-04 13:50:24.000000 elephant-0.8.0/elephant/gpfa/__init__.py
--rw-rw-r--   0 ulianych  (1001) ulianych  (1001)    18587 2020-08-07 12:33:53.000000 elephant-0.8.0/elephant/gpfa/gpfa.py
--rw-rw-r--   0 ulianych  (1001) ulianych  (1001)    20639 2020-08-04 13:50:24.000000 elephant-0.8.0/elephant/gpfa/gpfa_core.py
--rw-rw-r--   0 ulianych  (1001) ulianych  (1001)    17821 2020-08-07 12:33:53.000000 elephant-0.8.0/elephant/gpfa/gpfa_util.py
--rw-rw-r--   0 ulianych  (1001) ulianych  (1001)    27594 2020-08-07 12:33:53.000000 elephant-0.8.0/elephant/kernels.py
--rw-rw-r--   0 ulianych  (1001) ulianych  (1001)     7156 2020-08-07 12:33:53.000000 elephant-0.8.0/elephant/neo_tools.py
--rw-rw-r--   0 ulianych  (1001) ulianych  (1001)    21991 2020-08-07 12:33:53.000000 elephant-0.8.0/elephant/pandas_bridge.py
-drwxrwxr-x   0 ulianych  (1001) ulianych  (1001)        0 2020-08-07 12:55:55.513376 elephant-0.8.0/elephant/parallel/
--rw-rw-r--   0 ulianych  (1001) ulianych  (1001)     1234 2020-08-07 12:33:53.000000 elephant-0.8.0/elephant/parallel/__init__.py
--rw-rw-r--   0 ulianych  (1001) ulianych  (1001)     2050 2020-08-04 13:50:24.000000 elephant-0.8.0/elephant/parallel/mpi.py
--rw-rw-r--   0 ulianych  (1001) ulianych  (1001)     3668 2020-08-07 12:33:53.000000 elephant-0.8.0/elephant/parallel/parallel.py
--rw-rw-r--   0 ulianych  (1001) ulianych  (1001)     7382 2020-08-04 13:50:24.000000 elephant-0.8.0/elephant/phase_analysis.py
--rw-rw-r--   0 ulianych  (1001) ulianych  (1001)    36193 2020-08-07 12:33:53.000000 elephant-0.8.0/elephant/signal_processing.py
--rw-rw-r--   0 ulianych  (1001) ulianych  (1001)    90713 2020-08-07 12:33:53.000000 elephant-0.8.0/elephant/spade.py
-drwxrwxr-x   0 ulianych  (1001) ulianych  (1001)        0 2020-08-07 12:55:55.513376 elephant-0.8.0/elephant/spade_src/
--rw-rw-r--   0 ulianych  (1001) ulianych  (1001)     1311 2019-05-15 09:32:00.000000 elephant-0.8.0/elephant/spade_src/LICENSE
--rw-rw-r--   0 ulianych  (1001) ulianych  (1001)        0 2020-02-19 12:59:34.000000 elephant-0.8.0/elephant/spade_src/__init__.py
--rw-rw-r--   0 ulianych  (1001) ulianych  (1001)    11273 2020-08-04 13:50:24.000000 elephant-0.8.0/elephant/spade_src/fast_fca.py
--rw-rw-r--   0 ulianych  (1001) ulianych  (1001)    19153 2020-08-07 12:33:53.000000 elephant-0.8.0/elephant/spectral.py
--rw-rw-r--   0 ulianych  (1001) ulianych  (1001)    40712 2020-08-07 12:33:53.000000 elephant-0.8.0/elephant/spike_train_correlation.py
--rw-rw-r--   0 ulianych  (1001) ulianych  (1001)    18784 2020-08-07 12:33:53.000000 elephant-0.8.0/elephant/spike_train_dissimilarity.py
--rw-rw-r--   0 ulianych  (1001) ulianych  (1001)    49932 2020-08-07 12:33:53.000000 elephant-0.8.0/elephant/spike_train_generation.py
--rw-rw-r--   0 ulianych  (1001) ulianych  (1001)    42093 2020-08-07 12:33:53.000000 elephant-0.8.0/elephant/spike_train_surrogates.py
--rw-rw-r--   0 ulianych  (1001) ulianych  (1001)    13361 2020-08-07 12:33:53.000000 elephant-0.8.0/elephant/sta.py
--rw-rw-r--   0 ulianych  (1001) ulianych  (1001)    40381 2020-08-07 12:33:53.000000 elephant-0.8.0/elephant/statistics.py
-drwxrwxr-x   0 ulianych  (1001) ulianych  (1001)        0 2020-08-07 12:55:55.517376 elephant-0.8.0/elephant/test/
--rw-rw-r--   0 ulianych  (1001) ulianych  (1001)        0 2020-02-19 12:59:34.000000 elephant-0.8.0/elephant/test/__init__.py
--rw-rw-r--   0 ulianych  (1001) ulianych  (1001)     1682 2020-08-07 12:33:53.000000 elephant-0.8.0/elephant/test/make_spike_extraction_test_data.py
--rw-rw-r--   0 ulianych  (1001) ulianych  (1001)    62953 2019-07-01 07:26:01.000000 elephant-0.8.0/elephant/test/spike_extraction_test_data.txt
--rw-rw-r--   0 ulianych  (1001) ulianych  (1001)    22307 2020-08-07 12:33:53.000000 elephant-0.8.0/elephant/test/test_asset.py
--rw-rw-r--   0 ulianych  (1001) ulianych  (1001)     9254 2020-08-07 12:33:53.000000 elephant-0.8.0/elephant/test/test_cell_assembly_detection.py
--rw-rw-r--   0 ulianych  (1001) ulianych  (1001)     9271 2020-08-07 12:33:53.000000 elephant-0.8.0/elephant/test/test_change_point_detection.py
--rw-rw-r--   0 ulianych  (1001) ulianych  (1001)    28008 2020-08-07 12:33:53.000000 elephant-0.8.0/elephant/test/test_conversion.py
--rw-rw-r--   0 ulianych  (1001) ulianych  (1001)     6715 2020-02-19 13:05:30.000000 elephant-0.8.0/elephant/test/test_csd.py
--rw-rw-r--   0 ulianych  (1001) ulianych  (1001)     5494 2020-08-07 12:33:53.000000 elephant-0.8.0/elephant/test/test_cubic.py
--rw-rw-r--   0 ulianych  (1001) ulianych  (1001)     9322 2020-08-07 12:33:53.000000 elephant-0.8.0/elephant/test/test_gpfa.py
--rw-rw-r--   0 ulianych  (1001) ulianych  (1001)    40516 2020-08-07 12:33:53.000000 elephant-0.8.0/elephant/test/test_icsd.py
--rw-rw-r--   0 ulianych  (1001) ulianych  (1001)     8373 2020-08-07 12:33:53.000000 elephant-0.8.0/elephant/test/test_kcsd.py
--rw-rw-r--   0 ulianych  (1001) ulianych  (1001)    16415 2020-08-07 12:33:53.000000 elephant-0.8.0/elephant/test/test_kernels.py
--rw-rw-r--   0 ulianych  (1001) ulianych  (1001)    53443 2020-08-07 12:33:53.000000 elephant-0.8.0/elephant/test/test_neo_tools.py
--rw-rw-r--   0 ulianych  (1001) ulianych  (1001)   113866 2020-08-07 12:33:53.000000 elephant-0.8.0/elephant/test/test_pandas_bridge.py
--rw-rw-r--   0 ulianych  (1001) ulianych  (1001)     1587 2020-08-04 13:50:24.000000 elephant-0.8.0/elephant/test/test_parallel.py
--rw-rw-r--   0 ulianych  (1001) ulianych  (1001)     8620 2020-08-07 12:33:53.000000 elephant-0.8.0/elephant/test/test_phase_analysis.py
--rw-rw-r--   0 ulianych  (1001) ulianych  (1001)    52003 2020-08-07 12:33:53.000000 elephant-0.8.0/elephant/test/test_signal_processing.py
--rw-rw-r--   0 ulianych  (1001) ulianych  (1001)    25885 2020-08-07 12:33:53.000000 elephant-0.8.0/elephant/test/test_spade.py
--rw-rw-r--   0 ulianych  (1001) ulianych  (1001)    16044 2020-08-07 12:33:53.000000 elephant-0.8.0/elephant/test/test_spectral.py
--rw-rw-r--   0 ulianych  (1001) ulianych  (1001)    35665 2020-08-07 12:33:53.000000 elephant-0.8.0/elephant/test/test_spike_train_correlation.py
--rw-rw-r--   0 ulianych  (1001) ulianych  (1001)    27288 2020-08-07 12:33:53.000000 elephant-0.8.0/elephant/test/test_spike_train_dissimilarity.py
--rw-rw-r--   0 ulianych  (1001) ulianych  (1001)    35735 2020-08-07 12:33:53.000000 elephant-0.8.0/elephant/test/test_spike_train_generation.py
--rw-rw-r--   0 ulianych  (1001) ulianych  (1001)    19487 2020-08-07 12:33:53.000000 elephant-0.8.0/elephant/test/test_spike_train_surrogates.py
--rw-rw-r--   0 ulianych  (1001) ulianych  (1001)    19061 2020-08-07 12:33:53.000000 elephant-0.8.0/elephant/test/test_sta.py
--rw-rw-r--   0 ulianych  (1001) ulianych  (1001)    34596 2020-08-07 12:33:53.000000 elephant-0.8.0/elephant/test/test_statistics.py
--rw-rw-r--   0 ulianych  (1001) ulianych  (1001)    20948 2020-08-07 12:33:53.000000 elephant-0.8.0/elephant/test/test_unitary_event_analysis.py
--rw-rw-r--   0 ulianych  (1001) ulianych  (1001)     3643 2020-08-04 13:50:24.000000 elephant-0.8.0/elephant/test/test_waveform_features.py
--rw-rw-r--   0 ulianych  (1001) ulianych  (1001)    27776 2020-08-07 12:33:53.000000 elephant-0.8.0/elephant/unitary_event_analysis.py
--rw-rw-r--   0 ulianych  (1001) ulianych  (1001)     2289 2020-08-07 12:33:53.000000 elephant-0.8.0/elephant/utils.py
--rw-rw-r--   0 ulianych  (1001) ulianych  (1001)     3459 2020-08-04 13:50:24.000000 elephant-0.8.0/elephant/waveform_features.py
-drwxrwxr-x   0 ulianych  (1001) ulianych  (1001)        0 2020-08-07 12:55:55.513376 elephant-0.8.0/elephant.egg-info/
--rw-rw-r--   0 ulianych  (1001) ulianych  (1001)     2200 2020-08-07 12:55:55.000000 elephant-0.8.0/elephant.egg-info/PKG-INFO
--rw-rw-r--   0 ulianych  (1001) ulianych  (1001)     4484 2020-08-07 12:55:55.000000 elephant-0.8.0/elephant.egg-info/SOURCES.txt
--rw-rw-r--   0 ulianych  (1001) ulianych  (1001)        1 2020-08-07 12:55:55.000000 elephant-0.8.0/elephant.egg-info/dependency_links.txt
--rw-rw-r--   0 ulianych  (1001) ulianych  (1001)      409 2020-08-07 12:55:55.000000 elephant-0.8.0/elephant.egg-info/requires.txt
--rw-rw-r--   0 ulianych  (1001) ulianych  (1001)        9 2020-08-07 12:55:55.000000 elephant-0.8.0/elephant.egg-info/top_level.txt
-drwxrwxr-x   0 ulianych  (1001) ulianych  (1001)        0 2020-08-07 12:55:55.517376 elephant-0.8.0/requirements/
--rw-rw-r--   0 ulianych  (1001) ulianych  (1001)      228 2020-08-05 09:48:24.000000 elephant-0.8.0/requirements/environment.yml
--rw-rw-r--   0 ulianych  (1001) ulianych  (1001)      203 2020-08-04 13:50:24.000000 elephant-0.8.0/requirements/requirements-docs.txt
--rw-rw-r--   0 ulianych  (1001) ulianych  (1001)       69 2020-08-04 13:50:24.000000 elephant-0.8.0/requirements/requirements-extras.txt
--rw-rw-r--   0 ulianych  (1001) ulianych  (1001)       11 2020-08-04 13:50:24.000000 elephant-0.8.0/requirements/requirements-tests.txt
--rw-rw-r--   0 ulianych  (1001) ulianych  (1001)      103 2020-08-07 10:14:09.000000 elephant-0.8.0/requirements/requirements-tutorials.txt
--rw-rw-r--   0 ulianych  (1001) ulianych  (1001)      115 2020-08-04 13:50:24.000000 elephant-0.8.0/requirements/requirements.txt
--rw-rw-r--   0 ulianych  (1001) ulianych  (1001)       38 2020-08-07 12:55:55.517376 elephant-0.8.0/setup.cfg
--rw-rw-r--   0 ulianych  (1001) ulianych  (1001)     2662 2020-08-04 13:50:24.000000 elephant-0.8.0/setup.py
+drwxrwxr-x   0 ulianych  (1001) ulianych  (1001)        0 2020-11-13 11:41:46.414894 elephant-0.9.0/
+-rw-rw-r--   0 ulianych  (1001) ulianych  (1001)      150 2020-11-06 12:59:54.000000 elephant-0.9.0/CITATION.txt
+-rw-rw-r--   0 ulianych  (1001) ulianych  (1001)     1506 2019-07-01 07:26:01.000000 elephant-0.9.0/LICENSE.txt
+-rw-rw-r--   0 ulianych  (1001) ulianych  (1001)      583 2020-11-06 12:59:54.000000 elephant-0.9.0/MANIFEST.in
+-rw-rw-r--   0 ulianych  (1001) ulianych  (1001)     2925 2020-11-13 11:41:46.414894 elephant-0.9.0/PKG-INFO
+-rw-rw-r--   0 ulianych  (1001) ulianych  (1001)     1770 2020-11-13 11:41:27.000000 elephant-0.9.0/README.md
+drwxrwxr-x   0 ulianych  (1001) ulianych  (1001)        0 2020-11-13 11:41:46.346893 elephant-0.9.0/doc/
+-rw-rw-r--   0 ulianych  (1001) ulianych  (1001)     5572 2019-05-15 09:32:00.000000 elephant-0.9.0/doc/Makefile
+drwxrwxr-x   0 ulianych  (1001) ulianych  (1001)        0 2020-11-13 11:41:46.342893 elephant-0.9.0/doc/_templates/
+drwxrwxr-x   0 ulianych  (1001) ulianych  (1001)        0 2020-11-13 11:41:46.346893 elephant-0.9.0/doc/_templates/autosummary/
+-rw-rw-r--   0 ulianych  (1001) ulianych  (1001)      590 2020-11-12 14:48:44.000000 elephant-0.9.0/doc/_templates/autosummary/class.rst
+-rw-rw-r--   0 ulianych  (1001) ulianych  (1001)      351 2020-11-06 12:59:54.000000 elephant-0.9.0/doc/acknowledgments.rst
+-rw-rw-r--   0 ulianych  (1001) ulianych  (1001)     2541 2020-11-12 11:11:44.000000 elephant-0.9.0/doc/authors.rst
+drwxrwxr-x   0 ulianych  (1001) ulianych  (1001)        0 2020-11-13 11:41:46.346893 elephant-0.9.0/doc/bib/
+-rw-rw-r--   0 ulianych  (1001) ulianych  (1001)     4032 2020-11-12 11:11:44.000000 elephant-0.9.0/doc/bib/elephant.bib
+-rw-rw-r--   0 ulianych  (1001) ulianych  (1001)     1197 2020-11-06 12:59:54.000000 elephant-0.9.0/doc/citation.rst
+-rw-rw-r--   0 ulianych  (1001) ulianych  (1001)    11529 2020-11-13 11:41:27.000000 elephant-0.9.0/doc/conf.py
+-rw-rw-r--   0 ulianych  (1001) ulianych  (1001)     2966 2020-11-12 14:48:44.000000 elephant-0.9.0/doc/developers_guide.rst
+-rw-rw-r--   0 ulianych  (1001) ulianych  (1001)     1248 2020-11-06 12:59:54.000000 elephant-0.9.0/doc/documentation_guide.rst
+-rw-rw-r--   0 ulianych  (1001) ulianych  (1001)     1075 2020-11-06 12:59:54.000000 elephant-0.9.0/doc/get_in_touch.rst
+drwxrwxr-x   0 ulianych  (1001) ulianych  (1001)        0 2020-11-13 11:41:46.346893 elephant-0.9.0/doc/images/
+-rw-rw-r--   0 ulianych  (1001) ulianych  (1001)     2238 2019-05-15 09:32:00.000000 elephant-0.9.0/doc/images/elephant_favicon.ico
+-rw-rw-r--   0 ulianych  (1001) ulianych  (1001)   116686 2019-05-15 09:32:00.000000 elephant-0.9.0/doc/images/elephant_logo.png
+-rw-rw-r--   0 ulianych  (1001) ulianych  (1001)    12239 2019-05-15 09:32:00.000000 elephant-0.9.0/doc/images/elephant_logo_sidebar.png
+-rw-rw-r--   0 ulianych  (1001) ulianych  (1001)     2195 2020-11-13 11:41:27.000000 elephant-0.9.0/doc/index.rst
+-rw-rw-r--   0 ulianych  (1001) ulianych  (1001)     3780 2020-11-12 14:48:44.000000 elephant-0.9.0/doc/install.rst
+-rw-rw-r--   0 ulianych  (1001) ulianych  (1001)     4780 2020-11-13 11:41:27.000000 elephant-0.9.0/doc/maintainers_guide.rst
+-rw-rw-r--   0 ulianych  (1001) ulianych  (1001)     5100 2019-05-15 09:32:00.000000 elephant-0.9.0/doc/make.bat
+-rw-rw-r--   0 ulianych  (1001) ulianych  (1001)      772 2020-11-12 11:11:44.000000 elephant-0.9.0/doc/modules.rst
+drwxrwxr-x   0 ulianych  (1001) ulianych  (1001)        0 2020-11-13 11:41:46.350893 elephant-0.9.0/doc/reference/
+-rw-rw-r--   0 ulianych  (1001) ulianych  (1001)      182 2020-11-12 11:11:44.000000 elephant-0.9.0/doc/reference/_spike_train_processing.rst
+-rw-rw-r--   0 ulianych  (1001) ulianych  (1001)      310 2020-11-06 12:59:54.000000 elephant-0.9.0/doc/reference/asset.rst
+-rw-rw-r--   0 ulianych  (1001) ulianych  (1001)      101 2020-11-06 12:59:54.000000 elephant-0.9.0/doc/reference/causality.rst
+-rw-rw-r--   0 ulianych  (1001) ulianych  (1001)      159 2020-11-06 12:59:54.000000 elephant-0.9.0/doc/reference/cell_assembly_detection.rst
+-rw-rw-r--   0 ulianych  (1001) ulianych  (1001)      176 2020-11-06 12:59:54.000000 elephant-0.9.0/doc/reference/change_point_detection.rst
+-rw-rw-r--   0 ulianych  (1001) ulianych  (1001)      127 2020-11-13 11:41:27.000000 elephant-0.9.0/doc/reference/conversion.rst
+-rw-rw-r--   0 ulianych  (1001) ulianych  (1001)      228 2020-11-06 12:59:54.000000 elephant-0.9.0/doc/reference/cubic.rst
+-rw-rw-r--   0 ulianych  (1001) ulianych  (1001)      158 2020-11-06 12:59:54.000000 elephant-0.9.0/doc/reference/current_source_density.rst
+-rw-rw-r--   0 ulianych  (1001) ulianych  (1001)      156 2020-11-13 11:41:27.000000 elephant-0.9.0/doc/reference/gpfa.rst
+-rw-rw-r--   0 ulianych  (1001) ulianych  (1001)       58 2020-11-06 12:59:54.000000 elephant-0.9.0/doc/reference/kernels.rst
+-rw-rw-r--   0 ulianych  (1001) ulianych  (1001)      115 2020-11-06 12:59:54.000000 elephant-0.9.0/doc/reference/neo_tools.rst
+-rw-rw-r--   0 ulianych  (1001) ulianych  (1001)      140 2020-11-06 12:59:54.000000 elephant-0.9.0/doc/reference/pandas_bridge.rst
+-rw-rw-r--   0 ulianych  (1001) ulianych  (1001)       62 2020-11-06 12:59:54.000000 elephant-0.9.0/doc/reference/parallel.rst
+-rw-rw-r--   0 ulianych  (1001) ulianych  (1001)      132 2020-11-06 12:59:54.000000 elephant-0.9.0/doc/reference/phase_analysis.rst
+-rw-rw-r--   0 ulianych  (1001) ulianych  (1001)      249 2020-11-06 12:59:54.000000 elephant-0.9.0/doc/reference/signal_processing.rst
+-rw-rw-r--   0 ulianych  (1001) ulianych  (1001)      173 2020-11-13 11:41:27.000000 elephant-0.9.0/doc/reference/spade.rst
+-rw-rw-r--   0 ulianych  (1001) ulianych  (1001)      102 2020-11-06 12:59:54.000000 elephant-0.9.0/doc/reference/spectral.rst
+-rw-rw-r--   0 ulianych  (1001) ulianych  (1001)      233 2020-11-13 11:41:27.000000 elephant-0.9.0/doc/reference/spike_train_correlation.rst
+-rw-rw-r--   0 ulianych  (1001) ulianych  (1001)      131 2020-11-13 11:41:27.000000 elephant-0.9.0/doc/reference/spike_train_dissimilarity.rst
+-rw-rw-r--   0 ulianych  (1001) ulianych  (1001)      284 2020-11-06 12:59:54.000000 elephant-0.9.0/doc/reference/spike_train_generation.rst
+-rw-rw-r--   0 ulianych  (1001) ulianych  (1001)      278 2020-11-06 12:59:54.000000 elephant-0.9.0/doc/reference/spike_train_surrogates.rst
+-rw-rw-r--   0 ulianych  (1001) ulianych  (1001)      241 2020-11-12 11:11:44.000000 elephant-0.9.0/doc/reference/spike_train_synchrony.rst
+-rw-rw-r--   0 ulianych  (1001) ulianych  (1001)      115 2020-11-06 12:59:54.000000 elephant-0.9.0/doc/reference/sta.rst
+-rw-rw-r--   0 ulianych  (1001) ulianych  (1001)      118 2020-11-06 12:59:54.000000 elephant-0.9.0/doc/reference/statistics.rst
+drwxrwxr-x   0 ulianych  (1001) ulianych  (1001)        0 2020-11-13 11:41:46.346893 elephant-0.9.0/doc/reference/toctree/
+drwxrwxr-x   0 ulianych  (1001) ulianych  (1001)        0 2020-11-13 11:41:46.350893 elephant-0.9.0/doc/reference/toctree/kernels/
+-rw-rw-r--   0 ulianych  (1001) ulianych  (1001)      546 2020-11-13 09:26:11.000000 elephant-0.9.0/doc/reference/toctree/kernels/elephant.kernels.AlphaKernel.rst
+-rw-rw-r--   0 ulianych  (1001) ulianych  (1001)      656 2020-11-13 09:26:11.000000 elephant-0.9.0/doc/reference/toctree/kernels/elephant.kernels.EpanechnikovLikeKernel.rst
+-rw-rw-r--   0 ulianych  (1001) ulianych  (1001)      606 2020-11-13 09:26:11.000000 elephant-0.9.0/doc/reference/toctree/kernels/elephant.kernels.ExponentialKernel.rst
+-rw-rw-r--   0 ulianych  (1001) ulianych  (1001)      576 2020-11-13 09:26:11.000000 elephant-0.9.0/doc/reference/toctree/kernels/elephant.kernels.GaussianKernel.rst
+-rw-rw-r--   0 ulianych  (1001) ulianych  (1001)      586 2020-11-13 09:26:11.000000 elephant-0.9.0/doc/reference/toctree/kernels/elephant.kernels.LaplacianKernel.rst
+-rw-rw-r--   0 ulianych  (1001) ulianych  (1001)      606 2020-11-13 09:26:11.000000 elephant-0.9.0/doc/reference/toctree/kernels/elephant.kernels.RectangularKernel.rst
+-rw-rw-r--   0 ulianych  (1001) ulianych  (1001)      596 2020-11-13 09:26:11.000000 elephant-0.9.0/doc/reference/toctree/kernels/elephant.kernels.TriangularKernel.rst
+-rw-rw-r--   0 ulianych  (1001) ulianych  (1001)      421 2020-11-06 12:59:54.000000 elephant-0.9.0/doc/reference/unitary_event_analysis.rst
+-rw-rw-r--   0 ulianych  (1001) ulianych  (1001)      111 2020-11-06 12:59:54.000000 elephant-0.9.0/doc/reference/waveform_features.rst
+-rw-rw-r--   0 ulianych  (1001) ulianych  (1001)    22657 2020-11-13 11:41:27.000000 elephant-0.9.0/doc/release_notes.rst
+-rw-rw-r--   0 ulianych  (1001) ulianych  (1001)    29332 2020-11-06 12:59:54.000000 elephant-0.9.0/doc/style_guide.rst
+drwxrwxr-x   0 ulianych  (1001) ulianych  (1001)        0 2020-11-13 11:41:46.398893 elephant-0.9.0/doc/tutorials/
+-rw-rw-r--   0 ulianych  (1001) ulianych  (1001)   334296 2020-11-06 12:59:54.000000 elephant-0.9.0/doc/tutorials/asset.ipynb
+-rw-rw-r--   0 ulianych  (1001) ulianych  (1001) 44142233 2020-11-02 11:16:41.000000 elephant-0.9.0/doc/tutorials/asset_showcase_500.nix
+-rw-rw-r--   0 ulianych  (1001) ulianych  (1001)  1578043 2020-11-06 12:59:54.000000 elephant-0.9.0/doc/tutorials/gpfa.ipynb
+-rw-rw-r--   0 ulianych  (1001) ulianych  (1001)    13125 2020-11-06 12:59:54.000000 elephant-0.9.0/doc/tutorials/parallel.ipynb
+-rw-rw-r--   0 ulianych  (1001) ulianych  (1001)    19838 2020-11-06 12:59:54.000000 elephant-0.9.0/doc/tutorials/statistics.ipynb
+-rw-rw-r--   0 ulianych  (1001) ulianych  (1001)    15368 2020-11-06 12:59:54.000000 elephant-0.9.0/doc/tutorials/unitary_event_analysis.ipynb
+-rw-rw-r--   0 ulianych  (1001) ulianych  (1001)     2256 2020-11-06 12:59:54.000000 elephant-0.9.0/doc/tutorials.rst
+drwxrwxr-x   0 ulianych  (1001) ulianych  (1001)        0 2020-11-13 11:41:46.402894 elephant-0.9.0/elephant/
+-rw-rw-r--   0 ulianych  (1001) ulianych  (1001)        5 2020-11-13 11:41:27.000000 elephant-0.9.0/elephant/VERSION
+-rw-rw-r--   0 ulianych  (1001) ulianych  (1001)     1394 2020-11-06 12:59:54.000000 elephant-0.9.0/elephant/__init__.py
+-rw-rw-r--   0 ulianych  (1001) ulianych  (1001)    72742 2020-11-12 14:48:44.000000 elephant-0.9.0/elephant/asset.py
+drwxrwxr-x   0 ulianych  (1001) ulianych  (1001)        0 2020-11-13 11:41:46.402894 elephant-0.9.0/elephant/causality/
+-rw-rw-r--   0 ulianych  (1001) ulianych  (1001)        0 2020-11-06 12:59:54.000000 elephant-0.9.0/elephant/causality/__init__.py
+-rw-rw-r--   0 ulianych  (1001) ulianych  (1001)    19241 2020-11-13 09:05:32.000000 elephant-0.9.0/elephant/causality/granger.py
+-rw-rw-r--   0 ulianych  (1001) ulianych  (1001)    49247 2020-11-12 14:48:44.000000 elephant-0.9.0/elephant/cell_assembly_detection.py
+-rw-rw-r--   0 ulianych  (1001) ulianych  (1001)    18575 2020-11-06 12:59:54.000000 elephant-0.9.0/elephant/change_point_detection.py
+-rw-rw-r--   0 ulianych  (1001) ulianych  (1001)    33551 2020-11-13 11:41:27.000000 elephant-0.9.0/elephant/conversion.py
+-rw-rw-r--   0 ulianych  (1001) ulianych  (1001)     6977 2020-11-06 12:59:54.000000 elephant-0.9.0/elephant/cubic.py
+-rw-rw-r--   0 ulianych  (1001) ulianych  (1001)    13697 2020-11-13 09:05:32.000000 elephant-0.9.0/elephant/current_source_density.py
+drwxrwxr-x   0 ulianych  (1001) ulianych  (1001)        0 2020-11-13 11:41:46.406894 elephant-0.9.0/elephant/current_source_density_src/
+-rw-rw-r--   0 ulianych  (1001) ulianych  (1001)    42718 2020-11-06 12:59:54.000000 elephant-0.9.0/elephant/current_source_density_src/KCSD.py
+-rw-rw-r--   0 ulianych  (1001) ulianych  (1001)     4060 2019-05-15 09:32:00.000000 elephant-0.9.0/elephant/current_source_density_src/README.md
+-rw-rw-r--   0 ulianych  (1001) ulianych  (1001)       62 2020-02-19 12:59:34.000000 elephant-0.9.0/elephant/current_source_density_src/__init__.py
+-rw-rw-r--   0 ulianych  (1001) ulianych  (1001)     4939 2020-02-19 12:59:34.000000 elephant-0.9.0/elephant/current_source_density_src/basis_functions.py
+-rw-rw-r--   0 ulianych  (1001) ulianych  (1001)    35175 2020-02-19 12:59:34.000000 elephant-0.9.0/elephant/current_source_density_src/icsd.py
+-rw-rw-r--   0 ulianych  (1001) ulianych  (1001)    65926 2019-05-15 09:32:00.000000 elephant-0.9.0/elephant/current_source_density_src/test_data.mat
+-rw-rw-r--   0 ulianych  (1001) ulianych  (1001)    11986 2020-11-06 12:59:54.000000 elephant-0.9.0/elephant/current_source_density_src/utility_functions.py
+drwxrwxr-x   0 ulianych  (1001) ulianych  (1001)        0 2020-11-13 11:41:46.406894 elephant-0.9.0/elephant/gpfa/
+-rw-rw-r--   0 ulianych  (1001) ulianych  (1001)      153 2020-11-06 12:59:54.000000 elephant-0.9.0/elephant/gpfa/__init__.py
+-rw-rw-r--   0 ulianych  (1001) ulianych  (1001)    19498 2020-11-13 11:41:27.000000 elephant-0.9.0/elephant/gpfa/gpfa.py
+-rw-rw-r--   0 ulianych  (1001) ulianych  (1001)    20892 2020-11-13 09:05:32.000000 elephant-0.9.0/elephant/gpfa/gpfa_core.py
+-rw-rw-r--   0 ulianych  (1001) ulianych  (1001)    17915 2020-11-13 09:05:32.000000 elephant-0.9.0/elephant/gpfa/gpfa_util.py
+-rw-rw-r--   0 ulianych  (1001) ulianych  (1001)    27594 2020-11-12 14:48:44.000000 elephant-0.9.0/elephant/kernels.py
+-rw-rw-r--   0 ulianych  (1001) ulianych  (1001)     7271 2020-11-06 12:59:54.000000 elephant-0.9.0/elephant/neo_tools.py
+-rw-rw-r--   0 ulianych  (1001) ulianych  (1001)    21991 2020-11-06 12:59:54.000000 elephant-0.9.0/elephant/pandas_bridge.py
+drwxrwxr-x   0 ulianych  (1001) ulianych  (1001)        0 2020-11-13 11:41:46.406894 elephant-0.9.0/elephant/parallel/
+-rw-rw-r--   0 ulianych  (1001) ulianych  (1001)     1342 2020-11-06 12:59:54.000000 elephant-0.9.0/elephant/parallel/__init__.py
+-rw-rw-r--   0 ulianych  (1001) ulianych  (1001)     2050 2020-11-06 12:59:54.000000 elephant-0.9.0/elephant/parallel/mpi.py
+-rw-rw-r--   0 ulianych  (1001) ulianych  (1001)     3668 2020-11-06 12:59:54.000000 elephant-0.9.0/elephant/parallel/parallel.py
+-rw-rw-r--   0 ulianych  (1001) ulianych  (1001)     7111 2020-11-13 09:05:32.000000 elephant-0.9.0/elephant/phase_analysis.py
+-rw-rw-r--   0 ulianych  (1001) ulianych  (1001)    36918 2020-11-12 14:48:44.000000 elephant-0.9.0/elephant/signal_processing.py
+-rw-rw-r--   0 ulianych  (1001) ulianych  (1001)    94492 2020-11-13 11:41:27.000000 elephant-0.9.0/elephant/spade.py
+drwxrwxr-x   0 ulianych  (1001) ulianych  (1001)        0 2020-11-13 11:41:46.406894 elephant-0.9.0/elephant/spade_src/
+-rw-rw-r--   0 ulianych  (1001) ulianych  (1001)     1311 2019-05-15 09:32:00.000000 elephant-0.9.0/elephant/spade_src/LICENSE
+-rw-rw-r--   0 ulianych  (1001) ulianych  (1001)        0 2020-02-19 12:59:34.000000 elephant-0.9.0/elephant/spade_src/__init__.py
+-rw-rw-r--   0 ulianych  (1001) ulianych  (1001)    11273 2020-11-06 12:59:54.000000 elephant-0.9.0/elephant/spade_src/fast_fca.py
+-rw-rw-r--   0 ulianych  (1001) ulianych  (1001)    19207 2020-11-06 12:59:54.000000 elephant-0.9.0/elephant/spectral.py
+-rw-rw-r--   0 ulianych  (1001) ulianych  (1001)    41787 2020-11-13 11:41:27.000000 elephant-0.9.0/elephant/spike_train_correlation.py
+-rw-rw-r--   0 ulianych  (1001) ulianych  (1001)    18976 2020-11-13 11:41:27.000000 elephant-0.9.0/elephant/spike_train_dissimilarity.py
+-rw-rw-r--   0 ulianych  (1001) ulianych  (1001)    53599 2020-11-06 12:59:54.000000 elephant-0.9.0/elephant/spike_train_generation.py
+-rw-rw-r--   0 ulianych  (1001) ulianych  (1001)    55993 2020-11-12 14:48:44.000000 elephant-0.9.0/elephant/spike_train_surrogates.py
+-rw-rw-r--   0 ulianych  (1001) ulianych  (1001)     7673 2020-11-13 11:41:27.000000 elephant-0.9.0/elephant/spike_train_synchrony.py
+-rw-rw-r--   0 ulianych  (1001) ulianych  (1001)    13435 2020-11-06 12:59:54.000000 elephant-0.9.0/elephant/sta.py
+-rw-rw-r--   0 ulianych  (1001) ulianych  (1001)    44688 2020-11-13 11:41:27.000000 elephant-0.9.0/elephant/statistics.py
+drwxrwxr-x   0 ulianych  (1001) ulianych  (1001)        0 2020-11-13 11:41:46.414894 elephant-0.9.0/elephant/test/
+-rw-rw-r--   0 ulianych  (1001) ulianych  (1001)        0 2020-02-19 12:59:34.000000 elephant-0.9.0/elephant/test/__init__.py
+-rw-rw-r--   0 ulianych  (1001) ulianych  (1001)     2384 2020-11-12 11:11:44.000000 elephant-0.9.0/elephant/test/download.py
+-rw-rw-r--   0 ulianych  (1001) ulianych  (1001)     1682 2020-11-06 12:59:54.000000 elephant-0.9.0/elephant/test/make_spike_extraction_test_data.py
+-rw-rw-r--   0 ulianych  (1001) ulianych  (1001)    62953 2019-07-01 07:26:01.000000 elephant-0.9.0/elephant/test/spike_extraction_test_data.txt
+-rw-rw-r--   0 ulianych  (1001) ulianych  (1001)    22307 2020-11-06 12:59:54.000000 elephant-0.9.0/elephant/test/test_asset.py
+-rw-rw-r--   0 ulianych  (1001) ulianych  (1001)    11321 2020-11-13 09:05:32.000000 elephant-0.9.0/elephant/test/test_causality.py
+-rw-rw-r--   0 ulianych  (1001) ulianych  (1001)     9254 2020-11-06 12:59:54.000000 elephant-0.9.0/elephant/test/test_cell_assembly_detection.py
+-rw-rw-r--   0 ulianych  (1001) ulianych  (1001)     9271 2020-11-06 12:59:54.000000 elephant-0.9.0/elephant/test/test_change_point_detection.py
+-rw-rw-r--   0 ulianych  (1001) ulianych  (1001)    26550 2020-11-12 14:48:44.000000 elephant-0.9.0/elephant/test/test_conversion.py
+-rw-rw-r--   0 ulianych  (1001) ulianych  (1001)     6715 2020-11-05 16:50:56.000000 elephant-0.9.0/elephant/test/test_csd.py
+-rw-rw-r--   0 ulianych  (1001) ulianych  (1001)     5494 2020-11-06 12:59:54.000000 elephant-0.9.0/elephant/test/test_cubic.py
+-rw-rw-r--   0 ulianych  (1001) ulianych  (1001)     9587 2020-11-13 09:05:32.000000 elephant-0.9.0/elephant/test/test_gpfa.py
+-rw-rw-r--   0 ulianych  (1001) ulianych  (1001)    40516 2020-11-06 12:59:54.000000 elephant-0.9.0/elephant/test/test_icsd.py
+-rw-rw-r--   0 ulianych  (1001) ulianych  (1001)     8373 2020-11-06 12:59:54.000000 elephant-0.9.0/elephant/test/test_kcsd.py
+-rw-rw-r--   0 ulianych  (1001) ulianych  (1001)    16415 2020-11-06 12:59:54.000000 elephant-0.9.0/elephant/test/test_kernels.py
+-rw-rw-r--   0 ulianych  (1001) ulianych  (1001)    53093 2020-11-13 11:41:27.000000 elephant-0.9.0/elephant/test/test_neo_tools.py
+-rw-rw-r--   0 ulianych  (1001) ulianych  (1001)   113866 2020-11-06 12:59:54.000000 elephant-0.9.0/elephant/test/test_pandas_bridge.py
+-rw-rw-r--   0 ulianych  (1001) ulianych  (1001)     1587 2020-11-06 12:59:54.000000 elephant-0.9.0/elephant/test/test_parallel.py
+-rw-rw-r--   0 ulianych  (1001) ulianych  (1001)     8620 2020-11-06 12:59:54.000000 elephant-0.9.0/elephant/test/test_phase_analysis.py
+-rw-rw-r--   0 ulianych  (1001) ulianych  (1001)    52337 2020-11-12 14:48:44.000000 elephant-0.9.0/elephant/test/test_signal_processing.py
+-rw-rw-r--   0 ulianych  (1001) ulianych  (1001)    32565 2020-11-06 12:59:54.000000 elephant-0.9.0/elephant/test/test_spade.py
+-rw-rw-r--   0 ulianych  (1001) ulianych  (1001)    16044 2020-11-06 12:59:54.000000 elephant-0.9.0/elephant/test/test_spectral.py
+-rw-rw-r--   0 ulianych  (1001) ulianych  (1001)    35941 2020-11-12 14:48:44.000000 elephant-0.9.0/elephant/test/test_spike_train_correlation.py
+-rw-rw-r--   0 ulianych  (1001) ulianych  (1001)    27288 2020-11-06 12:59:54.000000 elephant-0.9.0/elephant/test/test_spike_train_dissimilarity.py
+-rw-rw-r--   0 ulianych  (1001) ulianych  (1001)    42897 2020-11-12 14:48:44.000000 elephant-0.9.0/elephant/test/test_spike_train_generation.py
+-rw-rw-r--   0 ulianych  (1001) ulianych  (1001)    29287 2020-11-12 14:48:44.000000 elephant-0.9.0/elephant/test/test_spike_train_surrogates.py
+-rw-rw-r--   0 ulianych  (1001) ulianych  (1001)     9668 2020-11-13 08:44:23.000000 elephant-0.9.0/elephant/test/test_spike_train_synchrony.py
+-rw-rw-r--   0 ulianych  (1001) ulianych  (1001)    19061 2020-11-06 12:59:54.000000 elephant-0.9.0/elephant/test/test_sta.py
+-rw-rw-r--   0 ulianych  (1001) ulianych  (1001)    42632 2020-11-13 08:44:23.000000 elephant-0.9.0/elephant/test/test_statistics.py
+-rw-rw-r--   0 ulianych  (1001) ulianych  (1001)    20948 2020-11-06 12:59:54.000000 elephant-0.9.0/elephant/test/test_unitary_event_analysis.py
+-rw-rw-r--   0 ulianych  (1001) ulianych  (1001)     3577 2020-11-12 14:48:44.000000 elephant-0.9.0/elephant/test/test_waveform_features.py
+-rw-rw-r--   0 ulianych  (1001) ulianych  (1001)    28150 2020-11-12 14:48:44.000000 elephant-0.9.0/elephant/unitary_event_analysis.py
+-rw-rw-r--   0 ulianych  (1001) ulianych  (1001)     6932 2020-11-13 09:05:32.000000 elephant-0.9.0/elephant/utils.py
+-rw-rw-r--   0 ulianych  (1001) ulianych  (1001)     4105 2020-11-12 14:48:44.000000 elephant-0.9.0/elephant/waveform_features.py
+drwxrwxr-x   0 ulianych  (1001) ulianych  (1001)        0 2020-11-13 11:41:46.402894 elephant-0.9.0/elephant.egg-info/
+-rw-rw-r--   0 ulianych  (1001) ulianych  (1001)     2925 2020-11-13 11:41:46.000000 elephant-0.9.0/elephant.egg-info/PKG-INFO
+-rw-rw-r--   0 ulianych  (1001) ulianych  (1001)     4858 2020-11-13 11:41:46.000000 elephant-0.9.0/elephant.egg-info/SOURCES.txt
+-rw-rw-r--   0 ulianych  (1001) ulianych  (1001)        1 2020-11-13 11:41:46.000000 elephant-0.9.0/elephant.egg-info/dependency_links.txt
+-rw-rw-r--   0 ulianych  (1001) ulianych  (1001)      432 2020-11-13 11:41:46.000000 elephant-0.9.0/elephant.egg-info/requires.txt
+-rw-rw-r--   0 ulianych  (1001) ulianych  (1001)        9 2020-11-13 11:41:46.000000 elephant-0.9.0/elephant.egg-info/top_level.txt
+drwxrwxr-x   0 ulianych  (1001) ulianych  (1001)        0 2020-11-13 11:41:46.414894 elephant-0.9.0/requirements/
+-rw-rw-r--   0 ulianych  (1001) ulianych  (1001)      226 2020-11-12 14:48:44.000000 elephant-0.9.0/requirements/environment.yml
+-rw-rw-r--   0 ulianych  (1001) ulianych  (1001)      204 2020-11-13 11:41:27.000000 elephant-0.9.0/requirements/requirements-docs.txt
+-rw-rw-r--   0 ulianych  (1001) ulianych  (1001)       56 2020-11-13 11:41:27.000000 elephant-0.9.0/requirements/requirements-extras.txt
+-rw-rw-r--   0 ulianych  (1001) ulianych  (1001)       46 2020-11-12 14:48:44.000000 elephant-0.9.0/requirements/requirements-tests.txt
+-rw-rw-r--   0 ulianych  (1001) ulianych  (1001)      103 2020-11-13 11:41:27.000000 elephant-0.9.0/requirements/requirements-tutorials.txt
+-rw-rw-r--   0 ulianych  (1001) ulianych  (1001)      107 2020-11-13 11:41:27.000000 elephant-0.9.0/requirements/requirements.txt
+-rw-rw-r--   0 ulianych  (1001) ulianych  (1001)       38 2020-11-13 11:41:46.414894 elephant-0.9.0/setup.cfg
+-rw-rw-r--   0 ulianych  (1001) ulianych  (1001)     2662 2020-11-06 12:59:54.000000 elephant-0.9.0/setup.py
```

### Comparing `elephant-0.8.0/LICENSE.txt` & `elephant-0.9.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `elephant-0.8.0/MANIFEST.in` & `elephant-0.9.0/MANIFEST.in`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 recursive-include elephant *.py
 include requirements/*
 include README.md
 include LICENSE.txt
+include CITATION.txt
 include elephant/VERSION
 include elephant/current_source_density_src/README.md
 include elephant/current_source_density_src/test_data.mat
 include elephant/spade_src/LICENSE
 recursive-include elephant/spade_src *.so *.pyd
 include elephant/test/spike_extraction_test_data.txt
 recursive-include doc *
```

### Comparing `elephant-0.8.0/PKG-INFO` & `elephant-0.9.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,46 +1,62 @@
 Metadata-Version: 2.1
 Name: elephant
-Version: 0.8.0
+Version: 0.9.0
 Summary: Elephant is a package for analysis of electrophysiology data in Python
 Home-page: http://neuralensemble.org/elephant
 Author: Elephant authors and contributors
 Author-email: andrew.davison@unic.cnrs-gif.fr
 License: BSD
 Description: # Elephant - Electrophysiology Analysis Toolkit
         
-        ![](https://travis-ci.org/NeuralEnsemble/elephant.png?branch=master "Unit Test Status")
-        ![](https://coveralls.io/repos/NeuralEnsemble/elephant/badge.png "Unit Test Coverage")
-        ![](https://readthedocs.org/projects/elephant/badge/?version=latest "Documentation Status")
-        ![](https://img.shields.io/pypi/v/elephant)
-        ![](https://img.shields.io/pypi/dm/elephant)
+        [![Build Status](https://travis-ci.org/NeuralEnsemble/elephant.svg?branch=master)](https://travis-ci.org/NeuralEnsemble/elephant)
+        [![Coverage Status](https://coveralls.io/repos/github/NeuralEnsemble/elephant/badge.svg?branch=master)](https://coveralls.io/github/NeuralEnsemble/elephant?branch=master)
+        [![Documentation Status](https://readthedocs.org/projects/elephant/badge/?version=latest)](https://elephant.readthedocs.io/en/latest/?badge=latest)
+        [![![PyPi]](https://img.shields.io/pypi/v/elephant)](https://pypi.org/project/elephant/)
+        [![Statistics](https://img.shields.io/pypi/dm/elephant)](https://seladb.github.io/StarTrack-js/#/preload?r=neuralensemble,elephant)
         [![Gitter](https://badges.gitter.im/python-elephant/community.svg)](https://gitter.im/python-elephant/community?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge)
         
         *Elephant* package analyses all sorts of neurophysiological data:
         spike trains, LFP, analog signals. The input-output data format is either
         [Neo](https://github.com/NeuralEnsemble/python-neo), Quantity or Numpy array.
         
+        
         ### More Information
         
         * Documentation: https://elephant.readthedocs.io/en/latest/
         * Mailing list: https://groups.google.com/group/neuralensemble
         
         
+        #### Visualization of Elephant analysis objects
+        
+        Viziphant package (https://github.com/INM-6/viziphant) is developed by Elephant
+        team for plotting and visualization of the output of Elephant functions in a
+        few lines of code.
+        
+        
         #### License
          
         Modified BSD License, see [LICENSE.txt](LICENSE.txt) for details.
         
+        
         #### Copyright
         
         :copyright: 2014-2020 by the [Elephant team](doc/authors.rst).
         
+        
         #### Acknowledgments
         
         See [acknowledgments](doc/acknowledgments.rst).
         
+        
+        #### Citation
+        
+        See [citations](doc/citation.rst).
+        
+        
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 2
```

### Comparing `elephant-0.8.0/README.md` & `elephant-0.9.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,30 +1,46 @@
 # Elephant - Electrophysiology Analysis Toolkit
 
-![](https://travis-ci.org/NeuralEnsemble/elephant.png?branch=master "Unit Test Status")
-![](https://coveralls.io/repos/NeuralEnsemble/elephant/badge.png "Unit Test Coverage")
-![](https://readthedocs.org/projects/elephant/badge/?version=latest "Documentation Status")
-![](https://img.shields.io/pypi/v/elephant)
-![](https://img.shields.io/pypi/dm/elephant)
+[![Build Status](https://travis-ci.org/NeuralEnsemble/elephant.svg?branch=master)](https://travis-ci.org/NeuralEnsemble/elephant)
+[![Coverage Status](https://coveralls.io/repos/github/NeuralEnsemble/elephant/badge.svg?branch=master)](https://coveralls.io/github/NeuralEnsemble/elephant?branch=master)
+[![Documentation Status](https://readthedocs.org/projects/elephant/badge/?version=latest)](https://elephant.readthedocs.io/en/latest/?badge=latest)
+[![![PyPi]](https://img.shields.io/pypi/v/elephant)](https://pypi.org/project/elephant/)
+[![Statistics](https://img.shields.io/pypi/dm/elephant)](https://seladb.github.io/StarTrack-js/#/preload?r=neuralensemble,elephant)
 [![Gitter](https://badges.gitter.im/python-elephant/community.svg)](https://gitter.im/python-elephant/community?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge)
 
 *Elephant* package analyses all sorts of neurophysiological data:
 spike trains, LFP, analog signals. The input-output data format is either
 [Neo](https://github.com/NeuralEnsemble/python-neo), Quantity or Numpy array.
 
+
 ### More Information
 
 * Documentation: https://elephant.readthedocs.io/en/latest/
 * Mailing list: https://groups.google.com/group/neuralensemble
 
 
+#### Visualization of Elephant analysis objects
+
+Viziphant package (https://github.com/INM-6/viziphant) is developed by Elephant
+team for plotting and visualization of the output of Elephant functions in a
+few lines of code.
+
+
 #### License
  
 Modified BSD License, see [LICENSE.txt](LICENSE.txt) for details.
 
+
 #### Copyright
 
 :copyright: 2014-2020 by the [Elephant team](doc/authors.rst).
 
+
 #### Acknowledgments
 
 See [acknowledgments](doc/acknowledgments.rst).
+
+
+#### Citation
+
+See [citations](doc/citation.rst).
+
```

### Comparing `elephant-0.8.0/doc/Makefile` & `elephant-0.9.0/doc/Makefile`

 * *Files identical despite different names*

### Comparing `elephant-0.8.0/doc/authors.rst` & `elephant-0.9.0/doc/authors.rst`

 * *Files 8% similar despite different names*

```diff
@@ -43,21 +43,26 @@
 * Alexander van Meegen [1]
 * Aitor Morales-Gregorio [1]
 * Cristiano Köhler [1]
 * Paulina Dąbrowska [1]
 * Jan Lewen [1]
 * Alexander Kleinjohann [1]
 * Danylo Ulianych [1]
+* Anno Kurth [1]
+* Regimantas Jurkus [1]
+* Philipp Steigerwald [12]
+* Manuel Ciba [12]
 
 1. Institute of Neuroscience and Medicine (INM-6), Computational and Systems Neuroscience & Institute for Advanced Simulation (IAS-6), Theoretical Neuroscience, Jülich Research Centre and JARA, Jülich, Germany
 2. Unité de Neurosciences, Information et Complexité, CNRS UPR 3293, Gif-sur-Yvette, France
 3. Electronic Visions Group, Kirchhoff-Institute for Physics, University of Heidelberg, Germany
 4. Brain-Mind Institute, Ecole Polytechnique Fédérale de Lausanne, Switzerland
 5. NIH–NICHD, Laboratory of Cellular and Synaptic Physiology, Bethesda, Maryland 20892, USA
 6. Neural Information Processing Group, Institute of Software Engineering and Theoretical Computer Science, Technische Universität Berlin, Germany
 7. Arizona State University School of Life Sciences, USA
 8. Computational Neuroscience Research Group (CNRG), Waterloo Centre for Theoretical Neuroscience, Waterloo, Canada
 9. Nencki Institute of Experimental Biology, Warsaw, Poland
 10. Instituto de Neurobiología, Universidad Nacional Autónoma de México, Mexico City, Mexico
 11. Case Western Reserve University (CWRU), Cleveland, OH, USA
+12. BioMEMS Lab, TH Aschaffenburg University of applied sciences, Germany
 
 If we've somehow missed you off the list we're very sorry - please let us know.
```

### Comparing `elephant-0.8.0/doc/conf.py` & `elephant-0.9.0/doc/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -338,16 +338,18 @@
 # The depth of the table of contents in toc.ncx.
 #epub_tocdepth = 3
 
 # Allow duplicate toc entries.
 #epub_tocdup = True
 
 
-# Example configuration for intersphinx: refer to the Python standard library.
-intersphinx_mapping = {'http://docs.python.org/': None}
+# configuration for intersphinx: refer to Viziphant
+intersphinx_mapping = {
+    'viziphant': ('https://viziphant.readthedocs.io/en/latest/', None)
+}
 
 # Use more reliable mathjax source
 mathjax_path = 'https://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS-MML_HTMLorMML'
 
 # Remove the copyright notice from docstrings:
```

### Comparing `elephant-0.8.0/doc/developers_guide.rst` & `elephant-0.9.0/doc/developers_guide.rst`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,24 @@
 .. _developers_guide:
 
 =================
 Developers' Guide
 =================
 
-.. note:: The documentation guide (how to write a good documentation, naming
-          conventions, docstring examples) is in :ref:`documentation_guide`.
+.. note::
+    1. The documentation guide (how to write a good documentation, naming
+       conventions, docstring examples) is in the :ref:`documentation_guide`.
+
+    2. We highly recommend to get in touch with us (see :ref:`get_in_touch`) *before* starting
+       to implement a new feature in Elephant. This way, we can point out synergies with
+       complementary efforts and help in designing your implementation such that its integration
+       into Elephant will be an easy process.
+
+    3. If you experience any problems during one of the steps below, please
+       contact us and we'll help you.
 
 
 1. Follow the instructions in :ref:`prerequisites` to setup a clean conda
    environment. To be safe, run::
 
     $ pip uninstall elephant
 
@@ -19,20 +28,34 @@
 2. Fork `Elephant <https://github.com/NeuralEnsemble/elephant>`_ as described
    in `Fork a repo <https://help.github.com/en/github/getting-started-with-github/fork-a-repo>`_.
    Download Elephant source code from your forked repo::
 
     $ git clone git://github.com/<your-github-profile>/elephant.git
     $ cd elephant
 
-3. Install requirements.txt, (optionally) requirements-extras.txt, and
-   requirements-tests.txt::
+3. Install the requirements (either via pip or conda):
+
+.. tabs::
+
+    .. tab:: pip
+
+        .. code-block:: sh
+
+            pip install -r requirements/requirements.txt
+            pip install -r requirements/requirements-extras.txt  # optional
+            pip install -r requirements/requirements-tests.txt
+
+    .. tab:: conda
+
+        .. code-block:: sh
+
+            conda env create -f requirements/environment.yml
+            conda activate elephant
+            pip install -r requirements/requirements-tests.txt
 
-    $ pip install -r requirements/requirements.txt
-    $ pip install -r requirements/requirements-extras.txt  # optional
-    $ pip install -r requirements/requirements-tests.txt
 
 4. Before you make any changes, run the test suite to make sure all the tests
    pass on your system::
 
     $ nosetests .
 
    You can specify a particular module to test, for example
@@ -45,17 +68,17 @@
    on tests that failed or produced errors.
 
 5. **Implement the functional you want to add in Elephant**. This includes
    (either of them):
 
    * fixing a bug;
    * improving the documentation;
-   * adding a new functional.
+   * adding a new functionality.
 
-6. If it was a new functional, please write:
+6. If it is a new functionality, please write:
 
    - documentation (refer to :ref:`documentation_guide`);
    - tests to cover your new functions as much as possible.
 
 7. Run the tests again as described in step 4.
 
 8. Commit your changes::
@@ -65,11 +88,7 @@
     $ git push
 
    If this is your first commit to the project, please add your name and
    affiliation/employer to :file:`doc/authors.rst`
 
 9. Open a `pull request <https://github.com/NeuralEnsemble/elephant/pulls>`_.
    Then we'll merge your code in Elephant.
-
-
-.. note:: If you experience a problem during one of the steps above, please
-          contact us by :ref:`get_in_touch`.
```

### Comparing `elephant-0.8.0/doc/documentation_guide.rst` & `elephant-0.9.0/doc/documentation_guide.rst`

 * *Files identical despite different names*

### Comparing `elephant-0.8.0/doc/get_in_touch.rst` & `elephant-0.9.0/doc/get_in_touch.rst`

 * *Files identical despite different names*

### Comparing `elephant-0.8.0/doc/images/elephant_favicon.ico` & `elephant-0.9.0/doc/images/elephant_favicon.ico`

 * *Files identical despite different names*

### Comparing `elephant-0.8.0/doc/images/elephant_logo.png` & `elephant-0.9.0/doc/images/elephant_logo.png`

 * *Files identical despite different names*

### Comparing `elephant-0.8.0/doc/images/elephant_logo_sidebar.png` & `elephant-0.9.0/doc/images/elephant_logo_sidebar.png`

 * *Files identical despite different names*

### Comparing `elephant-0.8.0/doc/index.rst` & `elephant-0.9.0/doc/index.rst`

 * *Files 12% similar despite different names*

```diff
@@ -16,28 +16,40 @@
 neurotic_ for raw data visualization.
 
 The input-output data format is either Neo_, Quantity_ or Numpy_ array.
 Quantity is a Numpy-wrapper package for handling physical quantities like
 seconds, milliseconds, Hz, volts, etc. Quantity is used in both Neo and
 Elephant.
 
+
+**Visualization of Elephant analysis objects**
+
+`Viziphant <https://viziphant.readthedocs.io/en/latest/>`_ package is developed
+by Elephant team and provides a high-level API to easily generate plots and
+interactive visualizations of neuroscientific data and analysis results.
+The API uses and extends the same structure as in Elephant to ensure intuitive
+usage for scientists that are used to Elephant.
+
+
+
 Table of Contents
 -----------------
 
 .. toctree::
     :maxdepth: 1
 
     install
     tutorials
     modules
     developers_guide
     authors
     release_notes
     get_in_touch
     acknowledgments
+    citation
 
 
 
 .. Indices and tables
 .. ==================
 
 .. * :ref:`genindex`
```

### Comparing `elephant-0.8.0/doc/maintainers_guide.rst` & `elephant-0.9.0/doc/maintainers_guide.rst`

 * *Files 2% similar despite different names*

```diff
@@ -124,30 +124,32 @@
 3. Check that the copyright statement (in :file:`LICENSE.txt`,
    :file:`README.md`, and :file:`doc/conf.py`) is correct.
 
 4. If there is a new module do not forget to add the module name to the
    :file:`doc/modules.rst` and make a file with a short description in
    :file:`doc/reference/<modulename>.rst`.
 
-5. Remove :file:`elephant/spade_src/fim.so`. Otherwise, it'll be included in
+5. Push the commit with release notes and version updated to github.
+
+6. Remove :file:`elephant/spade_src/fim.so`. Otherwise, it'll be included in
    the built package (it should be downloaded at pip install).
 
-6. Build a source package and upload it to PyPi.
+7. Build a source package and upload it to PyPi.
 
    Build a source package (see `Packaging Python Projects
    <https://packaging.python.org/tutorials/packaging-projects/#generating-distribution-archives>`_)::
 
     $ pip install --user --upgrade twine
     $ python setup.py sdist
 
    To upload the package to `PyPI <http://pypi.python.org>`_
    (if you have the necessary permissions)::
 
     $ python -m twine upload dist/elephant-X.Y.Z.tar.gz
 
-7. Finally, make a release on GitHub UI page and copy-paste the release notes.
+8. Finally, make a release on GitHub UI page and copy-paste the release notes.
    Then tag the release in the Git repository and push it::
 
     $ git tag <version>
     $ git push --tags upstream
 
    Here, version should be of the form ``vX.Y.Z``.
```

### Comparing `elephant-0.8.0/doc/make.bat` & `elephant-0.9.0/doc/make.bat`

 * *Files identical despite different names*

### Comparing `elephant-0.8.0/doc/modules.rst` & `elephant-0.9.0/doc/modules.rst`

 * *Files 8% similar despite different names*

```diff
@@ -2,29 +2,34 @@
 Function Reference by Module
 ****************************
 
 .. toctree::
    :maxdepth: 1
 
    reference/asset
+   reference/causality
    reference/cell_assembly_detection
    reference/change_point_detection
    reference/conversion
    reference/cubic
    reference/current_source_density
    reference/gpfa
    reference/kernels
    reference/neo_tools
    reference/pandas_bridge
    reference/parallel
    reference/phase_analysis
    reference/signal_processing
    reference/spade
    reference/spectral
-   reference/spike_train_correlation
-   reference/spike_train_dissimilarity
    reference/spike_train_generation
    reference/spike_train_surrogates
    reference/sta
    reference/statistics
    reference/unitary_event_analysis
    reference/waveform_features
+
+
+.. toctree::
+   :maxdepth: 2
+
+   reference/_spike_train_processing
```

### Comparing `elephant-0.8.0/doc/reference/toctree/kernels/elephant.kernels.EpanechnikovLikeKernel.rst` & `elephant-0.9.0/doc/reference/toctree/kernels/elephant.kernels.EpanechnikovLikeKernel.rst`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,25 @@
-elephant.kernels.EpanechnikovLikeKernel
+﻿elephant.kernels.EpanechnikovLikeKernel
 =======================================
 
 .. currentmodule:: elephant.kernels
 
 .. autoclass:: EpanechnikovLikeKernel
    :members:
    :inherited-members:
+   :special-members: __call__
 
+   
 
+   
    .. rubric:: Methods
 
    .. autosummary::
    
-      ~EpanechnikovLikeKernel.__call__
+      ~EpanechnikovLikeKernel.__init__
       ~EpanechnikovLikeKernel.boundary_enclosing_area_fraction
       ~EpanechnikovLikeKernel.cdf
       ~EpanechnikovLikeKernel.icdf
       ~EpanechnikovLikeKernel.is_symmetric
       ~EpanechnikovLikeKernel.median_index
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `elephant-0.8.0/doc/reference/toctree/kernels/elephant.kernels.ExponentialKernel.rst` & `elephant-0.9.0/doc/reference/toctree/kernels/elephant.kernels.ExponentialKernel.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,25 @@
-elephant.kernels.ExponentialKernel
+﻿elephant.kernels.ExponentialKernel
 ==================================
 
 .. currentmodule:: elephant.kernels
 
 .. autoclass:: ExponentialKernel
    :members:
    :inherited-members:
+   :special-members: __call__
+
+   
 
    
    .. rubric:: Methods
 
    .. autosummary::
    
-      ~ExponentialKernel.__call__
+      ~ExponentialKernel.__init__
       ~ExponentialKernel.boundary_enclosing_area_fraction
       ~ExponentialKernel.cdf
       ~ExponentialKernel.icdf
       ~ExponentialKernel.is_symmetric
       ~ExponentialKernel.median_index
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `elephant-0.8.0/doc/reference/toctree/kernels/elephant.kernels.GaussianKernel.rst` & `elephant-0.9.0/doc/reference/toctree/kernels/elephant.kernels.AlphaKernel.rst`

 * *Files 25% similar despite different names*

```diff
@@ -1,32 +1,35 @@
-elephant.kernels.GaussianKernel
-===============================
+﻿elephant.kernels.AlphaKernel
+============================
 
 .. currentmodule:: elephant.kernels
 
-.. autoclass:: GaussianKernel
+.. autoclass:: AlphaKernel
    :members:
    :inherited-members:
+   :special-members: __call__
+
+   
 
    
    .. rubric:: Methods
 
    .. autosummary::
    
-      ~GaussianKernel.__call__
-      ~GaussianKernel.boundary_enclosing_area_fraction
-      ~GaussianKernel.cdf
-      ~GaussianKernel.icdf
-      ~GaussianKernel.is_symmetric
-      ~GaussianKernel.median_index
+      ~AlphaKernel.__init__
+      ~AlphaKernel.boundary_enclosing_area_fraction
+      ~AlphaKernel.cdf
+      ~AlphaKernel.icdf
+      ~AlphaKernel.is_symmetric
+      ~AlphaKernel.median_index
    
    
 
    
    
    .. rubric:: Attributes
 
    .. autosummary::
    
-      ~GaussianKernel.min_cutoff
+      ~AlphaKernel.min_cutoff
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `elephant-0.8.0/doc/reference/toctree/kernels/elephant.kernels.LaplacianKernel.rst` & `elephant-0.9.0/doc/reference/toctree/kernels/elephant.kernels.LaplacianKernel.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,25 @@
-elephant.kernels.LaplacianKernel
+﻿elephant.kernels.LaplacianKernel
 ================================
 
 .. currentmodule:: elephant.kernels
 
 .. autoclass:: LaplacianKernel
    :members:
    :inherited-members:
+   :special-members: __call__
+
+   
 
    
    .. rubric:: Methods
 
    .. autosummary::
    
-      ~LaplacianKernel.__call__
+      ~LaplacianKernel.__init__
       ~LaplacianKernel.boundary_enclosing_area_fraction
       ~LaplacianKernel.cdf
       ~LaplacianKernel.icdf
       ~LaplacianKernel.is_symmetric
       ~LaplacianKernel.median_index
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `elephant-0.8.0/doc/reference/toctree/kernels/elephant.kernels.RectangularKernel.rst` & `elephant-0.9.0/doc/reference/toctree/kernels/elephant.kernels.RectangularKernel.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,25 @@
-elephant.kernels.RectangularKernel
+﻿elephant.kernels.RectangularKernel
 ==================================
 
 .. currentmodule:: elephant.kernels
 
 .. autoclass:: RectangularKernel
    :members:
    :inherited-members:
+   :special-members: __call__
+
+   
 
    
    .. rubric:: Methods
 
    .. autosummary::
    
-      ~RectangularKernel.__call__
+      ~RectangularKernel.__init__
       ~RectangularKernel.boundary_enclosing_area_fraction
       ~RectangularKernel.cdf
       ~RectangularKernel.icdf
       ~RectangularKernel.is_symmetric
       ~RectangularKernel.median_index
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `elephant-0.8.0/doc/reference/toctree/kernels/elephant.kernels.TriangularKernel.rst` & `elephant-0.9.0/doc/reference/toctree/kernels/elephant.kernels.TriangularKernel.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,25 @@
-elephant.kernels.TriangularKernel
+﻿elephant.kernels.TriangularKernel
 =================================
 
 .. currentmodule:: elephant.kernels
 
 .. autoclass:: TriangularKernel
    :members:
    :inherited-members:
+   :special-members: __call__
+
+   
 
    
    .. rubric:: Methods
 
    .. autosummary::
    
-      ~TriangularKernel.__call__
+      ~TriangularKernel.__init__
       ~TriangularKernel.boundary_enclosing_area_fraction
       ~TriangularKernel.cdf
       ~TriangularKernel.icdf
       ~TriangularKernel.is_symmetric
       ~TriangularKernel.median_index
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `elephant-0.8.0/doc/release_notes.rst` & `elephant-0.9.0/doc/release_notes.rst`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,80 @@
 *************
 Release Notes
 *************
 
+
+Elephant 0.9.0 release notes
+============================
+
+This release is titled to accompany the [2nd Elephant User Workshop](https://www.humanbrainproject.eu/en/education/participatecollaborate/infrastructure-events-trainings/2nd-elephant-user-workshop/)
+
+Viziphant
+---------
+Meet Viziphant, the visualization of Elephant analysis methods, at https://viziphant.readthedocs.io/en/latest/. This package provides support to easily plot and visualize the output of Elephant functions in a few lines of code.
+
+Provenance tracking
+-------------------
+Provenance is becoming a separate direction in Elephant. Many things are still to come, and we started with annotating `time_histogram`, `instantaneous_rate` and `cross_correlation_histogram` outputs to carry the information about the parameters these functions used. This allowed Viziphant, the visualization of Elephant analyses, to look for the `.annotations` dictionary of the output of these function to "understand" how the object has been generated and label the plot axes accordingly.
+
+New functionality and features
+------------------------------
+* Time-domain pairwise and conditional pairwise Granger causality measures (https://github.com/NeuralEnsemble/elephant/pull/332, https://github.com/NeuralEnsemble/elephant/pull/359)
+* Spike contrast function that measures the synchrony of spike trains (https://github.com/NeuralEnsemble/elephant/pull/354; thanks to @Broxy7 for bringing this in Elephant).
+* Revised local variability LvR (https://github.com/NeuralEnsemble/elephant/pull/346) as an alternative to the LV measure.
+* Three surrogate methods: Trial-shifting, Bin Shuffling, ISI dithering (https://github.com/NeuralEnsemble/elephant/pull/343).
+* Added a new function to generate spike trains: `inhomogeneous_gamma_process` (https://github.com/NeuralEnsemble/elephant/pull/339).
+* The output of `instantaneous_rate` function is now a 2D matrix of shape `(time, len(spiketrains))` (https://github.com/NeuralEnsemble/elephant/issues/363). Not only can the users assess the averaged instantaneous rate (`rates.mean(axis=1)`) but also explore how much the instantaneous rate deviates from trial to trial (`rates.std(axis=1)`) (originally asked in https://github.com/NeuralEnsemble/elephant/issues/363).
+
+Python 3 only
+-------------
+* Python 2.7 and 3.5 support is dropped. You can still however enjoy the features of Elephant v0.9.0 with Python 2.7 or 3.5 by installing Elephant from [this](https://github.com/NeuralEnsemble/elephant/tree/295c6bd7fea196cf9665a78649fafedab5840cfa) commit `pip install git+https://github.com/NeuralEnsemble/elephant@295c6bd7fea196cf9665a78649fafedab5840cfa#egg=elephant[extras]`
+* Added Python 3.9 support.
+
+Optimization
+------------
+* You have been asking for direct numpy support for years. Added `_t_start`, `_t_stop`, and `_bin_size` attributes of BinnedSpikeTrain are guaranteed to be of the same units and hence are unitless (https://github.com/NeuralEnsemble/elephant/pull/378). It doesn't mean though that you need to care about units on your own: `t_start`, `t_stop`, and `bin_size` properties are still quantities with units. The `.rescale()` method of a BinnedSpikeTrain rescales the internal units to new ones in-place. The following Elephant functions are optimized with unitless BinnedSpikeTrain:
+  - cross_correlation_histogram
+  - bin_shuffling (one of the surrogate methods)
+  - spike_train_timescale
+* X4 faster binning and overall BinnedSpikeTrain object creation (https://github.com/NeuralEnsemble/elephant/pull/368).
+* `instantaneous_rate` function is vectorized to work with a list of spike train trials rather than computing them in a loop (previously, `for spiketrain in spiketrains; do compute instantaneous_rate(spiketrain); done`), which brought X25 speedup (https://github.com/NeuralEnsemble/elephant/pull/362; thanks to @gyyang for the idea and original implementation).
+* Memory-efficient `zscore` function (https://github.com/NeuralEnsemble/elephant/pull/372).
+* Don't sort the input array in ISI function (https://github.com/NeuralEnsemble/elephant/pull/371), which reduces function algorithmic time complexity from `O(N logN)` to linear `O(N)`. Now, when the input time array is not sorted, a warning is shown.
+* Vectorized Current Source Density `generate_lfp` function (https://github.com/NeuralEnsemble/elephant/pull/358).
+
+Breaking changes
+----------------
+* mpi4py package is removed from the extra requirements to allow `pip install elephant[extras]` on machines without MPI installed system-wide. Refer to [MPI support](https://elephant.readthedocs.io/en/latest/install.html#mpi-support) installation page in elephant.
+* BinnedSpikeTrain (https://github.com/NeuralEnsemble/elephant/pull/368, https://github.com/NeuralEnsemble/elephant/pull/377):
+  - previously, when t_start/stop, if set manually, was outside of the shared time interval, only the shared [t_start_shared=max(t_start), t_stop_shared=min(t_stop)] interval was implicitly considered without any warnings. Now an error is thrown with a description on how to fix it.
+  - removed `lst_input`, `input_spiketrains`, `matrix_columns`, `matrix_rows` (in favor of the new attribute - `shape`), `tolerance`, `is_spiketrain`, `is_binned` attributes from BinnedSpikeTrain class. Part of them are confusing (e.g., `is_binned` was just the opposite of `is_spiketrain`, but one can erroneously think that it's data is clipped to 0 and 1), and part of them - `lst_input`, `input_spiketrains` input data - should not have been saved as attributes of an object in the first place because the input spike trains are not used after the sparse matrix is created.
+  - now the users can directly access `.sparse_matrix` attribute of BinnedSpikeTrain to do efficient (yet unsafe in general) operations. For this reason, `to_sparse_array()` function, which does not make a copy, as one could think of, is deprecated.
+* `instantaneous_rate` function (https://github.com/NeuralEnsemble/elephant/pull/362):
+  - in case of multiple input spike trains, the output of the instantaneous rate function is (always) a 2D matrix of shape `(time, len(spiketrains))` instead of a pseudo 1D array (previous behavior) of shape `(time, 1)` that contained the instantaneous rate summed across input spike trains;
+  - in case of multiple input spike trains, the user needs to manually provide the input kernel instead of `auto`, which is set by default, for the reason that it's currently not clear how to estimate the common kernel for a set of spike trains. If you have an idea how to do this, we`d appreciate if you let us know by [getting in touch with us](https://elephant.readthedocs.io/en/latest/get_in_touch.html).
+
+Other changes
+-------------
+* `waveform_snr` function now directly takes a 2D or 3D waveforms matrix rather than a spike train (deprecated behavior).
+* Added a warning in fanofactor function when the input spiketrains vary in their durations (https://github.com/NeuralEnsemble/elephant/pull/341).
+* SPADE: New way to count patterns for multiple testing (https://github.com/NeuralEnsemble/elephant/pull/347)
+* GPFA renamed 'xsm' -> 'latent_variable' and 'xorth' -> 'latent_variable_orth'
+
+Bug fixes
+---------
+* Instantaneous rate arrays were not centered at the origin for spike trains that are symmetric at t=0 with `center_kernel=True` option (https://github.com/NeuralEnsemble/elephant/pull/362).
+* The number of discarded spikes that fall into the last bin of a BinnedSpikeTrain object was incorrectly calculated (https://github.com/NeuralEnsemble/elephant/pull/368).
+* Fixed index selection in `spike_triggered_phase` (https://github.com/NeuralEnsemble/elephant/pull/382)
+* Fixed surrogates bugs:
+  - `joint-ISI` and `shuffle ISI` output spike trains were not sorted in time (https://github.com/NeuralEnsemble/elephant/pull/364);
+  - surrogates get arbitrary sampling_rate (https://github.com/NeuralEnsemble/elephant/pull/353), which relates to the provenance tracking issue;
+
+
+
 Elephant 0.8.0 release notes
 ============================
 
 New features
 ------------
 * The `parallel` module is a new experimental module (https://github.com/NeuralEnsemble/elephant/pull/307) to run python functions concurrently. Supports native (pythonic) ProcessPollExecutor and MPI. Not limited to Elephant functional.
 * Added an optional `refractory_period` argument, set to None by default, to `dither_spikes` function (https://github.com/NeuralEnsemble/elephant/pull/297).
@@ -25,15 +94,14 @@
 ------------------------------
 Python 2.7 and 3.5 are deprecated and will not be maintained by the end of 2020. Switch to Python 3.6+.
 
 Breaking changes
 ----------------
 * Naming convention changes (`binsize` -> `bin_size`, etc.) in almost all Elephant functions (https://github.com/NeuralEnsemble/elephant/pull/316).
 
-
 Elephant 0.7.0 release notes
 ============================
 
 Breaking changes
 ----------------
 * [gpfa] GPFA dimensionality reduction method is rewritten in easy-to-use scikit-learn class style format (https://github.com/NeuralEnsemble/elephant/pull/287):
```

### Comparing `elephant-0.8.0/doc/style_guide.rst` & `elephant-0.9.0/doc/style_guide.rst`

 * *Files identical despite different names*

### Comparing `elephant-0.8.0/doc/tutorials/asset.ipynb` & `elephant-0.9.0/doc/tutorials/asset.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.999537037037037%*

 * *Differences: {"'cells'": "{5: {'source': ['!curl "*

 * *            'https://web.gin.g-node.org/INM-6/elephant-data/raw/master/dataset-2/asset_showcase_500.nix '*

 * *            "--output asset_showcase_500.nix --location']}}"}*

```diff
@@ -80,15 +80,15 @@
         },
         {
             "cell_type": "code",
             "execution_count": 3,
             "metadata": {},
             "outputs": [],
             "source": [
-                "!wget -N https://web.gin.g-node.org/INM-6/elephant-data/raw/master/dataset-2/asset_showcase_500.nix"
+                "!curl https://web.gin.g-node.org/INM-6/elephant-data/raw/master/dataset-2/asset_showcase_500.nix --output asset_showcase_500.nix --location"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "The data is represented as a `neo.Block` with one `neo.Segment` inside, which contains raw `neo.SpikeTrain`s. For more information on `neo.Block`, `neo.Segment`, and `neo.SpikeTrain` refer to https://neo.readthedocs.io/en/stable/core.html"
```

### Comparing `elephant-0.8.0/doc/tutorials/asset_showcase_500.nix` & `elephant-0.9.0/doc/tutorials/asset_showcase_500.nix`

 * *Files identical despite different names*

### Comparing `elephant-0.8.0/doc/tutorials/gpfa.ipynb` & `elephant-0.9.0/doc/tutorials/gpfa.ipynb`

 * *Files identical despite different names*

### Comparing `elephant-0.8.0/doc/tutorials/parallel.ipynb` & `elephant-0.9.0/doc/tutorials/parallel.ipynb`

 * *Files identical despite different names*

### Comparing `elephant-0.8.0/doc/tutorials/statistics.ipynb` & `elephant-0.9.0/doc/tutorials/statistics.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998759920634921%*

 * *Differences: {"'cells'": "{1: {'source': {insert: [(0, '## 1. Generating homogeneous Poisson and Gamma "*

 * *            "processes\\n')], delete: [0]}}}"}*

```diff
@@ -11,15 +11,15 @@
                 "This notebook provides an overview of the functions provided by the elephant `statistics` module.\n"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "## 1. Generating homogeneous Poisson and Gama processes\n",
+                "## 1. Generating homogeneous Poisson and Gamma processes\n",
                 "\n",
                 "All measures presented here require one or two spiketrains as input. We start by importing physical quantities (seconds, milliseconds and Hertz) and two generators of spiketrains - `homogeneous_poisson_process()` and `homogeneous_gamma_process()` functions from `elephant.spike_train_generation` module.\n",
                 "\n",
                 "Let's explore `homogeneous_poisson_process()` function in details with Python `help()` command."
             ]
         },
         {
```

### Comparing `elephant-0.8.0/doc/tutorials/unitary_event_analysis.ipynb` & `elephant-0.9.0/doc/tutorials/unitary_event_analysis.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9992424242424243%*

 * *Differences: {"'cells'": "{4: {'source': {insert: [(1, '!curl "*

 * *            'https://web.gin.g-node.org/INM-6/elephant-data/raw/master/dataset-1/dataset-1.h5 '*

 * *            "--output dataset-1.h5 --location')], delete: [1]}}}"}*

```diff
@@ -69,15 +69,15 @@
                     "end_time": "2018-07-18T08:56:32.142189Z",
                     "start_time": "2018-07-18T08:56:31.420462Z"
                 }
             },
             "outputs": [],
             "source": [
                 "# Download data\n",
-                "!wget -Nq https://web.gin.g-node.org/INM-6/elephant-data/raw/master/dataset-1/dataset-1.h5"
+                "!curl https://web.gin.g-node.org/INM-6/elephant-data/raw/master/dataset-1/dataset-1.h5 --output dataset-1.h5 --location"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "nbsphinx": "hidden"
             },
```

### Comparing `elephant-0.8.0/doc/tutorials.rst` & `elephant-0.9.0/doc/tutorials.rst`

 * *Files identical despite different names*

### Comparing `elephant-0.8.0/elephant/__init__.py` & `elephant-0.9.0/elephant/__init__.py`

 * *Files identical despite different names*

### Comparing `elephant-0.8.0/elephant/asset.py` & `elephant-0.9.0/elephant/asset.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 """
-ASSET is a statistical method :cite:`asset-torre2016asset` for the detection of
-repeating sequences of synchronous spiking events in parallel spike trains.
+ASSET is a statistical method :cite:`asset-Torre16_e1004939` for the detection
+of repeating sequences of synchronous spiking events in parallel spike trains.
 
 
 ASSET analysis class object of finding patterns
 -----------------------------------------------
 
 .. autosummary::
     :toctree: toctree/asset/
@@ -121,14 +121,25 @@
     rank = comm.Get_rank()
 except ImportError:
     mpi_accelerated = False
     size = 1
     rank = 0
 
 
+__all__ = [
+    "ASSET",
+    "synchronous_events_intersection",
+    "synchronous_events_difference",
+    "synchronous_events_identical",
+    "synchronous_events_no_overlap",
+    "synchronous_events_contained_in",
+    "synchronous_events_contains_all",
+    "synchronous_events_overlap"
+]
+
 # =============================================================================
 # Some Utility Functions to be dealt with in some way or another
 # =============================================================================
 
 
 def _signals_same_attribute(signals, attr_name):
     """
@@ -1113,16 +1124,16 @@
         spiketrains, bin_size=bin_size,
         t_start=t_start_x, t_stop=t_stop_x)
     spiketrains_binned_y = conv.BinnedSpikeTrain(
         spiketrains_y, bin_size=bin_size,
         t_start=t_start_y, t_stop=t_stop_y)
 
     # Compute imat by matrix multiplication
-    bsts_x = spiketrains_binned.to_sparse_array()
-    bsts_y = spiketrains_binned_y.to_sparse_array()
+    bsts_x = spiketrains_binned.sparse_matrix
+    bsts_y = spiketrains_binned_y.sparse_matrix
 
     # Compute the number of spikes in each bin, for both time axes
     # 'A1' property returns self as a flattened ndarray.
     spikes_per_bin_x = bsts_x.sum(axis=0).A1
     spikes_per_bin_y = bsts_y.sum(axis=0).A1
 
     # Compute the intersection matrix imat
```

### Comparing `elephant-0.8.0/elephant/cell_assembly_detection.py` & `elephant-0.9.0/elephant/cell_assembly_detection.py`

 * *Files 0% similar despite different names*

```diff
@@ -76,14 +76,18 @@
 
 import numpy as np
 from scipy.stats import f
 
 import elephant.conversion as conv
 from elephant.utils import deprecated_alias
 
+__all__ = [
+    "cell_assembly_detection"
+]
+
 
 @deprecated_alias(data='binned_spiketrain', maxlag='max_lag',
                   min_occ='min_occurrences',
                   same_config_cut='same_configuration_pruning')
 def cell_assembly_detection(binned_spiketrain, max_lag, reference_lag=2,
                             alpha=0.05, min_occurrences=1, size_chunks=100,
                             max_spikes=np.inf, significance_pruning=True,
@@ -1192,15 +1196,15 @@
 
     if size_chunks < 2:
         raise ValueError('length of the chunks cannot be 1 or less')
 
     if max_spikes < 2:
         raise ValueError('maximal assembly order must be less than 2')
 
-    if binned_spiketrain.matrix_columns - max_lag < 100:
+    if binned_spiketrain.shape[1] - max_lag < 100:
         raise ValueError('The time series is too short, consider '
                          'taking a longer portion of spike train '
                          'or diminish the bin size to be tested')
 
 
 # alias for the function
 cad = cell_assembly_detection
```

### Comparing `elephant-0.8.0/elephant/change_point_detection.py` & `elephant-0.9.0/elephant/change_point_detection.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,14 +49,19 @@
 from __future__ import division, print_function, unicode_literals
 
 import numpy as np
 import quantities as pq
 
 from elephant.utils import deprecated_alias
 
+__all__ = [
+    "multiple_filter_test",
+    "empirical_parameters"
+]
+
 
 @deprecated_alias(dt='time_step')
 def multiple_filter_test(window_sizes, spiketrain, t_final, alpha,
                          n_surrogates, test_quantile=None, test_param=None,
                          time_step=None):
     """
     Detects change points.
```

### Comparing `elephant-0.8.0/elephant/conversion.py` & `elephant-0.9.0/elephant/conversion.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,29 +2,41 @@
 """
 This module allows to convert standard data representations
 (e.g., a spike train stored as Neo SpikeTrain object)
 into other representations useful to perform calculations on the data.
 An example is the representation of a spike train as a sequence of 0-1 values
 (binned spike train).
 
+
+.. autosummary::
+    :toctree: toctree/conversion
+
+    BinnedSpikeTrain
+    binarize
+
 :copyright: Copyright 2014-2016 by the Elephant team, see `doc/authors.rst`.
 :license: BSD, see LICENSE.txt for details.
 """
 
 from __future__ import division, print_function, unicode_literals
 
 import warnings
-from copy import deepcopy
 
 import neo
 import numpy as np
 import quantities as pq
 import scipy.sparse as sps
 
-from elephant.utils import is_binary, deprecated_alias
+from elephant.utils import is_binary, deprecated_alias, \
+    check_neo_consistency, get_common_start_stop_times
+
+__all__ = [
+    "binarize",
+    "BinnedSpikeTrain"
+]
 
 
 def binarize(spiketrain, sampling_rate=None, t_start=None, t_stop=None,
              return_times=False):
     """
     Return an array indicating if spikes occurred at individual time points.
 
@@ -175,184 +187,18 @@
 
 def _detect_rounding_errors(values, tolerance):
     """
     Finds rounding errors in values that will be cast to int afterwards.
     Returns True for values that are within tolerance of the next integer.
     Works for both scalars and numpy arrays.
     """
-    if tolerance is None:
+    if tolerance is None or tolerance == 0:
         return np.zeros_like(values, dtype=bool)
-    return 1 - (values % 1) <= tolerance
-
-
-def _calc_tstart(n_bins, bin_size, t_stop):
-    """
-    Calculates the start point from given parameters.
-
-    Calculates the start point `t_start` from the three parameters
-    `n_bins`, `bin_size`, `t_stop`.
-
-    Parameters
-    ----------
-    n_bins : int
-        Number of bins
-    bin_size : pq.Quantity
-        Size of Bins
-    t_stop : pq.Quantity
-        Stop time
-
-    Returns
-    -------
-    t_start : pq.Quantity
-        Starting point calculated from given parameters.
-    """
-    if n_bins is not None and bin_size is not None and t_stop is not None:
-        return t_stop.rescale(bin_size.units) - n_bins * bin_size
-
-
-def _calc_tstop(n_bins, bin_size, t_start):
-    """
-    Calculates the stop point from given parameters.
-
-    Calculates the stop point `t_stop` from the three parameters
-    `n_bins`, `bin_size`, `t_start`.
-
-    Parameters
-    ----------
-    n_bins : int
-        Number of bins
-    bin_size : pq.Quantity
-        Size of bins
-    t_start : pq.Quantity
-        Start time
-
-    Returns
-    -------
-    t_stop : pq.Quantity
-        Stopping point calculated from given parameters.
-    """
-    if n_bins is not None and bin_size is not None and t_start is not None:
-        return t_start.rescale(bin_size.units) + n_bins * bin_size
-
-
-def _calc_number_of_bins(bin_size, t_start, t_stop, tolerance):
-    """
-    Calculates the number of bins from given parameters.
-
-    Calculates the number of bins `n_bins` from the three parameters
-    `bin_size`, `t_start`, `t_stop`.
-
-    Parameters
-    ----------
-    bin_size : pq.Quantity
-        Size of Bins
-    t_start : pq.Quantity
-        Start time
-    t_stop : pq.Quantity
-        Stop time
-    tolerance : float
-        tolerance for detection of rounding errors before casting
-        the resulting num. of bins to integer
-
-    Returns
-    -------
-    n_bins : int
-       Number of bins calculated from given parameters.
-
-    Raises
-    ------
-    ValueError
-        When `t_stop` is smaller than `t_start`".
-
-    """
-    if bin_size is not None and t_start is not None and t_stop is not None:
-        if t_stop < t_start:
-            raise ValueError("t_stop (%s) is smaller than t_start (%s)"
-                             % (t_stop, t_start))
-        n_bins = ((t_stop - t_start).rescale(
-                        bin_size.units) / bin_size.magnitude).item()
-        if _detect_rounding_errors(n_bins, tolerance):
-            warnings.warn('Correcting a rounding error in the calculation '
-                          'of n_bins by increasing n_bins by 1. '
-                          'You can set tolerance=None to disable this '
-                          'behaviour.')
-            n_bins += 1
-        return int(n_bins)
-
-
-def _calc_bin_size(n_bins, t_start, t_stop):
-    """
-    Calculates the stop point from given parameters.
-
-    Calculates the size of bins `bin_size` from the three parameters
-    `n_bins`, `t_start` and `t_stop`.
-
-    Parameters
-    ----------
-    n_bins : int
-        Number of bins
-    t_start : pq.Quantity
-        Start time
-    t_stop : pq.Quantity
-        Stop time
-
-    Returns
-    -------
-    bin_size : pq.Quantity
-        Size of bins calculated from given parameters.
-
-    Raises
-    ------
-    ValueError
-        When `t_stop` is smaller than `t_start`.
-    """
-
-    if n_bins is not None and t_start is not None and t_stop is not None:
-        if t_stop < t_start:
-            raise ValueError("t_stop (%s) is smaller than t_start (%s)"
-                             % (t_stop, t_start))
-        return (t_stop - t_start) / n_bins
-
-
-def _get_start_stop_from_input(spiketrains):
-    """
-    Extracts the `t_start`and the `t_stop` from 'spiketrains'.
-
-    If a single `neo.SpikeTrain` is given, the `t_start `and
-    `t_stop` of this spike train is returned.
-    Otherwise, the aligned times are returned: the maximal `t_start` and
-    minimal `t_stop` across `spiketrains`.
-
-    Parameters
-    ----------
-    spiketrains : neo.SpikeTrain or list or np.ndarray of neo.SpikeTrain
-        `neo.SpikeTrain`s to extract `t_start` and `t_stop` from.
-
-    Returns
-    -------
-    start : pq.Quantity
-        Start point extracted from input `spiketrains`
-    stop : pq.Quantity
-        Stop point extracted from input `spiketrains`
-
-    Raises
-    ------
-    AttributeError
-        If spiketrains (or any element of it) do not have `t_start` or `t_stop`
-        attribute.
-    """
-    if isinstance(spiketrains, neo.SpikeTrain):
-        return spiketrains.t_start, spiketrains.t_stop
-    else:
-        try:
-            start = max([elem.t_start for elem in spiketrains])
-            stop = min([elem.t_stop for elem in spiketrains])
-        except AttributeError as ae:
-            raise AttributeError(ae, 'Please provide t_start or t_stop')
-    return start, stop
+    # same as '1 - (values % 1) <= tolerance' but faster
+    return 1 - tolerance <= values % 1
 
 
 class BinnedSpikeTrain(object):
     """
     Class which calculates a binned spike train and provides methods to
     transform the binned spike train to a boolean matrix or a matrix with
     counted time points.
@@ -444,233 +290,231 @@
     requirements.
 
     """
 
     @deprecated_alias(binsize='bin_size', num_bins='n_bins')
     def __init__(self, spiketrains, bin_size=None, n_bins=None, t_start=None,
                  t_stop=None, tolerance=1e-8):
-        """
-        Defines a BinnedSpikeTrain class
-
-        """
-        self.is_spiketrain = _check_neo_spiketrain(spiketrains)
-        if not self.is_spiketrain:
-            self.is_binned = _check_binned_array(spiketrains)
-        else:
-            self.is_binned = False
         # Converting spiketrains to a list, if spiketrains is one
         # SpikeTrain object
-        if isinstance(spiketrains,
-                      neo.SpikeTrain) and self.is_spiketrain:
+        if isinstance(spiketrains, neo.SpikeTrain):
             spiketrains = [spiketrains]
 
-        # Link to input
-        self.input_spiketrains = spiketrains
         # Set given parameters
-        self.t_start = t_start
-        self.t_stop = t_stop
+        self._t_start = t_start
+        self._t_stop = t_stop
         self.n_bins = n_bins
-        self.bin_size = bin_size
-        self.tolerance = tolerance
-        # Empty matrix for storage, time points matrix
-        self._mat_u = None
-        # Variables to store the sparse matrix
-        self._sparse_mat_u = None
+        self._bin_size = bin_size
+        self.units = None  # will be set later
         # Check all parameter, set also missing values
-        if self.is_binned:
-            self.n_bins = np.shape(spiketrains)[1]
-        self._calc_start_stop(spiketrains)
-        self._check_init_params(
-            self.bin_size, self.n_bins, self.t_start, self.t_stop)
-        self._check_consistency(spiketrains, self.bin_size, self.n_bins,
-                                self.t_start, self.t_stop)
-        # Now create sparse matrix
-        self._convert_to_binned(spiketrains)
-
-        if self.is_spiketrain:
-            n_spikes = sum(map(len, spiketrains))
-            n_spikes_binned = self.get_num_of_spikes()
-            if n_spikes != n_spikes_binned:
-                warnings.warn("Binning discarded {n} last spike(s) in the "
-                              "input spiketrain.".format(
-                                  n=n_spikes - n_spikes_binned))
+        self._resolve_input_parameters(spiketrains, tolerance=tolerance)
+        # Now create the sparse matrix
+        self.sparse_matrix = self._create_sparse_matrix(spiketrains,
+                                                        tolerance=tolerance)
 
     @property
-    def matrix_rows(self):
-        return self._sparse_mat_u.shape[0]
+    def shape(self):
+        return self.sparse_matrix.shape
 
     @property
-    def matrix_columns(self):
-        return self._sparse_mat_u.shape[1]
+    def bin_size(self):
+        return pq.Quantity(self._bin_size, units=self.units, copy=False)
 
     @property
-    def binsize(self):
-        warnings.warn("'.binsize' is deprecated; use '.bin_size'",
-                      DeprecationWarning)
-        return self.bin_size
+    def t_start(self):
+        return pq.Quantity(self._t_start, units=self.units, copy=False)
+
+    @property
+    def t_stop(self):
+        return pq.Quantity(self._t_stop, units=self.units, copy=False)
 
     @property
-    def lst_input(self):
-        warnings.warn("'.lst_input' is deprecated; use '.input_spiketrains'",
+    def binsize(self):
+        warnings.warn("'.binsize' is deprecated; use '.bin_size'",
                       DeprecationWarning)
-        return self.input_spiketrains
+        return self._bin_size
 
     @property
     def num_bins(self):
         warnings.warn("'.num_bins' is deprecated; use '.n_bins'")
         return self.n_bins
 
-    # =========================================================================
-    # There are four cases the given parameters must fulfill, or a `ValueError`
-    # will be raised:
-    # t_start, n_bins, bin_size
-    # t_start, n_bins, t_stop
-    # t_start, bin_size, t_stop
-    # t_stop, n_bins, bin_size
-    # =========================================================================
+    def __repr__(self):
+        return "{klass}(t_start={t_start}, t_stop={t_stop}, " \
+               "bin_size={bin_size}; shape={shape})".format(
+                     klass=type(self).__name__,
+                     t_start=self.t_start,
+                     t_stop=self.t_stop,
+                     bin_size=self.bin_size,
+                     shape=self.shape)
 
-    def _check_init_params(self, bin_size, n_bins, t_start, t_stop):
+    def rescale(self, units):
         """
-        Checks given parameters.
-        Calculates also missing parameter.
+        Inplace rescaling to the new quantity units.
 
         Parameters
         ----------
-        bin_size : pq.Quantity
-            Size of bins
-        n_bins : int
-            Number of bins
-        t_start: pq.Quantity
-            Start time for the binned spike train
-        t_stop: pq.Quantity
-            Stop time for the binned spike train
+        units : pq.Quantity or str
+            New quantity units.
 
         Raises
         ------
         TypeError
-            If type of `n_bins` is not an `int`.
-        ValueError
-            When `t_stop` is smaller than `t_start`.
-
-        """
-        # Check if n_bins is an integer (special case)
-        if n_bins is not None:
-            if not np.issubdtype(type(n_bins), np.integer):
-                raise TypeError("'n_bins' is not an integer!")
-        # Check if all parameters can be calculated, otherwise raise ValueError
-        if t_start is None:
-            self.t_start = _calc_tstart(n_bins, bin_size, t_stop)
-        elif t_stop is None:
-            self.t_stop = _calc_tstop(n_bins, bin_size, t_start)
-        elif n_bins is None:
-            self.n_bins = _calc_number_of_bins(bin_size, t_start, t_stop,
-                                               self.tolerance)
-        elif bin_size is None:
-            self.bin_size = _calc_bin_size(n_bins, t_start, t_stop)
+            If the input units are not quantities.
 
-    def _calc_start_stop(self, spiketrains):
+        """
+        if isinstance(units, str):
+            units = pq.Quantity(1, units=units)
+        if units == self.units:
+            # do nothing
+            return
+        if not isinstance(units, pq.Quantity):
+            raise TypeError("The input units must be quantities or string")
+        scale = self.units.rescale(units).item()
+        self._t_stop *= scale
+        self._t_start *= scale
+        self._bin_size *= scale
+        self.units = units
+
+    def __resolve_binned(self, spiketrains):
+        spiketrains = np.asarray(spiketrains)
+        if spiketrains.ndim != 2 or spiketrains.dtype == np.dtype('O'):
+            raise ValueError("If the input is not a spiketrain(s), it "
+                             "must be an MxN numpy array, each cell of "
+                             "which represents the number of (binned) "
+                             "spikes that fall in an interval - not "
+                             "raw spike times.")
+        if self.n_bins is not None:
+            raise ValueError("When the input is a binned matrix, 'n_bins' "
+                             "must be set to None - it's extracted from the "
+                             "input shape.")
+        self.n_bins = spiketrains.shape[1]
+        if self._bin_size is None:
+            if self._t_start is None or self._t_stop is None:
+                raise ValueError("To determine the bin size, both 't_start' "
+                                 "and 't_stop' must be set")
+            self._bin_size = (self._t_stop - self._t_start) / self.n_bins
+        if self._t_start is None and self._t_stop is None:
+            raise ValueError("Either 't_start' or 't_stop' must be set")
+        if self._t_start is None:
+            self._t_start = self._t_stop - self._bin_size * self.n_bins
+        if self._t_stop is None:
+            self._t_stop = self._t_start + self._bin_size * self.n_bins
+
+    def _resolve_input_parameters(self, spiketrains, tolerance):
         """
         Calculates `t_start`, `t_stop` from given spike trains.
 
         The start and stop points are calculated from given spike trains only
         if they are not calculable from given parameters or the number of
         parameters is less than three.
 
         Parameters
         ----------
         spiketrains : neo.SpikeTrain or list or np.ndarray of neo.SpikeTrain
 
         """
-        if self._count_params() is False:
-            start, stop = _get_start_stop_from_input(spiketrains)
-            if self.t_start is None:
-                self.t_start = start
-            if self.t_stop is None:
-                self.t_stop = stop
-
-    def _count_params(self):
-        """
-        Checks the number of explicitly provided parameters and returns `True`
-        if the count is greater or equal `3`.
-
-        The calculation of the binned matrix is only possible if there are at
-        least three parameters (fourth parameter will be calculated out of
-        them).
-        This method checks if the necessary parameters are not `None` and
-        returns `True` if the count is greater or equal to `3`.
+        def get_n_bins():
+            n_bins = (self._t_stop - self._t_start) / self._bin_size
+            if isinstance(n_bins, pq.Quantity):
+                n_bins = n_bins.simplified.item()
+            if _detect_rounding_errors(n_bins, tolerance=tolerance):
+                warnings.warn('Correcting a rounding error in the calculation '
+                              'of n_bins by increasing n_bins by 1. '
+                              'You can set tolerance=None to disable this '
+                              'behaviour.')
+            return int(n_bins)
 
-        Returns
-        -------
-        bool
-            True, if the count of not None parameters is greater or equal to
-            `3`, False otherwise.
+        def check_n_bins_consistency():
+            if self.n_bins != get_n_bins():
+                raise ValueError(
+                    "Inconsistent arguments: t_start ({t_start}), "
+                    "t_stop ({t_stop}), bin_size ({bin_size}), and "
+                    "n_bins ({n_bins})".format(
+                        t_start=self.t_start, t_stop=self.t_stop,
+                        bin_size=self.bin_size, n_bins=self.n_bins))
+
+        def check_consistency():
+            if self.t_start >= self.t_stop:
+                raise ValueError("t_start must be smaller than t_stop")
+            if not isinstance(self.n_bins, int) or self.n_bins <= 0:
+                raise TypeError("The number of bins ({}) must be a positive "
+                                "integer".format(self.n_bins))
+
+        if not _check_neo_spiketrain(spiketrains):
+            # a binned numpy matrix
+            self.__resolve_binned(spiketrains)
+            self.units = self._bin_size.units
+            check_n_bins_consistency()
+            check_consistency()
+            self._t_start = self._t_start.rescale(self.units).item()
+            self._t_stop = self._t_stop.rescale(self.units).item()
+            self._bin_size = self._bin_size.rescale(self.units).item()
+            return
 
-        """
-        return sum(x is not None for x in
-                   [self.t_start, self.t_stop, self.bin_size,
-                    self.n_bins]) >= 3
+        if self._bin_size is None and self.n_bins is None:
+            raise ValueError("Either 'bin_size' or 'n_bins' must be given")
 
-    def _check_consistency(self, spiketrains, bin_size, n_bins, t_start,
-                           t_stop):
-        """
-        Checks the given parameters for consistency
+        try:
+            check_neo_consistency(spiketrains,
+                                  object_type=neo.SpikeTrain,
+                                  t_start=self._t_start,
+                                  t_stop=self._t_stop,
+                                  tolerance=tolerance)
+        except ValueError as er:
+            # different t_start/t_stop
+            raise ValueError(er, "If you want to bin over the shared "
+                                 "[t_start, t_stop] interval, provide "
+                                 "shared t_start and t_stop explicitly, "
+                                 "which can be obtained like so: "
+                                 "t_start, t_stop = elephant.utils."
+                                 "get_common_start_stop_times(spiketrains)"
+                             )
+
+        if self._t_start is None:
+            self._t_start = spiketrains[0].t_start
+        if self._t_stop is None:
+            self._t_stop = spiketrains[0].t_stop
+        # At this point, all spiketrains share the same units.
+        self.units = spiketrains[0].units
 
-        Raises
-        ------
-        AttributeError
-            If there is an insufficient number of parameters.
-        TypeError
-            If `n_bins` is not an `int` or is <0.
-        ValueError
-            If an inconsistency regarding the parameters appears, e.g.
-            `t_start` > `t_stop`.
-
-        """
-        if self._count_params() is False:
-            raise AttributeError("Too few parameters given. Please provide "
-                                 "at least one of the parameter which are "
-                                 "None.\n"
-                                 "t_start: %s, t_stop: %s, bin_size: %s, "
-                                 "n_bins: %s" % (
-                                     self.t_start,
-                                     self.t_stop,
-                                     self.bin_size,
-                                     self.n_bins))
-        if self.is_spiketrain:
-            t_starts = [elem.t_start for elem in spiketrains]
-            t_stops = [elem.t_stop for elem in spiketrains]
-            max_tstart = max(t_starts)
-            min_tstop = min(t_stops)
-            if max_tstart >= min_tstop:
-                raise ValueError("Starting time of each spike train must be "
-                                 "smaller than each stopping time")
-            if t_start < max_tstart or t_start > min_tstop:
-                raise ValueError(
-                    'some spike trains are not defined in the time given '
-                    'by t_start')
-            if not (t_start < t_stop <= min_tstop):
-                raise ValueError(
-                    'too many / too large time bins. Some spike trains are '
-                    'not defined in the ending time')
+        try:
+            self._t_start = self._t_start.rescale(self.units).item()
+            self._t_stop = self._t_stop.rescale(self.units).item()
+        except AttributeError:
+            raise ValueError("'t_start' and 't_stop' must be quantities")
+
+        start_shared, stop_shared = get_common_start_stop_times(spiketrains)
+        start_shared = start_shared.rescale(self.units).item()
+        stop_shared = stop_shared.rescale(self.units).item()
+
+        if tolerance is None:
+            tolerance = 0
+        if self._t_start < start_shared - tolerance \
+                or self._t_stop > stop_shared + tolerance:
+            raise ValueError("'t_start' ({t_start}) or 't_stop' ({t_stop}) is "
+                             "outside of the shared [{start_shared}, "
+                             "{stop_shared}] interval".format(
+                                 t_start=self.t_start, t_stop=self.t_stop,
+                                 start_shared=start_shared,
+                                 stop_shared=stop_shared))
+
+        if self.n_bins is None:
+            # bin_size is provided
+            self._bin_size = self._bin_size.rescale(self.units).item()
+            self.n_bins = get_n_bins()
+        elif self._bin_size is None:
+            # n_bins is provided
+            self._bin_size = (self._t_stop - self._t_start) / self.n_bins
+        else:
+            # both n_bins are bin_size are given
+            self._bin_size = self._bin_size.rescale(self.units).item()
+            check_n_bins_consistency()
 
-        # account for rounding errors in the reference num_bins
-        n_bins_test = ((
-            (t_stop - t_start).rescale(
-                bin_size.units) / bin_size).magnitude)
-        if _detect_rounding_errors(n_bins_test, tolerance=self.tolerance):
-            n_bins_test += 1
-        n_bins_test = int(n_bins_test)
-        if n_bins != n_bins_test:
-            raise ValueError(
-                "Inconsistent arguments t_start (%s), " % t_start +
-                "t_stop (%s), bin_size (%s) " % (t_stop, bin_size) +
-                "and n_bins (%d)" % n_bins)
-        if n_bins - int(n_bins) != 0 or n_bins < 0:
-            raise TypeError(
-                "Number of bins ({}) is not an integer or < 0".format(n_bins))
+        check_consistency()
 
     @property
     def bin_edges(self):
         """
         Returns all time edges as a quantity array with :attr:`n_bins` bins.
 
         The borders of all time steps between :attr:`t_start` and
@@ -683,19 +527,18 @@
 
         Returns
         -------
         bin_edges : pq.Quantity
             All edges in interval [:attr:`t_start`, :attr:`t_stop`] with
             :attr:`n_bins` bins are returned as a quantity array.
         """
-        t_start = self.t_start.rescale(self.bin_size.units).magnitude
-        bin_edges = np.linspace(t_start, t_start + self.n_bins *
-                                self.bin_size.magnitude,
+        bin_edges = np.linspace(self._t_start, self._t_start + self.n_bins *
+                                self._bin_size,
                                 num=self.n_bins + 1, endpoint=True)
-        return pq.Quantity(bin_edges, units=self.bin_size.units)
+        return pq.Quantity(bin_edges, units=self.units, copy=False)
 
     @property
     def bin_centers(self):
         """
         Returns each center time point of all bins between :attr:`t_start` and
         :attr:`t_stop` points.
 
@@ -703,15 +546,21 @@
 
         Returns
         -------
         bin_edges : pq.Quantity
             All center edges in interval (:attr:`start`, :attr:`stop`).
 
         """
-        return self.bin_edges[:-1] + self.bin_size / 2
+        start = self._t_start + self._bin_size / 2
+        stop = start + (self.n_bins - 1) * self._bin_size
+        bin_centers = np.linspace(start=start,
+                                  stop=stop,
+                                  num=self.n_bins, endpoint=True)
+        bin_centers = pq.Quantity(bin_centers, units=self.units, copy=False)
+        return bin_centers
 
     def to_sparse_array(self):
         """
         Getter for sparse matrix with time points.
 
         Returns
         -------
@@ -720,15 +569,18 @@
 
         See also
         --------
         scipy.sparse.csr_matrix
         to_array
 
         """
-        return self._sparse_mat_u
+        warnings.warn("'.to_sparse_array()' function is deprecated; "
+                      "use '.sparse_matrix' attribute directly",
+                      DeprecationWarning)
+        return self.sparse_matrix
 
     def to_sparse_bool_array(self):
         """
         Getter for boolean version of the sparse matrix, calculated from
         sparse matrix with counted time points.
 
         Returns
@@ -739,17 +591,17 @@
         See also
         --------
         scipy.sparse.csr_matrix
         to_bool_array
 
         """
         # Return sparse Matrix as a copy
-        tmp_mat = self._sparse_mat_u.copy()
-        tmp_mat[tmp_mat.nonzero()] = 1
-        return tmp_mat.astype(bool)
+        spmat_copy = self.sparse_matrix.copy()
+        spmat_copy.data = spmat_copy.data.astype(bool)
+        return spmat_copy
 
     def get_num_of_spikes(self, axis=None):
         """
         Compute the number of binned spikes.
 
         Parameters
         ----------
@@ -762,17 +614,17 @@
         Returns
         -------
         n_spikes_per_row : int or np.ndarray
             The number of binned spikes.
 
         """
         if axis is None:
-            return self._sparse_mat_u.sum(axis=axis)
-        n_spikes_per_row = self._sparse_mat_u.sum(axis=axis)
-        n_spikes_per_row = np.asarray(n_spikes_per_row)[:, 0]
+            return self.sparse_matrix.sum(axis=axis)
+        n_spikes_per_row = self.sparse_matrix.sum(axis=axis)
+        n_spikes_per_row = np.ravel(n_spikes_per_row)
         return n_spikes_per_row
 
     @property
     def spike_indices(self):
         """
         A list of lists for each spike train (i.e., rows of the binned matrix),
         that in turn contains for each spike the index into the binned matrix
@@ -788,22 +640,22 @@
         >>> import quantities as pq
         >>> st = n.SpikeTrain([0.5, 0.7, 1.2, 3.1, 4.3, 5.5, 6.7] * pq.s,
         ...                   t_stop=10.0 * pq.s)
         >>> x = conv.BinnedSpikeTrain(st, n_bins=10, bin_size=1 * pq.s,
         ...                           t_start=0 * pq.s)
         >>> print(x.spike_indices)
         [[0, 0, 1, 3, 4, 5, 6]]
-        >>> print(x.to_sparse_array().nonzero()[1])
+        >>> print(x.sparse_matrix.nonzero()[1])
         [0 1 3 4 5 6]
         >>> print(x.to_array())
         [[2, 1, 0, 1, 1, 1, 1, 0, 0, 0]]
 
         """
         spike_idx = []
-        for row in self._sparse_mat_u:
+        for row in self.sparse_matrix:
             # Extract each non-zeros column index and how often it exists,
             # i.e., how many spikes fall in this column
             n_cols = np.repeat(row.indices, row.data)
             spike_idx.append(n_cols)
         return spike_idx
 
     @property
@@ -816,15 +668,15 @@
 
         Returns
         -------
         bool
             True for binary input, False otherwise.
         """
 
-        return is_binary(self.input_spiketrains)
+        return is_binary(self.sparse_matrix.data)
 
     def to_bool_array(self):
         """
         Returns a matrix, in which the rows correspond to the spike trains and
         the columns correspond to the bins in the `BinnedSpikeTrain`.
         `True` indicates a spike in given bin of given spike train and
         `False` indicates lack of spikes.
@@ -851,25 +703,23 @@
         ...                  t_stop=10.0 * pq.s)
         >>> x = conv.BinnedSpikeTrain(a, n_bins=10, bin_size=1 * pq.s,
         ...                           t_start=0 * pq.s)
         >>> print(x.to_bool_array())
         [[ True  True False  True  True  True  True False False False]]
 
         """
-        return self.to_array().astype(bool)
+        return self.to_array(dtype=bool)
 
-    def to_array(self, store_array=False):
+    def to_array(self, dtype=None):
         """
         Returns a dense matrix, calculated from the sparse matrix, with counted
         time points of spikes. The rows correspond to spike trains and the
         columns correspond to bins in a `BinnedSpikeTrain`.
         Entries contain the count of spikes that occurred in the given bin of
         the given spike train.
-        If the boolean :attr:`store_array` is set to `True`, the matrix
-        will be stored in memory.
 
         Returns
         -------
         matrix : np.ndarray
             Matrix with spike counts. Columns represent the index positions of
             the binned spikes and rows represent the spike trains.
 
@@ -887,130 +737,140 @@
 
         See also
         --------
         scipy.sparse.csr_matrix
         scipy.sparse.csr_matrix.toarray
 
         """
-        if self._mat_u is not None:
-            return self._mat_u
-        if store_array:
-            self._store_array()
-            return self._mat_u
-        # Matrix on demand
-        else:
-            return self._sparse_mat_u.toarray()
-
-    def _store_array(self):
-        """
-        Stores the matrix with counted time points in memory.
-
-        """
-        if self._mat_u is None:
-            self._mat_u = self._sparse_mat_u.toarray()
-
-    def remove_stored_array(self):
-        """
-        Unlinks the matrix with counted time points from memory.
-        """
-        self._mat_u = None
+        spmat = self.sparse_matrix
+        if dtype is not None and dtype != spmat.data.dtype:
+            # avoid a copy
+            spmat = sps.csr_matrix(
+                (spmat.data.astype(dtype), spmat.indices, spmat.indptr),
+                shape=spmat.shape)
+        return spmat.toarray()
 
-    def binarize(self, copy=True):
+    def binarize(self, copy=None):
         """
         Clip the internal array (no. of spikes in a bin) to `0` (no spikes) or
         `1` (at least one spike) values only.
 
         Parameters
         ----------
-        copy : bool
-            Perform the clipping in-place (False) or on a copy (True).
-            Default: True.
+        copy : bool, optional
+            Deprecated parameter. It has no effect.
 
         Returns
         -------
-        bst : BinnedSpikeTrain
-            `BinnedSpikeTrain` with both sparse and dense (if present) array
-            representation clipped to `0` (no spike) or `1` (at least one
-            spike) entries.
-
-        """
-        if copy:
-            bst = deepcopy(self)
-        else:
-            bst = self
-        bst._sparse_mat_u.data.clip(max=1, out=bst._sparse_mat_u.data)
-        if bst._mat_u is not None:
-            bst._mat_u.clip(max=1, out=bst._mat_u)
+        bst : _BinnedSpikeTrainView
+            A view of `BinnedSpikeTrain` with a sparse matrix containing
+            data clipped to `0`s and `1`s.
+
+        """
+        if copy is not None:
+            warnings.warn("'copy' parameter is deprecated - a view is always "
+                          "returned; set this parameter to None.",
+                          DeprecationWarning)
+        spmat = self.sparse_matrix
+        spmat = sps.csr_matrix(
+            (spmat.data.clip(max=1), spmat.indices, spmat.indptr),
+            shape=spmat.shape, copy=False)
+        bst = _BinnedSpikeTrainView(t_start=self._t_start,
+                                    t_stop=self._t_stop,
+                                    bin_size=self._bin_size,
+                                    units=self.units,
+                                    sparse_matrix=spmat)
         return bst
 
     @property
     def sparsity(self):
         """
         Returns
         -------
         float
             Matrix sparsity defined as no. of nonzero elements divided by
             the matrix size
         """
-        num_nonzero = self._sparse_mat_u.data.shape[0]
-        return num_nonzero / np.prod(self._sparse_mat_u.shape)
+        num_nonzero = self.sparse_matrix.data.shape[0]
+        return num_nonzero / np.prod(self.sparse_matrix.shape)
 
-    def _convert_to_binned(self, spiketrains):
+    def _create_sparse_matrix(self, spiketrains, tolerance):
         """
         Converts `neo.SpikeTrain` objects to a sparse matrix
         (`scipy.sparse.csr_matrix`), which contains the binned spike times, and
         stores it in :attr:`_sparse_mat_u`.
 
         Parameters
         ----------
         spiketrains : neo.SpikeTrain or list of neo.SpikeTrain
             Spike trains to bin.
 
         """
-        if not self.is_spiketrain:
-            self._sparse_mat_u = sps.csr_matrix(spiketrains, dtype=int)
-            return
+        if not _check_neo_spiketrain(spiketrains):
+            # a binned numpy array
+            sparse_matrix = sps.csr_matrix(spiketrains, dtype=np.int32)
+            return sparse_matrix
 
         row_ids, column_ids = [], []
         # data
         counts = []
+        n_discarded = 0
 
+        # all spiketrains carry the same units
+        scale_units = 1 / self._bin_size
         for idx, st in enumerate(spiketrains):
-            times = (st.times - self.t_start).rescale(self.bin_size.units)
-            scale = np.array((times / self.bin_size).magnitude)
+            times = st.magnitude
+            times = times[(times >= self._t_start) & (
+                    times <= self._t_stop)] - self._t_start
+            bins = times * scale_units
 
             # shift spikes that are very close
             # to the right edge into the next bin
-            rounding_error_indices = _detect_rounding_errors(scale,
-                                                             self.tolerance)
+            rounding_error_indices = _detect_rounding_errors(
+                bins, tolerance=tolerance)
             num_rounding_corrections = rounding_error_indices.sum()
             if num_rounding_corrections > 0:
                 warnings.warn('Correcting {} rounding errors by shifting '
                               'the affected spikes into the following bin. '
                               'You can set tolerance=None to disable this '
                               'behaviour.'.format(num_rounding_corrections))
-            scale[rounding_error_indices] += .5
+            bins[rounding_error_indices] += .5
 
-            scale = scale.astype(int)
-
-            la = np.logical_and(times >= 0 * self.bin_size.units,
-                                times <= (self.t_stop
-                                          - self.t_start).rescale(
-                                              self.bin_size.units))
-            filled_tmp = scale[la]
-            filled_tmp = filled_tmp[filled_tmp < self.n_bins]
-            f, c = np.unique(filled_tmp, return_counts=True)
-            column_ids.extend(f)
-            counts.extend(c)
-            row_ids.extend([idx] * len(f))
-        csr_matrix = sps.csr_matrix((counts, (row_ids, column_ids)),
-                                    shape=(len(spiketrains),
-                                           self.n_bins),
-                                    dtype=int)
-        self._sparse_mat_u = csr_matrix
+            bins = bins.astype(np.int32)
+            valid_bins = bins[bins < self.n_bins]
+            n_discarded += len(bins) - len(valid_bins)
+            f, c = np.unique(valid_bins, return_counts=True)
+            column_ids.append(f)
+            counts.append(c)
+            row_ids.append(np.repeat(idx, repeats=len(f)))
+
+        if n_discarded > 0:
+            warnings.warn("Binning discarded {} last spike(s) of the "
+                          "input spiketrain".format(n_discarded))
+
+        counts = np.hstack(counts)
+        row_ids = np.hstack(row_ids)
+        column_ids = np.hstack(column_ids)
+
+        sparse_matrix = sps.csr_matrix((counts, (row_ids, column_ids)),
+                                       shape=(len(spiketrains), self.n_bins),
+                                       dtype=np.int32, copy=False)
+        return sparse_matrix
+
+
+class _BinnedSpikeTrainView(BinnedSpikeTrain):
+    # Experimental feature and should not be public now.
+
+    def __init__(self, t_start, t_stop, bin_size, units, sparse_matrix):
+        self._t_start = t_start
+        self._t_stop = t_stop
+        self._bin_size = bin_size
+        self.n_bins = sparse_matrix.shape[1]
+        self.units = units
+        self.sparse_matrix = sparse_matrix
 
 
 def _check_neo_spiketrain(matrix):
     """
     Checks if given input contains neo.SpikeTrain objects
 
     Parameters
@@ -1028,41 +888,7 @@
     # Check for single spike train
     if isinstance(matrix, neo.SpikeTrain):
         return True
     # Check for list or tuple
     if isinstance(matrix, (list, tuple)):
         return all(map(_check_neo_spiketrain, matrix))
     return False
-
-
-def _check_binned_array(matrix):
-    """
-    Checks if given input is a binned array
-
-    Parameters
-    ----------
-    matrix
-        Object to test
-
-    Returns
-    -------
-    bool
-        True if `matrix` is an 2D array-like object,
-        otherwise False.
-
-    Raises
-    ------
-    TypeError
-        If `matrix` is not 2-dimensional.
-
-    """
-    matrix = np.asarray(matrix)
-    # Check for proper dimension MxN
-    if matrix.ndim == 2:
-        return True
-    elif matrix.dtype == np.dtype('O'):
-        raise TypeError('Please check the dimensions of the input, '
-                        'it should be an MxN array, '
-                        'the input has the shape: {}'.format(matrix.shape))
-    else:
-        # Otherwise not supported
-        raise TypeError('Input not supported. Please check again')
```

### Comparing `elephant-0.8.0/elephant/cubic.py` & `elephant-0.9.0/elephant/cubic.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,18 @@
 import scipy.stats
 import scipy.special
 import math
 import warnings
 
 from elephant.utils import deprecated_alias
 
+__all__ = [
+    "cubic"
+]
+
 
 # Based on matlab code by Benjamin Staude
 # Adaptation to python by Pietro Quaglio and Emiliano Torre
 
 
 @deprecated_alias(data='histogram', ximax='max_iterations')
 def cubic(histogram, max_iterations=100, alpha=0.05):
```

### Comparing `elephant-0.8.0/elephant/current_source_density.py` & `elephant-0.9.0/elephant/current_source_density.py`

 * *Files 8% similar despite different names*

```diff
@@ -39,18 +39,22 @@
 
 import neo
 import numpy as np
 import quantities as pq
 from scipy.integrate import simps
 
 import elephant.current_source_density_src.utility_functions as utils
-from elephant.current_source_density_src import KCSD
-from elephant.current_source_density_src import icsd
+from elephant.current_source_density_src import KCSD, icsd
 from elephant.utils import deprecated_alias
 
+__all__ = [
+    "estimate_csd",
+    "generate_lfp"
+]
+
 utils.patch_quantities()
 
 available_1d = ['StandardCSD', 'DeltaiCSD', 'StepiCSD', 'SplineiCSD', 'KCSD1D']
 available_2d = ['KCSD2D', 'MoIKCSD']
 available_3d = ['KCSD3D']
 
 kernel_methods = ['KCSD1D', 'KCSD2D', 'KCSD3D', 'MoIKCSD']
@@ -247,98 +251,90 @@
 
     Returns
     -------
     LFP : neo.AnalogSignal
        The potentials created by the csd profile at the electrode positions.
        The electrode positions are attached as RecordingChannel's coordinate.
     """
+
     def integrate_1D(x0, csd_x, csd, h):
-        m = np.sqrt((csd_x - x0)**2 + h**2) - abs(csd_x - x0)
+        m = np.sqrt((csd_x - x0) ** 2 + h ** 2) - abs(csd_x - x0)
         y = csd * m
         I = simps(y, csd_x)
         return I
 
     def integrate_2D(x, y, xlin, ylin, csd, h, X, Y):
-        Ny = ylin.shape[0]
-        m = np.sqrt((x - X)**2 + (y - Y)**2)
-        m[m < 0.0000001] = 0.0000001
+        x = np.reshape(x, (1, 1, len(x)))
+        y = np.reshape(y, (1, 1, len(y)))
+        X = np.expand_dims(X, axis=2)
+        Y = np.expand_dims(Y, axis=2)
+        csd = np.expand_dims(csd, axis=2)
+        m = np.sqrt((x - X) ** 2 + (y - Y) ** 2)
+        np.clip(m, a_min=0.0000001, a_max=None, out=m)
         y = np.arcsinh(2 * h / m) * csd
-        I = np.zeros(Ny)
-        for i in range(Ny):
-            I[i] = simps(y[:, i], ylin)
+        I = simps(y.T, ylin)
         F = simps(I, xlin)
         return F
 
-    def integrate_3D(x, y, z, xlim, ylim, zlim, csd, xlin, ylin, zlin,
-                     X, Y, Z):
-        Nz = zlin.shape[0]
-        Ny = ylin.shape[0]
-        m = np.sqrt((x - X)**2 + (y - Y)**2 + (z - Z)**2)
-        m[m < 0.0000001] = 0.0000001
+    def integrate_3D(x, y, z, csd, xlin, ylin, zlin, X, Y, Z):
+        m = np.sqrt((x - X) ** 2 + (y - Y) ** 2 + (z - Z) ** 2)
+        np.clip(m, a_min=0.0000001, a_max=None, out=m)
         z = csd / m
-        Iy = np.zeros(Ny)
-        for j in range(Ny):
-            Iz = np.zeros(Nz)
-            for i in range(Nz):
-                Iz[i] = simps(z[:, j, i], zlin)
-            Iy[j] = simps(Iz, ylin)
+        Iy = simps(np.transpose(z, (1, 0, 2)), zlin)
+        Iy = simps(Iy, ylin)
         F = simps(Iy, xlin)
         return F
+
     dim = 1
     if z_positions is not None:
         dim = 3
     elif y_positions is not None:
         dim = 2
+
     x = np.linspace(x_limits[0], x_limits[1], resolution)
-    if dim >= 2:
-        y = np.linspace(y_limits[0], y_limits[1], resolution)
-    if dim == 3:
-        z = np.linspace(z_limits[0], z_limits[1], resolution)
     sigma = 1.0
     h = 50.
-    pots = np.zeros(len(x_positions))
     if dim == 1:
-        chrg_x = np.linspace(x_limits[0], x_limits[1], resolution)
+        chrg_x = x
         csd = csd_profile(chrg_x)
-        for ii in range(len(x_positions)):
-            pots[ii] = integrate_1D(x_positions[ii], chrg_x, csd, h)
+        pots = integrate_1D(x_positions, chrg_x, csd, h)
         pots /= 2. * sigma  # eq.: 26 from Potworowski et al
         ele_pos = x_positions
     elif dim == 2:
-        chrg_x, chrg_y = np.mgrid[
-                         x_limits[0]:x_limits[1]:np.complex(0, resolution),
-                         y_limits[0]:y_limits[1]:np.complex(0, resolution)]
+        y = np.linspace(y_limits[0], y_limits[1], resolution)
+        chrg_x = np.expand_dims(x, axis=1)
+        chrg_y = np.expand_dims(y, axis=0)
         csd = csd_profile(chrg_x, chrg_y)
-        for ii in range(len(x_positions)):
-            pots[ii] = integrate_2D(x_positions[ii], y_positions[ii],
-                                    x, y, csd, h, chrg_x, chrg_y)
+        pots = integrate_2D(x_positions, y_positions,
+                            x, y,
+                            csd, h,
+                            chrg_x, chrg_y)
         pots /= 2 * np.pi * sigma
         ele_pos = np.vstack((x_positions, y_positions)).T
     elif dim == 3:
+        y = np.linspace(y_limits[0], y_limits[1], resolution)
+        z = np.linspace(z_limits[0], z_limits[1], resolution)
         chrg_x, chrg_y, chrg_z = np.mgrid[
-            x_limits[0]:x_limits[1]:np.complex(0, resolution),
-            y_limits[0]:y_limits[1]:np.complex(0, resolution),
-            z_limits[0]:z_limits[1]:np.complex(0, resolution)
+            x_limits[0]: x_limits[1]: np.complex(0, resolution),
+            y_limits[0]: y_limits[1]: np.complex(0, resolution),
+            z_limits[0]: z_limits[1]: np.complex(0, resolution)
         ]
+
         csd = csd_profile(chrg_x, chrg_y, chrg_z)
-        xlin = chrg_x[:, 0, 0]
-        ylin = chrg_y[0, :, 0]
-        zlin = chrg_z[0, 0, :]
+
+        pots = np.zeros(len(x_positions))
         for ii in range(len(x_positions)):
             pots[ii] = integrate_3D(x_positions[ii], y_positions[ii],
                                     z_positions[ii],
-                                    x_limits, y_limits, z_limits, csd,
-                                    xlin, ylin, zlin,
+                                    csd,
+                                    x, y, z,
                                     chrg_x, chrg_y, chrg_z)
         pots /= 4 * np.pi * sigma
         ele_pos = np.vstack((x_positions, y_positions, z_positions)).T
-    pots = np.reshape(pots, (-1, 1)) * pq.mV
     ele_pos = ele_pos * pq.mm
-    lfp = []
     ch = neo.ChannelIndex(index=range(len(pots)))
-    for ii in range(len(pots)):
-        lfp.append(pots[ii])
-    asig = neo.AnalogSignal(np.array(lfp).T, sampling_rate=pq.kHz, units='mV')
+    asig = neo.AnalogSignal(np.expand_dims(pots, axis=0),
+                            sampling_rate=pq.kHz, units='mV')
     ch.coordinates = ele_pos
     ch.analogsignals.append(asig)
     ch.create_relationship()
     return asig
```

### Comparing `elephant-0.8.0/elephant/current_source_density_src/KCSD.py` & `elephant-0.9.0/elephant/current_source_density_src/KCSD.py`

 * *Files identical despite different names*

### Comparing `elephant-0.8.0/elephant/current_source_density_src/README.md` & `elephant-0.9.0/elephant/current_source_density_src/README.md`

 * *Files identical despite different names*

### Comparing `elephant-0.8.0/elephant/current_source_density_src/basis_functions.py` & `elephant-0.9.0/elephant/current_source_density_src/basis_functions.py`

 * *Files identical despite different names*

### Comparing `elephant-0.8.0/elephant/current_source_density_src/icsd.py` & `elephant-0.9.0/elephant/current_source_density_src/icsd.py`

 * *Files identical despite different names*

### Comparing `elephant-0.8.0/elephant/current_source_density_src/test_data.mat` & `elephant-0.9.0/elephant/current_source_density_src/test_data.mat`

 * *Files identical despite different names*

### Comparing `elephant-0.8.0/elephant/current_source_density_src/utility_functions.py` & `elephant-0.9.0/elephant/current_source_density_src/utility_functions.py`

 * *Files identical despite different names*

### Comparing `elephant-0.8.0/elephant/gpfa/gpfa.py` & `elephant-0.9.0/elephant/gpfa/gpfa.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 Gaussian-process factor analysis (GPFA) is a dimensionality reduction method
-[#f1]_ for neural trajectory visualization of parallel spike trains. GPFA applies
-factor analysis (FA) to time-binned spike count data to reduce the
+[#f1]_ for neural trajectory visualization of parallel spike trains. GPFA
+applies factor analysis (FA) to time-binned spike count data to reduce the
 dimensionality and at the same time smoothes the resulting low-dimensional
 trajectories by fitting a Gaussian process (GP) model to them.
 
 The input consists of a set of trials (Y), each containing a list of spike
 trains (N neurons). The output is the projection (X) of the data in a space
 of pre-chosen dimensionality x_dim < N.
 
@@ -29,14 +29,39 @@
 
 2) projection of single trials in the low dimensional space (c.f.,
 `gpfa_core.exact_inference_with_ll()`)
 
 3) orthonormalization of the matrix C and the corresponding subspace, for
 visualization purposes: (c.f., `gpfa_core.orthonormalize()`)
 
+
+.. autosummary::
+    :toctree: toctree/gpfa
+
+    GPFA
+
+
+Visualization
+-------------
+Visualization of GPFA transforms is covered in Viziphant:
+https://viziphant.readthedocs.io/en/latest/modules.html
+
+
+Tutorial
+--------
+
+:doc:`View tutorial <../tutorials/gpfa>`
+
+Run tutorial interactively:
+
+.. image:: https://mybinder.org/badge.svg
+   :target: https://mybinder.org/v2/gh/NeuralEnsemble/elephant/master
+            ?filepath=doc/tutorials/gpfa.ipynb
+
+
 References
 ----------
 The code was ported from the MATLAB code based on Byron Yu's implementation.
 The original MATLAB code is available at Byron Yu's website:
 https://users.ece.cmu.edu/~byronyu/software.shtml
 
 .. [#f1] Yu MB, Cunningham JP, Santhanam G, Ryu SI, Shenoy K V, Sahani M (2009)
@@ -55,14 +80,19 @@
 import sklearn
 import warnings
 
 from elephant.gpfa import gpfa_core, gpfa_util
 from elephant.utils import deprecated_alias
 
 
+__all__ = [
+    "GPFA"
+]
+
+
 class GPFA(sklearn.base.BaseEstimator):
     """
     Apply Gaussian process factor analysis (GPFA) to spike train data
 
     There are two principle scenarios of using the GPFA analysis, both of which
     can be performed in an instance of the GPFA() class.
 
@@ -194,36 +224,44 @@
     ...                                      size=n_channels) * pq.Hz
     >>>     spike_times = [homogeneous_poisson_process(rate=rate)
     ...                    for rate in firing_rates]
     >>>     data.append((trial, spike_times))
     ...
     >>> gpfa = GPFA(bin_size=20*pq.ms, x_dim=8)
     >>> gpfa.fit(data)
-    >>> results = gpfa.transform(data, returned_data=['xorth', 'xsm'])
-    >>> xorth = results['xorth']; xsm = results['xsm']
+    >>> results = gpfa.transform(data, returned_data=['latent_variable_orth',
+    ...                                               'latent_variable'])
+    >>> latent_variable_orth = results['latent_variable_orth']
+    >>> latent_variable = results['latent_variable']
 
     or simply
 
     >>> results = GPFA(bin_size=20*pq.ms, x_dim=8).fit_transform(data,
-    ...                returned_data=['xorth', 'xsm'])
+    ...                returned_data=['latent_variable_orth',
+    ...                               'latent_variable'])
     """
 
     @deprecated_alias(binsize='bin_size')
     def __init__(self, bin_size=20 * pq.ms, x_dim=3, min_var_frac=0.01,
                  tau_init=100.0 * pq.ms, eps_init=1.0E-3, em_tol=1.0E-8,
                  em_max_iters=500, freq_ll=5, verbose=False):
         self.bin_size = bin_size
         self.x_dim = x_dim
         self.min_var_frac = min_var_frac
         self.tau_init = tau_init
         self.eps_init = eps_init
         self.em_tol = em_tol
         self.em_max_iters = em_max_iters
         self.freq_ll = freq_ll
-        self.valid_data_names = ('xorth', 'xsm', 'Vsm', 'VsmGP', 'y')
+        self.valid_data_names = (
+            'latent_variable_orth',
+            'latent_variable',
+            'Vsm',
+            'VsmGP',
+            'y')
         self.verbose = verbose
 
         if not isinstance(self.bin_size, pq.Quantity):
             raise ValueError("'bin_size' must be of type pq.Quantity")
         if not isinstance(self.tau_init, pq.Quantity):
             raise ValueError("'tau_init' must be of type pq.Quantity")
 
@@ -313,15 +351,15 @@
         seqs = gpfa_util.get_seqs(spiketrains, self.bin_size)
         # Remove inactive units based on training set
         self.has_spikes_bool = np.hstack(seqs['y']).any(axis=1)
         for seq in seqs:
             seq['y'] = seq['y'][self.has_spikes_bool, :]
         return seqs
 
-    def transform(self, spiketrains, returned_data=['xorth']):
+    def transform(self, spiketrains, returned_data=['latent_variable_orth']):
         """
         Obtain trajectories of neural activity in a low-dimensional latent
         variable space by inferring the posterior mean of the obtained GPFA
         model and applying an orthonormalization on the latent variable space.
 
         Parameters
         ----------
@@ -334,46 +372,47 @@
             trial must be fixed such that `spiketrains[l][n]` and
             `spiketrains[k][n]` refer to spike trains of the same neuron
             for any choices of `l`, `k`, and `n`.
         returned_data : list of str
             The dimensionality reduction transform generates the following
             resultant data:
 
-               'xorth': orthonormalized posterior mean of latent variable
+               'latent_variable_orth': orthonormalized posterior mean of latent
+               variable
 
-               'xsm': posterior mean of latent variable before
+               'latent_variable': posterior mean of latent variable before
                orthonormalization
 
                'Vsm': posterior covariance between latent variables
 
                'VsmGP': posterior covariance over time for each latent variable
 
                'y': neural data used to estimate the GPFA model parameters
 
             `returned_data` specifies the keys by which the data dict is
             returned.
 
-            Default is ['xorth'].
+            Default is ['latent_variable_orth'].
 
         Returns
         -------
         np.ndarray or dict
             When the length of `returned_data` is one, a single np.ndarray,
             containing the requested data (the first entry in `returned_data`
             keys list), is returned. Otherwise, a dict of multiple np.ndarrays
             with the keys identical to the data names in `returned_data` is
             returned.
 
             N-th entry of each np.ndarray is a np.ndarray of the following
             shape, specific to each data type, containing the corresponding
             data for the n-th trial:
 
-                `xorth`: (#latent_vars, #bins) np.ndarray
+                `latent_variable_orth`: (#latent_vars, #bins) np.ndarray
 
-                `xsm`:  (#latent_vars, #bins) np.ndarray
+                `latent_variable`:  (#latent_vars, #bins) np.ndarray
 
                 `y`:  (#units, #bins) np.ndarray
 
                 `Vsm`:  (#latent_vars, #latent_vars, #bins) np.ndarray
 
                 `VsmGP`:  (#bins, #bins, #latent_vars) np.ndarray
 
@@ -406,15 +445,16 @@
         self.transform_info['num_bins'] = seqs['T']
         Corth, seqs = gpfa_core.orthonormalize(self.params_estimated, seqs)
         self.transform_info['Corth'] = Corth
         if len(returned_data) == 1:
             return seqs[returned_data[0]]
         return {x: seqs[x] for x in returned_data}
 
-    def fit_transform(self, spiketrains, returned_data=['xorth']):
+    def fit_transform(self, spiketrains, returned_data=[
+                      'latent_variable_orth']):
         """
         Fit the model with `spiketrains` data and apply the dimensionality
         reduction on `spiketrains`.
 
         Parameters
         ----------
         spiketrains : list of list of neo.SpikeTrain
```

### Comparing `elephant-0.8.0/elephant/gpfa/gpfa_core.py` & `elephant-0.9.0/elephant/gpfa/gpfa_core.py`

 * *Files 4% similar despite different names*

```diff
@@ -199,15 +199,15 @@
     -------
     params_est : dict
         GPFA model parameter estimates, returned by EM algorithm (same
         format as params_init)
     seqs_latent : np.recarray
         a copy of the training data structure, augmented with the new
         fields:
-        xsm : np.ndarray of shape (#latent_vars x #bins)
+        latent_variable : np.ndarray of shape (#latent_vars x #bins)
             posterior mean of latent variables at each time bin
         Vsm : np.ndarray of shape (#latent_vars, #latent_vars, #bins)
             posterior covariance between latent variables at each
             timepoint
         VsmGP : np.ndarray of shape (#bins, #bins, #latent_vars)
             posterior covariance over time for each latent
             variable
@@ -240,34 +240,35 @@
                                                   get_ll=get_ll)
         lls.append(ll)
 
         # ==== M STEP ====
         sum_p_auto = np.zeros((x_dim, x_dim))
         for seq_latent in seqs_latent:
             sum_p_auto += seq_latent['Vsm'].sum(axis=2) \
-                + seq_latent['xsm'].dot(seq_latent['xsm'].T)
+                + seq_latent['latent_variable'].dot(
+                seq_latent['latent_variable'].T)
         y = np.hstack(seqs_train['y'])
-        xsm = np.hstack(seqs_latent['xsm'])
-        sum_yxtrans = y.dot(xsm.T)
-        sum_xall = xsm.sum(axis=1)[:, np.newaxis]
+        latent_variable = np.hstack(seqs_latent['latent_variable'])
+        sum_yxtrans = y.dot(latent_variable.T)
+        sum_xall = latent_variable.sum(axis=1)[:, np.newaxis]
         sum_yall = y.sum(axis=1)[:, np.newaxis]
 
         # term is (xDim+1) x (xDim+1)
         term = np.vstack([np.hstack([sum_p_auto, sum_xall]),
                           np.hstack([sum_xall.T, t.sum().reshape((1, 1))])])
         # yDim x (xDim+1)
         cd = gpfa_util.rdiv(np.hstack([sum_yxtrans, sum_yall]), term)
 
         params['C'] = cd[:, :x_dim]
         params['d'] = cd[:, -1]
 
         # yCent must be based on the new d
         # yCent = bsxfun(@minus, [seq.y], currentParams.d);
-        # R = (yCent * yCent' - (yCent * [seq.xsm]') * currentParams.C')
-        #     / sum(T);
+        # R = (yCent * yCent' - (yCent * [seq.latent_variable]') * \
+        #     currentParams.C') / sum(T);
         c = params['C']
         d = params['d'][:, np.newaxis]
         if params['notes']['RforceDiagonal']:
             sum_yytrans = (y * y).sum(axis=1)[:, np.newaxis]
             yd = sum_yall * d
             term = ((sum_yxtrans - d.dot(sum_xall.T)) * c).sum(axis=1)
             term = term[:, np.newaxis]
@@ -340,30 +341,30 @@
           specifies whether to compute data log likelihood (default: True)
 
     Returns
     -------
     seqs_latent : np.recarray
         a copy of the input data structure, augmented with the new
         fields:
-        xsm :  (#latent_vars, #bins) np.ndarray
+        latent_variable :  (#latent_vars, #bins) np.ndarray
               posterior mean of latent variables at each time bin
         Vsm :  (#latent_vars, #latent_vars, #bins) np.ndarray
               posterior covariance between latent variables at each
               timepoint
         VsmGP :  (#bins, #bins, #latent_vars) np.ndarray
                 posterior covariance over time for each latent
                 variable
     ll : float
         data log likelihood, np.nan is returned when `get_ll` is set False
     """
     y_dim, x_dim = params['C'].shape
 
     # copy the contents of the input data structure to output structure
     dtype_out = [(x, seqs[x].dtype) for x in seqs.dtype.names]
-    dtype_out.extend([('xsm', np.object), ('Vsm', np.object),
+    dtype_out.extend([('latent_variable', np.object), ('Vsm', np.object),
                       ('VsmGP', np.object)])
     seqs_latent = np.empty(len(seqs), dtype=dtype_out)
     for dtype_name in seqs.dtype.names:
         seqs_latent[dtype_name] = seqs[dtype_name]
 
     # Precomputations
     if params['notes']['RforceDiagonal']:
@@ -420,20 +421,21 @@
         idx = range(0, x_dim * t_half + 1, x_dim)
         for i in range(t_half):
             blk_prod[idx[i]:idx[i + 1], :] = c_rinv_c.dot(
                 minv[idx[i]:idx[i + 1], :])
         blk_prod = k_big[:x_dim * t_half, :].dot(
             gpfa_util.fill_persymm(np.eye(x_dim * t_half, x_dim * t) -
                                    blk_prod, x_dim, t))
-        # xsmMat is (xDim*T) x length(nList)
-        xsm_mat = gpfa_util.fill_persymm(blk_prod, x_dim, t).dot(term1_mat)
+        # latent_variableMat is (xDim*T) x length(nList)
+        latent_variable_mat = gpfa_util.fill_persymm(
+            blk_prod, x_dim, t).dot(term1_mat)
 
         for i, n in enumerate(n_list):
-            seqs_latent[n]['xsm'] = xsm_mat[:, i].reshape((x_dim, t),
-                                                          order='F')
+            seqs_latent[n]['latent_variable'] = \
+                latent_variable_mat[:, i].reshape((x_dim, t), order='F')
             seqs_latent[n]['Vsm'] = vsm
             seqs_latent[n]['VsmGP'] = vsm_gp
 
         if get_ll:
             # Compute data likelihood
             val = -t * logdet_r - logdet_k_big - logdet_m \
                   - y_dim * t * np.log(2 * np.pi)
@@ -532,32 +534,33 @@
         space.
         Data structure, whose n-th entry (corresponding to the n-th
         experimental trial) has fields
         T : int
           number of timesteps
         y : np.ndarray of shape (#units, #bins)
           neural data
-        xsm : np.ndarray of shape (#latent_vars, #bins)
+        latent_variable : np.ndarray of shape (#latent_vars, #bins)
           posterior mean of latent variables at each time bin
         Vsm : np.ndarray of shape (#latent_vars, #latent_vars, #bins)
           posterior covariance between latent variables at each
           timepoint
         VsmGP : np.ndarray of shape (#bins, #bins, #latent_vars)
           posterior covariance over time for each latent variable
 
     Returns
     -------
     params_est : dict
         Estimated model parameters, including `Corth`, obtained by
         orthonormalizing the columns of C.
     seqs : np.recarray
-        Training data structure that contains the new field `xorth`,
-        the orthonormalized neural trajectories.
+        Training data structure that contains the new field
+        `latent_variable_orth`, the orthonormalized neural trajectories.
     """
     C = params_est['C']
-    X = np.hstack(seqs['xsm'])
-    Xorth, Corth, _ = gpfa_util.orthonormalize(X, C)
-    seqs = gpfa_util.segment_by_trial(seqs, Xorth, 'xorth')
+    X = np.hstack(seqs['latent_variable'])
+    latent_variable_orth, Corth, _ = gpfa_util.orthonormalize(X, C)
+    seqs = gpfa_util.segment_by_trial(
+        seqs, latent_variable_orth, 'latent_variable_orth')
 
     params_est['Corth'] = Corth
 
     return Corth, seqs
```

### Comparing `elephant-0.8.0/elephant/gpfa/gpfa_util.py` & `elephant-0.9.0/elephant/gpfa/gpfa_util.py`

 * *Files 2% similar despite different names*

```diff
@@ -419,16 +419,16 @@
     # Loop once for each state dimension (each GP)
     for i in range(xDim):
         # Loop once for each trial length (each of Tu)
         for j in range(len(trial_lengths_num_unique)):
             # Loop once for each trial (each of nList)
             for n in precomp[i]['Tu'][j]['nList']:
                 precomp[i]['Tu'][j]['PautoSUM'] += seqs[n]['VsmGP'][:, :, i] \
-                    + np.outer(
-                    seqs[n]['xsm'][i, :], seqs[n]['xsm'][i, :])
+                    + np.outer(seqs[n]['latent_variable'][i, :],
+                               seqs[n]['latent_variable'][i, :])
     return precomp
 
 
 def grad_betgam(p, pre_comp, const):
     """
     Gradient computation for GP timescale optimization.
     This function is called by minimize.m.
@@ -508,34 +508,34 @@
     x :  (xDim, T) np.ndarray
         Latent variables
     l :  (yDim, xDim) np.ndarray
         Loading matrix
 
     Returns
     -------
-    Xorth : (xDim, T) np.ndarray
+    latent_variable_orth : (xDim, T) np.ndarray
         Orthonormalized latent variables
     Lorth : (yDim, xDim) np.ndarray
         Orthonormalized loading matrix
     TT :  (xDim, xDim) np.ndarray
        Linear transform applied to latent variables
     """
     xDim = l.shape[1]
     if xDim == 1:
         TT = np.sqrt(np.dot(l.T, l))
         Lorth = rdiv(l, TT)
-        Xorth = np.dot(TT, x)
+        latent_variable_orth = np.dot(TT, x)
     else:
         UU, DD, VV = sp.linalg.svd(l, full_matrices=False)
         # TT is transform matrix
         TT = np.dot(np.diag(DD), VV)
 
         Lorth = UU
-        Xorth = np.dot(TT, x)
-    return Xorth, Lorth, TT
+        latent_variable_orth = np.dot(TT, x)
+    return latent_variable_orth, Lorth, TT
 
 
 def segment_by_trial(seqs, x, fn):
     """
     Segment and store data by trial.
 
     Parameters
```

### Comparing `elephant-0.8.0/elephant/kernels.py` & `elephant-0.9.0/elephant/kernels.py`

 * *Files 0% similar despite different names*

```diff
@@ -757,16 +757,16 @@
 
 class ExponentialKernel(Kernel):
     r"""
     Class for exponential kernels.
 
     .. math::
         K(t) = \left\{\begin{array}{ll} (1 / \tau) \exp{(-t / \tau)},
-        & t > 0 \\
-        0, & t \leq 0 \end{array} \right.
+        & t \geq 0 \\
+        0, & t < 0 \end{array} \right.
 
     with :math:`\tau = \sigma`.
 
     Examples
     --------
 
     .. plot::
```

### Comparing `elephant-0.8.0/elephant/neo_tools.py` & `elephant-0.9.0/elephant/neo_tools.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,14 +10,21 @@
 import warnings
 
 from itertools import chain
 
 from neo.core.container import unique_objs
 from elephant.utils import deprecated_alias
 
+__all__ = [
+    "extract_neo_attributes",
+    "get_all_spiketrains",
+    "get_all_events",
+    "get_all_epochs"
+]
+
 
 @deprecated_alias(obj='neo_object')
 def extract_neo_attributes(neo_object, parents=True, child_first=True,
                            skip_array=False, skip_none=False):
     """
     Given a Neo object, return a dictionary of attributes and annotations.
```

### Comparing `elephant-0.8.0/elephant/pandas_bridge.py` & `elephant-0.9.0/elephant/pandas_bridge.py`

 * *Files identical despite different names*

### Comparing `elephant-0.8.0/elephant/parallel/__init__.py` & `elephant-0.9.0/elephant/parallel/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -42,7 +42,14 @@
 
 try:
     from .mpi import MPIPoolExecutor, MPICommExecutor
 except ImportError:
     # mpi4py is missing
     warnings.warn("mpi4py package is missing. Please run 'pip install mpi4py' "
                   "in a terminal to activate MPI features.")
+
+__all__ = [
+    "ProcessPoolExecutor",
+    "SingleProcess",
+    "MPIPoolExecutor",
+    "MPICommExecutor"
+]
```

### Comparing `elephant-0.8.0/elephant/parallel/mpi.py` & `elephant-0.9.0/elephant/parallel/mpi.py`

 * *Files identical despite different names*

### Comparing `elephant-0.8.0/elephant/parallel/parallel.py` & `elephant-0.9.0/elephant/parallel/parallel.py`

 * *Files identical despite different names*

### Comparing `elephant-0.8.0/elephant/phase_analysis.py` & `elephant-0.9.0/elephant/phase_analysis.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,14 +7,18 @@
 """
 
 from __future__ import division, print_function, unicode_literals
 
 import numpy as np
 import quantities as pq
 
+__all__ = [
+    "spike_triggered_phase"
+]
+
 
 def spike_triggered_phase(hilbert_transform, spiketrains, interpolate):
     """
     Calculate the set of spike-triggered phases of a `neo.AnalogSignal`.
 
     Parameters
     ----------
@@ -117,53 +121,46 @@
             phase_i = 0
 
         # Take only spikes which lie directly within the signal segment -
         # ignore spikes sitting on the last sample
         sttimeind = np.where(np.logical_and(
             spiketrain >= start[phase_i], spiketrain < stop[phase_i]))[0]
 
+        # Extract times for speed reasons
+        times = hilbert_transform[phase_i].times
+
         # Find index into signal for each spike
-        ind_at_spike = np.round(
+        ind_at_spike = (
             (spiketrain[sttimeind] - hilbert_transform[phase_i].t_start) /
             hilbert_transform[phase_i].sampling_period). \
             simplified.magnitude.astype(int)
 
-        # Extract times for speed reasons
-        times = hilbert_transform[phase_i].times
-
         # Append new list to the results for this spiketrain
         result_phases.append([])
         result_amps.append([])
         result_times.append([])
 
         # Step through all spikes
         for spike_i, ind_at_spike_j in enumerate(ind_at_spike):
-            # Difference vector between actual spike time and sample point,
-            # positive if spike time is later than sample point
-            dv = spiketrain[sttimeind[spike_i]] - times[ind_at_spike_j]
-
-            # Make sure ind_at_spike is to the left of the spike time
-            if dv < 0 and ind_at_spike_j > 0:
-                ind_at_spike_j = ind_at_spike_j - 1
 
-            if interpolate:
+            if interpolate and ind_at_spike_j+1 < len(times):
                 # Get relative spike occurrence between the two closest signal
                 # sample points
                 # if z->0 spike is more to the left sample
                 # if z->1 more to the right sample
                 z = (spiketrain[sttimeind[spike_i]] - times[ind_at_spike_j]) /\
                     hilbert_transform[phase_i].sampling_period
 
                 # Save hilbert_transform (interpolate on circle)
                 p1 = np.angle(hilbert_transform[phase_i][ind_at_spike_j])
                 p2 = np.angle(hilbert_transform[phase_i][ind_at_spike_j + 1])
-                result_phases[spiketrain_i].append(
-                    np.angle(
-                        (1 - z) * np.exp(np.complex(0, p1)) +
-                        z * np.exp(np.complex(0, p2))))
+                interpolation = (1 - z) * np.exp(np.complex(0, p1)) \
+                                    + z * np.exp(np.complex(0, p2))
+                p12 = np.angle([interpolation])
+                result_phases[spiketrain_i].append(p12)
 
                 # Save amplitude
                 result_amps[spiketrain_i].append(
                     (1 - z) * np.abs(
                         hilbert_transform[phase_i][ind_at_spike_j]) +
                     z * np.abs(hilbert_transform[phase_i][ind_at_spike_j + 1]))
             else:
@@ -180,9 +177,8 @@
     # Convert outputs to arrays
     for i, entry in enumerate(result_phases):
         result_phases[i] = np.array(entry).flatten()
     for i, entry in enumerate(result_amps):
         result_amps[i] = pq.Quantity(entry, units=entry[0].units).flatten()
     for i, entry in enumerate(result_times):
         result_times[i] = pq.Quantity(entry, units=entry[0].units).flatten()
-
     return result_phases, result_amps, result_times
```

### Comparing `elephant-0.8.0/elephant/signal_processing.py` & `elephant-0.9.0/elephant/signal_processing.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,25 @@
 from __future__ import division, print_function, unicode_literals
 
 import neo
 import numpy as np
 import quantities as pq
 import scipy.signal
 
-from elephant.utils import deprecated_alias
+from elephant.utils import deprecated_alias, check_same_units
+
+__all__ = [
+    "zscore",
+    "cross_correlation_function",
+    "butter",
+    "wavelet_transform",
+    "hilbert",
+    "rauc",
+    "derivative"
+]
 
 
 def zscore(signal, inplace=True):
     r"""
     Apply a z-score operation to one or several `neo.AnalogSignal` objects.
 
     The z-score operation subtracts the mean :math:`\mu` of the signal, and
@@ -40,17 +50,17 @@
 
     Parameters
     ----------
     signal : neo.AnalogSignal or list of neo.AnalogSignal
         Signals for which to calculate the z-score.
     inplace : bool, optional
         If True, the contents of the input `signal` is replaced by the
-        z-transformed signal.
+        z-transformed signal, if possible, i.e when the signal type is float.
         If False, a copy of the original `signal` is returned.
-        Default: True.
+        Default: True
 
     Returns
     -------
     signal_ztransofrmed : neo.AnalogSignal or list of neo.AnalogSignal
         The output format matches the input format: for each input
         `neo.AnalogSignal`, a corresponding `neo.AnalogSignal` is returned,
         containing the z-transformed signal with dimensionless unit.
@@ -118,37 +128,40 @@
        [ 1.03523694,  1.02627526],
        [ 1.11974608,  1.08576948],
        [ 1.20425521,  1.1452637 ]]) * dimensionless, [0.0 s, 0.006 s],
        sampling rate: 1000.0 Hz)>]
 
     """
     # Transform input to a list
-    if not isinstance(signal, list):
+    if isinstance(signal, neo.AnalogSignal):
         signal = [signal]
+    check_same_units(signal, object_type=neo.AnalogSignal)
 
     # Calculate mean and standard deviation
-    signal_stacked = np.vstack(signal)
-    m = np.mean(signal_stacked, axis=0)
-    s = np.std(signal_stacked, axis=0)
+    signal_stacked = np.vstack(signal).magnitude
+    mean = signal_stacked.mean(axis=0)
+    std = signal_stacked.std(axis=0)
 
     signal_ztransofrmed = []
     for sig in signal:
-        sig_normalized = sig.magnitude - m.magnitude
-        sig_normalized = np.divide(sig_normalized, s.magnitude,
-                                   out=np.zeros_like(sig_normalized),
-                                   where=s.magnitude != 0)
-        if inplace:
-            sig[:] = pq.Quantity(sig_normalized, units=sig.units)
-            sig_normalized = sig
-        else:
-            sig_normalized = sig.duplicate_with_new_data(sig_normalized)
-            # todo use flag once is fixed
-            #      https://github.com/NeuralEnsemble/python-neo/issues/752
-            sig_normalized.array_annotate(**sig.array_annotations)
-        sig_dimless = sig_normalized / sig.units
+        sig_normalized = sig.magnitude.astype(mean.dtype, copy=not inplace)
+        sig_normalized -= mean
+        # items where std is zero are already zero
+        np.divide(sig_normalized, std, out=sig_normalized, where=std != 0)
+        sig_dimless = neo.AnalogSignal(signal=sig_normalized,
+                                       units=pq.dimensionless,
+                                       dtype=sig_normalized.dtype,
+                                       copy=False,
+                                       t_start=sig.t_start,
+                                       sampling_rate=sig.sampling_rate,
+                                       name=sig.name,
+                                       file_origin=sig.file_origin,
+                                       description=sig.description,
+                                       array_annotations=sig.array_annotations,
+                                       **sig.annotations)
         signal_ztransofrmed.append(sig_dimless)
 
     # Return single object, or list of objects
     if len(signal_ztransofrmed) == 1:
         signal_ztransofrmed = signal_ztransofrmed[0]
     return signal_ztransofrmed
 
@@ -299,15 +312,18 @@
         raise ValueError("'hilbert_envelope' must be a boolean value")
     if n_lags is not None:
         if not isinstance(n_lags, int) or n_lags <= 0:
             raise ValueError('n_lags must be a non-negative integer')
 
     # z-score analog signal and store channel time series in different arrays
     # Cross-correlation will be calculated between xsig and ysig
-    z_transformed = zscore(signal, inplace=False).magnitude
+    z_transformed = signal.magnitude - signal.magnitude.mean(axis=0)
+    z_transformed = np.divide(z_transformed, signal.magnitude.std(axis=0),
+                              out=z_transformed,
+                              where=z_transformed != 0)
     # transpose (nch, xy, nt) -> (xy, nt, nch)
     xsig, ysig = np.transpose(z_transformed.T[pairs], (1, 2, 0))
 
     # Define vector of lags tau
     nt, nch = xsig.shape
     tau = np.arange(nt) - nt // 2
```

### Comparing `elephant-0.8.0/elephant/spade.py` & `elephant-0.9.0/elephant/spade.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,47 @@
 """
-SPADE is the combination of a mining technique and multiple statistical tests
-to detect and assess the statistical significance of repeated occurrences of
-spike sequences (spatio-temporal patterns, STP).
+SPADE [1]_, [2]_, [3]_ is the combination of a mining technique and multiple
+statistical tests to detect and assess the statistical significance of repeated
+occurrences of spike sequences (spatio-temporal patterns, STP).
+
+
+.. autosummary::
+    :toctree: toctree/spade
+
+    spade
+    concepts_mining
+    pvalue_spectrum
+    test_signature_significance
+    approximate_stability
+    pattern_set_reduction
+    concept_output_to_patterns
 
-Given a list of Neo Spiketrain objects, assumed to be recorded in parallel, the
-SPADE analysis can be applied as demonstrated in this short toy example of 10
-artificial spike trains of exhibiting fully synchronous events of order 10.
 
+Visualization
+-------------
+Visualization of SPADE analysis is covered in Viziphant:
+https://viziphant.readthedocs.io/en/latest/modules.html
+
+
+Notes
+-----
 This modules relies on the implementation of the fp-growth algorithm contained
 in the file fim.so which can be found here (http://www.borgelt.net/pyfim.html)
 and should be available in the spade_src folder (elephant/spade_src/).
 If the fim.so module is not present in the correct location or cannot be
 imported (only available for linux OS) SPADE will make use of a python
 implementation of the fast fca algorithm contained in
 `elephant/spade_src/fast_fca.py`, which is about 10 times slower.
 
 Examples
 --------
+Given a list of Neo Spiketrain objects, assumed to be recorded in parallel, the
+SPADE analysis can be applied as demonstrated in this short toy example of 10
+artificial spike trains of exhibiting fully synchronous events of order 10.
+
 >>> from elephant.spade import spade
 >>> import elephant.spike_train_generation
 >>> import quantities as pq
 
 Generate correlated spiketrains.
 
 >>> spiketrains = elephant.spike_train_generation.cpp(
@@ -48,14 +69,27 @@
 ...              'k.', label=label)
 >>> plt.ylim([-1, len(spiketrains)])
 >>> plt.xlabel('time (ms)')
 >>> plt.ylabel('neurons ids')
 >>> plt.legend()
 >>> plt.show()
 
+References
+----------
+.. [1] Torre, E., Picado-Muino, D., Denker, M., Borgelt, C., & Gruen, S.
+   (2013). Statistical evaluation of synchronous spike patterns extracted
+   by frequent item set mining. Frontiers in Computational Neuroscience, 7.
+.. [2] Quaglio, P., Yegenoglu, A., Torre, E., Endres, D. M., & Gruen, S.
+   (2017). Detection and Evaluation of Spatio-Temporal Spike Patterns in
+   Massively Parallel Spike Train Data with SPADE. Frontiers in
+   Computational Neuroscience, 11.
+.. [3] Stella, A., Quaglio, P., Torre, E., & Gruen, S. (2019). 3d-SPADE:
+   Significance evaluation of spatio-temporal patterns of various temporal
+   extents. Biosystems, 185, 104022.
+
 :copyright: Copyright 2017 by the Elephant team, see `doc/authors.rst`.
 :license: BSD, see LICENSE.txt for details.
 """
 from __future__ import division, print_function, unicode_literals
 
 import operator
 import time
@@ -70,14 +104,24 @@
 from scipy import sparse
 
 import elephant.conversion as conv
 import elephant.spike_train_surrogates as surr
 from elephant.spade_src import fast_fca
 from elephant.utils import deprecated_alias
 
+__all__ = [
+    "spade",
+    "concepts_mining",
+    "pvalue_spectrum",
+    "test_signature_significance",
+    "approximate_stability",
+    "pattern_set_reduction",
+    "concept_output_to_patterns"
+]
+
 warnings.simplefilter('once', UserWarning)
 
 try:
     from mpi4py import MPI  # for parallelized routines
 
     HAVE_MPI = True
 except ImportError:  # pragma: no cover
@@ -92,181 +136,180 @@
 
 
 @deprecated_alias(binsize='bin_size')
 def spade(spiketrains, bin_size, winlen, min_spikes=2, min_occ=2,
           max_spikes=None, max_occ=None, min_neu=1, approx_stab_pars=None,
           n_surr=0, dither=15 * pq.ms, spectrum='#',
           alpha=None, stat_corr='fdr_bh', surr_method='dither_spikes',
-          psr_param=None, output_format='patterns'):
+          psr_param=None, output_format='patterns', **surr_kwargs):
     r"""
-    Perform the SPADE [1-3] analysis for the parallel input `spiketrains`.
-    They are discretized with a temporal resolution equal to
+    Perform the SPADE [1]_, [2]_, [3]_ analysis for the parallel input
+    `spiketrains`. They are discretized with a temporal resolution equal to
     `bin_size` in a sliding window of `winlen*bin_size`.
 
     First, spike patterns are mined from the `spiketrains` using a technique
     called frequent itemset mining (FIM) or formal concept analysis (FCA). In
     this framework, a particular spatio-temporal spike pattern is called a
     "concept". It is then possible to compute the stability and the p-value
     of all pattern candidates. In a final step, concepts are filtered
     according to a stability threshold and a significance level `alpha`.
 
     Parameters
     ----------
-    spiketrains: list of neo.SpikeTrain
+    spiketrains : list of neo.SpikeTrain
         List containing the parallel spike trains to analyze
-    bin_size: pq.Quantity
+    bin_size : pq.Quantity
         The time precision used to discretize the spiketrains (binning).
-    winlen: int
+    winlen : int
         The size (number of bins) of the sliding window used for the analysis.
         The maximal length of a pattern (delay between first and last spike) is
         then given by winlen*bin_size
-    min_spikes: int, optional
+    min_spikes : int, optional
         Minimum number of spikes of a sequence to be considered a pattern.
         Default: 2
-    min_occ: int, optional
+    min_occ : int, optional
         Minimum number of occurrences of a sequence to be considered as a
         pattern.
         Default: 2
-    max_spikes: int, optional
+    max_spikes : int, optional
         Maximum number of spikes of a sequence to be considered a pattern. If
         None no maximal number of spikes is considered.
         Default: None
-    max_occ: int, optional
+    max_occ : int, optional
         Maximum number of occurrences of a sequence to be considered as a
         pattern. If None, no maximal number of occurrences is considered.
         Default: None
-    min_neu: int, optional
+    min_neu : int, optional
         Minimum number of neurons in a sequence to considered a pattern.
         Default: 1
-    approx_stab_pars: dict or None, optional
+    approx_stab_pars : dict or None, optional
         Parameter values for approximate stability computation.
 
         'n_subsets': int
             Number of subsets of a concept used to approximate its stability.
             If `n_subsets` is 0, it is calculated according to to the formula
             given in Babin, Kuznetsov (2012), proposition 6:
 
             .. math::
                    n_{\text{subset}} = \frac{1}{2 \cdot \epsilon^2}
                     \ln{\left( \frac{2}{\delta} \right)} +1
 
-        'delta': float, optional
+        'delta' : float, optional
             delta: probability with at least :math:`1-\delta`
-        'epsilon': float, optional
+        'epsilon' : float, optional
             epsilon: absolute error
-        'stability_thresh': None or list of float
+        'stability_thresh' : None or list of float
             List containing the stability thresholds used to filter the
             concepts.
             If `stability_thresh` is None, then the concepts are not filtered.
             Otherwise, only concepts with
 
-            intensional stability is greater than `stability_thresh[0]` or
-
-            extensional stability is greater than `stability_thresh[1]`
+            * intensional stability is greater than `stability_thresh[0]` or
+            * extensional stability is greater than `stability_thresh[1]`
 
             are further analyzed.
-    n_surr: int, optional
+    n_surr : int, optional
         Number of surrogates to generate to compute the p-value spectrum.
         This number should be large (`n_surr >= 1000` is recommended for 100
         spike trains in `spiketrains`). If `n_surr == 0`, then the p-value
         spectrum is not computed.
         Default: 0
-    dither: pq.Quantity, optional
+    dither : pq.Quantity, optional
         Amount of spike time dithering for creating the surrogates for
         filtering the pattern spectrum. A spike at time `t` is placed randomly
         within `[t-dither, t+dither]` (see also
         :func:`elephant.spike_train_surrogates.dither_spikes`).
         Default: 15*pq.ms
-    spectrum: {'#', '3d#'}, optional
+    spectrum : {'#', '3d#'}, optional
         Define the signature of the patterns.
 
         '#': pattern spectrum using the as signature the pair:
             (number of spikes, number of occurrences)
         '3d#': pattern spectrum using the as signature the triplets:
             (number of spikes, number of occurrence, difference between last
             and first spike of the pattern)
+
         Default: '#'
-    alpha: float, optional
+    alpha : float, optional
         The significance level of the hypothesis tests performed.
         If `alpha is None`, all the concepts are returned.
         If `0.<alpha<1.`, the concepts are filtered according to their
         signature in the p-value spectrum.
         Default: None
-    stat_corr: str
+    stat_corr : str
         Method used for multiple testing.
         See: :func:`test_signature_significance`
         Default: 'fdr_bh'
-    surr_method: str
+    surr_method : str
         Method to generate surrogates. You can use every method defined in
         :func:`elephant.spike_train_surrogates.surrogates`.
         Default: 'dither_spikes'
-    psr_param: None or list of int
+    psr_param : None or list of int or tuple of int
         This list contains parameters used in the pattern spectrum filtering:
-            `psr_param[0]`: correction parameter for subset filtering
-                (see `h_subset_filtering` in :func:`pattern_set_reduction`).
-            `psr_param[1]`: correction parameter for superset filtering
-                (see `k_superset_filtering` in :func:`pattern_set_reduction`).
-            `psr_param[2]`: correction parameter for covered-spikes criterion
-                (see `l_covered_spikes` in :func:`pattern_set_reduction`).
-    output_format: {'concepts', 'patterns'}
+
+        `psr_param[0]`: correction parameter for subset filtering
+            (see `h_subset_filtering` in :func:`pattern_set_reduction`).
+        `psr_param[1]`: correction parameter for superset filtering
+            (see `k_superset_filtering` in :func:`pattern_set_reduction`).
+        `psr_param[2]`: correction parameter for covered-spikes criterion
+            (see `l_covered_spikes` in :func:`pattern_set_reduction`).
+
+    output_format : {'concepts', 'patterns'}
         Distinguish the format of the output (see Returns).
         Default: 'patterns'
+    surr_kwargs
+        Keyword arguments that are passed to the surrogate methods.
 
     Returns
     -------
     output : dict
         'patterns':
             If `output_format` is 'patterns', see the return of
             :func:`concept_output_to_patterns`
 
             If `output_format` is 'concepts', then `output['patterns']` is a
             tuple of patterns which in turn are tuples of
-             1. spikes in the pattern
-
-             2. occurrences of the pattern
+                1. spikes in the pattern
+                2. occurrences of the pattern
 
-             For details see :func:`concepts_mining`.
+            For details see :func:`concepts_mining`.
 
-             if stability is calculated, there are also:
+            if stability is calculated, there are also:
+                3. intensional stability
+                4. extensional stability
 
-             3. intensional stability
-
-             4. extensional stability
-
-             For details see :func:`approximate_stability`.
+            For details see :func:`approximate_stability`.
 
         'pvalue_spectrum' (only if `n_surr > 0`):
             A list of signatures in tuples format:
-             * size
-
-             * number of occurrences
 
-             * duration (only if `spectrum=='3d#'`)
-
-             * p-value
+            * size
+            * number of occurrences
+            * duration (only if `spectrum=='3d#'`)
+            * p-value
 
         'non_sgnf_sgnt': list
             Non significant signatures of 'pvalue_spectrum'.
 
     Notes
     -----
     If detected, this function will use MPI to parallelize the analysis.
 
     References
     ----------
-    [1] Torre, E., Picado-Muino, D., Denker, M., Borgelt, C., & Gruen, S.(2013)
-     Statistical evaluation of synchronous spike patterns extracted by
-     frequent item set mining. Frontiers in Computational Neuroscience, 7.
-    [2] Quaglio, P., Yegenoglu, A., Torre, E., Endres, D. M., & Gruen, S.(2017)
-     Detection and Evaluation of Spatio-Temporal Spike Patterns in Massively
-     Parallel Spike Train Data with SPADE.
-     Frontiers in Computational Neuroscience, 11.
-    [3] Stella, A., Quaglio, P., Torre, E., & Gruen, S. (2019).
-     3d-SPADE: Significance evaluation of spatio-temporal patterns of various
-     temporal extents. Biosystems, 185, 104022.
+    .. [1] Torre, E., Picado-Muino, D., Denker, M., Borgelt, C., & Gruen, S.
+       (2013). Statistical evaluation of synchronous spike patterns extracted
+       by frequent item set mining. Frontiers in Computational Neuroscience, 7.
+    .. [2] Quaglio, P., Yegenoglu, A., Torre, E., Endres, D. M., & Gruen, S.
+       (2017). Detection and Evaluation of Spatio-Temporal Spike Patterns in
+       Massively Parallel Spike Train Data with SPADE. Frontiers in
+       Computational Neuroscience, 11.
+    .. [3] Stella, A., Quaglio, P., Torre, E., & Gruen, S. (2019). 3d-SPADE:
+       Significance evaluation of spatio-temporal patterns of various temporal
+       extents. Biosystems, 185, 104022.
 
     Examples
     --------
     The following example applies SPADE to `spiketrains` (list of
     `neo.SpikeTrain`).
 
     >>> from elephant.spade import spade
@@ -324,15 +367,15 @@
     if n_surr > 0:
         # Compute pvalue spectrum
         time_pvalue_spectrum = time.time()
         pv_spec = pvalue_spectrum(
             spiketrains, bin_size, winlen, dither=dither, n_surr=n_surr,
             min_spikes=min_spikes, min_occ=min_occ, max_spikes=max_spikes,
             max_occ=max_occ, min_neu=min_neu, spectrum=spectrum,
-            surr_method=surr_method)
+            surr_method=surr_method, **surr_kwargs)
         time_pvalue_spectrum = time.time() - time_pvalue_spectrum
         print("Time for pvalue spectrum computation: {}".format(
             time_pvalue_spectrum))
         # Storing pvalue spectrum
         output['pvalue_spectrum'] = pv_spec
 
     # rank!=0 returning None
@@ -405,39 +448,39 @@
             not all([spiketrain.t_stop == spiketrains[0].t_stop
                      for spiketrain in spiketrains]):
         raise ValueError(
             'All spiketrains must have the same t_start and t_stop')
 
     # Check bin_size
     if not isinstance(bin_size, pq.Quantity):
-        raise ValueError('bin_size must be a pq.Quantity')
+        raise TypeError('bin_size must be a pq.Quantity')
 
     # Check winlen
     if not isinstance(winlen, int):
-        raise ValueError('winlen must be an integer')
+        raise TypeError('winlen must be an integer')
 
     # Check min_spikes
     if not isinstance(min_spikes, int):
-        raise ValueError('min_spikes must be an integer')
+        raise TypeError('min_spikes must be an integer')
 
     # Check min_occ
     if not isinstance(min_occ, int):
-        raise ValueError('min_occ must be an integer')
+        raise TypeError('min_occ must be an integer')
 
     # Check max_spikes
     if not (isinstance(max_spikes, int) or max_spikes is None):
-        raise ValueError('max_spikes must be an integer or None')
+        raise TypeError('max_spikes must be an integer or None')
 
     # Check max_occ
     if not (isinstance(max_occ, int) or max_occ is None):
-        raise ValueError('max_occ must be an integer or None')
+        raise TypeError('max_occ must be an integer or None')
 
     # Check min_neu
     if not isinstance(min_neu, int):
-        raise ValueError('min_neu must be an integer')
+        raise TypeError('min_neu must be an integer')
 
     # Check approx_stab_pars
     compute_stability = False
     if isinstance(approx_stab_pars, dict):
         if 'n_subsets' in approx_stab_pars.keys() or\
             ('epsilon' in approx_stab_pars.keys() and
              'delta' in approx_stab_pars.keys()):
@@ -445,51 +488,52 @@
         else:
             raise ValueError(
                 'for approximate stability computation you need to '
                 'pass n_subsets or epsilon and delta.')
 
     # Check n_surr
     if not isinstance(n_surr, int):
-        raise ValueError('n_surr must be an integer')
+        raise TypeError('n_surr must be an integer')
 
     # Check dither
     if not isinstance(dither, pq.Quantity):
-        raise ValueError('dither must be a pq.Quantity')
+        raise TypeError('dither must be a pq.Quantity')
 
     # Check spectrum
     if spectrum not in ('#', '3d#'):
         raise ValueError("spectrum must be '#' or '3d#'")
 
     # Check alpha
     if isinstance(alpha, (int, float)):
         # Check redundant use of alpha
         if 0. < alpha < 1. and n_surr == 0:
             warnings.warn('0.<alpha<1. but p-value spectrum has not been '
                           'computed (n_surr==0)')
     elif alpha is not None:
-        raise ValueError('alpha must be an integer, a float or None')
+        raise TypeError('alpha must be an integer, a float or None')
 
     # Check stat_corr:
     if stat_corr not in \
-            ['bonferroni', 'sidak', 'holm-sidak', 'holm',
+            ('bonferroni', 'sidak', 'holm-sidak', 'holm',
              'simes-hochberg', 'hommel', 'fdr_bh', 'fdr_by',
-             'fdr_tsbh', 'fdr_tsbky', '', 'no']:
+             'fdr_tsbh', 'fdr_tsbky', '', 'no'):
         raise ValueError("Parameter stat_corr not recognized")
 
     # Check surr_method
     if surr_method not in surr.SURR_METHODS:
         raise ValueError(
             'specified surr_method (=%s) not valid' % surr_method)
 
     # Check psr_param
     if psr_param is not None:
-        if not isinstance(psr_param, list):
-            raise ValueError('psr_param must be None or a list of integer')
+        if not isinstance(psr_param, (list, tuple)):
+            raise TypeError('psr_param must be None or a list or tuple of '
+                            'integer')
         if not all(isinstance(param, int) for param in psr_param):
-            raise ValueError('elements of psr_param must be integers')
+            raise TypeError('elements of psr_param must be integers')
 
     # Check output_format
     if output_format not in ('concepts', 'patterns'):
         raise ValueError("The output_format value has to be"
                          "'patterns' or 'concepts'")
 
     return compute_stability
@@ -497,49 +541,49 @@
 
 @deprecated_alias(binsize='bin_size')
 def concepts_mining(spiketrains, bin_size, winlen, min_spikes=2, min_occ=2,
                     max_spikes=None, max_occ=None, min_neu=1, report='a'):
     """
     Find pattern candidates extracting all the concepts of the context, formed
     by the objects defined as all windows of length `winlen*bin_size` slided
-    along the `spiketrains` and the attributes as the spikes occurring in each
-    of the window discretized at a time resolution equal to `bin_size`. Hence,
-    the output are all the repeated sequences of spikes with maximal length
-    `winlen`, which are not trivially explained by the same number of
-    occurrences of a superset of spikes.
+    along the discretized `spiketrains` and the attributes as the spikes
+    occurring in each of the windows. Hence, the output are all the repeated
+    sequences of spikes with maximal length `winlen`, which are not trivially
+    explained by the same number of occurrences of a superset of spikes.
 
     Parameters
     ----------
-    spiketrains: list of neo.SpikeTrain
-        List containing the parallel spike trains to analyze
-    bin_size: pq.Quantity
+    spiketrains : list of neo.SpikeTrain or conv.BinnedSpikeTrain
+        Either list of the spiketrains to analyze or
+        BinningSpikeTrain object containing the binned spiketrains to analyze
+    bin_size : pq.Quantity
         The time precision used to discretize the `spiketrains` (clipping).
-    winlen: int
+    winlen : int
         The size (number of bins) of the sliding window used for the analysis.
         The maximal length of a pattern (delay between first and last spike) is
         then given by `winlen*bin_size`
-    min_spikes: int, optional
+    min_spikes : int, optional
         Minimum number of spikes of a sequence to be considered a pattern.
         Default: 2
-    min_occ: int, optional
+    min_occ : int, optional
         Minimum number of occurrences of a sequence to be considered as a
         pattern.
         Default: 2
-    max_spikes: int, optional
+    max_spikes : int, optional
         Maximum number of spikes of a sequence to be considered a pattern. If
         None no maximal number of spikes is considered.
         Default: None
-    max_occ: int, optional
+    max_occ : int, optional
         Maximum number of occurrences of a sequence to be considered as a
         pattern. If None, no maximal number of occurrences is considered.
         Default: None
-    min_neu: int, optional
+    min_neu : int, optional
         Minimum number of neurons in a sequence to considered a pattern.
         Default: 1
-    report: {'a', '#', '3d#'}, optional
+    report : {'a', '#', '3d#'}, optional
         Indicates the output of the function.
 
         'a':
             All the mined patterns
 
         '#':
             Pattern spectrum using as signature the pair:
@@ -575,40 +619,37 @@
         according to their position in time). Each column corresponds to one
         bin and one neuron and it is 0 if no spikes or 1 if one or more spikes
         occurred in that bin for that particular neuron. For example, the entry
         [0,0] of this matrix corresponds to the first bin of the first window
         position for the first neuron, the entry `[0,winlen]` to the first
         bin of the first window position for the second neuron.
     """
-    # Check that spiketrains is a list of SpikeTrains
-    if not all([isinstance(elem, neo.SpikeTrain) for elem in spiketrains]):
-        raise TypeError(
-            'spiketrains must be a list of SpikeTrains')
-    # Check that all spiketrains have same t_start and same t_stop
-    if not all([spiketrain.t_start == spiketrains[0].t_start
-                for spiketrain in spiketrains]) or\
-            not all([spiketrain.t_stop == spiketrains[0].t_stop
-                     for spiketrain in spiketrains]):
-        raise ValueError(
-            'All spiketrains must have the same t_start and t_stop')
-    if report not in ['a', '#', '3d#']:
+    if report not in ('a', '#', '3d#'):
         raise ValueError(
             "report has to assume of the following values:" +
             "  'a', '#' and '3d#,' got {} instead".format(report))
-    # Binning the spiketrains and clipping (binary matrix)
-    binary_matrix = conv.BinnedSpikeTrain(
-        spiketrains, bin_size).to_sparse_bool_array().tocoo()
+    # if spiketrains is list of neo.SpikeTrain convert to conv.BinnedSpikeTrain
+    if isinstance(spiketrains, list) and \
+            isinstance(spiketrains[0], neo.SpikeTrain):
+        spiketrains = conv.BinnedSpikeTrain(
+            spiketrains, bin_size=bin_size, tolerance=None)
+    if not isinstance(spiketrains, conv.BinnedSpikeTrain):
+        raise TypeError(
+            'spiketrains must be either a list of neo.SpikeTrain or '
+            'a conv.BinnedSpikeTrain object')
+    # Clipping the spiketrains and (binary matrix)
+    binary_matrix = spiketrains.to_sparse_bool_array().tocoo(copy=False)
     # Computing the context and the binary matrix encoding the relation between
     # objects (window positions) and attributes (spikes,
     # indexed with a number equal to  neuron idx*winlen+bin idx)
     context, transactions, rel_matrix = _build_context(binary_matrix, winlen)
     # By default, set the maximum pattern size to the maximum number of
     # spikes in a window
     if max_spikes is None:
-        max_spikes = len(spiketrains) * winlen
+        max_spikes = binary_matrix.shape[0] * winlen
     # By default, set maximum number of occurrences to number of non-empty
     # windows
     if max_occ is None:
         max_occ = int(np.sum(np.sum(rel_matrix, axis=1) > 0))
     # Check if fim.so available and use it
     if HAVE_FIM:
         # Return the output
@@ -1146,103 +1187,99 @@
         len(np.unique(np.array(intent) // winlen)) >= min_neu and \
         min(np.array(intent) % winlen) == 0
     return keep_concepts
 
 
 @deprecated_alias(binsize='bin_size')
 def pvalue_spectrum(
-        spiketrains,
-        bin_size,
-        winlen,
-        dither,
-        n_surr,
-        min_spikes=2,
-        min_occ=2,
-        max_spikes=None,
-        max_occ=None,
-        min_neu=1,
-        spectrum='#',
-        surr_method='dither_spikes'):
+        spiketrains, bin_size, winlen, dither, n_surr, min_spikes=2, min_occ=2,
+        max_spikes=None, max_occ=None, min_neu=1, spectrum='#',
+        surr_method='dither_spikes', **surr_kwargs):
     """
     Compute the p-value spectrum of pattern signatures extracted from
     surrogates of parallel spike trains, under the null hypothesis of
     independent spiking.
 
     * n_surr surrogates are obtained from each spike train by spike dithering
     * pattern candidates (concepts) are collected from each surrogate data
     * the signatures (number of spikes, number of occurrences) of all patterns
       are computed, and their  occurrence probability estimated by their
       occurrence frequency (p-value spectrum)
 
     Parameters
     ----------
-    spiketrains: list of neo.SpikeTrain
+    spiketrains : list of neo.SpikeTrain
         List containing the parallel spike trains to analyze
-    bin_size: pq.Quantity
+    bin_size : pq.Quantity
         The time precision used to discretize the `spiketrains` (binning).
-    winlen: int
+    winlen : int
         The size (number of bins) of the sliding window used for the analysis.
         The maximal length of a pattern (delay between first and last spike) is
         then given by `winlen*bin_size`
-    dither: pq.Quantity
+    dither : pq.Quantity
         Amount of spike time dithering for creating the surrogates for
         filtering the pattern spectrum. A spike at time t is placed randomly
         within `[t-dither, t+dither]` (see also
         :func:`elephant.spike_train_surrogates.dither_spikes`).
         Default: 15*pq.s
-    n_surr: int
+    n_surr : int
         Number of surrogates to generate to compute the p-value spectrum.
         This number should be large (`n_surr>=1000` is recommended for 100
         spike trains in spiketrains). If `n_surr` is 0, then the p-value
         spectrum is not computed.
         Default: 0
-    min_spikes: int, optional
+    min_spikes : int, optional
         Minimum number of spikes of a sequence to be considered a pattern.
         Default: 2
-    min_occ: int, optional
+    min_occ : int, optional
         Minimum number of occurrences of a sequence to be considered as a
         pattern.
         Default: 2
-    max_spikes: int, optional
+    max_spikes : int, optional
         Maximum number of spikes of a sequence to be considered a pattern. If
         None no maximal number of spikes is considered.
         Default: None
-    max_occ: int, optional
+    max_occ : int, optional
         Maximum number of occurrences of a sequence to be considered as a
         pattern. If None, no maximal number of occurrences is considered.
         Default: None
-    min_neu: int, optional
+    min_neu : int, optional
         Minimum number of neurons in a sequence to considered a pattern.
         Default: 1
-    spectrum: {'#', '3d#'}, optional
+    spectrum : {'#', '3d#'}, optional
         Defines the signature of the patterns.
 
         '#': pattern spectrum using the as signature the pair:
             (number of spikes, number of occurrence)
         '3d#': pattern spectrum using the as signature the triplets:
             (number of spikes, number of occurrence, difference between last
             and first spike of the pattern)
+
         Default: '#'
-    surr_method: str
+    surr_method : str
         Method that is used to generate the surrogates. You can use every
         method defined in
         :func:`elephant.spike_train_surrogates.dither_spikes`.
         Default: 'dither_spikes'
+    surr_kwargs
+        Keyword arguments that are passed to the surrogate methods.
 
     Returns
     -------
     pv_spec : list
+
         if spectrum == '#':
             A list of triplets (z,c,p), where (z,c) is a pattern signature
             and p is the corresponding p-value (fraction of surrogates
             containing signatures (z*,c*)>=(z,c)).
         if spectrum == '3d#':
             A list of triplets (z,c,l,p), where (z,c,l) is a pattern signature
             and p is the corresponding p-value (fraction of surrogates
             containing signatures (z*,c*,l*)>=(z,c,l)).
+
         Signatures whose empirical p-value is 0 are not listed.
 
     """
     # Initializing variables for parallel computing
     if HAVE_MPI:  # pragma: no cover
         comm = MPI.COMM_WORLD  # create MPI communicator
         rank = comm.Get_rank()  # get rank of current MPI task
@@ -1252,14 +1289,16 @@
         size = 1
     # Check on number of surrogates
     if n_surr <= 0:
         raise ValueError('n_surr has to be >0')
     if surr_method not in surr.SURR_METHODS:
         raise ValueError(
             'specified surr_method (=%s) not valid' % surr_method)
+    if spectrum not in ('#', '3d#'):
+        raise ValueError("Invalid spectrum: '{}'".format(spectrum))
 
     len_partition = n_surr // size  # length of each MPI task
     len_remainder = n_surr % size
 
     add_remainder = rank < len_remainder
 
     if max_spikes is None:
@@ -1272,46 +1311,30 @@
                                    max_spikes - min_spikes + 1),
                             dtype=np.uint16)
     else:  # spectrum == '3d#':
         max_occs = np.empty(shape=(len_partition + add_remainder,
                                    max_spikes - min_spikes + 1, winlen),
                             dtype=np.uint16)
 
-    if surr_method == 'joint_isi_dithering':
-        joint_isi_instances = [surr.JointISI(spiketrain, dither=dither,
-                                             method='window')
-                               for spiketrain in spiketrains]
-    for i in range(len_partition + add_remainder):
-        if surr_method == 'joint_isi_dithering':
-            surrs = [instance.dithering()[0] for
-                     instance in joint_isi_instances]
-        elif surr_method == 'dither_spikes_with_refractory_period':
-            # The initial refractory period is set to the bin size in order to
-            # prevent that spikes fall into the same bin, if the spike trains
-            # are sparse (min(ISI)>bin size).
-            surrs = [surr.dither_spikes(
-                spiketrain, dither=dither, n_surrogates=1,
-                refractory_period=bin_size)[0]
-                for spiketrain in spiketrains]
-        else:
-            surrs = [surr.surrogates(
-                spiketrain, n_surrogates=1, method=surr_method,
-                dt=dither)[0] for spiketrain in spiketrains]
+    for surr_id, binned_surrogates in _generate_binned_surrogates(
+            spiketrains, bin_size=bin_size, dither=dither,
+            surr_method=surr_method, n_surrogates=len_partition+add_remainder,
+            **surr_kwargs):
 
         # Find all pattern signatures in the current surrogate data set
         surr_concepts = concepts_mining(
-            surrs, bin_size, winlen, min_spikes=min_spikes,
+            binned_surrogates, bin_size, winlen, min_spikes=min_spikes,
             max_spikes=max_spikes, min_occ=min_occ, max_occ=max_occ,
             min_neu=min_neu, report=spectrum)[0]
         # The last entry of the signature is the number of times the
         # signature appeared. This entry is not needed here.
         surr_concepts = surr_concepts[:, :-1]
 
-        max_occs[i] = _get_max_occ(surr_concepts, min_spikes, max_spikes,
-                                   winlen, spectrum)
+        max_occs[surr_id] = _get_max_occ(
+            surr_concepts, min_spikes, max_spikes, winlen, spectrum)
 
     # Collecting results on the first PCU
     if size != 1:
         max_occs = comm.gather(max_occs, root=0)
 
         if rank != 0:  # pragma: no cover
             return []
@@ -1321,14 +1344,70 @@
         max_occs = np.vstack(max_occs)
 
     # Compute the p-value spectrum, and return it
     return _get_pvalue_spec(max_occs, min_spikes, max_spikes, min_occ,
                             n_surr, winlen, spectrum)
 
 
+def _generate_binned_surrogates(
+        spiketrains, bin_size, dither, surr_method, n_surrogates,
+        **surr_kwargs):
+    if surr_method == 'bin_shuffling':
+        binned_spiketrains = [
+            conv.BinnedSpikeTrain(
+                spiketrain, bin_size=bin_size, tolerance=None)
+            for spiketrain in spiketrains]
+        max_displacement = int(dither.rescale(pq.ms).magnitude /
+                               bin_size.rescale(pq.ms).magnitude)
+    elif surr_method in ('joint_isi_dithering', 'isi_dithering'):
+        isi_dithering = surr_method == 'isi_dithering'
+        joint_isi_instances = \
+            [surr.JointISI(spiketrain, dither=dither,
+                           isi_dithering=isi_dithering, **surr_kwargs)
+             for spiketrain in spiketrains]
+    for surr_id in range(n_surrogates):
+        if surr_method == 'bin_shuffling':
+            binned_surrogates = \
+                [surr.bin_shuffling(binned_spiketrain,
+                                    max_displacement=max_displacement,
+                                    **surr_kwargs)[0]
+                 for binned_spiketrain in binned_spiketrains]
+            binned_surrogates = np.array(
+                [binned_surrogate.to_bool_array()[0]
+                 for binned_surrogate in binned_surrogates])
+            binned_surrogates = conv.BinnedSpikeTrain(
+                binned_surrogates,
+                bin_size=bin_size,
+                t_start=spiketrains[0].t_start,
+                t_stop=spiketrains[0].t_stop)
+        elif surr_method in ('joint_isi_dithering', 'isi_dithering'):
+            surrs = [instance.dithering()[0]
+                     for instance in joint_isi_instances]
+        elif surr_method == 'dither_spikes_with_refractory_period':
+            # The initial refractory period is set to the bin size in order to
+            # prevent that spikes fall into the same bin, if the spike trains
+            # are sparse (min(ISI)>bin size).
+            surrs = \
+                [surr.dither_spikes(
+                    spiketrain, dither=dither, n_surrogates=1,
+                    refractory_period=bin_size, **surr_kwargs)[0]
+                 for spiketrain in spiketrains]
+        else:
+            surrs = \
+                [surr.surrogates(
+                    spiketrain, n_surrogates=1, method=surr_method,
+                    dt=dither, **surr_kwargs)[0]
+                 for spiketrain in spiketrains]
+
+        if surr_method != 'bin_shuffling':
+            binned_surrogates = conv.BinnedSpikeTrain(
+                surrs, bin_size=bin_size, tolerance=None)
+        yield surr_id, binned_surrogates
+
+
 def _get_pvalue_spec(max_occs, min_spikes, max_spikes, min_occ, n_surr, winlen,
                      spectrum):
     """
     This function converts the list of maximal occurrences into the
     corresponding p-value spectrum.
 
     Parameters
@@ -1393,17 +1472,14 @@
     np.ndarray
         Two-dimensional array. Each element corresponds to a highest occurrence
         for a specific pattern size (which range from min_spikes to max_spikes)
         and pattern duration (which range from 0 to winlen-1).
         The first axis corresponds to the pattern size the second to the
         duration.
     """
-    if spectrum not in ('#', '3d#'):
-        raise ValueError("Invalid spectrum: '{}'".format(spectrum))
-
     if spectrum == '#':
         winlen = 1
     max_occ = np.zeros(shape=(max_spikes - min_spikes + 1, winlen))
     for size_id, pt_size in enumerate(range(min_spikes, max_spikes + 1)):
         concepts_for_size = surr_concepts[
             surr_concepts[:, 0] == pt_size][:, 1:]
         for dur in range(winlen):
@@ -1456,17 +1532,32 @@
         signatures = {(len(concept[0]), len(concept[1]))
                       for concept in concepts}
     else:  # spectrum == '3d#':
         # third entry of signatures is the duration, fixed as the maximum lag
         signatures = {(len(concept[0]), len(concept[1]),
                        max(np.array(concept[0]) % winlen))
                       for concept in concepts}
-    mask = np.array([tuple(pvs[:-1]) in signatures
-                     and not np.isclose(pvs[-1], [1])
-                     for pvs in pv_spec])
+    mask = np.zeros(len(pv_spec), dtype=bool)
+    for index, pv_entry in enumerate(pv_spec):
+        if tuple(pv_entry[:-1]) in signatures \
+                and not np.isclose(pv_entry[-1], [1]):
+            # select the highest number of occurrences for size and duration
+            mask[index] = True
+            if mask[index-1]:
+                if spectrum == '#':
+                    size = pv_spec[index][0]
+                    prev_size = pv_spec[index-1][0]
+                    if prev_size == size:
+                        mask[index-1] = False
+                else:
+                    size, duration = pv_spec[index][[0, 2]]
+                    prev_size, prev_duration = pv_spec[index-1][[0, 2]]
+                    if prev_size == size and duration == prev_duration:
+                        mask[index-1] = False
+
     return mask
 
 
 def test_signature_significance(pv_spec, concepts, alpha, winlen,
                                 corr='fdr_bh', report='spectrum',
                                 spectrum='#'):
     """
@@ -1477,98 +1568,103 @@
     (z,c), this routine assesses the significance of (z,c) using the
     confidence level alpha.
 
     Bonferroni or FDR statistical corrections can be applied.
 
     Parameters
     ----------
-    pv_spec: list
+    pv_spec : list
         A list of triplets (z,c,p), where z is pattern size, c is pattern
         support and p is the p-value of signature (z,c)
-    concepts: list of tuple
+    concepts : list of tuple
         Output of the concepts mining for the original data.
-    alpha: float
+    alpha : float
         Significance level of the statistical test
-    winlen: int
+    winlen : int
         Size (number of bins) of the sliding window used for the analysis
-    corr: str, optional
+    corr : str, optional
         Method used for testing and adjustment of pvalues.
         Can be either the full name or initial letters.
         Available methods are:
-            'bonferroni' : one-step correction
 
-            'sidak' : one-step correction
+        'bonferroni' : one-step correction
+
+        'sidak' : one-step correction
 
-            'holm-sidak' : step down method using Sidak adjustments
+        'holm-sidak' : step down method using Sidak adjustments
 
-            'holm' : step-down method using Bonferroni adjustments
+        'holm' : step-down method using Bonferroni adjustments
 
-            'simes-hochberg' : step-up method (independent)
+        'simes-hochberg' : step-up method (independent)
 
-            'hommel' : closed method based on Simes tests (non-negative)
+        'hommel' : closed method based on Simes tests (non-negative)
 
-            'fdr_bh' : Benjamini/Hochberg (non-negative)
+        'fdr_bh' : Benjamini/Hochberg (non-negative)
 
-            'fdr_by' : Benjamini/Yekutieli (negative)
+        'fdr_by' : Benjamini/Yekutieli (negative)
 
-            'fdr_tsbh' : two stage fdr correction (non-negative)
+        'fdr_tsbh' : two stage fdr correction (non-negative)
 
-            'fdr_tsbky' : two stage fdr correction (non-negative)
+        'fdr_tsbky' : two stage fdr correction (non-negative)
+
+        '' or 'no': no statistical correction
 
-            '' or 'no': no statistical correction
         For further description see:
         https://www.statsmodels.org/stable/generated/statsmodels.stats.multitest.multipletests.html
         Default: 'fdr_bh'
 
-    report: {'spectrum', 'significant', 'non_significant'}, optional
+    report : {'spectrum', 'significant', 'non_significant'}, optional
         Format to be returned for the significance spectrum:
 
         'spectrum': list of triplets (z,c,b), where b is a boolean specifying
                     whether signature (z,c) is significant (True) or not
                     (False)
 
         'significant': list containing only the significant signatures (z,c) of
                        pvalue_spectrum
 
         'non_significant': list containing only the non-significant signatures
-    spectrum: {'#', '3d#'}, optional
+
+    spectrum : {'#', '3d#'}, optional
         Defines the signature of the patterns.
 
         '#': pattern spectrum using the as signature the pair:
             (number of spikes, number of occurrence)
         '3d#': pattern spectrum using the as signature the triplets:
             (number of spikes, number of occurrence, difference between last
             and first spike of the pattern)
+
         Default: '#'
 
     Returns
     -------
     sig_spectrum : list
         Significant signatures of pvalue_spectrum, in the format specified
         by `report`
     """
     # If alpha == 1 all signatures are significant
     if alpha == 1:
         return []
 
-    if spectrum not in ['#', '3d#']:
+    if spectrum not in ('#', '3d#'):
         raise ValueError("spectrum must be either '#' or '3d#', "
                          "got {} instead".format(spectrum))
-    if report not in ['spectrum', 'significant', 'non_significant']:
+    if report not in ('spectrum', 'significant', 'non_significant'):
         raise ValueError("report must be either 'spectrum'," +
                          "  'significant' or 'non_significant'," +
                          "got {} instead".format(report))
-    if corr not in ['bonferroni', 'sidak', 'holm-sidak', 'holm',
+    if corr not in ('bonferroni', 'sidak', 'holm-sidak', 'holm',
                     'simes-hochberg', 'hommel', 'fdr_bh', 'fdr_by',
-                    'fdr_tsbh', 'fdr_tsbky', '', 'no']:
+                    'fdr_tsbh', 'fdr_tsbky', '', 'no'):
         raise ValueError("Parameter corr not recognized")
 
     pv_spec = np.array(pv_spec)
     mask = _mask_pvalue_spectrum(pv_spec, concepts, spectrum, winlen)
     pvalues = pv_spec[:, -1]
+
     pvalues_totest = pvalues[mask]
 
     # Initialize test array to False
     tests = [False] * len(pvalues)
 
     if len(pvalues_totest) > 0:
 
@@ -1583,42 +1679,43 @@
                     "Please run 'pip install statsmodels' if you "
                     "want to use multiple testing correction")
 
             tests_selected = sm.multipletests(pvalues_totest, alpha=alpha,
                                               method=corr)[0]
 
         # assign each corrected pvalue to its corresponding entry
+        # this breaks
         for index, value in zip(mask.nonzero()[0], tests_selected):
             tests[index] = value
 
     # Return the specified results:
     if spectrum == '#':
         if report == 'spectrum':
-            sig_spectrum = [(size, supp, test)
-                            for (size, supp, pv), test in zip(pv_spec, tests)]
+            sig_spectrum = [(size, occ, test)
+                            for (size, occ, pv), test in zip(pv_spec, tests)]
         elif report == 'significant':
-            sig_spectrum = [(size, supp) for ((size, supp, pv), test)
+            sig_spectrum = [(size, occ) for ((size, occ, pv), test)
                             in zip(pv_spec, tests) if test]
         else:  # report == 'non_significant'
-            sig_spectrum = [(size, supp)
-                            for ((size, supp, pv), test) in zip(pv_spec, tests)
+            sig_spectrum = [(size, occ)
+                            for ((size, occ, pv), test) in zip(pv_spec, tests)
                             if not test]
 
     else:  # spectrum == '3d#'
         if report == 'spectrum':
             sig_spectrum =\
-                [(size, supp, l, test)
-                 for (size, supp, l, pv), test in zip(pv_spec, tests)]
+                [(size, occ, l, test)
+                 for (size, occ, l, pv), test in zip(pv_spec, tests)]
         elif report == 'significant':
-            sig_spectrum = [(size, supp, l) for ((size, supp, l, pv), test)
+            sig_spectrum = [(size, occ, l) for ((size, occ, l, pv), test)
                             in zip(pv_spec, tests) if test]
         else:  # report == 'non_significant'
             sig_spectrum =\
-                [(size, supp, l)
-                 for ((size, supp, l, pv), test) in zip(pv_spec, tests)
+                [(size, occ, l)
+                 for ((size, occ, l, pv), test) in zip(pv_spec, tests)
                  if not test]
     return sig_spectrum
 
 
 def _pattern_spectrum_filter(concept, ns_signatures, spectrum, winlen):
     """
     Filter for significant concepts
@@ -1637,44 +1734,45 @@
                           delta=0., epsilon=0.):
     r"""
     Approximate the stability of concepts. Uses the algorithm described
     in Babin, Kuznetsov (2012): Approximating Concept Stability
 
     Parameters
     ----------
-    concepts: list
+    concepts : list
         All the pattern candidates (concepts) found in the spiketrains. Each
         pattern is represented as a tuple containing (spike IDs,
         discrete times (window position)
         of the  occurrences of the pattern). The spike IDs are defined as:
         `spike_id=neuron_id*bin_id` with `neuron_id` in `[0, len(spiketrains)]`
         and `bin_id` in `[0, winlen]`.
-    rel_matrix: sparse.coo_matrix
+    rel_matrix : sparse.coo_matrix
         A binary matrix with shape (number of windows,
         winlen*len(spiketrains)). Each row corresponds to a window (order
         according to their position in time).
         Each column corresponds to one bin and one neuron and it is 0 if
         no spikes or 1 if one or more spikes occurred in that bin for that
         particular neuron. For example, the entry [0,0] of this matrix
         corresponds to the first bin of the first window position for the first
         neuron, the entry `[0, winlen]` to the first bin of the first window
         position for the second neuron.
-    n_subsets: int
+    n_subsets : int
         Number of subsets of a concept used to approximate its stability.
         If `n_subsets` is 0, it is calculated according to to the formula
         given in Babin, Kuznetsov (2012), proposition 6:
 
         .. math::
                n_{\text{subset}} = \frac{1}{2 \cdot \epsilon^2}
                 \ln{\left( \frac{2}{\delta} \right)} +1
+
         Default: 0
-    delta: float, optional
+    delta : float, optional
         delta: probability with at least :math:`1-\delta`
         Default: 0.
-    epsilon: float, optional
+    epsilon : float, optional
         epsilon: absolute error
         Default: 0.
 
     Returns
     -------
     output : list
         List of all the pattern candidates (concepts) given in input, each with
@@ -1891,43 +1989,43 @@
         * a pair of concepts cannot cause one another to be rejected
         * if two concepts overlap more than min_occ times, one of them can
           account for all occurrences of the other one if it passes the
           filtering
 
     Parameters
     ----------
-    concepts: list
+    concepts : list
         List of concepts, each consisting in its intent and extent
-    ns_signatures: list
+    ns_signatures : list
         A list of non-significant pattern signatures (z, c)
-    winlen: int
+    winlen : int
         The size (number of bins) of the sliding window used for the analysis.
         The maximal length of a pattern (delay between first and last spike) is
         then given by `winlen*bin_size`.
-    spectrum: {'#', '3d#'}
+    spectrum : {'#', '3d#'}
         Define the signature of the patterns.
 
         '#': pattern spectrum using the as signature the pair:
             (number of spikes, number of occurrences)
         '3d#': pattern spectrum using the as signature the triplets:
             (number of spikes, number of occurrence, difference between last
             and first spike of the pattern)
-    h_subset_filtering: int, optional
+    h_subset_filtering : int, optional
         Correction parameter for subset filtering
         Default: 0
-    k_superset_filtering: int, optional
+    k_superset_filtering : int, optional
         Correction parameter for superset filtering
         Default: 0
-    l_covered_spikes: int, optional
+    l_covered_spikes : int, optional
         Correction parameter for covered-spikes criterion
         Default: 0
-    min_spikes: int, optional
+    min_spikes : int, optional
         Minimum pattern size
         Default: 2
-    min_occ: int, optional
+    min_occ : int, optional
         Minimum number of pattern occurrences
         Default: 2
 
     Returns
     -------
     tuple
         A tuple containing the elements of the input argument
@@ -2179,46 +2277,49 @@
         to None all p-values are set to -1.
     spectrum: {'#', '3d#'}
         '#': pattern spectrum using the as signature the pair:
             (number of spikes, number of occurrences)
         '3d#': pattern spectrum using the as signature the triplets:
             (number of spikes, number of occurrence, difference between last
             and first spike of the pattern)
+
         Default: '#'
     t_start: pq.Quantity
         t_start of the analyzed spike trains
 
     Returns
     -------
     output : list
         List of dictionaries. Each dictionary corresponds to a pattern and
         has the following entries:
-            'itemset':
-                A list of the spikes in the pattern, expressed in theform of
-                itemset, each spike is encoded by
-                `spiketrain_id * winlen + bin_id`.
-            'windows_ids':
-                The ids of the windows in which the pattern occurred
-                in discretized time (given byt the binning).
-            'neurons':
-                An array containing the idx of the neurons of the pattern.
-            'lags':
-                An array containing the lags (integers corresponding to the
-                number of bins) between the spikes of the patterns. The first
-                lag is always assumed to be 0 and corresponds to the first
-                spike.
-            'times':
-                An array containing the times (integers corresponding to the
-                bin idx) of the occurrences of the patterns.
-            'signature':
-                A tuple containing two integers (number of spikes of the
-                patterns, number of occurrences of the pattern).
-            'pvalue':
-                The p-value corresponding to the pattern. If `n_surr==0`,
-                all p-values are set to -1.
+
+        'itemset':
+            A list of the spikes in the pattern, expressed in theform of
+            itemset, each spike is encoded by
+            `spiketrain_id * winlen + bin_id`.
+        'windows_ids':
+            The ids of the windows in which the pattern occurred
+            in discretized time (given byt the binning).
+        'neurons':
+            An array containing the idx of the neurons of the pattern.
+        'lags':
+            An array containing the lags (integers corresponding to the
+            number of bins) between the spikes of the patterns. The first
+            lag is always assumed to be 0 and corresponds to the first
+            spike.
+        'times':
+            An array containing the times (integers corresponding to the
+            bin idx) of the occurrences of the patterns.
+        'signature':
+            A tuple containing two integers (number of spikes of the
+            patterns, number of occurrences of the pattern).
+        'pvalue':
+            The p-value corresponding to the pattern. If `n_surr==0`,
+            all p-values are set to -1.
+
     """
     if pv_spec is not None:
         pvalue_dict = defaultdict(float)
         # Creating a dictionary for the pvalue spectrum
         for entry in pv_spec:
             if spectrum == '3d#':
                 pvalue_dict[(entry[0], entry[1], entry[2])] = entry[-1]
```

### Comparing `elephant-0.8.0/elephant/spade_src/LICENSE` & `elephant-0.9.0/elephant/spade_src/LICENSE`

 * *Files identical despite different names*

### Comparing `elephant-0.8.0/elephant/spade_src/fast_fca.py` & `elephant-0.9.0/elephant/spade_src/fast_fca.py`

 * *Files identical despite different names*

### Comparing `elephant-0.8.0/elephant/spectral.py` & `elephant-0.9.0/elephant/spectral.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,19 @@
 import warnings
 import numpy as np
 import quantities as pq
 import scipy.signal
 
 from elephant.utils import deprecated_alias
 
+__all__ = [
+    "welch_psd",
+    "welch_coherence"
+]
+
 
 @deprecated_alias(num_seg='n_segments', len_seg='len_segment',
                   freq_res='frequency_resolution')
 def welch_psd(signal, n_segments=8, len_segment=None,
               frequency_resolution=None, overlap=0.5, fs=1.0, window='hanning',
               nfft=None, detrend='constant', return_onesided=True,
               scaling='density', axis=-1):
```

### Comparing `elephant-0.8.0/elephant/spike_train_correlation.py` & `elephant-0.9.0/elephant/spike_train_correlation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,20 @@
 # -*- coding: utf-8 -*-
 """
 This modules provides functions to calculate correlations between spike trains.
 
+.. autosummary::
+    :toctree: toctree/spike_train_correlation
+
+    covariance
+    correlation_coefficient
+    cross_correlation_histogram
+    spike_time_tiling_coefficient
+    spike_train_timescale
+
 :copyright: Copyright 2015-2016 by the Elephant team, see `doc/authors.rst`.
 :license: Modified BSD, see LICENSE.txt for details.
 """
 from __future__ import division, print_function, unicode_literals
 
 import warnings
 
@@ -13,14 +22,22 @@
 import numpy as np
 import quantities as pq
 import scipy.signal
 from scipy import integrate
 
 from elephant.utils import deprecated_alias
 
+__all__ = [
+    "covariance",
+    "correlation_coefficient",
+    "cross_correlation_histogram",
+    "spike_time_tiling_coefficient",
+    "spike_train_timescale"
+]
+
 # The highest sparsity of the `BinnedSpikeTrain` matrix for which
 # memory-efficient (sparse) implementation of `covariance()` is faster than
 # with the corresponding numpy dense array.
 _SPARSITY_MEMORY_EFFICIENT_THR = 0.1
 
 
 class _CrossCorrHist(object):
@@ -62,61 +79,59 @@
         Returns
         -------
         lags : np.ndarray
             Array of lags at which the cross-correlation can be computed
             at full overlap (valid mode).
         """
 
-        bin_size = binned_spiketrain_i.bin_size
+        bin_size = binned_spiketrain_i._bin_size
 
         # see cross_correlation_histogram for the examples
         if binned_spiketrain_i.n_bins < binned_spiketrain_j.n_bins:
             # ex. 1) lags range: [-2, 5] ms
             # ex. 2) lags range: [1, 2] ms
-            left_edge = (binned_spiketrain_j.t_start -
-                         binned_spiketrain_i.t_start) / bin_size
-            right_edge = (binned_spiketrain_j.t_stop -
-                          binned_spiketrain_i.t_stop) / bin_size
+            left_edge = (binned_spiketrain_j._t_start -
+                         binned_spiketrain_i._t_start) / bin_size
+            right_edge = (binned_spiketrain_j._t_stop -
+                          binned_spiketrain_i._t_stop) / bin_size
         else:
             # ex. 3) lags range: [-1, 3] ms
-            left_edge = (binned_spiketrain_j.t_stop -
-                         binned_spiketrain_i.t_stop) / bin_size
-            right_edge = (binned_spiketrain_j.t_start -
-                          binned_spiketrain_i.t_start) / bin_size
-        right_edge = int(right_edge.simplified.magnitude)
-        left_edge = int(left_edge.simplified.magnitude)
+            left_edge = (binned_spiketrain_j._t_stop -
+                         binned_spiketrain_i._t_stop) / bin_size
+            right_edge = (binned_spiketrain_j._t_start -
+                          binned_spiketrain_i._t_start) / bin_size
+        right_edge = int(right_edge)
+        left_edge = int(left_edge)
         lags = np.arange(left_edge, right_edge + 1, dtype=np.int32)
 
         return lags
 
     def correlate_memory(self, cch_mode):
         """
         Slow, but memory-safe mode.
 
         Return
         -------
         cross_corr : np.ndarray
             Cross-correlation of `self.binned_spiketrain1` and
             `self.binned_spiketrain2`.
         """
-        binned_spiketrain1 = self.binned_spiketrain_i
-        binned_spiketrain2 = self.binned_spiketrain_j
-
-        st1_spmat = self.binned_spiketrain_i._sparse_mat_u
-        st2_spmat = self.binned_spiketrain_j._sparse_mat_u
+        st1_spmat = self.binned_spiketrain_i.sparse_matrix
+        st2_spmat = self.binned_spiketrain_j.sparse_matrix
         left_edge, right_edge = self.window
 
         # extract the nonzero column indices of 1-d matrices
         st1_bin_idx_unique = st1_spmat.nonzero()[1]
         st2_bin_idx_unique = st2_spmat.nonzero()[1]
 
         # 'valid' mode requires bins correction due to the shift in t_starts
         # 'full' and 'pad' modes don't need this correction
         if cch_mode == "valid":
-            if binned_spiketrain1.n_bins > binned_spiketrain2.n_bins:
+            if self.binned_spiketrain_i.n_bins > \
+                    self.binned_spiketrain_j.n_bins:
                 st2_bin_idx_unique += right_edge
             else:
                 st2_bin_idx_unique += left_edge
 
         st1_spmat = st1_spmat.data
         st2_spmat = st2_spmat.data
 
@@ -217,16 +232,16 @@
         np.ndarray
             Normalized cross-correlation array in range `[-1, 1]`.
         """
         max_num_bins = max(self.binned_spiketrain_i.n_bins,
                            self.binned_spiketrain_j.n_bins)
         n_spikes1 = self.binned_spiketrain_i.get_num_of_spikes()
         n_spikes2 = self.binned_spiketrain_j.get_num_of_spikes()
-        data1 = self.binned_spiketrain_i._sparse_mat_u.data
-        data2 = self.binned_spiketrain_j._sparse_mat_u.data
+        data1 = self.binned_spiketrain_i.sparse_matrix.data
+        data2 = self.binned_spiketrain_j.sparse_matrix.data
         ii = data1.dot(data1)
         jj = data2.dot(data2)
         cov_mean = n_spikes1 * n_spikes2 / max_num_bins
         std_xy = np.sqrt((ii - n_spikes1 ** 2. / max_num_bins) * (
             jj - n_spikes2 ** 2. / max_num_bins))
         cross_corr_normalized = (cross_corr - cov_mean) / std_xy
         return cross_corr_normalized
@@ -342,15 +357,15 @@
     ...       rate=10.0*Hz, t_start=0.0*s, t_stop=10.0*s)
     >>> cov_matrix = covariance(BinnedSpikeTrain([st1, st2], bin_size=5*ms))
     >>> print(cov_matrix[0, 1])
     -0.001668334167083546
 
     """
     if binary:
-        binned_spiketrain = binned_spiketrain.binarize(copy=True)
+        binned_spiketrain = binned_spiketrain.binarize()
 
     if fast and binned_spiketrain.sparsity > _SPARSITY_MEMORY_EFFICIENT_THR:
         array = binned_spiketrain.to_array()
         return np.cov(array)
 
     return _covariance_sparse(
         binned_spiketrain, corrcoef_norm=False)
@@ -379,14 +394,18 @@
     However, if k-th spike train is empty, k-th row and k-th column of the
     returned matrix are set to np.nan.
 
     If binary is True, the binned spike trains are clipped to 0 or 1 before
     computing the correlation coefficients, so that the binned vectors
     :math:`b_i` and :math:`b_j` are binary.
 
+    Visualization of this function is covered in Viziphant:
+    :func:`viziphant.spike_train_correlation.plot_corrcoef`.
+
+
     Parameters
     ----------
     binned_spiketrain : (N, ) elephant.conversion.BinnedSpikeTrain
         A binned spike train containing the spike trains to be evaluated.
     binary : bool, optional
         If True, two spikes of a particular spike train falling in the same bin
         are counted as 1, resulting in binary binned vectors :math:`b_i`. If
@@ -442,15 +461,15 @@
     >>> cc_matrix = correlation_coefficient(BinnedSpikeTrain([st1, st2],
     ... bin_size=5*ms))
     >>> print(cc_matrix[0, 1])
     0.015477320222075359
 
     """
     if binary:
-        binned_spiketrain = binned_spiketrain.binarize(copy=True)
+        binned_spiketrain = binned_spiketrain.binarize()
 
     if fast and binned_spiketrain.sparsity > _SPARSITY_MEMORY_EFFICIENT_THR:
         array = binned_spiketrain.to_array()
         return np.corrcoef(array)
 
     return _covariance_sparse(
         binned_spiketrain, corrcoef_norm=True)
@@ -496,15 +515,15 @@
         If at least one row in `binned_spiketrain` is empty (has no spikes).
 
     Returns
     -------
     (N, N) np.ndarray
         Pearson correlation or covariance matrix.
     """
-    spmat = binned_spiketrain._sparse_mat_u
+    spmat = binned_spiketrain.sparse_matrix
     n_bins = binned_spiketrain.n_bins
 
     # Check for empty spike trains
     n_spikes_per_row = spmat.sum(axis=1)
     if n_spikes_per_row.min() == 0:
         warnings.warn(
             'Detected empty spike trains (rows) in the binned_spiketrain.')
@@ -528,14 +547,18 @@
         binned_spiketrain_i, binned_spiketrain_j, window='full',
         border_correction=False, binary=False, kernel=None, method='speed',
         cross_correlation_coefficient=False):
     """
     Computes the cross-correlation histogram (CCH) between two binned spike
     trains `binned_spiketrain_i` and `binned_spiketrain_j`.
 
+    Visualization of this function is covered in Viziphant:
+    :func:`viziphant.spike_train_correlation.plot_cross_correlation_histogram`.
+
+
     Parameters
     ----------
     binned_spiketrain_i, binned_spiketrain_j :
         elephant.conversion.BinnedSpikeTrain
         Binned spike trains of lengths N and M to cross-correlate. The input
         spike trains can have any `t_start` and `t_stop`.
     window : {'valid', 'full'} or list of int, optional
@@ -664,28 +687,32 @@
     >>> plt.axis('tight')
     >>> plt.show()
 
     """
 
     # Check that the spike trains are binned with the same temporal
     # resolution
-    if binned_spiketrain_i.matrix_rows != 1 or \
-            binned_spiketrain_j.matrix_rows != 1:
+    if binned_spiketrain_i.shape[0] != 1 or \
+            binned_spiketrain_j.shape[0] != 1:
         raise ValueError("Spike trains must be one dimensional")
-    if not np.isclose(binned_spiketrain_i.bin_size.simplified.item(),
-                      binned_spiketrain_j.bin_size.simplified.item()):
+
+    # rescale to the common units
+    # this does not change the data - only its representation
+    binned_spiketrain_j.rescale(binned_spiketrain_i.units)
+
+    if not np.isclose(binned_spiketrain_i._bin_size,
+                      binned_spiketrain_j._bin_size):
         raise ValueError("Bin sizes must be equal")
 
-    bin_size = binned_spiketrain_i.bin_size
+    bin_size = binned_spiketrain_i._bin_size
     left_edge_min = -binned_spiketrain_i.n_bins + 1
     right_edge_max = binned_spiketrain_j.n_bins - 1
 
-    t_lags_shift = (binned_spiketrain_j.t_start -
-                    binned_spiketrain_i.t_start) / bin_size
-    t_lags_shift = t_lags_shift.simplified.item()
+    t_lags_shift = (binned_spiketrain_j._t_start -
+                    binned_spiketrain_i._t_start) / bin_size
     if not np.isclose(t_lags_shift, round(t_lags_shift)):
         # For example, if bin_size=1 ms, binned_spiketrain_i.t_start=0 ms, and
         # binned_spiketrain_j.t_start=0.5 ms then there is a global shift in
         # the binning of the spike trains.
         raise ValueError(
             "Binned spiketrains time shift is not multiple of bin_size")
     t_lags_shift = int(round(t_lags_shift))
@@ -734,16 +761,16 @@
                                              binned_spiketrain_j)
         left_edge, right_edge = lags[(0, -1), ]
         cch_mode = window
     else:
         raise ValueError("Invalid window parameter")
 
     if binary:
-        binned_spiketrain_i = binned_spiketrain_i.binarize(copy=True)
-        binned_spiketrain_j = binned_spiketrain_j.binarize(copy=True)
+        binned_spiketrain_i = binned_spiketrain_i.binarize()
+        binned_spiketrain_j = binned_spiketrain_j.binarize()
 
     cch_builder = _CrossCorrHist(binned_spiketrain_i, binned_spiketrain_j,
                                  window=(left_edge, right_edge))
     if method == 'memory':
         cross_corr = cch_builder.correlate_memory(cch_mode=cch_mode)
     else:
         cross_corr = cch_builder.correlate_speed(cch_mode=cch_mode)
@@ -756,20 +783,29 @@
         else:
             cross_corr = cch_builder.border_correction(cross_corr)
     if kernel is not None:
         cross_corr = cch_builder.kernel_smoothing(cross_corr, kernel=kernel)
     if cross_correlation_coefficient:
         cross_corr = cch_builder.cross_correlation_coefficient(cross_corr)
 
+    normalization = 'normalized' if cross_correlation_coefficient else 'counts'
+    annotations = dict(window=window, border_correction=border_correction,
+                       binary=binary, kernel=kernel is not None,
+                       normalization=normalization)
+    annotations = dict(cch_parameters=annotations)
+
     # Transform the array count into an AnalogSignal
+    t_start = pq.Quantity((lags[0] - 0.5) * bin_size,
+                          units=binned_spiketrain_i.units, copy=False)
     cch_result = neo.AnalogSignal(
         signal=np.expand_dims(cross_corr, axis=1),
         units=pq.dimensionless,
-        t_start=(lags[0] - 0.5) * binned_spiketrain_i.bin_size,
-        sampling_period=binned_spiketrain_i.bin_size)
+        t_start=t_start,
+        sampling_period=binned_spiketrain_i.bin_size, copy=False,
+        **annotations)
     return cch_result, lags
 
 
 # Alias for common abbreviation
 cch = cross_correlation_histogram
 
 
@@ -957,17 +993,17 @@
         Maximal integration time :math:`\tau_{max}` of the auto-correlation
         function. It needs to be a multiple of the `bin_size` of
         `binned_spiketrain`.
 
     Returns
     -------
     timescale : pq.Quantity
-        The auto-correlation time of the binned spiketrain. If
-        `binned_spiketrain` has less than 2 spikes, a warning is raised and
-        `np.nan` is returned.
+        The auto-correlation time of the binned spiketrain with the same units
+        as in the input. If `binned_spiketrain` has less than 2 spikes, a
+        warning is raised and `np.nan` is returned.
 
     Notes
     -----
     * :math:`\tau_\mathrm{max}` is a critical parameter: numerical estimates
       of the auto-correlation functions are inherently noisy. Due to the
       square in the definition above, this noise is integrated. Thus, it is
       necessary to introduce a cutoff for the numerical integration - this
@@ -984,29 +1020,31 @@
         Physical Review E, 92(4), 040901.
     """
     if binned_spiketrain.get_num_of_spikes() < 2:
         warnings.warn("Spike train contains less than 2 spikes! "
                       "np.nan will be returned.")
         return np.nan
 
-    bin_size = binned_spiketrain.bin_size
-    if not (max_tau / bin_size).simplified.units == pq.dimensionless:
+    bin_size = binned_spiketrain._bin_size
+    try:
+        max_tau = max_tau.rescale(binned_spiketrain.units).item()
+    except (AttributeError, ValueError):
         raise ValueError("max_tau needs units of time")
 
     # safe casting of max_tau/bin_size to integer
-    max_tau_bins = int(np.round((max_tau / bin_size).simplified.magnitude))
-    if not np.isclose(max_tau.simplified.magnitude,
-                      (max_tau_bins * bin_size).simplified.magnitude):
+    max_tau_bins = int(round(max_tau / bin_size))
+    if not np.isclose(max_tau, max_tau_bins * bin_size):
         raise ValueError("max_tau has to be a multiple of the bin_size")
 
     cch_window = [-max_tau_bins, max_tau_bins]
     corrfct, bin_ids = cross_correlation_histogram(
         binned_spiketrain, binned_spiketrain, window=cch_window,
         cross_correlation_coefficient=True
     )
     # Take only t > 0 values, in particular neglecting the delta peak.
-    corrfct_pos = corrfct.time_slice(bin_size / 2, corrfct.t_stop).flatten()
+    start_id = corrfct.time_index((bin_size / 2) * binned_spiketrain.units)
+    corrfct = corrfct.magnitude.squeeze()[start_id:]
 
     # Calculate the timescale using trapezoidal integration
-    integr = np.abs((corrfct_pos / corrfct_pos[0]).magnitude)**2
+    integr = (corrfct / corrfct[0]) ** 2
     timescale = 2 * integrate.trapz(integr, dx=bin_size)
-    return timescale
+    return pq.Quantity(timescale, units=binned_spiketrain.units, copy=False)
```

### Comparing `elephant-0.8.0/elephant/spike_train_dissimilarity.py` & `elephant-0.9.0/elephant/spike_train_dissimilarity.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,21 @@
 spike train dissimilarity measures were introduced in the literature.
 They differ, e.g., by the properties of having the mathematical properties of
 a metric or by being time-scale dependent or not. Well known representatives
 of spike train dissimilarity measures are the Victor-Purpura distance and the
 Van Rossum distance implemented in this module, which both are metrics in the
 mathematical sense and time-scale dependent.
 
+
+.. autosummary::
+    :toctree: toctree/spike_train_dissimilarity
+
+    victor_purpura_distance
+    van_rossum_distance
+
 :copyright: Copyright 2016 by the Elephant team, see `doc/authors.rst`.
 :license: Modified BSD, see LICENSE.txt for details.
 """
 
 from __future__ import division, print_function, unicode_literals
 
 import warnings
@@ -21,14 +28,19 @@
 import quantities as pq
 import scipy as sp
 from neo.core import SpikeTrain
 
 import elephant.kernels as kernels
 from elephant.utils import deprecated_alias
 
+__all__ = [
+    "victor_purpura_distance",
+    "van_rossum_distance"
+]
+
 
 def _create_matrix_from_indexed_function(
         shape, func, symmetric_2d=False, **func_params):
     mat = np.empty(shape)
     if symmetric_2d:
         for i in range(shape[0]):
             for j in range(i, shape[1]):
```

### Comparing `elephant-0.8.0/elephant/spike_train_generation.py` & `elephant-0.9.0/elephant/spike_train_generation.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,14 +18,25 @@
 import neo
 import numpy as np
 import quantities as pq
 
 from elephant.spike_train_surrogates import dither_spike_train
 from elephant.utils import deprecated_alias
 
+__all__ = [
+    "spike_extraction",
+    "threshold_detection",
+    "peak_detection",
+    "homogeneous_poisson_process",
+    "inhomogeneous_poisson_process",
+    "homogeneous_gamma_process",
+    "single_interaction_process",
+    "compound_poisson_process"
+]
+
 
 @deprecated_alias(extr_interval='interval')
 def spike_extraction(signal, threshold=0.0 * pq.mV, sign='above',
                      time_stamps=None, interval=(-2 * pq.ms, 4 * pq.ms)):
     """
     Return the peak times for all events that cross threshold and the
     waveforms. Usually used for extracting spikes from a membrane
@@ -648,15 +659,98 @@
     rate = b / a
     theta = 1. / b.magnitude
     interval_generator = partial(np.random.gamma, shape=a, scale=theta)
     return _homogeneous_process(interval_generator, rate, t_start,
                                 t_stop, as_array)
 
 
-def _n_poisson(rate, t_stop, t_start=0.0 * pq.ms, n=1):
+def inhomogeneous_gamma_process(rate, shape_factor, as_array=False):
+    """
+    Returns a spike train whose spikes are a realization of an inhomogeneous
+    Gamma process with the given rate profile and the given shape factor.
+    The implementation using operational time is inspired by Nawrot et al.
+    (2018) [1]_.
+
+    Parameters
+    ----------
+    rate : neo.AnalogSignal
+        A `neo.AnalogSignal` representing the rate profile evolving over time.
+        Its values have all to be `>=0`. The output spiketrain will have
+        `t_start = rate.t_start` and `t_stop = rate.t_stop`
+    shape_factor : float
+        The shape factor of the Gamma process
+    as_array : bool, optional
+        If True, a NumPy array of sorted spikes is returned,
+        rather than a SpikeTrain object.
+        Default: False.
+
+    Returns
+    -------
+    spiketrain : neo.SpikeTrain or np.ndarray
+        Inhomogeneous Poisson process realization, of type `neo.SpikeTrain`
+        if `as_array` is False (default) and `np.ndarray` otherwise.
+
+    Raises
+    ------
+    ValueError
+        If `rate` is not a neo AnalogSignal
+        If `rate` contains a negative value.
+
+    References
+    ----------
+    .. [1] Nawrot, M., Boucsein, C., Denker, M., Rodriguez Molina, V.,
+           Riehle A., Aertsen A., & Rotter, S. (2008). Measurement of
+           variability dynamics in cortical spike trains. Journal of
+           Neuroscience Methods, 169, 374–390.
+    """
+
+    if not isinstance(rate, neo.AnalogSignal):
+        raise ValueError('rate must be a neo AnalogSignal')
+
+    # Check rate contains only positive values
+    if np.any(rate < 0) or rate.size == 0:
+        raise ValueError(
+            'rate must be a positive non empty signal, representing the'
+            'rate at time t')
+
+    # Operational time corresponds to the integral of the firing rate over time
+    operational_time = np.cumsum(
+        (rate*rate.sampling_period).simplified.magnitude)
+    operational_time = np.hstack((0., operational_time))
+
+    # The time points at which the firing rates are given
+    real_time = np.hstack((rate.times.simplified.magnitude,
+                           rate.t_stop.simplified.magnitude))
+
+    spiketrain_operational_time = homogeneous_gamma_process(
+        a=shape_factor, b=shape_factor*1.*pq.Hz,
+        t_start=0.*pq.s, t_stop=operational_time[-1]*pq.s, as_array=True)
+
+    # indices where between which points in operational time the spikes lie
+    indices = np.searchsorted(operational_time, spiketrain_operational_time)
+
+    # In real time the spikes are first aligned to the left border of the bin.
+    # Note that indices are greater than 0 because 'operational_time' was
+    # padded with zeros.
+    spiketrain = real_time[indices - 1]
+    # the relative position of the spikes in the operational time bins
+    positions_in_bins = \
+        (spiketrain_operational_time - operational_time[indices-1]) / (
+            operational_time[indices]-operational_time[indices-1])
+    # add the positions in the bin times the sampling period in real time
+    spiketrain += rate.sampling_period.simplified.magnitude * positions_in_bins
+
+    if as_array:
+        return spiketrain
+
+    return neo.SpikeTrain(spiketrain, units=pq.s, t_stop=rate.t_stop)
+
+
+@deprecated_alias(n='n_spiketrains')
+def _n_poisson(rate, t_stop, t_start=0.0 * pq.ms, n_spiketrains=1):
     """
     Generates one or more independent Poisson spike trains.
 
     Parameters
     ----------
     rate : pq.Quantity scalar or pq.Quantity array
         Expected firing rate (frequency) of each output SpikeTrain.
@@ -666,15 +760,15 @@
         *  a pq.Quantity array: rate[i] is the expected firing rate of the i-th
            output SpikeTrain
     t_stop : pq.Quantity
         Single common stop time of each output SpikeTrain. Must be > t_start.
     t_start : pq.Quantity, optional
         Single common start time of each output SpikeTrain. Must be < t_stop.
         Default: 0 * pq.ms
-    n: int, optional
+    n_spiketrains: int, optional
         If rate is a single pq.Quantity value, n specifies the number of
         SpikeTrains to be generated. If rate is an array, n is ignored and the
         number of SpikeTrains is equal to len(rate).
         Default: 1
 
 
     Returns
@@ -692,26 +786,27 @@
         rate.rescale(pq.Hz)
     except ValueError:
         raise ValueError('rate argument must have rate unit (1/time)')
 
     # Check t_start < t_stop and create their strip dimensions
     if not t_start < t_stop:
         raise ValueError(
-            't_start (=%s) must be < t_stop (=%s)' % (t_start, t_stop))
+            't_start (={}) must be < t_stop (={})'.format(t_start, t_stop))
 
     # Set number n of output spike trains (specified or set to len(rate))
-    if not (isinstance(n, int) and n > 0):
-        raise ValueError('n (=%s) must be a positive integer' % str(n))
+    if not (isinstance(n_spiketrains, int) and n_spiketrains > 0):
+        raise ValueError(
+            'n (={}) must be a positive integer'.format(str(n_spiketrains)))
     rate_dl = rate.simplified.magnitude.flatten()
 
     # Check rate input parameter
     if len(rate_dl) == 1:
         if rate_dl < 0:
-            raise ValueError('rate (=%s) must be non-negative.' % rate)
-        rates = np.array([rate_dl] * n)
+            raise ValueError('rate (={}) must be non-negative.'.format(rate))
+        rates = np.array([rate_dl] * n_spiketrains)
     else:
         rates = rate_dl.flatten()
         if any(rates < 0):
             raise ValueError('rate must have non-negative elements.')
 
     return [homogeneous_poisson_process(rate * pq.Hz, t_start, t_stop)
             for rate in rates]
@@ -1206,15 +1301,15 @@
     Parameters
     ----------
     rate : pq.Quantity
         Average rate of each spike train generated. Can be:
           - a single value, all spike trains will have same rate rate
           - an array of values (of length len(A)-1), each indicating the
             firing rate of one process in output
-    amplitude_distribution : np.ndarray
+    amplitude_distribution : np.ndarray or list
         CPP's amplitude distribution :math:`A`. `A[j]` represents the
         probability of a synchronous event of size `j` among the generated
         spike trains. The sum over all entries of :math:`A` must be equal to
         one.
     t_stop : pq.Quantity
         The end time of the output spike trains.
     shift : pq.Quantity, optional
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `elephant-0.8.0/elephant/spike_train_surrogates.py` & `elephant-0.9.0/elephant/spike_train_surrogates.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,69 +1,91 @@
 # -*- coding: utf-8 -*-
 """
 Module to generate surrogates of a spike train by randomising its spike times
-in different ways (see [1]). Different methods destroy different features of
-the original data:
+in different ways (see [2]_ and [3]_). Different methods destroy different
+features of the original data:
 
 * randomise_spikes:
     randomly reposition all spikes inside the time interval (t_start, t_stop).
     Keeps spike count, generates Poisson spike trains with time-stationary
     firing rate
 * dither_spikes:
     dither each spike time around original position by a random amount;
     keeps spike count and firing rates computed on a slow temporal scale;
     destroys ISIs, making them more exponentially distributed
 * dither_spike_train:
     dither the whole input spike train (i.e. all spikes equally) by a random
     amount; keeps spike count, ISIs, and firing rates computed on a slow
     temporal scale
 * jitter_spikes:
-    discretise the full time interval (t_start, t_stop) into time segments
+    discretize the full time interval (t_start, t_stop) into time segments
     and locally randomise the spike times (see randomise_spikes) inside each
     segment. Keeps spike count inside each segment and creates locally Poisson
     spike trains with locally time-stationary rates
 * shuffle_isis:
     shuffle the inter-spike intervals (ISIs) of the spike train randomly,
     keeping the first spike time fixed and generating the others from the
     new sequence of ISIs. Keeps spike count and ISIs, flattens the firing rate
     profile
 * joint_isi_dithering:
     calculate the Joint-ISI distribution and moves spike according to the
     probability distribution, that results from a fixed sum of ISI_before
-    and the ISI_afterwards. For further details see [1].
+    and the ISI_afterwards. For further details see [1]_ and [2]_.
+* bin_shuffling:
+    shuffles the bins of a binned spiketrain inside of exclusive windows.
+* trial_shifting:
+    shifts each trial, i.e., each element of a list of spiketrains by a
+    uniformly drawn random amount.
 
 References
 ----------
-[1] Louis et al (2010). Surrogate Spike Train Generation Through Dithering in
-    Operational Time. Front Comput Neurosci. 2010; 4: 127.
-[2] Gerstein, G. L. (2004). Searching for significance in spatio-temporal
-    firing patterns. Acta Neurobiologiae Experimentalis, 64(2), 203-208.
+.. [1] Gerstein, G. L. (2004). Searching for significance in spatio-temporal
+   firing patterns. Acta Neurobiol. Exp., 64:203–207.
+.. [2] Louis, S., Gerstein, G. L., Gruen, S., and Diesmann, M. (2010).
+   Surrogate spike train generation through dithering in operational time.
+   Front. Comput. Neurosci., 4(127).
+.. [3] Louis, S., Borgelt, C., and Gruen, S. (2010). Generation and selection
+   of surrogate methods for correlation analysis. In Rotter, S. and Gruen, S.,
+   editors, Analysis of Parallel Spike Trains. Springer, Berlin.
 
 Original implementation by: Emiliano Torre [e.torre@fz-juelich.de]
 :copyright: Copyright 2015-2016 by the Elephant team, see `doc/authors.rst`.
 :license: Modified BSD, see LICENSE.txt for details.
 """
 
 from __future__ import division, print_function, unicode_literals
 
 import random
 import warnings
+import copy
 
 import neo
 import numpy as np
 import quantities as pq
 from scipy.ndimage import gaussian_filter
 
 from elephant.statistics import isi
+import elephant.conversion as conv
 from elephant.utils import deprecated_alias
 
+__all__ = [
+    "dither_spikes",
+    "randomise_spikes",
+    "shuffle_isis",
+    "dither_spike_train",
+    "jitter_spikes",
+    "JointISI",
+    "surrogates"
+]
+
 # List of all available surrogate methods
-SURR_METHODS = ['dither_spike_train', 'dither_spikes', 'jitter_spikes',
+SURR_METHODS = ('dither_spike_train', 'dither_spikes', 'jitter_spikes',
                 'randomise_spikes', 'shuffle_isis', 'joint_isi_dithering',
-                'dither_spikes_with_refractory_period']
+                'dither_spikes_with_refractory_period', 'trial_shifting',
+                'bin_shuffling', 'isi_dithering')
 
 
 def _dither_spikes_with_refractory_period(spiketrain, dither, n_surrogates,
                                           refractory_period):
     units = spiketrain.units
     t_start = spiketrain.t_start.rescale(units).magnitude
     t_stop = spiketrain.t_stop.rescale(units).magnitude
@@ -121,19 +143,19 @@
 
     The surrogates retain the `spiketrain.t_start` and `spiketrain.t_stop`.
     Spikes moved beyond this range are lost or moved to the range's ends,
     depending on the parameter `edges`.
 
     Parameters
     ----------
-    spiketrain :  neo.SpikeTrain
+    spiketrain : neo.SpikeTrain
         The spike train from which to generate the surrogates.
     dither : pq.Quantity
         Amount of dithering. A spike at time `t` is placed randomly within
-        `]t-dither, t+dither[`.
+        `(t-dither, t+dither)`.
     n_surrogates : int, optional
         Number of surrogates to be generated.
         Default: 1.
     decimals : int or None, optional
         Number of decimal points for every spike time in the surrogates at a
         millisecond level.
         If None, machine precision is used.
@@ -148,16 +170,16 @@
         The dither range of each spike is adjusted such that the spike can not
         fall into the `refractory_period` of the previous or next spike.
         To account this, the refractory period is estimated as the smallest ISI
         of the spike train. The given argument `refractory_period` here is thus
         an initial estimation.
         Note, that with this option a spike cannot "jump" over the previous or
         next spike as it is normally possible.
-        If set to `None`, no refractoriness is in dithering.
-        Default: None
+        If set to None, no refractoriness is in dithering.
+        Default: None.
 
     Returns
     -------
     list of neo.SpikeTrain
         Each surrogate spike train obtained independently from `spiketrain` by
         randomly dithering its spikes. The range of the surrogate spike trains
         is the same as of `spiketrain`.
@@ -200,15 +222,15 @@
         dithered_spiketrains.sort(axis=1)
 
         if edges:
             # Leave out all spikes outside
             # [spiketrain.t_start, spiketrain.t_stop]
             dithered_spiketrains = \
                 [train[
-                     np.all([t_start < train, train < t_stop], axis=0)]
+                    np.all([t_start < train, train < t_stop], axis=0)]
                  for train in dithered_spiketrains]
         else:
             # Move all spikes outside
             # [spiketrain.t_start, spiketrain.t_stop] to the range's ends
             dithered_spiketrains = np.minimum(
                 np.maximum(dithered_spiketrains, t_start),
                 t_stop)
@@ -223,33 +245,33 @@
 
     # Round the surrogate data to decimal position, if requested
     if decimals is not None:
         dithered_spiketrains = \
             dithered_spiketrains.rescale(pq.ms).round(decimals).rescale(units)
 
     # Return the surrogates as list of neo.SpikeTrain
-    return [neo.SpikeTrain(
-        train, t_start=t_start, t_stop=t_stop)
+    return [neo.SpikeTrain(train, t_start=t_start, t_stop=t_stop,
+                           sampling_rate=spiketrain.sampling_rate)
             for train in dithered_spiketrains]
 
 
 @deprecated_alias(n='n_surrogates')
 def randomise_spikes(spiketrain, n_surrogates=1, decimals=None):
     """
     Generates surrogates of a spike train by spike time randomization.
 
     The surrogates are obtained by keeping the spike count of the original
     `spiketrain`, but placing the spikes randomly in the interval
     `[spiketrain.t_start, spiketrain.t_stop]`. The generated independent
-    neo.SpikeTrain objects follow  Poisson statistics (exponentially
+    `neo.SpikeTrain` objects follow  Poisson statistics (exponentially
     distributed inter-spike intervals).
 
     Parameters
     ----------
-    spiketrain :  neo.SpikeTrain
+    spiketrain : neo.SpikeTrain
         The spike train from which to generate the surrogates.
     n_surrogates : int, optional
         Number of surrogates to be generated.
         Default: 1.
     decimals : int or None, optional
         Number of decimal points for every spike time in the surrogates.
         If None, machine precision is used.
@@ -288,15 +310,16 @@
 
     # Round the surrogate data to decimal position, if requested
     if decimals is not None:
         sts = sts.round(decimals)
 
     # Convert the Quantity array to a list of SpikeTrains, and return them
     return [neo.SpikeTrain(np.sort(st), t_start=spiketrain.t_start,
-                           t_stop=spiketrain.t_stop)
+                           t_stop=spiketrain.t_stop,
+                           sampling_rate=spiketrain.sampling_rate)
             for st in sts]
 
 
 @deprecated_alias(n='n_surrogates')
 def shuffle_isis(spiketrain, n_surrogates=1, decimals=None):
     """
     Generates surrogates of a spike train by inter-spike-interval (ISI)
@@ -305,15 +328,15 @@
     The surrogates are obtained by randomly sorting the ISIs of the given input
     `spiketrain`. This generates independent `neo.SpikeTrain` object(s) with
     same ISI distribution and spike count as in `spiketrain`, while
     destroying temporal dependencies and firing rate profile.
 
     Parameters
     ----------
-    spiketrain :  neo.SpikeTrain
+    spiketrain : neo.SpikeTrain
         The spike train from which to generate the surrogates.
     n_surrogates : int, optional
         Number of surrogates to be generated.
         Default: 1.
     decimals : int or None, optional
         Number of decimal points for every spike time in the surrogates.
         If None, machine precision is used.
@@ -338,36 +361,40 @@
     >>> print(shuffle_isis(st, n_surrogates=2))  # doctest: +SKIP
         [<SpikeTrain(array([ 100.,  300.,  450.,  800.]) * ms,
               [0.0 ms, 1000.0 ms])>,
          <SpikeTrain(array([ 200.,  350.,  700.,  800.]) * ms,
               [0.0 ms, 1000.0 ms])>]
 
     """
-    if len(spiketrain) > 0:
-        isi0 = spiketrain[0] - spiketrain.t_start
-        ISIs = np.hstack([isi0, isi(spiketrain)])
-
-        # Round the isis to decimal position, if requested
-        if decimals is not None:
-            ISIs = ISIs.round(decimals)
-
-        # Create list of surrogate spike trains by random ISI permutation
-        sts = []
-        for surrogate_id in range(n_surrogates):
-            surr_times = np.cumsum(np.random.permutation(ISIs)) * \
-                spiketrain.units + spiketrain.t_start
-            sts.append(neo.SpikeTrain(
-                surr_times, t_start=spiketrain.t_start,
-                t_stop=spiketrain.t_stop))
+    if len(spiketrain) == 0:
+        return [neo.SpikeTrain([] * spiketrain.units,
+                               t_start=spiketrain.t_start,
+                               t_stop=spiketrain.t_stop,
+                               sampling_rate=spiketrain.sampling_rate)
+                for _ in range(n_surrogates)]
+
+    # A correct sorting is necessary, to calculate the ISIs
+    spiketrain = spiketrain.copy()
+    spiketrain.sort()
+    isi0 = spiketrain[0] - spiketrain.t_start
+    isis = np.hstack([isi0, isi(spiketrain)])
 
-    else:
-        sts = [neo.SpikeTrain([] * spiketrain.units,
-                              t_start=spiketrain.t_start,
-                              t_stop=spiketrain.t_stop)] * n_surrogates
+    # Round the isis to decimal position, if requested
+    if decimals is not None:
+        isis = isis.round(decimals)
 
+    # Create list of surrogate spike trains by random ISI permutation
+    sts = []
+    for surrogate_id in range(n_surrogates):
+        surr_times = np.cumsum(np.random.permutation(isis)) * \
+            spiketrain.units + spiketrain.t_start
+        sts.append(neo.SpikeTrain(
+            surr_times, t_start=spiketrain.t_start,
+            t_stop=spiketrain.t_stop,
+            sampling_rate=spiketrain.sampling_rate))
     return sts
 
 
 @deprecated_alias(n='n_surrogates')
 def dither_spike_train(spiketrain, shift, n_surrogates=1, decimals=None,
                        edges=True):
     """
@@ -380,27 +407,27 @@
 
     The surrogates retain the `spiketrain.t_start` and `spiketrain.t_stop`.
     Spikes moved beyond this range are lost or moved to the range's ends,
     depending on the parameter `edges`.
 
     Parameters
     ----------
-    spiketrain :  neo.SpikeTrain
+    spiketrain : neo.SpikeTrain
         The spike train from which to generate the surrogates.
     shift : pq.Quantity
         Amount of shift. `spiketrain` is shifted by a random amount uniformly
-        drawn from the range ]-shift, +shift[.
+        drawn from the range `(-shift, +shift)`.
     n_surrogates : int, optional
         Number of surrogates to be generated.
         Default: 1.
     decimals : int or None, optional
         Number of decimal points for every spike time in the surrogates.
         If None, machine precision is used.
         Default: None.
-    edges : bool
+    edges : bool, optional
         For surrogate spikes falling outside the range `[spiketrain.t_start,
         spiketrain.t_stop)`, whether to drop them out (for `edges = True`) or
         set them to the range's closest end (for `edges = False`).
         Default: True.
 
     Returns
     -------
@@ -431,15 +458,15 @@
     """
     # Transform spiketrain into a Quantity object (needed for matrix algebra)
     data = spiketrain.view(pq.Quantity)
 
     # Main: generate the surrogates by spike train shifting
     surr = data.reshape(
         (1, len(data))) + 2 * shift * np.random.random_sample(
-        (n_surrogates, 1)) - shift
+            (n_surrogates, 1)) - shift
 
     # Round the surrogate data to decimal position, if requested
     if decimals is not None:
         surr = surr.round(decimals)
 
     if edges is False:
         # Move all spikes outside [spiketrain.t_start, spiketrain.t_stop] to
@@ -452,15 +479,17 @@
         tstart, tstop = spiketrain.t_start.simplified.magnitude, \
             spiketrain.t_stop.simplified.magnitude
         surr = [np.sort(s[np.all([s >= tstart, s < tstop], axis=0)]) * pq.s
                 for s in surr.simplified.magnitude]
 
     # Return the surrogates as SpikeTrains
     return [neo.SpikeTrain(s, t_start=spiketrain.t_start,
-                           t_stop=spiketrain.t_stop).rescale(spiketrain.units)
+                           t_stop=spiketrain.t_stop,
+                           sampling_rate=spiketrain.sampling_rate
+                           ).rescale(spiketrain.units)
             for s in surr]
 
 
 @deprecated_alias(binsize='bin_size', n='n_surrogates')
 def jitter_spikes(spiketrain, bin_size, n_surrogates=1):
     """
     Generates surrogates of a spike train by spike jittering.
@@ -471,15 +500,15 @@
 
     The surrogates retain the `spiketrain.t_start` and `spiketrain.t_stop`.
     Note that within each time bin the surrogate spike trains are locally
     Poissonian (the inter-spike-intervals are exponentially distributed).
 
     Parameters
     ----------
-    spiketrain :  neo.SpikeTrain
+    spiketrain : neo.SpikeTrain
         The spike train from which to generate the surrogates.
     bin_size : pq.Quantity
         Size of the time bins within which to randomize the spike times.
         Note: the last bin lasts until `spiketrain.t_stop` and might have
         width different from `bin_size`.
     n_surrogates : int, optional
         Number of surrogates to be generated.
@@ -542,84 +571,157 @@
     dilats = np.array([bin_sizes_dl[bin_id] for bin_id in bin_ids])
 
     # Compute each surrogate by dilating and shifting each spike s in the
     # poisson 0-1 spike trains to dilat * s + offset. Attach time unit again
     surr = np.sort(surr_poiss01 * dilats + offsets, axis=1) * std_unit
 
     return [neo.SpikeTrain(s, t_start=spiketrain.t_start,
-                           t_stop=spiketrain.t_stop).rescale(spiketrain.units)
+                           t_stop=spiketrain.t_stop,
+                           sampling_rate=spiketrain.sampling_rate
+                           ).rescale(spiketrain.units)
             for s in surr]
 
 
-class JointISI(object):
+def bin_shuffling(
+        binned_spiketrain, max_displacement, n_surrogates=1, sliding=False):
     """
+    Bin shuffling surrogate generation.
+
+    The function shuffles the entries of a binned spike train entries inside
+    windows with a fixed maximal displacement. The windows are either exclusive
+    or sliding.
+
+    Parameters
+    ----------
+    binned_spiketrain : conv.BinnedSpikeTrain
+        The binned spiketrain to create surrogates of.
+    max_displacement : int
+        Number of bins that a single spike can be displaced.
+    n_surrogates : int, optional
+        Number of surrogates to create.
+        Default: 1.
+    sliding : bool, optional
+        If True, the window is slided bin by bin.
+        Default: False.
+
+    Returns
+    -------
+    binned_surrogates : list of conv.BinnedSpikeTrain
+        Each entry of the list is a binned surrogate spiketrain.
+    """
+    displacement_window = 2 * max_displacement
+
+    binned_spiketrain_bool = binned_spiketrain.to_bool_array()[0]
+    st_length = len(binned_spiketrain_bool)
+
+    surrogate_spiketrains = []
+    for surrogate_id in range(n_surrogates):
+        surrogate_spiketrain = np.copy(binned_spiketrain_bool)
+        if sliding:
+            for window_position in range(st_length - displacement_window):
+                # shuffling the binned spike train within the window
+                np.random.shuffle(
+                    surrogate_spiketrain[
+                        window_position:
+                        window_position + displacement_window])
+        else:
+            windows = st_length // displacement_window
+            windows_remainder = st_length % displacement_window
+            for window_position in range(windows):
+                # shuffling the binned spike train within the window
+                np.random.shuffle(
+                    surrogate_spiketrain[
+                        window_position * displacement_window:
+                        (window_position + 1) * displacement_window])
+            if windows_remainder != 0:
+                np.random.shuffle(
+                    surrogate_spiketrain[windows * displacement_window:])
+        surrogate_spiketrain = surrogate_spiketrain.reshape((1, st_length))
+
+        surrogate_spiketrains.append(
+            conv.BinnedSpikeTrain(
+                surrogate_spiketrain,
+                bin_size=binned_spiketrain.bin_size,
+                t_start=binned_spiketrain.t_start,
+                t_stop=binned_spiketrain.t_stop))
+    return surrogate_spiketrains
+
+
+class JointISI(object):
+    r"""
     The class :class:`JointISI` is implemented for Joint-ISI dithering
-    as a continuation of the ideas of Louis et al. (2010) and Gerstein (2004).
+    as a continuation of the ideas of [1]_ and [2]_.
 
     When creating a class instance, all necessary preprocessing steps are done
     to use :func:`JointISI.dithering` method.
 
     Parameters
     ----------
     spiketrain : neo.SpikeTrain
-        Input spiketrain to create surrogates from.
+        Input spiketrain to create surrogates of.
     dither : pq.Quantity, optional
         This quantity describes the maximum displacement of a spike, when
-        method is 'window'. It is also used for the uniform dithering for
+        `method` is 'window'. It is also used for the uniform dithering for
         the spikes, which are outside the regime in the Joint-ISI
         histogram, where Joint-ISI dithering is applicable.
         Default: 15. * pq.ms.
     truncation_limit : pq.Quantity, optional
         The Joint-ISI distribution of :math:`(ISI_i, ISI_{i+1})` is defined
-        within the range `[0, inf]`. Since this is computationally not
+        within the range :math:`[0, \infty)`. Since this is computationally not
         feasible, the Joint-ISI distribution is truncated for high ISI.
         The Joint-ISI histogram is calculated for
         :math:`(ISI_i, ISI_{i+1})` from 0 to `truncation_limit`.
-        Default: 100 * pq.ms.
+        Default: 100. * pq.ms.
     n_bins : int, optional
         The size of the joint-ISI-distribution will be
         `n_bins*n_bins/2`.
         Default: 100.
     sigma : pq.Quantity, optional
         The standard deviation of the Gaussian kernel, with which
         the data is convolved.
         Default: 2. * pq.ms.
-    alternate : boolean, optional
+    alternate : bool, optional
         If True, then all even spikes are dithered followed
         by all odd spikes. Otherwise, the spikes are dithered in ascending
         order from the first to the last spike.
         Default: True.
-    use_sqrt : boolean, optional
+    use_sqrt : bool, optional
         If True, the joint-ISI histogram is preprocessed by
-        applying a square root (following Gerstein et al. 2004).
+        applying a square root (following [1]).
         Default: False.
-    method : {'fast', window'}, optional
+    method : {'fast', 'window'}, optional
         * 'fast': the spike can move in the whole range between the
             previous and subsequent spikes (computationally efficient).
-        * 'window': the spike movement is limited to the parameter `dither`
-        Default: 'fast'.
-    cutoff : boolean, optional
+        * 'window': the spike movement is limited to the parameter `dither`.
+
+        Default: 'window'.
+    cutoff : bool, optional
         If True, then the filtering of the Joint-ISI histogram is
         limited on the lower side by the minimal ISI.
         This can be necessary, if in the data there is a certain refractory
         period, which will be destroyed by the convolution with the
         2d-Gaussian function.
         Default: True.
     refractory_period : pq.Quantity, optional
         Defines the refractory period of the dithered `spiketrain` unless
         the smallest ISI of the `spiketrain` is lower than this value.
         Default: 4. * pq.ms.
+    isi_dithering : bool, optional
+        If True, the Joint-ISI distribution is evaluated as the outer product
+        of the ISI-distribution with itself. Thus, all serial correlations are
+        destroyed.
+        Default: False.
 
-    Attributes
+    References
     ----------
-    max_change_index : np.ndarray or int:
-        For each ISI the corresponding index in the Joint-ISI distribution.
-    max_change_isi : np.ndarray or float:
-        The corresponding ISI for each index in :attr:`max_change_index`.
-
+    .. [1] Gerstein, G. L. (2004). Searching for significance in
+       spatio-temporal firing patterns. Acta Neurobiol. Exp., 64:203–207.
+    .. [2] Louis, S., Gerstein, G. L., Gruen, S., and Diesmann, M. (2010).
+       Surrogate spike train generation through dithering in operational time.
+       Front. Comput. Neurosci., 4(127).
     """
 
     # The min number of spikes, required for dithering.
     # Otherwise, the original spiketrain is copied N times.
     MIN_SPIKES = 3
 
     @deprecated_alias(num_bins='n_bins', refr_period='refractory_period')
@@ -627,281 +729,328 @@
                  spiketrain,
                  dither=15. * pq.ms,
                  truncation_limit=100. * pq.ms,
                  n_bins=100,
                  sigma=2. * pq.ms,
                  alternate=True,
                  use_sqrt=False,
-                 method='fast',
+                 method='window',
                  cutoff=True,
-                 refractory_period=4. * pq.ms
-                 ):
+                 refractory_period=4. * pq.ms,
+                 isi_dithering=False):
+
+        if not isinstance(spiketrain, neo.SpikeTrain):
+            raise TypeError('spiketrain must be of type neo.SpikeTrain')
+
+        # A correct sorting is necessary to calculate the ISIs
+        spiketrain = spiketrain.copy()
+        spiketrain.sort()
         self.spiketrain = spiketrain
-        self.truncation_limit = self.get_magnitude(truncation_limit)
+        self.truncation_limit = self._get_magnitude(truncation_limit)
         self.n_bins = n_bins
 
-        self.dither = self.get_magnitude(dither)
+        self.dither = self._get_magnitude(dither)
 
-        self.sigma = self.get_magnitude(sigma)
+        self.sigma = self._get_magnitude(sigma)
         self.alternate = alternate
 
-        if method not in ['fast', 'window']:
+        if method not in ('fast', 'window'):
             raise ValueError("The method can either be 'fast' or 'window', "
                              "but not '{}'".format(method))
         self.method = method
 
-        refractory_period = self.get_magnitude(refractory_period)
-        if not self.too_less_spikes:
+        refractory_period = self._get_magnitude(refractory_period)
+        if not self._too_less_spikes:
             minimal_isi = np.min(self.isi)
             refractory_period = min(refractory_period, minimal_isi)
         self.refractory_period = refractory_period
 
         self.cutoff = cutoff
         self.use_sqrt = use_sqrt
         self._jisih_cumulatives = None
 
-        self.max_change_index = self.isi_to_index(self.dither)
-        self.max_change_isi = self.index_to_isi(self.max_change_index)
+        self._max_change_index = self._isi_to_index(self.dither)
+        self._max_change_isi = self._index_to_isi(self._max_change_index)
+
+        self.isi_dithering = isi_dithering
 
     @property
     def refr_period(self):
         warnings.warn("'.refr_period' is deprecated; use '.refractory_period'",
                       DeprecationWarning)
         return self.refractory_period
 
     @property
     def num_bins(self):
         warnings.warn("'.num_bins' is deprecated; use '.n_bins'",
                       DeprecationWarning)
         return self.n_bins
 
-    def get_magnitude(self, quantity):
+    def _get_magnitude(self, quantity):
         """
         Parameters
         ----------
-        quantity: pq.Quantity or float
+        quantity : pq.Quantity or float
 
         Returns
         -------
-        float
+        magnitude : float
             The magnitude of `quantity`, rescaled to the units of the input
             :attr:`spiketrain`.
         """
         if isinstance(quantity, pq.Quantity):
-            return quantity.rescale(self.unit).magnitude
+            return quantity.rescale(self._unit).magnitude
         return quantity
 
     @property
-    def too_less_spikes(self):
+    def _too_less_spikes(self):
         """
         This is a check if the :attr:`spiketrain` has enough spikes to evaluate
         the joint-ISI histogram.
 
         Returns
         -------
         bool
+            If True, the spike train is so sparse, that this algorithm can't be
+            applied properly. Than in dithering() copies of the spiketrains are
+            returned.
         """
         return len(self.spiketrain) < self.MIN_SPIKES
 
     @property
-    def unit(self):
+    def _unit(self):
+        """
+        The unit of the spiketrain. Thus, the unit of the output surrogates.
+        """
         return self.spiketrain.units
 
     @property
     def isi(self):
-        if self.too_less_spikes:
+        """
+        The inter-spike intervals of the spiketrain.
+
+        Returns
+        -------
+        np.ndarray or None
+            An array of inter-spike intervals of the `spiketrain`.
+            None, if not enough spikes in the `spiketrain`.
+        """
+        if self._too_less_spikes:
             return None
         return isi(self.spiketrain.magnitude)
 
     @property
     def bin_width(self):
         return self.truncation_limit / self.n_bins
 
-    def isi_to_index(self, inter_spike_interval):
+    def _isi_to_index(self, inter_spike_interval):
         """
         A function that gives for each ISI the corresponding index in the
         Joint-ISI distribution.
 
         Parameters
         ----------
         inter_spike_interval : np.ndarray or float
             An array of ISIs or a single ISI.
 
         Returns
         -------
-        np.ndarray or int
-            The corresponding index for each ISI.
+        indices : np.ndarray or int
+            The corresponding indices/index for each ISI. When the input is an
+            array, also the output is.
         """
         return np.floor(inter_spike_interval / self.bin_width).astype(int)
 
-    def index_to_isi(self, isi_index):
+    def _index_to_isi(self, isi_index):
         """
         Maps `isi_index` back to the original ISI.
 
         Parameters
         ----------
         isi_index : np.ndarray or int
             The index of ISI.
 
         Returns
         -------
-        np.ndarray or float:
-            The corresponding ISI for each index.
+        np.ndarray or float
+            The corresponding ISI(s) for each indices/index. When the input is
+            an array, also the output is.
         """
         return (isi_index + 0.5) * self.bin_width
 
     def joint_isi_histogram(self):
         """
         Calculates a 2D histogram of :math:`(ISI_i, ISI_{i+1})` and applies
         square root or gaussian filtering if necessary.
 
         Returns
         -------
-        joint_isi_histogram : np.ndarray
+        joint_isi_histogram : np.ndarray or None
+            A np.ndarray with shape `n_bins` x `n_bins` containing the
+            joint-ISI histogram.
+            None, if not enough spikes in the `spiketrain`.
         """
-        if self.too_less_spikes:
+        if self._too_less_spikes:
             return None
         isis = self.isi
-        joint_isi_histogram = np.histogram2d(
-            isis[:-1], isis[1:],
-            bins=[self.n_bins, self.n_bins],
-            range=[[0., self.truncation_limit],
-                   [0., self.truncation_limit]])[0]
+        if not self.isi_dithering:
+            joint_isi_histogram = np.histogram2d(
+                isis[:-1], isis[1:],
+                bins=[self.n_bins, self.n_bins],
+                range=[[0., self.truncation_limit],
+                       [0., self.truncation_limit]])[0]
+        else:
+            isi_histogram = np.histogram(
+                isis,
+                bins=self.n_bins,
+                range=[0., self.truncation_limit])[0]
+            joint_isi_histogram = np.outer(isi_histogram, isi_histogram)
 
         if self.use_sqrt:
             joint_isi_histogram = np.sqrt(joint_isi_histogram)
 
         if self.sigma:
             if self.cutoff:
-                start_index = self.isi_to_index(self.refractory_period)
+                start_index = self._isi_to_index(self.refractory_period)
                 joint_isi_histogram[
                     start_index:, start_index:] = gaussian_filter(
                         joint_isi_histogram[start_index:, start_index:],
                         sigma=self.sigma / self.bin_width)
                 joint_isi_histogram[:start_index, :] = 0
                 joint_isi_histogram[:, :start_index] = 0
             else:
                 joint_isi_histogram = gaussian_filter(
                     joint_isi_histogram, sigma=self.sigma / self.bin_width)
         return joint_isi_histogram
 
     @staticmethod
-    def normalize_cumulative_distribution(array):
+    def _normalize_cumulative_distribution(array):
         """
-        This function normalizes parts of a cumulative distribution function
-        to be a cumulative distribution function again.
+        This function normalizes the cut-off of a cumulative distribution
+        function so that the first element is again zero and the last element
+        is one.
 
         Parameters
         ----------
-        array: np.ndarray
+        array : np.ndarray
             A monotonously increasing array as a part of an unnormalized
-             cumulative distribution function.
+            cumulative distribution function.
 
         Returns
         -------
         np.ndarray
             Monotonously increasing array from 0 to 1.
+            If `array` does not contain all equal elements, a only-zeros array
+            is returned.
         """
         if array[-1] - array[0] > 0.:
             return (array - array[0]) / (array[-1] - array[0])
         return np.zeros_like(array)
 
     def dithering(self, n_surrogates=1):
         """
         Implementation of Joint-ISI-dithering for spike trains that pass the
         threshold of the dense rate. If not, a uniform dithered spike train is
-        given back. The implementation continued the ideas of Louis et al.
-        (2010) and Gerstein (2004).
+        given back.
 
         Parameters
         ----------
-        n_surrogates: int
+        n_surrogates : int
             The number of dithered spiketrains to be returned.
             Default: 1.
 
         Returns
         ----------
-        dithered_sts: list of neo.SpikeTrain
+        dithered_sts : list of neo.SpikeTrain
             Spike trains, that are dithered versions of the given
-            :attr:`spiketrain`
+            :attr:`spiketrain`.
         """
-        if self.too_less_spikes:
+        if self._too_less_spikes:
             return [self.spiketrain] * n_surrogates
 
         # Checks, whether the preprocessing is already done.
         if self._jisih_cumulatives is None:
             self._determine_cumulative_functions()
 
         dithered_sts = []
         isi_to_dither = self.isi
         for _ in range(n_surrogates):
             dithered_isi = self._get_dithered_isi(isi_to_dither)
 
             dithered_st = self.spiketrain[0].magnitude + \
                 np.r_[0., np.cumsum(dithered_isi)]
-            dithered_st = neo.SpikeTrain(dithered_st * self.unit,
+            sampling_rate = self.spiketrain.sampling_rate
+
+            # Due to rounding errors, the last spike may be above t_stop.
+            # If the case, this is set to t_stop.
+            if dithered_st[-1] > self.spiketrain.t_stop:
+                dithered_st[-1] = self.spiketrain.t_stop
+
+            dithered_st = neo.SpikeTrain(dithered_st * self._unit,
                                          t_start=self.spiketrain.t_start,
-                                         t_stop=self.spiketrain.t_stop)
+                                         t_stop=self.spiketrain.t_stop,
+                                         sampling_rate=sampling_rate)
             dithered_sts.append(dithered_st)
         return dithered_sts
 
     def _determine_cumulative_functions(self):
         rotated_jisih = np.rot90(self.joint_isi_histogram())
 
         if self.method == 'fast':
             self._jisih_cumulatives = []
             for double_index in range(self.n_bins):
                 # Taking anti-diagonals of the original joint-ISI histogram
                 diagonal = np.diagonal(
                     rotated_jisih, offset=-self.n_bins + double_index + 1)
-                jisih_cum = self.normalize_cumulative_distribution(
+                jisih_cum = self._normalize_cumulative_distribution(
                     np.cumsum(diagonal))
                 self._jisih_cumulatives.append(jisih_cum)
-            self._jisih_cumulatives = np.array(self._jisih_cumulatives)
+            self._jisih_cumulatives = np.array(
+                self._jisih_cumulatives, dtype=object)
         else:
             self._jisih_cumulatives = self._window_cumulatives(rotated_jisih)
 
     def _window_cumulatives(self, rotated_jisih):
         jisih_diag_cums = self._window_diagonal_cumulatives(rotated_jisih)
         jisih_cumulatives = np.zeros(
             (self.n_bins, self.n_bins,
-             2 * self.max_change_index + 1))
+             2 * self._max_change_index + 1))
         for curr_isi_id in range(self.n_bins):
             for next_isi_id in range(self.n_bins - curr_isi_id):
                 double_index = next_isi_id + curr_isi_id
                 cum_slice = jisih_diag_cums[
                     double_index,
-                    curr_isi_id: curr_isi_id + 2 * self.max_change_index + 1]
+                    curr_isi_id: curr_isi_id + 2 * self._max_change_index + 1]
 
-                normalized_cum = self.normalize_cumulative_distribution(
+                normalized_cum = self._normalize_cumulative_distribution(
                     cum_slice)
                 jisih_cumulatives[curr_isi_id][next_isi_id] = normalized_cum
         return jisih_cumulatives
 
     def _window_diagonal_cumulatives(self, rotated_jisih):
         # An element of the first axis is defined as the sum of indices
         # for previous and subsequent ISI.
 
         jisih_diag_cums = np.zeros((self.n_bins,
                                     self.n_bins
-                                    + 2 * self.max_change_index))
+                                    + 2 * self._max_change_index))
 
         # double_index corresponds to the sum of the indices for the previous
         # and the subsequent ISI.
         for double_index in range(self.n_bins):
             cum_diag = np.cumsum(np.diagonal(rotated_jisih,
                                              - self.n_bins
                                              + double_index + 1))
 
             right_padding = jisih_diag_cums.shape[1] - \
-                len(cum_diag) - self.max_change_index
+                len(cum_diag) - self._max_change_index
 
             jisih_diag_cums[double_index] = np.pad(
                 cum_diag,
-                pad_width=(self.max_change_index, right_padding),
+                pad_width=(self._max_change_index, right_padding),
                 mode='constant',
                 constant_values=(cum_diag[0], cum_diag[-1])
             )
 
         return jisih_diag_cums
 
     def _get_dithered_isi(self, isi_to_dither):
@@ -911,15 +1060,15 @@
         # dither the "even" ones and then the "odd" ones.
         # if alternate is false, we just go dither from the first to the last
         # spike, which corresponds to a sampling_rhythm of 1.
         sampling_rhythm = self.alternate + 1
         number_of_isis = len(dithered_isi)
 
         for start in range(sampling_rhythm):
-            dithered_isi_indices = self.isi_to_index(dithered_isi)
+            dithered_isi_indices = self._isi_to_index(dithered_isi)
             for i in range(start, number_of_isis - 1,
                            sampling_rhythm):
                 step = self._get_dithering_step(
                     dithered_isi,
                     dithered_isi_indices,
                     i)
                 dithered_isi[i] += step
@@ -934,25 +1083,25 @@
         curr_isi_id = dithered_isi_indices[i]
         next_isi_id = dithered_isi_indices[i + 1]
         double_index = curr_isi_id + next_isi_id
         if double_index < self.n_bins:
             if self.method == 'fast':
                 cum_dist_func = self._jisih_cumulatives[
                     double_index]
-                compare_isi = self.index_to_isi(curr_isi_id)
+                compare_isi = self._index_to_isi(curr_isi_id)
             else:
                 cum_dist_func = self._jisih_cumulatives[
                     curr_isi_id][next_isi_id]
-                compare_isi = self.max_change_isi
+                compare_isi = self._max_change_isi
 
             if cum_dist_func[-1] > 0.:
                 # when the method is 'fast', new_isi_id is where the current
                 # ISI id should go to.
                 new_isi_id = np.searchsorted(cum_dist_func, random.random())
-                step = self.index_to_isi(new_isi_id) - compare_isi
+                step = self._index_to_isi(new_isi_id) - compare_isi
                 return step
 
         return self._uniform_dither_not_jisi_movable_spikes(
             dithered_isi[i],
             dithered_isi[i + 1])
 
     def _uniform_dither_not_jisi_movable_spikes(self,
@@ -960,94 +1109,288 @@
                                                 next_isi):
         left_dither = min(curr_isi - self.refractory_period, self.dither)
         right_dither = min(next_isi - self.refractory_period, self.dither)
         step = random.random() * (right_dither + left_dither) - left_dither
         return step
 
 
+def trial_shifting(spiketrains, dither, n_surrogates=1):
+    """
+    Generates surrogates of a spike train by trial shifting.
+
+    It shifts by a random uniform amount independently different trials,
+    which are the elements of a list of spiketrains.
+
+    The shifting is done independently for each surrogate.
+
+    Parameters
+    ----------
+    spiketrains : list of neo.SpikeTrain
+        A list of spike trains of the same neuron
+        where each element corresponds to one trial.
+    dither : pq.Quantity
+        Amount of dithering.
+    n_surrogates : int, optional
+        Number of surrogates to be generated.
+        Default: 1.
+
+    Returns
+    -------
+    surrogate_spiketrains : list of list of neo.SpikeTrain
+        Each surrogate spike train obtained independently from `spiketrain` by
+        randomly dithering its spikes. The range of the surrogate spike trains
+        is the same as of `spiketrain`.
+    """
+    dither = dither.simplified.magnitude
+
+    units = spiketrains[0].units
+    t_starts = [single_trial_st.t_start.simplified.magnitude
+                for single_trial_st in spiketrains]
+    t_stops = [single_trial_st.t_stop.simplified.magnitude
+               for single_trial_st in spiketrains]
+    sampling_rates = [single_trial_st.sampling_rate
+                      for single_trial_st in spiketrains]
+    spiketrains = [single_trial_st.simplified.magnitude
+                   for single_trial_st in spiketrains]
+
+    surrogate_spiketrains = \
+        _trial_shifting(spiketrains, dither, t_starts, t_stops,
+                        n_surrogates)
+
+    surrogate_spiketrains = \
+        [[neo.SpikeTrain(
+            surrogate_spiketrain[trial_id] * pq.s,
+            t_start=t_starts[trial_id] * pq.s,
+            t_stop=t_stops[trial_id] * pq.s,
+            units=units,
+            sampling_rate=sampling_rates[trial_id])
+          for trial_id in range(len(surrogate_spiketrain))]
+         for surrogate_spiketrain in surrogate_spiketrains]
+
+    return surrogate_spiketrains
+
+
+def _trial_shifting(spiketrains, dither, t_starts, t_stops, n_surrogates):
+    """
+    Inner nucleus of the trial shuffling procedure.
+    """
+    surrogate_spiketrains = []
+    for surrogate_id in range(n_surrogates):
+        copied_spiketrain = copy.copy(spiketrains)
+        surrogate_spiketrain = []
+        # looping over all trials
+        for trial_id, single_trial_st in enumerate(copied_spiketrain):
+            single_trial_st += dither * (2 * random.random() - 1)
+            single_trial_st = np.remainder(
+                single_trial_st - t_starts[trial_id],
+                t_stops[trial_id] - t_starts[trial_id]
+            ) + t_starts[trial_id]
+            single_trial_st.sort()
+
+            surrogate_spiketrain.append(single_trial_st)
+
+        surrogate_spiketrains.append(surrogate_spiketrain)
+    return surrogate_spiketrains
+
+
+def _trial_shifting_of_concatenated_spiketrain(
+        spiketrain, dither, trial_length, trial_separation, n_surrogates=1):
+    """
+    Generates surrogates of a spike train by trial shifting.
+
+    It shifts by a random uniform amount independently different trials,
+    individuated by the `trial_length` and the possible buffering period
+    `trial_separation` present in between trials.
+
+    The shifting is done independently for each surrogate.
+
+    Parameters
+    ----------
+    spiketrain : neo.SpikeTrain
+        A single spike train, where the trials are concatenated.
+    dither : pq.Quantity
+        Amount of dithering.
+    trial_length : pq.Quantity
+        The length of the single-trial spiketrain.
+    trial_separation : pq.Quantity
+        Buffering in between trials in the concatenation of the spiketrain.
+    n_surrogates : int, optional
+        Number of surrogates to be generated.
+        Default: 1.
+
+    Returns
+    -------
+    surrogate_spiketrains : list of neo.SpikeTrain
+        Each surrogate spike train obtained independently from `spiketrain` by
+        randomly dithering its spikes. The range of the surrogate spike trains
+        is the same as of `spiketrain`.
+    """
+    units = spiketrain.units
+    t_start = spiketrain.t_start.simplified.magnitude
+    t_stop = spiketrain.t_stop.simplified.magnitude
+    trial_length = trial_length.simplified.magnitude
+    trial_separation = trial_separation.simplified.magnitude
+    dither = dither.simplified.magnitude
+    n_trials = int((t_stop - t_start) // (trial_length + trial_separation))
+    t_starts = t_start + \
+        np.arange(n_trials) * (trial_length + trial_separation)
+    t_stops = t_starts + trial_length
+    spiketrains = spiketrain.simplified.magnitude
+    spiketrains = [spiketrains[(spiketrains >= t_starts[trial_id]) &
+                               (spiketrains <= t_stops[trial_id])]
+                   for trial_id in range(n_trials)]
+
+    surrogate_spiketrains = _trial_shifting(
+        spiketrains, dither, t_starts, t_stops, n_surrogates)
+
+    surrogate_spiketrains = [neo.SpikeTrain(
+        np.hstack(surrogate_spiketrain) * pq.s,
+        t_start=t_start * pq.s,
+        t_stop=t_stop * pq.s,
+        units=units,
+        sampling_rate=spiketrain.sampling_rate)
+        for surrogate_spiketrain in surrogate_spiketrains]
+    return surrogate_spiketrains
+
+
 @deprecated_alias(n='n_surrogates', surr_method='method')
-def surrogates(spiketrain, n_surrogates=1, method='dither_spike_train',
-               dt=None, decimals=None, edges=True):
+def surrogates(
+        spiketrain, n_surrogates=1, method='dither_spike_train',
+        dt=None, **kwargs):
     """
     Generates surrogates of a `spiketrain` by a desired generation
     method.
 
     This routine is a wrapper for the other surrogate generators in the
     module.
 
     The surrogates retain the `spiketrain.t_start` and `spiketrain.t_stop` of
     the original `spiketrain`.
 
 
     Parameters
     ----------
-    spiketrain : neo.SpikeTrain
-        The spike train from which to generate the surrogates
+    spiketrain : neo.SpikeTrain or list of neo.SpikeTrain
+        The spike train from which to generate the surrogates.
+        The only method that accepts a list of spike trains instead of a single
+        spike train to generate the surrogates from is 'trial_shifting'.
     n_surrogates : int, optional
         Number of surrogates to be generated.
         Default: 1.
     method : str, optional
         The method to use to generate surrogate spike trains. Can be one of:
-        * 'dither_spike_train': see `surrogates.dither_spike_train` [dt needed]
-        * 'dither_spikes': see `surrogates.dither_spikes` [dt needed]
-        * 'jitter_spikes': see `surrogates.jitter_spikes` [dt needed]
-        * 'randomise_spikes': see `surrogates.randomise_spikes`
-        * 'shuffle_isis': see `surrogates.shuffle_isis`
-        * 'joint_isi_dithering': see `surrogates.joint_isi_dithering`
-        Default: 'dither_spike_train'.
+
+        * 'dither_spike_train': see `surrogates.dither_spike_train()`
+            [`dt` needed]
+        * 'dither_spikes': see `surrogates.dither_spikes()` [`dt` needed]
+        * 'jitter_spikes': see `surrogates.jitter_spikes()` [`dt` needed]
+        * 'randomise_spikes': see `surrogates.randomise_spikes()`
+        * 'shuffle_isis': see `surrogates.shuffle_isis()`
+        * 'joint_isi_dithering': see `surrogates.joint_isi_dithering()`
+            [`dt` needed]
+        * 'trial_shifting': see `surrogates.trial_shifting` [`dt` needed]
+            If used on a neo.SpikeTrain, specify the key-word argument
+            `trial_length` and `trial_separation` of type pq.Quantity.
+            Else, `spiketrain` has to be a list of neo.SpikeTrain.
+        * 'bin_shuffling': see `surrogates.bin_shuffling()` [`dt` needed]
+            If used in this module, specify the key-word argument `bin_size`
+            of type pq.Quantity.
+
+        Default: 'dither_spike_train'
     dt : pq.Quantity, optional
-        For methods shifting spike times randomly around their original time
+        For methods shifting spike times or spike trains randomly around
+        their original time
         (`dither_spikes`, `dither_spike_train`) or replacing them randomly
         within a certain window (`jitter_spikes`), dt represents the size of
         that shift / window. For other methods, dt is ignored.
         Default: None.
-    decimals : int or None, optional
-        Number of decimal points for every spike time in the surrogates
-        If None, machine precision is used.
-        Default: None.
-    edges : bool
-        For surrogate spikes falling outside the range `[spiketrain.t_start,
-        spiketrain.t_stop)`, whether to drop them out (for `edges = True`) or
-        set them to the range's closest end (for `edges = False`).
-        Default: True.
+    kwargs
+        Keyword arguments passed to the chosen surrogate method.
 
     Returns
     -------
     list of neo.SpikeTrain
         Each surrogate spike train obtained independently from `spiketrain`
         according to chosen surrogate type. The time range of the surrogate
         spike trains is the same as in `spiketrain`.
+
+    Raises
+    ------
+    TypeError
+        If `spiketrain` is not either a `neo.SpikeTrain` object or a list of
+        `neo.SpikeTrain`.
+
+    ValueError
+        If `method` is not one of the surrogate methods defined in this module.
+
+        If `dt` is None and `method` is not 'randomise_spikes' nor
+        'shuffle_isis'.
     """
 
-    if not isinstance(spiketrain, neo.SpikeTrain):
-        raise ValueError("spiketrain must be of instance neo.SpikeTrain")
+    if isinstance(spiketrain, list):
+        if not isinstance(spiketrain[0], neo.SpikeTrain):
+            raise TypeError('spiketrain must be an instance neo.SpikeTrain or'
+                            ' a list of neo.SpikeTrain')
+    elif not isinstance(spiketrain, neo.SpikeTrain):
+        raise TypeError('spiketrain must be an instance neo.SpikeTrain or'
+                        ' a list of neo.SpikeTrain')
 
     # Define the surrogate function to use, depending on the specified method
     surrogate_types = {
         'dither_spike_train': dither_spike_train,
         'dither_spikes': dither_spikes,
+        'dither_spikes_with_refractory_period': dither_spikes,
         'jitter_spikes': jitter_spikes,
         'randomise_spikes': randomise_spikes,
         'shuffle_isis': shuffle_isis,
-        'joint_isi_dithering': JointISI(spiketrain).dithering,
+        'bin_shuffling': bin_shuffling,
+        'trial_shifting': trial_shifting,
+        'joint_isi_dithering': lambda n: JointISI(
+            spiketrain, **kwargs).dithering(n),
+        'isi_dithering': lambda n: JointISI(
+            spiketrain, isi_dithering=True, **kwargs).dithering(n)
     }
 
     if method not in surrogate_types.keys():
         raise ValueError("Specified surrogate method ('{}') "
                          "is not valid".format(method))
     method = surrogate_types[method]
 
     # PYTHON2: replace with inspect.signature()
-    if dt is None and method in (dither_spike_train, dither_spikes,
-                                 jitter_spikes):
+    if dt is None and method not in (randomise_spikes, shuffle_isis):
         raise ValueError("{}() method requires 'dt' parameter to be "
                          "not None".format(method.__name__))
 
     if method in (dither_spike_train, dither_spikes):
-        return method(spiketrain, dt, n=n_surrogates, decimals=decimals,
-                      edges=edges)
+        return method(
+            spiketrain, dt, n_surrogates=n_surrogates, **kwargs)
     if method in (randomise_spikes, shuffle_isis):
-        return method(spiketrain, n=n_surrogates, decimals=decimals)
-    if method == jitter_spikes:
-        return method(spiketrain, dt, n=n_surrogates)
-    # method == 'joint_isi_dithering':
+        return method(spiketrain, n_surrogates=n_surrogates, **kwargs)
+    if method is jitter_spikes:
+        return method(spiketrain, dt, n_surrogates=n_surrogates)
+    if method is trial_shifting:
+        if isinstance(spiketrain, list):
+            return method(
+                spiketrain, dither=dt, n_surrogates=n_surrogates)
+        return _trial_shifting_of_concatenated_spiketrain(
+            spiketrain, dither=dt, n_surrogates=n_surrogates, **kwargs)
+    if method is bin_shuffling:
+        binned_spiketrain = conv.BinnedSpikeTrain(
+            spiketrain, bin_size=kwargs['bin_size'])
+        bin_size = binned_spiketrain._bin_size
+        # bin_centers share the same units as bin_size
+        bin_grid = binned_spiketrain.bin_centers.magnitude
+        max_displacement = int(
+            dt.rescale(binned_spiketrain.units).item() / bin_size)
+        binned_surrogates = bin_shuffling(binned_spiketrain,
+                                          max_displacement=max_displacement,
+                                          n_surrogates=n_surrogates)
+        surrogate_spiketrains = \
+            [neo.SpikeTrain(bin_grid[binned_surr.sparse_matrix.nonzero()[1]],
+                            t_start=spiketrain.t_start,
+                            t_stop=spiketrain.t_stop,
+                            units=binned_spiketrain.units,
+                            sampling_rate=spiketrain.sampling_rate)
+             for binned_surr in binned_surrogates]
+        return surrogate_spiketrains
+    # surr_method is 'joint_isi_dithering' or isi_dithering:
     return method(n_surrogates)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `elephant-0.8.0/elephant/sta.py` & `elephant-0.9.0/elephant/sta.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,19 @@
 import numpy as np
 import scipy.signal
 import quantities as pq
 from neo.core import AnalogSignal, SpikeTrain
 import warnings
 from .conversion import BinnedSpikeTrain
 
+__all__ = [
+    "spike_triggered_average",
+    "spike_field_coherence"
+]
+
 
 def spike_triggered_average(signal, spiketrains, window):
     """
     Calculates the spike-triggered averages of analog signals in a time window
     relative to the spike times of a corresponding spiketrain for multiple
     signals each. The function receives n analog signals and either one or
     n spiketrains. In case it is one spiketrain this one is muliplied n-fold
```

### Comparing `elephant-0.8.0/elephant/statistics.py` & `elephant-0.9.0/elephant/statistics.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,27 +25,28 @@
 
 .. autosummary::
     :toctree: toctree/statistics/
 
     mean_firing_rate
     instantaneous_rate
     time_histogram
-    sskernel
+    optimal_kernel_bandwidth
 
 
 Spike interval statistics
 ~~~~~~~~~~~~~~~~~~~~~~~~~
 
 .. autosummary::
     :toctree: toctree/statistics/
 
     isi
     cv
-    lv
     cv2
+    lv
+    lvr
 
 
 Statistics across spike trains
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 .. autosummary::
     :toctree: toctree/statistics/
@@ -67,53 +68,81 @@
 import numpy as np
 import math
 import quantities as pq
 import scipy.signal
 import scipy.stats
 from neo.core import SpikeTrain
 
-import elephant.conversion as conv
 import elephant.kernels as kernels
-from elephant.utils import deprecated_alias
+from elephant.conversion import BinnedSpikeTrain
+from elephant.utils import deprecated_alias, get_common_start_stop_times, \
+    check_neo_consistency
 
 from elephant.utils import is_time_quantity
 
+__all__ = [
+    "isi",
+    "mean_firing_rate",
+    "fanofactor",
+    "cv",
+    "cv2",
+    "lv",
+    "lvr",
+    "instantaneous_rate",
+    "time_histogram",
+    "complexity_pdf",
+    "fftkernel",
+    "optimal_kernel_bandwidth"
+]
+
 cv = scipy.stats.variation
 
 
 def isi(spiketrain, axis=-1):
     """
     Return an array containing the inter-spike intervals of the spike train.
 
-    Accepts a `neo.SpikeTrain`, a `pq.Quantity` array, or a plain
-    `np.ndarray`. If either a `neo.SpikeTrain` or `pq.Quantity` is provided,
-    the return value will be `pq.Quantity`, otherwise `np.ndarray`. The units
-    of `pq.Quantity` will be the same as `spiketrain`.
+    Accepts a `neo.SpikeTrain`, a `pq.Quantity` array, a `np.ndarray`, or a
+    list of time spikes. If either a `neo.SpikeTrain` or `pq.Quantity` is
+    provided, the return value will be `pq.Quantity`, otherwise `np.ndarray`.
+    The units of `pq.Quantity` will be the same as `spiketrain`.
+
+    Visualization of this function is covered in Viziphant:
+    :func:`viziphant.statistics.plot_isi_histogram`.
 
     Parameters
     ----------
-    spiketrain : neo.SpikeTrain or pq.Quantity or np.ndarray
+    spiketrain : neo.SpikeTrain or pq.Quantity or array-like
         The spike times.
     axis : int, optional
         The axis along which the difference is taken.
         Default: the last axis.
 
     Returns
     -------
     intervals : np.ndarray or pq.Quantity
         The inter-spike intervals of the `spiketrain`.
 
+    Warns
+    -----
+    UserWarning
+        When the input array is not sorted, negative intervals are returned
+        with a warning.
+
     """
-    if axis is None:
-        axis = -1
     if isinstance(spiketrain, neo.SpikeTrain):
-        intervals = np.diff(
-            np.sort(spiketrain.times.view(pq.Quantity)), axis=axis)
+        intervals = np.diff(spiketrain.magnitude, axis=axis)
+        # np.diff makes a copy
+        intervals = pq.Quantity(intervals, units=spiketrain.units, copy=False)
     else:
-        intervals = np.diff(np.sort(spiketrain), axis=axis)
+        intervals = np.diff(spiketrain, axis=axis)
+    if (intervals < 0).any():
+        warnings.warn("ISI evaluated to negative values. "
+                      "Please sort the input array.")
+
     return intervals
 
 
 def mean_firing_rate(spiketrain, t_start=None, t_stop=None, axis=None):
     """
     Return the firing rate of the spike train.
 
@@ -218,15 +247,15 @@
         return rates
     else:
         raise TypeError("Invalid input spiketrain type: '{}'. Allowed: "
                         "neo.SpikeTrain, Quantity, ndarray".
                         format(type(spiketrain)))
 
 
-def fanofactor(spiketrains):
+def fanofactor(spiketrains, warn_tolerance=0.1 * pq.ms):
     r"""
     Evaluates the empirical Fano factor F of the spike counts of
     a list of `neo.SpikeTrain` objects.
 
     Given the vector v containing the observed spike counts (one per
     spike train) in the time window [t0, t1], F is defined as:
 
@@ -239,31 +268,61 @@
     Poisson process, F=1.
 
     Parameters
     ----------
     spiketrains : list
         List of `neo.SpikeTrain` or `pq.Quantity` or `np.ndarray` or list of
         spike times for which to compute the Fano factor of spike counts.
+    warn_tolerance : pq.Quantity
+        In case of a list of input neo.SpikeTrains, if their durations vary by
+        more than `warn_tolerence` in their absolute values, throw a warning
+        (see Notes).
+        Default: 0.1 ms.
 
     Returns
     -------
     fano : float
         The Fano factor of the spike counts of the input spike trains.
         Returns np.NaN if an empty list is specified, or if all spike trains
         are empty.
 
+    Raises
+    ------
+    TypeError
+        If the input spiketrains are neo.SpikeTrain objects, but
+        `warn_tolerance` is not a quantity.
+
+    Notes
+    -----
+    The check for the equal duration of the input spike trains is performed
+    only if the input is of type`neo.SpikeTrain`: if you pass a numpy array,
+    please make sure that they all have the same duration manually.
     """
     # Build array of spike counts (one per spike train)
-    spike_counts = np.array([len(t) for t in spiketrains])
+    spike_counts = np.array([len(st) for st in spiketrains])
 
     # Compute FF
     if all(count == 0 for count in spike_counts):
-        fano = np.nan
-    else:
-        fano = spike_counts.var() / spike_counts.mean()
+        # empty list of spiketrains reaches this branch, and NaN is returned
+        return np.nan
+
+    if all(isinstance(st, neo.SpikeTrain) for st in spiketrains):
+        if not is_time_quantity(warn_tolerance):
+            raise TypeError("'warn_tolerance' must be a time quantity.")
+        durations = [(st.t_stop - st.t_start).simplified.item()
+                     for st in spiketrains]
+        durations_min = min(durations)
+        durations_max = max(durations)
+        if durations_max - durations_min > warn_tolerance.simplified.item():
+            warnings.warn("Fano factor calculated for spike trains of "
+                          "different duration (minimum: {_min}s, maximum "
+                          "{_max}s).".format(_min=durations_min,
+                                             _max=durations_max))
+
+    fano = spike_counts.var() / spike_counts.mean()
     return fano
 
 
 def __variation_check(v, with_nan):
     # ensure the input ia a vector
     if v.ndim != 1:
         raise ValueError("The input must be a vector, not a {}-dim matrix.".
@@ -281,60 +340,130 @@
                              "an input with more than 1 entry. Set 'with_nan' "
                              "to True to replace the error by a warning.")
 
     return None
 
 
 @deprecated_alias(v='time_intervals')
+def cv2(time_intervals, with_nan=False):
+    r"""
+    Calculate the measure of Cv2 for a sequence of time intervals between
+    events.
+
+    Given a vector :math:`I` containing a sequence of intervals, the Cv2 is
+    defined as:
+
+    .. math::
+        Cv2 := \frac{1}{N} \sum_{i=1}^{N-1}
+                           \frac{2|I_{i+1}-I_i|}
+                          {|I_{i+1}+I_i|}
+
+    The Cv2 is typically computed as a substitute for the classical
+    coefficient of variation (Cv) for sequences of events which include some
+    (relatively slow) rate fluctuation.  As with the Cv, Cv2=1 for a sequence
+    of intervals generated by a Poisson process.
+
+    Parameters
+    ----------
+    time_intervals : pq.Quantity or np.ndarray or list
+        Vector of consecutive time intervals.
+    with_nan : bool, optional
+        If True, `cv2` of a spike train with less than two spikes results in a
+        np.NaN value and a warning is raised.
+        If False, `ValueError` exception is raised with a spike train with
+        less than two spikes.
+        Default: True.
+
+    Returns
+    -------
+    float
+        The Cv2 of the inter-spike interval of the input sequence.
+
+    Raises
+    ------
+    ValueError
+        If an empty list is specified, or if the sequence has less than two
+        entries and `with_nan` is False.
+
+        If a matrix is passed to the function. Only vector inputs are
+        supported.
+
+    Warns
+    -----
+    UserWarning
+        If `with_nan` is True and `cv2` is calculated for a sequence with less
+        than two entries, generating a np.NaN.
+
+    References
+    ----------
+    .. [1] G. R. Holt, W. R. Softky, C. Koch, & R. J. Douglas, "Comparison of
+           discharge variability in vitro and in vivo in cat visual cortex
+           neurons," Journal of Neurophysiology, vol. 75, no. 5, pp. 1806-1814,
+           1996.
+
+    """
+    # convert to array, cast to float
+    time_intervals = np.asarray(time_intervals)
+    np_nan = __variation_check(time_intervals, with_nan)
+    if np_nan is not None:
+        return np_nan
+
+    # calculate Cv2 and return result
+    cv_i = np.diff(time_intervals) / (time_intervals[:-1] + time_intervals[1:])
+    return 2. * np.mean(np.abs(cv_i))
+
+
+@deprecated_alias(v='time_intervals')
 def lv(time_intervals, with_nan=False):
     r"""
-    Calculate the measure of local variation LV for a sequence of time
+    Calculate the measure of local variation Lv for a sequence of time
     intervals between events.
 
-    Given a vector v containing a sequence of intervals, the LV is defined as:
+    Given a vector :math:`I` containing a sequence of intervals, the Lv is
+    defined as:
 
     .. math::
-        LV := \frac{1}{N} \sum_{i=1}^{N-1}
-                          \frac{3(isi_i-isi_{i+1})^2}
-                          {(isi_i+isi_{i+1})^2}
+        Lv := \frac{1}{N} \sum_{i=1}^{N-1}
+                          \frac{3(I_i-I_{i+1})^2}
+                          {(I_i+I_{i+1})^2}
 
-    The LV is typically computed as a substitute for the classical coefficient
+    The Lv is typically computed as a substitute for the classical coefficient
     of variation for sequences of events which include some (relatively slow)
-    rate fluctuation.  As with the CV, LV=1 for a sequence of intervals
+    rate fluctuation.  As with the Cv, Lv=1 for a sequence of intervals
     generated by a Poisson process.
 
     Parameters
     ----------
     time_intervals : pq.Quantity or np.ndarray or list
         Vector of consecutive time intervals.
     with_nan : bool, optional
-        If True, `lv` of a spike train with less than two spikes results in a
-        np.NaN value and a warning is raised.
+        If True, the Lv of a spike train with less than two spikes results in a
+        `np.NaN` value and a warning is raised.
         If False, a `ValueError` exception is raised with a spike train with
         less than two spikes.
         Default: True.
 
     Returns
     -------
     float
-        The LV of the inter-spike interval of the input sequence.
+        The Lv of the inter-spike interval of the input sequence.
 
     Raises
     ------
     ValueError
         If an empty list is specified, or if the sequence has less than two
         entries and `with_nan` is False.
 
         If a matrix is passed to the function. Only vector inputs are
         supported.
 
     Warns
     -----
     UserWarning
-        If `with_nan` is True and the `lv` is calculated for a spike train
+        If `with_nan` is True and the Lv is calculated for a spike train
         with less than two spikes, generating a np.NaN.
 
     References
     ----------
     .. [1] S. Shinomoto, K. Shima, & J. Tanji, "Differences in spiking
            patterns among cortical neurons," Neural Computation, vol. 15,
            pp. 2823–2842, 2003.
@@ -346,92 +475,112 @@
     if np_nan is not None:
         return np_nan
 
     cv_i = np.diff(time_intervals) / (time_intervals[:-1] + time_intervals[1:])
     return 3. * np.mean(np.power(cv_i, 2))
 
 
-@deprecated_alias(v='time_intervals')
-def cv2(time_intervals, with_nan=False):
+def lvr(time_intervals, R=5*pq.ms, with_nan=False):
     r"""
-    Calculate the measure of CV2 for a sequence of time intervals between
-    events.
+    Calculate the measure of revised local variation LvR for a sequence of time
+    intervals between events.
 
-    Given a vector v containing a sequence of intervals, the CV2 is defined
-    as:
+    Given a vector :math:`I` containing a sequence of intervals, the LvR is
+    defined as:
 
     .. math::
-        CV2 := \frac{1}{N} \sum_{i=1}^{N-1}
-                           \frac{2|isi_{i+1}-isi_i|}
-                          {|isi_{i+1}+isi_i|}
-
-    The CV2 is typically computed as a substitute for the classical
-    coefficient of variation (CV) for sequences of events which include some
-    (relatively slow) rate fluctuation.  As with the CV, CV2=1 for a sequence
-    of intervals generated by a Poisson process.
+        LvR := \frac{3}{N-1} \sum_{i=1}^{N-1}
+                            \left(1-\frac{4 I_i I_{i+1}}
+                            {(I_i+I_{i+1})^2}\right)
+                            \left(1+\frac{4 R}{I_i+I_{i+1}}\right)
+
+    The LvR is a revised version of the Lv, with enhanced invariance to firing
+    rate fluctuations by introducing a refractoriness constant R. The LvR with
+    `R=5ms` was shown to outperform other ISI variability measures in spike
+    trains with firing rate fluctuatins and sensory stimuli [1]_.
 
     Parameters
     ----------
     time_intervals : pq.Quantity or np.ndarray or list
         Vector of consecutive time intervals.
+    R : pq.Quantity or int or float
+        Refractoriness constant (R >= 0). If no quantity is passed `ms` are
+        assumed.
+        Default: 5 ms.
     with_nan : bool, optional
-        If True, `cv2` of a spike train with less than two spikes results in a
+        If True, LvR of a spike train with less than two spikes results in a
         np.NaN value and a warning is raised.
-        If False, `ValueError` exception is raised with a spike train with
+        If False, a `ValueError` exception is raised with a spike train with
         less than two spikes.
         Default: True.
 
     Returns
     -------
     float
-        The CV2 of the inter-spike interval of the input sequence.
+        The LvR of the inter-spike interval of the input sequence.
 
     Raises
     ------
     ValueError
         If an empty list is specified, or if the sequence has less than two
         entries and `with_nan` is False.
 
         If a matrix is passed to the function. Only vector inputs are
         supported.
 
     Warns
     -----
     UserWarning
-        If `with_nan` is True and `cv2` is calculated for a sequence with less
-        than two entries, generating a np.NaN.
+        If `with_nan` is True and the `lvr` is calculated for a spike train
+        with less than two spikes, generating a np.NaN.
+        If R is passed without any units attached milliseconds are assumed.
 
     References
     ----------
-    .. [1] G. R. Holt, W. R. Softky, C. Koch, & R. J. Douglas, "Comparison of
-           discharge variability in vitro and in vivo in cat visual cortex
-           neurons," Journal of Neurophysiology, vol. 75, no. 5, pp. 1806-1814,
-           1996.
+    .. [1] S. Shinomoto, H. Kim, T. Shimokawa et al. "Relating Neuronal Firing
+           Patterns to Functional Differentiation of Cerebral Cortex" PLOS
+           Computational Biology 5(7): e1000433, 2009.
 
     """
+    if isinstance(R, pq.Quantity):
+        R = R.rescale('ms').magnitude
+    else:
+        warnings.warn('No units specified for R, assuming milliseconds (ms)')
+
+    if R < 0:
+        raise ValueError('R must be >= 0')
+
     # convert to array, cast to float
     time_intervals = np.asarray(time_intervals)
     np_nan = __variation_check(time_intervals, with_nan)
     if np_nan is not None:
         return np_nan
 
-    # calculate CV2 and return result
-    cv_i = np.diff(time_intervals) / (time_intervals[:-1] + time_intervals[1:])
-    return 2. * np.mean(np.abs(cv_i))
+    N = len(time_intervals)
+    t = time_intervals[:-1] + time_intervals[1:]
+    frac1 = 4 * time_intervals[:-1] * time_intervals[1:] / t**2
+    frac2 = 4 * R / t
+    lvr = (3 / (N-1)) * np.sum((1-frac1) * (1+frac2))
+    return lvr
 
 
-def instantaneous_rate(spiketrain, sampling_period, kernel='auto',
+@deprecated_alias(spiketrain='spiketrains')
+def instantaneous_rate(spiketrains, sampling_period, kernel='auto',
                        cutoff=5.0, t_start=None, t_stop=None, trim=False,
                        center_kernel=True):
     """
     Estimates instantaneous firing rate by kernel convolution.
 
+    Visualization of this function is covered in Viziphant:
+    :func:`viziphant.statistics.plot_instantaneous_rates_colormesh`.
+
+
     Parameters
     ----------
-    spiketrain : neo.SpikeTrain or list of neo.SpikeTrain
+    spiketrains : neo.SpikeTrain or list of neo.SpikeTrain
         Neo object(s) that contains spike times, the unit of the time stamps,
         and `t_start` and `t_stop` of the spike train.
     sampling_period : pq.Quantity
         Time stamp resolution of the spike times. The same resolution will
         be assumed for the kernel.
     kernel : 'auto' or Kernel, optional
         The string 'auto' or callable object of class `kernels.Kernel`.
@@ -480,18 +629,18 @@
         spike. If False, no adjustment is performed such that the spike sits at
         the origin of the kernel.
         Default: True
 
     Returns
     -------
     rate : neo.AnalogSignal
-        Contains the rate estimation in unit hertz (Hz). In case a list of
-        spike trains was given, this is the combined rate of all spike trains
-        (not the average rate). `rate.times` contains the time axis of the rate
-        estimate. The unit of this property is the same as the resolution that
+        2D matrix that contains the rate estimation in unit hertz (Hz) of shape
+        ``(time, len(spiketrains))`` or ``(time, 1)`` in case of a single
+        input spiketrain. `rate.times` contains the time axis of the rate
+        estimate: the unit of this property is the same as the resolution that
         is given via the argument `sampling_period` to the function.
 
     Raises
     ------
     TypeError
         If `spiketrain` is not an instance of `neo.SpikeTrain`.
 
@@ -514,77 +663,65 @@
 
     Warns
     -----
     UserWarning
         If `cutoff` is less than `min_cutoff` attribute of `kernel`, the width
         of the kernel is adjusted to a minimally allowed width.
 
-        If the instantaneous firing rate approximation contains negative values
-        with respect to a tolerance (less than -1e-5), possibly due to machine
-        precision errors.
+    Notes
+    -----
+    The resulting instantaneous firing rate values smaller than ``0``, which
+    can happen due to machine precision errors, are clipped to zero.
 
     References
     ----------
     .. [1] H. Shimazaki, & S. Shinomoto, "Kernel bandwidth optimization in
            spike rate estimation," J Comput Neurosci, vol. 29, pp. 171–182,
            2010.
 
     Examples
     --------
     >>> import quantities as pq
     >>> from elephant import kernels
+    >>> from elephant.spike_train_generation import homogeneous_poisson_process
+    >>> spiketrain = homogeneous_poisson_process(rate=10*pq.Hz, t_stop=5*pq.s)
     >>> kernel = kernels.AlphaKernel(sigma=0.05*pq.s, invert=True)
     >>> rate = instantaneous_rate(spiketrain, sampling_period=2*pq.ms,
-    ...     kernel=kernel)
+    ...        kernel=kernel)
 
     """
-    # Merge spike trains if list of spike trains given:
-    if isinstance(spiketrain, list):
-        _check_consistency_of_spiketrains(
-            spiketrain, t_start=t_start, t_stop=t_stop)
-        if t_start is None:
-            t_start = spiketrain[0].t_start
-        if t_stop is None:
-            t_stop = spiketrain[0].t_stop
-        spikes = np.concatenate([st.magnitude for st in spiketrain])
-        merged_spiketrain = SpikeTrain(np.sort(spikes),
-                                       units=spiketrain[0].units,
-                                       t_start=t_start, t_stop=t_stop)
-        return instantaneous_rate(merged_spiketrain,
-                                  sampling_period=sampling_period,
-                                  kernel=kernel, cutoff=cutoff,
-                                  t_start=t_start,
-                                  t_stop=t_stop, trim=trim)
-
-    # Checks of input variables:
-    if not isinstance(spiketrain, SpikeTrain):
+    def optimal_kernel(st):
+        width_sigma = None
+        if len(st) > 0:
+            width_sigma = optimal_kernel_bandwidth(
+                st.magnitude, times=None, bootstrap=False)['optw']
+        if width_sigma is None:
+            raise ValueError("Unable to calculate optimal kernel width for "
+                             "instantaneous rate from input data.")
+        return kernels.GaussianKernel(width_sigma * st.units)
+
+    if isinstance(spiketrains, neo.SpikeTrain):
+        if kernel == 'auto':
+            kernel = optimal_kernel(spiketrains)
+        spiketrains = [spiketrains]
+    elif not isinstance(spiketrains, (list, tuple)):
         raise TypeError(
-            "'spiketrain' must be an instance of neo.SpikeTrain. \n"
-            "Found: '{}'".format(type(spiketrain)))
+            "'spiketrains' must be a list of neo.SpikeTrain's or a single "
+            "neo.SpikeTrain. Found: '{}'".format(type(spiketrains)))
 
     if not is_time_quantity(sampling_period):
         raise TypeError(
             "The 'sampling_period' must be a time Quantity. \n"
             "Found: {}".format(type(sampling_period)))
 
     if sampling_period.magnitude < 0:
         raise ValueError("The 'sampling_period' ({}) must be non-negative.".
                          format(sampling_period))
 
-    if kernel == 'auto':
-        kernel_width_sigma = None
-        if len(spiketrain) > 0:
-            kernel_width_sigma = optimal_kernel_bandwidth(
-                spiketrain.magnitude, times=None, bootstrap=False)['optw']
-        if kernel_width_sigma is None:
-            raise ValueError(
-                "Unable to calculate optimal kernel width for "
-                "instantaneous rate from input data.")
-        kernel = kernels.GaussianKernel(kernel_width_sigma * spiketrain.units)
-    elif not isinstance(kernel, kernels.Kernel):
+    if not (isinstance(kernel, kernels.Kernel) or kernel == 'auto'):
         raise TypeError(
             "'kernel' must be either instance of class elephant.kernels.Kernel"
             " or the string 'auto'. Found: %s, value %s" % (type(kernel),
                                                             str(kernel)))
 
     if not isinstance(cutoff, (float, int)):
         raise TypeError("'cutoff' must be float or integer")
@@ -594,131 +731,158 @@
 
     if not is_time_quantity(t_stop, allow_none=True):
         raise TypeError("'t_stop' must be a time Quantity")
 
     if not isinstance(trim, bool):
         raise TypeError("'trim' must be bool")
 
-    # main function:
-    units = pq.CompoundUnit(
-        "{}*s".format(sampling_period.rescale('s').item()))
-    spiketrain = spiketrain.rescale(units)
-    if t_start is None:
-        t_start = spiketrain.t_start
-    else:
-        t_start = t_start.rescale(spiketrain.units)
+    check_neo_consistency(spiketrains,
+                          object_type=neo.SpikeTrain,
+                          t_start=t_start, t_stop=t_stop)
+    if kernel == 'auto':
+        if len(spiketrains) == 1:
+            kernel = optimal_kernel(spiketrains[0])
+        else:
+            raise ValueError("Cannot estimate a kernel for a list of spike "
+                             "trains. Please provide a kernel explicitly "
+                             "rather than 'auto'.")
 
+    if t_start is None:
+        t_start = spiketrains[0].t_start
     if t_stop is None:
-        t_stop = spiketrain.t_stop
-    else:
-        t_stop = t_stop.rescale(spiketrain.units)
+        t_stop = spiketrains[0].t_stop
 
-    # float32 makes fftconvolve less precise which may result in nan
-    time_vector = np.zeros(int(t_stop - t_start) + 1, dtype=np.float64)
-    spikes_slice = spiketrain.time_slice(t_start, t_stop)
-    bins_active = (spikes_slice.times - t_start).magnitude.astype(np.int32)
-    bins_unique, bin_counts = np.unique(bins_active, return_counts=True)
-    time_vector[bins_unique] = bin_counts
+    units = pq.CompoundUnit(
+        "{}*s".format(sampling_period.rescale('s').item()))
+    t_start = t_start.rescale(spiketrains[0].units)
+    t_stop = t_stop.rescale(spiketrains[0].units)
+
+    n_bins = int(((t_stop - t_start) / sampling_period).simplified) + 1
+    time_vectors = np.zeros((len(spiketrains), n_bins), dtype=np.float64)
+    hist_range_end = t_stop + sampling_period.rescale(spiketrains[0].units)
+    hist_range = (t_start.item(), hist_range_end.item())
+    for i, st in enumerate(spiketrains):
+        time_vectors[i], _ = np.histogram(st.magnitude, bins=n_bins,
+                                          range=hist_range)
 
     if cutoff < kernel.min_cutoff:
         cutoff = kernel.min_cutoff
         warnings.warn("The width of the kernel was adjusted to a minimally "
                       "allowed width.")
 
-    t_arr = np.arange(-cutoff * kernel.sigma.rescale(units).magnitude,
-                      cutoff * kernel.sigma.rescale(units).magnitude +
-                      sampling_period.rescale(units).magnitude,
-                      sampling_period.rescale(units).magnitude) * units
+    # An odd number of points correctly resolves the median index and the
+    # fact that the peak of an instantaneous rate should be centered at t=0
+    # for symmetric kernels applied on a single spike at t=0.
+    # See issue https://github.com/NeuralEnsemble/elephant/issues/360
+    n_half = math.ceil(cutoff * (
+            kernel.sigma / sampling_period).simplified.item())
+    cutoff_sigma = cutoff * kernel.sigma.rescale(units).magnitude
+    if center_kernel:
+        # t_arr must be centered at the kernel median.
+        # Not centering on the kernel median leads to underestimating the
+        # instantaneous rate in cases when sampling_period >> kernel.sigma.
+        median = kernel.icdf(0.5).rescale(units).item()
+    else:
+        median = 0
+    t_arr = np.linspace(-cutoff_sigma + median, stop=cutoff_sigma + median,
+                        num=2 * n_half + 1, endpoint=True) * units
 
     if center_kernel:
         # keep the full convolve range and do the trimming afterwards;
         # trimming is performed according to the kernel median index
         fft_mode = 'full'
     elif trim:
         # no median index trimming is involved
         fft_mode = 'valid'
     else:
         # no median index trimming is involved
         fft_mode = 'same'
-    rate = scipy.signal.fftconvolve(time_vector,
-                                    kernel(t_arr).rescale(pq.Hz).magnitude,
+
+    time_vectors = time_vectors.T  # make it (time, units)
+    kernel_arr = np.expand_dims(kernel(t_arr).rescale(pq.Hz).magnitude, axis=1)
+    rate = scipy.signal.fftconvolve(time_vectors,
+                                    kernel_arr,
                                     mode=fft_mode)
+    # the convolution of non-negative vectors is non-negative
+    rate = np.clip(rate, a_min=0, a_max=None, out=rate)
 
-    if np.any(rate < -1e-8):  # abs tolerance in np.isclose
-        warnings.warn("Instantaneous firing rate approximation contains "
-                      "negative values, possibly caused due to machine "
-                      "precision errors.")
-
-    median_id = kernel.median_index(t_arr)
-    # the size of kernel() output matches the input size
-    kernel_array_size = len(t_arr)
-    if center_kernel:
-        # account for the kernel asymmetry
+    if center_kernel:  # account for the kernel asymmetry
+        median_id = kernel.median_index(t_arr)
+        # the size of kernel() output matches the input size, len(t_arr)
+        kernel_array_size = len(t_arr)
         if not trim:
             rate = rate[median_id: -kernel_array_size + median_id]
         else:
             rate = rate[2 * median_id: -2 * (kernel_array_size - median_id)]
-            t_start = t_start + median_id * spiketrain.units
-            t_stop = t_stop - (kernel_array_size - median_id
-                               ) * spiketrain.units
+            t_start = t_start + median_id * units
+            t_stop = t_stop - (kernel_array_size - median_id) * units
     else:
+        # FIXME: don't shrink the output array
         # (to be consistent with center_kernel=True)
         # n points have n-1 intervals;
         # instantaneous rate is a list of intervals;
         # hence, the last element is excluded
         rate = rate[:-1]
 
-    rate = neo.AnalogSignal(signal=np.expand_dims(rate, axis=1),
+    kernel_annotation = dict(type=type(kernel).__name__,
+                             sigma=str(kernel.sigma),
+                             invert=kernel.invert)
+
+    rate = neo.AnalogSignal(signal=rate,
                             sampling_period=sampling_period,
-                            units=pq.Hz, t_start=t_start, t_stop=t_stop)
+                            units=pq.Hz, t_start=t_start, t_stop=t_stop,
+                            kernel=kernel_annotation)
 
     return rate
 
 
 @deprecated_alias(binsize='bin_size')
 def time_histogram(spiketrains, bin_size, t_start=None, t_stop=None,
                    output='counts', binary=False):
     """
     Time Histogram of a list of `neo.SpikeTrain` objects.
 
+    Visualization of this function is covered in Viziphant:
+    :func:`viziphant.statistics.plot_time_histogram`.
+
     Parameters
     ----------
     spiketrains : list of neo.SpikeTrain
         `neo.SpikeTrain`s with a common time axis (same `t_start` and `t_stop`)
     bin_size : pq.Quantity
         Width of the histogram's time bins.
     t_start : pq.Quantity, optional
         Start time of the histogram. Only events in `spiketrains` falling
         between `t_start` and `t_stop` (both included) are considered in the
         histogram.
         If None, the maximum `t_start` of all `neo.SpikeTrain`s is used as
         `t_start`.
-        Default: None.
+        Default: None
     t_stop : pq.Quantity, optional
         Stop time of the histogram. Only events in `spiketrains` falling
         between `t_start` and `t_stop` (both included) are considered in the
         histogram.
         If None, the minimum `t_stop` of all `neo.SpikeTrain`s is used as
         `t_stop`.
-        Default: None.
+        Default: None
     output : {'counts', 'mean', 'rate'}, optional
         Normalization of the histogram. Can be one of:
         * 'counts': spike counts at each bin (as integer numbers)
         * 'mean': mean spike counts per spike train
         * 'rate': mean spike rate per spike train. Like 'mean', but the
           counts are additionally normalized by the bin width.
-        Default: 'counts'.
+        Default: 'counts'
     binary : bool, optional
         If True, indicates whether all `neo.SpikeTrain` objects should first
         be binned to a binary representation (using the
         `conversion.BinnedSpikeTrain` class) and the calculation of the
         histogram is based on this representation.
         Note that the output is not binary, but a histogram of the converted,
         binary representation.
-        Default: False.
+        Default: False
 
     Returns
     -------
     neo.AnalogSignal
         A `neo.AnalogSignal` object containing the histogram values.
         `neo.AnalogSignal[j]` is the histogram computed between
         `t_start + j * bin_size` and `t_start + (j + 1) * bin_size`.
@@ -737,64 +901,41 @@
         `t_stop` values.
 
     See also
     --------
     elephant.conversion.BinnedSpikeTrain
 
     """
-    min_tstop = 0
-    if t_start is None:
-        # Find the internal range for t_start, where all spike trains are
-        # defined; cut all spike trains taking that time range only
-        max_tstart, min_tstop = conv._get_start_stop_from_input(spiketrains)
-        t_start = max_tstart
-        if not all([max_tstart == t.t_start for t in spiketrains]):
-            warnings.warn(
-                "Spiketrains have different t_start values -- "
-                "using maximum t_start as t_start.")
-
-    if t_stop is None:
-        # Find the internal range for t_stop
-        if not min_tstop:
-            min_tstop = conv._get_start_stop_from_input(spiketrains)[1]
-        t_stop = min_tstop
-        if not all([min_tstop == t.t_stop for t in spiketrains]):
-            warnings.warn(
-                "Spiketrains have different t_stop values -- "
-                "using minimum t_stop as t_stop.")
-
-    sts_cut = [st.time_slice(t_start=t_start, t_stop=t_stop) for st in
-               spiketrains]
-
     # Bin the spike trains and sum across columns
-    bs = conv.BinnedSpikeTrain(sts_cut, t_start=t_start, t_stop=t_stop,
-                               bin_size=bin_size)
+    bs = BinnedSpikeTrain(spiketrains, t_start=t_start, t_stop=t_stop,
+                          bin_size=bin_size)
 
     if binary:
-        bin_hist = bs.to_sparse_bool_array().sum(axis=0)
-    else:
-        bin_hist = bs.to_sparse_array().sum(axis=0)
+        bs = bs.binarize()
+    bin_hist = bs.get_num_of_spikes(axis=0)
     # Flatten array
     bin_hist = np.ravel(bin_hist)
     # Renormalise the histogram
     if output == 'counts':
         # Raw
-        bin_hist = bin_hist * pq.dimensionless
+        bin_hist = pq.Quantity(bin_hist, units=pq.dimensionless, copy=False)
     elif output == 'mean':
         # Divide by number of input spike trains
-        bin_hist = bin_hist * 1. / len(spiketrains) * pq.dimensionless
+        bin_hist = pq.Quantity(bin_hist / len(spiketrains),
+                               units=pq.dimensionless, copy=False)
     elif output == 'rate':
         # Divide by number of input spike trains and bin width
-        bin_hist = bin_hist * 1. / len(spiketrains) / bin_size
+        bin_hist = bin_hist / (len(spiketrains) * bin_size)
     else:
         raise ValueError('Parameter output is not valid.')
 
     return neo.AnalogSignal(signal=np.expand_dims(bin_hist, axis=1),
                             sampling_period=bin_size, units=bin_hist.units,
-                            t_start=t_start)
+                            t_start=bs.t_start, normalization=output,
+                            copy=False)
 
 
 @deprecated_alias(binsize='bin_size')
 def complexity_pdf(spiketrains, bin_size):
     """
     Complexity Distribution of a list of `neo.SpikeTrain` objects.
 
@@ -1109,23 +1250,7 @@
             'yb': yb}
 
 
 def sskernel(*args, **kwargs):
     warnings.warn("'sskernel' function is deprecated; "
                   "use 'optimal_kernel_bandwidth'", DeprecationWarning)
     return optimal_kernel_bandwidth(*args, **kwargs)
-
-
-def _check_consistency_of_spiketrains(spiketrains, t_start=None,
-                                      t_stop=None):
-    for st in spiketrains:
-        if not isinstance(st, SpikeTrain):
-            raise TypeError("The spike trains must be instances of "
-                            "neo.SpikeTrain. Found: '{}'".
-                            format(type(st)))
-
-        if t_start is None and not st.t_start == spiketrains[0].t_start:
-            raise ValueError("The spike trains must have the same t_start.")
-        if t_stop is None and not st.t_stop == spiketrains[0].t_stop:
-            raise ValueError("The spike trains must have the same t_stop.")
-        if not st.units == spiketrains[0].units:
-            raise ValueError("The spike trains must have the same units.")
```

### Comparing `elephant-0.8.0/elephant/test/make_spike_extraction_test_data.py` & `elephant-0.9.0/elephant/test/make_spike_extraction_test_data.py`

 * *Files identical despite different names*

### Comparing `elephant-0.8.0/elephant/test/spike_extraction_test_data.txt` & `elephant-0.9.0/elephant/test/spike_extraction_test_data.txt`

 * *Files identical despite different names*

### Comparing `elephant-0.8.0/elephant/test/test_asset.py` & `elephant-0.9.0/elephant/test/test_asset.py`

 * *Files identical despite different names*

### Comparing `elephant-0.8.0/elephant/test/test_cell_assembly_detection.py` & `elephant-0.9.0/elephant/test/test_cell_assembly_detection.py`

 * *Files identical despite different names*

### Comparing `elephant-0.8.0/elephant/test/test_change_point_detection.py` & `elephant-0.9.0/elephant/test/test_change_point_detection.py`

 * *Files identical despite different names*

### Comparing `elephant-0.8.0/elephant/test/test_conversion.py` & `elephant-0.9.0/elephant/test/test_conversion.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,18 +8,18 @@
 
 import sys
 import unittest
 
 import neo
 import numpy as np
 import quantities as pq
-from numpy.testing.utils import (assert_array_almost_equal,
-                                 assert_array_equal)
+from numpy.testing import (assert_array_almost_equal, assert_array_equal)
 
 import elephant.conversion as cv
+from elephant.utils import get_common_start_stop_times
 
 python_version_major = sys.version_info.major
 
 
 def get_nearest(times, time):
     return (np.abs(times - time)).argmin()
 
@@ -174,15 +174,15 @@
         self.assertRaises(ValueError, cv.binarize, st1,
                           t_start=pq.Quantity(0, 'ms'), t_stop=10.)
         self.assertRaises(ValueError, cv.binarize, st1,
                           t_start=0., t_stop=pq.Quantity(10, 'ms'))
         self.assertRaises(ValueError, cv.binarize, st1)
 
     @unittest.skipUnless(python_version_major == 3, "assertWarns requires 3.2")
-    def test_bin_edges(self):
+    def test_bin_edges_empty_binned_spiketrain(self):
         st = neo.SpikeTrain(times=np.array([2.5]) * pq.s, t_start=0 * pq.s,
                             t_stop=3 * pq.s)
         with self.assertWarns(UserWarning):
             bst = cv.BinnedSpikeTrain(st, bin_size=2 * pq.s, t_start=0 * pq.s,
                                       t_stop=3 * pq.s)
         assert_array_equal(bst.bin_edges, [0., 2.] * pq.s)
         assert_array_equal(bst.spike_indices, [[]])  # no binned spikes
@@ -218,271 +218,206 @@
         a = neo.SpikeTrain([1.7, 1.8, 4.3] * pq.s, t_stop=10.0 * pq.s)
         b = neo.SpikeTrain([1.7, 1.8, 4.3] * pq.s, t_stop=10.0 * pq.s)
         bin_size = 1 * pq.s
         nbins = 10
         x = cv.BinnedSpikeTrain([a, b], n_bins=nbins, bin_size=bin_size,
                                 t_start=0 * pq.s)
         x_sparse = [2, 1, 2, 1]
-        s = x.to_sparse_array()
-        self.assertTrue(np.array_equal(s.data, x_sparse))
+        assert_array_equal(x.sparse_matrix.data, x_sparse)
         assert_array_equal(x.spike_indices, [[1, 1, 4], [1, 1, 4]])
 
     def test_binned_spiketrain_shape(self):
         a = self.spiketrain_a
         x = cv.BinnedSpikeTrain(a, n_bins=10,
                                 bin_size=self.bin_size,
                                 t_start=0 * pq.s)
         x_bool = cv.BinnedSpikeTrain(a, n_bins=10, bin_size=self.bin_size,
                                      t_start=0 * pq.s)
-        self.assertTrue(x.to_array().shape == (1, 10))
-        self.assertTrue(x_bool.to_bool_array().shape == (1, 10))
+        self.assertEqual(x.to_array().shape, (1, 10))
+        self.assertEqual(x_bool.to_bool_array().shape, (1, 10))
 
     # shape of the matrix for a list of spike trains
     def test_binned_spiketrain_shape_list(self):
         a = self.spiketrain_a
         b = self.spiketrain_b
         c = [a, b]
         nbins = 5
         x = cv.BinnedSpikeTrain(c, n_bins=nbins, t_start=0 * pq.s,
                                 t_stop=10.0 * pq.s)
         x_bool = cv.BinnedSpikeTrain(c, n_bins=nbins, t_start=0 * pq.s,
                                      t_stop=10.0 * pq.s)
-        self.assertTrue(x.to_array().shape == (2, 5))
-        self.assertTrue(x_bool.to_bool_array().shape == (2, 5))
+        self.assertEqual(x.to_array().shape, (2, 5))
+        self.assertEqual(x_bool.to_bool_array().shape, (2, 5))
 
     def test_binned_spiketrain_neg_times(self):
         a = neo.SpikeTrain(
             [-6.5, 0.5, 0.7, 1.2, 3.1, 4.3, 5.5, 6.7] * pq.s,
             t_start=-6.5 * pq.s, t_stop=10.0 * pq.s)
         bin_size = self.bin_size
         nbins = 16
         x = cv.BinnedSpikeTrain(a, n_bins=nbins, bin_size=bin_size,
                                 t_start=-6.5 * pq.s)
-        y = [
-            np.array([1, 0, 0, 0, 0, 0, 0, 1, 0, 1, 1, 0, 1, 1, 0, 0])]
-        self.assertTrue(np.array_equal(x.to_bool_array(), y))
+        y = [[1, 0, 0, 0, 0, 0, 0, 1, 0, 1, 1, 0, 1, 1, 0, 0]]
+        assert_array_equal(x.to_bool_array(), y)
 
-    @unittest.skipUnless(python_version_major == 3, "assertWarns requires 3.2")
     def test_binned_spiketrain_neg_times_list(self):
         a = neo.SpikeTrain(
             [-6.5, 0.5, 0.7, 1.2, 3.1, 4.3, 5.5, 6.7] * pq.s,
             t_start=-7 * pq.s, t_stop=7 * pq.s)
         b = neo.SpikeTrain(
             [-0.1, -0.7, 1.2, 2.2, 4.3, 5.5, 8.0] * pq.s,
             t_start=-1 * pq.s, t_stop=8 * pq.s)
-        c = [a, b]
+        spiketrains = [a, b]
 
-        bin_size = self.bin_size
-        with self.assertWarns(UserWarning):
-            x_bool = cv.BinnedSpikeTrain(c, bin_size=bin_size)
+        # not the same t_start and t_stop
+        self.assertRaises(ValueError, cv.BinnedSpikeTrain,
+                          spiketrains=spiketrains,
+                          bin_size=self.bin_size)
+        t_start, t_stop = get_common_start_stop_times(spiketrains)
+        self.assertEqual(t_start, -1 * pq.s)
+        self.assertEqual(t_stop, 7 * pq.s)
+        x_bool = cv.BinnedSpikeTrain(spiketrains, bin_size=self.bin_size,
+                                     t_start=t_start, t_stop=t_stop)
         y_bool = [[0, 1, 1, 0, 1, 1, 1, 1],
                   [1, 0, 1, 1, 0, 1, 1, 0]]
 
-        self.assertTrue(
-            np.array_equal(x_bool.to_bool_array(), y_bool))
+        assert_array_equal(x_bool.to_bool_array(), y_bool)
 
     # checking spike_indices(f) and matrix(m) for 1 spiketrain
     def test_binned_spiketrain_indices(self):
         a = self.spiketrain_a
         bin_size = self.bin_size
         nbins = 10
         x = cv.BinnedSpikeTrain(a, n_bins=nbins, bin_size=bin_size,
                                 t_start=0 * pq.s)
         x_bool = cv.BinnedSpikeTrain(a, n_bins=nbins, bin_size=bin_size,
                                      t_start=0 * pq.s)
-        y_matrix = [
-            np.array([2., 1., 0., 1., 1., 1., 1., 0., 0., 0.])]
-        y_bool_matrix = [
-            np.array([1., 1., 0., 1., 1., 1., 1., 0., 0., 0.])]
-        self.assertTrue(
-            np.array_equal(x.to_array(),
-                           y_matrix))
-        self.assertTrue(
-            np.array_equal(x_bool.to_bool_array(), y_bool_matrix))
-        self.assertTrue(
-            np.array_equal(x_bool.to_bool_array(), y_bool_matrix))
+        y_matrix = [[2., 1., 0., 1., 1., 1., 1., 0., 0., 0.]]
+        y_bool_matrix = [[1., 1., 0., 1., 1., 1., 1., 0., 0., 0.]]
+        assert_array_equal(x.to_array(), y_matrix)
+        assert_array_equal(x_bool.to_bool_array(), y_bool_matrix)
         s = x_bool.to_sparse_bool_array()[
             x_bool.to_sparse_bool_array().nonzero()]
-        self.assertTrue(np.array_equal(s, [[True] * 6]))
+        assert_array_equal(s, [[True] * 6])
 
     def test_binned_spiketrain_list(self):
         a = self.spiketrain_a
         b = self.spiketrain_b
 
         bin_size = self.bin_size
         nbins = 10
         c = [a, b]
         x = cv.BinnedSpikeTrain(c, n_bins=nbins, bin_size=bin_size,
                                 t_start=0 * pq.s)
         x_bool = cv.BinnedSpikeTrain(c, n_bins=nbins, bin_size=bin_size,
                                      t_start=0 * pq.s)
-        y_matrix = np.array(
-            [[2, 1, 0, 1, 1, 1, 1, 0, 0, 0],
-             [2, 1, 1, 0, 1, 1, 0, 0, 1, 0]])
-        y_matrix_bool = np.array(
-            [[1, 1, 0, 1, 1, 1, 1, 0, 0, 0],
-             [1, 1, 1, 0, 1, 1, 0, 0, 1, 0]])
-        self.assertTrue(
-            np.array_equal(x.to_array(),
-                           y_matrix))
-        self.assertTrue(
-            np.array_equal(x_bool.to_bool_array(), y_matrix_bool))
+        y_matrix = [[2, 1, 0, 1, 1, 1, 1, 0, 0, 0],
+                    [2, 1, 1, 0, 1, 1, 0, 0, 1, 0]]
+        y_matrix_bool = [[1, 1, 0, 1, 1, 1, 1, 0, 0, 0],
+                         [1, 1, 1, 0, 1, 1, 0, 0, 1, 0]]
+        assert_array_equal(x.to_array(), y_matrix)
+        assert_array_equal(x_bool.to_bool_array(), y_matrix_bool)
 
     # t_stop is None
     def test_binned_spiketrain_list_t_stop(self):
         a = self.spiketrain_a
         b = self.spiketrain_b
         c = [a, b]
         bin_size = self.bin_size
         nbins = 10
         x = cv.BinnedSpikeTrain(c, n_bins=nbins, bin_size=bin_size,
                                 t_start=0 * pq.s,
                                 t_stop=None)
         x_bool = cv.BinnedSpikeTrain(c, n_bins=nbins, bin_size=bin_size,
                                      t_start=0 * pq.s)
-        self.assertTrue(x.t_stop == 10 * pq.s)
-        self.assertTrue(x_bool.t_stop == 10 * pq.s)
+        self.assertEqual(x.t_stop, 10 * pq.s)
+        self.assertEqual(x_bool.t_stop, 10 * pq.s)
 
     # Test number of bins
     def test_binned_spiketrain_list_numbins(self):
         a = self.spiketrain_a
         b = self.spiketrain_b
         c = [a, b]
         bin_size = 1 * pq.s
         x = cv.BinnedSpikeTrain(c, bin_size=bin_size, t_start=0 * pq.s,
                                 t_stop=10. * pq.s)
         x_bool = cv.BinnedSpikeTrain(c, bin_size=bin_size, t_start=0 * pq.s,
                                      t_stop=10. * pq.s)
-        self.assertTrue(x.n_bins == 10)
-        self.assertTrue(x_bool.n_bins == 10)
+        self.assertEqual(x.n_bins, 10)
+        self.assertEqual(x_bool.n_bins, 10)
 
     def test_binned_spiketrain_matrix(self):
         # Init
         a = self.spiketrain_a
         b = self.spiketrain_b
         x_bool_a = cv.BinnedSpikeTrain(a, bin_size=pq.s, t_start=0 * pq.s,
                                        t_stop=10. * pq.s)
         x_bool_b = cv.BinnedSpikeTrain(b, bin_size=pq.s, t_start=0 * pq.s,
                                        t_stop=10. * pq.s)
 
         # Assumed results
-        y_matrix_a = [
-            np.array([2, 1, 0, 1, 1, 1, 1, 0, 0, 0])]
-        y_matrix_bool_a = [np.array([1, 1, 0, 1, 1, 1, 1, 0, 0, 0])]
-        y_matrix_bool_b = [np.array([1, 1, 1, 0, 1, 1, 0, 0, 1, 0])]
+        y_matrix_a = [[2, 1, 0, 1, 1, 1, 1, 0, 0, 0]]
+        y_matrix_bool_a = [[1, 1, 0, 1, 1, 1, 1, 0, 0, 0]]
+        y_matrix_bool_b = [[1, 1, 1, 0, 1, 1, 0, 0, 1, 0]]
 
         # Asserts
-        self.assertTrue(
-            np.array_equal(x_bool_a.to_bool_array(), y_matrix_bool_a))
-        self.assertTrue(np.array_equal(x_bool_b.to_bool_array(),
-                                       y_matrix_bool_b))
-        self.assertTrue(
-            np.array_equal(x_bool_a.to_array(), y_matrix_a))
-
-    def test_binned_spiketrain_matrix_storing(self):
-        a = self.spiketrain_a
-        b = self.spiketrain_b
-
-        x_bool = cv.BinnedSpikeTrain(a, bin_size=pq.s, t_start=0 * pq.s,
-                                     t_stop=10. * pq.s)
-        x = cv.BinnedSpikeTrain(b, bin_size=pq.s, t_start=0 * pq.s,
-                                t_stop=10. * pq.s)
-        # Store Matrix in variable
-        matrix_bool = x_bool.to_bool_array()
-        matrix = x.to_array(store_array=True)
-
-        # Check if same matrix
-        self.assertTrue(np.array_equal(x._mat_u,
-                                       matrix))
-        # Get the stored matrix using method
-        self.assertTrue(
-            np.array_equal(x_bool.to_bool_array(),
-                           matrix_bool))
-        self.assertTrue(
-            np.array_equal(x.to_array(),
-                           matrix))
-
-        # Test storing of sparse mat
-        sparse_bool = x_bool.to_sparse_bool_array()
-        self.assertTrue(np.array_equal(
-            sparse_bool.toarray(),
-            x_bool.to_sparse_bool_array().toarray()))
-
-        # New class without calculating the matrix
-        x = cv.BinnedSpikeTrain(b, bin_size=pq.s, t_start=0 * pq.s,
-                                t_stop=10. * pq.s)
-        # No matrix calculated, should be None
-        self.assertEqual(x._mat_u, None)
-        # Test with stored matrix
-        self.assertFalse(np.array_equal(x, matrix))
-
-    # Test matrix removing
-    def test_binned_spiketrain_remove_matrix(self):
-        a = self.spiketrain_a
-        x = cv.BinnedSpikeTrain(a, bin_size=1 * pq.s, n_bins=10,
-                                t_stop=10. * pq.s)
-        # Store
-        x.to_array(store_array=True)
-        # Remove
-        x.remove_stored_array()
-        # Assert matrix is not stored
-        self.assertIsNone(x._mat_u)
+        assert_array_equal(x_bool_a.to_bool_array(), y_matrix_bool_a)
+        assert_array_equal(x_bool_b.to_bool_array(), y_matrix_bool_b)
+        assert_array_equal(x_bool_a.to_array(), y_matrix_a)
 
     # Test if t_start is calculated correctly
     def test_binned_spiketrain_parameter_calc_tstart(self):
-        a = self.spiketrain_a
-        x = cv.BinnedSpikeTrain(a, bin_size=1 * pq.s, n_bins=10,
-                                t_stop=10. * pq.s)
+        x = cv.BinnedSpikeTrain(self.spiketrain_a, bin_size=1 * pq.s,
+                                n_bins=10, t_stop=10. * pq.s)
         self.assertEqual(x.t_start, 0. * pq.s)
         self.assertEqual(x.t_stop, 10. * pq.s)
         self.assertEqual(x.bin_size, 1 * pq.s)
         self.assertEqual(x.n_bins, 10)
 
     # Test if error raises when type of n_bins is not an integer
-    def test_binned_spiketrain_numbins_type_error(self):
+    def test_binned_spiketrain_n_bins_not_int(self):
         a = self.spiketrain_a
-        self.assertRaises(TypeError, cv.BinnedSpikeTrain, a, bin_size=pq.s,
+        self.assertRaises(ValueError, cv.BinnedSpikeTrain, a, bin_size=pq.s,
                           n_bins=1.4, t_start=0 * pq.s,
                           t_stop=10. * pq.s)
 
+    def test_to_array(self):
+        x = cv.BinnedSpikeTrain(self.spiketrain_a, bin_size=1 * pq.s,
+                                n_bins=10, t_stop=10. * pq.s)
+        arr_float = x.to_array(dtype=np.float32)
+        assert_array_equal(arr_float, x.to_array().astype(np.float32))
+
     # Test if error is raised when providing insufficient number of
     # parameters
     def test_binned_spiketrain_insufficient_arguments(self):
         a = self.spiketrain_a
-        self.assertRaises(AttributeError, cv.BinnedSpikeTrain, a)
+        self.assertRaises(ValueError, cv.BinnedSpikeTrain, a)
         self.assertRaises(
             ValueError,
             cv.BinnedSpikeTrain,
             a,
             bin_size=1 * pq.s,
             t_start=0 * pq.s,
             t_stop=0 * pq.s)
 
-    def test_calc_attributes_error(self):
-        self.assertRaises(ValueError, cv._calc_number_of_bins,
-                          1, 1 * pq.s, 0 * pq.s, self.tolerance)
-        self.assertRaises(ValueError, cv._calc_bin_size,
-                          1, 1 * pq.s, 0 * pq.s)
-
     def test_different_input_types(self):
         a = self.spiketrain_a
         q = [1, 2, 3] * pq.s
-        self.assertRaises(
-            TypeError, cv.BinnedSpikeTrain, [
-                a, q], bin_size=pq.s)
+        self.assertRaises(ValueError, cv.BinnedSpikeTrain,
+                          spiketrains=[a, q], bin_size=pq.s)
 
     def test_get_start_stop(self):
         a = self.spiketrain_a
         b = neo.SpikeTrain(
             [-0.1, -0.7, 1.2, 2.2, 4.3, 5.5, 8.0] * pq.s,
             t_start=-1 * pq.s, t_stop=8 * pq.s)
-        start, stop = cv._get_start_stop_from_input(a)
+        start, stop = cv.get_common_start_stop_times(a)
         self.assertEqual(start, a.t_start)
         self.assertEqual(stop, a.t_stop)
-        start, stop = cv._get_start_stop_from_input([a, b])
+        start, stop = cv.get_common_start_stop_times([a, b])
         self.assertEqual(start, a.t_start)
         self.assertEqual(stop, b.t_stop)
 
     def test_consistency_errors(self):
         a = self.spiketrain_a
         b = neo.SpikeTrain([-2, -1] * pq.s, t_start=-2 * pq.s,
                            t_stop=-1 * pq.s)
@@ -508,57 +443,44 @@
 
     # Test edges
     def test_binned_spiketrain_bin_edges(self):
         a = self.spiketrain_a
         x = cv.BinnedSpikeTrain(a, bin_size=1 * pq.s, n_bins=10,
                                 t_stop=10. * pq.s)
         # Test all edges
-        edges = [float(i) for i in range(11)]
-        self.assertTrue(np.array_equal(x.bin_edges, edges))
-
-        # Test left edges
-        edges = [float(i) for i in range(10)]
-        self.assertTrue(np.array_equal(x.bin_edges[:-1], edges))
-
-        # Test right edges
-        edges = [float(i) for i in range(1, 11)]
-        self.assertTrue(np.array_equal(x.bin_edges[1:], edges))
+        assert_array_equal(x.bin_edges, [float(i) for i in range(11)])
 
         # Test center edges
-        edges = np.arange(0, 10) + 0.5
-        self.assertTrue(np.array_equal(x.bin_centers, edges))
+        assert_array_equal(x.bin_centers, np.arange(0, 10) + 0.5)
 
     # Test for different units but same times
     def test_binned_spiketrain_different_units(self):
         a = self.spiketrain_a
         b = a.rescale(pq.ms)
         bin_size = 1 * pq.s
         xa = cv.BinnedSpikeTrain(a, bin_size=bin_size)
         xb = cv.BinnedSpikeTrain(b, bin_size=bin_size.rescale(pq.ms))
-        self.assertTrue(
-            np.array_equal(xa.to_bool_array(), xb.to_bool_array()))
-        self.assertTrue(
-            np.array_equal(xa.to_sparse_array().data,
-                           xb.to_sparse_array().data))
-        self.assertTrue(
-            np.array_equal(xa.bin_edges[:-1],
-                           xb.bin_edges[:-1].rescale(bin_size.units)))
+        assert_array_equal(xa.to_array(), xb.to_array())
+        assert_array_equal(xa.to_bool_array(), xb.to_bool_array())
+        assert_array_equal(xa.sparse_matrix.data,
+                           xb.sparse_matrix.data)
+        assert_array_equal(xa.bin_edges, xb.bin_edges)
 
     def test_binary_to_binned_matrix(self):
         a = [[1, 0, 0, 0], [0, 1, 1, 0]]
         x = cv.BinnedSpikeTrain(a, t_start=0 * pq.s, t_stop=5 * pq.s)
         # Check for correctness with different init params
-        self.assertTrue(np.array_equal(a, x.to_bool_array()))
-        self.assertTrue(np.array_equal(np.array(a), x.to_bool_array()))
-        self.assertTrue(np.array_equal(a, x.to_bool_array()))
+        assert_array_equal(x.to_array(), a)
+        assert_array_equal(x.to_bool_array(), a)
         self.assertEqual(x.n_bins, 4)
         self.assertEqual(x.bin_size, 1.25 * pq.s)
 
         x = cv.BinnedSpikeTrain(a, t_start=1 * pq.s, bin_size=2 * pq.s)
-        self.assertTrue(np.array_equal(a, x.to_bool_array()))
+        assert_array_equal(x.to_array(), a)
+        assert_array_equal(x.to_bool_array(), a)
         self.assertEqual(x.t_stop, 9 * pq.s)
 
         x = cv.BinnedSpikeTrain(a, t_stop=9 * pq.s, bin_size=2 * pq.s)
         self.assertEqual(x.t_start, 1 * pq.s)
 
         # Raise error
         self.assertRaises(ValueError, cv.BinnedSpikeTrain, a,
@@ -573,68 +495,95 @@
         # Check binary property
         self.assertTrue(x.is_binary)
 
     def test_binned_to_binned(self):
         a = self.spiketrain_a
         x = cv.BinnedSpikeTrain(a, bin_size=1 * pq.s).to_array()
         y = cv.BinnedSpikeTrain(x, bin_size=1 * pq.s, t_start=0 * pq.s)
-        self.assertTrue(np.array_equal(x, y.to_array()))
+        assert_array_equal(y.to_array(), x)
 
         # test with a list
         x = cv.BinnedSpikeTrain([[0, 1, 2, 3]], bin_size=1 * pq.s,
                                 t_stop=3 * pq.s).to_array()
         y = cv.BinnedSpikeTrain(x, bin_size=1 * pq.s, t_start=0 * pq.s)
-        self.assertTrue(np.array_equal(x, y.to_array()))
+        assert_array_equal(y.to_array(), x)
 
         # test with a numpy array
         a = np.array([[0, 1, 2, 3], [1, 2, 2.5, 3]])
         x = cv.BinnedSpikeTrain(a, bin_size=1 * pq.s,
                                 t_stop=3 * pq.s).to_array()
         y = cv.BinnedSpikeTrain(x, bin_size=1 * pq.s, t_start=0 * pq.s)
-        self.assertTrue(np.array_equal(x, y.to_array()))
+        assert_array_equal(y.to_array(), x)
 
         # Check binary property
         self.assertFalse(y.is_binary)
 
         # Raise Errors
-        # give a strangely shaped matrix as input (not MxN), which should
-        # produce a TypeError
-        a = np.array([[0, 1, 2, 3], [1, 2, 3]])
-        self.assertRaises(TypeError, cv.BinnedSpikeTrain, a, t_start=0 * pq.s,
+        # give a strangely shaped matrix as input (not MxN)
+        a = np.array([[0, 1, 2, 3], [1, 2, 3]], dtype=object)
+        self.assertRaises(ValueError, cv.BinnedSpikeTrain, a, t_start=0 * pq.s,
                           bin_size=1 * pq.s)
         # Give no t_start or t_stop
         a = np.array([[0, 1, 2, 3], [1, 2, 3, 4]])
-        self.assertRaises(AttributeError, cv.BinnedSpikeTrain, a,
+        self.assertRaises(ValueError, cv.BinnedSpikeTrain, a,
                           bin_size=1 * pq.s)
         # Input format not supported
-        a = np.array(([0, 1, 2], [0, 1, 2, 3, 4]))
-        self.assertRaises(TypeError, cv.BinnedSpikeTrain, a, bin_size=1 * pq.s)
+        a = np.array(([0, 1, 2], [0, 1, 2, 3, 4]), dtype=object)
+        self.assertRaises(ValueError, cv.BinnedSpikeTrain, a,
+                          bin_size=1 * pq.s)
 
-    def test_binnend_spiketrain_rescaling(self):
+    def test_binnend_spiketrain_different_input_units(self):
         train = neo.SpikeTrain(times=np.array([1.001, 1.002, 1.005]) * pq.s,
                                t_start=1 * pq.s, t_stop=1.01 * pq.s)
         bst = cv.BinnedSpikeTrain(train,
                                   t_start=1 * pq.s, t_stop=1.01 * pq.s,
                                   bin_size=1 * pq.ms)
+        self.assertEqual(bst.units, pq.s)
         target_edges = np.array([1000, 1001, 1002, 1003, 1004, 1005, 1006,
-                                 1007, 1008, 1009, 1010], dtype=np.float)
+                                 1007, 1008, 1009, 1010], dtype=np.float
+                                ) * pq.ms
         target_centers = np.array(
             [1000.5, 1001.5, 1002.5, 1003.5, 1004.5, 1005.5, 1006.5, 1007.5,
-             1008.5, 1009.5], dtype=np.float)
-        self.assertTrue(np.allclose(bst.bin_edges.magnitude, target_edges))
-        self.assertTrue(np.allclose(bst.bin_centers.magnitude, target_centers))
-        self.assertTrue(bst.bin_centers.units == pq.ms)
-        self.assertTrue(bst.bin_edges.units == pq.ms)
+             1008.5, 1009.5], dtype=np.float) * pq.ms
+        assert_array_almost_equal(bst.bin_edges, target_edges)
+        assert_array_almost_equal(bst.bin_centers, target_centers)
+
         bst = cv.BinnedSpikeTrain(train,
                                   t_start=1 * pq.s, t_stop=1010 * pq.ms,
                                   bin_size=1 * pq.ms)
-        self.assertTrue(np.allclose(bst.bin_edges.magnitude, target_edges))
-        self.assertTrue(np.allclose(bst.bin_centers.magnitude, target_centers))
-        self.assertTrue(bst.bin_centers.units == pq.ms)
-        self.assertTrue(bst.bin_edges.units == pq.ms)
+        self.assertEqual(bst.units, pq.s)
+        assert_array_almost_equal(bst.bin_edges, target_edges)
+        assert_array_almost_equal(bst.bin_centers, target_centers)
+
+    def test_rescale(self):
+        train = neo.SpikeTrain(times=np.array([1.001, 1.002, 1.005]) * pq.s,
+                               t_start=1 * pq.s, t_stop=1.01 * pq.s)
+        bst = cv.BinnedSpikeTrain(train, t_start=1 * pq.s,
+                                  t_stop=1.01 * pq.s,
+                                  bin_size=1 * pq.ms)
+        self.assertEqual(bst.units, pq.s)
+        self.assertEqual(bst._t_start, 1)  # 1 s
+        self.assertEqual(bst._t_stop, 1.01)  # 1.01 s
+        self.assertEqual(bst._bin_size, 0.001)  # 0.001 s
+
+        bst.rescale(units='ms')
+        self.assertEqual(bst.units, pq.ms)
+        self.assertEqual(bst._t_start, 1000)  # 1 s
+        self.assertEqual(bst._t_stop, 1010)  # 1.01 s
+        self.assertEqual(bst._bin_size, 1)  # 0.001 s
+
+    def test_repr(self):
+        train = neo.SpikeTrain(times=np.array([1.001, 1.002, 1.005]) * pq.s,
+                               t_start=1 * pq.s, t_stop=1.01 * pq.s)
+        bst = cv.BinnedSpikeTrain(train, t_start=1 * pq.s,
+                                  t_stop=1.01 * pq.s,
+                                  bin_size=1 * pq.ms)
+        self.assertEqual(repr(bst), "BinnedSpikeTrain(t_start=1.0 s, "
+                                    "t_stop=1.01 s, bin_size=0.001 s; "
+                                    "shape=(1, 10))")
 
     def test_binned_sparsity(self):
         train = neo.SpikeTrain(np.arange(10), t_stop=10 * pq.s, units=pq.s)
         bst = cv.BinnedSpikeTrain(train, n_bins=100)
         self.assertAlmostEqual(bst.sparsity, 0.1)
 
     # Test fix for rounding errors
```

### Comparing `elephant-0.8.0/elephant/test/test_csd.py` & `elephant-0.9.0/elephant/test/test_csd.py`

 * *Files identical despite different names*

### Comparing `elephant-0.8.0/elephant/test/test_cubic.py` & `elephant-0.9.0/elephant/test/test_cubic.py`

 * *Files identical despite different names*

### Comparing `elephant-0.8.0/elephant/test/test_gpfa.py` & `elephant-0.9.0/elephant/test/test_gpfa.py`

 * *Files 3% similar despite different names*

```diff
@@ -87,25 +87,27 @@
             spike_times = [homogeneous_poisson_process(rate=rate * pq.Hz)
                            for rate in rates]
             self.data2.append(spike_times)
 
     def test_data1(self):
         gpfa = GPFA(x_dim=self.x_dim, em_max_iters=self.n_iters)
         gpfa.fit(self.data1)
-        xorth = gpfa.transform(self.data1)
+        latent_variable_orth = gpfa.transform(self.data1)
         self.assertAlmostEqual(gpfa.transform_info['log_likelihood'],
                                -8172.004695554373, places=5)
         # Since data1 is inherently 2 dimensional, only the first two
-        # dimensions of xorth should have finite power.
+        # dimensions of latent_variable_orth should have finite power.
         for i in [0, 1]:
-            self.assertNotEqual(xorth[0][i].mean(), 0)
-            self.assertNotEqual(xorth[0][i].var(), 0)
+            self.assertNotEqual(latent_variable_orth[0][i].mean(), 0)
+            self.assertNotEqual(latent_variable_orth[0][i].var(), 0)
         for i in [2, 3]:
-            self.assertAlmostEqual(xorth[0][i].mean(), 0, places=2)
-            self.assertAlmostEqual(xorth[0][i].var(), 0, places=2)
+            self.assertAlmostEqual(latent_variable_orth[0][i].mean(), 0,
+                                   places=2)
+            self.assertAlmostEqual(latent_variable_orth[0][i].var(), 0,
+                                   places=2)
 
     def test_transform_testing_data(self):
         # check if the num. of neurons in the test data matches the
         # num. of neurons in the training data
         gpfa1 = GPFA(x_dim=self.x_dim, em_max_iters=self.n_iters)
         gpfa1.fit(self.data1)
         with self.assertRaises(ValueError):
@@ -165,20 +167,22 @@
         with self.assertRaises(ValueError):
             seqs = gpfa.transform(self.data2, returned_data=['invalid_name'])
 
     def test_fit_transform(self):
         gpfa1 = GPFA(bin_size=self.bin_size, x_dim=self.x_dim,
                      em_max_iters=self.n_iters)
         gpfa1.fit(self.data1)
-        xorth1 = gpfa1.transform(self.data1)
-        xorth2 = GPFA(bin_size=self.bin_size, x_dim=self.x_dim,
-                      em_max_iters=self.n_iters).fit_transform(self.data1)
+        latent_variable_orth1 = gpfa1.transform(self.data1)
+        latent_variable_orth2 = GPFA(
+            bin_size=self.bin_size, x_dim=self.x_dim,
+            em_max_iters=self.n_iters).fit_transform(self.data1)
         for i in range(len(self.data1)):
             for j in range(self.x_dim):
-                assert_array_almost_equal(xorth1[i][j], xorth2[i][j])
+                assert_array_almost_equal(latent_variable_orth1[i][j],
+                                          latent_variable_orth2[i][j])
 
     def test_get_seq_sqrt(self):
         data = [self.data2[0]]
         seqs = gpfa_util.get_seqs(data, bin_size=self.bin_size)
         seqs_not_sqrt = gpfa_util.get_seqs(data, bin_size=self.bin_size,
                                            use_sqrt=False)
         self.assertEqual(seqs['T'], seqs_not_sqrt['T'])
```

### Comparing `elephant-0.8.0/elephant/test/test_icsd.py` & `elephant-0.9.0/elephant/test/test_icsd.py`

 * *Files identical despite different names*

### Comparing `elephant-0.8.0/elephant/test/test_kcsd.py` & `elephant-0.9.0/elephant/test/test_kcsd.py`

 * *Files identical despite different names*

### Comparing `elephant-0.8.0/elephant/test/test_kernels.py` & `elephant-0.9.0/elephant/test/test_kernels.py`

 * *Files identical despite different names*

### Comparing `elephant-0.8.0/elephant/test/test_neo_tools.py` & `elephant-0.9.0/elephant/test/test_neo_tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -857,41 +857,34 @@
 
         self.assertEqual(targ, res0)
 
     def test__extract_neo_attrs__spiketrain_parents_childfirst_array(self):
         obj = self.block.list_children_by_class('SpikeTrain')[0]
         blk = self.block
         seg = self.block.segments[0]
-        rcg = self.block.channel_indexes[0]
         unit = self.block.channel_indexes[0].units[0]
 
         targ = get_fake_values('Block', seed=blk.annotations['seed'])
-        targ.update(get_fake_values('ChannelIndex',
-                                    seed=rcg.annotations['seed']))
-        targ['channel_names'] = rcg.channel_names
         targ.update(get_fake_values('Unit', seed=unit.annotations['seed']))
         targ.update(get_fake_values('Segment', seed=seg.annotations['seed']))
         targ.update(get_fake_values('SpikeTrain',
                                     seed=obj.annotations['seed']))
         del targ['times']
 
         res00 = nt.extract_neo_attributes(obj, parents=True, skip_array=False)
         res10 = nt.extract_neo_attributes(obj, parents=True, skip_array=False,
                                           child_first=True)
         res01 = nt.extract_neo_attributes(obj, parents=True)
         res11 = nt.extract_neo_attributes(obj, parents=True, child_first=True)
 
-        del res00['i']
-        del res10['i']
-        del res01['i']
-        del res11['i']
-        del res00['j']
-        del res10['j']
-        del res01['j']
-        del res11['j']
+        ignore_annotations = ('i', 'j', 'channel_names',
+                              'channel_ids', 'coordinates')
+        for res in (res00, res01, res10, res11):
+            for attr in ignore_annotations:
+                del res[attr]
 
         self.assert_dicts_equal(targ, res00)
         self.assert_dicts_equal(targ, res10)
         self.assert_dicts_equal(targ, res01)
         self.assert_dicts_equal(targ, res11)
 
     def test__extract_neo_attrs__epoch_parents_childfirst_array(self):
@@ -908,22 +901,18 @@
 
         res00 = nt.extract_neo_attributes(obj, parents=True, skip_array=False)
         res10 = nt.extract_neo_attributes(obj, parents=True, skip_array=False,
                                           child_first=True)
         res01 = nt.extract_neo_attributes(obj, parents=True)
         res11 = nt.extract_neo_attributes(obj, parents=True, child_first=True)
 
-        del res00['i']
-        del res10['i']
-        del res01['i']
-        del res11['i']
-        del res00['j']
-        del res10['j']
-        del res01['j']
-        del res11['j']
+        ignore_annotations = ('i', 'j')
+        for res in (res00, res01, res10, res11):
+            for attr in ignore_annotations:
+                del res[attr]
 
         self.assert_dicts_equal(targ, res00)
         self.assert_dicts_equal(targ, res10)
         self.assert_dicts_equal(targ, res01)
         self.assert_dicts_equal(targ, res11)
 
     def test__extract_neo_attrs__event_parents_childfirst_array(self):
@@ -956,39 +945,32 @@
         self.assert_dicts_equal(targ, res01)
         self.assert_dicts_equal(targ, res11)
 
     def test__extract_neo_attrs__spiketrain_parents_parentfirst_array(self):
         obj = self.block.list_children_by_class('SpikeTrain')[0]
         blk = self.block
         seg = self.block.segments[0]
-        rcg = self.block.channel_indexes[0]
         unit = self.block.channel_indexes[0].units[0]
 
         targ = get_fake_values('SpikeTrain', seed=obj.annotations['seed'])
         targ.update(get_fake_values('Segment', seed=seg.annotations['seed']))
         targ.update(get_fake_values('Unit', seed=unit.annotations['seed']))
-        targ.update(get_fake_values('ChannelIndex',
-                                    seed=rcg.annotations['seed']))
         targ.update(get_fake_values('Block', seed=blk.annotations['seed']))
         del targ['times']
         del targ['index']
-        del targ['channel_names']
 
         res0 = nt.extract_neo_attributes(obj, parents=True, skip_array=False,
                                          child_first=False)
         res1 = nt.extract_neo_attributes(obj, parents=True, child_first=False)
 
-        del res0['i']
-        del res1['i']
-        del res0['j']
-        del res1['j']
-        del res0['index']
-        del res1['index']
-        del res0['channel_names']
-        del res1['channel_names']
+        ignore_annotations = ('i', 'j', 'index', 'channel_names',
+                              'channel_ids', 'coordinates')
+        for res in (res0, res1):
+            for attr in ignore_annotations:
+                del res[attr]
 
         self.assert_dicts_equal(targ, res0)
         self.assert_dicts_equal(targ, res1)
 
     def test__extract_neo_attrs__epoch_parents_parentfirst_array(self):
         obj = self.block.list_children_by_class('Epoch')[0]
         blk = self.block
```

### Comparing `elephant-0.8.0/elephant/test/test_pandas_bridge.py` & `elephant-0.9.0/elephant/test/test_pandas_bridge.py`

 * *Files identical despite different names*

### Comparing `elephant-0.8.0/elephant/test/test_parallel.py` & `elephant-0.9.0/elephant/test/test_parallel.py`

 * *Files identical despite different names*

### Comparing `elephant-0.8.0/elephant/test/test_phase_analysis.py` & `elephant-0.9.0/elephant/test/test_phase_analysis.py`

 * *Files identical despite different names*

### Comparing `elephant-0.8.0/elephant/test/test_signal_processing.py` & `elephant-0.9.0/elephant/test/test_signal_processing.py`

 * *Files 1% similar despite different names*

```diff
@@ -291,28 +291,24 @@
         self.assertEqual(signal.magnitude[0], self.test_seq1[0])
 
     def test_zscore_single_inplace_int(self):
         """
         Test if the z-score is correctly calculated even if the input is an
         AnalogSignal of type int, asking for an inplace operation.
         """
-        signal = neo.AnalogSignal(
-            self.test_seq1, units='mV',
-            t_start=0. * pq.ms, sampling_rate=1000. * pq.Hz, dtype=int)
-
         m = np.mean(self.test_seq1)
         s = np.std(self.test_seq1)
         target = (self.test_seq1 - m) / s
 
-        assert_array_almost_equal(
-            elephant.signal_processing.zscore(signal, inplace=True).magnitude,
-            target.reshape(-1, 1).astype(int), decimal=9)
+        signal = neo.AnalogSignal(
+            self.test_seq1, units='mV',
+            t_start=0. * pq.ms, sampling_rate=1000. * pq.Hz, dtype=int)
+        zscored = elephant.signal_processing.zscore(signal, inplace=True)
 
-        # Assert original signal is overwritten
-        self.assertEqual(signal[0].magnitude, target.astype(int)[0])
+        assert_array_almost_equal(zscored.magnitude.squeeze(), target)
 
     def test_zscore_list_dup(self):
         """
         Test zscore on a list of AnalogSignal objects, asking to return a
         duplicate.
         """
         signal1 = neo.AnalogSignal(
@@ -382,14 +378,24 @@
             result[1].magnitude,
             np.transpose(np.vstack([target21, target22])), decimal=9)
 
         # Assert original signal is overwritten
         self.assertEqual(signal1[0, 0].magnitude, target11[0])
         self.assertEqual(signal2[0, 0].magnitude, target21[0])
 
+    def test_wrong_input(self):
+        # wrong type
+        self.assertRaises(TypeError, elephant.signal_processing.zscore,
+                          signal=[1, 2] * pq.uV)
+        # units mismatch
+        asig1 = neo.AnalogSignal([0, 1], units=pq.uV, sampling_rate=1 * pq.ms)
+        asig2 = neo.AnalogSignal([0, 1], units=pq.V, sampling_rate=1 * pq.ms)
+        self.assertRaises(ValueError, elephant.signal_processing.zscore,
+                          signal=[asig1, asig2])
+
 
 class ButterTestCase(unittest.TestCase):
 
     def test_butter_filter_type(self):
         """
         Test if correct type of filtering is performed according to how cut-off
         frequencies are given
```

### Comparing `elephant-0.8.0/elephant/test/test_spade.py` & `elephant-0.9.0/elephant/test/test_spade.py`

 * *Files 19% similar despite different names*

```diff
@@ -4,37 +4,39 @@
 :copyright: Copyright 2014-2016 by the Elephant team, see `doc/authors.rst`.
 :license: Modified BSD, see LICENSE.txt for details.
 """
 from __future__ import division
 
 import sys
 import unittest
+import random
 
 import neo
 import numpy as np
 import quantities as pq
 from numpy.testing.utils import assert_array_equal
 
 import elephant.conversion as conv
 import elephant.spade as spade
 import elephant.spike_train_generation as stg
-import elephant.spike_train_surrogates as surr
-from elephant.spade import HAVE_FIM
-
-python_version_major = sys.version_info.major
 
 try:
     import statsmodels
     HAVE_STATSMODELS = True
 except ImportError:
     HAVE_STATSMODELS = False
 
+python_version_major = sys.version_info.major
+
+HAVE_FIM = spade.HAVE_FIM
+
 
 class SpadeTestCase(unittest.TestCase):
     def setUp(self):
+        np.random.seed(0)
         # Spade parameters
         self.bin_size = 1 * pq.ms
         self.winlen = 10
         self.n_subset = 10
         self.n_surr = 10
         self.alpha = 0.05
         self.stability_thresh = [0.1, 0.1]
@@ -144,19 +146,18 @@
     # Testing spectrum cpp
     def test_spade_spectrum_cpp(self):
         # Computing Spectrum
         spectrum_cpp = spade.concepts_mining(self.cpp, self.bin_size,
                                              1, report='#')[0]
         # Check spectrum
         assert_array_equal(
-            spectrum_cpp, [
-                (len(
-                    self.cpp), np.sum(
-                    conv.BinnedSpikeTrain(
-                        self.cpp[0], self.bin_size).to_bool_array()), 1)])
+            spectrum_cpp,
+            [(len(self.cpp),
+              np.sum(conv.BinnedSpikeTrain(
+                  self.cpp[0], self.bin_size).to_bool_array()), 1)])
 
     # Testing with multiple patterns input
     def test_spade_msip(self):
         output_msip = spade.spade(self.msip, self.bin_size, self.winlen,
                                   approx_stab_pars=dict(
                                       n_subsets=self.n_subset,
                                       stability_thresh=self.stability_thresh),
@@ -418,27 +419,137 @@
         assert_array_equal(spectrum_3d, [
             [len(self.lags1) + 1, self.n_occ1, max(self.lags1), 1]])
 
     def test_spade_raise_error(self):
         # Test list not using neo.Spiketrain
         self.assertRaises(TypeError, spade.spade, [
             [1, 2, 3], [3, 4, 5]], 1 * pq.ms, 4, stat_corr='no')
+        self.assertRaises(TypeError, spade.concepts_mining, [
+            [1, 2, 3], [3, 4, 5]], 1 * pq.ms, 4)
         # Test neo.Spiketrain with different t_stop
         self.assertRaises(
             ValueError, spade.spade,
             [neo.SpikeTrain([1, 2, 3] * pq.s, t_stop=5 * pq.s),
              neo.SpikeTrain([3, 4, 5] * pq.s, t_stop=6 * pq.s)],
             1 * pq.ms, 4, stat_corr='no')
+        # Test bin_size not pq.Quantity
+        self.assertRaises(
+            TypeError, spade.spade,
+            [neo.SpikeTrain([1, 2, 3] * pq.s, t_stop=6 * pq.s),
+             neo.SpikeTrain([3, 4, 5] * pq.s, t_stop=6 * pq.s)],
+            bin_size=1., winlen=4, stat_corr='no')
+        # Test winlen not int
+        self.assertRaises(
+            TypeError, spade.spade,
+            [neo.SpikeTrain([1, 2, 3] * pq.s, t_stop=6 * pq.s),
+             neo.SpikeTrain([3, 4, 5] * pq.s, t_stop=6 * pq.s)],
+            bin_size=1.*pq.ms, winlen=4.1, stat_corr='no')
+        # Test min_spikes not int
+        self.assertRaises(
+            TypeError, spade.spade,
+            [neo.SpikeTrain([1, 2, 3] * pq.s, t_stop=6 * pq.s),
+             neo.SpikeTrain([3, 4, 5] * pq.s, t_stop=6 * pq.s)],
+            bin_size=1.*pq.ms, winlen=4, min_spikes=3.4, stat_corr='no')
+        # Test min_occ not int
+        self.assertRaises(
+            TypeError, spade.spade,
+            [neo.SpikeTrain([1, 2, 3] * pq.s, t_stop=6 * pq.s),
+             neo.SpikeTrain([3, 4, 5] * pq.s, t_stop=6 * pq.s)],
+            bin_size=1.*pq.ms, winlen=4, min_occ=3.4, stat_corr='no')
+        # Test max_spikes not int
+        self.assertRaises(
+            TypeError, spade.spade,
+            [neo.SpikeTrain([1, 2, 3] * pq.s, t_stop=6 * pq.s),
+             neo.SpikeTrain([3, 4, 5] * pq.s, t_stop=6 * pq.s)],
+            bin_size=1.*pq.ms, winlen=4, max_spikes=3.4, stat_corr='no')
+        # Test max_occ not int
+        self.assertRaises(
+            TypeError, spade.spade,
+            [neo.SpikeTrain([1, 2, 3] * pq.s, t_stop=6 * pq.s),
+             neo.SpikeTrain([3, 4, 5] * pq.s, t_stop=6 * pq.s)],
+            bin_size=1.*pq.ms, winlen=4, max_occ=3.4, stat_corr='no')
+        # Test min_neu not int
+        self.assertRaises(
+            TypeError, spade.spade,
+            [neo.SpikeTrain([1, 2, 3] * pq.s, t_stop=6 * pq.s),
+             neo.SpikeTrain([3, 4, 5] * pq.s, t_stop=6 * pq.s)],
+            bin_size=1.*pq.ms, winlen=4, min_neu=3.4, stat_corr='no')
+        # Test wrong stability params
+        self.assertRaises(
+            ValueError, spade.spade,
+            [neo.SpikeTrain([1, 2, 3] * pq.s, t_stop=6 * pq.s),
+             neo.SpikeTrain([3, 4, 5] * pq.s, t_stop=6 * pq.s)],
+            bin_size=1.*pq.ms, winlen=4, approx_stab_pars={'wrong key': 0},
+            stat_corr='no')
+        # Test n_surr not int
+        self.assertRaises(
+            TypeError, spade.spade,
+            [neo.SpikeTrain([1, 2, 3] * pq.s, t_stop=6 * pq.s),
+             neo.SpikeTrain([3, 4, 5] * pq.s, t_stop=6 * pq.s)],
+            bin_size=1.*pq.ms, winlen=4, n_surr=3.4, stat_corr='no')
+        # Test dither not pq.Quantity
+        self.assertRaises(
+            TypeError, spade.spade,
+            [neo.SpikeTrain([1, 2, 3] * pq.s, t_stop=6 * pq.s),
+             neo.SpikeTrain([3, 4, 5] * pq.s, t_stop=6 * pq.s)],
+            bin_size=1.*pq.ms, winlen=4, n_surr=100, alpha=0.05,
+            dither=15., stat_corr='no')
+        # Test wrong alpha
+        self.assertRaises(
+            TypeError, spade.spade,
+            [neo.SpikeTrain([1, 2, 3] * pq.s, t_stop=6 * pq.s),
+             neo.SpikeTrain([3, 4, 5] * pq.s, t_stop=6 * pq.s)],
+            bin_size=1.*pq.ms, winlen=4, n_surr=100, alpha='5 %',
+            dither=15.*pq.ms, stat_corr='no')
+        # Test wrong statistical correction
+        self.assertRaises(
+            ValueError, spade.spade,
+            [neo.SpikeTrain([1, 2, 3] * pq.s, t_stop=6 * pq.s),
+             neo.SpikeTrain([3, 4, 5] * pq.s, t_stop=6 * pq.s)],
+            bin_size=1.*pq.ms, winlen=4, n_surr=100, alpha=0.05,
+            dither=15.*pq.ms, stat_corr='wrong correction')
+        # Test wrong psr_params
+        self.assertRaises(
+            TypeError, spade.spade,
+            [neo.SpikeTrain([1, 2, 3] * pq.s, t_stop=6 * pq.s),
+             neo.SpikeTrain([3, 4, 5] * pq.s, t_stop=6 * pq.s)],
+            bin_size=1.*pq.ms, winlen=4, n_surr=100, alpha=0.05,
+            dither=15.*pq.ms, stat_corr='no', psr_param=(2.5, 3.4, 2.1))
+        # Test wrong psr_params
+        self.assertRaises(
+            TypeError, spade.spade,
+            [neo.SpikeTrain([1, 2, 3] * pq.s, t_stop=6 * pq.s),
+             neo.SpikeTrain([3, 4, 5] * pq.s, t_stop=6 * pq.s)],
+            bin_size=1.*pq.ms, winlen=4, n_surr=100, alpha=0.05,
+            dither=15.*pq.ms, stat_corr='no', psr_param=3.1)
+        # Test output format
+        self.assertRaises(
+            ValueError, spade.spade,
+            [neo.SpikeTrain([1, 2, 3] * pq.s, t_stop=6 * pq.s),
+             neo.SpikeTrain([3, 4, 5] * pq.s, t_stop=6 * pq.s)],
+            bin_size=1.*pq.ms, winlen=4, n_surr=100, alpha=0.05,
+            dither=15.*pq.ms, stat_corr='no', output_format='wrong_output')
         # Test wrong spectrum parameter
         self.assertRaises(
             ValueError, spade.spade,
             [neo.SpikeTrain([1, 2, 3] * pq.s, t_stop=6 * pq.s),
              neo.SpikeTrain([3, 4, 5] * pq.s, t_stop=6 * pq.s)],
             1 * pq.ms, 4, n_surr=1, stat_corr='no',
             spectrum='invalid_key')
+        self.assertRaises(
+            ValueError, spade.concepts_mining,
+            [neo.SpikeTrain([1, 2, 3] * pq.s, t_stop=6 * pq.s),
+             neo.SpikeTrain([3, 4, 5] * pq.s, t_stop=6 * pq.s)],
+            1 * pq.ms, 4, report='invalid_key')
+        self.assertRaises(
+            ValueError, spade.pvalue_spectrum,
+            [neo.SpikeTrain([1, 2, 3] * pq.s, t_stop=6 * pq.s),
+             neo.SpikeTrain([3, 4, 5] * pq.s, t_stop=6 * pq.s)],
+            1 * pq.ms, 4, dither=10*pq.ms, n_surr=1,
+            spectrum='invalid_key')
         # Test negative minimum number of spikes
         self.assertRaises(
             ValueError, spade.spade,
             [neo.SpikeTrain([1, 2, 3] * pq.s, t_stop=5 * pq.s),
              neo.SpikeTrain([3, 4, 5] * pq.s, t_stop=5 * pq.s)],
             1 * pq.ms, 4, min_neu=-3, stat_corr='no')
         # Test wrong dither method
@@ -448,14 +559,21 @@
              neo.SpikeTrain([3, 4, 5] * pq.s, t_stop=5 * pq.s)],
             1 * pq.ms, 4, surr_method='invalid_key', stat_corr='no')
         # Test negative number of surrogates
         self.assertRaises(
             ValueError, spade.pvalue_spectrum,
             [neo.SpikeTrain([1, 2, 3] * pq.s, t_stop=5 * pq.s),
              neo.SpikeTrain([3, 4, 5] * pq.s, t_stop=5 * pq.s)],
+            1 * pq.ms, 4, dither=10*pq.ms, n_surr=100,
+            surr_method='invalid_key')
+        # Test negative number of surrogates
+        self.assertRaises(
+            ValueError, spade.pvalue_spectrum,
+            [neo.SpikeTrain([1, 2, 3] * pq.s, t_stop=5 * pq.s),
+             neo.SpikeTrain([3, 4, 5] * pq.s, t_stop=5 * pq.s)],
             1 * pq.ms, 4, 3 * pq.ms, n_surr=-3)
         # Test wrong correction parameter
         self.assertRaises(ValueError, spade.test_signature_significance,
                           pv_spec=((2, 3, 0.2), (2, 4, 0.1)),
                           concepts=([[(2, 3), (1, 2, 3)]]),
                           alpha=0.01,
                           winlen=1,
@@ -580,14 +698,34 @@
         sig_spectrum = spade.test_signature_significance(
             pv_spec=((2, 3, 0.2), (2, 4, 0.05)),
             concepts=([[(2, 3), (1, 2, 3)],
                        [(2, 4), (1, 2, 3, 4)]]),
             alpha=0.15, winlen=1, corr='fdr_bh')
         self.assertEqual(sig_spectrum, [(2., 3., False), (2., 4., True)])
 
+    def test_different_surrogate_method(self):
+        np.random.seed(0)
+        random.seed(0)
+        spiketrains = [stg.homogeneous_poisson_process(rate=20*pq.Hz)
+                       for _ in range(2)]
+        surr_methods = ('dither_spikes', 'joint_isi_dithering',
+                        'bin_shuffling',
+                        'dither_spikes_with_refractory_period')
+        pv_specs = {'dither_spikes': [[2, 2, 0.8], [2, 3, 0.2]],
+                    'joint_isi_dithering': [[2, 2, 0.8]],
+                    'bin_shuffling': [[2, 2, 1.0], [2, 3, 0.2]],
+                    'dither_spikes_with_refractory_period':
+                        [[2, 2, 0.8]]}
+        for surr_method in surr_methods:
+            pv_spec = spade.pvalue_spectrum(
+                spiketrains, bin_size=self.bin_size,
+                winlen=self.winlen, dither=15*pq.ms,
+                n_surr=5, surr_method=surr_method)
+            self.assertEqual(pv_spec, pv_specs[surr_method])
+
 
 def suite():
     suite = unittest.makeSuite(SpadeTestCase, 'test')
     return suite
 
 
 if __name__ == "__main__":
```

### Comparing `elephant-0.8.0/elephant/test/test_spectral.py` & `elephant-0.9.0/elephant/test/test_spectral.py`

 * *Files identical despite different names*

### Comparing `elephant-0.8.0/elephant/test/test_spike_train_correlation.py` & `elephant-0.9.0/elephant/test/test_spike_train_correlation.py`

 * *Files 1% similar despite different names*

```diff
@@ -621,14 +621,23 @@
 
     def test_exist_alias(self):
         '''
         Test if alias cch still exists.
         '''
         self.assertEqual(sc.cross_correlation_histogram, sc.cch)
 
+    def test_annotations(self):
+        cch, _ = sc.cross_correlation_histogram(
+            self.binned_st1, self.binned_st2, kernel=np.ones(3))
+        target_dict = dict(window='full', border_correction=False,
+                           binary=False, kernel=True,
+                           normalization='counts')
+        self.assertIn('cch_parameters', cch.annotations)
+        self.assertEqual(cch.annotations['cch_parameters'], target_dict)
+
 
 @unittest.skipUnless(python_version_major == 3, "subTest requires 3.4")
 class CrossCorrelationHistDifferentTStartTStopTest(unittest.TestCase):
 
     def _run_sub_tests(self, st1, st2, lags_true):
         for window in ('valid', 'full'):
             for method in ('speed', 'memory'):
@@ -779,23 +788,19 @@
         '''
         nu = 25 / pq.s
         T = 15 * pq.min
         bin_size = 1 * pq.ms
         timescale = 1 / (4 * nu)
         np.random.seed(35)
 
-        timescale_num = []
         for _ in range(10):
             spikes = homogeneous_gamma_process(2, 2 * nu, 0 * pq.ms, T)
             spikes_bin = conv.BinnedSpikeTrain(spikes, bin_size)
             timescale_i = sc.spike_train_timescale(spikes_bin, 10 * timescale)
-            timescale_i.units = timescale.units
-            timescale_num.append(timescale_i.magnitude)
-        assert_array_almost_equal(timescale.magnitude, timescale_num,
-                                  decimal=3)
+            assert_array_almost_equal(timescale, timescale_i, decimal=3)
 
     def test_timescale_errors(self):
         spikes = neo.SpikeTrain([1, 5, 7, 8] * pq.ms, t_stop=10 * pq.ms)
         binsize = 1 * pq.ms
         spikes_bin = conv.BinnedSpikeTrain(spikes, binsize)
 
         # Tau max with no units
```

### Comparing `elephant-0.8.0/elephant/test/test_spike_train_dissimilarity.py` & `elephant-0.9.0/elephant/test/test_spike_train_dissimilarity.py`

 * *Files identical despite different names*

### Comparing `elephant-0.8.0/elephant/test/test_spike_train_generation.py` & `elephant-0.9.0/elephant/test/test_spike_train_generation.py`

 * *Files 20% similar despite different names*

```diff
@@ -11,21 +11,22 @@
 import os
 import sys
 import unittest
 import warnings
 
 import neo
 import numpy as np
-from numpy.testing import assert_array_almost_equal
-from quantities import V, s, ms, second, Hz, kHz, mV, dimensionless
+from numpy.testing import assert_array_almost_equal, assert_allclose
+import quantities as pq
 from scipy.stats import expon
 from scipy.stats import kstest, poisson
 
 import elephant.spike_train_generation as stgen
-from elephant.statistics import isi
+from elephant.statistics import isi, instantaneous_rate
+from elephant import kernels
 
 python_version_major = sys.version_info.major
 
 
 def pdiff(a, b):
     """Difference between a and b as a fraction of a
 
@@ -40,19 +41,20 @@
         # Load membrane potential simulated using Brian2
         # according to make_spike_extraction_test_data.py.
         curr_dir = os.path.dirname(os.path.realpath(__file__))
         raw_data_file_loc = os.path.join(
             curr_dir, 'spike_extraction_test_data.txt')
         raw_data = []
         with open(raw_data_file_loc, 'r') as f:
-            for x in (f.readlines()):
+            for x in f.readlines():
                 raw_data.append(float(x))
-        self.vm = neo.AnalogSignal(raw_data, units=V, sampling_period=0.1 * ms)
+        self.vm = neo.AnalogSignal(
+            raw_data, units=pq.V, sampling_period=0.1 * pq.ms)
         self.true_time_stamps = [0.0123, 0.0354, 0.0712, 0.1191, 0.1694,
-                                 0.2200, 0.2711] * second
+                                 0.2200, 0.2711] * pq.s
 
     def test_threshold_detection(self):
         # Test whether spikes are extracted at the correct times from
         # an analog signal.
 
         spike_train = stgen.threshold_detection(self.vm)
         try:
@@ -75,74 +77,76 @@
         try:
             assert_array_almost_equal(spike_train, self.true_time_stamps)
         except AttributeError:  # If numpy version too old to have allclose
             self.assertTrue(np.array_equal(spike_train, self.true_time_stamps))
 
     def test_peak_detection_threshold(self):
         # Test for empty SpikeTrain when threshold is too high
-        result = stgen.threshold_detection(self.vm, threshold=30 * mV)
+        result = stgen.threshold_detection(self.vm, threshold=30 * pq.mV)
         self.assertEqual(len(result), 0)
 
 
 class AnalogSignalPeakDetectionTestCase(unittest.TestCase):
 
     def setUp(self):
         curr_dir = os.path.dirname(os.path.realpath(__file__))
         raw_data_file_loc = os.path.join(
             curr_dir, 'spike_extraction_test_data.txt')
         raw_data = []
         with open(raw_data_file_loc, 'r') as f:
-            for x in (f.readlines()):
+            for x in f.readlines():
                 raw_data.append(float(x))
-        self.vm = neo.AnalogSignal(raw_data, units=V, sampling_period=0.1 * ms)
+        self.vm = neo.AnalogSignal(
+            raw_data, units=pq.V, sampling_period=0.1 * pq.ms)
         self.true_time_stamps = [0.0124, 0.0354, 0.0713, 0.1192, 0.1695,
-                                 0.2201, 0.2711] * second
+                                 0.2201, 0.2711] * pq.s
 
     def test_peak_detection_time_stamps(self):
         # Test with default arguments
         result = stgen.peak_detection(self.vm)
         self.assertEqual(len(self.true_time_stamps), len(result))
         self.assertIsInstance(result, neo.core.SpikeTrain)
 
         try:
             assert_array_almost_equal(result, self.true_time_stamps)
         except AttributeError:
             self.assertTrue(np.array_equal(result, self.true_time_stamps))
 
     def test_peak_detection_threshold(self):
         # Test for empty SpikeTrain when threshold is too high
-        result = stgen.peak_detection(self.vm, threshold=30 * mV)
+        result = stgen.peak_detection(self.vm, threshold=30 * pq.mV)
         self.assertEqual(len(result), 0)
 
 
 class AnalogSignalSpikeExtractionTestCase(unittest.TestCase):
 
     def setUp(self):
         curr_dir = os.path.dirname(os.path.realpath(__file__))
         raw_data_file_loc = os.path.join(
             curr_dir, 'spike_extraction_test_data.txt')
         raw_data = []
         with open(raw_data_file_loc, 'r') as f:
-            for x in (f.readlines()):
+            for x in f.readlines():
                 raw_data.append(float(x))
-        self.vm = neo.AnalogSignal(raw_data, units=V, sampling_period=0.1 * ms)
+        self.vm = neo.AnalogSignal(
+            raw_data, units=pq.V, sampling_period=0.1 * pq.ms)
         self.first_spike = np.array([-0.04084546, -0.03892033, -0.03664779,
                                      -0.03392689, -0.03061474, -0.02650277,
                                      -0.0212756, -0.01443531, -0.00515365,
                                      0.00803962, 0.02797951, -0.07,
                                      -0.06974495, -0.06950466, -0.06927778,
                                      -0.06906314, -0.06885969, -0.06866651,
                                      -0.06848277, -0.06830773, -0.06814071,
                                      -0.06798113, -0.06782843, -0.06768213,
                                      -0.06754178, -0.06740699, -0.06727737,
                                      -0.06715259, -0.06703235, -0.06691635])
 
     def test_spike_extraction_waveform(self):
         spike_train = stgen.spike_extraction(self.vm.reshape(-1),
-                                             interval=(-1 * ms, 2 * ms))
+                                             interval=(-1 * pq.ms, 2 * pq.ms))
         try:
             assert_array_almost_equal(
                 spike_train.waveforms[0][0].magnitude.reshape(-1),
                 self.first_spike)
         except AttributeError:
             self.assertTrue(
                 np.array_equal(spike_train.waveforms[0][0].magnitude,
@@ -152,99 +156,99 @@
 class HomogeneousPoissonProcessTestCase(unittest.TestCase):
 
     def test_statistics(self):
         # This is a statistical test that has a non-zero chance of failure
         # during normal operation. Thus, we set the random seed to a value that
         # creates a realization passing the test.
 
-        for rate in [123.0 * Hz, 0.123 * kHz]:
-            for t_stop in [2345 * ms, 2.345 * second]:
+        for rate in [123.0 * pq.Hz, 0.123 * pq.kHz]:
+            for t_stop in [2345 * pq.ms, 2.345 * pq.s]:
                 # zero refractory period should act as no refractory period
-                for refractory_period in (None, 0 * ms):
+                for refractory_period in (None, 0 * pq.ms):
                     np.random.seed(seed=12345)
                     spiketrain = stgen.homogeneous_poisson_process(
                         rate, t_stop=t_stop,
                         refractory_period=refractory_period)
                     intervals = isi(spiketrain)
 
                     expected_mean_isi = 1. / rate.simplified
                     self.assertAlmostEqual(
                         expected_mean_isi.magnitude,
                         intervals.mean().simplified.magnitude,
                         places=3)
 
-                    expected_first_spike = 0 * ms
+                    expected_first_spike = 0 * pq.ms
                     self.assertLess(
                         spiketrain[0] - expected_first_spike,
                         7 * expected_mean_isi)
 
                     expected_last_spike = t_stop
                     self.assertLess(expected_last_spike -
                                     spiketrain[-1], 7 * expected_mean_isi)
 
                     # Kolmogorov-Smirnov test
-                    D, p = kstest(intervals.rescale(t_stop.units),
-                                  "expon",
-                                  # args are (loc, scale)
-                                  args=(
-                        0, expected_mean_isi.rescale(
-                            t_stop.units)),
+                    D, p = kstest(
+                        intervals.rescale(t_stop.units),
+                        "expon",
+                        # args are (loc, scale)
+                        args=(0,
+                              expected_mean_isi.rescale(t_stop.units)),
                         alternative='two-sided')
                     self.assertGreater(p, 0.001)
                     self.assertLess(D, 0.12)
 
     def test_zero_refractory_period(self):
-        rate = 10 * Hz
-        t_stop = 20 * s
+        rate = 10 * pq.Hz
+        t_stop = 20 * pq.s
         np.random.seed(27)
         sp1 = stgen.homogeneous_poisson_process(rate, t_stop=t_stop,
                                                 as_array=True)
         np.random.seed(27)
         sp2 = stgen.homogeneous_poisson_process(rate, t_stop=t_stop,
-                                                refractory_period=0 * ms,
+                                                refractory_period=0 * pq.ms,
                                                 as_array=True)
         assert_array_almost_equal(sp1, sp2)
 
     def test_t_start_and_t_stop(self):
-        rate = 10 * Hz
-        t_start = 17 * ms
-        t_stop = 2 * s
-        for refractory_period in (None, 3 * ms):
+        rate = 10 * pq.Hz
+        t_start = 17 * pq.ms
+        t_stop = 2 * pq.s
+        for refractory_period in (None, 3 * pq.ms):
             spiketrain = stgen.homogeneous_poisson_process(
                 rate=rate, t_start=t_start, t_stop=t_stop,
                 refractory_period=refractory_period)
             self.assertEqual(spiketrain.t_start, t_start)
             self.assertEqual(spiketrain.t_stop, t_stop)
 
     def test_zero_rate(self):
-        for refractory_period in (None, 3 * ms):
+        for refractory_period in (None, 3 * pq.ms):
             with warnings.catch_warnings():
                 warnings.simplefilter("ignore")
                 """
                 Catch RuntimeWarning: divide by zero encountered in true_divide
                 mean_interval = 1 / rate.magnitude, when rate == 0 Hz.
                 """
                 sp = stgen.homogeneous_poisson_process(
-                    rate=0 * Hz, t_stop=10 * s,
+                    rate=0 * pq.Hz, t_stop=10 * pq.s,
                     refractory_period=refractory_period)
                 self.assertEqual(sp.size, 0)
 
     def test_nondecrease_spike_times(self):
-        for refractory_period in (None, 3 * ms):
+        for refractory_period in (None, 3 * pq.ms):
             np.random.seed(27)
             spiketrain = stgen.homogeneous_poisson_process(
-                rate=10 * Hz, t_stop=1000 * s,
+                rate=10 * pq.Hz, t_stop=1000 * pq.s,
                 refractory_period=refractory_period)
             diffs = np.diff(spiketrain.times)
             self.assertTrue((diffs >= 0).all())
 
     def test_compare_with_as_array(self):
-        rate = 10 * Hz
-        t_stop = 10 * s
-        for refractory_period in (None, 3 * ms):
+        rate = 10 * pq.Hz
+        t_stop = 10 * pq.s
+        for refractory_period in (None, 3 * pq.ms):
             np.random.seed(27)
             spiketrain = stgen.homogeneous_poisson_process(
                 rate=rate, t_stop=t_stop, refractory_period=refractory_period)
             self.assertIsInstance(spiketrain, neo.SpikeTrain)
             np.random.seed(27)
             spiketrain_array = stgen.homogeneous_poisson_process(
                 rate=rate, t_stop=t_stop, refractory_period=refractory_period,
@@ -252,68 +256,177 @@
             # don't check with isinstance: Quantity is a subclass of np.ndarray
             self.assertTrue(isinstance(spiketrain_array, np.ndarray))
             assert_array_almost_equal(spiketrain.times.magnitude,
                                       spiketrain_array)
 
     def test_effective_rate_refractory_period(self):
         np.random.seed(27)
-        rate_expected = 10 * Hz
-        refractory_period = 90 * ms  # 10 ms of effective ISI
+        rate_expected = 10 * pq.Hz
+        refractory_period = 90 * pq.ms  # 10 ms of effective ISI
         spiketrain = stgen.homogeneous_poisson_process(
-            rate_expected, t_stop=1000 * s,
+            rate_expected, t_stop=1000 * pq.s,
             refractory_period=refractory_period)
         rate_obtained = len(spiketrain) / spiketrain.t_stop
         rate_obtained = rate_obtained.simplified
         self.assertAlmostEqual(rate_expected.simplified,
                                rate_obtained.simplified, places=1)
         intervals = isi(spiketrain)
         isi_mean_expected = 1. / rate_expected
         self.assertAlmostEqual(isi_mean_expected.simplified,
                                intervals.mean().simplified, places=3)
 
     def test_invalid(self):
-        rate = 10 * Hz
-        for refractory_period in (None, 3 * ms):
+        rate = 10 * pq.Hz
+        for refractory_period in (None, 3 * pq.ms):
             # t_stop < t_start
             hpp = stgen.homogeneous_poisson_process
             self.assertRaises(
-                ValueError, hpp, rate=rate, t_start=5 * ms,
-                t_stop=1 * ms, refractory_period=refractory_period)
+                ValueError, hpp, rate=rate, t_start=5 * pq.ms,
+                t_stop=1 * pq.ms, refractory_period=refractory_period)
 
             # no units provided for rate, t_stop
             self.assertRaises(ValueError, hpp, rate=10,
                               refractory_period=refractory_period)
             self.assertRaises(ValueError, hpp, rate=rate, t_stop=5,
                               refractory_period=refractory_period)
 
         # no units provided for refractory_period
         self.assertRaises(ValueError, hpp, rate=rate, refractory_period=2)
 
 
+class InhomogeneousGammaTestCase(unittest.TestCase):
+    def setUp(self):
+        rate_list = [[20]] * 1000 + [[200]] * 1000
+        self.rate_profile = neo.AnalogSignal(
+            rate_list * pq.Hz, sampling_period=0.001 * pq.s)
+        rate_0 = [[0]] * 1000
+        self.rate_profile_0 = neo.AnalogSignal(
+            rate_0 * pq.Hz, sampling_period=0.001 * pq.s)
+        rate_negative = [[-1]] * 1000
+        self.rate_profile_negative = neo.AnalogSignal(
+            rate_negative * pq.Hz, sampling_period=0.001 * pq.s)
+
+    def test_statistics(self):
+        # This is a statistical test that has a non-zero chance of failure
+        # during normal operation. Thus, we set the random seed to a value that
+        # creates a realization passing the test.
+        np.random.seed(seed=12345)
+
+        shape_factor = 2.5
+
+        for rate in [self.rate_profile, self.rate_profile.rescale(pq.kHz)]:
+            spiketrain = stgen.inhomogeneous_gamma_process(
+                rate, shape_factor=shape_factor)
+            intervals = isi(spiketrain)
+
+            # Computing expected statistics and percentiles
+            expected_spike_count = (np.sum(
+                rate) * rate.sampling_period).simplified
+            percentile_count = poisson.ppf(.999, expected_spike_count)
+            expected_min_isi = (1 / np.min(rate))
+            expected_max_isi = (1 / np.max(rate))
+            percentile_min_isi = expon.ppf(.999, expected_min_isi)
+            percentile_max_isi = expon.ppf(.999, expected_max_isi)
+
+            # Testing (each should fail 1 every 1000 times)
+            self.assertLess(spiketrain.size, percentile_count)
+            self.assertLess(np.min(intervals), percentile_min_isi)
+            self.assertLess(np.max(intervals), percentile_max_isi)
+
+            # Testing t_start t_stop
+            self.assertEqual(rate.t_stop, spiketrain.t_stop)
+            self.assertEqual(rate.t_start, spiketrain.t_start)
+
+        # Testing type
+        spiketrain_as_array = stgen.inhomogeneous_gamma_process(
+            rate, shape_factor=shape_factor, as_array=True)
+        self.assertTrue(isinstance(spiketrain_as_array, np.ndarray))
+        self.assertTrue(isinstance(spiketrain, neo.SpikeTrain))
+
+        # check error if rate has wrong format
+        self.assertRaises(
+            ValueError, stgen.inhomogeneous_gamma_process,
+            rate=[0.1, 2.],
+            shape_factor=shape_factor)
+
+        # check error if negative values in rate
+        self.assertRaises(
+            ValueError, stgen.inhomogeneous_gamma_process,
+            rate=neo.AnalogSignal([-0.1, 10.] * pq.Hz,
+                                  sampling_period=0.001 * pq.s),
+            shape_factor=shape_factor)
+
+        # check error if rate is empty
+        self.assertRaises(
+            ValueError, stgen.inhomogeneous_gamma_process,
+            rate=neo.AnalogSignal([] * pq.Hz, sampling_period=0.001 * pq.s),
+            shape_factor=shape_factor)
+
+    def test_recovered_firing_rate_profile(self):
+        np.random.seed(54)
+        t_start = 0 * pq.s
+        t_stop = 4 * np.round(np.pi, decimals=3) * pq.s  # 2 full periods
+        sampling_period = 0.001 * pq.s
+
+        # an arbitrary rate profile
+        profile = 0.5 * (1 + np.sin(np.arange(t_start.item(), t_stop.item(),
+                                              sampling_period.item())))
+
+        time_generation = 0
+        n_trials = 200
+        rtol = 0.05  # 5% of deviation allowed
+        kernel = kernels.RectangularKernel(sigma=0.25 * pq.s)
+        for rate in (10 * pq.Hz, 100 * pq.Hz):
+            rate_profile = neo.AnalogSignal(rate * profile,
+                                            sampling_period=sampling_period)
+            # the recovered firing rate profile should not depend on the
+            # shape factor; here we test float and integer values of the shape
+            # factor: the method supports float values that is not trivial
+            # for inhomogeneous gamma process generation
+            for shape_factor in (1, 2.5, 10.):
+
+                spiketrains = \
+                    [stgen.inhomogeneous_gamma_process(
+                        rate_profile, shape_factor=shape_factor)
+                     for _ in range(n_trials)]
+                rate_recovered = instantaneous_rate(
+                    spiketrains,
+                    sampling_period=sampling_period,
+                    kernel=kernel,
+                    t_start=t_start,
+                    t_stop=t_stop, trim=True).sum(axis=1) / n_trials
+
+                rate_recovered = rate_recovered.flatten().magnitude
+                trim = (rate_profile.shape[0] - rate_recovered.shape[0]) // 2
+                rate_profile_valid = rate_profile.magnitude.squeeze()
+                rate_profile_valid = rate_profile_valid[trim: -trim - 1]
+                assert_allclose(rate_recovered, rate_profile_valid,
+                                rtol=0, atol=rtol * rate.item())
+
+
 class InhomogeneousPoissonProcessTestCase(unittest.TestCase):
     def setUp(self):
         rate_list = [[20]] * 1000 + [[200]] * 1000
         self.rate_profile = neo.AnalogSignal(
-            rate_list * Hz, sampling_period=0.001 * s)
+            rate_list * pq.Hz, sampling_period=0.001 * pq.s)
         rate_0 = [[0]] * 1000
         self.rate_profile_0 = neo.AnalogSignal(
-            rate_0 * Hz, sampling_period=0.001 * s)
+            rate_0 * pq.Hz, sampling_period=0.001 * pq.s)
         rate_negative = [[-1]] * 1000
         self.rate_profile_negative = neo.AnalogSignal(
-            rate_negative * Hz, sampling_period=0.001 * s)
-        pass
+            rate_negative * pq.Hz, sampling_period=0.001 * pq.s)
 
     def test_statistics(self):
         # This is a statistical test that has a non-zero chance of failure
         # during normal operation. Thus, we set the random seed to a value that
         # creates a realization passing the test.
         np.random.seed(seed=12345)
 
-        for rate in [self.rate_profile, self.rate_profile.rescale(kHz)]:
-            for refractory_period in [3 * ms, None]:
+        for rate in (self.rate_profile, self.rate_profile.rescale(pq.kHz)):
+            for refractory_period in (3 * pq.ms, None):
                 spiketrain = stgen.inhomogeneous_poisson_process(
                     rate, refractory_period=refractory_period)
                 intervals = isi(spiketrain)
 
                 # Computing expected statistics and percentiles
                 expected_spike_count = (np.sum(
                     rate) * rate.sampling_period).simplified
@@ -339,59 +452,59 @@
         # Testing type
         spiketrain_as_array = stgen.inhomogeneous_poisson_process(
             rate, as_array=True)
         self.assertTrue(isinstance(spiketrain_as_array, np.ndarray))
         self.assertTrue(isinstance(spiketrain, neo.SpikeTrain))
 
         # Testing type for refractory period
-        refractory_period = 3 * ms
+        refractory_period = 3 * pq.ms
         spiketrain = stgen.inhomogeneous_poisson_process(
             rate, refractory_period=refractory_period)
         spiketrain_as_array = stgen.inhomogeneous_poisson_process(
             rate, as_array=True, refractory_period=refractory_period)
         self.assertTrue(isinstance(spiketrain_as_array, np.ndarray))
         self.assertTrue(isinstance(spiketrain, neo.SpikeTrain))
 
         # Check that to high refractory period raises error
         self.assertRaises(
             ValueError, stgen.inhomogeneous_poisson_process,
             self.rate_profile,
-            refractory_period=1000 * ms)
+            refractory_period=1000 * pq.ms)
 
     def test_effective_rate_refractory_period(self):
         np.random.seed(27)
-        rate_expected = 10 * Hz
-        refractory_period = 90 * ms  # 10 ms of effective ISI
-        rates = neo.AnalogSignal(np.repeat(rate_expected, 1000), units=Hz,
-                                 t_start=0 * ms, sampling_rate=1 * Hz)
+        rate_expected = 10 * pq.Hz
+        refractory_period = 90 * pq.ms  # 10 ms of effective ISI
+        rates = neo.AnalogSignal(np.repeat(rate_expected, 1000), units=pq.Hz,
+                                 t_start=0 * pq.ms, sampling_rate=1 * pq.Hz)
         spiketrain = stgen.inhomogeneous_poisson_process(
             rates, refractory_period=refractory_period)
         rate_obtained = len(spiketrain) / spiketrain.t_stop
         self.assertAlmostEqual(rate_expected, rate_obtained.simplified,
                                places=1)
         intervals_inhomo = isi(spiketrain)
         isi_mean_expected = 1. / rate_expected
         self.assertAlmostEqual(isi_mean_expected.simplified,
                                intervals_inhomo.mean().simplified,
                                places=3)
 
     def test_zero_rate(self):
-        for refractory_period in [3 * ms, None]:
+        for refractory_period in (3 * pq.ms, None):
             with warnings.catch_warnings():
                 warnings.simplefilter("ignore")
                 """
                 Catch RuntimeWarning: divide by zero encountered in true_divide
                 mean_interval = 1 / rate.magnitude, when rate == 0 Hz.
                 """
                 spiketrain = stgen.inhomogeneous_poisson_process(
                     self.rate_profile_0, refractory_period=refractory_period)
             self.assertEqual(spiketrain.size, 0)
 
     def test_negative_rates(self):
-        for refractory_period in [3 * ms, None]:
+        for refractory_period in (3 * pq.ms, None):
             self.assertRaises(
                 ValueError, stgen.inhomogeneous_poisson_process,
                 self.rate_profile_negative,
                 refractory_period=refractory_period)
 
 
 class HomogeneousGammaProcessTestCase(unittest.TestCase):
@@ -399,30 +512,30 @@
     def test_statistics(self):
         # This is a statistical test that has a non-zero chance of failure
         # during normal operation. Thus, we set the random seed to a value that
         # creates a realization passing the test.
         np.random.seed(seed=12345)
 
         a = 3.0
-        for b in (67.0 * Hz, 0.067 * kHz):
-            for t_stop in (2345 * ms, 2.345 * second):
+        for b in (67.0 * pq.Hz, 0.067 * pq.kHz):
+            for t_stop in (2345 * pq.ms, 2.345 * pq.s):
                 spiketrain = stgen.homogeneous_gamma_process(
                     a, b, t_stop=t_stop)
                 intervals = isi(spiketrain)
 
                 expected_spike_count = int((b / a * t_stop).simplified)
                 # should fail about 1 time in 1000
                 self.assertLess(
                     pdiff(expected_spike_count, spiketrain.size), 0.25)
 
-                expected_mean_isi = (a / b).rescale(ms)
+                expected_mean_isi = (a / b).rescale(pq.ms)
                 self.assertLess(
                     pdiff(expected_mean_isi, intervals.mean()), 0.3)
 
-                expected_first_spike = 0 * ms
+                expected_first_spike = 0 * pq.ms
                 self.assertLess(
                     spiketrain[0] - expected_first_spike,
                     4 * expected_mean_isi)
 
                 expected_last_spike = t_stop
                 self.assertLess(expected_last_spike -
                                 spiketrain[-1], 4 * expected_mean_isi)
@@ -434,15 +547,15 @@
                               args=(a, 0, (1 / b).rescale(t_stop.units)),
                               alternative='two-sided')
                 self.assertGreater(p, 0.001)
                 self.assertLess(D, 0.25)
 
     def test_compare_with_as_array(self):
         a = 3.
-        b = 10 * Hz
+        b = 10 * pq.Hz
         np.random.seed(27)
         spiketrain = stgen.homogeneous_gamma_process(a=a, b=b)
         self.assertIsInstance(spiketrain, neo.SpikeTrain)
         np.random.seed(27)
         spiketrain_array = stgen.homogeneous_gamma_process(a=a, b=b,
                                                            as_array=True)
         # don't check with isinstance: pq.Quantity is a subclass of np.ndarray
@@ -450,80 +563,80 @@
         assert_array_almost_equal(spiketrain.times.magnitude, spiketrain_array)
 
 
 class _n_poisson_TestCase(unittest.TestCase):
 
     def setUp(self):
         self.n = 4
-        self.rate = 10 * Hz
-        self.rates = range(1, self.n + 1) * Hz
-        self.t_stop = 10000 * ms
+        self.rate = 10 * pq.Hz
+        self.rates = np.arange(1, self.n + 1) * pq.Hz
+        self.t_stop = 10000 * pq.ms
 
     def test_poisson(self):
 
         # Check the output types for input rate + n number of neurons
         pp = stgen._n_poisson(
             rate=self.rate,
             t_stop=self.t_stop,
             n_spiketrains=self.n)
         self.assertIsInstance(pp, list)
         self.assertIsInstance(pp[0], neo.core.spiketrain.SpikeTrain)
-        self.assertEqual(pp[0].simplified.units, 1000 * ms)
+        self.assertEqual(pp[0].simplified.units, 1000 * pq.ms)
         self.assertEqual(len(pp), self.n)
 
         # Check the output types for input list of rates
         pp = stgen._n_poisson(rate=self.rates, t_stop=self.t_stop)
         self.assertIsInstance(pp, list)
         self.assertIsInstance(pp[0], neo.core.spiketrain.SpikeTrain)
-        self.assertEqual(pp[0].simplified.units, 1000 * ms)
+        self.assertEqual(pp[0].simplified.units, 1000 * pq.ms)
         self.assertEqual(len(pp), self.n)
 
     def test_poisson_error(self):
 
         # Dimensionless rate
         self.assertRaises(
             ValueError, stgen._n_poisson, rate=5, t_stop=self.t_stop)
         # Negative rate
         self.assertRaises(
-            ValueError, stgen._n_poisson, rate=-5 * Hz, t_stop=self.t_stop)
+            ValueError, stgen._n_poisson, rate=-5 * pq.Hz, t_stop=self.t_stop)
         # Negative value when rate is a list
         self.assertRaises(
-            ValueError, stgen._n_poisson, rate=[-5, 3] * Hz,
+            ValueError, stgen._n_poisson, rate=[-5, 3] * pq.Hz,
             t_stop=self.t_stop)
         # Negative n
         self.assertRaises(
             ValueError, stgen._n_poisson, rate=self.rate, t_stop=self.t_stop,
-            n=-1)
+            n_spiketrains=-1)
         # t_start>t_stop
         self.assertRaises(
-            ValueError, stgen._n_poisson, rate=self.rate, t_start=4 * ms,
-            t_stop=3 * ms, n=3)
+            ValueError, stgen._n_poisson, rate=self.rate, t_start=4 * pq.ms,
+            t_stop=3 * pq.ms, n_spiketrains=3)
 
 
 class singleinteractionprocess_TestCase(unittest.TestCase):
     def setUp(self):
         self.n = 4
-        self.rate = 10 * Hz
-        self.rates = range(1, self.n + 1) * Hz
-        self.t_stop = 10000 * ms
-        self.rate_c = 1 * Hz
+        self.rate = 10 * pq.Hz
+        self.rates = np.arange(1, self.n + 1) * pq.Hz
+        self.t_stop = 10000 * pq.ms
+        self.rate_c = 1 * pq.Hz
 
     def test_sip(self):
 
         # Generate an example SIP mode
         sip, coinc = stgen.single_interaction_process(
             n_spiketrains=self.n, t_stop=self.t_stop, rate=self.rate,
             coincidence_rate=self.rate_c, return_coincidences=True)
 
         # Check the output types
         self.assertEqual(type(sip), list)
         self.assertEqual(type(sip[0]), neo.core.spiketrain.SpikeTrain)
         self.assertEqual(type(coinc[0]), neo.core.spiketrain.SpikeTrain)
-        self.assertEqual(sip[0].simplified.units, 1000 * ms)
-        self.assertEqual(coinc[0].simplified.units, 1000 * ms)
+        self.assertEqual(sip[0].simplified.units, 1000 * pq.ms)
+        self.assertEqual(coinc[0].simplified.units, 1000 * pq.ms)
 
         # Check the output length
         self.assertEqual(len(sip), self.n)
         self.assertEqual(
             len(coinc[0]), (self.rate_c * self.t_stop).simplified.magnitude)
 
         with warnings.catch_warnings():
@@ -533,339 +646,390 @@
                 t_stop=self.t_stop, rate=self.rates,
                 coincidence_rate=self.rate_c, return_coincidences=True)
 
         # Check the output types
         self.assertEqual(type(sip), list)
         self.assertEqual(type(sip[0]), neo.core.spiketrain.SpikeTrain)
         self.assertEqual(type(coinc[0]), neo.core.spiketrain.SpikeTrain)
-        self.assertEqual(sip[0].simplified.units, 1000 * ms)
-        self.assertEqual(coinc[0].simplified.units, 1000 * ms)
+        self.assertEqual(sip[0].simplified.units, 1000 * pq.ms)
+        self.assertEqual(coinc[0].simplified.units, 1000 * pq.ms)
 
         # Check the output length
         self.assertEqual(len(sip), self.n)
         self.assertEqual(
-            len(coinc[0]), (self.rate_c * self.t_stop).rescale(dimensionless))
+            len(coinc[0]),
+            (self.rate_c * self.t_stop).rescale(pq.dimensionless))
 
         # Generate an example SIP mode stochastic number of coincidences
         sip = stgen.single_interaction_process(
             n_spiketrains=self.n,
             t_stop=self.t_stop,
             rate=self.rate,
             coincidence_rate=self.rate_c,
             coincidences='stochastic',
             return_coincidences=False)
 
         # Check the output types
         self.assertEqual(type(sip), list)
         self.assertEqual(type(sip[0]), neo.core.spiketrain.SpikeTrain)
-        self.assertEqual(sip[0].simplified.units, 1000 * ms)
+        self.assertEqual(sip[0].simplified.units, 1000 * pq.ms)
 
     def test_sip_error(self):
         # Negative rate
         self.assertRaises(
             ValueError, stgen.single_interaction_process, n_spiketrains=self.n,
-            rate=-5 * Hz,
+            rate=-5 * pq.Hz,
             coincidence_rate=self.rate_c, t_stop=self.t_stop)
         # Negative coincidence rate
         self.assertRaises(
             ValueError, stgen.single_interaction_process, n_spiketrains=self.n,
-            rate=self.rate, coincidence_rate=-3 * Hz, t_stop=self.t_stop)
+            rate=self.rate, coincidence_rate=-3 * pq.Hz, t_stop=self.t_stop)
         # Negative value when rate is a list
         self.assertRaises(
             ValueError, stgen.single_interaction_process, n_spiketrains=self.n,
-            rate=[-5, 3, 4, 2] * Hz, coincidence_rate=self.rate_c,
+            rate=[-5, 3, 4, 2] * pq.Hz, coincidence_rate=self.rate_c,
             t_stop=self.t_stop)
         # Negative n
         self.assertRaises(
             ValueError, stgen.single_interaction_process, n_spiketrains=-1,
             rate=self.rate, coincidence_rate=self.rate_c, t_stop=self.t_stop)
         # Rate_c < rate
         self.assertRaises(
             ValueError,
             stgen.single_interaction_process,
             n_spiketrains=self.n,
             rate=self.rate,
-            coincidence_rate=self.rate + 1 * Hz,
+            coincidence_rate=self.rate + 1 * pq.Hz,
             t_stop=self.t_stop)
 
 
 class cppTestCase(unittest.TestCase):
     def test_cpp_hom(self):
         # testing output with generic inputs
-        A = [0, .9, .1]
-        t_stop = 10 * 1000 * ms
-        t_start = 5 * 1000 * ms
-        rate = 3 * Hz
-        cpp_hom = stgen.cpp(rate, A, t_stop, t_start=t_start)
+        amplitude_distribution = np.array([0, .9, .1])
+        t_stop = 10 * 1000 * pq.ms
+        t_start = 5 * 1000 * pq.ms
+        rate = 3 * pq.Hz
+        cpp_hom = stgen.cpp(rate, amplitude_distribution,
+                            t_stop, t_start=t_start)
         # testing the ouput formats
         self.assertEqual(
             [type(train) for train in cpp_hom],
             [neo.SpikeTrain] * len(cpp_hom))
-        self.assertEqual(cpp_hom[0].simplified.units, 1000 * ms)
+        self.assertEqual(cpp_hom[0].simplified.units, 1000 * pq.ms)
         self.assertEqual(type(cpp_hom), list)
         # testing quantities format of the output
         self.assertEqual(
-            [train.simplified.units for train in cpp_hom], [1000 * ms] * len(
-                cpp_hom))
+            [train.simplified.units for train in cpp_hom],
+            [1000 * pq.ms] * len(cpp_hom))
         # testing output t_start t_stop
         for st in cpp_hom:
             self.assertEqual(st.t_stop, t_stop)
             self.assertEqual(st.t_start, t_start)
-        self.assertEqual(len(cpp_hom), len(A) - 1)
+        self.assertEqual(len(cpp_hom), len(amplitude_distribution) - 1)
 
         # testing the units
-        A = [0, 0.9, 0.1]
-        t_stop = 10000 * ms
-        t_start = 5 * 1000 * ms
-        rate = 3 * Hz
-        cpp_unit = stgen.cpp(rate, A, t_stop, t_start=t_start)
+        t_stop = 10000 * pq.ms
+        t_start = 5 * 1000 * pq.ms
+        rate = 3 * pq.Hz
+        cpp_unit = stgen.cpp(rate, amplitude_distribution,
+                             t_stop, t_start=t_start)
 
         self.assertEqual(cpp_unit[0].units, t_stop.units)
         self.assertEqual(cpp_unit[0].t_stop.units, t_stop.units)
         self.assertEqual(cpp_unit[0].t_start.units, t_stop.units)
 
         # testing output without copy of spikes
-        A = [1]
-        t_stop = 10 * 1000 * ms
-        t_start = 5 * 1000 * ms
-        rate = 3 * Hz
-        cpp_hom_empty = stgen.cpp(rate, A, t_stop, t_start=t_start)
+        amplitude_distribution = np.array([1])
+        t_stop = 10 * 1000 * pq.ms
+        t_start = 5 * 1000 * pq.ms
+        rate = 3 * pq.Hz
+        cpp_hom_empty = stgen.cpp(
+            rate, amplitude_distribution, t_stop, t_start=t_start)
 
         self.assertEqual(
             [len(train) for train in cpp_hom_empty], [0] * len(cpp_hom_empty))
 
         # testing output with rate equal to 0
-        A = [0, .9, .1]
-        t_stop = 10 * 1000 * ms
-        t_start = 5 * 1000 * ms
-        rate = 0 * Hz
-        cpp_hom_empty_r = stgen.cpp(rate, A, t_stop, t_start=t_start)
+        amplitude_distribution = np.array([0, .9, .1])
+        t_stop = 10 * 1000 * pq.ms
+        t_start = 5 * 1000 * pq.ms
+        rate = 0 * pq.Hz
+        cpp_hom_empty_r = stgen.cpp(
+            rate, amplitude_distribution, t_stop, t_start=t_start)
         self.assertEqual(
             [len(train) for train in cpp_hom_empty_r], [0] * len(
                 cpp_hom_empty_r))
 
         # testing output with same spike trains in output
-        A = [0., 0., 1.]
-        t_stop = 10 * 1000 * ms
-        t_start = 5 * 1000 * ms
-        rate = 3 * Hz
-        cpp_hom_eq = stgen.cpp(rate, A, t_stop, t_start=t_start)
+        amplitude_distribution = np.array([0., 0., 1.])
+        t_stop = 10 * 1000 * pq.ms
+        t_start = 5 * 1000 * pq.ms
+        rate = 3 * pq.Hz
+        cpp_hom_eq = stgen.cpp(
+            rate, amplitude_distribution, t_stop, t_start=t_start)
 
         self.assertTrue(
             np.allclose(cpp_hom_eq[0].magnitude, cpp_hom_eq[1].magnitude))
 
     def test_cpp_hom_errors(self):
         # testing raises of ValueError (wrong inputs)
         # testing empty amplitude
         self.assertRaises(
-            ValueError, stgen.cpp, A=[], t_stop=10 * 1000 * ms,
-            rate=3 * Hz)
+            ValueError,
+            stgen.cpp,
+            amplitude_distribution=[],
+            t_stop=10 * 1000 * pq.ms,
+            rate=3 * pq.Hz)
 
         # testing sum of amplitude>1
         self.assertRaises(
-            ValueError, stgen.cpp, A=[1, 1, 1], t_stop=10 * 1000 * ms,
-            rate=3 * Hz)
+            ValueError,
+            stgen.cpp,
+            amplitude_distribution=[1, 1, 1],
+            t_stop=10 * 1000 * pq.ms,
+            rate=3 * pq.Hz)
         # testing negative value in the amplitude
         self.assertRaises(
-            ValueError, stgen.cpp, A=[-1, 1, 1],
-            t_stop=10 * 1000 * ms,
-            rate=3 * Hz)
+            ValueError, stgen.cpp, amplitude_distribution=[-1, 1, 1],
+            t_stop=10 * 1000 * pq.ms,
+            rate=3 * pq.Hz)
         # test negative rate
         with warnings.catch_warnings():
             warnings.simplefilter("ignore")
             """
             Catches RuntimeWarning: invalid value encountered in sqrt
             number = np.ceil(n + 3 * np.sqrt(n)), when `n` == -3 Hz.
             """
             self.assertRaises(
-                ValueError, stgen.cpp, A=[0, 1, 0],
-                t_stop=10 * 1000 * ms,
-                rate=-3 * Hz)
+                ValueError, stgen.cpp, amplitude_distribution=[0, 1, 0],
+                t_stop=10 * 1000 * pq.ms,
+                rate=-3 * pq.Hz)
         # test wrong unit for rate
         self.assertRaises(
-            ValueError, stgen.cpp, A=[0, 1, 0], t_stop=10 * 1000 * ms,
-            rate=3 * 1000 * ms)
+            ValueError,
+            stgen.cpp,
+            amplitude_distribution=[0, 1, 0],
+            t_stop=10 * 1000 * pq.ms,
+            rate=3 * 1000 * pq.ms)
 
         # testing raises of AttributeError (missing input units)
         # Testing missing unit to t_stop
         self.assertRaises(
-            ValueError, stgen.cpp, A=[0, 1, 0], t_stop=10,
-            rate=3 * Hz)
+            ValueError, stgen.cpp, amplitude_distribution=[0, 1, 0], t_stop=10,
+            rate=3 * pq.Hz)
         # Testing missing unit to t_start
         self.assertRaises(
-            ValueError, stgen.cpp, A=[0, 1, 0], t_stop=10 * 1000 * ms,
-            rate=3 * Hz,
+            ValueError,
+            stgen.cpp,
+            amplitude_distribution=[0, 1, 0],
+            t_stop=10 * 1000 * pq.ms,
+            rate=3 * pq.Hz,
             t_start=3)
         # testing rate missing unit
         self.assertRaises(
-            AttributeError, stgen.cpp, A=[0, 1, 0],
-            t_stop=10 * 1000 * ms,
+            AttributeError, stgen.cpp, amplitude_distribution=[0, 1, 0],
+            t_stop=10 * 1000 * pq.ms,
             rate=3)
 
     def test_cpp_het(self):
         # testing output with generic inputs
-        A = [0, .9, .1]
-        t_stop = 10 * 1000 * ms
-        t_start = 5 * 1000 * ms
-        rate = [3, 4] * Hz
+        amplitude_distribution = np.array([0, .9, .1])
+        t_stop = 10 * 1000 * pq.ms
+        t_start = 5 * 1000 * pq.ms
+        rate = [3, 4] * pq.Hz
         with warnings.catch_warnings():
             warnings.simplefilter("ignore")
             """
             Catch RuntimeWarning: divide by zero encountered in true_divide
             mean_interval = 1 / rate.magnitude, when rate == 0 Hz.
             """
-            cpp_het = stgen.cpp(rate, A, t_stop, t_start=t_start)
+            cpp_het = stgen.cpp(rate, amplitude_distribution,
+                                t_stop, t_start=t_start)
             # testing the ouput formats
             self.assertEqual(
                 [type(train) for train in cpp_het],
                 [neo.SpikeTrain] * len(cpp_het))
-            self.assertEqual(cpp_het[0].simplified.units, 1000 * ms)
+            self.assertEqual(cpp_het[0].simplified.units, 1000 * pq.ms)
             self.assertEqual(type(cpp_het), list)
             # testing units
             self.assertEqual(
                 [train.simplified.units for train in cpp_het],
-                [1000 * ms] * len(cpp_het))
+                [1000 * pq.ms] * len(cpp_het))
             # testing output t_start and t_stop
             for st in cpp_het:
                 self.assertEqual(st.t_stop, t_stop)
                 self.assertEqual(st.t_start, t_start)
             # testing the number of output spiketrains
-            self.assertEqual(len(cpp_het), len(A) - 1)
+            self.assertEqual(len(cpp_het), len(amplitude_distribution) - 1)
             self.assertEqual(len(cpp_het), len(rate))
 
             # testing the units
-            A = [0, 0.9, 0.1]
-            t_stop = 10000 * ms
-            t_start = 5 * 1000 * ms
-            rate = [3, 4] * Hz
-            cpp_unit = stgen.cpp(rate, A, t_stop, t_start=t_start)
+            t_stop = 10000 * pq.ms
+            t_start = 5 * 1000 * pq.ms
+            rate = [3, 4] * pq.Hz
+            cpp_unit = stgen.cpp(
+                rate, amplitude_distribution, t_stop, t_start=t_start)
 
             self.assertEqual(cpp_unit[0].units, t_stop.units)
             self.assertEqual(cpp_unit[0].t_stop.units, t_stop.units)
             self.assertEqual(cpp_unit[0].t_start.units, t_stop.units)
             # testing without copying any spikes
-            A = [1, 0, 0]
-            t_stop = 10 * 1000 * ms
-            t_start = 5 * 1000 * ms
-            rate = [3, 4] * Hz
-            cpp_het_empty = stgen.cpp(rate, A, t_stop, t_start=t_start)
+            amplitude_distribution = np.array([1, 0, 0])
+            t_stop = 10 * 1000 * pq.ms
+            t_start = 5 * 1000 * pq.ms
+            rate = [3, 4] * pq.Hz
+            cpp_het_empty = stgen.cpp(
+                rate, amplitude_distribution, t_stop, t_start=t_start)
 
             self.assertEqual(len(cpp_het_empty[0]), 0)
 
             # testing output with rate equal to 0
-            A = [0, .9, .1]
-            t_stop = 10 * 1000 * ms
-            t_start = 5 * 1000 * ms
-            rate = [0, 0] * Hz
-            cpp_het_empty_r = stgen.cpp(rate, A, t_stop, t_start=t_start)
+            amplitude_distribution = np.array([0, .9, .1])
+            t_stop = 10 * 1000 * pq.ms
+            t_start = 5 * 1000 * pq.ms
+            rate = [0, 0] * pq.Hz
+            cpp_het_empty_r = stgen.cpp(
+                rate, amplitude_distribution, t_stop, t_start=t_start)
             self.assertEqual(
                 [len(train) for train in cpp_het_empty_r], [0] * len(
                     cpp_het_empty_r))
 
             # testing completely sync spiketrains
-            A = [0, 0, 1]
-            t_stop = 10 * 1000 * ms
-            t_start = 5 * 1000 * ms
-            rate = [3, 3] * Hz
-            cpp_het_eq = stgen.cpp(rate, A, t_stop, t_start=t_start)
+            amplitude_distribution = np.array([0, 0, 1])
+            t_stop = 10 * 1000 * pq.ms
+            t_start = 5 * 1000 * pq.ms
+            rate = [3, 3] * pq.Hz
+            cpp_het_eq = stgen.cpp(
+                rate, amplitude_distribution, t_stop, t_start=t_start)
 
             self.assertTrue(np.allclose(
                 cpp_het_eq[0].magnitude, cpp_het_eq[1].magnitude))
 
     def test_cpp_het_err(self):
         # testing raises of ValueError (wrong inputs)
         # testing empty amplitude
         self.assertRaises(
-            ValueError, stgen.cpp, A=[], t_stop=10 * 1000 * ms,
-            rate=[3, 4] * Hz)
+            ValueError,
+            stgen.cpp,
+            amplitude_distribution=[],
+            t_stop=10 * 1000 * pq.ms,
+            rate=[3, 4] * pq.Hz)
         # testing sum amplitude>1
         self.assertRaises(
-            ValueError, stgen.cpp, A=[1, 1, 1], t_stop=10 * 1000 * ms,
-            rate=[3, 4] * Hz)
+            ValueError,
+            stgen.cpp,
+            amplitude_distribution=[1, 1, 1],
+            t_stop=10 * 1000 * pq.ms,
+            rate=[3, 4] * pq.Hz)
         # testing amplitude negative value
         self.assertRaises(
-            ValueError, stgen.cpp, A=[-1, 1, 1],
-            t_stop=10 * 1000 * ms,
-            rate=[3, 4] * Hz)
+            ValueError, stgen.cpp, amplitude_distribution=[-1, 1, 1],
+            t_stop=10 * 1000 * pq.ms,
+            rate=[3, 4] * pq.Hz)
         # testing negative rate
-        self.assertRaises(
-            ValueError, stgen.cpp, A=[0, 1, 0], t_stop=10 * 1000 * ms,
-            rate=[-3, 4] * Hz)
+        self.assertRaises(ValueError, stgen.cpp, amplitude_distribution=[
+            0, 1, 0], t_stop=10 * 1000 * pq.ms, rate=[-3, 4] * pq.Hz)
         # testing empty rate
         self.assertRaises(
-            ValueError, stgen.cpp, A=[0, 1, 0], t_stop=10 * 1000 * ms,
-            rate=[] * Hz)
+            ValueError,
+            stgen.cpp,
+            amplitude_distribution=[0, 1, 0],
+            t_stop=10 * 1000 * pq.ms,
+            rate=[] * pq.Hz)
         # testing empty amplitude
         self.assertRaises(
-            ValueError, stgen.cpp, A=[], t_stop=10 * 1000 * ms,
-            rate=[3, 4] * Hz)
+            ValueError,
+            stgen.cpp,
+            amplitude_distribution=[],
+            t_stop=10 * 1000 * pq.ms,
+            rate=[3, 4] * pq.Hz)
         # testing different len(A)-1 and len(rate)
         self.assertRaises(
-            ValueError, stgen.cpp, A=[0, 1], t_stop=10 * 1000 * ms,
-            rate=[3, 4] * Hz)
+            ValueError,
+            stgen.cpp,
+            amplitude_distribution=[0, 1],
+            t_stop=10 * 1000 * pq.ms,
+            rate=[3, 4] * pq.Hz)
         # testing rate with different unit from Hz
         self.assertRaises(
-            ValueError, stgen.cpp, A=[0, 1], t_stop=10 * 1000 * ms,
-            rate=[3, 4] * 1000 * ms)
+            ValueError,
+            stgen.cpp,
+            amplitude_distribution=[0, 1],
+            t_stop=10 * 1000 * pq.ms,
+            rate=[3, 4] * 1000 * pq.ms)
         # Testing analytical constrain between amplitude and rate
         self.assertRaises(
-            ValueError, stgen.cpp, A=[0, 0, 1], t_stop=10 * 1000 * ms,
-            rate=[3, 4] * Hz, t_start=3)
+            ValueError,
+            stgen.cpp,
+            amplitude_distribution=[0, 0, 1],
+            t_stop=10 * 1000 * pq.ms,
+            rate=[3, 4] * pq.Hz,
+            t_start=3)
 
         # testing raises of AttributeError (missing input units)
         # Testing missing unit to t_stop
         self.assertRaises(
-            ValueError, stgen.cpp, A=[0, 1, 0], t_stop=10,
-            rate=[3, 4] * Hz)
+            ValueError, stgen.cpp, amplitude_distribution=[0, 1, 0], t_stop=10,
+            rate=[3, 4] * pq.Hz)
         # Testing missing unit to t_start
         self.assertRaises(
-            ValueError, stgen.cpp, A=[0, 1, 0], t_stop=10 * 1000 * ms,
-            rate=[3, 4] * Hz, t_start=3)
+            ValueError,
+            stgen.cpp,
+            amplitude_distribution=[0, 1, 0],
+            t_stop=10 * 1000 * pq.ms,
+            rate=[3, 4] * pq.Hz,
+            t_start=3)
         # Testing missing unit to rate
         self.assertRaises(
-            AttributeError, stgen.cpp, A=[0, 1, 0],
-            t_stop=10 * 1000 * ms,
+            AttributeError, stgen.cpp, amplitude_distribution=[0, 1, 0],
+            t_stop=10 * 1000 * pq.ms,
             rate=[3, 4])
 
     def test_cpp_jttered(self):
         # testing output with generic inputs
-        A = [0, .9, .1]
-        t_stop = 10 * 1000 * ms
-        t_start = 5 * 1000 * ms
-        rate = 3 * Hz
+        amplitude_distribution = np.array([0, .9, .1])
+        t_stop = 10 * 1000 * pq.ms
+        t_start = 5 * 1000 * pq.ms
+        rate = 3 * pq.Hz
         cpp_shift = stgen.cpp(
-            rate, A, t_stop, t_start=t_start, shift=3 * ms)
+            rate,
+            amplitude_distribution,
+            t_stop,
+            t_start=t_start,
+            shift=3 * pq.ms)
         # testing the ouput formats
         self.assertEqual(
             [type(train) for train in cpp_shift], [neo.SpikeTrain] * len(
                 cpp_shift))
-        self.assertEqual(cpp_shift[0].simplified.units, 1000 * ms)
+        self.assertEqual(cpp_shift[0].simplified.units, 1000 * pq.ms)
         self.assertEqual(type(cpp_shift), list)
         # testing quantities format of the output
         self.assertEqual(
             [train.simplified.units for train in cpp_shift],
-            [1000 * ms] * len(cpp_shift))
+            [1000 * pq.ms] * len(cpp_shift))
         # testing output t_start t_stop
-        for st in cpp_shift:
-            self.assertEqual(st.t_stop, t_stop)
-            self.assertEqual(st.t_start, t_start)
-        self.assertEqual(len(cpp_shift), len(A) - 1)
+        for spiketrain in cpp_shift:
+            self.assertEqual(spiketrain.t_stop, t_stop)
+            self.assertEqual(spiketrain.t_start, t_start)
+        self.assertEqual(len(cpp_shift), len(amplitude_distribution) - 1)
 
 
 class HomogeneousPoissonProcessWithRefrPeriodTestCase(unittest.TestCase):
 
     def test_invalid(self):
-        rate = 10 * Hz
+        rate = 10 * pq.Hz
         # t_stop < t_start
         hpp = stgen.homogeneous_poisson_process
-        self.assertRaises(ValueError, hpp, rate=rate, t_start=5 * ms,
-                          t_stop=1 * ms, refractory_period=3 * ms)
+        self.assertRaises(ValueError, hpp, rate=rate, t_start=5 * pq.ms,
+                          t_stop=1 * pq.ms, refractory_period=3 * pq.ms)
 
         # no units provided
-        self.assertRaises(ValueError, hpp, rate=10, refractory_period=3 * ms)
+        self.assertRaises(ValueError, hpp, rate=10,
+                          refractory_period=3 * pq.ms)
         self.assertRaises(ValueError, hpp, rate=rate, t_stop=5,
-                          refractory_period=3 * ms)
+                          refractory_period=3 * pq.ms)
         self.assertRaises(ValueError, hpp, rate=rate, refractory_period=2)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `elephant-0.8.0/elephant/test/test_spike_train_surrogates.py` & `elephant-0.9.0/elephant/test/test_spike_train_surrogates.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,21 +3,23 @@
 unittests for spike_train_surrogates module.
 
 :copyright: Copyright 2014-2016 by the Elephant team, see `doc/authors.rst`.
 :license: Modified BSD, see LICENSE.txt for details.
 """
 
 import unittest
+import random
+
 import elephant.spike_train_surrogates as surr
 import elephant.spike_train_generation as stg
+import elephant.conversion as conv
 import numpy as np
 from numpy.testing import assert_array_almost_equal, assert_array_less
 import quantities as pq
 import neo
-import random
 
 
 class SurrogatesTestCase(unittest.TestCase):
 
     def setUp(self):
         np.random.seed(0)
         random.seed(0)
@@ -27,15 +29,14 @@
         spiketrain = neo.SpikeTrain([90, 93, 97, 100, 105,
                                      150, 180, 350] * pq.ms, t_stop=.5 * pq.s)
         spiketrain.t_stop = .5 * pq.s
         n_surrogates = 2
         dither = 10 * pq.ms
         surrogate_trains = surr.dither_spikes(
             spiketrain, dither=dither, n_surrogates=n_surrogates)
-        print(surrogate_trains)
 
         self.assertIsInstance(surrogate_trains, list)
         self.assertEqual(len(surrogate_trains), n_surrogates)
 
         self.assertIsInstance(surrogate_trains[0], neo.SpikeTrain)
         for surrogate_train in surrogate_trains:
             self.assertEqual(surrogate_train.units, spiketrain.units)
@@ -113,14 +114,17 @@
                                  np.min(np.diff(surrogate_train)))
             sigma_displacement = np.std(surrogate_train - spiketrain)
             # Check that spikes are moved
             self.assertLessEqual(dither / 10, sigma_displacement)
             # Spikes are not moved more than dither
             self.assertLessEqual(sigma_displacement, dither)
 
+        self.assertRaises(ValueError, surr.dither_spikes,
+                          spiketrain, dither=dither, refractory_period=3)
+
     def test_dither_spikes_with_refractory_period_empty_train(self):
 
         spiketrain = neo.SpikeTrain([] * pq.ms, t_stop=500 * pq.ms)
 
         dither = 10 * pq.ms
         surrogate_train = surr.dither_spikes(
             spiketrain, dither=dither, n_surrogates=1,
@@ -227,14 +231,32 @@
         ISIs_orig = np.sort([isi0_orig] + [isi for isi in np.diff(st_pq)])
 
         isi0_surr = surrogate_train[0] - surrogate_train.t_start
         ISIs_surr = np.sort([isi0_surr] + [isi for isi in np.diff(surr_pq)])
 
         self.assertTrue(np.all(ISIs_orig == ISIs_surr))
 
+    def test_shuffle_isis_with_wrongly_ordered_spikes(self):
+        surr_method = 'shuffle_isis'
+        n_surr = 30
+        dither = 15 * pq.ms
+        spiketrain = neo.SpikeTrain(
+            [39.65696411,  98.93868274, 120.2417674,  134.70971166,
+             154.20788924,
+             160.29077989, 179.19884034, 212.86773029, 247.59488061,
+             273.04095041,
+             297.56437605, 344.99204215, 418.55696486, 460.54298334,
+             482.82299125,
+             524.236052,   566.38966742, 597.87562722, 651.26965293,
+             692.39802855,
+             740.90285815, 849.45874695, 974.57724848,   8.79247605],
+            t_start=0.*pq.ms, t_stop=1000.*pq.ms, units=pq.ms)
+        surr.surrogates(spiketrain, n_surrogates=n_surr, method=surr_method,
+                        dt=dither)
+
     def test_dither_spike_train_output_format(self):
 
         spiketrain = neo.SpikeTrain(
             [90, 150, 180, 350] * pq.ms, t_stop=500 * pq.ms)
 
         n_surrogates = 2
         shift = 10 * pq.ms
@@ -367,63 +389,79 @@
                 pq.dimensionless).magnitude,
             dtype=int)
 
         self.assertTrue(np.all(bin_ids_orig == bin_ids_surr))
 
     def test_surr_method(self):
 
+        surr_methods = \
+            ('dither_spike_train', 'dither_spikes', 'jitter_spikes',
+             'randomise_spikes', 'shuffle_isis', 'joint_isi_dithering',
+             'dither_spikes_with_refractory_period', 'trial_shifting',
+             'bin_shuffling', 'isi_dithering')
+
+        surr_method_kwargs = \
+            {'dither_spikes': {},
+             'dither_spikes_with_refractory_period': {'refractory_period':
+                                                      3*pq.ms},
+             'randomise_spikes': {},
+             'shuffle_isis': {},
+             'dither_spike_train': {},
+             'jitter_spikes': {},
+             'bin_shuffling': {'bin_size': 3*pq.ms},
+             'joint_isi_dithering': {},
+             'isi_dithering': {},
+             'trial_shifting': {'trial_length': 200*pq.ms,
+                                'trial_separation': 50*pq.ms}}
+
+        dt = 15 * pq.ms
         spiketrain = neo.SpikeTrain(
             [90, 150, 180, 350] * pq.ms, t_stop=500 * pq.ms)
-        n_surrogates = 2
-        surrogate_trains = surr.surrogates(
-            spiketrain,
-            dt=3 * pq.ms,
-            n_surrogates=n_surrogates,
-            method='shuffle_isis',
-            edges=False)
-
-        self.assertRaises(ValueError, surr.surrogates, spiketrain, n=1,
-                          surr_method='spike_shifting',
+        n_surrogates = 3
+        for method in surr_methods:
+            surrogates = surr.surrogates(
+                spiketrain,
+                dt=dt,
+                n_surrogates=n_surrogates,
+                method=method,
+                **surr_method_kwargs[method]
+            )
+            self.assertTrue(len(surrogates) == n_surrogates)
+
+            for surrogate_train in surrogates:
+                self.assertTrue(
+                    isinstance(surrogates[0], neo.SpikeTrain))
+                self.assertEqual(surrogate_train.units, spiketrain.units)
+                self.assertEqual(surrogate_train.t_start, spiketrain.t_start)
+                self.assertEqual(surrogate_train.t_stop, spiketrain.t_stop)
+                self.assertEqual(len(surrogate_train), len(spiketrain))
+            self.assertTrue(len(surrogates) == n_surrogates)
+
+        self.assertRaises(ValueError, surr.surrogates, spiketrain,
+                          n_surrogates=1,
+                          method='spike_shifting',
                           dt=None, decimals=None, edges=True)
-        self.assertTrue(len(surrogate_trains) == n_surrogates)
 
-        n_surrogates2 = 4
-        surrogate_trains2 = surr.surrogates(
-            spiketrain,
-            dt=5 * pq.ms,
-            n_surrogates=n_surrogates2,
-            method='dither_spike_train',
-            edges=True)
+        self.assertRaises(ValueError, surr.surrogates, spiketrain,
+                          method='dither_spikes', dt=None)
 
-        for surrogate_train in surrogate_trains:
-            self.assertTrue(isinstance(surrogate_trains[0], neo.SpikeTrain))
-            self.assertEqual(surrogate_train.units, spiketrain.units)
-            self.assertEqual(surrogate_train.t_start, spiketrain.t_start)
-            self.assertEqual(surrogate_train.t_stop, spiketrain.t_stop)
-            self.assertEqual(len(surrogate_train), len(spiketrain))
-        self.assertTrue(len(surrogate_trains) == n_surrogates)
-
-        for surrogate_train in surrogate_trains2:
-            self.assertTrue(isinstance(surrogate_trains2[0], neo.SpikeTrain))
-            self.assertEqual(surrogate_train.units, spiketrain.units)
-            self.assertEqual(surrogate_train.t_start, spiketrain.t_start)
-            self.assertEqual(surrogate_train.t_stop, spiketrain.t_stop)
-            self.assertEqual(len(surrogate_train), len(spiketrain))
-        self.assertTrue(len(surrogate_trains2) == n_surrogates2)
+        self.assertRaises(TypeError, surr.surrogates, spiketrain.magnitude,
+                          method='dither_spikes', dt=10*pq.ms)
 
     def test_joint_isi_dithering_format(self):
 
         rate = 100. * pq.Hz
         t_stop = 1. * pq.s
         spiketrain = stg.homogeneous_poisson_process(rate, t_stop=t_stop)
         n_surrogates = 2
         dither = 10 * pq.ms
 
         # Test fast version
-        joint_isi_instance = surr.JointISI(spiketrain, dither=dither)
+        joint_isi_instance = surr.JointISI(spiketrain, dither=dither,
+                                           method='fast')
         surrogate_trains = joint_isi_instance.dithering(
             n_surrogates=n_surrogates)
 
         self.assertIsInstance(surrogate_trains, list)
         self.assertEqual(len(surrogate_trains), n_surrogates)
         self.assertEqual(joint_isi_instance.method, 'fast')
 
@@ -449,28 +487,56 @@
         for surrogate_train in surrogate_trains:
             self.assertIsInstance(surrogate_train, neo.SpikeTrain)
             self.assertEqual(surrogate_train.units, spiketrain.units)
             self.assertEqual(surrogate_train.t_start, spiketrain.t_start)
             self.assertEqual(surrogate_train.t_stop, spiketrain.t_stop)
             self.assertEqual(len(surrogate_train), len(spiketrain))
 
+        # Test isi_dithering
+        joint_isi_instance = surr.JointISI(spiketrain,
+                                           method='window',
+                                           dither=2 * dither,
+                                           n_bins=50,
+                                           isi_dithering=True,
+                                           use_sqrt=True,
+                                           cutoff=False)
+        surrogate_trains = joint_isi_instance.dithering(
+            n_surrogates=n_surrogates)
+
+        self.assertIsInstance(surrogate_trains, list)
+        self.assertEqual(len(surrogate_trains), n_surrogates)
+        self.assertEqual(joint_isi_instance.method, 'window')
+
+        for surrogate_train in surrogate_trains:
+            self.assertIsInstance(surrogate_train, neo.SpikeTrain)
+            self.assertEqual(surrogate_train.units, spiketrain.units)
+            self.assertEqual(surrogate_train.t_start, spiketrain.t_start)
+            self.assertEqual(surrogate_train.t_stop, spiketrain.t_stop)
+            self.assertEqual(len(surrogate_train), len(spiketrain))
+
         # Test surrogate methods wrapper
         surrogate_trains = surr.surrogates(
             spiketrain,
+            dt=15*pq.ms,
             n_surrogates=n_surrogates,
             method='joint_isi_dithering')
         self.assertIsInstance(surrogate_trains, list)
         self.assertEqual(len(surrogate_trains), n_surrogates)
 
         for surrogate_train in surrogate_trains:
             self.assertIsInstance(surrogate_train, neo.SpikeTrain)
             self.assertEqual(surrogate_train.units, spiketrain.units)
             self.assertEqual(surrogate_train.t_start, spiketrain.t_start)
             self.assertEqual(surrogate_train.t_stop, spiketrain.t_stop)
             self.assertEqual(len(surrogate_train), len(spiketrain))
+        with self.assertRaises(ValueError):
+            joint_isi_instance = surr.JointISI(spiketrain,
+                                               method='wrong method',
+                                               dither=2 * dither,
+                                               n_bins=50)
 
     def test_joint_isi_dithering_empty_train(self):
         spiketrain = neo.SpikeTrain([] * pq.ms, t_stop=500 * pq.ms)
         surrogate_train = surr.JointISI(spiketrain).dithering()[0]
         self.assertEqual(len(surrogate_train), 0)
 
     def test_joint_isi_dithering_output(self):
@@ -479,14 +545,161 @@
             refractory_period=3 * pq.ms,
             t_stop=0.1 * pq.s)
         surrogate_train = surr.JointISI(spiketrain).dithering()[0]
         ground_truth = [0.005571, 0.018363, 0.026825, 0.036336, 0.045193,
                         0.05146, 0.058489, 0.078053]
         assert_array_almost_equal(surrogate_train.magnitude, ground_truth)
 
+    def test_joint_isi_with_wrongly_ordered_spikes(self):
+        surr_method = 'joint_isi_dithering'
+        n_surr = 30
+        dither = 15 * pq.ms
+        spiketrain = neo.SpikeTrain(
+            [39.65696411,  98.93868274, 120.2417674,  134.70971166,
+             154.20788924,
+             160.29077989, 179.19884034, 212.86773029, 247.59488061,
+             273.04095041,
+             297.56437605, 344.99204215, 418.55696486, 460.54298334,
+             482.82299125,
+             524.236052,   566.38966742, 597.87562722, 651.26965293,
+             692.39802855,
+             740.90285815, 849.45874695, 974.57724848,   8.79247605],
+            t_start=0.*pq.ms, t_stop=1000.*pq.ms, units=pq.ms)
+        surr.surrogates(spiketrain, n_surrogates=n_surr, method=surr_method,
+                        dt=dither)
+
+    def test_joint_isi_spikes_at_border(self):
+        surr_method = 'joint_isi_dithering'
+        n_surr = 30
+        dither = 15 * pq.ms
+        spiketrain = neo.SpikeTrain(
+            [4.,   28.,   45.,  51.,   83.,   87.,   96., 111., 126.,  131.,
+             138.,  150.,
+             209.,  232.,  253.,  275.,  279.,  303.,  320.,  371.,  396.,
+             401.,  429.,  447.,
+             479.,  511.,  535.,  549.,  581.,  585.,  605.,  607.,  626.,
+             630.,  644.,  714.,
+             832.,  835.,  853.,  858.,  878.,  905.,  909.,  932.,  950.,
+             961.,  999.,  1000.],
+            t_start=0.*pq.ms, t_stop=1000.*pq.ms, units=pq.ms)
+        surr.surrogates(
+            spiketrain, n_surrogates=n_surr, method=surr_method, dt=dither)
+
+    def test_bin_shuffling_output_format(self):
+
+        self.bin_size = 3*pq.ms
+        self.max_displacement = 10
+        spiketrain = neo.SpikeTrain([90, 93, 97, 100, 105,
+                                     150, 180, 350] * pq.ms, t_stop=.5 * pq.s)
+        binned_spiketrain = conv.BinnedSpikeTrain(spiketrain, self.bin_size)
+        n_surrogates = 2
+
+        for sliding in (True, False):
+            surrogate_trains = surr.bin_shuffling(
+                binned_spiketrain, max_displacement=self.max_displacement,
+                n_surrogates=n_surrogates, sliding=sliding)
+
+            self.assertIsInstance(surrogate_trains, list)
+            self.assertEqual(len(surrogate_trains), n_surrogates)
+
+            self.assertIsInstance(surrogate_trains[0], conv.BinnedSpikeTrain)
+            for surrogate_train in surrogate_trains:
+                self.assertEqual(surrogate_train.t_start,
+                                 binned_spiketrain.t_start)
+                self.assertEqual(surrogate_train.t_stop,
+                                 binned_spiketrain.t_stop)
+                self.assertEqual(surrogate_train.n_bins,
+                                 binned_spiketrain.n_bins)
+                self.assertEqual(surrogate_train.bin_size,
+                                 binned_spiketrain.bin_size)
+
+    def test_bin_shuffling_empty_train(self):
+
+        self.bin_size = 3 * pq.ms
+        self.max_displacement = 10
+        empty_spiketrain = neo.SpikeTrain([] * pq.ms, t_stop=500 * pq.ms)
+
+        binned_spiketrain = conv.BinnedSpikeTrain(empty_spiketrain,
+                                                  self.bin_size)
+        surrogate_train = surr.bin_shuffling(
+            binned_spiketrain, max_displacement=self.max_displacement,
+            n_surrogates=1)[0]
+        self.assertEqual(np.sum(surrogate_train.to_bool_array()), 0)
+
+    def test_trial_shuffling_output_format(self):
+        spiketrain = \
+            [neo.SpikeTrain([90, 93, 97, 100, 105, 150, 180, 190] * pq.ms,
+                            t_stop=.2 * pq.s),
+             neo.SpikeTrain([90, 93, 97, 100, 105, 150, 180, 190] * pq.ms,
+                            t_stop=.2 * pq.s)]
+        # trial_length = 200 * pq.ms
+        # trial_separation = 50 * pq.ms
+        n_surrogates = 2
+        dither = 10 * pq.ms
+        surrogate_trains = surr.trial_shifting(
+            spiketrain, dither=dither, n_surrogates=n_surrogates)
+
+        self.assertIsInstance(surrogate_trains, list)
+        self.assertEqual(len(surrogate_trains), n_surrogates)
+
+        self.assertIsInstance(surrogate_trains[0], list)
+        self.assertIsInstance(surrogate_trains[0][0], neo.SpikeTrain)
+        for surrogate_train in surrogate_trains[0]:
+            self.assertEqual(surrogate_train.units, spiketrain[0].units)
+            self.assertEqual(surrogate_train.t_start, spiketrain[0].t_start)
+            self.assertEqual(surrogate_train.t_stop, spiketrain[0].t_stop)
+            self.assertEqual(len(surrogate_train), len(spiketrain[0]))
+            assert_array_less(0., np.diff(surrogate_train))  # check ordering
+
+    def test_trial_shuffling_empty_train(self):
+
+        empty_spiketrain = [neo.SpikeTrain([] * pq.ms, t_stop=500 * pq.ms),
+                            neo.SpikeTrain([] * pq.ms, t_stop=500 * pq.ms)]
+
+        dither = 10 * pq.ms
+        surrogate_train = surr.trial_shifting(
+            empty_spiketrain, dither=dither, n_surrogates=1)[0]
+
+        self.assertEqual(len(surrogate_train), 2)
+        self.assertEqual(len(surrogate_train[0]), 0)
+
+    def test_trial_shuffling_output_format_concatenated(self):
+        spiketrain = neo.SpikeTrain([90, 93, 97, 100, 105,
+                                     150, 180, 350] * pq.ms, t_stop=.5 * pq.s)
+        trial_length = 200 * pq.ms
+        trial_separation = 50 * pq.ms
+        n_surrogates = 2
+        dither = 10 * pq.ms
+        surrogate_trains = surr._trial_shifting_of_concatenated_spiketrain(
+            spiketrain, dither=dither, n_surrogates=n_surrogates,
+            trial_length=trial_length, trial_separation=trial_separation)
+
+        self.assertIsInstance(surrogate_trains, list)
+        self.assertEqual(len(surrogate_trains), n_surrogates)
+
+        self.assertIsInstance(surrogate_trains[0], neo.SpikeTrain)
+        for surrogate_train in surrogate_trains:
+            self.assertEqual(surrogate_train.units, spiketrain.units)
+            self.assertEqual(surrogate_train.t_start, spiketrain.t_start)
+            self.assertEqual(surrogate_train.t_stop, spiketrain.t_stop)
+            self.assertEqual(len(surrogate_train), len(spiketrain))
+            assert_array_less(0., np.diff(surrogate_train))  # check ordering
+
+    def test_trial_shuffling_empty_train_concatenated(self):
+
+        empty_spiketrain = neo.SpikeTrain([] * pq.ms, t_stop=500 * pq.ms)
+        trial_length = 200 * pq.ms
+        trial_separation = 50 * pq.ms
+
+        dither = 10 * pq.ms
+        surrogate_train = surr._trial_shifting_of_concatenated_spiketrain(
+            empty_spiketrain, dither=dither, n_surrogates=1,
+            trial_length=trial_length, trial_separation=trial_separation)[0]
+        self.assertEqual(len(surrogate_train), 0)
+
 
 def suite():
     suite = unittest.makeSuite(SurrogatesTestCase, 'test')
     return suite
 
 
 if __name__ == "__main__":
```

### Comparing `elephant-0.8.0/elephant/test/test_sta.py` & `elephant-0.9.0/elephant/test/test_sta.py`

 * *Files identical despite different names*

### Comparing `elephant-0.8.0/elephant/test/test_statistics.py` & `elephant-0.9.0/elephant/test/test_statistics.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,29 +3,32 @@
 Unit tests for the statistics module.
 
 :copyright: Copyright 2014-2016 by the Elephant team, see `doc/authors.rst`.
 :license: Modified BSD, see LICENSE.txt for details.
 """
 from __future__ import division
 
+import itertools
 import math
 import sys
 import unittest
 
 import neo
 import numpy as np
 import quantities as pq
 import scipy.integrate as spint
-from numpy.testing.utils import assert_array_almost_equal, assert_array_equal
+from numpy.testing import assert_array_almost_equal, assert_array_equal, \
+    assert_array_less
 
 import elephant.kernels as kernels
 from elephant import statistics
 from elephant.spike_train_generation import homogeneous_poisson_process
 
-python_version_major = sys.version_info.major
+if sys.version_info.major == 2:
+    import unittest2 as unittest
 
 
 class isi_TestCase(unittest.TestCase):
     def setUp(self):
         self.test_array_2d = np.array([[0.3, 0.56, 0.87, 1.23],
                                        [0.02, 0.71, 1.82, 8.46],
                                        [0.03, 0.14, 0.15, 0.92]])
@@ -76,14 +79,20 @@
     def test_isi_with_plain_array_2d_1(self):
         st = self.test_array_2d
         target = self.targ_array_2d_1
         res = statistics.isi(st, axis=1)
         assert not isinstance(res, pq.Quantity)
         assert_array_almost_equal(res, target, decimal=9)
 
+    def test_unsorted_array(self):
+        np.random.seed(0)
+        array = np.random.rand(100)
+        with self.assertWarns(UserWarning):
+            isi = statistics.isi(array)
+
 
 class isi_cv_TestCase(unittest.TestCase):
     def setUp(self):
         self.test_array_regular = np.arange(1, 6)
 
     def test_cv_isi_regular_spiketrain_is_zero(self):
         st = neo.SpikeTrain(self.test_array_regular, units='ms', t_stop=10.0)
@@ -330,14 +339,25 @@
         self.assertEqual(statistics.fanofactor(self.test_list),
                          np.var(self.sp_counts) / np.mean(self.sp_counts))
 
     def test_fanofactor_list_same(self):
         lst = [self.test_list[0]] * 3
         self.assertEqual(statistics.fanofactor(lst), 0.0)
 
+    def test_fanofactor_different_durations(self):
+        st1 = neo.SpikeTrain([1, 2, 3] * pq.s, t_stop=4 * pq.s)
+        st2 = neo.SpikeTrain([1, 2, 3] * pq.s, t_stop=4.5 * pq.s)
+        self.assertWarns(UserWarning, statistics.fanofactor, (st1, st2))
+
+    def test_fanofactor_wrong_type(self):
+        # warn_tolerance is not a quantity
+        st1 = neo.SpikeTrain([1, 2, 3] * pq.s, t_stop=4 * pq.s)
+        self.assertRaises(TypeError, statistics.fanofactor, [st1],
+                          warn_tolerance=1e-4)
+
 
 class LVTestCase(unittest.TestCase):
     def setUp(self):
         self.test_seq = [1, 28, 4, 47, 5, 16, 2, 5, 21, 12,
                          4, 12, 59, 2, 4, 18, 33, 25, 2, 34,
                          4, 1, 1, 14, 8, 1, 10, 1, 8, 20,
                          5, 1, 6, 5, 12, 2, 8, 8, 2, 8,
@@ -364,25 +384,74 @@
 
     def test_lv_raise_error(self):
         seq = self.test_seq
         self.assertRaises(ValueError, statistics.lv, [])
         self.assertRaises(ValueError, statistics.lv, 1)
         self.assertRaises(ValueError, statistics.lv, np.array([seq, seq]))
 
-    @unittest.skipUnless(python_version_major == 3, "assertWarns requires 3.2")
     def test_2short_spike_train(self):
         seq = [1]
         with self.assertWarns(UserWarning):
             """
             Catches UserWarning: Input size is too small. Please provide
             an input with more than 1 entry.
             """
             self.assertTrue(math.isnan(statistics.lv(seq, with_nan=True)))
 
 
+class LVRTestCase(unittest.TestCase):
+    def setUp(self):
+        self.test_seq = [1, 28, 4, 47, 5, 16, 2, 5, 21, 12,
+                         4, 12, 59, 2, 4, 18, 33, 25, 2, 34,
+                         4, 1, 1, 14, 8, 1, 10, 1, 8, 20,
+                         5, 1, 6, 5, 12, 2, 8, 8, 2, 8,
+                         2, 10, 2, 1, 1, 2, 15, 3, 20, 6,
+                         11, 6, 18, 2, 5, 17, 4, 3, 13, 6,
+                         1, 18, 1, 16, 12, 2, 52, 2, 5, 7,
+                         6, 25, 6, 5, 3, 15, 4, 3, 16, 3,
+                         6, 5, 24, 21, 3, 3, 4, 8, 4, 11,
+                         5, 7, 5, 6, 8, 11, 33, 10, 7, 4]
+
+        self.target = 2.1845363464753134
+
+    def test_lvr_with_quantities(self):
+        seq = pq.Quantity(self.test_seq, units='ms')
+        assert_array_almost_equal(statistics.lvr(seq), self.target, decimal=9)
+
+    def test_lvr_with_plain_array(self):
+        seq = np.array(self.test_seq)
+        assert_array_almost_equal(statistics.lvr(seq), self.target, decimal=9)
+
+    def test_lvr_with_list(self):
+        seq = self.test_seq
+        assert_array_almost_equal(statistics.lvr(seq), self.target, decimal=9)
+
+    def test_lvr_raise_error(self):
+        seq = self.test_seq
+        self.assertRaises(ValueError, statistics.lvr, [])
+        self.assertRaises(ValueError, statistics.lvr, 1)
+        self.assertRaises(ValueError, statistics.lvr, np.array([seq, seq]))
+        self.assertRaises(ValueError, statistics.lvr, seq, -1 * pq.ms)
+
+    def test_lvr_refractoriness_kwarg(self):
+        seq = np.array(self.test_seq)
+        with self.assertWarns(UserWarning):
+            assert_array_almost_equal(statistics.lvr(seq, R=5),
+                                      self.target, decimal=9)
+
+    def test_2short_spike_train(self):
+        seq = [1]
+        with self.assertWarns(UserWarning):
+            """
+            Catches UserWarning: Input size is too small. Please provide
+            an input with more than 1 entry.
+            """
+            self.assertTrue(math.isnan(statistics.lvr(seq, with_nan=True)))
+
+
 class CV2TestCase(unittest.TestCase):
     def setUp(self):
         self.test_seq = [1, 28, 4, 47, 5, 16, 2, 5, 21, 12,
                          4, 12, 59, 2, 4, 18, 33, 25, 2, 34,
                          4, 1, 1, 14, 8, 1, 10, 1, 8, 20,
                          5, 1, 6, 5, 12, 2, 8, 8, 2, 8,
                          2, 10, 2, 1, 1, 2, 15, 3, 20, 6,
@@ -409,15 +478,15 @@
     def test_cv2_raise_error(self):
         seq = self.test_seq
         self.assertRaises(ValueError, statistics.cv2, [])
         self.assertRaises(ValueError, statistics.cv2, 1)
         self.assertRaises(ValueError, statistics.cv2, np.array([seq, seq]))
 
 
-class RateEstimationTestCase(unittest.TestCase):
+class InstantaneousRateTest(unittest.TestCase):
 
     def setUp(self):
         # create a poisson spike train:
         self.st_tr = (0, 20.0)  # seconds
         self.st_dur = self.st_tr[1] - self.st_tr[0]  # seconds
         self.st_margin = 5.0  # seconds
         self.st_rate = 10.0  # Hertz
@@ -434,15 +503,14 @@
         self.spike_train = neo.SpikeTrain(spike_train * pq.s,
                                           t_start=self.st_tr[0] * pq.s,
                                           t_stop=self.st_tr[1] * pq.s)
 
         # generation of a multiply used specific kernel
         self.kernel = kernels.TriangularKernel(sigma=0.03 * pq.s)
 
-    @unittest.skipUnless(python_version_major == 3, "assertWarns requires 3.2")
     def test_instantaneous_rate_and_warnings(self):
         st = self.spike_train
         sampling_period = 0.01 * pq.s
         with self.assertWarns(UserWarning):
             # Catches warning: The width of the kernel was adjusted to a
             # minimally allowed width.
             inst_rate = statistics.instantaneous_rate(
@@ -453,50 +521,55 @@
         self.assertEqual(inst_rate.simplified.units, pq.Hz)
         self.assertEqual(inst_rate.t_stop.simplified, st.t_stop.simplified)
         self.assertEqual(inst_rate.t_start.simplified, st.t_start.simplified)
 
     def test_error_instantaneous_rate(self):
         self.assertRaises(
             TypeError, statistics.instantaneous_rate,
-            spiketrain=[1, 2, 3] * pq.s,
+            spiketrains=[1, 2, 3] * pq.s,
             sampling_period=0.01 * pq.ms, kernel=self.kernel)
         self.assertRaises(
-            TypeError, statistics.instantaneous_rate, spiketrain=[1, 2, 3],
+            TypeError, statistics.instantaneous_rate, spiketrains=[1, 2, 3],
             sampling_period=0.01 * pq.ms, kernel=self.kernel)
         st = self.spike_train
         self.assertRaises(
-            TypeError, statistics.instantaneous_rate, spiketrain=st,
+            TypeError, statistics.instantaneous_rate, spiketrains=st,
             sampling_period=0.01, kernel=self.kernel)
         self.assertRaises(
-            ValueError, statistics.instantaneous_rate, spiketrain=st,
+            ValueError, statistics.instantaneous_rate, spiketrains=st,
             sampling_period=-0.01 * pq.ms, kernel=self.kernel)
         self.assertRaises(
-            TypeError, statistics.instantaneous_rate, spiketrain=st,
+            TypeError, statistics.instantaneous_rate, spiketrains=st,
             sampling_period=0.01 * pq.ms, kernel='NONE')
         self.assertRaises(TypeError, statistics.instantaneous_rate,
                           self.spike_train,
                           sampling_period=0.01 * pq.s, kernel='wrong_string',
                           t_start=self.st_tr[0] * pq.s,
                           t_stop=self.st_tr[1] * pq.s,
                           trim=False)
         self.assertRaises(
-            TypeError, statistics.instantaneous_rate, spiketrain=st,
+            TypeError, statistics.instantaneous_rate, spiketrains=st,
             sampling_period=0.01 * pq.ms, kernel=self.kernel,
             cutoff=20 * pq.ms)
         self.assertRaises(
-            TypeError, statistics.instantaneous_rate, spiketrain=st,
+            TypeError, statistics.instantaneous_rate, spiketrains=st,
             sampling_period=0.01 * pq.ms, kernel=self.kernel, t_start=2)
         self.assertRaises(
-            TypeError, statistics.instantaneous_rate, spiketrain=st,
+            TypeError, statistics.instantaneous_rate, spiketrains=st,
             sampling_period=0.01 * pq.ms, kernel=self.kernel,
             t_stop=20 * pq.mV)
         self.assertRaises(
-            TypeError, statistics.instantaneous_rate, spiketrain=st,
+            TypeError, statistics.instantaneous_rate, spiketrains=st,
             sampling_period=0.01 * pq.ms, kernel=self.kernel, trim=1)
 
+        # cannot estimate a kernel for a list of spiketrains
+        self.assertRaises(ValueError, statistics.instantaneous_rate,
+                          spiketrains=[st, st], sampling_period=10 * pq.ms,
+                          kernel='auto')
+
     def test_rate_estimation_consistency(self):
         """
         Test, whether the integral of the rate estimation curve is (almost)
         equal to the number of spikes of the spike train.
         """
         kernel_types = tuple(
             kern_cls for kern_cls in kernels.__dict__.values()
@@ -545,24 +618,47 @@
     def test_regression_288(self):
         np.random.seed(9)
         sampling_period = 200 * pq.ms
         spiketrain = homogeneous_poisson_process(10 * pq.Hz,
                                                  t_start=0 * pq.s,
                                                  t_stop=10 * pq.s)
         kernel = kernels.AlphaKernel(sigma=5 * pq.ms, invert=True)
+        # check that instantaneous_rate "works" for kernels with small sigma
+        # without triggering an incomprehensible error
         rate = statistics.instantaneous_rate(spiketrain,
                                              sampling_period=sampling_period,
                                              kernel=kernel)
         self.assertEqual(
             len(rate), (spiketrain.t_stop / sampling_period).simplified.item())
 
-        # 3 Hz is not a target - it's meant to test the non-negativity of the
-        # result rate; ideally, for smaller sampling rates, the integral
-        # should match the num. of spikes in the spiketrain
-        self.assertGreater(rate.mean(), 3 * pq.Hz)
+    def test_small_kernel_sigma(self):
+        # Test that the instantaneous rate is overestimated when
+        # kernel.sigma << sampling_period and center_kernel is True.
+        # The setup is set to match the issue 288.
+        np.random.seed(9)
+        sampling_period = 200 * pq.ms
+        sigma = 5 * pq.ms
+        rate_expected = 10 * pq.Hz
+        spiketrain = homogeneous_poisson_process(rate_expected,
+                                                 t_start=0 * pq.s,
+                                                 t_stop=10 * pq.s)
+        kernel_types = tuple(
+            kern_cls for kern_cls in kernels.__dict__.values()
+            if isinstance(kern_cls, type) and
+            issubclass(kern_cls, kernels.Kernel) and
+            kern_cls is not kernels.Kernel and
+            kern_cls is not kernels.SymmetricKernel)
+        for kern_cls, invert in itertools.product(kernel_types, (False, True)):
+            kernel = kern_cls(sigma=sigma, invert=invert)
+            with self.subTest(kernel=kernel):
+                rate = statistics.instantaneous_rate(
+                    spiketrain,
+                    sampling_period=sampling_period,
+                    kernel=kernel, center_kernel=True)
+                self.assertGreater(rate.mean(), rate_expected)
 
     def test_spikes_on_edges(self):
         # this test demonstrates that the trimming (convolve valid mode)
         # removes the edge spikes, underestimating the true firing rate and
         # thus is not able to reconstruct the number of spikes in a
         # spiketrain (see test_rate_estimation_consistency)
         cutoff = 5
@@ -632,19 +728,19 @@
         st_rate_2 = statistics.instantaneous_rate(spike_train2,
                                                   sampling_period=0.01 * pq.s,
                                                   kernel=self.kernel)
         combined_rate = statistics.instantaneous_rate(
             [self.spike_train, spike_train2],
             sampling_period=0.01 * pq.s,
             kernel=self.kernel)
-        summed_rate = st_rate_1 + st_rate_2  # equivalent for identical kernels
+        rate_concat = np.c_[st_rate_1, st_rate_2]
         # 'time_vector.dtype' in instantaneous_rate() is changed from float64
         # to float32 which results in 3e-6 abs difference
         assert_array_almost_equal(combined_rate.magnitude,
-                                  summed_rate.magnitude, decimal=5)
+                                  rate_concat.magnitude, decimal=5)
 
     # Regression test for #144
     def test_instantaneous_rate_regression_144(self):
         # The following spike train contains spikes that are so close to each
         # other, that the optimal kernel cannot be detected. Therefore, the
         # function should react with a ValueError.
         st = neo.SpikeTrain([2.12, 2.13, 2.15] * pq.s, t_stop=10 * pq.s)
@@ -676,14 +772,82 @@
         # factor 2.7 connects half width of Gaussian distribution with
         #            99% probability mass with its standard deviation.
         result_automatic = statistics.instantaneous_rate(
             spiketrain, 10 * pq.ms, kernel='auto')
 
         assert_array_almost_equal(result_target, result_automatic)
 
+    def test_instantaneous_rate_grows_with_sampling_period(self):
+        np.random.seed(0)
+        rate_expected = 10 * pq.Hz
+        spiketrain = homogeneous_poisson_process(rate=rate_expected,
+                                                 t_stop=10 * pq.s)
+        kernel = kernels.GaussianKernel(sigma=100 * pq.ms)
+        rates_mean = []
+        for sampling_period in np.linspace(1, 1000, num=10) * pq.ms:
+            with self.subTest(sampling_period=sampling_period):
+                rate = statistics.instantaneous_rate(
+                    spiketrain,
+                    sampling_period=sampling_period,
+                    kernel=kernel)
+                rates_mean.append(rate.mean())
+        # rate means are greater or equal the expected rate
+        assert_array_less(rate_expected, rates_mean)
+        # check sorted
+        self.assertTrue(np.all(rates_mean[:-1] < rates_mean[1:]))
+
+    # Regression test for #360
+    def test_centered_at_origin(self):
+        # Skip RectangularKernel because it doesn't have a strong peak.
+        kernel_types = tuple(
+            kern_cls for kern_cls in kernels.__dict__.values()
+            if isinstance(kern_cls, type) and
+            issubclass(kern_cls, kernels.SymmetricKernel) and
+            kern_cls not in (kernels.SymmetricKernel,
+                             kernels.RectangularKernel))
+        kernels_symmetric = [kern_cls(sigma=50 * pq.ms, invert=False)
+                             for kern_cls in kernel_types]
+
+        # first part: a symmetric spiketrain with a symmetric kernel
+        spiketrain = neo.SpikeTrain(np.array([-0.0001, 0, 0.0001]) * pq.s,
+                                    t_start=-1,
+                                    t_stop=1)
+        for kernel in kernels_symmetric:
+            rate = statistics.instantaneous_rate(spiketrain,
+                                                 sampling_period=20 * pq.ms,
+                                                 kernel=kernel)
+            # the peak time must be centered at origin
+            self.assertEqual(rate.times[np.argmax(rate)], 0)
+
+        # second part: a single spike at t=0
+        periods = [2 ** c for c in range(-3, 6)]
+        for period in periods:
+            with self.subTest(period=period):
+                spiketrain = neo.SpikeTrain(np.array([0]) * pq.s,
+                                            t_start=-period * 10 * pq.ms,
+                                            t_stop=period * 10 * pq.ms)
+                for kernel in kernels_symmetric:
+                    rate = statistics.instantaneous_rate(
+                        spiketrain,
+                        sampling_period=period * pq.ms,
+                        kernel=kernel)
+                    self.assertEqual(rate.times[np.argmax(rate)], 0)
+
+    def test_annotations(self):
+        spiketrain = neo.SpikeTrain([1, 2], t_stop=2 * pq.s, units=pq.s)
+        kernel = kernels.AlphaKernel(sigma=100 * pq.ms)
+        rate = statistics.instantaneous_rate(spiketrain,
+                                             sampling_period=10 * pq.ms,
+                                             kernel=kernel)
+        kernel_annotation = dict(type=type(kernel).__name__,
+                                 sigma=str(kernel.sigma),
+                                 invert=kernel.invert)
+        self.assertIn('kernel', rate.annotations)
+        self.assertEqual(rate.annotations['kernel'], kernel_annotation)
+
 
 class TimeHistogramTestCase(unittest.TestCase):
     def setUp(self):
         self.spiketrain_a = neo.SpikeTrain(
             [0.5, 0.7, 1.2, 3.1, 4.3, 5.5, 6.7] * pq.s, t_stop=10.0 * pq.s)
         self.spiketrain_b = neo.SpikeTrain(
             [0.1, 0.7, 1.2, 2.2, 4.3, 5.5, 8.0] * pq.s, t_stop=10.0 * pq.s)
@@ -741,14 +905,25 @@
                            targ.reshape(targ.size, 1) * 1 / pq.s)
 
         # Normalization unspecified, raises error
         self.assertRaises(ValueError, statistics.time_histogram,
                           self.spiketrains,
                           bin_size=pq.s, output=' ')
 
+    def test_annotations(self):
+        np.random.seed(1)
+        spiketrains = [homogeneous_poisson_process(
+            rate=10 * pq.Hz, t_stop=10 * pq.s) for _ in range(10)]
+        for output in ("counts", "mean", "rate"):
+            histogram = statistics.time_histogram(spiketrains,
+                                                  bin_size=3 * pq.ms,
+                                                  output=output)
+            self.assertIn('normalization', histogram.annotations)
+            self.assertEqual(histogram.annotations['normalization'], output)
+
 
 class ComplexityPdfTestCase(unittest.TestCase):
     def setUp(self):
         self.spiketrain_a = neo.SpikeTrain(
             [0.5, 0.7, 1.2, 2.3, 4.3, 5.5, 6.7] * pq.s, t_stop=10.0 * pq.s)
         self.spiketrain_b = neo.SpikeTrain(
             [0.5, 0.7, 1.2, 2.3, 4.3, 5.5, 8.0] * pq.s, t_stop=10.0 * pq.s)
```

### Comparing `elephant-0.8.0/elephant/test/test_unitary_event_analysis.py` & `elephant-0.9.0/elephant/test/test_unitary_event_analysis.py`

 * *Files identical despite different names*

### Comparing `elephant-0.8.0/elephant/test/test_waveform_features.py` & `elephant-0.9.0/elephant/test/test_waveform_features.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 """
 
 from __future__ import division
 
 import sys
 import unittest
 
-import neo
 import numpy as np
 import quantities as pq
+from numpy.testing import assert_array_almost_equal
 
 from elephant import waveform_features
 
 python_version_major = sys.version_info.major
 
 
 class WaveformWidthTestCase(unittest.TestCase):
@@ -60,41 +60,37 @@
                               waveform, cutoff=cutoff)
         for cutoff in np.linspace(0., 1., num=size, endpoint=False):
             width = waveform_features.waveform_width(waveform, cutoff=cutoff)
             self.assertEqual(width, size - 1)
 
 
 class WaveformSignalToNoiseRatioTestCase(unittest.TestCase):
-    def setUp(self):
-        self.spiketrain_without_waveforms = neo.SpikeTrain(
-            [0.5, 0.7, 1.2, 2.3, 4.3, 5.5, 6.7] * pq.s, t_stop=10.0 * pq.s)
-        self.spiketrain_with_zero_waveforms = neo.SpikeTrain(
-            [0.5, 0.7, 1.2, 2.3, 4.3, 5.5, 6.7] * pq.s, t_stop=10.0 * pq.s)
-        self.spiketrain_with_zero_waveforms.waveforms = \
-            np.zeros((10, 1, 10)) * pq.uV
-
-        self.spiketrain_with_waveforms = neo.SpikeTrain(
-            [0.5, 6.7] * pq.s, t_stop=10.0 * pq.s)
-        self.spiketrain_with_waveforms.waveforms = \
-            np.arange(20).reshape((2, 1, 10)) * pq.uV
-
-    def test_without_wavefroms(self):
-        self.assertRaises(ValueError, waveform_features.waveform_snr,
-                          self.spiketrain_without_waveforms)
-
     @unittest.skipUnless(python_version_major == 3, "assertWarns requires 3.2")
-    def test_with_zero_waveforms(self):
-        with self.assertWarns(UserWarning):
-            # expect np.nan result when spiketrain noise is zero.
-            result = waveform_features.waveform_snr(
-                self.spiketrain_with_zero_waveforms)
-        self.assertTrue(np.isnan(result))
-
-    def test_with_waveforms(self):
-        target_value = 0.9
-        result = waveform_features.waveform_snr(
-            self.spiketrain_with_waveforms)
-        self.assertEqual(result, target_value)
+    def test_zero_waveforms(self):
+        zero_waveforms = [np.zeros((5, 10)),
+                          np.zeros((5, 1, 10)),
+                          np.zeros((5, 3, 10))]
+        for zero_wf in zero_waveforms:
+            with self.assertWarns(UserWarning):
+                # expect np.nan result when waveform noise is zero.
+                result = waveform_features.waveform_snr(zero_wf)
+            self.assertTrue(np.all(np.isnan(result)))
+
+    def test_waveforms_arange_single_spiketrain(self):
+        target_snr = 0.9
+        waveforms = np.arange(20).reshape((2, 1, 10))
+        snr_float = waveform_features.waveform_snr(waveforms)
+        self.assertIsInstance(snr_float, float)
+        self.assertEqual(snr_float, target_snr)
+        self.assertEqual(waveform_features.waveform_snr(np.squeeze(waveforms)),
+                         target_snr)
+
+    def test_waveforms_arange_multiple_spiketrains(self):
+        target_snr = [0.3, 0.3, 0.3]
+        waveforms = np.arange(60).reshape((2, 3, 10))
+        snr_arr = waveform_features.waveform_snr(waveforms)
+        self.assertIsInstance(snr_arr, np.ndarray)
+        assert_array_almost_equal(snr_arr, target_snr)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `elephant-0.8.0/elephant/unitary_event_analysis.py` & `elephant-0.9.0/elephant/unitary_event_analysis.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,14 +60,26 @@
 import numpy as np
 import quantities as pq
 import scipy
 
 import elephant.conversion as conv
 from elephant.utils import is_binary
 
+__all__ = [
+    "hash_from_pattern",
+    "inverse_hash_from_pattern",
+    "n_emp_mat",
+    "n_emp_mat_sum_trial",
+    "n_exp_mat",
+    "n_exp_mat_sum_trial",
+    "gen_pval_anal",
+    "jointJ",
+    "jointJ_window_analysis"
+]
+
 
 def hash_from_pattern(m, base=2):
     """
     Calculate for a spike pattern or a matrix of spike patterns
     (provide each pattern as a column) composed of N neurons a
     unique number.
 
@@ -608,15 +620,18 @@
     --------
     >>> p_val = np.array([0.31271072,  0.01175031])
     >>> jointJ(p_val)
     array([0.3419968 ,  1.92481736])
 
     """
     p_arr = np.asarray(p_val)
-    Js = np.log10(1 - p_arr) - np.log10(p_arr)
+    with np.errstate(divide='ignore'):
+        # Ignore 'Division by zero' warning which happens when p_arr is 1.0 or
+        # 0.0 (no spikes).
+        Js = np.log10(1 - p_arr) - np.log10(p_arr)
     return Js
 
 
 def _rate_mat_avg_trial(mat):
     """
     Calculates the average firing rate of each neurons across trials.
     """
```

### Comparing `elephant-0.8.0/elephant/waveform_features.py` & `elephant-0.9.0/elephant/waveform_features.py`

 * *Files 23% similar despite different names*

```diff
@@ -6,29 +6,36 @@
 :license: Modified BSD, see LICENSE.txt for details.
 """
 
 from __future__ import division, print_function, unicode_literals
 
 import warnings
 
+import neo
 import numpy as np
 
+__all__ = [
+    "waveform_width",
+    "waveform_snr"
+]
+
 
 def waveform_width(waveform, cutoff=0.75):
     """
     Calculate the width (trough-to-peak TTP) of a waveform.
 
     Searches for an index of a minimum within first `cutoff` of the waveform
     vector, next for a maximum after the identified minimum, and returns the
     difference between them.
 
     Parameters
     ----------
-    waveform : np.ndarray or list or pq.Quantity
-        Time course of a single waveform
+    waveform : array-like
+        Time course of a single waveform. Accepts a list, a numpy array or a
+        quantity.
     cutoff : float, optional
         Defines the normalized range `[0, cutoff]` of the input sequence for
         computing the minimum. Must be in `[0, 1)` range.
         Default: 0.75.
 
     Returns
     -------
@@ -56,62 +63,68 @@
     idx_min = np.argmin(waveform[:min_border])
     idx_max = np.argmax(waveform[idx_min:]) + idx_min
     width = idx_max - idx_min
 
     return width
 
 
-def waveform_snr(spiketrain):
+def waveform_snr(waveforms):
     """
-    Return the signal-to-noise ratio of the waveforms of a SpikeTrain.
+    Return the signal-to-noise ratio of the waveforms of one or more
+    spike trains.
 
     Signal-to-noise ratio is defined as the difference in mean peak-to-trough
     voltage divided by twice the mean SD. The mean SD is computed by
     measuring the SD of the spike waveform over all acquired spikes
     at each of the sample time points of the waveform and then averaging [1]_.
 
     Parameters
     ----------
-    spiketrain : neo.SpikeTrain
-        The spike times with attached waveforms.
+    waveforms : array-like
+        A list or a quantity or a numpy array of waveforms of shape
+        ``(n_waveforms, time)`` in case of a single spike train or
+        ``(n_waveforms, n_spiketrains, time)`` in case of one or more spike
+        trains.
 
     Returns
     -------
-    snr : float
-        signal-to-noise ratio according to [1]_
-
-    Raises
-    ------
-    ValueError
-        If `spiketrain` has no attached waveforms.
+    snr : float or np.ndarray
+        Signal-to-noise ratio according to [1]_. If the input `waveforms`
+        shape is ``(n_waveforms, time)`` or ``(n_waveforms, 1, time)``, a
+        single float is returned. Otherwise, if the shape is
+        ``(n_waveforms, n_spiketrains, time)``, a numpy array of length
+        ``n_spiketrains`` is returned.
+
+    Notes
+    -----
+    The waveforms of a `neo.SpikeTrain` can be extracted as
+    `spiketrain.waveforms`, if it's loaded from a file, in which case you need
+    to set ``load_waveforms=True`` in ``neo.read_block()``.
 
     References
     ----------
-
     .. [1] Hatsopoulos, N. G., Xu, Q. & Amit, Y.
            Encoding of Movement Fragments in the Motor Cortex.
            J. Neurosci. 27, 5105–5114 (2007).
 
     """
-    # check whether spiketrain contains waveforms
-    if spiketrain.waveforms is None:
-        raise ValueError('There are no waveforms attached to this \
-                         neo.Spiketrain. Did you forget to set \
-                         load_waveforms=True in neoIO.read_block()?')
-
+    if isinstance(waveforms, neo.SpikeTrain):
+        warnings.warn("spiketrain input is deprecated; "
+                      "pass 'spiketrain.waveforms' directly.")
+        waveforms = waveforms.waveforms
+    # asarray removes quantities, if present
+    waveforms = np.squeeze(np.asarray(waveforms))
     # average over all waveforms for each bin
-    mean_waveform = np.mean(spiketrain.waveforms.magnitude, axis=0)[0]
-    # standard deviation over all waveforms for each bin
-    std_waveform = np.std(spiketrain.waveforms.magnitude, axis=0)[0]
-    mean_std = np.mean(std_waveform)
+    mean_waveform = waveforms.mean(axis=0)
+    # standard deviation over all waveforms over all bins
+    std_waveform = waveforms.std(axis=0).mean(axis=-1)
 
-    # signal
-    peak_to_trough_voltage = np.max(mean_waveform) - np.min(mean_waveform)
+    # peak to trough voltage signal
+    peak_range = mean_waveform.max(axis=-1) - mean_waveform.min(axis=-1)
     # noise
-    noise = 2 * mean_std
+    noise = 2 * std_waveform
+
+    snr = peak_range / noise
+    if np.isnan(snr).any():
+        warnings.warn('The waveforms noise was evaluated to 0. Returning NaN')
 
-    if noise == 0:
-        warnings.warn('The noise was evaluated to 0.')
-        snr = np.nan
-    else:
-        snr = peak_to_trough_voltage / noise
     return snr
```

### Comparing `elephant-0.8.0/elephant.egg-info/PKG-INFO` & `elephant-0.9.0/elephant.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,46 +1,62 @@
 Metadata-Version: 2.1
 Name: elephant
-Version: 0.8.0
+Version: 0.9.0
 Summary: Elephant is a package for analysis of electrophysiology data in Python
 Home-page: http://neuralensemble.org/elephant
 Author: Elephant authors and contributors
 Author-email: andrew.davison@unic.cnrs-gif.fr
 License: BSD
 Description: # Elephant - Electrophysiology Analysis Toolkit
         
-        ![](https://travis-ci.org/NeuralEnsemble/elephant.png?branch=master "Unit Test Status")
-        ![](https://coveralls.io/repos/NeuralEnsemble/elephant/badge.png "Unit Test Coverage")
-        ![](https://readthedocs.org/projects/elephant/badge/?version=latest "Documentation Status")
-        ![](https://img.shields.io/pypi/v/elephant)
-        ![](https://img.shields.io/pypi/dm/elephant)
+        [![Build Status](https://travis-ci.org/NeuralEnsemble/elephant.svg?branch=master)](https://travis-ci.org/NeuralEnsemble/elephant)
+        [![Coverage Status](https://coveralls.io/repos/github/NeuralEnsemble/elephant/badge.svg?branch=master)](https://coveralls.io/github/NeuralEnsemble/elephant?branch=master)
+        [![Documentation Status](https://readthedocs.org/projects/elephant/badge/?version=latest)](https://elephant.readthedocs.io/en/latest/?badge=latest)
+        [![![PyPi]](https://img.shields.io/pypi/v/elephant)](https://pypi.org/project/elephant/)
+        [![Statistics](https://img.shields.io/pypi/dm/elephant)](https://seladb.github.io/StarTrack-js/#/preload?r=neuralensemble,elephant)
         [![Gitter](https://badges.gitter.im/python-elephant/community.svg)](https://gitter.im/python-elephant/community?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge)
         
         *Elephant* package analyses all sorts of neurophysiological data:
         spike trains, LFP, analog signals. The input-output data format is either
         [Neo](https://github.com/NeuralEnsemble/python-neo), Quantity or Numpy array.
         
+        
         ### More Information
         
         * Documentation: https://elephant.readthedocs.io/en/latest/
         * Mailing list: https://groups.google.com/group/neuralensemble
         
         
+        #### Visualization of Elephant analysis objects
+        
+        Viziphant package (https://github.com/INM-6/viziphant) is developed by Elephant
+        team for plotting and visualization of the output of Elephant functions in a
+        few lines of code.
+        
+        
         #### License
          
         Modified BSD License, see [LICENSE.txt](LICENSE.txt) for details.
         
+        
         #### Copyright
         
         :copyright: 2014-2020 by the [Elephant team](doc/authors.rst).
         
+        
         #### Acknowledgments
         
         See [acknowledgments](doc/acknowledgments.rst).
         
+        
+        #### Citation
+        
+        See [citations](doc/citation.rst).
+        
+        
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 2
```

### Comparing `elephant-0.8.0/elephant.egg-info/SOURCES.txt` & `elephant-0.9.0/elephant.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,31 +1,36 @@
+CITATION.txt
 LICENSE.txt
 MANIFEST.in
 README.md
 setup.py
 doc/Makefile
 doc/acknowledgments.rst
 doc/authors.rst
+doc/citation.rst
 doc/conf.py
 doc/developers_guide.rst
 doc/documentation_guide.rst
 doc/get_in_touch.rst
 doc/index.rst
 doc/install.rst
 doc/maintainers_guide.rst
 doc/make.bat
 doc/modules.rst
 doc/release_notes.rst
 doc/style_guide.rst
 doc/tutorials.rst
+doc/_templates/autosummary/class.rst
 doc/bib/elephant.bib
 doc/images/elephant_favicon.ico
 doc/images/elephant_logo.png
 doc/images/elephant_logo_sidebar.png
+doc/reference/_spike_train_processing.rst
 doc/reference/asset.rst
+doc/reference/causality.rst
 doc/reference/cell_assembly_detection.rst
 doc/reference/change_point_detection.rst
 doc/reference/conversion.rst
 doc/reference/cubic.rst
 doc/reference/current_source_density.rst
 doc/reference/gpfa.rst
 doc/reference/kernels.rst
@@ -36,14 +41,15 @@
 doc/reference/signal_processing.rst
 doc/reference/spade.rst
 doc/reference/spectral.rst
 doc/reference/spike_train_correlation.rst
 doc/reference/spike_train_dissimilarity.rst
 doc/reference/spike_train_generation.rst
 doc/reference/spike_train_surrogates.rst
+doc/reference/spike_train_synchrony.rst
 doc/reference/sta.rst
 doc/reference/statistics.rst
 doc/reference/unitary_event_analysis.rst
 doc/reference/waveform_features.rst
 doc/reference/toctree/kernels/elephant.kernels.AlphaKernel.rst
 doc/reference/toctree/kernels/elephant.kernels.EpanechnikovLikeKernel.rst
 doc/reference/toctree/kernels/elephant.kernels.ExponentialKernel.rst
@@ -72,24 +78,27 @@
 elephant/signal_processing.py
 elephant/spade.py
 elephant/spectral.py
 elephant/spike_train_correlation.py
 elephant/spike_train_dissimilarity.py
 elephant/spike_train_generation.py
 elephant/spike_train_surrogates.py
+elephant/spike_train_synchrony.py
 elephant/sta.py
 elephant/statistics.py
 elephant/unitary_event_analysis.py
 elephant/utils.py
 elephant/waveform_features.py
 elephant.egg-info/PKG-INFO
 elephant.egg-info/SOURCES.txt
 elephant.egg-info/dependency_links.txt
 elephant.egg-info/requires.txt
 elephant.egg-info/top_level.txt
+elephant/causality/__init__.py
+elephant/causality/granger.py
 elephant/current_source_density_src/KCSD.py
 elephant/current_source_density_src/README.md
 elephant/current_source_density_src/__init__.py
 elephant/current_source_density_src/basis_functions.py
 elephant/current_source_density_src/icsd.py
 elephant/current_source_density_src/test_data.mat
 elephant/current_source_density_src/utility_functions.py
@@ -100,17 +109,19 @@
 elephant/parallel/__init__.py
 elephant/parallel/mpi.py
 elephant/parallel/parallel.py
 elephant/spade_src/LICENSE
 elephant/spade_src/__init__.py
 elephant/spade_src/fast_fca.py
 elephant/test/__init__.py
+elephant/test/download.py
 elephant/test/make_spike_extraction_test_data.py
 elephant/test/spike_extraction_test_data.txt
 elephant/test/test_asset.py
+elephant/test/test_causality.py
 elephant/test/test_cell_assembly_detection.py
 elephant/test/test_change_point_detection.py
 elephant/test/test_conversion.py
 elephant/test/test_csd.py
 elephant/test/test_cubic.py
 elephant/test/test_gpfa.py
 elephant/test/test_icsd.py
@@ -123,14 +134,15 @@
 elephant/test/test_signal_processing.py
 elephant/test/test_spade.py
 elephant/test/test_spectral.py
 elephant/test/test_spike_train_correlation.py
 elephant/test/test_spike_train_dissimilarity.py
 elephant/test/test_spike_train_generation.py
 elephant/test/test_spike_train_surrogates.py
+elephant/test/test_spike_train_synchrony.py
 elephant/test/test_sta.py
 elephant/test/test_statistics.py
 elephant/test/test_unitary_event_analysis.py
 elephant/test/test_waveform_features.py
 requirements/environment.yml
 requirements/requirements-docs.txt
 requirements/requirements-extras.txt
```

### Comparing `elephant-0.8.0/setup.py` & `elephant-0.9.0/setup.py`

 * *Files identical despite different names*

