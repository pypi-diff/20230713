# Comparing `tmp/netbox-secrets-1.8.4.tar.gz` & `tmp/netbox-secrets-1.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netbox-secrets-1.8.4.tar", last modified: Thu Jul 13 11:11:29 2023, max compression
+gzip compressed data, was "netbox-secrets-1.8.5.tar", last modified: Thu Jul 13 11:17:06 2023, max compression
```

## Comparing `netbox-secrets-1.8.4.tar` & `netbox-secrets-1.8.5.tar`

### file list

```diff
@@ -1,87 +1,87 @@
-drwxrwxr-x   0 asaharan  (1000) asaharan  (1000)        0 2023-07-13 11:11:29.821516 netbox-secrets-1.8.4/
--rw-rw-r--   0 asaharan  (1000) asaharan  (1000)    10174 2023-02-10 10:27:02.000000 netbox-secrets-1.8.4/LICENSE.md
--rw-rw-r--   0 asaharan  (1000) asaharan  (1000)      121 2023-02-10 10:27:02.000000 netbox-secrets-1.8.4/MANIFEST.in
--rw-rw-r--   0 asaharan  (1000) asaharan  (1000)      446 2023-07-13 11:11:29.821516 netbox-secrets-1.8.4/PKG-INFO
--rw-rw-r--   0 asaharan  (1000) asaharan  (1000)     4420 2023-07-13 11:09:59.000000 netbox-secrets-1.8.4/README.md
-drwxrwxr-x   0 asaharan  (1000) asaharan  (1000)        0 2023-07-13 11:11:29.821516 netbox-secrets-1.8.4/netbox_secrets/
--rw-rw-r--   0 asaharan  (1000) asaharan  (1000)     1723 2023-07-13 11:09:59.000000 netbox-secrets-1.8.4/netbox_secrets/__init__.py
--rw-rw-r--   0 asaharan  (1000) asaharan  (1000)     2620 2023-02-10 10:27:02.000000 netbox-secrets-1.8.4/netbox_secrets/admin.py
-drwxrwxr-x   0 asaharan  (1000) asaharan  (1000)        0 2023-07-13 11:11:29.821516 netbox-secrets-1.8.4/netbox_secrets/api/
--rw-rw-r--   0 asaharan  (1000) asaharan  (1000)        0 2023-02-10 10:27:02.000000 netbox-secrets-1.8.4/netbox_secrets/api/__init__.py
--rw-rw-r--   0 asaharan  (1000) asaharan  (1000)     1374 2023-07-13 11:09:59.000000 netbox-secrets-1.8.4/netbox_secrets/api/nested_serializers.py
--rw-rw-r--   0 asaharan  (1000) asaharan  (1000)     5078 2023-07-13 11:09:59.000000 netbox-secrets-1.8.4/netbox_secrets/api/serializers.py
--rw-rw-r--   0 asaharan  (1000) asaharan  (1000)      590 2023-07-13 11:09:59.000000 netbox-secrets-1.8.4/netbox_secrets/api/urls.py
--rw-rw-r--   0 asaharan  (1000) asaharan  (1000)    12415 2023-07-13 11:10:04.000000 netbox-secrets-1.8.4/netbox_secrets/api/views.py
--rw-rw-r--   0 asaharan  (1000) asaharan  (1000)      442 2023-07-13 11:09:59.000000 netbox-secrets-1.8.4/netbox_secrets/constants.py
--rw-rw-r--   0 asaharan  (1000) asaharan  (1000)       98 2023-02-10 10:27:02.000000 netbox-secrets-1.8.4/netbox_secrets/exceptions.py
--rw-rw-r--   0 asaharan  (1000) asaharan  (1000)     4628 2023-07-13 11:10:12.000000 netbox-secrets-1.8.4/netbox_secrets/filtersets.py
-drwxrwxr-x   0 asaharan  (1000) asaharan  (1000)        0 2023-07-13 11:11:29.821516 netbox-secrets-1.8.4/netbox_secrets/forms/
--rw-rw-r--   0 asaharan  (1000) asaharan  (1000)      136 2023-07-13 11:09:59.000000 netbox-secrets-1.8.4/netbox_secrets/forms/__init__.py
--rw-rw-r--   0 asaharan  (1000) asaharan  (1000)     1030 2023-07-13 11:09:59.000000 netbox-secrets-1.8.4/netbox_secrets/forms/bulk_edit.py
--rw-rw-r--   0 asaharan  (1000) asaharan  (1000)      322 2023-07-13 11:09:59.000000 netbox-secrets-1.8.4/netbox_secrets/forms/bulk_import.py
--rw-rw-r--   0 asaharan  (1000) asaharan  (1000)     1302 2023-07-13 11:10:12.000000 netbox-secrets-1.8.4/netbox_secrets/forms/filterset.py
--rw-rw-r--   0 asaharan  (1000) asaharan  (1000)     4392 2023-07-13 11:09:59.000000 netbox-secrets-1.8.4/netbox_secrets/forms/model_forms.py
-drwxrwxr-x   0 asaharan  (1000) asaharan  (1000)        0 2023-07-13 11:11:29.821516 netbox-secrets-1.8.4/netbox_secrets/graphql/
--rw-rw-r--   0 asaharan  (1000) asaharan  (1000)       29 2023-07-13 11:09:59.000000 netbox-secrets-1.8.4/netbox_secrets/graphql/__init__.py
--rw-rw-r--   0 asaharan  (1000) asaharan  (1000)      327 2023-02-10 10:27:02.000000 netbox-secrets-1.8.4/netbox_secrets/graphql/schema.py
--rw-rw-r--   0 asaharan  (1000) asaharan  (1000)      750 2023-07-13 11:09:59.000000 netbox-secrets-1.8.4/netbox_secrets/graphql/types.py
--rw-rw-r--   0 asaharan  (1000) asaharan  (1000)      387 2023-02-10 10:27:02.000000 netbox-secrets-1.8.4/netbox_secrets/hashers.py
-drwxrwxr-x   0 asaharan  (1000) asaharan  (1000)        0 2023-07-13 11:11:29.821516 netbox-secrets-1.8.4/netbox_secrets/migrations/
--rw-rw-r--   0 asaharan  (1000) asaharan  (1000)     4996 2023-02-10 10:27:02.000000 netbox-secrets-1.8.4/netbox_secrets/migrations/0001_initial.py
--rw-rw-r--   0 asaharan  (1000) asaharan  (1000)     1375 2023-07-13 11:09:59.000000 netbox-secrets-1.8.4/netbox_secrets/migrations/0002_populate_userkeys.py
--rw-rw-r--   0 asaharan  (1000) asaharan  (1000)     1485 2023-07-13 11:09:59.000000 netbox-secrets-1.8.4/netbox_secrets/migrations/0003_populate_secretroles.py
--rw-rw-r--   0 asaharan  (1000) asaharan  (1000)     3494 2023-07-13 11:09:59.000000 netbox-secrets-1.8.4/netbox_secrets/migrations/0004_populate_secrets.py
--rw-rw-r--   0 asaharan  (1000) asaharan  (1000)      708 2023-02-10 10:27:02.000000 netbox-secrets-1.8.4/netbox_secrets/migrations/0005_alter_secret_custom_field_data_and_more.py
--rw-rw-r--   0 asaharan  (1000) asaharan  (1000)      610 2023-02-10 10:27:02.000000 netbox-secrets-1.8.4/netbox_secrets/migrations/0006_alter_userkey_created_alter_userkey_last_updated.py
--rw-rw-r--   0 asaharan  (1000) asaharan  (1000)     1567 2023-07-13 11:10:12.000000 netbox-secrets-1.8.4/netbox_secrets/migrations/0007_secret__object_repr_secret_comments_and_more.py
--rw-rw-r--   0 asaharan  (1000) asaharan  (1000)        0 2023-02-10 10:27:02.000000 netbox-secrets-1.8.4/netbox_secrets/migrations/__init__.py
-drwxrwxr-x   0 asaharan  (1000) asaharan  (1000)        0 2023-07-13 11:11:29.821516 netbox-secrets-1.8.4/netbox_secrets/models/
--rw-rw-r--   0 asaharan  (1000) asaharan  (1000)       31 2023-07-13 11:09:59.000000 netbox-secrets-1.8.4/netbox_secrets/models/__init__.py
--rw-rw-r--   0 asaharan  (1000) asaharan  (1000)    14680 2023-07-13 11:09:59.000000 netbox-secrets-1.8.4/netbox_secrets/models/secrets.py
--rw-rw-r--   0 asaharan  (1000) asaharan  (1000)     1261 2023-02-10 10:27:02.000000 netbox-secrets-1.8.4/netbox_secrets/navigation.py
--rw-rw-r--   0 asaharan  (1000) asaharan  (1000)      333 2023-02-10 10:27:02.000000 netbox-secrets-1.8.4/netbox_secrets/querysets.py
-drwxrwxr-x   0 asaharan  (1000) asaharan  (1000)        0 2023-07-13 11:11:29.817516 netbox-secrets-1.8.4/netbox_secrets/static/
-drwxrwxr-x   0 asaharan  (1000) asaharan  (1000)        0 2023-07-13 11:11:29.821516 netbox-secrets-1.8.4/netbox_secrets/static/netbox_secrets/
--rw-rw-r--   0 asaharan  (1000) asaharan  (1000)     8341 2023-07-13 11:09:59.000000 netbox-secrets-1.8.4/netbox_secrets/static/netbox_secrets/secrets.js
--rw-rw-r--   0 asaharan  (1000) asaharan  (1000)    29495 2023-07-13 11:09:59.000000 netbox-secrets-1.8.4/netbox_secrets/static/netbox_secrets/secrets.js.map
--rw-rw-r--   0 asaharan  (1000) asaharan  (1000)     1934 2023-07-13 11:09:59.000000 netbox-secrets-1.8.4/netbox_secrets/tables.py
--rw-rw-r--   0 asaharan  (1000) asaharan  (1000)     3235 2023-07-13 11:09:59.000000 netbox-secrets-1.8.4/netbox_secrets/template_content.py
-drwxrwxr-x   0 asaharan  (1000) asaharan  (1000)        0 2023-07-13 11:11:29.817516 netbox-secrets-1.8.4/netbox_secrets/templates/
-drwxrwxr-x   0 asaharan  (1000) asaharan  (1000)        0 2023-07-13 11:11:29.821516 netbox-secrets-1.8.4/netbox_secrets/templates/netbox_secrets/
--rw-rw-r--   0 asaharan  (1000) asaharan  (1000)      297 2023-02-10 10:27:02.000000 netbox-secrets-1.8.4/netbox_secrets/templates/netbox_secrets/activate_keys.html
-drwxrwxr-x   0 asaharan  (1000) asaharan  (1000)        0 2023-07-13 11:11:29.821516 netbox-secrets-1.8.4/netbox_secrets/templates/netbox_secrets/inc/
--rw-rw-r--   0 asaharan  (1000) asaharan  (1000)     1594 2023-02-10 10:27:02.000000 netbox-secrets-1.8.4/netbox_secrets/templates/netbox_secrets/inc/private_key_modal.html
--rw-rw-r--   0 asaharan  (1000) asaharan  (1000)     1299 2023-02-10 10:27:02.000000 netbox-secrets-1.8.4/netbox_secrets/templates/netbox_secrets/inc/secret_actions.html
--rw-rw-r--   0 asaharan  (1000) asaharan  (1000)      328 2023-07-13 11:09:59.000000 netbox-secrets-1.8.4/netbox_secrets/templates/netbox_secrets/inc/secret_add_button.html
--rw-rw-r--   0 asaharan  (1000) asaharan  (1000)     1798 2023-07-13 11:09:59.000000 netbox-secrets-1.8.4/netbox_secrets/templates/netbox_secrets/inc/secrets_panel.html
--rw-rw-r--   0 asaharan  (1000) asaharan  (1000)      582 2023-02-10 10:27:02.000000 netbox-secrets-1.8.4/netbox_secrets/templates/netbox_secrets/inc/view_tab.html
--rw-rw-r--   0 asaharan  (1000) asaharan  (1000)     2633 2023-07-13 11:10:04.000000 netbox-secrets-1.8.4/netbox_secrets/templates/netbox_secrets/secret.html
--rw-rw-r--   0 asaharan  (1000) asaharan  (1000)      627 2023-07-13 11:09:59.000000 netbox-secrets-1.8.4/netbox_secrets/templates/netbox_secrets/secret_edit.html
--rw-rw-r--   0 asaharan  (1000) asaharan  (1000)     1883 2023-07-13 11:09:59.000000 netbox-secrets-1.8.4/netbox_secrets/templates/netbox_secrets/secretrole.html
--rw-rw-r--   0 asaharan  (1000) asaharan  (1000)     5510 2023-02-10 10:27:02.000000 netbox-secrets-1.8.4/netbox_secrets/templates/netbox_secrets/userkey.html
--rw-rw-r--   0 asaharan  (1000) asaharan  (1000)     4738 2023-02-10 10:27:02.000000 netbox-secrets-1.8.4/netbox_secrets/templates/netbox_secrets/userkey_edit.html
-drwxrwxr-x   0 asaharan  (1000) asaharan  (1000)        0 2023-07-13 11:11:29.821516 netbox-secrets-1.8.4/netbox_secrets/tests/
--rw-rw-r--   0 asaharan  (1000) asaharan  (1000)        0 2023-02-10 10:27:02.000000 netbox-secrets-1.8.4/netbox_secrets/tests/__init__.py
--rw-rw-r--   0 asaharan  (1000) asaharan  (1000)     2798 2023-07-13 11:09:59.000000 netbox-secrets-1.8.4/netbox_secrets/tests/constants.py
--rw-rw-r--   0 asaharan  (1000) asaharan  (1000)    11064 2023-07-13 11:09:59.000000 netbox-secrets-1.8.4/netbox_secrets/tests/test_api.py
--rw-rw-r--   0 asaharan  (1000) asaharan  (1000)     4436 2023-07-13 11:10:12.000000 netbox-secrets-1.8.4/netbox_secrets/tests/test_filters.py
--rw-rw-r--   0 asaharan  (1000) asaharan  (1000)      934 2023-02-10 10:27:02.000000 netbox-secrets-1.8.4/netbox_secrets/tests/test_form.py
--rw-rw-r--   0 asaharan  (1000) asaharan  (1000)     7464 2023-07-13 11:09:59.000000 netbox-secrets-1.8.4/netbox_secrets/tests/test_models.py
--rw-rw-r--   0 asaharan  (1000) asaharan  (1000)     4156 2023-02-10 10:27:02.000000 netbox-secrets-1.8.4/netbox_secrets/tests/test_views.py
--rw-rw-r--   0 asaharan  (1000) asaharan  (1000)     1408 2023-07-13 11:09:59.000000 netbox-secrets-1.8.4/netbox_secrets/urls.py
-drwxrwxr-x   0 asaharan  (1000) asaharan  (1000)        0 2023-07-13 11:11:29.821516 netbox-secrets-1.8.4/netbox_secrets/utils/
--rw-rw-r--   0 asaharan  (1000) asaharan  (1000)      162 2023-05-25 11:12:45.000000 netbox-secrets-1.8.4/netbox_secrets/utils/__init__.py
--rw-rw-r--   0 asaharan  (1000) asaharan  (1000)      863 2023-02-10 10:27:02.000000 netbox-secrets-1.8.4/netbox_secrets/utils/crypto.py
--rw-rw-r--   0 asaharan  (1000) asaharan  (1000)      387 2023-05-25 11:12:45.000000 netbox-secrets-1.8.4/netbox_secrets/utils/hashers.py
--rw-rw-r--   0 asaharan  (1000) asaharan  (1000)      408 2023-07-13 11:09:59.000000 netbox-secrets-1.8.4/netbox_secrets/utils/helpers.py
--rw-rw-r--   0 asaharan  (1000) asaharan  (1000)    13567 2023-07-13 11:10:04.000000 netbox-secrets-1.8.4/netbox_secrets/views.py
-drwxrwxr-x   0 asaharan  (1000) asaharan  (1000)        0 2023-07-13 11:11:29.821516 netbox-secrets-1.8.4/netbox_secrets.egg-info/
--rw-rw-r--   0 asaharan  (1000) asaharan  (1000)      446 2023-07-13 11:11:29.000000 netbox-secrets-1.8.4/netbox_secrets.egg-info/PKG-INFO
--rw-rw-r--   0 asaharan  (1000) asaharan  (1000)     2708 2023-07-13 11:11:29.000000 netbox-secrets-1.8.4/netbox_secrets.egg-info/SOURCES.txt
--rw-rw-r--   0 asaharan  (1000) asaharan  (1000)        1 2023-07-13 11:11:29.000000 netbox-secrets-1.8.4/netbox_secrets.egg-info/dependency_links.txt
--rw-rw-r--   0 asaharan  (1000) asaharan  (1000)        1 2023-02-10 10:27:25.000000 netbox-secrets-1.8.4/netbox_secrets.egg-info/not-zip-safe
--rw-rw-r--   0 asaharan  (1000) asaharan  (1000)       13 2023-07-13 11:11:29.000000 netbox-secrets-1.8.4/netbox_secrets.egg-info/requires.txt
--rw-rw-r--   0 asaharan  (1000) asaharan  (1000)       15 2023-07-13 11:11:29.000000 netbox-secrets-1.8.4/netbox_secrets.egg-info/top_level.txt
--rw-rw-r--   0 asaharan  (1000) asaharan  (1000)      424 2023-02-10 10:27:02.000000 netbox-secrets-1.8.4/pyproject.toml
--rw-rw-r--   0 asaharan  (1000) asaharan  (1000)       38 2023-07-13 11:11:29.821516 netbox-secrets-1.8.4/setup.cfg
--rw-rw-r--   0 asaharan  (1000) asaharan  (1000)      679 2023-07-13 11:11:14.000000 netbox-secrets-1.8.4/setup.py
+drwxrwxr-x   0 asaharan  (1000) asaharan  (1000)        0 2023-07-13 11:17:06.000672 netbox-secrets-1.8.5/
+-rw-rw-r--   0 asaharan  (1000) asaharan  (1000)    10174 2023-02-10 10:27:02.000000 netbox-secrets-1.8.5/LICENSE.md
+-rw-rw-r--   0 asaharan  (1000) asaharan  (1000)      121 2023-02-10 10:27:02.000000 netbox-secrets-1.8.5/MANIFEST.in
+-rw-rw-r--   0 asaharan  (1000) asaharan  (1000)      446 2023-07-13 11:17:06.000672 netbox-secrets-1.8.5/PKG-INFO
+-rw-rw-r--   0 asaharan  (1000) asaharan  (1000)     4420 2023-07-13 11:09:59.000000 netbox-secrets-1.8.5/README.md
+drwxrwxr-x   0 asaharan  (1000) asaharan  (1000)        0 2023-07-13 11:17:06.000672 netbox-secrets-1.8.5/netbox_secrets/
+-rw-rw-r--   0 asaharan  (1000) asaharan  (1000)     1723 2023-07-13 11:09:59.000000 netbox-secrets-1.8.5/netbox_secrets/__init__.py
+-rw-rw-r--   0 asaharan  (1000) asaharan  (1000)     2620 2023-02-10 10:27:02.000000 netbox-secrets-1.8.5/netbox_secrets/admin.py
+drwxrwxr-x   0 asaharan  (1000) asaharan  (1000)        0 2023-07-13 11:17:06.000672 netbox-secrets-1.8.5/netbox_secrets/api/
+-rw-rw-r--   0 asaharan  (1000) asaharan  (1000)        0 2023-02-10 10:27:02.000000 netbox-secrets-1.8.5/netbox_secrets/api/__init__.py
+-rw-rw-r--   0 asaharan  (1000) asaharan  (1000)     1374 2023-07-13 11:09:59.000000 netbox-secrets-1.8.5/netbox_secrets/api/nested_serializers.py
+-rw-rw-r--   0 asaharan  (1000) asaharan  (1000)     5078 2023-07-13 11:09:59.000000 netbox-secrets-1.8.5/netbox_secrets/api/serializers.py
+-rw-rw-r--   0 asaharan  (1000) asaharan  (1000)      590 2023-07-13 11:09:59.000000 netbox-secrets-1.8.5/netbox_secrets/api/urls.py
+-rw-rw-r--   0 asaharan  (1000) asaharan  (1000)    12415 2023-07-13 11:10:04.000000 netbox-secrets-1.8.5/netbox_secrets/api/views.py
+-rw-rw-r--   0 asaharan  (1000) asaharan  (1000)      442 2023-07-13 11:09:59.000000 netbox-secrets-1.8.5/netbox_secrets/constants.py
+-rw-rw-r--   0 asaharan  (1000) asaharan  (1000)       98 2023-02-10 10:27:02.000000 netbox-secrets-1.8.5/netbox_secrets/exceptions.py
+-rw-rw-r--   0 asaharan  (1000) asaharan  (1000)     4628 2023-07-13 11:10:12.000000 netbox-secrets-1.8.5/netbox_secrets/filtersets.py
+drwxrwxr-x   0 asaharan  (1000) asaharan  (1000)        0 2023-07-13 11:17:06.000672 netbox-secrets-1.8.5/netbox_secrets/forms/
+-rw-rw-r--   0 asaharan  (1000) asaharan  (1000)      136 2023-07-13 11:09:59.000000 netbox-secrets-1.8.5/netbox_secrets/forms/__init__.py
+-rw-rw-r--   0 asaharan  (1000) asaharan  (1000)     1030 2023-07-13 11:09:59.000000 netbox-secrets-1.8.5/netbox_secrets/forms/bulk_edit.py
+-rw-rw-r--   0 asaharan  (1000) asaharan  (1000)      322 2023-07-13 11:09:59.000000 netbox-secrets-1.8.5/netbox_secrets/forms/bulk_import.py
+-rw-rw-r--   0 asaharan  (1000) asaharan  (1000)     1302 2023-07-13 11:10:12.000000 netbox-secrets-1.8.5/netbox_secrets/forms/filterset.py
+-rw-rw-r--   0 asaharan  (1000) asaharan  (1000)     4392 2023-07-13 11:09:59.000000 netbox-secrets-1.8.5/netbox_secrets/forms/model_forms.py
+drwxrwxr-x   0 asaharan  (1000) asaharan  (1000)        0 2023-07-13 11:17:06.000672 netbox-secrets-1.8.5/netbox_secrets/graphql/
+-rw-rw-r--   0 asaharan  (1000) asaharan  (1000)       29 2023-07-13 11:09:59.000000 netbox-secrets-1.8.5/netbox_secrets/graphql/__init__.py
+-rw-rw-r--   0 asaharan  (1000) asaharan  (1000)      327 2023-02-10 10:27:02.000000 netbox-secrets-1.8.5/netbox_secrets/graphql/schema.py
+-rw-rw-r--   0 asaharan  (1000) asaharan  (1000)      750 2023-07-13 11:09:59.000000 netbox-secrets-1.8.5/netbox_secrets/graphql/types.py
+-rw-rw-r--   0 asaharan  (1000) asaharan  (1000)      387 2023-02-10 10:27:02.000000 netbox-secrets-1.8.5/netbox_secrets/hashers.py
+drwxrwxr-x   0 asaharan  (1000) asaharan  (1000)        0 2023-07-13 11:17:06.000672 netbox-secrets-1.8.5/netbox_secrets/migrations/
+-rw-rw-r--   0 asaharan  (1000) asaharan  (1000)     4996 2023-02-10 10:27:02.000000 netbox-secrets-1.8.5/netbox_secrets/migrations/0001_initial.py
+-rw-rw-r--   0 asaharan  (1000) asaharan  (1000)     1375 2023-07-13 11:09:59.000000 netbox-secrets-1.8.5/netbox_secrets/migrations/0002_populate_userkeys.py
+-rw-rw-r--   0 asaharan  (1000) asaharan  (1000)     1485 2023-07-13 11:09:59.000000 netbox-secrets-1.8.5/netbox_secrets/migrations/0003_populate_secretroles.py
+-rw-rw-r--   0 asaharan  (1000) asaharan  (1000)     3494 2023-07-13 11:09:59.000000 netbox-secrets-1.8.5/netbox_secrets/migrations/0004_populate_secrets.py
+-rw-rw-r--   0 asaharan  (1000) asaharan  (1000)      708 2023-02-10 10:27:02.000000 netbox-secrets-1.8.5/netbox_secrets/migrations/0005_alter_secret_custom_field_data_and_more.py
+-rw-rw-r--   0 asaharan  (1000) asaharan  (1000)      610 2023-02-10 10:27:02.000000 netbox-secrets-1.8.5/netbox_secrets/migrations/0006_alter_userkey_created_alter_userkey_last_updated.py
+-rw-rw-r--   0 asaharan  (1000) asaharan  (1000)     1555 2023-07-13 11:16:26.000000 netbox-secrets-1.8.5/netbox_secrets/migrations/0007_secret__object_repr_secret_comments_and_more.py
+-rw-rw-r--   0 asaharan  (1000) asaharan  (1000)        0 2023-02-10 10:27:02.000000 netbox-secrets-1.8.5/netbox_secrets/migrations/__init__.py
+drwxrwxr-x   0 asaharan  (1000) asaharan  (1000)        0 2023-07-13 11:17:06.000672 netbox-secrets-1.8.5/netbox_secrets/models/
+-rw-rw-r--   0 asaharan  (1000) asaharan  (1000)       31 2023-07-13 11:09:59.000000 netbox-secrets-1.8.5/netbox_secrets/models/__init__.py
+-rw-rw-r--   0 asaharan  (1000) asaharan  (1000)    14680 2023-07-13 11:09:59.000000 netbox-secrets-1.8.5/netbox_secrets/models/secrets.py
+-rw-rw-r--   0 asaharan  (1000) asaharan  (1000)     1261 2023-02-10 10:27:02.000000 netbox-secrets-1.8.5/netbox_secrets/navigation.py
+-rw-rw-r--   0 asaharan  (1000) asaharan  (1000)      333 2023-02-10 10:27:02.000000 netbox-secrets-1.8.5/netbox_secrets/querysets.py
+drwxrwxr-x   0 asaharan  (1000) asaharan  (1000)        0 2023-07-13 11:17:05.996673 netbox-secrets-1.8.5/netbox_secrets/static/
+drwxrwxr-x   0 asaharan  (1000) asaharan  (1000)        0 2023-07-13 11:17:06.000672 netbox-secrets-1.8.5/netbox_secrets/static/netbox_secrets/
+-rw-rw-r--   0 asaharan  (1000) asaharan  (1000)     8341 2023-07-13 11:09:59.000000 netbox-secrets-1.8.5/netbox_secrets/static/netbox_secrets/secrets.js
+-rw-rw-r--   0 asaharan  (1000) asaharan  (1000)    29495 2023-07-13 11:09:59.000000 netbox-secrets-1.8.5/netbox_secrets/static/netbox_secrets/secrets.js.map
+-rw-rw-r--   0 asaharan  (1000) asaharan  (1000)     1934 2023-07-13 11:09:59.000000 netbox-secrets-1.8.5/netbox_secrets/tables.py
+-rw-rw-r--   0 asaharan  (1000) asaharan  (1000)     3235 2023-07-13 11:09:59.000000 netbox-secrets-1.8.5/netbox_secrets/template_content.py
+drwxrwxr-x   0 asaharan  (1000) asaharan  (1000)        0 2023-07-13 11:17:05.996673 netbox-secrets-1.8.5/netbox_secrets/templates/
+drwxrwxr-x   0 asaharan  (1000) asaharan  (1000)        0 2023-07-13 11:17:06.000672 netbox-secrets-1.8.5/netbox_secrets/templates/netbox_secrets/
+-rw-rw-r--   0 asaharan  (1000) asaharan  (1000)      297 2023-02-10 10:27:02.000000 netbox-secrets-1.8.5/netbox_secrets/templates/netbox_secrets/activate_keys.html
+drwxrwxr-x   0 asaharan  (1000) asaharan  (1000)        0 2023-07-13 11:17:06.000672 netbox-secrets-1.8.5/netbox_secrets/templates/netbox_secrets/inc/
+-rw-rw-r--   0 asaharan  (1000) asaharan  (1000)     1594 2023-02-10 10:27:02.000000 netbox-secrets-1.8.5/netbox_secrets/templates/netbox_secrets/inc/private_key_modal.html
+-rw-rw-r--   0 asaharan  (1000) asaharan  (1000)     1299 2023-02-10 10:27:02.000000 netbox-secrets-1.8.5/netbox_secrets/templates/netbox_secrets/inc/secret_actions.html
+-rw-rw-r--   0 asaharan  (1000) asaharan  (1000)      328 2023-07-13 11:09:59.000000 netbox-secrets-1.8.5/netbox_secrets/templates/netbox_secrets/inc/secret_add_button.html
+-rw-rw-r--   0 asaharan  (1000) asaharan  (1000)     1798 2023-07-13 11:09:59.000000 netbox-secrets-1.8.5/netbox_secrets/templates/netbox_secrets/inc/secrets_panel.html
+-rw-rw-r--   0 asaharan  (1000) asaharan  (1000)      582 2023-02-10 10:27:02.000000 netbox-secrets-1.8.5/netbox_secrets/templates/netbox_secrets/inc/view_tab.html
+-rw-rw-r--   0 asaharan  (1000) asaharan  (1000)     2633 2023-07-13 11:10:04.000000 netbox-secrets-1.8.5/netbox_secrets/templates/netbox_secrets/secret.html
+-rw-rw-r--   0 asaharan  (1000) asaharan  (1000)      627 2023-07-13 11:09:59.000000 netbox-secrets-1.8.5/netbox_secrets/templates/netbox_secrets/secret_edit.html
+-rw-rw-r--   0 asaharan  (1000) asaharan  (1000)     1883 2023-07-13 11:09:59.000000 netbox-secrets-1.8.5/netbox_secrets/templates/netbox_secrets/secretrole.html
+-rw-rw-r--   0 asaharan  (1000) asaharan  (1000)     5510 2023-02-10 10:27:02.000000 netbox-secrets-1.8.5/netbox_secrets/templates/netbox_secrets/userkey.html
+-rw-rw-r--   0 asaharan  (1000) asaharan  (1000)     4738 2023-02-10 10:27:02.000000 netbox-secrets-1.8.5/netbox_secrets/templates/netbox_secrets/userkey_edit.html
+drwxrwxr-x   0 asaharan  (1000) asaharan  (1000)        0 2023-07-13 11:17:06.000672 netbox-secrets-1.8.5/netbox_secrets/tests/
+-rw-rw-r--   0 asaharan  (1000) asaharan  (1000)        0 2023-02-10 10:27:02.000000 netbox-secrets-1.8.5/netbox_secrets/tests/__init__.py
+-rw-rw-r--   0 asaharan  (1000) asaharan  (1000)     2798 2023-07-13 11:09:59.000000 netbox-secrets-1.8.5/netbox_secrets/tests/constants.py
+-rw-rw-r--   0 asaharan  (1000) asaharan  (1000)    11064 2023-07-13 11:09:59.000000 netbox-secrets-1.8.5/netbox_secrets/tests/test_api.py
+-rw-rw-r--   0 asaharan  (1000) asaharan  (1000)     4436 2023-07-13 11:10:12.000000 netbox-secrets-1.8.5/netbox_secrets/tests/test_filters.py
+-rw-rw-r--   0 asaharan  (1000) asaharan  (1000)      934 2023-02-10 10:27:02.000000 netbox-secrets-1.8.5/netbox_secrets/tests/test_form.py
+-rw-rw-r--   0 asaharan  (1000) asaharan  (1000)     7464 2023-07-13 11:09:59.000000 netbox-secrets-1.8.5/netbox_secrets/tests/test_models.py
+-rw-rw-r--   0 asaharan  (1000) asaharan  (1000)     4156 2023-02-10 10:27:02.000000 netbox-secrets-1.8.5/netbox_secrets/tests/test_views.py
+-rw-rw-r--   0 asaharan  (1000) asaharan  (1000)     1408 2023-07-13 11:09:59.000000 netbox-secrets-1.8.5/netbox_secrets/urls.py
+drwxrwxr-x   0 asaharan  (1000) asaharan  (1000)        0 2023-07-13 11:17:06.000672 netbox-secrets-1.8.5/netbox_secrets/utils/
+-rw-rw-r--   0 asaharan  (1000) asaharan  (1000)      162 2023-05-25 11:12:45.000000 netbox-secrets-1.8.5/netbox_secrets/utils/__init__.py
+-rw-rw-r--   0 asaharan  (1000) asaharan  (1000)      863 2023-02-10 10:27:02.000000 netbox-secrets-1.8.5/netbox_secrets/utils/crypto.py
+-rw-rw-r--   0 asaharan  (1000) asaharan  (1000)      387 2023-05-25 11:12:45.000000 netbox-secrets-1.8.5/netbox_secrets/utils/hashers.py
+-rw-rw-r--   0 asaharan  (1000) asaharan  (1000)      408 2023-07-13 11:09:59.000000 netbox-secrets-1.8.5/netbox_secrets/utils/helpers.py
+-rw-rw-r--   0 asaharan  (1000) asaharan  (1000)    13567 2023-07-13 11:10:04.000000 netbox-secrets-1.8.5/netbox_secrets/views.py
+drwxrwxr-x   0 asaharan  (1000) asaharan  (1000)        0 2023-07-13 11:17:06.000672 netbox-secrets-1.8.5/netbox_secrets.egg-info/
+-rw-rw-r--   0 asaharan  (1000) asaharan  (1000)      446 2023-07-13 11:17:05.000000 netbox-secrets-1.8.5/netbox_secrets.egg-info/PKG-INFO
+-rw-rw-r--   0 asaharan  (1000) asaharan  (1000)     2708 2023-07-13 11:17:05.000000 netbox-secrets-1.8.5/netbox_secrets.egg-info/SOURCES.txt
+-rw-rw-r--   0 asaharan  (1000) asaharan  (1000)        1 2023-07-13 11:17:05.000000 netbox-secrets-1.8.5/netbox_secrets.egg-info/dependency_links.txt
+-rw-rw-r--   0 asaharan  (1000) asaharan  (1000)        1 2023-02-10 10:27:25.000000 netbox-secrets-1.8.5/netbox_secrets.egg-info/not-zip-safe
+-rw-rw-r--   0 asaharan  (1000) asaharan  (1000)       13 2023-07-13 11:17:05.000000 netbox-secrets-1.8.5/netbox_secrets.egg-info/requires.txt
+-rw-rw-r--   0 asaharan  (1000) asaharan  (1000)       15 2023-07-13 11:17:05.000000 netbox-secrets-1.8.5/netbox_secrets.egg-info/top_level.txt
+-rw-rw-r--   0 asaharan  (1000) asaharan  (1000)      424 2023-02-10 10:27:02.000000 netbox-secrets-1.8.5/pyproject.toml
+-rw-rw-r--   0 asaharan  (1000) asaharan  (1000)       38 2023-07-13 11:17:06.000672 netbox-secrets-1.8.5/setup.cfg
+-rw-rw-r--   0 asaharan  (1000) asaharan  (1000)      679 2023-07-13 11:17:02.000000 netbox-secrets-1.8.5/setup.py
```

### Comparing `netbox-secrets-1.8.4/LICENSE.md` & `netbox-secrets-1.8.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `netbox-secrets-1.8.4/README.md` & `netbox-secrets-1.8.5/README.md`

 * *Files identical despite different names*

### Comparing `netbox-secrets-1.8.4/netbox_secrets/__init__.py` & `netbox-secrets-1.8.5/netbox_secrets/__init__.py`

 * *Files identical despite different names*

### Comparing `netbox-secrets-1.8.4/netbox_secrets/admin.py` & `netbox-secrets-1.8.5/netbox_secrets/admin.py`

 * *Files identical despite different names*

### Comparing `netbox-secrets-1.8.4/netbox_secrets/api/nested_serializers.py` & `netbox-secrets-1.8.5/netbox_secrets/api/nested_serializers.py`

 * *Files identical despite different names*

### Comparing `netbox-secrets-1.8.4/netbox_secrets/api/serializers.py` & `netbox-secrets-1.8.5/netbox_secrets/api/serializers.py`

 * *Files identical despite different names*

### Comparing `netbox-secrets-1.8.4/netbox_secrets/api/urls.py` & `netbox-secrets-1.8.5/netbox_secrets/api/urls.py`

 * *Files identical despite different names*

### Comparing `netbox-secrets-1.8.4/netbox_secrets/api/views.py` & `netbox-secrets-1.8.5/netbox_secrets/api/views.py`

 * *Files identical despite different names*

### Comparing `netbox-secrets-1.8.4/netbox_secrets/filtersets.py` & `netbox-secrets-1.8.5/netbox_secrets/filtersets.py`

 * *Files identical despite different names*

### Comparing `netbox-secrets-1.8.4/netbox_secrets/forms/bulk_edit.py` & `netbox-secrets-1.8.5/netbox_secrets/forms/bulk_edit.py`

 * *Files identical despite different names*

### Comparing `netbox-secrets-1.8.4/netbox_secrets/forms/filterset.py` & `netbox-secrets-1.8.5/netbox_secrets/forms/filterset.py`

 * *Files identical despite different names*

### Comparing `netbox-secrets-1.8.4/netbox_secrets/forms/model_forms.py` & `netbox-secrets-1.8.5/netbox_secrets/forms/model_forms.py`

 * *Files identical despite different names*

### Comparing `netbox-secrets-1.8.4/netbox_secrets/graphql/types.py` & `netbox-secrets-1.8.5/netbox_secrets/graphql/types.py`

 * *Files identical despite different names*

### Comparing `netbox-secrets-1.8.4/netbox_secrets/migrations/0001_initial.py` & `netbox-secrets-1.8.5/netbox_secrets/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `netbox-secrets-1.8.4/netbox_secrets/migrations/0002_populate_userkeys.py` & `netbox-secrets-1.8.5/netbox_secrets/migrations/0002_populate_userkeys.py`

 * *Files identical despite different names*

### Comparing `netbox-secrets-1.8.4/netbox_secrets/migrations/0003_populate_secretroles.py` & `netbox-secrets-1.8.5/netbox_secrets/migrations/0003_populate_secretroles.py`

 * *Files identical despite different names*

### Comparing `netbox-secrets-1.8.4/netbox_secrets/migrations/0004_populate_secrets.py` & `netbox-secrets-1.8.5/netbox_secrets/migrations/0004_populate_secrets.py`

 * *Files identical despite different names*

### Comparing `netbox-secrets-1.8.4/netbox_secrets/migrations/0005_alter_secret_custom_field_data_and_more.py` & `netbox-secrets-1.8.5/netbox_secrets/migrations/0005_alter_secret_custom_field_data_and_more.py`

 * *Files identical despite different names*

### Comparing `netbox-secrets-1.8.4/netbox_secrets/migrations/0006_alter_userkey_created_alter_userkey_last_updated.py` & `netbox-secrets-1.8.5/netbox_secrets/migrations/0006_alter_userkey_created_alter_userkey_last_updated.py`

 * *Files identical despite different names*

### Comparing `netbox-secrets-1.8.4/netbox_secrets/migrations/0007_secret__object_repr_secret_comments_and_more.py` & `netbox-secrets-1.8.5/netbox_secrets/migrations/0007_secret__object_repr_secret_comments_and_more.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,23 +2,24 @@
 
 from django.contrib.contenttypes.models import ContentType
 from django.db import migrations, models
 
 
 def copy_assigned_object(apps, schema_editor):
     Secret = apps.get_model('netbox_secrets', 'Secret')
-    try:
-        for secret in Secret.objects.all():
-            content_type = ContentType.objects.get(id=secret.assigned_object_type_id)
-            Model = apps.get_model(content_type.app_label, str(content_type.model).capitalize())
-            object = Model.objects.filter(id=secret.assigned_object_id).first()
-            secret._object_repr = object.name
-            secret.save()
-    except:
-        pass
+    for secret in Secret.objects.all():
+        content_type = ContentType.objects.get(id=secret.assigned_object_type_id)
+        Model = apps.get_model(content_type.app_label, str(content_type.model).capitalize())
+        object = Model.objects.filter(id=secret.assigned_object_id).first()
+        if not object:
+            continue
+        secret._object_repr = object.name
+        secret.save()
+
+
 
 
 class Migration(migrations.Migration):
     dependencies = [
         ('netbox_secrets', '0006_alter_userkey_created_alter_userkey_last_updated'),
     ]
```

### Comparing `netbox-secrets-1.8.4/netbox_secrets/models/secrets.py` & `netbox-secrets-1.8.5/netbox_secrets/models/secrets.py`

 * *Files identical despite different names*

### Comparing `netbox-secrets-1.8.4/netbox_secrets/navigation.py` & `netbox-secrets-1.8.5/netbox_secrets/navigation.py`

 * *Files identical despite different names*

### Comparing `netbox-secrets-1.8.4/netbox_secrets/static/netbox_secrets/secrets.js` & `netbox-secrets-1.8.5/netbox_secrets/static/netbox_secrets/secrets.js`

 * *Files identical despite different names*

### Comparing `netbox-secrets-1.8.4/netbox_secrets/static/netbox_secrets/secrets.js.map` & `netbox-secrets-1.8.5/netbox_secrets/static/netbox_secrets/secrets.js.map`

 * *Files identical despite different names*

### Comparing `netbox-secrets-1.8.4/netbox_secrets/tables.py` & `netbox-secrets-1.8.5/netbox_secrets/tables.py`

 * *Files identical despite different names*

### Comparing `netbox-secrets-1.8.4/netbox_secrets/template_content.py` & `netbox-secrets-1.8.5/netbox_secrets/template_content.py`

 * *Files identical despite different names*

### Comparing `netbox-secrets-1.8.4/netbox_secrets/templates/netbox_secrets/inc/private_key_modal.html` & `netbox-secrets-1.8.5/netbox_secrets/templates/netbox_secrets/inc/private_key_modal.html`

 * *Files identical despite different names*

### Comparing `netbox-secrets-1.8.4/netbox_secrets/templates/netbox_secrets/inc/secret_actions.html` & `netbox-secrets-1.8.5/netbox_secrets/templates/netbox_secrets/inc/secret_actions.html`

 * *Files identical despite different names*

### Comparing `netbox-secrets-1.8.4/netbox_secrets/templates/netbox_secrets/inc/secrets_panel.html` & `netbox-secrets-1.8.5/netbox_secrets/templates/netbox_secrets/inc/secrets_panel.html`

 * *Files identical despite different names*

### Comparing `netbox-secrets-1.8.4/netbox_secrets/templates/netbox_secrets/inc/view_tab.html` & `netbox-secrets-1.8.5/netbox_secrets/templates/netbox_secrets/inc/view_tab.html`

 * *Files identical despite different names*

### Comparing `netbox-secrets-1.8.4/netbox_secrets/templates/netbox_secrets/secret.html` & `netbox-secrets-1.8.5/netbox_secrets/templates/netbox_secrets/secret.html`

 * *Files identical despite different names*

### Comparing `netbox-secrets-1.8.4/netbox_secrets/templates/netbox_secrets/secret_edit.html` & `netbox-secrets-1.8.5/netbox_secrets/templates/netbox_secrets/secret_edit.html`

 * *Files identical despite different names*

### Comparing `netbox-secrets-1.8.4/netbox_secrets/templates/netbox_secrets/secretrole.html` & `netbox-secrets-1.8.5/netbox_secrets/templates/netbox_secrets/secretrole.html`

 * *Files identical despite different names*

### Comparing `netbox-secrets-1.8.4/netbox_secrets/templates/netbox_secrets/userkey.html` & `netbox-secrets-1.8.5/netbox_secrets/templates/netbox_secrets/userkey.html`

 * *Files identical despite different names*

### Comparing `netbox-secrets-1.8.4/netbox_secrets/templates/netbox_secrets/userkey_edit.html` & `netbox-secrets-1.8.5/netbox_secrets/templates/netbox_secrets/userkey_edit.html`

 * *Files identical despite different names*

### Comparing `netbox-secrets-1.8.4/netbox_secrets/tests/constants.py` & `netbox-secrets-1.8.5/netbox_secrets/tests/constants.py`

 * *Files identical despite different names*

### Comparing `netbox-secrets-1.8.4/netbox_secrets/tests/test_api.py` & `netbox-secrets-1.8.5/netbox_secrets/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `netbox-secrets-1.8.4/netbox_secrets/tests/test_filters.py` & `netbox-secrets-1.8.5/netbox_secrets/tests/test_filters.py`

 * *Files identical despite different names*

### Comparing `netbox-secrets-1.8.4/netbox_secrets/tests/test_form.py` & `netbox-secrets-1.8.5/netbox_secrets/tests/test_form.py`

 * *Files identical despite different names*

### Comparing `netbox-secrets-1.8.4/netbox_secrets/tests/test_models.py` & `netbox-secrets-1.8.5/netbox_secrets/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `netbox-secrets-1.8.4/netbox_secrets/tests/test_views.py` & `netbox-secrets-1.8.5/netbox_secrets/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `netbox-secrets-1.8.4/netbox_secrets/urls.py` & `netbox-secrets-1.8.5/netbox_secrets/urls.py`

 * *Files identical despite different names*

### Comparing `netbox-secrets-1.8.4/netbox_secrets/utils/crypto.py` & `netbox-secrets-1.8.5/netbox_secrets/utils/crypto.py`

 * *Files identical despite different names*

### Comparing `netbox-secrets-1.8.4/netbox_secrets/views.py` & `netbox-secrets-1.8.5/netbox_secrets/views.py`

 * *Files identical despite different names*

### Comparing `netbox-secrets-1.8.4/netbox_secrets.egg-info/SOURCES.txt` & `netbox-secrets-1.8.5/netbox_secrets.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `netbox-secrets-1.8.4/setup.py` & `netbox-secrets-1.8.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name='netbox-secrets',
-    version='1.8.4',
+    version='1.8.5',
     description='Netbox Secrets',
     long_description='A Secret store for NetBox',
     url='https://github.com/Onemind-Services-LLC/netbox-secrets/',
     author='Daniel Sheppard',
     author_email='dans@dansheps.com',
     license='Apache 2.0',
     install_requires=[
```

