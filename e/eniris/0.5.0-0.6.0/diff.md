# Comparing `tmp/eniris-0.5.0.tar.gz` & `tmp/eniris-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eniris-0.5.0.tar", last modified: Mon May  8 08:36:20 2023, max compression
+gzip compressed data, was "eniris-0.6.0.tar", last modified: Thu Jul 13 16:18:34 2023, max compression
```

## Comparing `eniris-0.5.0.tar` & `eniris-0.6.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 08:36:20.823093 eniris-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-08 08:36:04.000000 eniris-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-05-08 08:36:20.823093 eniris-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-05-08 08:36:04.000000 eniris-0.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 08:36:20.823093 eniris-0.5.0/eniris/
--rw-r--r--   0 runner    (1001) docker     (123)     8916 2023-05-08 08:36:04.000000 eniris-0.5.0/eniris/ApiDriver.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 08:36:04.000000 eniris-0.5.0/eniris/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 08:36:20.823093 eniris-0.5.0/eniris.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-05-08 08:36:20.000000 eniris-0.5.0/eniris.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-05-08 08:36:20.000000 eniris-0.5.0/eniris.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 08:36:20.000000 eniris-0.5.0/eniris.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-08 08:36:20.000000 eniris-0.5.0/eniris.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-08 08:36:20.000000 eniris-0.5.0/eniris.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 08:36:20.823093 eniris-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-08 08:36:04.000000 eniris-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:18:34.665442 eniris-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-07-13 16:18:24.000000 eniris-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-07-13 16:18:34.665442 eniris-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-07-13 16:18:24.000000 eniris-0.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:18:34.665442 eniris-0.6.0/eniris/
+-rw-r--r--   0 runner    (1001) docker     (123)     8819 2023-07-13 16:18:24.000000 eniris-0.6.0/eniris/ApiDriver.py
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-13 16:18:24.000000 eniris-0.6.0/eniris/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:18:34.665442 eniris-0.6.0/eniris.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-07-13 16:18:34.000000 eniris-0.6.0/eniris.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-07-13 16:18:34.000000 eniris-0.6.0/eniris.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 16:18:34.000000 eniris-0.6.0/eniris.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-13 16:18:34.000000 eniris-0.6.0/eniris.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-13 16:18:34.000000 eniris-0.6.0/eniris.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 16:18:34.665442 eniris-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-07-13 16:18:24.000000 eniris-0.6.0/setup.py
```

### Comparing `eniris-0.5.0/LICENSE` & `eniris-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `eniris-0.5.0/PKG-INFO` & `eniris-0.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: eniris
-Version: 0.5.0
+Version: 0.6.0
 Summary: Eniris API driver for Python
 Home-page: https://github.com/eniris-international/eniris-api-python-driver
-Download-URL: https://github.com/eniris-international/eniris-api-python-driver/archive/refs/tags/v0.5.0.tar.gz
+Download-URL: https://github.com/eniris-international/eniris-api-python-driver/archive/refs/tags/v0.6.0.tar.gz
 Author: Enris BV
 Author-email: info@eniris.be
 License: MIT
 Keywords: eniris,api,rest
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
@@ -43,14 +43,15 @@
 - timeoutS (int, optional, default: 60): Request timeout in seconds
 - maximumRetries (int, optional, default: 5): How many times to try again in case of a failure due to connection or unavailability problems
 - initialRetryDelayS (int, optional, default: 1): The initial delay between successive retries in seconds.
 - maximumRetryDelayS (int, optional, default: 60): The maximum delay between successive retries in seconds.
 - session (requests.Session, optional, default: requests.Session()): A session object to use for all API calls.
 
 Furthermore, the following methods are exposed:
+- accesstoken: Get a currently valid accesstoken
 - get/delete: Send a HTTP GET/DELETE request. The following parameters are allowed:
   - path (string, required): Either a path relative to the apiUrl, or a full URL path
   - params (dict, optional, default: None): URL query parameters
 - post/put: Send a HTTP POST or PUT request. The following parameters are allowed:
   - path (string, required): Either a path relative to the apiUrl, or a full URL path
   - json (dict, optional, default: None): JSON body of the request. The json argument and the data argument cannot both be different from None
   - params (dict, optional, default: None): URL query parameters
```

### Comparing `eniris-0.5.0/README.md` & `eniris-0.6.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 - timeoutS (int, optional, default: 60): Request timeout in seconds
 - maximumRetries (int, optional, default: 5): How many times to try again in case of a failure due to connection or unavailability problems
 - initialRetryDelayS (int, optional, default: 1): The initial delay between successive retries in seconds.
 - maximumRetryDelayS (int, optional, default: 60): The maximum delay between successive retries in seconds.
 - session (requests.Session, optional, default: requests.Session()): A session object to use for all API calls.
 
 Furthermore, the following methods are exposed:
+- accesstoken: Get a currently valid accesstoken
 - get/delete: Send a HTTP GET/DELETE request. The following parameters are allowed:
   - path (string, required): Either a path relative to the apiUrl, or a full URL path
   - params (dict, optional, default: None): URL query parameters
 - post/put: Send a HTTP POST or PUT request. The following parameters are allowed:
   - path (string, required): Either a path relative to the apiUrl, or a full URL path
   - json (dict, optional, default: None): JSON body of the request. The json argument and the data argument cannot both be different from None
   - params (dict, optional, default: None): URL query parameters
```

### Comparing `eniris-0.5.0/eniris/ApiDriver.py` & `eniris-0.6.0/eniris/ApiDriver.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Union, Callable
+from typing import Callable
 import datetime
 import requests
 import logging
 import time
 from http import HTTPStatus
 
 class AuthenticationFailure(Exception):
@@ -53,49 +53,50 @@
     self.maximumRetries = maximumRetries
     self.initialRetryDelayS = initialRetryDelayS
     self.maximumRetryDelayS = maximumRetryDelayS
     self.refreshDtAndToken = None
     self.accessDtAndToken = None
     self.session = requests.Session() if session is None else session
     
-  def _authenticate(self):
+  def accesstoken(self):
     dt = datetime.datetime.now()
     if self.refreshDtAndToken is None or (dt - self.refreshDtAndToken[0]).total_seconds() > 13*24*60*60: # 13 days
       data = { "username": self.username, "password": self.password }
-      resp = self.session.post(self.authUrl + '/auth/login', json = data, timeout=self.timeoutS)
+      resp = self.session.post(f'{self.authUrl}/auth/login', json = data, timeout=self.timeoutS)
       if resp.status_code != 200:
-        raise AuthenticationFailure("login failed: " + resp.text)
+        raise AuthenticationFailure(f"login failed: {resp.text}")
       self.refreshDtAndToken = (dt, resp.text)
     elif (dt - self.refreshDtAndToken[0]).total_seconds() > 7*24*60*60: # 7 days
-      resp = self.session.get(self.authUrl + '/auth/refreshtoken', headers = {'Authorization': 'Bearer ' + self.refreshDtAndToken[1]}, timeout=self.timeoutS)
+      resp = self.session.get(f"{self.authUrl}/auth/refreshtoken", headers = {'Authorization': f"Bearer {self.refreshDtAndToken[1]}"}, timeout=self.timeoutS)
       if resp.status_code == 200:
         self.refreshDtAndToken = (dt, resp.text)
       else:
         # Not the biggest problem, sice the refresh token will still be valid for a while, but we should log an exception
-        logging.warning("Unable to renew the refresh token: " + resp.text)
+        logging.warning(f"Unable to renew the refresh token: {resp.text}")
     if self.accessDtAndToken is None or (dt - self.accessDtAndToken[0]).total_seconds() > 2*60: # 2 minutes
-      resp = self.session.get(self.authUrl + '/auth/accesstoken', headers = {'Authorization': 'Bearer ' + self.refreshDtAndToken[1]}, timeout=self.timeoutS)
+      resp = self.session.get(f"{self.authUrl}/auth/accesstoken", headers = {'Authorization': f"Bearer {self.refreshDtAndToken[1]}"}, timeout=self.timeoutS)
       if resp.status_code != 200:
-        raise AuthenticationFailure("accesstoken failed: " + resp.text)
+        raise AuthenticationFailure(f"accesstoken failed: {resp.text}")
       self.accessDtAndToken = (dt, resp.text)
+    return self.accessDtAndToken[1]
       
   def close(self):
     """Log out from the API
     """
     dt = datetime.datetime.now()
     if self.refreshDtAndToken is None or (dt - self.refreshDtAndToken[0]).total_seconds() > 14*24*60*60: # 14 days
       # The refresh token did already expire, there is no reason to log out
       return
-    resp = self.session.post(self.authUrl + '/auth/logout', headers = {'Authorization': 'Bearer ' + self.refreshDtAndToken[1]}, timeout=self.timeoutS)
+    resp = self.session.post(f"{self.authUrl}/auth/logout", headers = {'Authorization': f"Bearer {self.refreshDtAndToken[1]}"}, timeout=self.timeoutS)
     if resp.status_code == 204 or resp.status_code == 401:
       # The refresh token was either succesfully added to the deny list, or it was already invalid
       self.refreshDtAndToken = None
       self.accessDtAndToken = None 
     else:
-      raise AuthenticationFailure("logout failed: " + resp.text)
+      raise AuthenticationFailure(f"logout failed: {resp.text}")
   
   def __retry(self, requests_function:Callable, path:str, retryNr = 0, **req_function_kwargs) -> requests.Response:
     """Execute the given requests_function with the provided req_function_kwargs keyword arguments. If the function fails, it will try again until the amount of retries has exceeded.
 
     Args:
         requests_function (Callable): Requests function to use. Can be self.session.get, self.session.post, self.session.put or self.session.delete
         path (str): Path relative to the apiUrl.
@@ -129,50 +130,46 @@
     Args:
         path (str): Path relative to the apiUrl.
         params (dict, optional): URL parameters. Defaults to None.
 
     Returns:
         requests.Response: API call response
     """
-    self._authenticate()
-    return self.__retry(self.session.get, path, params = params, headers = {'Authorization': 'Bearer ' + self.accessDtAndToken[1]}, timeout=self.timeoutS)
+    return self.__retry(self.session.get, path, params = params, headers = {'Authorization': f'Bearer {self.accesstoken()}'}, timeout=self.timeoutS)
 
   def post(self, path:str, json = None, params = None, data = None, **kwargs) -> requests.Response:
     """API POST call()
 
     Args:
         path (str): Path relative to the apiUrl.
         json (dict, optional): JSON body. Defaults to None.
         params (dict, optional): URL parameters. Defaults to None.
 
     Returns:
         requests.Response: API call response
     """
-    self._authenticate()
-    return self.__retry(self.session.post, path, json = json, params = params, data = data, headers = {'Authorization': 'Bearer ' + self.accessDtAndToken[1]}, timeout=self.timeoutS)
+    return self.__retry(self.session.post, path, json = json, params = params, data = data, headers = {'Authorization': f'Bearer {self.accesstoken()}'}, timeout=self.timeoutS)
     
   def put(self, path:str, json = None, params = None, data = None, **kwargs) -> requests.Response:
     """API PUT call
 
     Args:
         path (str): Path relative to the apiUrl.
         json (dict, optional): JSON body. Defaults to None.
         params (dict, optional): URL parameters. Defaults to None.
 
     Returns:
         requests.Response: API call response
     """
-    self._authenticate()
-    return self.__retry(self.session.put, path, json = json, params = params, data = data, headers = {'Authorization': 'Bearer ' + self.accessDtAndToken[1]}, timeout=self.timeoutS)
+    return self.__retry(self.session.put, path, json = json, params = params, data = data, headers = {'Authorization': f'Bearer {self.accesstoken()}'}, timeout=self.timeoutS)
   
   def delete(self, path:str, params = None, **kwargs) -> requests.Response:
     """API DELETE call
 
     Args:
         path (str): Path relative to the baseUrl.
         params (dict, optional): URL parameters. Defaults to None.
 
     Returns:
         requests.Response: API call response
     """
-    self._authenticate()
-    return self.__retry(self.session.delete, path, params = params, headers = {'Authorization': 'Bearer ' + self.accessDtAndToken[1]}, timeout=self.timeoutS)
+    return self.__retry(self.session.delete, path, params = params, headers = {'Authorization': f'Bearer {self.accesstoken()}'}, timeout=self.timeoutS)
```

### Comparing `eniris-0.5.0/eniris.egg-info/PKG-INFO` & `eniris-0.6.0/eniris.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: eniris
-Version: 0.5.0
+Version: 0.6.0
 Summary: Eniris API driver for Python
 Home-page: https://github.com/eniris-international/eniris-api-python-driver
-Download-URL: https://github.com/eniris-international/eniris-api-python-driver/archive/refs/tags/v0.5.0.tar.gz
+Download-URL: https://github.com/eniris-international/eniris-api-python-driver/archive/refs/tags/v0.6.0.tar.gz
 Author: Enris BV
 Author-email: info@eniris.be
 License: MIT
 Keywords: eniris,api,rest
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
@@ -43,14 +43,15 @@
 - timeoutS (int, optional, default: 60): Request timeout in seconds
 - maximumRetries (int, optional, default: 5): How many times to try again in case of a failure due to connection or unavailability problems
 - initialRetryDelayS (int, optional, default: 1): The initial delay between successive retries in seconds.
 - maximumRetryDelayS (int, optional, default: 60): The maximum delay between successive retries in seconds.
 - session (requests.Session, optional, default: requests.Session()): A session object to use for all API calls.
 
 Furthermore, the following methods are exposed:
+- accesstoken: Get a currently valid accesstoken
 - get/delete: Send a HTTP GET/DELETE request. The following parameters are allowed:
   - path (string, required): Either a path relative to the apiUrl, or a full URL path
   - params (dict, optional, default: None): URL query parameters
 - post/put: Send a HTTP POST or PUT request. The following parameters are allowed:
   - path (string, required): Either a path relative to the apiUrl, or a full URL path
   - json (dict, optional, default: None): JSON body of the request. The json argument and the data argument cannot both be different from None
   - params (dict, optional, default: None): URL query parameters
```

### Comparing `eniris-0.5.0/setup.py` & `eniris-0.6.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 
 with open("README.md", 'r') as f:
     long_description = f.read()
     
 setup(
   name = 'eniris',
   packages = ['eniris'],
-  version = '0.5.0',
+  version = '0.6.0',
   description = 'Eniris API driver for Python',
   license='MIT',
   long_description=long_description,
   long_description_content_type="text/markdown",
   author = 'Enris BV',
   author_email = 'info@eniris.be',
   url = 'https://github.com/eniris-international/eniris-api-python-driver',
-  download_url = 'https://github.com/eniris-international/eniris-api-python-driver/archive/refs/tags/v0.5.0.tar.gz',
+  download_url = 'https://github.com/eniris-international/eniris-api-python-driver/archive/refs/tags/v0.6.0.tar.gz',
   keywords = ['eniris', 'api', 'rest'],   # Keywords that define your package best
   install_requires=[
     'requests',
   ],
   classifiers=[
     'Development Status :: 4 - Beta',      # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state of your package
     'Intended Audience :: Developers',
```

