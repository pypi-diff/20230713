# Comparing `tmp/trustedtwin-0.4.9.tar.gz` & `tmp/trustedtwin-3.4.20230713205841.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trustedtwin-0.4.9.tar", last modified: Fri Sep 30 10:44:50 2022, max compression
+gzip compressed data, was "trustedtwin-3.4.20230713205841.tar", last modified: Thu Jul 13 20:58:58 2023, max compression
```

## Comparing `trustedtwin-0.4.9.tar` & `trustedtwin-3.4.20230713205841.tar`

### file list

```diff
@@ -1,49 +1,21 @@
-drwxr-xr-x   0 rekowskip  (1000) rekowskip  (1000)        0 2022-09-30 10:44:50.528953 trustedtwin-0.4.9/
--rw-r--r--   0 rekowskip  (1000) rekowskip  (1000)     1106 2022-04-26 12:40:06.000000 trustedtwin-0.4.9/LICENSE
--rw-r--r--   0 rekowskip  (1000) rekowskip  (1000)      941 2022-09-30 10:44:50.528953 trustedtwin-0.4.9/PKG-INFO
--rw-r--r--   0 rekowskip  (1000) rekowskip  (1000)      625 2022-04-26 12:40:06.000000 trustedtwin-0.4.9/README.md
-drwxr-xr-x   0 rekowskip  (1000) rekowskip  (1000)        0 2022-09-30 10:44:50.524953 trustedtwin-0.4.9/api_generator/
--rw-r--r--   0 rekowskip  (1000) rekowskip  (1000)        0 2022-04-26 12:40:06.000000 trustedtwin-0.4.9/api_generator/__init__.py
--rw-r--r--   0 rekowskip  (1000) rekowskip  (1000)    12134 2022-05-19 08:31:57.000000 trustedtwin-0.4.9/api_generator/generate.py
--rw-r--r--   0 rekowskip  (1000) rekowskip  (1000)     2545 2022-06-07 10:10:43.000000 trustedtwin-0.4.9/api_generator/templates.py
-drwxr-xr-x   0 rekowskip  (1000) rekowskip  (1000)        0 2022-09-30 10:44:50.528953 trustedtwin-0.4.9/examples/
--rw-r--r--   0 rekowskip  (1000) rekowskip  (1000)        0 2022-04-26 12:40:06.000000 trustedtwin-0.4.9/examples/__init__.py
--rw-r--r--   0 rekowskip  (1000) rekowskip  (1000)     3461 2022-09-16 13:45:24.000000 trustedtwin-0.4.9/examples/ledgers.py
--rw-r--r--   0 rekowskip  (1000) rekowskip  (1000)     1495 2022-09-16 13:45:24.000000 trustedtwin-0.4.9/examples/twins.py
--rw-r--r--   0 rekowskip  (1000) rekowskip  (1000)      103 2022-09-30 10:44:50.528953 trustedtwin-0.4.9/setup.cfg
--rw-r--r--   0 rekowskip  (1000) rekowskip  (1000)      518 2022-09-30 10:40:10.000000 trustedtwin-0.4.9/setup.py
-drwxr-xr-x   0 rekowskip  (1000) rekowskip  (1000)        0 2022-09-30 10:44:50.528953 trustedtwin-0.4.9/trustedtwin/
--rw-r--r--   0 rekowskip  (1000) rekowskip  (1000)      129 2022-04-26 12:40:06.000000 trustedtwin-0.4.9/trustedtwin/__init__.py
--rw-r--r--   0 rekowskip  (1000) rekowskip  (1000)     2990 2022-09-16 13:45:24.000000 trustedtwin-0.4.9/trustedtwin/exceptions.py
--rw-r--r--   0 rekowskip  (1000) rekowskip  (1000)     3323 2022-09-16 13:45:24.000000 trustedtwin-0.4.9/trustedtwin/http_client.py
--rw-r--r--   0 rekowskip  (1000) rekowskip  (1000)      319 2022-04-26 12:40:06.000000 trustedtwin-0.4.9/trustedtwin/misc.py
-drwxr-xr-x   0 rekowskip  (1000) rekowskip  (1000)        0 2022-09-30 10:44:50.528953 trustedtwin-0.4.9/trustedtwin/models/
--rw-r--r--   0 rekowskip  (1000) rekowskip  (1000)        0 2022-04-26 12:40:06.000000 trustedtwin-0.4.9/trustedtwin/models/__init__.py
--rw-r--r--   0 rekowskip  (1000) rekowskip  (1000)      839 2022-04-26 12:40:06.000000 trustedtwin-0.4.9/trustedtwin/models/responses.py
-drwxr-xr-x   0 rekowskip  (1000) rekowskip  (1000)        0 2022-09-30 10:44:50.528953 trustedtwin-0.4.9/trustedtwin/operations/
--rw-r--r--   0 rekowskip  (1000) rekowskip  (1000)        0 2022-04-26 12:40:06.000000 trustedtwin-0.4.9/trustedtwin/operations/__init__.py
--rw-r--r--   0 rekowskip  (1000) rekowskip  (1000)     4998 2022-09-16 13:45:24.000000 trustedtwin-0.4.9/trustedtwin/operations/docs.py
--rw-r--r--   0 rekowskip  (1000) rekowskip  (1000)     1551 2022-09-16 13:45:24.000000 trustedtwin-0.4.9/trustedtwin/operations/history.py
--rw-r--r--   0 rekowskip  (1000) rekowskip  (1000)     4773 2022-09-16 13:45:24.000000 trustedtwin-0.4.9/trustedtwin/operations/identities.py
--rw-r--r--   0 rekowskip  (1000) rekowskip  (1000)     4320 2022-09-29 10:14:24.000000 trustedtwin-0.4.9/trustedtwin/operations/indexes.py
--rw-r--r--   0 rekowskip  (1000) rekowskip  (1000)     3635 2022-09-16 13:45:24.000000 trustedtwin-0.4.9/trustedtwin/operations/ledgers.py
--rw-r--r--   0 rekowskip  (1000) rekowskip  (1000)     1110 2022-09-16 13:45:24.000000 trustedtwin-0.4.9/trustedtwin/operations/log.py
--rw-r--r--   0 rekowskip  (1000) rekowskip  (1000)     3144 2022-09-16 13:45:24.000000 trustedtwin-0.4.9/trustedtwin/operations/notifications.py
--rw-r--r--   0 rekowskip  (1000) rekowskip  (1000)     3288 2022-09-16 13:45:24.000000 trustedtwin-0.4.9/trustedtwin/operations/roles.py
--rw-r--r--   0 rekowskip  (1000) rekowskip  (1000)     3215 2022-09-16 13:45:24.000000 trustedtwin-0.4.9/trustedtwin/operations/secrets.py
--rw-r--r--   0 rekowskip  (1000) rekowskip  (1000)     3933 2022-09-30 10:25:16.000000 trustedtwin-0.4.9/trustedtwin/operations/stickers.py
--rw-r--r--   0 rekowskip  (1000) rekowskip  (1000)     4842 2022-09-29 10:14:24.000000 trustedtwin-0.4.9/trustedtwin/operations/timeseries.py
--rw-r--r--   0 rekowskip  (1000) rekowskip  (1000)     1833 2022-09-27 13:35:12.000000 trustedtwin-0.4.9/trustedtwin/operations/token.py
--rw-r--r--   0 rekowskip  (1000) rekowskip  (1000)      571 2022-09-16 13:45:24.000000 trustedtwin-0.4.9/trustedtwin/operations/trace.py
--rw-r--r--   0 rekowskip  (1000) rekowskip  (1000)     2767 2022-09-16 13:45:24.000000 trustedtwin-0.4.9/trustedtwin/operations/twins.py
--rw-r--r--   0 rekowskip  (1000) rekowskip  (1000)     1375 2022-09-16 13:45:24.000000 trustedtwin-0.4.9/trustedtwin/operations/usage.py
--rw-r--r--   0 rekowskip  (1000) rekowskip  (1000)     2843 2022-09-16 13:45:24.000000 trustedtwin-0.4.9/trustedtwin/operations/users.py
--rw-r--r--   0 rekowskip  (1000) rekowskip  (1000)      583 2022-09-16 13:45:24.000000 trustedtwin-0.4.9/trustedtwin/operations/who_am_i.py
--rw-r--r--   0 rekowskip  (1000) rekowskip  (1000)     4398 2022-09-29 10:14:24.000000 trustedtwin-0.4.9/trustedtwin/service.py
-drwxr-xr-x   0 rekowskip  (1000) rekowskip  (1000)        0 2022-09-30 10:44:50.528953 trustedtwin-0.4.9/trustedtwin.egg-info/
--rw-r--r--   0 rekowskip  (1000) rekowskip  (1000)      941 2022-09-30 10:44:50.000000 trustedtwin-0.4.9/trustedtwin.egg-info/PKG-INFO
--rw-r--r--   0 rekowskip  (1000) rekowskip  (1000)     1173 2022-09-30 10:44:50.000000 trustedtwin-0.4.9/trustedtwin.egg-info/SOURCES.txt
--rw-r--r--   0 rekowskip  (1000) rekowskip  (1000)        1 2022-09-30 10:44:50.000000 trustedtwin-0.4.9/trustedtwin.egg-info/dependency_links.txt
--rw-r--r--   0 rekowskip  (1000) rekowskip  (1000)        1 2022-05-20 04:10:03.000000 trustedtwin-0.4.9/trustedtwin.egg-info/not-zip-safe
--rw-r--r--   0 rekowskip  (1000) rekowskip  (1000)        9 2022-09-30 10:44:50.000000 trustedtwin-0.4.9/trustedtwin.egg-info/requires.txt
--rw-r--r--   0 rekowskip  (1000) rekowskip  (1000)       35 2022-09-30 10:44:50.000000 trustedtwin-0.4.9/trustedtwin.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 20:58:58.701361 trustedtwin-3.4.20230713205841/
+-rw-rw-rw-   0 root         (0) root         (0)     1106 2023-07-13 20:58:38.000000 trustedtwin-3.4.20230713205841/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      922 2023-07-13 20:58:58.701361 trustedtwin-3.4.20230713205841/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      616 2023-07-13 20:58:38.000000 trustedtwin-3.4.20230713205841/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      103 2023-07-13 20:58:58.701361 trustedtwin-3.4.20230713205841/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1156 2023-07-13 20:58:38.000000 trustedtwin-3.4.20230713205841/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 20:58:58.699361 trustedtwin-3.4.20230713205841/trustedtwin/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-13 20:58:38.000000 trustedtwin-3.4.20230713205841/trustedtwin/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2331 2023-07-13 20:58:38.000000 trustedtwin-3.4.20230713205841/trustedtwin/tt_api.py
+-rw-r--r--   0 root         (0) root         (0)   105509 2023-07-13 20:58:58.000000 trustedtwin-3.4.20230713205841/trustedtwin/tt_api.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     2466 2023-07-13 20:58:38.000000 trustedtwin-3.4.20230713205841/trustedtwin/tt_api_async.py
+-rw-r--r--   0 root         (0) root         (0)   126439 2023-07-13 20:58:58.000000 trustedtwin-3.4.20230713205841/trustedtwin/tt_api_async.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     2614 2023-07-13 20:58:38.000000 trustedtwin-3.4.20230713205841/trustedtwin/tt_api_base.py
+-rw-r--r--   0 root         (0) root         (0)     4195 2023-07-13 20:58:58.000000 trustedtwin-3.4.20230713205841/trustedtwin/tt_endpoints.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 20:58:58.701361 trustedtwin-3.4.20230713205841/trustedtwin.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      922 2023-07-13 20:58:58.000000 trustedtwin-3.4.20230713205841/trustedtwin.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      425 2023-07-13 20:58:58.000000 trustedtwin-3.4.20230713205841/trustedtwin.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-13 20:58:58.000000 trustedtwin-3.4.20230713205841/trustedtwin.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-13 20:58:58.000000 trustedtwin-3.4.20230713205841/trustedtwin.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       58 2023-07-13 20:58:58.000000 trustedtwin-3.4.20230713205841/trustedtwin.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-07-13 20:58:58.000000 trustedtwin-3.4.20230713205841/trustedtwin.egg-info/top_level.txt
```

### Comparing `trustedtwin-0.4.9/LICENSE` & `trustedtwin-3.4.20230713205841/LICENSE`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 The MIT License (MIT)
 
-Copyright (c) 2022 Trusted Twin - https://trustedtwin.com/
+Copyright (c) 2023 Trusted Twin - https://trustedtwin.com/
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"),
 to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense,
 and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
```

### Comparing `trustedtwin-0.4.9/trustedtwin/http_client.py` & `trustedtwin-3.4.20230713205841/trustedtwin/tt_api_base.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,115 +1,86 @@
-"""HTTP client for TrustedTwin API client"""
-import json
+"""Trusted Twin API call library"""
 import logging
-import threading
+import json
+
+from typing import Any, Dict, Tuple, Optional, Union
 from base64 import b64encode
-from typing import Dict, Optional, Any
 
-from requests import Response, Session
+# tt_endpoints is generated automatically
+from trustedtwin.tt_endpoints import ENDPOINTS
+
+logger = logging.getLogger(__name__)
+
+# Number of tries before failure
+_TT_RETRIES = 5
+_TT_RETRIES_SLEEP = 2
+
+# Logger message
+_LOG_TEMPLATE = "TrustedTwin REST API call failed: Attempt=[%d], URL=[%s], Code=[%d], Response=[%s]."
 
-from trustedtwin.misc import RESTMethod
-from trustedtwin.models.responses import TTResponse
+# TrustedTwin headers
+_TT_DICT_HEADER = 'X-TrustedTwin'
+_TT_AUTH_HEADER = "Authorization"
 
-logger = logging.getLogger("trustedtwin")
 
-TT_DICT_HEADER = 'X-TrustedTwin'
+class TTEndpointBase:
+    """Trusted Twin endpoint base."""
 
+    def __init__(self, method: str, url: str, headers: Dict, session: Optional[Any] = None, codes: Optional[Dict] = None) -> None:
+        """Base class init."""
+        self.method = method
+        self.url = url
+        self.headers = headers
+        self.session = session
+        self.codes = codes
 
-def http_header_encode(dictionary: Dict) -> str:
-    """Encode dictionary into base64 string"""
-    return b64encode(json.dumps(dictionary).encode('utf-8')).decode('utf-8')
+    def __call__(self, *args: Any, **kwargs: Any) -> Tuple[int, str]:
+        raise NotImplementedError
 
 
-class HTTPClient:
-    """HTTP client used by TrustedTwin Service"""
+class TTRESTServiceBase:
+    """Trusted Twin REST client base."""
+    _endpoint_type = TTEndpointBase
 
     def __init__(
-            self,
-            host_name: str,
-            auth: Optional[str] = None,
-            session: Optional[Session] = None,
-            tt_dict: Optional[Dict] = None
-    ):
-        """Initialize object.
-
-        :param auth: authorization token
-        :param host_name: string containing host name
-        """
-        self.host_name = host_name
-        self._headers = {"Content-Type": "application/json"}
-        self._locals = threading.local()
+        self,
+        tt_auth: str,
+        tt_base: Optional[str] = None,
+        tt_dict: Optional[Dict] = None,
+        session: Optional[Any] = None,
+        codes: Optional[Dict] = None,
+    ) -> None:
+        self._headers = {
+            'Content-Type': "application/json",
+            _TT_AUTH_HEADER: tt_auth
+        }
+        if tt_dict is not None:
+            self._headers[_TT_DICT_HEADER] = b64encode(json.dumps(tt_dict).encode('utf-8')).decode('utf-8')
+
+        self._base = tt_base or 'https://rest.trustedtwin.com'
         self._session = session
+        self._codes = codes
 
-        if auth:
-            self._headers["Authorization"] = auth
-        else:
-            logger.warning("Warning - Auth token not set")
-
-        if tt_dict:
-            self._headers[TT_DICT_HEADER] = http_header_encode(tt_dict)
-
-    def __repr__(self) -> str:
-        """Return nicer print presentation."""
-        return "{} - {}".format(self.__class__.__name__, self.host_name)
+        self._cache = {}
 
-    def _call(
-        self,
-        method: RESTMethod,
-        url: str,
-        headers: Optional[Dict] = None,
-        body: Optional[Dict] = None,
-        params: Optional[Dict] = None,
-        **kwargs: Any
-    ) -> Response:
-        """Perform actual call to API
-
-        :param method: REST API method to be executed on an endpoint e.g. 'GET', 'POST', 'PATCH'
-        :param url: url to be called
-        :param headers: headers for request
-        :param body: optional payload passed as a json object
-        :param params: optional parameters passed as key-worded arguments
-        :return: endpoint response
-        """
-        _method = str(method).lower()
-        logging.debug("Calling url: %s", url)
-
-        if getattr(self._locals, "session", None) is None:
-            self._locals.session = self._session or Session()
-
-        return self._locals.session.request(
-            method=_method,
-            url=url,
-            data=json.dumps(body) if body else None,
-            headers=headers,
-            params=params,
-            **kwargs
-        )
+        assert issubclass(self._endpoint_type, TTEndpointBase), "ASSERT 0dc15258-8569-4bba-89a2-fa5f255431e4"
+        assert isinstance(self._codes, (type(None), Dict)), "ASSERT 976039b6-431d-4120-bec0-1b7a3fd84eec"
 
+    def __getattr__(self, name: str) -> Union[TTEndpointBase, Any]:
+        if name in ENDPOINTS:
+            _endpoint = self._cache.get(name, None)
 
-    def execute_request(
-        self,
-        method: RESTMethod,
-        url_root: str,
-        endpoint: str,
-        body: Optional[Dict] = None,
-        params: Optional[Dict] = None,
-        **kwargs: Any
-    ) -> TTResponse:
-        """Execute API request"""
-        url = "{}/{}".format(url_root, endpoint)
-        params = (
-            {key: value for key, value in params.items() if value is not None}
-            if params
-            else {}
-        )
-
-        response = self._call(
-            method=method,
-            url=url,
-            body=body,
-            params=params,
-            headers=self._headers,
-            **kwargs
-        )
+            if _endpoint is None:
+                _method, _url = ENDPOINTS[name]
+                _endpoint = self._endpoint_type(
+                    method=_method,
+                    url=self._base + _url,
+                    headers=self._headers,
+                    session=self._session,
+                    codes=self._codes
+                )
+
+                self._cache[name] = _endpoint
+
+            return _endpoint
 
-        return TTResponse(body=response.text, http_code=response.status_code)
+        return super().__getattribute__(name)
```

