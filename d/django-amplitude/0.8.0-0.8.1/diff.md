# Comparing `tmp/django_amplitude-0.8.0.tar.gz` & `tmp/django_amplitude-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_amplitude-0.8.0.tar", max compression
+gzip compressed data, was "django_amplitude-0.8.1.tar", max compression
```

## Comparing `django_amplitude-0.8.0.tar` & `django_amplitude-0.8.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1065 2023-07-12 23:33:39.973174 django_amplitude-0.8.0/LICENSE.md
--rw-r--r--   0        0        0     6093 2023-07-12 23:33:39.973272 django_amplitude-0.8.0/README.md
--rw-r--r--   0        0        0      469 2023-07-12 23:33:39.973379 django_amplitude-0.8.0/amplitude/__init__.py
--rw-r--r--   0        0        0     8958 2023-07-13 01:50:37.105980 django_amplitude-0.8.0/amplitude/amplitude.py
--rw-r--r--   0        0        0       93 2023-07-12 23:33:39.973615 django_amplitude-0.8.0/amplitude/apps.py
--rw-r--r--   0        0        0     1452 2023-07-12 23:33:39.973723 django_amplitude-0.8.0/amplitude/middleware.py
--rw-r--r--   0        0        0     2221 2023-07-13 02:06:04.010157 django_amplitude-0.8.0/amplitude/settings.py
--rw-r--r--   0        0        0      997 2023-07-12 23:33:39.973935 django_amplitude-0.8.0/amplitude/utils.py
--rw-r--r--   0        0        0     1048 2023-07-13 01:56:44.721523 django_amplitude-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     7021 1970-01-01 00:00:00.000000 django_amplitude-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-07-12 23:33:39.973174 django_amplitude-0.8.1/LICENSE.md
+-rw-r--r--   0        0        0     6093 2023-07-12 23:33:39.973272 django_amplitude-0.8.1/README.md
+-rw-r--r--   0        0        0      469 2023-07-12 23:33:39.973379 django_amplitude-0.8.1/amplitude/__init__.py
+-rw-r--r--   0        0        0     8958 2023-07-13 01:50:37.105980 django_amplitude-0.8.1/amplitude/amplitude.py
+-rw-r--r--   0        0        0       93 2023-07-12 23:33:39.973615 django_amplitude-0.8.1/amplitude/apps.py
+-rw-r--r--   0        0        0     1452 2023-07-12 23:33:39.973723 django_amplitude-0.8.1/amplitude/middleware.py
+-rw-r--r--   0        0        0     2221 2023-07-13 02:06:04.010157 django_amplitude-0.8.1/amplitude/settings.py
+-rw-r--r--   0        0        0      997 2023-07-12 23:33:39.973935 django_amplitude-0.8.1/amplitude/utils.py
+-rw-r--r--   0        0        0     1041 2023-07-13 09:05:47.043577 django_amplitude-0.8.1/pyproject.toml
+-rw-r--r--   0        0        0     7008 1970-01-01 00:00:00.000000 django_amplitude-0.8.1/PKG-INFO
```

### Comparing `django_amplitude-0.8.0/LICENSE.md` & `django_amplitude-0.8.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `django_amplitude-0.8.0/README.md` & `django_amplitude-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `django_amplitude-0.8.0/amplitude/amplitude.py` & `django_amplitude-0.8.1/amplitude/amplitude.py`

 * *Files identical despite different names*

### Comparing `django_amplitude-0.8.0/amplitude/middleware.py` & `django_amplitude-0.8.1/amplitude/middleware.py`

 * *Files identical despite different names*

### Comparing `django_amplitude-0.8.0/amplitude/settings.py` & `django_amplitude-0.8.1/amplitude/settings.py`

 * *Files identical despite different names*

### Comparing `django_amplitude-0.8.0/amplitude/utils.py` & `django_amplitude-0.8.1/amplitude/utils.py`

 * *Files identical despite different names*

### Comparing `django_amplitude-0.8.0/pyproject.toml` & `django_amplitude-0.8.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 [tool.poetry]
 name = "django-amplitude"
 packages = [
     {include = "amplitude"}
 ]
-version = "0.8.0"
+version = "0.8.1"
 description = "Integration between Django and Amplitude"
 authors = ["Matt Pye <pyematt@gmail.com>"]
 readme = "README.md"
 license = "MIT"
 repository = "https://github.com/pyepye/django-amplitude"
 homepage = "https://github.com/pyepye/django-amplitude"
 keywords = ["amplitude", "analytics", "product analytics", "saas"]
 
 
 [tool.poetry.dependencies]
 python = "^3.6"
 Django = ">=2.1"
-httpx = ">=0.13.2,<0.21.0"
-user-agents = "^2.1"
+httpx = ">=0.13.2"
+user-agents = ">=2.1"
 
 
 [tool.poetry.dev-dependencies]
 django-stubs = "^1.5.0"
 flake8 = "^4.0.1"
 isort = {extras = ["pyproject"], version = "^5.2.0"}
 pytest = "^7.0.1"
```

### Comparing `django_amplitude-0.8.0/PKG-INFO` & `django_amplitude-0.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-amplitude
-Version: 0.8.0
+Version: 0.8.1
 Summary: Integration between Django and Amplitude
 Home-page: https://github.com/pyepye/django-amplitude
 License: MIT
 Keywords: amplitude,analytics,product analytics,saas
 Author: Matt Pye
 Author-email: pyematt@gmail.com
 Requires-Python: >=3.6,<4.0
@@ -13,16 +13,16 @@
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: Django (>=2.1)
-Requires-Dist: httpx (>=0.13.2,<0.21.0)
-Requires-Dist: user-agents (>=2.1,<3.0)
+Requires-Dist: httpx (>=0.13.2)
+Requires-Dist: user-agents (>=2.1)
 Project-URL: Repository, https://github.com/pyepye/django-amplitude
 Description-Content-Type: text/markdown
 
 # Django Amplitude
 
 Integration between Django and [Amplitude.com](https://amplitude.com/) to help send events via the [Amplitude HTTP API (v2)](https://developers.amplitude.com/docs/http-api-v2)
```

