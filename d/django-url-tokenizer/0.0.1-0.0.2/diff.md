# Comparing `tmp/django-url-tokenizer-0.0.1.tar.gz` & `tmp/django-url-tokenizer-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-url-tokenizer-0.0.1.tar", last modified: Thu Jul 13 01:48:04 2023, max compression
+gzip compressed data, was "django-url-tokenizer-0.0.2.tar", last modified: Thu Jul 13 01:56:42 2023, max compression
```

## Comparing `django-url-tokenizer-0.0.1.tar` & `django-url-tokenizer-0.0.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 nibblex   (1000) nibblex   (1000)        0 2023-07-13 01:48:04.693769 django-url-tokenizer-0.0.1/
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)     1074 2023-07-13 01:29:20.000000 django-url-tokenizer-0.0.1/LICENSE
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)      441 2023-07-13 01:48:04.693769 django-url-tokenizer-0.0.1/PKG-INFO
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)      144 2023-07-13 01:29:20.000000 django-url-tokenizer-0.0.1/README.md
-drwxr-xr-x   0 nibblex   (1000) nibblex   (1000)        0 2023-07-13 01:48:04.693769 django-url-tokenizer-0.0.1/django_url_tokenizer.egg-info/
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)      441 2023-07-13 01:48:04.000000 django-url-tokenizer-0.0.1/django_url_tokenizer.egg-info/PKG-INFO
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)      448 2023-07-13 01:48:04.000000 django-url-tokenizer-0.0.1/django_url_tokenizer.egg-info/SOURCES.txt
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)        1 2023-07-13 01:48:04.000000 django-url-tokenizer-0.0.1/django_url_tokenizer.egg-info/dependency_links.txt
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)       36 2023-07-13 01:48:04.000000 django-url-tokenizer-0.0.1/django_url_tokenizer.egg-info/requires.txt
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)       13 2023-07-13 01:48:04.000000 django-url-tokenizer-0.0.1/django_url_tokenizer.egg-info/top_level.txt
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)       38 2023-07-13 01:48:04.693769 django-url-tokenizer-0.0.1/setup.cfg
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)      824 2023-07-13 01:47:47.000000 django-url-tokenizer-0.0.1/setup.py
-drwxr-xr-x   0 nibblex   (1000) nibblex   (1000)        0 2023-07-13 01:48:04.693769 django-url-tokenizer-0.0.1/urltokenizer/
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)        0 2023-07-13 00:48:39.000000 django-url-tokenizer-0.0.1/urltokenizer/__init__.py
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)      156 2023-07-13 00:48:39.000000 django-url-tokenizer-0.0.1/urltokenizer/apps.py
-drwxr-xr-x   0 nibblex   (1000) nibblex   (1000)        0 2023-07-13 01:48:04.693769 django-url-tokenizer-0.0.1/urltokenizer/migrations/
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)        0 2023-07-13 00:48:39.000000 django-url-tokenizer-0.0.1/urltokenizer/migrations/__init__.py
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)      710 2023-07-13 00:50:14.000000 django-url-tokenizer-0.0.1/urltokenizer/mixins.py
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)     1485 2023-07-13 00:51:13.000000 django-url-tokenizer-0.0.1/urltokenizer/serializers.py
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)       60 2023-07-13 00:48:39.000000 django-url-tokenizer-0.0.1/urltokenizer/tests.py
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)     4548 2023-07-13 00:51:53.000000 django-url-tokenizer-0.0.1/urltokenizer/tokenizer.py
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)      406 2023-07-13 00:52:10.000000 django-url-tokenizer-0.0.1/urltokenizer/views.py
+drwxr-xr-x   0 nibblex   (1000) nibblex   (1000)        0 2023-07-13 01:56:42.493710 django-url-tokenizer-0.0.2/
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)     1074 2023-07-13 01:29:20.000000 django-url-tokenizer-0.0.2/LICENSE
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)      441 2023-07-13 01:56:42.493710 django-url-tokenizer-0.0.2/PKG-INFO
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)      144 2023-07-13 01:29:20.000000 django-url-tokenizer-0.0.2/README.md
+drwxr-xr-x   0 nibblex   (1000) nibblex   (1000)        0 2023-07-13 01:56:42.493710 django-url-tokenizer-0.0.2/django_url_tokenizer.egg-info/
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)      441 2023-07-13 01:56:42.000000 django-url-tokenizer-0.0.2/django_url_tokenizer.egg-info/PKG-INFO
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)      448 2023-07-13 01:56:42.000000 django-url-tokenizer-0.0.2/django_url_tokenizer.egg-info/SOURCES.txt
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)        1 2023-07-13 01:56:42.000000 django-url-tokenizer-0.0.2/django_url_tokenizer.egg-info/dependency_links.txt
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)       41 2023-07-13 01:56:42.000000 django-url-tokenizer-0.0.2/django_url_tokenizer.egg-info/requires.txt
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)       13 2023-07-13 01:56:42.000000 django-url-tokenizer-0.0.2/django_url_tokenizer.egg-info/top_level.txt
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)       38 2023-07-13 01:56:42.493710 django-url-tokenizer-0.0.2/setup.cfg
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)      829 2023-07-13 01:53:37.000000 django-url-tokenizer-0.0.2/setup.py
+drwxr-xr-x   0 nibblex   (1000) nibblex   (1000)        0 2023-07-13 01:56:42.493710 django-url-tokenizer-0.0.2/urltokenizer/
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)        0 2023-07-13 00:48:39.000000 django-url-tokenizer-0.0.2/urltokenizer/__init__.py
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)      156 2023-07-13 00:48:39.000000 django-url-tokenizer-0.0.2/urltokenizer/apps.py
+drwxr-xr-x   0 nibblex   (1000) nibblex   (1000)        0 2023-07-13 01:56:42.493710 django-url-tokenizer-0.0.2/urltokenizer/migrations/
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)        0 2023-07-13 00:48:39.000000 django-url-tokenizer-0.0.2/urltokenizer/migrations/__init__.py
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)      710 2023-07-13 00:50:14.000000 django-url-tokenizer-0.0.2/urltokenizer/mixins.py
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)     1485 2023-07-13 00:51:13.000000 django-url-tokenizer-0.0.2/urltokenizer/serializers.py
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)       60 2023-07-13 00:48:39.000000 django-url-tokenizer-0.0.2/urltokenizer/tests.py
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)     4548 2023-07-13 00:51:53.000000 django-url-tokenizer-0.0.2/urltokenizer/tokenizer.py
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)      406 2023-07-13 00:52:10.000000 django-url-tokenizer-0.0.2/urltokenizer/views.py
```

### Comparing `django-url-tokenizer-0.0.1/LICENSE` & `django-url-tokenizer-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django-url-tokenizer-0.0.1/setup.py` & `django-url-tokenizer-0.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,25 +2,25 @@
 import setuptools
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setuptools.setup(
     name="django-url-tokenizer",
-    version="0.0.1",
+    version="0.0.2",
     author="Sergio Rodríguez",
     author_email="srodriguez3441@gmail.com",
     description="""A python package that provides a Django app that allows you to
     generate tokenized urls and send them to users via email.""",
     url="https://github.com/nibblex/django-url-tokenizer",
     packages=setuptools.find_packages(),
     license="MIT",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     install_requires=[
         "Django>=1.11",
-        "rest_framework>=3.13.1",
+        "djangorestframework>=3.13.1",
     ],
 )
```

### Comparing `django-url-tokenizer-0.0.1/urltokenizer/mixins.py` & `django-url-tokenizer-0.0.2/urltokenizer/mixins.py`

 * *Files identical despite different names*

### Comparing `django-url-tokenizer-0.0.1/urltokenizer/serializers.py` & `django-url-tokenizer-0.0.2/urltokenizer/serializers.py`

 * *Files identical despite different names*

### Comparing `django-url-tokenizer-0.0.1/urltokenizer/tokenizer.py` & `django-url-tokenizer-0.0.2/urltokenizer/tokenizer.py`

 * *Files identical despite different names*

