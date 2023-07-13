# Comparing `tmp/django-url-tokenizer-0.0.7.tar.gz` & `tmp/django-url-tokenizer-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-url-tokenizer-0.0.7.tar", last modified: Thu Jul 13 05:57:09 2023, max compression
+gzip compressed data, was "django-url-tokenizer-0.0.8.tar", last modified: Thu Jul 13 06:17:38 2023, max compression
```

## Comparing `django-url-tokenizer-0.0.7.tar` & `django-url-tokenizer-0.0.8.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 nibblex   (1000) nibblex   (1000)        0 2023-07-13 05:57:09.412035 django-url-tokenizer-0.0.7/
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)     1074 2023-07-13 01:29:20.000000 django-url-tokenizer-0.0.7/LICENSE
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)      441 2023-07-13 05:57:09.412035 django-url-tokenizer-0.0.7/PKG-INFO
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)      144 2023-07-13 01:29:20.000000 django-url-tokenizer-0.0.7/README.md
-drwxr-xr-x   0 nibblex   (1000) nibblex   (1000)        0 2023-07-13 05:57:09.412035 django-url-tokenizer-0.0.7/django_url_tokenizer.egg-info/
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)      441 2023-07-13 05:57:09.000000 django-url-tokenizer-0.0.7/django_url_tokenizer.egg-info/PKG-INFO
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)      448 2023-07-13 05:57:09.000000 django-url-tokenizer-0.0.7/django_url_tokenizer.egg-info/SOURCES.txt
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)        1 2023-07-13 05:57:09.000000 django-url-tokenizer-0.0.7/django_url_tokenizer.egg-info/dependency_links.txt
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)       41 2023-07-13 05:57:09.000000 django-url-tokenizer-0.0.7/django_url_tokenizer.egg-info/requires.txt
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)       13 2023-07-13 05:57:09.000000 django-url-tokenizer-0.0.7/django_url_tokenizer.egg-info/top_level.txt
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)       38 2023-07-13 05:57:09.412035 django-url-tokenizer-0.0.7/setup.cfg
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)      829 2023-07-13 05:55:16.000000 django-url-tokenizer-0.0.7/setup.py
-drwxr-xr-x   0 nibblex   (1000) nibblex   (1000)        0 2023-07-13 05:57:09.412035 django-url-tokenizer-0.0.7/urltokenizer/
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)        0 2023-07-13 00:48:39.000000 django-url-tokenizer-0.0.7/urltokenizer/__init__.py
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)      156 2023-07-13 00:48:39.000000 django-url-tokenizer-0.0.7/urltokenizer/apps.py
-drwxr-xr-x   0 nibblex   (1000) nibblex   (1000)        0 2023-07-13 05:57:09.412035 django-url-tokenizer-0.0.7/urltokenizer/migrations/
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)        0 2023-07-13 00:48:39.000000 django-url-tokenizer-0.0.7/urltokenizer/migrations/__init__.py
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)      716 2023-07-13 03:03:12.000000 django-url-tokenizer-0.0.7/urltokenizer/mixins.py
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)     1623 2023-07-13 05:54:17.000000 django-url-tokenizer-0.0.7/urltokenizer/serializers.py
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)       60 2023-07-13 00:48:39.000000 django-url-tokenizer-0.0.7/urltokenizer/tests.py
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)     4571 2023-07-13 04:44:48.000000 django-url-tokenizer-0.0.7/urltokenizer/tokenizer.py
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)      406 2023-07-13 00:52:10.000000 django-url-tokenizer-0.0.7/urltokenizer/views.py
+drwxr-xr-x   0 nibblex   (1000) nibblex   (1000)        0 2023-07-13 06:17:38.291848 django-url-tokenizer-0.0.8/
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)     1074 2023-07-13 01:29:20.000000 django-url-tokenizer-0.0.8/LICENSE
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)      441 2023-07-13 06:17:38.291848 django-url-tokenizer-0.0.8/PKG-INFO
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)      144 2023-07-13 01:29:20.000000 django-url-tokenizer-0.0.8/README.md
+drwxr-xr-x   0 nibblex   (1000) nibblex   (1000)        0 2023-07-13 06:17:38.291848 django-url-tokenizer-0.0.8/django_url_tokenizer.egg-info/
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)      441 2023-07-13 06:17:38.000000 django-url-tokenizer-0.0.8/django_url_tokenizer.egg-info/PKG-INFO
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)      448 2023-07-13 06:17:38.000000 django-url-tokenizer-0.0.8/django_url_tokenizer.egg-info/SOURCES.txt
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)        1 2023-07-13 06:17:38.000000 django-url-tokenizer-0.0.8/django_url_tokenizer.egg-info/dependency_links.txt
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)       41 2023-07-13 06:17:38.000000 django-url-tokenizer-0.0.8/django_url_tokenizer.egg-info/requires.txt
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)       13 2023-07-13 06:17:38.000000 django-url-tokenizer-0.0.8/django_url_tokenizer.egg-info/top_level.txt
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)       38 2023-07-13 06:17:38.291848 django-url-tokenizer-0.0.8/setup.cfg
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)      829 2023-07-13 06:14:53.000000 django-url-tokenizer-0.0.8/setup.py
+drwxr-xr-x   0 nibblex   (1000) nibblex   (1000)        0 2023-07-13 06:17:38.291848 django-url-tokenizer-0.0.8/urltokenizer/
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)        0 2023-07-13 00:48:39.000000 django-url-tokenizer-0.0.8/urltokenizer/__init__.py
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)      156 2023-07-13 00:48:39.000000 django-url-tokenizer-0.0.8/urltokenizer/apps.py
+drwxr-xr-x   0 nibblex   (1000) nibblex   (1000)        0 2023-07-13 06:17:38.291848 django-url-tokenizer-0.0.8/urltokenizer/migrations/
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)        0 2023-07-13 00:48:39.000000 django-url-tokenizer-0.0.8/urltokenizer/migrations/__init__.py
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)      716 2023-07-13 03:03:12.000000 django-url-tokenizer-0.0.8/urltokenizer/mixins.py
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)     1506 2023-07-13 06:17:13.000000 django-url-tokenizer-0.0.8/urltokenizer/serializers.py
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)       60 2023-07-13 00:48:39.000000 django-url-tokenizer-0.0.8/urltokenizer/tests.py
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)     4609 2023-07-13 06:15:21.000000 django-url-tokenizer-0.0.8/urltokenizer/tokenizer.py
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)      406 2023-07-13 00:52:10.000000 django-url-tokenizer-0.0.8/urltokenizer/views.py
```

### Comparing `django-url-tokenizer-0.0.7/LICENSE` & `django-url-tokenizer-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `django-url-tokenizer-0.0.7/setup.py` & `django-url-tokenizer-0.0.8/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setuptools.setup(
     name="django-url-tokenizer",
-    version="0.0.7",
+    version="0.0.8",
     author="Sergio Rodríguez",
     author_email="srodriguez3441@gmail.com",
     description="""A python package that provides a Django app that allows you to
     generate tokenized urls and send them to users via email.""",
     url="https://github.com/nibblex/django-url-tokenizer",
     packages=setuptools.find_packages(),
     license="MIT",
```

### Comparing `django-url-tokenizer-0.0.7/urltokenizer/mixins.py` & `django-url-tokenizer-0.0.8/urltokenizer/mixins.py`

 * *Files identical despite different names*

### Comparing `django-url-tokenizer-0.0.7/urltokenizer/serializers.py` & `django-url-tokenizer-0.0.8/urltokenizer/serializers.py`

 * *Files 19% similar despite different names*

```diff
@@ -32,20 +32,17 @@
     token = serializers.CharField(required=True)
     extra_data = serializers.JSONField(required=False, write_only=True)
 
     def create(self, validated_data):
         token_type = self.context["view"].kwargs["type"]
         tokenizer = Tokenizer(token_type)
 
-        try:
-            user = tokenizer.check_token(
-                validated_data["uidb64"],
-                validated_data["token"],
-                **validated_data.get("extra_data", {})
-            )
-        except Exception as e:
-            raise serializers.ValidationError from e
+        user = tokenizer.check_token(
+            validated_data["uidb64"],
+            validated_data["token"],
+            **validated_data.get("extra_data", {})
+        )
 
         if not user:
             raise AuthenticationFailed(_("invalid token"))
 
         return validated_data
```

### Comparing `django-url-tokenizer-0.0.7/urltokenizer/tokenizer.py` & `django-url-tokenizer-0.0.8/urltokenizer/tokenizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 from enum import Enum
 from typing import Any
 
 from django.conf import settings
 from django.contrib.auth import get_user_model
 from django.contrib.auth.tokens import PasswordResetTokenGenerator
-from django.core.exceptions import ValidationError, ImproperlyConfigured
+from django.core.exceptions import ImproperlyConfigured
 from django.core.mail import send_mail
 from django.utils.encoding import force_bytes, force_str, DjangoUnicodeDecodeError
 from django.utils.http import urlsafe_base64_encode, urlsafe_base64_decode
 from django.utils.translation import gettext_lazy as _
 
+from rest_framework.exceptions import ValidationError
+
 
 class TokenGenerator(PasswordResetTokenGenerator):
     def __init__(self, token_config):
         self.token_config = token_config
         super().__init__()
 
     def _make_hash_value(self, user, timestamp):
```

