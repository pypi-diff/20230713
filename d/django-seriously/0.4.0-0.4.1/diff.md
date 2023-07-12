# Comparing `tmp/django-seriously-0.4.0.tar.gz` & `tmp/django-seriously-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-seriously-0.4.0.tar", last modified: Sun Dec 18 23:14:15 2022, max compression
+gzip compressed data, was "django-seriously-0.4.1.tar", last modified: Wed Jul 12 22:54:44 2023, max compression
```

## Comparing `django-seriously-0.4.0.tar` & `django-seriously-0.4.1.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-18 23:14:15.710547 django-seriously-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1517 2022-12-18 23:13:59.000000 django-seriously-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      193 2022-12-18 23:13:59.000000 django-seriously-0.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6777 2022-12-18 23:14:15.706547 django-seriously-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5636 2022-12-18 23:13:59.000000 django-seriously-0.4.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-18 23:14:15.702547 django-seriously-0.4.0/django_seriously/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2022-12-18 23:13:59.000000 django-seriously-0.4.0/django_seriously/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-18 23:14:15.702547 django-seriously-0.4.0/django_seriously/authtoken/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-18 23:13:59.000000 django-seriously-0.4.0/django_seriously/authtoken/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2022-12-18 23:13:59.000000 django-seriously-0.4.0/django_seriously/authtoken/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)      167 2022-12-18 23:13:59.000000 django-seriously-0.4.0/django_seriously/authtoken/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     3957 2022-12-18 23:13:59.000000 django-seriously-0.4.0/django_seriously/authtoken/authentication.py
--rw-r--r--   0 runner    (1001) docker     (123)      338 2022-12-18 23:13:59.000000 django-seriously-0.4.0/django_seriously/authtoken/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-18 23:14:15.706547 django-seriously-0.4.0/django_seriously/authtoken/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2022-12-18 23:13:59.000000 django-seriously-0.4.0/django_seriously/authtoken/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)      681 2022-12-18 23:13:59.000000 django-seriously-0.4.0/django_seriously/authtoken/migrations/0002_token_last_seen_at_alter_token_scopes.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-18 23:13:59.000000 django-seriously-0.4.0/django_seriously/authtoken/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1836 2022-12-18 23:13:59.000000 django-seriously-0.4.0/django_seriously/authtoken/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2022-12-18 23:13:59.000000 django-seriously-0.4.0/django_seriously/authtoken/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-18 23:14:15.706547 django-seriously-0.4.0/django_seriously/minimaluser/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-18 23:13:59.000000 django-seriously-0.4.0/django_seriously/minimaluser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3302 2022-12-18 23:13:59.000000 django-seriously-0.4.0/django_seriously/minimaluser/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)      171 2022-12-18 23:13:59.000000 django-seriously-0.4.0/django_seriously/minimaluser/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     2942 2022-12-18 23:13:59.000000 django-seriously-0.4.0/django_seriously/minimaluser/models.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-18 23:13:59.000000 django-seriously-0.4.0/django_seriously/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      445 2022-12-18 23:13:59.000000 django-seriously-0.4.0/django_seriously/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-18 23:14:15.706547 django-seriously-0.4.0/django_seriously/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-18 23:13:59.000000 django-seriously-0.4.0/django_seriously/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4836 2022-12-18 23:13:59.000000 django-seriously-0.4.0/django_seriously/utils/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3088 2022-12-18 23:13:59.000000 django-seriously-0.4.0/django_seriously/utils/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2022-12-18 23:13:59.000000 django-seriously-0.4.0/django_seriously/utils/forms.py
--rw-r--r--   0 runner    (1001) docker     (123)      699 2022-12-18 23:13:59.000000 django-seriously-0.4.0/django_seriously/utils/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2027 2022-12-18 23:13:59.000000 django-seriously-0.4.0/django_seriously/utils/pydantic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2022-12-18 23:13:59.000000 django-seriously-0.4.0/django_seriously/utils/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     1705 2022-12-18 23:13:59.000000 django-seriously-0.4.0/django_seriously/utils/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-18 23:14:15.702547 django-seriously-0.4.0/django_seriously.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6777 2022-12-18 23:14:15.000000 django-seriously-0.4.0/django_seriously.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1561 2022-12-18 23:14:15.000000 django-seriously-0.4.0/django_seriously.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-18 23:14:15.000000 django-seriously-0.4.0/django_seriously.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       84 2022-12-18 23:14:15.000000 django-seriously-0.4.0/django_seriously.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)      134 2022-12-18 23:14:15.000000 django-seriously-0.4.0/django_seriously.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      311 2022-12-18 23:13:59.000000 django-seriously-0.4.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-18 23:14:15.706547 django-seriously-0.4.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2022-12-18 23:13:59.000000 django-seriously-0.4.0/requirements/base.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2022-12-18 23:13:59.000000 django-seriously-0.4.0/requirements/optionals.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2022-12-18 23:13:59.000000 django-seriously-0.4.0/requirements/packaging.txt
--rw-r--r--   0 runner    (1001) docker     (123)      160 2022-12-18 23:13:59.000000 django-seriously-0.4.0/requirements/testing.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-18 23:14:15.710547 django-seriously-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3342 2022-12-18 23:13:59.000000 django-seriously-0.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-18 23:14:15.706547 django-seriously-0.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-18 23:13:59.000000 django-seriously-0.4.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2913 2022-12-18 23:13:59.000000 django-seriously-0.4.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-18 23:13:59.000000 django-seriously-0.4.0/tests/models.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-18 23:13:59.000000 django-seriously-0.4.0/tests/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-18 23:13:59.000000 django-seriously-0.4.0/tests/test_adminitemaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     2372 2022-12-18 23:13:59.000000 django-seriously-0.4.0/tests/test_authtoken.py
--rw-r--r--   0 runner    (1001) docker     (123)      760 2022-12-18 23:13:59.000000 django-seriously-0.4.0/tests/test_base_model.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-18 23:13:59.000000 django-seriously-0.4.0/tests/test_minimaluser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1980 2022-12-18 23:13:59.000000 django-seriously-0.4.0/tests/test_pydantic_field.py
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2022-12-18 23:13:59.000000 django-seriously-0.4.0/tests/test_validated_field.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2022-12-18 23:13:59.000000 django-seriously-0.4.0/tests/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 22:54:44.256696 django-seriously-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-07-12 22:54:31.000000 django-seriously-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-07-12 22:54:31.000000 django-seriously-0.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6777 2023-07-12 22:54:44.256696 django-seriously-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5636 2023-07-12 22:54:31.000000 django-seriously-0.4.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 22:54:44.252696 django-seriously-0.4.1/django_seriously/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-12 22:54:31.000000 django-seriously-0.4.1/django_seriously/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 22:54:44.252696 django-seriously-0.4.1/django_seriously/authtoken/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 22:54:31.000000 django-seriously-0.4.1/django_seriously/authtoken/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-07-12 22:54:31.000000 django-seriously-0.4.1/django_seriously/authtoken/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-07-12 22:54:31.000000 django-seriously-0.4.1/django_seriously/authtoken/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4136 2023-07-12 22:54:31.000000 django-seriously-0.4.1/django_seriously/authtoken/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-07-12 22:54:31.000000 django-seriously-0.4.1/django_seriously/authtoken/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 22:54:44.252696 django-seriously-0.4.1/django_seriously/authtoken/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-07-12 22:54:31.000000 django-seriously-0.4.1/django_seriously/authtoken/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-07-12 22:54:31.000000 django-seriously-0.4.1/django_seriously/authtoken/migrations/0002_token_last_seen_at_alter_token_scopes.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 22:54:31.000000 django-seriously-0.4.1/django_seriously/authtoken/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-07-12 22:54:31.000000 django-seriously-0.4.1/django_seriously/authtoken/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-07-12 22:54:31.000000 django-seriously-0.4.1/django_seriously/authtoken/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 22:54:44.256696 django-seriously-0.4.1/django_seriously/minimaluser/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 22:54:31.000000 django-seriously-0.4.1/django_seriously/minimaluser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3302 2023-07-12 22:54:31.000000 django-seriously-0.4.1/django_seriously/minimaluser/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-07-12 22:54:31.000000 django-seriously-0.4.1/django_seriously/minimaluser/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-07-12 22:54:31.000000 django-seriously-0.4.1/django_seriously/minimaluser/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 22:54:31.000000 django-seriously-0.4.1/django_seriously/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-07-12 22:54:31.000000 django-seriously-0.4.1/django_seriously/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 22:54:44.256696 django-seriously-0.4.1/django_seriously/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 22:54:31.000000 django-seriously-0.4.1/django_seriously/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4903 2023-07-12 22:54:31.000000 django-seriously-0.4.1/django_seriously/utils/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3088 2023-07-12 22:54:31.000000 django-seriously-0.4.1/django_seriously/utils/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-07-12 22:54:31.000000 django-seriously-0.4.1/django_seriously/utils/forms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-12 22:54:31.000000 django-seriously-0.4.1/django_seriously/utils/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-07-12 22:54:31.000000 django-seriously-0.4.1/django_seriously/utils/pydantic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-07-12 22:54:31.000000 django-seriously-0.4.1/django_seriously/utils/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-07-12 22:54:31.000000 django-seriously-0.4.1/django_seriously/utils/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 22:54:44.252696 django-seriously-0.4.1/django_seriously.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6777 2023-07-12 22:54:44.000000 django-seriously-0.4.1/django_seriously.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-07-12 22:54:44.000000 django-seriously-0.4.1/django_seriously.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 22:54:44.000000 django-seriously-0.4.1/django_seriously.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-12 22:54:44.000000 django-seriously-0.4.1/django_seriously.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-12 22:54:44.000000 django-seriously-0.4.1/django_seriously.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-12 22:54:31.000000 django-seriously-0.4.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 22:54:44.256696 django-seriously-0.4.1/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-12 22:54:31.000000 django-seriously-0.4.1/requirements/base.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-12 22:54:31.000000 django-seriously-0.4.1/requirements/optionals.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-12 22:54:31.000000 django-seriously-0.4.1/requirements/packaging.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-12 22:54:31.000000 django-seriously-0.4.1/requirements/testing.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 22:54:44.256696 django-seriously-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3342 2023-07-12 22:54:31.000000 django-seriously-0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 22:54:44.256696 django-seriously-0.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 22:54:31.000000 django-seriously-0.4.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-07-12 22:54:31.000000 django-seriously-0.4.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 22:54:31.000000 django-seriously-0.4.1/tests/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 22:54:31.000000 django-seriously-0.4.1/tests/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 22:54:31.000000 django-seriously-0.4.1/tests/test_adminitemaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-07-12 22:54:31.000000 django-seriously-0.4.1/tests/test_authtoken.py
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-07-12 22:54:31.000000 django-seriously-0.4.1/tests/test_base_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 22:54:31.000000 django-seriously-0.4.1/tests/test_minimaluser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-07-12 22:54:31.000000 django-seriously-0.4.1/tests/test_pydantic_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-07-12 22:54:31.000000 django-seriously-0.4.1/tests/test_validated_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-12 22:54:31.000000 django-seriously-0.4.1/tests/urls.py
```

### Comparing `django-seriously-0.4.0/LICENSE` & `django-seriously-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-seriously-0.4.0/PKG-INFO` & `django-seriously-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-seriously
-Version: 0.4.0
+Version: 0.4.1
 Summary: Opinionated collection of Django and DRF tools that came in handy time and again.
 Home-page: https://github.com/tfranzel/django-seriously
 Author: T. Franzel
 Author-email: tfranzel@gmail.com
 License: BSD
 Project-URL: Source, https://github.com/tfranzel/django-seriously
 Classifier: Development Status :: 4 - Beta
```

### Comparing `django-seriously-0.4.0/README.rst` & `django-seriously-0.4.1/README.rst`

 * *Files identical despite different names*

### Comparing `django-seriously-0.4.0/django_seriously/authtoken/admin.py` & `django-seriously-0.4.1/django_seriously/authtoken/admin.py`

 * *Files identical despite different names*

### Comparing `django-seriously-0.4.0/django_seriously/authtoken/authentication.py` & `django-seriously-0.4.1/django_seriously/authtoken/authentication.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,14 +77,18 @@
 
         if not token.user.is_active:
             raise exceptions.AuthenticationFailed(_("User inactive or deleted."))
 
         token.last_seen_at = timezone.now()
         token.save(update_fields=["last_seen_at"])
 
+        if seriously_settings.CHECK_PASSWORD_REHASH(token.key):
+            token.key = seriously_settings.MAKE_PASSWORD(raw_token)
+            token.save(update_fields=["key"])
+
         return token.user, token
 
     def check_expiration(self, token: "Token"):
         """user method that handles expired tokens"""
         return True
 
     def authenticate_header(self, request):
```

### Comparing `django-seriously-0.4.0/django_seriously/authtoken/migrations/0001_initial.py` & `django-seriously-0.4.1/django_seriously/authtoken/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-seriously-0.4.0/django_seriously/authtoken/migrations/0002_token_last_seen_at_alter_token_scopes.py` & `django-seriously-0.4.1/django_seriously/authtoken/migrations/0002_token_last_seen_at_alter_token_scopes.py`

 * *Files identical despite different names*

### Comparing `django-seriously-0.4.0/django_seriously/authtoken/models.py` & `django-seriously-0.4.1/django_seriously/authtoken/models.py`

 * *Files identical despite different names*

### Comparing `django-seriously-0.4.0/django_seriously/minimaluser/admin.py` & `django-seriously-0.4.1/django_seriously/minimaluser/admin.py`

 * *Files identical despite different names*

### Comparing `django-seriously-0.4.0/django_seriously/minimaluser/models.py` & `django-seriously-0.4.1/django_seriously/minimaluser/models.py`

 * *Files identical despite different names*

### Comparing `django-seriously-0.4.0/django_seriously/utils/admin.py` & `django-seriously-0.4.1/django_seriously/utils/admin.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import abc
-from typing import Any, Generic, Optional, Type, TypeVar
+from typing import Any, Generic, Optional, Type, TypeVar, Union
 
 from django.contrib import messages
 from django.contrib.auth.mixins import AccessMixin
 from django.db import models, transaction
 from django.http.response import HttpResponse, JsonResponse
 from django.urls.base import reverse
 from django.urls.conf import include, path
+from django.utils.functional import Promise
 from django.utils.html import format_html
 from django.utils.safestring import mark_safe
 from django.utils.translation import gettext_lazy as _
 from django.views.generic.base import View
 
 _T = TypeVar("_T", bound=models.Model)
 
@@ -76,15 +77,15 @@
     @classmethod
     def action_markup(cls, obj: _T):
         return mark_safe(
             " ".join([cls._action(obj, action, label) for action, label in cls.actions])
         )
 
     @classmethod
-    def _action(cls, obj: _T, action: str, label: str):
+    def _action(cls, obj: _T, action: str, label: Union[str, Promise]):
         """template rendering of action"""
         if not cls.is_actionable(obj, action):
             return ""
 
         return format_html(
             """
             <a class="button" href="#" style="white-space: nowrap" onclick="
```

### Comparing `django-seriously-0.4.0/django_seriously/utils/fields.py` & `django-seriously-0.4.1/django_seriously/utils/fields.py`

 * *Files identical despite different names*

### Comparing `django-seriously-0.4.0/django_seriously/utils/forms.py` & `django-seriously-0.4.1/django_seriously/utils/forms.py`

 * *Files identical despite different names*

### Comparing `django-seriously-0.4.0/django_seriously/utils/models.py` & `django-seriously-0.4.1/django_seriously/utils/models.py`

 * *Files identical despite different names*

### Comparing `django-seriously-0.4.0/django_seriously/utils/pydantic.py` & `django-seriously-0.4.1/django_seriously/utils/pydantic.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import json
 from typing import Any
 
+from django import VERSION as DJANGO_VERSION
 from django.core import exceptions
 from pydantic import BaseModel, ValidationError, parse_obj_as, parse_raw_as
 
 
 def _build_container(structure, *, json_loads=None, json_dumps=None):
     loads_callable = json_loads or json.loads
     dumps_callable = json_dumps or json.dumps
@@ -28,15 +29,20 @@
 
 def pydantic_dumps(structure, value: Any, *, json_dumps=None, encoder=None) -> str:
     try:
         if _is_pydantic(value) and not json_dumps:
             obj = value
         else:
             obj = _build_container(structure, json_dumps=json_dumps)(__root__=value)
-        return obj.json()
+
+        if DJANGO_VERSION < (4, 2):
+            return obj.json()
+        else:
+            obj = obj.dict()
+            return obj["__root__"] if "__root__" in obj else obj
     except ValidationError as e:
         raise exceptions.ValidationError(f"Invalid type structure for {structure}: {e}")
 
 
 def pydantic_loads(structure, value: Any, *, json_loads=None, decoder=None) -> Any:
     try:
         if json_loads:
```

### Comparing `django-seriously-0.4.0/django_seriously/utils/schema.py` & `django-seriously-0.4.1/django_seriously/utils/schema.py`

 * *Files identical despite different names*

### Comparing `django-seriously-0.4.0/django_seriously/utils/settings.py` & `django-seriously-0.4.1/django_seriously/utils/settings.py`

 * *Files identical despite different names*

### Comparing `django-seriously-0.4.0/django_seriously.egg-info/PKG-INFO` & `django-seriously-0.4.1/django_seriously.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-seriously
-Version: 0.4.0
+Version: 0.4.1
 Summary: Opinionated collection of Django and DRF tools that came in handy time and again.
 Home-page: https://github.com/tfranzel/django-seriously
 Author: T. Franzel
 Author-email: tfranzel@gmail.com
 License: BSD
 Project-URL: Source, https://github.com/tfranzel/django-seriously
 Classifier: Development Status :: 4 - Beta
```

### Comparing `django-seriously-0.4.0/django_seriously.egg-info/SOURCES.txt` & `django-seriously-0.4.1/django_seriously.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-seriously-0.4.0/setup.py` & `django-seriously-0.4.1/setup.py`

 * *Files identical despite different names*

### Comparing `django-seriously-0.4.0/tests/conftest.py` & `django-seriously-0.4.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `django-seriously-0.4.0/tests/test_base_model.py` & `django-seriously-0.4.1/tests/test_base_model.py`

 * *Files identical despite different names*

### Comparing `django-seriously-0.4.0/tests/test_pydantic_field.py` & `django-seriously-0.4.1/tests/test_pydantic_field.py`

 * *Files identical despite different names*

### Comparing `django-seriously-0.4.0/tests/test_validated_field.py` & `django-seriously-0.4.1/tests/test_validated_field.py`

 * *Files identical despite different names*

