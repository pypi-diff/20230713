# Comparing `tmp/rpcclient-3.17.0.tar.gz` & `tmp/rpcclient-3.17.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rpcclient-3.17.0.tar", last modified: Thu Jul 13 11:25:57 2023, max compression
+gzip compressed data, was "rpcclient-3.17.1.tar", last modified: Thu Jul 13 11:33:21 2023, max compression
```

## Comparing `rpcclient-3.17.0.tar` & `rpcclient-3.17.1.tar`

### file list

```diff
@@ -1,101 +1,101 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:25:57.049653 rpcclient-3.17.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-07-13 11:25:39.000000 rpcclient-3.17.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    41689 2023-07-13 11:25:57.049653 rpcclient-3.17.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-13 11:25:39.000000 rpcclient-3.17.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-07-13 11:25:39.000000 rpcclient-3.17.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-13 11:25:39.000000 rpcclient-3.17.0/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:25:57.041653 rpcclient-3.17.0/rpcclient/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 11:25:39.000000 rpcclient-3.17.0/rpcclient/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-07-13 11:25:39.000000 rpcclient-3.17.0/rpcclient/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-07-13 11:25:39.000000 rpcclient-3.17.0/rpcclient/allocated.py
--rw-r--r--   0 runner    (1001) docker     (123)    23671 2023-07-13 11:25:39.000000 rpcclient-3.17.0/rpcclient/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3218 2023-07-13 11:25:39.000000 rpcclient-3.17.0/rpcclient/client_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:25:57.045653 rpcclient-3.17.0/rpcclient/darwin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 11:25:39.000000 rpcclient-3.17.0/rpcclient/darwin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-07-13 11:25:39.000000 rpcclient-3.17.0/rpcclient/darwin/bluetooth.py
--rw-r--r--   0 runner    (1001) docker     (123)     4853 2023-07-13 11:25:39.000000 rpcclient-3.17.0/rpcclient/darwin/cfpreferences.py
--rw-r--r--   0 runner    (1001) docker     (123)    12667 2023-07-13 11:25:39.000000 rpcclient-3.17.0/rpcclient/darwin/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-13 11:25:39.000000 rpcclient-3.17.0/rpcclient/darwin/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    37890 2023-07-13 11:25:39.000000 rpcclient-3.17.0/rpcclient/darwin/consts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-07-13 11:25:39.000000 rpcclient-3.17.0/rpcclient/darwin/core_graphics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-07-13 11:25:39.000000 rpcclient-3.17.0/rpcclient/darwin/crash_reports.py
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-13 11:25:39.000000 rpcclient-3.17.0/rpcclient/darwin/darwin_lief.py
--rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-07-13 11:25:39.000000 rpcclient-3.17.0/rpcclient/darwin/fs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8438 2023-07-13 11:25:39.000000 rpcclient-3.17.0/rpcclient/darwin/hid.py
--rw-r--r--   0 runner    (1001) docker     (123)     5437 2023-07-13 11:25:39.000000 rpcclient-3.17.0/rpcclient/darwin/ioregistry.py
--rw-r--r--   0 runner    (1001) docker     (123)     3421 2023-07-13 11:25:39.000000 rpcclient-3.17.0/rpcclient/darwin/keychain.py
--rw-r--r--   0 runner    (1001) docker     (123)     3368 2023-07-13 11:25:39.000000 rpcclient-3.17.0/rpcclient/darwin/location.py
--rw-r--r--   0 runner    (1001) docker     (123)     7638 2023-07-13 11:25:39.000000 rpcclient-3.17.0/rpcclient/darwin/media.py
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-07-13 11:25:39.000000 rpcclient-3.17.0/rpcclient/darwin/network.py
--rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-07-13 11:25:39.000000 rpcclient-3.17.0/rpcclient/darwin/objc.py
--rw-r--r--   0 runner    (1001) docker     (123)     7588 2023-07-13 11:25:39.000000 rpcclient-3.17.0/rpcclient/darwin/objective_c_class.py
--rw-r--r--   0 runner    (1001) docker     (123)     7990 2023-07-13 11:25:39.000000 rpcclient-3.17.0/rpcclient/darwin/objective_c_symbol.py
--rw-r--r--   0 runner    (1001) docker     (123)     3786 2023-07-13 11:25:39.000000 rpcclient-3.17.0/rpcclient/darwin/power.py
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-07-13 11:25:39.000000 rpcclient-3.17.0/rpcclient/darwin/preferences.py
--rw-r--r--   0 runner    (1001) docker     (123)    33780 2023-07-13 11:25:39.000000 rpcclient-3.17.0/rpcclient/darwin/processes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-07-13 11:25:39.000000 rpcclient-3.17.0/rpcclient/darwin/reports.py
--rw-r--r--   0 runner    (1001) docker     (123)     5152 2023-07-13 11:25:39.000000 rpcclient-3.17.0/rpcclient/darwin/scpreferences.py
--rw-r--r--   0 runner    (1001) docker     (123)    29308 2023-07-13 11:25:39.000000 rpcclient-3.17.0/rpcclient/darwin/structs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-07-13 11:25:39.000000 rpcclient-3.17.0/rpcclient/darwin/symbol.py
--rw-r--r--   0 runner    (1001) docker     (123)     9396 2023-07-13 11:25:39.000000 rpcclient-3.17.0/rpcclient/darwin/syslog.py
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-07-13 11:25:39.000000 rpcclient-3.17.0/rpcclient/darwin/time.py
--rw-r--r--   0 runner    (1001) docker     (123)     8327 2023-07-13 11:25:39.000000 rpcclient-3.17.0/rpcclient/darwin/xpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4254 2023-07-13 11:25:39.000000 rpcclient-3.17.0/rpcclient/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    20680 2023-07-13 11:25:39.000000 rpcclient-3.17.0/rpcclient/fs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:25:57.045653 rpcclient-3.17.0/rpcclient/ios/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 11:25:39.000000 rpcclient-3.17.0/rpcclient/ios/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17603 2023-07-13 11:25:39.000000 rpcclient-3.17.0/rpcclient/ios/accessibility.py
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-07-13 11:25:39.000000 rpcclient-3.17.0/rpcclient/ios/amfi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-07-13 11:25:39.000000 rpcclient-3.17.0/rpcclient/ios/backlight.py
--rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-07-13 11:25:39.000000 rpcclient-3.17.0/rpcclient/ios/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3498 2023-07-13 11:25:39.000000 rpcclient-3.17.0/rpcclient/ios/lockdown.py
--rw-r--r--   0 runner    (1001) docker     (123)    12890 2023-07-13 11:25:39.000000 rpcclient-3.17.0/rpcclient/ios/mobile_gestalt.py
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-07-13 11:25:39.000000 rpcclient-3.17.0/rpcclient/ios/screen_capture.py
--rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-07-13 11:25:39.000000 rpcclient-3.17.0/rpcclient/ios/sprinboard.py
--rw-r--r--   0 runner    (1001) docker     (123)     3144 2023-07-13 11:25:39.000000 rpcclient-3.17.0/rpcclient/ios/telephony.py
--rw-r--r--   0 runner    (1001) docker     (123)     7605 2023-07-13 11:25:39.000000 rpcclient-3.17.0/rpcclient/ios/wifi.py
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-07-13 11:25:39.000000 rpcclient-3.17.0/rpcclient/lief.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:25:57.045653 rpcclient-3.17.0/rpcclient/linux/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 11:25:39.000000 rpcclient-3.17.0/rpcclient/linux/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-13 11:25:39.000000 rpcclient-3.17.0/rpcclient/linux/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-07-13 11:25:39.000000 rpcclient-3.17.0/rpcclient/linux/structs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:25:57.045653 rpcclient-3.17.0/rpcclient/macos/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 11:25:39.000000 rpcclient-3.17.0/rpcclient/macos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-07-13 11:25:39.000000 rpcclient-3.17.0/rpcclient/macos/apple_script.py
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-07-13 11:25:39.000000 rpcclient-3.17.0/rpcclient/macos/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     8707 2023-07-13 11:25:39.000000 rpcclient-3.17.0/rpcclient/network.py
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-07-13 11:25:39.000000 rpcclient-3.17.0/rpcclient/processes.py
--rw-r--r--   0 runner    (1001) docker     (123)     4430 2023-07-13 11:25:39.000000 rpcclient-3.17.0/rpcclient/protocol.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:25:57.049653 rpcclient-3.17.0/rpcclient/structs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 11:25:39.000000 rpcclient-3.17.0/rpcclient/structs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-07-13 11:25:39.000000 rpcclient-3.17.0/rpcclient/structs/consts.py
--rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-07-13 11:25:39.000000 rpcclient-3.17.0/rpcclient/structs/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     6782 2023-07-13 11:25:39.000000 rpcclient-3.17.0/rpcclient/symbol.py
--rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-07-13 11:25:39.000000 rpcclient-3.17.0/rpcclient/symbols_jar.py
--rw-r--r--   0 runner    (1001) docker     (123)     7139 2023-07-13 11:25:39.000000 rpcclient-3.17.0/rpcclient/sysctl.py
--rw-r--r--   0 runner    (1001) docker     (123)    24398 2023-07-13 11:25:39.000000 rpcclient-3.17.0/rpcclient/xonshrc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:25:57.041653 rpcclient-3.17.0/rpcclient.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    41689 2023-07-13 11:25:57.000000 rpcclient-3.17.0/rpcclient.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-07-13 11:25:57.000000 rpcclient-3.17.0/rpcclient.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 11:25:57.000000 rpcclient-3.17.0/rpcclient.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-13 11:25:57.000000 rpcclient-3.17.0/rpcclient.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-07-13 11:25:57.000000 rpcclient-3.17.0/rpcclient.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-13 11:25:57.000000 rpcclient-3.17.0/rpcclient.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 11:25:57.049653 rpcclient-3.17.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:25:57.049653 rpcclient-3.17.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-07-13 11:25:39.000000 rpcclient-3.17.0/tests/test_allocation_cleanup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-07-13 11:25:39.000000 rpcclient-3.17.0/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-13 11:25:39.000000 rpcclient-3.17.0/tests/test_core_foundation_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-07-13 11:25:39.000000 rpcclient-3.17.0/tests/test_darwin_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     4676 2023-07-13 11:25:39.000000 rpcclient-3.17.0/tests/test_fs.py
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-13 11:25:39.000000 rpcclient-3.17.0/tests/test_keychain.py
--rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-07-13 11:25:39.000000 rpcclient-3.17.0/tests/test_objc_symbol.py
--rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-07-13 11:25:39.000000 rpcclient-3.17.0/tests/test_power.py
--rw-r--r--   0 runner    (1001) docker     (123)     7329 2023-07-13 11:25:39.000000 rpcclient-3.17.0/tests/test_preferences.py
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-07-13 11:25:39.000000 rpcclient-3.17.0/tests/test_processes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3316 2023-07-13 11:25:39.000000 rpcclient-3.17.0/tests/test_socket.py
--rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-07-13 11:25:39.000000 rpcclient-3.17.0/tests/test_spawn.py
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-07-13 11:25:39.000000 rpcclient-3.17.0/tests/test_thread_safe.py
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-07-13 11:25:39.000000 rpcclient-3.17.0/tests/test_time.py
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-07-13 11:25:39.000000 rpcclient-3.17.0/tests/test_worker_processes.py
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-07-13 11:25:39.000000 rpcclient-3.17.0/tests/test_xpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:33:21.742803 rpcclient-3.17.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-07-13 11:33:03.000000 rpcclient-3.17.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    41689 2023-07-13 11:33:21.742803 rpcclient-3.17.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-13 11:33:03.000000 rpcclient-3.17.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-07-13 11:33:03.000000 rpcclient-3.17.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-07-13 11:33:03.000000 rpcclient-3.17.1/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:33:21.734803 rpcclient-3.17.1/rpcclient/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 11:33:03.000000 rpcclient-3.17.1/rpcclient/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-07-13 11:33:03.000000 rpcclient-3.17.1/rpcclient/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-07-13 11:33:03.000000 rpcclient-3.17.1/rpcclient/allocated.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23671 2023-07-13 11:33:03.000000 rpcclient-3.17.1/rpcclient/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3218 2023-07-13 11:33:03.000000 rpcclient-3.17.1/rpcclient/client_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:33:21.738803 rpcclient-3.17.1/rpcclient/darwin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 11:33:03.000000 rpcclient-3.17.1/rpcclient/darwin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-07-13 11:33:03.000000 rpcclient-3.17.1/rpcclient/darwin/bluetooth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4853 2023-07-13 11:33:03.000000 rpcclient-3.17.1/rpcclient/darwin/cfpreferences.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12667 2023-07-13 11:33:03.000000 rpcclient-3.17.1/rpcclient/darwin/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-13 11:33:03.000000 rpcclient-3.17.1/rpcclient/darwin/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37890 2023-07-13 11:33:03.000000 rpcclient-3.17.1/rpcclient/darwin/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-07-13 11:33:03.000000 rpcclient-3.17.1/rpcclient/darwin/core_graphics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-07-13 11:33:03.000000 rpcclient-3.17.1/rpcclient/darwin/crash_reports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-13 11:33:03.000000 rpcclient-3.17.1/rpcclient/darwin/darwin_lief.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-07-13 11:33:03.000000 rpcclient-3.17.1/rpcclient/darwin/fs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8438 2023-07-13 11:33:03.000000 rpcclient-3.17.1/rpcclient/darwin/hid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5437 2023-07-13 11:33:03.000000 rpcclient-3.17.1/rpcclient/darwin/ioregistry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3421 2023-07-13 11:33:03.000000 rpcclient-3.17.1/rpcclient/darwin/keychain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3368 2023-07-13 11:33:03.000000 rpcclient-3.17.1/rpcclient/darwin/location.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7638 2023-07-13 11:33:03.000000 rpcclient-3.17.1/rpcclient/darwin/media.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-07-13 11:33:03.000000 rpcclient-3.17.1/rpcclient/darwin/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-07-13 11:33:03.000000 rpcclient-3.17.1/rpcclient/darwin/objc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7588 2023-07-13 11:33:03.000000 rpcclient-3.17.1/rpcclient/darwin/objective_c_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7990 2023-07-13 11:33:03.000000 rpcclient-3.17.1/rpcclient/darwin/objective_c_symbol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3786 2023-07-13 11:33:03.000000 rpcclient-3.17.1/rpcclient/darwin/power.py
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-07-13 11:33:03.000000 rpcclient-3.17.1/rpcclient/darwin/preferences.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33780 2023-07-13 11:33:03.000000 rpcclient-3.17.1/rpcclient/darwin/processes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-07-13 11:33:03.000000 rpcclient-3.17.1/rpcclient/darwin/reports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5152 2023-07-13 11:33:03.000000 rpcclient-3.17.1/rpcclient/darwin/scpreferences.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29308 2023-07-13 11:33:03.000000 rpcclient-3.17.1/rpcclient/darwin/structs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-07-13 11:33:03.000000 rpcclient-3.17.1/rpcclient/darwin/symbol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9396 2023-07-13 11:33:03.000000 rpcclient-3.17.1/rpcclient/darwin/syslog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-07-13 11:33:03.000000 rpcclient-3.17.1/rpcclient/darwin/time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8327 2023-07-13 11:33:03.000000 rpcclient-3.17.1/rpcclient/darwin/xpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4254 2023-07-13 11:33:03.000000 rpcclient-3.17.1/rpcclient/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20680 2023-07-13 11:33:03.000000 rpcclient-3.17.1/rpcclient/fs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:33:21.738803 rpcclient-3.17.1/rpcclient/ios/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 11:33:03.000000 rpcclient-3.17.1/rpcclient/ios/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17603 2023-07-13 11:33:03.000000 rpcclient-3.17.1/rpcclient/ios/accessibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-07-13 11:33:03.000000 rpcclient-3.17.1/rpcclient/ios/amfi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-07-13 11:33:03.000000 rpcclient-3.17.1/rpcclient/ios/backlight.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-07-13 11:33:03.000000 rpcclient-3.17.1/rpcclient/ios/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3498 2023-07-13 11:33:03.000000 rpcclient-3.17.1/rpcclient/ios/lockdown.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12890 2023-07-13 11:33:03.000000 rpcclient-3.17.1/rpcclient/ios/mobile_gestalt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-07-13 11:33:03.000000 rpcclient-3.17.1/rpcclient/ios/screen_capture.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-07-13 11:33:03.000000 rpcclient-3.17.1/rpcclient/ios/sprinboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3144 2023-07-13 11:33:03.000000 rpcclient-3.17.1/rpcclient/ios/telephony.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7605 2023-07-13 11:33:03.000000 rpcclient-3.17.1/rpcclient/ios/wifi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-07-13 11:33:03.000000 rpcclient-3.17.1/rpcclient/lief.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:33:21.738803 rpcclient-3.17.1/rpcclient/linux/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 11:33:03.000000 rpcclient-3.17.1/rpcclient/linux/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-13 11:33:03.000000 rpcclient-3.17.1/rpcclient/linux/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-07-13 11:33:03.000000 rpcclient-3.17.1/rpcclient/linux/structs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:33:21.738803 rpcclient-3.17.1/rpcclient/macos/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 11:33:03.000000 rpcclient-3.17.1/rpcclient/macos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-07-13 11:33:03.000000 rpcclient-3.17.1/rpcclient/macos/apple_script.py
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-07-13 11:33:03.000000 rpcclient-3.17.1/rpcclient/macos/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8707 2023-07-13 11:33:03.000000 rpcclient-3.17.1/rpcclient/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-07-13 11:33:03.000000 rpcclient-3.17.1/rpcclient/processes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4430 2023-07-13 11:33:03.000000 rpcclient-3.17.1/rpcclient/protocol.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:33:21.742803 rpcclient-3.17.1/rpcclient/structs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 11:33:03.000000 rpcclient-3.17.1/rpcclient/structs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-07-13 11:33:03.000000 rpcclient-3.17.1/rpcclient/structs/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-07-13 11:33:03.000000 rpcclient-3.17.1/rpcclient/structs/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6782 2023-07-13 11:33:03.000000 rpcclient-3.17.1/rpcclient/symbol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-07-13 11:33:03.000000 rpcclient-3.17.1/rpcclient/symbols_jar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7139 2023-07-13 11:33:03.000000 rpcclient-3.17.1/rpcclient/sysctl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24398 2023-07-13 11:33:03.000000 rpcclient-3.17.1/rpcclient/xonshrc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:33:21.734803 rpcclient-3.17.1/rpcclient.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    41689 2023-07-13 11:33:21.000000 rpcclient-3.17.1/rpcclient.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-07-13 11:33:21.000000 rpcclient-3.17.1/rpcclient.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 11:33:21.000000 rpcclient-3.17.1/rpcclient.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-13 11:33:21.000000 rpcclient-3.17.1/rpcclient.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-07-13 11:33:21.000000 rpcclient-3.17.1/rpcclient.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-13 11:33:21.000000 rpcclient-3.17.1/rpcclient.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 11:33:21.742803 rpcclient-3.17.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:33:21.742803 rpcclient-3.17.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-07-13 11:33:03.000000 rpcclient-3.17.1/tests/test_allocation_cleanup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-07-13 11:33:03.000000 rpcclient-3.17.1/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-13 11:33:03.000000 rpcclient-3.17.1/tests/test_core_foundation_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-07-13 11:33:03.000000 rpcclient-3.17.1/tests/test_darwin_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4676 2023-07-13 11:33:03.000000 rpcclient-3.17.1/tests/test_fs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-13 11:33:03.000000 rpcclient-3.17.1/tests/test_keychain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-07-13 11:33:03.000000 rpcclient-3.17.1/tests/test_objc_symbol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-07-13 11:33:03.000000 rpcclient-3.17.1/tests/test_power.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7329 2023-07-13 11:33:03.000000 rpcclient-3.17.1/tests/test_preferences.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-07-13 11:33:03.000000 rpcclient-3.17.1/tests/test_processes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3316 2023-07-13 11:33:03.000000 rpcclient-3.17.1/tests/test_socket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-07-13 11:33:03.000000 rpcclient-3.17.1/tests/test_spawn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-07-13 11:33:03.000000 rpcclient-3.17.1/tests/test_thread_safe.py
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-07-13 11:33:03.000000 rpcclient-3.17.1/tests/test_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-07-13 11:33:03.000000 rpcclient-3.17.1/tests/test_worker_processes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-07-13 11:33:03.000000 rpcclient-3.17.1/tests/test_xpc.py
```

### Comparing `rpcclient-3.17.0/LICENSE` & `rpcclient-3.17.1/LICENSE`

 * *Files identical despite different names*

### Comparing `rpcclient-3.17.0/PKG-INFO` & `rpcclient-3.17.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rpcclient
-Version: 3.17.0
+Version: 3.17.1
 Summary: rpcclient for connecting with the rpcserver
 Author-email: doronz88 <doron88@gmail.com>, matan <matan1008@gmail.com>
 Maintainer-email: doronz88 <doron88@gmail.com>, matan <matan1008@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
```

### Comparing `rpcclient-3.17.0/pyproject.toml` & `rpcclient-3.17.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "rpcclient"
-version = "3.17.0"
+version = "3.17.1"
 description = "rpcclient for connecting with the rpcserver"
 readme = "README.md"
 requires-python = ">=3.8"
 license = { file = "LICENSE" }
 keywords = ["ios", "macos", "linux", "automation", "remote-shell", "remote-control", "ipython"]
 authors = [
     { name = "doronz88", email = "doron88@gmail.com" },
```

### Comparing `rpcclient-3.17.0/rpcclient/__main__.py` & `rpcclient-3.17.1/rpcclient/__main__.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.17.0/rpcclient/client.py` & `rpcclient-3.17.1/rpcclient/client.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.17.0/rpcclient/client_factory.py` & `rpcclient-3.17.1/rpcclient/client_factory.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.17.0/rpcclient/darwin/bluetooth.py` & `rpcclient-3.17.1/rpcclient/darwin/bluetooth.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.17.0/rpcclient/darwin/cfpreferences.py` & `rpcclient-3.17.1/rpcclient/darwin/cfpreferences.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.17.0/rpcclient/darwin/client.py` & `rpcclient-3.17.1/rpcclient/darwin/client.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.17.0/rpcclient/darwin/consts.py` & `rpcclient-3.17.1/rpcclient/darwin/consts.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.17.0/rpcclient/darwin/core_graphics.py` & `rpcclient-3.17.1/rpcclient/darwin/core_graphics.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.17.0/rpcclient/darwin/crash_reports.py` & `rpcclient-3.17.1/rpcclient/darwin/crash_reports.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.17.0/rpcclient/darwin/darwin_lief.py` & `rpcclient-3.17.1/rpcclient/darwin/darwin_lief.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.17.0/rpcclient/darwin/fs.py` & `rpcclient-3.17.1/rpcclient/darwin/fs.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.17.0/rpcclient/darwin/hid.py` & `rpcclient-3.17.1/rpcclient/darwin/hid.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.17.0/rpcclient/darwin/ioregistry.py` & `rpcclient-3.17.1/rpcclient/darwin/ioregistry.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.17.0/rpcclient/darwin/keychain.py` & `rpcclient-3.17.1/rpcclient/darwin/keychain.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.17.0/rpcclient/darwin/location.py` & `rpcclient-3.17.1/rpcclient/darwin/location.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.17.0/rpcclient/darwin/media.py` & `rpcclient-3.17.1/rpcclient/darwin/media.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.17.0/rpcclient/darwin/network.py` & `rpcclient-3.17.1/rpcclient/darwin/network.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.17.0/rpcclient/darwin/objc.py` & `rpcclient-3.17.1/rpcclient/darwin/objc.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.17.0/rpcclient/darwin/objective_c_class.py` & `rpcclient-3.17.1/rpcclient/darwin/objective_c_class.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.17.0/rpcclient/darwin/objective_c_symbol.py` & `rpcclient-3.17.1/rpcclient/darwin/objective_c_symbol.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.17.0/rpcclient/darwin/power.py` & `rpcclient-3.17.1/rpcclient/darwin/power.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.17.0/rpcclient/darwin/processes.py` & `rpcclient-3.17.1/rpcclient/darwin/processes.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.17.0/rpcclient/darwin/reports.py` & `rpcclient-3.17.1/rpcclient/darwin/reports.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.17.0/rpcclient/darwin/scpreferences.py` & `rpcclient-3.17.1/rpcclient/darwin/scpreferences.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.17.0/rpcclient/darwin/structs.py` & `rpcclient-3.17.1/rpcclient/darwin/structs.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.17.0/rpcclient/darwin/symbol.py` & `rpcclient-3.17.1/rpcclient/darwin/symbol.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.17.0/rpcclient/darwin/syslog.py` & `rpcclient-3.17.1/rpcclient/darwin/syslog.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.17.0/rpcclient/darwin/time.py` & `rpcclient-3.17.1/rpcclient/darwin/time.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.17.0/rpcclient/darwin/xpc.py` & `rpcclient-3.17.1/rpcclient/darwin/xpc.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.17.0/rpcclient/exceptions.py` & `rpcclient-3.17.1/rpcclient/exceptions.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.17.0/rpcclient/fs.py` & `rpcclient-3.17.1/rpcclient/fs.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.17.0/rpcclient/ios/accessibility.py` & `rpcclient-3.17.1/rpcclient/ios/accessibility.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.17.0/rpcclient/ios/amfi.py` & `rpcclient-3.17.1/rpcclient/ios/amfi.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.17.0/rpcclient/ios/backlight.py` & `rpcclient-3.17.1/rpcclient/ios/backlight.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.17.0/rpcclient/ios/client.py` & `rpcclient-3.17.1/rpcclient/ios/client.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.17.0/rpcclient/ios/lockdown.py` & `rpcclient-3.17.1/rpcclient/ios/lockdown.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.17.0/rpcclient/ios/mobile_gestalt.py` & `rpcclient-3.17.1/rpcclient/ios/mobile_gestalt.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.17.0/rpcclient/ios/screen_capture.py` & `rpcclient-3.17.1/rpcclient/ios/screen_capture.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.17.0/rpcclient/ios/sprinboard.py` & `rpcclient-3.17.1/rpcclient/ios/sprinboard.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.17.0/rpcclient/ios/telephony.py` & `rpcclient-3.17.1/rpcclient/ios/telephony.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.17.0/rpcclient/ios/wifi.py` & `rpcclient-3.17.1/rpcclient/ios/wifi.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.17.0/rpcclient/lief.py` & `rpcclient-3.17.1/rpcclient/lief.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.17.0/rpcclient/linux/client.py` & `rpcclient-3.17.1/rpcclient/linux/client.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.17.0/rpcclient/linux/structs.py` & `rpcclient-3.17.1/rpcclient/linux/structs.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.17.0/rpcclient/macos/apple_script.py` & `rpcclient-3.17.1/rpcclient/macos/apple_script.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.17.0/rpcclient/macos/client.py` & `rpcclient-3.17.1/rpcclient/macos/client.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.17.0/rpcclient/network.py` & `rpcclient-3.17.1/rpcclient/network.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.17.0/rpcclient/processes.py` & `rpcclient-3.17.1/rpcclient/processes.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.17.0/rpcclient/protocol.py` & `rpcclient-3.17.1/rpcclient/protocol.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.17.0/rpcclient/structs/consts.py` & `rpcclient-3.17.1/rpcclient/structs/consts.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.17.0/rpcclient/structs/generic.py` & `rpcclient-3.17.1/rpcclient/structs/generic.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.17.0/rpcclient/symbol.py` & `rpcclient-3.17.1/rpcclient/symbol.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.17.0/rpcclient/symbols_jar.py` & `rpcclient-3.17.1/rpcclient/symbols_jar.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.17.0/rpcclient/sysctl.py` & `rpcclient-3.17.1/rpcclient/sysctl.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.17.0/rpcclient/xonshrc.py` & `rpcclient-3.17.1/rpcclient/xonshrc.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.17.0/rpcclient.egg-info/PKG-INFO` & `rpcclient-3.17.1/rpcclient.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rpcclient
-Version: 3.17.0
+Version: 3.17.1
 Summary: rpcclient for connecting with the rpcserver
 Author-email: doronz88 <doron88@gmail.com>, matan <matan1008@gmail.com>
 Maintainer-email: doronz88 <doron88@gmail.com>, matan <matan1008@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
```

### Comparing `rpcclient-3.17.0/rpcclient.egg-info/SOURCES.txt` & `rpcclient-3.17.1/rpcclient.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rpcclient-3.17.0/tests/test_allocation_cleanup.py` & `rpcclient-3.17.1/tests/test_allocation_cleanup.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.17.0/tests/test_client.py` & `rpcclient-3.17.1/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.17.0/tests/test_darwin_client.py` & `rpcclient-3.17.1/tests/test_darwin_client.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.17.0/tests/test_fs.py` & `rpcclient-3.17.1/tests/test_fs.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.17.0/tests/test_objc_symbol.py` & `rpcclient-3.17.1/tests/test_objc_symbol.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.17.0/tests/test_power.py` & `rpcclient-3.17.1/tests/test_power.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.17.0/tests/test_preferences.py` & `rpcclient-3.17.1/tests/test_preferences.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.17.0/tests/test_processes.py` & `rpcclient-3.17.1/tests/test_processes.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.17.0/tests/test_socket.py` & `rpcclient-3.17.1/tests/test_socket.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.17.0/tests/test_spawn.py` & `rpcclient-3.17.1/tests/test_spawn.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.17.0/tests/test_thread_safe.py` & `rpcclient-3.17.1/tests/test_thread_safe.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.17.0/tests/test_time.py` & `rpcclient-3.17.1/tests/test_time.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.17.0/tests/test_xpc.py` & `rpcclient-3.17.1/tests/test_xpc.py`

 * *Files identical despite different names*

