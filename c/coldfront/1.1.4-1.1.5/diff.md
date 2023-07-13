# Comparing `tmp/coldfront-1.1.4.tar.gz` & `tmp/coldfront-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coldfront-1.1.4.tar", last modified: Sun Feb 12 02:48:33 2023, max compression
+gzip compressed data, was "coldfront-1.1.5.tar", last modified: Thu Jul 13 00:45:36 2023, max compression
```

## Comparing `coldfront-1.1.4.tar` & `coldfront-1.1.5.tar`

### file list

```diff
@@ -1,468 +1,465 @@
-drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-02-12 02:48:33.370168 coldfront-1.1.4/
--rw-r--r--   0 aeb       (1000) aeb       (1000)      468 2022-02-07 13:09:23.000000 coldfront-1.1.4/AUTHORS.md
--rw-r--r--   0 aeb       (1000) aeb       (1000)    35147 2021-02-25 21:11:22.000000 coldfront-1.1.4/LICENSE
--rw-r--r--   0 aeb       (1000) aeb       (1000)      706 2022-03-09 21:14:23.000000 coldfront-1.1.4/MANIFEST.in
--rw-r--r--   0 aeb       (1000) aeb       (1000)     2979 2023-02-12 02:48:33.370168 coldfront-1.1.4/PKG-INFO
--rw-r--r--   0 aeb       (1000) aeb       (1000)     2071 2022-08-05 14:28:00.000000 coldfront-1.1.4/README.md
-drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-02-12 02:48:33.322167 coldfront-1.1.4/coldfront/
--rw-r--r--   0 aeb       (1000) aeb       (1000)      268 2023-02-12 02:44:04.000000 coldfront-1.1.4/coldfront/__init__.py
-drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-02-12 02:48:33.322167 coldfront-1.1.4/coldfront/config/
--rw-r--r--   0 aeb       (1000) aeb       (1000)        0 2021-02-25 21:11:22.000000 coldfront-1.1.4/coldfront/config/__init__.py
--rw-r--r--   0 aeb       (1000) aeb       (1000)     1268 2023-02-10 14:14:51.000000 coldfront-1.1.4/coldfront/config/auth.py
--rw-r--r--   0 aeb       (1000) aeb       (1000)     5450 2022-07-07 16:08:59.000000 coldfront-1.1.4/coldfront/config/base.py
--rw-r--r--   0 aeb       (1000) aeb       (1000)     4638 2022-07-07 13:52:57.000000 coldfront-1.1.4/coldfront/config/core.py
--rw-r--r--   0 aeb       (1000) aeb       (1000)     1515 2022-02-07 13:09:25.000000 coldfront-1.1.4/coldfront/config/database.py
--rw-r--r--   0 aeb       (1000) aeb       (1000)     1589 2022-09-23 21:50:06.000000 coldfront-1.1.4/coldfront/config/email.py
--rw-r--r--   0 aeb       (1000) aeb       (1000)      475 2021-11-10 16:20:52.000000 coldfront-1.1.4/coldfront/config/env.py
--rw-r--r--   0 aeb       (1000) aeb       (1000)      992 2021-03-02 21:10:03.000000 coldfront-1.1.4/coldfront/config/logging.py
-drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-02-12 02:48:33.326167 coldfront-1.1.4/coldfront/config/plugins/
--rw-r--r--   0 aeb       (1000) aeb       (1000)        0 2021-03-02 21:10:03.000000 coldfront-1.1.4/coldfront/config/plugins/__init__.py
--rw-r--r--   0 aeb       (1000) aeb       (1000)      414 2021-03-02 21:10:03.000000 coldfront-1.1.4/coldfront/config/plugins/freeipa.py
--rw-r--r--   0 aeb       (1000) aeb       (1000)      332 2021-03-02 21:10:03.000000 coldfront-1.1.4/coldfront/config/plugins/iquota.py
--rw-r--r--   0 aeb       (1000) aeb       (1000)     1748 2021-03-25 15:26:38.000000 coldfront-1.1.4/coldfront/config/plugins/ldap.py
--rw-r--r--   0 aeb       (1000) aeb       (1000)      935 2022-01-12 23:53:55.000000 coldfront-1.1.4/coldfront/config/plugins/ldap_user_search.py
--rw-r--r--   0 aeb       (1000) aeb       (1000)     1582 2021-03-02 21:10:03.000000 coldfront-1.1.4/coldfront/config/plugins/openid.py
--rw-r--r--   0 aeb       (1000) aeb       (1000)      406 2022-04-27 00:11:56.000000 coldfront-1.1.4/coldfront/config/plugins/slurm.py
--rw-r--r--   0 aeb       (1000) aeb       (1000)      420 2021-03-02 21:10:03.000000 coldfront-1.1.4/coldfront/config/plugins/system_monitor.py
--rw-r--r--   0 aeb       (1000) aeb       (1000)      365 2021-03-02 21:10:03.000000 coldfront-1.1.4/coldfront/config/plugins/xdmod.py
--rw-r--r--   0 aeb       (1000) aeb       (1000)     1532 2022-09-29 18:05:12.000000 coldfront-1.1.4/coldfront/config/settings.py
--rw-r--r--   0 aeb       (1000) aeb       (1000)     1683 2022-09-29 18:05:12.000000 coldfront-1.1.4/coldfront/config/urls.py
--rw-r--r--   0 aeb       (1000) aeb       (1000)      302 2021-02-25 21:11:22.000000 coldfront-1.1.4/coldfront/config/wsgi.py
-drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-02-12 02:48:33.326167 coldfront-1.1.4/coldfront/core/
--rw-r--r--   0 aeb       (1000) aeb       (1000)        0 2021-02-25 21:11:22.000000 coldfront-1.1.4/coldfront/core/__init__.py
-drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-02-12 02:48:33.326167 coldfront-1.1.4/coldfront/core/allocation/
--rw-r--r--   0 aeb       (1000) aeb       (1000)        0 2021-02-25 21:11:22.000000 coldfront-1.1.4/coldfront/core/allocation/__init__.py
--rw-r--r--   0 aeb       (1000) aeb       (1000)    12577 2021-12-23 13:28:09.000000 coldfront-1.1.4/coldfront/core/allocation/admin.py
--rw-r--r--   0 aeb       (1000) aeb       (1000)      110 2022-02-07 13:09:25.000000 coldfront-1.1.4/coldfront/core/allocation/apps.py
--rw-r--r--   0 aeb       (1000) aeb       (1000)    11419 2023-02-09 20:15:46.000000 coldfront-1.1.4/coldfront/core/allocation/forms.py
-drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-02-12 02:48:33.326167 coldfront-1.1.4/coldfront/core/allocation/management/
--rw-r--r--   0 aeb       (1000) aeb       (1000)        0 2021-03-03 01:27:01.000000 coldfront-1.1.4/coldfront/core/allocation/management/__init__.py
-drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-02-12 02:48:33.326167 coldfront-1.1.4/coldfront/core/allocation/management/commands/
--rw-r--r--   0 aeb       (1000) aeb       (1000)        0 2021-03-03 01:27:01.000000 coldfront-1.1.4/coldfront/core/allocation/management/commands/__init__.py
--rw-r--r--   0 aeb       (1000) aeb       (1000)     2972 2022-10-09 13:46:08.000000 coldfront-1.1.4/coldfront/core/allocation/management/commands/add_allocation_defaults.py
--rw-r--r--   0 aeb       (1000) aeb       (1000)      448 2022-03-11 14:30:53.000000 coldfront-1.1.4/coldfront/core/allocation/management/commands/enable_change_requests_globally.py
-drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-02-12 02:48:33.326167 coldfront-1.1.4/coldfront/core/allocation/migrations/
--rw-r--r--   0 aeb       (1000) aeb       (1000)    19472 2021-02-25 21:11:22.000000 coldfront-1.1.4/coldfront/core/allocation/migrations/0001_initial.py
--rw-r--r--   0 aeb       (1000) aeb       (1000)      878 2021-02-25 21:11:22.000000 coldfront-1.1.4/coldfront/core/allocation/migrations/0002_auto_20190718_1451.py
--rw-r--r--   0 aeb       (1000) aeb       (1000)      568 2021-02-25 21:11:22.000000 coldfront-1.1.4/coldfront/core/allocation/migrations/0003_auto_20191018_1049.py
--rw-r--r--   0 aeb       (1000) aeb       (1000)     7952 2021-12-23 13:28:09.000000 coldfront-1.1.4/coldfront/core/allocation/migrations/0004_auto_20211102_1017.py
--rw-r--r--   0 aeb       (1000) aeb       (1000)      554 2021-12-23 13:28:09.000000 coldfront-1.1.4/coldfront/core/allocation/migrations/0005_auto_20211117_1413.py
--rw-r--r--   0 aeb       (1000) aeb       (1000)        0 2021-02-25 21:11:22.000000 coldfront-1.1.4/coldfront/core/allocation/migrations/__init__.py
--rw-r--r--   0 aeb       (1000) aeb       (1000)    20509 2023-02-10 01:45:05.000000 coldfront-1.1.4/coldfront/core/allocation/models.py
--rw-r--r--   0 aeb       (1000) aeb       (1000)      499 2022-08-05 14:28:00.000000 coldfront-1.1.4/coldfront/core/allocation/signals.py
--rw-r--r--   0 aeb       (1000) aeb       (1000)    10122 2022-09-20 14:51:20.000000 coldfront-1.1.4/coldfront/core/allocation/tasks.py
-drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-02-12 02:48:33.314167 coldfront-1.1.4/coldfront/core/allocation/templates/
-drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-02-12 02:48:33.330167 coldfront-1.1.4/coldfront/core/allocation/templates/allocation/
--rw-r--r--   0 aeb       (1000) aeb       (1000)     1021 2021-02-25 21:11:22.000000 coldfront-1.1.4/coldfront/core/allocation/templates/allocation/allocation_account_list.html
--rw-r--r--   0 aeb       (1000) aeb       (1000)      554 2021-02-25 21:11:22.000000 coldfront-1.1.4/coldfront/core/allocation/templates/allocation/allocation_add_invoice_note.html
--rw-r--r--   0 aeb       (1000) aeb       (1000)     2525 2023-02-09 20:15:46.000000 coldfront-1.1.4/coldfront/core/allocation/templates/allocation/allocation_add_users.html
--rw-r--r--   0 aeb       (1000) aeb       (1000)      501 2021-02-25 21:11:22.000000 coldfront-1.1.4/coldfront/core/allocation/templates/allocation/allocation_allocationaccount_create.html
--rw-r--r--   0 aeb       (1000) aeb       (1000)      657 2023-02-09 20:15:46.000000 coldfront-1.1.4/coldfront/core/allocation/templates/allocation/allocation_allocationattribute_create.html
--rw-r--r--   0 aeb       (1000) aeb       (1000)     2280 2023-02-09 20:15:46.000000 coldfront-1.1.4/coldfront/core/allocation/templates/allocation/allocation_allocationattribute_delete.html
--rw-r--r--   0 aeb       (1000) aeb       (1000)     5035 2023-02-09 20:15:46.000000 coldfront-1.1.4/coldfront/core/allocation/templates/allocation/allocation_change.html
--rw-r--r--   0 aeb       (1000) aeb       (1000)     8588 2023-02-09 20:15:46.000000 coldfront-1.1.4/coldfront/core/allocation/templates/allocation/allocation_change_detail.html
--rw-r--r--   0 aeb       (1000) aeb       (1000)     3247 2023-02-09 20:15:46.000000 coldfront-1.1.4/coldfront/core/allocation/templates/allocation/allocation_change_list.html
--rw-r--r--   0 aeb       (1000) aeb       (1000)     6005 2023-02-09 20:15:46.000000 coldfront-1.1.4/coldfront/core/allocation/templates/allocation/allocation_create.html
--rw-r--r--   0 aeb       (1000) aeb       (1000)     1828 2021-02-25 21:11:22.000000 coldfront-1.1.4/coldfront/core/allocation/templates/allocation/allocation_delete_invoice_note.html
--rw-r--r--   0 aeb       (1000) aeb       (1000)    16062 2023-02-09 20:15:46.000000 coldfront-1.1.4/coldfront/core/allocation/templates/allocation/allocation_detail.html
--rw-r--r--   0 aeb       (1000) aeb       (1000)     1990 2021-02-25 21:11:22.000000 coldfront-1.1.4/coldfront/core/allocation/templates/allocation/allocation_email_pending_request.html
--rw-r--r--   0 aeb       (1000) aeb       (1000)     4540 2021-02-25 21:11:22.000000 coldfront-1.1.4/coldfront/core/allocation/templates/allocation/allocation_invoice_detail.html
--rw-r--r--   0 aeb       (1000) aeb       (1000)     1029 2022-03-09 21:14:23.000000 coldfront-1.1.4/coldfront/core/allocation/templates/allocation/allocation_invoice_list.html
--rw-r--r--   0 aeb       (1000) aeb       (1000)     6186 2023-02-09 20:15:46.000000 coldfront-1.1.4/coldfront/core/allocation/templates/allocation/allocation_list.html
--rw-r--r--   0 aeb       (1000) aeb       (1000)      652 2022-01-11 16:10:19.000000 coldfront-1.1.4/coldfront/core/allocation/templates/allocation/allocation_note_create.html
--rw-r--r--   0 aeb       (1000) aeb       (1000)     2543 2023-02-09 20:15:46.000000 coldfront-1.1.4/coldfront/core/allocation/templates/allocation/allocation_remove_users.html
--rw-r--r--   0 aeb       (1000) aeb       (1000)     3521 2021-02-25 21:11:22.000000 coldfront-1.1.4/coldfront/core/allocation/templates/allocation/allocation_renew.html
--rw-r--r--   0 aeb       (1000) aeb       (1000)     2997 2023-02-09 20:15:46.000000 coldfront-1.1.4/coldfront/core/allocation/templates/allocation/allocation_request_list.html
--rw-r--r--   0 aeb       (1000) aeb       (1000)      572 2021-02-25 21:11:22.000000 coldfront-1.1.4/coldfront/core/allocation/templates/allocation/allocation_update_invoice_note.html
--rw-r--r--   0 aeb       (1000) aeb       (1000)       60 2023-02-09 20:15:46.000000 coldfront-1.1.4/coldfront/core/allocation/tests.py
--rw-r--r--   0 aeb       (1000) aeb       (1000)     2874 2023-02-09 20:15:46.000000 coldfront-1.1.4/coldfront/core/allocation/urls.py
--rw-r--r--   0 aeb       (1000) aeb       (1000)     1622 2021-12-23 15:00:25.000000 coldfront-1.1.4/coldfront/core/allocation/utils.py
--rw-r--r--   0 aeb       (1000) aeb       (1000)    80919 2023-02-10 01:45:05.000000 coldfront-1.1.4/coldfront/core/allocation/views.py
--rw-r--r--   0 aeb       (1000) aeb       (1000)    20969 2022-01-07 20:54:01.000000 coldfront-1.1.4/coldfront/core/attribute_expansion.py
-drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-02-12 02:48:33.330167 coldfront-1.1.4/coldfront/core/field_of_science/
--rw-r--r--   0 aeb       (1000) aeb       (1000)       81 2021-02-25 21:11:22.000000 coldfront-1.1.4/coldfront/core/field_of_science/__init__.py
--rw-r--r--   0 aeb       (1000) aeb       (1000)      427 2021-02-25 21:11:22.000000 coldfront-1.1.4/coldfront/core/field_of_science/admin.py
--rw-r--r--   0 aeb       (1000) aeb       (1000)      158 2021-02-25 21:11:22.000000 coldfront-1.1.4/coldfront/core/field_of_science/apps.py
-drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-02-12 02:48:33.330167 coldfront-1.1.4/coldfront/core/field_of_science/management/
--rw-r--r--   0 aeb       (1000) aeb       (1000)        0 2021-02-25 21:11:22.000000 coldfront-1.1.4/coldfront/core/field_of_science/management/__init__.py
-drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-02-12 02:48:33.330167 coldfront-1.1.4/coldfront/core/field_of_science/management/commands/
--rw-r--r--   0 aeb       (1000) aeb       (1000)        0 2021-02-25 21:11:22.000000 coldfront-1.1.4/coldfront/core/field_of_science/management/commands/__init__.py
-drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-02-12 02:48:33.330167 coldfront-1.1.4/coldfront/core/field_of_science/management/commands/data/
--rw-r--r--   0 aeb       (1000) aeb       (1000)     7584 2021-02-25 21:11:22.000000 coldfront-1.1.4/coldfront/core/field_of_science/management/commands/data/field_of_science_data.csv
--rw-r--r--   0 aeb       (1000) aeb       (1000)     1282 2021-02-25 21:11:22.000000 coldfront-1.1.4/coldfront/core/field_of_science/management/commands/import_field_of_science_data.py
-drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-02-12 02:48:33.330167 coldfront-1.1.4/coldfront/core/field_of_science/migrations/
--rw-r--r--   0 aeb       (1000) aeb       (1000)     1426 2021-02-25 21:11:22.000000 coldfront-1.1.4/coldfront/core/field_of_science/migrations/0001_initial.py
--rw-r--r--   0 aeb       (1000) aeb       (1000)        0 2021-02-25 21:11:22.000000 coldfront-1.1.4/coldfront/core/field_of_science/migrations/__init__.py
--rw-r--r--   0 aeb       (1000) aeb       (1000)      636 2021-02-25 21:11:22.000000 coldfront-1.1.4/coldfront/core/field_of_science/models.py
--rw-r--r--   0 aeb       (1000) aeb       (1000)     4235 2021-11-10 16:20:52.000000 coldfront-1.1.4/coldfront/core/field_of_science/tests.py
--rw-r--r--   0 aeb       (1000) aeb       (1000)       63 2021-02-25 21:11:22.000000 coldfront-1.1.4/coldfront/core/field_of_science/views.py
-drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-02-12 02:48:33.334167 coldfront-1.1.4/coldfront/core/grant/
--rw-r--r--   0 aeb       (1000) aeb       (1000)        0 2021-02-25 21:11:22.000000 coldfront-1.1.4/coldfront/core/grant/__init__.py
--rw-r--r--   0 aeb       (1000) aeb       (1000)     1455 2022-09-29 18:05:12.000000 coldfront-1.1.4/coldfront/core/grant/admin.py
--rw-r--r--   0 aeb       (1000) aeb       (1000)      100 2022-02-07 13:09:25.000000 coldfront-1.1.4/coldfront/core/grant/apps.py
--rw-r--r--   0 aeb       (1000) aeb       (1000)     2589 2022-09-29 18:05:12.000000 coldfront-1.1.4/coldfront/core/grant/forms.py
-drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-02-12 02:48:33.334167 coldfront-1.1.4/coldfront/core/grant/management/
--rw-r--r--   0 aeb       (1000) aeb       (1000)        0 2021-03-03 01:27:01.000000 coldfront-1.1.4/coldfront/core/grant/management/__init__.py
-drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-02-12 02:48:33.334167 coldfront-1.1.4/coldfront/core/grant/management/commands/
--rw-r--r--   0 aeb       (1000) aeb       (1000)        0 2021-03-03 01:27:01.000000 coldfront-1.1.4/coldfront/core/grant/management/commands/__init__.py
--rw-r--r--   0 aeb       (1000) aeb       (1000)     1186 2021-02-25 21:11:22.000000 coldfront-1.1.4/coldfront/core/grant/management/commands/add_default_grant_options.py
-drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-02-12 02:48:33.334167 coldfront-1.1.4/coldfront/core/grant/migrations/
--rw-r--r--   0 aeb       (1000) aeb       (1000)     7260 2021-02-25 21:11:22.000000 coldfront-1.1.4/coldfront/core/grant/migrations/0001_initial.py
--rw-r--r--   0 aeb       (1000) aeb       (1000)        0 2021-02-25 21:11:22.000000 coldfront-1.1.4/coldfront/core/grant/migrations/__init__.py
--rw-r--r--   0 aeb       (1000) aeb       (1000)     2438 2022-09-29 18:05:12.000000 coldfront-1.1.4/coldfront/core/grant/models.py
-drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-02-12 02:48:33.314167 coldfront-1.1.4/coldfront/core/grant/templates/
-drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-02-12 02:48:33.334167 coldfront-1.1.4/coldfront/core/grant/templates/grant/
--rw-r--r--   0 aeb       (1000) aeb       (1000)      499 2023-02-09 20:15:46.000000 coldfront-1.1.4/coldfront/core/grant/templates/grant/grant_create.html
--rw-r--r--   0 aeb       (1000) aeb       (1000)     2281 2023-02-09 20:15:46.000000 coldfront-1.1.4/coldfront/core/grant/templates/grant/grant_delete_grants.html
--rw-r--r--   0 aeb       (1000) aeb       (1000)     3647 2022-04-27 00:08:38.000000 coldfront-1.1.4/coldfront/core/grant/templates/grant/grant_report_list.html
--rw-r--r--   0 aeb       (1000) aeb       (1000)      492 2022-09-20 14:51:20.000000 coldfront-1.1.4/coldfront/core/grant/templates/grant/grant_update_form.html
--rw-r--r--   0 aeb       (1000) aeb       (1000)     9083 2023-02-09 20:15:46.000000 coldfront-1.1.4/coldfront/core/grant/tests.py
--rw-r--r--   0 aeb       (1000) aeb       (1000)      599 2022-09-29 18:05:12.000000 coldfront-1.1.4/coldfront/core/grant/urls.py
--rw-r--r--   0 aeb       (1000) aeb       (1000)    13714 2022-09-29 18:05:12.000000 coldfront-1.1.4/coldfront/core/grant/views.py
-drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-02-12 02:48:33.334167 coldfront-1.1.4/coldfront/core/portal/
--rw-r--r--   0 aeb       (1000) aeb       (1000)        0 2021-02-25 21:11:22.000000 coldfront-1.1.4/coldfront/core/portal/__init__.py
--rw-r--r--   0 aeb       (1000) aeb       (1000)      397 2021-02-25 21:11:22.000000 coldfront-1.1.4/coldfront/core/portal/admin.py
--rw-r--r--   0 aeb       (1000) aeb       (1000)      102 2022-02-07 13:09:25.000000 coldfront-1.1.4/coldfront/core/portal/apps.py
-drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-02-12 02:48:33.334167 coldfront-1.1.4/coldfront/core/portal/migrations/
--rw-r--r--   0 aeb       (1000) aeb       (1000)        0 2021-02-25 21:11:22.000000 coldfront-1.1.4/coldfront/core/portal/migrations/__init__.py
--rw-r--r--   0 aeb       (1000) aeb       (1000)       57 2021-02-25 21:11:22.000000 coldfront-1.1.4/coldfront/core/portal/models.py
-drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-02-12 02:48:33.314167 coldfront-1.1.4/coldfront/core/portal/templates/
-drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-02-12 02:48:33.334167 coldfront-1.1.4/coldfront/core/portal/templates/portal/
--rw-r--r--   0 aeb       (1000) aeb       (1000)      696 2021-02-25 21:11:22.000000 coldfront-1.1.4/coldfront/core/portal/templates/portal/allocation_by_fos.html
--rw-r--r--   0 aeb       (1000) aeb       (1000)     1867 2021-02-25 21:11:22.000000 coldfront-1.1.4/coldfront/core/portal/templates/portal/allocation_summary.html
--rw-r--r--   0 aeb       (1000) aeb       (1000)     4207 2021-02-25 21:11:22.000000 coldfront-1.1.4/coldfront/core/portal/templates/portal/authorized_home.html
--rw-r--r--   0 aeb       (1000) aeb       (1000)     1415 2021-02-25 21:11:22.000000 coldfront-1.1.4/coldfront/core/portal/templates/portal/carousel.html
--rw-r--r--   0 aeb       (1000) aeb       (1000)     5519 2022-02-07 13:09:25.000000 coldfront-1.1.4/coldfront/core/portal/templates/portal/center_summary.html
--rw-r--r--   0 aeb       (1000) aeb       (1000)      259 2021-02-25 21:11:22.000000 coldfront-1.1.4/coldfront/core/portal/templates/portal/extra_app_templates.html
--rw-r--r--   0 aeb       (1000) aeb       (1000)      891 2023-02-09 20:15:46.000000 coldfront-1.1.4/coldfront/core/portal/templates/portal/nonauthorized_home.html
-drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-02-12 02:48:33.334167 coldfront-1.1.4/coldfront/core/portal/templatetags/
--rw-r--r--   0 aeb       (1000) aeb       (1000)        0 2021-03-03 01:27:01.000000 coldfront-1.1.4/coldfront/core/portal/templatetags/__init__.py
--rw-r--r--   0 aeb       (1000) aeb       (1000)      247 2021-02-25 21:11:22.000000 coldfront-1.1.4/coldfront/core/portal/templatetags/portal_tags.py
--rw-r--r--   0 aeb       (1000) aeb       (1000)       60 2023-02-09 20:15:46.000000 coldfront-1.1.4/coldfront/core/portal/tests.py
--rw-r--r--   0 aeb       (1000) aeb       (1000)     3448 2021-02-25 21:11:22.000000 coldfront-1.1.4/coldfront/core/portal/utils.py
--rw-r--r--   0 aeb       (1000) aeb       (1000)     6907 2021-03-02 21:10:03.000000 coldfront-1.1.4/coldfront/core/portal/views.py
-drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-02-12 02:48:33.338168 coldfront-1.1.4/coldfront/core/project/
--rw-r--r--   0 aeb       (1000) aeb       (1000)       65 2021-02-25 21:11:22.000000 coldfront-1.1.4/coldfront/core/project/__init__.py
--rw-r--r--   0 aeb       (1000) aeb       (1000)    10121 2022-11-23 21:22:01.000000 coldfront-1.1.4/coldfront/core/project/admin.py
--rw-r--r--   0 aeb       (1000) aeb       (1000)      104 2021-02-25 21:11:22.000000 coldfront-1.1.4/coldfront/core/project/apps.py
--rw-r--r--   0 aeb       (1000) aeb       (1000)     8727 2023-02-09 20:15:46.000000 coldfront-1.1.4/coldfront/core/project/forms.py
-drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-02-12 02:48:33.338168 coldfront-1.1.4/coldfront/core/project/management/
--rw-r--r--   0 aeb       (1000) aeb       (1000)        0 2021-03-03 01:27:01.000000 coldfront-1.1.4/coldfront/core/project/management/__init__.py
-drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-02-12 02:48:33.338168 coldfront-1.1.4/coldfront/core/project/management/commands/
--rw-r--r--   0 aeb       (1000) aeb       (1000)        0 2021-03-03 01:27:01.000000 coldfront-1.1.4/coldfront/core/project/management/commands/__init__.py
--rw-r--r--   0 aeb       (1000) aeb       (1000)     1645 2022-11-23 21:22:01.000000 coldfront-1.1.4/coldfront/core/project/management/commands/add_default_project_choices.py
-drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-02-12 02:48:33.338168 coldfront-1.1.4/coldfront/core/project/migrations/
--rw-r--r--   0 aeb       (1000) aeb       (1000)    15306 2021-02-25 21:11:22.000000 coldfront-1.1.4/coldfront/core/project/migrations/0001_initial.py
--rw-r--r--   0 aeb       (1000) aeb       (1000)      392 2022-07-07 13:52:57.000000 coldfront-1.1.4/coldfront/core/project/migrations/0002_projectusermessage_is_private.py
--rw-r--r--   0 aeb       (1000) aeb       (1000)     9244 2022-11-23 21:22:01.000000 coldfront-1.1.4/coldfront/core/project/migrations/0003_auto_20221013_1215.py
--rw-r--r--   0 aeb       (1000) aeb       (1000)        0 2021-02-25 21:11:22.000000 coldfront-1.1.4/coldfront/core/project/migrations/__init__.py
--rw-r--r--   0 aeb       (1000) aeb       (1000)     9922 2022-11-23 21:22:01.000000 coldfront-1.1.4/coldfront/core/project/models.py
-drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-02-12 02:48:33.314167 coldfront-1.1.4/coldfront/core/project/templates/
-drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-02-12 02:48:33.338168 coldfront-1.1.4/coldfront/core/project/templates/project/
--rw-r--r--   0 aeb       (1000) aeb       (1000)     3403 2023-02-09 20:15:46.000000 coldfront-1.1.4/coldfront/core/project/templates/project/add_user_search_results.html
--rw-r--r--   0 aeb       (1000) aeb       (1000)     3189 2021-02-25 21:11:22.000000 coldfront-1.1.4/coldfront/core/project/templates/project/project_add_users.html
--rw-r--r--   0 aeb       (1000) aeb       (1000)     1358 2021-02-25 21:11:22.000000 coldfront-1.1.4/coldfront/core/project/templates/project/project_archive.html
--rw-r--r--   0 aeb       (1000) aeb       (1000)     5320 2022-01-11 16:10:19.000000 coldfront-1.1.4/coldfront/core/project/templates/project/project_archived_list.html
--rw-r--r--   0 aeb       (1000) aeb       (1000)      513 2022-11-23 21:22:01.000000 coldfront-1.1.4/coldfront/core/project/templates/project/project_attribute_create.html
--rw-r--r--   0 aeb       (1000) aeb       (1000)     2286 2022-11-23 21:22:01.000000 coldfront-1.1.4/coldfront/core/project/templates/project/project_attribute_delete.html
--rw-r--r--   0 aeb       (1000) aeb       (1000)     1444 2022-11-23 21:22:01.000000 coldfront-1.1.4/coldfront/core/project/templates/project/project_attribute_update.html
--rw-r--r--   0 aeb       (1000) aeb       (1000)      488 2023-02-09 20:15:46.000000 coldfront-1.1.4/coldfront/core/project/templates/project/project_create_form.html
--rw-r--r--   0 aeb       (1000) aeb       (1000)    26553 2023-02-09 20:15:46.000000 coldfront-1.1.4/coldfront/core/project/templates/project/project_detail.html
--rw-r--r--   0 aeb       (1000) aeb       (1000)     5666 2023-02-09 20:15:46.000000 coldfront-1.1.4/coldfront/core/project/templates/project/project_list.html
--rw-r--r--   0 aeb       (1000) aeb       (1000)      611 2022-07-07 13:52:57.000000 coldfront-1.1.4/coldfront/core/project/templates/project/project_note_create.html
--rw-r--r--   0 aeb       (1000) aeb       (1000)     2536 2021-02-25 21:11:22.000000 coldfront-1.1.4/coldfront/core/project/templates/project/project_remove_users.html
--rw-r--r--   0 aeb       (1000) aeb       (1000)     2453 2023-02-09 20:15:46.000000 coldfront-1.1.4/coldfront/core/project/templates/project/project_review.html
--rw-r--r--   0 aeb       (1000) aeb       (1000)     1883 2023-02-09 20:15:46.000000 coldfront-1.1.4/coldfront/core/project/templates/project/project_review_email.html
--rw-r--r--   0 aeb       (1000) aeb       (1000)     2158 2023-02-09 20:15:46.000000 coldfront-1.1.4/coldfront/core/project/templates/project/project_review_list.html
--rw-r--r--   0 aeb       (1000) aeb       (1000)      498 2021-02-25 21:11:22.000000 coldfront-1.1.4/coldfront/core/project/templates/project/project_update_form.html
--rw-r--r--   0 aeb       (1000) aeb       (1000)     2300 2021-02-25 21:11:22.000000 coldfront-1.1.4/coldfront/core/project/templates/project/project_user_detail.html
--rw-r--r--   0 aeb       (1000) aeb       (1000)     4684 2023-02-09 20:15:46.000000 coldfront-1.1.4/coldfront/core/project/tests.py
--rw-r--r--   0 aeb       (1000) aeb       (1000)     2434 2022-11-23 21:22:01.000000 coldfront-1.1.4/coldfront/core/project/urls.py
--rw-r--r--   0 aeb       (1000) aeb       (1000)      770 2021-02-25 21:11:22.000000 coldfront-1.1.4/coldfront/core/project/utils.py
--rw-r--r--   0 aeb       (1000) aeb       (1000)    57685 2022-11-23 21:22:01.000000 coldfront-1.1.4/coldfront/core/project/views.py
-drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-02-12 02:48:33.342168 coldfront-1.1.4/coldfront/core/publication/
--rw-r--r--   0 aeb       (1000) aeb       (1000)        0 2021-02-25 21:11:22.000000 coldfront-1.1.4/coldfront/core/publication/__init__.py
--rw-r--r--   0 aeb       (1000) aeb       (1000)      500 2021-02-25 21:11:22.000000 coldfront-1.1.4/coldfront/core/publication/admin.py
--rw-r--r--   0 aeb       (1000) aeb       (1000)      112 2022-02-07 13:09:25.000000 coldfront-1.1.4/coldfront/core/publication/apps.py
--rw-r--r--   0 aeb       (1000) aeb       (1000)     1799 2022-09-29 18:05:12.000000 coldfront-1.1.4/coldfront/core/publication/forms.py
-drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-02-12 02:48:33.342168 coldfront-1.1.4/coldfront/core/publication/management/
--rw-r--r--   0 aeb       (1000) aeb       (1000)        0 2021-03-03 01:27:01.000000 coldfront-1.1.4/coldfront/core/publication/management/__init__.py
-drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-02-12 02:48:33.342168 coldfront-1.1.4/coldfront/core/publication/management/commands/
--rw-r--r--   0 aeb       (1000) aeb       (1000)        0 2021-03-03 01:27:01.000000 coldfront-1.1.4/coldfront/core/publication/management/commands/__init__.py
--rw-r--r--   0 aeb       (1000) aeb       (1000)      490 2022-09-29 18:05:12.000000 coldfront-1.1.4/coldfront/core/publication/management/commands/add_default_publication_sources.py
-drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-02-12 02:48:33.342168 coldfront-1.1.4/coldfront/core/publication/migrations/
--rw-r--r--   0 aeb       (1000) aeb       (1000)     4520 2021-02-25 21:11:22.000000 coldfront-1.1.4/coldfront/core/publication/migrations/0001_initial.py
--rw-r--r--   0 aeb       (1000) aeb       (1000)      650 2021-02-25 21:11:22.000000 coldfront-1.1.4/coldfront/core/publication/migrations/0002_auto_20191223_1115.py
--rw-r--r--   0 aeb       (1000) aeb       (1000)      581 2021-02-25 21:11:22.000000 coldfront-1.1.4/coldfront/core/publication/migrations/0003_auto_20200104_1700.py
--rw-r--r--   0 aeb       (1000) aeb       (1000)      562 2021-02-25 21:11:22.000000 coldfront-1.1.4/coldfront/core/publication/migrations/0004_add_manual_publication_source.py
--rw-r--r--   0 aeb       (1000) aeb       (1000)        0 2021-02-25 21:11:22.000000 coldfront-1.1.4/coldfront/core/publication/migrations/__init__.py
--rw-r--r--   0 aeb       (1000) aeb       (1000)     1207 2022-09-29 18:05:12.000000 coldfront-1.1.4/coldfront/core/publication/models.py
-drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-02-12 02:48:33.314167 coldfront-1.1.4/coldfront/core/publication/templates/
-drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-02-12 02:48:33.342168 coldfront-1.1.4/coldfront/core/publication/templates/publication/
--rw-r--r--   0 aeb       (1000) aeb       (1000)     1200 2023-02-09 20:15:46.000000 coldfront-1.1.4/coldfront/core/publication/templates/publication/publication_add_publication_manually.html
--rw-r--r--   0 aeb       (1000) aeb       (1000)     2509 2023-02-09 20:15:46.000000 coldfront-1.1.4/coldfront/core/publication/templates/publication/publication_add_publication_search.html
--rw-r--r--   0 aeb       (1000) aeb       (1000)     2486 2023-02-09 20:15:46.000000 coldfront-1.1.4/coldfront/core/publication/templates/publication/publication_add_publication_search_result.html
--rw-r--r--   0 aeb       (1000) aeb       (1000)     2270 2023-02-09 20:15:46.000000 coldfront-1.1.4/coldfront/core/publication/templates/publication/publication_delete_publications.html
--rw-r--r--   0 aeb       (1000) aeb       (1000)     3215 2021-02-25 21:11:22.000000 coldfront-1.1.4/coldfront/core/publication/templates/publication/publication_export_publications.html
--rw-r--r--   0 aeb       (1000) aeb       (1000)    10164 2023-02-09 20:15:46.000000 coldfront-1.1.4/coldfront/core/publication/tests.py
--rw-r--r--   0 aeb       (1000) aeb       (1000)      974 2022-09-29 18:05:12.000000 coldfront-1.1.4/coldfront/core/publication/urls.py
--rw-r--r--   0 aeb       (1000) aeb       (1000)    19605 2022-09-29 18:05:12.000000 coldfront-1.1.4/coldfront/core/publication/views.py
-drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-02-12 02:48:33.342168 coldfront-1.1.4/coldfront/core/research_output/
--rw-r--r--   0 aeb       (1000) aeb       (1000)        0 2021-02-25 21:11:22.000000 coldfront-1.1.4/coldfront/core/research_output/__init__.py
--rw-r--r--   0 aeb       (1000) aeb       (1000)     1018 2021-02-25 21:11:22.000000 coldfront-1.1.4/coldfront/core/research_output/admin.py
--rw-r--r--   0 aeb       (1000) aeb       (1000)      119 2022-02-07 13:09:25.000000 coldfront-1.1.4/coldfront/core/research_output/apps.py
--rw-r--r--   0 aeb       (1000) aeb       (1000)      219 2021-02-25 21:11:22.000000 coldfront-1.1.4/coldfront/core/research_output/forms.py
-drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-02-12 02:48:33.342168 coldfront-1.1.4/coldfront/core/research_output/migrations/
--rw-r--r--   0 aeb       (1000) aeb       (1000)     3220 2021-02-25 21:11:22.000000 coldfront-1.1.4/coldfront/core/research_output/migrations/0001_initial.py
--rw-r--r--   0 aeb       (1000) aeb       (1000)        0 2021-02-25 21:11:22.000000 coldfront-1.1.4/coldfront/core/research_output/migrations/__init__.py
--rw-r--r--   0 aeb       (1000) aeb       (1000)     1618 2021-02-25 21:11:22.000000 coldfront-1.1.4/coldfront/core/research_output/models.py
-drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-02-12 02:48:33.314167 coldfront-1.1.4/coldfront/core/research_output/templates/
-drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-02-12 02:48:33.342168 coldfront-1.1.4/coldfront/core/research_output/templates/research_output/
--rw-r--r--   0 aeb       (1000) aeb       (1000)      407 2023-02-09 20:15:46.000000 coldfront-1.1.4/coldfront/core/research_output/templates/research_output/research_output_create.html
--rw-r--r--   0 aeb       (1000) aeb       (1000)     2332 2023-02-09 20:15:46.000000 coldfront-1.1.4/coldfront/core/research_output/templates/research_output/research_output_delete_research_outputs.html
--rw-r--r--   0 aeb       (1000) aeb       (1000)     4906 2023-02-09 20:15:46.000000 coldfront-1.1.4/coldfront/core/research_output/tests.py
--rw-r--r--   0 aeb       (1000) aeb       (1000)      438 2021-02-25 21:11:22.000000 coldfront-1.1.4/coldfront/core/research_output/urls.py
--rw-r--r--   0 aeb       (1000) aeb       (1000)     3615 2021-02-25 21:11:22.000000 coldfront-1.1.4/coldfront/core/research_output/views.py
-drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-02-12 02:48:33.346168 coldfront-1.1.4/coldfront/core/resource/
--rw-r--r--   0 aeb       (1000) aeb       (1000)        0 2021-02-25 21:11:22.000000 coldfront-1.1.4/coldfront/core/resource/__init__.py
--rw-r--r--   0 aeb       (1000) aeb       (1000)     3108 2022-04-27 00:08:38.000000 coldfront-1.1.4/coldfront/core/resource/admin.py
--rw-r--r--   0 aeb       (1000) aeb       (1000)      106 2022-02-07 13:09:25.000000 coldfront-1.1.4/coldfront/core/resource/apps.py
--rw-r--r--   0 aeb       (1000) aeb       (1000)     2052 2022-09-20 14:51:20.000000 coldfront-1.1.4/coldfront/core/resource/forms.py
-drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-02-12 02:48:33.346168 coldfront-1.1.4/coldfront/core/resource/management/
--rw-r--r--   0 aeb       (1000) aeb       (1000)        0 2021-03-03 01:27:01.000000 coldfront-1.1.4/coldfront/core/resource/management/__init__.py
-drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-02-12 02:48:33.346168 coldfront-1.1.4/coldfront/core/resource/management/commands/
--rw-r--r--   0 aeb       (1000) aeb       (1000)        0 2021-03-03 01:27:01.000000 coldfront-1.1.4/coldfront/core/resource/management/commands/__init__.py
--rw-r--r--   0 aeb       (1000) aeb       (1000)     2147 2022-03-07 19:51:38.000000 coldfront-1.1.4/coldfront/core/resource/management/commands/add_resource_defaults.py
-drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-02-12 02:48:33.346168 coldfront-1.1.4/coldfront/core/resource/migrations/
--rw-r--r--   0 aeb       (1000) aeb       (1000)    12612 2021-02-25 21:11:22.000000 coldfront-1.1.4/coldfront/core/resource/migrations/0001_initial.py
--rw-r--r--   0 aeb       (1000) aeb       (1000)      533 2021-02-25 21:11:22.000000 coldfront-1.1.4/coldfront/core/resource/migrations/0002_auto_20191017_1141.py
--rw-r--r--   0 aeb       (1000) aeb       (1000)        0 2021-02-25 21:11:22.000000 coldfront-1.1.4/coldfront/core/resource/migrations/__init__.py
--rw-r--r--   0 aeb       (1000) aeb       (1000)    11484 2022-01-07 20:54:01.000000 coldfront-1.1.4/coldfront/core/resource/models.py
-drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-02-12 02:48:33.346168 coldfront-1.1.4/coldfront/core/resource/templates/
--rw-r--r--   0 aeb       (1000) aeb       (1000)     5371 2022-03-07 19:51:38.000000 coldfront-1.1.4/coldfront/core/resource/templates/resource_detail.html
--rw-r--r--   0 aeb       (1000) aeb       (1000)     5257 2022-09-20 14:51:20.000000 coldfront-1.1.4/coldfront/core/resource/templates/resource_list.html
--rw-r--r--   0 aeb       (1000) aeb       (1000)      500 2022-03-07 19:51:38.000000 coldfront-1.1.4/coldfront/core/resource/templates/resource_resourceattribute_create.html
--rw-r--r--   0 aeb       (1000) aeb       (1000)     2218 2022-03-07 19:51:38.000000 coldfront-1.1.4/coldfront/core/resource/templates/resource_resourceattribute_delete.html
--rw-r--r--   0 aeb       (1000) aeb       (1000)       60 2023-02-09 20:15:46.000000 coldfront-1.1.4/coldfront/core/resource/tests.py
--rw-r--r--   0 aeb       (1000) aeb       (1000)      574 2022-03-07 19:51:38.000000 coldfront-1.1.4/coldfront/core/resource/urls.py
--rw-r--r--   0 aeb       (1000) aeb       (1000)    12279 2022-09-20 14:51:20.000000 coldfront-1.1.4/coldfront/core/resource/views.py
-drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-02-12 02:48:33.346168 coldfront-1.1.4/coldfront/core/user/
--rw-r--r--   0 aeb       (1000) aeb       (1000)       59 2021-02-25 21:11:22.000000 coldfront-1.1.4/coldfront/core/user/__init__.py
--rw-r--r--   0 aeb       (1000) aeb       (1000)      529 2021-02-25 21:11:22.000000 coldfront-1.1.4/coldfront/core/user/admin.py
--rw-r--r--   0 aeb       (1000) aeb       (1000)      163 2021-02-25 21:11:22.000000 coldfront-1.1.4/coldfront/core/user/apps.py
--rw-r--r--   0 aeb       (1000) aeb       (1000)      918 2022-09-29 18:05:12.000000 coldfront-1.1.4/coldfront/core/user/forms.py
-drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-02-12 02:48:33.346168 coldfront-1.1.4/coldfront/core/user/migrations/
--rw-r--r--   0 aeb       (1000) aeb       (1000)      749 2021-02-25 21:11:22.000000 coldfront-1.1.4/coldfront/core/user/migrations/0001_initial.py
--rw-r--r--   0 aeb       (1000) aeb       (1000)        0 2021-02-25 21:11:22.000000 coldfront-1.1.4/coldfront/core/user/migrations/__init__.py
--rw-r--r--   0 aeb       (1000) aeb       (1000)      219 2022-09-29 18:05:12.000000 coldfront-1.1.4/coldfront/core/user/models.py
--rw-r--r--   0 aeb       (1000) aeb       (1000)      518 2021-02-25 21:11:22.000000 coldfront-1.1.4/coldfront/core/user/signals.py
-drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-02-12 02:48:33.318167 coldfront-1.1.4/coldfront/core/user/templates/
-drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-02-12 02:48:33.346168 coldfront-1.1.4/coldfront/core/user/templates/user/
--rw-r--r--   0 aeb       (1000) aeb       (1000)     1316 2022-02-07 13:09:25.000000 coldfront-1.1.4/coldfront/core/user/templates/user/login.html
--rw-r--r--   0 aeb       (1000) aeb       (1000)      303 2023-02-09 20:15:46.000000 coldfront-1.1.4/coldfront/core/user/templates/user/login_form.html
--rw-r--r--   0 aeb       (1000) aeb       (1000)     2025 2022-03-09 21:14:23.000000 coldfront-1.1.4/coldfront/core/user/templates/user/user_list_allocations.html
--rw-r--r--   0 aeb       (1000) aeb       (1000)     2549 2022-09-29 18:05:12.000000 coldfront-1.1.4/coldfront/core/user/templates/user/user_profile.html
--rw-r--r--   0 aeb       (1000) aeb       (1000)     5500 2022-02-07 13:09:25.000000 coldfront-1.1.4/coldfront/core/user/templates/user/user_projects_managers.html
--rw-r--r--   0 aeb       (1000) aeb       (1000)     2638 2021-02-25 21:11:22.000000 coldfront-1.1.4/coldfront/core/user/templates/user/user_search_home.html
--rw-r--r--   0 aeb       (1000) aeb       (1000)     1257 2021-02-25 21:11:22.000000 coldfront-1.1.4/coldfront/core/user/templates/user/user_search_results.html
--rw-r--r--   0 aeb       (1000) aeb       (1000)     1669 2023-02-09 20:15:46.000000 coldfront-1.1.4/coldfront/core/user/tests.py
--rw-r--r--   0 aeb       (1000) aeb       (1000)     1356 2022-09-29 18:05:12.000000 coldfront-1.1.4/coldfront/core/user/urls.py
--rw-r--r--   0 aeb       (1000) aeb       (1000)     4301 2021-07-20 15:45:35.000000 coldfront-1.1.4/coldfront/core/user/utils.py
--rw-r--r--   0 aeb       (1000) aeb       (1000)     9968 2022-09-29 18:05:12.000000 coldfront-1.1.4/coldfront/core/user/views.py
-drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-02-12 02:48:33.350168 coldfront-1.1.4/coldfront/core/utils/
--rw-r--r--   0 aeb       (1000) aeb       (1000)        0 2021-02-25 21:11:22.000000 coldfront-1.1.4/coldfront/core/utils/__init__.py
--rw-r--r--   0 aeb       (1000) aeb       (1000)       63 2021-02-25 21:11:22.000000 coldfront-1.1.4/coldfront/core/utils/admin.py
--rw-r--r--   0 aeb       (1000) aeb       (1000)      137 2022-02-07 13:09:25.000000 coldfront-1.1.4/coldfront/core/utils/apps.py
--rw-r--r--   0 aeb       (1000) aeb       (1000)     1272 2021-02-25 21:11:22.000000 coldfront-1.1.4/coldfront/core/utils/common.py
-drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-02-12 02:48:33.350168 coldfront-1.1.4/coldfront/core/utils/fixtures/
--rw-r--r--   0 aeb       (1000) aeb       (1000)        0 2021-02-25 21:11:22.000000 coldfront-1.1.4/coldfront/core/utils/fixtures/__init__.py
--rw-r--r--   0 aeb       (1000) aeb       (1000)     4710 2022-09-23 21:50:06.000000 coldfront-1.1.4/coldfront/core/utils/mail.py
-drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-02-12 02:48:33.350168 coldfront-1.1.4/coldfront/core/utils/management/
--rw-r--r--   0 aeb       (1000) aeb       (1000)        0 2021-03-03 01:27:01.000000 coldfront-1.1.4/coldfront/core/utils/management/__init__.py
-drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-02-12 02:48:33.350168 coldfront-1.1.4/coldfront/core/utils/management/commands/
--rw-r--r--   0 aeb       (1000) aeb       (1000)        0 2021-03-03 01:27:01.000000 coldfront-1.1.4/coldfront/core/utils/management/commands/__init__.py
--rw-r--r--   0 aeb       (1000) aeb       (1000)      763 2021-03-02 21:10:03.000000 coldfront-1.1.4/coldfront/core/utils/management/commands/add_scheduled_tasks.py
--rw-r--r--   0 aeb       (1000) aeb       (1000)     7506 2021-02-25 21:11:22.000000 coldfront-1.1.4/coldfront/core/utils/management/commands/import_grants.py
--rw-r--r--   0 aeb       (1000) aeb       (1000)     5372 2021-02-25 21:11:22.000000 coldfront-1.1.4/coldfront/core/utils/management/commands/import_projects.py
--rw-r--r--   0 aeb       (1000) aeb       (1000)     2591 2021-02-25 21:11:22.000000 coldfront-1.1.4/coldfront/core/utils/management/commands/import_publications.py
--rw-r--r--   0 aeb       (1000) aeb       (1000)     5630 2021-02-25 21:11:22.000000 coldfront-1.1.4/coldfront/core/utils/management/commands/import_resources.py
--rw-r--r--   0 aeb       (1000) aeb       (1000)     6535 2021-02-25 21:11:22.000000 coldfront-1.1.4/coldfront/core/utils/management/commands/import_resources_from_json.py
--rw-r--r--   0 aeb       (1000) aeb       (1000)     8817 2021-02-25 21:11:22.000000 coldfront-1.1.4/coldfront/core/utils/management/commands/import_subscriptions.py
--rw-r--r--   0 aeb       (1000) aeb       (1000)     1774 2021-02-25 21:11:22.000000 coldfront-1.1.4/coldfront/core/utils/management/commands/import_users.py
--rw-r--r--   0 aeb       (1000) aeb       (1000)     1419 2022-12-06 13:04:35.000000 coldfront-1.1.4/coldfront/core/utils/management/commands/initial_setup.py
--rw-r--r--   0 aeb       (1000) aeb       (1000)    28403 2023-02-09 20:03:17.000000 coldfront-1.1.4/coldfront/core/utils/management/commands/load_test_data.py
--rw-r--r--   0 aeb       (1000) aeb       (1000)     1236 2021-02-25 21:11:22.000000 coldfront-1.1.4/coldfront/core/utils/management/commands/show_users_in_project_but_not_in_allocation.py
-drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-02-12 02:48:33.350168 coldfront-1.1.4/coldfront/core/utils/migrations/
--rw-r--r--   0 aeb       (1000) aeb       (1000)        0 2021-02-25 21:11:22.000000 coldfront-1.1.4/coldfront/core/utils/migrations/__init__.py
-drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-02-12 02:48:33.350168 coldfront-1.1.4/coldfront/core/utils/mixins/
--rw-r--r--   0 aeb       (1000) aeb       (1000)        0 2021-02-26 20:30:52.000000 coldfront-1.1.4/coldfront/core/utils/mixins/__init__.py
--rw-r--r--   0 aeb       (1000) aeb       (1000)     2548 2021-02-25 21:11:22.000000 coldfront-1.1.4/coldfront/core/utils/mixins/views.py
--rw-r--r--   0 aeb       (1000) aeb       (1000)       57 2021-02-25 21:11:22.000000 coldfront-1.1.4/coldfront/core/utils/models.py
-drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-02-12 02:48:33.350168 coldfront-1.1.4/coldfront/core/utils/templatetags/
--rw-r--r--   0 aeb       (1000) aeb       (1000)        0 2021-03-03 01:27:01.000000 coldfront-1.1.4/coldfront/core/utils/templatetags/__init__.py
--rw-r--r--   0 aeb       (1000) aeb       (1000)     1900 2021-02-25 21:11:22.000000 coldfront-1.1.4/coldfront/core/utils/templatetags/common_tags.py
--rw-r--r--   0 aeb       (1000) aeb       (1000)       60 2023-02-09 20:15:46.000000 coldfront-1.1.4/coldfront/core/utils/tests.py
--rw-r--r--   0 aeb       (1000) aeb       (1000)     1360 2022-11-23 21:22:01.000000 coldfront-1.1.4/coldfront/core/utils/validate.py
--rw-r--r--   0 aeb       (1000) aeb       (1000)       63 2021-02-25 21:11:22.000000 coldfront-1.1.4/coldfront/core/utils/views.py
-drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-02-12 02:48:33.350168 coldfront-1.1.4/coldfront/plugins/
--rw-r--r--   0 aeb       (1000) aeb       (1000)        0 2021-02-25 21:11:22.000000 coldfront-1.1.4/coldfront/plugins/__init__.py
-drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-02-12 02:48:33.354168 coldfront-1.1.4/coldfront/plugins/freeipa/
--rw-r--r--   0 aeb       (1000) aeb       (1000)       64 2021-02-25 21:11:22.000000 coldfront-1.1.4/coldfront/plugins/freeipa/__init__.py
--rw-r--r--   0 aeb       (1000) aeb       (1000)      354 2021-02-25 21:11:22.000000 coldfront-1.1.4/coldfront/plugins/freeipa/apps.py
-drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-02-12 02:48:33.354168 coldfront-1.1.4/coldfront/plugins/freeipa/management/
--rw-r--r--   0 aeb       (1000) aeb       (1000)        0 2021-02-25 21:11:22.000000 coldfront-1.1.4/coldfront/plugins/freeipa/management/__init__.py
-drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-02-12 02:48:33.354168 coldfront-1.1.4/coldfront/plugins/freeipa/management/commands/
--rw-r--r--   0 aeb       (1000) aeb       (1000)        0 2021-02-25 21:11:22.000000 coldfront-1.1.4/coldfront/plugins/freeipa/management/commands/__init__.py
--rw-r--r--   0 aeb       (1000) aeb       (1000)    10200 2022-08-05 14:28:00.000000 coldfront-1.1.4/coldfront/plugins/freeipa/management/commands/freeipa_check.py
--rw-r--r--   0 aeb       (1000) aeb       (1000)     4189 2021-02-25 21:11:22.000000 coldfront-1.1.4/coldfront/plugins/freeipa/management/commands/freeipa_expire_users.py
--rw-r--r--   0 aeb       (1000) aeb       (1000)     3353 2021-02-25 21:11:22.000000 coldfront-1.1.4/coldfront/plugins/freeipa/search.py
--rw-r--r--   0 aeb       (1000) aeb       (1000)     1338 2023-02-09 20:05:18.000000 coldfront-1.1.4/coldfront/plugins/freeipa/signals.py
--rw-r--r--   0 aeb       (1000) aeb       (1000)     4782 2021-02-25 21:11:22.000000 coldfront-1.1.4/coldfront/plugins/freeipa/tasks.py
--rw-r--r--   0 aeb       (1000) aeb       (1000)     1408 2021-02-25 21:11:22.000000 coldfront-1.1.4/coldfront/plugins/freeipa/utils.py
-drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-02-12 02:48:33.354168 coldfront-1.1.4/coldfront/plugins/iquota/
--rw-r--r--   0 aeb       (1000) aeb       (1000)        0 2021-02-25 21:11:22.000000 coldfront-1.1.4/coldfront/plugins/iquota/__init__.py
--rw-r--r--   0 aeb       (1000) aeb       (1000)       63 2021-02-25 21:11:22.000000 coldfront-1.1.4/coldfront/plugins/iquota/admin.py
--rw-r--r--   0 aeb       (1000) aeb       (1000)      105 2022-02-07 13:09:25.000000 coldfront-1.1.4/coldfront/plugins/iquota/apps.py
--rw-r--r--   0 aeb       (1000) aeb       (1000)      276 2021-02-25 21:11:22.000000 coldfront-1.1.4/coldfront/plugins/iquota/exceptions.py
-drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-02-12 02:48:33.354168 coldfront-1.1.4/coldfront/plugins/iquota/migrations/
--rw-r--r--   0 aeb       (1000) aeb       (1000)        0 2021-02-25 21:11:22.000000 coldfront-1.1.4/coldfront/plugins/iquota/migrations/__init__.py
-drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-02-12 02:48:33.318167 coldfront-1.1.4/coldfront/plugins/iquota/templates/
-drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-02-12 02:48:33.354168 coldfront-1.1.4/coldfront/plugins/iquota/templates/iquota/
--rw-r--r--   0 aeb       (1000) aeb       (1000)     1711 2021-02-25 21:11:22.000000 coldfront-1.1.4/coldfront/plugins/iquota/templates/iquota/iquota.html
--rw-r--r--   0 aeb       (1000) aeb       (1000)      955 2021-02-25 21:11:22.000000 coldfront-1.1.4/coldfront/plugins/iquota/templates/iquota/iquota_div.html
--rw-r--r--   0 aeb       (1000) aeb       (1000)      183 2021-02-25 21:11:22.000000 coldfront-1.1.4/coldfront/plugins/iquota/urls.py
--rw-r--r--   0 aeb       (1000) aeb       (1000)     3548 2021-03-25 01:57:34.000000 coldfront-1.1.4/coldfront/plugins/iquota/utils.py
--rw-r--r--   0 aeb       (1000) aeb       (1000)      639 2021-02-25 21:11:22.000000 coldfront-1.1.4/coldfront/plugins/iquota/views.py
-drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-02-12 02:48:33.354168 coldfront-1.1.4/coldfront/plugins/ldap_user_search/
--rw-r--r--   0 aeb       (1000) aeb       (1000)        0 2021-02-25 21:11:22.000000 coldfront-1.1.4/coldfront/plugins/ldap_user_search/__init__.py
--rw-r--r--   0 aeb       (1000) aeb       (1000)       63 2021-02-25 21:11:22.000000 coldfront-1.1.4/coldfront/plugins/ldap_user_search/admin.py
--rw-r--r--   0 aeb       (1000) aeb       (1000)      123 2022-02-07 13:09:25.000000 coldfront-1.1.4/coldfront/plugins/ldap_user_search/apps.py
-drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-02-12 02:48:33.354168 coldfront-1.1.4/coldfront/plugins/ldap_user_search/migrations/
--rw-r--r--   0 aeb       (1000) aeb       (1000)        0 2021-02-25 21:11:22.000000 coldfront-1.1.4/coldfront/plugins/ldap_user_search/migrations/__init__.py
--rw-r--r--   0 aeb       (1000) aeb       (1000)       57 2021-02-25 21:11:22.000000 coldfront-1.1.4/coldfront/plugins/ldap_user_search/models.py
--rw-r--r--   0 aeb       (1000) aeb       (1000)       60 2023-02-09 20:15:46.000000 coldfront-1.1.4/coldfront/plugins/ldap_user_search/tests.py
--rw-r--r--   0 aeb       (1000) aeb       (1000)     2824 2022-01-12 23:53:55.000000 coldfront-1.1.4/coldfront/plugins/ldap_user_search/utils.py
--rw-r--r--   0 aeb       (1000) aeb       (1000)       63 2021-02-25 21:11:22.000000 coldfront-1.1.4/coldfront/plugins/ldap_user_search/views.py
-drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-02-12 02:48:33.354168 coldfront-1.1.4/coldfront/plugins/mokey_oidc/
--rw-r--r--   0 aeb       (1000) aeb       (1000)        0 2021-02-25 21:11:22.000000 coldfront-1.1.4/coldfront/plugins/mokey_oidc/__init__.py
--rw-r--r--   0 aeb       (1000) aeb       (1000)      112 2022-02-07 13:09:25.000000 coldfront-1.1.4/coldfront/plugins/mokey_oidc/apps.py
--rw-r--r--   0 aeb       (1000) aeb       (1000)     3222 2021-11-10 16:20:52.000000 coldfront-1.1.4/coldfront/plugins/mokey_oidc/auth.py
-drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-02-12 02:48:33.354168 coldfront-1.1.4/coldfront/plugins/mokey_oidc/migrations/
--rw-r--r--   0 aeb       (1000) aeb       (1000)        0 2021-02-25 21:11:22.000000 coldfront-1.1.4/coldfront/plugins/mokey_oidc/migrations/__init__.py
-drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-02-12 02:48:33.354168 coldfront-1.1.4/coldfront/plugins/slurm/
--rw-r--r--   0 aeb       (1000) aeb       (1000)       64 2021-02-25 21:11:22.000000 coldfront-1.1.4/coldfront/plugins/slurm/__init__.py
--rw-r--r--   0 aeb       (1000) aeb       (1000)      103 2021-02-25 21:11:22.000000 coldfront-1.1.4/coldfront/plugins/slurm/apps.py
--rw-r--r--   0 aeb       (1000) aeb       (1000)     9271 2022-09-20 14:51:20.000000 coldfront-1.1.4/coldfront/plugins/slurm/associations.py
-drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-02-12 02:48:33.354168 coldfront-1.1.4/coldfront/plugins/slurm/management/
--rw-r--r--   0 aeb       (1000) aeb       (1000)        0 2021-02-25 21:11:22.000000 coldfront-1.1.4/coldfront/plugins/slurm/management/__init__.py
-drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-02-12 02:48:33.358168 coldfront-1.1.4/coldfront/plugins/slurm/management/commands/
--rw-r--r--   0 aeb       (1000) aeb       (1000)        0 2021-02-25 21:11:22.000000 coldfront-1.1.4/coldfront/plugins/slurm/management/commands/__init__.py
--rw-r--r--   0 aeb       (1000) aeb       (1000)    10552 2021-02-25 21:11:22.000000 coldfront-1.1.4/coldfront/plugins/slurm/management/commands/slurm_check.py
--rw-r--r--   0 aeb       (1000) aeb       (1000)     1872 2021-03-25 01:57:34.000000 coldfront-1.1.4/coldfront/plugins/slurm/management/commands/slurm_dump.py
--rw-r--r--   0 aeb       (1000) aeb       (1000)     4540 2021-02-25 21:11:22.000000 coldfront-1.1.4/coldfront/plugins/slurm/utils.py
-drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-02-12 02:48:33.358168 coldfront-1.1.4/coldfront/plugins/system_monitor/
--rw-r--r--   0 aeb       (1000) aeb       (1000)        0 2021-02-25 21:11:22.000000 coldfront-1.1.4/coldfront/plugins/system_monitor/__init__.py
-drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-02-12 02:48:33.318167 coldfront-1.1.4/coldfront/plugins/system_monitor/templates/
-drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-02-12 02:48:33.358168 coldfront-1.1.4/coldfront/plugins/system_monitor/templates/system_monitor/
--rw-r--r--   0 aeb       (1000) aeb       (1000)     2305 2022-02-07 13:09:25.000000 coldfront-1.1.4/coldfront/plugins/system_monitor/templates/system_monitor/system_monitor_div.html
--rw-r--r--   0 aeb       (1000) aeb       (1000)     5627 2021-02-25 21:11:22.000000 coldfront-1.1.4/coldfront/plugins/system_monitor/utils.py
-drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-02-12 02:48:33.358168 coldfront-1.1.4/coldfront/plugins/xdmod/
--rw-r--r--   0 aeb       (1000) aeb       (1000)       64 2021-02-25 21:11:22.000000 coldfront-1.1.4/coldfront/plugins/xdmod/__init__.py
--rw-r--r--   0 aeb       (1000) aeb       (1000)      103 2021-02-25 21:11:22.000000 coldfront-1.1.4/coldfront/plugins/xdmod/apps.py
-drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-02-12 02:48:33.358168 coldfront-1.1.4/coldfront/plugins/xdmod/management/
--rw-r--r--   0 aeb       (1000) aeb       (1000)        0 2021-02-25 21:11:22.000000 coldfront-1.1.4/coldfront/plugins/xdmod/management/__init__.py
-drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-02-12 02:48:33.358168 coldfront-1.1.4/coldfront/plugins/xdmod/management/commands/
--rw-r--r--   0 aeb       (1000) aeb       (1000)        0 2021-02-25 21:11:22.000000 coldfront-1.1.4/coldfront/plugins/xdmod/management/commands/__init__.py
--rw-r--r--   0 aeb       (1000) aeb       (1000)    18434 2022-10-09 13:46:08.000000 coldfront-1.1.4/coldfront/plugins/xdmod/management/commands/xdmod_usage.py
--rw-r--r--   0 aeb       (1000) aeb       (1000)     6492 2022-10-09 13:46:08.000000 coldfront-1.1.4/coldfront/plugins/xdmod/utils.py
-drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-02-12 02:48:33.318167 coldfront-1.1.4/coldfront/static/
-drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-02-12 02:48:33.358168 coldfront-1.1.4/coldfront/static/bootstrap/
--rw-r--r--   0 aeb       (1000) aeb       (1000)    83253 2022-07-07 16:08:59.000000 coldfront-1.1.4/coldfront/static/bootstrap/bootstrap.bundle.min.js
--rw-r--r--   0 aeb       (1000) aeb       (1000)   311239 2022-07-07 16:08:59.000000 coldfront-1.1.4/coldfront/static/bootstrap/bootstrap.bundle.min.js.map
--rw-r--r--   0 aeb       (1000) aeb       (1000)   162017 2022-07-07 16:08:59.000000 coldfront-1.1.4/coldfront/static/bootstrap/bootstrap.min.css
--rw-r--r--   0 aeb       (1000) aeb       (1000)   653535 2022-07-07 16:08:59.000000 coldfront-1.1.4/coldfront/static/bootstrap/bootstrap.min.css.map
-drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-02-12 02:48:33.358168 coldfront-1.1.4/coldfront/static/c3js/
--rwxr-xr-x   0 aeb       (1000) aeb       (1000)     2386 2021-02-25 21:11:22.000000 coldfront-1.1.4/coldfront/static/c3js/c3.min.css
--rwxr-xr-x   0 aeb       (1000) aeb       (1000)   191799 2022-07-07 14:47:15.000000 coldfront-1.1.4/coldfront/static/c3js/c3.min.js
-drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-02-12 02:48:33.318167 coldfront-1.1.4/coldfront/static/coldfront/
-drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-02-12 02:48:33.318167 coldfront-1.1.4/coldfront/static/coldfront/plugins/
-drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-02-12 02:48:33.318167 coldfront-1.1.4/coldfront/static/coldfront/plugins/system_monitor/
-drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-02-12 02:48:33.358168 coldfront-1.1.4/coldfront/static/coldfront/plugins/system_monitor/images/
--rw-r--r--   0 aeb       (1000) aeb       (1000)    42418 2021-02-25 21:11:22.000000 coldfront-1.1.4/coldfront/static/coldfront/plugins/system_monitor/images/xdmod.png
-drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-02-12 02:48:33.358168 coldfront-1.1.4/coldfront/static/common/
-drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-02-12 02:48:33.358168 coldfront-1.1.4/coldfront/static/common/css/
--rw-r--r--   0 aeb       (1000) aeb       (1000)     3925 2022-09-29 18:05:12.000000 coldfront-1.1.4/coldfront/static/common/css/common.css
-drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-02-12 02:48:33.362168 coldfront-1.1.4/coldfront/static/common/images/
--rw-r--r--   0 aeb       (1000) aeb       (1000)    12165 2022-07-07 22:12:57.000000 coldfront-1.1.4/coldfront/static/common/images/android-chrome-192x192.png
--rw-r--r--   0 aeb       (1000) aeb       (1000)    30499 2022-07-07 22:12:57.000000 coldfront-1.1.4/coldfront/static/common/images/android-chrome-512x512.png
--rw-r--r--   0 aeb       (1000) aeb       (1000)    10941 2022-07-07 22:12:57.000000 coldfront-1.1.4/coldfront/static/common/images/apple-touch-icon.png
--rw-r--r--   0 aeb       (1000) aeb       (1000)      626 2022-07-07 22:12:57.000000 coldfront-1.1.4/coldfront/static/common/images/favicon-16x16.png
--rw-r--r--   0 aeb       (1000) aeb       (1000)     1431 2022-07-07 22:12:57.000000 coldfront-1.1.4/coldfront/static/common/images/favicon-32x32.png
--rw-r--r--   0 aeb       (1000) aeb       (1000)    15406 2022-07-07 22:12:57.000000 coldfront-1.1.4/coldfront/static/common/images/favicon.ico
--rw-r--r--   0 aeb       (1000) aeb       (1000)   121290 2022-07-07 22:12:57.000000 coldfront-1.1.4/coldfront/static/common/images/logo.png
--rw-r--r--   0 aeb       (1000) aeb       (1000)      306 2022-07-07 22:12:57.000000 coldfront-1.1.4/coldfront/static/common/site.webmanifest
-drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-02-12 02:48:33.318167 coldfront-1.1.4/coldfront/static/core/
-drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-02-12 02:48:33.318167 coldfront-1.1.4/coldfront/static/core/portal/
-drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-02-12 02:48:33.362168 coldfront-1.1.4/coldfront/static/core/portal/imgs/
--rw-r--r--   0 aeb       (1000) aeb       (1000)   418141 2021-02-25 21:11:22.000000 coldfront-1.1.4/coldfront/static/core/portal/imgs/airport-business-cabinets-236093.jpg
--rw-r--r--   0 aeb       (1000) aeb       (1000)  1148253 2021-02-25 21:11:22.000000 coldfront-1.1.4/coldfront/static/core/portal/imgs/analogue-blur-business-159282.jpg
--rw-r--r--   0 aeb       (1000) aeb       (1000)   954249 2021-02-25 21:11:22.000000 coldfront-1.1.4/coldfront/static/core/portal/imgs/computer-electronics-equipment-325223.jpg
--rw-r--r--   0 aeb       (1000) aeb       (1000)     5118 2021-02-25 21:11:22.000000 coldfront-1.1.4/coldfront/static/core/portal/imgs/ondemand.png
-drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-02-12 02:48:33.362168 coldfront-1.1.4/coldfront/static/d3/
--rw-r--r--   0 aeb       (1000) aeb       (1000)   237682 2022-07-07 14:47:15.000000 coldfront-1.1.4/coldfront/static/d3/d3.v5.min.js
-drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-02-12 02:48:33.366168 coldfront-1.1.4/coldfront/static/datatable/
--rw-r--r--   0 aeb       (1000) aeb       (1000)     5222 2022-07-07 16:08:59.000000 coldfront-1.1.4/coldfront/static/datatable/dataTables.bootstrap4.min.css
--rw-r--r--   0 aeb       (1000) aeb       (1000)     2085 2022-07-07 16:08:59.000000 coldfront-1.1.4/coldfront/static/datatable/dataTables.bootstrap4.min.js
--rw-r--r--   0 aeb       (1000) aeb       (1000)    82411 2022-07-07 16:08:59.000000 coldfront-1.1.4/coldfront/static/datatable/jquery.dataTables.min.js
-drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-02-12 02:48:33.366168 coldfront-1.1.4/coldfront/static/flatpickr/
--rw-r--r--   0 aeb       (1000) aeb       (1000)    50679 2022-09-20 14:51:20.000000 coldfront-1.1.4/coldfront/static/flatpickr/flatpickr.js
--rw-r--r--   0 aeb       (1000) aeb       (1000)    16166 2022-09-20 14:51:20.000000 coldfront-1.1.4/coldfront/static/flatpickr/flatpickr.min.css
-drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-02-12 02:48:33.366168 coldfront-1.1.4/coldfront/static/jquery/
--rw-r--r--   0 aeb       (1000) aeb       (1000)    89501 2022-07-07 16:08:59.000000 coldfront-1.1.4/coldfront/static/jquery/jquery-3.6.0.min.js
-drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-02-12 02:48:33.366168 coldfront-1.1.4/coldfront/static/select2/
--rw-r--r--   0 aeb       (1000) aeb       (1000)    15275 2022-07-07 16:08:59.000000 coldfront-1.1.4/coldfront/static/select2/select2.min.css
--rw-r--r--   0 aeb       (1000) aeb       (1000)    67751 2022-07-07 16:08:59.000000 coldfront-1.1.4/coldfront/static/select2/select2.min.js
-drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-02-12 02:48:33.366168 coldfront-1.1.4/coldfront/templates/
--rw-r--r--   0 aeb       (1000) aeb       (1000)      396 2023-02-09 20:05:18.000000 coldfront-1.1.4/coldfront/templates/400.html
--rw-r--r--   0 aeb       (1000) aeb       (1000)      418 2021-03-25 01:57:34.000000 coldfront-1.1.4/coldfront/templates/403.html
--rw-r--r--   0 aeb       (1000) aeb       (1000)      425 2021-02-25 21:11:22.000000 coldfront-1.1.4/coldfront/templates/404.html
--rw-r--r--   0 aeb       (1000) aeb       (1000)      456 2021-02-25 21:11:22.000000 coldfront-1.1.4/coldfront/templates/500.html
-drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-02-12 02:48:33.366168 coldfront-1.1.4/coldfront/templates/common/
--rw-r--r--   0 aeb       (1000) aeb       (1000)     2470 2023-02-09 20:15:46.000000 coldfront-1.1.4/coldfront/templates/common/authorized_navbar.html
--rw-r--r--   0 aeb       (1000) aeb       (1000)     2530 2022-09-20 14:51:20.000000 coldfront-1.1.4/coldfront/templates/common/base.html
--rw-r--r--   0 aeb       (1000) aeb       (1000)      357 2021-02-25 21:11:22.000000 coldfront-1.1.4/coldfront/templates/common/footer.html
--rw-r--r--   0 aeb       (1000) aeb       (1000)      289 2021-02-25 21:11:22.000000 coldfront-1.1.4/coldfront/templates/common/messages.html
--rw-r--r--   0 aeb       (1000) aeb       (1000)     1140 2023-02-09 20:15:46.000000 coldfront-1.1.4/coldfront/templates/common/navbar_admin.html
--rw-r--r--   0 aeb       (1000) aeb       (1000)      444 2022-07-07 22:12:57.000000 coldfront-1.1.4/coldfront/templates/common/navbar_brand.html
--rw-r--r--   0 aeb       (1000) aeb       (1000)      686 2022-03-07 19:51:38.000000 coldfront-1.1.4/coldfront/templates/common/navbar_director.html
--rw-r--r--   0 aeb       (1000) aeb       (1000)      140 2022-07-07 13:52:57.000000 coldfront-1.1.4/coldfront/templates/common/navbar_help.html
--rw-r--r--   0 aeb       (1000) aeb       (1000)      321 2021-02-25 21:11:22.000000 coldfront-1.1.4/coldfront/templates/common/navbar_invoice.html
--rw-r--r--   0 aeb       (1000) aeb       (1000)      523 2021-02-25 21:11:22.000000 coldfront-1.1.4/coldfront/templates/common/navbar_login.html
--rw-r--r--   0 aeb       (1000) aeb       (1000)     1501 2022-03-07 19:51:38.000000 coldfront-1.1.4/coldfront/templates/common/navbar_nonadmin_staff.html
--rw-r--r--   0 aeb       (1000) aeb       (1000)     1123 2022-07-07 13:52:57.000000 coldfront-1.1.4/coldfront/templates/common/nonauthorized_navbar.html
-drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-02-12 02:48:33.370168 coldfront-1.1.4/coldfront/templates/email/
--rw-r--r--   0 aeb       (1000) aeb       (1000)      710 2022-09-20 14:51:20.000000 coldfront-1.1.4/coldfront/templates/email/admin_allocation_expired.txt
--rw-r--r--   0 aeb       (1000) aeb       (1000)      432 2023-02-10 02:08:24.000000 coldfront-1.1.4/coldfront/templates/email/allocation_activated.txt
--rw-r--r--   0 aeb       (1000) aeb       (1000)      454 2023-02-10 02:08:24.000000 coldfront-1.1.4/coldfront/templates/email/allocation_change_approved.txt
--rw-r--r--   0 aeb       (1000) aeb       (1000)      470 2023-02-10 02:08:24.000000 coldfront-1.1.4/coldfront/templates/email/allocation_change_denied.txt
--rw-r--r--   0 aeb       (1000) aeb       (1000)      403 2023-02-10 02:08:24.000000 coldfront-1.1.4/coldfront/templates/email/allocation_denied.txt
--rw-r--r--   0 aeb       (1000) aeb       (1000)     1447 2022-09-20 14:51:20.000000 coldfront-1.1.4/coldfront/templates/email/allocation_expired.txt
--rw-r--r--   0 aeb       (1000) aeb       (1000)     1430 2022-09-20 14:51:20.000000 coldfront-1.1.4/coldfront/templates/email/allocation_expiring.txt
--rw-r--r--   0 aeb       (1000) aeb       (1000)       97 2021-02-25 21:11:22.000000 coldfront-1.1.4/coldfront/templates/email/allocation_renewed.txt
--rw-r--r--   0 aeb       (1000) aeb       (1000)      396 2023-02-10 02:08:24.000000 coldfront-1.1.4/coldfront/templates/email/allocation_revoked.txt
--rw-r--r--   0 aeb       (1000) aeb       (1000)      116 2022-02-07 13:09:25.000000 coldfront-1.1.4/coldfront/templates/email/new_allocation_change_request.txt
--rw-r--r--   0 aeb       (1000) aeb       (1000)      103 2021-02-25 21:11:22.000000 coldfront-1.1.4/coldfront/templates/email/new_allocation_request.txt
--rw-r--r--   0 aeb       (1000) aeb       (1000)       94 2021-02-25 21:11:22.000000 coldfront-1.1.4/coldfront/templates/email/new_project_review.txt
--rw-r--r--   0 aeb       (1000) aeb       (1000)      155 2021-02-25 21:11:22.000000 coldfront-1.1.4/coldfront/templates/email/upgrade_account_request.txt
--rw-r--r--   0 aeb       (1000) aeb       (1000)      238 2021-02-25 21:11:22.000000 coldfront-1.1.4/coldfront/templates/robots.txt
-drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-02-12 02:48:33.370168 coldfront-1.1.4/coldfront/templates/su/
--rw-r--r--   0 aeb       (1000) aeb       (1000)      497 2021-02-25 21:11:22.000000 coldfront-1.1.4/coldfront/templates/su/is_su.html
-drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-02-12 02:48:33.322167 coldfront-1.1.4/coldfront.egg-info/
--rw-r--r--   0 aeb       (1000) aeb       (1000)     2979 2023-02-12 02:48:33.000000 coldfront-1.1.4/coldfront.egg-info/PKG-INFO
--rw-r--r--   0 aeb       (1000) aeb       (1000)    17464 2023-02-12 02:48:33.000000 coldfront-1.1.4/coldfront.egg-info/SOURCES.txt
--rw-r--r--   0 aeb       (1000) aeb       (1000)        1 2023-02-12 02:48:33.000000 coldfront-1.1.4/coldfront.egg-info/dependency_links.txt
--rw-r--r--   0 aeb       (1000) aeb       (1000)       47 2023-02-12 02:48:33.000000 coldfront-1.1.4/coldfront.egg-info/entry_points.txt
--rw-r--r--   0 aeb       (1000) aeb       (1000)      643 2023-02-12 02:48:33.000000 coldfront-1.1.4/coldfront.egg-info/requires.txt
--rw-r--r--   0 aeb       (1000) aeb       (1000)       10 2023-02-12 02:48:33.000000 coldfront-1.1.4/coldfront.egg-info/top_level.txt
--rw-r--r--   0 aeb       (1000) aeb       (1000)       38 2023-02-12 02:48:33.370168 coldfront-1.1.4/setup.cfg
--rw-r--r--   0 aeb       (1000) aeb       (1000)     2371 2023-02-09 20:03:17.000000 coldfront-1.1.4/setup.py
+drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-07-13 00:45:36.947884 coldfront-1.1.5/
+-rw-r--r--   0 aeb       (1000) aeb       (1000)      482 2023-07-13 00:35:23.000000 coldfront-1.1.5/AUTHORS.md
+-rw-r--r--   0 aeb       (1000) aeb       (1000)    35147 2021-02-25 21:11:22.000000 coldfront-1.1.5/LICENSE
+-rw-r--r--   0 aeb       (1000) aeb       (1000)      706 2022-03-09 21:14:23.000000 coldfront-1.1.5/MANIFEST.in
+-rw-r--r--   0 aeb       (1000) aeb       (1000)     3428 2023-07-13 00:45:36.947884 coldfront-1.1.5/PKG-INFO
+-rw-r--r--   0 aeb       (1000) aeb       (1000)     2520 2023-04-20 18:12:49.000000 coldfront-1.1.5/README.md
+drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-07-13 00:45:36.895883 coldfront-1.1.5/coldfront/
+-rw-r--r--   0 aeb       (1000) aeb       (1000)      268 2023-07-13 00:38:05.000000 coldfront-1.1.5/coldfront/__init__.py
+drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-07-13 00:45:36.899883 coldfront-1.1.5/coldfront/config/
+-rw-r--r--   0 aeb       (1000) aeb       (1000)        0 2021-02-25 21:11:22.000000 coldfront-1.1.5/coldfront/config/__init__.py
+-rw-r--r--   0 aeb       (1000) aeb       (1000)     1268 2023-03-09 12:41:00.000000 coldfront-1.1.5/coldfront/config/auth.py
+-rw-r--r--   0 aeb       (1000) aeb       (1000)     5450 2022-07-07 16:08:59.000000 coldfront-1.1.5/coldfront/config/base.py
+-rw-r--r--   0 aeb       (1000) aeb       (1000)     4638 2022-07-07 13:52:57.000000 coldfront-1.1.5/coldfront/config/core.py
+-rw-r--r--   0 aeb       (1000) aeb       (1000)     1515 2022-02-07 13:09:25.000000 coldfront-1.1.5/coldfront/config/database.py
+-rw-r--r--   0 aeb       (1000) aeb       (1000)     1589 2022-09-23 21:50:06.000000 coldfront-1.1.5/coldfront/config/email.py
+-rw-r--r--   0 aeb       (1000) aeb       (1000)      475 2021-11-10 16:20:52.000000 coldfront-1.1.5/coldfront/config/env.py
+-rw-r--r--   0 aeb       (1000) aeb       (1000)      992 2021-03-02 21:10:03.000000 coldfront-1.1.5/coldfront/config/logging.py
+drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-07-13 00:45:36.899883 coldfront-1.1.5/coldfront/config/plugins/
+-rw-r--r--   0 aeb       (1000) aeb       (1000)        0 2021-03-02 21:10:03.000000 coldfront-1.1.5/coldfront/config/plugins/__init__.py
+-rw-r--r--   0 aeb       (1000) aeb       (1000)      414 2021-03-02 21:10:03.000000 coldfront-1.1.5/coldfront/config/plugins/freeipa.py
+-rw-r--r--   0 aeb       (1000) aeb       (1000)      332 2021-03-02 21:10:03.000000 coldfront-1.1.5/coldfront/config/plugins/iquota.py
+-rw-r--r--   0 aeb       (1000) aeb       (1000)     1748 2021-03-25 15:26:38.000000 coldfront-1.1.5/coldfront/config/plugins/ldap.py
+-rw-r--r--   0 aeb       (1000) aeb       (1000)      935 2022-01-12 23:53:55.000000 coldfront-1.1.5/coldfront/config/plugins/ldap_user_search.py
+-rw-r--r--   0 aeb       (1000) aeb       (1000)     1582 2021-03-02 21:10:03.000000 coldfront-1.1.5/coldfront/config/plugins/openid.py
+-rw-r--r--   0 aeb       (1000) aeb       (1000)      406 2022-04-27 00:11:56.000000 coldfront-1.1.5/coldfront/config/plugins/slurm.py
+-rw-r--r--   0 aeb       (1000) aeb       (1000)      420 2021-03-02 21:10:03.000000 coldfront-1.1.5/coldfront/config/plugins/system_monitor.py
+-rw-r--r--   0 aeb       (1000) aeb       (1000)      365 2021-03-02 21:10:03.000000 coldfront-1.1.5/coldfront/config/plugins/xdmod.py
+-rw-r--r--   0 aeb       (1000) aeb       (1000)     1532 2022-09-29 18:05:12.000000 coldfront-1.1.5/coldfront/config/settings.py
+-rw-r--r--   0 aeb       (1000) aeb       (1000)     1683 2022-09-29 18:05:12.000000 coldfront-1.1.5/coldfront/config/urls.py
+-rw-r--r--   0 aeb       (1000) aeb       (1000)      302 2021-02-25 21:11:22.000000 coldfront-1.1.5/coldfront/config/wsgi.py
+drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-07-13 00:45:36.899883 coldfront-1.1.5/coldfront/core/
+-rw-r--r--   0 aeb       (1000) aeb       (1000)        0 2021-02-25 21:11:22.000000 coldfront-1.1.5/coldfront/core/__init__.py
+drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-07-13 00:45:36.903883 coldfront-1.1.5/coldfront/core/allocation/
+-rw-r--r--   0 aeb       (1000) aeb       (1000)        0 2021-02-25 21:11:22.000000 coldfront-1.1.5/coldfront/core/allocation/__init__.py
+-rw-r--r--   0 aeb       (1000) aeb       (1000)    12577 2021-12-23 13:28:09.000000 coldfront-1.1.5/coldfront/core/allocation/admin.py
+-rw-r--r--   0 aeb       (1000) aeb       (1000)      110 2022-02-07 13:09:25.000000 coldfront-1.1.5/coldfront/core/allocation/apps.py
+-rw-r--r--   0 aeb       (1000) aeb       (1000)    11419 2023-03-09 12:41:00.000000 coldfront-1.1.5/coldfront/core/allocation/forms.py
+drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-07-13 00:45:36.903883 coldfront-1.1.5/coldfront/core/allocation/management/
+-rw-r--r--   0 aeb       (1000) aeb       (1000)        0 2021-03-03 01:27:01.000000 coldfront-1.1.5/coldfront/core/allocation/management/__init__.py
+drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-07-13 00:45:36.903883 coldfront-1.1.5/coldfront/core/allocation/management/commands/
+-rw-r--r--   0 aeb       (1000) aeb       (1000)        0 2021-03-03 01:27:01.000000 coldfront-1.1.5/coldfront/core/allocation/management/commands/__init__.py
+-rw-r--r--   0 aeb       (1000) aeb       (1000)     2972 2022-10-09 13:46:08.000000 coldfront-1.1.5/coldfront/core/allocation/management/commands/add_allocation_defaults.py
+-rw-r--r--   0 aeb       (1000) aeb       (1000)      448 2022-03-11 14:30:53.000000 coldfront-1.1.5/coldfront/core/allocation/management/commands/enable_change_requests_globally.py
+drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-07-13 00:45:36.903883 coldfront-1.1.5/coldfront/core/allocation/migrations/
+-rw-r--r--   0 aeb       (1000) aeb       (1000)    19472 2021-02-25 21:11:22.000000 coldfront-1.1.5/coldfront/core/allocation/migrations/0001_initial.py
+-rw-r--r--   0 aeb       (1000) aeb       (1000)      878 2021-02-25 21:11:22.000000 coldfront-1.1.5/coldfront/core/allocation/migrations/0002_auto_20190718_1451.py
+-rw-r--r--   0 aeb       (1000) aeb       (1000)      568 2021-02-25 21:11:22.000000 coldfront-1.1.5/coldfront/core/allocation/migrations/0003_auto_20191018_1049.py
+-rw-r--r--   0 aeb       (1000) aeb       (1000)     7952 2021-12-23 13:28:09.000000 coldfront-1.1.5/coldfront/core/allocation/migrations/0004_auto_20211102_1017.py
+-rw-r--r--   0 aeb       (1000) aeb       (1000)      554 2021-12-23 13:28:09.000000 coldfront-1.1.5/coldfront/core/allocation/migrations/0005_auto_20211117_1413.py
+-rw-r--r--   0 aeb       (1000) aeb       (1000)        0 2021-02-25 21:11:22.000000 coldfront-1.1.5/coldfront/core/allocation/migrations/__init__.py
+-rw-r--r--   0 aeb       (1000) aeb       (1000)    26897 2023-04-20 15:19:39.000000 coldfront-1.1.5/coldfront/core/allocation/models.py
+-rw-r--r--   0 aeb       (1000) aeb       (1000)      499 2022-08-05 14:28:00.000000 coldfront-1.1.5/coldfront/core/allocation/signals.py
+-rw-r--r--   0 aeb       (1000) aeb       (1000)    10122 2022-09-20 14:51:20.000000 coldfront-1.1.5/coldfront/core/allocation/tasks.py
+drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-07-13 00:45:36.887883 coldfront-1.1.5/coldfront/core/allocation/templates/
+drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-07-13 00:45:36.907883 coldfront-1.1.5/coldfront/core/allocation/templates/allocation/
+-rw-r--r--   0 aeb       (1000) aeb       (1000)     1021 2021-02-25 21:11:22.000000 coldfront-1.1.5/coldfront/core/allocation/templates/allocation/allocation_account_list.html
+-rw-r--r--   0 aeb       (1000) aeb       (1000)      554 2021-02-25 21:11:22.000000 coldfront-1.1.5/coldfront/core/allocation/templates/allocation/allocation_add_invoice_note.html
+-rw-r--r--   0 aeb       (1000) aeb       (1000)     2525 2023-02-09 20:15:46.000000 coldfront-1.1.5/coldfront/core/allocation/templates/allocation/allocation_add_users.html
+-rw-r--r--   0 aeb       (1000) aeb       (1000)      501 2021-02-25 21:11:22.000000 coldfront-1.1.5/coldfront/core/allocation/templates/allocation/allocation_allocationaccount_create.html
+-rw-r--r--   0 aeb       (1000) aeb       (1000)      657 2023-02-09 20:15:46.000000 coldfront-1.1.5/coldfront/core/allocation/templates/allocation/allocation_allocationattribute_create.html
+-rw-r--r--   0 aeb       (1000) aeb       (1000)     2280 2023-02-09 20:15:46.000000 coldfront-1.1.5/coldfront/core/allocation/templates/allocation/allocation_allocationattribute_delete.html
+-rw-r--r--   0 aeb       (1000) aeb       (1000)     5035 2023-02-09 20:15:46.000000 coldfront-1.1.5/coldfront/core/allocation/templates/allocation/allocation_change.html
+-rw-r--r--   0 aeb       (1000) aeb       (1000)     8588 2023-02-09 20:15:46.000000 coldfront-1.1.5/coldfront/core/allocation/templates/allocation/allocation_change_detail.html
+-rw-r--r--   0 aeb       (1000) aeb       (1000)     3247 2023-02-09 20:15:46.000000 coldfront-1.1.5/coldfront/core/allocation/templates/allocation/allocation_change_list.html
+-rw-r--r--   0 aeb       (1000) aeb       (1000)     6005 2023-02-09 20:15:46.000000 coldfront-1.1.5/coldfront/core/allocation/templates/allocation/allocation_create.html
+-rw-r--r--   0 aeb       (1000) aeb       (1000)     1828 2021-02-25 21:11:22.000000 coldfront-1.1.5/coldfront/core/allocation/templates/allocation/allocation_delete_invoice_note.html
+-rw-r--r--   0 aeb       (1000) aeb       (1000)    16062 2023-02-09 20:15:46.000000 coldfront-1.1.5/coldfront/core/allocation/templates/allocation/allocation_detail.html
+-rw-r--r--   0 aeb       (1000) aeb       (1000)     1990 2021-02-25 21:11:22.000000 coldfront-1.1.5/coldfront/core/allocation/templates/allocation/allocation_email_pending_request.html
+-rw-r--r--   0 aeb       (1000) aeb       (1000)     4540 2021-02-25 21:11:22.000000 coldfront-1.1.5/coldfront/core/allocation/templates/allocation/allocation_invoice_detail.html
+-rw-r--r--   0 aeb       (1000) aeb       (1000)     1029 2022-03-09 21:14:23.000000 coldfront-1.1.5/coldfront/core/allocation/templates/allocation/allocation_invoice_list.html
+-rw-r--r--   0 aeb       (1000) aeb       (1000)     6186 2023-02-09 20:15:46.000000 coldfront-1.1.5/coldfront/core/allocation/templates/allocation/allocation_list.html
+-rw-r--r--   0 aeb       (1000) aeb       (1000)      652 2022-01-11 16:10:19.000000 coldfront-1.1.5/coldfront/core/allocation/templates/allocation/allocation_note_create.html
+-rw-r--r--   0 aeb       (1000) aeb       (1000)     2543 2023-02-09 20:15:46.000000 coldfront-1.1.5/coldfront/core/allocation/templates/allocation/allocation_remove_users.html
+-rw-r--r--   0 aeb       (1000) aeb       (1000)     3521 2021-02-25 21:11:22.000000 coldfront-1.1.5/coldfront/core/allocation/templates/allocation/allocation_renew.html
+-rw-r--r--   0 aeb       (1000) aeb       (1000)     2997 2023-02-09 20:15:46.000000 coldfront-1.1.5/coldfront/core/allocation/templates/allocation/allocation_request_list.html
+-rw-r--r--   0 aeb       (1000) aeb       (1000)      572 2021-02-25 21:11:22.000000 coldfront-1.1.5/coldfront/core/allocation/templates/allocation/allocation_update_invoice_note.html
+-rw-r--r--   0 aeb       (1000) aeb       (1000)       60 2023-02-09 20:15:46.000000 coldfront-1.1.5/coldfront/core/allocation/tests.py
+-rw-r--r--   0 aeb       (1000) aeb       (1000)     2874 2023-02-09 20:15:46.000000 coldfront-1.1.5/coldfront/core/allocation/urls.py
+-rw-r--r--   0 aeb       (1000) aeb       (1000)     1622 2021-12-23 15:00:25.000000 coldfront-1.1.5/coldfront/core/allocation/utils.py
+-rw-r--r--   0 aeb       (1000) aeb       (1000)    80919 2023-03-09 12:41:00.000000 coldfront-1.1.5/coldfront/core/allocation/views.py
+-rw-r--r--   0 aeb       (1000) aeb       (1000)    20969 2022-01-07 20:54:01.000000 coldfront-1.1.5/coldfront/core/attribute_expansion.py
+drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-07-13 00:45:36.907883 coldfront-1.1.5/coldfront/core/field_of_science/
+-rw-r--r--   0 aeb       (1000) aeb       (1000)       81 2021-02-25 21:11:22.000000 coldfront-1.1.5/coldfront/core/field_of_science/__init__.py
+-rw-r--r--   0 aeb       (1000) aeb       (1000)      427 2021-02-25 21:11:22.000000 coldfront-1.1.5/coldfront/core/field_of_science/admin.py
+-rw-r--r--   0 aeb       (1000) aeb       (1000)      158 2021-02-25 21:11:22.000000 coldfront-1.1.5/coldfront/core/field_of_science/apps.py
+drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-07-13 00:45:36.907883 coldfront-1.1.5/coldfront/core/field_of_science/management/
+-rw-r--r--   0 aeb       (1000) aeb       (1000)        0 2021-02-25 21:11:22.000000 coldfront-1.1.5/coldfront/core/field_of_science/management/__init__.py
+drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-07-13 00:45:36.907883 coldfront-1.1.5/coldfront/core/field_of_science/management/commands/
+-rw-r--r--   0 aeb       (1000) aeb       (1000)        0 2021-02-25 21:11:22.000000 coldfront-1.1.5/coldfront/core/field_of_science/management/commands/__init__.py
+drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-07-13 00:45:36.907883 coldfront-1.1.5/coldfront/core/field_of_science/management/commands/data/
+-rw-r--r--   0 aeb       (1000) aeb       (1000)     7584 2021-02-25 21:11:22.000000 coldfront-1.1.5/coldfront/core/field_of_science/management/commands/data/field_of_science_data.csv
+-rw-r--r--   0 aeb       (1000) aeb       (1000)     1282 2021-02-25 21:11:22.000000 coldfront-1.1.5/coldfront/core/field_of_science/management/commands/import_field_of_science_data.py
+drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-07-13 00:45:36.907883 coldfront-1.1.5/coldfront/core/field_of_science/migrations/
+-rw-r--r--   0 aeb       (1000) aeb       (1000)     1426 2021-02-25 21:11:22.000000 coldfront-1.1.5/coldfront/core/field_of_science/migrations/0001_initial.py
+-rw-r--r--   0 aeb       (1000) aeb       (1000)      412 2023-04-20 15:19:19.000000 coldfront-1.1.5/coldfront/core/field_of_science/migrations/0002_alter_fieldofscience_description.py
+-rw-r--r--   0 aeb       (1000) aeb       (1000)        0 2021-02-25 21:11:22.000000 coldfront-1.1.5/coldfront/core/field_of_science/migrations/__init__.py
+-rw-r--r--   0 aeb       (1000) aeb       (1000)     1771 2023-04-20 15:19:39.000000 coldfront-1.1.5/coldfront/core/field_of_science/models.py
+-rw-r--r--   0 aeb       (1000) aeb       (1000)     4235 2021-11-10 16:20:52.000000 coldfront-1.1.5/coldfront/core/field_of_science/tests.py
+-rw-r--r--   0 aeb       (1000) aeb       (1000)       63 2021-02-25 21:11:22.000000 coldfront-1.1.5/coldfront/core/field_of_science/views.py
+drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-07-13 00:45:36.907883 coldfront-1.1.5/coldfront/core/grant/
+-rw-r--r--   0 aeb       (1000) aeb       (1000)        0 2021-02-25 21:11:22.000000 coldfront-1.1.5/coldfront/core/grant/__init__.py
+-rw-r--r--   0 aeb       (1000) aeb       (1000)     1455 2022-09-29 18:05:12.000000 coldfront-1.1.5/coldfront/core/grant/admin.py
+-rw-r--r--   0 aeb       (1000) aeb       (1000)      100 2022-02-07 13:09:25.000000 coldfront-1.1.5/coldfront/core/grant/apps.py
+-rw-r--r--   0 aeb       (1000) aeb       (1000)     2589 2022-09-29 18:05:12.000000 coldfront-1.1.5/coldfront/core/grant/forms.py
+drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-07-13 00:45:36.907883 coldfront-1.1.5/coldfront/core/grant/management/
+-rw-r--r--   0 aeb       (1000) aeb       (1000)        0 2021-03-03 01:27:01.000000 coldfront-1.1.5/coldfront/core/grant/management/__init__.py
+drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-07-13 00:45:36.907883 coldfront-1.1.5/coldfront/core/grant/management/commands/
+-rw-r--r--   0 aeb       (1000) aeb       (1000)        0 2021-03-03 01:27:01.000000 coldfront-1.1.5/coldfront/core/grant/management/commands/__init__.py
+-rw-r--r--   0 aeb       (1000) aeb       (1000)     1186 2021-02-25 21:11:22.000000 coldfront-1.1.5/coldfront/core/grant/management/commands/add_default_grant_options.py
+drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-07-13 00:45:36.911883 coldfront-1.1.5/coldfront/core/grant/migrations/
+-rw-r--r--   0 aeb       (1000) aeb       (1000)     7260 2021-02-25 21:11:22.000000 coldfront-1.1.5/coldfront/core/grant/migrations/0001_initial.py
+-rw-r--r--   0 aeb       (1000) aeb       (1000)      573 2023-04-20 15:19:19.000000 coldfront-1.1.5/coldfront/core/grant/migrations/0002_auto_20230406_1310.py
+-rw-r--r--   0 aeb       (1000) aeb       (1000)        0 2021-02-25 21:11:22.000000 coldfront-1.1.5/coldfront/core/grant/migrations/__init__.py
+-rw-r--r--   0 aeb       (1000) aeb       (1000)     4510 2023-04-20 15:19:39.000000 coldfront-1.1.5/coldfront/core/grant/models.py
+drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-07-13 00:45:36.891883 coldfront-1.1.5/coldfront/core/grant/templates/
+drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-07-13 00:45:36.911883 coldfront-1.1.5/coldfront/core/grant/templates/grant/
+-rw-r--r--   0 aeb       (1000) aeb       (1000)      499 2023-02-09 20:15:46.000000 coldfront-1.1.5/coldfront/core/grant/templates/grant/grant_create.html
+-rw-r--r--   0 aeb       (1000) aeb       (1000)     2281 2023-02-09 20:15:46.000000 coldfront-1.1.5/coldfront/core/grant/templates/grant/grant_delete_grants.html
+-rw-r--r--   0 aeb       (1000) aeb       (1000)     3647 2022-04-27 00:08:38.000000 coldfront-1.1.5/coldfront/core/grant/templates/grant/grant_report_list.html
+-rw-r--r--   0 aeb       (1000) aeb       (1000)      492 2022-09-20 14:51:20.000000 coldfront-1.1.5/coldfront/core/grant/templates/grant/grant_update_form.html
+-rw-r--r--   0 aeb       (1000) aeb       (1000)     9083 2023-02-09 20:15:46.000000 coldfront-1.1.5/coldfront/core/grant/tests.py
+-rw-r--r--   0 aeb       (1000) aeb       (1000)      599 2022-09-29 18:05:12.000000 coldfront-1.1.5/coldfront/core/grant/urls.py
+-rw-r--r--   0 aeb       (1000) aeb       (1000)    13714 2022-09-29 18:05:12.000000 coldfront-1.1.5/coldfront/core/grant/views.py
+drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-07-13 00:45:36.911883 coldfront-1.1.5/coldfront/core/portal/
+-rw-r--r--   0 aeb       (1000) aeb       (1000)        0 2021-02-25 21:11:22.000000 coldfront-1.1.5/coldfront/core/portal/__init__.py
+-rw-r--r--   0 aeb       (1000) aeb       (1000)      397 2021-02-25 21:11:22.000000 coldfront-1.1.5/coldfront/core/portal/admin.py
+-rw-r--r--   0 aeb       (1000) aeb       (1000)      102 2022-02-07 13:09:25.000000 coldfront-1.1.5/coldfront/core/portal/apps.py
+drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-07-13 00:45:36.911883 coldfront-1.1.5/coldfront/core/portal/migrations/
+-rw-r--r--   0 aeb       (1000) aeb       (1000)        0 2021-02-25 21:11:22.000000 coldfront-1.1.5/coldfront/core/portal/migrations/__init__.py
+-rw-r--r--   0 aeb       (1000) aeb       (1000)       57 2021-02-25 21:11:22.000000 coldfront-1.1.5/coldfront/core/portal/models.py
+drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-07-13 00:45:36.891883 coldfront-1.1.5/coldfront/core/portal/templates/
+drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-07-13 00:45:36.911883 coldfront-1.1.5/coldfront/core/portal/templates/portal/
+-rw-r--r--   0 aeb       (1000) aeb       (1000)      696 2021-02-25 21:11:22.000000 coldfront-1.1.5/coldfront/core/portal/templates/portal/allocation_by_fos.html
+-rw-r--r--   0 aeb       (1000) aeb       (1000)     1867 2021-02-25 21:11:22.000000 coldfront-1.1.5/coldfront/core/portal/templates/portal/allocation_summary.html
+-rw-r--r--   0 aeb       (1000) aeb       (1000)     4207 2021-02-25 21:11:22.000000 coldfront-1.1.5/coldfront/core/portal/templates/portal/authorized_home.html
+-rw-r--r--   0 aeb       (1000) aeb       (1000)     1415 2021-02-25 21:11:22.000000 coldfront-1.1.5/coldfront/core/portal/templates/portal/carousel.html
+-rw-r--r--   0 aeb       (1000) aeb       (1000)     5519 2022-02-07 13:09:25.000000 coldfront-1.1.5/coldfront/core/portal/templates/portal/center_summary.html
+-rw-r--r--   0 aeb       (1000) aeb       (1000)      259 2021-02-25 21:11:22.000000 coldfront-1.1.5/coldfront/core/portal/templates/portal/extra_app_templates.html
+-rw-r--r--   0 aeb       (1000) aeb       (1000)      891 2023-02-09 20:15:46.000000 coldfront-1.1.5/coldfront/core/portal/templates/portal/nonauthorized_home.html
+drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-07-13 00:45:36.911883 coldfront-1.1.5/coldfront/core/portal/templatetags/
+-rw-r--r--   0 aeb       (1000) aeb       (1000)        0 2021-03-03 01:27:01.000000 coldfront-1.1.5/coldfront/core/portal/templatetags/__init__.py
+-rw-r--r--   0 aeb       (1000) aeb       (1000)      247 2021-02-25 21:11:22.000000 coldfront-1.1.5/coldfront/core/portal/templatetags/portal_tags.py
+-rw-r--r--   0 aeb       (1000) aeb       (1000)       60 2023-02-09 20:15:46.000000 coldfront-1.1.5/coldfront/core/portal/tests.py
+-rw-r--r--   0 aeb       (1000) aeb       (1000)     3448 2021-02-25 21:11:22.000000 coldfront-1.1.5/coldfront/core/portal/utils.py
+-rw-r--r--   0 aeb       (1000) aeb       (1000)     6907 2021-03-02 21:10:03.000000 coldfront-1.1.5/coldfront/core/portal/views.py
+drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-07-13 00:45:36.915884 coldfront-1.1.5/coldfront/core/project/
+-rw-r--r--   0 aeb       (1000) aeb       (1000)       65 2021-02-25 21:11:22.000000 coldfront-1.1.5/coldfront/core/project/__init__.py
+-rw-r--r--   0 aeb       (1000) aeb       (1000)    10121 2022-11-23 21:22:01.000000 coldfront-1.1.5/coldfront/core/project/admin.py
+-rw-r--r--   0 aeb       (1000) aeb       (1000)      104 2021-02-25 21:11:22.000000 coldfront-1.1.5/coldfront/core/project/apps.py
+-rw-r--r--   0 aeb       (1000) aeb       (1000)     8727 2023-03-09 12:41:00.000000 coldfront-1.1.5/coldfront/core/project/forms.py
+drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-07-13 00:45:36.915884 coldfront-1.1.5/coldfront/core/project/management/
+-rw-r--r--   0 aeb       (1000) aeb       (1000)        0 2021-03-03 01:27:01.000000 coldfront-1.1.5/coldfront/core/project/management/__init__.py
+drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-07-13 00:45:36.915884 coldfront-1.1.5/coldfront/core/project/management/commands/
+-rw-r--r--   0 aeb       (1000) aeb       (1000)        0 2021-03-03 01:27:01.000000 coldfront-1.1.5/coldfront/core/project/management/commands/__init__.py
+-rw-r--r--   0 aeb       (1000) aeb       (1000)     1645 2022-11-23 21:22:01.000000 coldfront-1.1.5/coldfront/core/project/management/commands/add_default_project_choices.py
+drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-07-13 00:45:36.915884 coldfront-1.1.5/coldfront/core/project/migrations/
+-rw-r--r--   0 aeb       (1000) aeb       (1000)    15306 2021-02-25 21:11:22.000000 coldfront-1.1.5/coldfront/core/project/migrations/0001_initial.py
+-rw-r--r--   0 aeb       (1000) aeb       (1000)      392 2022-07-07 13:52:57.000000 coldfront-1.1.5/coldfront/core/project/migrations/0002_projectusermessage_is_private.py
+-rw-r--r--   0 aeb       (1000) aeb       (1000)     9244 2022-11-23 21:22:01.000000 coldfront-1.1.5/coldfront/core/project/migrations/0003_auto_20221013_1215.py
+-rw-r--r--   0 aeb       (1000) aeb       (1000)      771 2023-04-20 15:19:39.000000 coldfront-1.1.5/coldfront/core/project/migrations/0004_auto_20230406_1133.py
+-rw-r--r--   0 aeb       (1000) aeb       (1000)        0 2021-02-25 21:11:22.000000 coldfront-1.1.5/coldfront/core/project/migrations/__init__.py
+-rw-r--r--   0 aeb       (1000) aeb       (1000)    16628 2023-04-20 15:19:39.000000 coldfront-1.1.5/coldfront/core/project/models.py
+drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-07-13 00:45:36.891883 coldfront-1.1.5/coldfront/core/project/templates/
+drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-07-13 00:45:36.915884 coldfront-1.1.5/coldfront/core/project/templates/project/
+-rw-r--r--   0 aeb       (1000) aeb       (1000)     3403 2023-02-09 20:15:46.000000 coldfront-1.1.5/coldfront/core/project/templates/project/add_user_search_results.html
+-rw-r--r--   0 aeb       (1000) aeb       (1000)     3189 2021-02-25 21:11:22.000000 coldfront-1.1.5/coldfront/core/project/templates/project/project_add_users.html
+-rw-r--r--   0 aeb       (1000) aeb       (1000)     1358 2021-02-25 21:11:22.000000 coldfront-1.1.5/coldfront/core/project/templates/project/project_archive.html
+-rw-r--r--   0 aeb       (1000) aeb       (1000)     5320 2022-01-11 16:10:19.000000 coldfront-1.1.5/coldfront/core/project/templates/project/project_archived_list.html
+-rw-r--r--   0 aeb       (1000) aeb       (1000)      513 2022-11-23 21:22:01.000000 coldfront-1.1.5/coldfront/core/project/templates/project/project_attribute_create.html
+-rw-r--r--   0 aeb       (1000) aeb       (1000)     2286 2022-11-23 21:22:01.000000 coldfront-1.1.5/coldfront/core/project/templates/project/project_attribute_delete.html
+-rw-r--r--   0 aeb       (1000) aeb       (1000)     1444 2022-11-23 21:22:01.000000 coldfront-1.1.5/coldfront/core/project/templates/project/project_attribute_update.html
+-rw-r--r--   0 aeb       (1000) aeb       (1000)      488 2023-02-09 20:15:46.000000 coldfront-1.1.5/coldfront/core/project/templates/project/project_create_form.html
+-rw-r--r--   0 aeb       (1000) aeb       (1000)    26553 2023-02-09 20:15:46.000000 coldfront-1.1.5/coldfront/core/project/templates/project/project_detail.html
+-rw-r--r--   0 aeb       (1000) aeb       (1000)     5666 2023-02-09 20:15:46.000000 coldfront-1.1.5/coldfront/core/project/templates/project/project_list.html
+-rw-r--r--   0 aeb       (1000) aeb       (1000)      611 2022-07-07 13:52:57.000000 coldfront-1.1.5/coldfront/core/project/templates/project/project_note_create.html
+-rw-r--r--   0 aeb       (1000) aeb       (1000)     2536 2021-02-25 21:11:22.000000 coldfront-1.1.5/coldfront/core/project/templates/project/project_remove_users.html
+-rw-r--r--   0 aeb       (1000) aeb       (1000)     2453 2023-02-09 20:15:46.000000 coldfront-1.1.5/coldfront/core/project/templates/project/project_review.html
+-rw-r--r--   0 aeb       (1000) aeb       (1000)     1883 2023-02-09 20:15:46.000000 coldfront-1.1.5/coldfront/core/project/templates/project/project_review_email.html
+-rw-r--r--   0 aeb       (1000) aeb       (1000)     2158 2023-02-09 20:15:46.000000 coldfront-1.1.5/coldfront/core/project/templates/project/project_review_list.html
+-rw-r--r--   0 aeb       (1000) aeb       (1000)      498 2021-02-25 21:11:22.000000 coldfront-1.1.5/coldfront/core/project/templates/project/project_update_form.html
+-rw-r--r--   0 aeb       (1000) aeb       (1000)     2300 2021-02-25 21:11:22.000000 coldfront-1.1.5/coldfront/core/project/templates/project/project_user_detail.html
+-rw-r--r--   0 aeb       (1000) aeb       (1000)     4684 2023-02-09 20:15:46.000000 coldfront-1.1.5/coldfront/core/project/tests.py
+-rw-r--r--   0 aeb       (1000) aeb       (1000)     2434 2022-11-23 21:22:01.000000 coldfront-1.1.5/coldfront/core/project/urls.py
+-rw-r--r--   0 aeb       (1000) aeb       (1000)      770 2021-02-25 21:11:22.000000 coldfront-1.1.5/coldfront/core/project/utils.py
+-rw-r--r--   0 aeb       (1000) aeb       (1000)    57685 2022-11-23 21:22:01.000000 coldfront-1.1.5/coldfront/core/project/views.py
+drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-07-13 00:45:36.919884 coldfront-1.1.5/coldfront/core/publication/
+-rw-r--r--   0 aeb       (1000) aeb       (1000)        0 2021-02-25 21:11:22.000000 coldfront-1.1.5/coldfront/core/publication/__init__.py
+-rw-r--r--   0 aeb       (1000) aeb       (1000)      500 2021-02-25 21:11:22.000000 coldfront-1.1.5/coldfront/core/publication/admin.py
+-rw-r--r--   0 aeb       (1000) aeb       (1000)      112 2022-02-07 13:09:25.000000 coldfront-1.1.5/coldfront/core/publication/apps.py
+-rw-r--r--   0 aeb       (1000) aeb       (1000)     1799 2022-09-29 18:05:12.000000 coldfront-1.1.5/coldfront/core/publication/forms.py
+drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-07-13 00:45:36.919884 coldfront-1.1.5/coldfront/core/publication/management/
+-rw-r--r--   0 aeb       (1000) aeb       (1000)        0 2021-03-03 01:27:01.000000 coldfront-1.1.5/coldfront/core/publication/management/__init__.py
+drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-07-13 00:45:36.919884 coldfront-1.1.5/coldfront/core/publication/management/commands/
+-rw-r--r--   0 aeb       (1000) aeb       (1000)        0 2021-03-03 01:27:01.000000 coldfront-1.1.5/coldfront/core/publication/management/commands/__init__.py
+-rw-r--r--   0 aeb       (1000) aeb       (1000)      490 2022-09-29 18:05:12.000000 coldfront-1.1.5/coldfront/core/publication/management/commands/add_default_publication_sources.py
+drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-07-13 00:45:36.919884 coldfront-1.1.5/coldfront/core/publication/migrations/
+-rw-r--r--   0 aeb       (1000) aeb       (1000)     4520 2021-02-25 21:11:22.000000 coldfront-1.1.5/coldfront/core/publication/migrations/0001_initial.py
+-rw-r--r--   0 aeb       (1000) aeb       (1000)      650 2021-02-25 21:11:22.000000 coldfront-1.1.5/coldfront/core/publication/migrations/0002_auto_20191223_1115.py
+-rw-r--r--   0 aeb       (1000) aeb       (1000)      581 2021-02-25 21:11:22.000000 coldfront-1.1.5/coldfront/core/publication/migrations/0003_auto_20200104_1700.py
+-rw-r--r--   0 aeb       (1000) aeb       (1000)      562 2021-02-25 21:11:22.000000 coldfront-1.1.5/coldfront/core/publication/migrations/0004_add_manual_publication_source.py
+-rw-r--r--   0 aeb       (1000) aeb       (1000)        0 2021-02-25 21:11:22.000000 coldfront-1.1.5/coldfront/core/publication/migrations/__init__.py
+-rw-r--r--   0 aeb       (1000) aeb       (1000)     1976 2023-04-06 13:09:32.000000 coldfront-1.1.5/coldfront/core/publication/models.py
+drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-07-13 00:45:36.891883 coldfront-1.1.5/coldfront/core/publication/templates/
+drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-07-13 00:45:36.919884 coldfront-1.1.5/coldfront/core/publication/templates/publication/
+-rw-r--r--   0 aeb       (1000) aeb       (1000)    12288 2023-07-13 00:17:46.000000 coldfront-1.1.5/coldfront/core/publication/templates/publication/.publication_add_publication_search_result.html.swp
+-rw-r--r--   0 aeb       (1000) aeb       (1000)     1200 2023-02-09 20:15:46.000000 coldfront-1.1.5/coldfront/core/publication/templates/publication/publication_add_publication_manually.html
+-rw-r--r--   0 aeb       (1000) aeb       (1000)     2509 2023-02-09 20:15:46.000000 coldfront-1.1.5/coldfront/core/publication/templates/publication/publication_add_publication_search.html
+-rw-r--r--   0 aeb       (1000) aeb       (1000)     2486 2023-02-09 20:15:46.000000 coldfront-1.1.5/coldfront/core/publication/templates/publication/publication_add_publication_search_result.html
+-rw-r--r--   0 aeb       (1000) aeb       (1000)     2270 2023-02-09 20:15:46.000000 coldfront-1.1.5/coldfront/core/publication/templates/publication/publication_delete_publications.html
+-rw-r--r--   0 aeb       (1000) aeb       (1000)     3215 2021-02-25 21:11:22.000000 coldfront-1.1.5/coldfront/core/publication/templates/publication/publication_export_publications.html
+-rw-r--r--   0 aeb       (1000) aeb       (1000)    10164 2023-02-09 20:15:46.000000 coldfront-1.1.5/coldfront/core/publication/tests.py
+-rw-r--r--   0 aeb       (1000) aeb       (1000)      974 2022-09-29 18:05:12.000000 coldfront-1.1.5/coldfront/core/publication/urls.py
+-rw-r--r--   0 aeb       (1000) aeb       (1000)    19628 2023-07-13 00:24:16.000000 coldfront-1.1.5/coldfront/core/publication/views.py
+drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-07-13 00:45:36.919884 coldfront-1.1.5/coldfront/core/research_output/
+-rw-r--r--   0 aeb       (1000) aeb       (1000)        0 2021-02-25 21:11:22.000000 coldfront-1.1.5/coldfront/core/research_output/__init__.py
+-rw-r--r--   0 aeb       (1000) aeb       (1000)     1018 2021-02-25 21:11:22.000000 coldfront-1.1.5/coldfront/core/research_output/admin.py
+-rw-r--r--   0 aeb       (1000) aeb       (1000)      119 2022-02-07 13:09:25.000000 coldfront-1.1.5/coldfront/core/research_output/apps.py
+-rw-r--r--   0 aeb       (1000) aeb       (1000)      219 2021-02-25 21:11:22.000000 coldfront-1.1.5/coldfront/core/research_output/forms.py
+drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-07-13 00:45:36.919884 coldfront-1.1.5/coldfront/core/research_output/migrations/
+-rw-r--r--   0 aeb       (1000) aeb       (1000)     3220 2021-02-25 21:11:22.000000 coldfront-1.1.5/coldfront/core/research_output/migrations/0001_initial.py
+-rw-r--r--   0 aeb       (1000) aeb       (1000)        0 2021-02-25 21:11:22.000000 coldfront-1.1.5/coldfront/core/research_output/migrations/__init__.py
+-rw-r--r--   0 aeb       (1000) aeb       (1000)     2159 2023-04-06 13:09:32.000000 coldfront-1.1.5/coldfront/core/research_output/models.py
+drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-07-13 00:45:36.891883 coldfront-1.1.5/coldfront/core/research_output/templates/
+drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-07-13 00:45:36.923884 coldfront-1.1.5/coldfront/core/research_output/templates/research_output/
+-rw-r--r--   0 aeb       (1000) aeb       (1000)      407 2023-02-09 20:15:46.000000 coldfront-1.1.5/coldfront/core/research_output/templates/research_output/research_output_create.html
+-rw-r--r--   0 aeb       (1000) aeb       (1000)     2332 2023-02-09 20:15:46.000000 coldfront-1.1.5/coldfront/core/research_output/templates/research_output/research_output_delete_research_outputs.html
+-rw-r--r--   0 aeb       (1000) aeb       (1000)     4906 2023-02-09 20:15:46.000000 coldfront-1.1.5/coldfront/core/research_output/tests.py
+-rw-r--r--   0 aeb       (1000) aeb       (1000)      438 2021-02-25 21:11:22.000000 coldfront-1.1.5/coldfront/core/research_output/urls.py
+-rw-r--r--   0 aeb       (1000) aeb       (1000)     3615 2021-02-25 21:11:22.000000 coldfront-1.1.5/coldfront/core/research_output/views.py
+drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-07-13 00:45:36.923884 coldfront-1.1.5/coldfront/core/resource/
+-rw-r--r--   0 aeb       (1000) aeb       (1000)        0 2021-02-25 21:11:22.000000 coldfront-1.1.5/coldfront/core/resource/__init__.py
+-rw-r--r--   0 aeb       (1000) aeb       (1000)     3108 2022-04-27 00:08:38.000000 coldfront-1.1.5/coldfront/core/resource/admin.py
+-rw-r--r--   0 aeb       (1000) aeb       (1000)      106 2022-02-07 13:09:25.000000 coldfront-1.1.5/coldfront/core/resource/apps.py
+-rw-r--r--   0 aeb       (1000) aeb       (1000)     2052 2022-09-20 14:51:20.000000 coldfront-1.1.5/coldfront/core/resource/forms.py
+drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-07-13 00:45:36.923884 coldfront-1.1.5/coldfront/core/resource/management/
+-rw-r--r--   0 aeb       (1000) aeb       (1000)        0 2021-03-03 01:27:01.000000 coldfront-1.1.5/coldfront/core/resource/management/__init__.py
+drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-07-13 00:45:36.923884 coldfront-1.1.5/coldfront/core/resource/management/commands/
+-rw-r--r--   0 aeb       (1000) aeb       (1000)        0 2021-03-03 01:27:01.000000 coldfront-1.1.5/coldfront/core/resource/management/commands/__init__.py
+-rw-r--r--   0 aeb       (1000) aeb       (1000)     2147 2022-03-07 19:51:38.000000 coldfront-1.1.5/coldfront/core/resource/management/commands/add_resource_defaults.py
+drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-07-13 00:45:36.923884 coldfront-1.1.5/coldfront/core/resource/migrations/
+-rw-r--r--   0 aeb       (1000) aeb       (1000)    12612 2021-02-25 21:11:22.000000 coldfront-1.1.5/coldfront/core/resource/migrations/0001_initial.py
+-rw-r--r--   0 aeb       (1000) aeb       (1000)      533 2021-02-25 21:11:22.000000 coldfront-1.1.5/coldfront/core/resource/migrations/0002_auto_20191017_1141.py
+-rw-r--r--   0 aeb       (1000) aeb       (1000)        0 2021-02-25 21:11:22.000000 coldfront-1.1.5/coldfront/core/resource/migrations/__init__.py
+-rw-r--r--   0 aeb       (1000) aeb       (1000)    13750 2023-04-20 15:19:39.000000 coldfront-1.1.5/coldfront/core/resource/models.py
+drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-07-13 00:45:36.923884 coldfront-1.1.5/coldfront/core/resource/templates/
+-rw-r--r--   0 aeb       (1000) aeb       (1000)     5371 2022-03-07 19:51:38.000000 coldfront-1.1.5/coldfront/core/resource/templates/resource_detail.html
+-rw-r--r--   0 aeb       (1000) aeb       (1000)     5257 2022-09-20 14:51:20.000000 coldfront-1.1.5/coldfront/core/resource/templates/resource_list.html
+-rw-r--r--   0 aeb       (1000) aeb       (1000)      500 2022-03-07 19:51:38.000000 coldfront-1.1.5/coldfront/core/resource/templates/resource_resourceattribute_create.html
+-rw-r--r--   0 aeb       (1000) aeb       (1000)     2218 2022-03-07 19:51:38.000000 coldfront-1.1.5/coldfront/core/resource/templates/resource_resourceattribute_delete.html
+-rw-r--r--   0 aeb       (1000) aeb       (1000)       60 2023-02-09 20:15:46.000000 coldfront-1.1.5/coldfront/core/resource/tests.py
+-rw-r--r--   0 aeb       (1000) aeb       (1000)      574 2022-03-07 19:51:38.000000 coldfront-1.1.5/coldfront/core/resource/urls.py
+-rw-r--r--   0 aeb       (1000) aeb       (1000)    12279 2022-09-20 14:51:20.000000 coldfront-1.1.5/coldfront/core/resource/views.py
+drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-07-13 00:45:36.923884 coldfront-1.1.5/coldfront/core/user/
+-rw-r--r--   0 aeb       (1000) aeb       (1000)       59 2021-02-25 21:11:22.000000 coldfront-1.1.5/coldfront/core/user/__init__.py
+-rw-r--r--   0 aeb       (1000) aeb       (1000)      529 2021-02-25 21:11:22.000000 coldfront-1.1.5/coldfront/core/user/admin.py
+-rw-r--r--   0 aeb       (1000) aeb       (1000)      163 2021-02-25 21:11:22.000000 coldfront-1.1.5/coldfront/core/user/apps.py
+-rw-r--r--   0 aeb       (1000) aeb       (1000)      918 2022-09-29 18:05:12.000000 coldfront-1.1.5/coldfront/core/user/forms.py
+drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-07-13 00:45:36.923884 coldfront-1.1.5/coldfront/core/user/migrations/
+-rw-r--r--   0 aeb       (1000) aeb       (1000)      749 2021-02-25 21:11:22.000000 coldfront-1.1.5/coldfront/core/user/migrations/0001_initial.py
+-rw-r--r--   0 aeb       (1000) aeb       (1000)        0 2021-02-25 21:11:22.000000 coldfront-1.1.5/coldfront/core/user/migrations/__init__.py
+-rw-r--r--   0 aeb       (1000) aeb       (1000)      526 2023-04-06 13:09:32.000000 coldfront-1.1.5/coldfront/core/user/models.py
+-rw-r--r--   0 aeb       (1000) aeb       (1000)      518 2021-02-25 21:11:22.000000 coldfront-1.1.5/coldfront/core/user/signals.py
+drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-07-13 00:45:36.891883 coldfront-1.1.5/coldfront/core/user/templates/
+drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-07-13 00:45:36.927884 coldfront-1.1.5/coldfront/core/user/templates/user/
+-rw-r--r--   0 aeb       (1000) aeb       (1000)     1316 2022-02-07 13:09:25.000000 coldfront-1.1.5/coldfront/core/user/templates/user/login.html
+-rw-r--r--   0 aeb       (1000) aeb       (1000)      303 2023-02-09 20:15:46.000000 coldfront-1.1.5/coldfront/core/user/templates/user/login_form.html
+-rw-r--r--   0 aeb       (1000) aeb       (1000)     2025 2022-03-09 21:14:23.000000 coldfront-1.1.5/coldfront/core/user/templates/user/user_list_allocations.html
+-rw-r--r--   0 aeb       (1000) aeb       (1000)     2549 2022-09-29 18:05:12.000000 coldfront-1.1.5/coldfront/core/user/templates/user/user_profile.html
+-rw-r--r--   0 aeb       (1000) aeb       (1000)     5500 2022-02-07 13:09:25.000000 coldfront-1.1.5/coldfront/core/user/templates/user/user_projects_managers.html
+-rw-r--r--   0 aeb       (1000) aeb       (1000)     2638 2021-02-25 21:11:22.000000 coldfront-1.1.5/coldfront/core/user/templates/user/user_search_home.html
+-rw-r--r--   0 aeb       (1000) aeb       (1000)     1257 2021-02-25 21:11:22.000000 coldfront-1.1.5/coldfront/core/user/templates/user/user_search_results.html
+-rw-r--r--   0 aeb       (1000) aeb       (1000)     1669 2023-02-09 20:15:46.000000 coldfront-1.1.5/coldfront/core/user/tests.py
+-rw-r--r--   0 aeb       (1000) aeb       (1000)     1356 2022-09-29 18:05:12.000000 coldfront-1.1.5/coldfront/core/user/urls.py
+-rw-r--r--   0 aeb       (1000) aeb       (1000)     4301 2021-07-20 15:45:35.000000 coldfront-1.1.5/coldfront/core/user/utils.py
+-rw-r--r--   0 aeb       (1000) aeb       (1000)     9968 2022-09-29 18:05:12.000000 coldfront-1.1.5/coldfront/core/user/views.py
+drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-07-13 00:45:36.927884 coldfront-1.1.5/coldfront/core/utils/
+-rw-r--r--   0 aeb       (1000) aeb       (1000)        0 2021-02-25 21:11:22.000000 coldfront-1.1.5/coldfront/core/utils/__init__.py
+-rw-r--r--   0 aeb       (1000) aeb       (1000)       63 2021-02-25 21:11:22.000000 coldfront-1.1.5/coldfront/core/utils/admin.py
+-rw-r--r--   0 aeb       (1000) aeb       (1000)      137 2022-02-07 13:09:25.000000 coldfront-1.1.5/coldfront/core/utils/apps.py
+-rw-r--r--   0 aeb       (1000) aeb       (1000)     1272 2021-02-25 21:11:22.000000 coldfront-1.1.5/coldfront/core/utils/common.py
+drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-07-13 00:45:36.927884 coldfront-1.1.5/coldfront/core/utils/fixtures/
+-rw-r--r--   0 aeb       (1000) aeb       (1000)        0 2021-02-25 21:11:22.000000 coldfront-1.1.5/coldfront/core/utils/fixtures/__init__.py
+-rw-r--r--   0 aeb       (1000) aeb       (1000)     4710 2022-09-23 21:50:06.000000 coldfront-1.1.5/coldfront/core/utils/mail.py
+drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-07-13 00:45:36.927884 coldfront-1.1.5/coldfront/core/utils/management/
+-rw-r--r--   0 aeb       (1000) aeb       (1000)        0 2021-03-03 01:27:01.000000 coldfront-1.1.5/coldfront/core/utils/management/__init__.py
+drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-07-13 00:45:36.927884 coldfront-1.1.5/coldfront/core/utils/management/commands/
+-rw-r--r--   0 aeb       (1000) aeb       (1000)        0 2021-03-03 01:27:01.000000 coldfront-1.1.5/coldfront/core/utils/management/commands/__init__.py
+-rw-r--r--   0 aeb       (1000) aeb       (1000)      763 2021-03-02 21:10:03.000000 coldfront-1.1.5/coldfront/core/utils/management/commands/add_scheduled_tasks.py
+-rw-r--r--   0 aeb       (1000) aeb       (1000)     1419 2022-12-06 13:04:35.000000 coldfront-1.1.5/coldfront/core/utils/management/commands/initial_setup.py
+-rw-r--r--   0 aeb       (1000) aeb       (1000)    28403 2023-02-09 20:03:17.000000 coldfront-1.1.5/coldfront/core/utils/management/commands/load_test_data.py
+-rw-r--r--   0 aeb       (1000) aeb       (1000)     1236 2021-02-25 21:11:22.000000 coldfront-1.1.5/coldfront/core/utils/management/commands/show_users_in_project_but_not_in_allocation.py
+drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-07-13 00:45:36.927884 coldfront-1.1.5/coldfront/core/utils/migrations/
+-rw-r--r--   0 aeb       (1000) aeb       (1000)        0 2021-02-25 21:11:22.000000 coldfront-1.1.5/coldfront/core/utils/migrations/__init__.py
+drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-07-13 00:45:36.927884 coldfront-1.1.5/coldfront/core/utils/mixins/
+-rw-r--r--   0 aeb       (1000) aeb       (1000)        0 2021-02-26 20:30:52.000000 coldfront-1.1.5/coldfront/core/utils/mixins/__init__.py
+-rw-r--r--   0 aeb       (1000) aeb       (1000)     2548 2021-02-25 21:11:22.000000 coldfront-1.1.5/coldfront/core/utils/mixins/views.py
+-rw-r--r--   0 aeb       (1000) aeb       (1000)       57 2021-02-25 21:11:22.000000 coldfront-1.1.5/coldfront/core/utils/models.py
+drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-07-13 00:45:36.927884 coldfront-1.1.5/coldfront/core/utils/templatetags/
+-rw-r--r--   0 aeb       (1000) aeb       (1000)        0 2021-03-03 01:27:01.000000 coldfront-1.1.5/coldfront/core/utils/templatetags/__init__.py
+-rw-r--r--   0 aeb       (1000) aeb       (1000)     1900 2021-02-25 21:11:22.000000 coldfront-1.1.5/coldfront/core/utils/templatetags/common_tags.py
+-rw-r--r--   0 aeb       (1000) aeb       (1000)       60 2023-02-09 20:15:46.000000 coldfront-1.1.5/coldfront/core/utils/tests.py
+-rw-r--r--   0 aeb       (1000) aeb       (1000)     1360 2022-11-23 21:22:01.000000 coldfront-1.1.5/coldfront/core/utils/validate.py
+-rw-r--r--   0 aeb       (1000) aeb       (1000)       63 2021-02-25 21:11:22.000000 coldfront-1.1.5/coldfront/core/utils/views.py
+drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-07-13 00:45:36.927884 coldfront-1.1.5/coldfront/plugins/
+-rw-r--r--   0 aeb       (1000) aeb       (1000)        0 2021-02-25 21:11:22.000000 coldfront-1.1.5/coldfront/plugins/__init__.py
+drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-07-13 00:45:36.931884 coldfront-1.1.5/coldfront/plugins/freeipa/
+-rw-r--r--   0 aeb       (1000) aeb       (1000)       64 2021-02-25 21:11:22.000000 coldfront-1.1.5/coldfront/plugins/freeipa/__init__.py
+-rw-r--r--   0 aeb       (1000) aeb       (1000)      354 2021-02-25 21:11:22.000000 coldfront-1.1.5/coldfront/plugins/freeipa/apps.py
+drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-07-13 00:45:36.931884 coldfront-1.1.5/coldfront/plugins/freeipa/management/
+-rw-r--r--   0 aeb       (1000) aeb       (1000)        0 2021-02-25 21:11:22.000000 coldfront-1.1.5/coldfront/plugins/freeipa/management/__init__.py
+drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-07-13 00:45:36.931884 coldfront-1.1.5/coldfront/plugins/freeipa/management/commands/
+-rw-r--r--   0 aeb       (1000) aeb       (1000)        0 2021-02-25 21:11:22.000000 coldfront-1.1.5/coldfront/plugins/freeipa/management/commands/__init__.py
+-rw-r--r--   0 aeb       (1000) aeb       (1000)    10200 2022-08-05 14:28:00.000000 coldfront-1.1.5/coldfront/plugins/freeipa/management/commands/freeipa_check.py
+-rw-r--r--   0 aeb       (1000) aeb       (1000)     4189 2021-02-25 21:11:22.000000 coldfront-1.1.5/coldfront/plugins/freeipa/management/commands/freeipa_expire_users.py
+-rw-r--r--   0 aeb       (1000) aeb       (1000)     3353 2021-02-25 21:11:22.000000 coldfront-1.1.5/coldfront/plugins/freeipa/search.py
+-rw-r--r--   0 aeb       (1000) aeb       (1000)     1338 2023-02-09 20:05:18.000000 coldfront-1.1.5/coldfront/plugins/freeipa/signals.py
+-rw-r--r--   0 aeb       (1000) aeb       (1000)     4782 2021-02-25 21:11:22.000000 coldfront-1.1.5/coldfront/plugins/freeipa/tasks.py
+-rw-r--r--   0 aeb       (1000) aeb       (1000)     1408 2021-02-25 21:11:22.000000 coldfront-1.1.5/coldfront/plugins/freeipa/utils.py
+drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-07-13 00:45:36.931884 coldfront-1.1.5/coldfront/plugins/iquota/
+-rw-r--r--   0 aeb       (1000) aeb       (1000)        0 2021-02-25 21:11:22.000000 coldfront-1.1.5/coldfront/plugins/iquota/__init__.py
+-rw-r--r--   0 aeb       (1000) aeb       (1000)       63 2021-02-25 21:11:22.000000 coldfront-1.1.5/coldfront/plugins/iquota/admin.py
+-rw-r--r--   0 aeb       (1000) aeb       (1000)      105 2022-02-07 13:09:25.000000 coldfront-1.1.5/coldfront/plugins/iquota/apps.py
+-rw-r--r--   0 aeb       (1000) aeb       (1000)      276 2021-02-25 21:11:22.000000 coldfront-1.1.5/coldfront/plugins/iquota/exceptions.py
+drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-07-13 00:45:36.931884 coldfront-1.1.5/coldfront/plugins/iquota/migrations/
+-rw-r--r--   0 aeb       (1000) aeb       (1000)        0 2021-02-25 21:11:22.000000 coldfront-1.1.5/coldfront/plugins/iquota/migrations/__init__.py
+drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-07-13 00:45:36.895883 coldfront-1.1.5/coldfront/plugins/iquota/templates/
+drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-07-13 00:45:36.931884 coldfront-1.1.5/coldfront/plugins/iquota/templates/iquota/
+-rw-r--r--   0 aeb       (1000) aeb       (1000)     1711 2021-02-25 21:11:22.000000 coldfront-1.1.5/coldfront/plugins/iquota/templates/iquota/iquota.html
+-rw-r--r--   0 aeb       (1000) aeb       (1000)      955 2021-02-25 21:11:22.000000 coldfront-1.1.5/coldfront/plugins/iquota/templates/iquota/iquota_div.html
+-rw-r--r--   0 aeb       (1000) aeb       (1000)      183 2021-02-25 21:11:22.000000 coldfront-1.1.5/coldfront/plugins/iquota/urls.py
+-rw-r--r--   0 aeb       (1000) aeb       (1000)     3548 2021-03-25 01:57:34.000000 coldfront-1.1.5/coldfront/plugins/iquota/utils.py
+-rw-r--r--   0 aeb       (1000) aeb       (1000)      639 2021-02-25 21:11:22.000000 coldfront-1.1.5/coldfront/plugins/iquota/views.py
+drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-07-13 00:45:36.931884 coldfront-1.1.5/coldfront/plugins/ldap_user_search/
+-rw-r--r--   0 aeb       (1000) aeb       (1000)        0 2021-02-25 21:11:22.000000 coldfront-1.1.5/coldfront/plugins/ldap_user_search/__init__.py
+-rw-r--r--   0 aeb       (1000) aeb       (1000)       63 2021-02-25 21:11:22.000000 coldfront-1.1.5/coldfront/plugins/ldap_user_search/admin.py
+-rw-r--r--   0 aeb       (1000) aeb       (1000)      123 2022-02-07 13:09:25.000000 coldfront-1.1.5/coldfront/plugins/ldap_user_search/apps.py
+drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-07-13 00:45:36.931884 coldfront-1.1.5/coldfront/plugins/ldap_user_search/migrations/
+-rw-r--r--   0 aeb       (1000) aeb       (1000)        0 2021-02-25 21:11:22.000000 coldfront-1.1.5/coldfront/plugins/ldap_user_search/migrations/__init__.py
+-rw-r--r--   0 aeb       (1000) aeb       (1000)       57 2021-02-25 21:11:22.000000 coldfront-1.1.5/coldfront/plugins/ldap_user_search/models.py
+-rw-r--r--   0 aeb       (1000) aeb       (1000)       60 2023-02-09 20:15:46.000000 coldfront-1.1.5/coldfront/plugins/ldap_user_search/tests.py
+-rw-r--r--   0 aeb       (1000) aeb       (1000)     2824 2022-01-12 23:53:55.000000 coldfront-1.1.5/coldfront/plugins/ldap_user_search/utils.py
+-rw-r--r--   0 aeb       (1000) aeb       (1000)       63 2021-02-25 21:11:22.000000 coldfront-1.1.5/coldfront/plugins/ldap_user_search/views.py
+drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-07-13 00:45:36.931884 coldfront-1.1.5/coldfront/plugins/mokey_oidc/
+-rw-r--r--   0 aeb       (1000) aeb       (1000)        0 2021-02-25 21:11:22.000000 coldfront-1.1.5/coldfront/plugins/mokey_oidc/__init__.py
+-rw-r--r--   0 aeb       (1000) aeb       (1000)      112 2022-02-07 13:09:25.000000 coldfront-1.1.5/coldfront/plugins/mokey_oidc/apps.py
+-rw-r--r--   0 aeb       (1000) aeb       (1000)     3222 2021-11-10 16:20:52.000000 coldfront-1.1.5/coldfront/plugins/mokey_oidc/auth.py
+drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-07-13 00:45:36.931884 coldfront-1.1.5/coldfront/plugins/mokey_oidc/migrations/
+-rw-r--r--   0 aeb       (1000) aeb       (1000)        0 2021-02-25 21:11:22.000000 coldfront-1.1.5/coldfront/plugins/mokey_oidc/migrations/__init__.py
+drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-07-13 00:45:36.935884 coldfront-1.1.5/coldfront/plugins/slurm/
+-rw-r--r--   0 aeb       (1000) aeb       (1000)       64 2021-02-25 21:11:22.000000 coldfront-1.1.5/coldfront/plugins/slurm/__init__.py
+-rw-r--r--   0 aeb       (1000) aeb       (1000)      103 2021-02-25 21:11:22.000000 coldfront-1.1.5/coldfront/plugins/slurm/apps.py
+-rw-r--r--   0 aeb       (1000) aeb       (1000)     9271 2022-09-20 14:51:20.000000 coldfront-1.1.5/coldfront/plugins/slurm/associations.py
+drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-07-13 00:45:36.935884 coldfront-1.1.5/coldfront/plugins/slurm/management/
+-rw-r--r--   0 aeb       (1000) aeb       (1000)        0 2021-02-25 21:11:22.000000 coldfront-1.1.5/coldfront/plugins/slurm/management/__init__.py
+drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-07-13 00:45:36.935884 coldfront-1.1.5/coldfront/plugins/slurm/management/commands/
+-rw-r--r--   0 aeb       (1000) aeb       (1000)        0 2021-02-25 21:11:22.000000 coldfront-1.1.5/coldfront/plugins/slurm/management/commands/__init__.py
+-rw-r--r--   0 aeb       (1000) aeb       (1000)    10552 2021-02-25 21:11:22.000000 coldfront-1.1.5/coldfront/plugins/slurm/management/commands/slurm_check.py
+-rw-r--r--   0 aeb       (1000) aeb       (1000)     1872 2021-03-25 01:57:34.000000 coldfront-1.1.5/coldfront/plugins/slurm/management/commands/slurm_dump.py
+-rw-r--r--   0 aeb       (1000) aeb       (1000)     4540 2021-02-25 21:11:22.000000 coldfront-1.1.5/coldfront/plugins/slurm/utils.py
+drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-07-13 00:45:36.935884 coldfront-1.1.5/coldfront/plugins/system_monitor/
+-rw-r--r--   0 aeb       (1000) aeb       (1000)        0 2021-02-25 21:11:22.000000 coldfront-1.1.5/coldfront/plugins/system_monitor/__init__.py
+drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-07-13 00:45:36.895883 coldfront-1.1.5/coldfront/plugins/system_monitor/templates/
+drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-07-13 00:45:36.935884 coldfront-1.1.5/coldfront/plugins/system_monitor/templates/system_monitor/
+-rw-r--r--   0 aeb       (1000) aeb       (1000)     2305 2022-02-07 13:09:25.000000 coldfront-1.1.5/coldfront/plugins/system_monitor/templates/system_monitor/system_monitor_div.html
+-rw-r--r--   0 aeb       (1000) aeb       (1000)     5627 2021-02-25 21:11:22.000000 coldfront-1.1.5/coldfront/plugins/system_monitor/utils.py
+drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-07-13 00:45:36.935884 coldfront-1.1.5/coldfront/plugins/xdmod/
+-rw-r--r--   0 aeb       (1000) aeb       (1000)       64 2021-02-25 21:11:22.000000 coldfront-1.1.5/coldfront/plugins/xdmod/__init__.py
+-rw-r--r--   0 aeb       (1000) aeb       (1000)      103 2021-02-25 21:11:22.000000 coldfront-1.1.5/coldfront/plugins/xdmod/apps.py
+drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-07-13 00:45:36.935884 coldfront-1.1.5/coldfront/plugins/xdmod/management/
+-rw-r--r--   0 aeb       (1000) aeb       (1000)        0 2021-02-25 21:11:22.000000 coldfront-1.1.5/coldfront/plugins/xdmod/management/__init__.py
+drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-07-13 00:45:36.935884 coldfront-1.1.5/coldfront/plugins/xdmod/management/commands/
+-rw-r--r--   0 aeb       (1000) aeb       (1000)        0 2021-02-25 21:11:22.000000 coldfront-1.1.5/coldfront/plugins/xdmod/management/commands/__init__.py
+-rw-r--r--   0 aeb       (1000) aeb       (1000)    18434 2022-10-09 13:46:08.000000 coldfront-1.1.5/coldfront/plugins/xdmod/management/commands/xdmod_usage.py
+-rw-r--r--   0 aeb       (1000) aeb       (1000)     6492 2022-10-09 13:46:08.000000 coldfront-1.1.5/coldfront/plugins/xdmod/utils.py
+drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-07-13 00:45:36.895883 coldfront-1.1.5/coldfront/static/
+drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-07-13 00:45:36.935884 coldfront-1.1.5/coldfront/static/bootstrap/
+-rw-r--r--   0 aeb       (1000) aeb       (1000)    83253 2022-07-07 16:08:59.000000 coldfront-1.1.5/coldfront/static/bootstrap/bootstrap.bundle.min.js
+-rw-r--r--   0 aeb       (1000) aeb       (1000)   311239 2022-07-07 16:08:59.000000 coldfront-1.1.5/coldfront/static/bootstrap/bootstrap.bundle.min.js.map
+-rw-r--r--   0 aeb       (1000) aeb       (1000)   162017 2022-07-07 16:08:59.000000 coldfront-1.1.5/coldfront/static/bootstrap/bootstrap.min.css
+-rw-r--r--   0 aeb       (1000) aeb       (1000)   653535 2022-07-07 16:08:59.000000 coldfront-1.1.5/coldfront/static/bootstrap/bootstrap.min.css.map
+drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-07-13 00:45:36.935884 coldfront-1.1.5/coldfront/static/c3js/
+-rwxr-xr-x   0 aeb       (1000) aeb       (1000)     2386 2021-02-25 21:11:22.000000 coldfront-1.1.5/coldfront/static/c3js/c3.min.css
+-rwxr-xr-x   0 aeb       (1000) aeb       (1000)   191799 2022-07-07 14:47:15.000000 coldfront-1.1.5/coldfront/static/c3js/c3.min.js
+drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-07-13 00:45:36.895883 coldfront-1.1.5/coldfront/static/coldfront/
+drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-07-13 00:45:36.895883 coldfront-1.1.5/coldfront/static/coldfront/plugins/
+drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-07-13 00:45:36.895883 coldfront-1.1.5/coldfront/static/coldfront/plugins/system_monitor/
+drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-07-13 00:45:36.935884 coldfront-1.1.5/coldfront/static/coldfront/plugins/system_monitor/images/
+-rw-r--r--   0 aeb       (1000) aeb       (1000)    42418 2021-02-25 21:11:22.000000 coldfront-1.1.5/coldfront/static/coldfront/plugins/system_monitor/images/xdmod.png
+drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-07-13 00:45:36.939884 coldfront-1.1.5/coldfront/static/common/
+drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-07-13 00:45:36.939884 coldfront-1.1.5/coldfront/static/common/css/
+-rw-r--r--   0 aeb       (1000) aeb       (1000)     3925 2022-09-29 18:05:12.000000 coldfront-1.1.5/coldfront/static/common/css/common.css
+drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-07-13 00:45:36.939884 coldfront-1.1.5/coldfront/static/common/images/
+-rw-r--r--   0 aeb       (1000) aeb       (1000)    12165 2022-07-07 22:12:57.000000 coldfront-1.1.5/coldfront/static/common/images/android-chrome-192x192.png
+-rw-r--r--   0 aeb       (1000) aeb       (1000)    30499 2022-07-07 22:12:57.000000 coldfront-1.1.5/coldfront/static/common/images/android-chrome-512x512.png
+-rw-r--r--   0 aeb       (1000) aeb       (1000)    10941 2022-07-07 22:12:57.000000 coldfront-1.1.5/coldfront/static/common/images/apple-touch-icon.png
+-rw-r--r--   0 aeb       (1000) aeb       (1000)      626 2022-07-07 22:12:57.000000 coldfront-1.1.5/coldfront/static/common/images/favicon-16x16.png
+-rw-r--r--   0 aeb       (1000) aeb       (1000)     1431 2022-07-07 22:12:57.000000 coldfront-1.1.5/coldfront/static/common/images/favicon-32x32.png
+-rw-r--r--   0 aeb       (1000) aeb       (1000)    15406 2022-07-07 22:12:57.000000 coldfront-1.1.5/coldfront/static/common/images/favicon.ico
+-rw-r--r--   0 aeb       (1000) aeb       (1000)   121290 2022-07-07 22:12:57.000000 coldfront-1.1.5/coldfront/static/common/images/logo.png
+-rw-r--r--   0 aeb       (1000) aeb       (1000)      306 2022-07-07 22:12:57.000000 coldfront-1.1.5/coldfront/static/common/site.webmanifest
+drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-07-13 00:45:36.895883 coldfront-1.1.5/coldfront/static/core/
+drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-07-13 00:45:36.895883 coldfront-1.1.5/coldfront/static/core/portal/
+drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-07-13 00:45:36.943884 coldfront-1.1.5/coldfront/static/core/portal/imgs/
+-rw-r--r--   0 aeb       (1000) aeb       (1000)   418141 2021-02-25 21:11:22.000000 coldfront-1.1.5/coldfront/static/core/portal/imgs/airport-business-cabinets-236093.jpg
+-rw-r--r--   0 aeb       (1000) aeb       (1000)  1148253 2021-02-25 21:11:22.000000 coldfront-1.1.5/coldfront/static/core/portal/imgs/analogue-blur-business-159282.jpg
+-rw-r--r--   0 aeb       (1000) aeb       (1000)   954249 2021-02-25 21:11:22.000000 coldfront-1.1.5/coldfront/static/core/portal/imgs/computer-electronics-equipment-325223.jpg
+-rw-r--r--   0 aeb       (1000) aeb       (1000)     5118 2021-02-25 21:11:22.000000 coldfront-1.1.5/coldfront/static/core/portal/imgs/ondemand.png
+drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-07-13 00:45:36.943884 coldfront-1.1.5/coldfront/static/d3/
+-rw-r--r--   0 aeb       (1000) aeb       (1000)   237682 2022-07-07 14:47:15.000000 coldfront-1.1.5/coldfront/static/d3/d3.v5.min.js
+drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-07-13 00:45:36.943884 coldfront-1.1.5/coldfront/static/datatable/
+-rw-r--r--   0 aeb       (1000) aeb       (1000)     5222 2022-07-07 16:08:59.000000 coldfront-1.1.5/coldfront/static/datatable/dataTables.bootstrap4.min.css
+-rw-r--r--   0 aeb       (1000) aeb       (1000)     2085 2022-07-07 16:08:59.000000 coldfront-1.1.5/coldfront/static/datatable/dataTables.bootstrap4.min.js
+-rw-r--r--   0 aeb       (1000) aeb       (1000)    82411 2022-07-07 16:08:59.000000 coldfront-1.1.5/coldfront/static/datatable/jquery.dataTables.min.js
+drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-07-13 00:45:36.943884 coldfront-1.1.5/coldfront/static/flatpickr/
+-rw-r--r--   0 aeb       (1000) aeb       (1000)    50679 2022-09-20 14:51:20.000000 coldfront-1.1.5/coldfront/static/flatpickr/flatpickr.js
+-rw-r--r--   0 aeb       (1000) aeb       (1000)    16166 2022-09-20 14:51:20.000000 coldfront-1.1.5/coldfront/static/flatpickr/flatpickr.min.css
+drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-07-13 00:45:36.943884 coldfront-1.1.5/coldfront/static/jquery/
+-rw-r--r--   0 aeb       (1000) aeb       (1000)    89501 2022-07-07 16:08:59.000000 coldfront-1.1.5/coldfront/static/jquery/jquery-3.6.0.min.js
+drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-07-13 00:45:36.943884 coldfront-1.1.5/coldfront/static/select2/
+-rw-r--r--   0 aeb       (1000) aeb       (1000)    15275 2022-07-07 16:08:59.000000 coldfront-1.1.5/coldfront/static/select2/select2.min.css
+-rw-r--r--   0 aeb       (1000) aeb       (1000)    67751 2022-07-07 16:08:59.000000 coldfront-1.1.5/coldfront/static/select2/select2.min.js
+drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-07-13 00:45:36.943884 coldfront-1.1.5/coldfront/templates/
+-rw-r--r--   0 aeb       (1000) aeb       (1000)      396 2023-02-09 20:05:18.000000 coldfront-1.1.5/coldfront/templates/400.html
+-rw-r--r--   0 aeb       (1000) aeb       (1000)      418 2021-03-25 01:57:34.000000 coldfront-1.1.5/coldfront/templates/403.html
+-rw-r--r--   0 aeb       (1000) aeb       (1000)      425 2021-02-25 21:11:22.000000 coldfront-1.1.5/coldfront/templates/404.html
+-rw-r--r--   0 aeb       (1000) aeb       (1000)      456 2021-02-25 21:11:22.000000 coldfront-1.1.5/coldfront/templates/500.html
+drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-07-13 00:45:36.947884 coldfront-1.1.5/coldfront/templates/common/
+-rw-r--r--   0 aeb       (1000) aeb       (1000)     2470 2023-02-09 20:15:46.000000 coldfront-1.1.5/coldfront/templates/common/authorized_navbar.html
+-rw-r--r--   0 aeb       (1000) aeb       (1000)     2530 2022-09-20 14:51:20.000000 coldfront-1.1.5/coldfront/templates/common/base.html
+-rw-r--r--   0 aeb       (1000) aeb       (1000)      357 2021-02-25 21:11:22.000000 coldfront-1.1.5/coldfront/templates/common/footer.html
+-rw-r--r--   0 aeb       (1000) aeb       (1000)      289 2021-02-25 21:11:22.000000 coldfront-1.1.5/coldfront/templates/common/messages.html
+-rw-r--r--   0 aeb       (1000) aeb       (1000)     1140 2023-02-09 20:15:46.000000 coldfront-1.1.5/coldfront/templates/common/navbar_admin.html
+-rw-r--r--   0 aeb       (1000) aeb       (1000)      444 2022-07-07 22:12:57.000000 coldfront-1.1.5/coldfront/templates/common/navbar_brand.html
+-rw-r--r--   0 aeb       (1000) aeb       (1000)      686 2022-03-07 19:51:38.000000 coldfront-1.1.5/coldfront/templates/common/navbar_director.html
+-rw-r--r--   0 aeb       (1000) aeb       (1000)      140 2022-07-07 13:52:57.000000 coldfront-1.1.5/coldfront/templates/common/navbar_help.html
+-rw-r--r--   0 aeb       (1000) aeb       (1000)      321 2021-02-25 21:11:22.000000 coldfront-1.1.5/coldfront/templates/common/navbar_invoice.html
+-rw-r--r--   0 aeb       (1000) aeb       (1000)      523 2021-02-25 21:11:22.000000 coldfront-1.1.5/coldfront/templates/common/navbar_login.html
+-rw-r--r--   0 aeb       (1000) aeb       (1000)     1501 2022-03-07 19:51:38.000000 coldfront-1.1.5/coldfront/templates/common/navbar_nonadmin_staff.html
+-rw-r--r--   0 aeb       (1000) aeb       (1000)     1123 2022-07-07 13:52:57.000000 coldfront-1.1.5/coldfront/templates/common/nonauthorized_navbar.html
+drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-07-13 00:45:36.947884 coldfront-1.1.5/coldfront/templates/email/
+-rw-r--r--   0 aeb       (1000) aeb       (1000)      710 2022-09-20 14:51:20.000000 coldfront-1.1.5/coldfront/templates/email/admin_allocation_expired.txt
+-rw-r--r--   0 aeb       (1000) aeb       (1000)      432 2023-03-09 12:41:00.000000 coldfront-1.1.5/coldfront/templates/email/allocation_activated.txt
+-rw-r--r--   0 aeb       (1000) aeb       (1000)      454 2023-03-09 12:41:00.000000 coldfront-1.1.5/coldfront/templates/email/allocation_change_approved.txt
+-rw-r--r--   0 aeb       (1000) aeb       (1000)      470 2023-03-09 12:41:00.000000 coldfront-1.1.5/coldfront/templates/email/allocation_change_denied.txt
+-rw-r--r--   0 aeb       (1000) aeb       (1000)      403 2023-03-09 12:41:00.000000 coldfront-1.1.5/coldfront/templates/email/allocation_denied.txt
+-rw-r--r--   0 aeb       (1000) aeb       (1000)     1447 2022-09-20 14:51:20.000000 coldfront-1.1.5/coldfront/templates/email/allocation_expired.txt
+-rw-r--r--   0 aeb       (1000) aeb       (1000)     1430 2022-09-20 14:51:20.000000 coldfront-1.1.5/coldfront/templates/email/allocation_expiring.txt
+-rw-r--r--   0 aeb       (1000) aeb       (1000)       97 2021-02-25 21:11:22.000000 coldfront-1.1.5/coldfront/templates/email/allocation_renewed.txt
+-rw-r--r--   0 aeb       (1000) aeb       (1000)      396 2023-03-09 12:41:00.000000 coldfront-1.1.5/coldfront/templates/email/allocation_revoked.txt
+-rw-r--r--   0 aeb       (1000) aeb       (1000)      116 2022-02-07 13:09:25.000000 coldfront-1.1.5/coldfront/templates/email/new_allocation_change_request.txt
+-rw-r--r--   0 aeb       (1000) aeb       (1000)      103 2021-02-25 21:11:22.000000 coldfront-1.1.5/coldfront/templates/email/new_allocation_request.txt
+-rw-r--r--   0 aeb       (1000) aeb       (1000)       94 2021-02-25 21:11:22.000000 coldfront-1.1.5/coldfront/templates/email/new_project_review.txt
+-rw-r--r--   0 aeb       (1000) aeb       (1000)      155 2021-02-25 21:11:22.000000 coldfront-1.1.5/coldfront/templates/email/upgrade_account_request.txt
+-rw-r--r--   0 aeb       (1000) aeb       (1000)      238 2021-02-25 21:11:22.000000 coldfront-1.1.5/coldfront/templates/robots.txt
+drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-07-13 00:45:36.947884 coldfront-1.1.5/coldfront/templates/su/
+-rw-r--r--   0 aeb       (1000) aeb       (1000)      497 2021-02-25 21:11:22.000000 coldfront-1.1.5/coldfront/templates/su/is_su.html
+drwxr-xr-x   0 aeb       (1000) aeb       (1000)        0 2023-07-13 00:45:36.899883 coldfront-1.1.5/coldfront.egg-info/
+-rw-r--r--   0 aeb       (1000) aeb       (1000)     3428 2023-07-13 00:45:36.000000 coldfront-1.1.5/coldfront.egg-info/PKG-INFO
+-rw-r--r--   0 aeb       (1000) aeb       (1000)    17333 2023-07-13 00:45:36.000000 coldfront-1.1.5/coldfront.egg-info/SOURCES.txt
+-rw-r--r--   0 aeb       (1000) aeb       (1000)        1 2023-07-13 00:45:36.000000 coldfront-1.1.5/coldfront.egg-info/dependency_links.txt
+-rw-r--r--   0 aeb       (1000) aeb       (1000)       47 2023-07-13 00:45:36.000000 coldfront-1.1.5/coldfront.egg-info/entry_points.txt
+-rw-r--r--   0 aeb       (1000) aeb       (1000)      643 2023-07-13 00:45:36.000000 coldfront-1.1.5/coldfront.egg-info/requires.txt
+-rw-r--r--   0 aeb       (1000) aeb       (1000)       10 2023-07-13 00:45:36.000000 coldfront-1.1.5/coldfront.egg-info/top_level.txt
+-rw-r--r--   0 aeb       (1000) aeb       (1000)       38 2023-07-13 00:45:36.947884 coldfront-1.1.5/setup.cfg
+-rw-r--r--   0 aeb       (1000) aeb       (1000)     2371 2023-07-13 00:41:09.000000 coldfront-1.1.5/setup.py
```

### Comparing `coldfront-1.1.4/LICENSE` & `coldfront-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/MANIFEST.in` & `coldfront-1.1.5/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/PKG-INFO` & `coldfront-1.1.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coldfront
-Version: 1.1.4
+Version: 1.1.5
 Summary: HPC Resource Allocation System 
 Home-page: http://coldfront.io
 Author: Andrew E. Bruno, Dori Sajdak, Mohammad Zia
 License: GNU General Public License v3 (GPLv3)
 Project-URL: Bug Tracker, https://github.com/ubccr/coldfront/issues
 Project-URL: Documentation, https://coldfront.readthedocs.io
 Project-URL: Source Code, https://github.com/ubccr/coldfront
@@ -22,29 +22,30 @@
 
 ![ColdFront](docs/pages/images/logo-lg.png)
 
 # ColdFront - Resource Allocation System
 
 [![Documentation Status](https://readthedocs.org/projects/coldfront/badge/?version=latest)](https://coldfront.readthedocs.io/en/latest/?badge=latest)
 
-ColdFront is an open source resource allocation system designed to provide a
+ColdFront is an open source resource and allocation management system designed to provide a
 central portal for administration, reporting, and measuring scientific impact
-of HPC resources. ColdFront was created to help HPC centers manage access to a
-diverse set of resources across large groups of users and provide a rich set of
-extensible meta data for comprehensive reporting. ColdFront is written in
-Python and released under the GPLv3 license.
+of cyberinfrastructure resources. ColdFront was created to help high performance computing (HPC) centers manage access to a diverse set of resources across large groups of users and provide a rich set of
+extensible meta data for comprehensive reporting. The flexiblity of ColdFront allows centers to manage and automate their policies and procedures within the framework provided or extend the functionality with [plugins](docs/pages/index.md#extensibility).  ColdFront is written in Python and released under the GPLv3 license.
 
 ## Features
 
 - Allocation based system for managing access to resources
-- Collect Project, Grant, and Publication data from users
-- Define custom attributes on resources and allocations
+- Self-service portal for users to request access to resources for their research group
+- Collection of Project, Grant, and Publication data from users
+- Center director approval system and annual project review process
 - Email notifications for expiring/renewing access to resources
-- Integration with 3rd party systems for automation and access control
-- Center director approval system and annual project reviews
+- Ability to define custom attributes on resources and allocations 
+- Integration with 3rd party systems for automation, access control, and other system provisioning tasks
+
+[Read more](docs/pages/index.md)  
 
 ## Community Supported Plugins
 
 - [OpenStack Plugin](https://github.com/nerc-project/coldfront-plugin-openstack)
 - [Keycloak User Search](https://github.com/nerc-project/coldfront-plugin-keycloak)
 - [Starfish Plugin](https://github.com/fasrc/sftocf)
```

### Comparing `coldfront-1.1.4/README.md` & `coldfront-1.1.5/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 ![ColdFront](docs/pages/images/logo-lg.png)
 
 # ColdFront - Resource Allocation System
 
 [![Documentation Status](https://readthedocs.org/projects/coldfront/badge/?version=latest)](https://coldfront.readthedocs.io/en/latest/?badge=latest)
 
-ColdFront is an open source resource allocation system designed to provide a
+ColdFront is an open source resource and allocation management system designed to provide a
 central portal for administration, reporting, and measuring scientific impact
-of HPC resources. ColdFront was created to help HPC centers manage access to a
-diverse set of resources across large groups of users and provide a rich set of
-extensible meta data for comprehensive reporting. ColdFront is written in
-Python and released under the GPLv3 license.
+of cyberinfrastructure resources. ColdFront was created to help high performance computing (HPC) centers manage access to a diverse set of resources across large groups of users and provide a rich set of
+extensible meta data for comprehensive reporting. The flexiblity of ColdFront allows centers to manage and automate their policies and procedures within the framework provided or extend the functionality with [plugins](docs/pages/index.md#extensibility).  ColdFront is written in Python and released under the GPLv3 license.
 
 ## Features
 
 - Allocation based system for managing access to resources
-- Collect Project, Grant, and Publication data from users
-- Define custom attributes on resources and allocations
+- Self-service portal for users to request access to resources for their research group
+- Collection of Project, Grant, and Publication data from users
+- Center director approval system and annual project review process
 - Email notifications for expiring/renewing access to resources
-- Integration with 3rd party systems for automation and access control
-- Center director approval system and annual project reviews
+- Ability to define custom attributes on resources and allocations 
+- Integration with 3rd party systems for automation, access control, and other system provisioning tasks
+
+[Read more](docs/pages/index.md)  
 
 ## Community Supported Plugins
 
 - [OpenStack Plugin](https://github.com/nerc-project/coldfront-plugin-openstack)
 - [Keycloak User Search](https://github.com/nerc-project/coldfront-plugin-keycloak)
 - [Starfish Plugin](https://github.com/fasrc/sftocf)
```

### Comparing `coldfront-1.1.4/coldfront/config/auth.py` & `coldfront-1.1.5/coldfront/config/auth.py`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/config/base.py` & `coldfront-1.1.5/coldfront/config/base.py`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/config/core.py` & `coldfront-1.1.5/coldfront/config/core.py`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/config/database.py` & `coldfront-1.1.5/coldfront/config/database.py`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/config/email.py` & `coldfront-1.1.5/coldfront/config/email.py`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/config/logging.py` & `coldfront-1.1.5/coldfront/config/logging.py`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/config/plugins/ldap.py` & `coldfront-1.1.5/coldfront/config/plugins/ldap.py`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/config/plugins/ldap_user_search.py` & `coldfront-1.1.5/coldfront/config/plugins/ldap_user_search.py`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/config/plugins/openid.py` & `coldfront-1.1.5/coldfront/config/plugins/openid.py`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/config/settings.py` & `coldfront-1.1.5/coldfront/config/settings.py`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/config/urls.py` & `coldfront-1.1.5/coldfront/config/urls.py`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/core/allocation/admin.py` & `coldfront-1.1.5/coldfront/core/allocation/admin.py`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/core/allocation/forms.py` & `coldfront-1.1.5/coldfront/core/allocation/forms.py`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/core/allocation/management/commands/add_allocation_defaults.py` & `coldfront-1.1.5/coldfront/core/allocation/management/commands/add_allocation_defaults.py`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/core/allocation/migrations/0001_initial.py` & `coldfront-1.1.5/coldfront/core/allocation/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/core/allocation/migrations/0002_auto_20190718_1451.py` & `coldfront-1.1.5/coldfront/core/allocation/migrations/0002_auto_20190718_1451.py`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/core/allocation/migrations/0003_auto_20191018_1049.py` & `coldfront-1.1.5/coldfront/core/allocation/migrations/0003_auto_20191018_1049.py`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/core/allocation/migrations/0004_auto_20211102_1017.py` & `coldfront-1.1.5/coldfront/core/allocation/migrations/0004_auto_20211102_1017.py`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/core/allocation/migrations/0005_auto_20211117_1413.py` & `coldfront-1.1.5/coldfront/core/allocation/migrations/0005_auto_20211117_1413.py`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/core/allocation/models.py` & `coldfront-1.1.5/coldfront/core/attribute_expansion.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,528 +1,516 @@
-import datetime
-import importlib
+#Collection of functions related to attribute expansion.
+#
+#This is a collection common functions related to the expansion
+#of parameters (typically related to other attributes) inside of 
+#attributes.  Used in the expanded_value() method of AllocationAttribute
+#and ResourceAttribute.
+
 import logging
-from ast import literal_eval
-from enum import Enum
+import math
 
-from django.conf import settings
-from django.contrib.auth.models import User
-from django.core.exceptions import ValidationError
-from django.db import models
-from django.utils.html import mark_safe
-from django.utils.module_loading import import_string
-from model_utils.models import TimeStampedModel
-from simple_history.models import HistoricalRecords
-
-from coldfront.core.project.models import Project, ProjectPermission
-from coldfront.core.resource.models import Resource
-from coldfront.core.utils.common import import_from_settings
-import coldfront.core.attribute_expansion as attribute_expansion
 
 logger = logging.getLogger(__name__)
 
-ALLOCATION_ATTRIBUTE_VIEW_LIST = import_from_settings(
-    'ALLOCATION_ATTRIBUTE_VIEW_LIST', [])
-ALLOCATION_FUNCS_ON_EXPIRE = import_from_settings(
-    'ALLOCATION_FUNCS_ON_EXPIRE', [])
-ALLOCATION_RESOURCE_ORDERING = import_from_settings(
-    'ALLOCATION_RESOURCE_ORDERING',
-    ['-is_allocatable', 'name'])
-
-class AllocationPermission(Enum):
-    USER = 'USER'
-    MANAGER = 'MANAGER'
-
-class AllocationStatusChoice(TimeStampedModel):
-    name = models.CharField(max_length=64)
-
-    def __str__(self):
-        return self.name
-
-    class Meta:
-        ordering = ['name', ]
-
-
-class Allocation(TimeStampedModel):
-    """ Allocation to a system Resource. """
-    project = models.ForeignKey(Project, on_delete=models.CASCADE,)
-    resources = models.ManyToManyField(Resource)
-    status = models.ForeignKey(
-        AllocationStatusChoice, on_delete=models.CASCADE, verbose_name='Status')
-    quantity = models.IntegerField(default=1)
-    start_date = models.DateField(blank=True, null=True)
-    end_date = models.DateField(blank=True, null=True)
-    justification = models.TextField()
-    description = models.CharField(max_length=512, blank=True, null=True)
-    is_locked = models.BooleanField(default=False)
-    is_changeable = models.BooleanField(default=False)
-    history = HistoricalRecords()
-
-    class Meta:
-        ordering = ['end_date', ]
-
-        permissions = (
-            ('can_view_all_allocations', 'Can view all allocations'),
-            ('can_review_allocation_requests',
-             'Can review allocation requests'),
-            ('can_manage_invoice', 'Can manage invoice'),
-        )
-
-    def clean(self):
-        if self.status.name == 'Expired':
-            if not self.end_date:
-                raise ValidationError('You have to set the end date.')
-
-            if self.end_date > datetime.datetime.now().date():
-                raise ValidationError(
-                    'End date cannot be greater than today.')
-
-            if self.start_date > self.end_date:
-                raise ValidationError(
-                    'End date cannot be greater than start date.')
-
-        elif self.status.name == 'Active':
-            if not self.start_date:
-                raise ValidationError('You have to set the start date.')
-
-            if not self.end_date:
-                raise ValidationError('You have to set the end date.')
-
-            if self.start_date > self.end_date:
-                raise ValidationError(
-                    'Start date cannot be greater than the end date.')
-
-    def save(self, *args, **kwargs):
-        if self.pk:
-            old_obj = Allocation.objects.get(pk=self.pk)
-            if old_obj.status.name != self.status.name and self.status.name == 'Expired':
-                for func_string in ALLOCATION_FUNCS_ON_EXPIRE:
-                    func_to_run = import_string(func_string)
-                    func_to_run(self.pk)
-
-        super().save(*args, **kwargs)
-
-    @property
-    def expires_in(self):
-        return (self.end_date - datetime.date.today()).days
-
-    @property
-    def get_information(self):
-        html_string = ''
-        for attribute in self.allocationattribute_set.all():
-            if attribute.allocation_attribute_type.name in ALLOCATION_ATTRIBUTE_VIEW_LIST:
-                html_string += '%s: %s <br>' % (
-                    attribute.allocation_attribute_type.name, attribute.value)
-
-            if hasattr(attribute, 'allocationattributeusage'):
-                try:
-                    percent = round(float(attribute.allocationattributeusage.value) /
-                                    float(attribute.value) * 10000) / 100
-                except ValueError:
-                    percent = 'Invalid Value'
-                    logger.error("Allocation attribute '%s' is not an int but has a usage",
-                                 attribute.allocation_attribute_type.name)
-                except ZeroDivisionError:
-                    percent = 100
-                    logger.error("Allocation attribute '%s' == 0 but has a usage",
-                                 attribute.allocation_attribute_type.name)
-
-                string = '{}: {}/{} ({} %) <br>'.format(
-                    attribute.allocation_attribute_type.name,
-                    attribute.allocationattributeusage.value,
-                    attribute.value,
-                    percent
-                )
-                html_string += string
-
-        return mark_safe(html_string)
-
-    @property
-    def get_resources_as_string(self):
-        return ', '.join([ele.name for ele in self.resources.all().order_by(
-            *ALLOCATION_RESOURCE_ORDERING)])
-
-    @property
-    def get_resources_as_list(self):
-        return [ele for ele in self.resources.all().order_by('-is_allocatable')]
-
-    @property
-    def get_parent_resource(self):
-        if self.resources.count() == 1:
-            return self.resources.first()
-        else:
-            parent = self.resources.order_by(
-                *ALLOCATION_RESOURCE_ORDERING).first()
-            if parent:
-                return parent
-            # Fallback
-            return self.resources.first()
-
-    def get_attribute(self, name, expand=True, typed=True,
-        extra_allocations=[]):
-        """Return the value of the first attribute found with specified name
-
-        This will return the value of the first attribute found for this
-        allocation with the specified name.
-
-        If expand is True (the default), we will return the expanded_value()
-        method of the attribute, which will expand attributes/parameters in
-        the attribute value for attributes with a base type of 'Attribute
-        Expanded Text'.  If the attribute is not of that type, or expand is
-        false, returns the value attribute/data member (i.e. the raw, unexpanded
-        value).
-
-        Extra_allocations is a list of Allocations which, if expand is True,
-        will have their attributes available for referencing.
-
-        If typed is True (the default), we will attempt to convert the value
-        returned to the appropriate python type (int/float/str) based on the
-        base AttributeType name.
-        """
-        attr = self.allocationattribute_set.filter(
-            allocation_attribute_type__name=name).first()
-        if attr:
-            if expand:
-                return attr.expanded_value(
-                    extra_allocations=extra_allocations, typed=typed)
-            else:
-                if typed:
-                    return attr.typed_value()
-                else:
-                    return attr.value
-        return None
+#ALLOCATION_ATTRIBUTE_VIEW_LIST = import_from_settings(
+#    'ALLOCATION_ATTRIBUTE_VIEW_LIST', [])
 
-    def set_usage(self, name, value):
-        attr = self.allocationattribute_set.filter(
-            allocation_attribute_type__name=name).first()
-        if not attr:
-            return
-
-        if not attr.allocation_attribute_type.has_usage:
-            return
-
-        if not AllocationAttributeUsage.objects.filter(allocation_attribute=attr).exists():
-            usage = AllocationAttributeUsage.objects.create(
-                allocation_attribute=attr)
-        else:
-            usage = attr.allocationattributeusage
+ATTRIBUTE_EXPANSION_TYPE_PREFIX = 'Attribute Expanded'
+ATTRIBUTE_EXPANSION_ATTRIBLIST_SUFFIX = '_attriblist'
 
-        usage.value = value
-        usage.save()
 
-    def get_attribute_list(self, name, expand=True, typed=True,
-        extra_allocations=[]):
-        """Return a list of values of the attributes found with specified name
-
-        This will return a list consisting of the values of the all attributes
-        found for this allocation with the specified name.
-
-        If expand is True (the default), we will return the result of the
-        expanded_value() method for each attribute, which will expand 
-        attributes/parameters in the attribute value for attributes with a base 
-        type of 'Attribute Expanded Text'.  If the attribute is not of that 
-        type, or expand is false, returns the value attribute/data member (i.e. 
-        the raw, unexpanded value).
-
-        Extra_allocations is a list of Allocations which, if expand is True,
-        will have their attributes available for referencing.
-        """
-        attr = self.allocationattribute_set.filter(
-            allocation_attribute_type__name=name).all()
-        if expand:
-            return [a.expanded_value(typed=typed,
-                extra_allocations=extra_allocations) for a in attr]
-        else:
-            if typed:
-                return [a.typed_value() for a in attr]
+def is_expandable_type(attribute_type):
+    """Returns True if attribute_type is expandable.
+
+    Takes an AttributeType (from either Resource or Allocation, but
+    wants AttributeType, not ResourceAttributeType or
+    AllocationAttributeType) and checks if type name matches 
+    ATTRIBUTE_EXPANSION_TYPE_PREFIX
+    """
+
+    atype_name = attribute_type.name;
+    return atype_name.startswith(ATTRIBUTE_EXPANSION_TYPE_PREFIX)
+
+def get_attriblist_str(attribute_name, resources=[], allocations=[]):
+    """This finds the attriblist string for the named expandable attribute.
+
+    We append the ATTRIBUTE_EXPANSION_ATTRIBLIST_SUFFIX to the given
+    attribute_name, and then search for attributes with that name in
+    all resources and allocations given.  The values of any such attriblist
+    attributes found are concatenated together and returned.  If no
+    attriblist attributes are found, we return None.
+    """
+
+    attriblist_name = "{aname}{suffix}".format(
+        aname=attribute_name, suffix=ATTRIBUTE_EXPANSION_ATTRIBLIST_SUFFIX)
+    attriblist = None
+
+    # Check resources first
+    for res in resources:
+        alist_list = res.get_attribute_list(attriblist_name)
+        for alist in alist_list:
+            if attriblist:
+                attriblist = attriblist + '\n' + alist
             else:
-                return [a.value for a in attr]
-
-    def get_attribute_set(self, user):
-        """Returns the set of allocation attributes the user is allowed to view.
-           1. super users can see all allocation attributes
-           2. all other users can only see non-private ones
-        """
-        if user.is_superuser:
-            return self.allocationattribute_set.all().order_by('allocation_attribute_type__name')
-
-        return self.allocationattribute_set.filter(allocation_attribute_type__is_private=False).order_by('allocation_attribute_type__name')
-
-    def user_permissions(self, user):
-        """Return list of a user's permissions for the allocation
-        """
-        if user.is_superuser:
-            return list(AllocationPermission)
-
-        project_perms = self.project.user_permissions(user)
-
-        if ProjectPermission.USER not in project_perms:
-            return []
-
-        if ProjectPermission.PI in project_perms or ProjectPermission.MANAGER in project_perms:
-            return [AllocationPermission.USER, AllocationPermission.MANAGER]
-
-        if self.allocationuser_set.filter(user=user, status__name__in=['Active', 'New', ]).exists():
-            return [AllocationPermission.USER]
-
-        return []
-
-    def has_perm(self, user, perm):
-        """Return true if user has permission for the allocation
-        """
-        perms = self.user_permissions(user)
-        return perm in perms
-
-    def __str__(self):
-        return "%s (%s)" % (self.get_parent_resource.name, self.project.pi)
-
-
-class AllocationAdminNote(TimeStampedModel):
-    allocation = models.ForeignKey(Allocation, on_delete=models.CASCADE)
-    author = models.ForeignKey(User, on_delete=models.CASCADE)
-    note = models.TextField()
-
-    def __str__(self):
-        return self.note
-
-
-class AllocationUserNote(TimeStampedModel):
-    allocation = models.ForeignKey(Allocation, on_delete=models.CASCADE)
-    author = models.ForeignKey(User, on_delete=models.CASCADE)
-    is_private = models.BooleanField(default=True)
-    note = models.TextField()
-
-    def __str__(self):
-        return self.note
-
-
-class AttributeType(TimeStampedModel):
-    """ AttributeType. """
-    name = models.CharField(max_length=64)
-
-    def __str__(self):
-        return self.name
-
-    class Meta:
-        ordering = ['name', ]
-
-
-class AllocationAttributeType(TimeStampedModel):
-    """ AllocationAttributeType. """
-    attribute_type = models.ForeignKey(AttributeType, on_delete=models.CASCADE)
-    name = models.CharField(max_length=50)
-    has_usage = models.BooleanField(default=False)
-    is_required = models.BooleanField(default=False)
-    is_unique = models.BooleanField(default=False)
-    is_private = models.BooleanField(default=True)
-    is_changeable = models.BooleanField(default=False)
-    history = HistoricalRecords()
-
-    def __str__(self):
-        return '%s' % (self.name)
-
-    class Meta:
-        ordering = ['name', ]
-
-
-class AllocationAttribute(TimeStampedModel):
-    """ AllocationAttribute. """
-    allocation_attribute_type = models.ForeignKey(
-        AllocationAttributeType, on_delete=models.CASCADE)
-    allocation = models.ForeignKey(Allocation, on_delete=models.CASCADE)
-    value = models.CharField(max_length=128)
-    history = HistoricalRecords()
-
-    def save(self, *args, **kwargs):
-        super().save(*args, **kwargs)
-        if self.allocation_attribute_type.has_usage and not AllocationAttributeUsage.objects.filter(allocation_attribute=self).exists():
-            AllocationAttributeUsage.objects.create(
-                allocation_attribute=self)
-
-    def clean(self):
-        if self.allocation_attribute_type.is_unique and self.allocation.allocationattribute_set.filter(allocation_attribute_type=self.allocation_attribute_type).exclude(id=self.pk).exists():
-            raise ValidationError("'{}' attribute already exists for this allocation.".format(
-                self.allocation_attribute_type))
-
-        expected_value_type = self.allocation_attribute_type.attribute_type.name.strip()
-
-        if expected_value_type == "Int" and not isinstance(literal_eval(self.value), int):
-            raise ValidationError(
-                'Invalid Value "%s" for "%s". Value must be an integer.' % (self.value, self.allocation_attribute_type.name))
-        elif expected_value_type == "Float" and not (isinstance(literal_eval(self.value), float) or isinstance(literal_eval(self.value), int)):
-            raise ValidationError(
-                'Invalid Value "%s" for "%s". Value must be a float.' % (self.value, self.allocation_attribute_type.name))
-        elif expected_value_type == "Yes/No" and self.value not in ["Yes", "No"]:
-            raise ValidationError(
-                'Invalid Value "%s" for "%s". Allowed inputs are "Yes" or "No".' % (self.value, self.allocation_attribute_type.name))
-        elif expected_value_type == "Date":
-            try:
-                datetime.datetime.strptime(self.value.strip(), "%Y-%m-%d")
-            except ValueError:
-                raise ValidationError(
-                    'Invalid Value "%s" for "%s". Date must be in format YYYY-MM-DD' % (self.value, self.allocation_attribute_type.name))
-
-    def __str__(self):
-        return '%s' % (self.allocation_attribute_type.name)
-
-    def typed_value(self):
-        """Returns the value of the attribute, with proper type.
-
-        For attributes with Int or Float types, we return the value of
-        the attribute coerced into an Int or Float.  If the coercion
-        fails, we log a warning and return the string.
-
-        For all other attribute types, we return the value as a string.
-
-        This is needed when computing values for expanded_value()
-        """
-        raw_value = self.value
-        atype_name = self.allocation_attribute_type.attribute_type.name
-        return attribute_expansion.convert_type(
-            value=raw_value, type_name=atype_name)
-                
-    
-    def expanded_value(self, extra_allocations=[], typed=True):
-        """Returns the value of the attribute, after attribute expansion.
-
-        For attributes with attribute type of  'Attribute Expanded Text' we
-        look for an attribute with same name suffixed with '_attriblist' (this
-        should be either an AllocationAttribute of the Allocation associated
-        with this attribute  or a ResourceAttribute of a Resource of the 
-        Allocation associated with this AllocationAttribute).  
-        If the attriblist attribute is found, we use
-        it to generate a dictionary to use to expand the attribute value,
-        and the expanded value is returned.  
-        If extra_allocations is given, it should be a list of Allocations and
-        the attriblist can reference attributes for allocations in the
-        extra_allocations list (as well as in the Allocation associated with
-        this AllocationAttribute or Resources associated with that allocation)
-
-        If typed is True (the default), we use typed to convert the returned
-        value to the expected (int, float, str) python data type according to
-        the AttributeType of the AllocationAttributeType (unrecognized values
-        not converted, so will return str).
-
-        If the expansion fails, or if no attriblist attribute is found, or if
-        the attribute type is not 'Attribute Expanded Text', we just return
-        the raw value.
-        """
-        raw_value = self.value
-        if typed:
-            # Try to convert to python type as per AttributeType
-            raw_value = self.typed_value()
-
-        if not attribute_expansion.is_expandable_type(
-            self.allocation_attribute_type.attribute_type):
-            # We are not an expandable type, return raw_value
-            return raw_value
-
-        allocs = [ self.allocation ] + extra_allocations
-        resources = list(self.allocation.resources.all())
-        attrib_name = self.allocation_attribute_type.name
-
-        attriblist = attribute_expansion.get_attriblist_str(
-            attribute_name = attrib_name,
-            resources = resources,
-            allocations = allocs)
-
-        if not attriblist:
-            # We do not have an attriblist, return raw_value
-            return raw_value
-
-        expanded = attribute_expansion.expand_attribute(
-            raw_value = raw_value,
-            attribute_name = attrib_name,
-            attriblist_string = attriblist,
-            resources = resources,
-            allocations = allocs)
-        return expanded
-
-            
-
-class AllocationAttributeUsage(TimeStampedModel):
-    """ AllocationAttributeUsage. """
-    allocation_attribute = models.OneToOneField(
-        AllocationAttribute, on_delete=models.CASCADE, primary_key=True)
-    value = models.FloatField(default=0)
-    history = HistoricalRecords()
-
-    def __str__(self):
-        return '{}: {}'.format(self.allocation_attribute.allocation_attribute_type.name, self.value)
-
-
-class AllocationUserStatusChoice(TimeStampedModel):
-    name = models.CharField(max_length=64)
-
-    def __str__(self):
-        return self.name
-
-    class Meta:
-        ordering = ['name', ]
-
-
-class AllocationUser(TimeStampedModel):
-    """ AllocationUser. """
-    allocation = models.ForeignKey(Allocation, on_delete=models.CASCADE)
-    user = models.ForeignKey(User, on_delete=models.CASCADE)
-    status = models.ForeignKey(AllocationUserStatusChoice, on_delete=models.CASCADE,
-                               verbose_name='Allocation User Status')
-    history = HistoricalRecords()
-
-    def __str__(self):
-        return '%s' % (self.user)
-
-    class Meta:
-        verbose_name_plural = 'Allocation User Status'
-        unique_together = ('user', 'allocation')
-
-
-class AllocationAccount(TimeStampedModel):
-    user = models.ForeignKey(User, on_delete=models.CASCADE)
-    name = models.CharField(max_length=64, unique=True)
+                attriblist = alist
+    # Then check allocations
+    for alloc in allocations:
+        alist_list = alloc.get_attribute_list(attriblist_name)
+        for alist in alist_list:
+            if attriblist:
+                attriblist = attriblist + '\n' + alist
+            else:
+                attriblist = alist
 
-    def __str__(self):
-        return self.name
+    return attriblist
 
-    class Meta:
-        ordering = ['name', ]
+def get_attribute_parameter_value(
+    argument, attribute_parameter_dict, error_text,
+    resources=[], allocations=[]):
+    """Evaluates the argument for a attribute parameter statement.
+
+    This is called by process_attribute_parameter_string and handles
+    evaluating/dereferencing the argument portion of the statement.
+
+    The following argument types are recognized:
+    APDICT:pname - expands to the value of a parameter named pname already
+        in the attribute_parameter_dict (or None if not present)
+    RESOURCE:aname - expands to the value of the first attribute of type
+        named aname found in the resources list of resources. 
+        NOTE: 'RESOURCE:' is a literal.  Or None if not found.
+    ALLOCATION:aname - expands to the value of the first attribute of type
+        named aname found in the allocations list of allocations.
+        NOTE: 'ALLOCATION:' is a literal.  Or None if not found.
+    :keyname - expands to value of the parameter named keyname in
+        attribute_parameter_dict, or if not found then will expand to the
+        value of the first attribute of type named aname found in the
+        allocations list, or then resources list.  Or None if all the
+        preceding fail.
+    'single line of text' - expands to a string literal contained between
+        the two single quotes.  Very simplistic, nothing is allowed after
+        the last single quote, and we just remove the leading and trailing
+        single quote --- everything in between is treated literally 
+        (including any contained single quotes).
+    digits (optionally with decimal): expands to a numeric literal
+
+    error_text is used to give context in diagnostic messages.
+
+    This method returns the expanded value, or None if unable to 
+    evaluate
+    """
+    value = None
+    
+    # Check for string constant
+    if argument.startswith("'"):
+        # Looks like a string literal
+        # Strip leading quote
+        tmpstr = argument[1:]
+        # Verify the last character is a single quote
+        tmp = tmpstr[-1:]
+        if tmp == "'":
+            #Good string literal
+            tmpstr = tmpstr[:-1]
+            return tmpstr
+        else:
+            #Bad string literal
+            logger.warn("Bad string literal '{}' found while processing "
+                "{}; missing final single quote".format(
+                argument, error_text))
+            return None
+
+    # If argument if prefixed with any of the strings in attrib_sources,
+    # strip the prefix and set attrib_source accordingly
+    attrib_source = None
+    attrib_sources = [ ':APDICT', 'RESOURCE:', 'ALLOCATION:', ':' ]
+    for asrc in attrib_sources:
+        if argument.startswith(asrc):
+            # Got a match
+            attrib_source = asrc
+            tmplen = len(asrc)
+            argument = argument[tmplen:]
+            break
+
+    # Try expanding as a parameter/attribute
+    # We do attribute_parameter_dict first, then allocations, then
+    # resources to try to get value most specific to use case
+    if ( attribute_parameter_dict is not None and 
+        (attrib_source == ':' or attrib_source == 'APDICT:')):
+        if argument in attribute_parameter_dict:
+            return attribute_parameter_dict[argument]
+
+    if attrib_source == ':' or attrib_source == 'ALLOCATION:':
+        for alloc in allocations:
+            tmp = alloc.get_attribute(argument)
+            if tmp is not None:
+                return tmp
+
+    if attrib_source == ':' or attrib_source == 'RESOURCE:':
+        for res in resources:
+            tmp = res.get_attribute(argument)
+            if tmp is not None:
+                return tmp
+
+    if attrib_source is not None:
+        # We were given an attribute or parameter name, but could not
+        # find it.  Just return None
+        return None
 
+    # If reach here, argument is not a string literal, or a 
+    # parameter or attribute name, so try numeric constant
+    try:
+        value = int(argument)
+        return value
+    except ValueError:
+        try:
+            value = float(argument)
+            return value
+        except ValueError:
+            logger.warn("Unable to evaluate argument '{arg}' while "
+                "processing {etxt}, returning None".format(
+                arg=argument, etxt=error_text))
+            return None
 
-class AllocationChangeStatusChoice(TimeStampedModel):
-    name = models.CharField(max_length=64)
+    # Should not reach here
+    return None
+    
+def process_attribute_parameter_operation(
+    opcode, oldvalue, argument, error_text):
+    """Process the specified operation for attribute_parameter_dict.
+
+    This is called by process_attribute_parameter_string and handles
+    performing the specifed operation on the parameter.  Oldvalue is
+    the starting value of the parameter (or None if not previously
+    defined), opcode is the one character operation to perform, and
+    argument is argument to the operation (typically the value of
+    a constant, parameter, or attribute --- this should have been
+    previously dereferenced by get_attribute_parameter_value).
+
+    Opcode is the single character preceding the '=' in the parameter
+    definition/statement.  E.g. the ':' in ':=', etc.  Recognized
+    values are:
+    : - assignment.  Any previous value of parameter will be replaced
+        by argument. (Oldvalue is allowed to be None)
+    | - default. If oldvalue is None, the value of the parameter is
+        replaced by argument.  Otherwise, no action is taken.
+    + - addition.  The new value of parameter is the oldvalue plus
+        argument for numerical values.  For string values, it is
+        oldvalue with argument concatenated to it (ie string +).
+    - - subtraction: Numeric values only.  newval = oldvalue - argument
+    * - multiplication: Numeric values only.  newval = oldvalue * argument
+    / - division: Numeric values only.  newval = oldvalue / argument
+    ( - apply unary function: In this case, argument is the name of an
+        unary function to apply to oldvalue.  Recognized function names are:
+        'floor': converts oldvalue to integer using floor()
+
+    Error_text is used to provide context in diagnostic messages.
+
+    On success, returns the new value that should be used for the
+    parameter.  Generally returns None on errors (e.g. undefined
+    required values, or bad types, etc)
+    """
+    # Argument should never be None
+    if argument is None:
+        logger.warn("Operator {}= acting on None argument in {}, "
+            "returning None".format(opcode, error_text))
+        return None
+    # Assignment and default operations allow oldvalue to be None
+    if oldvalue is None:
+        if opcode != ':' and opcode != '|':
+            logger.warn("Operator {}= acting on oldvalue=None in {}, "
+                "returning None".format(opcode, error_text))
+            return None
+
+    try:
+        if opcode == ':':
+            # Assignment operation
+            return argument
+        if opcode == '|':
+            # Defaulting operation
+            if oldvalue is None:
+                return argument
+            else:
+                return oldvalue
+        if opcode == '+':
+            # Addition/concatenation operation
+            if isinstance(oldvalue, int) or isinstance(oldvalue, float):
+                newval = oldvalue + argument
+                return newval
+            elif isinstance(oldvalue, str):
+                newval = oldvalue + argument
+                return newval
+            else:
+                logger.warn('Operator {}= acting on parameter of type '
+                    '{} in {}, returning None'.format(
+                    opcode, type(oldvalue), error_text))
+                return None
+        if opcode == '-':
+            newval = oldvalue - argument
+            return newval
+        if opcode == '*':
+            newval = oldvalue * argument
+            return newval
+        if opcode == '/':
+            newval = oldvalue / argument
+            return newval
+        if opcode == '(':
+            if argument == 'floor':
+                newval = math.floor(oldvalue)
+            else:
+                logger.error('Unrecognized function named {} in {}= for '
+                    '{}, returning None'.format(
+                    argument, opcode, error_text))
+                return None
+        # If reached here, we do not recognize opcode
+        logger.error('Unrecognized operation {}= in {}, '
+            'returning None'.format( opcode, error_text))
+    except Exception as xcept:
+        logger.warn("Error performing operator {op}= on oldvalue='{old}' "
+            "and argument={arg} in {errtext}".format(
+            op=opcode, old=oldvalue, arg=argument, errtext=error_text))
+        return None
 
-    def __str__(self):
-        return self.name
 
-    class Meta:
-        ordering = ['name', ]
+def process_attribute_parameter_string(
+    parameter_string, attribute_name, attribute_parameter_dict = {},
+    resources = [], allocations = []):
+    """Processes a single attribute parameter definition/statement.
+
+    This is called by make_attribute_parameter_dictionary, and handles
+    the processing of a single attribute parameter definition/statement
+    given by 'parameter_string' in the attribute parameter list.  The
+    passed attribute_parameter_dict, as well as passed lists of resources
+    and allocations, will be used when dereferencing parameters/attributes,
+    and the new value for any parameter will be stored back in the
+    attribute_parameter_dict, which is also returned.
+
+    Attribute_name is just used in diagnostic messages.
+
+    Each statement should have the general form:
+    '<parameter_name> <op>= <argument>'
+    <parameter_name> is the name of the parameter in
+    attribute_parameter_dict to create/update.
+    <op> is a single character operator defining the operation to do
+    on the specified parameter.
+    <argument> is an additional argument to use in the operation.  Typically
+    it will be a numeric constant, a string constant, or the name of an
+    AllocationAttribute or ResourceAttribute (which is then replaced by
+    its (expanded if expandable) value).
+
+    See the methods get_attribute_parameter_value() and 
+    process_attribute_parameter_operation() for more information about
+    the operations and argument values.
+    """
+
+    # Strip leading/trailing white space
+    parmstr = parameter_string.strip()
+    # Ignore comment lines/blank lines (return attribute_parameter_dict)
+    if not parmstr:
+        return attribute_parameter_dict
+    if parmstr.startswith('#'):
+        return attribute_parameter_dict
+
+    # Parse the parameter string to get pname, op, and argument
+    tmp = parmstr.split('=', 1)
+    if len(tmp) != 2:
+        # No '=' found, so invalid format of parmstr
+        # Log error and return unmodified attribute_parameter_dict
+        logger.error("Invalid parameter string '{pstr}', no '=', while "
+            "creating attribute parameter dictionary for expanding "
+            "attribute {aname}".format(
+            aname=attribute_name, pstr=parameter_string))
+        return attribute_parameter_dict
+    pname = tmp[0]
+    argument = tmp[1].strip()
+    # Remove opcode and remove trailing whitespace from pname
+    opcode = pname[-1:]
+    pname = pname[:-1].strip()
+
+    # Argument is a parameter/attribute/constant unless opcode is '('
+    # So get its value if parameter/attribute/constant
+    value = None
+    if opcode == '(':
+        value = argument
+    else:
+        # Extra text to display in diagnostics if error occurs
+        error_text = 'processing attribute_parameter_string={pstr} ' \
+            'for expansion of attribute {aname}'.format(
+            pstr = parameter_string, aname=attribute_name)
+        value = get_attribute_parameter_value(
+            argument = argument,
+            attribute_parameter_dict = attribute_parameter_dict,
+            resources = resources, 
+            allocations = allocations,
+            error_text = error_text)
+
+    # Get the old value of the parameter
+    if pname in attribute_parameter_dict:
+        oldval = attribute_parameter_dict[pname]
+    else:
+        oldval = None
+
+    # Perform the requested operation
+    newval = process_attribute_parameter_operation(
+        opcode=opcode, oldvalue=oldval, argument=value,
+        error_text=error_text)
+    # Set value in dictionary and return
+    attribute_parameter_dict[pname] = newval
+    return attribute_parameter_dict
+
+
+def make_attribute_parameter_dictionary(attribute_name,
+        attribute_parameter_string, resources=[], allocations=[]):
+    """Create the attribute parameter dictionary.  Used by expand_attribute.
+
+    This processes the given attribute parameter string to generate a
+    dictionary that will (in expand_attribute()) be passed as the argument 
+    to the standard python format() method acting on the raw value of the 
+    attribute to expand it.
+
+    The attribute parameter string is a string consisting of one or more
+    attribute parameter definitions, one per line, with the following
+    general format:
+    '<parameter_name> <op>= <argument>'
+    
+    This routine processes the attribute_parameter_string line by line, in
+    order top to bottom, to generate the dictionary that is returned.
 
+    See process_attribute_parameter_string for details on the processing
+    of each line.
+    """
+
+    # Initialize our dictionary
+    apdict = dict()
+
+    # Covert attribute_parameter_string to a real list
+    attrib_parm_list = list(map(str.strip,
+        attribute_parameter_string.splitlines() ))
+    # Process each element in the list
+    for parmstr in attrib_parm_list:
+        apdict = process_attribute_parameter_string(
+            parameter_string = parmstr,
+            attribute_parameter_dict = apdict,
+            attribute_name = attribute_name,
+            resources = resources,
+            allocations = allocations)
+    return apdict
 
-class AllocationChangeRequest(TimeStampedModel):
-    allocation = models.ForeignKey(Allocation, on_delete=models.CASCADE,)
-    status = models.ForeignKey(
-        AllocationChangeStatusChoice, on_delete=models.CASCADE, verbose_name='Status')
-    end_date_extension = models.IntegerField(blank=True, null=True)
-    justification = models.TextField()
-    notes = models.CharField(max_length=512, blank=True, null=True)
-    history = HistoricalRecords()
 
-    @property
-    def get_parent_resource(self):
-        if self.allocation.resources.count() == 1:
-            return self.allocation.resources.first()
-        else:
-            return self.allocation.resources.filter(is_allocatable=True).first()
+def expand_attribute(raw_value, attribute_name, attriblist_string, 
+    resources = [], allocations = []):
+    """Main method to expand parameters in an attribute.
+
+    This takes the (raw) value raw_value of either an AllocationAttribute 
+    or ResourceAttribute, which should be in a python formatted string 
+    (f-string) format; i.e. a string with places where parameter 
+    replacement is desired to have the name of the desired replacement 
+    parameter enclosed in curly braces ('{' and '}').  The parameter name 
+    can be followed by standard format() format specifiers, as per
+    standard format() rules.  The argument attribute_name should have
+    the name of this attribute, for use in diagnostic messages.
+
+    The parameters and their values are defined in attriblist_string.
+    This string consists of one or more parameter declaration statements,
+    one per line.  Each parameter declaration statement is of the form
+    '<parameter_name> <op>= <argument>'
+    Leading and trailing whitespace, as well as whitespace around the
+    <op>= string, is ignored.
+    These statements are processed in order from top to bottom.
+
+    <parameter_name> is the name of the parameter to be defined/operated
+    on, and should be a valid python identifier.  You can give the same
+    <parameter_name> on multiple lines to perform multiple operations on
+    the parameter, e.g. set it from an attribute then multiple by another
+    attribute.
+
+    <op> is a single character defining the operation to perform; see
+    the process_attribute_parameter_operation method for list of allowed
+    operations.
+
+    <argument> is an argument for use in the operation.  Typically it is
+    a string or numeric constant, or the name an Attribute in either
+    one of the listed resources or allocations (which would then be looked
+    up and the value returned).  See the get_attribute_parameter_value()
+    method for more information.
+
+    This method will parse the attriblist_string to form an attribute
+    parameter dictionary, which will then be used via the standard python
+    format() method to expand the parameters in the raw_value.  If all
+    of this is successful, we return the expanded string.
+
+    On errors, we just return the raw_value
+    """
+
+    # We wrap everything in a try block so we can return raw_value on error
+    try:
+        # Create the attribute parameter dictionary
+        apdict = make_attribute_parameter_dictionary(
+            attribute_parameter_string = attriblist_string,
+            attribute_name = attribute_name,
+            resources = resources,
+            allocations = allocations)
 
-    def __str__(self):
-        return "%s (%s)" % (self.get_parent_resource.name, self.allocation.project.pi)
+        # Expand the attribute
+        expanded = raw_value.format(**apdict)
+        return expanded
+    except Exception as xcept:
+        # We got an exception.  This could be for many reasons, from
+        # referencing a parameter not defined in apdict to divide by
+        # zero errors in processing apdict.  We just log it and then
+        # return raw_value
+        logger.error("Error expanding {aname}: {error}".format(
+            aname=attribute_name, error=xcept))
+        return raw_value
+
+
+def convert_type(value, type_name, error_text='unknown'):
+    """This returns value with a python type corresponding to type_name.
+
+    Value is the value to operate on.
+    Type_name is the name of the underlying attribute type (AttributeType),
+    e.g. Text, Float, Int, Date, etc.  
+
+    If type_name ends in Int, we try to return value as a python int.
+    If type_name ends in Float, we try to return value as a python float.
+    If type_name ends in Text, we try to return value as a python string.
+    For anything else, we just return value (which typically is a string)
+    If there is an error in the conversion, we just return value (and
+    log the error; error_text is used in such messages to provide context)
+
+    We compare the end of the type name, to allow for possible
+    future "Attribute Expanded ..." types.
+    """
+    if type_name is None:
+        logger.error('No AttributeType found for {}'.format(error_text))
+        return value
+
+    if type_name.endswith('Text'):
+        try:
+            newval = str(value)
+            return newval
+        except ValueError:
+            logger.error('Error converting "{}" to {} in {}'.format(
+                value, 'Text', error_text))
+            return value
+
+    if type_name.endswith('Int'):
+        try:
+            newval = int(value)
+            return newval
+        except ValueError:
+            logger.error('Error converting "{}" to {} in {}'.format(
+                value, 'Int', error_text))
+            return value
+
+    if type_name.endswith('Float'):
+        try:
+            newval = float(value)
+            return newval
+        except ValueError:
+            logger.error('Error converting "{}" to {} in {}'.format(
+                value, 'Float', error_text))
+            return value
 
+    #If not any of the above, just return the value (probably a string)
+    return value
 
-class AllocationAttributeChangeRequest(TimeStampedModel):
-    allocation_change_request = models.ForeignKey(AllocationChangeRequest, on_delete=models.CASCADE)
-    allocation_attribute = models.ForeignKey(AllocationAttribute, on_delete=models.CASCADE)
-    new_value = models.CharField(max_length=128)
-    history = HistoricalRecords()
 
-    def __str__(self):
-        return '%s' % (self.allocation_attribute.allocation_attribute_type.name)
```

### Comparing `coldfront-1.1.4/coldfront/core/allocation/tasks.py` & `coldfront-1.1.5/coldfront/core/allocation/tasks.py`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/core/allocation/templates/allocation/allocation_account_list.html` & `coldfront-1.1.5/coldfront/core/allocation/templates/allocation/allocation_account_list.html`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/core/allocation/templates/allocation/allocation_add_invoice_note.html` & `coldfront-1.1.5/coldfront/core/allocation/templates/allocation/allocation_add_invoice_note.html`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/core/allocation/templates/allocation/allocation_add_users.html` & `coldfront-1.1.5/coldfront/core/allocation/templates/allocation/allocation_add_users.html`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/core/allocation/templates/allocation/allocation_allocationattribute_create.html` & `coldfront-1.1.5/coldfront/core/allocation/templates/allocation/allocation_allocationattribute_create.html`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/core/allocation/templates/allocation/allocation_allocationattribute_delete.html` & `coldfront-1.1.5/coldfront/core/allocation/templates/allocation/allocation_allocationattribute_delete.html`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/core/allocation/templates/allocation/allocation_change.html` & `coldfront-1.1.5/coldfront/core/allocation/templates/allocation/allocation_change.html`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/core/allocation/templates/allocation/allocation_change_detail.html` & `coldfront-1.1.5/coldfront/core/allocation/templates/allocation/allocation_change_detail.html`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/core/allocation/templates/allocation/allocation_change_list.html` & `coldfront-1.1.5/coldfront/core/allocation/templates/allocation/allocation_change_list.html`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/core/allocation/templates/allocation/allocation_create.html` & `coldfront-1.1.5/coldfront/core/allocation/templates/allocation/allocation_create.html`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/core/allocation/templates/allocation/allocation_delete_invoice_note.html` & `coldfront-1.1.5/coldfront/core/allocation/templates/allocation/allocation_delete_invoice_note.html`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/core/allocation/templates/allocation/allocation_detail.html` & `coldfront-1.1.5/coldfront/core/allocation/templates/allocation/allocation_detail.html`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/core/allocation/templates/allocation/allocation_email_pending_request.html` & `coldfront-1.1.5/coldfront/core/allocation/templates/allocation/allocation_email_pending_request.html`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/core/allocation/templates/allocation/allocation_invoice_detail.html` & `coldfront-1.1.5/coldfront/core/allocation/templates/allocation/allocation_invoice_detail.html`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/core/allocation/templates/allocation/allocation_invoice_list.html` & `coldfront-1.1.5/coldfront/core/allocation/templates/allocation/allocation_invoice_list.html`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/core/allocation/templates/allocation/allocation_list.html` & `coldfront-1.1.5/coldfront/core/allocation/templates/allocation/allocation_list.html`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/core/allocation/templates/allocation/allocation_note_create.html` & `coldfront-1.1.5/coldfront/core/allocation/templates/allocation/allocation_note_create.html`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/core/allocation/templates/allocation/allocation_remove_users.html` & `coldfront-1.1.5/coldfront/core/allocation/templates/allocation/allocation_remove_users.html`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/core/allocation/templates/allocation/allocation_renew.html` & `coldfront-1.1.5/coldfront/core/allocation/templates/allocation/allocation_renew.html`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/core/allocation/templates/allocation/allocation_request_list.html` & `coldfront-1.1.5/coldfront/core/allocation/templates/allocation/allocation_request_list.html`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/core/allocation/templates/allocation/allocation_update_invoice_note.html` & `coldfront-1.1.5/coldfront/core/allocation/templates/allocation/allocation_update_invoice_note.html`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/core/allocation/urls.py` & `coldfront-1.1.5/coldfront/core/allocation/urls.py`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/core/allocation/utils.py` & `coldfront-1.1.5/coldfront/core/allocation/utils.py`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/core/allocation/views.py` & `coldfront-1.1.5/coldfront/core/allocation/views.py`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/core/field_of_science/management/commands/data/field_of_science_data.csv` & `coldfront-1.1.5/coldfront/core/field_of_science/management/commands/data/field_of_science_data.csv`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/core/field_of_science/management/commands/import_field_of_science_data.py` & `coldfront-1.1.5/coldfront/core/field_of_science/management/commands/import_field_of_science_data.py`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/core/field_of_science/migrations/0001_initial.py` & `coldfront-1.1.5/coldfront/core/field_of_science/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/core/field_of_science/tests.py` & `coldfront-1.1.5/coldfront/core/field_of_science/tests.py`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/core/grant/admin.py` & `coldfront-1.1.5/coldfront/core/grant/admin.py`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/core/grant/forms.py` & `coldfront-1.1.5/coldfront/core/grant/forms.py`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/core/grant/management/commands/add_default_grant_options.py` & `coldfront-1.1.5/coldfront/core/grant/management/commands/add_default_grant_options.py`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/core/grant/migrations/0001_initial.py` & `coldfront-1.1.5/coldfront/core/grant/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/core/grant/models.py` & `coldfront-1.1.5/coldfront/core/publication/models.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,75 +1,59 @@
-from django.core.validators import (MaxLengthValidator, MaxValueValidator,
-                                    MinLengthValidator)
 from django.db import models
 from model_utils.models import TimeStampedModel
 from simple_history.models import HistoricalRecords
 
 from coldfront.core.project.models import Project
 
 
-class GrantFundingAgency(TimeStampedModel):
-    name = models.CharField(max_length=255)
-
-    def __str__(self):
-        return self.name
+class PublicationSource(TimeStampedModel):
+    """ A publication source is a source that a publication is cited/ derived from. Examples include doi and adsabs.
+        
+    Attributes:
+        name (str): source name
+        url (URL): links to the url of the source
+    """
 
-
-class GrantStatusChoice(TimeStampedModel):
-    name = models.CharField(max_length=64)
+    name = models.CharField(max_length=255, unique=True)
+    url = models.URLField(null=True, blank=True)
 
     def __str__(self):
         return self.name
 
-    class Meta:
-        ordering = ('name',)
 
+class Publication(TimeStampedModel):
+    """ A publication source is a source that a publication is cited/ derived from. Examples include doi and adsabs.
+        
+    Attributes:
+        project (Project): links the publication to its project
+        title (str): publication title
+        author (str): publication author's name
+        year (int): year of publication
+        journal (str): journal name
+        unique_id (str): publication ID
+        source (PublicationSource): represents the source of the publication
+        status (str): publication status
+    """
 
-class Grant(TimeStampedModel):
-    """ Grant model """
     project = models.ForeignKey(Project, on_delete=models.CASCADE)
-    title = models.CharField(
-        validators=[MinLengthValidator(3), MaxLengthValidator(255)],
-        max_length=255,
-    )
-    grant_number = models.CharField(
-        'Grant Number from funding agency',
-        validators=[MinLengthValidator(3), MaxLengthValidator(255)],
-        max_length=255,
+    title = models.CharField(max_length=1024)
+    author = models.CharField(max_length=1024)
+    year = models.PositiveIntegerField()
+    journal = models.CharField(max_length=1024)
+    unique_id = models.CharField(max_length=255, null=True, blank=True)
+    source = models.ForeignKey(PublicationSource, on_delete=models.CASCADE)
+    STATUS_CHOICES = (
+        ('Active', 'Active'),
+        ('Archived', 'Archived'),
     )
-    ROLE_CHOICES = (
-        ('PI', 'Principal Investigator (PI)'),
-        ('CoPI', 'Co-Principal Investigator (CoPI)'),
-        ('SP', 'Senior Personnel (SP)'),
-    )
-    role = models.CharField(
-        max_length=10,
-        choices=ROLE_CHOICES,
-    )
-    grant_pi_full_name = models.CharField('Grant PI Full Name', max_length=255, blank=True)
-    funding_agency = models.ForeignKey(GrantFundingAgency, on_delete=models.CASCADE)
-    other_funding_agency = models.CharField(max_length=255, blank=True)
-    other_award_number = models.CharField(max_length=255, blank=True)
-    grant_start = models.DateField('Grant Start Date')
-    grant_end = models.DateField('Grant End Date')
-    percent_credit = models.FloatField(validators=[MaxValueValidator(100)])
-    direct_funding = models.FloatField()
-    total_amount_awarded = models.FloatField()
-    status = models.ForeignKey(GrantStatusChoice, on_delete=models.CASCADE)
+    status = models.CharField(max_length=16, choices=STATUS_CHOICES, default='Active')
     history = HistoricalRecords()
 
-    @property
-    def grant_pi(self):
-        if self.role == 'PI':
-            return '{} {}'.format(self.project.pi.first_name, self.project.pi.last_name)
-        else:
-            return self.grant_pi_full_name
+
+    class Meta:
+        unique_together = ('project', 'unique_id')
 
     def __str__(self):
         return self.title
 
-    class Meta:
-        verbose_name_plural = "Grants"
-
-        permissions = (
-            ("can_view_all_grants", "Can view all grants"),
-        )
+    def display_uid(self):
+        return self.unique_id
```

### Comparing `coldfront-1.1.4/coldfront/core/grant/templates/grant/grant_delete_grants.html` & `coldfront-1.1.5/coldfront/core/grant/templates/grant/grant_delete_grants.html`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/core/grant/templates/grant/grant_report_list.html` & `coldfront-1.1.5/coldfront/core/grant/templates/grant/grant_report_list.html`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/core/grant/tests.py` & `coldfront-1.1.5/coldfront/core/grant/tests.py`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/core/grant/urls.py` & `coldfront-1.1.5/coldfront/core/grant/urls.py`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/core/grant/views.py` & `coldfront-1.1.5/coldfront/core/grant/views.py`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/core/portal/templates/portal/allocation_by_fos.html` & `coldfront-1.1.5/coldfront/core/portal/templates/portal/allocation_by_fos.html`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/core/portal/templates/portal/allocation_summary.html` & `coldfront-1.1.5/coldfront/core/portal/templates/portal/allocation_summary.html`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/core/portal/templates/portal/authorized_home.html` & `coldfront-1.1.5/coldfront/core/portal/templates/portal/authorized_home.html`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/core/portal/templates/portal/carousel.html` & `coldfront-1.1.5/coldfront/core/portal/templates/portal/carousel.html`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/core/portal/templates/portal/center_summary.html` & `coldfront-1.1.5/coldfront/core/portal/templates/portal/center_summary.html`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/core/portal/templates/portal/nonauthorized_home.html` & `coldfront-1.1.5/coldfront/core/portal/templates/portal/nonauthorized_home.html`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/core/portal/utils.py` & `coldfront-1.1.5/coldfront/core/portal/utils.py`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/core/portal/views.py` & `coldfront-1.1.5/coldfront/core/portal/views.py`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/core/project/admin.py` & `coldfront-1.1.5/coldfront/core/project/admin.py`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/core/project/forms.py` & `coldfront-1.1.5/coldfront/core/project/forms.py`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/core/project/management/commands/add_default_project_choices.py` & `coldfront-1.1.5/coldfront/core/project/management/commands/add_default_project_choices.py`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/core/project/migrations/0001_initial.py` & `coldfront-1.1.5/coldfront/core/project/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/core/project/migrations/0003_auto_20221013_1215.py` & `coldfront-1.1.5/coldfront/core/project/migrations/0003_auto_20221013_1215.py`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/core/project/templates/project/add_user_search_results.html` & `coldfront-1.1.5/coldfront/core/project/templates/project/add_user_search_results.html`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/core/project/templates/project/project_add_users.html` & `coldfront-1.1.5/coldfront/core/project/templates/project/project_add_users.html`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/core/project/templates/project/project_archive.html` & `coldfront-1.1.5/coldfront/core/project/templates/project/project_archive.html`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/core/project/templates/project/project_archived_list.html` & `coldfront-1.1.5/coldfront/core/project/templates/project/project_archived_list.html`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/core/project/templates/project/project_attribute_create.html` & `coldfront-1.1.5/coldfront/core/project/templates/project/project_attribute_create.html`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/core/project/templates/project/project_attribute_delete.html` & `coldfront-1.1.5/coldfront/core/project/templates/project/project_attribute_delete.html`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/core/project/templates/project/project_attribute_update.html` & `coldfront-1.1.5/coldfront/core/project/templates/project/project_attribute_update.html`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/core/project/templates/project/project_detail.html` & `coldfront-1.1.5/coldfront/core/project/templates/project/project_detail.html`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/core/project/templates/project/project_list.html` & `coldfront-1.1.5/coldfront/core/project/templates/project/project_list.html`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/core/project/templates/project/project_note_create.html` & `coldfront-1.1.5/coldfront/core/project/templates/project/project_note_create.html`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/core/project/templates/project/project_remove_users.html` & `coldfront-1.1.5/coldfront/core/project/templates/project/project_remove_users.html`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/core/project/templates/project/project_review.html` & `coldfront-1.1.5/coldfront/core/project/templates/project/project_review.html`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/core/project/templates/project/project_review_email.html` & `coldfront-1.1.5/coldfront/core/project/templates/project/project_review_email.html`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/core/project/templates/project/project_review_list.html` & `coldfront-1.1.5/coldfront/core/project/templates/project/project_review_list.html`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/core/project/templates/project/project_user_detail.html` & `coldfront-1.1.5/coldfront/core/project/templates/project/project_user_detail.html`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/core/project/tests.py` & `coldfront-1.1.5/coldfront/core/project/tests.py`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/core/project/urls.py` & `coldfront-1.1.5/coldfront/core/project/urls.py`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/core/project/utils.py` & `coldfront-1.1.5/coldfront/core/project/utils.py`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/core/project/views.py` & `coldfront-1.1.5/coldfront/core/project/views.py`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/core/publication/forms.py` & `coldfront-1.1.5/coldfront/core/publication/forms.py`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/core/publication/migrations/0001_initial.py` & `coldfront-1.1.5/coldfront/core/publication/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/core/publication/migrations/0002_auto_20191223_1115.py` & `coldfront-1.1.5/coldfront/core/publication/migrations/0002_auto_20191223_1115.py`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/core/publication/migrations/0003_auto_20200104_1700.py` & `coldfront-1.1.5/coldfront/core/publication/migrations/0003_auto_20200104_1700.py`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/core/publication/migrations/0004_add_manual_publication_source.py` & `coldfront-1.1.5/coldfront/core/publication/migrations/0004_add_manual_publication_source.py`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/core/publication/templates/publication/publication_add_publication_manually.html` & `coldfront-1.1.5/coldfront/core/publication/templates/publication/publication_add_publication_manually.html`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/core/publication/templates/publication/publication_add_publication_search.html` & `coldfront-1.1.5/coldfront/core/publication/templates/publication/publication_add_publication_search.html`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/core/publication/templates/publication/publication_add_publication_search_result.html` & `coldfront-1.1.5/coldfront/core/publication/templates/publication/publication_add_publication_search_result.html`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/core/publication/templates/publication/publication_delete_publications.html` & `coldfront-1.1.5/coldfront/core/publication/templates/publication/publication_delete_publications.html`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/core/publication/templates/publication/publication_export_publications.html` & `coldfront-1.1.5/coldfront/core/publication/templates/publication/publication_export_publications.html`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/core/publication/tests.py` & `coldfront-1.1.5/coldfront/core/publication/tests.py`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/core/publication/urls.py` & `coldfront-1.1.5/coldfront/core/publication/urls.py`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/core/publication/views.py` & `coldfront-1.1.5/coldfront/core/publication/views.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import ast
 import re
 import uuid
 import requests
 import os
 import io
 from io import StringIO
 from bibtexparser.bibdatabase import as_text
@@ -199,15 +200,15 @@
             messages.error(
                 request, 'You cannot add publications to an archived project.')
             return HttpResponseRedirect(reverse('project-detail', kwargs={'pk': project_obj.pk}))
         else:
             return super().dispatch(request, *args, **kwargs)
 
     def post(self, request, *args, **kwargs):
-        pubs = eval(request.POST.get('pubs'))
+        pubs = ast.literal_eval(request.POST.get('pubs'))
         project_pk = self.kwargs.get('project_pk')
 
         project_obj = get_object_or_404(Project, pk=project_pk)
         formset = formset_factory(PublicationResultForm, max_num=len(pubs))
         formset = formset(request.POST, initial=pubs, prefix='pubform')
 
         publications_added = 0
```

### Comparing `coldfront-1.1.4/coldfront/core/research_output/admin.py` & `coldfront-1.1.5/coldfront/core/research_output/admin.py`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/core/research_output/migrations/0001_initial.py` & `coldfront-1.1.5/coldfront/core/research_output/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/core/research_output/models.py` & `coldfront-1.1.5/coldfront/core/research_output/models.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,14 +4,23 @@
 from model_utils.models import TimeStampedModel
 from simple_history.models import HistoricalRecords
 
 from coldfront.core.project.models import Project
 
 
 class ResearchOutput(TimeStampedModel):
+    """ A research output represents anything related a project that would not fall under the publication section. Examples include magazine or newspaper articles, media coverage, databases, software, or other products created.
+    
+    Attributes:
+        project (Project): links project to research output
+        title (str): title of research output
+        description (str): description of output
+        created_by (User): represents the User model of the user creating the output
+    """
+
     # core fields
     project = models.ForeignKey(Project, on_delete=models.CASCADE)
     title = models.CharField(max_length=128, blank=True)
     description = models.TextField(
         validators=[MinLengthValidator(3)],
     )
 
@@ -24,14 +33,15 @@
     )
 
     # automatic fields
     created = models.DateTimeField(auto_now_add=True, editable=False)
     history = HistoricalRecords()
 
     def save(self, *args, **kwargs):
+        """ Saves the research output. """
         if not self.pk:
             # ensure that created_by is set initially - preventing most
             # accidental omission
             #
             # this field won't be autopopulated by Django and must instead be
             # populated by the code that adds the ResearchOutput to the
             # database
```

### Comparing `coldfront-1.1.4/coldfront/core/research_output/templates/research_output/research_output_delete_research_outputs.html` & `coldfront-1.1.5/coldfront/core/research_output/templates/research_output/research_output_delete_research_outputs.html`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/core/research_output/tests.py` & `coldfront-1.1.5/coldfront/core/research_output/tests.py`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/core/research_output/views.py` & `coldfront-1.1.5/coldfront/core/research_output/views.py`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/core/resource/admin.py` & `coldfront-1.1.5/coldfront/core/resource/admin.py`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/core/resource/forms.py` & `coldfront-1.1.5/coldfront/core/resource/forms.py`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/core/resource/management/commands/add_resource_defaults.py` & `coldfront-1.1.5/coldfront/core/resource/management/commands/add_resource_defaults.py`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/core/resource/migrations/0001_initial.py` & `coldfront-1.1.5/coldfront/core/resource/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/core/resource/migrations/0002_auto_20191017_1141.py` & `coldfront-1.1.5/coldfront/core/resource/migrations/0002_auto_20191017_1141.py`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/core/resource/models.py` & `coldfront-1.1.5/coldfront/core/resource/models.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,80 +4,143 @@
 from django.core.exceptions import ValidationError
 from django.db import models
 from model_utils.models import TimeStampedModel
 from simple_history.models import HistoricalRecords
 import coldfront.core.attribute_expansion as attribute_expansion
 
 class AttributeType(TimeStampedModel):
+    """ An attribute type indicates the data type of the attribute. Examples include Date, Float, Int, Text, and Yes/No. 
+    
+    Attributes:
+        name (str): name of attribute data type
+    """
+
     name = models.CharField(max_length=128, unique=True)
 
     def __str__(self):
         return self.name
 
     class Meta:
         ordering = ['name', ]
 
-
 class ResourceType(TimeStampedModel):
+    """ A resource type class links a resource and its value. 
+    
+    Attributes:
+        name (str): name of resource type
+        description (str): description of resource type
+    """
+    class Meta:
+        ordering = ['name', ]
+
+    class ResourceTypeManager(models.Manager):
+        def get_by_natural_key(self, name):
+            return self.get(name=name)
+
     name = models.CharField(max_length=128, unique=True)
     description = models.CharField(max_length=255)
     history = HistoricalRecords()
+    objects = ResourceTypeManager()
 
     @property
     def active_count(self):
+        """ 
+        Returns:
+            int: the number of active resources of that type
+        """
+
         return ResourceAttribute.objects.filter(
             resource__resource_type__name=self.name, value="Active").count()
 
     @property
     def inactive_count(self):
+        """ 
+        Returns:
+            int: the number of inactive resources of that type
+        """
+
         return ResourceAttribute.objects.filter(
             resource__resource_type__name=self.name, value="Inactive").count()
 
     def __str__(self):
         return self.name
 
-    class Meta:
-        ordering = ['name', ]
-
+    def natural_key(self):
+        return [self.name]
 
 class ResourceAttributeType(TimeStampedModel):
+    """ A resource attribute type indicates the type of the attribute. Examples include slurm_specs and slurm_cluster. 
+    
+    Attributes:
+        attribute_type (AttributeType): indicates the AttributeType of the attribute
+        name (str): name of resource attribute type
+        is_required (bool): indicates whether or not the attribute is required
+        is_value_unique (bool): indicates whether or not the value is unique
+
+    Note: the is_unique_per_resource field is rarely used, hence documentation does not exist.
+    """
+
     attribute_type = models.ForeignKey(AttributeType, on_delete=models.CASCADE)
     name = models.CharField(max_length=128)
     is_required = models.BooleanField(default=False)
     is_unique_per_resource = models.BooleanField(default=False)
     is_value_unique = models.BooleanField(default=False)
     history = HistoricalRecords()
 
     def __str__(self):
         return self.name
 
     class Meta:
         ordering = ['name', ]
 
-
 class Resource(TimeStampedModel):
+    """ A resource is something a center maintains and provides access to for the community. Examples include Budgetstorage, Server, and Software License. 
+    
+    Attributes:
+        parent_resource (Resource): used for the Cluster Partition resource type as these partitions fall under a main cluster
+        resource_type (ResourceType): the type of resource (Cluster, Storage, etc.)
+        name (str): name of resource 
+        description (str): description of what the resource does and is used for 
+        is_available (bool): indicates whether or not the resource is available for users to request an allocation for
+        is_public (bool):  indicates whether or not users can see the resource
+        requires_payment (bool): indicates whether or not users have to pay to use this resource
+        allowed_groups (Group): uses the Django Group model to allow certain user groups to request the resource
+        allowed_users (User): links Django Users that are allowed to request the resource to the resource
+    """
+    class Meta:
+        ordering = ['name', ]
+
+    class ResourceManager(models.Manager):
+        def get_by_natural_key(self, name):
+            return self.get(name=name)
+
     parent_resource = models.ForeignKey(
         'self', on_delete=models.CASCADE, blank=True, null=True)
     resource_type = models.ForeignKey(ResourceType, on_delete=models.CASCADE)
     name = models.CharField(max_length=128, unique=True)
     description = models.TextField()
     is_available = models.BooleanField(default=True)
     is_public = models.BooleanField(default=True)
     is_allocatable = models.BooleanField(default=True)
     requires_payment = models.BooleanField(default=False)
     allowed_groups = models.ManyToManyField(Group, blank=True)
     allowed_users = models.ManyToManyField(User, blank=True)
     linked_resources = models.ManyToManyField('self', blank=True)
     history = HistoricalRecords()
+    objects = ResourceManager()
 
     def get_missing_resource_attributes(self, required=False):
         """
-        if required == True, get only the required missing attributes;
-        otherwise, get required and non-required missing attributes
+        Params:
+            required (bool): indicates whether or not to get only the missing resource attributes that are required (if True, get only required missing attributes; else, get required and non-required missing attributes)
+
+        Returns:
+            list[ResourceAttribute]: a list of resource attributes that do not already exist for this resource
         """
+
         if required:
             resource_attributes = ResourceAttributeType.objects.filter(
                 resource_type=self.resource_type, required=True)
         else:
             resource_attributes = ResourceAttributeType.objects.filter(
                 resource_type=self.resource_type)
 
@@ -86,39 +149,34 @@
         for attribute in resource_attributes:
             if not ResourceAttribute.objects.filter(resource=self, resource_attribute_type=attribute).exists():
                 missing_resource_attributes.append(attribute)
         return missing_resource_attributes
 
     @property
     def status(self):
+        """ 
+        Returns:
+            str: the status of the resource
+        """
+
         return ResourceAttribute.objects.get(resource=self, resource_attribute_type__attribute="Status").value
 
     def get_attribute(self, name, expand=True, typed=True, 
         extra_allocations=[]):
-        """Return the value of the first attribute found with specified name
-
-        This will return the value of the first attribute found for this
-        resource with the specified name.
+        """
+        Params:
+            name (str): name of the resource attribute type
+            expand (bool): indicates whether or not to return the expanded value with attributes/parameters for attributes with a base type of 'Attribute Expanded Text'
+            typed (bool): indicates whether or not to convert the attribute value to an int/ float/ str based on the base AttributeType name
+            extra_allocations (list[Allocation]): allocations which are available to reference in the attribute list in addition to those associated with this ResourceAttribute
 
-        If expand is True (the default), we will return the expanded_value()
-        method of the attribute, which will expand attributes/parameters in
-        the attribute value for attributes with a base type of 'Attribute
-        Expanded Text'.  If the attribute is not of that type, or expand is
-        false, returns the value attribute/data member (i.e. the raw, unexpanded
-        value).
-
-        If extra_allocations is given, it should be a list of Allocations, and
-        when expand=True, the attributes of those Allocations (in addition to
-        attributes of the Resources associated with this ResourceAttribute) are
-        available for referencing in the attribute list.
-
-        If typed is True (the default), we will attempt to convert the value
-        returned to the appropriate python type (int/float/str) based on the
-        base AttributeType name.
+        Returns:
+            str: the value of the first attribute found for this resource with the specified name
         """
+
         attr = self.resourceattribute_set.filter(
             resource_attribute_type__name=name).first()
         if attr:
             if expand:
                 return attr.expanded_value(
                     typed=typed, extra_allocations=extra_allocations)
             else:
@@ -126,69 +184,71 @@
                     return attr.typed_value()
                 else:
                     return attr.value
         return None
 
     def get_attribute_list(self, name, expand=True, typed=True,
         extra_allocations=[]):
-        """Return a list of values of the attributes found with specified name
-
-        This will return a list consisting of the values of the all attributes
-        found for this resource with the specified name.
+        """
+        Params:
+            name (str): name of the resource
+            expand (bool): indicates whether or not to return the expanded value with attributes/parameters for attributes with a base type of 'Attribute Expanded Text'
+            typed (bool): indicates whether or not to convert the attribute value to an int/ float/ str based on the base AttributeType name
+            extra_allocations (list[Allocation]): allocations which are available to reference in the attribute list in addition to those associated with this ResourceAttribute
 
-        If expand is True (the default), we will return the result of the
-        expanded_value() method for each attribute, which will expand
-        attributes/parameters in the attribute value for attributes with a base 
-        type of 'Attribute Expanded Text'.  If the attribute is not of that 
-        type, or expand is false, returns the value attribute/data member (i.e.
-         the raw, unexpanded value).
-
-        If extra_allocations is given, it should be a list of Allocations, and
-        when expand=True, the attributes of those Allocations (in addition to
-        attributes of the Resources associated with this ResourceAttribute) are
-        available for referencing in the attribute list.
-
-        If typed is True (the default), we will attempt to convert the value
-        returned to the appropriate python type (int/float/str) based on the
-        base AttributeType name.
+        Returns:
+            list: the list of values of the attributes found with specified name
         """
+
         attr = self.resourceattribute_set.filter(
             resource_attribute_type__name=name).all()
         if expand:
             return [a.expanded_value(extra_allocations=extra_allocations,
                 typed=typed) for a in attr]
         else:
             if typed:
                 return [a.typed_value() for a in attr]
             else:
                 return [a.value for a in attr]
 
     def get_ondemand_status(self):
+        """
+        Returns:
+            str: If the resource has OnDemand status or not
+        """
+
         ondemand = self.resourceattribute_set.filter(
             resource_attribute_type__name='OnDemand').first()
         if ondemand:
             return ondemand.value
         return None
             
     def __str__(self):
         return '%s (%s)' % (self.name, self.resource_type.name)
 
-    class Meta:
-        ordering = ['name', ]
-
+    def natural_key(self):
+        return [self.name]
 
 class ResourceAttribute(TimeStampedModel):
+    """ A resource attribute class links a resource attribute type and a resource. 
+    
+    Attributes:
+        resource_attribute_type (ResourceAttributeType): resource attribute type to link
+        resource (Resource): resource to link
+        value (str): value of the resource attribute
+    """
+
     resource_attribute_type = models.ForeignKey(
         ResourceAttributeType, on_delete=models.CASCADE)
     resource = models.ForeignKey(Resource, on_delete=models.CASCADE)
     value = models.TextField()
     history = HistoricalRecords()
 
     def clean(self):
-
+        """ Validates the resource and raises errors if the resource is invalid. """
         expected_value_type = self.resource_attribute_type.attribute_type.name.strip()
 
         if expected_value_type == "Int" and not self.value.isdigit():
             raise ValidationError(
                 'Invalid Value "%s". Value must be an integer.' % (self.value))
         elif expected_value_type == "Active/Inactive" and self.value not in ["Active", "Inactive"]:
             raise ValidationError(
@@ -203,54 +263,38 @@
                 raise ValidationError(
                     'Invalid Value "%s". Date must be in format MM/DD/YYYY' % (self.value))
 
     def __str__(self):
         return '%s: %s (%s)' % (self.resource_attribute_type, self.value, self.resource)
 
     def typed_value(self):
-        """Returns the value of the attribute, with proper type.
-
-        For attributes with Int or Float types, we return the value of
-        the attribute coerced into an Int or Float.  If the coercion
-        fails, we log a warning and return the string.
-
-        For all other attribute types, we return the value as a string.
-
-        This is needed when computing values for expanded_value()
         """
+        Returns:
+            int, float, str: the value of the attribute with proper type and is used for computing expanded_value() (coerced into int or float for attributes with Int or Float types; if it fails or the attribute is of any other type, it is coerced into a str)
+        """
+
         raw_value = self.value
         atype_name = self.resource_attribute_type.attribute_type.name
         return attribute_expansion.convert_type(
             value=raw_value, type_name=atype_name)
 
     def expanded_value(self, typed=True, extra_allocations=[]):
-        """Returns the value of the attribute, after attribute expansion.
+        """
+        Params:
+            typed (bool): indicates whether or not to convert the attribute value to an int/ float/ str based on the base AttributeType name (unrecognized values not converted, so will return str)
+            extra_allocations (list[Allocation]): allocations which are available to reference in the attribute list in addition to those associated with this ResourceAttribute
+
+        Returns:
+            int, float, str: the value of the attribute after attribute expansion
+
+        For attributes with attribute type of 'Attribute Expanded Text' we look for an attribute with same name suffixed with '_attriblist' (this should be ResourceAttribute of the Resource associated with the attribute). If the attriblist attribute is found, we use it to generate a dictionary to use to expand the attribute value, and the expanded value is returned.  
 
-        For attributes with attribute type of  'Attribute Expanded Text' we
-        look for an attribute with same name suffixed with '_attriblist' (this
-        should be ResourceAttribute of the Resource associated with the
-        attribute).
-        If the attriblist attribute is found, we use
-        it to generate a dictionary to use to expand the attribute value,
-        and the expanded value is returned.  
-
-        If extra_allocations is given, it should be a list of Allocations, and
-        the attributes of these allocations will be available for referencing
-        in the attriblist (in addition to attributes of the Resource associated
-        with this ResourceAttribute).
-
-        If typed is True (the default), we use typed to convert the returned
-        value to the expected (int, float, str) python data type according to
-        the AttributeType of the AllocationAttributeType (unrecognized values
-        not converted, so will return str).
-
-        If the expansion fails, or if no attriblist attribute is found, or if
-        the attribute type is not 'Attribute Expanded Text', we just return
-        the raw value.
+        If the expansion fails, or if no attriblist attribute is found, or if the attribute type is not 'Attribute Expanded Text', we just return the raw value.
         """
+        
         raw_value = self.value
         if typed:
             # Try to convert to python type as per AttributeType
             raw_value = self.typed_value()
 
         if not attribute_expansion.is_expandable_type(
             self.resource_attribute_type.attribute_type):
```

### Comparing `coldfront-1.1.4/coldfront/core/resource/templates/resource_detail.html` & `coldfront-1.1.5/coldfront/core/resource/templates/resource_detail.html`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/core/resource/templates/resource_list.html` & `coldfront-1.1.5/coldfront/core/resource/templates/resource_list.html`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/core/resource/templates/resource_resourceattribute_delete.html` & `coldfront-1.1.5/coldfront/core/resource/templates/resource_resourceattribute_delete.html`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/core/resource/urls.py` & `coldfront-1.1.5/coldfront/core/resource/urls.py`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/core/resource/views.py` & `coldfront-1.1.5/coldfront/core/resource/views.py`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/core/user/admin.py` & `coldfront-1.1.5/coldfront/core/user/admin.py`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/core/user/forms.py` & `coldfront-1.1.5/coldfront/core/user/forms.py`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/core/user/migrations/0001_initial.py` & `coldfront-1.1.5/coldfront/core/user/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/core/user/signals.py` & `coldfront-1.1.5/coldfront/core/user/signals.py`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/core/user/templates/user/login.html` & `coldfront-1.1.5/coldfront/core/user/templates/user/login.html`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/core/user/templates/user/user_list_allocations.html` & `coldfront-1.1.5/coldfront/core/user/templates/user/user_list_allocations.html`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/core/user/templates/user/user_profile.html` & `coldfront-1.1.5/coldfront/core/user/templates/user/user_profile.html`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/core/user/templates/user/user_projects_managers.html` & `coldfront-1.1.5/coldfront/core/user/templates/user/user_projects_managers.html`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/core/user/templates/user/user_search_home.html` & `coldfront-1.1.5/coldfront/core/user/templates/user/user_search_home.html`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/core/user/templates/user/user_search_results.html` & `coldfront-1.1.5/coldfront/core/user/templates/user/user_search_results.html`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/core/user/tests.py` & `coldfront-1.1.5/coldfront/core/user/tests.py`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/core/user/urls.py` & `coldfront-1.1.5/coldfront/core/user/urls.py`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/core/user/utils.py` & `coldfront-1.1.5/coldfront/core/user/utils.py`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/core/user/views.py` & `coldfront-1.1.5/coldfront/core/user/views.py`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/core/utils/common.py` & `coldfront-1.1.5/coldfront/core/utils/common.py`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/core/utils/mail.py` & `coldfront-1.1.5/coldfront/core/utils/mail.py`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/core/utils/management/commands/add_scheduled_tasks.py` & `coldfront-1.1.5/coldfront/core/utils/management/commands/add_scheduled_tasks.py`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/core/utils/management/commands/initial_setup.py` & `coldfront-1.1.5/coldfront/core/utils/management/commands/initial_setup.py`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/core/utils/management/commands/load_test_data.py` & `coldfront-1.1.5/coldfront/core/utils/management/commands/load_test_data.py`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/core/utils/management/commands/show_users_in_project_but_not_in_allocation.py` & `coldfront-1.1.5/coldfront/core/utils/management/commands/show_users_in_project_but_not_in_allocation.py`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/core/utils/mixins/views.py` & `coldfront-1.1.5/coldfront/core/utils/mixins/views.py`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/core/utils/templatetags/common_tags.py` & `coldfront-1.1.5/coldfront/core/utils/templatetags/common_tags.py`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/core/utils/validate.py` & `coldfront-1.1.5/coldfront/core/utils/validate.py`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/plugins/freeipa/management/commands/freeipa_check.py` & `coldfront-1.1.5/coldfront/plugins/freeipa/management/commands/freeipa_check.py`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/plugins/freeipa/management/commands/freeipa_expire_users.py` & `coldfront-1.1.5/coldfront/plugins/freeipa/management/commands/freeipa_expire_users.py`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/plugins/freeipa/search.py` & `coldfront-1.1.5/coldfront/plugins/freeipa/search.py`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/plugins/freeipa/signals.py` & `coldfront-1.1.5/coldfront/plugins/freeipa/signals.py`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/plugins/freeipa/tasks.py` & `coldfront-1.1.5/coldfront/plugins/freeipa/tasks.py`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/plugins/freeipa/utils.py` & `coldfront-1.1.5/coldfront/plugins/freeipa/utils.py`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/plugins/iquota/templates/iquota/iquota.html` & `coldfront-1.1.5/coldfront/plugins/iquota/templates/iquota/iquota.html`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/plugins/iquota/templates/iquota/iquota_div.html` & `coldfront-1.1.5/coldfront/plugins/iquota/templates/iquota/iquota_div.html`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/plugins/iquota/utils.py` & `coldfront-1.1.5/coldfront/plugins/iquota/utils.py`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/plugins/iquota/views.py` & `coldfront-1.1.5/coldfront/plugins/iquota/views.py`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/plugins/ldap_user_search/utils.py` & `coldfront-1.1.5/coldfront/plugins/ldap_user_search/utils.py`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/plugins/mokey_oidc/auth.py` & `coldfront-1.1.5/coldfront/plugins/mokey_oidc/auth.py`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/plugins/slurm/associations.py` & `coldfront-1.1.5/coldfront/plugins/slurm/associations.py`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/plugins/slurm/management/commands/slurm_check.py` & `coldfront-1.1.5/coldfront/plugins/slurm/management/commands/slurm_check.py`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/plugins/slurm/management/commands/slurm_dump.py` & `coldfront-1.1.5/coldfront/plugins/slurm/management/commands/slurm_dump.py`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/plugins/slurm/utils.py` & `coldfront-1.1.5/coldfront/plugins/slurm/utils.py`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/plugins/system_monitor/templates/system_monitor/system_monitor_div.html` & `coldfront-1.1.5/coldfront/plugins/system_monitor/templates/system_monitor/system_monitor_div.html`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/plugins/system_monitor/utils.py` & `coldfront-1.1.5/coldfront/plugins/system_monitor/utils.py`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/plugins/xdmod/management/commands/xdmod_usage.py` & `coldfront-1.1.5/coldfront/plugins/xdmod/management/commands/xdmod_usage.py`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/plugins/xdmod/utils.py` & `coldfront-1.1.5/coldfront/plugins/xdmod/utils.py`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/static/bootstrap/bootstrap.bundle.min.js` & `coldfront-1.1.5/coldfront/static/bootstrap/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/static/bootstrap/bootstrap.bundle.min.js.map` & `coldfront-1.1.5/coldfront/static/bootstrap/bootstrap.bundle.min.js.map`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/static/bootstrap/bootstrap.min.css` & `coldfront-1.1.5/coldfront/static/bootstrap/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/static/bootstrap/bootstrap.min.css.map` & `coldfront-1.1.5/coldfront/static/bootstrap/bootstrap.min.css.map`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/static/c3js/c3.min.css` & `coldfront-1.1.5/coldfront/static/c3js/c3.min.css`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/static/c3js/c3.min.js` & `coldfront-1.1.5/coldfront/static/c3js/c3.min.js`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/static/coldfront/plugins/system_monitor/images/xdmod.png` & `coldfront-1.1.5/coldfront/static/coldfront/plugins/system_monitor/images/xdmod.png`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/static/common/css/common.css` & `coldfront-1.1.5/coldfront/static/common/css/common.css`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/static/common/images/android-chrome-192x192.png` & `coldfront-1.1.5/coldfront/static/common/images/android-chrome-192x192.png`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/static/common/images/android-chrome-512x512.png` & `coldfront-1.1.5/coldfront/static/common/images/android-chrome-512x512.png`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/static/common/images/apple-touch-icon.png` & `coldfront-1.1.5/coldfront/static/common/images/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/static/common/images/favicon-16x16.png` & `coldfront-1.1.5/coldfront/static/common/images/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/static/common/images/favicon-32x32.png` & `coldfront-1.1.5/coldfront/static/common/images/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/static/common/images/favicon.ico` & `coldfront-1.1.5/coldfront/static/common/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/static/common/images/logo.png` & `coldfront-1.1.5/coldfront/static/common/images/logo.png`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/static/core/portal/imgs/airport-business-cabinets-236093.jpg` & `coldfront-1.1.5/coldfront/static/core/portal/imgs/airport-business-cabinets-236093.jpg`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/static/core/portal/imgs/analogue-blur-business-159282.jpg` & `coldfront-1.1.5/coldfront/static/core/portal/imgs/analogue-blur-business-159282.jpg`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/static/core/portal/imgs/computer-electronics-equipment-325223.jpg` & `coldfront-1.1.5/coldfront/static/core/portal/imgs/computer-electronics-equipment-325223.jpg`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/static/core/portal/imgs/ondemand.png` & `coldfront-1.1.5/coldfront/static/core/portal/imgs/ondemand.png`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/static/d3/d3.v5.min.js` & `coldfront-1.1.5/coldfront/static/d3/d3.v5.min.js`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/static/datatable/dataTables.bootstrap4.min.css` & `coldfront-1.1.5/coldfront/static/datatable/dataTables.bootstrap4.min.css`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/static/datatable/dataTables.bootstrap4.min.js` & `coldfront-1.1.5/coldfront/static/datatable/dataTables.bootstrap4.min.js`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/static/datatable/jquery.dataTables.min.js` & `coldfront-1.1.5/coldfront/static/datatable/jquery.dataTables.min.js`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/static/flatpickr/flatpickr.js` & `coldfront-1.1.5/coldfront/static/flatpickr/flatpickr.js`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/static/flatpickr/flatpickr.min.css` & `coldfront-1.1.5/coldfront/static/flatpickr/flatpickr.min.css`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/static/jquery/jquery-3.6.0.min.js` & `coldfront-1.1.5/coldfront/static/jquery/jquery-3.6.0.min.js`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/static/select2/select2.min.css` & `coldfront-1.1.5/coldfront/static/select2/select2.min.css`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/static/select2/select2.min.js` & `coldfront-1.1.5/coldfront/static/select2/select2.min.js`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/templates/common/authorized_navbar.html` & `coldfront-1.1.5/coldfront/templates/common/authorized_navbar.html`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/templates/common/base.html` & `coldfront-1.1.5/coldfront/templates/common/base.html`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/templates/common/navbar_admin.html` & `coldfront-1.1.5/coldfront/templates/common/navbar_admin.html`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/templates/common/navbar_director.html` & `coldfront-1.1.5/coldfront/templates/common/navbar_director.html`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/templates/common/navbar_login.html` & `coldfront-1.1.5/coldfront/templates/common/navbar_login.html`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/templates/common/navbar_nonadmin_staff.html` & `coldfront-1.1.5/coldfront/templates/common/navbar_nonadmin_staff.html`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/templates/common/nonauthorized_navbar.html` & `coldfront-1.1.5/coldfront/templates/common/nonauthorized_navbar.html`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/templates/email/admin_allocation_expired.txt` & `coldfront-1.1.5/coldfront/templates/email/admin_allocation_expired.txt`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/templates/email/allocation_expired.txt` & `coldfront-1.1.5/coldfront/templates/email/allocation_expired.txt`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront/templates/email/allocation_expiring.txt` & `coldfront-1.1.5/coldfront/templates/email/allocation_expiring.txt`

 * *Files identical despite different names*

### Comparing `coldfront-1.1.4/coldfront.egg-info/PKG-INFO` & `coldfront-1.1.5/coldfront.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coldfront
-Version: 1.1.4
+Version: 1.1.5
 Summary: HPC Resource Allocation System 
 Home-page: http://coldfront.io
 Author: Andrew E. Bruno, Dori Sajdak, Mohammad Zia
 License: GNU General Public License v3 (GPLv3)
 Project-URL: Bug Tracker, https://github.com/ubccr/coldfront/issues
 Project-URL: Documentation, https://coldfront.readthedocs.io
 Project-URL: Source Code, https://github.com/ubccr/coldfront
@@ -22,29 +22,30 @@
 
 ![ColdFront](docs/pages/images/logo-lg.png)
 
 # ColdFront - Resource Allocation System
 
 [![Documentation Status](https://readthedocs.org/projects/coldfront/badge/?version=latest)](https://coldfront.readthedocs.io/en/latest/?badge=latest)
 
-ColdFront is an open source resource allocation system designed to provide a
+ColdFront is an open source resource and allocation management system designed to provide a
 central portal for administration, reporting, and measuring scientific impact
-of HPC resources. ColdFront was created to help HPC centers manage access to a
-diverse set of resources across large groups of users and provide a rich set of
-extensible meta data for comprehensive reporting. ColdFront is written in
-Python and released under the GPLv3 license.
+of cyberinfrastructure resources. ColdFront was created to help high performance computing (HPC) centers manage access to a diverse set of resources across large groups of users and provide a rich set of
+extensible meta data for comprehensive reporting. The flexiblity of ColdFront allows centers to manage and automate their policies and procedures within the framework provided or extend the functionality with [plugins](docs/pages/index.md#extensibility).  ColdFront is written in Python and released under the GPLv3 license.
 
 ## Features
 
 - Allocation based system for managing access to resources
-- Collect Project, Grant, and Publication data from users
-- Define custom attributes on resources and allocations
+- Self-service portal for users to request access to resources for their research group
+- Collection of Project, Grant, and Publication data from users
+- Center director approval system and annual project review process
 - Email notifications for expiring/renewing access to resources
-- Integration with 3rd party systems for automation and access control
-- Center director approval system and annual project reviews
+- Ability to define custom attributes on resources and allocations 
+- Integration with 3rd party systems for automation, access control, and other system provisioning tasks
+
+[Read more](docs/pages/index.md)  
 
 ## Community Supported Plugins
 
 - [OpenStack Plugin](https://github.com/nerc-project/coldfront-plugin-openstack)
 - [Keycloak User Search](https://github.com/nerc-project/coldfront-plugin-keycloak)
 - [Starfish Plugin](https://github.com/fasrc/sftocf)
```

### Comparing `coldfront-1.1.4/coldfront.egg-info/SOURCES.txt` & `coldfront-1.1.5/coldfront.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -81,27 +81,29 @@
 coldfront/core/field_of_science/tests.py
 coldfront/core/field_of_science/views.py
 coldfront/core/field_of_science/management/__init__.py
 coldfront/core/field_of_science/management/commands/__init__.py
 coldfront/core/field_of_science/management/commands/import_field_of_science_data.py
 coldfront/core/field_of_science/management/commands/data/field_of_science_data.csv
 coldfront/core/field_of_science/migrations/0001_initial.py
+coldfront/core/field_of_science/migrations/0002_alter_fieldofscience_description.py
 coldfront/core/field_of_science/migrations/__init__.py
 coldfront/core/grant/__init__.py
 coldfront/core/grant/admin.py
 coldfront/core/grant/apps.py
 coldfront/core/grant/forms.py
 coldfront/core/grant/models.py
 coldfront/core/grant/tests.py
 coldfront/core/grant/urls.py
 coldfront/core/grant/views.py
 coldfront/core/grant/management/__init__.py
 coldfront/core/grant/management/commands/__init__.py
 coldfront/core/grant/management/commands/add_default_grant_options.py
 coldfront/core/grant/migrations/0001_initial.py
+coldfront/core/grant/migrations/0002_auto_20230406_1310.py
 coldfront/core/grant/migrations/__init__.py
 coldfront/core/grant/templates/grant/grant_create.html
 coldfront/core/grant/templates/grant/grant_delete_grants.html
 coldfront/core/grant/templates/grant/grant_report_list.html
 coldfront/core/grant/templates/grant/grant_update_form.html
 coldfront/core/portal/__init__.py
 coldfront/core/portal/admin.py
@@ -131,14 +133,15 @@
 coldfront/core/project/views.py
 coldfront/core/project/management/__init__.py
 coldfront/core/project/management/commands/__init__.py
 coldfront/core/project/management/commands/add_default_project_choices.py
 coldfront/core/project/migrations/0001_initial.py
 coldfront/core/project/migrations/0002_projectusermessage_is_private.py
 coldfront/core/project/migrations/0003_auto_20221013_1215.py
+coldfront/core/project/migrations/0004_auto_20230406_1133.py
 coldfront/core/project/migrations/__init__.py
 coldfront/core/project/templates/project/add_user_search_results.html
 coldfront/core/project/templates/project/project_add_users.html
 coldfront/core/project/templates/project/project_archive.html
 coldfront/core/project/templates/project/project_archived_list.html
 coldfront/core/project/templates/project/project_attribute_create.html
 coldfront/core/project/templates/project/project_attribute_delete.html
@@ -165,14 +168,15 @@
 coldfront/core/publication/management/commands/__init__.py
 coldfront/core/publication/management/commands/add_default_publication_sources.py
 coldfront/core/publication/migrations/0001_initial.py
 coldfront/core/publication/migrations/0002_auto_20191223_1115.py
 coldfront/core/publication/migrations/0003_auto_20200104_1700.py
 coldfront/core/publication/migrations/0004_add_manual_publication_source.py
 coldfront/core/publication/migrations/__init__.py
+coldfront/core/publication/templates/publication/.publication_add_publication_search_result.html.swp
 coldfront/core/publication/templates/publication/publication_add_publication_manually.html
 coldfront/core/publication/templates/publication/publication_add_publication_search.html
 coldfront/core/publication/templates/publication/publication_add_publication_search_result.html
 coldfront/core/publication/templates/publication/publication_delete_publications.html
 coldfront/core/publication/templates/publication/publication_export_publications.html
 coldfront/core/research_output/__init__.py
 coldfront/core/research_output/admin.py
@@ -232,21 +236,14 @@
 coldfront/core/utils/tests.py
 coldfront/core/utils/validate.py
 coldfront/core/utils/views.py
 coldfront/core/utils/fixtures/__init__.py
 coldfront/core/utils/management/__init__.py
 coldfront/core/utils/management/commands/__init__.py
 coldfront/core/utils/management/commands/add_scheduled_tasks.py
-coldfront/core/utils/management/commands/import_grants.py
-coldfront/core/utils/management/commands/import_projects.py
-coldfront/core/utils/management/commands/import_publications.py
-coldfront/core/utils/management/commands/import_resources.py
-coldfront/core/utils/management/commands/import_resources_from_json.py
-coldfront/core/utils/management/commands/import_subscriptions.py
-coldfront/core/utils/management/commands/import_users.py
 coldfront/core/utils/management/commands/initial_setup.py
 coldfront/core/utils/management/commands/load_test_data.py
 coldfront/core/utils/management/commands/show_users_in_project_but_not_in_allocation.py
 coldfront/core/utils/migrations/__init__.py
 coldfront/core/utils/mixins/__init__.py
 coldfront/core/utils/mixins/views.py
 coldfront/core/utils/templatetags/__init__.py
```

### Comparing `coldfront-1.1.4/coldfront.egg-info/requires.txt` & `coldfront-1.1.5/coldfront.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 arrow==1.2.3
 bibtexparser==1.4.0
 blessed==1.20.0
 chardet==5.1.0
-Django==3.2.17
+Django==3.2.20
 django-crispy-forms==1.14.0
 Faker==11.3.0
 fontawesome-free==5.15.4
 django-environ==0.9.0
 django-model-utils==4.3.1
 django-picklefield==3.1
 django-q==1.3.9
```

### Comparing `coldfront-1.1.4/setup.py` & `coldfront-1.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     python_requires='>=3.6',
     packages=find_packages(),
     install_requires=[
         'arrow==1.2.3',
         'bibtexparser==1.4.0',
         'blessed==1.20.0',
         'chardet==5.1.0',
-        'Django==3.2.17',
+        'Django==3.2.20',
         'django-crispy-forms==1.14.0',
         'Faker==11.3.0',
         'fontawesome-free==5.15.4',
         'django-environ==0.9.0',
         'django-model-utils==4.3.1',
         'django-picklefield==3.1',
         'django-q==1.3.9',
```

