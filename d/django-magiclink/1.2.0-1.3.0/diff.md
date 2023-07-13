# Comparing `tmp/django-magiclink-1.2.0.tar.gz` & `tmp/django_magiclink-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-magiclink-1.2.0.tar", max compression
+gzip compressed data, was "django_magiclink-1.3.0.tar", max compression
```

## Comparing `django-magiclink-1.2.0.tar` & `django_magiclink-1.3.0.tar`

### file list

```diff
@@ -1,27 +1,26 @@
--rw-r--r--   0        0        0     1065 2022-01-24 00:46:23.580153 django-magiclink-1.2.0/LICENSE.md
--rw-r--r--   0        0        0    17562 2022-01-24 02:22:00.773586 django-magiclink-1.2.0/README.md
--rw-r--r--   0        0        0      421 2022-01-24 00:46:23.584102 django-magiclink-1.2.0/magiclink/__init__.py
--rw-r--r--   0        0        0       93 2022-01-24 00:46:23.584298 django-magiclink-1.2.0/magiclink/apps.py
--rw-r--r--   0        0        0     1427 2022-01-24 00:46:23.584479 django-magiclink-1.2.0/magiclink/backends.py
--rw-r--r--   0        0        0     5395 2022-01-24 02:24:09.568862 django-magiclink-1.2.0/magiclink/forms.py
--rw-r--r--   0        0        0     3209 2022-01-24 00:46:23.584801 django-magiclink-1.2.0/magiclink/helpers.py
--rw-r--r--   0        0        0        0 2022-01-24 00:46:23.584932 django-magiclink-1.2.0/magiclink/management/__init__.py
--rw-r--r--   0        0        0        0 2022-01-24 00:46:23.585062 django-magiclink-1.2.0/magiclink/management/commands/__init__.py
--rw-r--r--   0        0        0      791 2022-01-24 00:46:23.585198 django-magiclink-1.2.0/magiclink/management/commands/magiclink_clear_logins.py
--rw-r--r--   0        0        0      981 2022-01-24 00:46:23.585390 django-magiclink-1.2.0/magiclink/migrations/0001_initial.py
--rw-r--r--   0        0        0      521 2022-01-24 01:36:25.632428 django-magiclink-1.2.0/magiclink/migrations/0002_magiclinkunsubscribe.py
--rw-r--r--   0        0        0        0 2022-01-24 00:46:23.585494 django-magiclink-1.2.0/magiclink/migrations/__init__.py
--rw-r--r--   0        0        0     5089 2022-01-24 01:40:01.542926 django-magiclink-1.2.0/magiclink/models.py
--rw-r--r--   0        0        0     5791 2022-01-24 01:39:32.872205 django-magiclink-1.2.0/magiclink/settings.py
--rw-r--r--   0        0        0     1122 2022-01-24 00:46:23.586206 django-magiclink-1.2.0/magiclink/templates/magiclink/login.html
--rw-r--r--   0        0        0     8147 2022-01-24 00:46:23.586395 django-magiclink-1.2.0/magiclink/templates/magiclink/login_email.html
--rw-r--r--   0        0        0      268 2022-01-24 00:46:23.586652 django-magiclink-1.2.0/magiclink/templates/magiclink/login_email.txt
--rw-r--r--   0        0        0     1510 2022-01-24 00:46:23.586868 django-magiclink-1.2.0/magiclink/templates/magiclink/login_failed.html
--rw-r--r--   0        0        0      700 2022-01-24 00:46:23.587062 django-magiclink-1.2.0/magiclink/templates/magiclink/login_sent.html
--rw-r--r--   0        0        0     1077 2022-01-24 00:46:23.587230 django-magiclink-1.2.0/magiclink/templates/magiclink/signup.html
--rw-r--r--   0        0        0      433 2022-01-24 00:46:23.587441 django-magiclink-1.2.0/magiclink/urls.py
--rw-r--r--   0        0        0      643 2022-01-24 00:46:23.587679 django-magiclink-1.2.0/magiclink/utils.py
--rw-r--r--   0        0        0     8006 2022-01-24 01:19:09.838163 django-magiclink-1.2.0/magiclink/views.py
--rw-r--r--   0        0        0     1025 2022-01-24 02:22:37.297724 django-magiclink-1.2.0/pyproject.toml
--rw-r--r--   0        0        0    18951 2022-01-24 02:56:14.676047 django-magiclink-1.2.0/setup.py
--rw-r--r--   0        0        0    18359 2022-01-24 02:56:14.677120 django-magiclink-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2022-07-09 13:28:24.207859 django_magiclink-1.3.0/LICENSE.md
+-rw-r--r--   0        0        0    17562 2022-07-09 13:28:24.208108 django_magiclink-1.3.0/README.md
+-rw-r--r--   0        0        0      421 2022-07-09 13:28:24.213456 django_magiclink-1.3.0/magiclink/__init__.py
+-rw-r--r--   0        0        0       93 2022-07-09 13:28:24.213561 django_magiclink-1.3.0/magiclink/apps.py
+-rw-r--r--   0        0        0     1427 2022-07-09 13:28:24.213682 django_magiclink-1.3.0/magiclink/backends.py
+-rw-r--r--   0        0        0     5429 2023-07-13 00:57:48.715294 django_magiclink-1.3.0/magiclink/forms.py
+-rw-r--r--   0        0        0     3209 2022-07-09 13:28:24.213951 django_magiclink-1.3.0/magiclink/helpers.py
+-rw-r--r--   0        0        0        0 2022-07-09 13:28:24.214049 django_magiclink-1.3.0/magiclink/management/__init__.py
+-rw-r--r--   0        0        0        0 2022-07-09 13:28:24.214152 django_magiclink-1.3.0/magiclink/management/commands/__init__.py
+-rw-r--r--   0        0        0      791 2022-07-09 13:28:24.214284 django_magiclink-1.3.0/magiclink/management/commands/magiclink_clear_logins.py
+-rw-r--r--   0        0        0      981 2022-07-09 13:28:24.214458 django_magiclink-1.3.0/magiclink/migrations/0001_initial.py
+-rw-r--r--   0        0        0      521 2022-07-09 13:28:24.214577 django_magiclink-1.3.0/magiclink/migrations/0002_magiclinkunsubscribe.py
+-rw-r--r--   0        0        0        0 2022-07-09 13:28:24.214625 django_magiclink-1.3.0/magiclink/migrations/__init__.py
+-rw-r--r--   0        0        0     5089 2022-07-09 13:28:24.214781 django_magiclink-1.3.0/magiclink/models.py
+-rw-r--r--   0        0        0     5791 2022-07-09 13:28:24.214913 django_magiclink-1.3.0/magiclink/settings.py
+-rw-r--r--   0        0        0     1122 2022-07-09 13:28:24.215132 django_magiclink-1.3.0/magiclink/templates/magiclink/login.html
+-rw-r--r--   0        0        0     8147 2022-07-09 13:28:24.215274 django_magiclink-1.3.0/magiclink/templates/magiclink/login_email.html
+-rw-r--r--   0        0        0      268 2022-07-09 13:28:24.215398 django_magiclink-1.3.0/magiclink/templates/magiclink/login_email.txt
+-rw-r--r--   0        0        0     1510 2022-07-09 13:28:24.215513 django_magiclink-1.3.0/magiclink/templates/magiclink/login_failed.html
+-rw-r--r--   0        0        0      700 2022-07-09 13:28:24.215622 django_magiclink-1.3.0/magiclink/templates/magiclink/login_sent.html
+-rw-r--r--   0        0        0     1077 2022-07-09 13:28:24.215711 django_magiclink-1.3.0/magiclink/templates/magiclink/signup.html
+-rw-r--r--   0        0        0      433 2022-07-09 13:28:24.215811 django_magiclink-1.3.0/magiclink/urls.py
+-rw-r--r--   0        0        0      643 2022-07-09 13:28:24.215924 django_magiclink-1.3.0/magiclink/utils.py
+-rw-r--r--   0        0        0     8022 2023-07-13 00:57:50.636349 django_magiclink-1.3.0/magiclink/views.py
+-rw-r--r--   0        0        0     1031 2023-07-13 02:30:59.407626 django_magiclink-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0    18461 1970-01-01 00:00:00.000000 django_magiclink-1.3.0/PKG-INFO
```

### Comparing `django-magiclink-1.2.0/LICENSE.md` & `django_magiclink-1.3.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `django-magiclink-1.2.0/README.md` & `django_magiclink-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `django-magiclink-1.2.0/magiclink/backends.py` & `django_magiclink-1.3.0/magiclink/backends.py`

 * *Files identical despite different names*

### Comparing `django-magiclink-1.2.0/magiclink/forms.py` & `django_magiclink-1.3.0/magiclink/forms.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,23 +30,23 @@
                 'tabindex': '-1',
                 'style': 'display: none !important',
             }
         ),
     )
 
     def clean_url(self) -> str:
-        url = self.cleaned_data.get('url')
+        url: str = self.cleaned_data.get('url', '')
         if url:
             raise ValidationError('url should be empty')
         return url
 
     def clean_load_time(self) -> float:
-        load_time = self.cleaned_data.get('load_time')
+        cleaned_load_time: str = self.cleaned_data.get('load_time', '')
         try:
-            load_time = float(load_time)
+            load_time = float(cleaned_load_time)
         except ValueError:
             raise ValidationError('Invalid value')
 
         shown_field_count = 0
         spam_fields = ['load_time', 'url']
         for name, field in self.fields.items():
             if field.widget.input_type != 'hidden' and name not in spam_fields:
```

### Comparing `django-magiclink-1.2.0/magiclink/helpers.py` & `django_magiclink-1.3.0/magiclink/helpers.py`

 * *Files identical despite different names*

### Comparing `django-magiclink-1.2.0/magiclink/management/commands/magiclink_clear_logins.py` & `django_magiclink-1.3.0/magiclink/management/commands/magiclink_clear_logins.py`

 * *Files identical despite different names*

### Comparing `django-magiclink-1.2.0/magiclink/migrations/0001_initial.py` & `django_magiclink-1.3.0/magiclink/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-magiclink-1.2.0/magiclink/migrations/0002_magiclinkunsubscribe.py` & `django_magiclink-1.3.0/magiclink/migrations/0002_magiclinkunsubscribe.py`

 * *Files identical despite different names*

### Comparing `django-magiclink-1.2.0/magiclink/models.py` & `django_magiclink-1.3.0/magiclink/models.py`

 * *Files identical despite different names*

### Comparing `django-magiclink-1.2.0/magiclink/settings.py` & `django_magiclink-1.3.0/magiclink/settings.py`

 * *Files identical despite different names*

### Comparing `django-magiclink-1.2.0/magiclink/templates/magiclink/login.html` & `django_magiclink-1.3.0/magiclink/templates/magiclink/login.html`

 * *Files identical despite different names*

### Comparing `django-magiclink-1.2.0/magiclink/templates/magiclink/login_email.html` & `django_magiclink-1.3.0/magiclink/templates/magiclink/login_email.html`

 * *Files identical despite different names*

### Comparing `django-magiclink-1.2.0/magiclink/templates/magiclink/login_failed.html` & `django_magiclink-1.3.0/magiclink/templates/magiclink/login_failed.html`

 * *Files identical despite different names*

### Comparing `django-magiclink-1.2.0/magiclink/templates/magiclink/login_sent.html` & `django_magiclink-1.3.0/magiclink/templates/magiclink/login_sent.html`

 * *Files identical despite different names*

### Comparing `django-magiclink-1.2.0/magiclink/templates/magiclink/signup.html` & `django_magiclink-1.3.0/magiclink/templates/magiclink/signup.html`

 * *Files identical despite different names*

### Comparing `django-magiclink-1.2.0/magiclink/utils.py` & `django_magiclink-1.3.0/magiclink/utils.py`

 * *Files identical despite different names*

### Comparing `django-magiclink-1.2.0/magiclink/views.py` & `django_magiclink-1.3.0/magiclink/views.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from django.views.decorators.cache import never_cache
 from django.views.generic import TemplateView
 from django.views.generic.base import RedirectView
 
 try:
     from django.utils.http import url_has_allowed_host_and_scheme as safe_url
 except ImportError:  # pragma: no cover
-    from django.utils.http import is_safe_url as safe_url
+    from django.utils.http import is_safe_url as safe_url  # type: ignore
 
 from django.views.decorators.csrf import csrf_protect
 
 from . import settings
 from .forms import (
     LoginForm, SignupForm, SignupFormEmailOnly, SignupFormFull,
     SignupFormWithUsername
```

### Comparing `django-magiclink-1.2.0/pyproject.toml` & `django_magiclink-1.3.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 [tool.poetry]
 name = "django-magiclink"
 packages = [
     {include = "magiclink"}
 ]
-version = "1.2.0"
+version = "1.3.0"
 description = "Passwordless authentication for Django with Magic Links"
 authors = ["Matt Pye <pyematt@gmail.com>"]
 readme = "README.md"
 license = "MIT"
 repository = "https://github.com/pyepye/django-magiclink"
 homepage = "https://github.com/pyepye/django-magiclink"
 keywords = ["magic link", "authentication", "passwordless"]
 
 [tool.poetry.dependencies]
 python = "^3.6"
 Django = ">=2.1"
-packaging = "^20.9"
+packaging = ">=20.9,<22.0"
 
 [tool.poetry.dev-dependencies]
-flake8 = "^3.8.3"
-tox = "^3.17.0"
+flake8 = "^4.0.1"
+tox = "^3.28.0"
 isort = {extras = ["pyproject"], version = "^5.4.2"}
 django-stubs = "^1.5.0"
-pytest = "^5.4.3"
-pytest-cov = "^2.10.0"
-pytest-django = "^3.9.0"
+pytest = "^7.0.1"
+pytest-cov = "^4.0.0"
+pytest-django = "^4.5.2"
 pytest-mock = "^3.2.0"
 pytest-freezegun = "^0.4.1"
 
 [tool.isort]
 line_length = 79
 multi_line_output = 5
 known_third_party = "pytest"
```

### Comparing `django-magiclink-1.2.0/setup.py` & `django_magiclink-1.3.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,33 +1,467 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: django-magiclink
+Version: 1.3.0
+Summary: Passwordless authentication for Django with Magic Links
+Home-page: https://github.com/pyepye/django-magiclink
+License: MIT
+Keywords: magic link,authentication,passwordless
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
+Requires-Dist: packaging (>=20.9,<22.0)
+Project-URL: Repository, https://github.com/pyepye/django-magiclink
+Description-Content-Type: text/markdown
 
-packages = \
-['magiclink',
- 'magiclink.management',
- 'magiclink.management.commands',
- 'magiclink.migrations']
-
-package_data = \
-{'': ['*'], 'magiclink': ['templates/magiclink/*']}
-
-install_requires = \
-['Django>=2.1', 'packaging>=20.9,<21.0']
-
-setup_kwargs = {
-    'name': 'django-magiclink',
-    'version': '1.2.0',
-    'description': 'Passwordless authentication for Django with Magic Links',
-    'long_description': '# Django MagicLink\n\n\nPasswordless Authentication for Django with Magic Links.\n\nThis package was created with a focus on [ease of setup](#steps-to-impliment), [security](#security) and testing (coverage is currently at 100%). The idea is to use sane defaults to quickly create secure single-use token authentication for Django.\n\n![](example.gif)\n\n\n## Install\n\n```bash\npip install django-magiclink\n```\n\n## Setup\n\nThe setup of the app is simple but has a few steps and a few templates that need overriding.\n\n1. [Install the app](#install)\n1. [Configure the app](#configuration) adding urls and settings. There are also a number of [additional configuration settings](#configuration-settings)\n1. [Set up the login page](#login-page) by overriding the login page template\n1. [Override the login sent page HTML](#login-sent-page)\n1. [Customise the login failed page](#login-failed-page)\n1. [Set up the magic link email](#magic-link-email) (optional) by setting the email logo and colours. It\'s also possible to override the email templates\n1. [Create a signup page](#signup-page) (optional) depending on your settings configuration\n\n\n### Basic login flow\n\n1. The user signs up via the sign up page (This can be skipped if `MAGICLINK_REQUIRE_SIGNUP = False`)\n1. They enter their email on the login page to request a magic link\n1. A magic link is sent to users email address\n1. The user is redirected to a login sent page\n1. The user clicks on the magic link in their email\n1. The user is logged in and redirected\n\n\n*If you want to create a different passwordless login flow see the [Manual usage](#manual-usage) section*\n\n\n#### Configuration\n\nAdd to the `urlpatterns` in `urls.py`:\n```python\nurlpatterns = [\n    ...\n    path(\'auth/\', include(\'magiclink.urls\', namespace=\'magiclink\')),\n    ...\n]\n```\n\nAdd `magiclink` to your `INSTALLED_APPS`:\n```python\nINSTALLED_APPS = (\n    ...\n    \'magiclink\',\n    ...\n)\n```\n\n```python\nAUTHENTICATION_BACKENDS = (\n    \'magiclink.backends.MagicLinkBackend\',\n    ...\n    \'django.contrib.auth.backends.ModelBackend\',\n)\n```\n*Note: MagicLinkBackend should be placed at the top of AUTHENTICATION_BACKENDS* to ensure it is used as the primary login backend.\n\n\nAdd the following settings to your `settings.py` (you will need to replace the template names in the below steps):\n```python\n# Set Djangos login URL to the magiclink login page\nLOGIN_URL = \'magiclink:login\'\n\nMAGICLINK_LOGIN_TEMPLATE_NAME = \'magiclink/login.html\'\nMAGICLINK_LOGIN_SENT_TEMPLATE_NAME = \'magiclink/login_sent.html\'\nMAGICLINK_LOGIN_FAILED_TEMPLATE_NAME = \'magiclink/login_failed.html\'\n\n# Optional:\n# If this setting is set to False a user account will be created the first\n# time a user requests a login link.\nMAGICLINK_REQUIRE_SIGNUP = True\nMAGICLINK_SIGNUP_TEMPLATE_NAME = \'magiclink/signup.html\'\n```\n\nSee [additional configuration settings](#configuration-settings) for all of the different available settings.\n\n\nOnce the app has been added to `INSTALLED_APPS` you must run the migrations for `magiclink`\n\n```bash\npython manage.py migrate magiclink\n```\n\n#### Login page\n\nEach login page will need different HTML so you need to set the `MAGICLINK_LOGIN_TEMPLATE_NAME` setting to a template of your own. When overriding this template please ensure the following code is included:\n\n```html\n<form action="{% url \'magiclink:login\' %}{% if request.GET.next %}?next={{ request.GET.next }}{% endif %}" method="post">\n    {% csrf_token %}\n    {{ login_form }}\n    <button type=\'submit\'>Send login email</button>\n</form>\n```\n\nSee the login docs if you want to create your own login view\n\n\n#### Login sent page\n\nAfter the user has requested a magic link, they will be redirected to a success page. The HTML for this page can be overridden using the setting `MAGICLINK_LOGIN_SENT_TEMPLATE_NAME`. It is advised you return a simple message telling the user to check their email:\n\n```html\n<h1>Check your email</h1>\n<p>We have sent you a magic link to your email address</p>\n<p>Please click the link to be logged in automatically</p>\n```\n\n\n#### Login failed page\n\nIf the user tries to use an invalid magic token they will be shown a custom error page. To override the HTML for this page you can set the `MAGICLINK_LOGIN_FAILED_TEMPLATE_NAME` setting. If you would like to return a 404 page you can set this setting to a empty string (or any falsy value). If you would like to redirect to another page (say a custom front-end) you can use the `MAGICLINK_LOGIN_FAILED_REDIRECT` setting.\n\nThe reasons for the login failing is passed through as the context variable `{{ login_error }}`\n\nTo help tailor the error page and explain the possible reasons the user could not login the following context variables are provided:\n\n* `{{ login_error }}` - The reason the login failed (raised by `MagicLink.validate()`)\n* `{{ one_token_per_user }}` - The value of the `MAGICLINK_ONE_TOKEN_PER_USER` setting\n* `{{ require_same_browser }}` - The value of the `MAGICLINK_REQUIRE_SAME_BROWSER` setting\n* `{{ require_same_ip }}` - The value of the `MAGICLINK_REQUIRE_SAME_IP` setting\n* `{{ allow_superuser_login }}` - The value of the `MAGICLINK_ALLOW_SUPERUSER_LOGIN` setting\n* `{{ allow_staff_login }}` - The value of the `MAGICLINK_ALLOW_STAFF_LOGIN` setting\n\n\nFor an example of this page see the [default login failed template](https://github.com/pyepye/django-magiclink/blob/master/magiclink/templates/magiclink/login_failed.html)\n\n\n#### Magic link email\n\nThe login email which includes the magic link needs to be configured. By default, a simple HTML template is used which can be adapted to your own branding using the `MAGICLINK_EMAIL_STYLES` setting, or you can override the template (see below)\n\nThis `MAGICLINK_EMAIL_STYLES` setting should be a dict with the following key values:\n\n```python\nMAGICLINK_EMAIL_STYLES = {\n    \'logo_url\': \'https://example.com/logo.png\',\n    \'background-colour\': \'#ffffff\',\n    \'main-text-color\': \'#000000\',\n    \'button-background-color\': \'#0078be\',\n    \'button-text-color\': \'#ffffff\',\n}\n```\n*Note: The logo URL must be a full URL. For email client support you should use either a jpeg or png.*\n\nIf this email template is not to your liking you can override the email templates (one for text and one for html). To do so you need to override the `MAGICLINK_EMAIL_TEMPLATE_NAME_TEXT` and `MAGICLINK_EMAIL_TEMPLATE_NAME_HTML` settings.  If you override these templates the following context variables are available:\n\n* `{{ subject }}` - The subject of the email "Your login magic link"\n* `{{ magiclink }}` - The magic link URL\n* `{{ user }}` - The full user object\n* `{{ expiry }}` - Datetime for when the magiclink expires\n* `{{ ip_address }}` - The IP address of the person who requested the magic link\n* `{{ created }}` - Datetime of when the magic link was created\n* `{{ require_same_ip }}` - The value of `MAGICLINK_REQUIRE_SAME_IP`\n* `{{ require_same_browser }}` - The value of `MAGICLINK_REQUIRE_SAME_BROWSER`\n* `{{ token_uses }}` - The value of `MAGICLINK_TOKEN_USES`\n\n\n#### Signup page\n\nIf you want users to have to signup before being able to log in you will want to override the signup page template using the `MAGICLINK_SIGNUP_TEMPLATE_NAME` setting. This is needed when `MAGICLINK_REQUIRE_SIGNUP = True`. On successful signup the user will be sent a login email with a magic link.\n\nWhen overriding this template please ensure the following content is included:\n\n```html\n<form action="{% url \'magiclink:signup\' %}" method="post">\n    {% csrf_token %}\n    {{ SignupForm }}\n    <button type=\'submit\'>Signup</button>\n</form>\n<p>Already have an account? <a href=\'{% url \'magiclink:login\' %}\'>Log in here</a></p>\n```\n\nThere are several forms made avalible in the context on this page depending on what information you want to collect:\n* **SignupFormEmailOnly** - Only includes an `email` field\n* **SignupForm** - Includes `name` and `email` fields\n* **SignupFormWithUsername** - Includes `username` and `email` fields\n* **SignupFormFull** - Includes `username`, `name` and `email` fields\n\n\nLike the login for the sign up flow can be overridden if you require more information from the user on signup. See the login/setup docs for more details.\n\n\n#### Configuration settings\n\nBelow are the different settings that can be overridden. To do so place the setting into your `settings.py`.\n\n*Note: Each of the url / redirect settings can either be a URL or url name*\n\n```python\n\n# Override the login page template. See \'Login page\' in the Setup section\nMAGICLINK_LOGIN_TEMPLATE_NAME = \'myapp/login.html\'\n\n# Override the login page template. See \'Login sent page\' in the Setup section\nMAGICLINK_LOGIN_SENT_TEMPLATE_NAME = \'myapp/login_sent.html\'\n\n# Override the template that shows when the user tries to login with a\n# magic link that is not valid. See \'Login failed page\' in the Setup section\nMAGICLINK_LOGIN_FAILED_TEMPLATE_NAME = \'magiclink/login_failed.html\'\n\n# If a login failed redirect is specified the user will be redirected to this\n# URL instead of being shown the LOGIN_FAILED_TEMPLATE\nMAGICLINK_LOGIN_FAILED_REDIRECT = \'\'\n\n# If this setting is set to False a user account will be created the first time\n# a user requests a login link.\nMAGICLINK_REQUIRE_SIGNUP = True\n# Override the login page template. See \'Login sent page\' in the Setup section\nMAGICLINK_SIGNUP_TEMPLATE_NAME = \'myapp/signup.html\'\n\n# Set Djangos login redirect URL to be used once the user opens the magic link\n# This will be used whenever a ?next parameter is not set on login\nLOGIN_REDIRECT_URL = \'/accounts/profile/\'\n\n# If a new user is created via the signup page use this setting to send them to\n# a different url than LOGIN_REDIRECT_URL when clicking the magic link\n# This will fall back to LOGIN_REDIRECT_URL\nMAGICLINK_SIGNUP_LOGIN_REDIRECT = \'/welcome/\'\n\n# Change the url a user is redirect to after requesting a magic link\nMAGICLINK_LOGIN_SENT_REDIRECT = \'magiclink:login_sent\'\n\n# Ensure the branding of the login email is correct. This setting is not needed\n# if you override the `login_email.html` template\nMAGICLINK_EMAIL_STYLES = {\n    \'logo_url\': \'\',\n    \'background-colour\': \'#ffffff\',\n    \'main-text-color\': \'#000000\',\n    \'button-background-color\': \'#0078be\',\n    \'button-text-color\': \'#ffffff\',\n}\n\n# If you want to use your own email templates you can override the text and\n# html templates used with:\nMAGICLINK_EMAIL_TEMPLATE_NAME_TEXT = \'myapp/login_email.text\'\nMAGICLINK_EMAIL_TEMPLATE_NAME_HTML = \'myapp/login_email.html\'\n\n# How long a magic link is valid for before returning an error\nMAGICLINK_AUTH_TIMEOUT = 300  # In second - Default is 5 minutes\n\n# Email address is not case sensitive. If this setting is set to True all\n# emails addresses will be set to lowercase before any checks are run against it\nMAGICLINK_IGNORE_EMAIL_CASE = True\n\n# When creating a user assign their email as the username (if the User model\n# has a username field)\nMAGICLINK_EMAIL_AS_USERNAME = True\n\n# Allow superusers to login via a magic link\nMAGICLINK_ALLOW_SUPERUSER_LOGIN = True\n\n# Allow staff users to login via a magic link\nMAGICLINK_ALLOW_STAFF_LOGIN = True\n\n# Ignore the Django user model\'s is_active flag for login requests\nMAGICLINK_IGNORE_IS_ACTIVE_FLAG = True\n\n# Override the default magic link length\n# Warning: Overriding this setting has security implications, shorter tokens\n# are much more susceptible to brute force attacks*\nMAGICLINK_TOKEN_LENGTH = 50\n\n# Require the user email to be included in the verification link\n# Warning: If this is set to false tokens are more vulnerable to brute force\nMAGICLINK_VERIFY_INCLUDE_EMAIL = True\n\n# Ensure the user who clicked magic link used the same browser as the\n# initial login request.\n# Note: This can cause issues on devices where the default browser is\n# different from the browser being used by the user such as on iOS)\nMAGICLINK_REQUIRE_SAME_BROWSER = True\n\n# Ensure the user who clicked magic link has the same IP address as the\n# initial login request.\nMAGICLINK_REQUIRE_SAME_IP = True\n\n# Remove the last 8-bit octet of a clients IP address.\n# Note: This has no effect if MAGICLINK_REQUIRE_SAME_IP as no IP address\n# is stored\nMAGICLINK_ANONYMIZE_IP = True\n\n# The number of times a login token can be used before being disabled\nMAGICLINK_TOKEN_USES = 1\n\n# How often a user can request a new login token (basic rate limiting).\nMAGICLINK_LOGIN_REQUEST_TIME_LIMIT = 30  # In seconds\n\n# Disable all other tokens for a user when a new token is requested\nMAGICLINK_ONE_TOKEN_PER_USER = True\n\n# Include basic anti spam form fields to help stop bots. False by default\n# Note: IF you use the default forms you will need to add CSS to your\n# page / stylesheet to hide the labels for the anti spam fields.\n# See the login.html or signup.html for an example\nMAGICLINK_ANTISPAM_FORMS = False\n# The shortest time a user can fill out each field and submit a form without\n# being considered a bot. The time is per field and defaults to 1 second.\n# This means if the form has 3 fields and the user will need to make more than\n# 3 seconds to fill out a form.\nMAGICLINK_ANTISPAM_FIELD_TIME = 1\n\n# Override the login verify address. You must inherit from Magiclink LoginVerify\n# view. See Manual usage for more details\nMAGICLINK_LOGIN_VERIFY_URL = \'magiclink:login_verify\'\n\n# If an email address has been added to the unsubscribe table but is also\n# assocaited with a Django user, should a login email be sent\nMAGICLINK_IGNORE_UNSUBSCRIBE_IF_USER = False\n```\n\n## Magic Link cleanup\n\nEach Magic Link is a seperate row in the database. To help give the user a better warning as to why their login was not successful, magic links are not cleared even once they have expired or have been disabled.\n\nTo clear old disabled magic links as well as magic links which expired over 1 week ago, you can use the `magiclink_clear_logins` management command\n\n```\npython manage.py magiclink_clear_logins\n```\n\n\n## Security\n\nUsing magic links can be dangerous as poorly implemented login links can be brute-forced and emails can be forwarded by accident. There are several security measures used to mitigate these risks:\n\n* The one-time password issued will be valid for 5 minutes before it expires\n* The user\'s email is specified alongside login tokens to stop URLs being brute-forced\n* Each login token will be at least 20 digits\n* The initial request and its response must take place from the same IP address\n* The initial request and its response must take place in the same browser\n* Each one-time link can only be used once\n* Only the last one-time link issued will be accepted. Once the latest one is issued, any others are invalidated.\n\n*Note: Each of the above settings can be overridden / changed when configuring django-magiclink*\n\n\n## Unsubscribe / stopping email spam\n\nSadly bots like to go around the internet and fill out any forms they can with random email addresses that don\'t belong to them. Because of this, if an email is added to the `MagicLinkUnsubscribe` model they will no longer receive a login or welcome email, even if the email has a user associated with it. This behaviour can be changed for existing users using the `MAGICLINK_IGNORE_UNSUBSCRIBE_IF_USER` setting.\n\nAdding a user to the unsubscribe model is done using the normal Django ORM create method\n\n```python\nfrom magiclink.models import MagicLinkUnsubscribe\n\nMagicLinkUnsubscribe.objects.create(email=\'test@example.com\')\n```\n\nIf you are using the Django Magiclink login or signup functionality, the unsubscribe check happens during form validation. This means a new user will never be created if their email address has already been added to the `MagicLinkUnsubscribe` list.\n\n\n## Manual usage\n\n### Creating magiclinks\n\ndjango-magiclink uses a model to help create, send and validate magic links. A `create_magiclink` helper function can be used easily create a MagicLink using the correct settings:\n\n```python\nfrom magiclink.helpers import create_magiclink\n\n# Returns newly created from magiclink.models.MagicLink instance\nmagiclink = create_magiclink(email, request, redirect_url=\'\')\n\n# Generates the magic link url and sends it in an email\nmagiclink.send(request)\n\n# If you want to build the magic link from the model instance but don\'t want to\n#  send the email you can you can use:\nmagic_link_url = magiclink.generate_url(request)\n```\n\n### Custom Login verify flow\n\nIt is also possible to override the login verify flow to run your own code once the user has successfully logged in instead of a simple redirect. To do this you will need to create a new view which inherits the `magiclink.views.LoginVerify` view and overrides the `login_complete_action` method.\n\nThe below example will redirect the user to a different page depending on superuser / staff status:\n\n\nYour own `views.py`\n\n```python\nfrom magiclink.views import LoginVerify\n\n\nclass CustomLoginVerify(LoginVerify):\n\n    def login_complete_action(self):\n        if self.request.user.is_superuser:\n            url = reverse(\'superuser_page\')\n        elif self.request.user.is_staff:\n            url = reverse(\'staff_page\')\n        else:\n            url = reverse(\'normal_page\')\n        return HttpResponseRedirect(url)\n```\n\n\nYour own `urls.py`\n\n```python\nurlpatterns = [\n    ...\n    path(\n        \'custom-login-verify/\',\n        CustomLoginVerify.as_view(),\n        name=\'custom_login_verify\'\n    ),\n    ...\n]\n```\n\n\n`settings.py`\n\n```python\n...\nMAGICLINK_LOGIN_VERIFY_URL = \'custom_login_verify\'\n...\n```\n\n\n## Upgrading\n\nA new migration was added to version `1.2.0`. If you upgrade to `1.2.0` or above from a previous version please ensure you migrate\n\n```bash\npython manage.py migrate magiclink\n```\n',
-    'author': 'Matt Pye',
-    'author_email': 'pyematt@gmail.com',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/pyepye/django-magiclink',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.6,<4.0',
+# Django MagicLink
+
+
+Passwordless Authentication for Django with Magic Links.
+
+This package was created with a focus on [ease of setup](#steps-to-impliment), [security](#security) and testing (coverage is currently at 100%). The idea is to use sane defaults to quickly create secure single-use token authentication for Django.
+
+![](example.gif)
+
+
+## Install
+
+```bash
+pip install django-magiclink
+```
+
+## Setup
+
+The setup of the app is simple but has a few steps and a few templates that need overriding.
+
+1. [Install the app](#install)
+1. [Configure the app](#configuration) adding urls and settings. There are also a number of [additional configuration settings](#configuration-settings)
+1. [Set up the login page](#login-page) by overriding the login page template
+1. [Override the login sent page HTML](#login-sent-page)
+1. [Customise the login failed page](#login-failed-page)
+1. [Set up the magic link email](#magic-link-email) (optional) by setting the email logo and colours. It's also possible to override the email templates
+1. [Create a signup page](#signup-page) (optional) depending on your settings configuration
+
+
+### Basic login flow
+
+1. The user signs up via the sign up page (This can be skipped if `MAGICLINK_REQUIRE_SIGNUP = False`)
+1. They enter their email on the login page to request a magic link
+1. A magic link is sent to users email address
+1. The user is redirected to a login sent page
+1. The user clicks on the magic link in their email
+1. The user is logged in and redirected
+
+
+*If you want to create a different passwordless login flow see the [Manual usage](#manual-usage) section*
+
+
+#### Configuration
+
+Add to the `urlpatterns` in `urls.py`:
+```python
+urlpatterns = [
+    ...
+    path('auth/', include('magiclink.urls', namespace='magiclink')),
+    ...
+]
+```
+
+Add `magiclink` to your `INSTALLED_APPS`:
+```python
+INSTALLED_APPS = (
+    ...
+    'magiclink',
+    ...
+)
+```
+
+```python
+AUTHENTICATION_BACKENDS = (
+    'magiclink.backends.MagicLinkBackend',
+    ...
+    'django.contrib.auth.backends.ModelBackend',
+)
+```
+*Note: MagicLinkBackend should be placed at the top of AUTHENTICATION_BACKENDS* to ensure it is used as the primary login backend.
+
+
+Add the following settings to your `settings.py` (you will need to replace the template names in the below steps):
+```python
+# Set Djangos login URL to the magiclink login page
+LOGIN_URL = 'magiclink:login'
+
+MAGICLINK_LOGIN_TEMPLATE_NAME = 'magiclink/login.html'
+MAGICLINK_LOGIN_SENT_TEMPLATE_NAME = 'magiclink/login_sent.html'
+MAGICLINK_LOGIN_FAILED_TEMPLATE_NAME = 'magiclink/login_failed.html'
+
+# Optional:
+# If this setting is set to False a user account will be created the first
+# time a user requests a login link.
+MAGICLINK_REQUIRE_SIGNUP = True
+MAGICLINK_SIGNUP_TEMPLATE_NAME = 'magiclink/signup.html'
+```
+
+See [additional configuration settings](#configuration-settings) for all of the different available settings.
+
+
+Once the app has been added to `INSTALLED_APPS` you must run the migrations for `magiclink`
+
+```bash
+python manage.py migrate magiclink
+```
+
+#### Login page
+
+Each login page will need different HTML so you need to set the `MAGICLINK_LOGIN_TEMPLATE_NAME` setting to a template of your own. When overriding this template please ensure the following code is included:
+
+```html
+<form action="{% url 'magiclink:login' %}{% if request.GET.next %}?next={{ request.GET.next }}{% endif %}" method="post">
+    {% csrf_token %}
+    {{ login_form }}
+    <button type='submit'>Send login email</button>
+</form>
+```
+
+See the login docs if you want to create your own login view
+
+
+#### Login sent page
+
+After the user has requested a magic link, they will be redirected to a success page. The HTML for this page can be overridden using the setting `MAGICLINK_LOGIN_SENT_TEMPLATE_NAME`. It is advised you return a simple message telling the user to check their email:
+
+```html
+<h1>Check your email</h1>
+<p>We have sent you a magic link to your email address</p>
+<p>Please click the link to be logged in automatically</p>
+```
+
+
+#### Login failed page
+
+If the user tries to use an invalid magic token they will be shown a custom error page. To override the HTML for this page you can set the `MAGICLINK_LOGIN_FAILED_TEMPLATE_NAME` setting. If you would like to return a 404 page you can set this setting to a empty string (or any falsy value). If you would like to redirect to another page (say a custom front-end) you can use the `MAGICLINK_LOGIN_FAILED_REDIRECT` setting.
+
+The reasons for the login failing is passed through as the context variable `{{ login_error }}`
+
+To help tailor the error page and explain the possible reasons the user could not login the following context variables are provided:
+
+* `{{ login_error }}` - The reason the login failed (raised by `MagicLink.validate()`)
+* `{{ one_token_per_user }}` - The value of the `MAGICLINK_ONE_TOKEN_PER_USER` setting
+* `{{ require_same_browser }}` - The value of the `MAGICLINK_REQUIRE_SAME_BROWSER` setting
+* `{{ require_same_ip }}` - The value of the `MAGICLINK_REQUIRE_SAME_IP` setting
+* `{{ allow_superuser_login }}` - The value of the `MAGICLINK_ALLOW_SUPERUSER_LOGIN` setting
+* `{{ allow_staff_login }}` - The value of the `MAGICLINK_ALLOW_STAFF_LOGIN` setting
+
+
+For an example of this page see the [default login failed template](https://github.com/pyepye/django-magiclink/blob/master/magiclink/templates/magiclink/login_failed.html)
+
+
+#### Magic link email
+
+The login email which includes the magic link needs to be configured. By default, a simple HTML template is used which can be adapted to your own branding using the `MAGICLINK_EMAIL_STYLES` setting, or you can override the template (see below)
+
+This `MAGICLINK_EMAIL_STYLES` setting should be a dict with the following key values:
+
+```python
+MAGICLINK_EMAIL_STYLES = {
+    'logo_url': 'https://example.com/logo.png',
+    'background-colour': '#ffffff',
+    'main-text-color': '#000000',
+    'button-background-color': '#0078be',
+    'button-text-color': '#ffffff',
+}
+```
+*Note: The logo URL must be a full URL. For email client support you should use either a jpeg or png.*
+
+If this email template is not to your liking you can override the email templates (one for text and one for html). To do so you need to override the `MAGICLINK_EMAIL_TEMPLATE_NAME_TEXT` and `MAGICLINK_EMAIL_TEMPLATE_NAME_HTML` settings.  If you override these templates the following context variables are available:
+
+* `{{ subject }}` - The subject of the email "Your login magic link"
+* `{{ magiclink }}` - The magic link URL
+* `{{ user }}` - The full user object
+* `{{ expiry }}` - Datetime for when the magiclink expires
+* `{{ ip_address }}` - The IP address of the person who requested the magic link
+* `{{ created }}` - Datetime of when the magic link was created
+* `{{ require_same_ip }}` - The value of `MAGICLINK_REQUIRE_SAME_IP`
+* `{{ require_same_browser }}` - The value of `MAGICLINK_REQUIRE_SAME_BROWSER`
+* `{{ token_uses }}` - The value of `MAGICLINK_TOKEN_USES`
+
+
+#### Signup page
+
+If you want users to have to signup before being able to log in you will want to override the signup page template using the `MAGICLINK_SIGNUP_TEMPLATE_NAME` setting. This is needed when `MAGICLINK_REQUIRE_SIGNUP = True`. On successful signup the user will be sent a login email with a magic link.
+
+When overriding this template please ensure the following content is included:
+
+```html
+<form action="{% url 'magiclink:signup' %}" method="post">
+    {% csrf_token %}
+    {{ SignupForm }}
+    <button type='submit'>Signup</button>
+</form>
+<p>Already have an account? <a href='{% url 'magiclink:login' %}'>Log in here</a></p>
+```
+
+There are several forms made avalible in the context on this page depending on what information you want to collect:
+* **SignupFormEmailOnly** - Only includes an `email` field
+* **SignupForm** - Includes `name` and `email` fields
+* **SignupFormWithUsername** - Includes `username` and `email` fields
+* **SignupFormFull** - Includes `username`, `name` and `email` fields
+
+
+Like the login for the sign up flow can be overridden if you require more information from the user on signup. See the login/setup docs for more details.
+
+
+#### Configuration settings
+
+Below are the different settings that can be overridden. To do so place the setting into your `settings.py`.
+
+*Note: Each of the url / redirect settings can either be a URL or url name*
+
+```python
+
+# Override the login page template. See 'Login page' in the Setup section
+MAGICLINK_LOGIN_TEMPLATE_NAME = 'myapp/login.html'
+
+# Override the login page template. See 'Login sent page' in the Setup section
+MAGICLINK_LOGIN_SENT_TEMPLATE_NAME = 'myapp/login_sent.html'
+
+# Override the template that shows when the user tries to login with a
+# magic link that is not valid. See 'Login failed page' in the Setup section
+MAGICLINK_LOGIN_FAILED_TEMPLATE_NAME = 'magiclink/login_failed.html'
+
+# If a login failed redirect is specified the user will be redirected to this
+# URL instead of being shown the LOGIN_FAILED_TEMPLATE
+MAGICLINK_LOGIN_FAILED_REDIRECT = ''
+
+# If this setting is set to False a user account will be created the first time
+# a user requests a login link.
+MAGICLINK_REQUIRE_SIGNUP = True
+# Override the login page template. See 'Login sent page' in the Setup section
+MAGICLINK_SIGNUP_TEMPLATE_NAME = 'myapp/signup.html'
+
+# Set Djangos login redirect URL to be used once the user opens the magic link
+# This will be used whenever a ?next parameter is not set on login
+LOGIN_REDIRECT_URL = '/accounts/profile/'
+
+# If a new user is created via the signup page use this setting to send them to
+# a different url than LOGIN_REDIRECT_URL when clicking the magic link
+# This will fall back to LOGIN_REDIRECT_URL
+MAGICLINK_SIGNUP_LOGIN_REDIRECT = '/welcome/'
+
+# Change the url a user is redirect to after requesting a magic link
+MAGICLINK_LOGIN_SENT_REDIRECT = 'magiclink:login_sent'
+
+# Ensure the branding of the login email is correct. This setting is not needed
+# if you override the `login_email.html` template
+MAGICLINK_EMAIL_STYLES = {
+    'logo_url': '',
+    'background-colour': '#ffffff',
+    'main-text-color': '#000000',
+    'button-background-color': '#0078be',
+    'button-text-color': '#ffffff',
 }
 
+# If you want to use your own email templates you can override the text and
+# html templates used with:
+MAGICLINK_EMAIL_TEMPLATE_NAME_TEXT = 'myapp/login_email.text'
+MAGICLINK_EMAIL_TEMPLATE_NAME_HTML = 'myapp/login_email.html'
+
+# How long a magic link is valid for before returning an error
+MAGICLINK_AUTH_TIMEOUT = 300  # In second - Default is 5 minutes
+
+# Email address is not case sensitive. If this setting is set to True all
+# emails addresses will be set to lowercase before any checks are run against it
+MAGICLINK_IGNORE_EMAIL_CASE = True
+
+# When creating a user assign their email as the username (if the User model
+# has a username field)
+MAGICLINK_EMAIL_AS_USERNAME = True
+
+# Allow superusers to login via a magic link
+MAGICLINK_ALLOW_SUPERUSER_LOGIN = True
+
+# Allow staff users to login via a magic link
+MAGICLINK_ALLOW_STAFF_LOGIN = True
+
+# Ignore the Django user model's is_active flag for login requests
+MAGICLINK_IGNORE_IS_ACTIVE_FLAG = True
+
+# Override the default magic link length
+# Warning: Overriding this setting has security implications, shorter tokens
+# are much more susceptible to brute force attacks*
+MAGICLINK_TOKEN_LENGTH = 50
+
+# Require the user email to be included in the verification link
+# Warning: If this is set to false tokens are more vulnerable to brute force
+MAGICLINK_VERIFY_INCLUDE_EMAIL = True
+
+# Ensure the user who clicked magic link used the same browser as the
+# initial login request.
+# Note: This can cause issues on devices where the default browser is
+# different from the browser being used by the user such as on iOS)
+MAGICLINK_REQUIRE_SAME_BROWSER = True
+
+# Ensure the user who clicked magic link has the same IP address as the
+# initial login request.
+MAGICLINK_REQUIRE_SAME_IP = True
+
+# Remove the last 8-bit octet of a clients IP address.
+# Note: This has no effect if MAGICLINK_REQUIRE_SAME_IP as no IP address
+# is stored
+MAGICLINK_ANONYMIZE_IP = True
+
+# The number of times a login token can be used before being disabled
+MAGICLINK_TOKEN_USES = 1
+
+# How often a user can request a new login token (basic rate limiting).
+MAGICLINK_LOGIN_REQUEST_TIME_LIMIT = 30  # In seconds
+
+# Disable all other tokens for a user when a new token is requested
+MAGICLINK_ONE_TOKEN_PER_USER = True
+
+# Include basic anti spam form fields to help stop bots. False by default
+# Note: IF you use the default forms you will need to add CSS to your
+# page / stylesheet to hide the labels for the anti spam fields.
+# See the login.html or signup.html for an example
+MAGICLINK_ANTISPAM_FORMS = False
+# The shortest time a user can fill out each field and submit a form without
+# being considered a bot. The time is per field and defaults to 1 second.
+# This means if the form has 3 fields and the user will need to make more than
+# 3 seconds to fill out a form.
+MAGICLINK_ANTISPAM_FIELD_TIME = 1
+
+# Override the login verify address. You must inherit from Magiclink LoginVerify
+# view. See Manual usage for more details
+MAGICLINK_LOGIN_VERIFY_URL = 'magiclink:login_verify'
+
+# If an email address has been added to the unsubscribe table but is also
+# assocaited with a Django user, should a login email be sent
+MAGICLINK_IGNORE_UNSUBSCRIBE_IF_USER = False
+```
+
+## Magic Link cleanup
+
+Each Magic Link is a seperate row in the database. To help give the user a better warning as to why their login was not successful, magic links are not cleared even once they have expired or have been disabled.
+
+To clear old disabled magic links as well as magic links which expired over 1 week ago, you can use the `magiclink_clear_logins` management command
+
+```
+python manage.py magiclink_clear_logins
+```
+
+
+## Security
+
+Using magic links can be dangerous as poorly implemented login links can be brute-forced and emails can be forwarded by accident. There are several security measures used to mitigate these risks:
+
+* The one-time password issued will be valid for 5 minutes before it expires
+* The user's email is specified alongside login tokens to stop URLs being brute-forced
+* Each login token will be at least 20 digits
+* The initial request and its response must take place from the same IP address
+* The initial request and its response must take place in the same browser
+* Each one-time link can only be used once
+* Only the last one-time link issued will be accepted. Once the latest one is issued, any others are invalidated.
+
+*Note: Each of the above settings can be overridden / changed when configuring django-magiclink*
+
+
+## Unsubscribe / stopping email spam
+
+Sadly bots like to go around the internet and fill out any forms they can with random email addresses that don't belong to them. Because of this, if an email is added to the `MagicLinkUnsubscribe` model they will no longer receive a login or welcome email, even if the email has a user associated with it. This behaviour can be changed for existing users using the `MAGICLINK_IGNORE_UNSUBSCRIBE_IF_USER` setting.
+
+Adding a user to the unsubscribe model is done using the normal Django ORM create method
+
+```python
+from magiclink.models import MagicLinkUnsubscribe
+
+MagicLinkUnsubscribe.objects.create(email='test@example.com')
+```
+
+If you are using the Django Magiclink login or signup functionality, the unsubscribe check happens during form validation. This means a new user will never be created if their email address has already been added to the `MagicLinkUnsubscribe` list.
+
+
+## Manual usage
+
+### Creating magiclinks
+
+django-magiclink uses a model to help create, send and validate magic links. A `create_magiclink` helper function can be used easily create a MagicLink using the correct settings:
+
+```python
+from magiclink.helpers import create_magiclink
+
+# Returns newly created from magiclink.models.MagicLink instance
+magiclink = create_magiclink(email, request, redirect_url='')
+
+# Generates the magic link url and sends it in an email
+magiclink.send(request)
+
+# If you want to build the magic link from the model instance but don't want to
+#  send the email you can you can use:
+magic_link_url = magiclink.generate_url(request)
+```
+
+### Custom Login verify flow
+
+It is also possible to override the login verify flow to run your own code once the user has successfully logged in instead of a simple redirect. To do this you will need to create a new view which inherits the `magiclink.views.LoginVerify` view and overrides the `login_complete_action` method.
+
+The below example will redirect the user to a different page depending on superuser / staff status:
+
+
+Your own `views.py`
+
+```python
+from magiclink.views import LoginVerify
+
+
+class CustomLoginVerify(LoginVerify):
+
+    def login_complete_action(self):
+        if self.request.user.is_superuser:
+            url = reverse('superuser_page')
+        elif self.request.user.is_staff:
+            url = reverse('staff_page')
+        else:
+            url = reverse('normal_page')
+        return HttpResponseRedirect(url)
+```
+
+
+Your own `urls.py`
+
+```python
+urlpatterns = [
+    ...
+    path(
+        'custom-login-verify/',
+        CustomLoginVerify.as_view(),
+        name='custom_login_verify'
+    ),
+    ...
+]
+```
+
+
+`settings.py`
+
+```python
+...
+MAGICLINK_LOGIN_VERIFY_URL = 'custom_login_verify'
+...
+```
+
+
+## Upgrading
+
+A new migration was added to version `1.2.0`. If you upgrade to `1.2.0` or above from a previous version please ensure you migrate
+
+```bash
+python manage.py migrate magiclink
+```
 
-setup(**setup_kwargs)
```

