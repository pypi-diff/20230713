# Comparing `tmp/eandb-0.1.1.tar.gz` & `tmp/eandb-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eandb-0.1.1.tar", max compression
+gzip compressed data, was "eandb-0.1.2.tar", max compression
```

## Comparing `eandb-0.1.1.tar` & `eandb-0.1.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1686 2023-06-24 05:46:51.693016 eandb-0.1.1/README.md
--rw-r--r--   0        0        0        0 2023-06-21 22:18:22.090555 eandb-0.1.1/eandb/__init__.py
--rw-r--r--   0        0        0        0 2023-06-23 14:27:00.935366 eandb-0.1.1/eandb/clients/__init__.py
--rw-r--r--   0        0        0     3806 2023-06-24 05:01:13.947313 eandb-0.1.1/eandb/clients/v1/__init__.py
--rw-r--r--   0        0        0        0 2023-06-23 14:25:40.421487 eandb-0.1.1/eandb/models/__init__.py
--rw-r--r--   0        0        0     3040 2023-06-23 20:50:17.797645 eandb-0.1.1/eandb/models/v1/__init__.py
--rw-r--r--   0        0        0      664 2023-06-24 18:53:06.324863 eandb-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2438 1970-01-01 00:00:00.000000 eandb-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1686 2023-06-24 05:46:51.693016 eandb-0.1.2/README.md
+-rw-r--r--   0        0        0        0 2023-06-21 22:18:22.090555 eandb-0.1.2/eandb/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-23 14:27:00.935366 eandb-0.1.2/eandb/clients/__init__.py
+-rw-r--r--   0        0        0     3806 2023-06-24 05:01:13.947313 eandb-0.1.2/eandb/clients/v1/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-23 14:25:40.421487 eandb-0.1.2/eandb/models/__init__.py
+-rw-r--r--   0        0        0     3078 2023-07-13 11:51:33.098355 eandb-0.1.2/eandb/models/v1/__init__.py
+-rw-r--r--   0        0        0      664 2023-07-13 15:21:00.593170 eandb-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2438 1970-01-01 00:00:00.000000 eandb-0.1.2/PKG-INFO
```

### Comparing `eandb-0.1.1/README.md` & `eandb-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `eandb-0.1.1/eandb/clients/v1/__init__.py` & `eandb-0.1.2/eandb/clients/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `eandb-0.1.1/eandb/models/v1/__init__.py` & `eandb-0.1.2/eandb/models/v1/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,13 +101,14 @@
         printBook: Optional[PrintBook]
         musicCD: Optional[MusicCD]
 
     barcode: str
     titles: dict[str, str]
     categories: list[Category]
     manufacturer: Optional[Manufacturer]
+    relatedBrands: list[Manufacturer]
     images: list[Image]
     metadata: Optional[Metadata]
 
 
 class ProductResponse(EandbResponse):
     product: Product
```

### Comparing `eandb-0.1.1/pyproject.toml` & `eandb-0.1.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "eandb"
-version = "0.1.1"
+version = "0.1.2"
 description = "Python client for EAN-DB API"
 authors = ["EAN-DB <support@ean-db.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/ean-db/python-client"
 repository = "https://github.com/ean-db/python-client"
 keywords = ["barcode", "ean", "upc", "isbn"]
```

### Comparing `eandb-0.1.1/PKG-INFO` & `eandb-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eandb
-Version: 0.1.1
+Version: 0.1.2
 Summary: Python client for EAN-DB API
 Home-page: https://github.com/ean-db/python-client
 License: MIT
 Keywords: barcode,ean,upc,isbn
 Author: EAN-DB
 Author-email: support@ean-db.com
 Requires-Python: >=3.8.1
```

