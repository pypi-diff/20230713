# Comparing `tmp/aptos_sdk-0.6.3.tar.gz` & `tmp/aptos_sdk-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aptos_sdk-0.6.3.tar", max compression
+gzip compressed data, was "aptos_sdk-0.6.4.tar", max compression
```

## Comparing `aptos_sdk-0.6.3.tar` & `aptos_sdk-0.6.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     2746 2023-06-03 10:15:17.666676 aptos_sdk-0.6.3/README.md
--rw-r--r--   0        0        0       70 2023-05-26 05:51:23.736675 aptos_sdk-0.6.3/aptos_sdk/__init__.py
--rw-r--r--   0        0        0     5651 2023-05-26 05:51:23.723342 aptos_sdk-0.6.3/aptos_sdk/account.py
--rw-r--r--   0        0        0     5873 2023-05-26 05:51:23.630008 aptos_sdk-0.6.3/aptos_sdk/account_address.py
--rw-r--r--   0        0        0     8546 2023-06-09 00:05:39.956760 aptos_sdk-0.6.3/aptos_sdk/account_sequence_number.py
--rw-r--r--   0        0        0    20257 2023-06-09 02:20:19.940022 aptos_sdk-0.6.3/aptos_sdk/aptos_token_client.py
--rw-r--r--   0        0        0    27697 2023-06-09 02:20:19.943356 aptos_sdk-0.6.3/aptos_sdk/async_client.py
--rw-r--r--   0        0        0     5811 2023-05-26 05:51:23.743342 aptos_sdk-0.6.3/aptos_sdk/authenticator.py
--rw-r--r--   0        0        0    10447 2023-05-26 05:51:23.720008 aptos_sdk-0.6.3/aptos_sdk/bcs.py
--rw-r--r--   0        0        0    24350 2023-06-09 02:20:19.910022 aptos_sdk-0.6.3/aptos_sdk/client.py
--rw-r--r--   0        0        0    12056 2023-05-26 05:51:23.716675 aptos_sdk-0.6.3/aptos_sdk/ed25519.py
--rw-r--r--   0        0        0      277 2023-06-03 10:15:17.666676 aptos_sdk-0.6.3/aptos_sdk/metadata.py
--rw-r--r--   0        0        0     8405 2023-06-09 00:05:39.910093 aptos_sdk-0.6.3/aptos_sdk/transaction_worker.py
--rw-r--r--   0        0        0    26552 2023-06-09 02:20:19.920022 aptos_sdk-0.6.3/aptos_sdk/transactions.py
--rw-r--r--   0        0        0     8991 2023-05-26 05:51:23.730008 aptos_sdk-0.6.3/aptos_sdk/type_tag.py
--rw-r--r--   0        0        0      762 2023-06-09 01:08:05.026671 aptos_sdk-0.6.3/pyproject.toml
--rw-r--r--   0        0        0     3628 1970-01-01 00:00:00.000000 aptos_sdk-0.6.3/PKG-INFO
+-rw-r--r--   0        0        0     2746 2023-07-03 23:02:13.166668 aptos_sdk-0.6.4/README.md
+-rw-r--r--   0        0        0       70 2023-07-03 17:38:08.063361 aptos_sdk-0.6.4/aptos_sdk/__init__.py
+-rw-r--r--   0        0        0     5651 2023-07-03 17:38:08.063361 aptos_sdk-0.6.4/aptos_sdk/account.py
+-rw-r--r--   0        0        0     5873 2023-07-03 17:38:08.063361 aptos_sdk-0.6.4/aptos_sdk/account_address.py
+-rw-r--r--   0        0        0     8546 2023-07-03 23:02:13.166668 aptos_sdk-0.6.4/aptos_sdk/account_sequence_number.py
+-rw-r--r--   0        0        0    20257 2023-07-10 13:13:45.680059 aptos_sdk-0.6.4/aptos_sdk/aptos_token_client.py
+-rw-r--r--   0        0        0    27697 2023-07-10 13:13:45.703392 aptos_sdk-0.6.4/aptos_sdk/async_client.py
+-rw-r--r--   0        0        0     5811 2023-07-13 18:30:47.912625 aptos_sdk-0.6.4/aptos_sdk/authenticator.py
+-rw-r--r--   0        0        0    10447 2023-07-03 17:38:08.063361 aptos_sdk-0.6.4/aptos_sdk/bcs.py
+-rw-r--r--   0        0        0    24385 2023-07-13 18:31:05.182625 aptos_sdk-0.6.4/aptos_sdk/client.py
+-rw-r--r--   0        0        0    12056 2023-07-03 17:38:08.063361 aptos_sdk-0.6.4/aptos_sdk/ed25519.py
+-rw-r--r--   0        0        0      277 2023-07-03 23:02:13.166668 aptos_sdk-0.6.4/aptos_sdk/metadata.py
+-rw-r--r--   0        0        0     8541 2023-07-03 23:02:13.166668 aptos_sdk-0.6.4/aptos_sdk/transaction_worker.py
+-rw-r--r--   0        0        0    26552 2023-07-10 13:13:45.686725 aptos_sdk-0.6.4/aptos_sdk/transactions.py
+-rw-r--r--   0        0        0     8991 2023-07-03 17:38:08.063361 aptos_sdk-0.6.4/aptos_sdk/type_tag.py
+-rw-r--r--   0        0        0      782 2023-07-13 19:14:56.392619 aptos_sdk-0.6.4/pyproject.toml
+-rw-r--r--   0        0        0     3663 1970-01-01 00:00:00.000000 aptos_sdk-0.6.4/PKG-INFO
```

### Comparing `aptos_sdk-0.6.3/README.md` & `aptos_sdk-0.6.4/README.md`

 * *Files identical despite different names*

### Comparing `aptos_sdk-0.6.3/aptos_sdk/account.py` & `aptos_sdk-0.6.4/aptos_sdk/account.py`

 * *Files identical despite different names*

### Comparing `aptos_sdk-0.6.3/aptos_sdk/account_address.py` & `aptos_sdk-0.6.4/aptos_sdk/account_address.py`

 * *Files identical despite different names*

### Comparing `aptos_sdk-0.6.3/aptos_sdk/account_sequence_number.py` & `aptos_sdk-0.6.4/aptos_sdk/account_sequence_number.py`

 * *Files identical despite different names*

### Comparing `aptos_sdk-0.6.3/aptos_sdk/aptos_token_client.py` & `aptos_sdk-0.6.4/aptos_sdk/aptos_token_client.py`

 * *Files identical despite different names*

### Comparing `aptos_sdk-0.6.3/aptos_sdk/async_client.py` & `aptos_sdk-0.6.4/aptos_sdk/async_client.py`

 * *Files identical despite different names*

### Comparing `aptos_sdk-0.6.3/aptos_sdk/authenticator.py` & `aptos_sdk-0.6.4/aptos_sdk/authenticator.py`

 * *Files identical despite different names*

### Comparing `aptos_sdk-0.6.3/aptos_sdk/bcs.py` & `aptos_sdk-0.6.4/aptos_sdk/bcs.py`

 * *Files identical despite different names*

### Comparing `aptos_sdk-0.6.3/aptos_sdk/client.py` & `aptos_sdk-0.6.4/aptos_sdk/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Copyright © Aptos Foundation
 # SPDX-License-Identifier: Apache-2.0
 
 import time
 from typing import Any, Dict, List
 
-import httpx
+import requests
 
 from . import ed25519
 from .account import Account
 from .account_address import AccountAddress
 from .authenticator import Authenticator, Ed25519Authenticator, MultiAgentAuthenticator
 from .bcs import Serializer
 from .metadata import Metadata
@@ -34,22 +34,24 @@
     transaction_wait_in_seconds: int = 20
 
 
 class RestClient:
     """A wrapper around the Aptos-core Rest API"""
 
     chain_id: int
-    client: httpx.Client
+    client: requests.Session
     client_config: ClientConfig
     base_url: str
 
     def __init__(self, base_url: str, client_config: ClientConfig = ClientConfig()):
         self.base_url = base_url
-        self.client = httpx.Client()
-        self.client.headers[Metadata.APTOS_HEADER] = Metadata.get_aptos_header_val()
+        self.client = requests.Session()
+        self.client.headers.update(
+            {Metadata.APTOS_HEADER: Metadata.get_aptos_header_val()}
+        )
         self.client_config = client_config
         self.chain_id = int(self.info()["chain_id"])
 
     def close(self):
         self.client.close()
 
     #
@@ -201,28 +203,28 @@
             )
         )
         signed_transaction = SignedTransaction(transaction, authenticator)
 
         headers = {"Content-Type": "application/x.aptos.signed_transaction+bcs"}
         response = self.client.post(
             f"{self.base_url}/transactions/simulate",
+            data=signed_transaction.bytes(),
             headers=headers,
-            content=signed_transaction.bytes(),
         )
         if response.status_code >= 400:
             raise ApiError(response.text, response.status_code)
 
         return response.json()
 
     def submit_bcs_transaction(self, signed_transaction: SignedTransaction) -> str:
         headers = {"Content-Type": "application/x.aptos.signed_transaction+bcs"}
         response = self.client.post(
             f"{self.base_url}/transactions",
+            data=signed_transaction.bytes(),
             headers=headers,
-            content=signed_transaction.bytes(),
         )
         if response.status_code >= 400:
             raise ApiError(response.text, response.status_code)
         return response.json()["hash"]
 
     def submit_transaction(self, sender: Account, payload: Dict[str, Any]) -> str:
         """
```

### Comparing `aptos_sdk-0.6.3/aptos_sdk/ed25519.py` & `aptos_sdk-0.6.4/aptos_sdk/ed25519.py`

 * *Files identical despite different names*

### Comparing `aptos_sdk-0.6.3/aptos_sdk/transaction_worker.py` & `aptos_sdk-0.6.4/aptos_sdk/transaction_worker.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,14 +45,17 @@
             [Account, int], typing.Awaitable[SignedTransaction]
         ],
     ):
         self._account = account
         self._account_sequence_number = AccountSequenceNumber(
             rest_client, account.address()
         )
+        self._account_sequence_number.maximum_wait_time = (
+            rest_client.client_config.transaction_wait_in_seconds
+        )
         self._rest_client = rest_client
         self._transaction_generator = transaction_generator
 
         self._started = False
         self._stopped = False
         self._outstanding_transactions = asyncio.Queue()
         self._processed_transactions = asyncio.Queue()
```

### Comparing `aptos_sdk-0.6.3/aptos_sdk/transactions.py` & `aptos_sdk-0.6.4/aptos_sdk/transactions.py`

 * *Files identical despite different names*

### Comparing `aptos_sdk-0.6.3/aptos_sdk/type_tag.py` & `aptos_sdk-0.6.4/aptos_sdk/type_tag.py`

 * *Files identical despite different names*

### Comparing `aptos_sdk-0.6.3/pyproject.toml` & `aptos_sdk-0.6.4/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 [tool.poetry]
 name = "aptos-sdk"
-version = "0.6.3"
+version = "0.6.4"
 description = "Aptos SDK"
 authors = ["Aptos Labs <opensource@aptoslabs.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 repository = "https://github.com/aptos-labs/aptos-core"
 homepage = "https://github.com/aptos-labs/aptos-core/tree/main/ecosystem/python/sdk"
 keywords = ["web3", "sdk", "aptos", "blockchain"]
 
 [tool.poetry.dependencies]
 h2 = "^4.1.0"
 httpx = "^0.23.0"
 PyNaCl = "^1.5.0"
 python = ">=3.7,<4.0"
+requests = "2.28.2"
 
 [tool.poetry.dev-dependencies]
 autoflake = "1.4.0"
 black = "^22.6.0"
 coverage = "^7.2.4"
 flake8 = ">=3.8.3,<6.0.0"
 isort = "^5.10.1"
```

### Comparing `aptos_sdk-0.6.3/PKG-INFO` & `aptos_sdk-0.6.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aptos-sdk
-Version: 0.6.3
+Version: 0.6.4
 Summary: Aptos SDK
 Home-page: https://github.com/aptos-labs/aptos-core/tree/main/ecosystem/python/sdk
 License: Apache-2.0
 Keywords: web3,sdk,aptos,blockchain
 Author: Aptos Labs
 Author-email: opensource@aptoslabs.com
 Requires-Python: >=3.7,<4.0
@@ -14,14 +14,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: PyNaCl (>=1.5.0,<2.0.0)
 Requires-Dist: h2 (>=4.1.0,<5.0.0)
 Requires-Dist: httpx (>=0.23.0,<0.24.0)
+Requires-Dist: requests (==2.28.2)
 Project-URL: Repository, https://github.com/aptos-labs/aptos-core
 Description-Content-Type: text/markdown
 
 # Aptos Python SDK
 [![Discord][discord-image]][discord-url]
 [![PyPI Package Version][pypi-image-version]][pypi-url]
 [![PyPI Package Downloads][pypi-image-downloads]][pypi-url]
```

