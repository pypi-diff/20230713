# Comparing `tmp/ckanext-editable-config-0.0.2.tar.gz` & `tmp/ckanext-editable-config-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ckanext-editable-config-0.0.2.tar", last modified: Thu Jul 13 10:26:11 2023, max compression
+gzip compressed data, was "ckanext-editable-config-0.0.3.tar", last modified: Thu Jul 13 11:05:40 2023, max compression
```

## Comparing `ckanext-editable-config-0.0.2.tar` & `ckanext-editable-config-0.0.3.tar`

### file list

```diff
@@ -1,56 +1,60 @@
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-07-13 10:26:11.137951 ckanext-editable-config-0.0.2/
--rw-r--r--   0 sergey    (1000) sergey    (1000)    34500 2023-06-18 11:13:48.000000 ckanext-editable-config-0.0.2/LICENSE
--rw-r--r--   0 sergey    (1000) sergey    (1000)      215 2023-06-18 11:13:48.000000 ckanext-editable-config-0.0.2/MANIFEST.in
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4933 2023-07-13 10:26:11.137951 ckanext-editable-config-0.0.2/PKG-INFO
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4345 2023-06-19 21:13:09.000000 ckanext-editable-config-0.0.2/README.md
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-07-13 10:26:11.127951 ckanext-editable-config-0.0.2/ckanext/
--rw-r--r--   0 sergey    (1000) sergey    (1000)      202 2023-06-18 20:14:29.000000 ckanext-editable-config-0.0.2/ckanext/__init__.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-07-13 10:26:11.127951 ckanext-editable-config-0.0.2/ckanext/editable_config/
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2023-06-18 11:13:48.000000 ckanext-editable-config-0.0.2/ckanext/editable_config/__init__.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-07-13 10:26:11.127951 ckanext-editable-config-0.0.2/ckanext/editable_config/assets/
--rw-r--r--   0 sergey    (1000) sergey    (1000)      167 2023-06-18 11:13:48.000000 ckanext-editable-config-0.0.2/ckanext/editable_config/assets/script.js
--rw-r--r--   0 sergey    (1000) sergey    (1000)       35 2023-06-18 11:13:48.000000 ckanext-editable-config-0.0.2/ckanext/editable_config/assets/style.css
--rw-r--r--   0 sergey    (1000) sergey    (1000)      359 2023-06-18 11:13:48.000000 ckanext-editable-config-0.0.2/ckanext/editable_config/assets/webassets.yml
--rw-r--r--   0 sergey    (1000) sergey    (1000)      451 2023-06-19 12:53:41.000000 ckanext-editable-config-0.0.2/ckanext/editable_config/config.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-07-13 10:26:11.137951 ckanext-editable-config-0.0.2/ckanext/editable_config/logic/
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2023-06-18 11:15:55.000000 ckanext-editable-config-0.0.2/ckanext/editable_config/logic/__init__.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     6037 2023-07-07 13:06:54.000000 ckanext-editable-config-0.0.2/ckanext/editable_config/logic/action.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1589 2023-06-19 10:13:19.000000 ckanext-editable-config-0.0.2/ckanext/editable_config/logic/auth.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2719 2023-06-19 20:17:49.000000 ckanext-editable-config-0.0.2/ckanext/editable_config/logic/schema.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2023-06-18 11:16:21.000000 ckanext-editable-config-0.0.2/ckanext/editable_config/logic/validators.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-07-13 10:26:11.127951 ckanext-editable-config-0.0.2/ckanext/editable_config/migration/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-07-13 10:26:11.137951 ckanext-editable-config-0.0.2/ckanext/editable_config/migration/editable_config/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1834 2023-06-18 15:19:17.000000 ckanext-editable-config-0.0.2/ckanext/editable_config/migration/editable_config/alembic.ini
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2148 2023-06-18 20:14:29.000000 ckanext-editable-config-0.0.2/ckanext/editable_config/migration/editable_config/env.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      494 2023-06-18 15:19:17.000000 ckanext-editable-config-0.0.2/ckanext/editable_config/migration/editable_config/script.py.mako
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-07-13 10:26:11.137951 ckanext-editable-config-0.0.2/ckanext/editable_config/migration/editable_config/versions/
--rw-r--r--   0 sergey    (1000) sergey    (1000)      655 2023-06-18 19:08:06.000000 ckanext-editable-config-0.0.2/ckanext/editable_config/migration/editable_config/versions/a8d116986c3f_create_editable_config_table.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-07-13 10:26:11.137951 ckanext-editable-config-0.0.2/ckanext/editable_config/model/
--rw-r--r--   0 sergey    (1000) sergey    (1000)       49 2023-06-18 19:08:06.000000 ckanext-editable-config-0.0.2/ckanext/editable_config/model/__init__.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1859 2023-06-19 13:13:22.000000 ckanext-editable-config-0.0.2/ckanext/editable_config/model/option.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3140 2023-07-07 13:13:48.000000 ckanext-editable-config-0.0.2/ckanext/editable_config/plugin.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2605 2023-06-19 20:17:42.000000 ckanext-editable-config-0.0.2/ckanext/editable_config/shared.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-07-13 10:26:11.137951 ckanext-editable-config-0.0.2/ckanext/editable_config/tests/
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2023-06-18 11:13:48.000000 ckanext-editable-config-0.0.2/ckanext/editable_config/tests/__init__.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1254 2023-06-19 20:17:49.000000 ckanext-editable-config-0.0.2/ckanext/editable_config/tests/conftest.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-07-13 10:26:11.137951 ckanext-editable-config-0.0.2/ckanext/editable_config/tests/logic/
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2023-06-18 20:35:03.000000 ckanext-editable-config-0.0.2/ckanext/editable_config/tests/logic/__init__.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4430 2023-06-19 20:17:49.000000 ckanext-editable-config-0.0.2/ckanext/editable_config/tests/logic/test_action.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      750 2023-06-19 12:49:49.000000 ckanext-editable-config-0.0.2/ckanext/editable_config/tests/logic/test_schema.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-07-13 10:26:11.137951 ckanext-editable-config-0.0.2/ckanext/editable_config/tests/model/
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2023-06-18 21:22:56.000000 ckanext-editable-config-0.0.2/ckanext/editable_config/tests/model/__init__.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3473 2023-06-19 20:17:49.000000 ckanext-editable-config-0.0.2/ckanext/editable_config/tests/model/test_option.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1609 2023-06-19 20:17:42.000000 ckanext-editable-config-0.0.2/ckanext/editable_config/tests/test_fixtures.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2023-06-18 19:08:32.000000 ckanext-editable-config-0.0.2/ckanext/editable_config/tests/test_plugin.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2911 2023-06-19 20:17:47.000000 ckanext-editable-config-0.0.2/ckanext/editable_config/tests/test_shared.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-07-13 10:26:11.137951 ckanext-editable-config-0.0.2/ckanext_editable_config.egg-info/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4933 2023-07-13 10:26:11.000000 ckanext-editable-config-0.0.2/ckanext_editable_config.egg-info/PKG-INFO
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1703 2023-07-13 10:26:11.000000 ckanext-editable-config-0.0.2/ckanext_editable_config.egg-info/SOURCES.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)        1 2023-07-13 10:26:11.000000 ckanext-editable-config-0.0.2/ckanext_editable_config.egg-info/dependency_links.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)      142 2023-07-13 10:26:11.000000 ckanext-editable-config-0.0.2/ckanext_editable_config.egg-info/entry_points.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)        8 2023-07-13 10:26:11.000000 ckanext-editable-config-0.0.2/ckanext_editable_config.egg-info/namespace_packages.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)        8 2023-07-13 10:26:11.000000 ckanext-editable-config-0.0.2/ckanext_editable_config.egg-info/top_level.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4324 2023-06-18 20:58:41.000000 ckanext-editable-config-0.0.2/pyproject.toml
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2023-06-18 11:13:48.000000 ckanext-editable-config-0.0.2/requirements.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1691 2023-07-13 10:26:11.137951 ckanext-editable-config-0.0.2/setup.cfg
--rw-r--r--   0 sergey    (1000) sergey    (1000)      505 2023-06-18 19:08:08.000000 ckanext-editable-config-0.0.2/setup.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-07-13 11:05:40.366833 ckanext-editable-config-0.0.3/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    34500 2023-06-18 11:13:48.000000 ckanext-editable-config-0.0.3/LICENSE
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      215 2023-06-18 11:13:48.000000 ckanext-editable-config-0.0.3/MANIFEST.in
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4933 2023-07-13 11:05:40.366833 ckanext-editable-config-0.0.3/PKG-INFO
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4345 2023-06-19 21:13:09.000000 ckanext-editable-config-0.0.3/README.md
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-07-13 11:05:40.356833 ckanext-editable-config-0.0.3/ckanext/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      202 2023-06-18 20:14:29.000000 ckanext-editable-config-0.0.3/ckanext/__init__.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-07-13 11:05:40.356833 ckanext-editable-config-0.0.3/ckanext/editable_config/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2023-06-18 11:13:48.000000 ckanext-editable-config-0.0.3/ckanext/editable_config/__init__.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-07-13 11:05:40.366833 ckanext-editable-config-0.0.3/ckanext/editable_config/assets/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      167 2023-06-18 11:13:48.000000 ckanext-editable-config-0.0.3/ckanext/editable_config/assets/script.js
+-rw-r--r--   0 sergey    (1000) sergey    (1000)       35 2023-06-18 11:13:48.000000 ckanext-editable-config-0.0.3/ckanext/editable_config/assets/style.css
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      359 2023-06-18 11:13:48.000000 ckanext-editable-config-0.0.3/ckanext/editable_config/assets/webassets.yml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      451 2023-06-19 12:53:41.000000 ckanext-editable-config-0.0.3/ckanext/editable_config/config.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      200 2023-07-13 11:05:24.000000 ckanext-editable-config-0.0.3/ckanext/editable_config/helpers.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-07-13 11:05:40.366833 ckanext-editable-config-0.0.3/ckanext/editable_config/logic/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2023-06-18 11:15:55.000000 ckanext-editable-config-0.0.3/ckanext/editable_config/logic/__init__.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     6037 2023-07-07 13:06:54.000000 ckanext-editable-config-0.0.3/ckanext/editable_config/logic/action.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1589 2023-06-19 10:13:19.000000 ckanext-editable-config-0.0.3/ckanext/editable_config/logic/auth.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2719 2023-06-19 20:17:49.000000 ckanext-editable-config-0.0.3/ckanext/editable_config/logic/schema.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2023-06-18 11:16:21.000000 ckanext-editable-config-0.0.3/ckanext/editable_config/logic/validators.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-07-13 11:05:40.356833 ckanext-editable-config-0.0.3/ckanext/editable_config/migration/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-07-13 11:05:40.366833 ckanext-editable-config-0.0.3/ckanext/editable_config/migration/editable_config/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1834 2023-06-18 15:19:17.000000 ckanext-editable-config-0.0.3/ckanext/editable_config/migration/editable_config/alembic.ini
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2148 2023-06-18 20:14:29.000000 ckanext-editable-config-0.0.3/ckanext/editable_config/migration/editable_config/env.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      494 2023-06-18 15:19:17.000000 ckanext-editable-config-0.0.3/ckanext/editable_config/migration/editable_config/script.py.mako
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-07-13 11:05:40.366833 ckanext-editable-config-0.0.3/ckanext/editable_config/migration/editable_config/versions/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      655 2023-06-18 19:08:06.000000 ckanext-editable-config-0.0.3/ckanext/editable_config/migration/editable_config/versions/a8d116986c3f_create_editable_config_table.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-07-13 11:05:40.366833 ckanext-editable-config-0.0.3/ckanext/editable_config/model/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)       49 2023-06-18 19:08:06.000000 ckanext-editable-config-0.0.3/ckanext/editable_config/model/__init__.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1859 2023-06-19 13:13:22.000000 ckanext-editable-config-0.0.3/ckanext/editable_config/model/option.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4170 2023-07-13 11:05:24.000000 ckanext-editable-config-0.0.3/ckanext/editable_config/plugin.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2605 2023-06-19 20:17:42.000000 ckanext-editable-config-0.0.3/ckanext/editable_config/shared.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-07-13 11:05:40.356833 ckanext-editable-config-0.0.3/ckanext/editable_config/templates/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-07-13 11:05:40.366833 ckanext-editable-config-0.0.3/ckanext/editable_config/templates/admin/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      399 2023-07-13 11:05:24.000000 ckanext-editable-config-0.0.3/ckanext/editable_config/templates/admin/base.html
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-07-13 11:05:40.366833 ckanext-editable-config-0.0.3/ckanext/editable_config/tests/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2023-06-18 11:13:48.000000 ckanext-editable-config-0.0.3/ckanext/editable_config/tests/__init__.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1254 2023-06-19 20:17:49.000000 ckanext-editable-config-0.0.3/ckanext/editable_config/tests/conftest.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-07-13 11:05:40.366833 ckanext-editable-config-0.0.3/ckanext/editable_config/tests/logic/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2023-06-18 20:35:03.000000 ckanext-editable-config-0.0.3/ckanext/editable_config/tests/logic/__init__.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4430 2023-06-19 20:17:49.000000 ckanext-editable-config-0.0.3/ckanext/editable_config/tests/logic/test_action.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      750 2023-06-19 12:49:49.000000 ckanext-editable-config-0.0.3/ckanext/editable_config/tests/logic/test_schema.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-07-13 11:05:40.366833 ckanext-editable-config-0.0.3/ckanext/editable_config/tests/model/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2023-06-18 21:22:56.000000 ckanext-editable-config-0.0.3/ckanext/editable_config/tests/model/__init__.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3473 2023-06-19 20:17:49.000000 ckanext-editable-config-0.0.3/ckanext/editable_config/tests/model/test_option.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1609 2023-06-19 20:17:42.000000 ckanext-editable-config-0.0.3/ckanext/editable_config/tests/test_fixtures.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2023-06-18 19:08:32.000000 ckanext-editable-config-0.0.3/ckanext/editable_config/tests/test_plugin.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2911 2023-06-19 20:17:47.000000 ckanext-editable-config-0.0.3/ckanext/editable_config/tests/test_shared.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-07-13 11:05:40.366833 ckanext-editable-config-0.0.3/ckanext_editable_config.egg-info/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4933 2023-07-13 11:05:40.000000 ckanext-editable-config-0.0.3/ckanext_editable_config.egg-info/PKG-INFO
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1788 2023-07-13 11:05:40.000000 ckanext-editable-config-0.0.3/ckanext_editable_config.egg-info/SOURCES.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        1 2023-07-13 11:05:40.000000 ckanext-editable-config-0.0.3/ckanext_editable_config.egg-info/dependency_links.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      142 2023-07-13 11:05:40.000000 ckanext-editable-config-0.0.3/ckanext_editable_config.egg-info/entry_points.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        8 2023-07-13 11:05:40.000000 ckanext-editable-config-0.0.3/ckanext_editable_config.egg-info/namespace_packages.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        8 2023-07-13 11:05:40.000000 ckanext-editable-config-0.0.3/ckanext_editable_config.egg-info/top_level.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4324 2023-06-18 20:58:41.000000 ckanext-editable-config-0.0.3/pyproject.toml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2023-06-18 11:13:48.000000 ckanext-editable-config-0.0.3/requirements.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1691 2023-07-13 11:05:40.366833 ckanext-editable-config-0.0.3/setup.cfg
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      505 2023-06-18 19:08:08.000000 ckanext-editable-config-0.0.3/setup.py
```

### Comparing `ckanext-editable-config-0.0.2/LICENSE` & `ckanext-editable-config-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ckanext-editable-config-0.0.2/PKG-INFO` & `ckanext-editable-config-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ckanext-editable-config
-Version: 0.0.2
+Version: 0.0.3
 Home-page: https://github.com/DataShades/ckanext-editable-config
 Author: Sergey Motornyuk
 Author-email: sergey.motornyuk@linkdigital.com.au
 License: AGPL
 Keywords: CKAN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
```

### Comparing `ckanext-editable-config-0.0.2/README.md` & `ckanext-editable-config-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `ckanext-editable-config-0.0.2/ckanext/editable_config/logic/action.py` & `ckanext-editable-config-0.0.3/ckanext/editable_config/logic/action.py`

 * *Files identical despite different names*

### Comparing `ckanext-editable-config-0.0.2/ckanext/editable_config/logic/auth.py` & `ckanext-editable-config-0.0.3/ckanext/editable_config/logic/auth.py`

 * *Files identical despite different names*

### Comparing `ckanext-editable-config-0.0.2/ckanext/editable_config/logic/schema.py` & `ckanext-editable-config-0.0.3/ckanext/editable_config/logic/schema.py`

 * *Files identical despite different names*

### Comparing `ckanext-editable-config-0.0.2/ckanext/editable_config/migration/editable_config/alembic.ini` & `ckanext-editable-config-0.0.3/ckanext/editable_config/migration/editable_config/alembic.ini`

 * *Files identical despite different names*

### Comparing `ckanext-editable-config-0.0.2/ckanext/editable_config/migration/editable_config/env.py` & `ckanext-editable-config-0.0.3/ckanext/editable_config/migration/editable_config/env.py`

 * *Files identical despite different names*

### Comparing `ckanext-editable-config-0.0.2/ckanext/editable_config/migration/editable_config/versions/a8d116986c3f_create_editable_config_table.py` & `ckanext-editable-config-0.0.3/ckanext/editable_config/migration/editable_config/versions/a8d116986c3f_create_editable_config_table.py`

 * *Files identical despite different names*

### Comparing `ckanext-editable-config-0.0.2/ckanext/editable_config/model/option.py` & `ckanext-editable-config-0.0.3/ckanext/editable_config/model/option.py`

 * *Files identical despite different names*

### Comparing `ckanext-editable-config-0.0.2/ckanext/editable_config/plugin.py` & `ckanext-editable-config-0.0.3/ckanext/editable_config/plugin.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,23 +8,25 @@
 
 import ckan.plugins.toolkit as tk
 from ckan import model, plugins, types
 from ckan.common import CKANConfig
 from ckan.common import config_declaration as cd
 from ckan.config.declaration import Key
 from ckan.config.declaration.option import Flag
+from ckan.logic import clear_actions_cache
 
 from . import config, shared
 
 log = logging.getLogger(__name__)
 ENVVAR_DISABLE = "CKANEXT_EDITABLE_CONFIG_DISABLE"
 
 
 @tk.blanket.config_declarations
 @tk.blanket.actions
+@tk.blanket.helpers
 @tk.blanket.auth_functions
 class EditableConfigPlugin(plugins.SingletonPlugin):
     plugins.implements(plugins.IConfigurer, inherit=True)
     plugins.implements(plugins.IConfigurable, inherit=True)
     plugins.implements(plugins.IMiddleware, inherit=True)
     plugins.implements(plugins.IConfigDeclaration, inherit=True)
 
@@ -37,14 +39,16 @@
         return app
 
     def _apply_overrides(self):
         shared.apply_config_overrides()
 
     # IConfigurer
     def update_config(self, config_: CKANConfig):
+        tk.add_template_directory(config_, "templates")
+
         self._update_editable_flag(config.extra_editable(), True)
         self._update_editable_flag(config.blacklist(), False)
 
         if whitelist := config.whitelist():
             for key in cd.iter_options():
                 if key in whitelist:
                     continue
@@ -83,13 +87,42 @@
         stmt = sa.select(model.SystemInfo.key)
         legacy_modified: Iterable[str] = model.Session.scalars(stmt)
         editable = {
             str(op) for op in cd.iter_options() if cd[op].has_flag(Flag.editable)
         }
 
         if problems := (set(legacy_modified) & editable):
-            log.warning(
-                "Modification via core AdminUI will produce undefined behavior: %s",
-                problems,
-            )
+            if tk.config["ckanext.editable_config.convert_core_overrides"]:
+                self._convert_core_overrides(problems)
+            else:
+                log.warning(
+                    "Modification via core AdminUI will cause undefined behavior: %s",
+                    problems,
+                )
 
         shared.apply_config_overrides()
+
+    def _convert_core_overrides(self, names: Iterable[str]):
+        clear_actions_cache()
+        try:
+            change = tk.get_action("editable_config_change")
+        except KeyError:
+            log.debug("Do not convert core overrides because plugin is not loaded yet")
+            return
+
+        q = model.Session.query(model.SystemInfo).filter(
+            model.SystemInfo.key.in_(names)
+        )
+        options = {
+            op.key: op.value
+            for op in
+            q
+        }
+
+        log.debug("Convert core overrides into editable config: %s", options)
+        change({"ignore_auth": True}, {
+            "apply": False,
+            "options": options,
+        })
+
+        q.delete()
+        model.Session.commit()
```

### Comparing `ckanext-editable-config-0.0.2/ckanext/editable_config/shared.py` & `ckanext-editable-config-0.0.3/ckanext/editable_config/shared.py`

 * *Files identical despite different names*

### Comparing `ckanext-editable-config-0.0.2/ckanext/editable_config/tests/conftest.py` & `ckanext-editable-config-0.0.3/ckanext/editable_config/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ckanext-editable-config-0.0.2/ckanext/editable_config/tests/logic/test_action.py` & `ckanext-editable-config-0.0.3/ckanext/editable_config/tests/logic/test_action.py`

 * *Files identical despite different names*

### Comparing `ckanext-editable-config-0.0.2/ckanext/editable_config/tests/logic/test_schema.py` & `ckanext-editable-config-0.0.3/ckanext/editable_config/tests/logic/test_schema.py`

 * *Files identical despite different names*

### Comparing `ckanext-editable-config-0.0.2/ckanext/editable_config/tests/model/test_option.py` & `ckanext-editable-config-0.0.3/ckanext/editable_config/tests/model/test_option.py`

 * *Files identical despite different names*

### Comparing `ckanext-editable-config-0.0.2/ckanext/editable_config/tests/test_fixtures.py` & `ckanext-editable-config-0.0.3/ckanext/editable_config/tests/test_fixtures.py`

 * *Files identical despite different names*

### Comparing `ckanext-editable-config-0.0.2/ckanext/editable_config/tests/test_shared.py` & `ckanext-editable-config-0.0.3/ckanext/editable_config/tests/test_shared.py`

 * *Files identical despite different names*

### Comparing `ckanext-editable-config-0.0.2/ckanext_editable_config.egg-info/PKG-INFO` & `ckanext-editable-config-0.0.3/ckanext_editable_config.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ckanext-editable-config
-Version: 0.0.2
+Version: 0.0.3
 Home-page: https://github.com/DataShades/ckanext-editable-config
 Author: Sergey Motornyuk
 Author-email: sergey.motornyuk@linkdigital.com.au
 License: AGPL
 Keywords: CKAN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
```

### Comparing `ckanext-editable-config-0.0.2/ckanext_editable_config.egg-info/SOURCES.txt` & `ckanext-editable-config-0.0.3/ckanext_editable_config.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 pyproject.toml
 requirements.txt
 setup.cfg
 setup.py
 ckanext/__init__.py
 ckanext/editable_config/__init__.py
 ckanext/editable_config/config.py
+ckanext/editable_config/helpers.py
 ckanext/editable_config/plugin.py
 ckanext/editable_config/shared.py
 ckanext/editable_config/assets/script.js
 ckanext/editable_config/assets/style.css
 ckanext/editable_config/assets/webassets.yml
 ckanext/editable_config/logic/__init__.py
 ckanext/editable_config/logic/action.py
@@ -20,14 +21,15 @@
 ckanext/editable_config/logic/validators.py
 ckanext/editable_config/migration/editable_config/alembic.ini
 ckanext/editable_config/migration/editable_config/env.py
 ckanext/editable_config/migration/editable_config/script.py.mako
 ckanext/editable_config/migration/editable_config/versions/a8d116986c3f_create_editable_config_table.py
 ckanext/editable_config/model/__init__.py
 ckanext/editable_config/model/option.py
+ckanext/editable_config/templates/admin/base.html
 ckanext/editable_config/tests/__init__.py
 ckanext/editable_config/tests/conftest.py
 ckanext/editable_config/tests/test_fixtures.py
 ckanext/editable_config/tests/test_plugin.py
 ckanext/editable_config/tests/test_shared.py
 ckanext/editable_config/tests/logic/__init__.py
 ckanext/editable_config/tests/logic/test_action.py
```

### Comparing `ckanext-editable-config-0.0.2/pyproject.toml` & `ckanext-editable-config-0.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ckanext-editable-config-0.0.2/setup.cfg` & `ckanext-editable-config-0.0.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ckanext-editable-config
-version = 0.0.2
+version = 0.0.3
 description = 
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/DataShades/ckanext-editable-config
 author = Sergey Motornyuk
 author_email = sergey.motornyuk@linkdigital.com.au
 license = AGPL
```

