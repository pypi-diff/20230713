# Comparing `tmp/django-amplitude-0.7.1.tar.gz` & `tmp/django_amplitude-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-amplitude-0.7.1.tar", last modified: Tue Sep  7 22:52:24 2021, max compression
+gzip compressed data, was "django_amplitude-0.8.0.tar", max compression
```

## Comparing `django-amplitude-0.7.1.tar` & `django_amplitude-0.8.0.tar`

### file list

```diff
@@ -1,11 +1,10 @@
--rw-r--r--   0        0        0     1065 2020-05-27 21:59:29.816341 django-amplitude-0.7.1/LICENSE.md
--rw-r--r--   0        0        0     6093 2021-09-07 22:12:43.619925 django-amplitude-0.7.1/README.md
--rw-r--r--   0        0        0      469 2021-09-07 22:51:18.607254 django-amplitude-0.7.1/amplitude/__init__.py
--rw-r--r--   0        0        0     8019 2021-01-28 12:23:49.126437 django-amplitude-0.7.1/amplitude/amplitude.py
--rw-r--r--   0        0        0       93 2020-07-10 11:26:45.511988 django-amplitude-0.7.1/amplitude/apps.py
--rw-r--r--   0        0        0     1452 2020-12-22 23:55:00.795338 django-amplitude-0.7.1/amplitude/middleware.py
--rw-r--r--   0        0        0     2161 2021-01-28 12:15:45.995634 django-amplitude-0.7.1/amplitude/settings.py
--rw-r--r--   0        0        0      997 2021-09-07 22:13:27.573356 django-amplitude-0.7.1/amplitude/utils.py
--rw-r--r--   0        0        0     1039 2021-09-07 22:51:18.608630 django-amplitude-0.7.1/pyproject.toml
--rw-r--r--   0        0        0     6974 2021-09-07 22:52:27.196945 django-amplitude-0.7.1/setup.py
--rw-r--r--   0        0        0     6869 2021-09-07 22:52:27.197432 django-amplitude-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-07-12 23:33:39.973174 django_amplitude-0.8.0/LICENSE.md
+-rw-r--r--   0        0        0     6093 2023-07-12 23:33:39.973272 django_amplitude-0.8.0/README.md
+-rw-r--r--   0        0        0      469 2023-07-12 23:33:39.973379 django_amplitude-0.8.0/amplitude/__init__.py
+-rw-r--r--   0        0        0     8958 2023-07-13 01:50:37.105980 django_amplitude-0.8.0/amplitude/amplitude.py
+-rw-r--r--   0        0        0       93 2023-07-12 23:33:39.973615 django_amplitude-0.8.0/amplitude/apps.py
+-rw-r--r--   0        0        0     1452 2023-07-12 23:33:39.973723 django_amplitude-0.8.0/amplitude/middleware.py
+-rw-r--r--   0        0        0     2221 2023-07-13 02:06:04.010157 django_amplitude-0.8.0/amplitude/settings.py
+-rw-r--r--   0        0        0      997 2023-07-12 23:33:39.973935 django_amplitude-0.8.0/amplitude/utils.py
+-rw-r--r--   0        0        0     1048 2023-07-13 01:56:44.721523 django_amplitude-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0     7021 1970-01-01 00:00:00.000000 django_amplitude-0.8.0/PKG-INFO
```

### Comparing `django-amplitude-0.7.1/LICENSE.md` & `django_amplitude-0.8.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `django-amplitude-0.7.1/README.md` & `django_amplitude-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `django-amplitude-0.7.1/amplitude/amplitude.py` & `django_amplitude-0.8.0/amplitude/amplitude.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import logging
 import time
 from typing import Any, Dict, List
 
 import httpx
 from django.contrib.auth import get_user_model
 from django.http import HttpRequest
@@ -24,18 +26,18 @@
     pass
 
 
 class Amplitude():
 
     def __init__(
         self,
-        api_key: str = None,
-        include_user_data: bool = None,
-        include_group_data: bool = None,
-        min_id_length: int = None,
+        api_key: str = '',
+        include_user_data: bool | None = None,
+        include_group_data: bool | None = None,
+        min_id_length: int | None = None,
     ):
         if not api_key:
             api_key = app_settings.API_KEY
         if include_user_data is None:
             include_user_data = app_settings.INCLUDE_USER_DATA
         if include_group_data is None:
             include_group_data = app_settings.INCLUDE_GROUP_DATA
@@ -116,15 +118,18 @@
 
         if event_properties:
             event['event_properties'] = event_properties
         else:
             event['event_properties'] = self.event_properties_from_request(request)  # NOQA: E501
 
         try:
-            event['user_id'] = f'{request.user.pk:05}'
+            if self.min_id_length:
+                event['user_id'] = f'{request.user.pk:0{self.min_id_length}}'
+            else:
+                event['user_id'] = f'{request.user.pk:05}'
         except (AttributeError, TypeError):
             pass
         event['user_properties'] = self.user_properties_from_request(request)
         event['groups'] = self.group_from_request(request)
 
         device_data = self.device_data_from_request(request)
         event.update(device_data)
@@ -167,50 +172,67 @@
             return {}
 
         User = get_user_model()
         user = User.objects.get(pk=request.user.pk)
 
         user_data = {
             'username': user.get_username(),
-            'email': user.email,
-            'full_name': user.get_full_name(),
-            'is_staff': user.is_staff,
-            'is_superuser': user.is_superuser,
         }
-        if user.last_login:
+
+        if hasattr(user, 'email') and user.email:
+            user_data['email'] = user.email
+        if hasattr(user, 'full_name') and user.full_name:
+            get_full_name = getattr(user, "get_full_name")
+            if get_full_name and callable(get_full_name):
+                user_data['full_name'] = user.get_full_name()  # type: ignore
+            else:
+                user_data['full_name'] = user.full_name
+        if hasattr(user, 'is_staff') and user.is_staff:
+            user_data['is_staff'] = user.is_staff
+        if hasattr(user, 'is_superuser') and user.is_superuser:
+            user_data['is_superuser'] = user.is_superuser
+
+        if hasattr(user, 'last_login') and user.last_login:
             user_data['last_login'] = user.last_login.isoformat()
-        if user.date_joined:
+        if hasattr(user, 'date_joined') and user.date_joined:
             user_data['date_joined'] = user.date_joined.isoformat()
         return user_data
 
     def group_from_request(self, request: HttpRequest) -> list:
         try:
             request.user.is_authenticated
         except AttributeError:
             return []
 
         if not self.include_group_data or not request.user.is_authenticated:
             return []
 
         User = get_user_model()
         user = User.objects.get(pk=request.user.pk)
-        groups = user.groups.all().values_list('name', flat=True)
+
+        groups = []
+        if hasattr(user, 'groups'):
+            groups = user.groups.all().values_list('name', flat=True)
         return list(groups)
 
     def location_data_from_ip_address(self, ip_address: str) -> dict:
         location_data: dict = {}
 
         if not ip_address or not CAN_GEOIP:
             return location_data
 
         # pip install geoip2
         # https://pypi.org/project/geoip2/
         # from django.contrib.gis.geoip2 import GeoIP2
         g = GeoIP2()
-        location = g.city(ip_address)
+        try:
+            location = g.city(ip_address)
+        except RuntimeError:
+            # Catch exceptions like `AddressNotFoundError`
+            return location_data
         location_data['country'] = location['country_name']
         location_data['city'] = location['city']
         lat_lon = g.lat_lon(ip_address)
         location_data['location_lat'] = lat_lon[0]
         location_data['location_lng'] = lat_lon[1]
         return location_data
```

### Comparing `django-amplitude-0.7.1/amplitude/middleware.py` & `django_amplitude-0.8.0/amplitude/middleware.py`

 * *Files identical despite different names*

### Comparing `django-amplitude-0.7.1/amplitude/settings.py` & `django_amplitude-0.8.0/amplitude/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,24 @@
+from __future__ import annotations
+
 from django.conf import settings
 from django.core.exceptions import ImproperlyConfigured
 
 API_KEY = getattr(settings, 'AMPLITUDE_API_KEY')
 if not API_KEY:
     raise ImproperlyConfigured('"AMPLITUDE_API_KEY" is not set')
 
-INCLUDE_USER_DATA = getattr(settings, 'AMPLITUDE_INCLUDE_USER_DATA', False)  # NOQA: E501
-INCLUDE_GROUP_DATA = getattr(settings, 'AMPLITUDE_INCLUDE_GROUP_DATA', False)  # NOQA: E501
+INCLUDE_USER_DATA: bool = getattr(settings, 'AMPLITUDE_INCLUDE_USER_DATA', False)  # NOQA: E501
+INCLUDE_GROUP_DATA: bool = getattr(settings, 'AMPLITUDE_INCLUDE_GROUP_DATA', False)  # NOQA: E501
 IGNORE_URLS = getattr(settings, 'AMPLITUDE_IGNORE_URLS', [])
 if not isinstance(IGNORE_URLS, list):
     error = '"AMPLITUDE_IGNORE_URLS" must be a list of URLs or URL names'
     raise ImproperlyConfigured(error)
 
-MIN_ID_LENGTH = getattr(settings, 'AMPLITUDE_MIN_ID_LENGTH', None)
+MIN_ID_LENGTH: int | None = getattr(settings, 'AMPLITUDE_MIN_ID_LENGTH', None)
 if MIN_ID_LENGTH and not isinstance(MIN_ID_LENGTH, int):
     raise ImproperlyConfigured('"AMPLITUDE_MIN_ID_LENGTH" must be an integer')
 
 installed_apps = getattr(settings, 'INSTALLED_APPS')
 middleware = getattr(settings, 'MIDDLEWARE')
 missing_session_settings = (
     'django.contrib.sessions' not in installed_apps
```

### Comparing `django-amplitude-0.7.1/amplitude/utils.py` & `django_amplitude-0.8.0/amplitude/utils.py`

 * *Files identical despite different names*

### Comparing `django-amplitude-0.7.1/pyproject.toml` & `django_amplitude-0.8.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 [tool.poetry]
 name = "django-amplitude"
 packages = [
     {include = "amplitude"}
 ]
-version = "0.7.1"
+version = "0.8.0"
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
-httpx = "^0.13.2"
+httpx = ">=0.13.2,<0.21.0"
 user-agents = "^2.1"
 
 
 [tool.poetry.dev-dependencies]
-pytest = "^5.4.2"
-pytest-cov = "^2.9.0"
-pytest-mock = "^3.1.0"
-pytest-django = "^3.9.0"
-pytest-freezegun = "^0.4.1"
-flake8 = "^3.8.2"
-tox = "^3.15.1"
 django-stubs = "^1.5.0"
+flake8 = "^4.0.1"
 isort = {extras = ["pyproject"], version = "^5.2.0"}
+pytest = "^7.0.1"
+pytest-cov = "^4.0.0"
+pytest-django = "^4.5.2"
+pytest-freezegun = "^0.4.1"
+pytest-mock = "^3.1.0"
+tox = "^3.28.0"
 
 
 [tool.isort]
 line_length = 79
 multi_line_output = 5
 known_third_party = "pytest"
 known_first_party = "amplitude"
```

### Comparing `django-amplitude-0.7.1/setup.py` & `django_amplitude-0.8.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,199 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: django-amplitude
+Version: 0.8.0
+Summary: Integration between Django and Amplitude
+Home-page: https://github.com/pyepye/django-amplitude
+License: MIT
+Keywords: amplitude,analytics,product analytics,saas
+Author: Matt Pye
+Author-email: pyematt@gmail.com
+Requires-Python: >=3.6,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: Django (>=2.1)
+Requires-Dist: httpx (>=0.13.2,<0.21.0)
+Requires-Dist: user-agents (>=2.1,<3.0)
+Project-URL: Repository, https://github.com/pyepye/django-amplitude
+Description-Content-Type: text/markdown
+
+# Django Amplitude
+
+Integration between Django and [Amplitude.com](https://amplitude.com/) to help send events via the [Amplitude HTTP API (v2)](https://developers.amplitude.com/docs/http-api-v2)
+
+
+## Quick start
+
+### Installation
+
+```bash
+pip install django-amplitude
+```
+
+Add `amplitude` to your `INSTALLED_APPS`. If they are not already the Django `sessions` app must also be added:
+
+```python
+INSTALLED_APPS = [
+    ...
+    'django.contrib.sessions',
+    ...
+    'amplitude',
+]
+```
+
+If you do not have it already you must also add the Django `django.contrib.sessions.middleware.SessionMiddleware`. Then add the ampliturde `SessionInfo` middleware after the `SessionMiddleware`:
+```python
+MIDDLEWARE = [
+    ...
+    'django.contrib.sessions.middleware.SessionMiddleware',
+    ...
+    'amplitude.middleware.SessionInfo',
+]
+```
+
+Now set your Amplitude API key and user / group options in your `settings.py`:
+```python
+# Settings > Projects > <Your project> > General > API Key
+AMPLITUDE_API_KEY = '<amplitude-project-api-key>'
+
+# You can also choose if you want to include user and group data (Default False)
+AMPLITUDE_INCLUDE_USER_DATA = False
+AMPLITUDE_INCLUDE_GROUP_DATA = False
+```
+
+*Note: If you want to include user or group data you must ensure the [Django auth is setup correctly](https://docs.djangoproject.com/en/3.0/topics/auth/#installation). This includes adding `django.contrib.auth` and `django.contrib.contenttypes` to `INSTALLED_APPS` and `django.contrib.auth.middleware.AuthenticationMiddleware` to `MIDDLEWARE`*.
+
+
+For more information on the above settings see the [configuration settings](#configuration-settings) section.
+
+
+
+## Usage
+
+### Page view events
+
+If you want to send an event to Amplitude on every page view you can use the django-amplitude `SendPageViewEvent` middleware to your `MIDDLEWARE` in your Django settings.
+
+This will automatically create an event called `Page view` with all the information it's possible to pull from the Django request object such as URL path and parameters, user agent info, IP info, user info etc.
+
+It must be placed after the `amplitude.middleware.SessionInfo` middleware:
+
+```python
+MIDDLEWARE = [
+    'django.contrib.sessions.middleware.SessionMiddleware',
+    ...
+    'amplitude.middleware.SessionInfo',
+    'amplitude.middleware.SendPageViewEvent',
+]
+```
+
+While using `SendPageViewEvent` if there are certain URLs that you do not want to update Amplitude with you can use the `AMPLITUDE_IGNORE_URLS` setting. This setting take a list of relative urls or URL names. Relative URLS most match exactly so need to start with a forward slash (`/`)
+
+```python
+AMPLITUDE_IGNORE_URLS = ['my_url_name', '/testurl']
+```
+
+
+### Sending events manually
+
+If you want to send your own events:
+```python
+from amplitude import Amplitude
+
+amplitude = Amplitude()
+event_data = amplitude.build_event_data(
+    event_type='Some event type',
+    request=request,
+)
+amplitude.send_events([event_data])
+```
+
+The above request will include URL and HTTP header info in the `event_properties`. If you want to override the event properties you can pass them through to `build_event_data`:
+
+```python
+event_data = amplitude.build_event_data(
+    event_type='User purchase',
+    request=request,
+    event_properties={'products': ['laptop', 'phone']}
+)
+```
+
+### build_event_data missing event data keys
+
+The `build_event_data` method (and in extension the `SendPageViewEvent` middleware) currently does not send the following keys from `UploadRequestBody` type in [Amplitude HTTP API (v2)](https://developers.amplitude.com/docs/http-api-v2):
+
+* event_id
+* app_version
+* carrier
+* price
+* quantity
+* revenue
+* productId
+* revenueType
+* idfa
+* idfv
+* adid
+* android_id
+* dma
+* insert_id
+
+If you want to record an event in Amplitude with any of these keys you must use build and send your own event data using `amplitude.build_event_data` where you can pass any of the above as kwargs:
+
+```python
+amplitude = Amplitude()
+event_data = amplitude.build_event_data(
+    event_type='Some event type',
+    request=request,
+    app_version='1.0.0',
+)
+amplitude.send_events([event_data])
+```
+
+
+### Building you own event
+
+If you are not happy with the data from `build_event_data` you can build you own event data based on the `UploadRequestBody` type in [Amplitude HTTP API (v2)](https://developers.amplitude.com/docs/http-api-v2). If you want to do this There are a few helper functions to build different parts of the event data from the Django request object:
+
+```python
+amplitude.event_properties_from_request(request)  # Gets URL and HTTP header data
+amplitude.device_data_from_request(request)  # Gets device info from user agent
+amplitude.user_properties_from_request(request)  # Gets info from user model
+amplitude.group_from_request(request)  # Gets the list of groups a user is in
+
+amplitude.location_data_from_ip_address(ip_address)  # Gets location data from IP if GeoIP2 is setup
+```
+
+* `user_properties_from_request` will return an empty dict if `AMPLITUDE_INCLUDE_USER_DATA` is `False`
+* `group_from_request` will return an empty dict if `AMPLITUDE_INCLUDE_GROUP_DATA` is `False`
+
+
+#### Configuration settings
+
+Below are the different settings that can be overridden. To do so place the setting into your `settings.py`.
+
+```python
+# This variable is required when amplitude is added to INSTALLED_APPS
+AMPLITUDE_API_KEY = '<amplitude-project-api-key>'
+
+# If the users Django user information is included in the Amplitude event.
+# This includes - username, email, full_name, is_staff, is_superuser
+AMPLITUDE_INCLUDE_USER_DATA = False
+
+# If the groups the user is a member of is included in the Amplitude event.
+# A list of the group names will be sent in the request.
+AMPLITUDE_INCLUDE_GROUP_DATA = False
+
+# A list of URLs which `SendPageViewEvent` middleware should not run for.
+# Each item in the list can be either a URL or url name
+AMPLITUDE_IGNORE_URLS = ['home', '/please/ignore/']
+
+# The minimum permitted length for user_id & device_id fields
+# https://developers.amplitude.com/docs/http-api-v2#properties-2
+AMPLITUDE_MIN_ID_LENGTH = None
+```
 
-packages = \
-['amplitude']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['Django>=2.1', 'httpx>=0.13.2,<0.14.0', 'user-agents>=2.1,<3.0']
-
-setup_kwargs = {
-    'name': 'django-amplitude',
-    'version': '0.7.1',
-    'description': 'Integration between Django and Amplitude',
-    'long_description': "# Django Amplitude\n\nIntegration between Django and [Amplitude.com](https://amplitude.com/) to help send events via the [Amplitude HTTP API (v2)](https://developers.amplitude.com/docs/http-api-v2)\n\n\n## Quick start\n\n### Installation\n\n```bash\npip install django-amplitude\n```\n\nAdd `amplitude` to your `INSTALLED_APPS`. If they are not already the Django `sessions` app must also be added:\n\n```python\nINSTALLED_APPS = [\n    ...\n    'django.contrib.sessions',\n    ...\n    'amplitude',\n]\n```\n\nIf you do not have it already you must also add the Django `django.contrib.sessions.middleware.SessionMiddleware`. Then add the ampliturde `SessionInfo` middleware after the `SessionMiddleware`:\n```python\nMIDDLEWARE = [\n    ...\n    'django.contrib.sessions.middleware.SessionMiddleware',\n    ...\n    'amplitude.middleware.SessionInfo',\n]\n```\n\nNow set your Amplitude API key and user / group options in your `settings.py`:\n```python\n# Settings > Projects > <Your project> > General > API Key\nAMPLITUDE_API_KEY = '<amplitude-project-api-key>'\n\n# You can also choose if you want to include user and group data (Default False)\nAMPLITUDE_INCLUDE_USER_DATA = False\nAMPLITUDE_INCLUDE_GROUP_DATA = False\n```\n\n*Note: If you want to include user or group data you must ensure the [Django auth is setup correctly](https://docs.djangoproject.com/en/3.0/topics/auth/#installation). This includes adding `django.contrib.auth` and `django.contrib.contenttypes` to `INSTALLED_APPS` and `django.contrib.auth.middleware.AuthenticationMiddleware` to `MIDDLEWARE`*.\n\n\nFor more information on the above settings see the [configuration settings](#configuration-settings) section.\n\n\n\n## Usage\n\n### Page view events\n\nIf you want to send an event to Amplitude on every page view you can use the django-amplitude `SendPageViewEvent` middleware to your `MIDDLEWARE` in your Django settings.\n\nThis will automatically create an event called `Page view` with all the information it's possible to pull from the Django request object such as URL path and parameters, user agent info, IP info, user info etc.\n\nIt must be placed after the `amplitude.middleware.SessionInfo` middleware:\n\n```python\nMIDDLEWARE = [\n    'django.contrib.sessions.middleware.SessionMiddleware',\n    ...\n    'amplitude.middleware.SessionInfo',\n    'amplitude.middleware.SendPageViewEvent',\n]\n```\n\nWhile using `SendPageViewEvent` if there are certain URLs that you do not want to update Amplitude with you can use the `AMPLITUDE_IGNORE_URLS` setting. This setting take a list of relative urls or URL names. Relative URLS most match exactly so need to start with a forward slash (`/`)\n\n```python\nAMPLITUDE_IGNORE_URLS = ['my_url_name', '/testurl']\n```\n\n\n### Sending events manually\n\nIf you want to send your own events:\n```python\nfrom amplitude import Amplitude\n\namplitude = Amplitude()\nevent_data = amplitude.build_event_data(\n    event_type='Some event type',\n    request=request,\n)\namplitude.send_events([event_data])\n```\n\nThe above request will include URL and HTTP header info in the `event_properties`. If you want to override the event properties you can pass them through to `build_event_data`:\n\n```python\nevent_data = amplitude.build_event_data(\n    event_type='User purchase',\n    request=request,\n    event_properties={'products': ['laptop', 'phone']}\n)\n```\n\n### build_event_data missing event data keys\n\nThe `build_event_data` method (and in extension the `SendPageViewEvent` middleware) currently does not send the following keys from `UploadRequestBody` type in [Amplitude HTTP API (v2)](https://developers.amplitude.com/docs/http-api-v2):\n\n* event_id\n* app_version\n* carrier\n* price\n* quantity\n* revenue\n* productId\n* revenueType\n* idfa\n* idfv\n* adid\n* android_id\n* dma\n* insert_id\n\nIf you want to record an event in Amplitude with any of these keys you must use build and send your own event data using `amplitude.build_event_data` where you can pass any of the above as kwargs:\n\n```python\namplitude = Amplitude()\nevent_data = amplitude.build_event_data(\n    event_type='Some event type',\n    request=request,\n    app_version='1.0.0',\n)\namplitude.send_events([event_data])\n```\n\n\n### Building you own event\n\nIf you are not happy with the data from `build_event_data` you can build you own event data based on the `UploadRequestBody` type in [Amplitude HTTP API (v2)](https://developers.amplitude.com/docs/http-api-v2). If you want to do this There are a few helper functions to build different parts of the event data from the Django request object:\n\n```python\namplitude.event_properties_from_request(request)  # Gets URL and HTTP header data\namplitude.device_data_from_request(request)  # Gets device info from user agent\namplitude.user_properties_from_request(request)  # Gets info from user model\namplitude.group_from_request(request)  # Gets the list of groups a user is in\n\namplitude.location_data_from_ip_address(ip_address)  # Gets location data from IP if GeoIP2 is setup\n```\n\n* `user_properties_from_request` will return an empty dict if `AMPLITUDE_INCLUDE_USER_DATA` is `False`\n* `group_from_request` will return an empty dict if `AMPLITUDE_INCLUDE_GROUP_DATA` is `False`\n\n\n#### Configuration settings\n\nBelow are the different settings that can be overridden. To do so place the setting into your `settings.py`.\n\n```python\n# This variable is required when amplitude is added to INSTALLED_APPS\nAMPLITUDE_API_KEY = '<amplitude-project-api-key>'\n\n# If the users Django user information is included in the Amplitude event.\n# This includes - username, email, full_name, is_staff, is_superuser\nAMPLITUDE_INCLUDE_USER_DATA = False\n\n# If the groups the user is a member of is included in the Amplitude event.\n# A list of the group names will be sent in the request.\nAMPLITUDE_INCLUDE_GROUP_DATA = False\n\n# A list of URLs which `SendPageViewEvent` middleware should not run for.\n# Each item in the list can be either a URL or url name\nAMPLITUDE_IGNORE_URLS = ['home', '/please/ignore/']\n\n# The minimum permitted length for user_id & device_id fields\n# https://developers.amplitude.com/docs/http-api-v2#properties-2\nAMPLITUDE_MIN_ID_LENGTH = None\n```\n",
-    'author': 'Matt Pye',
-    'author_email': 'pyematt@gmail.com',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/pyepye/django-amplitude',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.6,<4.0',
-}
-
-
-setup(**setup_kwargs)
```

