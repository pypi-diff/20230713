# Comparing `tmp/metal_python-0.9.4.tar.gz` & `tmp/metal_python-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/metal_python-0.9.4.tar", last modified: Tue Oct 20 11:38:33 2020, max compression
+gzip compressed data, was "dist/metal_python-0.9.5.tar", last modified: Wed Oct 21 15:07:41 2020, max compression
```

## Comparing `metal_python-0.9.4.tar` & `metal_python-0.9.5.tar`

### file list

```diff
@@ -1,193 +1,193 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-20 11:38:33.431429 metal_python-0.9.4/
--rw-r--r--   0 runner    (1001) docker     (116)      779 2020-10-20 11:38:33.431429 metal_python-0.9.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      360 2020-10-20 11:38:26.000000 metal_python-0.9.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-20 11:38:33.415428 metal_python-0.9.4/metal_python/
--rw-r--r--   0 runner    (1001) docker     (116)     6610 2020-10-20 11:38:26.000000 metal_python-0.9.4/metal_python/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-20 11:38:33.419428 metal_python-0.9.4/metal_python/api/
--rw-r--r--   0 runner    (1001) docker     (116)      641 2020-10-20 11:38:26.000000 metal_python-0.9.4/metal_python/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    15068 2020-10-20 11:38:26.000000 metal_python-0.9.4/metal_python/api/firewall_api.py
--rw-r--r--   0 runner    (1001) docker     (116)     3933 2020-10-20 11:38:26.000000 metal_python-0.9.4/metal_python/api/health_api.py
--rw-r--r--   0 runner    (1001) docker     (116)    22417 2020-10-20 11:38:26.000000 metal_python-0.9.4/metal_python/api/image_api.py
--rw-r--r--   0 runner    (1001) docker     (116)    26227 2020-10-20 11:38:26.000000 metal_python-0.9.4/metal_python/api/ip_api.py
--rw-r--r--   0 runner    (1001) docker     (116)    88615 2020-10-20 11:38:26.000000 metal_python-0.9.4/metal_python/api/machine_api.py
--rw-r--r--   0 runner    (1001) docker     (116)    29994 2020-10-20 11:38:26.000000 metal_python-0.9.4/metal_python/api/network_api.py
--rw-r--r--   0 runner    (1001) docker     (116)    22297 2020-10-20 11:38:26.000000 metal_python-0.9.4/metal_python/api/partition_api.py
--rw-r--r--   0 runner    (1001) docker     (116)    22511 2020-10-20 11:38:26.000000 metal_python-0.9.4/metal_python/api/project_api.py
--rw-r--r--   0 runner    (1001) docker     (116)    22591 2020-10-20 11:38:26.000000 metal_python-0.9.4/metal_python/api/size_api.py
--rw-r--r--   0 runner    (1001) docker     (116)    22943 2020-10-20 11:38:26.000000 metal_python-0.9.4/metal_python/api/switch_api.py
--rw-r--r--   0 runner    (1001) docker     (116)     3990 2020-10-20 11:38:26.000000 metal_python-0.9.4/metal_python/api/version_api.py
--rw-r--r--   0 runner    (1001) docker     (116)    25055 2020-10-20 11:38:26.000000 metal_python-0.9.4/metal_python/api_client.py
--rw-r--r--   0 runner    (1001) docker     (116)     8398 2020-10-20 11:38:26.000000 metal_python-0.9.4/metal_python/configuration.py
--rw-r--r--   0 runner    (1001) docker     (116)     2524 2020-10-20 11:38:26.000000 metal_python-0.9.4/metal_python/driver.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-20 11:38:33.423429 metal_python-0.9.4/metal_python/models/
--rw-r--r--   0 runner    (1001) docker     (116)     5907 2020-10-20 11:38:26.000000 metal_python-0.9.4/metal_python/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     4319 2020-10-20 11:38:26.000000 metal_python-0.9.4/metal_python/models/httperrors_http_error_response.py
--rw-r--r--   0 runner    (1001) docker     (116)     3881 2020-10-20 11:38:26.000000 metal_python-0.9.4/metal_python/models/rest_status.py
--rw-r--r--   0 runner    (1001) docker     (116)     6071 2020-10-20 11:38:26.000000 metal_python-0.9.4/metal_python/models/rest_version.py
--rw-r--r--   0 runner    (1001) docker     (116)     4110 2020-10-20 11:38:26.000000 metal_python-0.9.4/metal_python/models/v1_bgp_filter.py
--rw-r--r--   0 runner    (1001) docker     (116)     8349 2020-10-20 11:38:26.000000 metal_python-0.9.4/metal_python/models/v1_boot_info.py
--rw-r--r--   0 runner    (1001) docker     (116)     4464 2020-10-20 11:38:26.000000 metal_python-0.9.4/metal_python/models/v1_chassis_identify_led_state.py
--rw-r--r--   0 runner    (1001) docker     (116)     2476 2020-10-20 11:38:26.000000 metal_python-0.9.4/metal_python/models/v1_empty_body.py
--rw-r--r--   0 runner    (1001) docker     (116)    14728 2020-10-20 11:38:26.000000 metal_python-0.9.4/metal_python/models/v1_firewall_create_request.py
--rw-r--r--   0 runner    (1001) docker     (116)    39210 2020-10-20 11:38:26.000000 metal_python-0.9.4/metal_python/models/v1_firewall_find_request.py
--rw-r--r--   0 runner    (1001) docker     (116)    15837 2020-10-20 11:38:26.000000 metal_python-0.9.4/metal_python/models/v1_firewall_response.py
--rw-r--r--   0 runner    (1001) docker     (116)     8246 2020-10-20 11:38:26.000000 metal_python-0.9.4/metal_python/models/v1_image_create_request.py
--rw-r--r--   0 runner    (1001) docker     (116)    10427 2020-10-20 11:38:26.000000 metal_python-0.9.4/metal_python/models/v1_image_response.py
--rw-r--r--   0 runner    (1001) docker     (116)     9041 2020-10-20 11:38:26.000000 metal_python-0.9.4/metal_python/models/v1_image_update_request.py
--rw-r--r--   0 runner    (1001) docker     (116)     8805 2020-10-20 11:38:26.000000 metal_python-0.9.4/metal_python/models/v1_ip_allocate_request.py
--rw-r--r--   0 runner    (1001) docker     (116)     8225 2020-10-20 11:38:26.000000 metal_python-0.9.4/metal_python/models/v1_ip_find_request.py
--rw-r--r--   0 runner    (1001) docker     (116)    10189 2020-10-20 11:38:26.000000 metal_python-0.9.4/metal_python/models/v1_ip_response.py
--rw-r--r--   0 runner    (1001) docker     (116)     6955 2020-10-20 11:38:26.000000 metal_python-0.9.4/metal_python/models/v1_ip_update_request.py
--rw-r--r--   0 runner    (1001) docker     (116)     3729 2020-10-20 11:38:26.000000 metal_python-0.9.4/metal_python/models/v1_machine_abort_reinstall_request.py
--rw-r--r--   0 runner    (1001) docker     (116)    14022 2020-10-20 11:38:26.000000 metal_python-0.9.4/metal_python/models/v1_machine_allocate_request.py
--rw-r--r--   0 runner    (1001) docker     (116)    14192 2020-10-20 11:38:26.000000 metal_python-0.9.4/metal_python/models/v1_machine_allocation.py
--rw-r--r--   0 runner    (1001) docker     (116)     4589 2020-10-20 11:38:26.000000 metal_python-0.9.4/metal_python/models/v1_machine_allocation_network.py
--rw-r--r--   0 runner    (1001) docker     (116)     4827 2020-10-20 11:38:26.000000 metal_python-0.9.4/metal_python/models/v1_machine_bios.py
--rw-r--r--   0 runner    (1001) docker     (116)     5888 2020-10-20 11:38:26.000000 metal_python-0.9.4/metal_python/models/v1_machine_block_device.py
--rw-r--r--   0 runner    (1001) docker     (116)    11282 2020-10-20 11:38:26.000000 metal_python-0.9.4/metal_python/models/v1_machine_disk_partition.py
--rw-r--r--   0 runner    (1001) docker     (116)     9361 2020-10-20 11:38:26.000000 metal_python-0.9.4/metal_python/models/v1_machine_finalize_allocation_request.py
--rw-r--r--   0 runner    (1001) docker     (116)    39030 2020-10-20 11:38:26.000000 metal_python-0.9.4/metal_python/models/v1_machine_find_request.py
--rw-r--r--   0 runner    (1001) docker     (116)     9814 2020-10-20 11:38:26.000000 metal_python-0.9.4/metal_python/models/v1_machine_fru.py
--rw-r--r--   0 runner    (1001) docker     (116)     5968 2020-10-20 11:38:26.000000 metal_python-0.9.4/metal_python/models/v1_machine_hardware.py
--rw-r--r--   0 runner    (1001) docker     (116)     6204 2020-10-20 11:38:26.000000 metal_python-0.9.4/metal_python/models/v1_machine_hardware_extended.py
--rw-r--r--   0 runner    (1001) docker     (116)     7495 2020-10-20 11:38:26.000000 metal_python-0.9.4/metal_python/models/v1_machine_ipmi.py
--rw-r--r--   0 runner    (1001) docker     (116)     5242 2020-10-20 11:38:26.000000 metal_python-0.9.4/metal_python/models/v1_machine_ipmi_report.py
--rw-r--r--   0 runner    (1001) docker     (116)     4472 2020-10-20 11:38:26.000000 metal_python-0.9.4/metal_python/models/v1_machine_ipmi_report_response.py
--rw-r--r--   0 runner    (1001) docker     (116)    16877 2020-10-20 11:38:26.000000 metal_python-0.9.4/metal_python/models/v1_machine_ipmi_response.py
--rw-r--r--   0 runner    (1001) docker     (116)    10566 2020-10-20 11:38:26.000000 metal_python-0.9.4/metal_python/models/v1_machine_network.py
--rw-r--r--   0 runner    (1001) docker     (116)     4021 2020-10-20 11:38:26.000000 metal_python-0.9.4/metal_python/models/v1_machine_nic.py
--rw-r--r--   0 runner    (1001) docker     (116)     5123 2020-10-20 11:38:26.000000 metal_python-0.9.4/metal_python/models/v1_machine_nic_extended.py
--rw-r--r--   0 runner    (1001) docker     (116)     4972 2020-10-20 11:38:26.000000 metal_python-0.9.4/metal_python/models/v1_machine_provisioning_event.py
--rw-r--r--   0 runner    (1001) docker     (116)     6100 2020-10-20 11:38:26.000000 metal_python-0.9.4/metal_python/models/v1_machine_recent_provisioning_events.py
--rw-r--r--   0 runner    (1001) docker     (116)     8697 2020-10-20 11:38:26.000000 metal_python-0.9.4/metal_python/models/v1_machine_register_request.py
--rw-r--r--   0 runner    (1001) docker     (116)     5791 2020-10-20 11:38:26.000000 metal_python-0.9.4/metal_python/models/v1_machine_reinstall_request.py
--rw-r--r--   0 runner    (1001) docker     (116)    15769 2020-10-20 11:38:26.000000 metal_python-0.9.4/metal_python/models/v1_machine_response.py
--rw-r--r--   0 runner    (1001) docker     (116)     4300 2020-10-20 11:38:26.000000 metal_python-0.9.4/metal_python/models/v1_machine_state.py
--rw-r--r--   0 runner    (1001) docker     (116)     7601 2020-10-20 11:38:26.000000 metal_python-0.9.4/metal_python/models/v1_meta.py
--rw-r--r--   0 runner    (1001) docker     (116)     6776 2020-10-20 11:38:26.000000 metal_python-0.9.4/metal_python/models/v1_network_allocate_request.py
--rw-r--r--   0 runner    (1001) docker     (116)    15475 2020-10-20 11:38:26.000000 metal_python-0.9.4/metal_python/models/v1_network_create_request.py
--rw-r--r--   0 runner    (1001) docker     (116)    10938 2020-10-20 11:38:26.000000 metal_python-0.9.4/metal_python/models/v1_network_find_request.py
--rw-r--r--   0 runner    (1001) docker     (116)    17559 2020-10-20 11:38:26.000000 metal_python-0.9.4/metal_python/models/v1_network_response.py
--rw-r--r--   0 runner    (1001) docker     (116)     6517 2020-10-20 11:38:26.000000 metal_python-0.9.4/metal_python/models/v1_network_update_request.py
--rw-r--r--   0 runner    (1001) docker     (116)     6284 2020-10-20 11:38:26.000000 metal_python-0.9.4/metal_python/models/v1_network_usage.py
--rw-r--r--   0 runner    (1001) docker     (116)     5209 2020-10-20 11:38:26.000000 metal_python-0.9.4/metal_python/models/v1_partition_boot_configuration.py
--rw-r--r--   0 runner    (1001) docker     (116)     5742 2020-10-20 11:38:26.000000 metal_python-0.9.4/metal_python/models/v1_partition_capacity.py
--rw-r--r--   0 runner    (1001) docker     (116)     8770 2020-10-20 11:38:26.000000 metal_python-0.9.4/metal_python/models/v1_partition_create_request.py
--rw-r--r--   0 runner    (1001) docker     (116)    10228 2020-10-20 11:38:26.000000 metal_python-0.9.4/metal_python/models/v1_partition_response.py
--rw-r--r--   0 runner    (1001) docker     (116)     6905 2020-10-20 11:38:26.000000 metal_python-0.9.4/metal_python/models/v1_partition_update_request.py
--rw-r--r--   0 runner    (1001) docker     (116)     5915 2020-10-20 11:38:26.000000 metal_python-0.9.4/metal_python/models/v1_project_create_request.py
--rw-r--r--   0 runner    (1001) docker     (116)     5148 2020-10-20 11:38:26.000000 metal_python-0.9.4/metal_python/models/v1_project_find_request.py
--rw-r--r--   0 runner    (1001) docker     (116)     5795 2020-10-20 11:38:26.000000 metal_python-0.9.4/metal_python/models/v1_project_response.py
--rw-r--r--   0 runner    (1001) docker     (116)     5915 2020-10-20 11:38:26.000000 metal_python-0.9.4/metal_python/models/v1_project_update_request.py
--rw-r--r--   0 runner    (1001) docker     (116)     3594 2020-10-20 11:38:26.000000 metal_python-0.9.4/metal_python/models/v1_quota.py
--rw-r--r--   0 runner    (1001) docker     (116)     4936 2020-10-20 11:38:26.000000 metal_python-0.9.4/metal_python/models/v1_quota_set.py
--rw-r--r--   0 runner    (1001) docker     (116)     9494 2020-10-20 11:38:26.000000 metal_python-0.9.4/metal_python/models/v1_server_capacity.py
--rw-r--r--   0 runner    (1001) docker     (116)     5094 2020-10-20 11:38:26.000000 metal_python-0.9.4/metal_python/models/v1_size_constraint.py
--rw-r--r--   0 runner    (1001) docker     (116)     5290 2020-10-20 11:38:26.000000 metal_python-0.9.4/metal_python/models/v1_size_constraint_matching_log.py
--rw-r--r--   0 runner    (1001) docker     (116)     5844 2020-10-20 11:38:26.000000 metal_python-0.9.4/metal_python/models/v1_size_create_request.py
--rw-r--r--   0 runner    (1001) docker     (116)     5460 2020-10-20 11:38:26.000000 metal_python-0.9.4/metal_python/models/v1_size_matching_log.py
--rw-r--r--   0 runner    (1001) docker     (116)     7302 2020-10-20 11:38:26.000000 metal_python-0.9.4/metal_python/models/v1_size_response.py
--rw-r--r--   0 runner    (1001) docker     (116)     5754 2020-10-20 11:38:26.000000 metal_python-0.9.4/metal_python/models/v1_size_update_request.py
--rw-r--r--   0 runner    (1001) docker     (116)     4170 2020-10-20 11:38:26.000000 metal_python-0.9.4/metal_python/models/v1_switch_connection.py
--rw-r--r--   0 runner    (1001) docker     (116)     5477 2020-10-20 11:38:26.000000 metal_python-0.9.4/metal_python/models/v1_switch_nic.py
--rw-r--r--   0 runner    (1001) docker     (116)     4248 2020-10-20 11:38:26.000000 metal_python-0.9.4/metal_python/models/v1_switch_notify_request.py
--rw-r--r--   0 runner    (1001) docker     (116)     8416 2020-10-20 11:38:26.000000 metal_python-0.9.4/metal_python/models/v1_switch_register_request.py
--rw-r--r--   0 runner    (1001) docker     (116)    12627 2020-10-20 11:38:26.000000 metal_python-0.9.4/metal_python/models/v1_switch_response.py
--rw-r--r--   0 runner    (1001) docker     (116)     4886 2020-10-20 11:38:26.000000 metal_python-0.9.4/metal_python/models/v1_switch_sync.py
--rw-r--r--   0 runner    (1001) docker     (116)     6480 2020-10-20 11:38:26.000000 metal_python-0.9.4/metal_python/models/v1_switch_update_request.py
--rw-r--r--   0 runner    (1001) docker     (116)    13235 2020-10-20 11:38:26.000000 metal_python-0.9.4/metal_python/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-20 11:38:33.415428 metal_python-0.9.4/metal_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)      779 2020-10-20 11:38:33.000000 metal_python-0.9.4/metal_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     7008 2020-10-20 11:38:33.000000 metal_python-0.9.4/metal_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2020-10-20 11:38:33.000000 metal_python-0.9.4/metal_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       91 2020-10-20 11:38:33.000000 metal_python-0.9.4/metal_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       18 2020-10-20 11:38:33.000000 metal_python-0.9.4/metal_python.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)       38 2020-10-20 11:38:33.431429 metal_python-0.9.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     1172 2020-10-20 11:38:26.000000 metal_python-0.9.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-20 11:38:33.431429 metal_python-0.9.4/test/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2020-10-20 11:38:26.000000 metal_python-0.9.4/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1362 2020-10-20 11:38:26.000000 metal_python-0.9.4/test/test_firewall_api.py
--rw-r--r--   0 runner    (1001) docker     (116)      881 2020-10-20 11:38:26.000000 metal_python-0.9.4/test/test_health_api.py
--rw-r--r--   0 runner    (1001) docker     (116)     1069 2020-10-20 11:38:26.000000 metal_python-0.9.4/test/test_httperrors_http_error_response.py
--rw-r--r--   0 runner    (1001) docker     (116)     1734 2020-10-20 11:38:26.000000 metal_python-0.9.4/test/test_image_api.py
--rw-r--r--   0 runner    (1001) docker     (116)     1787 2020-10-20 11:38:26.000000 metal_python-0.9.4/test/test_ip_api.py
--rw-r--r--   0 runner    (1001) docker     (116)     4470 2020-10-20 11:38:26.000000 metal_python-0.9.4/test/test_machine_api.py
--rw-r--r--   0 runner    (1001) docker     (116)     2118 2020-10-20 11:38:26.000000 metal_python-0.9.4/test/test_network_api.py
--rw-r--r--   0 runner    (1001) docker     (116)     1820 2020-10-20 11:38:26.000000 metal_python-0.9.4/test/test_partition_api.py
--rw-r--r--   0 runner    (1001) docker     (116)     1745 2020-10-20 11:38:26.000000 metal_python-0.9.4/test/test_project_api.py
--rw-r--r--   0 runner    (1001) docker     (116)      929 2020-10-20 11:38:26.000000 metal_python-0.9.4/test/test_rest_status.py
--rw-r--r--   0 runner    (1001) docker     (116)      937 2020-10-20 11:38:26.000000 metal_python-0.9.4/test/test_rest_version.py
--rw-r--r--   0 runner    (1001) docker     (116)     1840 2020-10-20 11:38:26.000000 metal_python-0.9.4/test/test_size_api.py
--rw-r--r--   0 runner    (1001) docker     (116)     1738 2020-10-20 11:38:26.000000 metal_python-0.9.4/test/test_switch_api.py
--rw-r--r--   0 runner    (1001) docker     (116)      939 2020-10-20 11:38:26.000000 metal_python-0.9.4/test/test_v1_bgp_filter.py
--rw-r--r--   0 runner    (1001) docker     (116)      931 2020-10-20 11:38:26.000000 metal_python-0.9.4/test/test_v1_boot_info.py
--rw-r--r--   0 runner    (1001) docker     (116)     1055 2020-10-20 11:38:26.000000 metal_python-0.9.4/test/test_v1_chassis_identify_led_state.py
--rw-r--r--   0 runner    (1001) docker     (116)      939 2020-10-20 11:38:26.000000 metal_python-0.9.4/test/test_v1_empty_body.py
--rw-r--r--   0 runner    (1001) docker     (116)     1037 2020-10-20 11:38:26.000000 metal_python-0.9.4/test/test_v1_firewall_create_request.py
--rw-r--r--   0 runner    (1001) docker     (116)     1021 2020-10-20 11:38:26.000000 metal_python-0.9.4/test/test_v1_firewall_find_request.py
--rw-r--r--   0 runner    (1001) docker     (116)      995 2020-10-20 11:38:26.000000 metal_python-0.9.4/test/test_v1_firewall_response.py
--rw-r--r--   0 runner    (1001) docker     (116)     1013 2020-10-20 11:38:26.000000 metal_python-0.9.4/test/test_v1_image_create_request.py
--rw-r--r--   0 runner    (1001) docker     (116)      971 2020-10-20 11:38:26.000000 metal_python-0.9.4/test/test_v1_image_response.py
--rw-r--r--   0 runner    (1001) docker     (116)     1013 2020-10-20 11:38:26.000000 metal_python-0.9.4/test/test_v1_image_update_request.py
--rw-r--r--   0 runner    (1001) docker     (116)     1005 2020-10-20 11:38:26.000000 metal_python-0.9.4/test/test_v1_ip_allocate_request.py
--rw-r--r--   0 runner    (1001) docker     (116)      973 2020-10-20 11:38:26.000000 metal_python-0.9.4/test/test_v1_ip_find_request.py
--rw-r--r--   0 runner    (1001) docker     (116)      947 2020-10-20 11:38:26.000000 metal_python-0.9.4/test/test_v1_ip_response.py
--rw-r--r--   0 runner    (1001) docker     (116)      989 2020-10-20 11:38:26.000000 metal_python-0.9.4/test/test_v1_ip_update_request.py
--rw-r--r--   0 runner    (1001) docker     (116)     1095 2020-10-20 11:38:26.000000 metal_python-0.9.4/test/test_v1_machine_abort_reinstall_request.py
--rw-r--r--   0 runner    (1001) docker     (116)     1045 2020-10-20 11:38:26.000000 metal_python-0.9.4/test/test_v1_machine_allocate_request.py
--rw-r--r--   0 runner    (1001) docker     (116)     1003 2020-10-20 11:38:26.000000 metal_python-0.9.4/test/test_v1_machine_allocation.py
--rw-r--r--   0 runner    (1001) docker     (116)     1061 2020-10-20 11:38:26.000000 metal_python-0.9.4/test/test_v1_machine_allocation_network.py
--rw-r--r--   0 runner    (1001) docker     (116)      955 2020-10-20 11:38:26.000000 metal_python-0.9.4/test/test_v1_machine_bios.py
--rw-r--r--   0 runner    (1001) docker     (116)     1013 2020-10-20 11:38:26.000000 metal_python-0.9.4/test/test_v1_machine_block_device.py
--rw-r--r--   0 runner    (1001) docker     (116)     1029 2020-10-20 11:38:26.000000 metal_python-0.9.4/test/test_v1_machine_disk_partition.py
--rw-r--r--   0 runner    (1001) docker     (116)     1127 2020-10-20 11:38:26.000000 metal_python-0.9.4/test/test_v1_machine_finalize_allocation_request.py
--rw-r--r--   0 runner    (1001) docker     (116)     1013 2020-10-20 11:38:26.000000 metal_python-0.9.4/test/test_v1_machine_find_request.py
--rw-r--r--   0 runner    (1001) docker     (116)      947 2020-10-20 11:38:26.000000 metal_python-0.9.4/test/test_v1_machine_fru.py
--rw-r--r--   0 runner    (1001) docker     (116)      987 2020-10-20 11:38:26.000000 metal_python-0.9.4/test/test_v1_machine_hardware.py
--rw-r--r--   0 runner    (1001) docker     (116)     1053 2020-10-20 11:38:26.000000 metal_python-0.9.4/test/test_v1_machine_hardware_extended.py
--rw-r--r--   0 runner    (1001) docker     (116)      955 2020-10-20 11:38:26.000000 metal_python-0.9.4/test/test_v1_machine_ipmi.py
--rw-r--r--   0 runner    (1001) docker     (116)     1005 2020-10-20 11:38:26.000000 metal_python-0.9.4/test/test_v1_machine_ipmi_report.py
--rw-r--r--   0 runner    (1001) docker     (116)     1071 2020-10-20 11:38:26.000000 metal_python-0.9.4/test/test_v1_machine_ipmi_report_response.py
--rw-r--r--   0 runner    (1001) docker     (116)     1021 2020-10-20 11:38:26.000000 metal_python-0.9.4/test/test_v1_machine_ipmi_response.py
--rw-r--r--   0 runner    (1001) docker     (116)      979 2020-10-20 11:38:26.000000 metal_python-0.9.4/test/test_v1_machine_network.py
--rw-r--r--   0 runner    (1001) docker     (116)      947 2020-10-20 11:38:26.000000 metal_python-0.9.4/test/test_v1_machine_nic.py
--rw-r--r--   0 runner    (1001) docker     (116)     1013 2020-10-20 11:38:26.000000 metal_python-0.9.4/test/test_v1_machine_nic_extended.py
--rw-r--r--   0 runner    (1001) docker     (116)     1061 2020-10-20 11:38:26.000000 metal_python-0.9.4/test/test_v1_machine_provisioning_event.py
--rw-r--r--   0 runner    (1001) docker     (116)     1119 2020-10-20 11:38:26.000000 metal_python-0.9.4/test/test_v1_machine_recent_provisioning_events.py
--rw-r--r--   0 runner    (1001) docker     (116)     1045 2020-10-20 11:38:26.000000 metal_python-0.9.4/test/test_v1_machine_register_request.py
--rw-r--r--   0 runner    (1001) docker     (116)     1053 2020-10-20 11:38:26.000000 metal_python-0.9.4/test/test_v1_machine_reinstall_request.py
--rw-r--r--   0 runner    (1001) docker     (116)      987 2020-10-20 11:38:26.000000 metal_python-0.9.4/test/test_v1_machine_response.py
--rw-r--r--   0 runner    (1001) docker     (116)      963 2020-10-20 11:38:26.000000 metal_python-0.9.4/test/test_v1_machine_state.py
--rw-r--r--   0 runner    (1001) docker     (116)      897 2020-10-20 11:38:26.000000 metal_python-0.9.4/test/test_v1_meta.py
--rw-r--r--   0 runner    (1001) docker     (116)     1045 2020-10-20 11:38:26.000000 metal_python-0.9.4/test/test_v1_network_allocate_request.py
--rw-r--r--   0 runner    (1001) docker     (116)     1029 2020-10-20 11:38:26.000000 metal_python-0.9.4/test/test_v1_network_create_request.py
--rw-r--r--   0 runner    (1001) docker     (116)     1013 2020-10-20 11:38:26.000000 metal_python-0.9.4/test/test_v1_network_find_request.py
--rw-r--r--   0 runner    (1001) docker     (116)      987 2020-10-20 11:38:26.000000 metal_python-0.9.4/test/test_v1_network_response.py
--rw-r--r--   0 runner    (1001) docker     (116)     1029 2020-10-20 11:38:26.000000 metal_python-0.9.4/test/test_v1_network_update_request.py
--rw-r--r--   0 runner    (1001) docker     (116)      963 2020-10-20 11:38:26.000000 metal_python-0.9.4/test/test_v1_network_usage.py
--rw-r--r--   0 runner    (1001) docker     (116)     1077 2020-10-20 11:38:26.000000 metal_python-0.9.4/test/test_v1_partition_boot_configuration.py
--rw-r--r--   0 runner    (1001) docker     (116)     1003 2020-10-20 11:38:26.000000 metal_python-0.9.4/test/test_v1_partition_capacity.py
--rw-r--r--   0 runner    (1001) docker     (116)     1045 2020-10-20 11:38:26.000000 metal_python-0.9.4/test/test_v1_partition_create_request.py
--rw-r--r--   0 runner    (1001) docker     (116)     1003 2020-10-20 11:38:26.000000 metal_python-0.9.4/test/test_v1_partition_response.py
--rw-r--r--   0 runner    (1001) docker     (116)     1045 2020-10-20 11:38:26.000000 metal_python-0.9.4/test/test_v1_partition_update_request.py
--rw-r--r--   0 runner    (1001) docker     (116)     1029 2020-10-20 11:38:26.000000 metal_python-0.9.4/test/test_v1_project_create_request.py
--rw-r--r--   0 runner    (1001) docker     (116)     1013 2020-10-20 11:38:26.000000 metal_python-0.9.4/test/test_v1_project_find_request.py
--rw-r--r--   0 runner    (1001) docker     (116)      987 2020-10-20 11:38:26.000000 metal_python-0.9.4/test/test_v1_project_response.py
--rw-r--r--   0 runner    (1001) docker     (116)     1029 2020-10-20 11:38:26.000000 metal_python-0.9.4/test/test_v1_project_update_request.py
--rw-r--r--   0 runner    (1001) docker     (116)      905 2020-10-20 11:38:26.000000 metal_python-0.9.4/test/test_v1_quota.py
--rw-r--r--   0 runner    (1001) docker     (116)      931 2020-10-20 11:38:26.000000 metal_python-0.9.4/test/test_v1_quota_set.py
--rw-r--r--   0 runner    (1001) docker     (116)      979 2020-10-20 11:38:26.000000 metal_python-0.9.4/test/test_v1_server_capacity.py
--rw-r--r--   0 runner    (1001) docker     (116)      979 2020-10-20 11:38:26.000000 metal_python-0.9.4/test/test_v1_size_constraint.py
--rw-r--r--   0 runner    (1001) docker     (116)     1071 2020-10-20 11:38:26.000000 metal_python-0.9.4/test/test_v1_size_constraint_matching_log.py
--rw-r--r--   0 runner    (1001) docker     (116)     1005 2020-10-20 11:38:26.000000 metal_python-0.9.4/test/test_v1_size_create_request.py
--rw-r--r--   0 runner    (1001) docker     (116)      989 2020-10-20 11:38:26.000000 metal_python-0.9.4/test/test_v1_size_matching_log.py
--rw-r--r--   0 runner    (1001) docker     (116)      963 2020-10-20 11:38:26.000000 metal_python-0.9.4/test/test_v1_size_response.py
--rw-r--r--   0 runner    (1001) docker     (116)     1005 2020-10-20 11:38:26.000000 metal_python-0.9.4/test/test_v1_size_update_request.py
--rw-r--r--   0 runner    (1001) docker     (116)      995 2020-10-20 11:38:26.000000 metal_python-0.9.4/test/test_v1_switch_connection.py
--rw-r--r--   0 runner    (1001) docker     (116)      939 2020-10-20 11:38:26.000000 metal_python-0.9.4/test/test_v1_switch_nic.py
--rw-r--r--   0 runner    (1001) docker     (116)     1021 2020-10-20 11:38:26.000000 metal_python-0.9.4/test/test_v1_switch_notify_request.py
--rw-r--r--   0 runner    (1001) docker     (116)     1037 2020-10-20 11:38:26.000000 metal_python-0.9.4/test/test_v1_switch_register_request.py
--rw-r--r--   0 runner    (1001) docker     (116)      979 2020-10-20 11:38:26.000000 metal_python-0.9.4/test/test_v1_switch_response.py
--rw-r--r--   0 runner    (1001) docker     (116)      947 2020-10-20 11:38:26.000000 metal_python-0.9.4/test/test_v1_switch_sync.py
--rw-r--r--   0 runner    (1001) docker     (116)     1021 2020-10-20 11:38:26.000000 metal_python-0.9.4/test/test_v1_switch_update_request.py
--rw-r--r--   0 runner    (1001) docker     (116)      916 2020-10-20 11:38:26.000000 metal_python-0.9.4/test/test_version_api.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-21 15:07:41.837566 metal_python-0.9.5/
+-rw-r--r--   0 runner    (1001) docker     (116)      779 2020-10-21 15:07:41.837566 metal_python-0.9.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)      360 2020-10-21 15:07:25.000000 metal_python-0.9.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-21 15:07:41.813566 metal_python-0.9.5/metal_python/
+-rw-r--r--   0 runner    (1001) docker     (116)     6610 2020-10-21 15:07:25.000000 metal_python-0.9.5/metal_python/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-21 15:07:41.817566 metal_python-0.9.5/metal_python/api/
+-rw-r--r--   0 runner    (1001) docker     (116)      641 2020-10-21 15:07:25.000000 metal_python-0.9.5/metal_python/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)    15068 2020-10-21 15:07:25.000000 metal_python-0.9.5/metal_python/api/firewall_api.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3933 2020-10-21 15:07:25.000000 metal_python-0.9.5/metal_python/api/health_api.py
+-rw-r--r--   0 runner    (1001) docker     (116)    22417 2020-10-21 15:07:25.000000 metal_python-0.9.5/metal_python/api/image_api.py
+-rw-r--r--   0 runner    (1001) docker     (116)    26227 2020-10-21 15:07:25.000000 metal_python-0.9.5/metal_python/api/ip_api.py
+-rw-r--r--   0 runner    (1001) docker     (116)    88615 2020-10-21 15:07:25.000000 metal_python-0.9.5/metal_python/api/machine_api.py
+-rw-r--r--   0 runner    (1001) docker     (116)    29994 2020-10-21 15:07:25.000000 metal_python-0.9.5/metal_python/api/network_api.py
+-rw-r--r--   0 runner    (1001) docker     (116)    22297 2020-10-21 15:07:25.000000 metal_python-0.9.5/metal_python/api/partition_api.py
+-rw-r--r--   0 runner    (1001) docker     (116)    22511 2020-10-21 15:07:25.000000 metal_python-0.9.5/metal_python/api/project_api.py
+-rw-r--r--   0 runner    (1001) docker     (116)    22591 2020-10-21 15:07:25.000000 metal_python-0.9.5/metal_python/api/size_api.py
+-rw-r--r--   0 runner    (1001) docker     (116)    22943 2020-10-21 15:07:25.000000 metal_python-0.9.5/metal_python/api/switch_api.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3990 2020-10-21 15:07:25.000000 metal_python-0.9.5/metal_python/api/version_api.py
+-rw-r--r--   0 runner    (1001) docker     (116)    25055 2020-10-21 15:07:25.000000 metal_python-0.9.5/metal_python/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (116)     8398 2020-10-21 15:07:25.000000 metal_python-0.9.5/metal_python/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2524 2020-10-21 15:07:25.000000 metal_python-0.9.5/metal_python/driver.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-21 15:07:41.829566 metal_python-0.9.5/metal_python/models/
+-rw-r--r--   0 runner    (1001) docker     (116)     5907 2020-10-21 15:07:25.000000 metal_python-0.9.5/metal_python/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4319 2020-10-21 15:07:25.000000 metal_python-0.9.5/metal_python/models/httperrors_http_error_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3881 2020-10-21 15:07:25.000000 metal_python-0.9.5/metal_python/models/rest_status.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6071 2020-10-21 15:07:25.000000 metal_python-0.9.5/metal_python/models/rest_version.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4110 2020-10-21 15:07:25.000000 metal_python-0.9.5/metal_python/models/v1_bgp_filter.py
+-rw-r--r--   0 runner    (1001) docker     (116)     8349 2020-10-21 15:07:25.000000 metal_python-0.9.5/metal_python/models/v1_boot_info.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4464 2020-10-21 15:07:25.000000 metal_python-0.9.5/metal_python/models/v1_chassis_identify_led_state.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2476 2020-10-21 15:07:25.000000 metal_python-0.9.5/metal_python/models/v1_empty_body.py
+-rw-r--r--   0 runner    (1001) docker     (116)    14728 2020-10-21 15:07:25.000000 metal_python-0.9.5/metal_python/models/v1_firewall_create_request.py
+-rw-r--r--   0 runner    (1001) docker     (116)    38477 2020-10-21 15:07:25.000000 metal_python-0.9.5/metal_python/models/v1_firewall_find_request.py
+-rw-r--r--   0 runner    (1001) docker     (116)    15837 2020-10-21 15:07:25.000000 metal_python-0.9.5/metal_python/models/v1_firewall_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)     8246 2020-10-21 15:07:25.000000 metal_python-0.9.5/metal_python/models/v1_image_create_request.py
+-rw-r--r--   0 runner    (1001) docker     (116)    10427 2020-10-21 15:07:25.000000 metal_python-0.9.5/metal_python/models/v1_image_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)     9041 2020-10-21 15:07:25.000000 metal_python-0.9.5/metal_python/models/v1_image_update_request.py
+-rw-r--r--   0 runner    (1001) docker     (116)     8805 2020-10-21 15:07:25.000000 metal_python-0.9.5/metal_python/models/v1_ip_allocate_request.py
+-rw-r--r--   0 runner    (1001) docker     (116)     8225 2020-10-21 15:07:25.000000 metal_python-0.9.5/metal_python/models/v1_ip_find_request.py
+-rw-r--r--   0 runner    (1001) docker     (116)    10189 2020-10-21 15:07:25.000000 metal_python-0.9.5/metal_python/models/v1_ip_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6955 2020-10-21 15:07:25.000000 metal_python-0.9.5/metal_python/models/v1_ip_update_request.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3729 2020-10-21 15:07:25.000000 metal_python-0.9.5/metal_python/models/v1_machine_abort_reinstall_request.py
+-rw-r--r--   0 runner    (1001) docker     (116)    14022 2020-10-21 15:07:25.000000 metal_python-0.9.5/metal_python/models/v1_machine_allocate_request.py
+-rw-r--r--   0 runner    (1001) docker     (116)    14192 2020-10-21 15:07:25.000000 metal_python-0.9.5/metal_python/models/v1_machine_allocation.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4589 2020-10-21 15:07:25.000000 metal_python-0.9.5/metal_python/models/v1_machine_allocation_network.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4827 2020-10-21 15:07:25.000000 metal_python-0.9.5/metal_python/models/v1_machine_bios.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5888 2020-10-21 15:07:25.000000 metal_python-0.9.5/metal_python/models/v1_machine_block_device.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11282 2020-10-21 15:07:25.000000 metal_python-0.9.5/metal_python/models/v1_machine_disk_partition.py
+-rw-r--r--   0 runner    (1001) docker     (116)     9361 2020-10-21 15:07:25.000000 metal_python-0.9.5/metal_python/models/v1_machine_finalize_allocation_request.py
+-rw-r--r--   0 runner    (1001) docker     (116)    38301 2020-10-21 15:07:25.000000 metal_python-0.9.5/metal_python/models/v1_machine_find_request.py
+-rw-r--r--   0 runner    (1001) docker     (116)     9814 2020-10-21 15:07:25.000000 metal_python-0.9.5/metal_python/models/v1_machine_fru.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5968 2020-10-21 15:07:25.000000 metal_python-0.9.5/metal_python/models/v1_machine_hardware.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6204 2020-10-21 15:07:25.000000 metal_python-0.9.5/metal_python/models/v1_machine_hardware_extended.py
+-rw-r--r--   0 runner    (1001) docker     (116)     7495 2020-10-21 15:07:25.000000 metal_python-0.9.5/metal_python/models/v1_machine_ipmi.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5242 2020-10-21 15:07:25.000000 metal_python-0.9.5/metal_python/models/v1_machine_ipmi_report.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4472 2020-10-21 15:07:25.000000 metal_python-0.9.5/metal_python/models/v1_machine_ipmi_report_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)    16877 2020-10-21 15:07:25.000000 metal_python-0.9.5/metal_python/models/v1_machine_ipmi_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)    10566 2020-10-21 15:07:25.000000 metal_python-0.9.5/metal_python/models/v1_machine_network.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4021 2020-10-21 15:07:25.000000 metal_python-0.9.5/metal_python/models/v1_machine_nic.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5123 2020-10-21 15:07:25.000000 metal_python-0.9.5/metal_python/models/v1_machine_nic_extended.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4972 2020-10-21 15:07:25.000000 metal_python-0.9.5/metal_python/models/v1_machine_provisioning_event.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6100 2020-10-21 15:07:25.000000 metal_python-0.9.5/metal_python/models/v1_machine_recent_provisioning_events.py
+-rw-r--r--   0 runner    (1001) docker     (116)     8697 2020-10-21 15:07:25.000000 metal_python-0.9.5/metal_python/models/v1_machine_register_request.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5791 2020-10-21 15:07:25.000000 metal_python-0.9.5/metal_python/models/v1_machine_reinstall_request.py
+-rw-r--r--   0 runner    (1001) docker     (116)    15769 2020-10-21 15:07:25.000000 metal_python-0.9.5/metal_python/models/v1_machine_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4300 2020-10-21 15:07:25.000000 metal_python-0.9.5/metal_python/models/v1_machine_state.py
+-rw-r--r--   0 runner    (1001) docker     (116)     7601 2020-10-21 15:07:25.000000 metal_python-0.9.5/metal_python/models/v1_meta.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6776 2020-10-21 15:07:25.000000 metal_python-0.9.5/metal_python/models/v1_network_allocate_request.py
+-rw-r--r--   0 runner    (1001) docker     (116)    15475 2020-10-21 15:07:25.000000 metal_python-0.9.5/metal_python/models/v1_network_create_request.py
+-rw-r--r--   0 runner    (1001) docker     (116)    10938 2020-10-21 15:07:25.000000 metal_python-0.9.5/metal_python/models/v1_network_find_request.py
+-rw-r--r--   0 runner    (1001) docker     (116)    17559 2020-10-21 15:07:25.000000 metal_python-0.9.5/metal_python/models/v1_network_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6517 2020-10-21 15:07:25.000000 metal_python-0.9.5/metal_python/models/v1_network_update_request.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6284 2020-10-21 15:07:25.000000 metal_python-0.9.5/metal_python/models/v1_network_usage.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5209 2020-10-21 15:07:25.000000 metal_python-0.9.5/metal_python/models/v1_partition_boot_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5742 2020-10-21 15:07:25.000000 metal_python-0.9.5/metal_python/models/v1_partition_capacity.py
+-rw-r--r--   0 runner    (1001) docker     (116)     8770 2020-10-21 15:07:25.000000 metal_python-0.9.5/metal_python/models/v1_partition_create_request.py
+-rw-r--r--   0 runner    (1001) docker     (116)    10228 2020-10-21 15:07:25.000000 metal_python-0.9.5/metal_python/models/v1_partition_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6905 2020-10-21 15:07:25.000000 metal_python-0.9.5/metal_python/models/v1_partition_update_request.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5915 2020-10-21 15:07:25.000000 metal_python-0.9.5/metal_python/models/v1_project_create_request.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5148 2020-10-21 15:07:25.000000 metal_python-0.9.5/metal_python/models/v1_project_find_request.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5795 2020-10-21 15:07:25.000000 metal_python-0.9.5/metal_python/models/v1_project_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5915 2020-10-21 15:07:25.000000 metal_python-0.9.5/metal_python/models/v1_project_update_request.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3594 2020-10-21 15:07:25.000000 metal_python-0.9.5/metal_python/models/v1_quota.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4936 2020-10-21 15:07:25.000000 metal_python-0.9.5/metal_python/models/v1_quota_set.py
+-rw-r--r--   0 runner    (1001) docker     (116)     9494 2020-10-21 15:07:25.000000 metal_python-0.9.5/metal_python/models/v1_server_capacity.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5094 2020-10-21 15:07:25.000000 metal_python-0.9.5/metal_python/models/v1_size_constraint.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5290 2020-10-21 15:07:25.000000 metal_python-0.9.5/metal_python/models/v1_size_constraint_matching_log.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5844 2020-10-21 15:07:25.000000 metal_python-0.9.5/metal_python/models/v1_size_create_request.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5460 2020-10-21 15:07:25.000000 metal_python-0.9.5/metal_python/models/v1_size_matching_log.py
+-rw-r--r--   0 runner    (1001) docker     (116)     7302 2020-10-21 15:07:25.000000 metal_python-0.9.5/metal_python/models/v1_size_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5754 2020-10-21 15:07:25.000000 metal_python-0.9.5/metal_python/models/v1_size_update_request.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4170 2020-10-21 15:07:25.000000 metal_python-0.9.5/metal_python/models/v1_switch_connection.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5477 2020-10-21 15:07:25.000000 metal_python-0.9.5/metal_python/models/v1_switch_nic.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4248 2020-10-21 15:07:25.000000 metal_python-0.9.5/metal_python/models/v1_switch_notify_request.py
+-rw-r--r--   0 runner    (1001) docker     (116)     8416 2020-10-21 15:07:25.000000 metal_python-0.9.5/metal_python/models/v1_switch_register_request.py
+-rw-r--r--   0 runner    (1001) docker     (116)    12627 2020-10-21 15:07:25.000000 metal_python-0.9.5/metal_python/models/v1_switch_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4886 2020-10-21 15:07:25.000000 metal_python-0.9.5/metal_python/models/v1_switch_sync.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6480 2020-10-21 15:07:25.000000 metal_python-0.9.5/metal_python/models/v1_switch_update_request.py
+-rw-r--r--   0 runner    (1001) docker     (116)    13235 2020-10-21 15:07:25.000000 metal_python-0.9.5/metal_python/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-21 15:07:41.817566 metal_python-0.9.5/metal_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (116)      779 2020-10-21 15:07:41.000000 metal_python-0.9.5/metal_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)     7008 2020-10-21 15:07:41.000000 metal_python-0.9.5/metal_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2020-10-21 15:07:41.000000 metal_python-0.9.5/metal_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       91 2020-10-21 15:07:41.000000 metal_python-0.9.5/metal_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       18 2020-10-21 15:07:41.000000 metal_python-0.9.5/metal_python.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       38 2020-10-21 15:07:41.837566 metal_python-0.9.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (116)     1172 2020-10-21 15:07:25.000000 metal_python-0.9.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-21 15:07:41.837566 metal_python-0.9.5/test/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2020-10-21 15:07:25.000000 metal_python-0.9.5/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1362 2020-10-21 15:07:25.000000 metal_python-0.9.5/test/test_firewall_api.py
+-rw-r--r--   0 runner    (1001) docker     (116)      881 2020-10-21 15:07:25.000000 metal_python-0.9.5/test/test_health_api.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1069 2020-10-21 15:07:25.000000 metal_python-0.9.5/test/test_httperrors_http_error_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1734 2020-10-21 15:07:25.000000 metal_python-0.9.5/test/test_image_api.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1787 2020-10-21 15:07:25.000000 metal_python-0.9.5/test/test_ip_api.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4470 2020-10-21 15:07:25.000000 metal_python-0.9.5/test/test_machine_api.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2118 2020-10-21 15:07:25.000000 metal_python-0.9.5/test/test_network_api.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1820 2020-10-21 15:07:25.000000 metal_python-0.9.5/test/test_partition_api.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1745 2020-10-21 15:07:25.000000 metal_python-0.9.5/test/test_project_api.py
+-rw-r--r--   0 runner    (1001) docker     (116)      929 2020-10-21 15:07:25.000000 metal_python-0.9.5/test/test_rest_status.py
+-rw-r--r--   0 runner    (1001) docker     (116)      937 2020-10-21 15:07:25.000000 metal_python-0.9.5/test/test_rest_version.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1840 2020-10-21 15:07:25.000000 metal_python-0.9.5/test/test_size_api.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1738 2020-10-21 15:07:25.000000 metal_python-0.9.5/test/test_switch_api.py
+-rw-r--r--   0 runner    (1001) docker     (116)      939 2020-10-21 15:07:25.000000 metal_python-0.9.5/test/test_v1_bgp_filter.py
+-rw-r--r--   0 runner    (1001) docker     (116)      931 2020-10-21 15:07:25.000000 metal_python-0.9.5/test/test_v1_boot_info.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1055 2020-10-21 15:07:25.000000 metal_python-0.9.5/test/test_v1_chassis_identify_led_state.py
+-rw-r--r--   0 runner    (1001) docker     (116)      939 2020-10-21 15:07:25.000000 metal_python-0.9.5/test/test_v1_empty_body.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1037 2020-10-21 15:07:25.000000 metal_python-0.9.5/test/test_v1_firewall_create_request.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1021 2020-10-21 15:07:25.000000 metal_python-0.9.5/test/test_v1_firewall_find_request.py
+-rw-r--r--   0 runner    (1001) docker     (116)      995 2020-10-21 15:07:25.000000 metal_python-0.9.5/test/test_v1_firewall_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1013 2020-10-21 15:07:25.000000 metal_python-0.9.5/test/test_v1_image_create_request.py
+-rw-r--r--   0 runner    (1001) docker     (116)      971 2020-10-21 15:07:25.000000 metal_python-0.9.5/test/test_v1_image_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1013 2020-10-21 15:07:25.000000 metal_python-0.9.5/test/test_v1_image_update_request.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1005 2020-10-21 15:07:25.000000 metal_python-0.9.5/test/test_v1_ip_allocate_request.py
+-rw-r--r--   0 runner    (1001) docker     (116)      973 2020-10-21 15:07:25.000000 metal_python-0.9.5/test/test_v1_ip_find_request.py
+-rw-r--r--   0 runner    (1001) docker     (116)      947 2020-10-21 15:07:25.000000 metal_python-0.9.5/test/test_v1_ip_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)      989 2020-10-21 15:07:25.000000 metal_python-0.9.5/test/test_v1_ip_update_request.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1095 2020-10-21 15:07:25.000000 metal_python-0.9.5/test/test_v1_machine_abort_reinstall_request.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1045 2020-10-21 15:07:25.000000 metal_python-0.9.5/test/test_v1_machine_allocate_request.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1003 2020-10-21 15:07:25.000000 metal_python-0.9.5/test/test_v1_machine_allocation.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1061 2020-10-21 15:07:25.000000 metal_python-0.9.5/test/test_v1_machine_allocation_network.py
+-rw-r--r--   0 runner    (1001) docker     (116)      955 2020-10-21 15:07:25.000000 metal_python-0.9.5/test/test_v1_machine_bios.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1013 2020-10-21 15:07:25.000000 metal_python-0.9.5/test/test_v1_machine_block_device.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1029 2020-10-21 15:07:25.000000 metal_python-0.9.5/test/test_v1_machine_disk_partition.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1127 2020-10-21 15:07:25.000000 metal_python-0.9.5/test/test_v1_machine_finalize_allocation_request.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1013 2020-10-21 15:07:25.000000 metal_python-0.9.5/test/test_v1_machine_find_request.py
+-rw-r--r--   0 runner    (1001) docker     (116)      947 2020-10-21 15:07:25.000000 metal_python-0.9.5/test/test_v1_machine_fru.py
+-rw-r--r--   0 runner    (1001) docker     (116)      987 2020-10-21 15:07:25.000000 metal_python-0.9.5/test/test_v1_machine_hardware.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1053 2020-10-21 15:07:25.000000 metal_python-0.9.5/test/test_v1_machine_hardware_extended.py
+-rw-r--r--   0 runner    (1001) docker     (116)      955 2020-10-21 15:07:25.000000 metal_python-0.9.5/test/test_v1_machine_ipmi.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1005 2020-10-21 15:07:25.000000 metal_python-0.9.5/test/test_v1_machine_ipmi_report.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1071 2020-10-21 15:07:25.000000 metal_python-0.9.5/test/test_v1_machine_ipmi_report_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1021 2020-10-21 15:07:25.000000 metal_python-0.9.5/test/test_v1_machine_ipmi_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)      979 2020-10-21 15:07:25.000000 metal_python-0.9.5/test/test_v1_machine_network.py
+-rw-r--r--   0 runner    (1001) docker     (116)      947 2020-10-21 15:07:25.000000 metal_python-0.9.5/test/test_v1_machine_nic.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1013 2020-10-21 15:07:25.000000 metal_python-0.9.5/test/test_v1_machine_nic_extended.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1061 2020-10-21 15:07:25.000000 metal_python-0.9.5/test/test_v1_machine_provisioning_event.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1119 2020-10-21 15:07:25.000000 metal_python-0.9.5/test/test_v1_machine_recent_provisioning_events.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1045 2020-10-21 15:07:25.000000 metal_python-0.9.5/test/test_v1_machine_register_request.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1053 2020-10-21 15:07:25.000000 metal_python-0.9.5/test/test_v1_machine_reinstall_request.py
+-rw-r--r--   0 runner    (1001) docker     (116)      987 2020-10-21 15:07:25.000000 metal_python-0.9.5/test/test_v1_machine_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)      963 2020-10-21 15:07:25.000000 metal_python-0.9.5/test/test_v1_machine_state.py
+-rw-r--r--   0 runner    (1001) docker     (116)      897 2020-10-21 15:07:25.000000 metal_python-0.9.5/test/test_v1_meta.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1045 2020-10-21 15:07:25.000000 metal_python-0.9.5/test/test_v1_network_allocate_request.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1029 2020-10-21 15:07:25.000000 metal_python-0.9.5/test/test_v1_network_create_request.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1013 2020-10-21 15:07:25.000000 metal_python-0.9.5/test/test_v1_network_find_request.py
+-rw-r--r--   0 runner    (1001) docker     (116)      987 2020-10-21 15:07:25.000000 metal_python-0.9.5/test/test_v1_network_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1029 2020-10-21 15:07:25.000000 metal_python-0.9.5/test/test_v1_network_update_request.py
+-rw-r--r--   0 runner    (1001) docker     (116)      963 2020-10-21 15:07:25.000000 metal_python-0.9.5/test/test_v1_network_usage.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1077 2020-10-21 15:07:25.000000 metal_python-0.9.5/test/test_v1_partition_boot_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1003 2020-10-21 15:07:25.000000 metal_python-0.9.5/test/test_v1_partition_capacity.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1045 2020-10-21 15:07:25.000000 metal_python-0.9.5/test/test_v1_partition_create_request.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1003 2020-10-21 15:07:25.000000 metal_python-0.9.5/test/test_v1_partition_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1045 2020-10-21 15:07:25.000000 metal_python-0.9.5/test/test_v1_partition_update_request.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1029 2020-10-21 15:07:25.000000 metal_python-0.9.5/test/test_v1_project_create_request.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1013 2020-10-21 15:07:25.000000 metal_python-0.9.5/test/test_v1_project_find_request.py
+-rw-r--r--   0 runner    (1001) docker     (116)      987 2020-10-21 15:07:25.000000 metal_python-0.9.5/test/test_v1_project_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1029 2020-10-21 15:07:25.000000 metal_python-0.9.5/test/test_v1_project_update_request.py
+-rw-r--r--   0 runner    (1001) docker     (116)      905 2020-10-21 15:07:25.000000 metal_python-0.9.5/test/test_v1_quota.py
+-rw-r--r--   0 runner    (1001) docker     (116)      931 2020-10-21 15:07:25.000000 metal_python-0.9.5/test/test_v1_quota_set.py
+-rw-r--r--   0 runner    (1001) docker     (116)      979 2020-10-21 15:07:25.000000 metal_python-0.9.5/test/test_v1_server_capacity.py
+-rw-r--r--   0 runner    (1001) docker     (116)      979 2020-10-21 15:07:25.000000 metal_python-0.9.5/test/test_v1_size_constraint.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1071 2020-10-21 15:07:25.000000 metal_python-0.9.5/test/test_v1_size_constraint_matching_log.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1005 2020-10-21 15:07:25.000000 metal_python-0.9.5/test/test_v1_size_create_request.py
+-rw-r--r--   0 runner    (1001) docker     (116)      989 2020-10-21 15:07:25.000000 metal_python-0.9.5/test/test_v1_size_matching_log.py
+-rw-r--r--   0 runner    (1001) docker     (116)      963 2020-10-21 15:07:25.000000 metal_python-0.9.5/test/test_v1_size_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1005 2020-10-21 15:07:25.000000 metal_python-0.9.5/test/test_v1_size_update_request.py
+-rw-r--r--   0 runner    (1001) docker     (116)      995 2020-10-21 15:07:25.000000 metal_python-0.9.5/test/test_v1_switch_connection.py
+-rw-r--r--   0 runner    (1001) docker     (116)      939 2020-10-21 15:07:25.000000 metal_python-0.9.5/test/test_v1_switch_nic.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1021 2020-10-21 15:07:25.000000 metal_python-0.9.5/test/test_v1_switch_notify_request.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1037 2020-10-21 15:07:25.000000 metal_python-0.9.5/test/test_v1_switch_register_request.py
+-rw-r--r--   0 runner    (1001) docker     (116)      979 2020-10-21 15:07:25.000000 metal_python-0.9.5/test/test_v1_switch_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)      947 2020-10-21 15:07:25.000000 metal_python-0.9.5/test/test_v1_switch_sync.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1021 2020-10-21 15:07:25.000000 metal_python-0.9.5/test/test_v1_switch_update_request.py
+-rw-r--r--   0 runner    (1001) docker     (116)      916 2020-10-21 15:07:25.000000 metal_python-0.9.5/test/test_version_api.py
```

### Comparing `metal_python-0.9.4/PKG-INFO` & `metal_python-0.9.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metal_python
-Version: 0.9.4
+Version: 0.9.5
 Summary: Python API client for metal-api
 Home-page: https://github.com/metal-stack/metal-python
 Author: metal-stack authors
 License: MIT
 Description: UNKNOWN
 Keywords: metal-stack,metal-api,swagger,swagger-client
 Platform: UNKNOWN
```

### Comparing `metal_python-0.9.4/metal_python/__init__.py` & `metal_python-0.9.5/metal_python/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # flake8: noqa
 
 """
     metal-api
 
     API to manage and control plane resources like machines, switches, operating system images, machine sizes, networks, IP addresses and more  # noqa: E501
 
-    OpenAPI spec version: v0.9.4
+    OpenAPI spec version: v0.9.5
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `metal_python-0.9.4/metal_python/api/__init__.py` & `metal_python-0.9.5/metal_python/api/__init__.py`

 * *Files identical despite different names*

### Comparing `metal_python-0.9.4/metal_python/api/firewall_api.py` & `metal_python-0.9.5/metal_python/api/firewall_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     metal-api
 
     API to manage and control plane resources like machines, switches, operating system images, machine sizes, networks, IP addresses and more  # noqa: E501
 
-    OpenAPI spec version: v0.9.4
+    OpenAPI spec version: v0.9.5
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `metal_python-0.9.4/metal_python/api/health_api.py` & `metal_python-0.9.5/metal_python/api/health_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     metal-api
 
     API to manage and control plane resources like machines, switches, operating system images, machine sizes, networks, IP addresses and more  # noqa: E501
 
-    OpenAPI spec version: v0.9.4
+    OpenAPI spec version: v0.9.5
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `metal_python-0.9.4/metal_python/api/image_api.py` & `metal_python-0.9.5/metal_python/api/image_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     metal-api
 
     API to manage and control plane resources like machines, switches, operating system images, machine sizes, networks, IP addresses and more  # noqa: E501
 
-    OpenAPI spec version: v0.9.4
+    OpenAPI spec version: v0.9.5
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `metal_python-0.9.4/metal_python/api/ip_api.py` & `metal_python-0.9.5/metal_python/api/ip_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     metal-api
 
     API to manage and control plane resources like machines, switches, operating system images, machine sizes, networks, IP addresses and more  # noqa: E501
 
-    OpenAPI spec version: v0.9.4
+    OpenAPI spec version: v0.9.5
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `metal_python-0.9.4/metal_python/api/machine_api.py` & `metal_python-0.9.5/metal_python/api/machine_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     metal-api
 
     API to manage and control plane resources like machines, switches, operating system images, machine sizes, networks, IP addresses and more  # noqa: E501
 
-    OpenAPI spec version: v0.9.4
+    OpenAPI spec version: v0.9.5
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `metal_python-0.9.4/metal_python/api/network_api.py` & `metal_python-0.9.5/metal_python/api/network_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     metal-api
 
     API to manage and control plane resources like machines, switches, operating system images, machine sizes, networks, IP addresses and more  # noqa: E501
 
-    OpenAPI spec version: v0.9.4
+    OpenAPI spec version: v0.9.5
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `metal_python-0.9.4/metal_python/api/partition_api.py` & `metal_python-0.9.5/metal_python/api/partition_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     metal-api
 
     API to manage and control plane resources like machines, switches, operating system images, machine sizes, networks, IP addresses and more  # noqa: E501
 
-    OpenAPI spec version: v0.9.4
+    OpenAPI spec version: v0.9.5
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `metal_python-0.9.4/metal_python/api/project_api.py` & `metal_python-0.9.5/metal_python/api/project_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     metal-api
 
     API to manage and control plane resources like machines, switches, operating system images, machine sizes, networks, IP addresses and more  # noqa: E501
 
-    OpenAPI spec version: v0.9.4
+    OpenAPI spec version: v0.9.5
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `metal_python-0.9.4/metal_python/api/size_api.py` & `metal_python-0.9.5/metal_python/api/size_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     metal-api
 
     API to manage and control plane resources like machines, switches, operating system images, machine sizes, networks, IP addresses and more  # noqa: E501
 
-    OpenAPI spec version: v0.9.4
+    OpenAPI spec version: v0.9.5
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `metal_python-0.9.4/metal_python/api/switch_api.py` & `metal_python-0.9.5/metal_python/api/switch_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     metal-api
 
     API to manage and control plane resources like machines, switches, operating system images, machine sizes, networks, IP addresses and more  # noqa: E501
 
-    OpenAPI spec version: v0.9.4
+    OpenAPI spec version: v0.9.5
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `metal_python-0.9.4/metal_python/api/version_api.py` & `metal_python-0.9.5/metal_python/api/version_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     metal-api
 
     API to manage and control plane resources like machines, switches, operating system images, machine sizes, networks, IP addresses and more  # noqa: E501
 
-    OpenAPI spec version: v0.9.4
+    OpenAPI spec version: v0.9.5
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `metal_python-0.9.4/metal_python/api_client.py` & `metal_python-0.9.5/metal_python/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     metal-api
 
     API to manage and control plane resources like machines, switches, operating system images, machine sizes, networks, IP addresses and more  # noqa: E501
 
-    OpenAPI spec version: v0.9.4
+    OpenAPI spec version: v0.9.5
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import datetime
@@ -70,15 +70,15 @@
         self._pool = None
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'Swagger-Codegen/v0.9.4/python'
+        self.user_agent = 'Swagger-Codegen/v0.9.5/python'
 
     def __del__(self):
         if self._pool is not None:
             self._pool.close()
             self._pool.join()
 
     @property
```

### Comparing `metal_python-0.9.4/metal_python/configuration.py` & `metal_python-0.9.5/metal_python/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     metal-api
 
     API to manage and control plane resources like machines, switches, operating system images, machine sizes, networks, IP addresses and more  # noqa: E501
 
-    OpenAPI spec version: v0.9.4
+    OpenAPI spec version: v0.9.5
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
 
@@ -250,10 +250,10 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: v0.9.4\n"\
-               "SDK Package Version: v0.9.4".\
+               "Version of the API: v0.9.5\n"\
+               "SDK Package Version: v0.9.5".\
                format(env=sys.platform, pyversion=sys.version)
```

### Comparing `metal_python-0.9.4/metal_python/driver.py` & `metal_python-0.9.5/metal_python/driver.py`

 * *Files identical despite different names*

### Comparing `metal_python-0.9.4/metal_python/models/__init__.py` & `metal_python-0.9.5/metal_python/models/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # flake8: noqa
 """
     metal-api
 
     API to manage and control plane resources like machines, switches, operating system images, machine sizes, networks, IP addresses and more  # noqa: E501
 
-    OpenAPI spec version: v0.9.4
+    OpenAPI spec version: v0.9.5
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `metal_python-0.9.4/metal_python/models/httperrors_http_error_response.py` & `metal_python-0.9.5/metal_python/models/httperrors_http_error_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     metal-api
 
     API to manage and control plane resources like machines, switches, operating system images, machine sizes, networks, IP addresses and more  # noqa: E501
 
-    OpenAPI spec version: v0.9.4
+    OpenAPI spec version: v0.9.5
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `metal_python-0.9.4/metal_python/models/rest_status.py` & `metal_python-0.9.5/metal_python/models/rest_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     metal-api
 
     API to manage and control plane resources like machines, switches, operating system images, machine sizes, networks, IP addresses and more  # noqa: E501
 
-    OpenAPI spec version: v0.9.4
+    OpenAPI spec version: v0.9.5
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `metal_python-0.9.4/metal_python/models/rest_version.py` & `metal_python-0.9.5/metal_python/models/rest_version.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     metal-api
 
     API to manage and control plane resources like machines, switches, operating system images, machine sizes, networks, IP addresses and more  # noqa: E501
 
-    OpenAPI spec version: v0.9.4
+    OpenAPI spec version: v0.9.5
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `metal_python-0.9.4/metal_python/models/v1_bgp_filter.py` & `metal_python-0.9.5/metal_python/models/v1_bgp_filter.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     metal-api
 
     API to manage and control plane resources like machines, switches, operating system images, machine sizes, networks, IP addresses and more  # noqa: E501
 
-    OpenAPI spec version: v0.9.4
+    OpenAPI spec version: v0.9.5
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `metal_python-0.9.4/metal_python/models/v1_boot_info.py` & `metal_python-0.9.5/metal_python/models/v1_boot_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     metal-api
 
     API to manage and control plane resources like machines, switches, operating system images, machine sizes, networks, IP addresses and more  # noqa: E501
 
-    OpenAPI spec version: v0.9.4
+    OpenAPI spec version: v0.9.5
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `metal_python-0.9.4/metal_python/models/v1_chassis_identify_led_state.py` & `metal_python-0.9.5/metal_python/models/v1_chassis_identify_led_state.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     metal-api
 
     API to manage and control plane resources like machines, switches, operating system images, machine sizes, networks, IP addresses and more  # noqa: E501
 
-    OpenAPI spec version: v0.9.4
+    OpenAPI spec version: v0.9.5
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `metal_python-0.9.4/metal_python/models/v1_empty_body.py` & `metal_python-0.9.5/metal_python/models/v1_empty_body.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     metal-api
 
     API to manage and control plane resources like machines, switches, operating system images, machine sizes, networks, IP addresses and more  # noqa: E501
 
-    OpenAPI spec version: v0.9.4
+    OpenAPI spec version: v0.9.5
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `metal_python-0.9.4/metal_python/models/v1_firewall_create_request.py` & `metal_python-0.9.5/metal_python/models/v1_firewall_create_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     metal-api
 
     API to manage and control plane resources like machines, switches, operating system images, machine sizes, networks, IP addresses and more  # noqa: E501
 
-    OpenAPI spec version: v0.9.4
+    OpenAPI spec version: v0.9.5
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `metal_python-0.9.4/metal_python/models/v1_firewall_find_request.py` & `metal_python-0.9.5/metal_python/models/v1_firewall_find_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     metal-api
 
     API to manage and control plane resources like machines, switches, operating system images, machine sizes, networks, IP addresses and more  # noqa: E501
 
-    OpenAPI spec version: v0.9.4
+    OpenAPI spec version: v0.9.5
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
@@ -49,15 +49,14 @@
         'hardware_cpu_cores': 'int',
         'hardware_memory': 'int',
         'id': 'str',
         'ipmi_address': 'str',
         'ipmi_interface': 'str',
         'ipmi_mac_address': 'str',
         'ipmi_user': 'str',
-        'liveliness': 'str',
         'name': 'str',
         'network_asns': 'list[int]',
         'network_destination_prefixes': 'list[str]',
         'network_ids': 'list[str]',
         'network_ips': 'list[str]',
         'network_nat': 'bool',
         'network_prefixes': 'list[str]',
@@ -96,15 +95,14 @@
         'hardware_cpu_cores': 'hardware_cpu_cores',
         'hardware_memory': 'hardware_memory',
         'id': 'id',
         'ipmi_address': 'ipmi_address',
         'ipmi_interface': 'ipmi_interface',
         'ipmi_mac_address': 'ipmi_mac_address',
         'ipmi_user': 'ipmi_user',
-        'liveliness': 'liveliness',
         'name': 'name',
         'network_asns': 'network_asns',
         'network_destination_prefixes': 'network_destination_prefixes',
         'network_ids': 'network_ids',
         'network_ips': 'network_ips',
         'network_nat': 'network_nat',
         'network_prefixes': 'network_prefixes',
@@ -120,15 +118,15 @@
         'partition_id': 'partition_id',
         'rackid': 'rackid',
         'sizeid': 'sizeid',
         'state_value': 'state_value',
         'tags': 'tags'
     }
 
-    def __init__(self, allocation_hostname=None, allocation_image_id=None, allocation_name=None, allocation_project=None, allocation_succeeded=None, disk_names=None, disk_sizes=None, fru_board_mfg=None, fru_board_mfg_serial=None, fru_board_part_number=None, fru_chassis_part_number=None, fru_chassis_part_serial=None, fru_product_manufacturer=None, fru_product_part_number=None, fru_product_serial=None, hardware_cpu_cores=None, hardware_memory=None, id=None, ipmi_address=None, ipmi_interface=None, ipmi_mac_address=None, ipmi_user=None, liveliness=None, name=None, network_asns=None, network_destination_prefixes=None, network_ids=None, network_ips=None, network_nat=None, network_prefixes=None, network_private=None, network_underlay=None, network_vrfs=None, nics_mac_addresses=None, nics_names=None, nics_neighbor_mac_addresses=None, nics_neighbor_names=None, nics_neighbor_vrfs=None, nics_vrfs=None, partition_id=None, rackid=None, sizeid=None, state_value=None, tags=None):  # noqa: E501
+    def __init__(self, allocation_hostname=None, allocation_image_id=None, allocation_name=None, allocation_project=None, allocation_succeeded=None, disk_names=None, disk_sizes=None, fru_board_mfg=None, fru_board_mfg_serial=None, fru_board_part_number=None, fru_chassis_part_number=None, fru_chassis_part_serial=None, fru_product_manufacturer=None, fru_product_part_number=None, fru_product_serial=None, hardware_cpu_cores=None, hardware_memory=None, id=None, ipmi_address=None, ipmi_interface=None, ipmi_mac_address=None, ipmi_user=None, name=None, network_asns=None, network_destination_prefixes=None, network_ids=None, network_ips=None, network_nat=None, network_prefixes=None, network_private=None, network_underlay=None, network_vrfs=None, nics_mac_addresses=None, nics_names=None, nics_neighbor_mac_addresses=None, nics_neighbor_names=None, nics_neighbor_vrfs=None, nics_vrfs=None, partition_id=None, rackid=None, sizeid=None, state_value=None, tags=None):  # noqa: E501
         """V1FirewallFindRequest - a model defined in Swagger"""  # noqa: E501
 
         self._allocation_hostname = None
         self._allocation_image_id = None
         self._allocation_name = None
         self._allocation_project = None
         self._allocation_succeeded = None
@@ -145,15 +143,14 @@
         self._hardware_cpu_cores = None
         self._hardware_memory = None
         self._id = None
         self._ipmi_address = None
         self._ipmi_interface = None
         self._ipmi_mac_address = None
         self._ipmi_user = None
-        self._liveliness = None
         self._name = None
         self._network_asns = None
         self._network_destination_prefixes = None
         self._network_ids = None
         self._network_ips = None
         self._network_nat = None
         self._network_prefixes = None
@@ -213,16 +210,14 @@
             self.ipmi_address = ipmi_address
         if ipmi_interface is not None:
             self.ipmi_interface = ipmi_interface
         if ipmi_mac_address is not None:
             self.ipmi_mac_address = ipmi_mac_address
         if ipmi_user is not None:
             self.ipmi_user = ipmi_user
-        if liveliness is not None:
-            self.liveliness = liveliness
         if name is not None:
             self.name = name
         if network_asns is not None:
             self.network_asns = network_asns
         if network_destination_prefixes is not None:
             self.network_destination_prefixes = network_destination_prefixes
         if network_ids is not None:
@@ -721,35 +716,14 @@
         :param ipmi_user: The ipmi_user of this V1FirewallFindRequest.  # noqa: E501
         :type: str
         """
 
         self._ipmi_user = ipmi_user
 
     @property
-    def liveliness(self):
-        """Gets the liveliness of this V1FirewallFindRequest.  # noqa: E501
-
-
-        :return: The liveliness of this V1FirewallFindRequest.  # noqa: E501
-        :rtype: str
-        """
-        return self._liveliness
-
-    @liveliness.setter
-    def liveliness(self, liveliness):
-        """Sets the liveliness of this V1FirewallFindRequest.
-
-
-        :param liveliness: The liveliness of this V1FirewallFindRequest.  # noqa: E501
-        :type: str
-        """
-
-        self._liveliness = liveliness
-
-    @property
     def name(self):
         """Gets the name of this V1FirewallFindRequest.  # noqa: E501
 
 
         :return: The name of this V1FirewallFindRequest.  # noqa: E501
         :rtype: str
         """
```

### Comparing `metal_python-0.9.4/metal_python/models/v1_firewall_response.py` & `metal_python-0.9.5/metal_python/models/v1_firewall_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     metal-api
 
     API to manage and control plane resources like machines, switches, operating system images, machine sizes, networks, IP addresses and more  # noqa: E501
 
-    OpenAPI spec version: v0.9.4
+    OpenAPI spec version: v0.9.5
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `metal_python-0.9.4/metal_python/models/v1_image_create_request.py` & `metal_python-0.9.5/metal_python/models/v1_image_create_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     metal-api
 
     API to manage and control plane resources like machines, switches, operating system images, machine sizes, networks, IP addresses and more  # noqa: E501
 
-    OpenAPI spec version: v0.9.4
+    OpenAPI spec version: v0.9.5
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `metal_python-0.9.4/metal_python/models/v1_image_response.py` & `metal_python-0.9.5/metal_python/models/v1_image_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     metal-api
 
     API to manage and control plane resources like machines, switches, operating system images, machine sizes, networks, IP addresses and more  # noqa: E501
 
-    OpenAPI spec version: v0.9.4
+    OpenAPI spec version: v0.9.5
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `metal_python-0.9.4/metal_python/models/v1_image_update_request.py` & `metal_python-0.9.5/metal_python/models/v1_image_update_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     metal-api
 
     API to manage and control plane resources like machines, switches, operating system images, machine sizes, networks, IP addresses and more  # noqa: E501
 
-    OpenAPI spec version: v0.9.4
+    OpenAPI spec version: v0.9.5
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `metal_python-0.9.4/metal_python/models/v1_ip_allocate_request.py` & `metal_python-0.9.5/metal_python/models/v1_ip_allocate_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     metal-api
 
     API to manage and control plane resources like machines, switches, operating system images, machine sizes, networks, IP addresses and more  # noqa: E501
 
-    OpenAPI spec version: v0.9.4
+    OpenAPI spec version: v0.9.5
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `metal_python-0.9.4/metal_python/models/v1_ip_find_request.py` & `metal_python-0.9.5/metal_python/models/v1_ip_find_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     metal-api
 
     API to manage and control plane resources like machines, switches, operating system images, machine sizes, networks, IP addresses and more  # noqa: E501
 
-    OpenAPI spec version: v0.9.4
+    OpenAPI spec version: v0.9.5
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `metal_python-0.9.4/metal_python/models/v1_ip_response.py` & `metal_python-0.9.5/metal_python/models/v1_ip_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     metal-api
 
     API to manage and control plane resources like machines, switches, operating system images, machine sizes, networks, IP addresses and more  # noqa: E501
 
-    OpenAPI spec version: v0.9.4
+    OpenAPI spec version: v0.9.5
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `metal_python-0.9.4/metal_python/models/v1_ip_update_request.py` & `metal_python-0.9.5/metal_python/models/v1_ip_update_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     metal-api
 
     API to manage and control plane resources like machines, switches, operating system images, machine sizes, networks, IP addresses and more  # noqa: E501
 
-    OpenAPI spec version: v0.9.4
+    OpenAPI spec version: v0.9.5
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `metal_python-0.9.4/metal_python/models/v1_machine_abort_reinstall_request.py` & `metal_python-0.9.5/metal_python/models/v1_machine_abort_reinstall_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     metal-api
 
     API to manage and control plane resources like machines, switches, operating system images, machine sizes, networks, IP addresses and more  # noqa: E501
 
-    OpenAPI spec version: v0.9.4
+    OpenAPI spec version: v0.9.5
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `metal_python-0.9.4/metal_python/models/v1_machine_allocate_request.py` & `metal_python-0.9.5/metal_python/models/v1_machine_allocate_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     metal-api
 
     API to manage and control plane resources like machines, switches, operating system images, machine sizes, networks, IP addresses and more  # noqa: E501
 
-    OpenAPI spec version: v0.9.4
+    OpenAPI spec version: v0.9.5
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `metal_python-0.9.4/metal_python/models/v1_machine_allocation.py` & `metal_python-0.9.5/metal_python/models/v1_machine_allocation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     metal-api
 
     API to manage and control plane resources like machines, switches, operating system images, machine sizes, networks, IP addresses and more  # noqa: E501
 
-    OpenAPI spec version: v0.9.4
+    OpenAPI spec version: v0.9.5
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `metal_python-0.9.4/metal_python/models/v1_machine_allocation_network.py` & `metal_python-0.9.5/metal_python/models/v1_machine_allocation_network.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     metal-api
 
     API to manage and control plane resources like machines, switches, operating system images, machine sizes, networks, IP addresses and more  # noqa: E501
 
-    OpenAPI spec version: v0.9.4
+    OpenAPI spec version: v0.9.5
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `metal_python-0.9.4/metal_python/models/v1_machine_bios.py` & `metal_python-0.9.5/metal_python/models/v1_machine_bios.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     metal-api
 
     API to manage and control plane resources like machines, switches, operating system images, machine sizes, networks, IP addresses and more  # noqa: E501
 
-    OpenAPI spec version: v0.9.4
+    OpenAPI spec version: v0.9.5
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `metal_python-0.9.4/metal_python/models/v1_machine_block_device.py` & `metal_python-0.9.5/metal_python/models/v1_machine_block_device.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     metal-api
 
     API to manage and control plane resources like machines, switches, operating system images, machine sizes, networks, IP addresses and more  # noqa: E501
 
-    OpenAPI spec version: v0.9.4
+    OpenAPI spec version: v0.9.5
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `metal_python-0.9.4/metal_python/models/v1_machine_disk_partition.py` & `metal_python-0.9.5/metal_python/models/v1_machine_disk_partition.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     metal-api
 
     API to manage and control plane resources like machines, switches, operating system images, machine sizes, networks, IP addresses and more  # noqa: E501
 
-    OpenAPI spec version: v0.9.4
+    OpenAPI spec version: v0.9.5
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `metal_python-0.9.4/metal_python/models/v1_machine_finalize_allocation_request.py` & `metal_python-0.9.5/metal_python/models/v1_machine_finalize_allocation_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     metal-api
 
     API to manage and control plane resources like machines, switches, operating system images, machine sizes, networks, IP addresses and more  # noqa: E501
 
-    OpenAPI spec version: v0.9.4
+    OpenAPI spec version: v0.9.5
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `metal_python-0.9.4/metal_python/models/v1_machine_find_request.py` & `metal_python-0.9.5/metal_python/models/v1_machine_find_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     metal-api
 
     API to manage and control plane resources like machines, switches, operating system images, machine sizes, networks, IP addresses and more  # noqa: E501
 
-    OpenAPI spec version: v0.9.4
+    OpenAPI spec version: v0.9.5
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
@@ -49,15 +49,14 @@
         'hardware_cpu_cores': 'int',
         'hardware_memory': 'int',
         'id': 'str',
         'ipmi_address': 'str',
         'ipmi_interface': 'str',
         'ipmi_mac_address': 'str',
         'ipmi_user': 'str',
-        'liveliness': 'str',
         'name': 'str',
         'network_asns': 'list[int]',
         'network_destination_prefixes': 'list[str]',
         'network_ids': 'list[str]',
         'network_ips': 'list[str]',
         'network_nat': 'bool',
         'network_prefixes': 'list[str]',
@@ -96,15 +95,14 @@
         'hardware_cpu_cores': 'hardware_cpu_cores',
         'hardware_memory': 'hardware_memory',
         'id': 'id',
         'ipmi_address': 'ipmi_address',
         'ipmi_interface': 'ipmi_interface',
         'ipmi_mac_address': 'ipmi_mac_address',
         'ipmi_user': 'ipmi_user',
-        'liveliness': 'liveliness',
         'name': 'name',
         'network_asns': 'network_asns',
         'network_destination_prefixes': 'network_destination_prefixes',
         'network_ids': 'network_ids',
         'network_ips': 'network_ips',
         'network_nat': 'network_nat',
         'network_prefixes': 'network_prefixes',
@@ -120,15 +118,15 @@
         'partition_id': 'partition_id',
         'rackid': 'rackid',
         'sizeid': 'sizeid',
         'state_value': 'state_value',
         'tags': 'tags'
     }
 
-    def __init__(self, allocation_hostname=None, allocation_image_id=None, allocation_name=None, allocation_project=None, allocation_succeeded=None, disk_names=None, disk_sizes=None, fru_board_mfg=None, fru_board_mfg_serial=None, fru_board_part_number=None, fru_chassis_part_number=None, fru_chassis_part_serial=None, fru_product_manufacturer=None, fru_product_part_number=None, fru_product_serial=None, hardware_cpu_cores=None, hardware_memory=None, id=None, ipmi_address=None, ipmi_interface=None, ipmi_mac_address=None, ipmi_user=None, liveliness=None, name=None, network_asns=None, network_destination_prefixes=None, network_ids=None, network_ips=None, network_nat=None, network_prefixes=None, network_private=None, network_underlay=None, network_vrfs=None, nics_mac_addresses=None, nics_names=None, nics_neighbor_mac_addresses=None, nics_neighbor_names=None, nics_neighbor_vrfs=None, nics_vrfs=None, partition_id=None, rackid=None, sizeid=None, state_value=None, tags=None):  # noqa: E501
+    def __init__(self, allocation_hostname=None, allocation_image_id=None, allocation_name=None, allocation_project=None, allocation_succeeded=None, disk_names=None, disk_sizes=None, fru_board_mfg=None, fru_board_mfg_serial=None, fru_board_part_number=None, fru_chassis_part_number=None, fru_chassis_part_serial=None, fru_product_manufacturer=None, fru_product_part_number=None, fru_product_serial=None, hardware_cpu_cores=None, hardware_memory=None, id=None, ipmi_address=None, ipmi_interface=None, ipmi_mac_address=None, ipmi_user=None, name=None, network_asns=None, network_destination_prefixes=None, network_ids=None, network_ips=None, network_nat=None, network_prefixes=None, network_private=None, network_underlay=None, network_vrfs=None, nics_mac_addresses=None, nics_names=None, nics_neighbor_mac_addresses=None, nics_neighbor_names=None, nics_neighbor_vrfs=None, nics_vrfs=None, partition_id=None, rackid=None, sizeid=None, state_value=None, tags=None):  # noqa: E501
         """V1MachineFindRequest - a model defined in Swagger"""  # noqa: E501
 
         self._allocation_hostname = None
         self._allocation_image_id = None
         self._allocation_name = None
         self._allocation_project = None
         self._allocation_succeeded = None
@@ -145,15 +143,14 @@
         self._hardware_cpu_cores = None
         self._hardware_memory = None
         self._id = None
         self._ipmi_address = None
         self._ipmi_interface = None
         self._ipmi_mac_address = None
         self._ipmi_user = None
-        self._liveliness = None
         self._name = None
         self._network_asns = None
         self._network_destination_prefixes = None
         self._network_ids = None
         self._network_ips = None
         self._network_nat = None
         self._network_prefixes = None
@@ -213,16 +210,14 @@
             self.ipmi_address = ipmi_address
         if ipmi_interface is not None:
             self.ipmi_interface = ipmi_interface
         if ipmi_mac_address is not None:
             self.ipmi_mac_address = ipmi_mac_address
         if ipmi_user is not None:
             self.ipmi_user = ipmi_user
-        if liveliness is not None:
-            self.liveliness = liveliness
         if name is not None:
             self.name = name
         if network_asns is not None:
             self.network_asns = network_asns
         if network_destination_prefixes is not None:
             self.network_destination_prefixes = network_destination_prefixes
         if network_ids is not None:
@@ -721,35 +716,14 @@
         :param ipmi_user: The ipmi_user of this V1MachineFindRequest.  # noqa: E501
         :type: str
         """
 
         self._ipmi_user = ipmi_user
 
     @property
-    def liveliness(self):
-        """Gets the liveliness of this V1MachineFindRequest.  # noqa: E501
-
-
-        :return: The liveliness of this V1MachineFindRequest.  # noqa: E501
-        :rtype: str
-        """
-        return self._liveliness
-
-    @liveliness.setter
-    def liveliness(self, liveliness):
-        """Sets the liveliness of this V1MachineFindRequest.
-
-
-        :param liveliness: The liveliness of this V1MachineFindRequest.  # noqa: E501
-        :type: str
-        """
-
-        self._liveliness = liveliness
-
-    @property
     def name(self):
         """Gets the name of this V1MachineFindRequest.  # noqa: E501
 
 
         :return: The name of this V1MachineFindRequest.  # noqa: E501
         :rtype: str
         """
```

### Comparing `metal_python-0.9.4/metal_python/models/v1_machine_fru.py` & `metal_python-0.9.5/metal_python/models/v1_machine_fru.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     metal-api
 
     API to manage and control plane resources like machines, switches, operating system images, machine sizes, networks, IP addresses and more  # noqa: E501
 
-    OpenAPI spec version: v0.9.4
+    OpenAPI spec version: v0.9.5
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `metal_python-0.9.4/metal_python/models/v1_machine_hardware.py` & `metal_python-0.9.5/metal_python/models/v1_machine_hardware.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     metal-api
 
     API to manage and control plane resources like machines, switches, operating system images, machine sizes, networks, IP addresses and more  # noqa: E501
 
-    OpenAPI spec version: v0.9.4
+    OpenAPI spec version: v0.9.5
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `metal_python-0.9.4/metal_python/models/v1_machine_hardware_extended.py` & `metal_python-0.9.5/metal_python/models/v1_machine_hardware_extended.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     metal-api
 
     API to manage and control plane resources like machines, switches, operating system images, machine sizes, networks, IP addresses and more  # noqa: E501
 
-    OpenAPI spec version: v0.9.4
+    OpenAPI spec version: v0.9.5
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `metal_python-0.9.4/metal_python/models/v1_machine_ipmi.py` & `metal_python-0.9.5/metal_python/models/v1_machine_ipmi.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     metal-api
 
     API to manage and control plane resources like machines, switches, operating system images, machine sizes, networks, IP addresses and more  # noqa: E501
 
-    OpenAPI spec version: v0.9.4
+    OpenAPI spec version: v0.9.5
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `metal_python-0.9.4/metal_python/models/v1_machine_ipmi_report.py` & `metal_python-0.9.5/metal_python/models/v1_machine_ipmi_report.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     metal-api
 
     API to manage and control plane resources like machines, switches, operating system images, machine sizes, networks, IP addresses and more  # noqa: E501
 
-    OpenAPI spec version: v0.9.4
+    OpenAPI spec version: v0.9.5
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `metal_python-0.9.4/metal_python/models/v1_machine_ipmi_report_response.py` & `metal_python-0.9.5/metal_python/models/v1_machine_ipmi_report_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     metal-api
 
     API to manage and control plane resources like machines, switches, operating system images, machine sizes, networks, IP addresses and more  # noqa: E501
 
-    OpenAPI spec version: v0.9.4
+    OpenAPI spec version: v0.9.5
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `metal_python-0.9.4/metal_python/models/v1_machine_ipmi_response.py` & `metal_python-0.9.5/metal_python/models/v1_machine_ipmi_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     metal-api
 
     API to manage and control plane resources like machines, switches, operating system images, machine sizes, networks, IP addresses and more  # noqa: E501
 
-    OpenAPI spec version: v0.9.4
+    OpenAPI spec version: v0.9.5
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `metal_python-0.9.4/metal_python/models/v1_machine_network.py` & `metal_python-0.9.5/metal_python/models/v1_machine_network.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     metal-api
 
     API to manage and control plane resources like machines, switches, operating system images, machine sizes, networks, IP addresses and more  # noqa: E501
 
-    OpenAPI spec version: v0.9.4
+    OpenAPI spec version: v0.9.5
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `metal_python-0.9.4/metal_python/models/v1_machine_nic.py` & `metal_python-0.9.5/metal_python/models/v1_machine_nic.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     metal-api
 
     API to manage and control plane resources like machines, switches, operating system images, machine sizes, networks, IP addresses and more  # noqa: E501
 
-    OpenAPI spec version: v0.9.4
+    OpenAPI spec version: v0.9.5
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `metal_python-0.9.4/metal_python/models/v1_machine_nic_extended.py` & `metal_python-0.9.5/metal_python/models/v1_machine_nic_extended.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     metal-api
 
     API to manage and control plane resources like machines, switches, operating system images, machine sizes, networks, IP addresses and more  # noqa: E501
 
-    OpenAPI spec version: v0.9.4
+    OpenAPI spec version: v0.9.5
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `metal_python-0.9.4/metal_python/models/v1_machine_provisioning_event.py` & `metal_python-0.9.5/metal_python/models/v1_machine_provisioning_event.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     metal-api
 
     API to manage and control plane resources like machines, switches, operating system images, machine sizes, networks, IP addresses and more  # noqa: E501
 
-    OpenAPI spec version: v0.9.4
+    OpenAPI spec version: v0.9.5
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `metal_python-0.9.4/metal_python/models/v1_machine_recent_provisioning_events.py` & `metal_python-0.9.5/metal_python/models/v1_machine_recent_provisioning_events.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     metal-api
 
     API to manage and control plane resources like machines, switches, operating system images, machine sizes, networks, IP addresses and more  # noqa: E501
 
-    OpenAPI spec version: v0.9.4
+    OpenAPI spec version: v0.9.5
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `metal_python-0.9.4/metal_python/models/v1_machine_register_request.py` & `metal_python-0.9.5/metal_python/models/v1_machine_register_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     metal-api
 
     API to manage and control plane resources like machines, switches, operating system images, machine sizes, networks, IP addresses and more  # noqa: E501
 
-    OpenAPI spec version: v0.9.4
+    OpenAPI spec version: v0.9.5
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `metal_python-0.9.4/metal_python/models/v1_machine_reinstall_request.py` & `metal_python-0.9.5/metal_python/models/v1_machine_reinstall_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     metal-api
 
     API to manage and control plane resources like machines, switches, operating system images, machine sizes, networks, IP addresses and more  # noqa: E501
 
-    OpenAPI spec version: v0.9.4
+    OpenAPI spec version: v0.9.5
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `metal_python-0.9.4/metal_python/models/v1_machine_response.py` & `metal_python-0.9.5/metal_python/models/v1_machine_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     metal-api
 
     API to manage and control plane resources like machines, switches, operating system images, machine sizes, networks, IP addresses and more  # noqa: E501
 
-    OpenAPI spec version: v0.9.4
+    OpenAPI spec version: v0.9.5
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `metal_python-0.9.4/metal_python/models/v1_machine_state.py` & `metal_python-0.9.5/metal_python/models/v1_machine_state.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     metal-api
 
     API to manage and control plane resources like machines, switches, operating system images, machine sizes, networks, IP addresses and more  # noqa: E501
 
-    OpenAPI spec version: v0.9.4
+    OpenAPI spec version: v0.9.5
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `metal_python-0.9.4/metal_python/models/v1_meta.py` & `metal_python-0.9.5/metal_python/models/v1_meta.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     metal-api
 
     API to manage and control plane resources like machines, switches, operating system images, machine sizes, networks, IP addresses and more  # noqa: E501
 
-    OpenAPI spec version: v0.9.4
+    OpenAPI spec version: v0.9.5
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `metal_python-0.9.4/metal_python/models/v1_network_allocate_request.py` & `metal_python-0.9.5/metal_python/models/v1_network_allocate_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     metal-api
 
     API to manage and control plane resources like machines, switches, operating system images, machine sizes, networks, IP addresses and more  # noqa: E501
 
-    OpenAPI spec version: v0.9.4
+    OpenAPI spec version: v0.9.5
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `metal_python-0.9.4/metal_python/models/v1_network_create_request.py` & `metal_python-0.9.5/metal_python/models/v1_network_create_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     metal-api
 
     API to manage and control plane resources like machines, switches, operating system images, machine sizes, networks, IP addresses and more  # noqa: E501
 
-    OpenAPI spec version: v0.9.4
+    OpenAPI spec version: v0.9.5
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `metal_python-0.9.4/metal_python/models/v1_network_find_request.py` & `metal_python-0.9.5/metal_python/models/v1_network_find_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     metal-api
 
     API to manage and control plane resources like machines, switches, operating system images, machine sizes, networks, IP addresses and more  # noqa: E501
 
-    OpenAPI spec version: v0.9.4
+    OpenAPI spec version: v0.9.5
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `metal_python-0.9.4/metal_python/models/v1_network_response.py` & `metal_python-0.9.5/metal_python/models/v1_network_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     metal-api
 
     API to manage and control plane resources like machines, switches, operating system images, machine sizes, networks, IP addresses and more  # noqa: E501
 
-    OpenAPI spec version: v0.9.4
+    OpenAPI spec version: v0.9.5
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `metal_python-0.9.4/metal_python/models/v1_network_update_request.py` & `metal_python-0.9.5/metal_python/models/v1_network_update_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     metal-api
 
     API to manage and control plane resources like machines, switches, operating system images, machine sizes, networks, IP addresses and more  # noqa: E501
 
-    OpenAPI spec version: v0.9.4
+    OpenAPI spec version: v0.9.5
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `metal_python-0.9.4/metal_python/models/v1_network_usage.py` & `metal_python-0.9.5/metal_python/models/v1_network_usage.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     metal-api
 
     API to manage and control plane resources like machines, switches, operating system images, machine sizes, networks, IP addresses and more  # noqa: E501
 
-    OpenAPI spec version: v0.9.4
+    OpenAPI spec version: v0.9.5
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `metal_python-0.9.4/metal_python/models/v1_partition_boot_configuration.py` & `metal_python-0.9.5/metal_python/models/v1_partition_boot_configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     metal-api
 
     API to manage and control plane resources like machines, switches, operating system images, machine sizes, networks, IP addresses and more  # noqa: E501
 
-    OpenAPI spec version: v0.9.4
+    OpenAPI spec version: v0.9.5
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `metal_python-0.9.4/metal_python/models/v1_partition_capacity.py` & `metal_python-0.9.5/metal_python/models/v1_partition_capacity.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     metal-api
 
     API to manage and control plane resources like machines, switches, operating system images, machine sizes, networks, IP addresses and more  # noqa: E501
 
-    OpenAPI spec version: v0.9.4
+    OpenAPI spec version: v0.9.5
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `metal_python-0.9.4/metal_python/models/v1_partition_create_request.py` & `metal_python-0.9.5/metal_python/models/v1_partition_create_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     metal-api
 
     API to manage and control plane resources like machines, switches, operating system images, machine sizes, networks, IP addresses and more  # noqa: E501
 
-    OpenAPI spec version: v0.9.4
+    OpenAPI spec version: v0.9.5
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `metal_python-0.9.4/metal_python/models/v1_partition_response.py` & `metal_python-0.9.5/metal_python/models/v1_partition_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     metal-api
 
     API to manage and control plane resources like machines, switches, operating system images, machine sizes, networks, IP addresses and more  # noqa: E501
 
-    OpenAPI spec version: v0.9.4
+    OpenAPI spec version: v0.9.5
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `metal_python-0.9.4/metal_python/models/v1_partition_update_request.py` & `metal_python-0.9.5/metal_python/models/v1_partition_update_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     metal-api
 
     API to manage and control plane resources like machines, switches, operating system images, machine sizes, networks, IP addresses and more  # noqa: E501
 
-    OpenAPI spec version: v0.9.4
+    OpenAPI spec version: v0.9.5
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `metal_python-0.9.4/metal_python/models/v1_project_create_request.py` & `metal_python-0.9.5/metal_python/models/v1_project_create_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     metal-api
 
     API to manage and control plane resources like machines, switches, operating system images, machine sizes, networks, IP addresses and more  # noqa: E501
 
-    OpenAPI spec version: v0.9.4
+    OpenAPI spec version: v0.9.5
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `metal_python-0.9.4/metal_python/models/v1_project_find_request.py` & `metal_python-0.9.5/metal_python/models/v1_project_find_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     metal-api
 
     API to manage and control plane resources like machines, switches, operating system images, machine sizes, networks, IP addresses and more  # noqa: E501
 
-    OpenAPI spec version: v0.9.4
+    OpenAPI spec version: v0.9.5
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `metal_python-0.9.4/metal_python/models/v1_project_response.py` & `metal_python-0.9.5/metal_python/models/v1_project_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     metal-api
 
     API to manage and control plane resources like machines, switches, operating system images, machine sizes, networks, IP addresses and more  # noqa: E501
 
-    OpenAPI spec version: v0.9.4
+    OpenAPI spec version: v0.9.5
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `metal_python-0.9.4/metal_python/models/v1_project_update_request.py` & `metal_python-0.9.5/metal_python/models/v1_project_update_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     metal-api
 
     API to manage and control plane resources like machines, switches, operating system images, machine sizes, networks, IP addresses and more  # noqa: E501
 
-    OpenAPI spec version: v0.9.4
+    OpenAPI spec version: v0.9.5
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `metal_python-0.9.4/metal_python/models/v1_quota.py` & `metal_python-0.9.5/metal_python/models/v1_quota.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     metal-api
 
     API to manage and control plane resources like machines, switches, operating system images, machine sizes, networks, IP addresses and more  # noqa: E501
 
-    OpenAPI spec version: v0.9.4
+    OpenAPI spec version: v0.9.5
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `metal_python-0.9.4/metal_python/models/v1_quota_set.py` & `metal_python-0.9.5/metal_python/models/v1_quota_set.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     metal-api
 
     API to manage and control plane resources like machines, switches, operating system images, machine sizes, networks, IP addresses and more  # noqa: E501
 
-    OpenAPI spec version: v0.9.4
+    OpenAPI spec version: v0.9.5
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `metal_python-0.9.4/metal_python/models/v1_server_capacity.py` & `metal_python-0.9.5/metal_python/models/v1_server_capacity.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     metal-api
 
     API to manage and control plane resources like machines, switches, operating system images, machine sizes, networks, IP addresses and more  # noqa: E501
 
-    OpenAPI spec version: v0.9.4
+    OpenAPI spec version: v0.9.5
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `metal_python-0.9.4/metal_python/models/v1_size_constraint.py` & `metal_python-0.9.5/metal_python/models/v1_size_constraint.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     metal-api
 
     API to manage and control plane resources like machines, switches, operating system images, machine sizes, networks, IP addresses and more  # noqa: E501
 
-    OpenAPI spec version: v0.9.4
+    OpenAPI spec version: v0.9.5
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `metal_python-0.9.4/metal_python/models/v1_size_constraint_matching_log.py` & `metal_python-0.9.5/metal_python/models/v1_size_constraint_matching_log.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     metal-api
 
     API to manage and control plane resources like machines, switches, operating system images, machine sizes, networks, IP addresses and more  # noqa: E501
 
-    OpenAPI spec version: v0.9.4
+    OpenAPI spec version: v0.9.5
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `metal_python-0.9.4/metal_python/models/v1_size_create_request.py` & `metal_python-0.9.5/metal_python/models/v1_size_create_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     metal-api
 
     API to manage and control plane resources like machines, switches, operating system images, machine sizes, networks, IP addresses and more  # noqa: E501
 
-    OpenAPI spec version: v0.9.4
+    OpenAPI spec version: v0.9.5
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `metal_python-0.9.4/metal_python/models/v1_size_matching_log.py` & `metal_python-0.9.5/metal_python/models/v1_size_matching_log.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     metal-api
 
     API to manage and control plane resources like machines, switches, operating system images, machine sizes, networks, IP addresses and more  # noqa: E501
 
-    OpenAPI spec version: v0.9.4
+    OpenAPI spec version: v0.9.5
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `metal_python-0.9.4/metal_python/models/v1_size_response.py` & `metal_python-0.9.5/metal_python/models/v1_size_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     metal-api
 
     API to manage and control plane resources like machines, switches, operating system images, machine sizes, networks, IP addresses and more  # noqa: E501
 
-    OpenAPI spec version: v0.9.4
+    OpenAPI spec version: v0.9.5
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `metal_python-0.9.4/metal_python/models/v1_size_update_request.py` & `metal_python-0.9.5/metal_python/models/v1_size_update_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     metal-api
 
     API to manage and control plane resources like machines, switches, operating system images, machine sizes, networks, IP addresses and more  # noqa: E501
 
-    OpenAPI spec version: v0.9.4
+    OpenAPI spec version: v0.9.5
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `metal_python-0.9.4/metal_python/models/v1_switch_connection.py` & `metal_python-0.9.5/metal_python/models/v1_switch_connection.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     metal-api
 
     API to manage and control plane resources like machines, switches, operating system images, machine sizes, networks, IP addresses and more  # noqa: E501
 
-    OpenAPI spec version: v0.9.4
+    OpenAPI spec version: v0.9.5
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `metal_python-0.9.4/metal_python/models/v1_switch_nic.py` & `metal_python-0.9.5/metal_python/models/v1_switch_nic.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     metal-api
 
     API to manage and control plane resources like machines, switches, operating system images, machine sizes, networks, IP addresses and more  # noqa: E501
 
-    OpenAPI spec version: v0.9.4
+    OpenAPI spec version: v0.9.5
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `metal_python-0.9.4/metal_python/models/v1_switch_notify_request.py` & `metal_python-0.9.5/metal_python/models/v1_switch_notify_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     metal-api
 
     API to manage and control plane resources like machines, switches, operating system images, machine sizes, networks, IP addresses and more  # noqa: E501
 
-    OpenAPI spec version: v0.9.4
+    OpenAPI spec version: v0.9.5
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `metal_python-0.9.4/metal_python/models/v1_switch_register_request.py` & `metal_python-0.9.5/metal_python/models/v1_switch_register_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     metal-api
 
     API to manage and control plane resources like machines, switches, operating system images, machine sizes, networks, IP addresses and more  # noqa: E501
 
-    OpenAPI spec version: v0.9.4
+    OpenAPI spec version: v0.9.5
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `metal_python-0.9.4/metal_python/models/v1_switch_response.py` & `metal_python-0.9.5/metal_python/models/v1_switch_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     metal-api
 
     API to manage and control plane resources like machines, switches, operating system images, machine sizes, networks, IP addresses and more  # noqa: E501
 
-    OpenAPI spec version: v0.9.4
+    OpenAPI spec version: v0.9.5
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `metal_python-0.9.4/metal_python/models/v1_switch_sync.py` & `metal_python-0.9.5/metal_python/models/v1_switch_sync.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     metal-api
 
     API to manage and control plane resources like machines, switches, operating system images, machine sizes, networks, IP addresses and more  # noqa: E501
 
-    OpenAPI spec version: v0.9.4
+    OpenAPI spec version: v0.9.5
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `metal_python-0.9.4/metal_python/models/v1_switch_update_request.py` & `metal_python-0.9.5/metal_python/models/v1_switch_update_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     metal-api
 
     API to manage and control plane resources like machines, switches, operating system images, machine sizes, networks, IP addresses and more  # noqa: E501
 
-    OpenAPI spec version: v0.9.4
+    OpenAPI spec version: v0.9.5
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `metal_python-0.9.4/metal_python/rest.py` & `metal_python-0.9.5/metal_python/rest.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     metal-api
 
     API to manage and control plane resources like machines, switches, operating system images, machine sizes, networks, IP addresses and more  # noqa: E501
 
-    OpenAPI spec version: v0.9.4
+    OpenAPI spec version: v0.9.5
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `metal_python-0.9.4/metal_python.egg-info/PKG-INFO` & `metal_python-0.9.5/metal_python.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metal-python
-Version: 0.9.4
+Version: 0.9.5
 Summary: Python API client for metal-api
 Home-page: https://github.com/metal-stack/metal-python
 Author: metal-stack authors
 License: MIT
 Description: UNKNOWN
 Keywords: metal-stack,metal-api,swagger,swagger-client
 Platform: UNKNOWN
```

### Comparing `metal_python-0.9.4/metal_python.egg-info/SOURCES.txt` & `metal_python-0.9.5/metal_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `metal_python-0.9.4/setup.py` & `metal_python-0.9.5/setup.py`

 * *Files identical despite different names*

### Comparing `metal_python-0.9.4/test/test_firewall_api.py` & `metal_python-0.9.5/test/test_firewall_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     metal-api
 
     API to manage and control plane resources like machines, switches, operating system images, machine sizes, networks, IP addresses and more  # noqa: E501
 
-    OpenAPI spec version: v0.9.4
+    OpenAPI spec version: v0.9.5
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `metal_python-0.9.4/test/test_health_api.py` & `metal_python-0.9.5/test/test_health_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     metal-api
 
     API to manage and control plane resources like machines, switches, operating system images, machine sizes, networks, IP addresses and more  # noqa: E501
 
-    OpenAPI spec version: v0.9.4
+    OpenAPI spec version: v0.9.5
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `metal_python-0.9.4/test/test_httperrors_http_error_response.py` & `metal_python-0.9.5/test/test_httperrors_http_error_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     metal-api
 
     API to manage and control plane resources like machines, switches, operating system images, machine sizes, networks, IP addresses and more  # noqa: E501
 
-    OpenAPI spec version: v0.9.4
+    OpenAPI spec version: v0.9.5
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `metal_python-0.9.4/test/test_image_api.py` & `metal_python-0.9.5/test/test_image_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     metal-api
 
     API to manage and control plane resources like machines, switches, operating system images, machine sizes, networks, IP addresses and more  # noqa: E501
 
-    OpenAPI spec version: v0.9.4
+    OpenAPI spec version: v0.9.5
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `metal_python-0.9.4/test/test_ip_api.py` & `metal_python-0.9.5/test/test_ip_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     metal-api
 
     API to manage and control plane resources like machines, switches, operating system images, machine sizes, networks, IP addresses and more  # noqa: E501
 
-    OpenAPI spec version: v0.9.4
+    OpenAPI spec version: v0.9.5
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `metal_python-0.9.4/test/test_machine_api.py` & `metal_python-0.9.5/test/test_machine_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     metal-api
 
     API to manage and control plane resources like machines, switches, operating system images, machine sizes, networks, IP addresses and more  # noqa: E501
 
-    OpenAPI spec version: v0.9.4
+    OpenAPI spec version: v0.9.5
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `metal_python-0.9.4/test/test_network_api.py` & `metal_python-0.9.5/test/test_network_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     metal-api
 
     API to manage and control plane resources like machines, switches, operating system images, machine sizes, networks, IP addresses and more  # noqa: E501
 
-    OpenAPI spec version: v0.9.4
+    OpenAPI spec version: v0.9.5
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `metal_python-0.9.4/test/test_partition_api.py` & `metal_python-0.9.5/test/test_partition_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     metal-api
 
     API to manage and control plane resources like machines, switches, operating system images, machine sizes, networks, IP addresses and more  # noqa: E501
 
-    OpenAPI spec version: v0.9.4
+    OpenAPI spec version: v0.9.5
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `metal_python-0.9.4/test/test_project_api.py` & `metal_python-0.9.5/test/test_project_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     metal-api
 
     API to manage and control plane resources like machines, switches, operating system images, machine sizes, networks, IP addresses and more  # noqa: E501
 
-    OpenAPI spec version: v0.9.4
+    OpenAPI spec version: v0.9.5
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `metal_python-0.9.4/test/test_rest_status.py` & `metal_python-0.9.5/test/test_rest_status.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     metal-api
 
     API to manage and control plane resources like machines, switches, operating system images, machine sizes, networks, IP addresses and more  # noqa: E501
 
-    OpenAPI spec version: v0.9.4
+    OpenAPI spec version: v0.9.5
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `metal_python-0.9.4/test/test_rest_version.py` & `metal_python-0.9.5/test/test_rest_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     metal-api
 
     API to manage and control plane resources like machines, switches, operating system images, machine sizes, networks, IP addresses and more  # noqa: E501
 
-    OpenAPI spec version: v0.9.4
+    OpenAPI spec version: v0.9.5
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `metal_python-0.9.4/test/test_size_api.py` & `metal_python-0.9.5/test/test_size_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     metal-api
 
     API to manage and control plane resources like machines, switches, operating system images, machine sizes, networks, IP addresses and more  # noqa: E501
 
-    OpenAPI spec version: v0.9.4
+    OpenAPI spec version: v0.9.5
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `metal_python-0.9.4/test/test_switch_api.py` & `metal_python-0.9.5/test/test_switch_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     metal-api
 
     API to manage and control plane resources like machines, switches, operating system images, machine sizes, networks, IP addresses and more  # noqa: E501
 
-    OpenAPI spec version: v0.9.4
+    OpenAPI spec version: v0.9.5
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `metal_python-0.9.4/test/test_v1_bgp_filter.py` & `metal_python-0.9.5/test/test_v1_bgp_filter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     metal-api
 
     API to manage and control plane resources like machines, switches, operating system images, machine sizes, networks, IP addresses and more  # noqa: E501
 
-    OpenAPI spec version: v0.9.4
+    OpenAPI spec version: v0.9.5
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `metal_python-0.9.4/test/test_v1_boot_info.py` & `metal_python-0.9.5/test/test_v1_boot_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     metal-api
 
     API to manage and control plane resources like machines, switches, operating system images, machine sizes, networks, IP addresses and more  # noqa: E501
 
-    OpenAPI spec version: v0.9.4
+    OpenAPI spec version: v0.9.5
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `metal_python-0.9.4/test/test_v1_chassis_identify_led_state.py` & `metal_python-0.9.5/test/test_v1_chassis_identify_led_state.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     metal-api
 
     API to manage and control plane resources like machines, switches, operating system images, machine sizes, networks, IP addresses and more  # noqa: E501
 
-    OpenAPI spec version: v0.9.4
+    OpenAPI spec version: v0.9.5
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `metal_python-0.9.4/test/test_v1_empty_body.py` & `metal_python-0.9.5/test/test_v1_empty_body.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     metal-api
 
     API to manage and control plane resources like machines, switches, operating system images, machine sizes, networks, IP addresses and more  # noqa: E501
 
-    OpenAPI spec version: v0.9.4
+    OpenAPI spec version: v0.9.5
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `metal_python-0.9.4/test/test_v1_firewall_create_request.py` & `metal_python-0.9.5/test/test_v1_firewall_create_request.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     metal-api
 
     API to manage and control plane resources like machines, switches, operating system images, machine sizes, networks, IP addresses and more  # noqa: E501
 
-    OpenAPI spec version: v0.9.4
+    OpenAPI spec version: v0.9.5
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `metal_python-0.9.4/test/test_v1_firewall_find_request.py` & `metal_python-0.9.5/test/test_v1_firewall_find_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     metal-api
 
     API to manage and control plane resources like machines, switches, operating system images, machine sizes, networks, IP addresses and more  # noqa: E501
 
-    OpenAPI spec version: v0.9.4
+    OpenAPI spec version: v0.9.5
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `metal_python-0.9.4/test/test_v1_firewall_response.py` & `metal_python-0.9.5/test/test_v1_firewall_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     metal-api
 
     API to manage and control plane resources like machines, switches, operating system images, machine sizes, networks, IP addresses and more  # noqa: E501
 
-    OpenAPI spec version: v0.9.4
+    OpenAPI spec version: v0.9.5
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `metal_python-0.9.4/test/test_v1_image_create_request.py` & `metal_python-0.9.5/test/test_v1_image_create_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     metal-api
 
     API to manage and control plane resources like machines, switches, operating system images, machine sizes, networks, IP addresses and more  # noqa: E501
 
-    OpenAPI spec version: v0.9.4
+    OpenAPI spec version: v0.9.5
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `metal_python-0.9.4/test/test_v1_image_response.py` & `metal_python-0.9.5/test/test_v1_image_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     metal-api
 
     API to manage and control plane resources like machines, switches, operating system images, machine sizes, networks, IP addresses and more  # noqa: E501
 
-    OpenAPI spec version: v0.9.4
+    OpenAPI spec version: v0.9.5
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `metal_python-0.9.4/test/test_v1_image_update_request.py` & `metal_python-0.9.5/test/test_v1_image_update_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     metal-api
 
     API to manage and control plane resources like machines, switches, operating system images, machine sizes, networks, IP addresses and more  # noqa: E501
 
-    OpenAPI spec version: v0.9.4
+    OpenAPI spec version: v0.9.5
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `metal_python-0.9.4/test/test_v1_ip_allocate_request.py` & `metal_python-0.9.5/test/test_v1_ip_allocate_request.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     metal-api
 
     API to manage and control plane resources like machines, switches, operating system images, machine sizes, networks, IP addresses and more  # noqa: E501
 
-    OpenAPI spec version: v0.9.4
+    OpenAPI spec version: v0.9.5
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `metal_python-0.9.4/test/test_v1_ip_find_request.py` & `metal_python-0.9.5/test/test_v1_ip_find_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     metal-api
 
     API to manage and control plane resources like machines, switches, operating system images, machine sizes, networks, IP addresses and more  # noqa: E501
 
-    OpenAPI spec version: v0.9.4
+    OpenAPI spec version: v0.9.5
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `metal_python-0.9.4/test/test_v1_ip_response.py` & `metal_python-0.9.5/test/test_v1_ip_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     metal-api
 
     API to manage and control plane resources like machines, switches, operating system images, machine sizes, networks, IP addresses and more  # noqa: E501
 
-    OpenAPI spec version: v0.9.4
+    OpenAPI spec version: v0.9.5
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `metal_python-0.9.4/test/test_v1_ip_update_request.py` & `metal_python-0.9.5/test/test_v1_ip_update_request.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     metal-api
 
     API to manage and control plane resources like machines, switches, operating system images, machine sizes, networks, IP addresses and more  # noqa: E501
 
-    OpenAPI spec version: v0.9.4
+    OpenAPI spec version: v0.9.5
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `metal_python-0.9.4/test/test_v1_machine_abort_reinstall_request.py` & `metal_python-0.9.5/test/test_v1_machine_abort_reinstall_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     metal-api
 
     API to manage and control plane resources like machines, switches, operating system images, machine sizes, networks, IP addresses and more  # noqa: E501
 
-    OpenAPI spec version: v0.9.4
+    OpenAPI spec version: v0.9.5
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `metal_python-0.9.4/test/test_v1_machine_allocate_request.py` & `metal_python-0.9.5/test/test_v1_machine_allocate_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     metal-api
 
     API to manage and control plane resources like machines, switches, operating system images, machine sizes, networks, IP addresses and more  # noqa: E501
 
-    OpenAPI spec version: v0.9.4
+    OpenAPI spec version: v0.9.5
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `metal_python-0.9.4/test/test_v1_machine_allocation.py` & `metal_python-0.9.5/test/test_v1_machine_allocation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     metal-api
 
     API to manage and control plane resources like machines, switches, operating system images, machine sizes, networks, IP addresses and more  # noqa: E501
 
-    OpenAPI spec version: v0.9.4
+    OpenAPI spec version: v0.9.5
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `metal_python-0.9.4/test/test_v1_machine_allocation_network.py` & `metal_python-0.9.5/test/test_v1_machine_allocation_network.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     metal-api
 
     API to manage and control plane resources like machines, switches, operating system images, machine sizes, networks, IP addresses and more  # noqa: E501
 
-    OpenAPI spec version: v0.9.4
+    OpenAPI spec version: v0.9.5
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `metal_python-0.9.4/test/test_v1_machine_bios.py` & `metal_python-0.9.5/test/test_v1_machine_bios.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     metal-api
 
     API to manage and control plane resources like machines, switches, operating system images, machine sizes, networks, IP addresses and more  # noqa: E501
 
-    OpenAPI spec version: v0.9.4
+    OpenAPI spec version: v0.9.5
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `metal_python-0.9.4/test/test_v1_machine_block_device.py` & `metal_python-0.9.5/test/test_v1_machine_block_device.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     metal-api
 
     API to manage and control plane resources like machines, switches, operating system images, machine sizes, networks, IP addresses and more  # noqa: E501
 
-    OpenAPI spec version: v0.9.4
+    OpenAPI spec version: v0.9.5
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `metal_python-0.9.4/test/test_v1_machine_disk_partition.py` & `metal_python-0.9.5/test/test_v1_machine_disk_partition.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     metal-api
 
     API to manage and control plane resources like machines, switches, operating system images, machine sizes, networks, IP addresses and more  # noqa: E501
 
-    OpenAPI spec version: v0.9.4
+    OpenAPI spec version: v0.9.5
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `metal_python-0.9.4/test/test_v1_machine_finalize_allocation_request.py` & `metal_python-0.9.5/test/test_v1_machine_finalize_allocation_request.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     metal-api
 
     API to manage and control plane resources like machines, switches, operating system images, machine sizes, networks, IP addresses and more  # noqa: E501
 
-    OpenAPI spec version: v0.9.4
+    OpenAPI spec version: v0.9.5
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `metal_python-0.9.4/test/test_v1_machine_find_request.py` & `metal_python-0.9.5/test/test_v1_project_find_request.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 # coding: utf-8
 
 """
     metal-api
 
     API to manage and control plane resources like machines, switches, operating system images, machine sizes, networks, IP addresses and more  # noqa: E501
 
-    OpenAPI spec version: v0.9.4
+    OpenAPI spec version: v0.9.5
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
 
 import unittest
 
 import metal_python
-from metal_python.models.v1_machine_find_request import V1MachineFindRequest  # noqa: E501
+from metal_python.models.v1_project_find_request import V1ProjectFindRequest  # noqa: E501
 from metal_python.rest import ApiException
 
 
-class TestV1MachineFindRequest(unittest.TestCase):
-    """V1MachineFindRequest unit test stubs"""
+class TestV1ProjectFindRequest(unittest.TestCase):
+    """V1ProjectFindRequest unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testV1MachineFindRequest(self):
-        """Test V1MachineFindRequest"""
+    def testV1ProjectFindRequest(self):
+        """Test V1ProjectFindRequest"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = metal_python.models.v1_machine_find_request.V1MachineFindRequest()  # noqa: E501
+        # model = metal_python.models.v1_project_find_request.V1ProjectFindRequest()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `metal_python-0.9.4/test/test_v1_machine_fru.py` & `metal_python-0.9.5/test/test_v1_machine_fru.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     metal-api
 
     API to manage and control plane resources like machines, switches, operating system images, machine sizes, networks, IP addresses and more  # noqa: E501
 
-    OpenAPI spec version: v0.9.4
+    OpenAPI spec version: v0.9.5
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `metal_python-0.9.4/test/test_v1_machine_hardware.py` & `metal_python-0.9.5/test/test_v1_machine_hardware.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     metal-api
 
     API to manage and control plane resources like machines, switches, operating system images, machine sizes, networks, IP addresses and more  # noqa: E501
 
-    OpenAPI spec version: v0.9.4
+    OpenAPI spec version: v0.9.5
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `metal_python-0.9.4/test/test_v1_machine_hardware_extended.py` & `metal_python-0.9.5/test/test_v1_machine_hardware_extended.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     metal-api
 
     API to manage and control plane resources like machines, switches, operating system images, machine sizes, networks, IP addresses and more  # noqa: E501
 
-    OpenAPI spec version: v0.9.4
+    OpenAPI spec version: v0.9.5
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `metal_python-0.9.4/test/test_v1_machine_ipmi.py` & `metal_python-0.9.5/test/test_v1_machine_ipmi.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     metal-api
 
     API to manage and control plane resources like machines, switches, operating system images, machine sizes, networks, IP addresses and more  # noqa: E501
 
-    OpenAPI spec version: v0.9.4
+    OpenAPI spec version: v0.9.5
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `metal_python-0.9.4/test/test_v1_machine_ipmi_report.py` & `metal_python-0.9.5/test/test_v1_machine_ipmi_report.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     metal-api
 
     API to manage and control plane resources like machines, switches, operating system images, machine sizes, networks, IP addresses and more  # noqa: E501
 
-    OpenAPI spec version: v0.9.4
+    OpenAPI spec version: v0.9.5
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `metal_python-0.9.4/test/test_v1_machine_ipmi_report_response.py` & `metal_python-0.9.5/test/test_v1_machine_ipmi_report_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     metal-api
 
     API to manage and control plane resources like machines, switches, operating system images, machine sizes, networks, IP addresses and more  # noqa: E501
 
-    OpenAPI spec version: v0.9.4
+    OpenAPI spec version: v0.9.5
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `metal_python-0.9.4/test/test_v1_machine_ipmi_response.py` & `metal_python-0.9.5/test/test_v1_machine_ipmi_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     metal-api
 
     API to manage and control plane resources like machines, switches, operating system images, machine sizes, networks, IP addresses and more  # noqa: E501
 
-    OpenAPI spec version: v0.9.4
+    OpenAPI spec version: v0.9.5
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `metal_python-0.9.4/test/test_v1_machine_network.py` & `metal_python-0.9.5/test/test_v1_machine_network.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     metal-api
 
     API to manage and control plane resources like machines, switches, operating system images, machine sizes, networks, IP addresses and more  # noqa: E501
 
-    OpenAPI spec version: v0.9.4
+    OpenAPI spec version: v0.9.5
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `metal_python-0.9.4/test/test_v1_machine_nic.py` & `metal_python-0.9.5/test/test_v1_machine_nic.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     metal-api
 
     API to manage and control plane resources like machines, switches, operating system images, machine sizes, networks, IP addresses and more  # noqa: E501
 
-    OpenAPI spec version: v0.9.4
+    OpenAPI spec version: v0.9.5
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `metal_python-0.9.4/test/test_v1_machine_nic_extended.py` & `metal_python-0.9.5/test/test_v1_machine_nic_extended.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     metal-api
 
     API to manage and control plane resources like machines, switches, operating system images, machine sizes, networks, IP addresses and more  # noqa: E501
 
-    OpenAPI spec version: v0.9.4
+    OpenAPI spec version: v0.9.5
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `metal_python-0.9.4/test/test_v1_machine_provisioning_event.py` & `metal_python-0.9.5/test/test_v1_machine_provisioning_event.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     metal-api
 
     API to manage and control plane resources like machines, switches, operating system images, machine sizes, networks, IP addresses and more  # noqa: E501
 
-    OpenAPI spec version: v0.9.4
+    OpenAPI spec version: v0.9.5
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `metal_python-0.9.4/test/test_v1_machine_recent_provisioning_events.py` & `metal_python-0.9.5/test/test_v1_machine_recent_provisioning_events.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     metal-api
 
     API to manage and control plane resources like machines, switches, operating system images, machine sizes, networks, IP addresses and more  # noqa: E501
 
-    OpenAPI spec version: v0.9.4
+    OpenAPI spec version: v0.9.5
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `metal_python-0.9.4/test/test_v1_machine_register_request.py` & `metal_python-0.9.5/test/test_v1_machine_register_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     metal-api
 
     API to manage and control plane resources like machines, switches, operating system images, machine sizes, networks, IP addresses and more  # noqa: E501
 
-    OpenAPI spec version: v0.9.4
+    OpenAPI spec version: v0.9.5
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `metal_python-0.9.4/test/test_v1_machine_reinstall_request.py` & `metal_python-0.9.5/test/test_v1_machine_reinstall_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     metal-api
 
     API to manage and control plane resources like machines, switches, operating system images, machine sizes, networks, IP addresses and more  # noqa: E501
 
-    OpenAPI spec version: v0.9.4
+    OpenAPI spec version: v0.9.5
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `metal_python-0.9.4/test/test_v1_machine_response.py` & `metal_python-0.9.5/test/test_v1_machine_response.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     metal-api
 
     API to manage and control plane resources like machines, switches, operating system images, machine sizes, networks, IP addresses and more  # noqa: E501
 
-    OpenAPI spec version: v0.9.4
+    OpenAPI spec version: v0.9.5
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `metal_python-0.9.4/test/test_v1_machine_state.py` & `metal_python-0.9.5/test/test_v1_machine_state.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     metal-api
 
     API to manage and control plane resources like machines, switches, operating system images, machine sizes, networks, IP addresses and more  # noqa: E501
 
-    OpenAPI spec version: v0.9.4
+    OpenAPI spec version: v0.9.5
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `metal_python-0.9.4/test/test_v1_meta.py` & `metal_python-0.9.5/test/test_v1_meta.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     metal-api
 
     API to manage and control plane resources like machines, switches, operating system images, machine sizes, networks, IP addresses and more  # noqa: E501
 
-    OpenAPI spec version: v0.9.4
+    OpenAPI spec version: v0.9.5
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `metal_python-0.9.4/test/test_v1_network_allocate_request.py` & `metal_python-0.9.5/test/test_v1_network_allocate_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     metal-api
 
     API to manage and control plane resources like machines, switches, operating system images, machine sizes, networks, IP addresses and more  # noqa: E501
 
-    OpenAPI spec version: v0.9.4
+    OpenAPI spec version: v0.9.5
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `metal_python-0.9.4/test/test_v1_network_create_request.py` & `metal_python-0.9.5/test/test_v1_network_create_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     metal-api
 
     API to manage and control plane resources like machines, switches, operating system images, machine sizes, networks, IP addresses and more  # noqa: E501
 
-    OpenAPI spec version: v0.9.4
+    OpenAPI spec version: v0.9.5
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `metal_python-0.9.4/test/test_v1_network_find_request.py` & `metal_python-0.9.5/test/test_v1_network_find_request.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     metal-api
 
     API to manage and control plane resources like machines, switches, operating system images, machine sizes, networks, IP addresses and more  # noqa: E501
 
-    OpenAPI spec version: v0.9.4
+    OpenAPI spec version: v0.9.5
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `metal_python-0.9.4/test/test_v1_network_response.py` & `metal_python-0.9.5/test/test_v1_network_response.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     metal-api
 
     API to manage and control plane resources like machines, switches, operating system images, machine sizes, networks, IP addresses and more  # noqa: E501
 
-    OpenAPI spec version: v0.9.4
+    OpenAPI spec version: v0.9.5
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `metal_python-0.9.4/test/test_v1_network_update_request.py` & `metal_python-0.9.5/test/test_v1_network_update_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     metal-api
 
     API to manage and control plane resources like machines, switches, operating system images, machine sizes, networks, IP addresses and more  # noqa: E501
 
-    OpenAPI spec version: v0.9.4
+    OpenAPI spec version: v0.9.5
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `metal_python-0.9.4/test/test_v1_network_usage.py` & `metal_python-0.9.5/test/test_v1_network_usage.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     metal-api
 
     API to manage and control plane resources like machines, switches, operating system images, machine sizes, networks, IP addresses and more  # noqa: E501
 
-    OpenAPI spec version: v0.9.4
+    OpenAPI spec version: v0.9.5
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `metal_python-0.9.4/test/test_v1_partition_boot_configuration.py` & `metal_python-0.9.5/test/test_v1_partition_boot_configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     metal-api
 
     API to manage and control plane resources like machines, switches, operating system images, machine sizes, networks, IP addresses and more  # noqa: E501
 
-    OpenAPI spec version: v0.9.4
+    OpenAPI spec version: v0.9.5
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `metal_python-0.9.4/test/test_v1_partition_capacity.py` & `metal_python-0.9.5/test/test_v1_partition_capacity.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     metal-api
 
     API to manage and control plane resources like machines, switches, operating system images, machine sizes, networks, IP addresses and more  # noqa: E501
 
-    OpenAPI spec version: v0.9.4
+    OpenAPI spec version: v0.9.5
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `metal_python-0.9.4/test/test_v1_partition_create_request.py` & `metal_python-0.9.5/test/test_v1_partition_create_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     metal-api
 
     API to manage and control plane resources like machines, switches, operating system images, machine sizes, networks, IP addresses and more  # noqa: E501
 
-    OpenAPI spec version: v0.9.4
+    OpenAPI spec version: v0.9.5
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `metal_python-0.9.4/test/test_v1_partition_response.py` & `metal_python-0.9.5/test/test_v1_partition_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     metal-api
 
     API to manage and control plane resources like machines, switches, operating system images, machine sizes, networks, IP addresses and more  # noqa: E501
 
-    OpenAPI spec version: v0.9.4
+    OpenAPI spec version: v0.9.5
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `metal_python-0.9.4/test/test_v1_partition_update_request.py` & `metal_python-0.9.5/test/test_v1_partition_update_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     metal-api
 
     API to manage and control plane resources like machines, switches, operating system images, machine sizes, networks, IP addresses and more  # noqa: E501
 
-    OpenAPI spec version: v0.9.4
+    OpenAPI spec version: v0.9.5
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `metal_python-0.9.4/test/test_v1_project_create_request.py` & `metal_python-0.9.5/test/test_v1_project_create_request.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     metal-api
 
     API to manage and control plane resources like machines, switches, operating system images, machine sizes, networks, IP addresses and more  # noqa: E501
 
-    OpenAPI spec version: v0.9.4
+    OpenAPI spec version: v0.9.5
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `metal_python-0.9.4/test/test_v1_project_find_request.py` & `metal_python-0.9.5/test/test_v1_project_update_request.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 # coding: utf-8
 
 """
     metal-api
 
     API to manage and control plane resources like machines, switches, operating system images, machine sizes, networks, IP addresses and more  # noqa: E501
 
-    OpenAPI spec version: v0.9.4
+    OpenAPI spec version: v0.9.5
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
 
 import unittest
 
 import metal_python
-from metal_python.models.v1_project_find_request import V1ProjectFindRequest  # noqa: E501
+from metal_python.models.v1_project_update_request import V1ProjectUpdateRequest  # noqa: E501
 from metal_python.rest import ApiException
 
 
-class TestV1ProjectFindRequest(unittest.TestCase):
-    """V1ProjectFindRequest unit test stubs"""
+class TestV1ProjectUpdateRequest(unittest.TestCase):
+    """V1ProjectUpdateRequest unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testV1ProjectFindRequest(self):
-        """Test V1ProjectFindRequest"""
+    def testV1ProjectUpdateRequest(self):
+        """Test V1ProjectUpdateRequest"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = metal_python.models.v1_project_find_request.V1ProjectFindRequest()  # noqa: E501
+        # model = metal_python.models.v1_project_update_request.V1ProjectUpdateRequest()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `metal_python-0.9.4/test/test_v1_project_response.py` & `metal_python-0.9.5/test/test_v1_project_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     metal-api
 
     API to manage and control plane resources like machines, switches, operating system images, machine sizes, networks, IP addresses and more  # noqa: E501
 
-    OpenAPI spec version: v0.9.4
+    OpenAPI spec version: v0.9.5
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `metal_python-0.9.4/test/test_v1_project_update_request.py` & `metal_python-0.9.5/test/test_v1_switch_update_request.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 # coding: utf-8
 
 """
     metal-api
 
     API to manage and control plane resources like machines, switches, operating system images, machine sizes, networks, IP addresses and more  # noqa: E501
 
-    OpenAPI spec version: v0.9.4
+    OpenAPI spec version: v0.9.5
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
 
 import unittest
 
 import metal_python
-from metal_python.models.v1_project_update_request import V1ProjectUpdateRequest  # noqa: E501
+from metal_python.models.v1_switch_update_request import V1SwitchUpdateRequest  # noqa: E501
 from metal_python.rest import ApiException
 
 
-class TestV1ProjectUpdateRequest(unittest.TestCase):
-    """V1ProjectUpdateRequest unit test stubs"""
+class TestV1SwitchUpdateRequest(unittest.TestCase):
+    """V1SwitchUpdateRequest unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testV1ProjectUpdateRequest(self):
-        """Test V1ProjectUpdateRequest"""
+    def testV1SwitchUpdateRequest(self):
+        """Test V1SwitchUpdateRequest"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = metal_python.models.v1_project_update_request.V1ProjectUpdateRequest()  # noqa: E501
+        # model = metal_python.models.v1_switch_update_request.V1SwitchUpdateRequest()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `metal_python-0.9.4/test/test_v1_quota.py` & `metal_python-0.9.5/test/test_v1_quota_set.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 # coding: utf-8
 
 """
     metal-api
 
     API to manage and control plane resources like machines, switches, operating system images, machine sizes, networks, IP addresses and more  # noqa: E501
 
-    OpenAPI spec version: v0.9.4
+    OpenAPI spec version: v0.9.5
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
 
 import unittest
 
 import metal_python
-from metal_python.models.v1_quota import V1Quota  # noqa: E501
+from metal_python.models.v1_quota_set import V1QuotaSet  # noqa: E501
 from metal_python.rest import ApiException
 
 
-class TestV1Quota(unittest.TestCase):
-    """V1Quota unit test stubs"""
+class TestV1QuotaSet(unittest.TestCase):
+    """V1QuotaSet unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testV1Quota(self):
-        """Test V1Quota"""
+    def testV1QuotaSet(self):
+        """Test V1QuotaSet"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = metal_python.models.v1_quota.V1Quota()  # noqa: E501
+        # model = metal_python.models.v1_quota_set.V1QuotaSet()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `metal_python-0.9.4/test/test_v1_quota_set.py` & `metal_python-0.9.5/test/test_v1_switch_nic.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 # coding: utf-8
 
 """
     metal-api
 
     API to manage and control plane resources like machines, switches, operating system images, machine sizes, networks, IP addresses and more  # noqa: E501
 
-    OpenAPI spec version: v0.9.4
+    OpenAPI spec version: v0.9.5
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
 
 import unittest
 
 import metal_python
-from metal_python.models.v1_quota_set import V1QuotaSet  # noqa: E501
+from metal_python.models.v1_switch_nic import V1SwitchNic  # noqa: E501
 from metal_python.rest import ApiException
 
 
-class TestV1QuotaSet(unittest.TestCase):
-    """V1QuotaSet unit test stubs"""
+class TestV1SwitchNic(unittest.TestCase):
+    """V1SwitchNic unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testV1QuotaSet(self):
-        """Test V1QuotaSet"""
+    def testV1SwitchNic(self):
+        """Test V1SwitchNic"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = metal_python.models.v1_quota_set.V1QuotaSet()  # noqa: E501
+        # model = metal_python.models.v1_switch_nic.V1SwitchNic()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `metal_python-0.9.4/test/test_v1_server_capacity.py` & `metal_python-0.9.5/test/test_v1_server_capacity.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     metal-api
 
     API to manage and control plane resources like machines, switches, operating system images, machine sizes, networks, IP addresses and more  # noqa: E501
 
-    OpenAPI spec version: v0.9.4
+    OpenAPI spec version: v0.9.5
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `metal_python-0.9.4/test/test_v1_size_constraint.py` & `metal_python-0.9.5/test/test_v1_size_constraint.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     metal-api
 
     API to manage and control plane resources like machines, switches, operating system images, machine sizes, networks, IP addresses and more  # noqa: E501
 
-    OpenAPI spec version: v0.9.4
+    OpenAPI spec version: v0.9.5
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `metal_python-0.9.4/test/test_v1_size_constraint_matching_log.py` & `metal_python-0.9.5/test/test_v1_size_constraint_matching_log.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     metal-api
 
     API to manage and control plane resources like machines, switches, operating system images, machine sizes, networks, IP addresses and more  # noqa: E501
 
-    OpenAPI spec version: v0.9.4
+    OpenAPI spec version: v0.9.5
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `metal_python-0.9.4/test/test_v1_size_create_request.py` & `metal_python-0.9.5/test/test_v1_size_create_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     metal-api
 
     API to manage and control plane resources like machines, switches, operating system images, machine sizes, networks, IP addresses and more  # noqa: E501
 
-    OpenAPI spec version: v0.9.4
+    OpenAPI spec version: v0.9.5
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `metal_python-0.9.4/test/test_v1_size_matching_log.py` & `metal_python-0.9.5/test/test_v1_size_matching_log.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     metal-api
 
     API to manage and control plane resources like machines, switches, operating system images, machine sizes, networks, IP addresses and more  # noqa: E501
 
-    OpenAPI spec version: v0.9.4
+    OpenAPI spec version: v0.9.5
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `metal_python-0.9.4/test/test_v1_size_response.py` & `metal_python-0.9.5/test/test_v1_size_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     metal-api
 
     API to manage and control plane resources like machines, switches, operating system images, machine sizes, networks, IP addresses and more  # noqa: E501
 
-    OpenAPI spec version: v0.9.4
+    OpenAPI spec version: v0.9.5
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `metal_python-0.9.4/test/test_v1_size_update_request.py` & `metal_python-0.9.5/test/test_v1_size_update_request.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     metal-api
 
     API to manage and control plane resources like machines, switches, operating system images, machine sizes, networks, IP addresses and more  # noqa: E501
 
-    OpenAPI spec version: v0.9.4
+    OpenAPI spec version: v0.9.5
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `metal_python-0.9.4/test/test_v1_switch_connection.py` & `metal_python-0.9.5/test/test_v1_switch_connection.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     metal-api
 
     API to manage and control plane resources like machines, switches, operating system images, machine sizes, networks, IP addresses and more  # noqa: E501
 
-    OpenAPI spec version: v0.9.4
+    OpenAPI spec version: v0.9.5
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `metal_python-0.9.4/test/test_v1_switch_nic.py` & `metal_python-0.9.5/test/test_v1_switch_sync.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 # coding: utf-8
 
 """
     metal-api
 
     API to manage and control plane resources like machines, switches, operating system images, machine sizes, networks, IP addresses and more  # noqa: E501
 
-    OpenAPI spec version: v0.9.4
+    OpenAPI spec version: v0.9.5
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
 
 import unittest
 
 import metal_python
-from metal_python.models.v1_switch_nic import V1SwitchNic  # noqa: E501
+from metal_python.models.v1_switch_sync import V1SwitchSync  # noqa: E501
 from metal_python.rest import ApiException
 
 
-class TestV1SwitchNic(unittest.TestCase):
-    """V1SwitchNic unit test stubs"""
+class TestV1SwitchSync(unittest.TestCase):
+    """V1SwitchSync unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testV1SwitchNic(self):
-        """Test V1SwitchNic"""
+    def testV1SwitchSync(self):
+        """Test V1SwitchSync"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = metal_python.models.v1_switch_nic.V1SwitchNic()  # noqa: E501
+        # model = metal_python.models.v1_switch_sync.V1SwitchSync()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `metal_python-0.9.4/test/test_v1_switch_notify_request.py` & `metal_python-0.9.5/test/test_v1_switch_notify_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     metal-api
 
     API to manage and control plane resources like machines, switches, operating system images, machine sizes, networks, IP addresses and more  # noqa: E501
 
-    OpenAPI spec version: v0.9.4
+    OpenAPI spec version: v0.9.5
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `metal_python-0.9.4/test/test_v1_switch_register_request.py` & `metal_python-0.9.5/test/test_v1_switch_register_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     metal-api
 
     API to manage and control plane resources like machines, switches, operating system images, machine sizes, networks, IP addresses and more  # noqa: E501
 
-    OpenAPI spec version: v0.9.4
+    OpenAPI spec version: v0.9.5
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `metal_python-0.9.4/test/test_v1_switch_response.py` & `metal_python-0.9.5/test/test_v1_switch_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     metal-api
 
     API to manage and control plane resources like machines, switches, operating system images, machine sizes, networks, IP addresses and more  # noqa: E501
 
-    OpenAPI spec version: v0.9.4
+    OpenAPI spec version: v0.9.5
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `metal_python-0.9.4/test/test_version_api.py` & `metal_python-0.9.5/test/test_version_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     metal-api
 
     API to manage and control plane resources like machines, switches, operating system images, machine sizes, networks, IP addresses and more  # noqa: E501
 
-    OpenAPI spec version: v0.9.4
+    OpenAPI spec version: v0.9.5
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

