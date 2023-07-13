# Comparing `tmp/epson_connect-0.2.1.tar.gz` & `tmp/epson_connect-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "epson_connect-0.2.1.tar", max compression
+gzip compressed data, was "epson_connect-0.2.2.tar", max compression
```

## Comparing `epson_connect-0.2.1.tar` & `epson_connect-0.2.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1119 2023-07-09 20:45:17.736792 epson_connect-0.2.1/LICENSE
--rw-r--r--   0        0        0      763 2023-07-12 19:25:52.875427 epson_connect-0.2.1/README.md
--rw-r--r--   0        0        0     1339 2023-07-12 19:24:10.856304 epson_connect-0.2.1/pyproject.toml
--rw-r--r--   0        0        0       41 2023-07-10 04:04:57.289077 epson_connect-0.2.1/src/epson_connect/__init__.py
--rw-r--r--   0        0        0     3984 2023-07-12 19:21:10.575014 epson_connect-0.2.1/src/epson_connect/authenticate.py
--rw-r--r--   0        0        0     1154 2023-07-09 05:46:28.548782 epson_connect-0.2.1/src/epson_connect/client.py
--rw-r--r--   0        0        0     4465 2023-07-12 19:19:38.422590 epson_connect-0.2.1/src/epson_connect/printer.py
--rw-r--r--   0        0        0     4924 2023-07-10 04:09:53.041881 epson_connect-0.2.1/src/epson_connect/printer_settings.py
--rw-r--r--   0        0        0     2450 2023-07-12 19:25:30.140848 epson_connect-0.2.1/src/epson_connect/scanner.py
--rw-r--r--   0        0        0     1836 1970-01-01 00:00:00.000000 epson_connect-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1119 2023-07-09 20:45:17.736792 epson_connect-0.2.2/LICENSE
+-rw-r--r--   0        0        0      763 2023-07-12 23:18:21.630580 epson_connect-0.2.2/README.md
+-rw-r--r--   0        0        0     1339 2023-07-13 00:42:37.047774 epson_connect-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0       41 2023-07-10 04:04:57.289077 epson_connect-0.2.2/src/epson_connect/__init__.py
+-rw-r--r--   0        0        0     3661 2023-07-13 00:22:52.026520 epson_connect-0.2.2/src/epson_connect/authenticate.py
+-rw-r--r--   0        0        0     1265 2023-07-12 23:49:14.792209 epson_connect-0.2.2/src/epson_connect/client.py
+-rw-r--r--   0        0        0     4460 2023-07-12 23:51:36.755455 epson_connect-0.2.2/src/epson_connect/printer.py
+-rw-r--r--   0        0        0     4924 2023-07-10 04:09:53.041881 epson_connect-0.2.2/src/epson_connect/printer_settings.py
+-rw-r--r--   0        0        0     2450 2023-07-12 19:25:30.140848 epson_connect-0.2.2/src/epson_connect/scanner.py
+-rw-r--r--   0        0        0     1836 1970-01-01 00:00:00.000000 epson_connect-0.2.2/PKG-INFO
```

### Comparing `epson_connect-0.2.1/LICENSE` & `epson_connect-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `epson_connect-0.2.1/README.md` & `epson_connect-0.2.2/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -11,25 +11,25 @@
 ```
 
 ## Usage
 
 ```python
 import epson_connect
 
-ec = espon_connect.Client(
+ec = epson_connect.Client(
     printer_email='...',
     client_id='...',
     client_secret='...',
 )
 
 # Or with these enviornment variables defined...
-# export ESPON_CONNECT_API_PRINTER_EMAIL=<an email address for the device>
-# export ESPON_CONNECT_API_CLIENT_ID=<client id>
-# export ESPON_CONNECT_API_CLIENT_SECRET=<client secret>
-# ec = espon_connect.Client()
+# export EPSON_CONNECT_API_PRINTER_EMAIL=<an email address for the device>
+# export EPSON_CONNECT_API_CLIENT_ID=<client id>
+# export EPSON_CONNECT_API_CLIENT_SECRET=<client secret>
+# ec = epson_connect.Client()
 
 # Print a PDF.
 job_id = ec.printer.print('./path/to/file.pdf')
 
 # List scan destinations.
 ec.scanner.list()
 ```
```

### Comparing `epson_connect-0.2.1/pyproject.toml` & `epson_connect-0.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "epson-connect"
-version = "0.2.1"
+version = "0.2.2"
 description = "Bindings for the Espon Connect API"
 license = "MIT"
 authors = ["Paul Logston <paul.logston@gmail.com>"]
 maintainers = ["Paul Logston <paul.logston@gmail.com>"]
 readme = "README.md"
 homepage = "https://pypi.org/project/epson-connect/"
 repository = "https://github.com/logston/epson-connect"
```

### Comparing `epson_connect-0.2.1/src/epson_connect/authenticate.py` & `epson_connect-0.2.2/src/epson_connect/authenticate.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import logging
-import os
 from datetime import datetime, timedelta
 
 import requests
 from requests.auth import HTTPBasicAuth
 
 logger = logging.getLogger(__name__)
 
@@ -65,15 +64,15 @@
         if self._access_token == '':
             self._refresh_token = body['refresh_token']
 
         self._expires_at = datetime.now() + timedelta(seconds=int(body['expires_in']))
         self._access_token = body['access_token']
         self._subject_id = body['subject_id']
 
-    def _deauthticate(self):
+    def _deauthenticate(self):
         """
         Cancel authentication.
         """
         method = 'DELETE'
         path = f'/api/1/printing/printers/{self._subject_id}'
         self.send(method, path)
 
@@ -129,17 +128,7 @@
     """
 
 
 class ApiError(RuntimeError):
     """
     General base error for any API errors after authentication has succeeded.
     """
-
-
-if __name__ == '__main__':
-    # For testing.
-    AuthCtx(
-        base_url='https://api.epsonconnect.com',
-        printer_email=os.environ['ESPON_CONNECT_API_PRINTER_EMAIL'],
-        client_id=os.environ['ESPON_CONNECT_API_CLIENT_ID'],
-        client_secret=os.environ['ESPON_CONNECT_API_CLIENT_SECRET'],
-    )
```

### Comparing `epson_connect-0.2.1/src/epson_connect/client.py` & `epson_connect-0.2.2/src/epson_connect/client.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,31 +7,37 @@
 
 class Client:
     EC_BASE_URL = 'https://api.epsonconnect.com'
 
     def __init__(self, base_url='', printer_email='', client_id='', client_secret='') -> None:
         base_url = base_url or self.EC_BASE_URL
 
-        printer_email = printer_email or os.environ.get('ESPON_CONNECT_API_PRINTER_EMAIL')
+        printer_email = printer_email or os.environ.get('EPSON_CONNECT_API_PRINTER_EMAIL')
         if not printer_email:
-            raise ValueError('Printer Email can not be empty')
+            raise ClientError('Printer Email can not be empty')
 
-        client_id = client_id or os.environ.get('ESPON_CONNECT_API_CLIENT_ID')
+        client_id = client_id or os.environ.get('EPSON_CONNECT_API_CLIENT_ID')
         if not client_id:
-            raise ValueError('Client ID can not be empty')
+            raise ClientError('Client ID can not be empty')
 
-        client_secret = client_secret or os.environ.get('ESPON_CONNECT_API_CLIENT_SECRET')
+        client_secret = client_secret or os.environ.get('EPSON_CONNECT_API_CLIENT_SECRET')
         if not client_secret:
-            raise ValueError('Client Secret can not be empty')
+            raise ClientError('Client Secret can not be empty')
 
         self._auth_ctx = AuthCtx(base_url, printer_email, client_id, client_secret)
 
-    def deauthticate(self):
-        self._auth_ctx._deauthticate()
+    def deauthenticate(self):
+        self._auth_ctx._deauthenticate()
 
     @property
     def printer(self):
         return Printer(self._auth_ctx)
 
     @property
     def scanner(self):
         return Scanner(self._auth_ctx)
+
+
+class ClientError(ValueError):
+    """
+    General base error for any client specific errors.
+    """
```

### Comparing `epson_connect-0.2.1/src/epson_connect/printer.py` & `epson_connect-0.2.2/src/epson_connect/printer.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,24 +39,26 @@
         Get device print capabilities.
         """
         method = 'GET'
         path = f'/api/1/printing/printers/{self.device_id}/capability/{mode}'
 
         return self._auth_ctx.send(method, path)
 
-    def _print_setting(self, settings) -> dict:
+    def print_setting(self, settings) -> dict:
         """
         Create a print job.
         """
         method = 'POST'
         path = f'/api/1/printing/printers/{self.device_id}/jobs'
 
+        validate_settings(settings)
+
         return self._auth_ctx.send(method, path, json=settings)
 
-    def _upload_file(self, upload_uri: str, file_path: str, print_mode: str) -> None:
+    def upload_file(self, upload_uri: str, file_path: str, print_mode: str) -> None:
         """
         Upload file to be printed.
         """
         # Get extension from file path.
         extension = pathlib.Path(file_path).suffix.lower()
         if extension[1:] not in self.VALID_EXTENSIONS:
             raise PrinterError(f'{extension} is not a valid printing extension.')
@@ -81,34 +83,33 @@
             'Content-Type': content_type,
             'Content-Length': str(len(data)),
         }
 
         method = 'POST'
         self._auth_ctx.send(method, path, data=data, headers=headers)
 
-    def _execute_print(self, job_id):
+    def execute_print(self, job_id):
         """
         Execute print job.
         """
         method = 'POST'
         path = f'/api/1/printing/printers/{self.device_id}/jobs/{job_id}/print'
         self._auth_ctx.send(method, path)
 
     def print(self, file_path, settings=None) -> str:
         """
         Print file.
 
         :return: Job ID for print job.
         """
         settings = merge_with_default_settings(settings)
-        validate_settings(settings)
 
-        job_data = self._print_setting(settings)
-        self._upload_file(job_data['upload_uri'], file_path, settings['print_mode'])
-        self._execute_print(job_data['id'])
+        job_data = self.print_setting(settings)
+        self.upload_file(job_data['upload_uri'], file_path, settings['print_mode'])
+        self.execute_print(job_data['id'])
         return job_data['id']
 
     def cancel_print(self, job_id, operated_by='user'):
         """
         Cancel print.
         """
         method = 'POST'
```

### Comparing `epson_connect-0.2.1/src/epson_connect/printer_settings.py` & `epson_connect-0.2.2/src/epson_connect/printer_settings.py`

 * *Files identical despite different names*

### Comparing `epson_connect-0.2.1/src/epson_connect/scanner.py` & `epson_connect-0.2.2/src/epson_connect/scanner.py`

 * *Files identical despite different names*

### Comparing `epson_connect-0.2.1/PKG-INFO` & `epson_connect-0.2.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: epson-connect
-Version: 0.2.1
+Version: 0.2.2
 Summary: Bindings for the Espon Connect API
 Home-page: https://pypi.org/project/epson-connect/
 License: MIT
 Keywords: epson,connect,api
 Author: Paul Logston
 Author-email: paul.logston@gmail.com
 Maintainer: Paul Logston
@@ -40,25 +40,25 @@
 ```
 
 ## Usage
 
 ```python
 import epson_connect
 
-ec = espon_connect.Client(
+ec = epson_connect.Client(
     printer_email='...',
     client_id='...',
     client_secret='...',
 )
 
 # Or with these enviornment variables defined...
-# export ESPON_CONNECT_API_PRINTER_EMAIL=<an email address for the device>
-# export ESPON_CONNECT_API_CLIENT_ID=<client id>
-# export ESPON_CONNECT_API_CLIENT_SECRET=<client secret>
-# ec = espon_connect.Client()
+# export EPSON_CONNECT_API_PRINTER_EMAIL=<an email address for the device>
+# export EPSON_CONNECT_API_CLIENT_ID=<client id>
+# export EPSON_CONNECT_API_CLIENT_SECRET=<client secret>
+# ec = epson_connect.Client()
 
 # Print a PDF.
 job_id = ec.printer.print('./path/to/file.pdf')
 
 # List scan destinations.
 ec.scanner.list()
 ```
```

