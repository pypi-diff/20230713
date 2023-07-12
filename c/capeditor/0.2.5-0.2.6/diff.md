# Comparing `tmp/capeditor-0.2.5.tar.gz` & `tmp/capeditor-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "capeditor-0.2.5.tar", last modified: Wed Jul 12 12:31:49 2023, max compression
+gzip compressed data, was "capeditor-0.2.6.tar", last modified: Wed Jul 12 21:55:05 2023, max compression
```

## Comparing `capeditor-0.2.5.tar` & `capeditor-0.2.6.tar`

### file list

```diff
@@ -1,83 +1,83 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:31:49.684218 capeditor-0.2.5/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-12 12:31:32.000000 capeditor-0.2.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8191 2023-07-12 12:31:49.684218 capeditor-0.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7323 2023-07-12 12:31:32.000000 capeditor-0.2.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:31:49.680219 capeditor-0.2.5/capeditor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 12:31:32.000000 capeditor-0.2.5/capeditor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-12 12:31:32.000000 capeditor-0.2.5/capeditor/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-07-12 12:31:32.000000 capeditor-0.2.5/capeditor/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)    23816 2023-07-12 12:31:32.000000 capeditor-0.2.5/capeditor/blocks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:31:49.680219 capeditor-0.2.5/capeditor/forms/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 12:31:32.000000 capeditor-0.2.5/capeditor/forms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-07-12 12:31:32.000000 capeditor-0.2.5/capeditor/forms/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     5673 2023-07-12 12:31:32.000000 capeditor-0.2.5/capeditor/forms/widgets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:31:49.676219 capeditor-0.2.5/capeditor/locale/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:31:49.676219 capeditor-0.2.5/capeditor/locale/am/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:31:49.680219 capeditor-0.2.5/capeditor/locale/am/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    20372 2023-07-12 12:31:32.000000 capeditor-0.2.5/capeditor/locale/am/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    30677 2023-07-12 12:31:32.000000 capeditor-0.2.5/capeditor/locale/am/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:31:49.676219 capeditor-0.2.5/capeditor/locale/ar/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:31:49.680219 capeditor-0.2.5/capeditor/locale/ar/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    19629 2023-07-12 12:31:32.000000 capeditor-0.2.5/capeditor/locale/ar/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    30023 2023-07-12 12:31:32.000000 capeditor-0.2.5/capeditor/locale/ar/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:31:49.676219 capeditor-0.2.5/capeditor/locale/en/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:31:49.680219 capeditor-0.2.5/capeditor/locale/en/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    16403 2023-07-12 12:31:32.000000 capeditor-0.2.5/capeditor/locale/en/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    26134 2023-07-12 12:31:32.000000 capeditor-0.2.5/capeditor/locale/en/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:31:49.676219 capeditor-0.2.5/capeditor/locale/es/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:31:49.680219 capeditor-0.2.5/capeditor/locale/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    17296 2023-07-12 12:31:32.000000 capeditor-0.2.5/capeditor/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    27356 2023-07-12 12:31:32.000000 capeditor-0.2.5/capeditor/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:31:49.676219 capeditor-0.2.5/capeditor/locale/fr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:31:49.680219 capeditor-0.2.5/capeditor/locale/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    17262 2023-07-12 12:31:32.000000 capeditor-0.2.5/capeditor/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    27296 2023-07-12 12:31:32.000000 capeditor-0.2.5/capeditor/locale/fr/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:31:49.676219 capeditor-0.2.5/capeditor/locale/sw/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:31:49.684218 capeditor-0.2.5/capeditor/locale/sw/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    16625 2023-07-12 12:31:32.000000 capeditor-0.2.5/capeditor/locale/sw/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    26453 2023-07-12 12:31:32.000000 capeditor-0.2.5/capeditor/locale/sw/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:31:49.684218 capeditor-0.2.5/capeditor/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-07-12 12:31:32.000000 capeditor-0.2.5/capeditor/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 12:31:32.000000 capeditor-0.2.5/capeditor/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14556 2023-07-12 12:31:32.000000 capeditor-0.2.5/capeditor/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-07-12 12:31:32.000000 capeditor-0.2.5/capeditor/renderers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4608 2023-07-12 12:31:32.000000 capeditor-0.2.5/capeditor/serializers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:31:49.676219 capeditor-0.2.5/capeditor/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:31:49.676219 capeditor-0.2.5/capeditor/static/capeditor/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:31:49.684218 capeditor-0.2.5/capeditor/static/capeditor/css/
--rw-r--r--   0 runner    (1001) docker     (123)     3269 2023-07-12 12:31:32.000000 capeditor-0.2.5/capeditor/static/capeditor/css/cap_detail_page.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:31:49.684218 capeditor-0.2.5/capeditor/static/capeditor/css/widget/
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-12 12:31:32.000000 capeditor-0.2.5/capeditor/static/capeditor/css/widget/boundary-widget.css
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-07-12 12:31:32.000000 capeditor-0.2.5/capeditor/static/capeditor/css/widget/circle-widget.css
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-07-12 12:31:32.000000 capeditor-0.2.5/capeditor/static/capeditor/css/widget/polygon-widget.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:31:49.684218 capeditor-0.2.5/capeditor/static/capeditor/js/
--rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-07-12 12:31:32.000000 capeditor-0.2.5/capeditor/static/capeditor/js/cap_accordion.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:31:49.684218 capeditor-0.2.5/capeditor/static/capeditor/js/widget/
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-07-12 12:31:32.000000 capeditor-0.2.5/capeditor/static/capeditor/js/widget/boundary-polygon-widget-telepath.js
--rw-r--r--   0 runner    (1001) docker     (123)     8434 2023-07-12 12:31:32.000000 capeditor-0.2.5/capeditor/static/capeditor/js/widget/boundary-polygon-widget.js
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-07-12 12:31:32.000000 capeditor-0.2.5/capeditor/static/capeditor/js/widget/circle-widget-telepath.js
--rw-r--r--   0 runner    (1001) docker     (123)     8278 2023-07-12 12:31:32.000000 capeditor-0.2.5/capeditor/static/capeditor/js/widget/circle-widget.js
--rw-r--r--   0 runner    (1001) docker     (123)     2912 2023-07-12 12:31:32.000000 capeditor-0.2.5/capeditor/static/capeditor/js/widget/conditional_fields.js
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-07-12 12:31:32.000000 capeditor-0.2.5/capeditor/static/capeditor/js/widget/polygon-widget-telepath.js
--rw-r--r--   0 runner    (1001) docker     (123)    10704 2023-07-12 12:31:32.000000 capeditor-0.2.5/capeditor/static/capeditor/js/widget/polygon-widget.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:31:49.676219 capeditor-0.2.5/capeditor/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:31:49.684218 capeditor-0.2.5/capeditor/templates/capeditor/
--rw-r--r--   0 runner    (1001) docker     (123)    15623 2023-07-12 12:31:32.000000 capeditor-0.2.5/capeditor/templates/capeditor/cap_alert_page.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:31:49.684218 capeditor-0.2.5/capeditor/templates/capeditor/icons/
--rw-r--r--   0 runner    (1001) docker     (123)     4092 2023-07-12 12:31:32.000000 capeditor-0.2.5/capeditor/templates/capeditor/icons/cap-alert-full.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-07-12 12:31:32.000000 capeditor-0.2.5/capeditor/templates/capeditor/icons/cap-alert.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:31:49.684218 capeditor-0.2.5/capeditor/templates/capeditor/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-07-12 12:31:32.000000 capeditor-0.2.5/capeditor/templates/capeditor/widgets/boundary_polygon_widget.html
--rw-r--r--   0 runner    (1001) docker     (123)     2659 2023-07-12 12:31:32.000000 capeditor-0.2.5/capeditor/templates/capeditor/widgets/circle_widget.html
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-07-12 12:31:32.000000 capeditor-0.2.5/capeditor/templates/capeditor/widgets/polygon_widget.html
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-12 12:31:32.000000 capeditor-0.2.5/capeditor/tests.py
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-12 12:31:32.000000 capeditor-0.2.5/capeditor/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-07-12 12:31:32.000000 capeditor-0.2.5/capeditor/wagtail_hooks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:31:49.680219 capeditor-0.2.5/capeditor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8191 2023-07-12 12:31:49.000000 capeditor-0.2.5/capeditor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-07-12 12:31:49.000000 capeditor-0.2.5/capeditor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 12:31:49.000000 capeditor-0.2.5/capeditor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-12 12:31:49.000000 capeditor-0.2.5/capeditor.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-12 12:31:49.000000 capeditor-0.2.5/capeditor.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-12 12:31:32.000000 capeditor-0.2.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-07-12 12:31:49.684218 capeditor-0.2.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:55:05.859484 capeditor-0.2.6/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-12 21:54:48.000000 capeditor-0.2.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8191 2023-07-12 21:55:05.859484 capeditor-0.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7323 2023-07-12 21:54:48.000000 capeditor-0.2.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:55:05.855484 capeditor-0.2.6/capeditor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 21:54:48.000000 capeditor-0.2.6/capeditor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-12 21:54:48.000000 capeditor-0.2.6/capeditor/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-07-12 21:54:48.000000 capeditor-0.2.6/capeditor/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23891 2023-07-12 21:54:48.000000 capeditor-0.2.6/capeditor/blocks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:55:05.855484 capeditor-0.2.6/capeditor/forms/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 21:54:48.000000 capeditor-0.2.6/capeditor/forms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-07-12 21:54:48.000000 capeditor-0.2.6/capeditor/forms/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5673 2023-07-12 21:54:48.000000 capeditor-0.2.6/capeditor/forms/widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:55:05.851483 capeditor-0.2.6/capeditor/locale/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:55:05.851483 capeditor-0.2.6/capeditor/locale/am/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:55:05.855484 capeditor-0.2.6/capeditor/locale/am/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    20372 2023-07-12 21:54:48.000000 capeditor-0.2.6/capeditor/locale/am/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    30677 2023-07-12 21:54:48.000000 capeditor-0.2.6/capeditor/locale/am/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:55:05.851483 capeditor-0.2.6/capeditor/locale/ar/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:55:05.855484 capeditor-0.2.6/capeditor/locale/ar/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    19629 2023-07-12 21:54:48.000000 capeditor-0.2.6/capeditor/locale/ar/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    30023 2023-07-12 21:54:48.000000 capeditor-0.2.6/capeditor/locale/ar/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:55:05.851483 capeditor-0.2.6/capeditor/locale/en/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:55:05.855484 capeditor-0.2.6/capeditor/locale/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16403 2023-07-12 21:54:48.000000 capeditor-0.2.6/capeditor/locale/en/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    26134 2023-07-12 21:54:48.000000 capeditor-0.2.6/capeditor/locale/en/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:55:05.851483 capeditor-0.2.6/capeditor/locale/es/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:55:05.855484 capeditor-0.2.6/capeditor/locale/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    17296 2023-07-12 21:54:48.000000 capeditor-0.2.6/capeditor/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    27356 2023-07-12 21:54:48.000000 capeditor-0.2.6/capeditor/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:55:05.851483 capeditor-0.2.6/capeditor/locale/fr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:55:05.859484 capeditor-0.2.6/capeditor/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    17262 2023-07-12 21:54:48.000000 capeditor-0.2.6/capeditor/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    27296 2023-07-12 21:54:48.000000 capeditor-0.2.6/capeditor/locale/fr/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:55:05.851483 capeditor-0.2.6/capeditor/locale/sw/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:55:05.859484 capeditor-0.2.6/capeditor/locale/sw/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16625 2023-07-12 21:54:48.000000 capeditor-0.2.6/capeditor/locale/sw/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    26453 2023-07-12 21:54:48.000000 capeditor-0.2.6/capeditor/locale/sw/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:55:05.859484 capeditor-0.2.6/capeditor/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-07-12 21:54:48.000000 capeditor-0.2.6/capeditor/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 21:54:48.000000 capeditor-0.2.6/capeditor/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14556 2023-07-12 21:54:48.000000 capeditor-0.2.6/capeditor/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-07-12 21:54:48.000000 capeditor-0.2.6/capeditor/renderers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4608 2023-07-12 21:54:48.000000 capeditor-0.2.6/capeditor/serializers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:55:05.851483 capeditor-0.2.6/capeditor/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:55:05.851483 capeditor-0.2.6/capeditor/static/capeditor/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:55:05.859484 capeditor-0.2.6/capeditor/static/capeditor/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     3269 2023-07-12 21:54:48.000000 capeditor-0.2.6/capeditor/static/capeditor/css/cap_detail_page.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:55:05.859484 capeditor-0.2.6/capeditor/static/capeditor/css/widget/
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-12 21:54:48.000000 capeditor-0.2.6/capeditor/static/capeditor/css/widget/boundary-widget.css
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-07-12 21:54:48.000000 capeditor-0.2.6/capeditor/static/capeditor/css/widget/circle-widget.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-07-12 21:54:48.000000 capeditor-0.2.6/capeditor/static/capeditor/css/widget/polygon-widget.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:55:05.859484 capeditor-0.2.6/capeditor/static/capeditor/js/
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-07-12 21:54:48.000000 capeditor-0.2.6/capeditor/static/capeditor/js/cap_accordion.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:55:05.859484 capeditor-0.2.6/capeditor/static/capeditor/js/widget/
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-07-12 21:54:48.000000 capeditor-0.2.6/capeditor/static/capeditor/js/widget/boundary-polygon-widget-telepath.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8434 2023-07-12 21:54:48.000000 capeditor-0.2.6/capeditor/static/capeditor/js/widget/boundary-polygon-widget.js
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-07-12 21:54:48.000000 capeditor-0.2.6/capeditor/static/capeditor/js/widget/circle-widget-telepath.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8278 2023-07-12 21:54:48.000000 capeditor-0.2.6/capeditor/static/capeditor/js/widget/circle-widget.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2912 2023-07-12 21:54:48.000000 capeditor-0.2.6/capeditor/static/capeditor/js/widget/conditional_fields.js
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-07-12 21:54:48.000000 capeditor-0.2.6/capeditor/static/capeditor/js/widget/polygon-widget-telepath.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10704 2023-07-12 21:54:48.000000 capeditor-0.2.6/capeditor/static/capeditor/js/widget/polygon-widget.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:55:05.851483 capeditor-0.2.6/capeditor/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:55:05.859484 capeditor-0.2.6/capeditor/templates/capeditor/
+-rw-r--r--   0 runner    (1001) docker     (123)    15623 2023-07-12 21:54:48.000000 capeditor-0.2.6/capeditor/templates/capeditor/cap_alert_page.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:55:05.859484 capeditor-0.2.6/capeditor/templates/capeditor/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)     4092 2023-07-12 21:54:48.000000 capeditor-0.2.6/capeditor/templates/capeditor/icons/cap-alert-full.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-07-12 21:54:48.000000 capeditor-0.2.6/capeditor/templates/capeditor/icons/cap-alert.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:55:05.859484 capeditor-0.2.6/capeditor/templates/capeditor/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-07-12 21:54:48.000000 capeditor-0.2.6/capeditor/templates/capeditor/widgets/boundary_polygon_widget.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2659 2023-07-12 21:54:48.000000 capeditor-0.2.6/capeditor/templates/capeditor/widgets/circle_widget.html
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-07-12 21:54:48.000000 capeditor-0.2.6/capeditor/templates/capeditor/widgets/polygon_widget.html
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-12 21:54:48.000000 capeditor-0.2.6/capeditor/tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-12 21:54:48.000000 capeditor-0.2.6/capeditor/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-07-12 21:54:48.000000 capeditor-0.2.6/capeditor/wagtail_hooks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:55:05.855484 capeditor-0.2.6/capeditor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8191 2023-07-12 21:55:05.000000 capeditor-0.2.6/capeditor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-07-12 21:55:05.000000 capeditor-0.2.6/capeditor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 21:55:05.000000 capeditor-0.2.6/capeditor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-12 21:55:05.000000 capeditor-0.2.6/capeditor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-12 21:55:05.000000 capeditor-0.2.6/capeditor.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-12 21:54:48.000000 capeditor-0.2.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-07-12 21:55:05.859484 capeditor-0.2.6/setup.cfg
```

### Comparing `capeditor-0.2.5/PKG-INFO` & `capeditor-0.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: capeditor
-Version: 0.2.5
+Version: 0.2.6
 Summary: Wagtail based CAP Editor
 Home-page: https://github.com/wmo-raf/cap-editor
 Author: Grace Amondi, Erick Otenyo
 Author-email: miswa.grace@gmail.com, otenyo.erick@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
```

### Comparing `capeditor-0.2.5/README.md` & `capeditor-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `capeditor-0.2.5/capeditor/blocks.py` & `capeditor-0.2.6/capeditor/blocks.py`

 * *Files 1% similar despite different names*

```diff
@@ -427,19 +427,21 @@
             return features
 
     @cached_property
     def area_properties(self):
         severity_blocks = self.get("severity")
         certainty_blocks = self.get("certainty")
         urgency_blocks = self.get("urgency")
+        event_blocks = self.get("event")
 
         return {
             'severity':severity_blocks,
             'certainty':certainty_blocks,
-            'urgency':urgency_blocks
+            'urgency':urgency_blocks,
+            'event':event_blocks
         }
 
     @cached_property
     def features(self):
         area_blocks = self.get("area")
         
         features = []
```

### Comparing `capeditor-0.2.5/capeditor/forms/widgets.py` & `capeditor-0.2.6/capeditor/forms/widgets.py`

 * *Files identical despite different names*

### Comparing `capeditor-0.2.5/capeditor/locale/am/LC_MESSAGES/django.mo` & `capeditor-0.2.6/capeditor/locale/am/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `capeditor-0.2.5/capeditor/locale/am/LC_MESSAGES/django.po` & `capeditor-0.2.6/capeditor/locale/am/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `capeditor-0.2.5/capeditor/locale/ar/LC_MESSAGES/django.mo` & `capeditor-0.2.6/capeditor/locale/ar/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `capeditor-0.2.5/capeditor/locale/ar/LC_MESSAGES/django.po` & `capeditor-0.2.6/capeditor/locale/ar/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `capeditor-0.2.5/capeditor/locale/en/LC_MESSAGES/django.mo` & `capeditor-0.2.6/capeditor/locale/en/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `capeditor-0.2.5/capeditor/locale/en/LC_MESSAGES/django.po` & `capeditor-0.2.6/capeditor/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `capeditor-0.2.5/capeditor/locale/es/LC_MESSAGES/django.mo` & `capeditor-0.2.6/capeditor/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `capeditor-0.2.5/capeditor/locale/es/LC_MESSAGES/django.po` & `capeditor-0.2.6/capeditor/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `capeditor-0.2.5/capeditor/locale/fr/LC_MESSAGES/django.mo` & `capeditor-0.2.6/capeditor/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `capeditor-0.2.5/capeditor/locale/fr/LC_MESSAGES/django.po` & `capeditor-0.2.6/capeditor/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `capeditor-0.2.5/capeditor/locale/sw/LC_MESSAGES/django.mo` & `capeditor-0.2.6/capeditor/locale/sw/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `capeditor-0.2.5/capeditor/locale/sw/LC_MESSAGES/django.po` & `capeditor-0.2.6/capeditor/locale/sw/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `capeditor-0.2.5/capeditor/migrations/0001_initial.py` & `capeditor-0.2.6/capeditor/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `capeditor-0.2.5/capeditor/models.py` & `capeditor-0.2.6/capeditor/models.py`

 * *Files identical despite different names*

### Comparing `capeditor-0.2.5/capeditor/renderers.py` & `capeditor-0.2.6/capeditor/renderers.py`

 * *Files identical despite different names*

### Comparing `capeditor-0.2.5/capeditor/serializers.py` & `capeditor-0.2.6/capeditor/serializers.py`

 * *Files identical despite different names*

### Comparing `capeditor-0.2.5/capeditor/static/capeditor/css/cap_detail_page.css` & `capeditor-0.2.6/capeditor/static/capeditor/css/cap_detail_page.css`

 * *Files identical despite different names*

### Comparing `capeditor-0.2.5/capeditor/static/capeditor/css/widget/circle-widget.css` & `capeditor-0.2.6/capeditor/static/capeditor/css/widget/circle-widget.css`

 * *Files identical despite different names*

### Comparing `capeditor-0.2.5/capeditor/static/capeditor/css/widget/polygon-widget.css` & `capeditor-0.2.6/capeditor/static/capeditor/css/widget/polygon-widget.css`

 * *Files identical despite different names*

### Comparing `capeditor-0.2.5/capeditor/static/capeditor/js/cap_accordion.js` & `capeditor-0.2.6/capeditor/static/capeditor/js/cap_accordion.js`

 * *Files identical despite different names*

### Comparing `capeditor-0.2.5/capeditor/static/capeditor/js/widget/boundary-polygon-widget-telepath.js` & `capeditor-0.2.6/capeditor/static/capeditor/js/widget/boundary-polygon-widget-telepath.js`

 * *Files identical despite different names*

### Comparing `capeditor-0.2.5/capeditor/static/capeditor/js/widget/boundary-polygon-widget.js` & `capeditor-0.2.6/capeditor/static/capeditor/js/widget/boundary-polygon-widget.js`

 * *Files identical despite different names*

### Comparing `capeditor-0.2.5/capeditor/static/capeditor/js/widget/circle-widget-telepath.js` & `capeditor-0.2.6/capeditor/static/capeditor/js/widget/circle-widget-telepath.js`

 * *Files identical despite different names*

### Comparing `capeditor-0.2.5/capeditor/static/capeditor/js/widget/circle-widget.js` & `capeditor-0.2.6/capeditor/static/capeditor/js/widget/circle-widget.js`

 * *Files identical despite different names*

### Comparing `capeditor-0.2.5/capeditor/static/capeditor/js/widget/conditional_fields.js` & `capeditor-0.2.6/capeditor/static/capeditor/js/widget/conditional_fields.js`

 * *Files identical despite different names*

### Comparing `capeditor-0.2.5/capeditor/static/capeditor/js/widget/polygon-widget-telepath.js` & `capeditor-0.2.6/capeditor/static/capeditor/js/widget/polygon-widget-telepath.js`

 * *Files identical despite different names*

### Comparing `capeditor-0.2.5/capeditor/static/capeditor/js/widget/polygon-widget.js` & `capeditor-0.2.6/capeditor/static/capeditor/js/widget/polygon-widget.js`

 * *Files identical despite different names*

### Comparing `capeditor-0.2.5/capeditor/templates/capeditor/cap_alert_page.html` & `capeditor-0.2.6/capeditor/templates/capeditor/cap_alert_page.html`

 * *Files identical despite different names*

### Comparing `capeditor-0.2.5/capeditor/templates/capeditor/icons/cap-alert-full.svg` & `capeditor-0.2.6/capeditor/templates/capeditor/icons/cap-alert-full.svg`

 * *Files identical despite different names*

### Comparing `capeditor-0.2.5/capeditor/templates/capeditor/icons/cap-alert.svg` & `capeditor-0.2.6/capeditor/templates/capeditor/icons/cap-alert.svg`

 * *Files identical despite different names*

### Comparing `capeditor-0.2.5/capeditor/templates/capeditor/widgets/circle_widget.html` & `capeditor-0.2.6/capeditor/templates/capeditor/widgets/circle_widget.html`

 * *Files identical despite different names*

### Comparing `capeditor-0.2.5/capeditor.egg-info/PKG-INFO` & `capeditor-0.2.6/capeditor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: capeditor
-Version: 0.2.5
+Version: 0.2.6
 Summary: Wagtail based CAP Editor
 Home-page: https://github.com/wmo-raf/cap-editor
 Author: Grace Amondi, Erick Otenyo
 Author-email: miswa.grace@gmail.com, otenyo.erick@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
```

### Comparing `capeditor-0.2.5/capeditor.egg-info/SOURCES.txt` & `capeditor-0.2.6/capeditor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `capeditor-0.2.5/setup.cfg` & `capeditor-0.2.6/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = capeditor
-version = 0.2.5
+version = 0.2.6
 description = Wagtail based CAP Editor
 long_description = file:README.md
 long_description_content_type = text/markdown
 url = https://github.com/wmo-raf/cap-editor
 author = Grace Amondi, Erick Otenyo
 author_email = miswa.grace@gmail.com, otenyo.erick@gmail.com
 license = MIT
```

