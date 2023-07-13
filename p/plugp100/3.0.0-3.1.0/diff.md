# Comparing `tmp/plugp100-3.0.0.tar.gz` & `tmp/plugp100-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plugp100-3.0.0.tar", last modified: Fri Jun 30 06:29:54 2023, max compression
+gzip compressed data, was "plugp100-3.1.0.tar", last modified: Thu Jul 13 17:24:43 2023, max compression
```

## Comparing `plugp100-3.0.0.tar` & `plugp100-3.1.0.tar`

### file list

```diff
@@ -1,59 +1,77 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 06:29:54.495865 plugp100-3.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-30 06:29:42.000000 plugp100-3.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-30 06:29:42.000000 plugp100-3.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-06-30 06:29:54.495865 plugp100-3.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-06-30 06:29:42.000000 plugp100-3.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 06:29:54.491865 plugp100-3.0.0/plugp100/
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-06-30 06:29:42.000000 plugp100-3.0.0/plugp100/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 06:29:54.491865 plugp100-3.0.0/plugp100/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 06:29:42.000000 plugp100-3.0.0/plugp100/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-06-30 06:29:42.000000 plugp100-3.0.0/plugp100/api/ledstrip_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-06-30 06:29:42.000000 plugp100-3.0.0/plugp100/api/light_device.py
--rw-r--r--   0 runner    (1001) docker     (123)    14668 2023-06-30 06:29:42.000000 plugp100-3.0.0/plugp100/api/light_effect.py
--rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-06-30 06:29:42.000000 plugp100-3.0.0/plugp100/api/light_effect_preset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-06-30 06:29:42.000000 plugp100-3.0.0/plugp100/api/plug_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     7867 2023-06-30 06:29:42.000000 plugp100-3.0.0/plugp100/api/tapo_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 06:29:54.491865 plugp100-3.0.0/plugp100/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 06:29:42.000000 plugp100-3.0.0/plugp100/common/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 06:29:54.491865 plugp100-3.0.0/plugp100/common/functional/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 06:29:42.000000 plugp100-3.0.0/plugp100/common/functional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4309 2023-06-30 06:29:42.000000 plugp100-3.0.0/plugp100/common/functional/either.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 06:29:54.491865 plugp100-3.0.0/plugp100/common/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 06:29:42.000000 plugp100-3.0.0/plugp100/common/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-06-30 06:29:42.000000 plugp100-3.0.0/plugp100/common/utils/http_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-30 06:29:42.000000 plugp100-3.0.0/plugp100/common/utils/json_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-06-30 06:29:42.000000 plugp100-3.0.0/plugp100/discover.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 06:29:54.491865 plugp100-3.0.0/plugp100/encryption/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 06:29:42.000000 plugp100-3.0.0/plugp100/encryption/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-30 06:29:42.000000 plugp100-3.0.0/plugp100/encryption/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-06-30 06:29:42.000000 plugp100-3.0.0/plugp100/encryption/key_pair.py
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-06-30 06:29:42.000000 plugp100-3.0.0/plugp100/encryption/tp_link_cipher.py
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-06-30 06:29:42.000000 plugp100-3.0.0/plugp100/example.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 06:29:54.491865 plugp100-3.0.0/plugp100/requests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 06:29:42.000000 plugp100-3.0.0/plugp100/requests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-30 06:29:42.000000 plugp100-3.0.0/plugp100/requests/handshake_params.py
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-06-30 06:29:42.000000 plugp100-3.0.0/plugp100/requests/login_device.py
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-30 06:29:42.000000 plugp100-3.0.0/plugp100/requests/secure_passthrough_params.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 06:29:54.495865 plugp100-3.0.0/plugp100/requests/set_device_info/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 06:29:42.000000 plugp100-3.0.0/plugp100/requests/set_device_info/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-30 06:29:42.000000 plugp100-3.0.0/plugp100/requests/set_device_info/set_light_color_info_params.py
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-06-30 06:29:42.000000 plugp100-3.0.0/plugp100/requests/set_device_info/set_light_info_params.py
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-30 06:29:42.000000 plugp100-3.0.0/plugp100/requests/set_device_info/set_plug_info_params.py
--rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-06-30 06:29:42.000000 plugp100-3.0.0/plugp100/requests/tapo_request.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 06:29:54.495865 plugp100-3.0.0/plugp100/responses/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 06:29:42.000000 plugp100-3.0.0/plugp100/responses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-06-30 06:29:42.000000 plugp100-3.0.0/plugp100/responses/child_device_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-06-30 06:29:42.000000 plugp100-3.0.0/plugp100/responses/device_state.py
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-06-30 06:29:42.000000 plugp100-3.0.0/plugp100/responses/energy_info.py
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-30 06:29:42.000000 plugp100-3.0.0/plugp100/responses/power_info.py
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-06-30 06:29:42.000000 plugp100-3.0.0/plugp100/responses/tapo_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-06-30 06:29:42.000000 plugp100-3.0.0/plugp100/responses/tapo_response.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 06:29:54.491865 plugp100-3.0.0/plugp100.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-06-30 06:29:54.000000 plugp100-3.0.0/plugp100.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-06-30 06:29:54.000000 plugp100-3.0.0/plugp100.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 06:29:54.000000 plugp100-3.0.0/plugp100.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-30 06:29:54.000000 plugp100-3.0.0/plugp100.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-30 06:29:54.000000 plugp100-3.0.0/plugp100.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-30 06:29:42.000000 plugp100-3.0.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-30 06:29:54.495865 plugp100-3.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-06-30 06:29:42.000000 plugp100-3.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:24:43.195034 plugp100-3.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-13 17:24:30.000000 plugp100-3.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-13 17:24:30.000000 plugp100-3.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-07-13 17:24:43.195034 plugp100-3.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-07-13 17:24:30.000000 plugp100-3.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:24:43.187033 plugp100-3.1.0/plugp100/
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-07-13 17:24:30.000000 plugp100-3.1.0/plugp100/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:24:43.191033 plugp100-3.1.0/plugp100/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 17:24:30.000000 plugp100-3.1.0/plugp100/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:24:43.191033 plugp100-3.1.0/plugp100/api/hub/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 17:24:30.000000 plugp100-3.1.0/plugp100/api/hub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6196 2023-07-13 17:24:30.000000 plugp100-3.1.0/plugp100/api/hub/hub_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-07-13 17:24:30.000000 plugp100-3.1.0/plugp100/api/hub/hub_device_tracker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-07-13 17:24:30.000000 plugp100-3.1.0/plugp100/api/hub/s200b_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-07-13 17:24:30.000000 plugp100-3.1.0/plugp100/api/hub/t100_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-07-13 17:24:30.000000 plugp100-3.1.0/plugp100/api/hub/t110_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-07-13 17:24:30.000000 plugp100-3.1.0/plugp100/api/hub/t31x_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-07-13 17:24:30.000000 plugp100-3.1.0/plugp100/api/ledstrip_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4691 2023-07-13 17:24:30.000000 plugp100-3.1.0/plugp100/api/light_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14668 2023-07-13 17:24:30.000000 plugp100-3.1.0/plugp100/api/light_effect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-07-13 17:24:30.000000 plugp100-3.1.0/plugp100/api/light_effect_preset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-07-13 17:24:30.000000 plugp100-3.1.0/plugp100/api/plug_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12772 2023-07-13 17:24:30.000000 plugp100-3.1.0/plugp100/api/tapo_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:24:43.191033 plugp100-3.1.0/plugp100/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 17:24:30.000000 plugp100-3.1.0/plugp100/common/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:24:43.191033 plugp100-3.1.0/plugp100/common/functional/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 17:24:30.000000 plugp100-3.1.0/plugp100/common/functional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-07-13 17:24:30.000000 plugp100-3.1.0/plugp100/common/functional/either.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-07-13 17:24:30.000000 plugp100-3.1.0/plugp100/common/state_tracker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:24:43.191033 plugp100-3.1.0/plugp100/common/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 17:24:30.000000 plugp100-3.1.0/plugp100/common/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-07-13 17:24:30.000000 plugp100-3.1.0/plugp100/common/utils/http_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-13 17:24:30.000000 plugp100-3.1.0/plugp100/common/utils/json_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-07-13 17:24:30.000000 plugp100-3.1.0/plugp100/discover.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:24:43.191033 plugp100-3.1.0/plugp100/encryption/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 17:24:30.000000 plugp100-3.1.0/plugp100/encryption/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-07-13 17:24:30.000000 plugp100-3.1.0/plugp100/encryption/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-07-13 17:24:30.000000 plugp100-3.1.0/plugp100/encryption/key_pair.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-07-13 17:24:30.000000 plugp100-3.1.0/plugp100/encryption/tp_link_cipher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-07-13 17:24:30.000000 plugp100-3.1.0/plugp100/example.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:24:43.191033 plugp100-3.1.0/plugp100/requests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 17:24:30.000000 plugp100-3.1.0/plugp100/requests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-13 17:24:30.000000 plugp100-3.1.0/plugp100/requests/handshake_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-07-13 17:24:30.000000 plugp100-3.1.0/plugp100/requests/login_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-13 17:24:30.000000 plugp100-3.1.0/plugp100/requests/secure_passthrough_params.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:24:43.195034 plugp100-3.1.0/plugp100/requests/set_device_info/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 17:24:30.000000 plugp100-3.1.0/plugp100/requests/set_device_info/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-13 17:24:30.000000 plugp100-3.1.0/plugp100/requests/set_device_info/play_alarm_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-13 17:24:30.000000 plugp100-3.1.0/plugp100/requests/set_device_info/set_light_color_info_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-13 17:24:30.000000 plugp100-3.1.0/plugp100/requests/set_device_info/set_light_info_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-13 17:24:30.000000 plugp100-3.1.0/plugp100/requests/set_device_info/set_plug_info_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-07-13 17:24:30.000000 plugp100-3.1.0/plugp100/requests/tapo_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-13 17:24:30.000000 plugp100-3.1.0/plugp100/requests/trigger_logs_params.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:24:43.195034 plugp100-3.1.0/plugp100/responses/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 17:24:30.000000 plugp100-3.1.0/plugp100/responses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-07-13 17:24:30.000000 plugp100-3.1.0/plugp100/responses/child_device_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4012 2023-07-13 17:24:30.000000 plugp100-3.1.0/plugp100/responses/device_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-13 17:24:30.000000 plugp100-3.1.0/plugp100/responses/energy_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:24:43.195034 plugp100-3.1.0/plugp100/responses/hub_childs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 17:24:30.000000 plugp100-3.1.0/plugp100/responses/hub_childs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-07-13 17:24:30.000000 plugp100-3.1.0/plugp100/responses/hub_childs/s200b_device_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-07-13 17:24:30.000000 plugp100-3.1.0/plugp100/responses/hub_childs/t100_device_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2436 2023-07-13 17:24:30.000000 plugp100-3.1.0/plugp100/responses/hub_childs/t110_device_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3663 2023-07-13 17:24:30.000000 plugp100-3.1.0/plugp100/responses/hub_childs/t31x_device_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-07-13 17:24:30.000000 plugp100-3.1.0/plugp100/responses/hub_childs/trigger_log_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-13 17:24:30.000000 plugp100-3.1.0/plugp100/responses/power_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-07-13 17:24:30.000000 plugp100-3.1.0/plugp100/responses/tapo_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-07-13 17:24:30.000000 plugp100-3.1.0/plugp100/responses/tapo_response.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:24:43.191033 plugp100-3.1.0/plugp100.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-07-13 17:24:43.000000 plugp100-3.1.0/plugp100.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-07-13 17:24:43.000000 plugp100-3.1.0/plugp100.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 17:24:43.000000 plugp100-3.1.0/plugp100.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-13 17:24:43.000000 plugp100-3.1.0/plugp100.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-13 17:24:43.000000 plugp100-3.1.0/plugp100.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-13 17:24:30.000000 plugp100-3.1.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-13 17:24:43.195034 plugp100-3.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-07-13 17:24:30.000000 plugp100-3.1.0/setup.py
```

### Comparing `plugp100-3.0.0/LICENSE` & `plugp100-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `plugp100-3.0.0/PKG-INFO` & `plugp100-3.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plugp100
-Version: 3.0.0
+Version: 3.1.0
 Summary: Controller for TP-Link Tapo P100 and other devices
 Home-page: https://github.com/petretiandrea/plugp100
 Download-URL: https://github.com/petretiandrea/plugp100
 Author: @petretiandrea
 Author-email: petretiandrea@gmail.com
 License: GPL3
 Keywords: Tapo,P100
```

### Comparing `plugp100-3.0.0/README.md` & `plugp100-3.1.0/README.md`

 * *Files identical despite different names*

### Comparing `plugp100-3.0.0/plugp100/__init__.py` & `plugp100-3.1.0/plugp100/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -12,8 +12,8 @@
         sys.path.append(os.path.join(vendor_dir, vendor_path))
 
 from plugp100.responses import *
 from plugp100.requests import *
 from plugp100.api import *
 from plugp100.common import *
 
-__version__ = "3.0.0"
+__version__ = "3.1.0"
```

### Comparing `plugp100-3.0.0/plugp100/api/ledstrip_device.py` & `plugp100-3.1.0/plugp100/api/ledstrip_device.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,36 +6,36 @@
 from plugp100.requests.set_device_info.set_plug_info_params import SetPlugInfoParams
 from plugp100.responses.device_state import LedStripDeviceState
 
 
 class LedStripDevice:
 
     def __init__(self, api: TapoClient, address: str):
-        self.api = api
-        self.address = address
+        self._api = api
+        self._address = address
 
     async def login(self) -> Either[True, Exception]:
-        return await self.api.login(self.address)
+        return await self._api.login(self._address)
 
     async def get_state(self) -> Either[LedStripDeviceState, Exception]:
-        return (await self.api.get_device_info()) | LedStripDeviceState.from_json
+        return (await self._api.get_device_info()) | LedStripDeviceState.try_from_json
 
     async def on(self) -> Either[True, Exception]:
-        return await self.api.set_device_info_with_encode(SetPlugInfoParams(True))
+        return await self._api.set_device_info(SetPlugInfoParams(True))
 
     async def off(self) -> Either[True, Exception]:
-        return await self.api.set_device_info_with_encode(SetPlugInfoParams(False))
+        return await self._api.set_device_info(SetPlugInfoParams(False))
 
     async def set_brightness(self, brightness: int) -> Either[True, Exception]:
-        return await self.api.set_device_info_with_encode(LightDeviceInfoParams(brightness=brightness))
+        return await self._api.set_device_info(LightDeviceInfoParams(brightness=brightness))
 
     async def set_hue_saturation(self, hue: int, saturation: int) -> Either[True, Exception]:
-        return await self.api.set_device_info_with_encode(LightColorDeviceInfoParams(hue=hue, saturation=saturation, color_temp=0))
+        return await self._api.set_device_info(LightColorDeviceInfoParams(hue=hue, saturation=saturation, color_temp=0))
 
     async def set_color_temperature(self, color_temperature: int) -> Either[True, Exception]:
-        return await self.api.set_device_info_with_encode(LightColorDeviceInfoParams(color_temp=color_temperature))
+        return await self._api.set_device_info(LightColorDeviceInfoParams(color_temp=color_temperature))
 
     async def set_light_effect(self, effect: LightEffect) -> Either[True, Exception]:
-        return await self.api.set_lighting_effect(effect)
+        return await self._api.set_lighting_effect(effect)
 
     async def get_state_as_json(self) -> Either[Json, Exception]:
-        return await self.api.get_device_info()
+        return await self._api.get_device_info()
```

### Comparing `plugp100-3.0.0/plugp100/api/light_effect.py` & `plugp100-3.1.0/plugp100/api/light_effect.py`

 * *Files identical despite different names*

### Comparing `plugp100-3.0.0/plugp100/api/light_effect_preset.py` & `plugp100-3.1.0/plugp100/api/light_effect_preset.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,20 +21,17 @@
     Spring = 'Spring'
     Sunrise = 'Sunrise'
     Sunset = 'Sunset'
     Valentines = 'Valentines'
 
     @staticmethod
     def from_name(name: str) -> Optional['LightEffectPreset']:
-        for member in LightEffectPreset:
-            if member.value.lower() == name.lower():
-                return member
-        return None
+        return next([member for member in LightEffectPreset if member.value.lower() == name.lower()], None)
 
-    def to_effect(self) -> 'LightingEffect':
+    def to_effect(self) -> LightEffect:
         _preset_mapping = {
             LightEffectPreset.BubblingCauldron: LightEffect.bubbling_calderon,
             LightEffectPreset.Aurora: LightEffect.aurora,
             LightEffectPreset.CandyCane: LightEffect.candy_cane,
             LightEffectPreset.Christmas: LightEffect.christmas,
             LightEffectPreset.Flicker: LightEffect.flicker,
             LightEffectPreset.ChristmasLight: LightEffect.christmas_light,
```

### Comparing `plugp100-3.0.0/plugp100/common/functional/either.py` & `plugp100-3.1.0/plugp100/common/functional/either.py`

 * *Files 4% similar despite different names*

```diff
@@ -113,14 +113,18 @@
 
 class Left(Either[TSource, TError]):
     """Represents a computation that has failed."""
 
     def __init__(self, error: TError) -> None:
         self._error = error
 
+    @property
+    def error(self):
+        return self._error
+
     @classmethod
     def pure(cls, value: Callable[[TSource], TResult]) -> Either[Callable[[TSource], TResult], TError]:
         return Right(value)
 
     def apply(self, something: Either) -> Either:
         return Left(self._error)
```

### Comparing `plugp100-3.0.0/plugp100/common/utils/http_client.py` & `plugp100-3.1.0/plugp100/common/utils/http_client.py`

 * *Files identical despite different names*

### Comparing `plugp100-3.0.0/plugp100/encryption/key_pair.py` & `plugp100-3.1.0/plugp100/encryption/key_pair.py`

 * *Files identical despite different names*

### Comparing `plugp100-3.0.0/plugp100/encryption/tp_link_cipher.py` & `plugp100-3.1.0/plugp100/encryption/tp_link_cipher.py`

 * *Files identical despite different names*

### Comparing `plugp100-3.0.0/plugp100/example.py` & `plugp100-3.1.0/plugp100/example.py`

 * *Files identical despite different names*

### Comparing `plugp100-3.0.0/plugp100/requests/tapo_request.py` & `plugp100-3.1.0/plugp100/requests/tapo_request.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,13 +1,15 @@
-from typing import TypeVar, Any
+from dataclasses import dataclass
+from typing import TypeVar, Any, List
 
 from plugp100.api.light_effect import LightEffect
 from plugp100.requests.handshake_params import HandshakeParams
 from plugp100.requests.login_device import LoginDeviceParams
 from plugp100.requests.secure_passthrough_params import SecurePassthroughParams
+from plugp100.requests.trigger_logs_params import GetTriggerLogsParams
 
 T = TypeVar("T")
 
 
 class TapoRequest(object):
 
     @staticmethod
@@ -50,24 +52,52 @@
     def get_child_device_list() -> 'TapoRequest':
         return TapoRequest(method='get_child_device_list', params=None)
 
     @staticmethod
     def get_child_device_component_list() -> 'TapoRequest':
         return TapoRequest(method='get_child_device_component_list', params=None)
 
+    @staticmethod
+    def multiple_request(requests: 'MultipleRequestParams') -> 'TapoRequest':
+        return TapoRequest(method='multipleRequest', params=requests)
+
+    @staticmethod
+    def control_child(device_id: str, request: 'TapoRequest') -> 'TapoRequest':
+        return TapoRequest(method='control_child', params=ControlChildParams(device_id, request))
+
+    @staticmethod
+    def get_child_event_logs(trigger_log_params: GetTriggerLogsParams) -> 'TapoRequest':
+        return TapoRequest(method='get_trigger_logs', params=trigger_log_params)
+
+    @staticmethod
+    def get_temperature_humidity_records() -> 'TapoRequest':
+        return TapoRequest(method='get_temp_humidity_records', params=None)
+
     def __init__(self, method: str, params):
         self.method = method
         self.params = params
 
-    def with_request_time_milis(self, t: float) -> 'TapoRequest':
+    def with_request_time_millis(self, t: float) -> 'TapoRequest':
         self.request_time_milis = t
         return self
 
     def with_terminal_uuid(self, uuid: str) -> 'TapoRequest':
         self.terminal_uuid = uuid
         return self
 
     def get_params(self):
         return self.params
 
     def get_method(self):
         return self.method
+
+
+# moved here to avoid circular import in python
+@dataclass
+class ControlChildParams:
+    device_id: str
+    requestData: 'TapoRequest'
+
+
+@dataclass
+class MultipleRequestParams:
+    requests: List[TapoRequest]
```

### Comparing `plugp100-3.0.0/plugp100/responses/device_state.py` & `plugp100-3.1.0/plugp100/responses/device_state.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 @dataclass
 class PlugDeviceState(DeviceState):
     info: 'DeviceInfo'
     device_on: bool
 
     @staticmethod
-    def from_json(kwargs: dict[str, Any]) -> Either['PlugDeviceState', Exception]:
+    def try_from_json(kwargs: dict[str, Any]) -> Either['PlugDeviceState', Exception]:
         try:
             return Right(PlugDeviceState(
                 info=DeviceInfo(**kwargs),
                 device_on=kwargs.get('device_on', False),
             ))
         except Exception as e:
             return Left(e)
@@ -34,15 +34,15 @@
     device_on: bool
     brightness: Optional[int]
     hue: Optional[int]
     saturation: Optional[int]
     color_temp: Optional[int]
 
     @staticmethod
-    def from_json(kwargs: dict[str, Any]) -> Either['LightDeviceState', Exception]:
+    def try_from_json(kwargs: dict[str, Any]) -> Either['LightDeviceState', Exception]:
         try:
             return Right(LightDeviceState(
                 info=DeviceInfo(**kwargs),
                 device_on=kwargs.get('device_on', False),
                 brightness=kwargs.get('brightness', None),
                 hue=kwargs.get('hue', None),
                 saturation=kwargs.get('saturation', None),
@@ -59,15 +59,15 @@
     brightness: Optional[int]
     hue: Optional[int]
     saturation: Optional[int]
     color_temp: Optional[int]
     lighting_effect: Optional[LightEffect]
 
     @staticmethod
-    def from_json(kwargs: dict[str, Any]) -> Either['LedStripDeviceState', Exception]:
+    def try_from_json(kwargs: dict[str, Any]) -> Either['LedStripDeviceState', Exception]:
         try:
             return Right(LedStripDeviceState(
                 info=DeviceInfo(**kwargs),
                 device_on=kwargs.get('device_on', False),
                 brightness=kwargs.get('brightness', None),
                 hue=kwargs.get('hue', None),
                 saturation=kwargs.get('saturation', None),
@@ -109,7 +109,23 @@
         try:
             if len(pieces) > 0:
                 return semantic_version.Version(pieces[0].strip())
             else:
                 return semantic_version.Version('0.0.0')
         except ValueError:
             return semantic_version.Version('0.0.0')
+
+
+@dataclass
+class HubDeviceState(DeviceState):
+    info: 'DeviceInfo'
+    in_alarm: bool
+
+    @staticmethod
+    def try_from_json(kwargs: dict[str, Any]) -> Either['HubDeviceState', Exception]:
+        try:
+            return Right(HubDeviceState(
+                info=DeviceInfo(**kwargs),
+                in_alarm=kwargs.get('in_alarm', False),
+            ))
+        except Exception as e:
+            return Left(e)
```

### Comparing `plugp100-3.0.0/plugp100/responses/energy_info.py` & `plugp100-3.1.0/plugp100/responses/energy_info.py`

 * *Files identical despite different names*

### Comparing `plugp100-3.0.0/plugp100.egg-info/PKG-INFO` & `plugp100-3.1.0/plugp100.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plugp100
-Version: 3.0.0
+Version: 3.1.0
 Summary: Controller for TP-Link Tapo P100 and other devices
 Home-page: https://github.com/petretiandrea/plugp100
 Download-URL: https://github.com/petretiandrea/plugp100
 Author: @petretiandrea
 Author-email: petretiandrea@gmail.com
 License: GPL3
 Keywords: Tapo,P100
```

### Comparing `plugp100-3.0.0/plugp100.egg-info/SOURCES.txt` & `plugp100-3.1.0/plugp100.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -15,33 +15,49 @@
 plugp100/api/__init__.py
 plugp100/api/ledstrip_device.py
 plugp100/api/light_device.py
 plugp100/api/light_effect.py
 plugp100/api/light_effect_preset.py
 plugp100/api/plug_device.py
 plugp100/api/tapo_client.py
+plugp100/api/hub/__init__.py
+plugp100/api/hub/hub_device.py
+plugp100/api/hub/hub_device_tracker.py
+plugp100/api/hub/s200b_device.py
+plugp100/api/hub/t100_device.py
+plugp100/api/hub/t110_device.py
+plugp100/api/hub/t31x_device.py
 plugp100/common/__init__.py
+plugp100/common/state_tracker.py
 plugp100/common/functional/__init__.py
 plugp100/common/functional/either.py
 plugp100/common/utils/__init__.py
 plugp100/common/utils/http_client.py
 plugp100/common/utils/json_utils.py
 plugp100/encryption/__init__.py
 plugp100/encryption/helpers.py
 plugp100/encryption/key_pair.py
 plugp100/encryption/tp_link_cipher.py
 plugp100/requests/__init__.py
 plugp100/requests/handshake_params.py
 plugp100/requests/login_device.py
 plugp100/requests/secure_passthrough_params.py
 plugp100/requests/tapo_request.py
+plugp100/requests/trigger_logs_params.py
 plugp100/requests/set_device_info/__init__.py
+plugp100/requests/set_device_info/play_alarm_params.py
 plugp100/requests/set_device_info/set_light_color_info_params.py
 plugp100/requests/set_device_info/set_light_info_params.py
 plugp100/requests/set_device_info/set_plug_info_params.py
 plugp100/responses/__init__.py
 plugp100/responses/child_device_list.py
 plugp100/responses/device_state.py
 plugp100/responses/energy_info.py
 plugp100/responses/power_info.py
 plugp100/responses/tapo_exception.py
-plugp100/responses/tapo_response.py
+plugp100/responses/tapo_response.py
+plugp100/responses/hub_childs/__init__.py
+plugp100/responses/hub_childs/s200b_device_state.py
+plugp100/responses/hub_childs/t100_device_state.py
+plugp100/responses/hub_childs/t110_device_state.py
+plugp100/responses/hub_childs/t31x_device_state.py
+plugp100/responses/hub_childs/trigger_log_response.py
```

### Comparing `plugp100-3.0.0/setup.py` & `plugp100-3.1.0/setup.py`

 * *Files identical despite different names*

