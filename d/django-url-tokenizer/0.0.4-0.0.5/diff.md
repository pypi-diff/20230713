# Comparing `tmp/django-url-tokenizer-0.0.4.tar.gz` & `tmp/django-url-tokenizer-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-url-tokenizer-0.0.4.tar", last modified: Thu Jul 13 03:05:46 2023, max compression
+gzip compressed data, was "django-url-tokenizer-0.0.5.tar", last modified: Thu Jul 13 03:54:13 2023, max compression
```

## Comparing `django-url-tokenizer-0.0.4.tar` & `django-url-tokenizer-0.0.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 nibblex   (1000) nibblex   (1000)        0 2023-07-13 03:05:46.443261 django-url-tokenizer-0.0.4/
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)     1074 2023-07-13 01:29:20.000000 django-url-tokenizer-0.0.4/LICENSE
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)      441 2023-07-13 03:05:46.443261 django-url-tokenizer-0.0.4/PKG-INFO
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)      144 2023-07-13 01:29:20.000000 django-url-tokenizer-0.0.4/README.md
-drwxr-xr-x   0 nibblex   (1000) nibblex   (1000)        0 2023-07-13 03:05:46.443261 django-url-tokenizer-0.0.4/django_url_tokenizer.egg-info/
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)      441 2023-07-13 03:05:46.000000 django-url-tokenizer-0.0.4/django_url_tokenizer.egg-info/PKG-INFO
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)      448 2023-07-13 03:05:46.000000 django-url-tokenizer-0.0.4/django_url_tokenizer.egg-info/SOURCES.txt
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)        1 2023-07-13 03:05:46.000000 django-url-tokenizer-0.0.4/django_url_tokenizer.egg-info/dependency_links.txt
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)       41 2023-07-13 03:05:46.000000 django-url-tokenizer-0.0.4/django_url_tokenizer.egg-info/requires.txt
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)       13 2023-07-13 03:05:46.000000 django-url-tokenizer-0.0.4/django_url_tokenizer.egg-info/top_level.txt
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)       38 2023-07-13 03:05:46.443261 django-url-tokenizer-0.0.4/setup.cfg
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)      829 2023-07-13 03:04:37.000000 django-url-tokenizer-0.0.4/setup.py
-drwxr-xr-x   0 nibblex   (1000) nibblex   (1000)        0 2023-07-13 03:05:46.443261 django-url-tokenizer-0.0.4/urltokenizer/
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)        0 2023-07-13 00:48:39.000000 django-url-tokenizer-0.0.4/urltokenizer/__init__.py
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)      156 2023-07-13 00:48:39.000000 django-url-tokenizer-0.0.4/urltokenizer/apps.py
-drwxr-xr-x   0 nibblex   (1000) nibblex   (1000)        0 2023-07-13 03:05:46.443261 django-url-tokenizer-0.0.4/urltokenizer/migrations/
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)        0 2023-07-13 00:48:39.000000 django-url-tokenizer-0.0.4/urltokenizer/migrations/__init__.py
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)      716 2023-07-13 03:03:12.000000 django-url-tokenizer-0.0.4/urltokenizer/mixins.py
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)     1485 2023-07-13 00:51:13.000000 django-url-tokenizer-0.0.4/urltokenizer/serializers.py
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)       60 2023-07-13 00:48:39.000000 django-url-tokenizer-0.0.4/urltokenizer/tests.py
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)     4548 2023-07-13 00:51:53.000000 django-url-tokenizer-0.0.4/urltokenizer/tokenizer.py
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)      406 2023-07-13 00:52:10.000000 django-url-tokenizer-0.0.4/urltokenizer/views.py
+drwxr-xr-x   0 nibblex   (1000) nibblex   (1000)        0 2023-07-13 03:54:13.743154 django-url-tokenizer-0.0.5/
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)     1074 2023-07-13 01:29:20.000000 django-url-tokenizer-0.0.5/LICENSE
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)      441 2023-07-13 03:54:13.743154 django-url-tokenizer-0.0.5/PKG-INFO
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)      144 2023-07-13 01:29:20.000000 django-url-tokenizer-0.0.5/README.md
+drwxr-xr-x   0 nibblex   (1000) nibblex   (1000)        0 2023-07-13 03:54:13.743154 django-url-tokenizer-0.0.5/django_url_tokenizer.egg-info/
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)      441 2023-07-13 03:54:13.000000 django-url-tokenizer-0.0.5/django_url_tokenizer.egg-info/PKG-INFO
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)      448 2023-07-13 03:54:13.000000 django-url-tokenizer-0.0.5/django_url_tokenizer.egg-info/SOURCES.txt
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)        1 2023-07-13 03:54:13.000000 django-url-tokenizer-0.0.5/django_url_tokenizer.egg-info/dependency_links.txt
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)       41 2023-07-13 03:54:13.000000 django-url-tokenizer-0.0.5/django_url_tokenizer.egg-info/requires.txt
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)       13 2023-07-13 03:54:13.000000 django-url-tokenizer-0.0.5/django_url_tokenizer.egg-info/top_level.txt
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)       38 2023-07-13 03:54:13.743154 django-url-tokenizer-0.0.5/setup.cfg
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)      829 2023-07-13 03:51:15.000000 django-url-tokenizer-0.0.5/setup.py
+drwxr-xr-x   0 nibblex   (1000) nibblex   (1000)        0 2023-07-13 03:54:13.743154 django-url-tokenizer-0.0.5/urltokenizer/
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)        0 2023-07-13 00:48:39.000000 django-url-tokenizer-0.0.5/urltokenizer/__init__.py
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)      156 2023-07-13 00:48:39.000000 django-url-tokenizer-0.0.5/urltokenizer/apps.py
+drwxr-xr-x   0 nibblex   (1000) nibblex   (1000)        0 2023-07-13 03:54:13.743154 django-url-tokenizer-0.0.5/urltokenizer/migrations/
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)        0 2023-07-13 00:48:39.000000 django-url-tokenizer-0.0.5/urltokenizer/migrations/__init__.py
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)      716 2023-07-13 03:03:12.000000 django-url-tokenizer-0.0.5/urltokenizer/mixins.py
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)     1485 2023-07-13 00:51:13.000000 django-url-tokenizer-0.0.5/urltokenizer/serializers.py
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)       60 2023-07-13 00:48:39.000000 django-url-tokenizer-0.0.5/urltokenizer/tests.py
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)     4548 2023-07-13 03:50:45.000000 django-url-tokenizer-0.0.5/urltokenizer/tokenizer.py
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)      406 2023-07-13 00:52:10.000000 django-url-tokenizer-0.0.5/urltokenizer/views.py
```

### Comparing `django-url-tokenizer-0.0.4/LICENSE` & `django-url-tokenizer-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `django-url-tokenizer-0.0.4/setup.py` & `django-url-tokenizer-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setuptools.setup(
     name="django-url-tokenizer",
-    version="0.0.4",
+    version="0.0.5",
     author="Sergio Rodríguez",
     author_email="srodriguez3441@gmail.com",
     description="""A python package that provides a Django app that allows you to
     generate tokenized urls and send them to users via email.""",
     url="https://github.com/nibblex/django-url-tokenizer",
     packages=setuptools.find_packages(),
     license="MIT",
```

### Comparing `django-url-tokenizer-0.0.4/urltokenizer/mixins.py` & `django-url-tokenizer-0.0.5/urltokenizer/mixins.py`

 * *Files identical despite different names*

### Comparing `django-url-tokenizer-0.0.4/urltokenizer/serializers.py` & `django-url-tokenizer-0.0.5/urltokenizer/serializers.py`

 * *Files identical despite different names*

### Comparing `django-url-tokenizer-0.0.4/urltokenizer/tokenizer.py` & `django-url-tokenizer-0.0.5/urltokenizer/tokenizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,18 +47,18 @@
                 method(**kwargs)
             except Exception as e:
                 raise ValidationError(_("failed to execute callback")) from e
 
 
 class Tokenizer:
     def __init__(self, token_type: str | Enum):
-        SETTINGS = getattr(settings, "TOKENIZATION_SETTINGS", None)
+        SETTINGS = getattr(settings, "URLTOKENIZER_SETTINGS", None)
         if not SETTINGS:
             raise ValidationError(
-                _("TOKENIZATION_SETTINGS must be defined in settings.py")
+                _("URLTOKENIZER_SETTINGS must be defined in settings.py")
             )
 
         self.token_type = (
             token_type.value if isinstance(token_type, Enum) else token_type
         )
         self._settings = SETTINGS
         self._token_generator = self._get_token_generator(self.token_type, SETTINGS)
```

