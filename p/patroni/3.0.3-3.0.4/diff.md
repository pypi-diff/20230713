# Comparing `tmp/patroni-3.0.3.tar.gz` & `tmp/patroni-3.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "patroni-3.0.3.tar", last modified: Thu Jun 22 09:35:29 2023, max compression
+gzip compressed data, was "patroni-3.0.4.tar", last modified: Thu Jul 13 10:23:00 2023, max compression
```

## Comparing `patroni-3.0.3.tar` & `patroni-3.0.4.tar`

### file list

```diff
@@ -1,97 +1,97 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:35:29.793497 patroni-3.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-06-22 09:34:34.000000 patroni-3.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-22 09:34:34.000000 patroni-3.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    10213 2023-06-22 09:35:29.793497 patroni-3.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8683 2023-06-22 09:34:34.000000 patroni-3.0.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:35:29.781497 patroni-3.0.3/patroni/
--rw-r--r--   0 runner    (1001) docker     (123)     3156 2023-06-22 09:34:34.000000 patroni-3.0.3/patroni/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7100 2023-06-22 09:34:34.000000 patroni-3.0.3/patroni/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    80913 2023-06-22 09:34:34.000000 patroni-3.0.3/patroni/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     9059 2023-06-22 09:34:34.000000 patroni-3.0.3/patroni/async_executor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6893 2023-06-22 09:34:34.000000 patroni-3.0.3/patroni/collections.py
--rw-r--r--   0 runner    (1001) docker     (123)    27495 2023-06-22 09:34:34.000000 patroni-3.0.3/patroni/config.py
--rw-r--r--   0 runner    (1001) docker     (123)   101506 2023-06-22 09:34:34.000000 patroni-3.0.3/patroni/ctl.py
--rw-r--r--   0 runner    (1001) docker     (123)     5794 2023-06-22 09:34:34.000000 patroni-3.0.3/patroni/daemon.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:35:29.785497 patroni-3.0.3/patroni/dcs/
--rw-r--r--   0 runner    (1001) docker     (123)    46749 2023-06-22 09:34:34.000000 patroni-3.0.3/patroni/dcs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28487 2023-06-22 09:34:34.000000 patroni-3.0.3/patroni/dcs/consul.py
--rw-r--r--   0 runner    (1001) docker     (123)    37993 2023-06-22 09:34:34.000000 patroni-3.0.3/patroni/dcs/etcd.py
--rw-r--r--   0 runner    (1001) docker     (123)    38667 2023-06-22 09:34:34.000000 patroni-3.0.3/patroni/dcs/etcd3.py
--rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-06-22 09:34:34.000000 patroni-3.0.3/patroni/dcs/exhibitor.py
--rw-r--r--   0 runner    (1001) docker     (123)    63888 2023-06-22 09:34:34.000000 patroni-3.0.3/patroni/dcs/kubernetes.py
--rw-r--r--   0 runner    (1001) docker     (123)    19589 2023-06-22 09:34:34.000000 patroni-3.0.3/patroni/dcs/raft.py
--rw-r--r--   0 runner    (1001) docker     (123)    23478 2023-06-22 09:34:34.000000 patroni-3.0.3/patroni/dcs/zookeeper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-06-22 09:34:34.000000 patroni-3.0.3/patroni/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    99560 2023-06-22 09:34:34.000000 patroni-3.0.3/patroni/ha.py
--rw-r--r--   0 runner    (1001) docker     (123)    15509 2023-06-22 09:34:34.000000 patroni-3.0.3/patroni/log.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:35:29.785497 patroni-3.0.3/patroni/postgresql/
--rw-r--r--   0 runner    (1001) docker     (123)    58454 2023-06-22 09:34:34.000000 patroni-3.0.3/patroni/postgresql/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:35:29.785497 patroni-3.0.3/patroni/postgresql/available_parameters/
--rw-r--r--   0 runner    (1001) docker     (123)    35206 2023-06-22 09:34:34.000000 patroni-3.0.3/patroni/postgresql/available_parameters/0_postgres.yml
--rw-r--r--   0 runner    (1001) docker     (123)    21084 2023-06-22 09:34:34.000000 patroni-3.0.3/patroni/postgresql/bootstrap.py
--rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-06-22 09:34:34.000000 patroni-3.0.3/patroni/postgresql/callback_executor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4650 2023-06-22 09:34:34.000000 patroni-3.0.3/patroni/postgresql/cancellable.py
--rw-r--r--   0 runner    (1001) docker     (123)    19084 2023-06-22 09:34:34.000000 patroni-3.0.3/patroni/postgresql/citus.py
--rw-r--r--   0 runner    (1001) docker     (123)    58180 2023-06-22 09:34:34.000000 patroni-3.0.3/patroni/postgresql/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-06-22 09:34:34.000000 patroni-3.0.3/patroni/postgresql/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-06-22 09:34:34.000000 patroni-3.0.3/patroni/postgresql/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)    11101 2023-06-22 09:34:34.000000 patroni-3.0.3/patroni/postgresql/postmaster.py
--rw-r--r--   0 runner    (1001) docker     (123)    27305 2023-06-22 09:34:34.000000 patroni-3.0.3/patroni/postgresql/rewind.py
--rw-r--r--   0 runner    (1001) docker     (123)    23361 2023-06-22 09:34:34.000000 patroni-3.0.3/patroni/postgresql/slots.py
--rw-r--r--   0 runner    (1001) docker     (123)    13166 2023-06-22 09:34:34.000000 patroni-3.0.3/patroni/postgresql/sync.py
--rw-r--r--   0 runner    (1001) docker     (123)    20981 2023-06-22 09:34:34.000000 patroni-3.0.3/patroni/postgresql/validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4855 2023-06-22 09:34:34.000000 patroni-3.0.3/patroni/psycopg.py
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-06-22 09:34:34.000000 patroni-3.0.3/patroni/raft_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     7414 2023-06-22 09:34:34.000000 patroni-3.0.3/patroni/request.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:35:29.785497 patroni-3.0.3/patroni/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 09:34:34.000000 patroni-3.0.3/patroni/scripts/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3234 2023-06-22 09:34:34.000000 patroni-3.0.3/patroni/scripts/aws.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14799 2023-06-22 09:34:34.000000 patroni-3.0.3/patroni/scripts/wale_restore.py
--rw-r--r--   0 runner    (1001) docker     (123)    38346 2023-06-22 09:34:34.000000 patroni-3.0.3/patroni/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    42923 2023-06-22 09:34:34.000000 patroni-3.0.3/patroni/validator.py
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-22 09:34:34.000000 patroni-3.0.3/patroni/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:35:29.785497 patroni-3.0.3/patroni/watchdog/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-22 09:34:34.000000 patroni-3.0.3/patroni/watchdog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12608 2023-06-22 09:34:34.000000 patroni-3.0.3/patroni/watchdog/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     8514 2023-06-22 09:34:34.000000 patroni-3.0.3/patroni/watchdog/linux.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:35:29.781497 patroni-3.0.3/patroni.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10213 2023-06-22 09:35:29.000000 patroni-3.0.3/patroni.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-06-22 09:35:29.000000 patroni-3.0.3/patroni.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 09:35:29.000000 patroni-3.0.3/patroni.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-22 09:35:29.000000 patroni-3.0.3/patroni.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-22 09:35:29.000000 patroni-3.0.3/patroni.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-22 09:35:29.000000 patroni-3.0.3/patroni.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-22 09:34:34.000000 patroni-3.0.3/requirements.dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-22 09:34:34.000000 patroni-3.0.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 09:35:29.793497 patroni-3.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     5826 2023-06-22 09:34:34.000000 patroni-3.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:35:29.793497 patroni-3.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    31192 2023-06-22 09:34:34.000000 patroni-3.0.3/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-06-22 09:34:34.000000 patroni-3.0.3/tests/test_async_executor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-06-22 09:34:34.000000 patroni-3.0.3/tests/test_aws.py
--rw-r--r--   0 runner    (1001) docker     (123)    13392 2023-06-22 09:34:34.000000 patroni-3.0.3/tests/test_bootstrap.py
--rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-06-22 09:34:34.000000 patroni-3.0.3/tests/test_callback_executor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-06-22 09:34:34.000000 patroni-3.0.3/tests/test_cancellable.py
--rw-r--r--   0 runner    (1001) docker     (123)     9257 2023-06-22 09:34:34.000000 patroni-3.0.3/tests/test_citus.py
--rw-r--r--   0 runner    (1001) docker     (123)     6878 2023-06-22 09:34:34.000000 patroni-3.0.3/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    16072 2023-06-22 09:34:34.000000 patroni-3.0.3/tests/test_consul.py
--rw-r--r--   0 runner    (1001) docker     (123)    36966 2023-06-22 09:34:34.000000 patroni-3.0.3/tests/test_ctl.py
--rw-r--r--   0 runner    (1001) docker     (123)    16718 2023-06-22 09:34:34.000000 patroni-3.0.3/tests/test_etcd.py
--rw-r--r--   0 runner    (1001) docker     (123)    14889 2023-06-22 09:34:34.000000 patroni-3.0.3/tests/test_etcd3.py
--rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-06-22 09:34:34.000000 patroni-3.0.3/tests/test_exhibitor.py
--rw-r--r--   0 runner    (1001) docker     (123)    78479 2023-06-22 09:34:34.000000 patroni-3.0.3/tests/test_ha.py
--rw-r--r--   0 runner    (1001) docker     (123)    24674 2023-06-22 09:34:34.000000 patroni-3.0.3/tests/test_kubernetes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-06-22 09:34:34.000000 patroni-3.0.3/tests/test_log.py
--rw-r--r--   0 runner    (1001) docker     (123)     8333 2023-06-22 09:34:34.000000 patroni-3.0.3/tests/test_patroni.py
--rw-r--r--   0 runner    (1001) docker     (123)    46321 2023-06-22 09:34:34.000000 patroni-3.0.3/tests/test_postgresql.py
--rw-r--r--   0 runner    (1001) docker     (123)     7547 2023-06-22 09:34:34.000000 patroni-3.0.3/tests/test_postmaster.py
--rw-r--r--   0 runner    (1001) docker     (123)     7524 2023-06-22 09:34:34.000000 patroni-3.0.3/tests/test_raft.py
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-06-22 09:34:34.000000 patroni-3.0.3/tests/test_raft_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)    15833 2023-06-22 09:34:34.000000 patroni-3.0.3/tests/test_rewind.py
--rw-r--r--   0 runner    (1001) docker     (123)     9001 2023-06-22 09:34:34.000000 patroni-3.0.3/tests/test_slots.py
--rw-r--r--   0 runner    (1001) docker     (123)     5421 2023-06-22 09:34:34.000000 patroni-3.0.3/tests/test_sync.py
--rw-r--r--   0 runner    (1001) docker     (123)     4276 2023-06-22 09:34:34.000000 patroni-3.0.3/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11919 2023-06-22 09:34:34.000000 patroni-3.0.3/tests/test_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6791 2023-06-22 09:34:34.000000 patroni-3.0.3/tests/test_wale_restore.py
--rw-r--r--   0 runner    (1001) docker     (123)     9127 2023-06-22 09:34:34.000000 patroni-3.0.3/tests/test_watchdog.py
--rw-r--r--   0 runner    (1001) docker     (123)    12429 2023-06-22 09:34:34.000000 patroni-3.0.3/tests/test_zookeeper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:23:00.144235 patroni-3.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-07-13 10:22:09.000000 patroni-3.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-13 10:22:09.000000 patroni-3.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10209 2023-07-13 10:23:00.144235 patroni-3.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8679 2023-07-13 10:22:09.000000 patroni-3.0.4/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:23:00.136235 patroni-3.0.4/patroni/
+-rw-r--r--   0 runner    (1001) docker     (123)     3156 2023-07-13 10:22:09.000000 patroni-3.0.4/patroni/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7755 2023-07-13 10:22:09.000000 patroni-3.0.4/patroni/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    82325 2023-07-13 10:22:09.000000 patroni-3.0.4/patroni/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9059 2023-07-13 10:22:09.000000 patroni-3.0.4/patroni/async_executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6893 2023-07-13 10:22:09.000000 patroni-3.0.4/patroni/collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27495 2023-07-13 10:22:09.000000 patroni-3.0.4/patroni/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)   101568 2023-07-13 10:22:09.000000 patroni-3.0.4/patroni/ctl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5794 2023-07-13 10:22:09.000000 patroni-3.0.4/patroni/daemon.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:23:00.140235 patroni-3.0.4/patroni/dcs/
+-rw-r--r--   0 runner    (1001) docker     (123)    46802 2023-07-13 10:22:09.000000 patroni-3.0.4/patroni/dcs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28670 2023-07-13 10:22:09.000000 patroni-3.0.4/patroni/dcs/consul.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38262 2023-07-13 10:22:09.000000 patroni-3.0.4/patroni/dcs/etcd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38844 2023-07-13 10:22:09.000000 patroni-3.0.4/patroni/dcs/etcd3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-07-13 10:22:09.000000 patroni-3.0.4/patroni/dcs/exhibitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63858 2023-07-13 10:22:09.000000 patroni-3.0.4/patroni/dcs/kubernetes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19589 2023-07-13 10:22:09.000000 patroni-3.0.4/patroni/dcs/raft.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23478 2023-07-13 10:22:09.000000 patroni-3.0.4/patroni/dcs/zookeeper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-07-13 10:22:09.000000 patroni-3.0.4/patroni/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)   102190 2023-07-13 10:22:09.000000 patroni-3.0.4/patroni/ha.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15509 2023-07-13 10:22:09.000000 patroni-3.0.4/patroni/log.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:23:00.140235 patroni-3.0.4/patroni/postgresql/
+-rw-r--r--   0 runner    (1001) docker     (123)    60661 2023-07-13 10:22:09.000000 patroni-3.0.4/patroni/postgresql/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:23:00.140235 patroni-3.0.4/patroni/postgresql/available_parameters/
+-rw-r--r--   0 runner    (1001) docker     (123)    35206 2023-07-13 10:22:09.000000 patroni-3.0.4/patroni/postgresql/available_parameters/0_postgres.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    21107 2023-07-13 10:22:09.000000 patroni-3.0.4/patroni/postgresql/bootstrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-07-13 10:22:09.000000 patroni-3.0.4/patroni/postgresql/callback_executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4650 2023-07-13 10:22:09.000000 patroni-3.0.4/patroni/postgresql/cancellable.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19084 2023-07-13 10:22:09.000000 patroni-3.0.4/patroni/postgresql/citus.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58301 2023-07-13 10:22:09.000000 patroni-3.0.4/patroni/postgresql/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-07-13 10:22:09.000000 patroni-3.0.4/patroni/postgresql/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-07-13 10:22:09.000000 patroni-3.0.4/patroni/postgresql/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11101 2023-07-13 10:22:09.000000 patroni-3.0.4/patroni/postgresql/postmaster.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27305 2023-07-13 10:22:09.000000 patroni-3.0.4/patroni/postgresql/rewind.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24084 2023-07-13 10:22:09.000000 patroni-3.0.4/patroni/postgresql/slots.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13229 2023-07-13 10:22:09.000000 patroni-3.0.4/patroni/postgresql/sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20981 2023-07-13 10:22:09.000000 patroni-3.0.4/patroni/postgresql/validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4855 2023-07-13 10:22:09.000000 patroni-3.0.4/patroni/psycopg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-07-13 10:22:09.000000 patroni-3.0.4/patroni/raft_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7414 2023-07-13 10:22:09.000000 patroni-3.0.4/patroni/request.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:23:00.140235 patroni-3.0.4/patroni/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 10:22:09.000000 patroni-3.0.4/patroni/scripts/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3234 2023-07-13 10:22:09.000000 patroni-3.0.4/patroni/scripts/aws.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14799 2023-07-13 10:22:09.000000 patroni-3.0.4/patroni/scripts/wale_restore.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38723 2023-07-13 10:22:09.000000 patroni-3.0.4/patroni/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42892 2023-07-13 10:22:09.000000 patroni-3.0.4/patroni/validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-13 10:22:09.000000 patroni-3.0.4/patroni/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:23:00.140235 patroni-3.0.4/patroni/watchdog/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-13 10:22:09.000000 patroni-3.0.4/patroni/watchdog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12608 2023-07-13 10:22:09.000000 patroni-3.0.4/patroni/watchdog/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8514 2023-07-13 10:22:09.000000 patroni-3.0.4/patroni/watchdog/linux.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:23:00.136235 patroni-3.0.4/patroni.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10209 2023-07-13 10:23:00.000000 patroni-3.0.4/patroni.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-07-13 10:23:00.000000 patroni-3.0.4/patroni.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 10:23:00.000000 patroni-3.0.4/patroni.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-13 10:23:00.000000 patroni-3.0.4/patroni.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-07-13 10:23:00.000000 patroni-3.0.4/patroni.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-13 10:23:00.000000 patroni-3.0.4/patroni.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-13 10:22:09.000000 patroni-3.0.4/requirements.dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-13 10:22:09.000000 patroni-3.0.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 10:23:00.144235 patroni-3.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     5856 2023-07-13 10:22:09.000000 patroni-3.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:23:00.144235 patroni-3.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    31056 2023-07-13 10:22:09.000000 patroni-3.0.4/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-07-13 10:22:09.000000 patroni-3.0.4/tests/test_async_executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-07-13 10:22:09.000000 patroni-3.0.4/tests/test_aws.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13392 2023-07-13 10:22:09.000000 patroni-3.0.4/tests/test_bootstrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-07-13 10:22:09.000000 patroni-3.0.4/tests/test_callback_executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-07-13 10:22:09.000000 patroni-3.0.4/tests/test_cancellable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9257 2023-07-13 10:22:09.000000 patroni-3.0.4/tests/test_citus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6878 2023-07-13 10:22:09.000000 patroni-3.0.4/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16072 2023-07-13 10:22:09.000000 patroni-3.0.4/tests/test_consul.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36966 2023-07-13 10:22:09.000000 patroni-3.0.4/tests/test_ctl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16718 2023-07-13 10:22:09.000000 patroni-3.0.4/tests/test_etcd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14889 2023-07-13 10:22:09.000000 patroni-3.0.4/tests/test_etcd3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-07-13 10:22:09.000000 patroni-3.0.4/tests/test_exhibitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    78993 2023-07-13 10:22:09.000000 patroni-3.0.4/tests/test_ha.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24674 2023-07-13 10:22:09.000000 patroni-3.0.4/tests/test_kubernetes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-07-13 10:22:09.000000 patroni-3.0.4/tests/test_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10089 2023-07-13 10:22:09.000000 patroni-3.0.4/tests/test_patroni.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46321 2023-07-13 10:22:09.000000 patroni-3.0.4/tests/test_postgresql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7547 2023-07-13 10:22:09.000000 patroni-3.0.4/tests/test_postmaster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7524 2023-07-13 10:22:09.000000 patroni-3.0.4/tests/test_raft.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-07-13 10:22:09.000000 patroni-3.0.4/tests/test_raft_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15870 2023-07-13 10:22:09.000000 patroni-3.0.4/tests/test_rewind.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9025 2023-07-13 10:22:09.000000 patroni-3.0.4/tests/test_slots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5421 2023-07-13 10:22:09.000000 patroni-3.0.4/tests/test_sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4276 2023-07-13 10:22:09.000000 patroni-3.0.4/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11919 2023-07-13 10:22:09.000000 patroni-3.0.4/tests/test_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6791 2023-07-13 10:22:09.000000 patroni-3.0.4/tests/test_wale_restore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9127 2023-07-13 10:22:09.000000 patroni-3.0.4/tests/test_watchdog.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12429 2023-07-13 10:22:09.000000 patroni-3.0.4/tests/test_zookeeper.py
```

### Comparing `patroni-3.0.3/LICENSE` & `patroni-3.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `patroni-3.0.3/PKG-INFO` & `patroni-3.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: patroni
-Version: 3.0.3
+Version: 3.0.4
 Summary: PostgreSQL High-Available orchestrator and CLI
 Home-page: https://github.com/zalando/patroni
 Author: Alexander Kukushkin, Polina Bungina
 Author-email: akukushkin@microsoft.com, polina.bungina@zalando.de
 License: The MIT License
 Keywords: etcd governor patroni postgresql postgres ha haproxy confd zookeeper exhibitor consul streaming replication kubernetes k8s
 Classifier: Development Status :: 5 - Production/Stable
@@ -41,15 +41,15 @@
 --------------------------------------------------------------------
 
 You can find a version of this documentation that is searchable and also easier to navigate at `patroni.readthedocs.io <https://patroni.readthedocs.io>`__.
 
 
 There are many ways to run high availability with PostgreSQL; for a list, see the `PostgreSQL Documentation <https://wiki.postgresql.org/wiki/Replication,_Clustering,_and_Connection_Pooling>`__.
 
-Patroni is a template for high availability (HA) PostgreSQL solutions using Python. For maximum accessibility, Patroni supports a variety of distributed configuration stores like `ZooKeeper <https://zookeeper.apache.org/>`__, `etcd <https://github.com/coreos/etcd>`__, `Consul <https://github.com/hashicorp/consul>`__ or `Kubernetes <https://kubernetes.io>`__. Database engineers, DBAs, DevOps engineers, and SREs who are looking to quickly deploy HA PostgreSQL in datacenters — or anywhere else — will hopefully find it useful.
+Patroni is a template for high availability (HA) PostgreSQL solutions using Python. For maximum accessibility, Patroni supports a variety of distributed configuration stores like `ZooKeeper <https://zookeeper.apache.org/>`__, `etcd <https://github.com/coreos/etcd>`__, `Consul <https://github.com/hashicorp/consul>`__ or `Kubernetes <https://kubernetes.io>`__. Database engineers, DBAs, DevOps engineers, and SREs who are looking to quickly deploy HA PostgreSQL in datacenters - or anywhere else - will hopefully find it useful.
 
 We call Patroni a "template" because it is far from being a one-size-fits-all or plug-and-play replication system. It will have its own caveats. Use wisely.
 
 Currently supported PostgreSQL versions: 9.3 to 15.
 
 **Note to Citus users**: Starting from 3.0 Patroni nicely integrates with the `Citus <https://github.com/citusdata/citus>`__ database extension to Postgres. Please check the `Citus support page <https://github.com/zalando/patroni/blob/master/docs/citus.rst>`__ in the Patroni documentation for more info about how to use Patroni high availability together with a Citus distributed cluster.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `patroni-3.0.3/README.rst` & `patroni-3.0.4/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 --------------------------------------------------------------------
 
 You can find a version of this documentation that is searchable and also easier to navigate at `patroni.readthedocs.io <https://patroni.readthedocs.io>`__.
 
 
 There are many ways to run high availability with PostgreSQL; for a list, see the `PostgreSQL Documentation <https://wiki.postgresql.org/wiki/Replication,_Clustering,_and_Connection_Pooling>`__.
 
-Patroni is a template for high availability (HA) PostgreSQL solutions using Python. For maximum accessibility, Patroni supports a variety of distributed configuration stores like `ZooKeeper <https://zookeeper.apache.org/>`__, `etcd <https://github.com/coreos/etcd>`__, `Consul <https://github.com/hashicorp/consul>`__ or `Kubernetes <https://kubernetes.io>`__. Database engineers, DBAs, DevOps engineers, and SREs who are looking to quickly deploy HA PostgreSQL in datacenters — or anywhere else — will hopefully find it useful.
+Patroni is a template for high availability (HA) PostgreSQL solutions using Python. For maximum accessibility, Patroni supports a variety of distributed configuration stores like `ZooKeeper <https://zookeeper.apache.org/>`__, `etcd <https://github.com/coreos/etcd>`__, `Consul <https://github.com/hashicorp/consul>`__ or `Kubernetes <https://kubernetes.io>`__. Database engineers, DBAs, DevOps engineers, and SREs who are looking to quickly deploy HA PostgreSQL in datacenters - or anywhere else - will hopefully find it useful.
 
 We call Patroni a "template" because it is far from being a one-size-fits-all or plug-and-play replication system. It will have its own caveats. Use wisely.
 
 Currently supported PostgreSQL versions: 9.3 to 15.
 
 **Note to Citus users**: Starting from 3.0 Patroni nicely integrates with the `Citus <https://github.com/citusdata/citus>`__ database extension to Postgres. Please check the `Citus support page <https://github.com/zalando/patroni/blob/master/docs/citus.rst>`__ in the Patroni documentation for more info about how to use Patroni high availability together with a Citus distributed cluster.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `patroni-3.0.3/patroni/__init__.py` & `patroni-3.0.4/patroni/__init__.py`

 * *Files identical despite different names*

### Comparing `patroni-3.0.3/patroni/__main__.py` & `patroni-3.0.4/patroni/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,20 +26,23 @@
         from patroni.version import __version__
         from patroni.watchdog import Watchdog
 
         super(Patroni, self).__init__(config)
 
         self.version = __version__
         self.dcs = get_dcs(self.config)
+        self.request = PatroniRequest(self.config, True)
+
+        self.ensure_unique_name()
+
         self.watchdog = Watchdog(self.config)
         self.load_dynamic_configuration()
 
         self.postgresql = Postgresql(self.config['postgresql'])
         self.api = RestApiServer(self, self.config['restapi'])
-        self.request = PatroniRequest(self.config, True)
         self.ha = Ha(self)
 
         self.tags = self.get_tags()
         self.next_run = time.time()
         self.scheduled_restart: Dict[str, Any] = {}
 
     def load_dynamic_configuration(self) -> None:
@@ -56,14 +59,31 @@
                         self.dcs.reload_config(self.config)
                         self.watchdog.reload_config(self.config)
                 break
             except DCSError:
                 logger.warning('Can not get cluster from dcs')
                 time.sleep(5)
 
+    def ensure_unique_name(self) -> None:
+        """A helper method to prevent splitbrain from operator naming error."""
+        from patroni.dcs import Member
+
+        cluster = self.dcs.get_cluster()
+        if not cluster:
+            return
+        member = cluster.get_member(self.config['name'], False)
+        if not isinstance(member, Member):
+            return
+        try:
+            _ = self.request(member, endpoint="/liveness")
+            logger.fatal("Can't start; there is already a node named '%s' running", self.config['name'])
+            sys.exit(1)
+        except Exception:
+            return
+
     def get_tags(self) -> Dict[str, Any]:
         return {tag: value for tag, value in self.config.get('tags', {}).items()
                 if tag not in ('clonefrom', 'nofailover', 'noloadbalance', 'nosync') or value}
 
     @property
     def nofailover(self) -> bool:
         return bool(self.tags.get('nofailover', False))
```

### Comparing `patroni-3.0.3/patroni/api.py` & `patroni-3.0.4/patroni/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -531,14 +531,26 @@
         metrics.append("patroni_xlog_replayed_timestamp{0} {1}".format(scope_label, replayed_timestamp))
 
         metrics.append("# HELP patroni_xlog_paused Value is 1 if the Postgres xlog is paused, 0 otherwise.")
         metrics.append("# TYPE patroni_xlog_paused gauge")
         metrics.append("patroni_xlog_paused{0} {1}"
                        .format(scope_label, int(postgres.get('xlog', {}).get('paused', False) is True)))
 
+        if postgres.get('server_version', 0) >= 90600:
+            metrics.append("# HELP patroni_postgres_streaming Value is 1 if Postgres is streaming, 0 otherwise.")
+            metrics.append("# TYPE patroni_postgres_streaming gauge")
+            metrics.append("patroni_postgres_streaming{0} {1}"
+                           .format(scope_label, int(postgres.get('replication_state') == 'streaming')))
+
+            metrics.append("# HELP patroni_postgres_in_archive_recovery Value is 1"
+                           " if Postgres is replicating from archive, 0 otherwise.")
+            metrics.append("# TYPE patroni_postgres_in_archive_recovery gauge")
+            metrics.append("patroni_postgres_in_archive_recovery{0} {1}"
+                           .format(scope_label, int(postgres.get('replication_state') == 'in archive recovery')))
+
         metrics.append("# HELP patroni_postgres_server_version Version of Postgres (if running), 0 otherwise.")
         metrics.append("# TYPE patroni_postgres_server_version gauge")
         metrics.append("patroni_postgres_server_version {0} {1}".format(scope_label, postgres.get('server_version', 0)))
 
         metrics.append("# HELP patroni_cluster_unlocked Value is 1 if the cluster is unlocked, 0 if locked.")
         metrics.append("# TYPE patroni_cluster_unlocked gauge")
         metrics.append("patroni_cluster_unlocked{0} {1}".format(scope_label, int(postgres.get('cluster_unlocked', 0))))
@@ -1147,16 +1159,19 @@
         postgresql = self.server.patroni.postgresql
         cluster = self.server.patroni.dcs.cluster
         global_config = self.server.patroni.config.get_global_config(cluster)
         try:
 
             if postgresql.state not in ('running', 'restarting', 'starting'):
                 raise RetryFailedError('')
+            replication_state = ('(pg_catalog.pg_stat_get_wal_receiver()).status'
+                                 if postgresql.major_version >= 90600 else 'NULL') + ", " +\
+                ("pg_catalog.current_setting('restore_command')" if postgresql.major_version >= 120000 else "NULL")
             stmt = ("SELECT " + postgresql.POSTMASTER_START_TIME + ", " + postgresql.TL_LSN + ","
-                    " pg_catalog.pg_last_xact_replay_timestamp(),"
+                    " pg_catalog.pg_last_xact_replay_timestamp(), " + replication_state + ","
                     " pg_catalog.array_to_json(pg_catalog.array_agg(pg_catalog.row_to_json(ri))) "
                     "FROM (SELECT (SELECT rolname FROM pg_catalog.pg_authid WHERE oid = usesysid) AS usename,"
                     " application_name, client_addr, w.state, sync_state, sync_priority"
                     " FROM pg_catalog.pg_stat_get_wal_senders() w, pg_catalog.pg_stat_get_activity(pid)) AS ri")
 
             row = self.query(stmt.format(postgresql.wal_name, postgresql.lsn_name), retry=retry)[0]
 
@@ -1184,16 +1199,20 @@
             if row[1] > 0:
                 result['timeline'] = row[1]
             else:
                 leader_timeline = None\
                     if not cluster or cluster.is_unlocked() or not cluster.leader else cluster.leader.timeline
                 result['timeline'] = postgresql.replica_cached_timeline(leader_timeline)
 
-            if row[7]:
-                result['replication'] = row[7]
+            replication_state = postgresql.replication_state_from_parameters(row[1] > 0, row[7], row[8])
+            if replication_state:
+                result['replication_state'] = replication_state
+
+            if row[9]:
+                result['replication'] = row[9]
 
         except (psycopg.Error, RetryFailedError, PostgresConnectionException):
             state = postgresql.state
             if state == 'running':
                 logger.exception('get_postgresql_status')
                 state = 'unknown'
             result: Dict[str, Any] = {'state': state, 'role': postgresql.role}
@@ -1537,19 +1556,19 @@
         """Get serial number of the certificate used by the REST API.
 
         :returns: serial number of the certificate configured through ``restapi.certfile`` setting.
         """
         if self.__ssl_options.get('certfile'):
             import ssl
             try:
-                ctx = ssl.SSLContext(ssl.PROTOCOL_TLS_CLIENT)
-                crts = ctx.load_verify_locations(self.__ssl_options['certfile'])
-                if crts:
-                    return crts[0].get('serialNumber')
-            except Exception as e:
+                crt: Dict[str, Any] = ssl._ssl._test_decode_cert(self.__ssl_options['certfile'])  # pyright: ignore
+                if TYPE_CHECKING:  # pragma: no cover
+                    assert isinstance(crt, dict)
+                return crt.get('serialNumber')
+            except ssl.SSLError as e:
                 logger.error('Failed to get serial number from certificate %s: %r', self.__ssl_options['certfile'], e)
 
     def reload_local_certificate(self) -> Optional[bool]:
         """Reload the SSL certificate used by the REST API.
 
         :return: ``True`` if a different certificate has been configured through ``restapi.certfile` setting, ``None``
             otherwise.
```

### Comparing `patroni-3.0.3/patroni/async_executor.py` & `patroni-3.0.4/patroni/async_executor.py`

 * *Files identical despite different names*

### Comparing `patroni-3.0.3/patroni/collections.py` & `patroni-3.0.4/patroni/collections.py`

 * *Files identical despite different names*

### Comparing `patroni-3.0.3/patroni/config.py` & `patroni-3.0.4/patroni/config.py`

 * *Files identical despite different names*

### Comparing `patroni-3.0.3/patroni/ctl.py` & `patroni-3.0.4/patroni/ctl.py`

 * *Files 0% similar despite different names*

```diff
@@ -254,15 +254,15 @@
 option_default_citus_group = click.option('--group', required=False, type=int, help='Citus group',
                                           default=lambda: click.get_current_context().obj.get('citus', {}).get('group'))
 option_citus_group = click.option('--group', required=False, type=int, help='Citus group')
 option_insecure = click.option('-k', '--insecure', is_flag=True, help='Allow connections to SSL sites without certs')
 role_choice = click.Choice(['leader', 'primary', 'standby-leader', 'replica', 'standby', 'any', 'master'])
 
 
-@click.group()
+@click.group(cls=click.Group)
 @click.option('--config-file', '-c', help='Configuration file',
               envvar='PATRONICTL_CONFIG_FILE', default=CONFIG_FILE_PATH)
 @click.option('--dcs-url', '--dcs', '-d', 'dcs_url', help='The DCS connect url', envvar='DCS_URL')
 @option_insecure
 @click.pass_context
 def ctl(ctx: click.Context, config_file: str, dcs_url: Optional[str], insecure: bool) -> None:
     """Entry point of ``patronictl`` utility.
@@ -1486,15 +1486,16 @@
 
         * ``Cluster``: name of the Patroni cluster, as per ``scope`` configuration;
         * ``Member``: name of the Patroni node, as per ``name`` configuration;
         * ``Host``: hostname (or IP) and port, as per ``postgresql.listen`` configuration;
         * ``Role``: ``Leader``, ``Standby Leader``, ``Sync Standby`` or ``Replica``;
         * ``State``: ``stopping``, ``stopped``, ``stop failed``, ``crashed``, ``running``, ``starting``,
           ``start failed``, ``restarting``, ``restart failed``, ``initializing new cluster``, ``initdb failed``,
-          ``running custom bootstrap script``, ``custom bootstrap failed``, or ``creating replica``, and so on;
+          ``running custom bootstrap script``, ``custom bootstrap failed``, ``creating replica``, ``streaming``,
+          ``in archive recovery``, and so on;
         * ``TL``: current timeline in Postgres;
           ``Lag in MB``: replication lag.
 
     Besides that it may also have:
         * ``Group``: Citus group ID -- showed only if Citus is enabled.
         * ``Pending restart``: if the node is pending a restart -- showed only if *extended*;
         * ``Scheduled restart``: timestamp for scheduled restart, if any -- showed only if *extended*;
```

### Comparing `patroni-3.0.3/patroni/daemon.py` & `patroni-3.0.4/patroni/daemon.py`

 * *Files identical despite different names*

### Comparing `patroni-3.0.3/patroni/dcs/__init__.py` & `patroni-3.0.4/patroni/dcs/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -235,31 +235,34 @@
             try:
                 return tuple(map(int, version.split('.')))
             except Exception:
                 logger.debug('Failed to parse Patroni version %s', version)
 
 
 class RemoteMember(Member):
-    """Represents a remote member (typically a primary) for a standby cluster"""
+    """Represents a remote member (typically a primary) for a standby cluster.
+
+    :cvar ALLOWED_KEYS: Controls access to relevant key names that could be in stored :attr:`~RemoteMember.data`.
+    """
+
+    ALLOWED_KEYS: Tuple[str, ...] = (
+        'primary_slot_name',
+        'create_replica_methods',
+        'restore_command',
+        'archive_cleanup_command',
+        'recovery_min_apply_delay',
+        'no_replication_slot'
+    )
 
     @classmethod
     def from_name_and_data(cls, name: str, data: Dict[str, Any]) -> 'RemoteMember':
         return super(RemoteMember, cls).__new__(cls, -1, name, None, data)
 
-    @staticmethod
-    def allowed_keys() -> Tuple[str, ...]:
-        return ('primary_slot_name',
-                'create_replica_methods',
-                'restore_command',
-                'archive_cleanup_command',
-                'recovery_min_apply_delay',
-                'no_replication_slot')
-
     def __getattr__(self, name: str) -> Any:
-        if name in RemoteMember.allowed_keys():
+        if name in RemoteMember.ALLOWED_KEYS:
             return self.data.get(name)
 
 
 class Leader(NamedTuple):
     """Immutable object (namedtuple) which represents leader key.
 
     Consists of the following fields:
```

### Comparing `patroni-3.0.3/patroni/dcs/consul.py` & `patroni-3.0.4/patroni/dcs/consul.py`

 * *Files 1% similar despite different names*

```diff
@@ -396,27 +396,31 @@
         try:
             failsafe = json.loads(failsafe['Value']) if failsafe else None
         except Exception:
             failsafe = None
 
         return Cluster(initialize, config, leader, last_lsn, members, failover, sync, history, slots, failsafe)
 
+    @property
+    def _consistency(self) -> str:
+        return 'consistent' if self._ctl else self._client.consistency
+
     def _cluster_loader(self, path: str) -> Cluster:
-        _, results = self.retry(self._client.kv.get, path, recurse=True)
+        _, results = self.retry(self._client.kv.get, path, recurse=True, consistency=self._consistency)
         if results is None:
             raise NotFound
         nodes = {}
         for node in results:
             node['Value'] = (node['Value'] or b'').decode('utf-8')
             nodes[node['Key'][len(path):]] = node
 
         return self._cluster_from_nodes(nodes)
 
     def _citus_cluster_loader(self, path: str) -> Dict[int, Cluster]:
-        _, results = self.retry(self._client.kv.get, path, recurse=True)
+        _, results = self.retry(self._client.kv.get, path, recurse=True, consistency=self._consistency)
         clusters: Dict[int, Dict[str, Cluster]] = defaultdict(dict)
         for node in results or []:
             key = node['Key'][len(path):].split('/', 1)
             if len(key) == 2 and citus_group_re.match(key[0]):
                 node['Value'] = (node['Value'] or b'').decode('utf-8')
                 clusters[int(key[0])][key[1]] = node
         return {group: self._cluster_from_nodes(nodes) for group, nodes in clusters.items()}
```

### Comparing `patroni-3.0.3/patroni/dcs/etcd.py` & `patroni-3.0.4/patroni/dcs/etcd.py`

 * *Files 0% similar despite different names*

```diff
@@ -95,15 +95,15 @@
 
     ERROR_CLS: Type[Exception]
 
     def __init__(self, config: Dict[str, Any], dns_resolver: DnsCachingResolver, cache_ttl: int = 300) -> None:
         self._dns_resolver = dns_resolver
         self.set_machines_cache_ttl(cache_ttl)
         self._machines_cache_updated = 0
-        kwargs = {p: config.get(p) for p in ('host', 'port', 'protocol', 'use_proxies',
+        kwargs = {p: config.get(p) for p in ('host', 'port', 'protocol', 'use_proxies', 'version_prefix',
                                              'username', 'password', 'cert', 'ca_cert') if config.get(p)}
         super(AbstractEtcdClientWithFailover, self).__init__(read_timeout=config['retry_timeout'], **kwargs)
         # For some reason python3-etcd on debian and ubuntu are not based on the latest version
         # Workaround for the case when https://github.com/jplana/python-etcd/pull/196 is not applied
         self.http.connection_pool_kw.pop('ssl_version', None)
         self._config = config
         self._load_machines_cache()
@@ -439,14 +439,17 @@
             self._base_uri = value
 
 
 class EtcdClient(AbstractEtcdClientWithFailover):
 
     ERROR_CLS = EtcdError
 
+    def __init__(self, config: Dict[str, Any], dns_resolver: DnsCachingResolver, cache_ttl: int = 300) -> None:
+        super(EtcdClient, self).__init__({**config, 'version_prefix': None}, dns_resolver, cache_ttl)
+
     def __del__(self) -> None:
         try:
             self.http.clear()
         except (ReferenceError, TypeError, AttributeError):
             pass
 
     def _prepare_get_members(self, etcd_nodes: int) -> Dict[str, Any]:
@@ -718,21 +721,21 @@
             failsafe = json.loads(failsafe.value) if failsafe else None
         except Exception:
             failsafe = None
 
         return Cluster(initialize, config, leader, last_lsn, members, failover, sync, history, slots, failsafe)
 
     def _cluster_loader(self, path: str) -> Cluster:
-        result = self.retry(self._client.read, path, recursive=True)
+        result = self.retry(self._client.read, path, recursive=True, quorum=self._ctl)
         nodes = {node.key[len(result.key):].lstrip('/'): node for node in result.leaves}
         return self._cluster_from_nodes(result.etcd_index, nodes)
 
     def _citus_cluster_loader(self, path: str) -> Dict[int, Cluster]:
         clusters: Dict[int, Dict[str, etcd.EtcdResult]] = defaultdict(dict)
-        result = self.retry(self._client.read, path, recursive=True)
+        result = self.retry(self._client.read, path, recursive=True, quorum=self._ctl)
         for node in result.leaves:
             key = node.key[len(result.key):].lstrip('/').split('/', 1)
             if len(key) == 2 and citus_group_re.match(key[0]):
                 clusters[int(key[0])][key[1]] = node
         return {group: self._cluster_from_nodes(result.etcd_index, nodes) for group, nodes in clusters.items()}
 
     def _load_cluster(
```

### Comparing `patroni-3.0.3/patroni/dcs/etcd3.py` & `patroni-3.0.4/patroni/dcs/etcd3.py`

 * *Files 1% similar despite different names*

```diff
@@ -202,16 +202,15 @@
 class Etcd3Client(AbstractEtcdClientWithFailover):
 
     ERROR_CLS = Etcd3Error
 
     def __init__(self, config: Dict[str, Any], dns_resolver: DnsCachingResolver, cache_ttl: int = 300) -> None:
         self._token = None
         self._cluster_version: Tuple[int] = tuple()
-        self.version_prefix = '/v3beta'
-        super(Etcd3Client, self).__init__(config, dns_resolver, cache_ttl)
+        super(Etcd3Client, self).__init__({**config, 'version_prefix': '/v3beta'}, dns_resolver, cache_ttl)
 
         try:
             self.authenticate()
         except AuthFailed as e:
             logger.fatal('Etcd3 authentication failed: %r', e)
             sys.exit(1)
 
@@ -323,22 +322,22 @@
                                              '{0}'.format('.'.join(map(str, self._cluster_version))))
             return retry(e)
         except InvalidAuthToken as e:
             logger.error('Invalid auth token: %s', self._token)
             return retry(e)
 
     @_handle_auth_errors
-    def range(self, key: str, range_end: Union[bytes, str, None] = None,
+    def range(self, key: str, range_end: Union[bytes, str, None] = None, serializable: bool = True,
               retry: Optional[Retry] = None) -> Dict[str, Any]:
         params = build_range_request(key, range_end)
-        params['serializable'] = True  # For better performance. We can tolerate stale reads.
+        params['serializable'] = serializable  # For better performance. We can tolerate stale reads
         return self.call_rpc('/kv/range', params, retry)
 
-    def prefix(self, key: str, retry: Optional[Retry] = None) -> Dict[str, Any]:
-        return self.range(key, prefix_range_end(key), retry)
+    def prefix(self, key: str, serializable: bool = True, retry: Optional[Retry] = None) -> Dict[str, Any]:
+        return self.range(key, prefix_range_end(key), serializable, retry)
 
     @_handle_auth_errors
     def lease_grant(self, ttl: int, retry: Optional[Retry] = None) -> str:
         return self.call_rpc('/lease/grant', {'TTL': ttl}, retry)['ID']
 
     def lease_keepalive(self, ID: str, retry: Optional[Retry] = None) -> Optional[str]:
         return self.call_rpc('/lease/keepalive', {'ID': ID}, retry).get('result', {}).get('TTL')
@@ -591,15 +590,16 @@
 
     def get_cluster(self, path: str) -> List[Dict[str, Any]]:
         if self._kv_cache and path.startswith(self._etcd3.cluster_prefix):
             with self._kv_cache.condition:
                 self._wait_cache(self.read_timeout)
                 ret = self._kv_cache.copy()
         else:
-            ret = self._etcd3.retry(self.prefix, path).get('kvs', [])
+            serializable = not getattr(self._etcd3, '_ctl')  # use linearizable for patronictl
+            ret = self._etcd3.retry(self.prefix, path, serializable).get('kvs', [])
         for node in ret:
             node.update({'key': base64_decode(node['key']),
                          'value': base64_decode(node.get('value', '')),
                          'lease': node.get('lease')})
         return ret
 
     def call_rpc(self, method: str, fields: Dict[str, Any], retry: Optional[Retry] = None) -> Dict[str, Any]:
```

### Comparing `patroni-3.0.3/patroni/dcs/exhibitor.py` & `patroni-3.0.4/patroni/dcs/exhibitor.py`

 * *Files identical despite different names*

### Comparing `patroni-3.0.3/patroni/dcs/kubernetes.py` & `patroni-3.0.4/patroni/dcs/kubernetes.py`

 * *Files 0% similar despite different names*

```diff
@@ -762,23 +762,23 @@
         self._ttl = int(config.get('ttl') or 30)
         try:
             k8s_config.load_incluster_config(ca_certs=self._ca_certs)
         except k8s_config.ConfigException:
             k8s_config.load_kube_config(context=config.get('context', 'kind-kind'))
 
         pod_ip = config.get('pod_ip')
-        self.__ips: List[str] = [] if config.get('patronictl') or not isinstance(pod_ip, str) else [pod_ip]
+        self.__ips: List[str] = [] if self._ctl or not isinstance(pod_ip, str) else [pod_ip]
         self.__ports: List[K8sObject] = []
         ports: List[Dict[str, Any]] = config.get('ports', [{}])
         for p in ports:
             port: Dict[str, Any] = {'port': int(p.get('port', '5432'))}
             port.update({n: p[n] for n in ('name', 'protocol') if p.get(n)})
             self.__ports.append(k8s_client.V1EndpointPort(**port))
 
-        bypass_api_service = not config.get('patronictl') and config.get('bypass_api_service')
+        bypass_api_service = not self._ctl and config.get('bypass_api_service')
         self._api = CoreV1ApiProxy(config.get('use_endpoints'), bypass_api_service)
         self._should_create_config_service = self._api.use_endpoints
         self.reload_config(config)
         # leader_observed_record, leader_resource_version, and leader_observed_time are used only for leader race!
         self._leader_observed_record: Dict[str, str] = {}
         self._leader_observed_time = None
         self._leader_resource_version = None
```

### Comparing `patroni-3.0.3/patroni/dcs/raft.py` & `patroni-3.0.4/patroni/dcs/raft.py`

 * *Files identical despite different names*

### Comparing `patroni-3.0.3/patroni/dcs/zookeeper.py` & `patroni-3.0.4/patroni/dcs/zookeeper.py`

 * *Files identical despite different names*

### Comparing `patroni-3.0.3/patroni/exceptions.py` & `patroni-3.0.4/patroni/exceptions.py`

 * *Files identical despite different names*

### Comparing `patroni-3.0.3/patroni/ha.py` & `patroni-3.0.4/patroni/ha.py`

 * *Files 1% similar despite different names*

```diff
@@ -145,15 +145,14 @@
         self._is_leader = False
         self._is_leader_lock = RLock()
         self._failsafe = Failsafe(patroni.dcs)
         self._was_paused = False
         self._leader_timeline = None
         self.recovering = False
         self._async_response = CriticalTask()
-        self._crash_recovery_executed = False
         self._crash_recovery_started = 0
         self._start_timeout = None
         self._async_executor = AsyncExecutor(self.state_handler.cancellable, self.wakeup)
         self.watchdog = patroni.watchdog
 
         # Each member publishes various pieces of information to the DCS using touch_member. This lock protects
         # the state and publishing procedure to have consistent ordering and avoid publishing stale values.
@@ -303,18 +302,21 @@
             if tags:
                 data['tags'] = tags
             if self.state_handler.pending_restart:
                 data['pending_restart'] = True
             if self._async_executor.scheduled_action in (None, 'promote') \
                     and data['state'] in ['running', 'restarting', 'starting']:
                 try:
-                    timeline: Optional[int]
                     timeline, wal_position, pg_control_timeline = self.state_handler.timeline_wal_position()
                     data['xlog_location'] = wal_position
-                    if not timeline:  # try pg_stat_wal_receiver to get the timeline
+                    if not timeline:  # running as a standby
+                        replication_state = self.state_handler.replication_state()
+                        if replication_state:
+                            data['replication_state'] = replication_state
+                        # try pg_stat_wal_receiver to get the timeline
                         timeline = self.state_handler.received_timeline()
                     if not timeline:
                         # So far the only way to get the current timeline on the standby is from
                         # the replication connection. In order to avoid opening the replication
                         # connection on every iteration of HA loop we will do it only when noticed
                         # that the timeline on the primary has changed.
                         # Unfortunately such optimization isn't possible on the standby_leader,
@@ -407,16 +409,15 @@
             self._async_response.complete(result)
         if result:
             self.state_handler.set_role('standby_leader')
 
         return result
 
     def _handle_crash_recovery(self) -> Optional[str]:
-        if not self._crash_recovery_executed and (self.cluster.is_unlocked() or self._rewind.can_rewind):
-            self._crash_recovery_executed = True
+        if self._crash_recovery_started == 0 and (self.cluster.is_unlocked() or self._rewind.can_rewind):
             self._crash_recovery_started = time.time()
             msg = 'doing crash recovery in a single user mode'
             return self._async_executor.try_run_async(msg, self._rewind.ensure_clean_shutdown) or msg
 
     def _handle_rewind_or_reinitialize(self) -> Optional[str]:
         leader = self.get_remote_member() if self.is_standby_cluster() else self.cluster.leader
         if not self._rewind.rewind_or_reinitialize_needed_and_possible(leader) or not leader:
@@ -434,31 +435,62 @@
             return self._async_executor.try_run_async(msg, self._rewind.execute, args=(leader,)) or msg
 
         if self._rewind.should_remove_data_directory_on_diverged_timelines and not self.is_standby_cluster():
             msg = 'reinitializing due to diverged timelines'
             return self._async_executor.try_run_async(msg, self._do_reinitialize, args=(self.cluster,)) or msg
 
     def recover(self) -> str:
-        # Postgres is not running and we will restart in standby mode. Watchdog is not needed until we promote.
-        self.watchdog.disable()
+        """Handle the case when postgres isn't running.
+
+        Depending on the state of Patroni, DCS cluster view, and pg_controldata the following could happen:
+        - if ``primary_start_timeout`` is 0 and this node owns the leader lock, the lock
+          will be voluntarily released if there are healthy replicas to take it over.
+        - if postgres was running as a ``primary`` and this node owns the leader lock, postgres is started as primary.
+        - crash recover in a single-user mode is executed in the following cases:
+          - postgres was running as ``primary`` wasn't ``shut down`` cleanly and there is no leader in DCS
+          - postgres was running as ``replica`` wasn't ``shut down in recovery`` (cleanly)
+            and we need to run ``pg_rewind`` to join back to the cluster.
+        - ``pg_rewind`` is executed if it is necessary, or optinally, the data directory could
+           be removed if it is allowed by configuration.
+        - after ``crash recovery`` and/or ``pg_rewind`` are executed, postgres is started in recovery.
 
+        :returns: action message, describing what was performed.
+        """
         if self.has_lock() and self.update_lock():
             timeout = self.global_config.primary_start_timeout
             if timeout == 0:
                 # We are requested to prefer failing over to restarting primary. But see first if there
                 # is anyone to fail over to.
                 if self.is_failover_possible(self.cluster.members):
+                    self.watchdog.disable()
                     logger.info("Primary crashed. Failing over.")
                     self.demote('immediate')
                     return 'stopped PostgreSQL to fail over after a crash'
         else:
             timeout = None
 
         data = self.state_handler.controldata()
         logger.info('pg_controldata:\n%s\n', '\n'.join('  {0}: {1}'.format(k, v) for k, v in data.items()))
+
+        # timeout > 0 indicates that we still have the leader lock, and it was just updated
+        if timeout\
+                and data.get('Database cluster state') in ('in production', 'shutting down', 'shut down')\
+                and self.state_handler.state == 'crashed'\
+                and self.state_handler.role in ('primary', 'master')\
+                and not self.state_handler.config.recovery_conf_exists():
+            # We know 100% that we were running as a primary a few moments ago, therefore could just start postgres
+            msg = 'starting primary after failure'
+            if self._async_executor.try_run_async(msg, self.state_handler.start,
+                                                  args=(timeout, self._async_executor.critical_task)) is None:
+                self.recovering = True
+                return msg
+
+        # Postgres is not running, and we will restart in standby mode. Watchdog is not needed until we promote.
+        self.watchdog.disable()
+
         if data.get('Database cluster state') in ('in production', 'shutting down', 'in crash recovery'):
             msg = self._handle_crash_recovery()
             if msg:
                 return msg
 
         self.load_cluster_from_dcs()
 
@@ -961,17 +993,14 @@
 
         if self.is_paused() and not self.patroni.nofailover and \
                 self.cluster.failover and not self.cluster.failover.scheduled_at:
             ret = self.manual_failover_process_no_leader()
             if ret is not None:  # continue if we just deleted the stale failover key as a leader
                 return ret
 
-        if self.state_handler.is_starting():  # postgresql still starting up is unhealthy
-            return False
-
         if self.state_handler.is_leader():
             # in pause leader is the healthiest only when no initialize or sysid matches with initialize!
             return not self.is_paused() or not self.cluster.initialize\
                 or self.state_handler.sysid == self.cluster.initialize
 
         if self.is_paused():
             return False
@@ -1447,15 +1476,15 @@
                     cancel = self._async_response.cancel()
                 if cancel:
                     self.state_handler.cancellable.cancel()
                     return 'lost leader before promote'
 
             if self.state_handler.role in ('master', 'primary'):
                 logger.info('Demoting primary during %s', self._async_executor.scheduled_action)
-                if self._async_executor.scheduled_action == 'restart':
+                if self._async_executor.scheduled_action in ('restart', 'starting primary after failure'):
                     # Restart needs a special interlocking cancel because postmaster may be just started in a
                     # background thread and has not even written a pid file yet.
                     with self._async_executor.critical_task as task:
                         if not task.cancel() and isinstance(task.result, PostmasterProcess):
                             self.state_handler.terminate_starting_postmaster(postmaster=task.result)
                 self.demote('immediate-nolock')
                 return 'lost leader lock during {0}'.format(self._async_executor.scheduled_action)
@@ -1511,14 +1540,17 @@
             self.cancel_initialization()
 
         self._rewind.ensure_checkpoint_after_promote(self.wakeup)
         self.dcs.initialize(create_new=(self.cluster.initialize is None), sysid=self.state_handler.sysid)
         self.dcs.set_config_value(json.dumps(self.patroni.config.dynamic_configuration, separators=(',', ':')))
         self.dcs.take_leader()
         self.set_is_leader(True)
+        if self.is_synchronous_mode():
+            self.state_handler.sync_handler.set_synchronous_standby_names(
+                CaseInsensitiveSet('*') if self.global_config.is_synchronous_mode_strict else CaseInsensitiveSet())
         self.state_handler.call_nowait(CallbackAction.ON_START)
         self.load_cluster_from_dcs()
 
         return 'initialized a new cluster'
 
     def handle_starting_instance(self) -> Optional[str]:
         """Starting up PostgreSQL may take a long time. In case we are the leader we may want to
@@ -1612,15 +1644,15 @@
                 if not self._rewind.is_needed:
                     # Check if we tried to recover from postgres crash and failed
                     msg = self.post_recover()
                     if msg is not None:
                         return msg
 
                 # Reset some states after postgres successfully started up
-                self._crash_recovery_executed = False
+                self._crash_recovery_started = 0
                 if self._rewind.executed and not self._rewind.failed:
                     self._rewind.reset_state()
 
                 # The Raft cluster without a quorum takes a bit of time to stabilize.
                 # Therefore we want to postpone the leader race if we just started up.
                 if self.cluster.is_unlocked() and self.dcs.__class__.__name__ == 'Raft':
                     return 'started as a secondary'
@@ -1704,24 +1736,29 @@
 
             if self.cluster.is_unlocked():
                 ret = self.process_unhealthy_cluster()
             else:
                 msg = self.process_healthy_cluster()
                 ret = self.evaluate_scheduled_restart() or msg
 
-            # we might not have a valid PostgreSQL connection here if another thread
-            # stops PostgreSQL, therefore, we only reload replication slots if no
-            # asynchronous processes are running (should be always the case for the primary)
-            if not self._async_executor.busy and not self.state_handler.is_starting():
+            # We might not have a valid PostgreSQL connection here if AsyncExecutor is doing
+            # something with PostgreSQL. Therefore we will sync replication slots only if no
+            # asynchronous processes are running or we know that this is a standby being promoted.
+            # But, we don't want to run pg_rewind checks or copy logical slots from itself,
+            # therefore we have a couple additional `not is_promoting` checks.
+            is_promoting = self._async_executor.scheduled_action == 'promote'
+            if (not self._async_executor.busy or is_promoting) and not self.state_handler.is_starting():
                 create_slots = self._sync_replication_slots(False)
+
                 if not self.state_handler.cb_called:
-                    if not self.state_handler.is_leader():
+                    if not is_promoting and not self.state_handler.is_leader():
                         self._rewind.trigger_check_diverged_lsn()
                     self.state_handler.call_nowait(CallbackAction.ON_START)
-                if create_slots and self.cluster.leader:
+
+                if not is_promoting and create_slots and self.cluster.leader:
                     err = self._async_executor.try_run_async('copy_logical_slots',
                                                              self.state_handler.slots_handler.copy_logical_slots,
                                                              args=(self.cluster, create_slots))
                     if not err:
                         ret = 'Copying logical slots {0} from the primary'.format(create_slots)
             return ret
         except DCSError:
@@ -1858,15 +1895,15 @@
             member to stream. Config can be both patroni config or
             cluster.config.data
         """
         data: Dict[str, Any] = {}
         cluster_params = self.global_config.get_standby_cluster_config()
 
         if cluster_params:
-            data.update({k: v for k, v in cluster_params.items() if k in RemoteMember.allowed_keys()})
+            data.update({k: v for k, v in cluster_params.items() if k in RemoteMember.ALLOWED_KEYS})
             data['no_replication_slot'] = 'primary_slot_name' not in cluster_params
             conn_kwargs = member.conn_kwargs() if member else \
                 {k: cluster_params[k] for k in ('host', 'port') if k in cluster_params}
             if conn_kwargs:
                 data['conn_kwargs'] = conn_kwargs
 
         name = member.name if member else 'remote_member:{}'.format(uuid.uuid1())
```

### Comparing `patroni-3.0.3/patroni/log.py` & `patroni-3.0.4/patroni/log.py`

 * *Files identical despite different names*

### Comparing `patroni-3.0.3/patroni/postgresql/__init__.py` & `patroni-3.0.4/patroni/postgresql/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -193,26 +193,27 @@
                          "FROM pg_catalog.pg_stat_get_wal_senders() w,"
                          " pg_catalog.pg_stat_get_activity(w.pid)"
                          " WHERE w.state = 'streaming') r)").format(self.wal_name, self.lsn_name)
                         if (not self.global_config or self.global_config.is_synchronous_mode)
                         and self.role in ('master', 'primary', 'promoted') else "'on', '', NULL")
 
         if self._major_version >= 90600:
-            extra = ("(SELECT pg_catalog.json_agg(s.*) FROM (SELECT slot_name, slot_type as type, datoid::bigint, "
-                     "plugin, catalog_xmin, pg_catalog.pg_wal_lsn_diff(confirmed_flush_lsn, '0/0')::bigint"
-                     " AS confirmed_flush_lsn FROM pg_catalog.pg_get_replication_slots()) AS s)"
-                     if self._has_permanent_logical_slots and self._major_version >= 110000 else "NULL") + extra
+            extra = ("pg_catalog.current_setting('restore_command')" if self._major_version >= 120000 else "NULL") +\
+                ", " + ("(SELECT pg_catalog.json_agg(s.*) FROM (SELECT slot_name, slot_type as type, datoid::bigint, "
+                        "plugin, catalog_xmin, pg_catalog.pg_wal_lsn_diff(confirmed_flush_lsn, '0/0')::bigint"
+                        " AS confirmed_flush_lsn FROM pg_catalog.pg_get_replication_slots()) AS s)"
+                        if self._has_permanent_logical_slots and self._major_version >= 110000 else "NULL") + extra
             extra = (", CASE WHEN latest_end_lsn IS NULL THEN NULL ELSE received_tli END,"
-                     " slot_name, conninfo, {0} FROM pg_catalog.pg_stat_get_wal_receiver()").format(extra)
+                     " slot_name, conninfo, status, {0} FROM pg_catalog.pg_stat_get_wal_receiver()").format(extra)
             if self.role == 'standby_leader':
                 extra = "timeline_id" + extra + ", pg_catalog.pg_control_checkpoint()"
             else:
                 extra = "0" + extra
         else:
-            extra = "0, NULL, NULL, NULL, NULL" + extra
+            extra = "0, NULL, NULL, NULL, NULL, NULL, NULL" + extra
 
         return ("SELECT " + self.TL_LSN + ", {2}").format(self.wal_name, self.lsn_name, extra)
 
     @property
     def available_gucs(self) -> CaseInsensitiveSet:
         """GUCs available in this Postgres server."""
         return self._get_gucs()
@@ -422,15 +423,16 @@
 
     def _cluster_info_state_get(self, name: str) -> Optional[Any]:
         if not self._cluster_info_state:
             try:
                 result = self._is_leader_retry(self._query, self.cluster_info_query).fetchone()
                 cluster_info_state = dict(zip(['timeline', 'wal_position', 'replayed_location',
                                                'received_location', 'replay_paused', 'pg_control_timeline',
-                                               'received_tli', 'slot_name', 'conninfo', 'slots', 'synchronous_commit',
+                                               'received_tli', 'slot_name', 'conninfo', 'receiver_state',
+                                               'restore_command', 'slots', 'synchronous_commit',
                                                'synchronous_standby_names', 'pg_stat_replication'], result))
                 if self._has_permanent_logical_slots:
                     cluster_info_state['slots'] =\
                         self.slots_handler.process_permanent_slots(cluster_info_state['slots'])
                 self._cluster_info_state = cluster_info_state
             except RetryFailedError as e:  # SELECT failed two times
                 self._cluster_info_state = {'error': str(e)}
@@ -468,14 +470,49 @@
         """:returns: "synchronous_standby_names" GUC value."""
         return self._cluster_info_state_get('synchronous_standby_names') or ''
 
     def pg_stat_replication(self) -> List[Dict[str, Any]]:
         """:returns: a result set of 'SELECT * FROM pg_stat_replication'."""
         return self._cluster_info_state_get('pg_stat_replication') or []
 
+    def replication_state_from_parameters(self, is_leader: bool, receiver_state: Optional[str],
+                                          restore_command: Optional[str]) -> Optional[str]:
+        """Figure out the replication state from input parameters.
+
+        .. note::
+            This method could be only called when Postgres is up, running and queries are successfuly executed.
+
+        :is_leader: `True` is postgres is not running in recovery
+        :receiver_state: value from `pg_stat_get_wal_receiver.state` or None if Postgres is older than 9.6
+        :restore_command: value of ``restore_command`` GUC for PostgreSQL 12+ or
+                          `postgresql.recovery_conf.restore_command` if it is set in Patroni configuration
+
+        :returns: - `None` for the primary and for Postgres older than 9.6;
+                  - 'streaming' if replica is streaming according to the `pg_stat_wal_receiver` view;
+                  - 'in archive recovery' if replica isn't streaming and there is a `restore_command`
+        """
+        if self._major_version >= 90600 and not is_leader:
+            if receiver_state == 'streaming':
+                return 'streaming'
+            # For Postgres older than 12 we get `restore_command` from Patroni config, otherwise we check GUC
+            if self._major_version < 120000 and self.config.restore_command() or restore_command:
+                return 'in archive recovery'
+
+    def replication_state(self) -> Optional[str]:
+        """Checks replication state from `pg_stat_get_wal_receiver()`.
+
+        .. note::
+            Available only since 9.6
+
+        :returns: ``streaming``, ``in archive recovery``, or ``None``
+        """
+        return self.replication_state_from_parameters(self.is_leader(),
+                                                      self._cluster_info_state_get('receiver_state'),
+                                                      self._cluster_info_state_get('restore_command'))
+
     def is_leader(self) -> bool:
         try:
             return bool(self._cluster_info_state_get('timeline'))
         except PostgresConnectionException:
             logger.warning('Failed to determine PostgreSQL state from the connection, falling back to cached role')
             return bool(self.is_running() and self.role in ('master', 'primary'))
```

### Comparing `patroni-3.0.3/patroni/postgresql/available_parameters/0_postgres.yml` & `patroni-3.0.4/patroni/postgresql/available_parameters/0_postgres.yml`

 * *Files identical despite different names*

### Comparing `patroni-3.0.3/patroni/postgresql/bootstrap.py` & `patroni-3.0.4/patroni/postgresql/bootstrap.py`

 * *Files 1% similar despite different names*

```diff
@@ -181,15 +181,15 @@
             if 'host' not in r:
                 # https://www.postgresql.org/docs/current/static/libpq-pgpass.html
                 # A host name of localhost matches both TCP (host name localhost) and Unix domain socket
                 # (pghost empty or the default socket directory) connections coming from the local machine.
                 r['host'] = 'localhost'  # set it to localhost to write into pgpass
 
             env = self._postgresql.config.write_pgpass(r)
-            env['PGOPTIONS'] = '-c synchronous_commit=local'
+            env['PGOPTIONS'] = '-c synchronous_commit=local -c statement_timeout=0'
 
             try:
                 ret = self._postgresql.cancellable.call(shlex.split(cmd) + [connstring], env=env)
             except OSError:
                 logger.error('post_init script %s failed', cmd)
                 return False
             if ret != 0:
```

### Comparing `patroni-3.0.3/patroni/postgresql/callback_executor.py` & `patroni-3.0.4/patroni/postgresql/callback_executor.py`

 * *Files identical despite different names*

### Comparing `patroni-3.0.3/patroni/postgresql/cancellable.py` & `patroni-3.0.4/patroni/postgresql/cancellable.py`

 * *Files identical despite different names*

### Comparing `patroni-3.0.3/patroni/postgresql/citus.py` & `patroni-3.0.4/patroni/postgresql/citus.py`

 * *Files identical despite different names*

### Comparing `patroni-3.0.3/patroni/postgresql/config.py` & `patroni-3.0.4/patroni/postgresql/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -1173,7 +1173,10 @@
 
     @property
     def postgresql_conf(self) -> str:
         return self._postgresql_conf
 
     def get(self, key: str, default: Optional[Any] = None) -> Optional[Any]:
         return self._config.get(key, default)
+
+    def restore_command(self) -> Optional[str]:
+        return (self.get('recovery_conf') or {}).get('restore_command')
```

### Comparing `patroni-3.0.3/patroni/postgresql/connection.py` & `patroni-3.0.4/patroni/postgresql/connection.py`

 * *Files identical despite different names*

### Comparing `patroni-3.0.3/patroni/postgresql/misc.py` & `patroni-3.0.4/patroni/postgresql/misc.py`

 * *Files identical despite different names*

### Comparing `patroni-3.0.3/patroni/postgresql/postmaster.py` & `patroni-3.0.4/patroni/postgresql/postmaster.py`

 * *Files identical despite different names*

### Comparing `patroni-3.0.3/patroni/postgresql/rewind.py` & `patroni-3.0.4/patroni/postgresql/rewind.py`

 * *Files identical despite different names*

### Comparing `patroni-3.0.3/patroni/postgresql/slots.py` & `patroni-3.0.4/patroni/postgresql/slots.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,16 +17,32 @@
     from psycopg2 import cursor
     from . import Postgresql
 
 logger = logging.getLogger(__name__)
 
 
 def compare_slots(s1: Dict[str, Any], s2: Dict[str, Any], dbid: str = 'database') -> bool:
-    return s1['type'] == s2['type'] and (s1['type'] == 'physical'
-                                         or s1.get(dbid) == s2.get(dbid) and s1['plugin'] == s2['plugin'])
+    """Compare 2 replication slot objects for equality.
+
+    ..note ::
+        If the first argument is a ``physical`` replication slot then only the `type` of the second slot is compared.
+        If the first argument is another ``type`` (e.g. ``logical``) then *dbid* and ``plugin`` are compared.
+
+    :param s1: First slot dictionary to be compared.
+    :param s2: Second slot dictionary to be compared.
+    :param dbid: Optional attribute to be compared when comparing ``logical`` replication slots.
+
+    :return: ``True`` if the slot ``type`` of *s1* and *s2* is matches, and the ``type`` of *s1* is ``physical``,
+             OR the ``types`` match AND the *dbid* and ``plugin`` attributes are equal.
+
+    """
+    return (s1['type'] == s2['type']
+            and (s1['type'] == 'physical'
+                 or s1.get(dbid) == s2.get(dbid)
+                 and s1['plugin'] == s2['plugin']))
 
 
 class SlotsAdvanceThread(Thread):
 
     def __init__(self, slots_handler: 'SlotsHandler') -> None:
         super(SlotsAdvanceThread, self).__init__()
         self.daemon = True
```

### Comparing `patroni-3.0.3/patroni/postgresql/sync.py` & `patroni-3.0.4/patroni/postgresql/sync.py`

 * *Files 1% similar despite different names*

```diff
@@ -189,15 +189,20 @@
         # Invalidate cache of "sync" connections
         for app_name in list(self._ready_replicas.keys()):
             if app_name not in self._ssn_data.members:
                 del self._ready_replicas[app_name]
 
         # Newly connected replicas will be counted as sync only when reached self._primary_flush_lsn
         self._primary_flush_lsn = self._postgresql.last_operation()
-        self._postgresql.query('SELECT pg_catalog.txid_current()')  # Ensure some WAL traffic to move replication
+        # Ensure some WAL traffic to move replication
+        self._postgresql.query("""DO $$
+BEGIN
+    SET local synchronous_commit = 'off';
+    PERFORM * FROM pg_catalog.txid_current();
+END;$$""")
         self._postgresql.reset_cluster_info_state(None)  # Reset internal cache to query fresh values
 
     def current_state(self, cluster: Cluster) -> Tuple[CaseInsensitiveSet, CaseInsensitiveSet]:
         """Finds best candidates to be the synchronous standbys.
 
         Current synchronous standby is always preferred, unless it has disconnected or does not want to be a
         synchronous standby any longer.
@@ -285,10 +290,10 @@
             return
 
         time.sleep(0.1)  # Usualy it takes 1ms to reload postgresql.conf, but we will give it 100ms
 
         # Reset internal cache to query fresh values
         self._postgresql.reset_cluster_info_state(None)
 
-        # timeline == 0 -- indicates that this is the replica, shoudn't ever happen
+        # timeline == 0 -- indicates that this is the replica
         if self._postgresql.get_primary_timeline() > 0:
             self._handle_synchronous_standby_names_change()
```

### Comparing `patroni-3.0.3/patroni/postgresql/validator.py` & `patroni-3.0.4/patroni/postgresql/validator.py`

 * *Files identical despite different names*

### Comparing `patroni-3.0.3/patroni/psycopg.py` & `patroni-3.0.4/patroni/psycopg.py`

 * *Files identical despite different names*

### Comparing `patroni-3.0.3/patroni/raft_controller.py` & `patroni-3.0.4/patroni/raft_controller.py`

 * *Files identical despite different names*

### Comparing `patroni-3.0.3/patroni/request.py` & `patroni-3.0.4/patroni/request.py`

 * *Files identical despite different names*

### Comparing `patroni-3.0.3/patroni/scripts/aws.py` & `patroni-3.0.4/patroni/scripts/aws.py`

 * *Files identical despite different names*

### Comparing `patroni-3.0.3/patroni/scripts/wale_restore.py` & `patroni-3.0.4/patroni/scripts/wale_restore.py`

 * *Files identical despite different names*

### Comparing `patroni-3.0.3/patroni/utils.py` & `patroni-3.0.4/patroni/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -322,14 +322,29 @@
 
         >>> parse_int('1000 ms', 's') == 1
         True
 
         >>> parse_int('1TB', 'GB') is None
         True
 
+        >>> parse_int(50, None) == 50
+        True
+
+        >>> parse_int("51", None) == 51
+        True
+
+        >>> parse_int("nonsense", None) == None
+        True
+
+        >>> parse_int("nonsense", "kB") == None
+        True
+
+        >>> parse_int("nonsense") == None
+        True
+
         >>> parse_int(0) == 0
         True
 
         >>> parse_int('6GB', '16MB') == 384
         True
 
         >>> parse_int('4097.4kB', 'kB') == 4097
@@ -754,15 +769,16 @@
         if m.name == leader_name:
             role = 'standby_leader' if global_config.is_standby_cluster else 'leader'
         elif cluster.sync.matches(m.name):
             role = 'sync_standby'
         else:
             role = 'replica'
 
-        member = {'name': m.name, 'role': role, 'state': m.data.get('state', ''), 'api_url': m.api_url}
+        state = (m.data.get('replication_state', '') if role != 'leader' else '') or m.data.get('state', '')
+        member = {'name': m.name, 'role': role, 'state': state, 'api_url': m.api_url}
         conn_kwargs = m.conn_kwargs()
         if conn_kwargs.get('host'):
             member['host'] = conn_kwargs['host']
             if conn_kwargs.get('port'):
                 member['port'] = int(conn_kwargs['port'])
         optional_attributes = ('timeline', 'pending_restart', 'scheduled_restart', 'tags')
         member.update({n: m.data[n] for n in optional_attributes if n in m.data})
```

### Comparing `patroni-3.0.3/patroni/validator.py` & `patroni-3.0.4/patroni/validator.py`

 * *Files 0% similar despite different names*

```diff
@@ -788,16 +788,15 @@
         """Check if *value* is a valid integer and within the expected range.
 
         .. note::
             If ``raise_assert`` is ``True`` and *value* is not valid, then an ``AssertionError`` will be triggered.
         :param value: value to be checked against the rules defined for this :class:`IntValidator` instance.
         :returns: ``True`` if *value* is valid and within the expected range.
         """
-        if self.base_unit:
-            value = parse_int(value, self.base_unit) or ""
+        value = parse_int(value, self.base_unit) or ""
         ret = isinstance(value, int)\
             and (self.min is None or value >= self.min)\
             and (self.max is None or value <= self.max)
 
         if self.raise_assert:
             assert_(ret)
         return ret
```

### Comparing `patroni-3.0.3/patroni/watchdog/base.py` & `patroni-3.0.4/patroni/watchdog/base.py`

 * *Files identical despite different names*

### Comparing `patroni-3.0.3/patroni/watchdog/linux.py` & `patroni-3.0.4/patroni/watchdog/linux.py`

 * *Files identical despite different names*

### Comparing `patroni-3.0.3/patroni.egg-info/PKG-INFO` & `patroni-3.0.4/patroni.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: patroni
-Version: 3.0.3
+Version: 3.0.4
 Summary: PostgreSQL High-Available orchestrator and CLI
 Home-page: https://github.com/zalando/patroni
 Author: Alexander Kukushkin, Polina Bungina
 Author-email: akukushkin@microsoft.com, polina.bungina@zalando.de
 License: The MIT License
 Keywords: etcd governor patroni postgresql postgres ha haproxy confd zookeeper exhibitor consul streaming replication kubernetes k8s
 Classifier: Development Status :: 5 - Production/Stable
@@ -41,15 +41,15 @@
 --------------------------------------------------------------------
 
 You can find a version of this documentation that is searchable and also easier to navigate at `patroni.readthedocs.io <https://patroni.readthedocs.io>`__.
 
 
 There are many ways to run high availability with PostgreSQL; for a list, see the `PostgreSQL Documentation <https://wiki.postgresql.org/wiki/Replication,_Clustering,_and_Connection_Pooling>`__.
 
-Patroni is a template for high availability (HA) PostgreSQL solutions using Python. For maximum accessibility, Patroni supports a variety of distributed configuration stores like `ZooKeeper <https://zookeeper.apache.org/>`__, `etcd <https://github.com/coreos/etcd>`__, `Consul <https://github.com/hashicorp/consul>`__ or `Kubernetes <https://kubernetes.io>`__. Database engineers, DBAs, DevOps engineers, and SREs who are looking to quickly deploy HA PostgreSQL in datacenters — or anywhere else — will hopefully find it useful.
+Patroni is a template for high availability (HA) PostgreSQL solutions using Python. For maximum accessibility, Patroni supports a variety of distributed configuration stores like `ZooKeeper <https://zookeeper.apache.org/>`__, `etcd <https://github.com/coreos/etcd>`__, `Consul <https://github.com/hashicorp/consul>`__ or `Kubernetes <https://kubernetes.io>`__. Database engineers, DBAs, DevOps engineers, and SREs who are looking to quickly deploy HA PostgreSQL in datacenters - or anywhere else - will hopefully find it useful.
 
 We call Patroni a "template" because it is far from being a one-size-fits-all or plug-and-play replication system. It will have its own caveats. Use wisely.
 
 Currently supported PostgreSQL versions: 9.3 to 15.
 
 **Note to Citus users**: Starting from 3.0 Patroni nicely integrates with the `Citus <https://github.com/citusdata/citus>`__ database extension to Postgres. Please check the `Citus support page <https://github.com/zalando/patroni/blob/master/docs/citus.rst>`__ in the Patroni documentation for more info about how to use Patroni high availability together with a Citus distributed cluster.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `patroni-3.0.3/patroni.egg-info/SOURCES.txt` & `patroni-3.0.4/patroni.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `patroni-3.0.3/setup.py` & `patroni-3.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,15 +84,15 @@
                 package_directory = package
 
             if not package_directory.startswith(seen_package_directories):
                 seen_package_directories += (package_directory + ".",)
                 yield package_directory
 
     def targets(self):
-        return [package for package in self.package_files()] + ['tests', 'setup.py']
+        return [package for package in self.package_files()] + ['tests', 'features', 'setup.py']
 
     def run(self):
         from flake8.main.cli import main
 
         logging.getLogger().setLevel(logging.ERROR)
         raise SystemExit(main(self.targets()))
 
@@ -112,15 +112,15 @@
             ['--cov', MAIN_PACKAGE, '--cov-report', 'term-missing', '--cov-report', 'xml']
 
         errno = pytest.main(args=args)
         sys.exit(errno)
 
 
 def read(fname):
-    with open(os.path.join(__location__, fname)) as fd:
+    with open(os.path.join(__location__, fname), encoding='utf-8') as fd:
         return fd.read()
 
 
 def setup_package(version):
     logging.basicConfig(format='%(message)s', level=os.getenv('LOGLEVEL', logging.WARNING))
 
     # Assemble additional setup commands
```

### Comparing `patroni-3.0.3/tests/test_api.py` & `patroni-3.0.4/tests/test_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,16 @@
 
 
 class MockPostgresql(object):
 
     name = 'test'
     state = 'running'
     role = 'primary'
-    server_version = '999999'
+    server_version = 90625
+    major_version = 90600
     sysid = 'dummysysid'
     scope = 'dummy'
     pending_restart = True
     wal_name = 'wal'
     lsn_name = 'lsn'
     POSTMASTER_START_TIME = 'pg_catalog.pg_postmaster_start_time()'
     TL_LSN = 'CASE WHEN pg_catalog.pg_is_in_recovery()'
@@ -51,14 +52,18 @@
     def replica_cached_timeline(_):
         return 2
 
     @staticmethod
     def is_running():
         return True
 
+    @staticmethod
+    def replication_state_from_parameters(*args):
+        return 'streaming'
+
 
 class MockWatchdog(object):
     is_healthy = False
 
 
 class MockHa(object):
 
@@ -176,15 +181,14 @@
                             'http_extra_headers': {'foo': 'bar'}, 'https_extra_headers': {'foo': 'sbar'}}
         super(MockRestApiServer, self).__init__(MockPatroni(), config)
         Handler(MockRequest(request), ('0.0.0.0', 8080), self)
 
 
 @patch('ssl.SSLContext.load_cert_chain', Mock())
 @patch('ssl.SSLContext.wrap_socket', Mock(return_value=0))
-@patch('ssl.SSLContext.load_verify_locations', Mock(return_value=[Mock()]))
 @patch.object(HTTPServer, '__init__', Mock())
 class TestRestApiHandler(unittest.TestCase):
 
     _authorization = '\nAuthorization: Basic dGVzdDp0ZXN0'
 
     def test_do_GET(self):
         MockPatroni.dcs.cluster.last_lsn = 20
@@ -216,15 +220,15 @@
                 MockRestApiServer(RestApiHandler, 'GET /standby_leader')
         MockPatroni.dcs.cluster = None
         with patch.object(RestApiHandler, 'get_postgresql_status', Mock(return_value={'role': 'primary'})):
             MockRestApiServer(RestApiHandler, 'GET /primary')
         with patch.object(MockHa, 'restart_scheduled', Mock(return_value=True)):
             MockRestApiServer(RestApiHandler, 'GET /primary')
         self.assertIsNotNone(MockRestApiServer(RestApiHandler, 'GET /primary'))
-        with patch.object(RestApiServer, 'query', Mock(return_value=[('', 1, '', '', '', '', False, '')])):
+        with patch.object(RestApiServer, 'query', Mock(return_value=[('', 1, '', '', '', '', False, None, None, '')])):
             self.assertIsNotNone(MockRestApiServer(RestApiHandler, 'GET /patroni'))
         with patch.object(GlobalConfig, 'is_standby_cluster', Mock(return_value=True)),\
                 patch.object(GlobalConfig, 'is_paused', Mock(return_value=True)):
             MockRestApiServer(RestApiHandler, 'GET /standby_leader')
 
         # test tags
         #
@@ -585,15 +589,14 @@
 
 
 class TestRestApiServer(unittest.TestCase):
 
     @patch('ssl.SSLContext.load_cert_chain', Mock())
     @patch('ssl.SSLContext.set_ciphers', Mock())
     @patch('ssl.SSLContext.wrap_socket', Mock(return_value=0))
-    @patch('ssl.SSLContext.load_verify_locations', Mock(return_value=[Mock()]))
     @patch.object(HTTPServer, '__init__', Mock())
     def setUp(self):
         self.srv = MockRestApiServer(Mock(), '', {'listen': '*:8008', 'certfile': 'a', 'verify_client': 'required',
                                                   'ciphers': '!SSLv1:!SSLv2:!SSLv3:!TLSv1:!TLSv1.1',
                                                   'allowlist': ['127.0.0.1', '::1/128', '::1/zxc'],
                                                   'allowlist_include_members': True})
 
@@ -648,14 +651,13 @@
 
     @patch.object(MockRestApiServer, 'process_request', Mock(side_effect=RuntimeError))
     @patch.object(MockRestApiServer, 'get_request')
     def test_process_request_error(self, mock_get_request):
         mock_get_request.return_value = (self.__create_socket(), ('127.0.0.1', 55555))
         self.srv._handle_request_noblock()
 
-    @patch('ssl.SSLContext.load_verify_locations', Mock(return_value=[Mock()]))
+    @patch('ssl._ssl._test_decode_cert', Mock())
     def test_reload_local_certificate(self):
         self.assertTrue(self.srv.reload_local_certificate())
 
-    @patch('ssl.SSLContext.load_verify_locations', Mock(side_effect=Exception))
     def test_get_certificate_serial_number(self):
         self.assertIsNone(self.srv.get_certificate_serial_number())
```

### Comparing `patroni-3.0.3/tests/test_async_executor.py` & `patroni-3.0.4/tests/test_async_executor.py`

 * *Files identical despite different names*

### Comparing `patroni-3.0.3/tests/test_aws.py` & `patroni-3.0.4/tests/test_aws.py`

 * *Files identical despite different names*

### Comparing `patroni-3.0.3/tests/test_bootstrap.py` & `patroni-3.0.4/tests/test_bootstrap.py`

 * *Files identical despite different names*

### Comparing `patroni-3.0.3/tests/test_callback_executor.py` & `patroni-3.0.4/tests/test_callback_executor.py`

 * *Files identical despite different names*

### Comparing `patroni-3.0.3/tests/test_cancellable.py` & `patroni-3.0.4/tests/test_cancellable.py`

 * *Files identical despite different names*

### Comparing `patroni-3.0.3/tests/test_citus.py` & `patroni-3.0.4/tests/test_citus.py`

 * *Files identical despite different names*

### Comparing `patroni-3.0.3/tests/test_config.py` & `patroni-3.0.4/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `patroni-3.0.3/tests/test_consul.py` & `patroni-3.0.4/tests/test_consul.py`

 * *Files identical despite different names*

### Comparing `patroni-3.0.3/tests/test_ctl.py` & `patroni-3.0.4/tests/test_ctl.py`

 * *Files identical despite different names*

### Comparing `patroni-3.0.3/tests/test_etcd.py` & `patroni-3.0.4/tests/test_etcd.py`

 * *Files identical despite different names*

### Comparing `patroni-3.0.3/tests/test_etcd3.py` & `patroni-3.0.4/tests/test_etcd3.py`

 * *Files identical despite different names*

### Comparing `patroni-3.0.3/tests/test_exhibitor.py` & `patroni-3.0.4/tests/test_exhibitor.py`

 * *Files identical despite different names*

### Comparing `patroni-3.0.3/tests/test_ha.py` & `patroni-3.0.4/tests/test_ha.py`

 * *Files 2% similar despite different names*

```diff
@@ -219,17 +219,20 @@
         self.p.last_operation = Mock(side_effect=PostgresConnectionException(''))
         self.ha.dcs.update_leader = Mock(side_effect=[DCSError(''), Exception])
         self.assertRaises(DCSError, self.ha.update_lock)
         self.assertFalse(self.ha.update_lock(True))
 
     @patch.object(Postgresql, 'received_timeline', Mock(return_value=None))
     def test_touch_member(self):
+        self.p._major_version = 110000
+        self.p.is_leader = false
         self.p.timeline_wal_position = Mock(return_value=(0, 1, 0))
         self.p.replica_cached_timeline = Mock(side_effect=Exception)
-        self.ha.touch_member()
+        with patch.object(Postgresql, '_cluster_info_state_get', Mock(return_value='streaming')):
+            self.ha.touch_member()
         self.p.timeline_wal_position = Mock(return_value=(0, 1, 1))
         self.p.set_role('standby_leader')
         self.ha.touch_member()
         self.p.set_role('primary')
         self.ha.dcs.touch_member = true
         self.ha.touch_member()
 
@@ -278,19 +281,28 @@
         self.ha.dcs.__class__.__name__ = 'Raft'
         self.assertEqual(self.ha.run_cycle(), 'started as a secondary')
 
     def test_recover_former_primary(self):
         self.p.follow = false
         self.p.is_running = false
         self.p.name = 'leader'
-        self.p.set_role('primary')
+        self.p.set_role('demoted')
         self.p.controldata = lambda: {'Database cluster state': 'shut down', 'Database system identifier': SYSID}
         self.ha.cluster = get_cluster_initialized_with_leader()
         self.assertEqual(self.ha.run_cycle(), 'starting as readonly because i had the session lock')
 
+    def test_start_primary_after_failure(self):
+        self.p.start = false
+        self.p.is_running = false
+        self.p.name = 'leader'
+        self.p.set_role('primary')
+        self.p.controldata = lambda: {'Database cluster state': 'in production', 'Database system identifier': SYSID}
+        self.ha.cluster = get_cluster_initialized_with_leader()
+        self.assertEqual(self.ha.run_cycle(), 'starting primary after failure')
+
     @patch.object(Rewind, 'ensure_clean_shutdown', Mock())
     def test_crash_recovery(self):
         self.ha.has_lock = true
         self.p.is_running = false
         self.p.controldata = lambda: {'Database cluster state': 'in production', 'Database system identifier': SYSID}
         self.assertEqual(self.ha.run_cycle(), 'doing crash recovery in a single user mode')
         with patch('patroni.async_executor.AsyncExecutor.busy', PropertyMock(return_value=True)),\
@@ -570,14 +582,15 @@
     def test_bootstrap_initialized_new_cluster(self):
         self.ha.cluster = get_cluster_not_initialized_without_leader()
         self.e.initialize = true
         self.assertEqual(self.ha.bootstrap(), 'trying to bootstrap a new cluster')
         self.p.is_leader = false
         self.assertEqual(self.ha.run_cycle(), 'waiting for end of recovery after bootstrap')
         self.p.is_leader = true
+        self.ha.is_synchronous_mode = true
         self.assertEqual(self.ha.run_cycle(), 'running post_bootstrap')
         self.assertEqual(self.ha.run_cycle(), 'initialized a new cluster')
 
     def test_bootstrap_release_initialize_key_on_failure(self):
         self.ha.cluster = get_cluster_not_initialized_without_leader()
         self.e.initialize = true
         self.ha.bootstrap()
@@ -833,16 +846,14 @@
         self.ha.dcs._last_failsafe = {'foo': ''}
         self.assertFalse(self.ha.is_healthiest_node())
         self.ha.dcs._last_failsafe = {'postgresql0': ''}
         self.assertTrue(self.ha.is_healthiest_node())
         self.ha.dcs._last_failsafe = None
         with patch.object(Watchdog, 'is_healthy', PropertyMock(return_value=False)):
             self.assertFalse(self.ha.is_healthiest_node())
-        with patch('patroni.postgresql.Postgresql.is_starting', return_value=True):
-            self.assertFalse(self.ha.is_healthiest_node())
         self.ha.is_paused = true
         self.assertFalse(self.ha.is_healthiest_node())
 
     def test__is_healthiest_node(self):
         self.p.is_leader = false
         self.ha.cluster = get_cluster_initialized_without_leader(sync=('postgresql1', self.p.name))
         self.ha.global_config = self.ha.patroni.config.get_global_config(self.ha.cluster)
```

### Comparing `patroni-3.0.3/tests/test_kubernetes.py` & `patroni-3.0.4/tests/test_kubernetes.py`

 * *Files identical despite different names*

### Comparing `patroni-3.0.3/tests/test_log.py` & `patroni-3.0.4/tests/test_log.py`

 * *Files identical despite different names*

### Comparing `patroni-3.0.3/tests/test_patroni.py` & `patroni-3.0.4/tests/test_patroni.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import unittest
 
 import patroni.config as config
 from http.server import HTTPServer
 from mock import Mock, PropertyMock, patch
 from patroni.api import RestApiServer
 from patroni.async_executor import AsyncExecutor
+from patroni.dcs import Cluster, Member
 from patroni.dcs.etcd import AbstractEtcdClientWithFailover
 from patroni.exceptions import DCSError
 from patroni.postgresql import Postgresql
 from patroni.postgresql.config import ConfigHandler
 from patroni import check_psycopg
 from patroni.__main__ import Patroni, main as _main
 from threading import Thread
@@ -198,7 +199,40 @@
         self.p.shutdown()
 
     def test_check_psycopg(self):
         with patch('builtins.__import__', Mock(side_effect=ImportError)):
             self.assertRaises(SystemExit, check_psycopg)
         with patch('builtins.__import__', mock_import):
             self.assertRaises(SystemExit, check_psycopg)
+
+    def test_ensure_unique_name(self):
+        # None/empty cluster implies unique name
+        with patch('patroni.dcs.AbstractDCS.get_cluster', Mock(return_value=None)):
+            self.assertIsNone(self.p.ensure_unique_name())
+        empty_cluster = Cluster.empty()
+        with patch('patroni.dcs.AbstractDCS.get_cluster', Mock(return_value=empty_cluster)):
+            self.assertIsNone(self.p.ensure_unique_name())
+        without_members = empty_cluster._asdict()
+        del without_members['members']
+
+        # Cluster with members with different names implies unique name
+        okay_cluster = Cluster(
+            members=[Member(version=1, name="distinct", session=1, data={})],
+            **without_members
+        )
+        with patch('patroni.dcs.AbstractDCS.get_cluster', Mock(return_value=okay_cluster)):
+            self.assertIsNone(self.p.ensure_unique_name())
+
+        # Cluster with a member with the same name that is running
+        bad_cluster = Cluster(
+            members=[Member(version=1, name="postgresql0", session=1, data={
+                "api_url": "https://127.0.0.1:8008",
+            })],
+            **without_members
+        )
+        with patch('patroni.dcs.AbstractDCS.get_cluster', Mock(return_value=bad_cluster)):
+            # If the api of the running node cannot be reached, this implies unique name
+            with patch.object(self.p, 'request', Mock(side_effect=ConnectionError)):
+                self.assertIsNone(self.p.ensure_unique_name())
+            # Only if the api of the running node is reachable do we throw an error
+            with patch.object(self.p, 'request', Mock()):
+                self.assertRaises(SystemExit, self.p.ensure_unique_name)
```

### Comparing `patroni-3.0.3/tests/test_postgresql.py` & `patroni-3.0.4/tests/test_postgresql.py`

 * *Files identical despite different names*

### Comparing `patroni-3.0.3/tests/test_postmaster.py` & `patroni-3.0.4/tests/test_postmaster.py`

 * *Files identical despite different names*

### Comparing `patroni-3.0.3/tests/test_raft.py` & `patroni-3.0.4/tests/test_raft.py`

 * *Files identical despite different names*

### Comparing `patroni-3.0.3/tests/test_raft_controller.py` & `patroni-3.0.4/tests/test_raft_controller.py`

 * *Files identical despite different names*

### Comparing `patroni-3.0.3/tests/test_rewind.py` & `patroni-3.0.4/tests/test_rewind.py`

 * *Files 0% similar despite different names*

```diff
@@ -87,17 +87,18 @@
         with patch.object(Postgresql, 'controldata',
                           Mock(return_value={'Database cluster state': 'shut down in recovery',
                                              'Minimum recovery ending location': '0/0',
                                              "Min recovery ending loc's timeline": '0',
                                              'Latest checkpoint location': '0/'})):
             self.r.rewind_or_reinitialize_needed_and_possible(self.leader)
 
-        with patch.object(Postgresql, 'is_running', Mock(return_value=True)):
-            with patch.object(MockCursor, 'fetchone', Mock(side_effect=[(0, 0, 1, 1, 0, 0, 0, 0, 0, None), Exception])):
-                self.r.rewind_or_reinitialize_needed_and_possible(self.leader)
+        with patch.object(Postgresql, 'is_running', Mock(return_value=True)),\
+                patch.object(MockCursor, 'fetchone',
+                             Mock(side_effect=[(0, 0, 1, 1, 0, 0, 0, 0, 0, None, None, None), Exception])):
+            self.r.rewind_or_reinitialize_needed_and_possible(self.leader)
 
     @patch.object(CancellableSubprocess, 'call', mock_cancellable_call)
     @patch.object(Postgresql, 'checkpoint', side_effect=['', '1'],)
     @patch.object(Postgresql, 'stop', Mock(return_value=False))
     @patch.object(Postgresql, 'start', Mock())
     def test_execute(self, mock_checkpoint):
         self.r.execute(self.leader)
```

### Comparing `patroni-3.0.3/tests/test_slots.py` & `patroni-3.0.4/tests/test_slots.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,22 +73,22 @@
         cluster = Cluster(True, config, self.leader, 0, [self.me, self.other, self.leadermem],
                           None, SyncState.empty(), None, None, None)
 
         self.s.sync_replication_slots(cluster, False)
         with patch.object(Postgresql, '_query') as mock_query:
             self.p.reset_cluster_info_state(None)
             mock_query.return_value.fetchone.return_value = (
-                1, 0, 0, 0, 0, 0, 0, 0, 0,
+                1, 0, 0, 0, 0, 0, 0, 0, 0, None, None,
                 [{"slot_name": "ls", "type": "logical", "datoid": 5, "plugin": "b",
                   "confirmed_flush_lsn": 12345, "catalog_xmin": 105}])
             self.assertEqual(self.p.slots(), {'ls': 12345})
 
             self.p.reset_cluster_info_state(None)
             mock_query.return_value.fetchone.return_value = (
-                1, 0, 0, 0, 0, 0, 0, 0, 0,
+                1, 0, 0, 0, 0, 0, 0, 0, 0, None, None,
                 [{"slot_name": "ls", "type": "logical", "datoid": 6, "plugin": "b",
                   "confirmed_flush_lsn": 12345, "catalog_xmin": 105}])
             self.assertEqual(self.p.slots(), {})
 
     @patch.object(Postgresql, 'is_leader', Mock(return_value=False))
     def test__ensure_logical_slots_replica(self):
         self.p.set_role('replica')
```

### Comparing `patroni-3.0.3/tests/test_sync.py` & `patroni-3.0.4/tests/test_sync.py`

 * *Files identical despite different names*

### Comparing `patroni-3.0.3/tests/test_utils.py` & `patroni-3.0.4/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `patroni-3.0.3/tests/test_validator.py` & `patroni-3.0.4/tests/test_validator.py`

 * *Files identical despite different names*

### Comparing `patroni-3.0.3/tests/test_wale_restore.py` & `patroni-3.0.4/tests/test_wale_restore.py`

 * *Files identical despite different names*

### Comparing `patroni-3.0.3/tests/test_watchdog.py` & `patroni-3.0.4/tests/test_watchdog.py`

 * *Files identical despite different names*

### Comparing `patroni-3.0.3/tests/test_zookeeper.py` & `patroni-3.0.4/tests/test_zookeeper.py`

 * *Files identical despite different names*

