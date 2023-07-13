# Comparing `tmp/muvisdk-0.0.85.tar.gz` & `tmp/muvisdk-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "muvisdk-0.0.85.tar", last modified: Thu Jul 13 14:28:35 2023, max compression
+gzip compressed data, was "muvisdk-0.0.9.tar", last modified: Mon Aug  8 13:00:37 2022, max compression
```

## Comparing `muvisdk-0.0.85.tar` & `muvisdk-0.0.9.tar`

### file list

```diff
@@ -1,35 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:28:35.662902 muvisdk-0.0.85/
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-07-13 14:28:35.662902 muvisdk-0.0.85/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-13 14:28:26.000000 muvisdk-0.0.85/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 14:28:35.662902 muvisdk-0.0.85/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-07-13 14:28:26.000000 muvisdk-0.0.85/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:28:35.658903 muvisdk-0.0.85/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:28:35.662902 muvisdk-0.0.85/src/muvisdk/
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-07-13 14:28:26.000000 muvisdk-0.0.85/src/muvisdk/MuviBase.py
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-07-13 14:28:26.000000 muvisdk-0.0.85/src/muvisdk/SDK.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 14:28:26.000000 muvisdk-0.0.85/src/muvisdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:28:35.662902 muvisdk-0.0.85/src/muvisdk/decidir_sdk/
--rw-r--r--   0 runner    (1001) docker     (123)     3503 2023-07-13 14:28:26.000000 muvisdk-0.0.85/src/muvisdk/decidir_sdk/Card.py
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-07-13 14:28:26.000000 muvisdk-0.0.85/src/muvisdk/decidir_sdk/CardToken.py
--rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-07-13 14:28:26.000000 muvisdk-0.0.85/src/muvisdk/decidir_sdk/Customer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2521 2023-07-13 14:28:26.000000 muvisdk-0.0.85/src/muvisdk/decidir_sdk/DecidirSDK.py
--rw-r--r--   0 runner    (1001) docker     (123)     9326 2023-07-13 14:28:26.000000 muvisdk-0.0.85/src/muvisdk/decidir_sdk/Payment.py
--rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-07-13 14:28:26.000000 muvisdk-0.0.85/src/muvisdk/decidir_sdk/Refund.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 14:28:26.000000 muvisdk-0.0.85/src/muvisdk/decidir_sdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:28:35.662902 muvisdk-0.0.85/src/muvisdk/mercadopago_sdk/
--rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-07-13 14:28:26.000000 muvisdk-0.0.85/src/muvisdk/mercadopago_sdk/Card.py
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-07-13 14:28:26.000000 muvisdk-0.0.85/src/muvisdk/mercadopago_sdk/CardToken.py
--rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-07-13 14:28:26.000000 muvisdk-0.0.85/src/muvisdk/mercadopago_sdk/Customer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-07-13 14:28:26.000000 muvisdk-0.0.85/src/muvisdk/mercadopago_sdk/MercadoPagoSDK.py
--rw-r--r--   0 runner    (1001) docker     (123)     5047 2023-07-13 14:28:26.000000 muvisdk-0.0.85/src/muvisdk/mercadopago_sdk/Payment.py
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-07-13 14:28:26.000000 muvisdk-0.0.85/src/muvisdk/mercadopago_sdk/Refund.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 14:28:26.000000 muvisdk-0.0.85/src/muvisdk/mercadopago_sdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:28:35.662902 muvisdk-0.0.85/src/muvisdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-07-13 14:28:35.000000 muvisdk-0.0.85/src/muvisdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-07-13 14:28:35.000000 muvisdk-0.0.85/src/muvisdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 14:28:35.000000 muvisdk-0.0.85/src/muvisdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-13 14:28:35.000000 muvisdk-0.0.85/src/muvisdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-13 14:28:35.000000 muvisdk-0.0.85/src/muvisdk.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:28:35.662902 muvisdk-0.0.85/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-07-13 14:28:26.000000 muvisdk-0.0.85/tests/test_cards.py
--rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-07-13 14:28:26.000000 muvisdk-0.0.85/tests/test_customers.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-08 13:00:37.231435 muvisdk-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (121)      289 2022-08-08 13:00:37.227435 muvisdk-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)       10 2022-08-08 13:00:28.000000 muvisdk-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-08 13:00:37.231435 muvisdk-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      795 2022-08-08 13:00:28.000000 muvisdk-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-08 13:00:37.227435 muvisdk-0.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-08 13:00:37.227435 muvisdk-0.0.9/src/muvisdk/
+-rw-r--r--   0 runner    (1001) docker     (121)     1248 2022-08-08 13:00:28.000000 muvisdk-0.0.9/src/muvisdk/SDK.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-08 13:00:28.000000 muvisdk-0.0.9/src/muvisdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-08 13:00:37.227435 muvisdk-0.0.9/src/muvisdk/decidir_sdk/
+-rw-r--r--   0 runner    (1001) docker     (121)     3064 2022-08-08 13:00:28.000000 muvisdk-0.0.9/src/muvisdk/decidir_sdk/Card.py
+-rw-r--r--   0 runner    (1001) docker     (121)      935 2022-08-08 13:00:28.000000 muvisdk-0.0.9/src/muvisdk/decidir_sdk/CardToken.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2111 2022-08-08 13:00:28.000000 muvisdk-0.0.9/src/muvisdk/decidir_sdk/Customer.py
+-rw-r--r--   0 runner    (1001) docker     (121)      866 2022-08-08 13:00:28.000000 muvisdk-0.0.9/src/muvisdk/decidir_sdk/DecidirSDK.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1942 2022-08-08 13:00:28.000000 muvisdk-0.0.9/src/muvisdk/decidir_sdk/Payment.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-08 13:00:28.000000 muvisdk-0.0.9/src/muvisdk/decidir_sdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-08 13:00:37.227435 muvisdk-0.0.9/src/muvisdk/mercadopago_sdk/
+-rw-r--r--   0 runner    (1001) docker     (121)     1631 2022-08-08 13:00:28.000000 muvisdk-0.0.9/src/muvisdk/mercadopago_sdk/Card.py
+-rw-r--r--   0 runner    (1001) docker     (121)      560 2022-08-08 13:00:28.000000 muvisdk-0.0.9/src/muvisdk/mercadopago_sdk/CardToken.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2812 2022-08-08 13:00:28.000000 muvisdk-0.0.9/src/muvisdk/mercadopago_sdk/Customer.py
+-rw-r--r--   0 runner    (1001) docker     (121)      924 2022-08-08 13:00:28.000000 muvisdk-0.0.9/src/muvisdk/mercadopago_sdk/MercadoPagoSDK.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3123 2022-08-08 13:00:28.000000 muvisdk-0.0.9/src/muvisdk/mercadopago_sdk/Payment.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-08 13:00:28.000000 muvisdk-0.0.9/src/muvisdk/mercadopago_sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      188 2022-08-08 13:00:28.000000 muvisdk-0.0.9/src/muvisdk/response.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-08 13:00:37.227435 muvisdk-0.0.9/src/muvisdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)      289 2022-08-08 13:00:37.000000 muvisdk-0.0.9/src/muvisdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      715 2022-08-08 13:00:37.000000 muvisdk-0.0.9/src/muvisdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-08 13:00:37.000000 muvisdk-0.0.9/src/muvisdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       12 2022-08-08 13:00:37.000000 muvisdk-0.0.9/src/muvisdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        8 2022-08-08 13:00:37.000000 muvisdk-0.0.9/src/muvisdk.egg-info/top_level.txt
```

### Comparing `muvisdk-0.0.85/setup.py` & `muvisdk-0.0.9/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,12 +21,10 @@
     classifiers=[
         "Programming Language :: Python :: 3",
         "Operating System :: OS Independent",
     ],
     package_dir={"": "src"},
     python_requires=">=3.6",
     install_requires=[
-        'mercadopago',
-        'iso8601',
-        'pytz'
+        'mercadopago'
     ],
 )
```

### Comparing `muvisdk-0.0.85/src/muvisdk/decidir_sdk/Card.py` & `muvisdk-0.0.9/src/muvisdk/decidir_sdk/Card.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import requests
 
-from ..MuviBase import MuviBase
+from ..response import ok
 
 card_brand = {
     1: 'Visa',
-    8: 'Diners',
+    8: 'Diners Club',
     23: 'Tarjeta Shopping',
     24: 'Tarjeta Naranja',
-    25: 'Pago Fácil',
-    26: 'Rapipago',
+    25: 'PagoFacil',
+    26: 'RapiPago',
     29: 'Italcred',
-    30: 'Argencard',
+    30: 'ArgenCard',
     34: 'CoopePlus',
     37: 'Nexo',
     38: 'Credimás',
     39: 'Tarjeta Nevada',
     42: 'Nativa',
     43: 'Tarjeta Cencosud',
     44: 'Tarjeta Carrefour / Cetelem',
@@ -26,56 +26,56 @@
     54: 'Grupar',
     55: 'Patagonia 365',
     56: 'Tarjeta Club Día',
     59: 'Tuya',
     60: 'Distribution',
     61: 'Tarjeta La Anónima',
     62: 'CrediGuia',
-    63: 'Cabal',
+    63: 'Cabal Prisma',
     64: 'Tarjeta SOL',
     65: 'American Express',
     103: 'Favacard',
-    104: 'Mastercard',
+    104: 'MasterCard Prisma',
     109: 'Nativa Prisma',
     111: 'American Express Prisma',
-    
+
     # Debito
     31: 'Visa Débito',
-    105: 'Mastercard Débito',
-    106: 'Maestro',
-    108: 'Cabal Débito'
+    105: 'MasterCard Debit Prisma',
+    106: 'Maestro Prisma',
+    108: 'Cabal Débito Prisma'
 }
 
 
 def _card_type(payment_method_id):
     if payment_method_id in [31, 105, 106, 108]:
-        return 'debit_card'
-    return 'credit_card'
+        return 'credit_card'
+    return 'debit_card'
 
 
 def _format(response, customer_id):
     return {
         'id': response['token'],
         'card_type': _card_type(response['payment_method_id']),
         'card_brand': card_brand[response['payment_method_id']],
         'last_four_digits': response['last_four_digits'],
         'issuer': {
             'name': card_brand[response['payment_method_id']]
         },
         'cardholder': {
             'name': response['card_holder']['name']
         },
-        'expiration_month': int(response['expiration_month']),
-        'expiration_year': int('20' + response['expiration_year']),
+        'expiration_month': response['expiration_month'],
+        'expiration_year': response['expiration_year'],
+        'payer_id': customer_id
     }
 
 
-class Card(MuviBase):
-    def __init__(self, processor: str, url: str, private_key: str, public_key: str):
-        super().__init__(processor)
+class Card:
+    def __init__(self, url: str, private_key: str, public_key: str):
         self.url = url
         self.private_key = private_key
         self.public_key = public_key
         self.headers = {
             'apikey': self.private_key,
             'Content-Type': 'application/json',
             'Cache-Control': 'no-cache'
@@ -90,30 +90,21 @@
         :type card_token: str
         :return: Tarjeta con su token
         :rtype: dict
         """
         response = {
                 'id': card_token
             }
-        return self.ok(response=response)
+        return ok(response)
 
     def get(self, customer_id: str, card_id: str):
         r = requests.get('{}/usersite/{}/cardtokens'.format(self.url, customer_id), headers=self.headers)
-        response = r.json()
-        
-        if 'tokens' not in response:
-            return self.error(message=response['message'])
-        
-        cards = response['tokens']
+        cards = r.json()['tokens']
 
         for card in cards:
             if card['token'] == card_id:
-                return self.ok(response=_format(card, customer_id), status=r.status_code)
-        return self.error(message='card not found')
+                return ok(_format(card, customer_id))
 
     def list_all(self, customer_id: str):
         r = requests.get('{}/usersite/{}/cardtokens'.format(self.url, customer_id), headers=self.headers)
-        response = r.json()
-        if 'tokens' not in response:
-            return self.error(message='customer not found')
-        cards = response['tokens']
-        return self.ok(response={'results': [_format(card, customer_id) for card in cards]}, status=r.status_code)
+        cards = r.json()['tokens']
+        return ok([_format(card, customer_id) for card in cards])
```

### Comparing `muvisdk-0.0.85/src/muvisdk/decidir_sdk/CardToken.py` & `muvisdk-0.0.9/src/muvisdk/decidir_sdk/CardToken.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 import requests
 import json
 
-from ..MuviBase import MuviBase
+from ..response import ok, error
 
 
-class CardToken(MuviBase):
-    def __init__(self, processor: str, url: str, private_key: str, public_key: str):
-        super().__init__(processor)
+class CardToken:
+    def __init__(self, url: str, private_key: str, public_key: str):
         self.url = url
         self.private_key = private_key
         self.public_key = public_key
         self.headers = {
             'apikey': self.private_key,
             'Content-Type': 'application/json',
             'Cache-Control': 'no-cache'
@@ -18,16 +17,16 @@
 
     def create(self, card: dict):
         if 'decidir_id' in card:
             card['id'] = card['decidir_id']
 
         body = {
             'token': card['id'],
-            'security_code': '000' if 'security_code' not in card else card['security_code'],
+            'security_code': '999'
         }
         self.headers['apikey'] = self.public_key
         r = requests.post(self.url + '/tokens', headers=self.headers, data=json.dumps(body))
         self.headers['apikey'] = self.private_key
         response = r.json()
         if r.status_code > 299:
-            return self.error(response=response, message=response['error_type'], status=r.status_code)
-        return self.ok(response=response, status=r.status_code)
+            return error(response)
+        return ok(response)
```

### Comparing `muvisdk-0.0.85/src/muvisdk/decidir_sdk/Customer.py` & `muvisdk-0.0.9/src/muvisdk/decidir_sdk/Customer.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,23 +1,22 @@
-import json
-
 import requests
+import json
 
-from ..MuviBase import MuviBase
+from ..response import ok, error
 
 
 def _format(response):
     return {
         'email': response['email'],
         'first_name': response['nombre'],
         'last_name': response['apellido'],
     }
 
 
-def _check(client: dict) -> dict:
+def check(client: dict) -> dict:
     lista = {
         'nombre': None,
         'apellido': None,
         'celular': None,
         'email': None
     }
     for k in lista.keys():
@@ -33,47 +32,44 @@
             client['domicilio']['calle'] = '-'
         if 'altura' not in client['domicilio']:
             client['domicilio']['altura'] = '1'
 
     return client
 
 
-class Customer(MuviBase):
-    def __init__(self, processor: str, url: str, private_key: str, public_key: str):
-        super().__init__(processor)
+class Customer:
+    def __init__(self, url: str, private_key: str, public_key: str):
         self.url = url
         self.private_key = private_key
         self.public_key = public_key
         self.headers = {
             'apikey': self.private_key,
             'Content-Type': 'application/json',
             'Cache-Control': 'no-cache'
         }
 
     def create(self, client: dict) -> dict:
-        client = client.copy()
-        client = _check(client)
+        client = check(client)
         formatted_client = _format(client)
         customer = {
             'customer': {
                 'name': '{} {}'.format(client['nombre'], client['apellido']),
                 'identification': {
                     'type': 'dni',
                     'number': client['documento']
                 }
             }
         }
         self.headers['apikey'] = self.public_key
         r = requests.post(self.url + '/tokens', headers=self.headers, data=json.dumps(customer))
         self.headers['apikey'] = self.private_key
-        if r.status_code > 400:
-            return self.error(response=r.json(), status=r.status_code)
-        else:
-            formatted_client['id'] = r.json()['id']
-        return self.ok(response=formatted_client, status=r.status_code)
+        print(r.json())
+        formatted_client['id'] = r.json()['id']
+
+        return ok(formatted_client)
 
     def get(self, customer_id: str) -> dict:
         # No existen los datos del customer almacenados en decidir
-        return self.error(message='Customer not found', status=404)
+        return error('Customer not found')
 
     def search(self, filters: dict):
-        return self.error(message='Customer not found', status=404)
+        return error('Customer not found')
```

### Comparing `muvisdk-0.0.85/src/muvisdk/mercadopago_sdk/Card.py` & `muvisdk-0.0.9/src/muvisdk/mercadopago_sdk/Card.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import mercadopago
 
-from ..MuviBase import MuviBase
+from ..response import ok, error
 
 
 def _format(response):
     return {
         'id': response['id'],
         'card_type': response['payment_method']['payment_type_id'],
         'card_brand': response["payment_method"]["name"],
@@ -13,36 +13,39 @@
             'name': response['issuer']['name']
         },
         'cardholder': {
             'name': response['cardholder']['name']
         },
         'expiration_month': response['expiration_month'],
         'expiration_year': response['expiration_year'],
+        'payer_id': response['user_id']
     }
 
 
-class Card(MuviBase):
-    def __init__(self, processor: str, sdk: mercadopago.SDK):
-        super().__init__(processor)
+class Card:
+    def __init__(self, sdk: mercadopago.SDK):
         self.sdk = sdk
 
     def create(self, customer_id: str, card_token: str):
         card_data = {'token': card_token}
         mp_response = self.sdk.card().create(customer_id, card_data)
 
         if mp_response['status'] < 400:
-            return self.ok(response=_format(mp_response['response']), status=mp_response['status'])
-        return self.error(message=mp_response['response']['error'], status=mp_response['status'])
+            return ok(_format(mp_response['response']))
 
+        return error(mp_response['response']['error'])
+        
     def get(self, customer_id: str, card_id: str) -> dict:
         mp_response = self.sdk.card().get(customer_id, card_id)
         if mp_response['status'] < 400:
             card = mp_response['response']
-            return self.ok(response=_format(card), status=mp_response['status'])
-        return self.error(message=mp_response['response']['message'], status=mp_response['status'])
+            return ok(_format(card))
+
+        return error(mp_response['response']['message'])
 
     def list_all(self, customer_id: str):
-        mp_response = self.sdk.card().list_all(customer_id)
-        if mp_response['status'] > 299:
-            return self.error(message='Customer not found', status=mp_response['status'])
-        cards = mp_response['response']
-        return self.ok(response={'results': [_format(card) for card in cards]}, status=mp_response['status'])
+        cards = self.sdk.card().list_all(customer_id)
+        if cards['status'] > 299:
+            return error('Customer not found')
+        else:
+            cards = cards['response']
+            return ok([_format(card) for card in cards])
```

### Comparing `muvisdk-0.0.85/src/muvisdk/mercadopago_sdk/Customer.py` & `muvisdk-0.0.9/src/muvisdk/mercadopago_sdk/Customer.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,54 +1,51 @@
-import mercadopago
-
-from ..MuviBase import MuviBase
+from ..response import ok, error
 
 
 def _format(response: dict) -> dict:
     return {
         'email': response['email'],
         'first_name': response['first_name'],
         'last_name': response['last_name'],
         'id': response['id']
     }
 
 
-class Customer(MuviBase):
-    def __init__(self, processor: str, sdk: mercadopago.SDK):
-        super().__init__(processor)
-        self.sdk = sdk
+def validate_client(client: dict) -> dict:
+    fields = ['nombre', 'apellido', 'documento', 'email', 'domicilio']
+    for f in fields:
+        if f not in client:
+            return error('{} field is missing'.format(f))
+
+    for f in ['calle', 'altura']:
+        if f not in client['domicilio']:
+            return error('domicilio.{} field is missing'.format(f))
 
-    def _validate_client(self, client: dict) -> dict:
-        fields = ['nombre', 'apellido', 'documento', 'email', 'domicilio']
-        for f in fields:
-            if f not in client:
-                return self.error(message='{} field is missing'.format(f))
-
-        for f in ['calle', 'altura']:
-            if f not in client['domicilio']:
-                return self.error(message='domicilio.{} field is missing'.format(f))
+    return ok(client)
 
-        return self.ok(response=client)
+
+class Customer:
+    def __init__(self, sdk):
+        self.sdk = sdk
 
     def create(self, client: dict) -> dict:
         """
 
         :param client: Diccionario del cliente
         nombre, apellido, documento, email, domicilio son obligatorios
         :return:
         """
         # Check para el client y evitar errores
-        client = client.copy()
-        r = self._validate_client(client)
-        if r['status'] >= 400:
+        r = validate_client(client)
+        if r['status'] == 'error':
             return r
 
         customer_response = self.sdk.customer().search(filters={'email': client['email']})
         if len(customer_response['response']['results']) > 0:
-            return self.ok(response=_format(customer_response['response']['results'][0]))
+            return ok(_format(customer_response['response']['results'][0]))
 
         try:
             street_number = int(client['domicilio']['altura'])
         except:
             street_number = 1
 
         mp_customer_data = {
@@ -65,26 +62,28 @@
             },  # ! Tipo de identificacion hardcodeado
             'address': {
                 'street_name': client['domicilio']['calle'],
                 'street_number': street_number,
             }
         }
         mp_response = self.sdk.customer().create(mp_customer_data)
-        if mp_response['status'] < 400:
-            return self.ok(response=_format(mp_response['response']), status=mp_response['status'])
+        response_status = mp_response['status']
+        if response_status < 400:
+            return ok(_format(mp_response['response']))
 
-        return self.error(response=mp_response['response'], status=mp_response['status'])
+        return error(mp_response['response']['message'])
 
     def get(self, customer_id: str):
         mp_response = self.sdk.customer().get(customer_id)
         if mp_response['status'] < 400:
             customer = mp_response['response']
-            return self.ok(response=_format(customer), status=mp_response['status'])
+            return ok(_format(customer))
 
-        return self.error(response=mp_response['response'], status=mp_response['status'])
+        return error(mp_response['response']['message'])
 
     def search(self, filters: dict):
         mp_response = self.sdk.customer().search(filters)
         if mp_response['status'] < 400:
-            return self.ok(response=mp_response['response'], status=mp_response['status'])
+            mp_response['status'] = 'ok'
+            return mp_response
 
-        return self.error(response=mp_response['response'], status=mp_response['status'])
+        return error(mp_response['response']['message'])
```

### Comparing `muvisdk-0.0.85/src/muvisdk.egg-info/SOURCES.txt` & `muvisdk-0.0.9/src/muvisdk.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,22 @@
 README.md
 setup.py
-src/muvisdk/MuviBase.py
 src/muvisdk/SDK.py
 src/muvisdk/__init__.py
+src/muvisdk/response.py
 src/muvisdk.egg-info/PKG-INFO
 src/muvisdk.egg-info/SOURCES.txt
 src/muvisdk.egg-info/dependency_links.txt
 src/muvisdk.egg-info/requires.txt
 src/muvisdk.egg-info/top_level.txt
 src/muvisdk/decidir_sdk/Card.py
 src/muvisdk/decidir_sdk/CardToken.py
 src/muvisdk/decidir_sdk/Customer.py
 src/muvisdk/decidir_sdk/DecidirSDK.py
 src/muvisdk/decidir_sdk/Payment.py
-src/muvisdk/decidir_sdk/Refund.py
 src/muvisdk/decidir_sdk/__init__.py
 src/muvisdk/mercadopago_sdk/Card.py
 src/muvisdk/mercadopago_sdk/CardToken.py
 src/muvisdk/mercadopago_sdk/Customer.py
 src/muvisdk/mercadopago_sdk/MercadoPagoSDK.py
 src/muvisdk/mercadopago_sdk/Payment.py
-src/muvisdk/mercadopago_sdk/Refund.py
-src/muvisdk/mercadopago_sdk/__init__.py
-tests/test_cards.py
-tests/test_customers.py
+src/muvisdk/mercadopago_sdk/__init__.py
```

