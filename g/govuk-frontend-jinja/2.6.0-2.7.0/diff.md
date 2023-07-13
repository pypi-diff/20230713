# Comparing `tmp/govuk-frontend-jinja-2.6.0.tar.gz` & `tmp/govuk-frontend-jinja-2.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "govuk-frontend-jinja-2.6.0.tar", last modified: Tue Apr 25 13:15:42 2023, max compression
+gzip compressed data, was "govuk-frontend-jinja-2.7.0.tar", last modified: Thu Jul 13 14:10:45 2023, max compression
```

## Comparing `govuk-frontend-jinja-2.6.0.tar` & `govuk-frontend-jinja-2.7.0.tar`

### file list

```diff
@@ -1,83 +1,85 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:15:42.621981 govuk-frontend-jinja-2.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-25 13:15:30.000000 govuk-frontend-jinja-2.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    10165 2023-04-25 13:15:42.621981 govuk-frontend-jinja-2.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9178 2023-04-25 13:15:30.000000 govuk-frontend-jinja-2.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:15:42.613981 govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 13:15:30.000000 govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:15:42.617981 govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:15:42.613981 govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/components/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:15:42.617981 govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/components/accordion/
--rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-04-25 13:15:30.000000 govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/components/accordion/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:15:42.617981 govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/components/back-link/
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-04-25 13:15:30.000000 govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/components/back-link/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:15:42.617981 govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/components/breadcrumbs/
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-04-25 13:15:30.000000 govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/components/breadcrumbs/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:15:42.617981 govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/components/button/
--rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-04-25 13:15:30.000000 govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/components/button/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:15:42.617981 govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/components/character-count/
--rw-r--r--   0 runner    (1001) docker     (123)     3461 2023-04-25 13:15:30.000000 govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/components/character-count/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:15:42.617981 govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/components/checkboxes/
--rw-r--r--   0 runner    (1001) docker     (123)     5980 2023-04-25 13:15:30.000000 govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/components/checkboxes/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:15:42.617981 govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/components/cookie-banner/
--rw-r--r--   0 runner    (1001) docker     (123)     3031 2023-04-25 13:15:30.000000 govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/components/cookie-banner/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:15:42.617981 govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/components/date-input/
--rw-r--r--   0 runner    (1001) docker     (123)     3940 2023-04-25 13:15:30.000000 govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/components/date-input/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:15:42.617981 govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/components/details/
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-25 13:15:30.000000 govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/components/details/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:15:42.617981 govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/components/error-message/
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-04-25 13:15:30.000000 govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/components/error-message/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:15:42.617981 govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/components/error-summary/
--rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-04-25 13:15:30.000000 govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/components/error-summary/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:15:42.617981 govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/components/fieldset/
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-04-25 13:15:30.000000 govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/components/fieldset/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:15:42.617981 govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/components/file-upload/
--rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-04-25 13:15:30.000000 govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/components/file-upload/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:15:42.617981 govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/components/footer/
--rw-r--r--   0 runner    (1001) docker     (123)     5088 2023-04-25 13:15:30.000000 govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/components/footer/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:15:42.617981 govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/components/header/
--rw-r--r--   0 runner    (1001) docker     (123)     6043 2023-04-25 13:15:30.000000 govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/components/header/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:15:42.617981 govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/components/hint/
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-04-25 13:15:30.000000 govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/components/hint/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:15:42.617981 govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/components/input/
--rw-r--r--   0 runner    (1001) docker     (123)     3804 2023-04-25 13:15:30.000000 govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/components/input/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:15:42.617981 govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/components/inset-text/
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-04-25 13:15:30.000000 govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/components/inset-text/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:15:42.617981 govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/components/label/
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-04-25 13:15:30.000000 govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/components/label/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:15:42.617981 govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/components/notification-banner/
--rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-04-25 13:15:30.000000 govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/components/notification-banner/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:15:42.617981 govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/components/pagination/
--rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-04-25 13:15:30.000000 govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/components/pagination/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:15:42.617981 govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/components/panel/
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-25 13:15:30.000000 govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/components/panel/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:15:42.617981 govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/components/phase-banner/
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-04-25 13:15:30.000000 govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/components/phase-banner/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:15:42.617981 govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/components/radios/
--rw-r--r--   0 runner    (1001) docker     (123)     5321 2023-04-25 13:15:30.000000 govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/components/radios/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:15:42.617981 govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/components/select/
--rw-r--r--   0 runner    (1001) docker     (123)     2892 2023-04-25 13:15:30.000000 govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/components/select/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:15:42.617981 govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/components/skip-link/
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-04-25 13:15:30.000000 govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/components/skip-link/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:15:42.621981 govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/components/summary-list/
--rw-r--r--   0 runner    (1001) docker     (123)     4426 2023-04-25 13:15:30.000000 govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/components/summary-list/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:15:42.621981 govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/components/table/
--rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-04-25 13:15:30.000000 govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/components/table/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:15:42.621981 govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/components/tabs/
--rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-04-25 13:15:30.000000 govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/components/tabs/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:15:42.621981 govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/components/tag/
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-04-25 13:15:30.000000 govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/components/tag/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:15:42.621981 govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/components/textarea/
--rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-04-25 13:15:30.000000 govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/components/textarea/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:15:42.621981 govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/components/warning-text/
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-04-25 13:15:30.000000 govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/components/warning-text/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:15:42.621981 govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/macros/
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-04-25 13:15:30.000000 govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/macros/i18n.html
--rw-r--r--   0 runner    (1001) docker     (123)     3298 2023-04-25 13:15:30.000000 govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/template.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:15:42.617981 govuk-frontend-jinja-2.6.0/govuk_frontend_jinja.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10165 2023-04-25 13:15:42.000000 govuk-frontend-jinja-2.6.0/govuk_frontend_jinja.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-04-25 13:15:42.000000 govuk-frontend-jinja-2.6.0/govuk_frontend_jinja.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 13:15:42.000000 govuk-frontend-jinja-2.6.0/govuk_frontend_jinja.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-25 13:15:42.000000 govuk-frontend-jinja-2.6.0/govuk_frontend_jinja.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-25 13:15:42.000000 govuk-frontend-jinja-2.6.0/govuk_frontend_jinja.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-04-25 13:15:42.621981 govuk-frontend-jinja-2.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-04-25 13:15:30.000000 govuk-frontend-jinja-2.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:10:45.811173 govuk-frontend-jinja-2.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-13 14:10:26.000000 govuk-frontend-jinja-2.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    10274 2023-07-13 14:10:45.811173 govuk-frontend-jinja-2.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9337 2023-07-13 14:10:26.000000 govuk-frontend-jinja-2.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:10:45.803173 govuk-frontend-jinja-2.7.0/govuk_frontend_jinja/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 14:10:26.000000 govuk-frontend-jinja-2.7.0/govuk_frontend_jinja/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:10:45.803173 govuk-frontend-jinja-2.7.0/govuk_frontend_jinja/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:10:45.803173 govuk-frontend-jinja-2.7.0/govuk_frontend_jinja/templates/components/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:10:45.803173 govuk-frontend-jinja-2.7.0/govuk_frontend_jinja/templates/components/accordion/
+-rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-07-13 14:10:26.000000 govuk-frontend-jinja-2.7.0/govuk_frontend_jinja/templates/components/accordion/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:10:45.803173 govuk-frontend-jinja-2.7.0/govuk_frontend_jinja/templates/components/back-link/
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-07-13 14:10:26.000000 govuk-frontend-jinja-2.7.0/govuk_frontend_jinja/templates/components/back-link/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:10:45.807173 govuk-frontend-jinja-2.7.0/govuk_frontend_jinja/templates/components/breadcrumbs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-07-13 14:10:26.000000 govuk-frontend-jinja-2.7.0/govuk_frontend_jinja/templates/components/breadcrumbs/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:10:45.807173 govuk-frontend-jinja-2.7.0/govuk_frontend_jinja/templates/components/button/
+-rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-07-13 14:10:26.000000 govuk-frontend-jinja-2.7.0/govuk_frontend_jinja/templates/components/button/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:10:45.807173 govuk-frontend-jinja-2.7.0/govuk_frontend_jinja/templates/components/character-count/
+-rw-r--r--   0 runner    (1001) docker     (123)     3461 2023-07-13 14:10:26.000000 govuk-frontend-jinja-2.7.0/govuk_frontend_jinja/templates/components/character-count/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:10:45.807173 govuk-frontend-jinja-2.7.0/govuk_frontend_jinja/templates/components/checkboxes/
+-rw-r--r--   0 runner    (1001) docker     (123)     5980 2023-07-13 14:10:26.000000 govuk-frontend-jinja-2.7.0/govuk_frontend_jinja/templates/components/checkboxes/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:10:45.807173 govuk-frontend-jinja-2.7.0/govuk_frontend_jinja/templates/components/cookie-banner/
+-rw-r--r--   0 runner    (1001) docker     (123)     3031 2023-07-13 14:10:26.000000 govuk-frontend-jinja-2.7.0/govuk_frontend_jinja/templates/components/cookie-banner/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:10:45.807173 govuk-frontend-jinja-2.7.0/govuk_frontend_jinja/templates/components/date-input/
+-rw-r--r--   0 runner    (1001) docker     (123)     3940 2023-07-13 14:10:26.000000 govuk-frontend-jinja-2.7.0/govuk_frontend_jinja/templates/components/date-input/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:10:45.807173 govuk-frontend-jinja-2.7.0/govuk_frontend_jinja/templates/components/details/
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-07-13 14:10:26.000000 govuk-frontend-jinja-2.7.0/govuk_frontend_jinja/templates/components/details/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:10:45.807173 govuk-frontend-jinja-2.7.0/govuk_frontend_jinja/templates/components/error-message/
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-07-13 14:10:26.000000 govuk-frontend-jinja-2.7.0/govuk_frontend_jinja/templates/components/error-message/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:10:45.807173 govuk-frontend-jinja-2.7.0/govuk_frontend_jinja/templates/components/error-summary/
+-rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-07-13 14:10:26.000000 govuk-frontend-jinja-2.7.0/govuk_frontend_jinja/templates/components/error-summary/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:10:45.807173 govuk-frontend-jinja-2.7.0/govuk_frontend_jinja/templates/components/exit-this-page/
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-07-13 14:10:26.000000 govuk-frontend-jinja-2.7.0/govuk_frontend_jinja/templates/components/exit-this-page/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:10:45.807173 govuk-frontend-jinja-2.7.0/govuk_frontend_jinja/templates/components/fieldset/
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-07-13 14:10:26.000000 govuk-frontend-jinja-2.7.0/govuk_frontend_jinja/templates/components/fieldset/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:10:45.807173 govuk-frontend-jinja-2.7.0/govuk_frontend_jinja/templates/components/file-upload/
+-rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-07-13 14:10:26.000000 govuk-frontend-jinja-2.7.0/govuk_frontend_jinja/templates/components/file-upload/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:10:45.807173 govuk-frontend-jinja-2.7.0/govuk_frontend_jinja/templates/components/footer/
+-rw-r--r--   0 runner    (1001) docker     (123)     5088 2023-07-13 14:10:26.000000 govuk-frontend-jinja-2.7.0/govuk_frontend_jinja/templates/components/footer/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:10:45.807173 govuk-frontend-jinja-2.7.0/govuk_frontend_jinja/templates/components/header/
+-rw-r--r--   0 runner    (1001) docker     (123)     6043 2023-07-13 14:10:26.000000 govuk-frontend-jinja-2.7.0/govuk_frontend_jinja/templates/components/header/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:10:45.807173 govuk-frontend-jinja-2.7.0/govuk_frontend_jinja/templates/components/hint/
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-07-13 14:10:26.000000 govuk-frontend-jinja-2.7.0/govuk_frontend_jinja/templates/components/hint/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:10:45.807173 govuk-frontend-jinja-2.7.0/govuk_frontend_jinja/templates/components/input/
+-rw-r--r--   0 runner    (1001) docker     (123)     3804 2023-07-13 14:10:26.000000 govuk-frontend-jinja-2.7.0/govuk_frontend_jinja/templates/components/input/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:10:45.807173 govuk-frontend-jinja-2.7.0/govuk_frontend_jinja/templates/components/inset-text/
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-07-13 14:10:26.000000 govuk-frontend-jinja-2.7.0/govuk_frontend_jinja/templates/components/inset-text/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:10:45.807173 govuk-frontend-jinja-2.7.0/govuk_frontend_jinja/templates/components/label/
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-13 14:10:26.000000 govuk-frontend-jinja-2.7.0/govuk_frontend_jinja/templates/components/label/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:10:45.811173 govuk-frontend-jinja-2.7.0/govuk_frontend_jinja/templates/components/notification-banner/
+-rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-07-13 14:10:26.000000 govuk-frontend-jinja-2.7.0/govuk_frontend_jinja/templates/components/notification-banner/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:10:45.811173 govuk-frontend-jinja-2.7.0/govuk_frontend_jinja/templates/components/pagination/
+-rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-07-13 14:10:26.000000 govuk-frontend-jinja-2.7.0/govuk_frontend_jinja/templates/components/pagination/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:10:45.811173 govuk-frontend-jinja-2.7.0/govuk_frontend_jinja/templates/components/panel/
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-07-13 14:10:26.000000 govuk-frontend-jinja-2.7.0/govuk_frontend_jinja/templates/components/panel/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:10:45.811173 govuk-frontend-jinja-2.7.0/govuk_frontend_jinja/templates/components/phase-banner/
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-07-13 14:10:26.000000 govuk-frontend-jinja-2.7.0/govuk_frontend_jinja/templates/components/phase-banner/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:10:45.811173 govuk-frontend-jinja-2.7.0/govuk_frontend_jinja/templates/components/radios/
+-rw-r--r--   0 runner    (1001) docker     (123)     5321 2023-07-13 14:10:26.000000 govuk-frontend-jinja-2.7.0/govuk_frontend_jinja/templates/components/radios/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:10:45.811173 govuk-frontend-jinja-2.7.0/govuk_frontend_jinja/templates/components/select/
+-rw-r--r--   0 runner    (1001) docker     (123)     2892 2023-07-13 14:10:26.000000 govuk-frontend-jinja-2.7.0/govuk_frontend_jinja/templates/components/select/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:10:45.811173 govuk-frontend-jinja-2.7.0/govuk_frontend_jinja/templates/components/skip-link/
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-13 14:10:26.000000 govuk-frontend-jinja-2.7.0/govuk_frontend_jinja/templates/components/skip-link/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:10:45.811173 govuk-frontend-jinja-2.7.0/govuk_frontend_jinja/templates/components/summary-list/
+-rw-r--r--   0 runner    (1001) docker     (123)     4426 2023-07-13 14:10:26.000000 govuk-frontend-jinja-2.7.0/govuk_frontend_jinja/templates/components/summary-list/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:10:45.811173 govuk-frontend-jinja-2.7.0/govuk_frontend_jinja/templates/components/table/
+-rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-07-13 14:10:26.000000 govuk-frontend-jinja-2.7.0/govuk_frontend_jinja/templates/components/table/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:10:45.811173 govuk-frontend-jinja-2.7.0/govuk_frontend_jinja/templates/components/tabs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-07-13 14:10:26.000000 govuk-frontend-jinja-2.7.0/govuk_frontend_jinja/templates/components/tabs/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:10:45.811173 govuk-frontend-jinja-2.7.0/govuk_frontend_jinja/templates/components/tag/
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-07-13 14:10:26.000000 govuk-frontend-jinja-2.7.0/govuk_frontend_jinja/templates/components/tag/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:10:45.811173 govuk-frontend-jinja-2.7.0/govuk_frontend_jinja/templates/components/textarea/
+-rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-07-13 14:10:26.000000 govuk-frontend-jinja-2.7.0/govuk_frontend_jinja/templates/components/textarea/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:10:45.811173 govuk-frontend-jinja-2.7.0/govuk_frontend_jinja/templates/components/warning-text/
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-07-13 14:10:26.000000 govuk-frontend-jinja-2.7.0/govuk_frontend_jinja/templates/components/warning-text/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:10:45.811173 govuk-frontend-jinja-2.7.0/govuk_frontend_jinja/templates/macros/
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-07-13 14:10:26.000000 govuk-frontend-jinja-2.7.0/govuk_frontend_jinja/templates/macros/i18n.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3298 2023-07-13 14:10:26.000000 govuk-frontend-jinja-2.7.0/govuk_frontend_jinja/templates/template.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:10:45.803173 govuk-frontend-jinja-2.7.0/govuk_frontend_jinja.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10274 2023-07-13 14:10:45.000000 govuk-frontend-jinja-2.7.0/govuk_frontend_jinja.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-07-13 14:10:45.000000 govuk-frontend-jinja-2.7.0/govuk_frontend_jinja.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 14:10:45.000000 govuk-frontend-jinja-2.7.0/govuk_frontend_jinja.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-13 14:10:45.000000 govuk-frontend-jinja-2.7.0/govuk_frontend_jinja.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-13 14:10:45.000000 govuk-frontend-jinja-2.7.0/govuk_frontend_jinja.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-13 14:10:45.811173 govuk-frontend-jinja-2.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-07-13 14:10:26.000000 govuk-frontend-jinja-2.7.0/setup.py
```

### Comparing `govuk-frontend-jinja-2.6.0/LICENSE` & `govuk-frontend-jinja-2.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `govuk-frontend-jinja-2.6.0/PKG-INFO` & `govuk-frontend-jinja-2.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,49 +1,49 @@
 Metadata-Version: 2.1
 Name: govuk-frontend-jinja
-Version: 2.6.0
+Version: 2.7.0
 Summary: GOV.UK Frontend Jinja Macros
 Home-page: https://github.com/LandRegistry/govuk-frontend-jinja
 Author: Matt Shaw
 Author-email: matthew.shaw@landregistry.gov.uk
 Classifier: Development Status :: 5 - Production/Stable
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Environment :: Web Environment
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Code Generators
 Classifier: Topic :: Software Development :: User Interfaces
 Classifier: Topic :: Text Processing :: Markup :: HTML
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # GOV.UK Frontend Jinja Macros
 
 [![PyPI version](https://badge.fury.io/py/govuk-frontend-jinja.svg)](https://pypi.org/project/govuk-frontend-jinja/)
-![govuk-frontend 4.6.0](https://img.shields.io/badge/govuk--frontend%20version-4.6.0-005EA5?logo=gov.uk&style=flat)
+![govuk-frontend 4.7.0](https://img.shields.io/badge/govuk--frontend%20version-4.7.0-005EA5?logo=gov.uk&style=flat)
 [![Python package](https://github.com/LandRegistry/govuk-frontend-jinja/actions/workflows/python-package.yml/badge.svg)](https://github.com/LandRegistry/govuk-frontend-jinja/actions/workflows/python-package.yml)
 
 **GOV.UK Frontend Jinja is a [community tool](https://design-system.service.gov.uk/community/resources-and-tools/) of the [GOV.UK Design System](https://design-system.service.gov.uk/). The Design System team is not responsible for it and cannot support you with using it. Contact the [maintainers](#contributors) directly if you need [help](#support) or you want to request a feature.**
 
 This repository provides a complete set of [Jinja](https://jinja.palletsprojects.com/) macros that are kept up-to-date and 100% compliant with the original [GOV.UK Frontend](https://github.com/alphagov/govuk-frontend) Nunjucks macros. Porting is intentionally manual rather than automated to make updates simpler than maintaining an automated conversion routine. A [comprehensive test suite](https://github.com/surevine/govuk-frontend-diff) ensures compliance against the latest, and every subsequent, GOV.UK Frontend release.
 
 If you are looking to build a fully featured Flask app that integrates with [GOV.UK Frontend Jinja](https://github.com/LandRegistry/govuk-frontend-jinja) and [GOV.UK Frontend WTForms](https://github.com/LandRegistry/govuk-frontend-wtf) please use the [GOV.UK Frontend Flask](https://github.com/LandRegistry/govuk-frontend-flask) template repository to [generate your app](https://github.com/LandRegistry/govuk-frontend-flask/generate).
 
 ## Compatibility
 
 The following table shows the version of GOV.UK Frontend Jinja that you should use for your targeted version of GOV.UK Frontend:
 
 | GOV.UK Frontend Jinja Version | Target GOV.UK Frontend Version |
 | ----------------------------- | ------------------------------ |
+| [2.7.0](https://github.com/LandRegistry/govuk-frontend-jinja/releases/tag/2.7.0) | [4.7.0](https://github.com/alphagov/govuk-frontend/releases/tag/v4.7.0) |
 | [2.6.0](https://github.com/LandRegistry/govuk-frontend-jinja/releases/tag/2.6.0) | [4.6.0](https://github.com/alphagov/govuk-frontend/releases/tag/v4.6.0) |
 | [2.5.0](https://github.com/LandRegistry/govuk-frontend-jinja/releases/tag/2.5.0) | [4.5.0](https://github.com/alphagov/govuk-frontend/releases/tag/v4.5.0) |
 | [2.4.0](https://github.com/LandRegistry/govuk-frontend-jinja/releases/tag/2.4.0) | [4.4.1](https://github.com/alphagov/govuk-frontend/releases/tag/v4.4.1) |
 | [2.3.0](https://github.com/LandRegistry/govuk-frontend-jinja/releases/tag/2.3.0) | [4.2.0](https://github.com/alphagov/govuk-frontend/releases/tag/v4.2.0) |
 | [2.2.0](https://github.com/LandRegistry/govuk-frontend-jinja/releases/tag/2.2.0) | [4.1.0](https://github.com/alphagov/govuk-frontend/releases/tag/v4.1.0) |
 | [2.1.0](https://github.com/LandRegistry/govuk-frontend-jinja/releases/tag/2.1.0) | [4.0.1](https://github.com/alphagov/govuk-frontend/releases/tag/v4.0.1) |
 | [2.0.0](https://github.com/LandRegistry/govuk-frontend-jinja/releases/tag/2.0.0) | [4.0.0](https://github.com/alphagov/govuk-frontend/releases/tag/v4.0.0) |
```

### Comparing `govuk-frontend-jinja-2.6.0/README.md` & `govuk-frontend-jinja-2.7.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 # GOV.UK Frontend Jinja Macros
 
 [![PyPI version](https://badge.fury.io/py/govuk-frontend-jinja.svg)](https://pypi.org/project/govuk-frontend-jinja/)
-![govuk-frontend 4.6.0](https://img.shields.io/badge/govuk--frontend%20version-4.6.0-005EA5?logo=gov.uk&style=flat)
+![govuk-frontend 4.7.0](https://img.shields.io/badge/govuk--frontend%20version-4.7.0-005EA5?logo=gov.uk&style=flat)
 [![Python package](https://github.com/LandRegistry/govuk-frontend-jinja/actions/workflows/python-package.yml/badge.svg)](https://github.com/LandRegistry/govuk-frontend-jinja/actions/workflows/python-package.yml)
 
 **GOV.UK Frontend Jinja is a [community tool](https://design-system.service.gov.uk/community/resources-and-tools/) of the [GOV.UK Design System](https://design-system.service.gov.uk/). The Design System team is not responsible for it and cannot support you with using it. Contact the [maintainers](#contributors) directly if you need [help](#support) or you want to request a feature.**
 
 This repository provides a complete set of [Jinja](https://jinja.palletsprojects.com/) macros that are kept up-to-date and 100% compliant with the original [GOV.UK Frontend](https://github.com/alphagov/govuk-frontend) Nunjucks macros. Porting is intentionally manual rather than automated to make updates simpler than maintaining an automated conversion routine. A [comprehensive test suite](https://github.com/surevine/govuk-frontend-diff) ensures compliance against the latest, and every subsequent, GOV.UK Frontend release.
 
 If you are looking to build a fully featured Flask app that integrates with [GOV.UK Frontend Jinja](https://github.com/LandRegistry/govuk-frontend-jinja) and [GOV.UK Frontend WTForms](https://github.com/LandRegistry/govuk-frontend-wtf) please use the [GOV.UK Frontend Flask](https://github.com/LandRegistry/govuk-frontend-flask) template repository to [generate your app](https://github.com/LandRegistry/govuk-frontend-flask/generate).
 
 ## Compatibility
 
 The following table shows the version of GOV.UK Frontend Jinja that you should use for your targeted version of GOV.UK Frontend:
 
 | GOV.UK Frontend Jinja Version | Target GOV.UK Frontend Version |
 | ----------------------------- | ------------------------------ |
+| [2.7.0](https://github.com/LandRegistry/govuk-frontend-jinja/releases/tag/2.7.0) | [4.7.0](https://github.com/alphagov/govuk-frontend/releases/tag/v4.7.0) |
 | [2.6.0](https://github.com/LandRegistry/govuk-frontend-jinja/releases/tag/2.6.0) | [4.6.0](https://github.com/alphagov/govuk-frontend/releases/tag/v4.6.0) |
 | [2.5.0](https://github.com/LandRegistry/govuk-frontend-jinja/releases/tag/2.5.0) | [4.5.0](https://github.com/alphagov/govuk-frontend/releases/tag/v4.5.0) |
 | [2.4.0](https://github.com/LandRegistry/govuk-frontend-jinja/releases/tag/2.4.0) | [4.4.1](https://github.com/alphagov/govuk-frontend/releases/tag/v4.4.1) |
 | [2.3.0](https://github.com/LandRegistry/govuk-frontend-jinja/releases/tag/2.3.0) | [4.2.0](https://github.com/alphagov/govuk-frontend/releases/tag/v4.2.0) |
 | [2.2.0](https://github.com/LandRegistry/govuk-frontend-jinja/releases/tag/2.2.0) | [4.1.0](https://github.com/alphagov/govuk-frontend/releases/tag/v4.1.0) |
 | [2.1.0](https://github.com/LandRegistry/govuk-frontend-jinja/releases/tag/2.1.0) | [4.0.1](https://github.com/alphagov/govuk-frontend/releases/tag/v4.0.1) |
 | [2.0.0](https://github.com/LandRegistry/govuk-frontend-jinja/releases/tag/2.0.0) | [4.0.0](https://github.com/alphagov/govuk-frontend/releases/tag/v4.0.0) |
```

### Comparing `govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/components/accordion/macro.html` & `govuk-frontend-jinja-2.7.0/govuk_frontend_jinja/templates/components/accordion/macro.html`

 * *Files identical despite different names*

### Comparing `govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/components/breadcrumbs/macro.html` & `govuk-frontend-jinja-2.7.0/govuk_frontend_jinja/templates/components/breadcrumbs/macro.html`

 * *Files identical despite different names*

### Comparing `govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/components/button/macro.html` & `govuk-frontend-jinja-2.7.0/govuk_frontend_jinja/templates/components/button/macro.html`

 * *Files identical despite different names*

### Comparing `govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/components/character-count/macro.html` & `govuk-frontend-jinja-2.7.0/govuk_frontend_jinja/templates/components/character-count/macro.html`

 * *Files identical despite different names*

### Comparing `govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/components/checkboxes/macro.html` & `govuk-frontend-jinja-2.7.0/govuk_frontend_jinja/templates/components/checkboxes/macro.html`

 * *Files identical despite different names*

### Comparing `govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/components/cookie-banner/macro.html` & `govuk-frontend-jinja-2.7.0/govuk_frontend_jinja/templates/components/cookie-banner/macro.html`

 * *Files identical despite different names*

### Comparing `govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/components/date-input/macro.html` & `govuk-frontend-jinja-2.7.0/govuk_frontend_jinja/templates/components/date-input/macro.html`

 * *Files identical despite different names*

### Comparing `govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/components/details/macro.html` & `govuk-frontend-jinja-2.7.0/govuk_frontend_jinja/templates/components/details/macro.html`

 * *Files identical despite different names*

### Comparing `govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/components/error-message/macro.html` & `govuk-frontend-jinja-2.7.0/govuk_frontend_jinja/templates/components/error-message/macro.html`

 * *Files identical despite different names*

### Comparing `govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/components/error-summary/macro.html` & `govuk-frontend-jinja-2.7.0/govuk_frontend_jinja/templates/components/error-summary/macro.html`

 * *Files identical despite different names*

### Comparing `govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/components/fieldset/macro.html` & `govuk-frontend-jinja-2.7.0/govuk_frontend_jinja/templates/components/fieldset/macro.html`

 * *Files identical despite different names*

### Comparing `govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/components/file-upload/macro.html` & `govuk-frontend-jinja-2.7.0/govuk_frontend_jinja/templates/components/file-upload/macro.html`

 * *Files identical despite different names*

### Comparing `govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/components/footer/macro.html` & `govuk-frontend-jinja-2.7.0/govuk_frontend_jinja/templates/components/footer/macro.html`

 * *Files identical despite different names*

### Comparing `govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/components/header/macro.html` & `govuk-frontend-jinja-2.7.0/govuk_frontend_jinja/templates/components/header/macro.html`

 * *Files identical despite different names*

### Comparing `govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/components/input/macro.html` & `govuk-frontend-jinja-2.7.0/govuk_frontend_jinja/templates/components/input/macro.html`

 * *Files identical despite different names*

### Comparing `govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/components/label/macro.html` & `govuk-frontend-jinja-2.7.0/govuk_frontend_jinja/templates/components/label/macro.html`

 * *Files identical despite different names*

### Comparing `govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/components/notification-banner/macro.html` & `govuk-frontend-jinja-2.7.0/govuk_frontend_jinja/templates/components/notification-banner/macro.html`

 * *Files identical despite different names*

### Comparing `govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/components/pagination/macro.html` & `govuk-frontend-jinja-2.7.0/govuk_frontend_jinja/templates/components/pagination/macro.html`

 * *Files identical despite different names*

### Comparing `govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/components/panel/macro.html` & `govuk-frontend-jinja-2.7.0/govuk_frontend_jinja/templates/components/panel/macro.html`

 * *Files identical despite different names*

### Comparing `govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/components/phase-banner/macro.html` & `govuk-frontend-jinja-2.7.0/govuk_frontend_jinja/templates/components/phase-banner/macro.html`

 * *Files identical despite different names*

### Comparing `govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/components/radios/macro.html` & `govuk-frontend-jinja-2.7.0/govuk_frontend_jinja/templates/components/radios/macro.html`

 * *Files identical despite different names*

### Comparing `govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/components/select/macro.html` & `govuk-frontend-jinja-2.7.0/govuk_frontend_jinja/templates/components/select/macro.html`

 * *Files identical despite different names*

### Comparing `govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/components/summary-list/macro.html` & `govuk-frontend-jinja-2.7.0/govuk_frontend_jinja/templates/components/summary-list/macro.html`

 * *Files identical despite different names*

### Comparing `govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/components/table/macro.html` & `govuk-frontend-jinja-2.7.0/govuk_frontend_jinja/templates/components/table/macro.html`

 * *Files identical despite different names*

### Comparing `govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/components/tabs/macro.html` & `govuk-frontend-jinja-2.7.0/govuk_frontend_jinja/templates/components/tabs/macro.html`

 * *Files identical despite different names*

### Comparing `govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/components/textarea/macro.html` & `govuk-frontend-jinja-2.7.0/govuk_frontend_jinja/templates/components/textarea/macro.html`

 * *Files identical despite different names*

### Comparing `govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/components/warning-text/macro.html` & `govuk-frontend-jinja-2.7.0/govuk_frontend_jinja/templates/components/warning-text/macro.html`

 * *Files identical despite different names*

### Comparing `govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/macros/i18n.html` & `govuk-frontend-jinja-2.7.0/govuk_frontend_jinja/templates/macros/i18n.html`

 * *Files identical despite different names*

### Comparing `govuk-frontend-jinja-2.6.0/govuk_frontend_jinja/templates/template.html` & `govuk-frontend-jinja-2.7.0/govuk_frontend_jinja/templates/template.html`

 * *Files identical despite different names*

### Comparing `govuk-frontend-jinja-2.6.0/govuk_frontend_jinja.egg-info/PKG-INFO` & `govuk-frontend-jinja-2.7.0/govuk_frontend_jinja.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,49 +1,49 @@
 Metadata-Version: 2.1
 Name: govuk-frontend-jinja
-Version: 2.6.0
+Version: 2.7.0
 Summary: GOV.UK Frontend Jinja Macros
 Home-page: https://github.com/LandRegistry/govuk-frontend-jinja
 Author: Matt Shaw
 Author-email: matthew.shaw@landregistry.gov.uk
 Classifier: Development Status :: 5 - Production/Stable
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Environment :: Web Environment
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Code Generators
 Classifier: Topic :: Software Development :: User Interfaces
 Classifier: Topic :: Text Processing :: Markup :: HTML
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # GOV.UK Frontend Jinja Macros
 
 [![PyPI version](https://badge.fury.io/py/govuk-frontend-jinja.svg)](https://pypi.org/project/govuk-frontend-jinja/)
-![govuk-frontend 4.6.0](https://img.shields.io/badge/govuk--frontend%20version-4.6.0-005EA5?logo=gov.uk&style=flat)
+![govuk-frontend 4.7.0](https://img.shields.io/badge/govuk--frontend%20version-4.7.0-005EA5?logo=gov.uk&style=flat)
 [![Python package](https://github.com/LandRegistry/govuk-frontend-jinja/actions/workflows/python-package.yml/badge.svg)](https://github.com/LandRegistry/govuk-frontend-jinja/actions/workflows/python-package.yml)
 
 **GOV.UK Frontend Jinja is a [community tool](https://design-system.service.gov.uk/community/resources-and-tools/) of the [GOV.UK Design System](https://design-system.service.gov.uk/). The Design System team is not responsible for it and cannot support you with using it. Contact the [maintainers](#contributors) directly if you need [help](#support) or you want to request a feature.**
 
 This repository provides a complete set of [Jinja](https://jinja.palletsprojects.com/) macros that are kept up-to-date and 100% compliant with the original [GOV.UK Frontend](https://github.com/alphagov/govuk-frontend) Nunjucks macros. Porting is intentionally manual rather than automated to make updates simpler than maintaining an automated conversion routine. A [comprehensive test suite](https://github.com/surevine/govuk-frontend-diff) ensures compliance against the latest, and every subsequent, GOV.UK Frontend release.
 
 If you are looking to build a fully featured Flask app that integrates with [GOV.UK Frontend Jinja](https://github.com/LandRegistry/govuk-frontend-jinja) and [GOV.UK Frontend WTForms](https://github.com/LandRegistry/govuk-frontend-wtf) please use the [GOV.UK Frontend Flask](https://github.com/LandRegistry/govuk-frontend-flask) template repository to [generate your app](https://github.com/LandRegistry/govuk-frontend-flask/generate).
 
 ## Compatibility
 
 The following table shows the version of GOV.UK Frontend Jinja that you should use for your targeted version of GOV.UK Frontend:
 
 | GOV.UK Frontend Jinja Version | Target GOV.UK Frontend Version |
 | ----------------------------- | ------------------------------ |
+| [2.7.0](https://github.com/LandRegistry/govuk-frontend-jinja/releases/tag/2.7.0) | [4.7.0](https://github.com/alphagov/govuk-frontend/releases/tag/v4.7.0) |
 | [2.6.0](https://github.com/LandRegistry/govuk-frontend-jinja/releases/tag/2.6.0) | [4.6.0](https://github.com/alphagov/govuk-frontend/releases/tag/v4.6.0) |
 | [2.5.0](https://github.com/LandRegistry/govuk-frontend-jinja/releases/tag/2.5.0) | [4.5.0](https://github.com/alphagov/govuk-frontend/releases/tag/v4.5.0) |
 | [2.4.0](https://github.com/LandRegistry/govuk-frontend-jinja/releases/tag/2.4.0) | [4.4.1](https://github.com/alphagov/govuk-frontend/releases/tag/v4.4.1) |
 | [2.3.0](https://github.com/LandRegistry/govuk-frontend-jinja/releases/tag/2.3.0) | [4.2.0](https://github.com/alphagov/govuk-frontend/releases/tag/v4.2.0) |
 | [2.2.0](https://github.com/LandRegistry/govuk-frontend-jinja/releases/tag/2.2.0) | [4.1.0](https://github.com/alphagov/govuk-frontend/releases/tag/v4.1.0) |
 | [2.1.0](https://github.com/LandRegistry/govuk-frontend-jinja/releases/tag/2.1.0) | [4.0.1](https://github.com/alphagov/govuk-frontend/releases/tag/v4.0.1) |
 | [2.0.0](https://github.com/LandRegistry/govuk-frontend-jinja/releases/tag/2.0.0) | [4.0.0](https://github.com/alphagov/govuk-frontend/releases/tag/v4.0.0) |
```

### Comparing `govuk-frontend-jinja-2.6.0/govuk_frontend_jinja.egg-info/SOURCES.txt` & `govuk-frontend-jinja-2.7.0/govuk_frontend_jinja.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 govuk_frontend_jinja/templates/components/character-count/macro.html
 govuk_frontend_jinja/templates/components/checkboxes/macro.html
 govuk_frontend_jinja/templates/components/cookie-banner/macro.html
 govuk_frontend_jinja/templates/components/date-input/macro.html
 govuk_frontend_jinja/templates/components/details/macro.html
 govuk_frontend_jinja/templates/components/error-message/macro.html
 govuk_frontend_jinja/templates/components/error-summary/macro.html
+govuk_frontend_jinja/templates/components/exit-this-page/macro.html
 govuk_frontend_jinja/templates/components/fieldset/macro.html
 govuk_frontend_jinja/templates/components/file-upload/macro.html
 govuk_frontend_jinja/templates/components/footer/macro.html
 govuk_frontend_jinja/templates/components/header/macro.html
 govuk_frontend_jinja/templates/components/hint/macro.html
 govuk_frontend_jinja/templates/components/input/macro.html
 govuk_frontend_jinja/templates/components/inset-text/macro.html
```

### Comparing `govuk-frontend-jinja-2.6.0/setup.py` & `govuk-frontend-jinja-2.7.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,34 +9,33 @@
 components = []
 directories = glob.glob("govuk_frontend_jinja/**/**/*.html", recursive=True)
 for directory in directories:
     components.append(os.path.relpath(os.path.dirname(directory), "govuk_frontend_jinja") + "/*.html")
 
 setuptools.setup(
     name="govuk-frontend-jinja",
-    version="2.6.0",
+    version="2.7.0",
     author="Matt Shaw",
     author_email="matthew.shaw@landregistry.gov.uk",
     description="GOV.UK Frontend Jinja Macros",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/LandRegistry/govuk-frontend-jinja",
     packages=setuptools.find_packages(exclude=["tests"]),
     package_data={"govuk_frontend_jinja": components},
     classifiers=[
         "Development Status :: 5 - Production/Stable",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "License :: OSI Approved :: MIT License",
         "Environment :: Web Environment",
         "Operating System :: OS Independent",
         "Intended Audience :: Developers",
         "Topic :: Software Development :: Code Generators",
         "Topic :: Software Development :: User Interfaces",
         "Topic :: Text Processing :: Markup :: HTML",
     ],
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     install_requires=["jinja2!=3.0.0,!=3.0.1"],
 )
```

