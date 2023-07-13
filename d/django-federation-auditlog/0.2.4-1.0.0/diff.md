# Comparing `tmp/django_federation_auditlog-0.2.4.tar.gz` & `tmp/django_federation_auditlog-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_federation_auditlog-0.2.4.tar", max compression
+gzip compressed data, was "django_federation_auditlog-1.0.0.tar", max compression
```

## Comparing `django_federation_auditlog-0.2.4.tar` & `django_federation_auditlog-1.0.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     2542 2023-06-20 20:03:52.117219 django_federation_auditlog-0.2.4/README.md
--rw-r--r--   0        0        0       22 2023-06-20 20:03:52.117219 django_federation_auditlog-0.2.4/django_federation_auditlog/__init__.py
--rw-r--r--   0        0        0      799 2023-06-20 20:03:52.117219 django_federation_auditlog-0.2.4/django_federation_auditlog/admin.py
--rw-r--r--   0        0        0      127 2023-06-20 20:03:52.117219 django_federation_auditlog-0.2.4/django_federation_auditlog/apps.py
--rw-r--r--   0        0        0     5513 2023-06-20 20:03:52.117219 django_federation_auditlog-0.2.4/django_federation_auditlog/diff.py
--rw-r--r--   0        0        0     4175 2023-06-20 20:03:52.117219 django_federation_auditlog-0.2.4/django_federation_auditlog/middleware.py
--rw-r--r--   0        0        0     3212 2023-06-20 20:03:52.117219 django_federation_auditlog-0.2.4/django_federation_auditlog/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2023-06-20 20:03:52.117219 django_federation_auditlog-0.2.4/django_federation_auditlog/migrations/__init__.py
--rw-r--r--   0        0        0     2373 2023-06-20 20:03:52.117219 django_federation_auditlog-0.2.4/django_federation_auditlog/mixins.py
--rw-r--r--   0        0        0    15062 2023-06-20 20:03:52.117219 django_federation_auditlog-0.2.4/django_federation_auditlog/models.py
--rw-r--r--   0        0        0     2084 2023-06-20 20:03:52.117219 django_federation_auditlog-0.2.4/django_federation_auditlog/receivers.py
--rw-r--r--   0        0        0     4720 2023-06-20 20:03:52.117219 django_federation_auditlog-0.2.4/django_federation_auditlog/registry.py
--rw-r--r--   0        0        0       60 2023-06-20 20:03:52.117219 django_federation_auditlog-0.2.4/django_federation_auditlog/tests.py
--rw-r--r--   0        0        0      742 2023-06-20 20:03:52.117219 django_federation_auditlog-0.2.4/pyproject.toml
--rw-r--r--   0        0        0     3201 1970-01-01 00:00:00.000000 django_federation_auditlog-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0     2664 2023-07-13 19:46:19.730240 django_federation_auditlog-1.0.0/README.md
+-rw-r--r--   0        0        0       22 2023-07-13 19:46:19.730240 django_federation_auditlog-1.0.0/django_federation_auditlog/__init__.py
+-rw-r--r--   0        0        0      799 2023-07-13 19:46:19.730240 django_federation_auditlog-1.0.0/django_federation_auditlog/admin.py
+-rw-r--r--   0        0        0      127 2023-07-13 19:46:19.730240 django_federation_auditlog-1.0.0/django_federation_auditlog/apps.py
+-rw-r--r--   0        0        0     5513 2023-07-13 19:46:19.730240 django_federation_auditlog-1.0.0/django_federation_auditlog/diff.py
+-rw-r--r--   0        0        0     4175 2023-07-13 19:46:19.730240 django_federation_auditlog-1.0.0/django_federation_auditlog/middleware.py
+-rw-r--r--   0        0        0     3146 2023-07-13 19:46:19.730240 django_federation_auditlog-1.0.0/django_federation_auditlog/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2023-07-13 19:46:19.730240 django_federation_auditlog-1.0.0/django_federation_auditlog/migrations/__init__.py
+-rw-r--r--   0        0        0     2373 2023-07-13 19:46:19.730240 django_federation_auditlog-1.0.0/django_federation_auditlog/mixins.py
+-rw-r--r--   0        0        0    14788 2023-07-13 19:46:19.734241 django_federation_auditlog-1.0.0/django_federation_auditlog/models.py
+-rw-r--r--   0        0        0     2084 2023-07-13 19:46:19.734241 django_federation_auditlog-1.0.0/django_federation_auditlog/receivers.py
+-rw-r--r--   0        0        0     4720 2023-07-13 19:46:19.734241 django_federation_auditlog-1.0.0/django_federation_auditlog/registry.py
+-rw-r--r--   0        0        0       60 2023-07-13 19:46:19.734241 django_federation_auditlog-1.0.0/django_federation_auditlog/tests.py
+-rw-r--r--   0        0        0      739 2023-07-13 19:46:19.734241 django_federation_auditlog-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     3326 1970-01-01 00:00:00.000000 django_federation_auditlog-1.0.0/PKG-INFO
```

### Comparing `django_federation_auditlog-0.2.4/README.md` & `django_federation_auditlog-1.0.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 ```shell
 pipenv install django-federation-auditlog
 ```
 
 with poetry
 
 ```shell
-poetry django-federation-auditlog
+poetry add django-federation-auditlog
 ```
 
 # Adding Django Federation Auditlog to your Django application
 
 To use in your application, just add 'django-federation-auditlog' to your project’s INSTALLED_APPS setting and add 'AuditlogMiddleware' to your's MIDDLEWARE setting then run manage.py migrate to create/upgrade the necessary database structure.
 
 ```python
@@ -63,14 +63,16 @@
     # Model definition goes here
 
 auditlog.register(MyModel)
 ```
 
 It is recommended to place the register code (auditlog.register(MyModel)) at the bottom of your models.py file.
 
+OBS: If ```.save()``` be called to a model and the fields have the same value, log entries ```don't``` be generated.
+
 ## Including Fields
 
 If ```include_fields``` is specified, only the fields with the given names will be included in the generated log entries.
 
 For example, to include only the field ```name``` from class MyModel, use:
 
 ```python
```

### Comparing `django_federation_auditlog-0.2.4/django_federation_auditlog/admin.py` & `django_federation_auditlog-1.0.0/django_federation_auditlog/admin.py`

 * *Files identical despite different names*

### Comparing `django_federation_auditlog-0.2.4/django_federation_auditlog/diff.py` & `django_federation_auditlog-1.0.0/django_federation_auditlog/diff.py`

 * *Files identical despite different names*

### Comparing `django_federation_auditlog-0.2.4/django_federation_auditlog/middleware.py` & `django_federation_auditlog-1.0.0/django_federation_auditlog/middleware.py`

 * *Files identical despite different names*

### Comparing `django_federation_auditlog-0.2.4/django_federation_auditlog/migrations/0001_initial.py` & `django_federation_auditlog-1.0.0/django_federation_auditlog/migrations/0001_initial.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # Generated by Django 2.2.17 on 2023-06-06 13:49
 
 from django.db import migrations, models
 import django.db.models.deletion
-import django_jsonfield_backport.models
 
 
 class Migration(migrations.Migration):
 
     initial = True
 
     dependencies = [
@@ -70,15 +69,15 @@
                     'timestamp',
                     models.DateTimeField(
                         auto_now_add=True, verbose_name='timestamp'
                     ),
                 ),
                 (
                     'additional_data',
-                    django_jsonfield_backport.models.JSONField(
+                    models.JSONField(
                         blank=True, null=True, verbose_name='additional data'
                     ),
                 ),
                 (
                     'content_type',
                     models.ForeignKey(
                         on_delete=django.db.models.deletion.CASCADE,
```

### Comparing `django_federation_auditlog-0.2.4/django_federation_auditlog/mixins.py` & `django_federation_auditlog-1.0.0/django_federation_auditlog/mixins.py`

 * *Files identical despite different names*

### Comparing `django_federation_auditlog-0.2.4/django_federation_auditlog/models.py` & `django_federation_auditlog-1.0.0/django_federation_auditlog/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 from django.contrib.contenttypes.models import ContentType
 from django.core.exceptions import FieldDoesNotExist
 from django.db import models
 from django.db.models import Field, Q, QuerySet
 from django.utils import formats, timezone
 from django.utils.encoding import smart_str
 from django.utils.translation import gettext_lazy as _
-from django_jsonfield_backport.models import JSONField
 
 
 class LogEntryManager(models.Manager):
     """
     Custom manager for the :py:class:`LogEntry` model.
     """
 
@@ -70,21 +69,15 @@
                         object_id=kwargs.get("object_id"),
                     ).delete()
                 else:
                     self.filter(
                         content_type=kwargs.get("content_type"),
                         object_pk=kwargs.get("object_pk", ""),
                     ).delete()
-            # save LogEntry to same database instance is using
-            db = instance._state.db
-            return (
-                self.create(**kwargs)
-                if db is None or db == ""
-                else self.using(db).create(**kwargs)
-            )
+            return self.create(**kwargs)
         return None
 
     def get_for_object(self, instance):
         """
         Get log entries for the specified model instance.
 
         :param instance: The model instance to get log entries for.
@@ -228,15 +221,15 @@
     actor = models.TextField(verbose_name=_("actor"))
     remote_addr = models.GenericIPAddressField(
         blank=True, null=True, verbose_name=_("remote address")
     )
     timestamp = models.DateTimeField(
         auto_now_add=True, verbose_name=_("timestamp")
     )
-    additional_data = JSONField(
+    additional_data = models.JSONField(
         blank=True, null=True, verbose_name=_("additional data")
     )
 
     objects = LogEntryManager()
 
     class Meta:
         get_latest_by = "timestamp"
```

### Comparing `django_federation_auditlog-0.2.4/django_federation_auditlog/receivers.py` & `django_federation_auditlog-1.0.0/django_federation_auditlog/receivers.py`

 * *Files identical despite different names*

### Comparing `django_federation_auditlog-0.2.4/django_federation_auditlog/registry.py` & `django_federation_auditlog-1.0.0/django_federation_auditlog/registry.py`

 * *Files identical despite different names*

### Comparing `django_federation_auditlog-0.2.4/PKG-INFO` & `django_federation_auditlog-1.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: django-federation-auditlog
-Version: 0.2.4
+Version: 1.0.0
 Summary: 
 Author: Anderson Marques
 Author-email: anderson89marques@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: django-auditlog (==1.0.0)
-Requires-Dist: djangorestframework (==3.11.1)
+Requires-Dist: django-auditlog (==2.0.0)
+Requires-Dist: djangorestframework (>=3.11,<4.0)
 Requires-Dist: djangorestframework-simplejwt (==5.0.0)
 Description-Content-Type: text/markdown
 
 # Django Auditlog
 This project is totally based in [Django Auditlog](https://github.com/jazzband/django-auditlog/tree/master) library.
 
 # Instalation
@@ -32,15 +32,15 @@
 ```shell
 pipenv install django-federation-auditlog
 ```
 
 with poetry
 
 ```shell
-poetry django-federation-auditlog
+poetry add django-federation-auditlog
 ```
 
 # Adding Django Federation Auditlog to your Django application
 
 To use in your application, just add 'django-federation-auditlog' to your project’s INSTALLED_APPS setting and add 'AuditlogMiddleware' to your's MIDDLEWARE setting then run manage.py migrate to create/upgrade the necessary database structure.
 
 ```python
@@ -81,14 +81,16 @@
     # Model definition goes here
 
 auditlog.register(MyModel)
 ```
 
 It is recommended to place the register code (auditlog.register(MyModel)) at the bottom of your models.py file.
 
+OBS: If ```.save()``` be called to a model and the fields have the same value, log entries ```don't``` be generated.
+
 ## Including Fields
 
 If ```include_fields``` is specified, only the fields with the given names will be included in the generated log entries.
 
 For example, to include only the field ```name``` from class MyModel, use:
 
 ```python
```

