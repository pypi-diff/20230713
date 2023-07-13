# Comparing `tmp/osim_utils-0.6.3.tar.gz` & `tmp/osim_utils-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "osim_utils-0.6.3.tar", max compression
+gzip compressed data, was "osim_utils-0.6.4.tar", max compression
```

## Comparing `osim_utils-0.6.3.tar` & `osim_utils-0.6.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      232 2023-05-03 10:56:19.733098 osim_utils-0.6.3/README.md
--rw-r--r--   0        0        0     1379 2023-07-13 15:40:44.165207 osim_utils-0.6.3/osim_utils/clients/crossref.py
--rw-r--r--   0        0        0     1828 2023-07-13 15:41:25.010976 osim_utils-0.6.3/osim_utils/clients/embl_data_warehouse.py
--rw-r--r--   0        0        0     5532 2023-07-13 15:43:19.021977 osim_utils-0.6.3/osim_utils/clients/epmc.py
--rw-r--r--   0        0        0     5022 2023-07-13 15:40:44.169302 osim_utils-0.6.3/osim_utils/clients/openalex.py
--rw-r--r--   0        0        0      831 2023-07-13 12:57:57.194267 osim_utils-0.6.3/osim_utils/clients/ror.py
--rw-r--r--   0        0        0     2550 2023-07-13 15:42:23.606888 osim_utils-0.6.3/osim_utils/clients/sherpa.py
--rw-r--r--   0        0        0      271 2023-05-03 13:04:39.071567 osim_utils-0.6.3/osim_utils/common.py
--rw-r--r--   0        0        0      311 2023-05-03 13:04:39.071765 osim_utils-0.6.3/osim_utils/constants.py
--rw-r--r--   0        0        0     1497 2023-06-07 12:38:09.090134 osim_utils-0.6.3/osim_utils/decorators.py
--rw-r--r--   0        0        0      769 2023-06-07 12:38:09.090340 osim_utils-0.6.3/osim_utils/exceptions.py
--rw-r--r--   0        0        0     2532 2023-01-12 14:22:33.188019 osim_utils-0.6.3/osim_utils/logger.py
--rw-r--r--   0        0        0      434 2023-07-13 15:51:19.001298 osim_utils-0.6.3/pyproject.toml
--rw-r--r--   0        0        0      705 1970-01-01 00:00:00.000000 osim_utils-0.6.3/PKG-INFO
+-rw-r--r--   0        0        0      232 2023-05-03 10:56:19.733098 osim_utils-0.6.4/README.md
+-rw-r--r--   0        0        0     1379 2023-07-13 15:40:44.165207 osim_utils-0.6.4/osim_utils/clients/crossref.py
+-rw-r--r--   0        0        0     1828 2023-07-13 15:41:25.010976 osim_utils-0.6.4/osim_utils/clients/embl_data_warehouse.py
+-rw-r--r--   0        0        0     5532 2023-07-13 15:43:19.021977 osim_utils-0.6.4/osim_utils/clients/epmc.py
+-rw-r--r--   0        0        0     5048 2023-07-13 16:15:11.725821 osim_utils-0.6.4/osim_utils/clients/openalex.py
+-rw-r--r--   0        0        0      831 2023-07-13 12:57:57.194267 osim_utils-0.6.4/osim_utils/clients/ror.py
+-rw-r--r--   0        0        0     2550 2023-07-13 15:42:23.606888 osim_utils-0.6.4/osim_utils/clients/sherpa.py
+-rw-r--r--   0        0        0      271 2023-05-03 13:04:39.071567 osim_utils-0.6.4/osim_utils/common.py
+-rw-r--r--   0        0        0      311 2023-05-03 13:04:39.071765 osim_utils-0.6.4/osim_utils/constants.py
+-rw-r--r--   0        0        0     1497 2023-06-07 12:38:09.090134 osim_utils-0.6.4/osim_utils/decorators.py
+-rw-r--r--   0        0        0      769 2023-06-07 12:38:09.090340 osim_utils-0.6.4/osim_utils/exceptions.py
+-rw-r--r--   0        0        0     2532 2023-01-12 14:22:33.188019 osim_utils-0.6.4/osim_utils/logger.py
+-rw-r--r--   0        0        0      434 2023-07-13 16:15:49.413451 osim_utils-0.6.4/pyproject.toml
+-rw-r--r--   0        0        0      705 1970-01-01 00:00:00.000000 osim_utils-0.6.4/PKG-INFO
```

### Comparing `osim_utils-0.6.3/osim_utils/clients/crossref.py` & `osim_utils-0.6.4/osim_utils/clients/crossref.py`

 * *Files identical despite different names*

### Comparing `osim_utils-0.6.3/osim_utils/clients/embl_data_warehouse.py` & `osim_utils-0.6.4/osim_utils/clients/embl_data_warehouse.py`

 * *Files identical despite different names*

### Comparing `osim_utils-0.6.3/osim_utils/clients/epmc.py` & `osim_utils-0.6.4/osim_utils/clients/epmc.py`

 * *Files identical despite different names*

### Comparing `osim_utils-0.6.3/osim_utils/clients/openalex.py` & `osim_utils-0.6.4/osim_utils/clients/openalex.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,16 +12,14 @@
 
 
 class OpenAlexClient:
     """
     Client for OpenAlex API
     """
 
-    max_page_size = 50
-
     def __init__(self):
         self.base_endpoint = "https://api.openalex.org"
         self.works_endpoint = f"{self.base_endpoint}/works"
         self.session = requests_cache.CachedSession(
             "openalex_cache", expire_after=timedelta(days=7)
         )
         self.logger = get_logger()
@@ -63,19 +61,22 @@
         Args:
             dois: list of dois to be queried
             **kwargs: additional parameters to be passed to the OpenAlex API
 
         Returns: OpenAlex API response
         """
         quoted_dois = [urllib.parse.quote(x) for x in dois]
-        sublists = chunk_list(quoted_dois, self.max_page_size)
+        sublists = chunk_list(quoted_dois, 50)
+        results = list()
         for sl in sublists:
             query = "|".join(sl)
-            params = {"filter": f"doi:{query}", "per-page": self.max_page_size}
-            yield self.get(self.works_endpoint, params=params, **kwargs)
+            params = {"filter": f"doi:{query}", "per-page": 50}
+            r = self.get(self.works_endpoint, params=params, **kwargs)
+            results += r["results"]
+        return results
 
     def get_embl_works(self, filters: dict, **kwargs) -> dict:
         """
         Queries works associated with any of the EMBL ROR ids in ror_id2site
 
         Args:
             filters: additional filters to apply to query
```

### Comparing `osim_utils-0.6.3/osim_utils/clients/ror.py` & `osim_utils-0.6.4/osim_utils/clients/ror.py`

 * *Files identical despite different names*

### Comparing `osim_utils-0.6.3/osim_utils/clients/sherpa.py` & `osim_utils-0.6.4/osim_utils/clients/sherpa.py`

 * *Files identical despite different names*

### Comparing `osim_utils-0.6.3/osim_utils/decorators.py` & `osim_utils-0.6.4/osim_utils/decorators.py`

 * *Files identical despite different names*

### Comparing `osim_utils-0.6.3/osim_utils/exceptions.py` & `osim_utils-0.6.4/osim_utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `osim_utils-0.6.3/osim_utils/logger.py` & `osim_utils-0.6.4/osim_utils/logger.py`

 * *Files identical despite different names*

### Comparing `osim_utils-0.6.3/PKG-INFO` & `osim_utils-0.6.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osim-utils
-Version: 0.6.3
+Version: 0.6.4
 Summary: 
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

