# Comparing `tmp/quantify-scheduler-0.8.0.tar.gz` & `tmp/quantify-scheduler-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quantify-scheduler-0.8.0.tar", last modified: Wed Aug 10 16:23:49 2022, max compression
+gzip compressed data, was "quantify-scheduler-0.9.0.tar", last modified: Thu Oct  6 16:58:55 2022, max compression
```

## Comparing `quantify-scheduler-0.8.0.tar` & `quantify-scheduler-0.9.0.tar`

### file list

```diff
@@ -1,243 +1,301 @@
-drwxr-xr-x   0 rsoko     (1000) rsoko     (1000)        0 2022-08-10 16:23:49.899132 quantify-scheduler-0.8.0/
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)      857 2022-08-10 15:17:32.000000 quantify-scheduler-0.8.0/AUTHORS.rst
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)      695 2022-08-09 13:08:37.000000 quantify-scheduler-0.8.0/CONTRIBUTING.rst
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)     1516 2022-07-22 15:36:09.000000 quantify-scheduler-0.8.0/LICENSE
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)      262 2022-08-09 13:08:37.000000 quantify-scheduler-0.8.0/MANIFEST.in
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)    36870 2022-08-10 16:23:49.900129 quantify-scheduler-0.8.0/PKG-INFO
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)     3903 2022-08-09 13:08:37.000000 quantify-scheduler-0.8.0/README.rst
-drwxr-xr-x   0 rsoko     (1000) rsoko     (1000)        0 2022-08-10 16:23:49.511087 quantify-scheduler-0.8.0/docs/
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)      852 2022-06-17 14:16:43.000000 quantify-scheduler-0.8.0/docs/Makefile
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)       28 2022-08-09 13:08:37.000000 quantify-scheduler-0.8.0/docs/authors.rst
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)       58 2022-08-09 13:08:37.000000 quantify-scheduler-0.8.0/docs/bibliography.rst
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)       30 2022-08-09 13:08:37.000000 quantify-scheduler-0.8.0/docs/changelog.rst
--rwxr-xr-x   0 rsoko     (1000) rsoko     (1000)    14275 2022-08-10 15:17:32.000000 quantify-scheduler-0.8.0/docs/conf.py
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)       33 2022-08-09 13:08:37.000000 quantify-scheduler-0.8.0/docs/contributing.rst
-drwxr-xr-x   0 rsoko     (1000) rsoko     (1000)        0 2022-08-10 16:23:49.519396 quantify-scheduler-0.8.0/docs/images/
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)   566915 2022-06-17 14:16:43.000000 quantify-scheduler-0.8.0/docs/images/Chevron_experiment_comb.png
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)     2254 2022-06-17 14:16:43.000000 quantify-scheduler-0.8.0/docs/images/QUANTIFY-FAVICON_16.png
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)    11887 2022-06-17 14:16:43.000000 quantify-scheduler-0.8.0/docs/images/bell_circuit_QI.png
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)      504 2022-08-09 13:08:37.000000 quantify-scheduler-0.8.0/docs/index.rst
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)     1896 2022-08-09 13:08:37.000000 quantify-scheduler-0.8.0/docs/installation.rst
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)     1269 2022-06-17 14:16:43.000000 quantify-scheduler-0.8.0/docs/make.bat
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)       27 2022-08-09 13:08:37.000000 quantify-scheduler-0.8.0/docs/readme.rst
-drwxr-xr-x   0 rsoko     (1000) rsoko     (1000)        0 2022-08-10 16:23:49.454380 quantify-scheduler-0.8.0/docs/tutorials/
-drwxr-xr-x   0 rsoko     (1000) rsoko     (1000)        0 2022-08-10 16:23:49.528513 quantify-scheduler-0.8.0/docs/tutorials/qblox/
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)     3506 2022-08-09 13:08:37.000000 quantify-scheduler-0.8.0/docs/tutorials/qblox/Cluster.rst
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)     1161 2022-08-10 15:17:32.000000 quantify-scheduler-0.8.0/docs/tutorials/qblox/How to use.rst
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)    14651 2022-08-09 13:08:37.000000 quantify-scheduler-0.8.0/docs/tutorials/qblox/Pulsar.rst
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)     2334 2022-08-10 15:17:32.000000 quantify-scheduler-0.8.0/docs/tutorials/qblox/index.rst
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)     3408 2022-08-10 15:17:32.000000 quantify-scheduler-0.8.0/docs/tutorials/qblox/recent.rst
-drwxr-xr-x   0 rsoko     (1000) rsoko     (1000)        0 2022-08-10 16:23:49.530836 quantify-scheduler-0.8.0/docs/tutorials/zhinst/
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)    14471 2022-08-09 13:08:37.000000 quantify-scheduler-0.8.0/docs/tutorials/zhinst/index.rst
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)    24216 2022-08-09 13:08:37.000000 quantify-scheduler-0.8.0/docs/user_guide.rst
-drwxr-xr-x   0 rsoko     (1000) rsoko     (1000)        0 2022-08-10 16:23:49.550644 quantify-scheduler-0.8.0/quantify_scheduler/
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)      845 2022-08-10 15:19:54.000000 quantify-scheduler-0.8.0/quantify_scheduler/__init__.py
-drwxr-xr-x   0 rsoko     (1000) rsoko     (1000)        0 2022-08-10 16:23:49.571379 quantify-scheduler-0.8.0/quantify_scheduler/backends/
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)        0 2022-07-12 13:23:48.000000 quantify-scheduler-0.8.0/quantify_scheduler/backends/__init__.py
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)    13641 2022-08-04 21:07:03.000000 quantify-scheduler-0.8.0/quantify_scheduler/backends/circuit_to_device.py
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)     7434 2022-07-22 15:36:09.000000 quantify-scheduler-0.8.0/quantify_scheduler/backends/corrections.py
-drwxr-xr-x   0 rsoko     (1000) rsoko     (1000)        0 2022-08-10 16:23:49.592399 quantify-scheduler-0.8.0/quantify_scheduler/backends/qblox/
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)        0 2022-06-17 14:16:43.000000 quantify-scheduler-0.8.0/quantify_scheduler/backends/qblox/__init__.py
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)    57545 2022-08-01 11:59:21.000000 quantify-scheduler-0.8.0/quantify_scheduler/backends/qblox/compiler_abc.py
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)     6654 2022-07-22 15:36:09.000000 quantify-scheduler-0.8.0/quantify_scheduler/backends/qblox/compiler_container.py
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)     2816 2022-07-27 16:52:22.000000 quantify-scheduler-0.8.0/quantify_scheduler/backends/qblox/constants.py
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)     2309 2022-08-10 12:37:45.000000 quantify-scheduler-0.8.0/quantify_scheduler/backends/qblox/driver_version_check.py
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)    20313 2022-08-10 15:17:32.000000 quantify-scheduler-0.8.0/quantify_scheduler/backends/qblox/helpers.py
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)    12340 2022-07-22 15:36:09.000000 quantify-scheduler-0.8.0/quantify_scheduler/backends/qblox/instrument_compilers.py
-drwxr-xr-x   0 rsoko     (1000) rsoko     (1000)        0 2022-08-10 16:23:49.605127 quantify-scheduler-0.8.0/quantify_scheduler/backends/qblox/operation_handling/
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)        0 2022-06-17 14:16:43.000000 quantify-scheduler-0.8.0/quantify_scheduler/backends/qblox/operation_handling/__init__.py
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)    10398 2022-06-17 14:16:43.000000 quantify-scheduler-0.8.0/quantify_scheduler/backends/qblox/operation_handling/acquisitions.py
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)     1451 2022-06-17 14:16:43.000000 quantify-scheduler-0.8.0/quantify_scheduler/backends/qblox/operation_handling/base.py
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)     3247 2022-08-10 15:17:32.000000 quantify-scheduler-0.8.0/quantify_scheduler/backends/qblox/operation_handling/factory.py
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)    17720 2022-08-10 15:17:32.000000 quantify-scheduler-0.8.0/quantify_scheduler/backends/qblox/operation_handling/pulses.py
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)     2565 2022-08-10 15:17:32.000000 quantify-scheduler-0.8.0/quantify_scheduler/backends/qblox/operation_handling/virtual.py
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)     1026 2022-06-17 14:16:43.000000 quantify-scheduler-0.8.0/quantify_scheduler/backends/qblox/q1asm_instructions.py
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)    19430 2022-08-10 15:17:32.000000 quantify-scheduler-0.8.0/quantify_scheduler/backends/qblox/qasm_program.py
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)     3580 2022-06-17 14:16:43.000000 quantify-scheduler-0.8.0/quantify_scheduler/backends/qblox/register_manager.py
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)     3465 2022-08-10 15:17:32.000000 quantify-scheduler-0.8.0/quantify_scheduler/backends/qblox_backend.py
-drwxr-xr-x   0 rsoko     (1000) rsoko     (1000)        0 2022-08-10 16:23:49.613053 quantify-scheduler-0.8.0/quantify_scheduler/backends/types/
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)        0 2022-06-17 14:16:43.000000 quantify-scheduler-0.8.0/quantify_scheduler/backends/types/__init__.py
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)     3175 2022-06-17 14:16:43.000000 quantify-scheduler-0.8.0/quantify_scheduler/backends/types/common.py
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)    14789 2022-08-01 11:59:21.000000 quantify-scheduler-0.8.0/quantify_scheduler/backends/types/qblox.py
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)     8766 2022-06-17 14:16:43.000000 quantify-scheduler-0.8.0/quantify_scheduler/backends/types/zhinst.py
-drwxr-xr-x   0 rsoko     (1000) rsoko     (1000)        0 2022-08-10 16:23:49.623385 quantify-scheduler-0.8.0/quantify_scheduler/backends/zhinst/
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)        0 2022-06-17 14:16:43.000000 quantify-scheduler-0.8.0/quantify_scheduler/backends/zhinst/__init__.py
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)     9324 2022-06-17 14:16:43.000000 quantify-scheduler-0.8.0/quantify_scheduler/backends/zhinst/helpers.py
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)     1634 2022-06-17 14:16:43.000000 quantify-scheduler-0.8.0/quantify_scheduler/backends/zhinst/resolvers.py
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)    20692 2022-06-17 14:16:43.000000 quantify-scheduler-0.8.0/quantify_scheduler/backends/zhinst/seqc_il_generator.py
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)    29146 2022-06-17 14:16:43.000000 quantify-scheduler-0.8.0/quantify_scheduler/backends/zhinst/settings.py
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)    63691 2022-07-12 13:23:48.000000 quantify-scheduler-0.8.0/quantify_scheduler/backends/zhinst_backend.py
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)    19060 2022-08-10 15:17:32.000000 quantify-scheduler-0.8.0/quantify_scheduler/compilation.py
-drwxr-xr-x   0 rsoko     (1000) rsoko     (1000)        0 2022-08-10 16:23:49.635389 quantify-scheduler-0.8.0/quantify_scheduler/device_under_test/
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)      386 2022-06-17 14:16:43.000000 quantify-scheduler-0.8.0/quantify_scheduler/device_under_test/__init__.py
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)     4466 2022-07-22 15:36:09.000000 quantify-scheduler-0.8.0/quantify_scheduler/device_under_test/composite_square_edge.py
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)      708 2022-06-17 14:16:43.000000 quantify-scheduler-0.8.0/quantify_scheduler/device_under_test/device_element.py
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)     1982 2022-07-22 15:36:09.000000 quantify-scheduler-0.8.0/quantify_scheduler/device_under_test/edge.py
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)     8754 2022-08-10 12:07:11.000000 quantify-scheduler-0.8.0/quantify_scheduler/device_under_test/quantum_device.py
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)    25149 2022-08-10 15:17:32.000000 quantify-scheduler-0.8.0/quantify_scheduler/device_under_test/transmon_element.py
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)     1949 2022-06-17 14:16:43.000000 quantify-scheduler-0.8.0/quantify_scheduler/enums.py
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)      314 2022-06-17 14:16:43.000000 quantify-scheduler-0.8.0/quantify_scheduler/frontends.py
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)    16202 2022-07-27 16:52:22.000000 quantify-scheduler-0.8.0/quantify_scheduler/gettables.py
-drwxr-xr-x   0 rsoko     (1000) rsoko     (1000)        0 2022-08-10 16:23:49.652784 quantify-scheduler-0.8.0/quantify_scheduler/helpers/
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)       58 2022-06-17 14:16:43.000000 quantify-scheduler-0.8.0/quantify_scheduler/helpers/__init__.py
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)     1637 2022-06-17 14:16:43.000000 quantify-scheduler-0.8.0/quantify_scheduler/helpers/collections.py
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)      547 2022-06-17 14:16:43.000000 quantify-scheduler-0.8.0/quantify_scheduler/helpers/importers.py
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)     1191 2022-06-17 14:16:43.000000 quantify-scheduler-0.8.0/quantify_scheduler/helpers/inspect.py
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)     1674 2022-07-22 15:36:09.000000 quantify-scheduler-0.8.0/quantify_scheduler/helpers/mock_instruments.py
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)    14459 2022-08-09 23:10:16.000000 quantify-scheduler-0.8.0/quantify_scheduler/helpers/schedule.py
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)      872 2022-06-17 14:16:43.000000 quantify-scheduler-0.8.0/quantify_scheduler/helpers/time.py
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)     2119 2022-06-17 14:16:43.000000 quantify-scheduler-0.8.0/quantify_scheduler/helpers/validators.py
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)    15226 2022-06-17 14:16:43.000000 quantify-scheduler-0.8.0/quantify_scheduler/helpers/waveforms.py
-drwxr-xr-x   0 rsoko     (1000) rsoko     (1000)        0 2022-08-10 16:23:49.660398 quantify-scheduler-0.8.0/quantify_scheduler/instrument_coordinator/
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)      562 2022-07-22 15:36:09.000000 quantify-scheduler-0.8.0/quantify_scheduler/instrument_coordinator/__init__.py
-drwxr-xr-x   0 rsoko     (1000) rsoko     (1000)        0 2022-08-10 16:23:49.676046 quantify-scheduler-0.8.0/quantify_scheduler/instrument_coordinator/components/
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)      463 2022-06-17 14:16:43.000000 quantify-scheduler-0.8.0/quantify_scheduler/instrument_coordinator/components/__init__.py
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)     4316 2022-06-17 14:16:43.000000 quantify-scheduler-0.8.0/quantify_scheduler/instrument_coordinator/components/base.py
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)     5137 2022-06-17 14:16:43.000000 quantify-scheduler-0.8.0/quantify_scheduler/instrument_coordinator/components/generic.py
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)    42388 2022-08-08 08:58:32.000000 quantify-scheduler-0.8.0/quantify_scheduler/instrument_coordinator/components/qblox.py
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)    10816 2022-06-17 14:16:43.000000 quantify-scheduler-0.8.0/quantify_scheduler/instrument_coordinator/components/zhinst.py
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)    14970 2022-06-17 14:16:43.000000 quantify-scheduler-0.8.0/quantify_scheduler/instrument_coordinator/instrument_coordinator.py
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)     2593 2022-06-17 14:16:43.000000 quantify-scheduler-0.8.0/quantify_scheduler/instrument_coordinator/utility.py
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)     9146 2022-08-10 12:37:45.000000 quantify-scheduler-0.8.0/quantify_scheduler/json_utils.py
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)      768 2022-06-17 14:16:43.000000 quantify-scheduler-0.8.0/quantify_scheduler/math.py
-drwxr-xr-x   0 rsoko     (1000) rsoko     (1000)        0 2022-08-10 16:23:49.697385 quantify-scheduler-0.8.0/quantify_scheduler/operations/
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)      425 2022-06-17 14:16:43.000000 quantify-scheduler-0.8.0/quantify_scheduler/operations/__init__.py
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)    18175 2022-06-17 14:16:43.000000 quantify-scheduler-0.8.0/quantify_scheduler/operations/acquisition_library.py
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)    17533 2022-08-10 15:17:32.000000 quantify-scheduler-0.8.0/quantify_scheduler/operations/gate_library.py
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)     3525 2022-08-10 15:17:32.000000 quantify-scheduler-0.8.0/quantify_scheduler/operations/measurement_factories.py
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)    12318 2022-08-10 12:37:45.000000 quantify-scheduler-0.8.0/quantify_scheduler/operations/operation.py
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)     3275 2022-08-10 15:17:32.000000 quantify-scheduler-0.8.0/quantify_scheduler/operations/pulse_factories.py
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)    27848 2022-08-10 15:17:32.000000 quantify-scheduler-0.8.0/quantify_scheduler/operations/pulse_library.py
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)     4763 2022-08-10 12:37:45.000000 quantify-scheduler-0.8.0/quantify_scheduler/resources.py
-drwxr-xr-x   0 rsoko     (1000) rsoko     (1000)        0 2022-08-10 16:23:49.714809 quantify-scheduler-0.8.0/quantify_scheduler/schedules/
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)      463 2022-06-17 14:16:43.000000 quantify-scheduler-0.8.0/quantify_scheduler/schedules/__init__.py
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)    34079 2022-08-10 15:17:32.000000 quantify-scheduler-0.8.0/quantify_scheduler/schedules/schedule.py
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)     5815 2022-06-17 14:16:43.000000 quantify-scheduler-0.8.0/quantify_scheduler/schedules/spectroscopy_schedules.py
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)    15859 2022-06-17 14:16:43.000000 quantify-scheduler-0.8.0/quantify_scheduler/schedules/timedomain_schedules.py
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)     6231 2022-08-08 08:58:32.000000 quantify-scheduler-0.8.0/quantify_scheduler/schedules/trace_schedules.py
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)    10478 2022-06-17 14:16:43.000000 quantify-scheduler-0.8.0/quantify_scheduler/schedules/verification.py
-drwxr-xr-x   0 rsoko     (1000) rsoko     (1000)        0 2022-08-10 16:23:49.725079 quantify-scheduler-0.8.0/quantify_scheduler/schemas/
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)        0 2022-06-17 14:16:43.000000 quantify-scheduler-0.8.0/quantify_scheduler/schemas/__init__.py
-drwxr-xr-x   0 rsoko     (1000) rsoko     (1000)        0 2022-08-10 16:23:49.735290 quantify-scheduler-0.8.0/quantify_scheduler/schemas/examples/
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)        0 2022-06-17 14:16:43.000000 quantify-scheduler-0.8.0/quantify_scheduler/schemas/examples/__init__.py
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)     4073 2022-07-22 15:36:09.000000 quantify-scheduler-0.8.0/quantify_scheduler/schemas/examples/circuit_to_device_example_cfgs.py
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)     6160 2022-08-01 11:59:21.000000 quantify-scheduler-0.8.0/quantify_scheduler/schemas/examples/qblox_test_mapping.json
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)     5478 2022-07-22 15:36:09.000000 quantify-scheduler-0.8.0/quantify_scheduler/schemas/examples/transmon_test_config.json
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)      694 2022-06-17 14:16:43.000000 quantify-scheduler-0.8.0/quantify_scheduler/schemas/examples/utils.py
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)     3495 2022-07-12 13:23:48.000000 quantify-scheduler-0.8.0/quantify_scheduler/schemas/examples/zhinst_test_mapping.json
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)     6013 2022-06-17 14:16:43.000000 quantify-scheduler-0.8.0/quantify_scheduler/schemas/operation.json
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)      468 2022-06-17 14:16:43.000000 quantify-scheduler-0.8.0/quantify_scheduler/schemas/resource.json
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)     1324 2022-06-17 14:16:43.000000 quantify-scheduler-0.8.0/quantify_scheduler/schemas/schedulable.json
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)     1144 2022-06-17 14:16:43.000000 quantify-scheduler-0.8.0/quantify_scheduler/schemas/schedule.json
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)     1126 2022-06-17 14:16:43.000000 quantify-scheduler-0.8.0/quantify_scheduler/schemas/transmon_cfg.json
-drwxr-xr-x   0 rsoko     (1000) rsoko     (1000)        0 2022-08-10 16:23:49.738232 quantify-scheduler-0.8.0/quantify_scheduler/structure/
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)      299 2022-06-17 14:16:43.000000 quantify-scheduler-0.8.0/quantify_scheduler/structure/__init__.py
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)     2138 2022-08-09 13:08:37.000000 quantify-scheduler-0.8.0/quantify_scheduler/structure/model.py
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)        0 2022-06-17 14:16:43.000000 quantify-scheduler-0.8.0/quantify_scheduler/types.py
-drwxr-xr-x   0 rsoko     (1000) rsoko     (1000)        0 2022-08-10 16:23:49.747997 quantify-scheduler-0.8.0/quantify_scheduler/visualization/
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)        0 2022-06-17 14:16:43.000000 quantify-scheduler-0.8.0/quantify_scheduler/visualization/__init__.py
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)    10092 2022-06-17 14:16:43.000000 quantify-scheduler-0.8.0/quantify_scheduler/visualization/circuit_diagram.py
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)      506 2022-06-17 14:16:43.000000 quantify-scheduler-0.8.0/quantify_scheduler/visualization/constants.py
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)    19596 2022-06-17 14:16:43.000000 quantify-scheduler-0.8.0/quantify_scheduler/visualization/pulse_diagram.py
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)     9786 2022-06-17 14:16:43.000000 quantify-scheduler-0.8.0/quantify_scheduler/visualization/pulse_scheme.py
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)    10943 2022-07-22 15:36:09.000000 quantify-scheduler-0.8.0/quantify_scheduler/waveforms.py
-drwxr-xr-x   0 rsoko     (1000) rsoko     (1000)        0 2022-08-10 16:23:49.562418 quantify-scheduler-0.8.0/quantify_scheduler.egg-info/
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)    36870 2022-08-10 16:23:48.000000 quantify-scheduler-0.8.0/quantify_scheduler.egg-info/PKG-INFO
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)     9040 2022-08-10 16:23:49.000000 quantify-scheduler-0.8.0/quantify_scheduler.egg-info/SOURCES.txt
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)        1 2022-08-10 16:23:48.000000 quantify-scheduler-0.8.0/quantify_scheduler.egg-info/dependency_links.txt
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)        1 2022-06-30 16:39:07.000000 quantify-scheduler-0.8.0/quantify_scheduler.egg-info/not-zip-safe
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)      250 2022-08-10 16:23:48.000000 quantify-scheduler-0.8.0/quantify_scheduler.egg-info/requires.txt
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)       19 2022-08-10 16:23:48.000000 quantify-scheduler-0.8.0/quantify_scheduler.egg-info/top_level.txt
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)      421 2022-08-10 16:23:49.903177 quantify-scheduler-0.8.0/setup.cfg
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)     2063 2022-08-10 15:19:54.000000 quantify-scheduler-0.8.0/setup.py
-drwxr-xr-x   0 rsoko     (1000) rsoko     (1000)        0 2022-08-10 16:23:49.754532 quantify-scheduler-0.8.0/tests/
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)        0 2022-06-17 14:16:43.000000 quantify-scheduler-0.8.0/tests/__init__.py
-drwxr-xr-x   0 rsoko     (1000) rsoko     (1000)        0 2022-08-10 16:23:49.771234 quantify-scheduler-0.8.0/tests/baseline_images/
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)    40694 2022-06-17 14:16:43.000000 quantify-scheduler-0.8.0/tests/baseline_images/test_hybrid_circuit_acquisitions_matplotlib.png
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)    47781 2022-06-17 14:16:43.000000 quantify-scheduler-0.8.0/tests/baseline_images/test_hybrid_circuit_diagram_baseband_matplotlib.png
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)    37124 2022-06-17 14:16:43.000000 quantify-scheduler-0.8.0/tests/baseline_images/test_hybrid_circuit_diagram_matplotlib.png
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)    53383 2022-06-17 14:16:43.000000 quantify-scheduler-0.8.0/tests/baseline_images/test_hybrid_circuit_diagram_modulated_matplotlib.png
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)    59476 2022-06-17 14:16:43.000000 quantify-scheduler-0.8.0/tests/baseline_images/test_hybrid_circuit_diagram_unknown_port_matplotlib.png
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)    73409 2022-06-17 14:16:43.000000 quantify-scheduler-0.8.0/tests/baseline_images/test_plot_pulses_n_q.png
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)    22113 2022-06-17 14:16:43.000000 quantify-scheduler-0.8.0/tests/baseline_images/test_plot_pulses_single_q.png
-drwxr-xr-x   0 rsoko     (1000) rsoko     (1000)        0 2022-08-10 16:23:49.777834 quantify-scheduler-0.8.0/tests/baseline_qblox_assembly/
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)    20682 2022-08-10 12:37:45.000000 quantify-scheduler-0.8.0/tests/baseline_qblox_assembly/AllXY_qrm0_seq0_instr.json
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)     9952 2022-08-10 12:37:45.000000 quantify-scheduler-0.8.0/tests/baseline_qblox_assembly/Readout calibration q0, [0, 1]_qrm0_seq0_instr.json
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)     1817 2022-06-17 14:16:43.000000 quantify-scheduler-0.8.0/tests/baseline_qblox_assembly/sched-looped-acq_qrm0_seq0_instr.json
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)      355 2022-06-17 14:16:43.000000 quantify-scheduler-0.8.0/tests/conftest.py
-drwxr-xr-x   0 rsoko     (1000) rsoko     (1000)        0 2022-08-10 16:23:49.784786 quantify-scheduler-0.8.0/tests/fixtures/
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)        0 2022-06-17 14:16:43.000000 quantify-scheduler-0.8.0/tests/fixtures/__init__.py
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)     4484 2022-08-10 14:24:37.000000 quantify-scheduler-0.8.0/tests/fixtures/mock_setup.py
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)      456 2022-06-17 14:16:43.000000 quantify-scheduler-0.8.0/tests/fixtures/qcodes_utilities.py
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)     5922 2022-08-10 12:37:45.000000 quantify-scheduler-0.8.0/tests/fixtures/schedule.py
-drwxr-xr-x   0 rsoko     (1000) rsoko     (1000)        0 2022-08-10 16:23:49.810275 quantify-scheduler-0.8.0/tests/scheduler/
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)        0 2022-06-17 14:16:43.000000 quantify-scheduler-0.8.0/tests/scheduler/__init__.py
-drwxr-xr-x   0 rsoko     (1000) rsoko     (1000)        0 2022-08-10 16:23:49.817923 quantify-scheduler-0.8.0/tests/scheduler/backends/
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)        0 2022-06-17 14:16:43.000000 quantify-scheduler-0.8.0/tests/scheduler/backends/__init__.py
-drwxr-xr-x   0 rsoko     (1000) rsoko     (1000)        0 2022-08-10 16:23:49.823468 quantify-scheduler-0.8.0/tests/scheduler/backends/qblox/
-drwxr-xr-x   0 rsoko     (1000) rsoko     (1000)        0 2022-08-10 16:23:49.832314 quantify-scheduler-0.8.0/tests/scheduler/backends/qblox/operation_handling/
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)    17612 2022-08-08 08:58:32.000000 quantify-scheduler-0.8.0/tests/scheduler/backends/qblox/operation_handling/test_acquisitions.py
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)     5737 2022-06-17 14:16:43.000000 quantify-scheduler-0.8.0/tests/scheduler/backends/qblox/operation_handling/test_factory.py
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)    20416 2022-06-17 14:16:43.000000 quantify-scheduler-0.8.0/tests/scheduler/backends/qblox/operation_handling/test_pulses.py
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)     4143 2022-08-10 15:17:32.000000 quantify-scheduler-0.8.0/tests/scheduler/backends/qblox/operation_handling/test_virtual.py
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)     1720 2022-06-17 14:16:43.000000 quantify-scheduler-0.8.0/tests/scheduler/backends/qblox/test_driver_version_check.py
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)     1278 2022-07-22 15:36:09.000000 quantify-scheduler-0.8.0/tests/scheduler/backends/qblox/test_helpers_qblox.py
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)     1992 2022-06-17 14:16:43.000000 quantify-scheduler-0.8.0/tests/scheduler/backends/qblox/test_register_manager.py
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)    12591 2022-07-12 13:23:48.000000 quantify-scheduler-0.8.0/tests/scheduler/backends/test_circuit_to_device.py
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)    69003 2022-08-10 15:17:32.000000 quantify-scheduler-0.8.0/tests/scheduler/backends/test_qblox_backend.py
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)    37127 2022-08-10 12:37:45.000000 quantify-scheduler-0.8.0/tests/scheduler/backends/test_zhinst_backend.py
-drwxr-xr-x   0 rsoko     (1000) rsoko     (1000)        0 2022-08-10 16:23:49.842484 quantify-scheduler-0.8.0/tests/scheduler/backends/zhinst/
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)    12451 2022-06-17 14:16:43.000000 quantify-scheduler-0.8.0/tests/scheduler/backends/zhinst/test_helpers.py
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)     2116 2022-06-17 14:16:43.000000 quantify-scheduler-0.8.0/tests/scheduler/backends/zhinst/test_resolvers.py
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)     6210 2022-06-17 14:16:43.000000 quantify-scheduler-0.8.0/tests/scheduler/backends/zhinst/test_seqc_il_generator.py
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)    16093 2022-06-17 14:16:43.000000 quantify-scheduler-0.8.0/tests/scheduler/backends/zhinst/test_settings.py
-drwxr-xr-x   0 rsoko     (1000) rsoko     (1000)        0 2022-08-10 16:23:49.848754 quantify-scheduler-0.8.0/tests/scheduler/device_under_test/
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)     2288 2022-07-22 15:36:09.000000 quantify-scheduler-0.8.0/tests/scheduler/device_under_test/test_composite_square_edge.py
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)     2660 2022-08-10 12:07:11.000000 quantify-scheduler-0.8.0/tests/scheduler/device_under_test/test_quantum_device.py
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)     2425 2022-08-10 12:07:11.000000 quantify-scheduler-0.8.0/tests/scheduler/device_under_test/test_transmon_element.py
-drwxr-xr-x   0 rsoko     (1000) rsoko     (1000)        0 2022-08-10 16:23:49.856219 quantify-scheduler-0.8.0/tests/scheduler/helpers/
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)        0 2022-06-17 14:16:43.000000 quantify-scheduler-0.8.0/tests/scheduler/helpers/__init__.py
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)      488 2022-06-17 14:16:43.000000 quantify-scheduler-0.8.0/tests/scheduler/helpers/test_inspect.py
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)    16223 2022-08-10 12:37:45.000000 quantify-scheduler-0.8.0/tests/scheduler/helpers/test_schedule.py
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)    11434 2022-08-10 12:37:45.000000 quantify-scheduler-0.8.0/tests/scheduler/helpers/test_waveforms.py
-drwxr-xr-x   0 rsoko     (1000) rsoko     (1000)        0 2022-08-10 16:23:49.861790 quantify-scheduler-0.8.0/tests/scheduler/instrument_coordinator/
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)        0 2022-06-17 14:16:43.000000 quantify-scheduler-0.8.0/tests/scheduler/instrument_coordinator/__init__.py
-drwxr-xr-x   0 rsoko     (1000) rsoko     (1000)        0 2022-08-10 16:23:49.870217 quantify-scheduler-0.8.0/tests/scheduler/instrument_coordinator/components/
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)        0 2022-06-17 14:16:43.000000 quantify-scheduler-0.8.0/tests/scheduler/instrument_coordinator/components/__init__.py
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)     3140 2022-07-22 15:36:09.000000 quantify-scheduler-0.8.0/tests/scheduler/instrument_coordinator/components/test_generic.py
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)    27546 2022-08-10 12:37:45.000000 quantify-scheduler-0.8.0/tests/scheduler/instrument_coordinator/components/test_qblox.py
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)     9072 2022-06-17 14:16:43.000000 quantify-scheduler-0.8.0/tests/scheduler/instrument_coordinator/components/test_zhinst.py
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)    11418 2022-06-17 14:16:43.000000 quantify-scheduler-0.8.0/tests/scheduler/instrument_coordinator/test_instrument_coordinator.py
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)     3675 2022-06-17 14:16:43.000000 quantify-scheduler-0.8.0/tests/scheduler/instrument_coordinator/test_utility.py
-drwxr-xr-x   0 rsoko     (1000) rsoko     (1000)        0 2022-08-10 16:23:49.886424 quantify-scheduler-0.8.0/tests/scheduler/schedules/
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)        0 2022-06-17 14:16:43.000000 quantify-scheduler-0.8.0/tests/scheduler/schedules/__init__.py
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)      989 2022-08-10 12:37:45.000000 quantify-scheduler-0.8.0/tests/scheduler/schedules/compiles_all_backends.py
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)     2019 2022-06-17 14:16:43.000000 quantify-scheduler-0.8.0/tests/scheduler/schedules/test_schedule_plotting_matplotlib.py
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)     3202 2022-06-17 14:16:43.000000 quantify-scheduler-0.8.0/tests/scheduler/schedules/test_schedule_sampling.py
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)     3845 2022-08-10 12:37:45.000000 quantify-scheduler-0.8.0/tests/scheduler/schedules/test_spectroscopy_schedules.py
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)    16370 2022-08-10 12:37:45.000000 quantify-scheduler-0.8.0/tests/scheduler/schedules/test_timedomain_schedules.py
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)     4480 2022-08-08 08:58:32.000000 quantify-scheduler-0.8.0/tests/scheduler/schedules/test_trace_schedules.py
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)     6245 2022-08-10 12:07:11.000000 quantify-scheduler-0.8.0/tests/scheduler/schedules/test_verification.py
-drwxr-xr-x   0 rsoko     (1000) rsoko     (1000)        0 2022-08-10 16:23:49.888380 quantify-scheduler-0.8.0/tests/scheduler/schemas/
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)        0 2022-06-17 14:16:43.000000 quantify-scheduler-0.8.0/tests/scheduler/schemas/__init__.py
-drwxr-xr-x   0 rsoko     (1000) rsoko     (1000)        0 2022-08-10 16:23:49.890575 quantify-scheduler-0.8.0/tests/scheduler/schemas/examples/
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)        0 2022-06-17 14:16:43.000000 quantify-scheduler-0.8.0/tests/scheduler/schemas/examples/__init__.py
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)      470 2022-06-17 14:16:43.000000 quantify-scheduler-0.8.0/tests/scheduler/schemas/examples/test_utils.py
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)     5891 2022-07-22 12:53:28.000000 quantify-scheduler-0.8.0/tests/scheduler/test_acquisition_library.py
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)    10672 2022-08-10 12:37:45.000000 quantify-scheduler-0.8.0/tests/scheduler/test_compilation.py
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)     5728 2022-07-22 15:36:09.000000 quantify-scheduler-0.8.0/tests/scheduler/test_corrections.py
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)     5861 2022-08-05 12:31:07.000000 quantify-scheduler-0.8.0/tests/scheduler/test_gate_library.py
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)    13705 2022-08-10 12:07:11.000000 quantify-scheduler-0.8.0/tests/scheduler/test_gettables.py
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)     2378 2022-08-08 08:58:32.000000 quantify-scheduler-0.8.0/tests/scheduler/test_json_utils.py
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)      498 2022-06-17 14:16:43.000000 quantify-scheduler-0.8.0/tests/scheduler/test_math.py
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)    10346 2022-08-10 15:17:32.000000 quantify-scheduler-0.8.0/tests/scheduler/test_pulse_library.py
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)      742 2022-06-17 14:16:43.000000 quantify-scheduler-0.8.0/tests/scheduler/test_resources.py
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)      716 2022-06-17 14:16:43.000000 quantify-scheduler-0.8.0/tests/scheduler/test_structure.py
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)    14101 2022-08-10 15:17:32.000000 quantify-scheduler-0.8.0/tests/scheduler/test_types.py
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)     5078 2022-06-17 14:16:43.000000 quantify-scheduler-0.8.0/tests/scheduler/test_waveforms.py
-drwxr-xr-x   0 rsoko     (1000) rsoko     (1000)        0 2022-08-10 16:23:49.897622 quantify-scheduler-0.8.0/tests/scheduler/visualization/
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)        0 2022-06-17 14:16:43.000000 quantify-scheduler-0.8.0/tests/scheduler/visualization/__init__.py
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)     3325 2022-06-17 14:16:43.000000 quantify-scheduler-0.8.0/tests/scheduler/visualization/test_circuit_diagram.py
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)     1331 2022-08-10 12:07:11.000000 quantify-scheduler-0.8.0/tests/scheduler/visualization/test_pulse_diagram.py
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)     1936 2022-06-17 14:16:43.000000 quantify-scheduler-0.8.0/tests/scheduler/visualization/test_pulse_scheme.py
--rw-r--r--   0 rsoko     (1000) rsoko     (1000)     2151 2022-06-17 14:16:43.000000 quantify-scheduler-0.8.0/tests/test_headers_and_copyright.py
+drwxrwxrwx   0        0        0        0 2022-10-06 16:58:55.999461 quantify-scheduler-0.9.0/
+-rw-rw-rw-   0        0        0     1050 2022-10-06 16:36:21.000000 quantify-scheduler-0.9.0/AUTHORS.md
+-rw-rw-rw-   0        0        0      656 2022-09-22 07:22:36.000000 quantify-scheduler-0.9.0/CONTRIBUTING.md
+-rw-rw-rw-   0        0        0     1516 2022-09-22 07:22:36.000000 quantify-scheduler-0.9.0/LICENSE
+-rw-rw-rw-   0        0        0      263 2022-09-22 07:22:36.000000 quantify-scheduler-0.9.0/MANIFEST.in
+-rw-rw-rw-   0        0        0    38382 2022-10-06 16:58:55.999461 quantify-scheduler-0.9.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3527 2022-10-05 11:24:37.000000 quantify-scheduler-0.9.0/README.md
+drwxrwxrwx   0        0        0        0 2022-10-06 16:58:55.714631 quantify-scheduler-0.9.0/docs/
+-rw-rw-rw-   0        0        0      852 2022-09-22 07:22:36.000000 quantify-scheduler-0.9.0/docs/Makefile
+drwxrwxrwx   0        0        0        0 2022-10-06 16:58:55.682795 quantify-scheduler-0.9.0/docs/_build/
+drwxrwxrwx   0        0        0        0 2022-10-06 16:58:55.682795 quantify-scheduler-0.9.0/docs/_build/html/
+drwxrwxrwx   0        0        0        0 2022-10-06 16:58:55.682795 quantify-scheduler-0.9.0/docs/_build/html/_downloads/
+drwxrwxrwx   0        0        0        0 2022-10-06 16:58:55.714631 quantify-scheduler-0.9.0/docs/_build/html/_downloads/dbb6a6669e687c562a8e08fc71962895/
+-rw-rw-rw-   0        0        0    14970 2022-10-05 19:33:42.000000 quantify-scheduler-0.9.0/docs/_build/html/_downloads/dbb6a6669e687c562a8e08fc71962895/quantify-validate-qblox.md
+drwxrwxrwx   0        0        0        0 2022-10-06 16:58:55.725344 quantify-scheduler-0.9.0/docs/_build/html/_images/
+-rw-rw-rw-   0        0        0    18578 2022-10-05 11:16:13.000000 quantify-scheduler-0.9.0/docs/_build/html/_images/03469962d7b549171a37aa0d94269bb6dcda55db16706b84f1736daeb14f191e.png
+-rw-rw-rw-   0        0        0    20797 2022-10-05 11:16:13.000000 quantify-scheduler-0.9.0/docs/_build/html/_images/23bb4479dc5ade89b3bfdec9f0ed2fd1beec4881c243be131083ac64c3c12ca3.png
+-rw-rw-rw-   0        0        0    15718 2022-10-05 11:16:13.000000 quantify-scheduler-0.9.0/docs/_build/html/_images/304514e0b7f2a94fe918a5566d29137a0fe07b5e6c3ad871564c3cba73156220.png
+-rw-rw-rw-   0        0        0    20387 2022-10-05 11:16:44.000000 quantify-scheduler-0.9.0/docs/_build/html/_images/315b2d3264215202641421edfbef4755692b49ab97b190975c61c618fd9946ad.png
+-rw-rw-rw-   0        0        0    54934 2022-10-05 11:24:34.000000 quantify-scheduler-0.9.0/docs/_build/html/_images/QRM_only_-_Trace_plot.png
+-rw-rw-rw-   0        0        0    11707 2022-10-05 11:16:13.000000 quantify-scheduler-0.9.0/docs/_build/html/_images/c2a231508f8856a2a1910e2f4304c19999a856684dade344e269c28e61bd1630.png
+-rw-rw-rw-   0        0        0    11320 2022-10-05 11:16:44.000000 quantify-scheduler-0.9.0/docs/_build/html/_images/c50c688eb70c2c69386b99b5c2e0a5077b5c33923744ed273166c25a2451f34e.png
+-rw-rw-rw-   0        0        0    45436 2022-10-05 11:15:15.000000 quantify-scheduler-0.9.0/docs/_build/html/_images/d09ad7bd99b334ca3e1b6472498bd275c53ad6e319df6707f10bbf100ec1adad.png
+drwxrwxrwx   0        0        0        0 2022-10-06 16:58:55.730585 quantify-scheduler-0.9.0/docs/_build/html/_static/
+-rw-rw-rw-   0        0        0     2254 2022-02-07 13:26:28.000000 quantify-scheduler-0.9.0/docs/_build/html/_static/QUANTIFY-FAVICON_16.png
+-rw-rw-rw-   0        0        0      286 2022-08-04 16:31:59.000000 quantify-scheduler-0.9.0/docs/_build/html/_static/file.png
+-rw-rw-rw-   0        0        0       90 2022-08-04 16:31:59.000000 quantify-scheduler-0.9.0/docs/_build/html/_static/minus.png
+-rw-rw-rw-   0        0        0       90 2022-08-04 16:31:59.000000 quantify-scheduler-0.9.0/docs/_build/html/_static/plus.png
+drwxrwxrwx   0        0        0        0 2022-10-06 16:58:55.741867 quantify-scheduler-0.9.0/docs/_build/jupyter_execute/
+-rw-rw-rw-   0        0        0    18578 2022-10-05 11:16:13.000000 quantify-scheduler-0.9.0/docs/_build/jupyter_execute/03469962d7b549171a37aa0d94269bb6dcda55db16706b84f1736daeb14f191e.png
+-rw-rw-rw-   0        0        0    20797 2022-10-05 11:16:13.000000 quantify-scheduler-0.9.0/docs/_build/jupyter_execute/23bb4479dc5ade89b3bfdec9f0ed2fd1beec4881c243be131083ac64c3c12ca3.png
+-rw-rw-rw-   0        0        0    15718 2022-10-05 11:16:13.000000 quantify-scheduler-0.9.0/docs/_build/jupyter_execute/304514e0b7f2a94fe918a5566d29137a0fe07b5e6c3ad871564c3cba73156220.png
+-rw-rw-rw-   0        0        0    20387 2022-10-05 11:16:44.000000 quantify-scheduler-0.9.0/docs/_build/jupyter_execute/315b2d3264215202641421edfbef4755692b49ab97b190975c61c618fd9946ad.png
+-rw-rw-rw-   0        0        0    11707 2022-10-05 11:16:13.000000 quantify-scheduler-0.9.0/docs/_build/jupyter_execute/c2a231508f8856a2a1910e2f4304c19999a856684dade344e269c28e61bd1630.png
+-rw-rw-rw-   0        0        0    11320 2022-10-05 11:16:44.000000 quantify-scheduler-0.9.0/docs/_build/jupyter_execute/c50c688eb70c2c69386b99b5c2e0a5077b5c33923744ed273166c25a2451f34e.png
+-rw-rw-rw-   0        0        0    45436 2022-10-05 11:15:15.000000 quantify-scheduler-0.9.0/docs/_build/jupyter_execute/d09ad7bd99b334ca3e1b6472498bd275c53ad6e319df6707f10bbf100ec1adad.png
+-rw-rw-rw-   0        0        0       31 2022-09-22 07:22:36.000000 quantify-scheduler-0.9.0/docs/authors.md
+-rw-rw-rw-   0        0        0       52 2022-09-22 07:22:36.000000 quantify-scheduler-0.9.0/docs/bibliography.md
+-rw-rw-rw-   0        0        0       33 2022-09-22 07:22:36.000000 quantify-scheduler-0.9.0/docs/changelog.md
+-rw-rw-rw-   0        0        0    14277 2022-10-05 11:24:37.000000 quantify-scheduler-0.9.0/docs/conf.py
+-rw-rw-rw-   0        0        0       36 2022-09-22 07:22:36.000000 quantify-scheduler-0.9.0/docs/contributing.md
+drwxrwxrwx   0        0        0        0 2022-10-06 16:58:55.741867 quantify-scheduler-0.9.0/docs/examples/
+-rw-rw-rw-   0        0        0     2274 2022-09-22 07:22:36.000000 quantify-scheduler-0.9.0/docs/examples/structure.DataStructure.rst
+drwxrwxrwx   0        0        0        0 2022-10-06 16:58:55.746436 quantify-scheduler-0.9.0/docs/images/
+-rw-rw-rw-   0        0        0   566915 2022-02-07 13:26:28.000000 quantify-scheduler-0.9.0/docs/images/Chevron_experiment_comb.png
+-rw-rw-rw-   0        0        0     2254 2022-02-07 13:26:28.000000 quantify-scheduler-0.9.0/docs/images/QUANTIFY-FAVICON_16.png
+-rw-rw-rw-   0        0        0    11887 2022-02-07 13:26:28.000000 quantify-scheduler-0.9.0/docs/images/bell_circuit_QI.png
+-rw-rw-rw-   0        0        0      439 2022-09-22 07:22:36.000000 quantify-scheduler-0.9.0/docs/index.md
+-rw-rw-rw-   0        0        0     1705 2022-09-22 07:22:36.000000 quantify-scheduler-0.9.0/docs/installation.md
+-rwxrwxrwx   0        0        0     1269 2022-09-22 07:22:36.000000 quantify-scheduler-0.9.0/docs/make.bat
+-rw-rw-rw-   0        0        0     5314 2022-09-22 07:22:36.000000 quantify-scheduler-0.9.0/docs/quantify_compilers.md
+-rw-rw-rw-   0        0        0       30 2022-09-22 07:22:36.000000 quantify-scheduler-0.9.0/docs/readme.md
+drwxrwxrwx   0        0        0        0 2022-10-06 16:58:55.746436 quantify-scheduler-0.9.0/docs/tutorials/
+-rw-rw-rw-   0        0        0     9925 2022-10-05 11:24:37.000000 quantify-scheduler-0.9.0/docs/tutorials/Compiling to Hardware.md
+-rw-rw-rw-   0        0        0    16885 2022-09-22 07:22:36.000000 quantify-scheduler-0.9.0/docs/tutorials/Operations and Qubits.md
+-rw-rw-rw-   0        0        0     6301 2022-09-22 07:22:36.000000 quantify-scheduler-0.9.0/docs/tutorials/Schedules and Pulses.md
+drwxrwxrwx   0        0        0        0 2022-10-06 16:58:55.746436 quantify-scheduler-0.9.0/docs/tutorials/qblox/
+drwxrwxrwx   0        0        0        0 2022-10-06 16:58:55.758636 quantify-scheduler-0.9.0/docs/tutorials/qblox/.ipynb_checkpoints/
+-rw-rw-rw-   0        0        0    16438 2022-10-05 11:24:37.000000 quantify-scheduler-0.9.0/docs/tutorials/qblox/.ipynb_checkpoints/Pulsar-checkpoint.md
+-rw-rw-rw-   0        0        0    14970 2022-10-05 19:33:42.000000 quantify-scheduler-0.9.0/docs/tutorials/qblox/.ipynb_checkpoints/quantify-validate-qblox-checkpoint.md
+-rw-rw-rw-   0        0        0     3450 2022-09-22 07:22:36.000000 quantify-scheduler-0.9.0/docs/tutorials/qblox/Cluster.md
+-rw-rw-rw-   0        0        0     1183 2022-09-22 07:22:36.000000 quantify-scheduler-0.9.0/docs/tutorials/qblox/How to use.md
+-rw-rw-rw-   0        0        0    16438 2022-10-05 11:24:37.000000 quantify-scheduler-0.9.0/docs/tutorials/qblox/Pulsar.md
+-rw-rw-rw-   0        0        0     2229 2022-10-06 14:14:43.000000 quantify-scheduler-0.9.0/docs/tutorials/qblox/index.md
+-rw-rw-rw-   0        0        0     4370 2022-10-05 11:24:37.000000 quantify-scheduler-0.9.0/docs/tutorials/qblox/recent.rst
+drwxrwxrwx   0        0        0        0 2022-10-06 16:58:55.758636 quantify-scheduler-0.9.0/docs/tutorials/zhinst/
+-rw-rw-rw-   0        0        0    11919 2022-09-22 07:22:36.000000 quantify-scheduler-0.9.0/docs/tutorials/zhinst/T_verification_programs.md
+-rw-rw-rw-   0        0        0    14111 2022-09-22 07:22:36.000000 quantify-scheduler-0.9.0/docs/tutorials/zhinst/index.md
+-rw-rw-rw-   0        0        0    23463 2022-09-22 07:22:36.000000 quantify-scheduler-0.9.0/docs/user_guide.md
+drwxrwxrwx   0        0        0        0 2022-10-06 16:58:55.762386 quantify-scheduler-0.9.0/quantify_scheduler/
+-rw-rw-rw-   0        0        0      845 2022-10-06 16:36:21.000000 quantify-scheduler-0.9.0/quantify_scheduler/__init__.py
+drwxrwxrwx   0        0        0        0 2022-10-06 16:58:55.777960 quantify-scheduler-0.9.0/quantify_scheduler/backends/
+-rw-rw-rw-   0        0        0      207 2022-09-22 07:22:36.000000 quantify-scheduler-0.9.0/quantify_scheduler/backends/__init__.py
+-rw-rw-rw-   0        0        0    14065 2022-10-05 11:24:37.000000 quantify-scheduler-0.9.0/quantify_scheduler/backends/circuit_to_device.py
+-rw-rw-rw-   0        0        0     8406 2022-10-05 11:24:37.000000 quantify-scheduler-0.9.0/quantify_scheduler/backends/corrections.py
+-rw-rw-rw-   0        0        0    13273 2022-09-22 07:22:36.000000 quantify-scheduler-0.9.0/quantify_scheduler/backends/graph_compilation.py
+drwxrwxrwx   0        0        0        0 2022-10-06 16:58:55.793643 quantify-scheduler-0.9.0/quantify_scheduler/backends/qblox/
+-rw-rw-rw-   0        0        0        0 2022-02-07 13:26:28.000000 quantify-scheduler-0.9.0/quantify_scheduler/backends/qblox/__init__.py
+-rw-rw-rw-   0        0        0    60981 2022-10-05 11:24:37.000000 quantify-scheduler-0.9.0/quantify_scheduler/backends/qblox/compiler_abc.py
+-rw-rw-rw-   0        0        0     6654 2022-09-22 07:22:36.000000 quantify-scheduler-0.9.0/quantify_scheduler/backends/qblox/compiler_container.py
+-rw-rw-rw-   0        0        0     2816 2022-09-22 07:22:36.000000 quantify-scheduler-0.9.0/quantify_scheduler/backends/qblox/constants.py
+-rw-rw-rw-   0        0        0     2309 2022-09-22 07:22:36.000000 quantify-scheduler-0.9.0/quantify_scheduler/backends/qblox/driver_version_check.py
+-rw-rw-rw-   0        0        0    20313 2022-09-22 07:22:36.000000 quantify-scheduler-0.9.0/quantify_scheduler/backends/qblox/helpers.py
+-rw-rw-rw-   0        0        0    12515 2022-10-05 11:24:37.000000 quantify-scheduler-0.9.0/quantify_scheduler/backends/qblox/instrument_compilers.py
+drwxrwxrwx   0        0        0        0 2022-10-06 16:58:55.793643 quantify-scheduler-0.9.0/quantify_scheduler/backends/qblox/operation_handling/
+-rw-rw-rw-   0        0        0        0 2022-02-07 13:26:28.000000 quantify-scheduler-0.9.0/quantify_scheduler/backends/qblox/operation_handling/__init__.py
+-rw-rw-rw-   0        0        0    10398 2022-02-07 13:26:28.000000 quantify-scheduler-0.9.0/quantify_scheduler/backends/qblox/operation_handling/acquisitions.py
+-rw-rw-rw-   0        0        0     1451 2022-02-07 13:26:28.000000 quantify-scheduler-0.9.0/quantify_scheduler/backends/qblox/operation_handling/base.py
+-rw-rw-rw-   0        0        0     3205 2022-10-05 11:24:37.000000 quantify-scheduler-0.9.0/quantify_scheduler/backends/qblox/operation_handling/factory.py
+-rw-rw-rw-   0        0        0    17720 2022-09-22 07:22:36.000000 quantify-scheduler-0.9.0/quantify_scheduler/backends/qblox/operation_handling/pulses.py
+-rw-rw-rw-   0        0        0     2565 2022-08-22 11:44:07.000000 quantify-scheduler-0.9.0/quantify_scheduler/backends/qblox/operation_handling/virtual.py
+-rw-rw-rw-   0        0        0     1026 2022-02-17 10:07:58.000000 quantify-scheduler-0.9.0/quantify_scheduler/backends/qblox/q1asm_instructions.py
+-rw-rw-rw-   0        0        0    19430 2022-09-22 07:22:36.000000 quantify-scheduler-0.9.0/quantify_scheduler/backends/qblox/qasm_program.py
+-rw-rw-rw-   0        0        0     3580 2022-02-07 13:26:28.000000 quantify-scheduler-0.9.0/quantify_scheduler/backends/qblox/register_manager.py
+-rw-rw-rw-   0        0        0     3840 2022-10-05 11:24:37.000000 quantify-scheduler-0.9.0/quantify_scheduler/backends/qblox_backend.py
+drwxrwxrwx   0        0        0        0 2022-10-06 16:58:55.809826 quantify-scheduler-0.9.0/quantify_scheduler/backends/types/
+-rw-rw-rw-   0        0        0        0 2022-02-07 13:26:28.000000 quantify-scheduler-0.9.0/quantify_scheduler/backends/types/__init__.py
+-rw-rw-rw-   0        0        0     3175 2022-02-07 13:26:28.000000 quantify-scheduler-0.9.0/quantify_scheduler/backends/types/common.py
+-rw-rw-rw-   0        0        0    15465 2022-10-05 11:24:37.000000 quantify-scheduler-0.9.0/quantify_scheduler/backends/types/qblox.py
+-rw-rw-rw-   0        0        0     8766 2022-08-04 12:12:09.000000 quantify-scheduler-0.9.0/quantify_scheduler/backends/types/zhinst.py
+drwxrwxrwx   0        0        0        0 2022-10-06 16:58:55.809826 quantify-scheduler-0.9.0/quantify_scheduler/backends/zhinst/
+-rw-rw-rw-   0        0        0        0 2022-02-07 13:26:28.000000 quantify-scheduler-0.9.0/quantify_scheduler/backends/zhinst/__init__.py
+-rw-rw-rw-   0        0        0     9324 2022-02-07 13:26:28.000000 quantify-scheduler-0.9.0/quantify_scheduler/backends/zhinst/helpers.py
+-rw-rw-rw-   0        0        0     1634 2022-02-07 13:26:28.000000 quantify-scheduler-0.9.0/quantify_scheduler/backends/zhinst/resolvers.py
+-rw-rw-rw-   0        0        0    20692 2022-08-04 12:12:09.000000 quantify-scheduler-0.9.0/quantify_scheduler/backends/zhinst/seqc_il_generator.py
+-rw-rw-rw-   0        0        0    29146 2022-08-04 12:12:09.000000 quantify-scheduler-0.9.0/quantify_scheduler/backends/zhinst/settings.py
+-rw-rw-rw-   0        0        0    64700 2022-10-05 11:24:37.000000 quantify-scheduler-0.9.0/quantify_scheduler/backends/zhinst_backend.py
+-rw-rw-rw-   0        0        0    22115 2022-10-05 11:24:37.000000 quantify-scheduler-0.9.0/quantify_scheduler/compilation.py
+drwxrwxrwx   0        0        0        0 2022-10-06 16:58:55.825047 quantify-scheduler-0.9.0/quantify_scheduler/device_under_test/
+-rw-rw-rw-   0        0        0      386 2022-02-07 13:26:28.000000 quantify-scheduler-0.9.0/quantify_scheduler/device_under_test/__init__.py
+-rw-rw-rw-   0        0        0     4466 2022-09-22 07:22:36.000000 quantify-scheduler-0.9.0/quantify_scheduler/device_under_test/composite_square_edge.py
+-rw-rw-rw-   0        0        0     1018 2022-10-05 11:24:37.000000 quantify-scheduler-0.9.0/quantify_scheduler/device_under_test/device_element.py
+-rw-rw-rw-   0        0        0     1982 2022-10-05 11:24:37.000000 quantify-scheduler-0.9.0/quantify_scheduler/device_under_test/edge.py
+-rw-rw-rw-   0        0        0     4549 2022-10-05 11:24:37.000000 quantify-scheduler-0.9.0/quantify_scheduler/device_under_test/mock_setup.py
+-rw-rw-rw-   0        0        0    10653 2022-10-06 16:36:21.000000 quantify-scheduler-0.9.0/quantify_scheduler/device_under_test/quantum_device.py
+-rw-rw-rw-   0        0        0    25659 2022-10-06 16:36:21.000000 quantify-scheduler-0.9.0/quantify_scheduler/device_under_test/transmon_element.py
+-rw-rw-rw-   0        0        0     2144 2022-10-05 11:24:37.000000 quantify-scheduler-0.9.0/quantify_scheduler/enums.py
+-rw-rw-rw-   0        0        0      314 2022-02-07 13:26:28.000000 quantify-scheduler-0.9.0/quantify_scheduler/frontends.py
+-rw-rw-rw-   0        0        0    16789 2022-09-22 07:22:36.000000 quantify-scheduler-0.9.0/quantify_scheduler/gettables.py
+-rw-rw-rw-   0        0        0     5057 2022-09-22 07:48:46.000000 quantify-scheduler-0.9.0/quantify_scheduler/gettables_profiled.py
+drwxrwxrwx   0        0        0        0 2022-10-06 16:58:55.825047 quantify-scheduler-0.9.0/quantify_scheduler/helpers/
+-rw-rw-rw-   0        0        0       58 2022-02-07 13:26:28.000000 quantify-scheduler-0.9.0/quantify_scheduler/helpers/__init__.py
+-rw-rw-rw-   0        0        0     1637 2022-08-04 12:12:09.000000 quantify-scheduler-0.9.0/quantify_scheduler/helpers/collections.py
+-rw-rw-rw-   0        0        0      547 2022-08-04 12:12:09.000000 quantify-scheduler-0.9.0/quantify_scheduler/helpers/importers.py
+-rw-rw-rw-   0        0        0     1191 2022-02-07 13:26:28.000000 quantify-scheduler-0.9.0/quantify_scheduler/helpers/inspect.py
+-rw-rw-rw-   0        0        0     1674 2022-09-22 07:22:36.000000 quantify-scheduler-0.9.0/quantify_scheduler/helpers/mock_instruments.py
+-rw-rw-rw-   0        0        0    14459 2022-10-04 09:55:42.000000 quantify-scheduler-0.9.0/quantify_scheduler/helpers/schedule.py
+-rw-rw-rw-   0        0        0      872 2022-02-07 13:26:28.000000 quantify-scheduler-0.9.0/quantify_scheduler/helpers/time.py
+-rw-rw-rw-   0        0        0     2119 2022-02-22 13:21:56.000000 quantify-scheduler-0.9.0/quantify_scheduler/helpers/validators.py
+-rw-rw-rw-   0        0        0    15226 2022-08-04 12:12:09.000000 quantify-scheduler-0.9.0/quantify_scheduler/helpers/waveforms.py
+drwxrwxrwx   0        0        0        0 2022-10-06 16:58:55.825047 quantify-scheduler-0.9.0/quantify_scheduler/instrument_coordinator/
+-rw-rw-rw-   0        0        0      562 2022-09-22 07:22:36.000000 quantify-scheduler-0.9.0/quantify_scheduler/instrument_coordinator/__init__.py
+drwxrwxrwx   0        0        0        0 2022-10-06 16:58:55.841753 quantify-scheduler-0.9.0/quantify_scheduler/instrument_coordinator/components/
+-rw-rw-rw-   0        0        0      463 2022-07-05 17:45:39.000000 quantify-scheduler-0.9.0/quantify_scheduler/instrument_coordinator/components/__init__.py
+-rw-rw-rw-   0        0        0     4316 2022-02-07 13:26:28.000000 quantify-scheduler-0.9.0/quantify_scheduler/instrument_coordinator/components/base.py
+-rw-rw-rw-   0        0        0     5137 2022-02-07 13:26:28.000000 quantify-scheduler-0.9.0/quantify_scheduler/instrument_coordinator/components/generic.py
+-rw-rw-rw-   0        0        0    43185 2022-10-05 11:24:37.000000 quantify-scheduler-0.9.0/quantify_scheduler/instrument_coordinator/components/qblox.py
+-rw-rw-rw-   0        0        0    10816 2022-08-04 12:12:09.000000 quantify-scheduler-0.9.0/quantify_scheduler/instrument_coordinator/components/zhinst.py
+-rw-rw-rw-   0        0        0    14970 2022-08-04 12:12:09.000000 quantify-scheduler-0.9.0/quantify_scheduler/instrument_coordinator/instrument_coordinator.py
+-rw-rw-rw-   0        0        0     2808 2022-09-22 07:22:36.000000 quantify-scheduler-0.9.0/quantify_scheduler/instrument_coordinator/utility.py
+-rw-rw-rw-   0        0        0     8646 2022-10-05 11:24:37.000000 quantify-scheduler-0.9.0/quantify_scheduler/json_utils.py
+-rw-rw-rw-   0        0        0      768 2022-02-07 13:26:28.000000 quantify-scheduler-0.9.0/quantify_scheduler/math.py
+drwxrwxrwx   0        0        0        0 2022-10-06 16:58:55.841753 quantify-scheduler-0.9.0/quantify_scheduler/operations/
+-rw-rw-rw-   0        0        0      425 2022-02-07 13:26:28.000000 quantify-scheduler-0.9.0/quantify_scheduler/operations/__init__.py
+-rw-rw-rw-   0        0        0    20617 2022-10-05 11:24:37.000000 quantify-scheduler-0.9.0/quantify_scheduler/operations/acquisition_library.py
+-rw-rw-rw-   0        0        0    21928 2022-10-05 11:24:37.000000 quantify-scheduler-0.9.0/quantify_scheduler/operations/gate_library.py
+-rw-rw-rw-   0        0        0     3525 2022-09-22 07:22:36.000000 quantify-scheduler-0.9.0/quantify_scheduler/operations/measurement_factories.py
+-rw-rw-rw-   0        0        0    11270 2022-10-06 16:36:21.000000 quantify-scheduler-0.9.0/quantify_scheduler/operations/operation.py
+-rw-rw-rw-   0        0        0     3275 2022-10-03 15:08:44.000000 quantify-scheduler-0.9.0/quantify_scheduler/operations/pulse_factories.py
+-rw-rw-rw-   0        0        0    33457 2022-10-05 11:24:37.000000 quantify-scheduler-0.9.0/quantify_scheduler/operations/pulse_library.py
+-rw-rw-rw-   0        0        0     5634 2022-10-05 11:24:37.000000 quantify-scheduler-0.9.0/quantify_scheduler/resources.py
+drwxrwxrwx   0        0        0        0 2022-10-06 16:58:55.858325 quantify-scheduler-0.9.0/quantify_scheduler/schedules/
+-rw-rw-rw-   0        0        0      463 2022-02-07 13:26:28.000000 quantify-scheduler-0.9.0/quantify_scheduler/schedules/__init__.py
+-rw-rw-rw-   0        0        0    31170 2022-10-06 16:36:21.000000 quantify-scheduler-0.9.0/quantify_scheduler/schedules/schedule.py
+-rw-rw-rw-   0        0        0     5815 2022-02-07 13:26:28.000000 quantify-scheduler-0.9.0/quantify_scheduler/schedules/spectroscopy_schedules.py
+-rw-rw-rw-   0        0        0    15859 2022-09-22 07:22:36.000000 quantify-scheduler-0.9.0/quantify_scheduler/schedules/timedomain_schedules.py
+-rw-rw-rw-   0        0        0     6231 2022-09-22 07:22:36.000000 quantify-scheduler-0.9.0/quantify_scheduler/schedules/trace_schedules.py
+-rw-rw-rw-   0        0        0    10478 2022-08-04 12:12:09.000000 quantify-scheduler-0.9.0/quantify_scheduler/schedules/verification.py
+drwxrwxrwx   0        0        0        0 2022-10-06 16:58:55.858325 quantify-scheduler-0.9.0/quantify_scheduler/schemas/
+-rw-rw-rw-   0        0        0        0 2022-02-07 13:26:28.000000 quantify-scheduler-0.9.0/quantify_scheduler/schemas/__init__.py
+drwxrwxrwx   0        0        0        0 2022-10-06 16:58:55.875693 quantify-scheduler-0.9.0/quantify_scheduler/schemas/examples/
+-rw-rw-rw-   0        0        0        0 2022-02-07 13:26:28.000000 quantify-scheduler-0.9.0/quantify_scheduler/schemas/examples/__init__.py
+-rw-rw-rw-   0        0        0     4073 2022-10-05 11:24:37.000000 quantify-scheduler-0.9.0/quantify_scheduler/schemas/examples/circuit_to_device_example_cfgs.py
+-rw-rw-rw-   0        0        0     9056 2022-10-05 11:24:37.000000 quantify-scheduler-0.9.0/quantify_scheduler/schemas/examples/qblox_test_mapping.json
+-rw-rw-rw-   0        0        0     5478 2022-10-05 11:24:37.000000 quantify-scheduler-0.9.0/quantify_scheduler/schemas/examples/transmon_test_config.json
+-rw-rw-rw-   0        0        0      694 2022-02-07 13:26:28.000000 quantify-scheduler-0.9.0/quantify_scheduler/schemas/examples/utils.py
+-rw-rw-rw-   0        0        0     5045 2022-09-22 07:22:36.000000 quantify-scheduler-0.9.0/quantify_scheduler/schemas/examples/zhinst_test_mapping.json
+-rw-rw-rw-   0        0        0     6013 2022-09-22 07:22:36.000000 quantify-scheduler-0.9.0/quantify_scheduler/schemas/operation.json
+-rw-rw-rw-   0        0        0      468 2022-02-07 13:26:28.000000 quantify-scheduler-0.9.0/quantify_scheduler/schemas/resource.json
+-rw-rw-rw-   0        0        0     1324 2022-02-17 10:07:58.000000 quantify-scheduler-0.9.0/quantify_scheduler/schemas/schedulable.json
+-rw-rw-rw-   0        0        0     1144 2022-02-17 10:07:58.000000 quantify-scheduler-0.9.0/quantify_scheduler/schemas/schedule.json
+-rw-rw-rw-   0        0        0     1134 2022-10-05 11:24:37.000000 quantify-scheduler-0.9.0/quantify_scheduler/schemas/transmon_cfg.json
+drwxrwxrwx   0        0        0        0 2022-10-06 16:58:55.875693 quantify-scheduler-0.9.0/quantify_scheduler/structure/
+-rw-rw-rw-   0        0        0      299 2022-02-07 13:26:28.000000 quantify-scheduler-0.9.0/quantify_scheduler/structure/__init__.py
+-rw-rw-rw-   0        0        0     2135 2022-09-22 07:22:36.000000 quantify-scheduler-0.9.0/quantify_scheduler/structure/model.py
+-rw-rw-rw-   0        0        0        0 2022-08-04 12:12:09.000000 quantify-scheduler-0.9.0/quantify_scheduler/types.py
+drwxrwxrwx   0        0        0        0 2022-10-06 16:58:55.875693 quantify-scheduler-0.9.0/quantify_scheduler/visualization/
+-rw-rw-rw-   0        0        0        0 2022-02-07 13:26:28.000000 quantify-scheduler-0.9.0/quantify_scheduler/visualization/__init__.py
+-rw-rw-rw-   0        0        0    10092 2022-08-04 12:12:09.000000 quantify-scheduler-0.9.0/quantify_scheduler/visualization/circuit_diagram.py
+-rw-rw-rw-   0        0        0      506 2022-02-07 13:26:28.000000 quantify-scheduler-0.9.0/quantify_scheduler/visualization/constants.py
+-rw-rw-rw-   0        0        0    19596 2022-09-22 07:22:36.000000 quantify-scheduler-0.9.0/quantify_scheduler/visualization/pulse_diagram.py
+-rw-rw-rw-   0        0        0     9786 2022-02-07 13:26:28.000000 quantify-scheduler-0.9.0/quantify_scheduler/visualization/pulse_scheme.py
+-rw-rw-rw-   0        0        0    10943 2022-10-03 15:08:44.000000 quantify-scheduler-0.9.0/quantify_scheduler/waveforms.py
+drwxrwxrwx   0        0        0        0 2022-10-06 16:58:55.777960 quantify-scheduler-0.9.0/quantify_scheduler.egg-info/
+-rw-rw-rw-   0        0        0    38382 2022-10-06 16:58:54.000000 quantify-scheduler-0.9.0/quantify_scheduler.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    11971 2022-10-06 16:58:55.000000 quantify-scheduler-0.9.0/quantify_scheduler.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-10-06 16:58:54.000000 quantify-scheduler-0.9.0/quantify_scheduler.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2022-07-25 08:51:24.000000 quantify-scheduler-0.9.0/quantify_scheduler.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      289 2022-10-06 16:58:54.000000 quantify-scheduler-0.9.0/quantify_scheduler.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2022-10-06 16:58:54.000000 quantify-scheduler-0.9.0/quantify_scheduler.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      445 2022-10-06 16:58:55.999461 quantify-scheduler-0.9.0/setup.cfg
+-rw-rw-rw-   0        0        0     2129 2022-10-06 16:57:43.000000 quantify-scheduler-0.9.0/setup.py
+drwxrwxrwx   0        0        0        0 2022-10-06 16:58:55.891880 quantify-scheduler-0.9.0/tests/
+-rw-rw-rw-   0        0        0        0 2022-02-07 13:26:28.000000 quantify-scheduler-0.9.0/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2022-10-06 16:58:55.891880 quantify-scheduler-0.9.0/tests/baseline_images/
+-rw-rw-rw-   0        0        0    40694 2022-02-07 13:26:28.000000 quantify-scheduler-0.9.0/tests/baseline_images/test_hybrid_circuit_acquisitions_matplotlib.png
+-rw-rw-rw-   0        0        0    47781 2022-02-07 13:26:28.000000 quantify-scheduler-0.9.0/tests/baseline_images/test_hybrid_circuit_diagram_baseband_matplotlib.png
+-rw-rw-rw-   0        0        0    37124 2022-02-07 13:26:28.000000 quantify-scheduler-0.9.0/tests/baseline_images/test_hybrid_circuit_diagram_matplotlib.png
+-rw-rw-rw-   0        0        0    53383 2022-02-07 13:26:28.000000 quantify-scheduler-0.9.0/tests/baseline_images/test_hybrid_circuit_diagram_modulated_matplotlib.png
+-rw-rw-rw-   0        0        0    59476 2022-02-07 13:26:28.000000 quantify-scheduler-0.9.0/tests/baseline_images/test_hybrid_circuit_diagram_unknown_port_matplotlib.png
+-rw-rw-rw-   0        0        0    73409 2022-02-07 13:26:28.000000 quantify-scheduler-0.9.0/tests/baseline_images/test_plot_pulses_n_q.png
+-rw-rw-rw-   0        0        0    22113 2022-02-07 13:26:28.000000 quantify-scheduler-0.9.0/tests/baseline_images/test_plot_pulses_single_q.png
+drwxrwxrwx   0        0        0        0 2022-10-06 16:58:55.891880 quantify-scheduler-0.9.0/tests/baseline_qblox_assembly/
+-rw-rw-rw-   0        0        0    20683 2022-10-05 11:24:37.000000 quantify-scheduler-0.9.0/tests/baseline_qblox_assembly/AllXY_qrm0_seq0_instr.json
+-rw-rw-rw-   0        0        0     9953 2022-10-05 11:24:37.000000 quantify-scheduler-0.9.0/tests/baseline_qblox_assembly/Readout calibration q0, [0, 1]_qrm0_seq0_instr.json
+-rw-rw-rw-   0        0        0     1818 2022-10-05 11:24:37.000000 quantify-scheduler-0.9.0/tests/baseline_qblox_assembly/sched-looped-acq_qrm0_seq0_instr.json
+-rw-rw-rw-   0        0        0      355 2022-06-13 10:01:39.000000 quantify-scheduler-0.9.0/tests/conftest.py
+drwxrwxrwx   0        0        0        0 2022-10-06 16:58:55.908406 quantify-scheduler-0.9.0/tests/fixtures/
+-rw-rw-rw-   0        0        0        0 2022-02-07 13:26:28.000000 quantify-scheduler-0.9.0/tests/fixtures/__init__.py
+-rw-rw-rw-   0        0        0     6017 2022-10-05 11:24:37.000000 quantify-scheduler-0.9.0/tests/fixtures/mock_setup.py
+-rw-rw-rw-   0        0        0      456 2022-06-13 09:25:06.000000 quantify-scheduler-0.9.0/tests/fixtures/qcodes_utilities.py
+-rw-rw-rw-   0        0        0     5922 2022-09-22 07:22:36.000000 quantify-scheduler-0.9.0/tests/fixtures/schedule.py
+drwxrwxrwx   0        0        0        0 2022-10-06 16:58:55.925763 quantify-scheduler-0.9.0/tests/scheduler/
+-rw-rw-rw-   0        0        0        0 2022-02-07 13:26:28.000000 quantify-scheduler-0.9.0/tests/scheduler/__init__.py
+drwxrwxrwx   0        0        0        0 2022-10-06 16:58:55.925763 quantify-scheduler-0.9.0/tests/scheduler/backends/
+-rw-rw-rw-   0        0        0        0 2022-02-07 13:26:28.000000 quantify-scheduler-0.9.0/tests/scheduler/backends/__init__.py
+drwxrwxrwx   0        0        0        0 2022-10-06 16:58:55.942063 quantify-scheduler-0.9.0/tests/scheduler/backends/graph_backends/
+-rw-rw-rw-   0        0        0      908 2022-09-22 07:22:36.000000 quantify-scheduler-0.9.0/tests/scheduler/backends/graph_backends/__init__.py
+-rw-rw-rw-   0        0        0     5081 2022-09-22 07:22:36.000000 quantify-scheduler-0.9.0/tests/scheduler/backends/graph_backends/standard_schedules.py
+-rw-rw-rw-   0        0        0      185 2022-09-22 07:22:36.000000 quantify-scheduler-0.9.0/tests/scheduler/backends/graph_backends/test_compilation_flow.py
+-rw-rw-rw-   0        0        0     1534 2022-09-22 07:22:36.000000 quantify-scheduler-0.9.0/tests/scheduler/backends/graph_backends/test_device_compile.py
+-rw-rw-rw-   0        0        0     2773 2022-09-22 07:22:36.000000 quantify-scheduler-0.9.0/tests/scheduler/backends/graph_backends/test_qblox_backend.py
+-rw-rw-rw-   0        0        0     4471 2022-09-22 07:22:36.000000 quantify-scheduler-0.9.0/tests/scheduler/backends/graph_backends/test_zhinst_backend.py
+drwxrwxrwx   0        0        0        0 2022-10-06 16:58:55.942063 quantify-scheduler-0.9.0/tests/scheduler/backends/qblox/
+drwxrwxrwx   0        0        0        0 2022-10-06 16:58:55.952057 quantify-scheduler-0.9.0/tests/scheduler/backends/qblox/operation_handling/
+-rw-rw-rw-   0        0        0    17749 2022-10-05 11:24:37.000000 quantify-scheduler-0.9.0/tests/scheduler/backends/qblox/operation_handling/test_acquisitions.py
+-rw-rw-rw-   0        0        0     5737 2022-04-14 13:58:55.000000 quantify-scheduler-0.9.0/tests/scheduler/backends/qblox/operation_handling/test_factory.py
+-rw-rw-rw-   0        0        0    20416 2022-04-14 13:58:55.000000 quantify-scheduler-0.9.0/tests/scheduler/backends/qblox/operation_handling/test_pulses.py
+-rw-rw-rw-   0        0        0     4143 2022-09-22 07:22:36.000000 quantify-scheduler-0.9.0/tests/scheduler/backends/qblox/operation_handling/test_virtual.py
+-rw-rw-rw-   0        0        0      324 2022-09-19 08:51:33.000000 quantify-scheduler-0.9.0/tests/scheduler/backends/qblox/operation_handling/tmp.hex
+-rw-rw-rw-   0        0        0     1437 2022-09-19 08:51:33.000000 quantify-scheduler-0.9.0/tests/scheduler/backends/qblox/operation_handling/tmp.q1asm
+-rw-rw-rw-   0        0        0     1720 2022-08-04 12:12:09.000000 quantify-scheduler-0.9.0/tests/scheduler/backends/qblox/test_driver_version_check.py
+-rw-rw-rw-   0        0        0     1278 2022-09-22 07:22:36.000000 quantify-scheduler-0.9.0/tests/scheduler/backends/qblox/test_helpers_qblox.py
+-rw-rw-rw-   0        0        0     1992 2022-02-07 13:26:28.000000 quantify-scheduler-0.9.0/tests/scheduler/backends/qblox/test_register_manager.py
+-rw-rw-rw-   0        0        0    12651 2022-09-22 07:22:36.000000 quantify-scheduler-0.9.0/tests/scheduler/backends/test_circuit_to_device.py
+-rw-rw-rw-   0        0        0     2193 2022-09-22 07:22:36.000000 quantify-scheduler-0.9.0/tests/scheduler/backends/test_graph_compilation.py
+-rw-rw-rw-   0        0        0    71857 2022-10-05 11:24:37.000000 quantify-scheduler-0.9.0/tests/scheduler/backends/test_qblox_backend.py
+-rw-rw-rw-   0        0        0    39270 2022-10-05 11:24:37.000000 quantify-scheduler-0.9.0/tests/scheduler/backends/test_zhinst_backend.py
+-rw-rw-rw-   0        0        0     3240 2022-08-09 12:58:11.000000 quantify-scheduler-0.9.0/tests/scheduler/backends/tmp.hex
+-rw-rw-rw-   0        0        0    13587 2022-08-09 12:58:11.000000 quantify-scheduler-0.9.0/tests/scheduler/backends/tmp.q1asm
+drwxrwxrwx   0        0        0        0 2022-10-06 16:58:55.958609 quantify-scheduler-0.9.0/tests/scheduler/backends/zhinst/
+-rw-rw-rw-   0        0        0    12451 2022-08-02 14:15:26.000000 quantify-scheduler-0.9.0/tests/scheduler/backends/zhinst/test_helpers.py
+-rw-rw-rw-   0        0        0     2116 2022-02-07 13:26:28.000000 quantify-scheduler-0.9.0/tests/scheduler/backends/zhinst/test_resolvers.py
+-rw-rw-rw-   0        0        0     6210 2022-08-04 12:12:09.000000 quantify-scheduler-0.9.0/tests/scheduler/backends/zhinst/test_seqc_il_generator.py
+-rw-rw-rw-   0        0        0    16093 2022-02-17 10:07:58.000000 quantify-scheduler-0.9.0/tests/scheduler/backends/zhinst/test_settings.py
+drwxrwxrwx   0        0        0        0 2022-10-06 16:58:55.958609 quantify-scheduler-0.9.0/tests/scheduler/device_under_test/
+-rw-rw-rw-   0        0        0     2288 2022-10-05 11:24:37.000000 quantify-scheduler-0.9.0/tests/scheduler/device_under_test/test_composite_square_edge.py
+-rw-rw-rw-   0        0        0     2941 2022-10-05 11:24:37.000000 quantify-scheduler-0.9.0/tests/scheduler/device_under_test/test_quantum_device.py
+-rw-rw-rw-   0        0        0     2475 2022-10-05 11:24:37.000000 quantify-scheduler-0.9.0/tests/scheduler/device_under_test/test_transmon_element.py
+drwxrwxrwx   0        0        0        0 2022-10-06 16:58:55.967645 quantify-scheduler-0.9.0/tests/scheduler/helpers/
+-rw-rw-rw-   0        0        0        0 2022-02-07 13:26:28.000000 quantify-scheduler-0.9.0/tests/scheduler/helpers/__init__.py
+-rw-rw-rw-   0        0        0      488 2022-02-07 13:26:28.000000 quantify-scheduler-0.9.0/tests/scheduler/helpers/test_inspect.py
+-rw-rw-rw-   0        0        0    16238 2022-10-05 11:24:37.000000 quantify-scheduler-0.9.0/tests/scheduler/helpers/test_schedule.py
+-rw-rw-rw-   0        0        0    11434 2022-09-22 07:22:36.000000 quantify-scheduler-0.9.0/tests/scheduler/helpers/test_waveforms.py
+drwxrwxrwx   0        0        0        0 2022-10-06 16:58:55.967728 quantify-scheduler-0.9.0/tests/scheduler/instrument_coordinator/
+-rw-rw-rw-   0        0        0        0 2022-02-07 13:26:28.000000 quantify-scheduler-0.9.0/tests/scheduler/instrument_coordinator/__init__.py
+drwxrwxrwx   0        0        0        0 2022-10-06 16:58:55.975108 quantify-scheduler-0.9.0/tests/scheduler/instrument_coordinator/components/
+-rw-rw-rw-   0        0        0        0 2022-02-07 13:26:28.000000 quantify-scheduler-0.9.0/tests/scheduler/instrument_coordinator/components/__init__.py
+-rw-rw-rw-   0        0        0     3140 2022-09-22 07:22:36.000000 quantify-scheduler-0.9.0/tests/scheduler/instrument_coordinator/components/test_generic.py
+-rw-rw-rw-   0        0        0    33298 2022-10-05 11:24:37.000000 quantify-scheduler-0.9.0/tests/scheduler/instrument_coordinator/components/test_qblox.py
+-rw-rw-rw-   0        0        0     9072 2022-08-04 12:12:09.000000 quantify-scheduler-0.9.0/tests/scheduler/instrument_coordinator/components/test_zhinst.py
+-rw-rw-rw-   0        0        0      288 2022-09-07 19:09:56.000000 quantify-scheduler-0.9.0/tests/scheduler/instrument_coordinator/components/tmp.hex
+-rw-rw-rw-   0        0        0     1287 2022-09-07 19:09:56.000000 quantify-scheduler-0.9.0/tests/scheduler/instrument_coordinator/components/tmp.q1asm
+-rw-rw-rw-   0        0        0    12467 2022-10-05 11:24:37.000000 quantify-scheduler-0.9.0/tests/scheduler/instrument_coordinator/test_instrument_coordinator.py
+-rw-rw-rw-   0        0        0     3990 2022-09-22 07:22:36.000000 quantify-scheduler-0.9.0/tests/scheduler/instrument_coordinator/test_utility.py
+drwxrwxrwx   0        0        0        0 2022-10-06 16:58:55.991859 quantify-scheduler-0.9.0/tests/scheduler/schedules/
+-rw-rw-rw-   0        0        0        0 2022-02-07 13:26:28.000000 quantify-scheduler-0.9.0/tests/scheduler/schedules/__init__.py
+-rw-rw-rw-   0        0        0      989 2022-09-22 07:22:36.000000 quantify-scheduler-0.9.0/tests/scheduler/schedules/compiles_all_backends.py
+-rw-rw-rw-   0        0        0     2019 2022-02-07 13:26:28.000000 quantify-scheduler-0.9.0/tests/scheduler/schedules/test_schedule_plotting_matplotlib.py
+-rw-rw-rw-   0        0        0     3057 2022-10-05 11:24:37.000000 quantify-scheduler-0.9.0/tests/scheduler/schedules/test_schedule_sampling.py
+-rw-rw-rw-   0        0        0     3845 2022-09-22 07:22:36.000000 quantify-scheduler-0.9.0/tests/scheduler/schedules/test_spectroscopy_schedules.py
+-rw-rw-rw-   0        0        0    16370 2022-09-22 07:22:36.000000 quantify-scheduler-0.9.0/tests/scheduler/schedules/test_timedomain_schedules.py
+-rw-rw-rw-   0        0        0     4480 2022-08-02 12:33:43.000000 quantify-scheduler-0.9.0/tests/scheduler/schedules/test_trace_schedules.py
+-rw-rw-rw-   0        0        0     6395 2022-10-05 11:24:37.000000 quantify-scheduler-0.9.0/tests/scheduler/schedules/test_verification.py
+drwxrwxrwx   0        0        0        0 2022-10-06 16:58:55.991859 quantify-scheduler-0.9.0/tests/scheduler/schemas/
+-rw-rw-rw-   0        0        0        0 2022-02-17 10:07:58.000000 quantify-scheduler-0.9.0/tests/scheduler/schemas/__init__.py
+drwxrwxrwx   0        0        0        0 2022-10-06 16:58:55.991859 quantify-scheduler-0.9.0/tests/scheduler/schemas/examples/
+-rw-rw-rw-   0        0        0        0 2022-02-17 10:07:58.000000 quantify-scheduler-0.9.0/tests/scheduler/schemas/examples/__init__.py
+-rw-rw-rw-   0        0        0      470 2022-02-07 13:26:28.000000 quantify-scheduler-0.9.0/tests/scheduler/schemas/examples/test_utils.py
+-rw-rw-rw-   0        0        0     6310 2022-10-05 11:24:37.000000 quantify-scheduler-0.9.0/tests/scheduler/test_acquisition_library.py
+-rw-rw-rw-   0        0        0    10324 2022-10-05 11:24:37.000000 quantify-scheduler-0.9.0/tests/scheduler/test_compilation.py
+-rw-rw-rw-   0        0        0     5758 2022-10-05 11:24:37.000000 quantify-scheduler-0.9.0/tests/scheduler/test_corrections.py
+-rw-rw-rw-   0        0        0     7839 2022-10-05 11:24:37.000000 quantify-scheduler-0.9.0/tests/scheduler/test_gate_library.py
+-rw-rw-rw-   0        0        0    16315 2022-10-05 11:24:37.000000 quantify-scheduler-0.9.0/tests/scheduler/test_gettables.py
+-rw-rw-rw-   0        0        0     2378 2022-09-22 07:22:36.000000 quantify-scheduler-0.9.0/tests/scheduler/test_json_utils.py
+-rw-rw-rw-   0        0        0      498 2022-02-07 13:26:28.000000 quantify-scheduler-0.9.0/tests/scheduler/test_math.py
+-rw-rw-rw-   0        0        0    10779 2022-10-05 11:24:37.000000 quantify-scheduler-0.9.0/tests/scheduler/test_pulse_library.py
+-rw-rw-rw-   0        0        0      742 2022-02-07 13:26:28.000000 quantify-scheduler-0.9.0/tests/scheduler/test_resources.py
+-rw-rw-rw-   0        0        0      716 2022-02-07 13:26:28.000000 quantify-scheduler-0.9.0/tests/scheduler/test_structure.py
+-rw-rw-rw-   0        0        0    13532 2022-10-05 11:24:37.000000 quantify-scheduler-0.9.0/tests/scheduler/test_types.py
+-rw-rw-rw-   0        0        0     5078 2022-10-03 15:08:44.000000 quantify-scheduler-0.9.0/tests/scheduler/test_waveforms.py
+-rw-rw-rw-   0        0        0      396 2022-07-21 09:11:41.000000 quantify-scheduler-0.9.0/tests/scheduler/tmp.hex
+-rw-rw-rw-   0        0        0     1737 2022-07-21 09:11:41.000000 quantify-scheduler-0.9.0/tests/scheduler/tmp.q1asm
+drwxrwxrwx   0        0        0        0 2022-10-06 16:58:55.991859 quantify-scheduler-0.9.0/tests/scheduler/visualization/
+-rw-rw-rw-   0        0        0        0 2022-02-07 13:26:28.000000 quantify-scheduler-0.9.0/tests/scheduler/visualization/__init__.py
+-rw-rw-rw-   0        0        0     3325 2022-02-07 13:26:28.000000 quantify-scheduler-0.9.0/tests/scheduler/visualization/test_circuit_diagram.py
+-rw-rw-rw-   0        0        0     1163 2022-10-05 11:24:37.000000 quantify-scheduler-0.9.0/tests/scheduler/visualization/test_pulse_diagram.py
+-rw-rw-rw-   0        0        0     1936 2022-02-07 13:26:28.000000 quantify-scheduler-0.9.0/tests/scheduler/visualization/test_pulse_scheme.py
+-rw-rw-rw-   0        0        0     2151 2022-02-07 13:26:28.000000 quantify-scheduler-0.9.0/tests/test_headers_and_copyright.py
+-rw-rw-rw-   0        0        0      396 2022-10-04 09:59:07.000000 quantify-scheduler-0.9.0/tests/tmp.hex
+-rw-rw-rw-   0        0        0     1737 2022-10-04 09:59:07.000000 quantify-scheduler-0.9.0/tests/tmp.q1asm
```

### Comparing `quantify-scheduler-0.8.0/CONTRIBUTING.rst` & `quantify-scheduler-0.9.0/CONTRIBUTING.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,44 +1,41 @@
-00000000: 2e2e 2068 6967 686c 6967 6874 3a3a 2073  .. highlight:: s
-00000010: 6865 6c6c 0a0a 3d3d 3d3d 3d3d 3d3d 3d3d  hell..==========
-00000020: 3d3d 0a43 6f6e 7472 6962 7574 696e 670a  ==.Contributing.
-00000030: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 0a0a 436f  ============..Co
-00000040: 6e74 7269 6275 7469 6f6e 7320 6172 6520  ntributions are 
-00000050: 7765 6c63 6f6d 6520 616e 6420 6772 6561  welcome and grea
-00000060: 746c 7920 6170 7072 6563 6961 7465 6421  tly appreciated!
-00000070: 2045 7665 7279 206c 6974 746c 6520 6269   Every little bi
-00000080: 7420 6865 6c70 732c 2061 6e64 2063 7265  t helps, and cre
-00000090: 6469 7420 7769 6c6c 2061 6c77 6179 7320  dit will always 
-000000a0: 6265 2067 6976 656e 2e0a 0a59 6f75 2063  be given...You c
-000000b0: 616e 2063 6f6e 7472 6962 7574 6520 696e  an contribute in
-000000c0: 206d 616e 7920 7761 7973 210a 0a54 6869   many ways!..Thi
-000000d0: 7320 7265 706f 7369 746f 7279 2066 6f6c  s repository fol
-000000e0: 6c6f 7773 2074 6865 2073 616d 6520 636f  lows the same co
-000000f0: 6e74 7269 6275 7469 6f6e 2067 7569 6465  ntribution guide
-00000100: 6c69 6e65 7320 6173 2074 6865 2060 5175  lines as the `Qu
-00000110: 616e 7469 6679 2043 6f72 6520 3c68 7474  antify Core <htt
-00000120: 7073 3a2f 2f67 6974 6c61 622e 636f 6d2f  ps://gitlab.com/
-00000130: 7175 616e 7469 6679 2d6f 732f 7175 616e  quantify-os/quan
-00000140: 7469 6679 2d63 6f72 653e 605f 2072 6570  tify-core>`_ rep
-00000150: 6f73 6974 6f72 792e 2050 6c65 6173 6520  ository. Please 
-00000160: 7365 6520 6074 6865 7365 2063 6f6e 7472  see `these contr
-00000170: 6962 7574 696f 6e20 6775 6964 656c 696e  ibution guidelin
-00000180: 6573 203c 6874 7470 733a 2f2f 7175 616e  es <https://quan
-00000190: 7469 6679 2d71 7561 6e74 6966 792d 636f  tify-quantify-co
-000001a0: 7265 2e72 6561 6474 6865 646f 6373 2d68  re.readthedocs-h
-000001b0: 6f73 7465 642e 636f 6d2f 656e 2f6c 6174  osted.com/en/lat
-000001c0: 6573 742f 636f 6e74 7269 6275 7469 6e67  est/contributing
-000001d0: 2e68 746d 6c3e 605f 2069 6620 796f 7520  .html>`_ if you 
-000001e0: 7769 7368 2074 6f20 636f 6e74 7269 6275  wish to contribu
-000001f0: 7465 2e0a 0a55 7365 6675 6c20 6c69 6e6b  te...Useful link
-00000200: 730a 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a  s.-------------.
-00000210: 0a2d 2060 4769 744c 6162 2054 7261 636b  .- `GitLab Track
-00000220: 6572 203c 6874 7470 733a 2f2f 6769 746c  er <https://gitl
-00000230: 6162 2e63 6f6d 2f71 7561 6e74 6966 792d  ab.com/quantify-
-00000240: 6f73 2f71 7561 6e74 6966 792d 7363 6865  os/quantify-sche
-00000250: 6475 6c65 722f 2d2f 6973 7375 6573 3e60  duler/-/issues>`
-00000260: 5f0a 2d20 6047 6974 4c61 6220 6973 7375  _.- `GitLab issu
-00000270: 6520 626f 6172 6420 3c68 7474 7073 3a2f  e board <https:/
-00000280: 2f67 6974 6c61 622e 636f 6d2f 7175 616e  /gitlab.com/quan
-00000290: 7469 6679 2d6f 732f 7175 616e 7469 6679  tify-os/quantify
-000002a0: 2d73 6368 6564 756c 6572 2f2d 2f62 6f61  -scheduler/-/boa
-000002b0: 7264 733e 605f 0a                        rds>`_.
+00000000: 6060 607b 6869 6768 6c69 6768 747d 2073  ```{highlight} s
+00000010: 6865 6c6c 0a60 6060 0a0a 2320 436f 6e74  hell.```..# Cont
+00000020: 7269 6275 7469 6e67 0a0a 436f 6e74 7269  ributing..Contri
+00000030: 6275 7469 6f6e 7320 6172 6520 7765 6c63  butions are welc
+00000040: 6f6d 6520 616e 6420 6772 6561 746c 7920  ome and greatly 
+00000050: 6170 7072 6563 6961 7465 6421 2045 7665  appreciated! Eve
+00000060: 7279 206c 6974 746c 6520 6269 7420 6865  ry little bit he
+00000070: 6c70 732c 2061 6e64 2063 7265 6469 7420  lps, and credit 
+00000080: 7769 6c6c 2061 6c77 6179 7320 6265 2067  will always be g
+00000090: 6976 656e 2e0a 0a59 6f75 2063 616e 2063  iven...You can c
+000000a0: 6f6e 7472 6962 7574 6520 696e 206d 616e  ontribute in man
+000000b0: 7920 7761 7973 210a 0a54 6869 7320 7265  y ways!..This re
+000000c0: 706f 7369 746f 7279 2066 6f6c 6c6f 7773  pository follows
+000000d0: 2074 6865 2073 616d 6520 636f 6e74 7269   the same contri
+000000e0: 6275 7469 6f6e 2067 7569 6465 6c69 6e65  bution guideline
+000000f0: 7320 6173 2074 6865 205b 5175 616e 7469  s as the [Quanti
+00000100: 6679 2043 6f72 655d 2868 7474 7073 3a2f  fy Core](https:/
+00000110: 2f67 6974 6c61 622e 636f 6d2f 7175 616e  /gitlab.com/quan
+00000120: 7469 6679 2d6f 732f 7175 616e 7469 6679  tify-os/quantify
+00000130: 2d63 6f72 6529 2072 6570 6f73 6974 6f72  -core) repositor
+00000140: 792e 2050 6c65 6173 6520 7365 6520 5b74  y. Please see [t
+00000150: 6865 7365 2063 6f6e 7472 6962 7574 696f  hese contributio
+00000160: 6e20 6775 6964 656c 696e 6573 5d28 6874  n guidelines](ht
+00000170: 7470 733a 2f2f 7175 616e 7469 6679 2d71  tps://quantify-q
+00000180: 7561 6e74 6966 792d 636f 7265 2e72 6561  uantify-core.rea
+00000190: 6474 6865 646f 6373 2d68 6f73 7465 642e  dthedocs-hosted.
+000001a0: 636f 6d2f 656e 2f6c 6174 6573 742f 636f  com/en/latest/co
+000001b0: 6e74 7269 6275 7469 6e67 2e68 746d 6c29  ntributing.html)
+000001c0: 2069 6620 796f 7520 7769 7368 2074 6f20   if you wish to 
+000001d0: 636f 6e74 7269 6275 7465 2e0a 0a23 2320  contribute...## 
+000001e0: 5573 6566 756c 206c 696e 6b73 0a0a 2d20  Useful links..- 
+000001f0: 5b47 6974 4c61 6220 5472 6163 6b65 725d  [GitLab Tracker]
+00000200: 2868 7474 7073 3a2f 2f67 6974 6c61 622e  (https://gitlab.
+00000210: 636f 6d2f 7175 616e 7469 6679 2d6f 732f  com/quantify-os/
+00000220: 7175 616e 7469 6679 2d73 6368 6564 756c  quantify-schedul
+00000230: 6572 2f2d 2f69 7373 7565 7329 0a2d 205b  er/-/issues).- [
+00000240: 4769 744c 6162 2069 7373 7565 2062 6f61  GitLab issue boa
+00000250: 7264 5d28 6874 7470 733a 2f2f 6769 746c  rd](https://gitl
+00000260: 6162 2e63 6f6d 2f71 7561 6e74 6966 792d  ab.com/quantify-
+00000270: 6f73 2f71 7561 6e74 6966 792d 7363 6865  os/quantify-sche
+00000280: 6475 6c65 722f 2d2f 626f 6172 6473 290a  duler/-/boards).
```

### Comparing `quantify-scheduler-0.8.0/LICENSE` & `quantify-scheduler-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `quantify-scheduler-0.8.0/PKG-INFO` & `quantify-scheduler-0.9.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,553 +1,521 @@
-Metadata-Version: 2.1
-Name: quantify-scheduler
-Version: 0.8.0
-Summary: Quantify-scheduler is a python package for writing quantum programs featuring a hybrid gate-pulse control model with explicit timing control.
-Home-page: https://gitlab.com/quantify-os/quantify-scheduler
-Author: The Quantify consortium consisting of Qblox and Orange Quantum Systems
-Author-email: maintainers@quantify-os.org
-License: BSD-3 license
-Keywords: quantify-scheduler
-Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.8
-License-File: LICENSE
-License-File: AUTHORS.rst
-
-==================
-quantify-scheduler
-==================
-
-.. image:: https://img.shields.io/badge/slack-chat-green.svg
-    :target: https://join.slack.com/t/quantify-hq/shared_invite/zt-vao45946-f_NaRc4mvYQDQE_oYB8xSw
-    :alt: Slack
-
-.. image:: https://gitlab.com/quantify-os/quantify-scheduler/badges/main/pipeline.svg
-    :target: https://gitlab.com/quantify-os/quantify-scheduler/pipelines/
-    :alt: Pipelines
-
-.. image:: https://img.shields.io/pypi/v/quantify-scheduler.svg
-    :target: https://pypi.org/pypi/quantify-scheduler
-    :alt: PyPi
-
-.. image:: https://app.codacy.com/project/badge/Grade/0c9cf5b6eb5f47ffbd2bb484d555c7e3
-    :target: https://www.codacy.com/gl/quantify-os/quantify-scheduler/dashboard?utm_source=gitlab.com&amp;utm_medium=referral&amp;utm_content=quantify-os/quantify-scheduler&amp;utm_campaign=Badge_Grade
-    :alt: Code Quality
-
-.. image:: https://app.codacy.com/project/badge/Coverage/0c9cf5b6eb5f47ffbd2bb484d555c7e3
-    :target: https://www.codacy.com/gl/quantify-os/quantify-scheduler/dashboard?utm_source=gitlab.com&amp;utm_medium=referral&amp;utm_content=quantify-os/quantify-scheduler&amp;utm_campaign=Badge_Coverage
-    :alt: Coverage
-
-.. image:: https://readthedocs.com/projects/quantify-quantify-scheduler/badge/?version=latest&token=ed6fdbf228e1369eacbeafdbad464f6de927e5dfb3a8e482ad0adcbea76fe74c
-    :target: https://quantify-quantify-scheduler.readthedocs-hosted.com
-    :alt: Documentation Status
-
-.. image:: https://img.shields.io/badge/License-BSD%203--Clause-blue.svg
-    :target: https://gitlab.com/quantify-os/quantify-scheduler/-/raw/main/LICENSE
-    :alt: License
-
-.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
-    :target: https://github.com/psf/black
-    :alt: Code style
-
-.. image:: https://img.shields.io/badge/Supported%20By-UNITARY%20FUND-brightgreen.svg?style=flat
-    :target: http://unitary.fund
-    :alt: Unitary Fund
-
-.. figure:: /images/QUANTIFY_LANDSCAPE.svg
-    :align: center
-    :alt: Quantify logo
-
-Quantify is a python based data acquisition platform focused on Quantum Computing and solid-state physics experiments.
-It is build on top of `QCoDeS <https://qcodes.github.io/Qcodes/>`_ and is a spiritual successor of `PycQED <https://github.com/DiCarloLab-Delft/PycQED_py3>`_.
-Quantify currently consists of `quantify-core <https://pypi.org/project/quantify-core/>`_ and `quantify-scheduler <https://pypi.org/project/quantify-scheduler/>`_.
-
-Take a look at the `latest documentation for quantify-scheduler <https://quantify-quantify-scheduler.readthedocs-hosted.com/>`_ or use the switch in the bottom of left panel to read the documentation for older releases.
-
-Quantify-scheduler is a python module for writing quantum programs featuring a hybrid gate-pulse control model with explicit timing control.
-The control model allows quantum gate- and pulse-level descriptions to be combined in a clearly defined and hardware-agnostic way.
-Quantify-scheduler is designed to allow experimentalists to easily define complex experiments, and produces synchronized pulse schedules to be distributed to control hardware.
-
-.. caution::
-
-    This is a pre-release **alpha version**, major changes are expected. Use for testing & development purposes only.
-
-About
------
-
-Quantify-scheduler is maintained by The Quantify consortium consisting of Qblox and Orange Quantum Systems.
-
-.. |_| unicode:: 0xA0
-   :trim:
-
-
-.. figure:: https://cdn.sanity.io/images/ostxzp7d/production/f9ab429fc72aea1b31c4b2c7fab5e378b67d75c3-132x31.svg
-    :width: 200px
-    :target: https://qblox.com
-    :align: left
-
-.. figure:: https://orangeqs.com/OQS_logo_with_text.svg
-    :width: 200px
-    :target: https://orangeqs.com
-    :align: left
-
-|_|
-
-
-|_|
-
-The software is free to use under the conditions specified in the `license <https://gitlab.com/quantify-os/quantify-scheduler/-/raw/main/LICENSE>`_.
-
-.. nothing-to-avoid-a-sphinx-warning:
-
-
-=======
-Credits
-=======
-
-Contributors
-------------
-
-* Adam Lawrence <adam@orangeqs.com>
-* Adriaan Rol <adriaan@orangeqs.com>
-* Callum Attryde <cattryde@qblox.com>
-* Christian Dickel <christiandickel8@gmail.com>
-* Damaz de Jong <ddejong@qblox.com>
-* Damien Crielaard <dcrielaard@qblox.com>
-* Diogo Valada <dvalada@qblox.com>
-* Edgar Reehuis <ereehuis@qblox.com>
-* Gabor Oszkar Denes <gdenes@qblox.com>
-* Gijs Vermarien <gijs@orangeqs.com>
-* Jordy Gloudemans <jgloudemans@qblox.com>
-* Jules van Oven <jules@qblox.com>
-* Kelvin Loh <kelvin@orangeqs.com>
-* Luis Miguens Fernandez <lmiguens@qblox.com>
-* Michiel Dubbelman <michiel@orangeqs.com>
-* Pieter Eendebak <pieter.eendebak@tno.nl>
-* Robert Sokolewicz <rsokolewicz@qblox.com>
-* Thomas Reynders <thomas@orangeqs.com>
-* Viacheslav Ostroukh <viacheslav@orangeqs.com>
-* Victor Negirneac <vnegirneac@qblox.com>
-
-
-=========
-Changelog
-=========
-
-0.8.0 Support for two qubit operations and basic CZ-gate implementation (2022-08-10)
-------------------------------------------------------------------------------------
-
-Breaking changes
-~~~~~~~~~~~~~~~~
-* Operations - Pin `qcodes` package to <0.34.0 due to breaking `Edge` naming (#300, !409)
-* Qblox backend - Sequencers are now dynamically allocated. The hardware config file schema was changed. (!328)
-    - For each instrument, the config now contains a `portclock_configs` entry, a list with a dictionary of settings per port-clock combination
-    - See https://quantify-quantify-scheduler.readthedocs-hosted.com/en/0.8.0/tutorials/qblox/recent.html
-* Qblox backend - Strictly requires v0.7.x of the `qblox-instruments` package (!449)
-* Zhinst backend - Strictly requires v21.8.20515 of the `zhinst` package (!387)
-
-Merged branches and closed issues
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-* Compilation - Added `acq_protocol` optional parameter to the `Measure` gate. (!386)
-* Compilation - Call `determine_absolute_timing` in `qcompile` when no `device_cfg` supplied. (!436)
-* Compilation - Decrease test usage of deprecated transmon_test_config.json / add_pulse_information_transmon (!450)
-* DRAG Pulse - Removed an extra G_amp factor from the Q component (derivative pulse). (#298, !406)
-* Docs - Fix API reference pages on read-the-docs (#303, !413)
-* Docs - Pin sphinx to 5.0.2 due to crash in napoleon (!437)
-* Docs - Unpin sphinx >=5.1.1 (!445)
-* Docs - Fix jsonschemas not rendered on read-the-docs (!448)
-* Docs - Clarify port and clock concepts (!431)
-* Docs - New scheduler tutorials: Schedules and Pulses; Compiling to Hardware; Operations and Qubits (!336, !439)
-* Gettables - Added `generate_diagnostic_report` method to save the internal state of `ScheduleGettable` to a zip-file. (!408)
-* Helpers - Moved `MockLocalOscillator` definition from tests to `helpers.mock_instruments.MockLocalOscillator` (!392, !336).
-* JSON utilities - Add JSON serialization/deserialization methods based on `__getstate__`/`__setstate__` (!444)
-* Operations - Added a `symmetric` key in the `gate_info` to flag symmetric operations. (!389)
-* Operations - Introduce basic CZ-gate via `CompositeSquareEdge` (utilizing `quantify_scheduler.operations.pulse_factories.composite_square_pulse`) (!411)
-    - Replaces the incomplete `SuddenNetZeroEdge` basic CZ-gate implementation
-* Operations - Rxy theta rotations now fall into the domain of [-180 to 180) degrees. (!433)
-* QuantumDevice - Added implementation for `edges` in the quantum device config in order to support two qubit operations. (!389)
-    - The `Edge` has been added as an abstract base class for edges to be added to a device.
-* Qblox backend - Only add clocks to the schedule that are actually being used, avoids trying to assign frequencies for unused clocks (#278, !371)
-* Qblox backend - Fix for supplying negative NCO phase (!393)
-* Qblox backend - Fix compilation of ShiftClockPhase (!404, broken by merge of !328)
-* Qblox backend - Fix for outputting signals on even output paths of qblox hardware in real_output_x mode (!397)
-* Qblox backend - Make Qblox backend compatible with generic downconverter values in hardware_config (!418)
-* Qblox backend - Fix for 90 degree phase shift on even output paths as a result of the !397 hotfix. (!412)
-* Qblox backend - Fix cluster compatibility when converting old hwconfig to new specs (!419)
-* Qblox backend - Latency corrections must now be defined in top layer of hw config (!400)
-* Qblox backend - Fix combination of cluster and latency corrections when converting hw_configs to new specs  (!417)
-* Qblox backend - Fix handling of composite pulses (#299, !411)
-* Qblox backend - Implementation of distortion correction (#285, !388)
-* Qblox backend - Fix incompatibility of distortion_correction parameters as numpy arrays (!426)
-* Qblox backend - Remove all references to the inactive `line_gain_db` param (!435)
-* Qblox ICCs - Fix for setting `scope_acq_sequencer_select` for QRM and QRM-RF (!432, !441)
-* Qblox ICCs - Fix `ClusterComponent.prepare` mutating the schedule (!443)
-* Schedules - Revert rename of `trace_schedule` done in !432 and rename new schedule using gates to `trace_schedule_circuit_layer` (!442)
-* Schedules - Make `AcquisitionMetadata` a serializable class (!446)
-
-
-0.7.0 Support for qblox-instruments v0.6.0, new BasicTransmonElement, change for triggers in Zhinst backend (2022-04-11)
-------------------------------------------------------------------------------------------------------------------------
-
-Breaking changes
-~~~~~~~~~~~~~~~~
-* Qblox ICCs - Updated Qblox components for using the new unified-style qblox driver (see https://gitlab.com/quantify-os/quantify-scheduler/-/wikis/Qblox-ICCs:-Interface-changes-in-using-qblox-instruments-v0.6.0) (!377).
-* Qblox backend - Strictly requires v0.6.0 of the qblox-instruments package (!377).
-* Zhinst backend - Hardware config for the devices. Replaced keyword "triggers" to "trigger", and the value type from `List[int]` to `int`. E.g. old style, `"triggers": [2]`, new style, `"trigger": 2` (#264, !372).
-
-Merged branches and closed issues
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-* QuantumDevice - The `DeviceElement` has been added as an abstract base class for elements to be added to a device (#148, !374).
-* QuantumDevice - The `BasicTransmonElement` has been added that generates a device config in a more structured manner (#246, !374).
-* QuantumDevice - Fixed a bug in the `BasicTransmonElement` where operations had clock-frequencies (`float`) specified instead of clocks (`str`) (!379).
-* QuantumDevice - The `TransmonElement` will be deprecated after version 0.8 (!374).
-
-
-0.6.0 Full support for multiplexed readout, transmon element update, fixes to backends (2022-03-10)
----------------------------------------------------------------------------------------------------
-
-Breaking changes
-~~~~~~~~~~~~~~~~
-* Compilation - Deprecated `add_pulse_information_transmon` in favor of `compilation.backends.circuit_to_device.compile_circuit_to_device` (#64, #67, !339).
-* Compilation - attempting compilation with missing values in the `DeviceCompilationConfig` configuration will now raise validation errors. Be sure to set initial values when generating a config using the `QuantumDevice` object (!339)
-* Compilation - Device compile making use of `.compile_circuit_to_device` no longer modifies the input schedule (#249, !339).
-* Compilation - When specifying multiple timing constraints for a schedulable, the constraint specifying the latest time determines the absolute time of the shedulable (!309)
-* Gettables - `ScheduleGettableSingleChannel` renamed to `ScheduleGettable` as it now supports multiple acquisition channels (!299).
-* Hardware config - Removed the need for a `ic_` prefix from the hardware config (!312).
-* Instrument Coordinator - IC now adds a `GenericInstrumentCoordinatorComponent` to itself on instantiation by default (!350)
-* Instrument Coordinator - IC stop function has an `allow_failure` parameter which allows IC components attached to it to fail to stop with warning instead of raising errors. Allows for situations when some components cannot have a stop instruction sent before the prepare stage. (!359)
-* Operations - The internal behavior of how acquisition channels and acquisition indices are configured in the `Measure` operation has changed slightly. See #262 for details. (!339).
-* Operations - Added "operation_type" key to the schema. (!345)
-* Structure - `Schedule.timing_constraints` has been renamed to `Schedule.schedulables`. It now points to a dictionary of schedulables rather than a list of dicts. (!309)
-* Structure - Pydantic-based model is now used for the data structures. (!341)
-* Visualization - Deprecated `plot_circuit_diagram_mpl` and `plot_pulse_diagram_mpl` in `ScheduleBase` in favour of `plot_circuit_diagram` and `plot_pulse_diagram` (!313)
-* Qblox backend - Strictly requires v0.5.4 of the qblox-instruments package (!314)
-* Zhinst backend - Due to !312, the csv files used to upload the waveforms to the UHFQA no longer use the `ic_` prefix in their filenames. (!334)
-* Zhinst backend - Fixes bug when doing SSRO experiments. No more duplicated shots. Adds support for BinMode.APPEND during compilation. (#276, !358)
-* Zhinst backend - Removed `latency` and `line_trigger_delay` keys in the channels of the devices for the Zhinst hardware config. (!363)
-* Zhinst backend - Added `latency_corrections` main entry in the Zhinst hardware config for latency corrections on a port-clock combination basis. (!363)
-
-Merged branches and closed issues
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-* Compilation - Added a new compilation backend `compilation.backends.circuit_to_device.compile_circuit_to_device` for the quantum-circuit to quantum-device layer (#64, #67, !339).
-* Compilation - Fixed `add_pulse_information_transmon` when using "Trace" acquisition mode (!300)
-* Compilation - Fixed the deprecation warnings from pandas `DataFrame.append`. (!347)
-* Docs - Pinning qcodes package to <0.32.0 due to Read the Docs API reference failure (!361)
-* Gettables - `ScheduleGettable` now first stops all instruments in IC during initialization (!324)
-* Schedules - Adds a multiplexing verification schedule. (!329)
-* Operations - Sudden Net Zero from Negirneac 2021 added to the `pulse_library` (!339)
-* Operations - Docstrings for the X90, X, Y90, Y, and Rxy gate unitary have been aligned with literature. (#261, !305)
-* Operations - Adds an optional "data" argument to staircase pulse. (!335)
-* Pulse library - Added `ShiftClockPhase` operation that can be used to shift the phase of a clock during execution of a `Schedule` (!346)
-* Pulse library - Added a numerically defined pulse. (!157)
-* QuantumDevice - Unknown values are initialized as `float('nan')` (#274, !356)
-* TransmonElement - Corrected the motzoi parameter range validator. (!351)
-* Visualization - Adds visualisation of acquisitions to plotly pulse diagrams (!304)
-* Visualization - Add `plot_pulse_diagram` and `plot_circuit_diagram` to schedule for easier method names, and enable plotly visualization directly from `ScheduleBase` (!313)
-* Utilities - Migrates the utilities from quantify-core. (!357)
-* Generic ICC - Adds support for nested parameters. (!330)
-* Qblox ICCs - Stop now disables sync on all sequencers to prevent hanging during next run, where it gets re-enabled if needed (!324)
-* Qblox ICCs - `_QRMAcquisitionManager._get_scope_data` now has correct return type (#232, !300)
-* Qblox ICCs - Fixed bug where QRM scope mode sequencer does not get set correctly (!342)
-* Qblox ICCs - Fixed reference source cluster issue when it is not being set correctly. (!323)
-* Qblox backend - NCO phase now gets reset every averaging loop (!337)
-* Qblox backend - Enables RF output switch at the start of a program. (!344)
-* Qblox backend - Added logic for changing the NCO phase during execution of a `Schedule` (!346)
-* Qblox backend - Added ability to correct for latency by delaying program execution on a per sequencer basis (!325)
-* Qblox backend - Compilation with local oscillators changed to work with generic instrument coordinator components (!306)
-* Qblox backend - Refactored operation handling and greatly increased test coverage (!301).
-* Qblox backend - Made max duration of wait instructions (!319).
-* Qblox backend - Fixed an issue with the downconverter frequency correction. (!318)
-* Qblox backend - Temporary fix for a floating point rounding error when calculating the length of pulses. (#284, !365)
-* Zhinst backend - Fixed the ZI resolver return typehint. (!307)
-* Zhinst backend - Fixed an issue when compiling seqc programs for multiple sequencers end up overwriting the first sequencer. (!340, #260)
-
-
-0.5.2 Fixes to backends, and other incremental fixes  (2021-12-08)
-------------------------------------------------------------------
-
-Breaking changes
-~~~~~~~~~~~~~~~~
-* Dependency on `jsonschema` has been replaced with `fastjsonschema`. (!284, !293)
-* Zhinst hardware config json schema has changed. See the example schema. (!283)
-* In `hardware_compile` function, the `hardware_map` is changed to `hardware_cfg` parameter. (!279)
-* Remove enum tools dependency (!270)
-
-Merged branches and closed issues
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-
-* Compilation - The `determine_absolute_scheduling` function now sorts the list of labels in the timing constraints, and then a binary search (via `np.searchsorted`) is applied. (!272, !274)
-* Compilation - Make `device_cfg` an optional argument of qcompile(!281)
-* Compilation - renamed the hardware_mapping argument of qcompile into hardware_cfg (#165, !279)
-* Compilation - Introduced the hardware_compile function to perform the hardware compilation returning a CompiledSchedule (#224, !279)
-* Docs - Updating user guide to mention correctly the QuantumDevice and ScheduleGettable(s) available. (!209)
-* Infrastructure - Adds rich package in the requirements since tutorials use it. (!276)
-* Operations - The `locate` function now uses the `functools.lru_cache` to cache the result (only for python >= 3.8). For python 3.7, behaviour remains the same.  (!273, !275)
-* Operations - Resolved a minor issue where identical Rxy rotations (for angles >360) would be treated as separate operations in a schedule (!263)
-* Visualization - Adds a function `plot_acquisition_operations` which together with the new `AcquisitionOperation` class will help highlight acquisition pulses in the pulse diagrams. (!271, !277)
-* Zhinst backend - Large parts of the Zhinst backend have been rewritten. This should resolve a range of issues. (!263)
-    - Calculation of the timelines for different operations now makes using of a timing table, improving code readability and debugability.
-    - Timing issues related to triggering should be resolved (#218)
-    - The backend can now always use the same hardware configuration file (#214)
-    - Acquisition is now done using the StartQA instruction (#213)
-    - error handling in the Zhinst backend has been improved catching several exceptions at compile time of the schedule instead of manifesting in unexpected results during runtime.
-    - Local oscillators through the ZI backend uses the GenericInstrumentCoordinatorComponent. Configures other parameters other than frequency. (!283, #204)
-* Qblox backend - only check major and minor version when checking compatibility with the qblox_instruments package (!290)
-    - Added support for the Qblox Downconverter (!297)
-    - Added workaround for staircase_amplitude. (!292)
-    - Fix looped acquisition integration time, fix acquire index offset by one (!291)
-    - Qblox instruments version == 0.5.3 (!289)
-    - Fix sequencer_sync_en not being reset in the qblox instrument coordinator component. (!285)
-    - Fix rounding of time to samples in qblox backend (!282)
-    - Fix pulse stitching at zero amplitude. (!280)
-    - Allow instruction generated staircase with modulation (!278)
-* Utilities - Improve JSON validation speed (!284)
-* Utilities - Improve operation deserialization speed (!273)
-* Bugfix - For calculating the pulse area, the mathematical area is used instead of area of sampled pulse. (!242, !286)
-* Bugfix - Fix for plot window operations (!294)
-
-
-0.5.1 Incremental fixes, refactoring, and addition of convenience methods and classes (2021-11-11)
---------------------------------------------------------------------------------------------------
-
-Breaking changes
-~~~~~~~~~~~~~~~~
-* InstrumentCoordinator - `last_schedule` is now a property (!252).
-* Structure - We have refactored the Operation and Schedule classes out of the types module and moved the different operation libraries (acquisition_library, gate_library, and pulse_library) (#217, !256).
-    * `quantify_scheduler.types.Operation` -> `quantify_scheduler.operations.operation.Operation`, the import `quantify_scheduler.Operation` still works.
-    * `quantify_scheduler.types.Schedule` -> `quantify_scheduler.schedules.schedule.Schedule`, the import `quantify_scheduler.Schedule` still works.
-    * `quantify_scheduler.types.CompiledSchedule` -> `quantify_scheduler.schedules.schedule.CompiledSchedule`
-    * `quantify_scheduler.types.ScheduleBase` -> `quantify_scheduler.schedules.schedule.ScheduleBase`
-    * `quantify_scheduler.types.AcquisitionMetadata` -> `quantify_scheduler.schedules.schedule.AcquisitionMetadata`
-    * `quantify_scheduler.acquisition_library` -> `quantify_scheduler.operations.acquisition_library`
-    * `quantify_scheduler.gate_library` -> `quantify_scheduler.operations.gate_library`
-    * `quantify_scheduler.pulse_library` -> `quantify_scheduler.operations.pulse_library`
-
-Merged branches and closed issues
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-* Control - Add option to set output port in heterodyne_spec_sched (!262)
-* Control - Expand SingleChannelScheduleGettable to support trace acquisitions (!248)
-* Control - Update create_dc_compensation_pulse behaviour and docstring. (!244)
-* Control - Refactor ScheduleGettableSingleChannel (!240, !249)
-* Control - Reduce the default init_duration of spectroscopy schedules (!237)
-* Generic ICC - Added a GenericInstrumentCoordinatorComponent. (!267)
-* ICCs - InstrumentCoordinatorComponentBase now has a `force_set_parameter` as a ManualParameter to enable the user to switch the lazy_set behaviour when setting parameters of the instruments connected to the InstrumentCoordinatorComponent. (!267)
-* Qblox ICCs - Adds a lazy_set behaviour by default when setting parameters with the same value to an instrument connected to the Qblox ICC. (!230)
-* Visualization - made matplotlib schedule visualization methods accessible as methods `plot_circuit_diagram_mpl` and `plot_pulse_diagram_mpl` of the `Schedule` class (!253)
-* Visualization - resolved a bug where a schedule was modified when drawing a circuit diagram (#197, !250)
-* Visualization - Add support for window operation to transmon backend (!245)
-* Infrastructure - Fix and enhance pre-commit + add to CI (!257, !265)
-* Infrastructure - Added prospector config file for CI. (!261)
-* Bugfix - Removed redundant `determine_absolute_timing` step in `qcompile`. (!259)
-* Bugfix - Ramp pulse sampling utilizing `np.linspace` behaviour changed. (!258)
-* Docs - Adds the new Quantify logo similar to quantify_core. (!266)
-* Docs - Enhance documentation of public API for reimported modules [imports aliases] (!254)
-* Docs - Fixes the funcparserlib error in rtd. (!251)
-* Docs - Updated Qblox backend docs to include the new features. (!247)
-
-
-0.5.0 Expanded feature sets hardware compilation backends (2021-10-25)
-----------------------------------------------------------------------
-
-Breaking changes
-~~~~~~~~~~~~~~~~
-* The `schedules.timedomain_schedules.allxy_sched` function no longer accepts the string "All" as an argument to the `element_select_idx` keyword.
-* The `QuantumDevice.cfg_nr_averages` parameter was renamed to `QuantumDevice.cfg_sched_repetitions`
-* The call signature of `gettables.ScheduleVectorAcqGettable` has been renamed to `gettables.ScheduleGettableSingleChannel`, and the call signature has been updated according to #36 to no longer accept several keyword arguments.
-* Qblox Backend - The NCO phase is now reset at the start of a program (!213).
-* Qblox Backend - Compilation now requires qblox_instruments version 0.5.0, 0.5.1 or 0.5.2 (!214, !221).
-
-Merged branches and closed issues
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-* Compilation - Added the ability to specify the BinMode at the quantum-circuit layer (#183, !180).
-* Compilation - qcompile no longer modifies schedules (#102, !178).
-* Control - Added a first version of the QuantumDevice object (#148, !180).
-* Control - A single-qubit ScheduleGettable has been added (#36, !180).
-* Docs - Added bibliography with sphinxcontrib-bibtex extension (!171).
-* Docs - Fixed missing files in API reference (!176).
-* InstrumentCoordinator - CompiledSchedule class added to specify interfaces of InstrumentCoordinator and compilation functions (#174, !177).
-* InstrumentCoordinator - CompiledSchedule.last_schedule method added to provide access to last executed schedule (#167, !177).
-* Qblox Backend - Added support for qblox_instruments version 0.4.0 (new acquisition path) (!143).
-* Qblox Backend - Added support for real time mixer corrections rather than pre-distorting the uploaded waveforms (!192).
-* Qblox Backend - Waveforms are now compared using the normalized data array rather than the parameterized description (!182).
-* Qblox Backend - Support for append bin mode (#184, !180).
-* Qblox Backend - Support for using real value pulses on arbitrary outputs added (!142).
-* Qblox Backend - Compilation now supports 6 sequencers for both the QCM as well as the QRM (!142).
-* Qblox Backend - Support for a cluster, along with its QCM, QRM, QCM-RF and QRM-RF modules (!164)
-* Qblox Backend - Registers are now dynamically allocated during compilation (!195)
-* Zhinst backend - No exception is raised when an LO that is in the config is not part of a schedule. (#203, !223)
-* Zhinst backend - Instrument coordinator components for ZI will only be configured when the settings used to configure it have changed (#196, !227)
-* Zhinst backend - Solved a bug that caused single-sideband demodulation to not be configured correctly when using the UHFQA (!227)
-* Zhinst backend - Warnings raised during compilation of seqc programs will no longer raise an exception but will use logging.warning (!227)
-* Zhinst backend - resolved a bug where the instrument coordinator cannot write waveforms to the UHFQA if it has never been used before (!227)
-* Zhinst backend - resolved a bug where multiple identical measurements in a schedule would result in multiple integration weights being uploaded to the UFHQA (#207, !234)
-* Zhinst backend - resolved a bug where the UHFQA would not be triggered properly when executing a schedule with multiple samples (batched mode) (#205, !234)
-* Qblox ICCs - Compensated integration time for Qblox QRM IC component (!199).
-* Qblox ICCs - Added error handling for error flags given by `get_sequencer_state` (!215)
-* QuantumDevice - Added docstrings to the TransmonElement parameters (!216, !218)
-* Qblox ICCs - QCoDeS parameters are now only set if they differ from the value in the cache (!230)
-* Visualization - Allow user defined axis for plotting circuit diagram (!206)
-* Visualization - Adds schedule plotting using matplotlib and a WindowOperation to help visualize pulse diagrams (!225, !232)
-* Other - Added method `sample_schedule` to sample a `Schedule` (!212)
-* Other - The `RampPulse` has an extra (optional) parameter `offset` (!211)
-* Other - Updated existing schedules to make use of the acquisition index (#180, !180).
-* Other - Added a function to extract acquisition metadata from a schedule (#179, !180).
-* Other - The soft square waveform can now be evaluated with only one datapoint without raising an exception (!235)
-* Other - Added a function that generates a square pulse that compensates DC components of a sequence of pulses (!173)
-
-0.4.0 InstrumentCoordinator and improvements to backends (2021-08-06)
----------------------------------------------------------------------
-
-Breaking changes
-~~~~~~~~~~~~~~~~
-* Change of namespace from quantify.scheduler.* to quantify_scheduler.*
-
-Merged branches and closed issues
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-* Changes the namespace from quantify.scheduler to quantify_scheduler (!124)
-* InstrumentCoordinator - Add is_running property and wait_done method. Closes #133 (!140)
-* InstrumentCoordinator - Add instrument coordinator reference parameter to transmon element (!152)
-* InstrumentCoordinator - Prefix serialized settings for ZI ControlStack components. (!149)
-* InstrumentCoordinator - Refactored ControlStack name to InstrumentCoordinator (!151)
-* InstrumentCoordinator - Make use of InstrumentRefParameters (!144)
-* InstrumentCoordinator - Add controlstack class (!70)
-* InstrumentCoordinator - Add Zurich Instruments InstrumentCoordinatorComponent. (!99)
-* InstrumentCoordinator - Add Qblox InstrumentCoordinatorComponent. (!112)
-* InstrumentCoordinator - Avoid garbage collection for instrument coordinator components (!162)
-* Qblox backend - Removed limit in Qblox backend that keeps the QCM sequencer count at 2 (!135)
-* Qblox backend - Restructured compilation using external local oscillators. (!116)
-* Qblox backend - Added Chirp and Staircase pulses; and efficient implementation for QD spin qubit experiments (!106)
-* Qblox backend - Only run `start_sequencer` on pulsar instruments which have been armed (!156)
-* Zhinst backend - Assert current with new sequence program to skip compilation (!131)
-* Zhinst backend - Deserialize zhinst settings from JSON to ZISettingsBuilder (!130)
-* Zhinst backend - Add waveform mixer skewness corrections (!103)
-* Zhinst backend - Add backend option to enable Calibration mode (#103, !123)
-* Zhinst backend - Replace weights string array with a numerical array in JSON format (!148)
-* Zhinst backend - Add grouping of instrument settings (!133)
-* Zhinst backend - Add qcompile tests for the zurich instruments backend (!118)
-* Zhinst backend - Add repetitions parameter (!138)
-* Zhinst backend - Fixes the bug where the seqc in the datadir is not copied to the webserver location. (!165)
-* Fix for circuit diagram plotting failure after pulse scheduling (#157, !163)
-* Fixed typo in the gate_info of the Y gate in the gate_library (!155)
-* Add artificial detuning in Ramsey Schedule and bug fixes (!120)
-* Use individual loggers per python file (!134)
-* Recolour draw circuit diagram mpl (!96)
-* Fix issues with timedomain schedules (!145)
-* Renamed input parameters of quantify_scheduler.schedules.* functions. (!136)
-* Added acquisitions to circuit diagram (!93)
-* Add string representations to acquisition protocols of the acquisitions library (!114)
-* Transmon element and config generation (!75)
-* Rename operation_hash to operation_repr (!122)
-* Add types.Schedule from_json conversion (!119)
-* Add missing return types (!121)
-* Add serialization to Operations (!110)
-
-
-
-0.3.0 Multiple backends support (2021-05-20)
-------------------------------------------------
-* Added support for both Qblox and Zurich Instrument backends.
-* Added convenience pylintrc configuration file.
-* Added examples for timedomain and spectroscopy schedules.
-
-
-Breaking changes
-~~~~~~~~~~~~~~~~
-* Major refactor of the Qblox backend. (For example, it's now `quantify_core.backends.qblox_backend` instead of the previous `quantify_core.backends.pulsar_backend`)
-* Qblox backend requires strictly v0.3.2 of the qblox-instruments package.
-
-
-Merged branches and closed issues
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-
-* Add mixer skewness corrections helper function. (!102)
-* Added Qblox backend support. (!81)
-* Compile backend with ZISettingsBuilder. (!87)
-* Add vscode IDE config files. (!100)
-* Add ZISettingsBuilder class. (!86)
-* Added representation to gates in gate library and defined equality operation. (!101)
-* Fix/operation duration. Fixes #107. (!89)
-* Feat/long pulses fix validators name. (!90)
-* Implemented long square pulses unrolling (for waveform-memory-limited devices). (!83)
-* Changed Qblox-Instruments version to 0.3.2. (!88)
-* Feature: Improve overall zhinst backend timing. (!77)
-* Plotly cleanup. (!69)
-* Pulsar backend version bump. (!82)
-* Added zhinst backend support. (!49)
-* Added example timedomain programs. (!71)
-* Added example spectroscopy programs. (!64)
-* Added pylintrc configuration file. (!55)
-* Added repetitions property to Schedule. (!56)
-* Added Acquisition Protocols. (!51)
-* Hotfix for filename sanitization pulsar backend. (!61)
-* Pulsar backend function sanitization. (!60)
-* Potential fix time-out pulsar. (!58)
-* Updated Pulsar backend version to v0.2.3.. (!57)
-* Fixed datadir related bugs. (!54)
-* Added Station implementation. (!52)
-* Pulsar backend v0.2.2 check. (!48)
-* Fix for issue with acq delay. (!45)
-* Fix for issue #52. (!44)
-* Add artificial detuning to Ramsey schedule (!120)
-* Added support for the Qblox Pulsar QCM-RF/QRM-RF devices (!158)
-
-
-
-0.2.0 Hybrid pulse- gate-level control model (2021-01-14)
----------------------------------------------------------
-
-* Major refactor of the scheduler resource code enabling hybrid pulse- gate-level control.
-* Moved quantify_scheduler.types.Resource class to a separate quantify_scheduler.resources module.
-* Adds a BasebandClockResource class within the newly created quantify_scheduler.resources module.
-* Moved QRM and QCM related classes to the quantify_scheduler.backends.pulsar_backend module.
-* In quantify_scheduler.compilation, rename of function '_determine_absolute_timing' to 'determine_absolute_timing'. Argument changed from clock_unit to time_unit.
-* In quantify_scheduler.compilation, rename of function '_add_pulse_information_transmon' to 'add_pulse_information_transmon'.
-* Added ramp waveform in quantify_scheduler.waveforms.
-* Added schemas for operation and transmon_cfg.
-* Added a basic hybrid visualisation for pulses using new addressing scheme.
-* Operations check whether an operation is a valid gate or pulse.
-* Refactor of visualization module. Moved quantify_scheduler.backends.visualization to quantify_scheduler.visualization module. Expect code breaking reorganization and changes to function names.
-* Pulsar backend version now checks for QCM and QRM drivers version 0.1.2.
-
-Merged branches and closed issues
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-
-* fix(pulse_scheme): Add tickformatstops for x-axis using SI-unit 'seconds'. Closes #39. (!39)
-* Resolve "y-axis label is broken in plotly visualization after resources-refactor". Closes #45. (!38)
-* Resources refactor (!28, !29, !30)
-* Hybrid visualisation for pulses and circuit gate operations. Closes #22 and #6. (!27)
-* Support Pulsar parameterisation from scheduler. Support feature for #29. (!2)
-* Operation properties to check if an operation is a valid gate or pulse. Closes #28 (!25)
-* Visualisation refactor. Closes #26. (!22)
-* Windows job (!20)
-* Changed Pulsar backend version check from 0.1.1 to 0.1.2. (!21)
-
-
-
-0.1.0 (2020-10-21)
-------------------
-* Refactored scheduler functionality from quantify-core into quantify-scheduler
-* Support for modifying Pulsar params via the sequencer #54 (!2)
-* Simplification of compilation through `qcompile` (!1)
-* Qubit resources can be parameters of gates #11 (!4)
-* Circuit diagram visualization of operations without no pulse info raises exception #5 (!5)
-* Pulsar backend verifies driver and firmware versions of hardware #14 (!6)
-* Sequencer renamed to scheduler #15 (!7)
-* Documentation update to reflect refactor #8 (!8)
-* Refactor circuit diagram to be more usable !10 (relates to #6)
-* Unify API docstrings to adhere to NumpyDocstring format !11
-* Changes to addressing of where a pulse is played !9 (#10)
-* Renamed doc -docs folder for consistency #18 (!12)
-* Moved test folder outside of project #19 (!14)
-* Add copyright notices and cleanup documenation #21 (!13)
-* Add installation tip for plotly dependency in combination with jupyter #24 (!15)
-
-.. note::
-
-    * # denotes a closed issue.
-    * ! denotes a merge request.
+Metadata-Version: 2.1
+Name: quantify-scheduler
+Version: 0.9.0
+Summary: Quantify-scheduler is a python package for writing quantum programs featuring a hybrid gate-pulse control model with explicit timing control.
+Home-page: https://gitlab.com/quantify-os/quantify-scheduler
+Author: The Quantify consortium consisting of Qblox and Orange Quantum Systems
+Author-email: maintainers@quantify-os.org
+License: BSD-3 license
+Keywords: quantify-scheduler
+Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+License-File: AUTHORS.md
+
+# quantify-scheduler
+
+[![Slack](https://img.shields.io/badge/slack-chat-green.svg)](https://join.slack.com/t/quantify-hq/shared_invite/zt-vao45946-f_NaRc4mvYQDQE_oYB8xSw)
+[![Pipelines](https://gitlab.com/quantify-os/quantify-scheduler/badges/main/pipeline.svg)](https://gitlab.com/quantify-os/quantify-scheduler/pipelines/)
+[![PyPi](https://img.shields.io/pypi/v/quantify-scheduler.svg)](https://pypi.org/pypi/quantify-scheduler)
+[![Code Quality](https://app.codacy.com/project/badge/Grade/0c9cf5b6eb5f47ffbd2bb484d555c7e3)](https://www.codacy.com/gl/quantify-os/quantify-scheduler/dashboard?utm_source=gitlab.com&amp;utm_medium=referral&amp;utm_content=quantify-os/quantify-scheduler&amp;utm_campaign=Badge_Grade)
+[![Coverage](https://app.codacy.com/project/badge/Coverage/0c9cf5b6eb5f47ffbd2bb484d555c7e3)](https://www.codacy.com/gl/quantify-os/quantify-scheduler/dashboard?utm_source=gitlab.com&amp;utm_medium=referral&amp;utm_content=quantify-os/quantify-scheduler&amp;utm_campaign=Badge_Coverage)
+[![Documentation Status](https://readthedocs.com/projects/quantify-quantify-scheduler/badge/?version=latest&token=ed6fdbf228e1369eacbeafdbad464f6de927e5dfb3a8e482ad0adcbea76fe74c)](https://quantify-quantify-scheduler.readthedocs-hosted.com)
+[![License](https://img.shields.io/badge/License-BSD%203--Clause-blue.svg)](https://gitlab.com/quantify-os/quantify-scheduler/-/raw/main/LICENSE)
+[![Code style](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![Unitary Fund](https://img.shields.io/badge/Supported%20By-UNITARY%20FUND-brightgreen.svg?style=flat)](http://unitary.fund)
+
+![Quantify logo](https://orangeqs.com/logos/QUANTIFY_LANDSCAPE.svg)
+
+Quantify is a python based data acquisition platform focused on Quantum Computing and solid-state physics experiments.
+It is built on top of [QCoDeS](https://qcodes.github.io/Qcodes/) and is a spiritual successor of [PycQED](https://github.com/DiCarloLab-Delft/PycQED_py3).
+Quantify currently consists of [quantify-core](https://pypi.org/project/quantify-core/) and [quantify-scheduler](https://pypi.org/project/quantify-scheduler/).
+
+Take a look at the [latest documentation for quantify-scheduler](https://quantify-quantify-scheduler.readthedocs-hosted.com/) or use the switch at the bottom of the left panel to read the documentation for older releases.
+
+Quantify-scheduler is a python module for writing quantum programs featuring a hybrid gate-pulse control model with explicit timing control.
+The control model allows quantum gate- and pulse-level descriptions to be combined in a clearly defined and hardware-agnostic way.
+Quantify-scheduler is designed to allow experimentalists to easily define complex experiments, and produces synchronized pulse schedules to be distributed to control hardware.
+
+⚠️**Caution!**
+This is a pre-release **alpha version**, major changes are expected. Use for testing & development purposes only.
+
+## About
+
+Quantify-scheduler is maintained by The Quantify consortium consisting of Qblox and Orange Quantum Systems.
+
+
+[<img src="https://cdn.sanity.io/images/ostxzp7d/production/f9ab429fc72aea1b31c4b2c7fab5e378b67d75c3-132x31.svg" alt="Qblox logo" width=200px/>](https://qblox.com)
+&nbsp;
+&nbsp;
+&nbsp;
+&nbsp;
+[<img src="https://orangeqs.com/OQS_logo_with_text.svg" alt="Orange Quantum Systems logo" width=200px/>](https://orangeqs.com)
+
+&nbsp;
+
+The software is free to use under the conditions specified in the [license](https://gitlab.com/quantify-os/quantify-scheduler/-/raw/main/LICENSE).
+
+
+# Credits
+
+## Contributors
+
+- [Adam Lawrence](mailto:adam@orangeqs.com)
+- [Adriaan Rol](mailto:adriaan@orangeqs.com)
+- [Callum Attryde](mailto:cattryde@qblox.com)
+- [Christian Dickel](mailto:christiandickel8@gmail.com)
+- [Damaz de Jong](mailto:ddejong@qblox.com)
+- [Damien Crielaard](mailto:dcrielaard@qblox.com)
+- [Diogo Valada](mailto:dvalada@qblox.com)
+- [Edgar Reehuis](mailto:ereehuis@qblox.com)
+- [Gabor Oszkar Denes](mailto:gdenes@qblox.com)
+- [Gijs Vermarien](mailto:gijs@orangeqs.com)
+- [Hiresh Jadoenathmissier](mailto:hiresh@orangeqs.com)
+- [Jordy Gloudemans](mailto:jgloudemans@qblox.com)
+- [Jules van Oven](mailto:jules@qblox.com)
+- [Kelvin Loh](mailto:kelvin@orangeqs.com)
+- [Luis Miguens Fernandez](mailto:lmiguens@qblox.com)
+- [Michiel Dubbelman](mailto:michiel@orangeqs.com)
+- [Pieter Eendebak](mailto:pieter.eendebak@tno.nl)
+- [Robert Sokolewicz](mailto:rsokolewicz@qblox.com)
+- [Thomas Reynders](mailto:thomas@orangeqs.com)
+- [Viacheslav Ostroukh](mailto:viacheslav@orangeqs.com)
+- [Victor Negirneac](mailto:vnegirneac@qblox.com)
+
+
+
+# Changelog
+
+## 0.9.0 (2022-10-06)
+
+### Breaking changes
+
+- Deprecated methods removed:
+  - `QuantumDevice`
+    - `components` -> `elements`
+    - `get_component` -> `get_element`
+    - `add_component` -> `add_element`
+    - `remove_component` -> `remove_element`
+  - `ScheduleBase`
+    - `plot_circuit_diagram_mpl` -> `plot_circuit_diagram`
+    - `plot_pulse_diagram_mpl` -> `plot_pulse_diagram`  
+- Compilation - Compilation is now a graph. (#305, !407)
+- Operations - Allow moving to `qcodes` >=0.34 (#300, !473)
+    - Disallow `"_"` in `DeviceElement` names to comply with qcodes version 0.34
+    - Enforces `"_"` as the separator between device elements in `Edge` names
+    - Note: We are still on `qcodes` 0.33 due to pin in `quantify-core` package requirements
+- Operations, Resources, and Schedulables - Deprecate the use of the `data` argument (!455)
+- Qblox ICCs - Hotfix for storing scope acquisition (broken by !432) (!470)
+- Qblox ICCs - Only activate markers and LOs of used outputs to prevent noise (!474)
+
+### Merged branches and closed issues
+
+- Docs - Support for `myst-nb` added (#301, !407)
+- Docs - Sources are converted from restructured text format to MyST markdown. (!452)
+- Docs - Add pin on `nbclient<0.6` for Read-the-Docs to build; Remove various old temp requirement pins (!477)
+- Docs - Added documentation and unit tests for the Rxy, X, X90, Y and Y90 unitaries (#349)
+- Gettables - Added a `ProfiledScheduleGettable` for profiling execution times of schedule steps. (!420, !469)
+  - Please note: Setup in need of refactoring so interface is subject to change (see #320)
+- Instrument Coordinator - Small fix for `search_settable_param` when scheduler is searching for qcodes parameters (!461)
+- JSON utilities - Remove `repr` based serialization/deserialization methods (!445, #248)
+- JSON utilities - Extend the capabilities of the ``__getstate__/__setstate__`` json serializer (!445, #248)
+- Qblox ICCs - Added input/output gain/attenuation configurable hardware parameter (!458)
+- Structure - Pydantic-based model is now used to validate latency corrections. (!467, #333)
+- Zhinst backend - Raise a more understandable exception when compiling an acquisition with larger than allowed duration (!407).
+
+## 0.8.0 Support for two qubit operations and basic CZ-gate implementation (2022-08-10)
+
+### Breaking changes
+
+- Operations - Pin `qcodes` package to \<0.34.0 due to breaking `Edge` naming (#300, !409)
+- Qblox backend - Sequencers are now dynamically allocated. The hardware config file schema was changed. (!328)
+    - For each instrument, the config now contains a `portclock_configs` entry, a list with a dictionary of settings per port-clock combination
+    - See <https://quantify-quantify-scheduler.readthedocs-hosted.com/en/0.8.0/tutorials/qblox/recent.html>
+- Qblox backend - Strictly requires v0.7.x of the `qblox-instruments` package (!449)
+- Zhinst backend - Strictly requires v21.8.20515 of the `zhinst` package (!387)
+
+### Merged branches and closed issues
+
+- Compilation - Added `acq_protocol` optional parameter to the `Measure` gate. (!386)
+- Compilation - Call `determine_absolute_timing` in `qcompile` when no `device_cfg` supplied. (!436)
+- Compilation - Decrease test usage of deprecated transmon_test_config.json / add_pulse_information_transmon (!450)
+- DRAG Pulse - Removed an extra G_amp factor from the Q component (derivative pulse). (#298, !406)
+- Docs - Fix API reference pages on read-the-docs (#303, !413)
+- Docs - Pin sphinx to 5.0.2 due to crash in napoleon (!437)
+- Docs - Unpin sphinx >=5.1.1 (!445)
+- Docs - Fix jsonschemas not rendered on read-the-docs (!448)
+- Docs - Clarify port and clock concepts (!431)
+- Docs - New scheduler tutorials: Schedules and Pulses; Compiling to Hardware; Operations and Qubits (!336, !439)
+- Gettables - Added `generate_diagnostic_report` method to save the internal state of `ScheduleGettable` to a zip-file. (!408)
+- Helpers - Moved `MockLocalOscillator` definition from tests to `helpers.mock_instruments.MockLocalOscillator` (!392, !336).
+- JSON utilities - Add JSON serialization/deserialization methods based on `__getstate__`/`__setstate__` (!444)
+- Operations - Added a `symmetric` key in the `gate_info` to flag symmetric operations. (!389)
+- Operations - Introduce basic CZ-gate via `CompositeSquareEdge` (utilizing `quantify_scheduler.operations.pulse_factories.composite_square_pulse`) (!411)
+    - Replaces the incomplete `SuddenNetZeroEdge` basic CZ-gate implementation
+- Operations - Rxy theta rotations now fall into the domain of \[-180 to 180) degrees. (!433)
+- QuantumDevice - Added implementation for `edges` in the quantum device config in order to support two qubit operations. (!389)
+    - The `Edge` has been added as an abstract base class for edges to be added to a device.
+- Qblox backend - Only add clocks to the schedule that are actually being used, avoids trying to assign frequencies for unused clocks (#278, !371)
+- Qblox backend - Fix for supplying negative NCO phase (!393)
+- Qblox backend - Fix compilation of ShiftClockPhase (!404, broken by merge of !328)
+- Qblox backend - Fix for outputting signals on even output paths of qblox hardware in real_output_x mode (!397)
+- Qblox backend - Make Qblox backend compatible with generic downconverter values in hardware_config (!418)
+- Qblox backend - Fix for 90 degree phase shift on even output paths as a result of the !397 hotfix. (!412)
+- Qblox backend - Fix cluster compatibility when converting old hwconfig to new specs (!419)
+- Qblox backend - Latency corrections must now be defined in top layer of hw config (!400)
+- Qblox backend - Fix combination of cluster and latency corrections when converting hw_configs to new specs  (!417)
+- Qblox backend - Fix handling of composite pulses (#299, !411)
+- Qblox backend - Implementation of distortion correction (#285, !388)
+- Qblox backend - Fix incompatibility of distortion_correction parameters as numpy arrays (!426)
+- Qblox backend - Remove all references to the inactive `line_gain_db` param (!435)
+- Qblox ICCs - Fix for setting `scope_acq_sequencer_select` for QRM and QRM-RF (!432, !441)
+- Qblox ICCs - Fix `ClusterComponent.prepare` mutating the schedule (!443)
+- Schedules - Revert rename of `trace_schedule` done in !432 and rename new schedule using gates to `trace_schedule_circuit_layer` (!442)
+- Schedules - Make `AcquisitionMetadata` a serializable class (!446)
+
+## 0.7.0 Support for qblox-instruments v0.6.0, new BasicTransmonElement, change for triggers in Zhinst backend (2022-04-11)
+
+### Breaking changes
+
+- Qblox ICCs - Updated Qblox components for using the new unified-style qblox driver (see <https://gitlab.com/quantify-os/quantify-scheduler/-/wikis/Qblox-ICCs:-Interface-changes-in-using-qblox-instruments-v0.6.0>) (!377).
+- Qblox backend - Strictly requires v0.6.0 of the qblox-instruments package (!377).
+- Zhinst backend - Hardware config for the devices. Replaced keyword "triggers" to "trigger", and the value type from `List[int]` to `int`. E.g. old style, `"triggers": [2]`, new style, `"trigger": 2` (#264, !372).
+
+### Merged branches and closed issues
+
+- QuantumDevice - The `DeviceElement` has been added as an abstract base class for elements to be added to a device (#148, !374).
+- QuantumDevice - The `BasicTransmonElement` has been added that generates a device config in a more structured manner (#246, !374).
+- QuantumDevice - Fixed a bug in the `BasicTransmonElement` where operations had clock-frequencies (`float`) specified instead of clocks (`str`) (!379).
+- QuantumDevice - The `TransmonElement` will be deprecated after version 0.8 (!374).
+
+## 0.6.0 Full support for multiplexed readout, transmon element update, fixes to backends (2022-03-10)
+
+### Breaking changes
+
+- Compilation - Deprecated `add_pulse_information_transmon` in favor of `compilation.backends.circuit_to_device.compile_circuit_to_device` (#64, #67, !339).
+- Compilation - attempting compilation with missing values in the `DeviceCompilationConfig` configuration will now raise validation errors. Be sure to set initial values when generating a config using the `QuantumDevice` object (!339)
+- Compilation - Device compile making use of `.compile_circuit_to_device` no longer modifies the input schedule (#249, !339).
+- Compilation - When specifying multiple timing constraints for a schedulable, the constraint specifying the latest time determines the absolute time of the shedulable (!309)
+- Gettables - `ScheduleGettableSingleChannel` renamed to `ScheduleGettable` as it now supports multiple acquisition channels (!299).
+- Hardware config - Removed the need for a `ic_` prefix from the hardware config (!312).
+- Instrument Coordinator - IC now adds a `GenericInstrumentCoordinatorComponent` to itself on instantiation by default (!350)
+- Instrument Coordinator - IC stop function has an `allow_failure` parameter which allows IC components attached to it to fail to stop with warning instead of raising errors. Allows for situations when some components cannot have a stop instruction sent before the prepare stage. (!359)
+- Operations - The internal behavior of how acquisition channels and acquisition indices are configured in the `Measure` operation has changed slightly. See #262 for details. (!339).
+- Operations - Added "operation_type" key to the schema. (!345)
+- Structure - `Schedule.timing_constraints` has been renamed to `Schedule.schedulables`. It now points to a dictionary of schedulables rather than a list of dicts. (!309)
+- Structure - Pydantic-based model is now used for the data structures. (!341)
+- Visualization - Deprecated `plot_circuit_diagram_mpl` and `plot_pulse_diagram_mpl` in `ScheduleBase` in favour of `plot_circuit_diagram` and `plot_pulse_diagram` (!313)
+- Qblox backend - Strictly requires v0.5.4 of the qblox-instruments package (!314)
+- Zhinst backend - Due to !312, the csv files used to upload the waveforms to the UHFQA no longer use the `ic_` prefix in their filenames. (!334)
+- Zhinst backend - Fixes bug when doing SSRO experiments. No more duplicated shots. Adds support for BinMode.APPEND during compilation. (#276, !358)
+- Zhinst backend - Removed `latency` and `line_trigger_delay` keys in the channels of the devices for the Zhinst hardware config. (!363)
+- Zhinst backend - Added `latency_corrections` main entry in the Zhinst hardware config for latency corrections on a port-clock combination basis. (!363)
+
+### Merged branches and closed issues
+
+- Compilation - Added a new compilation backend `compilation.backends.circuit_to_device.compile_circuit_to_device` for the quantum-circuit to quantum-device layer (#64, #67, !339).
+- Compilation - Fixed `add_pulse_information_transmon` when using "Trace" acquisition mode (!300)
+- Compilation - Fixed the deprecation warnings from pandas `DataFrame.append`. (!347)
+- Docs - Pinning qcodes package to \<0.32.0 due to Read the Docs API reference failure (!361)
+- Gettables - `ScheduleGettable` now first stops all instruments in IC during initialization (!324)
+- Schedules - Adds a multiplexing verification schedule. (!329)
+- Operations - Sudden Net Zero from Negirneac 2021 added to the `pulse_library` (!339)
+- Operations - Docstrings for the X90, X, Y90, Y, and Rxy gate unitary have been aligned with literature. (#261, !305)
+- Operations - Adds an optional "data" argument to staircase pulse. (!335)
+- Pulse library - Added `ShiftClockPhase` operation that can be used to shift the phase of a clock during execution of a `Schedule` (!346)
+- Pulse library - Added a numerically defined pulse. (!157)
+- QuantumDevice - Unknown values are initialized as `float('nan')` (#274, !356)
+- TransmonElement - Corrected the motzoi parameter range validator. (!351)
+- Visualization - Adds visualisation of acquisitions to plotly pulse diagrams (!304)
+- Visualization - Add `plot_pulse_diagram` and `plot_circuit_diagram` to schedule for easier method names, and enable plotly visualization directly from `ScheduleBase` (!313)
+- Utilities - Migrates the utilities from quantify-core. (!357)
+- Generic ICC - Adds support for nested parameters. (!330)
+- Qblox ICCs - Stop now disables sync on all sequencers to prevent hanging during next run, where it gets re-enabled if needed (!324)
+- Qblox ICCs - `_QRMAcquisitionManager._get_scope_data` now has correct return type (#232, !300)
+- Qblox ICCs - Fixed bug where QRM scope mode sequencer does not get set correctly (!342)
+- Qblox ICCs - Fixed reference source cluster issue when it is not being set correctly. (!323)
+- Qblox backend - NCO phase now gets reset every averaging loop (!337)
+- Qblox backend - Enables RF output switch at the start of a program. (!344)
+- Qblox backend - Added logic for changing the NCO phase during execution of a `Schedule` (!346)
+- Qblox backend - Added ability to correct for latency by delaying program execution on a per sequencer basis (!325)
+- Qblox backend - Compilation with local oscillators changed to work with generic instrument coordinator components (!306)
+- Qblox backend - Refactored operation handling and greatly increased test coverage (!301).
+- Qblox backend - Made max duration of wait instructions (!319).
+- Qblox backend - Fixed an issue with the downconverter frequency correction. (!318)
+- Qblox backend - Temporary fix for a floating point rounding error when calculating the length of pulses. (#284, !365)
+- Zhinst backend - Fixed the ZI resolver return typehint. (!307)
+- Zhinst backend - Fixed an issue when compiling seqc programs for multiple sequencers end up overwriting the first sequencer. (!340, #260)
+
+## 0.5.2 Fixes to backends, and other incremental fixes  (2021-12-08)
+
+### Breaking changes
+
+- Dependency on `jsonschema` has been replaced with `fastjsonschema`. (!284, !293)
+- Zhinst hardware config json schema has changed. See the example schema. (!283)
+- In `hardware_compile` function, the `hardware_map` is changed to `hardware_cfg` parameter. (!279)
+- Remove enum tools dependency (!270)
+
+### Merged branches and closed issues
+
+- Compilation - The `determine_absolute_scheduling` function now sorts the list of labels in the timing constraints, and then a binary search (via `np.searchsorted`) is applied. (!272, !274)
+- Compilation - Make `device_cfg` an optional argument of qcompile(!281)
+- Compilation - renamed the hardware_mapping argument of qcompile into hardware_cfg (#165, !279)
+- Compilation - Introduced the hardware_compile function to perform the hardware compilation returning a CompiledSchedule (#224, !279)
+- Docs - Updating user guide to mention correctly the QuantumDevice and ScheduleGettable(s) available. (!209)
+- Infrastructure - Adds rich package in the requirements since tutorials use it. (!276)
+- Operations - The `locate` function now uses the `functools.lru_cache` to cache the result (only for python >= 3.8). For python 3.7, behaviour remains the same.  (!273, !275)
+- Operations - Resolved a minor issue where identical Rxy rotations (for angles >360) would be treated as separate operations in a schedule (!263)
+- Visualization - Adds a function `plot_acquisition_operations` which together with the new `AcquisitionOperation` class will help highlight acquisition pulses in the pulse diagrams. (!271, !277)
+- Zhinst backend - Large parts of the Zhinst backend have been rewritten. This should resolve a range of issues. (!263)
+    - Calculation of the timelines for different operations now makes using of a timing table, improving code readability and debugability.
+    - Timing issues related to triggering should be resolved (#218)
+    - The backend can now always use the same hardware configuration file (#214)
+    - Acquisition is now done using the StartQA instruction (#213)
+    - error handling in the Zhinst backend has been improved catching several exceptions at compile time of the schedule instead of manifesting in unexpected results during runtime.
+    - Local oscillators through the ZI backend uses the GenericInstrumentCoordinatorComponent. Configures other parameters other than frequency. (!283, #204)
+- Qblox backend - only check major and minor version when checking compatibility with the qblox_instruments package (!290)
+    - Added support for the Qblox Downconverter (!297)
+    - Added workaround for staircase_amplitude. (!292)
+    - Fix looped acquisition integration time, fix acquire index offset by one (!291)
+    - Qblox instruments version == 0.5.3 (!289)
+    - Fix sequencer_sync_en not being reset in the qblox instrument coordinator component. (!285)
+    - Fix rounding of time to samples in qblox backend (!282)
+    - Fix pulse stitching at zero amplitude. (!280)
+    - Allow instruction generated staircase with modulation (!278)
+- Utilities - Improve JSON validation speed (!284)
+- Utilities - Improve operation deserialization speed (!273)
+- Bugfix - For calculating the pulse area, the mathematical area is used instead of area of sampled pulse. (!242, !286)
+- Bugfix - Fix for plot window operations (!294)
+
+## 0.5.1 Incremental fixes, refactoring, and addition of convenience methods and classes (2021-11-11)
+
+### Breaking changes
+
+- InstrumentCoordinator - `last_schedule` is now a property (!252).
+- Structure - We have refactored the Operation and Schedule classes out of the types module and moved the different operation libraries (acquisition_library, gate_library, and pulse_library) (#217, !256).
+    - `quantify_scheduler.types.Operation` -> `quantify_scheduler.operations.operation.Operation`, the import `quantify_scheduler.Operation` still works.
+    - `quantify_scheduler.types.Schedule` -> `quantify_scheduler.schedules.schedule.Schedule`, the import `quantify_scheduler.Schedule` still works.
+    - `quantify_scheduler.types.CompiledSchedule` -> `quantify_scheduler.schedules.schedule.CompiledSchedule`
+    - `quantify_scheduler.types.ScheduleBase` -> `quantify_scheduler.schedules.schedule.ScheduleBase`
+    - `quantify_scheduler.types.AcquisitionMetadata` -> `quantify_scheduler.schedules.schedule.AcquisitionMetadata`
+    - `quantify_scheduler.acquisition_library` -> `quantify_scheduler.operations.acquisition_library`
+    - `quantify_scheduler.gate_library` -> `quantify_scheduler.operations.gate_library`
+    - `quantify_scheduler.pulse_library` -> `quantify_scheduler.operations.pulse_library`
+
+### Merged branches and closed issues
+
+- Control - Add option to set output port in heterodyne_spec_sched (!262)
+- Control - Expand SingleChannelScheduleGettable to support trace acquisitions (!248)
+- Control - Update create_dc_compensation_pulse behaviour and docstring. (!244)
+- Control - Refactor ScheduleGettableSingleChannel (!240, !249)
+- Control - Reduce the default init_duration of spectroscopy schedules (!237)
+- Generic ICC - Added a GenericInstrumentCoordinatorComponent. (!267)
+- ICCs - InstrumentCoordinatorComponentBase now has a `force_set_parameter` as a ManualParameter to enable the user to switch the lazy_set behaviour when setting parameters of the instruments connected to the InstrumentCoordinatorComponent. (!267)
+- Qblox ICCs - Adds a lazy_set behaviour by default when setting parameters with the same value to an instrument connected to the Qblox ICC. (!230)
+- Visualization - made matplotlib schedule visualization methods accessible as methods `plot_circuit_diagram_mpl` and `plot_pulse_diagram_mpl` of the `Schedule` class (!253)
+- Visualization - resolved a bug where a schedule was modified when drawing a circuit diagram (#197, !250)
+- Visualization - Add support for window operation to transmon backend (!245)
+- Infrastructure - Fix and enhance pre-commit + add to CI (!257, !265)
+- Infrastructure - Added prospector config file for CI. (!261)
+- Bugfix - Removed redundant `determine_absolute_timing` step in `qcompile`. (!259)
+- Bugfix - Ramp pulse sampling utilizing `np.linspace` behaviour changed. (!258)
+- Docs - Adds the new Quantify logo similar to quantify_core. (!266)
+- Docs - Enhance documentation of public API for reimported modules \[imports aliases\] (!254)
+- Docs - Fixes the funcparserlib error in rtd. (!251)
+- Docs - Updated Qblox backend docs to include the new features. (!247)
+
+## 0.5.0 Expanded feature sets hardware compilation backends (2021-10-25)
+
+### Breaking changes
+
+- The `schedules.timedomain_schedules.allxy_sched` function no longer accepts the string "All" as an argument to the `element_select_idx` keyword.
+- The `QuantumDevice.cfg_nr_averages` parameter was renamed to `QuantumDevice.cfg_sched_repetitions`
+- The call signature of `gettables.ScheduleVectorAcqGettable` has been renamed to `gettables.ScheduleGettableSingleChannel`, and the call signature has been updated according to #36 to no longer accept several keyword arguments.
+- Qblox Backend - The NCO phase is now reset at the start of a program (!213).
+- Qblox Backend - Compilation now requires qblox_instruments version 0.5.0, 0.5.1 or 0.5.2 (!214, !221).
+
+### Merged branches and closed issues
+
+- Compilation - Added the ability to specify the BinMode at the quantum-circuit layer (#183, !180).
+- Compilation - qcompile no longer modifies schedules (#102, !178).
+- Control - Added a first version of the QuantumDevice object (#148, !180).
+- Control - A single-qubit ScheduleGettable has been added (#36, !180).
+- Docs - Added bibliography with sphinxcontrib-bibtex extension (!171).
+- Docs - Fixed missing files in API reference (!176).
+- InstrumentCoordinator - CompiledSchedule class added to specify interfaces of InstrumentCoordinator and compilation functions (#174, !177).
+- InstrumentCoordinator - CompiledSchedule.last_schedule method added to provide access to last executed schedule (#167, !177).
+- Qblox Backend - Added support for qblox_instruments version 0.4.0 (new acquisition path) (!143).
+- Qblox Backend - Added support for real time mixer corrections rather than pre-distorting the uploaded waveforms (!192).
+- Qblox Backend - Waveforms are now compared using the normalized data array rather than the parameterized description (!182).
+- Qblox Backend - Support for append bin mode (#184, !180).
+- Qblox Backend - Support for using real value pulses on arbitrary outputs added (!142).
+- Qblox Backend - Compilation now supports 6 sequencers for both the QCM as well as the QRM (!142).
+- Qblox Backend - Support for a cluster, along with its QCM, QRM, QCM-RF and QRM-RF modules (!164)
+- Qblox Backend - Registers are now dynamically allocated during compilation (!195)
+- Zhinst backend - No exception is raised when an LO that is in the config is not part of a schedule. (#203, !223)
+- Zhinst backend - Instrument coordinator components for ZI will only be configured when the settings used to configure it have changed (#196, !227)
+- Zhinst backend - Solved a bug that caused single-sideband demodulation to not be configured correctly when using the UHFQA (!227)
+- Zhinst backend - Warnings raised during compilation of seqc programs will no longer raise an exception but will use logging.warning (!227)
+- Zhinst backend - resolved a bug where the instrument coordinator cannot write waveforms to the UHFQA if it has never been used before (!227)
+- Zhinst backend - resolved a bug where multiple identical measurements in a schedule would result in multiple integration weights being uploaded to the UFHQA (#207, !234)
+- Zhinst backend - resolved a bug where the UHFQA would not be triggered properly when executing a schedule with multiple samples (batched mode) (#205, !234)
+- Qblox ICCs - Compensated integration time for Qblox QRM IC component (!199).
+- Qblox ICCs - Added error handling for error flags given by `get_sequencer_state` (!215)
+- QuantumDevice - Added docstrings to the TransmonElement parameters (!216, !218)
+- Qblox ICCs - QCoDeS parameters are now only set if they differ from the value in the cache (!230)
+- Visualization - Allow user defined axis for plotting circuit diagram (!206)
+- Visualization - Adds schedule plotting using matplotlib and a WindowOperation to help visualize pulse diagrams (!225, !232)
+- Other - Added method `sample_schedule` to sample a `Schedule` (!212)
+- Other - The `RampPulse` has an extra (optional) parameter `offset` (!211)
+- Other - Updated existing schedules to make use of the acquisition index (#180, !180).
+- Other - Added a function to extract acquisition metadata from a schedule (#179, !180).
+- Other - The soft square waveform can now be evaluated with only one datapoint without raising an exception (!235)
+- Other - Added a function that generates a square pulse that compensates DC components of a sequence of pulses (!173)
+
+## 0.4.0 InstrumentCoordinator and improvements to backends (2021-08-06)
+
+### Breaking changes
+
+- Change of namespace from quantify.scheduler.\* to quantify_scheduler.\*
+
+### Merged branches and closed issues
+
+- Changes the namespace from quantify.scheduler to quantify_scheduler (!124)
+- InstrumentCoordinator - Add is_running property and wait_done method. Closes #133 (!140)
+- InstrumentCoordinator - Add instrument coordinator reference parameter to transmon element (!152)
+- InstrumentCoordinator - Prefix serialized settings for ZI ControlStack components. (!149)
+- InstrumentCoordinator - Refactored ControlStack name to InstrumentCoordinator (!151)
+- InstrumentCoordinator - Make use of InstrumentRefParameters (!144)
+- InstrumentCoordinator - Add controlstack class (!70)
+- InstrumentCoordinator - Add Zurich Instruments InstrumentCoordinatorComponent. (!99)
+- InstrumentCoordinator - Add Qblox InstrumentCoordinatorComponent. (!112)
+- InstrumentCoordinator - Avoid garbage collection for instrument coordinator components (!162)
+- Qblox backend - Removed limit in Qblox backend that keeps the QCM sequencer count at 2 (!135)
+- Qblox backend - Restructured compilation using external local oscillators. (!116)
+- Qblox backend - Added Chirp and Staircase pulses; and efficient implementation for QD spin qubit experiments (!106)
+- Qblox backend - Only run `start_sequencer` on pulsar instruments which have been armed (!156)
+- Zhinst backend - Assert current with new sequence program to skip compilation (!131)
+- Zhinst backend - Deserialize zhinst settings from JSON to ZISettingsBuilder (!130)
+- Zhinst backend - Add waveform mixer skewness corrections (!103)
+- Zhinst backend - Add backend option to enable Calibration mode (#103, !123)
+- Zhinst backend - Replace weights string array with a numerical array in JSON format (!148)
+- Zhinst backend - Add grouping of instrument settings (!133)
+- Zhinst backend - Add qcompile tests for the zurich instruments backend (!118)
+- Zhinst backend - Add repetitions parameter (!138)
+- Zhinst backend - Fixes the bug where the seqc in the datadir is not copied to the webserver location. (!165)
+- Fix for circuit diagram plotting failure after pulse scheduling (#157, !163)
+- Fixed typo in the gate_info of the Y gate in the gate_library (!155)
+- Add artificial detuning in Ramsey Schedule and bug fixes (!120)
+- Use individual loggers per python file (!134)
+- Recolour draw circuit diagram mpl (!96)
+- Fix issues with timedomain schedules (!145)
+- Renamed input parameters of quantify_scheduler.schedules.\* functions. (!136)
+- Added acquisitions to circuit diagram (!93)
+- Add string representations to acquisition protocols of the acquisitions library (!114)
+- Transmon element and config generation (!75)
+- Rename operation_hash to operation_repr (!122)
+- Add types.Schedule from_json conversion (!119)
+- Add missing return types (!121)
+- Add serialization to Operations (!110)
+
+## 0.3.0 Multiple backends support (2021-05-20)
+
+- Added support for both Qblox and Zurich Instrument backends.
+- Added convenience pylintrc configuration file.
+- Added examples for timedomain and spectroscopy schedules.
+
+### Breaking changes
+
+- Major refactor of the Qblox backend. (For example, it's now `quantify_core.backends.qblox_backend` instead of the previous `quantify_core.backends.pulsar_backend`)
+- Qblox backend requires strictly v0.3.2 of the qblox-instruments package.
+
+### Merged branches and closed issues
+
+- Add mixer skewness corrections helper function. (!102)
+- Added Qblox backend support. (!81)
+- Compile backend with ZISettingsBuilder. (!87)
+- Add vscode IDE config files. (!100)
+- Add ZISettingsBuilder class. (!86)
+- Added representation to gates in gate library and defined equality operation. (!101)
+- Fix/operation duration. Fixes #107. (!89)
+- Feat/long pulses fix validators name. (!90)
+- Implemented long square pulses unrolling (for waveform-memory-limited devices). (!83)
+- Changed Qblox-Instruments version to 0.3.2. (!88)
+- Feature: Improve overall zhinst backend timing. (!77)
+- Plotly cleanup. (!69)
+- Pulsar backend version bump. (!82)
+- Added zhinst backend support. (!49)
+- Added example timedomain programs. (!71)
+- Added example spectroscopy programs. (!64)
+- Added pylintrc configuration file. (!55)
+- Added repetitions property to Schedule. (!56)
+- Added Acquisition Protocols. (!51)
+- Hotfix for filename sanitization pulsar backend. (!61)
+- Pulsar backend function sanitization. (!60)
+- Potential fix time-out pulsar. (!58)
+- Updated Pulsar backend version to v0.2.3.. (!57)
+- Fixed datadir related bugs. (!54)
+- Added Station implementation. (!52)
+- Pulsar backend v0.2.2 check. (!48)
+- Fix for issue with acq delay. (!45)
+- Fix for issue #52. (!44)
+- Add artificial detuning to Ramsey schedule (!120)
+- Added support for the Qblox Pulsar QCM-RF/QRM-RF devices (!158)
+
+## 0.2.0 Hybrid pulse- gate-level control model (2021-01-14)
+
+- Major refactor of the scheduler resource code enabling hybrid pulse- gate-level control.
+- Moved quantify_scheduler.types.Resource class to a separate quantify_scheduler.resources module.
+- Adds a BasebandClockResource class within the newly created quantify_scheduler.resources module.
+- Moved QRM and QCM related classes to the quantify_scheduler.backends.pulsar_backend module.
+- In quantify_scheduler.compilation, rename of function '\_determine_absolute_timing' to 'determine_absolute_timing'. Argument changed from clock_unit to time_unit.
+- In quantify_scheduler.compilation, rename of function '\_add_pulse_information_transmon' to 'add_pulse_information_transmon'.
+- Added ramp waveform in quantify_scheduler.waveforms.
+- Added schemas for operation and transmon_cfg.
+- Added a basic hybrid visualisation for pulses using new addressing scheme.
+- Operations check whether an operation is a valid gate or pulse.
+- Refactor of visualization module. Moved quantify_scheduler.backends.visualization to quantify_scheduler.visualization module. Expect code breaking reorganization and changes to function names.
+- Pulsar backend version now checks for QCM and QRM drivers version 0.1.2.
+
+### Merged branches and closed issues
+
+- fix(pulse_scheme): Add tickformatstops for x-axis using SI-unit 'seconds'. Closes #39. (!39)
+- Resolve "y-axis label is broken in plotly visualization after resources-refactor". Closes #45. (!38)
+- Resources refactor (!28, !29, !30)
+- Hybrid visualisation for pulses and circuit gate operations. Closes #22 and #6. (!27)
+- Support Pulsar parameterisation from scheduler. Support feature for #29. (!2)
+- Operation properties to check if an operation is a valid gate or pulse. Closes #28 (!25)
+- Visualisation refactor. Closes #26. (!22)
+- Windows job (!20)
+- Changed Pulsar backend version check from 0.1.1 to 0.1.2. (!21)
+
+## 0.1.0 (2020-10-21)
+
+- Refactored scheduler functionality from quantify-core into quantify-scheduler
+- Support for modifying Pulsar params via the sequencer #54 (!2)
+- Simplification of compilation through `qcompile` (!1)
+- Qubit resources can be parameters of gates #11 (!4)
+- Circuit diagram visualization of operations without no pulse info raises exception #5 (!5)
+- Pulsar backend verifies driver and firmware versions of hardware #14 (!6)
+- Sequencer renamed to scheduler #15 (!7)
+- Documentation update to reflect refactor #8 (!8)
+- Refactor circuit diagram to be more usable !10 (relates to #6)
+- Unify API docstrings to adhere to NumpyDocstring format !11
+- Changes to addressing of where a pulse is played !9 (#10)
+- Renamed doc -docs folder for consistency #18 (!12)
+- Moved test folder outside of project #19 (!14)
+- Add copyright notices and cleanup documenation #21 (!13)
+- Add installation tip for plotly dependency in combination with jupyter #24 (!15)
+
+```{note}
+- \# denotes a closed issue.
+- ! denotes a merge request.
+```
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `quantify-scheduler-0.8.0/README.rst` & `quantify-scheduler-0.9.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,85 +1,42 @@
-==================
-quantify-scheduler
-==================
-
-.. image:: https://img.shields.io/badge/slack-chat-green.svg
-    :target: https://join.slack.com/t/quantify-hq/shared_invite/zt-vao45946-f_NaRc4mvYQDQE_oYB8xSw
-    :alt: Slack
-
-.. image:: https://gitlab.com/quantify-os/quantify-scheduler/badges/main/pipeline.svg
-    :target: https://gitlab.com/quantify-os/quantify-scheduler/pipelines/
-    :alt: Pipelines
-
-.. image:: https://img.shields.io/pypi/v/quantify-scheduler.svg
-    :target: https://pypi.org/pypi/quantify-scheduler
-    :alt: PyPi
-
-.. image:: https://app.codacy.com/project/badge/Grade/0c9cf5b6eb5f47ffbd2bb484d555c7e3
-    :target: https://www.codacy.com/gl/quantify-os/quantify-scheduler/dashboard?utm_source=gitlab.com&amp;utm_medium=referral&amp;utm_content=quantify-os/quantify-scheduler&amp;utm_campaign=Badge_Grade
-    :alt: Code Quality
-
-.. image:: https://app.codacy.com/project/badge/Coverage/0c9cf5b6eb5f47ffbd2bb484d555c7e3
-    :target: https://www.codacy.com/gl/quantify-os/quantify-scheduler/dashboard?utm_source=gitlab.com&amp;utm_medium=referral&amp;utm_content=quantify-os/quantify-scheduler&amp;utm_campaign=Badge_Coverage
-    :alt: Coverage
-
-.. image:: https://readthedocs.com/projects/quantify-quantify-scheduler/badge/?version=latest&token=ed6fdbf228e1369eacbeafdbad464f6de927e5dfb3a8e482ad0adcbea76fe74c
-    :target: https://quantify-quantify-scheduler.readthedocs-hosted.com
-    :alt: Documentation Status
-
-.. image:: https://img.shields.io/badge/License-BSD%203--Clause-blue.svg
-    :target: https://gitlab.com/quantify-os/quantify-scheduler/-/raw/main/LICENSE
-    :alt: License
-
-.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
-    :target: https://github.com/psf/black
-    :alt: Code style
-
-.. image:: https://img.shields.io/badge/Supported%20By-UNITARY%20FUND-brightgreen.svg?style=flat
-    :target: http://unitary.fund
-    :alt: Unitary Fund
-
-.. figure:: /images/QUANTIFY_LANDSCAPE.svg
-    :align: center
-    :alt: Quantify logo
+# quantify-scheduler
+
+[![Slack](https://img.shields.io/badge/slack-chat-green.svg)](https://join.slack.com/t/quantify-hq/shared_invite/zt-vao45946-f_NaRc4mvYQDQE_oYB8xSw)
+[![Pipelines](https://gitlab.com/quantify-os/quantify-scheduler/badges/main/pipeline.svg)](https://gitlab.com/quantify-os/quantify-scheduler/pipelines/)
+[![PyPi](https://img.shields.io/pypi/v/quantify-scheduler.svg)](https://pypi.org/pypi/quantify-scheduler)
+[![Code Quality](https://app.codacy.com/project/badge/Grade/0c9cf5b6eb5f47ffbd2bb484d555c7e3)](https://www.codacy.com/gl/quantify-os/quantify-scheduler/dashboard?utm_source=gitlab.com&amp;utm_medium=referral&amp;utm_content=quantify-os/quantify-scheduler&amp;utm_campaign=Badge_Grade)
+[![Coverage](https://app.codacy.com/project/badge/Coverage/0c9cf5b6eb5f47ffbd2bb484d555c7e3)](https://www.codacy.com/gl/quantify-os/quantify-scheduler/dashboard?utm_source=gitlab.com&amp;utm_medium=referral&amp;utm_content=quantify-os/quantify-scheduler&amp;utm_campaign=Badge_Coverage)
+[![Documentation Status](https://readthedocs.com/projects/quantify-quantify-scheduler/badge/?version=latest&token=ed6fdbf228e1369eacbeafdbad464f6de927e5dfb3a8e482ad0adcbea76fe74c)](https://quantify-quantify-scheduler.readthedocs-hosted.com)
+[![License](https://img.shields.io/badge/License-BSD%203--Clause-blue.svg)](https://gitlab.com/quantify-os/quantify-scheduler/-/raw/main/LICENSE)
+[![Code style](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![Unitary Fund](https://img.shields.io/badge/Supported%20By-UNITARY%20FUND-brightgreen.svg?style=flat)](http://unitary.fund)
+
+![Quantify logo](https://orangeqs.com/logos/QUANTIFY_LANDSCAPE.svg)
 
 Quantify is a python based data acquisition platform focused on Quantum Computing and solid-state physics experiments.
-It is build on top of `QCoDeS <https://qcodes.github.io/Qcodes/>`_ and is a spiritual successor of `PycQED <https://github.com/DiCarloLab-Delft/PycQED_py3>`_.
-Quantify currently consists of `quantify-core <https://pypi.org/project/quantify-core/>`_ and `quantify-scheduler <https://pypi.org/project/quantify-scheduler/>`_.
+It is built on top of [QCoDeS](https://qcodes.github.io/Qcodes/) and is a spiritual successor of [PycQED](https://github.com/DiCarloLab-Delft/PycQED_py3).
+Quantify currently consists of [quantify-core](https://pypi.org/project/quantify-core/) and [quantify-scheduler](https://pypi.org/project/quantify-scheduler/).
 
-Take a look at the `latest documentation for quantify-scheduler <https://quantify-quantify-scheduler.readthedocs-hosted.com/>`_ or use the switch in the bottom of left panel to read the documentation for older releases.
+Take a look at the [latest documentation for quantify-scheduler](https://quantify-quantify-scheduler.readthedocs-hosted.com/) or use the switch at the bottom of the left panel to read the documentation for older releases.
 
 Quantify-scheduler is a python module for writing quantum programs featuring a hybrid gate-pulse control model with explicit timing control.
 The control model allows quantum gate- and pulse-level descriptions to be combined in a clearly defined and hardware-agnostic way.
 Quantify-scheduler is designed to allow experimentalists to easily define complex experiments, and produces synchronized pulse schedules to be distributed to control hardware.
 
-.. caution::
+⚠️**Caution!**
+This is a pre-release **alpha version**, major changes are expected. Use for testing & development purposes only.
 
-    This is a pre-release **alpha version**, major changes are expected. Use for testing & development purposes only.
-
-About
------
+## About
 
 Quantify-scheduler is maintained by The Quantify consortium consisting of Qblox and Orange Quantum Systems.
 
-.. |_| unicode:: 0xA0
-   :trim:
-
-
-.. figure:: https://cdn.sanity.io/images/ostxzp7d/production/f9ab429fc72aea1b31c4b2c7fab5e378b67d75c3-132x31.svg
-    :width: 200px
-    :target: https://qblox.com
-    :align: left
-
-.. figure:: https://orangeqs.com/OQS_logo_with_text.svg
-    :width: 200px
-    :target: https://orangeqs.com
-    :align: left
-
-|_|
-
 
-|_|
+[<img src="https://cdn.sanity.io/images/ostxzp7d/production/f9ab429fc72aea1b31c4b2c7fab5e378b67d75c3-132x31.svg" alt="Qblox logo" width=200px/>](https://qblox.com)
+&nbsp;
+&nbsp;
+&nbsp;
+&nbsp;
+[<img src="https://orangeqs.com/OQS_logo_with_text.svg" alt="Orange Quantum Systems logo" width=200px/>](https://orangeqs.com)
 
-The software is free to use under the conditions specified in the `license <https://gitlab.com/quantify-os/quantify-scheduler/-/raw/main/LICENSE>`_.
+&nbsp;
 
-.. nothing-to-avoid-a-sphinx-warning:
+The software is free to use under the conditions specified in the [license](https://gitlab.com/quantify-os/quantify-scheduler/-/raw/main/LICENSE).
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `quantify-scheduler-0.8.0/docs/Makefile` & `quantify-scheduler-0.9.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `quantify-scheduler-0.8.0/docs/conf.py` & `quantify-scheduler-0.9.0/docs/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 # If your documentation needs a minimal Sphinx version, state it here.
 #
 # needs_sphinx = '1.0'
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom ones.
 extensions = [
+    "myst_nb",
     "sphinx.ext.autodoc",  # auto document docstrings
     "sphinx.ext.napoleon",  # autodoc understands numpy docstrings
     # load after napoleon, improved compatibility with type hints annotations
     "sphinx_autodoc_typehints",
     "sphinx.ext.viewcode",
     "sphinx.ext.intersphinx",
     "sphinx.ext.autosectionlabel",
@@ -49,15 +50,14 @@
     "jupyter_sphinx",
     "sphinx_togglebutton",
     # fancy type hints in docs and
     # solves the same issue as "sphinx_automodapi.smart_resolver"
     # however the smart_resolver seems to fail for external packages like `zhinst`
     "scanpydoc.elegant_typehints",
     "sphinxcontrib.bibtex",
-    "quantify_core.sphinx_extensions.notebook_to_jupyter_sphinx",
     "autoapi.extension",
 ]
 
 
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ["_templates"]
 
@@ -88,15 +88,15 @@
 bibtex_reference_style = "author_year"
 
 
 # The suffix(es) of source filenames.
 # You can specify multiple suffix as a list of string:
 #
 # source_suffix = ['.rst', '.md']
-source_suffix = ".rst"
+source_suffix = [".rst", ".md"]
 
 # The master toctree document.
 master_doc = "index"
 
 # General information about the project.
 project = "Quantify-Scheduler"
 copyright = "2020-2022, Qblox & Orange Quantum Systems"
@@ -252,14 +252,15 @@
     # multiple targets for cross-references.
     # "imported-members",
 ]
 
 # avoid duplicate label warning even when manual label has been used;
 suppress_warnings = [
     "autosectionlabel.*",
+    "mystnb.unknown_mime_type",
 ]
 
 # avoid ugly very long module_a.module_b.module_c.module_d.module_e.module_d.MyClass
 # display in docs (very ugly when overflowing the html page width)
 # NB the side bar and the link of these objects already includes the full path
 add_module_names = False
 
@@ -334,16 +335,14 @@
 # member directly from a module, i.e.:
 
 # if typing.TYPE_CHECKING:
 #     from my_expensive_to_import_module import BlaClass # Potential circular import
 
 set_type_checking_flag = True  # this will run `typing.TYPE_CHECKING = True`
 
-notebook_to_jupyter_sphinx_always_rebuild = True
-
 # Enable nitpicky mode - warns about all references where the target cannot be found
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#confval-nitpicky
 
 nitpicky = True  # equivalent to `-n` option in the docs Makefile
 nitpick_ignore = [
     ("py:class", "quantify_scheduler.device_under_test.composite_square_edge"),
     (
@@ -368,14 +367,15 @@
     ),
     ("py:class", "AcquisitionIndexing"),
     ("py:obj", "quantify_scheduler.Operation"),
     ("py:class", "quantify_scheduler.Operation"),
     ("py:obj", "quantify_scheduler.Resource"),
     ("py:class", "quantify_scheduler.Resource"),
     ("py:obj", "quantify_scheduler.structure.DataStructure"),
+    ("py:obj", "quantify_scheduler.backends.SerialCompiler"),
 ]  # Tuple[str, str], ignore certain warnings
 
 nitpick_ignore_regex = [
     ("py:class", r"numpy.*"),
     ("py:class", r"plotly.*"),
     ("py:.*", r"orjson.*"),
     ("py:.*", r"pydantic.*"),
```

### Comparing `quantify-scheduler-0.8.0/docs/images/Chevron_experiment_comb.png` & `quantify-scheduler-0.9.0/docs/images/Chevron_experiment_comb.png`

 * *Files identical despite different names*

### Comparing `quantify-scheduler-0.8.0/docs/images/QUANTIFY-FAVICON_16.png` & `quantify-scheduler-0.9.0/docs/_build/html/_static/QUANTIFY-FAVICON_16.png`

 * *Files identical despite different names*

### Comparing `quantify-scheduler-0.8.0/docs/images/bell_circuit_QI.png` & `quantify-scheduler-0.9.0/docs/images/bell_circuit_QI.png`

 * *Files identical despite different names*

### Comparing `quantify-scheduler-0.8.0/docs/installation.rst` & `quantify-scheduler-0.9.0/docs/installation.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,119 +1,107 @@
-00000000: 2e2e 2068 6967 686c 6967 6874 3a3a 2073  .. highlight:: s
-00000010: 6865 6c6c 0a0a 3d3d 3d3d 3d3d 3d3d 3d3d  hell..==========
-00000020: 3d3d 0a49 6e73 7461 6c6c 6174 696f 6e0a  ==.Installation.
-00000030: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 0a0a 5374  ============..St
-00000040: 6162 6c65 2072 656c 6561 7365 0a2d 2d2d  able release.---
-00000050: 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 0a54 6f20  -----------..To 
-00000060: 696e 7374 616c 6c20 5175 616e 7469 6679  install Quantify
-00000070: 2d53 6368 6564 756c 6572 2066 6f6c 6c6f  -Scheduler follo
-00000080: 7720 7468 6520 3a64 6f63 3a60 696e 7374  w the :doc:`inst
-00000090: 616c 6c61 7469 6f6e 2067 7569 6465 206f  allation guide o
-000000a0: 6620 7175 616e 7469 6679 2d63 6f72 6520  f quantify-core 
-000000b0: 3c71 7561 6e74 6966 792d 636f 7265 3a69  <quantify-core:i
-000000c0: 6e73 7461 6c6c 6174 696f 6e3e 602e 0a0a  nstallation>`...
-000000d0: 5570 6461 7465 2074 6f20 6c61 7465 7374  Update to latest
-000000e0: 2076 6572 7369 6f6e 0a2d 2d2d 2d2d 2d2d   version.-------
-000000f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000100: 2d0a 0a54 6f20 7570 6461 7465 2074 6f20  -..To update to 
-00000110: 7468 6520 6c61 7465 7374 2076 6572 7369  the latest versi
-00000120: 6f6e 0a0a 2e2e 2063 6f64 652d 626c 6f63  on.... code-bloc
-00000130: 6b3a 3a20 636f 6e73 6f6c 650a 0a20 2020  k:: console..   
-00000140: 2024 2070 6970 2069 6e73 7461 6c6c 202d   $ pip install -
-00000150: 2d75 7067 7261 6465 2071 7561 6e74 6966  -upgrade quantif
-00000160: 792d 7363 6865 6475 6c65 720a 0a46 726f  y-scheduler..Fro
-00000170: 6d20 736f 7572 6365 730a 2d2d 2d2d 2d2d  m sources.------
-00000180: 2d2d 2d2d 2d2d 0a0a 5468 6520 736f 7572  ------..The sour
-00000190: 6365 7320 666f 7220 6060 7175 616e 7469  ces for ``quanti
-000001a0: 6679 2d73 6368 6564 756c 6572 6060 2063  fy-scheduler`` c
-000001b0: 616e 2062 6520 646f 776e 6c6f 6164 6564  an be downloaded
-000001c0: 2066 726f 6d20 7468 6520 6047 6974 4c61   from the `GitLa
-000001d0: 6220 7265 706f 203c 6874 7470 733a 2f2f  b repo <https://
-000001e0: 6769 746c 6162 2e63 6f6d 2f71 7561 6e74  gitlab.com/quant
-000001f0: 6966 792d 6f73 2f71 7561 6e74 6966 792d  ify-os/quantify-
-00000200: 7363 6865 6475 6c65 723e 605f 2e0a 0a59  scheduler>`_...Y
-00000210: 6f75 2063 616e 2063 6c6f 6e65 2074 6865  ou can clone the
-00000220: 2070 7562 6c69 6320 7265 706f 7369 746f   public reposito
-00000230: 7279 3a0a 0a2e 2e20 636f 6465 2d62 6c6f  ry:.... code-blo
-00000240: 636b 3a3a 2063 6f6e 736f 6c65 0a0a 2020  ck:: console..  
-00000250: 2020 2420 6769 7420 636c 6f6e 6520 6769    $ git clone gi
-00000260: 7440 6769 746c 6162 2e63 6f6d 3a71 7561  t@gitlab.com:qua
-00000270: 6e74 6966 792d 6f73 2f71 7561 6e74 6966  ntify-os/quantif
-00000280: 792d 7363 6865 6475 6c65 722e 6769 740a  y-scheduler.git.
-00000290: 2020 2020 2420 2320 6f72 2069 6620 796f      $ # or if yo
-000002a0: 7520 7072 6566 6572 2074 6f20 7573 6520  u prefer to use 
-000002b0: 6874 7470 733a 0a20 2020 2024 2023 2067  https:.    $ # g
-000002c0: 6974 2063 6c6f 6e65 2068 7474 7073 3a2f  it clone https:/
-000002d0: 2f67 6974 6c61 622e 636f 6d2f 7175 616e  /gitlab.com/quan
-000002e0: 7469 6679 2d6f 732f 7175 616e 7469 6679  tify-os/quantify
-000002f0: 2d73 6368 6564 756c 6572 2e67 6974 2f0a  -scheduler.git/.
-00000300: 0a4f 6e63 6520 796f 7520 6861 7665 2061  .Once you have a
-00000310: 2063 6f70 7920 6f66 2074 6865 2073 6f75   copy of the sou
-00000320: 7263 652c 2079 6f75 2063 616e 2069 6e73  rce, you can ins
-00000330: 7461 6c6c 2069 7420 7769 7468 3a0a 0a2e  tall it with:...
-00000340: 2e20 636f 6465 2d62 6c6f 636b 3a3a 2063  . code-block:: c
-00000350: 6f6e 736f 6c65 0a0a 2020 2020 2420 7079  onsole..    $ py
-00000360: 7468 6f6e 202d 6d20 7069 7020 696e 7374  thon -m pip inst
-00000370: 616c 6c20 2d2d 7570 6772 6164 6520 2e0a  all --upgrade ..
-00000380: 0a49 6e20 6f72 6465 7220 746f 2064 6576  .In order to dev
-00000390: 656c 6f70 2074 6865 2063 6f64 6520 6c6f  elop the code lo
-000003a0: 6361 6c6c 792c 2074 6865 2070 6163 6b61  cally, the packa
-000003b0: 6765 2063 616e 2062 6520 696e 7374 616c  ge can be instal
-000003c0: 6c65 6420 696e 2074 6865 2022 6564 6974  led in the "edit
-000003d0: 6162 6c65 206d 6f64 6522 2077 6974 6820  able mode" with 
-000003e0: 7468 6520 6060 2d65 6060 2066 6c61 673a  the ``-e`` flag:
-000003f0: 0a0a 2e2e 2063 6f64 652d 626c 6f63 6b3a  .... code-block:
-00000400: 3a20 636f 6e73 6f6c 650a 0a20 2020 2024  : console..    $
-00000410: 2070 7974 686f 6e20 2d6d 2070 6970 2069   python -m pip i
-00000420: 6e73 7461 6c6c 202d 2d75 7067 7261 6465  nstall --upgrade
-00000430: 202d 6520 2e0a 0a53 6574 7469 6e67 2075   -e ...Setting u
-00000440: 7020 666f 7220 6c6f 6361 6c20 6465 7665  p for local deve
-00000450: 6c6f 706d 656e 740a 2d2d 2d2d 2d2d 2d2d  lopment.--------
-00000460: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000470: 2d2d 2d2d 2d2d 2d2d 0a0a 436f 6e74 7269  --------..Contri
-00000480: 6275 7469 6f6e 7320 6172 6520 7665 7279  butions are very
-00000490: 2077 656c 636f 6d65 2120 546f 2073 6574   welcome! To set
-000004a0: 7570 2061 2061 6e20 656e 7669 726f 6e6d  up a an environm
-000004b0: 656e 7420 666f 7220 6c6f 6361 6c20 6465  ent for local de
-000004c0: 7665 6c6f 706d 656e 7420 7365 6520 7468  velopment see th
-000004d0: 6520 696e 7374 7275 6374 696f 6e73 2069  e instructions i
-000004e0: 6e20 7468 6520 3a64 6f63 3a60 696e 7374  n the :doc:`inst
-000004f0: 616c 6c61 7469 6f6e 2067 7569 6465 206f  allation guide o
-00000500: 6620 7175 616e 7469 6679 2d63 6f72 6520  f quantify-core 
-00000510: 3c71 7561 6e74 6966 792d 636f 7265 3a69  <quantify-core:i
-00000520: 6e73 7461 6c6c 6174 696f 6e3e 602e 2059  nstallation>`. Y
-00000530: 6f75 206f 6e6c 7920 6e65 6564 2074 6f20  ou only need to 
-00000540: 7265 706c 6163 6520 3a63 6f64 653a 6071  replace :code:`q
-00000550: 7561 6e74 6966 792d 636f 7265 6020 7769  uantify-core` wi
-00000560: 7468 203a 636f 6465 3a60 7175 616e 7469  th :code:`quanti
-00000570: 6679 2d73 6368 6564 756c 6572 6020 696e  fy-scheduler` in
-00000580: 2074 6865 2070 726f 7669 6465 6420 636f   the provided co
-00000590: 6d6d 616e 6473 2e0a 0a49 6620 796f 7520  mmands...If you 
-000005a0: 6e65 6564 2061 6e79 2068 656c 7020 7265  need any help re
-000005b0: 6163 6820 6f75 7420 746f 2075 7320 6279  ach out to us by
-000005c0: 2060 6372 6561 7469 6e67 2061 206e 6577   `creating a new
-000005d0: 2069 7373 7565 203c 6874 7470 733a 2f2f   issue <https://
-000005e0: 6769 746c 6162 2e63 6f6d 2f71 7561 6e74  gitlab.com/quant
-000005f0: 6966 792d 6f73 2f71 7561 6e74 6966 792d  ify-os/quantify-
-00000600: 7363 6865 6475 6c65 722f 2d2f 6973 7375  scheduler/-/issu
-00000610: 6573 3e60 5f2e 0a0a 0a4a 7570 7974 6572  es>`_....Jupyter
-00000620: 2061 6e64 2070 6c6f 746c 790a 2d2d 2d2d   and plotly.----
-00000630: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a  ---------------.
-00000640: 0a51 7561 6e74 6966 792d 7363 6865 6475  .Quantify-schedu
-00000650: 6c65 7220 7573 6573 2074 6865 2060 706c  ler uses the `pl
-00000660: 6f74 7960 5f20 6772 6170 6869 6e67 2066  oty`_ graphing f
-00000670: 7261 6d65 776f 726b 2066 6f72 2073 6f6d  ramework for som
-00000680: 6520 636f 6d70 6f6e 656e 7473 2c20 7768  e components, wh
-00000690: 6963 6820 6361 6e20 7265 7175 6972 6520  ich can require 
-000006a0: 736f 6d65 2061 6464 6974 696f 6e61 6c20  some additional 
-000006b0: 7365 742d 7570 0a74 6f20 7275 6e20 7769  set-up.to run wi
-000006c0: 7468 2061 204a 7570 7974 6572 2065 6e76  th a Jupyter env
-000006d0: 6972 6f6e 6d65 6e74 202d 2070 6c65 6173  ironment - pleas
-000006e0: 6520 7365 6520 6074 6869 7320 7061 6765  e see `this page
-000006f0: 2066 6f72 2064 6574 6169 6c73 2e60 5f0a   for details.`_.
-00000700: 0a0a 2e2e 205f 706c 6f74 793a 2068 7474  .... _ploty: htt
-00000710: 7073 3a2f 2f70 6c6f 746c 792e 636f 6d2f  ps://plotly.com/
-00000720: 0a2e 2e20 5f74 6869 7320 7061 6765 2066  ... _this page f
-00000730: 6f72 2064 6574 6169 6c73 2e3a 2068 7474  or details.: htt
-00000740: 7073 3a2f 2f70 6c6f 746c 792e 636f 6d2f  ps://plotly.com/
-00000750: 7079 7468 6f6e 2f67 6574 7469 6e67 2d73  python/getting-s
-00000760: 7461 7274 6564 2f0a                      tarted/.
+00000000: 6060 607b 6869 6768 6c69 6768 747d 2073  ```{highlight} s
+00000010: 6865 6c6c 0a60 6060 0a0a 2320 496e 7374  hell.```..# Inst
+00000020: 616c 6c61 7469 6f6e 0a0a 2323 2053 7461  allation..## Sta
+00000030: 626c 6520 7265 6c65 6173 650a 0a54 6f20  ble release..To 
+00000040: 696e 7374 616c 6c20 5175 616e 7469 6679  install Quantify
+00000050: 2d53 6368 6564 756c 6572 2066 6f6c 6c6f  -Scheduler follo
+00000060: 7720 7468 6520 7b64 6f63 7d60 696e 7374  w the {doc}`inst
+00000070: 616c 6c61 7469 6f6e 2067 7569 6465 206f  allation guide o
+00000080: 6620 7175 616e 7469 6679 2d63 6f72 6520  f quantify-core 
+00000090: 3c71 7561 6e74 6966 792d 636f 7265 3a69  <quantify-core:i
+000000a0: 6e73 7461 6c6c 6174 696f 6e3e 602e 0a0a  nstallation>`...
+000000b0: 2323 2055 7064 6174 6520 746f 206c 6174  ## Update to lat
+000000c0: 6573 7420 7665 7273 696f 6e0a 0a54 6f20  est version..To 
+000000d0: 7570 6461 7465 2074 6f20 7468 6520 6c61  update to the la
+000000e0: 7465 7374 2076 6572 7369 6f6e 0a0a 6060  test version..``
+000000f0: 6063 6f6e 736f 6c65 0a24 2070 6970 2069  `console.$ pip i
+00000100: 6e73 7461 6c6c 202d 2d75 7067 7261 6465  nstall --upgrade
+00000110: 2071 7561 6e74 6966 792d 7363 6865 6475   quantify-schedu
+00000120: 6c65 720a 6060 600a 0a23 2320 4672 6f6d  ler.```..## From
+00000130: 2073 6f75 7263 6573 0a0a 5468 6520 736f   sources..The so
+00000140: 7572 6365 7320 666f 7220 6071 7561 6e74  urces for `quant
+00000150: 6966 792d 7363 6865 6475 6c65 7260 2063  ify-scheduler` c
+00000160: 616e 2062 6520 646f 776e 6c6f 6164 6564  an be downloaded
+00000170: 2066 726f 6d20 7468 6520 5b47 6974 4c61   from the [GitLa
+00000180: 6220 7265 706f 5d28 6874 7470 733a 2f2f  b repo](https://
+00000190: 6769 746c 6162 2e63 6f6d 2f71 7561 6e74  gitlab.com/quant
+000001a0: 6966 792d 6f73 2f71 7561 6e74 6966 792d  ify-os/quantify-
+000001b0: 7363 6865 6475 6c65 7229 2e0a 0a59 6f75  scheduler)...You
+000001c0: 2063 616e 2063 6c6f 6e65 2074 6865 2070   can clone the p
+000001d0: 7562 6c69 6320 7265 706f 7369 746f 7279  ublic repository
+000001e0: 3a0a 0a60 6060 636f 6e73 6f6c 650a 2420  :..```console.$ 
+000001f0: 6769 7420 636c 6f6e 6520 6769 7440 6769  git clone git@gi
+00000200: 746c 6162 2e63 6f6d 3a71 7561 6e74 6966  tlab.com:quantif
+00000210: 792d 6f73 2f71 7561 6e74 6966 792d 7363  y-os/quantify-sc
+00000220: 6865 6475 6c65 722e 6769 740a 2420 2320  heduler.git.$ # 
+00000230: 6f72 2069 6620 796f 7520 7072 6566 6572  or if you prefer
+00000240: 2074 6f20 7573 6520 6874 7470 733a 0a24   to use https:.$
+00000250: 2023 2067 6974 2063 6c6f 6e65 2068 7474   # git clone htt
+00000260: 7073 3a2f 2f67 6974 6c61 622e 636f 6d2f  ps://gitlab.com/
+00000270: 7175 616e 7469 6679 2d6f 732f 7175 616e  quantify-os/quan
+00000280: 7469 6679 2d73 6368 6564 756c 6572 2e67  tify-scheduler.g
+00000290: 6974 2f0a 6060 600a 0a4f 6e63 6520 796f  it/.```..Once yo
+000002a0: 7520 6861 7665 2061 2063 6f70 7920 6f66  u have a copy of
+000002b0: 2074 6865 2073 6f75 7263 652c 2079 6f75   the source, you
+000002c0: 2063 616e 2069 6e73 7461 6c6c 2069 7420   can install it 
+000002d0: 7769 7468 3a0a 0a60 6060 636f 6e73 6f6c  with:..```consol
+000002e0: 650a 2420 7079 7468 6f6e 202d 6d20 7069  e.$ python -m pi
+000002f0: 7020 696e 7374 616c 6c20 2d2d 7570 6772  p install --upgr
+00000300: 6164 6520 2e0a 6060 600a 0a49 6e20 6f72  ade ..```..In or
+00000310: 6465 7220 746f 2064 6576 656c 6f70 2074  der to develop t
+00000320: 6865 2063 6f64 6520 6c6f 6361 6c6c 792c  he code locally,
+00000330: 2074 6865 2070 6163 6b61 6765 2063 616e   the package can
+00000340: 2062 6520 696e 7374 616c 6c65 6420 696e   be installed in
+00000350: 2074 6865 2022 6564 6974 6162 6c65 206d   the "editable m
+00000360: 6f64 6522 2077 6974 6820 7468 6520 602d  ode" with the `-
+00000370: 6560 2066 6c61 673a 0a0a 6060 6063 6f6e  e` flag:..```con
+00000380: 736f 6c65 0a24 2070 7974 686f 6e20 2d6d  sole.$ python -m
+00000390: 2070 6970 2069 6e73 7461 6c6c 202d 2d75   pip install --u
+000003a0: 7067 7261 6465 202d 6520 2e0a 6060 600a  pgrade -e ..```.
+000003b0: 0a23 2320 5365 7474 696e 6720 7570 2066  .## Setting up f
+000003c0: 6f72 206c 6f63 616c 2064 6576 656c 6f70  or local develop
+000003d0: 6d65 6e74 0a0a 436f 6e74 7269 6275 7469  ment..Contributi
+000003e0: 6f6e 7320 6172 6520 7665 7279 2077 656c  ons are very wel
+000003f0: 636f 6d65 2120 546f 2073 6574 7570 2061  come! To setup a
+00000400: 2061 6e20 656e 7669 726f 6e6d 656e 7420   an environment 
+00000410: 666f 7220 6c6f 6361 6c20 6465 7665 6c6f  for local develo
+00000420: 706d 656e 7420 7365 6520 7468 6520 696e  pment see the in
+00000430: 7374 7275 6374 696f 6e73 2069 6e20 7468  structions in th
+00000440: 6520 7b64 6f63 7d60 696e 7374 616c 6c61  e {doc}`installa
+00000450: 7469 6f6e 2067 7569 6465 206f 6620 7175  tion guide of qu
+00000460: 616e 7469 6679 2d63 6f72 6520 3c71 7561  antify-core <qua
+00000470: 6e74 6966 792d 636f 7265 3a69 6e73 7461  ntify-core:insta
+00000480: 6c6c 6174 696f 6e3e 602e 2059 6f75 206f  llation>`. You o
+00000490: 6e6c 7920 6e65 6564 2074 6f20 7265 706c  nly need to repl
+000004a0: 6163 6520 7b63 6f64 657d 6071 7561 6e74  ace {code}`quant
+000004b0: 6966 792d 636f 7265 6020 7769 7468 207b  ify-core` with {
+000004c0: 636f 6465 7d60 7175 616e 7469 6679 2d73  code}`quantify-s
+000004d0: 6368 6564 756c 6572 6020 696e 2074 6865  cheduler` in the
+000004e0: 2070 726f 7669 6465 6420 636f 6d6d 616e   provided comman
+000004f0: 6473 2e0a 0a49 6620 796f 7520 6e65 6564  ds...If you need
+00000500: 2061 6e79 2068 656c 7020 7265 6163 6820   any help reach 
+00000510: 6f75 7420 746f 2075 7320 6279 205b 6372  out to us by [cr
+00000520: 6561 7469 6e67 2061 206e 6577 2069 7373  eating a new iss
+00000530: 7565 5d28 6874 7470 733a 2f2f 6769 746c  ue](https://gitl
+00000540: 6162 2e63 6f6d 2f71 7561 6e74 6966 792d  ab.com/quantify-
+00000550: 6f73 2f71 7561 6e74 6966 792d 7363 6865  os/quantify-sche
+00000560: 6475 6c65 722f 2d2f 6973 7375 6573 292e  duler/-/issues).
+00000570: 0a0a 2323 204a 7570 7974 6572 2061 6e64  ..## Jupyter and
+00000580: 2070 6c6f 746c 790a 0a51 7561 6e74 6966   plotly..Quantif
+00000590: 792d 7363 6865 6475 6c65 7220 7573 6573  y-scheduler uses
+000005a0: 2074 6865 205b 706c 6f74 795d 2067 7261   the [ploty] gra
+000005b0: 7068 696e 6720 6672 616d 6577 6f72 6b20  phing framework 
+000005c0: 666f 7220 736f 6d65 2063 6f6d 706f 6e65  for some compone
+000005d0: 6e74 732c 2077 6869 6368 2063 616e 2072  nts, which can r
+000005e0: 6571 7569 7265 2073 6f6d 6520 6164 6469  equire some addi
+000005f0: 7469 6f6e 616c 2073 6574 2d75 700a 746f  tional set-up.to
+00000600: 2072 756e 2077 6974 6820 6120 4a75 7079   run with a Jupy
+00000610: 7465 7220 656e 7669 726f 6e6d 656e 7420  ter environment 
+00000620: 2d20 706c 6561 7365 2073 6565 205b 7468  - please see [th
+00000630: 6973 2070 6167 6520 666f 7220 6465 7461  is page for deta
+00000640: 696c 732e 5d0a 0a5b 706c 6f74 795d 3a20  ils.]..[ploty]: 
+00000650: 6874 7470 733a 2f2f 706c 6f74 6c79 2e63  https://plotly.c
+00000660: 6f6d 2f0a 5b74 6869 7320 7061 6765 2066  om/.[this page f
+00000670: 6f72 2064 6574 6169 6c73 2e5d 3a20 6874  or details.]: ht
+00000680: 7470 733a 2f2f 706c 6f74 6c79 2e63 6f6d  tps://plotly.com
+00000690: 2f70 7974 686f 6e2f 6765 7474 696e 672d  /python/getting-
+000006a0: 7374 6172 7465 642f 0a                   started/.
```

### Comparing `quantify-scheduler-0.8.0/docs/make.bat` & `quantify-scheduler-0.9.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `quantify-scheduler-0.8.0/docs/tutorials/qblox/Cluster.rst` & `quantify-scheduler-0.9.0/docs/tutorials/qblox/Cluster.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,91 +1,108 @@
-.. _sec-qblox-cluster:
-
-Cluster
-=======
-
-.. jupyter-execute::
-    :hide-code:
-
-    # in the hidden cells we include some code that checks for correctness of the examples
-    from tempfile import TemporaryDirectory
-
-    from quantify_scheduler import Schedule
-    from quantify_scheduler.operations import pulse_library
-    from quantify_scheduler.compilation import determine_absolute_timing
-    from quantify_scheduler.backends.qblox_backend import hardware_compile
-    from quantify_scheduler.resources import ClockResource
-
-    from quantify_core.data.handling import set_datadir
-
-    temp_dir = TemporaryDirectory()
-    set_datadir(temp_dir.name)
-
-In the previous sections we explained how to configure the backend for use with the standalone `Pulsars <https://www.qblox.com/pulsar>`_, now we will explain how to adapt this config
-to use one or multiple `Clusters <https://www.qblox.com/cluster>`_ instead.
-Since the cluster modules behave similarly, we recommend first familiarizing yourself with the configuration for the :doc:`pulsars <Pulsar>`.
+---
+file_format: mystnb
+kernelspec:
+    name: python3
+
+---
+(sec-qblox-cluster)=
+
+# Cluster
+
+```{code-cell} ipython3
+---
+mystnb:
+  remove_code_source: true
+---
+
+# in the hidden cells we include some code that checks for correctness of the examples
+from tempfile import TemporaryDirectory
+
+from quantify_scheduler import Schedule
+from quantify_scheduler.operations import pulse_library
+from quantify_scheduler.compilation import determine_absolute_timing
+from quantify_scheduler.backends.qblox_backend import hardware_compile
+from quantify_scheduler.resources import ClockResource
+
+from quantify_core.data.handling import set_datadir
+
+temp_dir = TemporaryDirectory()
+set_datadir(temp_dir.name)
+```
+
+In the previous sections we explained how to configure the backend for use with the standalone [Pulsars](https://www.qblox.com/pulsar), now we will explain how to adapt this config
+to use one or multiple [Clusters](https://www.qblox.com/cluster) instead.
+Since the cluster modules behave similarly, we recommend first familiarizing yourself with the configuration for the {doc}`pulsars <Pulsar>`.
 
 We start by looking at an example config for a single cluster:
 
-.. jupyter-execute::
-    :hide-output:
-    :linenos:
-
-    mapping_config = {
-        "backend": "quantify_scheduler.backends.qblox_backend.hardware_compile",
-        "cluster0": {
-            "cluster0_module1": {
-                "complex_output_0": {
-                    "lo_name": "lo0",
-                    "portclock_configs": [
-                        {
-                            "clock": "q4.01",
-                            "interm_freq": 200000000.0,
-                            "mixer_amp_ratio": 0.9999,
-                            "mixer_phase_error_deg": -4.2,
-                            "port": "q4:mw",
-                        },
-                    ]
-                },
-                "instrument_type": "QCM",
+```{code-cell} ipython3
+---
+mystnb:
+  number_source_lines: true
+  remove_code_outputs: true
+---
+
+mapping_config = {
+    "backend": "quantify_scheduler.backends.qblox_backend.hardware_compile",
+    "cluster0": {
+        "cluster0_module1": {
+            "complex_output_0": {
+                "lo_name": "lo0",
+                "portclock_configs": [
+                    {
+                        "clock": "q4.01",
+                        "interm_freq": 200000000.0,
+                        "mixer_amp_ratio": 0.9999,
+                        "mixer_phase_error_deg": -4.2,
+                        "port": "q4:mw",
+                    },
+                ]
             },
-            "cluster0_module2": {
-                "complex_output_0": {
-                    "portclock_configs": [
-                        {
-                            "clock": "q5.01",
-                            "interm_freq": 50000000.0,
-                            "port": "q5:mw"
-                        }
-                    ]
-                },
-                "instrument_type": "QCM_RF",
+            "instrument_type": "QCM",
+        },
+        "cluster0_module2": {
+            "complex_output_0": {
+                "portclock_configs": [
+                    {
+                        "clock": "q5.01",
+                        "interm_freq": 50000000.0,
+                        "port": "q5:mw"
+                    }
+                ]
             },
-            "instrument_type": "Cluster",
-            "ref": "internal",
+            "instrument_type": "QCM_RF",
         },
-        "lo0": {"instrument_type": "LocalOscillator", "frequency": None, "power": 20},
-    }
-
-.. jupyter-execute::
-    :hide-code:
-    :hide-output:
-
-    # Validate mapping_config
-
-    test_sched = Schedule("test_sched")
-    test_sched.add(
-        pulse_library.SquarePulse(amp=1, duration=1e-6, port="q4:mw", clock="q4.01")
-    )
-    test_sched.add(
-        pulse_library.SquarePulse(amp=0.25, duration=1e-6, port="q5:mw", clock="q5.01")
-    )
-    test_sched.add_resource(ClockResource(name="q4.01", freq=7e9))
-    test_sched.add_resource(ClockResource(name="q5.01", freq=8e9))
-    test_sched = determine_absolute_timing(test_sched)
+        "instrument_type": "Cluster",
+        "ref": "internal",
+    },
+    "lo0": {"instrument_type": "LocalOscillator", "frequency": None, "power": 20},
+}
+```
+
+```{code-cell} ipython3
+---
+mystnb:
+  remove_code_source: true
+  remove_code_outputs: true
+---
+
+# Validate mapping_config
+
+test_sched = Schedule("test_sched")
+test_sched.add(
+    pulse_library.SquarePulse(amp=1, duration=1e-6, port="q4:mw", clock="q4.01")
+)
+test_sched.add(
+    pulse_library.SquarePulse(amp=0.25, duration=1e-6, port="q5:mw", clock="q5.01")
+)
+test_sched.add_resource(ClockResource(name="q4.01", freq=7e9))
+test_sched.add_resource(ClockResource(name="q5.01", freq=8e9))
+test_sched = determine_absolute_timing(test_sched)
 
-    hardware_compile(test_sched, mapping_config)
+hardware_compile(test_sched, mapping_config)
+```
 
-In the example, we notice that the cluster is specified using an instrument with :code:`"instrument_type": "Cluster"`. In the backend, the cluster instrument functions as a collection of
-modules. The modules themselves can be configured identically to pulsars, except for the :code:`ref`, which has now become a cluster wide setting.
+In the example, we notice that the cluster is specified using an instrument with {code}`"instrument_type": "Cluster"`. In the backend, the cluster instrument functions as a collection of
+modules. The modules themselves can be configured identically to pulsars, except for the {code}`ref`, which has now become a cluster wide setting.
 
-Valid values for :code:`"instrument_type"` for the modules are: :code:`QCM`, :code:`QRM`, :code:`QCM_RF` and :code:`QRM_RF`.
+Valid values for {code}`"instrument_type"` for the modules are: {code}`QCM`, {code}`QRM`, {code}`QCM_RF` and {code}`QRM_RF`.
```

### Comparing `quantify-scheduler-0.8.0/docs/tutorials/qblox/index.rst` & `quantify-scheduler-0.9.0/docs/tutorials/qblox/index.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,20 @@
-.. _sec-backend-qblox:
+(sec-backend-qblox)=
 
-Backend: Qblox
-==============
+# Backend: Qblox
 
-.. warning::
-    The :mod:`quantify_scheduler.backends.qblox_backend` is still under development.
-    Breaking changes at this stage are not excluded.
+```{warning}
+The {mod}`quantify_scheduler.backends.qblox_backend` is still under development.
+Breaking changes at this stage are not excluded.
+```
 
+## Introduction
 
-Introduction
-^^^^^^^^^^^^
-
-:mod:`quantify_scheduler` provides a modular system: :mod:`~quantify_scheduler.backends.qblox_backend`,
-that abstracts the full experimental setup using `Qblox <https://www.qblox.com>`_ hardware for
+{mod}`quantify_scheduler` provides a modular system: {mod}`~quantify_scheduler.backends.qblox_backend`,
+that abstracts the full experimental setup using [Qblox](https://www.qblox.com) hardware for
 experiments in a modern and automated fashion.
 
 Functionality included in this backend:
 
 - Full compilation of the schedule to a program for the sequencer.
 - Waveform generation and modulation, in a parameterized fashion as supported by Qblox hardware.
 - Built-in version handling to ensure the backend works correctly with the installed driver version.
@@ -24,42 +22,40 @@
 - Calculation of the optimal hardware settings for execution of the provided schedule using the Instrument Coordinator.
 - Real mode, which allows to address the individual outputs separately rather than using IQ signals.
 - Full support of frequency multiplexing.
 - Automatic calculation of the required parameters for external local oscillators.
 - Correction of the mixer errors using specified correction parameters.
 - Flexible configuration via JSON data structures.
 
-No special configuration is required to use this backend. Simply specify :obj:`quantify_scheduler.backends.qblox_backend.hardware_compile`
-in the hardware configuration to use this backend or call the function directly. Please see :ref:`Usage of the backend <sec-qblox-how-to-configure>`
+No special configuration is required to use this backend. Simply specify {obj}`quantify_scheduler.backends.qblox_backend.hardware_compile`
+in the hardware configuration to use this backend or call the function directly. Please see {ref}`Usage of the backend <sec-qblox-how-to-configure>`
 for information on how to set this up.
 After a schedule is compiled into a program, uploading to the hardware can be done using the usual
-`qblox-instruments <https://pypi.org/project/qblox-instruments/>`_ drivers. Installation of these drivers
+[qblox-instruments](https://pypi.org/project/qblox-instruments/) drivers. Installation of these drivers
 is done through
 
-.. code-block:: console
-
-    $ pip install qblox-instruments
+```console
+$ pip install qblox-instruments
+```
 
-Please visit the `Qblox instruments documentation <https://qblox-qblox-instruments.readthedocs-hosted.com>`_
+Please visit the [Qblox instruments documentation](https://qblox-qblox-instruments.readthedocs-hosted.com)
 for more information.
 
-Supported Instruments
-^^^^^^^^^^^^^^^^^^^^^
+## Supported Instruments
 
 - ✅ QCM
 - ✅ QRM
 - ✅ QCM-RF
 - ✅ QRM-RF
 - ✅ Cluster
 - ⬜️ SPI
 
+## How to use
 
-How to use
-^^^^^^^^^^^^^^^^^^^^^
+```{toctree}
+:maxdepth: 2
 
-.. toctree::
-    :maxdepth: 2
-
-    recent
-    How to use
-    Pulsar
-    Cluster
+recent
+How to use
+Pulsar
+Cluster
+```
```

### Comparing `quantify-scheduler-0.8.0/docs/tutorials/qblox/recent.rst` & `quantify-scheduler-0.9.0/docs/tutorials/qblox/recent.rst`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,37 @@
 Recent interface changes
 ========================
 
+Unreleased: Setting input/output gain and attenuation parameters
+----------------------------------------------------------------
+
+This change makes quantify-scheduler be able to set input/output gain/attenuation parameters through the hardware configuration for Qblox hardware.
+Note, that not every combination of input/output gain/attenuation 0/1 is possible.
+The following parameters are possible for each device type.
+
+- QRM (baseband)
+
+  - ``input_gain_I`` (for ``complex_output_0``) or ``input_gain`` (for ``real_output_0``)
+
+  - ``input_gain_Q`` (for ``complex_output_0``) or ``input_gain`` (for ``real_output_1``)
+
+- QRM-RF
+
+  - ``output_att`` (for ``complex_output_0``)
+
+  - ``input_att`` (for ``complex_output_0``)
+
+- QCM-RF
+
+  - ``output_att`` (for ``complex_output_0``)
+
+  - ``output_att`` (for ``complex_output_1``)
+
+See ``quantify_scheduler/schemas/examples/qblox_test_mapping.json`` for concrete examples (see :ref:`sec-qblox-how-to-configure`).
+
 0.8.0: Dynamic Sequencer Allocation
 -----------------------------------
 
 The Qblox backend now dynamically allocates sequencers to port-clock combinations as required.
 This enables the user to target an arbitrary number of port-clock combinations using the same module, as long as they are not being *simultaneously* targeted.
 Given that Qblox instruments have 6 sequencers, up to 6 port-clock combinations may be simultaneously targeted.
```

### Comparing `quantify-scheduler-0.8.0/docs/tutorials/zhinst/index.rst` & `quantify-scheduler-0.9.0/docs/tutorials/zhinst/index.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,275 +1,258 @@
-.. _sec-backend-zhinst:
+(sec-backend-zhinst)=
 
-Backend: Zurich Instruments
-===========================
+# Backend: Zurich Instruments
 
+## Introduction
 
-Introduction
-^^^^^^^^^^^^
+{mod}`quantify_scheduler` provides a stateless module: {mod}`~quantify_scheduler.backends.zhinst_backend`,
+that abstracts the complexity of setting up experiments using [Zurich Instruments](https://www.zhinst.com) hardware.
+{mod}`quantify_scheduler` uses information on the quantum device
+and instrument properties to compile a {class}`quantify_scheduler.schedules.schedule.Schedule` into waveforms and sequencing instructions suitable for execution on Zurich Instruments hardware.
+More information about `compilation` can be found in the {ref}`User Guide <sec-user-guide>`.
 
-:mod:`quantify_scheduler` provides a stateless module: :mod:`~quantify_scheduler.backends.zhinst_backend`,
-that abstracts the complexity of setting up experiments using `Zurich Instruments <https://www.zhinst.com>`_ hardware.
-:mod:`quantify_scheduler` uses information on the quantum device
-and instrument properties to compile a :class:`quantify_scheduler.schedules.schedule.Schedule` into waveforms and sequencing instructions suitable for execution on Zurich Instruments hardware.
-More information about `compilation` can be found in the :ref:`User Guide <sec-user-guide>`.
+Using existing programming interfaces provided via {doc}`zhinst-qcodes <zhinst-qcodes:index>` and {doc}`zhinst-toolkit <zhinst-toolkit:index>`, {mod}`quantify_scheduler` prepares the instruments that are present in the {ref}`sec-hardware configuration file <Hardware configuration file>`.
 
-Using existing programming interfaces provided via :doc:`zhinst-qcodes <zhinst-qcodes:index>` and :doc:`zhinst-toolkit <zhinst-toolkit:index>`, :mod:`quantify_scheduler` prepares the instruments that are present in the :ref:`sec-hardware configuration file <Hardware configuration file>`.
-
-Finally, after configuring and running :func:`~quantify_scheduler.backends.zhinst_backend.compile_backend`
+Finally, after configuring and running {func}`~quantify_scheduler.backends.zhinst_backend.compile_backend`
 successfully the instruments are prepared for execution.
 
 The Zurich Instruments backend provides:
 
 - Synchronized execution of a program in a UHFQA and an HDAWG through the use of Triggers and Markers.
 - Automatic generation of the SeqC Sequencer instructions.
 - Waveform generation and modulation.
 - Memory-efficient Sequencing with the CommandTable.
 - Configuration of the relevant settings on all instruments.
 - Configuration for Triggers and Markers.
 
-Supported Instruments
-^^^^^^^^^^^^^^^^^^^^^
+## Supported Instruments
 
 The Zurich Instruments backend currently supports the **HDAWG** and the **UHFQA** instruments.
 In addition to the Zurich Instruments devices, the hardware backend supports using microwave sources such as the R&S SGS100A.
 
-Basic paradigm and inner workings
-^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+## Basic paradigm and inner workings
 
-The Zurich Instruments back end threats a :class:`~.Schedule` as a linear timeline of operations executed on the quantum device and translates this into pulses and acquisitions to be executed on the different input and output channels of an HDAWG and a UHFQA.
+The Zurich Instruments back end threats a {class}`~.Schedule` as a linear timeline of operations executed on the quantum device and translates this into pulses and acquisitions to be executed on the different input and output channels of an HDAWG and a UHFQA.
 In this context a single HDAWG is treated as the master device that sends out a single marker pulse for synchronization at the start of each iteration of the schedule that is used to trigger all other devices.
 After the synchronization trigger is given, all devices execute a compiled program for which the timings of all instructions have been calculated.
 
 The compilation from operations at the quantum-device layer to instructions that the hardware can execute is done in several steps.
-The zhinst :func:`~quantify_scheduler.backends.zhinst_backend.compile_backend` starts from the :attr:`.ScheduleBase.timing_table` and maps the operations to channels on the hardware using information specified in the
-:ref:`sec-hardware configuration file <hardware configuration file>`.
+The zhinst {func}`~quantify_scheduler.backends.zhinst_backend.compile_backend` starts from the {attr}`.ScheduleBase.timing_table` and maps the operations to channels on the hardware using information specified in the
+{ref}`sec-hardware configuration file <hardware configuration file>`.
 Corrections for channel latency, as well as moving operations around to ensure all measurements start at the first sample (0) of a clock cycle are also done at this stage.
 
 Once the starting time and sample of each operation is known, the numerical waveforms that have to be uploaded to the hardware can be generated.
 The numerical waveforms differ from the idealized waveforms of the device description in that the they include corrections for effects such as mixer-skewness and linear-dynamical distortions (not implemented yet), and intermediate frequency modulation if required.
 
-Both the :attr:`.CompiledSchedule.hardware_timing_table` and :attr:`.CompiledSchedule.hardware_waveform_dict` are available as properties of the :class:`.CompiledSchedule`.
+Both the {attr}`.CompiledSchedule.hardware_timing_table` and {attr}`.CompiledSchedule.hardware_waveform_dict` are available as properties of the {class}`.CompiledSchedule`.
 
 In the next step, the clock-accurate Seqc instructions for each awg of each device are determined, as well as the settings (nodes) to be configured including the linking of the numerical waveforms to these nodes.
-All of this information is combined in :class:`~.backends.zhinst.settings.ZISettingsBuilder`\s and added to the compiled instructions of the :class:`.CompiledSchedule`.
+All of this information is combined in {class}`~.backends.zhinst.settings.ZISettingsBuilder`s and added to the compiled instructions of the {class}`.CompiledSchedule`.
 
+## Limitations
 
-Limitations
-^^^^^^^^^^^
 There are several limitation to the paradigm and to the current implementation.
 Some of these are relatively easy to address while others are more fundamental to the paradigm.
 Here we give an overview of the known limitations.
 Note that some of these can be quite specific.
 
-Inherent limitations
-~~~~~~~~~~~~~~~~~~~~
+### Inherent limitations
+
 There are some inherent limitations to the paradigm of describing the program as a single linear timeline that is started using a single synchronization trigger.
 These limitations cannot easily be addressed so should be taken into account when thinking about experiments.
 
-
 - Because the **synchronization of the HDAWG and the UFHQA relies on a trigger on two devices operating at different clock frequencies** one cannot guarantee at what sample within the clock domain the slave device gets triggered. The consequence is that although the triggering is stable within an experiment, the exact time difference (in number of samples) between the different devices varies between different experiments. This problem is inherent to the triggering scheme and cannot be easily resolved.
 - The paradigm of a single fixed timeline with a single synchronizing trigger is **not compatible with control loop affecting feedback**.
 
-Limitations with the current implementation
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+### Limitations with the current implementation
+
 There are also some practical limitations to the implementation.
 Keep these in mind when operating the hardware.
 
 - **Real-time modulation is currently not supported**, relying on pre-modulated waveforms, it is important to start waveforms at a multiple of the modulation frequency. Sticking to a 10 ns grid, it is recommended to use a modulation frequency of 100 MHz.
 - **All operations need to start at an integer number of samples**. Because of the choice of sampling rates of 2.4 GSps (~0.416 ns) and 1.8 GSps (~0.555 ns) it is useful to stick to a 10 ns grid for HDAWG (microwave and flux) pulses and a 40 ns grid for UHFQA (readout) pulses.
 - **Different instructions on the same "awg" cannot start in the same clock cycle.** This implies that the readout acquisition delay cannot be 0 (but it can be 40 ns or - 40ns).
 - **All measurements are triggered simultaneously** using the `StartQA(QA_INT_ALL, true)` instruction. This implies it is not possible to read out only a specific qubit/channel.
 - **All measurements have to start at the same sample within a clock cycle** because one can only define a single integration weight per channel. To guarantee this, all operations are shifted around a bit (the measurement fixpoint correction). As a consequence, the reset/initialization operation can sometimes be a bit longer than specified in the schedule.
 - Because the **timing between two devices needs to align over longer schedules**, it is important that the clock-rates are accurate. To ensure phase stability, use a 10 MHz shared reference and operate the hardware in external reference mode.
-
 - Only a single HDAWG supported as the primary device, other HDAWGs need to be configured as secondary devices.
 - **Multiplexed readout is currently not supported**. One can only read out a single channel. (#191)
 
-Hardware configuration
-^^^^^^^^^^^^^^^^^^^^^^
+## Hardware configuration
 
-.. note::
+```{note}
+This section will move to the documentation of the hardware configuration file themselves. See issue #222.
+```
 
-    This section will move to the documentation of the hardware configuration file themselves. See issue #222.
-
-The :mod:`~quantify_scheduler.backends.zhinst_backend` allows Zurich Instruments to be
+The {mod}`~quantify_scheduler.backends.zhinst_backend` allows Zurich Instruments to be
 configured individually or collectively by enabling master/slave configurations via
 Triggers and Markers.
 
-Instruments can be configured by adding them to the :ref:`hardware configuration file<user-guide-example-zhinst-config>`.
+Instruments can be configured by adding them to the {ref}`hardware configuration file<user-guide-example-zhinst-config>`.
 The configuration file contains parameters about the Instruments and properties required
-to map :class:`quantify_scheduler.operations.operation.Operation`\s, which act on
+to map {class}`quantify_scheduler.operations.operation.Operation`s, which act on
 qubits, onto physical properties of the instrument.
 
-
 The Zurich Instruments hardware configuration file is divided in four main sections.
 
-1. The `backend` property defines the python method which will be executed by
-:func:`~quantify_scheduler.compilation.qcompile` in order to compile the backend.
+1\. The `backend` property defines the python method which will be executed by
+{func}`~quantify_scheduler.compilation.qcompile` in order to compile the backend.
 
 2. The `local_oscillators` property is a list of dicts which describe the available local oscillators in the hardware setup. An example entry are as follows:
 
+```{code-block} json
+:linenos: true
 
-.. code-block:: json
-    :linenos:
-
+{
+  "backend": "quantify_scheduler.backends.zhinst_backend.compile_backend",
+  "local_oscillators": [
     {
-      "backend": "quantify_scheduler.backends.zhinst_backend.compile_backend",
-      "local_oscillators": [
-        {
-          "unique_name": "mw_qubit_ch1",
-          "instrument_name": "mw_qubit",
-          "frequency":
-              {
-                  "ch_1.frequency": null
-              },
-          "power":
-              {
-                  "power": 13
-              },
-          "phase":
-              {
-                  "ch_1.phase": 90
-              }
-        }
-      ]
+      "unique_name": "mw_qubit_ch1",
+      "instrument_name": "mw_qubit",
+      "frequency":
+          {
+              "ch_1.frequency": null
+          },
+      "power":
+          {
+              "power": 13
+          },
+      "phase":
+          {
+              "ch_1.phase": 90
+          }
     }
-
-
-* In the example, the particular local_oscillator is given a `unique_name` which is then used in the `devices` to couple the channel of the device to that local oscillator.
-
-* The `instrument_name` is the QCoDes Instrument name for the local oscillator object.
-
-* The `frequency` property maps the frequency parameter which is used to set the frequency of the local oscillator. If set to `null`, then the local oscillator frequency is automatically calculated from the relation, LO frequency = RF frequency - Intermodulation frequency.
-
-* The `power` property is an optional key which maps the power parameter used to set the power of the local oscillator. If the key is not provided, no value will be set. Note that the units are based on the instruments used (i.e. if the QCoDeS instrument sets the power in dbm, then the power value should be in dbm).
-
-* The `phase` property is an optional key that maps the phase parameter used to set the phase of the local oscillator signal. If the key is not provided, no value will be set. Note that the units are based on the instruments used (i.e. if the QCoDeS instrument sets the phase in radians, then the phase value should be in radians).
+  ]
+}
+```
+
+- In the example, the particular local_oscillator is given a `unique_name` which is then used in the `devices` to couple the channel of the device to that local oscillator.
+- The `instrument_name` is the QCoDes Instrument name for the local oscillator object.
+- The `frequency` property maps the frequency parameter which is used to set the frequency of the local oscillator. If set to `null`, then the local oscillator frequency is automatically calculated from the relation, LO frequency = RF frequency - Intermodulation frequency.
+- The `power` property is an optional key which maps the power parameter used to set the power of the local oscillator. If the key is not provided, no value will be set. Note that the units are based on the instruments used (i.e. if the QCoDeS instrument sets the power in dbm, then the power value should be in dbm).
+- The `phase` property is an optional key that maps the phase parameter used to set the phase of the local oscillator signal. If the key is not provided, no value will be set. Note that the units are based on the instruments used (i.e. if the QCoDeS instrument sets the phase in radians, then the phase value should be in radians).
 
 3. The `latency_corrections` property specifies a delay on a port-clock combination which is implemented by incrementing the `abs_time` of all operations applied to the port-clock combination. The delay is used to manually adjust the timing to correct for e.g., delays due to different cable lengths.
 
+```{code-block} json
+:linenos: true
 
-.. code-block:: json
-    :linenos:
-
-    {
-      "backend": "quantify_scheduler.backends.zhinst_backend.compile_backend",
-      "latency_corrections":
-          {
-              "q0:mw-q0.01": 95e-9,
-              "q1:mw-q1.01": 95e-9
-              "q0:res-q0.ro": -95e-9,
-              "q0:res-q1.ro": -95e-9,
-
-          }
-    }
-
+{
+  "backend": "quantify_scheduler.backends.zhinst_backend.compile_backend",
+  "latency_corrections":
+      {
+          "q0:mw-q0.01": 95e-9,
+          "q1:mw-q1.01": 95e-9
+          "q0:res-q0.ro": -95e-9,
+          "q0:res-q1.ro": -95e-9,
+
+      }
+}
+```
 
 In this example, the user has specified latencies at each port-clock combination in the hardware config. The relative latencies to the minimum of the latencies are then calculated and applied to the signals for the specific port-clock combination. For this case, pulses with `port=q0:res`, and `clock=q0.r0` i.e. "q0:res-q0.ro" will have no corrections, whilst, pulses with `port=q0:mw`, and `clock=q0.01` i.e. "q0:mw-q0.01" will have a corrected delay of 190e-9 s added to the pulses.
 
-4. The `devices` property is an array of :class:`~quantify_scheduler.backends.types.zhinst.Device`.
+4\. The `devices` property is an array of {class}`~quantify_scheduler.backends.types.zhinst.Device`.
 A Device describes the type of Zurich Instruments and the physical setup.
 
+```{code-block} json
+:linenos: true
 
-.. code-block:: json
-    :linenos:
-
-    {
-      "backend": "quantify_scheduler.backends.zhinst_backend.compile_backend",
-      "devices": [
-
-      ]
-    }
-
+{
+  "backend": "quantify_scheduler.backends.zhinst_backend.compile_backend",
+  "devices": [
+
+  ]
+}
+```
 
 The entries in the `devices` section of the configuration file are strictly mapped
-according to the :class:`~quantify_scheduler.backends.types.zhinst.Device` and
-:class:`~quantify_scheduler.backends.types.zhinst.Output` domain models.
+according to the {class}`~quantify_scheduler.backends.types.zhinst.Device` and
+{class}`~quantify_scheduler.backends.types.zhinst.Output` domain models.
 
-* In order for the backend to find the QCodes Instrument it is required that the
-  :class:`~quantify_scheduler.backends.types.zhinst.Device`'s `name` must be equal to
+- In order for the backend to find the QCodes Instrument it is required that the
+  {class}`~quantify_scheduler.backends.types.zhinst.Device`'s `name` must be equal to
   the name given to the QCodes Instrument during instantiation with an `ic` prepend.
 
-    * Example: If the hdawg QCodes Instrument name is "hdawg_dev8831" then the :class:`~quantify_scheduler.backends.types.zhinst.Device`'s `name` is "ic_hdawg_dev8831"
+  > - Example: If the hdawg QCodes Instrument name is "hdawg_dev8831" then the {class}`~quantify_scheduler.backends.types.zhinst.Device`'s `name` is "ic_hdawg_dev8831"
 
-* The `type` property defines the instrument's model. The :class:`~quantify_scheduler.backends.types.zhinst.DeviceType`
+- The `type` property defines the instrument's model. The {class}`~quantify_scheduler.backends.types.zhinst.DeviceType`
   is parsed from the string as well as the number of channels.
 
-    * Example: "HDAWG8"
-
-* The `ref` property describes if the instrument uses Markers (`int`), Triggers (`ext`) or `none`.
-
-    * `int` Enables sending Marker
-
-    * `ext` Enables waiting for Marker
+  > - Example: "HDAWG8"
 
-    * `none` Ignores waiting for Marker
+- The `ref` property describes if the instrument uses Markers (`int`), Triggers (`ext`) or `none`.
 
+  > - `int` Enables sending Marker
+  > - `ext` Enables waiting for Marker
+  > - `none` Ignores waiting for Marker
 
-* The `channelgrouping` property sets the HDAWG channel grouping value and impacts the amount
+- The `channelgrouping` property sets the HDAWG channel grouping value and impacts the amount
   of HDAWG channels per AWG must be used.
 
-.. code-block:: python
-    :linenos:
-    :emphasize-lines: 5,17
-
+```{code-block} python
+:emphasize-lines: 5,17
+:linenos: true
+
+{
+  "backend": "quantify_scheduler.backends.zhinst_backend.compile_backend",
+  "devices": [
     {
-      "backend": "quantify_scheduler.backends.zhinst_backend.compile_backend",
-      "devices": [
-        {
-          "name": "hdawg0",
-          "ref": "int",
-          "channelgrouping": 0,
-          "channel_0": {
-            ...
-          },
-        },
-      ]
-    }
+      "name": "hdawg0",
+      "ref": "int",
+      "channelgrouping": 0,
+      "channel_0": {
+        ...
+      },
+    },
+  ]
+}
 
-    ...
-
-    instrument = zhinst.qcodes.HDAWG(name='hdawg0', serial='dev1234', ...)
+...
 
+instrument = zhinst.qcodes.HDAWG(name='hdawg0', serial='dev1234', ...)
+```
 
+```{eval-rst}
 .. autoclass:: quantify_scheduler.backends.types.zhinst.Device
     :members:
     :noindex:
+```
 
-* The `channel_{0..3}` properties of the hardware configuration are mapped to
-  the :class:`~quantify_scheduler.backends.types.zhinst.Output` domain model. A single
+- The `channel_{0..3}` properties of the hardware configuration are mapped to
+  the {class}`~quantify_scheduler.backends.types.zhinst.Output` domain model. A single
   `channel` represents a complex output, consisting of two physical I/O channels on
   the Instrument.
 
-* The `port` and `clock` properties map the Operations to physical and frequency space.
+- The `port` and `clock` properties map the Operations to physical and frequency space.
 
-* The `mode` property specifies the channel mode: real or complex.
+- The `mode` property specifies the channel mode: real or complex.
 
-* The `modulation` property specifies if the uploaded waveforms are modulated.
+- The `modulation` property specifies if the uploaded waveforms are modulated.
   The backend supports:
 
-    * Premodulation "premod"
-
-    * No modulation "none"
+  > - Premodulation "premod"
+  > - No modulation "none"
 
-* The `interm_freq` property specifies the inter-modulation frequency.
+- The `interm_freq` property specifies the inter-modulation frequency.
 
-* The `markers` property specifies which markers to trigger on each sequencer iteration.
+- The `markers` property specifies which markers to trigger on each sequencer iteration.
   The values are used as input for the `setTrigger` sequencer instruction.
 
-* The `triggers` property specifies for a sequencer which digital trigger to wait for.
+- The `triggers` property specifies for a sequencer which digital trigger to wait for.
   The first value of the `triggers` array is used as input parameter for the
   `waitDigTrigger` sequencer instruction.
 
+```{eval-rst}
 .. autoclass:: quantify_scheduler.backends.types.zhinst.Output
     :members:
     :noindex:
 
+```
 
-Tutorials
-^^^^^^^^^
+## Tutorials
 
-.. toctree::
-    :maxdepth: 3
+```{toctree}
+:maxdepth: 3
 
-    T_verification_programs.py
+T_verification_programs
+```
```

### Comparing `quantify-scheduler-0.8.0/docs/user_guide.rst` & `quantify-scheduler-0.9.0/docs/user_guide.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,490 +1,475 @@
-.. _sec-user-guide:
+---
+file_format: mystnb
+kernelspec:
+    name: python3
 
-User guide
-==========
+---
+(sec-user-guide)=
 
-.. jupyter-kernel::
-  :id: Scheduler getting started
+# User guide
 
-.. jupyter-execute::
-    :hide-code:
 
-    # Make output easier to read
-    from rich import pretty
-    pretty.install()
+```{code-cell} ipython3
+---
+mystnb:
+  remove_code_source: true
+---
 
+# Make output easier to read
+from rich import pretty
+pretty.install()
+
+```
+
+## Introduction
 
-Introduction
-------------
 Quantify-scheduler is a python module for writing quantum programs featuring a hybrid gate-pulse control model with explicit timing control.
 It extends the circuit model from quantum information processing by adding a pulse-level representation to operations defined at the gate-level, and the ability to specify timing constraints between operations.
 Thus, a user is able to mix gate- and pulse-level operations in a quantum circuit.
 
-
-In quantify-scheduler, both a quantum circuit consisting of gates and measurements and a timed sequence of control pulses are described as a :class:`.Schedule` .
-The :class:`.Schedule` contains information on *when* operations should be performed.
-When adding operations to a schedule, one does not need to specify how to represent this :class:`.Operation` on all (both gate and pulse) abstraction levels.
-Instead, this information can be added later during :ref:`Compilation`.
+In quantify-scheduler, both a quantum circuit consisting of gates and measurements and a timed sequence of control pulses are described as a {class}`.Schedule` .
+The {class}`.Schedule` contains information on *when* operations should be performed.
+When adding operations to a schedule, one does not need to specify how to represent this {class}`.Operation` on all (both gate and pulse) abstraction levels.
+Instead, this information can be added later during {ref}`Compilation`.
 This allows the user to effortlessly mix the gate- and pulse-level descriptions as is required for many experiments.
-We support a similar flexibility in the timing constraints, one can either explicitly specify the timing using :attr:`.ScheduleBase.schedulables`, or rely on the compilation which will use the duration of operations to schedule them back-to-back.
-
-
-Creating a schedule
--------------------
-
-The most convenient way to interact with a :class:`.Schedule` is through the :mod:`quantify_scheduler` API.
-In the following example, we will create a function to generate a :class:`.Schedule` for a a `Bell experiment <https://en.wikipedia.org/wiki/Bell%27s_theorem>`_ and visualize one instance of such a circuit.
+We support a similar flexibility in the timing constraints, one can either explicitly specify the timing using {attr}`.ScheduleBase.schedulables`, or rely on the compilation which will use the duration of operations to schedule them back-to-back.
 
+## Creating a schedule
 
-.. jupyter-execute::
-    :hide-output:
+The most convenient way to interact with a {class}`.Schedule` is through the {mod}`quantify_scheduler` API.
+In the following example, we will create a function to generate a {class}`.Schedule` for a a [Bell experiment](https://en.wikipedia.org/wiki/Bell%27s_theorem) and visualize one instance of such a circuit.
 
-    # import the Schedule class and some basic operations.
-    from quantify_scheduler import Schedule
-    from quantify_scheduler.operations.gate_library import Reset, Measure, CZ, Rxy, X90
+```{code-cell} ipython3
+---
+mystnb:
+  remove_code_outputs: true
+---
 
-    def bell_schedule(angles, q0:str, q1:str, repetitions: int):
+# import the Schedule class and some basic operations.
+from quantify_scheduler import Schedule
+from quantify_scheduler.operations.gate_library import Reset, Measure, CZ, Rxy, X90
 
-        for acq_index, angle in enumerate(angles):
+def bell_schedule(angles, q0:str, q1:str, repetitions: int):
 
-            sched = Schedule(f"Bell experiment on {q0}-{q1}")
+    for acq_index, angle in enumerate(angles):
 
-            sched.add(Reset(q0, q1))  # initialize the qubits
-            sched.add(X90(qubit=q0))
-            # Here we use a timing constraint to explicitly schedule the second gate to start
-            # simultaneously with the first gate.
-            sched.add(X90(qubit=q1), ref_pt="start", rel_time=0)
-            sched.add(CZ(qC=q0, qT=q1))
-            sched.add(Rxy(theta=angle, phi=0, qubit=q0) )
-            sched.add(Measure(q0, acq_index=acq_index))  # denote where to store the data
-            sched.add(Measure(q1, acq_index=acq_index), ref_pt="start")
+        sched = Schedule(f"Bell experiment on {q0}-{q1}")
 
-        return sched
+        sched.add(Reset(q0, q1))  # initialize the qubits
+        sched.add(X90(qubit=q0))
+        # Here we use a timing constraint to explicitly schedule the second gate to start
+        # simultaneously with the first gate.
+        sched.add(X90(qubit=q1), ref_pt="start", rel_time=0)
+        sched.add(CZ(qC=q0, qT=q1))
+        sched.add(Rxy(theta=angle, phi=0, qubit=q0) )
+        sched.add(Measure(q0, acq_index=acq_index))  # denote where to store the data
+        sched.add(Measure(q1, acq_index=acq_index), ref_pt="start")
 
+    return sched
 
-    sched = bell_schedule(
-        angles=[45.0],
-        q0="q0",
-        q1="q1",
-        repetitions=1024)
 
+sched = bell_schedule(
+    angles=[45.0],
+    q0="q0",
+    q1="q1",
+    repetitions=1024)
 
 
-.. jupyter-execute::
+```
 
-    # import the circuit visualizer
-    from quantify_scheduler.visualization.circuit_diagram import circuit_diagram_matplotlib
+```{code-cell} ipython3
 
-    # visualize the circuit
-    f, ax = circuit_diagram_matplotlib(sched)
+# import the circuit visualizer
+from quantify_scheduler.visualization.circuit_diagram import circuit_diagram_matplotlib
 
+# visualize the circuit
+f, ax = circuit_diagram_matplotlib(sched)
 
-.. tip::
+```
 
-    Creating schedule generating functions is a convenient design pattern when creating measurement code. See :ref:`the section on execution <sec-user-guide-execution>` for an example of how this is used in practice.
-
-Concepts and terminology
-------------------------
+```{tip}
+Creating schedule generating functions is a convenient design pattern when creating measurement code. See {ref}`the section on execution <sec-user-guide-execution>` for an example of how this is used in practice.
+```
 
+## Concepts and terminology
 
 Quantify-scheduler can be understood by understanding the following concepts.
 
-- :class:`.Schedule`\s describe when an operation needs to be applied.
-- :class:`.Operation`\s describe what needs to be done.
-- :class:`~quantify_scheduler.resources.Resource`\s describe where an operation should be applied.
-- :ref:`Compilation <sec-compilation>`: between different abstraction layers and onto a hardware backend.
+- {class}`.Schedule`s describe when an operation needs to be applied.
+- {class}`.Operation`s describe what needs to be done.
+- {class}`~quantify_scheduler.resources.Resource`s describe where an operation should be applied.
+- {ref}`Compilation <sec-compilation>`: between different abstraction layers for execution on physical hardware.
 
 The following table shows an overview of the different concepts and how these are represented at the quantum-circuit layer and quantum-device layer.
 
+```{list-table} Overview of concepts and their representation at different levels of abstraction.
+:widths: 25 25 25 25
+:header-rows: 0
+
+- *
+  * Concept
+  * Quantum-circuit layer
+  * Quantum-device layer
+- * When
+  * {class}`.Schedule`
+  * --
+  * --
+- * What
+  * {class}`.Operation`
+  * {ref}`Gates and Measurements <sec-user-guide-gates-measurement>`
+  * {ref}`Pulses and acquisition protocols <sec-user-guide-pulses-acq-protocols>`
+- * Where
+  * {class}`~quantify_scheduler.resources.Resource`
+  * {ref}`Qubits <sec-user-guide-qubits>`
+  * {ref}`Ports and clocks <sec-user-guide-ports-clocks>`
 
-.. list-table:: Overview of concepts and their representation at different levels of abstraction.
-    :widths: 25 25 25 25
-    :header-rows: 0
-
-    * -
-      - Concept
-      - Quantum-circuit layer
-      - Quantum-device layer
-    * - When
-      - :class:`.Schedule`
-      - --
-      - --
-    * - What
-      - :class:`.Operation`
-      - :ref:`Gates and Measurements <sec-user-guide-gates-measurement>`
-      - :ref:`Pulses and acquisition protocols <sec-user-guide-pulses-acq-protocols>`
-    * - Where
-      - :class:`~quantify_scheduler.resources.Resource`
-      - :ref:`Qubits <sec-user-guide-qubits>`
-      - :ref:`Ports and clocks <sec-user-guide-ports-clocks>`
+```
 
+(sec-user-guide-quantum-circuit)=
 
-.. _sec-user-guide-quantum-circuit:
+### Quantum-circuit layer
 
-Quantum-circuit layer
-~~~~~~~~~~~~~~~~~~~~~
 The Quantum-circuit description is an idealized mathematical description of a schedule.
 
+(sec-user-guide-gates-measurement)=
 
-.. _sec-user-guide-gates-measurement:
+#### Gates and measurements
 
-Gates and measurements
-^^^^^^^^^^^^^^^^^^^^^^
-In this description operations are `quantum gates <https://en.wikipedia.org/wiki/Quantum_logic_gate>`_  that act on idealized qubits as part of a `quantum circuit <https://en.wikipedia.org/wiki/Quantum_circuit>`_.
+In this description operations are [quantum gates](https://en.wikipedia.org/wiki/Quantum_logic_gate)  that act on idealized qubits as part of a [quantum circuit](https://en.wikipedia.org/wiki/Quantum_circuit).
 Operations can be represented by (idealized) unitaries acting on qubits.
-The :mod:`~quantify_scheduler.operations.gate_library` contains common operations (including the measurement operation) described at the quantum-circuit level.
+The {mod}`~quantify_scheduler.operations.gate_library` contains common operations (including the measurement operation) described at the quantum-circuit level.
 
-The :class:`~quantify_scheduler.operations.gate_library.Measure` is a special operation that represents a measurement on a qubit.
+The {class}`~quantify_scheduler.operations.gate_library.Measure` is a special operation that represents a measurement on a qubit.
 In addition to the qubit it acts on, one also needs to specify where to store the data.
 
-.. _sec-user-guide-qubits:
+(sec-user-guide-qubits)=
+
+#### Qubits
 
-Qubits
-^^^^^^
 At the gate-level description, operations are applied to qubits.
-Qubits are represented by strings corresponding to the name of a qubit (e.g., :code:`q0`, :code:`q1`, :code:`A1`, :code:`QL`, :code:`qubit_1`, etc.).
-Valid qubits are strings that appear in the :ref:`device configuration file<sec-device-config>` used when compiling the schedule.
+Qubits are represented by strings corresponding to the name of a qubit (e.g., {code}`q0`, {code}`q1`, {code}`A1`, {code}`QL`, {code}`qubit_1`, etc.).
+Valid qubits are strings that appear in the {ref}`device configuration file<sec-device-config>` used when compiling the schedule.
 
+#### Visualization
 
-Visualization
-^^^^^^^^^^^^^
-A :class:`.Schedule` containing operations can be visualized using as a circuit diagram using :func:`~quantify_scheduler.visualization.circuit_diagram.circuit_diagram_matplotlib`.
+A {class}`.Schedule` containing operations can be visualized using as a circuit diagram using {func}`~quantify_scheduler.visualization.circuit_diagram.circuit_diagram_matplotlib`.
 
-Alternatively, one can plot the waveforms in schedules using :func:`~quantify_scheduler.visualization.pulse_diagram.pulse_diagram_matplotlib`:
+Alternatively, one can plot the waveforms in schedules using {func}`~quantify_scheduler.visualization.pulse_diagram.pulse_diagram_matplotlib`:
 
-.. jupyter-execute::
+```{code-cell} ipython3
 
-    from quantify_scheduler.operations.pulse_library import SquarePulse, RampPulse
-    from quantify_scheduler.compilation import determine_absolute_timing
-    from quantify_scheduler.visualization.pulse_diagram import pulse_diagram_matplotlib
+from quantify_scheduler.operations.pulse_library import SquarePulse, RampPulse
+from quantify_scheduler.compilation import determine_absolute_timing
+from quantify_scheduler.visualization.pulse_diagram import pulse_diagram_matplotlib
 
-    schedule = Schedule("waveforms")
-    schedule.add(SquarePulse(amp=0.2, duration=4e-6, port="P"))
-    schedule.add(RampPulse(amp=-0.1, offset=.2, duration=6e-6, port="P"))
-    schedule.add(SquarePulse(amp=0.1, duration=4e-6, port="Q"), ref_pt='start')
-    determine_absolute_timing(schedule)
+schedule = Schedule("waveforms")
+schedule.add(SquarePulse(amp=0.2, duration=4e-6, port="P"))
+schedule.add(RampPulse(amp=-0.1, offset=.2, duration=6e-6, port="P"))
+schedule.add(SquarePulse(amp=0.1, duration=4e-6, port="Q"), ref_pt='start')
+determine_absolute_timing(schedule)
 
-    _ = pulse_diagram_matplotlib(schedule, sampling_rate=20e6)
+_ = pulse_diagram_matplotlib(schedule, sampling_rate=20e6)
 
+```
 
-Summary
-^^^^^^^
+#### Summary
 
 - Gates are described by unitaries.
 - Gates are applied to qubits.
 - Measurements are applied to qubits.
 - Qubits are represented by strings.
 
+(sec-user-guide-quantum-device)=
 
-.. _sec-user-guide-quantum-device:
-
-Quantum-device layer
-~~~~~~~~~~~~~~~~~~~~~
+### Quantum-device layer
 
 The quantum-device layer describes waveforms and acquisition protocols applied to a device.
 These waveforms can be used to implement the idealized operations expressed on the quantum-circuit layer, or can be used without specifying a corresponding representation at the quantum-circuit layer.
 
-.. _sec-user-guide-pulses-acq-protocols:
+(sec-user-guide-pulses-acq-protocols)=
+
+#### Pulses and acquisition protocols
 
-Pulses and acquisition protocols
-^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 The pulse-level description typically contains parameterization information, such as amplitudes, durations and so forth required to synthesize the waveform on control hardware.
-The :mod:`~quantify_scheduler.operations.pulse_library` contains a collection of commonly used pulses.
+The {mod}`~quantify_scheduler.operations.pulse_library` contains a collection of commonly used pulses.
 
 Measurements are represented as acquisition protocols.
 Acquisition protocols describe the processing steps to perform on an acquired signal in order to interpret it.
-The :mod:`~quantify_scheduler.operations.acquisition_library` contains a collection of commonly used acquisition protocols.
+The {mod}`~quantify_scheduler.operations.acquisition_library` contains a collection of commonly used acquisition protocols.
 
-.. _sec-user-guide-ports-clocks:
+(sec-user-guide-ports-clocks)=
 
-Ports and clocks
-^^^^^^^^^^^^^^^^
+#### Ports and clocks
 
 To specify *where* an operation is applied, the quantum-device layer description needs to specify both the location in physical space as well as in frequency space.
 
 For many systems, it is possible to associate a qubit with an element or location on a device that a signal can be applied to.
 We call such a location on a device a port.
-Like qubits, ports are represented as strings (e.g., :code:`P0`, :code:`feedline_in`, :code:`q0:mw_drive`, etc.).
-In the last example, a port is associated with a qubit by including the qubit name in the beginning of the port name (separated by a colon :code:`:`).
+Like qubits, ports are represented as strings (e.g., {code}`P0`, {code}`feedline_in`, {code}`q0:mw_drive`, etc.).
+In the last example, a port is associated with a qubit by including the qubit name in the beginning of the port name (separated by a colon {code}`:`).
 
 Associating a qubit can be useful when visualizing a schedule and or to keep configuration files readable.
 It is, however, not required to associate a port with a single qubit.
 This keeps matters simple when ports are associated with multiple qubits or with non-qubit elements such as tunable couplers.
 
-
 Besides the physical location on a device, a pulse is typically applied at a certain frequency and with a phase.
-These two parameters are stored in a :class:`~quantify_scheduler.resources.ClockResource`.
-Each :class:`~quantify_scheduler.resources.ClockResource` also has a :code:`name` to be easily identified.
-The :code:`name` should identify the purpose of the clock resource, not the value of the frequency.
+These two parameters are stored in a {class}`~quantify_scheduler.resources.ClockResource`.
+Each {class}`~quantify_scheduler.resources.ClockResource` also has a {code}`name` to be easily identified.
+The {code}`name` should identify the purpose of the clock resource, not the value of the frequency.
 By storing the frequency and phase in a clock, we can adjust the frequency of a transition, but refer to it with the same name.
 
 Similar to ports, clocks can be associated with qubits by including the qubit name in the clock name (again, this is not required).
 If the frequency of a clock is set to 0 (zero), the pulse is applied at baseband and is assumed to be real-valued.
 
-:numref:`resources_fig` shows how the resources (qubit, port and clock) map to a physical device.
+{numref}`resources_fig` shows how the resources (qubit, port and clock) map to a physical device.
 
-.. figure:: /images/Device_ports_clocks.svg
-    :width: 800
-    :name: resources_fig
-
-    Resources are used to indicate *where* operations are applied.
-    (a) Ports (purple) indicate a location on a device.
-    By prefixing the name of a qubit in a port name (separated by a colon :code:`:`) a port can be associated with a qubit (red), but this is not required.
-    (b) Clocks (blue) denote the frequency and phase of a signal.
-    They can be set to track the phase of a known transition.
-    By prefixing the name of a qubit in a clock name (separated by a colon :code:`:`) a clock can be associated with a qubit (red), but this is not required.
-    Device image from `Dickel (2018) <https://doi.org/10.4233/uuid:78155c28-3204-4130-a645-a47e89c46bc5>`_ .
+```{figure} /images/Device_ports_clocks.svg
+:name: resources_fig
+:width: 800
+
+Resources are used to indicate *where* operations are applied.
+(a) Ports (purple) indicate a location on a device.
+By prefixing the name of a qubit in a port name (separated by a colon {code}`:`) a port can be associated with a qubit (red), but this is not required.
+(b) Clocks (blue) denote the frequency and phase of a signal.
+They can be set to track the phase of a known transition.
+By prefixing the name of a qubit in a clock name (separated by a colon {code}`:`) a clock can be associated with a qubit (red), but this is not required.
+Device image from [Dickel (2018)](https://doi.org/10.4233/uuid:78155c28-3204-4130-a645-a47e89c46bc5) .
+```
 
-
-Summary
-^^^^^^^
+#### Summary
 
 - Pulses are described as parameterized waveforms.
 - Pulses are applied to *ports* at a frequency specified by a *clock*.
 - Ports and clocks are represented by strings.
 - Acquisition protocols describe the processing steps to perform on an acquired signal in order to interpret it.
 
+(sec-compilation)=
 
-
-
-.. _sec-compilation:
-
-Compilation
------------
+## Compilation
 
 Different compilation steps are required to go from a high-level description of a schedule to something that can be executed on hardware.
-The scheduler supports two main compilation steps, the first from the gate to the pulse level, and a second from the pulse-level to a hardware back end.
-This is schematically shown in :numref:`compilation_overview`.
-
-
-.. figure:: /images/compilation_overview.svg
-    :name: compilation_overview
-    :align: center
-    :width: 900px
+The scheduler supports multiple compilation steps, the most important ones are the step from the quantum-circuit layer (gates) to the quantum-device layer (pulses), and the one from the quantum-device layer into instructions suitable for execution on physical hardware.
+The compilation is performed by a {class}`~.QuantifyCompiler`. The compilers are described in detail in {ref}`Compilers`.
+This is schematically shown in {numref}`compilation_overview`.
+
+```{figure} /images/compilation_overview.svg
+:align: center
+:name: compilation_overview
+:width: 900px
+
+A schematic overview of the different abstraction layers and the compilation process.
+Both a quantum circuit, consisting of gates and measurements of qubits, and timed sequences of control pulses are represented as a {class}`.Schedule` .
+The information specified in the {ref}`device configuration<sec-device-config>` is used during compilation to add information on how to represent {class}`.Operation` s specified at the quantum-circuit level as control pulses.
+The information in the {ref}`hardware configuration <sec-hardware-config>` is then used to compile the control pulses into instructions suitable for hardware execution.
+```
 
-    A schematic overview of the different abstraction layers and the compilation process.
-    Both a quantum circuit, consisting of gates and measurements of qubits, and timed sequences of control pulses are represented as a :class:`.Schedule` .
-    The information specified in the :ref:`device configuration<sec-device-config>` is used during compilation to add information on how to represent :class:`.Operation` s specified at the quantum-circuit level as control pulses.
-    The information in the :ref:`hardware configuration <sec-hardware-config>` is then used to compile the control pulses into instructions suitable for hardware execution.
+In the first compilation step, pulse information is added to all operations that are not valid pulses (see {attr}`.Operation.valid_pulse`) based on the information specified in the {ref}`device configuration file<sec-device-config>`.
 
+A second compilation step takes the schedule at the pulse level and translates this for use on a hardware back end.
+This compilation step is performed using a hardware dependent compiler and uses the information specified in the {ref}`hardware configuration file<sec-hardware-config>`.
 
-In the first compilation step, pulse information is added to all operations that are not valid pulses (see :attr:`.Operation.valid_pulse`) based on the information specified in the :ref:`device configuration file<sec-device-config>`.
+Both compilation steps can be triggered by passing a {class}`.Schedule` and the appropriate configuration files to {func}`~quantify_scheduler.compilation.qcompile`.
 
-A second compilation step takes the schedule at the pulse level and translates this for use on a hardware back end.
-This compilation step is performed using a hardware dependent compiler and uses the information specified in the :ref:`hardware configuration file<sec-hardware-config>`.
+```{note}
+We use the term "**device**" to refer to the physical object(s) on the receiving end of the control pulses, e.g. a thin-film chip inside a dilution refrigerator.
 
-Both compilation steps can be triggered by passing a :class:`.Schedule` and the appropriate configuration files to :func:`~quantify_scheduler.compilation.qcompile`.
+And we employ the term "**hardware**" to refer to the instruments (electronics) that are involved in the pulse generations / signal digitization.
+```
 
-.. note::
+```{toctree}
+:glob: true
+:hidden: true
+:maxdepth: 2
 
-    We use the term "**device**" to refer to the physical object(s) on the receiving end of the control pulses, e.g. a thin-film chip inside a dilution refrigerator.
+quantify_compilers
 
-    And we employ the term "**hardware**" to refer to the instruments (electronics) that are involved in the pulse generations / signal digitization.
+```
 
-.. _sec-device-config:
+(sec-device-config)=
 
-Device configuration
-~~~~~~~~~~~~~~~~~~~~
+### Device configuration
 
 The device configuration is used to compile from the quantum-circuit layer to the quantum-device layer.
-The :class:`~.backends.circuit_to_device.DeviceCompilationConfig` data structure contains the information required to add the quantum-device level representation to every operation in a schedule.
+The {class}`~.backends.circuit_to_device.DeviceCompilationConfig` data structure contains the information required to add the quantum-device level representation to every operation in a schedule.
 
+```{eval-rst}
 .. autoclass:: quantify_scheduler.backends.circuit_to_device.DeviceCompilationConfig
     :noindex:
 
+```
 
-.. _sec-hardware-config:
+(sec-hardware-config)=
 
-Hardware configuration file
-~~~~~~~~~~~~~~~~~~~~~~~~~~~
+### Hardware configuration file
 
 The hardware configuration file is used to compile pulses (and acquisition protocols) along with their timing information to instructions compatible with the specific control electronics.
 To do this, it contains information on what control electronics to compile to and the connectivity: which ports are connected to which hardware outputs/inputs, as well as other hardware-specific settings.
 Similar to the device configuration file, the hardware configuration file can be written down manually as JSON or be code generated.
 
-.. _user-guide-example-qblox-config:
-
-.. admonition:: Example Qblox hardware configuration file
-    :class: dropdown
-
-    .. jupyter-execute::
-        :hide-code:
-
-        from pathlib import Path
-        import json
-        import quantify_scheduler.schemas.examples as examples
+(user-guide-example-qblox-config)=
+````{admonition} Example Qblox hardware configuration file
+:class: dropdown
+```{literalinclude} ../quantify_scheduler/schemas/examples/qblox_test_mapping.json
+:language: JSON
+```
+````
+
+(user-guide-example-zhinst-config)=
+````{admonition} Example Zurich Instruments hardware configuration file
+:class: dropdown
+```{literalinclude} ../quantify_scheduler/schemas/examples/zhinst_test_mapping.json
+:language: JSON
+```
+````
+
+
+## Execution
+
+(sec-user-guide-execution)=
+
+```{warning}
+This section describes functionality that is not fully implemented yet.
+The documentation describes the intended design and may change as the functionality is added.
+```
 
-        path = Path(examples.__file__).parent / "qblox_test_mapping.json"
-        json_data = json.loads(path.read_text())
-        json_data
-
-.. _user-guide-example-zhinst-config:
-
-.. admonition:: Example Zurich Instruments hardware configuration file
-    :class: dropdown
-
-    .. jupyter-execute::
-        :hide-code:
-
-        from pathlib import Path
-        import json
-        import quantify_scheduler.schemas.examples as examples
-
-        path = Path(examples.__file__).parent / "zhinst_test_mapping.json"
-        json_data = json.loads(path.read_text())
-        json_data
-
-
-Execution
----------
-
-.. _sec-user-guide-execution:
-
-.. warning::
-
-    This section describes functionality that is not fully implemented yet.
-    The documentation describes the intended design and may change as the functionality is added.
-
-
-Different kinds of instruments
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+### Different kinds of instruments
 
 In order to execute a schedule, one needs both physical instruments to execute the compiled instructions as well as a way to manage the calibration parameters used to compile the schedule.
-Although one could use manually written configuration files and send the compiled files directly to the hardware, the Quantify framework provides different kinds of :class:`~qcodes.instrument.base.Instrument`\s to control the experiments and the management of the configuration files (:numref:`instruments_overview`).
-
-
-.. figure:: /images/instruments_overview.svg
-    :name: instruments_overview
-    :align: center
-    :width: 600px
+Although one could use manually written configuration files and send the compiled files directly to the hardware, the Quantify framework provides different kinds of {class}`~qcodes.instrument.base.Instrument`s to control the experiments and the management of the configuration files ({numref}`instruments_overview`).
 
-    A schematic overview of the different kinds of instruments present in an experiment.
-    Physical instruments are QCoDeS drivers that are directly responsible for executing commands on the control hardware.
-    On top of the physical instruments is a hardware abstraction layer, that provides a hardware agnostic interface to execute compiled schedules.
-    The instruments responsible for experiment control are treated to be as stateless as possible [*]_ .
-    The knowledge about the system that is required to generate the configuration files is described by the :class:`~quantify_scheduler.device_under_test.quantum_device.QuantumDevice` and :code:`DeviceElement`\s.
-    Several utility instruments are used to control the flow of the experiments.
+```{figure} /images/instruments_overview.svg
+:align: center
+:name: instruments_overview
+:width: 600px
+
+A schematic overview of the different kinds of instruments present in an experiment.
+Physical instruments are QCoDeS drivers that are directly responsible for executing commands on the control hardware.
+On top of the physical instruments is a hardware abstraction layer, that provides a hardware agnostic interface to execute compiled schedules.
+The instruments responsible for experiment control are treated to be as stateless as possible [^id3] .
+The knowledge about the system that is required to generate the configuration files is described by the {class}`~quantify_scheduler.device_under_test.quantum_device.QuantumDevice` and {code}`DeviceElement`s.
+Several utility instruments are used to control the flow of the experiments.
+```
 
-Physical instruments
-^^^^^^^^^^^^^^^^^^^^
+#### Physical instruments
 
-`QCoDeS instrument drivers <https://qcodes.github.io/Qcodes/api/generated/qcodes.instrument_drivers.html>`_ are used to represent the physical hardware.
+[QCoDeS instrument drivers](https://qcodes.github.io/Qcodes/api/generated/qcodes.instrument_drivers.html) are used to represent the physical hardware.
 For the purpose of quantify-scheduler, these instruments are treated as stateless, the desired configurations for an experiment being described by the compiled instructions.
 Because the instruments correspond to physical hardware, there is a significant overhead in querying and configuring these parameters.
 As such, the state of the instruments in the software is intended to track the state of the physical hardware to facilitate lazy configuration and logging purposes.
 
-Hardware abstraction layer
-^^^^^^^^^^^^^^^^^^^^^^^^^^
-Because different physical instruments have different interfaces, a hardware abstraction layer serves to provide a uniform interface.
-This hardware abstraction layer is implemented as the :class:`~.InstrumentCoordinator` to which individual :class:`InstrumentCoordinatorComponent <.InstrumentCoordinatorComponentBase>`\s are added that provide the uniform interface to the individual instruments.
-
-
-The quantum device and the device elements
-^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+#### Hardware abstraction layer
 
-The knowledge of the system is described by the :class:`~quantify_scheduler.device_under_test.quantum_device.QuantumDevice` and :code:`DeviceElement`\s.
-The :class:`~quantify_scheduler.device_under_test.quantum_device.QuantumDevice` directly represents the device under test (DUT) and contains a description of the connectivity to the control hardware as well as parameters specifying quantities like cross talk, attenuation and calibrated cable-delays.
-The :class:`~quantify_scheduler.device_under_test.quantum_device.QuantumDevice` also contains references to individual :code:`DeviceElement`\s, representations of elements on a device (e.g, a transmon qubit) containing the (calibrated) control-pulse parameters.
-
-Because the :class:`~quantify_scheduler.device_under_test.quantum_device.QuantumDevice` and the :code:`DeviceElement`\s are an :class:`~qcodes.instrument.base.Instrument`, the parameters used to generate the configuration files can be easily managed and are stored in the snapshot containing the experiment's metadata.
+Because different physical instruments have different interfaces, a hardware abstraction layer serves to provide a uniform interface.
+This hardware abstraction layer is implemented as the {class}`~.InstrumentCoordinator` to which individual {class}`InstrumentCoordinatorComponent <.InstrumentCoordinatorComponentBase>`s are added that provide the uniform interface to the individual instruments.
 
-Experiment flow
-~~~~~~~~~~~~~~~
+#### The quantum device and the device elements
 
-To use schedules in an experimental setting, in which the parameters used for compilation as well as the schedules themselves routinely change, we provide a framework for performing experiments making use of the concepts of :mod:`quantify_core`.
-Central in this framework are the schedule :mod:`quantify_scheduler.gettables` that can be used by the :class:`~quantify_core.measurement.control.MeasurementControl` and are responsible for the experiment flow.
+The knowledge of the system is described by the {class}`~quantify_scheduler.device_under_test.quantum_device.QuantumDevice` and {code}`DeviceElement`s.
+The {class}`~quantify_scheduler.device_under_test.quantum_device.QuantumDevice` directly represents the device under test (DUT) and contains a description of the connectivity to the control hardware as well as parameters specifying quantities like cross talk, attenuation and calibrated cable-delays.
+The {class}`~quantify_scheduler.device_under_test.quantum_device.QuantumDevice` also contains references to individual {code}`DeviceElement`s, representations of elements on a device (e.g, a transmon qubit) containing the (calibrated) control-pulse parameters.
 
-This flow is schematically shown in :numref:`experiments_control_flow`.
+Because the {class}`~quantify_scheduler.device_under_test.quantum_device.QuantumDevice` and the {code}`DeviceElement`s are an {class}`~qcodes.instrument.base.Instrument`, the parameters used to generate the configuration files can be easily managed and are stored in the snapshot containing the experiment's metadata.
 
+### Experiment flow
 
-.. figure:: /images/experiments_control_flow.svg
-    :name: experiments_control_flow
-    :align: center
-    :width: 800px
+To use schedules in an experimental setting, in which the parameters used for compilation as well as the schedules themselves routinely change, we provide a framework for performing experiments making use of the concepts of {mod}`quantify_core`.
+Central in this framework are the schedule {mod}`quantify_scheduler.gettables` that can be used by the {class}`~quantify_core.measurement.control.MeasurementControl` and are responsible for the experiment flow.
 
-    A schematic overview of the experiments control flow.
+This flow is schematically shown in {numref}`experiments_control_flow`.
 
+```{figure} /images/experiments_control_flow.svg
+:align: center
+:name: experiments_control_flow
+:width: 800px
 
-Let us consider the example of an experiment used to measure the coherence time :math:`T_1`.
-In this experiment a :math:`\pi` pulse is used to excite the qubit, which is left to idle for a time :math:`\tau` before it is measured.
-This experiment is then repeated for different :math:`\tau` and averaged.
+A schematic overview of the experiments control flow.
+```
 
-In terms of settables and gettables to use with the :class:`~quantify_core.measurement.control.MeasurementControl`, the settable in this experiment is the delay time :math:`\tau`, and the gettable is the execution of the schedule.
+Let us consider the example of an experiment used to measure the coherence time {math}`T_1`.
+In this experiment a {math}`\pi` pulse is used to excite the qubit, which is left to idle for a time {math}`\tau` before it is measured.
+This experiment is then repeated for different {math}`\tau` and averaged.
 
-We represent the settable as a :class:`qcodes.instrument.parameter.ManualParameter`:
+In terms of settables and gettables to use with the {class}`~quantify_core.measurement.control.MeasurementControl`, the settable in this experiment is the delay time {math}`\tau`, and the gettable is the execution of the schedule.
 
-.. jupyter-execute::
+We represent the settable as a {class}`qcodes.instrument.parameter.ManualParameter`:
 
-    from qcodes.instrument.parameter import ManualParameter
+```{code-cell} ipython3
 
-    tau = ManualParameter("tau", label=r"Delay time", initial_value=0, unit="s")
+from qcodes.instrument.parameter import ManualParameter
 
+tau = ManualParameter("tau", label=r"Delay time", initial_value=0, unit="s")
 
-To execute the schedule with the right parameters, the :code:`ScheduleGettable` needs to have a reference to a template function that generates the schedule, the appropriate keyword arguments for that function, and a reference to the :class:`~quantify_scheduler.device_under_test.quantum_device.QuantumDevice` to generate the required configuration files.
+```
 
-For the :math:`T_1` experiment, quantify-scheduler provides a schedule generating function as part of the :mod:`quantify_scheduler.schedules.timedomain_schedules`: the :func:`quantify_scheduler.schedules.timedomain_schedules.t1_sched`.
+To execute the schedule with the right parameters, the {code}`ScheduleGettable` needs to have a reference to a template function that generates the schedule, the appropriate keyword arguments for that function, and a reference to the {class}`~quantify_scheduler.device_under_test.quantum_device.QuantumDevice` to generate the required configuration files.
 
-.. jupyter-execute::
+For the {math}`T_1` experiment, quantify-scheduler provides a schedule generating function as part of the {mod}`quantify_scheduler.schedules.timedomain_schedules`: the {func}`quantify_scheduler.schedules.timedomain_schedules.t1_sched`.
 
-    from quantify_scheduler.schedules.timedomain_schedules import t1_sched
-    schedule_function = t1_sched
+```{code-cell} ipython3
 
+from quantify_scheduler.schedules.timedomain_schedules import t1_sched
+schedule_function = t1_sched
 
-Inspecting the :func:`quantify_scheduler.schedules.timedomain_schedules.t1_sched`, we find that we need to provide the times :math:`\tau`, the name of the qubit, and the number of times we want to repeat the schedule.
-Rather than specifying the values of the delay times, we pass the parameter :code:`tau`.
+```
 
-.. jupyter-execute::
+Inspecting the {func}`quantify_scheduler.schedules.timedomain_schedules.t1_sched`, we find that we need to provide the times {math}`\tau`, the name of the qubit, and the number of times we want to repeat the schedule.
+Rather than specifying the values of the delay times, we pass the parameter {code}`tau`.
 
-    qubit_name = "q0"
-    sched_kwargs = {
-        "times": tau,
-        "qubit": qubit_name,
-        "repetitions": 1024 # could also be a parameter
-    }
+```{code-cell} ipython3
 
-The :code:`ScheduleGettable` is set up to evaluate the value of these parameter on every call of :code:`ScheduleGettable.get`.
-This flexibility allows the user to create template schedules that can then be measured by varying any of it's input parameters using the :class:`~quantify_core.measurement.control.MeasurementControl`.
+qubit_name = "q0"
+sched_kwargs = {
+    "times": tau,
+    "qubit": qubit_name,
+    "repetitions": 1024 # could also be a parameter
+}
+```
 
-Similar to how the schedule keyword arguments are evaluated for every call to :code:`ScheduleGettable.get`, the device config and hardware config files are re-generated from the :class:`~quantify_scheduler.device_under_test.quantum_device.QuantumDevice` for every iteration.
-This ensures that if a calibration parameter is changed on the :class:`~quantify_scheduler.device_under_test.quantum_device.QuantumDevice`, the compilation will be affected as expected.
+The {code}`ScheduleGettable` is set up to evaluate the value of these parameter on every call of {code}`ScheduleGettable.get`.
+This flexibility allows the user to create template schedules that can then be measured by varying any of it's input parameters using the {class}`~quantify_core.measurement.control.MeasurementControl`.
 
+Similar to how the schedule keyword arguments are evaluated for every call to {code}`ScheduleGettable.get`, the device config and hardware config files are re-generated from the {class}`~quantify_scheduler.device_under_test.quantum_device.QuantumDevice` for every iteration.
+This ensures that if a calibration parameter is changed on the {class}`~quantify_scheduler.device_under_test.quantum_device.QuantumDevice`, the compilation will be affected as expected.
 
-.. jupyter-execute::
+```{code-cell} ipython3
 
-    from quantify_scheduler.device_under_test.quantum_device import QuantumDevice
-    device = QuantumDevice(name="quantum_sample")
+from quantify_scheduler.device_under_test.quantum_device import QuantumDevice
+device = QuantumDevice(name="quantum_sample")
+```
 
 These ingredients can then be combined to perform the experiment:
 
-.. jupyter-execute::
-
-    from quantify_core.measurement import MeasurementControl
-    meas_ctrl = MeasurementControl("meas_ctrl")
-
-.. code-block:: python
-
-    t1_gettable = ScheduleGettable(
-        device=device,
-        schedule_function=schedule_function,
-        schedule_kwargs=sched_kwargs
-    )
-
-    meas_ctrl.settables(tau)
-    meas_ctrl.setpoints(times)
-    meas_ctrl.gettables(t1_gettable)
-    label = f"T1 experiment {qubit_name}"
-    dataset = meas_ctrl.run(label)
+```{code-cell} ipython3
 
+from quantify_core.measurement import MeasurementControl
+meas_ctrl = MeasurementControl("meas_ctrl")
+```
+
+```{code-block} python
+t1_gettable = ScheduleGettable(
+    device=device,
+    schedule_function=schedule_function,
+    schedule_kwargs=sched_kwargs
+)
+
+meas_ctrl.settables(tau)
+meas_ctrl.setpoints(times)
+meas_ctrl.gettables(t1_gettable)
+label = f"T1 experiment {qubit_name}"
+dataset = meas_ctrl.run(label)
+```
 
 and the resulting dataset can be analyzed using
 
-.. jupyter-execute::
+```{code-cell} ipython3
 
-    # from quantify_core.analysis.t1_analysis import T1Analysis
-    # analysis = T1Analysis(label=label).run()
+# from quantify_core.analysis.t1_analysis import T1Analysis
+# analysis = T1Analysis(label=label).run()
 
 
+```
 
-.. rubric:: Footnotes
+```{rubric} Footnotes
+```
 
-.. [*] Quantify-scheduler threats physical instruments as stateless in the sense that the compiled instructions contain all information that specify the executing of a schedule. However, for performance reasons, it is important to not reconfigure all parameters of all instruments whenever a new schedule is executed. The parameters (state) of the instruments are used to track the state of physical instruments to allow lazy configuration as well as ensuring metadata containing the current settings is stored correctly.
+[^id3]: Quantify-scheduler threats physical instruments as stateless in the sense that the compiled instructions contain all information that specify the executing of a schedule. However, for performance reasons, it is important to not reconfigure all parameters of all instruments whenever a new schedule is executed. The parameters (state) of the instruments are used to track the state of physical instruments to allow lazy configuration as well as ensuring metadata containing the current settings is stored correctly.
```

### Comparing `quantify-scheduler-0.8.0/quantify_scheduler/__init__.py` & `quantify-scheduler-0.9.0/quantify_scheduler/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
       - :class:`!quantify_scheduler.schedules.schedule.CompiledSchedule`
     * - :class:`.Operation`
       - :class:`!quantify_scheduler.operations.operation.Operation`
     * - :class:`.Resource`
       - :class:`!quantify_scheduler.Resource`
 """
 
-__version__ = "0.8.0"
+__version__ = "0.9.0"
 
 
 from . import structure
 from .operations.operation import Operation
 from .resources import Resource
 from .schedules.schedule import CompiledSchedule, Schedule, Schedulable
```

### Comparing `quantify-scheduler-0.8.0/quantify_scheduler/backends/circuit_to_device.py` & `quantify-scheduler-0.9.0/quantify_scheduler/backends/circuit_to_device.py`

 * *Files 2% similar despite different names*

```diff
@@ -103,15 +103,15 @@
     backend: str
     clocks: Dict[str, float]
     elements: Dict[str, Dict[str, OperationCompilationConfig]]
     edges: Dict[str, Dict[str, OperationCompilationConfig]]
 
 
 def compile_circuit_to_device(
-    schedule: Schedule, device_cfg: Union[DeviceCompilationConfig, dict]
+    schedule: Schedule, device_cfg: Union[DeviceCompilationConfig, dict, None]
 ) -> Schedule:
     """
     Adds the information required to represent operations on the quantum-device
     abstraction layer to operations that contain information on how to be represented
     on the quantum-circuit layer.
 
     Parameters
@@ -122,14 +122,22 @@
         Device specific configuration, defines the compilation step from
         the quantum-circuit layer to the quantum-device layer description.
         Note, if a dictionary is passed, it will be parsed to a
         :class:`~DeviceCompilationConfig`.
 
     """
     if not isinstance(device_cfg, DeviceCompilationConfig):
+        # this is a special case to be supported to enable compilation for schedules
+        # that are defined completely at the quantum-device layer and require no
+        # circuit to device compilation.
+        # A better solution would be to omit skip this compile call in a backend,
+        # but this is supported for backwards compatibility reasons.
+        if device_cfg is None:
+            return schedule
+
         device_cfg = DeviceCompilationConfig.parse_obj(device_cfg)
 
     # to prevent the original input schedule from being modified.
     schedule = deepcopy(schedule)
 
     for operation in schedule.operations.values():
         # if operation is a valid pulse or acquisition it will not attempt to add
@@ -229,22 +237,22 @@
         operation=operation,
         operation_cfg=element_cfg[operation_type],
     )
 
 
 def _compile_two_qubits(operation, qubits, operation_type, device_cfg):
     parent_qubit, child_qubit = qubits
-    edge = f"{parent_qubit}-{child_qubit}"
+    edge = f"{parent_qubit}_{child_qubit}"
 
     symmetric_operation = operation.get("gate_info", {}).get("symmetric", False)
 
     if symmetric_operation:
         possible_permutations = permutations(qubits, 2)
         operable_edges = {
-            f"{permutation[0]}-{permutation[1]}"
+            f"{permutation[0]}_{permutation[1]}"
             for permutation in possible_permutations
         }
         valid_edge_list = list(operable_edges.intersection(device_cfg.edges))
         if len(valid_edge_list) == 1:
             edge = valid_edge_list[0]
         elif len(valid_edge_list) < 1:
             raise ConfigKeyError(
```

### Comparing `quantify-scheduler-0.8.0/quantify_scheduler/backends/corrections.py` & `quantify-scheduler-0.9.0/quantify_scheduler/backends/corrections.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,18 +7,42 @@
 import numpy as np
 
 from quantify_scheduler import Schedule
 from quantify_scheduler.backends.qblox import constants
 from quantify_scheduler.backends.qblox.helpers import generate_waveform_data
 from quantify_scheduler.helpers.importers import import_python_object_from_string
 from quantify_scheduler.operations.pulse_library import NumericalPulse
+from quantify_scheduler.structure import DataStructure
 
 
 logger = logging.getLogger(__name__)
 
+# pylint: disable=too-few-public-methods
+class LatencyCorrections(DataStructure):
+    """
+    A datastructure containing the information required to correct for latencies
+    on signals specified by port-clock combinations.
+
+    Note, if the port-clock combination of a signal is not specified in the latency
+    corrections, no correction will be applied.
+
+    Parameters
+    ----------
+    latencies
+        A dictionary specifying the latencies to be corrected for.
+        Keys are port-clocks combinations specifying the signal for which latency
+        should be corrected, e.g., `port=q0:mw` and `clock=q0.01` will have the
+        string ``"q0:mw-q0.01"`` as a key.
+        Values are latencies of the signal to be corrected for in seconds, e.g.,
+        if a signal has a latency of 120e-9, the signal will be shifted by
+        -120 ns to correct for this latency.
+    """
+
+    latencies: Dict[str, float]
+
 
 def distortion_correct_pulse(  # pylint: disable=too-many-arguments
     pulse_data: Dict[str, Any],
     sampling_rate: int,
     filter_func_name: str,
     input_var_name: str,
     kwargs_dict: Dict[str, Any],
```

### Comparing `quantify-scheduler-0.8.0/quantify_scheduler/backends/qblox/compiler_abc.py` & `quantify-scheduler-0.9.0/quantify_scheduler/backends/qblox/compiler_abc.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 import logging
 from abc import ABC, ABCMeta, abstractmethod
 from collections import defaultdict, deque
 from functools import partial
 from os import makedirs, path
 from typing import Any, Callable, Dict, List, Literal, Optional, Set, Tuple, Union
 
+import dataclasses
 from pathvalidate import sanitize_filename
 from qcodes.utils.helpers import NumpyJSONEncoder
 from quantify_core.data.handling import gen_tuid, get_datadir
 
 from quantify_scheduler.backends.qblox import (
     constants,
     driver_version_check,
@@ -36,14 +37,15 @@
     BaseModuleSettings,
     OpInfo,
     PulsarRFSettings,
     PulsarSettings,
     RFModuleSettings,
     SequencerSettings,
     StaticHardwareProperties,
+    MarkerConfiguration,
 )
 from quantify_scheduler.enums import BinMode
 from quantify_scheduler.helpers.schedule import (
     _extract_acquisition_metadata_from_acquisitions,
 )
 
 logger = logging.getLogger(__name__)
@@ -215,15 +217,15 @@
                 f"Attempting to add acquisition {repr(acq_info)} "
                 f"on port {port} with clock {clock}."
             )
 
         self._acquisitions[(port, clock)].append(acq_info)
 
     @property
-    def portclocks_with_data(self) -> Set[Tuple[str, str]]:
+    def _portclocks_with_data(self) -> Set[Tuple[str, str]]:
         """
         All the port-clock combinations associated with at least one pulse and/or
         acquisition.
 
         Returns
         -------
         :
@@ -231,14 +233,28 @@
             InstrumentCompiler.
         """
         portclocks_used = set()
         portclocks_used.update(self._pulses.keys())
         portclocks_used.update(self._acquisitions.keys())
         return portclocks_used
 
+    @property
+    def _portclocks_with_pulses(self) -> Set[Tuple[str, str]]:
+        """
+        All the port-clock combinations associated with at least one pulse.
+        Returns
+        -------
+        :
+            A set containing all the port-clock combinations that are used by this
+            InstrumentCompiler.
+        """
+        portclocks_used = set()
+        portclocks_used.update(self._pulses.keys())
+        return portclocks_used
+
     @abstractmethod
     def compile(self, repetitions: int = 1) -> Dict[str, Any]:
         """
         An abstract method that should be overridden by a subclass to implement the
         actual compilation. Method turns the pulses and acquisitions added to the device
         into device-specific instructions.
 
@@ -442,15 +458,15 @@
     def _generate_awg_dict(self) -> Dict[str, Any]:
         """
         Generates the dictionary that contains the awg waveforms in the
         format accepted by the driver.
 
         Notes
         -----
-        The final dictionary to be included in the json that is uploaded to the pulsar
+        The final dictionary to be included in the json that is uploaded to the module
         is of the form:
 
         .. code-block::
 
             program
             awg
                 waveform_name
@@ -481,15 +497,15 @@
     def _generate_weights_dict(self) -> Dict[str, Any]:
         """
         Generates the dictionary that corresponds that contains the acq weights
         waveforms in the format accepted by the driver.
 
         Notes
         -----
-        The final dictionary to be included in the json that is uploaded to the pulsar
+        The final dictionary to be included in the json that is uploaded to the module
         is of the form:
 
         .. code-block::
 
             program
             awg
                 waveform_name
@@ -550,15 +566,15 @@
         )
 
         # acquisition metadata for acquisitions relevant to this sequencer only
         acq_metadata = _extract_acquisition_metadata_from_acquisitions(
             acquisition_infos
         )
 
-        # initialize an empty dictionary for the format required by pulsar
+        # initialize an empty dictionary for the format required by module
         acq_declaration_dict = {}
         for acq_channel, acq_indices in acq_metadata.acq_indices.items():
 
             # Some sanity checks on the input for easier debugging.
             if min(acq_indices) != 0:
                 raise ValueError(
                     f"Please make sure the lowest bin index used is 0. "
@@ -1003,14 +1019,48 @@
             the hardware config.
         ValueError
             Raised when the same port-clock is multiply assigned in the hardware config.
         ValueError
             Attempting to use more sequencers than available.
 
         """
+        # Figure out which outputs need to be turned on.
+        marker_start_config = self.static_hw_properties.marker_configuration.start
+        for io, io_cfg in self.hw_mapping.items():
+            if (
+                not isinstance(io_cfg, dict)
+                or io not in self.static_hw_properties.valid_ios
+            ):
+                continue
+
+            portclock_configs: List[Dict[str, Any]] = io_cfg.get(
+                "portclock_configs", []
+            )
+            if not portclock_configs:
+                continue
+
+            for target in portclock_configs:
+                portclock = (target["port"], target["clock"])
+                if portclock in self._portclocks_with_pulses:
+                    output_map = (
+                        self.static_hw_properties.marker_configuration.output_map
+                    )
+                    if io in output_map:
+                        marker_start_config |= output_map[io]
+
+        updated_static_hw_properties = dataclasses.replace(
+            self.static_hw_properties,
+            marker_configuration=MarkerConfiguration(
+                init=self.static_hw_properties.marker_configuration.init,
+                start=marker_start_config,
+                end=self.static_hw_properties.marker_configuration.end,
+            ),
+        )
+
+        # Setup each sequencer.
         sequencers: Dict[str, Sequencer] = {}
         portclock_output_map: Dict[Tuple, str] = {}
 
         for io, io_cfg in self.hw_mapping.items():
             if not isinstance(io_cfg, dict):
                 continue
             if io not in self.static_hw_properties.valid_ios:
@@ -1031,22 +1081,22 @@
                 raise KeyError(
                     f"No 'portclock_configs' entry found in '{io}' of {self.name}."
                 )
 
             for target in portclock_configs:
                 portclock = (target["port"], target["clock"])
 
-                if portclock in self.portclocks_with_data:
+                if portclock in self._portclocks_with_data:
                     connected_outputs = helpers.output_name_to_outputs(io)
                     seq_idx = len(sequencers)
                     new_seq = Sequencer(
                         parent=self,
                         index=seq_idx,
                         portclock=portclock,
-                        static_hw_properties=self.static_hw_properties,
+                        static_hw_properties=updated_static_hw_properties,
                         connected_outputs=connected_outputs,
                         seq_settings=target,
                         latency_corrections=self.latency_corrections,
                         lo_name=lo_name,
                         downconverter_freq=downconverter_freq,
                     )
                     sequencers[new_seq.name] = new_seq
@@ -1071,15 +1121,15 @@
                 f"{self.static_hw_properties.max_sequencers}!"
             )
 
         return sequencers
 
     def distribute_data(self):
         """
-        Distributes the pulses and acquisitions assigned to this pulsar over the
+        Distributes the pulses and acquisitions assigned to this module over the
         different sequencers based on their portclocks. Raises an exception in case
         the device does not support acquisitions.
         """
 
         if len(self._acquisitions) > 0 and not self.supports_acquisition:
             raise RuntimeError(
                 f"Attempting to add acquisitions to {self.__class__} {self.name}, "
@@ -1138,17 +1188,24 @@
         Raises
         ------
         ValueError
             Neither the LO nor the IF frequency has been set and thus contain
             :code:`None` values.
         """
 
+    @abstractmethod
+    def assign_attenuation(self):
+        """
+        An abstract method that should be overridden. Meant to assign
+        attenuation settings from the hardware configuration if there is any.
+        """
+
     @staticmethod
     def downconvert_clock(downconverter_freq: float, clock_freq: float):
-        """ "
+        """
         Downconverts clock frequency.
 
         Parameters
         ----------
         downconverter_freq
             Frequency of the downconverter.
         clock_freq
@@ -1156,15 +1213,14 @@
 
         Raises
         ------
         ValueError
             When downconverter frequency is negative.
         ValueError
             When downconverter frequency is less than the clock frequency.
-        ------
         """
 
         if downconverter_freq == 0:
             return clock_freq
 
         if downconverter_freq < 0:
             raise ValueError("Downconverter frequency must be positive.")
@@ -1183,39 +1239,43 @@
         this means assigning the pulses and acquisitions to the sequencers and
         calculating the relevant frequencies in case an external local oscillator is
         used.
         """
         self._settings = self.settings_type.extract_settings_from_mapping(
             self.hw_mapping
         )
-        self._settings = self._configure_mixer_offsets(self._settings, self.hw_mapping)
+        self._settings = self._configure_mixer_offsets_and_gains(
+            self._settings, self.hw_mapping
+        )
         self.sequencers = self._construct_sequencers()
         self.distribute_data()
         self._determine_scope_mode_acquisition_sequencer()
         for seq in self.sequencers.values():
             self.assign_frequencies(seq)
+        self.assign_attenuation()
 
-    def _configure_mixer_offsets(
+    def _configure_mixer_offsets_and_gains(
         self, settings: BaseModuleSettings, hw_mapping: Dict[str, Any]
     ) -> BaseModuleSettings:
         """
-        We configure the mixer offsets after initializing the settings such we can
-        account for the differences in the hardware. e.g. the V vs mV encountered here.
+        We configure the mixer offsets, gains, attenuations
+        after initializing the settings such we can account for
+        the differences in the hardware. e.g. the V vs mV encountered here.
 
         Parameters
         ----------
         settings
-            The settings dataclass to which to add the dc offsets.
+            The settings dataclass to which to add the dc offsets and gains.
         hw_mapping
             The hardware configuration.
 
         Returns
         -------
         :
-            The settings dataclass after adding the normalized offsets
+            The settings dataclass after adding the normalized offsets and gains.
 
         Raises
         ------
         ValueError
             An offset was used outside of the allowed range.
         """
 
@@ -1269,14 +1329,26 @@
                 settings.offset_ch1_path0 = calc_from_units_volt(
                     "dc_mixer_offset_I", output_cfg
                 )
                 settings.offset_ch1_path1 = calc_from_units_volt(
                     "dc_mixer_offset_Q", output_cfg
                 )
 
+        complex_output_0 = hw_mapping.get("complex_output_0", None)
+        if complex_output_0 is not None:
+            settings.in0_gain = complex_output_0.get("input_gain_I", None)
+            settings.in1_gain = complex_output_0.get("input_gain_Q", None)
+        else:
+            settings.in0_gain = hw_mapping.get("real_output_0", {}).get(
+                "input_gain", None
+            )
+            settings.in1_gain = hw_mapping.get("real_output_1", {}).get(
+                "input_gain", None
+            )
+
         return settings
 
     @abstractmethod
     def update_settings(self):
         """
         Updates the settings to set all parameters that are determined by the
         compiler.
@@ -1314,27 +1386,27 @@
                     )
                 scope_acq_seq = seq.index
 
         self._settings.scope_mode_sequencer = scope_acq_seq
 
     def compile(self, repetitions: int = 1) -> Optional[Dict[str, Any]]:
         """
-        Performs the actual compilation steps for this pulsar, by calling the sequencer
+        Performs the actual compilation steps for this module, by calling the sequencer
         level compilation functions and combining them into a single dictionary. The
         compiled program has a settings key, and keys for every sequencer.
 
         Parameters
         ----------
         repetitions
             Number of times execution the schedule is repeated.
 
         Returns
         -------
         :
-            The compiled program corresponding to this pulsar. It contains an entry for
+            The compiled program corresponding to this module. It contains an entry for
             every sequencer and general "settings". If the device is not actually used,
             and an empty program is compiled, None is returned instead.
         """
         program = {}
         for seq_name, seq in self.sequencers.items():
             seq_program = seq.compile(repetitions=repetitions)
             if seq_program is not None:
@@ -1474,14 +1546,20 @@
         if lo_freq is not None:
             if_freq = clock_freq - lo_freq
             sequencer.frequency = if_freq
 
         if if_freq != 0 and if_freq is not None:
             sequencer.settings.nco_en = True
 
+    def assign_attenuation(self):
+        """
+        Meant to assign attenuation settings from the hardware configuration, if there
+        is any. For baseband modules there is no attenuation parameters currently.
+        """
+
 
 class QbloxRFModule(QbloxBaseModule):
     """
     Abstract class with all the shared functionality between the QRM-RF and QCM-RF
     modules.
     """
 
@@ -1566,14 +1644,28 @@
                     self._settings.lo0_freq = new_lo_freq
                 elif complex_output == 1:
                     self._settings.lo1_freq = new_lo_freq
 
             if lo_freq is not None:
                 sequencer.frequency = clock_freq - lo_freq
 
+    def assign_attenuation(self):
+        """
+        Assigns attenuation settings from the hardware configuration.
+        """
+        self._settings.in0_att = self.hw_mapping.get("complex_output_0", {}).get(
+            "input_att", None
+        )
+        self._settings.out0_att = self.hw_mapping.get("complex_output_0", {}).get(
+            "output_att", None
+        )
+        self._settings.out1_att = self.hw_mapping.get("complex_output_1", {}).get(
+            "output_att", None
+        )
+
     @classmethod
     def _validate_output_mode(cls, sequencer: Sequencer):
         if sequencer.output_mode != "complex":
             raise ValueError(
                 f"Attempting to use {cls.__name__} in real "
                 f"mode, but this is not supported for Qblox RF modules."
             )
```

### Comparing `quantify-scheduler-0.8.0/quantify_scheduler/backends/qblox/compiler_container.py` & `quantify-scheduler-0.9.0/quantify_scheduler/backends/qblox/compiler_container.py`

 * *Files identical despite different names*

### Comparing `quantify-scheduler-0.8.0/quantify_scheduler/backends/qblox/constants.py` & `quantify-scheduler-0.9.0/quantify_scheduler/backends/qblox/constants.py`

 * *Files identical despite different names*

### Comparing `quantify-scheduler-0.8.0/quantify_scheduler/backends/qblox/driver_version_check.py` & `quantify-scheduler-0.9.0/quantify_scheduler/backends/qblox/driver_version_check.py`

 * *Files identical despite different names*

### Comparing `quantify-scheduler-0.8.0/quantify_scheduler/backends/qblox/helpers.py` & `quantify-scheduler-0.9.0/quantify_scheduler/backends/qblox/helpers.py`

 * *Files identical despite different names*

### Comparing `quantify-scheduler-0.8.0/quantify_scheduler/backends/qblox/instrument_compilers.py` & `quantify-scheduler-0.9.0/quantify_scheduler/backends/qblox/instrument_compilers.py`

 * *Files 2% similar despite different names*

```diff
@@ -167,15 +167,23 @@
     """
 
     supports_acquisition: bool = False
     static_hw_properties: StaticHardwareProperties = StaticHardwareProperties(
         instrument_type="QCM-RF",
         max_sequencers=NUMBER_OF_SEQUENCERS_QCM,
         max_awg_output_voltage=0.25,
-        marker_configuration=MarkerConfiguration(init=0b0011, start=0b1111, end=0b0000),
+        marker_configuration=MarkerConfiguration(
+            init=0b0011,
+            start=0b1100,
+            end=0b0000,
+            output_map={
+                "complex_output_0": 0b0001,
+                "complex_output_1": 0b0010,
+            },
+        ),
         mixer_dc_offset_range=BoundedParameter(min_val=-50, max_val=50, units="mV"),
         valid_ios=[f"complex_output_{i}" for i in [0, 1]]
         + [f"real_output_{i}" for i in range(4)],
     )
 
 
 class QrmRfModule(compiler_abc.QbloxRFModule):
```

### Comparing `quantify-scheduler-0.8.0/quantify_scheduler/backends/qblox/operation_handling/acquisitions.py` & `quantify-scheduler-0.9.0/quantify_scheduler/backends/qblox/operation_handling/acquisitions.py`

 * *Files identical despite different names*

### Comparing `quantify-scheduler-0.8.0/quantify_scheduler/backends/qblox/operation_handling/base.py` & `quantify-scheduler-0.9.0/quantify_scheduler/backends/qblox/operation_handling/base.py`

 * *Files identical despite different names*

### Comparing `quantify-scheduler-0.8.0/quantify_scheduler/backends/qblox/operation_handling/factory.py` & `quantify-scheduler-0.9.0/quantify_scheduler/backends/qblox/operation_handling/factory.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,18 +48,15 @@
 def _get_acquisition_strategy(
     operation_info: OpInfo,
 ) -> acquisitions.AcquisitionStrategyPartial:
     """Handles the logic for determining the correct acquisition type."""
 
     protocol = operation_info.data["protocol"]
     if protocol in ("trace", "ssb_integration_complex"):
-        if (
-            protocol == "trace"
-            and operation_info.data["bin_mode"] == BinMode.APPEND.value
-        ):
+        if protocol == "trace" and operation_info.data["bin_mode"] == BinMode.APPEND:
             raise ValueError(
                 f"Trace acquisition does not support APPEND bin mode.\n\n"
                 f"{repr(operation_info)} caused this exception to occur."
             )
         return acquisitions.SquareAcquisitionStrategy(operation_info)
 
     if protocol == "weighted_integrated_complex":
```

### Comparing `quantify-scheduler-0.8.0/quantify_scheduler/backends/qblox/operation_handling/pulses.py` & `quantify-scheduler-0.9.0/quantify_scheduler/backends/qblox/operation_handling/pulses.py`

 * *Files identical despite different names*

### Comparing `quantify-scheduler-0.8.0/quantify_scheduler/backends/qblox/operation_handling/virtual.py` & `quantify-scheduler-0.9.0/quantify_scheduler/backends/qblox/operation_handling/virtual.py`

 * *Files identical despite different names*

### Comparing `quantify-scheduler-0.8.0/quantify_scheduler/backends/qblox/q1asm_instructions.py` & `quantify-scheduler-0.9.0/quantify_scheduler/backends/qblox/q1asm_instructions.py`

 * *Files identical despite different names*

### Comparing `quantify-scheduler-0.8.0/quantify_scheduler/backends/qblox/qasm_program.py` & `quantify-scheduler-0.9.0/quantify_scheduler/backends/qblox/qasm_program.py`

 * *Files identical despite different names*

### Comparing `quantify-scheduler-0.8.0/quantify_scheduler/backends/qblox/register_manager.py` & `quantify-scheduler-0.9.0/quantify_scheduler/backends/qblox/register_manager.py`

 * *Files identical despite different names*

### Comparing `quantify-scheduler-0.8.0/quantify_scheduler/backends/qblox_backend.py` & `quantify-scheduler-0.9.0/quantify_scheduler/backends/qblox_backend.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,15 +3,18 @@
 """Compiler backend for Qblox hardware."""
 from __future__ import annotations
 
 import warnings
 from typing import Any, Dict
 
 from quantify_scheduler import CompiledSchedule, Schedule
-from quantify_scheduler.backends.corrections import apply_distortion_corrections
+from quantify_scheduler.backends.corrections import (
+    apply_distortion_corrections,
+    LatencyCorrections,
+)
 from quantify_scheduler.backends.qblox import compiler_container, helpers
 
 
 def hardware_compile(
     schedule: Schedule, hardware_cfg: Dict[str, Any]
 ) -> CompiledSchedule:
     """
@@ -34,18 +37,25 @@
         The hardware configuration of the setup.
 
     Returns
     -------
     :
         The compiled schedule.
     """
+
     converted_hw_config = helpers.convert_hw_config_to_portclock_configs_spec(
         hardware_cfg
     )
 
+    if "latency_corrections" in converted_hw_config.keys():
+        # Important: currently only used to validate the input, should also be
+        # used for storing the latency corrections
+        # (see also https://gitlab.com/groups/quantify-os/-/epics/1)
+        LatencyCorrections(latencies=converted_hw_config["latency_corrections"])
+
     # Directly comparing dictionaries that contain numpy arrays raises a
     # ValueError. It is however sufficient to compare all the keys of nested
     # dictionaries.
     def _get_flattened_keys_from_dictionary(
         dictionary, parent_key: str = "", sep: str = "."
     ):
         flattened_keys = set()
```

### Comparing `quantify-scheduler-0.8.0/quantify_scheduler/backends/types/common.py` & `quantify-scheduler-0.9.0/quantify_scheduler/backends/types/common.py`

 * *Files identical despite different names*

### Comparing `quantify-scheduler-0.8.0/quantify_scheduler/backends/types/qblox.py` & `quantify-scheduler-0.9.0/quantify_scheduler/backends/types/qblox.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # Repository: https://gitlab.com/quantify-os/quantify-scheduler
 # Licensed according to the LICENCE file on the main branch
 """Python dataclasses for compilation to Qblox hardware."""
 
 from __future__ import annotations
 
 from dataclasses import dataclass
+from dataclasses import field as dataclasses_field
 from typing import Any, Dict, Optional, Tuple, Union, List
 
 from dataclasses_json import DataClassJsonMixin
 
 from quantify_scheduler.backends.qblox import constants
 
 
@@ -32,14 +33,18 @@
     init: Optional[int]
     """Value to set in the header before the wait sync."""
     start: Optional[int]
     """The setting set in the header at the start of the program (after the wait sync).
     """
     end: Optional[int]
     """Setting set in the footer at the end of the program."""
+    output_map: Dict[str, int] = dataclasses_field(default_factory=dict)
+    """A mapping from output name to marker setting.
+    Specifies which marker bit needs to be set at start if the
+    output (as a string ex. `complex_output_0`) contains a pulse."""
 
 
 @dataclass(frozen=True)
 class StaticHardwareProperties:
     """
     Specifies the fixed hardware properties needed in the backend.
     """
@@ -184,14 +189,18 @@
     """The DC offset on the path 0 of channel 0."""
     offset_ch0_path1: Union[float, None] = None
     """The DC offset on the path 1 of channel 0."""
     offset_ch1_path0: Union[float, None] = None
     """The DC offset on path 0 of channel 1."""
     offset_ch1_path1: Union[float, None] = None
     """The DC offset on path 1 of channel 1."""
+    in0_gain: Union[int, None] = None
+    """The gain of input 0."""
+    in1_gain: Union[int, None] = None
+    """The gain of input 1."""
 
 
 @dataclass
 class BasebandModuleSettings(BaseModuleSettings):
     """
     Settings for a baseband module.
 
@@ -262,14 +271,20 @@
 
     lo0_freq: Union[float, None] = None
     """The frequency of Output 0 (O0) LO. If left `None`, the parameter will not be set.
     """
     lo1_freq: Union[float, None] = None
     """The frequency of Output 1 (O1) LO. If left `None`, the parameter will not be set.
     """
+    out0_att: Union[int, None] = None
+    """The attenuation of Output 0."""
+    out1_att: Union[int, None] = None
+    """The attenuation of Output 1."""
+    in0_att: Union[int, None] = None
+    """The attenuation of Input 0."""
 
     @classmethod
     def extract_settings_from_mapping(
         cls, mapping: Dict[str, Any], **kwargs: Optional[dict]
     ) -> RFModuleSettings:
         """
         Factory method that takes all the settings defined in the mapping and generates
```

### Comparing `quantify-scheduler-0.8.0/quantify_scheduler/backends/types/zhinst.py` & `quantify-scheduler-0.9.0/quantify_scheduler/backends/types/zhinst.py`

 * *Files identical despite different names*

### Comparing `quantify-scheduler-0.8.0/quantify_scheduler/backends/zhinst/helpers.py` & `quantify-scheduler-0.9.0/quantify_scheduler/backends/zhinst/helpers.py`

 * *Files identical despite different names*

### Comparing `quantify-scheduler-0.8.0/quantify_scheduler/backends/zhinst/resolvers.py` & `quantify-scheduler-0.9.0/quantify_scheduler/backends/zhinst/resolvers.py`

 * *Files identical despite different names*

### Comparing `quantify-scheduler-0.8.0/quantify_scheduler/backends/zhinst/seqc_il_generator.py` & `quantify-scheduler-0.9.0/quantify_scheduler/backends/zhinst/seqc_il_generator.py`

 * *Files identical despite different names*

### Comparing `quantify-scheduler-0.8.0/quantify_scheduler/backends/zhinst/settings.py` & `quantify-scheduler-0.9.0/quantify_scheduler/backends/zhinst/settings.py`

 * *Files identical despite different names*

### Comparing `quantify-scheduler-0.8.0/quantify_scheduler/backends/zhinst_backend.py` & `quantify-scheduler-0.9.0/quantify_scheduler/backends/zhinst_backend.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,17 @@
 from functools import partial
 from typing import Any, Callable, Dict, Iterable, List, Optional, Tuple, Union, cast
 
 import numpy as np
 import pandas as pd
 from zhinst.toolkit.helpers import Waveform
 
+
 from quantify_scheduler import enums
+from quantify_scheduler.backends.corrections import LatencyCorrections
 from quantify_scheduler.backends.types import common, zhinst
 from quantify_scheduler.backends.zhinst import helpers as zi_helpers
 from quantify_scheduler.backends.zhinst import resolvers, seqc_il_generator
 from quantify_scheduler.backends.zhinst import settings as zi_settings
 from quantify_scheduler.helpers import waveforms as waveform_helpers
 from quantify_scheduler.helpers import schedule as schedule_helpers
 from quantify_scheduler.instrument_coordinator.components.generic import (
@@ -752,14 +754,20 @@
     ------
     NotImplementedError
         Thrown when using unsupported ZI Instruments.
     """
 
     _validate_schedule(schedule)
 
+    if "latency_corrections" in hardware_cfg.keys():
+        # Important: currently only used to validate the input, should also be
+        # used for storing the latency corrections
+        # (see also https://gitlab.com/groups/quantify-os/-/epics/1)
+        LatencyCorrections(latencies=hardware_cfg["latency_corrections"])
+
     ################################################
     # Timing table manipulation
     ################################################
 
     # the schedule has a Styled pandas dataframe as the return type.
     # here we want to manipulate the data directly so we extract the raw dataframe.
     timing_table = schedule.timing_table.data
@@ -1715,14 +1723,26 @@
                 output=output,
                 waveform=waveform,
                 start_and_duration_in_seconds=(0, row["duration"]),
                 instrument_info=instrument_info,
                 is_pulse=not row.is_acquisition,
             )
 
+            if len(corr_wf) > 4096:
+
+                raise ValueError(
+                    f"Attempting to set an integration weight of {len(corr_wf)} samples"
+                    " (>4096) corresponding to an integration time of "
+                    f"{len(corr_wf)/instrument_info.sample_rate*1e6} us. "
+                    "Please double check that your schedule does not contain any "
+                    "acquisitions with a duration longer than "
+                    f"{4096/instrument_info.sample_rate*1e6:.2f} us.\n"
+                    f'Offending operation: "{row["operation"]}"'
+                )
+
             numerical_wf_dict[row["waveform_id"]] = corr_wf
 
         else:
             waveform_info = operations_dict[row["operation"]]["pulse_info"][
                 row["wf_idx"]
             ]
             waveform = waveform_helpers.get_waveform(
```

### Comparing `quantify-scheduler-0.8.0/quantify_scheduler/compilation.py` & `quantify-scheduler-0.9.0/quantify_scheduler/compilation.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 # Repository: https://gitlab.com/quantify-os/quantify-scheduler
 # Licensed according to the LICENCE file on the main branch
 """Compiler for the quantify_scheduler."""
 import logging
 import warnings
 from copy import deepcopy
 from typing import Literal, Optional, Union
-
+from quantify_core.utilities import deprecated
 from quantify_scheduler.backends.circuit_to_device import DeviceCompilationConfig
+from quantify_scheduler.backends.graph_compilation import (
+    SimpleNodeConfig,
+    SerialCompilationConfig,
+)
 from quantify_scheduler.enums import BinMode
 from quantify_scheduler.helpers.importers import import_python_object_from_string
 from quantify_scheduler.json_utils import load_json_schema, validate_json
 from quantify_scheduler.operations.acquisition_library import (
     SSBIntegrationComplex,
     Trace,
 )
@@ -23,15 +27,15 @@
 from quantify_scheduler.resources import BasebandClockResource, ClockResource
 from quantify_scheduler.schedules.schedule import CompiledSchedule, Schedule
 
 logger = logging.getLogger(__name__)
 
 
 def determine_absolute_timing(
-    schedule: Schedule, time_unit: Literal["physical", "ideal"] = "physical"
+    schedule: Schedule, time_unit: Literal["physical", "ideal", None] = "physical"
 ) -> Schedule:
     """
     Determines the absolute timing of a schedule based on the timing constraints.
 
     This function determines absolute timings for every operation in the
     :attr:`~.ScheduleBase.schedulables`. It does this by:
 
@@ -42,27 +46,31 @@
 
     Parameters
     ----------
     schedule
         The schedule for which to determine timings.
     time_unit
         Whether to use physical units to determine the absolute time or ideal time.
-        When :code:`time_unit == 'physical'` the duration attribute is used.
-        When :code:`time_unit == 'ideal'` the duration attribute is ignored and treated
+        When :code:`time_unit == "physical"` the duration attribute is used.
+        When :code:`time_unit == "ideal"` the duration attribute is ignored and treated
         as if it is :code:`1`.
+        When :code:`time_unit == None` it will revert to :code:`"physical"`.
 
     Returns
     -------
     :
         a new schedule object where the absolute time for each operation has been
         determined.
     """
+
     if len(schedule.schedulables) == 0:
-        raise ValueError("schedule '{}' contains no schedulables".format(schedule.name))
+        raise ValueError(f"schedule '{schedule.name}' contains no schedulables.")
 
+    if time_unit is None:
+        time_unit = "physical"
     valid_time_units = ("physical", "ideal")
     if time_unit not in valid_time_units:
         raise ValueError(
             f"Undefined time_unit '{time_unit}'! Must be one of {valid_time_units}"
         )
 
     # iterate over the objects in the schedule.
@@ -93,17 +101,15 @@
                 t0 = ref_schedulable["abs_time"]
             elif t_constr["ref_pt"] == "center":
                 t0 = ref_schedulable["abs_time"] + duration_ref_op / 2
             elif t_constr["ref_pt"] == "end":
                 t0 = ref_schedulable["abs_time"] + duration_ref_op
             else:
                 raise NotImplementedError(
-                    'Timing "{}" not supported by backend'.format(
-                        ref_schedulable["abs_time"]
-                    )
+                    f'Timing "{ref_schedulable["abs_time"]}" not supported by backend.'
                 )
 
             duration_new_op = curr_op.duration if time_unit == "physical" else 1
 
             if t_constr["ref_pt_new"] == "start":
                 abs_time = t0 + t_constr["rel_time"]
             elif t_constr["ref_pt_new"] == "center":
@@ -116,21 +122,21 @@
         # update last_constraint and operation for next iteration of the loop
         last_schedulable = schedulable
         last_op = curr_op
 
     return schedule
 
 
-def _find_edge(device_cfg, q0, q1, op_name):
+def _find_edge(device_cfg, parent_element_name, child_element_name, op_name):
     try:
-        edge_cfg = device_cfg["edges"]["{}-{}".format(q0, q1)]
+        edge_cfg = device_cfg["edges"][f"{parent_element_name}_{child_element_name}"]
     except KeyError as e:
         raise ValueError(
-            f"Attempting operation '{op_name}' on qubits {q0} and {q1} which lack a"
-            " connective edge."
+            f"Attempting operation '{op_name}' on qubits {parent_element_name} "
+            f"and {child_element_name} which lack a connective edge."
         ) from e
     return edge_cfg
 
 
 def add_pulse_information_transmon(schedule: Schedule, device_cfg: dict) -> Schedule:
     # pylint: disable=line-too-long
     """
@@ -399,14 +405,19 @@
         True if valid
     """
     scheme = load_json_schema(__file__, scheme_fn)
     validate_json(config, scheme)
     return True
 
 
+@deprecated(
+    "0.9.0",
+    "Use the `QuantifyCompiler.compile` method instead. "
+    "See the user guide section on compilers for details.",
+)
 def qcompile(
     schedule: Schedule,
     device_cfg: Optional[Union[DeviceCompilationConfig, dict]] = None,
     hardware_cfg: Optional[dict] = None,
 ) -> CompiledSchedule:
     # pylint: disable=line-too-long
     """
@@ -436,26 +447,96 @@
 
     .. jsonschema:: https://gitlab.com/quantify-os/quantify-scheduler/-/raw/main/quantify_scheduler/schemas/transmon_cfg.json
 
     .. todo::
 
         Add a schema for the hardware config.
     """
+
+    def _construct_compilation_config_from_dev_hw_cfg(device_config, hardware_config):
+
+        compilation_passes = []
+
+        if isinstance(device_config, DeviceCompilationConfig):
+            compilation_passes.append(
+                SimpleNodeConfig(
+                    name="circuit_to_device",
+                    compilation_func=device_config.backend,
+                    compilation_options=device_config,
+                )
+            )
+        elif isinstance(device_config, dict):
+            # this is a deprecated config format. only legacy support here.
+            compilation_passes.append(
+                SimpleNodeConfig(
+                    name="add_pulse_information_transmon",
+                    compilation_func=device_config["backend"],
+                    compilation_options=device_config,
+                )
+            )
+        else:
+            # this is to support compiling when no device config is supplied
+            pass
+
+        compilation_passes.append(
+            SimpleNodeConfig(
+                name="determine_absolute_timing",
+                compilation_func="quantify_scheduler.compilation.determine_absolute_timing",
+            )
+        )
+
+        # If statements to support the different (currently unstructured) hardware
+        # configs.
+        if hardware_config is None:
+            backend_name = "Device compilation"
+        elif (
+            hardware_config["backend"]
+            == "quantify_scheduler.backends.qblox_backend.hardware_compile"
+        ):
+            backend_name = "Qblox backend"
+            compilation_passes.append(
+                SimpleNodeConfig(
+                    name="qblox_hardware_compile",
+                    compilation_func=hardware_config["backend"],
+                    compilation_options=hardware_config,
+                )
+            )
+        elif (
+            hardware_config["backend"]
+            == "quantify_scheduler.backends.zhinst_backend.compile_backend"
+        ):
+            backend_name = "Zhinst backend"
+            compilation_passes.append(
+                SimpleNodeConfig(
+                    name="zhinst_hardware_compile",
+                    compilation_func=hardware_config["backend"],
+                    compilation_options=hardware_config,
+                )
+            )
+
+        else:
+            raise NotImplementedError(
+                f"Hardware backend {hardware_config['backend']} not recognized"
+            )
+
+        compilation_config = SerialCompilationConfig(
+            name=backend_name, compilation_passes=compilation_passes
+        )
+        return compilation_config
+
+    compilation_config = _construct_compilation_config_from_dev_hw_cfg(
+        device_cfg, hardware_cfg
+    )
+
     # to prevent the original input schedule from being modified.
     schedule = deepcopy(schedule)
 
-    if device_cfg is not None:
-        schedule = device_compile(schedule=schedule, device_cfg=device_cfg)
-    else:
-        schedule = determine_absolute_timing(schedule=schedule, time_unit="physical")
-
-    if hardware_cfg is not None:
-        compiled_schedule = hardware_compile(schedule, hardware_cfg=hardware_cfg)
-    else:
-        compiled_schedule = CompiledSchedule(schedule)
+    backend_class = import_python_object_from_string(compilation_config.backend)
+    backend = backend_class(name=compilation_config.name)
+    compiled_schedule = backend.compile(schedule=schedule, config=compilation_config)
 
     return compiled_schedule
 
 
 def device_compile(
     schedule: Schedule, device_cfg: Union[DeviceCompilationConfig, dict]
 ) -> Schedule:
```

### Comparing `quantify-scheduler-0.8.0/quantify_scheduler/device_under_test/composite_square_edge.py` & `quantify-scheduler-0.9.0/quantify_scheduler/device_under_test/composite_square_edge.py`

 * *Files identical despite different names*

### Comparing `quantify-scheduler-0.8.0/quantify_scheduler/device_under_test/edge.py` & `quantify-scheduler-0.9.0/quantify_scheduler/device_under_test/edge.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     QuantumDevice. It provides an interface for the QuantumDevice to generate the
     edge information for use in the device compilation step. See
     :class:`quantify_scheduler.device_under_test.composite_square_edge` for an example
     edge implementation.
     """
 
     def __init__(self, parent_element_name: str, child_element_name: str):
-        edge_name = f"{parent_element_name}-{child_element_name}"
+        edge_name = f"{parent_element_name}_{child_element_name}"
         self._parent_element_name = parent_element_name
         self._child_element_name = child_element_name
         super().__init__(name=edge_name)
 
     @property
     def parent_device_element(self):
         """
```

### Comparing `quantify-scheduler-0.8.0/quantify_scheduler/device_under_test/quantum_device.py` & `quantify-scheduler-0.9.0/quantify_scheduler/device_under_test/quantum_device.py`

 * *Files 21% similar despite different names*

```diff
@@ -6,16 +6,20 @@
 
 from typing import Any, Dict
 
 from qcodes.instrument.base import Instrument
 from qcodes.instrument.parameter import InstrumentRefParameter, ManualParameter
 from qcodes.utils import validators
 
-from quantify_core.utilities import deprecated
 from quantify_scheduler.backends.circuit_to_device import DeviceCompilationConfig
+from quantify_scheduler.backends.graph_compilation import (
+    CompilationConfig,
+    SimpleNodeConfig,
+    SerialCompilationConfig,
+)
 from quantify_scheduler.device_under_test.device_element import DeviceElement
 from quantify_scheduler.device_under_test.edge import Edge
 
 
 class QuantumDevice(Instrument):
     """
     The QuantumDevice directly represents the device under test (DUT) and contains a
@@ -80,16 +84,84 @@
 
         self.add_parameter(
             "hardware_config",
             docstring="The hardware configuration file used for compiling from the "
             "quantum-device layer to a hardware backend.",
             parameter_class=ManualParameter,
             vals=validators.Dict(),
+            initial_value=None,
         )
 
+    def generate_compilation_config(self) -> CompilationConfig:
+        """
+        Generates a compilation config for use with a
+        :class:`~.graph_compilation.QuantifyCompiler`.
+        """
+
+        # Part that is always the same
+        dev_cfg = self.generate_device_config()
+        compilation_passes = [
+            SimpleNodeConfig(
+                name="circuit_to_device",
+                compilation_func=dev_cfg.backend,
+                compilation_options=dev_cfg,
+            ),
+            SimpleNodeConfig(
+                name="determine_absolute_timing",
+                compilation_func="quantify_scheduler.compilation."
+                + "determine_absolute_timing",
+            ),
+        ]
+
+        # If statements to support the different (currently unstructured) hardware
+        # configs.
+        hardware_config = self.generate_hardware_config()
+        if hardware_config is None:
+            backend_name = "Device compiler"
+        elif (
+            hardware_config["backend"]
+            == "quantify_scheduler.backends.qblox_backend.hardware_compile"
+        ):
+            backend_name = "Qblox compiler"
+            compilation_passes.append(
+                SimpleNodeConfig(
+                    name="qblox_hardware_compile",
+                    compilation_func=hardware_config["backend"],
+                    compilation_options=hardware_config,
+                )
+            )
+        elif (
+            hardware_config["backend"]
+            == "quantify_scheduler.backends.zhinst_backend.compile_backend"
+        ):
+            backend_name = "Zhinst compiler"
+            compilation_passes.append(
+                SimpleNodeConfig(
+                    name="zhinst_hardware_compile",
+                    compilation_func=hardware_config["backend"],
+                    compilation_options=hardware_config,
+                )
+            )
+
+        else:
+            backend_name = "Custom compiler"
+            compilation_passes.append(
+                SimpleNodeConfig(
+                    name="custom_hardware_compile",
+                    compilation_func=hardware_config["backend"],
+                    compilation_options=hardware_config,
+                )
+            )
+
+        compilation_config = SerialCompilationConfig(
+            name=backend_name, compilation_passes=compilation_passes
+        )
+
+        return compilation_config
+
     def generate_hardware_config(self) -> Dict[str, Any]:
         """
         Generates a valid hardware configuration describing the quantum device.
 
         Returns
         -------
             The hardware configuration file used for compiling from the quantum-device
@@ -251,24 +323,7 @@
         Parameters
         ----------
         edge_name
             The edge name.
         """
 
         self.edges().remove(edge_name)  # list gets updated in place
-
-    @property
-    @deprecated("0.8", "Consider replacing with elements")
-    def components(self):
-        return self.elements
-
-    @deprecated("0.8", "Consider replacing with get_element.")
-    def get_component(self, name: str) -> Instrument:
-        return self.get_element(name=name)
-
-    @deprecated("0.8", "Consider replacing with add_element.")
-    def add_component(self, component: DeviceElement) -> None:
-        self.add_element(element=component)
-
-    @deprecated("0.8", "Consider replacing with remove_element.")
-    def remove_component(self, name: str) -> None:
-        self.remove_element(name=name)
```

### Comparing `quantify-scheduler-0.8.0/quantify_scheduler/device_under_test/transmon_element.py` & `quantify-scheduler-0.9.0/quantify_scheduler/device_under_test/transmon_element.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # Repository: https://gitlab.com/quantify-os/quantify-scheduler
 # Licensed according to the LICENCE file on the main branch
 from typing import Dict, Any
 
-from qcodes.instrument.base import Instrument
 from qcodes.instrument import InstrumentChannel
 from qcodes.instrument.base import InstrumentBase
 from quantify_core.utilities import deprecated
 from qcodes.instrument.parameter import (
     InstrumentRefParameter,
     ManualParameter,
     Parameter,
@@ -191,27 +190,34 @@
             unit="#",
             parameter_class=ManualParameter,
             vals=validators.Ints(min_value=0),
         )
 
         self.add_parameter(
             "acq_delay",
-            docstring="Delay between the start of the readout pulse and the start of the acquisition.",
-            initial_value=0,
+            docstring="Delay between the start of the readout pulse and the start of "
+            + "the acquisition. Note that some hardware backends do not support "
+            "starting a pulse and the acquisition in the same clock cycle making 0 "
+            "delay an invalid value.",
+            initial_value=0,  # float("nan"),
             unit="s",
             parameter_class=ManualParameter,
-            vals=validators.Numbers(min_value=0, max_value=1),
+            # in principle the values should be a few 100 ns but the validator is here
+            # only to protect against silly typos that lead to out of memory errors.
+            vals=validators.Numbers(min_value=0, max_value=100e-6),
         )
         self.add_parameter(
             "integration_time",
             docstring="Integration time for the readout acquisition.",
             initial_value=1e-6,
             unit="s",
             parameter_class=ManualParameter,
-            vals=validators.Numbers(min_value=0, max_value=1),
+            # in principle the values should be a few us but the validator is here
+            # only to protect against silly typos that lead to out of memory errors.
+            vals=validators.Numbers(min_value=0, max_value=100e-6),
         )
 
         ro_acq_weight_type_validator = validators.Enum("SSB")
         self.add_parameter(
             "acq_weight_type",
             initial_value="SSB",
             parameter_class=ManualParameter,
```

### Comparing `quantify-scheduler-0.8.0/quantify_scheduler/enums.py` & `quantify-scheduler-0.9.0/quantify_scheduler/enums.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,24 @@
 # Repository: https://gitlab.com/quantify-os/quantify-scheduler
 # Licensed according to the LICENCE file on the main branch
 """Enums for quantify-scheduler."""
 
 from enum import Enum, unique
 
 
+class StrEnum(Enum):
+    """
+    This class functions to include explicit string serialization without adding `str`
+    as a base class.
+    """
+
+    def __str__(self):
+        return self.value
+
+
 @unique
 class SignalModeType(str, Enum):
 
     """
     The signal output enum type.
 
     Used to set the output signal type to a
@@ -51,15 +61,15 @@
 
     NONE = "none"
     PREMODULATE = "premod"
     MODULATE = "modulate"
 
 
 @unique
-class BinMode(str, Enum):
+class BinMode(StrEnum):
 
     """
     The acquisition protocol bin mode enum type.
 
     Used to set the bin type to
     append or average respectively.
```

### Comparing `quantify-scheduler-0.8.0/quantify_scheduler/gettables.py` & `quantify-scheduler-0.9.0/quantify_scheduler/gettables.py`

 * *Files 9% similar despite different names*

```diff
@@ -24,16 +24,16 @@
 import numpy as np
 from qcodes import Parameter
 from qcodes.utils.helpers import NumpyJSONEncoder
 
 from quantify_core.data.handling import gen_tuid, get_datadir, snapshot
 
 from quantify_scheduler import Schedule
-from quantify_scheduler.compilation import qcompile
 from quantify_scheduler.device_under_test.quantum_device import QuantumDevice
+from quantify_scheduler.helpers.importers import import_python_object_from_string
 from quantify_scheduler.enums import BinMode
 from quantify_scheduler.helpers.schedule import (
     extract_acquisition_metadata_from_schedule,
     AcquisitionMetadata,
 )
 
 logger = logging.getLogger(__name__)
@@ -151,37 +151,47 @@
         self.schedule_function = schedule_function
         self.schedule_kwargs = schedule_kwargs
         self._evaluated_sched_kwargs = {}
 
         # the quantum device object containing setup configuration information
         self.quantum_device = quantum_device
 
+        # The backend used for compilation. Available as a private variable
+        # to facilitate debugging. Will be assigned upon compilation in self.initialize
+        self._backend = None
+
     def __call__(self) -> Union[Tuple[float, ...], Tuple[np.ndarray, ...]]:
         """Acquire and return data"""
         return self.get()
 
+    def _compile(self, sched):
+        """Compile schedule, separated to allow for profiling compilation duration."""
+        compilation_config = self.quantum_device.generate_compilation_config()
+
+        # made into a private variable for debugging and future caching functionality
+        backend_class = import_python_object_from_string(compilation_config.backend)
+        self._backend = backend_class(name=compilation_config.name)
+        self._compiled_schedule = self._backend.compile(
+            schedule=sched, config=compilation_config
+        )
+
     def initialize(self):
         """
         This generates the schedule and uploads the compiled instructions to the
         hardware using the instrument coordinator.
         """
         logger.debug("Initializing schedule gettable.")
         self._evaluated_sched_kwargs = _evaluate_parameter_dict(self.schedule_kwargs)
 
         # generate a schedule using the evaluated keyword arguments dict
         sched = self.schedule_function(
             **self._evaluated_sched_kwargs,
             repetitions=self.quantum_device.cfg_sched_repetitions(),
         )
-
-        self._compiled_schedule = qcompile(
-            schedule=sched,
-            device_cfg=self.quantum_device.generate_device_config(),
-            hardware_cfg=self.quantum_device.generate_hardware_config(),
-        )
+        self._compile(sched)
 
         instr_coordinator = self.quantum_device.instr_instrument_coordinator.get_instr()
         instr_coordinator.prepare(self._compiled_schedule)
 
         self.is_initialized = True
 
     @property
```

### Comparing `quantify-scheduler-0.8.0/quantify_scheduler/helpers/collections.py` & `quantify-scheduler-0.9.0/quantify_scheduler/helpers/collections.py`

 * *Files identical despite different names*

### Comparing `quantify-scheduler-0.8.0/quantify_scheduler/helpers/importers.py` & `quantify-scheduler-0.9.0/quantify_scheduler/helpers/importers.py`

 * *Files identical despite different names*

### Comparing `quantify-scheduler-0.8.0/quantify_scheduler/helpers/inspect.py` & `quantify-scheduler-0.9.0/quantify_scheduler/helpers/inspect.py`

 * *Files identical despite different names*

### Comparing `quantify-scheduler-0.8.0/quantify_scheduler/helpers/mock_instruments.py` & `quantify-scheduler-0.9.0/quantify_scheduler/helpers/mock_instruments.py`

 * *Files identical despite different names*

### Comparing `quantify-scheduler-0.8.0/quantify_scheduler/helpers/schedule.py` & `quantify-scheduler-0.9.0/quantify_scheduler/helpers/schedule.py`

 * *Files identical despite different names*

### Comparing `quantify-scheduler-0.8.0/quantify_scheduler/helpers/time.py` & `quantify-scheduler-0.9.0/quantify_scheduler/helpers/time.py`

 * *Files identical despite different names*

### Comparing `quantify-scheduler-0.8.0/quantify_scheduler/helpers/validators.py` & `quantify-scheduler-0.9.0/quantify_scheduler/helpers/validators.py`

 * *Files identical despite different names*

### Comparing `quantify-scheduler-0.8.0/quantify_scheduler/helpers/waveforms.py` & `quantify-scheduler-0.9.0/quantify_scheduler/helpers/waveforms.py`

 * *Files identical despite different names*

### Comparing `quantify-scheduler-0.8.0/quantify_scheduler/instrument_coordinator/__init__.py` & `quantify-scheduler-0.9.0/quantify_scheduler/instrument_coordinator/__init__.py`

 * *Files identical despite different names*

### Comparing `quantify-scheduler-0.8.0/quantify_scheduler/instrument_coordinator/components/base.py` & `quantify-scheduler-0.9.0/quantify_scheduler/instrument_coordinator/components/base.py`

 * *Files identical despite different names*

### Comparing `quantify-scheduler-0.8.0/quantify_scheduler/instrument_coordinator/components/generic.py` & `quantify-scheduler-0.9.0/quantify_scheduler/instrument_coordinator/components/generic.py`

 * *Files identical despite different names*

### Comparing `quantify-scheduler-0.8.0/quantify_scheduler/instrument_coordinator/components/qblox.py` & `quantify-scheduler-0.9.0/quantify_scheduler/instrument_coordinator/components/qblox.py`

 * *Files 1% similar despite different names*

```diff
@@ -585,14 +585,19 @@
             self._set_parameter(
                 self.instrument, "out0_offset", settings.offset_ch0_path0
             )
         if settings.offset_ch0_path1 is not None:
             self._set_parameter(
                 self.instrument, "out1_offset", settings.offset_ch0_path1
             )
+        # configure gain
+        if settings.in0_gain is not None:
+            self._set_parameter(self.instrument, "in0_gain", settings.in0_gain)
+        if settings.in1_gain is not None:
+            self._set_parameter(self.instrument, "in1_gain", settings.in1_gain)
 
     def _configure_sequencer_settings(
         self, seq_idx: int, settings: SequencerSettings
     ) -> None:
         super()._configure_sequencer_settings(seq_idx, settings)
         if settings.integration_length_acq is not None:
             self._set_parameter(
@@ -642,14 +647,19 @@
             self._set_parameter(
                 self.instrument, "out1_offset_path0", settings.offset_ch1_path0
             )
         if settings.offset_ch1_path1 is not None:
             self._set_parameter(
                 self.instrument, "out1_offset_path1", settings.offset_ch1_path1
             )
+        # configure attenuation
+        if settings.out0_att is not None:
+            self._set_parameter(self.instrument, "out0_att", settings.out0_att)
+        if settings.out1_att is not None:
+            self._set_parameter(self.instrument, "out1_att", settings.out1_att)
 
 
 class QRMRFComponent(QRMComponent):
     """
     QRM-RF specific InstrumentCoordinator component.
     """
 
@@ -679,14 +689,19 @@
             self._set_parameter(
                 self.instrument, "out0_offset_path0", settings.offset_ch0_path0
             )
         if settings.offset_ch0_path1 is not None:
             self._set_parameter(
                 self.instrument, "out0_offset_path1", settings.offset_ch0_path1
             )
+        # configure gain and attenuation
+        if settings.out0_att is not None:
+            self._set_parameter(self.instrument, "out0_att", settings.out0_att)
+        if settings.in0_att is not None:
+            self._set_parameter(self.instrument, "in0_att", settings.in0_att)
 
 
 class PulsarQCMComponent(QCMComponent):
     """A component for a baseband Pulsar QCM."""
 
     def prepare(self, options: Dict[str, dict]) -> None:
         super().prepare(options)
@@ -814,15 +829,15 @@
                         i_vals[acq_idx::acq_stride],
                         q_vals[acq_idx::acq_stride],
                     )
 
         return formatted_acquisitions
 
     def _store_scope_acquisition(self):
-        sequencer_index = self.seq_name_to_idx_map.get(self.scope_mode_sequencer)
+        sequencer_index = self.scope_mode_sequencer
 
         if sequencer_index is None:
             return
 
         if sequencer_index > self.number_of_sequencers:
             raise ValueError(
                 f"Attempting to retrieve scope mode data from sequencer "
```

### Comparing `quantify-scheduler-0.8.0/quantify_scheduler/instrument_coordinator/components/zhinst.py` & `quantify-scheduler-0.9.0/quantify_scheduler/instrument_coordinator/components/zhinst.py`

 * *Files identical despite different names*

### Comparing `quantify-scheduler-0.8.0/quantify_scheduler/instrument_coordinator/instrument_coordinator.py` & `quantify-scheduler-0.9.0/quantify_scheduler/instrument_coordinator/instrument_coordinator.py`

 * *Files identical despite different names*

### Comparing `quantify-scheduler-0.8.0/quantify_scheduler/instrument_coordinator/utility.py` & `quantify-scheduler-0.9.0/quantify_scheduler/instrument_coordinator/utility.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,27 +29,34 @@
     -------
     Parameter:
 
     """
     root_param = instrument
     split_params = nested_parameter_name.split(".")
 
+    def _search_next_level(child_parameter_name, root_attr_dicts_list):
+        for root_attr_dict in root_attr_dicts_list:
+            if callable(child_parameter_name):
+                return child_parameter_name
+            if child_parameter_name in root_attr_dict:
+                return root_attr_dict.get(child_parameter_name)
+
+        return None
+
     # Search for the parameter within the parameter, function
     # or submodule delegate_attrs_dict of the instrument
     for child_parameter_name in split_params:
         root_attr_dicts_list = [
             root_param.parameters,
             root_param.submodules,
             root_param.functions,
         ]
-        for root_attr_dict in root_attr_dicts_list:
-            if child_parameter_name in root_attr_dict:
-                root_param = root_attr_dict.get(child_parameter_name)
-            if callable(child_parameter_name):
-                root_param = child_parameter_name
+        root_param = _search_next_level(child_parameter_name, root_attr_dicts_list)
+        if root_param is None:
+            break
 
     if not (isinstance(root_param, Parameter) or callable(root_param)):
         raise ValueError(
             f"Could not find settable parameter "
             f'"{nested_parameter_name}" in instrument "{instrument}"'
         )
```

### Comparing `quantify-scheduler-0.8.0/quantify_scheduler/json_utils.py` & `quantify-scheduler-0.9.0/quantify_scheduler/json_utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # Repository: https://gitlab.com/quantify-os/quantify-scheduler
 # Licensed according to the LICENCE file on the main branch
 """Module containing quantify JSON utilities."""
 from __future__ import annotations
 
-import ast
 import functools
 import json
 import pathlib
-import re
 import sys
 from types import ModuleType
 from typing import Any, Callable, Dict, List, Type, Union
 
 import fastjsonschema
+import numpy as np
 
 from quantify_scheduler.helpers import inspect as inspect_helpers
+from quantify_scheduler import enums
 
 current_python_version = sys.version_info
 
 lru_cache = functools.lru_cache(maxsize=200)
 
 
 def validate_json(data, schema):
@@ -148,27 +148,46 @@
         # pylint: disable=import-outside-toplevel
         from quantify_scheduler import resources
         from quantify_scheduler.schedules.schedule import (
             AcquisitionMetadata,
             Schedulable,
         )
         from quantify_scheduler.operations import (  # pylint: disable=import-outside-toplevel
+            operation,
             acquisition_library,
             gate_library,
             pulse_library,
         )
 
         self._modules: List[ModuleType] = [
+            enums,
+            operation,
             gate_library,
             pulse_library,
             acquisition_library,
             resources,
         ] + extended_modules
         self.classes = inspect_helpers.get_classes(*self._modules)
         self.classes.update({c.__name__: c for c in [AcquisitionMetadata, Schedulable]})
+        self.classes.update(
+            {
+                t.__name__: t
+                for t in [
+                    complex,
+                    float,
+                    int,
+                    bool,
+                    str,
+                    np.ndarray,
+                    np.complex128,
+                    np.int32,
+                    np.int64,
+                ]
+            }
+        )
 
     def decode_dict(self, obj: Dict[str, Any]) -> Dict[str, Any]:
         """
         Returns the deserialized JSON dictionary.
 
         Parameters
         ----------
@@ -181,68 +200,25 @@
             The deserialized result.
         """
         # If "deserialization_type" is present in `obj` it means the object was
         # serialized using `__getstate__` and should be deserialized using
         # `__setstate__`.
         if "deserialization_type" in obj:
             class_type: Type = self.classes[obj["deserialization_type"]]
+            if "mode" in obj and obj["mode"] == "__init__":
+                if class_type == np.ndarray:
+                    return np.array(obj["data"])
+                return class_type(obj["data"])
+            if "mode" in obj and obj["mode"] == "type":
+                return class_type
             new_obj = class_type.__new__(class_type)
             new_obj.__setstate__(obj)
             return new_obj
-
-        # Otherwise, check if serialization happened using `repr` and deserialize
-        # accordingly.
-        for key in obj:
-            value = obj[key]
-            if isinstance(value, str):
-                # Check if the string has a signature of a constructor
-                # example: Reset('q0', data={...})
-                if not re.match(r"^(\w+)\(.*\)$", value):
-                    return obj
-                obj[key] = self.decode_quantify_type(value)
         return obj
 
-    def decode_quantify_type(self, obj: str) -> object:
-        """
-        Returns the deserialized result of a possible known type stored in the
-        :class:`~.ScheduleJSONDecoder` .classes property.
-
-        For better security the usage of `eval` has been replaced in favour of
-        :func:`ast.literal_eval`.
-
-        Parameters
-        ----------
-        obj
-            The value of dictionary pair to deserialize.
-
-        Returns
-        -------
-        :
-            The decoded result.
-        """
-        kwargs = dict()
-        args = list()
-        ast_tree = ast.parse(obj)
-        class_name: str = ""
-        for node in ast.walk(ast_tree):
-            if isinstance(node, ast.Load):
-                break
-            if isinstance(node, ast.Call):
-                class_name = node.func.id
-            elif isinstance(node, ast.Constant):
-                args.append(node.value)
-            elif isinstance(node, ast.keyword):
-                kwargs[node.arg] = ast.literal_eval(node.value)
-
-        if class_name not in self.classes:
-            return obj
-
-        class_type: type = self.classes[class_name]
-        return class_type(*args, **kwargs)
-
     def custom_object_hook(self, obj: object) -> object:
         """
         The `object_hook` hook will be called with the result of every JSON object
         decoded and its return value will be used in place of the given ``dict``.
 
         Parameters
         ----------
@@ -268,24 +244,38 @@
     def default(self, o):
         """
         Overloads the json.JSONEncoder default method that returns a serializable
         object. It will try 3 different serialization methods which are, in order,
         check if the object is to be serialized to a string using repr. If not, try
         to use `__getstate__`. Finally, try to serialize the `__dict__` property.
         """
-        # Use local import to void Error('Operation' from partially initialized module
-        # 'quantify_scheduler')
-        from quantify_scheduler import (  # pylint: disable=import-outside-toplevel
-            Operation,
-            Schedulable,
-            resources,
-        )
-
-        if isinstance(o, (Operation, resources.Resource, Schedulable)):
-            return repr(o)
         if hasattr(o, "__getstate__"):
             return o.__getstate__()
+        if isinstance(o, (complex, np.int32, np.complex128, np.int64, enums.BinMode)):
+            return {
+                "deserialization_type": type(o).__name__,
+                "mode": "__init__",
+                "data": str(o),
+            }
+        if isinstance(o, (np.ndarray,)):
+            return {
+                "deserialization_type": type(o).__name__,
+                "mode": "__init__",
+                "data": list(o),
+            }
+        if o in [
+            complex,
+            float,
+            int,
+            bool,
+            str,
+            np.ndarray,
+            np.complex128,
+            np.int32,
+            np.int64,
+        ]:
+            return {"deserialization_type": o.__name__, "mode": "type"}
         if hasattr(o, "__dict__"):
             return o.__dict__
 
         # Let the base class default method raise the TypeError
         return json.JSONEncoder.default(self, o)
```

### Comparing `quantify-scheduler-0.8.0/quantify_scheduler/math.py` & `quantify-scheduler-0.9.0/quantify_scheduler/math.py`

 * *Files identical despite different names*

### Comparing `quantify-scheduler-0.8.0/quantify_scheduler/operations/acquisition_library.py` & `quantify-scheduler-0.9.0/quantify_scheduler/operations/acquisition_library.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Repository: https://gitlab.com/quantify-os/quantify-scheduler
 # Licensed according to the LICENCE file on the main branch
 # pylint: disable=too-many-arguments
 """Standard acquisition protocols for use with the quantify_scheduler."""
 
 from typing import Any, Dict, List, Optional, Union
+import warnings
 
 import numpy as np
 
 from quantify_scheduler import Operation
 from quantify_scheduler.enums import BinMode
 
 
@@ -69,39 +70,50 @@
         t0 :
             The acquisition start time in seconds, by default 0
         data :
             The operation's dictionary, by default None
             Note: if the data parameter is not None all other parameters are
             overwritten using the contents of data.
         """
-
         if data is None:
             if not isinstance(duration, float):
                 duration = float(duration)
             if isinstance(bin_mode, str):
                 bin_mode = BinMode(bin_mode)
 
-            data = {
-                "name": "Trace",
-                "acquisition_info": [
-                    {
-                        "waveforms": [],
-                        "duration": duration,
-                        "t0": t0,
-                        "port": port,
-                        "clock": clock,
-                        "acq_channel": acq_channel,
-                        "acq_index": acq_index,
-                        "bin_mode": bin_mode,
-                        "protocol": "trace",
-                        "acq_return_type": np.ndarray,
-                    }
-                ],
-            }
-        super().__init__(name=data["name"], data=data)
+            super().__init__(name="Trace")
+            self.data.update(
+                {
+                    "name": "Trace",
+                    "acquisition_info": [
+                        {
+                            "waveforms": [],
+                            "duration": duration,
+                            "t0": t0,
+                            "port": port,
+                            "clock": clock,
+                            "acq_channel": acq_channel,
+                            "acq_index": acq_index,
+                            "bin_mode": bin_mode,
+                            "protocol": "trace",
+                            "acq_return_type": np.ndarray,
+                        }
+                    ],
+                }
+            )
+            self._update()
+        else:
+            warnings.warn(
+                "Support for the data argument will be dropped in"
+                "quantify-scheduler >= 0.13.0.\n"
+                "Please consider updating the data "
+                "dictionary after initialization.",
+                DeprecationWarning,
+            )
+            super().__init__(name=data["name"], data=data)
 
     def __str__(self) -> str:
         acq_info = self.data["acquisition_info"][0]
         return self._get_signature(acq_info)
 
 
 class WeightedIntegratedComplex(
@@ -186,38 +198,55 @@
         NotImplementedError
         """
         if phase != 0:
             # Because of how clock interfaces were changed.
             raise NotImplementedError("Non-zero phase not yet implemented")
 
         if data is None:
-            data = {
-                "name": "WeightedIntegrationComplex",
-                "acquisition_info": [
-                    {
-                        "waveforms": [waveform_a, waveform_b],
-                        "t0": t0,
-                        "clock": clock,
-                        "port": port,
-                        "duration": duration,
-                        "phase": phase,
-                        "acq_channel": acq_channel,
-                        "acq_index": acq_index,
-                        "bin_mode": bin_mode,
-                        "protocol": "weighted_integrated_complex",
-                        "acq_return_type": complex,
-                    }
-                ],
-            }
-        # certain fields are required in the acquisition data
-        if "acq_return_type" not in data["acquisition_info"][0]:
-            data["acquisition_info"][0]["acq_return_type"] = complex
-            data["acquisition_info"][0]["protocol"] = "weighted_integrated_complex"
+            super().__init__(name="WeightedIntegrationComplex")
+            self.data.update(
+                {
+                    "name": "WeightedIntegrationComplex",
+                    "acquisition_info": [
+                        {
+                            "waveforms": [waveform_a, waveform_b],
+                            "t0": t0,
+                            "clock": clock,
+                            "port": port,
+                            "duration": duration,
+                            "phase": phase,
+                            "acq_channel": acq_channel,
+                            "acq_index": acq_index,
+                            "bin_mode": bin_mode,
+                            "protocol": "weighted_integrated_complex",
+                            "acq_return_type": complex,
+                        }
+                    ],
+                }
+            )
+            self._update()
+            # certain fields are required in the acquisition data
+            if "acq_return_type" not in self.data["acquisition_info"][0]:
+                self.data["acquisition_info"][0]["acq_return_type"] = complex
+                self.data["acquisition_info"][0][
+                    "protocol"
+                ] = "weighted_integrated_complex"
+        else:
+            warnings.warn(
+                "Support for the data argument will be dropped in"
+                "quantify-scheduler >= 0.13.0.\n"
+                "Please consider updating the data "
+                "dictionary after initialization.",
+                DeprecationWarning,
+            )
+            if "acq_return_type" not in data["acquisition_info"][0]:
+                data["acquisition_info"][0]["acq_return_type"] = complex
+                data["acquisition_info"][0]["protocol"] = "weighted_integrated_complex"
 
-        super().__init__(name=data["name"], data=data)
+            super().__init__(name=data["name"], data=data)
 
     def __str__(self) -> str:
         acq_info = self.data["acquisition_info"][0]
         return self._get_signature(acq_info)
 
 
 class SSBIntegrationComplex(AcquisitionOperation):  # pylint: disable=too-many-ancestors
@@ -298,38 +327,52 @@
         }
 
         if phase != 0:
             # Because of how clock interfaces were changed.
             raise NotImplementedError("Non-zero phase not yet implemented")
 
         if data is None:
-            data = {
-                "name": "SSBIntegrationComplex",
-                "acquisition_info": [
-                    {
-                        "waveforms": [waveform_i, waveform_q],
-                        "t0": t0,
-                        "clock": clock,
-                        "port": port,
-                        "duration": duration,
-                        "phase": phase,
-                        "acq_channel": acq_channel,
-                        "acq_index": acq_index,
-                        "bin_mode": bin_mode,
-                        "acq_return_type": complex,
-                        "protocol": "ssb_integration_complex",
-                    }
-                ],
-            }
-        # certain fields are required in the acquisition data
-        if "acq_return_type" not in data["acquisition_info"][0]:
-            data["acquisition_info"][0]["acq_return_type"] = complex
-            data["acquisition_info"][0]["protocol"] = "ssb_integration_complex"
-
-        super().__init__(name=data["name"], data=data)
+            super().__init__(name="SSBIntegrationComplex")
+            self.data.update(
+                {
+                    "name": "SSBIntegrationComplex",
+                    "acquisition_info": [
+                        {
+                            "waveforms": [waveform_i, waveform_q],
+                            "t0": t0,
+                            "clock": clock,
+                            "port": port,
+                            "duration": duration,
+                            "phase": phase,
+                            "acq_channel": acq_channel,
+                            "acq_index": acq_index,
+                            "bin_mode": bin_mode,
+                            "acq_return_type": complex,
+                            "protocol": "ssb_integration_complex",
+                        }
+                    ],
+                }
+            )
+            self._update()
+            # certain fields are required in the acquisition data
+            if "acq_return_type" not in self.data["acquisition_info"][0]:
+                self.data["acquisition_info"][0]["acq_return_type"] = complex
+                self.data["acquisition_info"][0]["protocol"] = "ssb_integration_complex"
+        else:
+            warnings.warn(
+                "Support for the data argument will be dropped in"
+                "quantify-scheduler >= 0.13.0.\n"
+                "Please consider updating the data "
+                "dictionary after initialization.",
+                DeprecationWarning,
+            )
+            if "acq_return_type" not in data["acquisition_info"][0]:
+                data["acquisition_info"][0]["acq_return_type"] = complex
+                data["acquisition_info"][0]["protocol"] = "ssb_integration_complex"
+            super().__init__(name=data["name"], data=data)
 
     def __str__(self) -> str:
         acq_info = self.data["acquisition_info"][0]
         return self._get_signature(acq_info)
 
 
 class NumericalWeightedIntegrationComplex(
@@ -429,27 +472,36 @@
         waveforms_b = {
             "wf_func": "quantify_scheduler.waveforms.interpolated_complex_waveform",
             "samples": weights_b,
             "t_samples": t,
             "interpolation": interpolation,
         }
         duration = t[-1] - t[0]
+        if data is not None:
+            warnings.warn(
+                "Support for the data argument will be dropped in"
+                "quantify-scheduler >= 0.13.0.\n"
+                "Please consider updating the data "
+                "dictionary after initialization.",
+                DeprecationWarning,
+            )
         super().__init__(
             waveforms_a,
             waveforms_b,
             port,
             clock,
             duration,
             acq_channel,
             acq_index,
             bin_mode,
             phase,
             t0,
             data,
         )
+        self._update()
         self.data["name"] = "NumericalWeightedIntegrationComplex"
 
     def __str__(self) -> str:
         acq_info = self.data["acquisition_info"][0]
         weights_a = np.array2string(
             acq_info["waveforms"][0]["samples"], separator=", ", precision=9
         )
```

### Comparing `quantify-scheduler-0.8.0/quantify_scheduler/operations/gate_library.py` & `quantify-scheduler-0.9.0/quantify_scheduler/operations/gate_library.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Repository: https://gitlab.com/quantify-os/quantify-scheduler
 # Licensed according to the LICENCE file on the main branch
 # pylint: disable=invalid-name
 """Standard gateset for use with the quantify_scheduler."""
 from typing import Literal, Optional, Tuple, Union
+import warnings
 
 import numpy as np
 
 from .operation import Operation
 from ..enums import BinMode
 
 
@@ -52,15 +53,14 @@
             phi = float(phi)
 
         # this solves an issue where different rotations with the same rotation angle
         # modulo a full period are treated as distinct operations in the OperationDict.
         theta = (theta + 180) % 360 - 180
 
         phi = phi % 360
-
         if data is None:
             tex = r"$R_{xy}^{" + f"{theta:.0f}, {phi:.0f}" + r"}$"
             plot_func = "quantify_scheduler.visualization.circuit_diagram.gate_box"
             theta_r = np.deg2rad(theta)
             phi_r = np.deg2rad(phi)
 
             # not all operations have a valid unitary description
@@ -73,29 +73,39 @@
                     ],
                     [
                         -1j * np.exp(1j * phi_r) * np.sin(theta_r / 2),
                         np.cos(theta_r / 2),
                     ],
                 ]
             )
-
-            data = {
-                "name": f"Rxy({theta:.8g}, {phi:.8g}, '{qubit}')",
-                "gate_info": {
-                    "unitary": unitary,
-                    "tex": tex,
-                    "plot_func": plot_func,
-                    "qubits": [qubit],
-                    "operation_type": "Rxy",
-                    "theta": theta,
-                    "phi": phi,
-                },
-            }
-
-        super().__init__(data["name"], data=data)
+            super().__init__(f"Rxy({theta:.8g}, {phi:.8g}, '{qubit}')")
+            self.data.update(
+                {
+                    "name": f"Rxy({theta:.8g}, {phi:.8g}, '{qubit}')",
+                    "gate_info": {
+                        "unitary": unitary,
+                        "tex": tex,
+                        "plot_func": plot_func,
+                        "qubits": [qubit],
+                        "operation_type": "Rxy",
+                        "theta": theta,
+                        "phi": phi,
+                    },
+                }
+            )
+            self._update()
+        else:
+            warnings.warn(
+                "Support for the data argument will be dropped in"
+                "quantify-scheduler >= 0.13.0.\n"
+                "Please consider updating the data "
+                "dictionary after initialization.",
+                DeprecationWarning,
+            )
+            super().__init__(name=data["name"], data=data)
 
     def __str__(self) -> str:
         gate_info = self.data["gate_info"]
         theta = gate_info["theta"]
         phi = gate_info["phi"]
         qubit = gate_info["qubits"][0]
         return f"{self.__class__.__name__}(theta={theta:.8g}, phi={phi:.8g}, qubit='{qubit}')"
@@ -106,43 +116,61 @@
     A single qubit rotation of 180 degrees around the X-axis.
 
 
     This operation can be represented by the following unitary:
 
     .. math::
 
-        X = \sigma_x = \begin{bmatrix}
-             0 & 1 \\
-             1 & 0 \\ \end{bmatrix}
+        X180 = R_{X180} = \begin{bmatrix}
+             0 & -i \\
+             -i & 0 \\ \end{bmatrix}
 
     """
 
     def __init__(self, qubit: str, data: Optional[dict] = None):
         """
         Parameters
         ----------
         qubit
             the target qubit
         data
             The operation's dictionary, by default None
             Note: if the data parameter is not None all other parameters are
             overwritten using the contents of data.
         """
+        if data is not None:
+            warnings.warn(
+                "Support for the data argument will be dropped in"
+                "quantify-scheduler >= 0.13.0.\n"
+                "Please consider updating the data "
+                "dictionary after initialization.",
+                DeprecationWarning,
+            )
         super().__init__(theta=180, phi=0, qubit=qubit, data=data)
         self.data["name"] = f"X {qubit}"
         self.data["gate_info"]["tex"] = r"$X_{\pi}$"
 
     def __str__(self) -> str:
         qubit = self.data["gate_info"]["qubits"][0]
         return f"{self.__class__.__name__}(qubit='{qubit}')"
 
 
 class X90(Rxy):
-    """
+    r"""
     A single qubit rotation of 90 degrees around the X-axis.
+
+    It is identical to the Rxy gate with theta=90 and phi=0
+
+    Defined by the unitary:
+
+    .. math::
+        X90 = R_{X90} = \frac{1}{\sqrt{2}}\begin{bmatrix}
+                1 & -i \\
+                -i & 1 \\ \end{bmatrix}
+
     """
 
     def __init__(self, qubit: str, data: Optional[dict] = None):
         """
         Create a new instance of X90.
 
         Parameters
@@ -150,34 +178,44 @@
         qubit
             The target qubit.
         data
             The operation's dictionary, by default None
             Note: if the data parameter is not None all other parameters are
             overwritten using the contents of data.
         """
+        if data is not None:
+            warnings.warn(
+                "Support for the data argument will be dropped in"
+                "quantify-scheduler >= 0.13.0.\n"
+                "Please consider updating the data "
+                "dictionary after initialization.",
+                DeprecationWarning,
+            )
         super().__init__(theta=90.0, phi=0.0, qubit=qubit, data=data)
         self.qubit = qubit
         self.data["name"] = f"X_90 {qubit}"
         self.data["gate_info"]["tex"] = r"$X_{\pi/2}$"
 
     def __str__(self) -> str:
         qubit = self.data["gate_info"]["qubits"][0]
         return f"{self.__class__.__name__}(qubit='{qubit}')"
 
 
 class Y(Rxy):
     r"""
     A single qubit rotation of 180 degrees around the Y-axis.
 
+    It is identical to the Rxy gate with theta=180 and phi=90
 
-    .. math::
+    Defined by the unitary: 
 
-        \mathsf Y = \sigma_y = \begin{bmatrix}
-             0 & -i \\
-             i & 0 \end{bmatrix}
+    .. math::
+        Y180 = R_{Y180} = \begin{bmatrix}
+             0 & -1 \\
+             1 & 0 \\ \end{bmatrix}
 
     """
 
     def __init__(self, qubit: str, data: Optional[dict] = None):
         """
         Create a new instance of Y.
 
@@ -189,26 +227,45 @@
         qubit
             The target qubit.
         data
             The operation's dictionary, by default None
             Note: if the data parameter is not None all other parameters are
             overwritten using the contents of data.
         """
+        if data is not None:
+            warnings.warn(
+                "Support for the data argument will be dropped in"
+                "quantify-scheduler >= 0.13.0.\n"
+                "Please consider updating the data "
+                "dictionary after initialization.",
+                DeprecationWarning,
+            )
         super().__init__(theta=180.0, phi=90.0, qubit=qubit, data=data)
         self.data["name"] = f"Y {qubit}"
         self.data["gate_info"]["tex"] = r"$Y_{\pi}$"
 
     def __str__(self) -> str:
         qubit = self.data["gate_info"]["qubits"][0]
         return f"{self.__class__.__name__}(qubit='{qubit}')"
 
 
 class Y90(Rxy):
-    """
+    r"""
     A single qubit rotation of 90 degrees around the Y-axis.
+
+    It is identical to the Rxy gate with theta=90 and phi=90
+
+    Defined by the unitary: 
+
+    .. math::
+
+        Y90 = R_{Y90} = \frac{1}{\sqrt{2}}\begin{bmatrix}
+                1 & -1 \\
+                1 & 1 \\ \end{bmatrix}
+
     """
 
     def __init__(self, qubit: str, data: Optional[dict] = None):
         """
         Create a new instance of Y90.
 
         The Y gate corresponds to a rotation of 90 degrees around the y-axis in the
@@ -219,23 +276,31 @@
         qubit
             The target qubit.
         data
             The operation's dictionary, by default None
             Note: if the data parameter is not None all other parameters are
             overwritten using the contents of data.
         """
+        if data is not None:
+            warnings.warn(
+                "Support for the data argument will be dropped in"
+                "quantify-scheduler >= 0.13.0.\n"
+                "Please consider updating the data "
+                "dictionary after initialization.",
+                DeprecationWarning,
+            )
         super().__init__(theta=90.0, phi=90.0, qubit=qubit, data=data)
         self.data["name"] = f"Y_90 {qubit}"
         self.data["gate_info"]["tex"] = r"$Y_{\pi/2}$"
 
     def __str__(self) -> str:
         """
         Returns a concise string representation
         which can be evaluated into a new instance
-        using `eval(str(operation))` only when the
+        using :code:`eval(str(operation))` only when the
         data dictionary has not been modified.
 
         This representation is guaranteed to be
         unique.
         """
         qubit = self.data["gate_info"]["qubits"][0]
         return f"{self.__class__.__name__}(qubit='{qubit}')"
@@ -276,28 +341,40 @@
         data
             The operation's dictionary, by default None
             Note: if the data parameter is not None all other parameters are
             overwritten using the contents of data.
         """
         if data is None:
             plot_func = "quantify_scheduler.visualization.circuit_diagram.cnot"
-            data = {
-                "name": f"CNOT ({qC}, {qT})",
-                "gate_info": {
-                    "unitary": np.array(
-                        [[1, 0, 0, 0], [0, 1, 0, 0], [0, 0, 0, 1], [0, 0, 1, 0]]
-                    ),
-                    "tex": r"CNOT",
-                    "plot_func": plot_func,
-                    "qubits": [qC, qT],
-                    "symmetric": False,
-                    "operation_type": "CNOT",
-                },
-            }
-        super().__init__(data["name"], data=data)
+            super().__init__(f"CNOT ({qC}, {qT})")
+            self.data.update(
+                {
+                    "name": f"CNOT ({qC}, {qT})",
+                    "gate_info": {
+                        "unitary": np.array(
+                            [[1, 0, 0, 0], [0, 1, 0, 0], [0, 0, 0, 1], [0, 0, 1, 0]]
+                        ),
+                        "tex": r"CNOT",
+                        "plot_func": plot_func,
+                        "qubits": [qC, qT],
+                        "symmetric": False,
+                        "operation_type": "CNOT",
+                    },
+                }
+            )
+            self._update()
+        else:
+            warnings.warn(
+                "Support for the data argument will be dropped in"
+                "quantify-scheduler >= 0.13.0.\n"
+                "Please consider updating the data "
+                "dictionary after initialization.",
+                DeprecationWarning,
+            )
+            super().__init__(name=data["name"], data=data)
 
     def __str__(self) -> str:
         gate_info = self.data["gate_info"]
         qC = gate_info["qubits"][0]
         qT = gate_info["qubits"][1]
         return f"{self.__class__.__name__}(qC='{qC}',qT='{qT}')"
 
@@ -337,28 +414,40 @@
         data
             The operation's dictionary, by default None
             Note: if the data parameter is not None all other parameters are
             overwritten using the contents of data.
         """
         if data is None:
             plot_func = "quantify_scheduler.visualization.circuit_diagram.cz"
-            data = {
-                "name": f"CZ ({qC}, {qT})",
-                "gate_info": {
-                    "unitary": np.array(
-                        [[1, 0, 0, 0], [0, 1, 0, 0], [0, 0, 1, 0], [0, 0, 0, -1]]
-                    ),
-                    "tex": r"CZ",
-                    "plot_func": plot_func,
-                    "qubits": [qC, qT],
-                    "symmetric": True,
-                    "operation_type": "CZ",
-                },
-            }
-        super().__init__(data["name"], data=data)
+            super().__init__(f"CZ ({qC}, {qT})")
+            self.data.update(
+                {
+                    "name": f"CZ ({qC}, {qT})",
+                    "gate_info": {
+                        "unitary": np.array(
+                            [[1, 0, 0, 0], [0, 1, 0, 0], [0, 0, 1, 0], [0, 0, 0, -1]]
+                        ),
+                        "tex": r"CZ",
+                        "plot_func": plot_func,
+                        "qubits": [qC, qT],
+                        "symmetric": True,
+                        "operation_type": "CZ",
+                    },
+                }
+            )
+            self._update()
+        else:
+            warnings.warn(
+                "Support for the data argument will be dropped in"
+                "quantify-scheduler >= 0.13.0.\n"
+                "Please consider updating the data "
+                "dictionary after initialization.",
+                DeprecationWarning,
+            )
+            super().__init__(name=data["name"], data=data)
 
     def __str__(self) -> str:
         gate_info = self.data["gate_info"]
         qC = gate_info["qubits"][0]
         qT = gate_info["qubits"][1]
 
         return f"{self.__class__.__name__}(qC='{qC}',qT='{qT}')"
@@ -402,26 +491,38 @@
             :code:`Reset("q0")`, :code:`Reset("q0", "q1", "q2")`, etc..
         data
             The operation's dictionary, by default :code:`None`.
             Note: if the data parameter is not :code:`None` all other parameters are
             overwritten using the contents of data.
         """
         if data is None:
+            super().__init__(f"Reset {', '.join(qubits)}")
             plot_func = "quantify_scheduler.visualization.circuit_diagram.reset"
-            data = {
-                "name": f"Reset {', '.join(qubits)}",
-                "gate_info": {
-                    "unitary": None,
-                    "tex": r"$|0\rangle$",
-                    "plot_func": plot_func,
-                    "qubits": list(qubits),
-                    "operation_type": "reset",
-                },
-            }
-        super().__init__(data["name"], data=data)
+            self.data.update(
+                {
+                    "name": f"Reset {', '.join(qubits)}",
+                    "gate_info": {
+                        "unitary": None,
+                        "tex": r"$|0\rangle$",
+                        "plot_func": plot_func,
+                        "qubits": list(qubits),
+                        "operation_type": "reset",
+                    },
+                }
+            )
+            self._update()
+        else:
+            warnings.warn(
+                "Support for the data argument will be dropped in"
+                "quantify-scheduler >= 0.13.0.\n"
+                "Please consider updating the data "
+                "dictionary after initialization.",
+                DeprecationWarning,
+            )
+            super().__init__(name=data["name"], data=data)
 
     def __str__(self) -> str:
         qubits = map(lambda x: f"'{x}'", self.data["gate_info"]["qubits"])
         return f'{self.__class__.__name__}({",".join(qubits)})'
 
 
 class Measure(Operation):
@@ -485,44 +586,58 @@
         if len(qubits) == 1:
             if acq_channel is None:
                 acq_channel = 0
             if acq_index is None:
                 acq_index = 0
         else:
             if isinstance(acq_index, int):
-                acq_index = (acq_index,) * len(qubits)
+                acq_index = [
+                    acq_index,
+                ] * len(qubits)
             elif acq_index is None:
                 # defaults to writing the result of all qubits to acq_index 0.
                 # note that this will result in averaging data together if multiple
                 # measurements are present in the same schedule (#262)
-                acq_index = tuple(0 for i in range(len(qubits)))
+                acq_index = list(0 for i in range(len(qubits)))
 
             # defaults to mapping qubits to channels dependent on the order of the
             # arguments. note that this will result in mislabeling data if not all
             # measurements in an experiment contain the same order of qubits (#262)
             if acq_channel is None:
-                acq_channel = tuple(i for i in range(len(qubits)))
+                acq_channel = list(i for i in range(len(qubits)))
 
         if data is None:
             plot_func = "quantify_scheduler.visualization.circuit_diagram.meter"
-            data = {
-                "name": f"Measure {', '.join(qubits)}",
-                "gate_info": {
-                    "unitary": None,
-                    "plot_func": plot_func,
-                    "tex": r"$\langle0|$",
-                    "qubits": list(qubits),
-                    "acq_channel": acq_channel,
-                    "acq_index": acq_index,
-                    "acq_protocol": acq_protocol,
-                    "bin_mode": bin_mode,
-                    "operation_type": "measure",
-                },
-            }
-        super().__init__(data["name"], data=data)
+            super().__init__(f"Measure {', '.join(qubits)}")
+            self.data.update(
+                {
+                    "name": f"Measure {', '.join(qubits)}",
+                    "gate_info": {
+                        "unitary": None,
+                        "plot_func": plot_func,
+                        "tex": r"$\langle0|$",
+                        "qubits": list(qubits),
+                        "acq_channel": acq_channel,
+                        "acq_index": acq_index,
+                        "acq_protocol": acq_protocol,
+                        "bin_mode": bin_mode,
+                        "operation_type": "measure",
+                    },
+                }
+            )
+            self._update()
+        else:
+            warnings.warn(
+                "Support for the data argument will be dropped in"
+                "quantify-scheduler >= 0.13.0.\n"
+                "Please consider updating the data "
+                "dictionary after initialization.",
+                DeprecationWarning,
+            )
+            super().__init__(name=data["name"], data=data)
 
     def __str__(self) -> str:
         gate_info = self.data["gate_info"]
         qubits = map(lambda x: f"'{x}'", gate_info["qubits"])
         acq_channel = gate_info["acq_channel"]
         acq_index = gate_info["acq_index"]
         acq_protocol = gate_info["acq_protocol"]
```

### Comparing `quantify-scheduler-0.8.0/quantify_scheduler/operations/measurement_factories.py` & `quantify-scheduler-0.9.0/quantify_scheduler/operations/measurement_factories.py`

 * *Files identical despite different names*

### Comparing `quantify-scheduler-0.8.0/quantify_scheduler/operations/operation.py` & `quantify-scheduler-0.9.0/quantify_scheduler/operations/operation.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,21 +3,22 @@
 """Module containing the core concepts of the scheduler."""
 from __future__ import annotations
 
 import ast
 import inspect
 import logging
 from collections import UserDict
-from copy import deepcopy
 from enum import Enum
 from pydoc import locate
-from typing import Any, Dict
+import warnings
 
 import numpy as np
 
+from quantify_core.utilities import deprecated
+
 from quantify_scheduler import enums
 from quantify_scheduler.helpers.collections import make_hash
 from quantify_scheduler.json_utils import JSONSchemaValMixin, lru_cache
 
 cached_locate = lru_cache(locate)
 
 
@@ -75,14 +76,21 @@
         self.data["gate_info"] = {}
         self.data["pulse_info"] = []
         self.data["acquisition_info"] = []
         self.data["logic_info"] = {}
         self._duration: float = 0
 
         if data is not None:
+            warnings.warn(
+                "Support for the data argument will be dropped in"
+                "quantify-scheduler >= 0.13.0.\n"
+                "Please consider updating the data "
+                "dictionary after initialization.",
+                DeprecationWarning,
+            )
             self.data.update(data)
             self._deserialize()
             self._update()
 
     def __eq__(self, other) -> bool:
         """
         Returns the equality of two instances based on its content :code:`self.data`.
@@ -96,38 +104,30 @@
         :
         """
         return repr(self) == repr(other)
 
     def __str__(self) -> str:
         """
         Returns a concise string representation which can be evaluated into a new
-        instance using `eval(str(operation))` only when the data dictionary has
+        instance using :code:`eval(str(operation))` only when the data dictionary has
         not been modified.
 
         This representation is guaranteed to be unique.
         """
         return f"{self.__class__.__name__}(name='{self.name}')"
 
-    def __repr__(self) -> str:
-        """
-        Returns the string representation  of this instance.
-
-        This representation can always be evaluated to create a new instance.
-
-        .. code-block::
-
-            eval(repr(operation))
+    def __getstate__(self):
+        return {
+            "deserialization_type": self.__class__.__name__,
+            "data": self.data,
+        }
 
-        Returns
-        -------
-        :
-        """
-        _data = self._serialize()
-        data_str = f"{str(self)[:-1]}, data={_data})"
-        return data_str
+    def __setstate__(self, state):
+        self.data = state["data"]
+        self._update()
 
     def _update(self) -> None:
         """Update the Operation's internals."""
 
         def _get_operation_end(info) -> float:
             """Return the operation end in seconds."""
             return info["t0"] + info["duration"]
@@ -255,52 +255,20 @@
         ----------
         acquisition_operation
             an operation containing acquisition_info.
         """
         self.data["acquisition_info"] += acquisition_operation.data["acquisition_info"]
         self._update()
 
-    def _serialize(self) -> Dict[str, Any]:
-        """
-        Serializes the data dictionary.
-
-        Returns
-        -------
-        :
-        """
-        _data = deepcopy(self.data)
-        if "unitary" in _data["gate_info"] and isinstance(
-            _data["gate_info"]["unitary"], (np.generic, np.ndarray)
-        ):
-            _data["gate_info"]["unitary"] = np.array2string(
-                _data["gate_info"]["unitary"], separator=", ", precision=9
-            )
-
-        for acq_info in _data["acquisition_info"]:
-            if "bin_mode" in acq_info and isinstance(
-                acq_info["bin_mode"], enums.BinMode
-            ):
-                acq_info["bin_mode"] = acq_info["bin_mode"].value
-
-            # types lead to problems when serialized without casting to string first
-            if "<class " in str(acq_info["acq_return_type"]):
-                acq_info["acq_return_type"] = str(acq_info["acq_return_type"])
-
-            for waveform in acq_info["waveforms"]:
-                if "t" in waveform:
-                    waveform["t"] = np.array2string(
-                        waveform["t"], separator=", ", precision=9
-                    )
-                if "weights" in waveform:
-                    waveform["weights"] = np.array2string(
-                        waveform["weights"], separator=", ", precision=9
-                    )
-
-        return _data
-
+    @deprecated(
+        "0.13.0",
+        "Deserialization is handled by the "
+        "`json_utils.ScheduleJSONDecoder` class together with the"
+        "`Operation.__set_state__` method.",
+    )
     def _deserialize(self) -> None:
         """Deserializes the data dictionary."""
         if "unitary" in self.data["gate_info"] and isinstance(
             self.data["gate_info"]["unitary"], str
         ):
             self.data["gate_info"]["unitary"] = np.array(
                 ast.literal_eval(self.data["gate_info"]["unitary"])
```

### Comparing `quantify-scheduler-0.8.0/quantify_scheduler/operations/pulse_factories.py` & `quantify-scheduler-0.9.0/quantify_scheduler/operations/pulse_factories.py`

 * *Files identical despite different names*

### Comparing `quantify-scheduler-0.8.0/quantify_scheduler/operations/pulse_library.py` & `quantify-scheduler-0.9.0/quantify_scheduler/operations/pulse_library.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # Repository: https://gitlab.com/quantify-os/quantify-scheduler
 # Licensed according to the LICENCE file on the main branch
 """Standard pulses for use with the quantify_scheduler."""
 # pylint: disable= too-many-arguments, too-many-ancestors
 from __future__ import annotations
 
 from typing import List, Optional, Dict, Any, Union
+import warnings
 
 import numpy as np
 from numpy.typing import NDArray
 from qcodes import validators
 
 from quantify_scheduler import Operation
 from quantify_scheduler.helpers.waveforms import area_pulses
@@ -32,28 +33,40 @@
             The clock of which to shift the phase.
         data
             The operation's dictionary, by default None
             Note: if the data parameter is not None all other parameters are
             overwritten using the contents of data.
         """
         if data is None:
-            data = {
-                "name": "ShiftClockPhase",
-                "pulse_info": [
-                    {
-                        "wf_func": None,
-                        "t0": t0,
-                        "phase": phase,
-                        "clock": clock,
-                        "port": None,
-                        "duration": 0,
-                    }
-                ],
-            }
-        super().__init__(name=data["name"], data=data)
+            super().__init__(name="ShiftClockPhase")
+            self.data.update(
+                {
+                    "name": "ShiftClockPhase",
+                    "pulse_info": [
+                        {
+                            "wf_func": None,
+                            "t0": t0,
+                            "phase": phase,
+                            "clock": clock,
+                            "port": None,
+                            "duration": 0,
+                        }
+                    ],
+                }
+            )
+            self._update()
+        else:
+            warnings.warn(
+                "Support for the data argument will be dropped in"
+                "quantify-scheduler >= 0.13.0.\n"
+                "Please consider updating the data "
+                "dictionary after initialization.",
+                DeprecationWarning,
+            )
+            super().__init__(name=data["name"], data=data)
 
     def __str__(self) -> str:
         pulse_info = self.data["pulse_info"][0]
         return self._get_signature(pulse_info)
 
 
 class IdlePulse(Operation):
@@ -73,29 +86,40 @@
         duration
             The duration of idle time in seconds.
         data
             The operation's dictionary, by default None
             Note: if the data parameter is not None all other parameters are
             overwritten using the contents of data.
         """
-
         if data is None:
-            data = {
-                "name": "Idle",
-                "pulse_info": [
-                    {
-                        "wf_func": None,
-                        "t0": 0,
-                        "duration": duration,
-                        "clock": BasebandClockResource.IDENTITY,
-                        "port": None,
-                    }
-                ],
-            }
-        super().__init__(name=data["name"], data=data)
+            super().__init__(name="Idle")
+            self.data.update(
+                {
+                    "name": "Idle",
+                    "pulse_info": [
+                        {
+                            "wf_func": None,
+                            "t0": 0,
+                            "duration": duration,
+                            "clock": BasebandClockResource.IDENTITY,
+                            "port": None,
+                        }
+                    ],
+                }
+            )
+            self._update()
+        else:
+            warnings.warn(
+                "Support for the data argument will be dropped in"
+                "quantify-scheduler >= 0.13.0.\n"
+                "Please consider updating the data "
+                "dictionary after initialization.",
+                DeprecationWarning,
+            )
+            super().__init__(name=data["name"], data=data)
 
     def __str__(self) -> str:
         pulse_info = self.data["pulse_info"][0]
         return self._get_signature(pulse_info)
 
 
 class RampPulse(Operation):
@@ -146,29 +170,41 @@
             of the Operation in the Schedule.
         data
             The operation's dictionary, by default None
             Note: if the data parameter is not None all other parameters are
             overwritten using the contents of data.
         """
         if data is None:
-            data = {
-                "name": "RampPulse",
-                "pulse_info": [
-                    {
-                        "wf_func": "quantify_scheduler.waveforms.ramp",
-                        "amp": amp,
-                        "duration": duration,
-                        "offset": offset,
-                        "t0": t0,
-                        "clock": clock,
-                        "port": port,
-                    }
-                ],
-            }
-        super().__init__(name=data["name"], data=data)
+            super().__init__(name="RampPulse")
+            self.data.update(
+                {
+                    "name": "RampPulse",
+                    "pulse_info": [
+                        {
+                            "wf_func": "quantify_scheduler.waveforms.ramp",
+                            "amp": amp,
+                            "duration": duration,
+                            "offset": offset,
+                            "t0": t0,
+                            "clock": clock,
+                            "port": port,
+                        }
+                    ],
+                }
+            )
+            self._update()
+        else:
+            warnings.warn(
+                "Support for the data argument will be dropped in"
+                "quantify-scheduler >= 0.13.0.\n"
+                "Please consider updating the data "
+                "dictionary after initialization.",
+                DeprecationWarning,
+            )
+            super().__init__(name=data["name"], data=data)
 
     def __str__(self) -> str:
         pulse_info = self.data["pulse_info"][0]
         return self._get_signature(pulse_info)
 
 
 class StaircasePulse(Operation):  # pylint: disable=too-many-ancestors
@@ -210,30 +246,43 @@
             of the Operation in the Schedule.
         data
             The operation's dictionary, by default None
             Note: if the data parameter is not None all other parameters are
             overwritten using the contents of data.
         """
         if data is None:
-            data = {
-                "name": "StaircasePulse",
-                "pulse_info": [
-                    {
-                        "wf_func": "quantify_scheduler.waveforms.staircase",
-                        "start_amp": start_amp,
-                        "final_amp": final_amp,
-                        "num_steps": num_steps,
-                        "duration": duration,
-                        "t0": t0,
-                        "clock": clock,
-                        "port": port,
-                    }
-                ],
-            }
-        super().__init__(name=data["name"], data=data)
+            super().__init__(name="StaircasePulse")
+
+            self.data.update(
+                {
+                    "name": "StaircasePulse",
+                    "pulse_info": [
+                        {
+                            "wf_func": "quantify_scheduler.waveforms.staircase",
+                            "start_amp": start_amp,
+                            "final_amp": final_amp,
+                            "num_steps": num_steps,
+                            "duration": duration,
+                            "t0": t0,
+                            "clock": clock,
+                            "port": port,
+                        }
+                    ],
+                }
+            )
+            self._update()
+        else:
+            warnings.warn(
+                "Support for the data argument will be dropped in"
+                "quantify-scheduler >= 0.13.0.\n"
+                "Please consider updating the data "
+                "dictionary after initialization.",
+                DeprecationWarning,
+            )
+            super().__init__(name=data["name"], data=data)
 
     def __str__(self) -> str:
         pulse_info = self.data["pulse_info"][0]
         return self._get_signature(pulse_info)
 
 
 class SquarePulse(Operation):
@@ -269,41 +318,49 @@
         clock
             Clock used to modulate the pulse.
         phase
             Phase of the pulse in degrees.
         t0
             Time in seconds when to start the pulses relative to the start time
             of the Operation in the Schedule.
-        data
-            The operation's dictionary, by default None
-            Note: if the data parameter is not None all other parameters are
-            overwritten using the contents of data.
         """
         if phase != 0:
             # Because of how clock interfaces were changed.
             # FIXME: need to be able to add phases to # pylint: disable=fixme
             # the waveform separate from the clock.
             raise NotImplementedError
 
         if data is None:
-            data = {
-                "name": "ModSquarePulse",
-                "pulse_info": [
-                    {
-                        "wf_func": "quantify_scheduler.waveforms.square",
-                        "amp": amp,
-                        "duration": duration,
-                        "phase": phase,
-                        "t0": t0,
-                        "clock": clock,
-                        "port": port,
-                    }
-                ],
-            }
-        super().__init__(name=data["name"], data=data)
+            super().__init__(name="ModSquarePulse")
+            self.data.update(
+                {
+                    "name": "ModSquarePulse",
+                    "pulse_info": [
+                        {
+                            "wf_func": "quantify_scheduler.waveforms.square",
+                            "amp": amp,
+                            "duration": duration,
+                            "phase": phase,
+                            "t0": t0,
+                            "clock": clock,
+                            "port": port,
+                        }
+                    ],
+                }
+            )
+            self._update()
+        else:
+            warnings.warn(
+                "Support for the data argument will be dropped in"
+                "quantify-scheduler >= 0.13.0.\n"
+                "Please consider updating the data "
+                "dictionary after initialization.",
+                DeprecationWarning,
+            )
+            super().__init__(name=data["name"], data=data)
 
     def __str__(self) -> str:
         pulse_info = self.data["pulse_info"][0]
         return self._get_signature(pulse_info)
 
 
 class SuddenNetZeroPulse(Operation):
@@ -355,34 +412,46 @@
             The operation's dictionary, by default None
             Note: if the data parameter is not None all other parameters are
             overwritten using the contents of data.
         """
         duration = t_pulse + t_phi + t_integral_correction
 
         if data is None:
-            data = {
-                "name": "SuddenNetZeroPulse",
-                "pulse_info": [
-                    {
-                        "wf_func": "quantify_scheduler.waveforms.sudden_net_zero",
-                        "amp_A": amp_A,
-                        "amp_B": amp_B,
-                        "net_zero_A_scale": net_zero_A_scale,
-                        "t_pulse": t_pulse,
-                        "t_phi": t_phi,
-                        "t_integral_correction": t_integral_correction,
-                        "duration": duration,
-                        "phase": 0,
-                        "t0": t0,
-                        "clock": clock,
-                        "port": port,
-                    }
-                ],
-            }
-        super().__init__(name=data["name"], data=data)
+            super().__init__(name="SuddenNetZeroPulse")
+            self.data.update(
+                {
+                    "name": "SuddenNetZeroPulse",
+                    "pulse_info": [
+                        {
+                            "wf_func": "quantify_scheduler.waveforms.sudden_net_zero",
+                            "amp_A": amp_A,
+                            "amp_B": amp_B,
+                            "net_zero_A_scale": net_zero_A_scale,
+                            "t_pulse": t_pulse,
+                            "t_phi": t_phi,
+                            "t_integral_correction": t_integral_correction,
+                            "duration": duration,
+                            "phase": 0,
+                            "t0": t0,
+                            "clock": clock,
+                            "port": port,
+                        }
+                    ],
+                }
+            )
+            self._update()
+        else:
+            warnings.warn(
+                "Support for the data argument will be dropped in"
+                "quantify-scheduler >= 0.13.0.\n"
+                "Please consider updating the data "
+                "dictionary after initialization.",
+                DeprecationWarning,
+            )
+            super().__init__(name=data["name"], data=data)
 
     def __str__(self) -> str:
         pulse_info = self.data["pulse_info"][0]
         return self._get_signature(pulse_info)
 
 
 def decompose_long_square_pulse(
@@ -468,28 +537,40 @@
             of the Operation in the Schedule.
         data
             The operation's dictionary, by default None
             Note: if the data parameter is not None all other parameters are
             overwritten using the contents of data.
         """
         if data is None:
-            data = {
-                "name": "SoftSquarePulse",
-                "pulse_info": [
-                    {
-                        "wf_func": "quantify_scheduler.waveforms.soft_square",
-                        "amp": amp,
-                        "duration": duration,
-                        "t0": t0,
-                        "clock": clock,
-                        "port": port,
-                    }
-                ],
-            }
-        super().__init__(name=data["name"], data=data)
+            super().__init__(name="SoftSquarePulse")
+            self.data.update(
+                {
+                    "name": "SoftSquarePulse",
+                    "pulse_info": [
+                        {
+                            "wf_func": "quantify_scheduler.waveforms.soft_square",
+                            "amp": amp,
+                            "duration": duration,
+                            "t0": t0,
+                            "clock": clock,
+                            "port": port,
+                        }
+                    ],
+                }
+            )
+            self._update()
+        else:
+            warnings.warn(
+                "Support for the data argument will be dropped in"
+                "quantify-scheduler >= 0.13.0.\n"
+                "Please consider updating the data "
+                "dictionary after initialization.",
+                DeprecationWarning,
+            )
+            super().__init__(name=data["name"], data=data)
 
     def __str__(self) -> str:
         pulse_info = self.data["pulse_info"][0]
         return self._get_signature(pulse_info)
 
 
 class ChirpPulse(Operation):  # pylint: disable=too-many-ancestors
@@ -502,14 +583,15 @@
         amp: float,
         duration: float,
         port: str,
         clock: str,
         start_freq: float,
         end_freq: float,
         t0: float = 0,
+        data: Optional[dict] = None,
     ):
         """
         Constructor for a chirp pulse.
 
         Parameters
         ----------
         amp
@@ -524,30 +606,43 @@
             Start frequency of the Chirp. Note that this is the frequency at which the
             waveform is calculated, this may differ from the clock frequency.
         end_freq
             End frequency of the Chirp.
         t0
             Shift of the start time with respect to the start of the operation.
         """
-        data = {
-            "name": "ChirpPulse",
-            "pulse_info": [
-                {
-                    "wf_func": "quantify_scheduler.waveforms.chirp",
-                    "amp": amp,
-                    "duration": duration,
-                    "start_freq": start_freq,
-                    "end_freq": end_freq,
-                    "t0": t0,
-                    "clock": clock,
-                    "port": port,
-                }
-            ],
-        }
-        super().__init__(name=data["name"], data=data)
+        if data is None:
+            super().__init__(name="ChirpPulse")
+            self.data.update(
+                {
+                    "name": "ChirpPulse",
+                    "pulse_info": [
+                        {
+                            "wf_func": "quantify_scheduler.waveforms.chirp",
+                            "amp": amp,
+                            "duration": duration,
+                            "start_freq": start_freq,
+                            "end_freq": end_freq,
+                            "t0": t0,
+                            "clock": clock,
+                            "port": port,
+                        }
+                    ],
+                }
+            )
+            self._update()
+        else:
+            warnings.warn(
+                "Support for the data argument will be dropped in"
+                "quantify-scheduler >= 0.13.0.\n"
+                "Please consider updating the data "
+                "dictionary after initialization.",
+                DeprecationWarning,
+            )
+            super().__init__(name=data["name"], data=data)
 
     def __str__(self) -> str:
         pulse_info = self.data["pulse_info"][0]
         return self._get_signature(pulse_info)
 
 
 class DRAGPulse(Operation):
@@ -597,31 +692,43 @@
         data
             The operation's dictionary, by default None
             Note: if the data parameter is not None all other parameters are
             overwritten using the contents of data.
         """
 
         if data is None:
-            data = {
-                "name": "DRAG",
-                "pulse_info": [
-                    {
-                        "wf_func": "quantify_scheduler.waveforms.drag",
-                        "G_amp": G_amp,
-                        "D_amp": D_amp,
-                        "duration": duration,
-                        "phase": phase,
-                        "nr_sigma": 4,
-                        "clock": clock,
-                        "port": port,
-                        "t0": t0,
-                    }
-                ],
-            }
-        super().__init__(name=data["name"], data=data)
+            super().__init__(name="DRAG")
+            self.data.update(
+                {
+                    "name": "DRAG",
+                    "pulse_info": [
+                        {
+                            "wf_func": "quantify_scheduler.waveforms.drag",
+                            "G_amp": G_amp,
+                            "D_amp": D_amp,
+                            "duration": duration,
+                            "phase": phase,
+                            "nr_sigma": 4,
+                            "clock": clock,
+                            "port": port,
+                            "t0": t0,
+                        }
+                    ],
+                }
+            )
+            self._update()
+        else:
+            warnings.warn(
+                "Support for the data argument will be dropped in"
+                "quantify-scheduler >= 0.13.0.\n"
+                "Please consider updating the data "
+                "dictionary after initialization.",
+                DeprecationWarning,
+            )
+            super().__init__(name=data["name"], data=data)
 
     def __str__(self) -> str:
         pulse_info = self.data["pulse_info"][0]
         return self._get_signature(pulse_info)
 
 
 def create_dc_compensation_pulse(
@@ -704,14 +811,23 @@
         c_duration = abs(area / c_amp)
     else:
         raise ValueError(
             "The `DCCompensationPulse` allows either amp or duration to "
             + "be specified, not both. Both amp and duration were passed."
         )
 
+    if data is not None:
+        warnings.warn(
+            "Support for the data argument will be dropped in"
+            "quantify-scheduler >= 0.13.0.\n"
+            "Please consider updating the data "
+            "dictionary after initialization.",
+            DeprecationWarning,
+        )
+
     return SquarePulse(
         amp=c_amp,
         duration=c_duration,
         port=port,
         clock=BasebandClockResource.IDENTITY,
         phase=0,
         t0=t0,
@@ -749,27 +865,39 @@
         data: Optional[Dict[str, Any]] = None,
     ):
         """
         Create a new instance of WindowOperation.
 
         """
         if data is None:
-            data = {
-                "name": "WindowOperation",
-                "pulse_info": [
-                    {
-                        "wf_func": None,
-                        "window_name": window_name,
-                        "duration": duration,
-                        "t0": t0,
-                        "port": None,
-                    }
-                ],
-            }
-        super().__init__(name=data["name"], data=data)
+            super().__init__(name="WindowOperation")
+            self.data.update(
+                {
+                    "name": "WindowOperation",
+                    "pulse_info": [
+                        {
+                            "wf_func": None,
+                            "window_name": window_name,
+                            "duration": duration,
+                            "t0": t0,
+                            "port": None,
+                        }
+                    ],
+                }
+            )
+            self._update()
+        else:
+            warnings.warn(
+                "Support for the data argument will be dropped in"
+                "quantify-scheduler >= 0.13.0.\n"
+                "Please consider updating the data "
+                "dictionary after initialization.",
+                DeprecationWarning,
+            )
+            super().__init__(name=data["name"], data=data)
 
     @property
     def window_name(self) -> str:
         """Return the window name of this operation"""
         return self.data["pulse_info"][0]["window_name"]
 
     def __str__(self) -> str:
@@ -830,29 +958,40 @@
                 new_val: List[float] = val.tolist()
                 return new_val
             return val
 
         duration = t_samples[-1] - t_samples[0]
         samples, t_samples = map(make_list_from_array, [samples, t_samples])
         if data is None:
-            data = {
-                "name": "NumericalPulse",
-                "pulse_info": [
-                    {  # pylint: disable=line-too-long
-                        "wf_func": "quantify_scheduler.waveforms.interpolated_complex_waveform",
-                        "samples": samples,
-                        "t_samples": t_samples,
-                        "duration": duration,
-                        "interpolation": interpolation,
-                        "clock": clock,
-                        "port": port,
-                        "t0": t0,
-                    }
-                ],
-            }
-
-        super().__init__(name=data["name"], data=data)
+            super().__init__(name="NumericalPulse")
+            self.data.update(
+                {
+                    "name": "NumericalPulse",
+                    "pulse_info": [
+                        {  # pylint: disable=line-too-long
+                            "wf_func": "quantify_scheduler.waveforms.interpolated_complex_waveform",
+                            "samples": samples,
+                            "t_samples": t_samples,
+                            "duration": duration,
+                            "interpolation": interpolation,
+                            "clock": clock,
+                            "port": port,
+                            "t0": t0,
+                        }
+                    ],
+                }
+            )
+            self._update()
+        else:
+            warnings.warn(
+                "Support for the data argument will be dropped in"
+                "quantify-scheduler >= 0.13.0.\n"
+                "Please consider updating the data "
+                "dictionary after initialization.",
+                DeprecationWarning,
+            )
+            super().__init__(name=data["name"], data=data)
 
     def __str__(self) -> str:
         """Provides a string representation of the Pulse."""
         pulse_info = self.data["pulse_info"][0]
         return self._get_signature(pulse_info)
```

### Comparing `quantify-scheduler-0.8.0/quantify_scheduler/resources.py` & `quantify-scheduler-0.9.0/quantify_scheduler/resources.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 # Licensed according to the LICENCE file on the main branch
 """Common resources for use with the quantify_scheduler."""
 
 from __future__ import annotations
 
 from collections import UserDict
 from typing import Optional
+import warnings
 
 from quantify_scheduler.json_utils import load_json_schema, validate_json
 
 
 class Resource(UserDict):
     # pylint: disable=line-too-long
     """
@@ -33,14 +34,21 @@
             The resource data dictionary, by default None
         """
         super().__init__()
 
         self.data["name"] = name
 
         if data is not None:
+            warnings.warn(
+                "Support for the data argument will be dropped in"
+                "quantify-scheduler >= 0.13.0.\n"
+                "Please consider updating the data "
+                "dictionary after initialization.",
+                DeprecationWarning,
+            )
             self.data.update(data)
 
     @classmethod
     def is_valid(cls, operation: Resource) -> bool:
         """
         Validates the Resource against the schemas/resource.json fastjsonschema.
 
@@ -87,37 +95,27 @@
         -------
         :
         """
         return repr(self) == repr(other)
 
     def __str__(self) -> str:
         """
-        Returns a concise string represenation which can be evaluated into a new
-        instance using `eval(str(operation))` only when the data dictionary has
+        Returns a concise string representation which can be evaluated into a new
+        instance using :code:`eval(str(operation))` only when the data dictionary has
         not been modified.
 
         This representation is guaranteed to be unique.
         """
         return f"{self.__class__.__name__}(name='{self.name}')"
 
-    def __repr__(self) -> str:
-        """
-        Returns the string representation  of this instance.
-
-        This represenation can always be evalued to create a new instance.
-
-        .. code-block::
+    def __getstate__(self):
+        return {"deserialization_type": self.__class__.__name__, "data": self.data}
 
-            eval(repr(operation))
-
-        Returns
-        -------
-        :
-        """
-        return f"{str(self)[:-1]}, data={self.data})"
+    def __setstate__(self, state):
+        self.data = state["data"]
 
 
 class ClockResource(Resource):
     """
     The ClockResource corresponds to a physical clock used to modulate pulses.
     """
 
@@ -133,21 +131,31 @@
             the name of this clock
         freq :
             the frequency of the clock in Hz
         phase :
             the starting phase of the clock in deg
         """
         if data is None:
-            data = {
+            super().__init__(name)
+
+            self.data = {
                 "name": name,
                 "type": str(self.__class__.__name__),
                 "freq": freq,
                 "phase": phase,
             }
-        super().__init__(data["name"], data=data)
+        else:
+            warnings.warn(
+                "Support for the data argument will be dropped in"
+                "quantify-scheduler >= 0.13.0.\n"
+                "Please consider updating the data "
+                "dictionary after initialization.",
+                DeprecationWarning,
+            )
+            super().__init__(data["name"], data=data)
 
     def __str__(self) -> str:
         freq = self.data["freq"]
         phase = self.data["phase"]
         return f"{super().__str__()[:-1]}, freq={freq}, phase={phase})"
 
 
@@ -166,14 +174,24 @@
 
         Parameters
         ----------
         name :
             the name of this clock
         """
         if data is None:
-            data = {
+            super().__init__(name)
+
+            self.data = {
                 "name": name,
                 "type": str(self.__class__.__name__),
                 "freq": 0,
                 "phase": 0,
             }
-        super().__init__(data["name"], data=data)
+        else:
+            warnings.warn(
+                "Support for the data argument will be dropped in"
+                "quantify-scheduler >= 0.13.0.\n"
+                "Please consider updating the data "
+                "dictionary after initialization.",
+                DeprecationWarning,
+            )
+            super().__init__(data["name"], data=data)
```

### Comparing `quantify-scheduler-0.8.0/quantify_scheduler/schedules/schedule.py` & `quantify-scheduler-0.9.0/quantify_scheduler/schedules/schedule.py`

 * *Files 4% similar despite different names*

```diff
@@ -180,55 +180,14 @@
         schedule_data = json_utils.ScheduleJSONDecoder().decode(data)
         name = schedule_data["name"]
         sched = Schedule.__new__(Schedule)
         sched.__setstate__(schedule_data)
 
         return sched
 
-    def plot_circuit_diagram_mpl(
-        self, figsize: Tuple[int, int] = None, ax: Optional[Axes] = None
-    ) -> Tuple[Figure, Union[Axes, List[Axes]]]:
-        """
-        Creates a circuit diagram visualization of the schedule using matplotlib.
-
-        The circuit diagram visualization visualizes the schedule at the quantum circuit
-        layer.
-        This visualization provides no timing information, only showing the order of
-        operations.
-        Because quantify-scheduler uses a hybrid gate-pulse paradigm, operations for
-        which no information is specified at the gate level are visualized using an
-        icon (e.g., a stylized wavy pulse) depending on the information specified at
-        the quantum device layer.
-
-        Alias of :func:`.circuit_diagram.circuit_diagram_matplotlib`.
-
-        Parameters
-        ----------
-        schedule
-            the schedule to render.
-        figsize
-            matplotlib figsize.
-        ax
-            Axis handle to use for plotting.
-
-        Returns
-        -------
-        fig
-            matplotlib figure object.
-        ax
-            matplotlib axis object.
-        """
-        warnings.warn(
-            "`plot_circuit_diagram_mpl` will be removed from this module in "
-            "quantify-scheduler >= 0.6.0.\n"
-            "Instead, use `plot_circuit_diagram`",
-            DeprecationWarning,
-        )
-        return self.plot_circuit_diagram(figsize, ax, "mpl")
-
     def plot_circuit_diagram(
         self,
         figsize: Tuple[int, int] = None,
         ax: Optional[Axes] = None,
         plot_backend: Literal["mpl"] = "mpl",
     ) -> Tuple[Figure, Union[Axes, List[Axes]]]:
         """
@@ -272,57 +231,14 @@
             return cd.circuit_diagram_matplotlib(schedule=self, figsize=figsize, ax=ax)
 
         raise ValueError(
             f"plot_backend must be equal to 'mpl', value given: {repr(plot_backend)}"
         )
 
     # pylint: disable=too-many-arguments
-    def plot_pulse_diagram_mpl(
-        self,
-        port_list: Optional[List[str]] = None,
-        sampling_rate: float = 1e9,
-        modulation: Literal["off", "if", "clock"] = "off",
-        modulation_if: float = 0.0,
-        ax: Optional[Axes] = None,
-    ) -> Tuple[Figure, Axes]:
-        """
-        Creates a visualization of all the pulses in a schedule using matplotlib.
-
-        The pulse diagram visualizes the schedule at the quantum device layer.
-        For this visualization to work, all operations need to have the information
-        present (e.g., pulse info) to represent these on the quantum-circuit level and
-        requires the absolute timing to have been determined.
-        This information is typically added when the quantum-device level compilation is
-        performed.
-
-        Alias of :func:`.pulse_diagram.pulse_diagram_matplotlib`.
-
-        port_list :
-            A list of ports to show. if set to `None` will use the first
-            8 ports it encounters in the sequence.
-        modulation :
-            Determines if modulation is included in the visualization.
-        modulation_if :
-            Modulation frequency used when modulation is set to "if".
-        sampling_rate :
-            The time resolution used to sample the schedule in Hz.
-        ax:
-            Axis onto which to plot.
-        """
-        warnings.warn(
-            "`plot_pulse_diagram_mpl` will be removed from this module in "
-            "quantify-scheduler >= 0.6.0.\n"
-            "Instead, use `plot_pulse_diagram`",
-            DeprecationWarning,
-        )
-        return self.plot_pulse_diagram(
-            port_list, sampling_rate, modulation, modulation_if, "mpl", {"ax": ax}
-        )
-
-    # pylint: disable=too-many-arguments
     def plot_pulse_diagram(
         self,
         port_list: Optional[List[str]] = None,
         sampling_rate: float = 1e9,
         modulation: Literal["off", "if", "clock"] = "off",
         modulation_if: float = 0.0,
         plot_backend: Literal["mpl", "plotly"] = "mpl",
@@ -485,14 +401,51 @@
             {
                 "abs_time": lambda val: f"{val*1e9:,.1f} ns",
                 "duration": lambda val: f"{val*1e9:,.1f} ns",
             }
         )
         return styled_timing_table
 
+    def get_schedule_duration(self):
+        """
+        Method to find the duration of the schedule.
+
+        Returns
+        -------
+        schedule_duration : float
+            Duration of current schedule
+
+        """
+        schedule_duration = 0
+
+        # find last timestamp
+        for schedulable in self.schedulables.values():
+            timestamp = schedulable["abs_time"]
+            operation_repr = schedulable["operation_repr"]
+
+            # find duration of last operation
+            operation = self.data["operation_dict"][operation_repr]
+            pulses_end_times = [
+                pulse.get("duration") + pulse.get("t0")
+                for pulse in operation.data["pulse_info"]
+            ]
+            acquisitions_end_times = [
+                acquisition.get("duration") + acquisition.get("t0")
+                for acquisition in operation.data["acquisition_info"]
+            ]
+            final_op_len = max(pulses_end_times + acquisitions_end_times, default=0)
+            tmp_time = timestamp + final_op_len
+
+            # keep track of longest found schedule
+            if tmp_time > schedule_duration:
+                schedule_duration = tmp_time
+
+        schedule_duration *= self.repetitions
+        return schedule_duration
+
 
 class Schedule(ScheduleBase):  # pylint: disable=too-many-ancestors
     """
     A modifiable schedule.
 
     Operations :class:`quantify_scheduler.operations.operation.Operation` can be added
     using the :meth:`~.Schedule.add` method, allowing precise
@@ -625,15 +578,15 @@
     """
     This class represents an element on a schedule. All elements on a schedule are
     schedulables. A schedulable contains all information regarding the timing of this
     element as well as the operation being executing by this element.
     This operation is currently represented by an operation ID.
 
     Schedulables can contain an arbitrary number of timing constraints to determine the
-    timing. Multiple different contraints are currently resolved by delaying the element
+    timing. Multiple different constraints are currently resolved by delaying the element
     until after all timing constraints have been met, to aid compatibility.
     To specify an exact timing between two schedulables, please ensure to only specify
     exactly one timing constraint.
     """
 
     schema_filename = "schedulable.json"
 
@@ -644,19 +597,26 @@
         ----------
         name
             The name of this schedulable, by which it can be referenced by other
             schedulables. Separate schedulables cannot share the same name
         operation_repr
             The operation which is to be executed by this schedulable
         schedule
-            The schedule to which the schedulable is added. This allows to scheduable to
-            find other elements on the schedule
+            The schedule to which the schedulable is added. This allows schedulable
+            to find other elements on the schedule
         """
         super().__init__()
         if data is not None:
+            warnings.warn(
+                "Support for the data argument will be dropped in"
+                "quantify-scheduler >= 0.13.0.\n"
+                "Please consider updating the data "
+                "dictionary after initialization.",
+                DeprecationWarning,
+            )
             self.data = data
             return
 
         # assert the name is unique
         name_is_unique = (
             len([item for item in schedule["schedulables"].keys() if item == name]) == 0
         )
@@ -722,54 +682,30 @@
             "ref_pt": ref_pt,
         }
         self.data["timing_constraints"].append(timing_constr)
 
     def __str__(self):
         return str(self.data["name"])
 
-    def __repr__(self) -> str:
-        """
-        Returns the string representation  of this instance.
-
-        This represenation can always be evalued to create a new instance.
-
-        .. code-block::
-
-            eval(repr(operation))
-
-        Returns
-        -------
-        :
-        """
-        cls = f"{self.__class__.__name__}"
-        return (
-            f"{cls}(name='{self.data['name']}', "
-            f"operation_repr='', "
-            f"schedule='', "
-            f"data={self.data})"
-        )
-
     def __getstate__(self):
-        return self.data
+        return {"deserialization_type": self.__class__.__name__, "data": self.data}
 
     def __setstate__(self, state):
-        self.data = state
+        self.data = state["data"]
 
 
 # pylint: disable=too-many-ancestors
 class CompiledSchedule(ScheduleBase):
     """
-    A schedule that contains compiled instructions.
-
-    These instructions are ready for execution using the
-    :class:`~.InstrumentCoordinator`.
+    A schedule that contains compiled instructions ready for execution using
+    the :class:`~.InstrumentCoordinator`.
 
     The :class:`CompiledSchedule` differs from a :class:`.Schedule` in
-    that it is considered immutable (no new operations or resources can be added),
-    and that it contains :attr:`~.compiled_instructions`.
+    that it is considered immutable (no new operations or resources can be added), and
+    that it contains :attr:`~.compiled_instructions`.
 
     .. tip::
 
         A :class:`~.CompiledSchedule` can be obtained by compiling a
         :class:`~.Schedule` using :func:`~quantify_scheduler.compilation.qcompile`.
 
     """  # pylint: disable=line-too-long
@@ -890,34 +826,14 @@
     """The datatype returned by the individual acquisitions."""
     acq_indices: Dict[int, List[int]]
     """A dictionary containing the acquisition channel as key and a list of acquisition
     indices that are used for every channel."""
 
     def __getstate__(self):
         data = dataclasses.asdict(self)
-        data["acq_return_type"] = str(self.acq_return_type)
         return {"deserialization_type": self.__class__.__name__, "data": data}
 
     def __setstate__(self, state):
-        return_types = {str(t): t for t in [complex, float, int, bool, str, np.ndarray]}
-
-        if state["data"]["acq_return_type"] in return_types:
-            state["data"]["acq_return_type"] = return_types[
-                state["data"]["acq_return_type"]
-            ]
-        else:
-            raise ValueError(
-                f"AcquisitionMetaData setstate got unknown "
-                f"type: {state['data']['acq_return_type']}"
-            )
-
-        for binmode in enums.BinMode:
-            if state["data"]["bin_mode"] == binmode.value:
-                state["data"]["bin_mode"] = binmode
-                break
-        else:
-            raise ValueError(f"Unknown binmode: {state['data']['bin_mode']}")
-
         state["data"]["acq_indices"] = {
             int(k): v for k, v in state["data"]["acq_indices"].items()
         }
         self.__init__(**state["data"])
```

### Comparing `quantify-scheduler-0.8.0/quantify_scheduler/schedules/spectroscopy_schedules.py` & `quantify-scheduler-0.9.0/quantify_scheduler/schedules/spectroscopy_schedules.py`

 * *Files identical despite different names*

### Comparing `quantify-scheduler-0.8.0/quantify_scheduler/schedules/timedomain_schedules.py` & `quantify-scheduler-0.9.0/quantify_scheduler/schedules/timedomain_schedules.py`

 * *Files identical despite different names*

### Comparing `quantify-scheduler-0.8.0/quantify_scheduler/schedules/trace_schedules.py` & `quantify-scheduler-0.9.0/quantify_scheduler/schedules/trace_schedules.py`

 * *Files identical despite different names*

### Comparing `quantify-scheduler-0.8.0/quantify_scheduler/schedules/verification.py` & `quantify-scheduler-0.9.0/quantify_scheduler/schedules/verification.py`

 * *Files identical despite different names*

### Comparing `quantify-scheduler-0.8.0/quantify_scheduler/schemas/examples/circuit_to_device_example_cfgs.py` & `quantify-scheduler-0.9.0/quantify_scheduler/schemas/examples/circuit_to_device_example_cfgs.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,15 +85,15 @@
                     "acq_duration": 3e-07,
                     "acq_channel": 1,
                 },
             },
         },
     },
     "edges": {
-        "q0-q1": {
+        "q0_q1": {
             "CZ": {
                 "factory_func": "quantify_scheduler.operations."
                 + "pulse_factories.composite_square_pulse",
                 "factory_kwargs": {
                     "square_port": "q0:fl",
                     "square_clock": "cl0.baseband",
                     "square_amp": 0.5,
```

### Comparing `quantify-scheduler-0.8.0/quantify_scheduler/schemas/examples/qblox_test_mapping.json` & `quantify-scheduler-0.9.0/quantify_scheduler/schemas/examples/qblox_test_mapping.json`

 * *Files 25% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9074686164529915%*

 * *Differences: {"'cluster0'": "{'cluster0_module2': {'complex_output_0': {'output_att': 4}, 'complex_output_1': "*

 * *               "OrderedDict([('output_att', 6), ('portclock_configs', [OrderedDict([('port', "*

 * *               "'q6:mw'), ('clock', 'q6.01'), ('interm_freq', 50000000.0)])])])}, "*

 * *               "'cluster0_module4': {'complex_output_0': {'portclock_configs': {insert: [(1, "*

 * *               "OrderedDict([('port', 'q5:mw'), ('clock', 'q5.01'), ('interm_freq', "*

 * *               "50000000.0)]))]}, 'output_att': 12, ' […]*

```diff
@@ -12,24 +12,81 @@
                         "mixer_phase_error_deg": -4.2,
                         "port": "q4:mw"
                     }
                 ]
             },
             "instrument_type": "QCM"
         },
+        "cluster0_module10": {
+            "instrument_type": "QCM",
+            "real_output_0": {
+                "portclock_configs": [
+                    {
+                        "clock": "cl0.baseband",
+                        "port": "q0:fl"
+                    }
+                ]
+            },
+            "real_output_1": {
+                "portclock_configs": [
+                    {
+                        "clock": "cl0.baseband",
+                        "port": "q1:fl"
+                    }
+                ]
+            },
+            "real_output_2": {
+                "portclock_configs": [
+                    {
+                        "clock": "cl0.baseband",
+                        "port": "q2:fl"
+                    }
+                ]
+            },
+            "real_output_3": {
+                "portclock_configs": [
+                    {
+                        "clock": "cl0.baseband",
+                        "port": "q3:fl"
+                    }
+                ]
+            }
+        },
+        "cluster0_module12": {
+            "instrument_type": "QCM",
+            "real_output_0": {
+                "portclock_configs": [
+                    {
+                        "clock": "cl0.baseband",
+                        "port": "q4:fl"
+                    }
+                ]
+            }
+        },
         "cluster0_module2": {
             "complex_output_0": {
+                "output_att": 4,
                 "portclock_configs": [
                     {
                         "clock": "q5.01",
                         "interm_freq": 50000000.0,
                         "port": "q5:mw"
                     }
                 ]
             },
+            "complex_output_1": {
+                "output_att": 6,
+                "portclock_configs": [
+                    {
+                        "clock": "q6.01",
+                        "interm_freq": 50000000.0,
+                        "port": "q6:mw"
+                    }
+                ]
+            },
             "instrument_type": "QCM_RF"
         },
         "cluster0_module3": {
             "complex_output_0": {
                 "dc_mixer_offset_I": -0.054,
                 "dc_mixer_offset_Q": -0.034,
                 "lo_name": "lo1",
@@ -43,19 +100,26 @@
                     }
                 ]
             },
             "instrument_type": "QRM"
         },
         "cluster0_module4": {
             "complex_output_0": {
+                "input_att": 10,
+                "output_att": 12,
                 "portclock_configs": [
                     {
                         "clock": "q5.ro",
                         "interm_freq": 50000000.0,
                         "port": "q5:res"
+                    },
+                    {
+                        "clock": "q5.01",
+                        "interm_freq": 50000000.0,
+                        "port": "q5:mw"
                     }
                 ]
             },
             "instrument_type": "QRM_RF"
         },
         "instrument_type": "Cluster",
         "ref": "internal"
@@ -106,14 +170,16 @@
                     "mixer_amp_ratio": 0.9998,
                     "mixer_phase_error_deg": -4.1,
                     "port": "q0:mw"
                 }
             ]
         },
         "complex_output_1": {
+            "dc_mixer_offset_I": 0.2345,
+            "dc_mixer_offset_Q": 1.337,
             "lo_name": "lo1",
             "portclock_configs": [
                 {
                     "clock": "q1.01",
                     "interm_freq": null,
                     "port": "q1:mw"
                 }
@@ -149,14 +215,16 @@
         "instrument_type": "Pulsar_QCM_RF",
         "ref": "internal"
     },
     "qrm0": {
         "complex_output_0": {
             "dc_mixer_offset_I": -0.054,
             "dc_mixer_offset_Q": -0.034,
+            "input_gain_I": 2,
+            "input_gain_Q": 3,
             "lo_name": "lo1",
             "portclock_configs": [
                 {
                     "clock": "q0.ro",
                     "interm_freq": null,
                     "mixer_amp_ratio": 0.9997,
                     "mixer_phase_error_deg": -4.0,
@@ -182,14 +250,42 @@
                     "port": "q1:res"
                 }
             ]
         },
         "instrument_type": "Pulsar_QRM",
         "ref": "external"
     },
+    "qrm2": {
+        "instrument_type": "Pulsar_QRM",
+        "real_output_0": {
+            "input_gain": 1,
+            "portclock_configs": [
+                {
+                    "clock": "cl0.baseband",
+                    "interm_freq": null,
+                    "mixer_amp_ratio": 0.9997,
+                    "mixer_phase_error_deg": -4.0,
+                    "port": "q0:fl"
+                }
+            ]
+        },
+        "real_output_1": {
+            "input_gain": 3,
+            "portclock_configs": [
+                {
+                    "clock": "cl0.baseband",
+                    "interm_freq": null,
+                    "mixer_amp_ratio": 0.9997,
+                    "mixer_phase_error_deg": -4.0,
+                    "port": "q1:fl"
+                }
+            ]
+        },
+        "ref": "external"
+    },
     "qrm_rf0": {
         "complex_output_0": {
             "dc_mixer_offset_I": -0.046,
             "dc_mixer_offset_Q": -0.036,
             "lo_freq": 7200000000.0,
             "portclock_configs": [
                 {
```

### Comparing `quantify-scheduler-0.8.0/quantify_scheduler/schemas/examples/transmon_test_config.json` & `quantify-scheduler-0.9.0/quantify_scheduler/schemas/examples/transmon_test_config.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8333333333333334%*

 * *Differences: {"'edges'": "{replace: OrderedDict([('q0_q1', OrderedDict([('resource_map', OrderedDict([('q0', "*

 * *            "'q0:fl'), ('q1', 'q1:fl')])), ('params', OrderedDict([('flux_duration', 4e-08), "*

 * *            "('flux_amp_control', 0.5), ('flux_amp_target', 0), ('phase_correction_control', 0), "*

 * *            "('phase_correction_target', 0)]))])), ('q2_q0', OrderedDict([('resource_map', "*

 * *            "OrderedDict([('q2', 'q2:fl'), ('q0', 'q0:fl')])), ('params', "*

 * *            "OrderedDict([('flux_duration', 3.2e-08 […]*

```diff
@@ -1,24 +1,24 @@
 {
     "backend": "quantify_scheduler.compilation.add_pulse_information_transmon",
     "edges": {
-        "q0-q1": {
+        "q0_q1": {
             "params": {
                 "flux_amp_control": 0.5,
                 "flux_amp_target": 0,
                 "flux_duration": 4e-08,
                 "phase_correction_control": 0,
                 "phase_correction_target": 0
             },
             "resource_map": {
                 "q0": "q0:fl",
                 "q1": "q1:fl"
             }
         },
-        "q2-q0": {
+        "q2_q0": {
             "params": {
                 "flux_amp_control": 0.5,
                 "flux_amp_target": 0,
                 "flux_duration": 3.2e-08,
                 "phase_correction_control": 0,
                 "phase_correction_target": 0
             },
```

### Comparing `quantify-scheduler-0.8.0/quantify_scheduler/schemas/examples/utils.py` & `quantify-scheduler-0.9.0/quantify_scheduler/schemas/examples/utils.py`

 * *Files identical despite different names*

### Comparing `quantify-scheduler-0.8.0/quantify_scheduler/schemas/examples/zhinst_test_mapping.json` & `quantify-scheduler-0.9.0/quantify_scheduler/schemas/examples/zhinst_test_mapping.json`

 * *Files 13% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.986111111111111%*

 * *Differences: {"'devices'": "{0: {'type': 'HDAWG8', 'channel_2': OrderedDict([('port', 'q2:mw'), ('clock', "*

 * *              "'q2.01'), ('mode', 'complex'), ('modulation', OrderedDict([('type', 'premod'), "*

 * *              "('interm_freq', -100000000.0)])), ('local_oscillator', 'mw_qubit_ch2'), "*

 * *              "('clock_frequency', 6000000000.0), ('markers', ['AWG_MARKER1', 'AWG_MARKER2']), "*

 * *              "('gain1', 1), ('gain2', 1), ('mixer_corrections', OrderedDict([('amp_ratio', 0.95), "*

 * *              "('phase_error', 0.0 […]*

```diff
@@ -44,19 +44,65 @@
                 "mode": "complex",
                 "modulation": {
                     "interm_freq": -100000000.0,
                     "type": "premod"
                 },
                 "port": "q1:mw"
             },
+            "channel_2": {
+                "clock": "q2.01",
+                "clock_frequency": 6000000000.0,
+                "gain1": 1,
+                "gain2": 1,
+                "local_oscillator": "mw_qubit_ch2",
+                "markers": [
+                    "AWG_MARKER1",
+                    "AWG_MARKER2"
+                ],
+                "mixer_corrections": {
+                    "amp_ratio": 0.95,
+                    "dc_offset_I": 0.042,
+                    "dc_offset_Q": 0.028,
+                    "phase_error": 0.07
+                },
+                "mode": "complex",
+                "modulation": {
+                    "interm_freq": -100000000.0,
+                    "type": "premod"
+                },
+                "port": "q2:mw"
+            },
+            "channel_3": {
+                "clock": "q3.01",
+                "clock_frequency": 6000000000.0,
+                "gain1": 1,
+                "gain2": 1,
+                "local_oscillator": "mw_qubit_ch2",
+                "markers": [
+                    "AWG_MARKER1",
+                    "AWG_MARKER2"
+                ],
+                "mixer_corrections": {
+                    "amp_ratio": 0.95,
+                    "dc_offset_I": 0.042,
+                    "dc_offset_Q": 0.028,
+                    "phase_error": 0.07
+                },
+                "mode": "complex",
+                "modulation": {
+                    "interm_freq": -100000000.0,
+                    "type": "premod"
+                },
+                "port": "q3:mw"
+            },
             "channelgrouping": 0,
             "clock_select": 0,
             "name": "ic_hdawg0",
             "ref": "int",
-            "type": "HDAWG4"
+            "type": "HDAWG8"
         },
         {
             "channel_0": {
                 "clock": "q0.ro",
                 "clock_frequency": 6000000000.0,
                 "local_oscillator": "mw_readout",
                 "mode": "real",
```

### Comparing `quantify-scheduler-0.8.0/quantify_scheduler/schemas/operation.json` & `quantify-scheduler-0.9.0/quantify_scheduler/schemas/operation.json`

 * *Files identical despite different names*

### Comparing `quantify-scheduler-0.8.0/quantify_scheduler/schemas/schedulable.json` & `quantify-scheduler-0.9.0/quantify_scheduler/schemas/schedulable.json`

 * *Files identical despite different names*

### Comparing `quantify-scheduler-0.8.0/quantify_scheduler/schemas/schedule.json` & `quantify-scheduler-0.9.0/quantify_scheduler/schemas/schedule.json`

 * *Files identical despite different names*

### Comparing `quantify-scheduler-0.8.0/quantify_scheduler/schemas/transmon_cfg.json` & `quantify-scheduler-0.9.0/quantify_scheduler/schemas/transmon_cfg.json`

 * *Files 18% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9958333333333333%*

 * *Differences: {"'properties'": '{\'edges\': {\'description\': "A dictionary with pairs of qubit names separated '*

 * *                 "by an underscore (str) as keys e.g., 'q0_q1'. \\nThe items contain the "*

 * *                 'informatation to compile gates on pairs of qubits to pulses acting on ports and '*

 * *                 'clocks using the specified backend."}}'}*

```diff
@@ -3,15 +3,15 @@
     "description": "JSON schema for a transmon based device configuration.",
     "properties": {
         "backend": {
             "description": "Specifies the function used for compiling from gate-level to pulse-level description. \nA valid specification is a period separated string e.g., 'quantify_scheduler.compilation.add_pulse_information_transmon'.",
             "type": "string"
         },
         "edges": {
-            "description": "A dictionary with pairs of qubit names separated by a dash (str) as keys e.g., 'q0-q1'. \nThe items contain the informtation to compile gates on pairs of qubits to pulses acting on ports and clocks using the specified backend.",
+            "description": "A dictionary with pairs of qubit names separated by an underscore (str) as keys e.g., 'q0_q1'. \nThe items contain the informatation to compile gates on pairs of qubits to pulses acting on ports and clocks using the specified backend.",
             "type": "object"
         },
         "qubits": {
             "description": "A dictionary with qubit names (str) as keys e.g., 'q0'. \nThe items contain the informtation to compile gates on individual qubits to pulses acting on ports and clocks using the specified backend.",
             "type": "object"
         }
     },
```

### Comparing `quantify-scheduler-0.8.0/quantify_scheduler/structure/model.py` & `quantify-scheduler-0.9.0/quantify_scheduler/structure/model.py`

 * *Files 7% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 
     This class is a pre-configured `pydantic <https://pydantic-docs.helpmanual.io/>`_
     model. See its documentation for details of usage information.
 
     .. admonition:: Examples
         :class: dropdown
 
-        .. include:: ../../../../examples/structure.DataStructure.py.rst
+        .. include:: ../../../../examples/structure.DataStructure.rst
     """
 
     class Config:  # pylint: disable=too-few-public-methods,missing-class-docstring
         json_loads = orjson.loads
         json_dumps = orjson_dumps
 
         # ensures exceptions are raised when passing extra argument that are not
```

### Comparing `quantify-scheduler-0.8.0/quantify_scheduler/visualization/circuit_diagram.py` & `quantify-scheduler-0.9.0/quantify_scheduler/visualization/circuit_diagram.py`

 * *Files identical despite different names*

### Comparing `quantify-scheduler-0.8.0/quantify_scheduler/visualization/pulse_diagram.py` & `quantify-scheduler-0.9.0/quantify_scheduler/visualization/pulse_diagram.py`

 * *Files identical despite different names*

### Comparing `quantify-scheduler-0.8.0/quantify_scheduler/visualization/pulse_scheme.py` & `quantify-scheduler-0.9.0/quantify_scheduler/visualization/pulse_scheme.py`

 * *Files identical despite different names*

### Comparing `quantify-scheduler-0.8.0/quantify_scheduler/waveforms.py` & `quantify-scheduler-0.9.0/quantify_scheduler/waveforms.py`

 * *Files identical despite different names*

### Comparing `quantify-scheduler-0.8.0/quantify_scheduler.egg-info/PKG-INFO` & `quantify-scheduler-0.9.0/quantify_scheduler.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,553 +1,521 @@
-Metadata-Version: 2.1
-Name: quantify-scheduler
-Version: 0.8.0
-Summary: Quantify-scheduler is a python package for writing quantum programs featuring a hybrid gate-pulse control model with explicit timing control.
-Home-page: https://gitlab.com/quantify-os/quantify-scheduler
-Author: The Quantify consortium consisting of Qblox and Orange Quantum Systems
-Author-email: maintainers@quantify-os.org
-License: BSD-3 license
-Keywords: quantify-scheduler
-Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.8
-License-File: LICENSE
-License-File: AUTHORS.rst
-
-==================
-quantify-scheduler
-==================
-
-.. image:: https://img.shields.io/badge/slack-chat-green.svg
-    :target: https://join.slack.com/t/quantify-hq/shared_invite/zt-vao45946-f_NaRc4mvYQDQE_oYB8xSw
-    :alt: Slack
-
-.. image:: https://gitlab.com/quantify-os/quantify-scheduler/badges/main/pipeline.svg
-    :target: https://gitlab.com/quantify-os/quantify-scheduler/pipelines/
-    :alt: Pipelines
-
-.. image:: https://img.shields.io/pypi/v/quantify-scheduler.svg
-    :target: https://pypi.org/pypi/quantify-scheduler
-    :alt: PyPi
-
-.. image:: https://app.codacy.com/project/badge/Grade/0c9cf5b6eb5f47ffbd2bb484d555c7e3
-    :target: https://www.codacy.com/gl/quantify-os/quantify-scheduler/dashboard?utm_source=gitlab.com&amp;utm_medium=referral&amp;utm_content=quantify-os/quantify-scheduler&amp;utm_campaign=Badge_Grade
-    :alt: Code Quality
-
-.. image:: https://app.codacy.com/project/badge/Coverage/0c9cf5b6eb5f47ffbd2bb484d555c7e3
-    :target: https://www.codacy.com/gl/quantify-os/quantify-scheduler/dashboard?utm_source=gitlab.com&amp;utm_medium=referral&amp;utm_content=quantify-os/quantify-scheduler&amp;utm_campaign=Badge_Coverage
-    :alt: Coverage
-
-.. image:: https://readthedocs.com/projects/quantify-quantify-scheduler/badge/?version=latest&token=ed6fdbf228e1369eacbeafdbad464f6de927e5dfb3a8e482ad0adcbea76fe74c
-    :target: https://quantify-quantify-scheduler.readthedocs-hosted.com
-    :alt: Documentation Status
-
-.. image:: https://img.shields.io/badge/License-BSD%203--Clause-blue.svg
-    :target: https://gitlab.com/quantify-os/quantify-scheduler/-/raw/main/LICENSE
-    :alt: License
-
-.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
-    :target: https://github.com/psf/black
-    :alt: Code style
-
-.. image:: https://img.shields.io/badge/Supported%20By-UNITARY%20FUND-brightgreen.svg?style=flat
-    :target: http://unitary.fund
-    :alt: Unitary Fund
-
-.. figure:: /images/QUANTIFY_LANDSCAPE.svg
-    :align: center
-    :alt: Quantify logo
-
-Quantify is a python based data acquisition platform focused on Quantum Computing and solid-state physics experiments.
-It is build on top of `QCoDeS <https://qcodes.github.io/Qcodes/>`_ and is a spiritual successor of `PycQED <https://github.com/DiCarloLab-Delft/PycQED_py3>`_.
-Quantify currently consists of `quantify-core <https://pypi.org/project/quantify-core/>`_ and `quantify-scheduler <https://pypi.org/project/quantify-scheduler/>`_.
-
-Take a look at the `latest documentation for quantify-scheduler <https://quantify-quantify-scheduler.readthedocs-hosted.com/>`_ or use the switch in the bottom of left panel to read the documentation for older releases.
-
-Quantify-scheduler is a python module for writing quantum programs featuring a hybrid gate-pulse control model with explicit timing control.
-The control model allows quantum gate- and pulse-level descriptions to be combined in a clearly defined and hardware-agnostic way.
-Quantify-scheduler is designed to allow experimentalists to easily define complex experiments, and produces synchronized pulse schedules to be distributed to control hardware.
-
-.. caution::
-
-    This is a pre-release **alpha version**, major changes are expected. Use for testing & development purposes only.
-
-About
------
-
-Quantify-scheduler is maintained by The Quantify consortium consisting of Qblox and Orange Quantum Systems.
-
-.. |_| unicode:: 0xA0
-   :trim:
-
-
-.. figure:: https://cdn.sanity.io/images/ostxzp7d/production/f9ab429fc72aea1b31c4b2c7fab5e378b67d75c3-132x31.svg
-    :width: 200px
-    :target: https://qblox.com
-    :align: left
-
-.. figure:: https://orangeqs.com/OQS_logo_with_text.svg
-    :width: 200px
-    :target: https://orangeqs.com
-    :align: left
-
-|_|
-
-
-|_|
-
-The software is free to use under the conditions specified in the `license <https://gitlab.com/quantify-os/quantify-scheduler/-/raw/main/LICENSE>`_.
-
-.. nothing-to-avoid-a-sphinx-warning:
-
-
-=======
-Credits
-=======
-
-Contributors
-------------
-
-* Adam Lawrence <adam@orangeqs.com>
-* Adriaan Rol <adriaan@orangeqs.com>
-* Callum Attryde <cattryde@qblox.com>
-* Christian Dickel <christiandickel8@gmail.com>
-* Damaz de Jong <ddejong@qblox.com>
-* Damien Crielaard <dcrielaard@qblox.com>
-* Diogo Valada <dvalada@qblox.com>
-* Edgar Reehuis <ereehuis@qblox.com>
-* Gabor Oszkar Denes <gdenes@qblox.com>
-* Gijs Vermarien <gijs@orangeqs.com>
-* Jordy Gloudemans <jgloudemans@qblox.com>
-* Jules van Oven <jules@qblox.com>
-* Kelvin Loh <kelvin@orangeqs.com>
-* Luis Miguens Fernandez <lmiguens@qblox.com>
-* Michiel Dubbelman <michiel@orangeqs.com>
-* Pieter Eendebak <pieter.eendebak@tno.nl>
-* Robert Sokolewicz <rsokolewicz@qblox.com>
-* Thomas Reynders <thomas@orangeqs.com>
-* Viacheslav Ostroukh <viacheslav@orangeqs.com>
-* Victor Negirneac <vnegirneac@qblox.com>
-
-
-=========
-Changelog
-=========
-
-0.8.0 Support for two qubit operations and basic CZ-gate implementation (2022-08-10)
-------------------------------------------------------------------------------------
-
-Breaking changes
-~~~~~~~~~~~~~~~~
-* Operations - Pin `qcodes` package to <0.34.0 due to breaking `Edge` naming (#300, !409)
-* Qblox backend - Sequencers are now dynamically allocated. The hardware config file schema was changed. (!328)
-    - For each instrument, the config now contains a `portclock_configs` entry, a list with a dictionary of settings per port-clock combination
-    - See https://quantify-quantify-scheduler.readthedocs-hosted.com/en/0.8.0/tutorials/qblox/recent.html
-* Qblox backend - Strictly requires v0.7.x of the `qblox-instruments` package (!449)
-* Zhinst backend - Strictly requires v21.8.20515 of the `zhinst` package (!387)
-
-Merged branches and closed issues
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-* Compilation - Added `acq_protocol` optional parameter to the `Measure` gate. (!386)
-* Compilation - Call `determine_absolute_timing` in `qcompile` when no `device_cfg` supplied. (!436)
-* Compilation - Decrease test usage of deprecated transmon_test_config.json / add_pulse_information_transmon (!450)
-* DRAG Pulse - Removed an extra G_amp factor from the Q component (derivative pulse). (#298, !406)
-* Docs - Fix API reference pages on read-the-docs (#303, !413)
-* Docs - Pin sphinx to 5.0.2 due to crash in napoleon (!437)
-* Docs - Unpin sphinx >=5.1.1 (!445)
-* Docs - Fix jsonschemas not rendered on read-the-docs (!448)
-* Docs - Clarify port and clock concepts (!431)
-* Docs - New scheduler tutorials: Schedules and Pulses; Compiling to Hardware; Operations and Qubits (!336, !439)
-* Gettables - Added `generate_diagnostic_report` method to save the internal state of `ScheduleGettable` to a zip-file. (!408)
-* Helpers - Moved `MockLocalOscillator` definition from tests to `helpers.mock_instruments.MockLocalOscillator` (!392, !336).
-* JSON utilities - Add JSON serialization/deserialization methods based on `__getstate__`/`__setstate__` (!444)
-* Operations - Added a `symmetric` key in the `gate_info` to flag symmetric operations. (!389)
-* Operations - Introduce basic CZ-gate via `CompositeSquareEdge` (utilizing `quantify_scheduler.operations.pulse_factories.composite_square_pulse`) (!411)
-    - Replaces the incomplete `SuddenNetZeroEdge` basic CZ-gate implementation
-* Operations - Rxy theta rotations now fall into the domain of [-180 to 180) degrees. (!433)
-* QuantumDevice - Added implementation for `edges` in the quantum device config in order to support two qubit operations. (!389)
-    - The `Edge` has been added as an abstract base class for edges to be added to a device.
-* Qblox backend - Only add clocks to the schedule that are actually being used, avoids trying to assign frequencies for unused clocks (#278, !371)
-* Qblox backend - Fix for supplying negative NCO phase (!393)
-* Qblox backend - Fix compilation of ShiftClockPhase (!404, broken by merge of !328)
-* Qblox backend - Fix for outputting signals on even output paths of qblox hardware in real_output_x mode (!397)
-* Qblox backend - Make Qblox backend compatible with generic downconverter values in hardware_config (!418)
-* Qblox backend - Fix for 90 degree phase shift on even output paths as a result of the !397 hotfix. (!412)
-* Qblox backend - Fix cluster compatibility when converting old hwconfig to new specs (!419)
-* Qblox backend - Latency corrections must now be defined in top layer of hw config (!400)
-* Qblox backend - Fix combination of cluster and latency corrections when converting hw_configs to new specs  (!417)
-* Qblox backend - Fix handling of composite pulses (#299, !411)
-* Qblox backend - Implementation of distortion correction (#285, !388)
-* Qblox backend - Fix incompatibility of distortion_correction parameters as numpy arrays (!426)
-* Qblox backend - Remove all references to the inactive `line_gain_db` param (!435)
-* Qblox ICCs - Fix for setting `scope_acq_sequencer_select` for QRM and QRM-RF (!432, !441)
-* Qblox ICCs - Fix `ClusterComponent.prepare` mutating the schedule (!443)
-* Schedules - Revert rename of `trace_schedule` done in !432 and rename new schedule using gates to `trace_schedule_circuit_layer` (!442)
-* Schedules - Make `AcquisitionMetadata` a serializable class (!446)
-
-
-0.7.0 Support for qblox-instruments v0.6.0, new BasicTransmonElement, change for triggers in Zhinst backend (2022-04-11)
-------------------------------------------------------------------------------------------------------------------------
-
-Breaking changes
-~~~~~~~~~~~~~~~~
-* Qblox ICCs - Updated Qblox components for using the new unified-style qblox driver (see https://gitlab.com/quantify-os/quantify-scheduler/-/wikis/Qblox-ICCs:-Interface-changes-in-using-qblox-instruments-v0.6.0) (!377).
-* Qblox backend - Strictly requires v0.6.0 of the qblox-instruments package (!377).
-* Zhinst backend - Hardware config for the devices. Replaced keyword "triggers" to "trigger", and the value type from `List[int]` to `int`. E.g. old style, `"triggers": [2]`, new style, `"trigger": 2` (#264, !372).
-
-Merged branches and closed issues
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-* QuantumDevice - The `DeviceElement` has been added as an abstract base class for elements to be added to a device (#148, !374).
-* QuantumDevice - The `BasicTransmonElement` has been added that generates a device config in a more structured manner (#246, !374).
-* QuantumDevice - Fixed a bug in the `BasicTransmonElement` where operations had clock-frequencies (`float`) specified instead of clocks (`str`) (!379).
-* QuantumDevice - The `TransmonElement` will be deprecated after version 0.8 (!374).
-
-
-0.6.0 Full support for multiplexed readout, transmon element update, fixes to backends (2022-03-10)
----------------------------------------------------------------------------------------------------
-
-Breaking changes
-~~~~~~~~~~~~~~~~
-* Compilation - Deprecated `add_pulse_information_transmon` in favor of `compilation.backends.circuit_to_device.compile_circuit_to_device` (#64, #67, !339).
-* Compilation - attempting compilation with missing values in the `DeviceCompilationConfig` configuration will now raise validation errors. Be sure to set initial values when generating a config using the `QuantumDevice` object (!339)
-* Compilation - Device compile making use of `.compile_circuit_to_device` no longer modifies the input schedule (#249, !339).
-* Compilation - When specifying multiple timing constraints for a schedulable, the constraint specifying the latest time determines the absolute time of the shedulable (!309)
-* Gettables - `ScheduleGettableSingleChannel` renamed to `ScheduleGettable` as it now supports multiple acquisition channels (!299).
-* Hardware config - Removed the need for a `ic_` prefix from the hardware config (!312).
-* Instrument Coordinator - IC now adds a `GenericInstrumentCoordinatorComponent` to itself on instantiation by default (!350)
-* Instrument Coordinator - IC stop function has an `allow_failure` parameter which allows IC components attached to it to fail to stop with warning instead of raising errors. Allows for situations when some components cannot have a stop instruction sent before the prepare stage. (!359)
-* Operations - The internal behavior of how acquisition channels and acquisition indices are configured in the `Measure` operation has changed slightly. See #262 for details. (!339).
-* Operations - Added "operation_type" key to the schema. (!345)
-* Structure - `Schedule.timing_constraints` has been renamed to `Schedule.schedulables`. It now points to a dictionary of schedulables rather than a list of dicts. (!309)
-* Structure - Pydantic-based model is now used for the data structures. (!341)
-* Visualization - Deprecated `plot_circuit_diagram_mpl` and `plot_pulse_diagram_mpl` in `ScheduleBase` in favour of `plot_circuit_diagram` and `plot_pulse_diagram` (!313)
-* Qblox backend - Strictly requires v0.5.4 of the qblox-instruments package (!314)
-* Zhinst backend - Due to !312, the csv files used to upload the waveforms to the UHFQA no longer use the `ic_` prefix in their filenames. (!334)
-* Zhinst backend - Fixes bug when doing SSRO experiments. No more duplicated shots. Adds support for BinMode.APPEND during compilation. (#276, !358)
-* Zhinst backend - Removed `latency` and `line_trigger_delay` keys in the channels of the devices for the Zhinst hardware config. (!363)
-* Zhinst backend - Added `latency_corrections` main entry in the Zhinst hardware config for latency corrections on a port-clock combination basis. (!363)
-
-Merged branches and closed issues
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-* Compilation - Added a new compilation backend `compilation.backends.circuit_to_device.compile_circuit_to_device` for the quantum-circuit to quantum-device layer (#64, #67, !339).
-* Compilation - Fixed `add_pulse_information_transmon` when using "Trace" acquisition mode (!300)
-* Compilation - Fixed the deprecation warnings from pandas `DataFrame.append`. (!347)
-* Docs - Pinning qcodes package to <0.32.0 due to Read the Docs API reference failure (!361)
-* Gettables - `ScheduleGettable` now first stops all instruments in IC during initialization (!324)
-* Schedules - Adds a multiplexing verification schedule. (!329)
-* Operations - Sudden Net Zero from Negirneac 2021 added to the `pulse_library` (!339)
-* Operations - Docstrings for the X90, X, Y90, Y, and Rxy gate unitary have been aligned with literature. (#261, !305)
-* Operations - Adds an optional "data" argument to staircase pulse. (!335)
-* Pulse library - Added `ShiftClockPhase` operation that can be used to shift the phase of a clock during execution of a `Schedule` (!346)
-* Pulse library - Added a numerically defined pulse. (!157)
-* QuantumDevice - Unknown values are initialized as `float('nan')` (#274, !356)
-* TransmonElement - Corrected the motzoi parameter range validator. (!351)
-* Visualization - Adds visualisation of acquisitions to plotly pulse diagrams (!304)
-* Visualization - Add `plot_pulse_diagram` and `plot_circuit_diagram` to schedule for easier method names, and enable plotly visualization directly from `ScheduleBase` (!313)
-* Utilities - Migrates the utilities from quantify-core. (!357)
-* Generic ICC - Adds support for nested parameters. (!330)
-* Qblox ICCs - Stop now disables sync on all sequencers to prevent hanging during next run, where it gets re-enabled if needed (!324)
-* Qblox ICCs - `_QRMAcquisitionManager._get_scope_data` now has correct return type (#232, !300)
-* Qblox ICCs - Fixed bug where QRM scope mode sequencer does not get set correctly (!342)
-* Qblox ICCs - Fixed reference source cluster issue when it is not being set correctly. (!323)
-* Qblox backend - NCO phase now gets reset every averaging loop (!337)
-* Qblox backend - Enables RF output switch at the start of a program. (!344)
-* Qblox backend - Added logic for changing the NCO phase during execution of a `Schedule` (!346)
-* Qblox backend - Added ability to correct for latency by delaying program execution on a per sequencer basis (!325)
-* Qblox backend - Compilation with local oscillators changed to work with generic instrument coordinator components (!306)
-* Qblox backend - Refactored operation handling and greatly increased test coverage (!301).
-* Qblox backend - Made max duration of wait instructions (!319).
-* Qblox backend - Fixed an issue with the downconverter frequency correction. (!318)
-* Qblox backend - Temporary fix for a floating point rounding error when calculating the length of pulses. (#284, !365)
-* Zhinst backend - Fixed the ZI resolver return typehint. (!307)
-* Zhinst backend - Fixed an issue when compiling seqc programs for multiple sequencers end up overwriting the first sequencer. (!340, #260)
-
-
-0.5.2 Fixes to backends, and other incremental fixes  (2021-12-08)
-------------------------------------------------------------------
-
-Breaking changes
-~~~~~~~~~~~~~~~~
-* Dependency on `jsonschema` has been replaced with `fastjsonschema`. (!284, !293)
-* Zhinst hardware config json schema has changed. See the example schema. (!283)
-* In `hardware_compile` function, the `hardware_map` is changed to `hardware_cfg` parameter. (!279)
-* Remove enum tools dependency (!270)
-
-Merged branches and closed issues
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-
-* Compilation - The `determine_absolute_scheduling` function now sorts the list of labels in the timing constraints, and then a binary search (via `np.searchsorted`) is applied. (!272, !274)
-* Compilation - Make `device_cfg` an optional argument of qcompile(!281)
-* Compilation - renamed the hardware_mapping argument of qcompile into hardware_cfg (#165, !279)
-* Compilation - Introduced the hardware_compile function to perform the hardware compilation returning a CompiledSchedule (#224, !279)
-* Docs - Updating user guide to mention correctly the QuantumDevice and ScheduleGettable(s) available. (!209)
-* Infrastructure - Adds rich package in the requirements since tutorials use it. (!276)
-* Operations - The `locate` function now uses the `functools.lru_cache` to cache the result (only for python >= 3.8). For python 3.7, behaviour remains the same.  (!273, !275)
-* Operations - Resolved a minor issue where identical Rxy rotations (for angles >360) would be treated as separate operations in a schedule (!263)
-* Visualization - Adds a function `plot_acquisition_operations` which together with the new `AcquisitionOperation` class will help highlight acquisition pulses in the pulse diagrams. (!271, !277)
-* Zhinst backend - Large parts of the Zhinst backend have been rewritten. This should resolve a range of issues. (!263)
-    - Calculation of the timelines for different operations now makes using of a timing table, improving code readability and debugability.
-    - Timing issues related to triggering should be resolved (#218)
-    - The backend can now always use the same hardware configuration file (#214)
-    - Acquisition is now done using the StartQA instruction (#213)
-    - error handling in the Zhinst backend has been improved catching several exceptions at compile time of the schedule instead of manifesting in unexpected results during runtime.
-    - Local oscillators through the ZI backend uses the GenericInstrumentCoordinatorComponent. Configures other parameters other than frequency. (!283, #204)
-* Qblox backend - only check major and minor version when checking compatibility with the qblox_instruments package (!290)
-    - Added support for the Qblox Downconverter (!297)
-    - Added workaround for staircase_amplitude. (!292)
-    - Fix looped acquisition integration time, fix acquire index offset by one (!291)
-    - Qblox instruments version == 0.5.3 (!289)
-    - Fix sequencer_sync_en not being reset in the qblox instrument coordinator component. (!285)
-    - Fix rounding of time to samples in qblox backend (!282)
-    - Fix pulse stitching at zero amplitude. (!280)
-    - Allow instruction generated staircase with modulation (!278)
-* Utilities - Improve JSON validation speed (!284)
-* Utilities - Improve operation deserialization speed (!273)
-* Bugfix - For calculating the pulse area, the mathematical area is used instead of area of sampled pulse. (!242, !286)
-* Bugfix - Fix for plot window operations (!294)
-
-
-0.5.1 Incremental fixes, refactoring, and addition of convenience methods and classes (2021-11-11)
---------------------------------------------------------------------------------------------------
-
-Breaking changes
-~~~~~~~~~~~~~~~~
-* InstrumentCoordinator - `last_schedule` is now a property (!252).
-* Structure - We have refactored the Operation and Schedule classes out of the types module and moved the different operation libraries (acquisition_library, gate_library, and pulse_library) (#217, !256).
-    * `quantify_scheduler.types.Operation` -> `quantify_scheduler.operations.operation.Operation`, the import `quantify_scheduler.Operation` still works.
-    * `quantify_scheduler.types.Schedule` -> `quantify_scheduler.schedules.schedule.Schedule`, the import `quantify_scheduler.Schedule` still works.
-    * `quantify_scheduler.types.CompiledSchedule` -> `quantify_scheduler.schedules.schedule.CompiledSchedule`
-    * `quantify_scheduler.types.ScheduleBase` -> `quantify_scheduler.schedules.schedule.ScheduleBase`
-    * `quantify_scheduler.types.AcquisitionMetadata` -> `quantify_scheduler.schedules.schedule.AcquisitionMetadata`
-    * `quantify_scheduler.acquisition_library` -> `quantify_scheduler.operations.acquisition_library`
-    * `quantify_scheduler.gate_library` -> `quantify_scheduler.operations.gate_library`
-    * `quantify_scheduler.pulse_library` -> `quantify_scheduler.operations.pulse_library`
-
-Merged branches and closed issues
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-* Control - Add option to set output port in heterodyne_spec_sched (!262)
-* Control - Expand SingleChannelScheduleGettable to support trace acquisitions (!248)
-* Control - Update create_dc_compensation_pulse behaviour and docstring. (!244)
-* Control - Refactor ScheduleGettableSingleChannel (!240, !249)
-* Control - Reduce the default init_duration of spectroscopy schedules (!237)
-* Generic ICC - Added a GenericInstrumentCoordinatorComponent. (!267)
-* ICCs - InstrumentCoordinatorComponentBase now has a `force_set_parameter` as a ManualParameter to enable the user to switch the lazy_set behaviour when setting parameters of the instruments connected to the InstrumentCoordinatorComponent. (!267)
-* Qblox ICCs - Adds a lazy_set behaviour by default when setting parameters with the same value to an instrument connected to the Qblox ICC. (!230)
-* Visualization - made matplotlib schedule visualization methods accessible as methods `plot_circuit_diagram_mpl` and `plot_pulse_diagram_mpl` of the `Schedule` class (!253)
-* Visualization - resolved a bug where a schedule was modified when drawing a circuit diagram (#197, !250)
-* Visualization - Add support for window operation to transmon backend (!245)
-* Infrastructure - Fix and enhance pre-commit + add to CI (!257, !265)
-* Infrastructure - Added prospector config file for CI. (!261)
-* Bugfix - Removed redundant `determine_absolute_timing` step in `qcompile`. (!259)
-* Bugfix - Ramp pulse sampling utilizing `np.linspace` behaviour changed. (!258)
-* Docs - Adds the new Quantify logo similar to quantify_core. (!266)
-* Docs - Enhance documentation of public API for reimported modules [imports aliases] (!254)
-* Docs - Fixes the funcparserlib error in rtd. (!251)
-* Docs - Updated Qblox backend docs to include the new features. (!247)
-
-
-0.5.0 Expanded feature sets hardware compilation backends (2021-10-25)
-----------------------------------------------------------------------
-
-Breaking changes
-~~~~~~~~~~~~~~~~
-* The `schedules.timedomain_schedules.allxy_sched` function no longer accepts the string "All" as an argument to the `element_select_idx` keyword.
-* The `QuantumDevice.cfg_nr_averages` parameter was renamed to `QuantumDevice.cfg_sched_repetitions`
-* The call signature of `gettables.ScheduleVectorAcqGettable` has been renamed to `gettables.ScheduleGettableSingleChannel`, and the call signature has been updated according to #36 to no longer accept several keyword arguments.
-* Qblox Backend - The NCO phase is now reset at the start of a program (!213).
-* Qblox Backend - Compilation now requires qblox_instruments version 0.5.0, 0.5.1 or 0.5.2 (!214, !221).
-
-Merged branches and closed issues
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-* Compilation - Added the ability to specify the BinMode at the quantum-circuit layer (#183, !180).
-* Compilation - qcompile no longer modifies schedules (#102, !178).
-* Control - Added a first version of the QuantumDevice object (#148, !180).
-* Control - A single-qubit ScheduleGettable has been added (#36, !180).
-* Docs - Added bibliography with sphinxcontrib-bibtex extension (!171).
-* Docs - Fixed missing files in API reference (!176).
-* InstrumentCoordinator - CompiledSchedule class added to specify interfaces of InstrumentCoordinator and compilation functions (#174, !177).
-* InstrumentCoordinator - CompiledSchedule.last_schedule method added to provide access to last executed schedule (#167, !177).
-* Qblox Backend - Added support for qblox_instruments version 0.4.0 (new acquisition path) (!143).
-* Qblox Backend - Added support for real time mixer corrections rather than pre-distorting the uploaded waveforms (!192).
-* Qblox Backend - Waveforms are now compared using the normalized data array rather than the parameterized description (!182).
-* Qblox Backend - Support for append bin mode (#184, !180).
-* Qblox Backend - Support for using real value pulses on arbitrary outputs added (!142).
-* Qblox Backend - Compilation now supports 6 sequencers for both the QCM as well as the QRM (!142).
-* Qblox Backend - Support for a cluster, along with its QCM, QRM, QCM-RF and QRM-RF modules (!164)
-* Qblox Backend - Registers are now dynamically allocated during compilation (!195)
-* Zhinst backend - No exception is raised when an LO that is in the config is not part of a schedule. (#203, !223)
-* Zhinst backend - Instrument coordinator components for ZI will only be configured when the settings used to configure it have changed (#196, !227)
-* Zhinst backend - Solved a bug that caused single-sideband demodulation to not be configured correctly when using the UHFQA (!227)
-* Zhinst backend - Warnings raised during compilation of seqc programs will no longer raise an exception but will use logging.warning (!227)
-* Zhinst backend - resolved a bug where the instrument coordinator cannot write waveforms to the UHFQA if it has never been used before (!227)
-* Zhinst backend - resolved a bug where multiple identical measurements in a schedule would result in multiple integration weights being uploaded to the UFHQA (#207, !234)
-* Zhinst backend - resolved a bug where the UHFQA would not be triggered properly when executing a schedule with multiple samples (batched mode) (#205, !234)
-* Qblox ICCs - Compensated integration time for Qblox QRM IC component (!199).
-* Qblox ICCs - Added error handling for error flags given by `get_sequencer_state` (!215)
-* QuantumDevice - Added docstrings to the TransmonElement parameters (!216, !218)
-* Qblox ICCs - QCoDeS parameters are now only set if they differ from the value in the cache (!230)
-* Visualization - Allow user defined axis for plotting circuit diagram (!206)
-* Visualization - Adds schedule plotting using matplotlib and a WindowOperation to help visualize pulse diagrams (!225, !232)
-* Other - Added method `sample_schedule` to sample a `Schedule` (!212)
-* Other - The `RampPulse` has an extra (optional) parameter `offset` (!211)
-* Other - Updated existing schedules to make use of the acquisition index (#180, !180).
-* Other - Added a function to extract acquisition metadata from a schedule (#179, !180).
-* Other - The soft square waveform can now be evaluated with only one datapoint without raising an exception (!235)
-* Other - Added a function that generates a square pulse that compensates DC components of a sequence of pulses (!173)
-
-0.4.0 InstrumentCoordinator and improvements to backends (2021-08-06)
----------------------------------------------------------------------
-
-Breaking changes
-~~~~~~~~~~~~~~~~
-* Change of namespace from quantify.scheduler.* to quantify_scheduler.*
-
-Merged branches and closed issues
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-* Changes the namespace from quantify.scheduler to quantify_scheduler (!124)
-* InstrumentCoordinator - Add is_running property and wait_done method. Closes #133 (!140)
-* InstrumentCoordinator - Add instrument coordinator reference parameter to transmon element (!152)
-* InstrumentCoordinator - Prefix serialized settings for ZI ControlStack components. (!149)
-* InstrumentCoordinator - Refactored ControlStack name to InstrumentCoordinator (!151)
-* InstrumentCoordinator - Make use of InstrumentRefParameters (!144)
-* InstrumentCoordinator - Add controlstack class (!70)
-* InstrumentCoordinator - Add Zurich Instruments InstrumentCoordinatorComponent. (!99)
-* InstrumentCoordinator - Add Qblox InstrumentCoordinatorComponent. (!112)
-* InstrumentCoordinator - Avoid garbage collection for instrument coordinator components (!162)
-* Qblox backend - Removed limit in Qblox backend that keeps the QCM sequencer count at 2 (!135)
-* Qblox backend - Restructured compilation using external local oscillators. (!116)
-* Qblox backend - Added Chirp and Staircase pulses; and efficient implementation for QD spin qubit experiments (!106)
-* Qblox backend - Only run `start_sequencer` on pulsar instruments which have been armed (!156)
-* Zhinst backend - Assert current with new sequence program to skip compilation (!131)
-* Zhinst backend - Deserialize zhinst settings from JSON to ZISettingsBuilder (!130)
-* Zhinst backend - Add waveform mixer skewness corrections (!103)
-* Zhinst backend - Add backend option to enable Calibration mode (#103, !123)
-* Zhinst backend - Replace weights string array with a numerical array in JSON format (!148)
-* Zhinst backend - Add grouping of instrument settings (!133)
-* Zhinst backend - Add qcompile tests for the zurich instruments backend (!118)
-* Zhinst backend - Add repetitions parameter (!138)
-* Zhinst backend - Fixes the bug where the seqc in the datadir is not copied to the webserver location. (!165)
-* Fix for circuit diagram plotting failure after pulse scheduling (#157, !163)
-* Fixed typo in the gate_info of the Y gate in the gate_library (!155)
-* Add artificial detuning in Ramsey Schedule and bug fixes (!120)
-* Use individual loggers per python file (!134)
-* Recolour draw circuit diagram mpl (!96)
-* Fix issues with timedomain schedules (!145)
-* Renamed input parameters of quantify_scheduler.schedules.* functions. (!136)
-* Added acquisitions to circuit diagram (!93)
-* Add string representations to acquisition protocols of the acquisitions library (!114)
-* Transmon element and config generation (!75)
-* Rename operation_hash to operation_repr (!122)
-* Add types.Schedule from_json conversion (!119)
-* Add missing return types (!121)
-* Add serialization to Operations (!110)
-
-
-
-0.3.0 Multiple backends support (2021-05-20)
-------------------------------------------------
-* Added support for both Qblox and Zurich Instrument backends.
-* Added convenience pylintrc configuration file.
-* Added examples for timedomain and spectroscopy schedules.
-
-
-Breaking changes
-~~~~~~~~~~~~~~~~
-* Major refactor of the Qblox backend. (For example, it's now `quantify_core.backends.qblox_backend` instead of the previous `quantify_core.backends.pulsar_backend`)
-* Qblox backend requires strictly v0.3.2 of the qblox-instruments package.
-
-
-Merged branches and closed issues
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-
-* Add mixer skewness corrections helper function. (!102)
-* Added Qblox backend support. (!81)
-* Compile backend with ZISettingsBuilder. (!87)
-* Add vscode IDE config files. (!100)
-* Add ZISettingsBuilder class. (!86)
-* Added representation to gates in gate library and defined equality operation. (!101)
-* Fix/operation duration. Fixes #107. (!89)
-* Feat/long pulses fix validators name. (!90)
-* Implemented long square pulses unrolling (for waveform-memory-limited devices). (!83)
-* Changed Qblox-Instruments version to 0.3.2. (!88)
-* Feature: Improve overall zhinst backend timing. (!77)
-* Plotly cleanup. (!69)
-* Pulsar backend version bump. (!82)
-* Added zhinst backend support. (!49)
-* Added example timedomain programs. (!71)
-* Added example spectroscopy programs. (!64)
-* Added pylintrc configuration file. (!55)
-* Added repetitions property to Schedule. (!56)
-* Added Acquisition Protocols. (!51)
-* Hotfix for filename sanitization pulsar backend. (!61)
-* Pulsar backend function sanitization. (!60)
-* Potential fix time-out pulsar. (!58)
-* Updated Pulsar backend version to v0.2.3.. (!57)
-* Fixed datadir related bugs. (!54)
-* Added Station implementation. (!52)
-* Pulsar backend v0.2.2 check. (!48)
-* Fix for issue with acq delay. (!45)
-* Fix for issue #52. (!44)
-* Add artificial detuning to Ramsey schedule (!120)
-* Added support for the Qblox Pulsar QCM-RF/QRM-RF devices (!158)
-
-
-
-0.2.0 Hybrid pulse- gate-level control model (2021-01-14)
----------------------------------------------------------
-
-* Major refactor of the scheduler resource code enabling hybrid pulse- gate-level control.
-* Moved quantify_scheduler.types.Resource class to a separate quantify_scheduler.resources module.
-* Adds a BasebandClockResource class within the newly created quantify_scheduler.resources module.
-* Moved QRM and QCM related classes to the quantify_scheduler.backends.pulsar_backend module.
-* In quantify_scheduler.compilation, rename of function '_determine_absolute_timing' to 'determine_absolute_timing'. Argument changed from clock_unit to time_unit.
-* In quantify_scheduler.compilation, rename of function '_add_pulse_information_transmon' to 'add_pulse_information_transmon'.
-* Added ramp waveform in quantify_scheduler.waveforms.
-* Added schemas for operation and transmon_cfg.
-* Added a basic hybrid visualisation for pulses using new addressing scheme.
-* Operations check whether an operation is a valid gate or pulse.
-* Refactor of visualization module. Moved quantify_scheduler.backends.visualization to quantify_scheduler.visualization module. Expect code breaking reorganization and changes to function names.
-* Pulsar backend version now checks for QCM and QRM drivers version 0.1.2.
-
-Merged branches and closed issues
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-
-* fix(pulse_scheme): Add tickformatstops for x-axis using SI-unit 'seconds'. Closes #39. (!39)
-* Resolve "y-axis label is broken in plotly visualization after resources-refactor". Closes #45. (!38)
-* Resources refactor (!28, !29, !30)
-* Hybrid visualisation for pulses and circuit gate operations. Closes #22 and #6. (!27)
-* Support Pulsar parameterisation from scheduler. Support feature for #29. (!2)
-* Operation properties to check if an operation is a valid gate or pulse. Closes #28 (!25)
-* Visualisation refactor. Closes #26. (!22)
-* Windows job (!20)
-* Changed Pulsar backend version check from 0.1.1 to 0.1.2. (!21)
-
-
-
-0.1.0 (2020-10-21)
-------------------
-* Refactored scheduler functionality from quantify-core into quantify-scheduler
-* Support for modifying Pulsar params via the sequencer #54 (!2)
-* Simplification of compilation through `qcompile` (!1)
-* Qubit resources can be parameters of gates #11 (!4)
-* Circuit diagram visualization of operations without no pulse info raises exception #5 (!5)
-* Pulsar backend verifies driver and firmware versions of hardware #14 (!6)
-* Sequencer renamed to scheduler #15 (!7)
-* Documentation update to reflect refactor #8 (!8)
-* Refactor circuit diagram to be more usable !10 (relates to #6)
-* Unify API docstrings to adhere to NumpyDocstring format !11
-* Changes to addressing of where a pulse is played !9 (#10)
-* Renamed doc -docs folder for consistency #18 (!12)
-* Moved test folder outside of project #19 (!14)
-* Add copyright notices and cleanup documenation #21 (!13)
-* Add installation tip for plotly dependency in combination with jupyter #24 (!15)
-
-.. note::
-
-    * # denotes a closed issue.
-    * ! denotes a merge request.
+Metadata-Version: 2.1
+Name: quantify-scheduler
+Version: 0.9.0
+Summary: Quantify-scheduler is a python package for writing quantum programs featuring a hybrid gate-pulse control model with explicit timing control.
+Home-page: https://gitlab.com/quantify-os/quantify-scheduler
+Author: The Quantify consortium consisting of Qblox and Orange Quantum Systems
+Author-email: maintainers@quantify-os.org
+License: BSD-3 license
+Keywords: quantify-scheduler
+Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+License-File: AUTHORS.md
+
+# quantify-scheduler
+
+[![Slack](https://img.shields.io/badge/slack-chat-green.svg)](https://join.slack.com/t/quantify-hq/shared_invite/zt-vao45946-f_NaRc4mvYQDQE_oYB8xSw)
+[![Pipelines](https://gitlab.com/quantify-os/quantify-scheduler/badges/main/pipeline.svg)](https://gitlab.com/quantify-os/quantify-scheduler/pipelines/)
+[![PyPi](https://img.shields.io/pypi/v/quantify-scheduler.svg)](https://pypi.org/pypi/quantify-scheduler)
+[![Code Quality](https://app.codacy.com/project/badge/Grade/0c9cf5b6eb5f47ffbd2bb484d555c7e3)](https://www.codacy.com/gl/quantify-os/quantify-scheduler/dashboard?utm_source=gitlab.com&amp;utm_medium=referral&amp;utm_content=quantify-os/quantify-scheduler&amp;utm_campaign=Badge_Grade)
+[![Coverage](https://app.codacy.com/project/badge/Coverage/0c9cf5b6eb5f47ffbd2bb484d555c7e3)](https://www.codacy.com/gl/quantify-os/quantify-scheduler/dashboard?utm_source=gitlab.com&amp;utm_medium=referral&amp;utm_content=quantify-os/quantify-scheduler&amp;utm_campaign=Badge_Coverage)
+[![Documentation Status](https://readthedocs.com/projects/quantify-quantify-scheduler/badge/?version=latest&token=ed6fdbf228e1369eacbeafdbad464f6de927e5dfb3a8e482ad0adcbea76fe74c)](https://quantify-quantify-scheduler.readthedocs-hosted.com)
+[![License](https://img.shields.io/badge/License-BSD%203--Clause-blue.svg)](https://gitlab.com/quantify-os/quantify-scheduler/-/raw/main/LICENSE)
+[![Code style](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![Unitary Fund](https://img.shields.io/badge/Supported%20By-UNITARY%20FUND-brightgreen.svg?style=flat)](http://unitary.fund)
+
+![Quantify logo](https://orangeqs.com/logos/QUANTIFY_LANDSCAPE.svg)
+
+Quantify is a python based data acquisition platform focused on Quantum Computing and solid-state physics experiments.
+It is built on top of [QCoDeS](https://qcodes.github.io/Qcodes/) and is a spiritual successor of [PycQED](https://github.com/DiCarloLab-Delft/PycQED_py3).
+Quantify currently consists of [quantify-core](https://pypi.org/project/quantify-core/) and [quantify-scheduler](https://pypi.org/project/quantify-scheduler/).
+
+Take a look at the [latest documentation for quantify-scheduler](https://quantify-quantify-scheduler.readthedocs-hosted.com/) or use the switch at the bottom of the left panel to read the documentation for older releases.
+
+Quantify-scheduler is a python module for writing quantum programs featuring a hybrid gate-pulse control model with explicit timing control.
+The control model allows quantum gate- and pulse-level descriptions to be combined in a clearly defined and hardware-agnostic way.
+Quantify-scheduler is designed to allow experimentalists to easily define complex experiments, and produces synchronized pulse schedules to be distributed to control hardware.
+
+⚠️**Caution!**
+This is a pre-release **alpha version**, major changes are expected. Use for testing & development purposes only.
+
+## About
+
+Quantify-scheduler is maintained by The Quantify consortium consisting of Qblox and Orange Quantum Systems.
+
+
+[<img src="https://cdn.sanity.io/images/ostxzp7d/production/f9ab429fc72aea1b31c4b2c7fab5e378b67d75c3-132x31.svg" alt="Qblox logo" width=200px/>](https://qblox.com)
+&nbsp;
+&nbsp;
+&nbsp;
+&nbsp;
+[<img src="https://orangeqs.com/OQS_logo_with_text.svg" alt="Orange Quantum Systems logo" width=200px/>](https://orangeqs.com)
+
+&nbsp;
+
+The software is free to use under the conditions specified in the [license](https://gitlab.com/quantify-os/quantify-scheduler/-/raw/main/LICENSE).
+
+
+# Credits
+
+## Contributors
+
+- [Adam Lawrence](mailto:adam@orangeqs.com)
+- [Adriaan Rol](mailto:adriaan@orangeqs.com)
+- [Callum Attryde](mailto:cattryde@qblox.com)
+- [Christian Dickel](mailto:christiandickel8@gmail.com)
+- [Damaz de Jong](mailto:ddejong@qblox.com)
+- [Damien Crielaard](mailto:dcrielaard@qblox.com)
+- [Diogo Valada](mailto:dvalada@qblox.com)
+- [Edgar Reehuis](mailto:ereehuis@qblox.com)
+- [Gabor Oszkar Denes](mailto:gdenes@qblox.com)
+- [Gijs Vermarien](mailto:gijs@orangeqs.com)
+- [Hiresh Jadoenathmissier](mailto:hiresh@orangeqs.com)
+- [Jordy Gloudemans](mailto:jgloudemans@qblox.com)
+- [Jules van Oven](mailto:jules@qblox.com)
+- [Kelvin Loh](mailto:kelvin@orangeqs.com)
+- [Luis Miguens Fernandez](mailto:lmiguens@qblox.com)
+- [Michiel Dubbelman](mailto:michiel@orangeqs.com)
+- [Pieter Eendebak](mailto:pieter.eendebak@tno.nl)
+- [Robert Sokolewicz](mailto:rsokolewicz@qblox.com)
+- [Thomas Reynders](mailto:thomas@orangeqs.com)
+- [Viacheslav Ostroukh](mailto:viacheslav@orangeqs.com)
+- [Victor Negirneac](mailto:vnegirneac@qblox.com)
+
+
+
+# Changelog
+
+## 0.9.0 (2022-10-06)
+
+### Breaking changes
+
+- Deprecated methods removed:
+  - `QuantumDevice`
+    - `components` -> `elements`
+    - `get_component` -> `get_element`
+    - `add_component` -> `add_element`
+    - `remove_component` -> `remove_element`
+  - `ScheduleBase`
+    - `plot_circuit_diagram_mpl` -> `plot_circuit_diagram`
+    - `plot_pulse_diagram_mpl` -> `plot_pulse_diagram`  
+- Compilation - Compilation is now a graph. (#305, !407)
+- Operations - Allow moving to `qcodes` >=0.34 (#300, !473)
+    - Disallow `"_"` in `DeviceElement` names to comply with qcodes version 0.34
+    - Enforces `"_"` as the separator between device elements in `Edge` names
+    - Note: We are still on `qcodes` 0.33 due to pin in `quantify-core` package requirements
+- Operations, Resources, and Schedulables - Deprecate the use of the `data` argument (!455)
+- Qblox ICCs - Hotfix for storing scope acquisition (broken by !432) (!470)
+- Qblox ICCs - Only activate markers and LOs of used outputs to prevent noise (!474)
+
+### Merged branches and closed issues
+
+- Docs - Support for `myst-nb` added (#301, !407)
+- Docs - Sources are converted from restructured text format to MyST markdown. (!452)
+- Docs - Add pin on `nbclient<0.6` for Read-the-Docs to build; Remove various old temp requirement pins (!477)
+- Docs - Added documentation and unit tests for the Rxy, X, X90, Y and Y90 unitaries (#349)
+- Gettables - Added a `ProfiledScheduleGettable` for profiling execution times of schedule steps. (!420, !469)
+  - Please note: Setup in need of refactoring so interface is subject to change (see #320)
+- Instrument Coordinator - Small fix for `search_settable_param` when scheduler is searching for qcodes parameters (!461)
+- JSON utilities - Remove `repr` based serialization/deserialization methods (!445, #248)
+- JSON utilities - Extend the capabilities of the ``__getstate__/__setstate__`` json serializer (!445, #248)
+- Qblox ICCs - Added input/output gain/attenuation configurable hardware parameter (!458)
+- Structure - Pydantic-based model is now used to validate latency corrections. (!467, #333)
+- Zhinst backend - Raise a more understandable exception when compiling an acquisition with larger than allowed duration (!407).
+
+## 0.8.0 Support for two qubit operations and basic CZ-gate implementation (2022-08-10)
+
+### Breaking changes
+
+- Operations - Pin `qcodes` package to \<0.34.0 due to breaking `Edge` naming (#300, !409)
+- Qblox backend - Sequencers are now dynamically allocated. The hardware config file schema was changed. (!328)
+    - For each instrument, the config now contains a `portclock_configs` entry, a list with a dictionary of settings per port-clock combination
+    - See <https://quantify-quantify-scheduler.readthedocs-hosted.com/en/0.8.0/tutorials/qblox/recent.html>
+- Qblox backend - Strictly requires v0.7.x of the `qblox-instruments` package (!449)
+- Zhinst backend - Strictly requires v21.8.20515 of the `zhinst` package (!387)
+
+### Merged branches and closed issues
+
+- Compilation - Added `acq_protocol` optional parameter to the `Measure` gate. (!386)
+- Compilation - Call `determine_absolute_timing` in `qcompile` when no `device_cfg` supplied. (!436)
+- Compilation - Decrease test usage of deprecated transmon_test_config.json / add_pulse_information_transmon (!450)
+- DRAG Pulse - Removed an extra G_amp factor from the Q component (derivative pulse). (#298, !406)
+- Docs - Fix API reference pages on read-the-docs (#303, !413)
+- Docs - Pin sphinx to 5.0.2 due to crash in napoleon (!437)
+- Docs - Unpin sphinx >=5.1.1 (!445)
+- Docs - Fix jsonschemas not rendered on read-the-docs (!448)
+- Docs - Clarify port and clock concepts (!431)
+- Docs - New scheduler tutorials: Schedules and Pulses; Compiling to Hardware; Operations and Qubits (!336, !439)
+- Gettables - Added `generate_diagnostic_report` method to save the internal state of `ScheduleGettable` to a zip-file. (!408)
+- Helpers - Moved `MockLocalOscillator` definition from tests to `helpers.mock_instruments.MockLocalOscillator` (!392, !336).
+- JSON utilities - Add JSON serialization/deserialization methods based on `__getstate__`/`__setstate__` (!444)
+- Operations - Added a `symmetric` key in the `gate_info` to flag symmetric operations. (!389)
+- Operations - Introduce basic CZ-gate via `CompositeSquareEdge` (utilizing `quantify_scheduler.operations.pulse_factories.composite_square_pulse`) (!411)
+    - Replaces the incomplete `SuddenNetZeroEdge` basic CZ-gate implementation
+- Operations - Rxy theta rotations now fall into the domain of \[-180 to 180) degrees. (!433)
+- QuantumDevice - Added implementation for `edges` in the quantum device config in order to support two qubit operations. (!389)
+    - The `Edge` has been added as an abstract base class for edges to be added to a device.
+- Qblox backend - Only add clocks to the schedule that are actually being used, avoids trying to assign frequencies for unused clocks (#278, !371)
+- Qblox backend - Fix for supplying negative NCO phase (!393)
+- Qblox backend - Fix compilation of ShiftClockPhase (!404, broken by merge of !328)
+- Qblox backend - Fix for outputting signals on even output paths of qblox hardware in real_output_x mode (!397)
+- Qblox backend - Make Qblox backend compatible with generic downconverter values in hardware_config (!418)
+- Qblox backend - Fix for 90 degree phase shift on even output paths as a result of the !397 hotfix. (!412)
+- Qblox backend - Fix cluster compatibility when converting old hwconfig to new specs (!419)
+- Qblox backend - Latency corrections must now be defined in top layer of hw config (!400)
+- Qblox backend - Fix combination of cluster and latency corrections when converting hw_configs to new specs  (!417)
+- Qblox backend - Fix handling of composite pulses (#299, !411)
+- Qblox backend - Implementation of distortion correction (#285, !388)
+- Qblox backend - Fix incompatibility of distortion_correction parameters as numpy arrays (!426)
+- Qblox backend - Remove all references to the inactive `line_gain_db` param (!435)
+- Qblox ICCs - Fix for setting `scope_acq_sequencer_select` for QRM and QRM-RF (!432, !441)
+- Qblox ICCs - Fix `ClusterComponent.prepare` mutating the schedule (!443)
+- Schedules - Revert rename of `trace_schedule` done in !432 and rename new schedule using gates to `trace_schedule_circuit_layer` (!442)
+- Schedules - Make `AcquisitionMetadata` a serializable class (!446)
+
+## 0.7.0 Support for qblox-instruments v0.6.0, new BasicTransmonElement, change for triggers in Zhinst backend (2022-04-11)
+
+### Breaking changes
+
+- Qblox ICCs - Updated Qblox components for using the new unified-style qblox driver (see <https://gitlab.com/quantify-os/quantify-scheduler/-/wikis/Qblox-ICCs:-Interface-changes-in-using-qblox-instruments-v0.6.0>) (!377).
+- Qblox backend - Strictly requires v0.6.0 of the qblox-instruments package (!377).
+- Zhinst backend - Hardware config for the devices. Replaced keyword "triggers" to "trigger", and the value type from `List[int]` to `int`. E.g. old style, `"triggers": [2]`, new style, `"trigger": 2` (#264, !372).
+
+### Merged branches and closed issues
+
+- QuantumDevice - The `DeviceElement` has been added as an abstract base class for elements to be added to a device (#148, !374).
+- QuantumDevice - The `BasicTransmonElement` has been added that generates a device config in a more structured manner (#246, !374).
+- QuantumDevice - Fixed a bug in the `BasicTransmonElement` where operations had clock-frequencies (`float`) specified instead of clocks (`str`) (!379).
+- QuantumDevice - The `TransmonElement` will be deprecated after version 0.8 (!374).
+
+## 0.6.0 Full support for multiplexed readout, transmon element update, fixes to backends (2022-03-10)
+
+### Breaking changes
+
+- Compilation - Deprecated `add_pulse_information_transmon` in favor of `compilation.backends.circuit_to_device.compile_circuit_to_device` (#64, #67, !339).
+- Compilation - attempting compilation with missing values in the `DeviceCompilationConfig` configuration will now raise validation errors. Be sure to set initial values when generating a config using the `QuantumDevice` object (!339)
+- Compilation - Device compile making use of `.compile_circuit_to_device` no longer modifies the input schedule (#249, !339).
+- Compilation - When specifying multiple timing constraints for a schedulable, the constraint specifying the latest time determines the absolute time of the shedulable (!309)
+- Gettables - `ScheduleGettableSingleChannel` renamed to `ScheduleGettable` as it now supports multiple acquisition channels (!299).
+- Hardware config - Removed the need for a `ic_` prefix from the hardware config (!312).
+- Instrument Coordinator - IC now adds a `GenericInstrumentCoordinatorComponent` to itself on instantiation by default (!350)
+- Instrument Coordinator - IC stop function has an `allow_failure` parameter which allows IC components attached to it to fail to stop with warning instead of raising errors. Allows for situations when some components cannot have a stop instruction sent before the prepare stage. (!359)
+- Operations - The internal behavior of how acquisition channels and acquisition indices are configured in the `Measure` operation has changed slightly. See #262 for details. (!339).
+- Operations - Added "operation_type" key to the schema. (!345)
+- Structure - `Schedule.timing_constraints` has been renamed to `Schedule.schedulables`. It now points to a dictionary of schedulables rather than a list of dicts. (!309)
+- Structure - Pydantic-based model is now used for the data structures. (!341)
+- Visualization - Deprecated `plot_circuit_diagram_mpl` and `plot_pulse_diagram_mpl` in `ScheduleBase` in favour of `plot_circuit_diagram` and `plot_pulse_diagram` (!313)
+- Qblox backend - Strictly requires v0.5.4 of the qblox-instruments package (!314)
+- Zhinst backend - Due to !312, the csv files used to upload the waveforms to the UHFQA no longer use the `ic_` prefix in their filenames. (!334)
+- Zhinst backend - Fixes bug when doing SSRO experiments. No more duplicated shots. Adds support for BinMode.APPEND during compilation. (#276, !358)
+- Zhinst backend - Removed `latency` and `line_trigger_delay` keys in the channels of the devices for the Zhinst hardware config. (!363)
+- Zhinst backend - Added `latency_corrections` main entry in the Zhinst hardware config for latency corrections on a port-clock combination basis. (!363)
+
+### Merged branches and closed issues
+
+- Compilation - Added a new compilation backend `compilation.backends.circuit_to_device.compile_circuit_to_device` for the quantum-circuit to quantum-device layer (#64, #67, !339).
+- Compilation - Fixed `add_pulse_information_transmon` when using "Trace" acquisition mode (!300)
+- Compilation - Fixed the deprecation warnings from pandas `DataFrame.append`. (!347)
+- Docs - Pinning qcodes package to \<0.32.0 due to Read the Docs API reference failure (!361)
+- Gettables - `ScheduleGettable` now first stops all instruments in IC during initialization (!324)
+- Schedules - Adds a multiplexing verification schedule. (!329)
+- Operations - Sudden Net Zero from Negirneac 2021 added to the `pulse_library` (!339)
+- Operations - Docstrings for the X90, X, Y90, Y, and Rxy gate unitary have been aligned with literature. (#261, !305)
+- Operations - Adds an optional "data" argument to staircase pulse. (!335)
+- Pulse library - Added `ShiftClockPhase` operation that can be used to shift the phase of a clock during execution of a `Schedule` (!346)
+- Pulse library - Added a numerically defined pulse. (!157)
+- QuantumDevice - Unknown values are initialized as `float('nan')` (#274, !356)
+- TransmonElement - Corrected the motzoi parameter range validator. (!351)
+- Visualization - Adds visualisation of acquisitions to plotly pulse diagrams (!304)
+- Visualization - Add `plot_pulse_diagram` and `plot_circuit_diagram` to schedule for easier method names, and enable plotly visualization directly from `ScheduleBase` (!313)
+- Utilities - Migrates the utilities from quantify-core. (!357)
+- Generic ICC - Adds support for nested parameters. (!330)
+- Qblox ICCs - Stop now disables sync on all sequencers to prevent hanging during next run, where it gets re-enabled if needed (!324)
+- Qblox ICCs - `_QRMAcquisitionManager._get_scope_data` now has correct return type (#232, !300)
+- Qblox ICCs - Fixed bug where QRM scope mode sequencer does not get set correctly (!342)
+- Qblox ICCs - Fixed reference source cluster issue when it is not being set correctly. (!323)
+- Qblox backend - NCO phase now gets reset every averaging loop (!337)
+- Qblox backend - Enables RF output switch at the start of a program. (!344)
+- Qblox backend - Added logic for changing the NCO phase during execution of a `Schedule` (!346)
+- Qblox backend - Added ability to correct for latency by delaying program execution on a per sequencer basis (!325)
+- Qblox backend - Compilation with local oscillators changed to work with generic instrument coordinator components (!306)
+- Qblox backend - Refactored operation handling and greatly increased test coverage (!301).
+- Qblox backend - Made max duration of wait instructions (!319).
+- Qblox backend - Fixed an issue with the downconverter frequency correction. (!318)
+- Qblox backend - Temporary fix for a floating point rounding error when calculating the length of pulses. (#284, !365)
+- Zhinst backend - Fixed the ZI resolver return typehint. (!307)
+- Zhinst backend - Fixed an issue when compiling seqc programs for multiple sequencers end up overwriting the first sequencer. (!340, #260)
+
+## 0.5.2 Fixes to backends, and other incremental fixes  (2021-12-08)
+
+### Breaking changes
+
+- Dependency on `jsonschema` has been replaced with `fastjsonschema`. (!284, !293)
+- Zhinst hardware config json schema has changed. See the example schema. (!283)
+- In `hardware_compile` function, the `hardware_map` is changed to `hardware_cfg` parameter. (!279)
+- Remove enum tools dependency (!270)
+
+### Merged branches and closed issues
+
+- Compilation - The `determine_absolute_scheduling` function now sorts the list of labels in the timing constraints, and then a binary search (via `np.searchsorted`) is applied. (!272, !274)
+- Compilation - Make `device_cfg` an optional argument of qcompile(!281)
+- Compilation - renamed the hardware_mapping argument of qcompile into hardware_cfg (#165, !279)
+- Compilation - Introduced the hardware_compile function to perform the hardware compilation returning a CompiledSchedule (#224, !279)
+- Docs - Updating user guide to mention correctly the QuantumDevice and ScheduleGettable(s) available. (!209)
+- Infrastructure - Adds rich package in the requirements since tutorials use it. (!276)
+- Operations - The `locate` function now uses the `functools.lru_cache` to cache the result (only for python >= 3.8). For python 3.7, behaviour remains the same.  (!273, !275)
+- Operations - Resolved a minor issue where identical Rxy rotations (for angles >360) would be treated as separate operations in a schedule (!263)
+- Visualization - Adds a function `plot_acquisition_operations` which together with the new `AcquisitionOperation` class will help highlight acquisition pulses in the pulse diagrams. (!271, !277)
+- Zhinst backend - Large parts of the Zhinst backend have been rewritten. This should resolve a range of issues. (!263)
+    - Calculation of the timelines for different operations now makes using of a timing table, improving code readability and debugability.
+    - Timing issues related to triggering should be resolved (#218)
+    - The backend can now always use the same hardware configuration file (#214)
+    - Acquisition is now done using the StartQA instruction (#213)
+    - error handling in the Zhinst backend has been improved catching several exceptions at compile time of the schedule instead of manifesting in unexpected results during runtime.
+    - Local oscillators through the ZI backend uses the GenericInstrumentCoordinatorComponent. Configures other parameters other than frequency. (!283, #204)
+- Qblox backend - only check major and minor version when checking compatibility with the qblox_instruments package (!290)
+    - Added support for the Qblox Downconverter (!297)
+    - Added workaround for staircase_amplitude. (!292)
+    - Fix looped acquisition integration time, fix acquire index offset by one (!291)
+    - Qblox instruments version == 0.5.3 (!289)
+    - Fix sequencer_sync_en not being reset in the qblox instrument coordinator component. (!285)
+    - Fix rounding of time to samples in qblox backend (!282)
+    - Fix pulse stitching at zero amplitude. (!280)
+    - Allow instruction generated staircase with modulation (!278)
+- Utilities - Improve JSON validation speed (!284)
+- Utilities - Improve operation deserialization speed (!273)
+- Bugfix - For calculating the pulse area, the mathematical area is used instead of area of sampled pulse. (!242, !286)
+- Bugfix - Fix for plot window operations (!294)
+
+## 0.5.1 Incremental fixes, refactoring, and addition of convenience methods and classes (2021-11-11)
+
+### Breaking changes
+
+- InstrumentCoordinator - `last_schedule` is now a property (!252).
+- Structure - We have refactored the Operation and Schedule classes out of the types module and moved the different operation libraries (acquisition_library, gate_library, and pulse_library) (#217, !256).
+    - `quantify_scheduler.types.Operation` -> `quantify_scheduler.operations.operation.Operation`, the import `quantify_scheduler.Operation` still works.
+    - `quantify_scheduler.types.Schedule` -> `quantify_scheduler.schedules.schedule.Schedule`, the import `quantify_scheduler.Schedule` still works.
+    - `quantify_scheduler.types.CompiledSchedule` -> `quantify_scheduler.schedules.schedule.CompiledSchedule`
+    - `quantify_scheduler.types.ScheduleBase` -> `quantify_scheduler.schedules.schedule.ScheduleBase`
+    - `quantify_scheduler.types.AcquisitionMetadata` -> `quantify_scheduler.schedules.schedule.AcquisitionMetadata`
+    - `quantify_scheduler.acquisition_library` -> `quantify_scheduler.operations.acquisition_library`
+    - `quantify_scheduler.gate_library` -> `quantify_scheduler.operations.gate_library`
+    - `quantify_scheduler.pulse_library` -> `quantify_scheduler.operations.pulse_library`
+
+### Merged branches and closed issues
+
+- Control - Add option to set output port in heterodyne_spec_sched (!262)
+- Control - Expand SingleChannelScheduleGettable to support trace acquisitions (!248)
+- Control - Update create_dc_compensation_pulse behaviour and docstring. (!244)
+- Control - Refactor ScheduleGettableSingleChannel (!240, !249)
+- Control - Reduce the default init_duration of spectroscopy schedules (!237)
+- Generic ICC - Added a GenericInstrumentCoordinatorComponent. (!267)
+- ICCs - InstrumentCoordinatorComponentBase now has a `force_set_parameter` as a ManualParameter to enable the user to switch the lazy_set behaviour when setting parameters of the instruments connected to the InstrumentCoordinatorComponent. (!267)
+- Qblox ICCs - Adds a lazy_set behaviour by default when setting parameters with the same value to an instrument connected to the Qblox ICC. (!230)
+- Visualization - made matplotlib schedule visualization methods accessible as methods `plot_circuit_diagram_mpl` and `plot_pulse_diagram_mpl` of the `Schedule` class (!253)
+- Visualization - resolved a bug where a schedule was modified when drawing a circuit diagram (#197, !250)
+- Visualization - Add support for window operation to transmon backend (!245)
+- Infrastructure - Fix and enhance pre-commit + add to CI (!257, !265)
+- Infrastructure - Added prospector config file for CI. (!261)
+- Bugfix - Removed redundant `determine_absolute_timing` step in `qcompile`. (!259)
+- Bugfix - Ramp pulse sampling utilizing `np.linspace` behaviour changed. (!258)
+- Docs - Adds the new Quantify logo similar to quantify_core. (!266)
+- Docs - Enhance documentation of public API for reimported modules \[imports aliases\] (!254)
+- Docs - Fixes the funcparserlib error in rtd. (!251)
+- Docs - Updated Qblox backend docs to include the new features. (!247)
+
+## 0.5.0 Expanded feature sets hardware compilation backends (2021-10-25)
+
+### Breaking changes
+
+- The `schedules.timedomain_schedules.allxy_sched` function no longer accepts the string "All" as an argument to the `element_select_idx` keyword.
+- The `QuantumDevice.cfg_nr_averages` parameter was renamed to `QuantumDevice.cfg_sched_repetitions`
+- The call signature of `gettables.ScheduleVectorAcqGettable` has been renamed to `gettables.ScheduleGettableSingleChannel`, and the call signature has been updated according to #36 to no longer accept several keyword arguments.
+- Qblox Backend - The NCO phase is now reset at the start of a program (!213).
+- Qblox Backend - Compilation now requires qblox_instruments version 0.5.0, 0.5.1 or 0.5.2 (!214, !221).
+
+### Merged branches and closed issues
+
+- Compilation - Added the ability to specify the BinMode at the quantum-circuit layer (#183, !180).
+- Compilation - qcompile no longer modifies schedules (#102, !178).
+- Control - Added a first version of the QuantumDevice object (#148, !180).
+- Control - A single-qubit ScheduleGettable has been added (#36, !180).
+- Docs - Added bibliography with sphinxcontrib-bibtex extension (!171).
+- Docs - Fixed missing files in API reference (!176).
+- InstrumentCoordinator - CompiledSchedule class added to specify interfaces of InstrumentCoordinator and compilation functions (#174, !177).
+- InstrumentCoordinator - CompiledSchedule.last_schedule method added to provide access to last executed schedule (#167, !177).
+- Qblox Backend - Added support for qblox_instruments version 0.4.0 (new acquisition path) (!143).
+- Qblox Backend - Added support for real time mixer corrections rather than pre-distorting the uploaded waveforms (!192).
+- Qblox Backend - Waveforms are now compared using the normalized data array rather than the parameterized description (!182).
+- Qblox Backend - Support for append bin mode (#184, !180).
+- Qblox Backend - Support for using real value pulses on arbitrary outputs added (!142).
+- Qblox Backend - Compilation now supports 6 sequencers for both the QCM as well as the QRM (!142).
+- Qblox Backend - Support for a cluster, along with its QCM, QRM, QCM-RF and QRM-RF modules (!164)
+- Qblox Backend - Registers are now dynamically allocated during compilation (!195)
+- Zhinst backend - No exception is raised when an LO that is in the config is not part of a schedule. (#203, !223)
+- Zhinst backend - Instrument coordinator components for ZI will only be configured when the settings used to configure it have changed (#196, !227)
+- Zhinst backend - Solved a bug that caused single-sideband demodulation to not be configured correctly when using the UHFQA (!227)
+- Zhinst backend - Warnings raised during compilation of seqc programs will no longer raise an exception but will use logging.warning (!227)
+- Zhinst backend - resolved a bug where the instrument coordinator cannot write waveforms to the UHFQA if it has never been used before (!227)
+- Zhinst backend - resolved a bug where multiple identical measurements in a schedule would result in multiple integration weights being uploaded to the UFHQA (#207, !234)
+- Zhinst backend - resolved a bug where the UHFQA would not be triggered properly when executing a schedule with multiple samples (batched mode) (#205, !234)
+- Qblox ICCs - Compensated integration time for Qblox QRM IC component (!199).
+- Qblox ICCs - Added error handling for error flags given by `get_sequencer_state` (!215)
+- QuantumDevice - Added docstrings to the TransmonElement parameters (!216, !218)
+- Qblox ICCs - QCoDeS parameters are now only set if they differ from the value in the cache (!230)
+- Visualization - Allow user defined axis for plotting circuit diagram (!206)
+- Visualization - Adds schedule plotting using matplotlib and a WindowOperation to help visualize pulse diagrams (!225, !232)
+- Other - Added method `sample_schedule` to sample a `Schedule` (!212)
+- Other - The `RampPulse` has an extra (optional) parameter `offset` (!211)
+- Other - Updated existing schedules to make use of the acquisition index (#180, !180).
+- Other - Added a function to extract acquisition metadata from a schedule (#179, !180).
+- Other - The soft square waveform can now be evaluated with only one datapoint without raising an exception (!235)
+- Other - Added a function that generates a square pulse that compensates DC components of a sequence of pulses (!173)
+
+## 0.4.0 InstrumentCoordinator and improvements to backends (2021-08-06)
+
+### Breaking changes
+
+- Change of namespace from quantify.scheduler.\* to quantify_scheduler.\*
+
+### Merged branches and closed issues
+
+- Changes the namespace from quantify.scheduler to quantify_scheduler (!124)
+- InstrumentCoordinator - Add is_running property and wait_done method. Closes #133 (!140)
+- InstrumentCoordinator - Add instrument coordinator reference parameter to transmon element (!152)
+- InstrumentCoordinator - Prefix serialized settings for ZI ControlStack components. (!149)
+- InstrumentCoordinator - Refactored ControlStack name to InstrumentCoordinator (!151)
+- InstrumentCoordinator - Make use of InstrumentRefParameters (!144)
+- InstrumentCoordinator - Add controlstack class (!70)
+- InstrumentCoordinator - Add Zurich Instruments InstrumentCoordinatorComponent. (!99)
+- InstrumentCoordinator - Add Qblox InstrumentCoordinatorComponent. (!112)
+- InstrumentCoordinator - Avoid garbage collection for instrument coordinator components (!162)
+- Qblox backend - Removed limit in Qblox backend that keeps the QCM sequencer count at 2 (!135)
+- Qblox backend - Restructured compilation using external local oscillators. (!116)
+- Qblox backend - Added Chirp and Staircase pulses; and efficient implementation for QD spin qubit experiments (!106)
+- Qblox backend - Only run `start_sequencer` on pulsar instruments which have been armed (!156)
+- Zhinst backend - Assert current with new sequence program to skip compilation (!131)
+- Zhinst backend - Deserialize zhinst settings from JSON to ZISettingsBuilder (!130)
+- Zhinst backend - Add waveform mixer skewness corrections (!103)
+- Zhinst backend - Add backend option to enable Calibration mode (#103, !123)
+- Zhinst backend - Replace weights string array with a numerical array in JSON format (!148)
+- Zhinst backend - Add grouping of instrument settings (!133)
+- Zhinst backend - Add qcompile tests for the zurich instruments backend (!118)
+- Zhinst backend - Add repetitions parameter (!138)
+- Zhinst backend - Fixes the bug where the seqc in the datadir is not copied to the webserver location. (!165)
+- Fix for circuit diagram plotting failure after pulse scheduling (#157, !163)
+- Fixed typo in the gate_info of the Y gate in the gate_library (!155)
+- Add artificial detuning in Ramsey Schedule and bug fixes (!120)
+- Use individual loggers per python file (!134)
+- Recolour draw circuit diagram mpl (!96)
+- Fix issues with timedomain schedules (!145)
+- Renamed input parameters of quantify_scheduler.schedules.\* functions. (!136)
+- Added acquisitions to circuit diagram (!93)
+- Add string representations to acquisition protocols of the acquisitions library (!114)
+- Transmon element and config generation (!75)
+- Rename operation_hash to operation_repr (!122)
+- Add types.Schedule from_json conversion (!119)
+- Add missing return types (!121)
+- Add serialization to Operations (!110)
+
+## 0.3.0 Multiple backends support (2021-05-20)
+
+- Added support for both Qblox and Zurich Instrument backends.
+- Added convenience pylintrc configuration file.
+- Added examples for timedomain and spectroscopy schedules.
+
+### Breaking changes
+
+- Major refactor of the Qblox backend. (For example, it's now `quantify_core.backends.qblox_backend` instead of the previous `quantify_core.backends.pulsar_backend`)
+- Qblox backend requires strictly v0.3.2 of the qblox-instruments package.
+
+### Merged branches and closed issues
+
+- Add mixer skewness corrections helper function. (!102)
+- Added Qblox backend support. (!81)
+- Compile backend with ZISettingsBuilder. (!87)
+- Add vscode IDE config files. (!100)
+- Add ZISettingsBuilder class. (!86)
+- Added representation to gates in gate library and defined equality operation. (!101)
+- Fix/operation duration. Fixes #107. (!89)
+- Feat/long pulses fix validators name. (!90)
+- Implemented long square pulses unrolling (for waveform-memory-limited devices). (!83)
+- Changed Qblox-Instruments version to 0.3.2. (!88)
+- Feature: Improve overall zhinst backend timing. (!77)
+- Plotly cleanup. (!69)
+- Pulsar backend version bump. (!82)
+- Added zhinst backend support. (!49)
+- Added example timedomain programs. (!71)
+- Added example spectroscopy programs. (!64)
+- Added pylintrc configuration file. (!55)
+- Added repetitions property to Schedule. (!56)
+- Added Acquisition Protocols. (!51)
+- Hotfix for filename sanitization pulsar backend. (!61)
+- Pulsar backend function sanitization. (!60)
+- Potential fix time-out pulsar. (!58)
+- Updated Pulsar backend version to v0.2.3.. (!57)
+- Fixed datadir related bugs. (!54)
+- Added Station implementation. (!52)
+- Pulsar backend v0.2.2 check. (!48)
+- Fix for issue with acq delay. (!45)
+- Fix for issue #52. (!44)
+- Add artificial detuning to Ramsey schedule (!120)
+- Added support for the Qblox Pulsar QCM-RF/QRM-RF devices (!158)
+
+## 0.2.0 Hybrid pulse- gate-level control model (2021-01-14)
+
+- Major refactor of the scheduler resource code enabling hybrid pulse- gate-level control.
+- Moved quantify_scheduler.types.Resource class to a separate quantify_scheduler.resources module.
+- Adds a BasebandClockResource class within the newly created quantify_scheduler.resources module.
+- Moved QRM and QCM related classes to the quantify_scheduler.backends.pulsar_backend module.
+- In quantify_scheduler.compilation, rename of function '\_determine_absolute_timing' to 'determine_absolute_timing'. Argument changed from clock_unit to time_unit.
+- In quantify_scheduler.compilation, rename of function '\_add_pulse_information_transmon' to 'add_pulse_information_transmon'.
+- Added ramp waveform in quantify_scheduler.waveforms.
+- Added schemas for operation and transmon_cfg.
+- Added a basic hybrid visualisation for pulses using new addressing scheme.
+- Operations check whether an operation is a valid gate or pulse.
+- Refactor of visualization module. Moved quantify_scheduler.backends.visualization to quantify_scheduler.visualization module. Expect code breaking reorganization and changes to function names.
+- Pulsar backend version now checks for QCM and QRM drivers version 0.1.2.
+
+### Merged branches and closed issues
+
+- fix(pulse_scheme): Add tickformatstops for x-axis using SI-unit 'seconds'. Closes #39. (!39)
+- Resolve "y-axis label is broken in plotly visualization after resources-refactor". Closes #45. (!38)
+- Resources refactor (!28, !29, !30)
+- Hybrid visualisation for pulses and circuit gate operations. Closes #22 and #6. (!27)
+- Support Pulsar parameterisation from scheduler. Support feature for #29. (!2)
+- Operation properties to check if an operation is a valid gate or pulse. Closes #28 (!25)
+- Visualisation refactor. Closes #26. (!22)
+- Windows job (!20)
+- Changed Pulsar backend version check from 0.1.1 to 0.1.2. (!21)
+
+## 0.1.0 (2020-10-21)
+
+- Refactored scheduler functionality from quantify-core into quantify-scheduler
+- Support for modifying Pulsar params via the sequencer #54 (!2)
+- Simplification of compilation through `qcompile` (!1)
+- Qubit resources can be parameters of gates #11 (!4)
+- Circuit diagram visualization of operations without no pulse info raises exception #5 (!5)
+- Pulsar backend verifies driver and firmware versions of hardware #14 (!6)
+- Sequencer renamed to scheduler #15 (!7)
+- Documentation update to reflect refactor #8 (!8)
+- Refactor circuit diagram to be more usable !10 (relates to #6)
+- Unify API docstrings to adhere to NumpyDocstring format !11
+- Changes to addressing of where a pulse is played !9 (#10)
+- Renamed doc -docs folder for consistency #18 (!12)
+- Moved test folder outside of project #19 (!14)
+- Add copyright notices and cleanup documenation #21 (!13)
+- Add installation tip for plotly dependency in combination with jupyter #24 (!15)
+
+```{note}
+- \# denotes a closed issue.
+- ! denotes a merge request.
+```
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `quantify-scheduler-0.8.0/setup.py` & `quantify-scheduler-0.9.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 #!/usr/bin/env python
 
 """The setup script."""
 
 from setuptools import find_packages, setup
 
-with open("README.rst") as readme_file:
+with open("README.md", encoding="utf-8") as readme_file:
     readme = readme_file.read()
 
-with open("AUTHORS.rst") as authors_file:
+with open("AUTHORS.md") as authors_file:
     authors = authors_file.read()
 
-with open("CHANGELOG.rst") as history_file:
+with open("CHANGELOG.md") as history_file:
     history = history_file.read()
 
 with open("requirements.txt") as installation_requirements_file:
     requirements = installation_requirements_file.read().splitlines()
 
 with open("requirements_setup.txt") as setup_requirements_file:
     setup_requirements = setup_requirements_file.read().splitlines()
 
 with open("requirements_dev.txt") as test_requirements_file:
     test_requirements = test_requirements_file.read().splitlines()
 
-version = "0.8.0"
+version = "0.9.0"
 
 setup(
     author="The Quantify consortium consisting of Qblox and Orange Quantum Systems",
     author_email="maintainers@quantify-os.org",
     python_requires=">=3.8",
     classifiers=[
         "Development Status :: 2 - Pre-Alpha",
@@ -39,14 +39,15 @@
         "Programming Language :: Python :: 3.10",
     ],
     description="Quantify-scheduler is a python package for writing quantum programs "
     "featuring a hybrid gate-pulse control model with explicit timing control.",
     install_requires=requirements,
     license="BSD-3 license",
     long_description=readme + "\n\n" + authors + "\n\n" + history,
+    long_description_content_type="text/markdown",
     include_package_data=True,
     keywords="quantify-scheduler",
     name="quantify-scheduler",
     packages=find_packages(include=["quantify_scheduler", "quantify_scheduler.*"]),
     package_data={"": ["*.json"]},  # ensures JSON schema are included
     setup_requires=setup_requirements,
     test_suite="tests",
```

### Comparing `quantify-scheduler-0.8.0/tests/baseline_images/test_hybrid_circuit_acquisitions_matplotlib.png` & `quantify-scheduler-0.9.0/tests/baseline_images/test_hybrid_circuit_acquisitions_matplotlib.png`

 * *Files identical despite different names*

### Comparing `quantify-scheduler-0.8.0/tests/baseline_images/test_hybrid_circuit_diagram_baseband_matplotlib.png` & `quantify-scheduler-0.9.0/tests/baseline_images/test_hybrid_circuit_diagram_baseband_matplotlib.png`

 * *Files identical despite different names*

### Comparing `quantify-scheduler-0.8.0/tests/baseline_images/test_hybrid_circuit_diagram_matplotlib.png` & `quantify-scheduler-0.9.0/tests/baseline_images/test_hybrid_circuit_diagram_matplotlib.png`

 * *Files identical despite different names*

### Comparing `quantify-scheduler-0.8.0/tests/baseline_images/test_hybrid_circuit_diagram_modulated_matplotlib.png` & `quantify-scheduler-0.9.0/tests/baseline_images/test_hybrid_circuit_diagram_modulated_matplotlib.png`

 * *Files identical despite different names*

### Comparing `quantify-scheduler-0.8.0/tests/baseline_images/test_hybrid_circuit_diagram_unknown_port_matplotlib.png` & `quantify-scheduler-0.9.0/tests/baseline_images/test_hybrid_circuit_diagram_unknown_port_matplotlib.png`

 * *Files identical despite different names*

### Comparing `quantify-scheduler-0.8.0/tests/baseline_images/test_plot_pulses_n_q.png` & `quantify-scheduler-0.9.0/tests/baseline_images/test_plot_pulses_n_q.png`

 * *Files identical despite different names*

### Comparing `quantify-scheduler-0.8.0/tests/baseline_images/test_plot_pulses_single_q.png` & `quantify-scheduler-0.9.0/tests/baseline_images/test_plot_pulses_single_q.png`

 * *Files identical despite different names*

### Comparing `quantify-scheduler-0.8.0/tests/baseline_qblox_assembly/AllXY_qrm0_seq0_instr.json` & `quantify-scheduler-0.9.0/tests/baseline_qblox_assembly/AllXY_qrm0_seq0_instr.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 0% similar despite different names*

```diff
@@ -1286,8 +1286,8 @@
 00005050: 2020 2277 6569 6768 7473 223a 207b 7d2c    "weights": {},
 00005060: 0a20 2020 2022 6163 7175 6973 6974 696f  .    "acquisitio
 00005070: 6e73 223a 207b 0a20 2020 2020 2020 2022  ns": {.        "
 00005080: 3022 3a20 7b0a 2020 2020 2020 2020 2020  0": {.          
 00005090: 2020 226e 756d 5f62 696e 7322 3a20 3231    "num_bins": 21
 000050a0: 2c0a 2020 2020 2020 2020 2020 2020 2269  ,.            "i
 000050b0: 6e64 6578 223a 2030 0a20 2020 2020 2020  ndex": 0.       
-000050c0: 207d 0a20 2020 207d 0a7d                  }.    }.}
+000050c0: 207d 0a20 2020 207d 0a7d 0a               }.    }.}.
```

### Comparing `quantify-scheduler-0.8.0/tests/baseline_qblox_assembly/Readout calibration q0, [0, 1]_qrm0_seq0_instr.json` & `quantify-scheduler-0.9.0/tests/baseline_qblox_assembly/Readout calibration q0, [0, 1]_qrm0_seq0_instr.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files identical despite different names*

```diff
@@ -616,7 +616,8 @@
 00002670: 3a20 7b7d 2c0a 2020 2020 2261 6371 7569  : {},.    "acqui
 00002680: 7369 7469 6f6e 7322 3a20 7b0a 2020 2020  sitions": {.    
 00002690: 2020 2020 2230 223a 207b 0a20 2020 2020      "0": {.     
 000026a0: 2020 2020 2020 2022 6e75 6d5f 6269 6e73         "num_bins
 000026b0: 223a 2035 3132 2c0a 2020 2020 2020 2020  ": 512,.        
 000026c0: 2020 2020 2269 6e64 6578 223a 2030 0a20      "index": 0. 
 000026d0: 2020 2020 2020 207d 0a20 2020 207d 0a7d         }.    }.}
+000026e0: 0a                                       .
```

### Comparing `quantify-scheduler-0.8.0/tests/baseline_qblox_assembly/sched-looped-acq_qrm0_seq0_instr.json` & `quantify-scheduler-0.9.0/tests/baseline_qblox_assembly/sched-looped-acq_qrm0_seq0_instr.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 0% similar despite different names*

```diff
@@ -107,8 +107,8 @@
 000006a0: 2020 2277 6569 6768 7473 223a 207b 7d2c    "weights": {},
 000006b0: 0a20 2020 2022 6163 7175 6973 6974 696f  .    "acquisitio
 000006c0: 6e73 223a 207b 0a20 2020 2020 2020 2022  ns": {.        "
 000006d0: 3022 3a20 7b0a 2020 2020 2020 2020 2020  0": {.          
 000006e0: 2020 226e 756d 5f62 696e 7322 3a20 312c    "num_bins": 1,
 000006f0: 0a20 2020 2020 2020 2020 2020 2022 696e  .            "in
 00000700: 6465 7822 3a20 300a 2020 2020 2020 2020  dex": 0.        
-00000710: 7d0a 2020 2020 7d0a 7d                   }.    }.}
+00000710: 7d0a 2020 2020 7d0a 7d0a                 }.    }.}.
```

### Comparing `quantify-scheduler-0.8.0/tests/fixtures/schedule.py` & `quantify-scheduler-0.9.0/tests/fixtures/schedule.py`

 * *Files identical despite different names*

### Comparing `quantify-scheduler-0.8.0/tests/scheduler/backends/qblox/operation_handling/test_acquisitions.py` & `quantify-scheduler-0.9.0/tests/scheduler/backends/qblox/operation_handling/test_acquisitions.py`

 * *Files 3% similar despite different names*

```diff
@@ -340,15 +340,15 @@
                 "# Store acq in acq_channel:2, bin_idx:R0",
             ],
             ["", "", "", ""],
         ]
 
 
 def test_trace_acquisition_measurement_control(
-    mock_setup, mocker, make_cluster_component
+    mock_setup_basic_transmon, mocker, make_cluster_component
 ):
     hardware_cfg = {
         "backend": "quantify_scheduler.backends.qblox_backend.hardware_compile",
         "cluster0": {
             "ref": "internal",
             "instrument_type": "Cluster",
             "cluster0_module4": {
@@ -359,21 +359,21 @@
                     ],
                 },
             },
         },
     }
 
     ic_cluster0 = make_cluster_component("cluster0")
-    instr_coordinator = mock_setup["instrument_coordinator"]
+    instr_coordinator = mock_setup_basic_transmon["instrument_coordinator"]
     instr_coordinator.add_component(ic_cluster0)
 
-    quantum_device = mock_setup["quantum_device"]
+    quantum_device = mock_setup_basic_transmon["quantum_device"]
     quantum_device.hardware_config(hardware_cfg)
 
-    q2 = mock_setup["q2"]
+    q2 = mock_setup_basic_transmon["q2"]
     q2.measure.acq_delay(600e-9)
     q2.clock_freqs.readout(7404000000.0)
 
     sample_param = ManualParameter("sample", label="Sample time", unit="s")
     sample_param.batched = True
 
     sample_size = 16384  # Trace acquisition will always return 16384 samples
@@ -412,15 +412,19 @@
 
 
 @pytest.mark.parametrize(
     "module_under_test",
     [ClusterType.CLUSTER_QRM_RF, ClusterType.CLUSTER_QRM, PulsarType.PULSAR_QRM],
 )
 def test_trace_acquisition_instrument_coordinator(  # pylint: disable=too-many-locals
-    mocker, mock_setup, make_cluster_component, make_qrm_component, module_under_test
+    mocker,
+    mock_setup_basic_transmon,
+    make_cluster_component,
+    make_qrm_component,
+    module_under_test,
 ):
     hardware_cfgs = {}
     hardware_cfgs[ClusterType.CLUSTER_QRM_RF] = {
         "backend": "quantify_scheduler.backends.qblox_backend.hardware_compile",
         "cluster0": {
             "ref": "internal",
             "instrument_type": "Cluster",
@@ -455,15 +459,15 @@
             "complex_output_0": {
                 "portclock_configs": [{"port": "q2:res", "clock": "q2.ro"}],
             },
         },
     }
     hardware_cfg = hardware_cfgs[module_under_test]
 
-    instr_coordinator = mock_setup["instrument_coordinator"]
+    instr_coordinator = mock_setup_basic_transmon["instrument_coordinator"]
 
     if isinstance(module_under_test, ClusterType):
         name = "cluster0"
 
         try:
             ic_component = make_cluster_component(name)
         except KeyError:
@@ -479,18 +483,18 @@
         instr_coordinator.add_component(ic_component)
 
     try:
         instr_coordinator.add_component(ic_component)
     except ValueError:
         ic_component.instrument.reset()
 
-    quantum_device = mock_setup["quantum_device"]
+    quantum_device = mock_setup_basic_transmon["quantum_device"]
     quantum_device.hardware_config(hardware_cfg)
 
-    q2 = mock_setup["q2"]
+    q2 = mock_setup_basic_transmon["q2"]
     q2.measure.acq_delay(600e-9)
     q2.clock_freqs.readout(
         7.404e9 if module_under_test is ClusterType.CLUSTER_QRM_RF else 3e8
     )
 
     schedule = trace_schedule_circuit_layer(qubit_name="q2")
```

### Comparing `quantify-scheduler-0.8.0/tests/scheduler/backends/qblox/operation_handling/test_factory.py` & `quantify-scheduler-0.9.0/tests/scheduler/backends/qblox/operation_handling/test_factory.py`

 * *Files identical despite different names*

### Comparing `quantify-scheduler-0.8.0/tests/scheduler/backends/qblox/operation_handling/test_pulses.py` & `quantify-scheduler-0.9.0/tests/scheduler/backends/qblox/operation_handling/test_pulses.py`

 * *Files identical despite different names*

### Comparing `quantify-scheduler-0.8.0/tests/scheduler/backends/qblox/operation_handling/test_virtual.py` & `quantify-scheduler-0.9.0/tests/scheduler/backends/qblox/operation_handling/test_virtual.py`

 * *Files identical despite different names*

### Comparing `quantify-scheduler-0.8.0/tests/scheduler/backends/qblox/test_driver_version_check.py` & `quantify-scheduler-0.9.0/tests/scheduler/backends/qblox/test_driver_version_check.py`

 * *Files identical despite different names*

### Comparing `quantify-scheduler-0.8.0/tests/scheduler/backends/qblox/test_helpers_qblox.py` & `quantify-scheduler-0.9.0/tests/scheduler/backends/qblox/test_helpers_qblox.py`

 * *Files identical despite different names*

### Comparing `quantify-scheduler-0.8.0/tests/scheduler/backends/qblox/test_register_manager.py` & `quantify-scheduler-0.9.0/tests/scheduler/backends/qblox/test_register_manager.py`

 * *Files identical despite different names*

### Comparing `quantify-scheduler-0.8.0/tests/scheduler/backends/test_circuit_to_device.py` & `quantify-scheduler-0.9.0/tests/scheduler/backends/test_circuit_to_device.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,15 +56,15 @@
     sched.add(Rxy(theta=90, phi=0, qubit=q0))
     sched.add(Measure(q0, q1), label="M_q0_q1")
 
     # test that all these operations compile correctly.
     _ = compile_circuit_to_device(sched, device_cfg=example_transmon_cfg)
 
 
-def test_compile_basic_transmon_example_program(mock_setup):
+def test_compile_basic_transmon_example_program(mock_setup_basic_transmon):
     """
     Test if compilation using the BasicTransmonElement reproduces old behaviour.
     """
 
     sched = Schedule("Test schedule")
 
     # define the resources
@@ -78,21 +78,21 @@
     sched.add(Y(qubit=q2))
     sched.add(Y90(qubit=q2))
     sched.add(operation=CZ(qC=q2, qT=q3))
     sched.add(Rxy(theta=90, phi=0, qubit=q2))
     sched.add(Measure(q2, q3), label="M_q2_q3")
 
     # test that all these operations compile correctly.
-    quantum_device = mock_setup["quantum_device"]
+    quantum_device = mock_setup_basic_transmon["quantum_device"]
     _ = compile_circuit_to_device(
         sched, device_cfg=quantum_device.generate_device_config()
     )
 
 
-def test_compile_asymmetric_gate(mock_setup):
+def test_compile_asymmetric_gate(mock_setup_basic_transmon):
     """
     Test if compilation fails when performing an asymmetric operation and the
     correct edge defining the parent-child device element connection is missing from
     the device config.
     """
     sched = Schedule("Test schedule")
 
@@ -104,15 +104,15 @@
     asymmetric_cz.data["gate_info"]["symmetric"] = False
 
     sched.add(Reset(q2, q3))
     sched.add(operation=asymmetric_cz)
     sched.add(Measure(q2, q3), label="M_q2_q3")
 
     # test that all these operations compile correctly.
-    quantum_device = mock_setup["quantum_device"]
+    quantum_device = mock_setup_basic_transmon["quantum_device"]
 
     with pytest.raises(ConfigKeyError):
         _ = compile_circuit_to_device(
             sched, device_cfg=quantum_device.generate_device_config()
         )
```

### Comparing `quantify-scheduler-0.8.0/tests/scheduler/backends/test_qblox_backend.py` & `quantify-scheduler-0.9.0/tests/scheduler/backends/test_qblox_backend.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,15 +15,17 @@
 import re
 import shutil
 import tempfile
 
 from typing import Dict, Generator
 
 import numpy as np
+
 import pytest
+from pydantic import ValidationError
 from qblox_instruments import Pulsar, PulsarType
 
 from quantify_core.data.handling import set_datadir  # pylint: disable=no-name-in-module
 
 import quantify_scheduler
 from quantify_scheduler import Schedule
 
@@ -49,22 +51,26 @@
     QcmModule,
     QcmRfModule,
     QrmModule,
     QrmRfModule,
 )
 from quantify_scheduler.backends.qblox.qasm_program import QASMProgram
 from quantify_scheduler.backends.types import qblox as types
-from quantify_scheduler.backends.types.qblox import BasebandModuleSettings
+from quantify_scheduler.backends.types.qblox import (
+    BasebandModuleSettings,
+    MarkerConfiguration,
+)
 
 from quantify_scheduler.compilation import (
     determine_absolute_timing,
     device_compile,
     qcompile,
 )
 
+from quantify_scheduler.device_under_test.mock_setup import set_standard_params_transmon
 from quantify_scheduler.operations.acquisition_library import Trace
 from quantify_scheduler.operations.gate_library import Measure, Reset, X
 from quantify_scheduler.operations.pulse_library import (
     DRAGPulse,
     IdlePulse,
     RampPulse,
     ShiftClockPhase,
@@ -77,14 +83,15 @@
 from quantify_scheduler.schedules.timedomain_schedules import (
     allxy_sched,
     readout_calibration_sched,
 )
 
 from tests.fixtures.mock_setup import close_instruments
 
+
 REGENERATE_REF_FILES: bool = False  # Set flag to true to regenerate the reference files
 
 
 # --------- Test fixtures ---------
 @pytest.fixture
 def hardware_cfg_baseband():
     yield {
@@ -235,14 +242,45 @@
                 },
             },
         },
     }
 
 
 @pytest.fixture
+def hardware_cfg_latency_corrections_invalid():
+    return {
+        "backend": "quantify_scheduler.backends.qblox_backend.hardware_compile",
+        # None is not a valid key for the latency corrections
+        "latency_corrections": {"q0:mw-q0.01": 2e-8, "q1:mw-q1.01": None},
+        "qcm0": {
+            "instrument_type": "Pulsar_QCM",
+            "ref": "internal",
+            "complex_output_0": {
+                "portclock_configs": [{"port": "q0:mw", "clock": "q0.01"}],
+            },
+        },
+        "cluster0": {
+            "instrument_type": "Cluster",
+            "ref": "internal",
+            "cluster0_module1": {
+                "instrument_type": "QCM",
+                "complex_output_0": {
+                    "portclock_configs": [
+                        {
+                            "port": "q1:mw",
+                            "clock": "q1.01",
+                        }
+                    ],
+                },
+            },
+        },
+    }
+
+
+@pytest.fixture
 def hardware_cfg_two_qubit_gate():
     return {
         "backend": "quantify_scheduler.backends.qblox_backend.hardware_compile",
         "qcm0": {
             "instrument_type": "Pulsar_QCM",
             "ref": "internal",
             "complex_output_0": {
@@ -635,98 +673,38 @@
         ("q3:mw", "q3.01"),
         ("q2:mw", "q2.01"),
         ("q2:res", "q2.ro"),
         ("q3:res", "q3.ro"),
         ("q3:mw", "q3.01"),
         ("q4:mw", "q4.01"),
         ("q5:mw", "q5.01"),
+        ("q6:mw", "q6.01"),
         ("q4:res", "q4.ro"),
         ("q5:res", "q5.ro"),
+        ("q0:fl", "cl0.baseband"),
+        ("q1:fl", "cl0.baseband"),
+        ("q2:fl", "cl0.baseband"),
+        ("q3:fl", "cl0.baseband"),
+        ("q4:fl", "cl0.baseband"),
     }
     assert portclocks == answer
 
 
 def test_generate_port_clock_to_device_map(load_example_qblox_hardware_config):
     portclock_map = generate_port_clock_to_device_map(
         load_example_qblox_hardware_config
     )
     assert (None, None) not in portclock_map.keys()
-    assert len(portclock_map.keys()) == 13
+    assert len(portclock_map.keys()) == 19
 
 
 # --------- Test classes and member methods ---------
-def test_portclocks(
-    make_basic_multi_qubit_schedule, load_example_qblox_hardware_config
-):
 
-    device_config = {
-        "backend": "quantify_scheduler.compilation.add_pulse_information_transmon",
-        "edges": {},
-        "qubits": {
-            "q4": {
-                "params": {
-                    "acquisition": "SSBIntegrationComplex",
-                    "init_duration": 0.0002,
-                    "mw_amp180": 0.25,
-                    "mw_duration": 1.6e-08,
-                    "mw_ef_amp180": 0.87,
-                    "mw_freq": 6.02e9,
-                    "mw_motzoi": 0.45,
-                },
-                "resources": {
-                    "clock_01": "q4.01",
-                    "clock_12": "q4.12",
-                    "clock_ro": "q4.ro",
-                    "port_flux": "q4:fl",
-                    "port_mw": "q4:mw",
-                    "port_ro": "q4:res",
-                },
-            },
-            "q5": {
-                "params": {
-                    "acquisition": "SSBIntegrationComplex",
-                    "init_duration": 0.0002,
-                    "mw_amp180": 0.25,
-                    "mw_duration": 2e-08,
-                    "mw_ef_amp180": 0.67,
-                    "mw_freq": 5.02e9,
-                    "mw_motzoi": 0.45,
-                },
-                "resources": {
-                    "clock_01": "q5.01",
-                    "clock_12": "q5.12",
-                    "clock_ro": "q5.ro",
-                    "port_flux": "q5:fl",
-                    "port_mw": "q5:mw",
-                    "port_ro": "q5:res",
-                },
-            },
-        },
-    }
-
-    sched = make_basic_multi_qubit_schedule(["q4", "q5"])
-    sched = device_compile(sched, device_config)
-
-    hardware_cfg = load_example_qblox_hardware_config
-    container = compiler_container.CompilerContainer.from_hardware_cfg(
-        sched, hardware_cfg
-    )
-
-    assign_pulse_and_acq_info_to_devices(
-        schedule=sched,
-        hardware_cfg=hardware_cfg,
-        device_compilers=container.instrument_compilers,
-    )
-
-    compilers = container.instrument_compilers["cluster0"].instrument_compilers
-    assert compilers["cluster0_module1"].portclocks == [("q4:mw", "q4.01")]
-    assert compilers["cluster0_module2"].portclocks == [("q5:mw", "q5.01")]
 
-
-def test_contruct_sequencers(
+def test_construct_sequencers(
     make_basic_multi_qubit_schedule,
     load_example_transmon_config,
     load_example_qblox_hardware_config,
 ):
     test_module = QcmModule(
         parent=None,
         name="tester",
@@ -745,15 +723,15 @@
     test_module.sequencers = test_module._construct_sequencers()
     seq_keys = list(test_module.sequencers.keys())
 
     assert len(seq_keys) == 2
     assert isinstance(test_module.sequencers[seq_keys[0]], Sequencer)
 
 
-def test_contruct_sequencers_repeated_portclocks_error(
+def test_construct_sequencers_repeated_portclocks_error(
     make_basic_multi_qubit_schedule,
     load_example_transmon_config,
     load_example_qblox_hardware_config,
 ):
     hardware_cfg = copy.deepcopy(load_example_qblox_hardware_config)
 
     hardware_cfg["qcm0"]["complex_output_0"]["portclock_configs"] = [
@@ -787,16 +765,18 @@
     with pytest.raises(ValueError):
         test_module.sequencers = test_module._construct_sequencers()
 
 
 @pytest.mark.parametrize(
     "element_names", [[f"q{i}" for i in range(constants.NUMBER_OF_SEQUENCERS_QCM + 1)]]
 )
-def test_contruct_sequencers_excess_error(
-    mock_setup_basic_transmon_elements, make_basic_multi_qubit_schedule, element_names
+def test_construct_sequencers_excess_error(
+    mock_setup_basic_transmon_elements,
+    make_basic_multi_qubit_schedule,
+    element_names,
 ):
     hardware_cfg = {
         "backend": "quantify_scheduler.backends.qblox_backend.hardware_compile",
         "qcm0": {
             "instrument_type": "Pulsar_QCM_RF",
             "ref": "internal",
             "complex_output_0": {
@@ -832,14 +812,45 @@
     assert (
         "Number of simultaneously active port-clock combinations exceeds "
         + "number of sequencers."
         in str(exc.value)
     )
 
 
+def test_portclocks(
+    mock_setup_basic_transmon,
+    make_basic_multi_qubit_schedule,
+    load_example_qblox_hardware_config,
+):
+
+    quantum_device = mock_setup_basic_transmon["quantum_device"]
+    device_config = quantum_device.generate_device_config()
+
+    sched = make_basic_multi_qubit_schedule(["q3", "q4"])
+    sched = device_compile(sched, device_config)
+
+    hardware_cfg = load_example_qblox_hardware_config
+    container = compiler_container.CompilerContainer.from_hardware_cfg(
+        sched, hardware_cfg
+    )
+
+    assign_pulse_and_acq_info_to_devices(
+        schedule=sched,
+        hardware_cfg=hardware_cfg,
+        device_compilers=container.instrument_compilers,
+    )
+
+    compilers = container.instrument_compilers["cluster0"].instrument_compilers
+    assert compilers["cluster0_module1"].portclocks == [("q4:mw", "q4.01")]
+    assert compilers["cluster0_module2"].portclocks == [
+        ("q5:mw", "q5.01"),
+        ("q6:mw", "q6.01"),
+    ]
+
+
 def test_compile_simple(
     pulse_only_schedule,
     load_example_transmon_config,
     load_example_qblox_hardware_config,
 ):
     """Tests if compilation with only pulses finishes without exceptions"""
     tmp_dir = tempfile.TemporaryDirectory()
@@ -848,23 +859,23 @@
         pulse_only_schedule,
         load_example_transmon_config,
         load_example_qblox_hardware_config,
     )
 
 
 def test_compile_cluster(
-    mock_setup,
+    mock_setup_basic_transmon,
     cluster_only_schedule,
     load_example_qblox_hardware_config,
 ):
     tmp_dir = tempfile.TemporaryDirectory()
     set_datadir(tmp_dir.name)
     qcompile(
         cluster_only_schedule,
-        mock_setup["quantum_device"].generate_device_config(),
+        mock_setup_basic_transmon["quantum_device"].generate_device_config(),
         load_example_qblox_hardware_config,
     )
 
 
 def test_compile_no_device_cfg(load_example_qblox_hardware_config):
     tmp_dir = tempfile.TemporaryDirectory()
     set_datadir(tmp_dir.name)
@@ -944,51 +955,63 @@
     [
         (IdlePulse(duration=64e-9), "wait       64"),
         (Reset("q1"), "wait       65532"),
         (ShiftClockPhase(clock="q1.01", phase=180.0), "set_ph_delta  199,399,6249"),
     ],
 )
 def test_compile_clock_operations(
-    mock_setup, hardware_cfg_baseband, operation: Operation, instruction_to_check: str
+    mock_setup_basic_transmon,
+    hardware_cfg_baseband,
+    operation: Operation,
+    instruction_to_check: str,
 ):
-    # mock_setup should arrange this but is not working here
+    # mock_setup_basic_transmon should arrange this but is not working here
     tmp_dir = tempfile.TemporaryDirectory()
     set_datadir(tmp_dir.name)
 
     sched = Schedule("shift_clock_phase_only")
     sched.add(operation)
     sched.add_resources(
         [ClockResource("q1.01", freq=5e9)]
     )  # Clocks need to be manually added at this stage.
 
     compiled_sched = qcompile(
         schedule=sched,
-        device_cfg=mock_setup["quantum_device"].generate_device_config(),
+        device_cfg=mock_setup_basic_transmon["quantum_device"].generate_device_config(),
         hardware_cfg=hardware_cfg_baseband,
     )
 
     filename = compiled_sched.compiled_instructions["qcm0"]["seq0"]["seq_fn"]
     with open(filename, "r") as file:
         program_lines = json.load(file)["program"].splitlines()
 
     assert any(instruction_to_check in line for line in program_lines), "\n".join(
         line for line in program_lines
     )
 
 
 def test_compile_cz_gate(
-    mock_setup, hardware_cfg_two_qubit_gate, two_qubit_gate_schedule
+    mock_setup_basic_transmon, hardware_cfg_two_qubit_gate, two_qubit_gate_schedule
 ):
-    # mock_setup should arrange this but is not working here
+    # mock_setup_basic_transmon should arrange this but is not working here
     tmp_dir = tempfile.TemporaryDirectory()
     set_datadir(tmp_dir.name)
 
+    set_standard_params_transmon(mock_setup_basic_transmon)
+
+    edge_q2_q3 = mock_setup_basic_transmon["q2_q3"]
+    edge_q2_q3.cz.q2_phase_correction(44)
+    edge_q2_q3.cz.q3_phase_correction(63)
+
+    quantum_device = mock_setup_basic_transmon["quantum_device"]
+    device_cfg = quantum_device.generate_device_config()
+
     compiled_sched = qcompile(
         schedule=two_qubit_gate_schedule,
-        device_cfg=mock_setup["quantum_device"].generate_device_config(),
+        device_cfg=device_cfg,
         hardware_cfg=hardware_cfg_two_qubit_gate,
     )
 
     program_lines = {}
     for seq in ["seq0", "seq1", "seq2"]:
         filename = compiled_sched.compiled_instructions["qcm0"][seq]["seq_fn"]
         with open(filename, "r") as file:
@@ -1263,16 +1286,16 @@
     )
     assign_pulse_and_acq_info_to_devices(
         sched_with_pulse_info,
         container.instrument_compilers,
         load_example_qblox_hardware_config,
     )
     qrm = container.instrument_compilers["qrm0"]
-    assert len(qrm._pulses[list(qrm.portclocks_with_data)[0]]) == 1
-    assert len(qrm._acquisitions[list(qrm.portclocks_with_data)[0]]) == 1
+    assert len(qrm._pulses[list(qrm._portclocks_with_data)[0]]) == 1
+    assert len(qrm._acquisitions[list(qrm._portclocks_with_data)[0]]) == 1
 
 
 def test_container_prepare(
     pulse_only_schedule,
     load_example_transmon_config,
     load_example_qblox_hardware_config,
 ):
@@ -1291,28 +1314,31 @@
     assert (
         container.instrument_compilers["qcm0"].sequencers["seq0"].frequency is not None
     )
     assert container.instrument_compilers["lo0"].frequency is not None
 
 
 def test_determine_scope_mode_acquisition_sequencer(
-    mock_setup, load_example_qblox_hardware_config
+    mock_setup_basic_transmon, load_example_qblox_hardware_config
 ):
-    # mock_setup should arrange this but is not working here
+    # mock_setup_basic_transmon should arrange this but is not working here
     tmp_dir = tempfile.TemporaryDirectory()
     set_datadir(tmp_dir.name)
 
+    set_standard_params_transmon(mock_setup_basic_transmon)
     sched = Schedule("determine_scope_mode_acquisition_sequencer")
     sched.add(Measure("q0"))
     sched.add(Trace(duration=100e-9, port="q0:res", clock="q0.multiplex"))
     sched.add(Trace(duration=100e-9, port="q5:res", clock="q5.ro"))
 
     hardware_cfg = load_example_qblox_hardware_config
     sched = qcompile(
-        sched, mock_setup["quantum_device"].generate_device_config(), hardware_cfg
+        sched,
+        mock_setup_basic_transmon["quantum_device"].generate_device_config(),
+        hardware_cfg,
     )
 
     assert hardware_cfg["qrm0"]["instrument_type"] == "Pulsar_QRM"
     assert sched.compiled_instructions["qrm0"]["settings"]["scope_mode_sequencer"] == 1
 
     assert hardware_cfg["cluster0"]["cluster0_module4"]["instrument_type"] == "QRM_RF"
     assert (
@@ -1564,15 +1590,15 @@
     assert expected_if1 == actual_if1, (
         f"Modulation frequency of channel 1 {status} downconversion must be equal to "
         f"{expected_if1} but it is equal to {actual_if1}"
     )
 
 
 def test_assign_frequencies_rf(
-    load_legacy_transmon_config, load_example_qblox_hardware_config
+    mock_setup_basic_transmon, load_example_qblox_hardware_config
 ):
     tmp_dir = tempfile.TemporaryDirectory()
     set_datadir(tmp_dir.name)
 
     sched = Schedule("two_gate_experiment")
     sched.add(X("q2"))
     sched.add(X("q3"))
@@ -1588,41 +1614,48 @@
     lo1 = hardware_cfg["qcm_rf0"]["complex_output_1"].get("lo_freq")
 
     assert if0 is not None
     assert if1 is None
     assert lo0 is None
     assert lo1 is not None
 
-    device_cfg = load_legacy_transmon_config
-    q2_clock_freq = device_cfg["qubits"]["q2"]["params"]["mw_freq"]
-    q3_clock_freq = device_cfg["qubits"]["q3"]["params"]["mw_freq"]
+    quantum_device = mock_setup_basic_transmon["quantum_device"]
 
-    if0 = hardware_cfg["qcm_rf0"]["complex_output_0"]["portclock_configs"][0][
-        "interm_freq"
-    ]
-    lo1 = hardware_cfg["qcm_rf0"]["complex_output_1"]["lo_freq"]
+    q2 = quantum_device.get_element("q2")
+    q3 = quantum_device.get_element("q3")
+    q2.clock_freqs.f01.set(6.02e9)
+    q3.clock_freqs.f01.set(5.02e9)
+
+    q2.rxy.amp180(0.213)
+    q3.rxy.amp180(0.215)
+
+    device_cfg = quantum_device.generate_device_config()
+
+    q2_clock_freq = device_cfg.clocks["q2.01"]
+    q3_clock_freq = device_cfg.clocks["q3.01"]
 
     lo0 = q2_clock_freq - if0
     if1 = q3_clock_freq - lo1
 
     compiled_schedule = qcompile(sched, device_cfg, hardware_cfg)
     compiled_instructions = compiled_schedule["compiled_instructions"]
     qcm_program = compiled_instructions["qcm_rf0"]
+
     assert qcm_program["settings"]["lo0_freq"] == lo0
     assert qcm_program["settings"]["lo1_freq"] == lo1
     assert qcm_program["seq1"]["settings"]["modulation_freq"] == if1
 
 
 @pytest.mark.parametrize(
     "downconverter_freq_0, downconverter_freq_1", [(0, 0), (8.2e9, 8.2e9)]
 )
 def test_assign_frequencies_rf_downconverter(
     downconverter_freq_0,
     downconverter_freq_1,
-    load_legacy_transmon_config,
+    mock_setup_basic_transmon,
     load_example_qblox_hardware_config,
 ):
     tmp_dir = tempfile.TemporaryDirectory()
     set_datadir(tmp_dir.name)
 
     sched = Schedule("two_gate_experiment")
     sched.add(X("q2"))
@@ -1649,21 +1682,32 @@
     ), "Modulation frequency must be set for channel 0 in hardware config"
     assert (
         if1 is None
     ), "Modulation frequency already set for channel 1 in hardware config"
     assert lo0 is None, "LO frequency already set for channel 0 in hardware config"
     assert lo1 is not None, "LO frequency must be set for channel 1 in hardware config"
 
-    device_cfg = load_legacy_transmon_config
+    quantum_device = mock_setup_basic_transmon["quantum_device"]
+
+    q2 = quantum_device.get_element("q2")
+    q3 = quantum_device.get_element("q3")
+    q2.clock_freqs.f01.set(6.02e9)
+    q3.clock_freqs.f01.set(5.02e9)
+
+    q2.rxy.amp180(0.213)
+    q3.rxy.amp180(0.215)
+
+    device_cfg = quantum_device.generate_device_config()
+
     compiled_schedule = qcompile(sched, device_cfg, hardware_cfg)
     compiled_instructions = compiled_schedule["compiled_instructions"]
     qcm_program = compiled_instructions["qcm_rf0"]
 
-    q2_clock_freq = device_cfg["qubits"]["q2"]["params"]["mw_freq"]
-    q3_clock_freq = device_cfg["qubits"]["q3"]["params"]["mw_freq"]
+    q2_clock_freq = device_cfg.clocks["q2.01"]
+    q3_clock_freq = device_cfg.clocks["q3.01"]
 
     actual_lo0 = qcm_program["settings"]["lo0_freq"]
     actual_lo1 = qcm_program["settings"]["lo1_freq"]
     actual_if1 = qcm_program["seq1"]["settings"]["modulation_freq"]
 
     expected_lo1 = lo1
 
@@ -1687,32 +1731,49 @@
     )
     assert expected_if1 == actual_if1, (
         f"Modulation frequency of channel 1 {status} downconversion must be equal "
         f"to {expected_if1}, but it is equal to {actual_if1}"
     )
 
 
-def test_markers(load_legacy_transmon_config, load_example_qblox_hardware_config):
+def test_markers(mock_setup_basic_transmon, load_example_qblox_hardware_config):
     tmp_dir = tempfile.TemporaryDirectory()
     set_datadir(tmp_dir.name)
 
     # Test for baseband
     sched = Schedule("gate_experiment")
     sched.add(X("q0"))
     sched.add(X("q2"))
     sched.add(Measure("q0"))
     sched.add(Measure("q2"))
 
-    compiled_schedule = qcompile(
-        sched, load_legacy_transmon_config, load_example_qblox_hardware_config
-    )
+    quantum_device = mock_setup_basic_transmon["quantum_device"]
+
+    q0 = quantum_device.get_element("q0")
+    q2 = quantum_device.get_element("q2")
+
+    q0.rxy.amp180(0.213)
+    q2.rxy.amp180(0.215)
+
+    q0.clock_freqs.f01(7.3e9)
+    q0.clock_freqs.f12(7.0e9)
+    q0.clock_freqs.readout(8.0e9)
+    q0.measure.acq_delay(100e-9)
+
+    q2.clock_freqs.f01(7.3e9)
+    q2.clock_freqs.f12(7.0e9)
+    q2.clock_freqs.readout(8.0e9)
+    q2.measure.acq_delay(100e-9)
+
+    device_cfg = quantum_device.generate_device_config()
+
+    compiled_schedule = qcompile(sched, device_cfg, load_example_qblox_hardware_config)
     program = compiled_schedule["compiled_instructions"]
 
-    def _confirm_correct_markers(device_program, device_compiler, is_rf=False):
-        mrk_config = device_compiler.static_hw_properties.marker_configuration
+    def _confirm_correct_markers(device_program, mrk_config, is_rf=False):
         answers = (
             mrk_config.init,
             mrk_config.start,
             mrk_config.end,
         )
         with open(device_program["seq0"]["seq_fn"]) as file:
             qasm = json.load(file)["program"]
@@ -1721,18 +1782,30 @@
             matches = [int(m.replace("set_mrk", "").strip()) for m in matches]
             if not is_rf:
                 matches = [None, *matches]
 
             for match, answer in zip(matches, answers):
                 assert match == answer
 
-    _confirm_correct_markers(program["qcm0"], QcmModule)
-    _confirm_correct_markers(program["qrm0"], QrmModule)
-    _confirm_correct_markers(program["qcm_rf0"], QcmRfModule, is_rf=True)
-    _confirm_correct_markers(program["qrm_rf0"], QrmRfModule, is_rf=True)
+    _confirm_correct_markers(
+        program["qcm0"], MarkerConfiguration(init=None, start=0b1111, end=0)
+    )
+    _confirm_correct_markers(
+        program["qrm0"], MarkerConfiguration(init=None, start=0b1111, end=0)
+    )
+    _confirm_correct_markers(
+        program["qcm_rf0"],
+        MarkerConfiguration(init=0b0011, start=0b1101, end=0),
+        is_rf=True,
+    )
+    _confirm_correct_markers(
+        program["qrm_rf0"],
+        MarkerConfiguration(init=0b0011, start=0b1111, end=0),
+        is_rf=True,
+    )
 
 
 def test_pulsar_rf_extract_from_mapping(load_example_qblox_hardware_config):
     hw_map = load_example_qblox_hardware_config["qcm_rf0"]
     types.PulsarRFSettings.extract_settings_from_mapping(hw_map)
 
 
@@ -1904,15 +1977,15 @@
 
     # the only key corresponds to channel 0
     assert set(acquisitions.keys()) == {"0"}
     assert acquisitions["0"] == {"num_bins": 21, "index": 0}
 
 
 def test_convert_hw_config_to_portclock_configs_spec(
-    make_basic_multi_qubit_schedule, load_legacy_transmon_config
+    make_basic_multi_qubit_schedule, load_example_transmon_config
 ):
     old_config = {
         "backend": "quantify_scheduler.backends.qblox_backend.hardware_compile",
         "qcm0": {
             "instrument_type": "Pulsar_QCM",
             "ref": "internal",
             "complex_output_0": {
@@ -2012,46 +2085,82 @@
     migrated_config = convert_hw_config_to_portclock_configs_spec(old_config)
     assert migrated_config == expected_config
 
     # Test that hardware_compile is converting automatically
     tmp_dir = tempfile.TemporaryDirectory()
     set_datadir(tmp_dir.name)
 
-    sched = make_basic_multi_qubit_schedule(["q0", "q1", "q2"])
-    sched = device_compile(sched, load_legacy_transmon_config)
+    sched = make_basic_multi_qubit_schedule(["q0", "q1"])
+    sched = device_compile(sched, load_example_transmon_config)
     with pytest.warns(
         DeprecationWarning,
         match=r"hardware config adheres to a specification that is deprecated",
     ):
         hardware_compile(sched, old_config)
 
 
-def test_apply_latency_corrections_valid(mock_setup, hardware_cfg_latency_corrections):
+def test_apply_latency_corrections_invalid_raises(
+    mock_setup_basic_transmon, hardware_cfg_latency_corrections_invalid
+):
+    """
+    This test function checks that:
+    Providing an invalid latency correction specification raises an exception
+    when compiling.
+    """
+    # mock_setup should arrange this but is not working here
+    tmp_dir = tempfile.TemporaryDirectory()
+    set_datadir(tmp_dir.name)
+
+    sched = Schedule("Single Gate Experiment on Two Qubits")
+    sched.add(X("q0"))
+    sched.add(
+        SquarePulse(port="q1:mw", clock="q1.01", amp=0.25, duration=12e-9),
+        ref_pt="start",
+    )
+    sched.add_resources([ClockResource("q0.01", freq=5e9)])
+    sched.add_resources([ClockResource("q1.01", freq=5e9)])
+
+    hardware_cfg = copy.deepcopy(hardware_cfg_latency_corrections_invalid)
+    hardware_cfg["latency_corrections"]["q1:mw-q1.01"] = None
+    with pytest.raises(ValidationError):
+        _ = qcompile(
+            schedule=sched,
+            device_cfg=mock_setup_basic_transmon[
+                "quantum_device"
+            ].generate_device_config(),
+            hardware_cfg=hardware_cfg,
+        )
+
+
+def test_apply_latency_corrections_valid(
+    mock_setup_basic_transmon, hardware_cfg_latency_corrections
+):
     """
     This test function checks that:
     Latency correction is set for the correct portclock key
     by checking against the value set in QASM instructions.
     """
-    # mock_setup should arrange this but is not working here
+    # mock_setup_basic_transmon should arrange this but is not working here
     tmp_dir = tempfile.TemporaryDirectory()
     set_datadir(tmp_dir.name)
 
+    set_standard_params_transmon(mock_setup_basic_transmon)
     sched = Schedule("Single Gate Experiment on Two Qubits")
     sched.add(X("q0"))
     sched.add(
         SquarePulse(port="q1:mw", clock="q1.01", amp=0.25, duration=12e-9),
         ref_pt="start",
     )
     sched.add_resources([ClockResource("q0.01", freq=5e9)])
     sched.add_resources([ClockResource("q1.01", freq=5e9)])
 
     hardware_cfg = hardware_cfg_latency_corrections
     compiled_sched = qcompile(
         schedule=sched,
-        device_cfg=mock_setup["quantum_device"].generate_device_config(),
+        device_cfg=mock_setup_basic_transmon["quantum_device"].generate_device_config(),
         hardware_cfg=hardware_cfg,
     )
 
     for instrument in ["qcm0", ("cluster0", "cluster0_module1")]:
         compiled_data = compiled_sched.compiled_instructions
         config_data = hardware_cfg
 
@@ -2074,21 +2183,21 @@
         assert any(
             f"latency correction of {constants.GRID_TIME} + {latency} ns" in line
             for line in program_lines
         ), f"instrument={instrument}, latency={latency}"
 
 
 def test_apply_latency_corrections_warning(
-    mock_setup, hardware_cfg_latency_corrections, caplog
+    mock_setup_basic_transmon, hardware_cfg_latency_corrections, caplog
 ):
     """
     Checks if warning is raised for a latency correction
     that is not a multiple of 4ns
     """
-    # mock_setup should arrange this but is not working here
+    # mock_setup_basic_transmon should arrange this but is not working here
     tmp_dir = tempfile.TemporaryDirectory()
     set_datadir(tmp_dir.name)
 
     sched = Schedule("Single Gate Experiment")
     sched.add(
         SquarePulse(port="q1:mw", clock="q1.01", amp=0.25, duration=12e-9),
         ref_pt="start",
@@ -2097,15 +2206,17 @@
 
     warning = f"not a multiple of {constants.GRID_TIME}"
     with caplog.at_level(
         logging.WARNING, logger="quantify_scheduler.backends.qblox.qblox_backend"
     ):
         qcompile(
             schedule=sched,
-            device_cfg=mock_setup["quantum_device"].generate_device_config(),
+            device_cfg=mock_setup_basic_transmon[
+                "quantum_device"
+            ].generate_device_config(),
             hardware_cfg=hardware_cfg_latency_corrections,
         )
     assert any(warning in mssg for mssg in caplog.messages)
 
 
 def _strip_comments(program: str):
     # helper function for comparing programs
```

### Comparing `quantify-scheduler-0.8.0/tests/scheduler/backends/test_zhinst_backend.py` & `quantify-scheduler-0.9.0/tests/scheduler/backends/test_zhinst_backend.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,20 +3,22 @@
 # pylint: disable=missing-function-docstring
 # pylint: disable=redefined-outer-name
 # pylint: disable=too-many-locals
 # pylint: disable=too-many-lines
 from __future__ import annotations
 
 import json
+from copy import deepcopy
 from textwrap import dedent
 from typing import Any, Dict, List
 from unittest.mock import ANY, call
 
 import numpy as np
 import pytest
+from pydantic import ValidationError
 from quantify_core.data.handling import set_datadir
 from zhinst.qcodes import hdawg, mfli, uhfli, uhfqa
 from zhinst.toolkit.control import drivers
 
 from quantify_scheduler import Schedule, enums
 from quantify_scheduler.backends import zhinst_backend
 from quantify_scheduler.backends.types import common, zhinst
@@ -24,18 +26,28 @@
 from quantify_scheduler.compilation import qcompile
 from quantify_scheduler.helpers import schedule as schedule_helpers
 from quantify_scheduler.helpers import waveforms as waveform_helpers
 from quantify_scheduler.operations.gate_library import X90, Measure, Reset
 from quantify_scheduler.schedules import spectroscopy_schedules, trace_schedules
 from quantify_scheduler.schedules.verification import acquisition_staircase_sched
 from quantify_scheduler.schemas.examples.utils import load_json_example_scheme
+from quantify_scheduler.operations.acquisition_library import SSBIntegrationComplex
+from quantify_scheduler.resources import ClockResource
 
 ARRAY_DECIMAL_PRECISION = 16
 
 
+@pytest.fixture
+def zhinst_hw_config_invalid_latencies(load_example_zhinst_hardware_config):
+    hw_config = deepcopy(load_example_zhinst_hardware_config)
+    hw_config["latency_corrections"] = {"q0:mw-q0.01": 2e-8, "q1:mw-q1.01": None}
+
+    yield hw_config
+
+
 def test__determine_measurement_fixpoint_correction():
 
     for i in range(16):
         (
             time_corr,
             sample_correction,
         ) = zhinst_backend._determine_measurement_fixpoint_correction(
@@ -328,14 +340,27 @@
     # assert "lo0" in device_configs
     # ro_freq = 7.04e9
     # intermodulation_frequency = 150e6
 
     # assert device_configs["lo0"] == ro_freq - intermodulation_frequency
 
 
+def test_compile_invalid_latencies_raises(
+    make_schedule,
+    zhinst_hw_config_invalid_latencies,
+) -> None:
+    hardware_cfg = zhinst_hw_config_invalid_latencies
+    # Arrange
+    schedule = make_schedule()
+
+    # should raise a pydantic validation error
+    with pytest.raises(ValidationError):
+        _ = zhinst_backend.compile_backend(schedule, hardware_cfg)
+
+
 def test_hdawg4_sequence(
     load_example_zhinst_hardware_config,
     make_schedule,
 ) -> None:
     hdawg_hardware_cfg = load_example_zhinst_hardware_config
     # Arrange
     awg_index = 0
@@ -377,15 +402,17 @@
 
     assert node == "compiler/sourcestring"
     assert zi_setting[0] == awg_index
     assert zi_setting[1].value == expected_seqc
 
 
 # pylint: disable=too-many-arguments
-@pytest.mark.parametrize("channelgrouping,enabled_channels", [(0, [0, 1]), (1, [0])])
+@pytest.mark.parametrize(
+    "channelgrouping,enabled_channels", [(0, [0, 1, 2, 3]), (1, [0])]
+)
 def test__program_hdawg4_channelgrouping(
     mocker,
     create_typical_timing_table,
     channelgrouping: int,
     enabled_channels: List[int],
 ):
 
@@ -773,14 +800,16 @@
     load_example_zhinst_hardware_config,
 ) -> None:
     hardware_config = load_example_zhinst_hardware_config
 
     expected_dict = {
         "q0:mw-q0.01": "ic_hdawg0.awg0",
         "q1:mw-q1.01": "ic_hdawg0.awg1",
+        "q2:mw-q2.01": "ic_hdawg0.awg2",
+        "q3:mw-q3.01": "ic_hdawg0.awg3",
         "q0:res-q0.ro": "ic_uhfqa0.awg0",
     }
     generated_dict = zhinst_backend._extract_port_clock_channelmapping(
         hardware_cfg=hardware_config
     )
     assert generated_dict == expected_dict
 
@@ -788,16 +817,18 @@
 def test__extract_latencies(
     load_example_zhinst_hardware_config,
 ) -> None:
     hardware_config = load_example_zhinst_hardware_config
 
     expected_latency_dict = {
         "q0:mw-q0.01": 190e-9,
-        "q0:res-q0.ro": 0,
+        "q0:res-q0.ro": 0.0,
         "q1:mw-q1.01": 190e-9,
+        "q2:mw-q2.01": 9.5e-08,
+        "q3:mw-q3.01": 9.5e-08,
     }
     generated_dict = zhinst_backend._extract_latencies(hardware_cfg=hardware_config)
 
     assert generated_dict == expected_latency_dict
 
 
 @pytest.mark.parametrize(
@@ -1127,7 +1158,41 @@
             decimal=ARRAY_DECIMAL_PRECISION,
         )
         np.testing.assert_array_almost_equal(
             settings_dict[f"qas/0/integration/weights/{i}/imag"],
             expected_zeros_array,
             decimal=ARRAY_DECIMAL_PRECISION,
         )
+
+
+def test_too_long_acquisition_raises_readable_exception():
+    sched = Schedule(name="Too long acquisition schedule", repetitions=1024)
+
+    # these are kind of magic names that are known to exist in the default config.
+    port = "q0:res"
+    clock = "q0.ro"
+
+    # this should not be required.
+    sched.add_resource(ClockResource(name=clock, freq=5e9))
+
+    sched.add(
+        SSBIntegrationComplex(
+            duration=2.4e-6,  # this is longer than the allowed 4096 samples.
+            port=port,
+            clock=clock,
+            acq_index=0,
+            acq_channel=0,
+        ),
+    )
+
+    device_cfg = load_json_example_scheme("transmon_test_config.json")
+    hw_cfg = load_json_example_scheme("zhinst_test_mapping.json")
+
+    # Act
+    with pytest.raises(ValueError) as exc_info:
+        _ = qcompile(sched, device_cfg=device_cfg, hardware_cfg=hw_cfg)
+
+    # assert that the name of the offending operation is in the exception message.
+    assert "SSBIntegrationComplex(" in str(exc_info.value)
+
+    # assert that the number of samples we are trying to set is in the exception message
+    assert "4320 samples" in str(exc_info.value)
```

### Comparing `quantify-scheduler-0.8.0/tests/scheduler/backends/zhinst/test_helpers.py` & `quantify-scheduler-0.9.0/tests/scheduler/backends/zhinst/test_helpers.py`

 * *Files identical despite different names*

### Comparing `quantify-scheduler-0.8.0/tests/scheduler/backends/zhinst/test_resolvers.py` & `quantify-scheduler-0.9.0/tests/scheduler/backends/zhinst/test_resolvers.py`

 * *Files identical despite different names*

### Comparing `quantify-scheduler-0.8.0/tests/scheduler/backends/zhinst/test_seqc_il_generator.py` & `quantify-scheduler-0.9.0/tests/scheduler/backends/zhinst/test_seqc_il_generator.py`

 * *Files identical despite different names*

### Comparing `quantify-scheduler-0.8.0/tests/scheduler/backends/zhinst/test_settings.py` & `quantify-scheduler-0.9.0/tests/scheduler/backends/zhinst/test_settings.py`

 * *Files identical despite different names*

### Comparing `quantify-scheduler-0.8.0/tests/scheduler/device_under_test/test_composite_square_edge.py` & `quantify-scheduler-0.9.0/tests/scheduler/device_under_test/test_composite_square_edge.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     q3b.close()
     edge_q2b_q3b.close()
 
 
 def test_generate_edge_config(edge_q2b_q3b):
     # Setup
     expected_edge_cfg = {
-        "q2b-q3b": {
+        "q2b_q3b": {
             "CZ": OperationCompilationConfig(
                 factory_func="quantify_scheduler.operations."
                 + "pulse_factories.composite_square_pulse",
                 factory_kwargs={
                     "square_port": "q2b:fl",
                     "square_clock": "cl0.baseband",
                     "square_amp": 0.65,
@@ -45,15 +45,15 @@
                     "virt_z_child_qubit_phase": 63,
                     "virt_z_child_qubit_clock": "q3b.01",
                 },
             ),
         }
     }
 
-    expected_cz_dict = expected_edge_cfg["q2b-q3b"]["CZ"].dict()
+    expected_cz_dict = expected_edge_cfg["q2b_q3b"]["CZ"].dict()
 
     edge_q2b_q3b.cz.square_amp(expected_cz_dict["factory_kwargs"]["square_amp"])
     edge_q2b_q3b.cz.square_duration(
         expected_cz_dict["factory_kwargs"]["square_duration"]
     )
     edge_q2b_q3b.cz.q2b_phase_correction(
         expected_cz_dict["factory_kwargs"]["virt_z_parent_qubit_phase"]
```

### Comparing `quantify-scheduler-0.8.0/tests/scheduler/device_under_test/test_quantum_device.py` & `quantify-scheduler-0.9.0/tests/scheduler/device_under_test/test_quantum_device.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,32 +1,35 @@
 # pylint: disable=missing-function-docstring
 # pylint: disable=invalid-name
 
 import pytest
 from quantify_scheduler.compilation import validate_config
+from quantify_scheduler.device_under_test.device_element import DeviceElement
 from quantify_scheduler.device_under_test.quantum_device import QuantumDevice
 
 
-def test_QuantumDevice_generate_device_config(mock_setup: dict) -> None:
+def test_QuantumDevice_generate_device_config(mock_setup_basic_transmon: dict) -> None:
 
-    quantum_device = mock_setup["quantum_device"]
+    quantum_device = mock_setup_basic_transmon["quantum_device"]
 
     # N.B. the validation of the generated config is happening inside the
     # device object itself using the pydantic dataclass. Invoking the function
     # tests this directly.
     dev_cfg = quantum_device.generate_device_config()
 
     assert {"q0", "q1", "q2", "q3"} <= set(dev_cfg.elements.keys())
     # Ensure that we also check that the edges are being configured
-    assert "q2-q3" in dev_cfg.edges
+    assert "q2_q3" in dev_cfg.edges
 
 
-def test_QuantumDevice_generate_hardware_config(mock_setup: dict) -> None:
+def test_QuantumDevice_generate_hardware_config(
+    mock_setup_basic_transmon: dict,
+) -> None:
 
-    quantum_device = mock_setup["quantum_device"]
+    quantum_device = mock_setup_basic_transmon["quantum_device"]
 
     mock_hardware_cfg = {
         "backend": "quantify_scheduler.backends.qblox_backend.hardware_compile",
         "ic_qcm0": {
             "name": "qcm0",
             "instrument_type": "Pulsar_QCM",
             "mode": "complex",
@@ -76,11 +79,18 @@
 @pytest.fixture
 def test_mc() -> QuantumDevice:
     test_mc = QuantumDevice("test_mc")
     yield test_mc
     test_mc.close()
 
 
-def test_adding_non_component_raises(dev, test_mc):
+def test_adding_non_element_raises(dev, test_mc):
 
     with pytest.raises(TypeError):
-        dev.add_component(test_mc)
+        dev.add_element(test_mc)
+
+
+def test_invalid_device_element_name():
+
+    invalid_name = "q_0"
+    with pytest.raises(ValueError):
+        DeviceElement(invalid_name)
```

### Comparing `quantify-scheduler-0.8.0/tests/scheduler/device_under_test/test_transmon_element.py` & `quantify-scheduler-0.9.0/tests/scheduler/device_under_test/test_transmon_element.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 # pylint: disable=missing-class-docstring
 # pylint: disable=missing-function-docstring
 # pylint: disable=redefined-outer-name
 import pytest
 
 from quantify_scheduler.compilation import validate_config
 from quantify_scheduler.device_under_test.transmon_element import (
-    TransmonElement,
     BasicTransmonElement,
 )
 from quantify_scheduler.device_under_test.quantum_device import QuantumDevice
 from quantify_scheduler.instrument_coordinator.instrument_coordinator import (
     InstrumentCoordinator,
 )
 from quantify_scheduler.backends.circuit_to_device import (
@@ -18,54 +17,54 @@
     DeviceCompilationConfig,
 )
 
 pytestmark = pytest.mark.usefixtures("close_all_instruments")
 
 
 @pytest.fixture
-def q0() -> TransmonElement:
+def q0() -> BasicTransmonElement:
     coordinator = InstrumentCoordinator("ic")
-    q0 = TransmonElement("q0")
-    q0.instrument_coordinator(coordinator.name)
+    q0 = BasicTransmonElement("q0")
 
     # Transmon element is returned
     yield q0
     # after the test, teardown...
     q0.close()
     coordinator.close()
 
 
-def test_qubit_name(q0: TransmonElement):
+def test_qubit_name(q0: BasicTransmonElement):
     assert q0.name == "q0"
 
 
-def test_generate_config(q0: TransmonElement):
+def test_generate_config(q0: BasicTransmonElement):
     # test that setting some values updates the correct values in the configuration
     # set some values
-    q0.ro_pulse_type("SquarePulse")
-    q0.ro_pulse_duration(400e-9)
+    q0.measure.pulse_type("SquarePulse")
+    q0.measure.pulse_duration(400e-9)
 
-    q_cfg = q0.generate_config()
+    quantum_device = QuantumDevice(name="quantum_device")
+    quantum_device.add_element(q0)
+
+    q_cfg = quantum_device.generate_device_config().elements
 
     # assert values in right place in config.
     assert q_cfg["q0"]["measure"].factory_kwargs["pulse_type"] == "SquarePulse"
     assert q_cfg["q0"]["measure"].factory_kwargs["pulse_duration"] == 400e-9
 
     assert q_cfg["q0"]["Rxy"].factory_kwargs["clock"] == "q0.01"
     assert q_cfg["q0"]["Rxy"].gate_info_factory_kwargs == ["theta", "phi"]
 
 
-def test_generate_device_config(q0: TransmonElement):
-    dev_cfg = q0.generate_device_config()
-    assert isinstance(dev_cfg, DeviceCompilationConfig)
-
+def test_generate_device_config(q0: BasicTransmonElement):
+    quantum_device = QuantumDevice(name="quantum_device")
+    quantum_device.add_element(q0)
 
-def test_find_coordinator(q0: TransmonElement):
-    coordinator = q0.instrument_coordinator.get_instr()
-    assert coordinator.name == "ic"
+    dev_cfg = quantum_device.generate_device_config()
+    assert isinstance(dev_cfg, DeviceCompilationConfig)
 
 
 @pytest.fixture
 def dev() -> QuantumDevice:
     dev = QuantumDevice("dev")
     yield dev
     dev.close()
@@ -79,9 +78,9 @@
 
 
 def test_generate_device_config(qb0):
     _ = qb0.generate_device_config()
 
 
 def test_generate_device_config_part_of_device(qb0, dev):
-    dev.add_component(qb0)
+    dev.add_element(qb0)
     _ = dev.generate_device_config()
```

### Comparing `quantify-scheduler-0.8.0/tests/scheduler/helpers/test_schedule.py` & `quantify-scheduler-0.9.0/tests/scheduler/helpers/test_schedule.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 
 from quantify_scheduler import Schedule
 from quantify_scheduler.enums import BinMode
 from quantify_scheduler.helpers.schedule import (
     extract_acquisition_metadata_from_schedule,
     get_acq_info_by_uuid,
     get_acq_uuid,
-    get_operation_end,
     get_operation_start,
+    get_operation_end,
     get_port_timeline,
     get_pulse_info_by_uuid,
     get_pulse_uuid,
     get_schedule_time_offset,
     get_total_duration,
 )
 from quantify_scheduler.helpers.collections import make_hash
@@ -401,22 +401,23 @@
     # Act
     start_empty = get_operation_start(empty_schedule, timeslot_index=0)
 
     start0_x90 = get_operation_start(schedule0, timeslot_index=0)
     start0_measure = get_operation_start(schedule0, timeslot_index=1)
 
     start1_measure = get_operation_start(schedule1, timeslot_index=0)
-    start1_x90 = get_operation_start(schedule0, timeslot_index=1)
+    start1_x90 = get_operation_start(schedule1, timeslot_index=1)
 
     # Assert
     assert start_empty == 0.0
     assert start0_x90 == 0.0
     assert start0_measure == 20e-9
+
     assert start1_measure == 0.0
-    assert start1_x90 == 20e-9
+    assert start1_x90 == 4.2e-07
 
 
 def test_get_operation_end(empty_schedule: Schedule, create_schedule_with_pulse_info):
     # Arrange
     mw_duration = 20e-9
     ro_acquisition_delay = 120e-9
     ro_integration_time = 300e-9
@@ -446,42 +447,41 @@
     assert end0_measure == approx(
         mw_duration + ro_acquisition_delay + ro_integration_time
     )
     assert end1_measure == approx(ro_acquisition_delay + ro_integration_time)
     assert end1_x90 == approx(ro_acquisition_delay + ro_integration_time + mw_duration)
 
 
-def test_get_schedule_time_offset(
-    empty_schedule: Schedule,
-    basic_schedule: Schedule,
-    schedule_with_measurement: Schedule,
+def test_schedule_timing_table(
+    load_example_transmon_config,
     create_schedule_with_pulse_info,
 ):
-    # Arrange
-    _basic_schedule = create_schedule_with_pulse_info(basic_schedule)
-    _schedule_with_measurement = create_schedule_with_pulse_info(
-        schedule_with_measurement
-    )
-    init_duration = 200e-6
+    device_cfg = load_example_transmon_config
 
-    # Act
-    offset0 = get_schedule_time_offset(
-        empty_schedule, get_port_timeline(empty_schedule)
-    )
-    offset1 = get_schedule_time_offset(
-        _basic_schedule, get_port_timeline(_basic_schedule)
-    )
-    offset2 = get_schedule_time_offset(
-        _schedule_with_measurement, get_port_timeline(_schedule_with_measurement)
-    )
+    schedule = Schedule("test_schedule_timing_table")
+    schedule.add(Reset("q0"))
+    schedule.add(X90("q0"))
+    schedule.add(Measure("q0"))
+    schedule = device_compile(schedule, device_cfg)
 
-    # Assert
-    assert offset0 == 0.0
-    assert offset1 == 0.0
-    assert offset2 == init_duration
+    q0 = device_cfg.elements["q0"]
+    X90_duration = q0["Rxy"].factory_kwargs["duration"]
+    measure_acq_delay = q0["measure"].factory_kwargs["acq_delay"]
+    reset_duration = q0["reset"].factory_kwargs["duration"]
+
+    expected_abs_timing = [
+        0.0,
+        reset_duration,
+        reset_duration + X90_duration,
+        reset_duration + X90_duration + measure_acq_delay,
+    ]
+
+    actual_abs_timing = schedule.timing_table.data.abs_time
+
+    assert all(expected_abs_timing == actual_abs_timing)
 
 
 def test_extract_acquisition_metadata_from_schedule(compiled_two_qubit_t1_schedule):
     comp_t1_sched = compiled_two_qubit_t1_schedule
     acq_metadata = extract_acquisition_metadata_from_schedule(comp_t1_sched)
 
     assert acq_metadata.acq_protocol == "ssb_integration_complex"
```

### Comparing `quantify-scheduler-0.8.0/tests/scheduler/helpers/test_waveforms.py` & `quantify-scheduler-0.9.0/tests/scheduler/helpers/test_waveforms.py`

 * *Files identical despite different names*

### Comparing `quantify-scheduler-0.8.0/tests/scheduler/instrument_coordinator/components/test_generic.py` & `quantify-scheduler-0.9.0/tests/scheduler/instrument_coordinator/components/test_generic.py`

 * *Files identical despite different names*

### Comparing `quantify-scheduler-0.8.0/tests/scheduler/instrument_coordinator/components/test_qblox.py` & `quantify-scheduler-0.9.0/tests/scheduler/instrument_coordinator/components/test_qblox.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 # pylint: disable=missing-class-docstring
 # pylint: disable=missing-function-docstring
 # pylint: disable=missing-module-docstring
 # pylint: disable=redefined-outer-name
 # pylint: disable=too-many-arguments
+# pylint: disable=too-many-locals
 # pylint: disable=unused-argument
 
 # Repository: https://gitlab.com/quantify-os/quantify-scheduler
 # Licensed according to the LICENCE file on the main branch
 """Tests for Qblox instrument coordinator components."""
-import inspect
-import json
 import logging
 import tempfile
 from copy import deepcopy
 from operator import countOf
-from pathlib import Path
 from typing import List, Optional
 
 import numpy as np
 import pytest
 from qblox_instruments import (
     Cluster,
     ClusterType,
@@ -28,14 +26,19 @@
     SequencerStatus,
     SequencerStatusFlags,
 )
 
 from quantify_core.data.handling import set_datadir  # pylint: disable=no-name-in-module
 
 from quantify_scheduler.compilation import qcompile
+from quantify_scheduler.device_under_test.mock_setup import (
+    set_standard_params_transmon,
+)
+from quantify_scheduler.device_under_test.quantum_device import QuantumDevice
+from quantify_scheduler.device_under_test.transmon_element import BasicTransmonElement
 from quantify_scheduler.instrument_coordinator.components import qblox
 
 from tests.fixtures.mock_setup import close_instruments
 
 
 @pytest.fixture
 def make_cluster_component(mocker):
@@ -43,49 +46,57 @@
 
     def _make_cluster_component(
         name: str = "cluster0",
         sequencer_status: SequencerStatus = SequencerStatus.ARMED,
         sequencer_flags: Optional[List[SequencerStatusFlags]] = None,
     ) -> qblox.ClusterComponent:
 
-        mocker.patch("qblox_instruments.native.cluster.Cluster.arm_sequencer")
-        mocker.patch("qblox_instruments.native.cluster.Cluster.start_sequencer")
-        mocker.patch("qblox_instruments.native.cluster.Cluster.stop_sequencer")
-
-        close_instruments([name])
+        close_instruments([f"ic_{name}", name])
         cluster = Cluster(
             name=name,
             dummy_cfg={
                 "1": ClusterType.CLUSTER_QCM,
                 "2": ClusterType.CLUSTER_QCM_RF,
                 "3": ClusterType.CLUSTER_QRM,
                 "4": ClusterType.CLUSTER_QRM_RF,
+                "10": ClusterType.CLUSTER_QCM,  # for flux pulsing q0_q3
+                "12": ClusterType.CLUSTER_QCM,  # for flux pulsing q4
             },
         )
         nonlocal cluster_component
         cluster_component = qblox.ClusterComponent(cluster)
 
         mocker.patch.object(cluster, "reference_source", wraps=cluster.reference_source)
 
-        for component in cluster_component._cluster_modules.values():
+        for comp in cluster_component._cluster_modules.values():
+            instrument = comp.instrument_channel
+            mocker.patch.object(
+                instrument, "arm_sequencer", wraps=instrument.arm_sequencer
+            )
+            mocker.patch.object(
+                instrument, "start_sequencer", wraps=instrument.start_sequencer
+            )
             mocker.patch.object(
-                component.instrument_channel,
+                instrument, "stop_sequencer", wraps=instrument.stop_sequencer
+            )
+            mocker.patch.object(
+                instrument,
                 "get_sequencer_state",
                 return_value=SequencerState(
                     sequencer_status, sequencer_flags if sequencer_flags else []
                 ),
             )
 
         return cluster_component
 
     yield _make_cluster_component
 
     if cluster_component:
-        for component in cluster_component._cluster_modules.values():
-            component.close()
+        for comp in cluster_component._cluster_modules.values():
+            comp.close()
         cluster_component.close()
 
 
 @pytest.fixture
 def make_qcm_component(mocker):
     component: qblox.PulsarQCMComponent = None
 
@@ -99,15 +110,15 @@
         mocker.patch("qblox_instruments.native.pulsar.Pulsar.arm_sequencer")
         mocker.patch("qblox_instruments.native.pulsar.Pulsar.start_sequencer")
         mocker.patch("qblox_instruments.native.pulsar.Pulsar.stop_sequencer")
         mocker.patch(
             "qblox_instruments.scpi.pulsar_qcm.PulsarQcm._set_reference_source"
         )
 
-        close_instruments([name])
+        close_instruments([f"ic_{name}", name])
         qcm = Pulsar(name=name, dummy_type=PulsarType.PULSAR_QCM)
         qcm._serial = serial
 
         nonlocal component
         component = qblox.PulsarQCMComponent(qcm)
 
         mocker.patch.object(component.instrument_ref, "get_instr", return_value=qcm)
@@ -146,15 +157,15 @@
             "qblox_instruments.scpi.pulsar_qrm.PulsarQrm._set_reference_source"
         )
         if patch_acquisitions:
             mocker.patch(
                 "qblox_instruments.native.pulsar.Pulsar.store_scope_acquisition"
             )
 
-        close_instruments([name])
+        close_instruments([f"ic_{name}", name])
         qrm = Pulsar(name=name, dummy_type=PulsarType.PULSAR_QRM)
         qrm._serial = serial
 
         nonlocal component
         component = qblox.PulsarQRMComponent(qrm)
 
         mocker.patch.object(component.instrument_ref, "get_instr", return_value=qrm)
@@ -354,116 +365,218 @@
     make_cluster_component("cluster0")
 
 
 @pytest.mark.parametrize(
     "set_reference_source, force_set_parameters",
     [(False, False), (False, True), (True, False), (True, True)],
 )
-def test_prepare(
+def test_prepare_qcm_qrm(
+    mocker,
+    tmp_test_data_dir,
     schedule_with_measurement,
     load_example_transmon_config,
     load_example_qblox_hardware_config,
     make_qcm_component,
     make_qrm_component,
     set_reference_source,
     force_set_parameters,
 ):
     # Arrange
-    qcm: qblox.PulsarQCMComponent = make_qcm_component("qcm0", "1234")
-    qrm: qblox.PulsarQRMComponent = make_qrm_component("qrm0", "1234")
+    qcm0: qblox.PulsarQCMComponent = make_qcm_component("qcm0", "1234")
+    qrm0: qblox.PulsarQRMComponent = make_qrm_component("qrm0", "1234")
+    qrm2: qblox.PulsarQRMComponent = make_qrm_component("qrm2", "1234")
+
+    mocker.patch.object(qcm0.instrument.parameters["out0_offset"], "set")
+    mocker.patch.object(qcm0.instrument.parameters["out1_offset"], "set")
+    mocker.patch.object(qcm0.instrument.parameters["out2_offset"], "set")
+    mocker.patch.object(qcm0.instrument.parameters["out3_offset"], "set")
+
+    mocker.patch.object(qrm0.instrument.parameters["out0_offset"], "set")
+    mocker.patch.object(qrm0.instrument.parameters["out1_offset"], "set")
+    mocker.patch.object(qrm0.instrument.parameters["in0_gain"], "set")
+    mocker.patch.object(qrm0.instrument.parameters["in1_gain"], "set")
+
+    mocker.patch.object(qrm2.instrument.parameters["in0_gain"], "set")
+    mocker.patch.object(qrm2.instrument.parameters["in1_gain"], "set")
 
+    hardware_cfg = load_example_qblox_hardware_config
     if set_reference_source:
-        qcm.instrument.reference_source("internal")
-        qcm.instrument._set_reference_source.reset_mock()
+        qcm0.instrument.reference_source(hardware_cfg[qcm0.instrument.name]["ref"])
+        qcm0.instrument._set_reference_source.reset_mock()
 
-        qrm.instrument.reference_source("external")
-        qrm.instrument._set_reference_source.reset_mock()
+        qrm0.instrument.reference_source(hardware_cfg[qrm0.instrument.name]["ref"])
+        qrm0.instrument._set_reference_source.reset_mock()
 
-    # Act
-    qcm.force_set_parameters(force_set_parameters)
-    qrm.force_set_parameters(force_set_parameters)
+        qrm2.instrument.reference_source(hardware_cfg[qrm2.instrument.name]["ref"])
+        qrm2.instrument._set_reference_source.reset_mock()
 
-    with tempfile.TemporaryDirectory() as tmp_dir:
-        set_datadir(tmp_dir)
+    qcm0.force_set_parameters(force_set_parameters)
+    qrm0.force_set_parameters(force_set_parameters)
+    qrm2.force_set_parameters(force_set_parameters)
 
-        compiled_schedule = qcompile(
-            schedule_with_measurement,
-            load_example_transmon_config,
-            load_example_qblox_hardware_config,
-        )
-        prog = compiled_schedule["compiled_instructions"]
+    # Act
+    set_datadir(tmp_test_data_dir)
 
-        qcm.prepare(prog["qcm0"])
-        qrm.prepare(prog["qrm0"])
+    compiled_schedule = qcompile(
+        schedule_with_measurement,
+        load_example_transmon_config,
+        hardware_cfg,
+    )
+    prog = compiled_schedule["compiled_instructions"]
+
+    qcm0.prepare(prog[qcm0.instrument.name])
+    qrm0.prepare(prog[qrm0.instrument.name])
+    qrm2.prepare(prog[qrm2.instrument.name])
 
     # Assert
-    if not set_reference_source:
-        qcm.instrument.arm_sequencer.assert_called_with(sequencer=0)
-        qrm.instrument.arm_sequencer.assert_called_with(sequencer=0)
-    else:
+    qcm0.instrument.arm_sequencer.assert_called_with(sequencer=1)
+    qrm0.instrument.arm_sequencer.assert_called_with(sequencer=1)
+    qrm2.instrument.arm_sequencer.assert_called_with(sequencer=1)
+
+    if set_reference_source:
         if force_set_parameters:
-            qcm.instrument._set_reference_source.assert_called()
-            qrm.instrument._set_reference_source.assert_called()
+            qcm0.instrument._set_reference_source.assert_called()
+            qrm0.instrument._set_reference_source.assert_called()
+            qrm2.instrument._set_reference_source.assert_called()
         else:
-            qcm.instrument._set_reference_source.assert_not_called()
-            qrm.instrument._set_reference_source.assert_not_called()
+            qcm0.instrument._set_reference_source.assert_not_called()
+            qrm0.instrument._set_reference_source.assert_not_called()
+            qrm2.instrument._set_reference_source.assert_not_called()
+
+    for (qcodes_param, hw_config_param) in [
+        ("out0_offset", ["complex_output_0", "dc_mixer_offset_I"]),
+        ("out1_offset", ["complex_output_0", "dc_mixer_offset_Q"]),
+        ("out2_offset", ["complex_output_1", "dc_mixer_offset_I"]),
+        ("out3_offset", ["complex_output_1", "dc_mixer_offset_Q"]),
+    ]:
+        qcm0.instrument.parameters[qcodes_param].set.assert_any_call(
+            hardware_cfg[qcm0.instrument.name][hw_config_param[0]][hw_config_param[1]]
+        )
+
+    for (qcodes_param, hw_config_param) in [
+        ("out0_offset", ["complex_output_0", "dc_mixer_offset_I"]),
+        ("out1_offset", ["complex_output_0", "dc_mixer_offset_Q"]),
+        ("in0_gain", ["complex_output_0", "input_gain_I"]),
+        ("in1_gain", ["complex_output_0", "input_gain_Q"]),
+    ]:
+        qrm0.instrument.parameters[qcodes_param].set.assert_any_call(
+            hardware_cfg[qrm0.instrument.name][hw_config_param[0]][hw_config_param[1]]
+        )
+
+    for (qcodes_param, hw_config_param) in [
+        ("in0_gain", ["real_output_0", "input_gain"]),
+        ("in1_gain", ["real_output_1", "input_gain"]),
+    ]:
+        qrm2.instrument.parameters[qcodes_param].set.assert_any_call(
+            hardware_cfg[qrm2.instrument.name][hw_config_param[0]][hw_config_param[1]]
+        )
 
 
 @pytest.mark.parametrize("force_set_parameters", [False, True])
-def test_prepare_ref_source_cluster(
+def test_prepare_cluster_rf(
+    mocker,
+    tmp_test_data_dir,
     make_basic_schedule,
-    load_legacy_transmon_config,
     load_example_qblox_hardware_config,
     make_cluster_component,
     force_set_parameters,
 ):
     # Arrange
     cluster_name = "cluster0"
-    cluster: qblox.ClusterComponent = make_cluster_component(cluster_name)
+    ic_cluster: qblox.ClusterComponent = make_cluster_component(cluster_name)
+
+    qcm_rf = ic_cluster.instrument.module2
+    mocker.patch.object(qcm_rf.parameters["out0_att"], "set")
+    mocker.patch.object(qcm_rf.parameters["out1_att"], "set")
+
+    qrm_rf = ic_cluster.instrument.module4
+    mocker.patch.object(qrm_rf.parameters["out0_att"], "set")
+    mocker.patch.object(qrm_rf.parameters["in0_att"], "set")
 
-    cluster.force_set_parameters(force_set_parameters)
-    cluster.instrument.reference_source("internal")  # Put it in a known state
+    ic_cluster.force_set_parameters(force_set_parameters)
+    ic_cluster.instrument.reference_source("internal")  # Put it in a known state
 
-    sched = make_basic_schedule("q4")
+    quantum_device = QuantumDevice(name="quantum_device")
+    q5 = BasicTransmonElement("q5")
+    quantum_device.add_element(q5)
+
+    q5.rxy.amp180(0.213)
+    q5.clock_freqs.f01(6.33e9)
+    q5.clock_freqs.f12(6.09e9)
+    q5.clock_freqs.readout(8.5e9)
+    q5.measure.acq_delay(100e-9)
+
+    sched = make_basic_schedule("q5")
 
     # Act
-    with tempfile.TemporaryDirectory() as tmp_dir:
-        set_datadir(tmp_dir)
+    set_datadir(tmp_test_data_dir)
 
-        compiled_schedule = qcompile(
-            sched, load_legacy_transmon_config, load_example_qblox_hardware_config
-        )
-        compiled_schedule2 = deepcopy(compiled_schedule)
-        prog = compiled_schedule["compiled_instructions"]
+    hardware_cfg = load_example_qblox_hardware_config
+    compiled_schedule = qcompile(
+        sched, quantum_device.generate_device_config(), hardware_cfg
+    )
+    compiled_schedule_before_prepare = deepcopy(compiled_schedule)
 
-        cluster.prepare(prog[cluster_name])
+    prog = compiled_schedule["compiled_instructions"]
+    ic_cluster.prepare(prog[cluster_name])
+
+    # Assert
+    assert compiled_schedule == compiled_schedule_before_prepare
+
+    qcm_rf.arm_sequencer.assert_called_with(sequencer=0)
+    qrm_rf.arm_sequencer.assert_called_with(sequencer=0)
 
     # Assert it's only set in initialization
-    cluster.instrument.reference_source.assert_called_once()
-    assert compiled_schedule == compiled_schedule2
+    ic_cluster.instrument.reference_source.assert_called_once()
+
+    for (qcodes_param, hw_config_param) in [
+        ("out0_att", ["complex_output_0", "output_att"]),
+        ("out1_att", ["complex_output_1", "output_att"]),
+    ]:
+        qcm_rf.parameters[qcodes_param].set.assert_any_call(
+            hardware_cfg[cluster_name][qcm_rf.name][hw_config_param[0]][
+                hw_config_param[1]
+            ]
+        )
+
+    for (qcodes_param, hw_config_param) in [
+        ("out0_att", ["complex_output_0", "output_att"]),
+        ("in0_att", ["complex_output_0", "input_att"]),
+    ]:
+        qrm_rf.parameters[qcodes_param].set.assert_any_call(
+            hardware_cfg[cluster_name][qrm_rf.name][hw_config_param[0]][
+                hw_config_param[1]
+            ]
+        )
 
 
 def test_prepare_rf(
+    close_all_instruments,
+    mock_setup_basic_transmon,
     schedule_with_measurement_q2,
-    load_legacy_transmon_config,
     load_example_qblox_hardware_config,
     make_qcm_rf,
     make_qrm_rf,
 ):
     # Arrange
     qcm: qblox.QCMRFComponent = make_qcm_rf("qcm_rf0", "1234")
     qrm: qblox.QRMRFComponent = make_qrm_rf("qrm_rf0", "1234")
 
+    set_standard_params_transmon(mock_setup_basic_transmon)
+    mock_setup_basic_transmon["q2"].clock_freqs.readout(7.5e9)
+    mock_setup_basic_transmon["q2"].clock_freqs.f01(6.03e9)
+
+    device_config = mock_setup_basic_transmon["quantum_device"].generate_device_config()
     # Act
     with tempfile.TemporaryDirectory() as tmp_dir:
         set_datadir(tmp_dir)
 
         compiled_schedule = qcompile(
             schedule_with_measurement_q2,
-            load_legacy_transmon_config,
+            device_config,
             load_example_qblox_hardware_config,
         )
         prog = compiled_schedule["compiled_instructions"]
 
         qcm.prepare(prog["qcm_rf0"])
         qrm.prepare(prog["qrm_rf0"])
 
@@ -613,28 +726,32 @@
 def test_retrieve_acquisition_qcm_rf(close_all_instruments, make_qcm_rf):
     qcm_rf: qblox.QCMRFComponent = make_qcm_rf("qcm_rf0", "1234")
 
     assert qcm_rf.retrieve_acquisition() is None
 
 
 def test_retrieve_acquisition_qrm_rf(
+    mock_setup_basic_transmon,
     schedule_with_measurement_q2,
-    load_legacy_transmon_config,
     load_example_qblox_hardware_config,
     make_qrm_rf,
 ):
     # Arrange
     qrm_rf: qblox.QRMRFComponent = make_qrm_rf("qrm_rf0", "1234")
 
+    set_standard_params_transmon(mock_setup_basic_transmon)
+    mock_setup_basic_transmon["q2"].clock_freqs.readout(7.3e9)
+    device_config = mock_setup_basic_transmon["quantum_device"].generate_device_config()
+
     # Act
     with tempfile.TemporaryDirectory() as tmp_dir:
         set_datadir(tmp_dir)
         compiled_schedule = qcompile(
             schedule_with_measurement_q2,
-            load_legacy_transmon_config,
+            device_config,
             load_example_qblox_hardware_config,
         )
         prog = compiled_schedule["compiled_instructions"]
         prog = dict(prog)
 
         qrm_rf.prepare(prog[qrm_rf.instrument.name])
         qrm_rf.start()
@@ -642,28 +759,37 @@
 
     # Assert
     assert len(acq[(0, 0)]) == 2
 
 
 def test_retrieve_acquisition_cluster(
     make_schedule_with_measurement,
-    load_legacy_transmon_config,
+    mock_setup_basic_transmon,
     load_example_qblox_hardware_config,
     make_cluster_component,
 ):
+    q4 = mock_setup_basic_transmon["q4"]
+    q4.clock_freqs.f01.set(5040000000)
+    q4.rxy.amp180(0.2)
+    q4.clock_freqs.f12(5.41e9)
+    q4.clock_freqs.readout(6950000000)
+    q4.measure.acq_delay(1.2e-07)
+
+    device_cfg = mock_setup_basic_transmon["quantum_device"].generate_device_config()
+
     # Arrange
     cluster_name = "cluster0"
     cluster: qblox.ClusterComponent = make_cluster_component(cluster_name)
 
     # Act
     with tempfile.TemporaryDirectory() as tmp_dir:
         set_datadir(tmp_dir)
         compiled_schedule = qcompile(
             make_schedule_with_measurement("q4"),
-            load_legacy_transmon_config,
+            device_cfg,
             load_example_qblox_hardware_config,
         )
         prog = compiled_schedule["compiled_instructions"]
         prog = dict(prog)
 
         cluster.prepare(prog[cluster_name])
         cluster.start()
@@ -703,31 +829,37 @@
 
     # Assert
     qcm.instrument.start_sequencer.assert_called()
     qrm.instrument.start_sequencer.assert_called()
 
 
 def test_start_qcm_qrm_rf(
+    mock_setup_basic_transmon,
     schedule_with_measurement_q2,
-    load_legacy_transmon_config,
     load_example_qblox_hardware_config,
     make_qcm_rf,
     make_qrm_rf,
 ):
     # Arrange
     qcm_rf: qblox.QCMRFComponent = make_qcm_rf("qcm_rf0", "1234")
     qrm_rf: qblox.QRMRFComponent = make_qrm_rf("qrm_rf0", "1234")
 
+    set_standard_params_transmon(mock_setup_basic_transmon)
+    mock_setup_basic_transmon["q2"].clock_freqs.readout(7.3e9)
+    mock_setup_basic_transmon["q2"].clock_freqs.f01(6.03e9)
+
+    device_config = mock_setup_basic_transmon["quantum_device"].generate_device_config()
+
     # Act
     with tempfile.TemporaryDirectory() as tmp_dir:
         set_datadir(tmp_dir)
 
         compiled_schedule = qcompile(
             schedule_with_measurement_q2,
-            load_legacy_transmon_config,
+            device_config,
             load_example_qblox_hardware_config,
         )
         prog = compiled_schedule["compiled_instructions"]
 
         qcm_rf.prepare(prog["qcm_rf0"])
         qrm_rf.prepare(prog["qrm_rf0"])
 
@@ -771,15 +903,16 @@
     # Arrange
     cluster: qblox.ClusterComponent = make_cluster_component("cluster0")
 
     # Act
     cluster.stop()
 
     # Assert
-    cluster.instrument.stop_sequencer.assert_called()
+    for comp in cluster._cluster_modules.values():
+        comp.instrument.stop_sequencer.assert_called()
 
 
 # ------------------- _QRMAcquisitionManager -------------------
 def test_qrm_acquisition_manager__init__(make_qrm_component):
     qrm: qblox.PulsarQRMComponent = make_qrm_component("qrm0", "1234")
     qblox._QRMAcquisitionManager(
         qrm, qrm._hardware_properties.number_of_sequencers, dict(), None
@@ -812,15 +945,15 @@
     }
     qrm: qblox.PulsarQRMComponent = make_qrm_component(
         name="qrm0", serial="1234", patch_acquisitions=True
     )
     acq_manager = qblox._QRMAcquisitionManager(
         qrm, qrm._hardware_properties.number_of_sequencers, acq_mapping, None
     )
-    acq_manager.scope_mode_sequencer = "seq0"
+    acq_manager.scope_mode_sequencer = 0
 
     # Act
     acq_manager._store_scope_acquisition()
 
     # Assert
     qrm.instrument.store_scope_acquisition.assert_called_once()
```

### Comparing `quantify-scheduler-0.8.0/tests/scheduler/instrument_coordinator/components/test_zhinst.py` & `quantify-scheduler-0.9.0/tests/scheduler/instrument_coordinator/components/test_zhinst.py`

 * *Files identical despite different names*

### Comparing `quantify-scheduler-0.8.0/tests/scheduler/instrument_coordinator/test_instrument_coordinator.py` & `quantify-scheduler-0.9.0/tests/scheduler/instrument_coordinator/test_instrument_coordinator.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 
 from quantify_scheduler import CompiledSchedule, Schedule
 from quantify_scheduler.instrument_coordinator import (
     InstrumentCoordinator,
     ZIInstrumentCoordinator,
 )
 from quantify_scheduler.instrument_coordinator.components import base as base_component
+from quantify_scheduler.gettables_profiled import ProfiledInstrumentCoordinator
 
 
 class MyICC(base_component.InstrumentCoordinatorComponentBase):
     @property
     def is_running(self):
         pass
 
@@ -377,7 +378,37 @@
     compiled_sched = CompiledSchedule(test_sched)
 
     # assert that the uploaded schedule is retrieved
     instrument_coordinator.prepare(compiled_sched)
     last_sched = instrument_coordinator.last_schedule
 
     assert last_sched == compiled_sched
+
+
+def test_profiled_instrument_coordinator(mock_setup_basic_transmon, dummy_components):
+    component1 = dummy_components.pop(0)
+    test_sched = Schedule(name="test_schedule")
+    args = {"dev0": {"foo": 0}}
+    test_sched["compiled_instructions"] = args
+    compiled_sched = CompiledSchedule(test_sched)
+
+    parent_ic = InstrumentCoordinator("IC")
+    instr_coordinator = ProfiledInstrumentCoordinator("d0", parent_ic)
+    instr_coordinator.add_component(component1)
+    instr_coordinator.prepare(compiled_sched)
+    instr_coordinator.start()
+    instr_coordinator.wait_done()
+    instr_coordinator.retrieve_acquisition()
+    instr_coordinator.stop()
+
+    verif_keys = [
+        "schedule",
+        "prepare",
+        "add_component",
+        "start",
+        "wait_done",
+        "retrieve_acquisition",
+        "stop",
+    ]
+    for key in verif_keys:
+        assert key in instr_coordinator.profile
+        assert (x > 0 for x in instr_coordinator.profile[key])
```

### Comparing `quantify-scheduler-0.8.0/tests/scheduler/instrument_coordinator/test_utility.py` & `quantify-scheduler-0.9.0/tests/scheduler/instrument_coordinator/test_utility.py`

 * *Files 6% similar despite different names*

```diff
@@ -64,14 +64,22 @@
 def test_search_settable_param_fail(mock_instrument, parameter_name):
     with pytest.raises(ValueError):
         utility.search_settable_param(
             instrument=mock_instrument, nested_parameter_name=parameter_name
         )
 
 
+@pytest.mark.parametrize("parameter_name", ["missing.ch_foo.bar"])
+def test_search_settable_param_fail_wrong_nesting(mock_instrument, parameter_name):
+    with pytest.raises(ValueError):
+        utility.search_settable_param(
+            instrument=mock_instrument, nested_parameter_name=parameter_name
+        )
+
+
 class CallCounter:
     def __init__(self, wrap_func):
         self.count: int = 0
         self.wrap_func = wrap_func
 
     def __call__(self, *args, **kwargs):
         self.count += 1
```

### Comparing `quantify-scheduler-0.8.0/tests/scheduler/schedules/compiles_all_backends.py` & `quantify-scheduler-0.9.0/tests/scheduler/schedules/compiles_all_backends.py`

 * *Files identical despite different names*

### Comparing `quantify-scheduler-0.8.0/tests/scheduler/schedules/test_schedule_plotting_matplotlib.py` & `quantify-scheduler-0.9.0/tests/scheduler/schedules/test_schedule_plotting_matplotlib.py`

 * *Files identical despite different names*

### Comparing `quantify-scheduler-0.8.0/tests/scheduler/schedules/test_schedule_sampling.py` & `quantify-scheduler-0.9.0/tests/scheduler/schedules/test_schedule_sampling.py`

 * *Files 6% similar despite different names*

```diff
@@ -48,23 +48,16 @@
     np.testing.assert_array_almost_equal(
         waveforms["T"], np.array([-0.2, -0.2, -0.2, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0])
     )
 
 
 def test_sample_modulated_waveform() -> None:
     schedule = Schedule("test")
-    clock0 = BasebandClockResource(
-        name="clock0",
-        data={
-            "name": "clock0",
-            "type": "BasebandClockResource",
-            "freq": 0.15e9,
-            "phase": 0,
-        },
-    )
+    clock0 = BasebandClockResource("clock0")
+    clock0["freq"] = 0.15e9
     schedule.add_resource(clock0)
 
     square_pulse_op = SquarePulse(amp=0.2, duration=3e-9, port="SDP", clock="clock0")
     schedule.add(square_pulse_op)
     square_pulse_op = SquarePulse(amp=0.2, duration=3e-9, port="T")
     schedule.add(square_pulse_op, ref_pt="start")
     determine_absolute_timing(schedule=schedule)
```

### Comparing `quantify-scheduler-0.8.0/tests/scheduler/schedules/test_spectroscopy_schedules.py` & `quantify-scheduler-0.9.0/tests/scheduler/schedules/test_spectroscopy_schedules.py`

 * *Files identical despite different names*

### Comparing `quantify-scheduler-0.8.0/tests/scheduler/schedules/test_timedomain_schedules.py` & `quantify-scheduler-0.9.0/tests/scheduler/schedules/test_timedomain_schedules.py`

 * *Files identical despite different names*

### Comparing `quantify-scheduler-0.8.0/tests/scheduler/schedules/test_trace_schedules.py` & `quantify-scheduler-0.9.0/tests/scheduler/schedules/test_trace_schedules.py`

 * *Files identical despite different names*

### Comparing `quantify-scheduler-0.8.0/tests/scheduler/test_acquisition_library.py` & `quantify-scheduler-0.9.0/tests/scheduler/test_acquisition_library.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 # Repository: https://gitlab.com/quantify-os/quantify-scheduler
 # Licensed according to the LICENCE file on the main branch
 """Unit tests acquisition protocols for use with the quantify_scheduler."""
 
 # pylint: disable=missing-class-docstring
 # pylint: disable=missing-function-docstring
 # pylint: disable=eval-used
+import json
 from unittest import TestCase
 
 import numpy as np
 import pytest
 
 from quantify_scheduler import Operation
 from quantify_scheduler.enums import BinMode
 from quantify_scheduler.operations.acquisition_library import (
     NumericalWeightedIntegrationComplex,
     SSBIntegrationComplex,
     Trace,
 )
 from quantify_scheduler.operations.gate_library import X90
 from quantify_scheduler.operations.pulse_library import DRAGPulse
+from quantify_scheduler.json_utils import ScheduleJSONEncoder, ScheduleJSONDecoder
 
 
 def test_ssb_integration_complex():
     ssb_acq = SSBIntegrationComplex(
         duration=100e-9,
         port="q0.res",
         clock="q0.01",
@@ -101,15 +103,20 @@
             port="q0:res",
             clock="q0.ro",
             duration=100e-9,
         ),
     ],
 )
 def test__repr__(operation: Operation):
-    assert eval(repr(operation)) == operation
+    # Arrange
+    operation_state: str = json.dumps(operation, cls=ScheduleJSONEncoder)
+
+    # Act
+    obj = json.loads(operation_state, cls=ScheduleJSONDecoder)
+    assert obj == operation
 
 
 @pytest.mark.parametrize(
     "operation",
     [
         Trace(
             duration=16e-9,
@@ -154,18 +161,18 @@
             port="q0:res",
             clock="q0.ro",
         ),
     ],
 )
 def test_deserialize(operation: Operation):
     # Arrange
-    operation_repr: str = repr(operation)
+    operation_state: str = json.dumps(operation, cls=ScheduleJSONEncoder)
 
     # Act
-    obj = eval(operation_repr)
+    obj = json.loads(operation_state, cls=ScheduleJSONDecoder)
 
     # Assert
     if isinstance(operation, NumericalWeightedIntegrationComplex):
         waveforms = operation.data["acquisition_info"][0]["waveforms"]
         for i, waveform in enumerate(waveforms):
             assert isinstance(waveform["t_samples"], (np.generic, np.ndarray))
             assert isinstance(waveform["samples"], (np.generic, np.ndarray))
@@ -203,15 +210,18 @@
             clock="q0.ro",
             duration=100e-9,
         ),
     ],
 )
 def test__repr__modify_not_equal(operation: Operation):
     # Arrange
-    obj = eval(repr(operation))
+    operation_state: str = json.dumps(operation, cls=ScheduleJSONEncoder)
+
+    # Act
+    obj = json.loads(operation_state, cls=ScheduleJSONDecoder)
     assert obj == operation
 
     # Act
     obj.data["acquisition_info"][0]["foo"] = "bar"
 
     # Assert
     assert obj != operation
```

### Comparing `quantify-scheduler-0.8.0/tests/scheduler/test_compilation.py` & `quantify-scheduler-0.9.0/tests/scheduler/test_compilation.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,24 +5,24 @@
 from copy import deepcopy
 
 import numpy as np
 import pytest
 
 from quantify_scheduler import Operation, Schedule
 from quantify_scheduler.compilation import (
-    add_pulse_information_transmon,
     determine_absolute_timing,
     device_compile,
     qcompile,
     validate_config,
 )
 from quantify_scheduler.enums import BinMode
 from quantify_scheduler.operations.gate_library import CNOT, CZ, Measure, Reset, Rxy
 from quantify_scheduler.operations.pulse_library import SquarePulse
 from quantify_scheduler.resources import BasebandClockResource, ClockResource, Resource
+from quantify_scheduler.backends.circuit_to_device import ConfigKeyError
 
 
 def test_determine_absolute_timing_ideal_clock():
     sched = Schedule("Test experiment")
 
     # define the resources
     # q0, q1 = Qubits(n=2) # assumes all to all connectivity
@@ -98,108 +98,101 @@
     sched = Schedule("test")
     q0, q1 = ("q0", "q1")
     ref_label_1 = "test_label"
     with pytest.raises(ValueError):
         sched.add(operation=CNOT(qC=q0, qT=q1), ref_op=ref_label_1)
 
 
-def test_config_spec(load_legacy_transmon_config):
-    validate_config(load_legacy_transmon_config, scheme_fn="transmon_cfg.json")
-
-
-def test_compile_transmon_program(load_legacy_transmon_config):
+def test_compile_transmon_program(load_example_transmon_config):
     sched = Schedule("Test schedule")
 
     # define the resources
     # q0, q1 = Qubits(n=2) # assumes all to all connectivity
     q0, q1 = ("q0", "q1")
     sched.add(Reset(q0, q1))
     sched.add(Rxy(90, 0, qubit=q0))
     sched.add(operation=CZ(qC=q0, qT=q1))
     sched.add(Rxy(theta=90, phi=0, qubit=q0))
     sched.add(Measure(q0, q1), label="M0")
-    # pulse information is added
-    sched = add_pulse_information_transmon(
-        sched, device_cfg=load_legacy_transmon_config
-    )
-    sched = determine_absolute_timing(sched, time_unit="physical")
+    sched = qcompile(sched, device_cfg=load_example_transmon_config)
 
 
-def test_missing_edge(load_legacy_transmon_config):
+def test_missing_edge(load_example_transmon_config):
     sched = Schedule("Bad edge")
-    bad_cfg = load_legacy_transmon_config
-    del bad_cfg["edges"]["q0-q1"]
+    bad_cfg = load_example_transmon_config
+    bad_cfg.edges = {}
 
     q0, q1 = ("q0", "q1")
     sched.add(operation=CZ(qC=q0, qT=q1))
     with pytest.raises(
-        ValueError,
-        match=(
-            "Attempting operation 'CZ' on qubits q1 "
-            "and q0 which lack a connective edge."
-        ),
+        ConfigKeyError,
+        match=('edge "q0_q1" is not present in the configuration file'),
     ):
-        add_pulse_information_transmon(sched, device_cfg=bad_cfg)
+        qcompile(sched, device_cfg=bad_cfg)
 
 
 def test_empty_sched():
     sched = Schedule("empty")
     with pytest.raises(ValueError, match="schedule 'empty' contains no schedulables"):
         determine_absolute_timing(sched)
 
 
-def test_bad_gate(load_legacy_transmon_config):
+def test_bad_gate(load_example_transmon_config):
     class NotAGate(Operation):
         def __init__(self, q):
             plot_func = "quantify_scheduler.visualization.circuit_diagram.cnot"
             data = {
                 "gate_info": {
                     "unitary": np.array(
                         [[1, 1, 1, 1], [1, 1, 1, 1], [1, 1, 1, 1], [1, 1, 1, 1]]
                     ),
                     "tex": r"bad",
                     "plot_func": plot_func,
-                    "qubits": q,
+                    "qubits": [q],
                     "operation_type": "bad",
                 }
             }
-            super().__init__("bad ({})".format(q), data=data)
+            super().__init__("bad ({})".format(q))
+            self.data.update(data)
 
     sched = Schedule("Bell experiment")
     sched.add(Reset("q0"))
     sched.add(NotAGate("q0"))
     with pytest.raises(
-        NotImplementedError, match='Operation type "bad" not supported by backend'
+        ConfigKeyError,
+        match='\'operation "bad" is not present in the configuration file.*',
     ):
-        add_pulse_information_transmon(sched, load_legacy_transmon_config)
+        qcompile(sched, load_example_transmon_config)
 
 
-def test_pulse_and_clock(load_legacy_transmon_config):
+def test_pulse_and_clock(load_example_transmon_config):
     sched = Schedule("pulse_no_clock")
     mystery_clock = "BigBen"
     op_label = sched.add(SquarePulse(0.5, 20e-9, "q0:mw_ch", clock=mystery_clock))
     op_hash = next(
         op for op in sched.schedulables.values() if op["label"] == str(op_label)
     )["operation_repr"]
     with pytest.raises(ValueError) as execinfo:
-        add_pulse_information_transmon(sched, device_cfg=load_legacy_transmon_config)
+        qcompile(sched, device_cfg=load_example_transmon_config)
 
     assert str(execinfo.value) == (
         "Operation '{}' contains an unknown clock '{}'; ensure this resource has "
         "been added to the schedule.".format(op_hash, mystery_clock)
     )
 
     sched.add_resources([ClockResource(mystery_clock, 6e9)])
-    add_pulse_information_transmon(sched, device_cfg=load_legacy_transmon_config)
+    qcompile(sched, device_cfg=load_example_transmon_config)
 
 
 def test_resource_resolution(load_example_transmon_config):
     sched = Schedule("resource_resolution")
-    qcm0_s0 = Resource("qcm0.s0", {"name": "qcm0.s0", "type": "qcm"})
-    qrm0_s0 = Resource("qrm0.s0", {"name": "qrm0.s0", "type": "qrm"})
+    qcm0_s0 = Resource("qcm0.s0")
+    qcm0_s0["type"] = "qcm"
+    qrm0_s0 = Resource("qrm0.s0")
+    qrm0_s0["type"] = "qrm"
 
     sched.add(Rxy(90, 0, "q0"))
     sched.add(SquarePulse(0.6, 20e-9, "q0:mw_ch", clock=BasebandClockResource.IDENTITY))
     sched.add(SquarePulse(0.4, 20e-9, "q0:ro_ch", clock=BasebandClockResource.IDENTITY))
 
     sched.add_resources([qcm0_s0, qrm0_s0])
     sched = qcompile(sched, load_example_transmon_config)
```

### Comparing `quantify-scheduler-0.8.0/tests/scheduler/test_corrections.py` & `quantify-scheduler-0.9.0/tests/scheduler/test_corrections.py`

 * *Files 2% similar despite different names*

```diff
@@ -127,24 +127,24 @@
     [
         (backend, use_numpy)
         for backend in ["quantify_scheduler.backends.qblox_backend.hardware_compile"]
         for use_numpy in [True, False]
     ],
 )
 def test_apply_distortion_corrections(  # pylint: disable=unused-argument disable=too-many-arguments
-    mock_setup,
+    mock_setup_basic_transmon,
     hardware_cfg_distortion_corrections,
     filter_coefficients,
     two_qubit_gate_schedule,
     backend,
     use_numpy_array,
 ):
     compiled_sched = qcompile(
         schedule=two_qubit_gate_schedule,
-        device_cfg=mock_setup["quantum_device"].generate_device_config(),
+        device_cfg=mock_setup_basic_transmon["quantum_device"].generate_device_config(),
         hardware_cfg=hardware_cfg_distortion_corrections,
     )
 
     operations_pretty_repr = "".join(
         f"\noperations:\n  key:  {operation_repr}\n  repr: {repr(operation)}\n"
         for operation_repr, operation in compiled_sched.operations.items()
     )
```

### Comparing `quantify-scheduler-0.8.0/tests/scheduler/test_gettables.py` & `quantify-scheduler-0.9.0/tests/scheduler/test_gettables.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,49 +1,57 @@
 # pylint: disable=missing-function-docstring
 # pylint: disable=missing-class-docstring
 # pylint: disable=missing-module-docstring
 # pylint: disable=too-many-locals
 # pylint: disable=invalid-name
+# pylint: disable=unused-argument
 
 # Repository: https://gitlab.com/quantify-os/quantify-scheduler
 # Licensed according to the LICENCE file on the main branch
 
 from typing import Any, Dict, Tuple
+from unittest import TestCase
 
 import json
+import os
 import zipfile
 
 import numpy as np
 import pytest
 from qcodes.instrument.parameter import ManualParameter
 
 from quantify_scheduler.compilation import qcompile
+from quantify_scheduler.device_under_test.mock_setup import set_standard_params_transmon
 from quantify_scheduler.enums import BinMode
 from quantify_scheduler.gettables import ScheduleGettable
+from quantify_scheduler.gettables_profiled import ProfiledScheduleGettable
 from quantify_scheduler.helpers.schedule import (
     extract_acquisition_metadata_from_schedule,
 )
 
 from quantify_scheduler.instrument_coordinator.components.qblox import (
     AcquisitionIndexing,
 )
 from quantify_scheduler.schedules.schedule import AcquisitionMetadata, Schedule
 from quantify_scheduler.schedules.spectroscopy_schedules import heterodyne_spec_sched
 from quantify_scheduler.schedules.timedomain_schedules import (
     allxy_sched,
+    rabi_sched,
     readout_calibration_sched,
     t1_sched,
 )
 from quantify_scheduler.schedules.trace_schedules import trace_schedule
 
 
 @pytest.mark.parametrize("num_channels, real_imag", [(1, True), (2, False), (10, True)])
-def test_process_acquired_data(mock_setup, num_channels: int, real_imag: bool):
+def test_process_acquired_data(
+    mock_setup_basic_transmon, num_channels: int, real_imag: bool
+):
     # arrange
-    quantum_device = mock_setup["quantum_device"]
+    quantum_device = mock_setup_basic_transmon["quantum_device"]
     acq_metadata = AcquisitionMetadata(
         acq_protocol="ssb_integration_complex",
         bin_mode=BinMode.AVERAGE,
         acq_return_type=complex,
         acq_indices={i: [0] for i in range(num_channels)},
     )
     mock_data = {AcquisitionIndexing(i, 0): (4815, 162342) for i in range(num_channels)}
@@ -59,32 +67,34 @@
         mock_data, acq_metadata, repetitions=10
     )
 
     # assert
     assert len(processed_data) == 2 * num_channels
 
 
-def test_ScheduleGettableSingleChannel_iterative_heterodyne_spec(mock_setup, mocker):
-    meas_ctrl = mock_setup["meas_ctrl"]
-    quantum_device = mock_setup["quantum_device"]
+def test_ScheduleGettableSingleChannel_iterative_heterodyne_spec(
+    mock_setup_basic_transmon, mocker
+):
+    meas_ctrl = mock_setup_basic_transmon["meas_ctrl"]
+    quantum_device = mock_setup_basic_transmon["quantum_device"]
 
-    qubit = quantum_device.get_component("q0")
+    qubit = quantum_device.get_element("q0")
 
     # manual parameter for testing purposes
     ro_freq = ManualParameter("ro_freq", initial_value=5e9, unit="Hz")
 
     schedule_kwargs = {
-        "pulse_amp": qubit.ro_pulse_amp,
-        "pulse_duration": qubit.ro_pulse_duration,
+        "pulse_amp": qubit.measure.pulse_amp(),
+        "pulse_duration": qubit.measure.pulse_duration(),
         "frequency": ro_freq,
-        "acquisition_delay": qubit.ro_acq_delay,
-        "integration_time": qubit.ro_acq_integration_time,
-        "port": qubit.ro_port,
-        "clock": qubit.ro_clock,
-        "init_duration": qubit.init_duration,
+        "acquisition_delay": qubit.measure.acq_delay(),
+        "integration_time": qubit.measure.integration_time(),
+        "port": qubit.ports.readout(),
+        "clock": qubit.name + ".ro",
+        "init_duration": qubit.reset.duration(),
     }
 
     # Prepare the mock data the spectroscopy schedule
 
     acq_metadata = AcquisitionMetadata(
         acq_protocol="ssb_integration_complex",
         bin_mode=BinMode.AVERAGE,
@@ -93,15 +103,15 @@
     )
 
     data = 1 * np.exp(1j * np.deg2rad(45))
 
     acq_indices_data = _reshape_array_into_acq_return_type(data, acq_metadata)
 
     mocker.patch.object(
-        mock_setup["instrument_coordinator"],
+        mock_setup_basic_transmon["instrument_coordinator"],
         "retrieve_acquisition",
         return_value=acq_indices_data,
     )
 
     # Configure the gettable
     spec_gettable = ScheduleGettable(
         quantum_device=quantum_device,
@@ -123,19 +133,19 @@
     # Assert that the data is coming out correctly.
     np.testing.assert_array_equal(dset.x0, freqs)
     np.testing.assert_array_equal(dset.y0, abs(exp_data))
     np.testing.assert_array_equal(dset.y1, np.angle(exp_data, deg=True))
 
 
 # test a batched case
-def test_ScheduleGettableSingleChannel_batched_allxy(mock_setup, mocker):
-    meas_ctrl = mock_setup["meas_ctrl"]
-    quantum_device = mock_setup["quantum_device"]
+def test_ScheduleGettableSingleChannel_batched_allxy(mock_setup_basic_transmon, mocker):
+    meas_ctrl = mock_setup_basic_transmon["meas_ctrl"]
+    quantum_device = mock_setup_basic_transmon["quantum_device"]
 
-    qubit = quantum_device.get_component("q0")
+    qubit = quantum_device.get_element("q0")
 
     index_par = ManualParameter("index", initial_value=0, unit="#")
     index_par.batched = True
 
     sched_kwargs = {
         "element_select_idx": index_par,
         "qubit": qubit.name,
@@ -153,15 +163,15 @@
     ) * np.exp(1j * np.deg2rad(45))
 
     acq_indices_data = _reshape_array_into_acq_return_type(
         data, extract_acquisition_metadata_from_schedule(comp_allxy_sched)
     )
 
     mocker.patch.object(
-        mock_setup["instrument_coordinator"],
+        mock_setup_basic_transmon["instrument_coordinator"],
         "retrieve_acquisition",
         return_value=acq_indices_data,
     )
 
     # Configure the gettable
 
     allxy_gettable = ScheduleGettable(
@@ -181,20 +191,22 @@
 
     # Assert that the data is coming out correctly.
     np.testing.assert_array_equal(dset.x0, indices)
     np.testing.assert_array_equal(dset.y0 + 1j * dset.y1, data)
 
 
 # test a batched case
-def test_ScheduleGettableSingleChannel_append_readout_cal(mock_setup, mocker):
-    meas_ctrl = mock_setup["meas_ctrl"]
-    quantum_device = mock_setup["quantum_device"]
+def test_ScheduleGettableSingleChannel_append_readout_cal(
+    mock_setup_basic_transmon, mocker
+):
+    meas_ctrl = mock_setup_basic_transmon["meas_ctrl"]
+    quantum_device = mock_setup_basic_transmon["quantum_device"]
 
     repetitions = 256
-    qubit = quantum_device.get_component("q0")
+    qubit = quantum_device.get_element("q0")
 
     prep_state = ManualParameter("prep_state", label="Prepared qubit state", unit="")
     prep_state.batched = True
 
     # extra repetition index will not be required after the new data format
     repetition_par = ManualParameter("repetition", label="Repetition", unit="#")
     repetition_par.batched = True
@@ -213,15 +225,15 @@
     data = np.tile(np.arange(2), repetitions) * np.exp(1j)
 
     acq_indices_data = _reshape_array_into_acq_return_type(
         data, extract_acquisition_metadata_from_schedule(comp_ssro_sched)
     )
 
     mocker.patch.object(
-        mock_setup["instrument_coordinator"],
+        mock_setup_basic_transmon["instrument_coordinator"],
         "retrieve_acquisition",
         return_value=acq_indices_data,
     )
 
     # Configure the gettable
 
     ssro_gettable = ScheduleGettable(
@@ -242,54 +254,56 @@
     # Assert that the data is coming out correctly.
     np.testing.assert_array_equal(dset.x0, np.tile(np.arange(2), repetitions))
     np.testing.assert_array_equal(dset.x1, np.repeat(np.arange(repetitions), 2))
 
     np.testing.assert_array_equal(dset.y0 + 1j * dset.y1, data)
 
 
-def test_ScheduleGettableSingleChannel_trace_acquisition(mock_setup, mocker):
-    meas_ctrl = mock_setup["meas_ctrl"]
-    quantum_device = mock_setup["quantum_device"]
+def test_ScheduleGettableSingleChannel_trace_acquisition(
+    mock_setup_basic_transmon, mocker
+):
+    meas_ctrl = mock_setup_basic_transmon["meas_ctrl"]
+    quantum_device = mock_setup_basic_transmon["quantum_device"]
     # q0 is a  device element from the test setup has all the right params
-    device_element = quantum_device.get_component("q0")
+    device_element = quantum_device.get_element("q0")
 
     sample_par = ManualParameter("sample", label="Sample time", unit="s")
     sample_par.batched = True
 
     schedule_kwargs = {
-        "pulse_amp": device_element.ro_pulse_amp,
-        "pulse_duration": device_element.ro_pulse_duration,
-        "pulse_delay": device_element.ro_pulse_delay,
-        "frequency": device_element.ro_freq,
-        "acquisition_delay": device_element.ro_acq_delay,
-        "integration_time": device_element.ro_acq_integration_time,
-        "port": device_element.ro_port,
-        "clock": device_element.ro_clock,
-        "init_duration": device_element.init_duration,
+        "pulse_amp": device_element.measure.pulse_amp(),
+        "pulse_duration": device_element.measure.pulse_duration(),
+        "pulse_delay": 2e-9,
+        "frequency": device_element.clock_freqs.readout(),
+        "acquisition_delay": device_element.measure.acq_delay(),
+        "integration_time": device_element.measure.integration_time(),
+        "port": device_element.ports.readout(),
+        "clock": device_element.name + ".ro",
+        "init_duration": device_element.reset.duration(),
     }
 
     sched_gettable = ScheduleGettable(
         quantum_device=quantum_device,
         schedule_function=trace_schedule,
         schedule_kwargs=schedule_kwargs,
         batched=True,
     )
 
-    sample_times = np.arange(0, device_element.ro_acq_integration_time(), 1 / 1e9)
+    sample_times = np.arange(0, device_element.measure.integration_time(), 1 / 1e9)
     exp_trace = np.ones(len(sample_times)) * np.exp(1j * np.deg2rad(35))
 
     exp_data = {
         AcquisitionIndexing(acq_channel=0, acq_index=0): (
             exp_trace.real,
             exp_trace.imag,
         )
     }
 
     mocker.patch.object(
-        mock_setup["instrument_coordinator"],
+        mock_setup_basic_transmon["instrument_coordinator"],
         "retrieve_acquisition",
         return_value=exp_data,
     )
 
     # Executing the experiment
     meas_ctrl.settables(sample_par)
     meas_ctrl.setpoints(sample_times)
@@ -299,32 +313,32 @@
 
     # Assert that the data is coming out correctly.
     np.testing.assert_array_equal(dset.x0, sample_times)
     np.testing.assert_array_equal(dset.y0, exp_trace.real)
     np.testing.assert_array_equal(dset.y1, exp_trace.imag)
 
 
-def test_ScheduleGettable_generate_diagnostic(mock_setup, mocker):
+def test_ScheduleGettable_generate_diagnostic(mock_setup_basic_transmon, mocker):
     schedule_kwargs = {"times": np.linspace(1e-6, 50e-6, 50), "qubit": "q0"}
-    quantum_device = mock_setup["quantum_device"]
+    quantum_device = mock_setup_basic_transmon["quantum_device"]
 
     # Prepare the mock data the t1 schedule
     acq_metadata = AcquisitionMetadata(
         acq_protocol="ssb_integration_complex",
         bin_mode=BinMode.AVERAGE,
         acq_return_type=complex,
         acq_indices={0: range(50)},
     )
 
     data = np.ones(50) * np.exp(1j * np.deg2rad(45))
 
     acq_indices_data = _reshape_array_into_acq_return_type(data, acq_metadata)
 
     mocker.patch.object(
-        mock_setup["instrument_coordinator"],
+        mock_setup_basic_transmon["instrument_coordinator"],
         "retrieve_acquisition",
         return_value=acq_indices_data,
     )
 
     # Configure the gettable
     gettable = ScheduleGettable(
         quantum_device=quantum_device,
@@ -345,15 +359,20 @@
     with zipfile.ZipFile(filename, mode="r") as zf:
         dev_cfg = json.loads(zf.read("device_cfg.json").decode())
         hw_cfg = json.loads(zf.read("hardware_cfg.json").decode())
         get_cfg = json.loads(zf.read("gettable.json").decode())
         sched = Schedule.from_json(zf.read("schedule.json").decode())
         snap = json.loads(zf.read("snapshot.json").decode())
 
-    assert snap["instruments"]["q0"]["parameters"]["init_duration"]["value"] == 0.0002
+    assert (
+        snap["instruments"]["q0"]["submodules"]["reset"]["parameters"]["duration"][
+            "value"
+        ]
+        == 0.0002
+    )
     assert gettable.quantum_device.cfg_sched_repetitions() == get_cfg["repetitions"]
     assert gettable._compiled_schedule == qcompile(
         sched, device_cfg=dev_cfg, hardware_cfg=hw_cfg
     )
 
 
 # this is probably useful somewhere, it illustrates the reshaping in the
@@ -398,7 +417,67 @@
                     AcquisitionIndexing(acq_channel, acq_index): (
                         data[acq_channel, acq_index].real,
                         data[acq_channel, acq_index].imag,
                     )
                 }
                 acquisitions.update(acqs)
     return acquisitions
+
+
+def test_profiling(mock_setup_basic_transmon, tmp_test_data_dir):
+    set_standard_params_transmon(mock_setup_basic_transmon)
+    quantum_device = mock_setup_basic_transmon["quantum_device"]
+    qubit = mock_setup_basic_transmon["q0"]
+
+    schedule_kwargs = {
+        "pulse_amp": qubit.measure.pulse_amp(),
+        "pulse_duration": qubit.measure.pulse_duration(),
+        "frequency": qubit.clock_freqs.readout(),
+        "qubit": "q0",
+    }
+    prof_gettable = ProfiledScheduleGettable(
+        quantum_device=quantum_device,
+        schedule_function=rabi_sched,
+        schedule_kwargs=schedule_kwargs,
+    )
+
+    prof_gettable.initialize()
+    instr_coordinator = (
+        prof_gettable.quantum_device.instr_instrument_coordinator.get_instr()
+    )
+    instr_coordinator.start()
+    instr_coordinator.wait_done()
+    instr_coordinator.retrieve_acquisition()
+    instr_coordinator.stop()
+    prof_gettable.close()
+
+    # Test if all steps have been measured and have a value > 0
+    log = prof_gettable.log_profile()
+    TestCase().assertAlmostEqual(log["schedule"][0], 0.2062336)
+    verif_keys = [
+        "schedule",
+        "_compile",
+        "prepare",
+        "start",
+        "wait_done",
+        "retrieve_acquisition",
+        "stop",
+    ]
+    for key in verif_keys:
+        assert len(log[key]) > 0
+        assert [value > 0 for value in log[key]]
+
+    # Test logging to json
+    obj = {"test": ["test"]}
+    path = tmp_test_data_dir
+    filename = "test"
+    prof_gettable.log_profile(
+        obj=obj, path=path, filename=filename, indent=4, separators=(",", ": ")
+    )
+    assert os.path.getsize(os.path.join(path, filename)) > 0
+
+    # Test plot function
+    path = tmp_test_data_dir
+    filename = "average_runtimes.pdf"
+    prof_gettable.plot_profile(path=path)
+    assert prof_gettable.plot is not None
+    assert os.path.getsize(os.path.join(path, filename)) > 0
```

### Comparing `quantify-scheduler-0.8.0/tests/scheduler/test_json_utils.py` & `quantify-scheduler-0.9.0/tests/scheduler/test_json_utils.py`

 * *Files identical despite different names*

### Comparing `quantify-scheduler-0.8.0/tests/scheduler/test_pulse_library.py` & `quantify-scheduler-0.9.0/tests/scheduler/test_pulse_library.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 # pylint: disable=missing-module-docstring
 # pylint: disable=missing-class-docstring
 # pylint: disable=missing-function-docstring
 # pylint: disable=eval-used
 from unittest import TestCase
 
+import json
 import pytest
 
 import numpy as np
 from quantify_scheduler import Operation, Schedule
+from quantify_scheduler.json_utils import ScheduleJSONDecoder, ScheduleJSONEncoder
 from quantify_scheduler.operations.gate_library import X90, X
 from quantify_scheduler.operations.pulse_library import (
     DRAGPulse,
     IdlePulse,
     ShiftClockPhase,
     RampPulse,
     SoftSquarePulse,
@@ -199,15 +201,20 @@
         NumericalPulse(
             np.linspace(0, 1, 1000), np.linspace(0, 20e-6, 1000), "q0:mw", "q0.01"
         ),
         DRAGPulse(0.8, 0.83, 1.0, "q0:mw", 16e-9, "q0.01", 0),
     ],
 )
 def test__repr__(operation: Operation) -> None:
-    assert eval(repr(operation)) == operation
+    # Arrange
+    operation_state: str = json.dumps(operation, cls=ScheduleJSONEncoder)
+
+    # Act
+    obj = json.loads(operation_state, cls=ScheduleJSONDecoder)
+    assert obj == operation
 
 
 @pytest.mark.parametrize(
     "operation",
     [
         IdlePulse(16e-9),
         ShiftClockPhase(clock="q0.01", phase=180.0),
@@ -236,18 +243,18 @@
             np.linspace(0, 1, 1000), np.linspace(0, 20e-6, 1000), "q0:mw", "q0.01"
         ),
         DRAGPulse(0.8, 0.83, 1.0, "q0:mw", 16e-9, "q0.01", 0),
     ],
 )
 def test_deserialize(operation: Operation) -> None:
     # Arrange
-    operation_repr: str = repr(operation)
+    operation_state: str = json.dumps(operation, cls=ScheduleJSONEncoder)
 
     # Act
-    obj = eval(operation_repr)
+    obj = json.loads(operation_state, cls=ScheduleJSONDecoder)
 
     # Assert
     TestCase().assertDictEqual(obj.data, operation.data)
 
 
 @pytest.mark.parametrize(
     "operation",
@@ -261,15 +268,19 @@
             np.linspace(0, 1, 1000), np.linspace(0, 20e-6, 1000), "q0:mw", "q0.01"
         ),
         DRAGPulse(0.8, 0.83, 1.0, "q0:mw", 16e-9, "q0.01", 0),
     ],
 )
 def test__repr__modify_not_equal(operation: Operation) -> None:
     # Arrange
-    obj = eval(repr(operation))
+    # Arrange
+    operation_state: str = json.dumps(operation, cls=ScheduleJSONEncoder)
+
+    # Act
+    obj = json.loads(operation_state, cls=ScheduleJSONDecoder)
     assert obj == operation
 
     # Act
     obj.data["pulse_info"][0]["foo"] = "bar"
 
     # Assert
     assert obj != operation
```

### Comparing `quantify-scheduler-0.8.0/tests/scheduler/test_resources.py` & `quantify-scheduler-0.9.0/tests/scheduler/test_resources.py`

 * *Files identical despite different names*

### Comparing `quantify-scheduler-0.8.0/tests/scheduler/test_structure.py` & `quantify-scheduler-0.9.0/tests/scheduler/test_structure.py`

 * *Files identical despite different names*

### Comparing `quantify-scheduler-0.8.0/tests/scheduler/test_types.py` & `quantify-scheduler-0.9.0/tests/scheduler/test_types.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 import numpy as np
 import pandas as pd
 import pytest
 from quantify_core.data.handling import set_datadir
 
 from quantify_scheduler import enums, json_utils, Operation
+from quantify_scheduler.json_utils import ScheduleJSONDecoder
 from quantify_scheduler.schedules.schedule import (
     AcquisitionMetadata,
     CompiledSchedule,
     Schedule,
 )
 from quantify_scheduler.compilation import qcompile
 from quantify_scheduler.operations.acquisition_library import SSBIntegrationComplex
@@ -212,16 +213,18 @@
     assert empty_x_gate.duration == 0
     assert pulse.duration == square_pulse_duration
     assert x_gate.duration == square_pulse_duration
     assert measure.duration == acquisition_duration
 
 
 def test___repr__():
-    operation = Operation("test", {"gate_info": {"clock": "q0.01"}})
-    assert eval(repr(operation)) == operation
+    operation = Operation("test")
+    operation["gate_info"] = {"clock": "q0.01"}
+    obj = ScheduleJSONDecoder().decode_dict(operation.__getstate__())
+    assert obj == operation
 
 
 def test___str__():
     operation = Operation("test")
     assert eval(str(operation)) == operation
 
 
@@ -245,15 +248,14 @@
     result = Schedule.from_json(json_data)
 
     # Assert
     assert schedule == result
     assert schedule.data == result.data
 
 
-@pytest.mark.xfail(reason="json serialization issue for schedules", strict=True)
 def test_spec_schedule_from_json():
     # Arrange
     schedule = heterodyne_spec_sched(
         0.1, 0.1, 6e9, 1e-7, 1e-6, "q0:mw", "q0.01", 200e-6, 1024
     )
 
     # Act
@@ -286,28 +288,28 @@
 
 
 def test_t1_sched_circuit_diagram(t1_schedule):
     """
     Tests that the test schedule can be visualized
     """
     # will only test that a figure is created and runs without errors
-    _ = t1_schedule.plot_circuit_diagram_mpl()
+    _ = t1_schedule.plot_circuit_diagram()
 
 
 def test_t1_sched_pulse_diagram(t1_schedule, tmp_test_data_dir):
     """
     Tests that the test schedule can be visualized
     """
 
     set_datadir(tmp_test_data_dir)
     device_cfg = load_json_example_scheme("transmon_test_config.json")
     comp_sched = qcompile(t1_schedule, device_cfg=device_cfg)
 
     # will only test that a figure is created and runs without errors
-    _ = comp_sched.plot_pulse_diagram_mpl()
+    _ = comp_sched.plot_pulse_diagram()
 
 
 def test_sched_timing_table(tmp_test_data_dir):
 
     schedule = Schedule(name="test_sched", repetitions=10)
     qubit = "q0"
     times = [0, 10e-6, 30e-6]
@@ -435,27 +437,7 @@
     # Test that json serialization works correctly
     serialized = json.dumps(metadata, cls=json_utils.ScheduleJSONEncoder)
     # Test that json deserialization works correctly
     metadata_copy = json.loads(serialized, cls=json_utils.ScheduleJSONDecoder)
     assert metadata_copy == metadata
     assert isinstance(metadata_copy.bin_mode, enums.BinMode)
     assert isinstance(metadata_copy.acq_return_type, type)
-
-    # An unknown return type should raise an error
-    metadata2 = AcquisitionMetadata(
-        acq_protocol="ssb_integration_complex",
-        bin_mode=enums.BinMode.AVERAGE,
-        acq_return_type=type,
-        acq_indices={0: [0]},
-    )
-    with pytest.raises(ValueError):
-        copy.copy(metadata2)
-
-    # An unknown binmode type should raise an error
-    metadata3 = AcquisitionMetadata(
-        acq_protocol="ssb_integration_complex",
-        bin_mode="forget",
-        acq_return_type=complex,
-        acq_indices={0: [0]},
-    )
-    with pytest.raises(ValueError):
-        copy.copy(metadata3)
```

### Comparing `quantify-scheduler-0.8.0/tests/scheduler/test_waveforms.py` & `quantify-scheduler-0.9.0/tests/scheduler/test_waveforms.py`

 * *Files identical despite different names*

### Comparing `quantify-scheduler-0.8.0/tests/scheduler/visualization/test_circuit_diagram.py` & `quantify-scheduler-0.9.0/tests/scheduler/visualization/test_circuit_diagram.py`

 * *Files identical despite different names*

### Comparing `quantify-scheduler-0.8.0/tests/scheduler/visualization/test_pulse_diagram.py` & `quantify-scheduler-0.9.0/tests/scheduler/visualization/test_pulse_diagram.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,36 +1,27 @@
 # pylint: disable=missing-module-docstring
 # pylint: disable=missing-class-docstring
 # pylint: disable=missing-function-docstring
 
-import inspect
-import json
-from pathlib import Path
-
-import quantify_scheduler.schemas.examples as es
 import quantify_scheduler.visualization.pulse_diagram as plsd
 from quantify_scheduler import Schedule
 from quantify_scheduler.compilation import qcompile
 from quantify_scheduler.operations.gate_library import Measure, Reset, Rxy
 
-esp = inspect.getfile(es)
-cfg_f = Path(esp).parent / "transmon_test_config.json"
-with open(cfg_f, "r") as f:
-    DEVICE_CFG = json.load(f)
-
 # Proper verification of this, probably requires some horrible selenium malarkey
-def test_pulse_diagram_plotly() -> None:
+def test_pulse_diagram_plotly(load_example_transmon_config) -> None:
+    device_cfg = load_example_transmon_config
     sched = Schedule("Test schedule")
 
     # define the resources
     qubit_0, qubit_1 = ("q0", "q1")
     sched.add(Reset(qubit_0, qubit_1))
     sched.add(Rxy(90, 0, qubit=qubit_0))
     # sched.add(operation=CZ(qC=qubit_0, qT=qubit_1)) # not implemented in config
     sched.add(Rxy(theta=90, phi=0, qubit=qubit_0))
     sched.add(Measure(qubit_0, qubit_1), label="M0")
     # pulse information is added
-    compiled_sched = qcompile(sched, DEVICE_CFG, None)
+    compiled_sched = qcompile(sched, device_cfg, None)
     # It should be possible to generate this visualization after compilation
     fig = plsd.pulse_diagram_plotly(compiled_sched)
 
     assert fig.data
```

### Comparing `quantify-scheduler-0.8.0/tests/scheduler/visualization/test_pulse_scheme.py` & `quantify-scheduler-0.9.0/tests/scheduler/visualization/test_pulse_scheme.py`

 * *Files identical despite different names*

### Comparing `quantify-scheduler-0.8.0/tests/test_headers_and_copyright.py` & `quantify-scheduler-0.9.0/tests/test_headers_and_copyright.py`

 * *Files identical despite different names*

