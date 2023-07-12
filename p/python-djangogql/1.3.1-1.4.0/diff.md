# Comparing `tmp/python-djangogql-1.3.1.tar.gz` & `tmp/python-djangogql-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-djangogql-1.3.1.tar", last modified: Wed Jul 12 00:05:09 2023, max compression
+gzip compressed data, was "python-djangogql-1.4.0.tar", last modified: Wed Jul 12 23:57:49 2023, max compression
```

## Comparing `python-djangogql-1.3.1.tar` & `python-djangogql-1.4.0.tar`

### file list

```diff
@@ -1,61 +1,58 @@
-drwxrwxr-x   0 felipefariapessoal  (1001) felipefariapessoal  (1001)        0 2023-07-12 00:05:09.468482 python-djangogql-1.3.1/
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     1086 2023-07-09 22:53:34.000000 python-djangogql-1.3.1/LICENSE
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)       74 2023-07-08 20:27:42.000000 python-djangogql-1.3.1/MANIFEST.in
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     1353 2023-07-12 00:05:09.468482 python-djangogql-1.3.1/PKG-INFO
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)      319 2023-07-09 21:56:06.000000 python-djangogql-1.3.1/README.md
-drwxrwxr-x   0 felipefariapessoal  (1001) felipefariapessoal  (1001)        0 2023-07-12 00:05:09.460482 python-djangogql-1.3.1/djangogql/
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)        0 2023-07-08 01:33:53.000000 python-djangogql-1.3.1/djangogql/__init__.py
-drwxrwxr-x   0 felipefariapessoal  (1001) felipefariapessoal  (1001)        0 2023-07-12 00:05:09.460482 python-djangogql-1.3.1/djangogql/account/
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)        0 2023-07-09 21:39:57.000000 python-djangogql-1.3.1/djangogql/account/__init__.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     1740 2023-07-09 21:42:29.000000 python-djangogql-1.3.1/djangogql/account/mixins.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     1833 2023-07-09 15:12:17.000000 python-djangogql-1.3.1/djangogql/auth_backend.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     1435 2023-07-10 00:14:32.000000 python-djangogql-1.3.1/djangogql/context.py
-drwxrwxr-x   0 felipefariapessoal  (1001) felipefariapessoal  (1001)        0 2023-07-12 00:05:09.464482 python-djangogql-1.3.1/djangogql/core/
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)      162 2023-07-10 00:14:38.000000 python-djangogql-1.3.1/djangogql/core/__init__.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)    15901 2023-07-10 00:13:32.000000 python-djangogql-1.3.1/djangogql/core/connection.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)      511 2023-07-10 00:14:08.000000 python-djangogql-1.3.1/djangogql/core/context.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     1467 2023-07-08 20:10:57.000000 python-djangogql-1.3.1/djangogql/core/dataloaders.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     1062 2023-07-10 17:27:11.000000 python-djangogql-1.3.1/djangogql/core/enums.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     3642 2023-07-10 17:27:09.000000 python-djangogql-1.3.1/djangogql/core/fields.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     5010 2023-07-10 17:27:06.000000 python-djangogql-1.3.1/djangogql/core/filters.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)    17475 2023-07-10 17:26:55.000000 python-djangogql-1.3.1/djangogql/core/mutations.py
-drwxrwxr-x   0 felipefariapessoal  (1001) felipefariapessoal  (1001)        0 2023-07-12 00:05:09.464482 python-djangogql-1.3.1/djangogql/core/types/
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)      119 2023-07-07 20:06:42.000000 python-djangogql-1.3.1/djangogql/core/types/__init__.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)      864 2023-04-29 23:33:17.000000 python-djangogql-1.3.1/djangogql/core/types/base.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     2384 2023-07-07 20:06:42.000000 python-djangogql-1.3.1/djangogql/core/types/common.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     7851 2023-07-12 00:03:45.000000 python-djangogql-1.3.1/djangogql/core/types/converter.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     3641 2023-07-12 00:03:59.000000 python-djangogql-1.3.1/djangogql/core/types/filter_input.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     3837 2023-07-12 00:04:17.000000 python-djangogql-1.3.1/djangogql/core/types/model.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     1193 2023-07-11 18:09:37.000000 python-djangogql-1.3.1/djangogql/core/types/registry.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)      970 2023-05-04 18:55:33.000000 python-djangogql-1.3.1/djangogql/core/types/sort_input.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)      587 2023-07-07 20:06:42.000000 python-djangogql-1.3.1/djangogql/core/types/upload.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)      826 2023-03-05 02:44:45.000000 python-djangogql-1.3.1/djangogql/core/validators.py
-drwxrwxr-x   0 felipefariapessoal  (1001) felipefariapessoal  (1001)        0 2023-07-12 00:05:09.464482 python-djangogql-1.3.1/djangogql/db/
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)        0 2023-07-08 18:13:19.000000 python-djangogql-1.3.1/djangogql/db/__init__.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)      377 2023-07-08 18:13:32.000000 python-djangogql-1.3.1/djangogql/db/utils.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     1746 2023-07-08 20:10:02.000000 python-djangogql-1.3.1/djangogql/decorators.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)      424 2023-07-08 15:32:48.000000 python-djangogql-1.3.1/djangogql/exceptions.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     5320 2023-07-09 15:01:48.000000 python-djangogql-1.3.1/djangogql/jwt.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     1943 2023-07-09 15:25:27.000000 python-djangogql-1.3.1/djangogql/middleware.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     3630 2023-07-09 18:06:00.000000 python-djangogql-1.3.1/djangogql/permissions.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     3010 2023-07-09 18:05:20.000000 python-djangogql-1.3.1/djangogql/settings.py
-drwxrwxr-x   0 felipefariapessoal  (1001) felipefariapessoal  (1001)        0 2023-07-12 00:05:09.460482 python-djangogql-1.3.1/djangogql/templates/
-drwxrwxr-x   0 felipefariapessoal  (1001) felipefariapessoal  (1001)        0 2023-07-12 00:05:09.464482 python-djangogql-1.3.1/djangogql/templates/graphql/
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     2012 2023-07-08 20:26:43.000000 python-djangogql-1.3.1/djangogql/templates/graphql/playground.html
-drwxrwxr-x   0 felipefariapessoal  (1001) felipefariapessoal  (1001)        0 2023-07-12 00:05:09.464482 python-djangogql-1.3.1/djangogql/utils/
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     7716 2023-07-10 17:27:24.000000 python-djangogql-1.3.1/djangogql/utils/__init__.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     1227 2023-07-11 18:09:37.000000 python-djangogql-1.3.1/djangogql/utils/fields.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     2140 2023-07-07 20:06:42.000000 python-djangogql-1.3.1/djangogql/utils/files.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)      978 2023-03-17 18:04:54.000000 python-djangogql-1.3.1/djangogql/utils/filters.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     3632 2023-07-11 00:24:22.000000 python-djangogql-1.3.1/djangogql/utils/sorting.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)    10231 2023-07-09 15:40:58.000000 python-djangogql-1.3.1/djangogql/views.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)       88 2023-07-09 16:38:33.000000 python-djangogql-1.3.1/pyproject.toml
-drwxrwxr-x   0 felipefariapessoal  (1001) felipefariapessoal  (1001)        0 2023-07-12 00:05:09.468482 python-djangogql-1.3.1/python_djangogql.egg-info/
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     1353 2023-07-12 00:05:09.000000 python-djangogql-1.3.1/python_djangogql.egg-info/PKG-INFO
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     1334 2023-07-12 00:05:09.000000 python-djangogql-1.3.1/python_djangogql.egg-info/SOURCES.txt
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)        1 2023-07-12 00:05:09.000000 python-djangogql-1.3.1/python_djangogql.egg-info/dependency_links.txt
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)        1 2023-07-09 23:00:28.000000 python-djangogql-1.3.1/python_djangogql.egg-info/not-zip-safe
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)      164 2023-07-12 00:05:09.000000 python-djangogql-1.3.1/python_djangogql.egg-info/requires.txt
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)       10 2023-07-12 00:05:09.000000 python-djangogql-1.3.1/python_djangogql.egg-info/top_level.txt
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)       38 2023-07-12 00:05:09.468482 python-djangogql-1.3.1/setup.cfg
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     1573 2023-07-12 00:04:34.000000 python-djangogql-1.3.1/setup.py
+drwxrwxr-x   0 felipefariapessoal  (1001) felipefariapessoal  (1001)        0 2023-07-12 23:57:49.599976 python-djangogql-1.4.0/
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     1086 2023-07-09 22:53:34.000000 python-djangogql-1.4.0/LICENSE
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)       74 2023-07-08 20:27:42.000000 python-djangogql-1.4.0/MANIFEST.in
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     1353 2023-07-12 23:57:49.599976 python-djangogql-1.4.0/PKG-INFO
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)      319 2023-07-09 21:56:06.000000 python-djangogql-1.4.0/README.md
+drwxrwxr-x   0 felipefariapessoal  (1001) felipefariapessoal  (1001)        0 2023-07-12 23:57:49.595976 python-djangogql-1.4.0/djangogql/
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)        0 2023-07-08 01:33:53.000000 python-djangogql-1.4.0/djangogql/__init__.py
+drwxrwxr-x   0 felipefariapessoal  (1001) felipefariapessoal  (1001)        0 2023-07-12 23:57:49.595976 python-djangogql-1.4.0/djangogql/account/
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)        0 2023-07-09 21:39:57.000000 python-djangogql-1.4.0/djangogql/account/__init__.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     1740 2023-07-09 21:42:29.000000 python-djangogql-1.4.0/djangogql/account/mixins.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)      455 2023-07-12 23:57:30.000000 python-djangogql-1.4.0/djangogql/context.py
+drwxrwxr-x   0 felipefariapessoal  (1001) felipefariapessoal  (1001)        0 2023-07-12 23:57:49.595976 python-djangogql-1.4.0/djangogql/core/
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)      110 2023-07-12 23:57:30.000000 python-djangogql-1.4.0/djangogql/core/__init__.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)    15901 2023-07-10 00:13:32.000000 python-djangogql-1.4.0/djangogql/core/connection.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)      511 2023-07-10 00:14:08.000000 python-djangogql-1.4.0/djangogql/core/context.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     1467 2023-07-08 20:10:57.000000 python-djangogql-1.4.0/djangogql/core/dataloaders.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     1062 2023-07-10 17:27:11.000000 python-djangogql-1.4.0/djangogql/core/enums.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     3642 2023-07-10 17:27:09.000000 python-djangogql-1.4.0/djangogql/core/fields.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     3973 2023-07-12 23:57:30.000000 python-djangogql-1.4.0/djangogql/core/filters.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)    17475 2023-07-10 17:26:55.000000 python-djangogql-1.4.0/djangogql/core/mutations.py
+drwxrwxr-x   0 felipefariapessoal  (1001) felipefariapessoal  (1001)        0 2023-07-12 23:57:49.595976 python-djangogql-1.4.0/djangogql/core/types/
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)      578 2023-07-12 23:57:30.000000 python-djangogql-1.4.0/djangogql/core/types/__init__.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)      864 2023-04-29 23:33:17.000000 python-djangogql-1.4.0/djangogql/core/types/base.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     1802 2023-07-12 23:57:30.000000 python-djangogql-1.4.0/djangogql/core/types/common.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     7851 2023-07-12 00:03:45.000000 python-djangogql-1.4.0/djangogql/core/types/converter.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     2910 2023-07-12 23:57:30.000000 python-djangogql-1.4.0/djangogql/core/types/filter_input.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     3806 2023-07-12 23:57:30.000000 python-djangogql-1.4.0/djangogql/core/types/model.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     1027 2023-07-12 23:57:30.000000 python-djangogql-1.4.0/djangogql/core/types/registry.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)      970 2023-05-04 18:55:33.000000 python-djangogql-1.4.0/djangogql/core/types/sort_input.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)      587 2023-07-07 20:06:42.000000 python-djangogql-1.4.0/djangogql/core/types/upload.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)      826 2023-03-05 02:44:45.000000 python-djangogql-1.4.0/djangogql/core/validators.py
+drwxrwxr-x   0 felipefariapessoal  (1001) felipefariapessoal  (1001)        0 2023-07-12 23:57:49.599976 python-djangogql-1.4.0/djangogql/db/
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)        0 2023-07-08 18:13:19.000000 python-djangogql-1.4.0/djangogql/db/__init__.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)      377 2023-07-08 18:13:32.000000 python-djangogql-1.4.0/djangogql/db/utils.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     1718 2023-07-12 23:57:30.000000 python-djangogql-1.4.0/djangogql/decorators.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)      424 2023-07-08 15:32:48.000000 python-djangogql-1.4.0/djangogql/exceptions.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     3630 2023-07-09 18:06:00.000000 python-djangogql-1.4.0/djangogql/permissions.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     3010 2023-07-09 18:05:20.000000 python-djangogql-1.4.0/djangogql/settings.py
+drwxrwxr-x   0 felipefariapessoal  (1001) felipefariapessoal  (1001)        0 2023-07-12 23:57:49.591976 python-djangogql-1.4.0/djangogql/templates/
+drwxrwxr-x   0 felipefariapessoal  (1001) felipefariapessoal  (1001)        0 2023-07-12 23:57:49.599976 python-djangogql-1.4.0/djangogql/templates/graphql/
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     2012 2023-07-08 20:26:43.000000 python-djangogql-1.4.0/djangogql/templates/graphql/playground.html
+drwxrwxr-x   0 felipefariapessoal  (1001) felipefariapessoal  (1001)        0 2023-07-12 23:57:49.599976 python-djangogql-1.4.0/djangogql/utils/
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     7716 2023-07-10 17:27:24.000000 python-djangogql-1.4.0/djangogql/utils/__init__.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     1227 2023-07-11 18:09:37.000000 python-djangogql-1.4.0/djangogql/utils/fields.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     2140 2023-07-07 20:06:42.000000 python-djangogql-1.4.0/djangogql/utils/files.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)      978 2023-03-17 18:04:54.000000 python-djangogql-1.4.0/djangogql/utils/filters.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     3632 2023-07-11 00:24:22.000000 python-djangogql-1.4.0/djangogql/utils/sorting.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)    10231 2023-07-09 15:40:58.000000 python-djangogql-1.4.0/djangogql/views.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)       88 2023-07-09 16:38:33.000000 python-djangogql-1.4.0/pyproject.toml
+drwxrwxr-x   0 felipefariapessoal  (1001) felipefariapessoal  (1001)        0 2023-07-12 23:57:49.599976 python-djangogql-1.4.0/python_djangogql.egg-info/
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     1353 2023-07-12 23:57:49.000000 python-djangogql-1.4.0/python_djangogql.egg-info/PKG-INFO
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     1267 2023-07-12 23:57:49.000000 python-djangogql-1.4.0/python_djangogql.egg-info/SOURCES.txt
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)        1 2023-07-12 23:57:49.000000 python-djangogql-1.4.0/python_djangogql.egg-info/dependency_links.txt
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)        1 2023-07-09 23:00:28.000000 python-djangogql-1.4.0/python_djangogql.egg-info/not-zip-safe
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)      164 2023-07-12 23:57:49.000000 python-djangogql-1.4.0/python_djangogql.egg-info/requires.txt
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)       10 2023-07-12 23:57:49.000000 python-djangogql-1.4.0/python_djangogql.egg-info/top_level.txt
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)       38 2023-07-12 23:57:49.599976 python-djangogql-1.4.0/setup.cfg
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     1573 2023-07-12 23:57:30.000000 python-djangogql-1.4.0/setup.py
```

### Comparing `python-djangogql-1.3.1/LICENSE` & `python-djangogql-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python-djangogql-1.3.1/PKG-INFO` & `python-djangogql-1.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-djangogql
-Version: 1.3.1
+Version: 1.4.0
 Summary: A Django app to build graphql APIs
 Home-page: https://github.com/felipevisu/djangogql
 Author: Felipe Faria
 Author-email: felipevisu@gmail.com
 License: MIT
 Keywords: api graphql graphene django
 Platform: any
```

### Comparing `python-djangogql-1.3.1/djangogql/account/mixins.py` & `python-djangogql-1.4.0/djangogql/account/mixins.py`

 * *Files identical despite different names*

### Comparing `python-djangogql-1.3.1/djangogql/core/connection.py` & `python-djangogql-1.4.0/djangogql/core/connection.py`

 * *Files identical despite different names*

### Comparing `python-djangogql-1.3.1/djangogql/core/dataloaders.py` & `python-djangogql-1.4.0/djangogql/core/dataloaders.py`

 * *Files identical despite different names*

### Comparing `python-djangogql-1.3.1/djangogql/core/enums.py` & `python-djangogql-1.4.0/djangogql/core/enums.py`

 * *Files identical despite different names*

### Comparing `python-djangogql-1.3.1/djangogql/core/fields.py` & `python-djangogql-1.4.0/djangogql/core/fields.py`

 * *Files identical despite different names*

### Comparing `python-djangogql-1.3.1/djangogql/core/filters.py` & `python-djangogql-1.4.0/djangogql/core/filters.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 import django_filters
-import graphene
 from django.core.exceptions import ValidationError
 from django.forms import CharField, Field, MultipleChoiceField
 from django_filters import Filter, MultipleChoiceFilter
 from graphql_relay import from_global_id
 
-from ..utils.filters import filter_range_field
-
 
 def search_filter(queryset, name, value):
     return queryset.filter(name__search=value)
 
 
 class DefaultMultipleChoiceField(MultipleChoiceField):
     default_error_messages = {"invalid_list": "Enter a list of values."}
@@ -57,49 +54,14 @@
 
 class ObjectTypeFilter(django_filters.Filter):
     def __init__(self, input_class, *args, **kwargs):
         self.input_class = input_class
         super().__init__(*args, **kwargs)
 
 
-def filter_created_at(qs, _, value):
-    return filter_range_field(qs, "created_at", value)
-
-
-def filter_updated_at(qs, _, value):
-    return filter_range_field(qs, "updated_at", value)
-
-
-def filter_status(qs, _, value):
-    if not value:
-        return qs
-    return qs.filter(status=value)
-
-
-def filter_metadata(qs, _, value):
-    for metadata_item in value:
-        if metadata_item.value:
-            qs = qs.filter(metadata__contains={metadata_item.key: metadata_item.value})
-        else:
-            qs = qs.filter(metadata__has_key=metadata_item.key)
-    return qs
-
-
-class MetadataFilter(graphene.InputObjectType):
-    key = graphene.String(required=True, description="Key of a metadata item.")
-    value = graphene.String(required=False, description="Value of a metadata item.")
-
-
-class MetadataFilterBase(django_filters.FilterSet):
-    metadata = ListObjectTypeFilter(input_class=MetadataFilter, method=filter_metadata)
-
-    class Meta:
-        abstract = True
-
-
 class GlobalIDFormField(Field):
     default_error_messages = {"invalid": "Invalid ID specified."}
 
     def clean(self, value):
         if not value and not self.required:
             return None
```

### Comparing `python-djangogql-1.3.1/djangogql/core/mutations.py` & `python-djangogql-1.4.0/djangogql/core/mutations.py`

 * *Files identical despite different names*

### Comparing `python-djangogql-1.3.1/djangogql/core/types/base.py` & `python-djangogql-1.4.0/djangogql/core/types/base.py`

 * *Files identical despite different names*

### Comparing `python-djangogql-1.3.1/djangogql/core/types/common.py` & `python-djangogql-1.4.0/djangogql/core/types/common.py`

 * *Files 10% similar despite different names*

```diff
@@ -47,29 +47,7 @@
     gte = graphene.DateTime(description="Start date.", required=False)
     lte = graphene.DateTime(description="End date.", required=False)
 
 
 class IntRangeInput(graphene.InputObjectType):
     gte = graphene.Int(description="Value greater than or equal to.", required=False)
     lte = graphene.Int(description="Value less than or equal to.", required=False)
-
-
-class EntryError(Error):
-    code = graphene.String(description="The error code.")
-    attributes = NonNullList(
-        graphene.ID,
-        description="List of attributes IDs which causes the error.",
-        required=False,
-    )
-    values = NonNullList(
-        graphene.ID,
-        description="List of attribute values IDs which causes the error.",
-        required=False,
-    )
-
-
-class EntryChannelListingError(EntryError):
-    channels = NonNullList(
-        graphene.ID,
-        description="List of channels IDs which causes the error.",
-        required=False,
-    )
```

### Comparing `python-djangogql-1.3.1/djangogql/core/types/converter.py` & `python-djangogql-1.4.0/djangogql/core/types/converter.py`

 * *Files identical despite different names*

### Comparing `python-djangogql-1.3.1/djangogql/core/types/filter_input.py` & `python-djangogql-1.4.0/djangogql/core/types/filter_input.py`

 * *Files 17% similar despite different names*

```diff
@@ -74,40 +74,10 @@
                 field_type.description = getattr(filter_field, "help_text", "")
             kwargs = getattr(field_type, "kwargs", {})
             field_type.kwargs = kwargs
             args[name] = field_type
         return args
 
 
-class ChannelFilterInputObjectType(FilterInputObjectType):
-    channel = Argument(String)
-
-    class Meta:
-        abstract = True
-
-
 class StringFilterInput(graphene.InputObjectType):
     eq = graphene.String(required=False)
     one_of = NonNullList(graphene.String, required=False)
-
-
-class WhereInputObjectType(FilterInputObjectType):
-    class Meta:
-        abstract = True
-
-    @classmethod
-    def __init_subclass_with_meta__(cls, _meta=None, **options):
-        super().__init_subclass_with_meta__(_meta=_meta, **options)
-        cls._meta.fields.update(
-            {
-                "AND": graphene.Field(
-                    NonNullList(
-                        cls,
-                    )
-                ),
-                "OR": graphene.Field(
-                    NonNullList(
-                        cls,
-                    )
-                ),
-            }
-        )
```

### Comparing `python-djangogql-1.3.1/djangogql/core/types/model.py` & `python-djangogql-1.4.0/djangogql/core/types/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -113,8 +113,7 @@
             return model.objects.get(lookup)
         except model.DoesNotExist:
             return None
 
     @classmethod
     def get_model(cls):
         return cls._meta.model
-        return cls._meta.model
```

### Comparing `python-djangogql-1.3.1/djangogql/core/types/registry.py` & `python-djangogql-1.4.0/djangogql/core/types/registry.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,17 +8,14 @@
 
         assert issubclass(
             cls, ModelObjectType
         ), 'Only DjangoObjectTypes can be registered, received "{}"'.format(
             cls.__name__
         )
         assert cls._meta.registry == self, "Registry for a Model have to match."
-        # assert self.get_type_for_model(cls._meta.model) == cls, (
-        #     'Multiple ModelObjectTypes registered for "{}"'.format(cls._meta.model)
-        # )
         if not getattr(cls._meta, "skip_registry", False):
             self._registry[cls._meta.model] = cls
 
     def get_type_for_model(self, model):
         return self._registry.get(model)
 
     def register_converted_field(self, field, converted):
```

### Comparing `python-djangogql-1.3.1/djangogql/core/types/sort_input.py` & `python-djangogql-1.4.0/djangogql/core/types/sort_input.py`

 * *Files identical despite different names*

### Comparing `python-djangogql-1.3.1/djangogql/core/types/upload.py` & `python-djangogql-1.4.0/djangogql/core/types/upload.py`

 * *Files identical despite different names*

### Comparing `python-djangogql-1.3.1/djangogql/core/validators.py` & `python-djangogql-1.4.0/djangogql/core/validators.py`

 * *Files identical despite different names*

### Comparing `python-djangogql-1.3.1/djangogql/decorators.py` & `python-djangogql-1.4.0/djangogql/decorators.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from functools import wraps
 from typing import Iterable
 
 from graphene import ResolveInfo
 
 from .exceptions import PermissionDenied
-from .permissions import (BasePermissionEnum,
-                          one_of_permissions_or_auth_filter_required)
+from .permissions import BasePermissionEnum, one_of_permissions_or_auth_filter_required
 
 
 def context(f):
     def decorator(func):
         @wraps(func)
         def wrapper(*args, **kwargs):
             info = next(arg for arg in args if isinstance(arg, ResolveInfo))
```

### Comparing `python-djangogql-1.3.1/djangogql/permissions.py` & `python-djangogql-1.4.0/djangogql/permissions.py`

 * *Files identical despite different names*

### Comparing `python-djangogql-1.3.1/djangogql/settings.py` & `python-djangogql-1.4.0/djangogql/settings.py`

 * *Files identical despite different names*

### Comparing `python-djangogql-1.3.1/djangogql/templates/graphql/playground.html` & `python-djangogql-1.4.0/djangogql/templates/graphql/playground.html`

 * *Files identical despite different names*

### Comparing `python-djangogql-1.3.1/djangogql/utils/__init__.py` & `python-djangogql-1.4.0/djangogql/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `python-djangogql-1.3.1/djangogql/utils/fields.py` & `python-djangogql-1.4.0/djangogql/utils/fields.py`

 * *Files identical despite different names*

### Comparing `python-djangogql-1.3.1/djangogql/utils/files.py` & `python-djangogql-1.4.0/djangogql/utils/files.py`

 * *Files identical despite different names*

### Comparing `python-djangogql-1.3.1/djangogql/utils/filters.py` & `python-djangogql-1.4.0/djangogql/utils/filters.py`

 * *Files identical despite different names*

### Comparing `python-djangogql-1.3.1/djangogql/utils/sorting.py` & `python-djangogql-1.4.0/djangogql/utils/sorting.py`

 * *Files identical despite different names*

### Comparing `python-djangogql-1.3.1/djangogql/views.py` & `python-djangogql-1.4.0/djangogql/views.py`

 * *Files identical despite different names*

### Comparing `python-djangogql-1.3.1/python_djangogql.egg-info/PKG-INFO` & `python-djangogql-1.4.0/python_djangogql.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-djangogql
-Version: 1.3.1
+Version: 1.4.0
 Summary: A Django app to build graphql APIs
 Home-page: https://github.com/felipevisu/djangogql
 Author: Felipe Faria
 Author-email: felipevisu@gmail.com
 License: MIT
 Keywords: api graphql graphene django
 Platform: any
```

### Comparing `python-djangogql-1.3.1/python_djangogql.egg-info/SOURCES.txt` & `python-djangogql-1.4.0/python_djangogql.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,16 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 setup.py
 djangogql/__init__.py
-djangogql/auth_backend.py
 djangogql/context.py
 djangogql/decorators.py
 djangogql/exceptions.py
-djangogql/jwt.py
-djangogql/middleware.py
 djangogql/permissions.py
 djangogql/settings.py
 djangogql/views.py
 djangogql/account/__init__.py
 djangogql/account/mixins.py
 djangogql/core/__init__.py
 djangogql/core/connection.py
```

### Comparing `python-djangogql-1.3.1/setup.py` & `python-djangogql-1.4.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name="python-djangogql",
-    version="1.3.1",
+    version="1.4.0",
     description="A Django app to build graphql APIs",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/felipevisu/djangogql",
     author="Felipe Faria",
     author_email="felipevisu@gmail.com",
     license="MIT",
```

