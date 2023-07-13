# Comparing `tmp/osim_utils-0.6.2.tar.gz` & `tmp/osim_utils-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "osim_utils-0.6.2.tar", max compression
+gzip compressed data, was "osim_utils-0.6.3.tar", max compression
```

## Comparing `osim_utils-0.6.2.tar` & `osim_utils-0.6.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      232 2023-05-03 10:56:19.733098 osim_utils-0.6.2/README.md
--rw-r--r--   0        0        0     1379 2023-07-13 15:40:44.165207 osim_utils-0.6.2/osim_utils/clients/crossref.py
--rw-r--r--   0        0        0     1828 2023-07-13 15:41:25.010976 osim_utils-0.6.2/osim_utils/clients/embl_data_warehouse.py
--rw-r--r--   0        0        0     5520 2023-07-13 15:42:11.917272 osim_utils-0.6.2/osim_utils/clients/epmc.py
--rw-r--r--   0        0        0     5022 2023-07-13 15:40:44.169302 osim_utils-0.6.2/osim_utils/clients/openalex.py
--rw-r--r--   0        0        0      831 2023-07-13 12:57:57.194267 osim_utils-0.6.2/osim_utils/clients/ror.py
--rw-r--r--   0        0        0     2550 2023-07-13 15:42:23.606888 osim_utils-0.6.2/osim_utils/clients/sherpa.py
--rw-r--r--   0        0        0      271 2023-05-03 13:04:39.071567 osim_utils-0.6.2/osim_utils/common.py
--rw-r--r--   0        0        0      311 2023-05-03 13:04:39.071765 osim_utils-0.6.2/osim_utils/constants.py
--rw-r--r--   0        0        0     1497 2023-06-07 12:38:09.090134 osim_utils-0.6.2/osim_utils/decorators.py
--rw-r--r--   0        0        0      769 2023-06-07 12:38:09.090340 osim_utils-0.6.2/osim_utils/exceptions.py
--rw-r--r--   0        0        0     2532 2023-01-12 14:22:33.188019 osim_utils-0.6.2/osim_utils/logger.py
--rw-r--r--   0        0        0      434 2023-07-13 15:42:26.968955 osim_utils-0.6.2/pyproject.toml
--rw-r--r--   0        0        0      705 1970-01-01 00:00:00.000000 osim_utils-0.6.2/PKG-INFO
+-rw-r--r--   0        0        0      232 2023-05-03 10:56:19.733098 osim_utils-0.6.3/README.md
+-rw-r--r--   0        0        0     1379 2023-07-13 15:40:44.165207 osim_utils-0.6.3/osim_utils/clients/crossref.py
+-rw-r--r--   0        0        0     1828 2023-07-13 15:41:25.010976 osim_utils-0.6.3/osim_utils/clients/embl_data_warehouse.py
+-rw-r--r--   0        0        0     5532 2023-07-13 15:43:19.021977 osim_utils-0.6.3/osim_utils/clients/epmc.py
+-rw-r--r--   0        0        0     5022 2023-07-13 15:40:44.169302 osim_utils-0.6.3/osim_utils/clients/openalex.py
+-rw-r--r--   0        0        0      831 2023-07-13 12:57:57.194267 osim_utils-0.6.3/osim_utils/clients/ror.py
+-rw-r--r--   0        0        0     2550 2023-07-13 15:42:23.606888 osim_utils-0.6.3/osim_utils/clients/sherpa.py
+-rw-r--r--   0        0        0      271 2023-05-03 13:04:39.071567 osim_utils-0.6.3/osim_utils/common.py
+-rw-r--r--   0        0        0      311 2023-05-03 13:04:39.071765 osim_utils-0.6.3/osim_utils/constants.py
+-rw-r--r--   0        0        0     1497 2023-06-07 12:38:09.090134 osim_utils-0.6.3/osim_utils/decorators.py
+-rw-r--r--   0        0        0      769 2023-06-07 12:38:09.090340 osim_utils-0.6.3/osim_utils/exceptions.py
+-rw-r--r--   0        0        0     2532 2023-01-12 14:22:33.188019 osim_utils-0.6.3/osim_utils/logger.py
+-rw-r--r--   0        0        0      434 2023-07-13 15:51:19.001298 osim_utils-0.6.3/pyproject.toml
+-rw-r--r--   0        0        0      705 1970-01-01 00:00:00.000000 osim_utils-0.6.3/PKG-INFO
```

### Comparing `osim_utils-0.6.2/osim_utils/clients/crossref.py` & `osim_utils-0.6.3/osim_utils/clients/crossref.py`

 * *Files identical despite different names*

### Comparing `osim_utils-0.6.2/osim_utils/clients/embl_data_warehouse.py` & `osim_utils-0.6.3/osim_utils/clients/embl_data_warehouse.py`

 * *Files identical despite different names*

### Comparing `osim_utils-0.6.2/osim_utils/clients/epmc.py` & `osim_utils-0.6.3/osim_utils/clients/epmc.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         except KeyError:
             raise ValueError(
                 "You must include a 'query' parameter when calling this method"
             )
 
     @process_response
     @check_response(HTTPStatus.OK)
-    def search(self, **kwargs) -> requests.models.Response:
+    def search(self, **kwargs) -> requests_cache.models.Response:
         """
         Queries the publication database using the GET search endpoint
 
         Args:
             **kwargs:
                 query (required; str): query string
 
@@ -51,15 +51,15 @@
         self._check_query(**kwargs)
         endpoint = f"{self.base_url}search"
         params = self.common_params | kwargs
         return self.session.get(endpoint, params=params)
 
     @process_response
     @check_response(HTTPStatus.OK)
-    def search_post(self, **kwargs) -> requests.models.Response:
+    def search_post(self, **kwargs) -> requests_cache.models.Response:
         """
         Queries the publication database using the POST searchPOST endpoint
 
         Args:
             **kwargs:
                 query (str): query string
                 resultType (str): It can have the following values:
```

### Comparing `osim_utils-0.6.2/osim_utils/clients/openalex.py` & `osim_utils-0.6.3/osim_utils/clients/openalex.py`

 * *Files identical despite different names*

### Comparing `osim_utils-0.6.2/osim_utils/clients/ror.py` & `osim_utils-0.6.3/osim_utils/clients/ror.py`

 * *Files identical despite different names*

### Comparing `osim_utils-0.6.2/osim_utils/clients/sherpa.py` & `osim_utils-0.6.3/osim_utils/clients/sherpa.py`

 * *Files identical despite different names*

### Comparing `osim_utils-0.6.2/osim_utils/decorators.py` & `osim_utils-0.6.3/osim_utils/decorators.py`

 * *Files identical despite different names*

### Comparing `osim_utils-0.6.2/osim_utils/exceptions.py` & `osim_utils-0.6.3/osim_utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `osim_utils-0.6.2/osim_utils/logger.py` & `osim_utils-0.6.3/osim_utils/logger.py`

 * *Files identical despite different names*

### Comparing `osim_utils-0.6.2/PKG-INFO` & `osim_utils-0.6.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osim-utils
-Version: 0.6.2
+Version: 0.6.3
 Summary: 
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

