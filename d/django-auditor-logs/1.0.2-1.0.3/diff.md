# Comparing `tmp/django_auditor_logs-1.0.2.tar.gz` & `tmp/django_auditor_logs-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_auditor_logs-1.0.2.tar", last modified: Sun Feb 19 22:29:58 2023, max compression
+gzip compressed data, was "django_auditor_logs-1.0.3.tar", last modified: Thu Jul 13 16:31:00 2023, max compression
```

## Comparing `django_auditor_logs-1.0.2.tar` & `django_auditor_logs-1.0.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 yeison    (1000) yeison    (1000)        0 2023-02-19 22:29:58.809033 django_auditor_logs-1.0.2/
--rw-r--r--   0 yeison    (1000) yeison    (1000)       22 2023-02-17 20:12:44.000000 django_auditor_logs-1.0.2/MANIFEST.in
--rw-r--r--   0 yeison    (1000) yeison    (1000)     2194 2023-02-19 22:29:58.809033 django_auditor_logs-1.0.2/PKG-INFO
--rw-r--r--   0 yeison    (1000) yeison    (1000)      985 2023-02-14 01:43:16.000000 django_auditor_logs-1.0.2/README.md
--rw-r--r--   0 yeison    (1000) yeison    (1000)     1617 2023-02-19 22:29:42.000000 django_auditor_logs-1.0.2/quickstart.rst
--rw-r--r--   0 yeison    (1000) yeison    (1000)      779 2023-02-19 22:29:58.813033 django_auditor_logs-1.0.2/setup.cfg
--rw-r--r--   0 yeison    (1000) yeison    (1000)       37 2023-02-17 20:13:05.000000 django_auditor_logs-1.0.2/setup.py
-drwxr-xr-x   0 yeison    (1000) yeison    (1000)        0 2023-02-19 22:29:58.805033 django_auditor_logs-1.0.2/src/
-drwxr-xr-x   0 yeison    (1000) yeison    (1000)        0 2023-02-19 22:29:58.809033 django_auditor_logs-1.0.2/src/django_auditor_logs/
--rw-r--r--   0 yeison    (1000) yeison    (1000)        0 2023-02-14 13:12:01.000000 django_auditor_logs-1.0.2/src/django_auditor_logs/__init__.py
--rw-r--r--   0 yeison    (1000) yeison    (1000)       63 2023-02-14 13:12:01.000000 django_auditor_logs-1.0.2/src/django_auditor_logs/admin.py
--rw-r--r--   0 yeison    (1000) yeison    (1000)      107 2023-02-18 02:34:42.000000 django_auditor_logs-1.0.2/src/django_auditor_logs/apps.py
--rw-r--r--   0 yeison    (1000) yeison    (1000)      477 2023-02-19 00:24:31.000000 django_auditor_logs-1.0.2/src/django_auditor_logs/metadata.py
-drwxr-xr-x   0 yeison    (1000) yeison    (1000)        0 2023-02-19 22:29:58.809033 django_auditor_logs-1.0.2/src/django_auditor_logs/middleware/
--rw-r--r--   0 yeison    (1000) yeison    (1000)        0 2023-02-19 00:14:15.000000 django_auditor_logs-1.0.2/src/django_auditor_logs/middleware/__init__.py
--rw-r--r--   0 yeison    (1000) yeison    (1000)     1654 2023-02-19 00:37:05.000000 django_auditor_logs-1.0.2/src/django_auditor_logs/middleware/metadata_middleware.py
--rw-r--r--   0 yeison    (1000) yeison    (1000)     5572 2023-02-19 00:46:19.000000 django_auditor_logs-1.0.2/src/django_auditor_logs/models.py
--rw-r--r--   0 yeison    (1000) yeison    (1000)       60 2023-02-14 13:12:01.000000 django_auditor_logs-1.0.2/src/django_auditor_logs/tests.py
--rw-r--r--   0 yeison    (1000) yeison    (1000)      108 2023-02-18 02:29:14.000000 django_auditor_logs-1.0.2/src/django_auditor_logs/views.py
-drwxr-xr-x   0 yeison    (1000) yeison    (1000)        0 2023-02-19 22:29:58.809033 django_auditor_logs-1.0.2/src/django_auditor_logs.egg-info/
--rw-r--r--   0 yeison    (1000) yeison    (1000)     2194 2023-02-19 22:29:58.000000 django_auditor_logs-1.0.2/src/django_auditor_logs.egg-info/PKG-INFO
--rw-r--r--   0 yeison    (1000) yeison    (1000)      648 2023-02-19 22:29:58.000000 django_auditor_logs-1.0.2/src/django_auditor_logs.egg-info/SOURCES.txt
--rw-r--r--   0 yeison    (1000) yeison    (1000)        1 2023-02-19 22:29:58.000000 django_auditor_logs-1.0.2/src/django_auditor_logs.egg-info/dependency_links.txt
--rw-r--r--   0 yeison    (1000) yeison    (1000)       12 2023-02-19 22:29:58.000000 django_auditor_logs-1.0.2/src/django_auditor_logs.egg-info/requires.txt
--rw-r--r--   0 yeison    (1000) yeison    (1000)       20 2023-02-19 22:29:58.000000 django_auditor_logs-1.0.2/src/django_auditor_logs.egg-info/top_level.txt
+drwxr-xr-x   0 yeison    (1000) yeison    (1000)        0 2023-07-13 16:31:00.338710 django_auditor_logs-1.0.3/
+-rw-r--r--   0 yeison    (1000) yeison    (1000)       22 2023-02-17 20:12:44.000000 django_auditor_logs-1.0.3/MANIFEST.in
+-rw-r--r--   0 yeison    (1000) yeison    (1000)     2248 2023-07-13 16:31:00.338710 django_auditor_logs-1.0.3/PKG-INFO
+-rw-r--r--   0 yeison    (1000) yeison    (1000)      985 2023-02-14 01:43:16.000000 django_auditor_logs-1.0.3/README.md
+-rw-r--r--   0 yeison    (1000) yeison    (1000)     1671 2023-07-13 16:30:25.000000 django_auditor_logs-1.0.3/quickstart.rst
+-rw-r--r--   0 yeison    (1000) yeison    (1000)      779 2023-07-13 16:31:00.338710 django_auditor_logs-1.0.3/setup.cfg
+-rw-r--r--   0 yeison    (1000) yeison    (1000)       37 2023-02-17 20:13:05.000000 django_auditor_logs-1.0.3/setup.py
+drwxr-xr-x   0 yeison    (1000) yeison    (1000)        0 2023-07-13 16:31:00.330710 django_auditor_logs-1.0.3/src/
+drwxr-xr-x   0 yeison    (1000) yeison    (1000)        0 2023-07-13 16:31:00.334710 django_auditor_logs-1.0.3/src/django_auditor_logs/
+-rw-r--r--   0 yeison    (1000) yeison    (1000)        0 2023-02-14 13:12:01.000000 django_auditor_logs-1.0.3/src/django_auditor_logs/__init__.py
+-rw-r--r--   0 yeison    (1000) yeison    (1000)       63 2023-02-14 13:12:01.000000 django_auditor_logs-1.0.3/src/django_auditor_logs/admin.py
+-rw-r--r--   0 yeison    (1000) yeison    (1000)      161 2023-07-13 16:29:40.000000 django_auditor_logs-1.0.3/src/django_auditor_logs/apps.py
+-rw-r--r--   0 yeison    (1000) yeison    (1000)      477 2023-02-19 00:24:31.000000 django_auditor_logs-1.0.3/src/django_auditor_logs/metadata.py
+drwxr-xr-x   0 yeison    (1000) yeison    (1000)        0 2023-07-13 16:31:00.338710 django_auditor_logs-1.0.3/src/django_auditor_logs/middleware/
+-rw-r--r--   0 yeison    (1000) yeison    (1000)        0 2023-02-19 00:14:15.000000 django_auditor_logs-1.0.3/src/django_auditor_logs/middleware/__init__.py
+-rw-r--r--   0 yeison    (1000) yeison    (1000)     1654 2023-02-19 00:37:05.000000 django_auditor_logs-1.0.3/src/django_auditor_logs/middleware/metadata_middleware.py
+-rw-r--r--   0 yeison    (1000) yeison    (1000)     5572 2023-02-19 00:46:19.000000 django_auditor_logs-1.0.3/src/django_auditor_logs/models.py
+-rw-r--r--   0 yeison    (1000) yeison    (1000)       60 2023-02-14 13:12:01.000000 django_auditor_logs-1.0.3/src/django_auditor_logs/tests.py
+-rw-r--r--   0 yeison    (1000) yeison    (1000)      108 2023-02-18 02:29:14.000000 django_auditor_logs-1.0.3/src/django_auditor_logs/views.py
+drwxr-xr-x   0 yeison    (1000) yeison    (1000)        0 2023-07-13 16:31:00.338710 django_auditor_logs-1.0.3/src/django_auditor_logs.egg-info/
+-rw-r--r--   0 yeison    (1000) yeison    (1000)     2248 2023-07-13 16:31:00.000000 django_auditor_logs-1.0.3/src/django_auditor_logs.egg-info/PKG-INFO
+-rw-r--r--   0 yeison    (1000) yeison    (1000)      648 2023-07-13 16:31:00.000000 django_auditor_logs-1.0.3/src/django_auditor_logs.egg-info/SOURCES.txt
+-rw-r--r--   0 yeison    (1000) yeison    (1000)        1 2023-07-13 16:31:00.000000 django_auditor_logs-1.0.3/src/django_auditor_logs.egg-info/dependency_links.txt
+-rw-r--r--   0 yeison    (1000) yeison    (1000)       12 2023-07-13 16:31:00.000000 django_auditor_logs-1.0.3/src/django_auditor_logs.egg-info/requires.txt
+-rw-r--r--   0 yeison    (1000) yeison    (1000)       20 2023-07-13 16:31:00.000000 django_auditor_logs-1.0.3/src/django_auditor_logs.egg-info/top_level.txt
```

### Comparing `django_auditor_logs-1.0.2/PKG-INFO` & `django_auditor_logs-1.0.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django_auditor_logs
-Version: 1.0.2
+Version: 1.0.3
 Summary: Package for easy creation of audit logs in Django projects
 Home-page: https://90horasporsemana.com
 Author: Yeison Fernandez
 Author-email: contacto@90horasporsemana.com
 License: MIT
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -63,7 +63,9 @@
 
     * 1.0.0
         - Initial release.
     * 1.0.1
         - Replace decorator and __user_metadata__ and __request_metadata__ fields by a MetadataManager class used in a Middleware.
     * 1.0.2
         - Fix documentation of the middleware.
+    * 1.0.3
+        - Fix WARNING default_auto_field.
```

### Comparing `django_auditor_logs-1.0.2/README.md` & `django_auditor_logs-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `django_auditor_logs-1.0.2/quickstart.rst` & `django_auditor_logs-1.0.3/quickstart.rst`

 * *Files 2% similar despite different names*

```diff
@@ -46,8 +46,10 @@
 --------------------------------
 
     * 1.0.0
         - Initial release.
     * 1.0.1
         - Replace decorator and __user_metadata__ and __request_metadata__ fields by a MetadataManager class used in a Middleware.
     * 1.0.2
-        - Fix documentation of the middleware.
+        - Fix documentation of the middleware.
+    * 1.0.3
+        - Fix WARNING default_auto_field.
```

### Comparing `django_auditor_logs-1.0.2/setup.cfg` & `django_auditor_logs-1.0.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django_auditor_logs
-version = 1.0.2
+version = 1.0.3
 description = Package for easy creation of audit logs in Django projects
 long_description = file:./quickstart.rst
 url = https://90horasporsemana.com
 author = Yeison Fernandez
 author_email = contacto@90horasporsemana.com
 license = MIT
 classifiers =
```

### Comparing `django_auditor_logs-1.0.2/src/django_auditor_logs/middleware/metadata_middleware.py` & `django_auditor_logs-1.0.3/src/django_auditor_logs/middleware/metadata_middleware.py`

 * *Files identical despite different names*

### Comparing `django_auditor_logs-1.0.2/src/django_auditor_logs/models.py` & `django_auditor_logs-1.0.3/src/django_auditor_logs/models.py`

 * *Files identical despite different names*

### Comparing `django_auditor_logs-1.0.2/src/django_auditor_logs.egg-info/PKG-INFO` & `django_auditor_logs-1.0.3/src/django_auditor_logs.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-auditor-logs
-Version: 1.0.2
+Version: 1.0.3
 Summary: Package for easy creation of audit logs in Django projects
 Home-page: https://90horasporsemana.com
 Author: Yeison Fernandez
 Author-email: contacto@90horasporsemana.com
 License: MIT
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -63,7 +63,9 @@
 
     * 1.0.0
         - Initial release.
     * 1.0.1
         - Replace decorator and __user_metadata__ and __request_metadata__ fields by a MetadataManager class used in a Middleware.
     * 1.0.2
         - Fix documentation of the middleware.
+    * 1.0.3
+        - Fix WARNING default_auto_field.
```

### Comparing `django_auditor_logs-1.0.2/src/django_auditor_logs.egg-info/SOURCES.txt` & `django_auditor_logs-1.0.3/src/django_auditor_logs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

