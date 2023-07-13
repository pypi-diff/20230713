# Comparing `tmp/osim_utils-0.6.1.tar.gz` & `tmp/osim_utils-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "osim_utils-0.6.1.tar", max compression
+gzip compressed data, was "osim_utils-0.6.2.tar", max compression
```

## Comparing `osim_utils-0.6.1.tar` & `osim_utils-0.6.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      232 2023-05-03 10:56:19.733098 osim_utils-0.6.1/README.md
--rw-r--r--   0        0        0     1446 2023-05-08 15:34:27.529473 osim_utils-0.6.1/osim_utils/clients/crossref.py
--rw-r--r--   0        0        0     1737 2023-06-14 09:36:56.204537 osim_utils-0.6.1/osim_utils/clients/embl_data_warehouse.py
--rw-r--r--   0        0        0     5470 2023-06-07 12:38:09.089910 osim_utils-0.6.1/osim_utils/clients/epmc.py
--rw-r--r--   0        0        0     4903 2023-06-28 15:50:58.664838 osim_utils-0.6.1/osim_utils/clients/openalex.py
--rw-r--r--   0        0        0      831 2023-07-13 12:57:57.194267 osim_utils-0.6.1/osim_utils/clients/ror.py
--rw-r--r--   0        0        0     2539 2023-06-07 09:08:46.139525 osim_utils-0.6.1/osim_utils/clients/sherpa.py
--rw-r--r--   0        0        0      271 2023-05-03 13:04:39.071567 osim_utils-0.6.1/osim_utils/common.py
--rw-r--r--   0        0        0      311 2023-05-03 13:04:39.071765 osim_utils-0.6.1/osim_utils/constants.py
--rw-r--r--   0        0        0     1497 2023-06-07 12:38:09.090134 osim_utils-0.6.1/osim_utils/decorators.py
--rw-r--r--   0        0        0      769 2023-06-07 12:38:09.090340 osim_utils-0.6.1/osim_utils/exceptions.py
--rw-r--r--   0        0        0     2532 2023-01-12 14:22:33.188019 osim_utils-0.6.1/osim_utils/logger.py
--rw-r--r--   0        0        0      434 2023-07-13 12:59:12.631315 osim_utils-0.6.1/pyproject.toml
--rw-r--r--   0        0        0      705 1970-01-01 00:00:00.000000 osim_utils-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0      232 2023-05-03 10:56:19.733098 osim_utils-0.6.2/README.md
+-rw-r--r--   0        0        0     1379 2023-07-13 15:40:44.165207 osim_utils-0.6.2/osim_utils/clients/crossref.py
+-rw-r--r--   0        0        0     1828 2023-07-13 15:41:25.010976 osim_utils-0.6.2/osim_utils/clients/embl_data_warehouse.py
+-rw-r--r--   0        0        0     5520 2023-07-13 15:42:11.917272 osim_utils-0.6.2/osim_utils/clients/epmc.py
+-rw-r--r--   0        0        0     5022 2023-07-13 15:40:44.169302 osim_utils-0.6.2/osim_utils/clients/openalex.py
+-rw-r--r--   0        0        0      831 2023-07-13 12:57:57.194267 osim_utils-0.6.2/osim_utils/clients/ror.py
+-rw-r--r--   0        0        0     2550 2023-07-13 15:42:23.606888 osim_utils-0.6.2/osim_utils/clients/sherpa.py
+-rw-r--r--   0        0        0      271 2023-05-03 13:04:39.071567 osim_utils-0.6.2/osim_utils/common.py
+-rw-r--r--   0        0        0      311 2023-05-03 13:04:39.071765 osim_utils-0.6.2/osim_utils/constants.py
+-rw-r--r--   0        0        0     1497 2023-06-07 12:38:09.090134 osim_utils-0.6.2/osim_utils/decorators.py
+-rw-r--r--   0        0        0      769 2023-06-07 12:38:09.090340 osim_utils-0.6.2/osim_utils/exceptions.py
+-rw-r--r--   0        0        0     2532 2023-01-12 14:22:33.188019 osim_utils-0.6.2/osim_utils/logger.py
+-rw-r--r--   0        0        0      434 2023-07-13 15:42:26.968955 osim_utils-0.6.2/pyproject.toml
+-rw-r--r--   0        0        0      705 1970-01-01 00:00:00.000000 osim_utils-0.6.2/PKG-INFO
```

### Comparing `osim_utils-0.6.1/osim_utils/clients/crossref.py` & `osim_utils-0.6.2/osim_utils/clients/crossref.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 import os
-import requests
-import urllib.parse
+import requests_cache
+from datetime import timedelta
 from http import HTTPStatus
-from typing import Optional, Union
+from typing import Optional
 
 from osim_utils.logger import get_logger
-from osim_utils.constants import ror_id2site
 from osim_utils.decorators import check_response, process_response
-from osim_utils.exceptions import DataNotFoundError, DataValidationError
-from osim_utils.common import chunk_list
 
 
 class CrossRefClient:
     """
     Client for CrossRef API
     """
 
     def __init__(self, user_email: Optional[str] = None):
-        self.session = requests.Session()
+        self.session = requests_cache.CachedSession(
+            "crossref_cache", expire_after=timedelta(days=7)
+        )
         self.logger = get_logger()
         self.user_email = user_email
         self.common_params = {"format": "json"}
         if user_email is None:
             try:
                 self.user_email = os.environ["CROSSREF_EMAIL"]
             except KeyError:
```

### Comparing `osim_utils-0.6.1/osim_utils/clients/embl_data_warehouse.py` & `osim_utils-0.6.2/osim_utils/clients/embl_data_warehouse.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,27 @@
-import functools
-import json
 import os
-import requests
+import requests_cache
+from datetime import timedelta
 from http import HTTPStatus
 
 import osim_utils.exceptions as exc
 from osim_utils.decorators import check_response, process_response
 from osim_utils.logger import get_logger
 
 
 class DataWareClient:
     """
     API client for EMBL's data warehouse API (Converis mirror)
     """
 
     def __init__(self):
         self.base_url = "https://xs-db.embl.de/v2/publications/"
-        self.session = requests.Session()
+        self.session = requests_cache.CachedSession(
+            "warehouse_cache", expire_after=timedelta(days=7)
+        )
         self.logger = get_logger()
 
         token_env_var = "DataWareHouseToken"
         self.default_headers = dict()
         try:
             self.default_headers[
                 "Authorization"
```

### Comparing `osim_utils-0.6.1/osim_utils/clients/epmc.py` & `osim_utils-0.6.2/osim_utils/clients/epmc.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-import functools
-import json
-import requests
+import requests_cache
+from datetime import timedelta
 from osim_utils.logger import get_logger
 
 from http import HTTPStatus
-import osim_utils.exceptions as exc
 from osim_utils.decorators import check_response, process_response
 
 
 class EpmcClient:
     """
     API client for EuropePMC Articles REST API
     (https://europepmc.org/RestfulWebService)
     """
 
     def __init__(self):
         self.base_url = "https://www.ebi.ac.uk/europepmc/webservices/rest/"
         self.common_params = {"format": "json"}
-        self.session = requests.Session()
+        self.session = requests_cache.CachedSession(
+            "epmc_cache", expire_after=timedelta(days=7)
+        )
         self.logger = get_logger()
 
     @staticmethod
     def _check_query(**kwargs) -> str:
         """
         Check that required "query" argument was passed to calling method
         Args:
```

### Comparing `osim_utils-0.6.1/osim_utils/clients/openalex.py` & `osim_utils-0.6.2/osim_utils/clients/openalex.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import os
-import requests
+import requests_cache
 import urllib.parse
+from datetime import timedelta
 from http import HTTPStatus
 from typing import Optional
 
 from osim_utils.logger import get_logger
 from osim_utils.constants import ror_id2site
 from osim_utils.decorators import check_response, process_response
 from osim_utils.common import chunk_list
@@ -16,15 +17,17 @@
     """
 
     max_page_size = 50
 
     def __init__(self):
         self.base_endpoint = "https://api.openalex.org"
         self.works_endpoint = f"{self.base_endpoint}/works"
-        self.session = requests.Session()
+        self.session = requests_cache.CachedSession(
+            "openalex_cache", expire_after=timedelta(days=7)
+        )
         self.logger = get_logger()
 
         req_env_var = "OpenAlexRequester"
         self.default_headers = dict()
         try:
             self.default_headers["User-agent"] = f"mailto:{os.environ[req_env_var]}"
         except KeyError:
```

### Comparing `osim_utils-0.6.1/osim_utils/clients/ror.py` & `osim_utils-0.6.2/osim_utils/clients/ror.py`

 * *Files identical despite different names*

### Comparing `osim_utils-0.6.1/osim_utils/clients/sherpa.py` & `osim_utils-0.6.2/osim_utils/clients/sherpa.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 import os
-import requests
-import urllib.parse
+import requests_cache
+from datetime import timedelta
 from http import HTTPStatus
 from typing import Optional, Union
 
 from osim_utils.logger import get_logger
-from osim_utils.constants import ror_id2site
 from osim_utils.decorators import check_response, process_response
 from osim_utils.exceptions import DataNotFoundError, DataValidationError
-from osim_utils.common import chunk_list
 
 
 class SherpaClient:
     """
     Client for JISC Sherpa APIs
     """
 
@@ -24,15 +22,17 @@
                 self.api_key = os.environ["SHERPA_KEY"]
             except KeyError:
                 raise DataNotFoundError(
                     "Could not find API key for JISC Sherpa services; please store the key "
                     "value in environment variable SHERPA_KEY or pass the key value directly as attribute api_key"
                     "when instantiating this SherpaClient"
                 )
-        self.session = requests.Session()
+        self.session = requests_cache.CachedSession(
+            "sherpa_cache", expire_after=timedelta(days=7)
+        )
         self.logger = get_logger()
 
     @process_response
     @check_response(HTTPStatus.OK)
     def get(self, **kwargs):
         params = {
             "api-key": self.api_key,
```

### Comparing `osim_utils-0.6.1/osim_utils/decorators.py` & `osim_utils-0.6.2/osim_utils/decorators.py`

 * *Files identical despite different names*

### Comparing `osim_utils-0.6.1/osim_utils/exceptions.py` & `osim_utils-0.6.2/osim_utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `osim_utils-0.6.1/osim_utils/logger.py` & `osim_utils-0.6.2/osim_utils/logger.py`

 * *Files identical despite different names*

### Comparing `osim_utils-0.6.1/PKG-INFO` & `osim_utils-0.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osim-utils
-Version: 0.6.1
+Version: 0.6.2
 Summary: 
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

