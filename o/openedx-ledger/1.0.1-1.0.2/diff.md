# Comparing `tmp/openedx-ledger-1.0.1.tar.gz` & `tmp/openedx-ledger-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openedx-ledger-1.0.1.tar", last modified: Thu Jun  1 18:08:10 2023, max compression
+gzip compressed data, was "openedx-ledger-1.0.2.tar", last modified: Thu Jul 13 19:25:39 2023, max compression
```

## Comparing `openedx-ledger-1.0.1.tar` & `openedx-ledger-1.0.2.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 18:08:10.743527 openedx-ledger-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (122)     2109 2023-06-01 18:08:05.000000 openedx-ledger-1.0.1/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (122)    35139 2023-06-01 18:08:05.000000 openedx-ledger-1.0.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)      209 2023-06-01 18:08:05.000000 openedx-ledger-1.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     8783 2023-06-01 18:08:10.743527 openedx-ledger-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     5962 2023-06-01 18:08:05.000000 openedx-ledger-1.0.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 18:08:10.739527 openedx-ledger-1.0.1/openedx_ledger/
--rw-r--r--   0 runner    (1001) docker     (122)      175 2023-06-01 18:08:05.000000 openedx-ledger-1.0.1/openedx_ledger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4859 2023-06-01 18:08:05.000000 openedx-ledger-1.0.1/openedx_ledger/admin.py
--rw-r--r--   0 runner    (1001) docker     (122)     5394 2023-06-01 18:08:05.000000 openedx-ledger-1.0.1/openedx_ledger/api.py
--rw-r--r--   0 runner    (1001) docker     (122)      156 2023-06-01 18:08:05.000000 openedx-ledger-1.0.1/openedx_ledger/apps.py
--rw-r--r--   0 runner    (1001) docker     (122)      246 2023-06-01 18:08:05.000000 openedx-ledger-1.0.1/openedx_ledger/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 18:08:10.743527 openedx-ledger-1.0.1/openedx_ledger/migrations/
--rw-r--r--   0 runner    (1001) docker     (122)     3768 2023-06-01 18:08:05.000000 openedx-ledger-1.0.1/openedx_ledger/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (122)     6005 2023-06-01 18:08:05.000000 openedx-ledger-1.0.1/openedx_ledger/migrations/0002_historicalledger_historicalreversal_historicaltransaction.py
--rw-r--r--   0 runner    (1001) docker     (122)     4294 2023-06-01 18:08:05.000000 openedx-ledger-1.0.1/openedx_ledger/migrations/0003_field_updates_20230216_1605.py
--rw-r--r--   0 runner    (1001) docker     (122)      638 2023-06-01 18:08:05.000000 openedx-ledger-1.0.1/openedx_ledger/migrations/0004_ledger_idpkey_blankable.py
--rw-r--r--   0 runner    (1001) docker     (122)    12708 2023-06-01 18:08:05.000000 openedx-ledger-1.0.1/openedx_ledger/migrations/0005_help_text_and_more_indices.py
--rw-r--r--   0 runner    (1001) docker     (122)     4291 2023-06-01 18:08:05.000000 openedx-ledger-1.0.1/openedx_ledger/migrations/0006_auto_20230404_1744.py
--rw-r--r--   0 runner    (1001) docker     (122)      468 2023-06-01 18:08:05.000000 openedx-ledger-1.0.1/openedx_ledger/migrations/0007_alter_externalfulfillmentprovider_name.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-01 18:08:05.000000 openedx-ledger-1.0.1/openedx_ledger/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    16107 2023-06-01 18:08:05.000000 openedx-ledger-1.0.1/openedx_ledger/models.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 18:08:10.743527 openedx-ledger-1.0.1/openedx_ledger/signals/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-01 18:08:05.000000 openedx-ledger-1.0.1/openedx_ledger/signals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      246 2023-06-01 18:08:05.000000 openedx-ledger-1.0.1/openedx_ledger/signals/signals.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 18:08:10.735527 openedx-ledger-1.0.1/openedx_ledger/templates/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 18:08:10.743527 openedx-ledger-1.0.1/openedx_ledger/templates/edx_ledger/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 18:08:10.743527 openedx-ledger-1.0.1/openedx_ledger/templates/edx_ledger/admin/
--rw-r--r--   0 runner    (1001) docker     (122)      831 2023-06-01 18:08:05.000000 openedx-ledger-1.0.1/openedx_ledger/templates/edx_ledger/admin/reverse_transaction.html
--rw-r--r--   0 runner    (1001) docker     (122)      662 2023-06-01 18:08:05.000000 openedx-ledger-1.0.1/openedx_ledger/templates/edx_ledger/base.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 18:08:10.743527 openedx-ledger-1.0.1/openedx_ledger/test_utils/
--rw-r--r--   0 runner    (1001) docker     (122)      341 2023-06-01 18:08:05.000000 openedx-ledger-1.0.1/openedx_ledger/test_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2305 2023-06-01 18:08:05.000000 openedx-ledger-1.0.1/openedx_ledger/test_utils/factories.py
--rw-r--r--   0 runner    (1001) docker     (122)      404 2023-06-01 18:08:05.000000 openedx-ledger-1.0.1/openedx_ledger/urls.py
--rw-r--r--   0 runner    (1001) docker     (122)     1463 2023-06-01 18:08:05.000000 openedx-ledger-1.0.1/openedx_ledger/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     2575 2023-06-01 18:08:05.000000 openedx-ledger-1.0.1/openedx_ledger/views.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 18:08:10.739527 openedx-ledger-1.0.1/openedx_ledger.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     8783 2023-06-01 18:08:10.000000 openedx-ledger-1.0.1/openedx_ledger.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1360 2023-06-01 18:08:10.000000 openedx-ledger-1.0.1/openedx_ledger.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-01 18:08:10.000000 openedx-ledger-1.0.1/openedx_ledger.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-01 18:08:10.000000 openedx-ledger-1.0.1/openedx_ledger.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)      197 2023-06-01 18:08:10.000000 openedx-ledger-1.0.1/openedx_ledger.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       15 2023-06-01 18:08:10.000000 openedx-ledger-1.0.1/openedx_ledger.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 18:08:10.743527 openedx-ledger-1.0.1/requirements/
--rw-r--r--   0 runner    (1001) docker     (122)      304 2023-06-01 18:08:05.000000 openedx-ledger-1.0.1/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (122)      561 2023-06-01 18:08:05.000000 openedx-ledger-1.0.1/requirements/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (122)      208 2023-06-01 18:08:10.743527 openedx-ledger-1.0.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (122)     5100 2023-06-01 18:08:05.000000 openedx-ledger-1.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 18:08:10.743527 openedx-ledger-1.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (122)     2468 2023-06-01 18:08:05.000000 openedx-ledger-1.0.1/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (122)     7504 2023-06-01 18:08:05.000000 openedx-ledger-1.0.1/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (122)     2489 2023-06-01 18:08:05.000000 openedx-ledger-1.0.1/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-13 19:25:39.310959 openedx-ledger-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (122)     2175 2023-07-13 19:25:34.000000 openedx-ledger-1.0.2/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    35139 2023-07-13 19:25:34.000000 openedx-ledger-1.0.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      209 2023-07-13 19:25:34.000000 openedx-ledger-1.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     8849 2023-07-13 19:25:39.310959 openedx-ledger-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     5962 2023-07-13 19:25:34.000000 openedx-ledger-1.0.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-13 19:25:39.306959 openedx-ledger-1.0.2/openedx_ledger/
+-rw-r--r--   0 runner    (1001) docker     (122)      175 2023-07-13 19:25:34.000000 openedx-ledger-1.0.2/openedx_ledger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4859 2023-07-13 19:25:34.000000 openedx-ledger-1.0.2/openedx_ledger/admin.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5897 2023-07-13 19:25:34.000000 openedx-ledger-1.0.2/openedx_ledger/api.py
+-rw-r--r--   0 runner    (1001) docker     (122)      156 2023-07-13 19:25:34.000000 openedx-ledger-1.0.2/openedx_ledger/apps.py
+-rw-r--r--   0 runner    (1001) docker     (122)      246 2023-07-13 19:25:34.000000 openedx-ledger-1.0.2/openedx_ledger/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-13 19:25:39.310959 openedx-ledger-1.0.2/openedx_ledger/migrations/
+-rw-r--r--   0 runner    (1001) docker     (122)     3768 2023-07-13 19:25:34.000000 openedx-ledger-1.0.2/openedx_ledger/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6005 2023-07-13 19:25:34.000000 openedx-ledger-1.0.2/openedx_ledger/migrations/0002_historicalledger_historicalreversal_historicaltransaction.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4294 2023-07-13 19:25:34.000000 openedx-ledger-1.0.2/openedx_ledger/migrations/0003_field_updates_20230216_1605.py
+-rw-r--r--   0 runner    (1001) docker     (122)      638 2023-07-13 19:25:34.000000 openedx-ledger-1.0.2/openedx_ledger/migrations/0004_ledger_idpkey_blankable.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12708 2023-07-13 19:25:34.000000 openedx-ledger-1.0.2/openedx_ledger/migrations/0005_help_text_and_more_indices.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4291 2023-07-13 19:25:34.000000 openedx-ledger-1.0.2/openedx_ledger/migrations/0006_auto_20230404_1744.py
+-rw-r--r--   0 runner    (1001) docker     (122)      468 2023-07-13 19:25:34.000000 openedx-ledger-1.0.2/openedx_ledger/migrations/0007_alter_externalfulfillmentprovider_name.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-13 19:25:34.000000 openedx-ledger-1.0.2/openedx_ledger/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16136 2023-07-13 19:25:34.000000 openedx-ledger-1.0.2/openedx_ledger/models.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-13 19:25:39.310959 openedx-ledger-1.0.2/openedx_ledger/signals/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-13 19:25:34.000000 openedx-ledger-1.0.2/openedx_ledger/signals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      246 2023-07-13 19:25:34.000000 openedx-ledger-1.0.2/openedx_ledger/signals/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-13 19:25:39.306959 openedx-ledger-1.0.2/openedx_ledger/templates/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-13 19:25:39.310959 openedx-ledger-1.0.2/openedx_ledger/templates/edx_ledger/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-13 19:25:39.310959 openedx-ledger-1.0.2/openedx_ledger/templates/edx_ledger/admin/
+-rw-r--r--   0 runner    (1001) docker     (122)      831 2023-07-13 19:25:34.000000 openedx-ledger-1.0.2/openedx_ledger/templates/edx_ledger/admin/reverse_transaction.html
+-rw-r--r--   0 runner    (1001) docker     (122)      662 2023-07-13 19:25:34.000000 openedx-ledger-1.0.2/openedx_ledger/templates/edx_ledger/base.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-13 19:25:39.310959 openedx-ledger-1.0.2/openedx_ledger/test_utils/
+-rw-r--r--   0 runner    (1001) docker     (122)      341 2023-07-13 19:25:34.000000 openedx-ledger-1.0.2/openedx_ledger/test_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2305 2023-07-13 19:25:34.000000 openedx-ledger-1.0.2/openedx_ledger/test_utils/factories.py
+-rw-r--r--   0 runner    (1001) docker     (122)      404 2023-07-13 19:25:34.000000 openedx-ledger-1.0.2/openedx_ledger/urls.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1463 2023-07-13 19:25:34.000000 openedx-ledger-1.0.2/openedx_ledger/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2893 2023-07-13 19:25:34.000000 openedx-ledger-1.0.2/openedx_ledger/views.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-13 19:25:39.310959 openedx-ledger-1.0.2/openedx_ledger.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     8849 2023-07-13 19:25:39.000000 openedx-ledger-1.0.2/openedx_ledger.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1360 2023-07-13 19:25:39.000000 openedx-ledger-1.0.2/openedx_ledger.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-13 19:25:39.000000 openedx-ledger-1.0.2/openedx_ledger.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-13 19:25:39.000000 openedx-ledger-1.0.2/openedx_ledger.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)      197 2023-07-13 19:25:39.000000 openedx-ledger-1.0.2/openedx_ledger.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       15 2023-07-13 19:25:39.000000 openedx-ledger-1.0.2/openedx_ledger.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-13 19:25:39.310959 openedx-ledger-1.0.2/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)      304 2023-07-13 19:25:34.000000 openedx-ledger-1.0.2/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (122)      561 2023-07-13 19:25:34.000000 openedx-ledger-1.0.2/requirements/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      208 2023-07-13 19:25:39.310959 openedx-ledger-1.0.2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (122)     5100 2023-07-13 19:25:34.000000 openedx-ledger-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-13 19:25:39.310959 openedx-ledger-1.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)     2604 2023-07-13 19:25:34.000000 openedx-ledger-1.0.2/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7504 2023-07-13 19:25:34.000000 openedx-ledger-1.0.2/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2489 2023-07-13 19:25:34.000000 openedx-ledger-1.0.2/tests/test_utils.py
```

### Comparing `openedx-ledger-1.0.1/CHANGELOG.rst` & `openedx-ledger-1.0.2/CHANGELOG.rst`

 * *Files 4% similar despite different names*

```diff
@@ -11,14 +11,18 @@
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 **********
 * Nothing unreleased
 
+[1.0.2]
+*******
+* only allow reversals of committed transactions
+
 [1.0.1]
 *******
 * make transaction and ledger admins friendlier
 
 [1.0.0]
 *******
 * Look for an ``lms_user_id`` key when generating transaction idempotency keys, not ``learner_id``.
```

### Comparing `openedx-ledger-1.0.1/LICENSE.txt` & `openedx-ledger-1.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `openedx-ledger-1.0.1/PKG-INFO` & `openedx-ledger-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openedx-ledger
-Version: 1.0.1
+Version: 1.0.2
 Summary: Records transactions against a ledger, denominated in units of value.
 Home-page: https://github.com/openedx/openedx-ledger
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Keywords: Python edx
 Classifier: Development Status :: 3 - Alpha
@@ -206,14 +206,18 @@
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 **********
 * Nothing unreleased
 
+[1.0.2]
+*******
+* only allow reversals of committed transactions
+
 [1.0.1]
 *******
 * make transaction and ledger admins friendlier
 
 [1.0.0]
 *******
 * Look for an ``lms_user_id`` key when generating transaction idempotency keys, not ``learner_id``.
```

### Comparing `openedx-ledger-1.0.1/README.rst` & `openedx-ledger-1.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `openedx-ledger-1.0.1/openedx_ledger/admin.py` & `openedx-ledger-1.0.2/openedx_ledger/admin.py`

 * *Files identical despite different names*

### Comparing `openedx-ledger-1.0.1/openedx_ledger/api.py` & `openedx-ledger-1.0.2/openedx_ledger/api.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,14 +9,20 @@
 
 class LedgerBalanceExceeded(Exception):
     """
     Exception for when a transaction could not be created because it would exceed the ledger balance.
     """
 
 
+class NonCommittedTransactionError(Exception):
+    """
+    Raised when a transaction that is not in a COMMITTED state is used in a reversal.
+    """
+
+
 def create_transaction(
     ledger,
     quantity,
     idempotency_key,
     lms_user_id=None,
     content_key=None,
     subsidy_access_policy_uuid=None,
@@ -46,14 +52,16 @@
             defined by the caller.
 
     Raises:
         openedx_ledger.models.LedgerLockAttemptFailed:
             Raises this if there's another attempt in process to add a transaction to this Ledger.
         openedx_ledger.api.LedgerBalanceExceeded:
             Raises this if the transaction would cause the balance of the ledger to become negative.
+        openedx_ledger.api.NonCommittedTransactionError:
+            Raises this if the transaction is not in a COMMITTED state.
     """
     with ledger.lock():
         durable = not get_connection().in_atomic_block
         with atomic(durable=durable):
             balance = ledger.balance()
             if (quantity < 0) and ((balance + quantity) < 0):
                 raise LedgerBalanceExceeded("A Transaction was not created because it would exceed the ledger balance.")
@@ -82,14 +90,20 @@
     Support idempotency key here, too.
     """
     with atomic(durable=True):
         # select the transaction and any reversals
         # if there is a reversal: return, no work to do here
         # if not, write a reversal for the transaction
         transaction.refresh_from_db()
+
+        if transaction.state != models.TransactionStateChoices.COMMITTED:
+            raise NonCommittedTransactionError(
+                "Cannot reverse transaction because it is not in a committed state."
+            )
+
         reversal, _ = models.Reversal.objects.get_or_create(
             transaction=transaction,
             idempotency_key=idempotency_key,
             defaults={
                 'quantity': transaction.quantity * -1,
                 'metadata': metadata,
             },
```

### Comparing `openedx-ledger-1.0.1/openedx_ledger/migrations/0001_initial.py` & `openedx-ledger-1.0.2/openedx_ledger/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `openedx-ledger-1.0.1/openedx_ledger/migrations/0002_historicalledger_historicalreversal_historicaltransaction.py` & `openedx-ledger-1.0.2/openedx_ledger/migrations/0002_historicalledger_historicalreversal_historicaltransaction.py`

 * *Files identical despite different names*

### Comparing `openedx-ledger-1.0.1/openedx_ledger/migrations/0003_field_updates_20230216_1605.py` & `openedx-ledger-1.0.2/openedx_ledger/migrations/0003_field_updates_20230216_1605.py`

 * *Files identical despite different names*

### Comparing `openedx-ledger-1.0.1/openedx_ledger/migrations/0004_ledger_idpkey_blankable.py` & `openedx-ledger-1.0.2/openedx_ledger/migrations/0004_ledger_idpkey_blankable.py`

 * *Files identical despite different names*

### Comparing `openedx-ledger-1.0.1/openedx_ledger/migrations/0005_help_text_and_more_indices.py` & `openedx-ledger-1.0.2/openedx_ledger/migrations/0005_help_text_and_more_indices.py`

 * *Files identical despite different names*

### Comparing `openedx-ledger-1.0.1/openedx_ledger/migrations/0006_auto_20230404_1744.py` & `openedx-ledger-1.0.2/openedx_ledger/migrations/0006_auto_20230404_1744.py`

 * *Files identical despite different names*

### Comparing `openedx-ledger-1.0.1/openedx_ledger/models.py` & `openedx-ledger-1.0.2/openedx_ledger/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -354,15 +354,15 @@
 
     def get_reversal(self):
         """
         Convenience method for fetching this transaction's related
         reversal, or None if no such reversal exists.
         """
         try:
-            return self.reversal
+            return self.reversal  # pylint: disable=no-member
         except Reversal.DoesNotExist:
             return None
 
 
 class ExternalFulfillmentProvider(TimeStampedModel):
     """
     Model of external fulfillment providers. This is used to track the external systems that are used to fulfill
```

### Comparing `openedx-ledger-1.0.1/openedx_ledger/templates/edx_ledger/admin/reverse_transaction.html` & `openedx-ledger-1.0.2/openedx_ledger/templates/edx_ledger/admin/reverse_transaction.html`

 * *Files identical despite different names*

### Comparing `openedx-ledger-1.0.1/openedx_ledger/templates/edx_ledger/base.html` & `openedx-ledger-1.0.2/openedx_ledger/templates/edx_ledger/base.html`

 * *Files identical despite different names*

### Comparing `openedx-ledger-1.0.1/openedx_ledger/test_utils/factories.py` & `openedx-ledger-1.0.2/openedx_ledger/test_utils/factories.py`

 * *Files identical despite different names*

### Comparing `openedx-ledger-1.0.1/openedx_ledger/utils.py` & `openedx-ledger-1.0.2/openedx_ledger/utils.py`

 * *Files identical despite different names*

### Comparing `openedx-ledger-1.0.1/openedx_ledger/views.py` & `openedx-ledger-1.0.2/openedx_ledger/views.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from django.core.exceptions import ObjectDoesNotExist
 from django.db.utils import IntegrityError
 from django.http import HttpResponseBadRequest, HttpResponseRedirect
 from django.shortcuts import render
 from django.urls import reverse
 from django.views.generic import View
 
-from openedx_ledger.api import reverse_full_transaction
+from openedx_ledger.api import NonCommittedTransactionError, reverse_full_transaction
 from openedx_ledger.models import Transaction
 
 logger = logging.getLogger(__name__)
 
 
 class ReverseTransactionView(View):
     """
@@ -65,9 +65,14 @@
                 idempotency_key=f"admin-invoked-reverse-{str(transaction.uuid)}"
             )
         except IntegrityError:
             logger.exception(
                 f"ReverseTransactionView Error: transaction reversal already exists: {transaction_id}"
             )
             return HttpResponseBadRequest('Transaction Reversal already exists')
+        except NonCommittedTransactionError as error:
+            logger.exception(
+                f"ReverseTransactionView Error: transaction is not in a committed state: {transaction_id}"
+            )
+            return HttpResponseBadRequest(f'Transaction Reversal failed: {error}')
         url = reverse("admin:openedx_ledger_transaction_change", args=(transaction_id,))
         return HttpResponseRedirect(url)
```

### Comparing `openedx-ledger-1.0.1/openedx_ledger.egg-info/PKG-INFO` & `openedx-ledger-1.0.2/openedx_ledger.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openedx-ledger
-Version: 1.0.1
+Version: 1.0.2
 Summary: Records transactions against a ledger, denominated in units of value.
 Home-page: https://github.com/openedx/openedx-ledger
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Keywords: Python edx
 Classifier: Development Status :: 3 - Alpha
@@ -206,14 +206,18 @@
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 **********
 * Nothing unreleased
 
+[1.0.2]
+*******
+* only allow reversals of committed transactions
+
 [1.0.1]
 *******
 * make transaction and ledger admins friendlier
 
 [1.0.0]
 *******
 * Look for an ``lms_user_id`` key when generating transaction idempotency keys, not ``learner_id``.
```

### Comparing `openedx-ledger-1.0.1/openedx_ledger.egg-info/SOURCES.txt` & `openedx-ledger-1.0.2/openedx_ledger.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openedx-ledger-1.0.1/requirements/constraints.txt` & `openedx-ledger-1.0.2/requirements/constraints.txt`

 * *Files identical despite different names*

### Comparing `openedx-ledger-1.0.1/setup.py` & `openedx-ledger-1.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `openedx-ledger-1.0.1/tests/test_api.py` & `openedx-ledger-1.0.2/tests/test_api.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,14 +14,17 @@
 
     api.create_transaction(ledger, quantity=5000, idempotency_key='tx-1', state=TransactionStateChoices.CREATED)
     assert ledger.balance() == 5000
 
     tx_2 = api.create_transaction(ledger, quantity=5000, idempotency_key='tx-2', state=TransactionStateChoices.CREATED)
     assert ledger.balance() == 10000
 
+    tx_2.state = TransactionStateChoices.COMMITTED
+    tx_2.save()
+
     api.reverse_full_transaction(tx_2, idempotency_key='reversal-1')
     assert ledger.balance() == 5000
 
     other_ledger = api.create_ledger(unit=UnitChoices.USD_CENTS, idempotency_key='my-happy-ledger')
     assert ledger == other_ledger
 
 
@@ -48,14 +51,17 @@
 def test_multiple_reversals():
     ledger = api.create_ledger(unit=UnitChoices.USD_CENTS, idempotency_key='my-other-ledger')
     assert ledger.balance() == 0
 
     tx_1 = api.create_transaction(ledger, quantity=5000, idempotency_key='tx-1', state=TransactionStateChoices.CREATED)
     assert ledger.balance() == 5000
 
+    tx_1.state = TransactionStateChoices.COMMITTED
+    tx_1.save()
+
     reversal = api.reverse_full_transaction(tx_1, idempotency_key='reversal-1')
     assert ledger.balance() == 0
 
     with pytest.raises(Exception):
         api.reverse_full_transaction(tx_1, idempotency_key='reversal-2')
 
     third_reversal = api.reverse_full_transaction(tx_1, idempotency_key='reversal-1')
```

### Comparing `openedx-ledger-1.0.1/tests/test_models.py` & `openedx-ledger-1.0.2/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `openedx-ledger-1.0.1/tests/test_utils.py` & `openedx-ledger-1.0.2/tests/test_utils.py`

 * *Files identical despite different names*

