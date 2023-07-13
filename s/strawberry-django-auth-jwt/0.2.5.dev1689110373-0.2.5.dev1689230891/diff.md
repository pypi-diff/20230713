# Comparing `tmp/strawberry_django_auth_jwt-0.2.5.dev1689110373.tar.gz` & `tmp/strawberry_django_auth_jwt-0.2.5.dev1689230891.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "strawberry_django_auth_jwt-0.2.5.dev1689110373.tar", max compression
+gzip compressed data, was "strawberry_django_auth_jwt-0.2.5.dev1689230891.tar", max compression
```

## Comparing `strawberry_django_auth_jwt-0.2.5.dev1689110373.tar` & `strawberry_django_auth_jwt-0.2.5.dev1689230891.tar`

### file list

```diff
@@ -1,60 +1,60 @@
--rw-r--r--   0        0        0     1074 2023-07-11 21:19:11.942256 strawberry_django_auth_jwt-0.2.5.dev1689110373/LICENSE
--rw-r--r--   0        0        0     7446 2023-07-11 21:19:11.942256 strawberry_django_auth_jwt-0.2.5.dev1689110373/README.md
--rw-r--r--   0        0        0     3102 2023-07-11 21:19:33.458588 strawberry_django_auth_jwt-0.2.5.dev1689110373/pyproject.toml
--rw-r--r--   0        0        0      248 2023-07-11 21:19:11.942256 strawberry_django_auth_jwt-0.2.5.dev1689110373/strawberry_django_jwt/__init__.py
--rw-r--r--   0        0        0     2409 2023-07-11 21:19:31.582558 strawberry_django_auth_jwt-0.2.5.dev1689110373/strawberry_django_jwt/auth.py
--rw-r--r--   0        0        0      859 2023-07-11 21:19:11.942256 strawberry_django_auth_jwt-0.2.5.dev1689110373/strawberry_django_jwt/backends.py
--rw-r--r--   0        0        0    10340 2023-07-11 21:19:11.942256 strawberry_django_auth_jwt-0.2.5.dev1689110373/strawberry_django_jwt/decorators.py
--rw-r--r--   0        0        0      482 2023-07-11 21:19:11.942256 strawberry_django_auth_jwt-0.2.5.dev1689110373/strawberry_django_jwt/exceptions.py
--rw-r--r--   0        0        0      576 2023-07-11 21:19:11.942256 strawberry_django_auth_jwt-0.2.5.dev1689110373/strawberry_django_jwt/fields.py
--rw-r--r--   0        0        0     1191 2023-07-11 21:19:11.942256 strawberry_django_auth_jwt-0.2.5.dev1689110373/strawberry_django_jwt/locale/ar/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     1570 2023-07-11 21:19:11.942256 strawberry_django_auth_jwt-0.2.5.dev1689110373/strawberry_django_jwt/locale/ar/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1039 2023-07-11 21:19:11.942256 strawberry_django_auth_jwt-0.2.5.dev1689110373/strawberry_django_jwt/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     1413 2023-07-11 21:19:11.942256 strawberry_django_auth_jwt-0.2.5.dev1689110373/strawberry_django_jwt/locale/es/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1078 2023-07-11 21:19:11.942256 strawberry_django_auth_jwt-0.2.5.dev1689110373/strawberry_django_jwt/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     1453 2023-07-11 21:19:11.942256 strawberry_django_auth_jwt-0.2.5.dev1689110373/strawberry_django_jwt/locale/fr/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1043 2023-07-11 21:19:11.942256 strawberry_django_auth_jwt-0.2.5.dev1689110373/strawberry_django_jwt/locale/nl/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     1303 2023-07-11 21:19:11.942256 strawberry_django_auth_jwt-0.2.5.dev1689110373/strawberry_django_jwt/locale/nl/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1069 2023-07-11 21:19:11.942256 strawberry_django_auth_jwt-0.2.5.dev1689110373/strawberry_django_jwt/locale/pt_BR/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     1443 2023-07-11 21:19:11.942256 strawberry_django_auth_jwt-0.2.5.dev1689110373/strawberry_django_jwt/locale/pt_BR/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     4656 2023-07-11 21:19:11.942256 strawberry_django_auth_jwt-0.2.5.dev1689110373/strawberry_django_jwt/middleware.py
--rw-r--r--   0        0        0     7267 2023-07-11 21:19:11.942256 strawberry_django_auth_jwt-0.2.5.dev1689110373/strawberry_django_jwt/mixins.py
--rw-r--r--   0        0        0     1015 2023-07-11 21:19:11.942256 strawberry_django_auth_jwt-0.2.5.dev1689110373/strawberry_django_jwt/model_object_types.py
--rw-r--r--   0        0        0     2600 2023-07-11 21:19:11.942256 strawberry_django_auth_jwt-0.2.5.dev1689110373/strawberry_django_jwt/mutations.py
--rw-r--r--   0        0        0     1148 2023-07-11 21:19:11.942256 strawberry_django_auth_jwt-0.2.5.dev1689110373/strawberry_django_jwt/object_types.py
--rw-r--r--   0        0        0      651 2023-07-11 21:19:11.942256 strawberry_django_auth_jwt-0.2.5.dev1689110373/strawberry_django_jwt/path.py
--rw-r--r--   0        0        0        0 2023-07-11 21:19:11.942256 strawberry_django_auth_jwt-0.2.5.dev1689110373/strawberry_django_jwt/refresh_token/__init__.py
--rw-r--r--   0        0        0      899 2023-07-11 21:19:11.942256 strawberry_django_auth_jwt-0.2.5.dev1689110373/strawberry_django_jwt/refresh_token/admin/__init__.py
--rw-r--r--   0        0        0     1035 2023-07-11 21:19:11.942256 strawberry_django_auth_jwt-0.2.5.dev1689110373/strawberry_django_jwt/refresh_token/admin/filters.py
--rw-r--r--   0        0        0      243 2023-07-11 21:19:11.942256 strawberry_django_auth_jwt-0.2.5.dev1689110373/strawberry_django_jwt/refresh_token/apps.py
--rw-r--r--   0        0        0      820 2023-07-11 21:19:11.942256 strawberry_django_auth_jwt-0.2.5.dev1689110373/strawberry_django_jwt/refresh_token/decorators.py
--rw-r--r--   0        0        0     1119 2023-07-11 21:19:11.942256 strawberry_django_auth_jwt-0.2.5.dev1689110373/strawberry_django_jwt/refresh_token/locale/ar/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     1742 2023-07-11 21:19:11.942256 strawberry_django_auth_jwt-0.2.5.dev1689110373/strawberry_django_jwt/refresh_token/locale/ar/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1051 2023-07-11 21:19:11.942256 strawberry_django_auth_jwt-0.2.5.dev1689110373/strawberry_django_jwt/refresh_token/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     1603 2023-07-11 21:19:11.942256 strawberry_django_auth_jwt-0.2.5.dev1689110373/strawberry_django_jwt/refresh_token/locale/es/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1135 2023-07-11 21:19:11.942256 strawberry_django_auth_jwt-0.2.5.dev1689110373/strawberry_django_jwt/refresh_token/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     1658 2023-07-11 21:19:11.942256 strawberry_django_auth_jwt-0.2.5.dev1689110373/strawberry_django_jwt/refresh_token/locale/fr/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1102 2023-07-11 21:19:11.942256 strawberry_django_auth_jwt-0.2.5.dev1689110373/strawberry_django_jwt/refresh_token/locale/nl/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     1504 2023-07-11 21:19:11.942256 strawberry_django_auth_jwt-0.2.5.dev1689110373/strawberry_django_jwt/refresh_token/locale/nl/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1144 2023-07-11 21:19:11.942256 strawberry_django_auth_jwt-0.2.5.dev1689110373/strawberry_django_jwt/refresh_token/locale/pt_BR/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     1847 2023-07-11 21:19:11.942256 strawberry_django_auth_jwt-0.2.5.dev1689110373/strawberry_django_jwt/refresh_token/locale/pt_BR/LC_MESSAGES/django.po
--rw-r--r--   0        0        0        0 2023-07-11 21:19:11.942256 strawberry_django_auth_jwt-0.2.5.dev1689110373/strawberry_django_jwt/refresh_token/management/__init__.py
--rw-r--r--   0        0        0        0 2023-07-11 21:19:11.942256 strawberry_django_auth_jwt-0.2.5.dev1689110373/strawberry_django_jwt/refresh_token/management/commands/__init__.py
--rw-r--r--   0        0        0      857 2023-07-11 21:19:11.942256 strawberry_django_auth_jwt-0.2.5.dev1689110373/strawberry_django_jwt/refresh_token/management/commands/cleartokens.py
--rw-r--r--   0        0        0      605 2023-07-11 21:19:11.942256 strawberry_django_auth_jwt-0.2.5.dev1689110373/strawberry_django_jwt/refresh_token/managers.py
--rw-r--r--   0        0        0     1659 2023-07-11 21:19:11.942256 strawberry_django_auth_jwt-0.2.5.dev1689110373/strawberry_django_jwt/refresh_token/migrations/0001_initial.py
--rw-r--r--   0        0        0      395 2023-07-11 21:19:11.942256 strawberry_django_auth_jwt-0.2.5.dev1689110373/strawberry_django_jwt/refresh_token/migrations/0002_auto_20190130_0900.py
--rw-r--r--   0        0        0        0 2023-07-11 21:19:11.942256 strawberry_django_auth_jwt-0.2.5.dev1689110373/strawberry_django_jwt/refresh_token/migrations/__init__.py
--rw-r--r--   0        0        0     2229 2023-07-11 21:19:11.942256 strawberry_django_auth_jwt-0.2.5.dev1689110373/strawberry_django_jwt/refresh_token/models.py
--rw-r--r--   0        0        0     1137 2023-07-11 21:19:11.942256 strawberry_django_auth_jwt-0.2.5.dev1689110373/strawberry_django_jwt/refresh_token/mutations.py
--rw-r--r--   0        0        0      314 2023-07-11 21:19:11.942256 strawberry_django_auth_jwt-0.2.5.dev1689110373/strawberry_django_jwt/refresh_token/object_types.py
--rw-r--r--   0        0        0     1418 2023-07-11 21:19:11.942256 strawberry_django_auth_jwt-0.2.5.dev1689110373/strawberry_django_jwt/refresh_token/shortcuts.py
--rw-r--r--   0        0        0      219 2023-07-11 21:19:11.942256 strawberry_django_auth_jwt-0.2.5.dev1689110373/strawberry_django_jwt/refresh_token/signals.py
--rw-r--r--   0        0        0      337 2023-07-11 21:19:11.942256 strawberry_django_auth_jwt-0.2.5.dev1689110373/strawberry_django_jwt/refresh_token/utils.py
--rw-r--r--   0        0        0     4423 2023-07-11 21:19:11.942256 strawberry_django_auth_jwt-0.2.5.dev1689110373/strawberry_django_jwt/settings.py
--rw-r--r--   0        0        0      936 2023-07-11 21:19:11.942256 strawberry_django_auth_jwt-0.2.5.dev1689110373/strawberry_django_jwt/shortcuts.py
--rw-r--r--   0        0        0      162 2023-07-11 21:19:11.942256 strawberry_django_auth_jwt-0.2.5.dev1689110373/strawberry_django_jwt/signals.py
--rw-r--r--   0        0        0     4144 2023-07-11 21:19:11.942256 strawberry_django_auth_jwt-0.2.5.dev1689110373/strawberry_django_jwt/testcases.py
--rw-r--r--   0        0        0     8771 2023-07-11 21:19:11.942256 strawberry_django_auth_jwt-0.2.5.dev1689110373/strawberry_django_jwt/utils.py
--rw-r--r--   0        0        0     1859 2023-07-11 21:19:11.942256 strawberry_django_auth_jwt-0.2.5.dev1689110373/strawberry_django_jwt/views.py
--rw-r--r--   0        0        0     9096 1970-01-01 00:00:00.000000 strawberry_django_auth_jwt-0.2.5.dev1689110373/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-07-13 06:47:47.222758 strawberry_django_auth_jwt-0.2.5.dev1689230891/LICENSE
+-rw-r--r--   0        0        0     7446 2023-07-13 06:47:47.222758 strawberry_django_auth_jwt-0.2.5.dev1689230891/README.md
+-rw-r--r--   0        0        0     3102 2023-07-13 06:48:12.333071 strawberry_django_auth_jwt-0.2.5.dev1689230891/pyproject.toml
+-rw-r--r--   0        0        0      248 2023-07-13 06:47:47.222758 strawberry_django_auth_jwt-0.2.5.dev1689230891/strawberry_django_jwt/__init__.py
+-rw-r--r--   0        0        0     2409 2023-07-13 06:47:47.222758 strawberry_django_auth_jwt-0.2.5.dev1689230891/strawberry_django_jwt/auth.py
+-rw-r--r--   0        0        0      859 2023-07-13 06:47:47.222758 strawberry_django_auth_jwt-0.2.5.dev1689230891/strawberry_django_jwt/backends.py
+-rw-r--r--   0        0        0    10340 2023-07-13 06:47:47.222758 strawberry_django_auth_jwt-0.2.5.dev1689230891/strawberry_django_jwt/decorators.py
+-rw-r--r--   0        0        0      482 2023-07-13 06:47:47.222758 strawberry_django_auth_jwt-0.2.5.dev1689230891/strawberry_django_jwt/exceptions.py
+-rw-r--r--   0        0        0      576 2023-07-13 06:47:47.222758 strawberry_django_auth_jwt-0.2.5.dev1689230891/strawberry_django_jwt/fields.py
+-rw-r--r--   0        0        0     1191 2023-07-13 06:47:47.222758 strawberry_django_auth_jwt-0.2.5.dev1689230891/strawberry_django_jwt/locale/ar/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     1570 2023-07-13 06:47:47.222758 strawberry_django_auth_jwt-0.2.5.dev1689230891/strawberry_django_jwt/locale/ar/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1039 2023-07-13 06:47:47.222758 strawberry_django_auth_jwt-0.2.5.dev1689230891/strawberry_django_jwt/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     1413 2023-07-13 06:47:47.222758 strawberry_django_auth_jwt-0.2.5.dev1689230891/strawberry_django_jwt/locale/es/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1078 2023-07-13 06:47:47.222758 strawberry_django_auth_jwt-0.2.5.dev1689230891/strawberry_django_jwt/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     1453 2023-07-13 06:47:47.222758 strawberry_django_auth_jwt-0.2.5.dev1689230891/strawberry_django_jwt/locale/fr/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1043 2023-07-13 06:47:47.222758 strawberry_django_auth_jwt-0.2.5.dev1689230891/strawberry_django_jwt/locale/nl/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     1303 2023-07-13 06:47:47.222758 strawberry_django_auth_jwt-0.2.5.dev1689230891/strawberry_django_jwt/locale/nl/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1069 2023-07-13 06:47:47.222758 strawberry_django_auth_jwt-0.2.5.dev1689230891/strawberry_django_jwt/locale/pt_BR/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     1443 2023-07-13 06:47:47.222758 strawberry_django_auth_jwt-0.2.5.dev1689230891/strawberry_django_jwt/locale/pt_BR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     4656 2023-07-13 06:47:47.222758 strawberry_django_auth_jwt-0.2.5.dev1689230891/strawberry_django_jwt/middleware.py
+-rw-r--r--   0        0        0     7267 2023-07-13 06:47:47.222758 strawberry_django_auth_jwt-0.2.5.dev1689230891/strawberry_django_jwt/mixins.py
+-rw-r--r--   0        0        0     1015 2023-07-13 06:47:47.222758 strawberry_django_auth_jwt-0.2.5.dev1689230891/strawberry_django_jwt/model_object_types.py
+-rw-r--r--   0        0        0     2600 2023-07-13 06:47:47.222758 strawberry_django_auth_jwt-0.2.5.dev1689230891/strawberry_django_jwt/mutations.py
+-rw-r--r--   0        0        0     1148 2023-07-13 06:47:47.222758 strawberry_django_auth_jwt-0.2.5.dev1689230891/strawberry_django_jwt/object_types.py
+-rw-r--r--   0        0        0      651 2023-07-13 06:47:47.222758 strawberry_django_auth_jwt-0.2.5.dev1689230891/strawberry_django_jwt/path.py
+-rw-r--r--   0        0        0        0 2023-07-13 06:47:47.222758 strawberry_django_auth_jwt-0.2.5.dev1689230891/strawberry_django_jwt/refresh_token/__init__.py
+-rw-r--r--   0        0        0      899 2023-07-13 06:47:47.226759 strawberry_django_auth_jwt-0.2.5.dev1689230891/strawberry_django_jwt/refresh_token/admin/__init__.py
+-rw-r--r--   0        0        0     1035 2023-07-13 06:47:47.226759 strawberry_django_auth_jwt-0.2.5.dev1689230891/strawberry_django_jwt/refresh_token/admin/filters.py
+-rw-r--r--   0        0        0      243 2023-07-13 06:47:47.226759 strawberry_django_auth_jwt-0.2.5.dev1689230891/strawberry_django_jwt/refresh_token/apps.py
+-rw-r--r--   0        0        0      820 2023-07-13 06:47:47.226759 strawberry_django_auth_jwt-0.2.5.dev1689230891/strawberry_django_jwt/refresh_token/decorators.py
+-rw-r--r--   0        0        0     1119 2023-07-13 06:47:47.226759 strawberry_django_auth_jwt-0.2.5.dev1689230891/strawberry_django_jwt/refresh_token/locale/ar/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     1742 2023-07-13 06:47:47.226759 strawberry_django_auth_jwt-0.2.5.dev1689230891/strawberry_django_jwt/refresh_token/locale/ar/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1051 2023-07-13 06:47:47.226759 strawberry_django_auth_jwt-0.2.5.dev1689230891/strawberry_django_jwt/refresh_token/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     1603 2023-07-13 06:47:47.226759 strawberry_django_auth_jwt-0.2.5.dev1689230891/strawberry_django_jwt/refresh_token/locale/es/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1135 2023-07-13 06:47:47.226759 strawberry_django_auth_jwt-0.2.5.dev1689230891/strawberry_django_jwt/refresh_token/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     1658 2023-07-13 06:47:47.226759 strawberry_django_auth_jwt-0.2.5.dev1689230891/strawberry_django_jwt/refresh_token/locale/fr/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1102 2023-07-13 06:47:47.226759 strawberry_django_auth_jwt-0.2.5.dev1689230891/strawberry_django_jwt/refresh_token/locale/nl/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     1504 2023-07-13 06:47:47.226759 strawberry_django_auth_jwt-0.2.5.dev1689230891/strawberry_django_jwt/refresh_token/locale/nl/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1144 2023-07-13 06:47:47.226759 strawberry_django_auth_jwt-0.2.5.dev1689230891/strawberry_django_jwt/refresh_token/locale/pt_BR/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     1847 2023-07-13 06:47:47.226759 strawberry_django_auth_jwt-0.2.5.dev1689230891/strawberry_django_jwt/refresh_token/locale/pt_BR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0        0 2023-07-13 06:47:47.226759 strawberry_django_auth_jwt-0.2.5.dev1689230891/strawberry_django_jwt/refresh_token/management/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-13 06:47:47.226759 strawberry_django_auth_jwt-0.2.5.dev1689230891/strawberry_django_jwt/refresh_token/management/commands/__init__.py
+-rw-r--r--   0        0        0      857 2023-07-13 06:47:47.226759 strawberry_django_auth_jwt-0.2.5.dev1689230891/strawberry_django_jwt/refresh_token/management/commands/cleartokens.py
+-rw-r--r--   0        0        0      605 2023-07-13 06:47:47.226759 strawberry_django_auth_jwt-0.2.5.dev1689230891/strawberry_django_jwt/refresh_token/managers.py
+-rw-r--r--   0        0        0     1659 2023-07-13 06:47:47.226759 strawberry_django_auth_jwt-0.2.5.dev1689230891/strawberry_django_jwt/refresh_token/migrations/0001_initial.py
+-rw-r--r--   0        0        0      395 2023-07-13 06:47:47.226759 strawberry_django_auth_jwt-0.2.5.dev1689230891/strawberry_django_jwt/refresh_token/migrations/0002_auto_20190130_0900.py
+-rw-r--r--   0        0        0        0 2023-07-13 06:47:47.226759 strawberry_django_auth_jwt-0.2.5.dev1689230891/strawberry_django_jwt/refresh_token/migrations/__init__.py
+-rw-r--r--   0        0        0     2229 2023-07-13 06:47:47.226759 strawberry_django_auth_jwt-0.2.5.dev1689230891/strawberry_django_jwt/refresh_token/models.py
+-rw-r--r--   0        0        0     1137 2023-07-13 06:47:47.226759 strawberry_django_auth_jwt-0.2.5.dev1689230891/strawberry_django_jwt/refresh_token/mutations.py
+-rw-r--r--   0        0        0      314 2023-07-13 06:47:47.226759 strawberry_django_auth_jwt-0.2.5.dev1689230891/strawberry_django_jwt/refresh_token/object_types.py
+-rw-r--r--   0        0        0     1418 2023-07-13 06:47:47.226759 strawberry_django_auth_jwt-0.2.5.dev1689230891/strawberry_django_jwt/refresh_token/shortcuts.py
+-rw-r--r--   0        0        0      219 2023-07-13 06:47:47.226759 strawberry_django_auth_jwt-0.2.5.dev1689230891/strawberry_django_jwt/refresh_token/signals.py
+-rw-r--r--   0        0        0      337 2023-07-13 06:47:47.226759 strawberry_django_auth_jwt-0.2.5.dev1689230891/strawberry_django_jwt/refresh_token/utils.py
+-rw-r--r--   0        0        0     4423 2023-07-13 06:47:47.226759 strawberry_django_auth_jwt-0.2.5.dev1689230891/strawberry_django_jwt/settings.py
+-rw-r--r--   0        0        0      936 2023-07-13 06:47:47.226759 strawberry_django_auth_jwt-0.2.5.dev1689230891/strawberry_django_jwt/shortcuts.py
+-rw-r--r--   0        0        0      162 2023-07-13 06:47:47.226759 strawberry_django_auth_jwt-0.2.5.dev1689230891/strawberry_django_jwt/signals.py
+-rw-r--r--   0        0        0     4144 2023-07-13 06:47:47.226759 strawberry_django_auth_jwt-0.2.5.dev1689230891/strawberry_django_jwt/testcases.py
+-rw-r--r--   0        0        0     8771 2023-07-13 06:47:47.226759 strawberry_django_auth_jwt-0.2.5.dev1689230891/strawberry_django_jwt/utils.py
+-rw-r--r--   0        0        0     1859 2023-07-13 06:47:47.226759 strawberry_django_auth_jwt-0.2.5.dev1689230891/strawberry_django_jwt/views.py
+-rw-r--r--   0        0        0     9096 1970-01-01 00:00:00.000000 strawberry_django_auth_jwt-0.2.5.dev1689230891/PKG-INFO
```

### Comparing `strawberry_django_auth_jwt-0.2.5.dev1689110373/LICENSE` & `strawberry_django_auth_jwt-0.2.5.dev1689230891/LICENSE`

 * *Files identical despite different names*

### Comparing `strawberry_django_auth_jwt-0.2.5.dev1689110373/README.md` & `strawberry_django_auth_jwt-0.2.5.dev1689230891/README.md`

 * *Files identical despite different names*

### Comparing `strawberry_django_auth_jwt-0.2.5.dev1689110373/pyproject.toml` & `strawberry_django_auth_jwt-0.2.5.dev1689230891/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "strawberry-django-auth-jwt"
-version = "0.2.5.dev.1689110373"
+version = "0.2.5.dev.1689230891"
 description = "Strawberry-graphql port of the graphene-django-jwt package"
 license = "MIT"
 authors = ["Javier Borrego <javierborregocejudo@gmail.com>"]
 maintainers = []
 readme = "README.md"
 classifiers = [
     'Development Status :: 3 - Alpha',
```

### Comparing `strawberry_django_auth_jwt-0.2.5.dev1689110373/strawberry_django_jwt/auth.py` & `strawberry_django_auth_jwt-0.2.5.dev1689230891/strawberry_django_jwt/auth.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_auth_jwt-0.2.5.dev1689110373/strawberry_django_jwt/backends.py` & `strawberry_django_auth_jwt-0.2.5.dev1689230891/strawberry_django_jwt/backends.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_auth_jwt-0.2.5.dev1689110373/strawberry_django_jwt/decorators.py` & `strawberry_django_auth_jwt-0.2.5.dev1689230891/strawberry_django_jwt/decorators.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_auth_jwt-0.2.5.dev1689110373/strawberry_django_jwt/fields.py` & `strawberry_django_auth_jwt-0.2.5.dev1689230891/strawberry_django_jwt/fields.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_auth_jwt-0.2.5.dev1689110373/strawberry_django_jwt/locale/ar/LC_MESSAGES/django.mo` & `strawberry_django_auth_jwt-0.2.5.dev1689230891/strawberry_django_jwt/locale/ar/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `strawberry_django_auth_jwt-0.2.5.dev1689110373/strawberry_django_jwt/locale/ar/LC_MESSAGES/django.po` & `strawberry_django_auth_jwt-0.2.5.dev1689230891/strawberry_django_jwt/locale/ar/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `strawberry_django_auth_jwt-0.2.5.dev1689110373/strawberry_django_jwt/locale/es/LC_MESSAGES/django.mo` & `strawberry_django_auth_jwt-0.2.5.dev1689230891/strawberry_django_jwt/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `strawberry_django_auth_jwt-0.2.5.dev1689110373/strawberry_django_jwt/locale/es/LC_MESSAGES/django.po` & `strawberry_django_auth_jwt-0.2.5.dev1689230891/strawberry_django_jwt/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `strawberry_django_auth_jwt-0.2.5.dev1689110373/strawberry_django_jwt/locale/fr/LC_MESSAGES/django.mo` & `strawberry_django_auth_jwt-0.2.5.dev1689230891/strawberry_django_jwt/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `strawberry_django_auth_jwt-0.2.5.dev1689110373/strawberry_django_jwt/locale/fr/LC_MESSAGES/django.po` & `strawberry_django_auth_jwt-0.2.5.dev1689230891/strawberry_django_jwt/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `strawberry_django_auth_jwt-0.2.5.dev1689110373/strawberry_django_jwt/locale/nl/LC_MESSAGES/django.mo` & `strawberry_django_auth_jwt-0.2.5.dev1689230891/strawberry_django_jwt/locale/nl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `strawberry_django_auth_jwt-0.2.5.dev1689110373/strawberry_django_jwt/locale/nl/LC_MESSAGES/django.po` & `strawberry_django_auth_jwt-0.2.5.dev1689230891/strawberry_django_jwt/locale/nl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `strawberry_django_auth_jwt-0.2.5.dev1689110373/strawberry_django_jwt/locale/pt_BR/LC_MESSAGES/django.mo` & `strawberry_django_auth_jwt-0.2.5.dev1689230891/strawberry_django_jwt/locale/pt_BR/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `strawberry_django_auth_jwt-0.2.5.dev1689110373/strawberry_django_jwt/locale/pt_BR/LC_MESSAGES/django.po` & `strawberry_django_auth_jwt-0.2.5.dev1689230891/strawberry_django_jwt/locale/pt_BR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `strawberry_django_auth_jwt-0.2.5.dev1689110373/strawberry_django_jwt/middleware.py` & `strawberry_django_auth_jwt-0.2.5.dev1689230891/strawberry_django_jwt/middleware.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_auth_jwt-0.2.5.dev1689110373/strawberry_django_jwt/mixins.py` & `strawberry_django_auth_jwt-0.2.5.dev1689230891/strawberry_django_jwt/mixins.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_auth_jwt-0.2.5.dev1689110373/strawberry_django_jwt/model_object_types.py` & `strawberry_django_auth_jwt-0.2.5.dev1689230891/strawberry_django_jwt/model_object_types.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_auth_jwt-0.2.5.dev1689110373/strawberry_django_jwt/mutations.py` & `strawberry_django_auth_jwt-0.2.5.dev1689230891/strawberry_django_jwt/mutations.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_auth_jwt-0.2.5.dev1689110373/strawberry_django_jwt/object_types.py` & `strawberry_django_auth_jwt-0.2.5.dev1689230891/strawberry_django_jwt/object_types.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_auth_jwt-0.2.5.dev1689110373/strawberry_django_jwt/path.py` & `strawberry_django_auth_jwt-0.2.5.dev1689230891/strawberry_django_jwt/path.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_auth_jwt-0.2.5.dev1689110373/strawberry_django_jwt/refresh_token/admin/__init__.py` & `strawberry_django_auth_jwt-0.2.5.dev1689230891/strawberry_django_jwt/refresh_token/admin/__init__.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_auth_jwt-0.2.5.dev1689110373/strawberry_django_jwt/refresh_token/admin/filters.py` & `strawberry_django_auth_jwt-0.2.5.dev1689230891/strawberry_django_jwt/refresh_token/admin/filters.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_auth_jwt-0.2.5.dev1689110373/strawberry_django_jwt/refresh_token/decorators.py` & `strawberry_django_auth_jwt-0.2.5.dev1689230891/strawberry_django_jwt/refresh_token/decorators.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_auth_jwt-0.2.5.dev1689110373/strawberry_django_jwt/refresh_token/locale/ar/LC_MESSAGES/django.mo` & `strawberry_django_auth_jwt-0.2.5.dev1689230891/strawberry_django_jwt/refresh_token/locale/ar/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `strawberry_django_auth_jwt-0.2.5.dev1689110373/strawberry_django_jwt/refresh_token/locale/ar/LC_MESSAGES/django.po` & `strawberry_django_auth_jwt-0.2.5.dev1689230891/strawberry_django_jwt/refresh_token/locale/ar/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `strawberry_django_auth_jwt-0.2.5.dev1689110373/strawberry_django_jwt/refresh_token/locale/es/LC_MESSAGES/django.mo` & `strawberry_django_auth_jwt-0.2.5.dev1689230891/strawberry_django_jwt/refresh_token/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `strawberry_django_auth_jwt-0.2.5.dev1689110373/strawberry_django_jwt/refresh_token/locale/es/LC_MESSAGES/django.po` & `strawberry_django_auth_jwt-0.2.5.dev1689230891/strawberry_django_jwt/refresh_token/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `strawberry_django_auth_jwt-0.2.5.dev1689110373/strawberry_django_jwt/refresh_token/locale/fr/LC_MESSAGES/django.mo` & `strawberry_django_auth_jwt-0.2.5.dev1689230891/strawberry_django_jwt/refresh_token/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `strawberry_django_auth_jwt-0.2.5.dev1689110373/strawberry_django_jwt/refresh_token/locale/fr/LC_MESSAGES/django.po` & `strawberry_django_auth_jwt-0.2.5.dev1689230891/strawberry_django_jwt/refresh_token/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `strawberry_django_auth_jwt-0.2.5.dev1689110373/strawberry_django_jwt/refresh_token/locale/nl/LC_MESSAGES/django.mo` & `strawberry_django_auth_jwt-0.2.5.dev1689230891/strawberry_django_jwt/refresh_token/locale/nl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `strawberry_django_auth_jwt-0.2.5.dev1689110373/strawberry_django_jwt/refresh_token/locale/nl/LC_MESSAGES/django.po` & `strawberry_django_auth_jwt-0.2.5.dev1689230891/strawberry_django_jwt/refresh_token/locale/nl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `strawberry_django_auth_jwt-0.2.5.dev1689110373/strawberry_django_jwt/refresh_token/locale/pt_BR/LC_MESSAGES/django.mo` & `strawberry_django_auth_jwt-0.2.5.dev1689230891/strawberry_django_jwt/refresh_token/locale/pt_BR/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `strawberry_django_auth_jwt-0.2.5.dev1689110373/strawberry_django_jwt/refresh_token/locale/pt_BR/LC_MESSAGES/django.po` & `strawberry_django_auth_jwt-0.2.5.dev1689230891/strawberry_django_jwt/refresh_token/locale/pt_BR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `strawberry_django_auth_jwt-0.2.5.dev1689110373/strawberry_django_jwt/refresh_token/management/commands/cleartokens.py` & `strawberry_django_auth_jwt-0.2.5.dev1689230891/strawberry_django_jwt/refresh_token/management/commands/cleartokens.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_auth_jwt-0.2.5.dev1689110373/strawberry_django_jwt/refresh_token/managers.py` & `strawberry_django_auth_jwt-0.2.5.dev1689230891/strawberry_django_jwt/refresh_token/managers.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_auth_jwt-0.2.5.dev1689110373/strawberry_django_jwt/refresh_token/migrations/0001_initial.py` & `strawberry_django_auth_jwt-0.2.5.dev1689230891/strawberry_django_jwt/refresh_token/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_auth_jwt-0.2.5.dev1689110373/strawberry_django_jwt/refresh_token/models.py` & `strawberry_django_auth_jwt-0.2.5.dev1689230891/strawberry_django_jwt/refresh_token/models.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_auth_jwt-0.2.5.dev1689110373/strawberry_django_jwt/refresh_token/mutations.py` & `strawberry_django_auth_jwt-0.2.5.dev1689230891/strawberry_django_jwt/refresh_token/mutations.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_auth_jwt-0.2.5.dev1689110373/strawberry_django_jwt/refresh_token/shortcuts.py` & `strawberry_django_auth_jwt-0.2.5.dev1689230891/strawberry_django_jwt/refresh_token/shortcuts.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_auth_jwt-0.2.5.dev1689110373/strawberry_django_jwt/settings.py` & `strawberry_django_auth_jwt-0.2.5.dev1689230891/strawberry_django_jwt/settings.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_auth_jwt-0.2.5.dev1689110373/strawberry_django_jwt/shortcuts.py` & `strawberry_django_auth_jwt-0.2.5.dev1689230891/strawberry_django_jwt/shortcuts.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_auth_jwt-0.2.5.dev1689110373/strawberry_django_jwt/testcases.py` & `strawberry_django_auth_jwt-0.2.5.dev1689230891/strawberry_django_jwt/testcases.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_auth_jwt-0.2.5.dev1689110373/strawberry_django_jwt/utils.py` & `strawberry_django_auth_jwt-0.2.5.dev1689230891/strawberry_django_jwt/utils.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_auth_jwt-0.2.5.dev1689110373/strawberry_django_jwt/views.py` & `strawberry_django_auth_jwt-0.2.5.dev1689230891/strawberry_django_jwt/views.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_auth_jwt-0.2.5.dev1689110373/PKG-INFO` & `strawberry_django_auth_jwt-0.2.5.dev1689230891/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: strawberry-django-auth-jwt
-Version: 0.2.5.dev1689110373
+Version: 0.2.5.dev1689230891
 Summary: Strawberry-graphql port of the graphene-django-jwt package
 License: MIT
 Author: Javier Borrego
 Author-email: javierborregocejudo@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Web Environment
```

