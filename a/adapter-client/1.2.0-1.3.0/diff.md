# Comparing `tmp/adapter-client-1.2.0.tar.gz` & `tmp/adapter-client-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adapter-client-1.2.0.tar", last modified: Thu Jul  6 12:44:45 2023, max compression
+gzip compressed data, was "adapter-client-1.3.0.tar", last modified: Thu Jul 13 05:51:55 2023, max compression
```

## Comparing `adapter-client-1.2.0.tar` & `adapter-client-1.3.0.tar`

### file list

```diff
@@ -1,58 +1,59 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 12:44:45.354353 adapter-client-1.2.0/
--rw-r--r--   0 root         (0) root         (0)      290 2022-07-22 09:13:24.000000 adapter-client-1.2.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     4353 2023-07-06 12:44:45.354353 adapter-client-1.2.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3243 2022-07-22 09:13:24.000000 adapter-client-1.2.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 12:44:45.330353 adapter-client-1.2.0/requirements/
--rw-r--r--   0 root         (0) root         (0)      217 2023-07-06 12:44:32.000000 adapter-client-1.2.0/requirements/base.txt
--rw-r--r--   0 root         (0) root         (0)       12 2022-07-22 09:13:24.000000 adapter-client-1.2.0/requirements/prod.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-06 12:44:45.354353 adapter-client-1.2.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2710 2023-07-06 12:44:32.000000 adapter-client-1.2.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 12:44:45.325353 adapter-client-1.2.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 12:44:45.334353 adapter-client-1.2.0/src/adapter_client/
--rw-r--r--   0 root         (0) root         (0)       70 2022-07-22 09:13:24.000000 adapter-client-1.2.0/src/adapter_client/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 12:44:45.336353 adapter-client-1.2.0/src/adapter_client/adapters/
--rw-r--r--   0 root         (0) root         (0)        0 2022-07-22 09:13:24.000000 adapter-client-1.2.0/src/adapter_client/adapters/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2478 2023-07-06 12:44:32.000000 adapter-client-1.2.0/src/adapter_client/adapters/base.py
--rw-r--r--   0 root         (0) root         (0)     9914 2022-07-22 09:13:24.000000 adapter-client-1.2.0/src/adapter_client/adapters/db.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 12:44:45.339353 adapter-client-1.2.0/src/adapter_client/adapters/smev/
--rw-r--r--   0 root         (0) root         (0)        0 2022-07-22 09:13:24.000000 adapter-client-1.2.0/src/adapter_client/adapters/smev/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8563 2023-04-17 05:18:46.000000 adapter-client-1.2.0/src/adapter_client/adapters/smev/adapter.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 12:44:45.341353 adapter-client-1.2.0/src/adapter_client/adapters/smev/interfaces/
--rw-r--r--   0 root         (0) root         (0)       95 2022-07-22 09:13:24.000000 adapter-client-1.2.0/src/adapter_client/adapters/smev/interfaces/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1622 2023-07-06 12:44:32.000000 adapter-client-1.2.0/src/adapter_client/adapters/smev/interfaces/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 12:44:45.341353 adapter-client-1.2.0/src/adapter_client/adapters/smev/interfaces/soap/
--rw-r--r--   0 root         (0) root         (0)        0 2022-07-22 09:13:24.000000 adapter-client-1.2.0/src/adapter_client/adapters/smev/interfaces/soap/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12607 2022-07-22 09:13:24.000000 adapter-client-1.2.0/src/adapter_client/adapters/smev/interfaces/soap/interface.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 12:44:45.345353 adapter-client-1.2.0/src/adapter_client/adapters/smev/interfaces/soap/schema/
--rw-r--r--   0 root         (0) root         (0)     8513 2022-07-22 09:13:24.000000 adapter-client-1.2.0/src/adapter_client/adapters/smev/interfaces/soap/schema/adapter.wsdl
--rw-r--r--   0 root         (0) root         (0)     4627 2022-07-22 09:13:24.000000 adapter-client-1.2.0/src/adapter_client/adapters/smev/interfaces/soap/schema/smev-service-adapter-faults.xsd
--rw-r--r--   0 root         (0) root         (0)    56967 2022-07-22 09:13:24.000000 adapter-client-1.2.0/src/adapter_client/adapters/smev/interfaces/soap/schema/smev-service-adapter-types.xsd
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 12:44:45.347353 adapter-client-1.2.0/src/adapter_client/adapters/smev/logging/
--rw-r--r--   0 root         (0) root         (0)     1714 2023-07-06 12:44:32.000000 adapter-client-1.2.0/src/adapter_client/adapters/smev/logging/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3613 2023-07-06 12:44:32.000000 adapter-client-1.2.0/src/adapter_client/adapters/smev/logging/opensearch.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 12:44:45.349353 adapter-client-1.2.0/src/adapter_client/adapters/smev/services/
--rw-r--r--   0 root         (0) root         (0)        0 2022-07-22 09:13:24.000000 adapter-client-1.2.0/src/adapter_client/adapters/smev/services/__init__.py
--rw-r--r--   0 root         (0) root         (0)      301 2022-07-22 09:13:24.000000 adapter-client-1.2.0/src/adapter_client/adapters/smev/services/base.py
--rw-r--r--   0 root         (0) root         (0)     1501 2022-07-22 09:13:24.000000 adapter-client-1.2.0/src/adapter_client/adapters/smev/services/registry.py
--rw-r--r--   0 root         (0) root         (0)     3624 2023-07-06 12:44:32.000000 adapter-client-1.2.0/src/adapter_client/apps.py
--rw-r--r--   0 root         (0) root         (0)      961 2022-07-22 09:13:24.000000 adapter-client-1.2.0/src/adapter_client/config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 12:44:45.350353 adapter-client-1.2.0/src/adapter_client/core/
--rw-r--r--   0 root         (0) root         (0)        0 2022-07-22 09:13:24.000000 adapter-client-1.2.0/src/adapter_client/core/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 12:44:45.351353 adapter-client-1.2.0/src/adapter_client/core/domain/
--rw-r--r--   0 root         (0) root         (0)        0 2022-07-22 09:13:24.000000 adapter-client-1.2.0/src/adapter_client/core/domain/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9067 2023-07-06 12:44:32.000000 adapter-client-1.2.0/src/adapter_client/core/domain/model.py
--rw-r--r--   0 root         (0) root         (0)      286 2022-07-22 09:13:24.000000 adapter-client-1.2.0/src/adapter_client/core/services.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 12:44:45.353353 adapter-client-1.2.0/src/adapter_client/migrations/
--rw-r--r--   0 root         (0) root         (0)     7165 2022-07-22 09:13:24.000000 adapter-client-1.2.0/src/adapter_client/migrations/0001_initial.py
--rw-r--r--   0 root         (0) root         (0)     3282 2023-07-06 12:44:32.000000 adapter-client-1.2.0/src/adapter_client/migrations/0002_alter_journalentry_options_config_adapter_interface_and_more.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-07-22 09:13:24.000000 adapter-client-1.2.0/src/adapter_client/migrations/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7821 2023-07-06 12:44:32.000000 adapter-client-1.2.0/src/adapter_client/models.py
--rw-r--r--   0 root         (0) root         (0)     5004 2023-07-06 12:44:32.000000 adapter-client-1.2.0/src/adapter_client/tasks.py
--rw-r--r--   0 root         (0) root         (0)      574 2023-04-17 05:18:46.000000 adapter-client-1.2.0/src/adapter_client/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 12:44:45.335353 adapter-client-1.2.0/src/adapter_client.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4353 2023-07-06 12:44:45.000000 adapter-client-1.2.0/src/adapter_client.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1750 2023-07-06 12:44:45.000000 adapter-client-1.2.0/src/adapter_client.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       44 2023-07-06 12:44:45.000000 adapter-client-1.2.0/src/adapter_client.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      219 2023-07-06 12:44:45.000000 adapter-client-1.2.0/src/adapter_client.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-07-06 12:44:45.000000 adapter-client-1.2.0/src/adapter_client.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      450 2023-07-06 12:44:45.000000 adapter-client-1.2.0/version.conf
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 05:51:55.915982 adapter-client-1.3.0/
+-rw-r--r--   0 root         (0) root         (0)      290 2022-07-22 09:13:24.000000 adapter-client-1.3.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     4353 2023-07-13 05:51:55.914982 adapter-client-1.3.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3243 2022-07-22 09:13:24.000000 adapter-client-1.3.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 05:51:55.890982 adapter-client-1.3.0/requirements/
+-rw-r--r--   0 root         (0) root         (0)      217 2023-07-06 12:44:32.000000 adapter-client-1.3.0/requirements/base.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2022-07-22 09:13:24.000000 adapter-client-1.3.0/requirements/prod.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-13 05:51:55.915982 adapter-client-1.3.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2710 2023-07-06 12:44:32.000000 adapter-client-1.3.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 05:51:55.887982 adapter-client-1.3.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 05:51:55.894982 adapter-client-1.3.0/src/adapter_client/
+-rw-r--r--   0 root         (0) root         (0)       70 2022-07-22 09:13:24.000000 adapter-client-1.3.0/src/adapter_client/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 05:51:55.898982 adapter-client-1.3.0/src/adapter_client/adapters/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-07-22 09:13:24.000000 adapter-client-1.3.0/src/adapter_client/adapters/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2478 2023-07-06 12:44:32.000000 adapter-client-1.3.0/src/adapter_client/adapters/base.py
+-rw-r--r--   0 root         (0) root         (0)     9914 2022-07-22 09:13:24.000000 adapter-client-1.3.0/src/adapter_client/adapters/db.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 05:51:55.899982 adapter-client-1.3.0/src/adapter_client/adapters/smev/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-07-22 09:13:24.000000 adapter-client-1.3.0/src/adapter_client/adapters/smev/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8563 2023-04-17 05:18:46.000000 adapter-client-1.3.0/src/adapter_client/adapters/smev/adapter.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 05:51:55.902982 adapter-client-1.3.0/src/adapter_client/adapters/smev/interfaces/
+-rw-r--r--   0 root         (0) root         (0)       95 2022-07-22 09:13:24.000000 adapter-client-1.3.0/src/adapter_client/adapters/smev/interfaces/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1622 2023-07-06 12:44:32.000000 adapter-client-1.3.0/src/adapter_client/adapters/smev/interfaces/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 05:51:55.903982 adapter-client-1.3.0/src/adapter_client/adapters/smev/interfaces/soap/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-07-22 09:13:24.000000 adapter-client-1.3.0/src/adapter_client/adapters/smev/interfaces/soap/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12745 2023-07-13 05:51:43.000000 adapter-client-1.3.0/src/adapter_client/adapters/smev/interfaces/soap/interface.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 05:51:55.906982 adapter-client-1.3.0/src/adapter_client/adapters/smev/interfaces/soap/schema/
+-rw-r--r--   0 root         (0) root         (0)     8513 2022-07-22 09:13:24.000000 adapter-client-1.3.0/src/adapter_client/adapters/smev/interfaces/soap/schema/adapter.wsdl
+-rw-r--r--   0 root         (0) root         (0)     4627 2022-07-22 09:13:24.000000 adapter-client-1.3.0/src/adapter_client/adapters/smev/interfaces/soap/schema/smev-service-adapter-faults.xsd
+-rw-r--r--   0 root         (0) root         (0)    56967 2022-07-22 09:13:24.000000 adapter-client-1.3.0/src/adapter_client/adapters/smev/interfaces/soap/schema/smev-service-adapter-types.xsd
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 05:51:55.908982 adapter-client-1.3.0/src/adapter_client/adapters/smev/logging/
+-rw-r--r--   0 root         (0) root         (0)     1714 2023-07-06 12:44:32.000000 adapter-client-1.3.0/src/adapter_client/adapters/smev/logging/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3613 2023-07-06 12:44:32.000000 adapter-client-1.3.0/src/adapter_client/adapters/smev/logging/opensearch.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 05:51:55.909982 adapter-client-1.3.0/src/adapter_client/adapters/smev/services/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-07-22 09:13:24.000000 adapter-client-1.3.0/src/adapter_client/adapters/smev/services/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      301 2022-07-22 09:13:24.000000 adapter-client-1.3.0/src/adapter_client/adapters/smev/services/base.py
+-rw-r--r--   0 root         (0) root         (0)     1501 2022-07-22 09:13:24.000000 adapter-client-1.3.0/src/adapter_client/adapters/smev/services/registry.py
+-rw-r--r--   0 root         (0) root         (0)     3624 2023-07-06 12:44:32.000000 adapter-client-1.3.0/src/adapter_client/apps.py
+-rw-r--r--   0 root         (0) root         (0)      961 2022-07-22 09:13:24.000000 adapter-client-1.3.0/src/adapter_client/config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 05:51:55.911982 adapter-client-1.3.0/src/adapter_client/core/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-07-22 09:13:24.000000 adapter-client-1.3.0/src/adapter_client/core/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 05:51:55.912982 adapter-client-1.3.0/src/adapter_client/core/domain/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-07-22 09:13:24.000000 adapter-client-1.3.0/src/adapter_client/core/domain/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9137 2023-07-13 05:51:43.000000 adapter-client-1.3.0/src/adapter_client/core/domain/model.py
+-rw-r--r--   0 root         (0) root         (0)      286 2022-07-22 09:13:24.000000 adapter-client-1.3.0/src/adapter_client/core/services.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 05:51:55.914982 adapter-client-1.3.0/src/adapter_client/migrations/
+-rw-r--r--   0 root         (0) root         (0)     7165 2022-07-22 09:13:24.000000 adapter-client-1.3.0/src/adapter_client/migrations/0001_initial.py
+-rw-r--r--   0 root         (0) root         (0)     3282 2023-07-06 12:44:32.000000 adapter-client-1.3.0/src/adapter_client/migrations/0002_alter_journalentry_options_config_adapter_interface_and_more.py
+-rw-r--r--   0 root         (0) root         (0)      613 2023-07-13 05:51:43.000000 adapter-client-1.3.0/src/adapter_client/migrations/0003_message_transaction_code_alter_config_journal_config_and_more.py
+-rw-r--r--   0 root         (0) root         (0)        0 2022-07-22 09:13:24.000000 adapter-client-1.3.0/src/adapter_client/migrations/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8019 2023-07-13 05:51:43.000000 adapter-client-1.3.0/src/adapter_client/models.py
+-rw-r--r--   0 root         (0) root         (0)     5004 2023-07-06 12:44:32.000000 adapter-client-1.3.0/src/adapter_client/tasks.py
+-rw-r--r--   0 root         (0) root         (0)      574 2023-04-17 05:18:46.000000 adapter-client-1.3.0/src/adapter_client/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 05:51:55.896982 adapter-client-1.3.0/src/adapter_client.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4353 2023-07-13 05:51:55.000000 adapter-client-1.3.0/src/adapter_client.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1850 2023-07-13 05:51:55.000000 adapter-client-1.3.0/src/adapter_client.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       44 2023-07-13 05:51:55.000000 adapter-client-1.3.0/src/adapter_client.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      219 2023-07-13 05:51:55.000000 adapter-client-1.3.0/src/adapter_client.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-07-13 05:51:55.000000 adapter-client-1.3.0/src/adapter_client.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      450 2023-07-13 05:51:55.000000 adapter-client-1.3.0/version.conf
```

### Comparing `adapter-client-1.2.0/PKG-INFO` & `adapter-client-1.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adapter-client
-Version: 1.2.0
+Version: 1.3.0
 Summary: Клиент для взаимодействия со СМЭВ3 посредством Адаптера
 Author: BARS Group
 Author-email: education_dev@bars-open.ru
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Web Environment
 Classifier: Natural Language :: Russian
```

### Comparing `adapter-client-1.2.0/README.md` & `adapter-client-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `adapter-client-1.2.0/setup.py` & `adapter-client-1.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `adapter-client-1.2.0/src/adapter_client/adapters/base.py` & `adapter-client-1.3.0/src/adapter_client/adapters/base.py`

 * *Files identical despite different names*

### Comparing `adapter-client-1.2.0/src/adapter_client/adapters/db.py` & `adapter-client-1.3.0/src/adapter_client/adapters/db.py`

 * *Files identical despite different names*

### Comparing `adapter-client-1.2.0/src/adapter_client/adapters/smev/adapter.py` & `adapter-client-1.3.0/src/adapter_client/adapters/smev/adapter.py`

 * *Files identical despite different names*

### Comparing `adapter-client-1.2.0/src/adapter_client/adapters/smev/interfaces/base.py` & `adapter-client-1.3.0/src/adapter_client/adapters/smev/interfaces/base.py`

 * *Files identical despite different names*

### Comparing `adapter-client-1.2.0/src/adapter_client/adapters/smev/interfaces/soap/interface.py` & `adapter-client-1.3.0/src/adapter_client/adapters/smev/interfaces/soap/interface.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # coding: utf-8
 from concurrent.futures import ThreadPoolExecutor
 from pathlib import Path
 from typing import Iterator
 from typing import List
 from typing import Optional
+from typing import Union
 
 from lxml import etree
 from requests.exceptions import RequestException
 from zeep import Client
 from zeep.exceptions import Fault
 from zeep.plugins import HistoryPlugin
 from zeep.transports import Transport
@@ -340,15 +341,15 @@
             ()
         )
         return [ah.filePath for ah in attachment_header]
 
     def _extract_incoming_message_data(
         self,
         adapter_message: CompoundValue,
-    ) -> Optional[model.MessageMetadataInterface]:
+    ) -> Union[Optional[model.MessageMetadataInterface], None]:
 
         request_msg = adapter_message.Message
         smev_metadata = adapter_message.smevMetadata
 
         if not all((request_msg, smev_metadata)):
             return
 
@@ -357,14 +358,15 @@
             getattr(request_msg, 'ResponseContent', None)
         ).content
 
         msg_metadata = (
             getattr(request_msg, 'RequestMetadata', None) or
             getattr(request_msg, 'ResponseMetadata', None)
         )
+        assert msg_metadata is not None
 
         assert smev_metadata.Recipient == self._config.app_mnemonics
 
         # полезная нагрузка ответа
         # не уверен что стоит трогать `_value_1`, но иного способа не вижу
         primary_content = msg_content.MessagePrimaryContent._value_1
         etree.indent(primary_content, '  ')
@@ -372,14 +374,15 @@
         message = model.Message(
             # client_id ответа
             client_id=msg_metadata.clientId,
             # message_id ответа
             message_id=smev_metadata.MessageId,
             # вид сведений
             message_type=primary_content.nsmap[primary_content.prefix],
+            transaction_code=smev_metadata.TransactionCode,
             body=etree.tostring(
                 primary_content,
                 pretty_print=True,
                 encoding='utf-8'
             ).decode('utf-8').strip(),
             reference_message_id=getattr(
                 smev_metadata,
```

### Comparing `adapter-client-1.2.0/src/adapter_client/adapters/smev/interfaces/soap/schema/adapter.wsdl` & `adapter-client-1.3.0/src/adapter_client/adapters/smev/interfaces/soap/schema/adapter.wsdl`

 * *Files identical despite different names*

### Comparing `adapter-client-1.2.0/src/adapter_client/adapters/smev/interfaces/soap/schema/smev-service-adapter-faults.xsd` & `adapter-client-1.3.0/src/adapter_client/adapters/smev/interfaces/soap/schema/smev-service-adapter-faults.xsd`

 * *Files identical despite different names*

### Comparing `adapter-client-1.2.0/src/adapter_client/adapters/smev/interfaces/soap/schema/smev-service-adapter-types.xsd` & `adapter-client-1.3.0/src/adapter_client/adapters/smev/interfaces/soap/schema/smev-service-adapter-types.xsd`

 * *Files identical despite different names*

### Comparing `adapter-client-1.2.0/src/adapter_client/adapters/smev/logging/__init__.py` & `adapter-client-1.3.0/src/adapter_client/adapters/smev/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `adapter-client-1.2.0/src/adapter_client/adapters/smev/logging/opensearch.py` & `adapter-client-1.3.0/src/adapter_client/adapters/smev/logging/opensearch.py`

 * *Files identical despite different names*

### Comparing `adapter-client-1.2.0/src/adapter_client/adapters/smev/services/registry.py` & `adapter-client-1.3.0/src/adapter_client/adapters/smev/services/registry.py`

 * *Files identical despite different names*

### Comparing `adapter-client-1.2.0/src/adapter_client/apps.py` & `adapter-client-1.3.0/src/adapter_client/apps.py`

 * *Files identical despite different names*

### Comparing `adapter-client-1.2.0/src/adapter_client/config.py` & `adapter-client-1.3.0/src/adapter_client/config.py`

 * *Files identical despite different names*

### Comparing `adapter-client-1.2.0/src/adapter_client/core/domain/model.py` & `adapter-client-1.3.0/src/adapter_client/core/domain/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,20 +2,18 @@
 from abc import ABC
 from datetime import datetime
 from enum import Enum
 from typing import TYPE_CHECKING
 from typing import Dict
 from typing import List
 from typing import Optional
-from typing import TypeVar
 from typing import Union
 from uuid import uuid4
 
 from pydantic.fields import Field
-from pydantic.types import Json
 
 
 if TYPE_CHECKING:
     from dataclasses import dataclass  # noqa
 else:
     from pydantic.dataclasses import dataclass  # noqa
 
@@ -154,17 +152,14 @@
 
 class RequestType(NamedIntEnum):
     send = (1, 'Send')
     get = (2, 'Get')
     find = (3, 'Find')
 
 
-Message = TypeVar('Message')
-
-
 @dataclass
 class Message:
 
     """Объект содержащий сообщение в/из РИС.
 
     РИС отправляет и получает на обработку объекты этого типа.
     """
@@ -184,21 +179,25 @@
         title='Клиентский идентификатор запроса',
         default_factory=lambda: str(uuid4()),
     )
     message_id: Union[str, None] = Field(
         title='Идентификатор запроса СМЭВ 3',
         default=None,
     )
-
+    transaction_code: Union[str, None] = Field(
+        title='Код транзакции из СМЭВ',
+        default=None,
+        max_length=1500
+    )
     reference_message_id: Optional[str] = Field(
         title='Идентификатор корневого запроса '
               '(запроса, порождающего цепочку запросов)',
         default=None,
     )
-    reply_to: Optional[Message] = Field(
+    reply_to: Optional['Message'] = Field(
         title='Сообщение, на которое пришел ответ',
         default=None,
     )
 
     test: bool = Field(
         title='Признак тестового взаимодействия',
         default=False,
```

### Comparing `adapter-client-1.2.0/src/adapter_client/migrations/0001_initial.py` & `adapter-client-1.3.0/src/adapter_client/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `adapter-client-1.2.0/src/adapter_client/migrations/0002_alter_journalentry_options_config_adapter_interface_and_more.py` & `adapter-client-1.3.0/src/adapter_client/migrations/0002_alter_journalentry_options_config_adapter_interface_and_more.py`

 * *Files identical despite different names*

### Comparing `adapter-client-1.2.0/src/adapter_client/models.py` & `adapter-client-1.3.0/src/adapter_client/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -139,14 +139,19 @@
     )
     reply_to = models.ForeignKey(
         'adapter_client.Message',
         verbose_name=model.Message.reply_to.title,
         on_delete=models.PROTECT,
         null=True, blank=True
     )
+    transaction_code = models.CharField(
+        verbose_name=model.Message.transaction_code.title,
+        max_length=model.Message.transaction_code.max_length,
+        null=True, blank=True
+    )
 
     test = models.BooleanField(
         verbose_name=model.Message.test.title,
         default=model.Message.test.default
     )
 
     timestamp = models.DateTimeField(
```

### Comparing `adapter-client-1.2.0/src/adapter_client/tasks.py` & `adapter-client-1.3.0/src/adapter_client/tasks.py`

 * *Files identical despite different names*

### Comparing `adapter-client-1.2.0/src/adapter_client/utils.py` & `adapter-client-1.3.0/src/adapter_client/utils.py`

 * *Files identical despite different names*

### Comparing `adapter-client-1.2.0/src/adapter_client.egg-info/PKG-INFO` & `adapter-client-1.3.0/src/adapter_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adapter-client
-Version: 1.2.0
+Version: 1.3.0
 Summary: Клиент для взаимодействия со СМЭВ3 посредством Адаптера
 Author: BARS Group
 Author-email: education_dev@bars-open.ru
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Web Environment
 Classifier: Natural Language :: Russian
```

### Comparing `adapter-client-1.2.0/src/adapter_client.egg-info/SOURCES.txt` & `adapter-client-1.3.0/src/adapter_client.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -34,8 +34,9 @@
 src/adapter_client/adapters/smev/services/registry.py
 src/adapter_client/core/__init__.py
 src/adapter_client/core/services.py
 src/adapter_client/core/domain/__init__.py
 src/adapter_client/core/domain/model.py
 src/adapter_client/migrations/0001_initial.py
 src/adapter_client/migrations/0002_alter_journalentry_options_config_adapter_interface_and_more.py
+src/adapter_client/migrations/0003_message_transaction_code_alter_config_journal_config_and_more.py
 src/adapter_client/migrations/__init__.py
```

