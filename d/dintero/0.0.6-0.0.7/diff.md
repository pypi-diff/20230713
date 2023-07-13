# Comparing `tmp/dintero-0.0.6.tar.gz` & `tmp/dintero-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dintero-0.0.6.tar", last modified: Fri Jun 18 08:38:07 2021, max compression
+gzip compressed data, was "dintero-0.0.7.tar", last modified: Thu Jul 13 19:32:29 2023, max compression
```

## Comparing `dintero-0.0.6.tar` & `dintero-0.0.7.tar`

### file list

```diff
@@ -1,28 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-18 08:38:07.408474 dintero-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (121)     1064 2021-06-18 08:38:06.000000 dintero-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      130 2021-06-18 08:38:06.000000 dintero-0.0.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     3367 2021-06-18 08:38:07.408474 dintero-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1651 2021-06-18 08:38:06.000000 dintero-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-18 08:38:07.408474 dintero-0.0.6/dintero/
--rw-r--r--   0 runner    (1001) docker     (121)     1071 2021-06-18 08:38:06.000000 dintero-0.0.6/dintero/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9414 2021-06-18 08:38:06.000000 dintero-0.0.6/dintero/checkout.py
--rw-r--r--   0 runner    (1001) docker     (121)      475 2021-06-18 08:38:06.000000 dintero-0.0.6/dintero/error.py
--rw-r--r--   0 runner    (1001) docker     (121)      182 2021-06-18 08:38:06.000000 dintero-0.0.6/dintero/types.py
--rw-r--r--   0 runner    (1001) docker     (121)       18 2021-06-18 08:38:06.000000 dintero-0.0.6/dintero/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-18 08:38:07.408474 dintero-0.0.6/dintero.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3367 2021-06-18 08:38:07.000000 dintero-0.0.6/dintero.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      444 2021-06-18 08:38:07.000000 dintero-0.0.6/dintero.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-06-18 08:38:07.000000 dintero-0.0.6/dintero.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-06-18 08:38:07.000000 dintero-0.0.6/dintero.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       67 2021-06-18 08:38:07.000000 dintero-0.0.6/dintero.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2021-06-18 08:38:07.000000 dintero-0.0.6/dintero.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-18 08:38:07.408474 dintero-0.0.6/examples/
--rw-r--r--   0 runner    (1001) docker     (121)     1123 2021-06-18 08:38:06.000000 dintero-0.0.6/examples/create_session.py
--rw-r--r--   0 runner    (1001) docker     (121)      468 2021-06-18 08:38:06.000000 dintero-0.0.6/examples/manage_transaction.py
--rw-r--r--   0 runner    (1001) docker     (121)      139 2021-06-18 08:38:06.000000 dintero-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      102 2021-06-18 08:38:07.412474 dintero-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1915 2021-06-18 08:38:06.000000 dintero-0.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-18 08:38:07.408474 dintero-0.0.6/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-06-18 08:38:06.000000 dintero-0.0.6/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      261 2021-06-18 08:38:06.000000 dintero-0.0.6/tests/test_error.py
--rw-r--r--   0 runner    (1001) docker     (121)      850 2021-06-18 08:38:06.000000 dintero-0.0.6/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:32:29.304495 dintero-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-13 19:32:27.000000 dintero-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-13 19:32:27.000000 dintero-0.0.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2933 2023-07-13 19:32:29.304495 dintero-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-07-13 19:32:27.000000 dintero-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:32:29.304495 dintero-0.0.7/dintero/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-13 19:32:27.000000 dintero-0.0.7/dintero/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9495 2023-07-13 19:32:27.000000 dintero-0.0.7/dintero/checkout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-07-13 19:32:27.000000 dintero-0.0.7/dintero/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-07-13 19:32:27.000000 dintero-0.0.7/dintero/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-07-13 19:32:27.000000 dintero-0.0.7/dintero/validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-13 19:32:27.000000 dintero-0.0.7/dintero/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:32:29.304495 dintero-0.0.7/dintero.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2933 2023-07-13 19:32:29.000000 dintero-0.0.7/dintero.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-07-13 19:32:29.000000 dintero-0.0.7/dintero.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 19:32:29.000000 dintero-0.0.7/dintero.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 19:32:29.000000 dintero-0.0.7/dintero.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-13 19:32:29.000000 dintero-0.0.7/dintero.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-13 19:32:29.000000 dintero-0.0.7/dintero.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:32:29.304495 dintero-0.0.7/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-07-13 19:32:27.000000 dintero-0.0.7/examples/create_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-07-13 19:32:27.000000 dintero-0.0.7/examples/manage_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-13 19:32:27.000000 dintero-0.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-13 19:32:29.304495 dintero-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-07-13 19:32:27.000000 dintero-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:32:29.304495 dintero-0.0.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 19:32:27.000000 dintero-0.0.7/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-07-13 19:32:27.000000 dintero-0.0.7/tests/test_checkout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-07-13 19:32:27.000000 dintero-0.0.7/tests/test_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-07-13 19:32:27.000000 dintero-0.0.7/tox.ini
```

### Comparing `dintero-0.0.6/LICENSE` & `dintero-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `dintero-0.0.6/PKG-INFO` & `dintero-0.0.7/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,96 +1,99 @@
 Metadata-Version: 2.1
 Name: dintero
-Version: 0.0.6
+Version: 0.0.7
 Summary: Python bindings for the Dintero API
 Home-page: https://github.com/dintero/Dintero.Python.SDK
 Author: Dintero
 Author-email: integration@dintero.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/dintero/Dintero.Python.SDK/issues
 Project-URL: Documentation, https://docs.dintero.com
 Project-URL: Source Code, https://github.com/dintero/Dintero.Python.SDK
-Description: # Dintero Python SDK
-        
-        With the Dintero Python SDK you can easily interact with the Dintero API to create and manage payments through the
-        Checkout API, and in the future also use the many other APIs we've got.
-        
-        ## Installation
-        
-        Install from pip by using:
-        
-        ```
-        pip install --upgrade dintero
-        ```
-        
-        ### Requirements
-        
-        * Python 3.6+
-        
-        ## Using the SDK
-        
-        Create an account through https://onboarding.dintero.com.
-        
-        Get client credentials from the Dintero Backoffice, see [guide](https://docs.dintero.com/docs/checkout-client/).
-        
-        Create a payment profile by going to [Dintero Backoffice](https://backoffice.dintero.com) --> Settings --> Payment
-        Profiles
-        
-        Use your newly created credentials to create a session:
-        
-        ```python
-        from dintero import Dintero
-        
-        account_id = 'T12345678'
-        client_id = '72e023b1-aeda-498e-b141-4669528c44b9'
-        client_secret = '125f9f0a-e240-4bfd-be57-0086343bf0e4'
-        
-        profile_id = 'P12345678.46dP6T4F1mUXYPeYKYc5Gj'
-        
-        dintero = Dintero(
-            account_id,
-            client_id,
-            client_secret)
-        checkout = dintero.checkout()
-        session_info = checkout.create_session({
-            "url": {
-                "return_url": "https://example.com/accept",
-                "callback_url": "https://example.com/callback"
-            },
-            "order": {
-                "amount": 29990,
-                "currency": "NOK",
-                "merchant_reference": "string",
-                "items": [
-                    {
-                        "id": "chair-1",
-                        "line_id": "1",
-                        "description": "Stablestol",
-                        "quantity": 1,
-                        "amount": 29990,
-                        "vat_amount": 6000,
-                        "vat": 25
-                    }
-                ]
-            },
-            "profile_id": profile_id
-        })
-        
-        print(session_info)
-        ```
-        
 Keywords: dintero api payments
-Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+Provides-Extra: dev
+License-File: LICENSE
+
+# Dintero Python SDK
+
+![Build Status](https://github.com/dintero/Dintero.Python.SDK/actions/workflows/ci.yml/badge.svg)
+
+With the Dintero Python SDK you can easily interact with the Dintero API to create and manage payments through the
+Checkout API, and in the future also use the many other APIs we've got.
+
+## Installation
+
+Install from pip by using:
+
+```
+pip install --upgrade dintero
+```
+
+### Requirements
+
+* Python 3.6+
+
+## Using the SDK
+
+Create an account through https://onboarding.dintero.com.
+
+Get client credentials from the Dintero Backoffice, see [guide](https://docs.dintero.com/docs/checkout-client/).
+
+Create a payment profile by going to [Dintero Backoffice](https://backoffice.dintero.com) --> Settings --> Payment
+Profiles
+
+Use your newly created credentials to create a session:
+
+```python
+from dintero import Dintero
+
+account_id = 'T12345678'
+client_id = '72e023b1-aeda-498e-b141-4669528c44b9'
+client_secret = '125f9f0a-e240-4bfd-be57-0086343bf0e4'
+
+profile_id = 'T12345678.46dP6T4F1mUXYPeYKYc5Gj'
+
+dintero = Dintero(
+    account_id,
+    client_id,
+    client_secret)
+checkout = dintero.checkout()
+session_info = checkout.create_session({
+    "url": {
+        "return_url": "https://example.com/accept",
+        "callback_url": "https://example.com/callback"
+    },
+    "order": {
+        "amount": 29990,
+        "currency": "NOK",
+        "merchant_reference": "string",
+        "items": [
+            {
+                "id": "chair-1",
+                "line_id": "1",
+                "description": "Stablestol",
+                "quantity": 1,
+                "amount": 29990,
+                "vat_amount": 6000,
+                "vat": 25
+            }
+        ]
+    },
+    "profile_id": profile_id
+})
+
+print(session_info)
+```
```

### Comparing `dintero-0.0.6/README.md` & `dintero-0.0.7/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # Dintero Python SDK
 
+![Build Status](https://github.com/dintero/Dintero.Python.SDK/actions/workflows/ci.yml/badge.svg)
+
 With the Dintero Python SDK you can easily interact with the Dintero API to create and manage payments through the
 Checkout API, and in the future also use the many other APIs we've got.
 
 ## Installation
 
 Install from pip by using:
 
@@ -29,15 +31,15 @@
 ```python
 from dintero import Dintero
 
 account_id = 'T12345678'
 client_id = '72e023b1-aeda-498e-b141-4669528c44b9'
 client_secret = '125f9f0a-e240-4bfd-be57-0086343bf0e4'
 
-profile_id = 'P12345678.46dP6T4F1mUXYPeYKYc5Gj'
+profile_id = 'T12345678.46dP6T4F1mUXYPeYKYc5Gj'
 
 dintero = Dintero(
     account_id,
     client_id,
     client_secret)
 checkout = dintero.checkout()
 session_info = checkout.create_session({
```

### Comparing `dintero-0.0.6/dintero/__init__.py` & `dintero-0.0.7/dintero/__init__.py`

 * *Files identical despite different names*

### Comparing `dintero-0.0.6/dintero/checkout.py` & `dintero-0.0.7/dintero/checkout.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import json
 from typing import List, Union
 import requests
 import time
 
 from dintero.error import InvalidRequestBody, AuthError, UnexpectedError
 from dintero.types import Item
+from dintero.validator import validate_session
 
 _default_headers = {
     "Dintero-System-Name": "python-application",
     "Dintero-System-Version": "0.0.0",
     "Dintero-System-Plugin-Name": "python-sdk",
     "Dintero-System-Plugin-Version": "0.0.0",
 }
@@ -54,14 +55,15 @@
 
         If the session contains a profile_id, the configuration from
         the profile_id will be used.
 
         :param session: The payload of the session to create
         :return: The id of the session and an URL to redirect to
         """
+        validate_session(session)
         url = f"{self.checkout_url}/v1/sessions"
         if "profile_id" in session and session["profile_id"]:
             # Override and use sessions-profile endpoint
             url = f"{self.checkout_url}/v1/sessions-profile"
 
         response = requests.post(
             url,
```

### Comparing `dintero-0.0.6/dintero.egg-info/PKG-INFO` & `dintero-0.0.7/dintero.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,96 +1,99 @@
 Metadata-Version: 2.1
 Name: dintero
-Version: 0.0.6
+Version: 0.0.7
 Summary: Python bindings for the Dintero API
 Home-page: https://github.com/dintero/Dintero.Python.SDK
 Author: Dintero
 Author-email: integration@dintero.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/dintero/Dintero.Python.SDK/issues
 Project-URL: Documentation, https://docs.dintero.com
 Project-URL: Source Code, https://github.com/dintero/Dintero.Python.SDK
-Description: # Dintero Python SDK
-        
-        With the Dintero Python SDK you can easily interact with the Dintero API to create and manage payments through the
-        Checkout API, and in the future also use the many other APIs we've got.
-        
-        ## Installation
-        
-        Install from pip by using:
-        
-        ```
-        pip install --upgrade dintero
-        ```
-        
-        ### Requirements
-        
-        * Python 3.6+
-        
-        ## Using the SDK
-        
-        Create an account through https://onboarding.dintero.com.
-        
-        Get client credentials from the Dintero Backoffice, see [guide](https://docs.dintero.com/docs/checkout-client/).
-        
-        Create a payment profile by going to [Dintero Backoffice](https://backoffice.dintero.com) --> Settings --> Payment
-        Profiles
-        
-        Use your newly created credentials to create a session:
-        
-        ```python
-        from dintero import Dintero
-        
-        account_id = 'T12345678'
-        client_id = '72e023b1-aeda-498e-b141-4669528c44b9'
-        client_secret = '125f9f0a-e240-4bfd-be57-0086343bf0e4'
-        
-        profile_id = 'P12345678.46dP6T4F1mUXYPeYKYc5Gj'
-        
-        dintero = Dintero(
-            account_id,
-            client_id,
-            client_secret)
-        checkout = dintero.checkout()
-        session_info = checkout.create_session({
-            "url": {
-                "return_url": "https://example.com/accept",
-                "callback_url": "https://example.com/callback"
-            },
-            "order": {
-                "amount": 29990,
-                "currency": "NOK",
-                "merchant_reference": "string",
-                "items": [
-                    {
-                        "id": "chair-1",
-                        "line_id": "1",
-                        "description": "Stablestol",
-                        "quantity": 1,
-                        "amount": 29990,
-                        "vat_amount": 6000,
-                        "vat": 25
-                    }
-                ]
-            },
-            "profile_id": profile_id
-        })
-        
-        print(session_info)
-        ```
-        
 Keywords: dintero api payments
-Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+Provides-Extra: dev
+License-File: LICENSE
+
+# Dintero Python SDK
+
+![Build Status](https://github.com/dintero/Dintero.Python.SDK/actions/workflows/ci.yml/badge.svg)
+
+With the Dintero Python SDK you can easily interact with the Dintero API to create and manage payments through the
+Checkout API, and in the future also use the many other APIs we've got.
+
+## Installation
+
+Install from pip by using:
+
+```
+pip install --upgrade dintero
+```
+
+### Requirements
+
+* Python 3.6+
+
+## Using the SDK
+
+Create an account through https://onboarding.dintero.com.
+
+Get client credentials from the Dintero Backoffice, see [guide](https://docs.dintero.com/docs/checkout-client/).
+
+Create a payment profile by going to [Dintero Backoffice](https://backoffice.dintero.com) --> Settings --> Payment
+Profiles
+
+Use your newly created credentials to create a session:
+
+```python
+from dintero import Dintero
+
+account_id = 'T12345678'
+client_id = '72e023b1-aeda-498e-b141-4669528c44b9'
+client_secret = '125f9f0a-e240-4bfd-be57-0086343bf0e4'
+
+profile_id = 'T12345678.46dP6T4F1mUXYPeYKYc5Gj'
+
+dintero = Dintero(
+    account_id,
+    client_id,
+    client_secret)
+checkout = dintero.checkout()
+session_info = checkout.create_session({
+    "url": {
+        "return_url": "https://example.com/accept",
+        "callback_url": "https://example.com/callback"
+    },
+    "order": {
+        "amount": 29990,
+        "currency": "NOK",
+        "merchant_reference": "string",
+        "items": [
+            {
+                "id": "chair-1",
+                "line_id": "1",
+                "description": "Stablestol",
+                "quantity": 1,
+                "amount": 29990,
+                "vat_amount": 6000,
+                "vat": 25
+            }
+        ]
+    },
+    "profile_id": profile_id
+})
+
+print(session_info)
+```
```

### Comparing `dintero-0.0.6/examples/create_session.py` & `dintero-0.0.7/examples/create_session.py`

 * *Files identical despite different names*

### Comparing `dintero-0.0.6/setup.py` & `dintero-0.0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,19 @@
     keywords="dintero api payments",
     packages=find_packages(exclude=["tests", "tests.*"]),
     zip_safe=False,
     install_requires=[
         'requests >= 2.20; python_version >= "3.0"',
         'typing_extensions >= 3.10; python_version >= "3.0"',
     ],
+    extras_require={
+        "dev": [
+            "pytest",
+        ]
+    },
     python_requires=">=3.6",
     project_urls={
         "Bug Tracker": "https://github.com/dintero/Dintero.Python.SDK/issues",
         "Documentation": "https://docs.dintero.com",
         "Source Code": "https://github.com/dintero/Dintero.Python.SDK",
     },
     classifiers=[
```

### Comparing `dintero-0.0.6/tox.ini` & `dintero-0.0.7/tox.ini`

 * *Files 15% similar despite different names*

```diff
@@ -11,25 +11,34 @@
     --cov-report=term-missing
 
 [testenv]
 description = run the unit tests under {basepython}
 setenv =
     COVERAGE_FILE = {toxworkdir}/.coverage.{envname}
 deps =
-    coverage >= 4.5.3, < 5 # TODO: upgrade to coverage 5 when we drop support for Python 3.4
-    py{310,39,38,37,36,py3}: pytest >= 6.0.0
-    pytest-cov >= 2.8.1, < 2.11.0
-commands = pytest --cov
+    coverage >= 5.5
+    pytest >= 6.0.0
+    pytest-cov >= 2.12.1
+depends =
+    report: py310
+commands = pytest --cov --cov-append
+
+[testenv:report]
+deps = coverage
+skip_install = true
+commands =
+    coverage report
+    coverage html
 
 [testenv:fmt]
 description = run code formatting using black
-basepython = python3.9
-deps = black==20.8b1
+basepython = python3.10
+deps = black==23.7.0
 commands = black . {posargs}
 skip_install = true
 
 [testenv:lint]
 description = run static analysis and style check using flake8
-basepython = python3.6
+basepython = python3.10
 deps = flake8
 commands = python -m flake8 --show-source dintero tests setup.py
 skip_install = true
```

