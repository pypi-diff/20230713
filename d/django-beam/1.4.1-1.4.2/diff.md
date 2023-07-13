# Comparing `tmp/django-beam-1.4.1.tar.gz` & `tmp/django-beam-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-beam-1.4.1.tar", last modified: Tue May 23 09:27:00 2023, max compression
+gzip compressed data, was "django-beam-1.4.2.tar", last modified: Thu Jul 13 12:43:43 2023, max compression
```

## Comparing `django-beam-1.4.1.tar` & `django-beam-1.4.2.tar`

### file list

```diff
@@ -1,122 +1,122 @@
-drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-05-23 09:27:00.422494 django-beam-1.4.1/
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     1511 2022-04-27 09:12:32.000000 django-beam-1.4.1/LICENSE
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)      284 2023-01-09 10:44:11.000000 django-beam-1.4.1/MANIFEST.in
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     3403 2023-05-23 09:27:00.422703 django-beam-1.4.1/PKG-INFO
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     2954 2023-03-28 08:37:32.000000 django-beam-1.4.1/README.md
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)      740 2023-05-23 09:27:00.423228 django-beam-1.4.1/setup.cfg
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)       53 2022-04-27 09:12:32.000000 django-beam-1.4.1/setup.py
-drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-05-23 09:27:00.391719 django-beam-1.4.1/src/
-drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-05-23 09:27:00.398187 django-beam-1.4.1/src/beam/
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)      105 2023-04-27 07:29:03.000000 django-beam-1.4.1/src/beam/__init__.py
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     4680 2023-04-27 07:29:03.000000 django-beam-1.4.1/src/beam/actions.py
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     7485 2023-04-27 07:29:03.000000 django-beam-1.4.1/src/beam/components.py
-drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-05-23 09:27:00.398499 django-beam-1.4.1/src/beam/contrib/
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)        0 2023-04-27 07:29:03.000000 django-beam-1.4.1/src/beam/contrib/__init__.py
-drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-05-23 09:27:00.399575 django-beam-1.4.1/src/beam/contrib/auth/
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)        0 2023-04-27 07:29:03.000000 django-beam-1.4.1/src/beam/contrib/auth/__init__.py
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)      196 2023-04-27 07:29:03.000000 django-beam-1.4.1/src/beam/contrib/auth/apps.py
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)      903 2023-04-27 07:29:03.000000 django-beam-1.4.1/src/beam/contrib/auth/forms.py
-drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-05-23 09:27:00.390044 django-beam-1.4.1/src/beam/contrib/auth/templates/
-drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-05-23 09:27:00.401625 django-beam-1.4.1/src/beam/contrib/auth/templates/registration/
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)      296 2023-04-27 07:29:03.000000 django-beam-1.4.1/src/beam/contrib/auth/templates/registration/logged_out.html
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     1136 2023-04-27 07:29:03.000000 django-beam-1.4.1/src/beam/contrib/auth/templates/registration/login.html
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)      261 2023-04-27 07:29:03.000000 django-beam-1.4.1/src/beam/contrib/auth/templates/registration/password_change_done.html
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)      837 2023-04-27 07:29:04.000000 django-beam-1.4.1/src/beam/contrib/auth/templates/registration/password_change_form.html
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)      364 2023-04-27 07:29:04.000000 django-beam-1.4.1/src/beam/contrib/auth/templates/registration/password_reset_complete.html
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)      980 2023-04-27 07:29:04.000000 django-beam-1.4.1/src/beam/contrib/auth/templates/registration/password_reset_confirm.html
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)      535 2023-04-27 07:29:04.000000 django-beam-1.4.1/src/beam/contrib/auth/templates/registration/password_reset_done.html
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)      616 2023-04-27 07:29:04.000000 django-beam-1.4.1/src/beam/contrib/auth/templates/registration/password_reset_email.html
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)      531 2023-04-27 07:29:04.000000 django-beam-1.4.1/src/beam/contrib/auth/templates/registration/password_reset_form.html
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)      230 2023-04-27 07:29:03.000000 django-beam-1.4.1/src/beam/contrib/auth/urls.py
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     3881 2023-04-27 07:29:03.000000 django-beam-1.4.1/src/beam/contrib/auth/views.py
-drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-05-23 09:27:00.401942 django-beam-1.4.1/src/beam/contrib/autocomplete_light/
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     2940 2023-04-27 07:29:04.000000 django-beam-1.4.1/src/beam/contrib/autocomplete_light/__init__.py
-drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-05-23 09:27:00.390290 django-beam-1.4.1/src/beam/contrib/autocomplete_light/static/
-drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-05-23 09:27:00.402176 django-beam-1.4.1/src/beam/contrib/autocomplete_light/static/autocomplete_light/
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     1011 2023-04-27 07:29:04.000000 django-beam-1.4.1/src/beam/contrib/autocomplete_light/static/autocomplete_light/select2.css
-drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-05-23 09:27:00.403026 django-beam-1.4.1/src/beam/contrib/reversion/
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)        0 2023-04-27 07:29:04.000000 django-beam-1.4.1/src/beam/contrib/reversion/__init__.py
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)      150 2023-04-27 07:29:04.000000 django-beam-1.4.1/src/beam/contrib/reversion/apps.py
-drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-05-23 09:27:00.390539 django-beam-1.4.1/src/beam/contrib/reversion/templates/
-drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-05-23 09:27:00.403577 django-beam-1.4.1/src/beam/contrib/reversion/templates/beam_reversion/
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     1140 2023-04-27 07:29:04.000000 django-beam-1.4.1/src/beam/contrib/reversion/templates/beam_reversion/version_detail.html
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     1879 2023-04-27 07:29:04.000000 django-beam-1.4.1/src/beam/contrib/reversion/templates/beam_reversion/version_list.html
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     4032 2023-04-27 07:29:04.000000 django-beam-1.4.1/src/beam/contrib/reversion/views.py
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     7137 2023-04-27 07:29:04.000000 django-beam-1.4.1/src/beam/contrib/reversion/viewsets.py
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)    11062 2023-04-27 07:29:03.000000 django-beam-1.4.1/src/beam/inlines.py
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     1235 2023-04-27 07:29:03.000000 django-beam-1.4.1/src/beam/layouts.py
-drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-05-23 09:27:00.390707 django-beam-1.4.1/src/beam/locale/
-drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-05-23 09:27:00.390776 django-beam-1.4.1/src/beam/locale/de/
-drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-05-23 09:27:00.403798 django-beam-1.4.1/src/beam/locale/de/LC_MESSAGES/
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     5525 2023-04-27 07:29:04.000000 django-beam-1.4.1/src/beam/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     2814 2023-04-27 07:29:03.000000 django-beam-1.4.1/src/beam/registry.py
-drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-05-23 09:27:00.404177 django-beam-1.4.1/src/beam/templatetags/
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)        0 2023-04-27 07:29:04.000000 django-beam-1.4.1/src/beam/templatetags/__init__.py
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     8705 2023-05-17 08:50:04.000000 django-beam-1.4.1/src/beam/templatetags/beam_tags.py
-drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-05-23 09:27:00.404509 django-beam-1.4.1/src/beam/themes/
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)        0 2023-04-27 07:29:04.000000 django-beam-1.4.1/src/beam/themes/__init__.py
-drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-05-23 09:27:00.404786 django-beam-1.4.1/src/beam/themes/bootstrap4/
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)        0 2023-04-27 07:29:04.000000 django-beam-1.4.1/src/beam/themes/bootstrap4/__init__.py
-drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-05-23 09:27:00.391203 django-beam-1.4.1/src/beam/themes/bootstrap4/static/
-drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-05-23 09:27:00.391360 django-beam-1.4.1/src/beam/themes/bootstrap4/static/beam/
-drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-05-23 09:27:00.405012 django-beam-1.4.1/src/beam/themes/bootstrap4/static/beam/css/
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)    12660 2023-04-27 07:29:04.000000 django-beam-1.4.1/src/beam/themes/bootstrap4/static/beam/css/bootstrap-select.min.css
-drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-05-23 09:27:00.406572 django-beam-1.4.1/src/beam/themes/bootstrap4/static/beam/js/
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     3291 2023-04-27 07:29:04.000000 django-beam-1.4.1/src/beam/themes/bootstrap4/static/beam/js/actions.js
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     1328 2023-04-27 07:29:04.000000 django-beam-1.4.1/src/beam/themes/bootstrap4/static/beam/js/add_related.js
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)    94341 2023-04-27 07:29:04.000000 django-beam-1.4.1/src/beam/themes/bootstrap4/static/beam/js/bootstrap-select.min.js
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     6007 2023-04-27 07:29:04.000000 django-beam-1.4.1/src/beam/themes/bootstrap4/static/beam/js/inlines.js
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)    82676 2023-04-27 07:29:04.000000 django-beam-1.4.1/src/beam/themes/bootstrap4/static/beam/js/sortable.min.js
-drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-05-23 09:27:00.391516 django-beam-1.4.1/src/beam/themes/bootstrap4/templates/
-drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-05-23 09:27:00.409258 django-beam-1.4.1/src/beam/themes/bootstrap4/templates/beam/
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     3374 2023-05-17 08:50:04.000000 django-beam-1.4.1/src/beam/themes/bootstrap4/templates/beam/base.html
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)      261 2023-04-27 07:29:04.000000 django-beam-1.4.1/src/beam/themes/bootstrap4/templates/beam/create.html
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     1537 2023-05-23 09:24:24.000000 django-beam-1.4.1/src/beam/themes/bootstrap4/templates/beam/dashboard.html
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     2265 2023-05-23 09:24:24.000000 django-beam-1.4.1/src/beam/themes/bootstrap4/templates/beam/delete.html
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     2894 2023-04-27 07:29:04.000000 django-beam-1.4.1/src/beam/themes/bootstrap4/templates/beam/detail.html
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     4361 2023-05-23 09:24:24.000000 django-beam-1.4.1/src/beam/themes/bootstrap4/templates/beam/form.html
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     7895 2023-05-23 09:24:24.000000 django-beam-1.4.1/src/beam/themes/bootstrap4/templates/beam/list.html
-drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-05-23 09:27:00.414663 django-beam-1.4.1/src/beam/themes/bootstrap4/templates/beam/partials/
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     1750 2023-05-23 09:24:24.000000 django-beam-1.4.1/src/beam/themes/bootstrap4/templates/beam/partials/actions.html
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     2168 2023-05-23 09:24:24.000000 django-beam-1.4.1/src/beam/themes/bootstrap4/templates/beam/partials/detail_field.html
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     4596 2023-05-23 09:24:24.000000 django-beam-1.4.1/src/beam/themes/bootstrap4/templates/beam/partials/detail_inline.html
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     3298 2023-05-23 09:24:24.000000 django-beam-1.4.1/src/beam/themes/bootstrap4/templates/beam/partials/detail_inline_tabular.html
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     1289 2023-04-27 07:29:04.000000 django-beam-1.4.1/src/beam/themes/bootstrap4/templates/beam/partials/filters.html
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)      604 2023-05-23 09:24:24.000000 django-beam-1.4.1/src/beam/themes/bootstrap4/templates/beam/partials/form_field.html
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     6373 2023-05-23 09:24:24.000000 django-beam-1.4.1/src/beam/themes/bootstrap4/templates/beam/partials/form_inline.html
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     3075 2023-05-23 09:24:24.000000 django-beam-1.4.1/src/beam/themes/bootstrap4/templates/beam/partials/form_inline_tabular.html
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     2865 2023-04-27 07:29:04.000000 django-beam-1.4.1/src/beam/themes/bootstrap4/templates/beam/partials/form_inline_tabular_row.html
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     4856 2023-05-23 09:24:24.000000 django-beam-1.4.1/src/beam/themes/bootstrap4/templates/beam/partials/form_layout.html
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     2094 2023-05-23 09:24:24.000000 django-beam-1.4.1/src/beam/themes/bootstrap4/templates/beam/partials/layout.html
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)      666 2023-04-27 07:29:04.000000 django-beam-1.4.1/src/beam/themes/bootstrap4/templates/beam/partials/links.html
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)      635 2023-04-27 07:29:04.000000 django-beam-1.4.1/src/beam/themes/bootstrap4/templates/beam/partials/list_links.html
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)      776 2023-04-27 07:29:04.000000 django-beam-1.4.1/src/beam/themes/bootstrap4/templates/beam/partials/messages.html
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     4826 2023-05-17 08:50:04.000000 django-beam-1.4.1/src/beam/themes/bootstrap4/templates/beam/partials/navigation.html
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     5068 2023-05-23 09:24:24.000000 django-beam-1.4.1/src/beam/themes/bootstrap4/templates/beam/partials/pagination.html
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     1489 2023-04-27 07:29:04.000000 django-beam-1.4.1/src/beam/themes/bootstrap4/templates/beam/update.html
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)      946 2023-04-27 07:29:04.000000 django-beam-1.4.1/src/beam/themes/bootstrap4/widgets.py
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)      127 2023-04-27 07:29:03.000000 django-beam-1.4.1/src/beam/types.py
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)      983 2023-04-27 07:29:03.000000 django-beam-1.4.1/src/beam/urls.py
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     1584 2023-05-17 08:50:04.000000 django-beam-1.4.1/src/beam/utils.py
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)    21601 2023-04-27 07:29:03.000000 django-beam-1.4.1/src/beam/views.py
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     7528 2023-04-27 07:29:03.000000 django-beam-1.4.1/src/beam/viewsets.py
-drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-05-23 09:27:00.415548 django-beam-1.4.1/src/django_beam.egg-info/
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     3403 2023-05-23 09:27:00.000000 django-beam-1.4.1/src/django_beam.egg-info/PKG-INFO
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     4077 2023-05-23 09:27:00.000000 django-beam-1.4.1/src/django_beam.egg-info/SOURCES.txt
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)        1 2023-05-23 09:27:00.000000 django-beam-1.4.1/src/django_beam.egg-info/dependency_links.txt
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)       88 2023-05-23 09:27:00.000000 django-beam-1.4.1/src/django_beam.egg-info/requires.txt
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)        5 2023-05-23 09:27:00.000000 django-beam-1.4.1/src/django_beam.egg-info/top_level.txt
-drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-05-23 09:27:00.422086 django-beam-1.4.1/tests/
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)    15449 2022-04-27 09:12:32.000000 django-beam-1.4.1/tests/test_actions.py
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     2782 2023-01-11 09:59:58.000000 django-beam-1.4.1/tests/test_components.py
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)    14309 2023-01-23 10:38:56.000000 django-beam-1.4.1/tests/test_contrib_auth.py
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     2040 2022-04-27 09:12:32.000000 django-beam-1.4.1/tests/test_contrib_autocomplete.py
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)    10694 2023-04-27 06:08:23.000000 django-beam-1.4.1/tests/test_contrib_reversion.py
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)      850 2022-04-27 09:12:32.000000 django-beam-1.4.1/tests/test_inlines.py
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)        0 2022-04-27 09:12:32.000000 django-beam-1.4.1/tests/test_layouts.py
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     1849 2022-04-27 09:12:32.000000 django-beam-1.4.1/tests/test_registry.py
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     3284 2023-05-17 08:50:04.000000 django-beam-1.4.1/tests/test_tags.py
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     4771 2023-01-11 09:59:58.000000 django-beam-1.4.1/tests/test_urls.py
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     3946 2023-01-11 09:59:58.000000 django-beam-1.4.1/tests/test_utils.py
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)    31258 2023-03-30 10:35:40.000000 django-beam-1.4.1/tests/test_views.py
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     4275 2022-04-27 09:12:32.000000 django-beam-1.4.1/tests/test_viewsets.py
+drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-07-13 12:43:43.255217 django-beam-1.4.2/
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     1511 2022-04-27 09:12:32.000000 django-beam-1.4.2/LICENSE
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)      284 2023-01-09 10:44:11.000000 django-beam-1.4.2/MANIFEST.in
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     3403 2023-07-13 12:43:43.255291 django-beam-1.4.2/PKG-INFO
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     2954 2023-03-28 08:37:32.000000 django-beam-1.4.2/README.md
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)      740 2023-07-13 12:43:43.255835 django-beam-1.4.2/setup.cfg
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)       53 2022-04-27 09:12:32.000000 django-beam-1.4.2/setup.py
+drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-07-13 12:43:43.231379 django-beam-1.4.2/src/
+drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-07-13 12:43:43.237210 django-beam-1.4.2/src/beam/
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)      105 2023-05-30 12:51:34.000000 django-beam-1.4.2/src/beam/__init__.py
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     4680 2023-05-30 12:51:34.000000 django-beam-1.4.2/src/beam/actions.py
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     7485 2023-05-30 12:51:34.000000 django-beam-1.4.2/src/beam/components.py
+drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-07-13 12:43:43.237488 django-beam-1.4.2/src/beam/contrib/
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)        0 2023-05-30 12:51:34.000000 django-beam-1.4.2/src/beam/contrib/__init__.py
+drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-07-13 12:43:43.238153 django-beam-1.4.2/src/beam/contrib/auth/
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)        0 2023-05-30 12:51:34.000000 django-beam-1.4.2/src/beam/contrib/auth/__init__.py
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)      196 2023-05-30 12:51:34.000000 django-beam-1.4.2/src/beam/contrib/auth/apps.py
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)      903 2023-05-30 12:51:34.000000 django-beam-1.4.2/src/beam/contrib/auth/forms.py
+drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-07-13 12:43:43.230107 django-beam-1.4.2/src/beam/contrib/auth/templates/
+drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-07-13 12:43:43.239867 django-beam-1.4.2/src/beam/contrib/auth/templates/registration/
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)      296 2023-05-30 12:51:34.000000 django-beam-1.4.2/src/beam/contrib/auth/templates/registration/logged_out.html
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     1136 2023-05-30 12:51:34.000000 django-beam-1.4.2/src/beam/contrib/auth/templates/registration/login.html
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)      261 2023-05-30 12:51:34.000000 django-beam-1.4.2/src/beam/contrib/auth/templates/registration/password_change_done.html
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)      837 2023-05-30 12:51:34.000000 django-beam-1.4.2/src/beam/contrib/auth/templates/registration/password_change_form.html
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)      364 2023-05-30 12:51:34.000000 django-beam-1.4.2/src/beam/contrib/auth/templates/registration/password_reset_complete.html
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)      980 2023-05-30 12:51:34.000000 django-beam-1.4.2/src/beam/contrib/auth/templates/registration/password_reset_confirm.html
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)      535 2023-05-30 12:51:34.000000 django-beam-1.4.2/src/beam/contrib/auth/templates/registration/password_reset_done.html
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)      616 2023-05-30 12:51:34.000000 django-beam-1.4.2/src/beam/contrib/auth/templates/registration/password_reset_email.html
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)      531 2023-05-30 12:51:34.000000 django-beam-1.4.2/src/beam/contrib/auth/templates/registration/password_reset_form.html
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)      230 2023-05-30 12:51:34.000000 django-beam-1.4.2/src/beam/contrib/auth/urls.py
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     3881 2023-05-30 12:51:34.000000 django-beam-1.4.2/src/beam/contrib/auth/views.py
+drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-07-13 12:43:43.240018 django-beam-1.4.2/src/beam/contrib/autocomplete_light/
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     2940 2023-05-30 12:51:34.000000 django-beam-1.4.2/src/beam/contrib/autocomplete_light/__init__.py
+drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-07-13 12:43:43.230305 django-beam-1.4.2/src/beam/contrib/autocomplete_light/static/
+drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-07-13 12:43:43.240166 django-beam-1.4.2/src/beam/contrib/autocomplete_light/static/autocomplete_light/
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     1011 2023-05-30 12:51:34.000000 django-beam-1.4.2/src/beam/contrib/autocomplete_light/static/autocomplete_light/select2.css
+drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-07-13 12:43:43.240756 django-beam-1.4.2/src/beam/contrib/reversion/
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)        0 2023-05-30 12:51:34.000000 django-beam-1.4.2/src/beam/contrib/reversion/__init__.py
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)      150 2023-05-30 12:51:34.000000 django-beam-1.4.2/src/beam/contrib/reversion/apps.py
+drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-07-13 12:43:43.230492 django-beam-1.4.2/src/beam/contrib/reversion/templates/
+drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-07-13 12:43:43.241049 django-beam-1.4.2/src/beam/contrib/reversion/templates/beam_reversion/
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     1140 2023-05-30 12:51:34.000000 django-beam-1.4.2/src/beam/contrib/reversion/templates/beam_reversion/version_detail.html
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     1879 2023-05-30 12:51:34.000000 django-beam-1.4.2/src/beam/contrib/reversion/templates/beam_reversion/version_list.html
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     4032 2023-05-30 12:51:34.000000 django-beam-1.4.2/src/beam/contrib/reversion/views.py
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     7137 2023-05-30 12:51:34.000000 django-beam-1.4.2/src/beam/contrib/reversion/viewsets.py
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)    11062 2023-05-30 12:51:34.000000 django-beam-1.4.2/src/beam/inlines.py
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     1235 2023-05-30 12:51:34.000000 django-beam-1.4.2/src/beam/layouts.py
+drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-07-13 12:43:43.230620 django-beam-1.4.2/src/beam/locale/
+drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-07-13 12:43:43.230674 django-beam-1.4.2/src/beam/locale/de/
+drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-07-13 12:43:43.241197 django-beam-1.4.2/src/beam/locale/de/LC_MESSAGES/
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     5525 2023-05-30 12:51:34.000000 django-beam-1.4.2/src/beam/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     2814 2023-05-30 12:51:34.000000 django-beam-1.4.2/src/beam/registry.py
+drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-07-13 12:43:43.241438 django-beam-1.4.2/src/beam/templatetags/
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)        0 2023-05-30 12:51:34.000000 django-beam-1.4.2/src/beam/templatetags/__init__.py
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)    10854 2023-07-13 12:40:44.000000 django-beam-1.4.2/src/beam/templatetags/beam_tags.py
+drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-07-13 12:43:43.241696 django-beam-1.4.2/src/beam/themes/
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)        0 2023-05-30 12:51:34.000000 django-beam-1.4.2/src/beam/themes/__init__.py
+drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-07-13 12:43:43.241888 django-beam-1.4.2/src/beam/themes/bootstrap4/
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)        0 2023-05-30 12:51:34.000000 django-beam-1.4.2/src/beam/themes/bootstrap4/__init__.py
+drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-07-13 12:43:43.231001 django-beam-1.4.2/src/beam/themes/bootstrap4/static/
+drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-07-13 12:43:43.231118 django-beam-1.4.2/src/beam/themes/bootstrap4/static/beam/
+drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-07-13 12:43:43.242033 django-beam-1.4.2/src/beam/themes/bootstrap4/static/beam/css/
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)    12660 2023-05-30 12:51:34.000000 django-beam-1.4.2/src/beam/themes/bootstrap4/static/beam/css/bootstrap-select.min.css
+drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-07-13 12:43:43.243094 django-beam-1.4.2/src/beam/themes/bootstrap4/static/beam/js/
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     3291 2023-05-30 12:51:34.000000 django-beam-1.4.2/src/beam/themes/bootstrap4/static/beam/js/actions.js
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     1328 2023-05-30 12:51:34.000000 django-beam-1.4.2/src/beam/themes/bootstrap4/static/beam/js/add_related.js
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)    94341 2023-05-30 12:51:34.000000 django-beam-1.4.2/src/beam/themes/bootstrap4/static/beam/js/bootstrap-select.min.js
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     6007 2023-05-30 12:51:34.000000 django-beam-1.4.2/src/beam/themes/bootstrap4/static/beam/js/inlines.js
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)    82676 2023-05-30 12:51:34.000000 django-beam-1.4.2/src/beam/themes/bootstrap4/static/beam/js/sortable.min.js
+drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-07-13 12:43:43.231238 django-beam-1.4.2/src/beam/themes/bootstrap4/templates/
+drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-07-13 12:43:43.245522 django-beam-1.4.2/src/beam/themes/bootstrap4/templates/beam/
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     3374 2023-05-30 12:51:34.000000 django-beam-1.4.2/src/beam/themes/bootstrap4/templates/beam/base.html
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)      261 2023-05-30 12:51:34.000000 django-beam-1.4.2/src/beam/themes/bootstrap4/templates/beam/create.html
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     1537 2023-05-30 12:51:34.000000 django-beam-1.4.2/src/beam/themes/bootstrap4/templates/beam/dashboard.html
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     2265 2023-05-30 12:51:34.000000 django-beam-1.4.2/src/beam/themes/bootstrap4/templates/beam/delete.html
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     2894 2023-05-30 12:51:34.000000 django-beam-1.4.2/src/beam/themes/bootstrap4/templates/beam/detail.html
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     4361 2023-07-13 12:40:03.000000 django-beam-1.4.2/src/beam/themes/bootstrap4/templates/beam/form.html
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     8143 2023-07-13 12:40:44.000000 django-beam-1.4.2/src/beam/themes/bootstrap4/templates/beam/list.html
+drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-07-13 12:43:43.249422 django-beam-1.4.2/src/beam/themes/bootstrap4/templates/beam/partials/
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     1750 2023-05-30 12:51:34.000000 django-beam-1.4.2/src/beam/themes/bootstrap4/templates/beam/partials/actions.html
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     2168 2023-05-30 12:51:34.000000 django-beam-1.4.2/src/beam/themes/bootstrap4/templates/beam/partials/detail_field.html
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     4596 2023-05-30 12:51:34.000000 django-beam-1.4.2/src/beam/themes/bootstrap4/templates/beam/partials/detail_inline.html
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     3298 2023-05-30 12:51:34.000000 django-beam-1.4.2/src/beam/themes/bootstrap4/templates/beam/partials/detail_inline_tabular.html
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     1516 2023-07-13 12:40:44.000000 django-beam-1.4.2/src/beam/themes/bootstrap4/templates/beam/partials/filters.html
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)      843 2023-07-13 12:39:52.000000 django-beam-1.4.2/src/beam/themes/bootstrap4/templates/beam/partials/form_field.html
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     6373 2023-05-30 12:51:34.000000 django-beam-1.4.2/src/beam/themes/bootstrap4/templates/beam/partials/form_inline.html
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     3075 2023-05-30 12:51:34.000000 django-beam-1.4.2/src/beam/themes/bootstrap4/templates/beam/partials/form_inline_tabular.html
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     2865 2023-05-30 12:51:34.000000 django-beam-1.4.2/src/beam/themes/bootstrap4/templates/beam/partials/form_inline_tabular_row.html
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     4856 2023-05-30 12:51:34.000000 django-beam-1.4.2/src/beam/themes/bootstrap4/templates/beam/partials/form_layout.html
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     2094 2023-05-30 12:51:34.000000 django-beam-1.4.2/src/beam/themes/bootstrap4/templates/beam/partials/layout.html
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)      666 2023-05-30 12:51:34.000000 django-beam-1.4.2/src/beam/themes/bootstrap4/templates/beam/partials/links.html
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)      635 2023-05-30 12:51:34.000000 django-beam-1.4.2/src/beam/themes/bootstrap4/templates/beam/partials/list_links.html
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)      776 2023-05-30 12:51:34.000000 django-beam-1.4.2/src/beam/themes/bootstrap4/templates/beam/partials/messages.html
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     4826 2023-05-30 12:51:34.000000 django-beam-1.4.2/src/beam/themes/bootstrap4/templates/beam/partials/navigation.html
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     5068 2023-05-30 12:51:34.000000 django-beam-1.4.2/src/beam/themes/bootstrap4/templates/beam/partials/pagination.html
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     1489 2023-05-30 12:51:34.000000 django-beam-1.4.2/src/beam/themes/bootstrap4/templates/beam/update.html
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)      946 2023-05-30 12:51:34.000000 django-beam-1.4.2/src/beam/themes/bootstrap4/widgets.py
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)      127 2023-05-30 12:51:34.000000 django-beam-1.4.2/src/beam/types.py
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)      983 2023-05-30 12:51:34.000000 django-beam-1.4.2/src/beam/urls.py
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     1584 2023-05-30 12:51:34.000000 django-beam-1.4.2/src/beam/utils.py
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)    21601 2023-05-31 11:33:31.000000 django-beam-1.4.2/src/beam/views.py
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     7528 2023-05-30 12:51:34.000000 django-beam-1.4.2/src/beam/viewsets.py
+drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-07-13 12:43:43.250053 django-beam-1.4.2/src/django_beam.egg-info/
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     3403 2023-07-13 12:43:43.000000 django-beam-1.4.2/src/django_beam.egg-info/PKG-INFO
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     4077 2023-07-13 12:43:43.000000 django-beam-1.4.2/src/django_beam.egg-info/SOURCES.txt
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)        1 2023-07-13 12:43:43.000000 django-beam-1.4.2/src/django_beam.egg-info/dependency_links.txt
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)       88 2023-07-13 12:43:43.000000 django-beam-1.4.2/src/django_beam.egg-info/requires.txt
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)        5 2023-07-13 12:43:43.000000 django-beam-1.4.2/src/django_beam.egg-info/top_level.txt
+drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-07-13 12:43:43.255066 django-beam-1.4.2/tests/
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)    15449 2022-04-27 09:12:32.000000 django-beam-1.4.2/tests/test_actions.py
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     2782 2023-01-11 09:59:58.000000 django-beam-1.4.2/tests/test_components.py
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)    14309 2023-01-23 10:38:56.000000 django-beam-1.4.2/tests/test_contrib_auth.py
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     2040 2022-04-27 09:12:32.000000 django-beam-1.4.2/tests/test_contrib_autocomplete.py
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)    10694 2023-04-27 06:08:23.000000 django-beam-1.4.2/tests/test_contrib_reversion.py
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)      850 2022-04-27 09:12:32.000000 django-beam-1.4.2/tests/test_inlines.py
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)        0 2022-04-27 09:12:32.000000 django-beam-1.4.2/tests/test_layouts.py
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     1849 2022-04-27 09:12:32.000000 django-beam-1.4.2/tests/test_registry.py
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     3284 2023-05-17 08:50:04.000000 django-beam-1.4.2/tests/test_tags.py
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     4771 2023-01-11 09:59:58.000000 django-beam-1.4.2/tests/test_urls.py
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     3946 2023-01-11 09:59:58.000000 django-beam-1.4.2/tests/test_utils.py
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)    31258 2023-03-30 10:35:40.000000 django-beam-1.4.2/tests/test_views.py
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     4275 2022-04-27 09:12:32.000000 django-beam-1.4.2/tests/test_viewsets.py
```

### Comparing `django-beam-1.4.1/LICENSE` & `django-beam-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.1/PKG-INFO` & `django-beam-1.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: django-beam
-Version: 1.4.1
+Version: 1.4.2
 Summary: A crud library for python
 Home-page: https://github.com/django-beam/django-beam
-Download-URL: https://github.com/django-beam/django-beam/archive/1.4.1.tar.gz
+Download-URL: https://github.com/django-beam/django-beam/archive/1.4.2.tar.gz
 Author: Raphael Kimmig
 Author-email: raphael@ampad.de
 License: BSD 3-Clause License
 Classifier: Framework :: Django
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `django-beam-1.4.1/README.md` & `django-beam-1.4.2/README.md`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.1/setup.cfg` & `django-beam-1.4.2/setup.cfg`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [metadata]
 name = django-beam
-version = 1.4.1
+version = 1.4.2
 description = A crud library for python
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/django-beam/django-beam
-download_url = https://github.com/django-beam/django-beam/archive/1.4.1.tar.gz
+download_url = https://github.com/django-beam/django-beam/archive/1.4.2.tar.gz
 author = Raphael Kimmig
 author_email = raphael@ampad.de
 keywords = 
 license = BSD 3-Clause License
 classifiers = 
 	Framework :: Django
 	Programming Language :: Python :: 3
```

### Comparing `django-beam-1.4.1/src/beam/actions.py` & `django-beam-1.4.2/src/beam/actions.py`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.1/src/beam/components.py` & `django-beam-1.4.2/src/beam/components.py`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.1/src/beam/contrib/auth/forms.py` & `django-beam-1.4.2/src/beam/contrib/auth/forms.py`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.1/src/beam/contrib/auth/templates/registration/login.html` & `django-beam-1.4.2/src/beam/contrib/auth/templates/registration/login.html`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.1/src/beam/contrib/auth/templates/registration/password_change_form.html` & `django-beam-1.4.2/src/beam/contrib/auth/templates/registration/password_change_form.html`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.1/src/beam/contrib/auth/templates/registration/password_reset_confirm.html` & `django-beam-1.4.2/src/beam/contrib/auth/templates/registration/password_reset_confirm.html`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.1/src/beam/contrib/auth/templates/registration/password_reset_done.html` & `django-beam-1.4.2/src/beam/contrib/auth/templates/registration/password_reset_done.html`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.1/src/beam/contrib/auth/templates/registration/password_reset_email.html` & `django-beam-1.4.2/src/beam/contrib/auth/templates/registration/password_reset_email.html`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.1/src/beam/contrib/auth/templates/registration/password_reset_form.html` & `django-beam-1.4.2/src/beam/contrib/auth/templates/registration/password_reset_form.html`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.1/src/beam/contrib/auth/views.py` & `django-beam-1.4.2/src/beam/contrib/auth/views.py`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.1/src/beam/contrib/autocomplete_light/__init__.py` & `django-beam-1.4.2/src/beam/contrib/autocomplete_light/__init__.py`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.1/src/beam/contrib/autocomplete_light/static/autocomplete_light/select2.css` & `django-beam-1.4.2/src/beam/contrib/autocomplete_light/static/autocomplete_light/select2.css`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.1/src/beam/contrib/reversion/templates/beam_reversion/version_detail.html` & `django-beam-1.4.2/src/beam/contrib/reversion/templates/beam_reversion/version_detail.html`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.1/src/beam/contrib/reversion/templates/beam_reversion/version_list.html` & `django-beam-1.4.2/src/beam/contrib/reversion/templates/beam_reversion/version_list.html`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.1/src/beam/contrib/reversion/views.py` & `django-beam-1.4.2/src/beam/contrib/reversion/views.py`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.1/src/beam/contrib/reversion/viewsets.py` & `django-beam-1.4.2/src/beam/contrib/reversion/viewsets.py`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.1/src/beam/inlines.py` & `django-beam-1.4.2/src/beam/inlines.py`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.1/src/beam/layouts.py` & `django-beam-1.4.2/src/beam/layouts.py`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.1/src/beam/locale/de/LC_MESSAGES/django.mo` & `django-beam-1.4.2/src/beam/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.1/src/beam/registry.py` & `django-beam-1.4.2/src/beam/registry.py`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.1/src/beam/templatetags/beam_tags.py` & `django-beam-1.4.2/src/beam/templatetags/beam_tags.py`

 * *Files 23% similar despite different names*

```diff
@@ -4,17 +4,20 @@
 
 from django import template
 from django.apps import apps
 from django.core.exceptions import FieldDoesNotExist
 from django.db.models import Manager, Model, QuerySet
 from django.db.models.fields.files import FieldFile, ImageFieldFile
 from django.db.models.fields.reverse_related import ForeignObjectRel
+from django.forms import Form
 from django.template import RequestContext
 from django.template.loader import get_template
+from django.utils.html import escape
 from django.utils.http import urlencode
+from django.utils.safestring import mark_safe
 
 from beam.components import BaseComponent
 from beam.layouts import layout_links
 from beam.registry import default_registry, get_viewset_for_model
 from beam.utils import navigation_component_entry, reverse_component
 
 register = template.Library()
@@ -224,15 +227,15 @@
 
 @register.simple_tag()
 def fields_to_layout(fields):
     return [[fields]]
 
 
 @register.simple_tag(takes_context=True)
-def sort_link(context, field: str, sorted_fields: Sequence[str]):
+def sort_link(context, field: str, sorted_fields: Sequence[str], page_param=None):
     sort_param = context["view"].sort_param
     sort_separator = context["view"].sort_separator
 
     sorted_fields = list(sorted_fields)
     negated_field = "-" + field
 
     if field in sorted_fields:
@@ -241,40 +244,96 @@
     elif negated_field in sorted_fields:
         sorted_fields.remove(negated_field)
         sorted_fields.append(field)
     else:
         sorted_fields.append(field)
 
     return preserve_query_string(
-        context, **{"page": "", sort_param: sort_separator.join(sorted_fields)}
+        context, ignore_params=page_param, **{sort_param: sort_separator.join(sorted_fields)}
     )
 
 
 @register.simple_tag(takes_context=True)
-def page_link(context, page_query_string, page_number):
-    return preserve_query_string(context, **{page_query_string: page_number})
+def page_link(context, page_param, page_number):
+    return preserve_query_string(context, **{page_param: page_number})
 
 
 @register.simple_tag(takes_context=True)
-def preserve_query_string(context, **kwargs):
+def preserve_query_string(context, ignore_params=None, **kwargs):
+    get = preserve_get_params(context, ignore_params=ignore_params, **kwargs)
+    return "?{}".format(get.urlencode())
+
+
+@register.simple_tag(takes_context=True)
+def preserve_get_params_as_hidden_inputs(context, ignore_params=None, **kwargs):
+    get = preserve_get_params(context, ignore_params=ignore_params, **kwargs)
+    inputs = [
+        f'<input type="hidden" name="{escape(k)}" value="{escape(v)}">' for k, v in get.items()
+    ]
+    return mark_safe("".join(inputs))
+
+
+@register.simple_tag(takes_context=True)
+def preserve_get_params(context, ignore_params=None, **kwargs):
+    """Preserve GET parameters from the current URL, whilst overwriting parameters
+    given by optional kwargs. Optional ignore_params will be removed from the parameters.
+
+    :param context: a Django template context
+    :param ignore_params: if provided, the ignore_params will be removed from the get parameters
+    :param kwargs: further kwargs will overwrite parameters with the given values
+    :return: a dict with all preserved get parameters
+    """
     if "request" not in context:
         raise Exception(
-            "The query_string tag requires django.core.context_processors.request"
+            "The preserve_get_params tag requires django.core.context_processors.request"
         )
-    request = context["request"]
 
+    request = context["request"]
     get = request.GET.copy()
 
-    for item, value in kwargs.items():
+    # ignore_params may be a string
+    if isinstance(ignore_params, str):
+        get.pop(ignore_params, None)
+
+    # or a list of strings
+    elif isinstance(ignore_params, list):
+        for param in ignore_params:
+            get.pop(param, None)
+
+    # kwargs overwrite the parameters
+    for key, value in kwargs.items():
         if value == "":
-            get.pop(item, None)
+            get.pop(key, None)
         else:
-            get[item] = value
+            get[key] = value
 
-    return "?{}".format(get.urlencode())
+    return get
+
+
+@register.simple_tag
+def build_ignore_params(*args):
+    """
+    Builds a list of parameter names which should be ignored when preserving GET params.
+
+    :param args: each arg may be a name of a parameter to ignore
+        or a form, whose fields should be ignored
+    :return: a list of parameter names to ignore
+    """
+    ignore_params = []
+    for arg in args:
+        if isinstance(arg, Form):
+            for field in arg:
+                key = field.name
+                if arg.prefix:
+                    key = arg.prefix + "-" + key
+                ignore_params.append(key)
+        elif isinstance(arg, str):
+            ignore_params.append(arg)
+
+    return ignore_params
 
 
 def _add_params_to_url_if_new(url, default_params):
     """
     Add params from default_params unless they already exist.
     """
     parsed_url = urlparse(url)
```

### Comparing `django-beam-1.4.1/src/beam/themes/bootstrap4/static/beam/css/bootstrap-select.min.css` & `django-beam-1.4.2/src/beam/themes/bootstrap4/static/beam/css/bootstrap-select.min.css`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.1/src/beam/themes/bootstrap4/static/beam/js/actions.js` & `django-beam-1.4.2/src/beam/themes/bootstrap4/static/beam/js/actions.js`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.1/src/beam/themes/bootstrap4/static/beam/js/add_related.js` & `django-beam-1.4.2/src/beam/themes/bootstrap4/static/beam/js/add_related.js`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.1/src/beam/themes/bootstrap4/static/beam/js/bootstrap-select.min.js` & `django-beam-1.4.2/src/beam/themes/bootstrap4/static/beam/js/bootstrap-select.min.js`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.1/src/beam/themes/bootstrap4/static/beam/js/inlines.js` & `django-beam-1.4.2/src/beam/themes/bootstrap4/static/beam/js/inlines.js`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.1/src/beam/themes/bootstrap4/static/beam/js/sortable.min.js` & `django-beam-1.4.2/src/beam/themes/bootstrap4/static/beam/js/sortable.min.js`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.1/src/beam/themes/bootstrap4/templates/beam/base.html` & `django-beam-1.4.2/src/beam/themes/bootstrap4/templates/beam/base.html`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.1/src/beam/themes/bootstrap4/templates/beam/dashboard.html` & `django-beam-1.4.2/src/beam/themes/bootstrap4/templates/beam/dashboard.html`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.1/src/beam/themes/bootstrap4/templates/beam/delete.html` & `django-beam-1.4.2/src/beam/themes/bootstrap4/templates/beam/delete.html`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.1/src/beam/themes/bootstrap4/templates/beam/detail.html` & `django-beam-1.4.2/src/beam/themes/bootstrap4/templates/beam/detail.html`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.1/src/beam/themes/bootstrap4/templates/beam/form.html` & `django-beam-1.4.2/src/beam/themes/bootstrap4/templates/beam/form.html`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.1/src/beam/themes/bootstrap4/templates/beam/list.html` & `django-beam-1.4.2/src/beam/themes/bootstrap4/templates/beam/list.html`

 * *Files 5% similar despite different names*

```diff
@@ -40,33 +40,36 @@
                 {% endblock %}
             </h1>
         {% endblock %}
 
         {% block search %}
             {% if view.search_fields %}
                 <form method="get" id="search-form">
+
+                    {% preserve_get_params_as_hidden_inputs ignore_params=view.page_kwarg q="" %}
+
                     <div class="input-group">
                         <input name="q" type="text" value="{{ search_query }}" class="form-control"
                                placeholder="{% trans 'Search the list below' %}"
                                aria-label="{% trans 'Search the list below' %}"
                                aria-describedby="search-form-input">
                         <div class="input-group-append">
 
                             {% if search_query %}
-                                <a href="{{ request.path }}"
+                                <a href="{{ request.path }}{% preserve_query_string ignore_params=view.page_kwarg q="" %}"
                                    class="btn btn-outline-secondary">{% trans "Clear" %}</a>
                             {% endif %}
                             <input type="submit" class="btn btn-outline-primary" value="{% trans 'Search' %}"/>
                         </div>
                     </div>
                 </form>
             {% endif %}
         {% endblock %}
         {% block filters %}
-            {% include "beam/partials/filters.html" %}
+            {% include "beam/partials/filters.html" with page_param=view.page_kwarg %}
         {% endblock %}
 
         {% if actions %}
         <form method="post" id="list-action-form" novalidate>
             {% csrf_token %}
             {% block actions %}
                 {% include "beam/partials/actions.html" %}
@@ -86,19 +89,19 @@
                     </th>
                     {% endif %}
                     {% for field in component.fields %}
                         <th scope="col" class="beam-list-field-label beam-field-label-{{ field }}">
                             {% with field_name=field|stringformat:"s" %}{# cast to string to support virtual fields #}
                                 {% if field_name in sortable_fields %}
                                     {# fixme text-nowrap only if there is a chance to fit this?  #}
-                                    <a class="text-nowrap" href="{% sort_link field_name sorted_fields %}">
+                                    <a class="text-nowrap" href="{% sort_link field_name sorted_fields page_param=view.page_kwarg %}">
                                         {{ component.model|field_verbose_name:field|capfirst }}&nbsp;{% if field_name in sorted_fields %}<i class="fa fa-caret-up"></i>{% elif "-"|add:field_name in sorted_fields %}<i class="fa fa-caret-down"></i>{% endif %}
                                     </a>
                                     {% if field_name in sorted_fields or "-"|add:field_name in sorted_fields %}
-                                        <a title="{% trans "reset sort" %}" href="{% sort_link "" "" %}"><i class="fa fa-remove"></i></a>
+                                        <a title="{% trans "reset sort" %}" href="{% sort_link "" "" page_param=view.page_kwarg %}"><i class="fa fa-remove"></i></a>
                                     {% endif %}
                                 {% else %}
                                     {{ component.model|field_verbose_name:field|capfirst }}
                                 {% endif %}
                             {% endwith %}
                         </th>
                     {% endfor %}
```

#### html2text {}

```diff
@@ -12,27 +12,31 @@
 component.model as options %}  {% block links_container %}
 {% block links %} {% include "beam/partials/links.html" with
 links=viewset.links link_layout=component.link_layout %} {% endblock %}
 {% endblock %} {% block heading_container %}
 ****** {% block heading %} {% if heading %} {{ heading }} {% else %} {
 { options.verbose_name_plural|capfirst }} {% endif %} {% endblock %} ******
 {% endblock %} {% block search %} {% if view.search_fields %}
+{% preserve_get_params_as_hidden_inputs ignore_params=view.page_kwarg q="" %}
 [{{ search_query }}  ]
-{% if search_query %} {%_trans_"Clear"_%} {% endif %} [{% trans 'Search' %}]
+{% if search_query %}
+ %}" class="btn btn-outline-secondary">{% trans "Clear" %}
+ {% endif %} [{% trans 'Search' %}]
 {% endif %} {% endblock %} {% block filters %} {% include "beam/partials/
-filters.html" %} {% endblock %} {% if actions %}
+filters.html" with page_param=view.page_kwarg %} {% endblock %} {% if actions
+%}
 {% csrf_token %} {% block actions %} {% include "beam/partials/actions.html" %}
 {% endblock %} {% endif %} {% block table %}
                  {% with field_name=field|stringformat:"s" %}{# cast to string to support
                  virtual fields #} {% if field_name in sortable_fields %} {# fixme text-
  %}"             nowrap only if there is a chance to fit this? #}
 class="beam-     {{_component.model|field_verbose_name:field|capfirst_}} {%_if_field_name_in
 action__select-  sorted_fields_%}{%_elif_"-"|add:field_name_in_sorted_fields_%}{%_endif_%}    {% trans "Actions" %}
 all"              {% if field_name in sorted_fields or "-"|add:field_name in sorted_fields %}
-type="checkbox">  %}" href="{% sort_link "" "" %}">
+type="checkbox">  %}" href="{% sort_link "" "" page_param=view.page_kwarg %}">
                   {% endif %} {% else %} {{ component.model|field_verbose_name:field|capfirst
                  }} {% endif %} {% endwith %}
                                                                                               {% include "beam/partials/list_links.html"
 ⁰              {% include "beam/partials/detail_field.html" with object=object field=field  with links=viewset.links
                  %}                                                                           link_layout=component.list_item_link_layout
                                                                                               object=object %}
 {% endblock %} {% block no_results %} {% if not object_list %}
```

### Comparing `django-beam-1.4.1/src/beam/themes/bootstrap4/templates/beam/partials/actions.html` & `django-beam-1.4.2/src/beam/themes/bootstrap4/templates/beam/partials/actions.html`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.1/src/beam/themes/bootstrap4/templates/beam/partials/detail_field.html` & `django-beam-1.4.2/src/beam/themes/bootstrap4/templates/beam/partials/detail_field.html`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.1/src/beam/themes/bootstrap4/templates/beam/partials/detail_inline.html` & `django-beam-1.4.2/src/beam/themes/bootstrap4/templates/beam/partials/detail_inline.html`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.1/src/beam/themes/bootstrap4/templates/beam/partials/detail_inline_tabular.html` & `django-beam-1.4.2/src/beam/themes/bootstrap4/templates/beam/partials/detail_inline_tabular.html`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.1/src/beam/themes/bootstrap4/templates/beam/partials/form_inline.html` & `django-beam-1.4.2/src/beam/themes/bootstrap4/templates/beam/partials/form_inline.html`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.1/src/beam/themes/bootstrap4/templates/beam/partials/form_inline_tabular.html` & `django-beam-1.4.2/src/beam/themes/bootstrap4/templates/beam/partials/form_inline_tabular.html`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.1/src/beam/themes/bootstrap4/templates/beam/partials/form_inline_tabular_row.html` & `django-beam-1.4.2/src/beam/themes/bootstrap4/templates/beam/partials/form_inline_tabular_row.html`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.1/src/beam/themes/bootstrap4/templates/beam/partials/form_layout.html` & `django-beam-1.4.2/src/beam/themes/bootstrap4/templates/beam/partials/form_layout.html`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.1/src/beam/themes/bootstrap4/templates/beam/partials/layout.html` & `django-beam-1.4.2/src/beam/themes/bootstrap4/templates/beam/partials/layout.html`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.1/src/beam/themes/bootstrap4/templates/beam/partials/links.html` & `django-beam-1.4.2/src/beam/themes/bootstrap4/templates/beam/partials/links.html`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.1/src/beam/themes/bootstrap4/templates/beam/partials/list_links.html` & `django-beam-1.4.2/src/beam/themes/bootstrap4/templates/beam/partials/list_links.html`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.1/src/beam/themes/bootstrap4/templates/beam/partials/messages.html` & `django-beam-1.4.2/src/beam/themes/bootstrap4/templates/beam/partials/messages.html`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.1/src/beam/themes/bootstrap4/templates/beam/partials/navigation.html` & `django-beam-1.4.2/src/beam/themes/bootstrap4/templates/beam/partials/navigation.html`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.1/src/beam/themes/bootstrap4/templates/beam/partials/pagination.html` & `django-beam-1.4.2/src/beam/themes/bootstrap4/templates/beam/partials/pagination.html`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.1/src/beam/themes/bootstrap4/templates/beam/update.html` & `django-beam-1.4.2/src/beam/themes/bootstrap4/templates/beam/update.html`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.1/src/beam/themes/bootstrap4/widgets.py` & `django-beam-1.4.2/src/beam/themes/bootstrap4/widgets.py`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.1/src/beam/urls.py` & `django-beam-1.4.2/src/beam/urls.py`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.1/src/beam/utils.py` & `django-beam-1.4.2/src/beam/utils.py`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.1/src/beam/views.py` & `django-beam-1.4.2/src/beam/views.py`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.1/src/beam/viewsets.py` & `django-beam-1.4.2/src/beam/viewsets.py`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.1/src/django_beam.egg-info/PKG-INFO` & `django-beam-1.4.2/src/django_beam.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: django-beam
-Version: 1.4.1
+Version: 1.4.2
 Summary: A crud library for python
 Home-page: https://github.com/django-beam/django-beam
-Download-URL: https://github.com/django-beam/django-beam/archive/1.4.1.tar.gz
+Download-URL: https://github.com/django-beam/django-beam/archive/1.4.2.tar.gz
 Author: Raphael Kimmig
 Author-email: raphael@ampad.de
 License: BSD 3-Clause License
 Classifier: Framework :: Django
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `django-beam-1.4.1/src/django_beam.egg-info/SOURCES.txt` & `django-beam-1.4.2/src/django_beam.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.1/tests/test_actions.py` & `django-beam-1.4.2/tests/test_actions.py`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.1/tests/test_components.py` & `django-beam-1.4.2/tests/test_components.py`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.1/tests/test_contrib_auth.py` & `django-beam-1.4.2/tests/test_contrib_auth.py`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.1/tests/test_contrib_autocomplete.py` & `django-beam-1.4.2/tests/test_contrib_autocomplete.py`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.1/tests/test_contrib_reversion.py` & `django-beam-1.4.2/tests/test_contrib_reversion.py`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.1/tests/test_inlines.py` & `django-beam-1.4.2/tests/test_inlines.py`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.1/tests/test_registry.py` & `django-beam-1.4.2/tests/test_registry.py`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.1/tests/test_tags.py` & `django-beam-1.4.2/tests/test_tags.py`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.1/tests/test_urls.py` & `django-beam-1.4.2/tests/test_urls.py`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.1/tests/test_utils.py` & `django-beam-1.4.2/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.1/tests/test_views.py` & `django-beam-1.4.2/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.1/tests/test_viewsets.py` & `django-beam-1.4.2/tests/test_viewsets.py`

 * *Files identical despite different names*

