# Comparing `tmp/pyPreservica-2.0.4.tar.gz` & `tmp/pyPreservica-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyPreservica-2.0.4.tar", last modified: Thu Jul 13 09:22:04 2023, max compression
+gzip compressed data, was "pyPreservica-2.0.5.tar", last modified: Thu Jul 13 17:40:05 2023, max compression
```

## Comparing `pyPreservica-2.0.4.tar` & `pyPreservica-2.0.5.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-07-13 09:22:04.914955 pyPreservica-2.0.4/
--rw-rw-rw-   0        0        0    11558 2020-08-17 10:38:19.000000 pyPreservica-2.0.4/LICENSE.txt
--rw-rw-rw-   0        0        0     2581 2023-07-13 09:22:04.914955 pyPreservica-2.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     1602 2022-03-16 17:04:00.000000 pyPreservica-2.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-07-13 09:22:04.868092 pyPreservica-2.0.4/pyPreservica/
--rw-rw-rw-   0        0        0     1085 2023-07-13 09:21:50.000000 pyPreservica-2.0.4/pyPreservica/__init__.py
--rw-rw-rw-   0        0        0    37810 2023-07-13 09:10:01.000000 pyPreservica-2.0.4/pyPreservica/adminAPI.py
--rw-rw-rw-   0        0        0     9142 2023-07-04 08:59:07.000000 pyPreservica-2.0.4/pyPreservica/authorityAPI.py
--rw-rw-rw-   0        0        0    34848 2023-07-03 10:50:28.000000 pyPreservica-2.0.4/pyPreservica/common.py
--rw-rw-rw-   0        0        0    16257 2023-05-24 17:32:04.000000 pyPreservica-2.0.4/pyPreservica/contentAPI.py
--rw-rw-rw-   0        0        0   105749 2023-07-05 09:27:42.000000 pyPreservica-2.0.4/pyPreservica/entityAPI.py
--rw-rw-rw-   0        0        0     6258 2023-05-16 11:37:54.000000 pyPreservica-2.0.4/pyPreservica/monitorAPI.py
--rw-rw-rw-   0        0        0     4875 2022-04-21 08:22:10.000000 pyPreservica-2.0.4/pyPreservica/opex.py
--rw-rw-rw-   0        0        0    10522 2021-11-17 14:16:50.000000 pyPreservica-2.0.4/pyPreservica/parAPI.py
--rw-rw-rw-   0        0        0    23612 2023-05-24 17:32:04.000000 pyPreservica-2.0.4/pyPreservica/retentionAPI.py
--rw-rw-rw-   0        0        0    92455 2023-06-06 12:57:35.000000 pyPreservica-2.0.4/pyPreservica/uploadAPI.py
--rw-rw-rw-   0        0        0     6736 2023-05-24 08:15:02.000000 pyPreservica-2.0.4/pyPreservica/webHooksAPI.py
--rw-rw-rw-   0        0        0    17862 2023-05-24 17:32:04.000000 pyPreservica-2.0.4/pyPreservica/workflowAPI.py
-drwxrwxrwx   0        0        0        0 2023-07-13 09:22:04.914955 pyPreservica-2.0.4/pyPreservica.egg-info/
--rw-rw-rw-   0        0        0     2581 2023-07-13 09:22:03.000000 pyPreservica-2.0.4/pyPreservica.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      546 2023-07-13 09:22:04.000000 pyPreservica-2.0.4/pyPreservica.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-13 09:22:03.000000 pyPreservica-2.0.4/pyPreservica.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       73 2023-07-13 09:22:03.000000 pyPreservica-2.0.4/pyPreservica.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-07-13 09:22:03.000000 pyPreservica-2.0.4/pyPreservica.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-13 09:22:04.930575 pyPreservica-2.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1654 2023-07-13 09:21:50.000000 pyPreservica-2.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-13 17:40:05.771385 pyPreservica-2.0.5/
+-rw-rw-rw-   0        0        0    11558 2020-08-17 10:38:19.000000 pyPreservica-2.0.5/LICENSE.txt
+-rw-rw-rw-   0        0        0     2581 2023-07-13 17:40:05.771385 pyPreservica-2.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1602 2022-03-16 17:04:00.000000 pyPreservica-2.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-07-13 17:40:05.718011 pyPreservica-2.0.5/pyPreservica/
+-rw-rw-rw-   0        0        0     1085 2023-07-13 17:36:18.000000 pyPreservica-2.0.5/pyPreservica/__init__.py
+-rw-rw-rw-   0        0        0    37810 2023-07-13 09:10:01.000000 pyPreservica-2.0.5/pyPreservica/adminAPI.py
+-rw-rw-rw-   0        0        0     9142 2023-07-04 08:59:07.000000 pyPreservica-2.0.5/pyPreservica/authorityAPI.py
+-rw-rw-rw-   0        0        0    34848 2023-07-03 10:50:28.000000 pyPreservica-2.0.5/pyPreservica/common.py
+-rw-rw-rw-   0        0        0    17206 2023-07-13 17:36:18.000000 pyPreservica-2.0.5/pyPreservica/contentAPI.py
+-rw-rw-rw-   0        0        0   105749 2023-07-05 09:27:42.000000 pyPreservica-2.0.5/pyPreservica/entityAPI.py
+-rw-rw-rw-   0        0        0     6258 2023-05-16 11:37:54.000000 pyPreservica-2.0.5/pyPreservica/monitorAPI.py
+-rw-rw-rw-   0        0        0     4875 2022-04-21 08:22:10.000000 pyPreservica-2.0.5/pyPreservica/opex.py
+-rw-rw-rw-   0        0        0    10522 2021-11-17 14:16:50.000000 pyPreservica-2.0.5/pyPreservica/parAPI.py
+-rw-rw-rw-   0        0        0    23612 2023-05-24 17:32:04.000000 pyPreservica-2.0.5/pyPreservica/retentionAPI.py
+-rw-rw-rw-   0        0        0    92455 2023-06-06 12:57:35.000000 pyPreservica-2.0.5/pyPreservica/uploadAPI.py
+-rw-rw-rw-   0        0        0     6736 2023-05-24 08:15:02.000000 pyPreservica-2.0.5/pyPreservica/webHooksAPI.py
+-rw-rw-rw-   0        0        0    17862 2023-05-24 17:32:04.000000 pyPreservica-2.0.5/pyPreservica/workflowAPI.py
+drwxrwxrwx   0        0        0        0 2023-07-13 17:40:05.755790 pyPreservica-2.0.5/pyPreservica.egg-info/
+-rw-rw-rw-   0        0        0     2581 2023-07-13 17:40:03.000000 pyPreservica-2.0.5/pyPreservica.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      546 2023-07-13 17:40:03.000000 pyPreservica-2.0.5/pyPreservica.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-13 17:40:03.000000 pyPreservica-2.0.5/pyPreservica.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       73 2023-07-13 17:40:03.000000 pyPreservica-2.0.5/pyPreservica.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-07-13 17:40:03.000000 pyPreservica-2.0.5/pyPreservica.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-13 17:40:05.771385 pyPreservica-2.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1654 2023-07-13 17:36:18.000000 pyPreservica-2.0.5/setup.py
```

### Comparing `pyPreservica-2.0.4/LICENSE.txt` & `pyPreservica-2.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyPreservica-2.0.4/PKG-INFO` & `pyPreservica-2.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyPreservica
-Version: 2.0.4
+Version: 2.0.5
 Summary: Python library for the Preservica API
 Home-page: https://pypreservica.readthedocs.io/
 Author: James Carr
 Author-email: drjamescarr@gmail.com
 License: Apache License 2.0
 Project-URL: Documentation, https://pypreservica.readthedocs.io
 Project-URL: Source, https://github.com/carj/pyPreservica
```

### Comparing `pyPreservica-2.0.4/README.md` & `pyPreservica-2.0.5/README.md`

 * *Files identical despite different names*

### Comparing `pyPreservica-2.0.4/pyPreservica/__init__.py` & `pyPreservica-2.0.5/pyPreservica/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,10 +19,10 @@
 from .webHooksAPI import WebHooksAPI, TriggerType, WebHookHandler
 from .authorityAPI import AuthorityAPI, Table
 
 
 __author__ = "James Carr (drjamescarr@gmail.com)"
 
 # Version of the Preservica API package
-__version__ = "2.0.4"
+__version__ = "2.0.5"
 
 __license__ = "Apache License Version 2.0"
```

### Comparing `pyPreservica-2.0.4/pyPreservica/adminAPI.py` & `pyPreservica-2.0.5/pyPreservica/adminAPI.py`

 * *Files identical despite different names*

### Comparing `pyPreservica-2.0.4/pyPreservica/authorityAPI.py` & `pyPreservica-2.0.5/pyPreservica/authorityAPI.py`

 * *Files identical despite different names*

### Comparing `pyPreservica-2.0.4/pyPreservica/common.py` & `pyPreservica-2.0.5/pyPreservica/common.py`

 * *Files identical despite different names*

### Comparing `pyPreservica-2.0.4/pyPreservica/contentAPI.py` & `pyPreservica-2.0.5/pyPreservica/contentAPI.py`

 * *Files 15% similar despite different names*

```diff
@@ -52,15 +52,16 @@
         :return: Dictionary of object attributes
         """
         headers = {HEADER_TOKEN: self.token, 'Content-Type': 'application/json'}
         if type(entity_type) == EntityType:
             params = {'id': f'sdb:{entity_type.value}|{reference}'}
         else:
             params = {'id': f'sdb:{entity_type}|{reference}'}
-        request = self.session.get(f'{self.protocol}://{self.server}/api/content/object-details', params=params, headers=headers)
+        request = self.session.get(f'{self.protocol}://{self.server}/api/content/object-details', params=params,
+                                   headers=headers)
         if request.status_code == requests.codes.ok:
             return request.json()["value"]
         elif request.status_code == requests.codes.not_found:
             logger.error(f"The requested reference is not found in the repository: {reference}")
             raise RuntimeError(reference, "The requested reference is not found in the repository")
         elif request.status_code == requests.codes.unauthorized:
             self.token = self.__token__()
@@ -159,15 +160,16 @@
         headers = {'Content-Type': 'application/x-www-form-urlencoded', HEADER_TOKEN: self.token}
         query_term = ('{ "q":  "%s" }' % query)
         if list_indexes is None or len(list_indexes) == 0:
             metadata_fields = "xip.title,xip.description,xip.document_type,xip.parent_ref,xip.security_descriptor"
         else:
             metadata_fields = ','.join(list_indexes)
         payload = {'start': start_from, 'max': str(page_size), 'metadata': metadata_fields, 'q': query_term}
-        results = self.session.post(f'{self.protocol}://{self.server}/api/content/search', data=payload, headers=headers)
+        results = self.session.post(f'{self.protocol}://{self.server}/api/content/search', data=payload,
+                                    headers=headers)
         results_list = []
         if results.status_code == requests.codes.ok:
             json_doc = results.json()
             metadata = json_doc['value']['metadata']
             refs = list(json_doc['value']['objectIds'])
             refs = list(map(lambda x: content_api_identifier_to_type(x), refs))
             hits = int(json_doc['value']['totalHits'])
@@ -188,44 +190,47 @@
         elif results.status_code == requests.codes.unauthorized:
             self.token = self.__token__()
             return self._simple_search(query, start_index, page_size, list_indexes)
         else:
             logger.error(f"search failed with error code: {results.status_code}")
             raise RuntimeError(results.status_code, f"simple_search failed with error code: {results.status_code}")
 
-    def search_index_filter_csv(self, query: str = "%", csv_file="search.csv", filter_values: dict = None):
+    def search_index_filter_csv(self, query: str = "%", csv_file="search.csv", filter_values: dict = None,
+                                sort_values: dict = None):
         page_size = 50
         if filter_values is None:
             filter_values = {}
         if "xip.reference" not in filter_values:
             filter_values["xip.reference"] = ""
 
         header_fields = list(filter_values.keys())
         index = header_fields.index("xip.reference")
         header_fields.insert(0, header_fields.pop(index))
         with open(csv_file, newline='', mode="wt", encoding="utf-8") as csv_file:
             writer = csv.DictWriter(csv_file, fieldnames=header_fields)
             writer.writeheader()
-            writer.writerows(self.search_index_filter_list(query, page_size, filter_values))
+            writer.writerows(self.search_index_filter_list(query, page_size, filter_values, sort_values))
 
-    def search_index_filter_list(self, query: str = "%", page_size: int = 25, filter_values: dict = None) -> Generator:
+    def search_index_filter_list(self, query: str = "%", page_size: int = 25, filter_values: dict = None,
+                                 sort_values: dict = None) -> Generator:
         """
         Run a search query with optional filters
 
         :param query: The main search query.
         :param page_size:  The default search page size
         :param filter_values:  Dictionary of index names and values
+        :param sort_values:    Dictionary of sort index names and values
         :return: search result
         """
-        search_result = self._search_index_filter(query, 0, page_size, filter_values)
+        search_result = self._search_index_filter(query, 0, page_size, filter_values, sort_values)
         for e in search_result.results_list:
             yield e
         found = len(search_result.results_list)
         while search_result.hits > found:
-            search_result = self._search_index_filter(query, found, page_size, filter_values)
+            search_result = self._search_index_filter(query, found, page_size, filter_values, sort_values)
             for e in search_result.results_list:
                 yield e
             found = found + len(search_result.results_list)
 
     def search_index_filter_hits(self, query: str = "%", filter_values: dict = None) -> int:
         """
         Run a search query with filters and return the number of hits only
@@ -245,44 +250,57 @@
                 field_list.append('{' f' "name": "{key}", "values": ["{value}"] ' + '}')
 
         filter_terms = ','.join(field_list)
 
         query_term = ('{ "q":  "%s",  "fields":  [ %s ] }' % (query, filter_terms))
 
         payload = {'start': start_from, 'max': str(10), 'metadata': list(filter_values.keys()), 'q': query_term}
-        results = self.session.post(f'{self.protocol}://{self.server}/api/content/search', data=payload, headers=headers)
+        results = self.session.post(f'{self.protocol}://{self.server}/api/content/search', data=payload,
+                                    headers=headers)
         if results.status_code == requests.codes.ok:
             json_doc = results.json()
             return int(json_doc['value']['totalHits'])
         elif results.status_code == requests.codes.unauthorized:
             self.token = self.__token__()
             return self.search_index_filter_hits(query, filter_values)
         else:
             logger.error(f"search failed with error code: {results.status_code}")
             raise RuntimeError(results.status_code, f"_search_index_filter_hits failed")
 
     def _search_index_filter(self, query: str = "%", start_index: int = 0, page_size: int = 25,
-                             filter_values: dict = None):
+                             filter_values: dict = None, sort_values: dict = None):
         start_from = str(start_index)
         headers = {'Content-Type': 'application/x-www-form-urlencoded', HEADER_TOKEN: self.token}
 
         field_list = []
         for key, value in filter_values.items():
             if value == "":
                 field_list.append('{' f' "name": "{key}", "values": [] ' + '}')
             else:
                 field_list.append('{' f' "name": "{key}", "values": ["{value}"] ' + '}')
 
         filter_terms = ','.join(field_list)
 
-        query_term = ('{ "q":  "%s",  "fields":  [ %s ] }' % (query, filter_terms))
+        if sort_values is None:
+            query_term = ('{ "q":  "%s",  "fields":  [ %s ] }' % (query, filter_terms))
+        else:
+            sort_list = []
+            for key, value in sort_values.items():
+                direction = "asc"
+                if str(value).lower().startswith("d"):
+                    direction = "desc"
+                sort_list.append(f'{{"sortFields": ["{key}"], "sortOrder": "{direction}"}}')
+            sort_terms = ','.join(sort_list)
+            query_term = ('{ "q":  "%s",  "fields":  [ %s ],  "sort": [ %s ]}' % (query, filter_terms, sort_terms))
 
         payload = {'start': start_from, 'max': str(page_size), 'metadata': list(filter_values.keys()), 'q': query_term}
+        print(payload)
         logger.debug(payload)
-        results = self.session.post(f'{self.protocol}://{self.server}/api/content/search', data=payload, headers=headers)
+        results = self.session.post(f'{self.protocol}://{self.server}/api/content/search', data=payload,
+                                    headers=headers)
         results_list = []
         if results.status_code == requests.codes.ok:
             json_doc = results.json()
             metadata = json_doc['value']['metadata']
             refs = list(json_doc['value']['objectIds'])
             refs = list(map(lambda x: content_api_identifier_to_type(x), refs))
             hits = int(json_doc['value']['totalHits'])
```

### Comparing `pyPreservica-2.0.4/pyPreservica/entityAPI.py` & `pyPreservica-2.0.5/pyPreservica/entityAPI.py`

 * *Files identical despite different names*

### Comparing `pyPreservica-2.0.4/pyPreservica/monitorAPI.py` & `pyPreservica-2.0.5/pyPreservica/monitorAPI.py`

 * *Files identical despite different names*

### Comparing `pyPreservica-2.0.4/pyPreservica/opex.py` & `pyPreservica-2.0.5/pyPreservica/opex.py`

 * *Files identical despite different names*

### Comparing `pyPreservica-2.0.4/pyPreservica/parAPI.py` & `pyPreservica-2.0.5/pyPreservica/parAPI.py`

 * *Files identical despite different names*

### Comparing `pyPreservica-2.0.4/pyPreservica/retentionAPI.py` & `pyPreservica-2.0.5/pyPreservica/retentionAPI.py`

 * *Files identical despite different names*

### Comparing `pyPreservica-2.0.4/pyPreservica/uploadAPI.py` & `pyPreservica-2.0.5/pyPreservica/uploadAPI.py`

 * *Files identical despite different names*

### Comparing `pyPreservica-2.0.4/pyPreservica/webHooksAPI.py` & `pyPreservica-2.0.5/pyPreservica/webHooksAPI.py`

 * *Files identical despite different names*

### Comparing `pyPreservica-2.0.4/pyPreservica/workflowAPI.py` & `pyPreservica-2.0.5/pyPreservica/workflowAPI.py`

 * *Files identical despite different names*

### Comparing `pyPreservica-2.0.4/pyPreservica.egg-info/PKG-INFO` & `pyPreservica-2.0.5/pyPreservica.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyPreservica
-Version: 2.0.4
+Version: 2.0.5
 Summary: Python library for the Preservica API
 Home-page: https://pypreservica.readthedocs.io/
 Author: James Carr
 Author-email: drjamescarr@gmail.com
 License: Apache License 2.0
 Project-URL: Documentation, https://pypreservica.readthedocs.io
 Project-URL: Source, https://github.com/carj/pyPreservica
```

### Comparing `pyPreservica-2.0.4/pyPreservica.egg-info/SOURCES.txt` & `pyPreservica-2.0.5/pyPreservica.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyPreservica-2.0.4/setup.py` & `pyPreservica-2.0.5/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     os.system('twine upload dist/*')
     sys.exit()
 
 
 # This call to setup() does all the work
 setup(
     name=PKG,
-    version="2.0.4",
+    version="2.0.5",
     description="Python library for the Preservica API",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://pypreservica.readthedocs.io/",
     author="James Carr",
     author_email="drjamescarr@gmail.com",
     license="Apache License 2.0",
```

