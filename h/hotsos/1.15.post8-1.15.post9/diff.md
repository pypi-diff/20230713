# Comparing `tmp/hotsos-1.15.post8.tar.gz` & `tmp/hotsos-1.15.post9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hotsos-1.15.post8.tar", last modified: Wed Jul  5 12:46:34 2023, max compression
+gzip compressed data, was "hotsos-1.15.post9.tar", last modified: Thu Jul  6 09:00:02 2023, max compression
```

## Comparing `hotsos-1.15.post8.tar` & `hotsos-1.15.post9.tar`

### file list

```diff
@@ -1,409 +1,409 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:46:34.238091 hotsos-1.15.post8/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-05 12:46:08.000000 hotsos-1.15.post8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-05 12:46:08.000000 hotsos-1.15.post8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-07-05 12:46:34.238091 hotsos-1.15.post8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-07-05 12:46:08.000000 hotsos-1.15.post8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:46:34.170090 hotsos-1.15.post8/hotsos/
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-05 12:46:15.000000 hotsos-1.15.post8/hotsos/.repo-info
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    15069 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/cli.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    15427 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:46:34.174090 hotsos-1.15.post8/hotsos/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10719 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/core/analytics.py
--rw-r--r--   0 runner    (1001) docker     (123)     9998 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/core/config.py
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/core/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/core/factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:46:34.178090 hotsos-1.15.post8/hotsos/core/host_helpers/
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/core/host_helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    35418 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/core/host_helpers/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3068 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/core/host_helpers/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     4696 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/core/host_helpers/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/core/host_helpers/filestat.py
--rw-r--r--   0 runner    (1001) docker     (123)    11021 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/core/host_helpers/network.py
--rw-r--r--   0 runner    (1001) docker     (123)    13241 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/core/host_helpers/packaging.py
--rw-r--r--   0 runner    (1001) docker     (123)     3346 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/core/host_helpers/pebble.py
--rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/core/host_helpers/ssl.py
--rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/core/host_helpers/sysctl.py
--rw-r--r--   0 runner    (1001) docker     (123)    11385 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/core/host_helpers/systemd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/core/host_helpers/uptime.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:46:34.178090 hotsos-1.15.post8/hotsos/core/issues/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/core/issues/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/core/issues/issue_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     5118 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/core/issues/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/core/log.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:46:34.178090 hotsos-1.15.post8/hotsos/core/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/core/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:46:34.178090 hotsos-1.15.post8/hotsos/core/plugins/juju/
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/core/plugins/juju/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/core/plugins/juju/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     6356 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/core/plugins/juju/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:46:34.182090 hotsos-1.15.post8/hotsos/core/plugins/kernel/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/core/plugins/kernel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/core/plugins/kernel/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/core/plugins/kernel/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:46:34.182090 hotsos-1.15.post8/hotsos/core/plugins/kernel/kernlog/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/core/plugins/kernel/kernlog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14852 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/core/plugins/kernel/kernlog/calltrace.py
--rw-r--r--   0 runner    (1001) docker     (123)     3835 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/core/plugins/kernel/kernlog/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/core/plugins/kernel/kernlog/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     7491 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/core/plugins/kernel/memory.py
--rw-r--r--   0 runner    (1001) docker     (123)    20374 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/core/plugins/kernel/net.py
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/core/plugins/kernel/sysfs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/core/plugins/kubernetes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:46:34.182090 hotsos-1.15.post8/hotsos/core/plugins/lxd/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/core/plugins/lxd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/core/plugins/lxd/common.py
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/core/plugins/maas.py
--rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/core/plugins/mysql.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:46:34.182090 hotsos-1.15.post8/hotsos/core/plugins/openstack/
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/core/plugins/openstack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8218 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/core/plugins/openstack/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    63860 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/core/plugins/openstack/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3793 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/core/plugins/openstack/neutron.py
--rw-r--r--   0 runner    (1001) docker     (123)    10636 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/core/plugins/openstack/nova.py
--rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/core/plugins/openstack/octavia.py
--rw-r--r--   0 runner    (1001) docker     (123)    19464 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/core/plugins/openstack/openstack.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:46:34.186090 hotsos-1.15.post8/hotsos/core/plugins/openvswitch/
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/core/plugins/openvswitch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/core/plugins/openvswitch/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     4786 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/core/plugins/openvswitch/ovn.py
--rw-r--r--   0 runner    (1001) docker     (123)     4804 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/core/plugins/openvswitch/ovs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/core/plugins/pacemaker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:46:34.186090 hotsos-1.15.post8/hotsos/core/plugins/rabbitmq/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/core/plugins/rabbitmq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/core/plugins/rabbitmq/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     9003 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/core/plugins/rabbitmq/report.py
--rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/core/plugins/sosreport.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:46:34.186090 hotsos-1.15.post8/hotsos/core/plugins/storage/
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/core/plugins/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6042 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/core/plugins/storage/bcache.py
--rw-r--r--   0 runner    (1001) docker     (123)    38224 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/core/plugins/storage/ceph.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:46:34.186090 hotsos-1.15.post8/hotsos/core/plugins/system/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/core/plugins/system/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/core/plugins/system/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     6774 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/core/plugins/system/system.py
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/core/plugins/vault.py
--rw-r--r--   0 runner    (1001) docker     (123)    13866 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/core/plugintools.py
--rw-r--r--   0 runner    (1001) docker     (123)     2416 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/core/search.py
--rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:46:34.190090 hotsos-1.15.post8/hotsos/core/ycheck/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/core/ycheck/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:46:34.190090 hotsos-1.15.post8/hotsos/core/ycheck/engine/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/core/ycheck/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4094 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/core/ycheck/engine/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:46:34.190090 hotsos-1.15.post8/hotsos/core/ycheck/engine/properties/
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/core/ycheck/engine/properties/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6204 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/core/ycheck/engine/properties/checks.py
--rw-r--r--   0 runner    (1001) docker     (123)    24992 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/core/ycheck/engine/properties/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     7599 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/core/ycheck/engine/properties/conclusions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3251 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/core/ycheck/engine/properties/input.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:46:34.190090 hotsos-1.15.post8/hotsos/core/ycheck/engine/properties/requires/
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/core/ycheck/engine/properties/requires/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7507 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/core/ycheck/engine/properties/requires/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/core/ycheck/engine/properties/requires/requires.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:46:34.194090 hotsos-1.15.post8/hotsos/core/ycheck/engine/properties/requires/types/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/core/ycheck/engine/properties/requires/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/core/ycheck/engine/properties/requires/types/apt.py
--rw-r--r--   0 runner    (1001) docker     (123)     5904 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/core/ycheck/engine/properties/requires/types/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/core/ycheck/engine/properties/requires/types/path.py
--rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/core/ycheck/engine/properties/requires/types/pebble.py
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/core/ycheck/engine/properties/requires/types/property.py
--rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/core/ycheck/engine/properties/requires/types/snap.py
--rw-r--r--   0 runner    (1001) docker     (123)     5032 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/core/ycheck/engine/properties/requires/types/systemd.py
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/core/ycheck/engine/properties/requires/types/varops.py
--rw-r--r--   0 runner    (1001) docker     (123)    16584 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/core/ycheck/engine/properties/search.py
--rw-r--r--   0 runner    (1001) docker     (123)     2961 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/core/ycheck/engine/properties/vars.py
--rw-r--r--   0 runner    (1001) docker     (123)    14353 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/core/ycheck/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     5179 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/core/ycheck/scenarios.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:46:34.158090 hotsos-1.15.post8/hotsos/defs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:46:34.158090 hotsos-1.15.post8/hotsos/defs/events/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:46:34.194090 hotsos-1.15.post8/hotsos/defs/events/openstack/
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/defs/events/openstack/apache.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/defs/events/openstack/apparmor.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/defs/events/openstack/http-requests.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:46:34.194090 hotsos-1.15.post8/hotsos/defs/events/openstack/neutron/
--rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/defs/events/openstack/neutron/agents.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/defs/events/openstack/neutron/ml2-routers.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:46:34.194090 hotsos-1.15.post8/hotsos/defs/events/openstack/nova/
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/defs/events/openstack/nova/external-events.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:46:34.194090 hotsos-1.15.post8/hotsos/defs/events/openstack/nova/migrations/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:46:34.194090 hotsos-1.15.post8/hotsos/defs/events/openstack/nova/migrations/live-migration/
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/defs/events/openstack/nova/migrations/live-migration/dst-pre-live-migration.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/defs/events/openstack/nova/migrations/live-migration/src-migration.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/defs/events/openstack/nova/migrations/live-migration/src-post-live-migration.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/defs/events/openstack/nova/migrations/migrations.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/defs/events/openstack/nova/nova-compute.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/defs/events/openstack/octavia.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:46:34.158090 hotsos-1.15.post8/hotsos/defs/events/openvswitch/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:46:34.194090 hotsos-1.15.post8/hotsos/defs/events/openvswitch/ovn/
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/defs/events/openvswitch/ovn/errors-and-warnings.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/defs/events/openvswitch/ovn/ovn-central.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/defs/events/openvswitch/ovn/ovn-controller.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:46:34.198090 hotsos-1.15.post8/hotsos/defs/events/openvswitch/ovs/
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/defs/events/openvswitch/ovs/bfd.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/defs/events/openvswitch/ovs/datapath-checks.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/defs/events/openvswitch/ovs/errors-and-warnings.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/defs/events/openvswitch/ovs/ovs-vswitchd.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:46:34.158090 hotsos-1.15.post8/hotsos/defs/events/storage/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:46:34.158090 hotsos-1.15.post8/hotsos/defs/events/storage/ceph/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:46:34.198090 hotsos-1.15.post8/hotsos/defs/events/storage/ceph/mon/
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/defs/events/storage/ceph/mon/mon.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/defs/events/storage/ceph/mon/monlogs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:46:34.198090 hotsos-1.15.post8/hotsos/defs/events/storage/ceph/osd/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/defs/events/storage/ceph/osd/osd.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/defs/events/storage/ceph/osd/osdlogs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:46:34.166090 hotsos-1.15.post8/hotsos/defs/scenarios/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:46:34.198090 hotsos-1.15.post8/hotsos/defs/scenarios/juju/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:46:34.202090 hotsos-1.15.post8/hotsos/defs/scenarios/juju/bugs/
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/defs/scenarios/juju/bugs/lp1812361.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/defs/scenarios/juju/bugs/lp1852502.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/defs/scenarios/juju/bugs/lp1858519.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/defs/scenarios/juju/bugs/lp1895040.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/defs/scenarios/juju/bugs/lp1910958.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/defs/scenarios/juju/bugs/lp1948906.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/defs/scenarios/juju/bugs/lp1983140.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/defs/scenarios/juju/bugs/lp1983506.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/defs/scenarios/juju/bugs/lp1996230.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/defs/scenarios/juju/charm_unit_checks.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/defs/scenarios/juju/juju.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/defs/scenarios/juju/jujud_machine_checks.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:46:34.202090 hotsos-1.15.post8/hotsos/defs/scenarios/kernel/
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/defs/scenarios/kernel/amd_iommu_pt.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/defs/scenarios/kernel/disk_failure.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/defs/scenarios/kernel/kernlog_calltrace.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/defs/scenarios/kernel/memory.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:46:34.202090 hotsos-1.15.post8/hotsos/defs/scenarios/kernel/network/
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/defs/scenarios/kernel/network/misc.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     7336 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/defs/scenarios/kernel/network/tcp.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/defs/scenarios/kernel/network/udp.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/defs/scenarios/kernel/qla2xxx.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:46:34.202090 hotsos-1.15.post8/hotsos/defs/scenarios/kubernetes/
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/defs/scenarios/kubernetes/kubernetes.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/defs/scenarios/kubernetes/system_cpufreq_mode.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:46:34.202090 hotsos-1.15.post8/hotsos/defs/scenarios/lxd/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:46:34.202090 hotsos-1.15.post8/hotsos/defs/scenarios/lxd/bugs/
--rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/defs/scenarios/lxd/bugs/lp1807628.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/defs/scenarios/lxd/lxcfs_deadlock.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:46:34.202090 hotsos-1.15.post8/hotsos/defs/scenarios/mysql/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:46:34.202090 hotsos-1.15.post8/hotsos/defs/scenarios/mysql/bugs/
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/defs/scenarios/mysql/bugs/lp1959861.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/defs/scenarios/mysql/bugs/lp1971565.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/defs/scenarios/mysql/bugs/lp372017.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/defs/scenarios/mysql/mysql.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/defs/scenarios/mysql/mysql_connections.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:46:34.206091 hotsos-1.15.post8/hotsos/defs/scenarios/openstack/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:46:34.162090 hotsos-1.15.post8/hotsos/defs/scenarios/openstack/barbican/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:46:34.206091 hotsos-1.15.post8/hotsos/defs/scenarios/openstack/barbican/bugs/
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/defs/scenarios/openstack/barbican/bugs/lp1946787.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/defs/scenarios/openstack/eol.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:46:34.162090 hotsos-1.15.post8/hotsos/defs/scenarios/openstack/keystone/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:46:34.206091 hotsos-1.15.post8/hotsos/defs/scenarios/openstack/keystone/bugs/
--rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/defs/scenarios/openstack/keystone/bugs/lp1896125.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:46:34.206091 hotsos-1.15.post8/hotsos/defs/scenarios/openstack/masakari/
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/defs/scenarios/openstack/masakari/pacemaker_remote.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:46:34.206091 hotsos-1.15.post8/hotsos/defs/scenarios/openstack/neutron/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:46:34.210090 hotsos-1.15.post8/hotsos/defs/scenarios/openstack/neutron/bugs/
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/defs/scenarios/openstack/neutron/bugs/lp1794991.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/defs/scenarios/openstack/neutron/bugs/lp1883089.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/defs/scenarios/openstack/neutron/bugs/lp1896506.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/defs/scenarios/openstack/neutron/bugs/lp1907686.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/defs/scenarios/openstack/neutron/bugs/lp1927868.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/defs/scenarios/openstack/neutron/bugs/lp1928031.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/defs/scenarios/openstack/neutron/bugs/lp1929832.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/defs/scenarios/openstack/neutron/bugs/lp1960319.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/defs/scenarios/openstack/neutron/bugs/lp1965297.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/defs/scenarios/openstack/neutron/bugs/lp1979089.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/defs/scenarios/openstack/neutron/bugs/lp1993628.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/defs/scenarios/openstack/neutron/bugs/lp1996594.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/defs/scenarios/openstack/neutron/neutron_ovs_cleanup.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/defs/scenarios/openstack/neutron/ovn_stale_db.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:46:34.210090 hotsos-1.15.post8/hotsos/defs/scenarios/openstack/nova/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:46:34.210090 hotsos-1.15.post8/hotsos/defs/scenarios/openstack/nova/bugs/
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/defs/scenarios/openstack/nova/bugs/lp1860743.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/defs/scenarios/openstack/nova/bugs/lp1888395.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/defs/scenarios/openstack/nova/bugs/lp1904580.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/defs/scenarios/openstack/nova/bugs/lp1944619.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/defs/scenarios/openstack/nova/bugs/lp1967956.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/defs/scenarios/openstack/nova/config_checks.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6020 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/defs/scenarios/openstack/nova/cpu_pinning.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/defs/scenarios/openstack/nova/service_mem_usage.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:46:34.210090 hotsos-1.15.post8/hotsos/defs/scenarios/openstack/octavia/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:46:34.210090 hotsos-1.15.post8/hotsos/defs/scenarios/openstack/octavia/bugs/
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/defs/scenarios/openstack/octavia/bugs/sb1896125.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/defs/scenarios/openstack/octavia/excessive_failovers.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/defs/scenarios/openstack/octavia/hm_port_health.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/defs/scenarios/openstack/openstack.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/defs/scenarios/openstack/openstack_apache2_certificates.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/defs/scenarios/openstack/openstack_charm_conflicts.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/defs/scenarios/openstack/pkgs_from_mixed_releases_found.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2934 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/defs/scenarios/openstack/system_cpufreq_mode.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/defs/scenarios/openstack/systemd_masked_services.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:46:34.210090 hotsos-1.15.post8/hotsos/defs/scenarios/openvswitch/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:46:34.210090 hotsos-1.15.post8/hotsos/defs/scenarios/openvswitch/bugs/
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/defs/scenarios/openvswitch/bugs/lp1839592.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/defs/scenarios/openvswitch/bugs/lp1978806.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/defs/scenarios/openvswitch/dpif_lost_packets.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/defs/scenarios/openvswitch/dpif_resubmit_actions.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/defs/scenarios/openvswitch/openvswitch.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:46:34.214090 hotsos-1.15.post8/hotsos/defs/scenarios/openvswitch/ovn/
--rw-r--r--   0 runner    (1001) docker     (123)     3058 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/defs/scenarios/openvswitch/ovn/bfd_flapping.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:46:34.214090 hotsos-1.15.post8/hotsos/defs/scenarios/openvswitch/ovn/bugs/
--rw-r--r--   0 runner    (1001) docker     (123)      801 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/defs/scenarios/openvswitch/ovn/bugs/lp1865127.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/defs/scenarios/openvswitch/ovn/bugs/lp1917475.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3543 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/defs/scenarios/openvswitch/ovn/ovn_central_certs_logs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/defs/scenarios/openvswitch/ovn/ovn_central_services.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/defs/scenarios/openvswitch/ovn/ovn_certs_valid.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/defs/scenarios/openvswitch/ovn/ovn_chassis_certs_logs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/defs/scenarios/openvswitch/ovn/ovn_db_upgrade.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/defs/scenarios/openvswitch/ovn/ovn_elections.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/defs/scenarios/openvswitch/ovn/ovsdb_reconnect_errors.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/defs/scenarios/openvswitch/ovn/service_mem_usage.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/defs/scenarios/openvswitch/service_restarts.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:46:34.214090 hotsos-1.15.post8/hotsos/defs/scenarios/pacemaker/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:46:34.214090 hotsos-1.15.post8/hotsos/defs/scenarios/pacemaker/bugs/
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/defs/scenarios/pacemaker/bugs/lp1874719.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/defs/scenarios/pacemaker/pacemaker.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:46:34.214090 hotsos-1.15.post8/hotsos/defs/scenarios/rabbitmq/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:46:34.214090 hotsos-1.15.post8/hotsos/defs/scenarios/rabbitmq/bugs/
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/defs/scenarios/rabbitmq/bugs/lp1943937.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/defs/scenarios/rabbitmq/cluster_config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/defs/scenarios/rabbitmq/cluster_logchecks.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/defs/scenarios/rabbitmq/cluster_resources.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/defs/scenarios/rabbitmq/rabbitmq.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:46:34.214090 hotsos-1.15.post8/hotsos/defs/scenarios/sosreport/
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/defs/scenarios/sosreport/plugin_timeouts.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:46:34.214090 hotsos-1.15.post8/hotsos/defs/scenarios/storage/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:46:34.218091 hotsos-1.15.post8/hotsos/defs/scenarios/storage/bcache/
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/defs/scenarios/storage/bcache/bcache.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/defs/scenarios/storage/bcache/bdev.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/defs/scenarios/storage/bcache/cacheset.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:46:34.166090 hotsos-1.15.post8/hotsos/defs/scenarios/storage/ceph/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:46:34.218091 hotsos-1.15.post8/hotsos/defs/scenarios/storage/ceph/ceph-mgr/
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/defs/scenarios/storage/ceph/ceph-mgr/autoscaler_overlap_roots.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:46:34.222091 hotsos-1.15.post8/hotsos/defs/scenarios/storage/ceph/ceph-mon/
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/defs/scenarios/storage/ceph/ceph-mon/auth_insecure_global_id_reclaim_allowed.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/defs/scenarios/storage/ceph/ceph-mon/autoscaler_bug.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/defs/scenarios/storage/ceph/ceph-mon/bluefs_size.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/defs/scenarios/storage/ceph/ceph-mon/bluefs_spillover.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/defs/scenarios/storage/ceph/ceph-mon/ceph-mon.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/defs/scenarios/storage/ceph/ceph-mon/ceph_address_overlap.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/defs/scenarios/storage/ceph/ceph-mon/ceph_cluster_health.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/defs/scenarios/storage/ceph/ceph-mon/ceph_versions_mismatch.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/defs/scenarios/storage/ceph/ceph-mon/crushmap_bucket_checks.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      909 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/defs/scenarios/storage/ceph/ceph-mon/empty_clog.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/defs/scenarios/storage/ceph/ceph-mon/eol.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/defs/scenarios/storage/ceph/ceph-mon/laggy_pgs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/defs/scenarios/storage/ceph/ceph-mon/large_omap_objects.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/defs/scenarios/storage/ceph/ceph-mon/meta_backend_mon.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/defs/scenarios/storage/ceph/ceph-mon/mon_db_too_big.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/defs/scenarios/storage/ceph/ceph-mon/mon_elections_flapping.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/defs/scenarios/storage/ceph/ceph-mon/osd_flapping.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/defs/scenarios/storage/ceph/ceph-mon/osd_maps_backlog_too_large.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      825 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/defs/scenarios/storage/ceph/ceph-mon/osd_messenger_v2_protocol.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/defs/scenarios/storage/ceph/ceph-mon/osd_slow_heartbeats.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/defs/scenarios/storage/ceph/ceph-mon/osd_slow_ops.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/defs/scenarios/storage/ceph/ceph-mon/pg_imbalance.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/defs/scenarios/storage/ceph/ceph-mon/pg_overdose.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/defs/scenarios/storage/ceph/ceph-mon/required_osd_release_mismatch.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/defs/scenarios/storage/ceph/ceph-mon/rgw_frontend.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/defs/scenarios/storage/ceph/ceph-mon/ssds_using_bcache.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/defs/scenarios/storage/ceph/ceph-mon/unresponsive_mon_mgr.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:46:34.226091 hotsos-1.15.post8/hotsos/defs/scenarios/storage/ceph/ceph-osd/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:46:34.226091 hotsos-1.15.post8/hotsos/defs/scenarios/storage/ceph/ceph-osd/bugs/
--rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/defs/scenarios/storage/ceph/ceph-osd/bugs/lp1936136.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/defs/scenarios/storage/ceph/ceph-osd/bugs/lp1959649.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/defs/scenarios/storage/ceph/ceph-osd/bugs/lp1996010.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/defs/scenarios/storage/ceph/ceph-osd/bugs/lp2013960.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/defs/scenarios/storage/ceph/ceph-osd/bugs/lp2016845.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/defs/scenarios/storage/ceph/ceph-osd/ceph-osd.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/defs/scenarios/storage/ceph/ceph-osd/ceph_address_overlap.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/defs/scenarios/storage/ceph/ceph-osd/eol.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/defs/scenarios/storage/ceph/ceph-osd/filestore_to_bluestore_upgrade.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/defs/scenarios/storage/ceph/ceph-osd/juju_ceph_no_bcache_tuning.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/defs/scenarios/storage/ceph/ceph-osd/meta_backend_osd.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/defs/scenarios/storage/ceph/ceph-osd/osd_flapping.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/defs/scenarios/storage/ceph/ceph-osd/osd_latency.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/defs/scenarios/storage/ceph/ceph-osd/osd_slow_ops.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/defs/scenarios/storage/ceph/ceph-osd/pg_overdose.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/defs/scenarios/storage/ceph/ceph-osd/ssd_osds_no_discard.yaml.disabled
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/defs/scenarios/storage/ceph/ceph-osd/system_cpufreq_mode.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:46:34.226091 hotsos-1.15.post8/hotsos/defs/scenarios/storage/ceph/ceph-rgw/
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/defs/scenarios/storage/ceph/ceph-rgw/rgw_frontend_rgw.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:46:34.226091 hotsos-1.15.post8/hotsos/defs/scenarios/storage/ceph/common/
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/defs/scenarios/storage/ceph/common/ceph_charm_conflicts.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/defs/scenarios/storage/storage.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:46:34.226091 hotsos-1.15.post8/hotsos/defs/scenarios/system/
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/defs/scenarios/system/system.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/defs/scenarios/system/unattended_upgrades.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:46:34.230091 hotsos-1.15.post8/hotsos/plugin_extensions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/plugin_extensions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:46:34.230091 hotsos-1.15.post8/hotsos/plugin_extensions/juju/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/plugin_extensions/juju/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5260 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/plugin_extensions/juju/summary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:46:34.230091 hotsos-1.15.post8/hotsos/plugin_extensions/kernel/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/plugin_extensions/kernel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/plugin_extensions/kernel/summary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:46:34.230091 hotsos-1.15.post8/hotsos/plugin_extensions/kubernetes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/plugin_extensions/kubernetes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/plugin_extensions/kubernetes/summary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:46:34.230091 hotsos-1.15.post8/hotsos/plugin_extensions/lxd/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/plugin_extensions/lxd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/plugin_extensions/lxd/summary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:46:34.230091 hotsos-1.15.post8/hotsos/plugin_extensions/maas/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/plugin_extensions/maas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/plugin_extensions/maas/summary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:46:34.230091 hotsos-1.15.post8/hotsos/plugin_extensions/mysql/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/plugin_extensions/mysql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/plugin_extensions/mysql/summary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:46:34.230091 hotsos-1.15.post8/hotsos/plugin_extensions/openstack/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/plugin_extensions/openstack/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:46:34.234091 hotsos-1.15.post8/hotsos/plugin_extensions/openstack/agent/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/plugin_extensions/openstack/agent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12200 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/plugin_extensions/openstack/agent/events.py
--rw-r--r--   0 runner    (1001) docker     (123)    11602 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/plugin_extensions/openstack/agent/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3420 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/plugin_extensions/openstack/nova_external_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/plugin_extensions/openstack/service_features.py
--rw-r--r--   0 runner    (1001) docker     (123)     3959 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/plugin_extensions/openstack/service_network_checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/plugin_extensions/openstack/summary.py
--rw-r--r--   0 runner    (1001) docker     (123)     7226 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/plugin_extensions/openstack/vm_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:46:34.234091 hotsos-1.15.post8/hotsos/plugin_extensions/openvswitch/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/plugin_extensions/openvswitch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10003 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/plugin_extensions/openvswitch/event_checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3054 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/plugin_extensions/openvswitch/summary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:46:34.234091 hotsos-1.15.post8/hotsos/plugin_extensions/pacemaker/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/plugin_extensions/pacemaker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/plugin_extensions/pacemaker/summary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:46:34.234091 hotsos-1.15.post8/hotsos/plugin_extensions/rabbitmq/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/plugin_extensions/rabbitmq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/plugin_extensions/rabbitmq/summary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:46:34.234091 hotsos-1.15.post8/hotsos/plugin_extensions/sosreport/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/plugin_extensions/sosreport/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/plugin_extensions/sosreport/summary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:46:34.234091 hotsos-1.15.post8/hotsos/plugin_extensions/storage/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/plugin_extensions/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/plugin_extensions/storage/bcache_summary.py
--rw-r--r--   0 runner    (1001) docker     (123)     4472 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/plugin_extensions/storage/ceph_event_checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/plugin_extensions/storage/ceph_summary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:46:34.234091 hotsos-1.15.post8/hotsos/plugin_extensions/system/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/plugin_extensions/system/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6474 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/plugin_extensions/system/checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/plugin_extensions/system/summary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:46:34.234091 hotsos-1.15.post8/hotsos/plugin_extensions/vault/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/plugin_extensions/vault/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/plugin_extensions/vault/summary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:46:34.238091 hotsos-1.15.post8/hotsos/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/templates/content_dict.html
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/templates/content_list.html
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/templates/footer.html
--rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-07-05 12:46:08.000000 hotsos-1.15.post8/hotsos/templates/header.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:46:34.170090 hotsos-1.15.post8/hotsos.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-07-05 12:46:34.000000 hotsos-1.15.post8/hotsos.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15380 2023-07-05 12:46:34.000000 hotsos-1.15.post8/hotsos.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 12:46:34.000000 hotsos-1.15.post8/hotsos.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-05 12:46:34.000000 hotsos-1.15.post8/hotsos.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-05 12:46:34.000000 hotsos-1.15.post8/hotsos.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-05 12:46:34.000000 hotsos-1.15.post8/hotsos.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-07-05 12:46:08.000000 hotsos-1.15.post8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 12:46:34.238091 hotsos-1.15.post8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-05 12:46:08.000000 hotsos-1.15.post8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.430256 hotsos-1.15.post9/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-06 08:59:40.000000 hotsos-1.15.post9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-06 08:59:40.000000 hotsos-1.15.post9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-07-06 09:00:02.430256 hotsos-1.15.post9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-07-06 08:59:40.000000 hotsos-1.15.post9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.394256 hotsos-1.15.post9/hotsos/
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-06 08:59:45.000000 hotsos-1.15.post9/hotsos/.repo-info
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15110 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/cli.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15371 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.398256 hotsos-1.15.post9/hotsos/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10727 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/core/analytics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10126 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/core/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/core/factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.398256 hotsos-1.15.post9/hotsos/core/host_helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/core/host_helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35388 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/core/host_helpers/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3068 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/core/host_helpers/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4694 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/core/host_helpers/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/core/host_helpers/filestat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11021 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/core/host_helpers/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13241 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/core/host_helpers/packaging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3346 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/core/host_helpers/pebble.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/core/host_helpers/ssl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/core/host_helpers/sysctl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11368 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/core/host_helpers/systemd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/core/host_helpers/uptime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.398256 hotsos-1.15.post9/hotsos/core/issues/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/core/issues/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2961 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/core/issues/issue_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5118 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/core/issues/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/core/log.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.398256 hotsos-1.15.post9/hotsos/core/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/core/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.398256 hotsos-1.15.post9/hotsos/core/plugins/juju/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/core/plugins/juju/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/core/plugins/juju/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6396 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/core/plugins/juju/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.402256 hotsos-1.15.post9/hotsos/core/plugins/kernel/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/core/plugins/kernel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/core/plugins/kernel/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/core/plugins/kernel/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.402256 hotsos-1.15.post9/hotsos/core/plugins/kernel/kernlog/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/core/plugins/kernel/kernlog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14852 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/core/plugins/kernel/kernlog/calltrace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3835 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/core/plugins/kernel/kernlog/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/core/plugins/kernel/kernlog/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7491 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/core/plugins/kernel/memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20366 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/core/plugins/kernel/net.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/core/plugins/kernel/sysfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/core/plugins/kubernetes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.402256 hotsos-1.15.post9/hotsos/core/plugins/lxd/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/core/plugins/lxd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/core/plugins/lxd/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/core/plugins/maas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/core/plugins/mysql.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.402256 hotsos-1.15.post9/hotsos/core/plugins/openstack/
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/core/plugins/openstack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8193 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/core/plugins/openstack/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63860 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/core/plugins/openstack/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3799 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/core/plugins/openstack/neutron.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10636 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/core/plugins/openstack/nova.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/core/plugins/openstack/octavia.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19464 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/core/plugins/openstack/openstack.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.402256 hotsos-1.15.post9/hotsos/core/plugins/openvswitch/
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/core/plugins/openvswitch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/core/plugins/openvswitch/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4809 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/core/plugins/openvswitch/ovn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4804 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/core/plugins/openvswitch/ovs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/core/plugins/pacemaker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.402256 hotsos-1.15.post9/hotsos/core/plugins/rabbitmq/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/core/plugins/rabbitmq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/core/plugins/rabbitmq/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9001 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/core/plugins/rabbitmq/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/core/plugins/sosreport.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.402256 hotsos-1.15.post9/hotsos/core/plugins/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/core/plugins/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6042 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/core/plugins/storage/bcache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38316 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/core/plugins/storage/ceph.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.402256 hotsos-1.15.post9/hotsos/core/plugins/system/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/core/plugins/system/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/core/plugins/system/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6752 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/core/plugins/system/system.py
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/core/plugins/vault.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13833 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/core/plugintools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2416 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/core/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.406256 hotsos-1.15.post9/hotsos/core/ycheck/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/core/ycheck/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.406256 hotsos-1.15.post9/hotsos/core/ycheck/engine/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/core/ycheck/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4094 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/core/ycheck/engine/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.406256 hotsos-1.15.post9/hotsos/core/ycheck/engine/properties/
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/core/ycheck/engine/properties/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6252 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/core/ycheck/engine/properties/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24973 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/core/ycheck/engine/properties/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7608 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/core/ycheck/engine/properties/conclusions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3251 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/core/ycheck/engine/properties/inputdef.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.406256 hotsos-1.15.post9/hotsos/core/ycheck/engine/properties/requires/
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/core/ycheck/engine/properties/requires/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7537 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/core/ycheck/engine/properties/requires/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/core/ycheck/engine/properties/requires/requires.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.406256 hotsos-1.15.post9/hotsos/core/ycheck/engine/properties/requires/types/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/core/ycheck/engine/properties/requires/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/core/ycheck/engine/properties/requires/types/apt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5906 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/core/ycheck/engine/properties/requires/types/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/core/ycheck/engine/properties/requires/types/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/core/ycheck/engine/properties/requires/types/pebble.py
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/core/ycheck/engine/properties/requires/types/property.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/core/ycheck/engine/properties/requires/types/snap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5034 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/core/ycheck/engine/properties/requires/types/systemd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/core/ycheck/engine/properties/requires/types/varops.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16533 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/core/ycheck/engine/properties/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2961 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/core/ycheck/engine/properties/vardef.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14358 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/core/ycheck/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5179 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/core/ycheck/scenarios.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.390256 hotsos-1.15.post9/hotsos/defs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.390256 hotsos-1.15.post9/hotsos/defs/events/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.406256 hotsos-1.15.post9/hotsos/defs/events/openstack/
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/events/openstack/apache.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/events/openstack/apparmor.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/events/openstack/http-requests.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.406256 hotsos-1.15.post9/hotsos/defs/events/openstack/neutron/
+-rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/events/openstack/neutron/agents.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/events/openstack/neutron/ml2-routers.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.406256 hotsos-1.15.post9/hotsos/defs/events/openstack/nova/
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/events/openstack/nova/external-events.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.406256 hotsos-1.15.post9/hotsos/defs/events/openstack/nova/migrations/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.406256 hotsos-1.15.post9/hotsos/defs/events/openstack/nova/migrations/live-migration/
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/events/openstack/nova/migrations/live-migration/dst-pre-live-migration.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/events/openstack/nova/migrations/live-migration/src-migration.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/events/openstack/nova/migrations/live-migration/src-post-live-migration.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/events/openstack/nova/migrations/migrations.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/events/openstack/nova/nova-compute.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/events/openstack/octavia.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.390256 hotsos-1.15.post9/hotsos/defs/events/openvswitch/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.410256 hotsos-1.15.post9/hotsos/defs/events/openvswitch/ovn/
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/events/openvswitch/ovn/errors-and-warnings.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/events/openvswitch/ovn/ovn-central.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/events/openvswitch/ovn/ovn-controller.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.410256 hotsos-1.15.post9/hotsos/defs/events/openvswitch/ovs/
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/events/openvswitch/ovs/bfd.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/events/openvswitch/ovs/datapath-checks.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/events/openvswitch/ovs/errors-and-warnings.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/events/openvswitch/ovs/ovs-vswitchd.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.390256 hotsos-1.15.post9/hotsos/defs/events/storage/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.390256 hotsos-1.15.post9/hotsos/defs/events/storage/ceph/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.410256 hotsos-1.15.post9/hotsos/defs/events/storage/ceph/mon/
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/events/storage/ceph/mon/mon.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/events/storage/ceph/mon/monlogs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.410256 hotsos-1.15.post9/hotsos/defs/events/storage/ceph/osd/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/events/storage/ceph/osd/osd.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/events/storage/ceph/osd/osdlogs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.390256 hotsos-1.15.post9/hotsos/defs/scenarios/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.410256 hotsos-1.15.post9/hotsos/defs/scenarios/juju/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.410256 hotsos-1.15.post9/hotsos/defs/scenarios/juju/bugs/
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/juju/bugs/lp1812361.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/juju/bugs/lp1852502.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/juju/bugs/lp1858519.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/juju/bugs/lp1895040.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/juju/bugs/lp1910958.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/juju/bugs/lp1948906.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/juju/bugs/lp1983140.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/juju/bugs/lp1983506.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/juju/bugs/lp1996230.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/juju/charm_unit_checks.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/juju/juju.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/juju/jujud_machine_checks.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.410256 hotsos-1.15.post9/hotsos/defs/scenarios/kernel/
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/kernel/amd_iommu_pt.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/kernel/disk_failure.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/kernel/kernlog_calltrace.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/kernel/memory.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.410256 hotsos-1.15.post9/hotsos/defs/scenarios/kernel/network/
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/kernel/network/misc.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     7336 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/kernel/network/tcp.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/kernel/network/udp.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/kernel/qla2xxx.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.410256 hotsos-1.15.post9/hotsos/defs/scenarios/kubernetes/
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/kubernetes/kubernetes.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/kubernetes/system_cpufreq_mode.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.410256 hotsos-1.15.post9/hotsos/defs/scenarios/lxd/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.410256 hotsos-1.15.post9/hotsos/defs/scenarios/lxd/bugs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/lxd/bugs/lp1807628.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/lxd/lxcfs_deadlock.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.410256 hotsos-1.15.post9/hotsos/defs/scenarios/mysql/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.414256 hotsos-1.15.post9/hotsos/defs/scenarios/mysql/bugs/
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/mysql/bugs/lp1959861.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/mysql/bugs/lp1971565.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/mysql/bugs/lp372017.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/mysql/mysql.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/mysql/mysql_connections.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.414256 hotsos-1.15.post9/hotsos/defs/scenarios/openstack/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.390256 hotsos-1.15.post9/hotsos/defs/scenarios/openstack/barbican/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.414256 hotsos-1.15.post9/hotsos/defs/scenarios/openstack/barbican/bugs/
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/openstack/barbican/bugs/lp1946787.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/openstack/eol.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.390256 hotsos-1.15.post9/hotsos/defs/scenarios/openstack/keystone/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.414256 hotsos-1.15.post9/hotsos/defs/scenarios/openstack/keystone/bugs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/openstack/keystone/bugs/lp1896125.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.414256 hotsos-1.15.post9/hotsos/defs/scenarios/openstack/masakari/
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/openstack/masakari/pacemaker_remote.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.414256 hotsos-1.15.post9/hotsos/defs/scenarios/openstack/neutron/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.414256 hotsos-1.15.post9/hotsos/defs/scenarios/openstack/neutron/bugs/
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/openstack/neutron/bugs/lp1794991.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/openstack/neutron/bugs/lp1883089.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/openstack/neutron/bugs/lp1896506.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/openstack/neutron/bugs/lp1907686.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/openstack/neutron/bugs/lp1927868.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/openstack/neutron/bugs/lp1928031.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/openstack/neutron/bugs/lp1929832.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/openstack/neutron/bugs/lp1960319.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/openstack/neutron/bugs/lp1965297.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/openstack/neutron/bugs/lp1979089.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/openstack/neutron/bugs/lp1993628.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/openstack/neutron/bugs/lp1996594.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/openstack/neutron/neutron_ovs_cleanup.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/openstack/neutron/ovn_stale_db.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.414256 hotsos-1.15.post9/hotsos/defs/scenarios/openstack/nova/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.414256 hotsos-1.15.post9/hotsos/defs/scenarios/openstack/nova/bugs/
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/openstack/nova/bugs/lp1860743.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/openstack/nova/bugs/lp1888395.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/openstack/nova/bugs/lp1904580.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/openstack/nova/bugs/lp1944619.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/openstack/nova/bugs/lp1967956.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/openstack/nova/config_checks.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6020 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/openstack/nova/cpu_pinning.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/openstack/nova/service_mem_usage.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.414256 hotsos-1.15.post9/hotsos/defs/scenarios/openstack/octavia/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.414256 hotsos-1.15.post9/hotsos/defs/scenarios/openstack/octavia/bugs/
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/openstack/octavia/bugs/sb1896125.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/openstack/octavia/excessive_failovers.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/openstack/octavia/hm_port_health.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/openstack/openstack.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/openstack/openstack_apache2_certificates.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/openstack/openstack_charm_conflicts.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/openstack/pkgs_from_mixed_releases_found.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2934 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/openstack/system_cpufreq_mode.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/openstack/systemd_masked_services.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.418256 hotsos-1.15.post9/hotsos/defs/scenarios/openvswitch/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.418256 hotsos-1.15.post9/hotsos/defs/scenarios/openvswitch/bugs/
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/openvswitch/bugs/lp1839592.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/openvswitch/bugs/lp1978806.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/openvswitch/dpif_lost_packets.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/openvswitch/dpif_resubmit_actions.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/openvswitch/openvswitch.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.418256 hotsos-1.15.post9/hotsos/defs/scenarios/openvswitch/ovn/
+-rw-r--r--   0 runner    (1001) docker     (123)     3058 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/openvswitch/ovn/bfd_flapping.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.418256 hotsos-1.15.post9/hotsos/defs/scenarios/openvswitch/ovn/bugs/
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/openvswitch/ovn/bugs/lp1865127.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/openvswitch/ovn/bugs/lp1917475.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3543 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/openvswitch/ovn/ovn_central_certs_logs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/openvswitch/ovn/ovn_central_services.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/openvswitch/ovn/ovn_certs_valid.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/openvswitch/ovn/ovn_chassis_certs_logs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/openvswitch/ovn/ovn_db_upgrade.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/openvswitch/ovn/ovn_elections.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/openvswitch/ovn/ovsdb_reconnect_errors.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/openvswitch/ovn/service_mem_usage.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/openvswitch/service_restarts.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.418256 hotsos-1.15.post9/hotsos/defs/scenarios/pacemaker/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.418256 hotsos-1.15.post9/hotsos/defs/scenarios/pacemaker/bugs/
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/pacemaker/bugs/lp1874719.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/pacemaker/pacemaker.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.418256 hotsos-1.15.post9/hotsos/defs/scenarios/rabbitmq/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.418256 hotsos-1.15.post9/hotsos/defs/scenarios/rabbitmq/bugs/
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/rabbitmq/bugs/lp1943937.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/rabbitmq/cluster_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/rabbitmq/cluster_logchecks.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/rabbitmq/cluster_resources.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/rabbitmq/rabbitmq.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.418256 hotsos-1.15.post9/hotsos/defs/scenarios/sosreport/
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/sosreport/plugin_timeouts.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.418256 hotsos-1.15.post9/hotsos/defs/scenarios/storage/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.418256 hotsos-1.15.post9/hotsos/defs/scenarios/storage/bcache/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/storage/bcache/bcache.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/storage/bcache/bdev.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/storage/bcache/cacheset.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.390256 hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.418256 hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-mgr/
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-mgr/autoscaler_overlap_roots.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.422256 hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/auth_insecure_global_id_reclaim_allowed.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/autoscaler_bug.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/bluefs_size.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/bluefs_spillover.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/ceph-mon.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/ceph_address_overlap.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/ceph_cluster_health.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/ceph_versions_mismatch.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/crushmap_bucket_checks.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/empty_clog.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/eol.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/laggy_pgs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/large_omap_objects.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/meta_backend_mon.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/mon_db_too_big.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/mon_elections_flapping.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/osd_flapping.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/osd_maps_backlog_too_large.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      825 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/osd_messenger_v2_protocol.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/osd_slow_heartbeats.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-07-06 08:59:41.000000 hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/osd_slow_ops.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-07-06 08:59:41.000000 hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/pg_imbalance.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-07-06 08:59:41.000000 hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/pg_overdose.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-06 08:59:41.000000 hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/required_osd_release_mismatch.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-07-06 08:59:41.000000 hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/rgw_frontend.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-06 08:59:41.000000 hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/ssds_using_bcache.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-07-06 08:59:41.000000 hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/unresponsive_mon_mgr.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.422256 hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-osd/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.426256 hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-osd/bugs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-07-06 08:59:41.000000 hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-osd/bugs/lp1936136.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-07-06 08:59:41.000000 hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-osd/bugs/lp1959649.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-07-06 08:59:41.000000 hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-osd/bugs/lp1996010.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-07-06 08:59:41.000000 hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-osd/bugs/lp2013960.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-07-06 08:59:41.000000 hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-osd/bugs/lp2016845.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-06 08:59:41.000000 hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-osd/ceph-osd.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-osd/ceph_address_overlap.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-osd/eol.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-06 08:59:41.000000 hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-osd/filestore_to_bluestore_upgrade.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-07-06 08:59:41.000000 hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-osd/juju_ceph_no_bcache_tuning.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-07-06 08:59:41.000000 hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-osd/meta_backend_osd.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-osd/osd_flapping.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-07-06 08:59:41.000000 hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-osd/osd_latency.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-07-06 08:59:41.000000 hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-osd/osd_slow_ops.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-07-06 08:59:41.000000 hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-osd/pg_overdose.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-07-06 08:59:41.000000 hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-osd/ssd_osds_no_discard.yaml.disabled
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-07-06 08:59:41.000000 hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-osd/system_cpufreq_mode.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.426256 hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-rgw/
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-07-06 08:59:41.000000 hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-rgw/rgw_frontend_rgw.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.426256 hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/common/
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-07-06 08:59:41.000000 hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/common/ceph_charm_conflicts.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-07-06 08:59:41.000000 hotsos-1.15.post9/hotsos/defs/scenarios/storage/storage.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.426256 hotsos-1.15.post9/hotsos/defs/scenarios/system/
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-07-06 08:59:41.000000 hotsos-1.15.post9/hotsos/defs/scenarios/system/system.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-07-06 08:59:41.000000 hotsos-1.15.post9/hotsos/defs/scenarios/system/unattended_upgrades.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.426256 hotsos-1.15.post9/hotsos/plugin_extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 08:59:41.000000 hotsos-1.15.post9/hotsos/plugin_extensions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.426256 hotsos-1.15.post9/hotsos/plugin_extensions/juju/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 08:59:41.000000 hotsos-1.15.post9/hotsos/plugin_extensions/juju/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5256 2023-07-06 08:59:41.000000 hotsos-1.15.post9/hotsos/plugin_extensions/juju/summary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.426256 hotsos-1.15.post9/hotsos/plugin_extensions/kernel/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 08:59:41.000000 hotsos-1.15.post9/hotsos/plugin_extensions/kernel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-07-06 08:59:41.000000 hotsos-1.15.post9/hotsos/plugin_extensions/kernel/summary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.426256 hotsos-1.15.post9/hotsos/plugin_extensions/kubernetes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 08:59:41.000000 hotsos-1.15.post9/hotsos/plugin_extensions/kubernetes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-07-06 08:59:41.000000 hotsos-1.15.post9/hotsos/plugin_extensions/kubernetes/summary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.426256 hotsos-1.15.post9/hotsos/plugin_extensions/lxd/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 08:59:41.000000 hotsos-1.15.post9/hotsos/plugin_extensions/lxd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-07-06 08:59:41.000000 hotsos-1.15.post9/hotsos/plugin_extensions/lxd/summary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.426256 hotsos-1.15.post9/hotsos/plugin_extensions/maas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 08:59:41.000000 hotsos-1.15.post9/hotsos/plugin_extensions/maas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-06 08:59:41.000000 hotsos-1.15.post9/hotsos/plugin_extensions/maas/summary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.426256 hotsos-1.15.post9/hotsos/plugin_extensions/mysql/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 08:59:41.000000 hotsos-1.15.post9/hotsos/plugin_extensions/mysql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-07-06 08:59:41.000000 hotsos-1.15.post9/hotsos/plugin_extensions/mysql/summary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.426256 hotsos-1.15.post9/hotsos/plugin_extensions/openstack/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 08:59:41.000000 hotsos-1.15.post9/hotsos/plugin_extensions/openstack/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.426256 hotsos-1.15.post9/hotsos/plugin_extensions/openstack/agent/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 08:59:41.000000 hotsos-1.15.post9/hotsos/plugin_extensions/openstack/agent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12198 2023-07-06 08:59:41.000000 hotsos-1.15.post9/hotsos/plugin_extensions/openstack/agent/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11600 2023-07-06 08:59:41.000000 hotsos-1.15.post9/hotsos/plugin_extensions/openstack/agent/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-07-06 08:59:41.000000 hotsos-1.15.post9/hotsos/plugin_extensions/openstack/nova_external_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-07-06 08:59:41.000000 hotsos-1.15.post9/hotsos/plugin_extensions/openstack/service_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3959 2023-07-06 08:59:41.000000 hotsos-1.15.post9/hotsos/plugin_extensions/openstack/service_network_checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-07-06 08:59:41.000000 hotsos-1.15.post9/hotsos/plugin_extensions/openstack/summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7226 2023-07-06 08:59:41.000000 hotsos-1.15.post9/hotsos/plugin_extensions/openstack/vm_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.426256 hotsos-1.15.post9/hotsos/plugin_extensions/openvswitch/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 08:59:41.000000 hotsos-1.15.post9/hotsos/plugin_extensions/openvswitch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9976 2023-07-06 08:59:41.000000 hotsos-1.15.post9/hotsos/plugin_extensions/openvswitch/event_checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-07-06 08:59:41.000000 hotsos-1.15.post9/hotsos/plugin_extensions/openvswitch/summary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.426256 hotsos-1.15.post9/hotsos/plugin_extensions/pacemaker/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 08:59:41.000000 hotsos-1.15.post9/hotsos/plugin_extensions/pacemaker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-07-06 08:59:41.000000 hotsos-1.15.post9/hotsos/plugin_extensions/pacemaker/summary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.426256 hotsos-1.15.post9/hotsos/plugin_extensions/rabbitmq/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 08:59:41.000000 hotsos-1.15.post9/hotsos/plugin_extensions/rabbitmq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-07-06 08:59:41.000000 hotsos-1.15.post9/hotsos/plugin_extensions/rabbitmq/summary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.430256 hotsos-1.15.post9/hotsos/plugin_extensions/sosreport/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 08:59:41.000000 hotsos-1.15.post9/hotsos/plugin_extensions/sosreport/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-06 08:59:41.000000 hotsos-1.15.post9/hotsos/plugin_extensions/sosreport/summary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.430256 hotsos-1.15.post9/hotsos/plugin_extensions/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 08:59:41.000000 hotsos-1.15.post9/hotsos/plugin_extensions/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-07-06 08:59:41.000000 hotsos-1.15.post9/hotsos/plugin_extensions/storage/bcache_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4472 2023-07-06 08:59:41.000000 hotsos-1.15.post9/hotsos/plugin_extensions/storage/ceph_event_checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-07-06 08:59:41.000000 hotsos-1.15.post9/hotsos/plugin_extensions/storage/ceph_summary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.430256 hotsos-1.15.post9/hotsos/plugin_extensions/system/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 08:59:41.000000 hotsos-1.15.post9/hotsos/plugin_extensions/system/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6474 2023-07-06 08:59:41.000000 hotsos-1.15.post9/hotsos/plugin_extensions/system/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-07-06 08:59:41.000000 hotsos-1.15.post9/hotsos/plugin_extensions/system/summary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.430256 hotsos-1.15.post9/hotsos/plugin_extensions/vault/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 08:59:41.000000 hotsos-1.15.post9/hotsos/plugin_extensions/vault/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-07-06 08:59:41.000000 hotsos-1.15.post9/hotsos/plugin_extensions/vault/summary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.430256 hotsos-1.15.post9/hotsos/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-06 08:59:41.000000 hotsos-1.15.post9/hotsos/templates/content_dict.html
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-06 08:59:41.000000 hotsos-1.15.post9/hotsos/templates/content_list.html
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-06 08:59:41.000000 hotsos-1.15.post9/hotsos/templates/footer.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-07-06 08:59:41.000000 hotsos-1.15.post9/hotsos/templates/header.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.394256 hotsos-1.15.post9/hotsos.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-07-06 09:00:02.000000 hotsos-1.15.post9/hotsos.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15385 2023-07-06 09:00:02.000000 hotsos-1.15.post9/hotsos.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 09:00:02.000000 hotsos-1.15.post9/hotsos.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-06 09:00:02.000000 hotsos-1.15.post9/hotsos.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-06 09:00:02.000000 hotsos-1.15.post9/hotsos.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-06 09:00:02.000000 hotsos-1.15.post9/hotsos.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-07-06 08:59:41.000000 hotsos-1.15.post9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 09:00:02.430256 hotsos-1.15.post9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-06 08:59:41.000000 hotsos-1.15.post9/setup.py
```

### Comparing `hotsos-1.15.post8/LICENSE` & `hotsos-1.15.post9/LICENSE`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post8/PKG-INFO` & `hotsos-1.15.post9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hotsos
-Version: 1.15.post8
+Version: 1.15.post9
 Summary: Software analysis toolkit. Define checks in high-level language and leverage library to perform analysis of common Cloud applications.
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Hotsos
```

### Comparing `hotsos-1.15.post8/README.md` & `hotsos-1.15.post9/README.md`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post8/hotsos/cli.py` & `hotsos-1.15.post9/hotsos/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,15 +72,15 @@
 
     return out.decode().strip()
 
 
 def set_plugin_options(f):
     for plugin in PLUGIN_CATALOG:
         click.option('--{}'.format(plugin), default=False, is_flag=True,
-                     help=('Run the {} plugin.'.format(plugin)))(f)
+                     help='Run the {} plugin.'.format(plugin))(f)
 
     return f
 
 
 def get_defs_path():
     # source
     defs = os.path.join(get_hotsos_root(), 'defs')
@@ -116,19 +116,19 @@
     if not os.path.exists(templates):
         raise Exception("templates path {} not found".format(templates))
 
     return templates
 
 
 def spinner(msg, done):
-    spinner = Spinner(msg)
+    cli_spinner = Spinner(msg)
     while not done.is_set():
-        spinner.next()
+        cli_spinner.next()
         done.wait(timeout=0.1)
-    spinner.finish()
+    cli_spinner.finish()
 
 
 @contextlib.contextmanager
 def progress_spinner(show_spinner, spinner_msg):
     if not show_spinner:
         yield
         return
@@ -177,29 +177,29 @@
                         'timing out and moving on.'))
     @click.option('--allow-constraints-for-unverifiable-logs', default=False,
                   is_flag=True)
     @click.option('--output-path', default=None,
                   help=('Optional path to use for saving output (with '
                         '--save).'))
     @click.option('--machine-readable', default=False, is_flag=True,
-                  help=("Don't format output for humans."))
+                  help="Don't format output for humans.")
     @click.option('--list-plugins', default=False, is_flag=True,
-                  help=('Show available plugins.'))
+                  help='Show available plugins.')
     @click.option('--max-parallel-tasks', default=8,
                   help=('The search module will execute searches across '
                         'files in parallel. By default the number of cores '
                         'used is limited to a max of 8. You can '
                         'override that value with this option.'))
     @click.option('--max-logrotate-depth', default=7,
                   help=('Searching all available logrotate history for a '
                         'given log file can be costly so we cap the history '
                         'to this value. Only applies when --all-logs is '
                         'provided.'))
     @click.option('--agent-error-key-by-time', default=False, is_flag=True,
-                  help=('DEPRECATED: use --event-tally-granularity'))
+                  help='DEPRECATED: use --event-tally-granularity')
     @click.option('--event-tally-granularity', default='date',
                   help=('By default event tallies will be grouped by date, '
                         'for example when tallying occurrences of an event '
                         'in a file and displaying them in the summary. If '
                         'finer granularity is required this can be set to '
                         '"time".'))
     @click.option('--force', default=False, is_flag=True,
@@ -226,44 +226,44 @@
     @click.option('--user-summary', default=None,
                   help=('[DEPRECATED] Provide an existing summary so that it '
                         'can be post-processed e.g. --format json. This '
                         'option is deprecated and no longer does anything'))
     @click.option('--html-escape', default=False, is_flag=True,
                   help=('Apply html escaping to the output so that it is safe '
                         'to display in html.'))
-    @click.option('--format',
+    @click.option('--format', '--output-format', 'output_format',
                   type=click.Choice(OutputManager.SUMMARY_FORMATS),
                   default='yaml',
                   show_default=True,
-                  help=('Summary output format.'))
+                  help='Summary output format.')
     @click.option('--save', '-s', default=False, is_flag=True,
-                  help=('Save output to a file.'))
+                  help='Save output to a file.')
     @click.option('--quiet', default=False, is_flag=True,
                   help=('Suppress normal stderr output, only errors will be '
                         'printed.'))
     @click.option('--debug', default=False, is_flag=True,
                   help=('Provide some debug output. Logs will be printed to '
                         'stderr.'))
     @click.option('--all-logs', default=False, is_flag=True,
                   help=('Some plugins may choose to only analyse the most '
                         'recent version of a log file by default since '
                         'parsing the full history could take a lot '
                         'longer. This tells plugins that we wish to analyse '
                         'all available log history (see --max-logrotate-depth '
                         'for limits).'))
     @click.option('--defs-path', default=get_defs_path(),
-                  help=('Path to yaml definitions (ydefs).'))
+                  help='Path to yaml definitions (ydefs).')
     @click.option('--templates-path', default=get_templates_path(),
-                  help=('Path to Jinja templates.'))
+                  help='Path to Jinja templates.')
     @click.option('--version', '-v', default=False, is_flag=True,
-                  help=('Show the version.'))
+                  help='Show the version.')
     @set_plugin_options
     @click.argument('data_root', required=False, type=click.Path(exists=True))
     def cli(data_root, version, defs_path, templates_path, all_logs, quiet,
-            debug, save, format, html_escape, short, very_short,
+            debug, save, output_format, html_escape, short, very_short,
             force, full, agent_error_key_by_time, event_tally_granularity,
             max_logrotate_depth, max_parallel_tasks, list_plugins,
             machine_readable, output_path,
             allow_constraints_for_unverifiable_logs, command_timeout,
             **kwargs):
         """
         Run this tool on a host or against an unpacked sosreport to perform
@@ -380,15 +380,15 @@
 
         if save:
             prefix = get_prefix(data_root)
             path = summary.save(prefix, html_escape=html_escape,
                                 output_path=output_path)
             sys.stdout.write("INFO: output saved to {}\n".format(path))
         else:
-            out = summary.get(format=format, html_escape=html_escape,
+            out = summary.get(fmt=output_format, html_escape=html_escape,
                               minimal_mode=minimal_mode)
             if out:
                 sys.stdout.write("{}\n".format(out))
 
     cli(prog_name='hotsos')
```

### Comparing `hotsos-1.15.post8/hotsos/client.py` & `hotsos-1.15.post9/hotsos/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -242,55 +242,55 @@
 
         log.debug("Minimising output (mode=%s).", mode)
         if not summary:
             return summary
 
         if mode == 'short':
             return self._get_short_format(summary)
-        elif mode == 'very-short':
+        if mode == 'very-short':
             return self._get_very_short_format(summary)
 
         log.warning("Unknown minimalmode '%s'", mode)
         return summary
 
-    def get(self, format='yaml', html_escape=False, minimal_mode=None,
+    def get(self, fmt='yaml', html_escape=False, minimal_mode=None,
             plugin=None, max_level=2):
         if plugin:
             filtered = {plugin: self._summary[plugin]}
         else:
             filtered = self._summary
 
         if minimal_mode:
             filtered = self.minimise(filtered, minimal_mode)
 
-        if format not in self.SUMMARY_FORMATS:
-            raise Exception("unsupported summary format '{}'".format(format))
+        if fmt not in self.SUMMARY_FORMATS:
+            raise Exception("unsupported summary format '{}'".format(fmt))
 
         hostname = CLIHelper().hostname() or ""
-        log.debug('Saving summary as %s', format)
-        if format == 'yaml':
+        log.debug('Saving summary as %s', fmt)
+        if fmt == 'yaml':
             filtered = plugintools.yaml_dump(filtered)
-        elif format == 'json':
+        elif fmt == 'json':
             filtered = json.dumps(filtered, indent=2, sort_keys=True)
-        elif format == 'markdown':
+        elif fmt == 'markdown':
             filtered = plugintools.MarkdownFormatter().dump(filtered)
-        elif format == 'html':
+        elif fmt == 'html':
             filtered = plugintools.HTMLFormatter(
                                             hostname=hostname,
                                             max_level=max_level).dump(filtered)
 
         if html_escape:
             log.debug('Applying html escaping to summary')
             filtered = html.escape(filtered)
 
         return filtered
 
-    def _save(self, path, format, html_escape=None, minimal_mode=None,
+    def _save(self, path, fmt, html_escape=None, minimal_mode=None,
               plugin=None):
-        content = self.get(format=format, html_escape=html_escape,
+        content = self.get(fmt=fmt, html_escape=html_escape,
                            minimal_mode=minimal_mode, plugin=plugin)
         with open(path, 'w', encoding='utf-8') as fd:
             fd.write(content)
             fd.write('\n')
 
     def save(self, name, html_escape=False, output_path=None):
         """
@@ -303,38 +303,38 @@
             output_root = output_path
         else:
             output_root = ('hotsos-output-{}'.
                            format(CLIHelper().date(format='+%s')))
 
         for minimal_mode in ['full', 'short', 'very-short']:
             _minimal_mode = minimal_mode.replace('-', '_')
-            for format in self.SUMMARY_FORMATS:
+            for fmt in self.SUMMARY_FORMATS:
                 output_path = os.path.join(output_root, name, 'summary',
-                                           _minimal_mode, format)
+                                           _minimal_mode, fmt)
                 if minimal_mode == 'full':
                     minimal_mode = None
 
                 if not os.path.exists(output_path):
                     os.makedirs(output_path)
 
                 for plugin in self._summary:
                     path = os.path.join(output_path,
                                         "hotsos-summary.{}.{}".format(plugin,
-                                                                      format))
-                    self._save(path, format, html_escape=html_escape,
+                                                                      fmt))
+                    self._save(path, fmt, html_escape=html_escape,
                                minimal_mode=minimal_mode, plugin=plugin)
 
                 path = os.path.join(output_path,
-                                    "hotsos-summary.all.{}".format(format))
-                self._save(path, format, html_escape=html_escape,
+                                    "hotsos-summary.all.{}".format(fmt))
+                self._save(path, fmt, html_escape=html_escape,
                            minimal_mode=minimal_mode)
 
                 if not minimal_mode:
                     dst = os.path.join(output_root, '{}.summary.{}'.
-                                       format(name, format))
+                                       format(name, fmt))
                     if os.path.exists(dst):
                         os.remove(dst)
 
                     os.symlink(path.partition(output_root)[2].lstrip('/'), dst)
 
         if log.handlers and isinstance(log.handlers[0], logging.FileHandler):
             log.handlers[0].close()
```

### Comparing `hotsos-1.15.post8/hotsos/core/analytics.py` & `hotsos-1.15.post9/hotsos/core/analytics.py`

 * *Files 0% similar despite different names*

```diff
@@ -220,15 +220,15 @@
             meta_key = seq_idxs.metadata_key
             event_id = result.get(seq_idxs.event_id)
             self.data.add_event_start(event_id, start, metadata=metadata,
                                       metadata_key=meta_key)
 
         self.data.calculate_event_deltas()
 
-    def get_top_n_events_sorted(self, max, reverse=True):
+    def get_top_n_events_sorted(self, maximum, reverse=True):
         """
         Find events with the longest duration limited to max results.
 
         @param max: integer number of events to include.
         @param reverse: defaults to True for longest durations. Set to False to
         fetch events with shortest duration.
         @return: dictionary of results.
@@ -236,15 +236,15 @@
         count = 0
         top_n = {}
         top_n_sorted = {}
 
         for event_id, item in sorted(self.data.complete_events.items(),
                                      key=lambda e: e[1]["duration"],
                                      reverse=reverse):
-            if count >= max:
+            if count >= maximum:
                 break
 
             count += 1
             top_n[event_id] = item
 
         for event_id, item in sorted(top_n.items(),
                                      key=lambda x: x[1]["start"],
```

### Comparing `hotsos-1.15.post8/hotsos/core/config.py` & `hotsos-1.15.post9/hotsos/core/config.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,19 +5,19 @@
 
 class ConfigException(Exception):
     pass
 
 
 class ConfigOpt(object):
 
-    def __init__(self, name, description, default_value, type):
+    def __init__(self, name, description, default_value, value_type):
         self.name = name
         self.description = description
         self.default_value = default_value
-        self.type = type
+        self.value_type = value_type
 
 
 class ConfigOptGroupBase(UserDict):
 
     def __init__(self):
         self.opts = {}
 
@@ -42,97 +42,97 @@
 
     def __init__(self):
         super().__init__()
         self.add(ConfigOpt(name='data_root',
                            description=('This is the filesystem root used for '
                                         'all files and is typically / or a '
                                         'path to a sosreport'),
-                           default_value=None, type=str))
+                           default_value=None, value_type=str))
         self.add(ConfigOpt(name='force_mode',
                            description=('Plugin execution is usually gated '
                                         'on a set of conditions. Setting this '
                                         'to True bypasses these conditions '
                                         'and forces all plugins to run'),
-                           default_value=False, type=bool))
+                           default_value=False, value_type=bool))
         self.add(ConfigOpt(name='global_tmp_dir',
                            description=('A temporary directory created at the '
                                         'start of execution and visible to '
                                         'all plugins.'),
-                           default_value=None, type=str))
+                           default_value=None, value_type=str))
         self.add(ConfigOpt(name='plugin_tmp_dir',
                            description=('A temporary directory created for '
                                         'each plugin.'),
-                           default_value=None, type=str))
+                           default_value=None, value_type=str))
         self.add(ConfigOpt(name='use_all_logs',
                            description=('Automatically convert log paths to '
                                         'glob e.g. <path> becomes <path>*'),
-                           default_value=False, type=bool))
+                           default_value=False, value_type=bool))
         self.add(ConfigOpt(name='machine_readable',
                            description=('If set to True, the summary output'
                                         'will contain extra information '
                                         'that might be useful if the output '
                                         'is being read by an application.'),
-                           default_value=False, type=bool))
+                           default_value=False, value_type=bool))
         self.add(ConfigOpt(name='part_name',
                            description=('Plugins have many parts each with '
                                         'its own name and this will be set to '
                                         'the current part being executed.'),
-                           default_value=None, type=str))
+                           default_value=None, value_type=str))
         self.add(ConfigOpt(name='repo_info',
                            description=('Source repository sha1 from which '
                                         'the current build was created'),
-                           default_value=None, type=str))
+                           default_value=None, value_type=str))
         self.add(ConfigOpt(name='hotsos_version',
                            description='Version of hotsos being run.',
-                           default_value=None, type=str))
+                           default_value=None, value_type=str))
         self.add(ConfigOpt(name='debug_mode',
                            description='Set to True to enable debug logging',
-                           default_value=False, type=bool))
+                           default_value=False, value_type=bool))
         self.add(ConfigOpt(name='plugin_yaml_defs',
                            description='Path to yaml-defined checks.',
-                           default_value=None, type=str))
+                           default_value=None, value_type=str))
         self.add(ConfigOpt(name='templates_path',
                            description='Path to jinja templates.',
-                           default_value='templates', type=str))
+                           default_value='templates', value_type=str))
         self.add(ConfigOpt(name='plugin_name',
                            description='Name of current plugin being executed',
-                           default_value=None, type=str))
+                           default_value=None, value_type=str))
         self.add(ConfigOpt(name='event_tally_granularity',
                            description=("By default event tallies are listed "
                                         "by date in the summary. This option "
                                         "can be set to one of 'date' or "
                                         "'time' to get the corresponding "
                                         "granularity of results."),
-                           default_value='date', type=str))
+                           default_value='date', value_type=str))
         self.add(ConfigOpt(name='command_timeout',
                            description=("Maximum time in seconds before "
                                         "command execution will timeout. Used "
                                         "by host_helpers.cli when executing "
                                         "binary commands"),
-                           default_value=300, type=int))
+                           default_value=300, value_type=int))
 
     @property
     def name(self):
         return 'hotsos'
 
 
 class SearchtoolsConfigOpts(ConfigOptGroupBase):
 
     def __init__(self):
         super().__init__()
         self.add(ConfigOpt(name='max_parallel_tasks',
                            description=('Maximum parallelism for searching '
                                         'files concurrently'),
-                           default_value=8, type=int))
+                           default_value=8, value_type=int))
         self.add(ConfigOpt(name='max_logrotate_depth',
                            description=('When log paths are expanded using '
                                         'use_all_logs and they are logrotated '
                                         'log files, this is used to limit the '
                                         'logrotate history in days.'),
-                           default_value=7, type=int))
+                           default_value=7, value_type=int))
         self.add(ConfigOpt(name='allow_constraints_for_unverifiable_logs',
                            description=('Search constraints use a binary '
                                         'search that sometimes needs to '
                                         'seek backwards to find a last '
                                         'known good line i.e. in log files '
                                         "that contain lines that don't start "
                                         'with a timestamp we treat those as '
@@ -146,15 +146,15 @@
                                         'slow as it will start from 0 each '
                                         'time. Backwards seeking is now not '
                                         'supported by default and requires '
                                         'setting this option to True '
                                         'to enable search constraints for '
                                         'files that contain unverifiable '
                                         'lines.'),
-                           default_value=False, type=bool))
+                           default_value=False, value_type=bool))
 
     @property
     def name(self):
         return 'search'
 
 
 class RegisteredOpts(UserDict):
@@ -173,15 +173,15 @@
                                 format(optgroup.name))
 
             self.data.update(optgroup)
 
     def __setitem__(self, key, item):
         for group in self.optsgroups:
             if key in group.opts:
-                item = group.opts[key].type(item)
+                item = group.opts[key].value_type(item)
                 break
         else:
             raise Exception("config option '{}' not found in any optgrpup".
                             format(key))
 
         self.data[key] = item
 
@@ -198,16 +198,16 @@
         raise ConfigException("fetching unknown config '{}'.".
                               format(key))
 
     def __setattr__(cls, key, val):
         if key in cls.CONFIG:
             cls.CONFIG[key] = val
             return
-        elif key not in ['__abstractmethods__', '_abc_impl', 'CONFIG',
-                         'REGISTERED']:
+        if key not in ['__abstractmethods__', '_abc_impl', 'CONFIG',
+                       'REGISTERED']:
             raise ConfigException("setting unknown config '{}'.".
                                   format(key))
 
         super().__setattr__(key, val)
 
 
 class HotSOSConfig(object, metaclass=ConfigMeta):
```

### Comparing `hotsos-1.15.post8/hotsos/core/factory.py` & `hotsos-1.15.post9/hotsos/core/factory.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post8/hotsos/core/host_helpers/__init__.py` & `hotsos-1.15.post9/hotsos/core/host_helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post8/hotsos/core/host_helpers/cli.py` & `hotsos-1.15.post9/hotsos/core/host_helpers/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -376,36 +376,36 @@
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.register_hook("pre-exec", self.format_date_cmd)
 
     def format_date_cmd(self, **kwargs):
         """ Add formatting to date command. """
         no_format = kwargs.get('no_format', False)
-        format = kwargs.get('format')
-        if not no_format and format is None:
-            format = '+%s'
+        fmt = kwargs.get('format')
+        if not no_format and fmt is None:
+            fmt = '+%s'
 
         self.cmd = '{} --utc'.format(self.cmd)
-        if format:
+        if fmt:
             # this can't get split() so add to the end of the command list
-            self.original_cmd_extras = [format]
+            self.original_cmd_extras = [fmt]
 
 
 class DateFileCmd(FileCmd):
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.register_hook("post-exec", self.format_date)
 
     def format_date(self, output, **kwargs):
         """ Apply some post-processing to the date output. """
         no_format = kwargs.get('no_format', False)
-        format = kwargs.get('format')
-        if not no_format and format is None:
-            format = '+%s'
+        fmt = kwargs.get('format')
+        if not no_format and fmt is None:
+            fmt = '+%s'
 
         ret = re.match(r"^(\S+ \S*\s*[0-9]+ [0-9:]+)\s*"
                        r"([A-Z]*|[+-]?[0-9]*)?"
                        r"\s*([0-9]+)$",
                        output)
 
         if ret is None:
@@ -417,16 +417,16 @@
         # convert to a format that is recognised.
         if tz == 'HKT':
             tz = 'UTC+8'
 
         # Include tz if available and then convert to utc
         date = "{} {} {}".format(ret[1], tz, ret[3])
         cmd = ["date", "--utc", "--date={}".format(date)]
-        if format:
-            cmd.append(format)
+        if fmt:
+            cmd.append(fmt)
 
         output = subprocess.check_output(cmd,
                                          timeout=HotSOSConfig.command_timeout)
         # date sometimes adds multiple whitespaces between fields so collapse
         # them.
         output = re.compile(r"\s+").sub(' ', output.decode('UTF-8'))
         ret = output.splitlines(keepends=True)[0]
```

### Comparing `hotsos-1.15.post8/hotsos/core/host_helpers/common.py` & `hotsos-1.15.post9/hotsos/core/host_helpers/common.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post8/hotsos/core/host_helpers/config.py` & `hotsos-1.15.post9/hotsos/core/host_helpers/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -90,15 +90,15 @@
         self._flattened_config = {}
         self._load()
 
     @staticmethod
     def bool_str(val):
         if val.lower() == "true":
             return True
-        elif val.lower() == "false":
+        if val.lower() == "false":
             return False
 
         return val
 
     @property
     def all(self):
         return self._sections
```

### Comparing `hotsos-1.15.post8/hotsos/core/host_helpers/filestat.py` & `hotsos-1.15.post9/hotsos/core/host_helpers/filestat.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post8/hotsos/core/host_helpers/network.py` & `hotsos-1.15.post9/hotsos/core/host_helpers/network.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post8/hotsos/core/host_helpers/packaging.py` & `hotsos-1.15.post9/hotsos/core/host_helpers/packaging.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post8/hotsos/core/host_helpers/pebble.py` & `hotsos-1.15.post9/hotsos/core/host_helpers/pebble.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post8/hotsos/core/host_helpers/ssl.py` & `hotsos-1.15.post9/hotsos/core/host_helpers/ssl.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,17 +32,17 @@
         return cert.not_valid_after
 
     @property
     def days_to_expire(self):
         """
         Return int(days) remaining until the certificate expires
         """
-        format = '%Y-%m-%d %H:%M:%S'
-        today = datetime.strptime(CLIHelper().date(format='+' + format),
-                                  format)
+        fmt = '%Y-%m-%d %H:%M:%S'
+        today = datetime.strptime(CLIHelper().date(format='+' + fmt),
+                                  fmt)
         days = self.expiry_date - today
         return int(days.days)
 
 
 class SSLCertificatesHelper(object):
 
     def __init__(self, certificate, expire_days):
```

### Comparing `hotsos-1.15.post8/hotsos/core/host_helpers/sysctl.py` & `hotsos-1.15.post9/hotsos/core/host_helpers/sysctl.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post8/hotsos/core/host_helpers/systemd.py` & `hotsos-1.15.post9/hotsos/core/host_helpers/systemd.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,16 +33,16 @@
         for line in journal:
             ret = cexpr.search(line)
             if ret:
                 last = ret.group(1)
 
         if last:
             return datetime.strptime(last, "%Y-%m-%dT%H:%M:%S%z")
-        else:
-            log.debug("no start time identified for svc %s", self.name)
+
+        log.debug("no start time identified for svc %s", self.name)
 
     @cached_property
     def start_time_secs(self):
         """ Get most recent start time of this service unit in seconds.
 
         @returns: posix timestamp
         """
```

### Comparing `hotsos-1.15.post8/hotsos/core/host_helpers/uptime.py` & `hotsos-1.15.post9/hotsos/core/host_helpers/uptime.py`

 * *Files 6% similar despite different names*

```diff
@@ -41,18 +41,18 @@
             expr = self.subgroups['day']['expr']
             ret = re.match(expr, self.subgroups['day']['value'])
             if ret:
                 count = int(ret.group(1))
                 hours = int(ret.group(2))
                 mins = int(ret.group(3))
                 day_mins = 24 * 60
-                sum = count * day_mins
-                sum += hours * 60
-                sum += mins
-                return sum
+                total = count * day_mins
+                total += hours * 60
+                total += mins
+                return total
         elif self.subgroups['min']['value']:
             expr = self.subgroups['min']['expr']
             ret = re.match(expr, self.subgroups['min']['value'])
             if ret:
                 return int(ret.group(1))
 
         log.warning("unknown uptime format in %s", self.uptime)
```

### Comparing `hotsos-1.15.post8/hotsos/core/issues/issue_types.py` & `hotsos-1.15.post9/hotsos/core/issues/issue_types.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,17 +11,17 @@
     def name(self):
         return self.__class__.__name__
 
 
 class BugTypeBase(abc.ABC, IssueTypeBase):
     ISSUE_TYPE = 'bug'
 
-    def __init__(self, id, msg):
-        self.id = id
-        self.msg = msg
+    def __init__(self, bug_id, msg):
+        super().__init__(msg)
+        self.id = bug_id
 
     @property
     @abc.abstractmethod
     def base_url(self):
         pass
 
     @property
```

### Comparing `hotsos-1.15.post8/hotsos/core/issues/utils.py` & `hotsos-1.15.post9/hotsos/core/issues/utils.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post8/hotsos/core/log.py` & `hotsos-1.15.post9/hotsos/core/log.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from hotsos.core.config import HotSOSConfig
 
 log = logging.getLogger()
 
 
 def setup_logging():
-    format = ("%(asctime)s.%(msecs)03d %(process)d %(levelname)s %(name)s [-] "
-              "%(message)s")
+    fmt = ("%(asctime)s.%(msecs)03d %(process)d %(levelname)s %(name)s [-] "
+           "%(message)s")
     log.name = 'plugin.{}'.format(HotSOSConfig.plugin_name)
     if not HotSOSConfig.debug_mode:
-        logging.basicConfig(format=format, level=logging.DEBUG,
+        logging.basicConfig(format=fmt, level=logging.DEBUG,
                             filename=tempfile.mktemp(suffix='hotsos.log'))
     else:
-        logging.basicConfig(format=format, level=logging.DEBUG)
+        logging.basicConfig(format=fmt, level=logging.DEBUG)
```

### Comparing `hotsos-1.15.post8/hotsos/core/plugins/juju/common.py` & `hotsos-1.15.post9/hotsos/core/plugins/juju/common.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post8/hotsos/core/plugins/juju/resources.py` & `hotsos-1.15.post9/hotsos/core/plugins/juju/resources.py`

 * *Files 3% similar despite different names*

```diff
@@ -59,28 +59,28 @@
         # requires >= 2.9.x
         _units = self.config.get("values", {}).get("deployed-units", "")
         if not _units:
             return units
 
         for unit in _units.split(','):
             app = unit.partition('/')[0]
-            id = unit.partition('/')[2]
+            unit_id = unit.partition('/')[2]
             path = os.path.join(self.juju_lib_path,
-                                "agents/unit-{}-{}".format(app, id))
-            units.append(JujuUnit(id, app, self.juju_lib_path, path=path))
+                                "agents/unit-{}-{}".format(app, unit_id))
+            units.append(JujuUnit(unit_id, app, self.juju_lib_path, path=path))
 
         return units
 
 
 class JujuUnit(object):
 
-    def __init__(self, id, application, juju_lib_path, path=None):
-        self.id = id
+    def __init__(self, unit_id, application, juju_lib_path, path=None):
+        self.id = unit_id
         self.application = application
-        self.name = '{}-{}'.format(application, id)
+        self.name = '{}-{}'.format(application, unit_id)
         self.juju_lib_path = juju_lib_path
         self.path = path
 
     @utils.cached_property
     def charm_name(self):
         """
         The deployer manifest file will give us the name of the charm used to
@@ -157,16 +157,16 @@
             paths = glob.glob(os.path.join(self.juju_lib_path,
                                            "agents/unit-*"))
             for unit in paths:
                 base = os.path.basename(unit)
                 ret = re.compile(r"unit-(\S+)-(\d+)").match(base)
                 if ret:
                     app = ret.group(1)
-                    id = ret.group(2)
-                    u = JujuUnit(id, app, self.juju_lib_path, path=unit)
+                    unit_id = ret.group(2)
+                    u = JujuUnit(unit_id, app, self.juju_lib_path, path=unit)
                     _units[u.name] = u
 
         return _units
 
     @utils.cached_property
     def charms(self):
         """
```

### Comparing `hotsos-1.15.post8/hotsos/core/plugins/kernel/common.py` & `hotsos-1.15.post9/hotsos/core/plugins/kernel/common.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post8/hotsos/core/plugins/kernel/config.py` & `hotsos-1.15.post9/hotsos/core/plugins/kernel/config.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post8/hotsos/core/plugins/kernel/kernlog/calltrace.py` & `hotsos-1.15.post9/hotsos/core/plugins/kernel/kernlog/calltrace.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post8/hotsos/core/plugins/kernel/kernlog/common.py` & `hotsos-1.15.post9/hotsos/core/plugins/kernel/kernlog/common.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post8/hotsos/core/plugins/kernel/kernlog/events.py` & `hotsos-1.15.post9/hotsos/core/plugins/kernel/kernlog/events.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post8/hotsos/core/plugins/kernel/memory.py` & `hotsos-1.15.post9/hotsos/core/plugins/kernel/memory.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post8/hotsos/core/plugins/kernel/net.py` & `hotsos-1.15.post9/hotsos/core/plugins/kernel/net.py`

 * *Files 2% similar despite different names*

```diff
@@ -144,15 +144,15 @@
         """
         Fields can be appended with PcentInSegs/PcentOutSegs to get a
         percentage of total rx/tx segments.
         """
         if fld.endswith('PcentInSegs'):
             fld = fld.partition('PcentInSegs')[0]
             return self.PcentInSegs(fld)
-        elif fld.endswith('PcentOutSegs'):
+        if fld.endswith('PcentOutSegs'):
             fld = fld.partition('PcentOutSegs')[0]
             return self.PcentOutSegs(fld)
 
         return super().__getattr__(fld)
 
 
 class SNMPUdp(SNMPBase):
@@ -189,15 +189,15 @@
         """
         Fields can be appended with PcentInDatagrams/PcentOutDatagrams to get a
         percentage of total rx/tx datagrams.
         """
         if fld.endswith('PcentInDatagrams'):
             fld = fld.partition('PcentInDatagrams')[0]
             return self.PcentInDatagrams(fld)
-        elif fld.endswith('PcentOutDatagrams'):
+        if fld.endswith('PcentOutDatagrams'):
             fld = fld.partition('PcentOutDatagrams')[0]
             return self.PcentOutDatagrams(fld)
 
         return super().__getattr__(fld)
 
 
 class NetStatBase(ProcNetBase):
@@ -276,15 +276,15 @@
         """
         Fields can be appended with PcentInSegs/PcentOutSegs to get a
         percentage of total rx/tx segments.
         """
         if fld.endswith('PcentInSegs'):
             fld = fld.partition('PcentInSegs')[0]
             return self.PcentInSegs(fld)
-        elif fld.endswith('PcentOutSegs'):
+        if fld.endswith('PcentOutSegs'):
             fld = fld.partition('PcentOutSegs')[0]
             return self.PcentOutSegs(fld)
 
         return super().__getattr__(fld)
 
 
 class SockStat(ProcNetBase):
@@ -608,9 +608,9 @@
         if v:
             # Correlate netlink sockets with process id's by inode
             # only if there's matching data.
             lsof = Lsof()
             for nlsock in v:
                 correlate_result = lsof.all_with_inode(nlsock.sk_inode_num)
                 nlsock.procs = set(
-                    [f"{v.COMMAND}/{v.PID}" for v in correlate_result])
+                    f"{v.COMMAND}/{v.PID}" for v in correlate_result)
         return v
```

### Comparing `hotsos-1.15.post8/hotsos/core/plugins/kernel/sysfs.py` & `hotsos-1.15.post9/hotsos/core/plugins/kernel/sysfs.py`

 * *Files 5% similar despite different names*

```diff
@@ -65,15 +65,15 @@
     def cpufreq_scaling_governor(self, cpu_id):
         return self.get('devices/system/cpu/cpu{}/cpufreq/scaling_governor'.
                         format(cpu_id))
 
     @property
     def cpufreq_scaling_governor_all(self):
         governors = set()
-        for id in range(SystemBase().num_cpus):
-            cpu_governor = self.cpufreq_scaling_governor(id)
+        for cpu_id in range(SystemBase().num_cpus):
+            cpu_governor = self.cpufreq_scaling_governor(cpu_id)
             if cpu_governor:
                 governors.add(cpu_governor)
             else:
                 governors.add('unknown')
 
         return ','.join(list(governors))
```

### Comparing `hotsos-1.15.post8/hotsos/core/plugins/kubernetes.py` & `hotsos-1.15.post9/hotsos/core/plugins/kubernetes.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post8/hotsos/core/plugins/lxd/common.py` & `hotsos-1.15.post9/hotsos/core/plugins/lxd/common.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post8/hotsos/core/plugins/maas.py` & `hotsos-1.15.post9/hotsos/core/plugins/maas.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post8/hotsos/core/plugins/mysql.py` & `hotsos-1.15.post9/hotsos/core/plugins/mysql.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post8/hotsos/core/plugins/openstack/common.py` & `hotsos-1.15.post9/hotsos/core/plugins/openstack/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -175,17 +175,17 @@
     def days_to_eol(self):
         if self.release_name != 'unknown':
             eol = OST_EOL_INFO.get(self.release_name)
             if eol is not None:
                 today = datetime.utcfromtimestamp(int(CLIHelper().date()))
                 delta = (eol - today).days
                 return delta
-            else:
-                log.warning("unable to determine eol info for unknown release "
-                            "name '%s'", self.release_name)
+
+            log.warning("unable to determine eol info for unknown release "
+                        "name '%s'", self.release_name)
 
     @property
     def bind_interfaces(self):
         """
         Fetch interfaces used by Openstack services and return dict.
         """
         interfaces = {}
```

### Comparing `hotsos-1.15.post8/hotsos/core/plugins/openstack/exceptions.py` & `hotsos-1.15.post9/hotsos/core/plugins/openstack/exceptions.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post8/hotsos/core/plugins/openstack/neutron.py` & `hotsos-1.15.post9/hotsos/core/plugins/openstack/neutron.py`

 * *Files 5% similar despite different names*

```diff
@@ -111,17 +111,17 @@
                         if ret:
                             router.vr_id = ret.group(1)
 
             _routers.append(router)
 
         return _routers
 
-    def find_router_with_vr_id(self, id):
+    def find_router_with_vr_id(self, vr_id):
         for r in self.ha_routers:
-            if r.vr_id == id:
+            if r.vr_id == vr_id:
                 return r
 
 
 class Config(FactoryBase):
 
     def __getattr__(self, path):
         path = os.path.join(HotSOSConfig.data_root, 'etc/neutron', path)
```

### Comparing `hotsos-1.15.post8/hotsos/core/plugins/openstack/nova.py` & `hotsos-1.15.post9/hotsos/core/plugins/openstack/nova.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post8/hotsos/core/plugins/openstack/octavia.py` & `hotsos-1.15.post9/hotsos/core/plugins/openstack/octavia.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post8/hotsos/core/plugins/openstack/openstack.py` & `hotsos-1.15.post9/hotsos/core/plugins/openstack/openstack.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post8/hotsos/core/plugins/openvswitch/common.py` & `hotsos-1.15.post9/hotsos/core/plugins/openvswitch/common.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post8/hotsos/core/plugins/openvswitch/ovn.py` & `hotsos-1.15.post9/hotsos/core/plugins/openvswitch/ovn.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 from hotsos.core.utils import cached_property, mktemp_dump
 from hotsos.core.host_helpers import SystemdHelper
 from hotsos.core.plugins.openvswitch.common import OVS_SERVICES_EXPRS
 
 
 class OVNSBDBPort(object):
 
-    def __init__(self, name, type):
+    def __init__(self, name, port_type):
         self.name = name
-        self.type = type
+        self.type = port_type
 
 
 class OVNSBDBChassis(object):
 
     def __init__(self, name, content):
         self.name = name
         self.content = content or {}
@@ -68,31 +68,31 @@
         body = SearchDef(r"^\s+(\S+)\s+(.+)")
         return SequenceSearchDef(start=start, body=body, tag='resources')
 
     @cached_property
     def resources(self):
         _resources = {}
         resource = None
-        id = None
+        rid = None
         sections = self.results.find_sequence_sections(self.resources_sd)
         for section in sections.values():
             for result in section:
                 if result.tag == self.resources_sd.start_tag:
                     resource = result.get(1)
-                    id = result.get(2)
+                    rid = result.get(2)
                     if resource in _resources:
-                        _resources[resource][id] = {}
+                        _resources[resource][rid] = {}
                     else:
-                        _resources[resource] = {id: {}}
+                        _resources[resource] = {rid: {}}
                 elif result.tag == self.resources_sd.body_tag:
                     rtype = result.get(1)
-                    if rtype in _resources[resource][id]:
-                        _resources[resource][id][rtype].append(result.get(2))
+                    if rtype in _resources[resource][rid]:
+                        _resources[resource][rid][rtype].append(result.get(2))
                     else:
-                        _resources[resource][id][rtype] = [result.get(2)]
+                        _resources[resource][rid][rtype] = [result.get(2)]
 
         return _resources
 
 
 class OVNNBDB(OVNDBBase):
     """ Represents OVN Northbound DB. """
 
@@ -101,26 +101,26 @@
         return CLIHelper().ovn_nbctl_show()
 
     @cached_property
     def routers(self):
         _routers = []
         for r, v in self.resources.items():
             if r == 'router':
-                for id in v:
-                    _routers.append(id)
+                for rid in v:
+                    _routers.append(rid)
 
         return _routers
 
     @cached_property
     def switches(self):
         _switches = []
         for r, v in self.resources.items():
             if r == 'switch':
-                for id in v:
-                    _switches.append(id)
+                for sid in v:
+                    _switches.append(sid)
 
         return _switches
 
 
 class OVNSBDB(OVNDBBase):
     """ Represents OVN Southbound DB. """
 
@@ -129,16 +129,16 @@
         return CLIHelper().ovn_sbctl_show()
 
     @cached_property
     def chassis(self):
         _chassis = []
         for r, v in self.resources.items():
             if r == 'Chassis':
-                for id, contents in v.items():
-                    _chassis.append(OVNSBDBChassis(id, contents))
+                for cid, contents in v.items():
+                    _chassis.append(OVNSBDBChassis(cid, contents))
 
         return _chassis
 
 
 class OVNBase(object):
     """
     Base class for all OVN components.
```

### Comparing `hotsos-1.15.post8/hotsos/core/plugins/openvswitch/ovs.py` & `hotsos-1.15.post9/hotsos/core/plugins/openvswitch/ovs.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post8/hotsos/core/plugins/pacemaker.py` & `hotsos-1.15.post9/hotsos/core/plugins/pacemaker.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post8/hotsos/core/plugins/rabbitmq/common.py` & `hotsos-1.15.post9/hotsos/core/plugins/rabbitmq/common.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post8/hotsos/core/plugins/rabbitmq/report.py` & `hotsos-1.15.post9/hotsos/core/plugins/rabbitmq/report.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,15 +55,15 @@
                                  tag='queues')
 
     @cached_property
     def skewed_nodes(self):
         vhosts = self.vhosts
         _skewed_nodes = {}
         skewed_queue_nodes = {}
-        global_total_queues = sum([vhost.total_queues for vhost in vhosts])
+        global_total_queues = sum(vhost.total_queues for vhost in vhosts)
         for vhost in self.vhosts:
             if not vhost.total_queues:
                 continue
 
             total_pcent = (float(100) / global_total_queues *
                            vhost.total_queues)
```

### Comparing `hotsos-1.15.post8/hotsos/core/plugins/sosreport.py` & `hotsos-1.15.post9/hotsos/core/plugins/sosreport.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post8/hotsos/core/plugins/storage/bcache.py` & `hotsos-1.15.post9/hotsos/core/plugins/storage/bcache.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post8/hotsos/core/plugins/storage/ceph.py` & `hotsos-1.15.post9/hotsos/core/plugins/storage/ceph.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,16 +38,16 @@
                        r"rados[a-z0-9-:]+"]
 CEPH_PKGS_CORE = [r"ceph",
                   r"rados",
                   r"rbd",
                   ]
 CEPH_PKGS_OTHER = []
 # Add in clients/deps
-for pkg in CEPH_PKGS_CORE:
-    CEPH_PKGS_OTHER.append(r"python3?-{}\S*".format(pkg))
+for ceph_pkg in CEPH_PKGS_CORE:
+    CEPH_PKGS_OTHER.append(r"python3?-{}\S*".format(ceph_pkg))
 
 CEPH_LOGS = "var/log/ceph/"
 
 # NOTE(tpsilva): when updating this list, refer to the supported Ceph
 # versions for Ubuntu page:
 # https://ubuntu.com/ceph/docs/supported-ceph-versions
 CEPH_EOL_INFO = {
@@ -78,15 +78,15 @@
 def csv_to_set(f):
     """
     Decorator used to convert a csv string to a set().
     """
     def csv_to_set_inner(*args, **kwargs):
         val = f(*args, **kwargs)
         if val is not None:
-            return set([v.strip(',') for v in val.split()])
+            return set(v.strip(',') for v in val.split())
 
         return set([])
 
     return csv_to_set_inner
 
 
 class CephTimestampMatcher(TimestampMatcherBase):
@@ -564,21 +564,21 @@
         laggy_like_states = ['laggy', 'wait']
         for pg in self.pg_dump['pg_map']['pg_stats']:
             if any(x in pg['state'].split('+') for x in laggy_like_states):
                 laggy_pgs.append(pg)
 
         return laggy_pgs
 
-    def pool_id_to_name(self, id):
+    def pool_id_to_name(self, pool_id):
         if not self.osd_dump:
             return
 
         pools = self.osd_dump.get('pools', [])
         for pool in pools:
-            if pool['pool'] == int(id):
+            if pool['pool'] == int(pool_id):
                 return pool['pool_name']
 
     @cached_property
     def large_omap_pgs(self):
         _large_omap_pgs = {}
         if not self.pg_dump:
             return _large_omap_pgs
@@ -796,20 +796,20 @@
         """Return memory RSS for a given daemon.
 
         NOTE: this assumes we have ps auxwwwm format.
         """
         s = FileSearcher()
         # columns: USER PID %CPU %MEM VSZ RSS TTY STAT START TIME COMMAND
         if self.id is not None:
-            id = r"--id\s+{}".format(self.id)
+            ceph_id = r"--id\s+{}".format(self.id)
         else:
-            id = ''
+            ceph_id = ''
 
         expr = (r"\S+\s+\d+\s+\S+\s+\S+\s+\d+\s+(\d+)\s+.+/ceph-{}\s+.+{}\s+.+"
-                r".+".format(self.daemon_type, id))
+                r".+".format(self.daemon_type, ceph_id))
         sd = SearchDef(expr)
         ps_out = mktemp_dump('\n'.join(self.cli.ps()))
         s.add(sd, path=ps_out)
         rss = 0
         # we only expect one result
         for result in s.run().find_by_path(ps_out):
             rss = int(int(result.get(1)) / 1024)
@@ -848,15 +848,15 @@
         _etime = None
         for cmd in ps_info:
             ret = re.compile(r".+\s+.+--id {}\s+.+".format(self.id)).match(cmd)
             if ret:
                 osd_start = ' '.join(cmd.split()[13:17])
                 if self.date_in_secs and osd_start:
                     osd_start_secs = self.get_date_secs(datestring=osd_start)
-                    osd_uptime_secs = (self.date_in_secs - osd_start_secs)
+                    osd_uptime_secs = self.date_in_secs - osd_start_secs
                     osd_uptime_str = seconds_to_date(osd_uptime_secs)
                     _etime = osd_uptime_str
 
         return _etime
 
 
 class CephMon(CephDaemonBase):
@@ -876,17 +876,17 @@
 
     def __init__(self):
         super().__init__('radosgw')
 
 
 class CephOSD(CephDaemonBase):
 
-    def __init__(self, id, fsid=None, device=None, dump=None):
+    def __init__(self, ceph_id, fsid=None, device=None, dump=None):
         super().__init__('osd')
-        self.id = id
+        self.id = ceph_id
         self.fsid = fsid
         self.device = device
         self.dump = dump
 
     def to_dict(self):
         d = {self.id: {
              'fsid': self.fsid,
@@ -961,45 +961,45 @@
     def days_to_eol(self):
         if self.release_name != 'unknown':
             eol = CEPH_EOL_INFO[self.release_name]
             today = datetime.utcfromtimestamp(int(CLIHelper().date()))
             delta = (eol - today).days
             return delta
 
-    def _get_bind_interfaces(self, type):
+    def _get_bind_interfaces(self, iface_type):
         """
         For the given config network type determine what interface ceph is
         binding to.
 
-        @param type: cluster or public
+        @param iface_type: cluster or public
         """
-        net = self.ceph_config.get('{} network'.format(type))
-        addr = self.ceph_config.get('{} addr'.format(type))
+        net = self.ceph_config.get('{} network'.format(iface_type))
+        addr = self.ceph_config.get('{} addr'.format(iface_type))
         if not any([net, addr]):
             return {}
 
         nethelp = HostNetworkingHelper()
         port = None
         if net:
             port = nethelp.get_interface_with_addr(net)
         elif addr:
             port = nethelp.get_interface_with_addr(addr)
 
         if port:
-            return {type: port}
+            return {iface_type: port}
 
     @cached_property
     def _ceph_bind_interfaces(self):
         """
         Returns a dict of network interfaces used by Ceph daemons on this host.
         The dict has the form {<type>: [<port>, ...]}
         """
         interfaces = {}
-        for type in ['cluster', 'public']:
-            ret = self._get_bind_interfaces(type)
+        for iface_type in ['cluster', 'public']:
+            ret = self._get_bind_interfaces(iface_type)
             if ret:
                 interfaces.update(ret)
 
         return interfaces
 
     @property
     def bind_interfaces(self):
@@ -1028,27 +1028,27 @@
         s = FileSearcher()
         sd = SequenceSearchDef(start=SearchDef(r"^=+\s+osd\.(\d+)\s+=+.*"),
                                body=SearchDef([r"\s+osd\s+(fsid)\s+(\S+)\s*",
                                                r"\s+(devices)\s+([\S]+)\s*"]),
                                tag="ceph-lvm")
         s.add(sd, path=out_path)
         for results in s.run().find_sequence_sections(sd).values():
-            id = None
+            osdid = None
             fsid = None
             dev = None
             for result in results:
                 if result.tag == sd.start_tag:
-                    id = int(result.get(1))
+                    osdid = int(result.get(1))
                 elif result.tag == sd.body_tag:
                     if result.get(1) == "fsid":
                         fsid = result.get(2)
                     elif result.get(1) == "devices":
                         dev = result.get(2)
 
-            osds.append(CephOSD(id, fsid, dev))
+            osds.append(CephOSD(osdid, fsid, dev))
 
         return osds
 
     @cached_property
     def local_osds_use_bcache(self):
         """
         Returns True if any local osds are using bcache devices.
```

### Comparing `hotsos-1.15.post8/hotsos/core/plugins/system/system.py` & `hotsos-1.15.post9/hotsos/core/plugins/system/system.py`

 * *Files 2% similar despite different names*

```diff
@@ -124,16 +124,15 @@
 
         for line in apt_config_dump:
             ret = re.compile(r"^APT::Periodic::Unattended-Upgrade\s+"
                              "\"([0-9]+)\";").match(line)
             if ret:
                 if int(ret[1]) == 0:
                     return False
-                else:
-                    return True
+                return True
 
         return False
 
     @cached_property
     def ubuntu_pro_status(self):
         """Parse and retrieve Ubuntu Pro status
 
@@ -191,27 +190,27 @@
                       "the expected format")
             return {"status": "error"}
 
         result = {}
         result["status"] = "attached"
         result["services"] = {}
 
-        for id in ssects:
+        for sid in ssects:
             result["services"] = {**result["services"], **{
                 v.get(1): {
                     "entitled": v.get(2),
                     "status": v.get(3)
                 }
-                for v in ssects[id] if v.tag == service_status_seqdef.body_tag
+                for v in ssects[sid] if v.tag == service_status_seqdef.body_tag
             }}
 
-        for id in asects:
+        for sid in asects:
             result = {**result, **{
                 re.sub(r'\W+', '_', v.get(1).strip()).lower(): v.get(2).strip()
-                for v in asects[id]
+                for v in asects[sid]
             }}
 
         return result
 
     @cached_property
     def sysctl_all(self):
         return SYSCtlFactory().sysctl_all
```

### Comparing `hotsos-1.15.post8/hotsos/core/plugins/vault.py` & `hotsos-1.15.post9/hotsos/core/plugins/vault.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post8/hotsos/core/plugintools.py` & `hotsos-1.15.post9/hotsos/core/plugintools.py`

 * *Files 0% similar despite different names*

```diff
@@ -102,15 +102,15 @@
         @param data: The data object. This can be a dict, list, or a flat type
                      such as int or str.
         @param level: The current header level
         @return: A string expansion formatted in HTML of the data object.
         """
         if isinstance(data, dict):
             return self._expand_dict(data, level)
-        elif isinstance(data, list):
+        if isinstance(data, list):
             return self._expand_list(data, level)
 
         return data
 
     def dump(self, data):
         """Convert the data (dict) into an html document.
 
@@ -129,31 +129,29 @@
         for key in data:
             markdown_output += f'\n{level_prefix} {key}\n'
             markdown_output += self._expand(data[key], level + 1)
 
         return markdown_output
 
     def _expand_list(self, data):
-        markdown_output = '\n'
-        for item in data:
-            markdown_output += f'- {item}\n'
+        markdown_output = '\n%s' % ''.join(f'- {item}\n' for item in data)
 
         return markdown_output
 
     def _expand(self, data, level):
         """Expand the data object.
 
         @param data: The data object. This can be a dict, list, or a flat type
                      such as int or str.
         @param level: The current header level
         @return: string expansion formatted in markdown of the data object.
         """
         if isinstance(data, dict):
             return self._expand_dict(data, level)
-        elif isinstance(data, list):
+        if isinstance(data, list):
             return self._expand_list(data)
 
         return f'\n{data}\n'
 
     def dump(self, data):
         """Convert the data (dict) into a markdown document.
 
@@ -408,15 +406,15 @@
                     for key, entry in output.items():
                         out = {key: entry.data}
                         if subkey:
                             out = {subkey: out}
 
                         part_max = PluginPartBase.PLUGIN_PART_OFFSET_MAX
                         part_offset = part_info['part_yaml_offset']
-                        offset = ((part_offset * part_max) + entry.offset)
+                        offset = (part_offset * part_max) + entry.offset
                         part_mgr.save(out, offset=offset)
 
         if failed_parts:
             # always put these at the top
             part_mgr.save({'failed-parts': failed_parts}, offset=0)
 
         imgr = IssuesManager()
```

### Comparing `hotsos-1.15.post8/hotsos/core/search.py` & `hotsos-1.15.post9/hotsos/core/search.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post8/hotsos/core/utils.py` & `hotsos-1.15.post9/hotsos/core/utils.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post8/hotsos/core/ycheck/engine/common.py` & `hotsos-1.15.post9/hotsos/core/ycheck/engine/common.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post8/hotsos/core/ycheck/engine/properties/checks.py` & `hotsos-1.15.post9/hotsos/core/ycheck/engine/properties/checks.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 )
 from hotsos.core.ycheck.engine.properties.requires.requires import (
     YPropertyRequires
 )
 from hotsos.core.ycheck.engine.properties.search import (
     YPropertySearch,
 )
-from hotsos.core.ycheck.engine.properties.input import YPropertyInput
+from hotsos.core.ycheck.engine.properties.inputdef import YPropertyInput
 
 
 @add_to_property_catalog
 class YPropertyCheck(YPropertyMappedOverrideBase):
 
     @property
     def _search_results(self):
@@ -66,41 +66,41 @@
         # @checks.<checkname>.search.<setting>
         self.cache.set('search', self.search.cache)
         self.search.cache.set('num_results', len(results))
         if not results:
             return
 
         # Saves a list of files that contained search results.
-        sources = set([r.source_id for r in results])
+        sources = set(r.source_id for r in results)
         files = [self.context.search_obj.resolve_source_id(s) for s in sources]
         self.search.cache.set('files', files)
 
     def _result(self):
         if self.search:
             _results = self._search_results
             self._set_search_cache_info(_results)
             if not _results:
                 log.debug("check %s search has no matches so result=False",
                           self.name)
                 return False
 
             return True
-        elif self.requires:
+        if self.requires:
             if self.cache.requires:
                 result = self.cache.requires.passes
                 log.debug("check %s - using cached result=%s", self.name,
                           result)
             else:
                 result = self.requires.passes
                 self.cache.set('requires', self.requires.cache)
 
             return result
-        else:
-            raise Exception("no supported properties found in check {}".format(
-                            self.name))
+
+        raise Exception("no supported properties found in check {}".format(
+                        self.name))
 
     @cached_yproperty_attr
     def result(self):
         log.debug("executing check %s", self.name)
         result = self._result()
         log.debug("check %s result=%s", self.name, result)
         return result
@@ -109,37 +109,37 @@
 @add_to_property_catalog
 class YPropertyChecks(YPropertyOverrideBase):
 
     @classmethod
     def _override_keys(cls):
         return ['checks']
 
-    def initialise(self, vars, input, searcher, scenario):
+    def initialise(self, local_vardefs, global_input, searcher, scenario):
         """
         Perform initialisation tasks for this set of checks.
 
-        * create context containing vars for each check
+        * create context containing vardefs for each check
         * pre-load searches from all/any checks and get results. This needs to
           be done before check results are consumed.
 
-        @param vars: YPropertyVars object containing all variables defined in
-                     the context of these checks and that we wil pass on to all
-                     check def and properties.
-        @param input: YPropertyInput object
+        @param local_vardefs: YPropertyVars object containing all variables
+                              defined in the context of these checks and that
+                              we wil pass on the all check def and properties.
+        @param global_input: YPropertyInput object
         @param searcher: FileSearcher object
         """
-        self.check_context = YDefsContext({'vars': vars})
+        self.check_context = YDefsContext({'vars': local_vardefs})
 
         log.debug("pre-loading scenario '%s' checks searches into "
                   "filesearcher", scenario.name)
         # first load all the search definitions into the searcher
         for c in self._checks:
             if c.search:
                 # local takes precedence over global
-                _input = c.input or input
+                _input = c.input or global_input
                 if _input.command:
                     # don't apply constraints to command outputs
                     allow_constraints = False
                 else:
                     allow_constraints = True
 
                 for path in _input.paths:
```

### Comparing `hotsos-1.15.post8/hotsos/core/ycheck/engine/properties/common.py` & `hotsos-1.15.post9/hotsos/core/ycheck/engine/properties/common.py`

 * *Files 0% similar despite different names*

```diff
@@ -90,23 +90,23 @@
         return self._ydefs_context.get(key)
 
 
 class PropertyCacheRefResolver(object):
     """
     This class is used to resolve string references to property cache entries.
     """
-    def __init__(self, refstr, vars=None, checks=None):
+    def __init__(self, refstr, pcrr_vars=None, checks=None):
         log.debug("%s: resolving '%s'", self.__class__.__name__, refstr)
         self.refstr = refstr
         if not self.is_valid_cache_ref(refstr):
             msg = ("{} is not a valid property cache reference or variable".
                    format(refstr))
             raise Exception(msg)
 
-        self.vars = vars
+        self.vars = pcrr_vars
         self.checks = checks
         if self.reftype == 'checks' and checks is None:
             msg = ("{} is a checks cache reference but checks dict not "
                    "provided".format(refstr))
             raise Exception(msg)
 
     @property
@@ -117,19 +117,19 @@
 
         Supported formats:
             $varname[:func]
             @checks.<check_name>.<property_name>.<property_cache_key>[:func]
         """
         if self.refstr.startswith('$'):
             return "variable"
-        elif self.refstr.startswith('@checks.'):
+        if self.refstr.startswith('@checks.'):
             # This is an implementation of YPropertyChecks
             return "checks"
-        else:
-            raise Exception("unknown ref type")
+
+        raise Exception("unknown ref type")
 
     @property
     def _ref_body(self):
         """
         Strip the prefix from the reference string.
         """
         if self.reftype == 'variable':
@@ -211,15 +211,15 @@
                                      lambda value: isinstance(value, dict)],
                     'action': lambda value: ', '.join(sorted(set(value)))},
                   'first': {
                     'requirements': [lambda value: isinstance(value, list)],
                     'action': lambda value: value[0]}}
 
         if func in extras:
-            if not any([req(value) for req in extras[func]['requirements']]):
+            if not any(req(value) for req in extras[func]['requirements']):
                 log.warning("attempted to apply '%s' to value of "
                             "type %s", func, type(value))
                 return value
 
             return extras[func]['action'](value)
 
         return getattr(builtins, func)(value)
@@ -599,16 +599,16 @@
     @abc.abstractmethod
     def get_item_result_callback(self, item, is_default_group=False):
         """
         Must be implemented to evaluate a single item and return its
         result.
         """
 
-    def _is_op_group(self, property):
-        return property._override_name in self.VALID_GROUP_KEYS
+    def _is_op_group(self, prop):
+        return prop._override_name in self.VALID_GROUP_KEYS
 
     def eval_op_group_items(self, logical_op_group):
         """
         Evaluate single group of items and return their results as a list.
 
         @return: list of boolean values
         """
```

### Comparing `hotsos-1.15.post8/hotsos/core/ycheck/engine/properties/conclusions.py` & `hotsos-1.15.post9/hotsos/core/ycheck/engine/properties/conclusions.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,15 @@
         fdict = self.format_dict
         if not fdict:
             return self.message
 
         for key, value in fdict.items():  # pylint: disable=E1101
             if PropertyCacheRefResolver.is_valid_cache_ref(value):
                 rvalue = PropertyCacheRefResolver(value,
-                                                  vars=self.context.vars,
+                                                  pcrr_vars=self.context.vars,
                                                   checks=checks).resolve()
                 log.debug("updating format-dict key=%s with cached %s (%s)",
                           key, value, rvalue)
                 fdict[key] = rvalue
 
         message = self.message
         if message is not None:
@@ -205,21 +205,21 @@
 @add_to_property_catalog
 class YPropertyConclusions(YPropertyOverrideBase):
 
     @classmethod
     def _override_keys(cls):
         return ['conclusions']
 
-    def initialise(self, vars):
+    def initialise(self, ypvars):
         """
         Perform initialisation tasks for this set of conclusions.
 
         * create conclusions context containing vars
         """
-        self.conclusion_context = YDefsContext({'vars': vars})
+        self.conclusion_context = YDefsContext({'vars': ypvars})
 
     @cached_yproperty_attr
     def _conclusions(self):
         log.debug("parsing conclusions section")
         if not hasattr(self, 'conclusion_context'):
             raise Exception("conclusions not yet initialised")
```

### Comparing `hotsos-1.15.post8/hotsos/core/ycheck/engine/properties/input.py` & `hotsos-1.15.post9/hotsos/core/ycheck/engine/properties/inputdef.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post8/hotsos/core/ycheck/engine/properties/requires/common.py` & `hotsos-1.15.post9/hotsos/core/ycheck/engine/properties/requires/common.py`

 * *Files 3% similar despite different names*

```diff
@@ -98,44 +98,44 @@
                 else:
                     item = "{} {}".format(item, op[1])
 
             _result.append(item)
 
         return ' -> '.join(_result)
 
-    def _apply_op(self, op, input=None, expected=None, force_expected=False):
+    def _apply_op(self, op, opinput=None, expected=None, force_expected=False):
         """
         @param expected: can be a value or variable name that needs to be
                          resolved. Variable names are identified by having a
                          "$" prefix.
         """
         log.debug("op=%s, input=%s, expected=%s, force_expected=%s", op,
-                  input, expected, force_expected)
+                  opinput, expected, force_expected)
         try:
             if expected is not None or force_expected:
-                return getattr(operator, op)(input, expected)
+                return getattr(operator, op)(opinput, expected)
 
-            return getattr(operator, op)(input)
+            return getattr(operator, op)(opinput)
         except Exception:
             log.exception("failed to apply operator '%s'", op)
             raise
 
-    def apply_ops(self, ops, input=None, normalise_value_types=False):
+    def apply_ops(self, ops, opinput=None, normalise_value_types=False):
         """
         Takes a list of operations and processes each one where each takes as
         input the output of the previous.
 
         @param ops: list of tuples of operations and optional args.
-        @param input: the value that is used as input to the first operation.
+        @param opinput: the value that is used as input to the first operation.
         @param normalise_value_types: if an operation has an expected value and
                                       and this is True, the type of the input
                                       will be cast to that of the expectced
                                       value.
         """
-        log.debug("ops=%s, input=%s", ops, input)
+        log.debug("ops=%s, input=%s", ops, opinput)
         if type(ops) != list:
             raise Exception("Expected list of ops but got {}".
                             format(ops))
 
         for op in ops:
             expected = None
             force_expected = False
@@ -149,22 +149,22 @@
                     if type(expected) == str and expected.startswith("$"):
                         varname = expected.partition("$")[2]
                         varval = self.context.vars.resolve(varname)  # noqa, pylint: disable=E1101
                         expected = varval
 
                     if normalise_value_types:
                         log.debug("normalising type(input)=%s to "
-                                  "type(expected)=%s", type(input),
+                                  "type(expected)=%s", type(opinput),
                                   type(expected))
-                        input = type(expected)(input)
+                        opinput = type(expected)(opinput)
 
-            input = self._apply_op(op[0], input=input, expected=expected,
-                                   force_expected=force_expected)
+            opinput = self._apply_op(op[0], opinput=opinput, expected=expected,
+                                     force_expected=force_expected)
 
-        return input
+        return opinput
 
 
 class YRequirementTypeBase(YPropertyOverrideBase, OpsUtils):
 
     @property
     @abc.abstractmethod
     def _result(self):
```

### Comparing `hotsos-1.15.post8/hotsos/core/ycheck/engine/properties/requires/requires.py` & `hotsos-1.15.post9/hotsos/core/ycheck/engine/properties/requires/requires.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post8/hotsos/core/ycheck/engine/properties/requires/types/apt.py` & `hotsos-1.15.post9/hotsos/core/ycheck/engine/properties/requires/types/apt.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,18 +43,15 @@
                 lt_broken = pkg_version < DPKGVersionCompare(v_min)
             else:
                 lt_broken = None
 
             if lt_broken:
                 continue
 
-            if lte_max:
-                result = True
-            else:
-                result = False
+            result = lte_max
 
             break
 
         log.debug("package %s=%s within version ranges %s "
                   "(result=%s)", pkg, pkg_version, versions, result)
         return result
```

### Comparing `hotsos-1.15.post8/hotsos/core/ycheck/engine/properties/requires/types/config.py` & `hotsos-1.15.post9/hotsos/core/ycheck/engine/properties/requires/types/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -70,15 +70,15 @@
             if item.section:
                 actual = cfg_obj.get(item.key, section=item.section)
             else:
                 actual = cfg_obj.get(item.key)
 
             _result = item.allow_unset
             if item.ops and actual is not None:
-                _result = self.apply_ops(item.ops, input=actual,
+                _result = self.apply_ops(item.ops, opinput=actual,
                                          normalise_value_types=True)
             log.debug("assertion: %s (%s) %s result=%s",
                       item.key, actual, self.ops_to_str(item.ops or []),
                       _result)
             if not _result and n < len(handlers) - 1:
                 log.debug("assertion is false and there are more configs to "
                           "check so trying next")
```

### Comparing `hotsos-1.15.post8/hotsos/core/ycheck/engine/properties/requires/types/path.py` & `hotsos-1.15.post9/hotsos/core/ycheck/engine/properties/requires/types/path.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 
 from hotsos.core.log import log
-from hotsos.core.ycheck.engine.properties.input import YPropertyInputBase
+from hotsos.core.ycheck.engine.properties.inputdef import YPropertyInputBase
 from hotsos.core.ycheck.engine.properties.requires import (
     intercept_exception,
     YRequirementTypeBase,
 )
 
 
 class YRequirementTypePath(YPropertyInputBase, YRequirementTypeBase):
```

### Comparing `hotsos-1.15.post8/hotsos/core/ycheck/engine/properties/requires/types/pebble.py` & `hotsos-1.15.post9/hotsos/core/ycheck/engine/properties/requires/types/pebble.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post8/hotsos/core/ycheck/engine/properties/requires/types/property.py` & `hotsos-1.15.post9/hotsos/core/ycheck/engine/properties/requires/types/property.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,14 +17,14 @@
     def _result(self):
         if type(self.content) != dict:
             path = self.content
         else:
             path = self.content['path']
 
         actual = self.get_property(path)
-        result = self.apply_ops(self.ops, input=actual)
+        result = self.apply_ops(self.ops, opinput=actual)
         log.debug('requirement check: property %s %s (result=%s)',
                   path, self.ops_to_str(self.ops), result)
         self.cache.set('property', path)
         self.cache.set('ops', self.ops_to_str(self.ops))
         self.cache.set('value_actual', actual)
         return result
```

### Comparing `hotsos-1.15.post8/hotsos/core/ycheck/engine/properties/requires/types/snap.py` & `hotsos-1.15.post9/hotsos/core/ycheck/engine/properties/requires/types/snap.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post8/hotsos/core/ycheck/engine/properties/requires/types/systemd.py` & `hotsos-1.15.post9/hotsos/core/ycheck/engine/properties/requires/types/systemd.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,15 +64,15 @@
                     return False
             else:
                 log.debug("svc %s started before or same as %s "
                           "(delta=%s)", svc.name,
                           started_after.name, delta)
                 return False
 
-        return self.apply_ops(ops, input=svc.state)
+        return self.apply_ops(ops, opinput=svc.state)
 
     @property
     @intercept_exception
     def _result(self):
         cache_info = {}
         default_op = 'eq'
         _result = True
```

### Comparing `hotsos-1.15.post8/hotsos/core/ycheck/engine/properties/requires/types/varops.py` & `hotsos-1.15.post9/hotsos/core/ycheck/engine/properties/requires/types/varops.py`

 * *Files 23% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
     @property
     def ops(self):
         return self.content[1:]
 
     def _apply_ops(self):
         actual = self.resolve_var(self.name)
-        result = self.apply_ops(self.ops, input=actual)
+        result = self.apply_ops(self.ops, opinput=actual)
         log.debug('requirement check: varref %s %s (result=%s)',
                   actual, self.ops_to_str(self.ops), result)
         self.cache.set('ops', self.ops_to_str(self.ops))
         self.cache.set('value', actual)
         self.cache.set('name', self.name)
         return result
```

### Comparing `hotsos-1.15.post8/hotsos/core/ycheck/engine/properties/search.py` & `hotsos-1.15.post9/hotsos/core/ycheck/engine/properties/search.py`

 * *Files 1% similar despite different names*

```diff
@@ -349,15 +349,15 @@
             return patterns[0]
 
         return patterns
 
     @property
     def is_sequence_search(self):
         seq_keys = YPropertySequencePart._override_keys()
-        return any([getattr(self, key) for key in seq_keys])
+        return any(getattr(self, key) for key in seq_keys)
 
     @property
     def simple_search(self):
         if (self.is_sequence_search or not self.search_pattern or
                 self.passthrough_results_opt):
             return
 
@@ -407,19 +407,18 @@
 
             # NOTE: we don't use hints here
             tag = self.unique_search_tag
             sdef = SequenceSearchDef(start=sd_start, body=sd_body,
                                      end=sd_end, tag=tag)
             self.cache.set('sequence_search', sdef)
             return sdef
-        else:
-            log.warning("invalid sequence definition passthrough=%s "
-                        "start=%s, body=%s, end=%s",
-                        self.passthrough_results_opt, seq_start, seq_body,
-                        seq_end)
+
+        log.warning("invalid sequence definition passthrough=%s "
+                    "start=%s, body=%s, end=%s",
+                    self.passthrough_results_opt, seq_start, seq_body, seq_end)
 
     @property
     def sequence_passthrough_search(self):
         if not self.is_sequence_search or not self.passthrough_results_opt:
             return
 
         sdef = self.cache.sequence_passthrough_search
```

### Comparing `hotsos-1.15.post8/hotsos/core/ycheck/engine/properties/vars.py` & `hotsos-1.15.post9/hotsos/core/ycheck/engine/properties/vardef.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post8/hotsos/core/ycheck/events.py` & `hotsos-1.15.post9/hotsos/core/ycheck/events.py`

 * *Files 1% similar despite different names*

```diff
@@ -282,15 +282,15 @@
     @property
     def final_event_results(self):
         """
         This is a cache of the results obtained by running run().
         """
         return self.__final_event_results
 
-    def run(self, results):
+    def run(self, results=None):
         """
         Provide a default way for results to be processed.
 
         See defs/events.yaml for definitions.
         """
         if self.__final_event_results:
             return self.__final_event_results
```

### Comparing `hotsos-1.15.post8/hotsos/core/ycheck/scenarios.py` & `hotsos-1.15.post9/hotsos/core/ycheck/scenarios.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post8/hotsos/defs/events/openstack/neutron/agents.yaml` & `hotsos-1.15.post9/hotsos/defs/events/openstack/neutron/agents.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post8/hotsos/defs/events/openstack/nova/external-events.yaml` & `hotsos-1.15.post9/hotsos/defs/events/openstack/nova/external-events.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post8/hotsos/defs/events/openstack/octavia.yaml` & `hotsos-1.15.post9/hotsos/defs/events/openstack/octavia.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post8/hotsos/defs/events/openvswitch/ovn/errors-and-warnings.yaml` & `hotsos-1.15.post9/hotsos/defs/events/openvswitch/ovn/errors-and-warnings.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post8/hotsos/defs/events/openvswitch/ovn/ovn-central.yaml` & `hotsos-1.15.post9/hotsos/defs/events/openvswitch/ovn/ovn-central.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post8/hotsos/defs/events/openvswitch/ovn/ovn-controller.yaml` & `hotsos-1.15.post9/hotsos/defs/events/openvswitch/ovn/ovn-controller.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post8/hotsos/defs/events/openvswitch/ovs/ovs-vswitchd.yaml` & `hotsos-1.15.post9/hotsos/defs/events/openvswitch/ovs/ovs-vswitchd.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post8/hotsos/defs/events/storage/ceph/mon/monlogs.yaml` & `hotsos-1.15.post9/hotsos/defs/events/storage/ceph/mon/monlogs.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post8/hotsos/defs/scenarios/juju/bugs/lp1812361.yaml` & `hotsos-1.15.post9/hotsos/defs/scenarios/juju/bugs/lp1812361.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post8/hotsos/defs/scenarios/juju/bugs/lp1852502.yaml` & `hotsos-1.15.post9/hotsos/defs/scenarios/juju/bugs/lp1852502.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post8/hotsos/defs/scenarios/juju/bugs/lp1858519.yaml` & `hotsos-1.15.post9/hotsos/defs/scenarios/juju/bugs/lp1858519.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post8/hotsos/defs/scenarios/juju/bugs/lp1895040.yaml` & `hotsos-1.15.post9/hotsos/defs/scenarios/juju/bugs/lp1895040.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post8/hotsos/defs/scenarios/juju/bugs/lp1910958.yaml` & `hotsos-1.15.post9/hotsos/defs/scenarios/juju/bugs/lp1910958.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post8/hotsos/defs/scenarios/juju/bugs/lp1948906.yaml` & `hotsos-1.15.post9/hotsos/defs/scenarios/juju/bugs/lp1948906.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post8/hotsos/defs/scenarios/juju/bugs/lp1996230.yaml` & `hotsos-1.15.post9/hotsos/defs/scenarios/juju/bugs/lp1996230.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post8/hotsos/defs/scenarios/juju/charm_unit_checks.yaml` & `hotsos-1.15.post9/hotsos/defs/scenarios/juju/charm_unit_checks.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post8/hotsos/defs/scenarios/kernel/amd_iommu_pt.yaml` & `hotsos-1.15.post9/hotsos/defs/scenarios/kernel/amd_iommu_pt.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post8/hotsos/defs/scenarios/kernel/kernlog_calltrace.yaml` & `hotsos-1.15.post9/hotsos/defs/scenarios/kernel/kernlog_calltrace.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post8/hotsos/defs/scenarios/kernel/memory.yaml` & `hotsos-1.15.post9/hotsos/defs/scenarios/kernel/memory.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post8/hotsos/defs/scenarios/kernel/network/misc.yaml` & `hotsos-1.15.post9/hotsos/defs/scenarios/kernel/network/misc.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post8/hotsos/defs/scenarios/kernel/network/tcp.yaml` & `hotsos-1.15.post9/hotsos/defs/scenarios/kernel/network/tcp.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post8/hotsos/defs/scenarios/kernel/network/udp.yaml` & `hotsos-1.15.post9/hotsos/defs/scenarios/kernel/network/udp.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post8/hotsos/defs/scenarios/kernel/qla2xxx.yaml` & `hotsos-1.15.post9/hotsos/defs/scenarios/kernel/qla2xxx.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post8/hotsos/defs/scenarios/kubernetes/system_cpufreq_mode.yaml` & `hotsos-1.15.post9/hotsos/defs/scenarios/kubernetes/system_cpufreq_mode.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post8/hotsos/defs/scenarios/lxd/bugs/lp1807628.yaml` & `hotsos-1.15.post9/hotsos/defs/scenarios/lxd/bugs/lp1807628.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post8/hotsos/defs/scenarios/lxd/lxcfs_deadlock.yaml` & `hotsos-1.15.post9/hotsos/defs/scenarios/lxd/lxcfs_deadlock.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post8/hotsos/defs/scenarios/mysql/bugs/lp1959861.yaml` & `hotsos-1.15.post9/hotsos/defs/scenarios/mysql/bugs/lp1959861.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post8/hotsos/defs/scenarios/mysql/bugs/lp1971565.yaml` & `hotsos-1.15.post9/hotsos/defs/scenarios/mysql/bugs/lp1971565.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post8/hotsos/defs/scenarios/mysql/mysql_connections.yaml` & `hotsos-1.15.post9/hotsos/defs/scenarios/mysql/mysql_connections.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post8/hotsos/defs/scenarios/openstack/barbican/bugs/lp1946787.yaml` & `hotsos-1.15.post9/hotsos/defs/scenarios/openstack/barbican/bugs/lp1946787.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post8/hotsos/defs/scenarios/openstack/eol.yaml` & `hotsos-1.15.post9/hotsos/defs/scenarios/openstack/eol.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post8/hotsos/defs/scenarios/openstack/keystone/bugs/lp1896125.yaml` & `hotsos-1.15.post9/hotsos/defs/scenarios/openstack/keystone/bugs/lp1896125.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post8/hotsos/defs/scenarios/openstack/masakari/pacemaker_remote.yaml` & `hotsos-1.15.post9/hotsos/defs/scenarios/openstack/masakari/pacemaker_remote.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post8/hotsos/defs/scenarios/openstack/neutron/bugs/lp1794991.yaml` & `hotsos-1.15.post9/hotsos/defs/scenarios/openstack/neutron/bugs/lp1794991.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post8/hotsos/defs/scenarios/openstack/neutron/bugs/lp1907686.yaml` & `hotsos-1.15.post9/hotsos/defs/scenarios/openstack/neutron/bugs/lp1907686.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post8/hotsos/defs/scenarios/openstack/neutron/bugs/lp1927868.yaml` & `hotsos-1.15.post9/hotsos/defs/scenarios/openstack/neutron/bugs/lp1927868.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post8/hotsos/defs/scenarios/openstack/neutron/bugs/lp1960319.yaml` & `hotsos-1.15.post9/hotsos/defs/scenarios/openstack/neutron/bugs/lp1960319.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post8/hotsos/defs/scenarios/openstack/neutron/bugs/lp1979089.yaml` & `hotsos-1.15.post9/hotsos/defs/scenarios/openstack/neutron/bugs/lp1979089.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post8/hotsos/defs/scenarios/openstack/neutron/bugs/lp1993628.yaml` & `hotsos-1.15.post9/hotsos/defs/scenarios/openstack/neutron/bugs/lp1993628.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post8/hotsos/defs/scenarios/openstack/neutron/bugs/lp1996594.yaml` & `hotsos-1.15.post9/hotsos/defs/scenarios/openstack/neutron/bugs/lp1996594.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post8/hotsos/defs/scenarios/openstack/neutron/neutron_ovs_cleanup.yaml` & `hotsos-1.15.post9/hotsos/defs/scenarios/openstack/neutron/neutron_ovs_cleanup.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post8/hotsos/defs/scenarios/openstack/neutron/ovn_stale_db.yaml` & `hotsos-1.15.post9/hotsos/defs/scenarios/openstack/neutron/ovn_stale_db.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post8/hotsos/defs/scenarios/openstack/nova/bugs/lp1860743.yaml` & `hotsos-1.15.post9/hotsos/defs/scenarios/openstack/nova/bugs/lp1860743.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post8/hotsos/defs/scenarios/openstack/nova/bugs/lp1888395.yaml` & `hotsos-1.15.post9/hotsos/defs/scenarios/openstack/nova/bugs/lp1888395.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post8/hotsos/defs/scenarios/openstack/nova/bugs/lp1904580.yaml` & `hotsos-1.15.post9/hotsos/defs/scenarios/openstack/nova/bugs/lp1904580.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post8/hotsos/defs/scenarios/openstack/nova/bugs/lp1967956.yaml` & `hotsos-1.15.post9/hotsos/defs/scenarios/openstack/nova/bugs/lp1967956.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post8/hotsos/defs/scenarios/openstack/nova/config_checks.yaml` & `hotsos-1.15.post9/hotsos/defs/scenarios/openstack/nova/config_checks.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post8/hotsos/defs/scenarios/openstack/nova/cpu_pinning.yaml` & `hotsos-1.15.post9/hotsos/defs/scenarios/openstack/nova/cpu_pinning.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post8/hotsos/defs/scenarios/openstack/nova/service_mem_usage.yaml` & `hotsos-1.15.post9/hotsos/defs/scenarios/openstack/nova/service_mem_usage.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post8/hotsos/defs/scenarios/openstack/octavia/bugs/sb1896125.yaml` & `hotsos-1.15.post9/hotsos/defs/scenarios/openstack/octavia/bugs/sb1896125.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post8/hotsos/defs/scenarios/openstack/octavia/excessive_failovers.yaml` & `hotsos-1.15.post9/hotsos/defs/scenarios/openstack/octavia/excessive_failovers.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post8/hotsos/defs/scenarios/openstack/octavia/hm_port_health.yaml` & `hotsos-1.15.post9/hotsos/defs/scenarios/openstack/octavia/hm_port_health.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post8/hotsos/defs/scenarios/openstack/openstack_apache2_certificates.yaml` & `hotsos-1.15.post9/hotsos/defs/scenarios/openstack/openstack_apache2_certificates.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post8/hotsos/defs/scenarios/openstack/openstack_charm_conflicts.yaml` & `hotsos-1.15.post9/hotsos/defs/scenarios/openstack/openstack_charm_conflicts.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post8/hotsos/defs/scenarios/openstack/system_cpufreq_mode.yaml` & `hotsos-1.15.post9/hotsos/defs/scenarios/openstack/system_cpufreq_mode.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post8/hotsos/defs/scenarios/openstack/systemd_masked_services.yaml` & `hotsos-1.15.post9/hotsos/defs/scenarios/openstack/systemd_masked_services.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post8/hotsos/defs/scenarios/openvswitch/bugs/lp1839592.yaml` & `hotsos-1.15.post9/hotsos/defs/scenarios/openvswitch/bugs/lp1839592.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post8/hotsos/defs/scenarios/openvswitch/bugs/lp1978806.yaml` & `hotsos-1.15.post9/hotsos/defs/scenarios/openvswitch/bugs/lp1978806.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post8/hotsos/defs/scenarios/openvswitch/dpif_lost_packets.yaml` & `hotsos-1.15.post9/hotsos/defs/scenarios/openvswitch/dpif_lost_packets.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post8/hotsos/defs/scenarios/openvswitch/dpif_resubmit_actions.yaml` & `hotsos-1.15.post9/hotsos/defs/scenarios/openvswitch/dpif_resubmit_actions.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post8/hotsos/defs/scenarios/openvswitch/ovn/bfd_flapping.yaml` & `hotsos-1.15.post9/hotsos/defs/scenarios/openvswitch/ovn/bfd_flapping.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post8/hotsos/defs/scenarios/openvswitch/ovn/bugs/lp1865127.yaml` & `hotsos-1.15.post9/hotsos/defs/scenarios/openvswitch/ovn/bugs/lp1865127.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post8/hotsos/defs/scenarios/openvswitch/ovn/ovn_central_certs_logs.yaml` & `hotsos-1.15.post9/hotsos/defs/scenarios/openvswitch/ovn/ovn_central_certs_logs.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post8/hotsos/defs/scenarios/openvswitch/ovn/ovn_central_services.yaml` & `hotsos-1.15.post9/hotsos/defs/scenarios/openvswitch/ovn/ovn_central_services.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post8/hotsos/defs/scenarios/openvswitch/ovn/ovn_certs_valid.yaml` & `hotsos-1.15.post9/hotsos/defs/scenarios/openvswitch/ovn/ovn_certs_valid.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post8/hotsos/defs/scenarios/openvswitch/ovn/ovn_chassis_certs_logs.yaml` & `hotsos-1.15.post9/hotsos/defs/scenarios/openvswitch/ovn/ovn_chassis_certs_logs.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post8/hotsos/defs/scenarios/openvswitch/ovn/ovn_db_upgrade.yaml` & `hotsos-1.15.post9/hotsos/defs/scenarios/openvswitch/ovn/ovn_db_upgrade.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post8/hotsos/defs/scenarios/openvswitch/ovn/ovn_elections.yaml` & `hotsos-1.15.post9/hotsos/defs/scenarios/openvswitch/ovn/ovn_elections.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post8/hotsos/defs/scenarios/openvswitch/ovn/ovsdb_reconnect_errors.yaml` & `hotsos-1.15.post9/hotsos/defs/scenarios/openvswitch/ovn/ovsdb_reconnect_errors.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post8/hotsos/defs/scenarios/openvswitch/ovn/service_mem_usage.yaml` & `hotsos-1.15.post9/hotsos/defs/scenarios/openvswitch/ovn/service_mem_usage.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post8/hotsos/defs/scenarios/openvswitch/service_restarts.yaml` & `hotsos-1.15.post9/hotsos/defs/scenarios/openvswitch/service_restarts.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post8/hotsos/defs/scenarios/pacemaker/bugs/lp1874719.yaml` & `hotsos-1.15.post9/hotsos/defs/scenarios/pacemaker/bugs/lp1874719.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post8/hotsos/defs/scenarios/rabbitmq/bugs/lp1943937.yaml` & `hotsos-1.15.post9/hotsos/defs/scenarios/rabbitmq/bugs/lp1943937.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post8/hotsos/defs/scenarios/rabbitmq/cluster_config.yaml` & `hotsos-1.15.post9/hotsos/defs/scenarios/rabbitmq/cluster_config.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post8/hotsos/defs/scenarios/rabbitmq/cluster_logchecks.yaml` & `hotsos-1.15.post9/hotsos/defs/scenarios/rabbitmq/cluster_logchecks.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post8/hotsos/defs/scenarios/rabbitmq/cluster_resources.yaml` & `hotsos-1.15.post9/hotsos/defs/scenarios/rabbitmq/cluster_resources.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post8/hotsos/defs/scenarios/sosreport/plugin_timeouts.yaml` & `hotsos-1.15.post9/hotsos/defs/scenarios/sosreport/plugin_timeouts.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post8/hotsos/defs/scenarios/storage/bcache/bdev.yaml` & `hotsos-1.15.post9/hotsos/defs/scenarios/storage/bcache/bdev.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post8/hotsos/defs/scenarios/storage/bcache/cacheset.yaml` & `hotsos-1.15.post9/hotsos/defs/scenarios/storage/bcache/cacheset.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post8/hotsos/defs/scenarios/storage/ceph/ceph-mgr/autoscaler_overlap_roots.yaml` & `hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-mgr/autoscaler_overlap_roots.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post8/hotsos/defs/scenarios/storage/ceph/ceph-mon/auth_insecure_global_id_reclaim_allowed.yaml` & `hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/auth_insecure_global_id_reclaim_allowed.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post8/hotsos/defs/scenarios/storage/ceph/ceph-mon/autoscaler_bug.yaml` & `hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/autoscaler_bug.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post8/hotsos/defs/scenarios/storage/ceph/ceph-mon/bluefs_size.yaml` & `hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/bluefs_size.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post8/hotsos/defs/scenarios/storage/ceph/ceph-mon/bluefs_spillover.yaml` & `hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/bluefs_spillover.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post8/hotsos/defs/scenarios/storage/ceph/ceph-mon/ceph-mon.yaml` & `hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/ceph-mon.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post8/hotsos/defs/scenarios/storage/ceph/ceph-mon/ceph_address_overlap.yaml` & `hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/ceph_address_overlap.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post8/hotsos/defs/scenarios/storage/ceph/ceph-mon/ceph_cluster_health.yaml` & `hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/ceph_cluster_health.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post8/hotsos/defs/scenarios/storage/ceph/ceph-mon/ceph_versions_mismatch.yaml` & `hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/ceph_versions_mismatch.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post8/hotsos/defs/scenarios/storage/ceph/ceph-mon/crushmap_bucket_checks.yaml` & `hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/crushmap_bucket_checks.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post8/hotsos/defs/scenarios/storage/ceph/ceph-mon/empty_clog.yaml` & `hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/empty_clog.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post8/hotsos/defs/scenarios/storage/ceph/ceph-mon/eol.yaml` & `hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/eol.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post8/hotsos/defs/scenarios/storage/ceph/ceph-mon/laggy_pgs.yaml` & `hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/laggy_pgs.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post8/hotsos/defs/scenarios/storage/ceph/ceph-mon/large_omap_objects.yaml` & `hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/large_omap_objects.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post8/hotsos/defs/scenarios/storage/ceph/ceph-mon/meta_backend_mon.yaml` & `hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/meta_backend_mon.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post8/hotsos/defs/scenarios/storage/ceph/ceph-mon/mon_db_too_big.yaml` & `hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/mon_db_too_big.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post8/hotsos/defs/scenarios/storage/ceph/ceph-mon/mon_elections_flapping.yaml` & `hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/mon_elections_flapping.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post8/hotsos/defs/scenarios/storage/ceph/ceph-mon/osd_flapping.yaml` & `hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/osd_flapping.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post8/hotsos/defs/scenarios/storage/ceph/ceph-mon/osd_maps_backlog_too_large.yaml` & `hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/osd_maps_backlog_too_large.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post8/hotsos/defs/scenarios/storage/ceph/ceph-mon/osd_messenger_v2_protocol.yaml` & `hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/osd_messenger_v2_protocol.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post8/hotsos/defs/scenarios/storage/ceph/ceph-mon/osd_slow_heartbeats.yaml` & `hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/osd_slow_heartbeats.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post8/hotsos/defs/scenarios/storage/ceph/ceph-mon/osd_slow_ops.yaml` & `hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/osd_slow_ops.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post8/hotsos/defs/scenarios/storage/ceph/ceph-mon/pg_imbalance.yaml` & `hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/pg_imbalance.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post8/hotsos/defs/scenarios/storage/ceph/ceph-mon/pg_overdose.yaml` & `hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/pg_overdose.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post8/hotsos/defs/scenarios/storage/ceph/ceph-mon/required_osd_release_mismatch.yaml` & `hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/required_osd_release_mismatch.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post8/hotsos/defs/scenarios/storage/ceph/ceph-mon/rgw_frontend.yaml` & `hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/rgw_frontend.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post8/hotsos/defs/scenarios/storage/ceph/ceph-mon/ssds_using_bcache.yaml` & `hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/ssds_using_bcache.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post8/hotsos/defs/scenarios/storage/ceph/ceph-mon/unresponsive_mon_mgr.yaml` & `hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/unresponsive_mon_mgr.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post8/hotsos/defs/scenarios/storage/ceph/ceph-osd/bugs/lp1936136.yaml` & `hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-osd/bugs/lp1936136.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post8/hotsos/defs/scenarios/storage/ceph/ceph-osd/bugs/lp1959649.yaml` & `hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-osd/bugs/lp1959649.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post8/hotsos/defs/scenarios/storage/ceph/ceph-osd/bugs/lp1996010.yaml` & `hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-osd/bugs/lp1996010.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post8/hotsos/defs/scenarios/storage/ceph/ceph-osd/bugs/lp2013960.yaml` & `hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-osd/bugs/lp2013960.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post8/hotsos/defs/scenarios/storage/ceph/ceph-osd/bugs/lp2016845.yaml` & `hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-osd/bugs/lp2016845.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post8/hotsos/defs/scenarios/storage/ceph/ceph-osd/ceph_address_overlap.yaml` & `hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-osd/ceph_address_overlap.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post8/hotsos/defs/scenarios/storage/ceph/ceph-osd/eol.yaml` & `hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-osd/eol.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post8/hotsos/defs/scenarios/storage/ceph/ceph-osd/filestore_to_bluestore_upgrade.yaml` & `hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-osd/filestore_to_bluestore_upgrade.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post8/hotsos/defs/scenarios/storage/ceph/ceph-osd/juju_ceph_no_bcache_tuning.yaml` & `hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-osd/juju_ceph_no_bcache_tuning.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post8/hotsos/defs/scenarios/storage/ceph/ceph-osd/meta_backend_osd.yaml` & `hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-osd/meta_backend_osd.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post8/hotsos/defs/scenarios/storage/ceph/ceph-osd/osd_flapping.yaml` & `hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-osd/osd_flapping.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post8/hotsos/defs/scenarios/storage/ceph/ceph-osd/osd_latency.yaml` & `hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-osd/osd_latency.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post8/hotsos/defs/scenarios/storage/ceph/ceph-osd/osd_slow_ops.yaml` & `hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-osd/osd_slow_ops.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post8/hotsos/defs/scenarios/storage/ceph/ceph-osd/pg_overdose.yaml` & `hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-osd/pg_overdose.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post8/hotsos/defs/scenarios/storage/ceph/ceph-osd/ssd_osds_no_discard.yaml.disabled` & `hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-osd/ssd_osds_no_discard.yaml.disabled`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post8/hotsos/defs/scenarios/storage/ceph/ceph-osd/system_cpufreq_mode.yaml` & `hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-osd/system_cpufreq_mode.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post8/hotsos/defs/scenarios/storage/ceph/ceph-rgw/rgw_frontend_rgw.yaml` & `hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-rgw/rgw_frontend_rgw.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post8/hotsos/defs/scenarios/storage/ceph/common/ceph_charm_conflicts.yaml` & `hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/common/ceph_charm_conflicts.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post8/hotsos/plugin_extensions/juju/summary.py` & `hotsos-1.15.post9/hotsos/plugin_extensions/juju/summary.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     def error_and_warnings(self):
         log.debug("searching unit logs for errors and warnings")
         c = SearchConstraintSearchSince(ts_matcher_cls=JujuTimestampMatcher)
         searchobj = FileSearcher(constraint=c)
         path = os.path.join(HotSOSConfig.data_root, 'var/log/juju/unit-*.log')
         ts_expr = r"^([\d-]+)\s+([\d:]+)"
         for msg in ['ERROR', 'WARNING']:
-            expr = (r'{} {} (\S+) (\S+):\d+ '.format(ts_expr, msg))
+            expr = r'{} {} (\S+) (\S+):\d+ '.format(ts_expr, msg)
             tag = msg
             hint = msg
             searchobj.add(SearchDef(expr, tag=tag, hint=hint), path)
 
         results = searchobj.run()
         log.debug("fetching unit log results")
         events = {}
@@ -102,15 +102,15 @@
 
 class JujuSummary(JujuChecksBase):
 
     @idx(0)
     def __summary_services(self):
         if self.systemd.services:
             return self.systemd.summary
-        elif self.pebble.services:
+        if self.pebble.services:
             return self.pebble.summary
 
     @idx(1)
     def __summary_version(self):
         if self.machine:
             return self.machine.version
```

### Comparing `hotsos-1.15.post8/hotsos/plugin_extensions/kernel/summary.py` & `hotsos-1.15.post9/hotsos/plugin_extensions/kernel/summary.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post8/hotsos/plugin_extensions/kubernetes/summary.py` & `hotsos-1.15.post9/hotsos/plugin_extensions/kubernetes/summary.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 class KubernetesSummary(KubernetesChecksBase):
 
     @idx(0)
     def __summary_services(self):
         if self.systemd.services:
             return self.systemd.summary
-        elif self.pebble.services:
+        if self.pebble.services:
             return self.pebble.summary
 
     @idx(1)
     def __summary_snaps(self):
         snaps = self.snaps.all_formatted
         if snaps:
             return snaps
```

### Comparing `hotsos-1.15.post8/hotsos/plugin_extensions/lxd/summary.py` & `hotsos-1.15.post9/hotsos/plugin_extensions/lxd/summary.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post8/hotsos/plugin_extensions/openstack/agent/events.py` & `hotsos-1.15.post9/hotsos/plugin_extensions/openstack/agent/events.py`

 * *Files 0% similar despite different names*

```diff
@@ -252,15 +252,15 @@
             return
 
         max_transitions = 0
         warn_count = 0
         threshold = VRRP_TRANSITION_WARN_THRESHOLD
         for router in transitions:
             r = transitions[router]
-            _transitions = sum([t for d, t in r.items()])
+            _transitions = sum(t for d, t in r.items())
             if _transitions > threshold:
                 max_transitions = max(_transitions, max_transitions)
                 warn_count += 1
 
         if warn_count:
             msg = ("{} router(s) have had more than {} vrrp transitions "
                    "(max={}) in the last 24 hours.".format(warn_count,
```

### Comparing `hotsos-1.15.post8/hotsos/plugin_extensions/openstack/agent/exceptions.py` & `hotsos-1.15.post9/hotsos/plugin_extensions/openstack/agent/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -91,15 +91,15 @@
         return list(_exceptions)
 
     @property
     def files_w_exceptions(self):
         """ Return a list of files containing exceptions. """
         files = []
         for results in self.results.values():
-            sources = set([r.source_id for r in results])
+            sources = set(r.source_id for r in results)
             files.extend([self.source_id_resolver_callback(s)
                           for s in sources])
 
         return files
 
 
 class AgentExceptionChecks(OpenstackChecksBase):
```

### Comparing `hotsos-1.15.post8/hotsos/plugin_extensions/openstack/nova_external_events.py` & `hotsos-1.15.post9/hotsos/plugin_extensions/openstack/nova_external_events.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,15 +64,15 @@
             stages = self.get_state_dict(event.name)
             for stage in stages:
                 tag = "{}_{}_{}".format(instance_id, event_id, stage)
                 r = results.find_by_tag(tag, path=data_source)
                 if r:
                     stages[stage] = True
 
-            if all([stages[stage] for stage in stages]):
+            if all(stages[stage] for stage in stages):
                 result = 'succeeded'
             else:
                 result = 'failed'
 
             if result not in ext_output:
                 ext_output[result] = []
```

### Comparing `hotsos-1.15.post8/hotsos/plugin_extensions/openstack/service_features.py` & `hotsos-1.15.post9/hotsos/plugin_extensions/openstack/service_features.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post8/hotsos/plugin_extensions/openstack/service_network_checks.py` & `hotsos-1.15.post9/hotsos/plugin_extensions/openstack/service_network_checks.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post8/hotsos/plugin_extensions/openstack/summary.py` & `hotsos-1.15.post9/hotsos/plugin_extensions/openstack/summary.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
                 'days-to-eol': self.days_to_eol}
 
     @idx(1)
     def __summary_services(self):
         """Get string info for running services."""
         if self.systemd.services:
             return self.systemd.summary
-        elif self.pebble.services:
+        if self.pebble.services:
             return self.pebble.summary
 
     @idx(2)
     def __summary_dpkg(self):
         # require at least one core package to be installed to include
         # this in the report.
         if self.apt.core:
```

### Comparing `hotsos-1.15.post8/hotsos/plugin_extensions/openstack/vm_info.py` & `hotsos-1.15.post9/hotsos/plugin_extensions/openstack/vm_info.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post8/hotsos/plugin_extensions/openvswitch/event_checks.py` & `hotsos-1.15.post9/hotsos/plugin_extensions/openvswitch/event_checks.py`

 * *Files 2% similar despite different names*

```diff
@@ -114,16 +114,15 @@
 
             if port and _stats:
                 # Ports to ignore - see docstring for info
                 if (port in [b.name for b in self.ovs.bridges] or
                         re.compile(r"^(q|s)g-\S{11}$").match(port)):
                     continue
 
-                for key in _stats:
-                    s = _stats[key]
+                for _, s in _stats.items():
                     if s.get('dropped') and not s['packets']:
                         all_dropped.append(port)
 
                     if s.get('errors') and not s['packets']:
                         all_errors.append(port)
 
                 stats[port] = _stats
```

### Comparing `hotsos-1.15.post8/hotsos/plugin_extensions/openvswitch/summary.py` & `hotsos-1.15.post9/hotsos/plugin_extensions/openvswitch/summary.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         self.ovn = OVNBase()
 
     @idx(0)
     def __summary_services(self):
         """Get string info for running daemons."""
         if self.systemd.services:
             return self.systemd.summary
-        elif self.pebble.services:
+        if self.pebble.services:
             return self.pebble.summary
 
     @idx(1)
     def __summary_dpkg(self):
         return self.apt.all_formatted
 
     @idx(2)
```

### Comparing `hotsos-1.15.post8/hotsos/plugin_extensions/pacemaker/summary.py` & `hotsos-1.15.post9/hotsos/plugin_extensions/pacemaker/summary.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post8/hotsos/plugin_extensions/rabbitmq/summary.py` & `hotsos-1.15.post9/hotsos/plugin_extensions/rabbitmq/summary.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 class RabbitMQSummary(RabbitMQChecksBase):
 
     @idx(0)
     def __summary_services(self):
         if self.systemd.services:
             return self.systemd.summary
-        elif self.pebble.services:
+        if self.pebble.services:
             return self.pebble.summary
 
     @idx(1)
     def __summary_dpkg(self):
         apt = self.apt.all_formatted
         if apt:
             return apt
```

### Comparing `hotsos-1.15.post8/hotsos/plugin_extensions/sosreport/summary.py` & `hotsos-1.15.post9/hotsos/plugin_extensions/sosreport/summary.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post8/hotsos/plugin_extensions/storage/bcache_summary.py` & `hotsos-1.15.post9/hotsos/plugin_extensions/storage/bcache_summary.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post8/hotsos/plugin_extensions/storage/ceph_event_checks.py` & `hotsos-1.15.post9/hotsos/plugin_extensions/storage/ceph_event_checks.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post8/hotsos/plugin_extensions/storage/ceph_summary.py` & `hotsos-1.15.post9/hotsos/plugin_extensions/storage/ceph_summary.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
                 'days-to-eol': self.days_to_eol}
 
     @idx(1)
     def __summary_services(self):
         """Get string info for running services."""
         if self.systemd.services:
             return self.systemd.summary
-        elif self.pebble.services:
+        if self.pebble.services:
             return self.pebble.summary
 
     @idx(2)
     def __summary_dpkg(self):
         # require at least one core package to be installed to include
         # this in the report.
         if self.apt.core:
```

### Comparing `hotsos-1.15.post8/hotsos/plugin_extensions/system/checks.py` & `hotsos-1.15.post9/hotsos/plugin_extensions/system/checks.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post8/hotsos/plugin_extensions/system/summary.py` & `hotsos-1.15.post9/hotsos/plugin_extensions/system/summary.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,16 +40,15 @@
                 if ret:
                     return ret[1]
 
     @idx(6)
     def __summary_unattended_upgrades(self):
         if self.unattended_upgrades_enabled:
             return "ENABLED"
-        else:
-            return "disabled"
+        return "disabled"
 
     @idx(7)
     def __summary_date(self):
         return self.date
 
     @idx(8)
     def __summary_ubuntu_pro(self):
```

### Comparing `hotsos-1.15.post8/hotsos/templates/header.html` & `hotsos-1.15.post9/hotsos/templates/header.html`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post8/hotsos.egg-info/PKG-INFO` & `hotsos-1.15.post9/hotsos.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hotsos
-Version: 1.15.post8
+Version: 1.15.post9
 Summary: Software analysis toolkit. Define checks in high-level language and leverage library to perform analysis of common Cloud applications.
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Hotsos
```

### Comparing `hotsos-1.15.post8/hotsos.egg-info/SOURCES.txt` & `hotsos-1.15.post9/hotsos.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -84,17 +84,17 @@
 hotsos/core/ycheck/scenarios.py
 hotsos/core/ycheck/engine/__init__.py
 hotsos/core/ycheck/engine/common.py
 hotsos/core/ycheck/engine/properties/__init__.py
 hotsos/core/ycheck/engine/properties/checks.py
 hotsos/core/ycheck/engine/properties/common.py
 hotsos/core/ycheck/engine/properties/conclusions.py
-hotsos/core/ycheck/engine/properties/input.py
+hotsos/core/ycheck/engine/properties/inputdef.py
 hotsos/core/ycheck/engine/properties/search.py
-hotsos/core/ycheck/engine/properties/vars.py
+hotsos/core/ycheck/engine/properties/vardef.py
 hotsos/core/ycheck/engine/properties/requires/__init__.py
 hotsos/core/ycheck/engine/properties/requires/common.py
 hotsos/core/ycheck/engine/properties/requires/requires.py
 hotsos/core/ycheck/engine/properties/requires/types/__init__.py
 hotsos/core/ycheck/engine/properties/requires/types/apt.py
 hotsos/core/ycheck/engine/properties/requires/types/config.py
 hotsos/core/ycheck/engine/properties/requires/types/path.py
```

### Comparing `hotsos-1.15.post8/pyproject.toml` & `hotsos-1.15.post9/pyproject.toml`

 * *Files identical despite different names*

