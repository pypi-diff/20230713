# Comparing `tmp/django-mp-cap-3.0.5.tar.gz` & `tmp/django-mp-cap-3.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-mp-cap-3.0.5.tar", last modified: Wed Apr 26 13:38:23 2023, max compression
+gzip compressed data, was "dist/django-mp-cap-3.0.6.tar", last modified: Thu Jul 13 14:19:09 2023, max compression
```

## Comparing `django-mp-cap-3.0.5.tar` & `django-mp-cap-3.0.6.tar`

### file list

```diff
@@ -1,155 +1,158 @@
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-04-26 13:38:23.000000 django-mp-cap-3.0.5/
--rw-rw-r--   0 dev       (1000) dev       (1000)      746 2021-12-18 20:11:37.000000 django-mp-cap-3.0.5/LICENSE
--rw-rw-r--   0 dev       (1000) dev       (1000)      161 2022-02-21 14:06:34.000000 django-mp-cap-3.0.5/MANIFEST.in
--rw-rw-r--   0 dev       (1000) dev       (1000)      324 2023-04-26 13:38:23.000000 django-mp-cap-3.0.5/PKG-INFO
--rw-rw-r--   0 dev       (1000) dev       (1000)      245 2022-02-21 14:06:34.000000 django-mp-cap-3.0.5/README.md
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-04-26 13:38:23.000000 django-mp-cap-3.0.5/cap/
--rw-rw-r--   0 dev       (1000) dev       (1000)     1757 2023-04-26 13:36:09.000000 django-mp-cap-3.0.5/cap/__init__.py
--rw-rw-r--   0 dev       (1000) dev       (1000)     1535 2023-04-26 13:36:09.000000 django-mp-cap-3.0.5/cap/actions.py
--rw-rw-r--   0 dev       (1000) dev       (1000)      324 2023-04-26 13:36:09.000000 django-mp-cap-3.0.5/cap/configs.py
--rw-rw-r--   0 dev       (1000) dev       (1000)     1183 2023-04-26 13:36:09.000000 django-mp-cap-3.0.5/cap/decorators.py
--rw-rw-r--   0 dev       (1000) dev       (1000)     1735 2023-04-26 13:36:09.000000 django-mp-cap-3.0.5/cap/filters.py
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-04-26 13:38:23.000000 django-mp-cap-3.0.5/cap/locale/
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-04-26 13:38:23.000000 django-mp-cap-3.0.5/cap/locale/uk/
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-04-26 13:38:23.000000 django-mp-cap-3.0.5/cap/locale/uk/LC_MESSAGES/
--rw-rw-r--   0 dev       (1000) dev       (1000)      915 2022-06-27 18:44:23.000000 django-mp-cap-3.0.5/cap/locale/uk/LC_MESSAGES/django.mo
--rw-rw-r--   0 dev       (1000) dev       (1000)     1329 2022-06-27 18:44:23.000000 django-mp-cap-3.0.5/cap/locale/uk/LC_MESSAGES/django.po
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-04-26 13:38:23.000000 django-mp-cap-3.0.5/cap/static/
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-04-26 13:38:23.000000 django-mp-cap-3.0.5/cap/static/cap/
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-04-26 13:38:23.000000 django-mp-cap-3.0.5/cap/static/cap/components/
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-04-26 13:38:23.000000 django-mp-cap-3.0.5/cap/static/cap/components/bootstrap/
--rw-rw-r--   0 dev       (1000) dev       (1000)   159470 2023-04-26 13:36:09.000000 django-mp-cap-3.0.5/cap/static/cap/components/bootstrap/bootstrap.min.css
--rw-rw-r--   0 dev       (1000) dev       (1000)    59969 2023-04-26 13:36:09.000000 django-mp-cap-3.0.5/cap/static/cap/components/bootstrap/bootstrap.min.js
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-04-26 13:38:23.000000 django-mp-cap-3.0.5/cap/static/cap/components/bootstrap-tagsinput/
--rw-rw-r--   0 dev       (1000) dev       (1000)     1508 2022-06-27 18:44:23.000000 django-mp-cap-3.0.5/cap/static/cap/components/bootstrap-tagsinput/bootstrap-tagsinput.css
--rw-rw-r--   0 dev       (1000) dev       (1000)    22341 2023-04-26 13:36:09.000000 django-mp-cap-3.0.5/cap/static/cap/components/bootstrap-tagsinput/bootstrap-tagsinput.js
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-04-26 13:38:23.000000 django-mp-cap-3.0.5/cap/static/cap/components/bootstrap-treeview/
--rw-rw-r--   0 dev       (1000) dev       (1000)      204 2022-06-27 18:44:23.000000 django-mp-cap-3.0.5/cap/static/cap/components/bootstrap-treeview/bootstrap-treeview.min.css
--rw-rw-r--   0 dev       (1000) dev       (1000)    16735 2022-06-27 18:44:23.000000 django-mp-cap-3.0.5/cap/static/cap/components/bootstrap-treeview/bootstrap-treeview.min.js
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-04-26 13:38:23.000000 django-mp-cap-3.0.5/cap/static/cap/components/fancybox/
--rw-rw-r--   0 dev       (1000) dev       (1000)    12795 2022-06-27 18:44:23.000000 django-mp-cap-3.0.5/cap/static/cap/components/fancybox/jquery.fancybox.min.css
--rw-rw-r--   0 dev       (1000) dev       (1000)    68253 2022-06-27 18:44:23.000000 django-mp-cap-3.0.5/cap/static/cap/components/fancybox/jquery.fancybox.min.js
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-04-26 13:38:23.000000 django-mp-cap-3.0.5/cap/static/cap/components/font-awesome/
--rw-rw-r--   0 dev       (1000) dev       (1000)    30994 2022-06-27 18:44:23.000000 django-mp-cap-3.0.5/cap/static/cap/components/font-awesome/font-awesome.min.css
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-04-26 13:38:23.000000 django-mp-cap-3.0.5/cap/static/cap/components/font-awesome/fonts/
--rw-rw-r--   0 dev       (1000) dev       (1000)   134808 2022-06-27 18:44:23.000000 django-mp-cap-3.0.5/cap/static/cap/components/font-awesome/fonts/FontAwesome.otf
--rw-rw-r--   0 dev       (1000) dev       (1000)   165742 2022-06-27 18:44:23.000000 django-mp-cap-3.0.5/cap/static/cap/components/font-awesome/fonts/fontawesome-webfont.eot
--rw-rw-r--   0 dev       (1000) dev       (1000)   444379 2023-04-26 13:36:09.000000 django-mp-cap-3.0.5/cap/static/cap/components/font-awesome/fonts/fontawesome-webfont.svg
--rw-rw-r--   0 dev       (1000) dev       (1000)   165548 2022-06-27 18:44:23.000000 django-mp-cap-3.0.5/cap/static/cap/components/font-awesome/fonts/fontawesome-webfont.ttf
--rw-rw-r--   0 dev       (1000) dev       (1000)    98024 2022-06-27 18:44:23.000000 django-mp-cap-3.0.5/cap/static/cap/components/font-awesome/fonts/fontawesome-webfont.woff
--rw-rw-r--   0 dev       (1000) dev       (1000)    77160 2022-06-27 18:44:23.000000 django-mp-cap-3.0.5/cap/static/cap/components/font-awesome/fonts/fontawesome-webfont.woff2
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-04-26 13:38:23.000000 django-mp-cap-3.0.5/cap/static/cap/components/jquery-ui/
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-04-26 13:38:23.000000 django-mp-cap-3.0.5/cap/static/cap/components/jquery-ui/i18n/
--rw-rw-r--   0 dev       (1000) dev       (1000)     1157 2023-04-26 13:36:09.000000 django-mp-cap-3.0.5/cap/static/cap/components/jquery-ui/i18n/en.js
--rw-rw-r--   0 dev       (1000) dev       (1000)     1382 2023-04-26 13:36:09.000000 django-mp-cap-3.0.5/cap/static/cap/components/jquery-ui/i18n/ru.js
--rw-rw-r--   0 dev       (1000) dev       (1000)     1448 2023-04-26 13:36:09.000000 django-mp-cap-3.0.5/cap/static/cap/components/jquery-ui/i18n/uk.js
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-04-26 13:38:23.000000 django-mp-cap-3.0.5/cap/static/cap/components/jquery-ui/images/
--rw-rw-r--   0 dev       (1000) dev       (1000)       86 2022-06-27 18:44:23.000000 django-mp-cap-3.0.5/cap/static/cap/components/jquery-ui/images/ui-bg_flat_0_aaaaaa_40x100.png
--rw-rw-r--   0 dev       (1000) dev       (1000)     3266 2022-06-27 18:44:23.000000 django-mp-cap-3.0.5/cap/static/cap/components/jquery-ui/images/ui-icons_444444_256x240.png
--rw-rw-r--   0 dev       (1000) dev       (1000)     3274 2022-06-27 18:44:23.000000 django-mp-cap-3.0.5/cap/static/cap/components/jquery-ui/images/ui-icons_555555_256x240.png
--rw-rw-r--   0 dev       (1000) dev       (1000)     3262 2022-06-27 18:44:23.000000 django-mp-cap-3.0.5/cap/static/cap/components/jquery-ui/images/ui-icons_777620_256x240.png
--rw-rw-r--   0 dev       (1000) dev       (1000)     3266 2022-06-27 18:44:23.000000 django-mp-cap-3.0.5/cap/static/cap/components/jquery-ui/images/ui-icons_777777_256x240.png
--rw-rw-r--   0 dev       (1000) dev       (1000)     3262 2022-06-27 18:44:23.000000 django-mp-cap-3.0.5/cap/static/cap/components/jquery-ui/images/ui-icons_cc0000_256x240.png
--rw-rw-r--   0 dev       (1000) dev       (1000)     3264 2022-06-27 18:44:23.000000 django-mp-cap-3.0.5/cap/static/cap/components/jquery-ui/images/ui-icons_ffffff_256x240.png
--rw-rw-r--   0 dev       (1000) dev       (1000)    30724 2022-06-27 18:44:23.000000 django-mp-cap-3.0.5/cap/static/cap/components/jquery-ui/jquery-ui.min.css
--rw-rw-r--   0 dev       (1000) dev       (1000)   253669 2022-06-27 18:44:23.000000 django-mp-cap-3.0.5/cap/static/cap/components/jquery-ui/jquery-ui.min.js
--rwxrwxr-x   0 dev       (1000) dev       (1000)     3121 2023-04-26 13:36:09.000000 django-mp-cap-3.0.5/cap/static/cap/components/jquery.cookie.js
--rw-rw-r--   0 dev       (1000) dev       (1000)    17064 2023-04-26 13:36:09.000000 django-mp-cap-3.0.5/cap/static/cap/components/jquery.form.min.js
--rw-rw-r--   0 dev       (1000) dev       (1000)    96381 2023-04-26 13:36:09.000000 django-mp-cap-3.0.5/cap/static/cap/components/jquery.min.js
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-04-26 13:38:23.000000 django-mp-cap-3.0.5/cap/static/cap/components/qtip2/
--rw-rw-r--   0 dev       (1000) dev       (1000)     9061 2022-06-27 18:44:23.000000 django-mp-cap-3.0.5/cap/static/cap/components/qtip2/jquery.qtip.min.css
--rw-rw-r--   0 dev       (1000) dev       (1000)    44253 2023-04-26 13:36:09.000000 django-mp-cap-3.0.5/cap/static/cap/components/qtip2/jquery.qtip.min.js
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-04-26 13:38:23.000000 django-mp-cap-3.0.5/cap/static/cap/css/
--rw-rw-r--   0 dev       (1000) dev       (1000)     2590 2023-04-26 13:37:51.000000 django-mp-cap-3.0.5/cap/static/cap/css/common.css
--rw-rw-r--   0 dev       (1000) dev       (1000)     1565 2023-04-26 13:36:09.000000 django-mp-cap-3.0.5/cap/static/cap/css/sidebar.css
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-04-26 13:38:23.000000 django-mp-cap-3.0.5/cap/static/cap/img/
--rw-rw-r--   0 dev       (1000) dev       (1000)     7134 2022-06-27 18:44:23.000000 django-mp-cap-3.0.5/cap/static/cap/img/favicon.ico
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-04-26 13:38:23.000000 django-mp-cap-3.0.5/cap/static/cap/js/
--rw-rw-r--   0 dev       (1000) dev       (1000)      495 2023-04-26 13:36:09.000000 django-mp-cap-3.0.5/cap/static/cap/js/sidebar.js
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-04-26 13:38:23.000000 django-mp-cap-3.0.5/cap/templates/
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-04-26 13:38:23.000000 django-mp-cap-3.0.5/cap/templates/admin/
--rw-rw-r--   0 dev       (1000) dev       (1000)     1305 2023-04-26 13:36:09.000000 django-mp-cap-3.0.5/cap/templates/admin/base.html
--rw-rw-r--   0 dev       (1000) dev       (1000)      648 2023-04-26 13:36:09.000000 django-mp-cap-3.0.5/cap/templates/admin/change_related_field_action.html
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-04-26 13:38:23.000000 django-mp-cap-3.0.5/cap/templates/admin/includes/
--rw-rw-r--   0 dev       (1000) dev       (1000)     2390 2023-04-26 13:36:09.000000 django-mp-cap-3.0.5/cap/templates/admin/includes/fieldset.html
--rw-rw-r--   0 dev       (1000) dev       (1000)      913 2023-04-26 13:36:09.000000 django-mp-cap-3.0.5/cap/templates/admin/input_filter.html
--rw-rw-r--   0 dev       (1000) dev       (1000)      311 2023-04-26 13:36:09.000000 django-mp-cap-3.0.5/cap/templates/admin/list_item_preview.html
--rw-rw-r--   0 dev       (1000) dev       (1000)      132 2023-04-26 13:36:09.000000 django-mp-cap-3.0.5/cap/translation.py
--rw-rw-r--   0 dev       (1000) dev       (1000)      361 2023-04-26 13:36:09.000000 django-mp-cap-3.0.5/cap/urls.py
--rw-rw-r--   0 dev       (1000) dev       (1000)      391 2023-04-26 13:36:09.000000 django-mp-cap-3.0.5/cap/views.py
--rw-rw-r--   0 dev       (1000) dev       (1000)      382 2023-04-26 13:36:09.000000 django-mp-cap-3.0.5/cap/widgets.py
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-04-26 13:38:23.000000 django-mp-cap-3.0.5/django_mp_cap.egg-info/
--rw-rw-r--   0 dev       (1000) dev       (1000)      324 2023-04-26 13:38:23.000000 django-mp-cap-3.0.5/django_mp_cap.egg-info/PKG-INFO
--rw-rw-r--   0 dev       (1000) dev       (1000)     4316 2023-04-26 13:38:23.000000 django-mp-cap-3.0.5/django_mp_cap.egg-info/SOURCES.txt
--rw-rw-r--   0 dev       (1000) dev       (1000)        1 2023-04-26 13:38:23.000000 django-mp-cap-3.0.5/django_mp_cap.egg-info/dependency_links.txt
--rw-rw-r--   0 dev       (1000) dev       (1000)      121 2023-04-26 13:38:23.000000 django-mp-cap-3.0.5/django_mp_cap.egg-info/requires.txt
--rw-rw-r--   0 dev       (1000) dev       (1000)        9 2023-04-26 13:38:23.000000 django-mp-cap-3.0.5/django_mp_cap.egg-info/top_level.txt
--rw-rw-r--   0 dev       (1000) dev       (1000)      121 2022-09-07 17:17:17.000000 django-mp-cap-3.0.5/requirements.txt
--rw-rw-r--   0 dev       (1000) dev       (1000)       79 2023-04-26 13:38:23.000000 django-mp-cap-3.0.5/setup.cfg
--rw-rw-r--   0 dev       (1000) dev       (1000)      532 2023-04-26 13:37:51.000000 django-mp-cap-3.0.5/setup.py
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-04-26 13:38:23.000000 django-mp-cap-3.0.5/suit/
--rw-rw-r--   0 dev       (1000) dev       (1000)       68 2022-02-21 14:06:34.000000 django-mp-cap-3.0.5/suit/__init__.py
--rw-rw-r--   0 dev       (1000) dev       (1000)     3739 2022-02-21 14:06:34.000000 django-mp-cap-3.0.5/suit/admin.py
--rw-rw-r--   0 dev       (1000) dev       (1000)     1145 2022-09-07 17:17:17.000000 django-mp-cap-3.0.5/suit/admin_filters.py
--rw-rw-r--   0 dev       (1000) dev       (1000)     3400 2022-02-21 14:06:34.000000 django-mp-cap-3.0.5/suit/apps.py
--rw-rw-r--   0 dev       (1000) dev       (1000)      131 2022-02-21 14:06:34.000000 django-mp-cap-3.0.5/suit/compat.py
--rw-rw-r--   0 dev       (1000) dev       (1000)     1840 2022-02-21 14:06:34.000000 django-mp-cap-3.0.5/suit/config.py
--rw-rw-r--   0 dev       (1000) dev       (1000)    11318 2022-09-07 17:17:17.000000 django-mp-cap-3.0.5/suit/menu.py
--rw-rw-r--   0 dev       (1000) dev       (1000)     6638 2022-02-21 14:06:34.000000 django-mp-cap-3.0.5/suit/sortables.py
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-04-26 13:38:23.000000 django-mp-cap-3.0.5/suit/static/
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-04-26 13:38:23.000000 django-mp-cap-3.0.5/suit/static/admin/
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-04-26 13:38:23.000000 django-mp-cap-3.0.5/suit/static/admin/css/
--rw-rw-r--   0 dev       (1000) dev       (1000)       74 2022-02-21 14:06:34.000000 django-mp-cap-3.0.5/suit/static/admin/css/changelists.css
--rw-rw-r--   0 dev       (1000) dev       (1000)       74 2022-02-21 14:06:34.000000 django-mp-cap-3.0.5/suit/static/admin/css/dashboard.css
--rw-rw-r--   0 dev       (1000) dev       (1000)       74 2022-02-21 14:06:34.000000 django-mp-cap-3.0.5/suit/static/admin/css/forms.css
--rw-rw-r--   0 dev       (1000) dev       (1000)       74 2022-02-21 14:06:34.000000 django-mp-cap-3.0.5/suit/static/admin/css/login.css
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-04-26 13:38:23.000000 django-mp-cap-3.0.5/suit/static/suit/
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-04-26 13:38:23.000000 django-mp-cap-3.0.5/suit/static/suit/css/
--rw-rw-r--   0 dev       (1000) dev       (1000)    31000 2022-02-21 14:06:34.000000 django-mp-cap-3.0.5/suit/static/suit/css/font-awesome.min.css
--rw-rw-r--   0 dev       (1000) dev       (1000)   524193 2022-05-14 07:12:10.000000 django-mp-cap-3.0.5/suit/static/suit/css/suit.css
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-04-26 13:38:23.000000 django-mp-cap-3.0.5/suit/static/suit/fonts/
--rw-rw-r--   0 dev       (1000) dev       (1000)   134808 2022-02-21 14:06:34.000000 django-mp-cap-3.0.5/suit/static/suit/fonts/FontAwesome.otf
--rw-rw-r--   0 dev       (1000) dev       (1000)   165742 2022-02-21 14:06:34.000000 django-mp-cap-3.0.5/suit/static/suit/fonts/fontawesome-webfont.eot
--rw-rw-r--   0 dev       (1000) dev       (1000)   444379 2022-02-21 14:06:34.000000 django-mp-cap-3.0.5/suit/static/suit/fonts/fontawesome-webfont.svg
--rw-rw-r--   0 dev       (1000) dev       (1000)   165548 2022-02-21 14:06:34.000000 django-mp-cap-3.0.5/suit/static/suit/fonts/fontawesome-webfont.ttf
--rw-rw-r--   0 dev       (1000) dev       (1000)    98024 2022-02-21 14:06:34.000000 django-mp-cap-3.0.5/suit/static/suit/fonts/fontawesome-webfont.woff
--rw-rw-r--   0 dev       (1000) dev       (1000)    77160 2022-02-21 14:06:34.000000 django-mp-cap-3.0.5/suit/static/suit/fonts/fontawesome-webfont.woff2
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-04-26 13:38:23.000000 django-mp-cap-3.0.5/suit/static/suit/js/
--rw-rw-r--   0 dev       (1000) dev       (1000)     3275 2022-02-21 14:06:34.000000 django-mp-cap-3.0.5/suit/static/suit/js/autosize.min.js
--rw-rw-r--   0 dev       (1000) dev       (1000)     7609 2022-02-21 14:06:34.000000 django-mp-cap-3.0.5/suit/static/suit/js/suit.js
--rw-rw-r--   0 dev       (1000) dev       (1000)     7635 2022-02-21 14:06:34.000000 django-mp-cap-3.0.5/suit/static/suit/js/suit.sortables.js
--rw-rw-r--   0 dev       (1000) dev       (1000)     1660 2022-02-21 14:06:34.000000 django-mp-cap-3.0.5/suit/template.py
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-04-26 13:38:23.000000 django-mp-cap-3.0.5/suit/templates/
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-04-26 13:38:23.000000 django-mp-cap-3.0.5/suit/templates/admin/
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-04-26 13:38:23.000000 django-mp-cap-3.0.5/suit/templates/admin/auth/
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-04-26 13:38:23.000000 django-mp-cap-3.0.5/suit/templates/admin/auth/user/
--rw-rw-r--   0 dev       (1000) dev       (1000)      347 2022-02-21 14:06:34.000000 django-mp-cap-3.0.5/suit/templates/admin/auth/user/add_form.html
--rw-rw-r--   0 dev       (1000) dev       (1000)     6307 2022-02-21 14:06:34.000000 django-mp-cap-3.0.5/suit/templates/admin/base.html
--rw-rw-r--   0 dev       (1000) dev       (1000)       91 2022-02-21 14:06:34.000000 django-mp-cap-3.0.5/suit/templates/admin/base_site.html
--rw-rw-r--   0 dev       (1000) dev       (1000)     2377 2022-02-21 14:06:34.000000 django-mp-cap-3.0.5/suit/templates/admin/change_form.html
--rw-rw-r--   0 dev       (1000) dev       (1000)      761 2022-02-21 14:06:34.000000 django-mp-cap-3.0.5/suit/templates/admin/change_list.html
--rw-rw-r--   0 dev       (1000) dev       (1000)     1606 2022-02-21 14:06:34.000000 django-mp-cap-3.0.5/suit/templates/admin/change_list_results.html
--rw-rw-r--   0 dev       (1000) dev       (1000)      678 2022-02-21 14:06:34.000000 django-mp-cap-3.0.5/suit/templates/admin/filter_horizontal.html
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-04-26 13:38:23.000000 django-mp-cap-3.0.5/suit/templates/admin/includes/
--rw-rw-r--   0 dev       (1000) dev       (1000)     3087 2022-05-14 13:39:06.000000 django-mp-cap-3.0.5/suit/templates/admin/includes/fieldset.html
--rw-rw-r--   0 dev       (1000) dev       (1000)     2668 2022-02-21 14:06:34.000000 django-mp-cap-3.0.5/suit/templates/admin/login.html
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-04-26 13:38:23.000000 django-mp-cap-3.0.5/suit/templates/registration/
--rw-rw-r--   0 dev       (1000) dev       (1000)     2054 2022-02-21 14:06:34.000000 django-mp-cap-3.0.5/suit/templates/registration/password_change_form.html
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-04-26 13:38:23.000000 django-mp-cap-3.0.5/suit/templates/suit/
--rw-rw-r--   0 dev       (1000) dev       (1000)      308 2022-02-21 14:06:34.000000 django-mp-cap-3.0.5/suit/templates/suit/change_form_includes.html
--rw-rw-r--   0 dev       (1000) dev       (1000)     1324 2022-02-21 14:06:34.000000 django-mp-cap-3.0.5/suit/templates/suit/menu.html
--rw-rw-r--   0 dev       (1000) dev       (1000)      944 2022-02-21 14:06:34.000000 django-mp-cap-3.0.5/suit/templates/suit/menu_item.html
--rw-rw-r--   0 dev       (1000) dev       (1000)     1660 2022-02-21 14:06:34.000000 django-mp-cap-3.0.5/suit/templates/suit/search_form.html
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-04-26 13:38:23.000000 django-mp-cap-3.0.5/suit/templatetags/
--rw-rw-r--   0 dev       (1000) dev       (1000)        0 2022-02-21 14:06:34.000000 django-mp-cap-3.0.5/suit/templatetags/__init__.py
--rw-rw-r--   0 dev       (1000) dev       (1000)     3879 2022-02-21 14:06:34.000000 django-mp-cap-3.0.5/suit/templatetags/suit_forms.py
--rw-rw-r--   0 dev       (1000) dev       (1000)     7217 2022-02-21 14:06:34.000000 django-mp-cap-3.0.5/suit/templatetags/suit_list.py
--rw-rw-r--   0 dev       (1000) dev       (1000)     2097 2022-02-21 14:06:34.000000 django-mp-cap-3.0.5/suit/templatetags/suit_menu.py
--rw-rw-r--   0 dev       (1000) dev       (1000)     1314 2022-02-21 14:06:34.000000 django-mp-cap-3.0.5/suit/templatetags/suit_tags.py
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-04-26 13:38:23.000000 django-mp-cap-3.0.5/suit/tests/
--rw-rw-r--   0 dev       (1000) dev       (1000)        0 2022-02-21 14:06:34.000000 django-mp-cap-3.0.5/suit/tests/__init__.py
--rw-rw-r--   0 dev       (1000) dev       (1000)     1307 2022-02-21 14:06:34.000000 django-mp-cap-3.0.5/suit/tests/settings.py
--rw-rw-r--   0 dev       (1000) dev       (1000)      332 2022-02-21 14:06:34.000000 django-mp-cap-3.0.5/suit/tests/test_menu.py
--rw-rw-r--   0 dev       (1000) dev       (1000)      328 2022-02-21 14:06:34.000000 django-mp-cap-3.0.5/suit/tests/test_routes.py
--rw-rw-r--   0 dev       (1000) dev       (1000)      132 2022-02-21 14:06:34.000000 django-mp-cap-3.0.5/suit/tests/urls.py
--rw-rw-r--   0 dev       (1000) dev       (1000)     3571 2022-02-21 14:06:34.000000 django-mp-cap-3.0.5/suit/widgets.py
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-07-13 14:19:09.000000 django-mp-cap-3.0.6/
+-rw-rw-r--   0 dev       (1000) dev       (1000)      746 2021-12-18 20:11:37.000000 django-mp-cap-3.0.6/LICENSE
+-rw-rw-r--   0 dev       (1000) dev       (1000)      161 2022-02-21 14:06:34.000000 django-mp-cap-3.0.6/MANIFEST.in
+-rw-rw-r--   0 dev       (1000) dev       (1000)      324 2023-07-13 14:19:09.000000 django-mp-cap-3.0.6/PKG-INFO
+-rw-rw-r--   0 dev       (1000) dev       (1000)      245 2022-02-21 14:06:34.000000 django-mp-cap-3.0.6/README.md
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-07-13 14:19:09.000000 django-mp-cap-3.0.6/cap/
+-rw-rw-r--   0 dev       (1000) dev       (1000)     1757 2023-06-05 19:27:29.000000 django-mp-cap-3.0.6/cap/__init__.py
+-rw-rw-r--   0 dev       (1000) dev       (1000)     1535 2023-06-05 19:29:22.000000 django-mp-cap-3.0.6/cap/actions.py
+-rw-rw-r--   0 dev       (1000) dev       (1000)      324 2023-06-05 19:29:22.000000 django-mp-cap-3.0.6/cap/configs.py
+-rw-rw-r--   0 dev       (1000) dev       (1000)     1183 2023-06-05 19:29:22.000000 django-mp-cap-3.0.6/cap/decorators.py
+-rw-rw-r--   0 dev       (1000) dev       (1000)     1735 2023-06-05 19:29:22.000000 django-mp-cap-3.0.6/cap/filters.py
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-07-13 14:19:09.000000 django-mp-cap-3.0.6/cap/locale/
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-07-13 14:19:09.000000 django-mp-cap-3.0.6/cap/locale/uk/
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-07-13 14:19:09.000000 django-mp-cap-3.0.6/cap/locale/uk/LC_MESSAGES/
+-rw-rw-r--   0 dev       (1000) dev       (1000)      915 2023-05-27 09:23:55.000000 django-mp-cap-3.0.6/cap/locale/uk/LC_MESSAGES/django.mo
+-rw-rw-r--   0 dev       (1000) dev       (1000)     1329 2023-06-05 19:29:22.000000 django-mp-cap-3.0.6/cap/locale/uk/LC_MESSAGES/django.po
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-07-13 14:19:09.000000 django-mp-cap-3.0.6/cap/static/
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-07-13 14:19:09.000000 django-mp-cap-3.0.6/cap/static/cap/
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-07-13 14:19:09.000000 django-mp-cap-3.0.6/cap/static/cap/components/
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-07-13 14:19:09.000000 django-mp-cap-3.0.6/cap/static/cap/components/bootstrap/
+-rw-rw-r--   0 dev       (1000) dev       (1000)   159470 2023-06-05 19:29:22.000000 django-mp-cap-3.0.6/cap/static/cap/components/bootstrap/bootstrap.min.css
+-rw-rw-r--   0 dev       (1000) dev       (1000)    59969 2023-06-05 19:29:22.000000 django-mp-cap-3.0.6/cap/static/cap/components/bootstrap/bootstrap.min.js
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-07-13 14:19:09.000000 django-mp-cap-3.0.6/cap/static/cap/components/bootstrap-tagsinput/
+-rw-rw-r--   0 dev       (1000) dev       (1000)     1508 2022-06-27 18:44:23.000000 django-mp-cap-3.0.6/cap/static/cap/components/bootstrap-tagsinput/bootstrap-tagsinput.css
+-rw-rw-r--   0 dev       (1000) dev       (1000)    22341 2023-06-05 19:29:22.000000 django-mp-cap-3.0.6/cap/static/cap/components/bootstrap-tagsinput/bootstrap-tagsinput.js
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-07-13 14:19:09.000000 django-mp-cap-3.0.6/cap/static/cap/components/bootstrap-treeview/
+-rw-rw-r--   0 dev       (1000) dev       (1000)      204 2022-06-27 18:44:23.000000 django-mp-cap-3.0.6/cap/static/cap/components/bootstrap-treeview/bootstrap-treeview.min.css
+-rw-rw-r--   0 dev       (1000) dev       (1000)    16735 2022-06-27 18:44:23.000000 django-mp-cap-3.0.6/cap/static/cap/components/bootstrap-treeview/bootstrap-treeview.min.js
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-07-13 14:19:09.000000 django-mp-cap-3.0.6/cap/static/cap/components/fancybox/
+-rw-rw-r--   0 dev       (1000) dev       (1000)    12795 2022-06-27 18:44:23.000000 django-mp-cap-3.0.6/cap/static/cap/components/fancybox/jquery.fancybox.min.css
+-rw-rw-r--   0 dev       (1000) dev       (1000)    68253 2022-06-27 18:44:23.000000 django-mp-cap-3.0.6/cap/static/cap/components/fancybox/jquery.fancybox.min.js
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-07-13 14:19:09.000000 django-mp-cap-3.0.6/cap/static/cap/components/font-awesome/
+-rw-rw-r--   0 dev       (1000) dev       (1000)    30994 2022-06-27 18:44:23.000000 django-mp-cap-3.0.6/cap/static/cap/components/font-awesome/font-awesome.min.css
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-07-13 14:19:09.000000 django-mp-cap-3.0.6/cap/static/cap/components/font-awesome/fonts/
+-rw-rw-r--   0 dev       (1000) dev       (1000)   134808 2022-06-27 18:44:23.000000 django-mp-cap-3.0.6/cap/static/cap/components/font-awesome/fonts/FontAwesome.otf
+-rw-rw-r--   0 dev       (1000) dev       (1000)   165742 2022-06-27 18:44:23.000000 django-mp-cap-3.0.6/cap/static/cap/components/font-awesome/fonts/fontawesome-webfont.eot
+-rw-rw-r--   0 dev       (1000) dev       (1000)   444379 2023-06-05 19:29:22.000000 django-mp-cap-3.0.6/cap/static/cap/components/font-awesome/fonts/fontawesome-webfont.svg
+-rw-rw-r--   0 dev       (1000) dev       (1000)   165548 2022-06-27 18:44:23.000000 django-mp-cap-3.0.6/cap/static/cap/components/font-awesome/fonts/fontawesome-webfont.ttf
+-rw-rw-r--   0 dev       (1000) dev       (1000)    98024 2022-06-27 18:44:23.000000 django-mp-cap-3.0.6/cap/static/cap/components/font-awesome/fonts/fontawesome-webfont.woff
+-rw-rw-r--   0 dev       (1000) dev       (1000)    77160 2022-06-27 18:44:23.000000 django-mp-cap-3.0.6/cap/static/cap/components/font-awesome/fonts/fontawesome-webfont.woff2
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-07-13 14:19:09.000000 django-mp-cap-3.0.6/cap/static/cap/components/jquery-ui/
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-07-13 14:19:09.000000 django-mp-cap-3.0.6/cap/static/cap/components/jquery-ui/i18n/
+-rw-rw-r--   0 dev       (1000) dev       (1000)     1157 2023-06-05 19:29:22.000000 django-mp-cap-3.0.6/cap/static/cap/components/jquery-ui/i18n/en.js
+-rw-rw-r--   0 dev       (1000) dev       (1000)     1382 2023-06-05 19:29:22.000000 django-mp-cap-3.0.6/cap/static/cap/components/jquery-ui/i18n/ru.js
+-rw-rw-r--   0 dev       (1000) dev       (1000)     1448 2023-06-05 19:29:22.000000 django-mp-cap-3.0.6/cap/static/cap/components/jquery-ui/i18n/uk.js
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-07-13 14:19:09.000000 django-mp-cap-3.0.6/cap/static/cap/components/jquery-ui/images/
+-rw-rw-r--   0 dev       (1000) dev       (1000)       86 2022-06-27 18:44:23.000000 django-mp-cap-3.0.6/cap/static/cap/components/jquery-ui/images/ui-bg_flat_0_aaaaaa_40x100.png
+-rw-rw-r--   0 dev       (1000) dev       (1000)     3266 2022-06-27 18:44:23.000000 django-mp-cap-3.0.6/cap/static/cap/components/jquery-ui/images/ui-icons_444444_256x240.png
+-rw-rw-r--   0 dev       (1000) dev       (1000)     3274 2022-06-27 18:44:23.000000 django-mp-cap-3.0.6/cap/static/cap/components/jquery-ui/images/ui-icons_555555_256x240.png
+-rw-rw-r--   0 dev       (1000) dev       (1000)     3262 2022-06-27 18:44:23.000000 django-mp-cap-3.0.6/cap/static/cap/components/jquery-ui/images/ui-icons_777620_256x240.png
+-rw-rw-r--   0 dev       (1000) dev       (1000)     3266 2022-06-27 18:44:23.000000 django-mp-cap-3.0.6/cap/static/cap/components/jquery-ui/images/ui-icons_777777_256x240.png
+-rw-rw-r--   0 dev       (1000) dev       (1000)     3262 2022-06-27 18:44:23.000000 django-mp-cap-3.0.6/cap/static/cap/components/jquery-ui/images/ui-icons_cc0000_256x240.png
+-rw-rw-r--   0 dev       (1000) dev       (1000)     3264 2022-06-27 18:44:23.000000 django-mp-cap-3.0.6/cap/static/cap/components/jquery-ui/images/ui-icons_ffffff_256x240.png
+-rw-rw-r--   0 dev       (1000) dev       (1000)    30724 2022-06-27 18:44:23.000000 django-mp-cap-3.0.6/cap/static/cap/components/jquery-ui/jquery-ui.min.css
+-rw-rw-r--   0 dev       (1000) dev       (1000)   253669 2022-06-27 18:44:23.000000 django-mp-cap-3.0.6/cap/static/cap/components/jquery-ui/jquery-ui.min.js
+-rwxrwxr-x   0 dev       (1000) dev       (1000)     3121 2023-06-05 19:29:22.000000 django-mp-cap-3.0.6/cap/static/cap/components/jquery.cookie.js
+-rw-rw-r--   0 dev       (1000) dev       (1000)    17064 2023-06-05 19:29:22.000000 django-mp-cap-3.0.6/cap/static/cap/components/jquery.form.min.js
+-rw-rw-r--   0 dev       (1000) dev       (1000)    96381 2023-06-05 19:29:22.000000 django-mp-cap-3.0.6/cap/static/cap/components/jquery.min.js
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-07-13 14:19:09.000000 django-mp-cap-3.0.6/cap/static/cap/components/qtip2/
+-rw-rw-r--   0 dev       (1000) dev       (1000)     9061 2022-06-27 18:44:23.000000 django-mp-cap-3.0.6/cap/static/cap/components/qtip2/jquery.qtip.min.css
+-rw-rw-r--   0 dev       (1000) dev       (1000)    44253 2023-06-05 19:29:22.000000 django-mp-cap-3.0.6/cap/static/cap/components/qtip2/jquery.qtip.min.js
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-07-13 14:19:09.000000 django-mp-cap-3.0.6/cap/static/cap/css/
+-rw-rw-r--   0 dev       (1000) dev       (1000)     2590 2023-06-05 19:29:22.000000 django-mp-cap-3.0.6/cap/static/cap/css/common.css
+-rw-rw-r--   0 dev       (1000) dev       (1000)     1565 2023-06-05 19:29:22.000000 django-mp-cap-3.0.6/cap/static/cap/css/sidebar.css
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-07-13 14:19:09.000000 django-mp-cap-3.0.6/cap/static/cap/img/
+-rw-rw-r--   0 dev       (1000) dev       (1000)     7134 2022-06-27 18:44:23.000000 django-mp-cap-3.0.6/cap/static/cap/img/favicon.ico
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-07-13 14:19:09.000000 django-mp-cap-3.0.6/cap/static/cap/js/
+-rw-rw-r--   0 dev       (1000) dev       (1000)      495 2023-06-05 19:29:22.000000 django-mp-cap-3.0.6/cap/static/cap/js/sidebar.js
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-07-13 14:19:09.000000 django-mp-cap-3.0.6/cap/static/suit/
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-07-13 14:19:09.000000 django-mp-cap-3.0.6/cap/static/suit/js/
+-rw-rw-r--   0 dev       (1000) dev       (1000)     7685 2023-06-13 07:02:15.000000 django-mp-cap-3.0.6/cap/static/suit/js/suit.js
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-07-13 14:19:09.000000 django-mp-cap-3.0.6/cap/templates/
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-07-13 14:19:09.000000 django-mp-cap-3.0.6/cap/templates/admin/
+-rw-rw-r--   0 dev       (1000) dev       (1000)     1305 2023-06-05 19:29:22.000000 django-mp-cap-3.0.6/cap/templates/admin/base.html
+-rw-rw-r--   0 dev       (1000) dev       (1000)      648 2023-06-05 19:29:22.000000 django-mp-cap-3.0.6/cap/templates/admin/change_related_field_action.html
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-07-13 14:19:09.000000 django-mp-cap-3.0.6/cap/templates/admin/includes/
+-rw-rw-r--   0 dev       (1000) dev       (1000)     2390 2023-06-05 19:29:22.000000 django-mp-cap-3.0.6/cap/templates/admin/includes/fieldset.html
+-rw-rw-r--   0 dev       (1000) dev       (1000)      913 2023-06-05 19:29:22.000000 django-mp-cap-3.0.6/cap/templates/admin/input_filter.html
+-rw-rw-r--   0 dev       (1000) dev       (1000)      311 2023-06-05 19:29:22.000000 django-mp-cap-3.0.6/cap/templates/admin/list_item_preview.html
+-rw-rw-r--   0 dev       (1000) dev       (1000)      132 2023-06-05 19:28:51.000000 django-mp-cap-3.0.6/cap/translation.py
+-rw-rw-r--   0 dev       (1000) dev       (1000)      361 2023-06-05 19:28:47.000000 django-mp-cap-3.0.6/cap/urls.py
+-rw-rw-r--   0 dev       (1000) dev       (1000)      391 2023-06-05 19:27:59.000000 django-mp-cap-3.0.6/cap/views.py
+-rw-rw-r--   0 dev       (1000) dev       (1000)      382 2023-06-05 19:27:47.000000 django-mp-cap-3.0.6/cap/widgets.py
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-07-13 14:19:09.000000 django-mp-cap-3.0.6/django_mp_cap.egg-info/
+-rw-rw-r--   0 dev       (1000) dev       (1000)      324 2023-07-13 14:19:09.000000 django-mp-cap-3.0.6/django_mp_cap.egg-info/PKG-INFO
+-rw-rw-r--   0 dev       (1000) dev       (1000)     4343 2023-07-13 14:19:09.000000 django-mp-cap-3.0.6/django_mp_cap.egg-info/SOURCES.txt
+-rw-rw-r--   0 dev       (1000) dev       (1000)        1 2023-07-13 14:19:09.000000 django-mp-cap-3.0.6/django_mp_cap.egg-info/dependency_links.txt
+-rw-rw-r--   0 dev       (1000) dev       (1000)      121 2023-07-13 14:19:09.000000 django-mp-cap-3.0.6/django_mp_cap.egg-info/requires.txt
+-rw-rw-r--   0 dev       (1000) dev       (1000)        9 2023-07-13 14:19:09.000000 django-mp-cap-3.0.6/django_mp_cap.egg-info/top_level.txt
+-rw-rw-r--   0 dev       (1000) dev       (1000)      121 2022-09-07 17:17:17.000000 django-mp-cap-3.0.6/requirements.txt
+-rw-rw-r--   0 dev       (1000) dev       (1000)       79 2023-07-13 14:19:09.000000 django-mp-cap-3.0.6/setup.cfg
+-rw-rw-r--   0 dev       (1000) dev       (1000)      532 2023-07-13 14:18:19.000000 django-mp-cap-3.0.6/setup.py
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-07-13 14:19:09.000000 django-mp-cap-3.0.6/suit/
+-rw-rw-r--   0 dev       (1000) dev       (1000)       68 2022-02-21 14:06:34.000000 django-mp-cap-3.0.6/suit/__init__.py
+-rw-rw-r--   0 dev       (1000) dev       (1000)     3739 2022-02-21 14:06:34.000000 django-mp-cap-3.0.6/suit/admin.py
+-rw-rw-r--   0 dev       (1000) dev       (1000)     1145 2022-09-07 17:17:17.000000 django-mp-cap-3.0.6/suit/admin_filters.py
+-rw-rw-r--   0 dev       (1000) dev       (1000)     3400 2022-02-21 14:06:34.000000 django-mp-cap-3.0.6/suit/apps.py
+-rw-rw-r--   0 dev       (1000) dev       (1000)      131 2022-02-21 14:06:34.000000 django-mp-cap-3.0.6/suit/compat.py
+-rw-rw-r--   0 dev       (1000) dev       (1000)     1840 2022-02-21 14:06:34.000000 django-mp-cap-3.0.6/suit/config.py
+-rw-rw-r--   0 dev       (1000) dev       (1000)    11318 2022-09-07 17:17:17.000000 django-mp-cap-3.0.6/suit/menu.py
+-rw-rw-r--   0 dev       (1000) dev       (1000)     6638 2022-02-21 14:06:34.000000 django-mp-cap-3.0.6/suit/sortables.py
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-07-13 14:19:09.000000 django-mp-cap-3.0.6/suit/static/
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-07-13 14:19:09.000000 django-mp-cap-3.0.6/suit/static/admin/
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-07-13 14:19:09.000000 django-mp-cap-3.0.6/suit/static/admin/css/
+-rw-rw-r--   0 dev       (1000) dev       (1000)       74 2022-02-21 14:06:34.000000 django-mp-cap-3.0.6/suit/static/admin/css/changelists.css
+-rw-rw-r--   0 dev       (1000) dev       (1000)       74 2022-02-21 14:06:34.000000 django-mp-cap-3.0.6/suit/static/admin/css/dashboard.css
+-rw-rw-r--   0 dev       (1000) dev       (1000)       74 2022-02-21 14:06:34.000000 django-mp-cap-3.0.6/suit/static/admin/css/forms.css
+-rw-rw-r--   0 dev       (1000) dev       (1000)       74 2022-02-21 14:06:34.000000 django-mp-cap-3.0.6/suit/static/admin/css/login.css
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-07-13 14:19:09.000000 django-mp-cap-3.0.6/suit/static/suit/
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-07-13 14:19:09.000000 django-mp-cap-3.0.6/suit/static/suit/css/
+-rw-rw-r--   0 dev       (1000) dev       (1000)    31000 2022-02-21 14:06:34.000000 django-mp-cap-3.0.6/suit/static/suit/css/font-awesome.min.css
+-rw-rw-r--   0 dev       (1000) dev       (1000)   524193 2022-05-14 07:12:10.000000 django-mp-cap-3.0.6/suit/static/suit/css/suit.css
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-07-13 14:19:09.000000 django-mp-cap-3.0.6/suit/static/suit/fonts/
+-rw-rw-r--   0 dev       (1000) dev       (1000)   134808 2022-02-21 14:06:34.000000 django-mp-cap-3.0.6/suit/static/suit/fonts/FontAwesome.otf
+-rw-rw-r--   0 dev       (1000) dev       (1000)   165742 2022-02-21 14:06:34.000000 django-mp-cap-3.0.6/suit/static/suit/fonts/fontawesome-webfont.eot
+-rw-rw-r--   0 dev       (1000) dev       (1000)   444379 2022-02-21 14:06:34.000000 django-mp-cap-3.0.6/suit/static/suit/fonts/fontawesome-webfont.svg
+-rw-rw-r--   0 dev       (1000) dev       (1000)   165548 2022-02-21 14:06:34.000000 django-mp-cap-3.0.6/suit/static/suit/fonts/fontawesome-webfont.ttf
+-rw-rw-r--   0 dev       (1000) dev       (1000)    98024 2022-02-21 14:06:34.000000 django-mp-cap-3.0.6/suit/static/suit/fonts/fontawesome-webfont.woff
+-rw-rw-r--   0 dev       (1000) dev       (1000)    77160 2022-02-21 14:06:34.000000 django-mp-cap-3.0.6/suit/static/suit/fonts/fontawesome-webfont.woff2
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-07-13 14:19:09.000000 django-mp-cap-3.0.6/suit/static/suit/js/
+-rw-rw-r--   0 dev       (1000) dev       (1000)     3275 2022-02-21 14:06:34.000000 django-mp-cap-3.0.6/suit/static/suit/js/autosize.min.js
+-rw-rw-r--   0 dev       (1000) dev       (1000)     7609 2022-02-21 14:06:34.000000 django-mp-cap-3.0.6/suit/static/suit/js/suit.js
+-rw-rw-r--   0 dev       (1000) dev       (1000)     7635 2022-02-21 14:06:34.000000 django-mp-cap-3.0.6/suit/static/suit/js/suit.sortables.js
+-rw-rw-r--   0 dev       (1000) dev       (1000)     1660 2022-02-21 14:06:34.000000 django-mp-cap-3.0.6/suit/template.py
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-07-13 14:19:09.000000 django-mp-cap-3.0.6/suit/templates/
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-07-13 14:19:09.000000 django-mp-cap-3.0.6/suit/templates/admin/
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-07-13 14:19:09.000000 django-mp-cap-3.0.6/suit/templates/admin/auth/
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-07-13 14:19:09.000000 django-mp-cap-3.0.6/suit/templates/admin/auth/user/
+-rw-rw-r--   0 dev       (1000) dev       (1000)      347 2022-02-21 14:06:34.000000 django-mp-cap-3.0.6/suit/templates/admin/auth/user/add_form.html
+-rw-rw-r--   0 dev       (1000) dev       (1000)     6307 2022-02-21 14:06:34.000000 django-mp-cap-3.0.6/suit/templates/admin/base.html
+-rw-rw-r--   0 dev       (1000) dev       (1000)       91 2022-02-21 14:06:34.000000 django-mp-cap-3.0.6/suit/templates/admin/base_site.html
+-rw-rw-r--   0 dev       (1000) dev       (1000)     2377 2022-02-21 14:06:34.000000 django-mp-cap-3.0.6/suit/templates/admin/change_form.html
+-rw-rw-r--   0 dev       (1000) dev       (1000)      761 2022-02-21 14:06:34.000000 django-mp-cap-3.0.6/suit/templates/admin/change_list.html
+-rw-rw-r--   0 dev       (1000) dev       (1000)     1606 2022-02-21 14:06:34.000000 django-mp-cap-3.0.6/suit/templates/admin/change_list_results.html
+-rw-rw-r--   0 dev       (1000) dev       (1000)      678 2022-02-21 14:06:34.000000 django-mp-cap-3.0.6/suit/templates/admin/filter_horizontal.html
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-07-13 14:19:09.000000 django-mp-cap-3.0.6/suit/templates/admin/includes/
+-rw-rw-r--   0 dev       (1000) dev       (1000)     3087 2022-05-14 13:39:06.000000 django-mp-cap-3.0.6/suit/templates/admin/includes/fieldset.html
+-rw-rw-r--   0 dev       (1000) dev       (1000)     2668 2022-02-21 14:06:34.000000 django-mp-cap-3.0.6/suit/templates/admin/login.html
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-07-13 14:19:09.000000 django-mp-cap-3.0.6/suit/templates/registration/
+-rw-rw-r--   0 dev       (1000) dev       (1000)     2054 2022-02-21 14:06:34.000000 django-mp-cap-3.0.6/suit/templates/registration/password_change_form.html
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-07-13 14:19:09.000000 django-mp-cap-3.0.6/suit/templates/suit/
+-rw-rw-r--   0 dev       (1000) dev       (1000)      308 2022-02-21 14:06:34.000000 django-mp-cap-3.0.6/suit/templates/suit/change_form_includes.html
+-rw-rw-r--   0 dev       (1000) dev       (1000)     1324 2022-02-21 14:06:34.000000 django-mp-cap-3.0.6/suit/templates/suit/menu.html
+-rw-rw-r--   0 dev       (1000) dev       (1000)      944 2022-02-21 14:06:34.000000 django-mp-cap-3.0.6/suit/templates/suit/menu_item.html
+-rw-rw-r--   0 dev       (1000) dev       (1000)     1660 2022-02-21 14:06:34.000000 django-mp-cap-3.0.6/suit/templates/suit/search_form.html
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-07-13 14:19:09.000000 django-mp-cap-3.0.6/suit/templatetags/
+-rw-rw-r--   0 dev       (1000) dev       (1000)        0 2022-02-21 14:06:34.000000 django-mp-cap-3.0.6/suit/templatetags/__init__.py
+-rw-rw-r--   0 dev       (1000) dev       (1000)     3879 2022-02-21 14:06:34.000000 django-mp-cap-3.0.6/suit/templatetags/suit_forms.py
+-rw-rw-r--   0 dev       (1000) dev       (1000)     7217 2022-02-21 14:06:34.000000 django-mp-cap-3.0.6/suit/templatetags/suit_list.py
+-rw-rw-r--   0 dev       (1000) dev       (1000)     2097 2022-02-21 14:06:34.000000 django-mp-cap-3.0.6/suit/templatetags/suit_menu.py
+-rw-rw-r--   0 dev       (1000) dev       (1000)     1314 2022-02-21 14:06:34.000000 django-mp-cap-3.0.6/suit/templatetags/suit_tags.py
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-07-13 14:19:09.000000 django-mp-cap-3.0.6/suit/tests/
+-rw-rw-r--   0 dev       (1000) dev       (1000)        0 2022-02-21 14:06:34.000000 django-mp-cap-3.0.6/suit/tests/__init__.py
+-rw-rw-r--   0 dev       (1000) dev       (1000)     1307 2022-02-21 14:06:34.000000 django-mp-cap-3.0.6/suit/tests/settings.py
+-rw-rw-r--   0 dev       (1000) dev       (1000)      332 2022-02-21 14:06:34.000000 django-mp-cap-3.0.6/suit/tests/test_menu.py
+-rw-rw-r--   0 dev       (1000) dev       (1000)      328 2022-02-21 14:06:34.000000 django-mp-cap-3.0.6/suit/tests/test_routes.py
+-rw-rw-r--   0 dev       (1000) dev       (1000)      132 2022-02-21 14:06:34.000000 django-mp-cap-3.0.6/suit/tests/urls.py
+-rw-rw-r--   0 dev       (1000) dev       (1000)     3571 2022-02-21 14:06:34.000000 django-mp-cap-3.0.6/suit/widgets.py
```

### Comparing `django-mp-cap-3.0.5/LICENSE` & `django-mp-cap-3.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `django-mp-cap-3.0.5/cap/__init__.py` & `django-mp-cap-3.0.6/cap/__init__.py`

 * *Files identical despite different names*

### Comparing `django-mp-cap-3.0.5/cap/actions.py` & `django-mp-cap-3.0.6/cap/actions.py`

 * *Files identical despite different names*

### Comparing `django-mp-cap-3.0.5/cap/decorators.py` & `django-mp-cap-3.0.6/cap/decorators.py`

 * *Files identical despite different names*

### Comparing `django-mp-cap-3.0.5/cap/filters.py` & `django-mp-cap-3.0.6/cap/filters.py`

 * *Files identical despite different names*

### Comparing `django-mp-cap-3.0.5/cap/locale/uk/LC_MESSAGES/django.mo` & `django-mp-cap-3.0.6/cap/locale/uk/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-mp-cap-3.0.5/cap/locale/uk/LC_MESSAGES/django.po` & `django-mp-cap-3.0.6/cap/locale/uk/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-mp-cap-3.0.5/cap/static/cap/components/bootstrap/bootstrap.min.css` & `django-mp-cap-3.0.6/cap/static/cap/components/bootstrap/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `django-mp-cap-3.0.5/cap/static/cap/components/bootstrap/bootstrap.min.js` & `django-mp-cap-3.0.6/cap/static/cap/components/bootstrap/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `django-mp-cap-3.0.5/cap/static/cap/components/bootstrap-tagsinput/bootstrap-tagsinput.css` & `django-mp-cap-3.0.6/cap/static/cap/components/bootstrap-tagsinput/bootstrap-tagsinput.css`

 * *Files identical despite different names*

### Comparing `django-mp-cap-3.0.5/cap/static/cap/components/bootstrap-tagsinput/bootstrap-tagsinput.js` & `django-mp-cap-3.0.6/cap/static/cap/components/bootstrap-tagsinput/bootstrap-tagsinput.js`

 * *Files identical despite different names*

### Comparing `django-mp-cap-3.0.5/cap/static/cap/components/bootstrap-treeview/bootstrap-treeview.min.js` & `django-mp-cap-3.0.6/cap/static/cap/components/bootstrap-treeview/bootstrap-treeview.min.js`

 * *Files identical despite different names*

### Comparing `django-mp-cap-3.0.5/cap/static/cap/components/fancybox/jquery.fancybox.min.css` & `django-mp-cap-3.0.6/cap/static/cap/components/fancybox/jquery.fancybox.min.css`

 * *Files identical despite different names*

### Comparing `django-mp-cap-3.0.5/cap/static/cap/components/fancybox/jquery.fancybox.min.js` & `django-mp-cap-3.0.6/cap/static/cap/components/fancybox/jquery.fancybox.min.js`

 * *Files identical despite different names*

### Comparing `django-mp-cap-3.0.5/cap/static/cap/components/font-awesome/font-awesome.min.css` & `django-mp-cap-3.0.6/cap/static/cap/components/font-awesome/font-awesome.min.css`

 * *Files identical despite different names*

### Comparing `django-mp-cap-3.0.5/cap/static/cap/components/font-awesome/fonts/FontAwesome.otf` & `django-mp-cap-3.0.6/cap/static/cap/components/font-awesome/fonts/FontAwesome.otf`

 * *Files identical despite different names*

### Comparing `django-mp-cap-3.0.5/cap/static/cap/components/font-awesome/fonts/fontawesome-webfont.eot` & `django-mp-cap-3.0.6/cap/static/cap/components/font-awesome/fonts/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `django-mp-cap-3.0.5/cap/static/cap/components/font-awesome/fonts/fontawesome-webfont.svg` & `django-mp-cap-3.0.6/cap/static/cap/components/font-awesome/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `django-mp-cap-3.0.5/cap/static/cap/components/font-awesome/fonts/fontawesome-webfont.ttf` & `django-mp-cap-3.0.6/cap/static/cap/components/font-awesome/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `django-mp-cap-3.0.5/cap/static/cap/components/font-awesome/fonts/fontawesome-webfont.woff` & `django-mp-cap-3.0.6/cap/static/cap/components/font-awesome/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `django-mp-cap-3.0.5/cap/static/cap/components/font-awesome/fonts/fontawesome-webfont.woff2` & `django-mp-cap-3.0.6/cap/static/cap/components/font-awesome/fonts/fontawesome-webfont.woff2`

 * *Files identical despite different names*

### Comparing `django-mp-cap-3.0.5/cap/static/cap/components/jquery-ui/i18n/en.js` & `django-mp-cap-3.0.6/cap/static/cap/components/jquery-ui/i18n/en.js`

 * *Files identical despite different names*

### Comparing `django-mp-cap-3.0.5/cap/static/cap/components/jquery-ui/i18n/ru.js` & `django-mp-cap-3.0.6/cap/static/cap/components/jquery-ui/i18n/ru.js`

 * *Files identical despite different names*

### Comparing `django-mp-cap-3.0.5/cap/static/cap/components/jquery-ui/i18n/uk.js` & `django-mp-cap-3.0.6/cap/static/cap/components/jquery-ui/i18n/uk.js`

 * *Files identical despite different names*

### Comparing `django-mp-cap-3.0.5/cap/static/cap/components/jquery-ui/images/ui-icons_444444_256x240.png` & `django-mp-cap-3.0.6/cap/static/cap/components/jquery-ui/images/ui-icons_444444_256x240.png`

 * *Files identical despite different names*

### Comparing `django-mp-cap-3.0.5/cap/static/cap/components/jquery-ui/images/ui-icons_555555_256x240.png` & `django-mp-cap-3.0.6/cap/static/cap/components/jquery-ui/images/ui-icons_555555_256x240.png`

 * *Files identical despite different names*

### Comparing `django-mp-cap-3.0.5/cap/static/cap/components/jquery-ui/images/ui-icons_777620_256x240.png` & `django-mp-cap-3.0.6/cap/static/cap/components/jquery-ui/images/ui-icons_777620_256x240.png`

 * *Files identical despite different names*

### Comparing `django-mp-cap-3.0.5/cap/static/cap/components/jquery-ui/images/ui-icons_777777_256x240.png` & `django-mp-cap-3.0.6/cap/static/cap/components/jquery-ui/images/ui-icons_777777_256x240.png`

 * *Files identical despite different names*

### Comparing `django-mp-cap-3.0.5/cap/static/cap/components/jquery-ui/images/ui-icons_cc0000_256x240.png` & `django-mp-cap-3.0.6/cap/static/cap/components/jquery-ui/images/ui-icons_cc0000_256x240.png`

 * *Files identical despite different names*

### Comparing `django-mp-cap-3.0.5/cap/static/cap/components/jquery-ui/images/ui-icons_ffffff_256x240.png` & `django-mp-cap-3.0.6/cap/static/cap/components/jquery-ui/images/ui-icons_ffffff_256x240.png`

 * *Files identical despite different names*

### Comparing `django-mp-cap-3.0.5/cap/static/cap/components/jquery-ui/jquery-ui.min.css` & `django-mp-cap-3.0.6/cap/static/cap/components/jquery-ui/jquery-ui.min.css`

 * *Files identical despite different names*

### Comparing `django-mp-cap-3.0.5/cap/static/cap/components/jquery-ui/jquery-ui.min.js` & `django-mp-cap-3.0.6/cap/static/cap/components/jquery-ui/jquery-ui.min.js`

 * *Files identical despite different names*

### Comparing `django-mp-cap-3.0.5/cap/static/cap/components/jquery.cookie.js` & `django-mp-cap-3.0.6/cap/static/cap/components/jquery.cookie.js`

 * *Files identical despite different names*

### Comparing `django-mp-cap-3.0.5/cap/static/cap/components/jquery.form.min.js` & `django-mp-cap-3.0.6/cap/static/cap/components/jquery.form.min.js`

 * *Files identical despite different names*

### Comparing `django-mp-cap-3.0.5/cap/static/cap/components/jquery.min.js` & `django-mp-cap-3.0.6/cap/static/cap/components/jquery.min.js`

 * *Files identical despite different names*

### Comparing `django-mp-cap-3.0.5/cap/static/cap/components/qtip2/jquery.qtip.min.css` & `django-mp-cap-3.0.6/cap/static/cap/components/qtip2/jquery.qtip.min.css`

 * *Files identical despite different names*

### Comparing `django-mp-cap-3.0.5/cap/static/cap/components/qtip2/jquery.qtip.min.js` & `django-mp-cap-3.0.6/cap/static/cap/components/qtip2/jquery.qtip.min.js`

 * *Files identical despite different names*

### Comparing `django-mp-cap-3.0.5/cap/static/cap/css/common.css` & `django-mp-cap-3.0.6/cap/static/cap/css/common.css`

 * *Files identical despite different names*

### Comparing `django-mp-cap-3.0.5/cap/static/cap/css/sidebar.css` & `django-mp-cap-3.0.6/cap/static/cap/css/sidebar.css`

 * *Files identical despite different names*

### Comparing `django-mp-cap-3.0.5/cap/static/cap/img/favicon.ico` & `django-mp-cap-3.0.6/cap/static/cap/img/favicon.ico`

 * *Files identical despite different names*

### Comparing `django-mp-cap-3.0.5/cap/templates/admin/base.html` & `django-mp-cap-3.0.6/cap/templates/admin/base.html`

 * *Files identical despite different names*

### Comparing `django-mp-cap-3.0.5/cap/templates/admin/change_related_field_action.html` & `django-mp-cap-3.0.6/cap/templates/admin/change_related_field_action.html`

 * *Files identical despite different names*

### Comparing `django-mp-cap-3.0.5/cap/templates/admin/includes/fieldset.html` & `django-mp-cap-3.0.6/cap/templates/admin/includes/fieldset.html`

 * *Files identical despite different names*

### Comparing `django-mp-cap-3.0.5/cap/templates/admin/input_filter.html` & `django-mp-cap-3.0.6/cap/templates/admin/input_filter.html`

 * *Files identical despite different names*

### Comparing `django-mp-cap-3.0.5/django_mp_cap.egg-info/SOURCES.txt` & `django-mp-cap-3.0.6/django_mp_cap.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -47,14 +47,15 @@
 cap/static/cap/components/jquery-ui/images/ui-icons_ffffff_256x240.png
 cap/static/cap/components/qtip2/jquery.qtip.min.css
 cap/static/cap/components/qtip2/jquery.qtip.min.js
 cap/static/cap/css/common.css
 cap/static/cap/css/sidebar.css
 cap/static/cap/img/favicon.ico
 cap/static/cap/js/sidebar.js
+cap/static/suit/js/suit.js
 cap/templates/admin/base.html
 cap/templates/admin/change_related_field_action.html
 cap/templates/admin/input_filter.html
 cap/templates/admin/list_item_preview.html
 cap/templates/admin/includes/fieldset.html
 django_mp_cap.egg-info/PKG-INFO
 django_mp_cap.egg-info/SOURCES.txt
```

### Comparing `django-mp-cap-3.0.5/setup.py` & `django-mp-cap-3.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 
 from setuptools import setup, find_packages
 
 
-version = '3.0.5'
+version = '3.0.6'
 url = 'https://github.com/pmaigutyak/mp-cap'
 
 with open('requirements.txt') as f:
     requires = f.read().splitlines()
 
 setup(
     name='django-mp-cap',
```

### Comparing `django-mp-cap-3.0.5/suit/admin.py` & `django-mp-cap-3.0.6/suit/admin.py`

 * *Files identical despite different names*

### Comparing `django-mp-cap-3.0.5/suit/admin_filters.py` & `django-mp-cap-3.0.6/suit/admin_filters.py`

 * *Files identical despite different names*

### Comparing `django-mp-cap-3.0.5/suit/apps.py` & `django-mp-cap-3.0.6/suit/apps.py`

 * *Files identical despite different names*

### Comparing `django-mp-cap-3.0.5/suit/config.py` & `django-mp-cap-3.0.6/suit/config.py`

 * *Files identical despite different names*

### Comparing `django-mp-cap-3.0.5/suit/menu.py` & `django-mp-cap-3.0.6/suit/menu.py`

 * *Files identical despite different names*

### Comparing `django-mp-cap-3.0.5/suit/sortables.py` & `django-mp-cap-3.0.6/suit/sortables.py`

 * *Files identical despite different names*

### Comparing `django-mp-cap-3.0.5/suit/static/suit/css/font-awesome.min.css` & `django-mp-cap-3.0.6/suit/static/suit/css/font-awesome.min.css`

 * *Files identical despite different names*

### Comparing `django-mp-cap-3.0.5/suit/static/suit/css/suit.css` & `django-mp-cap-3.0.6/suit/static/suit/css/suit.css`

 * *Files identical despite different names*

### Comparing `django-mp-cap-3.0.5/suit/static/suit/fonts/FontAwesome.otf` & `django-mp-cap-3.0.6/suit/static/suit/fonts/FontAwesome.otf`

 * *Files identical despite different names*

### Comparing `django-mp-cap-3.0.5/suit/static/suit/fonts/fontawesome-webfont.eot` & `django-mp-cap-3.0.6/suit/static/suit/fonts/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `django-mp-cap-3.0.5/suit/static/suit/fonts/fontawesome-webfont.svg` & `django-mp-cap-3.0.6/suit/static/suit/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `django-mp-cap-3.0.5/suit/static/suit/fonts/fontawesome-webfont.ttf` & `django-mp-cap-3.0.6/suit/static/suit/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `django-mp-cap-3.0.5/suit/static/suit/fonts/fontawesome-webfont.woff` & `django-mp-cap-3.0.6/suit/static/suit/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `django-mp-cap-3.0.5/suit/static/suit/fonts/fontawesome-webfont.woff2` & `django-mp-cap-3.0.6/suit/static/suit/fonts/fontawesome-webfont.woff2`

 * *Files identical despite different names*

### Comparing `django-mp-cap-3.0.5/suit/static/suit/js/autosize.min.js` & `django-mp-cap-3.0.6/suit/static/suit/js/autosize.min.js`

 * *Files identical despite different names*

### Comparing `django-mp-cap-3.0.5/suit/static/suit/js/suit.js` & `django-mp-cap-3.0.6/suit/static/suit/js/suit.js`

 * *Files identical despite different names*

### Comparing `django-mp-cap-3.0.5/suit/static/suit/js/suit.sortables.js` & `django-mp-cap-3.0.6/suit/static/suit/js/suit.sortables.js`

 * *Files identical despite different names*

### Comparing `django-mp-cap-3.0.5/suit/template.py` & `django-mp-cap-3.0.6/suit/template.py`

 * *Files identical despite different names*

### Comparing `django-mp-cap-3.0.5/suit/templates/admin/base.html` & `django-mp-cap-3.0.6/suit/templates/admin/base.html`

 * *Files identical despite different names*

### Comparing `django-mp-cap-3.0.5/suit/templates/admin/change_form.html` & `django-mp-cap-3.0.6/suit/templates/admin/change_form.html`

 * *Files identical despite different names*

### Comparing `django-mp-cap-3.0.5/suit/templates/admin/change_list.html` & `django-mp-cap-3.0.6/suit/templates/admin/change_list.html`

 * *Files identical despite different names*

### Comparing `django-mp-cap-3.0.5/suit/templates/admin/change_list_results.html` & `django-mp-cap-3.0.6/suit/templates/admin/change_list_results.html`

 * *Files identical despite different names*

### Comparing `django-mp-cap-3.0.5/suit/templates/admin/filter_horizontal.html` & `django-mp-cap-3.0.6/suit/templates/admin/filter_horizontal.html`

 * *Files identical despite different names*

### Comparing `django-mp-cap-3.0.5/suit/templates/admin/includes/fieldset.html` & `django-mp-cap-3.0.6/suit/templates/admin/includes/fieldset.html`

 * *Files identical despite different names*

### Comparing `django-mp-cap-3.0.5/suit/templates/admin/login.html` & `django-mp-cap-3.0.6/suit/templates/admin/login.html`

 * *Files identical despite different names*

### Comparing `django-mp-cap-3.0.5/suit/templates/registration/password_change_form.html` & `django-mp-cap-3.0.6/suit/templates/registration/password_change_form.html`

 * *Files identical despite different names*

### Comparing `django-mp-cap-3.0.5/suit/templates/suit/menu.html` & `django-mp-cap-3.0.6/suit/templates/suit/menu.html`

 * *Files identical despite different names*

### Comparing `django-mp-cap-3.0.5/suit/templates/suit/menu_item.html` & `django-mp-cap-3.0.6/suit/templates/suit/menu_item.html`

 * *Files identical despite different names*

### Comparing `django-mp-cap-3.0.5/suit/templates/suit/search_form.html` & `django-mp-cap-3.0.6/suit/templates/suit/search_form.html`

 * *Files identical despite different names*

### Comparing `django-mp-cap-3.0.5/suit/templatetags/suit_forms.py` & `django-mp-cap-3.0.6/suit/templatetags/suit_forms.py`

 * *Files identical despite different names*

### Comparing `django-mp-cap-3.0.5/suit/templatetags/suit_list.py` & `django-mp-cap-3.0.6/suit/templatetags/suit_list.py`

 * *Files identical despite different names*

### Comparing `django-mp-cap-3.0.5/suit/templatetags/suit_menu.py` & `django-mp-cap-3.0.6/suit/templatetags/suit_menu.py`

 * *Files identical despite different names*

### Comparing `django-mp-cap-3.0.5/suit/templatetags/suit_tags.py` & `django-mp-cap-3.0.6/suit/templatetags/suit_tags.py`

 * *Files identical despite different names*

### Comparing `django-mp-cap-3.0.5/suit/tests/settings.py` & `django-mp-cap-3.0.6/suit/tests/settings.py`

 * *Files identical despite different names*

### Comparing `django-mp-cap-3.0.5/suit/widgets.py` & `django-mp-cap-3.0.6/suit/widgets.py`

 * *Files identical despite different names*

