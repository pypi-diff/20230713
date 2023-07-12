# Comparing `tmp/algocash-sdk-1.2.0.tar.gz` & `tmp/algocash-sdk-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "algocash-sdk-1.2.0.tar", last modified: Tue Jun 20 09:15:45 2023, max compression
+gzip compressed data, was "algocash-sdk-1.3.0.tar", last modified: Wed Jul 12 23:25:08 2023, max compression
```

## Comparing `algocash-sdk-1.2.0.tar` & `algocash-sdk-1.3.0.tar`

### file list

```diff
@@ -1,53 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 09:15:45.487049 algocash-sdk-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-20 09:15:45.487049 algocash-sdk-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-06-20 09:15:35.000000 algocash-sdk-1.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 09:15:45.483049 algocash-sdk-1.2.0/algocash_sdk/
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-06-20 09:15:35.000000 algocash-sdk-1.2.0/algocash_sdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 09:15:45.483049 algocash-sdk-1.2.0/algocash_sdk/api/
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-20 09:15:35.000000 algocash-sdk-1.2.0/algocash_sdk/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-06-20 09:15:35.000000 algocash-sdk-1.2.0/algocash_sdk/api/deposit_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3578 2023-06-20 09:15:35.000000 algocash-sdk-1.2.0/algocash_sdk/api/payout_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    27823 2023-06-20 09:15:35.000000 algocash-sdk-1.2.0/algocash_sdk/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     8724 2023-06-20 09:15:35.000000 algocash-sdk-1.2.0/algocash_sdk/configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 09:15:45.483049 algocash-sdk-1.2.0/algocash_sdk/models/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-20 09:15:35.000000 algocash-sdk-1.2.0/algocash_sdk/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4618 2023-06-20 09:15:35.000000 algocash-sdk-1.2.0/algocash_sdk/models/address.py
--rw-r--r--   0 runner    (1001) docker     (123)     6268 2023-06-20 09:15:35.000000 algocash-sdk-1.2.0/algocash_sdk/models/bank.py
--rw-r--r--   0 runner    (1001) docker     (123)     8287 2023-06-20 09:15:35.000000 algocash-sdk-1.2.0/algocash_sdk/models/callback_payload.py
--rw-r--r--   0 runner    (1001) docker     (123)     5951 2023-06-20 09:15:35.000000 algocash-sdk-1.2.0/algocash_sdk/models/deposit_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     7837 2023-06-20 09:15:35.000000 algocash-sdk-1.2.0/algocash_sdk/models/deposit_status_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     3525 2023-06-20 09:15:35.000000 algocash-sdk-1.2.0/algocash_sdk/models/deposit_status_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4685 2023-06-20 09:15:35.000000 algocash-sdk-1.2.0/algocash_sdk/models/deposit_success.py
--rw-r--r--   0 runner    (1001) docker     (123)     4021 2023-06-20 09:15:35.000000 algocash-sdk-1.2.0/algocash_sdk/models/error.py
--rw-r--r--   0 runner    (1001) docker     (123)     6747 2023-06-20 09:15:35.000000 algocash-sdk-1.2.0/algocash_sdk/models/payer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6671 2023-06-20 09:15:35.000000 algocash-sdk-1.2.0/algocash_sdk/models/payout_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     6903 2023-06-20 09:15:35.000000 algocash-sdk-1.2.0/algocash_sdk/models/payout_status_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     3510 2023-06-20 09:15:35.000000 algocash-sdk-1.2.0/algocash_sdk/models/payout_status_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3928 2023-06-20 09:15:35.000000 algocash-sdk-1.2.0/algocash_sdk/models/payout_success.py
--rw-r--r--   0 runner    (1001) docker     (123)     5874 2023-06-20 09:15:35.000000 algocash-sdk-1.2.0/algocash_sdk/models/url.py
--rw-r--r--   0 runner    (1001) docker     (123)    12905 2023-06-20 09:15:35.000000 algocash-sdk-1.2.0/algocash_sdk/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 09:15:45.483049 algocash-sdk-1.2.0/algocash_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-20 09:15:45.000000 algocash-sdk-1.2.0/algocash_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-06-20 09:15:45.000000 algocash-sdk-1.2.0/algocash_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 09:15:45.000000 algocash-sdk-1.2.0/algocash_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-20 09:15:45.000000 algocash-sdk-1.2.0/algocash_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-20 09:15:45.000000 algocash-sdk-1.2.0/algocash_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 09:15:45.487049 algocash-sdk-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-06-20 09:15:35.000000 algocash-sdk-1.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 09:15:45.487049 algocash-sdk-1.2.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-20 09:15:35.000000 algocash-sdk-1.2.0/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-06-20 09:15:35.000000 algocash-sdk-1.2.0/test/server.py
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-06-20 09:15:35.000000 algocash-sdk-1.2.0/test/test_address.py
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-06-20 09:15:35.000000 algocash-sdk-1.2.0/test/test_bank.py
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-06-20 09:15:35.000000 algocash-sdk-1.2.0/test/test_callback_payload.py
--rw-r--r--   0 runner    (1001) docker     (123)     2144 2023-06-20 09:15:35.000000 algocash-sdk-1.2.0/test/test_deposit_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-06-20 09:15:35.000000 algocash-sdk-1.2.0/test/test_deposit_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-06-20 09:15:35.000000 algocash-sdk-1.2.0/test/test_deposit_status_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-06-20 09:15:35.000000 algocash-sdk-1.2.0/test/test_deposit_success.py
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-06-20 09:15:35.000000 algocash-sdk-1.2.0/test/test_error.py
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-06-20 09:15:35.000000 algocash-sdk-1.2.0/test/test_payer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-06-20 09:15:35.000000 algocash-sdk-1.2.0/test/test_payout_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-06-20 09:15:35.000000 algocash-sdk-1.2.0/test/test_payout_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-06-20 09:15:35.000000 algocash-sdk-1.2.0/test/test_payout_status_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-06-20 09:15:35.000000 algocash-sdk-1.2.0/test/test_payout_success.py
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-06-20 09:15:35.000000 algocash-sdk-1.2.0/test/test_url.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 23:25:08.604491 algocash-sdk-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-12 23:25:08.604491 algocash-sdk-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-07-12 23:24:56.000000 algocash-sdk-1.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 23:25:08.600491 algocash-sdk-1.3.0/algocash_sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-12 23:24:56.000000 algocash-sdk-1.3.0/algocash_sdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 23:25:08.604491 algocash-sdk-1.3.0/algocash_sdk/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-07-12 23:24:56.000000 algocash-sdk-1.3.0/algocash_sdk/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-07-12 23:24:56.000000 algocash-sdk-1.3.0/algocash_sdk/api/deposit_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3578 2023-07-12 23:24:56.000000 algocash-sdk-1.3.0/algocash_sdk/api/payout_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27858 2023-07-12 23:24:56.000000 algocash-sdk-1.3.0/algocash_sdk/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-07-12 23:24:56.000000 algocash-sdk-1.3.0/algocash_sdk/callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8724 2023-07-12 23:24:56.000000 algocash-sdk-1.3.0/algocash_sdk/configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 23:25:08.604491 algocash-sdk-1.3.0/algocash_sdk/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-12 23:24:56.000000 algocash-sdk-1.3.0/algocash_sdk/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4618 2023-07-12 23:24:56.000000 algocash-sdk-1.3.0/algocash_sdk/models/address.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6268 2023-07-12 23:24:56.000000 algocash-sdk-1.3.0/algocash_sdk/models/bank.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8287 2023-07-12 23:24:56.000000 algocash-sdk-1.3.0/algocash_sdk/models/callback_payload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5951 2023-07-12 23:24:56.000000 algocash-sdk-1.3.0/algocash_sdk/models/deposit_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7837 2023-07-12 23:24:56.000000 algocash-sdk-1.3.0/algocash_sdk/models/deposit_status_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3525 2023-07-12 23:24:56.000000 algocash-sdk-1.3.0/algocash_sdk/models/deposit_status_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4685 2023-07-12 23:24:56.000000 algocash-sdk-1.3.0/algocash_sdk/models/deposit_success.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4021 2023-07-12 23:24:56.000000 algocash-sdk-1.3.0/algocash_sdk/models/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6747 2023-07-12 23:24:56.000000 algocash-sdk-1.3.0/algocash_sdk/models/payer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6671 2023-07-12 23:24:56.000000 algocash-sdk-1.3.0/algocash_sdk/models/payout_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6903 2023-07-12 23:24:56.000000 algocash-sdk-1.3.0/algocash_sdk/models/payout_status_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3510 2023-07-12 23:24:56.000000 algocash-sdk-1.3.0/algocash_sdk/models/payout_status_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3928 2023-07-12 23:24:56.000000 algocash-sdk-1.3.0/algocash_sdk/models/payout_success.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5874 2023-07-12 23:24:56.000000 algocash-sdk-1.3.0/algocash_sdk/models/url.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12905 2023-07-12 23:24:56.000000 algocash-sdk-1.3.0/algocash_sdk/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 23:25:08.604491 algocash-sdk-1.3.0/algocash_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-12 23:25:08.000000 algocash-sdk-1.3.0/algocash_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-07-12 23:25:08.000000 algocash-sdk-1.3.0/algocash_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 23:25:08.000000 algocash-sdk-1.3.0/algocash_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-12 23:25:08.000000 algocash-sdk-1.3.0/algocash_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-12 23:25:08.000000 algocash-sdk-1.3.0/algocash_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 23:25:08.604491 algocash-sdk-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-12 23:24:56.000000 algocash-sdk-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 23:25:08.604491 algocash-sdk-1.3.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-12 23:24:56.000000 algocash-sdk-1.3.0/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-07-12 23:24:56.000000 algocash-sdk-1.3.0/test/test_callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-07-12 23:24:56.000000 algocash-sdk-1.3.0/test/test_deposit_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-07-12 23:24:56.000000 algocash-sdk-1.3.0/test/test_deposit_status_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-07-12 23:24:56.000000 algocash-sdk-1.3.0/test/test_payout_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-07-12 23:24:56.000000 algocash-sdk-1.3.0/test/test_payout_status_api.py
```

### Comparing `algocash-sdk-1.2.0/README.md` & `algocash-sdk-1.3.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -44,15 +44,31 @@
     pprint(api_response)
 except ValueError as e:
             print("ValueError Exception when calling DepositApi->create_deposit: %s\n" % e)
 except ApiException as e:
     print("Exception when calling DepositApi->create_deposit: %s\n" % e)
     pprint(json.loads(e.body))
 ```
-
+### Callback Payload
+```python
+import algocash_sdk
+from algocash_sdk.callback import SignatureVerificationException
+try:
+    callback = algocash_sdk.Callback()
+    data = callback.construct_callback(payload.decode('utf-8'), 'Header_Signature', 'access_token')
+    print(data)
+except SignatureVerificationException as e:
+    print("SignatureVerificationException when listening callback: %s\n" % e)
+    self.send_response(401)
+except ValueError as e:
+    print("ValueError Exception when listening callback: %s\n" % e)
+    self.send_response(500)
+    
+self.send_response(200)
+```
 ## Documentation for API Endpoints
 
 Swagger: https://app.swaggerhub.com/apis-docs/gitdevstar/Algocash/1.0.0
 
 BASE_URL: https://testapi2.algorithmic.cash/  for dev
 
 Class | Method | HTTP request | Description
```

### Comparing `algocash-sdk-1.2.0/algocash_sdk/__init__.py` & `algocash-sdk-1.3.0/algocash_sdk/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 from __future__ import absolute_import
 
 # import apis into sdk package
 from algocash_sdk.api.deposit_api import DepositApi
 from algocash_sdk.api.payout_api import PayoutApi
 # import ApiClient
 from algocash_sdk.api_client import ApiClient
+from algocash_sdk.callback import Callback
 from algocash_sdk.configuration import Configuration
 # import models into sdk package
 from algocash_sdk.models.address import Address
 from algocash_sdk.models.bank import Bank
 from algocash_sdk.models.callback_payload import CallbackPayload
 from algocash_sdk.models.deposit_request import DepositRequest
 from algocash_sdk.models.deposit_success import DepositSuccess
```

### Comparing `algocash-sdk-1.2.0/algocash_sdk/api/deposit_api.py` & `algocash-sdk-1.3.0/algocash_sdk/api/deposit_api.py`

 * *Files identical despite different names*

### Comparing `algocash-sdk-1.2.0/algocash_sdk/api/payout_api.py` & `algocash-sdk-1.3.0/algocash_sdk/api/payout_api.py`

 * *Files identical despite different names*

### Comparing `algocash-sdk-1.2.0/algocash_sdk/api_client.py` & `algocash-sdk-1.3.0/algocash_sdk/api_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -205,15 +205,15 @@
             obj_dict = {obj.attribute_map[attr]: getattr(obj, attr)
                         for attr, _ in six.iteritems(obj.attribute_types)
                         if getattr(obj, attr) is not None}
 
         return {key: self.sanitize_for_serialization(val)
                 for key, val in six.iteritems(obj_dict)}
 
-    def deserialize(self, response, response_type):
+    def deserialize(self, response, response_type, http = True):
         """Deserializes response into an object.
 
         :param response: RESTResponse object to be deserialized.
         :param response_type: class literal for
             deserialized object, or string of class name.
 
         :return: deserialized object.
@@ -221,15 +221,15 @@
         # handle file downloading
         # save response body into a tmp file and return the instance
         if response_type == "file":
             return self.__deserialize_file(response)
 
         # fetch data from response object
         try:
-            data = json.loads(response.data)
+            data = json.loads(response.data if http else response)
         except ValueError:
             # return response.data
             raise ValueError(
                 response.data
             )
 
         return self.__deserialize(data, response_type)
```

### Comparing `algocash-sdk-1.2.0/algocash_sdk/configuration.py` & `algocash-sdk-1.3.0/algocash_sdk/configuration.py`

 * *Files identical despite different names*

### Comparing `algocash-sdk-1.2.0/algocash_sdk/models/__init__.py` & `algocash-sdk-1.3.0/algocash_sdk/models/__init__.py`

 * *Files identical despite different names*

### Comparing `algocash-sdk-1.2.0/algocash_sdk/models/address.py` & `algocash-sdk-1.3.0/algocash_sdk/models/address.py`

 * *Files identical despite different names*

### Comparing `algocash-sdk-1.2.0/algocash_sdk/models/bank.py` & `algocash-sdk-1.3.0/algocash_sdk/models/bank.py`

 * *Files identical despite different names*

### Comparing `algocash-sdk-1.2.0/algocash_sdk/models/callback_payload.py` & `algocash-sdk-1.3.0/algocash_sdk/models/callback_payload.py`

 * *Files identical despite different names*

### Comparing `algocash-sdk-1.2.0/algocash_sdk/models/deposit_request.py` & `algocash-sdk-1.3.0/algocash_sdk/models/deposit_request.py`

 * *Files identical despite different names*

### Comparing `algocash-sdk-1.2.0/algocash_sdk/models/deposit_status_info.py` & `algocash-sdk-1.3.0/algocash_sdk/models/deposit_status_info.py`

 * *Files identical despite different names*

### Comparing `algocash-sdk-1.2.0/algocash_sdk/models/deposit_status_response.py` & `algocash-sdk-1.3.0/algocash_sdk/models/deposit_status_response.py`

 * *Files identical despite different names*

### Comparing `algocash-sdk-1.2.0/algocash_sdk/models/deposit_success.py` & `algocash-sdk-1.3.0/algocash_sdk/models/deposit_success.py`

 * *Files identical despite different names*

### Comparing `algocash-sdk-1.2.0/algocash_sdk/models/error.py` & `algocash-sdk-1.3.0/algocash_sdk/models/error.py`

 * *Files identical despite different names*

### Comparing `algocash-sdk-1.2.0/algocash_sdk/models/payer.py` & `algocash-sdk-1.3.0/algocash_sdk/models/payer.py`

 * *Files identical despite different names*

### Comparing `algocash-sdk-1.2.0/algocash_sdk/models/payout_request.py` & `algocash-sdk-1.3.0/algocash_sdk/models/payout_request.py`

 * *Files identical despite different names*

### Comparing `algocash-sdk-1.2.0/algocash_sdk/models/payout_status_info.py` & `algocash-sdk-1.3.0/algocash_sdk/models/payout_status_info.py`

 * *Files identical despite different names*

### Comparing `algocash-sdk-1.2.0/algocash_sdk/models/payout_status_response.py` & `algocash-sdk-1.3.0/algocash_sdk/models/payout_status_response.py`

 * *Files identical despite different names*

### Comparing `algocash-sdk-1.2.0/algocash_sdk/models/payout_success.py` & `algocash-sdk-1.3.0/algocash_sdk/models/payout_success.py`

 * *Files identical despite different names*

### Comparing `algocash-sdk-1.2.0/algocash_sdk/models/url.py` & `algocash-sdk-1.3.0/algocash_sdk/models/url.py`

 * *Files identical despite different names*

### Comparing `algocash-sdk-1.2.0/algocash_sdk/rest.py` & `algocash-sdk-1.3.0/algocash_sdk/rest.py`

 * *Files identical despite different names*

### Comparing `algocash-sdk-1.2.0/algocash_sdk.egg-info/SOURCES.txt` & `algocash-sdk-1.3.0/algocash_sdk.egg-info/SOURCES.txt`

 * *Files 27% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 README.md
 setup.py
 algocash_sdk/__init__.py
 algocash_sdk/api_client.py
+algocash_sdk/callback.py
 algocash_sdk/configuration.py
 algocash_sdk/rest.py
 algocash_sdk.egg-info/PKG-INFO
 algocash_sdk.egg-info/SOURCES.txt
 algocash_sdk.egg-info/dependency_links.txt
 algocash_sdk.egg-info/requires.txt
 algocash_sdk.egg-info/top_level.txt
@@ -24,22 +25,12 @@
 algocash_sdk/models/payer.py
 algocash_sdk/models/payout_request.py
 algocash_sdk/models/payout_status_info.py
 algocash_sdk/models/payout_status_response.py
 algocash_sdk/models/payout_success.py
 algocash_sdk/models/url.py
 test/__init__.py
-test/server.py
-test/test_address.py
-test/test_bank.py
-test/test_callback_payload.py
+test/test_callback.py
 test/test_deposit_api.py
-test/test_deposit_request.py
 test/test_deposit_status_api.py
-test/test_deposit_success.py
-test/test_error.py
-test/test_payer.py
 test/test_payout_api.py
-test/test_payout_request.py
-test/test_payout_status_api.py
-test/test_payout_success.py
-test/test_url.py
+test/test_payout_status_api.py
```

### Comparing `algocash-sdk-1.2.0/setup.py` & `algocash-sdk-1.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     OpenAPI spec version: 1.0.0
     Contact: loganph.work@gmail.com
 """
 
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "algocash-sdk"
-VERSION = "1.2.0"
+VERSION = "1.3.0"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

### Comparing `algocash-sdk-1.2.0/test/server.py` & `algocash-sdk-1.3.0/test/test_callback.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,15 @@
+from __future__ import absolute_import
+
 from http.server import BaseHTTPRequestHandler, HTTPServer
 import logging
 
+import algocash_sdk
+from algocash_sdk.callback import SignatureVerificationException
+
 hostName = "localhost"
 serverPort = 8080
 
 class MyServer(BaseHTTPRequestHandler):
     def do_GET(self):
         self.send_response(200)
         self.send_header("Content-type", "text/html")
@@ -12,14 +17,27 @@
         self.wfile.write(bytes("Hello", "utf-8"))
     def do_POST(self):
         content_length = int(self.headers['Content-Length']) # <--- Gets the size of data
         post_data = self.rfile.read(content_length) # <--- Gets the data itself
         logging.info("POST request,\nPath: %s\nHeaders:\n%s\n\nBody:\n%s\n",
                 str(self.path), str(self.headers), post_data.decode('utf-8'))
         
+        try:
+            print("Signature: %s\n" % self.headers['Signature'])
+            callback = algocash_sdk.Callback()
+            data = callback.construct_callback(post_data.decode('utf-8'), self.headers['Signature'], '4q4epHrbUHykQwnc')
+            logging.info(data)
+            print(data)
+        except SignatureVerificationException as e:
+            print("SignatureVerificationException when listening callback: %s\n" % e)
+            self.send_response(401)
+        except ValueError as e:
+            print("ValueError Exception when listening callback: %s\n" % e)
+            self.send_response(500)
+            
         self.send_response(200)
 
 if __name__ == "__main__":        
     webServer = HTTPServer((hostName, serverPort), MyServer)
     print("Server started http://%s:%s" % (hostName, serverPort))
 
     try:
```

### Comparing `algocash-sdk-1.2.0/test/test_deposit_api.py` & `algocash-sdk-1.3.0/test/test_deposit_api.py`

 * *Files 6% similar despite different names*

```diff
@@ -45,19 +45,20 @@
         configuration.api_access_token = '4q4epHrbUHykQwnc'
         configuration.devmode = True
 
         client = ApiClient(configuration)
 
         # create an instance of the API class
         api_instance = DepositApi(client)
-        invoice_id = '46560389502' # str | 
+        invoice_id = '47602' # str | 
         amount = '100' # str | 
         payer = algocash_sdk.Payer('test@gmail.com', '+918885916123') # Payer 
         payment_method = 'UPI' # str | 
-        url = algocash_sdk.Url('https://localhost:8080/callback', 'https://localhost:8080/pending', 'https://localhost:8080/success', 'https://localhost:8080/error') # Url | 
+        base = 'https://1836-204-188-232-195.ngrok-free.app'
+        url = algocash_sdk.Url(base, 'https://localhost:8080/pending', 'https://localhost:8080/success', 'https://localhost:8080/error') # Url | 
 
         try:
             # create a deposit
             api_response = api_instance.create_deposit(invoice_id, amount, payer, url, payment_method)
             pprint(api_response)
         except ValueError as e:
             print("ValueError Exception when calling DepositApi->create_deposit: %s\n" % e)
```

### Comparing `algocash-sdk-1.2.0/test/test_deposit_status_api.py` & `algocash-sdk-1.3.0/test/test_deposit_status_api.py`

 * *Files identical despite different names*

### Comparing `algocash-sdk-1.2.0/test/test_payout_api.py` & `algocash-sdk-1.3.0/test/test_payout_api.py`

 * *Files identical despite different names*

### Comparing `algocash-sdk-1.2.0/test/test_payout_status_api.py` & `algocash-sdk-1.3.0/test/test_payout_status_api.py`

 * *Files identical despite different names*

