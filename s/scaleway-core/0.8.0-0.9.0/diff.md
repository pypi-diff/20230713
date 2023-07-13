# Comparing `tmp/scaleway_core-0.8.0.tar.gz` & `tmp/scaleway_core-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scaleway_core-0.8.0.tar", max compression
+gzip compressed data, was "scaleway_core-0.9.0.tar", max compression
```

## Comparing `scaleway_core-0.8.0.tar` & `scaleway_core-0.9.0.tar`

### file list

```diff
@@ -1,29 +1,28 @@
--rw-r--r--   0        0        0       29 2023-02-23 14:16:51.949723 scaleway_core-0.8.0/README.md
--rw-r--r--   0        0        0     1138 2023-02-23 14:17:16.730234 scaleway_core-0.8.0/pyproject.toml
--rw-r--r--   0        0        0      128 2023-02-23 14:16:51.949723 scaleway_core-0.8.0/scaleway_core/__init__.py
--rw-r--r--   0        0        0     4422 2023-02-23 14:16:51.949723 scaleway_core-0.8.0/scaleway_core/api.py
--rw-r--r--   0        0        0      981 2023-02-23 14:16:51.949723 scaleway_core-0.8.0/scaleway_core/bridge/__init__.py
--rw-r--r--   0        0        0     1468 2023-02-23 14:16:51.949723 scaleway_core-0.8.0/scaleway_core/bridge/money.py
--rw-r--r--   0        0        0      188 2023-02-23 14:16:51.949723 scaleway_core-0.8.0/scaleway_core/bridge/region.py
--rw-r--r--   0        0        0      950 2023-02-23 14:16:51.949723 scaleway_core-0.8.0/scaleway_core/bridge/scwfile.py
--rw-r--r--   0        0        0     1304 2023-02-23 14:16:51.949723 scaleway_core-0.8.0/scaleway_core/bridge/serviceinfo.py
--rw-r--r--   0        0        0     2186 2023-02-23 14:16:51.949723 scaleway_core-0.8.0/scaleway_core/bridge/timeseries.py
--rw-r--r--   0        0        0      392 2023-02-23 14:16:51.949723 scaleway_core-0.8.0/scaleway_core/bridge/zone.py
--rw-r--r--   0        0        0     3669 2023-02-23 14:16:51.949723 scaleway_core-0.8.0/scaleway_core/client.py
--rw-r--r--   0        0        0      670 2023-02-23 14:16:51.949723 scaleway_core-0.8.0/scaleway_core/profile/__init__.py
--rw-r--r--   0        0        0      774 2023-02-23 14:16:51.949723 scaleway_core-0.8.0/scaleway_core/profile/env.py
--rw-r--r--   0        0        0      351 2023-02-23 14:16:51.949723 scaleway_core-0.8.0/scaleway_core/profile/file.py
--rw-r--r--   0        0        0     6312 2023-02-23 14:16:51.949723 scaleway_core-0.8.0/scaleway_core/profile/profile.py
--rw-r--r--   0        0        0        0 2023-02-23 14:16:51.949723 scaleway_core-0.8.0/scaleway_core/py.typed
--rw-r--r--   0        0        0      770 2023-02-23 14:16:51.949723 scaleway_core-0.8.0/scaleway_core/utils/__init__.py
--rw-r--r--   0        0        0     2119 2023-02-23 14:16:51.949723 scaleway_core-0.8.0/scaleway_core/utils/fetch_all_pages.py
--rw-r--r--   0        0        0      600 2023-02-23 14:16:51.949723 scaleway_core-0.8.0/scaleway_core/utils/project_or_organization_id.py
--rw-r--r--   0        0        0    50787 2023-02-23 14:16:51.949723 scaleway_core-0.8.0/scaleway_core/utils/random_name.py
--rw-r--r--   0        0        0     1092 2023-02-23 14:16:51.949723 scaleway_core-0.8.0/scaleway_core/utils/resolve_one_of.py
--rw-r--r--   0        0        0      111 2023-02-23 14:16:51.949723 scaleway_core-0.8.0/scaleway_core/utils/strenum.py
--rw-r--r--   0        0        0      508 2023-02-23 14:16:51.949723 scaleway_core-0.8.0/scaleway_core/utils/validate_path_param.py
--rw-r--r--   0        0        0     3532 2023-02-23 14:16:51.949723 scaleway_core-0.8.0/scaleway_core/utils/waiter.py
--rw-r--r--   0        0        0        0 2023-02-23 14:16:51.949723 scaleway_core-0.8.0/scaleway_core/validations/__init__.py
--rw-r--r--   0        0        0      998 2023-02-23 14:16:51.949723 scaleway_core-0.8.0/scaleway_core/validations/string_validation.py
--rw-r--r--   0        0        0      813 1970-01-01 00:00:00.000000 scaleway_core-0.8.0/setup.py
--rw-r--r--   0        0        0     1343 1970-01-01 00:00:00.000000 scaleway_core-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0       29 2023-03-08 16:40:36.918432 scaleway_core-0.9.0/README.md
+-rw-r--r--   0        0        0     1138 2023-03-08 16:40:56.922549 scaleway_core-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0      128 2023-03-08 16:40:36.918432 scaleway_core-0.9.0/scaleway_core/__init__.py
+-rw-r--r--   0        0        0     4443 2023-03-08 16:40:36.918432 scaleway_core-0.9.0/scaleway_core/api.py
+-rw-r--r--   0        0        0      981 2023-03-08 16:40:36.918432 scaleway_core-0.9.0/scaleway_core/bridge/__init__.py
+-rw-r--r--   0        0        0     1468 2023-03-08 16:40:36.918432 scaleway_core-0.9.0/scaleway_core/bridge/money.py
+-rw-r--r--   0        0        0      188 2023-03-08 16:40:36.918432 scaleway_core-0.9.0/scaleway_core/bridge/region.py
+-rw-r--r--   0        0        0      950 2023-03-08 16:40:36.918432 scaleway_core-0.9.0/scaleway_core/bridge/scwfile.py
+-rw-r--r--   0        0        0     1304 2023-03-08 16:40:36.918432 scaleway_core-0.9.0/scaleway_core/bridge/serviceinfo.py
+-rw-r--r--   0        0        0     2186 2023-03-08 16:40:36.918432 scaleway_core-0.9.0/scaleway_core/bridge/timeseries.py
+-rw-r--r--   0        0        0      444 2023-03-08 16:40:36.918432 scaleway_core-0.9.0/scaleway_core/bridge/zone.py
+-rw-r--r--   0        0        0     3669 2023-03-08 16:40:36.918432 scaleway_core-0.9.0/scaleway_core/client.py
+-rw-r--r--   0        0        0      670 2023-03-08 16:40:36.918432 scaleway_core-0.9.0/scaleway_core/profile/__init__.py
+-rw-r--r--   0        0        0      774 2023-03-08 16:40:36.918432 scaleway_core-0.9.0/scaleway_core/profile/env.py
+-rw-r--r--   0        0        0      351 2023-03-08 16:40:36.918432 scaleway_core-0.9.0/scaleway_core/profile/file.py
+-rw-r--r--   0        0        0     6312 2023-03-08 16:40:36.918432 scaleway_core-0.9.0/scaleway_core/profile/profile.py
+-rw-r--r--   0        0        0        0 2023-03-08 16:40:36.918432 scaleway_core-0.9.0/scaleway_core/py.typed
+-rw-r--r--   0        0        0      770 2023-03-08 16:40:36.918432 scaleway_core-0.9.0/scaleway_core/utils/__init__.py
+-rw-r--r--   0        0        0     2119 2023-03-08 16:40:36.918432 scaleway_core-0.9.0/scaleway_core/utils/fetch_all_pages.py
+-rw-r--r--   0        0        0      600 2023-03-08 16:40:36.918432 scaleway_core-0.9.0/scaleway_core/utils/project_or_organization_id.py
+-rw-r--r--   0        0        0    50787 2023-03-08 16:40:36.918432 scaleway_core-0.9.0/scaleway_core/utils/random_name.py
+-rw-r--r--   0        0        0     1092 2023-03-08 16:40:36.918432 scaleway_core-0.9.0/scaleway_core/utils/resolve_one_of.py
+-rw-r--r--   0        0        0      111 2023-03-08 16:40:36.918432 scaleway_core-0.9.0/scaleway_core/utils/strenum.py
+-rw-r--r--   0        0        0      508 2023-03-08 16:40:36.918432 scaleway_core-0.9.0/scaleway_core/utils/validate_path_param.py
+-rw-r--r--   0        0        0     3532 2023-03-08 16:40:36.918432 scaleway_core-0.9.0/scaleway_core/utils/waiter.py
+-rw-r--r--   0        0        0        0 2023-03-08 16:40:36.918432 scaleway_core-0.9.0/scaleway_core/validations/__init__.py
+-rw-r--r--   0        0        0      998 2023-03-08 16:40:36.918432 scaleway_core-0.9.0/scaleway_core/validations/string_validation.py
+-rw-r--r--   0        0        0     1343 1970-01-01 00:00:00.000000 scaleway_core-0.9.0/PKG-INFO
```

### Comparing `scaleway_core-0.8.0/pyproject.toml` & `scaleway_core-0.9.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "scaleway-core"
-version = "0.8.0"
+version = "0.9.0"
 description = "Scaleway SDK for Python"
 authors = ["Scaleway <opensource@scaleway.com>"]
 license = "BSD"
 readme = "README.md"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Environment :: Console",
```

### Comparing `scaleway_core-0.8.0/scaleway_core/api.py` & `scaleway_core-0.9.0/scaleway_core/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -117,15 +117,15 @@
         params: Params = {},
         headers: Dict[str, str] = {},
         body: Optional[Body] = None,
     ) -> requests.Response:
         additional_headers: Dict[str, str] = {}
 
         method = method.upper()
-        if method == "POST" or method == "PUT":
+        if method == "POST" or method == "PUT" or method == "PATCH":
             additional_headers["Content-Type"] = "application/json; charset=utf-8"
 
             if body is None:
                 body = {}
 
         raw_body = json.dumps(body) if body is not None else None
```

### Comparing `scaleway_core-0.8.0/scaleway_core/bridge/__init__.py` & `scaleway_core-0.9.0/scaleway_core/bridge/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway_core-0.8.0/scaleway_core/bridge/money.py` & `scaleway_core-0.9.0/scaleway_core/bridge/money.py`

 * *Files identical despite different names*

### Comparing `scaleway_core-0.8.0/scaleway_core/bridge/scwfile.py` & `scaleway_core-0.9.0/scaleway_core/bridge/scwfile.py`

 * *Files identical despite different names*

### Comparing `scaleway_core-0.8.0/scaleway_core/bridge/serviceinfo.py` & `scaleway_core-0.9.0/scaleway_core/bridge/serviceinfo.py`

 * *Files identical despite different names*

### Comparing `scaleway_core-0.8.0/scaleway_core/bridge/timeseries.py` & `scaleway_core-0.9.0/scaleway_core/bridge/timeseries.py`

 * *Files identical despite different names*

### Comparing `scaleway_core-0.8.0/scaleway_core/client.py` & `scaleway_core-0.9.0/scaleway_core/client.py`

 * *Files identical despite different names*

### Comparing `scaleway_core-0.8.0/scaleway_core/profile/__init__.py` & `scaleway_core-0.9.0/scaleway_core/profile/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway_core-0.8.0/scaleway_core/profile/env.py` & `scaleway_core-0.9.0/scaleway_core/profile/env.py`

 * *Files identical despite different names*

### Comparing `scaleway_core-0.8.0/scaleway_core/profile/profile.py` & `scaleway_core-0.9.0/scaleway_core/profile/profile.py`

 * *Files identical despite different names*

### Comparing `scaleway_core-0.8.0/scaleway_core/utils/__init__.py` & `scaleway_core-0.9.0/scaleway_core/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway_core-0.8.0/scaleway_core/utils/fetch_all_pages.py` & `scaleway_core-0.9.0/scaleway_core/utils/fetch_all_pages.py`

 * *Files identical despite different names*

### Comparing `scaleway_core-0.8.0/scaleway_core/utils/project_or_organization_id.py` & `scaleway_core-0.9.0/scaleway_core/utils/project_or_organization_id.py`

 * *Files identical despite different names*

### Comparing `scaleway_core-0.8.0/scaleway_core/utils/random_name.py` & `scaleway_core-0.9.0/scaleway_core/utils/random_name.py`

 * *Files identical despite different names*

### Comparing `scaleway_core-0.8.0/scaleway_core/utils/resolve_one_of.py` & `scaleway_core-0.9.0/scaleway_core/utils/resolve_one_of.py`

 * *Files identical despite different names*

### Comparing `scaleway_core-0.8.0/scaleway_core/utils/waiter.py` & `scaleway_core-0.9.0/scaleway_core/utils/waiter.py`

 * *Files identical despite different names*

### Comparing `scaleway_core-0.8.0/scaleway_core/validations/string_validation.py` & `scaleway_core-0.9.0/scaleway_core/validations/string_validation.py`

 * *Files identical despite different names*

### Comparing `scaleway_core-0.8.0/PKG-INFO` & `scaleway_core-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scaleway-core
-Version: 0.8.0
+Version: 0.9.0
 Summary: Scaleway SDK for Python
 License: BSD
 Author: Scaleway
 Author-email: opensource@scaleway.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
```

