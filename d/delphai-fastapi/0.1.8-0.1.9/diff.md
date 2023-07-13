# Comparing `tmp/delphai_fastapi-0.1.8.tar.gz` & `tmp/delphai_fastapi-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "delphai_fastapi-0.1.8.tar", max compression
+gzip compressed data, was "delphai_fastapi-0.1.9.tar", max compression
```

## Comparing `delphai_fastapi-0.1.8.tar` & `delphai_fastapi-0.1.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0        0 2023-06-30 10:59:54.322178 delphai_fastapi-0.1.8/delphai_fastapi/__init__.py
--rw-r--r--   0        0        0     2521 2023-06-30 10:59:54.322178 delphai_fastapi-0.1.8/delphai_fastapi/app.py
--rw-r--r--   0        0        0     3822 2023-06-30 10:59:54.322178 delphai_fastapi-0.1.8/delphai_fastapi/auth.py
--rw-r--r--   0        0        0        0 2023-06-30 10:59:54.322178 delphai_fastapi-0.1.8/delphai_fastapi/companies/__init__.py
--rw-r--r--   0        0        0     3584 2023-06-30 10:59:54.322178 delphai_fastapi-0.1.8/delphai_fastapi/companies/models.py
--rw-r--r--   0        0        0      375 2023-06-30 10:59:54.322178 delphai_fastapi-0.1.8/delphai_fastapi/decorators.py
--rw-r--r--   0        0        0        0 2023-06-30 10:59:54.322178 delphai_fastapi-0.1.8/delphai_fastapi/job_posts/__init__.py
--rw-r--r--   0        0        0      912 2023-06-30 10:59:54.322178 delphai_fastapi-0.1.8/delphai_fastapi/job_posts/models.py
--rw-r--r--   0        0        0     1808 2023-06-30 10:59:54.322178 delphai_fastapi-0.1.8/delphai_fastapi/models.py
--rw-r--r--   0        0        0        0 2023-06-30 10:59:54.322178 delphai_fastapi-0.1.8/delphai_fastapi/news_articles/__init__.py
--rw-r--r--   0        0        0     1135 2023-06-30 10:59:54.322178 delphai_fastapi-0.1.8/delphai_fastapi/news_articles/models.py
--rw-r--r--   0        0        0     1342 2023-06-30 10:59:54.322178 delphai_fastapi-0.1.8/delphai_fastapi/types.py
--rw-r--r--   0        0        0      446 2023-06-30 11:00:23.394258 delphai_fastapi-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      806 1970-01-01 00:00:00.000000 delphai_fastapi-0.1.8/setup.py
--rw-r--r--   0        0        0      552 1970-01-01 00:00:00.000000 delphai_fastapi-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-04 08:53:32.309480 delphai_fastapi-0.1.9/delphai_fastapi/__init__.py
+-rw-r--r--   0        0        0     2521 2023-07-04 08:53:32.309480 delphai_fastapi-0.1.9/delphai_fastapi/app.py
+-rw-r--r--   0        0        0     3822 2023-07-04 08:53:32.309480 delphai_fastapi-0.1.9/delphai_fastapi/auth.py
+-rw-r--r--   0        0        0        0 2023-07-04 08:53:32.309480 delphai_fastapi-0.1.9/delphai_fastapi/companies/__init__.py
+-rw-r--r--   0        0        0     3584 2023-07-04 08:53:32.309480 delphai_fastapi-0.1.9/delphai_fastapi/companies/models.py
+-rw-r--r--   0        0        0      375 2023-07-04 08:53:32.309480 delphai_fastapi-0.1.9/delphai_fastapi/decorators.py
+-rw-r--r--   0        0        0        0 2023-07-04 08:53:32.309480 delphai_fastapi-0.1.9/delphai_fastapi/job_posts/__init__.py
+-rw-r--r--   0        0        0      912 2023-07-04 08:53:32.309480 delphai_fastapi-0.1.9/delphai_fastapi/job_posts/models.py
+-rw-r--r--   0        0        0     1808 2023-07-04 08:53:32.309480 delphai_fastapi-0.1.9/delphai_fastapi/models.py
+-rw-r--r--   0        0        0        0 2023-07-04 08:53:32.309480 delphai_fastapi-0.1.9/delphai_fastapi/news_articles/__init__.py
+-rw-r--r--   0        0        0     1135 2023-07-04 08:53:32.309480 delphai_fastapi-0.1.9/delphai_fastapi/news_articles/models.py
+-rw-r--r--   0        0        0     1826 2023-07-04 08:53:32.309480 delphai_fastapi-0.1.9/delphai_fastapi/types.py
+-rw-r--r--   0        0        0      446 2023-07-04 08:54:07.926657 delphai_fastapi-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      806 1970-01-01 00:00:00.000000 delphai_fastapi-0.1.9/setup.py
+-rw-r--r--   0        0        0      552 1970-01-01 00:00:00.000000 delphai_fastapi-0.1.9/PKG-INFO
```

### Comparing `delphai_fastapi-0.1.8/delphai_fastapi/app.py` & `delphai_fastapi-0.1.9/delphai_fastapi/app.py`

 * *Files identical despite different names*

### Comparing `delphai_fastapi-0.1.8/delphai_fastapi/auth.py` & `delphai_fastapi-0.1.9/delphai_fastapi/auth.py`

 * *Files identical despite different names*

### Comparing `delphai_fastapi-0.1.8/delphai_fastapi/companies/models.py` & `delphai_fastapi-0.1.9/delphai_fastapi/companies/models.py`

 * *Files identical despite different names*

### Comparing `delphai_fastapi-0.1.8/delphai_fastapi/job_posts/models.py` & `delphai_fastapi-0.1.9/delphai_fastapi/job_posts/models.py`

 * *Files identical despite different names*

### Comparing `delphai_fastapi-0.1.8/delphai_fastapi/models.py` & `delphai_fastapi-0.1.9/delphai_fastapi/models.py`

 * *Files identical despite different names*

### Comparing `delphai_fastapi-0.1.8/delphai_fastapi/news_articles/models.py` & `delphai_fastapi-0.1.9/delphai_fastapi/news_articles/models.py`

 * *Files identical despite different names*

### Comparing `delphai_fastapi-0.1.8/delphai_fastapi/types.py` & `delphai_fastapi-0.1.9/delphai_fastapi/types.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from enum import Enum
 from bson.objectid import ObjectId as BsonObjectId
 from fastapi import Query, Depends
 from typing import Tuple
 
 
 class ObjectId(str):
     @classmethod
@@ -43,7 +44,31 @@
             description="The (zero-based) offset of the first item returned in the collection",  # noqa: E501
             example=0,
         ),
     ) -> Tuple[int, int]:
         return limit, offset
 
     return get_limit_offset
+
+
+class Order(Enum):
+    asc = "asc"
+    desc = "desc"
+
+
+def Sorting():
+    @Depends
+    def get_sorting(
+        sort_by: str = Query(
+            default="",
+            description="Sorting field",
+            example="name",
+        ),
+        order_by: Order = Query(
+            default="asc",
+            description="Sorting order",
+            example="asc",
+        ),
+    ) -> Tuple[str, str]:
+        return sort_by, order_by
+
+    return get_sorting
```

### Comparing `delphai_fastapi-0.1.8/setup.py` & `delphai_fastapi-0.1.9/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -15,15 +15,15 @@
  'fastapi>=0,<1',
  'httpx>=0,<1',
  'pymongo>3',
  'python-jose>=3.3,<4.0']
 
 setup_kwargs = {
     'name': 'delphai-fastapi',
-    'version': '0.1.8',
+    'version': '0.1.9',
     'description': 'Package for fastAPI models',
     'long_description': 'None',
     'author': 'Berinike Tech',
     'author_email': 'berinike@delphai.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `delphai_fastapi-0.1.8/PKG-INFO` & `delphai_fastapi-0.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: delphai-fastapi
-Version: 0.1.8
+Version: 0.1.9
 Summary: Package for fastAPI models
 Author: Berinike Tech
 Author-email: berinike@delphai.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

