# Comparing `tmp/python-manilaclient-4.4.0.tar.gz` & `tmp/python-manilaclient-4.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-manilaclient-4.4.0.tar", last modified: Thu Apr 13 10:17:23 2023, max compression
+gzip compressed data, was "python-manilaclient-4.5.0.tar", last modified: Thu Jul 13 15:39:30 2023, max compression
```

## Comparing `python-manilaclient-4.4.0.tar` & `python-manilaclient-4.5.0.tar`

### file list

```diff
@@ -1,444 +1,454 @@
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:17:23.451994 python-manilaclient-4.4.0/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       74 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/.stestr.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7111 2023-04-13 10:17:23.000000 python-manilaclient-4.4.0/AUTHORS
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      649 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/CONTRIBUTING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    32493 2023-04-13 10:17:22.000000 python-manilaclient-4.4.0/ChangeLog
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2275 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/HACKING
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11837 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/LICENSE
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5859 2023-04-13 10:17:23.451994 python-manilaclient-4.4.0/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4088 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      462 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/bindep.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:17:23.375991 python-manilaclient-4.4.0/doc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        7 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/doc/.gitignore
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3188 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/doc/Makefile
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      387 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/doc/requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:17:23.375991 python-manilaclient-4.4.0/doc/source/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:17:23.375991 python-manilaclient-4.4.0/doc/source/cli/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/doc/source/cli/.gitkeep
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:17:23.367990 python-manilaclient-4.4.0/doc/source/cli/osc/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:17:23.375991 python-manilaclient-4.4.0/doc/source/cli/osc/v2/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4421 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/doc/source/cli/osc/v2/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1695 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/doc/source/cli/osc_plugin_cli.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3599 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/doc/source/conf.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:17:23.375991 python-manilaclient-4.4.0/doc/source/contributor/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2761 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/doc/source/contributor/contributing.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8806 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/doc/source/contributor/functional-tests.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      482 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/doc/source/contributor/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1193 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/doc/source/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:17:23.375991 python-manilaclient-4.4.0/doc/source/user/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2118 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/doc/source/user/api.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1389 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/doc/source/user/shell.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:17:23.367990 python-manilaclient-4.4.0/etc/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:17:23.375991 python-manilaclient-4.4.0/etc/manilaclient/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      140 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/etc/manilaclient/README.manilaclient.conf
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:17:23.375991 python-manilaclient-4.4.0/etc/oslo-config-generator/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       98 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/etc/oslo-config-generator/manilaclient.conf
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:17:23.379991 python-manilaclient-4.4.0/manilaclient/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1248 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15186 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/api_versions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    18067 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2387 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/client.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:17:23.379991 python-manilaclient-4.4.0/manilaclient/common/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/common/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1131 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/common/_i18n.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:17:23.379991 python-manilaclient-4.4.0/manilaclient/common/apiclient/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/common/apiclient/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12887 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/common/apiclient/exceptions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2781 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/common/apiclient/utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8150 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/common/cliutils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3503 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/common/constants.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7277 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/common/httpclient.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10524 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/config.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1825 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/exceptions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1405 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/extension.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:17:23.379991 python-manilaclient-4.4.0/manilaclient/osc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/osc/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4367 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/osc/plugin.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4021 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/osc/utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:17:23.383991 python-manilaclient-4.4.0/manilaclient/osc/v2/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/osc/v2/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1310 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/osc/v2/availability_zones.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6631 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/osc/v2/messages.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14775 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/osc/v2/quotas.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16678 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/osc/v2/security_services.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4321 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/osc/v2/services.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    53048 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/osc/v2/share.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13519 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/osc/v2/share_access_rules.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14824 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/osc/v2/share_group_snapshots.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6315 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/osc/v2/share_group_type_access.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11713 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/osc/v2/share_group_types.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    18730 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/osc/v2/share_groups.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3089 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/osc/v2/share_instance_export_locations.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7645 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/osc/v2/share_instances.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2202 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/osc/v2/share_limits.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7674 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/osc/v2/share_network_subnets.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    27394 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/osc/v2/share_networks.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3636 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/osc/v2/share_pools.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2831 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/osc/v2/share_replica_export_locations.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14367 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/osc/v2/share_replicas.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    23898 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/osc/v2/share_servers.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3244 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/osc/v2/share_snapshot_instance_export_locations.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5018 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/osc/v2/share_snapshot_instances.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    29068 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/osc/v2/share_snapshots.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3975 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/osc/v2/share_type_access.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16122 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/osc/v2/share_types.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    31317 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/shell.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:17:23.383991 python-manilaclient-4.4.0/manilaclient/tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:17:23.391991 python-manilaclient-4.4.0/manilaclient/tests/functional/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/functional/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    20087 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/functional/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    87123 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/functional/client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2322 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/functional/exceptions.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:17:23.395992 python-manilaclient-4.4.0/manilaclient/tests/functional/osc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/functional/osc/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15215 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/functional/osc/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      980 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/functional/osc/test_availability_zones.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4110 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/functional/osc/test_messages.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7049 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/functional/osc/test_share_access_rules.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3533 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/functional/osc/test_share_group_type_access.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1281 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/functional/osc/test_share_limits.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1418 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/functional/osc/test_share_network_subnets.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3896 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/functional/osc/test_share_networks.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1539 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/functional/osc/test_share_pools.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2618 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/functional/osc/test_share_replica_export_locations.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2248 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/functional/osc/test_share_replicas.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2264 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/functional/osc/test_share_services.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7773 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/functional/osc/test_share_snapshots.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5408 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/functional/osc/test_share_types.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8626 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/functional/osc/test_shares.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6111 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/functional/osc/test_shares_group_type.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2146 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/functional/test_availability_zones.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2442 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/functional/test_common.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6668 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/functional/test_export_locations.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1002 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/functional/test_limits.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2755 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/functional/test_messages.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13085 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/functional/test_quotas.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1896 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/functional/test_scheduler_stats.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2435 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/functional/test_security_services.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1729 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/functional/test_services.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13367 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/functional/test_share_access.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4622 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/functional/test_share_network_subnets.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    23687 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/functional/test_share_networks.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4371 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/functional/test_share_replica_export_locations.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1966 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/functional/test_share_replicas.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14265 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/functional/test_share_servers.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    20496 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/functional/test_share_types.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11999 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/functional/test_shares.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14916 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/functional/test_shares_listing.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5391 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/functional/test_shares_metadata.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7615 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/functional/test_snapshot_access.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4968 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/functional/test_snapshot_instances.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4634 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/functional/test_snapshot_instances_export_locations.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3584 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/functional/test_snapshots_export_locations.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4955 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/functional/utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:17:23.395992 python-manilaclient-4.4.0/manilaclient/tests/unit/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/unit/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:17:23.395992 python-manilaclient-4.4.0/manilaclient/tests/unit/common/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/unit/common/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:17:23.395992 python-manilaclient-4.4.0/manilaclient/tests/unit/common/apiclient/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/unit/common/apiclient/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8145 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/unit/common/test_httpclient.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2919 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/unit/fakes.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:17:23.395992 python-manilaclient-4.4.0/manilaclient/tests/unit/osc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/unit/osc/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6610 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/unit/osc/osc_fakes.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2555 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/unit/osc/osc_utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:17:23.403992 python-manilaclient-4.4.0/manilaclient/tests/unit/osc/v2/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/unit/osc/v2/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    46247 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/unit/osc/v2/fakes.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1963 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/unit/osc/v2/test_availability_zones.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6194 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/unit/osc/v2/test_messages.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15984 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/unit/osc/v2/test_quotas.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    19607 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/unit/osc/v2/test_security_services.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6858 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/unit/osc/v2/test_services.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    67674 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/unit/osc/v2/test_share.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14621 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/unit/osc/v2/test_share_access_rules.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    21560 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/unit/osc/v2/test_share_group_snapshots.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    17697 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/unit/osc/v2/test_share_group_type.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6874 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/unit/osc/v2/test_share_group_type_access.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    24594 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/unit/osc/v2/test_share_groups.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5208 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/unit/osc/v2/test_share_instance_export_locations.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12339 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/unit/osc/v2/test_share_instances.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3044 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/unit/osc/v2/test_share_limits.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9753 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/unit/osc/v2/test_share_network_subnets.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    27426 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/unit/osc/v2/test_share_networks.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5395 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/unit/osc/v2/test_share_pools.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3996 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/unit/osc/v2/test_share_replica_export_locations.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    22544 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/unit/osc/v2/test_share_replicas.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    24995 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/unit/osc/v2/test_share_servers.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5687 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/unit/osc/v2/test_share_snapshot_instance_export_locations.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8248 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/unit/osc/v2/test_share_snapshot_instances.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    43220 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/unit/osc/v2/test_share_snapshots.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    20743 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/unit/osc/v2/test_share_type.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6357 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/unit/osc/v2/test_share_type_access.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14907 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/unit/test_api_versions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2734 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/unit/test_base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5305 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/unit/test_client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7759 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/unit/test_functional_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    17744 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/unit/test_shell.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3104 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/unit/utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:17:23.403992 python-manilaclient-4.4.0/manilaclient/tests/unit/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1187 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/unit/v1/test_limits.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1212 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/unit/v1/test_quota_classes.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1161 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/unit/v1/test_quotas.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1206 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/unit/v1/test_scheduler_stats.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1240 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/unit/v1/test_security_services.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1171 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/unit/v1/test_services.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1216 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/unit/v1/test_share_networks.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1208 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/unit/v1/test_share_servers.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1224 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/unit/v1/test_share_snapshots.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1239 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/unit/v1/test_share_type_access.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1192 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/unit/v1/test_share_types.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1155 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/unit/v1/test_shares.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:17:23.411992 python-manilaclient-4.4.0/manilaclient/tests/unit/v2/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/unit/v2/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6889 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/unit/v2/fake_clients.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    46114 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/unit/v2/fakes.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2129 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/unit/v2/test_availability_zones.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13669 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/unit/v2/test_client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5456 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/unit/v2/test_limits.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4375 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/unit/v2/test_messages.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2780 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/unit/v2/test_quota_classes.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12085 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/unit/v2/test_quotas.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2962 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/unit/v2/test_scheduler_stats.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7487 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/unit/v2/test_security_services.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3758 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/unit/v2/test_services.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1945 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/unit/v2/test_share_export_locations.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9947 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/unit/v2/test_share_group_snapshots.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4083 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/unit/v2/test_share_group_type_access.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7915 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/unit/v2/test_share_group_types.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11617 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/unit/v2/test_share_groups.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2142 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/unit/v2/test_share_instance_export_locations.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4436 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/unit/v2/test_share_instances.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3029 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/unit/v2/test_share_network_subnets.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11773 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/unit/v2/test_share_networks.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1894 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/unit/v2/test_share_replica_export_locations.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5851 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/unit/v2/test_share_replicas.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11823 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/unit/v2/test_share_servers.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1653 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/unit/v2/test_share_snapshot_export_locations.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1831 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/unit/v2/test_share_snapshot_instance_export_locations.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3612 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/unit/v2/test_share_snapshot_instances.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9545 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/unit/v2/test_share_snapshots.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    30366 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/unit/v2/test_shares.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   156971 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/unit/v2/test_shell.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3595 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/unit/v2/test_type_access.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    18918 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/tests/unit/v2/test_types.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2107 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:17:23.415992 python-manilaclient-4.4.0/manilaclient/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      917 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/v1/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10490 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/v1/client.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:17:23.415992 python-manilaclient-4.4.0/manilaclient/v1/contrib/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/v1/contrib/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1253 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/v1/contrib/list_extensions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1225 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/v1/limits.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1260 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/v1/quota_classes.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1225 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/v1/quotas.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1269 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/v1/scheduler_stats.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1285 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/v1/security_services.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1235 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/v1/services.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1265 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/v1/share_networks.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1260 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/v1/share_servers.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1256 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/v1/share_snapshots.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1285 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/v1/share_type_access.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1252 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/v1/share_types.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1211 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/v1/shares.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:17:23.423993 python-manilaclient-4.4.0/manilaclient/v2/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      681 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/v2/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1313 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/v2/availability_zones.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12841 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/v2/client.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:17:23.423993 python-manilaclient-4.4.0/manilaclient/v2/contrib/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/v2/contrib/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1448 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/v2/contrib/list_extensions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2873 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/v2/limits.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2710 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/v2/messages.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6071 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/v2/quota_classes.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11053 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/v2/quotas.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1528 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/v2/scheduler_stats.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5486 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/v2/security_services.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3357 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/v2/services.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2994 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/v2/share_access_rules.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1801 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/v2/share_export_locations.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9326 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/v2/share_group_snapshots.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3695 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/v2/share_group_type_access.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7367 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/v2/share_group_types.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11213 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/v2/share_groups.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1994 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/v2/share_instance_export_locations.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4228 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/v2/share_instances.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3358 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/v2/share_network_subnets.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13094 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/v2/share_networks.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2943 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/v2/share_replica_export_locations.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11234 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/v2/share_replicas.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10761 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/v2/share_servers.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1826 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/v2/share_snapshot_export_locations.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1940 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/v2/share_snapshot_instance_export_locations.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2700 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/v2/share_snapshot_instances.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9276 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/v2/share_snapshots.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2373 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/v2/share_type_access.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10288 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/v2/share_types.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    30069 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/v2/shares.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   216521 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/manilaclient/v2/shell.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:17:23.423993 python-manilaclient-4.4.0/playbooks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       40 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/playbooks/enable-fips.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:17:23.423993 python-manilaclient-4.4.0/playbooks/python-manilaclient-functional/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      108 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/playbooks/python-manilaclient-functional/post.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      302 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/playbooks/python-manilaclient-functional/run.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:17:23.427993 python-manilaclient-4.4.0/python_manilaclient.egg-info/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5859 2023-04-13 10:17:23.000000 python-manilaclient-4.4.0/python_manilaclient.egg-info/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    20305 2023-04-13 10:17:23.000000 python-manilaclient-4.4.0/python_manilaclient.egg-info/SOURCES.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-04-13 10:17:23.000000 python-manilaclient-4.4.0/python_manilaclient.egg-info/dependency_links.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10116 2023-04-13 10:17:23.000000 python-manilaclient-4.4.0/python_manilaclient.egg-info/entry_points.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-04-13 10:17:23.000000 python-manilaclient-4.4.0/python_manilaclient.egg-info/not-zip-safe
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2023-04-13 10:17:23.000000 python-manilaclient-4.4.0/python_manilaclient.egg-info/pbr.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      251 2023-04-13 10:17:23.000000 python-manilaclient-4.4.0/python_manilaclient.egg-info/requires.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       13 2023-04-13 10:17:23.000000 python-manilaclient-4.4.0/python_manilaclient.egg-info/top_level.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:17:23.427993 python-manilaclient-4.4.0/rally-jobs/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1890 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/rally-jobs/rally-manila-no-ss.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4247 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/rally-jobs/rally-manila.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:17:23.367990 python-manilaclient-4.4.0/releasenotes/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:17:23.447994 python-manilaclient-4.4.0/releasenotes/notes/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/Bug-1990013-fix-share-grou-from-snapshot-create-fa3629cf1417ba20.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       83 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/add-count-info-in-share-21a6b36c0f4c87b2.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       90 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/add-dash-dash-help-subcomand-ad4226454aa07bc6.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      110 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/add-export-location-filter-4cf3114doe40k598.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/add-ipv6-access-type-4dko90r1a9a1e0b8.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      315 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/add-like-filter-591572762357ef4b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       90 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/add-message-list-and-delete-41b3323edd63d894.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      231 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/add-metadata-for-share-access-rule-11a6b36c0f4c87c2.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      196 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/add-per-share-gigabytes-quotas-40bc404bd3cbdd89.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/add-query-params-pools-list-api-12cf1s14ddf40kdd.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      319 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/add-quiesce-wait-time-for-replica-promote-30d9fa66afc854f2.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       59 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/add-quota-per-share-type-support-3b2708ea232e69bc.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      357 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/add-scheduler-hints-to-share-create-70d429cb0aaf8f11.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      431 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/add-scheduler-hints-to-share-replica-create-d152a3934e5ad3a7.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      259 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/add-share-group-quotas-support-b6563cec58209a1d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      216 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/add-share-group-support-a3166f6ca4d06a81.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      774 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/add-share-network-sec-service-add-update-to-in-use-networks-ec7a60d07ebceaf4.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      333 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/add-share-replicas-and-replica-gigabytes-quotas-909436c2b2420f2c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       90 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/add-snapshot-instances-admin-api-3cf3114doe40k598.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      166 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/add-snapshot-metadata-49b0288bf2f12bf0.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       72 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/add-support-filter-search-for-share-type-fdbaaa9510cc59dd.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       79 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/add-support-to-check-quota-usage-scfdg14dod40k71a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      310 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/add_support_multiple_subnet_per_az-46145c3e90e097be.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      197 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/bp-export-locations-replica-az-commands-03aa32c08f59c42d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      107 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/bp-integrate-os-profiler-4818066dc2fbf7b7.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      339 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/bp-ocata-migration-improvements-f63c5d233856fbee.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       88 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/bp-support-group-spec-search-share-group-type-api-d5d9a6096f084b91.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      155 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/bp-support-query-user-messages-by-timestamp-34b70bba2d1b4d13.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      180 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/bp-update-share-type-name-or-description-32d98b5a42cd8090.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       97 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/bug-1558995-fix-endpoint-not-found.yaml-a06a3b0ba5006718.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       73 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/bug-1608664-add-support-columns-share-replica-list-885bd8c8b4bfa8f1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      231 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/bug-1611506-allow-deletion-multiple-resources
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       96 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/bug-1622540-add-missing-az-list-command-f90265de5c2f261b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      179 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/bug-1650774-share-instance-reset-state-9c4b26f44b5da0e9.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      380 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/bug-1664877-c462bfad92ce03e5.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      163 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/bug-1674915-allow-user-access-fix-495b3e42bdc985ec.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       68 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/bug-1682726-remove-sort-key-export-location-from-list-885des26bd5ea2de.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      157 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/bug-1707303-fix-list-command-when-not-given-search-opts-c06af7b344e9cb91.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       65 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/bug-1709746-add-group-specs-in-share-group-type-create-command-f91265de5c2f251b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      120 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/bug-1717940-dash-dash-column-reports-nothing-for-capabilities-db8c1234fae91af5.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       63 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/bug-1724183-add-share-type-description-8c4b26f44b5da1e9.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      115 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/bug-1733494-allow-user-group-name-with-blank-access-fix-885a3e42bdc985ec.yaml
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      118 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/bug-1738917-and-1738918-fix-access-share-group-type-by-name-3a8760522c147f28.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      259 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/bug-1798229-fix-create-share-from-snap-using-name-44100b907ea6a040.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       83 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/bug-1799934-add-ou-parameter-260f9aaf939d1919.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      102 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/bug-1802059-fix-is_default-a8d3d95ffa0aede9.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      110 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/bug-1811516-bug-1811627-python3-fixes-4b26130027b2c076.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      235 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/bug-1814094-fix-_get_base_url-method-168e12292aeec8f1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      211 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/bug-1830677-fix-13b30d6a89f43246.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      189 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/bug-1855391-support-force-extend-share-6b5ebcfe1de0ca7b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      395 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/bug-1871252-update-default-quotas-via-quota-class-share-groups-share-group-snapshots-20ec1dfcc0a7e81c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      202 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/bug-1898304-add-wait-to-share-create-delete-f121073f2f4402ff.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      204 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/bug-1898308-add-wait-to-share-extend-shrink-c9cc413c50d9832a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      202 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/bug-1898309-add-wait-to-share-manage-unmanage-d2060c61cc295bfd.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      184 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/bug-1898315-add-wait-flag-to-manage-share-server-operation-be6488c2a57536e1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      186 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/bug-1898316-add-wait-option-for-deleting-a-share-server-e2228018585de5cb.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      269 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/bug-1898317-add-wait-option-for-force-deleting-share-snapshot-share-instance-fb2531b6033f0ae5.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      183 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/bug-1898318-add-wait-flag-for-deleting-a-share-group-operation-c602ba9faad411be.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      183 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/bug-1898318-add-wait-flag-to-create-sharee-group-operation-cd8310b241d377b0.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      188 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/bug-1899325-implement-usage-of-c-or-column-without-additional-logic-2970ee294f32bd31.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      246 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/bug-1902873-fix-py-raw-error-msg-a839fee2ac7b9d3d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      221 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/bug-1909477-fix-forbid-users-to-create-shares-with-the-name-none-cfb0a59baa597803.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      170 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/bug-1920888-fix-error-in-cli-manila-list-with-sorting-key-availabilityzone-cea5a1f5d8a38fc3.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      335 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/bug-1925486-add-share-network-option-to-replica-create-api-7d2ff3628e93fc77.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      220 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/bug-1953670-fix-id-attr-for-share-group-type-access-repr-008338a53d7a6a50.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      170 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/bug-1959329-fix-server-listing-by-subnets-fa6447fd43093cae.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      218 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/bug-1960422-fix-no-default-share-type-d6191ea0aa1e57fa.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      323 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/bug-1960490-use-suitable-version-for-osc-b375a32273b56522.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/bug-1962288-fixed-share-network-create-command-879dc3deca131ef9.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      201 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/bug-1975488-skip-force-kwarg-if-unspecified-f98c717df1d6e364.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      228 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/bug-1980985-dont-use-share-type-with-snapshot-ref-de0331c640afbbd3.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      149 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/bug-1999775-add-os-key-0cfc95c7b480df05.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      164 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/bug-share-access-list-3cf3114doe40k599.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      175 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/bug_1570085_fix-905786b797379309.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      132 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/bug_1603387_fix_env_variable_8ed5450aab41aa5f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       63 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/bug_1606168_fix-54d3c3bb78389f01.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/bug_1715769_fix-3ec701b0fb9d7910.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      108 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/bug_1777849_1779935_fix-344cb8f09b7df502.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       83 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/bug_1782672-1954059b373f03de.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      589 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/deprecate-v1-a0cfa6fd723c2f46.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/drop-py36-and-py37-85cf389b2842f045.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      293 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/drop-python2-support-71c7b9e1dcf8c890.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/expose-access-key-in-access-list-API-b57c386c9048ae55.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      246 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/fix-and-improve-access-rules-a118a7f8e22f65bb.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      249 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/fix-is-default-empty-557844001e0401e2.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      499 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/graduate-share-replication-feature-49770e921b4338fb.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       81 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/handle-missing-api-minor-version-5a6d242f28883442.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      165 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/manage-unmanage-share-servers-8c7b27a1fe80e5fa.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      155 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/manila-client-support-recycle-bin-4ecb5de770bd525f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2119 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/manila-openstackclient-bf61ceb270d3afb7.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       82 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/migration-share-type-4fc3b7c6187f5201.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       86 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/mountable_snapshot-ced01da7dffc6d7e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      823 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/newton-migration-improvements-166a03472948bdef.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      582 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/remove-experimental-flag-from-share-groups-feature-dcf2b0b67fe4cac4.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      272 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/remove-nova-net-id-option-for-share-nets-82e424b75221528b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      550 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/share-network-multiple-subnets-732309abfbf5987c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       68 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/share-revert-to-snapshot-e899a4b7e1126749.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      304 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/share_type-skip-format-119595e62900e571.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       86 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/start-using-reno-b744cd0259c7a88c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      153 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/support-create-share-from-snapshot-extra-spec-cdba92f179c1c5c6.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      322 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/support-share-server-migration-9804752270c6b153.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       53 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/support-show-type-6380b7c539c95ba8.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       73 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/type-create-extra-specs-691572762357ef3b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      262 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/update-api-version-create-share-from-snapshot-another-pool-or-backend-694cfda84a41c4ff.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      394 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/notes/v2-0-0-deprecated-opts-removal-863565618535733d.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:17:23.447994 python-manilaclient-4.4.0/releasenotes/source/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:17:23.447994 python-manilaclient-4.4.0/releasenotes/source/_static/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/source/_static/.placeholder
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:17:23.451994 python-manilaclient-4.4.0/releasenotes/source/_templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/source/_templates/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8911 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      268 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/source/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/source/newton.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/source/ocata.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/source/pike.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/source/queens.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/source/rocky.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/source/stein.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/source/train.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      107 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/source/unreleased.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/source/ussuri.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/source/victoria.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/source/wallaby.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/source/xena.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/source/yoga.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/releasenotes/source/zed.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      847 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:17:23.367990 python-manilaclient-4.4.0/roles/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:17:23.451994 python-manilaclient-4.4.0/roles/populate-manilaclient-config/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1257 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/roles/populate-manilaclient-config/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:17:23.451994 python-manilaclient-4.4.0/roles/populate-manilaclient-config/defaults/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      199 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/roles/populate-manilaclient-config/defaults/main.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:17:23.451994 python-manilaclient-4.4.0/roles/populate-manilaclient-config/tasks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2538 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/roles/populate-manilaclient-config/tasks/main.yaml
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     5570 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/run_tests.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11142 2023-04-13 10:17:23.451994 python-manilaclient-4.4.0/setup.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      697 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/setup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      241 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/test-requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:17:23.451994 python-manilaclient-4.4.0/tools/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      367 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/tools/manila.bash_completion
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2595 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/tox.ini
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:17:23.451994 python-manilaclient-4.4.0/zuul.d/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      492 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/zuul.d/project.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4755 2023-04-13 10:16:54.000000 python-manilaclient-4.4.0/zuul.d/python-manilaclient-jobs.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 15:39:30.030097 python-manilaclient-4.5.0/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       74 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/.stestr.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7143 2023-07-13 15:39:29.000000 python-manilaclient-4.5.0/AUTHORS
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      649 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/CONTRIBUTING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    32583 2023-07-13 15:39:29.000000 python-manilaclient-4.5.0/ChangeLog
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2275 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/HACKING
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11837 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/LICENSE
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5859 2023-07-13 15:39:30.030097 python-manilaclient-4.5.0/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4088 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      462 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/bindep.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 15:39:29.954099 python-manilaclient-4.5.0/doc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        7 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/doc/.gitignore
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3188 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/doc/Makefile
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      387 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/doc/requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 15:39:29.954099 python-manilaclient-4.5.0/doc/source/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 15:39:29.954099 python-manilaclient-4.5.0/doc/source/cli/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/doc/source/cli/.gitkeep
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 15:39:29.946099 python-manilaclient-4.5.0/doc/source/cli/osc/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 15:39:29.954099 python-manilaclient-4.5.0/doc/source/cli/osc/v2/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4421 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/doc/source/cli/osc/v2/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1695 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/doc/source/cli/osc_plugin_cli.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3599 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/doc/source/conf.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 15:39:29.954099 python-manilaclient-4.5.0/doc/source/contributor/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2761 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/doc/source/contributor/contributing.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8806 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/doc/source/contributor/functional-tests.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      482 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/doc/source/contributor/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1193 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/doc/source/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 15:39:29.954099 python-manilaclient-4.5.0/doc/source/user/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2118 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/doc/source/user/api.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1389 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/doc/source/user/shell.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 15:39:29.946099 python-manilaclient-4.5.0/etc/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 15:39:29.954099 python-manilaclient-4.5.0/etc/manilaclient/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      140 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/etc/manilaclient/README.manilaclient.conf
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 15:39:29.954099 python-manilaclient-4.5.0/etc/oslo-config-generator/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       98 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/etc/oslo-config-generator/manilaclient.conf
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 15:39:29.954099 python-manilaclient-4.5.0/manilaclient/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1248 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15186 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/api_versions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    18160 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2387 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/client.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 15:39:29.958099 python-manilaclient-4.5.0/manilaclient/common/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/common/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1131 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/common/_i18n.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 15:39:29.958099 python-manilaclient-4.5.0/manilaclient/common/apiclient/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/common/apiclient/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12887 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/common/apiclient/exceptions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2781 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/common/apiclient/utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8150 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/common/cliutils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3726 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/common/constants.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7277 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/common/httpclient.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10524 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/config.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1825 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/exceptions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1405 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/extension.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 15:39:29.958099 python-manilaclient-4.5.0/manilaclient/osc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/osc/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4367 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/osc/plugin.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4021 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/osc/utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 15:39:29.962098 python-manilaclient-4.5.0/manilaclient/osc/v2/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/osc/v2/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1310 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/osc/v2/availability_zones.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6631 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/osc/v2/messages.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14775 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/osc/v2/quotas.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    20321 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/osc/v2/security_services.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4321 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/osc/v2/services.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    53048 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/osc/v2/share.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13519 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/osc/v2/share_access_rules.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14824 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/osc/v2/share_group_snapshots.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6315 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/osc/v2/share_group_type_access.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11713 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/osc/v2/share_group_types.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    18730 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/osc/v2/share_groups.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3089 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/osc/v2/share_instance_export_locations.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7645 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/osc/v2/share_instances.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2202 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/osc/v2/share_limits.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13048 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/osc/v2/share_network_subnets.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    27777 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/osc/v2/share_networks.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3636 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/osc/v2/share_pools.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2831 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/osc/v2/share_replica_export_locations.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14367 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/osc/v2/share_replicas.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    23898 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/osc/v2/share_servers.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3244 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/osc/v2/share_snapshot_instance_export_locations.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5018 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/osc/v2/share_snapshot_instances.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    29068 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/osc/v2/share_snapshots.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9165 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/osc/v2/share_transfers.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3975 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/osc/v2/share_type_access.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16122 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/osc/v2/share_types.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    31317 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/shell.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 15:39:29.962098 python-manilaclient-4.5.0/manilaclient/tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/tests/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 15:39:29.970098 python-manilaclient-4.5.0/manilaclient/tests/functional/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/tests/functional/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    21493 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/tests/functional/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    90065 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/tests/functional/client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2322 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/tests/functional/exceptions.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 15:39:29.974098 python-manilaclient-4.5.0/manilaclient/tests/functional/osc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/tests/functional/osc/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15523 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/tests/functional/osc/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      980 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/tests/functional/osc/test_availability_zones.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4110 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/tests/functional/osc/test_messages.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7049 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/tests/functional/osc/test_share_access_rules.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3533 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/tests/functional/osc/test_share_group_type_access.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1281 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/tests/functional/osc/test_share_limits.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1418 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/tests/functional/osc/test_share_network_subnets.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3896 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/tests/functional/osc/test_share_networks.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1539 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/tests/functional/osc/test_share_pools.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2618 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/tests/functional/osc/test_share_replica_export_locations.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2248 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/tests/functional/osc/test_share_replicas.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2264 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/tests/functional/osc/test_share_services.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7773 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/tests/functional/osc/test_share_snapshots.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3541 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/tests/functional/osc/test_share_transfers.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5408 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/tests/functional/osc/test_share_types.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8626 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/tests/functional/osc/test_shares.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6111 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/tests/functional/osc/test_shares_group_type.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2146 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/tests/functional/test_availability_zones.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2442 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/tests/functional/test_common.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6668 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/tests/functional/test_export_locations.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1002 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/tests/functional/test_limits.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2755 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/tests/functional/test_messages.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13085 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/tests/functional/test_quotas.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1896 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/tests/functional/test_scheduler_stats.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2727 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/tests/functional/test_security_services.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1729 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/tests/functional/test_services.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13367 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/tests/functional/test_share_access.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4622 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/tests/functional/test_share_network_subnets.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    23687 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/tests/functional/test_share_networks.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4371 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/tests/functional/test_share_replica_export_locations.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1966 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/tests/functional/test_share_replicas.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14265 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/tests/functional/test_share_servers.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4050 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/tests/functional/test_share_transfers.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    20496 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/tests/functional/test_share_types.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11999 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/tests/functional/test_shares.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14916 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/tests/functional/test_shares_listing.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5391 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/tests/functional/test_shares_metadata.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7615 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/tests/functional/test_snapshot_access.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4968 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/tests/functional/test_snapshot_instances.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4634 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/tests/functional/test_snapshot_instances_export_locations.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3584 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/tests/functional/test_snapshots_export_locations.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4955 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/tests/functional/utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 15:39:29.974098 python-manilaclient-4.5.0/manilaclient/tests/unit/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/tests/unit/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 15:39:29.974098 python-manilaclient-4.5.0/manilaclient/tests/unit/common/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/tests/unit/common/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 15:39:29.974098 python-manilaclient-4.5.0/manilaclient/tests/unit/common/apiclient/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/tests/unit/common/apiclient/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8145 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/tests/unit/common/test_httpclient.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2919 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/tests/unit/fakes.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 15:39:29.974098 python-manilaclient-4.5.0/manilaclient/tests/unit/osc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/tests/unit/osc/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6610 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/tests/unit/osc/osc_fakes.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2555 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/tests/unit/osc/osc_utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 15:39:29.982098 python-manilaclient-4.5.0/manilaclient/tests/unit/osc/v2/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/tests/unit/osc/v2/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    48193 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/tests/unit/osc/v2/fakes.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1963 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/tests/unit/osc/v2/test_availability_zones.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6194 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/tests/unit/osc/v2/test_messages.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15984 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/tests/unit/osc/v2/test_quotas.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    22375 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/tests/unit/osc/v2/test_security_services.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6858 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/tests/unit/osc/v2/test_services.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    67674 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/tests/unit/osc/v2/test_share.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14621 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/tests/unit/osc/v2/test_share_access_rules.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    21560 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/tests/unit/osc/v2/test_share_group_snapshots.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    17697 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/tests/unit/osc/v2/test_share_group_type.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6874 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/tests/unit/osc/v2/test_share_group_type_access.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    24594 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/tests/unit/osc/v2/test_share_groups.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5208 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/tests/unit/osc/v2/test_share_instance_export_locations.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12339 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/tests/unit/osc/v2/test_share_instances.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3044 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/tests/unit/osc/v2/test_share_limits.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16353 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/tests/unit/osc/v2/test_share_network_subnets.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    27426 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/tests/unit/osc/v2/test_share_networks.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5395 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/tests/unit/osc/v2/test_share_pools.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3996 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/tests/unit/osc/v2/test_share_replica_export_locations.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    22544 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/tests/unit/osc/v2/test_share_replicas.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    24995 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/tests/unit/osc/v2/test_share_servers.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5687 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/tests/unit/osc/v2/test_share_snapshot_instance_export_locations.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8248 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/tests/unit/osc/v2/test_share_snapshot_instances.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    43220 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/tests/unit/osc/v2/test_share_snapshots.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8938 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/tests/unit/osc/v2/test_share_transfers.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    20743 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/tests/unit/osc/v2/test_share_type.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6357 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/tests/unit/osc/v2/test_share_type_access.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14907 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/tests/unit/test_api_versions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2734 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/tests/unit/test_base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5305 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/tests/unit/test_client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7759 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/tests/unit/test_functional_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    17744 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/tests/unit/test_shell.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3104 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/tests/unit/utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 15:39:29.986098 python-manilaclient-4.5.0/manilaclient/tests/unit/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1187 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/tests/unit/v1/test_limits.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1212 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/tests/unit/v1/test_quota_classes.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1161 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/tests/unit/v1/test_quotas.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1206 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/tests/unit/v1/test_scheduler_stats.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1240 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/tests/unit/v1/test_security_services.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1171 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/tests/unit/v1/test_services.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1216 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/tests/unit/v1/test_share_networks.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1208 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/tests/unit/v1/test_share_servers.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1224 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/tests/unit/v1/test_share_snapshots.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1239 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/tests/unit/v1/test_share_type_access.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1192 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/tests/unit/v1/test_share_types.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1155 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/tests/unit/v1/test_shares.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 15:39:29.990098 python-manilaclient-4.5.0/manilaclient/tests/unit/v2/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/tests/unit/v2/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6889 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/tests/unit/v2/fake_clients.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    47195 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/tests/unit/v2/fakes.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2129 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/tests/unit/v2/test_availability_zones.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13669 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/tests/unit/v2/test_client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5456 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/tests/unit/v2/test_limits.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4375 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/tests/unit/v2/test_messages.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2780 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/tests/unit/v2/test_quota_classes.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12085 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/tests/unit/v2/test_quotas.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2962 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/tests/unit/v2/test_scheduler_stats.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8545 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/tests/unit/v2/test_security_services.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3758 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/tests/unit/v2/test_services.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1945 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/tests/unit/v2/test_share_export_locations.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9947 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/tests/unit/v2/test_share_group_snapshots.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4083 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/tests/unit/v2/test_share_group_type_access.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7915 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/tests/unit/v2/test_share_group_types.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11617 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/tests/unit/v2/test_share_groups.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2142 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/tests/unit/v2/test_share_instance_export_locations.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4436 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/tests/unit/v2/test_share_instances.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3069 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/tests/unit/v2/test_share_network_subnets.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11773 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/tests/unit/v2/test_share_networks.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1894 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/tests/unit/v2/test_share_replica_export_locations.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5851 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/tests/unit/v2/test_share_replicas.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11823 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/tests/unit/v2/test_share_servers.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1653 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/tests/unit/v2/test_share_snapshot_export_locations.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1831 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/tests/unit/v2/test_share_snapshot_instance_export_locations.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3612 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/tests/unit/v2/test_share_snapshot_instances.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9545 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/tests/unit/v2/test_share_snapshots.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1801 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/tests/unit/v2/test_share_transfers.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    30366 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/tests/unit/v2/test_shares.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   156971 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/tests/unit/v2/test_shell.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3595 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/tests/unit/v2/test_type_access.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    18918 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/tests/unit/v2/test_types.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2107 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 15:39:29.994098 python-manilaclient-4.5.0/manilaclient/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      917 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/v1/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10490 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/v1/client.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 15:39:29.994098 python-manilaclient-4.5.0/manilaclient/v1/contrib/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/v1/contrib/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1253 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/v1/contrib/list_extensions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1225 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/v1/limits.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1260 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/v1/quota_classes.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1225 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/v1/quotas.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1269 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/v1/scheduler_stats.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1285 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/v1/security_services.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1235 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/v1/services.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1265 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/v1/share_networks.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1260 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/v1/share_servers.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1256 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/v1/share_snapshots.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1285 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/v1/share_type_access.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1252 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/v1/share_types.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1211 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/v1/shares.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 15:39:30.002097 python-manilaclient-4.5.0/manilaclient/v2/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      681 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/v2/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1313 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/v2/availability_zones.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12953 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/v2/client.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 15:39:30.002097 python-manilaclient-4.5.0/manilaclient/v2/contrib/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/v2/contrib/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1448 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/v2/contrib/list_extensions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2873 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/v2/limits.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2710 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/v2/messages.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6071 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/v2/quota_classes.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11053 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/v2/quotas.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1528 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/v2/scheduler_stats.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9732 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/v2/security_services.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3357 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/v2/services.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2994 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/v2/share_access_rules.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1801 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/v2/share_export_locations.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9326 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/v2/share_group_snapshots.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3695 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/v2/share_group_type_access.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7367 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/v2/share_group_types.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11213 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/v2/share_groups.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1994 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/v2/share_instance_export_locations.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4228 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/v2/share_instances.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5217 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/v2/share_network_subnets.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13094 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/v2/share_networks.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2943 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/v2/share_replica_export_locations.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11234 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/v2/share_replicas.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10761 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/v2/share_servers.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1826 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/v2/share_snapshot_export_locations.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1940 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/v2/share_snapshot_instance_export_locations.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2700 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/v2/share_snapshot_instances.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9276 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/v2/share_snapshots.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4526 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/v2/share_transfers.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2373 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/v2/share_type_access.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10288 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/v2/share_types.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    30069 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/v2/shares.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   224677 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/manilaclient/v2/shell.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 15:39:30.002097 python-manilaclient-4.5.0/playbooks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       40 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/playbooks/enable-fips.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 15:39:30.002097 python-manilaclient-4.5.0/playbooks/python-manilaclient-functional/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      108 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/playbooks/python-manilaclient-functional/post.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      302 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/playbooks/python-manilaclient-functional/run.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 15:39:30.002097 python-manilaclient-4.5.0/python_manilaclient.egg-info/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5859 2023-07-13 15:39:29.000000 python-manilaclient-4.5.0/python_manilaclient.egg-info/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    20851 2023-07-13 15:39:29.000000 python-manilaclient-4.5.0/python_manilaclient.egg-info/SOURCES.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-07-13 15:39:29.000000 python-manilaclient-4.5.0/python_manilaclient.egg-info/dependency_links.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10694 2023-07-13 15:39:29.000000 python-manilaclient-4.5.0/python_manilaclient.egg-info/entry_points.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-07-13 15:39:29.000000 python-manilaclient-4.5.0/python_manilaclient.egg-info/not-zip-safe
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2023-07-13 15:39:29.000000 python-manilaclient-4.5.0/python_manilaclient.egg-info/pbr.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      251 2023-07-13 15:39:29.000000 python-manilaclient-4.5.0/python_manilaclient.egg-info/requires.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       13 2023-07-13 15:39:29.000000 python-manilaclient-4.5.0/python_manilaclient.egg-info/top_level.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 15:39:30.002097 python-manilaclient-4.5.0/rally-jobs/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1890 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/rally-jobs/rally-manila-no-ss.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4247 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/rally-jobs/rally-manila.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 15:39:29.946099 python-manilaclient-4.5.0/releasenotes/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 15:39:30.026097 python-manilaclient-4.5.0/releasenotes/notes/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/releasenotes/notes/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/releasenotes/notes/Bug-1990013-fix-share-grou-from-snapshot-create-fa3629cf1417ba20.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       83 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/releasenotes/notes/add-count-info-in-share-21a6b36c0f4c87b2.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       90 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/releasenotes/notes/add-dash-dash-help-subcomand-ad4226454aa07bc6.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      250 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/releasenotes/notes/add-defaultadsite-to-security-service-33fd0a5d1b865b11.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      110 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/releasenotes/notes/add-export-location-filter-4cf3114doe40k598.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/releasenotes/notes/add-ipv6-access-type-4dko90r1a9a1e0b8.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      315 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/releasenotes/notes/add-like-filter-591572762357ef4b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       90 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/releasenotes/notes/add-message-list-and-delete-41b3323edd63d894.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      231 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/releasenotes/notes/add-metadata-for-share-access-rule-11a6b36c0f4c87c2.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      196 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/releasenotes/notes/add-per-share-gigabytes-quotas-40bc404bd3cbdd89.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/releasenotes/notes/add-query-params-pools-list-api-12cf1s14ddf40kdd.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      319 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/releasenotes/notes/add-quiesce-wait-time-for-replica-promote-30d9fa66afc854f2.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       59 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/releasenotes/notes/add-quota-per-share-type-support-3b2708ea232e69bc.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      357 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/releasenotes/notes/add-scheduler-hints-to-share-create-70d429cb0aaf8f11.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      431 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/releasenotes/notes/add-scheduler-hints-to-share-replica-create-d152a3934e5ad3a7.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      259 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/releasenotes/notes/add-share-group-quotas-support-b6563cec58209a1d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      216 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/releasenotes/notes/add-share-group-support-a3166f6ca4d06a81.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      774 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/releasenotes/notes/add-share-network-sec-service-add-update-to-in-use-networks-ec7a60d07ebceaf4.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      333 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/releasenotes/notes/add-share-replicas-and-replica-gigabytes-quotas-909436c2b2420f2c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       90 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/releasenotes/notes/add-snapshot-instances-admin-api-3cf3114doe40k598.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      166 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/releasenotes/notes/add-snapshot-metadata-49b0288bf2f12bf0.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      181 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/releasenotes/notes/add-subnet-metadata-82426986431b0179.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       72 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/releasenotes/notes/add-support-filter-search-for-share-type-fdbaaa9510cc59dd.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       79 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/releasenotes/notes/add-support-to-check-quota-usage-scfdg14dod40k71a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      310 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/releasenotes/notes/add_support_multiple_subnet_per_az-46145c3e90e097be.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      197 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/releasenotes/notes/bp-export-locations-replica-az-commands-03aa32c08f59c42d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      107 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/releasenotes/notes/bp-integrate-os-profiler-4818066dc2fbf7b7.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      339 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/releasenotes/notes/bp-ocata-migration-improvements-f63c5d233856fbee.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       88 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/releasenotes/notes/bp-support-group-spec-search-share-group-type-api-d5d9a6096f084b91.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      155 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/releasenotes/notes/bp-support-query-user-messages-by-timestamp-34b70bba2d1b4d13.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       98 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/releasenotes/notes/bp-support-share-transfer-between-project-faefead551380eca.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      180 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/releasenotes/notes/bp-update-share-type-name-or-description-32d98b5a42cd8090.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       97 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/releasenotes/notes/bug-1558995-fix-endpoint-not-found.yaml-a06a3b0ba5006718.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       73 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/releasenotes/notes/bug-1608664-add-support-columns-share-replica-list-885bd8c8b4bfa8f1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      231 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/releasenotes/notes/bug-1611506-allow-deletion-multiple-resources
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       96 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/releasenotes/notes/bug-1622540-add-missing-az-list-command-f90265de5c2f261b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      179 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/releasenotes/notes/bug-1650774-share-instance-reset-state-9c4b26f44b5da0e9.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      380 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/releasenotes/notes/bug-1664877-c462bfad92ce03e5.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      163 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/releasenotes/notes/bug-1674915-allow-user-access-fix-495b3e42bdc985ec.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       68 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/releasenotes/notes/bug-1682726-remove-sort-key-export-location-from-list-885des26bd5ea2de.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      157 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/releasenotes/notes/bug-1707303-fix-list-command-when-not-given-search-opts-c06af7b344e9cb91.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       65 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/releasenotes/notes/bug-1709746-add-group-specs-in-share-group-type-create-command-f91265de5c2f251b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      120 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/releasenotes/notes/bug-1717940-dash-dash-column-reports-nothing-for-capabilities-db8c1234fae91af5.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       63 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/releasenotes/notes/bug-1724183-add-share-type-description-8c4b26f44b5da1e9.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      115 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/releasenotes/notes/bug-1733494-allow-user-group-name-with-blank-access-fix-885a3e42bdc985ec.yaml
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      118 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/releasenotes/notes/bug-1738917-and-1738918-fix-access-share-group-type-by-name-3a8760522c147f28.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      259 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/releasenotes/notes/bug-1798229-fix-create-share-from-snap-using-name-44100b907ea6a040.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       83 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/releasenotes/notes/bug-1799934-add-ou-parameter-260f9aaf939d1919.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      102 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/releasenotes/notes/bug-1802059-fix-is_default-a8d3d95ffa0aede9.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      110 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/releasenotes/notes/bug-1811516-bug-1811627-python3-fixes-4b26130027b2c076.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      235 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/releasenotes/notes/bug-1814094-fix-_get_base_url-method-168e12292aeec8f1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      211 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/releasenotes/notes/bug-1830677-fix-13b30d6a89f43246.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      189 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/releasenotes/notes/bug-1855391-support-force-extend-share-6b5ebcfe1de0ca7b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      395 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/releasenotes/notes/bug-1871252-update-default-quotas-via-quota-class-share-groups-share-group-snapshots-20ec1dfcc0a7e81c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      202 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/releasenotes/notes/bug-1898304-add-wait-to-share-create-delete-f121073f2f4402ff.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      204 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/releasenotes/notes/bug-1898308-add-wait-to-share-extend-shrink-c9cc413c50d9832a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      202 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/releasenotes/notes/bug-1898309-add-wait-to-share-manage-unmanage-d2060c61cc295bfd.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      184 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/releasenotes/notes/bug-1898315-add-wait-flag-to-manage-share-server-operation-be6488c2a57536e1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      186 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/releasenotes/notes/bug-1898316-add-wait-option-for-deleting-a-share-server-e2228018585de5cb.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      269 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/releasenotes/notes/bug-1898317-add-wait-option-for-force-deleting-share-snapshot-share-instance-fb2531b6033f0ae5.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      183 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/releasenotes/notes/bug-1898318-add-wait-flag-for-deleting-a-share-group-operation-c602ba9faad411be.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      183 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/releasenotes/notes/bug-1898318-add-wait-flag-to-create-sharee-group-operation-cd8310b241d377b0.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      188 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/releasenotes/notes/bug-1899325-implement-usage-of-c-or-column-without-additional-logic-2970ee294f32bd31.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      246 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/releasenotes/notes/bug-1902873-fix-py-raw-error-msg-a839fee2ac7b9d3d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      221 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/releasenotes/notes/bug-1909477-fix-forbid-users-to-create-shares-with-the-name-none-cfb0a59baa597803.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      170 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/releasenotes/notes/bug-1920888-fix-error-in-cli-manila-list-with-sorting-key-availabilityzone-cea5a1f5d8a38fc3.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      335 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/releasenotes/notes/bug-1925486-add-share-network-option-to-replica-create-api-7d2ff3628e93fc77.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      220 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/releasenotes/notes/bug-1953670-fix-id-attr-for-share-group-type-access-repr-008338a53d7a6a50.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      170 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/releasenotes/notes/bug-1959329-fix-server-listing-by-subnets-fa6447fd43093cae.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      218 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/releasenotes/notes/bug-1960422-fix-no-default-share-type-d6191ea0aa1e57fa.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      323 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/releasenotes/notes/bug-1960490-use-suitable-version-for-osc-b375a32273b56522.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/releasenotes/notes/bug-1962288-fixed-share-network-create-command-879dc3deca131ef9.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      201 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/releasenotes/notes/bug-1975488-skip-force-kwarg-if-unspecified-f98c717df1d6e364.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      228 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/releasenotes/notes/bug-1980985-dont-use-share-type-with-snapshot-ref-de0331c640afbbd3.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      149 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/releasenotes/notes/bug-1999775-add-os-key-0cfc95c7b480df05.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      164 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/releasenotes/notes/bug-share-access-list-3cf3114doe40k599.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      175 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/releasenotes/notes/bug_1570085_fix-905786b797379309.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      132 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/releasenotes/notes/bug_1603387_fix_env_variable_8ed5450aab41aa5f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       63 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/releasenotes/notes/bug_1606168_fix-54d3c3bb78389f01.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/releasenotes/notes/bug_1715769_fix-3ec701b0fb9d7910.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      108 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/releasenotes/notes/bug_1777849_1779935_fix-344cb8f09b7df502.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       83 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/releasenotes/notes/bug_1782672-1954059b373f03de.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      589 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/releasenotes/notes/deprecate-v1-a0cfa6fd723c2f46.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/releasenotes/notes/drop-py36-and-py37-85cf389b2842f045.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      293 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/releasenotes/notes/drop-python2-support-71c7b9e1dcf8c890.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/releasenotes/notes/expose-access-key-in-access-list-API-b57c386c9048ae55.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      246 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/releasenotes/notes/fix-and-improve-access-rules-a118a7f8e22f65bb.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      249 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/releasenotes/notes/fix-is-default-empty-557844001e0401e2.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      499 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/releasenotes/notes/graduate-share-replication-feature-49770e921b4338fb.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       81 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/releasenotes/notes/handle-missing-api-minor-version-5a6d242f28883442.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      165 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/releasenotes/notes/manage-unmanage-share-servers-8c7b27a1fe80e5fa.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      155 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/releasenotes/notes/manila-client-support-recycle-bin-4ecb5de770bd525f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2119 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/releasenotes/notes/manila-openstackclient-bf61ceb270d3afb7.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       82 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/releasenotes/notes/migration-share-type-4fc3b7c6187f5201.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       86 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/releasenotes/notes/mountable_snapshot-ced01da7dffc6d7e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      823 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/releasenotes/notes/newton-migration-improvements-166a03472948bdef.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      582 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/releasenotes/notes/remove-experimental-flag-from-share-groups-feature-dcf2b0b67fe4cac4.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      272 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/releasenotes/notes/remove-nova-net-id-option-for-share-nets-82e424b75221528b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      550 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/releasenotes/notes/share-network-multiple-subnets-732309abfbf5987c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       68 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/releasenotes/notes/share-revert-to-snapshot-e899a4b7e1126749.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      304 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/releasenotes/notes/share_type-skip-format-119595e62900e571.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       86 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/releasenotes/notes/start-using-reno-b744cd0259c7a88c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      153 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/releasenotes/notes/support-create-share-from-snapshot-extra-spec-cdba92f179c1c5c6.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      322 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/releasenotes/notes/support-share-server-migration-9804752270c6b153.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       53 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/releasenotes/notes/support-show-type-6380b7c539c95ba8.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       73 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/releasenotes/notes/type-create-extra-specs-691572762357ef3b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      262 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/releasenotes/notes/update-api-version-create-share-from-snapshot-another-pool-or-backend-694cfda84a41c4ff.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      394 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/releasenotes/notes/v2-0-0-deprecated-opts-removal-863565618535733d.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 15:39:30.026097 python-manilaclient-4.5.0/releasenotes/source/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/releasenotes/source/2023.1.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 15:39:30.026097 python-manilaclient-4.5.0/releasenotes/source/_static/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/releasenotes/source/_static/.placeholder
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 15:39:30.026097 python-manilaclient-4.5.0/releasenotes/source/_templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/releasenotes/source/_templates/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8911 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/releasenotes/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      278 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/releasenotes/source/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/releasenotes/source/newton.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/releasenotes/source/ocata.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/releasenotes/source/pike.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/releasenotes/source/queens.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/releasenotes/source/rocky.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/releasenotes/source/stein.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/releasenotes/source/train.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      107 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/releasenotes/source/unreleased.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/releasenotes/source/ussuri.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/releasenotes/source/victoria.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/releasenotes/source/wallaby.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/releasenotes/source/xena.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/releasenotes/source/yoga.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/releasenotes/source/zed.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      847 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 15:39:29.950099 python-manilaclient-4.5.0/roles/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 15:39:30.030097 python-manilaclient-4.5.0/roles/populate-manilaclient-config/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1257 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/roles/populate-manilaclient-config/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 15:39:30.030097 python-manilaclient-4.5.0/roles/populate-manilaclient-config/defaults/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      199 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/roles/populate-manilaclient-config/defaults/main.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 15:39:30.030097 python-manilaclient-4.5.0/roles/populate-manilaclient-config/tasks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2538 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/roles/populate-manilaclient-config/tasks/main.yaml
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     5570 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/run_tests.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11727 2023-07-13 15:39:30.030097 python-manilaclient-4.5.0/setup.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      697 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/setup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      241 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/test-requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 15:39:30.030097 python-manilaclient-4.5.0/tools/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      367 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/tools/manila.bash_completion
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2595 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/tox.ini
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 15:39:30.030097 python-manilaclient-4.5.0/zuul.d/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      492 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/zuul.d/project.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4755 2023-07-13 15:39:01.000000 python-manilaclient-4.5.0/zuul.d/python-manilaclient-jobs.yaml
```

### Comparing `python-manilaclient-4.4.0/AUTHORS` & `python-manilaclient-4.5.0/AUTHORS`

 * *Files 0% similar despite different names*

```diff
@@ -131,14 +131,15 @@
 dengzhaosen <dengzhaosen@inspur.com>
 devin <genghang888@gmail.com>
 dineshbhor <dinesh.bhor@nttdata.com>
 drngsl <drngsl@qq.com>
 e <liuyamin@fiberhome.com>
 gugug <gu.jin@99cloud.net>
 haixin <653186640@qq.com>
+haixin <haix09@chinatelecom.cn>
 haixin <haixin@inspur.com>
 hassanasghar <hassanasghar666@gmail.com>
 houming-wang <houming.wang@easystack.cn>
 howardlee <lihongweibj@inspur.com>
 iswarya_vakati <v.iswarya@nectechnologies.in>
 jacky06 <zhang.min@99cloud.net>
 ji-xuepeng <ji.xuepeng@zte.com.cn>
```

### Comparing `python-manilaclient-4.4.0/CONTRIBUTING.rst` & `python-manilaclient-4.5.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/ChangeLog` & `python-manilaclient-4.5.0/ChangeLog`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 CHANGES
 =======
 
-4.4.0
+4.5.0
 -----
 
-* Fix share network create command with the AZ option
+* Metadata for Share Network Subnets
 * Use suitable api version for OSC
-* Update TOX\_CONSTRAINTS\_FILE for stable/2023.1
-* Update .gitreview for stable/2023.1
+* Fix share network create command with the AZ option
+* Add defaultadsite to security service
+* Update master for stable/2023.1
+* Update micversion to 2.77,support share transfer between project
 
 4.3.0
 -----
 
 * Add quiesce\_wait\_time for replica promote
 * Metadata for Share Snapshots
 * Drop duplicate tox config
```

### Comparing `python-manilaclient-4.4.0/HACKING` & `python-manilaclient-4.5.0/HACKING`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/LICENSE` & `python-manilaclient-4.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/PKG-INFO` & `python-manilaclient-4.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: python-manilaclient
-Version: 4.4.0
+Version: 4.5.0
 Summary: Client library for OpenStack Manila API.
 Home-page: https://docs.openstack.org/python-manilaclient/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ========================
         Team and repository tags
```

### Comparing `python-manilaclient-4.4.0/README.rst` & `python-manilaclient-4.5.0/README.rst`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/doc/Makefile` & `python-manilaclient-4.5.0/doc/Makefile`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/doc/source/cli/osc/v2/index.rst` & `python-manilaclient-4.5.0/doc/source/cli/osc/v2/index.rst`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/doc/source/cli/osc_plugin_cli.rst` & `python-manilaclient-4.5.0/doc/source/cli/osc_plugin_cli.rst`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/doc/source/conf.py` & `python-manilaclient-4.5.0/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/doc/source/contributor/contributing.rst` & `python-manilaclient-4.5.0/doc/source/contributor/contributing.rst`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/doc/source/contributor/functional-tests.rst` & `python-manilaclient-4.5.0/doc/source/contributor/functional-tests.rst`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/doc/source/index.rst` & `python-manilaclient-4.5.0/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/doc/source/user/api.rst` & `python-manilaclient-4.5.0/doc/source/user/api.rst`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/doc/source/user/shell.rst` & `python-manilaclient-4.5.0/doc/source/user/shell.rst`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/__init__.py` & `python-manilaclient-4.5.0/manilaclient/__init__.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/api_versions.py` & `python-manilaclient-4.5.0/manilaclient/api_versions.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 from manilaclient.common import cliutils
 from manilaclient.common import constants
 from manilaclient import exceptions
 from manilaclient import utils
 
 LOG = logging.getLogger(__name__)
 
-MAX_VERSION = '2.75'
+MAX_VERSION = '2.78'
 MIN_VERSION = '2.0'
 DEPRECATED_VERSION = '1.0'
 _VERSIONED_METHOD_MAP = {}
 
 
 class APIVersion(object):
     """Top level object to support Manila API Versioning.
```

### Comparing `python-manilaclient-4.4.0/manilaclient/base.py` & `python-manilaclient-4.5.0/manilaclient/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -189,14 +189,17 @@
         if return_raw:
             return body[response_key]
 
         with self.completion_cache('human_id', self.resource_class, mode="a"):
             with self.completion_cache('uuid', self.resource_class, mode="a"):
                 return self.resource_class(self, body[response_key])
 
+    def _accept(self, url, body):
+        resp, body = self.api.client.post(url, body=body)
+
     def _delete(self, url):
         resp, body = self.api.client.delete(url)
 
     def _update(self, url, body, response_key=None, **kwargs):
         self.run_hooks('modify_body_for_update', body, **kwargs)
         resp, body = self.api.client.put(url, body=body)
         if body:
```

### Comparing `python-manilaclient-4.4.0/manilaclient/client.py` & `python-manilaclient-4.5.0/manilaclient/client.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/common/_i18n.py` & `python-manilaclient-4.5.0/manilaclient/common/_i18n.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/common/apiclient/exceptions.py` & `python-manilaclient-4.5.0/manilaclient/common/apiclient/exceptions.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/common/apiclient/utils.py` & `python-manilaclient-4.5.0/manilaclient/common/apiclient/utils.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/common/cliutils.py` & `python-manilaclient-4.5.0/manilaclient/common/cliutils.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/common/constants.py` & `python-manilaclient-4.5.0/manilaclient/common/constants.py`

 * *Files 3% similar despite different names*

```diff
@@ -64,14 +64,25 @@
     'host',
     'user_id',
     'project_id',
     'created_at',
     'share_group_id',
 )
 
+SHARE_TRANSFER_SORT_KEY_VALUES = (
+    'id',
+    'resource_type',
+    'resource_id',
+    'name',
+    'source_project_id',
+    'destination_project_id',
+    'created_at',
+    'expires_at',
+)
+
 TASK_STATE_MIGRATION_SUCCESS = 'migration_success'
 TASK_STATE_MIGRATION_ERROR = 'migration_error'
 TASK_STATE_MIGRATION_CANCELLED = 'migration_cancelled'
 TASK_STATE_MIGRATION_DRIVER_PHASE1_DONE = 'migration_driver_phase1_done'
 TASK_STATE_DATA_COPYING_COMPLETED = 'data_copying_completed'
 
 EXPERIMENTAL_HTTP_HEADER = 'X-OpenStack-Manila-API-Experimental'
@@ -115,7 +126,8 @@
 # share group types
 GROUP_BOOL_SPECS = (
     CONSISTENT_SNAPSHOT_SUPPORT,
 )
 
 REPLICA_GRADUATION_VERSION = '2.56'
 REPLICA_PRE_GRADUATION_VERSION = '2.55'
+SHARE_TRANSFER_VERSION = '2.77'
```

### Comparing `python-manilaclient-4.4.0/manilaclient/common/httpclient.py` & `python-manilaclient-4.5.0/manilaclient/common/httpclient.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/config.py` & `python-manilaclient-4.5.0/manilaclient/config.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/exceptions.py` & `python-manilaclient-4.5.0/manilaclient/exceptions.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/extension.py` & `python-manilaclient-4.5.0/manilaclient/extension.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/osc/plugin.py` & `python-manilaclient-4.5.0/manilaclient/osc/plugin.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/osc/utils.py` & `python-manilaclient-4.5.0/manilaclient/osc/utils.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/osc/v2/availability_zones.py` & `python-manilaclient-4.5.0/manilaclient/osc/v2/availability_zones.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/osc/v2/messages.py` & `python-manilaclient-4.5.0/manilaclient/osc/v2/messages.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/osc/v2/quotas.py` & `python-manilaclient-4.5.0/manilaclient/osc/v2/quotas.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/osc/v2/security_services.py` & `python-manilaclient-4.5.0/manilaclient/osc/v2/security_services.py`

 * *Files 18% similar despite different names*

```diff
@@ -83,14 +83,23 @@
         )
         parser.add_argument(
             '--description',
             metavar='<description>',
             default=None,
             help=_("Security service description.")
         )
+        parser.add_argument(
+            '--default-ad-site',
+            metavar='<default_ad_site>',
+            dest='default_ad_site',
+            default=None,
+            help=_("Default AD site. Available only for "
+                   "microversion >= 2.76. Can be provided in the "
+                   "place of '--server' but not along with it.")
+        )
         return parser
 
     def take_action(self, parsed_args):
         share_client = self.app.client_manager.share
 
         kwargs = {
             'dns_ip': parsed_args.dns_ip,
@@ -100,20 +109,35 @@
             'password': parsed_args.password,
             'name': parsed_args.name,
             'description': parsed_args.description,
         }
 
         if share_client.api_version >= api_versions.APIVersion("2.44"):
             kwargs['ou'] = parsed_args.ou
-
         elif parsed_args.ou:
             raise exceptions.CommandError(
                 "Defining a security service Organizational Unit is "
                 "available only for microversion >= 2.44")
 
+        if share_client.api_version >= api_versions.APIVersion("2.76"):
+            kwargs['default_ad_site'] = parsed_args.default_ad_site
+        elif parsed_args.default_ad_site:
+            raise exceptions.CommandError(
+                "Defining a security service Default AD site is "
+                "available only for microversion >= 2.76")
+
+        if parsed_args.type == 'active_directory':
+            server = parsed_args.server
+            default_ad_site = parsed_args.default_ad_site
+            if server and default_ad_site:
+                raise exceptions.CommandError(
+                    "Cannot create security service because both "
+                    "server and 'default_ad_site' were provided. "
+                    "Specify either server or 'default_ad_site'.")
+
         security_service = share_client.security_services.create(
             parsed_args.type, **kwargs)
 
         return self.dict2columns(security_service._info)
 
 
 class DeleteShareSecurityService(command.Command):
@@ -239,14 +263,22 @@
         )
         parser.add_argument(
             '--description',
             metavar='<description>',
             default=None,
             help=_("Set security service description.")
         )
+        parser.add_argument(
+            '--default-ad-site',
+            metavar='<default_ad_site>',
+            dest='default_ad_site',
+            default=None,
+            help=_("Default AD site. "
+                   "Available only for microversion >= 2.76.")
+        )
         return parser
 
     def take_action(self, parsed_args):
         share_client = self.app.client_manager.share
 
         security_service = oscutils.find_resource(
             share_client.security_services,
@@ -260,19 +292,34 @@
             'password': parsed_args.password,
             'name': parsed_args.name,
             'description': parsed_args.description,
         }
 
         if share_client.api_version >= api_versions.APIVersion("2.44"):
             kwargs['ou'] = parsed_args.ou
-
         elif parsed_args.ou:
             raise exceptions.CommandError(_(
                 "Setting a security service Organizational Unit is "
                 "available only for microversion >= 2.44"))
+
+        if share_client.api_version >= api_versions.APIVersion("2.76"):
+            kwargs['default_ad_site'] = parsed_args.default_ad_site
+        elif parsed_args.default_ad_site:
+            raise exceptions.CommandError(
+                "Defining a security service Default AD site is "
+                "available only for microversion >= 2.76")
+
+        if security_service.type == 'active_directory':
+            server = parsed_args.server
+            default_ad_site = parsed_args.default_ad_site
+            if server and default_ad_site:
+                raise exceptions.CommandError(
+                    "Cannot set security service because both "
+                    "server and 'default_ad_site' were provided. "
+                    "Specify either server or 'default_ad_site'.")
         try:
             security_service.update(**kwargs)
         except Exception as e:
             raise exceptions.CommandError(
                 f"One or more set operations failed: {e}")
 
 
@@ -324,14 +371,21 @@
             help=_("Unset security service name.")
         )
         parser.add_argument(
             '--description',
             action='store_true',
             help=_("Unset security service description.")
         )
+        parser.add_argument(
+            '--default-ad-site',
+            dest='default_ad_site',
+            action='store_true',
+            help=_("Default AD site. "
+                   "Available only for microversion >= 2.76.")
+        )
         return parser
 
     def take_action(self, parsed_args):
         share_client = self.app.client_manager.share
 
         security_service = oscutils.find_resource(
             share_client.security_services,
@@ -350,14 +404,24 @@
             # the SDK unsets a value if it is an empty string
             kwargs['ou'] = ''
 
         elif parsed_args.ou:
             raise exceptions.CommandError(_(
                 "Unsetting a security service Organizational Unit is "
                 "available only for microversion >= 2.44"))
+
+        if (parsed_args.default_ad_site and
+                share_client.api_version >= api_versions.APIVersion("2.76")):
+            # the SDK unsets a value if it is an empty string
+            kwargs['default_ad_site'] = ''
+        elif parsed_args.default_ad_site:
+            raise exceptions.CommandError(_(
+                "Unsetting a security service Default AD site is "
+                "available only for microversion >= 2.76"))
+
         try:
             security_service.update(**kwargs)
         except Exception as e:
             raise exceptions.CommandError(
                 f"One or more unset operations failed: {e}")
 
 
@@ -415,14 +479,22 @@
             metavar='<ou>',
             default=None,
             help=_("Filter results by security service OU "
                    "(Organizational Unit). "
                    "Available only for microversion >= 2.44.")
         )
         parser.add_argument(
+            '--default-ad-site',
+            metavar='<default_ad_site>',
+            dest='default_ad_site',
+            default=None,
+            help=_("Filter results by security service default_ad_site. "
+                   "Available only for microversion >= 2.76.")
+        )
+        parser.add_argument(
             '--server',
             metavar='<server>',
             default=None,
             help=_("Filter results by security service IP "
                    "address or hostname.")
         )
         parser.add_argument(
@@ -481,14 +553,22 @@
             search_opts['ou'] = parsed_args.ou
 
         elif parsed_args.ou:
             raise exceptions.CommandError(_(
                 "Filtering results by security service Organizational Unit is "
                 "available only for microversion >= 2.44"))
 
+        if (parsed_args.default_ad_site and
+                share_client.api_version >= api_versions.APIVersion("2.76")):
+            search_opts['default_ad_site'] = parsed_args.default_ad_site
+        elif parsed_args.default_ad_site:
+            raise exceptions.CommandError(_(
+                "Filtering results by security service Default AD site is "
+                "available only for microversion >= 2.76"))
+
         if parsed_args.share_network:
             search_opts['share_network_id'] = oscutils.find_resource(
                 share_client.share_networks,
                 parsed_args.share_network).id
 
         data = share_client.security_services.list(
             search_opts=search_opts,
```

### Comparing `python-manilaclient-4.4.0/manilaclient/osc/v2/services.py` & `python-manilaclient-4.5.0/manilaclient/osc/v2/services.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/osc/v2/share.py` & `python-manilaclient-4.5.0/manilaclient/osc/v2/share.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/osc/v2/share_access_rules.py` & `python-manilaclient-4.5.0/manilaclient/osc/v2/share_access_rules.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/osc/v2/share_group_snapshots.py` & `python-manilaclient-4.5.0/manilaclient/osc/v2/share_group_snapshots.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/osc/v2/share_group_type_access.py` & `python-manilaclient-4.5.0/manilaclient/osc/v2/share_group_type_access.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/osc/v2/share_group_types.py` & `python-manilaclient-4.5.0/manilaclient/osc/v2/share_group_types.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/osc/v2/share_groups.py` & `python-manilaclient-4.5.0/manilaclient/osc/v2/share_groups.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/osc/v2/share_instance_export_locations.py` & `python-manilaclient-4.5.0/manilaclient/osc/v2/share_instance_export_locations.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/osc/v2/share_instances.py` & `python-manilaclient-4.5.0/manilaclient/osc/v2/share_instances.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/osc/v2/share_limits.py` & `python-manilaclient-4.5.0/manilaclient/osc/v2/share_limits.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/osc/v2/share_networks.py` & `python-manilaclient-4.5.0/manilaclient/osc/v2/share_networks.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 #   WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 #   License for the specific language governing permissions and limitations
 #   under the License.
 
 import logging
 
 from openstackclient.identity import common as identity_common
+from osc_lib.cli import format_columns
 from osc_lib.command import command
 from osc_lib import exceptions
 from osc_lib import utils as oscutils
 
 from manilaclient import api_versions
 from manilaclient.common._i18n import _
 from manilaclient.common import cliutils
@@ -207,14 +208,24 @@
 
         share_network = oscutils.find_resource(
             share_client.share_networks,
             parsed_args.share_network)
 
         data = share_network._info
 
+        # Special mapping for columns to make the output easier to read:
+        # 'metadata' --> 'properties'
+        for ss in data['share_network_subnets']:
+            ss.update(
+                {
+                    'properties':
+                        format_columns.DictColumn(ss.pop('metadata', {})),
+                },
+            )
+
         # Add security services information
         security_services = share_client.security_services.list(
             search_opts={'share_network_id': share_network.id}, detailed=False)
         data['security_services'] = [
             {
                 'security_service_name': ss.name,
                 'security_service_id': ss.id,
```

### Comparing `python-manilaclient-4.4.0/manilaclient/osc/v2/share_pools.py` & `python-manilaclient-4.5.0/manilaclient/osc/v2/share_pools.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/osc/v2/share_replica_export_locations.py` & `python-manilaclient-4.5.0/manilaclient/osc/v2/share_replica_export_locations.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/osc/v2/share_replicas.py` & `python-manilaclient-4.5.0/manilaclient/osc/v2/share_replicas.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/osc/v2/share_servers.py` & `python-manilaclient-4.5.0/manilaclient/osc/v2/share_servers.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/osc/v2/share_snapshot_instance_export_locations.py` & `python-manilaclient-4.5.0/manilaclient/osc/v2/share_snapshot_instance_export_locations.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/osc/v2/share_snapshot_instances.py` & `python-manilaclient-4.5.0/manilaclient/osc/v2/share_snapshot_instances.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/osc/v2/share_snapshots.py` & `python-manilaclient-4.5.0/manilaclient/osc/v2/share_snapshots.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/osc/v2/share_type_access.py` & `python-manilaclient-4.5.0/manilaclient/osc/v2/share_type_access.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/osc/v2/share_types.py` & `python-manilaclient-4.5.0/manilaclient/osc/v2/share_types.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/shell.py` & `python-manilaclient-4.5.0/manilaclient/shell.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/tests/functional/base.py` & `python-manilaclient-4.5.0/manilaclient/tests/functional/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -365,43 +365,75 @@
     def restore_share(cls, shares_to_restore,
                       client=None, microversion=None):
         client = client or cls.get_admin_client()
         client.restore_share(shares_to_restore,
                              microversion=microversion)
 
     @classmethod
+    def create_share_transfer(cls, share_id, name=None,
+                              client=None, microversion=None):
+        client = client or cls.get_admin_client()
+        return client.create_share_transfer(share_id, name=name,
+                                            microversion=microversion)
+
+    @classmethod
+    def delete_share_transfer(cls, transfer, client=None,
+                              microversion=None):
+        client = client or cls.get_admin_client()
+        client.delete_share_transfer(transfer, microversion=microversion)
+
+    @classmethod
+    def get_share_transfer(cls, transfer, client=None, microversion=None):
+        client = client or cls.get_admin_client()
+        return client.get_share_transfer(transfer, microversion=microversion)
+
+    @classmethod
+    def list_share_transfer(cls, client=None, microversion=None):
+        client = client or cls.get_admin_client()
+        return client.list_share_transfer(microversion=microversion)
+
+    @classmethod
+    def accept_share_transfer(cls, transfer, auth_key,
+                              client=None, microversion=None):
+        client = client or cls.get_admin_client()
+        client.accept_share_transfer(transfer, auth_key,
+                                     microversion=microversion)
+
+    @classmethod
     def _determine_share_network_to_use(cls, client, share_type,
                                         microversion=None):
         """Determine what share network we need from the share type."""
 
         # Get share type, determine if we need the share network
         share_type = client.get_share_type(share_type,
                                            microversion=microversion)
         dhss_pattern = re.compile('driver_handles_share_servers : ([a-zA-Z]+)')
         dhss = dhss_pattern.search(share_type['required_extra_specs']).group(1)
         return client.share_network if dhss.lower() == 'true' else None
 
     @classmethod
     def create_security_service(cls, type='ldap', name=None, description=None,
                                 dns_ip=None, ou=None, server=None, domain=None,
-                                user=None, password=None, client=None,
-                                cleanup_in_class=False, microversion=None):
+                                user=None, password=None, default_ad_site=None,
+                                client=None, cleanup_in_class=False,
+                                microversion=None):
         if client is None:
             client = cls.get_admin_client()
         data = {
             'type': type,
             'name': name,
             'description': description,
             'user': user,
             'password': password,
             'server': server,
             'domain': domain,
             'dns_ip': dns_ip,
             'ou': ou,
             'microversion': microversion,
+            'default_ad_site': default_ad_site,
         }
         ss = client.create_security_service(**data)
         resource = {
             "type": "share",
             "id": ss["id"],
             "client": client,
             "microversion": microversion,
```

### Comparing `python-manilaclient-4.4.0/manilaclient/tests/functional/client.py` & `python-manilaclient-4.5.0/manilaclient/tests/functional/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 SHARE = 'share'
 SHARE_TYPE = 'share_type'
 SHARE_NETWORK = 'share_network'
 SHARE_NETWORK_SUBNET = 'share_network_subnet'
 SHARE_SERVER = 'share_server'
 SNAPSHOT = 'snapshot'
 SHARE_REPLICA = 'share_replica'
+TRANSFER = 'transfer'
 
 
 def not_found_wrapper(f):
 
     def wrapped_func(self, *args, **kwargs):
         try:
             return f(self, *args, **kwargs)
@@ -138,14 +139,16 @@
             func = self.is_share_deleted
         elif res_type == SNAPSHOT:
             func = self.is_snapshot_deleted
         elif res_type == MESSAGE:
             func = self.is_message_deleted
         elif res_type == SHARE_REPLICA:
             func = self.is_share_replica_deleted
+        elif res_type == TRANSFER:
+            func = self.is_share_transfer_deleted
         else:
             raise exceptions.InvalidResource(message=res_type)
 
         end_loop_time = time.time() + timeout
         deleted = func(res_id, microversion=microversion, **kwargs)
 
         while not (deleted or time.time() > end_loop_time):
@@ -915,14 +918,63 @@
         if not isinstance(shares, list):
             shares = [shares]
         cmd = 'restore '
         for share in shares:
             cmd += '%s ' % share
         return self.manila(cmd, microversion=microversion)
 
+    def create_share_transfer(self, share_id, name=None,
+                              microversion=None):
+        """Create a share transfer.
+
+        :param share_id: ID of share.
+        ":param name: name of transfer.
+        """
+        cmd = 'share-transfer-create %s ' % share_id
+        if name:
+            cmd += '--name %s' % name
+        transfer_raw = self.manila(cmd, microversion=microversion)
+        transfer = output_parser.details(transfer_raw)
+        return transfer
+
+    def delete_share_transfer(self, transfer, microversion=None):
+        """Delete a share transfer.
+
+        :param transfer: ID or name of share transfer.
+        """
+        cmd = 'share-transfer-delete %s ' % transfer
+        self.manila(cmd, microversion=microversion)
+
+    def get_share_transfer(self, transfer, microversion=None):
+        """Get a share transfer.
+
+        :param transfer: ID or name of share transfer.
+        """
+        cmd = 'share-transfer-show %s ' % transfer
+        transfer_raw = self.manila(cmd, microversion=microversion)
+        transfer = output_parser.details(transfer_raw)
+        return transfer
+
+    def list_share_transfer(self, microversion=None):
+        """Get a share transfer."""
+
+        cmd = 'share-transfer-list '
+        transfer_raw = self.manila(cmd, microversion=microversion)
+        transfers = utils.listing(transfer_raw)
+        return transfers
+
+    def accept_share_transfer(self, transfer, auth_key,
+                              microversion=None):
+        """Accept a share transfer.
+
+        :param transfer: ID or name of share transfer.
+        """
+        cmd = 'share-transfer-accept %s %s' % (transfer, auth_key)
+        self.manila(cmd, microversion=microversion)
+
     def list_shares(self, all_tenants=False, is_soft_deleted=False,
                     filters=None, columns=None, is_public=False,
                     microversion=None):
         """List shares.
 
         :param all_tenants: bool -- whether to list shares that belong
             only to current project or for all tenants.
@@ -999,14 +1051,34 @@
 
         :param share: str -- Name or ID of share
         """
         self.wait_for_resource_deletion(
             SHARE, res_id=share, interval=5, timeout=300,
             microversion=microversion)
 
+    def is_share_transfer_deleted(self, transfer, microversion=None):
+        """Says whether transfer is deleted or not.
+
+        :param transfer: str -- Name or ID of transfer
+        """
+        try:
+            self.get_transfer(transfer, microversion=microversion)
+            return False
+        except tempest_lib_exc.NotFound:
+            return True
+
+    def wait_for_transfer_deletion(self, transfer, microversion=None):
+        """Wait for transfer deletion by its Name or ID.
+
+        :param transfer: str -- Name or ID of transfer.
+        """
+        self.wait_for_resource_deletion(
+            SHARE, res_id=transfer, interval=5, timeout=300,
+            microversion=microversion)
+
     def wait_for_share_soft_deletion(self, share_id, microversion=None):
         body = self.get_share(share_id, microversion=microversion)
         is_soft_deleted = body['is_soft_deleted']
         start = int(time.time())
 
         while is_soft_deleted == "False":
             time.sleep(self.build_interval)
@@ -1513,64 +1585,70 @@
         if detail:
             cmd += ' --column name,host,backend,pool,capabilities'
         response = self.manila(cmd)
         return output_parser.listing(response)
 
     def create_security_service(self, type='ldap', name=None, description=None,
                                 dns_ip=None, ou=None, server=None, domain=None,
-                                user=None, password=None, microversion=None):
+                                user=None, password=None, default_ad_site=None,
+                                microversion=None):
         """Creates security service.
 
         :param type: security service type (ldap, kerberos or active_directory)
         :param name: desired name of new security service.
         :param description: desired description of new security service.
         :param dns_ip: DNS IP address inside tenant's network.
         :param ou: security service organizational unit
         :param server: security service IP address or hostname.
         :param domain: security service domain.
         :param user: user of the new security service.
         :param password: password used by user.
+        :param default_ad_site: default AD site
         """
 
         cmd = 'security-service-create %s ' % type
         cmd += self. _combine_security_service_data(
             name=name,
             description=description,
             dns_ip=dns_ip,
             ou=ou,
             server=server,
             domain=domain,
             user=user,
-            password=password)
+            password=password,
+            default_ad_site=default_ad_site)
 
         ss_raw = self.manila(cmd, microversion=microversion)
         security_service = output_parser.details(ss_raw)
         return security_service
 
     @not_found_wrapper
     def update_security_service(self, security_service, name=None,
                                 description=None, dns_ip=None, ou=None,
                                 server=None, domain=None, user=None,
-                                password=None, microversion=None):
+                                password=None, default_ad_site=None,
+                                microversion=None):
         cmd = 'security-service-update %s ' % security_service
         cmd += self. _combine_security_service_data(
             name=name,
             description=description,
             dns_ip=dns_ip,
             ou=ou,
             server=server,
             domain=domain,
             user=user,
-            password=password)
+            password=password,
+            default_ad_site=default_ad_site)
         return output_parser.details(
             self.manila(cmd, microversion=microversion))
 
     def _combine_security_service_data(self, name=None, description=None,
                                        dns_ip=None, ou=None, server=None,
-                                       domain=None, user=None, password=None):
+                                       domain=None, user=None, password=None,
+                                       default_ad_site=None):
         data = ''
         if name is not None:
             data += '--name %s ' % name
         if description is not None:
             data += '--description %s ' % description
         if dns_ip is not None:
             data += '--dns-ip %s ' % dns_ip
@@ -1580,14 +1658,16 @@
             data += '--server %s ' % server
         if domain is not None:
             data += '--domain %s ' % domain
         if user is not None:
             data += '--user %s ' % user
         if password is not None:
             data += '--password %s ' % password
+        if default_ad_site is not None:
+            data += '--default-ad-site %s ' % default_ad_site
         return data
 
     @not_found_wrapper
     def list_share_export_locations(self, share, columns=None,
                                     microversion=None):
         """List share export locations.
```

### Comparing `python-manilaclient-4.4.0/manilaclient/tests/functional/exceptions.py` & `python-manilaclient-4.5.0/manilaclient/tests/functional/exceptions.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/tests/functional/osc/base.py` & `python-manilaclient-4.5.0/manilaclient/tests/functional/osc/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -298,14 +298,22 @@
         if add_cleanup:
             self.addCleanup(
                 self.openstack,
                 f'share snapshot delete {snapshot_object["id"]} --wait')
 
         return snapshot_object
 
+    def create_share_transfer(self, share, name=None, client=None):
+
+        name = name or data_utils.rand_name('autotest_share_transfer_name')
+        cmd = (f'transfer create {share} --name {name} ')
+        transfer_object = self.dict_result('share', cmd, client=client)
+
+        return transfer_object
+
     def create_share_network(self, neutron_net_id=None,
                              neutron_subnet_id=None, name=None,
                              description=None, availability_zone=None,
                              add_cleanup=True):
         name = name or data_utils.rand_name('autotest_share_network_name')
         cmd = (f'network create --name {name} --description {description}')
         if neutron_net_id:
```

### Comparing `python-manilaclient-4.4.0/manilaclient/tests/functional/osc/test_availability_zones.py` & `python-manilaclient-4.5.0/manilaclient/tests/functional/osc/test_availability_zones.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/tests/functional/osc/test_messages.py` & `python-manilaclient-4.5.0/manilaclient/tests/functional/osc/test_messages.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/tests/functional/osc/test_share_access_rules.py` & `python-manilaclient-4.5.0/manilaclient/tests/functional/osc/test_share_access_rules.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/tests/functional/osc/test_share_group_type_access.py` & `python-manilaclient-4.5.0/manilaclient/tests/functional/osc/test_share_group_type_access.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/tests/functional/osc/test_share_limits.py` & `python-manilaclient-4.5.0/manilaclient/tests/functional/osc/test_share_limits.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/tests/functional/osc/test_share_network_subnets.py` & `python-manilaclient-4.5.0/manilaclient/tests/functional/osc/test_share_network_subnets.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/tests/functional/osc/test_share_networks.py` & `python-manilaclient-4.5.0/manilaclient/tests/functional/osc/test_share_networks.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/tests/functional/osc/test_share_pools.py` & `python-manilaclient-4.5.0/manilaclient/tests/functional/osc/test_share_pools.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/tests/functional/osc/test_share_replica_export_locations.py` & `python-manilaclient-4.5.0/manilaclient/tests/functional/osc/test_share_replica_export_locations.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/tests/functional/osc/test_share_replicas.py` & `python-manilaclient-4.5.0/manilaclient/tests/functional/osc/test_share_replicas.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/tests/functional/osc/test_share_services.py` & `python-manilaclient-4.5.0/manilaclient/tests/functional/osc/test_share_services.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/tests/functional/osc/test_share_snapshots.py` & `python-manilaclient-4.5.0/manilaclient/tests/functional/osc/test_share_snapshots.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/tests/functional/osc/test_share_types.py` & `python-manilaclient-4.5.0/manilaclient/tests/functional/osc/test_share_types.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/tests/functional/osc/test_shares.py` & `python-manilaclient-4.5.0/manilaclient/tests/functional/osc/test_shares.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/tests/functional/osc/test_shares_group_type.py` & `python-manilaclient-4.5.0/manilaclient/tests/functional/osc/test_shares_group_type.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/tests/functional/test_availability_zones.py` & `python-manilaclient-4.5.0/manilaclient/tests/functional/test_availability_zones.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/tests/functional/test_common.py` & `python-manilaclient-4.5.0/manilaclient/tests/functional/test_common.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/tests/functional/test_export_locations.py` & `python-manilaclient-4.5.0/manilaclient/tests/functional/test_export_locations.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/tests/functional/test_limits.py` & `python-manilaclient-4.5.0/manilaclient/tests/functional/test_limits.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/tests/functional/test_messages.py` & `python-manilaclient-4.5.0/manilaclient/tests/functional/test_messages.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/tests/functional/test_quotas.py` & `python-manilaclient-4.5.0/manilaclient/tests/functional/test_quotas.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/tests/functional/test_scheduler_stats.py` & `python-manilaclient-4.5.0/manilaclient/tests/functional/test_scheduler_stats.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/tests/functional/test_security_services.py` & `python-manilaclient-4.5.0/manilaclient/tests/functional/test_security_services.py`

 * *Files 15% similar despite different names*

```diff
@@ -28,29 +28,32 @@
         self.description = 'fake_description'
         self.user = 'fake_user'
         self.password = 'fake_password'
         self.server = 'fake_server'
         self.domain = 'fake_domain'
         self.dns_ip = '1.2.3.4'
         self.ou = 'fake_ou'
+        self.default_ad_site = 'fake_default_ad_site'
 
     @ddt.data(
         {'name': 'test_name'},
         {'description': 'test_description'},
         {'user': 'test_username'},
         {'password': 'test_password'},
         {'server': 'test_server'},
+        {'default_ad_site': 'test_default_ad_site'},
         {'domain': 'test_domain'},
         {'dns_ip': 'test_dns_ip'},
         {'ou': 'test_ou'},
         {'name': '""'},
         {'description': '""'},
         {'user': '""'},
         {'password': '""'},
         {'server': '""'},
+        {'default_ad_site': '""'},
         {'domain': '""'},
         {'dns_ip': '""'},
         {'ou': '""'},
     )
     def test_create_update_security_service(self, ss_data):
         expected_data = {
             'name': self.name,
@@ -59,14 +62,18 @@
             'password': self.password,
             'server': self.server,
             'domain': self.domain,
             'dns_ip': self.dns_ip,
             'ou': self.ou,
         }
 
+        if 'default_ad_site' in ss_data:
+            expected_data.pop('server')
+            expected_data['default_ad_site'] = self.default_ad_site
+
         ss = self.create_security_service(**expected_data)
         update = self.admin_client.update_security_service(ss['id'], **ss_data)
         expected_data.update(ss_data)
 
         for k, v in expected_data.items():
             if v == '""':
                 self.assertEqual('None', update[k])
```

### Comparing `python-manilaclient-4.4.0/manilaclient/tests/functional/test_services.py` & `python-manilaclient-4.5.0/manilaclient/tests/functional/test_services.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/tests/functional/test_share_access.py` & `python-manilaclient-4.5.0/manilaclient/tests/functional/test_share_access.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/tests/functional/test_share_network_subnets.py` & `python-manilaclient-4.5.0/manilaclient/tests/functional/test_share_network_subnets.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/tests/functional/test_share_networks.py` & `python-manilaclient-4.5.0/manilaclient/tests/functional/test_share_networks.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/tests/functional/test_share_replica_export_locations.py` & `python-manilaclient-4.5.0/manilaclient/tests/functional/test_share_replica_export_locations.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/tests/functional/test_share_replicas.py` & `python-manilaclient-4.5.0/manilaclient/tests/functional/test_share_replicas.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/tests/functional/test_share_servers.py` & `python-manilaclient-4.5.0/manilaclient/tests/functional/test_share_servers.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/tests/functional/test_share_types.py` & `python-manilaclient-4.5.0/manilaclient/tests/functional/test_share_types.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/tests/functional/test_shares.py` & `python-manilaclient-4.5.0/manilaclient/tests/functional/test_shares.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/tests/functional/test_shares_listing.py` & `python-manilaclient-4.5.0/manilaclient/tests/functional/test_shares_listing.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/tests/functional/test_shares_metadata.py` & `python-manilaclient-4.5.0/manilaclient/tests/functional/test_shares_metadata.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/tests/functional/test_snapshot_access.py` & `python-manilaclient-4.5.0/manilaclient/tests/functional/test_snapshot_access.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/tests/functional/test_snapshot_instances.py` & `python-manilaclient-4.5.0/manilaclient/tests/functional/test_snapshot_instances.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/tests/functional/test_snapshot_instances_export_locations.py` & `python-manilaclient-4.5.0/manilaclient/tests/functional/test_snapshot_instances_export_locations.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/tests/functional/test_snapshots_export_locations.py` & `python-manilaclient-4.5.0/manilaclient/tests/functional/test_snapshots_export_locations.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/tests/functional/utils.py` & `python-manilaclient-4.5.0/manilaclient/tests/functional/utils.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/tests/unit/common/test_httpclient.py` & `python-manilaclient-4.5.0/manilaclient/tests/unit/common/test_httpclient.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/tests/unit/fakes.py` & `python-manilaclient-4.5.0/manilaclient/tests/unit/fakes.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/tests/unit/osc/osc_fakes.py` & `python-manilaclient-4.5.0/manilaclient/tests/unit/osc/osc_fakes.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/tests/unit/osc/osc_utils.py` & `python-manilaclient-4.5.0/manilaclient/tests/unit/osc/osc_utils.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/tests/unit/osc/v2/fakes.py` & `python-manilaclient-4.5.0/manilaclient/tests/unit/osc/v2/fakes.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 class FakeShareClient(object):
 
     def __init__(self, **kwargs):
         super(FakeShareClient, self).__init__()
         self.auth_token = kwargs['token']
         self.management_url = kwargs['endpoint']
         self.shares = mock.Mock()
+        self.transfers = mock.Mock()
         self.share_access_rules = mock.Mock()
         self.share_groups = mock.Mock()
         self.share_types = mock.Mock()
         self.share_type_access = mock.Mock()
         self.quotas = mock.Mock()
         self.quota_classes = mock.Mock()
         self.share_snapshots = mock.Mock()
@@ -581,14 +582,72 @@
         for n in range(0, count):
             share_snapshots.append(
                 FakeShareSnapshot.create_one_snapshot(attrs))
 
         return share_snapshots
 
 
+class FakeShareTransfer(object):
+    """Fake a share transfer"""
+
+    @staticmethod
+    def create_one_transfer(attrs=None, methods=None):
+        """Create a fake share transfer
+
+        :param Dictionary attrs:
+            A dictionary with all attributes
+        :return:
+            A FakeResource object, with id, resource and so on
+        """
+
+        attrs = attrs or {}
+        methods = methods or {}
+        now_time = datetime.datetime.now()
+        delta_time = now_time + datetime.timedelta(minutes=5)
+
+        share_transfer = {
+            'accepted': 'False',
+            'auth_key': 'auth-key-' + uuid.uuid4().hex,
+            'created_at': now_time.isoformat(),
+            'destination_project_id': None,
+            'expires_at': delta_time.isoformat(),
+            'id': 'transfer-id-' + uuid.uuid4().hex,
+            'name': 'name-' + uuid.uuid4().hex,
+            'resource_id': 'resource-id-' + uuid.uuid4().hex,
+            'resource_type': 'share',
+            'source_project_id': 'source-project-id-' + uuid.uuid4().hex
+        }
+
+        share_transfer.update(attrs)
+        share_transfer = osc_fakes.FakeResource(info=copy.deepcopy(
+            share_transfer),
+            methods=methods,
+            loaded=True)
+        return share_transfer
+
+    @staticmethod
+    def create_share_transfers(attrs=None, count=2):
+        """Create multiple fake transfers.
+
+        :param Dictionary attrs:
+            A dictionary with all attributes
+        :param Integer count:
+            The number of share transfers to be faked
+        :return:
+            A list of FakeResource objects
+        """
+
+        share_transfers = []
+        for n in range(0, count):
+            share_transfers.append(
+                FakeShareSnapshot.create_one_snapshot(attrs))
+
+        return share_transfers
+
+
 class FakeSnapshotAccessRule(object):
     """Fake one or more snapshot access rules"""
 
     @staticmethod
     def create_one_access_rule(attrs={}):
         """Create a fake snapshot access rule
 
@@ -916,14 +975,15 @@
             "domain": 'fake.domain',
             "id": uuid.uuid4().hex,
             "name": 'name-' + uuid.uuid4().hex,
             "ou": 'fake_OU',
             "password": 'password',
             "project_id": uuid.uuid4().hex,
             "server": 'fake_hostname',
+            "default_ad_site": 'fake_default_ad_site',
             "status": 'new',
             "type": 'ldap',
             "updated_at": datetime.datetime.now().isoformat(),
             "user": 'fake_user',
         }
 
         share_security_service_info.update(attrs)
@@ -1187,14 +1247,15 @@
             "network_type": "vlan",
             "neutron_net_id": str(uuid.uuid4()),
             "neutron_subnet_id": str(uuid.uuid4()),
             "segmentation_id": 1010,
             "share_network_id": str(uuid.uuid4()),
             "share_network_name": str(uuid.uuid4()),
             "updated_at": datetime.datetime.now().isoformat(),
+            "properties": {},
         }
 
         share_network_subnet.update(attrs)
         share_network_subnet = osc_fakes.FakeResource(info=copy.deepcopy(
             share_network_subnet),
             loaded=True)
         return share_network_subnet
```

### Comparing `python-manilaclient-4.4.0/manilaclient/tests/unit/osc/v2/test_availability_zones.py` & `python-manilaclient-4.5.0/manilaclient/tests/unit/osc/v2/test_availability_zones.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/tests/unit/osc/v2/test_messages.py` & `python-manilaclient-4.5.0/manilaclient/tests/unit/osc/v2/test_messages.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/tests/unit/osc/v2/test_quotas.py` & `python-manilaclient-4.5.0/manilaclient/tests/unit/osc/v2/test_quotas.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/tests/unit/osc/v2/test_security_services.py` & `python-manilaclient-4.5.0/manilaclient/tests/unit/osc/v2/test_security_services.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 #
 #   Unless required by applicable law or agreed to in writing, software
 #   distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 #   WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 #   License for the specific language governing permissions and limitations
 #   under the License.
 #
+import ddt
 from osc_lib import exceptions
 from osc_lib import utils as oscutils
 
 from manilaclient import api_versions
 from manilaclient.osc.v2 import security_services as osc_security_services
 from manilaclient.tests.unit.osc import osc_utils
 from manilaclient.tests.unit.osc.v2 import fakes as manila_fakes
@@ -32,14 +33,15 @@
         self.share_networks_mock.reset_mock()
 
         self.app.client_manager.share.api_version = api_versions.APIVersion(
             api_versions.MAX_VERSION
         )
 
 
+@ddt.ddt
 class TestShareSecurityServiceCreate(TestShareSecurityService):
 
     def setUp(self):
         super(TestShareSecurityServiceCreate, self).setUp()
 
         self.security_service = manila_fakes.FakeShareSecurityService \
             .create_fake_security_service()
@@ -63,60 +65,73 @@
             '--dns-ip', self.security_service.dns_ip,
             '--ou', self.security_service.ou,
             '--server', self.security_service.server,
             '--domain', self.security_service.domain,
             '--user', self.security_service.user,
             '--password', self.security_service.password,
             '--name', self.security_service.name,
-            '--description', self.security_service.description
+            '--description', self.security_service.description,
+            '--default-ad-site', self.security_service.default_ad_site
         ]
         verifylist = [
             ('type', self.security_service.type),
             ('dns_ip', self.security_service.dns_ip),
             ('ou', self.security_service.ou),
             ('server', self.security_service.server),
             ('domain', self.security_service.domain),
             ('user', self.security_service.user),
             ('password', self.security_service.password),
             ('name', self.security_service.name),
-            ('description', self.security_service.description)
+            ('description', self.security_service.description),
+            ('default_ad_site', self.security_service.default_ad_site)
         ]
 
         parsed_args = self.check_parser(self.cmd, arglist, verifylist)
         columns, data = self.cmd.take_action(parsed_args)
 
         self.security_services_mock.create.assert_called_with(
             self.security_service.type,
             dns_ip=self.security_service.dns_ip,
             server=self.security_service.server,
             domain=self.security_service.domain,
             user=self.security_service.user,
             password=self.security_service.password,
             name=self.security_service.name,
             description=self.security_service.description,
-            ou=self.security_service.ou
+            ou=self.security_service.ou,
+            default_ad_site=self.security_service.default_ad_site
         )
 
         self.assertCountEqual(self.columns, columns)
         self.assertCountEqual(self.data, data)
 
-    def test_share_security_service_create_api_version_exception(self):
+    @ddt.data('2.43', '2.75')
+    def test_share_security_service_create_api_version_exception(self,
+                                                                 version):
         self.app.client_manager.share.api_version = api_versions.APIVersion(
-            '2.43'
+            version
         )
 
         arglist = [
             self.security_service.type,
-            '--ou', self.security_service.ou,
         ]
         verifylist = [
             ('type', self.security_service.type),
-            ('ou', self.security_service.ou),
         ]
 
+        if api_versions.APIVersion(version) <= api_versions.APIVersion("2.43"):
+            arglist.extend(['--ou', self.security_service.ou])
+            verifylist.append(('ou', self.security_service.ou))
+
+        if api_versions.APIVersion(version) <= api_versions.APIVersion("2.75"):
+            arglist.extend(['--default-ad-site',
+                           self.security_service.default_ad_site])
+            verifylist.append(('default_ad_site',
+                               self.security_service.default_ad_site))
+
         parsed_args = self.check_parser(self.cmd, arglist, verifylist)
         self.assertRaises(
             exceptions.CommandError, self.cmd.take_action, parsed_args)
 
 
 class TestShareSecurityServiceDelete(TestShareSecurityService):
 
@@ -211,14 +226,15 @@
             self.security_service.id
         )
 
         self.assertCountEqual(self.columns, columns)
         self.assertCountEqual(self.data, data)
 
 
+@ddt.ddt
 class TestShareSecurityServiceSet(TestShareSecurityService):
 
     def setUp(self):
         super(TestShareSecurityServiceSet, self).setUp()
 
         self.security_service = manila_fakes.FakeShareSecurityService \
             .create_fake_security_service(methods={'update': None})
@@ -239,40 +255,43 @@
             '--dns-ip', self.security_service.dns_ip,
             '--ou', self.security_service.ou,
             '--server', self.security_service.server,
             '--domain', self.security_service.domain,
             '--user', self.security_service.user,
             '--password', self.security_service.password,
             '--name', self.security_service.name,
-            '--description', self.security_service.description
+            '--description', self.security_service.description,
+            '--default-ad-site', self.security_service.default_ad_site
         ]
         verifylist = [
             ('security_service', self.security_service.id),
             ('dns_ip', self.security_service.dns_ip),
             ('ou', self.security_service.ou),
             ('server', self.security_service.server),
             ('domain', self.security_service.domain),
             ('user', self.security_service.user),
             ('password', self.security_service.password),
             ('name', self.security_service.name),
-            ('description', self.security_service.description)
+            ('description', self.security_service.description),
+            ('default_ad_site', self.security_service.default_ad_site)
         ]
 
         parsed_args = self.check_parser(self.cmd, arglist, verifylist)
         result = self.cmd.take_action(parsed_args)
 
         self.security_service.update.assert_called_with(
             dns_ip=self.security_service.dns_ip,
             server=self.security_service.server,
             domain=self.security_service.domain,
             user=self.security_service.user,
             password=self.security_service.password,
             name=self.security_service.name,
             description=self.security_service.description,
-            ou=self.security_service.ou
+            ou=self.security_service.ou,
+            default_ad_site=self.security_service.default_ad_site,
         )
         self.assertIsNone(result)
 
     def test_share_security_service_set_exception(self):
         arglist = [
             self.security_service.id,
             '--name', self.security_service.name,
@@ -285,33 +304,43 @@
         parsed_args = self.check_parser(self.cmd, arglist, verifylist)
 
         self.security_service.update.side_effect = \
             exceptions.CommandError()
         self.assertRaises(
             exceptions.CommandError, self.cmd.take_action, parsed_args)
 
-    def test_share_security_service_set_api_version_exception(self):
+    @ddt.data('2.43', '2.75')
+    def test_share_security_service_set_api_version_exception(self, version):
         self.app.client_manager.share.api_version = api_versions.APIVersion(
-            '2.43'
+            version
         )
 
         arglist = [
             self.security_service.id,
-            '--ou', self.security_service.ou,
         ]
         verifylist = [
             ('security_service', self.security_service.id),
-            ('ou', self.security_service.ou),
         ]
 
+        if api_versions.APIVersion(version) <= api_versions.APIVersion("2.43"):
+            arglist.extend(['--ou', self.security_service.ou])
+            verifylist.append(('ou', self.security_service.ou))
+
+        if api_versions.APIVersion(version) <= api_versions.APIVersion("2.75"):
+            arglist.extend(['--default-ad-site',
+                           self.security_service.default_ad_site])
+            verifylist.append(('default_ad_site',
+                               self.security_service.default_ad_site))
+
         parsed_args = self.check_parser(self.cmd, arglist, verifylist)
         self.assertRaises(
             exceptions.CommandError, self.cmd.take_action, parsed_args)
 
 
+@ddt.ddt
 class TestShareSecurityServiceUnset(TestShareSecurityService):
 
     def setUp(self):
         super(TestShareSecurityServiceUnset, self).setUp()
 
         self.security_service = manila_fakes.FakeShareSecurityService \
             .create_fake_security_service(methods={'update': None})
@@ -333,39 +362,42 @@
             '--ou',
             '--server',
             '--domain',
             '--user',
             '--password',
             '--name',
             '--description',
+            '--default-ad-site',
         ]
         verifylist = [
             ('security_service', self.security_service.id),
             ('dns_ip', True),
             ('ou', True),
             ('server', True),
             ('domain', True),
             ('user', True),
             ('password', True),
             ('name', True),
-            ('description', True)
+            ('description', True),
+            ('default_ad_site', True)
         ]
 
         parsed_args = self.check_parser(self.cmd, arglist, verifylist)
         result = self.cmd.take_action(parsed_args)
 
         self.security_service.update.assert_called_with(
             dns_ip='',
             server='',
             domain='',
             user='',
             password='',
             name='',
             description='',
-            ou=''
+            ou='',
+            default_ad_site=''
         )
         self.assertIsNone(result)
 
     def test_share_security_service_unset_exception(self):
         arglist = [
             self.security_service.id,
             '--name',
@@ -378,28 +410,36 @@
         parsed_args = self.check_parser(self.cmd, arglist, verifylist)
 
         self.security_service.update.side_effect = \
             exceptions.CommandError()
         self.assertRaises(
             exceptions.CommandError, self.cmd.take_action, parsed_args)
 
-    def test_share_security_service_unset_api_version_exception(self):
+    @ddt.data('2.43', '2.75')
+    def test_share_security_service_unset_api_version_exception(self,
+                                                                version):
         self.app.client_manager.share.api_version = api_versions.APIVersion(
-            '2.43'
+            version
         )
 
         arglist = [
             self.security_service.id,
-            '--ou',
         ]
         verifylist = [
             ('security_service', self.security_service.id),
-            ('ou', True),
         ]
 
+        if api_versions.APIVersion(version) <= api_versions.APIVersion("2.43"):
+            arglist.extend(['--ou'])
+            verifylist.append(('ou', True))
+
+        if api_versions.APIVersion(version) <= api_versions.APIVersion("2.75"):
+            arglist.extend(['--default-ad-site']),
+            verifylist.append(('default_ad_site', True))
+
         parsed_args = self.check_parser(self.cmd, arglist, verifylist)
         self.assertRaises(
             exceptions.CommandError, self.cmd.take_action, parsed_args)
 
 
 class TestShareSecurityServiceList(TestShareSecurityService):
 
@@ -456,26 +496,28 @@
             '--name', self.services_list[0].name,
             '--type', self.services_list[0].type,
             '--user', self.services_list[0].user,
             '--dns-ip', self.services_list[0].dns_ip,
             '--ou', self.services_list[0].ou,
             '--server', self.services_list[0].server,
             '--domain', self.services_list[0].domain,
+            '--default-ad-site', self.services_list[0].default_ad_site,
             '--limit', '1',
         ]
         verifylist = [
             ('share_network', self.share_network.id),
             ('status', self.services_list[0].status),
             ('name', self.services_list[0].name),
             ('type', self.services_list[0].type),
             ('user', self.services_list[0].user),
             ('dns_ip', self.services_list[0].dns_ip),
             ('ou', self.services_list[0].ou),
             ('server', self.services_list[0].server),
             ('domain', self.services_list[0].domain),
+            ('default_ad_site', self.services_list[0].default_ad_site),
             ('limit', 1),
         ]
         parsed_args = self.check_parser(self.cmd, arglist, verifylist)
 
         columns, data = self.cmd.take_action(parsed_args)
 
         self.security_services_mock.list.assert_called_with(
@@ -484,14 +526,15 @@
                 'status': self.services_list[0].status,
                 'name': self.services_list[0].name,
                 'type': self.services_list[0].type,
                 'user': self.services_list[0].user,
                 'dns_ip': self.services_list[0].dns_ip,
                 'server': self.services_list[0].server,
                 'domain': self.services_list[0].domain,
+                'default_ad_site': self.services_list[0].default_ad_site,
                 'offset': None,
                 'limit': 1,
                 'ou': self.services_list[0].ou,
                 'share_network_id': self.share_network.id,
             },
             detailed=False)
 
@@ -509,14 +552,29 @@
             ('ou', self.services_list[0].ou),
         ]
         parsed_args = self.check_parser(self.cmd, arglist, verifylist)
 
         self.assertRaises(
             exceptions.CommandError, self.cmd.take_action, parsed_args)
 
+    def test_share_security_service_list_ad_site_api_version_exception(self):
+        self.app.client_manager.share.api_version = api_versions.APIVersion(
+            '2.75'
+        )
+        arglist = [
+            '--default-ad-site', self.services_list[0].default_ad_site,
+        ]
+        verifylist = [
+            ('default_ad_site', self.services_list[0].default_ad_site),
+        ]
+        parsed_args = self.check_parser(self.cmd, arglist, verifylist)
+
+        self.assertRaises(
+            exceptions.CommandError, self.cmd.take_action, parsed_args)
+
     def test_share_security_service_list_detail_all_projects(self):
         arglist = [
             '--all-projects',
             '--detail'
         ]
         verifylist = [
             ('all_projects', True),
```

### Comparing `python-manilaclient-4.4.0/manilaclient/tests/unit/osc/v2/test_services.py` & `python-manilaclient-4.5.0/manilaclient/tests/unit/osc/v2/test_services.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/tests/unit/osc/v2/test_share.py` & `python-manilaclient-4.5.0/manilaclient/tests/unit/osc/v2/test_share.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/tests/unit/osc/v2/test_share_access_rules.py` & `python-manilaclient-4.5.0/manilaclient/tests/unit/osc/v2/test_share_access_rules.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/tests/unit/osc/v2/test_share_group_snapshots.py` & `python-manilaclient-4.5.0/manilaclient/tests/unit/osc/v2/test_share_group_snapshots.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/tests/unit/osc/v2/test_share_group_type.py` & `python-manilaclient-4.5.0/manilaclient/tests/unit/osc/v2/test_share_group_type.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/tests/unit/osc/v2/test_share_group_type_access.py` & `python-manilaclient-4.5.0/manilaclient/tests/unit/osc/v2/test_share_group_type_access.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/tests/unit/osc/v2/test_share_groups.py` & `python-manilaclient-4.5.0/manilaclient/tests/unit/osc/v2/test_share_groups.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/tests/unit/osc/v2/test_share_instance_export_locations.py` & `python-manilaclient-4.5.0/manilaclient/tests/unit/osc/v2/test_share_instance_export_locations.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/tests/unit/osc/v2/test_share_instances.py` & `python-manilaclient-4.5.0/manilaclient/tests/unit/osc/v2/test_share_instances.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/tests/unit/osc/v2/test_share_limits.py` & `python-manilaclient-4.5.0/manilaclient/tests/unit/osc/v2/test_share_limits.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/tests/unit/osc/v2/test_share_network_subnets.py` & `python-manilaclient-4.5.0/manilaclient/tests/unit/osc/v2/test_share_network_subnets.py`

 * *Files 27% similar despite different names*

```diff
@@ -82,15 +82,16 @@
 
         columns, data = self.cmd.take_action(parsed_args)
 
         self.share_subnets_mock.create.assert_called_once_with(
             neutron_net_id=fake_neutron_net_id,
             neutron_subnet_id=fake_neutron_subnet_id,
             availability_zone='nova',
-            share_network_id=self.share_network.id
+            share_network_id=self.share_network.id,
+            metadata={}
         )
 
         self.assertCountEqual(self.columns, columns)
         self.assertCountEqual(self.data, data)
 
     def test_share_network_subnet_create_arg_group_exception(self):
         fake_neutron_net_id = str(uuid.uuid4())
@@ -159,14 +160,59 @@
 
         (self.share_networks_mock.share_network_subnet_create_check
          .assert_called_once_with(
              share_network_id=self.share_network.id, neutron_net_id=None,
              neutron_subnet_id=None, availability_zone=None,
              reset_operation=restart_check))
 
+    def test_share_network_subnet_create_metadata(self):
+        self.app.client_manager.share.api_version = api_versions.APIVersion(
+            '2.78'
+        )
+        arglist = [
+            self.share_network.id,
+            '--property', 'Manila=zorilla',
+            '--property', 'Zorilla=manila'
+        ]
+        verifylist = [
+            ('share_network', self.share_network.id),
+            ('property', {'Manila': 'zorilla', 'Zorilla': 'manila'}),
+        ]
+
+        parsed_args = self.check_parser(self.cmd, arglist, verifylist)
+
+        columns, data = self.cmd.take_action(parsed_args)
+
+        self.share_subnets_mock.create.assert_called_once_with(
+            neutron_net_id=None,
+            neutron_subnet_id=None,
+            availability_zone=None,
+            share_network_id=self.share_network.id,
+            metadata={'Manila': 'zorilla', 'Zorilla': 'manila'},
+        )
+        self.assertEqual(set(self.columns), set(columns))
+        self.assertCountEqual(self.data, data)
+
+    def test_share_network_subnet_create_metadata_api_version_exception(self):
+        self.app.client_manager.share.api_version = api_versions.APIVersion(
+            '2.77'
+        )
+        arglist = [
+            self.share_network.id,
+            '--property', 'Manila=zorilla',
+        ]
+        verifylist = [
+            ('share_network', self.share_network.id),
+            ('property', {'Manila': 'zorilla'})
+        ]
+        parsed_args = self.check_parser(self.cmd, arglist, verifylist)
+
+        self.assertRaises(
+            exceptions.CommandError, self.cmd.take_action, parsed_args)
+
 
 class TestShareNetworkSubnetDelete(TestShareNetworkSubnet):
 
     def setUp(self):
         super(TestShareNetworkSubnetDelete, self).setUp()
 
         self.share_network = (
@@ -265,7 +311,146 @@
         self.share_subnets_mock.get.assert_called_once_with(
             self.share_network.id,
             self.share_network_subnet.id
         )
 
         self.assertCountEqual(self.columns, columns)
         self.assertCountEqual(self.data, data)
+
+
+class TestShareNetworkSubnetSet(TestShareNetworkSubnet):
+
+    def setUp(self):
+        super(TestShareNetworkSubnetSet, self).setUp()
+
+        self.share_network = (
+            manila_fakes.FakeShareNetwork.create_one_share_network())
+        self.share_networks_mock.get.return_value = self.share_network
+
+        self.share_network_subnet = (
+            manila_fakes.FakeShareNetworkSubnet.create_one_share_subnet())
+
+        self.cmd = osc_share_subnets.SetShareNetworkSubnet(
+            self.app, None)
+
+    def test_set_share_network_subnet_property(self):
+        self.app.client_manager.share.api_version = api_versions.APIVersion(
+            '2.78'
+        )
+        arglist = [
+            self.share_network.id,
+            self.share_network_subnet.id,
+            '--property', 'Zorilla=manila',
+            '--property', 'test=my_test',
+        ]
+        verifylist = [
+            ('share_network', self.share_network.id),
+            ('share_network_subnet', self.share_network_subnet.id),
+            ('property', {'Zorilla': 'manila', 'test': 'my_test'}),
+        ]
+        parsed_args = self.check_parser(self.cmd, arglist, verifylist)
+
+        self.cmd.take_action(parsed_args)
+
+        self.share_subnets_mock.set_metadata.assert_called_once_with(
+            self.share_network.id, {'Zorilla': 'manila', 'test': 'my_test'},
+            subresource=self.share_network_subnet.id)
+
+    def test_set_share_network_subnet_property_exception(self):
+        self.app.client_manager.share.api_version = api_versions.APIVersion(
+            '2.78'
+        )
+        arglist = [
+            self.share_network.id,
+            self.share_network_subnet.id,
+            '--property', 'key=1',
+        ]
+        verifylist = [
+            ('share_network', self.share_network.id),
+            ('share_network_subnet', self.share_network_subnet.id),
+            ('property', {'key': '1'}),
+        ]
+
+        parsed_args = self.check_parser(self.cmd, arglist, verifylist)
+
+        self.cmd.take_action(parsed_args)
+
+        self.share_subnets_mock.set_metadata.assert_called_once_with(
+            self.share_network.id, {'key': '1'},
+            subresource=self.share_network_subnet.id)
+
+        self.share_subnets_mock.set_metadata.side_effect = (
+            exceptions.BadRequest)
+        self.assertRaises(
+            exceptions.CommandError, self.cmd.take_action,
+            parsed_args)
+
+
+class TestShareNetworkSubnetUnset(TestShareNetworkSubnet):
+
+    def setUp(self):
+        super(TestShareNetworkSubnetUnset, self).setUp()
+
+        self.share_network = (
+            manila_fakes.FakeShareNetwork.create_one_share_network())
+        self.share_networks_mock.get.return_value = self.share_network
+
+        self.share_network_subnet = (
+            manila_fakes.FakeShareNetworkSubnet.create_one_share_subnet())
+
+        self.cmd = osc_share_subnets.UnsetShareNetworkSubnet(
+            self.app, None)
+
+    def test_unset_share_network_subnet_property(self):
+        self.app.client_manager.share.api_version = api_versions.APIVersion(
+            '2.78'
+        )
+        arglist = [
+            self.share_network.id,
+            self.share_network_subnet.id,
+            '--property', 'Manila',
+        ]
+        verifylist = [
+            ('share_network', self.share_network.id),
+            ('share_network_subnet', self.share_network_subnet.id),
+            ('property', ['Manila']),
+        ]
+
+        parsed_args = self.check_parser(self.cmd, arglist, verifylist)
+
+        self.cmd.take_action(parsed_args)
+
+        self.share_subnets_mock.delete_metadata.assert_called_once_with(
+            self.share_network.id, ['Manila'],
+            subresource=self.share_network_subnet.id)
+
+    def test_unset_share_network_subnet_property_exception(self):
+        self.app.client_manager.share.api_version = api_versions.APIVersion(
+            '2.78'
+        )
+        arglist = [
+            self.share_network.id,
+            self.share_network_subnet.id,
+            '--property', 'Manila',
+            '--property', 'test',
+        ]
+        verifylist = [
+            ('share_network', self.share_network.id),
+            ('share_network_subnet', self.share_network_subnet.id),
+            ('property', ['Manila', 'test']),
+        ]
+
+        parsed_args = self.check_parser(self.cmd, arglist, verifylist)
+
+        self.cmd.take_action(parsed_args)
+
+        self.share_subnets_mock.delete_metadata.assert_has_calls([
+            mock.call(self.share_network.id, ['Manila'],
+                      subresource=self.share_network_subnet.id),
+            mock.call(self.share_network.id, ['test'],
+                      subresource=self.share_network_subnet.id)])
+
+        # 404 Not Found would be raised, if property 'Manila' doesn't exist.
+        self.share_subnets_mock.delete_metadata.side_effect = (
+            exceptions.NotFound)
+        self.assertRaises(
+            exceptions.CommandError, self.cmd.take_action, parsed_args)
```

### Comparing `python-manilaclient-4.4.0/manilaclient/tests/unit/osc/v2/test_share_networks.py` & `python-manilaclient-4.5.0/manilaclient/tests/unit/osc/v2/test_share_networks.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/tests/unit/osc/v2/test_share_pools.py` & `python-manilaclient-4.5.0/manilaclient/tests/unit/osc/v2/test_share_pools.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/tests/unit/osc/v2/test_share_replica_export_locations.py` & `python-manilaclient-4.5.0/manilaclient/tests/unit/osc/v2/test_share_replica_export_locations.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/tests/unit/osc/v2/test_share_replicas.py` & `python-manilaclient-4.5.0/manilaclient/tests/unit/osc/v2/test_share_replicas.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/tests/unit/osc/v2/test_share_servers.py` & `python-manilaclient-4.5.0/manilaclient/tests/unit/osc/v2/test_share_servers.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/tests/unit/osc/v2/test_share_snapshot_instance_export_locations.py` & `python-manilaclient-4.5.0/manilaclient/tests/unit/osc/v2/test_share_snapshot_instance_export_locations.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/tests/unit/osc/v2/test_share_snapshot_instances.py` & `python-manilaclient-4.5.0/manilaclient/tests/unit/osc/v2/test_share_snapshot_instances.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/tests/unit/osc/v2/test_share_snapshots.py` & `python-manilaclient-4.5.0/manilaclient/tests/unit/osc/v2/test_share_snapshots.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/tests/unit/osc/v2/test_share_type.py` & `python-manilaclient-4.5.0/manilaclient/tests/unit/osc/v2/test_share_type.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/tests/unit/osc/v2/test_share_type_access.py` & `python-manilaclient-4.5.0/manilaclient/tests/unit/osc/v2/test_share_type_access.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/tests/unit/test_api_versions.py` & `python-manilaclient-4.5.0/manilaclient/tests/unit/test_api_versions.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/tests/unit/test_base.py` & `python-manilaclient-4.5.0/manilaclient/tests/unit/test_base.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/tests/unit/test_client.py` & `python-manilaclient-4.5.0/manilaclient/tests/unit/test_client.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/tests/unit/test_functional_utils.py` & `python-manilaclient-4.5.0/manilaclient/tests/unit/test_functional_utils.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/tests/unit/test_shell.py` & `python-manilaclient-4.5.0/manilaclient/tests/unit/test_shell.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/tests/unit/utils.py` & `python-manilaclient-4.5.0/manilaclient/tests/unit/utils.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/tests/unit/v1/test_limits.py` & `python-manilaclient-4.5.0/manilaclient/tests/unit/v1/test_limits.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/tests/unit/v1/test_quota_classes.py` & `python-manilaclient-4.5.0/manilaclient/tests/unit/v1/test_quota_classes.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/tests/unit/v1/test_quotas.py` & `python-manilaclient-4.5.0/manilaclient/tests/unit/v1/test_quotas.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/tests/unit/v1/test_scheduler_stats.py` & `python-manilaclient-4.5.0/manilaclient/tests/unit/v1/test_scheduler_stats.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/tests/unit/v1/test_security_services.py` & `python-manilaclient-4.5.0/manilaclient/tests/unit/v1/test_security_services.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/tests/unit/v1/test_services.py` & `python-manilaclient-4.5.0/manilaclient/tests/unit/v1/test_services.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/tests/unit/v1/test_share_networks.py` & `python-manilaclient-4.5.0/manilaclient/tests/unit/v1/test_share_networks.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/tests/unit/v1/test_share_servers.py` & `python-manilaclient-4.5.0/manilaclient/tests/unit/v1/test_share_servers.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/tests/unit/v1/test_share_snapshots.py` & `python-manilaclient-4.5.0/manilaclient/tests/unit/v1/test_share_snapshots.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/tests/unit/v1/test_share_type_access.py` & `python-manilaclient-4.5.0/manilaclient/tests/unit/v1/test_share_type_access.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/tests/unit/v1/test_share_types.py` & `python-manilaclient-4.5.0/manilaclient/tests/unit/v1/test_share_types.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/tests/unit/v1/test_shares.py` & `python-manilaclient-4.5.0/manilaclient/tests/unit/v1/test_shares.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/tests/unit/v2/fake_clients.py` & `python-manilaclient-4.5.0/manilaclient/tests/unit/v2/fake_clients.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/tests/unit/v2/fakes.py` & `python-manilaclient-4.5.0/manilaclient/tests/unit/v2/fakes.py`

 * *Files 5% similar despite different names*

```diff
@@ -1313,14 +1313,27 @@
         'resource_type': 'SHARE',
         'resource_id': 'resource id',
         'created_at': '2015-08-27T09:49:58-05:00',
         'expires_at': '2015-09-27T09:49:58-05:00',
         'request_id': 'req-936666d2-4c8f-4e41-9ac9-237b43f8b848',
     }
 
+    fake_transfer = {
+        "id": "f21c72c4-2b77-445b-aa12-e8d1b44163a2",
+        "created_at": "2022-09-06T08:17:43.629495",
+        "name": "test_transfer",
+        "resource_type": "share",
+        "resource_id": "29476819-28a9-4b1a-a21d-3b2d203025a0",
+        "auth_key": "406a2d67cdb09afe",
+        "source_project_id": "714198c7ac5e45a4b785de732ea4695d",
+        "destination_project_id": None,
+        "accepted": False,
+        "expires_at": None,
+    }
+
     def get_messages(self, **kw):
         messages = {
             'messages': [self.fake_message],
         }
         return 200, {}, messages
 
     def get_messages_1234(self, **kw):
@@ -1329,14 +1342,33 @@
 
     def delete_messages_1234(self, **kw):
         return 202, {}, None
 
     def delete_messages_5678(self, **kw):
         return 202, {}, None
 
+    def post_share_transfers(self, **kw):
+        transfer = {'transfer': self.fake_transfer}
+        return 202, {}, transfer
+
+    def get_share_transfers_5678(self, **kw):
+        transfer = {'transfer': self.fake_transfer}
+        return 202, {}, transfer
+
+    def get_share_transfers_detail(self, **kw):
+        transfer = {'transfers': [self.fake_transfer]}
+        return 202, {}, transfer
+
+    def delete_share_transfers_5678(self, **kw):
+        return 202, {}, None
+
+    def post_share_transfers_5678_accept(self, **kw):
+        transfer = {'transfer': self.fake_transfer}
+        return 202, {}, transfer
+
 
 def fake_create(url, body, response_key):
     return {'url': url, 'body': body, 'resp_key': response_key}
 
 
 def fake_update(url, body, response_key):
     return {'url': url, 'body': body, 'resp_key': response_key}
```

### Comparing `python-manilaclient-4.4.0/manilaclient/tests/unit/v2/test_availability_zones.py` & `python-manilaclient-4.5.0/manilaclient/tests/unit/v2/test_availability_zones.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/tests/unit/v2/test_client.py` & `python-manilaclient-4.5.0/manilaclient/tests/unit/v2/test_client.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/tests/unit/v2/test_limits.py` & `python-manilaclient-4.5.0/manilaclient/tests/unit/v2/test_limits.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/tests/unit/v2/test_messages.py` & `python-manilaclient-4.5.0/manilaclient/tests/unit/v2/test_messages.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/tests/unit/v2/test_quota_classes.py` & `python-manilaclient-4.5.0/manilaclient/tests/unit/v2/test_quota_classes.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/tests/unit/v2/test_quotas.py` & `python-manilaclient-4.5.0/manilaclient/tests/unit/v2/test_quotas.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/tests/unit/v2/test_scheduler_stats.py` & `python-manilaclient-4.5.0/manilaclient/tests/unit/v2/test_scheduler_stats.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/tests/unit/v2/test_security_services.py` & `python-manilaclient-4.5.0/manilaclient/tests/unit/v2/test_security_services.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,20 +11,23 @@
 #    distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 #    WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 #    License for the specific language governing permissions and limitations
 #    under the License.
 
 from unittest import mock
 
+import ddt
+
 from manilaclient import exceptions
 from manilaclient.tests.unit import utils
 from manilaclient.tests.unit.v2 import fakes
 from manilaclient.v2 import security_services
 
 
+@ddt.ddt
 class SecurityServiceTest(utils.TestCase):
 
     class _FakeSecurityService(object):
         id = 'fake_security_service_id'
 
     def setUp(self):
         super(SecurityServiceTest, self).setUp()
@@ -47,14 +50,39 @@
         with mock.patch.object(self.manager, '_create', fakes.fake_create):
             result = self.manager.create(**values)
 
             self.assertEqual(result['url'], security_services.RESOURCES_PATH)
             self.assertEqual(result['resp_key'],
                              security_services.RESOURCE_NAME)
             self.assertIn(security_services.RESOURCE_NAME, result['body'])
+            self.assertEqual(result['body'][security_services.RESOURCE_NAME],
+                             values)
+
+    @ddt.data({'server': 'fake.ad.server'},
+              {'default_ad_site': 'fake.ad.default_ad_site'})
+    def test_create_all_fields_active_directory(self, option):
+        values = {
+            'type': 'active_directory',
+            'dns_ip': 'fake dns ip',
+            'ou': 'fake ou',
+            'domain': 'fake.ad.domain',
+            'user': 'fake user',
+            'password': 'fake password',
+            'name': 'fake name',
+            'description': 'fake description',
+        }
+
+        values.update(option)
+        with mock.patch.object(self.manager, '_create', fakes.fake_create):
+            result = self.manager.create(**values)
+
+            self.assertEqual(result['url'], security_services.RESOURCES_PATH)
+            self.assertEqual(result['resp_key'],
+                             security_services.RESOURCE_NAME)
+            self.assertIn(security_services.RESOURCE_NAME, result['body'])
             self.assertEqual(result['body'][security_services.RESOURCE_NAME],
                              values)
 
     def test_create_some_fields(self):
         values = {
             'type': 'ldap',
             'dns_ip': 'fake dns ip',
```

### Comparing `python-manilaclient-4.4.0/manilaclient/tests/unit/v2/test_services.py` & `python-manilaclient-4.5.0/manilaclient/tests/unit/v2/test_services.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/tests/unit/v2/test_share_export_locations.py` & `python-manilaclient-4.5.0/manilaclient/tests/unit/v2/test_share_export_locations.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/tests/unit/v2/test_share_group_snapshots.py` & `python-manilaclient-4.5.0/manilaclient/tests/unit/v2/test_share_group_snapshots.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/tests/unit/v2/test_share_group_type_access.py` & `python-manilaclient-4.5.0/manilaclient/tests/unit/v2/test_share_group_type_access.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/tests/unit/v2/test_share_group_types.py` & `python-manilaclient-4.5.0/manilaclient/tests/unit/v2/test_share_group_types.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/tests/unit/v2/test_share_groups.py` & `python-manilaclient-4.5.0/manilaclient/tests/unit/v2/test_share_groups.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/tests/unit/v2/test_share_instance_export_locations.py` & `python-manilaclient-4.5.0/manilaclient/tests/unit/v2/test_share_instance_export_locations.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/tests/unit/v2/test_share_instances.py` & `python-manilaclient-4.5.0/manilaclient/tests/unit/v2/test_share_instances.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/tests/unit/v2/test_share_network_subnets.py` & `python-manilaclient-4.5.0/manilaclient/tests/unit/v2/test_share_network_subnets.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,14 +35,15 @@
         expected_url = share_network_subnets.RESOURCES_PATH % {
             'share_network_id': share_network_id
         }
         expected_values = {
             'neutron_net_id': 'fake_net_id',
             'neutron_subnet_id': 'fake_subnet_id',
             'availability_zone': 'fake_availability_zone',
+            'metadata': 'fake_metadata'
         }
         expected_body = {'share-network-subnet': expected_values}
         payload = expected_values.copy()
         payload.update({'share_network_id': share_network_id})
 
         with mock.patch.object(self.manager, '_create', fakes.fake_create):
             result = self.manager.create(**payload)
```

### Comparing `python-manilaclient-4.4.0/manilaclient/tests/unit/v2/test_share_networks.py` & `python-manilaclient-4.5.0/manilaclient/tests/unit/v2/test_share_networks.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/tests/unit/v2/test_share_replica_export_locations.py` & `python-manilaclient-4.5.0/manilaclient/tests/unit/v2/test_share_replica_export_locations.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/tests/unit/v2/test_share_replicas.py` & `python-manilaclient-4.5.0/manilaclient/tests/unit/v2/test_share_replicas.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/tests/unit/v2/test_share_servers.py` & `python-manilaclient-4.5.0/manilaclient/tests/unit/v2/test_share_servers.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/tests/unit/v2/test_share_snapshot_export_locations.py` & `python-manilaclient-4.5.0/manilaclient/tests/unit/v2/test_share_snapshot_export_locations.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/tests/unit/v2/test_share_snapshot_instance_export_locations.py` & `python-manilaclient-4.5.0/manilaclient/tests/unit/v2/test_share_snapshot_instance_export_locations.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/tests/unit/v2/test_share_snapshot_instances.py` & `python-manilaclient-4.5.0/manilaclient/tests/unit/v2/test_share_snapshot_instances.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/tests/unit/v2/test_share_snapshots.py` & `python-manilaclient-4.5.0/manilaclient/tests/unit/v2/test_share_snapshots.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/tests/unit/v2/test_shares.py` & `python-manilaclient-4.5.0/manilaclient/tests/unit/v2/test_shares.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/tests/unit/v2/test_shell.py` & `python-manilaclient-4.5.0/manilaclient/tests/unit/v2/test_shell.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/tests/unit/v2/test_type_access.py` & `python-manilaclient-4.5.0/manilaclient/tests/unit/v2/test_type_access.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/tests/unit/v2/test_types.py` & `python-manilaclient-4.5.0/manilaclient/tests/unit/v2/test_types.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/utils.py` & `python-manilaclient-4.5.0/manilaclient/utils.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/v1/__init__.py` & `python-manilaclient-4.5.0/manilaclient/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/v1/client.py` & `python-manilaclient-4.5.0/manilaclient/v1/client.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/v1/contrib/list_extensions.py` & `python-manilaclient-4.5.0/manilaclient/v1/contrib/list_extensions.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/v1/limits.py` & `python-manilaclient-4.5.0/manilaclient/v1/limits.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/v1/quota_classes.py` & `python-manilaclient-4.5.0/manilaclient/v1/quota_classes.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/v1/quotas.py` & `python-manilaclient-4.5.0/manilaclient/v1/quotas.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/v1/scheduler_stats.py` & `python-manilaclient-4.5.0/manilaclient/v1/scheduler_stats.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/v1/security_services.py` & `python-manilaclient-4.5.0/manilaclient/v1/security_services.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/v1/services.py` & `python-manilaclient-4.5.0/manilaclient/v1/services.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/v1/share_networks.py` & `python-manilaclient-4.5.0/manilaclient/v1/share_networks.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/v1/share_servers.py` & `python-manilaclient-4.5.0/manilaclient/v1/share_servers.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/v1/share_snapshots.py` & `python-manilaclient-4.5.0/manilaclient/v1/share_snapshots.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/v1/share_type_access.py` & `python-manilaclient-4.5.0/manilaclient/v1/share_type_access.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/v1/share_types.py` & `python-manilaclient-4.5.0/manilaclient/v1/share_types.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/v1/shares.py` & `python-manilaclient-4.5.0/manilaclient/v1/shares.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/v2/__init__.py` & `python-manilaclient-4.5.0/manilaclient/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/v2/availability_zones.py` & `python-manilaclient-4.5.0/manilaclient/v2/availability_zones.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/v2/client.py` & `python-manilaclient-4.5.0/manilaclient/v2/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,14 +39,15 @@
 from manilaclient.v2 import share_replica_export_locations
 from manilaclient.v2 import share_replicas
 from manilaclient.v2 import share_servers
 from manilaclient.v2 import share_snapshot_export_locations
 from manilaclient.v2 import share_snapshot_instance_export_locations
 from manilaclient.v2 import share_snapshot_instances
 from manilaclient.v2 import share_snapshots
+from manilaclient.v2 import share_transfers
 from manilaclient.v2 import share_type_access
 from manilaclient.v2 import share_types
 from manilaclient.v2 import shares
 
 
 class Client(object):
     """Top-level object to access the OpenStack Manila API.
@@ -185,14 +186,15 @@
                                             retries=retries,
                                             http_log_debug=http_log_debug,
                                             api_version=self.api_version)
 
         self.availability_zones = availability_zones.AvailabilityZoneManager(
             self)
         self.limits = limits.LimitsManager(self)
+        self.transfers = share_transfers.ShareTransferManager(self)
         self.messages = messages.MessageManager(self)
         self.services = services.ServiceManager(self)
         self.security_services = security_services.SecurityServiceManager(self)
         self.share_networks = share_networks.ShareNetworkManager(self)
         self.share_network_subnets = (
             share_network_subnets.ShareNetworkSubnetManager(self))
```

### Comparing `python-manilaclient-4.4.0/manilaclient/v2/contrib/list_extensions.py` & `python-manilaclient-4.5.0/manilaclient/v2/contrib/list_extensions.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/v2/limits.py` & `python-manilaclient-4.5.0/manilaclient/v2/limits.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/v2/messages.py` & `python-manilaclient-4.5.0/manilaclient/v2/messages.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/v2/quota_classes.py` & `python-manilaclient-4.5.0/manilaclient/v2/quota_classes.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/v2/quotas.py` & `python-manilaclient-4.5.0/manilaclient/v2/quotas.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/v2/scheduler_stats.py` & `python-manilaclient-4.5.0/manilaclient/v2/scheduler_stats.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/v2/security_services.py` & `python-manilaclient-4.5.0/manilaclient/v2/security_services.py`

 * *Files 27% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 #
 #    Unless required by applicable law or agreed to in writing, software
 #    distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 #    WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 #    License for the specific language governing permissions and limitations
 #    under the License.
 
+from manilaclient import api_versions
 from manilaclient import base
 from manilaclient import exceptions
 
 RESOURCES_PATH = '/security-services'
 RESOURCE_PATH = "/security-services/%s"
 RESOURCE_NAME = 'security_service'
 RESOURCES_NAME = 'security_services'
@@ -37,14 +38,15 @@
 
 
 class SecurityServiceManager(base.ManagerWithFind):
     """Manage :class:`SecurityService` resources."""
 
     resource_class = SecurityService
 
+    @api_versions.wraps("1.0", "2.75")
     def create(self, type, dns_ip=None, ou=None, server=None, domain=None,
                user=None, password=None, name=None,
                description=None):
         """Create security service for NAS.
 
         :param type: security service type - 'ldap', 'kerberos' or
                      'active_directory'
@@ -54,14 +56,50 @@
         :param domain: security service domain
         :param user: security identifier used by tenant
         :param password: password used by user
         :param name: security service name
         :param description: security service description
         :rtype: :class:`SecurityService`
         """
+        return self._create_security_service(type, dns_ip=dns_ip, ou=ou,
+                                             server=server, domain=domain,
+                                             user=user, password=password,
+                                             name=name,
+                                             description=description)
+
+    @api_versions.wraps("2.76")  # noqa
+    def create(self, type, dns_ip=None, ou=None, server=None,   # noqa
+               domain=None, user=None, password=None, name=None,
+               description=None, default_ad_site=None):
+        """Create security service for NAS.
+
+        :param type: security service type - 'ldap', 'kerberos' or
+                     'active_directory'
+        :param dns_ip: dns ip address used inside tenant's network
+        :param ou: security service organizational unit
+        :param server: security service server ip address or hostname
+        :param domain: security service domain
+        :param user: security identifier used by tenant
+        :param password: password used by user
+        :param name: security service name
+        :param description: security service description
+        :param default_ad_site: default AD-Site
+        :rtype: :class:`SecurityService`
+        """
+        return self._create_security_service(type, dns_ip=dns_ip, ou=ou,
+                                             server=server, domain=domain,
+                                             user=user, password=password,
+                                             name=name,
+                                             description=description,
+                                             default_ad_site=default_ad_site)
+
+    def _create_security_service(self, type, dns_ip=None, ou=None,
+                                 server=None, domain=None, user=None,
+                                 password=None, name=None,
+                                 description=None, default_ad_site=None):
         values = {'type': type}
         if dns_ip:
             values['dns_ip'] = dns_ip
         if ou:
             values['ou'] = ou
         if server:
             values['server'] = server
@@ -71,14 +109,16 @@
             values['user'] = user
         if password:
             values['password'] = password
         if name:
             values['name'] = name
         if description:
             values['description'] = description
+        if default_ad_site:
+            values['default_ad_site'] = default_ad_site
 
         body = {RESOURCE_NAME: values}
 
         return self._create(RESOURCES_PATH, body, RESOURCE_NAME)
 
     def get(self, security_service):
         """Get a security service info.
@@ -87,14 +127,15 @@
         :rtype: :class:`SecurityService`
         """
         return self._get(
             RESOURCE_PATH % base.getid(security_service),
             RESOURCE_NAME,
         )
 
+    @api_versions.wraps("1.0", "2.75")
     def update(self, security_service, dns_ip=None, ou=None, server=None,
                domain=None, password=None, user=None, name=None,
                description=None):
         """Updates a security service.
 
         :param security_service: security service to update.
         :param dns_ip: dns ip address used inside tenant's network
@@ -103,15 +144,49 @@
         :param domain: security service domain
         :param user: security identifier used by tenant
         :param password: password used by user
         :param name: security service name
         :param description: security service description
         :rtype: :class:`SecurityService`
         """
+        return self._update_security_service(security_service, dns_ip=dns_ip,
+                                             ou=ou, server=server,
+                                             domain=domain, password=password,
+                                             user=user, name=name,
+                                             description=description)
+
+    @api_versions.wraps("2.76")  # noqa
+    def update(self, security_service, dns_ip=None, ou=None,     # noqa
+               server=None, domain=None, password=None, user=None,
+               name=None, description=None, default_ad_site=None):
+        """Updates a security service.
 
+        :param security_service: security service to update.
+        :param dns_ip: dns ip address used inside tenant's network
+        :param ou: security service organizational unit
+        :param server: security service server ip address or hostname
+        :param domain: security service domain
+        :param user: security identifier used by tenant
+        :param password: password used by user
+        :param name: security service name
+        :param description: security service description
+        :param default_ad_site: default AD-Site
+        :rtype: :class:`SecurityService`
+        """
+        return self._update_security_service(security_service, dns_ip=dns_ip,
+                                             ou=ou, server=server,
+                                             domain=domain, password=password,
+                                             user=user, name=name,
+                                             description=description,
+                                             default_ad_site=default_ad_site)
+
+    def _update_security_service(self, security_service, dns_ip=None, ou=None,
+                                 server=None, domain=None, password=None,
+                                 user=None, name=None, description=None,
+                                 default_ad_site=None):
         values = {}
         if dns_ip is not None:
             values['dns_ip'] = dns_ip
         if ou is not None:
             values['ou'] = ou
         if server is not None:
             values['server'] = server
@@ -121,14 +196,16 @@
             values['user'] = user
         if password is not None:
             values['password'] = password
         if name is not None:
             values['name'] = name
         if description is not None:
             values['description'] = description
+        if default_ad_site is not None:
+            values['default_ad_site'] = default_ad_site
 
         for k, v in values.items():
             if v == '':
                 values[k] = None
 
         if not values:
             msg = "Must specify fields to be updated"
```

### Comparing `python-manilaclient-4.4.0/manilaclient/v2/services.py` & `python-manilaclient-4.5.0/manilaclient/v2/services.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/v2/share_access_rules.py` & `python-manilaclient-4.5.0/manilaclient/v2/share_access_rules.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/v2/share_export_locations.py` & `python-manilaclient-4.5.0/manilaclient/v2/share_export_locations.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/v2/share_group_snapshots.py` & `python-manilaclient-4.5.0/manilaclient/v2/share_group_snapshots.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/v2/share_group_type_access.py` & `python-manilaclient-4.5.0/manilaclient/v2/share_group_type_access.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/v2/share_group_types.py` & `python-manilaclient-4.5.0/manilaclient/v2/share_group_types.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/v2/share_groups.py` & `python-manilaclient-4.5.0/manilaclient/v2/share_groups.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/v2/share_instance_export_locations.py` & `python-manilaclient-4.5.0/manilaclient/v2/share_instance_export_locations.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/v2/share_instances.py` & `python-manilaclient-4.5.0/manilaclient/v2/share_instances.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/v2/share_networks.py` & `python-manilaclient-4.5.0/manilaclient/v2/share_networks.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/v2/share_replica_export_locations.py` & `python-manilaclient-4.5.0/manilaclient/v2/share_replica_export_locations.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/v2/share_replicas.py` & `python-manilaclient-4.5.0/manilaclient/v2/share_replicas.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/v2/share_servers.py` & `python-manilaclient-4.5.0/manilaclient/v2/share_servers.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/v2/share_snapshot_export_locations.py` & `python-manilaclient-4.5.0/manilaclient/v2/share_snapshot_export_locations.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/v2/share_snapshot_instance_export_locations.py` & `python-manilaclient-4.5.0/manilaclient/v2/share_snapshot_instance_export_locations.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/v2/share_snapshot_instances.py` & `python-manilaclient-4.5.0/manilaclient/v2/share_snapshot_instances.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/v2/share_snapshots.py` & `python-manilaclient-4.5.0/manilaclient/v2/share_snapshots.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/v2/share_type_access.py` & `python-manilaclient-4.5.0/manilaclient/v2/share_type_access.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/v2/share_types.py` & `python-manilaclient-4.5.0/manilaclient/v2/share_types.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/v2/shares.py` & `python-manilaclient-4.5.0/manilaclient/v2/shares.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/manilaclient/v2/shell.py` & `python-manilaclient-4.5.0/manilaclient/v2/shell.py`

 * *Files 2% similar despite different names*

```diff
@@ -121,14 +121,19 @@
 
 
 def _find_share(cs, share):
     """Get a share by ID."""
     return apiclient_utils.find_resource(cs.shares, share)
 
 
+def _find_share_transfer(cs, transfer):
+    """Get a share transfer by ID."""
+    return apiclient_utils.find_resource(cs.transfers, transfer)
+
+
 @api_versions.wraps("1.0", "2.8")
 def _print_share(cs, share):
     info = share._info.copy()
     info.pop('links', None)
 
     # NOTE(vponomaryov): remove deprecated single field 'export_location' and
     # leave only list field 'export_locations'. Also, transform the latter to
@@ -4181,14 +4186,21 @@
     help="Password used by user.")
 @cliutils.arg(
     '--name',
     metavar='<name>',
     default=None,
     help="Security service name.")
 @cliutils.arg(
+    '--default-ad-site',
+    metavar='<default_ad_site>',
+    dest='default_ad_site',
+    default=None,
+    help="Default AD site. Available only for microversion >= 2.76. Can "
+         "be provided in the place of '--server' but not along with it.")
+@cliutils.arg(
     '--description',
     metavar='<description>',
     default=None,
     help="Security service description.")
 def do_security_service_create(cs, args):
     """Create security service used by project."""
     values = {
@@ -4205,14 +4217,29 @@
                               api_versions.APIVersion()):
         values['ou'] = args.ou
     elif args.ou:
         raise exceptions.CommandError(
             "Security service Organizational Unit (ou) option "
             "is only available with manila API version >= 2.44")
 
+    if cs.api_version.matches(api_versions.APIVersion("2.76"),
+                              api_versions.APIVersion()):
+        values['default_ad_site'] = args.default_ad_site
+    elif args.default_ad_site:
+        raise exceptions.CommandError(
+            "Default AD site option is only available with "
+            "manila API version >= 2.76")
+
+    if args.type == 'active_directory':
+        if args.server and args.default_ad_site:
+            raise exceptions.CommandError(
+                "Cannot create security service because both "
+                "server and 'default_ad_site' were provided. "
+                "Specify either server or 'default_ad_site'.")
+
     security_service = cs.security_services.create(args.type, **values)
     info = security_service._info.copy()
     cliutils.print_dict(info)
 
 
 @cliutils.arg(
     'security_service',
@@ -4251,14 +4278,20 @@
     help="Password used by user.")
 @cliutils.arg(
     '--name',
     metavar='<name>',
     default=None,
     help="Security service name.")
 @cliutils.arg(
+    '--default-ad-site',
+    metavar='<default_ad_site>',
+    dest='default_ad_site',
+    default=None,
+    help="Default AD site. Available only for microversion >= 2.76.")
+@cliutils.arg(
     '--description',
     metavar='<description>',
     default=None,
     help="Security service description.")
 def do_security_service_update(cs, args):
     """Update security service."""
     values = {
@@ -4275,14 +4308,22 @@
                               api_versions.APIVersion()):
         values['ou'] = args.ou
     elif args.ou:
         raise exceptions.CommandError(
             "Security service Organizational Unit (ou) option "
             "is only available with manila API version >= 2.44")
 
+    if cs.api_version.matches(api_versions.APIVersion("2.76"),
+                              api_versions.APIVersion()):
+        values['default_ad_site'] = args.default_ad_site
+    elif args.default_ad_site:
+        raise exceptions.CommandError(
+            "Default AD site option is only available with "
+            "manila API version >= 2.76")
+
     security_service = _find_security_service(
         cs, args.security_service).update(**values)
     cliutils.print_dict(security_service._info)
 
 
 @cliutils.arg(
     'security_service',
@@ -4371,14 +4412,20 @@
     help='Start position of security services listing.')
 @cliutils.arg(
     '--limit',
     metavar="<limit>",
     default=None,
     help='Number of security services to return per request.')
 @cliutils.arg(
+    '--default-ad-site',
+    metavar='<default_ad_site>',
+    dest='default_ad_site',
+    default=None,
+    help="Default AD site. Available only for microversion >= 2.76.")
+@cliutils.arg(
     '--columns',
     metavar='<columns>',
     type=str,
     default=None,
     help='Comma separated list of columns to be displayed '
          'example --columns "name,type".')
 def do_security_service_list(cs, args):
@@ -4405,14 +4452,22 @@
                               api_versions.APIVersion()):
         search_opts['ou'] = args.ou
     elif args.ou:
         raise exceptions.CommandError(
             "Security service Organizational Unit (ou) option "
             "is only available with manila API version >= 2.44")
 
+    if cs.api_version.matches(api_versions.APIVersion("2.76"),
+                              api_versions.APIVersion()):
+        search_opts['default_ad_site'] = args.default_ad_site
+    elif args.ou:
+        raise exceptions.CommandError(
+            "Security service Default AD site option "
+            "is only available with manila API version >= 2.76")
+
     if args.share_network:
         search_opts['share_network_id'] = _find_share_network(
             cs, args.share_network).id
     security_services = cs.security_services.list(search_opts=search_opts,
                                                   detailed=args.detailed)
     fields = ['id', 'name', 'status', 'type', ]
     if args.columns is not None:
@@ -6530,14 +6585,220 @@
     """Attempt to update the share replica with its 'active' mirror."""
     replica = _find_share_replica(cs, args.replica)
     cs.share_replicas.resync(replica)
 
 
 ##############################################################################
 #
+# Share Transfer
+#
+##############################################################################
+
+
+def _print_share_transfer(transfer):
+    info = transfer._info.copy()
+    info.pop('links', None)
+
+    cliutils.print_dict(info)
+
+
+@api_versions.wraps("2.77")
+@cliutils.arg(
+    'share',
+    metavar='<share>',
+    help='Name or ID of share to transfer.')
+@cliutils.arg(
+    '--name',
+    metavar='<name>',
+    default=None,
+    help='Transfer name. Default=None.')
+def do_share_transfer_create(cs, args):
+    """Creates a share transfer."""
+    share = _find_share(cs, args.share)
+    transfer = cs.transfers.create(share.id,
+                                   args.name)
+    _print_share_transfer(transfer)
+
+
+@api_versions.wraps("2.77")
+@cliutils.arg(
+    'transfer',
+    metavar='<transfer>',
+    nargs='+',
+    help='ID or name of the transfer(s).')
+def do_share_transfer_delete(cs, args):
+    """Remove one or more transfers."""
+    failure_count = 0
+
+    for transfer in args.transfer:
+        try:
+            transfer_ref = _find_share_transfer(cs, transfer)
+            transfer_ref.delete()
+        except Exception as e:
+            failure_count += 1
+            print("Delete for share transfer %s failed: %s" % (transfer, e),
+                  file=sys.stderr)
+
+    if failure_count == len(args.transfer):
+        raise exceptions.CommandError("Unable to delete any of the specified "
+                                      "transfers.")
+
+
+@api_versions.wraps("2.77")
+@cliutils.arg(
+    'transfer',
+    metavar='<transfer>',
+    help='ID of transfer to accept.')
+@cliutils.arg(
+    'auth_key',
+    metavar='<auth_key>',
+    help='Authentication key of transfer to accept.')
+@cliutils.arg(
+    '--clear-rules',
+    '--clear_rules',
+    dest='clear_rules',
+    action='store_true',
+    default=False,
+    help="Whether manila should clean up the access rules after the "
+         "transfer is complete. (Default=False)")
+def do_share_transfer_accept(cs, args):
+    """Accepts a share transfer."""
+    cs.transfers.accept(args.transfer, args.auth_key,
+                        clear_access_rules=args.clear_rules)
+
+
+@api_versions.wraps("2.77")
+@cliutils.arg(
+    '--all-tenants', '--all-projects',
+    action='single_alias',
+    dest='all_projects',
+    metavar='<0|1>',
+    nargs='?',
+    type=int,
+    const=1,
+    default=0,
+    help='Shows details for all tenants. (Admin only).')
+@cliutils.arg(
+    '--name',
+    metavar='<name>',
+    default=None,
+    action='single_alias',
+    help='Transfer name. Default=None.')
+@cliutils.arg(
+    '--id',
+    metavar='<id>',
+    default=None,
+    action='single_alias',
+    help='Transfer ID. Default=None.')
+@cliutils.arg(
+    '--resource-type', '--resource_type',
+    metavar='<resource_type>',
+    default=None,
+    action='single_alias',
+    help='Transfer type, which can be share or network. Default=None.')
+@cliutils.arg(
+    '--resource-id', '--resource_id',
+    metavar='<resource_id>',
+    default=None,
+    action='single_alias',
+    help='Transfer resource id. Default=None.')
+@cliutils.arg(
+    '--source-project-id', '--source_project_id',
+    metavar='<source_project_id>',
+    default=None,
+    action='single_alias',
+    help='Transfer source project id. Default=None.')
+@cliutils.arg(
+    '--limit',
+    metavar='<limit>',
+    type=int,
+    default=None,
+    help='Maximum number of messages to return. (Default=None)')
+@cliutils.arg(
+    '--offset',
+    metavar="<offset>",
+    default=None,
+    help='Start position of message listing.')
+@cliutils.arg(
+    '--sort-key', '--sort_key',
+    metavar='<sort_key>',
+    type=str,
+    default=None,
+    action='single_alias',
+    help='Key to be sorted, available keys are %(keys)s. Default=None.'
+         % {'keys': constants.SHARE_TRANSFER_SORT_KEY_VALUES})
+@cliutils.arg(
+    '--sort-dir', '--sort_dir',
+    metavar='<sort_dir>',
+    type=str,
+    default=None,
+    action='single_alias',
+    help='Sort direction, available values are %(values)s. '
+         'Optional: Default=None.' % {'values': constants.SORT_DIR_VALUES})
+@cliutils.arg(
+    '--detailed',
+    dest='detailed',
+    metavar='<0|1>',
+    nargs='?',
+    type=int,
+    const=1,
+    default=0,
+    help="Show detailed information about filtered share transfers.")
+@cliutils.arg(
+    '--columns',
+    metavar='<columns>',
+    type=str,
+    default=None,
+    help='Comma separated list of columns to be displayed '
+         'example --columns "id,resource_id".')
+def do_share_transfer_list(cs, args):
+    """Lists all transfers."""
+    if args.columns is not None:
+        list_of_keys = _split_columns(columns=args.columns)
+    else:
+        list_of_keys = ['ID', 'Name', 'Resource Type', 'Resource Id']
+
+    if args.detailed:
+        list_of_keys.extend(['Created At', 'Expires At', 'Source Project Id',
+                             'Destination Project Id', 'Accepted'])
+
+    all_projects = int(
+        os.environ.get("ALL_TENANTS",
+                       os.environ.get("ALL_PROJECTS",
+                                      args.all_projects))
+    )
+
+    search_opts = {
+        'offset': args.offset,
+        'limit': args.limit,
+        'all_tenants': all_projects,
+        'id': args.id,
+        'name': args.name,
+        'resource_type': args.resource_type,
+        'resource_id': args.resource_id,
+        'source_project_id': args.source_project_id,
+    }
+    share_transfers = cs.transfers.list(
+        detailed=args.detailed, search_opts=search_opts,
+        sort_key=args.sort_key, sort_dir=args.sort_dir)
+    cliutils.print_list(share_transfers, fields=list_of_keys,
+                        sortby_index=None)
+
+
+@api_versions.wraps("2.77")
+@cliutils.arg(
+    'transfer',
+    metavar='<transfer>',
+    help='Name or ID of transfer to show.')
+def do_share_transfer_show(cs, args):
+    """Delete a transfer."""
+    transfer = _find_share_transfer(cs, args.transfer)
+    _print_share_transfer(transfer)
+##############################################################################
+#
 # User Messages
 #
 ##############################################################################
 
 
 @api_versions.wraps("2.37")
 @cliutils.arg(
```

### Comparing `python-manilaclient-4.4.0/python_manilaclient.egg-info/PKG-INFO` & `python-manilaclient-4.5.0/python_manilaclient.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: python-manilaclient
-Version: 4.4.0
+Version: 4.5.0
 Summary: Client library for OpenStack Manila API.
 Home-page: https://docs.openstack.org/python-manilaclient/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ========================
         Team and repository tags
```

### Comparing `python-manilaclient-4.4.0/python_manilaclient.egg-info/SOURCES.txt` & `python-manilaclient-4.5.0/python_manilaclient.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -67,14 +67,15 @@
 manilaclient/osc/v2/share_pools.py
 manilaclient/osc/v2/share_replica_export_locations.py
 manilaclient/osc/v2/share_replicas.py
 manilaclient/osc/v2/share_servers.py
 manilaclient/osc/v2/share_snapshot_instance_export_locations.py
 manilaclient/osc/v2/share_snapshot_instances.py
 manilaclient/osc/v2/share_snapshots.py
+manilaclient/osc/v2/share_transfers.py
 manilaclient/osc/v2/share_type_access.py
 manilaclient/osc/v2/share_types.py
 manilaclient/tests/__init__.py
 manilaclient/tests/functional/__init__.py
 manilaclient/tests/functional/base.py
 manilaclient/tests/functional/client.py
 manilaclient/tests/functional/exceptions.py
@@ -89,14 +90,15 @@
 manilaclient/tests/functional/test_services.py
 manilaclient/tests/functional/test_share_access.py
 manilaclient/tests/functional/test_share_network_subnets.py
 manilaclient/tests/functional/test_share_networks.py
 manilaclient/tests/functional/test_share_replica_export_locations.py
 manilaclient/tests/functional/test_share_replicas.py
 manilaclient/tests/functional/test_share_servers.py
+manilaclient/tests/functional/test_share_transfers.py
 manilaclient/tests/functional/test_share_types.py
 manilaclient/tests/functional/test_shares.py
 manilaclient/tests/functional/test_shares_listing.py
 manilaclient/tests/functional/test_shares_metadata.py
 manilaclient/tests/functional/test_snapshot_access.py
 manilaclient/tests/functional/test_snapshot_instances.py
 manilaclient/tests/functional/test_snapshot_instances_export_locations.py
@@ -112,14 +114,15 @@
 manilaclient/tests/functional/osc/test_share_network_subnets.py
 manilaclient/tests/functional/osc/test_share_networks.py
 manilaclient/tests/functional/osc/test_share_pools.py
 manilaclient/tests/functional/osc/test_share_replica_export_locations.py
 manilaclient/tests/functional/osc/test_share_replicas.py
 manilaclient/tests/functional/osc/test_share_services.py
 manilaclient/tests/functional/osc/test_share_snapshots.py
+manilaclient/tests/functional/osc/test_share_transfers.py
 manilaclient/tests/functional/osc/test_share_types.py
 manilaclient/tests/functional/osc/test_shares.py
 manilaclient/tests/functional/osc/test_shares_group_type.py
 manilaclient/tests/unit/__init__.py
 manilaclient/tests/unit/fakes.py
 manilaclient/tests/unit/test_api_versions.py
 manilaclient/tests/unit/test_base.py
@@ -154,14 +157,15 @@
 manilaclient/tests/unit/osc/v2/test_share_pools.py
 manilaclient/tests/unit/osc/v2/test_share_replica_export_locations.py
 manilaclient/tests/unit/osc/v2/test_share_replicas.py
 manilaclient/tests/unit/osc/v2/test_share_servers.py
 manilaclient/tests/unit/osc/v2/test_share_snapshot_instance_export_locations.py
 manilaclient/tests/unit/osc/v2/test_share_snapshot_instances.py
 manilaclient/tests/unit/osc/v2/test_share_snapshots.py
+manilaclient/tests/unit/osc/v2/test_share_transfers.py
 manilaclient/tests/unit/osc/v2/test_share_type.py
 manilaclient/tests/unit/osc/v2/test_share_type_access.py
 manilaclient/tests/unit/v1/test_limits.py
 manilaclient/tests/unit/v1/test_quota_classes.py
 manilaclient/tests/unit/v1/test_quotas.py
 manilaclient/tests/unit/v1/test_scheduler_stats.py
 manilaclient/tests/unit/v1/test_security_services.py
@@ -196,14 +200,15 @@
 manilaclient/tests/unit/v2/test_share_replica_export_locations.py
 manilaclient/tests/unit/v2/test_share_replicas.py
 manilaclient/tests/unit/v2/test_share_servers.py
 manilaclient/tests/unit/v2/test_share_snapshot_export_locations.py
 manilaclient/tests/unit/v2/test_share_snapshot_instance_export_locations.py
 manilaclient/tests/unit/v2/test_share_snapshot_instances.py
 manilaclient/tests/unit/v2/test_share_snapshots.py
+manilaclient/tests/unit/v2/test_share_transfers.py
 manilaclient/tests/unit/v2/test_shares.py
 manilaclient/tests/unit/v2/test_shell.py
 manilaclient/tests/unit/v2/test_type_access.py
 manilaclient/tests/unit/v2/test_types.py
 manilaclient/v1/__init__.py
 manilaclient/v1/client.py
 manilaclient/v1/limits.py
@@ -243,14 +248,15 @@
 manilaclient/v2/share_replica_export_locations.py
 manilaclient/v2/share_replicas.py
 manilaclient/v2/share_servers.py
 manilaclient/v2/share_snapshot_export_locations.py
 manilaclient/v2/share_snapshot_instance_export_locations.py
 manilaclient/v2/share_snapshot_instances.py
 manilaclient/v2/share_snapshots.py
+manilaclient/v2/share_transfers.py
 manilaclient/v2/share_type_access.py
 manilaclient/v2/share_types.py
 manilaclient/v2/shares.py
 manilaclient/v2/shell.py
 manilaclient/v2/contrib/__init__.py
 manilaclient/v2/contrib/list_extensions.py
 playbooks/enable-fips.yaml
@@ -266,14 +272,15 @@
 python_manilaclient.egg-info/top_level.txt
 rally-jobs/rally-manila-no-ss.yaml
 rally-jobs/rally-manila.yaml
 releasenotes/notes/.placeholder
 releasenotes/notes/Bug-1990013-fix-share-grou-from-snapshot-create-fa3629cf1417ba20.yaml
 releasenotes/notes/add-count-info-in-share-21a6b36c0f4c87b2.yaml
 releasenotes/notes/add-dash-dash-help-subcomand-ad4226454aa07bc6.yaml
+releasenotes/notes/add-defaultadsite-to-security-service-33fd0a5d1b865b11.yaml
 releasenotes/notes/add-export-location-filter-4cf3114doe40k598.yaml
 releasenotes/notes/add-ipv6-access-type-4dko90r1a9a1e0b8.yaml
 releasenotes/notes/add-like-filter-591572762357ef4b.yaml
 releasenotes/notes/add-message-list-and-delete-41b3323edd63d894.yaml
 releasenotes/notes/add-metadata-for-share-access-rule-11a6b36c0f4c87c2.yaml
 releasenotes/notes/add-per-share-gigabytes-quotas-40bc404bd3cbdd89.yaml
 releasenotes/notes/add-query-params-pools-list-api-12cf1s14ddf40kdd.yaml
@@ -283,22 +290,24 @@
 releasenotes/notes/add-scheduler-hints-to-share-replica-create-d152a3934e5ad3a7.yaml
 releasenotes/notes/add-share-group-quotas-support-b6563cec58209a1d.yaml
 releasenotes/notes/add-share-group-support-a3166f6ca4d06a81.yaml
 releasenotes/notes/add-share-network-sec-service-add-update-to-in-use-networks-ec7a60d07ebceaf4.yaml
 releasenotes/notes/add-share-replicas-and-replica-gigabytes-quotas-909436c2b2420f2c.yaml
 releasenotes/notes/add-snapshot-instances-admin-api-3cf3114doe40k598.yaml
 releasenotes/notes/add-snapshot-metadata-49b0288bf2f12bf0.yaml
+releasenotes/notes/add-subnet-metadata-82426986431b0179.yaml
 releasenotes/notes/add-support-filter-search-for-share-type-fdbaaa9510cc59dd.yaml
 releasenotes/notes/add-support-to-check-quota-usage-scfdg14dod40k71a.yaml
 releasenotes/notes/add_support_multiple_subnet_per_az-46145c3e90e097be.yaml
 releasenotes/notes/bp-export-locations-replica-az-commands-03aa32c08f59c42d.yaml
 releasenotes/notes/bp-integrate-os-profiler-4818066dc2fbf7b7.yaml
 releasenotes/notes/bp-ocata-migration-improvements-f63c5d233856fbee.yaml
 releasenotes/notes/bp-support-group-spec-search-share-group-type-api-d5d9a6096f084b91.yaml
 releasenotes/notes/bp-support-query-user-messages-by-timestamp-34b70bba2d1b4d13.yaml
+releasenotes/notes/bp-support-share-transfer-between-project-faefead551380eca.yaml
 releasenotes/notes/bp-update-share-type-name-or-description-32d98b5a42cd8090.yaml
 releasenotes/notes/bug-1558995-fix-endpoint-not-found.yaml-a06a3b0ba5006718.yaml
 releasenotes/notes/bug-1608664-add-support-columns-share-replica-list-885bd8c8b4bfa8f1.yaml
 releasenotes/notes/bug-1611506-allow-deletion-multiple-resources
 releasenotes/notes/bug-1622540-add-missing-az-list-command-f90265de5c2f261b.yaml
 releasenotes/notes/bug-1650774-share-instance-reset-state-9c4b26f44b5da0e9.yaml
 releasenotes/notes/bug-1664877-c462bfad92ce03e5.yaml
@@ -368,14 +377,15 @@
 releasenotes/notes/start-using-reno-b744cd0259c7a88c.yaml
 releasenotes/notes/support-create-share-from-snapshot-extra-spec-cdba92f179c1c5c6.yaml
 releasenotes/notes/support-share-server-migration-9804752270c6b153.yaml
 releasenotes/notes/support-show-type-6380b7c539c95ba8.yaml
 releasenotes/notes/type-create-extra-specs-691572762357ef3b.yaml
 releasenotes/notes/update-api-version-create-share-from-snapshot-another-pool-or-backend-694cfda84a41c4ff.yaml
 releasenotes/notes/v2-0-0-deprecated-opts-removal-863565618535733d.yaml
+releasenotes/source/2023.1.rst
 releasenotes/source/conf.py
 releasenotes/source/index.rst
 releasenotes/source/newton.rst
 releasenotes/source/ocata.rst
 releasenotes/source/pike.rst
 releasenotes/source/queens.rst
 releasenotes/source/rocky.rst
```

### Comparing `python-manilaclient-4.4.0/python_manilaclient.egg-info/entry_points.txt` & `python-manilaclient-4.5.0/python_manilaclient.egg-info/entry_points.txt`

 * *Files 3% similar despite different names*

```diff
@@ -58,15 +58,17 @@
 share_network_create = manilaclient.osc.v2.share_networks:CreateShareNetwork
 share_network_delete = manilaclient.osc.v2.share_networks:DeleteShareNetwork
 share_network_list = manilaclient.osc.v2.share_networks:ListShareNetwork
 share_network_set = manilaclient.osc.v2.share_networks:SetShareNetwork
 share_network_show = manilaclient.osc.v2.share_networks:ShowShareNetwork
 share_network_subnet_create = manilaclient.osc.v2.share_network_subnets:CreateShareNetworkSubnet
 share_network_subnet_delete = manilaclient.osc.v2.share_network_subnets:DeleteShareNetworkSubnet
+share_network_subnet_set = manilaclient.osc.v2.share_network_subnets:SetShareNetworkSubnet
 share_network_subnet_show = manilaclient.osc.v2.share_network_subnets:ShowShareNetworkSubnet
+share_network_subnet_unset = manilaclient.osc.v2.share_network_subnets:UnsetShareNetworkSubnet
 share_network_unset = manilaclient.osc.v2.share_networks:UnsetShareNetwork
 share_pool_list = manilaclient.osc.v2.share_pools:ListSharePools
 share_properties_show = manilaclient.osc.v2.share:ShowShareProperties
 share_quota_delete = manilaclient.osc.v2.quotas:QuotaDelete
 share_quota_set = manilaclient.osc.v2.quotas:QuotaSet
 share_quota_show = manilaclient.osc.v2.quotas:QuotaShow
 share_replica_create = manilaclient.osc.v2.share_replicas:CreateShareReplica
@@ -115,14 +117,19 @@
 share_snapshot_instance_list = manilaclient.osc.v2.share_snapshot_instances:ListShareSnapshotInstance
 share_snapshot_instance_set = manilaclient.osc.v2.share_snapshot_instances:SetShareSnapshotInstance
 share_snapshot_instance_show = manilaclient.osc.v2.share_snapshot_instances:ShowShareSnapshotInstance
 share_snapshot_list = manilaclient.osc.v2.share_snapshots:ListShareSnapshot
 share_snapshot_set = manilaclient.osc.v2.share_snapshots:SetShareSnapshot
 share_snapshot_show = manilaclient.osc.v2.share_snapshots:ShowShareSnapshot
 share_snapshot_unset = manilaclient.osc.v2.share_snapshots:UnsetShareSnapshot
+share_transfer_accept = manilaclient.osc.v2.share_transfers:AcceptShareTransfer
+share_transfer_create = manilaclient.osc.v2.share_transfers:CreateShareTransfer
+share_transfer_delete = manilaclient.osc.v2.share_transfers:DeleteShareTransfer
+share_transfer_list = manilaclient.osc.v2.share_transfers:ListShareTransfer
+share_transfer_show = manilaclient.osc.v2.share_transfers:ShowShareTransfer
 share_type_access_create = manilaclient.osc.v2.share_type_access:ShareTypeAccessAllow
 share_type_access_delete = manilaclient.osc.v2.share_type_access:ShareTypeAccessDeny
 share_type_access_list = manilaclient.osc.v2.share_type_access:ListShareTypeAccess
 share_type_create = manilaclient.osc.v2.share_types:CreateShareType
 share_type_delete = manilaclient.osc.v2.share_types:DeleteShareType
 share_type_list = manilaclient.osc.v2.share_types:ListShareType
 share_type_set = manilaclient.osc.v2.share_types:SetShareType
```

### Comparing `python-manilaclient-4.4.0/rally-jobs/rally-manila-no-ss.yaml` & `python-manilaclient-4.5.0/rally-jobs/rally-manila-no-ss.yaml`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/rally-jobs/rally-manila.yaml` & `python-manilaclient-4.5.0/rally-jobs/rally-manila.yaml`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/releasenotes/notes/add-share-network-sec-service-add-update-to-in-use-networks-ec7a60d07ebceaf4.yaml` & `python-manilaclient-4.5.0/releasenotes/notes/add-share-network-sec-service-add-update-to-in-use-networks-ec7a60d07ebceaf4.yaml`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/releasenotes/notes/deprecate-v1-a0cfa6fd723c2f46.yaml` & `python-manilaclient-4.5.0/releasenotes/notes/deprecate-v1-a0cfa6fd723c2f46.yaml`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/releasenotes/notes/manila-openstackclient-bf61ceb270d3afb7.yaml` & `python-manilaclient-4.5.0/releasenotes/notes/manila-openstackclient-bf61ceb270d3afb7.yaml`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/releasenotes/notes/newton-migration-improvements-166a03472948bdef.yaml` & `python-manilaclient-4.5.0/releasenotes/notes/newton-migration-improvements-166a03472948bdef.yaml`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/releasenotes/notes/remove-experimental-flag-from-share-groups-feature-dcf2b0b67fe4cac4.yaml` & `python-manilaclient-4.5.0/releasenotes/notes/remove-experimental-flag-from-share-groups-feature-dcf2b0b67fe4cac4.yaml`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/releasenotes/notes/share-network-multiple-subnets-732309abfbf5987c.yaml` & `python-manilaclient-4.5.0/releasenotes/notes/share-network-multiple-subnets-732309abfbf5987c.yaml`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/releasenotes/source/conf.py` & `python-manilaclient-4.5.0/releasenotes/source/conf.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/requirements.txt` & `python-manilaclient-4.5.0/requirements.txt`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/roles/populate-manilaclient-config/README.rst` & `python-manilaclient-4.5.0/roles/populate-manilaclient-config/README.rst`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/roles/populate-manilaclient-config/tasks/main.yaml` & `python-manilaclient-4.5.0/roles/populate-manilaclient-config/tasks/main.yaml`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/run_tests.sh` & `python-manilaclient-4.5.0/run_tests.sh`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/setup.cfg` & `python-manilaclient-4.5.0/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -121,14 +121,16 @@
 	share_network_create = manilaclient.osc.v2.share_networks:CreateShareNetwork
 	share_network_delete = manilaclient.osc.v2.share_networks:DeleteShareNetwork
 	share_network_set = manilaclient.osc.v2.share_networks:SetShareNetwork
 	share_network_unset = manilaclient.osc.v2.share_networks:UnsetShareNetwork
 	share_network_subnet_create = manilaclient.osc.v2.share_network_subnets:CreateShareNetworkSubnet
 	share_network_subnet_delete = manilaclient.osc.v2.share_network_subnets:DeleteShareNetworkSubnet
 	share_network_subnet_show = manilaclient.osc.v2.share_network_subnets:ShowShareNetworkSubnet
+	share_network_subnet_set = manilaclient.osc.v2.share_network_subnets:SetShareNetworkSubnet
+	share_network_subnet_unset = manilaclient.osc.v2.share_network_subnets:UnsetShareNetworkSubnet
 	share_group_create = manilaclient.osc.v2.share_groups:CreateShareGroup
 	share_group_delete = manilaclient.osc.v2.share_groups:DeleteShareGroup
 	share_group_list = manilaclient.osc.v2.share_groups:ListShareGroup
 	share_group_show = manilaclient.osc.v2.share_groups:ShowShareGroup
 	share_group_set = manilaclient.osc.v2.share_groups:SetShareGroup
 	share_group_unset = manilaclient.osc.v2.share_groups:UnsetShareGroup
 	share_group_type_create = manilaclient.osc.v2.share_group_types:CreateShareGroupType
@@ -153,14 +155,19 @@
 	share_server_adopt = manilaclient.osc.v2.share_servers:AdoptShareServer
 	share_server_abandon = manilaclient.osc.v2.share_servers:AbandonShareServer
 	share_server_set = manilaclient.osc.v2.share_servers:SetShareServer
 	share_server_migration_cancel = manilaclient.osc.v2.share_servers:ShareServerMigrationCancel
 	share_server_migration_complete = manilaclient.osc.v2.share_servers:ShareServerMigrationComplete
 	share_server_migration_show = manilaclient.osc.v2.share_servers:ShareServerMigrationShow
 	share_server_migration_start = manilaclient.osc.v2.share_servers:ShareServerMigrationStart
+	share_transfer_create = manilaclient.osc.v2.share_transfers:CreateShareTransfer
+	share_transfer_delete = manilaclient.osc.v2.share_transfers:DeleteShareTransfer
+	share_transfer_list = manilaclient.osc.v2.share_transfers:ListShareTransfer
+	share_transfer_show = manilaclient.osc.v2.share_transfers:ShowShareTransfer
+	share_transfer_accept = manilaclient.osc.v2.share_transfers:AcceptShareTransfer
 
 [coverage:run]
 omit = manilaclient/tests/*
 branch = true
 
 [egg_info]
 tag_build =
```

### Comparing `python-manilaclient-4.4.0/setup.py` & `python-manilaclient-4.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.4.0/tox.ini` & `python-manilaclient-4.5.0/tox.ini`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 basepython = python3
 usedevelop = true
 setenv = VIRTUAL_ENV={envdir}
          OS_STDOUT_CAPTURE=1
          OS_STDERR_CAPTURE=1
          PYTHONDONTWRITEBYTECODE=1
 deps =
-       -c{env:TOX_CONSTRAINTS_FILE:https://releases.openstack.org/constraints/upper/2023.1}
+       -c{env:TOX_CONSTRAINTS_FILE:https://releases.openstack.org/constraints/upper/master}
        -r{toxinidir}/test-requirements.txt
 commands =
   stestr run {posargs}
   stestr slowest
 
 [testenv:debug]
 commands = oslo_debug_helper -t manilaclient/tests {posargs}
@@ -29,15 +29,15 @@
   flake8
 
 [testenv:venv]
 commands = {posargs}
 
 [testenv:docs]
 deps =
-       -c{env:TOX_CONSTRAINTS_FILE:https://releases.openstack.org/constraints/upper/2023.1}
+       -c{env:TOX_CONSTRAINTS_FILE:https://releases.openstack.org/constraints/upper/master}
        -r{toxinidir}/doc/requirements.txt
 allowlist_externals = rm
 commands =
   rm -rf doc/build
   sphinx-build -b html doc/source doc/build/html
 
 [testenv:pdf-docs]
@@ -46,15 +46,15 @@
   make
 commands =
   sphinx-build  -W -b latex doc/source doc/build/pdf
   make -C doc/build/pdf
 
 [testenv:releasenotes]
 deps =
-       -c{env:TOX_CONSTRAINTS_FILE:https://releases.openstack.org/constraints/upper/2023.1}
+       -c{env:TOX_CONSTRAINTS_FILE:https://releases.openstack.org/constraints/upper/master}
        -r{toxinidir}/doc/requirements.txt
 allowlist_externals = rm
 commands =
     rm -rf releasenotes/build
     sphinx-build -a -E -W -d releasenotes/build/doctrees \
          -b html releasenotes/source releasenotes/build/html
```

### Comparing `python-manilaclient-4.4.0/zuul.d/python-manilaclient-jobs.yaml` & `python-manilaclient-4.5.0/zuul.d/python-manilaclient-jobs.yaml`

 * *Files identical despite different names*

