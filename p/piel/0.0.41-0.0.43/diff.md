# Comparing `tmp/piel-0.0.41.tar.gz` & `tmp/piel-0.0.43.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "piel-0.0.41.tar", last modified: Sat Jul  8 15:26:00 2023, max compression
+gzip compressed data, was "piel-0.0.43.tar", last modified: Thu Jul 13 21:52:33 2023, max compression
```

## Comparing `piel-0.0.41.tar` & `piel-0.0.43.tar`

### file list

```diff
@@ -1,338 +1,386 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.151372 piel-0.0.41/
--rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-07-08 15:25:43.000000 piel-0.0.41/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-08 15:25:43.000000 piel-0.0.41/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-07-08 15:25:43.000000 piel-0.0.41/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3707 2023-07-08 15:26:00.151372 piel-0.0.41/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2882 2023-07-08 15:25:43.000000 piel-0.0.41/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.127372 piel-0.0.41/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-07-08 15:25:43.000000 piel-0.0.41/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.127372 piel-0.0.41/docs/autoapi/
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-08 15:25:43.000000 piel-0.0.41/docs/autoapi/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.127372 piel-0.0.41/docs/autoapi/piel/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.127372 piel-0.0.41/docs/autoapi/piel/cli/
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-08 15:25:43.000000 piel-0.0.41/docs/autoapi/piel/cli/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.127372 piel-0.0.41/docs/autoapi/piel/components/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-08 15:25:43.000000 piel-0.0.41/docs/autoapi/piel/components/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.127372 piel-0.0.41/docs/autoapi/piel/config/
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-08 15:25:43.000000 piel-0.0.41/docs/autoapi/piel/config/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.127372 piel-0.0.41/docs/autoapi/piel/defaults/
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-07-08 15:25:43.000000 piel-0.0.41/docs/autoapi/piel/defaults/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.127372 piel-0.0.41/docs/autoapi/piel/file_conversion/
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-07-08 15:25:43.000000 piel-0.0.41/docs/autoapi/piel/file_conversion/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.127372 piel-0.0.41/docs/autoapi/piel/file_system/
--rw-r--r--   0 runner    (1001) docker     (123)     5453 2023-07-08 15:25:43.000000 piel-0.0.41/docs/autoapi/piel/file_system/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)    39344 2023-07-08 15:25:43.000000 piel-0.0.41/docs/autoapi/piel/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.127372 piel-0.0.41/docs/autoapi/piel/integration/
--rw-r--r--   0 runner    (1001) docker     (123)     4394 2023-07-08 15:25:43.000000 piel-0.0.41/docs/autoapi/piel/integration/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.127372 piel-0.0.41/docs/autoapi/piel/integration/openlane_gdsfactory_core/
--rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-07-08 15:25:43.000000 piel-0.0.41/docs/autoapi/piel/integration/openlane_gdsfactory_core/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.127372 piel-0.0.41/docs/autoapi/piel/integration/sax_cocotb/
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-08 15:25:43.000000 piel-0.0.41/docs/autoapi/piel/integration/sax_cocotb/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.127372 piel-0.0.41/docs/autoapi/piel/integration/sax_qutip/
--rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-07-08 15:25:43.000000 piel-0.0.41/docs/autoapi/piel/integration/sax_qutip/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.127372 piel-0.0.41/docs/autoapi/piel/models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.127372 piel-0.0.41/docs/autoapi/piel/models/frequency/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.127372 piel-0.0.41/docs/autoapi/piel/models/frequency/all/
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-07-08 15:25:43.000000 piel-0.0.41/docs/autoapi/piel/models/frequency/all/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.127372 piel-0.0.41/docs/autoapi/piel/models/frequency/defaults/
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-07-08 15:25:43.000000 piel-0.0.41/docs/autoapi/piel/models/frequency/defaults/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.127372 piel-0.0.41/docs/autoapi/piel/models/frequency/electrical/
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-08 15:25:43.000000 piel-0.0.41/docs/autoapi/piel/models/frequency/electrical/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.131372 piel-0.0.41/docs/autoapi/piel/models/frequency/electro_optic/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.131372 piel-0.0.41/docs/autoapi/piel/models/frequency/electro_optic/ideal/
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-08 15:25:43.000000 piel-0.0.41/docs/autoapi/piel/models/frequency/electro_optic/ideal/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-08 15:25:43.000000 piel-0.0.41/docs/autoapi/piel/models/frequency/electro_optic/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.131372 piel-0.0.41/docs/autoapi/piel/models/frequency/electronic/
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-08 15:25:43.000000 piel-0.0.41/docs/autoapi/piel/models/frequency/electronic/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-07-08 15:25:43.000000 piel-0.0.41/docs/autoapi/piel/models/frequency/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.131372 piel-0.0.41/docs/autoapi/piel/models/frequency/opto_electronic/
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-07-08 15:25:43.000000 piel-0.0.41/docs/autoapi/piel/models/frequency/opto_electronic/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.131372 piel-0.0.41/docs/autoapi/piel/models/frequency/photonic/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.131372 piel-0.0.41/docs/autoapi/piel/models/frequency/photonic/coupler_simple/
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-07-08 15:25:43.000000 piel-0.0.41/docs/autoapi/piel/models/frequency/photonic/coupler_simple/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.131372 piel-0.0.41/docs/autoapi/piel/models/frequency/photonic/directional_coupler_length/
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-07-08 15:25:43.000000 piel-0.0.41/docs/autoapi/piel/models/frequency/photonic/directional_coupler_length/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.131372 piel-0.0.41/docs/autoapi/piel/models/frequency/photonic/directional_coupler_real/
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-07-08 15:25:43.000000 piel-0.0.41/docs/autoapi/piel/models/frequency/photonic/directional_coupler_real/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.131372 piel-0.0.41/docs/autoapi/piel/models/frequency/photonic/directional_coupler_simple/
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-07-08 15:25:43.000000 piel-0.0.41/docs/autoapi/piel/models/frequency/photonic/directional_coupler_simple/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.131372 piel-0.0.41/docs/autoapi/piel/models/frequency/photonic/grating_coupler/
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-07-08 15:25:43.000000 piel-0.0.41/docs/autoapi/piel/models/frequency/photonic/grating_coupler/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-07-08 15:25:43.000000 piel-0.0.41/docs/autoapi/piel/models/frequency/photonic/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.131372 piel-0.0.41/docs/autoapi/piel/models/frequency/photonic/mmi1x2/
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-07-08 15:25:43.000000 piel-0.0.41/docs/autoapi/piel/models/frequency/photonic/mmi1x2/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.131372 piel-0.0.41/docs/autoapi/piel/models/frequency/photonic/mmi2x2/
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-07-08 15:25:43.000000 piel-0.0.41/docs/autoapi/piel/models/frequency/photonic/mmi2x2/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.131372 piel-0.0.41/docs/autoapi/piel/models/frequency/photonic/straight_waveguide/
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-07-08 15:25:43.000000 piel-0.0.41/docs/autoapi/piel/models/frequency/photonic/straight_waveguide/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.131372 piel-0.0.41/docs/autoapi/piel/models/frequency/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-07-08 15:25:43.000000 piel-0.0.41/docs/autoapi/piel/models/frequency/utils/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-07-08 15:25:43.000000 piel-0.0.41/docs/autoapi/piel/models/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.131372 piel-0.0.41/docs/autoapi/piel/models/logic/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.131372 piel-0.0.41/docs/autoapi/piel/models/logic/electrical/
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-08 15:25:43.000000 piel-0.0.41/docs/autoapi/piel/models/logic/electrical/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.131372 piel-0.0.41/docs/autoapi/piel/models/logic/electro_optic/
--rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-07-08 15:25:43.000000 piel-0.0.41/docs/autoapi/piel/models/logic/electro_optic/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.131372 piel-0.0.41/docs/autoapi/piel/models/logic/electro_optic/signal_mapping/
--rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-07-08 15:25:43.000000 piel-0.0.41/docs/autoapi/piel/models/logic/electro_optic/signal_mapping/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.131372 piel-0.0.41/docs/autoapi/piel/models/logic/electronic/
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-08 15:25:43.000000 piel-0.0.41/docs/autoapi/piel/models/logic/electronic/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-08 15:25:43.000000 piel-0.0.41/docs/autoapi/piel/models/logic/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.131372 piel-0.0.41/docs/autoapi/piel/models/logic/opto_electronic/
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-08 15:25:43.000000 piel-0.0.41/docs/autoapi/piel/models/logic/opto_electronic/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.131372 piel-0.0.41/docs/autoapi/piel/models/logic/photonic/
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-08 15:25:43.000000 piel-0.0.41/docs/autoapi/piel/models/logic/photonic/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.131372 piel-0.0.41/docs/autoapi/piel/models/physical/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.131372 piel-0.0.41/docs/autoapi/piel/models/physical/electrical/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.131372 piel-0.0.41/docs/autoapi/piel/models/physical/electrical/cable/
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-07-08 15:25:43.000000 piel-0.0.41/docs/autoapi/piel/models/physical/electrical/cable/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-07-08 15:25:43.000000 piel-0.0.41/docs/autoapi/piel/models/physical/electrical/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.131372 piel-0.0.41/docs/autoapi/piel/models/physical/electro_optic/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.131372 piel-0.0.41/docs/autoapi/piel/models/physical/electro_optic/basic_heater/
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-08 15:25:43.000000 piel-0.0.41/docs/autoapi/piel/models/physical/electro_optic/basic_heater/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-07-08 15:25:43.000000 piel-0.0.41/docs/autoapi/piel/models/physical/electro_optic/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.131372 piel-0.0.41/docs/autoapi/piel/models/physical/electronic/
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-08 15:25:43.000000 piel-0.0.41/docs/autoapi/piel/models/physical/electronic/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.131372 piel-0.0.41/docs/autoapi/piel/models/physical/geometry/
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-07-08 15:25:43.000000 piel-0.0.41/docs/autoapi/piel/models/physical/geometry/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-07-08 15:25:43.000000 piel-0.0.41/docs/autoapi/piel/models/physical/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.131372 piel-0.0.41/docs/autoapi/piel/models/physical/opto_electronic/
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-07-08 15:25:43.000000 piel-0.0.41/docs/autoapi/piel/models/physical/opto_electronic/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.131372 piel-0.0.41/docs/autoapi/piel/models/physical/photonic/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-08 15:25:43.000000 piel-0.0.41/docs/autoapi/piel/models/physical/photonic/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.131372 piel-0.0.41/docs/autoapi/piel/models/physical/thermal/
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-07-08 15:25:43.000000 piel-0.0.41/docs/autoapi/piel/models/physical/thermal/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.135372 piel-0.0.41/docs/autoapi/piel/models/physical/units/
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-07-08 15:25:43.000000 piel-0.0.41/docs/autoapi/piel/models/physical/units/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.135372 piel-0.0.41/docs/autoapi/piel/models/transient/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.135372 piel-0.0.41/docs/autoapi/piel/models/transient/electrical/
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-08 15:25:43.000000 piel-0.0.41/docs/autoapi/piel/models/transient/electrical/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.135372 piel-0.0.41/docs/autoapi/piel/models/transient/electro_optic/
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-08 15:25:43.000000 piel-0.0.41/docs/autoapi/piel/models/transient/electro_optic/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.135372 piel-0.0.41/docs/autoapi/piel/models/transient/electronic/
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-08 15:25:43.000000 piel-0.0.41/docs/autoapi/piel/models/transient/electronic/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-07-08 15:25:43.000000 piel-0.0.41/docs/autoapi/piel/models/transient/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.135372 piel-0.0.41/docs/autoapi/piel/models/transient/opto_electronic/
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-07-08 15:25:43.000000 piel-0.0.41/docs/autoapi/piel/models/transient/opto_electronic/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.135372 piel-0.0.41/docs/autoapi/piel/models/transient/photonic/
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-08 15:25:43.000000 piel-0.0.41/docs/autoapi/piel/models/transient/photonic/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.135372 piel-0.0.41/docs/autoapi/piel/models/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-08 15:25:43.000000 piel-0.0.41/docs/autoapi/piel/models/utils/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.135372 piel-0.0.41/docs/autoapi/piel/parametric/
--rw-r--r--   0 runner    (1001) docker     (123)     3026 2023-07-08 15:25:43.000000 piel-0.0.41/docs/autoapi/piel/parametric/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.135372 piel-0.0.41/docs/autoapi/piel/project_structure/
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-07-08 15:25:43.000000 piel-0.0.41/docs/autoapi/piel/project_structure/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.135372 piel-0.0.41/docs/autoapi/piel/tools/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.135372 piel-0.0.41/docs/autoapi/piel/tools/cocotb/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.135372 piel-0.0.41/docs/autoapi/piel/tools/cocotb/core/
--rw-r--r--   0 runner    (1001) docker     (123)     3967 2023-07-08 15:25:43.000000 piel-0.0.41/docs/autoapi/piel/tools/cocotb/core/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.135372 piel-0.0.41/docs/autoapi/piel/tools/cocotb/data/
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-07-08 15:25:43.000000 piel-0.0.41/docs/autoapi/piel/tools/cocotb/data/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-07-08 15:25:43.000000 piel-0.0.41/docs/autoapi/piel/tools/cocotb/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.135372 piel-0.0.41/docs/autoapi/piel/tools/gdsfactory/
--rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-07-08 15:25:43.000000 piel-0.0.41/docs/autoapi/piel/tools/gdsfactory/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.135372 piel-0.0.41/docs/autoapi/piel/tools/gdsfactory/netlist/
--rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-07-08 15:25:43.000000 piel-0.0.41/docs/autoapi/piel/tools/gdsfactory/netlist/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)    26766 2023-07-08 15:25:43.000000 piel-0.0.41/docs/autoapi/piel/tools/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.135372 piel-0.0.41/docs/autoapi/piel/tools/openlane/
--rw-r--r--   0 runner    (1001) docker     (123)    16244 2023-07-08 15:25:43.000000 piel-0.0.41/docs/autoapi/piel/tools/openlane/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.135372 piel-0.0.41/docs/autoapi/piel/tools/openlane/migrate/
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-07-08 15:25:43.000000 piel-0.0.41/docs/autoapi/piel/tools/openlane/migrate/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.135372 piel-0.0.41/docs/autoapi/piel/tools/openlane/parse/
--rw-r--r--   0 runner    (1001) docker     (123)     8914 2023-07-08 15:25:43.000000 piel-0.0.41/docs/autoapi/piel/tools/openlane/parse/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.135372 piel-0.0.41/docs/autoapi/piel/tools/openlane/parse/sta_rpt/
--rw-r--r--   0 runner    (1001) docker     (123)     5458 2023-07-08 15:25:43.000000 piel-0.0.41/docs/autoapi/piel/tools/openlane/parse/sta_rpt/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.135372 piel-0.0.41/docs/autoapi/piel/tools/openlane/parse/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-07-08 15:25:43.000000 piel-0.0.41/docs/autoapi/piel/tools/openlane/parse/utils/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.135372 piel-0.0.41/docs/autoapi/piel/tools/openlane/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-07-08 15:25:43.000000 piel-0.0.41/docs/autoapi/piel/tools/openlane/utils/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.135372 piel-0.0.41/docs/autoapi/piel/tools/openlane/v1/
--rw-r--r--   0 runner    (1001) docker     (123)     5707 2023-07-08 15:25:43.000000 piel-0.0.41/docs/autoapi/piel/tools/openlane/v1/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.135372 piel-0.0.41/docs/autoapi/piel/tools/openlane/v2/
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-07-08 15:25:43.000000 piel-0.0.41/docs/autoapi/piel/tools/openlane/v2/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.135372 piel-0.0.41/docs/autoapi/piel/tools/sax/
--rw-r--r--   0 runner    (1001) docker     (123)     4883 2023-07-08 15:25:43.000000 piel-0.0.41/docs/autoapi/piel/tools/sax/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.135372 piel-0.0.41/docs/autoapi/piel/tools/sax/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     4983 2023-07-08 15:25:43.000000 piel-0.0.41/docs/autoapi/piel/tools/sax/utils/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.135372 piel-0.0.41/docs/autoapi/piel/visual/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.135372 piel-0.0.41/docs/autoapi/piel/visual/auto_plot_multiple/
--rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-07-08 15:25:43.000000 piel-0.0.41/docs/autoapi/piel/visual/auto_plot_multiple/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.135372 piel-0.0.41/docs/autoapi/piel/visual/data_conversion/
--rw-r--r--   0 runner    (1001) docker     (123)     2590 2023-07-08 15:25:43.000000 piel-0.0.41/docs/autoapi/piel/visual/data_conversion/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3697 2023-07-08 15:25:43.000000 piel-0.0.41/docs/autoapi/piel/visual/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4082 2023-07-08 15:25:43.000000 piel-0.0.41/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-08 15:25:43.000000 piel-0.0.41/docs/contributing.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.119372 piel-0.0.41/docs/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.119372 piel-0.0.41/docs/examples/designs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.119372 piel-0.0.41/docs/examples/designs/simple_design/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.119372 piel-0.0.41/docs/examples/designs/simple_design/simple_design/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.135372 piel-0.0.41/docs/examples/designs/simple_design/simple_design/tb/
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-07-08 15:25:43.000000 piel-0.0.41/docs/examples/designs/simple_design/simple_design/tb/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.135372 piel-0.0.41/docs/examples/designs/simple_design/simple_design/tb/default/
--rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-07-08 15:25:43.000000 piel-0.0.41/docs/examples/designs/simple_design/simple_design/tb/default/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-07-08 15:25:43.000000 piel-0.0.41/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-07-08 15:25:43.000000 piel-0.0.41/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-07-08 15:25:43.000000 piel-0.0.41/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.123372 piel-0.0.41/docs/sections/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.139372 piel-0.0.41/docs/sections/about/
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-07-08 15:25:43.000000 piel-0.0.41/docs/sections/about/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-08 15:25:43.000000 piel-0.0.41/docs/sections/about/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.139372 piel-0.0.41/docs/sections/codesign/
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-08 15:25:43.000000 piel-0.0.41/docs/sections/codesign/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.139372 piel-0.0.41/docs/sections/components/
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-08 15:25:43.000000 piel-0.0.41/docs/sections/components/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.139372 piel-0.0.41/docs/sections/environment/
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-07-08 15:25:43.000000 piel-0.0.41/docs/sections/environment/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.139372 piel-0.0.41/docs/sections/microservices/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.139372 piel-0.0.41/docs/sections/microservices/dependencies/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-08 15:25:43.000000 piel-0.0.41/docs/sections/microservices/dependencies/cocotb.rst
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-07-08 15:25:43.000000 piel-0.0.41/docs/sections/microservices/dependencies/gdsfactory.rst
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-08 15:25:43.000000 piel-0.0.41/docs/sections/microservices/dependencies/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-07-08 15:25:43.000000 piel-0.0.41/docs/sections/microservices/dependencies/openlane.rst
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-07-08 15:25:43.000000 piel-0.0.41/docs/sections/microservices/dependencies/principle.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-07-08 15:25:43.000000 piel-0.0.41/docs/sections/microservices/dependencies/pyspice.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3007 2023-07-08 15:25:43.000000 piel-0.0.41/docs/sections/microservices/dependencies/sax.rst
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-08 15:25:43.000000 piel-0.0.41/docs/sections/microservices/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.139372 piel-0.0.41/docs/sections/microservices/integration/
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-08 15:25:43.000000 piel-0.0.41/docs/sections/microservices/integration/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-07-08 15:25:43.000000 piel-0.0.41/docs/sections/microservices/integration/sax_qutip.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.139372 piel-0.0.41/docs/sections/models/
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-07-08 15:25:43.000000 piel-0.0.41/docs/sections/models/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.139372 piel-0.0.41/piel/
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-07-08 15:25:43.000000 piel-0.0.41/piel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-07-08 15:25:43.000000 piel-0.0.41/piel/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.143372 piel-0.0.41/piel/components/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 15:25:43.000000 piel-0.0.41/piel/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      905 2023-07-08 15:25:43.000000 piel-0.0.41/piel/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-07-08 15:25:43.000000 piel-0.0.41/piel/defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-07-08 15:25:43.000000 piel-0.0.41/piel/file_conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)    11207 2023-07-08 15:25:43.000000 piel-0.0.41/piel/file_system.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.143372 piel-0.0.41/piel/integration/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-08 15:25:43.000000 piel-0.0.41/piel/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-07-08 15:25:43.000000 piel-0.0.41/piel/integration/openlane_gdsfactory_core.py
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-08 15:25:43.000000 piel-0.0.41/piel/integration/sax_cocotb.py
--rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-07-08 15:25:43.000000 piel-0.0.41/piel/integration/sax_qutip.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.143372 piel-0.0.41/piel/models/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-07-08 15:25:43.000000 piel-0.0.41/piel/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.143372 piel-0.0.41/piel/models/frequency/
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-07-08 15:25:43.000000 piel-0.0.41/piel/models/frequency/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-07-08 15:25:43.000000 piel-0.0.41/piel/models/frequency/all.py
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-07-08 15:25:43.000000 piel-0.0.41/piel/models/frequency/defaults.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.143372 piel-0.0.41/piel/models/frequency/electrical/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 15:25:43.000000 piel-0.0.41/piel/models/frequency/electrical/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.143372 piel-0.0.41/piel/models/frequency/electro_optic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 15:25:43.000000 piel-0.0.41/piel/models/frequency/electro_optic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-08 15:25:43.000000 piel-0.0.41/piel/models/frequency/electro_optic/ideal.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.143372 piel-0.0.41/piel/models/frequency/electronic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 15:25:43.000000 piel-0.0.41/piel/models/frequency/electronic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.143372 piel-0.0.41/piel/models/frequency/opto_electronic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 15:25:43.000000 piel-0.0.41/piel/models/frequency/opto_electronic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.143372 piel-0.0.41/piel/models/frequency/photonic/
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-08 15:25:43.000000 piel-0.0.41/piel/models/frequency/photonic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-07-08 15:25:43.000000 piel-0.0.41/piel/models/frequency/photonic/coupler_simple.py
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-07-08 15:25:43.000000 piel-0.0.41/piel/models/frequency/photonic/directional_coupler_length.py
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-07-08 15:25:43.000000 piel-0.0.41/piel/models/frequency/photonic/directional_coupler_real.py
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-07-08 15:25:43.000000 piel-0.0.41/piel/models/frequency/photonic/directional_coupler_simple.py
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-07-08 15:25:43.000000 piel-0.0.41/piel/models/frequency/photonic/grating_coupler.py
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-07-08 15:25:43.000000 piel-0.0.41/piel/models/frequency/photonic/mmi1x2.py
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-07-08 15:25:43.000000 piel-0.0.41/piel/models/frequency/photonic/mmi2x2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-07-08 15:25:43.000000 piel-0.0.41/piel/models/frequency/photonic/straight_waveguide.py
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-07-08 15:25:43.000000 piel-0.0.41/piel/models/frequency/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.143372 piel-0.0.41/piel/models/logic/
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-07-08 15:25:43.000000 piel-0.0.41/piel/models/logic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.143372 piel-0.0.41/piel/models/logic/electrical/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 15:25:43.000000 piel-0.0.41/piel/models/logic/electrical/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.143372 piel-0.0.41/piel/models/logic/electro_optic/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-08 15:25:43.000000 piel-0.0.41/piel/models/logic/electro_optic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2964 2023-07-08 15:25:43.000000 piel-0.0.41/piel/models/logic/electro_optic/signal_mapping.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.143372 piel-0.0.41/piel/models/logic/electronic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 15:25:43.000000 piel-0.0.41/piel/models/logic/electronic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.143372 piel-0.0.41/piel/models/logic/opto_electronic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 15:25:43.000000 piel-0.0.41/piel/models/logic/opto_electronic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.143372 piel-0.0.41/piel/models/logic/photonic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 15:25:43.000000 piel-0.0.41/piel/models/logic/photonic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.147372 piel-0.0.41/piel/models/physical/
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-07-08 15:25:43.000000 piel-0.0.41/piel/models/physical/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.147372 piel-0.0.41/piel/models/physical/electrical/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 15:25:43.000000 piel-0.0.41/piel/models/physical/electrical/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 15:25:43.000000 piel-0.0.41/piel/models/physical/electrical/cable.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.147372 piel-0.0.41/piel/models/physical/electro_optic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 15:25:43.000000 piel-0.0.41/piel/models/physical/electro_optic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-07-08 15:25:43.000000 piel-0.0.41/piel/models/physical/electro_optic/basic_heater.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.147372 piel-0.0.41/piel/models/physical/electronic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 15:25:43.000000 piel-0.0.41/piel/models/physical/electronic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-07-08 15:25:43.000000 piel-0.0.41/piel/models/physical/geometry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.147372 piel-0.0.41/piel/models/physical/opto_electronic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 15:25:43.000000 piel-0.0.41/piel/models/physical/opto_electronic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.147372 piel-0.0.41/piel/models/physical/photonic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 15:25:43.000000 piel-0.0.41/piel/models/physical/photonic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-07-08 15:25:43.000000 piel-0.0.41/piel/models/physical/thermal.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-08 15:25:43.000000 piel-0.0.41/piel/models/physical/units.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.147372 piel-0.0.41/piel/models/transient/
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-07-08 15:25:43.000000 piel-0.0.41/piel/models/transient/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.147372 piel-0.0.41/piel/models/transient/electrical/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 15:25:43.000000 piel-0.0.41/piel/models/transient/electrical/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.147372 piel-0.0.41/piel/models/transient/electro_optic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 15:25:43.000000 piel-0.0.41/piel/models/transient/electro_optic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.147372 piel-0.0.41/piel/models/transient/electronic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 15:25:43.000000 piel-0.0.41/piel/models/transient/electronic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.147372 piel-0.0.41/piel/models/transient/opto_electronic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 15:25:43.000000 piel-0.0.41/piel/models/transient/opto_electronic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.147372 piel-0.0.41/piel/models/transient/photonic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 15:25:43.000000 piel-0.0.41/piel/models/transient/photonic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 15:25:43.000000 piel-0.0.41/piel/models/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3928 2023-07-08 15:25:43.000000 piel-0.0.41/piel/parametric.py
--rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-07-08 15:25:43.000000 piel-0.0.41/piel/project_structure.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.147372 piel-0.0.41/piel/tools/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-08 15:25:43.000000 piel-0.0.41/piel/tools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.147372 piel-0.0.41/piel/tools/cocotb/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-08 15:25:43.000000 piel-0.0.41/piel/tools/cocotb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6178 2023-07-08 15:25:43.000000 piel-0.0.41/piel/tools/cocotb/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-07-08 15:25:43.000000 piel-0.0.41/piel/tools/cocotb/data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.147372 piel-0.0.41/piel/tools/gdsfactory/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-08 15:25:43.000000 piel-0.0.41/piel/tools/gdsfactory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4517 2023-07-08 15:25:43.000000 piel-0.0.41/piel/tools/gdsfactory/netlist.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.147372 piel-0.0.41/piel/tools/openlane/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-08 15:25:43.000000 piel-0.0.41/piel/tools/openlane/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-07-08 15:25:43.000000 piel-0.0.41/piel/tools/openlane/migrate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.147372 piel-0.0.41/piel/tools/openlane/parse/
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-07-08 15:25:43.000000 piel-0.0.41/piel/tools/openlane/parse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10719 2023-07-08 15:25:43.000000 piel-0.0.41/piel/tools/openlane/parse/sta_rpt.py
--rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-07-08 15:25:43.000000 piel-0.0.41/piel/tools/openlane/parse/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-07-08 15:25:43.000000 piel-0.0.41/piel/tools/openlane/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10697 2023-07-08 15:25:43.000000 piel-0.0.41/piel/tools/openlane/v1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-07-08 15:25:43.000000 piel-0.0.41/piel/tools/openlane/v2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.147372 piel-0.0.41/piel/tools/sax/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-08 15:25:43.000000 piel-0.0.41/piel/tools/sax/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7121 2023-07-08 15:25:43.000000 piel-0.0.41/piel/tools/sax/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.151372 piel-0.0.41/piel/visual/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-08 15:25:43.000000 piel-0.0.41/piel/visual/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3000 2023-07-08 15:25:43.000000 piel-0.0.41/piel/visual/auto_plot_multiple.py
--rw-r--r--   0 runner    (1001) docker     (123)     4315 2023-07-08 15:25:43.000000 piel-0.0.41/piel/visual/data_conversion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.139372 piel-0.0.41/piel.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3707 2023-07-08 15:26:00.000000 piel-0.0.41/piel.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8203 2023-07-08 15:26:00.000000 piel-0.0.41/piel.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 15:26:00.000000 piel-0.0.41/piel.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-08 15:26:00.000000 piel-0.0.41/piel.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 15:25:59.000000 piel-0.0.41/piel.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-07-08 15:26:00.000000 piel-0.0.41/piel.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-08 15:26:00.000000 piel-0.0.41/piel.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-07-08 15:26:00.151372 piel-0.0.41/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-07-08 15:25:43.000000 piel-0.0.41/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.151372 piel-0.0.41/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-08 15:25:43.000000 piel-0.0.41/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.123372 piel-0.0.41/tests/models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.123372 piel-0.0.41/tests/models/logic/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.151372 piel-0.0.41/tests/models/logic/electro_optic/
--rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-07-08 15:25:43.000000 piel-0.0.41/tests/models/logic/electro_optic/test_signal_mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-07-08 15:25:43.000000 piel-0.0.41/tests/test_piel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.151372 piel-0.0.41/tests/tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 15:25:43.000000 piel-0.0.41/tests/tools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.151372 piel-0.0.41/tests/tools/gdsfactory/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-08 15:25:43.000000 piel-0.0.41/tests/tools/gdsfactory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-07-08 15:25:43.000000 piel-0.0.41/tests/tools/gdsfactory/test_netlist.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.151372 piel-0.0.41/tests/tools/sax/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 15:25:43.000000 piel-0.0.41/tests/tools/sax/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3773 2023-07-08 15:25:43.000000 piel-0.0.41/tests/tools/sax/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:26:00.151372 piel-0.0.41/tests/visual/
--rw-r--r--   0 runner    (1001) docker     (123)     9100 2023-07-08 15:25:43.000000 piel-0.0.41/tests/visual/test_data_conversion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.605553 piel-0.0.43/
+-rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-07-13 21:52:16.000000 piel-0.0.43/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-13 21:52:16.000000 piel-0.0.43/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-07-13 21:52:16.000000 piel-0.0.43/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3951 2023-07-13 21:52:33.605553 piel-0.0.43/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-07-13 21:52:16.000000 piel-0.0.43/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.577553 piel-0.0.43/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-07-13 21:52:16.000000 piel-0.0.43/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.565553 piel-0.0.43/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.577553 piel-0.0.43/docs/_static/img/
+-rw-r--r--   0 runner    (1001) docker     (123)     5176 2023-07-13 21:52:16.000000 piel-0.0.43/docs/_static/img/logo.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.577553 piel-0.0.43/docs/autoapi/
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-13 21:52:16.000000 piel-0.0.43/docs/autoapi/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.577553 piel-0.0.43/docs/autoapi/piel/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.577553 piel-0.0.43/docs/autoapi/piel/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-13 21:52:16.000000 piel-0.0.43/docs/autoapi/piel/cli/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.577553 piel-0.0.43/docs/autoapi/piel/components/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-13 21:52:16.000000 piel-0.0.43/docs/autoapi/piel/components/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.581553 piel-0.0.43/docs/autoapi/piel/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-13 21:52:16.000000 piel-0.0.43/docs/autoapi/piel/config/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.581553 piel-0.0.43/docs/autoapi/piel/defaults/
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-07-13 21:52:16.000000 piel-0.0.43/docs/autoapi/piel/defaults/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.581553 piel-0.0.43/docs/autoapi/piel/file_conversion/
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-07-13 21:52:16.000000 piel-0.0.43/docs/autoapi/piel/file_conversion/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.581553 piel-0.0.43/docs/autoapi/piel/file_system/
+-rw-r--r--   0 runner    (1001) docker     (123)     5453 2023-07-13 21:52:16.000000 piel-0.0.43/docs/autoapi/piel/file_system/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    47512 2023-07-13 21:52:16.000000 piel-0.0.43/docs/autoapi/piel/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.581553 piel-0.0.43/docs/autoapi/piel/integration/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.581553 piel-0.0.43/docs/autoapi/piel/integration/cocotb_sax/
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-13 21:52:16.000000 piel-0.0.43/docs/autoapi/piel/integration/cocotb_sax/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.581553 piel-0.0.43/docs/autoapi/piel/integration/gdsfactory_openlane/
+-rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-07-13 21:52:16.000000 piel-0.0.43/docs/autoapi/piel/integration/gdsfactory_openlane/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.581553 piel-0.0.43/docs/autoapi/piel/integration/gdsfactory_pyspice/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.581553 piel-0.0.43/docs/autoapi/piel/integration/gdsfactory_pyspice/conversion/
+-rw-r--r--   0 runner    (1001) docker     (123)     2810 2023-07-13 21:52:16.000000 piel-0.0.43/docs/autoapi/piel/integration/gdsfactory_pyspice/conversion/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.581553 piel-0.0.43/docs/autoapi/piel/integration/gdsfactory_pyspice/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     7627 2023-07-13 21:52:16.000000 piel-0.0.43/docs/autoapi/piel/integration/gdsfactory_pyspice/core/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3467 2023-07-13 21:52:16.000000 piel-0.0.43/docs/autoapi/piel/integration/gdsfactory_pyspice/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.581553 piel-0.0.43/docs/autoapi/piel/integration/gdsfactory_pyspice/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-07-13 21:52:16.000000 piel-0.0.43/docs/autoapi/piel/integration/gdsfactory_pyspice/utils/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    12128 2023-07-13 21:52:16.000000 piel-0.0.43/docs/autoapi/piel/integration/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.581553 piel-0.0.43/docs/autoapi/piel/integration/pyspice_sax/
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-07-13 21:52:16.000000 piel-0.0.43/docs/autoapi/piel/integration/pyspice_sax/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.581553 piel-0.0.43/docs/autoapi/piel/integration/sax_qutip/
+-rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-07-13 21:52:16.000000 piel-0.0.43/docs/autoapi/piel/integration/sax_qutip/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.581553 piel-0.0.43/docs/autoapi/piel/integration/sax_thewalrus/
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-07-13 21:52:16.000000 piel-0.0.43/docs/autoapi/piel/integration/sax_thewalrus/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.581553 piel-0.0.43/docs/autoapi/piel/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.581553 piel-0.0.43/docs/autoapi/piel/models/frequency/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.581553 piel-0.0.43/docs/autoapi/piel/models/frequency/all/
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-07-13 21:52:16.000000 piel-0.0.43/docs/autoapi/piel/models/frequency/all/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.581553 piel-0.0.43/docs/autoapi/piel/models/frequency/defaults/
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-07-13 21:52:16.000000 piel-0.0.43/docs/autoapi/piel/models/frequency/defaults/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.581553 piel-0.0.43/docs/autoapi/piel/models/frequency/electrical/
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-13 21:52:16.000000 piel-0.0.43/docs/autoapi/piel/models/frequency/electrical/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.581553 piel-0.0.43/docs/autoapi/piel/models/frequency/electro_optic/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.581553 piel-0.0.43/docs/autoapi/piel/models/frequency/electro_optic/ideal/
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-13 21:52:16.000000 piel-0.0.43/docs/autoapi/piel/models/frequency/electro_optic/ideal/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-13 21:52:16.000000 piel-0.0.43/docs/autoapi/piel/models/frequency/electro_optic/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.581553 piel-0.0.43/docs/autoapi/piel/models/frequency/electronic/
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-13 21:52:16.000000 piel-0.0.43/docs/autoapi/piel/models/frequency/electronic/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-07-13 21:52:16.000000 piel-0.0.43/docs/autoapi/piel/models/frequency/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.581553 piel-0.0.43/docs/autoapi/piel/models/frequency/opto_electronic/
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-07-13 21:52:16.000000 piel-0.0.43/docs/autoapi/piel/models/frequency/opto_electronic/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.581553 piel-0.0.43/docs/autoapi/piel/models/frequency/photonic/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.581553 piel-0.0.43/docs/autoapi/piel/models/frequency/photonic/coupler_simple/
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-07-13 21:52:16.000000 piel-0.0.43/docs/autoapi/piel/models/frequency/photonic/coupler_simple/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.581553 piel-0.0.43/docs/autoapi/piel/models/frequency/photonic/directional_coupler_length/
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-07-13 21:52:16.000000 piel-0.0.43/docs/autoapi/piel/models/frequency/photonic/directional_coupler_length/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.581553 piel-0.0.43/docs/autoapi/piel/models/frequency/photonic/directional_coupler_real/
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-07-13 21:52:16.000000 piel-0.0.43/docs/autoapi/piel/models/frequency/photonic/directional_coupler_real/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.581553 piel-0.0.43/docs/autoapi/piel/models/frequency/photonic/directional_coupler_simple/
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-07-13 21:52:16.000000 piel-0.0.43/docs/autoapi/piel/models/frequency/photonic/directional_coupler_simple/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.581553 piel-0.0.43/docs/autoapi/piel/models/frequency/photonic/grating_coupler/
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-07-13 21:52:16.000000 piel-0.0.43/docs/autoapi/piel/models/frequency/photonic/grating_coupler/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-07-13 21:52:16.000000 piel-0.0.43/docs/autoapi/piel/models/frequency/photonic/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.581553 piel-0.0.43/docs/autoapi/piel/models/frequency/photonic/mmi1x2/
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-07-13 21:52:16.000000 piel-0.0.43/docs/autoapi/piel/models/frequency/photonic/mmi1x2/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.585553 piel-0.0.43/docs/autoapi/piel/models/frequency/photonic/mmi2x2/
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-07-13 21:52:16.000000 piel-0.0.43/docs/autoapi/piel/models/frequency/photonic/mmi2x2/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.585553 piel-0.0.43/docs/autoapi/piel/models/frequency/photonic/straight_waveguide/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-07-13 21:52:16.000000 piel-0.0.43/docs/autoapi/piel/models/frequency/photonic/straight_waveguide/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.585553 piel-0.0.43/docs/autoapi/piel/models/frequency/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-07-13 21:52:16.000000 piel-0.0.43/docs/autoapi/piel/models/frequency/utils/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-07-13 21:52:16.000000 piel-0.0.43/docs/autoapi/piel/models/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.585553 piel-0.0.43/docs/autoapi/piel/models/logic/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.585553 piel-0.0.43/docs/autoapi/piel/models/logic/electrical/
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-13 21:52:16.000000 piel-0.0.43/docs/autoapi/piel/models/logic/electrical/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.585553 piel-0.0.43/docs/autoapi/piel/models/logic/electro_optic/
+-rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-07-13 21:52:16.000000 piel-0.0.43/docs/autoapi/piel/models/logic/electro_optic/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.585553 piel-0.0.43/docs/autoapi/piel/models/logic/electro_optic/signal_mapping/
+-rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-07-13 21:52:16.000000 piel-0.0.43/docs/autoapi/piel/models/logic/electro_optic/signal_mapping/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.585553 piel-0.0.43/docs/autoapi/piel/models/logic/electronic/
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-13 21:52:16.000000 piel-0.0.43/docs/autoapi/piel/models/logic/electronic/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-13 21:52:16.000000 piel-0.0.43/docs/autoapi/piel/models/logic/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.585553 piel-0.0.43/docs/autoapi/piel/models/logic/opto_electronic/
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-13 21:52:16.000000 piel-0.0.43/docs/autoapi/piel/models/logic/opto_electronic/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.585553 piel-0.0.43/docs/autoapi/piel/models/logic/photonic/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-13 21:52:16.000000 piel-0.0.43/docs/autoapi/piel/models/logic/photonic/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.585553 piel-0.0.43/docs/autoapi/piel/models/physical/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.585553 piel-0.0.43/docs/autoapi/piel/models/physical/electrical/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.585553 piel-0.0.43/docs/autoapi/piel/models/physical/electrical/cable/
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-07-13 21:52:16.000000 piel-0.0.43/docs/autoapi/piel/models/physical/electrical/cable/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-07-13 21:52:16.000000 piel-0.0.43/docs/autoapi/piel/models/physical/electrical/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.585553 piel-0.0.43/docs/autoapi/piel/models/physical/electro_optic/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.585553 piel-0.0.43/docs/autoapi/piel/models/physical/electro_optic/basic_heater/
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-13 21:52:16.000000 piel-0.0.43/docs/autoapi/piel/models/physical/electro_optic/basic_heater/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-07-13 21:52:16.000000 piel-0.0.43/docs/autoapi/piel/models/physical/electro_optic/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.585553 piel-0.0.43/docs/autoapi/piel/models/physical/electronic/
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-13 21:52:16.000000 piel-0.0.43/docs/autoapi/piel/models/physical/electronic/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.585553 piel-0.0.43/docs/autoapi/piel/models/physical/electronic/spice/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.585553 piel-0.0.43/docs/autoapi/piel/models/physical/electronic/spice/capacitor/
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-07-13 21:52:16.000000 piel-0.0.43/docs/autoapi/piel/models/physical/electronic/spice/capacitor/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.585553 piel-0.0.43/docs/autoapi/piel/models/physical/electronic/spice/defaults/
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-07-13 21:52:16.000000 piel-0.0.43/docs/autoapi/piel/models/physical/electronic/spice/defaults/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-07-13 21:52:16.000000 piel-0.0.43/docs/autoapi/piel/models/physical/electronic/spice/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.585553 piel-0.0.43/docs/autoapi/piel/models/physical/electronic/spice/resistor/
+-rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-07-13 21:52:16.000000 piel-0.0.43/docs/autoapi/piel/models/physical/electronic/spice/resistor/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.585553 piel-0.0.43/docs/autoapi/piel/models/physical/geometry/
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-07-13 21:52:16.000000 piel-0.0.43/docs/autoapi/piel/models/physical/geometry/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-07-13 21:52:16.000000 piel-0.0.43/docs/autoapi/piel/models/physical/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.585553 piel-0.0.43/docs/autoapi/piel/models/physical/opto_electronic/
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-07-13 21:52:16.000000 piel-0.0.43/docs/autoapi/piel/models/physical/opto_electronic/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.585553 piel-0.0.43/docs/autoapi/piel/models/physical/photonic/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-13 21:52:16.000000 piel-0.0.43/docs/autoapi/piel/models/physical/photonic/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.585553 piel-0.0.43/docs/autoapi/piel/models/physical/thermal/
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-07-13 21:52:16.000000 piel-0.0.43/docs/autoapi/piel/models/physical/thermal/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.585553 piel-0.0.43/docs/autoapi/piel/models/physical/units/
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-07-13 21:52:16.000000 piel-0.0.43/docs/autoapi/piel/models/physical/units/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.585553 piel-0.0.43/docs/autoapi/piel/models/transient/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.585553 piel-0.0.43/docs/autoapi/piel/models/transient/electrical/
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-13 21:52:16.000000 piel-0.0.43/docs/autoapi/piel/models/transient/electrical/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.585553 piel-0.0.43/docs/autoapi/piel/models/transient/electro_optic/
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-13 21:52:16.000000 piel-0.0.43/docs/autoapi/piel/models/transient/electro_optic/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.585553 piel-0.0.43/docs/autoapi/piel/models/transient/electronic/
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-13 21:52:16.000000 piel-0.0.43/docs/autoapi/piel/models/transient/electronic/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-07-13 21:52:16.000000 piel-0.0.43/docs/autoapi/piel/models/transient/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.585553 piel-0.0.43/docs/autoapi/piel/models/transient/opto_electronic/
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-07-13 21:52:16.000000 piel-0.0.43/docs/autoapi/piel/models/transient/opto_electronic/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.589553 piel-0.0.43/docs/autoapi/piel/models/transient/photonic/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-13 21:52:16.000000 piel-0.0.43/docs/autoapi/piel/models/transient/photonic/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.589553 piel-0.0.43/docs/autoapi/piel/models/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-13 21:52:16.000000 piel-0.0.43/docs/autoapi/piel/models/utils/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.589553 piel-0.0.43/docs/autoapi/piel/parametric/
+-rw-r--r--   0 runner    (1001) docker     (123)     3026 2023-07-13 21:52:16.000000 piel-0.0.43/docs/autoapi/piel/parametric/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.589553 piel-0.0.43/docs/autoapi/piel/project_structure/
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-07-13 21:52:16.000000 piel-0.0.43/docs/autoapi/piel/project_structure/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.589553 piel-0.0.43/docs/autoapi/piel/tools/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.589553 piel-0.0.43/docs/autoapi/piel/tools/cocotb/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.589553 piel-0.0.43/docs/autoapi/piel/tools/cocotb/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     3982 2023-07-13 21:52:16.000000 piel-0.0.43/docs/autoapi/piel/tools/cocotb/core/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.589553 piel-0.0.43/docs/autoapi/piel/tools/cocotb/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-07-13 21:52:16.000000 piel-0.0.43/docs/autoapi/piel/tools/cocotb/data/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4155 2023-07-13 21:52:16.000000 piel-0.0.43/docs/autoapi/piel/tools/cocotb/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.589553 piel-0.0.43/docs/autoapi/piel/tools/gdsfactory/
+-rw-r--r--   0 runner    (1001) docker     (123)     3472 2023-07-13 21:52:16.000000 piel-0.0.43/docs/autoapi/piel/tools/gdsfactory/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.589553 piel-0.0.43/docs/autoapi/piel/tools/gdsfactory/netlist/
+-rw-r--r--   0 runner    (1001) docker     (123)     3419 2023-07-13 21:52:16.000000 piel-0.0.43/docs/autoapi/piel/tools/gdsfactory/netlist/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    27444 2023-07-13 21:52:16.000000 piel-0.0.43/docs/autoapi/piel/tools/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.589553 piel-0.0.43/docs/autoapi/piel/tools/openlane/
+-rw-r--r--   0 runner    (1001) docker     (123)    16244 2023-07-13 21:52:16.000000 piel-0.0.43/docs/autoapi/piel/tools/openlane/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.589553 piel-0.0.43/docs/autoapi/piel/tools/openlane/migrate/
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-07-13 21:52:16.000000 piel-0.0.43/docs/autoapi/piel/tools/openlane/migrate/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.589553 piel-0.0.43/docs/autoapi/piel/tools/openlane/parse/
+-rw-r--r--   0 runner    (1001) docker     (123)     8914 2023-07-13 21:52:16.000000 piel-0.0.43/docs/autoapi/piel/tools/openlane/parse/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.589553 piel-0.0.43/docs/autoapi/piel/tools/openlane/parse/sta_rpt/
+-rw-r--r--   0 runner    (1001) docker     (123)     5458 2023-07-13 21:52:16.000000 piel-0.0.43/docs/autoapi/piel/tools/openlane/parse/sta_rpt/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.589553 piel-0.0.43/docs/autoapi/piel/tools/openlane/parse/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-07-13 21:52:16.000000 piel-0.0.43/docs/autoapi/piel/tools/openlane/parse/utils/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.589553 piel-0.0.43/docs/autoapi/piel/tools/openlane/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-07-13 21:52:16.000000 piel-0.0.43/docs/autoapi/piel/tools/openlane/utils/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.589553 piel-0.0.43/docs/autoapi/piel/tools/openlane/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)     5707 2023-07-13 21:52:16.000000 piel-0.0.43/docs/autoapi/piel/tools/openlane/v1/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.589553 piel-0.0.43/docs/autoapi/piel/tools/openlane/v2/
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-07-13 21:52:16.000000 piel-0.0.43/docs/autoapi/piel/tools/openlane/v2/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.589553 piel-0.0.43/docs/autoapi/piel/tools/pyspice/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.589553 piel-0.0.43/docs/autoapi/piel/tools/pyspice/component/
+-rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-07-13 21:52:16.000000 piel-0.0.43/docs/autoapi/piel/tools/pyspice/component/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-13 21:52:16.000000 piel-0.0.43/docs/autoapi/piel/tools/pyspice/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.589553 piel-0.0.43/docs/autoapi/piel/tools/sax/
+-rw-r--r--   0 runner    (1001) docker     (123)     4883 2023-07-13 21:52:16.000000 piel-0.0.43/docs/autoapi/piel/tools/sax/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.589553 piel-0.0.43/docs/autoapi/piel/tools/sax/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     4983 2023-07-13 21:52:16.000000 piel-0.0.43/docs/autoapi/piel/tools/sax/utils/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.589553 piel-0.0.43/docs/autoapi/piel/visual/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.589553 piel-0.0.43/docs/autoapi/piel/visual/auto_plot_multiple/
+-rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-07-13 21:52:16.000000 piel-0.0.43/docs/autoapi/piel/visual/auto_plot_multiple/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.589553 piel-0.0.43/docs/autoapi/piel/visual/data_conversion/
+-rw-r--r--   0 runner    (1001) docker     (123)     2590 2023-07-13 21:52:16.000000 piel-0.0.43/docs/autoapi/piel/visual/data_conversion/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3697 2023-07-13 21:52:16.000000 piel-0.0.43/docs/autoapi/piel/visual/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4143 2023-07-13 21:52:16.000000 piel-0.0.43/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-13 21:52:16.000000 piel-0.0.43/docs/contributing.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.573553 piel-0.0.43/docs/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.573553 piel-0.0.43/docs/examples/designs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.573553 piel-0.0.43/docs/examples/designs/simple_design/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.573553 piel-0.0.43/docs/examples/designs/simple_design/simple_design/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.589553 piel-0.0.43/docs/examples/designs/simple_design/simple_design/tb/
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-07-13 21:52:16.000000 piel-0.0.43/docs/examples/designs/simple_design/simple_design/tb/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.589553 piel-0.0.43/docs/examples/designs/simple_design/simple_design/tb/default/
+-rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-07-13 21:52:16.000000 piel-0.0.43/docs/examples/designs/simple_design/simple_design/tb/default/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-07-13 21:52:16.000000 piel-0.0.43/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-13 21:52:16.000000 piel-0.0.43/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-07-13 21:52:16.000000 piel-0.0.43/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.573553 piel-0.0.43/docs/sections/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.589553 piel-0.0.43/docs/sections/about/
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-07-13 21:52:16.000000 piel-0.0.43/docs/sections/about/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-13 21:52:16.000000 piel-0.0.43/docs/sections/about/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.589553 piel-0.0.43/docs/sections/codesign/
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-13 21:52:16.000000 piel-0.0.43/docs/sections/codesign/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.593553 piel-0.0.43/docs/sections/components/
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-07-13 21:52:16.000000 piel-0.0.43/docs/sections/components/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.593553 piel-0.0.43/docs/sections/environment/
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-07-13 21:52:16.000000 piel-0.0.43/docs/sections/environment/developer_docker_configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-07-13 21:52:16.000000 piel-0.0.43/docs/sections/environment/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-07-13 21:52:16.000000 piel-0.0.43/docs/sections/environment/setup.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.593553 piel-0.0.43/docs/sections/microservices/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.593553 piel-0.0.43/docs/sections/microservices/dependencies/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-13 21:52:16.000000 piel-0.0.43/docs/sections/microservices/dependencies/cocotb.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-07-13 21:52:16.000000 piel-0.0.43/docs/sections/microservices/dependencies/gdsfactory.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-13 21:52:16.000000 piel-0.0.43/docs/sections/microservices/dependencies/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-07-13 21:52:16.000000 piel-0.0.43/docs/sections/microservices/dependencies/openlane.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-07-13 21:52:16.000000 piel-0.0.43/docs/sections/microservices/dependencies/principle.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-07-13 21:52:16.000000 piel-0.0.43/docs/sections/microservices/dependencies/pyspice.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3007 2023-07-13 21:52:16.000000 piel-0.0.43/docs/sections/microservices/dependencies/sax.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-13 21:52:16.000000 piel-0.0.43/docs/sections/microservices/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.593553 piel-0.0.43/docs/sections/microservices/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-13 21:52:16.000000 piel-0.0.43/docs/sections/microservices/integration/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-07-13 21:52:16.000000 piel-0.0.43/docs/sections/microservices/integration/sax_qutip.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.593553 piel-0.0.43/docs/sections/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-07-13 21:52:16.000000 piel-0.0.43/docs/sections/models/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.593553 piel-0.0.43/piel/
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-07-13 21:52:16.000000 piel-0.0.43/piel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-07-13 21:52:16.000000 piel-0.0.43/piel/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.593553 piel-0.0.43/piel/components/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:16.000000 piel-0.0.43/piel/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-07-13 21:52:16.000000 piel-0.0.43/piel/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-07-13 21:52:16.000000 piel-0.0.43/piel/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-07-13 21:52:16.000000 piel-0.0.43/piel/file_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11207 2023-07-13 21:52:16.000000 piel-0.0.43/piel/file_system.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.597553 piel-0.0.43/piel/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-13 21:52:16.000000 piel-0.0.43/piel/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-13 21:52:16.000000 piel-0.0.43/piel/integration/cocotb_sax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-07-13 21:52:16.000000 piel-0.0.43/piel/integration/gdsfactory_openlane.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.597553 piel-0.0.43/piel/integration/gdsfactory_pyspice/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-13 21:52:16.000000 piel-0.0.43/piel/integration/gdsfactory_pyspice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5342 2023-07-13 21:52:16.000000 piel-0.0.43/piel/integration/gdsfactory_pyspice/conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7777 2023-07-13 21:52:16.000000 piel-0.0.43/piel/integration/gdsfactory_pyspice/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-07-13 21:52:16.000000 piel-0.0.43/piel/integration/gdsfactory_pyspice/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-13 21:52:16.000000 piel-0.0.43/piel/integration/pyspice_sax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-07-13 21:52:16.000000 piel-0.0.43/piel/integration/sax_qutip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-07-13 21:52:16.000000 piel-0.0.43/piel/integration/sax_thewalrus.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.597553 piel-0.0.43/piel/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-07-13 21:52:16.000000 piel-0.0.43/piel/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.597553 piel-0.0.43/piel/models/frequency/
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-07-13 21:52:16.000000 piel-0.0.43/piel/models/frequency/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-07-13 21:52:16.000000 piel-0.0.43/piel/models/frequency/all.py
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-07-13 21:52:16.000000 piel-0.0.43/piel/models/frequency/defaults.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.597553 piel-0.0.43/piel/models/frequency/electrical/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:16.000000 piel-0.0.43/piel/models/frequency/electrical/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.597553 piel-0.0.43/piel/models/frequency/electro_optic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:16.000000 piel-0.0.43/piel/models/frequency/electro_optic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-13 21:52:16.000000 piel-0.0.43/piel/models/frequency/electro_optic/ideal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.597553 piel-0.0.43/piel/models/frequency/electronic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:16.000000 piel-0.0.43/piel/models/frequency/electronic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.597553 piel-0.0.43/piel/models/frequency/opto_electronic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:16.000000 piel-0.0.43/piel/models/frequency/opto_electronic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.597553 piel-0.0.43/piel/models/frequency/photonic/
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-13 21:52:16.000000 piel-0.0.43/piel/models/frequency/photonic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-07-13 21:52:16.000000 piel-0.0.43/piel/models/frequency/photonic/coupler_simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-07-13 21:52:16.000000 piel-0.0.43/piel/models/frequency/photonic/directional_coupler_length.py
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-07-13 21:52:16.000000 piel-0.0.43/piel/models/frequency/photonic/directional_coupler_real.py
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-07-13 21:52:16.000000 piel-0.0.43/piel/models/frequency/photonic/directional_coupler_simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-07-13 21:52:16.000000 piel-0.0.43/piel/models/frequency/photonic/grating_coupler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-07-13 21:52:16.000000 piel-0.0.43/piel/models/frequency/photonic/mmi1x2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-07-13 21:52:16.000000 piel-0.0.43/piel/models/frequency/photonic/mmi2x2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-07-13 21:52:16.000000 piel-0.0.43/piel/models/frequency/photonic/straight_waveguide.py
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-07-13 21:52:16.000000 piel-0.0.43/piel/models/frequency/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.597553 piel-0.0.43/piel/models/logic/
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-07-13 21:52:16.000000 piel-0.0.43/piel/models/logic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.601554 piel-0.0.43/piel/models/logic/electrical/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:16.000000 piel-0.0.43/piel/models/logic/electrical/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.601554 piel-0.0.43/piel/models/logic/electro_optic/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-13 21:52:16.000000 piel-0.0.43/piel/models/logic/electro_optic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2964 2023-07-13 21:52:16.000000 piel-0.0.43/piel/models/logic/electro_optic/signal_mapping.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.601554 piel-0.0.43/piel/models/logic/electronic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:16.000000 piel-0.0.43/piel/models/logic/electronic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.601554 piel-0.0.43/piel/models/logic/opto_electronic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:16.000000 piel-0.0.43/piel/models/logic/opto_electronic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.601554 piel-0.0.43/piel/models/logic/photonic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:16.000000 piel-0.0.43/piel/models/logic/photonic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.601554 piel-0.0.43/piel/models/physical/
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-07-13 21:52:16.000000 piel-0.0.43/piel/models/physical/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.601554 piel-0.0.43/piel/models/physical/electrical/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:16.000000 piel-0.0.43/piel/models/physical/electrical/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:16.000000 piel-0.0.43/piel/models/physical/electrical/cable.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.601554 piel-0.0.43/piel/models/physical/electro_optic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:16.000000 piel-0.0.43/piel/models/physical/electro_optic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-07-13 21:52:16.000000 piel-0.0.43/piel/models/physical/electro_optic/basic_heater.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.601554 piel-0.0.43/piel/models/physical/electronic/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-13 21:52:16.000000 piel-0.0.43/piel/models/physical/electronic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.601554 piel-0.0.43/piel/models/physical/electronic/spice/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-13 21:52:16.000000 piel-0.0.43/piel/models/physical/electronic/spice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-13 21:52:16.000000 piel-0.0.43/piel/models/physical/electronic/spice/capacitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-07-13 21:52:16.000000 piel-0.0.43/piel/models/physical/electronic/spice/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-07-13 21:52:16.000000 piel-0.0.43/piel/models/physical/electronic/spice/resistor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-07-13 21:52:16.000000 piel-0.0.43/piel/models/physical/geometry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.601554 piel-0.0.43/piel/models/physical/opto_electronic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:16.000000 piel-0.0.43/piel/models/physical/opto_electronic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.601554 piel-0.0.43/piel/models/physical/photonic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:16.000000 piel-0.0.43/piel/models/physical/photonic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-07-13 21:52:16.000000 piel-0.0.43/piel/models/physical/thermal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-13 21:52:16.000000 piel-0.0.43/piel/models/physical/units.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.601554 piel-0.0.43/piel/models/transient/
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-07-13 21:52:16.000000 piel-0.0.43/piel/models/transient/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.601554 piel-0.0.43/piel/models/transient/electrical/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:16.000000 piel-0.0.43/piel/models/transient/electrical/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.601554 piel-0.0.43/piel/models/transient/electro_optic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:16.000000 piel-0.0.43/piel/models/transient/electro_optic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.601554 piel-0.0.43/piel/models/transient/electronic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:16.000000 piel-0.0.43/piel/models/transient/electronic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.601554 piel-0.0.43/piel/models/transient/opto_electronic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:16.000000 piel-0.0.43/piel/models/transient/opto_electronic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.601554 piel-0.0.43/piel/models/transient/photonic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:16.000000 piel-0.0.43/piel/models/transient/photonic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:16.000000 piel-0.0.43/piel/models/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3928 2023-07-13 21:52:16.000000 piel-0.0.43/piel/parametric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-07-13 21:52:16.000000 piel-0.0.43/piel/project_structure.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.601554 piel-0.0.43/piel/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-13 21:52:16.000000 piel-0.0.43/piel/tools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.601554 piel-0.0.43/piel/tools/cocotb/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-13 21:52:16.000000 piel-0.0.43/piel/tools/cocotb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6178 2023-07-13 21:52:16.000000 piel-0.0.43/piel/tools/cocotb/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-07-13 21:52:16.000000 piel-0.0.43/piel/tools/cocotb/data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.605553 piel-0.0.43/piel/tools/gdsfactory/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-13 21:52:16.000000 piel-0.0.43/piel/tools/gdsfactory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4636 2023-07-13 21:52:16.000000 piel-0.0.43/piel/tools/gdsfactory/netlist.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.605553 piel-0.0.43/piel/tools/openlane/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-13 21:52:16.000000 piel-0.0.43/piel/tools/openlane/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-07-13 21:52:16.000000 piel-0.0.43/piel/tools/openlane/migrate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.605553 piel-0.0.43/piel/tools/openlane/parse/
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-07-13 21:52:16.000000 piel-0.0.43/piel/tools/openlane/parse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-07-13 21:52:16.000000 piel-0.0.43/piel/tools/openlane/parse/run_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10719 2023-07-13 21:52:16.000000 piel-0.0.43/piel/tools/openlane/parse/sta_rpt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-07-13 21:52:16.000000 piel-0.0.43/piel/tools/openlane/parse/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-07-13 21:52:16.000000 piel-0.0.43/piel/tools/openlane/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10697 2023-07-13 21:52:16.000000 piel-0.0.43/piel/tools/openlane/v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-07-13 21:52:16.000000 piel-0.0.43/piel/tools/openlane/v2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.605553 piel-0.0.43/piel/tools/pyspice/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:16.000000 piel-0.0.43/piel/tools/pyspice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-07-13 21:52:16.000000 piel-0.0.43/piel/tools/pyspice/component.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.605553 piel-0.0.43/piel/tools/sax/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-13 21:52:16.000000 piel-0.0.43/piel/tools/sax/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7256 2023-07-13 21:52:16.000000 piel-0.0.43/piel/tools/sax/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.605553 piel-0.0.43/piel/visual/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-13 21:52:16.000000 piel-0.0.43/piel/visual/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3000 2023-07-13 21:52:16.000000 piel-0.0.43/piel/visual/auto_plot_multiple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4315 2023-07-13 21:52:16.000000 piel-0.0.43/piel/visual/data_conversion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.593553 piel-0.0.43/piel.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3951 2023-07-13 21:52:33.000000 piel-0.0.43/piel.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9705 2023-07-13 21:52:33.000000 piel-0.0.43/piel.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 21:52:33.000000 piel-0.0.43/piel.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-13 21:52:33.000000 piel-0.0.43/piel.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 21:52:33.000000 piel-0.0.43/piel.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-07-13 21:52:33.000000 piel-0.0.43/piel.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-13 21:52:33.000000 piel-0.0.43/piel.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-07-13 21:52:33.609554 piel-0.0.43/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-07-13 21:52:16.000000 piel-0.0.43/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.605553 piel-0.0.43/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-13 21:52:16.000000 piel-0.0.43/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.605553 piel-0.0.43/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)     5910 2023-07-13 21:52:16.000000 piel-0.0.43/tests/integration/test_gdsfactory_netlist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-07-13 21:52:16.000000 piel-0.0.43/tests/integration/test_gdsfactory_netlist_to_pyspice.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.577553 piel-0.0.43/tests/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.577553 piel-0.0.43/tests/models/logic/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.605553 piel-0.0.43/tests/models/logic/electro_optic/
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-07-13 21:52:16.000000 piel-0.0.43/tests/models/logic/electro_optic/test_signal_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-07-13 21:52:16.000000 piel-0.0.43/tests/test_piel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.605553 piel-0.0.43/tests/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:16.000000 piel-0.0.43/tests/tools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.605553 piel-0.0.43/tests/tools/gdsfactory/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-13 21:52:16.000000 piel-0.0.43/tests/tools/gdsfactory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-07-13 21:52:16.000000 piel-0.0.43/tests/tools/gdsfactory/test_netlist.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.605553 piel-0.0.43/tests/tools/sax/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:16.000000 piel-0.0.43/tests/tools/sax/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3773 2023-07-13 21:52:16.000000 piel-0.0.43/tests/tools/sax/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:52:33.605553 piel-0.0.43/tests/visual/
+-rw-r--r--   0 runner    (1001) docker     (123)     9100 2023-07-13 21:52:16.000000 piel-0.0.43/tests/visual/test_data_conversion.py
```

### Comparing `piel-0.0.41/CONTRIBUTING.rst` & `piel-0.0.43/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `piel-0.0.41/LICENSE` & `piel-0.0.43/LICENSE`

 * *Files identical despite different names*

### Comparing `piel-0.0.41/PKG-INFO` & `piel-0.0.43/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: piel
-Version: 0.0.41
-Summary: Photonic and electronic co-simulation system design tools interfaced with open-source design software like GDSFactory and OpenROAD.
+Version: 0.0.43
+Summary: Photonic Integrated Electronics: microservices to codesign photonics, electronics, communications, quantum, and more.
 Home-page: https://github.com/daquintero/piel
 Author: Dario Quintero
 Author-email: darioaquintero@gmail.com
 License: MIT license
 Keywords: piel
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
@@ -16,48 +16,70 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: develop
 License-File: LICENSE
 
-# `piel` - Photonic and Integrated ELectronic tools
-[![PyPI Version](https://img.shields.io/pypi/v/piel.svg)](https://pypi.python.org/pypi/piel)
-[![Build Status](https://img.shields.io/travis/daquintero/piel.svg)](https://travis-ci.com/daquintero/piel)
-[![Documentation Status](https://readthedocs.org/projects/piel/badge/?version=latest)](https://piel.readthedocs.io/en/latest/?version=latest)
-[![Updates](https://pyup.io/repos/github/daquintero/piel/shield.svg)](https://pyup.io/repos/github/daquintero/piel/)
+**P**\hotonic **I**\ntegrated **EL**\ectronics
+===============================================
 
-Microservices to codesign photonics, electronics, quantum, and more.
+|PyPI Version| |Build Status| |Documentation Status| |Updates|
 
-- Free software: MIT license
-- Documentation: [https://piel.readthedocs.io](https://piel.readthedocs.io)
+Microservices to codesign photonics, electronics, communications,
+quantum, and more.
 
-## Target functionality
-* Co-simulation and optimisation between integrated photonic and electronic chip design.
-* System interconnection modelling in multiple environments.
-* Individual and interposer design integration.
-* Multi-domain electronics and photonics component models.
-* Quantum models of physical circuitry
+-  Free software: MIT license
+-  Documentation: https://piel.readthedocs.io
 
-`piel` aims to provide an integrated workflow to co-design photonics and electronics, classically and quantum. It does not aim to replace the individual functionality of each design tool, but rather provide a glue to easily connect them all together and extract the system performance.
+Target functionality
+--------------------
 
-## Examples
+-  Co-simulation and optimisation between integrated photonic and
+   electronic chip design.
+-  System interconnection modelling in multiple domains.
+-  Chip and interposer design integration.
+-  Component models translation library between simulation tools.
+-  Quantum models of physical circuitry.
 
-Follow the many [examples in the documentation](https://piel.readthedocs.io/en/stable/examples.html).
+``piel`` aims to provide an integrated workflow to co-design photonics
+and electronics, classically and quantum. It does not aim to replace the
+individual functionality of each design tool, but rather provide a glue
+to easily connect them all together and extract the system performance.
 
-## Microservices Toolset
-This package provides interconnection functions to easily co-design microelectronics through the functionality of the [IIC-OSIC-TOOLS](https://github.com/iic-jku/iic-osic-tools) and photonics via [GDSFactory](https://github.com/gdsfactory/gdsfactory).
+Examples
+--------
 
-Some existing microservice dependency integrations are:
-* [cocotb](https://github.com/cocotb/cocotb) - a coroutine based cosimulation library for writing VHDL and Verilog testbenches in Python.
-* [GDSFactory](https://github.com/gdsfactory/gdsfactory) - An open source platform for end to-end photonic chip design and validation
-* [OpenLane v1](https://github.com/The-OpenROAD-Project/OpenLane) - an automated RTL to GDSII flow based on several components including OpenROAD, Yosys, Magic, Netgen and custom methodology scripts for design exploration and optimization
-* [pyspice](https://github.com/PySpice-org/PySpice) - Simulate electronic circuit using Python and the Ngspice / Xyce simulators
-* [sax](https://github.com/flaport/sax) - S-parameter based frequency domain circuit simulations and optimizations using JAX.
-* [qutip](https://github.com/qutip/qutip) - QuTiP: Quantum Toolbox in Python
+Follow the many `examples in the documentation <https://piel.readthedocs.io/en/stable/examples.html>`__.
+
+Microservices Toolset
+---------------------
 
-## Environment Requirements
-* Please install the Linux Docker environment provided by [IIC-OSIC-TOOLS](https://github.com/iic-jku/iic-osic-tools).
+This package provides interconnection functions to easily co-design
+microelectronics through the functionality of the
+`IIC-OSIC-TOOLS <https://github.com/iic-jku/iic-osic-tools>`__ and
+photonics via `GDSFactory <https://github.com/gdsfactory/gdsfactory>`__.
 
+Some existing microservice dependency integrations are:
 
-## Contribution
-If you feel dedicated enough to become a project maintainer, or just want to do a single contributor, let's do this together!
+* `cocotb <https://github.com/cocotb/cocotb>`__ - a coroutine based cosimulation library for writing VHDL and Verilog testbenches in Python.
+* `GDSFactory <https://github.com/gdsfactory/gdsfactory>`__ - An open source platform for end to-end photonic chip design and validation
+* `OpenLane v1 <https://github.com/The-OpenROAD-Project/OpenLane>`__ - an automated RTL to GDSII flow based on several components including OpenROAD, Yosys, Magic, Netgen and custom methodology scripts for design exploration and optimization
+* `pyspice <https://github.com/PySpice-org/PySpice>`__ - Simulate electronic circuit using Python and the Ngspice / Xyce simulators
+* `sax <https://github.com/flaport/sax>`__ - S-parameter based frequency domain circuit simulations and optimizations using JAX.
+* `thewalrus <https://github.com/XanaduAI/thewalrus>`__ -A library for the calculation of hafnians, Hermite polynomials and Gaussian boson sampling.
+* `qutip <https://github.com/qutip/qutip>`__ - QuTiP: Quantum Toolbox in Python
+
+Contribution
+------------
+
+If you feel dedicated enough to become a project maintainer, or just
+want to do a single contribution, let's do this together!
+
+.. |PyPI Version| image:: https://img.shields.io/pypi/v/piel.svg
+   :target: https://pypi.python.org/pypi/piel
+.. |Build Status| image:: https://img.shields.io/travis/daquintero/piel.svg
+   :target: https://travis-ci.com/daquintero/piel
+.. |Documentation Status| image:: https://readthedocs.org/projects/piel/badge/?version=latest
+   :target: https://piel.readthedocs.io/en/latest/?version=latest
+.. |Updates| image:: https://pyup.io/repos/github/daquintero/piel/shield.svg
+   :target: https://pyup.io/repos/github/daquintero/piel/
```

### Comparing `piel-0.0.41/README.md` & `piel-0.0.43/README.rst`

 * *Files 22% similar despite different names*

```diff
@@ -1,41 +1,63 @@
-# `piel` - Photonic and Integrated ELectronic tools
-[![PyPI Version](https://img.shields.io/pypi/v/piel.svg)](https://pypi.python.org/pypi/piel)
-[![Build Status](https://img.shields.io/travis/daquintero/piel.svg)](https://travis-ci.com/daquintero/piel)
-[![Documentation Status](https://readthedocs.org/projects/piel/badge/?version=latest)](https://piel.readthedocs.io/en/latest/?version=latest)
-[![Updates](https://pyup.io/repos/github/daquintero/piel/shield.svg)](https://pyup.io/repos/github/daquintero/piel/)
+**P**\hotonic **I**\ntegrated **EL**\ectronics
+===============================================
 
-Microservices to codesign photonics, electronics, quantum, and more.
+|PyPI Version| |Build Status| |Documentation Status| |Updates|
 
-- Free software: MIT license
-- Documentation: [https://piel.readthedocs.io](https://piel.readthedocs.io)
+Microservices to codesign photonics, electronics, communications,
+quantum, and more.
 
-## Target functionality
-* Co-simulation and optimisation between integrated photonic and electronic chip design.
-* System interconnection modelling in multiple environments.
-* Individual and interposer design integration.
-* Multi-domain electronics and photonics component models.
-* Quantum models of physical circuitry
+-  Free software: MIT license
+-  Documentation: https://piel.readthedocs.io
 
-`piel` aims to provide an integrated workflow to co-design photonics and electronics, classically and quantum. It does not aim to replace the individual functionality of each design tool, but rather provide a glue to easily connect them all together and extract the system performance.
+Target functionality
+--------------------
 
-## Examples
+-  Co-simulation and optimisation between integrated photonic and
+   electronic chip design.
+-  System interconnection modelling in multiple domains.
+-  Chip and interposer design integration.
+-  Component models translation library between simulation tools.
+-  Quantum models of physical circuitry.
 
-Follow the many [examples in the documentation](https://piel.readthedocs.io/en/stable/examples.html).
+``piel`` aims to provide an integrated workflow to co-design photonics
+and electronics, classically and quantum. It does not aim to replace the
+individual functionality of each design tool, but rather provide a glue
+to easily connect them all together and extract the system performance.
 
-## Microservices Toolset
-This package provides interconnection functions to easily co-design microelectronics through the functionality of the [IIC-OSIC-TOOLS](https://github.com/iic-jku/iic-osic-tools) and photonics via [GDSFactory](https://github.com/gdsfactory/gdsfactory).
+Examples
+--------
 
-Some existing microservice dependency integrations are:
-* [cocotb](https://github.com/cocotb/cocotb) - a coroutine based cosimulation library for writing VHDL and Verilog testbenches in Python.
-* [GDSFactory](https://github.com/gdsfactory/gdsfactory) - An open source platform for end to-end photonic chip design and validation
-* [OpenLane v1](https://github.com/The-OpenROAD-Project/OpenLane) - an automated RTL to GDSII flow based on several components including OpenROAD, Yosys, Magic, Netgen and custom methodology scripts for design exploration and optimization
-* [pyspice](https://github.com/PySpice-org/PySpice) - Simulate electronic circuit using Python and the Ngspice / Xyce simulators
-* [sax](https://github.com/flaport/sax) - S-parameter based frequency domain circuit simulations and optimizations using JAX.
-* [qutip](https://github.com/qutip/qutip) - QuTiP: Quantum Toolbox in Python
+Follow the many `examples in the documentation <https://piel.readthedocs.io/en/stable/examples.html>`__.
+
+Microservices Toolset
+---------------------
 
-## Environment Requirements
-* Please install the Linux Docker environment provided by [IIC-OSIC-TOOLS](https://github.com/iic-jku/iic-osic-tools).
+This package provides interconnection functions to easily co-design
+microelectronics through the functionality of the
+`IIC-OSIC-TOOLS <https://github.com/iic-jku/iic-osic-tools>`__ and
+photonics via `GDSFactory <https://github.com/gdsfactory/gdsfactory>`__.
 
+Some existing microservice dependency integrations are:
 
-## Contribution
-If you feel dedicated enough to become a project maintainer, or just want to do a single contributor, let's do this together!
+* `cocotb <https://github.com/cocotb/cocotb>`__ - a coroutine based cosimulation library for writing VHDL and Verilog testbenches in Python.
+* `GDSFactory <https://github.com/gdsfactory/gdsfactory>`__ - An open source platform for end to-end photonic chip design and validation
+* `OpenLane v1 <https://github.com/The-OpenROAD-Project/OpenLane>`__ - an automated RTL to GDSII flow based on several components including OpenROAD, Yosys, Magic, Netgen and custom methodology scripts for design exploration and optimization
+* `pyspice <https://github.com/PySpice-org/PySpice>`__ - Simulate electronic circuit using Python and the Ngspice / Xyce simulators
+* `sax <https://github.com/flaport/sax>`__ - S-parameter based frequency domain circuit simulations and optimizations using JAX.
+* `thewalrus <https://github.com/XanaduAI/thewalrus>`__ -A library for the calculation of hafnians, Hermite polynomials and Gaussian boson sampling.
+* `qutip <https://github.com/qutip/qutip>`__ - QuTiP: Quantum Toolbox in Python
+
+Contribution
+------------
+
+If you feel dedicated enough to become a project maintainer, or just
+want to do a single contribution, let's do this together!
+
+.. |PyPI Version| image:: https://img.shields.io/pypi/v/piel.svg
+   :target: https://pypi.python.org/pypi/piel
+.. |Build Status| image:: https://img.shields.io/travis/daquintero/piel.svg
+   :target: https://travis-ci.com/daquintero/piel
+.. |Documentation Status| image:: https://readthedocs.org/projects/piel/badge/?version=latest
+   :target: https://piel.readthedocs.io/en/latest/?version=latest
+.. |Updates| image:: https://pyup.io/repos/github/daquintero/piel/shield.svg
+   :target: https://pyup.io/repos/github/daquintero/piel/
```

### Comparing `piel-0.0.41/docs/Makefile` & `piel-0.0.43/docs/Makefile`

 * *Files identical despite different names*

### Comparing `piel-0.0.41/docs/autoapi/piel/config/index.rst` & `piel-0.0.43/docs/autoapi/piel/config/index.rst`

 * *Files identical despite different names*

### Comparing `piel-0.0.41/docs/autoapi/piel/file_conversion/index.rst` & `piel-0.0.43/docs/autoapi/piel/file_conversion/index.rst`

 * *Files identical despite different names*

### Comparing `piel-0.0.41/docs/autoapi/piel/file_system/index.rst` & `piel-0.0.43/docs/autoapi/piel/file_system/index.rst`

 * *Files identical despite different names*

### Comparing `piel-0.0.41/docs/autoapi/piel/index.rst` & `piel-0.0.43/docs/autoapi/piel/index.rst`

 * *Files 10% similar despite different names*

```diff
@@ -57,14 +57,20 @@
    piel.permit_script_execution
    piel.setup_example_design
    piel.read_json
    piel.return_path
    piel.run_script
    piel.write_script
    piel.create_gdsfactory_component_from_openlane
+   piel.gdsfactory_netlist_to_pyspice
+   piel.spice_netlist_to_pyspice_circuit
+   piel.gdsfactory_netlist_to_spice_netlist
+   piel.sax_to_s_parameters_standard_matrix
+   piel.unitary_permanent
+   piel.sax_circuit_permanent
    piel.sax_to_ideal_qutip_unitary
    piel.standard_s_parameters_to_ideal_qutip_unitary
    piel.single_parameter_sweep
    piel.multi_parameter_sweep
    piel.check_cocotb_testbench_exists
    piel.configure_cocotb_simulation
    piel.run_cocotb_simulation
@@ -81,18 +87,18 @@
    piel.configure_parametric_designs_openlane_v1
    piel.configure_flow_script_openlane_v1
    piel.create_parametric_designs_openlane_v1
    piel.get_design_directory_from_root_openlane_v1
    piel.get_latest_version_root_openlane_v1
    piel.read_configuration_openlane_v1
    piel.write_configuration_openlane_v1
-   piel.get_all_timing_sta_files
-   piel.get_all_power_sta_files
    piel.filter_timing_sta_files
    piel.filter_power_sta_files
+   piel.get_all_timing_sta_files
+   piel.get_all_power_sta_files
    piel.calculate_max_frame_amount
    piel.calculate_propagation_delay_from_file
    piel.calculate_propagation_delay_from_timing_data
    piel.configure_timing_data_rows
    piel.configure_frame_id
    piel.filter_timing_data_by_net_name_and_type
    piel.get_frame_meta_data
@@ -330,14 +336,201 @@
    :param v1: If True, it will import the design from the OpenLane v1 configuration.
    :type v1: bool
 
    :returns: GDSFactory component.
    :rtype: component(gf.Component)
 
 
+.. py:function:: gdsfactory_netlist_to_pyspice(gdsfactory_netlist: dict, return_raw_spice: bool = False)
+
+   This function converts a GDSFactory electrical netlist into a standard PySpice configuration. It follows the same
+   principle as the `sax` circuit composition. It returns a PySpice circuit and can return it in raw_spice form if
+   necessary.
+
+   Each GDSFactory netlist has a set of instances, each with a corresponding model, and each instance with a given
+   set of geometrical settings that can be applied to each particular model. We know the type of SPICE model from
+   the instance model we provides.
+
+   We know that the gdsfactory has a set of instances, and we can map unique models via sax through our own
+   composition circuit. Write the SPICE component based on the model into a total circuit representation in string
+   from the reshaped gdsfactory dictionary into our own structure.
+
+
+.. py:function:: spice_netlist_to_pyspice_circuit(spice_netlist: dict)
+
+   This function converts a SPICE netlist into a PySpice circuit.
+
+   # TODO implement validators
+
+
+.. py:function:: gdsfactory_netlist_to_spice_netlist(gdsfactory_netlist: dict, models=None)
+
+   This function maps the connections of a netlist to a node that can be used in a SPICE netlist. SPICE netlists are
+   in the form of:
+
+   .. code-block::
+
+       RXXXXXXX N1 N2 <VALUE> <MNAME> <L=LENGTH> <W=WIDTH> <TEMP=T>
+
+   This means that every instance, is an electrical type, and we define the two particular nodes in which it is
+   connected. This means we need to convert the gdsfactory dictionary netlist into a form that allows us to map the
+   connectivity for every instance. Then we can define that as a line of the SPICE netlist with a particular
+   electrical model. For passives this works fine when it's a two port network such as sources, or electrical
+   elements. However, non-passive elements like transistors have three ports or more which are provided in an ordered form.
+
+   This means that the order of translations is as follows:
+
+   .. code-block::
+
+       1. Extract all instances and required models from the netlist
+       2. Verify that the models have been provided. Each model describes the type of component this is, how many ports it requires and so on.
+       3. Map the connections to each instance port as part of the instance dictionary.
+
+   We should get as an output a dictionary in the structure:
+
+   .. code-block::
+
+       {
+           instance_1: {
+               ...
+               "connections": [('straight_1,e1', 'taper_1,e2'),
+                               ('straight_1,e2', 'taper_2,e2')],
+               'spice_nets': {'e1': 'straight_1__e1___taper_1__e2',
+                       'e2': 'straight_1__e2___taper_2__e2'},
+               'spice_model': <function piel.models.physical.electronic.spice.resistor.basic_resistor()>},
+           }
+           ...
+       }
+
+
+.. py:function:: sax_to_s_parameters_standard_matrix(sax_input: sax.SType, input_ports_order: tuple | None = None) -> tuple
+
+   A ``sax`` S-parameter SDict is provided as a dictionary of tuples with (port0, port1) as the key. This
+   determines the direction of the scattering relationship. It means that the number of terms in an S-parameter
+   matrix is the number of ports squared.
+
+   In order to generalise, this function returns both the S-parameter matrices and the indexing ports based on the
+   amount provided. In terms of computational speed, we definitely would like this function to be algorithmically
+   very fast. For now, I will write a simple python implementation and optimise in the future.
+
+   It is possible to see the `sax` SDense notation equivalence here:
+   https://flaport.github.io/sax/nbs/08_backends.html
+
+   .. code-block:: python
+
+       import jax.numpy as jnp
+       from sax.core import SDense
+
+       # Directional coupler SDense representation
+       dc_sdense: SDense = (
+           jnp.array([[0, 0, τ, κ], [0, 0, κ, τ], [τ, κ, 0, 0], [κ, τ, 0, 0]]),
+           {"in0": 0, "in1": 1, "out0": 2, "out1": 3},
+       )
+
+
+       # Directional coupler SDict representation
+       # Taken from https://flaport.github.io/sax/nbs/05_models.html
+       def coupler(*, coupling: float = 0.5) -> SDict:
+           kappa = coupling**0.5
+           tau = (1 - coupling) ** 0.5
+           sdict = reciprocal(
+               {
+                   ("in0", "out0"): tau,
+                   ("in0", "out1"): 1j * kappa,
+                   ("in1", "out0"): 1j * kappa,
+                   ("in1", "out1"): tau,
+               }
+           )
+           return sdict
+
+   If we were to relate the mapping accordingly based on the ports indexes, a S-Parameter matrix in the form of
+   :math:`S_{(output,i),(input,i)}` would be:
+
+   .. math::
+
+       S = \begin{bmatrix}
+               S_{00} & S_{10} \\
+               S_{01} & S_{11} \\
+           \end{bmatrix} =
+           \begin{bmatrix}
+           \tau & j \kappa \\
+           j \kappa & \tau \\
+           \end{bmatrix}
+
+   Note that the standard S-parameter and hence unitary representation is in the form of:
+
+   .. math::
+
+       S = \begin{bmatrix}
+               S_{00} & S_{01} \\
+               S_{10} & S_{11} \\
+           \end{bmatrix}
+
+
+   .. math::
+
+       \begin{bmatrix}
+           b_{1} \\
+           \vdots \\
+           b_{n}
+       \end{bmatrix}
+       =
+       \begin{bmatrix}
+           S_{11} & \dots & S_{1n} \\
+           \vdots & \ddots & \vdots \\
+           S_{n1} & \dots & S_{nn}
+       \end{bmatrix}
+       \begin{bmatrix}
+           a_{1} \\
+           \vdots \\
+           a_{n}
+       \end{bmatrix}
+
+   TODO check with Floris, does this mean we need to transpose the matrix?
+
+   :param sax_input: The sax S-parameter dictionary.
+   :type sax_input: sax.SType
+   :param input_ports_order: The ports order tuple containing the names and order of the input ports.
+   :type input_ports_order: tuple
+
+   :returns: The S-parameter matrix and the input ports index tuple in the standard S-parameter notation.
+   :rtype: tuple
+
+
+.. py:function:: unitary_permanent(unitary_matrix: numpy.ndarray) -> tuple
+
+   The permanent of a unitary is used to determine the state probability of combinatorial Gaussian boson samping systems.
+
+   ``thewalrus`` Ryser's algorithm permananet implementation is described here: https://the-walrus.readthedocs.io/en/latest/gallery/permanent_tutorial.html
+
+   # TODO maybe implement subroutine if computation is taking forever.
+   # TODO why two outputs? Understand this properly later.
+
+   :param unitary_permanent: The unitary matrix.
+   :type unitary_permanent: np.ndarray
+
+   :returns: The circuit permanent and the time it took to compute it.
+   :rtype: tuple
+
+
+.. py:function:: sax_circuit_permanent(sax_input: sax.SType) -> tuple
+
+   The permanent of a unitary is used to determine the state probability of combinatorial Gaussian boson samping systems.
+
+   ``thewalrus`` Ryser's algorithm permananet implementation is described here: https://the-walrus.readthedocs.io/en/latest/gallery/permanent_tutorial.html
+
+   # TODO maybe implement subroutine if computation is taking forever.
+
+   :param sax_input: The sax S-parameter dictionary.
+   :type sax_input: sax.SType
+
+   :returns: The circuit permanent and the time it took to compute it.
+   :rtype: tuple
+
+
 .. py:function:: sax_to_ideal_qutip_unitary(sax_input: sax.SType)
 
    This function converts the calculated S-parameters into a standard Unitary matrix topology so that the shape and
    dimensions of the matrix can be observed.
 
    I think this means we need to transpose the output of the filtered sax SDense matrix to map it to a QuTip matrix.
    Note that the documentation and formatting of the standard `sax` mapping to a S-parameter standard notation is
@@ -536,21 +729,33 @@
 
 .. py:data:: get_simulation_output_files
 
 
 
 .. py:function:: get_simulation_output_files_from_design(design_directory: piel.config.piel_path_types, extension: str = 'csv')
 
-   # TODO DOCS
+   This function returns a list of all the simulation output files in the design directory.
+
+   :param design_directory: The path to the design directory.
+   :type design_directory: piel_path_types
 
+   :returns: List of all the simulation output files in the design directory.
+   :rtype: output_files (list)
 
-.. py:function:: read_simulation_data(file_path)
+
+.. py:function:: read_simulation_data(file_path: piel.config.piel_path_types)
 
    This function returns a Pandas dataframe that contains all the simulation data outputted from the simulation run.
 
+   :param file_path: The path to the simulation data file.
+   :type file_path: piel_path_types
+
+   :returns: The simulation data in a Pandas dataframe.
+   :rtype: simulation_data (pd.DataFrame)
+
 
 .. py:function:: simple_plot_simulation_data(simulation_data: pandas.DataFrame)
 
 
 .. py:function:: get_input_ports_index(ports_index: dict, sorting_algorithm: Literal[get_input_ports_index.prefix] = 'prefix', prefix: str = 'in') -> tuple
 
    This function returns the input ports of a component. However, input ports may have different sets of prefixes and suffixes. This function implements different sorting algorithms for different ports names. The default algorithm is `prefix`, which sorts the ports by their prefix. The Endianness implementation means that the tuple order is determined according to the last numerical index order of the port numbering.
@@ -580,15 +785,15 @@
    :param prefix: The prefix to use for the sorting algorithm. Defaults to "in".
    :type prefix: str, optional
 
    :returns: The ordered input ports index tuple.
    :rtype: tuple
 
 
-.. py:function:: get_matched_ports_tuple_index(ports_index: dict, selected_ports_tuple: tuple, sorting_algorithm: Literal[get_matched_ports_tuple_index.prefix, selected_ports] = 'prefix', prefix: str = 'in') -> (tuple, tuple)
+.. py:function:: get_matched_ports_tuple_index(ports_index: dict, selected_ports_tuple: Optional[tuple] = None, sorting_algorithm: Literal[get_matched_ports_tuple_index.prefix, selected_ports] = 'prefix', prefix: str = 'in') -> (tuple, tuple)
 
    This function returns the input ports of a component. However, input ports may have different sets of prefixes
    and suffixes. This function implements different sorting algorithms for different ports names. The default
    algorithm is `prefix`, which sorts the ports by their prefix. The Endianness implementation means that the tuple
    order is determined according to the last numerical index order of the port numbering. Returns just a tuple of
    the index.
 
@@ -608,14 +813,16 @@
        get_input_ports_tuple_index(ports_index=raw_ports_index)
 
        # Output
        (0, 5, 6, 7)
 
    :param ports_index: The ports index dictionary.
    :type ports_index: dict
+   :param selected_ports_tuple: The selected ports tuple. Defaults to None.
+   :type selected_ports_tuple: tuple, optional
    :param sorting_algorithm: The sorting algorithm to use. Defaults to "prefix".
    :type sorting_algorithm: Literal["prefix"], optional
    :param prefix: The prefix to use for the sorting algorithm. Defaults to "in".
    :type prefix: str, optional
 
    :returns: The ordered input ports index tuple.
              matched_ports_name_tuple_order(tuple): The ordered input ports name tuple.
@@ -771,36 +978,14 @@
    :type configuration: dict
    :param design_directory: Design directory PATH.
    :type design_directory: str
 
    :returns: None
 
 
-.. py:function:: get_all_timing_sta_files(run_directory)
-
-   This function aims to list and perform analysis on all the relevant files in a particular run between all the corners.
-
-   :param run_directory: The run directory to perform the analysis on. Defaults to None.
-   :type run_directory: str, optional
-
-   :returns: List of all the .rpt files in the run directory.
-   :rtype: timing_sta_files_list (list)
-
-
-.. py:function:: get_all_power_sta_files(run_directory)
-
-   This function aims to list and perform analysis on all the relevant files in a particular run between all the corners.
-
-   :param run_directory: The run directory to perform the analysis on. Defaults to None.
-   :type run_directory: str, optional
-
-   :returns: List of all the .rpt files in the run directory.
-   :rtype: power_sta_files_list (list)
-
-
 .. py:function:: filter_timing_sta_files(file_list)
 
    Filter the timing sta files from the list of files
 
    :param file_list: List containing the file paths
    :type file_list: list
 
@@ -815,14 +1000,36 @@
    :param file_list: List containing the file paths
    :type file_list: list
 
    :returns: List containing the power sta files
    :rtype: power_sta_files (list)
 
 
+.. py:function:: get_all_timing_sta_files(run_directory)
+
+   This function aims to list and perform analysis on all the relevant files in a particular run between all the corners.
+
+   :param run_directory: The run directory to perform the analysis on. Defaults to None.
+   :type run_directory: str, optional
+
+   :returns: List of all the .rpt files in the run directory.
+   :rtype: timing_sta_files_list (list)
+
+
+.. py:function:: get_all_power_sta_files(run_directory)
+
+   This function aims to list and perform analysis on all the relevant files in a particular run between all the corners.
+
+   :param run_directory: The run directory to perform the analysis on. Defaults to None.
+   :type run_directory: str, optional
+
+   :returns: List of all the .rpt files in the run directory.
+   :rtype: power_sta_files_list (list)
+
+
 .. py:function:: calculate_max_frame_amount(file_lines_data: pandas.DataFrame)
 
    Calculate the maximum frame amount based on the frame IDs in the DataFrame
 
    :param file_lines_data: Dataframe containing the file lines
    :type file_lines_data: pd.DataFrame
 
@@ -1162,8 +1369,8 @@
 
 .. py:data:: __email__
    :value: 'darioaquintero@gmail.com'
 
 
 
 .. py:data:: __version__
-   :value: '0.0.40'
+   :value: '0.0.42'
```

### Comparing `piel-0.0.41/docs/autoapi/piel/integration/openlane_gdsfactory_core/index.rst` & `piel-0.0.43/docs/autoapi/piel/integration/gdsfactory_openlane/index.rst`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-:py:mod:`piel.integration.openlane_gdsfactory_core`
-===================================================
+:py:mod:`piel.integration.gdsfactory_openlane`
+==============================================
 
-.. py:module:: piel.integration.openlane_gdsfactory_core
+.. py:module:: piel.integration.gdsfactory_openlane
 
 .. autoapi-nested-parse::
 
    There are a number of ways to generate gdsfactory integration.
 
    It is worth noting that GDSFactory has already the following PDKs installed:
    * SKY130nm https://gdsfactory.github.io/skywater130/
@@ -18,15 +18,15 @@
 
 
 Functions
 ~~~~~~~~~
 
 .. autoapisummary::
 
-   piel.integration.openlane_gdsfactory_core.create_gdsfactory_component_from_openlane
+   piel.integration.gdsfactory_openlane.create_gdsfactory_component_from_openlane
 
 
 
 .. py:function:: create_gdsfactory_component_from_openlane(design_name_v1: str | None = None, design_directory: piel.config.piel_path_types | None = None, run_name: str | None = None, v1: bool = True) -> gdsfactory.Component
 
    This function cretes a gdsfactory layout component that can be included in the network codesign of the device, or that can be used for interconnection codesign.
```

### Comparing `piel-0.0.41/docs/autoapi/piel/integration/sax_qutip/index.rst` & `piel-0.0.43/docs/autoapi/piel/integration/sax_qutip/index.rst`

 * *Files identical despite different names*

### Comparing `piel-0.0.41/docs/autoapi/piel/models/frequency/defaults/index.rst` & `piel-0.0.43/docs/autoapi/piel/models/frequency/defaults/index.rst`

 * *Files identical despite different names*

### Comparing `piel-0.0.41/docs/autoapi/piel/models/frequency/index.rst` & `piel-0.0.43/docs/autoapi/piel/models/frequency/index.rst`

 * *Files identical despite different names*

### Comparing `piel-0.0.41/docs/autoapi/piel/models/frequency/photonic/directional_coupler_length/index.rst` & `piel-0.0.43/docs/autoapi/piel/models/frequency/photonic/directional_coupler_length/index.rst`

 * *Files identical despite different names*

### Comparing `piel-0.0.41/docs/autoapi/piel/models/frequency/photonic/directional_coupler_simple/index.rst` & `piel-0.0.43/docs/autoapi/piel/models/frequency/photonic/directional_coupler_simple/index.rst`

 * *Files identical despite different names*

### Comparing `piel-0.0.41/docs/autoapi/piel/models/frequency/photonic/grating_coupler/index.rst` & `piel-0.0.43/docs/autoapi/piel/models/frequency/photonic/grating_coupler/index.rst`

 * *Files identical despite different names*

### Comparing `piel-0.0.41/docs/autoapi/piel/models/frequency/photonic/index.rst` & `piel-0.0.43/docs/autoapi/piel/models/frequency/photonic/index.rst`

 * *Files identical despite different names*

### Comparing `piel-0.0.41/docs/autoapi/piel/models/frequency/photonic/straight_waveguide/index.rst` & `piel-0.0.43/docs/autoapi/piel/models/frequency/photonic/straight_waveguide/index.rst`

 * *Files identical despite different names*

### Comparing `piel-0.0.41/docs/autoapi/piel/models/frequency/utils/index.rst` & `piel-0.0.43/docs/autoapi/piel/models/frequency/utils/index.rst`

 * *Files identical despite different names*

### Comparing `piel-0.0.41/docs/autoapi/piel/models/logic/electro_optic/index.rst` & `piel-0.0.43/docs/autoapi/piel/models/logic/electro_optic/index.rst`

 * *Files identical despite different names*

### Comparing `piel-0.0.41/docs/autoapi/piel/models/logic/electro_optic/signal_mapping/index.rst` & `piel-0.0.43/docs/autoapi/piel/models/logic/electro_optic/signal_mapping/index.rst`

 * *Files identical despite different names*

### Comparing `piel-0.0.41/docs/autoapi/piel/models/physical/geometry/index.rst` & `piel-0.0.43/docs/autoapi/piel/models/physical/geometry/index.rst`

 * *Files identical despite different names*

### Comparing `piel-0.0.41/docs/autoapi/piel/models/physical/index.rst` & `piel-0.0.43/docs/autoapi/piel/models/physical/index.rst`

 * *Files identical despite different names*

### Comparing `piel-0.0.41/docs/autoapi/piel/models/physical/units/index.rst` & `piel-0.0.43/docs/autoapi/piel/models/physical/units/index.rst`

 * *Files identical despite different names*

### Comparing `piel-0.0.41/docs/autoapi/piel/parametric/index.rst` & `piel-0.0.43/docs/autoapi/piel/parametric/index.rst`

 * *Files identical despite different names*

### Comparing `piel-0.0.41/docs/autoapi/piel/project_structure/index.rst` & `piel-0.0.43/docs/autoapi/piel/project_structure/index.rst`

 * *Files identical despite different names*

### Comparing `piel-0.0.41/docs/autoapi/piel/tools/cocotb/core/index.rst` & `piel-0.0.43/docs/autoapi/piel/tools/cocotb/core/index.rst`

 * *Files 2% similar despite different names*

```diff
@@ -3,18 +3,23 @@
 
 .. py:module:: piel.tools.cocotb.core
 
 .. autoapi-nested-parse::
 
    The objective of this file is to provide the simulation ports and interconnection to consider modelling digital and mixed signal logic.
 
-   The main simulation driver is cocotb, and this generates a set of files that correspond to time-domain digital simulations.
-   The cocotb verification software can also be used to perform mixed signal simulation, and digital data can be inputted as a bitstream into a photonic solver, although the ideal situation would be to have integrated photonic time-domain models alongside the electronic simulation solver, and maybe this is where it will go. It can be assumed that, as is currently, cocotb can interface python with multiple solvers until someone (and I'd love to do this) writes an equivalent python-based or C++ based python time-domain simulation solver.
+   The main simulation driver is cocotb, and this generates a set of files that correspond to time-domain digital
+   simulations. The cocotb verification software can also be used to perform mixed signal simulation, and digital data
+   can be inputted as a bitstream into a photonic solver, although the ideal situation would be to have integrated
+   photonic time-domain models alongside the electronic simulation solver, and maybe this is where it will go. It can be
+   assumed that, as is currently, cocotb can interface python with multiple solvers until someone (and I'd love to do
+   this) writes an equivalent python-based or C++ based python time-domain simulation solver.
 
-   The nice thing about cocotb is that as long as the photonic simulations can be written asyncrhonously, time-domain simulations can be closely integrated or simulated through this verification software.
+   The nice thing about cocotb is that as long as the photonic simulations can be written asynchronously, time-domain
+   simulations can be closely integrated or simulated through this verification software.
 
 
 
 Module Contents
 ---------------
```

### Comparing `piel-0.0.41/docs/autoapi/piel/tools/cocotb/index.rst` & `piel-0.0.43/docs/autoapi/piel/tools/cocotb/index.rst`

 * *Files 12% similar despite different names*

```diff
@@ -119,16 +119,28 @@
 
 .. py:data:: get_simulation_output_files
 
 
 
 .. py:function:: get_simulation_output_files_from_design(design_directory: piel.config.piel_path_types, extension: str = 'csv')
 
-   # TODO DOCS
+   This function returns a list of all the simulation output files in the design directory.
 
+   :param design_directory: The path to the design directory.
+   :type design_directory: piel_path_types
 
-.. py:function:: read_simulation_data(file_path)
+   :returns: List of all the simulation output files in the design directory.
+   :rtype: output_files (list)
+
+
+.. py:function:: read_simulation_data(file_path: piel.config.piel_path_types)
 
    This function returns a Pandas dataframe that contains all the simulation data outputted from the simulation run.
 
+   :param file_path: The path to the simulation data file.
+   :type file_path: piel_path_types
+
+   :returns: The simulation data in a Pandas dataframe.
+   :rtype: simulation_data (pd.DataFrame)
+
 
 .. py:function:: simple_plot_simulation_data(simulation_data: pandas.DataFrame)
```

### Comparing `piel-0.0.41/docs/autoapi/piel/tools/gdsfactory/index.rst` & `piel-0.0.43/docs/autoapi/piel/tools/gdsfactory/netlist/index.rst`

 * *Files 11% similar despite different names*

```diff
@@ -1,98 +1,91 @@
-:py:mod:`piel.tools.gdsfactory`
-===============================
+:py:mod:`piel.tools.gdsfactory.netlist`
+=======================================
 
-.. py:module:: piel.tools.gdsfactory
+.. py:module:: piel.tools.gdsfactory.netlist
 
 
-Submodules
-----------
-.. toctree::
-   :titlesonly:
-   :maxdepth: 1
-
-   netlist/index.rst
-
-
-Package Contents
-----------------
+Module Contents
+---------------
 
 
 Functions
 ~~~~~~~~~
 
 .. autoapisummary::
 
-   piel.tools.gdsfactory.get_input_ports_index
-   piel.tools.gdsfactory.get_matched_ports_tuple_index
+   piel.tools.gdsfactory.netlist.get_matched_ports_tuple_index
+   piel.tools.gdsfactory.netlist.get_input_ports_index
 
 
 
-.. py:function:: get_input_ports_index(ports_index: dict, sorting_algorithm: Literal[get_input_ports_index.prefix] = 'prefix', prefix: str = 'in') -> tuple
+.. py:function:: get_matched_ports_tuple_index(ports_index: dict, selected_ports_tuple: Optional[tuple] = None, sorting_algorithm: Literal[get_matched_ports_tuple_index.prefix, selected_ports] = 'prefix', prefix: str = 'in') -> (tuple, tuple)
 
-   This function returns the input ports of a component. However, input ports may have different sets of prefixes and suffixes. This function implements different sorting algorithms for different ports names. The default algorithm is `prefix`, which sorts the ports by their prefix. The Endianness implementation means that the tuple order is determined according to the last numerical index order of the port numbering.
+   This function returns the input ports of a component. However, input ports may have different sets of prefixes
+   and suffixes. This function implements different sorting algorithms for different ports names. The default
+   algorithm is `prefix`, which sorts the ports by their prefix. The Endianness implementation means that the tuple
+   order is determined according to the last numerical index order of the port numbering. Returns just a tuple of
+   the index.
 
    .. code-block:: python
 
        raw_ports_index = {
            "in_o_0": 0,
            "out_o_0": 1,
            "out_o_1": 2,
            "out_o_2": 3,
            "out_o_3": 4,
            "in_o_1": 5,
            "in_o_2": 6,
            "in_o_3": 7,
        }
 
-       get_input_ports_index(ports_index=raw_ports_index)
+       get_input_ports_tuple_index(ports_index=raw_ports_index)
 
        # Output
-       ((0, "in_o_0"), (5, "in_o_1"), (6, "in_o_2"), (7, "in_o_3"))
+       (0, 5, 6, 7)
 
    :param ports_index: The ports index dictionary.
    :type ports_index: dict
+   :param selected_ports_tuple: The selected ports tuple. Defaults to None.
+   :type selected_ports_tuple: tuple, optional
    :param sorting_algorithm: The sorting algorithm to use. Defaults to "prefix".
    :type sorting_algorithm: Literal["prefix"], optional
    :param prefix: The prefix to use for the sorting algorithm. Defaults to "in".
    :type prefix: str, optional
 
    :returns: The ordered input ports index tuple.
-   :rtype: tuple
+             matched_ports_name_tuple_order(tuple): The ordered input ports name tuple.
+   :rtype: matches_ports_index_tuple_order(tuple)
 
 
-.. py:function:: get_matched_ports_tuple_index(ports_index: dict, selected_ports_tuple: tuple, sorting_algorithm: Literal[get_matched_ports_tuple_index.prefix, selected_ports] = 'prefix', prefix: str = 'in') -> (tuple, tuple)
+.. py:function:: get_input_ports_index(ports_index: dict, sorting_algorithm: Literal[get_input_ports_index.prefix] = 'prefix', prefix: str = 'in') -> tuple
 
-   This function returns the input ports of a component. However, input ports may have different sets of prefixes
-   and suffixes. This function implements different sorting algorithms for different ports names. The default
-   algorithm is `prefix`, which sorts the ports by their prefix. The Endianness implementation means that the tuple
-   order is determined according to the last numerical index order of the port numbering. Returns just a tuple of
-   the index.
+   This function returns the input ports of a component. However, input ports may have different sets of prefixes and suffixes. This function implements different sorting algorithms for different ports names. The default algorithm is `prefix`, which sorts the ports by their prefix. The Endianness implementation means that the tuple order is determined according to the last numerical index order of the port numbering.
 
    .. code-block:: python
 
        raw_ports_index = {
            "in_o_0": 0,
            "out_o_0": 1,
            "out_o_1": 2,
            "out_o_2": 3,
            "out_o_3": 4,
            "in_o_1": 5,
            "in_o_2": 6,
            "in_o_3": 7,
        }
 
-       get_input_ports_tuple_index(ports_index=raw_ports_index)
+       get_input_ports_index(ports_index=raw_ports_index)
 
        # Output
-       (0, 5, 6, 7)
+       ((0, "in_o_0"), (5, "in_o_1"), (6, "in_o_2"), (7, "in_o_3"))
 
    :param ports_index: The ports index dictionary.
    :type ports_index: dict
    :param sorting_algorithm: The sorting algorithm to use. Defaults to "prefix".
    :type sorting_algorithm: Literal["prefix"], optional
    :param prefix: The prefix to use for the sorting algorithm. Defaults to "in".
    :type prefix: str, optional
 
    :returns: The ordered input ports index tuple.
-             matched_ports_name_tuple_order(tuple): The ordered input ports name tuple.
-   :rtype: matches_ports_index_tuple_order(tuple)
+   :rtype: tuple
```

### Comparing `piel-0.0.41/docs/autoapi/piel/tools/gdsfactory/netlist/index.rst` & `piel-0.0.43/docs/autoapi/piel/tools/gdsfactory/index.rst`

 * *Files 11% similar despite different names*

```diff
@@ -1,89 +1,100 @@
-:py:mod:`piel.tools.gdsfactory.netlist`
-=======================================
+:py:mod:`piel.tools.gdsfactory`
+===============================
 
-.. py:module:: piel.tools.gdsfactory.netlist
+.. py:module:: piel.tools.gdsfactory
 
 
-Module Contents
----------------
+Submodules
+----------
+.. toctree::
+   :titlesonly:
+   :maxdepth: 1
+
+   netlist/index.rst
+
+
+Package Contents
+----------------
 
 
 Functions
 ~~~~~~~~~
 
 .. autoapisummary::
 
-   piel.tools.gdsfactory.netlist.get_matched_ports_tuple_index
-   piel.tools.gdsfactory.netlist.get_input_ports_index
+   piel.tools.gdsfactory.get_input_ports_index
+   piel.tools.gdsfactory.get_matched_ports_tuple_index
 
 
 
-.. py:function:: get_matched_ports_tuple_index(ports_index: dict, selected_ports_tuple: tuple, sorting_algorithm: Literal[get_matched_ports_tuple_index.prefix, selected_ports] = 'prefix', prefix: str = 'in') -> (tuple, tuple)
+.. py:function:: get_input_ports_index(ports_index: dict, sorting_algorithm: Literal[get_input_ports_index.prefix] = 'prefix', prefix: str = 'in') -> tuple
 
-   This function returns the input ports of a component. However, input ports may have different sets of prefixes
-   and suffixes. This function implements different sorting algorithms for different ports names. The default
-   algorithm is `prefix`, which sorts the ports by their prefix. The Endianness implementation means that the tuple
-   order is determined according to the last numerical index order of the port numbering. Returns just a tuple of
-   the index.
+   This function returns the input ports of a component. However, input ports may have different sets of prefixes and suffixes. This function implements different sorting algorithms for different ports names. The default algorithm is `prefix`, which sorts the ports by their prefix. The Endianness implementation means that the tuple order is determined according to the last numerical index order of the port numbering.
 
    .. code-block:: python
 
        raw_ports_index = {
            "in_o_0": 0,
            "out_o_0": 1,
            "out_o_1": 2,
            "out_o_2": 3,
            "out_o_3": 4,
            "in_o_1": 5,
            "in_o_2": 6,
            "in_o_3": 7,
        }
 
-       get_input_ports_tuple_index(ports_index=raw_ports_index)
+       get_input_ports_index(ports_index=raw_ports_index)
 
        # Output
-       (0, 5, 6, 7)
+       ((0, "in_o_0"), (5, "in_o_1"), (6, "in_o_2"), (7, "in_o_3"))
 
    :param ports_index: The ports index dictionary.
    :type ports_index: dict
    :param sorting_algorithm: The sorting algorithm to use. Defaults to "prefix".
    :type sorting_algorithm: Literal["prefix"], optional
    :param prefix: The prefix to use for the sorting algorithm. Defaults to "in".
    :type prefix: str, optional
 
    :returns: The ordered input ports index tuple.
-             matched_ports_name_tuple_order(tuple): The ordered input ports name tuple.
-   :rtype: matches_ports_index_tuple_order(tuple)
+   :rtype: tuple
 
 
-.. py:function:: get_input_ports_index(ports_index: dict, sorting_algorithm: Literal[get_input_ports_index.prefix] = 'prefix', prefix: str = 'in') -> tuple
+.. py:function:: get_matched_ports_tuple_index(ports_index: dict, selected_ports_tuple: Optional[tuple] = None, sorting_algorithm: Literal[get_matched_ports_tuple_index.prefix, selected_ports] = 'prefix', prefix: str = 'in') -> (tuple, tuple)
 
-   This function returns the input ports of a component. However, input ports may have different sets of prefixes and suffixes. This function implements different sorting algorithms for different ports names. The default algorithm is `prefix`, which sorts the ports by their prefix. The Endianness implementation means that the tuple order is determined according to the last numerical index order of the port numbering.
+   This function returns the input ports of a component. However, input ports may have different sets of prefixes
+   and suffixes. This function implements different sorting algorithms for different ports names. The default
+   algorithm is `prefix`, which sorts the ports by their prefix. The Endianness implementation means that the tuple
+   order is determined according to the last numerical index order of the port numbering. Returns just a tuple of
+   the index.
 
    .. code-block:: python
 
        raw_ports_index = {
            "in_o_0": 0,
            "out_o_0": 1,
            "out_o_1": 2,
            "out_o_2": 3,
            "out_o_3": 4,
            "in_o_1": 5,
            "in_o_2": 6,
            "in_o_3": 7,
        }
 
-       get_input_ports_index(ports_index=raw_ports_index)
+       get_input_ports_tuple_index(ports_index=raw_ports_index)
 
        # Output
-       ((0, "in_o_0"), (5, "in_o_1"), (6, "in_o_2"), (7, "in_o_3"))
+       (0, 5, 6, 7)
 
    :param ports_index: The ports index dictionary.
    :type ports_index: dict
+   :param selected_ports_tuple: The selected ports tuple. Defaults to None.
+   :type selected_ports_tuple: tuple, optional
    :param sorting_algorithm: The sorting algorithm to use. Defaults to "prefix".
    :type sorting_algorithm: Literal["prefix"], optional
    :param prefix: The prefix to use for the sorting algorithm. Defaults to "in".
    :type prefix: str, optional
 
    :returns: The ordered input ports index tuple.
-   :rtype: tuple
+             matched_ports_name_tuple_order(tuple): The ordered input ports name tuple.
+   :rtype: matches_ports_index_tuple_order(tuple)
```

### Comparing `piel-0.0.41/docs/autoapi/piel/tools/index.rst` & `piel-0.0.43/docs/autoapi/piel/tools/index.rst`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 .. toctree::
    :titlesonly:
    :maxdepth: 3
 
    cocotb/index.rst
    gdsfactory/index.rst
    openlane/index.rst
+   pyspice/index.rst
    sax/index.rst
 
 
 Package Contents
 ----------------
 
 
@@ -41,18 +42,18 @@
    piel.tools.configure_parametric_designs_openlane_v1
    piel.tools.configure_flow_script_openlane_v1
    piel.tools.create_parametric_designs_openlane_v1
    piel.tools.get_design_directory_from_root_openlane_v1
    piel.tools.get_latest_version_root_openlane_v1
    piel.tools.read_configuration_openlane_v1
    piel.tools.write_configuration_openlane_v1
-   piel.tools.get_all_timing_sta_files
-   piel.tools.get_all_power_sta_files
    piel.tools.filter_timing_sta_files
    piel.tools.filter_power_sta_files
+   piel.tools.get_all_timing_sta_files
+   piel.tools.get_all_power_sta_files
    piel.tools.calculate_max_frame_amount
    piel.tools.calculate_propagation_delay_from_file
    piel.tools.calculate_propagation_delay_from_timing_data
    piel.tools.configure_timing_data_rows
    piel.tools.configure_frame_id
    piel.tools.filter_timing_data_by_net_name_and_type
    piel.tools.get_frame_meta_data
@@ -158,21 +159,33 @@
 
 .. py:data:: get_simulation_output_files
 
 
 
 .. py:function:: get_simulation_output_files_from_design(design_directory: piel.config.piel_path_types, extension: str = 'csv')
 
-   # TODO DOCS
+   This function returns a list of all the simulation output files in the design directory.
 
+   :param design_directory: The path to the design directory.
+   :type design_directory: piel_path_types
 
-.. py:function:: read_simulation_data(file_path)
+   :returns: List of all the simulation output files in the design directory.
+   :rtype: output_files (list)
+
+
+.. py:function:: read_simulation_data(file_path: piel.config.piel_path_types)
 
    This function returns a Pandas dataframe that contains all the simulation data outputted from the simulation run.
 
+   :param file_path: The path to the simulation data file.
+   :type file_path: piel_path_types
+
+   :returns: The simulation data in a Pandas dataframe.
+   :rtype: simulation_data (pd.DataFrame)
+
 
 .. py:function:: simple_plot_simulation_data(simulation_data: pandas.DataFrame)
 
 
 .. py:function:: get_input_ports_index(ports_index: dict, sorting_algorithm: Literal[get_input_ports_index.prefix] = 'prefix', prefix: str = 'in') -> tuple
 
    This function returns the input ports of a component. However, input ports may have different sets of prefixes and suffixes. This function implements different sorting algorithms for different ports names. The default algorithm is `prefix`, which sorts the ports by their prefix. The Endianness implementation means that the tuple order is determined according to the last numerical index order of the port numbering.
@@ -202,15 +215,15 @@
    :param prefix: The prefix to use for the sorting algorithm. Defaults to "in".
    :type prefix: str, optional
 
    :returns: The ordered input ports index tuple.
    :rtype: tuple
 
 
-.. py:function:: get_matched_ports_tuple_index(ports_index: dict, selected_ports_tuple: tuple, sorting_algorithm: Literal[get_matched_ports_tuple_index.prefix, selected_ports] = 'prefix', prefix: str = 'in') -> (tuple, tuple)
+.. py:function:: get_matched_ports_tuple_index(ports_index: dict, selected_ports_tuple: Optional[tuple] = None, sorting_algorithm: Literal[get_matched_ports_tuple_index.prefix, selected_ports] = 'prefix', prefix: str = 'in') -> (tuple, tuple)
 
    This function returns the input ports of a component. However, input ports may have different sets of prefixes
    and suffixes. This function implements different sorting algorithms for different ports names. The default
    algorithm is `prefix`, which sorts the ports by their prefix. The Endianness implementation means that the tuple
    order is determined according to the last numerical index order of the port numbering. Returns just a tuple of
    the index.
 
@@ -230,14 +243,16 @@
        get_input_ports_tuple_index(ports_index=raw_ports_index)
 
        # Output
        (0, 5, 6, 7)
 
    :param ports_index: The ports index dictionary.
    :type ports_index: dict
+   :param selected_ports_tuple: The selected ports tuple. Defaults to None.
+   :type selected_ports_tuple: tuple, optional
    :param sorting_algorithm: The sorting algorithm to use. Defaults to "prefix".
    :type sorting_algorithm: Literal["prefix"], optional
    :param prefix: The prefix to use for the sorting algorithm. Defaults to "in".
    :type prefix: str, optional
 
    :returns: The ordered input ports index tuple.
              matched_ports_name_tuple_order(tuple): The ordered input ports name tuple.
@@ -393,36 +408,14 @@
    :type configuration: dict
    :param design_directory: Design directory PATH.
    :type design_directory: str
 
    :returns: None
 
 
-.. py:function:: get_all_timing_sta_files(run_directory)
-
-   This function aims to list and perform analysis on all the relevant files in a particular run between all the corners.
-
-   :param run_directory: The run directory to perform the analysis on. Defaults to None.
-   :type run_directory: str, optional
-
-   :returns: List of all the .rpt files in the run directory.
-   :rtype: timing_sta_files_list (list)
-
-
-.. py:function:: get_all_power_sta_files(run_directory)
-
-   This function aims to list and perform analysis on all the relevant files in a particular run between all the corners.
-
-   :param run_directory: The run directory to perform the analysis on. Defaults to None.
-   :type run_directory: str, optional
-
-   :returns: List of all the .rpt files in the run directory.
-   :rtype: power_sta_files_list (list)
-
-
 .. py:function:: filter_timing_sta_files(file_list)
 
    Filter the timing sta files from the list of files
 
    :param file_list: List containing the file paths
    :type file_list: list
 
@@ -437,14 +430,36 @@
    :param file_list: List containing the file paths
    :type file_list: list
 
    :returns: List containing the power sta files
    :rtype: power_sta_files (list)
 
 
+.. py:function:: get_all_timing_sta_files(run_directory)
+
+   This function aims to list and perform analysis on all the relevant files in a particular run between all the corners.
+
+   :param run_directory: The run directory to perform the analysis on. Defaults to None.
+   :type run_directory: str, optional
+
+   :returns: List of all the .rpt files in the run directory.
+   :rtype: timing_sta_files_list (list)
+
+
+.. py:function:: get_all_power_sta_files(run_directory)
+
+   This function aims to list and perform analysis on all the relevant files in a particular run between all the corners.
+
+   :param run_directory: The run directory to perform the analysis on. Defaults to None.
+   :type run_directory: str, optional
+
+   :returns: List of all the .rpt files in the run directory.
+   :rtype: power_sta_files_list (list)
+
+
 .. py:function:: calculate_max_frame_amount(file_lines_data: pandas.DataFrame)
 
    Calculate the maximum frame amount based on the frame IDs in the DataFrame
 
    :param file_lines_data: Dataframe containing the file lines
    :type file_lines_data: pd.DataFrame
```

### Comparing `piel-0.0.41/docs/autoapi/piel/tools/openlane/index.rst` & `piel-0.0.43/docs/autoapi/piel/tools/openlane/index.rst`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -42,18 +42,18 @@
    piel.tools.openlane.configure_parametric_designs_openlane_v1
    piel.tools.openlane.configure_flow_script_openlane_v1
    piel.tools.openlane.create_parametric_designs_openlane_v1
    piel.tools.openlane.get_design_directory_from_root_openlane_v1
    piel.tools.openlane.get_latest_version_root_openlane_v1
    piel.tools.openlane.read_configuration_openlane_v1
    piel.tools.openlane.write_configuration_openlane_v1
-   piel.tools.openlane.get_all_timing_sta_files
-   piel.tools.openlane.get_all_power_sta_files
    piel.tools.openlane.filter_timing_sta_files
    piel.tools.openlane.filter_power_sta_files
+   piel.tools.openlane.get_all_timing_sta_files
+   piel.tools.openlane.get_all_power_sta_files
    piel.tools.openlane.calculate_max_frame_amount
    piel.tools.openlane.calculate_propagation_delay_from_file
    piel.tools.openlane.calculate_propagation_delay_from_timing_data
    piel.tools.openlane.configure_timing_data_rows
    piel.tools.openlane.configure_frame_id
    piel.tools.openlane.filter_timing_data_by_net_name_and_type
    piel.tools.openlane.get_frame_meta_data
@@ -218,36 +218,14 @@
    :type configuration: dict
    :param design_directory: Design directory PATH.
    :type design_directory: str
 
    :returns: None
 
 
-.. py:function:: get_all_timing_sta_files(run_directory)
-
-   This function aims to list and perform analysis on all the relevant files in a particular run between all the corners.
-
-   :param run_directory: The run directory to perform the analysis on. Defaults to None.
-   :type run_directory: str, optional
-
-   :returns: List of all the .rpt files in the run directory.
-   :rtype: timing_sta_files_list (list)
-
-
-.. py:function:: get_all_power_sta_files(run_directory)
-
-   This function aims to list and perform analysis on all the relevant files in a particular run between all the corners.
-
-   :param run_directory: The run directory to perform the analysis on. Defaults to None.
-   :type run_directory: str, optional
-
-   :returns: List of all the .rpt files in the run directory.
-   :rtype: power_sta_files_list (list)
-
-
 .. py:function:: filter_timing_sta_files(file_list)
 
    Filter the timing sta files from the list of files
 
    :param file_list: List containing the file paths
    :type file_list: list
 
@@ -262,14 +240,36 @@
    :param file_list: List containing the file paths
    :type file_list: list
 
    :returns: List containing the power sta files
    :rtype: power_sta_files (list)
 
 
+.. py:function:: get_all_timing_sta_files(run_directory)
+
+   This function aims to list and perform analysis on all the relevant files in a particular run between all the corners.
+
+   :param run_directory: The run directory to perform the analysis on. Defaults to None.
+   :type run_directory: str, optional
+
+   :returns: List of all the .rpt files in the run directory.
+   :rtype: timing_sta_files_list (list)
+
+
+.. py:function:: get_all_power_sta_files(run_directory)
+
+   This function aims to list and perform analysis on all the relevant files in a particular run between all the corners.
+
+   :param run_directory: The run directory to perform the analysis on. Defaults to None.
+   :type run_directory: str, optional
+
+   :returns: List of all the .rpt files in the run directory.
+   :rtype: power_sta_files_list (list)
+
+
 .. py:function:: calculate_max_frame_amount(file_lines_data: pandas.DataFrame)
 
    Calculate the maximum frame amount based on the frame IDs in the DataFrame
 
    :param file_lines_data: Dataframe containing the file lines
    :type file_lines_data: pd.DataFrame
```

### Comparing `piel-0.0.41/docs/autoapi/piel/tools/openlane/migrate/index.rst` & `piel-0.0.43/docs/autoapi/piel/tools/openlane/migrate/index.rst`

 * *Files identical despite different names*

### Comparing `piel-0.0.41/docs/autoapi/piel/tools/openlane/parse/index.rst` & `piel-0.0.43/docs/autoapi/piel/tools/openlane/parse/index.rst`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -27,18 +27,18 @@
 
 
 Functions
 ~~~~~~~~~
 
 .. autoapisummary::
 
-   piel.tools.openlane.parse.get_all_timing_sta_files
-   piel.tools.openlane.parse.get_all_power_sta_files
    piel.tools.openlane.parse.filter_timing_sta_files
    piel.tools.openlane.parse.filter_power_sta_files
+   piel.tools.openlane.parse.get_all_timing_sta_files
+   piel.tools.openlane.parse.get_all_power_sta_files
    piel.tools.openlane.parse.calculate_max_frame_amount
    piel.tools.openlane.parse.calculate_propagation_delay_from_file
    piel.tools.openlane.parse.calculate_propagation_delay_from_timing_data
    piel.tools.openlane.parse.configure_timing_data_rows
    piel.tools.openlane.parse.configure_frame_id
    piel.tools.openlane.parse.filter_timing_data_by_net_name_and_type
    piel.tools.openlane.parse.get_frame_meta_data
@@ -49,36 +49,14 @@
    piel.tools.openlane.parse.contains_in_lines
    piel.tools.openlane.parse.create_file_lines_dataframe
    piel.tools.openlane.parse.get_file_line_by_keyword
    piel.tools.openlane.parse.read_file_lines
 
 
 
-.. py:function:: get_all_timing_sta_files(run_directory)
-
-   This function aims to list and perform analysis on all the relevant files in a particular run between all the corners.
-
-   :param run_directory: The run directory to perform the analysis on. Defaults to None.
-   :type run_directory: str, optional
-
-   :returns: List of all the .rpt files in the run directory.
-   :rtype: timing_sta_files_list (list)
-
-
-.. py:function:: get_all_power_sta_files(run_directory)
-
-   This function aims to list and perform analysis on all the relevant files in a particular run between all the corners.
-
-   :param run_directory: The run directory to perform the analysis on. Defaults to None.
-   :type run_directory: str, optional
-
-   :returns: List of all the .rpt files in the run directory.
-   :rtype: power_sta_files_list (list)
-
-
 .. py:function:: filter_timing_sta_files(file_list)
 
    Filter the timing sta files from the list of files
 
    :param file_list: List containing the file paths
    :type file_list: list
 
@@ -93,14 +71,36 @@
    :param file_list: List containing the file paths
    :type file_list: list
 
    :returns: List containing the power sta files
    :rtype: power_sta_files (list)
 
 
+.. py:function:: get_all_timing_sta_files(run_directory)
+
+   This function aims to list and perform analysis on all the relevant files in a particular run between all the corners.
+
+   :param run_directory: The run directory to perform the analysis on. Defaults to None.
+   :type run_directory: str, optional
+
+   :returns: List of all the .rpt files in the run directory.
+   :rtype: timing_sta_files_list (list)
+
+
+.. py:function:: get_all_power_sta_files(run_directory)
+
+   This function aims to list and perform analysis on all the relevant files in a particular run between all the corners.
+
+   :param run_directory: The run directory to perform the analysis on. Defaults to None.
+   :type run_directory: str, optional
+
+   :returns: List of all the .rpt files in the run directory.
+   :rtype: power_sta_files_list (list)
+
+
 .. py:function:: calculate_max_frame_amount(file_lines_data: pandas.DataFrame)
 
    Calculate the maximum frame amount based on the frame IDs in the DataFrame
 
    :param file_lines_data: Dataframe containing the file lines
    :type file_lines_data: pd.DataFrame
```

### Comparing `piel-0.0.41/docs/autoapi/piel/tools/openlane/parse/sta_rpt/index.rst` & `piel-0.0.43/docs/autoapi/piel/tools/openlane/parse/sta_rpt/index.rst`

 * *Files identical despite different names*

### Comparing `piel-0.0.41/docs/autoapi/piel/tools/openlane/parse/utils/index.rst` & `piel-0.0.43/docs/autoapi/piel/tools/openlane/parse/utils/index.rst`

 * *Files identical despite different names*

### Comparing `piel-0.0.41/docs/autoapi/piel/tools/openlane/utils/index.rst` & `piel-0.0.43/docs/autoapi/piel/tools/openlane/utils/index.rst`

 * *Files identical despite different names*

### Comparing `piel-0.0.41/docs/autoapi/piel/tools/openlane/v1/index.rst` & `piel-0.0.43/docs/autoapi/piel/tools/openlane/v1/index.rst`

 * *Files identical despite different names*

### Comparing `piel-0.0.41/docs/autoapi/piel/tools/openlane/v2/index.rst` & `piel-0.0.43/docs/autoapi/piel/tools/openlane/v2/index.rst`

 * *Files identical despite different names*

### Comparing `piel-0.0.41/docs/autoapi/piel/tools/sax/index.rst` & `piel-0.0.43/docs/autoapi/piel/tools/sax/index.rst`

 * *Files identical despite different names*

### Comparing `piel-0.0.41/docs/autoapi/piel/tools/sax/utils/index.rst` & `piel-0.0.43/docs/autoapi/piel/tools/sax/utils/index.rst`

 * *Files identical despite different names*

### Comparing `piel-0.0.41/docs/autoapi/piel/visual/auto_plot_multiple/index.rst` & `piel-0.0.43/docs/autoapi/piel/visual/auto_plot_multiple/index.rst`

 * *Files identical despite different names*

### Comparing `piel-0.0.41/docs/autoapi/piel/visual/data_conversion/index.rst` & `piel-0.0.43/docs/autoapi/piel/visual/data_conversion/index.rst`

 * *Files identical despite different names*

### Comparing `piel-0.0.41/docs/autoapi/piel/visual/index.rst` & `piel-0.0.43/docs/autoapi/piel/visual/index.rst`

 * *Files identical despite different names*

### Comparing `piel-0.0.41/docs/conf.py` & `piel-0.0.43/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,19 +65,21 @@
 
 # Grouping the document tree into LaTeX files. List of tuples
 # (source start file, target name, title, author, documentclass
 # [howto, manual, or own class]).
 latex_documents = [
     (master_doc, "piel.tex", "piel Documentation", "Dario Quintero", "manual"),
 ]
+html_logo = "_static/img/logo.png"
 html_show_sourcelink = (
     True  # Remove 'view source code' from top of page (for html, not python)
 )
 html_static_path = ["_static"]
-html_theme = "alabaster"
+html_theme = "sphinx_book_theme"
+html_title = "s "
 htmlhelp_basename = "pieldoc"
 man_pages = [(master_doc, "piel", "piel Documentation", [author], 1)]
 project = "piel"
 pygments_style = "sphinx"
 release = piel.__version__
 set_type_checking_flag = True  # Enable 'expensive' imports for sphinx_autodoc_typehints
 source_suffix = [".rst", ".md"]
```

### Comparing `piel-0.0.41/docs/examples/designs/simple_design/simple_design/tb/default/Makefile` & `piel-0.0.43/docs/examples/designs/simple_design/simple_design/tb/default/Makefile`

 * *Files identical despite different names*

### Comparing `piel-0.0.41/docs/make.bat` & `piel-0.0.43/docs/make.bat`

 * *Files identical despite different names*

### Comparing `piel-0.0.41/docs/sections/microservices/dependencies/cocotb.rst` & `piel-0.0.43/docs/sections/microservices/dependencies/cocotb.rst`

 * *Files identical despite different names*

### Comparing `piel-0.0.41/docs/sections/microservices/dependencies/openlane.rst` & `piel-0.0.43/docs/sections/microservices/dependencies/openlane.rst`

 * *Files identical despite different names*

### Comparing `piel-0.0.41/docs/sections/microservices/dependencies/pyspice.rst` & `piel-0.0.43/docs/sections/microservices/dependencies/pyspice.rst`

 * *Files identical despite different names*

### Comparing `piel-0.0.41/docs/sections/microservices/dependencies/sax.rst` & `piel-0.0.43/docs/sections/microservices/dependencies/sax.rst`

 * *Files identical despite different names*

### Comparing `piel-0.0.41/docs/sections/microservices/integration/sax_qutip.rst` & `piel-0.0.43/docs/sections/microservices/integration/sax_qutip.rst`

 * *Files identical despite different names*

### Comparing `piel-0.0.41/piel/__init__.py` & `piel-0.0.43/piel/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,8 +19,8 @@
 
 os.environ["PIEL_PACKAGE_DIRECTORY"] = str(
     pathlib.Path(__file__).parent.parent.resolve()
 )
 
 __author__ = """Dario Quintero"""
 __email__ = "darioaquintero@gmail.com"
-__version__ = "0.0.41"
+__version__ = "0.0.43"
```

### Comparing `piel-0.0.41/piel/config.py` & `piel-0.0.43/piel/config.py`

 * *Files identical despite different names*

### Comparing `piel-0.0.41/piel/defaults.py` & `piel-0.0.43/piel/defaults.py`

 * *Files identical despite different names*

### Comparing `piel-0.0.41/piel/file_conversion.py` & `piel-0.0.43/piel/file_conversion.py`

 * *Files identical despite different names*

### Comparing `piel-0.0.41/piel/file_system.py` & `piel-0.0.43/piel/file_system.py`

 * *Files identical despite different names*

### Comparing `piel-0.0.41/piel/integration/openlane_gdsfactory_core.py` & `piel-0.0.43/piel/integration/gdsfactory_openlane.py`

 * *Files identical despite different names*

### Comparing `piel-0.0.41/piel/integration/sax_qutip.py` & `piel-0.0.43/piel/integration/sax_qutip.py`

 * *Files identical despite different names*

### Comparing `piel-0.0.41/piel/models/frequency/all.py` & `piel-0.0.43/piel/models/frequency/all.py`

 * *Files identical despite different names*

### Comparing `piel-0.0.41/piel/models/frequency/defaults.py` & `piel-0.0.43/piel/models/frequency/defaults.py`

 * *Files identical despite different names*

### Comparing `piel-0.0.41/piel/models/frequency/photonic/directional_coupler_length.py` & `piel-0.0.43/piel/models/frequency/photonic/directional_coupler_length.py`

 * *Files identical despite different names*

### Comparing `piel-0.0.41/piel/models/frequency/photonic/directional_coupler_real.py` & `piel-0.0.43/piel/models/frequency/photonic/directional_coupler_real.py`

 * *Files identical despite different names*

### Comparing `piel-0.0.41/piel/models/frequency/photonic/grating_coupler.py` & `piel-0.0.43/piel/models/frequency/photonic/grating_coupler.py`

 * *Files identical despite different names*

### Comparing `piel-0.0.41/piel/models/frequency/photonic/straight_waveguide.py` & `piel-0.0.43/piel/models/frequency/photonic/straight_waveguide.py`

 * *Files identical despite different names*

### Comparing `piel-0.0.41/piel/models/logic/electro_optic/signal_mapping.py` & `piel-0.0.43/piel/models/logic/electro_optic/signal_mapping.py`

 * *Files identical despite different names*

### Comparing `piel-0.0.41/piel/parametric.py` & `piel-0.0.43/piel/parametric.py`

 * *Files identical despite different names*

### Comparing `piel-0.0.41/piel/project_structure.py` & `piel-0.0.43/piel/project_structure.py`

 * *Files identical despite different names*

### Comparing `piel-0.0.41/piel/tools/cocotb/core.py` & `piel-0.0.43/piel/tools/cocotb/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 """
 The objective of this file is to provide the simulation ports and interconnection to consider modelling digital and mixed signal logic.
 
-The main simulation driver is cocotb, and this generates a set of files that correspond to time-domain digital simulations.
-The cocotb verification software can also be used to perform mixed signal simulation, and digital data can be inputted as a bitstream into a photonic solver, although the ideal situation would be to have integrated photonic time-domain models alongside the electronic simulation solver, and maybe this is where it will go. It can be assumed that, as is currently, cocotb can interface python with multiple solvers until someone (and I'd love to do this) writes an equivalent python-based or C++ based python time-domain simulation solver.
+The main simulation driver is cocotb, and this generates a set of files that correspond to time-domain digital
+simulations. The cocotb verification software can also be used to perform mixed signal simulation, and digital data
+can be inputted as a bitstream into a photonic solver, although the ideal situation would be to have integrated
+photonic time-domain models alongside the electronic simulation solver, and maybe this is where it will go. It can be
+assumed that, as is currently, cocotb can interface python with multiple solvers until someone (and I'd love to do
+this) writes an equivalent python-based or C++ based python time-domain simulation solver.
 
-The nice thing about cocotb is that as long as the photonic simulations can be written asyncrhonously, time-domain simulations can be closely integrated or simulated through this verification software.
-"""
+The nice thing about cocotb is that as long as the photonic simulations can be written asynchronously, time-domain
+simulations can be closely integrated or simulated through this verification software. """
 import functools
 import pathlib
 import subprocess
 from typing import Literal
 from piel.file_system import return_path, write_script, delete_path_list_in_directory
 
 __all__ = [
```

### Comparing `piel-0.0.41/piel/tools/cocotb/data.py` & `piel-0.0.43/piel/tools/cocotb/data.py`

 * *Files 16% similar despite different names*

```diff
@@ -19,26 +19,38 @@
 
 
 def get_simulation_output_files_from_design(
     design_directory: piel_path_types,
     extension: str = "csv",
 ):
     """
-    # TODO DOCS
+    This function returns a list of all the simulation output files in the design directory.
+
+    Args:
+        design_directory (piel_path_types): The path to the design directory.
+
+    Returns:
+        output_files (list): List of all the simulation output files in the design directory.
     """
     design_directory = return_path(design_directory)
     output_files = get_files_recursively_in_directory(
         path=design_directory / "tb" / "out", extension=extension
     )
     return output_files
 
 
-def read_simulation_data(file_path):
+def read_simulation_data(file_path: piel_path_types):
     """
     This function returns a Pandas dataframe that contains all the simulation data outputted from the simulation run.
+
+    Args:
+        file_path (piel_path_types): The path to the simulation data file.
+
+    Returns:
+        simulation_data (pd.DataFrame): The simulation data in a Pandas dataframe.
     """
     file_path = return_path(file_path)
     simulation_data = pd.read_csv(file_path)
     return simulation_data
 
 
 def simple_plot_simulation_data(simulation_data: pd.DataFrame):
```

### Comparing `piel-0.0.41/piel/tools/gdsfactory/netlist.py` & `piel-0.0.43/piel/tools/gdsfactory/netlist.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-from typing import Literal
+from typing import Literal, Optional
 
 __all__ = ["get_input_ports_index", "get_matched_ports_tuple_index"]
 
 
 def get_matched_ports_tuple_index(
     ports_index: dict,
-    selected_ports_tuple: tuple,
+    selected_ports_tuple: Optional[tuple] = None,
     sorting_algorithm: Literal["prefix", "selected_ports"] = "prefix",
     prefix: str = "in",
 ) -> (tuple, tuple):
     """
     This function returns the input ports of a component. However, input ports may have different sets of prefixes
     and suffixes. This function implements different sorting algorithms for different ports names. The default
     algorithm is `prefix`, which sorts the ports by their prefix. The Endianness implementation means that the tuple
@@ -32,14 +32,15 @@
         get_input_ports_tuple_index(ports_index=raw_ports_index)
 
         # Output
         (0, 5, 6, 7)
 
     Args:
         ports_index (dict): The ports index dictionary.
+        selected_ports_tuple (tuple, optional): The selected ports tuple. Defaults to None.
         sorting_algorithm (Literal["prefix"], optional): The sorting algorithm to use. Defaults to "prefix".
         prefix (str, optional): The prefix to use for the sorting algorithm. Defaults to "in".
 
     Returns:
         matches_ports_index_tuple_order(tuple): The ordered input ports index tuple.
         matched_ports_name_tuple_order(tuple): The ordered input ports name tuple.
```

### Comparing `piel-0.0.41/piel/tools/openlane/migrate.py` & `piel-0.0.43/piel/tools/openlane/migrate.py`

 * *Files identical despite different names*

### Comparing `piel-0.0.41/piel/tools/openlane/parse/sta_rpt.py` & `piel-0.0.43/piel/tools/openlane/parse/sta_rpt.py`

 * *Files identical despite different names*

### Comparing `piel-0.0.41/piel/tools/openlane/parse/utils.py` & `piel-0.0.43/piel/tools/openlane/parse/utils.py`

 * *Files identical despite different names*

### Comparing `piel-0.0.41/piel/tools/openlane/utils.py` & `piel-0.0.43/piel/tools/openlane/utils.py`

 * *Files identical despite different names*

### Comparing `piel-0.0.41/piel/tools/openlane/v1.py` & `piel-0.0.43/piel/tools/openlane/v1.py`

 * *Files identical despite different names*

### Comparing `piel-0.0.41/piel/tools/openlane/v2.py` & `piel-0.0.43/piel/tools/openlane/v2.py`

 * *Files identical despite different names*

### Comparing `piel-0.0.41/piel/tools/sax/utils.py` & `piel-0.0.43/piel/tools/sax/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 This file provides a set of utilities that allow much easier integration between `sax` and the relevant tools that we use.
 """
+import numpy as np
 import sax
 from ..gdsfactory.netlist import get_matched_ports_tuple_index
 from typing import Optional  # NOQA : F401
 
 __all__ = ["get_sdense_ports_index", "sax_to_s_parameters_standard_matrix", "snet"]
 
 
@@ -176,14 +177,17 @@
             output_ports_index_tuple_order,
             output_matched_ports_name_tuple_order,
         ) = get_matched_ports_tuple_index(
             ports_index=dense_s_parameter_index, prefix="out"
         )
 
     # We now select the SDense columns that we care about.
+    dense_s_parameter_matrix = np.asarray(
+        dense_s_parameter_matrix
+    )  # TODO port to JAX multiindexing
     s_parameters_standard_matrix = dense_s_parameter_matrix[
         [output_ports_index_tuple_order]
     ][0]
     # Now we select the SDense rows that we care about after transposing the matrix.
     s_parameters_standard_matrix = s_parameters_standard_matrix[
         :, [input_ports_index_tuple_order][0]
     ]
```

### Comparing `piel-0.0.41/piel/visual/auto_plot_multiple.py` & `piel-0.0.43/piel/visual/auto_plot_multiple.py`

 * *Files identical despite different names*

### Comparing `piel-0.0.41/piel/visual/data_conversion.py` & `piel-0.0.43/piel/visual/data_conversion.py`

 * *Files identical despite different names*

### Comparing `piel-0.0.41/piel.egg-info/PKG-INFO` & `piel-0.0.43/piel.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: piel
-Version: 0.0.41
-Summary: Photonic and electronic co-simulation system design tools interfaced with open-source design software like GDSFactory and OpenROAD.
+Version: 0.0.43
+Summary: Photonic Integrated Electronics: microservices to codesign photonics, electronics, communications, quantum, and more.
 Home-page: https://github.com/daquintero/piel
 Author: Dario Quintero
 Author-email: darioaquintero@gmail.com
 License: MIT license
 Keywords: piel
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
@@ -16,48 +16,70 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: develop
 License-File: LICENSE
 
-# `piel` - Photonic and Integrated ELectronic tools
-[![PyPI Version](https://img.shields.io/pypi/v/piel.svg)](https://pypi.python.org/pypi/piel)
-[![Build Status](https://img.shields.io/travis/daquintero/piel.svg)](https://travis-ci.com/daquintero/piel)
-[![Documentation Status](https://readthedocs.org/projects/piel/badge/?version=latest)](https://piel.readthedocs.io/en/latest/?version=latest)
-[![Updates](https://pyup.io/repos/github/daquintero/piel/shield.svg)](https://pyup.io/repos/github/daquintero/piel/)
+**P**\hotonic **I**\ntegrated **EL**\ectronics
+===============================================
 
-Microservices to codesign photonics, electronics, quantum, and more.
+|PyPI Version| |Build Status| |Documentation Status| |Updates|
 
-- Free software: MIT license
-- Documentation: [https://piel.readthedocs.io](https://piel.readthedocs.io)
+Microservices to codesign photonics, electronics, communications,
+quantum, and more.
 
-## Target functionality
-* Co-simulation and optimisation between integrated photonic and electronic chip design.
-* System interconnection modelling in multiple environments.
-* Individual and interposer design integration.
-* Multi-domain electronics and photonics component models.
-* Quantum models of physical circuitry
+-  Free software: MIT license
+-  Documentation: https://piel.readthedocs.io
 
-`piel` aims to provide an integrated workflow to co-design photonics and electronics, classically and quantum. It does not aim to replace the individual functionality of each design tool, but rather provide a glue to easily connect them all together and extract the system performance.
+Target functionality
+--------------------
 
-## Examples
+-  Co-simulation and optimisation between integrated photonic and
+   electronic chip design.
+-  System interconnection modelling in multiple domains.
+-  Chip and interposer design integration.
+-  Component models translation library between simulation tools.
+-  Quantum models of physical circuitry.
 
-Follow the many [examples in the documentation](https://piel.readthedocs.io/en/stable/examples.html).
+``piel`` aims to provide an integrated workflow to co-design photonics
+and electronics, classically and quantum. It does not aim to replace the
+individual functionality of each design tool, but rather provide a glue
+to easily connect them all together and extract the system performance.
 
-## Microservices Toolset
-This package provides interconnection functions to easily co-design microelectronics through the functionality of the [IIC-OSIC-TOOLS](https://github.com/iic-jku/iic-osic-tools) and photonics via [GDSFactory](https://github.com/gdsfactory/gdsfactory).
+Examples
+--------
 
-Some existing microservice dependency integrations are:
-* [cocotb](https://github.com/cocotb/cocotb) - a coroutine based cosimulation library for writing VHDL and Verilog testbenches in Python.
-* [GDSFactory](https://github.com/gdsfactory/gdsfactory) - An open source platform for end to-end photonic chip design and validation
-* [OpenLane v1](https://github.com/The-OpenROAD-Project/OpenLane) - an automated RTL to GDSII flow based on several components including OpenROAD, Yosys, Magic, Netgen and custom methodology scripts for design exploration and optimization
-* [pyspice](https://github.com/PySpice-org/PySpice) - Simulate electronic circuit using Python and the Ngspice / Xyce simulators
-* [sax](https://github.com/flaport/sax) - S-parameter based frequency domain circuit simulations and optimizations using JAX.
-* [qutip](https://github.com/qutip/qutip) - QuTiP: Quantum Toolbox in Python
+Follow the many `examples in the documentation <https://piel.readthedocs.io/en/stable/examples.html>`__.
+
+Microservices Toolset
+---------------------
 
-## Environment Requirements
-* Please install the Linux Docker environment provided by [IIC-OSIC-TOOLS](https://github.com/iic-jku/iic-osic-tools).
+This package provides interconnection functions to easily co-design
+microelectronics through the functionality of the
+`IIC-OSIC-TOOLS <https://github.com/iic-jku/iic-osic-tools>`__ and
+photonics via `GDSFactory <https://github.com/gdsfactory/gdsfactory>`__.
 
+Some existing microservice dependency integrations are:
 
-## Contribution
-If you feel dedicated enough to become a project maintainer, or just want to do a single contributor, let's do this together!
+* `cocotb <https://github.com/cocotb/cocotb>`__ - a coroutine based cosimulation library for writing VHDL and Verilog testbenches in Python.
+* `GDSFactory <https://github.com/gdsfactory/gdsfactory>`__ - An open source platform for end to-end photonic chip design and validation
+* `OpenLane v1 <https://github.com/The-OpenROAD-Project/OpenLane>`__ - an automated RTL to GDSII flow based on several components including OpenROAD, Yosys, Magic, Netgen and custom methodology scripts for design exploration and optimization
+* `pyspice <https://github.com/PySpice-org/PySpice>`__ - Simulate electronic circuit using Python and the Ngspice / Xyce simulators
+* `sax <https://github.com/flaport/sax>`__ - S-parameter based frequency domain circuit simulations and optimizations using JAX.
+* `thewalrus <https://github.com/XanaduAI/thewalrus>`__ -A library for the calculation of hafnians, Hermite polynomials and Gaussian boson sampling.
+* `qutip <https://github.com/qutip/qutip>`__ - QuTiP: Quantum Toolbox in Python
+
+Contribution
+------------
+
+If you feel dedicated enough to become a project maintainer, or just
+want to do a single contribution, let's do this together!
+
+.. |PyPI Version| image:: https://img.shields.io/pypi/v/piel.svg
+   :target: https://pypi.python.org/pypi/piel
+.. |Build Status| image:: https://img.shields.io/travis/daquintero/piel.svg
+   :target: https://travis-ci.com/daquintero/piel
+.. |Documentation Status| image:: https://readthedocs.org/projects/piel/badge/?version=latest
+   :target: https://piel.readthedocs.io/en/latest/?version=latest
+.. |Updates| image:: https://pyup.io/repos/github/daquintero/piel/shield.svg
+   :target: https://pyup.io/repos/github/daquintero/piel/
```

### Comparing `piel-0.0.41/piel.egg-info/SOURCES.txt` & `piel-0.0.43/piel.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,31 +1,38 @@
 CONTRIBUTING.rst
 LICENSE
 MANIFEST.in
-README.md
+README.rst
 setup.cfg
 setup.py
 docs/Makefile
 docs/conf.py
 docs/contributing.rst
 docs/examples.rst
 docs/index.rst
 docs/make.bat
+docs/_static/img/logo.png
 docs/autoapi/index.rst
 docs/autoapi/piel/index.rst
 docs/autoapi/piel/cli/index.rst
 docs/autoapi/piel/components/index.rst
 docs/autoapi/piel/config/index.rst
 docs/autoapi/piel/defaults/index.rst
 docs/autoapi/piel/file_conversion/index.rst
 docs/autoapi/piel/file_system/index.rst
 docs/autoapi/piel/integration/index.rst
-docs/autoapi/piel/integration/openlane_gdsfactory_core/index.rst
-docs/autoapi/piel/integration/sax_cocotb/index.rst
+docs/autoapi/piel/integration/cocotb_sax/index.rst
+docs/autoapi/piel/integration/gdsfactory_openlane/index.rst
+docs/autoapi/piel/integration/gdsfactory_pyspice/index.rst
+docs/autoapi/piel/integration/gdsfactory_pyspice/conversion/index.rst
+docs/autoapi/piel/integration/gdsfactory_pyspice/core/index.rst
+docs/autoapi/piel/integration/gdsfactory_pyspice/utils/index.rst
+docs/autoapi/piel/integration/pyspice_sax/index.rst
 docs/autoapi/piel/integration/sax_qutip/index.rst
+docs/autoapi/piel/integration/sax_thewalrus/index.rst
 docs/autoapi/piel/models/index.rst
 docs/autoapi/piel/models/frequency/index.rst
 docs/autoapi/piel/models/frequency/all/index.rst
 docs/autoapi/piel/models/frequency/defaults/index.rst
 docs/autoapi/piel/models/frequency/electrical/index.rst
 docs/autoapi/piel/models/frequency/electro_optic/index.rst
 docs/autoapi/piel/models/frequency/electro_optic/ideal/index.rst
@@ -50,14 +57,18 @@
 docs/autoapi/piel/models/logic/photonic/index.rst
 docs/autoapi/piel/models/physical/index.rst
 docs/autoapi/piel/models/physical/electrical/index.rst
 docs/autoapi/piel/models/physical/electrical/cable/index.rst
 docs/autoapi/piel/models/physical/electro_optic/index.rst
 docs/autoapi/piel/models/physical/electro_optic/basic_heater/index.rst
 docs/autoapi/piel/models/physical/electronic/index.rst
+docs/autoapi/piel/models/physical/electronic/spice/index.rst
+docs/autoapi/piel/models/physical/electronic/spice/capacitor/index.rst
+docs/autoapi/piel/models/physical/electronic/spice/defaults/index.rst
+docs/autoapi/piel/models/physical/electronic/spice/resistor/index.rst
 docs/autoapi/piel/models/physical/geometry/index.rst
 docs/autoapi/piel/models/physical/opto_electronic/index.rst
 docs/autoapi/piel/models/physical/photonic/index.rst
 docs/autoapi/piel/models/physical/thermal/index.rst
 docs/autoapi/piel/models/physical/units/index.rst
 docs/autoapi/piel/models/transient/index.rst
 docs/autoapi/piel/models/transient/electrical/index.rst
@@ -78,26 +89,30 @@
 docs/autoapi/piel/tools/openlane/migrate/index.rst
 docs/autoapi/piel/tools/openlane/parse/index.rst
 docs/autoapi/piel/tools/openlane/parse/sta_rpt/index.rst
 docs/autoapi/piel/tools/openlane/parse/utils/index.rst
 docs/autoapi/piel/tools/openlane/utils/index.rst
 docs/autoapi/piel/tools/openlane/v1/index.rst
 docs/autoapi/piel/tools/openlane/v2/index.rst
+docs/autoapi/piel/tools/pyspice/index.rst
+docs/autoapi/piel/tools/pyspice/component/index.rst
 docs/autoapi/piel/tools/sax/index.rst
 docs/autoapi/piel/tools/sax/utils/index.rst
 docs/autoapi/piel/visual/index.rst
 docs/autoapi/piel/visual/auto_plot_multiple/index.rst
 docs/autoapi/piel/visual/data_conversion/index.rst
 docs/examples/designs/simple_design/simple_design/tb/Makefile
 docs/examples/designs/simple_design/simple_design/tb/default/Makefile
 docs/sections/about/AUTHORS.rst
 docs/sections/about/index.rst
 docs/sections/codesign/index.rst
 docs/sections/components/index.rst
+docs/sections/environment/developer_docker_configuration.rst
 docs/sections/environment/index.rst
+docs/sections/environment/setup.rst
 docs/sections/microservices/index.rst
 docs/sections/microservices/dependencies/cocotb.rst
 docs/sections/microservices/dependencies/gdsfactory.rst
 docs/sections/microservices/dependencies/index.rst
 docs/sections/microservices/dependencies/openlane.rst
 docs/sections/microservices/dependencies/principle.rst
 docs/sections/microservices/dependencies/pyspice.rst
@@ -118,17 +133,23 @@
 piel.egg-info/dependency_links.txt
 piel.egg-info/entry_points.txt
 piel.egg-info/not-zip-safe
 piel.egg-info/requires.txt
 piel.egg-info/top_level.txt
 piel/components/__init__.py
 piel/integration/__init__.py
-piel/integration/openlane_gdsfactory_core.py
-piel/integration/sax_cocotb.py
+piel/integration/cocotb_sax.py
+piel/integration/gdsfactory_openlane.py
+piel/integration/pyspice_sax.py
 piel/integration/sax_qutip.py
+piel/integration/sax_thewalrus.py
+piel/integration/gdsfactory_pyspice/__init__.py
+piel/integration/gdsfactory_pyspice/conversion.py
+piel/integration/gdsfactory_pyspice/core.py
+piel/integration/gdsfactory_pyspice/utils.py
 piel/models/__init__.py
 piel/models/utils.py
 piel/models/frequency/__init__.py
 piel/models/frequency/all.py
 piel/models/frequency/defaults.py
 piel/models/frequency/utils.py
 piel/models/frequency/electrical/__init__.py
@@ -157,14 +178,18 @@
 piel/models/physical/thermal.py
 piel/models/physical/units.py
 piel/models/physical/electrical/__init__.py
 piel/models/physical/electrical/cable.py
 piel/models/physical/electro_optic/__init__.py
 piel/models/physical/electro_optic/basic_heater.py
 piel/models/physical/electronic/__init__.py
+piel/models/physical/electronic/spice/__init__.py
+piel/models/physical/electronic/spice/capacitor.py
+piel/models/physical/electronic/spice/defaults.py
+piel/models/physical/electronic/spice/resistor.py
 piel/models/physical/opto_electronic/__init__.py
 piel/models/physical/photonic/__init__.py
 piel/models/transient/__init__.py
 piel/models/transient/electrical/__init__.py
 piel/models/transient/electro_optic/__init__.py
 piel/models/transient/electronic/__init__.py
 piel/models/transient/opto_electronic/__init__.py
@@ -177,23 +202,28 @@
 piel/tools/gdsfactory/netlist.py
 piel/tools/openlane/__init__.py
 piel/tools/openlane/migrate.py
 piel/tools/openlane/utils.py
 piel/tools/openlane/v1.py
 piel/tools/openlane/v2.py
 piel/tools/openlane/parse/__init__.py
+piel/tools/openlane/parse/run_output.py
 piel/tools/openlane/parse/sta_rpt.py
 piel/tools/openlane/parse/utils.py
+piel/tools/pyspice/__init__.py
+piel/tools/pyspice/component.py
 piel/tools/sax/__init__.py
 piel/tools/sax/utils.py
 piel/visual/__init__.py
 piel/visual/auto_plot_multiple.py
 piel/visual/data_conversion.py
 tests/__init__.py
 tests/test_piel.py
+tests/integration/test_gdsfactory_netlist.py
+tests/integration/test_gdsfactory_netlist_to_pyspice.py
 tests/models/logic/electro_optic/test_signal_mapping.py
 tests/tools/__init__.py
 tests/tools/gdsfactory/__init__.py
 tests/tools/gdsfactory/test_netlist.py
 tests/tools/sax/__init__.py
 tests/tools/sax/test_utils.py
 tests/visual/test_data_conversion.py
```

### Comparing `piel-0.0.41/setup.py` & `piel-0.0.43/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 #!/usr/bin/env python
 
 """The setup script."""
 
 from setuptools import setup, find_packages
 
-with open("README.md") as readme_file:
+with open("README.rst") as readme_file:
     readme = readme_file.read()
 
 requirements = [
     "bokeh",
     "jupyter_bokeh",
     "jupytext",
     "Click>=7.0",
     "cocotb",
     "gdsfactory",
+    "networkx",
     "openlane",
     "pandas",
     "pyspice",
     "sax",
-    "qutip",
+    "thewalrus" "qutip",
 ]
 
 test_requirements = [
     "pytest>=3",
 ]
 
 setup(
@@ -35,15 +36,15 @@
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
     ],
-    description="Photonic and electronic co-simulation system design tools interfaced with open-source design software like GDSFactory and OpenROAD.",
+    description="Photonic Integrated Electronics: microservices to codesign photonics, electronics, communications, quantum, and more.",
     entry_points={
         "console_scripts": [
             "piel=piel.cli:main",
         ],
     },
     extras_require={
         "develop": [
@@ -67,10 +68,10 @@
     include_package_data=True,
     keywords="piel",
     name="piel",
     packages=find_packages(include=["piel", "piel.*"]),
     test_suite="tests",
     tests_require=test_requirements,
     url="https://github.com/daquintero/piel",
-    version="0.0.41",
+    version="0.0.43",
     zip_safe=False,
 )
```

### Comparing `piel-0.0.41/tests/models/logic/electro_optic/test_signal_mapping.py` & `piel-0.0.43/tests/models/logic/electro_optic/test_signal_mapping.py`

 * *Files identical despite different names*

### Comparing `piel-0.0.41/tests/test_piel.py` & `piel-0.0.43/tests/test_piel.py`

 * *Files identical despite different names*

### Comparing `piel-0.0.41/tests/tools/gdsfactory/test_netlist.py` & `piel-0.0.43/tests/tools/gdsfactory/test_netlist.py`

 * *Files identical despite different names*

### Comparing `piel-0.0.41/tests/tools/sax/test_utils.py` & `piel-0.0.43/tests/tools/sax/test_utils.py`

 * *Files identical despite different names*

### Comparing `piel-0.0.41/tests/visual/test_data_conversion.py` & `piel-0.0.43/tests/visual/test_data_conversion.py`

 * *Files identical despite different names*

