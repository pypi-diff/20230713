# Comparing `tmp/django-toosimple-q-1.0.0b4.tar.gz` & `tmp/django-toosimple-q-1.0.0b5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-toosimple-q-1.0.0b4.tar", last modified: Wed Jul 12 21:37:06 2023, max compression
+gzip compressed data, was "dist/django-toosimple-q-1.0.0b5.tar", last modified: Thu Jul 13 20:01:51 2023, max compression
```

## Comparing `django-toosimple-q-1.0.0b4.tar` & `django-toosimple-q-1.0.0b5.tar`

### file list

```diff
@@ -1,74 +1,76 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:37:06.000000 django-toosimple-q-1.0.0b4/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-12 21:36:51.000000 django-toosimple-q-1.0.0b4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    16724 2023-07-12 21:37:06.000000 django-toosimple-q-1.0.0b4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12821 2023-07-12 21:36:51.000000 django-toosimple-q-1.0.0b4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:37:06.000000 django-toosimple-q-1.0.0b4/django_toosimple_q/
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-12 21:37:05.000000 django-toosimple-q-1.0.0b4/django_toosimple_q/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6897 2023-07-12 21:36:51.000000 django-toosimple-q-1.0.0b4/django_toosimple_q/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-07-12 21:36:51.000000 django-toosimple-q-1.0.0b4/django_toosimple_q/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:37:06.000000 django-toosimple-q-1.0.0b4/django_toosimple_q/contrib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 21:36:51.000000 django-toosimple-q-1.0.0b4/django_toosimple_q/contrib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:37:06.000000 django-toosimple-q-1.0.0b4/django_toosimple_q/contrib/mail/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 21:36:51.000000 django-toosimple-q-1.0.0b4/django_toosimple_q/contrib/mail/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-12 21:36:51.000000 django-toosimple-q-1.0.0b4/django_toosimple_q/contrib/mail/backend.py
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-07-12 21:36:51.000000 django-toosimple-q-1.0.0b4/django_toosimple_q/contrib/mail/tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     4738 2023-07-12 21:36:51.000000 django-toosimple-q-1.0.0b4/django_toosimple_q/contrib/mail/tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-07-12 21:36:51.000000 django-toosimple-q-1.0.0b4/django_toosimple_q/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-07-12 21:36:51.000000 django-toosimple-q-1.0.0b4/django_toosimple_q/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:37:06.000000 django-toosimple-q-1.0.0b4/django_toosimple_q/management/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 21:36:51.000000 django-toosimple-q-1.0.0b4/django_toosimple_q/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:37:06.000000 django-toosimple-q-1.0.0b4/django_toosimple_q/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 21:36:51.000000 django-toosimple-q-1.0.0b4/django_toosimple_q/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12289 2023-07-12 21:36:51.000000 django-toosimple-q-1.0.0b4/django_toosimple_q/management/commands/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:37:06.000000 django-toosimple-q-1.0.0b4/django_toosimple_q/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     3887 2023-07-12 21:36:51.000000 django-toosimple-q-1.0.0b4/django_toosimple_q/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-07-12 21:36:51.000000 django-toosimple-q-1.0.0b4/django_toosimple_q/migrations/0002_auto_20191101_1838.py
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-07-12 21:36:51.000000 django-toosimple-q-1.0.0b4/django_toosimple_q/migrations/0003_task_queue.py
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-07-12 21:36:51.000000 django-toosimple-q-1.0.0b4/django_toosimple_q/migrations/0004_auto_20200507_1339.py
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-07-12 21:36:51.000000 django-toosimple-q-1.0.0b4/django_toosimple_q/migrations/0005_auto_20210302_1748.py
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-12 21:36:51.000000 django-toosimple-q-1.0.0b4/django_toosimple_q/migrations/0006_task_replacement.py
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-07-12 21:36:51.000000 django-toosimple-q-1.0.0b4/django_toosimple_q/migrations/0007_schedule_datetime_kwarg.py
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-07-12 21:36:51.000000 django-toosimple-q-1.0.0b4/django_toosimple_q/migrations/0008_auto_20210902_2111.py
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-07-12 21:36:51.000000 django-toosimple-q-1.0.0b4/django_toosimple_q/migrations/0009_auto_20210902_2245.py
--rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-07-12 21:36:51.000000 django-toosimple-q-1.0.0b4/django_toosimple_q/migrations/0010_auto_20220324_0419.py
--rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-07-12 21:36:51.000000 django-toosimple-q-1.0.0b4/django_toosimple_q/migrations/0011_workerstatus.py
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-12 21:36:51.000000 django-toosimple-q-1.0.0b4/django_toosimple_q/migrations/0012_rename_last_run_scheduleexec_last_task.py
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-12 21:36:51.000000 django-toosimple-q-1.0.0b4/django_toosimple_q/migrations/0013_workerstatus_exit_code_workerstatus_exit_log.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 21:36:51.000000 django-toosimple-q-1.0.0b4/django_toosimple_q/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10084 2023-07-12 21:36:51.000000 django-toosimple-q-1.0.0b4/django_toosimple_q/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-07-12 21:36:51.000000 django-toosimple-q-1.0.0b4/django_toosimple_q/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-07-12 21:36:51.000000 django-toosimple-q-1.0.0b4/django_toosimple_q/schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)     2649 2023-07-12 21:36:51.000000 django-toosimple-q-1.0.0b4/django_toosimple_q/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:37:06.000000 django-toosimple-q-1.0.0b4/django_toosimple_q/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:37:06.000000 django-toosimple-q-1.0.0b4/django_toosimple_q/templates/toosimpleq/
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-12 21:36:51.000000 django-toosimple-q-1.0.0b4/django_toosimple_q/templates/toosimpleq/schedule.html
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-12 21:36:51.000000 django-toosimple-q-1.0.0b4/django_toosimple_q/templates/toosimpleq/task.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:37:06.000000 django-toosimple-q-1.0.0b4/django_toosimple_q/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 21:36:51.000000 django-toosimple-q-1.0.0b4/django_toosimple_q/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8448 2023-07-12 21:36:51.000000 django-toosimple-q-1.0.0b4/django_toosimple_q/tests/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:37:06.000000 django-toosimple-q-1.0.0b4/django_toosimple_q/tests/concurrency/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 21:36:51.000000 django-toosimple-q-1.0.0b4/django_toosimple_q/tests/concurrency/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-12 21:36:51.000000 django-toosimple-q-1.0.0b4/django_toosimple_q/tests/concurrency/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:37:06.000000 django-toosimple-q-1.0.0b4/django_toosimple_q/tests/demo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 21:36:51.000000 django-toosimple-q-1.0.0b4/django_toosimple_q/tests/demo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-07-12 21:36:51.000000 django-toosimple-q-1.0.0b4/django_toosimple_q/tests/demo/tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-07-12 21:36:51.000000 django-toosimple-q-1.0.0b4/django_toosimple_q/tests/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-12 21:36:51.000000 django-toosimple-q-1.0.0b4/django_toosimple_q/tests/settings_bg.py
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-07-12 21:36:51.000000 django-toosimple-q-1.0.0b4/django_toosimple_q/tests/settings_bg_lag.py
--rw-r--r--   0 runner    (1001) docker     (123)     2409 2023-07-12 21:36:51.000000 django-toosimple-q-1.0.0b4/django_toosimple_q/tests/tests_admin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3815 2023-07-12 21:36:51.000000 django-toosimple-q-1.0.0b4/django_toosimple_q/tests/tests_concurrency.py
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-07-12 21:36:51.000000 django-toosimple-q-1.0.0b4/django_toosimple_q/tests/tests_regression.py
--rw-r--r--   0 runner    (1001) docker     (123)     9711 2023-07-12 21:36:51.000000 django-toosimple-q-1.0.0b4/django_toosimple_q/tests/tests_schedules.py
--rw-r--r--   0 runner    (1001) docker     (123)    26230 2023-07-12 21:36:51.000000 django-toosimple-q-1.0.0b4/django_toosimple_q/tests/tests_tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     9100 2023-07-12 21:36:51.000000 django-toosimple-q-1.0.0b4/django_toosimple_q/tests/tests_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-07-12 21:36:51.000000 django-toosimple-q-1.0.0b4/django_toosimple_q/tests/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-07-12 21:36:51.000000 django-toosimple-q-1.0.0b4/django_toosimple_q/tests/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:37:06.000000 django-toosimple-q-1.0.0b4/django_toosimple_q.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16724 2023-07-12 21:37:06.000000 django-toosimple-q-1.0.0b4/django_toosimple_q.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-07-12 21:37:06.000000 django-toosimple-q-1.0.0b4/django_toosimple_q.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 21:37:06.000000 django-toosimple-q-1.0.0b4/django_toosimple_q.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 21:37:06.000000 django-toosimple-q-1.0.0b4/django_toosimple_q.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-12 21:37:06.000000 django-toosimple-q-1.0.0b4/django_toosimple_q.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-12 21:37:06.000000 django-toosimple-q-1.0.0b4/django_toosimple_q.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 21:37:06.000000 django-toosimple-q-1.0.0b4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-07-12 21:36:51.000000 django-toosimple-q-1.0.0b4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:01:51.000000 django-toosimple-q-1.0.0b5/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-13 20:01:40.000000 django-toosimple-q-1.0.0b5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    16724 2023-07-13 20:01:51.000000 django-toosimple-q-1.0.0b5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12821 2023-07-13 20:01:40.000000 django-toosimple-q-1.0.0b5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:01:51.000000 django-toosimple-q-1.0.0b5/django_toosimple_q/
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-13 20:01:50.000000 django-toosimple-q-1.0.0b5/django_toosimple_q/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6897 2023-07-13 20:01:40.000000 django-toosimple-q-1.0.0b5/django_toosimple_q/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-07-13 20:01:40.000000 django-toosimple-q-1.0.0b5/django_toosimple_q/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:01:51.000000 django-toosimple-q-1.0.0b5/django_toosimple_q/contrib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 20:01:40.000000 django-toosimple-q-1.0.0b5/django_toosimple_q/contrib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:01:51.000000 django-toosimple-q-1.0.0b5/django_toosimple_q/contrib/mail/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 20:01:40.000000 django-toosimple-q-1.0.0b5/django_toosimple_q/contrib/mail/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-13 20:01:40.000000 django-toosimple-q-1.0.0b5/django_toosimple_q/contrib/mail/backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-07-13 20:01:40.000000 django-toosimple-q-1.0.0b5/django_toosimple_q/contrib/mail/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4738 2023-07-13 20:01:40.000000 django-toosimple-q-1.0.0b5/django_toosimple_q/contrib/mail/tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-07-13 20:01:40.000000 django-toosimple-q-1.0.0b5/django_toosimple_q/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-07-13 20:01:40.000000 django-toosimple-q-1.0.0b5/django_toosimple_q/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:01:51.000000 django-toosimple-q-1.0.0b5/django_toosimple_q/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 20:01:40.000000 django-toosimple-q-1.0.0b5/django_toosimple_q/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:01:51.000000 django-toosimple-q-1.0.0b5/django_toosimple_q/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 20:01:40.000000 django-toosimple-q-1.0.0b5/django_toosimple_q/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12289 2023-07-13 20:01:40.000000 django-toosimple-q-1.0.0b5/django_toosimple_q/management/commands/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:01:51.000000 django-toosimple-q-1.0.0b5/django_toosimple_q/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     3887 2023-07-13 20:01:40.000000 django-toosimple-q-1.0.0b5/django_toosimple_q/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-07-13 20:01:40.000000 django-toosimple-q-1.0.0b5/django_toosimple_q/migrations/0002_auto_20191101_1838.py
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-07-13 20:01:40.000000 django-toosimple-q-1.0.0b5/django_toosimple_q/migrations/0003_task_queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-07-13 20:01:40.000000 django-toosimple-q-1.0.0b5/django_toosimple_q/migrations/0004_auto_20200507_1339.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-07-13 20:01:40.000000 django-toosimple-q-1.0.0b5/django_toosimple_q/migrations/0005_auto_20210302_1748.py
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-13 20:01:40.000000 django-toosimple-q-1.0.0b5/django_toosimple_q/migrations/0006_task_replacement.py
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-07-13 20:01:40.000000 django-toosimple-q-1.0.0b5/django_toosimple_q/migrations/0007_schedule_datetime_kwarg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-07-13 20:01:40.000000 django-toosimple-q-1.0.0b5/django_toosimple_q/migrations/0008_auto_20210902_2111.py
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-07-13 20:01:40.000000 django-toosimple-q-1.0.0b5/django_toosimple_q/migrations/0009_auto_20210902_2245.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-07-13 20:01:40.000000 django-toosimple-q-1.0.0b5/django_toosimple_q/migrations/0010_auto_20220324_0419.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-07-13 20:01:40.000000 django-toosimple-q-1.0.0b5/django_toosimple_q/migrations/0011_workerstatus.py
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-13 20:01:40.000000 django-toosimple-q-1.0.0b5/django_toosimple_q/migrations/0012_rename_last_run_scheduleexec_last_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-13 20:01:40.000000 django-toosimple-q-1.0.0b5/django_toosimple_q/migrations/0013_workerstatus_exit_code_workerstatus_exit_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-07-13 20:01:40.000000 django-toosimple-q-1.0.0b5/django_toosimple_q/migrations/0014_alter_workerstatus_exit_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 20:01:40.000000 django-toosimple-q-1.0.0b5/django_toosimple_q/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10084 2023-07-13 20:01:40.000000 django-toosimple-q-1.0.0b5/django_toosimple_q/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-07-13 20:01:40.000000 django-toosimple-q-1.0.0b5/django_toosimple_q/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-07-13 20:01:40.000000 django-toosimple-q-1.0.0b5/django_toosimple_q/schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2649 2023-07-13 20:01:40.000000 django-toosimple-q-1.0.0b5/django_toosimple_q/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:01:51.000000 django-toosimple-q-1.0.0b5/django_toosimple_q/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:01:51.000000 django-toosimple-q-1.0.0b5/django_toosimple_q/templates/toosimpleq/
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-13 20:01:40.000000 django-toosimple-q-1.0.0b5/django_toosimple_q/templates/toosimpleq/schedule.html
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-13 20:01:40.000000 django-toosimple-q-1.0.0b5/django_toosimple_q/templates/toosimpleq/task.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:01:51.000000 django-toosimple-q-1.0.0b5/django_toosimple_q/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 20:01:40.000000 django-toosimple-q-1.0.0b5/django_toosimple_q/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8448 2023-07-13 20:01:40.000000 django-toosimple-q-1.0.0b5/django_toosimple_q/tests/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:01:51.000000 django-toosimple-q-1.0.0b5/django_toosimple_q/tests/concurrency/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 20:01:40.000000 django-toosimple-q-1.0.0b5/django_toosimple_q/tests/concurrency/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-13 20:01:40.000000 django-toosimple-q-1.0.0b5/django_toosimple_q/tests/concurrency/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:01:51.000000 django-toosimple-q-1.0.0b5/django_toosimple_q/tests/demo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 20:01:40.000000 django-toosimple-q-1.0.0b5/django_toosimple_q/tests/demo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-07-13 20:01:40.000000 django-toosimple-q-1.0.0b5/django_toosimple_q/tests/demo/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-07-13 20:01:40.000000 django-toosimple-q-1.0.0b5/django_toosimple_q/tests/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-13 20:01:40.000000 django-toosimple-q-1.0.0b5/django_toosimple_q/tests/settings_bg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-07-13 20:01:40.000000 django-toosimple-q-1.0.0b5/django_toosimple_q/tests/settings_bg_lag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2409 2023-07-13 20:01:40.000000 django-toosimple-q-1.0.0b5/django_toosimple_q/tests/tests_admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3815 2023-07-13 20:01:40.000000 django-toosimple-q-1.0.0b5/django_toosimple_q/tests/tests_concurrency.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-07-13 20:01:40.000000 django-toosimple-q-1.0.0b5/django_toosimple_q/tests/tests_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-07-13 20:01:40.000000 django-toosimple-q-1.0.0b5/django_toosimple_q/tests/tests_regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9711 2023-07-13 20:01:40.000000 django-toosimple-q-1.0.0b5/django_toosimple_q/tests/tests_schedules.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26230 2023-07-13 20:01:40.000000 django-toosimple-q-1.0.0b5/django_toosimple_q/tests/tests_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9100 2023-07-13 20:01:40.000000 django-toosimple-q-1.0.0b5/django_toosimple_q/tests/tests_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-07-13 20:01:40.000000 django-toosimple-q-1.0.0b5/django_toosimple_q/tests/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-07-13 20:01:40.000000 django-toosimple-q-1.0.0b5/django_toosimple_q/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:01:51.000000 django-toosimple-q-1.0.0b5/django_toosimple_q.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16724 2023-07-13 20:01:51.000000 django-toosimple-q-1.0.0b5/django_toosimple_q.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-07-13 20:01:51.000000 django-toosimple-q-1.0.0b5/django_toosimple_q.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 20:01:51.000000 django-toosimple-q-1.0.0b5/django_toosimple_q.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 20:01:51.000000 django-toosimple-q-1.0.0b5/django_toosimple_q.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-13 20:01:51.000000 django-toosimple-q-1.0.0b5/django_toosimple_q.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-13 20:01:51.000000 django-toosimple-q-1.0.0b5/django_toosimple_q.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 20:01:51.000000 django-toosimple-q-1.0.0b5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-07-13 20:01:40.000000 django-toosimple-q-1.0.0b5/setup.py
```

### Comparing `django-toosimple-q-1.0.0b4/PKG-INFO` & `django-toosimple-q-1.0.0b5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-toosimple-q
-Version: 1.0.0b4
+Version: 1.0.0b5
 Summary: A simplistic task queue and cron-like scheduler for Django
 Home-page: https://github.com/olivierdalang/django-toosimple-q
 Author: Olivier Dalang
 Author-email: olivier.dalang@gmail.com
 License: MIT
 Description: # Django Too Simple Queue
```

### Comparing `django-toosimple-q-1.0.0b4/README.md` & `django-toosimple-q-1.0.0b5/README.md`

 * *Files identical despite different names*

### Comparing `django-toosimple-q-1.0.0b4/django_toosimple_q/admin.py` & `django-toosimple-q-1.0.0b5/django_toosimple_q/admin.py`

 * *Files identical despite different names*

### Comparing `django-toosimple-q-1.0.0b4/django_toosimple_q/contrib/mail/tests.py` & `django-toosimple-q-1.0.0b5/django_toosimple_q/contrib/mail/tests.py`

 * *Files identical despite different names*

### Comparing `django-toosimple-q-1.0.0b4/django_toosimple_q/decorators.py` & `django-toosimple-q-1.0.0b5/django_toosimple_q/decorators.py`

 * *Files identical despite different names*

### Comparing `django-toosimple-q-1.0.0b4/django_toosimple_q/logging.py` & `django-toosimple-q-1.0.0b5/django_toosimple_q/logging.py`

 * *Files identical despite different names*

### Comparing `django-toosimple-q-1.0.0b4/django_toosimple_q/management/commands/worker.py` & `django-toosimple-q-1.0.0b5/django_toosimple_q/management/commands/worker.py`

 * *Files identical despite different names*

### Comparing `django-toosimple-q-1.0.0b4/django_toosimple_q/migrations/0001_initial.py` & `django-toosimple-q-1.0.0b5/django_toosimple_q/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-toosimple-q-1.0.0b4/django_toosimple_q/migrations/0002_auto_20191101_1838.py` & `django-toosimple-q-1.0.0b5/django_toosimple_q/migrations/0002_auto_20191101_1838.py`

 * *Files identical despite different names*

### Comparing `django-toosimple-q-1.0.0b4/django_toosimple_q/migrations/0005_auto_20210302_1748.py` & `django-toosimple-q-1.0.0b5/django_toosimple_q/migrations/0005_auto_20210302_1748.py`

 * *Files identical despite different names*

### Comparing `django-toosimple-q-1.0.0b4/django_toosimple_q/migrations/0006_task_replacement.py` & `django-toosimple-q-1.0.0b5/django_toosimple_q/migrations/0006_task_replacement.py`

 * *Files identical despite different names*

### Comparing `django-toosimple-q-1.0.0b4/django_toosimple_q/migrations/0008_auto_20210902_2111.py` & `django-toosimple-q-1.0.0b5/django_toosimple_q/migrations/0008_auto_20210902_2111.py`

 * *Files identical despite different names*

### Comparing `django-toosimple-q-1.0.0b4/django_toosimple_q/migrations/0009_auto_20210902_2245.py` & `django-toosimple-q-1.0.0b5/django_toosimple_q/migrations/0009_auto_20210902_2245.py`

 * *Files identical despite different names*

### Comparing `django-toosimple-q-1.0.0b4/django_toosimple_q/migrations/0010_auto_20220324_0419.py` & `django-toosimple-q-1.0.0b5/django_toosimple_q/migrations/0010_auto_20220324_0419.py`

 * *Files identical despite different names*

### Comparing `django-toosimple-q-1.0.0b4/django_toosimple_q/migrations/0011_workerstatus.py` & `django-toosimple-q-1.0.0b5/django_toosimple_q/migrations/0011_workerstatus.py`

 * *Files identical despite different names*

### Comparing `django-toosimple-q-1.0.0b4/django_toosimple_q/migrations/0012_rename_last_run_scheduleexec_last_task.py` & `django-toosimple-q-1.0.0b5/django_toosimple_q/migrations/0012_rename_last_run_scheduleexec_last_task.py`

 * *Files identical despite different names*

### Comparing `django-toosimple-q-1.0.0b4/django_toosimple_q/migrations/0013_workerstatus_exit_code_workerstatus_exit_log.py` & `django-toosimple-q-1.0.0b5/django_toosimple_q/migrations/0013_workerstatus_exit_code_workerstatus_exit_log.py`

 * *Files identical despite different names*

### Comparing `django-toosimple-q-1.0.0b4/django_toosimple_q/models.py` & `django-toosimple-q-1.0.0b5/django_toosimple_q/models.py`

 * *Files identical despite different names*

### Comparing `django-toosimple-q-1.0.0b4/django_toosimple_q/schedule.py` & `django-toosimple-q-1.0.0b5/django_toosimple_q/schedule.py`

 * *Files identical despite different names*

### Comparing `django-toosimple-q-1.0.0b4/django_toosimple_q/task.py` & `django-toosimple-q-1.0.0b5/django_toosimple_q/task.py`

 * *Files identical despite different names*

### Comparing `django-toosimple-q-1.0.0b4/django_toosimple_q/tests/base.py` & `django-toosimple-q-1.0.0b5/django_toosimple_q/tests/base.py`

 * *Files identical despite different names*

### Comparing `django-toosimple-q-1.0.0b4/django_toosimple_q/tests/concurrency/tasks.py` & `django-toosimple-q-1.0.0b5/django_toosimple_q/tests/concurrency/tasks.py`

 * *Files identical despite different names*

### Comparing `django-toosimple-q-1.0.0b4/django_toosimple_q/tests/demo/tasks.py` & `django-toosimple-q-1.0.0b5/django_toosimple_q/tests/demo/tasks.py`

 * *Files identical despite different names*

### Comparing `django-toosimple-q-1.0.0b4/django_toosimple_q/tests/settings.py` & `django-toosimple-q-1.0.0b5/django_toosimple_q/tests/settings.py`

 * *Files identical despite different names*

### Comparing `django-toosimple-q-1.0.0b4/django_toosimple_q/tests/tests_admin.py` & `django-toosimple-q-1.0.0b5/django_toosimple_q/tests/tests_admin.py`

 * *Files identical despite different names*

### Comparing `django-toosimple-q-1.0.0b4/django_toosimple_q/tests/tests_concurrency.py` & `django-toosimple-q-1.0.0b5/django_toosimple_q/tests/tests_concurrency.py`

 * *Files identical despite different names*

### Comparing `django-toosimple-q-1.0.0b4/django_toosimple_q/tests/tests_regression.py` & `django-toosimple-q-1.0.0b5/django_toosimple_q/tests/tests_regression.py`

 * *Files identical despite different names*

### Comparing `django-toosimple-q-1.0.0b4/django_toosimple_q/tests/tests_schedules.py` & `django-toosimple-q-1.0.0b5/django_toosimple_q/tests/tests_schedules.py`

 * *Files identical despite different names*

### Comparing `django-toosimple-q-1.0.0b4/django_toosimple_q/tests/tests_tasks.py` & `django-toosimple-q-1.0.0b5/django_toosimple_q/tests/tests_tasks.py`

 * *Files identical despite different names*

### Comparing `django-toosimple-q-1.0.0b4/django_toosimple_q/tests/tests_worker.py` & `django-toosimple-q-1.0.0b5/django_toosimple_q/tests/tests_worker.py`

 * *Files identical despite different names*

### Comparing `django-toosimple-q-1.0.0b4/django_toosimple_q.egg-info/PKG-INFO` & `django-toosimple-q-1.0.0b5/django_toosimple_q.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-toosimple-q
-Version: 1.0.0b4
+Version: 1.0.0b5
 Summary: A simplistic task queue and cron-like scheduler for Django
 Home-page: https://github.com/olivierdalang/django-toosimple-q
 Author: Olivier Dalang
 Author-email: olivier.dalang@gmail.com
 License: MIT
 Description: # Django Too Simple Queue
```

### Comparing `django-toosimple-q-1.0.0b4/django_toosimple_q.egg-info/SOURCES.txt` & `django-toosimple-q-1.0.0b5/django_toosimple_q.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -33,24 +33,26 @@
 django_toosimple_q/migrations/0007_schedule_datetime_kwarg.py
 django_toosimple_q/migrations/0008_auto_20210902_2111.py
 django_toosimple_q/migrations/0009_auto_20210902_2245.py
 django_toosimple_q/migrations/0010_auto_20220324_0419.py
 django_toosimple_q/migrations/0011_workerstatus.py
 django_toosimple_q/migrations/0012_rename_last_run_scheduleexec_last_task.py
 django_toosimple_q/migrations/0013_workerstatus_exit_code_workerstatus_exit_log.py
+django_toosimple_q/migrations/0014_alter_workerstatus_exit_code.py
 django_toosimple_q/migrations/__init__.py
 django_toosimple_q/templates/toosimpleq/schedule.html
 django_toosimple_q/templates/toosimpleq/task.html
 django_toosimple_q/tests/__init__.py
 django_toosimple_q/tests/base.py
 django_toosimple_q/tests/settings.py
 django_toosimple_q/tests/settings_bg.py
 django_toosimple_q/tests/settings_bg_lag.py
 django_toosimple_q/tests/tests_admin.py
 django_toosimple_q/tests/tests_concurrency.py
+django_toosimple_q/tests/tests_integration.py
 django_toosimple_q/tests/tests_regression.py
 django_toosimple_q/tests/tests_schedules.py
 django_toosimple_q/tests/tests_tasks.py
 django_toosimple_q/tests/tests_worker.py
 django_toosimple_q/tests/urls.py
 django_toosimple_q/tests/utils.py
 django_toosimple_q/tests/concurrency/__init__.py
```

### Comparing `django-toosimple-q-1.0.0b4/setup.py` & `django-toosimple-q-1.0.0b5/setup.py`

 * *Files identical despite different names*

