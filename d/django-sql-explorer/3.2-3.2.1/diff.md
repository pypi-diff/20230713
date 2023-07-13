# Comparing `tmp/django-sql-explorer-3.2.tar.gz` & `tmp/django-sql-explorer-3.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-sql-explorer-3.2.tar", last modified: Wed May 17 16:56:28 2023, max compression
+gzip compressed data, was "django-sql-explorer-3.2.1.tar", last modified: Thu Jul 13 02:54:26 2023, max compression
```

## Comparing `django-sql-explorer-3.2.tar` & `django-sql-explorer-3.2.1.tar`

### file list

```diff
@@ -1,133 +1,133 @@
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-05-17 16:56:28.745464 django-sql-explorer-3.2/
--rw-r--r--   0 mark       (501) staff       (20)      519 2023-02-17 15:08:27.000000 django-sql-explorer-3.2/AUTHORS
--rw-r--r--   0 mark       (501) staff       (20)     1090 2023-02-17 15:08:27.000000 django-sql-explorer-3.2/LICENSE
--rw-r--r--   0 mark       (501) staff       (20)       96 2023-02-17 15:08:27.000000 django-sql-explorer-3.2/MANIFEST.in
--rw-r--r--   0 mark       (501) staff       (20)     4278 2023-05-17 16:56:28.745560 django-sql-explorer-3.2/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)     2807 2023-05-17 16:30:54.000000 django-sql-explorer-3.2/README.rst
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-05-17 16:56:28.620928 django-sql-explorer-3.2/django_sql_explorer.egg-info/
--rw-r--r--   0 mark       (501) staff       (20)     4278 2023-05-17 16:56:28.000000 django-sql-explorer-3.2/django_sql_explorer.egg-info/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)     4068 2023-05-17 16:56:28.000000 django-sql-explorer-3.2/django_sql_explorer.egg-info/SOURCES.txt
--rw-r--r--   0 mark       (501) staff       (20)        1 2023-05-17 16:56:28.000000 django-sql-explorer-3.2/django_sql_explorer.egg-info/dependency_links.txt
--rw-r--r--   0 mark       (501) staff       (20)        1 2023-02-17 15:08:55.000000 django-sql-explorer-3.2/django_sql_explorer.egg-info/not-zip-safe
--rw-r--r--   0 mark       (501) staff       (20)      131 2023-05-17 16:56:28.000000 django-sql-explorer-3.2/django_sql_explorer.egg-info/requires.txt
--rw-r--r--   0 mark       (501) staff       (20)        9 2023-05-17 16:56:28.000000 django-sql-explorer-3.2/django_sql_explorer.egg-info/top_level.txt
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-05-17 16:56:28.626337 django-sql-explorer-3.2/explorer/
--rw-r--r--   0 mark       (501) staff       (20)      637 2023-05-17 16:25:53.000000 django-sql-explorer-3.2/explorer/__init__.py
--rw-r--r--   0 mark       (501) staff       (20)     1741 2023-02-17 15:08:27.000000 django-sql-explorer-3.2/explorer/actions.py
--rw-r--r--   0 mark       (501) staff       (20)      356 2023-02-17 15:08:27.000000 django-sql-explorer-3.2/explorer/admin.py
--rw-r--r--   0 mark       (501) staff       (20)     4276 2023-05-02 15:12:27.000000 django-sql-explorer-3.2/explorer/app_settings.py
--rw-r--r--   0 mark       (501) staff       (20)     1366 2023-02-17 15:08:27.000000 django-sql-explorer-3.2/explorer/apps.py
--rw-r--r--   0 mark       (501) staff       (20)     3289 2023-02-17 15:08:27.000000 django-sql-explorer-3.2/explorer/charts.py
--rw-r--r--   0 mark       (501) staff       (20)      754 2023-02-17 15:08:27.000000 django-sql-explorer-3.2/explorer/connections.py
--rw-r--r--   0 mark       (501) staff       (20)     3921 2023-02-17 15:08:27.000000 django-sql-explorer-3.2/explorer/exporters.py
--rw-r--r--   0 mark       (501) staff       (20)     2051 2023-02-17 15:08:27.000000 django-sql-explorer-3.2/explorer/forms.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-05-17 16:56:28.615091 django-sql-explorer-3.2/explorer/locale/
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-05-17 16:56:28.614952 django-sql-explorer-3.2/explorer/locale/ru/
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-05-17 16:56:28.627137 django-sql-explorer-3.2/explorer/locale/ru/LC_MESSAGES/
--rw-r--r--   0 mark       (501) staff       (20)     5335 2023-02-17 15:08:27.000000 django-sql-explorer-3.2/explorer/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0 mark       (501) staff       (20)    10091 2023-02-17 15:08:27.000000 django-sql-explorer-3.2/explorer/locale/ru/LC_MESSAGES/django.po
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-05-17 16:56:28.615204 django-sql-explorer-3.2/explorer/locale/zh_Hans/
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-05-17 16:56:28.627799 django-sql-explorer-3.2/explorer/locale/zh_Hans/LC_MESSAGES/
--rw-r--r--   0 mark       (501) staff       (20)     2549 2023-02-17 15:08:27.000000 django-sql-explorer-3.2/explorer/locale/zh_Hans/LC_MESSAGES/django.mo
--rw-r--r--   0 mark       (501) staff       (20)     4863 2023-02-17 15:08:27.000000 django-sql-explorer-3.2/explorer/locale/zh_Hans/LC_MESSAGES/django.po
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-05-17 16:56:28.635495 django-sql-explorer-3.2/explorer/migrations/
--rw-r--r--   0 mark       (501) staff       (20)     1905 2023-02-17 15:08:27.000000 django-sql-explorer-3.2/explorer/migrations/0001_initial.py
--rw-r--r--   0 mark       (501) staff       (20)      435 2023-02-17 15:08:27.000000 django-sql-explorer-3.2/explorer/migrations/0002_auto_20150501_1515.py
--rw-r--r--   0 mark       (501) staff       (20)      392 2023-02-17 15:08:27.000000 django-sql-explorer-3.2/explorer/migrations/0003_query_snapshot.py
--rw-r--r--   0 mark       (501) staff       (20)      345 2023-02-17 15:08:27.000000 django-sql-explorer-3.2/explorer/migrations/0004_querylog_duration.py
--rw-r--r--   0 mark       (501) staff       (20)      439 2023-02-17 15:08:27.000000 django-sql-explorer-3.2/explorer/migrations/0005_auto_20160105_2052.py
--rw-r--r--   0 mark       (501) staff       (20)      500 2023-02-17 15:08:27.000000 django-sql-explorer-3.2/explorer/migrations/0006_query_connection.py
--rw-r--r--   0 mark       (501) staff       (20)      364 2023-02-17 15:08:27.000000 django-sql-explorer-3.2/explorer/migrations/0007_querylog_connection.py
--rw-r--r--   0 mark       (501) staff       (20)      502 2023-02-17 15:08:27.000000 django-sql-explorer-3.2/explorer/migrations/0008_auto_20190308_1642.py
--rw-r--r--   0 mark       (501) staff       (20)      913 2023-02-17 15:08:27.000000 django-sql-explorer-3.2/explorer/migrations/0009_auto_20201009_0547.py
--rw-r--r--   0 mark       (501) staff       (20)      370 2023-02-17 15:08:27.000000 django-sql-explorer-3.2/explorer/migrations/0010_sql_required.py
--rw-r--r--   0 mark       (501) staff       (20)      914 2023-02-17 15:08:27.000000 django-sql-explorer-3.2/explorer/migrations/0011_query_favorites.py
--rw-r--r--   0 mark       (501) staff       (20)      971 2023-02-27 16:05:34.000000 django-sql-explorer-3.2/explorer/migrations/0012_alter_queryfavorite_query_alter_queryfavorite_user.py
--rw-r--r--   0 mark       (501) staff       (20)        0 2023-02-17 15:08:27.000000 django-sql-explorer-3.2/explorer/migrations/__init__.py
--rw-r--r--   0 mark       (501) staff       (20)    10386 2023-02-25 20:39:51.000000 django-sql-explorer-3.2/explorer/models.py
--rw-r--r--   0 mark       (501) staff       (20)      954 2023-02-17 15:08:27.000000 django-sql-explorer-3.2/explorer/permissions.py
--rw-r--r--   0 mark       (501) staff       (20)     2791 2023-02-17 15:08:27.000000 django-sql-explorer-3.2/explorer/schema.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-05-17 16:56:28.615623 django-sql-explorer-3.2/explorer/static/
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-05-17 16:56:28.616047 django-sql-explorer-3.2/explorer/static/explorer/
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-05-17 16:56:28.648122 django-sql-explorer-3.2/explorer/static/explorer/css/
--rw-r--r--   0 mark       (501) staff       (20)   121356 2023-02-17 15:08:27.000000 django-sql-explorer-3.2/explorer/static/explorer/css/bootstrap.min.css
--rw-r--r--   0 mark       (501) staff       (20)     6038 2023-02-17 15:08:27.000000 django-sql-explorer-3.2/explorer/static/explorer/css/codemirror.min.css
--rw-r--r--   0 mark       (501) staff       (20)     2541 2023-02-17 15:08:27.000000 django-sql-explorer-3.2/explorer/static/explorer/css/explorer.css
--rw-r--r--   0 mark       (501) staff       (20)     2069 2023-02-17 15:08:27.000000 django-sql-explorer-3.2/explorer/static/explorer/css/pivot.min.css
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-05-17 16:56:28.652994 django-sql-explorer-3.2/explorer/static/explorer/fonts/
--rw-r--r--   0 mark       (501) staff       (20)    20127 2023-02-17 15:08:27.000000 django-sql-explorer-3.2/explorer/static/explorer/fonts/glyphicons-halflings-regular.eot
--rw-r--r--   0 mark       (501) staff       (20)   108738 2023-02-17 15:08:27.000000 django-sql-explorer-3.2/explorer/static/explorer/fonts/glyphicons-halflings-regular.svg
--rw-r--r--   0 mark       (501) staff       (20)    45404 2023-02-17 15:08:27.000000 django-sql-explorer-3.2/explorer/static/explorer/fonts/glyphicons-halflings-regular.ttf
--rw-r--r--   0 mark       (501) staff       (20)    23424 2023-02-17 15:08:27.000000 django-sql-explorer-3.2/explorer/static/explorer/fonts/glyphicons-halflings-regular.woff
--rw-r--r--   0 mark       (501) staff       (20)    18028 2023-02-17 15:08:27.000000 django-sql-explorer-3.2/explorer/static/explorer/fonts/glyphicons-halflings-regular.woff2
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-05-17 16:56:28.723224 django-sql-explorer-3.2/explorer/static/explorer/js/
--rw-r--r--   0 mark       (501) staff       (20)    39681 2023-02-17 15:08:27.000000 django-sql-explorer-3.2/explorer/static/explorer/js/bootstrap.min.js
--rw-r--r--   0 mark       (501) staff       (20)   170285 2023-02-17 15:08:27.000000 django-sql-explorer-3.2/explorer/static/explorer/js/codemirror.min.js
--rw-r--r--   0 mark       (501) staff       (20)     3976 2023-02-17 15:08:27.000000 django-sql-explorer-3.2/explorer/static/explorer/js/comment.min.js
--rw-r--r--   0 mark       (501) staff       (20)    10073 2023-05-02 15:12:27.000000 django-sql-explorer-3.2/explorer/static/explorer/js/explorer.js
--rw-r--r--   0 mark       (501) staff       (20)      647 2023-02-17 15:08:27.000000 django-sql-explorer-3.2/explorer/static/explorer/js/favorites.js
--rw-r--r--   0 mark       (501) staff       (20)    37880 2023-02-17 15:08:27.000000 django-sql-explorer-3.2/explorer/static/explorer/js/jquery-ui.min.js
--rw-r--r--   0 mark       (501) staff       (20)     1300 2023-02-17 15:08:27.000000 django-sql-explorer-3.2/explorer/static/explorer/js/jquery.cookie.min.js
--rw-r--r--   0 mark       (501) staff       (20)    13515 2023-02-17 15:08:27.000000 django-sql-explorer-3.2/explorer/static/explorer/js/jquery.floatThead.min.js
--rw-r--r--   0 mark       (501) staff       (20)    89501 2023-02-17 15:08:27.000000 django-sql-explorer-3.2/explorer/static/explorer/js/jquery.min.js
--rw-r--r--   0 mark       (501) staff       (20)    18101 2023-02-17 15:08:27.000000 django-sql-explorer-3.2/explorer/static/explorer/js/list.min.js
--rw-r--r--   0 mark       (501) staff       (20)    28569 2023-02-17 15:08:27.000000 django-sql-explorer-3.2/explorer/static/explorer/js/pivot.min.js
--rw-r--r--   0 mark       (501) staff       (20)     1776 2023-02-17 15:08:27.000000 django-sql-explorer-3.2/explorer/static/explorer/js/query-list.js
--rw-r--r--   0 mark       (501) staff       (20)    35417 2023-02-17 15:08:27.000000 django-sql-explorer-3.2/explorer/static/explorer/js/sql.min.js
--rw-r--r--   0 mark       (501) staff       (20)    19526 2023-02-17 15:08:27.000000 django-sql-explorer-3.2/explorer/static/explorer/js/underscore-min.js
--rw-r--r--   0 mark       (501) staff       (20)   268375 2023-02-17 15:08:27.000000 django-sql-explorer-3.2/explorer/static/explorer/js/xlsx.mini.min.js
--rw-r--r--   0 mark       (501) staff       (20)     3517 2023-02-17 15:08:27.000000 django-sql-explorer-3.2/explorer/tasks.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-05-17 16:56:28.616282 django-sql-explorer-3.2/explorer/templates/
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-05-17 16:56:28.728001 django-sql-explorer-3.2/explorer/templates/explorer/
--rw-r--r--   0 mark       (501) staff       (20)     4890 2023-05-02 15:12:27.000000 django-sql-explorer-3.2/explorer/templates/explorer/base.html
--rw-r--r--   0 mark       (501) staff       (20)      531 2023-02-17 15:08:27.000000 django-sql-explorer-3.2/explorer/templates/explorer/export_buttons.html
--rw-r--r--   0 mark       (501) staff       (20)     1648 2023-02-17 15:08:27.000000 django-sql-explorer-3.2/explorer/templates/explorer/fullscreen.html
--rw-r--r--   0 mark       (501) staff       (20)      597 2023-02-25 20:39:51.000000 django-sql-explorer-3.2/explorer/templates/explorer/params.html
--rw-r--r--   0 mark       (501) staff       (20)      548 2023-02-17 15:08:27.000000 django-sql-explorer-3.2/explorer/templates/explorer/pdf_template.html
--rw-r--r--   0 mark       (501) staff       (20)     4942 2023-02-17 15:08:27.000000 django-sql-explorer-3.2/explorer/templates/explorer/play.html
--rw-r--r--   0 mark       (501) staff       (20)    16882 2023-02-17 15:08:27.000000 django-sql-explorer-3.2/explorer/templates/explorer/preview_pane.html
--rw-r--r--   0 mark       (501) staff       (20)     9962 2023-02-17 15:08:27.000000 django-sql-explorer-3.2/explorer/templates/explorer/query.html
--rw-r--r--   0 mark       (501) staff       (20)      474 2023-02-17 15:08:27.000000 django-sql-explorer-3.2/explorer/templates/explorer/query_confirm_delete.html
--rw-r--r--   0 mark       (501) staff       (20)      349 2023-02-17 15:08:27.000000 django-sql-explorer-3.2/explorer/templates/explorer/query_favorite_button.html
--rw-r--r--   0 mark       (501) staff       (20)      888 2023-02-17 15:08:27.000000 django-sql-explorer-3.2/explorer/templates/explorer/query_favorites.html
--rw-r--r--   0 mark       (501) staff       (20)     5877 2023-05-02 15:12:27.000000 django-sql-explorer-3.2/explorer/templates/explorer/query_list.html
--rw-r--r--   0 mark       (501) staff       (20)     2801 2023-02-17 15:08:27.000000 django-sql-explorer-3.2/explorer/templates/explorer/querylog_list.html
--rw-r--r--   0 mark       (501) staff       (20)     2890 2023-02-17 15:08:27.000000 django-sql-explorer-3.2/explorer/templates/explorer/schema.html
--rw-r--r--   0 mark       (501) staff       (20)      294 2023-02-17 15:08:27.000000 django-sql-explorer-3.2/explorer/templates/explorer/schema_building.html
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-05-17 16:56:28.728678 django-sql-explorer-3.2/explorer/templatetags/
--rw-r--r--   0 mark       (501) staff       (20)        0 2023-02-17 15:08:27.000000 django-sql-explorer-3.2/explorer/templatetags/__init__.py
--rw-r--r--   0 mark       (501) staff       (20)      756 2023-02-17 15:08:27.000000 django-sql-explorer-3.2/explorer/templatetags/explorer_tags.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-05-17 16:56:28.733152 django-sql-explorer-3.2/explorer/tests/
--rw-r--r--   0 mark       (501) staff       (20)        0 2023-02-17 15:08:27.000000 django-sql-explorer-3.2/explorer/tests/__init__.py
--rw-r--r--   0 mark       (501) staff       (20)      771 2023-02-17 15:08:27.000000 django-sql-explorer-3.2/explorer/tests/factories.py
--rw-r--r--   0 mark       (501) staff       (20)     1433 2023-02-17 15:08:27.000000 django-sql-explorer-3.2/explorer/tests/test_actions.py
--rw-r--r--   0 mark       (501) staff       (20)      704 2023-02-17 15:08:27.000000 django-sql-explorer-3.2/explorer/tests/test_apps.py
--rw-r--r--   0 mark       (501) staff       (20)     1144 2023-02-17 15:08:27.000000 django-sql-explorer-3.2/explorer/tests/test_csrf_cookie_name.py
--rw-r--r--   0 mark       (501) staff       (20)     4235 2023-02-17 15:08:27.000000 django-sql-explorer-3.2/explorer/tests/test_exporters.py
--rw-r--r--   0 mark       (501) staff       (20)     1047 2023-02-17 15:08:27.000000 django-sql-explorer-3.2/explorer/tests/test_forms.py
--rw-r--r--   0 mark       (501) staff       (20)     8027 2023-02-25 20:39:51.000000 django-sql-explorer-3.2/explorer/tests/test_models.py
--rw-r--r--   0 mark       (501) staff       (20)     3438 2023-02-17 15:08:27.000000 django-sql-explorer-3.2/explorer/tests/test_schema.py
--rw-r--r--   0 mark       (501) staff       (20)     3376 2023-02-17 15:08:27.000000 django-sql-explorer-3.2/explorer/tests/test_tasks.py
--rw-r--r--   0 mark       (501) staff       (20)    10103 2023-02-25 20:39:51.000000 django-sql-explorer-3.2/explorer/tests/test_utils.py
--rw-r--r--   0 mark       (501) staff       (20)    32215 2023-02-25 20:39:51.000000 django-sql-explorer-3.2/explorer/tests/test_views.py
--rw-r--r--   0 mark       (501) staff       (20)      291 2023-02-17 15:08:27.000000 django-sql-explorer-3.2/explorer/tests/urls.py
--rw-r--r--   0 mark       (501) staff       (20)     1498 2023-02-17 15:08:27.000000 django-sql-explorer-3.2/explorer/urls.py
--rw-r--r--   0 mark       (501) staff       (20)     6057 2023-05-02 15:12:27.000000 django-sql-explorer-3.2/explorer/utils.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-05-17 16:56:28.745185 django-sql-explorer-3.2/explorer/views/
--rw-r--r--   0 mark       (501) staff       (20)      873 2023-02-17 15:08:27.000000 django-sql-explorer-3.2/explorer/views/__init__.py
--rw-r--r--   0 mark       (501) staff       (20)     1626 2023-02-17 15:08:27.000000 django-sql-explorer-3.2/explorer/views/auth.py
--rw-r--r--   0 mark       (501) staff       (20)      546 2023-02-17 15:08:27.000000 django-sql-explorer-3.2/explorer/views/create.py
--rw-r--r--   0 mark       (501) staff       (20)      447 2023-02-17 15:08:27.000000 django-sql-explorer-3.2/explorer/views/delete.py
--rw-r--r--   0 mark       (501) staff       (20)      909 2023-02-17 15:08:27.000000 django-sql-explorer-3.2/explorer/views/download.py
--rw-r--r--   0 mark       (501) staff       (20)      688 2023-02-17 15:08:27.000000 django-sql-explorer-3.2/explorer/views/email.py
--rw-r--r--   0 mark       (501) staff       (20)      874 2023-02-17 15:08:27.000000 django-sql-explorer-3.2/explorer/views/export.py
--rw-r--r--   0 mark       (501) staff       (20)      285 2023-02-17 15:08:27.000000 django-sql-explorer-3.2/explorer/views/format_sql.py
--rw-r--r--   0 mark       (501) staff       (20)     5218 2023-02-17 15:08:27.000000 django-sql-explorer-3.2/explorer/views/list.py
--rw-r--r--   0 mark       (501) staff       (20)      872 2023-05-02 15:12:27.000000 django-sql-explorer-3.2/explorer/views/mixins.py
--rw-r--r--   0 mark       (501) staff       (20)     5038 2023-02-17 15:08:27.000000 django-sql-explorer-3.2/explorer/views/query.py
--rw-r--r--   0 mark       (501) staff       (20)     1636 2023-02-17 15:08:27.000000 django-sql-explorer-3.2/explorer/views/query_favorite.py
--rw-r--r--   0 mark       (501) staff       (20)     1070 2023-02-17 15:08:27.000000 django-sql-explorer-3.2/explorer/views/schema.py
--rw-r--r--   0 mark       (501) staff       (20)      476 2023-02-17 15:08:27.000000 django-sql-explorer-3.2/explorer/views/stream.py
--rw-r--r--   0 mark       (501) staff       (20)     2509 2023-02-25 20:39:51.000000 django-sql-explorer-3.2/explorer/views/utils.py
--rw-r--r--   0 mark       (501) staff       (20)      773 2023-05-17 16:56:28.760011 django-sql-explorer-3.2/setup.cfg
--rw-r--r--   0 mark       (501) staff       (20)     3406 2023-02-25 21:07:41.000000 django-sql-explorer-3.2/setup.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-07-13 02:54:26.325530 django-sql-explorer-3.2.1/
+-rw-r--r--   0 mark       (501) staff       (20)      519 2023-02-17 15:08:27.000000 django-sql-explorer-3.2.1/AUTHORS
+-rw-r--r--   0 mark       (501) staff       (20)     1090 2023-02-17 15:08:27.000000 django-sql-explorer-3.2.1/LICENSE
+-rw-r--r--   0 mark       (501) staff       (20)       96 2023-02-17 15:08:27.000000 django-sql-explorer-3.2.1/MANIFEST.in
+-rw-r--r--   0 mark       (501) staff       (20)     4280 2023-07-13 02:54:26.325599 django-sql-explorer-3.2.1/PKG-INFO
+-rw-r--r--   0 mark       (501) staff       (20)     2807 2023-05-17 16:30:54.000000 django-sql-explorer-3.2.1/README.rst
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-07-13 02:54:26.284969 django-sql-explorer-3.2.1/django_sql_explorer.egg-info/
+-rw-r--r--   0 mark       (501) staff       (20)     4280 2023-07-13 02:54:26.000000 django-sql-explorer-3.2.1/django_sql_explorer.egg-info/PKG-INFO
+-rw-r--r--   0 mark       (501) staff       (20)     4068 2023-07-13 02:54:26.000000 django-sql-explorer-3.2.1/django_sql_explorer.egg-info/SOURCES.txt
+-rw-r--r--   0 mark       (501) staff       (20)        1 2023-07-13 02:54:26.000000 django-sql-explorer-3.2.1/django_sql_explorer.egg-info/dependency_links.txt
+-rw-r--r--   0 mark       (501) staff       (20)        1 2023-07-13 02:54:26.000000 django-sql-explorer-3.2.1/django_sql_explorer.egg-info/not-zip-safe
+-rw-r--r--   0 mark       (501) staff       (20)      131 2023-07-13 02:54:26.000000 django-sql-explorer-3.2.1/django_sql_explorer.egg-info/requires.txt
+-rw-r--r--   0 mark       (501) staff       (20)        9 2023-07-13 02:54:26.000000 django-sql-explorer-3.2.1/django_sql_explorer.egg-info/top_level.txt
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-07-13 02:54:26.293692 django-sql-explorer-3.2.1/explorer/
+-rw-r--r--   0 mark       (501) staff       (20)      637 2023-07-13 02:52:10.000000 django-sql-explorer-3.2.1/explorer/__init__.py
+-rw-r--r--   0 mark       (501) staff       (20)     1741 2023-02-17 15:08:27.000000 django-sql-explorer-3.2.1/explorer/actions.py
+-rw-r--r--   0 mark       (501) staff       (20)      356 2023-02-17 15:08:27.000000 django-sql-explorer-3.2.1/explorer/admin.py
+-rw-r--r--   0 mark       (501) staff       (20)     4276 2023-05-02 15:12:27.000000 django-sql-explorer-3.2.1/explorer/app_settings.py
+-rw-r--r--   0 mark       (501) staff       (20)     1366 2023-02-17 15:08:27.000000 django-sql-explorer-3.2.1/explorer/apps.py
+-rw-r--r--   0 mark       (501) staff       (20)     3289 2023-02-17 15:08:27.000000 django-sql-explorer-3.2.1/explorer/charts.py
+-rw-r--r--   0 mark       (501) staff       (20)      754 2023-02-17 15:08:27.000000 django-sql-explorer-3.2.1/explorer/connections.py
+-rw-r--r--   0 mark       (501) staff       (20)     3921 2023-02-17 15:08:27.000000 django-sql-explorer-3.2.1/explorer/exporters.py
+-rw-r--r--   0 mark       (501) staff       (20)     2051 2023-02-17 15:08:27.000000 django-sql-explorer-3.2.1/explorer/forms.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-07-13 02:54:26.275325 django-sql-explorer-3.2.1/explorer/locale/
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-07-13 02:54:26.275192 django-sql-explorer-3.2.1/explorer/locale/ru/
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-07-13 02:54:26.294475 django-sql-explorer-3.2.1/explorer/locale/ru/LC_MESSAGES/
+-rw-r--r--   0 mark       (501) staff       (20)     5335 2023-02-17 15:08:27.000000 django-sql-explorer-3.2.1/explorer/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0 mark       (501) staff       (20)    10091 2023-02-17 15:08:27.000000 django-sql-explorer-3.2.1/explorer/locale/ru/LC_MESSAGES/django.po
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-07-13 02:54:26.275422 django-sql-explorer-3.2.1/explorer/locale/zh_Hans/
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-07-13 02:54:26.295080 django-sql-explorer-3.2.1/explorer/locale/zh_Hans/LC_MESSAGES/
+-rw-r--r--   0 mark       (501) staff       (20)     2549 2023-02-17 15:08:27.000000 django-sql-explorer-3.2.1/explorer/locale/zh_Hans/LC_MESSAGES/django.mo
+-rw-r--r--   0 mark       (501) staff       (20)     4863 2023-02-17 15:08:27.000000 django-sql-explorer-3.2.1/explorer/locale/zh_Hans/LC_MESSAGES/django.po
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-07-13 02:54:26.299006 django-sql-explorer-3.2.1/explorer/migrations/
+-rw-r--r--   0 mark       (501) staff       (20)     1905 2023-02-17 15:08:27.000000 django-sql-explorer-3.2.1/explorer/migrations/0001_initial.py
+-rw-r--r--   0 mark       (501) staff       (20)      435 2023-02-17 15:08:27.000000 django-sql-explorer-3.2.1/explorer/migrations/0002_auto_20150501_1515.py
+-rw-r--r--   0 mark       (501) staff       (20)      392 2023-02-17 15:08:27.000000 django-sql-explorer-3.2.1/explorer/migrations/0003_query_snapshot.py
+-rw-r--r--   0 mark       (501) staff       (20)      345 2023-02-17 15:08:27.000000 django-sql-explorer-3.2.1/explorer/migrations/0004_querylog_duration.py
+-rw-r--r--   0 mark       (501) staff       (20)      439 2023-02-17 15:08:27.000000 django-sql-explorer-3.2.1/explorer/migrations/0005_auto_20160105_2052.py
+-rw-r--r--   0 mark       (501) staff       (20)      500 2023-02-17 15:08:27.000000 django-sql-explorer-3.2.1/explorer/migrations/0006_query_connection.py
+-rw-r--r--   0 mark       (501) staff       (20)      364 2023-02-17 15:08:27.000000 django-sql-explorer-3.2.1/explorer/migrations/0007_querylog_connection.py
+-rw-r--r--   0 mark       (501) staff       (20)      502 2023-02-17 15:08:27.000000 django-sql-explorer-3.2.1/explorer/migrations/0008_auto_20190308_1642.py
+-rw-r--r--   0 mark       (501) staff       (20)      913 2023-02-17 15:08:27.000000 django-sql-explorer-3.2.1/explorer/migrations/0009_auto_20201009_0547.py
+-rw-r--r--   0 mark       (501) staff       (20)      370 2023-02-17 15:08:27.000000 django-sql-explorer-3.2.1/explorer/migrations/0010_sql_required.py
+-rw-r--r--   0 mark       (501) staff       (20)      914 2023-02-17 15:08:27.000000 django-sql-explorer-3.2.1/explorer/migrations/0011_query_favorites.py
+-rw-r--r--   0 mark       (501) staff       (20)      971 2023-02-27 16:05:34.000000 django-sql-explorer-3.2.1/explorer/migrations/0012_alter_queryfavorite_query_alter_queryfavorite_user.py
+-rw-r--r--   0 mark       (501) staff       (20)        0 2023-02-17 15:08:27.000000 django-sql-explorer-3.2.1/explorer/migrations/__init__.py
+-rw-r--r--   0 mark       (501) staff       (20)    10386 2023-02-25 20:39:51.000000 django-sql-explorer-3.2.1/explorer/models.py
+-rw-r--r--   0 mark       (501) staff       (20)      954 2023-02-17 15:08:27.000000 django-sql-explorer-3.2.1/explorer/permissions.py
+-rw-r--r--   0 mark       (501) staff       (20)     2791 2023-02-17 15:08:27.000000 django-sql-explorer-3.2.1/explorer/schema.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-07-13 02:54:26.275762 django-sql-explorer-3.2.1/explorer/static/
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-07-13 02:54:26.276076 django-sql-explorer-3.2.1/explorer/static/explorer/
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-07-13 02:54:26.300313 django-sql-explorer-3.2.1/explorer/static/explorer/css/
+-rw-r--r--   0 mark       (501) staff       (20)   121356 2023-02-17 15:08:27.000000 django-sql-explorer-3.2.1/explorer/static/explorer/css/bootstrap.min.css
+-rw-r--r--   0 mark       (501) staff       (20)     6038 2023-02-17 15:08:27.000000 django-sql-explorer-3.2.1/explorer/static/explorer/css/codemirror.min.css
+-rw-r--r--   0 mark       (501) staff       (20)     2541 2023-02-17 15:08:27.000000 django-sql-explorer-3.2.1/explorer/static/explorer/css/explorer.css
+-rw-r--r--   0 mark       (501) staff       (20)     2069 2023-02-17 15:08:27.000000 django-sql-explorer-3.2.1/explorer/static/explorer/css/pivot.min.css
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-07-13 02:54:26.302245 django-sql-explorer-3.2.1/explorer/static/explorer/fonts/
+-rw-r--r--   0 mark       (501) staff       (20)    20127 2023-02-17 15:08:27.000000 django-sql-explorer-3.2.1/explorer/static/explorer/fonts/glyphicons-halflings-regular.eot
+-rw-r--r--   0 mark       (501) staff       (20)   108738 2023-02-17 15:08:27.000000 django-sql-explorer-3.2.1/explorer/static/explorer/fonts/glyphicons-halflings-regular.svg
+-rw-r--r--   0 mark       (501) staff       (20)    45404 2023-02-17 15:08:27.000000 django-sql-explorer-3.2.1/explorer/static/explorer/fonts/glyphicons-halflings-regular.ttf
+-rw-r--r--   0 mark       (501) staff       (20)    23424 2023-02-17 15:08:27.000000 django-sql-explorer-3.2.1/explorer/static/explorer/fonts/glyphicons-halflings-regular.woff
+-rw-r--r--   0 mark       (501) staff       (20)    18028 2023-02-17 15:08:27.000000 django-sql-explorer-3.2.1/explorer/static/explorer/fonts/glyphicons-halflings-regular.woff2
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-07-13 02:54:26.310283 django-sql-explorer-3.2.1/explorer/static/explorer/js/
+-rw-r--r--   0 mark       (501) staff       (20)    39681 2023-02-17 15:08:27.000000 django-sql-explorer-3.2.1/explorer/static/explorer/js/bootstrap.min.js
+-rw-r--r--   0 mark       (501) staff       (20)   170285 2023-02-17 15:08:27.000000 django-sql-explorer-3.2.1/explorer/static/explorer/js/codemirror.min.js
+-rw-r--r--   0 mark       (501) staff       (20)     3976 2023-02-17 15:08:27.000000 django-sql-explorer-3.2.1/explorer/static/explorer/js/comment.min.js
+-rw-r--r--   0 mark       (501) staff       (20)    10073 2023-05-02 15:12:27.000000 django-sql-explorer-3.2.1/explorer/static/explorer/js/explorer.js
+-rw-r--r--   0 mark       (501) staff       (20)      647 2023-02-17 15:08:27.000000 django-sql-explorer-3.2.1/explorer/static/explorer/js/favorites.js
+-rw-r--r--   0 mark       (501) staff       (20)    37880 2023-02-17 15:08:27.000000 django-sql-explorer-3.2.1/explorer/static/explorer/js/jquery-ui.min.js
+-rw-r--r--   0 mark       (501) staff       (20)     1300 2023-02-17 15:08:27.000000 django-sql-explorer-3.2.1/explorer/static/explorer/js/jquery.cookie.min.js
+-rw-r--r--   0 mark       (501) staff       (20)    13515 2023-02-17 15:08:27.000000 django-sql-explorer-3.2.1/explorer/static/explorer/js/jquery.floatThead.min.js
+-rw-r--r--   0 mark       (501) staff       (20)    89501 2023-02-17 15:08:27.000000 django-sql-explorer-3.2.1/explorer/static/explorer/js/jquery.min.js
+-rw-r--r--   0 mark       (501) staff       (20)    18101 2023-02-17 15:08:27.000000 django-sql-explorer-3.2.1/explorer/static/explorer/js/list.min.js
+-rw-r--r--   0 mark       (501) staff       (20)    28569 2023-02-17 15:08:27.000000 django-sql-explorer-3.2.1/explorer/static/explorer/js/pivot.min.js
+-rw-r--r--   0 mark       (501) staff       (20)     1776 2023-02-17 15:08:27.000000 django-sql-explorer-3.2.1/explorer/static/explorer/js/query-list.js
+-rw-r--r--   0 mark       (501) staff       (20)    35417 2023-02-17 15:08:27.000000 django-sql-explorer-3.2.1/explorer/static/explorer/js/sql.min.js
+-rw-r--r--   0 mark       (501) staff       (20)    19526 2023-02-17 15:08:27.000000 django-sql-explorer-3.2.1/explorer/static/explorer/js/underscore-min.js
+-rw-r--r--   0 mark       (501) staff       (20)   268375 2023-02-17 15:08:27.000000 django-sql-explorer-3.2.1/explorer/static/explorer/js/xlsx.mini.min.js
+-rw-r--r--   0 mark       (501) staff       (20)     3517 2023-02-17 15:08:27.000000 django-sql-explorer-3.2.1/explorer/tasks.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-07-13 02:54:26.276279 django-sql-explorer-3.2.1/explorer/templates/
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-07-13 02:54:26.316151 django-sql-explorer-3.2.1/explorer/templates/explorer/
+-rw-r--r--   0 mark       (501) staff       (20)     4890 2023-05-02 15:12:27.000000 django-sql-explorer-3.2.1/explorer/templates/explorer/base.html
+-rw-r--r--   0 mark       (501) staff       (20)      531 2023-02-17 15:08:27.000000 django-sql-explorer-3.2.1/explorer/templates/explorer/export_buttons.html
+-rw-r--r--   0 mark       (501) staff       (20)     1648 2023-02-17 15:08:27.000000 django-sql-explorer-3.2.1/explorer/templates/explorer/fullscreen.html
+-rw-r--r--   0 mark       (501) staff       (20)      597 2023-02-25 20:39:51.000000 django-sql-explorer-3.2.1/explorer/templates/explorer/params.html
+-rw-r--r--   0 mark       (501) staff       (20)      548 2023-02-17 15:08:27.000000 django-sql-explorer-3.2.1/explorer/templates/explorer/pdf_template.html
+-rw-r--r--   0 mark       (501) staff       (20)     4942 2023-02-17 15:08:27.000000 django-sql-explorer-3.2.1/explorer/templates/explorer/play.html
+-rw-r--r--   0 mark       (501) staff       (20)    16882 2023-02-17 15:08:27.000000 django-sql-explorer-3.2.1/explorer/templates/explorer/preview_pane.html
+-rw-r--r--   0 mark       (501) staff       (20)     9962 2023-02-17 15:08:27.000000 django-sql-explorer-3.2.1/explorer/templates/explorer/query.html
+-rw-r--r--   0 mark       (501) staff       (20)      474 2023-02-17 15:08:27.000000 django-sql-explorer-3.2.1/explorer/templates/explorer/query_confirm_delete.html
+-rw-r--r--   0 mark       (501) staff       (20)      349 2023-02-17 15:08:27.000000 django-sql-explorer-3.2.1/explorer/templates/explorer/query_favorite_button.html
+-rw-r--r--   0 mark       (501) staff       (20)      888 2023-02-17 15:08:27.000000 django-sql-explorer-3.2.1/explorer/templates/explorer/query_favorites.html
+-rw-r--r--   0 mark       (501) staff       (20)     5877 2023-05-02 15:12:27.000000 django-sql-explorer-3.2.1/explorer/templates/explorer/query_list.html
+-rw-r--r--   0 mark       (501) staff       (20)     2801 2023-02-17 15:08:27.000000 django-sql-explorer-3.2.1/explorer/templates/explorer/querylog_list.html
+-rw-r--r--   0 mark       (501) staff       (20)     2890 2023-02-17 15:08:27.000000 django-sql-explorer-3.2.1/explorer/templates/explorer/schema.html
+-rw-r--r--   0 mark       (501) staff       (20)      294 2023-02-17 15:08:27.000000 django-sql-explorer-3.2.1/explorer/templates/explorer/schema_building.html
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-07-13 02:54:26.316683 django-sql-explorer-3.2.1/explorer/templatetags/
+-rw-r--r--   0 mark       (501) staff       (20)        0 2023-02-17 15:08:27.000000 django-sql-explorer-3.2.1/explorer/templatetags/__init__.py
+-rw-r--r--   0 mark       (501) staff       (20)      756 2023-02-17 15:08:27.000000 django-sql-explorer-3.2.1/explorer/templatetags/explorer_tags.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-07-13 02:54:26.320656 django-sql-explorer-3.2.1/explorer/tests/
+-rw-r--r--   0 mark       (501) staff       (20)        0 2023-02-17 15:08:27.000000 django-sql-explorer-3.2.1/explorer/tests/__init__.py
+-rw-r--r--   0 mark       (501) staff       (20)      771 2023-02-17 15:08:27.000000 django-sql-explorer-3.2.1/explorer/tests/factories.py
+-rw-r--r--   0 mark       (501) staff       (20)     1433 2023-02-17 15:08:27.000000 django-sql-explorer-3.2.1/explorer/tests/test_actions.py
+-rw-r--r--   0 mark       (501) staff       (20)      704 2023-02-17 15:08:27.000000 django-sql-explorer-3.2.1/explorer/tests/test_apps.py
+-rw-r--r--   0 mark       (501) staff       (20)     1144 2023-02-17 15:08:27.000000 django-sql-explorer-3.2.1/explorer/tests/test_csrf_cookie_name.py
+-rw-r--r--   0 mark       (501) staff       (20)     4235 2023-02-17 15:08:27.000000 django-sql-explorer-3.2.1/explorer/tests/test_exporters.py
+-rw-r--r--   0 mark       (501) staff       (20)     1047 2023-02-17 15:08:27.000000 django-sql-explorer-3.2.1/explorer/tests/test_forms.py
+-rw-r--r--   0 mark       (501) staff       (20)     8027 2023-02-25 20:39:51.000000 django-sql-explorer-3.2.1/explorer/tests/test_models.py
+-rw-r--r--   0 mark       (501) staff       (20)     3438 2023-02-17 15:08:27.000000 django-sql-explorer-3.2.1/explorer/tests/test_schema.py
+-rw-r--r--   0 mark       (501) staff       (20)     3376 2023-02-17 15:08:27.000000 django-sql-explorer-3.2.1/explorer/tests/test_tasks.py
+-rw-r--r--   0 mark       (501) staff       (20)    10140 2023-07-08 20:59:26.000000 django-sql-explorer-3.2.1/explorer/tests/test_utils.py
+-rw-r--r--   0 mark       (501) staff       (20)    32215 2023-02-25 20:39:51.000000 django-sql-explorer-3.2.1/explorer/tests/test_views.py
+-rw-r--r--   0 mark       (501) staff       (20)      291 2023-02-17 15:08:27.000000 django-sql-explorer-3.2.1/explorer/tests/urls.py
+-rw-r--r--   0 mark       (501) staff       (20)     1498 2023-02-17 15:08:27.000000 django-sql-explorer-3.2.1/explorer/urls.py
+-rw-r--r--   0 mark       (501) staff       (20)     6057 2023-05-02 15:12:27.000000 django-sql-explorer-3.2.1/explorer/utils.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-07-13 02:54:26.325297 django-sql-explorer-3.2.1/explorer/views/
+-rw-r--r--   0 mark       (501) staff       (20)      873 2023-02-17 15:08:27.000000 django-sql-explorer-3.2.1/explorer/views/__init__.py
+-rw-r--r--   0 mark       (501) staff       (20)     1626 2023-02-17 15:08:27.000000 django-sql-explorer-3.2.1/explorer/views/auth.py
+-rw-r--r--   0 mark       (501) staff       (20)      546 2023-02-17 15:08:27.000000 django-sql-explorer-3.2.1/explorer/views/create.py
+-rw-r--r--   0 mark       (501) staff       (20)      447 2023-02-17 15:08:27.000000 django-sql-explorer-3.2.1/explorer/views/delete.py
+-rw-r--r--   0 mark       (501) staff       (20)      909 2023-02-17 15:08:27.000000 django-sql-explorer-3.2.1/explorer/views/download.py
+-rw-r--r--   0 mark       (501) staff       (20)      688 2023-02-17 15:08:27.000000 django-sql-explorer-3.2.1/explorer/views/email.py
+-rw-r--r--   0 mark       (501) staff       (20)      874 2023-02-17 15:08:27.000000 django-sql-explorer-3.2.1/explorer/views/export.py
+-rw-r--r--   0 mark       (501) staff       (20)      285 2023-02-17 15:08:27.000000 django-sql-explorer-3.2.1/explorer/views/format_sql.py
+-rw-r--r--   0 mark       (501) staff       (20)     5218 2023-07-13 02:48:53.000000 django-sql-explorer-3.2.1/explorer/views/list.py
+-rw-r--r--   0 mark       (501) staff       (20)      872 2023-05-02 15:12:27.000000 django-sql-explorer-3.2.1/explorer/views/mixins.py
+-rw-r--r--   0 mark       (501) staff       (20)     5038 2023-02-17 15:08:27.000000 django-sql-explorer-3.2.1/explorer/views/query.py
+-rw-r--r--   0 mark       (501) staff       (20)     1636 2023-02-17 15:08:27.000000 django-sql-explorer-3.2.1/explorer/views/query_favorite.py
+-rw-r--r--   0 mark       (501) staff       (20)     1070 2023-02-17 15:08:27.000000 django-sql-explorer-3.2.1/explorer/views/schema.py
+-rw-r--r--   0 mark       (501) staff       (20)      476 2023-02-17 15:08:27.000000 django-sql-explorer-3.2.1/explorer/views/stream.py
+-rw-r--r--   0 mark       (501) staff       (20)     2509 2023-02-25 20:39:51.000000 django-sql-explorer-3.2.1/explorer/views/utils.py
+-rw-r--r--   0 mark       (501) staff       (20)      773 2023-07-13 02:54:26.325952 django-sql-explorer-3.2.1/setup.cfg
+-rw-r--r--   0 mark       (501) staff       (20)     3406 2023-02-25 21:07:41.000000 django-sql-explorer-3.2.1/setup.py
```

### Comparing `django-sql-explorer-3.2/AUTHORS` & `django-sql-explorer-3.2.1/AUTHORS`

 * *Files identical despite different names*

### Comparing `django-sql-explorer-3.2/LICENSE` & `django-sql-explorer-3.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-sql-explorer-3.2/PKG-INFO` & `django-sql-explorer-3.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-sql-explorer
-Version: 3.2
+Version: 3.2.1
 Summary: A pluggable app that allows users (admins) to execute SQL, view, and export the results.
 Home-page: https://github.com/groveco/django-sql-explorer
 Author: Chris Clark
 Author-email: chris@untrod.com
 Maintainer: Mark Walker
 Maintainer-email: theshow@gmail.com
 License: MIT
```

### Comparing `django-sql-explorer-3.2/README.rst` & `django-sql-explorer-3.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `django-sql-explorer-3.2/django_sql_explorer.egg-info/PKG-INFO` & `django-sql-explorer-3.2.1/django_sql_explorer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-sql-explorer
-Version: 3.2
+Version: 3.2.1
 Summary: A pluggable app that allows users (admins) to execute SQL, view, and export the results.
 Home-page: https://github.com/groveco/django-sql-explorer
 Author: Chris Clark
 Author-email: chris@untrod.com
 Maintainer: Mark Walker
 Maintainer-email: theshow@gmail.com
 License: MIT
```

### Comparing `django-sql-explorer-3.2/django_sql_explorer.egg-info/SOURCES.txt` & `django-sql-explorer-3.2.1/django_sql_explorer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-sql-explorer-3.2/explorer/__init__.py` & `django-sql-explorer-3.2.1/explorer/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 __version_info__ = {
     'major': 3,
     'minor': 2,
-    'patch': 0,
+    'patch': 1,
     'releaselevel': 'final',
     'serial': 0
 }
 
 
 def get_version(short=False):
     assert __version_info__['releaselevel'] in ('alpha', 'beta', 'final')
```

### Comparing `django-sql-explorer-3.2/explorer/actions.py` & `django-sql-explorer-3.2.1/explorer/actions.py`

 * *Files identical despite different names*

### Comparing `django-sql-explorer-3.2/explorer/app_settings.py` & `django-sql-explorer-3.2.1/explorer/app_settings.py`

 * *Files identical despite different names*

### Comparing `django-sql-explorer-3.2/explorer/apps.py` & `django-sql-explorer-3.2.1/explorer/apps.py`

 * *Files identical despite different names*

### Comparing `django-sql-explorer-3.2/explorer/charts.py` & `django-sql-explorer-3.2.1/explorer/charts.py`

 * *Files identical despite different names*

### Comparing `django-sql-explorer-3.2/explorer/connections.py` & `django-sql-explorer-3.2.1/explorer/connections.py`

 * *Files identical despite different names*

### Comparing `django-sql-explorer-3.2/explorer/exporters.py` & `django-sql-explorer-3.2.1/explorer/exporters.py`

 * *Files identical despite different names*

### Comparing `django-sql-explorer-3.2/explorer/forms.py` & `django-sql-explorer-3.2.1/explorer/forms.py`

 * *Files identical despite different names*

### Comparing `django-sql-explorer-3.2/explorer/locale/ru/LC_MESSAGES/django.mo` & `django-sql-explorer-3.2.1/explorer/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-sql-explorer-3.2/explorer/locale/ru/LC_MESSAGES/django.po` & `django-sql-explorer-3.2.1/explorer/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-sql-explorer-3.2/explorer/locale/zh_Hans/LC_MESSAGES/django.mo` & `django-sql-explorer-3.2.1/explorer/locale/zh_Hans/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-sql-explorer-3.2/explorer/locale/zh_Hans/LC_MESSAGES/django.po` & `django-sql-explorer-3.2.1/explorer/locale/zh_Hans/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-sql-explorer-3.2/explorer/migrations/0001_initial.py` & `django-sql-explorer-3.2.1/explorer/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-sql-explorer-3.2/explorer/migrations/0009_auto_20201009_0547.py` & `django-sql-explorer-3.2.1/explorer/migrations/0009_auto_20201009_0547.py`

 * *Files identical despite different names*

### Comparing `django-sql-explorer-3.2/explorer/migrations/0011_query_favorites.py` & `django-sql-explorer-3.2.1/explorer/migrations/0011_query_favorites.py`

 * *Files identical despite different names*

### Comparing `django-sql-explorer-3.2/explorer/migrations/0012_alter_queryfavorite_query_alter_queryfavorite_user.py` & `django-sql-explorer-3.2.1/explorer/migrations/0012_alter_queryfavorite_query_alter_queryfavorite_user.py`

 * *Files identical despite different names*

### Comparing `django-sql-explorer-3.2/explorer/models.py` & `django-sql-explorer-3.2.1/explorer/models.py`

 * *Files identical despite different names*

### Comparing `django-sql-explorer-3.2/explorer/permissions.py` & `django-sql-explorer-3.2.1/explorer/permissions.py`

 * *Files identical despite different names*

### Comparing `django-sql-explorer-3.2/explorer/schema.py` & `django-sql-explorer-3.2.1/explorer/schema.py`

 * *Files identical despite different names*

### Comparing `django-sql-explorer-3.2/explorer/static/explorer/css/bootstrap.min.css` & `django-sql-explorer-3.2.1/explorer/static/explorer/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `django-sql-explorer-3.2/explorer/static/explorer/css/codemirror.min.css` & `django-sql-explorer-3.2.1/explorer/static/explorer/css/codemirror.min.css`

 * *Files identical despite different names*

### Comparing `django-sql-explorer-3.2/explorer/static/explorer/css/explorer.css` & `django-sql-explorer-3.2.1/explorer/static/explorer/css/explorer.css`

 * *Files identical despite different names*

### Comparing `django-sql-explorer-3.2/explorer/static/explorer/css/pivot.min.css` & `django-sql-explorer-3.2.1/explorer/static/explorer/css/pivot.min.css`

 * *Files identical despite different names*

### Comparing `django-sql-explorer-3.2/explorer/static/explorer/fonts/glyphicons-halflings-regular.eot` & `django-sql-explorer-3.2.1/explorer/static/explorer/fonts/glyphicons-halflings-regular.eot`

 * *Files identical despite different names*

### Comparing `django-sql-explorer-3.2/explorer/static/explorer/fonts/glyphicons-halflings-regular.svg` & `django-sql-explorer-3.2.1/explorer/static/explorer/fonts/glyphicons-halflings-regular.svg`

 * *Files identical despite different names*

### Comparing `django-sql-explorer-3.2/explorer/static/explorer/fonts/glyphicons-halflings-regular.ttf` & `django-sql-explorer-3.2.1/explorer/static/explorer/fonts/glyphicons-halflings-regular.ttf`

 * *Files identical despite different names*

### Comparing `django-sql-explorer-3.2/explorer/static/explorer/fonts/glyphicons-halflings-regular.woff` & `django-sql-explorer-3.2.1/explorer/static/explorer/fonts/glyphicons-halflings-regular.woff`

 * *Files identical despite different names*

### Comparing `django-sql-explorer-3.2/explorer/static/explorer/fonts/glyphicons-halflings-regular.woff2` & `django-sql-explorer-3.2.1/explorer/static/explorer/fonts/glyphicons-halflings-regular.woff2`

 * *Files identical despite different names*

### Comparing `django-sql-explorer-3.2/explorer/static/explorer/js/bootstrap.min.js` & `django-sql-explorer-3.2.1/explorer/static/explorer/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `django-sql-explorer-3.2/explorer/static/explorer/js/codemirror.min.js` & `django-sql-explorer-3.2.1/explorer/static/explorer/js/codemirror.min.js`

 * *Files identical despite different names*

### Comparing `django-sql-explorer-3.2/explorer/static/explorer/js/comment.min.js` & `django-sql-explorer-3.2.1/explorer/static/explorer/js/comment.min.js`

 * *Files identical despite different names*

### Comparing `django-sql-explorer-3.2/explorer/static/explorer/js/explorer.js` & `django-sql-explorer-3.2.1/explorer/static/explorer/js/explorer.js`

 * *Files identical despite different names*

### Comparing `django-sql-explorer-3.2/explorer/static/explorer/js/favorites.js` & `django-sql-explorer-3.2.1/explorer/static/explorer/js/favorites.js`

 * *Files identical despite different names*

### Comparing `django-sql-explorer-3.2/explorer/static/explorer/js/jquery-ui.min.js` & `django-sql-explorer-3.2.1/explorer/static/explorer/js/jquery-ui.min.js`

 * *Files identical despite different names*

### Comparing `django-sql-explorer-3.2/explorer/static/explorer/js/jquery.cookie.min.js` & `django-sql-explorer-3.2.1/explorer/static/explorer/js/jquery.cookie.min.js`

 * *Files identical despite different names*

### Comparing `django-sql-explorer-3.2/explorer/static/explorer/js/jquery.floatThead.min.js` & `django-sql-explorer-3.2.1/explorer/static/explorer/js/jquery.floatThead.min.js`

 * *Files identical despite different names*

### Comparing `django-sql-explorer-3.2/explorer/static/explorer/js/jquery.min.js` & `django-sql-explorer-3.2.1/explorer/static/explorer/js/jquery.min.js`

 * *Files identical despite different names*

### Comparing `django-sql-explorer-3.2/explorer/static/explorer/js/list.min.js` & `django-sql-explorer-3.2.1/explorer/static/explorer/js/list.min.js`

 * *Files identical despite different names*

### Comparing `django-sql-explorer-3.2/explorer/static/explorer/js/pivot.min.js` & `django-sql-explorer-3.2.1/explorer/static/explorer/js/pivot.min.js`

 * *Files identical despite different names*

### Comparing `django-sql-explorer-3.2/explorer/static/explorer/js/query-list.js` & `django-sql-explorer-3.2.1/explorer/static/explorer/js/query-list.js`

 * *Files identical despite different names*

### Comparing `django-sql-explorer-3.2/explorer/static/explorer/js/sql.min.js` & `django-sql-explorer-3.2.1/explorer/static/explorer/js/sql.min.js`

 * *Files identical despite different names*

### Comparing `django-sql-explorer-3.2/explorer/static/explorer/js/underscore-min.js` & `django-sql-explorer-3.2.1/explorer/static/explorer/js/underscore-min.js`

 * *Files identical despite different names*

### Comparing `django-sql-explorer-3.2/explorer/static/explorer/js/xlsx.mini.min.js` & `django-sql-explorer-3.2.1/explorer/static/explorer/js/xlsx.mini.min.js`

 * *Files identical despite different names*

### Comparing `django-sql-explorer-3.2/explorer/tasks.py` & `django-sql-explorer-3.2.1/explorer/tasks.py`

 * *Files identical despite different names*

### Comparing `django-sql-explorer-3.2/explorer/templates/explorer/base.html` & `django-sql-explorer-3.2.1/explorer/templates/explorer/base.html`

 * *Files identical despite different names*

### Comparing `django-sql-explorer-3.2/explorer/templates/explorer/export_buttons.html` & `django-sql-explorer-3.2.1/explorer/templates/explorer/export_buttons.html`

 * *Files identical despite different names*

### Comparing `django-sql-explorer-3.2/explorer/templates/explorer/fullscreen.html` & `django-sql-explorer-3.2.1/explorer/templates/explorer/fullscreen.html`

 * *Files identical despite different names*

### Comparing `django-sql-explorer-3.2/explorer/templates/explorer/params.html` & `django-sql-explorer-3.2.1/explorer/templates/explorer/params.html`

 * *Files identical despite different names*

### Comparing `django-sql-explorer-3.2/explorer/templates/explorer/pdf_template.html` & `django-sql-explorer-3.2.1/explorer/templates/explorer/pdf_template.html`

 * *Files identical despite different names*

### Comparing `django-sql-explorer-3.2/explorer/templates/explorer/play.html` & `django-sql-explorer-3.2.1/explorer/templates/explorer/play.html`

 * *Files identical despite different names*

### Comparing `django-sql-explorer-3.2/explorer/templates/explorer/preview_pane.html` & `django-sql-explorer-3.2.1/explorer/templates/explorer/preview_pane.html`

 * *Files identical despite different names*

### Comparing `django-sql-explorer-3.2/explorer/templates/explorer/query.html` & `django-sql-explorer-3.2.1/explorer/templates/explorer/query.html`

 * *Files identical despite different names*

### Comparing `django-sql-explorer-3.2/explorer/templates/explorer/query_favorites.html` & `django-sql-explorer-3.2.1/explorer/templates/explorer/query_favorites.html`

 * *Files identical despite different names*

### Comparing `django-sql-explorer-3.2/explorer/templates/explorer/query_list.html` & `django-sql-explorer-3.2.1/explorer/templates/explorer/query_list.html`

 * *Files identical despite different names*

### Comparing `django-sql-explorer-3.2/explorer/templates/explorer/querylog_list.html` & `django-sql-explorer-3.2.1/explorer/templates/explorer/querylog_list.html`

 * *Files identical despite different names*

### Comparing `django-sql-explorer-3.2/explorer/templates/explorer/schema.html` & `django-sql-explorer-3.2.1/explorer/templates/explorer/schema.html`

 * *Files identical despite different names*

### Comparing `django-sql-explorer-3.2/explorer/templatetags/explorer_tags.py` & `django-sql-explorer-3.2.1/explorer/templatetags/explorer_tags.py`

 * *Files identical despite different names*

### Comparing `django-sql-explorer-3.2/explorer/tests/factories.py` & `django-sql-explorer-3.2.1/explorer/tests/factories.py`

 * *Files identical despite different names*

### Comparing `django-sql-explorer-3.2/explorer/tests/test_actions.py` & `django-sql-explorer-3.2.1/explorer/tests/test_actions.py`

 * *Files identical despite different names*

### Comparing `django-sql-explorer-3.2/explorer/tests/test_apps.py` & `django-sql-explorer-3.2.1/explorer/tests/test_apps.py`

 * *Files identical despite different names*

### Comparing `django-sql-explorer-3.2/explorer/tests/test_csrf_cookie_name.py` & `django-sql-explorer-3.2.1/explorer/tests/test_csrf_cookie_name.py`

 * *Files identical despite different names*

### Comparing `django-sql-explorer-3.2/explorer/tests/test_exporters.py` & `django-sql-explorer-3.2.1/explorer/tests/test_exporters.py`

 * *Files identical despite different names*

### Comparing `django-sql-explorer-3.2/explorer/tests/test_forms.py` & `django-sql-explorer-3.2.1/explorer/tests/test_forms.py`

 * *Files identical despite different names*

### Comparing `django-sql-explorer-3.2/explorer/tests/test_models.py` & `django-sql-explorer-3.2.1/explorer/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `django-sql-explorer-3.2/explorer/tests/test_schema.py` & `django-sql-explorer-3.2.1/explorer/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `django-sql-explorer-3.2/explorer/tests/test_tasks.py` & `django-sql-explorer-3.2.1/explorer/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `django-sql-explorer-3.2/explorer/tests/test_utils.py` & `django-sql-explorer-3.2.1/explorer/tests/test_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -105,15 +105,15 @@
 
     def test_dml_rollback(self):
         sql = "ROLLBACK TO SAVEPOINT my_savepoint;"
         passes, words = passes_blacklist(sql)
         self.assertFalse(passes)
 
     def test_dml_set(self):
-        sql = "SET TIME ZONE 'PST8PDT';"
+        sql = "SET PASSWORD FOR 'user-name-here' = PASSWORD('new-password');"
         passes, words = passes_blacklist(sql)
         self.assertFalse(passes)
 
     def test_dml_start(self):
         sql = "START TRANSACTION;"
         passes, words = passes_blacklist(sql)
         self.assertFalse(passes)
```

### Comparing `django-sql-explorer-3.2/explorer/tests/test_views.py` & `django-sql-explorer-3.2.1/explorer/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `django-sql-explorer-3.2/explorer/urls.py` & `django-sql-explorer-3.2.1/explorer/urls.py`

 * *Files identical despite different names*

### Comparing `django-sql-explorer-3.2/explorer/utils.py` & `django-sql-explorer-3.2.1/explorer/utils.py`

 * *Files identical despite different names*

### Comparing `django-sql-explorer-3.2/explorer/views/__init__.py` & `django-sql-explorer-3.2.1/explorer/views/__init__.py`

 * *Files identical despite different names*

### Comparing `django-sql-explorer-3.2/explorer/views/auth.py` & `django-sql-explorer-3.2.1/explorer/views/auth.py`

 * *Files identical despite different names*

### Comparing `django-sql-explorer-3.2/explorer/views/create.py` & `django-sql-explorer-3.2.1/explorer/views/create.py`

 * *Files identical despite different names*

### Comparing `django-sql-explorer-3.2/explorer/views/download.py` & `django-sql-explorer-3.2.1/explorer/views/download.py`

 * *Files identical despite different names*

### Comparing `django-sql-explorer-3.2/explorer/views/email.py` & `django-sql-explorer-3.2.1/explorer/views/email.py`

 * *Files identical despite different names*

### Comparing `django-sql-explorer-3.2/explorer/views/export.py` & `django-sql-explorer-3.2.1/explorer/views/export.py`

 * *Files identical despite different names*

### Comparing `django-sql-explorer-3.2/explorer/views/list.py` & `django-sql-explorer-3.2.1/explorer/views/list.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,15 +83,15 @@
         """
 
         dict_list = []
         rendered_headers = []
         pattern = re.compile(r'[\W_]+')
 
         headers = Counter([q.title.split(' - ')[0] for q in self.object_list])
-        query_favorites_for_user = QueryFavorite.objects.filter(user_id=self.request.user.id).values_list('query_id',
+        query_favorites_for_user = QueryFavorite.objects.filter(user_id=self.request.user.pk).values_list('query_id',
                                                                                                           flat=True)
 
         for q in self.object_list:
             model_dict = model_to_dict(q)
             header = q.title.split(' - ')[0]
             collapse_target = pattern.sub('', header)
```

### Comparing `django-sql-explorer-3.2/explorer/views/mixins.py` & `django-sql-explorer-3.2.1/explorer/views/mixins.py`

 * *Files identical despite different names*

### Comparing `django-sql-explorer-3.2/explorer/views/query.py` & `django-sql-explorer-3.2.1/explorer/views/query.py`

 * *Files identical despite different names*

### Comparing `django-sql-explorer-3.2/explorer/views/query_favorite.py` & `django-sql-explorer-3.2.1/explorer/views/query_favorite.py`

 * *Files identical despite different names*

### Comparing `django-sql-explorer-3.2/explorer/views/schema.py` & `django-sql-explorer-3.2.1/explorer/views/schema.py`

 * *Files identical despite different names*

### Comparing `django-sql-explorer-3.2/explorer/views/utils.py` & `django-sql-explorer-3.2.1/explorer/views/utils.py`

 * *Files identical despite different names*

### Comparing `django-sql-explorer-3.2/setup.cfg` & `django-sql-explorer-3.2.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `django-sql-explorer-3.2/setup.py` & `django-sql-explorer-3.2.1/setup.py`

 * *Files identical despite different names*

