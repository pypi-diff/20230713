# Comparing `tmp/rpcclient-3.16.2.tar.gz` & `tmp/rpcclient-3.17.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rpcclient-3.16.2.tar", last modified: Tue May 30 11:07:53 2023, max compression
+gzip compressed data, was "rpcclient-3.17.0.tar", last modified: Thu Jul 13 11:25:57 2023, max compression
```

## Comparing `rpcclient-3.16.2.tar` & `rpcclient-3.17.0.tar`

### file list

```diff
@@ -1,101 +1,101 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:07:53.588823 rpcclient-3.16.2/
--rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-05-30 11:07:35.000000 rpcclient-3.16.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    41739 2023-05-30 11:07:53.588823 rpcclient-3.16.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-30 11:07:35.000000 rpcclient-3.16.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-05-30 11:07:35.000000 rpcclient-3.16.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-30 11:07:35.000000 rpcclient-3.16.2/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:07:53.580823 rpcclient-3.16.2/rpcclient/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 11:07:35.000000 rpcclient-3.16.2/rpcclient/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-05-30 11:07:35.000000 rpcclient-3.16.2/rpcclient/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-05-30 11:07:35.000000 rpcclient-3.16.2/rpcclient/allocated.py
--rw-r--r--   0 runner    (1001) docker     (123)    23530 2023-05-30 11:07:35.000000 rpcclient-3.16.2/rpcclient/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-05-30 11:07:35.000000 rpcclient-3.16.2/rpcclient/client_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:07:53.584823 rpcclient-3.16.2/rpcclient/darwin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 11:07:35.000000 rpcclient-3.16.2/rpcclient/darwin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-05-30 11:07:35.000000 rpcclient-3.16.2/rpcclient/darwin/bluetooth.py
--rw-r--r--   0 runner    (1001) docker     (123)     4853 2023-05-30 11:07:35.000000 rpcclient-3.16.2/rpcclient/darwin/cfpreferences.py
--rw-r--r--   0 runner    (1001) docker     (123)    12396 2023-05-30 11:07:35.000000 rpcclient-3.16.2/rpcclient/darwin/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-30 11:07:35.000000 rpcclient-3.16.2/rpcclient/darwin/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    37890 2023-05-30 11:07:35.000000 rpcclient-3.16.2/rpcclient/darwin/consts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-05-30 11:07:35.000000 rpcclient-3.16.2/rpcclient/darwin/core_graphics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-05-30 11:07:35.000000 rpcclient-3.16.2/rpcclient/darwin/crash_reports.py
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-30 11:07:35.000000 rpcclient-3.16.2/rpcclient/darwin/darwin_lief.py
--rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-05-30 11:07:35.000000 rpcclient-3.16.2/rpcclient/darwin/fs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8438 2023-05-30 11:07:35.000000 rpcclient-3.16.2/rpcclient/darwin/hid.py
--rw-r--r--   0 runner    (1001) docker     (123)     5437 2023-05-30 11:07:35.000000 rpcclient-3.16.2/rpcclient/darwin/ioregistry.py
--rw-r--r--   0 runner    (1001) docker     (123)     3421 2023-05-30 11:07:35.000000 rpcclient-3.16.2/rpcclient/darwin/keychain.py
--rw-r--r--   0 runner    (1001) docker     (123)     3368 2023-05-30 11:07:35.000000 rpcclient-3.16.2/rpcclient/darwin/location.py
--rw-r--r--   0 runner    (1001) docker     (123)     7638 2023-05-30 11:07:35.000000 rpcclient-3.16.2/rpcclient/darwin/media.py
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-05-30 11:07:35.000000 rpcclient-3.16.2/rpcclient/darwin/network.py
--rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-05-30 11:07:35.000000 rpcclient-3.16.2/rpcclient/darwin/objc.py
--rw-r--r--   0 runner    (1001) docker     (123)     7348 2023-05-30 11:07:35.000000 rpcclient-3.16.2/rpcclient/darwin/objective_c_class.py
--rw-r--r--   0 runner    (1001) docker     (123)     7700 2023-05-30 11:07:35.000000 rpcclient-3.16.2/rpcclient/darwin/objective_c_symbol.py
--rw-r--r--   0 runner    (1001) docker     (123)     3786 2023-05-30 11:07:35.000000 rpcclient-3.16.2/rpcclient/darwin/power.py
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-30 11:07:35.000000 rpcclient-3.16.2/rpcclient/darwin/preferences.py
--rw-r--r--   0 runner    (1001) docker     (123)    33780 2023-05-30 11:07:35.000000 rpcclient-3.16.2/rpcclient/darwin/processes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-05-30 11:07:35.000000 rpcclient-3.16.2/rpcclient/darwin/reports.py
--rw-r--r--   0 runner    (1001) docker     (123)     5152 2023-05-30 11:07:35.000000 rpcclient-3.16.2/rpcclient/darwin/scpreferences.py
--rw-r--r--   0 runner    (1001) docker     (123)    29308 2023-05-30 11:07:35.000000 rpcclient-3.16.2/rpcclient/darwin/structs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-05-30 11:07:35.000000 rpcclient-3.16.2/rpcclient/darwin/symbol.py
--rw-r--r--   0 runner    (1001) docker     (123)     9397 2023-05-30 11:07:35.000000 rpcclient-3.16.2/rpcclient/darwin/syslog.py
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-05-30 11:07:35.000000 rpcclient-3.16.2/rpcclient/darwin/time.py
--rw-r--r--   0 runner    (1001) docker     (123)     4711 2023-05-30 11:07:35.000000 rpcclient-3.16.2/rpcclient/darwin/xpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4254 2023-05-30 11:07:35.000000 rpcclient-3.16.2/rpcclient/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    20680 2023-05-30 11:07:35.000000 rpcclient-3.16.2/rpcclient/fs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:07:53.584823 rpcclient-3.16.2/rpcclient/ios/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 11:07:35.000000 rpcclient-3.16.2/rpcclient/ios/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17603 2023-05-30 11:07:35.000000 rpcclient-3.16.2/rpcclient/ios/accessibility.py
--rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-05-30 11:07:35.000000 rpcclient-3.16.2/rpcclient/ios/amfi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-05-30 11:07:35.000000 rpcclient-3.16.2/rpcclient/ios/backlight.py
--rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-05-30 11:07:35.000000 rpcclient-3.16.2/rpcclient/ios/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3498 2023-05-30 11:07:35.000000 rpcclient-3.16.2/rpcclient/ios/lockdown.py
--rw-r--r--   0 runner    (1001) docker     (123)    12890 2023-05-30 11:07:35.000000 rpcclient-3.16.2/rpcclient/ios/mobile_gestalt.py
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-05-30 11:07:35.000000 rpcclient-3.16.2/rpcclient/ios/screen_capture.py
--rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-05-30 11:07:35.000000 rpcclient-3.16.2/rpcclient/ios/sprinboard.py
--rw-r--r--   0 runner    (1001) docker     (123)     3144 2023-05-30 11:07:35.000000 rpcclient-3.16.2/rpcclient/ios/telephony.py
--rw-r--r--   0 runner    (1001) docker     (123)     7605 2023-05-30 11:07:35.000000 rpcclient-3.16.2/rpcclient/ios/wifi.py
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-05-30 11:07:35.000000 rpcclient-3.16.2/rpcclient/lief.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:07:53.584823 rpcclient-3.16.2/rpcclient/linux/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 11:07:35.000000 rpcclient-3.16.2/rpcclient/linux/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-05-30 11:07:35.000000 rpcclient-3.16.2/rpcclient/linux/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-05-30 11:07:35.000000 rpcclient-3.16.2/rpcclient/linux/structs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:07:53.584823 rpcclient-3.16.2/rpcclient/macos/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 11:07:35.000000 rpcclient-3.16.2/rpcclient/macos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-05-30 11:07:35.000000 rpcclient-3.16.2/rpcclient/macos/apple_script.py
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-05-30 11:07:35.000000 rpcclient-3.16.2/rpcclient/macos/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     8707 2023-05-30 11:07:35.000000 rpcclient-3.16.2/rpcclient/network.py
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-05-30 11:07:35.000000 rpcclient-3.16.2/rpcclient/processes.py
--rw-r--r--   0 runner    (1001) docker     (123)     4430 2023-05-30 11:07:35.000000 rpcclient-3.16.2/rpcclient/protocol.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:07:53.584823 rpcclient-3.16.2/rpcclient/structs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 11:07:35.000000 rpcclient-3.16.2/rpcclient/structs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-05-30 11:07:35.000000 rpcclient-3.16.2/rpcclient/structs/consts.py
--rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-05-30 11:07:35.000000 rpcclient-3.16.2/rpcclient/structs/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     6665 2023-05-30 11:07:35.000000 rpcclient-3.16.2/rpcclient/symbol.py
--rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-05-30 11:07:35.000000 rpcclient-3.16.2/rpcclient/symbols_jar.py
--rw-r--r--   0 runner    (1001) docker     (123)     7139 2023-05-30 11:07:35.000000 rpcclient-3.16.2/rpcclient/sysctl.py
--rw-r--r--   0 runner    (1001) docker     (123)    24398 2023-05-30 11:07:35.000000 rpcclient-3.16.2/rpcclient/xonshrc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:07:53.580823 rpcclient-3.16.2/rpcclient.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    41739 2023-05-30 11:07:53.000000 rpcclient-3.16.2/rpcclient.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-05-30 11:07:53.000000 rpcclient-3.16.2/rpcclient.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 11:07:53.000000 rpcclient-3.16.2/rpcclient.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-30 11:07:53.000000 rpcclient-3.16.2/rpcclient.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-30 11:07:53.000000 rpcclient-3.16.2/rpcclient.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-30 11:07:53.000000 rpcclient-3.16.2/rpcclient.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 11:07:53.588823 rpcclient-3.16.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:07:53.588823 rpcclient-3.16.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-05-30 11:07:35.000000 rpcclient-3.16.2/tests/test_allocation_cleanup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-05-30 11:07:35.000000 rpcclient-3.16.2/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-05-30 11:07:35.000000 rpcclient-3.16.2/tests/test_core_foundation_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-05-30 11:07:35.000000 rpcclient-3.16.2/tests/test_darwin_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     4676 2023-05-30 11:07:35.000000 rpcclient-3.16.2/tests/test_fs.py
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-05-30 11:07:35.000000 rpcclient-3.16.2/tests/test_keychain.py
--rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-05-30 11:07:35.000000 rpcclient-3.16.2/tests/test_objc_symbol.py
--rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-05-30 11:07:35.000000 rpcclient-3.16.2/tests/test_power.py
--rw-r--r--   0 runner    (1001) docker     (123)     7329 2023-05-30 11:07:35.000000 rpcclient-3.16.2/tests/test_preferences.py
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-05-30 11:07:35.000000 rpcclient-3.16.2/tests/test_processes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3316 2023-05-30 11:07:35.000000 rpcclient-3.16.2/tests/test_socket.py
--rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-05-30 11:07:35.000000 rpcclient-3.16.2/tests/test_spawn.py
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-05-30 11:07:35.000000 rpcclient-3.16.2/tests/test_thread_safe.py
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-30 11:07:35.000000 rpcclient-3.16.2/tests/test_time.py
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-05-30 11:07:35.000000 rpcclient-3.16.2/tests/test_worker_processes.py
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-05-30 11:07:35.000000 rpcclient-3.16.2/tests/test_xpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:25:57.049653 rpcclient-3.17.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-07-13 11:25:39.000000 rpcclient-3.17.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    41689 2023-07-13 11:25:57.049653 rpcclient-3.17.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-13 11:25:39.000000 rpcclient-3.17.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-07-13 11:25:39.000000 rpcclient-3.17.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-13 11:25:39.000000 rpcclient-3.17.0/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:25:57.041653 rpcclient-3.17.0/rpcclient/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 11:25:39.000000 rpcclient-3.17.0/rpcclient/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-07-13 11:25:39.000000 rpcclient-3.17.0/rpcclient/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-07-13 11:25:39.000000 rpcclient-3.17.0/rpcclient/allocated.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23671 2023-07-13 11:25:39.000000 rpcclient-3.17.0/rpcclient/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3218 2023-07-13 11:25:39.000000 rpcclient-3.17.0/rpcclient/client_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:25:57.045653 rpcclient-3.17.0/rpcclient/darwin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 11:25:39.000000 rpcclient-3.17.0/rpcclient/darwin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-07-13 11:25:39.000000 rpcclient-3.17.0/rpcclient/darwin/bluetooth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4853 2023-07-13 11:25:39.000000 rpcclient-3.17.0/rpcclient/darwin/cfpreferences.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12667 2023-07-13 11:25:39.000000 rpcclient-3.17.0/rpcclient/darwin/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-13 11:25:39.000000 rpcclient-3.17.0/rpcclient/darwin/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37890 2023-07-13 11:25:39.000000 rpcclient-3.17.0/rpcclient/darwin/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-07-13 11:25:39.000000 rpcclient-3.17.0/rpcclient/darwin/core_graphics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-07-13 11:25:39.000000 rpcclient-3.17.0/rpcclient/darwin/crash_reports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-13 11:25:39.000000 rpcclient-3.17.0/rpcclient/darwin/darwin_lief.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-07-13 11:25:39.000000 rpcclient-3.17.0/rpcclient/darwin/fs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8438 2023-07-13 11:25:39.000000 rpcclient-3.17.0/rpcclient/darwin/hid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5437 2023-07-13 11:25:39.000000 rpcclient-3.17.0/rpcclient/darwin/ioregistry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3421 2023-07-13 11:25:39.000000 rpcclient-3.17.0/rpcclient/darwin/keychain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3368 2023-07-13 11:25:39.000000 rpcclient-3.17.0/rpcclient/darwin/location.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7638 2023-07-13 11:25:39.000000 rpcclient-3.17.0/rpcclient/darwin/media.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-07-13 11:25:39.000000 rpcclient-3.17.0/rpcclient/darwin/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-07-13 11:25:39.000000 rpcclient-3.17.0/rpcclient/darwin/objc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7588 2023-07-13 11:25:39.000000 rpcclient-3.17.0/rpcclient/darwin/objective_c_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7990 2023-07-13 11:25:39.000000 rpcclient-3.17.0/rpcclient/darwin/objective_c_symbol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3786 2023-07-13 11:25:39.000000 rpcclient-3.17.0/rpcclient/darwin/power.py
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-07-13 11:25:39.000000 rpcclient-3.17.0/rpcclient/darwin/preferences.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33780 2023-07-13 11:25:39.000000 rpcclient-3.17.0/rpcclient/darwin/processes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-07-13 11:25:39.000000 rpcclient-3.17.0/rpcclient/darwin/reports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5152 2023-07-13 11:25:39.000000 rpcclient-3.17.0/rpcclient/darwin/scpreferences.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29308 2023-07-13 11:25:39.000000 rpcclient-3.17.0/rpcclient/darwin/structs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-07-13 11:25:39.000000 rpcclient-3.17.0/rpcclient/darwin/symbol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9396 2023-07-13 11:25:39.000000 rpcclient-3.17.0/rpcclient/darwin/syslog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-07-13 11:25:39.000000 rpcclient-3.17.0/rpcclient/darwin/time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8327 2023-07-13 11:25:39.000000 rpcclient-3.17.0/rpcclient/darwin/xpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4254 2023-07-13 11:25:39.000000 rpcclient-3.17.0/rpcclient/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20680 2023-07-13 11:25:39.000000 rpcclient-3.17.0/rpcclient/fs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:25:57.045653 rpcclient-3.17.0/rpcclient/ios/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 11:25:39.000000 rpcclient-3.17.0/rpcclient/ios/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17603 2023-07-13 11:25:39.000000 rpcclient-3.17.0/rpcclient/ios/accessibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-07-13 11:25:39.000000 rpcclient-3.17.0/rpcclient/ios/amfi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-07-13 11:25:39.000000 rpcclient-3.17.0/rpcclient/ios/backlight.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-07-13 11:25:39.000000 rpcclient-3.17.0/rpcclient/ios/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3498 2023-07-13 11:25:39.000000 rpcclient-3.17.0/rpcclient/ios/lockdown.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12890 2023-07-13 11:25:39.000000 rpcclient-3.17.0/rpcclient/ios/mobile_gestalt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-07-13 11:25:39.000000 rpcclient-3.17.0/rpcclient/ios/screen_capture.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-07-13 11:25:39.000000 rpcclient-3.17.0/rpcclient/ios/sprinboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3144 2023-07-13 11:25:39.000000 rpcclient-3.17.0/rpcclient/ios/telephony.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7605 2023-07-13 11:25:39.000000 rpcclient-3.17.0/rpcclient/ios/wifi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-07-13 11:25:39.000000 rpcclient-3.17.0/rpcclient/lief.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:25:57.045653 rpcclient-3.17.0/rpcclient/linux/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 11:25:39.000000 rpcclient-3.17.0/rpcclient/linux/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-13 11:25:39.000000 rpcclient-3.17.0/rpcclient/linux/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-07-13 11:25:39.000000 rpcclient-3.17.0/rpcclient/linux/structs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:25:57.045653 rpcclient-3.17.0/rpcclient/macos/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 11:25:39.000000 rpcclient-3.17.0/rpcclient/macos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-07-13 11:25:39.000000 rpcclient-3.17.0/rpcclient/macos/apple_script.py
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-07-13 11:25:39.000000 rpcclient-3.17.0/rpcclient/macos/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8707 2023-07-13 11:25:39.000000 rpcclient-3.17.0/rpcclient/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-07-13 11:25:39.000000 rpcclient-3.17.0/rpcclient/processes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4430 2023-07-13 11:25:39.000000 rpcclient-3.17.0/rpcclient/protocol.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:25:57.049653 rpcclient-3.17.0/rpcclient/structs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 11:25:39.000000 rpcclient-3.17.0/rpcclient/structs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-07-13 11:25:39.000000 rpcclient-3.17.0/rpcclient/structs/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-07-13 11:25:39.000000 rpcclient-3.17.0/rpcclient/structs/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6782 2023-07-13 11:25:39.000000 rpcclient-3.17.0/rpcclient/symbol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-07-13 11:25:39.000000 rpcclient-3.17.0/rpcclient/symbols_jar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7139 2023-07-13 11:25:39.000000 rpcclient-3.17.0/rpcclient/sysctl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24398 2023-07-13 11:25:39.000000 rpcclient-3.17.0/rpcclient/xonshrc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:25:57.041653 rpcclient-3.17.0/rpcclient.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    41689 2023-07-13 11:25:57.000000 rpcclient-3.17.0/rpcclient.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-07-13 11:25:57.000000 rpcclient-3.17.0/rpcclient.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 11:25:57.000000 rpcclient-3.17.0/rpcclient.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-13 11:25:57.000000 rpcclient-3.17.0/rpcclient.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-07-13 11:25:57.000000 rpcclient-3.17.0/rpcclient.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-13 11:25:57.000000 rpcclient-3.17.0/rpcclient.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 11:25:57.049653 rpcclient-3.17.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:25:57.049653 rpcclient-3.17.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-07-13 11:25:39.000000 rpcclient-3.17.0/tests/test_allocation_cleanup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-07-13 11:25:39.000000 rpcclient-3.17.0/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-13 11:25:39.000000 rpcclient-3.17.0/tests/test_core_foundation_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-07-13 11:25:39.000000 rpcclient-3.17.0/tests/test_darwin_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4676 2023-07-13 11:25:39.000000 rpcclient-3.17.0/tests/test_fs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-13 11:25:39.000000 rpcclient-3.17.0/tests/test_keychain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-07-13 11:25:39.000000 rpcclient-3.17.0/tests/test_objc_symbol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-07-13 11:25:39.000000 rpcclient-3.17.0/tests/test_power.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7329 2023-07-13 11:25:39.000000 rpcclient-3.17.0/tests/test_preferences.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-07-13 11:25:39.000000 rpcclient-3.17.0/tests/test_processes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3316 2023-07-13 11:25:39.000000 rpcclient-3.17.0/tests/test_socket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-07-13 11:25:39.000000 rpcclient-3.17.0/tests/test_spawn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-07-13 11:25:39.000000 rpcclient-3.17.0/tests/test_thread_safe.py
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-07-13 11:25:39.000000 rpcclient-3.17.0/tests/test_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-07-13 11:25:39.000000 rpcclient-3.17.0/tests/test_worker_processes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-07-13 11:25:39.000000 rpcclient-3.17.0/tests/test_xpc.py
```

### Comparing `rpcclient-3.16.2/LICENSE` & `rpcclient-3.17.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rpcclient-3.16.2/PKG-INFO` & `rpcclient-3.17.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rpcclient
-Version: 3.16.2
+Version: 3.17.0
 Summary: rpcclient for connecting with the rpcserver
 Author-email: doronz88 <doron88@gmail.com>, matan <matan1008@gmail.com>
 Maintainer-email: doronz88 <doron88@gmail.com>, matan <matan1008@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
@@ -681,21 +681,20 @@
         
 Project-URL: Homepage, https://github.com/doronz88/rpc-project
 Project-URL: Bug Reports, https://github.com/doronz88/rpc-project/issues
 Keywords: ios,macos,linux,automation,remote-shell,remote-control,ipython
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: docs
 License-File: LICENSE
 
 # rpcclient
```

### Comparing `rpcclient-3.16.2/pyproject.toml` & `rpcclient-3.17.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 [project]
 name = "rpcclient"
-version = "3.16.2"
+version = "3.17.0"
 description = "rpcclient for connecting with the rpcserver"
 readme = "README.md"
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 license = { file = "LICENSE" }
 keywords = ["ios", "macos", "linux", "automation", "remote-shell", "remote-control", "ipython"]
 authors = [
     { name = "doronz88", email = "doron88@gmail.com" },
     { name = "matan", email = "matan1008@gmail.com" }
 ]
 maintainers = [
     { name = "doronz88", email = "doron88@gmail.com" },
     { name = "matan", email = "matan1008@gmail.com" }
 ]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3 :: Only",
 ]
 dynamic = ["dependencies"]
@@ -32,15 +31,16 @@
 docs = ["toml", "myst_parser", "sphinx", "sphinx-rtd-theme"]
 
 [project.urls]
 "Homepage" = "https://github.com/doronz88/rpc-project"
 "Bug Reports" = "https://github.com/doronz88/rpc-project/issues"
 
 [project.scripts]
-rpcclient = "rpcclient.__main__:cli"
+rpcclient = "rpcclient.__main__:rpcclient"
+rpclocal = "rpcclient.__main__:rpclocal"
 
 [tool.setuptools.packages.find]
 exclude = ["docs*", "tests*"]
 
 [tool.setuptools.dynamic]
 dependencies = { file = ["requirements.txt"] }
```

### Comparing `rpcclient-3.16.2/rpcclient/__main__.py` & `rpcclient-3.17.0/rpcclient/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,34 +1,41 @@
 import logging
 
 import click
 import coloredlogs
 
-from rpcclient.client_factory import create_tcp_client
+from rpcclient.client_factory import create_local, create_tcp_client
 from rpcclient.protocol import DEFAULT_PORT
 
 coloredlogs.install(level=logging.DEBUG)
 
 logging.getLogger('asyncio').disabled = True
 logging.getLogger('parso').disabled = True
 logging.getLogger('parso.cache').disabled = True
 logging.getLogger('parso.python.diff').disabled = True
 logging.getLogger('blib2to3.pgen2.driver').disabled = True
 logging.getLogger('humanfriendly.prompts').disabled = True
 
 
 @click.command()
+def rpclocal() -> None:
+    """ connect to local machine """
+    create_local().interactive()
+
+
+@click.command()
 @click.argument('hostname')
 @click.option('-p', '--port', type=click.INT, default=DEFAULT_PORT)
 @click.option('-r', '--rebind-symbols', is_flag=True, help='reload all symbols upon connection')
 @click.option('-l', '--load-all-libraries', is_flag=True, help='load all libraries')
-def cli(hostname: str, port: int, rebind_symbols: bool, load_all_libraries: bool):
+def rpcclient(hostname: str, port: int, rebind_symbols: bool, load_all_libraries: bool):
+    """ connect to remote host """
     client = create_tcp_client(hostname, port=port)
     if load_all_libraries:
         client.load_all_libraries(rebind_symbols=False)
     if rebind_symbols:
         client.rebind_symbols()
     client.interactive()
 
 
 if __name__ == '__main__':
-    cli()
+    rpcclient()
```

### Comparing `rpcclient-3.16.2/rpcclient/client.py` & `rpcclient-3.17.0/rpcclient/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -440,25 +440,27 @@
     def freeing(self, symbol):
         try:
             yield symbol
         finally:
             if symbol:
                 self.symbols.free(symbol)
 
-    def interactive(self):
+    def interactive(self, additional_namespace: typing.Mapping = None):
         """ Start an interactive shell """
         sys.argv = ['a']
         c = Config()
         c.IPCompleter.use_jedi = False
         c.InteractiveShellApp.exec_lines = [
             '''IPython.get_ipython().events.register('pre_run_cell', p._ipython_run_cell_hook)'''
         ]
         c.TerminalInteractiveShell.autoformatter = None
         namespace = globals()
         namespace.update({'p': self, 'symbols': self.symbols})
+        if additional_namespace is not None:
+            namespace.update(additional_namespace)
         print(USAGE)
         IPython.start_ipython(config=c, user_ns=namespace)
 
     def _add_global(self, name: str, value) -> None:
         globals()[name] = value
 
     def _ipython_run_cell_hook(self, info):
```

### Comparing `rpcclient-3.16.2/rpcclient/darwin/bluetooth.py` & `rpcclient-3.17.0/rpcclient/darwin/bluetooth.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.16.2/rpcclient/darwin/cfpreferences.py` & `rpcclient-3.17.0/rpcclient/darwin/cfpreferences.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.16.2/rpcclient/darwin/client.py` & `rpcclient-3.17.0/rpcclient/darwin/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -99,14 +99,20 @@
         self.keychain = Keychain(self)
         self.network = DarwinNetwork(self)
         self.power = Power(self)
         self.loaded_objc_classes = []
         self._NSPropertyListSerialization = self.objc_get_class('NSPropertyListSerialization')
         self._CFNullTypeID = self.symbols.CFNullGetTypeID()
 
+    def interactive(self, additional_namespace: typing.Mapping = None):
+        if additional_namespace is None:
+            additional_namespace = {}
+        additional_namespace['CFSTR'] = self.cf
+        super().interactive(additional_namespace=additional_namespace)
+
     @property
     def images(self) -> typing.List[DyldImage]:
         m = []
         for i in range(self.symbols._dyld_image_count()):
             module_name = self.symbols._dyld_get_image_name(i).peek_str()
             base_address = self.symbols._dyld_get_image_header(i)
             m.append(
```

### Comparing `rpcclient-3.16.2/rpcclient/darwin/consts.py` & `rpcclient-3.17.0/rpcclient/darwin/consts.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.16.2/rpcclient/darwin/core_graphics.py` & `rpcclient-3.17.0/rpcclient/darwin/core_graphics.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.16.2/rpcclient/darwin/crash_reports.py` & `rpcclient-3.17.0/rpcclient/darwin/crash_reports.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.16.2/rpcclient/darwin/darwin_lief.py` & `rpcclient-3.17.0/rpcclient/darwin/darwin_lief.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.16.2/rpcclient/darwin/fs.py` & `rpcclient-3.17.0/rpcclient/darwin/fs.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.16.2/rpcclient/darwin/hid.py` & `rpcclient-3.17.0/rpcclient/darwin/hid.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.16.2/rpcclient/darwin/ioregistry.py` & `rpcclient-3.17.0/rpcclient/darwin/ioregistry.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.16.2/rpcclient/darwin/keychain.py` & `rpcclient-3.17.0/rpcclient/darwin/keychain.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.16.2/rpcclient/darwin/location.py` & `rpcclient-3.17.0/rpcclient/darwin/location.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.16.2/rpcclient/darwin/media.py` & `rpcclient-3.17.0/rpcclient/darwin/media.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.16.2/rpcclient/darwin/network.py` & `rpcclient-3.17.0/rpcclient/darwin/network.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.16.2/rpcclient/darwin/objc.py` & `rpcclient-3.17.0/rpcclient/darwin/objc.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.16.2/rpcclient/darwin/objective_c_class.py` & `rpcclient-3.17.0/rpcclient/darwin/objective_c_class.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from collections import namedtuple
 from functools import partial
 from pathlib import Path
-from typing import Mapping
+from typing import Mapping, Optional
 
 from pygments import highlight
 from pygments.formatters import TerminalTrueColorFormatter
 from pygments.lexers import ObjectiveCLexer
 
 from rpcclient.darwin import objc
 from rpcclient.exceptions import GettingObjectiveCClassError
@@ -81,19 +81,25 @@
             objc.Property(name=prop['name'], attributes=objc.convert_encoded_property_attributes(prop['attributes']))
             for prop in class_description['properties']
         ]
         self.methods = [
             objc.Method.from_data(method, self._client) for method in class_description['methods']
         ]
 
-    def show(self):
+    def show(self, dump_to: Optional[str] = None):
         """
         Print to terminal the highlighted class description.
+        :param dump_to: directory to dump.
         """
-        print(highlight(str(self), ObjectiveCLexer(), TerminalTrueColorFormatter(style='native')))
+        formatted = str(self)
+        print(highlight(formatted, ObjectiveCLexer(), TerminalTrueColorFormatter(style='native')))
+
+        if dump_to is None:
+            return
+        (Path(dump_to) / f'{self.name}.m').expanduser().write_text(formatted)
 
     def objc_call(self, sel: str, *args, **kwargs):
         """
         Invoke a selector on the given class object.
         :param sel: Selector name.
         :return: whatever the selector returned as a symbol.
         """
```

### Comparing `rpcclient-3.16.2/rpcclient/darwin/objective_c_symbol.py` & `rpcclient-3.17.0/rpcclient/darwin/objective_c_symbol.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 from contextlib import suppress
 from dataclasses import dataclass
 from functools import partial
+from pathlib import Path
+from typing import Optional
 
 from pygments import highlight
 from pygments.formatters import TerminalTrueColorFormatter
 from pygments.lexers import ObjectiveCLexer
 
 from rpcclient.darwin import objc
 from rpcclient.darwin.objective_c_class import Class
@@ -72,20 +74,26 @@
         class_wrapper = Class(self._client, class_object)
 
         self.ivars = ivars_list
         self.methods = methods_list
         self.properties = properties_list
         self.class_ = class_wrapper
 
-    def show(self, recursive: bool = False):
+    def show(self, dump_to: Optional[str] = None, recursive: bool = False):
         """
         Print to terminal the highlighted class description.
+        :param dump_to: directory to dump.
         :param recursive: Show methods of super classes.
         """
-        print(highlight(self._to_str(recursive), ObjectiveCLexer(), TerminalTrueColorFormatter(style='native')))
+        formatted = self._to_str(recursive)
+        print(highlight(formatted, ObjectiveCLexer(), TerminalTrueColorFormatter(style='native')))
+
+        if dump_to is None:
+            return
+        (Path(dump_to) / f'{self.class_.name}.m').expanduser().write_text(formatted)
 
     def objc_call(self, selector: str, *params, **kwargs):
         """
         Make objc_call() from self return ObjectiveCSymbol when it's an objc symbol.
         :param selector: Selector to execute.
         :param params: Additional parameters.
         :return: ObjectiveCSymbol when return type is an objc symbol.
```

### Comparing `rpcclient-3.16.2/rpcclient/darwin/power.py` & `rpcclient-3.17.0/rpcclient/darwin/power.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.16.2/rpcclient/darwin/processes.py` & `rpcclient-3.17.0/rpcclient/darwin/processes.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.16.2/rpcclient/darwin/reports.py` & `rpcclient-3.17.0/rpcclient/darwin/reports.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.16.2/rpcclient/darwin/scpreferences.py` & `rpcclient-3.17.0/rpcclient/darwin/scpreferences.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.16.2/rpcclient/darwin/structs.py` & `rpcclient-3.17.0/rpcclient/darwin/structs.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.16.2/rpcclient/darwin/symbol.py` & `rpcclient-3.17.0/rpcclient/darwin/symbol.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.16.2/rpcclient/darwin/syslog.py` & `rpcclient-3.17.0/rpcclient/darwin/syslog.py`

 * *Files 0% similar despite different names*

```diff
@@ -178,17 +178,17 @@
         for p in self._client.processes.list():
             if p.pid == 0:
                 continue
             if expression and expression not in p.basename:
                 continue
             try:
                 self._set_harlogger_for_process(value, p)
-                logger.info(f'{"Enabled" if value else "Disabled"} for {p.name}')
+                logger.info(f'{"Enabled" if value else "Disabled"} for {p.basename}')
             except BadReturnValueError:
-                logger.error(f'Failed To enabled for {p.name}')
+                logger.error(f'Failed To enabled for {p}')
         self.set_har_capture_global(True)
 
     def set_unredacted_logs(self, enable: bool = True):
         """
         enable/disable unredacted logs (allows seeing the <private> strings)
         https://github.com/EthanArbuckle/unredact-private-os_logs
         """
```

### Comparing `rpcclient-3.16.2/rpcclient/darwin/time.py` & `rpcclient-3.17.0/rpcclient/darwin/time.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.16.2/rpcclient/exceptions.py` & `rpcclient-3.17.0/rpcclient/exceptions.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.16.2/rpcclient/fs.py` & `rpcclient-3.17.0/rpcclient/fs.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.16.2/rpcclient/ios/accessibility.py` & `rpcclient-3.17.0/rpcclient/ios/accessibility.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.16.2/rpcclient/ios/amfi.py` & `rpcclient-3.17.0/rpcclient/ios/amfi.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,15 +10,16 @@
     """ AMFI utils """
 
     def __init__(self, client):
         self._client = client
         self._load_amfi()
 
     def set_developer_mode_status(self, enabled: bool) -> None:
-        cfreply = self._client.xpc.send_message('com.apple.amfi.xpc', {'action': int(not (enabled))}, False)['cfreply']
+        cfreply = self._client.xpc.send_message_using_cf_serialization(
+            'com.apple.amfi.xpc', {'action': int(not (enabled))}, False)['cfreply']
         raw_response = list(cfreply.values())[0]
         if b'success' not in raw_response:
             raise RpcSetDeveloperModeError()
 
     @property
     def developer_mode_status(self) -> bool:
         """ get Developer Mode status """
```

### Comparing `rpcclient-3.16.2/rpcclient/ios/backlight.py` & `rpcclient-3.17.0/rpcclient/ios/backlight.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.16.2/rpcclient/ios/client.py` & `rpcclient-3.17.0/rpcclient/ios/client.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.16.2/rpcclient/ios/lockdown.py` & `rpcclient-3.17.0/rpcclient/ios/lockdown.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.16.2/rpcclient/ios/mobile_gestalt.py` & `rpcclient-3.17.0/rpcclient/ios/mobile_gestalt.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.16.2/rpcclient/ios/screen_capture.py` & `rpcclient-3.17.0/rpcclient/ios/screen_capture.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.16.2/rpcclient/ios/sprinboard.py` & `rpcclient-3.17.0/rpcclient/ios/sprinboard.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.16.2/rpcclient/ios/telephony.py` & `rpcclient-3.17.0/rpcclient/ios/telephony.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.16.2/rpcclient/ios/wifi.py` & `rpcclient-3.17.0/rpcclient/ios/wifi.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.16.2/rpcclient/lief.py` & `rpcclient-3.17.0/rpcclient/lief.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.16.2/rpcclient/linux/client.py` & `rpcclient-3.17.0/rpcclient/linux/client.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.16.2/rpcclient/linux/structs.py` & `rpcclient-3.17.0/rpcclient/linux/structs.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.16.2/rpcclient/macos/apple_script.py` & `rpcclient-3.17.0/rpcclient/macos/apple_script.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.16.2/rpcclient/macos/client.py` & `rpcclient-3.17.0/rpcclient/macos/client.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.16.2/rpcclient/network.py` & `rpcclient-3.17.0/rpcclient/network.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.16.2/rpcclient/processes.py` & `rpcclient-3.17.0/rpcclient/processes.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.16.2/rpcclient/protocol.py` & `rpcclient-3.17.0/rpcclient/protocol.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.16.2/rpcclient/structs/consts.py` & `rpcclient-3.17.0/rpcclient/structs/consts.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.16.2/rpcclient/structs/generic.py` & `rpcclient-3.17.0/rpcclient/structs/generic.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.16.2/rpcclient/symbol.py` & `rpcclient-3.17.0/rpcclient/symbol.py`

 * *Files 2% similar despite different names*

```diff
@@ -140,14 +140,19 @@
 
     @property
     def c_uint16(self) -> int:
         """ cast to c_uint16 """
         return ctypes.c_uint16(self).value
 
     @property
+    def c_bool(self) -> bool:
+        """ cast to c_bool """
+        return ctypes.c_bool(self).value
+
+    @property
     def dl_info(self) -> Container:
         dl_info = Dl_info(self._client)
         sizeof = dl_info.sizeof()
         with self._client.safe_malloc(sizeof) as info:
             if 0 == self._client.symbols.dladdr(self, info):
                 self._client.raise_errno_exception(f'failed to extract info for: {self}')
             return dl_info.parse_stream(info)
```

### Comparing `rpcclient-3.16.2/rpcclient/symbols_jar.py` & `rpcclient-3.17.0/rpcclient/symbols_jar.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.16.2/rpcclient/sysctl.py` & `rpcclient-3.17.0/rpcclient/sysctl.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.16.2/rpcclient/xonshrc.py` & `rpcclient-3.17.0/rpcclient/xonshrc.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.16.2/rpcclient.egg-info/PKG-INFO` & `rpcclient-3.17.0/rpcclient.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rpcclient
-Version: 3.16.2
+Version: 3.17.0
 Summary: rpcclient for connecting with the rpcserver
 Author-email: doronz88 <doron88@gmail.com>, matan <matan1008@gmail.com>
 Maintainer-email: doronz88 <doron88@gmail.com>, matan <matan1008@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
@@ -681,21 +681,20 @@
         
 Project-URL: Homepage, https://github.com/doronz88/rpc-project
 Project-URL: Bug Reports, https://github.com/doronz88/rpc-project/issues
 Keywords: ios,macos,linux,automation,remote-shell,remote-control,ipython
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: docs
 License-File: LICENSE
 
 # rpcclient
```

### Comparing `rpcclient-3.16.2/rpcclient.egg-info/SOURCES.txt` & `rpcclient-3.17.0/rpcclient.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rpcclient-3.16.2/tests/test_allocation_cleanup.py` & `rpcclient-3.17.0/tests/test_allocation_cleanup.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.16.2/tests/test_client.py` & `rpcclient-3.17.0/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.16.2/tests/test_darwin_client.py` & `rpcclient-3.17.0/tests/test_darwin_client.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.16.2/tests/test_fs.py` & `rpcclient-3.17.0/tests/test_fs.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.16.2/tests/test_objc_symbol.py` & `rpcclient-3.17.0/tests/test_objc_symbol.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.16.2/tests/test_power.py` & `rpcclient-3.17.0/tests/test_power.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.16.2/tests/test_preferences.py` & `rpcclient-3.17.0/tests/test_preferences.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.16.2/tests/test_processes.py` & `rpcclient-3.17.0/tests/test_processes.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.16.2/tests/test_socket.py` & `rpcclient-3.17.0/tests/test_socket.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.16.2/tests/test_spawn.py` & `rpcclient-3.17.0/tests/test_spawn.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.16.2/tests/test_thread_safe.py` & `rpcclient-3.17.0/tests/test_thread_safe.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.16.2/tests/test_time.py` & `rpcclient-3.17.0/tests/test_time.py`

 * *Files identical despite different names*

