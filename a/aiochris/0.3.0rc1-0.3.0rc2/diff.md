# Comparing `tmp/aiochris-0.3.0rc1.tar.gz` & `tmp/aiochris-0.3.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiochris-0.3.0rc1.tar", max compression
+gzip compressed data, was "aiochris-0.3.0rc2.tar", max compression
```

## Comparing `aiochris-0.3.0rc1.tar` & `aiochris-0.3.0rc2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0     1069 2023-07-12 19:47:55.140414 aiochris-0.3.0rc1/LICENSE
--rw-r--r--   0        0        0     1738 2023-07-12 19:47:55.140414 aiochris-0.3.0rc1/README.md
--rw-r--r--   0        0        0      594 2023-07-12 19:47:55.140414 aiochris-0.3.0rc1/aiochris/__init__.py
--rw-r--r--   0        0        0        0 2023-07-12 19:47:55.140414 aiochris-0.3.0rc1/aiochris/client/__init__.py
--rw-r--r--   0        0        0     6161 2023-07-12 19:47:55.140414 aiochris-0.3.0rc1/aiochris/client/admin.py
--rw-r--r--   0        0        0     1335 2023-07-12 19:47:55.140414 aiochris-0.3.0rc1/aiochris/client/anon.py
--rw-r--r--   0        0        0     9615 2023-07-12 19:47:55.140414 aiochris-0.3.0rc1/aiochris/client/authed.py
--rw-r--r--   0        0        0     3718 2023-07-12 19:47:55.140414 aiochris-0.3.0rc1/aiochris/client/base.py
--rw-r--r--   0        0        0     1695 2023-07-12 19:47:55.140414 aiochris-0.3.0rc1/aiochris/client/normal.py
--rw-r--r--   0        0        0      644 2023-07-12 19:47:55.140414 aiochris-0.3.0rc1/aiochris/enums.py
--rw-r--r--   0        0        0      698 2023-07-12 19:47:55.140414 aiochris-0.3.0rc1/aiochris/errors.py
--rw-r--r--   0        0        0     2284 2023-07-12 19:47:55.140414 aiochris-0.3.0rc1/aiochris/examples.md
--rw-r--r--   0        0        0     4811 2023-07-12 19:47:55.140414 aiochris-0.3.0rc1/aiochris/home.md
--rw-r--r--   0        0        0       97 2023-07-12 19:47:55.140414 aiochris-0.3.0rc1/aiochris/link/__init__.py
--rw-r--r--   0        0        0     1143 2023-07-12 19:47:55.140414 aiochris-0.3.0rc1/aiochris/link/collection_client.py
--rw-r--r--   0        0        0     4969 2023-07-12 19:47:55.140414 aiochris-0.3.0rc1/aiochris/link/http.py
--rw-r--r--   0        0        0     4659 2023-07-12 19:47:55.140414 aiochris-0.3.0rc1/aiochris/link/linked.py
--rw-r--r--   0        0        0     1450 2023-07-12 19:47:55.140414 aiochris-0.3.0rc1/aiochris/link/metaprog.py
--rw-r--r--   0        0        0        0 2023-07-12 19:47:55.140414 aiochris-0.3.0rc1/aiochris/models/__init__.py
--rw-r--r--   0        0        0     1631 2023-07-12 19:47:55.140414 aiochris-0.3.0rc1/aiochris/models/collection_links.py
--rw-r--r--   0        0        0     2898 2023-07-12 19:47:55.140414 aiochris-0.3.0rc1/aiochris/models/data.py
--rw-r--r--   0        0        0     5047 2023-07-12 19:47:55.140414 aiochris-0.3.0rc1/aiochris/models/logged_in.py
--rw-r--r--   0        0        0     1114 2023-07-12 19:47:55.140414 aiochris-0.3.0rc1/aiochris/models/public.py
--rw-r--r--   0        0        0     3118 2023-07-12 19:47:55.140414 aiochris-0.3.0rc1/aiochris/types.py
--rw-r--r--   0        0        0       31 2023-07-12 19:47:55.140414 aiochris-0.3.0rc1/aiochris/util/__init__.py
--rw-r--r--   0        0        0     6900 2023-07-12 19:47:55.140414 aiochris-0.3.0rc1/aiochris/util/search.py
--rw-r--r--   0        0        0      785 2023-07-12 19:47:55.140414 aiochris-0.3.0rc1/pyproject.toml
--rw-r--r--   0        0        0     2364 1970-01-01 00:00:00.000000 aiochris-0.3.0rc1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-07-12 21:45:17.766044 aiochris-0.3.0rc2/LICENSE
+-rw-r--r--   0        0        0     1738 2023-07-12 21:45:17.766044 aiochris-0.3.0rc2/README.md
+-rw-r--r--   0        0        0      594 2023-07-12 21:45:17.766044 aiochris-0.3.0rc2/aiochris/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-12 21:45:17.766044 aiochris-0.3.0rc2/aiochris/client/__init__.py
+-rw-r--r--   0        0        0     6161 2023-07-12 21:45:17.766044 aiochris-0.3.0rc2/aiochris/client/admin.py
+-rw-r--r--   0        0        0     1335 2023-07-12 21:45:17.766044 aiochris-0.3.0rc2/aiochris/client/anon.py
+-rw-r--r--   0        0        0     9615 2023-07-12 21:45:17.766044 aiochris-0.3.0rc2/aiochris/client/authed.py
+-rw-r--r--   0        0        0     3718 2023-07-12 21:45:17.766044 aiochris-0.3.0rc2/aiochris/client/base.py
+-rw-r--r--   0        0        0     1695 2023-07-12 21:45:17.766044 aiochris-0.3.0rc2/aiochris/client/normal.py
+-rw-r--r--   0        0        0      644 2023-07-12 21:45:17.766044 aiochris-0.3.0rc2/aiochris/enums.py
+-rw-r--r--   0        0        0      698 2023-07-12 21:45:17.766044 aiochris-0.3.0rc2/aiochris/errors.py
+-rw-r--r--   0        0        0     2284 2023-07-12 21:45:17.766044 aiochris-0.3.0rc2/aiochris/examples.md
+-rw-r--r--   0        0        0     4811 2023-07-12 21:45:17.766044 aiochris-0.3.0rc2/aiochris/home.md
+-rw-r--r--   0        0        0       97 2023-07-12 21:45:17.766044 aiochris-0.3.0rc2/aiochris/link/__init__.py
+-rw-r--r--   0        0        0     1143 2023-07-12 21:45:17.766044 aiochris-0.3.0rc2/aiochris/link/collection_client.py
+-rw-r--r--   0        0        0     5027 2023-07-12 21:45:17.766044 aiochris-0.3.0rc2/aiochris/link/http.py
+-rw-r--r--   0        0        0     4659 2023-07-12 21:45:17.766044 aiochris-0.3.0rc2/aiochris/link/linked.py
+-rw-r--r--   0        0        0     1450 2023-07-12 21:45:17.766044 aiochris-0.3.0rc2/aiochris/link/metaprog.py
+-rw-r--r--   0        0        0        0 2023-07-12 21:45:17.766044 aiochris-0.3.0rc2/aiochris/models/__init__.py
+-rw-r--r--   0        0        0     1631 2023-07-12 21:45:17.766044 aiochris-0.3.0rc2/aiochris/models/collection_links.py
+-rw-r--r--   0        0        0     2898 2023-07-12 21:45:17.766044 aiochris-0.3.0rc2/aiochris/models/data.py
+-rw-r--r--   0        0        0     5047 2023-07-12 21:45:17.766044 aiochris-0.3.0rc2/aiochris/models/logged_in.py
+-rw-r--r--   0        0        0     1129 2023-07-12 21:45:17.766044 aiochris-0.3.0rc2/aiochris/models/public.py
+-rw-r--r--   0        0        0     3118 2023-07-12 21:45:17.766044 aiochris-0.3.0rc2/aiochris/types.py
+-rw-r--r--   0        0        0       31 2023-07-12 21:45:17.766044 aiochris-0.3.0rc2/aiochris/util/__init__.py
+-rw-r--r--   0        0        0     6932 2023-07-12 21:45:17.766044 aiochris-0.3.0rc2/aiochris/util/search.py
+-rw-r--r--   0        0        0      785 2023-07-12 21:45:17.766044 aiochris-0.3.0rc2/pyproject.toml
+-rw-r--r--   0        0        0     2364 1970-01-01 00:00:00.000000 aiochris-0.3.0rc2/PKG-INFO
```

### Comparing `aiochris-0.3.0rc1/LICENSE` & `aiochris-0.3.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `aiochris-0.3.0rc1/README.md` & `aiochris-0.3.0rc2/README.md`

 * *Files identical despite different names*

### Comparing `aiochris-0.3.0rc1/aiochris/__init__.py` & `aiochris-0.3.0rc2/aiochris/__init__.py`

 * *Files identical despite different names*

### Comparing `aiochris-0.3.0rc1/aiochris/client/admin.py` & `aiochris-0.3.0rc2/aiochris/client/admin.py`

 * *Files identical despite different names*

### Comparing `aiochris-0.3.0rc1/aiochris/client/anon.py` & `aiochris-0.3.0rc2/aiochris/client/anon.py`

 * *Files identical despite different names*

### Comparing `aiochris-0.3.0rc1/aiochris/client/authed.py` & `aiochris-0.3.0rc2/aiochris/client/authed.py`

 * *Files identical despite different names*

### Comparing `aiochris-0.3.0rc1/aiochris/client/base.py` & `aiochris-0.3.0rc2/aiochris/client/base.py`

 * *Files identical despite different names*

### Comparing `aiochris-0.3.0rc1/aiochris/client/normal.py` & `aiochris-0.3.0rc2/aiochris/client/normal.py`

 * *Files identical despite different names*

### Comparing `aiochris-0.3.0rc1/aiochris/enums.py` & `aiochris-0.3.0rc2/aiochris/enums.py`

 * *Files identical despite different names*

### Comparing `aiochris-0.3.0rc1/aiochris/errors.py` & `aiochris-0.3.0rc2/aiochris/errors.py`

 * *Files identical despite different names*

### Comparing `aiochris-0.3.0rc1/aiochris/examples.md` & `aiochris-0.3.0rc2/aiochris/examples.md`

 * *Files identical despite different names*

### Comparing `aiochris-0.3.0rc1/aiochris/home.md` & `aiochris-0.3.0rc2/aiochris/home.md`

 * *Files identical despite different names*

### Comparing `aiochris-0.3.0rc1/aiochris/link/collection_client.py` & `aiochris-0.3.0rc2/aiochris/link/collection_client.py`

 * *Files identical despite different names*

### Comparing `aiochris-0.3.0rc1/aiochris/link/http.py` & `aiochris-0.3.0rc2/aiochris/link/http.py`

 * *Files 2% similar despite different names*

```diff
@@ -120,15 +120,15 @@
         LinkedMeta.mark_to_check(wrapped, link_name)
         return wrapped
 
     return decorator
 
 
 def search(
-    collection_name: str,
+    collection_name: str, subpath: str = "search/"
 ) -> Callable[[Callable[..., Search[_R]]], Callable[..., Search[_R]]]:
     """
     Creates a decorator which searches the collection using GET requests.
 
     (Pagination is handled internally, HTTP requests are made as-needed.)
     """
 
@@ -141,14 +141,15 @@
 
             return Search[return_item_type](
                 Item=return_item_type,
                 client=self,
                 base_url=self._get_link(collection_name),
                 params=kwargs,
                 max_requests=self.max_search_requests,
+                subpath=subpath,
             )
 
         LinkedMeta.mark_to_check(wrapped, collection_name)
         return wrapped
 
     return decorator
```

### Comparing `aiochris-0.3.0rc1/aiochris/link/linked.py` & `aiochris-0.3.0rc2/aiochris/link/linked.py`

 * *Files identical despite different names*

### Comparing `aiochris-0.3.0rc1/aiochris/link/metaprog.py` & `aiochris-0.3.0rc2/aiochris/link/metaprog.py`

 * *Files identical despite different names*

### Comparing `aiochris-0.3.0rc1/aiochris/models/collection_links.py` & `aiochris-0.3.0rc2/aiochris/models/collection_links.py`

 * *Files identical despite different names*

### Comparing `aiochris-0.3.0rc1/aiochris/models/data.py` & `aiochris-0.3.0rc2/aiochris/models/data.py`

 * *Files identical despite different names*

### Comparing `aiochris-0.3.0rc1/aiochris/models/logged_in.py` & `aiochris-0.3.0rc2/aiochris/models/logged_in.py`

 * *Files identical despite different names*

### Comparing `aiochris-0.3.0rc1/aiochris/models/public.py` & `aiochris-0.3.0rc2/aiochris/models/public.py`

 * *Files 7% similar despite different names*

```diff
@@ -39,11 +39,11 @@
     name: PluginName
     version: PluginVersion
     dock_image: ImageTag
     public_repo: str
     compute_resources: ComputeResourceUrl
     plugin_type: PluginType = serde.field(rename="type")
 
-    @http.get("compute_resources")
+    @http.search("compute_resources", subpath="")
     def get_compute_resources(self) -> Search[ComputeResource]:
         """Get the compute resources this plugin is registered to."""
         ...
```

### Comparing `aiochris-0.3.0rc1/aiochris/types.py` & `aiochris-0.3.0rc2/aiochris/types.py`

 * *Files identical despite different names*

### Comparing `aiochris-0.3.0rc1/aiochris/util/search.py` & `aiochris-0.3.0rc2/aiochris/util/search.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,14 +66,15 @@
     """
 
     base_url: str
     params: dict[str, Any]
     client: Linked
     Item: Type[T]
     max_requests: int = 100
+    subpath: str = "search/"
 
     def __aiter__(self) -> AsyncIterator[T]:
         return self._paginate(self.url)
 
     async def first(self) -> Optional[T]:
         """
         Get the first item.
@@ -164,15 +165,15 @@
         params = copy.copy(self.params)
         params["limit"] = 1
         params["offset"] = 0
         return self._search_url_with(params)
 
     @property
     def _search_url(self) -> yarl.URL:
-        return yarl.URL(self.base_url) / "search/"
+        return yarl.URL(self.base_url) / self.subpath
 
     def _search_url_with(self, query: dict[str, Any]):
         return yarl.URL(self._search_url).with_query(query)
 
 
 async def _get_paginated(
     client: Linked,
```

### Comparing `aiochris-0.3.0rc1/pyproject.toml` & `aiochris-0.3.0rc2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aiochris"
-version = "0.3.0rc1"
+version = "0.3.0rc2"
 description = "ChRIS client built on aiohttp"
 authors = ["FNNDSC <dev@babyMRI.org>"]
 readme = "README.md"
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `aiochris-0.3.0rc1/PKG-INFO` & `aiochris-0.3.0rc2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiochris
-Version: 0.3.0rc1
+Version: 0.3.0rc2
 Summary: ChRIS client built on aiohttp
 License: MIT
 Author: FNNDSC
 Author-email: dev@babyMRI.org
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

