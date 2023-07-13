# Comparing `tmp/fluvii-1.0.2.tar.gz` & `tmp/fluvii-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fluvii-1.0.2.tar", last modified: Fri Mar  3 01:07:20 2023, max compression
+gzip compressed data, was "fluvii-1.1.0.tar", last modified: Wed Apr  5 19:36:23 2023, max compression
```

## Comparing `fluvii-1.0.2.tar` & `fluvii-1.1.0.tar`

### file list

```diff
@@ -1,93 +1,93 @@
-drwxrwxr-x   0 tsawicki  (1000) tsawicki  (1000)        0 2023-03-03 01:07:20.969529 fluvii-1.0.2/
--rw-rw-r--   0 tsawicki  (1000) tsawicki  (1000)     1085 2022-10-04 23:35:24.000000 fluvii-1.0.2/LICENSE
--rw-rw-r--   0 tsawicki  (1000) tsawicki  (1000)      336 2023-03-03 01:07:20.969529 fluvii-1.0.2/PKG-INFO
--rw-rw-r--   0 tsawicki  (1000) tsawicki  (1000)    27119 2023-03-02 02:19:36.000000 fluvii-1.0.2/README.md
-drwxrwxr-x   0 tsawicki  (1000) tsawicki  (1000)        0 2023-03-03 01:07:20.961530 fluvii-1.0.2/fluvii/
--rw-rw-r--   0 tsawicki  (1000) tsawicki  (1000)      471 2023-02-24 19:18:17.000000 fluvii-1.0.2/fluvii/__init__.py
-drwxrwxr-x   0 tsawicki  (1000) tsawicki  (1000)        0 2023-03-03 01:07:20.961530 fluvii-1.0.2/fluvii/apps/
--rw-rw-r--   0 tsawicki  (1000) tsawicki  (1000)      192 2023-02-24 19:18:17.000000 fluvii-1.0.2/fluvii/apps/__init__.py
--rw-rw-r--   0 tsawicki  (1000) tsawicki  (1000)      973 2023-02-24 19:18:17.000000 fluvii-1.0.2/fluvii/apps/config.py
--rw-rw-r--   0 tsawicki  (1000) tsawicki  (1000)     4923 2023-03-02 02:19:36.000000 fluvii-1.0.2/fluvii/apps/fluvii_app.py
--rw-rw-r--   0 tsawicki  (1000) tsawicki  (1000)     1208 2023-02-24 21:59:00.000000 fluvii-1.0.2/fluvii/apps/fluvii_multi_msg_app.py
--rw-rw-r--   0 tsawicki  (1000) tsawicki  (1000)     7106 2023-03-02 02:19:36.000000 fluvii-1.0.2/fluvii/apps/fluvii_table_app.py
-drwxrwxr-x   0 tsawicki  (1000) tsawicki  (1000)        0 2023-03-03 01:07:20.965530 fluvii-1.0.2/fluvii/apps/helpers/
--rw-rw-r--   0 tsawicki  (1000) tsawicki  (1000)       94 2023-02-24 19:18:17.000000 fluvii-1.0.2/fluvii/apps/helpers/__init__.py
--rw-rw-r--   0 tsawicki  (1000) tsawicki  (1000)     4374 2023-03-02 02:19:36.000000 fluvii-1.0.2/fluvii/apps/helpers/app_factory_base.py
--rw-rw-r--   0 tsawicki  (1000) tsawicki  (1000)    11900 2023-02-24 19:18:17.000000 fluvii-1.0.2/fluvii/apps/helpers/rebalance_manager.py
-drwxrwxr-x   0 tsawicki  (1000) tsawicki  (1000)        0 2023-03-03 01:07:20.965530 fluvii-1.0.2/fluvii/apps/transactions/
--rw-rw-r--   0 tsawicki  (1000) tsawicki  (1000)      142 2023-02-24 19:18:17.000000 fluvii-1.0.2/fluvii/apps/transactions/__init__.py
--rw-rw-r--   0 tsawicki  (1000) tsawicki  (1000)     7535 2023-02-24 19:18:17.000000 fluvii-1.0.2/fluvii/apps/transactions/consumer.py
--rw-rw-r--   0 tsawicki  (1000) tsawicki  (1000)     1575 2023-02-24 19:18:17.000000 fluvii-1.0.2/fluvii/apps/transactions/producer.py
--rw-rw-r--   0 tsawicki  (1000) tsawicki  (1000)     8283 2023-03-02 02:19:36.000000 fluvii-1.0.2/fluvii/apps/transactions/transaction.py
-drwxrwxr-x   0 tsawicki  (1000) tsawicki  (1000)        0 2023-03-03 01:07:20.965530 fluvii-1.0.2/fluvii/cli/
--rw-rw-r--   0 tsawicki  (1000) tsawicki  (1000)        0 2023-02-24 19:18:17.000000 fluvii-1.0.2/fluvii/cli/__init__.py
--rw-rw-r--   0 tsawicki  (1000) tsawicki  (1000)       88 2023-01-09 19:04:10.000000 fluvii-1.0.2/fluvii/cli/__main__.py
-drwxrwxr-x   0 tsawicki  (1000) tsawicki  (1000)        0 2023-03-03 01:07:20.965530 fluvii-1.0.2/fluvii/cli/commands/
--rw-rw-r--   0 tsawicki  (1000) tsawicki  (1000)       62 2023-01-09 19:04:10.000000 fluvii-1.0.2/fluvii/cli/commands/__init__.py
--rw-rw-r--   0 tsawicki  (1000) tsawicki  (1000)      122 2023-01-09 19:04:10.000000 fluvii-1.0.2/fluvii/cli/commands/base.py
--rw-rw-r--   0 tsawicki  (1000) tsawicki  (1000)     3333 2023-02-24 19:18:17.000000 fluvii-1.0.2/fluvii/cli/commands/topics.py
-drwxrwxr-x   0 tsawicki  (1000) tsawicki  (1000)        0 2023-03-03 01:07:20.965530 fluvii-1.0.2/fluvii/components/
--rw-rw-r--   0 tsawicki  (1000) tsawicki  (1000)      208 2023-02-24 19:18:17.000000 fluvii-1.0.2/fluvii/components/__init__.py
-drwxrwxr-x   0 tsawicki  (1000) tsawicki  (1000)        0 2023-03-03 01:07:20.965530 fluvii-1.0.2/fluvii/components/admin/
--rw-rw-r--   0 tsawicki  (1000) tsawicki  (1000)       57 2023-02-24 19:18:17.000000 fluvii-1.0.2/fluvii/components/admin/__init__.py
--rw-rw-r--   0 tsawicki  (1000) tsawicki  (1000)      507 2023-02-24 19:18:17.000000 fluvii-1.0.2/fluvii/components/admin/admin.py
--rw-rw-r--   0 tsawicki  (1000) tsawicki  (1000)      766 2023-02-24 19:18:17.000000 fluvii-1.0.2/fluvii/components/admin/config.py
-drwxrwxr-x   0 tsawicki  (1000) tsawicki  (1000)        0 2023-03-03 01:07:20.965530 fluvii-1.0.2/fluvii/components/auth/
--rw-rw-r--   0 tsawicki  (1000) tsawicki  (1000)       59 2023-02-24 19:18:17.000000 fluvii-1.0.2/fluvii/components/auth/__init__.py
--rw-rw-r--   0 tsawicki  (1000) tsawicki  (1000)     2012 2023-03-03 01:05:42.000000 fluvii-1.0.2/fluvii/components/auth/config.py
-drwxrwxr-x   0 tsawicki  (1000) tsawicki  (1000)        0 2023-03-03 01:07:20.965530 fluvii-1.0.2/fluvii/components/consumer/
--rw-rw-r--   0 tsawicki  (1000) tsawicki  (1000)      112 2023-02-24 19:18:17.000000 fluvii-1.0.2/fluvii/components/consumer/__init__.py
--rw-rw-r--   0 tsawicki  (1000) tsawicki  (1000)     2390 2023-03-02 02:19:36.000000 fluvii-1.0.2/fluvii/components/consumer/config.py
--rw-rw-r--   0 tsawicki  (1000) tsawicki  (1000)     5449 2023-02-24 20:59:37.000000 fluvii-1.0.2/fluvii/components/consumer/consumer.py
--rw-rw-r--   0 tsawicki  (1000) tsawicki  (1000)     2764 2023-03-02 02:19:36.000000 fluvii-1.0.2/fluvii/components/consumer/consumer_factory.py
-drwxrwxr-x   0 tsawicki  (1000) tsawicki  (1000)        0 2023-03-03 01:07:20.965530 fluvii-1.0.2/fluvii/components/metrics/
--rw-rw-r--   0 tsawicki  (1000) tsawicki  (1000)      113 2023-02-24 19:18:17.000000 fluvii-1.0.2/fluvii/components/metrics/__init__.py
-drwxrwxr-x   0 tsawicki  (1000) tsawicki  (1000)        0 2023-03-03 01:07:20.965530 fluvii-1.0.2/fluvii/components/metrics/manager/
--rw-rw-r--   0 tsawicki  (1000) tsawicki  (1000)       85 2023-02-24 19:18:17.000000 fluvii-1.0.2/fluvii/components/metrics/manager/__init__.py
--rw-rw-r--   0 tsawicki  (1000) tsawicki  (1000)      290 2023-03-02 02:19:36.000000 fluvii-1.0.2/fluvii/components/metrics/manager/config.py
--rw-rw-r--   0 tsawicki  (1000) tsawicki  (1000)     3965 2023-03-02 02:19:36.000000 fluvii-1.0.2/fluvii/components/metrics/manager/metrics_manager.py
-drwxrwxr-x   0 tsawicki  (1000) tsawicki  (1000)        0 2023-03-03 01:07:20.965530 fluvii-1.0.2/fluvii/components/metrics/pusher/
--rw-rw-r--   0 tsawicki  (1000) tsawicki  (1000)       82 2023-02-24 19:18:17.000000 fluvii-1.0.2/fluvii/components/metrics/pusher/__init__.py
--rw-rw-r--   0 tsawicki  (1000) tsawicki  (1000)      402 2023-02-24 19:18:17.000000 fluvii-1.0.2/fluvii/components/metrics/pusher/config.py
--rw-rw-r--   0 tsawicki  (1000) tsawicki  (1000)     2586 2023-02-24 19:18:17.000000 fluvii-1.0.2/fluvii/components/metrics/pusher/metrics_pusher.py
-drwxrwxr-x   0 tsawicki  (1000) tsawicki  (1000)        0 2023-03-03 01:07:20.965530 fluvii-1.0.2/fluvii/components/producer/
--rw-rw-r--   0 tsawicki  (1000) tsawicki  (1000)      112 2023-02-24 19:18:17.000000 fluvii-1.0.2/fluvii/components/producer/__init__.py
--rw-rw-r--   0 tsawicki  (1000) tsawicki  (1000)      953 2023-02-24 19:18:17.000000 fluvii-1.0.2/fluvii/components/producer/config.py
--rw-rw-r--   0 tsawicki  (1000) tsawicki  (1000)     8971 2023-02-24 19:18:17.000000 fluvii-1.0.2/fluvii/components/producer/producer.py
--rw-rw-r--   0 tsawicki  (1000) tsawicki  (1000)     2495 2023-03-02 02:19:36.000000 fluvii-1.0.2/fluvii/components/producer/producer_factory.py
-drwxrwxr-x   0 tsawicki  (1000) tsawicki  (1000)        0 2023-03-03 01:07:20.969529 fluvii-1.0.2/fluvii/components/schema_registry/
--rw-rw-r--   0 tsawicki  (1000) tsawicki  (1000)       85 2023-02-24 19:18:17.000000 fluvii-1.0.2/fluvii/components/schema_registry/__init__.py
--rw-rw-r--   0 tsawicki  (1000) tsawicki  (1000)      480 2023-02-24 19:18:17.000000 fluvii-1.0.2/fluvii/components/schema_registry/config.py
--rw-rw-r--   0 tsawicki  (1000) tsawicki  (1000)     1931 2023-02-24 19:18:17.000000 fluvii-1.0.2/fluvii/components/schema_registry/schema_registry.py
-drwxrwxr-x   0 tsawicki  (1000) tsawicki  (1000)        0 2023-03-03 01:07:20.969529 fluvii-1.0.2/fluvii/components/sqlite/
--rw-rw-r--   0 tsawicki  (1000) tsawicki  (1000)       66 2023-02-24 19:18:17.000000 fluvii-1.0.2/fluvii/components/sqlite/__init__.py
--rw-rw-r--   0 tsawicki  (1000) tsawicki  (1000)      326 2023-02-24 19:18:17.000000 fluvii-1.0.2/fluvii/components/sqlite/config.py
--rw-rw-r--   0 tsawicki  (1000) tsawicki  (1000)     6136 2023-02-24 19:18:17.000000 fluvii-1.0.2/fluvii/components/sqlite/sqlite.py
--rw-rw-r--   0 tsawicki  (1000) tsawicki  (1000)      653 2023-02-24 19:18:17.000000 fluvii-1.0.2/fluvii/config_bases.py
--rw-rw-r--   0 tsawicki  (1000) tsawicki  (1000)     2963 2022-11-28 17:26:51.000000 fluvii-1.0.2/fluvii/exceptions.py
--rw-rw-r--   0 tsawicki  (1000) tsawicki  (1000)      927 2023-02-24 19:18:17.000000 fluvii-1.0.2/fluvii/general_utils.py
-drwxrwxr-x   0 tsawicki  (1000) tsawicki  (1000)        0 2023-03-03 01:07:20.969529 fluvii-1.0.2/fluvii/kafka_tools/
--rw-rw-r--   0 tsawicki  (1000) tsawicki  (1000)       42 2023-02-24 19:18:17.000000 fluvii-1.0.2/fluvii/kafka_tools/__init__.py
--rw-rw-r--   0 tsawicki  (1000) tsawicki  (1000)     7461 2023-02-24 19:18:17.000000 fluvii-1.0.2/fluvii/kafka_tools/fluvii_toolbox.py
--rw-rw-r--   0 tsawicki  (1000) tsawicki  (1000)     4398 2023-03-02 02:19:36.000000 fluvii-1.0.2/fluvii/kafka_tools/topic_dumper.py
--rw-rw-r--   0 tsawicki  (1000) tsawicki  (1000)      745 2023-02-14 17:34:34.000000 fluvii-1.0.2/fluvii/logging_utils.py
-drwxrwxr-x   0 tsawicki  (1000) tsawicki  (1000)        0 2023-03-03 01:07:20.961530 fluvii-1.0.2/fluvii.egg-info/
--rw-rw-r--   0 tsawicki  (1000) tsawicki  (1000)      336 2023-03-03 01:07:20.000000 fluvii-1.0.2/fluvii.egg-info/PKG-INFO
--rw-rw-r--   0 tsawicki  (1000) tsawicki  (1000)     2284 2023-03-03 01:07:20.000000 fluvii-1.0.2/fluvii.egg-info/SOURCES.txt
--rw-rw-r--   0 tsawicki  (1000) tsawicki  (1000)        1 2023-03-03 01:07:20.000000 fluvii-1.0.2/fluvii.egg-info/dependency_links.txt
--rw-rw-r--   0 tsawicki  (1000) tsawicki  (1000)       58 2023-03-03 01:07:20.000000 fluvii-1.0.2/fluvii.egg-info/entry_points.txt
--rw-rw-r--   0 tsawicki  (1000) tsawicki  (1000)      277 2023-03-03 01:07:20.000000 fluvii-1.0.2/fluvii.egg-info/requires.txt
--rw-rw-r--   0 tsawicki  (1000) tsawicki  (1000)       13 2023-03-03 01:07:20.000000 fluvii-1.0.2/fluvii.egg-info/top_level.txt
--rw-rw-r--   0 tsawicki  (1000) tsawicki  (1000)      340 2023-02-24 19:18:17.000000 fluvii-1.0.2/pyproject.toml
--rw-rw-r--   0 tsawicki  (1000) tsawicki  (1000)       38 2023-03-03 01:07:20.969529 fluvii-1.0.2/setup.cfg
--rw-rw-r--   0 tsawicki  (1000) tsawicki  (1000)      995 2023-03-03 01:05:42.000000 fluvii-1.0.2/setup.py
-drwxrwxr-x   0 tsawicki  (1000) tsawicki  (1000)        0 2023-03-03 01:07:20.969529 fluvii-1.0.2/tests/
--rw-rw-r--   0 tsawicki  (1000) tsawicki  (1000)        0 2022-11-28 17:26:51.000000 fluvii-1.0.2/tests/__init__.py
-drwxrwxr-x   0 tsawicki  (1000) tsawicki  (1000)        0 2023-03-03 01:07:20.969529 fluvii-1.0.2/tests/temp_integration/
--rw-rw-r--   0 tsawicki  (1000) tsawicki  (1000)        0 2023-02-24 19:18:17.000000 fluvii-1.0.2/tests/temp_integration/__init__.py
--rw-rw-r--   0 tsawicki  (1000) tsawicki  (1000)     4465 2023-02-24 19:18:17.000000 fluvii-1.0.2/tests/temp_integration/integration.py
-drwxrwxr-x   0 tsawicki  (1000) tsawicki  (1000)        0 2023-03-03 01:07:20.969529 fluvii-1.0.2/tests/unit/
--rw-rw-r--   0 tsawicki  (1000) tsawicki  (1000)        0 2022-10-12 22:34:27.000000 fluvii-1.0.2/tests/unit/__init__.py
--rw-rw-r--   0 tsawicki  (1000) tsawicki  (1000)      849 2023-03-02 02:19:36.000000 fluvii-1.0.2/tests/unit/test_consumer.py
--rw-rw-r--   0 tsawicki  (1000) tsawicki  (1000)     1242 2023-03-02 02:19:36.000000 fluvii-1.0.2/tests/unit/test_consumer_config.py
--rw-rw-r--   0 tsawicki  (1000) tsawicki  (1000)      269 2023-03-02 02:19:36.000000 fluvii-1.0.2/tests/unit/test_producer_config.py
+drwxrwxr-x   0 tsawicki  (1000) tsawicki  (1000)        0 2023-04-05 19:36:23.343592 fluvii-1.1.0/
+-rw-rw-r--   0 tsawicki  (1000) tsawicki  (1000)     1085 2022-10-04 23:35:24.000000 fluvii-1.1.0/LICENSE
+-rw-rw-r--   0 tsawicki  (1000) tsawicki  (1000)      400 2023-04-05 19:36:23.343592 fluvii-1.1.0/PKG-INFO
+-rw-rw-r--   0 tsawicki  (1000) tsawicki  (1000)    27298 2023-04-05 19:30:52.000000 fluvii-1.1.0/README.md
+drwxrwxr-x   0 tsawicki  (1000) tsawicki  (1000)        0 2023-04-05 19:36:23.339592 fluvii-1.1.0/fluvii/
+-rw-rw-r--   0 tsawicki  (1000) tsawicki  (1000)      471 2023-02-24 19:18:17.000000 fluvii-1.1.0/fluvii/__init__.py
+drwxrwxr-x   0 tsawicki  (1000) tsawicki  (1000)        0 2023-04-05 19:36:23.339592 fluvii-1.1.0/fluvii/apps/
+-rw-rw-r--   0 tsawicki  (1000) tsawicki  (1000)      192 2023-02-24 19:18:17.000000 fluvii-1.1.0/fluvii/apps/__init__.py
+-rw-rw-r--   0 tsawicki  (1000) tsawicki  (1000)      973 2023-02-24 19:18:17.000000 fluvii-1.1.0/fluvii/apps/config.py
+-rw-rw-r--   0 tsawicki  (1000) tsawicki  (1000)     4923 2023-03-02 02:19:36.000000 fluvii-1.1.0/fluvii/apps/fluvii_app.py
+-rw-rw-r--   0 tsawicki  (1000) tsawicki  (1000)     1208 2023-02-24 21:59:00.000000 fluvii-1.1.0/fluvii/apps/fluvii_multi_msg_app.py
+-rw-rw-r--   0 tsawicki  (1000) tsawicki  (1000)     7106 2023-03-02 02:19:36.000000 fluvii-1.1.0/fluvii/apps/fluvii_table_app.py
+drwxrwxr-x   0 tsawicki  (1000) tsawicki  (1000)        0 2023-04-05 19:36:23.339592 fluvii-1.1.0/fluvii/apps/helpers/
+-rw-rw-r--   0 tsawicki  (1000) tsawicki  (1000)       94 2023-02-24 19:18:17.000000 fluvii-1.1.0/fluvii/apps/helpers/__init__.py
+-rw-rw-r--   0 tsawicki  (1000) tsawicki  (1000)     4377 2023-04-05 19:30:52.000000 fluvii-1.1.0/fluvii/apps/helpers/app_factory_base.py
+-rw-rw-r--   0 tsawicki  (1000) tsawicki  (1000)    11900 2023-02-24 19:18:17.000000 fluvii-1.1.0/fluvii/apps/helpers/rebalance_manager.py
+drwxrwxr-x   0 tsawicki  (1000) tsawicki  (1000)        0 2023-04-05 19:36:23.339592 fluvii-1.1.0/fluvii/apps/transactions/
+-rw-rw-r--   0 tsawicki  (1000) tsawicki  (1000)      142 2023-02-24 19:18:17.000000 fluvii-1.1.0/fluvii/apps/transactions/__init__.py
+-rw-rw-r--   0 tsawicki  (1000) tsawicki  (1000)     7535 2023-02-24 19:18:17.000000 fluvii-1.1.0/fluvii/apps/transactions/consumer.py
+-rw-rw-r--   0 tsawicki  (1000) tsawicki  (1000)     1575 2023-02-24 19:18:17.000000 fluvii-1.1.0/fluvii/apps/transactions/producer.py
+-rw-rw-r--   0 tsawicki  (1000) tsawicki  (1000)     8283 2023-03-02 02:19:36.000000 fluvii-1.1.0/fluvii/apps/transactions/transaction.py
+drwxrwxr-x   0 tsawicki  (1000) tsawicki  (1000)        0 2023-04-05 19:36:23.339592 fluvii-1.1.0/fluvii/cli/
+-rw-rw-r--   0 tsawicki  (1000) tsawicki  (1000)        0 2023-02-24 19:18:17.000000 fluvii-1.1.0/fluvii/cli/__init__.py
+-rw-rw-r--   0 tsawicki  (1000) tsawicki  (1000)       88 2023-01-09 19:04:10.000000 fluvii-1.1.0/fluvii/cli/__main__.py
+drwxrwxr-x   0 tsawicki  (1000) tsawicki  (1000)        0 2023-04-05 19:36:23.339592 fluvii-1.1.0/fluvii/cli/commands/
+-rw-rw-r--   0 tsawicki  (1000) tsawicki  (1000)       62 2023-01-09 19:04:10.000000 fluvii-1.1.0/fluvii/cli/commands/__init__.py
+-rw-rw-r--   0 tsawicki  (1000) tsawicki  (1000)      122 2023-01-09 19:04:10.000000 fluvii-1.1.0/fluvii/cli/commands/base.py
+-rw-rw-r--   0 tsawicki  (1000) tsawicki  (1000)     4346 2023-04-05 19:30:52.000000 fluvii-1.1.0/fluvii/cli/commands/topics.py
+drwxrwxr-x   0 tsawicki  (1000) tsawicki  (1000)        0 2023-04-05 19:36:23.339592 fluvii-1.1.0/fluvii/components/
+-rw-rw-r--   0 tsawicki  (1000) tsawicki  (1000)      208 2023-02-24 19:18:17.000000 fluvii-1.1.0/fluvii/components/__init__.py
+drwxrwxr-x   0 tsawicki  (1000) tsawicki  (1000)        0 2023-04-05 19:36:23.339592 fluvii-1.1.0/fluvii/components/admin/
+-rw-rw-r--   0 tsawicki  (1000) tsawicki  (1000)       57 2023-02-24 19:18:17.000000 fluvii-1.1.0/fluvii/components/admin/__init__.py
+-rw-rw-r--   0 tsawicki  (1000) tsawicki  (1000)      507 2023-02-24 19:18:17.000000 fluvii-1.1.0/fluvii/components/admin/admin.py
+-rw-rw-r--   0 tsawicki  (1000) tsawicki  (1000)      766 2023-02-24 19:18:17.000000 fluvii-1.1.0/fluvii/components/admin/config.py
+drwxrwxr-x   0 tsawicki  (1000) tsawicki  (1000)        0 2023-04-05 19:36:23.339592 fluvii-1.1.0/fluvii/components/auth/
+-rw-rw-r--   0 tsawicki  (1000) tsawicki  (1000)       59 2023-02-24 19:18:17.000000 fluvii-1.1.0/fluvii/components/auth/__init__.py
+-rw-rw-r--   0 tsawicki  (1000) tsawicki  (1000)     2012 2023-03-03 01:05:42.000000 fluvii-1.1.0/fluvii/components/auth/config.py
+drwxrwxr-x   0 tsawicki  (1000) tsawicki  (1000)        0 2023-04-05 19:36:23.343592 fluvii-1.1.0/fluvii/components/consumer/
+-rw-rw-r--   0 tsawicki  (1000) tsawicki  (1000)      112 2023-02-24 19:18:17.000000 fluvii-1.1.0/fluvii/components/consumer/__init__.py
+-rw-rw-r--   0 tsawicki  (1000) tsawicki  (1000)     2390 2023-03-02 02:19:36.000000 fluvii-1.1.0/fluvii/components/consumer/config.py
+-rw-rw-r--   0 tsawicki  (1000) tsawicki  (1000)     5449 2023-02-24 20:59:37.000000 fluvii-1.1.0/fluvii/components/consumer/consumer.py
+-rw-rw-r--   0 tsawicki  (1000) tsawicki  (1000)     2764 2023-03-02 02:19:36.000000 fluvii-1.1.0/fluvii/components/consumer/consumer_factory.py
+drwxrwxr-x   0 tsawicki  (1000) tsawicki  (1000)        0 2023-04-05 19:36:23.343592 fluvii-1.1.0/fluvii/components/metrics/
+-rw-rw-r--   0 tsawicki  (1000) tsawicki  (1000)      113 2023-02-24 19:18:17.000000 fluvii-1.1.0/fluvii/components/metrics/__init__.py
+drwxrwxr-x   0 tsawicki  (1000) tsawicki  (1000)        0 2023-04-05 19:36:23.343592 fluvii-1.1.0/fluvii/components/metrics/manager/
+-rw-rw-r--   0 tsawicki  (1000) tsawicki  (1000)       85 2023-02-24 19:18:17.000000 fluvii-1.1.0/fluvii/components/metrics/manager/__init__.py
+-rw-rw-r--   0 tsawicki  (1000) tsawicki  (1000)      290 2023-03-02 02:19:36.000000 fluvii-1.1.0/fluvii/components/metrics/manager/config.py
+-rw-rw-r--   0 tsawicki  (1000) tsawicki  (1000)     3965 2023-03-02 02:19:36.000000 fluvii-1.1.0/fluvii/components/metrics/manager/metrics_manager.py
+drwxrwxr-x   0 tsawicki  (1000) tsawicki  (1000)        0 2023-04-05 19:36:23.343592 fluvii-1.1.0/fluvii/components/metrics/pusher/
+-rw-rw-r--   0 tsawicki  (1000) tsawicki  (1000)       82 2023-02-24 19:18:17.000000 fluvii-1.1.0/fluvii/components/metrics/pusher/__init__.py
+-rw-rw-r--   0 tsawicki  (1000) tsawicki  (1000)      402 2023-02-24 19:18:17.000000 fluvii-1.1.0/fluvii/components/metrics/pusher/config.py
+-rw-rw-r--   0 tsawicki  (1000) tsawicki  (1000)     2586 2023-02-24 19:18:17.000000 fluvii-1.1.0/fluvii/components/metrics/pusher/metrics_pusher.py
+drwxrwxr-x   0 tsawicki  (1000) tsawicki  (1000)        0 2023-04-05 19:36:23.343592 fluvii-1.1.0/fluvii/components/producer/
+-rw-rw-r--   0 tsawicki  (1000) tsawicki  (1000)      112 2023-02-24 19:18:17.000000 fluvii-1.1.0/fluvii/components/producer/__init__.py
+-rw-rw-r--   0 tsawicki  (1000) tsawicki  (1000)      953 2023-02-24 19:18:17.000000 fluvii-1.1.0/fluvii/components/producer/config.py
+-rw-rw-r--   0 tsawicki  (1000) tsawicki  (1000)     8971 2023-02-24 19:18:17.000000 fluvii-1.1.0/fluvii/components/producer/producer.py
+-rw-rw-r--   0 tsawicki  (1000) tsawicki  (1000)     2495 2023-03-02 02:19:36.000000 fluvii-1.1.0/fluvii/components/producer/producer_factory.py
+drwxrwxr-x   0 tsawicki  (1000) tsawicki  (1000)        0 2023-04-05 19:36:23.343592 fluvii-1.1.0/fluvii/components/schema_registry/
+-rw-rw-r--   0 tsawicki  (1000) tsawicki  (1000)       85 2023-02-24 19:18:17.000000 fluvii-1.1.0/fluvii/components/schema_registry/__init__.py
+-rw-rw-r--   0 tsawicki  (1000) tsawicki  (1000)      480 2023-02-24 19:18:17.000000 fluvii-1.1.0/fluvii/components/schema_registry/config.py
+-rw-rw-r--   0 tsawicki  (1000) tsawicki  (1000)     1891 2023-04-05 19:30:52.000000 fluvii-1.1.0/fluvii/components/schema_registry/schema_registry.py
+drwxrwxr-x   0 tsawicki  (1000) tsawicki  (1000)        0 2023-04-05 19:36:23.343592 fluvii-1.1.0/fluvii/components/sqlite/
+-rw-rw-r--   0 tsawicki  (1000) tsawicki  (1000)       66 2023-02-24 19:18:17.000000 fluvii-1.1.0/fluvii/components/sqlite/__init__.py
+-rw-rw-r--   0 tsawicki  (1000) tsawicki  (1000)      326 2023-02-24 19:18:17.000000 fluvii-1.1.0/fluvii/components/sqlite/config.py
+-rw-rw-r--   0 tsawicki  (1000) tsawicki  (1000)     6136 2023-02-24 19:18:17.000000 fluvii-1.1.0/fluvii/components/sqlite/sqlite.py
+-rw-rw-r--   0 tsawicki  (1000) tsawicki  (1000)      653 2023-02-24 19:18:17.000000 fluvii-1.1.0/fluvii/config_bases.py
+-rw-rw-r--   0 tsawicki  (1000) tsawicki  (1000)     2963 2022-11-28 17:26:51.000000 fluvii-1.1.0/fluvii/exceptions.py
+-rw-rw-r--   0 tsawicki  (1000) tsawicki  (1000)      927 2023-02-24 19:18:17.000000 fluvii-1.1.0/fluvii/general_utils.py
+drwxrwxr-x   0 tsawicki  (1000) tsawicki  (1000)        0 2023-04-05 19:36:23.343592 fluvii-1.1.0/fluvii/kafka_tools/
+-rw-rw-r--   0 tsawicki  (1000) tsawicki  (1000)       42 2023-02-24 19:18:17.000000 fluvii-1.1.0/fluvii/kafka_tools/__init__.py
+-rw-rw-r--   0 tsawicki  (1000) tsawicki  (1000)    10609 2023-04-05 19:30:52.000000 fluvii-1.1.0/fluvii/kafka_tools/fluvii_toolbox.py
+-rw-rw-r--   0 tsawicki  (1000) tsawicki  (1000)     4398 2023-03-02 02:19:36.000000 fluvii-1.1.0/fluvii/kafka_tools/topic_dumper.py
+-rw-rw-r--   0 tsawicki  (1000) tsawicki  (1000)      745 2023-02-14 17:34:34.000000 fluvii-1.1.0/fluvii/logging_utils.py
+drwxrwxr-x   0 tsawicki  (1000) tsawicki  (1000)        0 2023-04-05 19:36:23.339592 fluvii-1.1.0/fluvii.egg-info/
+-rw-rw-r--   0 tsawicki  (1000) tsawicki  (1000)      400 2023-04-05 19:36:23.000000 fluvii-1.1.0/fluvii.egg-info/PKG-INFO
+-rw-rw-r--   0 tsawicki  (1000) tsawicki  (1000)     2284 2023-04-05 19:36:23.000000 fluvii-1.1.0/fluvii.egg-info/SOURCES.txt
+-rw-rw-r--   0 tsawicki  (1000) tsawicki  (1000)        1 2023-04-05 19:36:23.000000 fluvii-1.1.0/fluvii.egg-info/dependency_links.txt
+-rw-rw-r--   0 tsawicki  (1000) tsawicki  (1000)       59 2023-04-05 19:36:23.000000 fluvii-1.1.0/fluvii.egg-info/entry_points.txt
+-rw-rw-r--   0 tsawicki  (1000) tsawicki  (1000)      277 2023-04-05 19:36:23.000000 fluvii-1.1.0/fluvii.egg-info/requires.txt
+-rw-rw-r--   0 tsawicki  (1000) tsawicki  (1000)       13 2023-04-05 19:36:23.000000 fluvii-1.1.0/fluvii.egg-info/top_level.txt
+-rw-rw-r--   0 tsawicki  (1000) tsawicki  (1000)      340 2023-02-24 19:18:17.000000 fluvii-1.1.0/pyproject.toml
+-rw-rw-r--   0 tsawicki  (1000) tsawicki  (1000)       38 2023-04-05 19:36:23.343592 fluvii-1.1.0/setup.cfg
+-rw-rw-r--   0 tsawicki  (1000) tsawicki  (1000)      995 2023-04-05 19:36:14.000000 fluvii-1.1.0/setup.py
+drwxrwxr-x   0 tsawicki  (1000) tsawicki  (1000)        0 2023-04-05 19:36:23.343592 fluvii-1.1.0/tests/
+-rw-rw-r--   0 tsawicki  (1000) tsawicki  (1000)        0 2022-11-28 17:26:51.000000 fluvii-1.1.0/tests/__init__.py
+drwxrwxr-x   0 tsawicki  (1000) tsawicki  (1000)        0 2023-04-05 19:36:23.343592 fluvii-1.1.0/tests/temp_integration/
+-rw-rw-r--   0 tsawicki  (1000) tsawicki  (1000)        0 2023-02-24 19:18:17.000000 fluvii-1.1.0/tests/temp_integration/__init__.py
+-rw-rw-r--   0 tsawicki  (1000) tsawicki  (1000)     4465 2023-02-24 19:18:17.000000 fluvii-1.1.0/tests/temp_integration/integration.py
+drwxrwxr-x   0 tsawicki  (1000) tsawicki  (1000)        0 2023-04-05 19:36:23.343592 fluvii-1.1.0/tests/unit/
+-rw-rw-r--   0 tsawicki  (1000) tsawicki  (1000)        0 2022-10-12 22:34:27.000000 fluvii-1.1.0/tests/unit/__init__.py
+-rw-rw-r--   0 tsawicki  (1000) tsawicki  (1000)      849 2023-03-02 02:19:36.000000 fluvii-1.1.0/tests/unit/test_consumer.py
+-rw-rw-r--   0 tsawicki  (1000) tsawicki  (1000)     1242 2023-03-02 02:19:36.000000 fluvii-1.1.0/tests/unit/test_consumer_config.py
+-rw-rw-r--   0 tsawicki  (1000) tsawicki  (1000)      269 2023-03-02 02:19:36.000000 fluvii-1.1.0/tests/unit/test_producer_config.py
```

### Comparing `fluvii-1.0.2/LICENSE` & `fluvii-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fluvii-1.0.2/README.md` & `fluvii-1.1.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -25,49 +25,23 @@
 
 `pip install fluvii`
 
 # What is _Fluvii_?
 
 _Fluvii_ is a Kafka client library built on top of [confluent-kafka-python](https://github.com/confluentinc/confluent-kafka-python).
 
-_Fluvii_ was originally written as a simpler alternative for the other popular Python client library [Faust](https://github.com/robinhood/faust).
-
-Much like Faust, _Fluvii_ offers _similar_ functionality to the Kafka-Streams java client;
-it's likely no surpise that "Fluvii" translates to "streams" in Latin!
+_Fluvii_ offers _similar_ functionality to the Kafka-Streams java client; it's likely no surpise that "Fluvii" translates to "streams" in Latin!
 
 We like to think of _Fluvii_ as a simplified kafka-streams; it was designed to make Exactly Once Semantics (aka transactions)
-and basic state storage (aka "tabling") require as little code as possible.
+and basic state storage (aka "tabling") as streamlined as possible via its elegant transaction interface.
 
 **We also take full advantage of transactions by handling multiple consumed/produced messages at once per transaction,
 significantly cutting down on I/O, which can tremendously improve throughput!**
 
-See below for further elaborations on _Fluvii_'s use-cases.
-
-## _Fluvii_ or Faust?
-
-We designed _Fluvii_ after using Faust/Kafka extensively; we found that in most cases, we didn't
-need most of the functionality provided by Faust to accomplish 95% of our work. We imagine this will be true for you, too!
-
-As such, we wanted an interface that required minimal interaction/repetition,
-yet offered the ability to easily extend it (or manually handle anything) when needed.
-
-The main reason we wrote _Fluvii_ was to replace Faust, for a few reasons:
-1. Faust is more monolithic in design:
-   1. It's very much its own orchestrator via agents, which if you use your own orchestrator (like Kubernetes), it creates unneccesary redundancy and complexity.
-   2. To help enable this orchestration, Faust is `async`, making it difficult to debug and extend.
-2. Faust is fairly bloated; it was likely designed to easily integrate with other existing event systems at Robinhood.
-3. The original project (and supporting libraries) have been dead for a long time. There are [other forks](https://github.com/faust-streaming/faust) being maintained, but when you combine the above points, we felt it prudent to design something new!
-
-All that being said, you might still choose Faust if:
-
-1. You prefer how Faust operates as an orchestrator, managing kafka clients via workers and agents.
-2. You have a beefy server to run it on...it may perform faster overall than a bunch of `Fluvii` apps.
-3. You're happy with the current feature set Faust offers, which is arguably a little larger than _Fluvii_ since it has rolling table windows.
-4. You want a fairly flexible interface and configuration options, _Fluvii_ is still maturing in this regard.
-5. You want a testing framework; Faust has a built-in testing framework...it's not fool-proof, but it's useful.
+See the bottom of the README for further elaborations on _Fluvii_ vs Faust if that's where you're coming from.
 
 ## Operational Assumptions of _Fluvii_
 
 _Fluvii_ assumes/defaults to:
 
 - Using a schema-registry
 - Using avro schemas (see examples for format)
@@ -79,154 +53,144 @@
 - Using Prometheus metrics (and a push-gateway for app metrics); **the metrics are turned off by default.**
 - Using Sqlite as your table database (which also changes the table storage point above)
 - Using SASL, Oauth, or nothing as your authentication scheme
 
 
 # Getting started with _Fluvii_
 
+Here, we will give you a brief overview of all the major pieces you should be aware of when writing
+an application with _Fluvii_. It will make your exploration much smoother!
+
+We recommend copying the example `FluviiApp` we have further down in the README and follow along with that, as
+most of this will make a lot of sense when viewed alongside it.
 
 ## Understanding `*Factory` classes
-In general, you'll be using "Factory" classes, which will generate the objects you will interface with.
+In general, you'll start with a "Factory" class, which will generate the final object that starts your application!
 
-They basically encapsulate the configuration step of their respective non-factory object;
+These basically encapsulate the configuration step of their respective object;
 i.e. `FluviiAppFactory` helps generate a fully-configured `FluviiApp` instance.
 
 The main ones to focus on would be:
 - `FluviiAppFactory`
 - `FluviiTableAppFactory`
 - `ProducerFactory`
 
-(Note: though `ConsumerFactory` exists, we generally recommend using a `FluviiAppFactory` instead, which uses transactions)
+(Note: though `ConsumerFactory` exists, we generally recommend using a `FluviiAppFactory` instead, which uses transactions).
 
 If you are only producing messages, the producer factory is probably the cleanest way to go, else you'll likely want
 to use one of the `FluviiApp*` factories.
 
 TL;DR `FluviiAppFactory` will likely be your one-stop shop, which makes a `FluviiApp` for you!
 
 ## Understanding "Components"
 
-_Fluvii_ comprises several classes that work in tandem. Some classes are referred to as "components",
-which `FluviiApp`'s coordinate and orchestrate (and some work as stand-alones, like the `Producer`). These include
+_Fluvii_ comprises several classes that work in tandem, which `FluviiApp`'s coordinate and orchestrate for you
+(and some work as stand-alones, like the `Producer`). These classes are referred to as "components".
+
+These include things like:
 - SchemaRegistry
-- MetricsManager/Pusher
 - Producer
 - Consumer
 
 One good rule of thumb for components is that they have a corresponding `config.py` to...well, configure them!
 
-For the most part, you won't have to mess with any of these directly if you use the `*Factory` classes, which will generate all
-the necessary components and their respective config objects for you! But, it's good to be aware of their existence.
+In general, you only need to be aware of them for configuration purposes and should not need to interface with them at all.
 
-## `Transaction` objects
+## `Transaction` objects - your primary application interface
 
-**`Transaction`s will be the object your application logic interfaces with for producing and handling messages while using any `FluviiApp` variant**.
+**`Transaction`s will be the object your `FluviiApp` application logic interfaces with for producing and handling messages**.
+The object's state will be managed for you under the hood!
 
-It is aptly named because the object is very much the equivalent of a Kafka transaction, and it gets recreated each time
-a new transaction is required.
+It is aptly named as the object is very much the equivalent of a Kafka transaction in terms of operation and lifecycle.
 
 You will see how this applies in the **Creating a FluviiApp** section below.
 
-Note that the state of said transaction is managed behind the scenes by the `FluviiApp`, you don't have to manage it yourself.
+### Using the `Transaction` object - some examples:
+Usually, your calls on the object will be as simple as:
+
+- Accessing the consumed message properties like key or value via `transaction.key() or .value()`
+- Produce messages via `transaction.produce(key/value/header args here)`
+- Read or update the message key table entry via `transaction.read_table_entry() or .update_table_entry()`
 
 
-# Creating a FluviiApp (via a Factory)
 
-A `FluviiApp` is any of the `*_app.py` file names located in the library folder `/fluvii/apps`.
+# Creating a FluviiApp (via a Factory)
 
 As previously mentioned, `FluviiApp`s have a corresponding `Factory` associated with them; we will outline their usage below.
 
-## `*Factory` args
-Here are the basic arguments when it comes to creating a `FluviiApp` (through a `*Factory`)
+For more details around configuring in general, see the **Configuring _Fluvii_** section further below.
 
-### Args without defaults (aka direct setup)
 
-- `app_function` (arg0)
-  - This is where you hand in your business logic function. See the **Setting up your app_function** section below
-- `consume_topics_list` (arg1)
-  - The topics you want to consume from
-- `produce_topic_schema_dict` (optional kwarg)
-  - Optionally, the topics (and respective schema) you may produce to in the app.
+### `*Factory` Required Arguments
 
-### Args with defaults - `*_config` args (aka indirect setup)
-Any arguments that end in `_config` are optional in that they generally have working defaults.
+1. `app_function` (arg0)
+   - This is where you hand in your business logic function. See the **Setting up your app_function** section below
+2. `consume_topics_list` (arg1)
+   - The topics you want to consume from
+3. `produce_topic_schema_dict` (optional kwarg)
+   - Optionally, the topics (and its respective avro schema) you may produce to in the app.
 
-Additionally, they are considered "indirect" because they can be set via the environment rather than using the factory argument.
 
-This somewhat artificial deliniation was made because these settings are far less likely to change between
-different application instances (among other design reasons).
+### `*Factory` Arguments with Working Defaults
+- Any arguments that end in `_config` are optional in that they generally have working defaults (and can be set via environment).
 
-Note: any configs that are manually handed here supercede any environment configurations.
+- These settings are far less likely to change between different application instances.
 
-For more details, see the **Configuring _Fluvii_** section.
 
 ## Setting up your app_function
 The `app_function` you pass to Fluvii is the heart of your application.
 
-Typically, you consume a message and do "logic n' stuff", which could include producing new messages. This function encapsulates all of that.
+Typically, you consume a message and then "do stuff", like process/transform a message value and then produce the result downstream.
+
+This is your "do stuff" part!
 
-Some notes:
-- By default, the function MUST take at minimum 1 argument, of which the first will be an injection of a `Transaction` object instance at runtime. For example,
+By default, your function MUST take at minimum 1 argument, of which the first will be an injection of a `Transaction` object instance at runtime. For example,
    ```python
    def my_app_function(transaction, my_arg, my_arg2):
       pass # do stuff; using the transaction object throughout
    ```
-- You can access the currently consumed message via `transaction.message`, or shorthand via `transaction.key()`
-- You can produce messages via `transaction.produce(ARGS_HERE)`
-- once the app runs through the entirety of your app_function, it will commit the current message and apply the function to the next message...and so on.
 
-# Configuring _Fluvii_
+This is the function that runs in a loop forever once you call `FluviiApp.run()`.
 
-_Fluvii_ allows you to configure its various components via environment (or directly via the config
-object itself).
+# Configuring _Fluvii_
 
-`FluviiApp`s also have an associated config object.
+_Fluvii_ is configured through its various components (including a `FluviiAppConfig`).
 
 These component configs (i.e. any `config.py`) typically have working defaults for most of their settings, and most
 of them will not need any additional tweaking.
 
-## Configuration options
-1. Component config handed to a `*Factory` argument.
-   - An (incomplete) example of this might look like:
-       ```python
-       app = FluviiAppFactory(consumer_config=ConsumerConfig(timeout_minutes=10))
-       ```
-2. With environment variables
+## Configuration Approaches
+
+1. \[RECOMMENDED] With environment variables
     - In general, this is the reccommended approach.
     - You can look at each config object, with defines a prefix. For any given config value, just prepend the prefix to said value.
     - For example, with `ConsumerConfig`:
       - its prefix is `FLUVII_CONSUMER_`.
       - It has a setting called `timeout_minutes`.
       - Then the respective environment variable for this setting is `FLUVII_CONSUMER_TIMEOUT_MINUTES`
 
-3. With a `.env` file, where the environment variable `FLUVII_CONFIG_DOTENV` is the filepath to it
+
+2. With a `.env` file, where the environment variable `FLUVII_CONFIG_DOTENV` is the filepath to the `.env`
     - This approach uses the same setting naming scheme as in (2.)
     - An (incomplete) example might look like:
         ```dotenv
         FLUVII_CONSUMER_TIMEOUT_MINUTES=10
         FLUVII_AUTH_KAFKA_USERNAME=my_cool_username
         ```
 
-## Configuration precedence
-
-Under the hood, Fluvii uses `Pydantic`, and as such, follows its rules for configuration precedence for each config value.
-
-Do note that the configs only populate with actual defined values at each step, so non-defined values won't overwrite
-previously defined ones unless you specifically define them to be empty.
-
-Here's the order from highest precedence to lowest (higher supercedes anything below it):
+3. Component config handed to a `*Factory` argument.
+   - An (incomplete) example of this might look like:
+       ```python
+       app = FluviiAppFactory(consumer_config=ConsumerConfig(timeout_minutes=10))
 
-1. config object with direct arguments handed to a Factory
-2. environment variable
-3. dotenv file
 
-## Minimum configuration requirements
+## Minimum Configuration Requirements
 
-No matter what, you will need to populate these configuration settings:
+You will need to populate these configuration settings for any `FluviiApp`:
 
-### FluviiApp
 ```dotenv
 ### Connection
 # Kafka Consumer/Producer
 FLUVII_PRODUCER_URLS=
 FLUVII_CONSUMER_URLS=
 # Schema Registry
 FLUVII_SCHEMA_REGISTRY_URL=
@@ -239,56 +203,87 @@
 FLUVII_AUTH_KAFKA_USERNAME=
 FLUVII_AUTH_KAFKA_PASSWORD=
 # Schema Registry
 FLUVII_SCHEMA_REGISTRY_USERNAME=
 FLUVII_SCHEMA_REGISTRY_PASSWORD=
 ```
 
-## Other configuration suggestions
+### FYI - Configuration precedence
+
+Under the hood, Fluvii uses `Pydantic`, and thus follows its rules for configuration precedence for each config value.
+
+Do note that the configs only populate with actual defined values at each step, so non-defined values won't overwrite
+previously defined ones unless you specifically define them to be empty.
+
+Here's the order from highest precedence to lowest (higher supercedes anything below it):
+
+1. config object with direct arguments handed to a Factory
+2. environment variable
+3. dotenv file
+
+
+### FYI - Other configuration suggestions
 
 In general, we recommend using the environment variable configuration approach.
 
 There is also a `FLUVII_APP_HOSTNAME` which we suggest setting to your kubernetes pod hostname, but it's not required.
 
 
 # Simple FluviiApp Examples
 
-## Initializing/running a bare-bones `FluviiApp`:
+Note: all these examples assume the kafka topics already exist.
 
-Note: This example assumes you have set the few required config settings via environment variables.
-You can find a manual configuration example further below.
+## Initializing/running a bare-bones `FluviiProducer` (required environment variables already set):
 
-There are two basic components you need to initialize an app at all:
+Here's a simple looping producer app.
 
-- `app_function` (first arg): the logic of your application, of which the first argument (which MUST exist) is assumed to be a transaction object that will be handed to it at runtime. Additional arguments, if needed, can be handed to `app_function_arglist`.
+Feel free to combine this with the next example to easily explore the functionality of Fluvii!
 
-- `consume_topics_list` (second arg): the topics you are consuming. Can be comma-separated string or python list.
+```python
+from fluvii.components.producer import ProducerFactory
+from time import sleep
 
-That's it! That being said, this is if your app only consumes. To produce, you will additionally need, at minimum:
+a_cool_schema = {
+    "name": "CoolSchema",
+    "type": "record",
+    "fields": [
+        {
+            "name": "cool_field",
+            "type": "string",
+            "default": ""
+        }
+    ]
+}
 
-- `produce_topic_schema_dict`: a dict that maps {'topic_name': _schema_obj_}, where the _schema_obj_ is a valid avro
-schema.
+producer = ProducerFactory(topic_schema_dict={"test_topic_a": a_cool_schema})
 
-Then, to run the app, do:
+try:
+    while True:
+        producer.produce({"cool_field": "test_value"}, key="my_key", topic="test_topic_a")
+        sleep(5)
+finally:
+    producer.close()
+```
 
-`FluviiApp.run()`
+## Initializing/running a bare-bones `FluviiApp` (required environment variables already set):
 
-Altogether, that might look something like this:
+For more details in terms of how this works, see "Configuring a `FluviiApp`" above!
 
 ```python
 from fluvii import FluviiAppFactory
 
 # assume the message consumed also had this schema to make it easy
 a_cool_schema = {
     "name": "CoolSchema",
     "type": "record",
     "fields": [
         {
             "name": "cool_field",
-            "type": "string"
+            "type": "string",
+            "default": "",
         }
     ]
 }
 
 # can hand off objects you'd like to init separately, like an api session object, or a heavy object built at runtime
 heavy_thing_inited_at_runtime = 'heavy thing'
 
@@ -303,35 +298,17 @@
     )
 
 fluvii_app = FluviiAppFactory(
     my_app_logic,
     ['test_topic_a', 'test_topic_b'],
     produce_topic_schema_dict={'cool_topic_out': a_cool_schema},
     app_function_arglist = [heavy_thing_inited_at_runtime])  # optional! Here to show functionality.
-fluvii_app.run()
-```
-If you're feeling really lazy, you can actually cut some the `transaction.produce()` dict arguments, as anything you
-don't pass (except `partition`) will be inhereted from the consumed message, like so:
-
-```python
-## will produce with the consumed message's key and headers
-transaction.produce({'value': cool_message_out, 'topic': 'cool_topic_out'}
-)
-```
-
-For maximum laziness,you could also cut the dict out entirely if there was only 1 topic in the `produce_topic_schema_dict`, as it will assume that's the topic
-you want to produce to, like so:
-
-```python
-## will produce with the consumed message's key and headers
-transaction.produce(cool_message_out)
+fluvii_app.run()  # once you call .run(), 'my_app_logic' runs until you explicitly kill the app!
 ```
 
-Just make sure your message value isn't itself a dictionary with a "value" key in this case =)
-
 ## Using a table with a `FluviiTableApp`
 
 Using tabling via `FLuviiTableApp` is very simple.
 
 Here is an example where we are consuming messages around purchases made by various account holders,
 storing the new balance for later comparisons, and producing that remaining balance downstream (maybe to notify the account holder?).
 
@@ -343,26 +320,26 @@
 from fluvii import FluviiTableAppFactory
 
 # -- Not used here, just so you know what the consumed messages look like
 # purchase_schema = {
 #     "name": "AccountPurchase",
 #     "type": "record",
 #     "fields": [
-#         {"name": "Account Number", "type": "string"},
-#         {"name": "Purchase Timestamp", "type": "string"},
-#         {"name": "Purchase Amount", "type": "string"},
+#         {"name": "Account Number", "type": "string", "default": ""},
+#         {"name": "Purchase Timestamp", "type": "string", "default": ""},
+#         {"name": "Purchase Amount", "type": "string", "default": ""},
 #     ]
 # }
 
 account_balance_schema = {
     "name": "AccountBalance",
     "type": "record",
     "fields": [
-        {"name": "Account Number", "type": "string"},
-        {"name": "Account Balance", "type": "string"},
+        {"name": "Account Number", "type": "string", "default": ""},
+        {"name": "Account Balance", "type": "string", "default": ""},
     ]
 }
 
 def my_app_logic(transaction):
     record = transaction.value()
     current_account_balance = float(transaction.read_table_entry()['balance'])  # looks up record via the message.key()
     purchase_amount = float(record['Purchase Amount'])
@@ -398,31 +375,42 @@
     FluviiAppConfig,
     ProducerConfig,
     ConsumerConfig,
     AuthKafkaConfig,
     SchemaRegistryConfig
 )
 
-my_schema = 'your schema here'
+a_cool_schema = {
+    "name": "CoolSchema",
+    "type": "record",
+    "fields": [
+        {
+            "name": "cool_field",
+            "type": "string",
+            "default": "",
+        }
+    ]
+}
+
 
 def my_business_logic(transaction):
     pass # do stuff to messages
 
 
 def my_fluvii_app():
     auth_kafka_kws = {
         'urls': 'my.broker.url0,my.broker.url1',
-        'auth_kafka_config': AuthKafkaConfig(username='my_kafka_un', password='my_kafka_pw')
+        'auth_config': AuthKafkaConfig(username='my_kafka_un', password='my_kafka_pw')
     }
     return FluviiAppFactory(
         my_business_logic,
-        ['my_input_topic'],
-        produce_topic_schema_dict={'my_output_topic': my_schema},
-        fluvii_config=FluviiAppConfig(app_name='my_fluvii_app'),
-        schema_registry_config=SchemaRegistryConfig(url='my.sr.url', username='my_sr_un', password='my_sr_pw'),
+        ['my_input_topic_name'],
+        produce_topic_schema_dict={'my_output_topic_name': a_cool_schema},
+        fluvii_config=FluviiAppConfig(name='my_fluvii_app'),
+        schema_registry_config=SchemaRegistryConfig(url='https://my.sr.url', username='my_sr_un', password='my_sr_pw'),
         consumer_config=ConsumerConfig(**auth_kafka_kws, timeout_minutes=10),
         producer_config=ProducerConfig(**auth_kafka_kws),
     )
 
 
 if __name__ == '__main__':
     app = my_fluvii_app()
@@ -638,19 +626,64 @@
 
 If you need more manual access to things, the `TransactionalConsumer`, `TransactionalProducer`, and the `FluviiApp` context is
 passed to every transaction object, so you'll always have access to whatever objects you need should the need arise.
 
 You can also refresh the transaction object to re-use should it prove difficult to manage your logic
 by remaking the transaction object, but this is certainly a more advanced use-case.
 
+### `transaction` Usage Shortcuts
+
+- If you're feeling really lazy, you can actually cut some the `transaction.produce()` dict arguments, as anything you
+don't pass (except `partition`) will be inhereted from the consumed message, like so:
+
+    ```python
+    ## will produce with the consumed message's key and headers
+    transaction.produce({'value': cool_message_out, 'topic': 'cool_topic_out'}
+    )
+    ```
+
+- For maximum laziness, you could also cut the dict out entirely if there was only 1 topic in the `produce_topic_schema_dict`, as it will assume that's the topic
+you want to produce to, like so:
+
+    ```python
+    ## will produce with the consumed message's key and headers
+    transaction.produce(cool_message_out)
+    ```
+
+    Just make sure your message value isn't itself a dictionary with a "value" key in this case =)
+
+
 ### TableTransaction
 
 `TableTransaction` objects operate very similarly, except you'll need to add two extra commands before committing.
 
 To read an entry, call `transaction.read_table_entry()`, which will return a dict.
 
 To update an entry for the given message key, call `transaction.update_table_entry(my_update_dict)`. Of course, skip this
 if you don't need to update it.
 
 One thing to keep in mind is the object stored in the table just needs to be a valid json (which includes dicts).
 
 Also, `FluviiTableApp` will ensure everything gets committed correctly for you just like the `FluviiApp`!
+
+## _Fluvii_ or Faust?
+
+We designed _Fluvii_ after using Faust/Kafka extensively; we found that in most cases, we didn't
+need most of the functionality provided by Faust to accomplish 95% of our work. We imagine this will be true for you, too!
+
+As such, we wanted an interface that required minimal interaction/repetition,
+yet offered the ability to easily extend it (or manually handle anything) when needed.
+
+The main reason we wrote _Fluvii_ was to replace Faust, for a few reasons:
+1. Faust is more monolithic in design:
+   1. It's very much its own orchestrator via agents, which if you use your own orchestrator (like Kubernetes), it creates unneccesary redundancy and complexity.
+   2. To help enable this orchestration, Faust is `async`, making it difficult to debug and extend.
+2. Faust is fairly bloated; it was likely designed to easily integrate with other existing event systems at Robinhood.
+3. The original project (and supporting libraries) have been dead for a long time. There are [other forks](https://github.com/faust-streaming/faust) being maintained, but when you combine the above points, we felt it prudent to design something new!
+
+All that being said, you might still choose Faust if:
+
+1. You prefer how Faust operates as an orchestrator, managing kafka clients via workers and agents.
+2. You have a beefy server to run it on...it may perform faster overall than a bunch of `Fluvii` apps.
+3. You're happy with the current feature set Faust offers, which is arguably a little larger than _Fluvii_ since it has rolling table windows.
+4. You want a fairly flexible interface and configuration options, _Fluvii_ is still maturing in this regard.
+5. You want a testing framework; Faust has a built-in testing framework...it's not fool-proof, but it's useful.
```

### Comparing `fluvii-1.0.2/fluvii/apps/config.py` & `fluvii-1.1.0/fluvii/apps/config.py`

 * *Files identical despite different names*

### Comparing `fluvii-1.0.2/fluvii/apps/fluvii_app.py` & `fluvii-1.1.0/fluvii/apps/fluvii_app.py`

 * *Files identical despite different names*

### Comparing `fluvii-1.0.2/fluvii/apps/fluvii_multi_msg_app.py` & `fluvii-1.1.0/fluvii/apps/fluvii_multi_msg_app.py`

 * *Files identical despite different names*

### Comparing `fluvii-1.0.2/fluvii/apps/fluvii_table_app.py` & `fluvii-1.1.0/fluvii/apps/fluvii_table_app.py`

 * *Files identical despite different names*

### Comparing `fluvii-1.0.2/fluvii/apps/helpers/app_factory_base.py` & `fluvii-1.1.0/fluvii/apps/helpers/app_factory_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,15 @@
         self._consume_topics_list = consume_topics_list.split(',') if isinstance(consume_topics_list, str) else consume_topics_list
         self._produce_topic_schema_dict = produce_topic_schema_dict if isinstance(produce_topic_schema_dict, dict) else {}
         self.obj_out = self._return_class()
 
     def _make_metrics_manager(self):
         LOGGER.info("Generating the MetricsManager component...")
         if not self._metrics_manager_config:
-            self._metrics_manager_config = MetricsManagerConfig(app_name=self._fluvii_config.name, hostname=self._fluvii_config.hostname)
+            self._metrics_manager_config = self.metrics_config_cls(app_name=self._fluvii_config.name, hostname=self._fluvii_config.hostname)
         if self._metrics_manager_config.enable_metrics:
             return self.metrics_cls(self._metrics_manager_config, auto_start=False)
         return None
 
     def _make_schema_registry(self):
         LOGGER.info("Generating the SchemaRegistry component...")
         return self.registry_cls(self._schema_registry_config, auto_start=False)
```

### Comparing `fluvii-1.0.2/fluvii/apps/helpers/rebalance_manager.py` & `fluvii-1.1.0/fluvii/apps/helpers/rebalance_manager.py`

 * *Files identical despite different names*

### Comparing `fluvii-1.0.2/fluvii/apps/transactions/consumer.py` & `fluvii-1.1.0/fluvii/apps/transactions/consumer.py`

 * *Files identical despite different names*

### Comparing `fluvii-1.0.2/fluvii/apps/transactions/producer.py` & `fluvii-1.1.0/fluvii/apps/transactions/producer.py`

 * *Files identical despite different names*

### Comparing `fluvii-1.0.2/fluvii/apps/transactions/transaction.py` & `fluvii-1.1.0/fluvii/apps/transactions/transaction.py`

 * *Files identical despite different names*

### Comparing `fluvii-1.0.2/fluvii/cli/commands/topics.py` & `fluvii-1.1.0/fluvii/cli/commands/topics.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,22 @@
 import click
 from .base import fluvii_cli
 from fluvii.kafka_tools import FluviiToolbox
 from fluvii.general_utils import parse_headers
 import json
 
 
+def read_from_stdin():
+    if not click.get_text_stream('stdin').isatty():  # means something is getting piped in
+        text_stream = click.get_text_stream('stdin')
+        std_in = text_stream.read()
+        text_stream.flush()
+        return std_in
+
+
 @fluvii_cli.group("topics")
 def topics_group():
     pass
 
 
 @topics_group.command(name="list")
 @click.option("--include-configs", is_flag=True)
@@ -17,32 +25,44 @@
 
 
 @topics_group.command(name="create")
 @click.option("--topic-config-dict", type=str, required=False)
 @click.option("--topic-list", type=str, required=False)
 @click.option("--config-dict", type=str, required=False)
 def create_topics(topic_config_dict, topic_list, config_dict):
+    if std_in := read_from_stdin():
+        topic_config_dict = std_in
     if topic_config_dict:
         topic_config_dict = json.loads(topic_config_dict)
     else:
         if ', ' in topic_list:
             topic_list = topic_list.split(', ')
         else:
             topic_list = topic_list.split(',')
 
         if config_dict:
             config_dict = json.loads(config_dict)
         else:
             click.echo('There were no configs defined; using defaults of {partitions=3, replication.factor=3}')
             config_dict = {'partitions': 3, 'replication.factor': 3}
         topic_config_dict = {topic: config_dict for topic in topic_list}
-    click.echo(f'Creating topics {list(topic_config_dict.keys())}')
+    click.echo(f'Attempting to create topics {list(topic_config_dict.keys())}')
     FluviiToolbox().create_topics(topic_config_dict)
 
 
+@topics_group.command(name="alter")
+@click.option("--topic-config-dict", type=str, required=False)
+def alter_topics(topic_config_dict):
+    if std_in := read_from_stdin():
+        topic_config_dict = std_in
+    topic_config_dict = json.loads(topic_config_dict)
+    click.echo(f'Attempting to alter topic configs for {list(topic_config_dict.keys())}')
+    FluviiToolbox().alter_topics(topic_config_dict)
+
+
 @topics_group.command(name="delete")
 @click.option("--topic-config-dict", type=str, required=False)
 @click.option("--topic-list", type=str, required=False)
 def delete_topics(topic_config_dict, topic_list):
     if topic_list:
         if ', ' in topic_list:
             topic_list = topic_list.split(', ')
@@ -50,14 +70,22 @@
             topic_list = topic_list.split(',')
     else:
         topic_list = list(json.loads(topic_config_dict).keys())
     click.echo(f'Deleting topics {topic_list}')
     FluviiToolbox().delete_topics(topic_list)
 
 
+@topics_group.command(name="sync")
+@click.option("--topic-config-dict", type=str, required=False)
+def sync_topics(topic_config_dict):
+    if std_in := read_from_stdin():
+        topic_config_dict = std_in
+    FluviiToolbox().sync_topics(json.loads(topic_config_dict))
+
+
 @topics_group.command(name="consume")
 @click.option("--topic-offset-dict", type=str, required=True)
 @click.option("--output-filepath", type=click.File("w"), required=True)
 def consume_topics(topic_offset_dict, output_filepath):
     def transform(transaction):
         msgs = [{k: msg.__getattribute__(k)() for k in ['key', 'value', 'headers', 'topic', 'partition', 'offset', 'timestamp']} for msg in transaction.messages()]
         for msg in msgs:
```

### Comparing `fluvii-1.0.2/fluvii/components/admin/config.py` & `fluvii-1.1.0/fluvii/components/admin/config.py`

 * *Files identical despite different names*

### Comparing `fluvii-1.0.2/fluvii/components/auth/config.py` & `fluvii-1.1.0/fluvii/components/auth/config.py`

 * *Files identical despite different names*

### Comparing `fluvii-1.0.2/fluvii/components/consumer/config.py` & `fluvii-1.1.0/fluvii/components/consumer/config.py`

 * *Files identical despite different names*

### Comparing `fluvii-1.0.2/fluvii/components/consumer/consumer.py` & `fluvii-1.1.0/fluvii/components/consumer/consumer.py`

 * *Files identical despite different names*

### Comparing `fluvii-1.0.2/fluvii/components/consumer/consumer_factory.py` & `fluvii-1.1.0/fluvii/components/consumer/consumer_factory.py`

 * *Files identical despite different names*

### Comparing `fluvii-1.0.2/fluvii/components/metrics/manager/metrics_manager.py` & `fluvii-1.1.0/fluvii/components/metrics/manager/metrics_manager.py`

 * *Files identical despite different names*

### Comparing `fluvii-1.0.2/fluvii/components/metrics/pusher/metrics_pusher.py` & `fluvii-1.1.0/fluvii/components/metrics/pusher/metrics_pusher.py`

 * *Files identical despite different names*

### Comparing `fluvii-1.0.2/fluvii/components/producer/config.py` & `fluvii-1.1.0/fluvii/components/producer/config.py`

 * *Files identical despite different names*

### Comparing `fluvii-1.0.2/fluvii/components/producer/producer.py` & `fluvii-1.1.0/fluvii/components/producer/producer.py`

 * *Files identical despite different names*

### Comparing `fluvii-1.0.2/fluvii/components/producer/producer_factory.py` & `fluvii-1.1.0/fluvii/components/producer/producer_factory.py`

 * *Files identical despite different names*

### Comparing `fluvii-1.0.2/fluvii/components/schema_registry/schema_registry.py` & `fluvii-1.1.0/fluvii/components/schema_registry/schema_registry.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,20 +38,17 @@
     def _init_registry(self):
         url = urlparse(self._config.url)
         auth = ''
         if self._config.username and self._config.password:
             auth = f"{quote(self._config.username)}:{quote(self._config.password.get_secret_value())}@"
         scheme = url.scheme
         if scheme:
-            url = url._replace(path=url.netloc, netloc='')
+            url = url._replace(path=f'{url.netloc}{url.path}', netloc='')
         else:
-            if auth:
-                scheme = 'https'
-            else:
-                scheme = 'http'
+            scheme = 'https' if auth else 'http'
         url = url._replace(scheme='')
         self.registry = SchemaRegistryClient({'url': f'{scheme}://{auth}{url.geturl()}'})
         LOGGER.info('Registry client initialized successfully!')
 
     def start(self):
         if not self._started:
             self._init_registry()
```

### Comparing `fluvii-1.0.2/fluvii/components/sqlite/sqlite.py` & `fluvii-1.1.0/fluvii/components/sqlite/sqlite.py`

 * *Files identical despite different names*

### Comparing `fluvii-1.0.2/fluvii/config_bases.py` & `fluvii-1.1.0/fluvii/config_bases.py`

 * *Files identical despite different names*

### Comparing `fluvii-1.0.2/fluvii/exceptions.py` & `fluvii-1.1.0/fluvii/exceptions.py`

 * *Files identical despite different names*

### Comparing `fluvii-1.0.2/fluvii/general_utils.py` & `fluvii-1.1.0/fluvii/general_utils.py`

 * *Files identical despite different names*

### Comparing `fluvii-1.0.2/fluvii/kafka_tools/topic_dumper.py` & `fluvii-1.1.0/fluvii/kafka_tools/topic_dumper.py`

 * *Files identical despite different names*

### Comparing `fluvii-1.0.2/fluvii/logging_utils.py` & `fluvii-1.1.0/fluvii/logging_utils.py`

 * *Files identical despite different names*

### Comparing `fluvii-1.0.2/fluvii.egg-info/SOURCES.txt` & `fluvii-1.1.0/fluvii.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fluvii-1.0.2/setup.py` & `fluvii-1.1.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     "twine",
 ]
 
 packages = setuptools.find_packages()
 
 setuptools.setup(
     name="fluvii",
-    version="1.0.2",
+    version="1.1.0",
     description="A simple Kafka streams implementation in Python using confluent-kafka-python",
     packages=packages,
     install_requires=install_requires,
     dev_requires=dev_requires,
     include_package_data=True,
     extras_require={"dev": dev_requires},
     entry_points={'console_scripts': ['fluvii = fluvii.cli.__main__:fluvii_cli']},
```

### Comparing `fluvii-1.0.2/tests/temp_integration/integration.py` & `fluvii-1.1.0/tests/temp_integration/integration.py`

 * *Files identical despite different names*

### Comparing `fluvii-1.0.2/tests/unit/test_consumer.py` & `fluvii-1.1.0/tests/unit/test_consumer.py`

 * *Files identical despite different names*

### Comparing `fluvii-1.0.2/tests/unit/test_consumer_config.py` & `fluvii-1.1.0/tests/unit/test_consumer_config.py`

 * *Files identical despite different names*

