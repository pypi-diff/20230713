# Comparing `tmp/osim_utils-0.5.0.tar.gz` & `tmp/osim_utils-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "osim_utils-0.5.0.tar", max compression
+gzip compressed data, was "osim_utils-0.6.0.tar", max compression
```

## Comparing `osim_utils-0.5.0.tar` & `osim_utils-0.6.0.tar`

### file list

```diff
@@ -1,13 +1,14 @@
--rw-r--r--   0        0        0      232 2023-05-03 10:56:19.733098 osim_utils-0.5.0/README.md
--rw-r--r--   0        0        0     1446 2023-05-08 15:34:27.529473 osim_utils-0.5.0/osim_utils/clients/crossref.py
--rw-r--r--   0        0        0     1732 2023-06-07 12:22:25.951705 osim_utils-0.5.0/osim_utils/clients/embl_data_warehouse.py
--rw-r--r--   0        0        0     5470 2023-06-07 12:06:24.954904 osim_utils-0.5.0/osim_utils/clients/epmc.py
--rw-r--r--   0        0        0     4130 2023-05-03 16:19:44.648513 osim_utils-0.5.0/osim_utils/clients/openalex.py
--rw-r--r--   0        0        0     2539 2023-06-07 09:08:46.139525 osim_utils-0.5.0/osim_utils/clients/sherpa.py
--rw-r--r--   0        0        0      271 2023-05-03 13:04:39.071567 osim_utils-0.5.0/osim_utils/common.py
--rw-r--r--   0        0        0      311 2023-05-03 13:04:39.071765 osim_utils-0.5.0/osim_utils/constants.py
--rw-r--r--   0        0        0     1497 2023-06-07 12:06:24.960205 osim_utils-0.5.0/osim_utils/decorators.py
--rw-r--r--   0        0        0      769 2023-06-07 12:00:54.184987 osim_utils-0.5.0/osim_utils/exceptions.py
--rw-r--r--   0        0        0     2532 2023-01-12 14:22:33.188019 osim_utils-0.5.0/osim_utils/logger.py
--rw-r--r--   0        0        0      408 2023-06-07 12:34:32.461580 osim_utils-0.5.0/pyproject.toml
--rw-r--r--   0        0        0      658 1970-01-01 00:00:00.000000 osim_utils-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0      232 2023-05-03 10:56:19.733098 osim_utils-0.6.0/README.md
+-rw-r--r--   0        0        0     1446 2023-05-08 15:34:27.529473 osim_utils-0.6.0/osim_utils/clients/crossref.py
+-rw-r--r--   0        0        0     1737 2023-06-14 09:36:56.204537 osim_utils-0.6.0/osim_utils/clients/embl_data_warehouse.py
+-rw-r--r--   0        0        0     5470 2023-06-07 12:38:09.089910 osim_utils-0.6.0/osim_utils/clients/epmc.py
+-rw-r--r--   0        0        0     4903 2023-06-28 15:50:58.664838 osim_utils-0.6.0/osim_utils/clients/openalex.py
+-rw-r--r--   0        0        0      717 2023-07-12 14:43:33.136096 osim_utils-0.6.0/osim_utils/clients/ror.py
+-rw-r--r--   0        0        0     2539 2023-06-07 09:08:46.139525 osim_utils-0.6.0/osim_utils/clients/sherpa.py
+-rw-r--r--   0        0        0      271 2023-05-03 13:04:39.071567 osim_utils-0.6.0/osim_utils/common.py
+-rw-r--r--   0        0        0      311 2023-05-03 13:04:39.071765 osim_utils-0.6.0/osim_utils/constants.py
+-rw-r--r--   0        0        0     1497 2023-06-07 12:38:09.090134 osim_utils-0.6.0/osim_utils/decorators.py
+-rw-r--r--   0        0        0      769 2023-06-07 12:38:09.090340 osim_utils-0.6.0/osim_utils/exceptions.py
+-rw-r--r--   0        0        0     2532 2023-01-12 14:22:33.188019 osim_utils-0.6.0/osim_utils/logger.py
+-rw-r--r--   0        0        0      408 2023-07-12 14:46:00.090278 osim_utils-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0      658 1970-01-01 00:00:00.000000 osim_utils-0.6.0/PKG-INFO
```

### Comparing `osim_utils-0.5.0/osim_utils/clients/crossref.py` & `osim_utils-0.6.0/osim_utils/clients/crossref.py`

 * *Files identical despite different names*

### Comparing `osim_utils-0.5.0/osim_utils/clients/embl_data_warehouse.py` & `osim_utils-0.6.0/osim_utils/clients/embl_data_warehouse.py`

 * *Files 10% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     def _get_all_pubs(self, **kwargs):
         headers = self.default_headers | kwargs.get("headers", dict())
         return self.session.get(self.base_url, headers=headers, params={"all": "true"})
 
     def get_all_publications(self, **kwargs):
         r = self._get_all_pubs(**kwargs)
         unique_pubs = list()
-        processed_dois = list()
+        processed_pubs = list()
         for owner in r:
             pubs = owner["publications"]
             for k, v in pubs.items():
-                if (doi := v["DOI"]) not in processed_dois:
-                    processed_dois.append(doi)
+                if (pub_id := v["id"]) not in processed_pubs:
+                    processed_pubs.append(pub_id)
                     unique_pubs.append(v)
         return unique_pubs
```

### Comparing `osim_utils-0.5.0/osim_utils/clients/epmc.py` & `osim_utils-0.6.0/osim_utils/clients/epmc.py`

 * *Files identical despite different names*

### Comparing `osim_utils-0.5.0/osim_utils/clients/openalex.py` & `osim_utils-0.6.0/osim_utils/clients/openalex.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import os
 import requests
 import urllib.parse
 from http import HTTPStatus
+from typing import Optional
 
 from osim_utils.logger import get_logger
 from osim_utils.constants import ror_id2site
 from osim_utils.decorators import check_response, process_response
 from osim_utils.common import chunk_list
 
 
@@ -106,7 +107,29 @@
             r = self.get_embl_works(filters=filters, params=params)
             results += r["results"]
             cursor = r["meta"]["next_cursor"]
         return {
             "meta": r["meta"],
             "results": results,
         }
+
+    def get_works_by_orcids(
+        self, orcids: list[str], filters: Optional[dict] = None, **kwargs
+    ) -> dict:
+        cursor = "*"
+        filter_str = f"author.orcid:{'|'.join(orcids)}"
+        if filters:
+            for k, v in filters.items():
+                filter_str += f",{k}:{v}"
+        params = (
+            {"filter": filter_str} | {"per-page": 200} | kwargs.pop("params", dict())
+        )
+        results = list()
+        while cursor:
+            params.update(cursor=cursor)
+            r = self.get(self.works_endpoint, params=params, **kwargs)
+            results += r["results"]
+            cursor = r["meta"]["next_cursor"]
+        return {
+            "meta": r["meta"],
+            "results": results,
+        }
```

### Comparing `osim_utils-0.5.0/osim_utils/clients/sherpa.py` & `osim_utils-0.6.0/osim_utils/clients/sherpa.py`

 * *Files identical despite different names*

### Comparing `osim_utils-0.5.0/osim_utils/decorators.py` & `osim_utils-0.6.0/osim_utils/decorators.py`

 * *Files identical despite different names*

### Comparing `osim_utils-0.5.0/osim_utils/exceptions.py` & `osim_utils-0.6.0/osim_utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `osim_utils-0.5.0/osim_utils/logger.py` & `osim_utils-0.6.0/osim_utils/logger.py`

 * *Files identical despite different names*

### Comparing `osim_utils-0.5.0/PKG-INFO` & `osim_utils-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osim-utils
-Version: 0.5.0
+Version: 0.6.0
 Summary: 
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

