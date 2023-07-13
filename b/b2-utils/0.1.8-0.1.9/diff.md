# Comparing `tmp/b2-utils-0.1.8.tar.gz` & `tmp/b2-utils-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "b2-utils-0.1.8.tar", last modified: Tue Jan 24 14:38:55 2023, max compression
+gzip compressed data, was "b2-utils-0.1.9.tar", last modified: Thu Feb  9 13:11:53 2023, max compression
```

## Comparing `b2-utils-0.1.8.tar` & `b2-utils-0.1.9.tar`

### file list

```diff
@@ -1,35 +1,38 @@
-drwxrwxr-x   0 felipesena  (1005) felipesena  (1005)        0 2023-01-24 14:38:55.882298 b2-utils-0.1.8/
--rw-rw-r--   0 felipesena  (1005) felipesena  (1005)      438 2023-01-24 14:38:55.882298 b2-utils-0.1.8/PKG-INFO
--rw-rw-r--   0 felipesena  (1005) felipesena  (1005)       11 2023-01-05 12:46:21.000000 b2-utils-0.1.8/README.md
--rw-rw-r--   0 felipesena  (1005) felipesena  (1005)     1490 2023-01-24 14:38:51.000000 b2-utils-0.1.8/pyproject.toml
--rw-rw-r--   0 felipesena  (1005) felipesena  (1005)       38 2023-01-24 14:38:55.882298 b2-utils-0.1.8/setup.cfg
-drwxrwxr-x   0 felipesena  (1005) felipesena  (1005)        0 2023-01-24 14:38:55.878297 b2-utils-0.1.8/src/
-drwxrwxr-x   0 felipesena  (1005) felipesena  (1005)        0 2023-01-24 14:38:55.878297 b2-utils-0.1.8/src/b2_utils/
--rw-rw-r--   0 felipesena  (1005) felipesena  (1005)        0 2023-01-05 10:38:52.000000 b2-utils-0.1.8/src/b2_utils/__init__.py
--rw-rw-r--   0 felipesena  (1005) felipesena  (1005)      166 2023-01-24 14:29:43.000000 b2-utils-0.1.8/src/b2_utils/admin.py
--rw-rw-r--   0 felipesena  (1005) felipesena  (1005)      147 2023-01-24 14:26:12.000000 b2-utils-0.1.8/src/b2_utils/apps.py
--rw-rw-r--   0 felipesena  (1005) felipesena  (1005)      902 2023-01-24 13:14:20.000000 b2-utils-0.1.8/src/b2_utils/fields.py
--rw-rw-r--   0 felipesena  (1005) felipesena  (1005)     1640 2023-01-24 13:14:50.000000 b2-utils-0.1.8/src/b2_utils/helpers.py
-drwxrwxr-x   0 felipesena  (1005) felipesena  (1005)        0 2023-01-24 14:38:55.878297 b2-utils-0.1.8/src/b2_utils/migrations/
--rw-rw-r--   0 felipesena  (1005) felipesena  (1005)     6814 2023-01-24 14:37:47.000000 b2-utils-0.1.8/src/b2_utils/migrations/0001_initial.py
--rw-rw-r--   0 felipesena  (1005) felipesena  (1005)        0 2023-01-24 14:37:39.000000 b2-utils-0.1.8/src/b2_utils/migrations/__init__.py
-drwxrwxr-x   0 felipesena  (1005) felipesena  (1005)        0 2023-01-24 14:38:55.882298 b2-utils-0.1.8/src/b2_utils/models/
--rw-rw-r--   0 felipesena  (1005) felipesena  (1005)     2029 2023-01-24 12:48:47.000000 b2-utils-0.1.8/src/b2_utils/models/__init__.py
--rw-rw-r--   0 felipesena  (1005) felipesena  (1005)     6290 2023-01-24 14:27:18.000000 b2-utils-0.1.8/src/b2_utils/models/enums.py
--rw-rw-r--   0 felipesena  (1005) felipesena  (1005)      424 2023-01-24 13:19:17.000000 b2-utils-0.1.8/src/b2_utils/pagination.py
--rw-rw-r--   0 felipesena  (1005) felipesena  (1005)     1916 2023-01-24 13:28:53.000000 b2-utils-0.1.8/src/b2_utils/permissions.py
-drwxrwxr-x   0 felipesena  (1005) felipesena  (1005)        0 2023-01-24 14:38:55.882298 b2-utils-0.1.8/src/b2_utils/serializers/
--rw-rw-r--   0 felipesena  (1005) felipesena  (1005)     1275 2023-01-24 12:34:02.000000 b2-utils-0.1.8/src/b2_utils/serializers/__init__.py
--rw-rw-r--   0 felipesena  (1005) felipesena  (1005)      889 2023-01-24 13:03:53.000000 b2-utils-0.1.8/src/b2_utils/serializers/relations.py
-drwxrwxr-x   0 felipesena  (1005) felipesena  (1005)        0 2023-01-24 14:38:55.882298 b2-utils-0.1.8/src/b2_utils/tests/
--rw-rw-r--   0 felipesena  (1005) felipesena  (1005)      131 2023-01-24 13:44:45.000000 b2-utils-0.1.8/src/b2_utils/tests/__init__.py
--rw-rw-r--   0 felipesena  (1005) felipesena  (1005)      850 2023-01-24 12:38:12.000000 b2-utils-0.1.8/src/b2_utils/tests/helpers.py
--rw-rw-r--   0 felipesena  (1005) felipesena  (1005)     2011 2023-01-24 13:39:37.000000 b2-utils-0.1.8/src/b2_utils/validators.py
-drwxrwxr-x   0 felipesena  (1005) felipesena  (1005)        0 2023-01-24 14:38:55.878297 b2-utils-0.1.8/src/b2_utils.egg-info/
--rw-rw-r--   0 felipesena  (1005) felipesena  (1005)      438 2023-01-24 14:38:55.000000 b2-utils-0.1.8/src/b2_utils.egg-info/PKG-INFO
--rw-rw-r--   0 felipesena  (1005) felipesena  (1005)      703 2023-01-24 14:38:55.000000 b2-utils-0.1.8/src/b2_utils.egg-info/SOURCES.txt
--rw-rw-r--   0 felipesena  (1005) felipesena  (1005)        1 2023-01-24 14:38:55.000000 b2-utils-0.1.8/src/b2_utils.egg-info/dependency_links.txt
--rw-rw-r--   0 felipesena  (1005) felipesena  (1005)      139 2023-01-24 14:38:55.000000 b2-utils-0.1.8/src/b2_utils.egg-info/requires.txt
--rw-rw-r--   0 felipesena  (1005) felipesena  (1005)       25 2023-01-24 14:38:55.000000 b2-utils-0.1.8/src/b2_utils.egg-info/top_level.txt
--rwxrwxr-x   0 felipesena  (1005) felipesena  (1005)      655 2023-01-24 14:36:46.000000 b2-utils-0.1.8/src/manage.py
--rw-rw-r--   0 felipesena  (1005) felipesena  (1005)       37 2023-01-24 14:37:52.000000 b2-utils-0.1.8/src/settings.py
+drwxrwxr-x   0 felipesena  (1005) felipesena  (1005)        0 2023-02-09 13:11:53.317531 b2-utils-0.1.9/
+-rw-rw-r--   0 felipesena  (1005) felipesena  (1005)      438 2023-02-09 13:11:53.317531 b2-utils-0.1.9/PKG-INFO
+-rw-rw-r--   0 felipesena  (1005) felipesena  (1005)       11 2023-01-05 12:46:21.000000 b2-utils-0.1.9/README.md
+-rw-rw-r--   0 felipesena  (1005) felipesena  (1005)     1559 2023-02-09 13:11:38.000000 b2-utils-0.1.9/pyproject.toml
+-rw-rw-r--   0 felipesena  (1005) felipesena  (1005)       38 2023-02-09 13:11:53.317531 b2-utils-0.1.9/setup.cfg
+drwxrwxr-x   0 felipesena  (1005) felipesena  (1005)        0 2023-02-09 13:11:53.301531 b2-utils-0.1.9/src/
+drwxrwxr-x   0 felipesena  (1005) felipesena  (1005)        0 2023-02-09 13:11:53.305531 b2-utils-0.1.9/src/b2_utils/
+-rw-rw-r--   0 felipesena  (1005) felipesena  (1005)        0 2023-01-05 10:38:52.000000 b2-utils-0.1.9/src/b2_utils/__init__.py
+-rw-rw-r--   0 felipesena  (1005) felipesena  (1005)      166 2023-01-24 14:29:43.000000 b2-utils-0.1.9/src/b2_utils/admin.py
+-rw-rw-r--   0 felipesena  (1005) felipesena  (1005)      147 2023-01-24 14:26:12.000000 b2-utils-0.1.9/src/b2_utils/apps.py
+-rw-rw-r--   0 felipesena  (1005) felipesena  (1005)      194 2023-02-09 12:47:40.000000 b2-utils-0.1.9/src/b2_utils/decorators.py
+-rw-rw-r--   0 felipesena  (1005) felipesena  (1005)      902 2023-01-24 13:14:20.000000 b2-utils-0.1.9/src/b2_utils/fields.py
+drwxrwxr-x   0 felipesena  (1005) felipesena  (1005)        0 2023-02-09 13:11:53.309531 b2-utils-0.1.9/src/b2_utils/helpers/
+-rw-rw-r--   0 felipesena  (1005) felipesena  (1005)     2911 2023-02-09 13:10:14.000000 b2-utils-0.1.9/src/b2_utils/helpers/__init__.py
+-rw-rw-r--   0 felipesena  (1005) felipesena  (1005)     1041 2023-02-09 13:09:47.000000 b2-utils-0.1.9/src/b2_utils/helpers/auth.py
+drwxrwxr-x   0 felipesena  (1005) felipesena  (1005)        0 2023-02-09 13:11:53.309531 b2-utils-0.1.9/src/b2_utils/migrations/
+-rw-rw-r--   0 felipesena  (1005) felipesena  (1005)     6814 2023-01-24 14:37:47.000000 b2-utils-0.1.9/src/b2_utils/migrations/0001_initial.py
+-rw-rw-r--   0 felipesena  (1005) felipesena  (1005)        0 2023-01-24 14:37:39.000000 b2-utils-0.1.9/src/b2_utils/migrations/__init__.py
+drwxrwxr-x   0 felipesena  (1005) felipesena  (1005)        0 2023-02-09 13:11:53.313531 b2-utils-0.1.9/src/b2_utils/models/
+-rw-rw-r--   0 felipesena  (1005) felipesena  (1005)     2043 2023-02-09 12:50:33.000000 b2-utils-0.1.9/src/b2_utils/models/__init__.py
+-rw-rw-r--   0 felipesena  (1005) felipesena  (1005)     7070 2023-02-09 12:51:02.000000 b2-utils-0.1.9/src/b2_utils/models/enums.py
+-rw-rw-r--   0 felipesena  (1005) felipesena  (1005)      424 2023-01-24 13:19:17.000000 b2-utils-0.1.9/src/b2_utils/pagination.py
+-rw-rw-r--   0 felipesena  (1005) felipesena  (1005)     1916 2023-01-24 13:28:53.000000 b2-utils-0.1.9/src/b2_utils/permissions.py
+drwxrwxr-x   0 felipesena  (1005) felipesena  (1005)        0 2023-02-09 13:11:53.313531 b2-utils-0.1.9/src/b2_utils/serializers/
+-rw-rw-r--   0 felipesena  (1005) felipesena  (1005)     1275 2023-01-24 12:34:02.000000 b2-utils-0.1.9/src/b2_utils/serializers/__init__.py
+-rw-rw-r--   0 felipesena  (1005) felipesena  (1005)      889 2023-01-24 13:03:53.000000 b2-utils-0.1.9/src/b2_utils/serializers/relations.py
+drwxrwxr-x   0 felipesena  (1005) felipesena  (1005)        0 2023-02-09 13:11:53.313531 b2-utils-0.1.9/src/b2_utils/tests/
+-rw-rw-r--   0 felipesena  (1005) felipesena  (1005)      131 2023-01-24 13:44:45.000000 b2-utils-0.1.9/src/b2_utils/tests/__init__.py
+-rw-rw-r--   0 felipesena  (1005) felipesena  (1005)     1634 2023-02-09 12:55:44.000000 b2-utils-0.1.9/src/b2_utils/tests/helpers.py
+-rw-rw-r--   0 felipesena  (1005) felipesena  (1005)     2011 2023-01-24 13:39:37.000000 b2-utils-0.1.9/src/b2_utils/validators.py
+drwxrwxr-x   0 felipesena  (1005) felipesena  (1005)        0 2023-02-09 13:11:53.305531 b2-utils-0.1.9/src/b2_utils.egg-info/
+-rw-rw-r--   0 felipesena  (1005) felipesena  (1005)      438 2023-02-09 13:11:53.000000 b2-utils-0.1.9/src/b2_utils.egg-info/PKG-INFO
+-rw-rw-r--   0 felipesena  (1005) felipesena  (1005)      768 2023-02-09 13:11:53.000000 b2-utils-0.1.9/src/b2_utils.egg-info/SOURCES.txt
+-rw-rw-r--   0 felipesena  (1005) felipesena  (1005)        1 2023-02-09 13:11:53.000000 b2-utils-0.1.9/src/b2_utils.egg-info/dependency_links.txt
+-rw-rw-r--   0 felipesena  (1005) felipesena  (1005)      139 2023-02-09 13:11:53.000000 b2-utils-0.1.9/src/b2_utils.egg-info/requires.txt
+-rw-rw-r--   0 felipesena  (1005) felipesena  (1005)       25 2023-02-09 13:11:53.000000 b2-utils-0.1.9/src/b2_utils.egg-info/top_level.txt
+-rwxrwxr-x   0 felipesena  (1005) felipesena  (1005)      655 2023-01-24 14:36:46.000000 b2-utils-0.1.9/src/manage.py
+-rw-rw-r--   0 felipesena  (1005) felipesena  (1005)       37 2023-01-24 14:37:52.000000 b2-utils-0.1.9/src/settings.py
```

### Comparing `b2-utils-0.1.8/pyproject.toml` & `b2-utils-0.1.9/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "b2-utils"
-version = "0.1.8"
+version = "0.1.9"
 authors = [
   { name="Felipe Sena", email="felipesena@b2bit.company" },
 ]
 description = "A useful package provided by B2BIT"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
@@ -41,14 +41,16 @@
 Faker = "^15.3.4"
 Django = "^4.1.5"
 djangorestframework = "^3.14.0"
 Pillow = "^9.4.0"
 django-model-utils = "^4.3.1"
 model-bakery = "^1.9.0"
 pre-commit = "^3.0.0"
+django-constance = "^2.9.1"
+djangorestframework-simplejwt = "^5.2.2"
 
 [tool.poetry.dev-dependencies]
 black = "^22.3.0"
 flake8 = "^4.0.1"
 pylint = "^2.13.5"
 pylint-django = "^2.5.3"
 bandit = "^1.7.4"
```

### Comparing `b2-utils-0.1.8/src/b2_utils/fields.py` & `b2-utils-0.1.9/src/b2_utils/fields.py`

 * *Files identical despite different names*

### Comparing `b2-utils-0.1.8/src/b2_utils/migrations/0001_initial.py` & `b2-utils-0.1.9/src/b2_utils/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `b2-utils-0.1.8/src/b2_utils/models/__init__.py` & `b2-utils-0.1.9/src/b2_utils/models/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,30 +20,30 @@
     number = _models.CharField("Número", max_length=9)
 
     class Meta:
         ordering = ["-created"]
         verbose_name = "Telefone"
         verbose_name_plural = "Telefones"
 
-    def __str__(self):
+    def __str__(self) -> str:
         return f"({self.country_code}) {self.area_code}-{self.number}"
 
 
 class City(_TimeStampedModel):
     """A TimeStampedModel City model, ordered by it's creation date"""
 
     name = _models.CharField("Cidade", max_length=255)
     state = _models.CharField("Estado", max_length=2, choices=States.choices)
 
     class Meta:
         ordering = ["-created"]
         verbose_name = "Cidade"
         verbose_name_plural = "Cidades"
 
-    def __str__(self):
+    def __str__(self) -> str:
         return f"{self.name}, {self.state}"
 
 
 class Address(_TimeStampedModel):
     """A TimeStampedModel Address model, ordered by it's creation date"""
 
     zip_code = _models.CharField("CEP", max_length=10)
```

### Comparing `b2-utils-0.1.8/src/b2_utils/models/enums.py` & `b2-utils-0.1.9/src/b2_utils/models/enums.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,44 @@
+import operator as _operator
+from enum import Enum as _Enum
+from typing import Callable as _Callable
+
+from django.db import models as _models
 from django.db.models import enums as _enums
 
 __all__ = [
     "States",
     "Colors",
+    "Operator",
+    "OrderedTextChoices",
 ]
 
 
+class Operator(_Enum):
+    LT = _operator.lt
+    GT = _operator.gt
+    LTE = _operator.le
+    GTE = _operator.ge
+
+
+class OrderedTextChoices(_models.TextChoices):
+    @classmethod
+    def get_value(cls, choice) -> int | None:
+        for index, option in enumerate(cls.choices):
+            if choice == option[0]:
+                return index
+
+    @classmethod
+    def compare(cls, first, op: Operator | _Callable, second) -> bool:
+        if callable(op):
+            return op(cls.get_value(first), cls.get_value(second))
+
+        return op.value(cls.get_value(first), cls.get_value(second))
+
+
 class States(_enums.TextChoices):
     AC = "AC", "Acre"
     AL = "AL", "Alagoas"
     AM = "AM", "Amazonas"
     AP = "AP", "Amapá"
     BA = "BA", "Bahia"
     CE = "CE", "Ceará"
```

### Comparing `b2-utils-0.1.8/src/b2_utils/permissions.py` & `b2-utils-0.1.9/src/b2_utils/permissions.py`

 * *Files identical despite different names*

### Comparing `b2-utils-0.1.8/src/b2_utils/serializers/__init__.py` & `b2-utils-0.1.9/src/b2_utils/serializers/__init__.py`

 * *Files identical despite different names*

### Comparing `b2-utils-0.1.8/src/b2_utils/serializers/relations.py` & `b2-utils-0.1.9/src/b2_utils/serializers/relations.py`

 * *Files identical despite different names*

### Comparing `b2-utils-0.1.8/src/b2_utils/validators.py` & `b2-utils-0.1.9/src/b2_utils/validators.py`

 * *Files identical despite different names*

### Comparing `b2-utils-0.1.8/src/b2_utils.egg-info/SOURCES.txt` & `b2-utils-0.1.9/src/b2_utils.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 README.md
 pyproject.toml
 src/manage.py
 src/settings.py
 src/b2_utils/__init__.py
 src/b2_utils/admin.py
 src/b2_utils/apps.py
+src/b2_utils/decorators.py
 src/b2_utils/fields.py
-src/b2_utils/helpers.py
 src/b2_utils/pagination.py
 src/b2_utils/permissions.py
 src/b2_utils/validators.py
 src/b2_utils.egg-info/PKG-INFO
 src/b2_utils.egg-info/SOURCES.txt
 src/b2_utils.egg-info/dependency_links.txt
 src/b2_utils.egg-info/requires.txt
 src/b2_utils.egg-info/top_level.txt
+src/b2_utils/helpers/__init__.py
+src/b2_utils/helpers/auth.py
 src/b2_utils/migrations/0001_initial.py
 src/b2_utils/migrations/__init__.py
 src/b2_utils/models/__init__.py
 src/b2_utils/models/enums.py
 src/b2_utils/serializers/__init__.py
 src/b2_utils/serializers/relations.py
 src/b2_utils/tests/__init__.py
```

### Comparing `b2-utils-0.1.8/src/manage.py` & `b2-utils-0.1.9/src/manage.py`

 * *Files identical despite different names*

