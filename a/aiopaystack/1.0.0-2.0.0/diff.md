# Comparing `tmp/aiopaystack-1.0.0.tar.gz` & `tmp/aiopaystack-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiopaystack-1.0.0.tar", last modified: Sun Nov 13 22:35:05 2022, max compression
+gzip compressed data, was "aiopaystack-2.0.0.tar", last modified: Thu Jul 13 21:32:33 2023, max compression
```

## Comparing `aiopaystack-1.0.0.tar` & `aiopaystack-2.0.0.tar`

### file list

```diff
@@ -1,40 +1,65 @@
-drwxrwxrwx   0        0        0        0 2022-11-13 22:35:05.881230 aiopaystack-1.0.0/
--rw-rw-rw-   0        0        0     1092 2022-10-08 17:33:58.000000 aiopaystack-1.0.0/LICENSE
--rw-rw-rw-   0        0        0     1775 2022-11-13 22:35:05.851202 aiopaystack-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     1198 2022-11-13 22:16:05.000000 aiopaystack-1.0.0/README.md
--rw-rw-rw-   0        0        0      718 2022-11-13 22:21:28.000000 aiopaystack-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2022-11-13 22:35:05.882246 aiopaystack-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0       41 2022-10-14 21:01:56.000000 aiopaystack-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2022-11-13 22:35:05.625559 aiopaystack-1.0.0/src/
-drwxrwxrwx   0        0        0        0 2022-11-13 22:35:05.696149 aiopaystack-1.0.0/src/aiopaystack.egg-info/
--rw-rw-rw-   0        0        0     1775 2022-11-13 22:35:05.000000 aiopaystack-1.0.0/src/aiopaystack.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      916 2022-11-13 22:35:05.000000 aiopaystack-1.0.0/src/aiopaystack.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-11-13 22:35:05.000000 aiopaystack-1.0.0/src/aiopaystack.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2022-11-13 22:35:05.000000 aiopaystack-1.0.0/src/aiopaystack.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2022-11-13 22:35:05.000000 aiopaystack-1.0.0/src/aiopaystack.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2022-11-13 22:35:05.846208 aiopaystack-1.0.0/src/paystack/
--rw-rw-rw-   0        0        0      889 2022-11-13 22:16:05.000000 aiopaystack-1.0.0/src/paystack/__init__.py
--rw-rw-rw-   0        0        0     1195 2022-11-13 22:16:05.000000 aiopaystack-1.0.0/src/paystack/apple_pay.py
--rw-rw-rw-   0        0        0     3006 2022-11-13 22:16:05.000000 aiopaystack-1.0.0/src/paystack/base.py
--rw-rw-rw-   0        0        0     4110 2022-11-13 22:16:05.000000 aiopaystack-1.0.0/src/paystack/bulkcharge.py
--rw-rw-rw-   0        0        0     3413 2022-11-13 22:16:05.000000 aiopaystack-1.0.0/src/paystack/charge.py
--rw-rw-rw-   0        0        0      924 2022-11-13 22:16:06.000000 aiopaystack-1.0.0/src/paystack/control_panel.py
--rw-rw-rw-   0        0        0     4979 2022-11-13 22:16:06.000000 aiopaystack-1.0.0/src/paystack/customers.py
--rw-rw-rw-   0        0        0     4447 2022-11-13 22:16:06.000000 aiopaystack-1.0.0/src/paystack/dedicated_virtual_accounts.py
--rw-rw-rw-   0        0        0     4480 2022-11-13 22:16:06.000000 aiopaystack-1.0.0/src/paystack/disputes.py
--rw-rw-rw-   0        0        0     4234 2022-11-13 22:16:06.000000 aiopaystack-1.0.0/src/paystack/invoices.py
--rw-rw-rw-   0        0        0     1818 2022-11-13 22:16:06.000000 aiopaystack-1.0.0/src/paystack/misc.py
--rw-rw-rw-   0        0        0     2985 2022-11-13 22:16:06.000000 aiopaystack-1.0.0/src/paystack/page.py
--rw-rw-rw-   0        0        0      588 2022-11-13 22:16:06.000000 aiopaystack-1.0.0/src/paystack/paystack.py
--rw-rw-rw-   0        0        0     2692 2022-11-13 22:16:06.000000 aiopaystack-1.0.0/src/paystack/plans.py
--rw-rw-rw-   0        0        0     2911 2022-11-13 22:16:06.000000 aiopaystack-1.0.0/src/paystack/products.py
--rw-rw-rw-   0        0        0     1459 2022-11-13 22:16:06.000000 aiopaystack-1.0.0/src/paystack/refund.py
--rw-rw-rw-   0        0        0     2361 2022-11-13 22:16:06.000000 aiopaystack-1.0.0/src/paystack/settlements.py
--rw-rw-rw-   0        0        0     3299 2022-11-13 22:16:06.000000 aiopaystack-1.0.0/src/paystack/subaccounts.py
--rw-rw-rw-   0        0        0     3521 2022-11-13 22:16:06.000000 aiopaystack-1.0.0/src/paystack/subscriptions.py
--rw-rw-rw-   0        0        0     4709 2022-11-13 22:16:06.000000 aiopaystack-1.0.0/src/paystack/transaction_splits.py
--rw-rw-rw-   0        0        0     7299 2022-11-13 22:16:06.000000 aiopaystack-1.0.0/src/paystack/transactions.py
--rw-rw-rw-   0        0        0     2315 2022-11-13 22:16:06.000000 aiopaystack-1.0.0/src/paystack/transfer_control.py
--rw-rw-rw-   0        0        0     4034 2022-11-13 22:16:06.000000 aiopaystack-1.0.0/src/paystack/transfer_recipient.py
--rw-rw-rw-   0        0        0     3690 2022-11-13 22:16:06.000000 aiopaystack-1.0.0/src/paystack/transfers.py
--rw-rw-rw-   0        0        0     2360 2022-11-13 22:16:06.000000 aiopaystack-1.0.0/src/paystack/verification.py
+drwxrwxrwx   0        0        0        0 2023-07-13 21:32:33.916012 aiopaystack-2.0.0/
+-rw-rw-rw-   0        0        0     1092 2023-07-08 10:00:50.000000 aiopaystack-2.0.0/LICENSE
+-rw-rw-rw-   0        0        0     2532 2023-07-13 21:32:33.914015 aiopaystack-2.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1955 2023-07-08 10:00:50.000000 aiopaystack-2.0.0/README.md
+-rw-rw-rw-   0        0        0      682 2023-07-13 21:29:10.000000 aiopaystack-2.0.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-13 21:32:33.916012 aiopaystack-2.0.0/setup.cfg
+-rw-rw-rw-   0        0        0       41 2023-07-08 10:00:50.000000 aiopaystack-2.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-13 21:32:28.184684 aiopaystack-2.0.0/src/
+drwxrwxrwx   0        0        0        0 2023-07-13 21:32:30.033575 aiopaystack-2.0.0/src/aiopaystack.egg-info/
+-rw-rw-rw-   0        0        0     2532 2023-07-13 21:32:28.000000 aiopaystack-2.0.0/src/aiopaystack.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1456 2023-07-13 21:32:28.000000 aiopaystack-2.0.0/src/aiopaystack.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-13 21:32:28.000000 aiopaystack-2.0.0/src/aiopaystack.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-13 21:32:28.000000 aiopaystack-2.0.0/src/aiopaystack.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-13 21:32:32.796177 aiopaystack-2.0.0/src/paystack/
+-rw-rw-rw-   0        0        0      889 2023-07-08 10:00:50.000000 aiopaystack-2.0.0/src/paystack/__init__.py
+-rw-rw-rw-   0        0        0     1195 2023-07-08 10:00:50.000000 aiopaystack-2.0.0/src/paystack/apple_pay.py
+-rw-rw-rw-   0        0        0     3181 2023-07-13 21:19:54.000000 aiopaystack-2.0.0/src/paystack/base.py
+-rw-rw-rw-   0        0        0     4110 2023-07-08 10:00:50.000000 aiopaystack-2.0.0/src/paystack/bulkcharge.py
+-rw-rw-rw-   0        0        0     3413 2023-07-08 10:00:50.000000 aiopaystack-2.0.0/src/paystack/charge.py
+-rw-rw-rw-   0        0        0      924 2023-07-08 10:00:50.000000 aiopaystack-2.0.0/src/paystack/control_panel.py
+-rw-rw-rw-   0        0        0     5020 2023-07-11 01:51:28.000000 aiopaystack-2.0.0/src/paystack/customers.py
+-rw-rw-rw-   0        0        0     4447 2023-07-08 10:00:50.000000 aiopaystack-2.0.0/src/paystack/dedicated_virtual_accounts.py
+-rw-rw-rw-   0        0        0     4480 2023-07-08 10:00:50.000000 aiopaystack-2.0.0/src/paystack/disputes.py
+-rw-rw-rw-   0        0        0     4234 2023-07-08 10:00:50.000000 aiopaystack-2.0.0/src/paystack/invoices.py
+-rw-rw-rw-   0        0        0     1818 2023-07-08 10:00:50.000000 aiopaystack-2.0.0/src/paystack/misc.py
+-rw-rw-rw-   0        0        0     2985 2023-07-08 10:00:50.000000 aiopaystack-2.0.0/src/paystack/page.py
+-rw-rw-rw-   0        0        0      599 2023-07-08 16:51:17.000000 aiopaystack-2.0.0/src/paystack/paystack.py
+-rw-rw-rw-   0        0        0     2692 2023-07-08 10:00:50.000000 aiopaystack-2.0.0/src/paystack/plans.py
+-rw-rw-rw-   0        0        0     2911 2023-07-08 10:00:50.000000 aiopaystack-2.0.0/src/paystack/products.py
+-rw-rw-rw-   0        0        0     1459 2023-07-08 10:00:50.000000 aiopaystack-2.0.0/src/paystack/refund.py
+-rw-rw-rw-   0        0        0     2361 2023-07-08 10:00:50.000000 aiopaystack-2.0.0/src/paystack/settlements.py
+-rw-rw-rw-   0        0        0     3299 2023-07-08 10:00:50.000000 aiopaystack-2.0.0/src/paystack/subaccounts.py
+-rw-rw-rw-   0        0        0     3521 2023-07-08 10:00:50.000000 aiopaystack-2.0.0/src/paystack/subscriptions.py
+-rw-rw-rw-   0        0        0     4758 2023-07-12 20:58:13.000000 aiopaystack-2.0.0/src/paystack/transaction_splits.py
+-rw-rw-rw-   0        0        0     7152 2023-07-11 02:02:44.000000 aiopaystack-2.0.0/src/paystack/transactions.py
+-rw-rw-rw-   0        0        0     2315 2023-07-08 10:00:50.000000 aiopaystack-2.0.0/src/paystack/transfer_control.py
+-rw-rw-rw-   0        0        0     4034 2023-07-08 10:00:50.000000 aiopaystack-2.0.0/src/paystack/transfer_recipient.py
+-rw-rw-rw-   0        0        0     3690 2023-07-08 10:00:50.000000 aiopaystack-2.0.0/src/paystack/transfers.py
+-rw-rw-rw-   0        0        0     2360 2023-07-08 10:00:50.000000 aiopaystack-2.0.0/src/paystack/verification.py
+drwxrwxrwx   0        0        0        0 2023-07-13 21:32:32.815174 aiopaystack-2.0.0/test/
+-rw-rw-rw-   0        0        0      549 2023-07-09 18:10:39.000000 aiopaystack-2.0.0/test/test_one.py
+-rw-rw-rw-   0        0        0      225 2023-07-09 18:11:12.000000 aiopaystack-2.0.0/test/test_two.py
+drwxrwxrwx   0        0        0        0 2023-07-13 21:32:33.911011 aiopaystack-2.0.0/tests/
+-rw-rw-rw-   0        0        0      459 2023-07-08 10:00:50.000000 aiopaystack-2.0.0/tests/test_apple_pay.py
+-rw-rw-rw-   0        0        0      950 2023-07-08 10:00:50.000000 aiopaystack-2.0.0/tests/test_bulk_charge.py
+-rw-rw-rw-   0        0        0     1248 2023-07-08 10:00:50.000000 aiopaystack-2.0.0/tests/test_charge.py
+-rw-rw-rw-   0        0        0      420 2023-07-08 10:00:50.000000 aiopaystack-2.0.0/tests/test_control_panel.py
+-rw-rw-rw-   0        0        0     1569 2023-07-12 21:17:38.000000 aiopaystack-2.0.0/tests/test_customers.py
+-rw-rw-rw-   0        0        0     1355 2023-07-08 10:00:50.000000 aiopaystack-2.0.0/tests/test_dispute.py
+-rw-rw-rw-   0        0        0     1343 2023-07-13 21:19:54.000000 aiopaystack-2.0.0/tests/test_dva.py
+-rw-rw-rw-   0        0        0     1178 2023-07-08 10:00:50.000000 aiopaystack-2.0.0/tests/test_invoices.py
+-rw-rw-rw-   0        0        0      600 2023-07-08 10:00:50.000000 aiopaystack-2.0.0/tests/test_misc.py
+-rw-rw-rw-   0        0        0      836 2023-07-08 10:00:50.000000 aiopaystack-2.0.0/tests/test_pages.py
+-rw-rw-rw-   0        0        0      671 2023-07-08 10:00:50.000000 aiopaystack-2.0.0/tests/test_plans.py
+-rw-rw-rw-   0        0        0      732 2023-07-08 10:00:50.000000 aiopaystack-2.0.0/tests/test_products.py
+-rw-rw-rw-   0        0        0      472 2023-07-08 10:00:50.000000 aiopaystack-2.0.0/tests/test_refund.py
+-rw-rw-rw-   0        0        0      363 2023-07-08 10:00:50.000000 aiopaystack-2.0.0/tests/test_settlements.py
+-rw-rw-rw-   0        0        0      645 2023-07-08 10:00:50.000000 aiopaystack-2.0.0/tests/test_subaccounts.py
+-rw-rw-rw-   0        0        0     1004 2023-07-08 10:00:50.000000 aiopaystack-2.0.0/tests/test_subscriptions.py
+-rw-rw-rw-   0        0        0     1353 2023-07-12 21:09:50.000000 aiopaystack-2.0.0/tests/test_transaction_splits.py
+-rw-rw-rw-   0        0        0     2104 2023-07-12 21:14:25.000000 aiopaystack-2.0.0/tests/test_transactions.py
+-rw-rw-rw-   0        0        0      902 2023-07-08 10:00:50.000000 aiopaystack-2.0.0/tests/test_transfer_control.py
+-rw-rw-rw-   0        0        0      832 2023-07-08 10:00:50.000000 aiopaystack-2.0.0/tests/test_transfer_recipient.py
+-rw-rw-rw-   0        0        0      934 2023-07-08 10:00:50.000000 aiopaystack-2.0.0/tests/test_transfers.py
+-rw-rw-rw-   0        0        0      573 2023-07-08 10:00:50.000000 aiopaystack-2.0.0/tests/test_verification.py
```

### Comparing `aiopaystack-1.0.0/LICENSE` & `aiopaystack-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aiopaystack-1.0.0/PKG-INFO` & `aiopaystack-2.0.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,47 +1,67 @@
 Metadata-Version: 2.1
 Name: aiopaystack
-Version: 1.0.0
+Version: 2.0.0
 Summary: Asynchronous PayStack library
 Author-email: Ichinga Samuel <ichingasamuel@gmail.com>
 Project-URL: Homepage, https://github.com/Ichinga-Samuel/aiopaystack
 Project-URL: Bug Tracker, https://github.com/Ichinga-Samuel/aiopaystack/issues
 Keywords: paystack,asynchronous
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # aiopaystack
 
+
 Asynchronous Python library for [Paystack](https://paystack.com/)
 
-Add your paystack secret key as an environment variable as PAY_STACK_SECRET_KEY
+![GitHub](https://img.shields.io/github/license/ichinga-samuel/aiopaystack)
+![PyPI](https://img.shields.io/pypi/v/aiopaystack)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/aiopaystack)
+![GitHub issues](https://img.shields.io/github/issues/ichinga-samuel/aiopaystack)
+![GitHub Workflow Status (branch)](https://img.shields.io/github/workflow/status/ichinga-samuel/aiopaystack/master/master)
+## Installation
+```bash
+pip install aiopaystack
+```
 
+## Usage
+Add your paystack secret key as an environment variable as PAY_STACK_SECRET_KEY
 ```python
 from paystack import Transactions
 
 trans = Transactions()
 
-await trans.initialize(email="sam@gmail.com", amount='5000')
 # All parameters must be passed in as keywords. For both required and optional arguments.
+res = await trans.initialize(email="sam@gmail.com", amount='5000')
 
 # Passing secret key as an argument
 # This replaces any key set in the environment
 from paystack import Paystack
 paystack = Paystack(secret_key="paystack_secret_key")
 
 # to use one session for multiple request use the class as a context manager
 async with Transactions() as trans:
     res= await trans.verify(reference="ref")
     
 # The response type for every request is a typed dict.
 from typing import TypedDict, Any
 Response = TypedDict('Response', {'status_code': int, 'status': bool, 'message': str, 'data': dict | Any})
 
+# Sample response
+{'status': True,
+ 'message': 'Authorization URL created',
+ 'data': 
+     {'authorization_url': 'https://checkout.paystack.com/3521i62zf1i0ljl',
+      'access_code': '3521i62zf1i0ljl', 'reference': '2q16btxglw'
+      },
+ 'status_code': 200
+ }
 ## DOC Reference: <https://developers.paystack.co/v2.0/reference>
 ### Static Use
 ```
 Don't forget to get your API key from [Paystack](https://paystack.com/) and assign to the variable `PAYSTACK_SECRET_KEY`
 Please reference the **docs** folder for usage,
```

### Comparing `aiopaystack-1.0.0/pyproject.toml` & `aiopaystack-2.0.0/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -3,23 +3,22 @@
     "setuptools>=42",
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "aiopaystack"
-version = "1.0.0"
+version = "2.0.0"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 keywords = ['paystack', 'asynchronous']
-dependencies = ['httpx >= 0.23.0']
 authors = [{name = "Ichinga Samuel", email = "ichingasamuel@gmail.com"}]
 description = "Asynchronous PayStack library"
 
 [project.urls]
 "Homepage" = "https://github.com/Ichinga-Samuel/aiopaystack"
 "Bug Tracker" = "https://github.com/Ichinga-Samuel/aiopaystack/issues"
```

### Comparing `aiopaystack-1.0.0/src/aiopaystack.egg-info/PKG-INFO` & `aiopaystack-2.0.0/src/aiopaystack.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,47 +1,67 @@
 Metadata-Version: 2.1
 Name: aiopaystack
-Version: 1.0.0
+Version: 2.0.0
 Summary: Asynchronous PayStack library
 Author-email: Ichinga Samuel <ichingasamuel@gmail.com>
 Project-URL: Homepage, https://github.com/Ichinga-Samuel/aiopaystack
 Project-URL: Bug Tracker, https://github.com/Ichinga-Samuel/aiopaystack/issues
 Keywords: paystack,asynchronous
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # aiopaystack
 
+
 Asynchronous Python library for [Paystack](https://paystack.com/)
 
-Add your paystack secret key as an environment variable as PAY_STACK_SECRET_KEY
+![GitHub](https://img.shields.io/github/license/ichinga-samuel/aiopaystack)
+![PyPI](https://img.shields.io/pypi/v/aiopaystack)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/aiopaystack)
+![GitHub issues](https://img.shields.io/github/issues/ichinga-samuel/aiopaystack)
+![GitHub Workflow Status (branch)](https://img.shields.io/github/workflow/status/ichinga-samuel/aiopaystack/master/master)
+## Installation
+```bash
+pip install aiopaystack
+```
 
+## Usage
+Add your paystack secret key as an environment variable as PAY_STACK_SECRET_KEY
 ```python
 from paystack import Transactions
 
 trans = Transactions()
 
-await trans.initialize(email="sam@gmail.com", amount='5000')
 # All parameters must be passed in as keywords. For both required and optional arguments.
+res = await trans.initialize(email="sam@gmail.com", amount='5000')
 
 # Passing secret key as an argument
 # This replaces any key set in the environment
 from paystack import Paystack
 paystack = Paystack(secret_key="paystack_secret_key")
 
 # to use one session for multiple request use the class as a context manager
 async with Transactions() as trans:
     res= await trans.verify(reference="ref")
     
 # The response type for every request is a typed dict.
 from typing import TypedDict, Any
 Response = TypedDict('Response', {'status_code': int, 'status': bool, 'message': str, 'data': dict | Any})
 
+# Sample response
+{'status': True,
+ 'message': 'Authorization URL created',
+ 'data': 
+     {'authorization_url': 'https://checkout.paystack.com/3521i62zf1i0ljl',
+      'access_code': '3521i62zf1i0ljl', 'reference': '2q16btxglw'
+      },
+ 'status_code': 200
+ }
 ## DOC Reference: <https://developers.paystack.co/v2.0/reference>
 ### Static Use
 ```
 Don't forget to get your API key from [Paystack](https://paystack.com/) and assign to the variable `PAYSTACK_SECRET_KEY`
 Please reference the **docs** folder for usage,
```

### Comparing `aiopaystack-1.0.0/src/paystack/__init__.py` & `aiopaystack-2.0.0/src/paystack/__init__.py`

 * *Files identical despite different names*

### Comparing `aiopaystack-1.0.0/src/paystack/apple_pay.py` & `aiopaystack-2.0.0/src/paystack/apple_pay.py`

 * *Files identical despite different names*

### Comparing `aiopaystack-1.0.0/src/paystack/bulkcharge.py` & `aiopaystack-2.0.0/src/paystack/bulkcharge.py`

 * *Files identical despite different names*

### Comparing `aiopaystack-1.0.0/src/paystack/charge.py` & `aiopaystack-2.0.0/src/paystack/charge.py`

 * *Files identical despite different names*

### Comparing `aiopaystack-1.0.0/src/paystack/control_panel.py` & `aiopaystack-2.0.0/src/paystack/control_panel.py`

 * *Files identical despite different names*

### Comparing `aiopaystack-1.0.0/src/paystack/customers.py` & `aiopaystack-2.0.0/src/paystack/customers.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,101 +1,103 @@
 from typing import Literal
 from datetime import datetime
 
-from .base import Base
+from .base import Base, Response
 
 
 class Customers(Base):
     """
     The Customers API allows you create and manage customers on your integration.
     """
 
     def __init__(self):
         super().__init__()
         url = "/customer/{}"
         self.url = url.format
 
-    async def create(self, *, email: str, last_name: str, first_name: str, **kwargs):
+    async def create(self, *, email: str, last_name: str, first_name: str, **kwargs) -> Response:
         """
         Create a customer on your integration
         :param email: Customer's email address
         :param last_name: Customer's last name
         :param first_name: Customer's first name
         :param kwargs: Optional params as kwargs
-        :return: Response
+        :return: Response Dict
         """
         data = {'email': email, 'last_name': last_name, 'first_name': first_name, **kwargs}
         return await self.post(url=self.url(""), json=data)
 
-    async def list(self, perPage: int = 50, page: int = 1, from_: datetime | None | str = None, to: datetime | None | str = None):
+    async def list(self, perPage: int = 50, page: int = 1, from_: datetime | None | str = None,
+                   to: datetime | None | str = None) -> Response:
         """
         List customers available on your integration
         :param perPage: Specify how many records you want to retrieve per page. If not specify we use a default value of 50.
         :param page: Specify exactly what page you want to retrieve. If not specify we use a default value of 1.
         :param from_: A timestamp from which to start listing customers e.g.
         :param to: A timestamp at which to stop listing product e.g. 2016-09-24T00:00:05.000Z, 2016-09-21
-        :return: Response
+        :return: Response Dict
         """
-        params = {key: value for key, value in (('perPage', perPage), ('page', page), ('from', from_), ('to', to)) if value}
+        params = {key: value for key, value in (('perPage', perPage), ('page', page), ('from', from_),
+                                                ('to', to)) if value}
         return await self.get(url=self.url(""), params=params)
 
-    async def fetch(self, *, email_or_code: str):
+    async def fetch(self, *, email_or_code: str) -> Response:
         """
         Get details of a customer on your integration.
         :param email_or_code: An email or customer code for the customer you want to fetch
-        :return: Response
+        :return: Response Dict
         """
         return await self.get(url=self.url(f"{email_or_code}"))
 
-    async def update(self, *, code, first_name: str, last_name: str, **kwargs):
+    async def update(self, *, code, **kwargs) -> Response:
         """
         Update a customer's details on your integration
-        :param last_name: Customer's last name
-        :param first_name: Customer's first name
         :param code: Customer's code
-        :param kwargs:
-        :return: Response
+        :param kwargs: Data to be updated as keyword args
+        :return: Response Dict
         """
-        data = {'code': code, 'last_name': last_name, 'first_name': first_name, **kwargs}
+        data = kwargs
         return await self.put(url=self.url(f"{code}"), json=data)
 
-    async def validate(self, *, code: str, last_name: str, first_name: str, value: str,
-                       bvn: str, bank_code: str, account_number: str, type: str = "bank_account", country: str = "NG",  **kwargs):
+    async def validate(self, *, code: str, last_name: str, first_name: str,
+                       bvn: str, bank_code: str, account_number: str, type: str = "bank_account", country: str = "NG",
+                       **kwargs) -> Response:
         """
         Validate a customer's identity
         :param code: customer_identity code
         :param last_name: Customer's last name
         :param first_name: Customer's first name
         :param type: redefined types of identification. Only bank_account is supported at the moment
         :param value: Customer's identification number
         :param country: 2 letter country code of identification issuer
         :param bvn: Customer's Bank Verification Number
         :param bank_code: You can get the list of Bank Codes by calling the List Banks endpoint. (
         required if type is bank_account)
         :param account_number: Customer's bank account number. (required if type is bank_account)
         :param kwargs: Optional params as keyword args
-        :return: Response
+        :return: Response Dict
         """
-        data = {'code': code, 'last_name': last_name, 'first_name': first_name, 'type': type, 'value': value,
+        data = {'last_name': last_name, 'first_name': first_name, 'type': type,
                 'country': country, 'bvn': bvn, 'bank_code': bank_code, "account_number": account_number, **kwargs}
         return await self.post(url=self.url(f"{code}/identification"), json=data)
 
-    async def set_risk_action(self, *, customer: str, email: str, risk_action: Literal['default', 'deny', 'allow'] = 'default'):
+    async def set_risk_action(self, *, customer: str, email: str,
+                              risk_action: Literal['default', 'deny', 'allow'] = 'default') -> Response:
         """
         Whitelist or blacklist a customer on your integration
         :param email: Customer email
         :param customer: Customer's code
         :param risk_action: One of the possible risk actions [ default, allow, deny ]. allow to whitelist.
         deny to blacklist. Customers start with a default risk action.
-        :return: Response
+        :return: Response Dict
         """
         data = {'customer': customer, 'risk_action': risk_action, 'email': email}
         return await self.post(url=self.url(""), json=data)
 
-    async def deactivate_authorization(self, authorization_code: str):
+    async def deactivate_authorization(self, authorization_code: str) -> Response:
         """
         Deactivate an authorization when the card needs to be forgotten
         :param authorization_code: Authorization code to be deactivated
         :return: Response
         """
         data = {'authorization_code': authorization_code}
         return await self.post(url=self.url("deactivate_authorization"), json=data)
```

### Comparing `aiopaystack-1.0.0/src/paystack/dedicated_virtual_accounts.py` & `aiopaystack-2.0.0/src/paystack/dedicated_virtual_accounts.py`

 * *Files identical despite different names*

### Comparing `aiopaystack-1.0.0/src/paystack/disputes.py` & `aiopaystack-2.0.0/src/paystack/disputes.py`

 * *Files identical despite different names*

### Comparing `aiopaystack-1.0.0/src/paystack/invoices.py` & `aiopaystack-2.0.0/src/paystack/invoices.py`

 * *Files identical despite different names*

### Comparing `aiopaystack-1.0.0/src/paystack/misc.py` & `aiopaystack-2.0.0/src/paystack/misc.py`

 * *Files identical despite different names*

### Comparing `aiopaystack-1.0.0/src/paystack/page.py` & `aiopaystack-2.0.0/src/paystack/page.py`

 * *Files identical despite different names*

### Comparing `aiopaystack-1.0.0/src/paystack/paystack.py` & `aiopaystack-2.0.0/src/paystack/paystack.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import os
-
-from httpx import AsyncClient
+from http.client import HTTPSConnection
 
 
 class Paystack:
 
     def __new__(cls, *args, **kwargs):
         if not hasattr(cls, '_instance'):
             cls._instance = super().__new__(cls)
         return cls._instance
 
     def __init__(self, *, secret_key=""):
         self.secret_key = secret_key or os.getenv('PAY_STACK_SECRET_KEY') or getattr(self, 'secret_key', '')
-        self.headers = {"Authorization": f"Bearer {self.secret_key}"}
+        self.headers = {'Authorization': f'Bearer {self.secret_key}'}
 
     @property
-    def async_client(self):
-        return AsyncClient(headers=self.headers, base_url="https://api.paystack.co")
+    def client(self) -> HTTPSConnection:
+        client = HTTPSConnection('api.paystack.co')
+        return client
```

### Comparing `aiopaystack-1.0.0/src/paystack/plans.py` & `aiopaystack-2.0.0/src/paystack/plans.py`

 * *Files identical despite different names*

### Comparing `aiopaystack-1.0.0/src/paystack/products.py` & `aiopaystack-2.0.0/src/paystack/products.py`

 * *Files identical despite different names*

### Comparing `aiopaystack-1.0.0/src/paystack/refund.py` & `aiopaystack-2.0.0/src/paystack/refund.py`

 * *Files identical despite different names*

### Comparing `aiopaystack-1.0.0/src/paystack/settlements.py` & `aiopaystack-2.0.0/src/paystack/settlements.py`

 * *Files identical despite different names*

### Comparing `aiopaystack-1.0.0/src/paystack/subaccounts.py` & `aiopaystack-2.0.0/src/paystack/subaccounts.py`

 * *Files identical despite different names*

### Comparing `aiopaystack-1.0.0/src/paystack/subscriptions.py` & `aiopaystack-2.0.0/src/paystack/subscriptions.py`

 * *Files identical despite different names*

### Comparing `aiopaystack-1.0.0/src/paystack/transaction_splits.py` & `aiopaystack-2.0.0/src/paystack/transaction_splits.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,37 +1,40 @@
-from typing import Literal
 from datetime import datetime
+from typing import Literal
+
+from .base import Base, Response, Currency
 
-from .base import Base
+BearerType = Literal['subaccount', 'account', 'all-proportional', 'all']
 
 
 class TransactionSplits(Base):
     """
     The Transaction Splits API enables merchants split the settlement for a transaction across their payout account,
     and one or more Subaccounts.
     """
     def __init__(self):
         super().__init__()
         url = '/split/{}'
         self.url = url.format
 
-    async def create(self, *, name: str, type: Literal['percentage', 'flat'], currency: Literal['NGN', 'GHS', 'ZAR', 'USD'],
-                           subaccounts: list[dict], bearer_type: Literal['subaccount', 'account', 'all-proportional', 'all'], bearer_subaccount: str):
+    async def create(self, *, name: str, type: Literal['percentage', 'flat'], currency: Currency,
+                     subaccounts: list[dict], bearer_type: BearerType, bearer_subaccount: str) -> Response:
         """
         Create a split payment on your integration
         :param name: Name of the transaction split
         :param type: The type of transaction split you want to create. You can use one of the following: percentage | flat
         :param currency: Any of NGN, GHS, ZAR, or USD
-        :param subaccounts: A list of object containing subaccount code and number of shares:[{subaccount: ‘ACT_xxxxxxxxxx’, share: xxx},{...}]
+        :param subaccounts: A list of object containing subaccount code and number of shares:
+            eg. [{subaccount: ‘ACT_xxxxxxxxxx’, share: xxx},{...}]
         :param bearer_type: Any of subaccount | account | all-proportional | all
         :param bearer_subaccount: Subaccount code
-        :return: Response
+        :return: Response Dict
         """
-        data = {'name': name, 'type': type, 'currency': currency, 'subaccounts': subaccounts, 'bearer_type': bearer_type,
-                'bearer_subaccount': bearer_subaccount}
+        data = {'name': name, 'type': type, 'currency': currency, 'subaccounts': subaccounts,
+                'bearer_type': bearer_type, 'bearer_subaccount': bearer_subaccount}
         return await self.post(url=self.url(""), json=data)
 
     async def list(self, name: str, active: bool, from_: datetime | None | str = None, **kwargs):
         """
         List/search for the transaction splits available on your integration.
         :param name: The name of the split
         :param active: Any of true or false
```

### Comparing `aiopaystack-1.0.0/src/paystack/transactions.py` & `aiopaystack-2.0.0/src/paystack/transactions.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,130 +1,128 @@
-from typing import Literal
 from datetime import datetime
 
-from .base import Base
+from .base import Base, Response, Currency
 
 
 class Transactions(Base):
     """
     The Transactions API allows you create and manage payments on your integration
     """
     def __init__(self):
         super().__init__()
         url = '/transaction/{}'
         self.url = url.format
 
-    async def initialize(self, *, email: str, amount: str, **kwargs):
+    async def initialize(self, *, email: str, amount: str, **kwargs) -> Response:
         """
-        Initialize transaction. Email and amount are required fields
+        Initialize transaction from your backend. Email and amount are required fields
         :param amount: Amount should be in kobo if currency is NGN, pesewas, if currency is GHS, and cents, if currency is ZAR
         :param email: Customer's email address
         :param kwargs: optional params of request body as keyword arguments
-        :return: json data from paystack API as a dict
+        :return: Response Dict
         """
         data = {'email': email, 'amount': amount, **kwargs}
         return await self.post(url=self.url('initialize'), json=data)
 
     async def verify(self, *, reference: str):
         """
+        Confirm the status of a transaction.
         :param reference: The transaction reference used to initiate the transaction
-        :return: json data from paystack API
+        :return: Response Dict
         """
-        params = {'reference': reference}
-        return await self.get(url=self.url(f'verify/{reference}'), params=params)
+        return await self.get(url=self.url(f'verify/{reference}'))
 
     async def list(self, *, perPage: int = 50, page: int = 1, from_: datetime | None = None, **kwargs):
         """
         List transactions carried out on your integration.
-        :param page:    Specify exactly what page you want to retrieve. If not specify we use a default value of 1.
+        :param page: Specify exactly what page you want to retrieve. If not specify we use a default value of 1.
         :param perPage: Specify how many records you want to retrieve per page. If not specify we use a default value of 50.
         :param from_: from should be added this way
         :param kwargs: Optional query parameters as keyword arguments
-        :return: List of transactions as json data from paystack API
+        :return: Response Dict
         """
         params = {"perPage": perPage, "page": page, **kwargs}
         params.update(**{'from': from_}) if from_ else from_
         return await self.get(url=self.url(""), params=params)
 
     async def fetch(self, *, id):
         """
         Get details of a transaction carried out on your integration.
         :param id: id of a single transaction
-        :return: json data from paystack API
+        :return: Response Dict
         """
         return await self.get(url=self.url(f"{id}"))
 
     async def charge_authorization(self, *, amount: str, email: str, authorization_code: str,  **kwargs):
         """
         All authorizations marked as reusable can be charged with this endpoint whenever you need to receive payments.
         :param authorization_code: Valid authorization code to charge
         :param email: Customer's email address
         :param amount: Amount should be in kobo if currency is NGN, pesewas, if currency is GHS, and cents, if currency is ZAR
         :param kwargs: optional params of request body as keyword arguments
-        :return: json data from paystack API
+        :return: Response Dict
         """
         data = {'amount': amount, 'email': email, 'authorization_code': authorization_code, **kwargs}
         return await self.post(url=self.url("charge_authorization"), json=data)
 
     async def check_authorization(self, *, amount: str, email: str, authorization_code: str, **kwargs):
         """
         All Mastercard and Visa authorizations can be checked with this endpoint to know if they have
         funds for the payment you seek. This endpoint should be used when you do not know the exact amount to
         charge a card when rendering a service. It should be used to check if a card has enough funds based on
-        a maximum range value. It is well suited for:
-        Ride hailing services
+        a maximum range value. It is well suited for Ride hailing services
         Logistics services
         :param authorization_code: Valid authorization code to charge
         :param email: Customer's email address
         :param amount: Amount should be in kobo if currency is NGN, pesewas, if currency is GHS, and cents, if currency is ZAR
         :param kwargs: optional params of request body as keyword arguments
-        :return: json data from paystack API
+        :return: Response Dict
         """
         data = {'amount': amount, 'email': email, 'authorization_code': authorization_code, **kwargs}
         return await self.post(url=self.url("check_authorization"), json=data)
 
     async def view_transaction_timeline(self, *, id_or_reference: str):
         """
         View the timeline of a transaction
         :param id_or_reference: id or reference of transaction
-        :return: json data from paystack API
+        :return: Response Dict
         """
         params = {'id_or_reference': id_or_reference}
         return await self.get(url=self.url(f"timeline/{id_or_reference}"), params=params)
 
     async def transaction_totals(self, *, perPage: int = 50, page: int = 1, from_: datetime | None = None, to: datetime | None = None):
         """
         If you specify a page number also specify a results per page. eg page=1, perPage=10
         You can specify from and to as query parameters
         :param page: Specify exactly what page you want to retrieve. If not specify we use a default value of 1.
         :param perPage: Specify how many records you want to retrieve per page. If not specify we use a default value of 50.
         :param to: Specify exactly what page you want to retrieve. If not specify we use a default value of 1.
         :param from_: A timestamp from which to start listing transaction e.g. 2016-09-24T00:00:05.000Z, 2016-09-21
-        :return: Response
+        :return: Response Dict
         """
         params = {key: value for key, value in (('from', from_), ('to', to), ('perPage', perPage), ('page', page)) if value}
         return await self.get(url=self.url(f"totals/"), params=params)
 
     async def export_transactions(self, perPage: int = 50, page: int = 1, **kwargs):
         """
         If you specify a page number also specify a results per page. eg page=1, perPage=10
         :param perPage: Specify how many records you want to retrieve per page. If not specify we use a default value of 50.
         :param page: Specify exactly what page you want to retrieve. If not specify we use a default value of 1.
         :param kwargs:
-        :return: Response
+        :return: Response Dict
         """
         params = {'perPage': perPage, 'page': page, **kwargs}
         return await self.get(url=self.url("export"), params=params)
 
-    async def partial_debit(self, *, authorization_code: str, email: str, amount: str, currency: Literal['NGN', 'GHS', 'ZAR', 'USD'],  **kwargs):
+    async def partial_debit(self, *, authorization_code: str, email: str, amount: str, currency: Currency,  **kwargs):
         """
         Retrieve part of a payment from a customer
         authorization_code, currency, amount, email are required fields
         :param authorization_code: Valid authorization code to charge
         :param email: Customer's email address
         :param amount: Amount should be in kobo if currency is NGN, pesewas, if currency is GHS, and cents, if currency is ZAR
         :param currency: Specify the currency you want to debit. Allowed values are NGN, GHS, ZAR or USD.
         :param kwargs: keyword arguments form body of requests
-        :return: Response
+        :return: Response Dict
         """
         data = {'authorization_code': authorization_code, 'email': email, 'amount': amount, 'currency': currency, **kwargs}
         return await self.post(url=self.url("partial_debit"), json=data)
```

### Comparing `aiopaystack-1.0.0/src/paystack/transfer_control.py` & `aiopaystack-2.0.0/src/paystack/transfer_control.py`

 * *Files identical despite different names*

### Comparing `aiopaystack-1.0.0/src/paystack/transfer_recipient.py` & `aiopaystack-2.0.0/src/paystack/transfer_recipient.py`

 * *Files identical despite different names*

### Comparing `aiopaystack-1.0.0/src/paystack/transfers.py` & `aiopaystack-2.0.0/src/paystack/transfers.py`

 * *Files identical despite different names*

### Comparing `aiopaystack-1.0.0/src/paystack/verification.py` & `aiopaystack-2.0.0/src/paystack/verification.py`

 * *Files identical despite different names*

