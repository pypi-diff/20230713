# Comparing `tmp/nubium-utils-4.1.0.post1.tar.gz` & `tmp/nubium-utils-4.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nubium-utils-4.1.0.post1.tar", last modified: Wed Mar 29 15:23:42 2023, max compression
+gzip compressed data, was "nubium-utils-4.2.0.tar", last modified: Wed Apr  5 19:50:44 2023, max compression
```

## Comparing `nubium-utils-4.1.0.post1.tar` & `nubium-utils-4.2.0.tar`

### file list

```diff
@@ -1,92 +1,94 @@
-drwxr-sr-x   0 1003370000 (1003370000) 1003370000        0 2023-03-29 15:23:42.895693 nubium-utils-4.1.0.post1/
--rw-rw-rw-   0 1003370000 (1003370000) 1003370000     1269 2023-03-29 15:23:31.000000 nubium-utils-4.1.0.post1/.gitignore
--rw-rw-rw-   0 1003370000 (1003370000) 1003370000      417 2023-03-29 15:23:31.000000 nubium-utils-4.1.0.post1/.gitlab-ci.yml
--rw-rw-rw-   0 1003370000 (1003370000) 1003370000      313 2023-03-29 15:23:31.000000 nubium-utils-4.1.0.post1/CONTRIBUTING.md
--rw-rw-rw-   0 1003370000 (1003370000) 1003370000       51 2023-03-29 15:23:31.000000 nubium-utils-4.1.0.post1/MANIFEST.in
--rw-r--r--   0 1003370000 (1003370000) 1003370000    17402 2023-03-29 15:23:42.894693 nubium-utils-4.1.0.post1/PKG-INFO
--rw-rw-rw-   0 1003370000 (1003370000) 1003370000    16931 2023-03-29 15:23:31.000000 nubium-utils-4.1.0.post1/README.md
-drwxr-sr-x   0 1003370000 (1003370000) 1003370000        0 2023-03-29 15:23:42.888692 nubium-utils-4.1.0.post1/nubium_utils/
--rw-rw-rw-   0 1003370000 (1003370000) 1003370000      242 2023-03-29 15:23:31.000000 nubium-utils-4.1.0.post1/nubium_utils/__init__.py
-drwxr-sr-x   0 1003370000 (1003370000) 1003370000        0 2023-03-29 15:23:42.889692 nubium-utils-4.1.0.post1/nubium_utils/custom_apps/
--rw-rw-rw-   0 1003370000 (1003370000) 1003370000      260 2023-03-29 15:23:31.000000 nubium-utils-4.1.0.post1/nubium_utils/custom_apps/__init__.py
--rw-rw-rw-   0 1003370000 (1003370000) 1003370000     2935 2023-03-29 15:23:31.000000 nubium-utils-4.1.0.post1/nubium_utils/custom_apps/eloqua_retriever.py
--rw-rw-rw-   0 1003370000 (1003370000) 1003370000     1494 2023-03-29 15:23:31.000000 nubium-utils-4.1.0.post1/nubium_utils/custom_apps/flask_receiver.py
--rw-rw-rw-   0 1003370000 (1003370000) 1003370000      998 2023-03-29 15:23:31.000000 nubium-utils-4.1.0.post1/nubium_utils/custom_apps/rest_bulk_switcher.py
--rw-rw-rw-   0 1003370000 (1003370000) 1003370000     3497 2023-03-29 15:23:31.000000 nubium-utils-4.1.0.post1/nubium_utils/custom_apps/salesforce_retriever.py
--rw-rw-rw-   0 1003370000 (1003370000) 1003370000      504 2023-03-29 15:23:31.000000 nubium-utils-4.1.0.post1/nubium_utils/custom_exceptions.py
--rw-rw-rw-   0 1003370000 (1003370000) 1003370000     4907 2023-03-29 15:23:31.000000 nubium-utils-4.1.0.post1/nubium_utils/dict_manipulator.py
-drwxr-sr-x   0 1003370000 (1003370000) 1003370000        0 2023-03-29 15:23:42.890693 nubium-utils-4.1.0.post1/nubium_utils/eloqua_utils/
--rw-rw-rw-   0 1003370000 (1003370000) 1003370000        0 2023-03-29 15:23:31.000000 nubium-utils-4.1.0.post1/nubium_utils/eloqua_utils/__init__.py
--rw-rw-rw-   0 1003370000 (1003370000) 1003370000     1172 2023-03-29 15:23:31.000000 nubium-utils-4.1.0.post1/nubium_utils/eloqua_utils/timestamps.py
-drwxr-sr-x   0 1003370000 (1003370000) 1003370000        0 2023-03-29 15:23:42.890693 nubium-utils-4.1.0.post1/nubium_utils/fluvii_extensions/
--rw-rw-rw-   0 1003370000 (1003370000) 1003370000        0 2023-03-29 15:23:31.000000 nubium-utils-4.1.0.post1/nubium_utils/fluvii_extensions/__init__.py
-drwxr-sr-x   0 1003370000 (1003370000) 1003370000        0 2023-03-29 15:23:42.890693 nubium-utils-4.1.0.post1/nubium_utils/fluvii_extensions/apps/
--rw-rw-rw-   0 1003370000 (1003370000) 1003370000      192 2023-03-29 15:23:31.000000 nubium-utils-4.1.0.post1/nubium_utils/fluvii_extensions/apps/__init__.py
--rw-rw-rw-   0 1003370000 (1003370000) 1003370000     1727 2023-03-29 15:23:31.000000 nubium-utils-4.1.0.post1/nubium_utils/fluvii_extensions/apps/config.py
--rw-rw-rw-   0 1003370000 (1003370000) 1003370000      846 2023-03-29 15:23:31.000000 nubium-utils-4.1.0.post1/nubium_utils/fluvii_extensions/apps/nubium_app.py
--rw-rw-rw-   0 1003370000 (1003370000) 1003370000      352 2023-03-29 15:23:31.000000 nubium-utils-4.1.0.post1/nubium_utils/fluvii_extensions/apps/nubium_multi_msg_app.py
--rw-rw-rw-   0 1003370000 (1003370000) 1003370000      542 2023-03-29 15:23:31.000000 nubium-utils-4.1.0.post1/nubium_utils/fluvii_extensions/apps/nubium_table_app.py
-drwxr-sr-x   0 1003370000 (1003370000) 1003370000        0 2023-03-29 15:23:42.890693 nubium-utils-4.1.0.post1/nubium_utils/fluvii_extensions/apps/transactions/
--rw-rw-rw-   0 1003370000 (1003370000) 1003370000       67 2023-03-29 15:23:31.000000 nubium-utils-4.1.0.post1/nubium_utils/fluvii_extensions/apps/transactions/__init__.py
--rw-rw-rw-   0 1003370000 (1003370000) 1003370000     3684 2023-03-29 15:23:31.000000 nubium-utils-4.1.0.post1/nubium_utils/fluvii_extensions/apps/transactions/transaction.py
-drwxr-sr-x   0 1003370000 (1003370000) 1003370000        0 2023-03-29 15:23:42.890693 nubium-utils-4.1.0.post1/nubium_utils/fluvii_extensions/components/
--rw-rw-rw-   0 1003370000 (1003370000) 1003370000        0 2023-03-29 15:23:31.000000 nubium-utils-4.1.0.post1/nubium_utils/fluvii_extensions/components/__init__.py
-drwxr-sr-x   0 1003370000 (1003370000) 1003370000        0 2023-03-29 15:23:42.891693 nubium-utils-4.1.0.post1/nubium_utils/fluvii_extensions/components/auth/
--rw-rw-rw-   0 1003370000 (1003370000) 1003370000       42 2023-03-29 15:23:31.000000 nubium-utils-4.1.0.post1/nubium_utils/fluvii_extensions/components/auth/__init__.py
--rw-rw-rw-   0 1003370000 (1003370000) 1003370000      308 2023-03-29 15:23:31.000000 nubium-utils-4.1.0.post1/nubium_utils/fluvii_extensions/components/auth/config.py
-drwxr-sr-x   0 1003370000 (1003370000) 1003370000        0 2023-03-29 15:23:42.891693 nubium-utils-4.1.0.post1/nubium_utils/fluvii_extensions/components/consumer/
--rw-rw-rw-   0 1003370000 (1003370000) 1003370000      130 2023-03-29 15:23:31.000000 nubium-utils-4.1.0.post1/nubium_utils/fluvii_extensions/components/consumer/__init__.py
--rw-rw-rw-   0 1003370000 (1003370000) 1003370000     1695 2023-03-29 15:23:31.000000 nubium-utils-4.1.0.post1/nubium_utils/fluvii_extensions/components/consumer/config.py
--rw-rw-rw-   0 1003370000 (1003370000) 1003370000      976 2023-03-29 15:23:31.000000 nubium-utils-4.1.0.post1/nubium_utils/fluvii_extensions/components/consumer/consumer.py
--rw-rw-rw-   0 1003370000 (1003370000) 1003370000      358 2023-03-29 15:23:31.000000 nubium-utils-4.1.0.post1/nubium_utils/fluvii_extensions/components/consumer/consumer_factory.py
-drwxr-sr-x   0 1003370000 (1003370000) 1003370000        0 2023-03-29 15:23:42.891693 nubium-utils-4.1.0.post1/nubium_utils/fluvii_extensions/components/metrics/
--rw-rw-rw-   0 1003370000 (1003370000) 1003370000       42 2023-03-29 15:23:31.000000 nubium-utils-4.1.0.post1/nubium_utils/fluvii_extensions/components/metrics/__init__.py
-drwxr-sr-x   0 1003370000 (1003370000) 1003370000        0 2023-03-29 15:23:42.891693 nubium-utils-4.1.0.post1/nubium_utils/fluvii_extensions/components/metrics/manager/
--rw-rw-rw-   0 1003370000 (1003370000) 1003370000       50 2023-03-29 15:23:31.000000 nubium-utils-4.1.0.post1/nubium_utils/fluvii_extensions/components/metrics/manager/__init__.py
--rw-rw-rw-   0 1003370000 (1003370000) 1003370000     2321 2023-03-29 15:23:31.000000 nubium-utils-4.1.0.post1/nubium_utils/fluvii_extensions/components/metrics/manager/metrics_manager.py
-drwxr-sr-x   0 1003370000 (1003370000) 1003370000        0 2023-03-29 15:23:42.892693 nubium-utils-4.1.0.post1/nubium_utils/fluvii_extensions/components/metrics/pusher/
--rw-rw-rw-   0 1003370000 (1003370000) 1003370000       46 2023-03-29 15:23:31.000000 nubium-utils-4.1.0.post1/nubium_utils/fluvii_extensions/components/metrics/pusher/__init__.py
--rw-rw-rw-   0 1003370000 (1003370000) 1003370000     1431 2023-03-29 15:23:31.000000 nubium-utils-4.1.0.post1/nubium_utils/fluvii_extensions/components/metrics/pusher/config.py
-drwxr-sr-x   0 1003370000 (1003370000) 1003370000        0 2023-03-29 15:23:42.892693 nubium-utils-4.1.0.post1/nubium_utils/fluvii_extensions/components/producer/
--rw-rw-rw-   0 1003370000 (1003370000) 1003370000       93 2023-03-29 15:23:31.000000 nubium-utils-4.1.0.post1/nubium_utils/fluvii_extensions/components/producer/__init__.py
--rw-rw-rw-   0 1003370000 (1003370000) 1003370000      246 2023-03-29 15:23:31.000000 nubium-utils-4.1.0.post1/nubium_utils/fluvii_extensions/components/producer/config.py
--rw-rw-rw-   0 1003370000 (1003370000) 1003370000      313 2023-03-29 15:23:31.000000 nubium-utils-4.1.0.post1/nubium_utils/fluvii_extensions/components/producer/producer_factory.py
-drwxr-sr-x   0 1003370000 (1003370000) 1003370000        0 2023-03-29 15:23:42.892693 nubium-utils-4.1.0.post1/nubium_utils/fluvii_extensions/components/sqlite/
--rw-rw-rw-   0 1003370000 (1003370000) 1003370000       38 2023-03-29 15:23:31.000000 nubium-utils-4.1.0.post1/nubium_utils/fluvii_extensions/components/sqlite/__init__.py
--rw-rw-rw-   0 1003370000 (1003370000) 1003370000      172 2023-03-29 15:23:31.000000 nubium-utils-4.1.0.post1/nubium_utils/fluvii_extensions/components/sqlite/config.py
--rw-rw-rw-   0 1003370000 (1003370000) 1003370000     1516 2023-03-29 15:23:31.000000 nubium-utils-4.1.0.post1/nubium_utils/general_utils.py
--rw-rw-rw-   0 1003370000 (1003370000) 1003370000      841 2023-03-29 15:23:31.000000 nubium-utils-4.1.0.post1/nubium_utils/hashing_utils.py
-drwxr-sr-x   0 1003370000 (1003370000) 1003370000        0 2023-03-29 15:23:42.893693 nubium-utils-4.1.0.post1/nubium_utils/integration_utils/
--rw-rw-rw-   0 1003370000 (1003370000) 1003370000        0 2023-03-29 15:23:31.000000 nubium-utils-4.1.0.post1/nubium_utils/integration_utils/__init__.py
--rw-rw-rw-   0 1003370000 (1003370000) 1003370000     4009 2023-03-29 15:23:31.000000 nubium-utils-4.1.0.post1/nubium_utils/integration_utils/eloqua_utils.py
--rw-rw-rw-   0 1003370000 (1003370000) 1003370000     3610 2023-03-29 15:23:31.000000 nubium-utils-4.1.0.post1/nubium_utils/integration_utils/new_validation_utils.py
--rw-rw-rw-   0 1003370000 (1003370000) 1003370000     4604 2023-03-29 15:23:31.000000 nubium-utils-4.1.0.post1/nubium_utils/integration_utils/salesforce_utils.py
--rw-rw-rw-   0 1003370000 (1003370000) 1003370000     1202 2023-03-29 15:23:31.000000 nubium-utils-4.1.0.post1/nubium_utils/integration_utils/setup_teardown_utils.py
--rw-rw-rw-   0 1003370000 (1003370000) 1003370000     1876 2023-03-29 15:23:31.000000 nubium-utils-4.1.0.post1/nubium_utils/integration_utils/topic_utils.py
--rw-rw-rw-   0 1003370000 (1003370000) 1003370000     2972 2023-03-29 15:23:31.000000 nubium-utils-4.1.0.post1/nubium_utils/integration_utils/validation_utils.py
-drwxr-sr-x   0 1003370000 (1003370000) 1003370000        0 2023-03-29 15:23:42.893693 nubium-utils-4.1.0.post1/nubium_utils/salesforce_utils/
--rw-rw-rw-   0 1003370000 (1003370000) 1003370000        0 2023-03-29 15:23:31.000000 nubium-utils-4.1.0.post1/nubium_utils/salesforce_utils/__init__.py
--rw-rw-rw-   0 1003370000 (1003370000) 1003370000     2182 2023-03-29 15:23:31.000000 nubium-utils-4.1.0.post1/nubium_utils/salesforce_utils/sessions.py
-drwxr-sr-x   0 1003370000 (1003370000) 1003370000        0 2023-03-29 15:23:42.893693 nubium-utils-4.1.0.post1/nubium_utils/test_utils/
--rw-rw-rw-   0 1003370000 (1003370000) 1003370000       35 2023-03-29 15:23:31.000000 nubium-utils-4.1.0.post1/nubium_utils/test_utils/__init__.py
--rw-rw-rw-   0 1003370000 (1003370000) 1003370000     2364 2023-03-29 15:23:31.000000 nubium-utils-4.1.0.post1/nubium_utils/test_utils/run_app.py
--rw-rw-rw-   0 1003370000 (1003370000) 1003370000     1168 2023-03-29 15:23:31.000000 nubium-utils-4.1.0.post1/nubium_utils/test_utils/test_tools.py
-drwxr-sr-x   0 1003370000 (1003370000) 1003370000        0 2023-03-29 15:23:42.889692 nubium-utils-4.1.0.post1/nubium_utils.egg-info/
--rw-r--r--   0 1003370000 (1003370000) 1003370000    17402 2023-03-29 15:23:42.000000 nubium-utils-4.1.0.post1/nubium_utils.egg-info/PKG-INFO
--rw-r--r--   0 1003370000 (1003370000) 1003370000     2973 2023-03-29 15:23:42.000000 nubium-utils-4.1.0.post1/nubium_utils.egg-info/SOURCES.txt
--rw-r--r--   0 1003370000 (1003370000) 1003370000        1 2023-03-29 15:23:42.000000 nubium-utils-4.1.0.post1/nubium_utils.egg-info/dependency_links.txt
--rw-r--r--   0 1003370000 (1003370000) 1003370000      368 2023-03-29 15:23:42.000000 nubium-utils-4.1.0.post1/nubium_utils.egg-info/requires.txt
--rw-r--r--   0 1003370000 (1003370000) 1003370000       19 2023-03-29 15:23:42.000000 nubium-utils-4.1.0.post1/nubium_utils.egg-info/top_level.txt
--rw-rw-rw-   0 1003370000 (1003370000) 1003370000      764 2023-03-29 15:23:31.000000 nubium-utils-4.1.0.post1/pyproject.toml
--rw-rw-rw-   0 1003370000 (1003370000) 1003370000     3654 2023-03-29 15:23:31.000000 nubium-utils-4.1.0.post1/requirements.txt
--rw-r--r--   0 1003370000 (1003370000) 1003370000       38 2023-03-29 15:23:42.895693 nubium-utils-4.1.0.post1/setup.cfg
--rw-rw-rw-   0 1003370000 (1003370000) 1003370000     1186 2023-03-29 15:23:31.000000 nubium-utils-4.1.0.post1/setup.py
-drwxr-sr-x   0 1003370000 (1003370000) 1003370000        0 2023-03-29 15:23:42.894693 nubium-utils-4.1.0.post1/tests/
--rw-rw-rw-   0 1003370000 (1003370000) 1003370000        0 2023-03-29 15:23:31.000000 nubium-utils-4.1.0.post1/tests/__init__.py
-drwxr-sr-x   0 1003370000 (1003370000) 1003370000        0 2023-03-29 15:23:42.894693 nubium-utils-4.1.0.post1/tests/eloqua_utils/
--rw-rw-rw-   0 1003370000 (1003370000) 1003370000        0 2023-03-29 15:23:31.000000 nubium-utils-4.1.0.post1/tests/eloqua_utils/__init__.py
--rw-rw-rw-   0 1003370000 (1003370000) 1003370000      618 2023-03-29 15:23:31.000000 nubium-utils-4.1.0.post1/tests/eloqua_utils/test_timestamps.py
--rw-rw-rw-   0 1003370000 (1003370000) 1003370000     6232 2023-03-29 15:23:31.000000 nubium-utils-4.1.0.post1/tests/test_dict_manipulator.py
--rw-rw-rw-   0 1003370000 (1003370000) 1003370000     3657 2023-03-29 15:23:31.000000 nubium-utils-4.1.0.post1/tests/test_general_utils.py
--rw-rw-rw-   0 1003370000 (1003370000) 1003370000     2746 2023-03-29 15:23:31.000000 nubium-utils-4.1.0.post1/tests/test_hashing_utils.py
--rw-rw-rw-   0 1003370000 (1003370000) 1003370000      798 2023-03-29 15:23:31.000000 nubium-utils-4.1.0.post1/tox.ini
+drwxr-sr-x   0 1003370000 (1003370000) 1003370000        0 2023-04-05 19:50:44.286588 nubium-utils-4.2.0/
+-rw-rw-rw-   0 1003370000 (1003370000) 1003370000     1269 2023-04-05 19:50:34.000000 nubium-utils-4.2.0/.gitignore
+-rw-rw-rw-   0 1003370000 (1003370000) 1003370000      417 2023-04-05 19:50:34.000000 nubium-utils-4.2.0/.gitlab-ci.yml
+-rw-rw-rw-   0 1003370000 (1003370000) 1003370000      313 2023-04-05 19:50:34.000000 nubium-utils-4.2.0/CONTRIBUTING.md
+-rw-rw-rw-   0 1003370000 (1003370000) 1003370000       51 2023-04-05 19:50:34.000000 nubium-utils-4.2.0/MANIFEST.in
+-rw-r--r--   0 1003370000 (1003370000) 1003370000    17396 2023-04-05 19:50:44.286588 nubium-utils-4.2.0/PKG-INFO
+-rw-rw-rw-   0 1003370000 (1003370000) 1003370000    16931 2023-04-05 19:50:34.000000 nubium-utils-4.2.0/README.md
+drwxr-sr-x   0 1003370000 (1003370000) 1003370000        0 2023-04-05 19:50:44.222582 nubium-utils-4.2.0/nubium_utils/
+-rw-rw-rw-   0 1003370000 (1003370000) 1003370000      242 2023-04-05 19:50:34.000000 nubium-utils-4.2.0/nubium_utils/__init__.py
+drwxr-sr-x   0 1003370000 (1003370000) 1003370000        0 2023-04-05 19:50:44.223582 nubium-utils-4.2.0/nubium_utils/custom_apps/
+-rw-rw-rw-   0 1003370000 (1003370000) 1003370000      263 2023-04-05 19:50:34.000000 nubium-utils-4.2.0/nubium_utils/custom_apps/__init__.py
+-rw-rw-rw-   0 1003370000 (1003370000) 1003370000     3225 2023-04-05 19:50:34.000000 nubium-utils-4.2.0/nubium_utils/custom_apps/eloqua_retriever.py
+-rw-rw-rw-   0 1003370000 (1003370000) 1003370000     1815 2023-04-05 19:50:34.000000 nubium-utils-4.2.0/nubium_utils/custom_apps/flask_receiver.py
+-rw-rw-rw-   0 1003370000 (1003370000) 1003370000      996 2023-04-05 19:50:34.000000 nubium-utils-4.2.0/nubium_utils/custom_apps/rest_bulk_switcher.py
+-rw-rw-rw-   0 1003370000 (1003370000) 1003370000     3518 2023-04-05 19:50:34.000000 nubium-utils-4.2.0/nubium_utils/custom_apps/salesforce_retriever.py
+-rw-rw-rw-   0 1003370000 (1003370000) 1003370000      504 2023-04-05 19:50:34.000000 nubium-utils-4.2.0/nubium_utils/custom_exceptions.py
+-rw-rw-rw-   0 1003370000 (1003370000) 1003370000     4907 2023-04-05 19:50:34.000000 nubium-utils-4.2.0/nubium_utils/dict_manipulator.py
+-rw-rw-rw-   0 1003370000 (1003370000) 1003370000     1386 2023-04-05 19:50:34.000000 nubium-utils-4.2.0/nubium_utils/dump_topic_configs.py
+drwxr-sr-x   0 1003370000 (1003370000) 1003370000        0 2023-04-05 19:50:44.223582 nubium-utils-4.2.0/nubium_utils/eloqua_utils/
+-rw-rw-rw-   0 1003370000 (1003370000) 1003370000        0 2023-04-05 19:50:34.000000 nubium-utils-4.2.0/nubium_utils/eloqua_utils/__init__.py
+-rw-rw-rw-   0 1003370000 (1003370000) 1003370000     1172 2023-04-05 19:50:34.000000 nubium-utils-4.2.0/nubium_utils/eloqua_utils/timestamps.py
+drwxr-sr-x   0 1003370000 (1003370000) 1003370000        0 2023-04-05 19:50:44.223582 nubium-utils-4.2.0/nubium_utils/fluvii_extensions/
+-rw-rw-rw-   0 1003370000 (1003370000) 1003370000        0 2023-04-05 19:50:34.000000 nubium-utils-4.2.0/nubium_utils/fluvii_extensions/__init__.py
+drwxr-sr-x   0 1003370000 (1003370000) 1003370000        0 2023-04-05 19:50:44.224582 nubium-utils-4.2.0/nubium_utils/fluvii_extensions/apps/
+-rw-rw-rw-   0 1003370000 (1003370000) 1003370000      192 2023-04-05 19:50:34.000000 nubium-utils-4.2.0/nubium_utils/fluvii_extensions/apps/__init__.py
+-rw-rw-rw-   0 1003370000 (1003370000) 1003370000     1727 2023-04-05 19:50:34.000000 nubium-utils-4.2.0/nubium_utils/fluvii_extensions/apps/config.py
+-rw-rw-rw-   0 1003370000 (1003370000) 1003370000      926 2023-04-05 19:50:34.000000 nubium-utils-4.2.0/nubium_utils/fluvii_extensions/apps/nubium_app.py
+-rw-rw-rw-   0 1003370000 (1003370000) 1003370000      352 2023-04-05 19:50:34.000000 nubium-utils-4.2.0/nubium_utils/fluvii_extensions/apps/nubium_multi_msg_app.py
+-rw-rw-rw-   0 1003370000 (1003370000) 1003370000      542 2023-04-05 19:50:34.000000 nubium-utils-4.2.0/nubium_utils/fluvii_extensions/apps/nubium_table_app.py
+drwxr-sr-x   0 1003370000 (1003370000) 1003370000        0 2023-04-05 19:50:44.224582 nubium-utils-4.2.0/nubium_utils/fluvii_extensions/apps/transactions/
+-rw-rw-rw-   0 1003370000 (1003370000) 1003370000       67 2023-04-05 19:50:34.000000 nubium-utils-4.2.0/nubium_utils/fluvii_extensions/apps/transactions/__init__.py
+-rw-rw-rw-   0 1003370000 (1003370000) 1003370000     3684 2023-04-05 19:50:34.000000 nubium-utils-4.2.0/nubium_utils/fluvii_extensions/apps/transactions/transaction.py
+drwxr-sr-x   0 1003370000 (1003370000) 1003370000        0 2023-04-05 19:50:44.224582 nubium-utils-4.2.0/nubium_utils/fluvii_extensions/components/
+-rw-rw-rw-   0 1003370000 (1003370000) 1003370000        0 2023-04-05 19:50:34.000000 nubium-utils-4.2.0/nubium_utils/fluvii_extensions/components/__init__.py
+drwxr-sr-x   0 1003370000 (1003370000) 1003370000        0 2023-04-05 19:50:44.224582 nubium-utils-4.2.0/nubium_utils/fluvii_extensions/components/auth/
+-rw-rw-rw-   0 1003370000 (1003370000) 1003370000       42 2023-04-05 19:50:34.000000 nubium-utils-4.2.0/nubium_utils/fluvii_extensions/components/auth/__init__.py
+-rw-rw-rw-   0 1003370000 (1003370000) 1003370000      308 2023-04-05 19:50:34.000000 nubium-utils-4.2.0/nubium_utils/fluvii_extensions/components/auth/config.py
+drwxr-sr-x   0 1003370000 (1003370000) 1003370000        0 2023-04-05 19:50:44.225582 nubium-utils-4.2.0/nubium_utils/fluvii_extensions/components/consumer/
+-rw-rw-rw-   0 1003370000 (1003370000) 1003370000      130 2023-04-05 19:50:34.000000 nubium-utils-4.2.0/nubium_utils/fluvii_extensions/components/consumer/__init__.py
+-rw-rw-rw-   0 1003370000 (1003370000) 1003370000     1695 2023-04-05 19:50:34.000000 nubium-utils-4.2.0/nubium_utils/fluvii_extensions/components/consumer/config.py
+-rw-rw-rw-   0 1003370000 (1003370000) 1003370000      976 2023-04-05 19:50:34.000000 nubium-utils-4.2.0/nubium_utils/fluvii_extensions/components/consumer/consumer.py
+-rw-rw-rw-   0 1003370000 (1003370000) 1003370000      438 2023-04-05 19:50:34.000000 nubium-utils-4.2.0/nubium_utils/fluvii_extensions/components/consumer/consumer_factory.py
+drwxr-sr-x   0 1003370000 (1003370000) 1003370000        0 2023-04-05 19:50:44.225582 nubium-utils-4.2.0/nubium_utils/fluvii_extensions/components/metrics/
+-rw-rw-rw-   0 1003370000 (1003370000) 1003370000       70 2023-04-05 19:50:34.000000 nubium-utils-4.2.0/nubium_utils/fluvii_extensions/components/metrics/__init__.py
+drwxr-sr-x   0 1003370000 (1003370000) 1003370000        0 2023-04-05 19:50:44.225582 nubium-utils-4.2.0/nubium_utils/fluvii_extensions/components/metrics/manager/
+-rw-rw-rw-   0 1003370000 (1003370000) 1003370000       97 2023-04-05 19:50:34.000000 nubium-utils-4.2.0/nubium_utils/fluvii_extensions/components/metrics/manager/__init__.py
+-rw-rw-rw-   0 1003370000 (1003370000) 1003370000      157 2023-04-05 19:50:34.000000 nubium-utils-4.2.0/nubium_utils/fluvii_extensions/components/metrics/manager/config.py
+-rw-rw-rw-   0 1003370000 (1003370000) 1003370000     2321 2023-04-05 19:50:34.000000 nubium-utils-4.2.0/nubium_utils/fluvii_extensions/components/metrics/manager/metrics_manager.py
+drwxr-sr-x   0 1003370000 (1003370000) 1003370000        0 2023-04-05 19:50:44.225582 nubium-utils-4.2.0/nubium_utils/fluvii_extensions/components/metrics/pusher/
+-rw-rw-rw-   0 1003370000 (1003370000) 1003370000       46 2023-04-05 19:50:34.000000 nubium-utils-4.2.0/nubium_utils/fluvii_extensions/components/metrics/pusher/__init__.py
+-rw-rw-rw-   0 1003370000 (1003370000) 1003370000     1431 2023-04-05 19:50:34.000000 nubium-utils-4.2.0/nubium_utils/fluvii_extensions/components/metrics/pusher/config.py
+drwxr-sr-x   0 1003370000 (1003370000) 1003370000        0 2023-04-05 19:50:44.226582 nubium-utils-4.2.0/nubium_utils/fluvii_extensions/components/producer/
+-rw-rw-rw-   0 1003370000 (1003370000) 1003370000       93 2023-04-05 19:50:34.000000 nubium-utils-4.2.0/nubium_utils/fluvii_extensions/components/producer/__init__.py
+-rw-rw-rw-   0 1003370000 (1003370000) 1003370000      246 2023-04-05 19:50:34.000000 nubium-utils-4.2.0/nubium_utils/fluvii_extensions/components/producer/config.py
+-rw-rw-rw-   0 1003370000 (1003370000) 1003370000      393 2023-04-05 19:50:34.000000 nubium-utils-4.2.0/nubium_utils/fluvii_extensions/components/producer/producer_factory.py
+drwxr-sr-x   0 1003370000 (1003370000) 1003370000        0 2023-04-05 19:50:44.226582 nubium-utils-4.2.0/nubium_utils/fluvii_extensions/components/sqlite/
+-rw-rw-rw-   0 1003370000 (1003370000) 1003370000       38 2023-04-05 19:50:34.000000 nubium-utils-4.2.0/nubium_utils/fluvii_extensions/components/sqlite/__init__.py
+-rw-rw-rw-   0 1003370000 (1003370000) 1003370000      172 2023-04-05 19:50:34.000000 nubium-utils-4.2.0/nubium_utils/fluvii_extensions/components/sqlite/config.py
+-rw-rw-rw-   0 1003370000 (1003370000) 1003370000     1516 2023-04-05 19:50:34.000000 nubium-utils-4.2.0/nubium_utils/general_utils.py
+-rw-rw-rw-   0 1003370000 (1003370000) 1003370000      841 2023-04-05 19:50:34.000000 nubium-utils-4.2.0/nubium_utils/hashing_utils.py
+drwxr-sr-x   0 1003370000 (1003370000) 1003370000        0 2023-04-05 19:50:44.284588 nubium-utils-4.2.0/nubium_utils/integration_utils/
+-rw-rw-rw-   0 1003370000 (1003370000) 1003370000        0 2023-04-05 19:50:34.000000 nubium-utils-4.2.0/nubium_utils/integration_utils/__init__.py
+-rw-rw-rw-   0 1003370000 (1003370000) 1003370000     4009 2023-04-05 19:50:34.000000 nubium-utils-4.2.0/nubium_utils/integration_utils/eloqua_utils.py
+-rw-rw-rw-   0 1003370000 (1003370000) 1003370000     3610 2023-04-05 19:50:34.000000 nubium-utils-4.2.0/nubium_utils/integration_utils/new_validation_utils.py
+-rw-rw-rw-   0 1003370000 (1003370000) 1003370000     4604 2023-04-05 19:50:34.000000 nubium-utils-4.2.0/nubium_utils/integration_utils/salesforce_utils.py
+-rw-rw-rw-   0 1003370000 (1003370000) 1003370000     1202 2023-04-05 19:50:34.000000 nubium-utils-4.2.0/nubium_utils/integration_utils/setup_teardown_utils.py
+-rw-rw-rw-   0 1003370000 (1003370000) 1003370000     1876 2023-04-05 19:50:34.000000 nubium-utils-4.2.0/nubium_utils/integration_utils/topic_utils.py
+-rw-rw-rw-   0 1003370000 (1003370000) 1003370000     2972 2023-04-05 19:50:34.000000 nubium-utils-4.2.0/nubium_utils/integration_utils/validation_utils.py
+drwxr-sr-x   0 1003370000 (1003370000) 1003370000        0 2023-04-05 19:50:44.284588 nubium-utils-4.2.0/nubium_utils/salesforce_utils/
+-rw-rw-rw-   0 1003370000 (1003370000) 1003370000        0 2023-04-05 19:50:34.000000 nubium-utils-4.2.0/nubium_utils/salesforce_utils/__init__.py
+-rw-rw-rw-   0 1003370000 (1003370000) 1003370000     2182 2023-04-05 19:50:34.000000 nubium-utils-4.2.0/nubium_utils/salesforce_utils/sessions.py
+drwxr-sr-x   0 1003370000 (1003370000) 1003370000        0 2023-04-05 19:50:44.285588 nubium-utils-4.2.0/nubium_utils/test_utils/
+-rw-rw-rw-   0 1003370000 (1003370000) 1003370000       35 2023-04-05 19:50:34.000000 nubium-utils-4.2.0/nubium_utils/test_utils/__init__.py
+-rw-rw-rw-   0 1003370000 (1003370000) 1003370000     2364 2023-04-05 19:50:34.000000 nubium-utils-4.2.0/nubium_utils/test_utils/run_app.py
+-rw-rw-rw-   0 1003370000 (1003370000) 1003370000     1168 2023-04-05 19:50:34.000000 nubium-utils-4.2.0/nubium_utils/test_utils/test_tools.py
+drwxr-sr-x   0 1003370000 (1003370000) 1003370000        0 2023-04-05 19:50:44.223582 nubium-utils-4.2.0/nubium_utils.egg-info/
+-rw-r--r--   0 1003370000 (1003370000) 1003370000    17396 2023-04-05 19:50:44.000000 nubium-utils-4.2.0/nubium_utils.egg-info/PKG-INFO
+-rw-r--r--   0 1003370000 (1003370000) 1003370000     3076 2023-04-05 19:50:44.000000 nubium-utils-4.2.0/nubium_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 1003370000 (1003370000) 1003370000        1 2023-04-05 19:50:44.000000 nubium-utils-4.2.0/nubium_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 1003370000 (1003370000) 1003370000      368 2023-04-05 19:50:44.000000 nubium-utils-4.2.0/nubium_utils.egg-info/requires.txt
+-rw-r--r--   0 1003370000 (1003370000) 1003370000       19 2023-04-05 19:50:44.000000 nubium-utils-4.2.0/nubium_utils.egg-info/top_level.txt
+-rw-rw-rw-   0 1003370000 (1003370000) 1003370000      763 2023-04-05 19:50:34.000000 nubium-utils-4.2.0/pyproject.toml
+-rw-rw-rw-   0 1003370000 (1003370000) 1003370000     4103 2023-04-05 19:50:34.000000 nubium-utils-4.2.0/requirements.txt
+-rw-r--r--   0 1003370000 (1003370000) 1003370000       38 2023-04-05 19:50:44.286588 nubium-utils-4.2.0/setup.cfg
+-rw-rw-rw-   0 1003370000 (1003370000) 1003370000     1186 2023-04-05 19:50:34.000000 nubium-utils-4.2.0/setup.py
+drwxr-sr-x   0 1003370000 (1003370000) 1003370000        0 2023-04-05 19:50:44.285588 nubium-utils-4.2.0/tests/
+-rw-rw-rw-   0 1003370000 (1003370000) 1003370000        0 2023-04-05 19:50:34.000000 nubium-utils-4.2.0/tests/__init__.py
+drwxr-sr-x   0 1003370000 (1003370000) 1003370000        0 2023-04-05 19:50:44.285588 nubium-utils-4.2.0/tests/eloqua_utils/
+-rw-rw-rw-   0 1003370000 (1003370000) 1003370000        0 2023-04-05 19:50:34.000000 nubium-utils-4.2.0/tests/eloqua_utils/__init__.py
+-rw-rw-rw-   0 1003370000 (1003370000) 1003370000      618 2023-04-05 19:50:34.000000 nubium-utils-4.2.0/tests/eloqua_utils/test_timestamps.py
+-rw-rw-rw-   0 1003370000 (1003370000) 1003370000     6232 2023-04-05 19:50:34.000000 nubium-utils-4.2.0/tests/test_dict_manipulator.py
+-rw-rw-rw-   0 1003370000 (1003370000) 1003370000     3657 2023-04-05 19:50:34.000000 nubium-utils-4.2.0/tests/test_general_utils.py
+-rw-rw-rw-   0 1003370000 (1003370000) 1003370000     2746 2023-04-05 19:50:34.000000 nubium-utils-4.2.0/tests/test_hashing_utils.py
+-rw-rw-rw-   0 1003370000 (1003370000) 1003370000      830 2023-04-05 19:50:34.000000 nubium-utils-4.2.0/tox.ini
```

### Comparing `nubium-utils-4.1.0.post1/.gitignore` & `nubium-utils-4.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `nubium-utils-4.1.0.post1/PKG-INFO` & `nubium-utils-4.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nubium-utils
-Version: 4.1.0.post1
+Version: 4.2.0
 Summary: Some Kafka utility functions and patterns for the nubium project
 Home-page: https://gitlab.corp.redhat.com/mkt-ops-de/nubium-utils.git
 Author: Edward Brennan
 Author-email: ebrennan@redhat.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `nubium-utils-4.1.0.post1/README.md` & `nubium-utils-4.2.0/README.md`

 * *Files identical despite different names*

### Comparing `nubium-utils-4.1.0.post1/nubium_utils/custom_apps/eloqua_retriever.py` & `nubium-utils-4.2.0/nubium_utils/custom_apps/eloqua_retriever.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,22 @@
 from nubium_utils.fluvii_extensions.apps.nubium_table_app import NubiumTableAppFactory, NubiumTableApp
 from nubium_utils.fluvii_extensions.apps.transactions import NubiumTableTransaction
+from nubium_utils.fluvii_extensions.components.consumer import NubiumConsumerConfig
 from fluvii.exceptions import FinishedTransactionBatch, PartitionsAssigned, TransactionNotRequired
 import logging
 
 
 LOGGER = logging.getLogger(__name__)
 
 
+class NubiumEloquaRetrieverConsumerConfig(NubiumConsumerConfig):
+    """Didn't want to hardcode a new timeout"""
+    timeout_minutes: int = 5
+
+
 class EloquaRetrieverTransaction(NubiumTableTransaction):
     """
     Necessary because we aren't usually consuming a message while producing table messages. We can mock out what
     we would need from a message by returning static values for the necessary items called.
     """
     def key(self):
         return 'timestamp'
@@ -60,14 +66,15 @@
             finally:
                 assignments = self._consumer.assignment()
         super()._run(**kwargs)
 
 
 class NubiumEloquaRetrieverAppFactory(NubiumTableAppFactory):
     fluvii_app_cls = NubiumEloquaRetrieverApp
+    consumer_config_cls = NubiumEloquaRetrieverConsumerConfig
 
     def _make_consumer(self, auto_subscribe=False):
         LOGGER.warning(f'By default, there are some hard-coded consumer settings for {self.__class__.__name__} '
                        'that will override any corresponding configuration settings to ensure expected functionality')
         self._consumer_config.poll_timeout_seconds = 5
         self._consumer_config.batch_consume_max_time_seconds = 4
         return super()._make_consumer(auto_subscribe=auto_subscribe)
```

### Comparing `nubium-utils-4.1.0.post1/nubium_utils/custom_apps/flask_receiver.py` & `nubium-utils-4.2.0/nubium_utils/custom_apps/flask_receiver.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,31 +1,35 @@
 from os import environ
 from unittest import mock
 from nubium_utils.fluvii_extensions.components.producer import NubiumProducerFactory
+from nubium_utils.fluvii_extensions.components.metrics import NubiumMetricsManagerConfig
 import threading
 import time
 
 
 class NubiumFlaskConfig:
-    def __init__(self, producer=None, topic=None, schema=None, producer_config=None):
+    def __init__(self, producer=None, topic=None, schema=None, producer_config=None, metrics_config=None):
         self.LOGLEVEL = environ.get('NUBIUM_LOGLEVEL', 'INFO')
 
         self.TOPIC = topic
         self.PRODUCER = producer
         self.SCHEMA = schema
 
         if self.TOPIC is None:
             self.TOPIC = environ['OUTPUT_TOPIC']
 
         self.TOPIC_SCHEMA_DICT = {self.TOPIC: self.SCHEMA}
 
         if self.PRODUCER is None:
+            if not metrics_config:
+                metrics_config = NubiumMetricsManagerConfig()  # enforces variables are set so the metrics manager works
             self.PRODUCER = NubiumProducerFactory(
                 topic_schema_dict=self.TOPIC_SCHEMA_DICT,
-                producer_config=producer_config)
+                producer_config=producer_config,
+                metrics_manager_config=metrics_config)
         self.METRICS_MANAGER = self.PRODUCER.metrics_manager
 
         self.PRODUCER_POLL_THREAD = threading.Thread(target=self._producer_poll_loop, daemon=True)
         self.PRODUCER_POLL_THREAD.start()
 
     def _producer_poll_loop(self):
         """So we dont get spammed with (harmless) re-auth errors"""
```

### Comparing `nubium-utils-4.1.0.post1/nubium_utils/custom_apps/rest_bulk_switcher.py` & `nubium-utils-4.2.0/nubium_utils/custom_apps/rest_bulk_switcher.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,14 +8,14 @@
 class NubiumRestBulkSwitcherConsumerConfig(NubiumConsumerConfig):
     """Didn't want to hardcode, but did need to change values to have this function reasonably"""
     batch_consume_trigger_message_age_seconds: int = 60
     batch_consume_max_time_seconds: int = 120
 
 
 class NubiumRestBulkSwitcherFactory(NubiumMultiMessageAppFactory):
-    fluvii_app_config_cls = NubiumRestBulkSwitcherConsumerConfig
+    consumer_config_cls = NubiumRestBulkSwitcherConsumerConfig
 
     def _make_consumer(self):
         LOGGER.warning(f'By default, there are some hard-coded consumer settings for {self.__class__.__name__} '
                        'that will override any corresponding configuration settings to ensure expected functionality')
         self._consumer_config.batch_consume_max_count = 0
         return super()._make_consumer()
```

### Comparing `nubium-utils-4.1.0.post1/nubium_utils/custom_apps/salesforce_retriever.py` & `nubium-utils-4.2.0/nubium_utils/custom_apps/salesforce_retriever.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from fluvii.exceptions import FinishedTransactionBatch, PartitionsAssigned, SignalRaise
-from nubium_utils.fluvii_extensions.apps import NubiumTableApp, NubiumTableAppFactory
+from nubium_utils.fluvii_extensions.apps.nubium_table_app import NubiumTableApp, NubiumTableAppFactory
 from nubium_utils.fluvii_extensions.apps.transactions import NubiumTableTransaction
 from nubium_utils.fluvii_extensions.apps import NubiumAppConfig
 import logging
 from time import sleep
 
 LOGGER = logging.getLogger(__name__)
 
@@ -80,10 +80,10 @@
             except PartitionsAssigned:
                 self._handle_rebalance()
             finally:
                 assignments = self._consumer.assignment()
         super()._run(**kwargs)
 
 
-class NubiumEloquaRetrieverAppFactory(NubiumTableAppFactory):
+class NubiumSalesforceRetrieverAppFactory(NubiumTableAppFactory):
     fluvii_app_cls = NubiumSalesforceRetrieverApp
     fluvii_app_config_cls = NubiumSalesforceRetrieverAppConfig
```

### Comparing `nubium-utils-4.1.0.post1/nubium_utils/dict_manipulator.py` & `nubium-utils-4.2.0/nubium_utils/dict_manipulator.py`

 * *Files identical despite different names*

### Comparing `nubium-utils-4.1.0.post1/nubium_utils/eloqua_utils/timestamps.py` & `nubium-utils-4.2.0/nubium_utils/eloqua_utils/timestamps.py`

 * *Files identical despite different names*

### Comparing `nubium-utils-4.1.0.post1/nubium_utils/fluvii_extensions/apps/config.py` & `nubium-utils-4.2.0/nubium_utils/fluvii_extensions/apps/config.py`

 * *Files identical despite different names*

### Comparing `nubium-utils-4.1.0.post1/nubium_utils/fluvii_extensions/apps/nubium_app.py` & `nubium-utils-4.2.0/nubium_utils/fluvii_extensions/apps/nubium_app.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from nubium_utils.general_utils import write_kubernetes_healthcheck_file, del_kubernetes_healthcheck_file
 from fluvii.apps.fluvii_app import FluviiApp, FluviiAppFactory
 from .config import NubiumAppConfig
 from nubium_utils.fluvii_extensions.apps.transactions.transaction import NubiumTransaction
-from nubium_utils.fluvii_extensions.components.metrics import NubiumMetricsManager
+from nubium_utils.fluvii_extensions.components.metrics import NubiumMetricsManager, NubiumMetricsManagerConfig
 
 
 class NubiumApp(FluviiApp):
     def __init__(self, *args, transaction_cls=NubiumTransaction, **kwargs):
         super().__init__(*args, transaction_cls=transaction_cls, **kwargs)
 
     def run(self):
@@ -15,7 +15,8 @@
         del_kubernetes_healthcheck_file()
 
 
 class NubiumAppFactory(FluviiAppFactory):
     fluvii_app_cls = NubiumApp
     fluvii_app_config_cls = NubiumAppConfig
     metrics_cls = NubiumMetricsManager
+    metrics_config_cls = NubiumMetricsManagerConfig
```

### Comparing `nubium-utils-4.1.0.post1/nubium_utils/fluvii_extensions/apps/nubium_table_app.py` & `nubium-utils-4.2.0/nubium_utils/fluvii_extensions/apps/nubium_table_app.py`

 * *Files identical despite different names*

### Comparing `nubium-utils-4.1.0.post1/nubium_utils/fluvii_extensions/apps/transactions/transaction.py` & `nubium-utils-4.2.0/nubium_utils/fluvii_extensions/apps/transactions/transaction.py`

 * *Files identical despite different names*

### Comparing `nubium-utils-4.1.0.post1/nubium_utils/fluvii_extensions/components/consumer/config.py` & `nubium-utils-4.2.0/nubium_utils/fluvii_extensions/components/consumer/config.py`

 * *Files identical despite different names*

### Comparing `nubium-utils-4.1.0.post1/nubium_utils/fluvii_extensions/components/consumer/consumer.py` & `nubium-utils-4.2.0/nubium_utils/fluvii_extensions/components/consumer/consumer.py`

 * *Files identical despite different names*

### Comparing `nubium-utils-4.1.0.post1/nubium_utils/fluvii_extensions/components/metrics/manager/metrics_manager.py` & `nubium-utils-4.2.0/nubium_utils/fluvii_extensions/components/metrics/manager/metrics_manager.py`

 * *Files identical despite different names*

### Comparing `nubium-utils-4.1.0.post1/nubium_utils/fluvii_extensions/components/metrics/pusher/config.py` & `nubium-utils-4.2.0/nubium_utils/fluvii_extensions/components/metrics/pusher/config.py`

 * *Files identical despite different names*

### Comparing `nubium-utils-4.1.0.post1/nubium_utils/general_utils.py` & `nubium-utils-4.2.0/nubium_utils/general_utils.py`

 * *Files identical despite different names*

### Comparing `nubium-utils-4.1.0.post1/nubium_utils/hashing_utils.py` & `nubium-utils-4.2.0/nubium_utils/hashing_utils.py`

 * *Files identical despite different names*

### Comparing `nubium-utils-4.1.0.post1/nubium_utils/integration_utils/eloqua_utils.py` & `nubium-utils-4.2.0/nubium_utils/integration_utils/eloqua_utils.py`

 * *Files identical despite different names*

### Comparing `nubium-utils-4.1.0.post1/nubium_utils/integration_utils/new_validation_utils.py` & `nubium-utils-4.2.0/nubium_utils/integration_utils/new_validation_utils.py`

 * *Files identical despite different names*

### Comparing `nubium-utils-4.1.0.post1/nubium_utils/integration_utils/salesforce_utils.py` & `nubium-utils-4.2.0/nubium_utils/integration_utils/salesforce_utils.py`

 * *Files identical despite different names*

### Comparing `nubium-utils-4.1.0.post1/nubium_utils/integration_utils/setup_teardown_utils.py` & `nubium-utils-4.2.0/nubium_utils/integration_utils/setup_teardown_utils.py`

 * *Files identical despite different names*

### Comparing `nubium-utils-4.1.0.post1/nubium_utils/integration_utils/topic_utils.py` & `nubium-utils-4.2.0/nubium_utils/integration_utils/topic_utils.py`

 * *Files identical despite different names*

### Comparing `nubium-utils-4.1.0.post1/nubium_utils/integration_utils/validation_utils.py` & `nubium-utils-4.2.0/nubium_utils/integration_utils/validation_utils.py`

 * *Files identical despite different names*

### Comparing `nubium-utils-4.1.0.post1/nubium_utils/salesforce_utils/sessions.py` & `nubium-utils-4.2.0/nubium_utils/salesforce_utils/sessions.py`

 * *Files identical despite different names*

### Comparing `nubium-utils-4.1.0.post1/nubium_utils/test_utils/run_app.py` & `nubium-utils-4.2.0/nubium_utils/test_utils/run_app.py`

 * *Files identical despite different names*

### Comparing `nubium-utils-4.1.0.post1/nubium_utils/test_utils/test_tools.py` & `nubium-utils-4.2.0/nubium_utils/test_utils/test_tools.py`

 * *Files identical despite different names*

### Comparing `nubium-utils-4.1.0.post1/nubium_utils.egg-info/PKG-INFO` & `nubium-utils-4.2.0/nubium_utils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nubium-utils
-Version: 4.1.0.post1
+Version: 4.2.0
 Summary: Some Kafka utility functions and patterns for the nubium project
 Home-page: https://gitlab.corp.redhat.com/mkt-ops-de/nubium-utils.git
 Author: Edward Brennan
 Author-email: ebrennan@redhat.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `nubium-utils-4.1.0.post1/nubium_utils.egg-info/SOURCES.txt` & `nubium-utils-4.2.0/nubium_utils.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 pyproject.toml
 requirements.txt
 setup.py
 tox.ini
 nubium_utils/__init__.py
 nubium_utils/custom_exceptions.py
 nubium_utils/dict_manipulator.py
+nubium_utils/dump_topic_configs.py
 nubium_utils/general_utils.py
 nubium_utils/hashing_utils.py
 nubium_utils.egg-info/PKG-INFO
 nubium_utils.egg-info/SOURCES.txt
 nubium_utils.egg-info/dependency_links.txt
 nubium_utils.egg-info/requires.txt
 nubium_utils.egg-info/top_level.txt
@@ -37,14 +38,15 @@
 nubium_utils/fluvii_extensions/components/auth/config.py
 nubium_utils/fluvii_extensions/components/consumer/__init__.py
 nubium_utils/fluvii_extensions/components/consumer/config.py
 nubium_utils/fluvii_extensions/components/consumer/consumer.py
 nubium_utils/fluvii_extensions/components/consumer/consumer_factory.py
 nubium_utils/fluvii_extensions/components/metrics/__init__.py
 nubium_utils/fluvii_extensions/components/metrics/manager/__init__.py
+nubium_utils/fluvii_extensions/components/metrics/manager/config.py
 nubium_utils/fluvii_extensions/components/metrics/manager/metrics_manager.py
 nubium_utils/fluvii_extensions/components/metrics/pusher/__init__.py
 nubium_utils/fluvii_extensions/components/metrics/pusher/config.py
 nubium_utils/fluvii_extensions/components/producer/__init__.py
 nubium_utils/fluvii_extensions/components/producer/config.py
 nubium_utils/fluvii_extensions/components/producer/producer_factory.py
 nubium_utils/fluvii_extensions/components/sqlite/__init__.py
```

### Comparing `nubium-utils-4.1.0.post1/pyproject.toml` & `nubium-utils-4.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -22,13 +22,13 @@
 fixme,
 missing-class-docstring,
 missing-function-docstring,
 missing-module-docstring,
 """
 
 [tool.pytest.ini_options]
-addopts = "-vvv --cov=nubium_utils --cov-report term-missing --cov-branch --no-cov-on-fail --cov-fail-under=10"
+addopts = "-vvv --cov=nubium_utils --cov-report term-missing --cov-branch --no-cov-on-fail --cov-fail-under=9"
 filterwarnings = "ignore:the imp module is deprecated in favour of importlib.*:DeprecationWarning:venusian:"
 testpaths = ["tests"]
 
 [tool.setuptools_scm]
 local_scheme = "no-local-version"
```

### Comparing `nubium-utils-4.1.0.post1/requirements.txt` & `nubium-utils-4.2.0/requirements.txt`

 * *Files 4% similar despite different names*

```diff
@@ -25,52 +25,64 @@
     # via confluent-kafka
 bleach==6.0.0
     # via readme-renderer
 build==0.10.0
     # via pip-tools
 certifi==2022.12.7
     # via requests
+cffi==1.15.1
+    # via cryptography
 charset-normalizer==3.0.1
     # via
     #   aiohttp
     #   requests
 click==8.1.3
     # via
     #   fluvii
     #   pip-tools
 confluent-kafka==1.9.2
     # via fluvii
 coverage==7.1.0
     # via pytest-cov
+cryptography==40.0.1
+    # via secretstorage
 dictdiffer==0.9.0
     # via nubium-utils (setup.py)
 docutils==0.19
     # via readme-renderer
+exceptiongroup==1.1.1
+    # via pytest
 fastavro==1.7.0
     # via confluent-kafka
-fluvii==1.0.2
+fluvii==1.1.0
     # via nubium-utils (setup.py)
 frozenlist==1.3.3
     # via
     #   aiohttp
     #   aiosignal
 idna==3.4
     # via
     #   requests
     #   yarl
 importlib-metadata==6.0.0
     # via
     #   keyring
     #   twine
+importlib-resources==5.12.0
+    # via keyring
 iniconfig==2.0.0
     # via pytest
 isodate==0.6.1
     # via zeep
 jaraco-classes==3.2.3
     # via keyring
+jeepney==0.8.0
+    # via
+    #   keyring
+    #   secretstorage
 keyring==23.13.1
     # via twine
 lxml==4.9.2
     # via zeep
 markdown-it-py==2.1.0
     # via rich
 mdurl==0.1.2
@@ -95,14 +107,16 @@
     # via zeep
 pluggy==1.0.0
     # via pytest
 prometheus-client==0.16.0
     # via fluvii
 psutil==5.9.4
     # via nubium-utils (setup.py)
+pycparser==2.21
+    # via cffi
 pydantic==1.10.4
     # via
     #   fluvii
     #   nubium-utils (setup.py)
 pygments==2.14.0
     # via
     #   readme-renderer
@@ -152,41 +166,53 @@
     # via
     #   twine
     #   zeep
 rfc3986==2.0.0
     # via twine
 rich==13.2.0
     # via twine
+secretstorage==3.3.3
+    # via keyring
 simple-salesforce==1.12.3
     # via nubium-utils (setup.py)
 six==1.16.0
     # via
     #   bleach
     #   isodate
     #   python-dateutil
     #   requests-file
 sqlitedict==2.1.0
     # via fluvii
 time-machine==2.9.0
     # via nubium-utils (setup.py)
+tomli==2.0.1
+    # via
+    #   build
+    #   coverage
+    #   pyproject-hooks
+    #   pytest
 twine==4.0.2
     # via nubium-utils (setup.py)
 typing-extensions==4.4.0
-    # via pydantic
+    # via
+    #   pydantic
+    #   rich
 urllib3==1.26.14
     # via
     #   requests
     #   twine
 webencodings==0.5.1
     # via bleach
 wheel==0.38.4
     # via pip-tools
 yarl==1.8.2
     # via aiohttp
 zeep==4.2.1
     # via simple-salesforce
 zipp==3.11.0
-    # via importlib-metadata
+    # via
+    #   importlib-metadata
+    #   importlib-resources
 
 # The following packages are considered to be unsafe in a requirements file:
 # pip
 # setuptools
```

### Comparing `nubium-utils-4.1.0.post1/setup.py` & `nubium-utils-4.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 
 with open("README.md", "r") as file_obj:
     long_description = file_obj.read()
 
 install_requires = [
-    "fluvii>=1.0.2,<1.1.0",
+    "fluvii>=1.1.0,<1.2.0",
     "aiosfstream",
     "dictdiffer",
     "psutil",
     "pydantic",
     "python-box<7",
     "python-dateutil",
     "python-dotenv",
```

### Comparing `nubium-utils-4.1.0.post1/tests/eloqua_utils/test_timestamps.py` & `nubium-utils-4.2.0/tests/eloqua_utils/test_timestamps.py`

 * *Files identical despite different names*

### Comparing `nubium-utils-4.1.0.post1/tests/test_dict_manipulator.py` & `nubium-utils-4.2.0/tests/test_dict_manipulator.py`

 * *Files identical despite different names*

### Comparing `nubium-utils-4.1.0.post1/tests/test_general_utils.py` & `nubium-utils-4.2.0/tests/test_general_utils.py`

 * *Files identical despite different names*

### Comparing `nubium-utils-4.1.0.post1/tests/test_hashing_utils.py` & `nubium-utils-4.2.0/tests/test_hashing_utils.py`

 * *Files identical despite different names*

### Comparing `nubium-utils-4.1.0.post1/tox.ini` & `nubium-utils-4.2.0/tox.ini`

 * *Files 4% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 
 [testenv:build]
 skip_install = True
 deps =
     setuptools_scm
     wheel
 commands =
+    python setup.py clean --all
     python setup.py sdist bdist_wheel
 
 [testenv:build_reqs]
 deps =
     pip-tools
 skip_install = True
 commands =
```

