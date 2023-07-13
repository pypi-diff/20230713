# Comparing `tmp/gramps-webapi-1.1.0.tar.gz` & `tmp/gramps-webapi-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gramps-webapi-1.1.0.tar", last modified: Sun Jul  9 14:22:40 2023, max compression
+gzip compressed data, was "gramps-webapi-1.1.1.tar", last modified: Thu Jul 13 08:44:47 2023, max compression
```

## Comparing `gramps-webapi-1.1.0.tar` & `gramps-webapi-1.1.1.tar`

### file list

```diff
@@ -1,164 +1,164 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 14:22:40.278103 gramps-webapi-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-07-09 14:22:35.000000 gramps-webapi-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-07-09 14:22:35.000000 gramps-webapi-1.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-07-09 14:22:40.278103 gramps-webapi-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-07-09 14:22:35.000000 gramps-webapi-1.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 14:22:40.258103 gramps-webapi-1.1.0/gramps_webapi/
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-07-09 14:22:35.000000 gramps-webapi-1.1.0/gramps_webapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5855 2023-07-09 14:22:35.000000 gramps-webapi-1.1.0/gramps_webapi/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-07-09 14:22:35.000000 gramps-webapi-1.1.0/gramps_webapi/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 14:22:40.262103 gramps-webapi-1.1.0/gramps_webapi/api/
--rw-r--r--   0 runner    (1001) docker     (123)    14023 2023-07-09 14:22:35.000000 gramps-webapi-1.1.0/gramps_webapi/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-07-09 14:22:35.000000 gramps-webapi-1.1.0/gramps_webapi/api/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-09 14:22:35.000000 gramps-webapi-1.1.0/gramps_webapi/api/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-07-09 14:22:35.000000 gramps-webapi-1.1.0/gramps_webapi/api/emails.py
--rw-r--r--   0 runner    (1001) docker     (123)    11051 2023-07-09 14:22:35.000000 gramps-webapi-1.1.0/gramps_webapi/api/export.py
--rw-r--r--   0 runner    (1001) docker     (123)     8362 2023-07-09 14:22:35.000000 gramps-webapi-1.1.0/gramps_webapi/api/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     5269 2023-07-09 14:22:35.000000 gramps-webapi-1.1.0/gramps_webapi/api/html.py
--rw-r--r--   0 runner    (1001) docker     (123)     7968 2023-07-09 14:22:35.000000 gramps-webapi-1.1.0/gramps_webapi/api/image.py
--rw-r--r--   0 runner    (1001) docker     (123)    12817 2023-07-09 14:22:35.000000 gramps-webapi-1.1.0/gramps_webapi/api/media.py
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-09 14:22:35.000000 gramps-webapi-1.1.0/gramps_webapi/api/ratelimiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     9615 2023-07-09 14:22:35.000000 gramps-webapi-1.1.0/gramps_webapi/api/report.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 14:22:40.266103 gramps-webapi-1.1.0/gramps_webapi/api/resources/
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-07-09 14:22:35.000000 gramps-webapi-1.1.0/gramps_webapi/api/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18046 2023-07-09 14:22:35.000000 gramps-webapi-1.1.0/gramps_webapi/api/resources/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-07-09 14:22:35.000000 gramps-webapi-1.1.0/gramps_webapi/api/resources/bookmarks.py
--rw-r--r--   0 runner    (1001) docker     (123)     2274 2023-07-09 14:22:35.000000 gramps-webapi-1.1.0/gramps_webapi/api/resources/citations.py
--rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-07-09 14:22:35.000000 gramps-webapi-1.1.0/gramps_webapi/api/resources/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    15215 2023-07-09 14:22:35.000000 gramps-webapi-1.1.0/gramps_webapi/api/resources/delete.py
--rw-r--r--   0 runner    (1001) docker     (123)     6036 2023-07-09 14:22:35.000000 gramps-webapi-1.1.0/gramps_webapi/api/resources/emit.py
--rw-r--r--   0 runner    (1001) docker     (123)     3937 2023-07-09 14:22:35.000000 gramps-webapi-1.1.0/gramps_webapi/api/resources/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-07-09 14:22:35.000000 gramps-webapi-1.1.0/gramps_webapi/api/resources/export_media.py
--rw-r--r--   0 runner    (1001) docker     (123)     8609 2023-07-09 14:22:35.000000 gramps-webapi-1.1.0/gramps_webapi/api/resources/exporters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-07-09 14:22:35.000000 gramps-webapi-1.1.0/gramps_webapi/api/resources/face_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)     6539 2023-07-09 14:22:35.000000 gramps-webapi-1.1.0/gramps_webapi/api/resources/facts.py
--rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-07-09 14:22:35.000000 gramps-webapi-1.1.0/gramps_webapi/api/resources/families.py
--rw-r--r--   0 runner    (1001) docker     (123)     5186 2023-07-09 14:22:35.000000 gramps-webapi-1.1.0/gramps_webapi/api/resources/file.py
--rw-r--r--   0 runner    (1001) docker     (123)    12280 2023-07-09 14:22:35.000000 gramps-webapi-1.1.0/gramps_webapi/api/resources/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-07-09 14:22:35.000000 gramps-webapi-1.1.0/gramps_webapi/api/resources/holidays.py
--rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-07-09 14:22:35.000000 gramps-webapi-1.1.0/gramps_webapi/api/resources/import_media.py
--rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-07-09 14:22:35.000000 gramps-webapi-1.1.0/gramps_webapi/api/resources/importers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3911 2023-07-09 14:22:35.000000 gramps-webapi-1.1.0/gramps_webapi/api/resources/living.py
--rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-07-09 14:22:35.000000 gramps-webapi-1.1.0/gramps_webapi/api/resources/match.py
--rw-r--r--   0 runner    (1001) docker     (123)     3553 2023-07-09 14:22:35.000000 gramps-webapi-1.1.0/gramps_webapi/api/resources/media.py
--rw-r--r--   0 runner    (1001) docker     (123)     4650 2023-07-09 14:22:35.000000 gramps-webapi-1.1.0/gramps_webapi/api/resources/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-07-09 14:22:35.000000 gramps-webapi-1.1.0/gramps_webapi/api/resources/name_formats.py
--rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-07-09 14:22:35.000000 gramps-webapi-1.1.0/gramps_webapi/api/resources/name_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     3159 2023-07-09 14:22:35.000000 gramps-webapi-1.1.0/gramps_webapi/api/resources/notes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3903 2023-07-09 14:22:35.000000 gramps-webapi-1.1.0/gramps_webapi/api/resources/objects.py
--rw-r--r--   0 runner    (1001) docker     (123)     2828 2023-07-09 14:22:35.000000 gramps-webapi-1.1.0/gramps_webapi/api/resources/people.py
--rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-07-09 14:22:35.000000 gramps-webapi-1.1.0/gramps_webapi/api/resources/places.py
--rw-r--r--   0 runner    (1001) docker     (123)     3891 2023-07-09 14:22:35.000000 gramps-webapi-1.1.0/gramps_webapi/api/resources/relations.py
--rw-r--r--   0 runner    (1001) docker     (123)     5788 2023-07-09 14:22:35.000000 gramps-webapi-1.1.0/gramps_webapi/api/resources/reports.py
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-07-09 14:22:35.000000 gramps-webapi-1.1.0/gramps_webapi/api/resources/repositories.py
--rw-r--r--   0 runner    (1001) docker     (123)     6165 2023-07-09 14:22:35.000000 gramps-webapi-1.1.0/gramps_webapi/api/resources/search.py
--rw-r--r--   0 runner    (1001) docker     (123)    11711 2023-07-09 14:22:35.000000 gramps-webapi-1.1.0/gramps_webapi/api/resources/sort.py
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-07-09 14:22:35.000000 gramps-webapi-1.1.0/gramps_webapi/api/resources/sources.py
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-07-09 14:22:35.000000 gramps-webapi-1.1.0/gramps_webapi/api/resources/tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-07-09 14:22:35.000000 gramps-webapi-1.1.0/gramps_webapi/api/resources/tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)    32597 2023-07-09 14:22:35.000000 gramps-webapi-1.1.0/gramps_webapi/api/resources/timeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     5584 2023-07-09 14:22:35.000000 gramps-webapi-1.1.0/gramps_webapi/api/resources/token.py
--rw-r--r--   0 runner    (1001) docker     (123)     5933 2023-07-09 14:22:35.000000 gramps-webapi-1.1.0/gramps_webapi/api/resources/transactions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5465 2023-07-09 14:22:35.000000 gramps-webapi-1.1.0/gramps_webapi/api/resources/translations.py
--rw-r--r--   0 runner    (1001) docker     (123)     6961 2023-07-09 14:22:35.000000 gramps-webapi-1.1.0/gramps_webapi/api/resources/trees.py
--rw-r--r--   0 runner    (1001) docker     (123)     8475 2023-07-09 14:22:35.000000 gramps-webapi-1.1.0/gramps_webapi/api/resources/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    19847 2023-07-09 14:22:35.000000 gramps-webapi-1.1.0/gramps_webapi/api/resources/user.py
--rw-r--r--   0 runner    (1001) docker     (123)    46112 2023-07-09 14:22:35.000000 gramps-webapi-1.1.0/gramps_webapi/api/resources/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     6721 2023-07-09 14:22:35.000000 gramps-webapi-1.1.0/gramps_webapi/api/s3.py
--rw-r--r--   0 runner    (1001) docker     (123)    13199 2023-07-09 14:22:35.000000 gramps-webapi-1.1.0/gramps_webapi/api/search.py
--rw-r--r--   0 runner    (1001) docker     (123)     7072 2023-07-09 14:22:35.000000 gramps-webapi-1.1.0/gramps_webapi/api/tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)    13165 2023-07-09 14:22:35.000000 gramps-webapi-1.1.0/gramps_webapi/api/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     6371 2023-07-09 14:22:35.000000 gramps-webapi-1.1.0/gramps_webapi/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 14:22:40.266103 gramps-webapi-1.1.0/gramps_webapi/auth/
--rw-r--r--   0 runner    (1001) docker     (123)    14451 2023-07-09 14:22:35.000000 gramps-webapi-1.1.0/gramps_webapi/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3311 2023-07-09 14:22:35.000000 gramps-webapi-1.1.0/gramps_webapi/auth/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-07-09 14:22:35.000000 gramps-webapi-1.1.0/gramps_webapi/auth/passwords.py
--rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-07-09 14:22:35.000000 gramps-webapi-1.1.0/gramps_webapi/auth/sql_guid.py
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-07-09 14:22:35.000000 gramps-webapi-1.1.0/gramps_webapi/celery.py
--rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-07-09 14:22:35.000000 gramps-webapi-1.1.0/gramps_webapi/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4673 2023-07-09 14:22:35.000000 gramps-webapi-1.1.0/gramps_webapi/const.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 14:22:40.270103 gramps-webapi-1.1.0/gramps_webapi/data/
--rw-r--r--   0 runner    (1001) docker     (123)   350862 2023-07-09 14:22:35.000000 gramps-webapi-1.1.0/gramps_webapi/data/apispec.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-07-09 14:22:35.000000 gramps-webapi-1.1.0/gramps_webapi/data/empty_gramps_auth.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-09 14:22:35.000000 gramps-webapi-1.1.0/gramps_webapi/data/example_gramps_auth.cfg
--rw-r--r--   0 runner    (1001) docker     (123)   930127 2023-07-09 14:22:35.000000 gramps-webapi-1.1.0/gramps_webapi/data/haarcascade_frontalface_default.xml
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-09 14:22:35.000000 gramps-webapi-1.1.0/gramps_webapi/data/test_auth.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     5510 2023-07-09 14:22:35.000000 gramps-webapi-1.1.0/gramps_webapi/dbloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     6949 2023-07-09 14:22:35.000000 gramps-webapi-1.1.0/gramps_webapi/dbmanager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 14:22:40.270103 gramps-webapi-1.1.0/gramps_webapi/static/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 14:22:35.000000 gramps-webapi-1.1.0/gramps_webapi/static/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 14:22:40.270103 gramps-webapi-1.1.0/gramps_webapi/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-09 14:22:35.000000 gramps-webapi-1.1.0/gramps_webapi/templates/confirmation.html
--rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-07-09 14:22:35.000000 gramps-webapi-1.1.0/gramps_webapi/templates/reset_password.html
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-07-09 14:22:35.000000 gramps-webapi-1.1.0/gramps_webapi/templates/reset_password_base.html
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-07-09 14:22:35.000000 gramps-webapi-1.1.0/gramps_webapi/templates/reset_password_error.html
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-07-09 14:22:35.000000 gramps-webapi-1.1.0/gramps_webapi/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 14:22:40.270103 gramps-webapi-1.1.0/gramps_webapi/util/
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-07-09 14:22:35.000000 gramps-webapi-1.1.0/gramps_webapi/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-07-09 14:22:35.000000 gramps-webapi-1.1.0/gramps_webapi/util/celery.py
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-07-09 14:22:35.000000 gramps-webapi-1.1.0/gramps_webapi/wsgi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 14:22:40.258103 gramps-webapi-1.1.0/gramps_webapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-07-09 14:22:40.000000 gramps-webapi-1.1.0/gramps_webapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5075 2023-07-09 14:22:40.000000 gramps-webapi-1.1.0/gramps_webapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 14:22:40.000000 gramps-webapi-1.1.0/gramps_webapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 14:22:40.000000 gramps-webapi-1.1.0/gramps_webapi.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-09 14:22:40.000000 gramps-webapi-1.1.0/gramps_webapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-09 14:22:40.000000 gramps-webapi-1.1.0/gramps_webapi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-09 14:22:40.278103 gramps-webapi-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-07-09 14:22:35.000000 gramps-webapi-1.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 14:22:40.270103 gramps-webapi-1.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4742 2023-07-09 14:22:35.000000 gramps-webapi-1.1.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6209 2023-07-09 14:22:35.000000 gramps-webapi-1.1.0/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-07-09 14:22:35.000000 gramps-webapi-1.1.0/tests/test_db.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 14:22:40.278103 gramps-webapi-1.1.0/tests/test_endpoints/
--rw-r--r--   0 runner    (1001) docker     (123)     3919 2023-07-09 14:22:35.000000 gramps-webapi-1.1.0/tests/test_endpoints/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13692 2023-07-09 14:22:35.000000 gramps-webapi-1.1.0/tests/test_endpoints/checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-07-09 14:22:35.000000 gramps-webapi-1.1.0/tests/test_endpoints/test_bookmarks.py
--rw-r--r--   0 runner    (1001) docker     (123)    23353 2023-07-09 14:22:35.000000 gramps-webapi-1.1.0/tests/test_endpoints/test_citations.py
--rw-r--r--   0 runner    (1001) docker     (123)     5804 2023-07-09 14:22:35.000000 gramps-webapi-1.1.0/tests/test_endpoints/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     9073 2023-07-09 14:22:35.000000 gramps-webapi-1.1.0/tests/test_endpoints/test_delete.py
--rw-r--r--   0 runner    (1001) docker     (123)    36600 2023-07-09 14:22:35.000000 gramps-webapi-1.1.0/tests/test_endpoints/test_events.py
--rw-r--r--   0 runner    (1001) docker     (123)    20530 2023-07-09 14:22:35.000000 gramps-webapi-1.1.0/tests/test_endpoints/test_exporters.py
--rw-r--r--   0 runner    (1001) docker     (123)     7353 2023-07-09 14:22:35.000000 gramps-webapi-1.1.0/tests/test_endpoints/test_facts.py
--rw-r--r--   0 runner    (1001) docker     (123)    48295 2023-07-09 14:22:35.000000 gramps-webapi-1.1.0/tests/test_endpoints/test_families.py
--rw-r--r--   0 runner    (1001) docker     (123)     9733 2023-07-09 14:22:35.000000 gramps-webapi-1.1.0/tests/test_endpoints/test_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     9350 2023-07-09 14:22:35.000000 gramps-webapi-1.1.0/tests/test_endpoints/test_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-07-09 14:22:35.000000 gramps-webapi-1.1.0/tests/test_endpoints/test_holidays.py
--rw-r--r--   0 runner    (1001) docker     (123)     5807 2023-07-09 14:22:35.000000 gramps-webapi-1.1.0/tests/test_endpoints/test_import_media.py
--rw-r--r--   0 runner    (1001) docker     (123)     7482 2023-07-09 14:22:35.000000 gramps-webapi-1.1.0/tests/test_endpoints/test_importers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5842 2023-07-09 14:22:35.000000 gramps-webapi-1.1.0/tests/test_endpoints/test_living.py
--rw-r--r--   0 runner    (1001) docker     (123)    22991 2023-07-09 14:22:35.000000 gramps-webapi-1.1.0/tests/test_endpoints/test_media.py
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-07-09 14:22:35.000000 gramps-webapi-1.1.0/tests/test_endpoints/test_media_archive.py
--rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-07-09 14:22:35.000000 gramps-webapi-1.1.0/tests/test_endpoints/test_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-07-09 14:22:35.000000 gramps-webapi-1.1.0/tests/test_endpoints/test_name_formats.py
--rw-r--r--   0 runner    (1001) docker     (123)     3889 2023-07-09 14:22:35.000000 gramps-webapi-1.1.0/tests/test_endpoints/test_name_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)    21252 2023-07-09 14:22:35.000000 gramps-webapi-1.1.0/tests/test_endpoints/test_notes.py
--rw-r--r--   0 runner    (1001) docker     (123)    67014 2023-07-09 14:22:35.000000 gramps-webapi-1.1.0/tests/test_endpoints/test_people.py
--rw-r--r--   0 runner    (1001) docker     (123)    24741 2023-07-09 14:22:35.000000 gramps-webapi-1.1.0/tests/test_endpoints/test_places.py
--rw-r--r--   0 runner    (1001) docker     (123)    28473 2023-07-09 14:22:35.000000 gramps-webapi-1.1.0/tests/test_endpoints/test_post.py
--rw-r--r--   0 runner    (1001) docker     (123)    10113 2023-07-09 14:22:35.000000 gramps-webapi-1.1.0/tests/test_endpoints/test_put.py
--rw-r--r--   0 runner    (1001) docker     (123)     7461 2023-07-09 14:22:35.000000 gramps-webapi-1.1.0/tests/test_endpoints/test_relations.py
--rw-r--r--   0 runner    (1001) docker     (123)     9101 2023-07-09 14:22:35.000000 gramps-webapi-1.1.0/tests/test_endpoints/test_reports.py
--rw-r--r--   0 runner    (1001) docker     (123)    21917 2023-07-09 14:22:35.000000 gramps-webapi-1.1.0/tests/test_endpoints/test_repositories.py
--rw-r--r--   0 runner    (1001) docker     (123)     3236 2023-07-09 14:22:35.000000 gramps-webapi-1.1.0/tests/test_endpoints/test_s3.py
--rw-r--r--   0 runner    (1001) docker     (123)    12745 2023-07-09 14:22:35.000000 gramps-webapi-1.1.0/tests/test_endpoints/test_search.py
--rw-r--r--   0 runner    (1001) docker     (123)    23669 2023-07-09 14:22:35.000000 gramps-webapi-1.1.0/tests/test_endpoints/test_sources.py
--rw-r--r--   0 runner    (1001) docker     (123)    11735 2023-07-09 14:22:35.000000 gramps-webapi-1.1.0/tests/test_endpoints/test_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-07-09 14:22:35.000000 gramps-webapi-1.1.0/tests/test_endpoints/test_tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)    23885 2023-07-09 14:22:35.000000 gramps-webapi-1.1.0/tests/test_endpoints/test_timelines.py
--rw-r--r--   0 runner    (1001) docker     (123)     8526 2023-07-09 14:22:35.000000 gramps-webapi-1.1.0/tests/test_endpoints/test_token.py
--rw-r--r--   0 runner    (1001) docker     (123)    14548 2023-07-09 14:22:35.000000 gramps-webapi-1.1.0/tests/test_endpoints/test_transactions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4981 2023-07-09 14:22:35.000000 gramps-webapi-1.1.0/tests/test_endpoints/test_translations.py
--rw-r--r--   0 runner    (1001) docker     (123)     9571 2023-07-09 14:22:35.000000 gramps-webapi-1.1.0/tests/test_endpoints/test_trees.py
--rw-r--r--   0 runner    (1001) docker     (123)     6281 2023-07-09 14:22:35.000000 gramps-webapi-1.1.0/tests/test_endpoints/test_types.py
--rw-r--r--   0 runner    (1001) docker     (123)    10209 2023-07-09 14:22:35.000000 gramps-webapi-1.1.0/tests/test_endpoints/test_upload.py
--rw-r--r--   0 runner    (1001) docker     (123)    38607 2023-07-09 14:22:35.000000 gramps-webapi-1.1.0/tests/test_endpoints/test_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-07-09 14:22:35.000000 gramps-webapi-1.1.0/tests/test_endpoints/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-07-09 14:22:35.000000 gramps-webapi-1.1.0/tests/test_init.py
--rw-r--r--   0 runner    (1001) docker     (123)     7854 2023-07-09 14:22:35.000000 gramps-webapi-1.1.0/tests/test_jwt.py
--rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-07-09 14:22:35.000000 gramps-webapi-1.1.0/tests/test_limiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-07-09 14:22:35.000000 gramps-webapi-1.1.0/tests/test_password.py
--rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-07-09 14:22:35.000000 gramps-webapi-1.1.0/tests/test_s3.py
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-07-09 14:22:35.000000 gramps-webapi-1.1.0/tests/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     6191 2023-07-09 14:22:35.000000 gramps-webapi-1.1.0/tests/test_sqlauth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-07-09 14:22:35.000000 gramps-webapi-1.1.0/tests/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:44:47.883770 gramps-webapi-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-07-13 08:44:42.000000 gramps-webapi-1.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-07-13 08:44:42.000000 gramps-webapi-1.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-07-13 08:44:47.883770 gramps-webapi-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-07-13 08:44:42.000000 gramps-webapi-1.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:44:47.863770 gramps-webapi-1.1.1/gramps_webapi/
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-07-13 08:44:42.000000 gramps-webapi-1.1.1/gramps_webapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5855 2023-07-13 08:44:42.000000 gramps-webapi-1.1.1/gramps_webapi/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-07-13 08:44:42.000000 gramps-webapi-1.1.1/gramps_webapi/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:44:47.863770 gramps-webapi-1.1.1/gramps_webapi/api/
+-rw-r--r--   0 runner    (1001) docker     (123)    14023 2023-07-13 08:44:42.000000 gramps-webapi-1.1.1/gramps_webapi/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-07-13 08:44:42.000000 gramps-webapi-1.1.1/gramps_webapi/api/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-13 08:44:42.000000 gramps-webapi-1.1.1/gramps_webapi/api/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-07-13 08:44:42.000000 gramps-webapi-1.1.1/gramps_webapi/api/emails.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11051 2023-07-13 08:44:42.000000 gramps-webapi-1.1.1/gramps_webapi/api/export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8362 2023-07-13 08:44:42.000000 gramps-webapi-1.1.1/gramps_webapi/api/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5269 2023-07-13 08:44:42.000000 gramps-webapi-1.1.1/gramps_webapi/api/html.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7968 2023-07-13 08:44:42.000000 gramps-webapi-1.1.1/gramps_webapi/api/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12817 2023-07-13 08:44:42.000000 gramps-webapi-1.1.1/gramps_webapi/api/media.py
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-13 08:44:42.000000 gramps-webapi-1.1.1/gramps_webapi/api/ratelimiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9615 2023-07-13 08:44:42.000000 gramps-webapi-1.1.1/gramps_webapi/api/report.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:44:47.871770 gramps-webapi-1.1.1/gramps_webapi/api/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-07-13 08:44:42.000000 gramps-webapi-1.1.1/gramps_webapi/api/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18046 2023-07-13 08:44:42.000000 gramps-webapi-1.1.1/gramps_webapi/api/resources/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-07-13 08:44:42.000000 gramps-webapi-1.1.1/gramps_webapi/api/resources/bookmarks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2274 2023-07-13 08:44:42.000000 gramps-webapi-1.1.1/gramps_webapi/api/resources/citations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-07-13 08:44:42.000000 gramps-webapi-1.1.1/gramps_webapi/api/resources/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15215 2023-07-13 08:44:42.000000 gramps-webapi-1.1.1/gramps_webapi/api/resources/delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6036 2023-07-13 08:44:42.000000 gramps-webapi-1.1.1/gramps_webapi/api/resources/emit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3937 2023-07-13 08:44:42.000000 gramps-webapi-1.1.1/gramps_webapi/api/resources/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-07-13 08:44:42.000000 gramps-webapi-1.1.1/gramps_webapi/api/resources/export_media.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8609 2023-07-13 08:44:42.000000 gramps-webapi-1.1.1/gramps_webapi/api/resources/exporters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-07-13 08:44:42.000000 gramps-webapi-1.1.1/gramps_webapi/api/resources/face_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6539 2023-07-13 08:44:42.000000 gramps-webapi-1.1.1/gramps_webapi/api/resources/facts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-07-13 08:44:42.000000 gramps-webapi-1.1.1/gramps_webapi/api/resources/families.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5186 2023-07-13 08:44:42.000000 gramps-webapi-1.1.1/gramps_webapi/api/resources/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12280 2023-07-13 08:44:42.000000 gramps-webapi-1.1.1/gramps_webapi/api/resources/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-07-13 08:44:42.000000 gramps-webapi-1.1.1/gramps_webapi/api/resources/holidays.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-07-13 08:44:42.000000 gramps-webapi-1.1.1/gramps_webapi/api/resources/import_media.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-07-13 08:44:42.000000 gramps-webapi-1.1.1/gramps_webapi/api/resources/importers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3911 2023-07-13 08:44:42.000000 gramps-webapi-1.1.1/gramps_webapi/api/resources/living.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-07-13 08:44:42.000000 gramps-webapi-1.1.1/gramps_webapi/api/resources/match.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3553 2023-07-13 08:44:42.000000 gramps-webapi-1.1.1/gramps_webapi/api/resources/media.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4650 2023-07-13 08:44:42.000000 gramps-webapi-1.1.1/gramps_webapi/api/resources/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-07-13 08:44:42.000000 gramps-webapi-1.1.1/gramps_webapi/api/resources/name_formats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-07-13 08:44:42.000000 gramps-webapi-1.1.1/gramps_webapi/api/resources/name_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3159 2023-07-13 08:44:42.000000 gramps-webapi-1.1.1/gramps_webapi/api/resources/notes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3992 2023-07-13 08:44:42.000000 gramps-webapi-1.1.1/gramps_webapi/api/resources/objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2828 2023-07-13 08:44:42.000000 gramps-webapi-1.1.1/gramps_webapi/api/resources/people.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-07-13 08:44:42.000000 gramps-webapi-1.1.1/gramps_webapi/api/resources/places.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3891 2023-07-13 08:44:42.000000 gramps-webapi-1.1.1/gramps_webapi/api/resources/relations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5788 2023-07-13 08:44:42.000000 gramps-webapi-1.1.1/gramps_webapi/api/resources/reports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-07-13 08:44:42.000000 gramps-webapi-1.1.1/gramps_webapi/api/resources/repositories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6165 2023-07-13 08:44:42.000000 gramps-webapi-1.1.1/gramps_webapi/api/resources/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11711 2023-07-13 08:44:42.000000 gramps-webapi-1.1.1/gramps_webapi/api/resources/sort.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-07-13 08:44:42.000000 gramps-webapi-1.1.1/gramps_webapi/api/resources/sources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-07-13 08:44:42.000000 gramps-webapi-1.1.1/gramps_webapi/api/resources/tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-07-13 08:44:42.000000 gramps-webapi-1.1.1/gramps_webapi/api/resources/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32597 2023-07-13 08:44:42.000000 gramps-webapi-1.1.1/gramps_webapi/api/resources/timeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5584 2023-07-13 08:44:42.000000 gramps-webapi-1.1.1/gramps_webapi/api/resources/token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6019 2023-07-13 08:44:42.000000 gramps-webapi-1.1.1/gramps_webapi/api/resources/transactions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5465 2023-07-13 08:44:42.000000 gramps-webapi-1.1.1/gramps_webapi/api/resources/translations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6961 2023-07-13 08:44:42.000000 gramps-webapi-1.1.1/gramps_webapi/api/resources/trees.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8475 2023-07-13 08:44:42.000000 gramps-webapi-1.1.1/gramps_webapi/api/resources/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19847 2023-07-13 08:44:42.000000 gramps-webapi-1.1.1/gramps_webapi/api/resources/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46112 2023-07-13 08:44:42.000000 gramps-webapi-1.1.1/gramps_webapi/api/resources/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6721 2023-07-13 08:44:42.000000 gramps-webapi-1.1.1/gramps_webapi/api/s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13199 2023-07-13 08:44:42.000000 gramps-webapi-1.1.1/gramps_webapi/api/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7064 2023-07-13 08:44:42.000000 gramps-webapi-1.1.1/gramps_webapi/api/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13165 2023-07-13 08:44:42.000000 gramps-webapi-1.1.1/gramps_webapi/api/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6376 2023-07-13 08:44:42.000000 gramps-webapi-1.1.1/gramps_webapi/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:44:47.871770 gramps-webapi-1.1.1/gramps_webapi/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)    14451 2023-07-13 08:44:42.000000 gramps-webapi-1.1.1/gramps_webapi/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3311 2023-07-13 08:44:42.000000 gramps-webapi-1.1.1/gramps_webapi/auth/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-07-13 08:44:42.000000 gramps-webapi-1.1.1/gramps_webapi/auth/passwords.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-07-13 08:44:42.000000 gramps-webapi-1.1.1/gramps_webapi/auth/sql_guid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-07-13 08:44:42.000000 gramps-webapi-1.1.1/gramps_webapi/celery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-07-13 08:44:42.000000 gramps-webapi-1.1.1/gramps_webapi/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4673 2023-07-13 08:44:42.000000 gramps-webapi-1.1.1/gramps_webapi/const.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:44:47.875770 gramps-webapi-1.1.1/gramps_webapi/data/
+-rw-r--r--   0 runner    (1001) docker     (123)   350862 2023-07-13 08:44:42.000000 gramps-webapi-1.1.1/gramps_webapi/data/apispec.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-07-13 08:44:42.000000 gramps-webapi-1.1.1/gramps_webapi/data/empty_gramps_auth.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-13 08:44:42.000000 gramps-webapi-1.1.1/gramps_webapi/data/example_gramps_auth.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)   930127 2023-07-13 08:44:42.000000 gramps-webapi-1.1.1/gramps_webapi/data/haarcascade_frontalface_default.xml
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-13 08:44:42.000000 gramps-webapi-1.1.1/gramps_webapi/data/test_auth.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     5510 2023-07-13 08:44:42.000000 gramps-webapi-1.1.1/gramps_webapi/dbloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6949 2023-07-13 08:44:42.000000 gramps-webapi-1.1.1/gramps_webapi/dbmanager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:44:47.875770 gramps-webapi-1.1.1/gramps_webapi/static/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 08:44:42.000000 gramps-webapi-1.1.1/gramps_webapi/static/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:44:47.875770 gramps-webapi-1.1.1/gramps_webapi/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-13 08:44:42.000000 gramps-webapi-1.1.1/gramps_webapi/templates/confirmation.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-07-13 08:44:42.000000 gramps-webapi-1.1.1/gramps_webapi/templates/reset_password.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-07-13 08:44:42.000000 gramps-webapi-1.1.1/gramps_webapi/templates/reset_password_base.html
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-07-13 08:44:42.000000 gramps-webapi-1.1.1/gramps_webapi/templates/reset_password_error.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-07-13 08:44:42.000000 gramps-webapi-1.1.1/gramps_webapi/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:44:47.875770 gramps-webapi-1.1.1/gramps_webapi/util/
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-07-13 08:44:42.000000 gramps-webapi-1.1.1/gramps_webapi/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-07-13 08:44:42.000000 gramps-webapi-1.1.1/gramps_webapi/util/celery.py
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-07-13 08:44:42.000000 gramps-webapi-1.1.1/gramps_webapi/wsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:44:47.863770 gramps-webapi-1.1.1/gramps_webapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-07-13 08:44:47.000000 gramps-webapi-1.1.1/gramps_webapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5075 2023-07-13 08:44:47.000000 gramps-webapi-1.1.1/gramps_webapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 08:44:47.000000 gramps-webapi-1.1.1/gramps_webapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 08:44:47.000000 gramps-webapi-1.1.1/gramps_webapi.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-13 08:44:47.000000 gramps-webapi-1.1.1/gramps_webapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-13 08:44:47.000000 gramps-webapi-1.1.1/gramps_webapi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-13 08:44:47.883770 gramps-webapi-1.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-07-13 08:44:42.000000 gramps-webapi-1.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:44:47.875770 gramps-webapi-1.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4742 2023-07-13 08:44:42.000000 gramps-webapi-1.1.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6209 2023-07-13 08:44:42.000000 gramps-webapi-1.1.1/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-07-13 08:44:42.000000 gramps-webapi-1.1.1/tests/test_db.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:44:47.883770 gramps-webapi-1.1.1/tests/test_endpoints/
+-rw-r--r--   0 runner    (1001) docker     (123)     3919 2023-07-13 08:44:42.000000 gramps-webapi-1.1.1/tests/test_endpoints/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13692 2023-07-13 08:44:42.000000 gramps-webapi-1.1.1/tests/test_endpoints/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-07-13 08:44:42.000000 gramps-webapi-1.1.1/tests/test_endpoints/test_bookmarks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23353 2023-07-13 08:44:42.000000 gramps-webapi-1.1.1/tests/test_endpoints/test_citations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5804 2023-07-13 08:44:42.000000 gramps-webapi-1.1.1/tests/test_endpoints/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9073 2023-07-13 08:44:42.000000 gramps-webapi-1.1.1/tests/test_endpoints/test_delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36600 2023-07-13 08:44:42.000000 gramps-webapi-1.1.1/tests/test_endpoints/test_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20530 2023-07-13 08:44:42.000000 gramps-webapi-1.1.1/tests/test_endpoints/test_exporters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7353 2023-07-13 08:44:42.000000 gramps-webapi-1.1.1/tests/test_endpoints/test_facts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48295 2023-07-13 08:44:42.000000 gramps-webapi-1.1.1/tests/test_endpoints/test_families.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9733 2023-07-13 08:44:42.000000 gramps-webapi-1.1.1/tests/test_endpoints/test_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9350 2023-07-13 08:44:42.000000 gramps-webapi-1.1.1/tests/test_endpoints/test_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-07-13 08:44:42.000000 gramps-webapi-1.1.1/tests/test_endpoints/test_holidays.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5807 2023-07-13 08:44:42.000000 gramps-webapi-1.1.1/tests/test_endpoints/test_import_media.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7482 2023-07-13 08:44:42.000000 gramps-webapi-1.1.1/tests/test_endpoints/test_importers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5842 2023-07-13 08:44:42.000000 gramps-webapi-1.1.1/tests/test_endpoints/test_living.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22991 2023-07-13 08:44:42.000000 gramps-webapi-1.1.1/tests/test_endpoints/test_media.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-07-13 08:44:42.000000 gramps-webapi-1.1.1/tests/test_endpoints/test_media_archive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-07-13 08:44:42.000000 gramps-webapi-1.1.1/tests/test_endpoints/test_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-07-13 08:44:42.000000 gramps-webapi-1.1.1/tests/test_endpoints/test_name_formats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3889 2023-07-13 08:44:42.000000 gramps-webapi-1.1.1/tests/test_endpoints/test_name_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21252 2023-07-13 08:44:42.000000 gramps-webapi-1.1.1/tests/test_endpoints/test_notes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67014 2023-07-13 08:44:42.000000 gramps-webapi-1.1.1/tests/test_endpoints/test_people.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24741 2023-07-13 08:44:42.000000 gramps-webapi-1.1.1/tests/test_endpoints/test_places.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28473 2023-07-13 08:44:42.000000 gramps-webapi-1.1.1/tests/test_endpoints/test_post.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10113 2023-07-13 08:44:42.000000 gramps-webapi-1.1.1/tests/test_endpoints/test_put.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7461 2023-07-13 08:44:42.000000 gramps-webapi-1.1.1/tests/test_endpoints/test_relations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9101 2023-07-13 08:44:42.000000 gramps-webapi-1.1.1/tests/test_endpoints/test_reports.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21917 2023-07-13 08:44:42.000000 gramps-webapi-1.1.1/tests/test_endpoints/test_repositories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3236 2023-07-13 08:44:42.000000 gramps-webapi-1.1.1/tests/test_endpoints/test_s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12745 2023-07-13 08:44:42.000000 gramps-webapi-1.1.1/tests/test_endpoints/test_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23669 2023-07-13 08:44:42.000000 gramps-webapi-1.1.1/tests/test_endpoints/test_sources.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11735 2023-07-13 08:44:42.000000 gramps-webapi-1.1.1/tests/test_endpoints/test_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-07-13 08:44:42.000000 gramps-webapi-1.1.1/tests/test_endpoints/test_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23885 2023-07-13 08:44:42.000000 gramps-webapi-1.1.1/tests/test_endpoints/test_timelines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8526 2023-07-13 08:44:42.000000 gramps-webapi-1.1.1/tests/test_endpoints/test_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14548 2023-07-13 08:44:42.000000 gramps-webapi-1.1.1/tests/test_endpoints/test_transactions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4981 2023-07-13 08:44:42.000000 gramps-webapi-1.1.1/tests/test_endpoints/test_translations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9571 2023-07-13 08:44:42.000000 gramps-webapi-1.1.1/tests/test_endpoints/test_trees.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6281 2023-07-13 08:44:42.000000 gramps-webapi-1.1.1/tests/test_endpoints/test_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10209 2023-07-13 08:44:42.000000 gramps-webapi-1.1.1/tests/test_endpoints/test_upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38607 2023-07-13 08:44:42.000000 gramps-webapi-1.1.1/tests/test_endpoints/test_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-07-13 08:44:42.000000 gramps-webapi-1.1.1/tests/test_endpoints/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-07-13 08:44:42.000000 gramps-webapi-1.1.1/tests/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7854 2023-07-13 08:44:42.000000 gramps-webapi-1.1.1/tests/test_jwt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-07-13 08:44:42.000000 gramps-webapi-1.1.1/tests/test_limiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-07-13 08:44:42.000000 gramps-webapi-1.1.1/tests/test_password.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-07-13 08:44:42.000000 gramps-webapi-1.1.1/tests/test_s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-07-13 08:44:42.000000 gramps-webapi-1.1.1/tests/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6191 2023-07-13 08:44:42.000000 gramps-webapi-1.1.1/tests/test_sqlauth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-07-13 08:44:42.000000 gramps-webapi-1.1.1/tests/test_version.py
```

### Comparing `gramps-webapi-1.1.0/LICENSE` & `gramps-webapi-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.0/PKG-INFO` & `gramps-webapi-1.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gramps-webapi
-Version: 1.1.0
+Version: 1.1.1
 Summary: A RESTful web API for the Gramps genealogical database.
 Home-page: https://github.com/gramps-project/web-api
 Author: Gramps Development Team
 License: AGPL v3 or greater
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `gramps-webapi-1.1.0/README.md` & `gramps-webapi-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.0/gramps_webapi/__init__.py` & `gramps-webapi-1.1.1/gramps_webapi/__init__.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.0/gramps_webapi/__main__.py` & `gramps-webapi-1.1.1/gramps_webapi/__main__.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.0/gramps_webapi/_version.py` & `gramps-webapi-1.1.1/gramps_webapi/_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,8 +14,8 @@
 # GNU Affero General Public License for more details.
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with this program. If not, see <https://www.gnu.org/licenses/>.
 #
 
 # make sure to match this version with the one in apispec.yaml
-__version__ = "1.1.0"
+__version__ = "1.1.1"
```

### Comparing `gramps-webapi-1.1.0/gramps_webapi/api/__init__.py` & `gramps-webapi-1.1.1/gramps_webapi/api/__init__.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.0/gramps_webapi/api/auth.py` & `gramps-webapi-1.1.1/gramps_webapi/api/auth.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.0/gramps_webapi/api/emails.py` & `gramps-webapi-1.1.1/gramps_webapi/api/emails.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.0/gramps_webapi/api/export.py` & `gramps-webapi-1.1.1/gramps_webapi/api/export.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.0/gramps_webapi/api/file.py` & `gramps-webapi-1.1.1/gramps_webapi/api/file.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.0/gramps_webapi/api/html.py` & `gramps-webapi-1.1.1/gramps_webapi/api/html.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.0/gramps_webapi/api/image.py` & `gramps-webapi-1.1.1/gramps_webapi/api/image.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.0/gramps_webapi/api/media.py` & `gramps-webapi-1.1.1/gramps_webapi/api/media.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.0/gramps_webapi/api/report.py` & `gramps-webapi-1.1.1/gramps_webapi/api/report.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.0/gramps_webapi/api/resources/__init__.py` & `gramps-webapi-1.1.1/gramps_webapi/api/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.0/gramps_webapi/api/resources/base.py` & `gramps-webapi-1.1.1/gramps_webapi/api/resources/base.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.0/gramps_webapi/api/resources/bookmarks.py` & `gramps-webapi-1.1.1/gramps_webapi/api/resources/bookmarks.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.0/gramps_webapi/api/resources/citations.py` & `gramps-webapi-1.1.1/gramps_webapi/api/resources/citations.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.0/gramps_webapi/api/resources/config.py` & `gramps-webapi-1.1.1/gramps_webapi/api/resources/config.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.0/gramps_webapi/api/resources/delete.py` & `gramps-webapi-1.1.1/gramps_webapi/api/resources/delete.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.0/gramps_webapi/api/resources/emit.py` & `gramps-webapi-1.1.1/gramps_webapi/api/resources/emit.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.0/gramps_webapi/api/resources/events.py` & `gramps-webapi-1.1.1/gramps_webapi/api/resources/events.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.0/gramps_webapi/api/resources/export_media.py` & `gramps-webapi-1.1.1/gramps_webapi/api/resources/export_media.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.0/gramps_webapi/api/resources/exporters.py` & `gramps-webapi-1.1.1/gramps_webapi/api/resources/exporters.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.0/gramps_webapi/api/resources/face_detection.py` & `gramps-webapi-1.1.1/gramps_webapi/api/resources/face_detection.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.0/gramps_webapi/api/resources/facts.py` & `gramps-webapi-1.1.1/gramps_webapi/api/resources/facts.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.0/gramps_webapi/api/resources/families.py` & `gramps-webapi-1.1.1/gramps_webapi/api/resources/families.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.0/gramps_webapi/api/resources/file.py` & `gramps-webapi-1.1.1/gramps_webapi/api/resources/file.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.0/gramps_webapi/api/resources/filters.py` & `gramps-webapi-1.1.1/gramps_webapi/api/resources/filters.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.0/gramps_webapi/api/resources/holidays.py` & `gramps-webapi-1.1.1/gramps_webapi/api/resources/holidays.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.0/gramps_webapi/api/resources/import_media.py` & `gramps-webapi-1.1.1/gramps_webapi/api/resources/import_media.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.0/gramps_webapi/api/resources/importers.py` & `gramps-webapi-1.1.1/gramps_webapi/api/resources/importers.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.0/gramps_webapi/api/resources/living.py` & `gramps-webapi-1.1.1/gramps_webapi/api/resources/living.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.0/gramps_webapi/api/resources/match.py` & `gramps-webapi-1.1.1/gramps_webapi/api/resources/match.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.0/gramps_webapi/api/resources/media.py` & `gramps-webapi-1.1.1/gramps_webapi/api/resources/media.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.0/gramps_webapi/api/resources/metadata.py` & `gramps-webapi-1.1.1/gramps_webapi/api/resources/metadata.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.0/gramps_webapi/api/resources/name_formats.py` & `gramps-webapi-1.1.1/gramps_webapi/api/resources/name_formats.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.0/gramps_webapi/api/resources/name_groups.py` & `gramps-webapi-1.1.1/gramps_webapi/api/resources/name_groups.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.0/gramps_webapi/api/resources/notes.py` & `gramps-webapi-1.1.1/gramps_webapi/api/resources/notes.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.0/gramps_webapi/api/resources/objects.py` & `gramps-webapi-1.1.1/gramps_webapi/api/resources/objects.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 from ..search import SearchIndexer
 from ..util import (
     abort_with_message,
     check_quota_people,
     get_db_handle,
     get_search_indexer,
     get_tree_from_jwt,
+    update_usage_people,
 )
 from . import ProtectedResource
 from .util import add_object, fix_object_dict, transaction_to_json, validate_object_dict
 
 
 class CreateObjectsResource(ProtectedResource):
     """Resource for creating multiple objects."""
@@ -78,14 +79,16 @@
         with DbTxn("Add objects", db_handle) as trans:
             for obj in objects:
                 try:
                     add_object(db_handle, obj, trans, fail_if_exists=True)
                 except ValueError:
                     abort_with_message(400, "Error while adding object")
             trans_dict = transaction_to_json(trans)
+        if number_new_people:
+            update_usage_people()
         # update search index
         tree = get_tree_from_jwt()
         indexer: SearchIndexer = get_search_indexer(tree)
         with indexer.get_writer(overwrite=False, use_async=True) as writer:
             for _trans_dict in trans_dict:
                 handle = _trans_dict["handle"]
                 class_name = _trans_dict["_class"]
```

### Comparing `gramps-webapi-1.1.0/gramps_webapi/api/resources/people.py` & `gramps-webapi-1.1.1/gramps_webapi/api/resources/people.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.0/gramps_webapi/api/resources/places.py` & `gramps-webapi-1.1.1/gramps_webapi/api/resources/places.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.0/gramps_webapi/api/resources/relations.py` & `gramps-webapi-1.1.1/gramps_webapi/api/resources/relations.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.0/gramps_webapi/api/resources/reports.py` & `gramps-webapi-1.1.1/gramps_webapi/api/resources/reports.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.0/gramps_webapi/api/resources/repositories.py` & `gramps-webapi-1.1.1/gramps_webapi/api/resources/repositories.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.0/gramps_webapi/api/resources/search.py` & `gramps-webapi-1.1.1/gramps_webapi/api/resources/search.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.0/gramps_webapi/api/resources/sort.py` & `gramps-webapi-1.1.1/gramps_webapi/api/resources/sort.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.0/gramps_webapi/api/resources/sources.py` & `gramps-webapi-1.1.1/gramps_webapi/api/resources/sources.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.0/gramps_webapi/api/resources/tags.py` & `gramps-webapi-1.1.1/gramps_webapi/api/resources/tags.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.0/gramps_webapi/api/resources/tasks.py` & `gramps-webapi-1.1.1/gramps_webapi/api/resources/tasks.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.0/gramps_webapi/api/resources/timeline.py` & `gramps-webapi-1.1.1/gramps_webapi/api/resources/timeline.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.0/gramps_webapi/api/resources/token.py` & `gramps-webapi-1.1.1/gramps_webapi/api/resources/token.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.0/gramps_webapi/api/resources/transactions.py` & `gramps-webapi-1.1.1/gramps_webapi/api/resources/transactions.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,14 +36,15 @@
 from ..search import SearchIndexer
 from ..util import (
     abort_with_message,
     check_quota_people,
     get_db_handle,
     get_search_indexer,
     get_tree_from_jwt,
+    update_usage_people,
     use_args,
 )
 from . import ProtectedResource
 from .util import reverse_transaction, transaction_to_json
 
 trans_code = {"delete": TXNDEL, "add": TXNADD, "update": TXNUPD}
 
@@ -94,14 +95,16 @@
                     elif trans_type == "update":
                         self.handle_commit(trans, class_name, new_obj)
                     else:
                         abort_with_message(400, "Unexpected transaction type")
                 except (KeyError, UnicodeDecodeError, json.JSONDecodeError, TypeError):
                     abort_with_message(400, "Error while processing transaction")
             trans_dict = transaction_to_json(trans)
+        if num_people_new:
+            update_usage_people()
         # update search index
         tree = get_tree_from_jwt()
         indexer: SearchIndexer = get_search_indexer(tree)
         with indexer.get_writer(overwrite=False, use_async=True) as writer:
             for _trans_dict in trans_dict:
                 handle = _trans_dict["handle"]
                 class_name = _trans_dict["_class"]
```

### Comparing `gramps-webapi-1.1.0/gramps_webapi/api/resources/translations.py` & `gramps-webapi-1.1.1/gramps_webapi/api/resources/translations.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.0/gramps_webapi/api/resources/trees.py` & `gramps-webapi-1.1.1/gramps_webapi/api/resources/trees.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.0/gramps_webapi/api/resources/types.py` & `gramps-webapi-1.1.1/gramps_webapi/api/resources/types.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.0/gramps_webapi/api/resources/user.py` & `gramps-webapi-1.1.1/gramps_webapi/api/resources/user.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.0/gramps_webapi/api/resources/util.py` & `gramps-webapi-1.1.1/gramps_webapi/api/resources/util.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.0/gramps_webapi/api/s3.py` & `gramps-webapi-1.1.1/gramps_webapi/api/s3.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.0/gramps_webapi/api/search.py` & `gramps-webapi-1.1.1/gramps_webapi/api/search.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.0/gramps_webapi/api/tasks.py` & `gramps-webapi-1.1.1/gramps_webapi/api/tasks.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,14 +36,15 @@
 from .resources.util import dry_run_import, run_import, run_import_media_archive
 from .util import (
     check_quota_people,
     get_config,
     get_db_outside_request,
     get_search_indexer,
     send_email,
+    update_usage_people,
 )
 
 
 def run_task(task: Callable, **kwargs) -> Union[AsyncResult, Any]:
     """Send a task to the task queue or run immediately if no queue set up."""
     if not current_app.config["CELERY_CONFIG"]:
         with current_app.app_context():
@@ -131,14 +132,15 @@
     db_handle = get_db_outside_request(tree=tree, view_private=True, readonly=True)
     run_import(
         db_handle=db_handle,
         file_name=file_name,
         extension=extension.lower(),
         delete=delete,
     )
+    update_usage_people(tree=tree)
     _search_reindex_incremental(tree)
 
 
 @shared_task()
 def export_db(
     tree: str, extension: str, options: Dict, view_private: bool
 ) -> Dict[str, str]:
@@ -202,15 +204,14 @@
         "file_size": file_size,
     }
 
 
 @shared_task()
 def import_media_archive(tree: str, file_name: str, delete: bool = True):
     """Import a media archive."""
-    # check_quota_people(to_add=object_counts["people"], tree=tree)
     db_handle = get_db_outside_request(tree=tree, view_private=True, readonly=True)
     result = run_import_media_archive(
         tree=tree,
         db_handle=db_handle,
         file_name=file_name,
         delete=delete,
     )
```

### Comparing `gramps-webapi-1.1.0/gramps_webapi/api/util.py` & `gramps-webapi-1.1.1/gramps_webapi/api/util.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.0/gramps_webapi/app.py` & `gramps-webapi-1.1.1/gramps_webapi/app.py`

 * *Files 0% similar despite different names*

```diff
@@ -118,15 +118,15 @@
             "set to `False`. This is strongly discouraged as it exposes media "
             "files to users belonging to different trees!"
         )
 
     if app.config["TREE"] == TREE_MULTI and app.config["NEW_DB_BACKEND"] != "sqlite":
         # needed in case a new postgres tree is to be created
         gramps_config.set("database.host", app.config["POSTGRES_HOST"])
-        gramps_config.set("database.port", app.config["POSTGRES_PORT"])
+        gramps_config.set("database.port", str(app.config["POSTGRES_PORT"]))
 
     # load JWT default settings
     app.config.from_object(DefaultConfigJWT)
 
     # instantiate JWT manager
     JWTManager(app)
```

### Comparing `gramps-webapi-1.1.0/gramps_webapi/auth/__init__.py` & `gramps-webapi-1.1.1/gramps_webapi/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.0/gramps_webapi/auth/const.py` & `gramps-webapi-1.1.1/gramps_webapi/auth/const.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.0/gramps_webapi/auth/passwords.py` & `gramps-webapi-1.1.1/gramps_webapi/auth/passwords.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.0/gramps_webapi/auth/sql_guid.py` & `gramps-webapi-1.1.1/gramps_webapi/auth/sql_guid.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.0/gramps_webapi/config.py` & `gramps-webapi-1.1.1/gramps_webapi/config.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.0/gramps_webapi/const.py` & `gramps-webapi-1.1.1/gramps_webapi/const.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.0/gramps_webapi/data/apispec.yaml` & `gramps-webapi-1.1.1/gramps_webapi/data/apispec.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 00000170: 6d70 7320 616e 6420 7468 6520 6e75 6d65  mps and the nume
 00000180: 726f 7573 2066 6561 7475 7265 7320 6974  rous features it
 00000190: 2070 726f 7669 6465 7320 666f 7220 6765   provides for ge
 000001a0: 6e65 616c 6f67 6973 7473 2063 616e 2062  nealogists can b
 000001b0: 6520 666f 756e 6420 6174 2068 7474 7073  e found at https
 000001c0: 3a2f 2f67 7261 6d70 732d 7072 6f6a 6563  ://gramps-projec
 000001d0: 742e 6f72 670a 2020 7665 7273 696f 6e3a  t.org.  version:
-000001e0: 2022 312e 312e 3022 2020 2320 6d61 6b65   "1.1.0"  # make
+000001e0: 2022 312e 312e 3122 2020 2320 6d61 6b65   "1.1.1"  # make
 000001f0: 2073 7572 6520 746f 206d 6174 6368 2074   sure to match t
 00000200: 6869 7320 7665 7273 696f 6e20 7769 7468  his version with
 00000210: 2074 6865 206f 6e65 2069 6e20 5f76 6572   the one in _ver
 00000220: 7369 6f6e 2e70 790a 2020 6c69 6365 6e73  sion.py.  licens
 00000230: 653a 0a20 2020 206e 616d 653a 2022 474e  e:.    name: "GN
 00000240: 5520 4166 6665 726f 2047 656e 6572 616c  U Affero General
 00000250: 2050 7562 6c69 6320 4c69 6365 6e73 6520   Public License
```

### Comparing `gramps-webapi-1.1.0/gramps_webapi/data/haarcascade_frontalface_default.xml` & `gramps-webapi-1.1.1/gramps_webapi/data/haarcascade_frontalface_default.xml`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.0/gramps_webapi/dbloader.py` & `gramps-webapi-1.1.1/gramps_webapi/dbloader.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.0/gramps_webapi/dbmanager.py` & `gramps-webapi-1.1.1/gramps_webapi/dbmanager.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.0/gramps_webapi/templates/confirmation.html` & `gramps-webapi-1.1.1/gramps_webapi/templates/confirmation.html`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.0/gramps_webapi/templates/reset_password.html` & `gramps-webapi-1.1.1/gramps_webapi/templates/reset_password.html`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.0/gramps_webapi/templates/reset_password_base.html` & `gramps-webapi-1.1.1/gramps_webapi/templates/reset_password_base.html`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.0/gramps_webapi/types.py` & `gramps-webapi-1.1.1/gramps_webapi/types.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.0/gramps_webapi/util/__init__.py` & `gramps-webapi-1.1.1/gramps_webapi/util/__init__.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.0/gramps_webapi/util/celery.py` & `gramps-webapi-1.1.1/gramps_webapi/util/celery.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.0/gramps_webapi/wsgi.py` & `gramps-webapi-1.1.1/gramps_webapi/wsgi.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.0/gramps_webapi.egg-info/PKG-INFO` & `gramps-webapi-1.1.1/gramps_webapi.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gramps-webapi
-Version: 1.1.0
+Version: 1.1.1
 Summary: A RESTful web API for the Gramps genealogical database.
 Home-page: https://github.com/gramps-project/web-api
 Author: Gramps Development Team
 License: AGPL v3 or greater
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `gramps-webapi-1.1.0/gramps_webapi.egg-info/SOURCES.txt` & `gramps-webapi-1.1.1/gramps_webapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.0/setup.py` & `gramps-webapi-1.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.0/tests/__init__.py` & `gramps-webapi-1.1.1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.0/tests/test_cli.py` & `gramps-webapi-1.1.1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.0/tests/test_db.py` & `gramps-webapi-1.1.1/tests/test_db.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.0/tests/test_endpoints/__init__.py` & `gramps-webapi-1.1.1/tests/test_endpoints/__init__.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.0/tests/test_endpoints/checks.py` & `gramps-webapi-1.1.1/tests/test_endpoints/checks.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.0/tests/test_endpoints/test_bookmarks.py` & `gramps-webapi-1.1.1/tests/test_endpoints/test_bookmarks.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.0/tests/test_endpoints/test_citations.py` & `gramps-webapi-1.1.1/tests/test_endpoints/test_citations.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.0/tests/test_endpoints/test_config.py` & `gramps-webapi-1.1.1/tests/test_endpoints/test_config.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.0/tests/test_endpoints/test_delete.py` & `gramps-webapi-1.1.1/tests/test_endpoints/test_delete.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.0/tests/test_endpoints/test_events.py` & `gramps-webapi-1.1.1/tests/test_endpoints/test_events.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.0/tests/test_endpoints/test_exporters.py` & `gramps-webapi-1.1.1/tests/test_endpoints/test_exporters.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.0/tests/test_endpoints/test_facts.py` & `gramps-webapi-1.1.1/tests/test_endpoints/test_facts.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.0/tests/test_endpoints/test_families.py` & `gramps-webapi-1.1.1/tests/test_endpoints/test_families.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.0/tests/test_endpoints/test_file.py` & `gramps-webapi-1.1.1/tests/test_endpoints/test_file.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.0/tests/test_endpoints/test_filters.py` & `gramps-webapi-1.1.1/tests/test_endpoints/test_filters.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.0/tests/test_endpoints/test_holidays.py` & `gramps-webapi-1.1.1/tests/test_endpoints/test_holidays.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.0/tests/test_endpoints/test_import_media.py` & `gramps-webapi-1.1.1/tests/test_endpoints/test_import_media.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.0/tests/test_endpoints/test_importers.py` & `gramps-webapi-1.1.1/tests/test_endpoints/test_importers.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.0/tests/test_endpoints/test_living.py` & `gramps-webapi-1.1.1/tests/test_endpoints/test_living.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.0/tests/test_endpoints/test_media.py` & `gramps-webapi-1.1.1/tests/test_endpoints/test_media.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.0/tests/test_endpoints/test_media_archive.py` & `gramps-webapi-1.1.1/tests/test_endpoints/test_media_archive.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.0/tests/test_endpoints/test_metadata.py` & `gramps-webapi-1.1.1/tests/test_endpoints/test_metadata.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.0/tests/test_endpoints/test_name_formats.py` & `gramps-webapi-1.1.1/tests/test_endpoints/test_name_formats.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.0/tests/test_endpoints/test_name_groups.py` & `gramps-webapi-1.1.1/tests/test_endpoints/test_name_groups.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.0/tests/test_endpoints/test_notes.py` & `gramps-webapi-1.1.1/tests/test_endpoints/test_notes.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.0/tests/test_endpoints/test_people.py` & `gramps-webapi-1.1.1/tests/test_endpoints/test_people.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.0/tests/test_endpoints/test_places.py` & `gramps-webapi-1.1.1/tests/test_endpoints/test_places.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.0/tests/test_endpoints/test_post.py` & `gramps-webapi-1.1.1/tests/test_endpoints/test_post.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.0/tests/test_endpoints/test_put.py` & `gramps-webapi-1.1.1/tests/test_endpoints/test_put.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.0/tests/test_endpoints/test_relations.py` & `gramps-webapi-1.1.1/tests/test_endpoints/test_relations.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.0/tests/test_endpoints/test_reports.py` & `gramps-webapi-1.1.1/tests/test_endpoints/test_reports.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.0/tests/test_endpoints/test_repositories.py` & `gramps-webapi-1.1.1/tests/test_endpoints/test_repositories.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.0/tests/test_endpoints/test_s3.py` & `gramps-webapi-1.1.1/tests/test_endpoints/test_s3.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.0/tests/test_endpoints/test_search.py` & `gramps-webapi-1.1.1/tests/test_endpoints/test_search.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.0/tests/test_endpoints/test_sources.py` & `gramps-webapi-1.1.1/tests/test_endpoints/test_sources.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.0/tests/test_endpoints/test_tags.py` & `gramps-webapi-1.1.1/tests/test_endpoints/test_tags.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.0/tests/test_endpoints/test_tasks.py` & `gramps-webapi-1.1.1/tests/test_endpoints/test_tasks.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.0/tests/test_endpoints/test_timelines.py` & `gramps-webapi-1.1.1/tests/test_endpoints/test_timelines.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.0/tests/test_endpoints/test_token.py` & `gramps-webapi-1.1.1/tests/test_endpoints/test_token.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.0/tests/test_endpoints/test_transactions.py` & `gramps-webapi-1.1.1/tests/test_endpoints/test_transactions.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.0/tests/test_endpoints/test_translations.py` & `gramps-webapi-1.1.1/tests/test_endpoints/test_translations.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.0/tests/test_endpoints/test_trees.py` & `gramps-webapi-1.1.1/tests/test_endpoints/test_trees.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.0/tests/test_endpoints/test_types.py` & `gramps-webapi-1.1.1/tests/test_endpoints/test_types.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.0/tests/test_endpoints/test_upload.py` & `gramps-webapi-1.1.1/tests/test_endpoints/test_upload.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.0/tests/test_endpoints/test_user.py` & `gramps-webapi-1.1.1/tests/test_endpoints/test_user.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.0/tests/test_endpoints/util.py` & `gramps-webapi-1.1.1/tests/test_endpoints/util.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.0/tests/test_init.py` & `gramps-webapi-1.1.1/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.0/tests/test_jwt.py` & `gramps-webapi-1.1.1/tests/test_jwt.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.0/tests/test_limiter.py` & `gramps-webapi-1.1.1/tests/test_limiter.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.0/tests/test_password.py` & `gramps-webapi-1.1.1/tests/test_password.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.0/tests/test_s3.py` & `gramps-webapi-1.1.1/tests/test_s3.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.0/tests/test_schema.py` & `gramps-webapi-1.1.1/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.0/tests/test_sqlauth.py` & `gramps-webapi-1.1.1/tests/test_sqlauth.py`

 * *Files identical despite different names*

### Comparing `gramps-webapi-1.1.0/tests/test_version.py` & `gramps-webapi-1.1.1/tests/test_version.py`

 * *Files identical despite different names*

