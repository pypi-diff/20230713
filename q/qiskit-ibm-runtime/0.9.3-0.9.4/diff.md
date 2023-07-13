# Comparing `tmp/qiskit-ibm-runtime-0.9.3.tar.gz` & `tmp/qiskit-ibm-runtime-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qiskit-ibm-runtime-0.9.3.tar", last modified: Thu Apr 13 17:22:39 2023, max compression
+gzip compressed data, was "qiskit-ibm-runtime-0.9.4.tar", last modified: Thu May  4 20:43:16 2023, max compression
```

## Comparing `qiskit-ibm-runtime-0.9.3.tar` & `qiskit-ibm-runtime-0.9.4.tar`

### file list

```diff
@@ -1,172 +1,172 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:22:39.164676 qiskit-ibm-runtime-0.9.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11416 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    12913 2023-04-13 17:22:39.164676 qiskit-ibm-runtime-0.9.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11687 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:22:39.144676 qiskit-ibm-runtime-0.9.3/program_source/
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/program_source/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:22:39.144676 qiskit-ibm-runtime-0.9.3/program_source/circuit_runner/
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/program_source/circuit_runner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/program_source/circuit_runner/circuit_runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:22:39.144676 qiskit-ibm-runtime-0.9.3/program_source/hello_world/
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/program_source/hello_world/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/program_source/hello_world/hello_world.py
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/program_source/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:22:39.144676 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/VERSION.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8939 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:22:39.148676 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/accounts/
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/accounts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7433 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/accounts/account.py
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/accounts/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    10826 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/accounts/management.py
--rw-r--r--   0 runner    (1001) docker     (123)     3293 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/accounts/storage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:22:39.148676 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/api/
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/api/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     2763 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/api/client_parameters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:22:39.148676 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/api/clients/
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/api/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6235 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/api/clients/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/api/clients/backend.py
--rw-r--r--   0 runner    (1001) docker     (123)    10203 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/api/clients/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    12679 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/api/clients/runtime.py
--rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/api/clients/runtime_ws.py
--rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/api/clients/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/api/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:22:39.148676 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/api/rest/
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/api/rest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4292 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/api/rest/backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/api/rest/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/api/rest/cloud_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/api/rest/program.py
--rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/api/rest/program_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/api/rest/root.py
--rw-r--r--   0 runner    (1001) docker     (123)     9621 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/api/rest/runtime.py
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/api/rest/runtime_session.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:22:39.152676 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/api/rest/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/api/rest/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/api/rest/utils/data_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    15526 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/api/session.py
--rw-r--r--   0 runner    (1001) docker     (123)     4176 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/backendreservation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    17990 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/estimator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3225 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/hub_group_project.py
--rw-r--r--   0 runner    (1001) docker     (123)    23941 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/ibm_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/ibm_qubit_properties.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:22:39.152676 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/options/
--rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/options/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/options/environment_options.py
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/options/execution_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     9023 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/options/options.py
--rw-r--r--   0 runner    (1001) docker     (123)     3672 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/options/resilience_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/options/simulator_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/options/transpilation_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/options/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:22:39.152676 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/program/
--rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/program/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/program/program_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/program/program_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/program/result_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/program/user_messenger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:22:39.152676 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/proxies/
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/proxies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4684 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/proxies/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)    63935 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/qiskit_runtime_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:22:39.152676 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/qpy/
--rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/qpy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:22:39.156676 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/qpy/binary_io/
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/qpy/binary_io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    38998 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/qpy/binary_io/circuits.py
--rw-r--r--   0 runner    (1001) docker     (123)    16213 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/qpy/binary_io/schedules.py
--rw-r--r--   0 runner    (1001) docker     (123)    12505 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/qpy/binary_io/value.py
--rw-r--r--   0 runner    (1001) docker     (123)    10830 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/qpy/common.py
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/qpy/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7833 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/qpy/formats.py
--rw-r--r--   0 runner    (1001) docker     (123)     9707 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/qpy/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    11718 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/qpy/type_keys.py
--rw-r--r--   0 runner    (1001) docker     (123)    22526 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/runtime_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     4864 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/runtime_options.py
--rw-r--r--   0 runner    (1001) docker     (123)    15441 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/runtime_program.py
--rw-r--r--   0 runner    (1001) docker     (123)     4834 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/runtime_session.py
--rw-r--r--   0 runner    (1001) docker     (123)    15607 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)    10374 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/session.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:22:39.156676 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6837 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/utils/backend_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5318 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/utils/backend_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     5262 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/utils/converters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/utils/deprecation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/utils/estimator_result_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/utils/hgp.py
--rw-r--r--   0 runner    (1001) docker     (123)    11267 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/utils/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/utils/runner_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/utils/sampler_result_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)    11350 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:22:39.144676 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12913 2023-04-13 17:22:39.000000 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5280 2023-04-13 17:22:39.000000 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 17:22:39.000000 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 17:22:39.000000 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-04-13 17:22:39.000000 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-13 17:22:39.000000 qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-04-13 17:22:39.164676 qiskit-ibm-runtime-0.9.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:22:39.156676 qiskit-ibm-runtime-0.9.3/test/
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5756 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/test/account.py
--rw-r--r--   0 runner    (1001) docker     (123)     5069 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/test/decorators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:22:39.156676 qiskit-ibm-runtime-0.9.3/test/e2e/
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/test/e2e/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3270 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/test/e2e/test_tutorials.py
--rw-r--r--   0 runner    (1001) docker     (123)     7553 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/test/ibm_test_case.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:22:39.160676 qiskit-ibm-runtime-0.9.3/test/integration/
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/test/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/test/integration/test_account.py
--rw-r--r--   0 runner    (1001) docker     (123)     4024 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/test/integration/test_auth_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     5648 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/test/integration/test_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     5742 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/test/integration/test_backend_serialization.py
--rw-r--r--   0 runner    (1001) docker     (123)     2544 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/test/integration/test_basic_server_paths.py
--rw-r--r--   0 runner    (1001) docker     (123)    13736 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/test/integration/test_estimator.py
--rw-r--r--   0 runner    (1001) docker     (123)    11564 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/test/integration/test_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     4754 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/test/integration/test_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     8698 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/test/integration/test_program.py
--rw-r--r--   0 runner    (1001) docker     (123)    11720 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/test/integration/test_proxies.py
--rw-r--r--   0 runner    (1001) docker     (123)     9571 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/test/integration/test_results.py
--rw-r--r--   0 runner    (1001) docker     (123)     8813 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/test/integration/test_retrieve_job.py
--rw-r--r--   0 runner    (1001) docker     (123)    11968 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/test/integration/test_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3908 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/test/integration/test_session.py
--rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/test/program.py
--rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/test/serialization.py
--rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/test/templates.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:22:39.160676 qiskit-ibm-runtime-0.9.3/test/unit/
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/test/unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:22:39.164676 qiskit-ibm-runtime-0.9.3/test/unit/mock/
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/test/unit/mock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/test/unit/mock/fake_api_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/test/unit/mock/fake_quantum_auth_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    17945 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/test/unit/mock/fake_runtime_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     5196 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/test/unit/mock/fake_runtime_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     3561 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/test/unit/mock/http_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/test/unit/mock/proxy_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/test/unit/mock/ws_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/test/unit/mock/ws_server.py
--rw-r--r--   0 runner    (1001) docker     (123)    39797 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/test/unit/test_account.py
--rw-r--r--   0 runner    (1001) docker     (123)    11129 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/test/unit/test_backend_retrieval.py
--rw-r--r--   0 runner    (1001) docker     (123)     6828 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/test/unit/test_client_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)    11992 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/test/unit/test_data_serialization.py
--rw-r--r--   0 runner    (1001) docker     (123)     4580 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/test/unit/test_estimator.py
--rw-r--r--   0 runner    (1001) docker     (123)    36753 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/test/unit/test_ibm_primitives.py
--rw-r--r--   0 runner    (1001) docker     (123)    12854 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/test/unit/test_job_retrieval.py
--rw-r--r--   0 runner    (1001) docker     (123)    12750 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/test/unit/test_jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8004 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/test/unit/test_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     7127 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/test/unit/test_options.py
--rw-r--r--   0 runner    (1001) docker     (123)    10715 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/test/unit/test_programs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/test/unit/test_runtime_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     8700 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/test/unit/test_runtime_ws.py
--rw-r--r--   0 runner    (1001) docker     (123)     4221 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/test/unit/test_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     9354 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/test/unit/test_session.py
--rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/test/unit/test_utils_converters.py
--rw-r--r--   0 runner    (1001) docker     (123)     8311 2023-04-13 17:22:17.000000 qiskit-ibm-runtime-0.9.3/test/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 20:43:16.733611 qiskit-ibm-runtime-0.9.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11416 2023-05-04 20:43:06.000000 qiskit-ibm-runtime-0.9.4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-04 20:43:06.000000 qiskit-ibm-runtime-0.9.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    12913 2023-05-04 20:43:16.733611 qiskit-ibm-runtime-0.9.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11687 2023-05-04 20:43:06.000000 qiskit-ibm-runtime-0.9.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 20:43:16.713611 qiskit-ibm-runtime-0.9.4/program_source/
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-05-04 20:43:06.000000 qiskit-ibm-runtime-0.9.4/program_source/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 20:43:16.713611 qiskit-ibm-runtime-0.9.4/program_source/circuit_runner/
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-05-04 20:43:06.000000 qiskit-ibm-runtime-0.9.4/program_source/circuit_runner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-05-04 20:43:06.000000 qiskit-ibm-runtime-0.9.4/program_source/circuit_runner/circuit_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 20:43:16.713611 qiskit-ibm-runtime-0.9.4/program_source/hello_world/
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-05-04 20:43:06.000000 qiskit-ibm-runtime-0.9.4/program_source/hello_world/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-05-04 20:43:06.000000 qiskit-ibm-runtime-0.9.4/program_source/hello_world/hello_world.py
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-05-04 20:43:06.000000 qiskit-ibm-runtime-0.9.4/program_source/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 20:43:16.717611 qiskit-ibm-runtime-0.9.4/qiskit_ibm_runtime/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-04 20:43:06.000000 qiskit-ibm-runtime-0.9.4/qiskit_ibm_runtime/VERSION.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8939 2023-05-04 20:43:06.000000 qiskit-ibm-runtime-0.9.4/qiskit_ibm_runtime/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 20:43:16.717611 qiskit-ibm-runtime-0.9.4/qiskit_ibm_runtime/accounts/
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-05-04 20:43:06.000000 qiskit-ibm-runtime-0.9.4/qiskit_ibm_runtime/accounts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7433 2023-05-04 20:43:06.000000 qiskit-ibm-runtime-0.9.4/qiskit_ibm_runtime/accounts/account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-05-04 20:43:06.000000 qiskit-ibm-runtime-0.9.4/qiskit_ibm_runtime/accounts/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10826 2023-05-04 20:43:06.000000 qiskit-ibm-runtime-0.9.4/qiskit_ibm_runtime/accounts/management.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3293 2023-05-04 20:43:06.000000 qiskit-ibm-runtime-0.9.4/qiskit_ibm_runtime/accounts/storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 20:43:16.717611 qiskit-ibm-runtime-0.9.4/qiskit_ibm_runtime/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-05-04 20:43:06.000000 qiskit-ibm-runtime-0.9.4/qiskit_ibm_runtime/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-05-04 20:43:06.000000 qiskit-ibm-runtime-0.9.4/qiskit_ibm_runtime/api/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2763 2023-05-04 20:43:06.000000 qiskit-ibm-runtime-0.9.4/qiskit_ibm_runtime/api/client_parameters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 20:43:16.717611 qiskit-ibm-runtime-0.9.4/qiskit_ibm_runtime/api/clients/
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-05-04 20:43:06.000000 qiskit-ibm-runtime-0.9.4/qiskit_ibm_runtime/api/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6235 2023-05-04 20:43:06.000000 qiskit-ibm-runtime-0.9.4/qiskit_ibm_runtime/api/clients/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-05-04 20:43:06.000000 qiskit-ibm-runtime-0.9.4/qiskit_ibm_runtime/api/clients/backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10203 2023-05-04 20:43:06.000000 qiskit-ibm-runtime-0.9.4/qiskit_ibm_runtime/api/clients/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12679 2023-05-04 20:43:06.000000 qiskit-ibm-runtime-0.9.4/qiskit_ibm_runtime/api/clients/runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-05-04 20:43:06.000000 qiskit-ibm-runtime-0.9.4/qiskit_ibm_runtime/api/clients/runtime_ws.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-05-04 20:43:06.000000 qiskit-ibm-runtime-0.9.4/qiskit_ibm_runtime/api/clients/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-05-04 20:43:06.000000 qiskit-ibm-runtime-0.9.4/qiskit_ibm_runtime/api/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 20:43:16.721611 qiskit-ibm-runtime-0.9.4/qiskit_ibm_runtime/api/rest/
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-05-04 20:43:06.000000 qiskit-ibm-runtime-0.9.4/qiskit_ibm_runtime/api/rest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4292 2023-05-04 20:43:06.000000 qiskit-ibm-runtime-0.9.4/qiskit_ibm_runtime/api/rest/backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-05-04 20:43:06.000000 qiskit-ibm-runtime-0.9.4/qiskit_ibm_runtime/api/rest/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-05-04 20:43:06.000000 qiskit-ibm-runtime-0.9.4/qiskit_ibm_runtime/api/rest/cloud_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-05-04 20:43:06.000000 qiskit-ibm-runtime-0.9.4/qiskit_ibm_runtime/api/rest/program.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-05-04 20:43:06.000000 qiskit-ibm-runtime-0.9.4/qiskit_ibm_runtime/api/rest/program_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-05-04 20:43:06.000000 qiskit-ibm-runtime-0.9.4/qiskit_ibm_runtime/api/rest/root.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9621 2023-05-04 20:43:06.000000 qiskit-ibm-runtime-0.9.4/qiskit_ibm_runtime/api/rest/runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-05-04 20:43:06.000000 qiskit-ibm-runtime-0.9.4/qiskit_ibm_runtime/api/rest/runtime_session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 20:43:16.721611 qiskit-ibm-runtime-0.9.4/qiskit_ibm_runtime/api/rest/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-05-04 20:43:06.000000 qiskit-ibm-runtime-0.9.4/qiskit_ibm_runtime/api/rest/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-05-04 20:43:06.000000 qiskit-ibm-runtime-0.9.4/qiskit_ibm_runtime/api/rest/utils/data_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15526 2023-05-04 20:43:06.000000 qiskit-ibm-runtime-0.9.4/qiskit_ibm_runtime/api/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4176 2023-05-04 20:43:06.000000 qiskit-ibm-runtime-0.9.4/qiskit_ibm_runtime/backendreservation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-05-04 20:43:06.000000 qiskit-ibm-runtime-0.9.4/qiskit_ibm_runtime/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14657 2023-05-04 20:43:06.000000 qiskit-ibm-runtime-0.9.4/qiskit_ibm_runtime/estimator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-05-04 20:43:06.000000 qiskit-ibm-runtime-0.9.4/qiskit_ibm_runtime/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3225 2023-05-04 20:43:06.000000 qiskit-ibm-runtime-0.9.4/qiskit_ibm_runtime/hub_group_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24074 2023-05-04 20:43:06.000000 qiskit-ibm-runtime-0.9.4/qiskit_ibm_runtime/ibm_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-05-04 20:43:06.000000 qiskit-ibm-runtime-0.9.4/qiskit_ibm_runtime/ibm_qubit_properties.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 20:43:16.721611 qiskit-ibm-runtime-0.9.4/qiskit_ibm_runtime/options/
+-rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-05-04 20:43:06.000000 qiskit-ibm-runtime-0.9.4/qiskit_ibm_runtime/options/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-05-04 20:43:06.000000 qiskit-ibm-runtime-0.9.4/qiskit_ibm_runtime/options/environment_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-05-04 20:43:06.000000 qiskit-ibm-runtime-0.9.4/qiskit_ibm_runtime/options/execution_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9219 2023-05-04 20:43:06.000000 qiskit-ibm-runtime-0.9.4/qiskit_ibm_runtime/options/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3676 2023-05-04 20:43:06.000000 qiskit-ibm-runtime-0.9.4/qiskit_ibm_runtime/options/resilience_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-05-04 20:43:06.000000 qiskit-ibm-runtime-0.9.4/qiskit_ibm_runtime/options/simulator_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-05-04 20:43:06.000000 qiskit-ibm-runtime-0.9.4/qiskit_ibm_runtime/options/transpilation_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-05-04 20:43:06.000000 qiskit-ibm-runtime-0.9.4/qiskit_ibm_runtime/options/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 20:43:16.721611 qiskit-ibm-runtime-0.9.4/qiskit_ibm_runtime/program/
+-rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-05-04 20:43:06.000000 qiskit-ibm-runtime-0.9.4/qiskit_ibm_runtime/program/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-05-04 20:43:06.000000 qiskit-ibm-runtime-0.9.4/qiskit_ibm_runtime/program/program_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-05-04 20:43:06.000000 qiskit-ibm-runtime-0.9.4/qiskit_ibm_runtime/program/program_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-05-04 20:43:06.000000 qiskit-ibm-runtime-0.9.4/qiskit_ibm_runtime/program/result_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-05-04 20:43:06.000000 qiskit-ibm-runtime-0.9.4/qiskit_ibm_runtime/program/user_messenger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 20:43:16.721611 qiskit-ibm-runtime-0.9.4/qiskit_ibm_runtime/proxies/
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-05-04 20:43:06.000000 qiskit-ibm-runtime-0.9.4/qiskit_ibm_runtime/proxies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4684 2023-05-04 20:43:06.000000 qiskit-ibm-runtime-0.9.4/qiskit_ibm_runtime/proxies/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59748 2023-05-04 20:43:06.000000 qiskit-ibm-runtime-0.9.4/qiskit_ibm_runtime/qiskit_runtime_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 20:43:16.721611 qiskit-ibm-runtime-0.9.4/qiskit_ibm_runtime/qpy/
+-rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-05-04 20:43:06.000000 qiskit-ibm-runtime-0.9.4/qiskit_ibm_runtime/qpy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 20:43:16.725611 qiskit-ibm-runtime-0.9.4/qiskit_ibm_runtime/qpy/binary_io/
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-05-04 20:43:06.000000 qiskit-ibm-runtime-0.9.4/qiskit_ibm_runtime/qpy/binary_io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40086 2023-05-04 20:43:06.000000 qiskit-ibm-runtime-0.9.4/qiskit_ibm_runtime/qpy/binary_io/circuits.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18811 2023-05-04 20:43:06.000000 qiskit-ibm-runtime-0.9.4/qiskit_ibm_runtime/qpy/binary_io/schedules.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12654 2023-05-04 20:43:06.000000 qiskit-ibm-runtime-0.9.4/qiskit_ibm_runtime/qpy/binary_io/value.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10830 2023-05-04 20:43:06.000000 qiskit-ibm-runtime-0.9.4/qiskit_ibm_runtime/qpy/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-05-04 20:43:06.000000 qiskit-ibm-runtime-0.9.4/qiskit_ibm_runtime/qpy/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7833 2023-05-04 20:43:06.000000 qiskit-ibm-runtime-0.9.4/qiskit_ibm_runtime/qpy/formats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9719 2023-05-04 20:43:06.000000 qiskit-ibm-runtime-0.9.4/qiskit_ibm_runtime/qpy/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12466 2023-05-04 20:43:06.000000 qiskit-ibm-runtime-0.9.4/qiskit_ibm_runtime/qpy/type_keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22526 2023-05-04 20:43:06.000000 qiskit-ibm-runtime-0.9.4/qiskit_ibm_runtime/runtime_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4164 2023-05-04 20:43:06.000000 qiskit-ibm-runtime-0.9.4/qiskit_ibm_runtime/runtime_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15441 2023-05-04 20:43:06.000000 qiskit-ibm-runtime-0.9.4/qiskit_ibm_runtime/runtime_program.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4834 2023-05-04 20:43:06.000000 qiskit-ibm-runtime-0.9.4/qiskit_ibm_runtime/runtime_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12673 2023-05-04 20:43:06.000000 qiskit-ibm-runtime-0.9.4/qiskit_ibm_runtime/sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10374 2023-05-04 20:43:06.000000 qiskit-ibm-runtime-0.9.4/qiskit_ibm_runtime/session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 20:43:16.725611 qiskit-ibm-runtime-0.9.4/qiskit_ibm_runtime/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-05-04 20:43:06.000000 qiskit-ibm-runtime-0.9.4/qiskit_ibm_runtime/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7560 2023-05-04 20:43:06.000000 qiskit-ibm-runtime-0.9.4/qiskit_ibm_runtime/utils/backend_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5318 2023-05-04 20:43:06.000000 qiskit-ibm-runtime-0.9.4/qiskit_ibm_runtime/utils/backend_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5262 2023-05-04 20:43:06.000000 qiskit-ibm-runtime-0.9.4/qiskit_ibm_runtime/utils/converters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-05-04 20:43:06.000000 qiskit-ibm-runtime-0.9.4/qiskit_ibm_runtime/utils/deprecation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-04 20:43:06.000000 qiskit-ibm-runtime-0.9.4/qiskit_ibm_runtime/utils/estimator_result_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-05-04 20:43:06.000000 qiskit-ibm-runtime-0.9.4/qiskit_ibm_runtime/utils/hgp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11267 2023-05-04 20:43:06.000000 qiskit-ibm-runtime-0.9.4/qiskit_ibm_runtime/utils/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-05-04 20:43:06.000000 qiskit-ibm-runtime-0.9.4/qiskit_ibm_runtime/utils/runner_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-05-04 20:43:06.000000 qiskit-ibm-runtime-0.9.4/qiskit_ibm_runtime/utils/sampler_result_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11350 2023-05-04 20:43:06.000000 qiskit-ibm-runtime-0.9.4/qiskit_ibm_runtime/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-05-04 20:43:06.000000 qiskit-ibm-runtime-0.9.4/qiskit_ibm_runtime/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 20:43:16.717611 qiskit-ibm-runtime-0.9.4/qiskit_ibm_runtime.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12913 2023-05-04 20:43:16.000000 qiskit-ibm-runtime-0.9.4/qiskit_ibm_runtime.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5280 2023-05-04 20:43:16.000000 qiskit-ibm-runtime-0.9.4/qiskit_ibm_runtime.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 20:43:16.000000 qiskit-ibm-runtime-0.9.4/qiskit_ibm_runtime.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 20:43:16.000000 qiskit-ibm-runtime-0.9.4/qiskit_ibm_runtime.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-04 20:43:16.000000 qiskit-ibm-runtime-0.9.4/qiskit_ibm_runtime.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-04 20:43:16.000000 qiskit-ibm-runtime-0.9.4/qiskit_ibm_runtime.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-05-04 20:43:16.733611 qiskit-ibm-runtime-0.9.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-05-04 20:43:06.000000 qiskit-ibm-runtime-0.9.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 20:43:16.725611 qiskit-ibm-runtime-0.9.4/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-05-04 20:43:06.000000 qiskit-ibm-runtime-0.9.4/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5756 2023-05-04 20:43:06.000000 qiskit-ibm-runtime-0.9.4/test/account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5069 2023-05-04 20:43:06.000000 qiskit-ibm-runtime-0.9.4/test/decorators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 20:43:16.725611 qiskit-ibm-runtime-0.9.4/test/e2e/
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-05-04 20:43:06.000000 qiskit-ibm-runtime-0.9.4/test/e2e/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3270 2023-05-04 20:43:06.000000 qiskit-ibm-runtime-0.9.4/test/e2e/test_tutorials.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7120 2023-05-04 20:43:06.000000 qiskit-ibm-runtime-0.9.4/test/ibm_test_case.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 20:43:16.729611 qiskit-ibm-runtime-0.9.4/test/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-04 20:43:06.000000 qiskit-ibm-runtime-0.9.4/test/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-05-04 20:43:06.000000 qiskit-ibm-runtime-0.9.4/test/integration/test_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4024 2023-05-04 20:43:06.000000 qiskit-ibm-runtime-0.9.4/test/integration/test_auth_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5648 2023-05-04 20:43:06.000000 qiskit-ibm-runtime-0.9.4/test/integration/test_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5742 2023-05-04 20:43:06.000000 qiskit-ibm-runtime-0.9.4/test/integration/test_backend_serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2544 2023-05-04 20:43:06.000000 qiskit-ibm-runtime-0.9.4/test/integration/test_basic_server_paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10799 2023-05-04 20:43:06.000000 qiskit-ibm-runtime-0.9.4/test/integration/test_estimator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11834 2023-05-04 20:43:06.000000 qiskit-ibm-runtime-0.9.4/test/integration/test_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4754 2023-05-04 20:43:06.000000 qiskit-ibm-runtime-0.9.4/test/integration/test_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8698 2023-05-04 20:43:06.000000 qiskit-ibm-runtime-0.9.4/test/integration/test_program.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11720 2023-05-04 20:43:06.000000 qiskit-ibm-runtime-0.9.4/test/integration/test_proxies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9578 2023-05-04 20:43:06.000000 qiskit-ibm-runtime-0.9.4/test/integration/test_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8418 2023-05-04 20:43:06.000000 qiskit-ibm-runtime-0.9.4/test/integration/test_retrieve_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10033 2023-05-04 20:43:06.000000 qiskit-ibm-runtime-0.9.4/test/integration/test_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3908 2023-05-04 20:43:06.000000 qiskit-ibm-runtime-0.9.4/test/integration/test_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-05-04 20:43:06.000000 qiskit-ibm-runtime-0.9.4/test/program.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-05-04 20:43:06.000000 qiskit-ibm-runtime-0.9.4/test/serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-05-04 20:43:06.000000 qiskit-ibm-runtime-0.9.4/test/templates.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 20:43:16.729611 qiskit-ibm-runtime-0.9.4/test/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-05-04 20:43:06.000000 qiskit-ibm-runtime-0.9.4/test/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 20:43:16.733611 qiskit-ibm-runtime-0.9.4/test/unit/mock/
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-04 20:43:06.000000 qiskit-ibm-runtime-0.9.4/test/unit/mock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-05-04 20:43:06.000000 qiskit-ibm-runtime-0.9.4/test/unit/mock/fake_api_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-05-04 20:43:06.000000 qiskit-ibm-runtime-0.9.4/test/unit/mock/fake_quantum_auth_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17945 2023-05-04 20:43:06.000000 qiskit-ibm-runtime-0.9.4/test/unit/mock/fake_runtime_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5196 2023-05-04 20:43:06.000000 qiskit-ibm-runtime-0.9.4/test/unit/mock/fake_runtime_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3561 2023-05-04 20:43:06.000000 qiskit-ibm-runtime-0.9.4/test/unit/mock/http_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-05-04 20:43:06.000000 qiskit-ibm-runtime-0.9.4/test/unit/mock/proxy_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-05-04 20:43:06.000000 qiskit-ibm-runtime-0.9.4/test/unit/mock/ws_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-05-04 20:43:06.000000 qiskit-ibm-runtime-0.9.4/test/unit/mock/ws_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39797 2023-05-04 20:43:06.000000 qiskit-ibm-runtime-0.9.4/test/unit/test_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11129 2023-05-04 20:43:06.000000 qiskit-ibm-runtime-0.9.4/test/unit/test_backend_retrieval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6828 2023-05-04 20:43:06.000000 qiskit-ibm-runtime-0.9.4/test/unit/test_client_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11992 2023-05-04 20:43:06.000000 qiskit-ibm-runtime-0.9.4/test/unit/test_data_serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4580 2023-05-04 20:43:06.000000 qiskit-ibm-runtime-0.9.4/test/unit/test_estimator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36947 2023-05-04 20:43:06.000000 qiskit-ibm-runtime-0.9.4/test/unit/test_ibm_primitives.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12854 2023-05-04 20:43:06.000000 qiskit-ibm-runtime-0.9.4/test/unit/test_job_retrieval.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12750 2023-05-04 20:43:06.000000 qiskit-ibm-runtime-0.9.4/test/unit/test_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8004 2023-05-04 20:43:06.000000 qiskit-ibm-runtime-0.9.4/test/unit/test_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7127 2023-05-04 20:43:06.000000 qiskit-ibm-runtime-0.9.4/test/unit/test_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10715 2023-05-04 20:43:06.000000 qiskit-ibm-runtime-0.9.4/test/unit/test_programs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-05-04 20:43:06.000000 qiskit-ibm-runtime-0.9.4/test/unit/test_runtime_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8700 2023-05-04 20:43:06.000000 qiskit-ibm-runtime-0.9.4/test/unit/test_runtime_ws.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4221 2023-05-04 20:43:06.000000 qiskit-ibm-runtime-0.9.4/test/unit/test_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9354 2023-05-04 20:43:06.000000 qiskit-ibm-runtime-0.9.4/test/unit/test_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-05-04 20:43:06.000000 qiskit-ibm-runtime-0.9.4/test/unit/test_utils_converters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8311 2023-05-04 20:43:06.000000 qiskit-ibm-runtime-0.9.4/test/utils.py
```

### Comparing `qiskit-ibm-runtime-0.9.3/LICENSE.txt` & `qiskit-ibm-runtime-0.9.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.3/PKG-INFO` & `qiskit-ibm-runtime-0.9.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qiskit-ibm-runtime
-Version: 0.9.3
+Version: 0.9.4
 Summary: IBM Quantum client for Qiskit Runtime.
 Home-page: https://github.com/Qiskit/qiskit-ibm-runtime
 Author: Qiskit Development Team
 Author-email: hello@qiskit.org
 License: Apache 2.0
 Project-URL: Bug Tracker, https://github.com/Qiskit/qiskit-ibm-runtime/issues
 Project-URL: Documentation, https://qiskit.org/documentation/
```

### Comparing `qiskit-ibm-runtime-0.9.3/README.md` & `qiskit-ibm-runtime-0.9.4/README.md`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.3/program_source/__init__.py` & `qiskit-ibm-runtime-0.9.4/program_source/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.3/program_source/circuit_runner/__init__.py` & `qiskit-ibm-runtime-0.9.4/program_source/circuit_runner/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.3/program_source/circuit_runner/circuit_runner.py` & `qiskit-ibm-runtime-0.9.4/program_source/circuit_runner/circuit_runner.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.3/program_source/hello_world/__init__.py` & `qiskit-ibm-runtime-0.9.4/program_source/hello_world/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.3/program_source/hello_world/hello_world.py` & `qiskit-ibm-runtime-0.9.4/program_source/hello_world/hello_world.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/__init__.py` & `qiskit-ibm-runtime-0.9.4/qiskit_ibm_runtime/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/accounts/__init__.py` & `qiskit-ibm-runtime-0.9.4/qiskit_ibm_runtime/accounts/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/accounts/account.py` & `qiskit-ibm-runtime-0.9.4/qiskit_ibm_runtime/accounts/account.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/accounts/exceptions.py` & `qiskit-ibm-runtime-0.9.4/qiskit_ibm_runtime/accounts/exceptions.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/accounts/management.py` & `qiskit-ibm-runtime-0.9.4/qiskit_ibm_runtime/accounts/management.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/accounts/storage.py` & `qiskit-ibm-runtime-0.9.4/qiskit_ibm_runtime/accounts/storage.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/api/__init__.py` & `qiskit-ibm-runtime-0.9.4/qiskit_ibm_runtime/api/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/api/auth.py` & `qiskit-ibm-runtime-0.9.4/qiskit_ibm_runtime/api/auth.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/api/client_parameters.py` & `qiskit-ibm-runtime-0.9.4/qiskit_ibm_runtime/api/client_parameters.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/api/clients/__init__.py` & `qiskit-ibm-runtime-0.9.4/qiskit_ibm_runtime/api/clients/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/api/clients/auth.py` & `qiskit-ibm-runtime-0.9.4/qiskit_ibm_runtime/api/clients/auth.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/api/clients/backend.py` & `qiskit-ibm-runtime-0.9.4/qiskit_ibm_runtime/api/clients/backend.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/api/clients/base.py` & `qiskit-ibm-runtime-0.9.4/qiskit_ibm_runtime/api/clients/base.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/api/clients/runtime.py` & `qiskit-ibm-runtime-0.9.4/qiskit_ibm_runtime/api/clients/runtime.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/api/clients/runtime_ws.py` & `qiskit-ibm-runtime-0.9.4/qiskit_ibm_runtime/api/clients/runtime_ws.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/api/clients/version.py` & `qiskit-ibm-runtime-0.9.4/qiskit_ibm_runtime/api/clients/version.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/api/exceptions.py` & `qiskit-ibm-runtime-0.9.4/qiskit_ibm_runtime/api/exceptions.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/api/rest/__init__.py` & `qiskit-ibm-runtime-0.9.4/qiskit_ibm_runtime/api/rest/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/api/rest/backend.py` & `qiskit-ibm-runtime-0.9.4/qiskit_ibm_runtime/api/rest/backend.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/api/rest/base.py` & `qiskit-ibm-runtime-0.9.4/qiskit_ibm_runtime/api/rest/base.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/api/rest/cloud_backend.py` & `qiskit-ibm-runtime-0.9.4/qiskit_ibm_runtime/api/rest/cloud_backend.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/api/rest/program.py` & `qiskit-ibm-runtime-0.9.4/qiskit_ibm_runtime/api/rest/program.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/api/rest/program_job.py` & `qiskit-ibm-runtime-0.9.4/qiskit_ibm_runtime/api/rest/program_job.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/api/rest/root.py` & `qiskit-ibm-runtime-0.9.4/qiskit_ibm_runtime/api/rest/root.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/api/rest/runtime.py` & `qiskit-ibm-runtime-0.9.4/qiskit_ibm_runtime/api/rest/runtime.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/api/rest/runtime_session.py` & `qiskit-ibm-runtime-0.9.4/qiskit_ibm_runtime/api/rest/runtime_session.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/api/rest/utils/__init__.py` & `qiskit-ibm-runtime-0.9.4/qiskit_ibm_runtime/api/rest/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/api/rest/utils/data_mapper.py` & `qiskit-ibm-runtime-0.9.4/qiskit_ibm_runtime/api/rest/utils/data_mapper.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/api/session.py` & `qiskit-ibm-runtime-0.9.4/qiskit_ibm_runtime/api/session.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/backendreservation.py` & `qiskit-ibm-runtime-0.9.4/qiskit_ibm_runtime/backendreservation.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/constants.py` & `qiskit-ibm-runtime-0.9.4/qiskit_ibm_runtime/constants.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/estimator.py` & `qiskit-ibm-runtime-0.9.4/qiskit_ibm_runtime/estimator.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,33 +11,26 @@
 # that they have been altered from the originals.
 
 """Estimator primitive."""
 
 from __future__ import annotations
 import os
 import copy
-from typing import Iterable, Optional, Dict, Sequence, Any, Union
+from typing import Optional, Dict, Sequence, Any, Union
 import logging
 from dataclasses import asdict
 
-from qiskit.circuit import QuantumCircuit, Parameter
-from qiskit.quantum_info import SparsePauliOp
+from qiskit.circuit import QuantumCircuit
 from qiskit.opflow import PauliSumOp
 from qiskit.quantum_info.operators.base_operator import BaseOperator
 from qiskit.providers.options import Options as TerraOptions
 from qiskit.primitives import BaseEstimator, EstimatorResult
 
 # TODO import _circuit_key from terra once 0.23 is released
-from .qiskit_runtime_service import QiskitRuntimeService
 from .runtime_job import RuntimeJob
-from .utils.deprecation import (
-    deprecate_arguments,
-    issue_deprecation_msg,
-    deprecate_function,
-)
 from .ibm_backend import IBMBackend
 from .session import get_default_session
 from .options import Options
 from .options.utils import set_default_error_levels
 from .constants import DEFAULT_DECODERS
 
 # pylint: disable=unused-import,cyclic-import
@@ -95,118 +88,57 @@
             session.close()
     """
 
     _PROGRAM_ID = "estimator"
 
     def __init__(
         self,
-        circuits: Optional[Union[QuantumCircuit, Iterable[QuantumCircuit]]] = None,
-        observables: Optional[Iterable[SparsePauliOp]] = None,
-        parameters: Optional[Iterable[Iterable[Parameter]]] = None,
-        service: Optional[QiskitRuntimeService] = None,
         session: Optional[Union[Session, str, IBMBackend]] = None,
         options: Optional[Union[Dict, Options]] = None,
-        skip_transpilation: Optional[bool] = False,
     ):
         """Initializes the Estimator primitive.
 
         Args:
-            circuits: (DEPRECATED) A (parameterized) :class:`~qiskit.circuit.QuantumCircuit` or
-                a list of (parameterized) :class:`~qiskit.circuit.QuantumCircuit`.
-
-            observables: (DEPRECATED) A list of :class:`~qiskit.quantum_info.SparsePauliOp`
-
-            parameters: (DEPRECATED) A list of parameters of the quantum circuits.
-                (:class:`~qiskit.circuit.parametertable.ParameterView` or
-                a list of :class:`~qiskit.circuit.Parameter`) specifying the order
-                in which parameter values will be bound.
-
-            service: (DEPRECATED) Optional instance of
-                :class:`qiskit_ibm_runtime.QiskitRuntimeService` class,
-                defaults to `QiskitRuntimeService()` which tries to initialize your default
-                saved account.
-
             session: Session in which to call the primitive.
 
                 * If an instance of :class:`qiskit_ibm_runtime.IBMBackend` class or
                   string name of a backend is specified, a new session is created for
                   that backend, unless a default session for the same backend
                   and channel already exists.
 
                 * If ``None``, a new session is created using the default saved
                   account and a default backend (IBM Cloud channel only), unless
                   a default session already exists.
 
             options: Primitive options, see :class:`Options` for detailed description.
                 The ``backend`` keyword is still supported but is deprecated.
-
-            skip_transpilation: (DEPRECATED) Transpilation is skipped if set to True. False by default.
-                Ignored ``skip_transpilation`` is also specified in ``options``.
         """
         # `self._options` in this class is a Dict.
         # The base class, however, uses a `_run_options` which is an instance of
         # qiskit.providers.Options. We largely ignore this _run_options because we use
         # a nested dictionary to categorize options.
-        super().__init__(
-            circuits=circuits,
-            observables=observables,
-            parameters=parameters,
-        )
-
-        if skip_transpilation:
-            deprecate_arguments(
-                "skip_transpilation",
-                "0.7",
-                "Instead, use the skip_transpilation keyword argument in transpilation_settings.",
-            )
-        if service:
-            deprecate_arguments(
-                "service", "0.7", "Please use the session parameter instead."
-            )
+        super().__init__()
 
         backend = None
         self._session: Session = None
 
         if options is None:
             self._options = asdict(Options())
         elif isinstance(options, Options):
-            skip_transpilation = (
-                options.transpilation.skip_transpilation  # type: ignore[union-attr]
-            )
             self._options = asdict(copy.deepcopy(options))
         else:
             options_copy = copy.deepcopy(options)
-            backend = options_copy.pop("backend", None)
-            if backend is not None:
-                issue_deprecation_msg(
-                    msg="The 'backend' key in 'options' has been deprecated",
-                    version="0.7",
-                    remedy="Please pass the backend when opening a session.",
-                )
             default_options = asdict(Options())
             self._options = Options._merge_options(default_options, options_copy)
-            skip_transpilation = self._options.get("transpilation", {}).get(
-                "skip_transpilation", False
-            )
-
-        self._options["transpilation"][
-            "skip_transpilation"
-        ] = skip_transpilation  # type: ignore[union-attr]
-
-        self._initial_inputs = {
-            "circuits": circuits,
-            "observables": observables,
-            "parameters": parameters,
-        }
 
         if isinstance(session, Session):
             self._session = session
         else:
             backend = session or backend
-            self._session = get_default_session(service, backend)
+            self._session = get_default_session(None, backend)
 
         # self._first_run = True
         # self._circuits_map = {}
         # if self.circuits:
         #     for circuit in self.circuits:
         #         circuit_id = _hash(
         #             json.dumps(_circuit_key(circuit), cls=RuntimeEncoder)
@@ -382,25 +314,14 @@
         return self._session.run(
             program_id=self._PROGRAM_ID,
             inputs=inputs,
             options=Options._get_runtime_options(combined),
             result_decoder=DEFAULT_DECODERS.get(self._PROGRAM_ID),
         ).result()
 
-    @deprecate_function(
-        deprecated="close",
-        version="0.7",
-        remedy="Use qiskit_ibm_runtime.Session.close() instead",
-    )
-    def close(self) -> None:
-        """Close the session and free resources.
-        Close the session only if all jobs are finished
-        and you don't need to run more in the session."""
-        self._session.close()
-
     @property
     def session(self) -> Session:
         """Return session used by this primitive.
 
         Returns:
             Session used by this primitive.
         """
```

### Comparing `qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/exceptions.py` & `qiskit-ibm-runtime-0.9.4/qiskit_ibm_runtime/exceptions.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/hub_group_project.py` & `qiskit-ibm-runtime-0.9.4/qiskit_ibm_runtime/hub_group_project.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/ibm_backend.py` & `qiskit-ibm-runtime-0.9.4/qiskit_ibm_runtime/ibm_backend.py`

 * *Files 0% similar despite different names*

```diff
@@ -174,15 +174,19 @@
         self._service = service
         self._api_client = api_client
         self._configuration = configuration
         self._properties = None
         self._defaults = None
         self._target = None
         self._max_circuits = configuration.max_experiments
-        if not self._configuration.simulator:
+        if (
+            not self._configuration.simulator
+            and hasattr(self.options, "noise_model")
+            and hasattr(self.options, "seed_simulator")
+        ):
             self.options.set_validator("noise_model", type(None))
             self.options.set_validator("seed_simulator", type(None))
         if hasattr(configuration, "max_shots"):
             self.options.set_validator("shots", (1, configuration.max_shots))
         if hasattr(configuration, "rep_delay_range"):
             self.options.set_validator(
                 "rep_delay",
```

### Comparing `qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/ibm_qubit_properties.py` & `qiskit-ibm-runtime-0.9.4/qiskit_ibm_runtime/ibm_qubit_properties.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/options/__init__.py` & `qiskit-ibm-runtime-0.9.4/qiskit_ibm_runtime/options/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/options/environment_options.py` & `qiskit-ibm-runtime-0.9.4/qiskit_ibm_runtime/options/environment_options.py`

 * *Files 26% similar despite different names*

```diff
@@ -10,17 +10,26 @@
 # copyright notice, and modified files need to carry a notice indicating
 # that they have been altered from the originals.
 
 """Options related to the execution environment."""
 
 from typing import Optional, Callable, List
 from dataclasses import dataclass, field
+from typing_extensions import Literal, get_args
 
 from .utils import _flexible
 
+LogLevelType = Literal[
+    "DEBUG",
+    "INFO",
+    "WARNING",
+    "ERROR",
+    "CRITICAL",
+]
+
 
 @_flexible
 @dataclass
 class EnvironmentOptions:
     """Options related to the execution environment.
 
     Args:
@@ -38,7 +47,20 @@
             as a filter in the :meth:`qiskit_ibm_runtime.qiskit_runtime_service.jobs()`
             function call.
     """
 
     log_level: str = "WARNING"
     callback: Optional[Callable] = None
     job_tags: Optional[List] = field(default_factory=list)
+
+    @staticmethod
+    def validate_environment_options(environment_options: dict) -> None:
+        """Validate that environment options are legal.
+        Raises:
+            ValueError: if log_level is not in LogLevelType.
+        """
+        log_level = environment_options.get("log_level")
+        if not log_level in get_args(LogLevelType):
+            raise ValueError(
+                f"Unsupported value {log_level} for log_level. "
+                f"Supported values are {get_args(LogLevelType)}"
+            )
```

### Comparing `qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/options/execution_options.py` & `qiskit-ibm-runtime-0.9.4/qiskit_ibm_runtime/options/execution_options.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/options/options.py` & `qiskit-ibm-runtime-0.9.4/qiskit_ibm_runtime/options/options.py`

 * *Files 2% similar despite different names*

```diff
@@ -170,14 +170,18 @@
             range(Options._MAX_OPTIMIZATION_LEVEL + 1)
         ):
             raise ValueError(
                 f"optimization_level can only take the values "
                 f"{list(range(Options._MAX_OPTIMIZATION_LEVEL + 1))}"
             )
         ResilienceOptions.validate_resilience_options(options.get("resilience"))
+        TranspilationOptions.validate_transpilation_options(
+            options.get("transpilation")
+        )
+        EnvironmentOptions.validate_environment_options(options.get("environment"))
 
     @staticmethod
     def _get_runtime_options(options: dict) -> dict:
         """Extract runtime options.
 
         Returns:
             Runtime options.
```

### Comparing `qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/options/resilience_options.py` & `qiskit-ibm-runtime-0.9.4/qiskit_ibm_runtime/options/resilience_options.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,26 +68,26 @@
             ValueError: if extrapolator is not in ExtrapolatorType.
             ValueError: if extrapolator == "QuarticExtrapolator" and number of noise_factors < 5.
             ValueError: if extrapolator == "CubicExtrapolator" and number of noise_factors < 4.
         """
         noise_amplifier = resilience_options.get("noise_amplifier")
         if not noise_amplifier in get_args(NoiseAmplifierType):
             raise ValueError(
-                f"Unsupported value {noise_amplifier} for noise_amplifier."
+                f"Unsupported value {noise_amplifier} for noise_amplifier. "
                 f"Supported values are {get_args(NoiseAmplifierType)}"
             )
         extrapolator = resilience_options.get("extrapolator")
         if not extrapolator in get_args(ExtrapolatorType):
             raise ValueError(
-                f"Unsupported value {extrapolator} for extrapolator."
+                f"Unsupported value {extrapolator} for extrapolator. "
                 f"Supported values are {get_args(ExtrapolatorType)}"
             )
         if (
             extrapolator == "QuarticExtrapolator"
             and len(resilience_options.get("noise_factors")) < 5
         ):
-            raise ValueError("QuarticExtrapolator requires at least 5 noise_factors")
+            raise ValueError("QuarticExtrapolator requires at least 5 noise_factors.")
         if (
             extrapolator == "CubicExtrapolator"
             and len(resilience_options.get("noise_factors")) < 4
         ):
-            raise ValueError("CubicExtrapolator requires at least 4 noise_factors")
+            raise ValueError("CubicExtrapolator requires at least 4 noise_factors.")
```

### Comparing `qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/options/simulator_options.py` & `qiskit-ibm-runtime-0.9.4/qiskit_ibm_runtime/options/simulator_options.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/options/utils.py` & `qiskit-ibm-runtime-0.9.4/qiskit_ibm_runtime/options/utils.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/program/__init__.py` & `qiskit-ibm-runtime-0.9.4/qiskit_ibm_runtime/program/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/program/program_backend.py` & `qiskit-ibm-runtime-0.9.4/qiskit_ibm_runtime/program/program_backend.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/program/program_template.py` & `qiskit-ibm-runtime-0.9.4/qiskit_ibm_runtime/program/program_template.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/program/result_decoder.py` & `qiskit-ibm-runtime-0.9.4/qiskit_ibm_runtime/program/result_decoder.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/program/user_messenger.py` & `qiskit-ibm-runtime-0.9.4/qiskit_ibm_runtime/program/user_messenger.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/proxies/__init__.py` & `qiskit-ibm-runtime-0.9.4/qiskit_ibm_runtime/proxies/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/proxies/configuration.py` & `qiskit-ibm-runtime-0.9.4/qiskit_ibm_runtime/proxies/configuration.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/qiskit_runtime_service.py` & `qiskit-ibm-runtime-0.9.4/qiskit_ibm_runtime/qiskit_runtime_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,38 +43,25 @@
     RuntimeProgramNotFound,
     RuntimeJobNotFound,
 )
 from .hub_group_project import HubGroupProject  # pylint: disable=cyclic-import
 from .program.result_decoder import ResultDecoder
 from .runtime_job import RuntimeJob
 from .runtime_program import RuntimeProgram, ParameterNamespace
-from .runtime_session import RuntimeSession  # pylint: disable=cyclic-import
 from .utils import RuntimeDecoder, to_base64_string, to_python_identifier
 from .utils.backend_decoder import configuration_from_server_data
 from .utils.hgp import to_instance_format, from_instance_format
 from .api.client_parameters import ClientParameters
 from .runtime_options import RuntimeOptions
 from .ibm_backend import IBMBackend
-from .utils.deprecation import (
-    deprecate_function,
-    deprecate_arguments,
-)
 
 logger = logging.getLogger(__name__)
 
 SERVICE_NAME = "runtime"
 
-DEPRECATED_PROGRAMS = [
-    "torch-train",
-    "torch-infer",
-    "sample-expval",
-    "quantum_kernal_alignment",
-    "sample-program",
-]
-
 
 class QiskitRuntimeService(Provider):
     """Class for interacting with the Qiskit Runtime service.
 
     Qiskit Runtime is a new architecture offered by IBM Quantum that
     streamlines computations requiring many iterations. These experiments will
     execute significantly faster within its improved hybrid quantum/classical
@@ -129,15 +116,14 @@
     methods to perform tasks like checking job status, getting job result, and
     canceling job.
     """
 
     def __init__(
         self,
         channel: Optional[ChannelType] = None,
-        auth: Optional[AccountType] = None,
         token: Optional[str] = None,
         url: Optional[str] = None,
         filename: Optional[str] = None,
         name: Optional[str] = None,
         instance: Optional[str] = None,
         proxies: Optional[dict] = None,
         verify: Optional[bool] = None,
@@ -154,15 +140,14 @@
             - Default account for the ``ibm_quantum`` account, if one is available.
 
         `instance`, `proxies`, and `verify` can be used to overwrite corresponding
         values in the loaded account.
 
         Args:
             channel: Channel type. ``ibm_cloud`` or ``ibm_quantum``.
-            auth: (DEPRECATED, use `channel` instead) Authentication type. ``cloud`` or ``legacy``.
             token: IBM Cloud API key or IBM Quantum API token.
             url: The API URL.
                 Defaults to https://cloud.ibm.com (ibm_cloud) or
                 https://auth.quantum-computing.ibm.com/api (ibm_quantum).
             filename: Full path of the file where the account is created.
                 Default: _DEFAULT_ACCOUNT_CONFIG_JSON_FILE
             name: Name of the account to load.
@@ -180,23 +165,19 @@
             An instance of QiskitRuntimeService.
 
         Raises:
             IBMInputValueError: If an input is invalid.
         """
         super().__init__()
 
-        if auth:
-            self._auth_warning()
-
         self._account = self._discover_account(
             token=token,
             url=url,
             instance=instance,
             channel=channel,
-            auth=auth,
             filename=filename,
             name=name,
             proxies=ProxyConfiguration(**proxies) if proxies else None,
             verify=verify,
         )
 
         self._client_params = ClientParameters(
@@ -232,25 +213,14 @@
                     if backend_name not in self._backends:
                         self._backends[backend_name] = None
 
         # TODO - it'd be nice to allow some kind of autocomplete, but `service.ibmq_foo`
         # just seems wrong since backends are not runtime service instances.
         # self._discover_backends()
 
-    @staticmethod
-    def _auth_warning() -> None:
-        warnings.warn(
-            "Use of `auth` parameter is deprecated and will "
-            "be removed in a future release. "
-            "You can now use channel='ibm_cloud' or "
-            "channel='ibm_quantum' instead.",
-            DeprecationWarning,
-            stacklevel=3,
-        )
-
     def _discover_account(
         self,
         token: Optional[str] = None,
         url: Optional[str] = None,
         instance: Optional[str] = None,
         channel: Optional[ChannelType] = None,
         auth: Optional[AccountType] = None,
@@ -686,35 +656,28 @@
         """
         return self._account.to_saved_format()
 
     @staticmethod
     def delete_account(
         filename: Optional[str] = None,
         name: Optional[str] = None,
-        auth: Optional[str] = None,
         channel: Optional[ChannelType] = None,
     ) -> bool:
         """Delete a saved account from disk.
 
         Args:
             filename: Name of file from which to delete the account.
             name: Name of the saved account to delete.
-            auth: (DEPRECATED, use `channel` instead) Authentication type of the default
-                account to delete. Ignored if account name is provided.
             channel: Channel type of the default account to delete.
                 Ignored if account name is provided.
 
         Returns:
             True if the account was deleted.
             False if no account was found.
         """
-        if auth:
-            QiskitRuntimeService._auth_warning()
-            channel = channel or QiskitRuntimeService._get_channel_for_auth(auth=auth)
-
         return AccountManager.delete(filename=filename, name=name, channel=channel)
 
     @staticmethod
     def _get_channel_for_auth(auth: str) -> str:
         """Returns channel type based on auth"""
         if auth == "legacy":
             return "ibm_quantum"
@@ -722,15 +685,14 @@
 
     @staticmethod
     def save_account(
         token: Optional[str] = None,
         url: Optional[str] = None,
         instance: Optional[str] = None,
         channel: Optional[ChannelType] = None,
-        auth: Optional[AccountType] = None,
         filename: Optional[str] = None,
         name: Optional[str] = None,
         proxies: Optional[dict] = None,
         verify: Optional[bool] = None,
         overwrite: Optional[bool] = False,
     ) -> None:
         """Save the account to disk for future use.
@@ -738,28 +700,24 @@
         Args:
             token: IBM Cloud API key or IBM Quantum API token.
             url: The API URL.
                 Defaults to https://cloud.ibm.com (ibm_cloud) or
                 https://auth.quantum-computing.ibm.com/api (ibm_quantum).
             instance: The CRN (ibm_cloud) or hub/group/project (ibm_quantum).
             channel: Channel type. `ibm_cloud` or `ibm_quantum`.
-            auth: (DEPRECATED, use `channel` instead) Authentication type. `cloud` or `legacy`.
             filename: Full path of the file where the account is saved.
             name: Name of the account to save.
             proxies: Proxy configuration. Supported optional keys are
                 ``urls`` (a dictionary mapping protocol or protocol and host to the URL of the proxy,
                 documented at https://docs.python-requests.org/en/latest/api/#requests.Session.proxies),
                 ``username_ntlm``, ``password_ntlm`` (username and password to enable NTLM user
                 authentication)
             verify: Verify the server's TLS certificate.
             overwrite: ``True`` if the existing account is to be overwritten.
         """
-        if auth:
-            QiskitRuntimeService._auth_warning()
-            channel = channel or QiskitRuntimeService._get_channel_for_auth(auth)
 
         AccountManager.save(
             token=token,
             url=url,
             instance=instance,
             channel=channel,
             filename=filename,
@@ -768,38 +726,32 @@
             verify=verify,
             overwrite=overwrite,
         )
 
     @staticmethod
     def saved_accounts(
         default: Optional[bool] = None,
-        auth: Optional[str] = None,
         channel: Optional[ChannelType] = None,
         filename: Optional[str] = None,
         name: Optional[str] = None,
     ) -> dict:
         """List the accounts saved on disk.
 
         Args:
             default: If set to True, only default accounts are returned.
-            auth: (DEPRECATED, use `channel` instead) If set, only accounts with the given
-                authentication type are returned.
             channel: Channel type. `ibm_cloud` or `ibm_quantum`.
             filename: Name of file whose accounts are returned.
             name: If set, only accounts with the given name are returned.
 
         Returns:
             A dictionary with information about the accounts saved on disk.
 
         Raises:
             ValueError: If an invalid account is found on disk.
         """
-        if auth:
-            QiskitRuntimeService._auth_warning()
-            channel = channel or QiskitRuntimeService._get_channel_for_auth(auth)
         return dict(
             map(
                 lambda kv: (kv[0], Account.to_saved_format(kv[1])),
                 AccountManager.list(
                     default=default, channel=channel, filename=filename, name=name
                 ).items(),
             ),
@@ -989,18 +941,15 @@
         program_id: str,
         inputs: Union[Dict, ParameterNamespace],
         options: Optional[Union[RuntimeOptions, Dict]] = None,
         callback: Optional[Callable] = None,
         result_decoder: Optional[
             Union[Type[ResultDecoder], Sequence[Type[ResultDecoder]]]
         ] = None,
-        instance: Optional[str] = None,
         session_id: Optional[str] = None,
-        job_tags: Optional[List[str]] = None,
-        max_execution_time: Optional[int] = None,
         start_session: Optional[bool] = False,
     ) -> RuntimeJob:
         """Execute the runtime program.
 
         Args:
             program_id: Program ID.
             inputs: Program input parameters. These input values are passed
@@ -1014,59 +963,32 @@
                     1. Job ID
                     2. Job result.
 
             result_decoder: A :class:`ResultDecoder` subclass used to decode job results.
                 If more than one decoder is specified, the first is used for interim results and
                 the second final results. If not specified, a program-specific decoder or the default
                 ``ResultDecoder`` is used.
-            instance: (DEPRECATED) This is only supported for ``ibm_quantum`` runtime and is in the
-                hub/group/project format.
             session_id: Job ID of the first job in a runtime session.
-            job_tags: (DEPRECATED) Tags to be assigned to the job. The tags can subsequently be used
-                as a filter in the :meth:`jobs()` function call.
-            max_execution_time: (DEPRECATED) Maximum execution time in seconds. This overrides
-                the max_execution_time of the program.
             start_session: Set to True to explicitly start a runtime session. Defaults to False.
 
         Returns:
             A ``RuntimeJob`` instance representing the execution.
 
         Raises:
             IBMInputValueError: If input is invalid.
             RuntimeProgramNotFound: If the program cannot be found.
             IBMRuntimeError: An error occurred running the program.
         """
-        if program_id in DEPRECATED_PROGRAMS:
-            warnings.warn(
-                f"The {program_id} program has been deprecated as of qiskit-ibm-runtime 0.7 \
-                and will be removed no sooner than 1 month after the release date.",
-                DeprecationWarning,
-                stacklevel=2,
-            )
 
         qrt_options: RuntimeOptions = options
         if options is None:
             qrt_options = RuntimeOptions()
         elif isinstance(options, Dict):
             qrt_options = RuntimeOptions(**options)
 
-        deprecated = {
-            "instance": instance,
-            "job_tags": job_tags,
-            "max_execution_time": max_execution_time,
-        }
-        for name, param in deprecated.items():
-            if param is not None:
-                deprecate_arguments(
-                    deprecated=name,
-                    version="0.7",
-                    remedy=f'Please specify "{name}" inside "options".',
-                )
-                setattr(qrt_options, name, param)
-
         # If using params object, extract as dictionary
         if isinstance(inputs, ParameterNamespace):
             inputs.validate()
             inputs = vars(inputs)
 
         qrt_options.validate(channel=self.channel)
 
@@ -1111,41 +1033,14 @@
             user_callback=callback,
             result_decoder=result_decoder,
             image=qrt_options.image,
             service=self,
         )
         return job
 
-    @deprecate_function(
-        "QiskitRuntimeService.open",
-        "0.7",
-        "Instead, use the qiskit_ibm_runtime.Session class to create a runtime session.",
-    )
-    def open(
-        self,
-        program_id: str,
-        inputs: Union[Dict, ParameterNamespace],
-        options: Optional[Union[RuntimeOptions, Dict]] = None,
-    ) -> RuntimeSession:
-        """Open a new runtime session.
-
-        Args:
-            program_id: Program ID.
-            inputs: Initial program input parameters. These input values are
-                persistent throughout the session.
-            options: Runtime options that control the execution environment. See
-                :class:`RuntimeOptions` for all available options.
-
-        Returns:
-            Runtime session.
-        """
-        return RuntimeSession(
-            service=self, program_id=program_id, inputs=inputs, options=options
-        )
-
     def upload_program(
         self, data: str, metadata: Optional[Union[Dict, str]] = None
     ) -> str:
         """Upload a runtime program.
 
         In addition to program data, the following program metadata is also
         required:
@@ -1607,15 +1502,14 @@
     @property
     def auth(self) -> str:
         """Return the authentication type used.
 
         Returns:
             The authentication type used.
         """
-        self._auth_warning()
         return "cloud" if self._channel == "ibm_cloud" else "legacy"
 
     @property
     def channel(self) -> str:
         """Return the channel type used.
 
         Returns:
```

### Comparing `qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/qpy/__init__.py` & `qiskit-ibm-runtime-0.9.4/qiskit_ibm_runtime/qpy/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/qpy/binary_io/__init__.py` & `qiskit-ibm-runtime-0.9.4/qiskit_ibm_runtime/qpy/binary_io/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/qpy/binary_io/circuits.py` & `qiskit-ibm-runtime-0.9.4/qiskit_ibm_runtime/qpy/binary_io/circuits.py`

 * *Files 2% similar despite different names*

```diff
@@ -121,41 +121,57 @@
         if data.type.decode("utf8") == "q":
             registers["q"][name] = (data.standalone, bit_indices, True)
         else:
             registers["c"][name] = (data.standalone, bit_indices, True)
     return registers
 
 
-def _loads_instruction_parameter(type_key, data_bytes, version, vectors):  # type: ignore[no-untyped-def]
+def _loads_instruction_parameter(  # type: ignore[no-untyped-def]
+    type_key, data_bytes, version, vectors, registers, circuit
+):
     if type_key == type_keys.Program.CIRCUIT:
         param = common.data_from_binary(data_bytes, read_circuit, version=version)
     elif type_key == type_keys.Container.RANGE:
         data = formats.RANGE._make(struct.unpack(formats.RANGE_PACK, data_bytes))
         param = range(data.start, data.stop, data.step)
     elif type_key == type_keys.Container.TUPLE:
         param = tuple(
             common.sequence_from_binary(
                 data_bytes,
                 _loads_instruction_parameter,
                 version=version,
                 vectors=vectors,
+                registers=registers,
+                circuit=circuit,
             )
         )
     elif type_key == type_keys.Value.INTEGER:
         # TODO This uses little endian. Should be fixed in the next QPY version.
         param = struct.unpack("<q", data_bytes)[0]
     elif type_key == type_keys.Value.FLOAT:
         # TODO This uses little endian. Should be fixed in the next QPY version.
         param = struct.unpack("<d", data_bytes)[0]
+    elif type_key == type_keys.Value.REGISTER:
+        param = _loads_register_param(
+            data_bytes.decode(common.ENCODE), circuit, registers
+        )
     else:
         param = value.loads_value(type_key, data_bytes, version, vectors)
 
     return param
 
 
+def _loads_register_param(data_bytes, circuit, registers):  # type: ignore[no-untyped-def]
+    # If register name prefixed with null character it's a clbit index for single bit condition.
+    if data_bytes[0] == "\x00":
+        conditional_bit = int(data_bytes[1:])
+        return circuit.clbits[conditional_bit]
+    return registers["c"][data_bytes]
+
+
 def _read_instruction(  # type: ignore[no-untyped-def]
     file_obj, circuit, registers, custom_operations, version, vectors
 ):
     if version < 5:
         instruction = formats.CIRCUIT_INSTRUCTION._make(
             struct.unpack(
                 formats.CIRCUIT_INSTRUCTION_PACK,
@@ -176,25 +192,18 @@
     )
     qargs = []
     cargs = []
     params = []
     condition_tuple = None
     if instruction.has_condition:
         # If register name prefixed with null character it's a clbit index for single bit condition.
-        if condition_register[0] == "\x00":
-            conditional_bit = int(condition_register[1:])
-            condition_tuple = (
-                circuit.clbits[conditional_bit],
-                instruction.condition_value,
-            )
-        else:
-            condition_tuple = (
-                registers["c"][condition_register],
-                instruction.condition_value,
-            )
+        condition_tuple = (
+            _loads_register_param(condition_register, circuit, registers),
+            instruction.condition_value,
+        )
     if circuit is not None:
         qubit_indices = dict(enumerate(circuit.qubits))
         clbit_indices = dict(enumerate(circuit.clbits))
     else:
         qubit_indices = {}
         clbit_indices = {}
 
@@ -220,15 +229,17 @@
             if carg.type.decode(common.ENCODE) == "q":
                 raise TypeError("Invalid input qarg after all qargs")
             cargs.append(clbit_indices[carg.size])
 
     # Load Parameters
     for _param in range(instruction.num_parameters):
         type_key, data_bytes = common.read_generic_typed_data(file_obj)
-        param = _loads_instruction_parameter(type_key, data_bytes, version, vectors)
+        param = _loads_instruction_parameter(
+            type_key, data_bytes, version, vectors, registers, circuit
+        )
         params.append(param)
 
     # Load Gate object
     if gate_name in {"Gate", "Instruction", "ControlledGate"}:
         inst_obj = _parse_custom_operation(
             custom_operations, gate_name, params, version, vectors, registers
         )
@@ -277,15 +288,21 @@
             gate = gate_class(*params, instruction.num_ctrl_qubits)
         else:
             gate = gate_class(*params)
             gate.num_ctrl_qubits = instruction.num_ctrl_qubits
             gate.ctrl_state = instruction.ctrl_state
         gate.condition = condition_tuple
     else:
-        if gate_name in {"Initialize", "UCRXGate", "UCRYGate", "UCRZGate"}:
+        if gate_name in {
+            "Initialize",
+            "StatePreparation",
+            "UCRXGate",
+            "UCRYGate",
+            "UCRZGate",
+        }:
             gate = gate_class(params)
         else:
             if gate_name == "Barrier":
                 params = [len(qargs)]
             elif gate_name in {"BreakLoopOp", "ContinueLoopOp"}:
                 params = [len(qargs), len(cargs)]
             gate = gate_class(*params)
@@ -489,34 +506,46 @@
             calibrations[name] = {(qubits, params): schedule}
         else:
             calibrations[name][(qubits, params)] = schedule
 
     return calibrations
 
 
-def _dumps_instruction_parameter(param):  # type: ignore[no-untyped-def]
+def _dumps_register(register, index_map):  # type: ignore[no-untyped-def]
+    if isinstance(register, ClassicalRegister):
+        return register.name.encode(common.ENCODE)
+    # Clbit.
+    return b"\x00" + str(index_map["c"][register]).encode(common.ENCODE)
+
+
+def _dumps_instruction_parameter(param, index_map):  # type: ignore[no-untyped-def]
     if isinstance(param, QuantumCircuit):
         type_key = type_keys.Program.CIRCUIT
         data_bytes = common.data_to_binary(param, write_circuit)
     elif isinstance(param, range):
         type_key = type_keys.Container.RANGE
         data_bytes = struct.pack(
             formats.RANGE_PACK, param.start, param.stop, param.step
         )
     elif isinstance(param, tuple):
         type_key = type_keys.Container.TUPLE
-        data_bytes = common.sequence_to_binary(param, _dumps_instruction_parameter)
+        data_bytes = common.sequence_to_binary(
+            param, _dumps_instruction_parameter, index_map=index_map
+        )
     elif isinstance(param, int):
         # TODO This uses little endian. This should be fixed in next QPY version.
         type_key = type_keys.Value.INTEGER
         data_bytes = struct.pack("<q", param)
     elif isinstance(param, float):
         # TODO This uses little endian. This should be fixed in next QPY version.
         type_key = type_keys.Value.FLOAT
         data_bytes = struct.pack("<d", param)
+    elif isinstance(param, (Clbit, ClassicalRegister)):
+        type_key = type_keys.Value.REGISTER
+        data_bytes = _dumps_register(param, index_map)
     else:
         type_key, data_bytes = value.dumps_value(param)
 
     return type_key, data_bytes
 
 
 # pylint: disable=too-many-boolean-expressions
@@ -549,38 +578,43 @@
         custom_operations_list.append(gate_class_name)
 
     has_condition = False
     condition_register = b""
     condition_value = 0
     if getattr(instruction.operation, "condition", None):
         has_condition = True
-        if isinstance(instruction.operation.condition[0], Clbit):
-            bit_index = index_map["c"][instruction.operation.condition[0]]
-            condition_register = b"\x00" + str(bit_index).encode(common.ENCODE)
-            condition_value = int(instruction.operation.condition[1])
-        else:
-            condition_register = instruction.operation.condition[0].name.encode(
-                common.ENCODE
-            )
-            condition_value = instruction.operation.condition[1]
+        condition_register = _dumps_register(
+            instruction.operation.condition[0], index_map
+        )
+        condition_value = int(instruction.operation.condition[1])
 
     gate_class_name = gate_class_name.encode(common.ENCODE)
     label = getattr(instruction.operation, "label")
     if label:
         label_raw = label.encode(common.ENCODE)
     else:
         label_raw = b""
 
+    # The instruction params we store are about being able to reconstruct the objects; they don't
+    # necessarily need to match one-to-one to the `params` field.
+    if isinstance(instruction.operation, controlflow.SwitchCaseOp):
+        instruction_params = [
+            instruction.operation.target,
+            tuple(instruction.operation.cases_specifier()),
+        ]
+    else:
+        instruction_params = instruction.operation.params
+
     num_ctrl_qubits = getattr(instruction.operation, "num_ctrl_qubits", 0)
     ctrl_state = getattr(instruction.operation, "ctrl_state", 0)
     instruction_raw = struct.pack(
         formats.CIRCUIT_INSTRUCTION_V2_PACK,
         len(gate_class_name),
         len(label_raw),
-        len(instruction.operation.params),
+        len(instruction_params),
         instruction.operation.num_qubits,
         instruction.operation.num_clbits,
         has_condition,
         len(condition_register),
         condition_value,
         num_ctrl_qubits,
         ctrl_state,
@@ -597,16 +631,16 @@
         file_obj.write(instruction_arg_raw)
     for clbit in instruction.clbits:
         instruction_arg_raw = struct.pack(
             formats.CIRCUIT_INSTRUCTION_ARG_PACK, b"c", index_map["c"][clbit]
         )
         file_obj.write(instruction_arg_raw)
     # Encode instruction params
-    for param in instruction.operation.params:
-        type_key, data_bytes = _dumps_instruction_parameter(param)
+    for param in instruction_params:
+        type_key, data_bytes = _dumps_instruction_parameter(param, index_map)
         common.write_generic_typed_data(file_obj, type_key, data_bytes)
     return custom_operations_list
 
 
 def _write_pauli_evolution_gate(file_obj, evolution_gate):  # type: ignore[no-untyped-def]
     operator_list = evolution_gate.operator
     standalone = False
```

### Comparing `qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/qpy/binary_io/schedules.py` & `qiskit-ibm-runtime-0.9.4/qiskit_ibm_runtime/qpy/binary_io/schedules.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,18 +17,19 @@
 import struct
 import zlib
 import warnings
 
 import numpy as np
 
 from qiskit.exceptions import QiskitError
-from qiskit.pulse import library, channels
+from qiskit.pulse import library, channels, instructions
 from qiskit.pulse.schedule import ScheduleBlock
 from qiskit.utils import optionals as _optional
 from .. import formats, common, type_keys
+from ..exceptions import QpyError
 from . import value
 
 
 if _optional.HAS_SYMENGINE:
     import symengine as sym
 else:
     import sympy as sym
@@ -245,14 +246,16 @@
             )
         else:
             return common.data_from_binary(
                 data_bytes, _read_symbolic_pulse_v6, version=version
             )
     if type_key == type_keys.ScheduleOperand.CHANNEL:
         return common.data_from_binary(data_bytes, _read_channel, version=version)
+    if type_key == type_keys.ScheduleOperand.OPERAND_STR:
+        return data_bytes.decode(common.ENCODE)
 
     return value.loads_value(type_key, data_bytes, version, {})
 
 
 def _read_element(file_obj, version, metadata_deserializer):  # type: ignore[no-untyped-def]
     type_key = common.read_type_key(file_obj)
 
@@ -268,14 +271,34 @@
     instance._operands = tuple(operands)
     instance._name = name
     instance._hash = None
 
     return instance
 
 
+def _loads_reference_item(  # type: ignore[no-untyped-def]
+    type_key, data_bytes, version, metadata_deserializer
+):
+    if type_key == type_keys.Value.NULL:
+        return None
+    if type_key == type_keys.Program.SCHEDULE_BLOCK:
+        return common.data_from_binary(
+            data_bytes,
+            deserializer=read_schedule_block,
+            version=version,
+            metadata_deserializer=metadata_deserializer,
+        )
+
+    raise QpyError(
+        f"Loaded schedule reference item is neither None nor ScheduleBlock. "
+        f"Type key {type_key} is not valid data type for a reference items. "
+        "This data cannot be loaded. Please check QPY version."
+    )
+
+
 def _write_channel(file_obj, data):  # type: ignore[no-untyped-def]
     type_key = type_keys.ScheduleChannel.assign(data)
     common.write_type_key(file_obj, type_key)
     value.write_value(file_obj, data.index)
 
 
 def _write_waveform(file_obj, data):  # type: ignore[no-untyped-def]
@@ -349,14 +372,17 @@
         data_bytes = common.data_to_binary(operand, _write_waveform)
     elif isinstance(operand, library.SymbolicPulse):
         type_key = type_keys.ScheduleOperand.SYMBOLIC_PULSE
         data_bytes = common.data_to_binary(operand, _write_symbolic_pulse)
     elif isinstance(operand, channels.Channel):
         type_key = type_keys.ScheduleOperand.CHANNEL
         data_bytes = common.data_to_binary(operand, _write_channel)
+    elif isinstance(operand, str):
+        type_key = type_keys.ScheduleOperand.OPERAND_STR
+        data_bytes = operand.encode(common.ENCODE)
     else:
         type_key, data_bytes = value.dumps_value(operand)
 
     return type_key, data_bytes
 
 
 def _write_element(file_obj, element, metadata_serializer):  # type: ignore[no-untyped-def]
@@ -370,14 +396,28 @@
             file_obj,
             sequence=element.operands,
             serializer=_dumps_operand,
         )
         value.write_value(file_obj, element.name)
 
 
+def _dumps_reference_item(schedule, metadata_serializer):  # type: ignore[no-untyped-def]
+    if schedule is None:
+        type_key = type_keys.Value.NULL
+        data_bytes = b""
+    else:
+        type_key = type_keys.Program.SCHEDULE_BLOCK
+        data_bytes = common.data_to_binary(
+            obj=schedule,
+            serializer=write_schedule_block,
+            metadata_serializer=metadata_serializer,
+        )
+    return type_key, data_bytes
+
+
 def read_schedule_block(file_obj, version, metadata_deserializer=None):  # type: ignore[no-untyped-def]
     """Read a single ScheduleBlock from the file like object.
 
     Args:
         file_obj (File): A file like object that contains the QPY binary data.
         version (int): QPY version.
         metadata_deserializer (JSONDecoder): An optional JSONDecoder class
@@ -415,14 +455,32 @@
         metadata=metadata,
         alignment_context=context,
     )
     for _ in range(data.num_elements):
         block_elm = _read_element(file_obj, version, metadata_deserializer)
         block.append(block_elm, inplace=True)
 
+    # Load references
+    if version >= 7:
+        flat_key_refdict = common.read_mapping(
+            file_obj=file_obj,
+            deserializer=_loads_reference_item,
+            version=version,
+            metadata_deserializer=metadata_deserializer,
+        )
+        ref_dict = {}
+        for key_str, schedule in flat_key_refdict.items():
+            if schedule is not None:
+                composite_key = tuple(
+                    key_str.split(instructions.Reference.key_delimiter)
+                )
+                ref_dict[composite_key] = schedule
+        if ref_dict:
+            block.assign_references(ref_dict, inplace=True)
+
     return block
 
 
 def write_schedule_block(file_obj, block, metadata_serializer=None):  # type: ignore[no-untyped-def]
     """Write a single ScheduleBlock object in the file like object.
 
     Args:
@@ -449,9 +507,22 @@
     )
     header = struct.pack(formats.SCHEDULE_BLOCK_HEADER_PACK, *header_raw)
     file_obj.write(header)
     file_obj.write(block_name)
     file_obj.write(metadata)
 
     _write_alignment_context(file_obj, block.alignment_context)
-    for block_elm in block.blocks:
+    for block_elm in block._blocks:
         _write_element(file_obj, block_elm, metadata_serializer)
+
+    # Write references
+    flat_key_refdict = {}
+    for ref_keys, schedule in block._reference_manager.items():
+        # Do not call block.reference. This returns the reference of most outer program by design.
+        key_str = instructions.Reference.key_delimiter.join(ref_keys)
+        flat_key_refdict[key_str] = schedule
+    common.write_mapping(
+        file_obj=file_obj,
+        mapping=flat_key_refdict,
+        serializer=_dumps_reference_item,
+        metadata_serializer=metadata_serializer,
+    )
```

### Comparing `qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/qpy/binary_io/value.py` & `qiskit-ibm-runtime-0.9.4/qiskit_ibm_runtime/qpy/binary_io/value.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 
 import struct
 from typing import Any
 import uuid
 
 import numpy as np
 
+from qiskit.circuit import CASE_DEFAULT
 from qiskit.circuit.parameter import Parameter
 from qiskit.circuit.parameterexpression import ParameterExpression
 from qiskit.circuit.parametervector import ParameterVector, ParameterVectorElement
 from qiskit.utils import optionals as _optional
 
 from .. import common, formats, exceptions, type_keys
 
@@ -241,15 +242,15 @@
         binary_data = struct.pack("!d", obj)
     elif type_key == type_keys.Value.COMPLEX:
         binary_data = struct.pack(formats.COMPLEX_PACK, obj.real, obj.imag)
     elif type_key == type_keys.Value.NUMPY_OBJ:
         binary_data = common.data_to_binary(obj, np.save)
     elif type_key == type_keys.Value.STRING:
         binary_data = obj.encode(common.ENCODE)
-    elif type_key == type_keys.Value.NULL:
+    elif type_key in (type_keys.Value.NULL, type_keys.Value.CASE_DEFAULT):
         binary_data = b""
     elif type_key == type_keys.Value.PARAMETER_VECTOR:
         binary_data = common.data_to_binary(obj, _write_parameter_vec)
     elif type_key == type_keys.Value.PARAMETER:
         binary_data = common.data_to_binary(obj, _write_parameter)
     elif type_key == type_keys.Value.PARAMETER_EXPRESSION:
         binary_data = common.data_to_binary(
@@ -298,14 +299,16 @@
         return complex(*struct.unpack(formats.COMPLEX_PACK, binary_data))
     if type_key == type_keys.Value.NUMPY_OBJ:
         return common.data_from_binary(binary_data, np.load)
     if type_key == type_keys.Value.STRING:
         return binary_data.decode(common.ENCODE)
     if type_key == type_keys.Value.NULL:
         return None
+    if type_key == type_keys.Value.CASE_DEFAULT:
+        return CASE_DEFAULT
     if type_key == type_keys.Value.PARAMETER_VECTOR:
         return common.data_from_binary(
             binary_data, _read_parameter_vec, vectors=vectors
         )
     if type_key == type_keys.Value.PARAMETER:
         return common.data_from_binary(binary_data, _read_parameter)
     if type_key == type_keys.Value.PARAMETER_EXPRESSION:
```

### Comparing `qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/qpy/common.py` & `qiskit-ibm-runtime-0.9.4/qiskit_ibm_runtime/qpy/common.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 """
 
 import io
 import struct
 
 from . import formats
 
-QPY_VERSION = 6
+QPY_VERSION = 7
 ENCODE = "utf8"
 
 
 def read_generic_typed_data(file_obj):  # type: ignore[no-untyped-def]
     """Read a single data chunk from the file like object.
 
     Args:
```

### Comparing `qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/qpy/exceptions.py` & `qiskit-ibm-runtime-0.9.4/qiskit_ibm_runtime/qpy/exceptions.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/qpy/formats.py` & `qiskit-ibm-runtime-0.9.4/qiskit_ibm_runtime/qpy/formats.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/qpy/interface.py` & `qiskit-ibm-runtime-0.9.4/qiskit_ibm_runtime/qpy/interface.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 import warnings
 import re
 
 from qiskit.circuit import QuantumCircuit
 from qiskit.pulse import ScheduleBlock
 from qiskit.exceptions import QiskitError
 from qiskit.version import __version__
-from qiskit.utils.deprecation import deprecate_arguments
+from qiskit.utils.deprecation import deprecate_arg
 
 from . import formats, common, binary_io, type_keys
 from .exceptions import QpyError
 
 
 # pylint: disable=invalid-name
 QPY_SUPPORTED_TYPES = Union[QuantumCircuit, ScheduleBlock]
@@ -70,15 +70,15 @@
     (?:\+(?P<local>[a-z0-9]+(?:[-_\.][a-z0-9]+)*))?       # local version
 """
     + "$"
 )
 VERSION_PATTERN_REGEX = re.compile(VERSION_PATTERN, re.VERBOSE | re.IGNORECASE)
 
 
-@deprecate_arguments({"circuits": "programs"})
+@deprecate_arg("circuits", new_alias="programs", since="0.21.0")
 def dump(  # type: ignore[no-untyped-def]
     programs: Union[List[QPY_SUPPORTED_TYPES], QPY_SUPPORTED_TYPES],
     file_obj: BinaryIO,
     metadata_serializer: Optional[Type[JSONEncoder]] = None,
 ):
     """Write QPY binary data to a file
```

### Comparing `qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/qpy/type_keys.py` & `qiskit-ibm-runtime-0.9.4/qiskit_ibm_runtime/qpy/type_keys.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,15 +17,23 @@
 """
 
 from abc import abstractmethod
 from enum import Enum
 
 import numpy as np
 
-from qiskit.circuit import Gate, Instruction, QuantumCircuit, ControlledGate
+from qiskit.circuit import (
+    Gate,
+    Instruction,
+    QuantumCircuit,
+    ControlledGate,
+    CASE_DEFAULT,
+    Clbit,
+    ClassicalRegister,
+)
 from qiskit.circuit.library import PauliEvolutionGate
 from qiskit.circuit.parameter import Parameter
 from qiskit.circuit.parameterexpression import ParameterExpression
 from qiskit.circuit.parametervector import ParameterVectorElement
 from qiskit.pulse.channels import (
     Channel,
     DriveChannel,
@@ -41,14 +49,15 @@
     Delay,
     SetFrequency,
     ShiftFrequency,
     SetPhase,
     ShiftPhase,
     RelativeBarrier,
     TimeBlockade,
+    Reference,
 )
 from qiskit.pulse.library import Waveform, SymbolicPulse
 from qiskit.pulse.schedule import ScheduleBlock
 from qiskit.pulse.transforms.alignments import (
     AlignLeft,
     AlignRight,
     AlignSequential,
@@ -91,14 +100,16 @@
     COMPLEX = b"c"
     NUMPY_OBJ = b"n"
     PARAMETER = b"p"
     PARAMETER_VECTOR = b"v"
     PARAMETER_EXPRESSION = b"e"
     STRING = b"s"
     NULL = b"z"
+    CASE_DEFAULT = b"d"
+    REGISTER = b"R"
 
     @classmethod
     def assign(cls, obj):  # type: ignore[no-untyped-def]
         if isinstance(obj, int):
             return cls.INTEGER
         if isinstance(obj, float):
             return cls.FLOAT
@@ -110,16 +121,20 @@
             return cls.PARAMETER_VECTOR
         if isinstance(obj, Parameter):
             return cls.PARAMETER
         if isinstance(obj, ParameterExpression):
             return cls.PARAMETER_EXPRESSION
         if isinstance(obj, str):
             return cls.STRING
+        if isinstance(obj, (Clbit, ClassicalRegister)):
+            return cls.REGISTER
         if obj is None:
             return cls.NULL
+        if obj is CASE_DEFAULT:
+            return cls.CASE_DEFAULT
 
         raise exceptions.QpyError(
             f"Object type '{type(obj)}' is not supported in {cls.__name__} namespace."
         )
 
     @classmethod
     def retrieve(cls, type_key):  # type: ignore[no-untyped-def]
@@ -225,14 +240,15 @@
     DELAY = b"d"
     SET_FREQUENCY = b"f"
     SHIFT_FREQUENCY = b"g"
     SET_PHASE = b"q"
     SHIFT_PHASE = b"r"
     BARRIER = b"b"
     TIME_BLOCKADE = b"t"
+    REFERENCE = b"y"
 
     # 's' is reserved by ScheduleBlock, i.e. block can be nested as an element.
     # Call instructon is not supported by QPY.
     # This instruction has been excluded from ScheduleBlock instructions with
     # qiskit-terra/#8005 and new instruction Reference will be added instead.
     # Call is only applied to Schedule which is not supported by QPY.
     # Also snapshot is not suppored because of its limited usecase.
@@ -253,14 +269,16 @@
             return cls.SET_PHASE
         if isinstance(obj, ShiftPhase):
             return cls.SHIFT_PHASE
         if isinstance(obj, RelativeBarrier):
             return cls.BARRIER
         if isinstance(obj, TimeBlockade):
             return cls.TIME_BLOCKADE
+        if isinstance(obj, Reference):
+            return cls.REFERENCE
 
         raise exceptions.QpyError(
             f"Object type '{type(obj)}' is not supported in {cls.__name__} namespace."
         )
 
     @classmethod
     def retrieve(cls, type_key):  # type: ignore[no-untyped-def]
@@ -278,14 +296,16 @@
             return SetPhase
         if type_key == cls.SHIFT_PHASE:
             return ShiftPhase
         if type_key == cls.BARRIER:
             return RelativeBarrier
         if type_key == cls.TIME_BLOCKADE:
             return TimeBlockade
+        if type_key == cls.REFERENCE:
+            return Reference
 
         raise exceptions.QpyError(
             f"A class corresponding to type key '{type_key}' is not found in {cls.__name__} namespace."
         )
 
 
 class ScheduleOperand(TypeKeyBase):
@@ -295,14 +315,20 @@
     SYMBOLIC_PULSE = b"s"
     CHANNEL = b"c"
 
     # Discriminator and Acquire instance are not serialzied.
     # Data format of these object is somewhat opaque and not defiend well.
     # It's rarely used in the Qiskit experiements. Of course these can be added later.
 
+    # We need to have own string type definition for operands of schedule instruction.
+    # Note that string type is already defined in the Value namespace,
+    # but its key "s" conflicts with the SYMBOLIC_PULSE in the ScheduleOperand namespace.
+    # New in QPY version 7.
+    OPERAND_STR = b"o"
+
     @classmethod
     def assign(cls, obj):  # type: ignore[no-untyped-def]
         if isinstance(obj, Waveform):
             return cls.WAVEFORM
         if isinstance(obj, SymbolicPulse):
             return cls.SYMBOLIC_PULSE
         if isinstance(obj, Channel):
```

### Comparing `qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/runtime_job.py` & `qiskit-ibm-runtime-0.9.4/qiskit_ibm_runtime/runtime_job.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/runtime_options.py` & `qiskit-ibm-runtime-0.9.4/qiskit_ibm_runtime/runtime_options.py`

 * *Files 25% similar despite different names*

```diff
@@ -13,18 +13,15 @@
 """Runtime options that control the execution environment."""
 
 import re
 import logging
 from dataclasses import dataclass
 from typing import Optional, List
 
-from qiskit.utils.deprecation import deprecate_arguments
-
 from .exceptions import IBMInputValueError
-from .utils.deprecation import issue_deprecation_msg
 from .utils.utils import validate_job_tags
 
 
 @dataclass(init=False)
 class RuntimeOptions:
     """Class for representing generic runtime execution options."""
 
@@ -32,15 +29,14 @@
     image: Optional[str] = None
     log_level: Optional[str] = None
     instance: Optional[str] = None
     job_tags: Optional[List[str]] = None
     max_execution_time: Optional[int] = None
     session_time: Optional[int] = None
 
-    @deprecate_arguments({"backend_name": "backend"})
     def __init__(
         self,
         backend: Optional[str] = None,
         image: Optional[str] = None,
         log_level: Optional[str] = None,
         instance: Optional[str] = None,
         job_tags: Optional[List[str]] = None,
@@ -105,30 +101,7 @@
             raise IBMInputValueError(
                 f"{self.log_level} is not a valid log level. The valid log levels are: `DEBUG`, "
                 f"`INFO`, `WARNING`, `ERROR`, and `CRITICAL`."
             )
 
         if self.job_tags:
             validate_job_tags(self.job_tags, IBMInputValueError)
-
-    @property
-    def backend_name(self) -> str:
-        """Return backend.
-
-        Returns:
-            Backend name.
-        """
-        return self.backend
-
-    @backend_name.setter
-    def backend_name(self, name: str) -> None:
-        """Set backend name.
-
-        Args:
-            name: Backend to use.
-        """
-        issue_deprecation_msg(
-            msg="The 'backend_name' attribute is deprecated",
-            version="0.7",
-            remedy="Please use 'backend' instead.",
-        )
-        self._backend = name
```

### Comparing `qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/runtime_program.py` & `qiskit-ibm-runtime-0.9.4/qiskit_ibm_runtime/runtime_program.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/runtime_session.py` & `qiskit-ibm-runtime-0.9.4/qiskit_ibm_runtime/runtime_session.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/sampler.py` & `qiskit-ibm-runtime-0.9.4/qiskit_ibm_runtime/sampler.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,35 +10,29 @@
 # copyright notice, and modified files need to carry a notice indicating
 # that they have been altered from the originals.
 
 """Sampler primitive."""
 
 from __future__ import annotations
 import os
-from typing import Dict, Iterable, Optional, Sequence, Any, Union
+from typing import Dict, Optional, Sequence, Any, Union
 import copy
 import logging
 from dataclasses import asdict
 
-from qiskit.circuit import QuantumCircuit, Parameter
+from qiskit.circuit import QuantumCircuit
 from qiskit.providers.options import Options as TerraOptions
 from qiskit.primitives import BaseSampler, SamplerResult
 
 # TODO import _circuit_key from terra once 0.23 released
-from .qiskit_runtime_service import QiskitRuntimeService
 from .options import Options
 from .options.utils import set_default_error_levels
 from .runtime_job import RuntimeJob
 from .ibm_backend import IBMBackend
 from .session import get_default_session
-from .utils.deprecation import (
-    deprecate_arguments,
-    issue_deprecation_msg,
-    deprecate_function,
-)
 from .constants import DEFAULT_DECODERS
 
 # pylint: disable=unused-import,cyclic-import
 from .session import Session
 
 logger = logging.getLogger(__name__)
 
@@ -74,109 +68,58 @@
             session.close()
     """
 
     _PROGRAM_ID = "sampler"
 
     def __init__(
         self,
-        circuits: Optional[Union[QuantumCircuit, Iterable[QuantumCircuit]]] = None,
-        parameters: Optional[Iterable[Iterable[Parameter]]] = None,
-        service: Optional[QiskitRuntimeService] = None,
         session: Optional[Union[Session, str, IBMBackend]] = None,
         options: Optional[Union[Dict, Options]] = None,
-        skip_transpilation: Optional[bool] = False,
     ):
         """Initializes the Sampler primitive.
 
         Args:
-            circuits: (DEPRECATED) A (parameterized) :class:`~qiskit.circuit.QuantumCircuit` or
-                a list of (parameterized) :class:`~qiskit.circuit.QuantumCircuit`.
-
-            parameters: (DEPRECATED) A list of parameters of the quantum circuits
-                (:class:`~qiskit.circuit.parametertable.ParameterView` or
-                a list of :class:`~qiskit.circuit.Parameter`)
-
-            service: (DEPRECATED) Optional instance of
-                :class:`qiskit_ibm_runtime.QiskitRuntimeService` class,
-                defaults to `QiskitRuntimeService()` which tries to initialize your default
-                saved account.
-
             session: Session in which to call the primitive.
 
                 * If an instance of :class:`qiskit_ibm_runtime.IBMBackend` class or
                   string name of a backend is specified, a new session is created for
                   that backend, unless a default session for the same backend
                   and channel already exists.
 
                 * If ``None``, a new session is created using the default saved
                   account and a default backend (IBM Cloud channel only), unless
                   a default session already exists.
 
             options: Primitive options, see :class:`Options` for detailed description.
                 The ``backend`` keyword is still supported but is deprecated.
-
-            skip_transpilation (DEPRECATED): Transpilation is skipped if set to True. False by default.
-                Ignored if ``skip_transpilation`` is also specified in ``options``.
         """
         # `self._options` in this class is a Dict.
         # The base class, however, uses a `_run_options` which is an instance of
         # qiskit.providers.Options. We largely ignore this _run_options because we use
         # a nested dictionary to categorize options.
 
-        super().__init__(
-            circuits=circuits,
-            parameters=parameters,
-        )
-
-        if skip_transpilation:
-            deprecate_arguments(
-                "skip_transpilation",
-                "0.7",
-                "Instead, use the skip_transpilation keyword argument in transpilation_settings.",
-            )
-        if service:
-            deprecate_arguments(
-                "service", "0.7", "Please use the session parameter instead."
-            )
+        super().__init__()
 
         backend = None
         self._session: Session = None
 
         if options is None:
             self._options = asdict(Options())
         elif isinstance(options, Options):
-            skip_transpilation = (
-                options.transpilation.skip_transpilation  # type: ignore[union-attr]
-            )
             self._options = asdict(copy.deepcopy(options))
         else:
             options_copy = copy.deepcopy(options)
-            backend = options_copy.pop("backend", None)
-            if backend is not None:
-                issue_deprecation_msg(
-                    msg="The 'backend' key in 'options' has been deprecated",
-                    version="0.7",
-                    remedy="Please pass the backend when opening a session.",
-                )
             default_options = asdict(Options())
             self._options = Options._merge_options(default_options, options_copy)
-            skip_transpilation = self._options.get("transpilation", {}).get(
-                "skip_transpilation", False
-            )
-        self._options["transpilation"][
-            "skip_transpilation"
-        ] = skip_transpilation  # type: ignore[union-attr]
-
-        self._initial_inputs = {"circuits": circuits, "parameters": parameters}
 
         if isinstance(session, Session):
             self._session = session
         else:
             backend = session or backend
-            self._session = get_default_session(service, backend)
+            self._session = get_default_session(None, backend)
 
         # self._first_run = True
         # self._circuits_map = {}
         # if self.circuits:
         #     for circuit in self.circuits:
         #         circuit_id = _hash(
         #             json.dumps(_circuit_key(circuit), cls=RuntimeEncoder)
@@ -333,24 +276,14 @@
             program_id=self._PROGRAM_ID,
             inputs=inputs,
             options=Options._get_runtime_options(combined),
         ).result()
 
         return raw_result
 
-    @deprecate_function(
-        deprecated="close",
-        version="0.7",
-        remedy="Use qiskit_ibm_runtime.Session.close() instead",
-    )
-    def close(self) -> None:
-        """Close the session and free resources.
-        Close the session only if all jobs are finished and you don't need to run more in the session."""
-        self._session.close()
-
     @property
     def session(self) -> Session:
         """Return session used by this primitive.
 
         Returns:
             Session used by this primitive.
         """
```

### Comparing `qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/session.py` & `qiskit-ibm-runtime-0.9.4/qiskit_ibm_runtime/session.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/utils/__init__.py` & `qiskit-ibm-runtime-0.9.4/qiskit_ibm_runtime/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/utils/backend_converter.py` & `qiskit-ibm-runtime-0.9.4/qiskit_ibm_runtime/utils/backend_converter.py`

 * *Files 16% similar despite different names*

```diff
@@ -74,14 +74,18 @@
                     gates[name] = {}
             elif name not in custom_gates:
                 custom_gate = Gate(name, len(gate.qubits), [])
                 custom_gates[name] = custom_gate
                 gates[name] = {}
 
             qubits = tuple(gate.qubits)
+            if any(not properties.is_qubit_operational(qubit) for qubit in qubits):
+                continue
+            if not properties.is_gate_operational(name, gate.qubits):
+                continue
             gate_props = {}
             for param in gate.parameters:
                 if param.name == "gate_error":
                     gate_props["error"] = param.value
                 if param.name == "gate_length":
                     gate_props["duration"] = apply_prefix(param.value, param.unit)
             gates[name][qubits] = InstructionProperties(**gate_props)
@@ -90,14 +94,16 @@
                 inst = name_mapping.get(gate)
             else:
                 inst = custom_gates[gate]
             target.add_instruction(inst, props)
         # Create measurement instructions:
         measure_props = {}
         for qubit, _ in enumerate(properties.qubits):
+            if not properties.is_qubit_operational(qubit):
+                continue
             measure_props[(qubit,)] = InstructionProperties(
                 duration=properties.readout_length(qubit),
                 error=properties.readout_error(qubit),
             )
         target.add_instruction(Measure(), measure_props)
     # Parse from configuration because properties doesn't exist
     else:
@@ -124,31 +130,43 @@
         target.min_length = configuration.timing_constraints.get("min_length")
         target.pulse_alignment = configuration.timing_constraints.get("pulse_alignment")
         target.aquire_alignment = configuration.timing_constraints.get(
             "acquire_alignment"
         )
     # If pulse defaults exists use that as the source of truth
     if defaults is not None:
+        faulty_qubits = set()
+        if properties is not None:
+            faulty_qubits = set(properties.faulty_qubits())
         inst_map = defaults.instruction_schedule_map
         for inst in inst_map.instructions:
             for qarg in inst_map.qubits_with_instruction(inst):
                 sched = inst_map.get(inst, qarg)
                 if inst in target:
                     try:
                         qarg = tuple(qarg)
                     except TypeError:
                         qarg = (qarg,)
                     if inst == "measure":
                         for qubit in qarg:
+                            if qubit in faulty_qubits:
+                                continue
                             target[inst][(qubit,)].calibration = sched
                     else:
+                        if any(qubit in faulty_qubits for qubit in qarg):
+                            continue
                         target[inst][qarg].calibration = sched
     if "delay" not in target:
         target.add_instruction(
-            Delay(Parameter("t")), {(bit,): None for bit in range(target.num_qubits)}
+            Delay(Parameter("t")),
+            {
+                (bit,): None
+                for bit in range(target.num_qubits)
+                if bit not in faulty_qubits
+            },
         )
     return target
 
 
 def qubit_props_list_from_props(
     properties: BackendProperties,
 ) -> List[IBMQubitProperties]:
```

### Comparing `qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/utils/backend_decoder.py` & `qiskit-ibm-runtime-0.9.4/qiskit_ibm_runtime/utils/backend_decoder.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/utils/converters.py` & `qiskit-ibm-runtime-0.9.4/qiskit_ibm_runtime/utils/converters.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/utils/deprecation.py` & `qiskit-ibm-runtime-0.9.4/qiskit_ibm_runtime/utils/deprecation.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/utils/estimator_result_decoder.py` & `qiskit-ibm-runtime-0.9.4/qiskit_ibm_runtime/utils/estimator_result_decoder.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/utils/hgp.py` & `qiskit-ibm-runtime-0.9.4/qiskit_ibm_runtime/utils/hgp.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/utils/json.py` & `qiskit-ibm-runtime-0.9.4/qiskit_ibm_runtime/utils/json.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/utils/runner_result.py` & `qiskit-ibm-runtime-0.9.4/qiskit_ibm_runtime/utils/runner_result.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/utils/sampler_result_decoder.py` & `qiskit-ibm-runtime-0.9.4/qiskit_ibm_runtime/utils/sampler_result_decoder.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/utils/utils.py` & `qiskit-ibm-runtime-0.9.4/qiskit_ibm_runtime/utils/utils.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime/version.py` & `qiskit-ibm-runtime-0.9.4/qiskit_ibm_runtime/version.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime.egg-info/PKG-INFO` & `qiskit-ibm-runtime-0.9.4/qiskit_ibm_runtime.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qiskit-ibm-runtime
-Version: 0.9.3
+Version: 0.9.4
 Summary: IBM Quantum client for Qiskit Runtime.
 Home-page: https://github.com/Qiskit/qiskit-ibm-runtime
 Author: Qiskit Development Team
 Author-email: hello@qiskit.org
 License: Apache 2.0
 Project-URL: Bug Tracker, https://github.com/Qiskit/qiskit-ibm-runtime/issues
 Project-URL: Documentation, https://qiskit.org/documentation/
```

### Comparing `qiskit-ibm-runtime-0.9.3/qiskit_ibm_runtime.egg-info/SOURCES.txt` & `qiskit-ibm-runtime-0.9.4/qiskit_ibm_runtime.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.3/setup.py` & `qiskit-ibm-runtime-0.9.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 """Setup qiskit_ibm_runtime"""
 
 import os
 
 import setuptools
 
 REQUIREMENTS = [
-    "qiskit-terra>=0.23.1",
+    "qiskit-terra>=0.24.0",
     "requests>=2.19",
     "requests-ntlm>=1.1.0",
     "numpy<1.24",
     "urllib3>=1.21.1",
     "python-dateutil>=2.8.0",
     "websocket-client>=1.5.1",
     "typing-extensions>=4.0.0",  # remove when support for Python 3.7 is dropped (use "from typing import" instead)
```

### Comparing `qiskit-ibm-runtime-0.9.3/test/__init__.py` & `qiskit-ibm-runtime-0.9.4/test/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.3/test/account.py` & `qiskit-ibm-runtime-0.9.4/test/account.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.3/test/decorators.py` & `qiskit-ibm-runtime-0.9.4/test/decorators.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.3/test/e2e/test_tutorials.py` & `qiskit-ibm-runtime-0.9.4/test/e2e/test_tutorials.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.3/test/ibm_test_case.py` & `qiskit-ibm-runtime-0.9.4/test/ibm_test_case.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,14 @@
 import inspect
 import unittest
 from contextlib import suppress
 from collections import defaultdict
 from typing import DefaultDict, Dict
 
 from qiskit_ibm_runtime import QISKIT_IBM_RUNTIME_LOGGER_NAME
-from qiskit_ibm_runtime.exceptions import IBMNotAuthorizedError
 from qiskit_ibm_runtime import QiskitRuntimeService
 
 from .utils import setup_test_logging
 from .decorators import IntegrationTestDependencies, integration_test_setup
 from .templates import RUNTIME_PROGRAM, RUNTIME_PROGRAM_METADATA, PROGRAM_PREFIX
 
 
@@ -91,15 +90,16 @@
     def tearDown(self) -> None:
         """Test level teardown."""
         super().tearDown()
         # Delete programs
         service = self.service
         for prog in self.to_delete[service.channel]:
             with suppress(Exception):
-                service.delete_program(prog)
+                if "qiskit-test" in prog:
+                    service.delete_program(prog)
 
         # Cancel and delete jobs.
         for job in self.to_cancel[service.channel]:
             with suppress(Exception):
                 job.cancel()
             with suppress(Exception):
                 service.delete_job(job.job_id())
@@ -129,45 +129,34 @@
 
     @classmethod
     def setUpClass(cls):
         """Initial class level setup."""
         # pylint: disable=arguments-differ
         # pylint: disable=no-value-for-parameter
         super().setUpClass()
-        cls._create_default_program()
+        cls.program_ids = {}
+        cls.sim_backends = {}
+        service = cls.service
+        cls.program_ids[service.channel] = "hello-world"
         cls._find_sim_backends()
 
     @classmethod
     def tearDownClass(cls) -> None:
         """Class level teardown."""
         super().tearDownClass()
         # Delete default program.
         with suppress(Exception):
             service = cls.service
-            service.delete_program(cls.program_ids[service.channel])
-            cls.log.debug(
-                "Deleted %s program %s",
-                service.channel,
-                cls.program_ids[service.channel],
-            )
-
-    @classmethod
-    def _create_default_program(cls):
-        """Create a default program."""
-        metadata = copy.deepcopy(RUNTIME_PROGRAM_METADATA)
-        metadata["name"] = PROGRAM_PREFIX
-        cls.program_ids = {}
-        cls.sim_backends = {}
-        service = cls.service
-        try:
-            prog_id = service.upload_program(data=RUNTIME_PROGRAM, metadata=metadata)
-            cls.log.debug("Uploaded %s program %s", service.channel, prog_id)
-            cls.program_ids[service.channel] = prog_id
-        except IBMNotAuthorizedError:
-            raise unittest.SkipTest("No upload access.")
+            if "qiskit-test" in cls.program_ids[service.channel]:
+                service.delete_program(cls.program_ids[service.channel])
+                cls.log.debug(
+                    "Deleted %s program %s",
+                    service.channel,
+                    cls.program_ids[service.channel],
+                )
 
     @classmethod
     def _find_sim_backends(cls):
         """Find a simulator backend for each service."""
         cls.sim_backends[cls.service.channel] = cls.service.backends(simulator=True)[
             0
         ].name
```

### Comparing `qiskit-ibm-runtime-0.9.3/test/integration/test_account.py` & `qiskit-ibm-runtime-0.9.4/test/integration/test_account.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.3/test/integration/test_auth_client.py` & `qiskit-ibm-runtime-0.9.4/test/integration/test_auth_client.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.3/test/integration/test_backend.py` & `qiskit-ibm-runtime-0.9.4/test/integration/test_backend.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.3/test/integration/test_backend_serialization.py` & `qiskit-ibm-runtime-0.9.4/test/integration/test_backend_serialization.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.3/test/integration/test_basic_server_paths.py` & `qiskit-ibm-runtime-0.9.4/test/integration/test_basic_server_paths.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.3/test/integration/test_estimator.py` & `qiskit-ibm-runtime-0.9.4/test/integration/test_estimator.py`

 * *Files 18% similar despite different names*

```diff
@@ -200,81 +200,14 @@
                 circuits=[qc1], observables=[H], transpilation=transpilation
             )
             with self.assertRaises(RuntimeJobFailureError):
                 job.result()
             session.close()
 
     @run_integration_test
-    def test_estimator_primitive(self, service):
-        """Test to verify that estimator as a primitive still works."""
-
-        options = {
-            "backend": self.backend,
-            "optimization_level": 1,
-            "resilience_level": 0,
-        }
-
-        psi1 = RealAmplitudes(num_qubits=2, reps=2)
-        psi2 = RealAmplitudes(num_qubits=2, reps=3)
-
-        # pylint: disable=invalid-name
-        H1 = SparsePauliOp.from_list([("II", 1), ("IZ", 2), ("XI", 3)])
-        H2 = SparsePauliOp.from_list([("IZ", 1)])
-        H3 = SparsePauliOp.from_list([("ZI", 1), ("ZZ", 1)])
-
-        with Estimator(
-            circuits=[psi1, psi2],
-            observables=[H1, H2, H3],
-            service=service,
-            options=options,
-        ) as estimator:
-            self.assertIsInstance(estimator, BaseEstimator)
-
-            theta1 = [0, 1, 1, 2, 3, 5]
-            theta2 = [0, 1, 1, 2, 3, 5, 8, 13]
-            theta3 = [1, 2, 3, 4, 5, 6]
-
-            circuits1 = [0]
-            # calculate [ <psi1(theta1)|H1|psi1(theta1)> ]
-            result1 = estimator(circuits1, [0], [theta1])
-            self.assertIsInstance(result1, EstimatorResult)
-            self.assertEqual(len(result1.values), len(circuits1))
-            self.assertEqual(len(result1.metadata), len(circuits1))
-
-            circuits2 = [0, 0]
-            # calculate [ <psi1(theta1)|H2|psi1(theta1)>, <psi1(theta1)|H3|psi1(theta1)> ]
-            result2 = estimator(circuits2, [1, 2], [theta1] * 2)
-            self.assertIsInstance(result2, EstimatorResult)
-            self.assertEqual(len(result2.values), len(circuits2))
-            self.assertEqual(len(result2.metadata), len(circuits2))
-
-            circuits3 = [psi2]
-            # calculate [ <psi2(theta2)|H2|psi2(theta2)> ]
-            result3 = estimator(circuits3, [H2], [theta2])
-            self.assertIsInstance(result3, EstimatorResult)
-            self.assertEqual(len(result3.values), len(circuits3))
-            self.assertEqual(len(result3.metadata), len(circuits3))
-
-            circuits4 = [psi1, psi1]
-            # calculate [ <psi1(theta1)|H1|psi1(theta1)>, <psi1(theta3)|H1|psi1(theta3)> ]
-            result4 = estimator(circuits4, [H1, H1], [theta1, theta3])
-            self.assertIsInstance(result4, EstimatorResult)
-            self.assertEqual(len(result4.values), len(circuits4))
-            self.assertEqual(len(result4.metadata), len(circuits4))
-
-            circuits5 = [psi1, psi2, psi1]
-            # calculate [ <psi1(theta1)|H1|psi1(theta1)>,
-            #             <psi2(theta2)|H2|psi2(theta2)>,
-            #             <psi1(theta3)|H3|psi1(theta3)> ]
-            result5 = estimator(circuits5, [0, 1, 2], [theta1, theta2, theta3])
-            self.assertIsInstance(result5, EstimatorResult)
-            self.assertEqual(len(result5.values), len(circuits5))
-            self.assertEqual(len(result5.metadata), len(circuits5))
-
-    @run_integration_test
     def test_estimator_callback(self, service):
         """Test Estimator callback function."""
 
         def _callback(job_id_, result_):
             nonlocal ws_result
             ws_result.append(result_)
             nonlocal job_ids
```

### Comparing `qiskit-ibm-runtime-0.9.3/test/integration/test_job.py` & `qiskit-ibm-runtime-0.9.4/test/integration/test_job.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,46 +10,47 @@
 # copyright notice, and modified files need to carry a notice indicating
 # that they have been altered from the originals.
 
 """Tests for job functions using real runtime service."""
 
 import random
 import time
+import unittest
 
 from qiskit.providers.jobstatus import JOB_FINAL_STATES, JobStatus
 from qiskit.test.decorators import slow_test
 
 from qiskit_ibm_runtime.constants import API_TO_JOB_ERROR_MESSAGE
 from qiskit_ibm_runtime.exceptions import (
     IBMRuntimeError,
     RuntimeJobFailureError,
     RuntimeInvalidStateError,
     RuntimeJobNotFound,
     RuntimeJobMaxTimeoutError,
 )
 from ..ibm_test_case import IBMIntegrationJobTestCase
-from ..decorators import run_integration_test, production_only
+from ..decorators import run_integration_test, production_only, quantum_only
 from ..serialization import (
     get_complex_types,
     SerializableClassDecoder,
     SerializableClass,
 )
 from ..utils import cancel_job_safe, wait_for_status, get_real_device
 
 
 class TestIntegrationJob(IBMIntegrationJobTestCase):
     """Integration tests for job functions."""
 
     @run_integration_test
     def test_run_program(self, service):
         """Test running a program."""
-        job = self._run_program(service, final_result="foo")
+        job = self._run_program(service)
         result = job.result()
         self.assertEqual(JobStatus.DONE, job.status())
-        self.assertEqual("foo", result)
+        self.assertEqual("Hello, World!", result)
 
     @slow_test
     @run_integration_test
     def test_run_program_real_device(self, service):
         """Test running a program."""
         device = get_real_device(service)
         job = self._run_program(service, final_result="foo", backend=device)
@@ -72,35 +73,37 @@
         """Test running with a custom log level."""
         levels = ["INFO", "ERROR"]
         for level in levels:
             with self.subTest(level=level):
                 job = self._run_program(service, log_level=level)
                 job.wait_for_final_state()
                 expect_info_msg = level == "INFO"
-                self.assertEqual(
-                    "info log" in job.logs(),
-                    expect_info_msg,
-                    f"Job log is {job.logs()}",
-                )
+                if job.logs():
+                    self.assertEqual(
+                        "INFO Pass" in job.logs(),
+                        expect_info_msg,
+                        f"Job log is {job.logs()}",
+                    )
 
     @run_integration_test
+    @quantum_only
     def test_run_program_failed(self, service):
         """Test a failed program execution."""
-        job = self._run_program(service, inputs={})
+        job = self._run_program(service, program_id="circuit-runner", inputs={})
         job.wait_for_final_state()
         self.assertEqual(JobStatus.ERROR, job.status())
         self.assertIn(
             API_TO_JOB_ERROR_MESSAGE["FAILED"].format(job.job_id(), ""),
             job.error_message(),
         )
-        with self.assertRaises(RuntimeJobFailureError):
+        with self.assertRaises(RuntimeJobFailureError) as err_cm:
             job.result()
-        # TODO: Re-enable when ntc-1651 is fixed
-        # self.assertIn("KeyError", str(err_cm.exception))
+            self.assertIn("KeyError", str(err_cm.exception))
 
+    @unittest.skip("Custom programs not currently supported.")
     @run_integration_test
     def test_run_program_failed_ran_too_long(self, service):
         """Test a program that failed since it ran longer than maximum execution time."""
         max_execution_time = 60
         inputs = {"iterations": 1, "sleep_per_iteration": 61}
         program_id = self._upload_program(
             service, max_execution_time=max_execution_time
@@ -115,14 +118,15 @@
                 job.job_id(), job_result_raw
             ),
             job.error_message(),
         )
         with self.assertRaises(RuntimeJobMaxTimeoutError):
             job.result()
 
+    @unittest.skip("Custom programs not currently supported.")
     @run_integration_test
     def test_run_program_override_max_execution_time(self, service):
         """Test that the program max execution time is overridden."""
         program_max_execution_time = 400
         job_max_execution_time = 350
         program_id = self._upload_program(
             service, max_execution_time=program_max_execution_time
@@ -147,15 +151,15 @@
         """Test canceling a queued job."""
         real_device = get_real_device(service)
         _ = self._run_program(service, iterations=10, backend=real_device)
         job = self._run_program(service, iterations=2, backend=real_device)
         wait_for_status(job, JobStatus.QUEUED)
         if not cancel_job_safe(job, self.log):
             return
-        time.sleep(10)  # Wait a bit for DB to update.
+        time.sleep(15)  # Wait a bit for DB to update.
         rjob = service.job(job.job_id())
         self.assertEqual(rjob.status(), JobStatus.CANCELLED)
 
     @run_integration_test
     def test_cancel_job_running(self, service):
         """Test canceling a running job."""
         job = self._run_program(service, iterations=3)
@@ -194,14 +198,15 @@
         _ = self._run_program(service, iterations=10, backend=real_device)
         job = self._run_program(service, iterations=2, backend=real_device)
         wait_for_status(job, JobStatus.QUEUED)
         service.delete_job(job.job_id())
         with self.assertRaises(RuntimeJobNotFound):
             service.job(job.job_id())
 
+    @unittest.skip("Final result only supported in custom programs.")
     @run_integration_test
     def test_final_result(self, service):
         """Test getting final result."""
         final_result = get_complex_types()
         job = self._run_program(service, final_result=final_result)
         result = job.result(decoder=SerializableClassDecoder)
         self.assertEqual(final_result, result)
@@ -238,22 +243,22 @@
         """Test job program ID."""
         job = self._run_program(service)
         self.assertEqual(self.program_ids[service.channel], job.program_id)
 
     @run_integration_test
     def test_wait_for_final_state(self, service):
         """Test wait for final state."""
-        job = self._run_program(service)
+        job = self._run_program(service, backend="ibmq_qasm_simulator")
         job.wait_for_final_state()
         self.assertEqual(JobStatus.DONE, job.status())
 
     @run_integration_test
     def test_wait_for_final_state_after_job_status(self, service):
         """Test wait for final state on a completed job when the status is updated first."""
-        job = self._run_program(service)
+        job = self._run_program(service, backend="ibmq_qasm_simulator")
         status = job.status()
         while status not in JOB_FINAL_STATES:
             status = job.status()
         job.wait_for_final_state()
         self.assertEqual(JobStatus.DONE, job.status())
 
     @run_integration_test
@@ -266,21 +271,21 @@
         rjobs = service.jobs(limit=2)
         for rjob in rjobs:
             self.assertTrue(rjob.creation_date)
 
     @run_integration_test
     def test_job_logs(self, service):
         """Test job logs."""
-        job = self._run_program(service, final_result="foo")
+        job = self._run_program(service)
         with self.assertLogs("qiskit_ibm_runtime", "WARN"):
             job.logs()
         job.wait_for_final_state()
         job_logs = job.logs()
-        self.assertIn("this is a stdout message", job_logs)
-        self.assertIn("this is a stderr message", job_logs)
+        if job_logs:
+            self.assertIn("INFO Pass", job_logs)
 
     @run_integration_test
     def test_job_metrics(self, service):
         """Test job metrics."""
         job = self._run_program(service)
         job.wait_for_final_state()
         metrics = job.metrics()
```

### Comparing `qiskit-ibm-runtime-0.9.3/test/integration/test_options.py` & `qiskit-ibm-runtime-0.9.4/test/integration/test_options.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.3/test/integration/test_program.py` & `qiskit-ibm-runtime-0.9.4/test/integration/test_program.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.3/test/integration/test_proxies.py` & `qiskit-ibm-runtime-0.9.4/test/integration/test_proxies.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.3/test/integration/test_results.py` & `qiskit-ibm-runtime-0.9.4/test/integration/test_results.py`

 * *Files 2% similar despite different names*

```diff
@@ -134,19 +134,19 @@
         # Callback is expected twice because both interim and final results are returned
         self.assertEqual(2, called_back_count)
         self.assertIsNotNone(job._ws_client._server_close_code)
 
     @run_integration_test
     def test_retrieve_interim_results(self, service):
         """Test retrieving interim results with API endpoint"""
-        int_res = "foo"
-        job = self._run_program(service, interim_results=int_res)
+        job = self._run_program(service)
         job.wait_for_final_state()
         interim_results = job.interim_results()
-        self.assertIn(int_res, interim_results[0])
+        self.assertIn("iteration", interim_results[0])
+        self.assertIn("counts", interim_results[0])
 
     @run_integration_test
     def test_result_timeout(self, service):
         """Test job result timeout"""
         job = self._run_program(service)
         with self.assertRaises(RuntimeJobTimeoutError):
             job.result(0.1)
```

### Comparing `qiskit-ibm-runtime-0.9.3/test/integration/test_retrieve_job.py` & `qiskit-ibm-runtime-0.9.4/test/integration/test_retrieve_job.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 """Tests for job functions using real runtime service."""
 
 import uuid
 from datetime import datetime, timezone
 from qiskit.providers.jobstatus import JobStatus
 
 from ..ibm_test_case import IBMIntegrationJobTestCase
-from ..decorators import run_integration_test, production_only
+from ..decorators import run_integration_test, production_only, quantum_only
 from ..utils import wait_for_status, get_real_device
 
 
 class TestIntegrationRetrieveJob(IBMIntegrationJobTestCase):
     """Integration tests for job retrieval functions."""
 
     @run_integration_test
@@ -84,15 +84,15 @@
         self.assertTrue(
             rjob_ids.issubset(job_ids), f"Submitted: {job_ids}, Retrieved: {rjob_ids}"
         )
 
     @run_integration_test
     def test_retrieve_pending_jobs(self, service):
         """Test retrieving pending jobs (QUEUED, RUNNING)."""
-        job = self._run_program(service, iterations=10)
+        job = self._run_program(service, iterations=20)
         wait_for_status(job, JobStatus.RUNNING)
         rjobs = service.jobs(pending=True)
         after_status = job.status()
         found = False
         for rjob in rjobs:
             if rjob.job_id() == job.job_id():
                 self.assertEqual(job.program_id, rjob.program_id)
@@ -117,24 +117,21 @@
                 self.assertEqual(job.program_id, rjob.program_id)
                 self.assertEqual(job.inputs, rjob.inputs)
                 found = True
                 break
         self.assertTrue(found, f"Returned job {job.job_id()} not retrieved.")
 
     @run_integration_test
+    @quantum_only
     def test_retrieve_jobs_by_program_id(self, service):
         """Test retrieving jobs by Program ID."""
-        program_id = self._upload_program(service)
-        job = self._run_program(service, program_id=program_id)
-        job.wait_for_final_state()
-        rjobs = service.jobs(program_id=program_id)
-        self.assertEqual(program_id, rjobs[0].program_id)
-        self.assertEqual(
-            1, len(rjobs), f"Retrieved jobs: {[j.job_id() for j in rjobs]}"
-        )
+        program_id = "hello-world"
+        jobs = service.jobs(program_id=program_id)
+        for job in jobs:
+            self.assertEqual(program_id, job.program_id)
 
     @run_integration_test
     def test_retrieve_jobs_by_job_tags(self, service):
         """Test retrieving jobs by job_tags."""
         job_tags = ["test_tag"]
         job = self._run_program(service, job_tags=job_tags)
         job.wait_for_final_state()
@@ -175,26 +172,24 @@
     @run_integration_test
     def test_jobs_filter_by_hgp(self, service):
         """Test retrieving jobs by hgp."""
         if self.dependencies.channel == "ibm_cloud":
             self.skipTest("Not supported on ibm_cloud")
 
         default_hgp = list(service._hgps.keys())[0]
-        program_id = self._upload_program(service)
-        job = self._run_program(service, program_id=program_id)
+
+        job = self._run_program(service)
         job.wait_for_final_state()
-        rjobs = service.jobs(program_id=program_id, instance=default_hgp)
-        self.assertEqual(program_id, rjobs[0].program_id)
-        self.assertEqual(
-            1, len(rjobs), f"Retrieved jobs: {[j.job_id() for j in rjobs]}"
-        )
+        rjobs = service.jobs(instance=default_hgp)
+
+        self.assertIn(job.job_id(), [j.job_id() for j in rjobs])
 
         uuid_ = uuid.uuid4().hex
         fake_hgp = f"{uuid_}/{uuid_}/{uuid_}"
-        rjobs = service.jobs(program_id=program_id, instance=fake_hgp)
+        rjobs = service.jobs(instance=fake_hgp)
         self.assertFalse(rjobs)
 
     @run_integration_test
     def test_retrieve_jobs_sorted_by_date(self, service):
         """Test retrieving jobs sorted by the date."""
         job = self._run_program(service)
         job.wait_for_final_state()
```

### Comparing `qiskit-ibm-runtime-0.9.3/test/integration/test_sampler.py` & `qiskit-ibm-runtime-0.9.4/test/integration/test_sampler.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,32 +33,14 @@
 
     def setUp(self) -> None:
         super().setUp()
         self.bell = ReferenceCircuits.bell()
         self.backend = "ibmq_qasm_simulator"
 
     @run_integration_test
-    def test_sampler_non_parameterized_single_circuit(self, service):
-        """Verify if sampler primitive returns expected results for non-parameterized circuits."""
-
-        # Execute a Bell circuit
-        with Session(service, self.backend) as session:
-            sampler = Sampler(session=session)
-            self.assertIsInstance(sampler, BaseSampler)
-            job = sampler.run(circuits=self.bell)
-            result = job.result()
-            self.assertIsInstance(result, SamplerResult)
-            self.assertEqual(len(result.quasi_dists), 1)
-            self.assertEqual(len(result.metadata), 1)
-            self.assertAlmostEqual(result.quasi_dists[0][3], 0.5, delta=0.1)
-            self.assertAlmostEqual(result.quasi_dists[0][0], 0.5, delta=0.1)
-            self.assertTrue(session.session_id)
-            session.close()
-
-    @run_integration_test
     def test_sampler_non_parameterized_circuits(self, service):
         """Test sampler with multiple non-parameterized circuits."""
         # Execute three Bell circuits
         with Session(service, self.backend) as session:
             sampler = Sampler(session=session)
             self.assertIsInstance(sampler, BaseSampler)
             circuits = [self.bell] * 3
@@ -227,44 +209,14 @@
                 result.quasi_dists[0]._stddev_upper_bound, sqrt(1 / shots), delta=0.1
             )
             self.assertAlmostEqual(result.quasi_dists[0][3], 0.5, delta=0.1)
             self.assertAlmostEqual(result.quasi_dists[0][0], 0.5, delta=0.1)
             session.close()
 
     @run_integration_test
-    def test_sampler_primitive_as_session(self, service):
-        """Verify Sampler as a session still works."""
-
-        # parameterized circuit
-        pqc = RealAmplitudes(num_qubits=2, reps=2)
-        pqc.measure_all()
-        pqc2 = RealAmplitudes(num_qubits=2, reps=3)
-        pqc2.measure_all()
-
-        theta1 = [0, 1, 1, 2, 3, 5]
-        theta2 = [1, 2, 3, 4, 5, 6]
-        theta3 = [0, 1, 2, 3, 4, 5, 6, 7]
-
-        with Sampler(
-            circuits=[pqc, pqc2],
-            service=service,
-            options={"backend": "ibmq_qasm_simulator", "optimization_level": 1},
-        ) as sampler:
-            self.assertIsInstance(sampler, BaseSampler)
-
-            circuits0 = [pqc, pqc, pqc2]
-            result = sampler(
-                circuits=circuits0,
-                parameter_values=[theta1, theta2, theta3],
-            )
-            self.assertIsInstance(result, SamplerResult)
-            self.assertEqual(len(result.quasi_dists), len(circuits0))
-            self.assertEqual(len(result.metadata), len(circuits0))
-
-    @run_integration_test
     def test_sampler_callback(self, service):
         """Test Sampler callback function."""
 
         def _callback(job_id_, result_):
             nonlocal ws_result
             ws_result.append(result_)
             nonlocal job_ids
```

### Comparing `qiskit-ibm-runtime-0.9.3/test/integration/test_session.py` & `qiskit-ibm-runtime-0.9.4/test/integration/test_session.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.3/test/program.py` & `qiskit-ibm-runtime-0.9.4/test/program.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.3/test/serialization.py` & `qiskit-ibm-runtime-0.9.4/test/serialization.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.3/test/templates.py` & `qiskit-ibm-runtime-0.9.4/test/templates.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.3/test/unit/mock/fake_api_backend.py` & `qiskit-ibm-runtime-0.9.4/test/unit/mock/fake_api_backend.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.3/test/unit/mock/fake_quantum_auth_client.py` & `qiskit-ibm-runtime-0.9.4/test/unit/mock/fake_quantum_auth_client.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.3/test/unit/mock/fake_runtime_client.py` & `qiskit-ibm-runtime-0.9.4/test/unit/mock/fake_runtime_client.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.3/test/unit/mock/fake_runtime_service.py` & `qiskit-ibm-runtime-0.9.4/test/unit/mock/fake_runtime_service.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.3/test/unit/mock/http_server.py` & `qiskit-ibm-runtime-0.9.4/test/unit/mock/http_server.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.3/test/unit/mock/proxy_server.py` & `qiskit-ibm-runtime-0.9.4/test/unit/mock/proxy_server.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.3/test/unit/mock/ws_handler.py` & `qiskit-ibm-runtime-0.9.4/test/unit/mock/ws_handler.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.3/test/unit/mock/ws_server.py` & `qiskit-ibm-runtime-0.9.4/test/unit/mock/ws_server.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.3/test/unit/test_account.py` & `qiskit-ibm-runtime-0.9.4/test/unit/test_account.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.3/test/unit/test_backend_retrieval.py` & `qiskit-ibm-runtime-0.9.4/test/unit/test_backend_retrieval.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.3/test/unit/test_client_parameters.py` & `qiskit-ibm-runtime-0.9.4/test/unit/test_client_parameters.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.3/test/unit/test_data_serialization.py` & `qiskit-ibm-runtime-0.9.4/test/unit/test_data_serialization.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.3/test/unit/test_estimator.py` & `qiskit-ibm-runtime-0.9.4/test/unit/test_estimator.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.3/test/unit/test_ibm_primitives.py` & `qiskit-ibm-runtime-0.9.4/test/unit/test_ibm_primitives.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,40 +66,14 @@
         cls.obs = SparsePauliOp.from_list([("IZ", 1)])
         return super().setUpClass()
 
     def tearDown(self) -> None:
         super().tearDown()
         session_pkg._DEFAULT_SESSION.set(None)
 
-    def test_skip_transpilation(self):
-        """Test skip_transpilation is hornored."""
-        primitives = [Sampler, Estimator]
-        for cls in primitives:
-            with self.subTest(primitive=cls):
-                inst = cls(session=MagicMock(spec=MockSession), skip_transpilation=True)
-                self.assertTrue(
-                    inst.options.get("transpilation").get("skip_transpilation")
-                )
-
-    def test_skip_transpilation_overwrite(self):
-        """Test overwriting skip_transpilation."""
-        options = Options()
-        options.transpilation.skip_transpilation = False
-        primitives = [Sampler, Estimator]
-        for cls in primitives:
-            with self.subTest(primitive=cls):
-                inst = cls(
-                    session=MagicMock(spec=MockSession),
-                    options=options,
-                    skip_transpilation=True,
-                )
-                self.assertFalse(
-                    inst.options.get("transpilation").get("skip_transpilation")
-                )
-
     def test_dict_options(self):
         """Test passing a dictionary as options."""
         options_vars = [
             {},
             {
                 "resilience_level": 1,
                 "transpilation": {"initial_layout": [1, 2]},
@@ -127,43 +101,21 @@
         backends = [backend_name, backend]
         for cls in primitives:
             for backend in backends:
                 with self.subTest(primitive=cls, backend=backend):
                     options = {"backend": backend}
                     with warnings.catch_warnings(record=True) as warn:
                         warnings.simplefilter("always")
-                        inst = cls(service=MagicMock(), options=options)
-                        # We'll get 2 deprecation warnings - one for service and one for backend.
-                        # We need service otherwise backend will get ignored.
-                        self.assertEqual(len(warn), 2)
+                        cls(session=MagicMock(spec=MockSession), options=options)
                         self.assertTrue(
                             all(
                                 issubclass(one_warn.category, DeprecationWarning)
                                 for one_warn in warn
                             )
                         )
-                    self.assertEqual(inst.session.backend(), backend_name)
-
-    def test_old_options(self):
-        """Test specifying old runtime options."""
-        primitives = [Sampler, Estimator]
-        session = MagicMock(spec=MockSession)
-        options = [{"log_level": "WARNING"}, {"image": "foo:bar"}]
-
-        for cls in primitives:
-            for opt in options:
-                with self.subTest(primitive=cls, options=opt):
-                    inst = cls(session=session, options=opt)
-                    inst.run(self.qx, observables=self.obs)
-                    _, kwargs = session.run.call_args
-                    run_options = kwargs["options"]
-                    for key, val in opt.items():
-                        self.assertEqual(run_options[key], val)
-                    inputs = kwargs["inputs"]
-                    self.assertTrue(all(key not in inputs.keys() for key in opt))
 
     def test_runtime_options(self):
         """Test RuntimeOptions specified as primitive options."""
         session = MagicMock(spec=MockSession)
         primitives = [Sampler, Estimator]
         env_vars = [
             {"log_level": "DEBUG"},
@@ -207,20 +159,18 @@
             self.assertEqual(estimator.session, sampler.session)
         finally:
             # Ensure it's cleaned up or next test will fail.
             session_pkg._DEFAULT_SESSION.set(None)
 
     def test_default_session_after_close(self):
         """Test a new default session is open after previous is closed."""
-        service = MagicMock()
-        sampler = Sampler(service=service)
+        sampler = Sampler(session=MagicMock(spec=MockSession))
         sampler.session.close()
-        estimator = Estimator(service=service)
+        estimator = Estimator(session=MagicMock(spec=MockSession))
         self.assertIsNotNone(estimator.session)
-        self.assertTrue(estimator.session._active)
         self.assertNotEqual(estimator.session, sampler.session)
 
     @patch("qiskit_ibm_runtime.session.Session")
     @patch("qiskit_ibm_runtime.session.QiskitRuntimeService")
     def test_backend_str_as_session(self, _, mock_session):
         """Test specifying a backend name as session."""
         primitives = [Sampler, Estimator]
@@ -674,14 +624,66 @@
                     list(opts_dict["resilience"].values())[0], str(exc.exception)
                 )
                 if len(opts_dict["resilience"].keys()) > 1:
                     self.assertIn(
                         list(opts_dict["resilience"].keys())[1], str(exc.exception)
                     )
 
+    def test_environment_options(self):
+        """Test environment options."""
+        options_dicts = [
+            {"environment": {"log_level": "NoLogLevel"}},
+        ]
+        session = MagicMock(spec=MockSession)
+        primitives = [Sampler, Estimator]
+
+        for cls in primitives:
+            for opts_dict in options_dicts:
+                # When this environment variable is set, validation is turned off
+                try:
+                    os.environ["QISKIT_RUNTIME_SKIP_OPTIONS_VALIDATION"] = "1"
+                    inst = cls(session=session, options=opts_dict)
+                    inst.run(self.qx, observables=self.obs)
+                finally:
+                    # Delete environment variable to validate input
+                    del os.environ["QISKIT_RUNTIME_SKIP_OPTIONS_VALIDATION"]
+                with self.assertRaises(ValueError) as exc:
+                    inst = cls(session=session, options=opts_dict)
+                    inst.run(self.qx, observables=self.obs)
+                self.assertIn(
+                    list(opts_dict["environment"].values())[0], str(exc.exception)
+                )
+
+    def test_transpilation_options(self):
+        """Test transpilation options."""
+        options_dicts = [
+            {"transpilation": {"layout_method": "NoLayoutMethod"}},
+            {"transpilation": {"routing_method": "NoRoutingMethod"}},
+            {"transpilation": {"approximation_degree": 1.1}},
+        ]
+        session = MagicMock(spec=MockSession)
+        primitives = [Sampler, Estimator]
+
+        for cls in primitives:
+            for opts_dict in options_dicts:
+                # When this environment variable is set, validation is turned off
+                try:
+                    os.environ["QISKIT_RUNTIME_SKIP_OPTIONS_VALIDATION"] = "1"
+                    inst = cls(session=session, options=opts_dict)
+                    inst.run(self.qx, observables=self.obs)
+                finally:
+                    # Delete environment variable to validate input
+                    del os.environ["QISKIT_RUNTIME_SKIP_OPTIONS_VALIDATION"]
+                with self.assertRaises(ValueError) as exc:
+                    inst = cls(session=session, options=opts_dict)
+                    inst.run(self.qx, observables=self.obs)
+                self.assertIn(
+                    list(opts_dict["transpilation"].keys())[0], str(exc.exception)
+                )
+
     def test_raise_faulty_qubits(self):
         """Test faulty qubits is raised."""
         fake_backend = FakeManila()
         num_qubits = fake_backend.configuration().num_qubits
         circ = QuantumCircuit(num_qubits, num_qubits)
         for i in range(num_qubits):
             circ.x(i)
```

### Comparing `qiskit-ibm-runtime-0.9.3/test/unit/test_job_retrieval.py` & `qiskit-ibm-runtime-0.9.4/test/unit/test_job_retrieval.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.3/test/unit/test_jobs.py` & `qiskit-ibm-runtime-0.9.4/test/unit/test_jobs.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.3/test/unit/test_logger.py` & `qiskit-ibm-runtime-0.9.4/test/unit/test_logger.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.3/test/unit/test_options.py` & `qiskit-ibm-runtime-0.9.4/test/unit/test_options.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.3/test/unit/test_programs.py` & `qiskit-ibm-runtime-0.9.4/test/unit/test_programs.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.3/test/unit/test_runtime_client.py` & `qiskit-ibm-runtime-0.9.4/test/unit/test_runtime_client.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.3/test/unit/test_runtime_ws.py` & `qiskit-ibm-runtime-0.9.4/test/unit/test_runtime_ws.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.3/test/unit/test_sampler.py` & `qiskit-ibm-runtime-0.9.4/test/unit/test_sampler.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.3/test/unit/test_session.py` & `qiskit-ibm-runtime-0.9.4/test/unit/test_session.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.3/test/unit/test_utils_converters.py` & `qiskit-ibm-runtime-0.9.4/test/unit/test_utils_converters.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-runtime-0.9.3/test/utils.py` & `qiskit-ibm-runtime-0.9.4/test/utils.py`

 * *Files identical despite different names*

