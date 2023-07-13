# Comparing `tmp/eandb-0.1.2.tar.gz` & `tmp/eandb-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eandb-0.1.2.tar", max compression
+gzip compressed data, was "eandb-0.2.0.tar", max compression
```

## Comparing `eandb-0.1.2.tar` & `eandb-0.2.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1686 2023-06-24 05:46:51.693016 eandb-0.1.2/README.md
--rw-r--r--   0        0        0        0 2023-06-21 22:18:22.090555 eandb-0.1.2/eandb/__init__.py
--rw-r--r--   0        0        0        0 2023-06-23 14:27:00.935366 eandb-0.1.2/eandb/clients/__init__.py
--rw-r--r--   0        0        0     3806 2023-06-24 05:01:13.947313 eandb-0.1.2/eandb/clients/v1/__init__.py
--rw-r--r--   0        0        0        0 2023-06-23 14:25:40.421487 eandb-0.1.2/eandb/models/__init__.py
--rw-r--r--   0        0        0     3078 2023-07-13 11:51:33.098355 eandb-0.1.2/eandb/models/v1/__init__.py
--rw-r--r--   0        0        0      664 2023-07-13 15:21:00.593170 eandb-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     2438 1970-01-01 00:00:00.000000 eandb-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1686 2023-06-24 05:46:51.693016 eandb-0.2.0/README.md
+-rw-r--r--   0        0        0        0 2023-06-21 22:18:22.090555 eandb-0.2.0/eandb/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-23 14:27:00.935366 eandb-0.2.0/eandb/clients/__init__.py
+-rw-r--r--   0        0        0     3806 2023-06-24 05:01:13.947313 eandb-0.2.0/eandb/clients/v1/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-23 14:25:40.421487 eandb-0.2.0/eandb/models/__init__.py
+-rw-r--r--   0        0        0     3229 2023-07-13 15:43:23.909369 eandb-0.2.0/eandb/models/v1/__init__.py
+-rw-r--r--   0        0        0      664 2023-07-13 15:45:11.834380 eandb-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2438 1970-01-01 00:00:00.000000 eandb-0.2.0/PKG-INFO
```

### Comparing `eandb-0.1.2/README.md` & `eandb-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `eandb-0.1.2/eandb/clients/v1/__init__.py` & `eandb-0.2.0/eandb/clients/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `eandb-0.1.2/eandb/models/v1/__init__.py` & `eandb-0.2.0/eandb/models/v1/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -27,16 +27,15 @@
 
 class Error(BaseModel):
     code: int
     description: str
 
 
 class EandbResponse(BaseModel):
-    balance: Optional[int]
-    error: Optional[Error]
+    error: Optional[Error] = None
 
     def get_error_type(self) -> Optional[ErrorType]:
         if not self.error:
             return None
 
         if self.error.code == 400:
             return ErrorType.INVALID_BARCODE
@@ -50,65 +49,66 @@
 
 class Product(BaseModel):
     class Category(BaseModel):
         id: str
         titles: dict[str, str]
 
     class Manufacturer(BaseModel):
-        id: Optional[str]
+        id: Optional[str] = None
         titles: dict[str, str]
-        wikidataId: Optional[str]
+        wikidataId: Optional[str] = None
 
     class Image(BaseModel):
         url: str
 
     class Metadata(BaseModel):
         class ExternalIds(BaseModel):
             amazonAsin: Optional[str]
 
         class Generic(BaseModel):
             class Contributor(BaseModel):
                 names: dict[str, str]
                 type: str
 
-            weightGrams: Optional[int]
-            manufacturerCode: Optional[str]
-            color: Optional[str]
-            materials: Optional[list[str]]
-            contributors: Optional[list[Contributor]]
+            weightGrams: Optional[int] = None
+            manufacturerCode: Optional[str] = None
+            color: Optional[str] = None
+            materials: Optional[list[str]] = None
+            contributors: Optional[list[Contributor]] = None
 
         class Food(BaseModel):
             class Nutriments(BaseModel):
-                fatGrams: Optional[Decimal]
-                proteinsGrams: Optional[Decimal]
-                carbohydratesGrams: Optional[Decimal]
-                energyKCal: Optional[Decimal]
+                fatGrams: Optional[Decimal] = None
+                proteinsGrams: Optional[Decimal] = None
+                carbohydratesGrams: Optional[Decimal] = None
+                energyKCal: Optional[Decimal] = None
 
             nutrimentsPer100Grams: Optional[Nutriments]
 
         class PrintBook(BaseModel):
-            numPages: Optional[int]
-            publishedYear: Optional[int]
-            bisacCodes: Optional[list[str]]
-            bindingType: Optional[str]
+            numPages: Optional[int] = None
+            publishedYear: Optional[int] = None
+            bisacCodes: Optional[list[str]] = None
+            bindingType: Optional[str] = None
 
         class MusicCD(BaseModel):
-            releasedYear: Optional[int]
-            numberOfDiscs: Optional[int]
+            releasedYear: Optional[int] = None
+            numberOfDiscs: Optional[int] = None
 
-        externalIds: Optional[ExternalIds]
-        generic: Optional[Generic]
-        food: Optional[Food]
-        printBook: Optional[PrintBook]
-        musicCD: Optional[MusicCD]
+        externalIds: Optional[ExternalIds] = None
+        generic: Optional[Generic] = None
+        food: Optional[Food] = None
+        printBook: Optional[PrintBook] = None
+        musicCD: Optional[MusicCD] = None
 
     barcode: str
     titles: dict[str, str]
     categories: list[Category]
     manufacturer: Optional[Manufacturer]
     relatedBrands: list[Manufacturer]
     images: list[Image]
     metadata: Optional[Metadata]
 
 
 class ProductResponse(EandbResponse):
+    balance: int
     product: Product
```

### Comparing `eandb-0.1.2/pyproject.toml` & `eandb-0.2.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "eandb"
-version = "0.1.2"
+version = "0.2.0"
 description = "Python client for EAN-DB API"
 authors = ["EAN-DB <support@ean-db.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/ean-db/python-client"
 repository = "https://github.com/ean-db/python-client"
 keywords = ["barcode", "ean", "upc", "isbn"]
```

### Comparing `eandb-0.1.2/PKG-INFO` & `eandb-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eandb
-Version: 0.1.2
+Version: 0.2.0
 Summary: Python client for EAN-DB API
 Home-page: https://github.com/ean-db/python-client
 License: MIT
 Keywords: barcode,ean,upc,isbn
 Author: EAN-DB
 Author-email: support@ean-db.com
 Requires-Python: >=3.8.1
```

