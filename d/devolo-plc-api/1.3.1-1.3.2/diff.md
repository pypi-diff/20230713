# Comparing `tmp/devolo_plc_api-1.3.1.tar.gz` & `tmp/devolo_plc_api-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "devolo_plc_api-1.3.1.tar", last modified: Fri May 12 13:38:19 2023, max compression
+gzip compressed data, was "devolo_plc_api-1.3.2.tar", last modified: Thu Jul 13 19:54:47 2023, max compression
```

## Comparing `devolo_plc_api-1.3.1.tar` & `devolo_plc_api-1.3.2.tar`

### file list

```diff
@@ -1,95 +1,95 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:38:19.842818 devolo_plc_api-1.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-12 13:38:03.000000 devolo_plc_api-1.3.1/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:38:19.834818 devolo_plc_api-1.3.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:38:19.834818 devolo_plc_api-1.3.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-05-12 13:38:03.000000 devolo_plc_api-1.3.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-12 13:38:03.000000 devolo_plc_api-1.3.1/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-05-12 13:38:03.000000 devolo_plc_api-1.3.1/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-05-12 13:38:03.000000 devolo_plc_api-1.3.1/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:38:19.834818 devolo_plc_api-1.3.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-12 13:38:03.000000 devolo_plc_api-1.3.1/.github/workflows/convert_todos_to_issues.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-05-12 13:38:03.000000 devolo_plc_api-1.3.1/.github/workflows/pythonpackage.yml
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-12 13:38:03.000000 devolo_plc_api-1.3.1/.github/workflows/pythonpublish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-05-12 13:38:03.000000 devolo_plc_api-1.3.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-05-12 13:38:03.000000 devolo_plc_api-1.3.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-12 13:38:03.000000 devolo_plc_api-1.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    44988 2023-05-12 13:38:19.842818 devolo_plc_api-1.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3811 2023-05-12 13:38:03.000000 devolo_plc_api-1.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:38:19.834818 devolo_plc_api-1.3.1/devolo_plc_api/
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-12 13:38:03.000000 devolo_plc_api-1.3.1/devolo_plc_api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:38:19.834818 devolo_plc_api-1.3.1/devolo_plc_api/clients/
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-12 13:38:03.000000 devolo_plc_api-1.3.1/devolo_plc_api/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3366 2023-05-12 13:38:03.000000 devolo_plc_api-1.3.1/devolo_plc_api/clients/protobuf.py
--rw-r--r--   0 runner    (1001) docker     (123)    11471 2023-05-12 13:38:03.000000 devolo_plc_api-1.3.1/devolo_plc_api/device.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:38:19.838818 devolo_plc_api-1.3.1/devolo_plc_api/device_api/
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-05-12 13:38:03.000000 devolo_plc_api-1.3.1/devolo_plc_api/device_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12407 2023-05-12 13:38:03.000000 devolo_plc_api-1.3.1/devolo_plc_api/device_api/deviceapi.py
--rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-05-12 13:38:03.000000 devolo_plc_api-1.3.1/devolo_plc_api/device_api/deviceapi.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-05-12 13:38:03.000000 devolo_plc_api-1.3.1/devolo_plc_api/device_api/factoryreset_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-05-12 13:38:03.000000 devolo_plc_api-1.3.1/devolo_plc_api/device_api/factoryreset_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3269 2023-05-12 13:38:03.000000 devolo_plc_api-1.3.1/devolo_plc_api/device_api/ledsettings_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4009 2023-05-12 13:38:03.000000 devolo_plc_api-1.3.1/devolo_plc_api/device_api/ledsettings_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-05-12 13:38:03.000000 devolo_plc_api-1.3.1/devolo_plc_api/device_api/multiap_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-05-12 13:38:03.000000 devolo_plc_api-1.3.1/devolo_plc_api/device_api/multiap_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-05-12 13:38:03.000000 devolo_plc_api-1.3.1/devolo_plc_api/device_api/restart_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-05-12 13:38:03.000000 devolo_plc_api-1.3.1/devolo_plc_api/device_api/restart_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3029 2023-05-12 13:38:03.000000 devolo_plc_api-1.3.1/devolo_plc_api/device_api/support_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4557 2023-05-12 13:38:03.000000 devolo_plc_api-1.3.1/devolo_plc_api/device_api/support_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-05-12 13:38:03.000000 devolo_plc_api-1.3.1/devolo_plc_api/device_api/updatefirmware_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3535 2023-05-12 13:38:03.000000 devolo_plc_api-1.3.1/devolo_plc_api/device_api/updatefirmware_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    15720 2023-05-12 13:38:03.000000 devolo_plc_api-1.3.1/devolo_plc_api/device_api/wifinetwork_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    19608 2023-05-12 13:38:03.000000 devolo_plc_api-1.3.1/devolo_plc_api/device_api/wifinetwork_pb2.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:38:19.838818 devolo_plc_api-1.3.1/devolo_plc_api/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-12 13:38:03.000000 devolo_plc_api-1.3.1/devolo_plc_api/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-05-12 13:38:03.000000 devolo_plc_api-1.3.1/devolo_plc_api/exceptions/device.py
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-05-12 13:38:03.000000 devolo_plc_api-1.3.1/devolo_plc_api/exceptions/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:38:19.838818 devolo_plc_api-1.3.1/devolo_plc_api/network/
--rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-05-12 13:38:03.000000 devolo_plc_api-1.3.1/devolo_plc_api/network/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:38:19.838818 devolo_plc_api-1.3.1/devolo_plc_api/plcnet_api/
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-05-12 13:38:03.000000 devolo_plc_api-1.3.1/devolo_plc_api/plcnet_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4782 2023-05-12 13:38:03.000000 devolo_plc_api-1.3.1/devolo_plc_api/plcnet_api/getnetworkoverview_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     9456 2023-05-12 13:38:03.000000 devolo_plc_api-1.3.1/devolo_plc_api/plcnet_api/getnetworkoverview_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-05-12 13:38:03.000000 devolo_plc_api-1.3.1/devolo_plc_api/plcnet_api/identifydevice_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-05-12 13:38:03.000000 devolo_plc_api-1.3.1/devolo_plc_api/plcnet_api/identifydevice_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-05-12 13:38:03.000000 devolo_plc_api-1.3.1/devolo_plc_api/plcnet_api/pairdevice_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-05-12 13:38:03.000000 devolo_plc_api-1.3.1/devolo_plc_api/plcnet_api/pairdevice_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4120 2023-05-12 13:38:03.000000 devolo_plc_api-1.3.1/devolo_plc_api/plcnet_api/plcnetapi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-12 13:38:03.000000 devolo_plc_api-1.3.1/devolo_plc_api/plcnet_api/plcnetapi.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-05-12 13:38:03.000000 devolo_plc_api-1.3.1/devolo_plc_api/plcnet_api/setuserdevicename_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-05-12 13:38:03.000000 devolo_plc_api-1.3.1/devolo_plc_api/plcnet_api/setuserdevicename_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 13:38:03.000000 devolo_plc_api-1.3.1/devolo_plc_api/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:38:19.838818 devolo_plc_api-1.3.1/devolo_plc_api/zeroconf/
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-05-12 13:38:03.000000 devolo_plc_api-1.3.1/devolo_plc_api/zeroconf/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:38:19.834818 devolo_plc_api-1.3.1/devolo_plc_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    44988 2023-05-12 13:38:19.000000 devolo_plc_api-1.3.1/devolo_plc_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-05-12 13:38:19.000000 devolo_plc_api-1.3.1/devolo_plc_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 13:38:19.000000 devolo_plc_api-1.3.1/devolo_plc_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-12 13:38:19.000000 devolo_plc_api-1.3.1/devolo_plc_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-12 13:38:19.000000 devolo_plc_api-1.3.1/devolo_plc_api.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:38:19.838818 devolo_plc_api-1.3.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     4496 2023-05-12 13:38:03.000000 devolo_plc_api-1.3.1/docs/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     3372 2023-05-12 13:38:03.000000 devolo_plc_api-1.3.1/docs/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-05-12 13:38:03.000000 devolo_plc_api-1.3.1/docs/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     7086 2023-05-12 13:38:03.000000 devolo_plc_api-1.3.1/example_async.py
--rw-r--r--   0 runner    (1001) docker     (123)     6805 2023-05-12 13:38:03.000000 devolo_plc_api-1.3.1/example_sync.py
--rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-05-12 13:38:03.000000 devolo_plc_api-1.3.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:38:19.838818 devolo_plc_api-1.3.1/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)     4419 2023-05-12 13:38:03.000000 devolo_plc_api-1.3.1/scripts/stubgen.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 13:38:19.842818 devolo_plc_api-1.3.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:38:19.838818 devolo_plc_api-1.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-05-12 13:38:03.000000 devolo_plc_api-1.3.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2618 2023-05-12 13:38:03.000000 devolo_plc_api-1.3.1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:38:19.838818 devolo_plc_api-1.3.1/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-12 13:38:03.000000 devolo_plc_api-1.3.1/tests/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-05-12 13:38:03.000000 devolo_plc_api-1.3.1/tests/fixtures/device_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-05-12 13:38:03.000000 devolo_plc_api-1.3.1/tests/fixtures/plcnet_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:38:19.838818 devolo_plc_api-1.3.1/tests/mocks/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-12 13:38:03.000000 devolo_plc_api-1.3.1/tests/mocks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-05-12 13:38:03.000000 devolo_plc_api-1.3.1/tests/mocks/zeroconf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:38:19.842818 devolo_plc_api-1.3.1/tests/snapshots/
--rw-r--r--   0 runner    (1001) docker     (123)     3105 2023-05-12 13:38:03.000000 devolo_plc_api-1.3.1/tests/snapshots/test_device.ambr
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-05-12 13:38:03.000000 devolo_plc_api-1.3.1/tests/test_data.json
--rw-r--r--   0 runner    (1001) docker     (123)     6840 2023-05-12 13:38:03.000000 devolo_plc_api-1.3.1/tests/test_device.py
--rw-r--r--   0 runner    (1001) docker     (123)    18393 2023-05-12 13:38:03.000000 devolo_plc_api-1.3.1/tests/test_deviceapi.py
--rw-r--r--   0 runner    (1001) docker     (123)     3365 2023-05-12 13:38:03.000000 devolo_plc_api-1.3.1/tests/test_network.py
--rw-r--r--   0 runner    (1001) docker     (123)     6530 2023-05-12 13:38:03.000000 devolo_plc_api-1.3.1/tests/test_plcnetapi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:54:47.509129 devolo_plc_api-1.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-13 19:54:25.000000 devolo_plc_api-1.3.2/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:54:47.481129 devolo_plc_api-1.3.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:54:47.481129 devolo_plc_api-1.3.2/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-07-13 19:54:25.000000 devolo_plc_api-1.3.2/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-07-13 19:54:25.000000 devolo_plc_api-1.3.2/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-07-13 19:54:25.000000 devolo_plc_api-1.3.2/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-07-13 19:54:25.000000 devolo_plc_api-1.3.2/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:54:47.481129 devolo_plc_api-1.3.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-07-13 19:54:25.000000 devolo_plc_api-1.3.2/.github/workflows/convert_todos_to_issues.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-07-13 19:54:25.000000 devolo_plc_api-1.3.2/.github/workflows/pythonpackage.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-07-13 19:54:25.000000 devolo_plc_api-1.3.2/.github/workflows/pythonpublish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-07-13 19:54:25.000000 devolo_plc_api-1.3.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-07-13 19:54:25.000000 devolo_plc_api-1.3.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-13 19:54:25.000000 devolo_plc_api-1.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    44988 2023-07-13 19:54:47.509129 devolo_plc_api-1.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3811 2023-07-13 19:54:25.000000 devolo_plc_api-1.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:54:47.485128 devolo_plc_api-1.3.2/devolo_plc_api/
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-13 19:54:25.000000 devolo_plc_api-1.3.2/devolo_plc_api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:54:47.489129 devolo_plc_api-1.3.2/devolo_plc_api/clients/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-13 19:54:25.000000 devolo_plc_api-1.3.2/devolo_plc_api/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3366 2023-07-13 19:54:25.000000 devolo_plc_api-1.3.2/devolo_plc_api/clients/protobuf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11584 2023-07-13 19:54:25.000000 devolo_plc_api-1.3.2/devolo_plc_api/device.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:54:47.497129 devolo_plc_api-1.3.2/devolo_plc_api/device_api/
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-07-13 19:54:25.000000 devolo_plc_api-1.3.2/devolo_plc_api/device_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12407 2023-07-13 19:54:25.000000 devolo_plc_api-1.3.2/devolo_plc_api/device_api/deviceapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-07-13 19:54:25.000000 devolo_plc_api-1.3.2/devolo_plc_api/device_api/deviceapi.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-07-13 19:54:25.000000 devolo_plc_api-1.3.2/devolo_plc_api/device_api/factoryreset_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-07-13 19:54:25.000000 devolo_plc_api-1.3.2/devolo_plc_api/device_api/factoryreset_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3269 2023-07-13 19:54:25.000000 devolo_plc_api-1.3.2/devolo_plc_api/device_api/ledsettings_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4009 2023-07-13 19:54:25.000000 devolo_plc_api-1.3.2/devolo_plc_api/device_api/ledsettings_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-07-13 19:54:25.000000 devolo_plc_api-1.3.2/devolo_plc_api/device_api/multiap_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-07-13 19:54:25.000000 devolo_plc_api-1.3.2/devolo_plc_api/device_api/multiap_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-07-13 19:54:25.000000 devolo_plc_api-1.3.2/devolo_plc_api/device_api/restart_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-07-13 19:54:25.000000 devolo_plc_api-1.3.2/devolo_plc_api/device_api/restart_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3029 2023-07-13 19:54:25.000000 devolo_plc_api-1.3.2/devolo_plc_api/device_api/support_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4557 2023-07-13 19:54:25.000000 devolo_plc_api-1.3.2/devolo_plc_api/device_api/support_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-07-13 19:54:25.000000 devolo_plc_api-1.3.2/devolo_plc_api/device_api/updatefirmware_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3535 2023-07-13 19:54:25.000000 devolo_plc_api-1.3.2/devolo_plc_api/device_api/updatefirmware_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    15720 2023-07-13 19:54:25.000000 devolo_plc_api-1.3.2/devolo_plc_api/device_api/wifinetwork_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19608 2023-07-13 19:54:25.000000 devolo_plc_api-1.3.2/devolo_plc_api/device_api/wifinetwork_pb2.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:54:47.497129 devolo_plc_api-1.3.2/devolo_plc_api/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-13 19:54:25.000000 devolo_plc_api-1.3.2/devolo_plc_api/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-07-13 19:54:25.000000 devolo_plc_api-1.3.2/devolo_plc_api/exceptions/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-07-13 19:54:25.000000 devolo_plc_api-1.3.2/devolo_plc_api/exceptions/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:54:47.497129 devolo_plc_api-1.3.2/devolo_plc_api/network/
+-rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-07-13 19:54:25.000000 devolo_plc_api-1.3.2/devolo_plc_api/network/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:54:47.501129 devolo_plc_api-1.3.2/devolo_plc_api/plcnet_api/
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-07-13 19:54:25.000000 devolo_plc_api-1.3.2/devolo_plc_api/plcnet_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4782 2023-07-13 19:54:25.000000 devolo_plc_api-1.3.2/devolo_plc_api/plcnet_api/getnetworkoverview_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9456 2023-07-13 19:54:25.000000 devolo_plc_api-1.3.2/devolo_plc_api/plcnet_api/getnetworkoverview_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-07-13 19:54:25.000000 devolo_plc_api-1.3.2/devolo_plc_api/plcnet_api/identifydevice_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-07-13 19:54:25.000000 devolo_plc_api-1.3.2/devolo_plc_api/plcnet_api/identifydevice_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-07-13 19:54:25.000000 devolo_plc_api-1.3.2/devolo_plc_api/plcnet_api/pairdevice_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-07-13 19:54:25.000000 devolo_plc_api-1.3.2/devolo_plc_api/plcnet_api/pairdevice_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4120 2023-07-13 19:54:25.000000 devolo_plc_api-1.3.2/devolo_plc_api/plcnet_api/plcnetapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-13 19:54:25.000000 devolo_plc_api-1.3.2/devolo_plc_api/plcnet_api/plcnetapi.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-07-13 19:54:25.000000 devolo_plc_api-1.3.2/devolo_plc_api/plcnet_api/setuserdevicename_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-07-13 19:54:25.000000 devolo_plc_api-1.3.2/devolo_plc_api/plcnet_api/setuserdevicename_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 19:54:25.000000 devolo_plc_api-1.3.2/devolo_plc_api/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:54:47.501129 devolo_plc_api-1.3.2/devolo_plc_api/zeroconf/
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-07-13 19:54:25.000000 devolo_plc_api-1.3.2/devolo_plc_api/zeroconf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:54:47.489129 devolo_plc_api-1.3.2/devolo_plc_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    44988 2023-07-13 19:54:47.000000 devolo_plc_api-1.3.2/devolo_plc_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-07-13 19:54:47.000000 devolo_plc_api-1.3.2/devolo_plc_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 19:54:47.000000 devolo_plc_api-1.3.2/devolo_plc_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-07-13 19:54:47.000000 devolo_plc_api-1.3.2/devolo_plc_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-13 19:54:47.000000 devolo_plc_api-1.3.2/devolo_plc_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:54:47.501129 devolo_plc_api-1.3.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     4601 2023-07-13 19:54:25.000000 devolo_plc_api-1.3.2/docs/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3372 2023-07-13 19:54:25.000000 devolo_plc_api-1.3.2/docs/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-07-13 19:54:25.000000 devolo_plc_api-1.3.2/docs/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7086 2023-07-13 19:54:25.000000 devolo_plc_api-1.3.2/example_async.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6805 2023-07-13 19:54:25.000000 devolo_plc_api-1.3.2/example_sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-07-13 19:54:25.000000 devolo_plc_api-1.3.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:54:47.505129 devolo_plc_api-1.3.2/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4419 2023-07-13 19:54:25.000000 devolo_plc_api-1.3.2/scripts/stubgen.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 19:54:47.509129 devolo_plc_api-1.3.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:54:47.505129 devolo_plc_api-1.3.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-07-13 19:54:25.000000 devolo_plc_api-1.3.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2618 2023-07-13 19:54:25.000000 devolo_plc_api-1.3.2/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:54:47.509129 devolo_plc_api-1.3.2/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-13 19:54:25.000000 devolo_plc_api-1.3.2/tests/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-07-13 19:54:25.000000 devolo_plc_api-1.3.2/tests/fixtures/device_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-07-13 19:54:25.000000 devolo_plc_api-1.3.2/tests/fixtures/plcnet_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:54:47.509129 devolo_plc_api-1.3.2/tests/mocks/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-13 19:54:25.000000 devolo_plc_api-1.3.2/tests/mocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-07-13 19:54:25.000000 devolo_plc_api-1.3.2/tests/mocks/zeroconf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:54:47.509129 devolo_plc_api-1.3.2/tests/snapshots/
+-rw-r--r--   0 runner    (1001) docker     (123)     3105 2023-07-13 19:54:25.000000 devolo_plc_api-1.3.2/tests/snapshots/test_device.ambr
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-07-13 19:54:25.000000 devolo_plc_api-1.3.2/tests/test_data.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6898 2023-07-13 19:54:25.000000 devolo_plc_api-1.3.2/tests/test_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18393 2023-07-13 19:54:25.000000 devolo_plc_api-1.3.2/tests/test_deviceapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3365 2023-07-13 19:54:25.000000 devolo_plc_api-1.3.2/tests/test_network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6527 2023-07-13 19:54:25.000000 devolo_plc_api-1.3.2/tests/test_plcnetapi.py
```

### Comparing `devolo_plc_api-1.3.1/.github/ISSUE_TEMPLATE/bug_report.md` & `devolo_plc_api-1.3.2/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `devolo_plc_api-1.3.1/.github/ISSUE_TEMPLATE/feature_request.md` & `devolo_plc_api-1.3.2/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `devolo_plc_api-1.3.1/.github/workflows/pythonpackage.yml` & `devolo_plc_api-1.3.2/.github/workflows/pythonpackage.yml`

 * *Files 5% similar despite different names*

```diff
@@ -5,34 +5,34 @@
 jobs:
 
   format:
     name: Check formatting
     runs-on: ubuntu-latest
     steps:
     - name: Checkout sources
-      uses: actions/checkout@v3.5.2
+      uses: actions/checkout@v3.5.3
     - name: Set up Python
-      uses: actions/setup-python@v4.6.0
+      uses: actions/setup-python@v4.6.1
       with:
         python-version: "3.8"
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         python -m pip install --no-binary=mypy mypy
     - name: Check formatting
       uses: pre-commit/action@v3.0.0
 
   lint:
     name: Lint
     runs-on: ubuntu-latest
     steps:
     - name: Checkout sources
-      uses: actions/checkout@v3.5.2
+      uses: actions/checkout@v3.5.3
     - name: Set up Python
-      uses: actions/setup-python@v4.6.0
+      uses: actions/setup-python@v4.6.1
       with:
         python-version: "3.8"
     - name: Lint with ruff
       run: |
         python -m pip install --upgrade pip
         python -m pip install ruff
         ruff check --format=github devolo_plc_api scripts
@@ -47,17 +47,17 @@
     name: Test with Python ${{ matrix.python-version }}
     runs-on: ubuntu-latest
     strategy:
       matrix:
         python-version: ["3.8", "3.9", "3.10", "3.11"]
     steps:
     - name: Checkout sources
-      uses: actions/checkout@v3.5.2
+      uses: actions/checkout@v3.5.3
     - name: Set up Python ${{ matrix.python-version }}
-      uses: actions/setup-python@v4.6.0
+      uses: actions/setup-python@v4.6.1
       with:
         python-version: ${{ matrix.python-version }}
         check-latest: true
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         python -m pip install -e .[test]
@@ -72,17 +72,17 @@
 
   coverage:
     name: Upload coverage
     runs-on: ubuntu-latest
     needs: test
     steps:
     - name: Checkout sources
-      uses: actions/checkout@v3.5.2
+      uses: actions/checkout@v3.5.3
     - name: Set up Python
-      uses: actions/setup-python@v4.6.0
+      uses: actions/setup-python@v4.6.1
       with:
         python-version: "3.8"
     - name: Download coverage
       uses: actions/download-artifact@v3.0.2
       with:
         name: coverage
     - name: Coveralls
```

### Comparing `devolo_plc_api-1.3.1/.github/workflows/pythonpublish.yml` & `devolo_plc_api-1.3.2/.github/workflows/pythonpublish.yml`

 * *Files 17% similar despite different names*

```diff
@@ -4,17 +4,17 @@
   release:
     types: [created]
 
 jobs:
   deploy:
     runs-on: ubuntu-latest
     steps:
-    - uses: actions/checkout@v3.5.2
+    - uses: actions/checkout@v3.5.3
     - name: Set up Python
-      uses: actions/setup-python@v4.6.0
+      uses: actions/setup-python@v4.6.1
       with:
         python-version: "3.8"
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         python -m pip install --upgrade build twine
     - name: Build and publish
```

### Comparing `devolo_plc_api-1.3.1/.gitignore` & `devolo_plc_api-1.3.2/.gitignore`

 * *Files identical despite different names*

### Comparing `devolo_plc_api-1.3.1/.pre-commit-config.yaml` & `devolo_plc_api-1.3.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `devolo_plc_api-1.3.1/LICENSE` & `devolo_plc_api-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `devolo_plc_api-1.3.1/PKG-INFO` & `devolo_plc_api-1.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: devolo_plc_api
-Version: 1.3.1
+Version: 1.3.2
 Summary: devolo PLC devices in Python
 Author-email: Markus Bong <m.bong@famabo.de>, Guido Schmitz <guido.schmitz@fedaix.de>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `devolo_plc_api-1.3.1/README.md` & `devolo_plc_api-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `devolo_plc_api-1.3.1/devolo_plc_api/clients/protobuf.py` & `devolo_plc_api-1.3.2/devolo_plc_api/clients/protobuf.py`

 * *Files identical despite different names*

### Comparing `devolo_plc_api-1.3.1/devolo_plc_api/device.py` & `devolo_plc_api-1.3.2/devolo_plc_api/device.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,15 @@
         self.technology = ""
         self.serial_number = "0"
 
         self.device: DeviceApi | None = None
         self.plcnet: PlcNetApi | None = None
 
         self._background_tasks: set[asyncio.Task] = set()
-        self._browser: AsyncServiceBrowser | None
+        self._browser: AsyncServiceBrowser | None = None
         self._connected = False
         self._info: dict[str, ZeroconfServiceInfo] = {PLCNETAPI: ZeroconfServiceInfo(), DEVICEAPI: ZeroconfServiceInfo()}
         self._logger = logging.getLogger(f"{self.__class__.__module__}.{self.__class__.__name__}")
         self._multicast = False
         self._password = ""
         self._session_instance: AsyncClient | None = None
         self._zeroconf_instance = zeroconf_instance
@@ -203,14 +203,17 @@
     async def _get_zeroconf_info(self) -> None:
         """Browse for the desired mDNS service types and query them."""
         service_types = [DEVICEAPI, PLCNETAPI]
         counter = 0
         self._logger.debug("Browsing for %s", service_types)
         addr = None if self._multicast else self.ip
         question_type = DNSQuestionType.QM if self._multicast else DNSQuestionType.QU
+        if self._browser:
+            await self._browser.async_cancel()
+            self._browser = None
         self._browser = AsyncServiceBrowser(
             zeroconf=self._zeroconf.zeroconf,
             type_=service_types,
             handlers=[self._state_change],
             addr=addr,
             question_type=question_type,
         )
```

### Comparing `devolo_plc_api-1.3.1/devolo_plc_api/device_api/__init__.py` & `devolo_plc_api-1.3.2/devolo_plc_api/device_api/__init__.py`

 * *Files identical despite different names*

### Comparing `devolo_plc_api-1.3.1/devolo_plc_api/device_api/deviceapi.py` & `devolo_plc_api-1.3.2/devolo_plc_api/device_api/deviceapi.py`

 * *Files identical despite different names*

### Comparing `devolo_plc_api-1.3.1/devolo_plc_api/device_api/deviceapi.pyi` & `devolo_plc_api-1.3.2/devolo_plc_api/device_api/deviceapi.pyi`

 * *Files identical despite different names*

### Comparing `devolo_plc_api-1.3.1/devolo_plc_api/device_api/factoryreset_pb2.py` & `devolo_plc_api-1.3.2/devolo_plc_api/device_api/factoryreset_pb2.py`

 * *Files identical despite different names*

### Comparing `devolo_plc_api-1.3.1/devolo_plc_api/device_api/factoryreset_pb2.pyi` & `devolo_plc_api-1.3.2/devolo_plc_api/device_api/factoryreset_pb2.pyi`

 * *Files identical despite different names*

### Comparing `devolo_plc_api-1.3.1/devolo_plc_api/device_api/ledsettings_pb2.py` & `devolo_plc_api-1.3.2/devolo_plc_api/device_api/ledsettings_pb2.py`

 * *Files identical despite different names*

### Comparing `devolo_plc_api-1.3.1/devolo_plc_api/device_api/ledsettings_pb2.pyi` & `devolo_plc_api-1.3.2/devolo_plc_api/device_api/ledsettings_pb2.pyi`

 * *Files identical despite different names*

### Comparing `devolo_plc_api-1.3.1/devolo_plc_api/device_api/multiap_pb2.py` & `devolo_plc_api-1.3.2/devolo_plc_api/device_api/multiap_pb2.py`

 * *Files identical despite different names*

### Comparing `devolo_plc_api-1.3.1/devolo_plc_api/device_api/multiap_pb2.pyi` & `devolo_plc_api-1.3.2/devolo_plc_api/device_api/multiap_pb2.pyi`

 * *Files identical despite different names*

### Comparing `devolo_plc_api-1.3.1/devolo_plc_api/device_api/restart_pb2.py` & `devolo_plc_api-1.3.2/devolo_plc_api/device_api/restart_pb2.py`

 * *Files identical despite different names*

### Comparing `devolo_plc_api-1.3.1/devolo_plc_api/device_api/restart_pb2.pyi` & `devolo_plc_api-1.3.2/devolo_plc_api/device_api/restart_pb2.pyi`

 * *Files identical despite different names*

### Comparing `devolo_plc_api-1.3.1/devolo_plc_api/device_api/support_pb2.py` & `devolo_plc_api-1.3.2/devolo_plc_api/device_api/support_pb2.py`

 * *Files identical despite different names*

### Comparing `devolo_plc_api-1.3.1/devolo_plc_api/device_api/support_pb2.pyi` & `devolo_plc_api-1.3.2/devolo_plc_api/device_api/support_pb2.pyi`

 * *Files identical despite different names*

### Comparing `devolo_plc_api-1.3.1/devolo_plc_api/device_api/updatefirmware_pb2.py` & `devolo_plc_api-1.3.2/devolo_plc_api/device_api/updatefirmware_pb2.py`

 * *Files identical despite different names*

### Comparing `devolo_plc_api-1.3.1/devolo_plc_api/device_api/updatefirmware_pb2.pyi` & `devolo_plc_api-1.3.2/devolo_plc_api/device_api/updatefirmware_pb2.pyi`

 * *Files identical despite different names*

### Comparing `devolo_plc_api-1.3.1/devolo_plc_api/device_api/wifinetwork_pb2.py` & `devolo_plc_api-1.3.2/devolo_plc_api/device_api/wifinetwork_pb2.py`

 * *Files identical despite different names*

### Comparing `devolo_plc_api-1.3.1/devolo_plc_api/device_api/wifinetwork_pb2.pyi` & `devolo_plc_api-1.3.2/devolo_plc_api/device_api/wifinetwork_pb2.pyi`

 * *Files identical despite different names*

### Comparing `devolo_plc_api-1.3.1/devolo_plc_api/exceptions/device.py` & `devolo_plc_api-1.3.2/devolo_plc_api/exceptions/device.py`

 * *Files identical despite different names*

### Comparing `devolo_plc_api-1.3.1/devolo_plc_api/network/__init__.py` & `devolo_plc_api-1.3.2/devolo_plc_api/network/__init__.py`

 * *Files identical despite different names*

### Comparing `devolo_plc_api-1.3.1/devolo_plc_api/plcnet_api/__init__.py` & `devolo_plc_api-1.3.2/devolo_plc_api/plcnet_api/__init__.py`

 * *Files identical despite different names*

### Comparing `devolo_plc_api-1.3.1/devolo_plc_api/plcnet_api/getnetworkoverview_pb2.py` & `devolo_plc_api-1.3.2/devolo_plc_api/plcnet_api/getnetworkoverview_pb2.py`

 * *Files identical despite different names*

### Comparing `devolo_plc_api-1.3.1/devolo_plc_api/plcnet_api/getnetworkoverview_pb2.pyi` & `devolo_plc_api-1.3.2/devolo_plc_api/plcnet_api/getnetworkoverview_pb2.pyi`

 * *Files identical despite different names*

### Comparing `devolo_plc_api-1.3.1/devolo_plc_api/plcnet_api/identifydevice_pb2.py` & `devolo_plc_api-1.3.2/devolo_plc_api/plcnet_api/identifydevice_pb2.py`

 * *Files identical despite different names*

### Comparing `devolo_plc_api-1.3.1/devolo_plc_api/plcnet_api/identifydevice_pb2.pyi` & `devolo_plc_api-1.3.2/devolo_plc_api/plcnet_api/identifydevice_pb2.pyi`

 * *Files identical despite different names*

### Comparing `devolo_plc_api-1.3.1/devolo_plc_api/plcnet_api/pairdevice_pb2.py` & `devolo_plc_api-1.3.2/devolo_plc_api/plcnet_api/pairdevice_pb2.py`

 * *Files identical despite different names*

### Comparing `devolo_plc_api-1.3.1/devolo_plc_api/plcnet_api/pairdevice_pb2.pyi` & `devolo_plc_api-1.3.2/devolo_plc_api/plcnet_api/pairdevice_pb2.pyi`

 * *Files identical despite different names*

### Comparing `devolo_plc_api-1.3.1/devolo_plc_api/plcnet_api/plcnetapi.py` & `devolo_plc_api-1.3.2/devolo_plc_api/plcnet_api/plcnetapi.py`

 * *Files identical despite different names*

### Comparing `devolo_plc_api-1.3.1/devolo_plc_api/plcnet_api/plcnetapi.pyi` & `devolo_plc_api-1.3.2/devolo_plc_api/plcnet_api/plcnetapi.pyi`

 * *Files identical despite different names*

### Comparing `devolo_plc_api-1.3.1/devolo_plc_api/plcnet_api/setuserdevicename_pb2.py` & `devolo_plc_api-1.3.2/devolo_plc_api/plcnet_api/setuserdevicename_pb2.py`

 * *Files identical despite different names*

### Comparing `devolo_plc_api-1.3.1/devolo_plc_api/plcnet_api/setuserdevicename_pb2.pyi` & `devolo_plc_api-1.3.2/devolo_plc_api/plcnet_api/setuserdevicename_pb2.pyi`

 * *Files identical despite different names*

### Comparing `devolo_plc_api-1.3.1/devolo_plc_api.egg-info/PKG-INFO` & `devolo_plc_api-1.3.2/devolo_plc_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: devolo-plc-api
-Version: 1.3.1
+Version: 1.3.2
 Summary: devolo PLC devices in Python
 Author-email: Markus Bong <m.bong@famabo.de>, Guido Schmitz <guido.schmitz@fedaix.de>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `devolo_plc_api-1.3.1/devolo_plc_api.egg-info/SOURCES.txt` & `devolo_plc_api-1.3.2/devolo_plc_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `devolo_plc_api-1.3.1/docs/CHANGELOG.md` & `devolo_plc_api-1.3.2/docs/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,19 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/), and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [v1.3.2] - 2023/07/13
+
+### Fixed
+
+- Frequently connecting to an offline device lead to a memory leak
+
 ## [v1.3.1] - 2023/05/12
 
 ### Fixed
 
 - Reduce zeroconf traffic
 
 ## [v1.3.0] - 2023/04/13
```

### Comparing `devolo_plc_api-1.3.1/docs/CODE_OF_CONDUCT.md` & `devolo_plc_api-1.3.2/docs/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `devolo_plc_api-1.3.1/docs/CONTRIBUTING.md` & `devolo_plc_api-1.3.2/docs/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `devolo_plc_api-1.3.1/example_async.py` & `devolo_plc_api-1.3.2/example_async.py`

 * *Files identical despite different names*

### Comparing `devolo_plc_api-1.3.1/example_sync.py` & `devolo_plc_api-1.3.2/example_sync.py`

 * *Files identical despite different names*

### Comparing `devolo_plc_api-1.3.1/pyproject.toml` & `devolo_plc_api-1.3.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `devolo_plc_api-1.3.1/scripts/stubgen.py` & `devolo_plc_api-1.3.2/scripts/stubgen.py`

 * *Files identical despite different names*

### Comparing `devolo_plc_api-1.3.1/tests/__init__.py` & `devolo_plc_api-1.3.2/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `devolo_plc_api-1.3.1/tests/conftest.py` & `devolo_plc_api-1.3.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `devolo_plc_api-1.3.1/tests/fixtures/device_api.py` & `devolo_plc_api-1.3.2/tests/fixtures/device_api.py`

 * *Files identical despite different names*

### Comparing `devolo_plc_api-1.3.1/tests/fixtures/plcnet_api.py` & `devolo_plc_api-1.3.2/tests/fixtures/plcnet_api.py`

 * *Files identical despite different names*

### Comparing `devolo_plc_api-1.3.1/tests/mocks/zeroconf.py` & `devolo_plc_api-1.3.2/tests/mocks/zeroconf.py`

 * *Files identical despite different names*

### Comparing `devolo_plc_api-1.3.1/tests/snapshots/test_device.ambr` & `devolo_plc_api-1.3.2/tests/snapshots/test_device.ambr`

 * *Files identical despite different names*

### Comparing `devolo_plc_api-1.3.1/tests/test_data.json` & `devolo_plc_api-1.3.2/tests/test_data.json`

 * *Files identical despite different names*

### Comparing `devolo_plc_api-1.3.1/tests/test_device.py` & `devolo_plc_api-1.3.2/tests/test_device.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,17 +55,19 @@
         with patch("devolo_plc_api.device.Device._get_zeroconf_info") as get_zeroconf_info, pytest.raises(DeviceNotFound):
             device = Device(test_data.ip)
             await device.async_connect()
             assert device._multicast
             assert get_zeroconf_info.call_count == 2
 
     @pytest.mark.asyncio()
+    @pytest.mark.parametrize("device_type", [DeviceType.PLC])
+    @pytest.mark.usefixtures("service_browser")
     async def test_async_connect_not_found(self, mock_device: Device, sleep: AsyncMock):
         """Test that an exception is raised if both APIs are not available."""
-        with patch("devolo_plc_api.device.AsyncServiceBrowser"), pytest.raises(DeviceNotFound):
+        with pytest.raises(DeviceNotFound):
             await mock_device.async_connect()
             assert not mock_device._connected
             assert sleep.call_count == Device.MDNS_TIMEOUT
 
     def test_connect(self, mock_device: Device):
         """Test that the sync connect method just calls the async connect method."""
         with patch("devolo_plc_api.device.Device.async_connect", new=AsyncMock()) as ac:
```

### Comparing `devolo_plc_api-1.3.1/tests/test_deviceapi.py` & `devolo_plc_api-1.3.2/tests/test_deviceapi.py`

 * *Files identical despite different names*

### Comparing `devolo_plc_api-1.3.1/tests/test_network.py` & `devolo_plc_api-1.3.2/tests/test_network.py`

 * *Files identical despite different names*

### Comparing `devolo_plc_api-1.3.1/tests/test_plcnetapi.py` & `devolo_plc_api-1.3.2/tests/test_plcnetapi.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from devolo_plc_api.plcnet_api.identifydevice_pb2 import IdentifyDeviceResponse
 from devolo_plc_api.plcnet_api.pairdevice_pb2 import PairDeviceStart
 from devolo_plc_api.plcnet_api.setuserdevicename_pb2 import SetUserDeviceNameResponse
 
 from . import DeviceType
 
 
-class TestDeviceApi:
+class TestPlcApi:
     """Test devolo_plc_api.plcnet_api.plcnetapi.PlcNetApi class."""
 
     @pytest.mark.asyncio()
     @pytest.mark.parametrize("device_type", [DeviceType.PLC])
     @pytest.mark.usefixtures("block_communication", "service_browser")
     async def test_wrong_password_type(self, httpx_mock: HTTPXMock, mock_device: Device):
         """Test using different password hash if original password failed."""
```

