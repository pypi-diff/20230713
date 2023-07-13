# Comparing `tmp/EModelRunner-1.1.8.tar.gz` & `tmp/EModelRunner-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/EModelRunner-1.1.8.tar", last modified: Mon Apr 17 14:11:36 2023, max compression
+gzip compressed data, was "dist/EModelRunner-1.1.9.tar", last modified: Thu Jun  1 13:41:17 2023, max compression
```

## Comparing `EModelRunner-1.1.8.tar` & `EModelRunner-1.1.9.tar`

### file list

```diff
@@ -1,287 +1,286 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:11:36.000000 EModelRunner-1.1.8/
--rwxr-xr-x   0 runner    (1001) docker     (123)      126 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/.compile_mod.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:11:36.000000 EModelRunner-1.1.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:11:36.000000 EModelRunner-1.1.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/.github/workflows/keep-alive.yml
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11360 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/COPYING
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:11:36.000000 EModelRunner-1.1.8/EModelRunner.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13332 2023-04-17 14:11:35.000000 EModelRunner-1.1.8/EModelRunner.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11087 2023-04-17 14:11:36.000000 EModelRunner-1.1.8/EModelRunner.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 14:11:35.000000 EModelRunner-1.1.8/EModelRunner.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-17 14:11:35.000000 EModelRunner-1.1.8/EModelRunner.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-17 14:11:35.000000 EModelRunner-1.1.8/EModelRunner.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)    13332 2023-04-17 14:11:36.000000 EModelRunner-1.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10156 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:11:36.000000 EModelRunner-1.1.8/doc/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/doc/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:11:36.000000 EModelRunner-1.1.8/doc/source/
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/doc/source/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/doc/source/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3263 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/doc/source/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:11:36.000000 EModelRunner-1.1.8/doc/source/images/
--rw-r--r--   0 runner    (1001) docker     (123)   207165 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/doc/source/images/GUI_screenshot.png
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/doc/source/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:11:36.000000 EModelRunner-1.1.8/doc/source/logo/
--rw-r--r--   0 runner    (1001) docker     (123)   303675 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/doc/source/logo/BBP-eModelRunner.jpg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:11:36.000000 EModelRunner-1.1.8/emodelrunner/
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/emodelrunner/GUI.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:11:36.000000 EModelRunner-1.1.8/emodelrunner/GUI_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/emodelrunner/GUI_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    42494 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/emodelrunner/GUI_utils/frames.py
--rw-r--r--   0 runner    (1001) docker     (123)     8725 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/emodelrunner/GUI_utils/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     7805 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/emodelrunner/GUI_utils/plotshape.py
--rw-r--r--   0 runner    (1001) docker     (123)    18792 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/emodelrunner/GUI_utils/simulator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3790 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/emodelrunner/GUI_utils/style.py
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/emodelrunner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9843 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/emodelrunner/cell.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:11:36.000000 EModelRunner-1.1.8/emodelrunner/configuration/
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/emodelrunner/configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4892 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/emodelrunner/configuration/configparser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/emodelrunner/configuration/subgroups.py
--rw-r--r--   0 runner    (1001) docker     (123)    18555 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/emodelrunner/configuration/validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6263 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/emodelrunner/create_cells.py
--rw-r--r--   0 runner    (1001) docker     (123)     7565 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/emodelrunner/create_hoc.py
--rw-r--r--   0 runner    (1001) docker     (123)    25018 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/emodelrunner/create_hoc_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/emodelrunner/create_recordings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/emodelrunner/create_stimuli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:11:36.000000 EModelRunner-1.1.8/emodelrunner/factsheets/
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/emodelrunner/factsheets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4374 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/emodelrunner/factsheets/experimental_features.py
--rw-r--r--   0 runner    (1001) docker     (123)    10833 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/emodelrunner/factsheets/ion_channel_mechanisms.py
--rw-r--r--   0 runner    (1001) docker     (123)    20087 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/emodelrunner/factsheets/morphology_features.py
--rw-r--r--   0 runner    (1001) docker     (123)     7633 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/emodelrunner/factsheets/output.py
--rw-r--r--   0 runner    (1001) docker     (123)     3856 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/emodelrunner/factsheets/physiology_features.py
--rw-r--r--   0 runner    (1001) docker     (123)     4155 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/emodelrunner/features.py
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/emodelrunner/json_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    13656 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/emodelrunner/load.py
--rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/emodelrunner/locations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:11:36.000000 EModelRunner-1.1.8/emodelrunner/morphology/
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/emodelrunner/morphology/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/emodelrunner/morphology/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     7315 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/emodelrunner/morphology/morphology.py
--rw-r--r--   0 runner    (1001) docker     (123)     4391 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/emodelrunner/output.py
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/emodelrunner/parsing_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:11:36.000000 EModelRunner-1.1.8/emodelrunner/protocols/
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/emodelrunner/protocols/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15690 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/emodelrunner/protocols/create_protocols.py
--rw-r--r--   0 runner    (1001) docker     (123)     5734 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/emodelrunner/protocols/protocols_func.py
--rw-r--r--   0 runner    (1001) docker     (123)    26089 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/emodelrunner/protocols/reader.py
--rw-r--r--   0 runner    (1001) docker     (123)    46821 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/emodelrunner/protocols/sscx_protocols.py
--rw-r--r--   0 runner    (1001) docker     (123)    16774 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/emodelrunner/protocols/synplas_protocols.py
--rw-r--r--   0 runner    (1001) docker     (123)    35315 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/emodelrunner/protocols/thalamus_protocols.py
--rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/emodelrunner/recordings.py
--rw-r--r--   0 runner    (1001) docker     (123)     3101 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/emodelrunner/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     4663 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/emodelrunner/run_pairsim.py
--rw-r--r--   0 runner    (1001) docker     (123)     4379 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/emodelrunner/run_synplas.py
--rw-r--r--   0 runner    (1001) docker     (123)     7750 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/emodelrunner/stimuli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:11:36.000000 EModelRunner-1.1.8/emodelrunner/synapses/
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/emodelrunner/synapses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/emodelrunner/synapses/create_locations.py
--rw-r--r--   0 runner    (1001) docker     (123)     7288 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/emodelrunner/synapses/glusynapse.py
--rw-r--r--   0 runner    (1001) docker     (123)     6968 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/emodelrunner/synapses/mechanism.py
--rw-r--r--   0 runner    (1001) docker     (123)     7608 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/emodelrunner/synapses/minis.py
--rw-r--r--   0 runner    (1001) docker     (123)     3486 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/emodelrunner/synapses/recordings.py
--rw-r--r--   0 runner    (1001) docker     (123)    10317 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/emodelrunner/synapses/stimuli.py
--rw-r--r--   0 runner    (1001) docker     (123)     6473 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/emodelrunner/synapses/synapse.py
--rw-r--r--   0 runner    (1001) docker     (123)     9719 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/emodelrunner/synplas_analysis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:11:36.000000 EModelRunner-1.1.8/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:11:36.000000 EModelRunner-1.1.8/examples/sscx_sample_dir/
--rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/sscx_sample_dir/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)    15070 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/sscx_sample_dir/LICENSE_CC-BY-CA-SA-4.0
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/sscx_sample_dir/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:11:36.000000 EModelRunner-1.1.8/examples/sscx_sample_dir/config/
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/sscx_sample_dir/config/config_allsteps.ini
--rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/sscx_sample_dir/config/config_factsheets.ini
--rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/sscx_sample_dir/config/config_multiprotocols.ini
--rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/sscx_sample_dir/config/config_recipe_protocols.ini
--rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/sscx_sample_dir/config/config_singlestep.ini
--rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/sscx_sample_dir/config/config_synapses.ini
--rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/sscx_sample_dir/config/config_synapses_short.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:11:36.000000 EModelRunner-1.1.8/examples/sscx_sample_dir/config/features/
--rw-r--r--   0 runner    (1001) docker     (123)    14709 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/sscx_sample_dir/config/features/cADpyr_L4PC.json
--rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/sscx_sample_dir/config/features/units.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:11:36.000000 EModelRunner-1.1.8/examples/sscx_sample_dir/config/params/
--rw-r--r--   0 runner    (1001) docker     (123)     6710 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/sscx_sample_dir/config/params/final.json
--rw-r--r--   0 runner    (1001) docker     (123)    10218 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/sscx_sample_dir/config/params/pyr.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:11:36.000000 EModelRunner-1.1.8/examples/sscx_sample_dir/config/protocols/
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/sscx_sample_dir/config/protocols/RmpRiTau.json
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/sscx_sample_dir/config/protocols/allsteps.json
--rw-r--r--   0 runner    (1001) docker     (123)     5372 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/sscx_sample_dir/config/protocols/cADpyr_L4PC.json
--rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/sscx_sample_dir/config/protocols/multiprotocols.json
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/sscx_sample_dir/config/protocols/singlestep.json
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/sscx_sample_dir/config/protocols/synapses.json
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/sscx_sample_dir/config/protocols/synapses_short.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:11:36.000000 EModelRunner-1.1.8/examples/sscx_sample_dir/hoc_recordings/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/sscx_sample_dir/hoc_recordings/.keep
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:11:36.000000 EModelRunner-1.1.8/examples/sscx_sample_dir/mechanisms/
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/sscx_sample_dir/mechanisms/CaDynamics_DC0.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/sscx_sample_dir/mechanisms/Ca_HVA2.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/sscx_sample_dir/mechanisms/Ca_LVAst.mod
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/sscx_sample_dir/mechanisms/Ih.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/sscx_sample_dir/mechanisms/K_Pst.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/sscx_sample_dir/mechanisms/K_Tst.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/sscx_sample_dir/mechanisms/KdShu2007.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/sscx_sample_dir/mechanisms/NaTg.mod
--rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/sscx_sample_dir/mechanisms/Nap_Et2.mod
--rw-r--r--   0 runner    (1001) docker     (123)    19708 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/sscx_sample_dir/mechanisms/ProbAMPANMDA_EMS.mod
--rw-r--r--   0 runner    (1001) docker     (123)    19859 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/sscx_sample_dir/mechanisms/ProbGABAAB_EMS.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/sscx_sample_dir/mechanisms/SK_E2.mod
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/sscx_sample_dir/mechanisms/SKv3_1.mod
--rw-r--r--   0 runner    (1001) docker     (123)    15181 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/sscx_sample_dir/mechanisms/StochKv3.mod
--rw-r--r--   0 runner    (1001) docker     (123)     3859 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/sscx_sample_dir/mechanisms/VecStim.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/sscx_sample_dir/mechanisms/notes.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:11:36.000000 EModelRunner-1.1.8/examples/sscx_sample_dir/morphology/
--rw-r--r--   0 runner    (1001) docker     (123)   135189 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/sscx_sample_dir/morphology/dend-C231296A-P4B2_axon-C200897C-P2_-_Scale_x1.000_y0.975_z1.000.asc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:11:36.000000 EModelRunner-1.1.8/examples/sscx_sample_dir/python_recordings/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/sscx_sample_dir/python_recordings/.keep
--rwxr-xr-x   0 runner    (1001) docker     (123)      229 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/sscx_sample_dir/run_hoc.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      322 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/sscx_sample_dir/run_py.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:11:36.000000 EModelRunner-1.1.8/examples/sscx_sample_dir/synapses/
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/sscx_sample_dir/synapses/mtype_map.tsv
--rw-r--r--   0 runner    (1001) docker     (123)   177229 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/sscx_sample_dir/synapses/synapses.tsv
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/sscx_sample_dir/synapses/synconf.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:11:36.000000 EModelRunner-1.1.8/examples/sscx_sample_dir/templates/
--rwxr-xr-x   0 runner    (1001) docker     (123)     7087 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/sscx_sample_dir/templates/cell_template_neurodamus.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     5695 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/sscx_sample_dir/templates/createsimulation.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/sscx_sample_dir/templates/features.hoc
--rw-r--r--   0 runner    (1001) docker     (123)     8149 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/sscx_sample_dir/templates/main_protocol.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     2814 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/sscx_sample_dir/templates/replace_axon_hoc.hoc
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/sscx_sample_dir/templates/run_hoc.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)    11711 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/sscx_sample_dir/templates/synapses.jinja2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:11:36.000000 EModelRunner-1.1.8/examples/synplas_sample_dir/
--rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/synplas_sample_dir/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)    15070 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/synplas_sample_dir/LICENSE_CC-BY-CA-SA-4.0
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:11:36.000000 EModelRunner-1.1.8/examples/synplas_sample_dir/config/
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/synplas_sample_dir/config/config_1Hz_10ms.ini
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/synplas_sample_dir/config/fit_params.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:11:36.000000 EModelRunner-1.1.8/examples/synplas_sample_dir/config/params/
--rw-r--r--   0 runner    (1001) docker     (123)    13406 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/synplas_sample_dir/config/params/final.json
--rw-r--r--   0 runner    (1001) docker     (123)     5585 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/synplas_sample_dir/config/params/pyr.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:11:36.000000 EModelRunner-1.1.8/examples/synplas_sample_dir/mechanisms/
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/synplas_sample_dir/mechanisms/CaDynamics_DC0.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/synplas_sample_dir/mechanisms/Ca_HVA2.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/synplas_sample_dir/mechanisms/Ca_LVAst.mod
--rw-r--r--   0 runner    (1001) docker     (123)    10423 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/synplas_sample_dir/mechanisms/DetAMPANMDA.mod
--rw-r--r--   0 runner    (1001) docker     (123)    10512 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/synplas_sample_dir/mechanisms/DetGABAAB.mod
--rw-r--r--   0 runner    (1001) docker     (123)    19936 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/synplas_sample_dir/mechanisms/GluSynapse.mod
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/synplas_sample_dir/mechanisms/Ih.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/synplas_sample_dir/mechanisms/K_Pst.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/synplas_sample_dir/mechanisms/K_Tst.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/synplas_sample_dir/mechanisms/KdShu2007.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/synplas_sample_dir/mechanisms/NaTg.mod
--rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/synplas_sample_dir/mechanisms/Nap_Et2.mod
--rw-r--r--   0 runner    (1001) docker     (123)    19708 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/synplas_sample_dir/mechanisms/ProbAMPANMDA_EMS.mod
--rw-r--r--   0 runner    (1001) docker     (123)    19859 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/synplas_sample_dir/mechanisms/ProbGABAAB_EMS.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/synplas_sample_dir/mechanisms/SK_E2.mod
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/synplas_sample_dir/mechanisms/SKv3_1.mod
--rw-r--r--   0 runner    (1001) docker     (123)    15181 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/synplas_sample_dir/mechanisms/StochKv3.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/synplas_sample_dir/mechanisms/TTXDynamicsSwitch.mod
--rw-r--r--   0 runner    (1001) docker     (123)     3859 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/synplas_sample_dir/mechanisms/VecStim.mod
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/synplas_sample_dir/mechanisms/gap.mod
--rw-r--r--   0 runner    (1001) docker     (123)    15094 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/synplas_sample_dir/mechanisms/netstim_inhpoisson.mod
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:11:36.000000 EModelRunner-1.1.8/examples/synplas_sample_dir/mechanisms/optimized/
--rw-r--r--   0 runner    (1001) docker     (123)    18042 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/synplas_sample_dir/mechanisms/optimized/ProbAMPANMDA_EMS.mod
--rw-r--r--   0 runner    (1001) docker     (123)    18098 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/synplas_sample_dir/mechanisms/optimized/ProbGABAAB_EMS.mod
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:11:36.000000 EModelRunner-1.1.8/examples/synplas_sample_dir/morphology/
--rw-r--r--   0 runner    (1001) docker     (123)   322804 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/synplas_sample_dir/morphology/dend-C120398A-P3_axon-sm100429a1-5_INT_idG_-_Scale_x1.000_y0.975_z1.000.asc
--rw-r--r--   0 runner    (1001) docker     (123)   491533 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/synplas_sample_dir/morphology/dend-sm100429a1-5_INT_idG_axon-sm100429a1-5_INT_idE_-_Scale_x1.000_y0.950_z1.000_-_Clone_0.asc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:11:36.000000 EModelRunner-1.1.8/examples/synplas_sample_dir/protocols/
--rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/synplas_sample_dir/protocols/spiketrain_1Hz_10ms.dat
--rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/synplas_sample_dir/protocols/stimuli_1Hz.json
--rwxr-xr-x   0 runner    (1001) docker     (123)      268 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/synplas_sample_dir/run.sh
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/synplas_sample_dir/run_pairsim.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:11:36.000000 EModelRunner-1.1.8/examples/synplas_sample_dir/synapses/
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/synplas_sample_dir/synapses/cpre_cpost.json
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/synplas_sample_dir/synapses/mtype_map.tsv
--rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/synplas_sample_dir/synapses/syn_extra_params.json
--rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/synplas_sample_dir/synapses/synapse_properties.json
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/synplas_sample_dir/synapses/synapses.tsv
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/synplas_sample_dir/synapses/synconf.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:11:36.000000 EModelRunner-1.1.8/examples/thalamus_sample_dir/
--rw-r--r--   0 runner    (1001) docker     (123)     3301 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/thalamus_sample_dir/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)    15070 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/thalamus_sample_dir/LICENSE_CC-BY-CA-SA-4.0
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/thalamus_sample_dir/cell_info.json
--rwxr-xr-x   0 runner    (1001) docker     (123)      214 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/thalamus_sample_dir/compile_mechanisms.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:11:36.000000 EModelRunner-1.1.8/examples/thalamus_sample_dir/config/
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/thalamus_sample_dir/config/config_recipe_prots_short.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:11:36.000000 EModelRunner-1.1.8/examples/thalamus_sample_dir/config/features/
--rw-r--r--   0 runner    (1001) docker     (123)     3844 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/thalamus_sample_dir/config/features/dNAD_ltb.json
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/thalamus_sample_dir/config/features/units.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:11:36.000000 EModelRunner-1.1.8/examples/thalamus_sample_dir/config/params/
--rw-r--r--   0 runner    (1001) docker     (123)     2473 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/thalamus_sample_dir/config/params/bAC_TC_VPL.json
--rw-r--r--   0 runner    (1001) docker     (123)     3711 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/thalamus_sample_dir/config/params/final.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:11:36.000000 EModelRunner-1.1.8/examples/thalamus_sample_dir/config/protocols/
--rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/thalamus_sample_dir/config/protocols/dNAD_ltb_short.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:11:36.000000 EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/CaDynamics_DC0.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/Ca_HVA.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/Ca_HVA2.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/Ca_LVAst.mod
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/Ih.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/K_Pst.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/K_Tst.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/KdShu2007.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/NaTg.mod
--rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/Nap_Et2.mod
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/SK_E2.mod
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/SKv3_1.mod
--rw-r--r--   0 runner    (1001) docker     (123)    15181 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/StochKv3.mod
--rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/TC_HH.mod
--rw-r--r--   0 runner    (1001) docker     (123)     3873 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/TC_ITGHK.mod
--rw-r--r--   0 runner    (1001) docker     (123)     3908 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/TC_ITGHK_Ama14.mod
--rw-r--r--   0 runner    (1001) docker     (123)     3798 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/TC_ITGHK_Des98.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/TC_Ih.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/TC_Ih_Bud97.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/TC_KCa_bk.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/TC_Kir2_2.mod
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/TC_Kleak.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/TC_NaP.mod
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/TC_Naleak.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/TC_Nap_Et2.mod
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/TC_cadecay.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/TC_iA.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/TC_iA_old.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/TC_iL.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/TC_ic.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/TC_ih2.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/TC_kahp.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/TC_kir_Con15.mod
--rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/ican.mod
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:11:36.000000 EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/other_versions/
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/other_versions/IKCa.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/other_versions/NaTg.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/other_versions/Nap_Et2.mod
--rw-r--r--   0 runner    (1001) docker     (123)     3873 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/other_versions/TC_ITGHK.mod
--rw-r--r--   0 runner    (1001) docker     (123)     3908 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/other_versions/TC_ITGHK_Ama14.mod
--rw-r--r--   0 runner    (1001) docker     (123)     3780 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/other_versions/TC_ITGHK_Wei2011.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/other_versions/TC_Ih.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/other_versions/TC_KCa_bk.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/other_versions/TC_Kir2_2.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/other_versions/TC_NaP.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/other_versions/TC_iA_old.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/other_versions/TC_ic.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/other_versions/TC_ih2.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/other_versions/TC_kahp.mod
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/other_versions/caidL.mod
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:11:36.000000 EModelRunner-1.1.8/examples/thalamus_sample_dir/morphology/
--rw-r--r--   0 runner    (1001) docker     (123)   384138 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/thalamus_sample_dir/morphology/dend-jy180118_C_idD_axon-AA0318_-_Scale_x1.000_y1.050_z1.000.asc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:11:36.000000 EModelRunner-1.1.8/examples/thalamus_sample_dir/python_recordings/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/thalamus_sample_dir/python_recordings/.gitkeep
--rwxr-xr-x   0 runner    (1001) docker     (123)      221 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/thalamus_sample_dir/run_py.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:11:36.000000 EModelRunner-1.1.8/examples/thalamus_sample_dir/synapses/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/examples/thalamus_sample_dir/synapses/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/requirements_docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 14:11:36.000000 EModelRunner-1.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2469 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-04-17 14:11:26.000000 EModelRunner-1.1.8/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:41:17.000000 EModelRunner-1.1.9/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      126 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/.compile_mod.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:41:17.000000 EModelRunner-1.1.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:41:17.000000 EModelRunner-1.1.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/.github/workflows/keep-alive.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11360 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/COPYING
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:41:17.000000 EModelRunner-1.1.9/EModelRunner.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13332 2023-06-01 13:41:17.000000 EModelRunner-1.1.9/EModelRunner.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11012 2023-06-01 13:41:17.000000 EModelRunner-1.1.9/EModelRunner.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 13:41:17.000000 EModelRunner-1.1.9/EModelRunner.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-01 13:41:17.000000 EModelRunner-1.1.9/EModelRunner.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-01 13:41:17.000000 EModelRunner-1.1.9/EModelRunner.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)    13332 2023-06-01 13:41:17.000000 EModelRunner-1.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10156 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:41:17.000000 EModelRunner-1.1.9/doc/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/doc/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:41:17.000000 EModelRunner-1.1.9/doc/source/
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/doc/source/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/doc/source/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3263 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/doc/source/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:41:17.000000 EModelRunner-1.1.9/doc/source/images/
+-rw-r--r--   0 runner    (1001) docker     (123)   207165 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/doc/source/images/GUI_screenshot.png
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/doc/source/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:41:17.000000 EModelRunner-1.1.9/doc/source/logo/
+-rw-r--r--   0 runner    (1001) docker     (123)   303675 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/doc/source/logo/BBP-eModelRunner.jpg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:41:17.000000 EModelRunner-1.1.9/emodelrunner/
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/emodelrunner/GUI.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:41:17.000000 EModelRunner-1.1.9/emodelrunner/GUI_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/emodelrunner/GUI_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42494 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/emodelrunner/GUI_utils/frames.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8725 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/emodelrunner/GUI_utils/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7805 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/emodelrunner/GUI_utils/plotshape.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18792 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/emodelrunner/GUI_utils/simulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3790 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/emodelrunner/GUI_utils/style.py
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/emodelrunner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9843 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/emodelrunner/cell.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:41:17.000000 EModelRunner-1.1.9/emodelrunner/configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/emodelrunner/configuration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4892 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/emodelrunner/configuration/configparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/emodelrunner/configuration/subgroups.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18287 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/emodelrunner/configuration/validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6263 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/emodelrunner/create_cells.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7565 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/emodelrunner/create_hoc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25018 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/emodelrunner/create_hoc_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/emodelrunner/create_recordings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/emodelrunner/create_stimuli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:41:17.000000 EModelRunner-1.1.9/emodelrunner/factsheets/
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/emodelrunner/factsheets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4302 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/emodelrunner/factsheets/experimental_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10833 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/emodelrunner/factsheets/ion_channel_mechanisms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20087 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/emodelrunner/factsheets/morphology_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7497 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/emodelrunner/factsheets/output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3856 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/emodelrunner/factsheets/physiology_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/emodelrunner/factsheets/units.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4155 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/emodelrunner/features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/emodelrunner/json_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13656 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/emodelrunner/load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/emodelrunner/locations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:41:17.000000 EModelRunner-1.1.9/emodelrunner/morphology/
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/emodelrunner/morphology/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/emodelrunner/morphology/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7315 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/emodelrunner/morphology/morphology.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4391 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/emodelrunner/output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/emodelrunner/parsing_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:41:17.000000 EModelRunner-1.1.9/emodelrunner/protocols/
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/emodelrunner/protocols/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15690 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/emodelrunner/protocols/create_protocols.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5734 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/emodelrunner/protocols/protocols_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26089 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/emodelrunner/protocols/reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46821 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/emodelrunner/protocols/sscx_protocols.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16774 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/emodelrunner/protocols/synplas_protocols.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35315 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/emodelrunner/protocols/thalamus_protocols.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/emodelrunner/recordings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3101 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/emodelrunner/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4663 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/emodelrunner/run_pairsim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4379 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/emodelrunner/run_synplas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7750 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/emodelrunner/stimuli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:41:17.000000 EModelRunner-1.1.9/emodelrunner/synapses/
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/emodelrunner/synapses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/emodelrunner/synapses/create_locations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7288 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/emodelrunner/synapses/glusynapse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6968 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/emodelrunner/synapses/mechanism.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7608 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/emodelrunner/synapses/minis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3486 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/emodelrunner/synapses/recordings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10317 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/emodelrunner/synapses/stimuli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6473 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/emodelrunner/synapses/synapse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9719 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/emodelrunner/synplas_analysis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:41:17.000000 EModelRunner-1.1.9/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:41:17.000000 EModelRunner-1.1.9/examples/sscx_sample_dir/
+-rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/examples/sscx_sample_dir/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    15070 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/examples/sscx_sample_dir/LICENSE_CC-BY-CA-SA-4.0
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/examples/sscx_sample_dir/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:41:17.000000 EModelRunner-1.1.9/examples/sscx_sample_dir/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/examples/sscx_sample_dir/config/config_allsteps.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/examples/sscx_sample_dir/config/config_factsheets.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/examples/sscx_sample_dir/config/config_multiprotocols.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/examples/sscx_sample_dir/config/config_recipe_protocols.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/examples/sscx_sample_dir/config/config_singlestep.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/examples/sscx_sample_dir/config/config_synapses.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/examples/sscx_sample_dir/config/config_synapses_short.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:41:17.000000 EModelRunner-1.1.9/examples/sscx_sample_dir/config/features/
+-rw-r--r--   0 runner    (1001) docker     (123)    14709 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/examples/sscx_sample_dir/config/features/cADpyr_L4PC.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:41:17.000000 EModelRunner-1.1.9/examples/sscx_sample_dir/config/params/
+-rw-r--r--   0 runner    (1001) docker     (123)     6710 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/examples/sscx_sample_dir/config/params/final.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10218 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/examples/sscx_sample_dir/config/params/pyr.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:41:17.000000 EModelRunner-1.1.9/examples/sscx_sample_dir/config/protocols/
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/examples/sscx_sample_dir/config/protocols/RmpRiTau.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/examples/sscx_sample_dir/config/protocols/allsteps.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5372 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/examples/sscx_sample_dir/config/protocols/cADpyr_L4PC.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/examples/sscx_sample_dir/config/protocols/multiprotocols.json
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/examples/sscx_sample_dir/config/protocols/singlestep.json
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/examples/sscx_sample_dir/config/protocols/synapses.json
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/examples/sscx_sample_dir/config/protocols/synapses_short.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:41:17.000000 EModelRunner-1.1.9/examples/sscx_sample_dir/hoc_recordings/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/examples/sscx_sample_dir/hoc_recordings/.keep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:41:17.000000 EModelRunner-1.1.9/examples/sscx_sample_dir/mechanisms/
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/examples/sscx_sample_dir/mechanisms/CaDynamics_DC0.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/examples/sscx_sample_dir/mechanisms/Ca_HVA2.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/examples/sscx_sample_dir/mechanisms/Ca_LVAst.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/examples/sscx_sample_dir/mechanisms/Ih.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/examples/sscx_sample_dir/mechanisms/K_Pst.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/examples/sscx_sample_dir/mechanisms/K_Tst.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/examples/sscx_sample_dir/mechanisms/KdShu2007.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/examples/sscx_sample_dir/mechanisms/NaTg.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/examples/sscx_sample_dir/mechanisms/Nap_Et2.mod
+-rw-r--r--   0 runner    (1001) docker     (123)    19708 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/examples/sscx_sample_dir/mechanisms/ProbAMPANMDA_EMS.mod
+-rw-r--r--   0 runner    (1001) docker     (123)    19859 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/examples/sscx_sample_dir/mechanisms/ProbGABAAB_EMS.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/examples/sscx_sample_dir/mechanisms/SK_E2.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/examples/sscx_sample_dir/mechanisms/SKv3_1.mod
+-rw-r--r--   0 runner    (1001) docker     (123)    15181 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/examples/sscx_sample_dir/mechanisms/StochKv3.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     3859 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/examples/sscx_sample_dir/mechanisms/VecStim.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/examples/sscx_sample_dir/mechanisms/notes.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:41:17.000000 EModelRunner-1.1.9/examples/sscx_sample_dir/morphology/
+-rw-r--r--   0 runner    (1001) docker     (123)   135189 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/examples/sscx_sample_dir/morphology/dend-C231296A-P4B2_axon-C200897C-P2_-_Scale_x1.000_y0.975_z1.000.asc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:41:17.000000 EModelRunner-1.1.9/examples/sscx_sample_dir/python_recordings/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/examples/sscx_sample_dir/python_recordings/.keep
+-rwxr-xr-x   0 runner    (1001) docker     (123)      229 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/examples/sscx_sample_dir/run_hoc.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      322 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/examples/sscx_sample_dir/run_py.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:41:17.000000 EModelRunner-1.1.9/examples/sscx_sample_dir/synapses/
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/examples/sscx_sample_dir/synapses/mtype_map.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)   177229 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/examples/sscx_sample_dir/synapses/synapses.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/examples/sscx_sample_dir/synapses/synconf.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:41:17.000000 EModelRunner-1.1.9/examples/sscx_sample_dir/templates/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7087 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/examples/sscx_sample_dir/templates/cell_template_neurodamus.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     5695 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/examples/sscx_sample_dir/templates/createsimulation.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/examples/sscx_sample_dir/templates/features.hoc
+-rw-r--r--   0 runner    (1001) docker     (123)     8149 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/examples/sscx_sample_dir/templates/main_protocol.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     2814 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/examples/sscx_sample_dir/templates/replace_axon_hoc.hoc
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/examples/sscx_sample_dir/templates/run_hoc.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)    11711 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/examples/sscx_sample_dir/templates/synapses.jinja2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:41:17.000000 EModelRunner-1.1.9/examples/synplas_sample_dir/
+-rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/examples/synplas_sample_dir/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    15070 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/examples/synplas_sample_dir/LICENSE_CC-BY-CA-SA-4.0
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:41:17.000000 EModelRunner-1.1.9/examples/synplas_sample_dir/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/examples/synplas_sample_dir/config/config_1Hz_10ms.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/examples/synplas_sample_dir/config/fit_params.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:41:17.000000 EModelRunner-1.1.9/examples/synplas_sample_dir/config/params/
+-rw-r--r--   0 runner    (1001) docker     (123)    13406 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/examples/synplas_sample_dir/config/params/final.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5585 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/examples/synplas_sample_dir/config/params/pyr.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:41:17.000000 EModelRunner-1.1.9/examples/synplas_sample_dir/mechanisms/
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/examples/synplas_sample_dir/mechanisms/CaDynamics_DC0.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/examples/synplas_sample_dir/mechanisms/Ca_HVA2.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/examples/synplas_sample_dir/mechanisms/Ca_LVAst.mod
+-rw-r--r--   0 runner    (1001) docker     (123)    10423 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/examples/synplas_sample_dir/mechanisms/DetAMPANMDA.mod
+-rw-r--r--   0 runner    (1001) docker     (123)    10512 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/examples/synplas_sample_dir/mechanisms/DetGABAAB.mod
+-rw-r--r--   0 runner    (1001) docker     (123)    19936 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/examples/synplas_sample_dir/mechanisms/GluSynapse.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/examples/synplas_sample_dir/mechanisms/Ih.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/examples/synplas_sample_dir/mechanisms/K_Pst.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/examples/synplas_sample_dir/mechanisms/K_Tst.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/examples/synplas_sample_dir/mechanisms/KdShu2007.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/examples/synplas_sample_dir/mechanisms/NaTg.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/examples/synplas_sample_dir/mechanisms/Nap_Et2.mod
+-rw-r--r--   0 runner    (1001) docker     (123)    19708 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/examples/synplas_sample_dir/mechanisms/ProbAMPANMDA_EMS.mod
+-rw-r--r--   0 runner    (1001) docker     (123)    19859 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/examples/synplas_sample_dir/mechanisms/ProbGABAAB_EMS.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/examples/synplas_sample_dir/mechanisms/SK_E2.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/examples/synplas_sample_dir/mechanisms/SKv3_1.mod
+-rw-r--r--   0 runner    (1001) docker     (123)    15181 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/examples/synplas_sample_dir/mechanisms/StochKv3.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/examples/synplas_sample_dir/mechanisms/TTXDynamicsSwitch.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     3859 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/examples/synplas_sample_dir/mechanisms/VecStim.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/examples/synplas_sample_dir/mechanisms/gap.mod
+-rw-r--r--   0 runner    (1001) docker     (123)    15094 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/examples/synplas_sample_dir/mechanisms/netstim_inhpoisson.mod
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:41:17.000000 EModelRunner-1.1.9/examples/synplas_sample_dir/mechanisms/optimized/
+-rw-r--r--   0 runner    (1001) docker     (123)    18042 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/examples/synplas_sample_dir/mechanisms/optimized/ProbAMPANMDA_EMS.mod
+-rw-r--r--   0 runner    (1001) docker     (123)    18098 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/examples/synplas_sample_dir/mechanisms/optimized/ProbGABAAB_EMS.mod
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:41:17.000000 EModelRunner-1.1.9/examples/synplas_sample_dir/morphology/
+-rw-r--r--   0 runner    (1001) docker     (123)   322804 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/examples/synplas_sample_dir/morphology/dend-C120398A-P3_axon-sm100429a1-5_INT_idG_-_Scale_x1.000_y0.975_z1.000.asc
+-rw-r--r--   0 runner    (1001) docker     (123)   491533 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/examples/synplas_sample_dir/morphology/dend-sm100429a1-5_INT_idG_axon-sm100429a1-5_INT_idE_-_Scale_x1.000_y0.950_z1.000_-_Clone_0.asc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:41:17.000000 EModelRunner-1.1.9/examples/synplas_sample_dir/protocols/
+-rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/examples/synplas_sample_dir/protocols/spiketrain_1Hz_10ms.dat
+-rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/examples/synplas_sample_dir/protocols/stimuli_1Hz.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)      268 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/examples/synplas_sample_dir/run.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/examples/synplas_sample_dir/run_pairsim.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:41:17.000000 EModelRunner-1.1.9/examples/synplas_sample_dir/synapses/
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/examples/synplas_sample_dir/synapses/cpre_cpost.json
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/examples/synplas_sample_dir/synapses/mtype_map.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/examples/synplas_sample_dir/synapses/syn_extra_params.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/examples/synplas_sample_dir/synapses/synapse_properties.json
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/examples/synplas_sample_dir/synapses/synapses.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/examples/synplas_sample_dir/synapses/synconf.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:41:17.000000 EModelRunner-1.1.9/examples/thalamus_sample_dir/
+-rw-r--r--   0 runner    (1001) docker     (123)     3301 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/examples/thalamus_sample_dir/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    15070 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/examples/thalamus_sample_dir/LICENSE_CC-BY-CA-SA-4.0
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/examples/thalamus_sample_dir/cell_info.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)      214 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/examples/thalamus_sample_dir/compile_mechanisms.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:41:17.000000 EModelRunner-1.1.9/examples/thalamus_sample_dir/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/examples/thalamus_sample_dir/config/config_recipe_prots_short.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:41:17.000000 EModelRunner-1.1.9/examples/thalamus_sample_dir/config/features/
+-rw-r--r--   0 runner    (1001) docker     (123)     3844 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/examples/thalamus_sample_dir/config/features/dNAD_ltb.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:41:17.000000 EModelRunner-1.1.9/examples/thalamus_sample_dir/config/params/
+-rw-r--r--   0 runner    (1001) docker     (123)     2473 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/examples/thalamus_sample_dir/config/params/bAC_TC_VPL.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3711 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/examples/thalamus_sample_dir/config/params/final.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:41:17.000000 EModelRunner-1.1.9/examples/thalamus_sample_dir/config/protocols/
+-rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/examples/thalamus_sample_dir/config/protocols/dNAD_ltb_short.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:41:17.000000 EModelRunner-1.1.9/examples/thalamus_sample_dir/mechanisms/
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/examples/thalamus_sample_dir/mechanisms/CaDynamics_DC0.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/examples/thalamus_sample_dir/mechanisms/Ca_HVA.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/examples/thalamus_sample_dir/mechanisms/Ca_HVA2.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/examples/thalamus_sample_dir/mechanisms/Ca_LVAst.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/examples/thalamus_sample_dir/mechanisms/Ih.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/examples/thalamus_sample_dir/mechanisms/K_Pst.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/examples/thalamus_sample_dir/mechanisms/K_Tst.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/examples/thalamus_sample_dir/mechanisms/KdShu2007.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/examples/thalamus_sample_dir/mechanisms/NaTg.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/examples/thalamus_sample_dir/mechanisms/Nap_Et2.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/examples/thalamus_sample_dir/mechanisms/SK_E2.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/examples/thalamus_sample_dir/mechanisms/SKv3_1.mod
+-rw-r--r--   0 runner    (1001) docker     (123)    15181 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/examples/thalamus_sample_dir/mechanisms/StochKv3.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/examples/thalamus_sample_dir/mechanisms/TC_HH.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     3873 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/examples/thalamus_sample_dir/mechanisms/TC_ITGHK.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     3908 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/examples/thalamus_sample_dir/mechanisms/TC_ITGHK_Ama14.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     3798 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/examples/thalamus_sample_dir/mechanisms/TC_ITGHK_Des98.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/examples/thalamus_sample_dir/mechanisms/TC_Ih.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/examples/thalamus_sample_dir/mechanisms/TC_Ih_Bud97.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/examples/thalamus_sample_dir/mechanisms/TC_KCa_bk.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/examples/thalamus_sample_dir/mechanisms/TC_Kir2_2.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/examples/thalamus_sample_dir/mechanisms/TC_Kleak.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/examples/thalamus_sample_dir/mechanisms/TC_NaP.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/examples/thalamus_sample_dir/mechanisms/TC_Naleak.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/examples/thalamus_sample_dir/mechanisms/TC_Nap_Et2.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/examples/thalamus_sample_dir/mechanisms/TC_cadecay.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/examples/thalamus_sample_dir/mechanisms/TC_iA.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/examples/thalamus_sample_dir/mechanisms/TC_iA_old.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/examples/thalamus_sample_dir/mechanisms/TC_iL.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/examples/thalamus_sample_dir/mechanisms/TC_ic.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/examples/thalamus_sample_dir/mechanisms/TC_ih2.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/examples/thalamus_sample_dir/mechanisms/TC_kahp.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/examples/thalamus_sample_dir/mechanisms/TC_kir_Con15.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/examples/thalamus_sample_dir/mechanisms/ican.mod
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:41:17.000000 EModelRunner-1.1.9/examples/thalamus_sample_dir/mechanisms/other_versions/
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/examples/thalamus_sample_dir/mechanisms/other_versions/IKCa.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/examples/thalamus_sample_dir/mechanisms/other_versions/NaTg.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/examples/thalamus_sample_dir/mechanisms/other_versions/Nap_Et2.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     3873 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/examples/thalamus_sample_dir/mechanisms/other_versions/TC_ITGHK.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     3908 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/examples/thalamus_sample_dir/mechanisms/other_versions/TC_ITGHK_Ama14.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     3780 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/examples/thalamus_sample_dir/mechanisms/other_versions/TC_ITGHK_Wei2011.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/examples/thalamus_sample_dir/mechanisms/other_versions/TC_Ih.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/examples/thalamus_sample_dir/mechanisms/other_versions/TC_KCa_bk.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/examples/thalamus_sample_dir/mechanisms/other_versions/TC_Kir2_2.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/examples/thalamus_sample_dir/mechanisms/other_versions/TC_NaP.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/examples/thalamus_sample_dir/mechanisms/other_versions/TC_iA_old.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/examples/thalamus_sample_dir/mechanisms/other_versions/TC_ic.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/examples/thalamus_sample_dir/mechanisms/other_versions/TC_ih2.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/examples/thalamus_sample_dir/mechanisms/other_versions/TC_kahp.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/examples/thalamus_sample_dir/mechanisms/other_versions/caidL.mod
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:41:17.000000 EModelRunner-1.1.9/examples/thalamus_sample_dir/morphology/
+-rw-r--r--   0 runner    (1001) docker     (123)   384138 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/examples/thalamus_sample_dir/morphology/dend-jy180118_C_idD_axon-AA0318_-_Scale_x1.000_y1.050_z1.000.asc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:41:17.000000 EModelRunner-1.1.9/examples/thalamus_sample_dir/python_recordings/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/examples/thalamus_sample_dir/python_recordings/.gitkeep
+-rwxr-xr-x   0 runner    (1001) docker     (123)      221 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/examples/thalamus_sample_dir/run_py.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:41:17.000000 EModelRunner-1.1.9/examples/thalamus_sample_dir/synapses/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/examples/thalamus_sample_dir/synapses/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/requirements_docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 13:41:17.000000 EModelRunner-1.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2949 2023-06-01 13:41:06.000000 EModelRunner-1.1.9/tox.ini
```

### Comparing `EModelRunner-1.1.8/.github/workflows/build.yml` & `EModelRunner-1.1.9/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.8/.github/workflows/keep-alive.yml` & `EModelRunner-1.1.9/.github/workflows/keep-alive.yml`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.8/.github/workflows/test.yml` & `EModelRunner-1.1.9/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.8/.gitignore` & `EModelRunner-1.1.9/.gitignore`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 *.pyc
 *.swp
 coverage.xml
 coverage.json
 coverage.html
+.coverage
+.coverage.*
 *.egg-info
 .coverage
 doc/build
 doc/source/generated
 doc/source/_autosummary
 .tox
 build
```

### Comparing `EModelRunner-1.1.8/.pylintrc` & `EModelRunner-1.1.9/.pylintrc`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.8/CONTRIBUTING.rst` & `EModelRunner-1.1.9/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.8/COPYING` & `EModelRunner-1.1.9/COPYING`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.8/EModelRunner.egg-info/PKG-INFO` & `EModelRunner-1.1.9/EModelRunner.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EModelRunner
-Version: 1.1.8
+Version: 1.1.9
 Summary: Runs cells from Blue Brain Project cell packages, such as sscx, synapse plasticity, etc.
 Home-page: https://github.com/BlueBrain/EModelRunner
 Author: Blue Brain Project, EPFL
 License: Apache 2.0
 Project-URL: Tracker, https://github.com/BlueBrain/EModelRunner/issues
 Project-URL: Source, https://github.com/BlueBrain/EModelRunner
 Project-URL: Documentation, https://emodelrunner.readthedocs.io/en/latest
```

### Comparing `EModelRunner-1.1.8/EModelRunner.egg-info/SOURCES.txt` & `EModelRunner-1.1.9/EModelRunner.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -60,14 +60,15 @@
 emodelrunner/configuration/validator.py
 emodelrunner/factsheets/__init__.py
 emodelrunner/factsheets/experimental_features.py
 emodelrunner/factsheets/ion_channel_mechanisms.py
 emodelrunner/factsheets/morphology_features.py
 emodelrunner/factsheets/output.py
 emodelrunner/factsheets/physiology_features.py
+emodelrunner/factsheets/units.py
 emodelrunner/morphology/__init__.py
 emodelrunner/morphology/builder.py
 emodelrunner/morphology/morphology.py
 emodelrunner/protocols/__init__.py
 emodelrunner/protocols/create_protocols.py
 emodelrunner/protocols/protocols_func.py
 emodelrunner/protocols/reader.py
@@ -91,15 +92,14 @@
 examples/sscx_sample_dir/config/config_factsheets.ini
 examples/sscx_sample_dir/config/config_multiprotocols.ini
 examples/sscx_sample_dir/config/config_recipe_protocols.ini
 examples/sscx_sample_dir/config/config_singlestep.ini
 examples/sscx_sample_dir/config/config_synapses.ini
 examples/sscx_sample_dir/config/config_synapses_short.ini
 examples/sscx_sample_dir/config/features/cADpyr_L4PC.json
-examples/sscx_sample_dir/config/features/units.json
 examples/sscx_sample_dir/config/params/final.json
 examples/sscx_sample_dir/config/params/pyr.json
 examples/sscx_sample_dir/config/protocols/RmpRiTau.json
 examples/sscx_sample_dir/config/protocols/allsteps.json
 examples/sscx_sample_dir/config/protocols/cADpyr_L4PC.json
 examples/sscx_sample_dir/config/protocols/multiprotocols.json
 examples/sscx_sample_dir/config/protocols/singlestep.json
@@ -178,15 +178,14 @@
 examples/thalamus_sample_dir/LICENSE.txt
 examples/thalamus_sample_dir/LICENSE_CC-BY-CA-SA-4.0
 examples/thalamus_sample_dir/cell_info.json
 examples/thalamus_sample_dir/compile_mechanisms.sh
 examples/thalamus_sample_dir/run_py.sh
 examples/thalamus_sample_dir/config/config_recipe_prots_short.ini
 examples/thalamus_sample_dir/config/features/dNAD_ltb.json
-examples/thalamus_sample_dir/config/features/units.json
 examples/thalamus_sample_dir/config/params/bAC_TC_VPL.json
 examples/thalamus_sample_dir/config/params/final.json
 examples/thalamus_sample_dir/config/protocols/dNAD_ltb_short.json
 examples/thalamus_sample_dir/mechanisms/CaDynamics_DC0.mod
 examples/thalamus_sample_dir/mechanisms/Ca_HVA.mod
 examples/thalamus_sample_dir/mechanisms/Ca_HVA2.mod
 examples/thalamus_sample_dir/mechanisms/Ca_LVAst.mod
```

### Comparing `EModelRunner-1.1.8/LICENSE.txt` & `EModelRunner-1.1.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.8/PKG-INFO` & `EModelRunner-1.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EModelRunner
-Version: 1.1.8
+Version: 1.1.9
 Summary: Runs cells from Blue Brain Project cell packages, such as sscx, synapse plasticity, etc.
 Home-page: https://github.com/BlueBrain/EModelRunner
 Author: Blue Brain Project, EPFL
 License: Apache 2.0
 Project-URL: Tracker, https://github.com/BlueBrain/EModelRunner/issues
 Project-URL: Source, https://github.com/BlueBrain/EModelRunner
 Project-URL: Documentation, https://emodelrunner.readthedocs.io/en/latest
```

### Comparing `EModelRunner-1.1.8/README.rst` & `EModelRunner-1.1.9/README.rst`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.8/doc/Makefile` & `EModelRunner-1.1.9/doc/Makefile`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.8/doc/source/conf.py` & `EModelRunner-1.1.9/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.8/doc/source/images/GUI_screenshot.png` & `EModelRunner-1.1.9/doc/source/images/GUI_screenshot.png`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.8/doc/source/logo/BBP-eModelRunner.jpg` & `EModelRunner-1.1.9/doc/source/logo/BBP-eModelRunner.jpg`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.8/emodelrunner/GUI.py` & `EModelRunner-1.1.9/emodelrunner/GUI.py`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.8/emodelrunner/GUI_utils/__init__.py` & `EModelRunner-1.1.9/emodelrunner/GUI_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.8/emodelrunner/GUI_utils/frames.py` & `EModelRunner-1.1.9/emodelrunner/GUI_utils/frames.py`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.8/emodelrunner/GUI_utils/interface.py` & `EModelRunner-1.1.9/emodelrunner/GUI_utils/interface.py`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.8/emodelrunner/GUI_utils/plotshape.py` & `EModelRunner-1.1.9/emodelrunner/GUI_utils/plotshape.py`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.8/emodelrunner/GUI_utils/simulator.py` & `EModelRunner-1.1.9/emodelrunner/GUI_utils/simulator.py`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.8/emodelrunner/GUI_utils/style.py` & `EModelRunner-1.1.9/emodelrunner/GUI_utils/style.py`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.8/emodelrunner/__init__.py` & `EModelRunner-1.1.9/emodelrunner/__init__.py`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.8/emodelrunner/cell.py` & `EModelRunner-1.1.9/emodelrunner/cell.py`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.8/emodelrunner/configuration/__init__.py` & `EModelRunner-1.1.9/emodelrunner/configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.8/emodelrunner/configuration/configparser.py` & `EModelRunner-1.1.9/emodelrunner/configuration/configparser.py`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.8/emodelrunner/configuration/subgroups.py` & `EModelRunner-1.1.9/emodelrunner/configuration/subgroups.py`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.8/emodelrunner/configuration/validator.py` & `EModelRunner-1.1.9/emodelrunner/configuration/validator.py`

 * *Files 0% similar despite different names*

```diff
@@ -185,15 +185,14 @@
             # name to use for the hoc synapse template
             "hoc_synapse_template_name": "hoc_synapses",
         },
         "Paths": {
             "memodel_dir": ".",
             "output_dir": "%(memodel_dir)s/python_recordings",
             "params_path": "%(memodel_dir)s/config/params/final.json",
-            "units_path": "%(memodel_dir)s/config/features/units.json",
             "templates_dir": "%(memodel_dir)s/templates",
             "cell_template_path": "%(templates_dir)s/cell_template_neurodamus.jinja2",
             "run_hoc_template_path": "%(templates_dir)s/run_hoc.jinja2",
             "createsimulation_template_path": "%(templates_dir)s/createsimulation.jinja2",
             "synapses_template_path": "%(templates_dir)s/synapses.jinja2",
             "main_protocol_template_path": "%(templates_dir)s/main_protocol.jinja2",
             "features_hoc_template_path": "%(templates_dir)s/features.hoc",
@@ -244,15 +243,14 @@
                     "morph_path": lambda n: Path(n).exists(),
                     "prot_path": lambda n: Path(n).exists(),
                     "features_path": lambda n: Path(n).exists(),
                     "unoptimized_params_path": lambda n: Path(n).exists(),
                     "memodel_dir": lambda n: Path(n).exists(),
                     "output_dir": lambda n: Path(n).exists(),
                     "params_path": lambda n: Path(n).exists(),
-                    "units_path": lambda n: Path(n).exists(),
                     "templates_dir": lambda n: Path(n).exists(),
                     "cell_template_path": lambda n: Path(n).exists(),
                     "run_hoc_template_path": lambda n: Path(n).exists(),
                     "createsimulation_template_path": lambda n: Path(n).exists(),
                     "synapses_template_path": lambda n: Path(n).exists(),
                     "main_protocol_template_path": lambda n: Path(n).exists(),
                     "features_hoc_template_path": lambda n: Path(n).exists(),
@@ -301,15 +299,14 @@
             "seed": "846515",
             "rng_settings_mode": "Random123",  # can be "Random123" or "Compatibility"
         },
         "Paths": {
             "memodel_dir": ".",
             "output_dir": "%(memodel_dir)s/python_recordings",
             "params_path": "%(memodel_dir)s/config/params/final.json",
-            "units_path": "%(memodel_dir)s/config/features/units.json",
             "syn_dir": "%(memodel_dir)s/synapses",
             "syn_data_file": "synapses.tsv",
             "syn_conf_file": "synconf.txt",
             "syn_mtype_map": "mtype_map.tsv",
         },
     }
 
@@ -344,15 +341,14 @@
                     "morph_path": lambda n: Path(n).exists(),
                     "prot_path": lambda n: Path(n).exists(),
                     "features_path": lambda n: Path(n).exists(),
                     "unoptimized_params_path": lambda n: Path(n).exists(),
                     "memodel_dir": lambda n: Path(n).exists(),
                     "output_dir": lambda n: Path(n).exists(),
                     "params_path": lambda n: Path(n).exists(),
-                    "units_path": lambda n: Path(n).exists(),
                     "syn_dir": lambda n: Path(n).exists(),
                     "syn_data_file": And(str, len),
                     "syn_conf_file": And(str, len),
                     "syn_mtype_map": And(str, len),
                 },
             }
         )
```

### Comparing `EModelRunner-1.1.8/emodelrunner/create_cells.py` & `EModelRunner-1.1.9/emodelrunner/create_cells.py`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.8/emodelrunner/create_hoc.py` & `EModelRunner-1.1.9/emodelrunner/create_hoc.py`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.8/emodelrunner/create_hoc_tools.py` & `EModelRunner-1.1.9/emodelrunner/create_hoc_tools.py`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.8/emodelrunner/create_recordings.py` & `EModelRunner-1.1.9/emodelrunner/create_recordings.py`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.8/emodelrunner/create_stimuli.py` & `EModelRunner-1.1.9/emodelrunner/create_stimuli.py`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.8/emodelrunner/factsheets/__init__.py` & `EModelRunner-1.1.9/emodelrunner/factsheets/__init__.py`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.8/emodelrunner/factsheets/experimental_features.py` & `EModelRunner-1.1.9/emodelrunner/factsheets/experimental_features.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import logging
+from emodelrunner.factsheets.units import feature_units
 
 logger = logging.getLogger(__name__)
 
 
 def morphology_used_in_fitting(optimized_params_dict, emodel):
     """Returns the morphology name from finals.json used in model fitting.
 
@@ -32,34 +33,33 @@
     """
     emodel_params = optimized_params_dict[emodel]
     morph_path = emodel_params["morph_path"]
     morph_name = morph_path.split("/")[-1]
     return morph_name
 
 
-def get_feature_dict(feature, units, morphology_prefix, stimulus, location, fitness):
+def get_feature_dict(feature, morphology_prefix, stimulus, location, fitness):
     """Return dict containing one feature.
 
     Args:
         feature (dict): contains feature name and mean and std of feature
-        units (dict): contains the units for the feature
         morphology_prefix (str): prefix used in the fitness key to the feature
         stimulus (str): name of the stimulus used for this feature
         location (str): name of the location for which the feature is calculated
         fitness (dict): contains the fitness of the feature
 
     Returns:
         dict containing name, values, unit and model fitness of the feature
     """
     feature_name = feature["feature"]
     mean = feature["val"][0]
     std = feature["val"][1]
 
     try:
-        unit = units[feature_name]
+        unit = feature_units[feature_name]
     except KeyError:
         logger.warning(
             "%s was not found in units file. Setting unit to ''.", feature_name
         )
         unit = ""
 
     key_fitness = ".".join((morphology_prefix, stimulus, location, feature_name))
@@ -77,23 +77,22 @@
         "values": [{"mean": mean, "std": std}],
         "unit": unit,
         "model fitness": fit,
     }
 
 
 def get_exp_features_data(
-    emodel, morphology_prefix, features_dict, units, optimized_params_dict
+    emodel, morphology_prefix, features_dict, optimized_params_dict
 ):
     """Returns a dict containing mean and std of experimental features and model fitness.
 
     Args:
         emodel (str): name of the emodel
         morphology_prefix (str): prefix used in the fitness key to the feature
         features_dict (dict): contains the features
-        units (dict): contains the units for the features
         optimized_params_dict (dict): contains the optimized parameters,
             as well as the original morphology path
 
     Returns:
         dict containing the output feature dicts and the original morph name used in model fitting
     """
     # pylint: disable=too-many-locals
@@ -104,15 +103,15 @@
     for stimulus, stim_data in features_dict.items():
         stim_dict = {}
         for location, loc_data in stim_data.items():
             features_list = []
             for feature in loc_data:
                 features_list.append(
                     get_feature_dict(
-                        feature, units, morphology_prefix, stimulus, location, fitness
+                        feature, morphology_prefix, stimulus, location, fitness
                     )
                 )
             loc_dict = {"features": features_list}
             stim_dict[location] = loc_dict
         values_dict[stimulus] = stim_dict
     values = [values_dict]
```

### Comparing `EModelRunner-1.1.8/emodelrunner/factsheets/ion_channel_mechanisms.py` & `EModelRunner-1.1.9/emodelrunner/factsheets/ion_channel_mechanisms.py`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.8/emodelrunner/factsheets/morphology_features.py` & `EModelRunner-1.1.9/emodelrunner/factsheets/morphology_features.py`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.8/emodelrunner/factsheets/output.py` & `EModelRunner-1.1.9/emodelrunner/factsheets/output.py`

 * *Files 4% similar despite different names*

```diff
@@ -169,41 +169,38 @@
     )
 
 
 def write_emodel_json(
     emodel,
     morphology_prefix,
     features_dict,
-    feature_units_dict,
     unoptimized_params_dict,
     optimized_params_dict,
     output_path,
 ):
     """Write the e-model factsheet json file.
 
     The output metype factsheet contains experimental features and channel mechanisms data.
 
     Args:
         emodel (str): name of the emodel
         morphology_prefix (str): prefix used in the fitness key to the experimental feature
         features_dict (dict): contains the experimental features
-        feature_units_dict (dict): contains the units for the experimental features
         unoptimized_params_dict (dict): contains the unoptimized parameters,
             and also contains the decay and exponential equations
         optimized_params_dict (dict): contains the optimized parameters,
             as well as the original morphology path
         output_path (str): path to the e-model factsheet output
     """
     output_path = Path(output_path)
     output_path.parent.mkdir(parents=True, exist_ok=True)
     exp_features = get_exp_features_data(
         emodel,
         morphology_prefix,
         features_dict,
-        feature_units_dict,
         optimized_params_dict,
     )
     channel_mechanisms = get_mechanisms_data(
         emodel, optimized_params_dict, unoptimized_params_dict
     )
 
     output = [
```

### Comparing `EModelRunner-1.1.8/emodelrunner/factsheets/physiology_features.py` & `EModelRunner-1.1.9/emodelrunner/factsheets/physiology_features.py`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.8/emodelrunner/features.py` & `EModelRunner-1.1.9/emodelrunner/features.py`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.8/emodelrunner/json_utilities.py` & `EModelRunner-1.1.9/emodelrunner/json_utilities.py`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.8/emodelrunner/load.py` & `EModelRunner-1.1.9/emodelrunner/load.py`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.8/emodelrunner/locations.py` & `EModelRunner-1.1.9/emodelrunner/locations.py`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.8/emodelrunner/morphology/__init__.py` & `EModelRunner-1.1.9/emodelrunner/morphology/__init__.py`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.8/emodelrunner/morphology/builder.py` & `EModelRunner-1.1.9/emodelrunner/morphology/builder.py`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.8/emodelrunner/morphology/morphology.py` & `EModelRunner-1.1.9/emodelrunner/morphology/morphology.py`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.8/emodelrunner/output.py` & `EModelRunner-1.1.9/emodelrunner/output.py`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.8/emodelrunner/parsing_utilities.py` & `EModelRunner-1.1.9/emodelrunner/parsing_utilities.py`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.8/emodelrunner/protocols/__init__.py` & `EModelRunner-1.1.9/emodelrunner/protocols/__init__.py`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.8/emodelrunner/protocols/create_protocols.py` & `EModelRunner-1.1.9/emodelrunner/protocols/create_protocols.py`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.8/emodelrunner/protocols/protocols_func.py` & `EModelRunner-1.1.9/emodelrunner/protocols/protocols_func.py`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.8/emodelrunner/protocols/reader.py` & `EModelRunner-1.1.9/emodelrunner/protocols/reader.py`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.8/emodelrunner/protocols/sscx_protocols.py` & `EModelRunner-1.1.9/emodelrunner/protocols/sscx_protocols.py`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.8/emodelrunner/protocols/synplas_protocols.py` & `EModelRunner-1.1.9/emodelrunner/protocols/synplas_protocols.py`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.8/emodelrunner/protocols/thalamus_protocols.py` & `EModelRunner-1.1.9/emodelrunner/protocols/thalamus_protocols.py`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.8/emodelrunner/recordings.py` & `EModelRunner-1.1.9/emodelrunner/recordings.py`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.8/emodelrunner/run.py` & `EModelRunner-1.1.9/emodelrunner/run.py`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.8/emodelrunner/run_pairsim.py` & `EModelRunner-1.1.9/emodelrunner/run_pairsim.py`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.8/emodelrunner/run_synplas.py` & `EModelRunner-1.1.9/emodelrunner/run_synplas.py`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.8/emodelrunner/stimuli.py` & `EModelRunner-1.1.9/emodelrunner/stimuli.py`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.8/emodelrunner/synapses/__init__.py` & `EModelRunner-1.1.9/emodelrunner/synapses/__init__.py`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.8/emodelrunner/synapses/create_locations.py` & `EModelRunner-1.1.9/emodelrunner/synapses/create_locations.py`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.8/emodelrunner/synapses/glusynapse.py` & `EModelRunner-1.1.9/emodelrunner/synapses/glusynapse.py`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.8/emodelrunner/synapses/mechanism.py` & `EModelRunner-1.1.9/emodelrunner/synapses/mechanism.py`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.8/emodelrunner/synapses/minis.py` & `EModelRunner-1.1.9/emodelrunner/synapses/minis.py`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.8/emodelrunner/synapses/recordings.py` & `EModelRunner-1.1.9/emodelrunner/synapses/recordings.py`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.8/emodelrunner/synapses/stimuli.py` & `EModelRunner-1.1.9/emodelrunner/synapses/stimuli.py`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.8/emodelrunner/synapses/synapse.py` & `EModelRunner-1.1.9/emodelrunner/synapses/synapse.py`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.8/emodelrunner/synplas_analysis.py` & `EModelRunner-1.1.9/emodelrunner/synplas_analysis.py`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.8/examples/sscx_sample_dir/LICENSE.txt` & `EModelRunner-1.1.9/examples/sscx_sample_dir/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.8/examples/sscx_sample_dir/LICENSE_CC-BY-CA-SA-4.0` & `EModelRunner-1.1.9/examples/sscx_sample_dir/LICENSE_CC-BY-CA-SA-4.0`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.8/examples/sscx_sample_dir/config/config_allsteps.ini` & `EModelRunner-1.1.9/examples/sscx_sample_dir/config/config_synapses_short.ini`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 [Package]
 type = sscx
 
 [Synapses]
-add_synapses = False
+add_synapses = True
 seed = 846515
 rng_settings_mode = Random123
 hoc_synapse_template_name = hoc_synapses
 
 [Paths]
-prot_path = config/protocols/allsteps.json
+prot_path = config/protocols/synapses_short.json
 features_path = config/features/cADpyr_L4PC.json
 unoptimized_params_path = config/params/pyr.json
 memodel_dir = .
 output_dir = %(memodel_dir)s/python_recordings
 params_path = %(memodel_dir)s/config/params/final.json
-units_path = %(memodel_dir)s/config/features/units.json
 templates_dir = %(memodel_dir)s/templates
 cell_template_path = %(templates_dir)s/cell_template_neurodamus.jinja2
 run_hoc_template_path = %(templates_dir)s/run_hoc.jinja2
 createsimulation_template_path = %(templates_dir)s/createsimulation.jinja2
 synapses_template_path = %(templates_dir)s/synapses.jinja2
 replace_axon_hoc_path = %(templates_dir)s/replace_axon_hoc.hoc
 syn_dir_for_hoc = %(memodel_dir)s/synapses
```

### Comparing `EModelRunner-1.1.8/examples/sscx_sample_dir/config/config_factsheets.ini` & `EModelRunner-1.1.9/examples/sscx_sample_dir/config/config_factsheets.ini`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 [Paths]
 prot_path = config/protocols/RmpRiTau.json
 features_path = config/features/cADpyr_L4PC.json
 unoptimized_params_path = config/params/pyr.json
 memodel_dir = .
 output_dir = %(memodel_dir)s/python_recordings
 params_path = %(memodel_dir)s/config/params/final.json
-units_path = %(memodel_dir)s/config/features/units.json
 templates_dir = %(memodel_dir)s/templates
 cell_template_path = %(templates_dir)s/cell_template_neurodamus.jinja2
 run_hoc_template_path = %(templates_dir)s/run_hoc.jinja2
 createsimulation_template_path = %(templates_dir)s/createsimulation.jinja2
 synapses_template_path = %(templates_dir)s/synapses.jinja2
 replace_axon_hoc_path = %(templates_dir)s/replace_axon_hoc.hoc
 syn_dir_for_hoc = %(memodel_dir)s/synapses
```

### Comparing `EModelRunner-1.1.8/examples/sscx_sample_dir/config/config_multiprotocols.ini` & `EModelRunner-1.1.9/examples/sscx_sample_dir/config/config_allsteps.ini`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 [Package]
 type = sscx
 
 [Synapses]
-add_synapses = True
+add_synapses = False
 seed = 846515
 rng_settings_mode = Random123
 hoc_synapse_template_name = hoc_synapses
 
 [Paths]
-prot_path = config/protocols/multiprotocols.json
+prot_path = config/protocols/allsteps.json
 features_path = config/features/cADpyr_L4PC.json
 unoptimized_params_path = config/params/pyr.json
 memodel_dir = .
 output_dir = %(memodel_dir)s/python_recordings
 params_path = %(memodel_dir)s/config/params/final.json
-units_path = %(memodel_dir)s/config/features/units.json
 templates_dir = %(memodel_dir)s/templates
 cell_template_path = %(templates_dir)s/cell_template_neurodamus.jinja2
 run_hoc_template_path = %(templates_dir)s/run_hoc.jinja2
 createsimulation_template_path = %(templates_dir)s/createsimulation.jinja2
 synapses_template_path = %(templates_dir)s/synapses.jinja2
 replace_axon_hoc_path = %(templates_dir)s/replace_axon_hoc.hoc
 syn_dir_for_hoc = %(memodel_dir)s/synapses
@@ -44,7 +43,8 @@
 
 [Sim]
 dt = 0.025
 cvode_active = False
 
 [Protocol]
 apical_point_isec = 22
+
```

### Comparing `EModelRunner-1.1.8/examples/sscx_sample_dir/config/config_recipe_protocols.ini` & `EModelRunner-1.1.9/examples/sscx_sample_dir/config/config_singlestep.ini`

 * *Files 4% similar despite different names*

```diff
@@ -4,21 +4,20 @@
 [Synapses]
 add_synapses = False
 seed = 846515
 rng_settings_mode = Random123
 hoc_synapse_template_name = hoc_synapses
 
 [Paths]
+prot_path = config/protocols/singlestep.json
 features_path = config/features/cADpyr_L4PC.json
 unoptimized_params_path = config/params/pyr.json
-prot_path = config/protocols/cADpyr_L4PC.json
 memodel_dir = .
 output_dir = %(memodel_dir)s/python_recordings
 params_path = %(memodel_dir)s/config/params/final.json
-units_path = %(memodel_dir)s/config/features/units.json
 templates_dir = %(memodel_dir)s/templates
 cell_template_path = %(templates_dir)s/cell_template_neurodamus.jinja2
 run_hoc_template_path = %(templates_dir)s/run_hoc.jinja2
 createsimulation_template_path = %(templates_dir)s/createsimulation.jinja2
 synapses_template_path = %(templates_dir)s/synapses.jinja2
 replace_axon_hoc_path = %(templates_dir)s/replace_axon_hoc.hoc
 syn_dir_for_hoc = %(memodel_dir)s/synapses
```

### Comparing `EModelRunner-1.1.8/examples/sscx_sample_dir/config/config_singlestep.ini` & `EModelRunner-1.1.9/examples/sscx_sample_dir/config/config_synapses.ini`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 [Package]
 type = sscx
 
 [Synapses]
-add_synapses = False
+add_synapses = True
 seed = 846515
 rng_settings_mode = Random123
 hoc_synapse_template_name = hoc_synapses
 
 [Paths]
-prot_path = config/protocols/singlestep.json
+prot_path = config/protocols/synapses.json
 features_path = config/features/cADpyr_L4PC.json
 unoptimized_params_path = config/params/pyr.json
 memodel_dir = .
 output_dir = %(memodel_dir)s/python_recordings
 params_path = %(memodel_dir)s/config/params/final.json
-units_path = %(memodel_dir)s/config/features/units.json
 templates_dir = %(memodel_dir)s/templates
 cell_template_path = %(templates_dir)s/cell_template_neurodamus.jinja2
 run_hoc_template_path = %(templates_dir)s/run_hoc.jinja2
 createsimulation_template_path = %(templates_dir)s/createsimulation.jinja2
 synapses_template_path = %(templates_dir)s/synapses.jinja2
 replace_axon_hoc_path = %(templates_dir)s/replace_axon_hoc.hoc
 syn_dir_for_hoc = %(memodel_dir)s/synapses
```

### Comparing `EModelRunner-1.1.8/examples/sscx_sample_dir/config/config_synapses.ini` & `EModelRunner-1.1.9/examples/sscx_sample_dir/config/config_multiprotocols.ini`

 * *Files 6% similar despite different names*

```diff
@@ -4,21 +4,20 @@
 [Synapses]
 add_synapses = True
 seed = 846515
 rng_settings_mode = Random123
 hoc_synapse_template_name = hoc_synapses
 
 [Paths]
-prot_path = config/protocols/synapses.json
+prot_path = config/protocols/multiprotocols.json
 features_path = config/features/cADpyr_L4PC.json
 unoptimized_params_path = config/params/pyr.json
 memodel_dir = .
 output_dir = %(memodel_dir)s/python_recordings
 params_path = %(memodel_dir)s/config/params/final.json
-units_path = %(memodel_dir)s/config/features/units.json
 templates_dir = %(memodel_dir)s/templates
 cell_template_path = %(templates_dir)s/cell_template_neurodamus.jinja2
 run_hoc_template_path = %(templates_dir)s/run_hoc.jinja2
 createsimulation_template_path = %(templates_dir)s/createsimulation.jinja2
 synapses_template_path = %(templates_dir)s/synapses.jinja2
 replace_axon_hoc_path = %(templates_dir)s/replace_axon_hoc.hoc
 syn_dir_for_hoc = %(memodel_dir)s/synapses
@@ -44,8 +43,7 @@
 
 [Sim]
 dt = 0.025
 cvode_active = False
 
 [Protocol]
 apical_point_isec = 22
-
```

### Comparing `EModelRunner-1.1.8/examples/sscx_sample_dir/config/config_synapses_short.ini` & `EModelRunner-1.1.9/examples/sscx_sample_dir/config/config_recipe_protocols.ini`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 [Package]
 type = sscx
 
 [Synapses]
-add_synapses = True
+add_synapses = False
 seed = 846515
 rng_settings_mode = Random123
 hoc_synapse_template_name = hoc_synapses
 
 [Paths]
-prot_path = config/protocols/synapses_short.json
 features_path = config/features/cADpyr_L4PC.json
 unoptimized_params_path = config/params/pyr.json
+prot_path = config/protocols/cADpyr_L4PC.json
 memodel_dir = .
 output_dir = %(memodel_dir)s/python_recordings
 params_path = %(memodel_dir)s/config/params/final.json
-units_path = %(memodel_dir)s/config/features/units.json
 templates_dir = %(memodel_dir)s/templates
 cell_template_path = %(templates_dir)s/cell_template_neurodamus.jinja2
 run_hoc_template_path = %(templates_dir)s/run_hoc.jinja2
 createsimulation_template_path = %(templates_dir)s/createsimulation.jinja2
 synapses_template_path = %(templates_dir)s/synapses.jinja2
 replace_axon_hoc_path = %(templates_dir)s/replace_axon_hoc.hoc
 syn_dir_for_hoc = %(memodel_dir)s/synapses
```

### Comparing `EModelRunner-1.1.8/examples/sscx_sample_dir/config/features/cADpyr_L4PC.json` & `EModelRunner-1.1.9/examples/sscx_sample_dir/config/features/cADpyr_L4PC.json`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.8/examples/sscx_sample_dir/config/params/final.json` & `EModelRunner-1.1.9/examples/sscx_sample_dir/config/params/final.json`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.8/examples/sscx_sample_dir/config/params/pyr.json` & `EModelRunner-1.1.9/examples/sscx_sample_dir/config/params/pyr.json`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.8/examples/sscx_sample_dir/config/protocols/allsteps.json` & `EModelRunner-1.1.9/examples/sscx_sample_dir/config/protocols/allsteps.json`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.8/examples/sscx_sample_dir/config/protocols/cADpyr_L4PC.json` & `EModelRunner-1.1.9/examples/sscx_sample_dir/config/protocols/cADpyr_L4PC.json`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.8/examples/sscx_sample_dir/config/protocols/multiprotocols.json` & `EModelRunner-1.1.9/examples/sscx_sample_dir/config/protocols/multiprotocols.json`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.8/examples/sscx_sample_dir/mechanisms/CaDynamics_DC0.mod` & `EModelRunner-1.1.9/examples/sscx_sample_dir/mechanisms/CaDynamics_DC0.mod`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.8/examples/sscx_sample_dir/mechanisms/Ca_HVA2.mod` & `EModelRunner-1.1.9/examples/sscx_sample_dir/mechanisms/Ca_HVA2.mod`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.8/examples/sscx_sample_dir/mechanisms/Ca_LVAst.mod` & `EModelRunner-1.1.9/examples/sscx_sample_dir/mechanisms/Ca_LVAst.mod`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.8/examples/sscx_sample_dir/mechanisms/Ih.mod` & `EModelRunner-1.1.9/examples/sscx_sample_dir/mechanisms/Ih.mod`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.8/examples/sscx_sample_dir/mechanisms/K_Pst.mod` & `EModelRunner-1.1.9/examples/sscx_sample_dir/mechanisms/K_Pst.mod`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.8/examples/sscx_sample_dir/mechanisms/K_Tst.mod` & `EModelRunner-1.1.9/examples/sscx_sample_dir/mechanisms/K_Tst.mod`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.8/examples/sscx_sample_dir/mechanisms/KdShu2007.mod` & `EModelRunner-1.1.9/examples/sscx_sample_dir/mechanisms/KdShu2007.mod`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.8/examples/sscx_sample_dir/mechanisms/NaTg.mod` & `EModelRunner-1.1.9/examples/sscx_sample_dir/mechanisms/NaTg.mod`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.8/examples/sscx_sample_dir/mechanisms/Nap_Et2.mod` & `EModelRunner-1.1.9/examples/sscx_sample_dir/mechanisms/Nap_Et2.mod`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.8/examples/sscx_sample_dir/mechanisms/ProbAMPANMDA_EMS.mod` & `EModelRunner-1.1.9/examples/sscx_sample_dir/mechanisms/ProbAMPANMDA_EMS.mod`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.8/examples/sscx_sample_dir/mechanisms/ProbGABAAB_EMS.mod` & `EModelRunner-1.1.9/examples/sscx_sample_dir/mechanisms/ProbGABAAB_EMS.mod`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.8/examples/sscx_sample_dir/mechanisms/SK_E2.mod` & `EModelRunner-1.1.9/examples/sscx_sample_dir/mechanisms/SK_E2.mod`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.8/examples/sscx_sample_dir/mechanisms/SKv3_1.mod` & `EModelRunner-1.1.9/examples/sscx_sample_dir/mechanisms/SKv3_1.mod`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.8/examples/sscx_sample_dir/mechanisms/StochKv3.mod` & `EModelRunner-1.1.9/examples/sscx_sample_dir/mechanisms/StochKv3.mod`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.8/examples/sscx_sample_dir/mechanisms/VecStim.mod` & `EModelRunner-1.1.9/examples/sscx_sample_dir/mechanisms/VecStim.mod`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.8/examples/sscx_sample_dir/mechanisms/notes.txt` & `EModelRunner-1.1.9/examples/sscx_sample_dir/mechanisms/notes.txt`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.8/examples/sscx_sample_dir/morphology/dend-C231296A-P4B2_axon-C200897C-P2_-_Scale_x1.000_y0.975_z1.000.asc` & `EModelRunner-1.1.9/examples/sscx_sample_dir/morphology/dend-C231296A-P4B2_axon-C200897C-P2_-_Scale_x1.000_y0.975_z1.000.asc`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.8/examples/sscx_sample_dir/synapses/synapses.tsv` & `EModelRunner-1.1.9/examples/sscx_sample_dir/synapses/synapses.tsv`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.8/examples/sscx_sample_dir/templates/cell_template_neurodamus.jinja2` & `EModelRunner-1.1.9/examples/sscx_sample_dir/templates/cell_template_neurodamus.jinja2`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.8/examples/sscx_sample_dir/templates/createsimulation.jinja2` & `EModelRunner-1.1.9/examples/sscx_sample_dir/templates/createsimulation.jinja2`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.8/examples/sscx_sample_dir/templates/features.hoc` & `EModelRunner-1.1.9/examples/sscx_sample_dir/templates/features.hoc`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.8/examples/sscx_sample_dir/templates/main_protocol.jinja2` & `EModelRunner-1.1.9/examples/sscx_sample_dir/templates/main_protocol.jinja2`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.8/examples/sscx_sample_dir/templates/replace_axon_hoc.hoc` & `EModelRunner-1.1.9/examples/sscx_sample_dir/templates/replace_axon_hoc.hoc`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.8/examples/sscx_sample_dir/templates/run_hoc.jinja2` & `EModelRunner-1.1.9/examples/sscx_sample_dir/templates/run_hoc.jinja2`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.8/examples/sscx_sample_dir/templates/synapses.jinja2` & `EModelRunner-1.1.9/examples/sscx_sample_dir/templates/synapses.jinja2`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.8/examples/synplas_sample_dir/LICENSE.txt` & `EModelRunner-1.1.9/examples/synplas_sample_dir/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.8/examples/synplas_sample_dir/LICENSE_CC-BY-CA-SA-4.0` & `EModelRunner-1.1.9/examples/synplas_sample_dir/LICENSE_CC-BY-CA-SA-4.0`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.8/examples/synplas_sample_dir/config/config_1Hz_10ms.ini` & `EModelRunner-1.1.9/examples/synplas_sample_dir/config/config_1Hz_10ms.ini`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.8/examples/synplas_sample_dir/config/params/final.json` & `EModelRunner-1.1.9/examples/synplas_sample_dir/config/params/final.json`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.8/examples/synplas_sample_dir/config/params/pyr.json` & `EModelRunner-1.1.9/examples/synplas_sample_dir/config/params/pyr.json`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.8/examples/synplas_sample_dir/mechanisms/CaDynamics_DC0.mod` & `EModelRunner-1.1.9/examples/synplas_sample_dir/mechanisms/CaDynamics_DC0.mod`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.8/examples/synplas_sample_dir/mechanisms/Ca_HVA2.mod` & `EModelRunner-1.1.9/examples/synplas_sample_dir/mechanisms/Ca_HVA2.mod`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.8/examples/synplas_sample_dir/mechanisms/Ca_LVAst.mod` & `EModelRunner-1.1.9/examples/synplas_sample_dir/mechanisms/Ca_LVAst.mod`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.8/examples/synplas_sample_dir/mechanisms/DetAMPANMDA.mod` & `EModelRunner-1.1.9/examples/synplas_sample_dir/mechanisms/DetAMPANMDA.mod`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.8/examples/synplas_sample_dir/mechanisms/DetGABAAB.mod` & `EModelRunner-1.1.9/examples/synplas_sample_dir/mechanisms/DetGABAAB.mod`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.8/examples/synplas_sample_dir/mechanisms/GluSynapse.mod` & `EModelRunner-1.1.9/examples/synplas_sample_dir/mechanisms/GluSynapse.mod`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.8/examples/synplas_sample_dir/mechanisms/Ih.mod` & `EModelRunner-1.1.9/examples/synplas_sample_dir/mechanisms/Ih.mod`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.8/examples/synplas_sample_dir/mechanisms/K_Pst.mod` & `EModelRunner-1.1.9/examples/synplas_sample_dir/mechanisms/K_Pst.mod`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.8/examples/synplas_sample_dir/mechanisms/K_Tst.mod` & `EModelRunner-1.1.9/examples/synplas_sample_dir/mechanisms/K_Tst.mod`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.8/examples/synplas_sample_dir/mechanisms/KdShu2007.mod` & `EModelRunner-1.1.9/examples/synplas_sample_dir/mechanisms/KdShu2007.mod`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.8/examples/synplas_sample_dir/mechanisms/NaTg.mod` & `EModelRunner-1.1.9/examples/synplas_sample_dir/mechanisms/NaTg.mod`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.8/examples/synplas_sample_dir/mechanisms/Nap_Et2.mod` & `EModelRunner-1.1.9/examples/synplas_sample_dir/mechanisms/Nap_Et2.mod`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.8/examples/synplas_sample_dir/mechanisms/ProbAMPANMDA_EMS.mod` & `EModelRunner-1.1.9/examples/synplas_sample_dir/mechanisms/ProbAMPANMDA_EMS.mod`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.8/examples/synplas_sample_dir/mechanisms/ProbGABAAB_EMS.mod` & `EModelRunner-1.1.9/examples/synplas_sample_dir/mechanisms/ProbGABAAB_EMS.mod`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.8/examples/synplas_sample_dir/mechanisms/SK_E2.mod` & `EModelRunner-1.1.9/examples/synplas_sample_dir/mechanisms/SK_E2.mod`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.8/examples/synplas_sample_dir/mechanisms/SKv3_1.mod` & `EModelRunner-1.1.9/examples/synplas_sample_dir/mechanisms/SKv3_1.mod`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.8/examples/synplas_sample_dir/mechanisms/StochKv3.mod` & `EModelRunner-1.1.9/examples/synplas_sample_dir/mechanisms/StochKv3.mod`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.8/examples/synplas_sample_dir/mechanisms/TTXDynamicsSwitch.mod` & `EModelRunner-1.1.9/examples/synplas_sample_dir/mechanisms/TTXDynamicsSwitch.mod`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.8/examples/synplas_sample_dir/mechanisms/VecStim.mod` & `EModelRunner-1.1.9/examples/synplas_sample_dir/mechanisms/VecStim.mod`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.8/examples/synplas_sample_dir/mechanisms/netstim_inhpoisson.mod` & `EModelRunner-1.1.9/examples/synplas_sample_dir/mechanisms/netstim_inhpoisson.mod`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.8/examples/synplas_sample_dir/mechanisms/optimized/ProbAMPANMDA_EMS.mod` & `EModelRunner-1.1.9/examples/synplas_sample_dir/mechanisms/optimized/ProbAMPANMDA_EMS.mod`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.8/examples/synplas_sample_dir/mechanisms/optimized/ProbGABAAB_EMS.mod` & `EModelRunner-1.1.9/examples/synplas_sample_dir/mechanisms/optimized/ProbGABAAB_EMS.mod`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.8/examples/synplas_sample_dir/morphology/dend-C120398A-P3_axon-sm100429a1-5_INT_idG_-_Scale_x1.000_y0.975_z1.000.asc` & `EModelRunner-1.1.9/examples/synplas_sample_dir/morphology/dend-C120398A-P3_axon-sm100429a1-5_INT_idG_-_Scale_x1.000_y0.975_z1.000.asc`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.8/examples/synplas_sample_dir/morphology/dend-sm100429a1-5_INT_idG_axon-sm100429a1-5_INT_idE_-_Scale_x1.000_y0.950_z1.000_-_Clone_0.asc` & `EModelRunner-1.1.9/examples/synplas_sample_dir/morphology/dend-sm100429a1-5_INT_idG_axon-sm100429a1-5_INT_idE_-_Scale_x1.000_y0.950_z1.000_-_Clone_0.asc`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.8/examples/synplas_sample_dir/protocols/spiketrain_1Hz_10ms.dat` & `EModelRunner-1.1.9/examples/synplas_sample_dir/protocols/spiketrain_1Hz_10ms.dat`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.8/examples/synplas_sample_dir/protocols/stimuli_1Hz.json` & `EModelRunner-1.1.9/examples/synplas_sample_dir/protocols/stimuli_1Hz.json`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.8/examples/synplas_sample_dir/synapses/syn_extra_params.json` & `EModelRunner-1.1.9/examples/synplas_sample_dir/synapses/syn_extra_params.json`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.8/examples/synplas_sample_dir/synapses/synapse_properties.json` & `EModelRunner-1.1.9/examples/synplas_sample_dir/synapses/synapse_properties.json`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.8/examples/thalamus_sample_dir/LICENSE.txt` & `EModelRunner-1.1.9/examples/thalamus_sample_dir/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.8/examples/thalamus_sample_dir/LICENSE_CC-BY-CA-SA-4.0` & `EModelRunner-1.1.9/examples/thalamus_sample_dir/LICENSE_CC-BY-CA-SA-4.0`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.8/examples/thalamus_sample_dir/config/config_recipe_prots_short.ini` & `EModelRunner-1.1.9/examples/thalamus_sample_dir/config/config_recipe_prots_short.ini`

 * *Files 9% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 [Paths]
 prot_path = config/protocols/dNAD_ltb_short.json
 features_path = config/features/dNAD_ltb.json
 unoptimized_params_path = config/params/bAC_TC_VPL.json
 memodel_dir = .
 output_dir = %(memodel_dir)s/python_recordings
 params_path = %(memodel_dir)s/config/params/final.json
-units_path = %(memodel_dir)s/config/features/units.json
 syn_dir = %(memodel_dir)s/synapses
 syn_data_file = synapses.tsv
 syn_conf_file = synconf.txt
 syn_mtype_map = mtype_map.tsv
 morph_path = morphology/dend-jy180118_C_idD_axon-AA0318_-_Scale_x1.000_y1.050_z1.000.asc
 
 [Morphology]
```

### Comparing `EModelRunner-1.1.8/examples/thalamus_sample_dir/config/features/dNAD_ltb.json` & `EModelRunner-1.1.9/examples/thalamus_sample_dir/config/features/dNAD_ltb.json`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.8/examples/thalamus_sample_dir/config/params/bAC_TC_VPL.json` & `EModelRunner-1.1.9/examples/thalamus_sample_dir/config/params/bAC_TC_VPL.json`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.8/examples/thalamus_sample_dir/config/params/final.json` & `EModelRunner-1.1.9/examples/thalamus_sample_dir/config/params/final.json`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.8/examples/thalamus_sample_dir/config/protocols/dNAD_ltb_short.json` & `EModelRunner-1.1.9/examples/thalamus_sample_dir/config/protocols/dNAD_ltb_short.json`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/CaDynamics_DC0.mod` & `EModelRunner-1.1.9/examples/thalamus_sample_dir/mechanisms/CaDynamics_DC0.mod`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/Ca_HVA.mod` & `EModelRunner-1.1.9/examples/thalamus_sample_dir/mechanisms/Ca_HVA.mod`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/Ca_HVA2.mod` & `EModelRunner-1.1.9/examples/thalamus_sample_dir/mechanisms/Ca_HVA2.mod`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/Ca_LVAst.mod` & `EModelRunner-1.1.9/examples/thalamus_sample_dir/mechanisms/Ca_LVAst.mod`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/Ih.mod` & `EModelRunner-1.1.9/examples/thalamus_sample_dir/mechanisms/Ih.mod`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/K_Pst.mod` & `EModelRunner-1.1.9/examples/thalamus_sample_dir/mechanisms/K_Pst.mod`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/K_Tst.mod` & `EModelRunner-1.1.9/examples/thalamus_sample_dir/mechanisms/K_Tst.mod`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/KdShu2007.mod` & `EModelRunner-1.1.9/examples/thalamus_sample_dir/mechanisms/KdShu2007.mod`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/NaTg.mod` & `EModelRunner-1.1.9/examples/thalamus_sample_dir/mechanisms/NaTg.mod`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/Nap_Et2.mod` & `EModelRunner-1.1.9/examples/thalamus_sample_dir/mechanisms/Nap_Et2.mod`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/SK_E2.mod` & `EModelRunner-1.1.9/examples/thalamus_sample_dir/mechanisms/SK_E2.mod`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/SKv3_1.mod` & `EModelRunner-1.1.9/examples/thalamus_sample_dir/mechanisms/SKv3_1.mod`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/StochKv3.mod` & `EModelRunner-1.1.9/examples/thalamus_sample_dir/mechanisms/StochKv3.mod`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/TC_HH.mod` & `EModelRunner-1.1.9/examples/thalamus_sample_dir/mechanisms/TC_HH.mod`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/TC_ITGHK.mod` & `EModelRunner-1.1.9/examples/thalamus_sample_dir/mechanisms/TC_ITGHK.mod`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/TC_ITGHK_Ama14.mod` & `EModelRunner-1.1.9/examples/thalamus_sample_dir/mechanisms/TC_ITGHK_Ama14.mod`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/TC_ITGHK_Des98.mod` & `EModelRunner-1.1.9/examples/thalamus_sample_dir/mechanisms/TC_ITGHK_Des98.mod`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/TC_Ih.mod` & `EModelRunner-1.1.9/examples/thalamus_sample_dir/mechanisms/TC_Ih.mod`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/TC_Ih_Bud97.mod` & `EModelRunner-1.1.9/examples/thalamus_sample_dir/mechanisms/TC_Ih_Bud97.mod`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/TC_KCa_bk.mod` & `EModelRunner-1.1.9/examples/thalamus_sample_dir/mechanisms/TC_KCa_bk.mod`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/TC_Kir2_2.mod` & `EModelRunner-1.1.9/examples/thalamus_sample_dir/mechanisms/TC_Kir2_2.mod`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/TC_NaP.mod` & `EModelRunner-1.1.9/examples/thalamus_sample_dir/mechanisms/TC_NaP.mod`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/TC_Nap_Et2.mod` & `EModelRunner-1.1.9/examples/thalamus_sample_dir/mechanisms/TC_Nap_Et2.mod`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/TC_cadecay.mod` & `EModelRunner-1.1.9/examples/thalamus_sample_dir/mechanisms/TC_cadecay.mod`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/TC_iA.mod` & `EModelRunner-1.1.9/examples/thalamus_sample_dir/mechanisms/TC_iA.mod`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/TC_iA_old.mod` & `EModelRunner-1.1.9/examples/thalamus_sample_dir/mechanisms/TC_iA_old.mod`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/TC_iL.mod` & `EModelRunner-1.1.9/examples/thalamus_sample_dir/mechanisms/TC_iL.mod`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/TC_ic.mod` & `EModelRunner-1.1.9/examples/thalamus_sample_dir/mechanisms/TC_ic.mod`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/TC_ih2.mod` & `EModelRunner-1.1.9/examples/thalamus_sample_dir/mechanisms/TC_ih2.mod`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/TC_kahp.mod` & `EModelRunner-1.1.9/examples/thalamus_sample_dir/mechanisms/TC_kahp.mod`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/TC_kir_Con15.mod` & `EModelRunner-1.1.9/examples/thalamus_sample_dir/mechanisms/TC_kir_Con15.mod`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/ican.mod` & `EModelRunner-1.1.9/examples/thalamus_sample_dir/mechanisms/ican.mod`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/other_versions/IKCa.mod` & `EModelRunner-1.1.9/examples/thalamus_sample_dir/mechanisms/other_versions/IKCa.mod`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/other_versions/NaTg.mod` & `EModelRunner-1.1.9/examples/thalamus_sample_dir/mechanisms/other_versions/NaTg.mod`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/other_versions/Nap_Et2.mod` & `EModelRunner-1.1.9/examples/thalamus_sample_dir/mechanisms/other_versions/Nap_Et2.mod`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/other_versions/TC_ITGHK.mod` & `EModelRunner-1.1.9/examples/thalamus_sample_dir/mechanisms/other_versions/TC_ITGHK.mod`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/other_versions/TC_ITGHK_Ama14.mod` & `EModelRunner-1.1.9/examples/thalamus_sample_dir/mechanisms/other_versions/TC_ITGHK_Ama14.mod`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/other_versions/TC_ITGHK_Wei2011.mod` & `EModelRunner-1.1.9/examples/thalamus_sample_dir/mechanisms/other_versions/TC_ITGHK_Wei2011.mod`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/other_versions/TC_Ih.mod` & `EModelRunner-1.1.9/examples/thalamus_sample_dir/mechanisms/other_versions/TC_Ih.mod`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/other_versions/TC_KCa_bk.mod` & `EModelRunner-1.1.9/examples/thalamus_sample_dir/mechanisms/other_versions/TC_KCa_bk.mod`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/other_versions/TC_Kir2_2.mod` & `EModelRunner-1.1.9/examples/thalamus_sample_dir/mechanisms/other_versions/TC_Kir2_2.mod`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/other_versions/TC_NaP.mod` & `EModelRunner-1.1.9/examples/thalamus_sample_dir/mechanisms/other_versions/TC_NaP.mod`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/other_versions/TC_iA_old.mod` & `EModelRunner-1.1.9/examples/thalamus_sample_dir/mechanisms/other_versions/TC_iA_old.mod`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/other_versions/TC_ic.mod` & `EModelRunner-1.1.9/examples/thalamus_sample_dir/mechanisms/other_versions/TC_ic.mod`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/other_versions/TC_ih2.mod` & `EModelRunner-1.1.9/examples/thalamus_sample_dir/mechanisms/other_versions/TC_ih2.mod`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/other_versions/TC_kahp.mod` & `EModelRunner-1.1.9/examples/thalamus_sample_dir/mechanisms/other_versions/TC_kahp.mod`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.8/examples/thalamus_sample_dir/mechanisms/other_versions/caidL.mod` & `EModelRunner-1.1.9/examples/thalamus_sample_dir/mechanisms/other_versions/caidL.mod`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.8/examples/thalamus_sample_dir/morphology/dend-jy180118_C_idD_axon-AA0318_-_Scale_x1.000_y1.050_z1.000.asc` & `EModelRunner-1.1.9/examples/thalamus_sample_dir/morphology/dend-jy180118_C_idD_axon-AA0318_-_Scale_x1.000_y1.050_z1.000.asc`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.8/requirements_docs.txt` & `EModelRunner-1.1.9/requirements_docs.txt`

 * *Files identical despite different names*

### Comparing `EModelRunner-1.1.8/setup.py` & `EModelRunner-1.1.9/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -39,14 +39,15 @@
         "Tracker": "https://github.com/BlueBrain/EModelRunner/issues",
         "Source": "https://github.com/BlueBrain/EModelRunner",
         "Documentation": "https://emodelrunner.readthedocs.io/en/latest",
     },
     license="Apache 2.0",
     install_requires=[
         "numpy",
+        "efel>=4.2,<5",
         "bluepyopt>=1.13.168",
         "neurom>=3.1.0",
         "h5py",
         "matplotlib",
         "schema",
         "Pebble>=4.3.10",
         "importlib_metadata; python_version<'3.8'",
```

### Comparing `EModelRunner-1.1.8/tox.ini` & `EModelRunner-1.1.9/tox.ini`

 * *Files 5% similar despite different names*

```diff
@@ -32,15 +32,16 @@
 deps = 
     {[base]testdeps}
     coverage
     pytest-cov
     pytest-xdist
     filelock
     hypothesis
-passenv = KRB5CCNAME, DISPLAY, https_proxy, USER
+setenv =
+    NEURON_MODULE_OPTIONS='-nogui'
 allowlist_externals =
     make
     ./.compile_mod.sh
 coverage_options = --cov-append --cov-report=xml --cov-config=.coveragerc
 dist-options = -n 13 --dist loadgroup
 commands =
     make clean
```

