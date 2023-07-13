# Comparing `tmp/lino-noi-23.5.0.tar.gz` & `tmp/lino-noi-23.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lino-noi-23.5.0.tar", last modified: Tue May  9 05:22:19 2023, max compression
+gzip compressed data, was "lino-noi-23.7.0.tar", last modified: Thu Jul 13 12:25:42 2023, max compression
```

## Comparing `lino-noi-23.5.0.tar` & `lino-noi-23.7.0.tar`

### file list

```diff
@@ -1,119 +1,120 @@
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-05-09 05:22:19.820716 lino-noi-23.5.0/
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-05-09 05:22:19.812715 lino-noi-23.5.0/.idea/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      166 2015-09-19 04:08:02.000000 lino-noi-23.5.0/.idea/encodings.xml
--rw-rw-rw-   0 luc       (1000) www-data    (33)     1839 2015-09-19 04:08:02.000000 lino-noi-23.5.0/.idea/misc.xml
--rw-rw-rw-   0 luc       (1000) www-data    (33)      260 2015-09-19 04:08:02.000000 lino-noi-23.5.0/.idea/modules.xml
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-05-09 05:22:19.812715 lino-noi-23.5.0/.idea/scopes/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      139 2015-09-19 04:08:02.000000 lino-noi-23.5.0/.idea/scopes/scope_settings.xml
--rw-rw-rw-   0 luc       (1000) www-data    (33)      166 2015-09-19 04:08:02.000000 lino-noi-23.5.0/.idea/vcs.xml
--rw-rw-rw-   0 luc       (1000) www-data    (33)     2202 2015-09-19 04:08:02.000000 lino-noi-23.5.0/.idea/workspace.xml
--rw-rw-rw-   0 luc       (1000) www-data    (33)    34523 2021-04-07 12:54:16.000000 lino-noi-23.5.0/COPYING
--rw-rw-rw-   0 luc       (1000) www-data    (33)      109 2016-08-14 01:22:00.000000 lino-noi-23.5.0/MANIFEST.in
--rw-rw-r--   0 luc       (1000) www-data    (33)     1518 2023-05-09 05:22:19.820716 lino-noi-23.5.0/PKG-INFO
--rw-rw-rw-   0 luc       (1000) www-data    (33)      716 2023-03-29 14:44:08.000000 lino-noi-23.5.0/README.rst
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-05-09 05:22:19.812715 lino-noi-23.5.0/lino_noi/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      457 2022-08-17 01:06:46.000000 lino-noi-23.5.0/lino_noi/__init__.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-05-09 05:22:19.812715 lino-noi-23.5.0/lino_noi/lib/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      297 2021-04-07 10:22:54.000000 lino-noi-23.5.0/lino_noi/lib/__init__.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-05-09 05:22:19.812715 lino-noi-23.5.0/lino_noi/lib/cal/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      299 2021-04-07 10:22:54.000000 lino-noi-23.5.0/lino_noi/lib/cal/__init__.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-05-09 05:22:19.812715 lino-noi-23.5.0/lino_noi/lib/cal/fixtures/
--rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2017-04-04 14:35:11.000000 lino-noi-23.5.0/lino_noi/lib/cal/fixtures/__init__.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)       49 2017-04-04 14:35:11.000000 lino-noi-23.5.0/lino_noi/lib/cal/fixtures/std.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     3523 2023-04-15 09:49:10.000000 lino-noi-23.5.0/lino_noi/lib/cal/models.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-05-09 05:22:19.812715 lino-noi-23.5.0/lino_noi/lib/contacts/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      274 2021-04-07 10:22:54.000000 lino-noi-23.5.0/lino_noi/lib/contacts/__init__.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-05-09 05:22:19.816715 lino-noi-23.5.0/lino_noi/lib/contacts/fixtures/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      245 2021-04-07 10:22:55.000000 lino-noi-23.5.0/lino_noi/lib/contacts/fixtures/__init__.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)       55 2020-04-04 06:56:19.000000 lino-noi-23.5.0/lino_noi/lib/contacts/fixtures/demo.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)       48 2017-05-26 22:13:00.000000 lino-noi-23.5.0/lino_noi/lib/contacts/fixtures/std.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     2587 2021-04-07 10:22:54.000000 lino-noi-23.5.0/lino_noi/lib/contacts/models.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-05-09 05:22:19.816715 lino-noi-23.5.0/lino_noi/lib/courses/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      812 2021-04-07 10:22:54.000000 lino-noi-23.5.0/lino_noi/lib/courses/__init__.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      717 2022-11-08 12:29:27.000000 lino-noi-23.5.0/lino_noi/lib/courses/models.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     2532 2022-11-08 12:30:48.000000 lino-noi-23.5.0/lino_noi/lib/courses/ui.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-05-09 05:22:19.816715 lino-noi-23.5.0/lino_noi/lib/groups/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      319 2021-04-07 10:22:54.000000 lino-noi-23.5.0/lino_noi/lib/groups/__init__.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      749 2021-08-16 10:54:17.000000 lino-noi-23.5.0/lino_noi/lib/groups/models.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-05-09 05:22:19.816715 lino-noi-23.5.0/lino_noi/lib/noi/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      329 2021-04-07 10:22:54.000000 lino-noi-23.5.0/lino_noi/lib/noi/__init__.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-05-09 05:22:19.816715 lino-noi-23.5.0/lino_noi/lib/noi/fixtures/
--rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2015-09-19 04:09:02.000000 lino-noi-23.5.0/lino_noi/lib/noi/fixtures/__init__.py
--rw-rw-r--   0 luc       (1000) www-data    (33)    18048 2023-04-05 09:42:20.000000 lino-noi-23.5.0/lino_noi/lib/noi/fixtures/demo.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     6630 2022-10-18 23:19:00.000000 lino-noi-23.5.0/lino_noi/lib/noi/fixtures/linotickets.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     2138 2023-05-02 09:00:00.000000 lino-noi-23.5.0/lino_noi/lib/noi/help_texts.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      540 2021-06-15 17:12:44.000000 lino-noi-23.5.0/lino_noi/lib/noi/layouts.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-05-09 05:22:19.812715 lino-noi-23.5.0/lino_noi/lib/noi/locale/
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-05-09 05:22:19.808715 lino-noi-23.5.0/lino_noi/lib/noi/locale/de/
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-05-09 05:22:19.816715 lino-noi-23.5.0/lino_noi/lib/noi/locale/de/LC_MESSAGES/
--rw-rw-rw-   0 luc       (1000) www-data    (33)     2008 2017-04-04 14:35:11.000000 lino-noi-23.5.0/lino_noi/lib/noi/locale/de/LC_MESSAGES/django.mo
--rw-rw-rw-   0 luc       (1000) www-data    (33)    14514 2019-03-29 11:25:54.000000 lino-noi-23.5.0/lino_noi/lib/noi/locale/de/LC_MESSAGES/django.po
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-05-09 05:22:19.812715 lino-noi-23.5.0/lino_noi/lib/noi/locale/et/
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-05-09 05:22:19.816715 lino-noi-23.5.0/lino_noi/lib/noi/locale/et/LC_MESSAGES/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      660 2017-04-04 14:35:11.000000 lino-noi-23.5.0/lino_noi/lib/noi/locale/et/LC_MESSAGES/django.mo
--rw-rw-rw-   0 luc       (1000) www-data    (33)    13858 2019-03-29 11:25:55.000000 lino-noi-23.5.0/lino_noi/lib/noi/locale/et/LC_MESSAGES/django.po
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-05-09 05:22:19.812715 lino-noi-23.5.0/lino_noi/lib/noi/locale/fr/
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-05-09 05:22:19.816715 lino-noi-23.5.0/lino_noi/lib/noi/locale/fr/LC_MESSAGES/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      490 2017-04-04 14:35:11.000000 lino-noi-23.5.0/lino_noi/lib/noi/locale/fr/LC_MESSAGES/django.mo
--rw-rw-rw-   0 luc       (1000) www-data    (33)    13846 2019-03-29 11:25:54.000000 lino-noi-23.5.0/lino_noi/lib/noi/locale/fr/LC_MESSAGES/django.po
--rw-rw-rw-   0 luc       (1000) www-data    (33)    22188 2021-04-07 10:22:54.000000 lino-noi-23.5.0/lino_noi/lib/noi/migrate.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     1131 2021-04-07 10:22:54.000000 lino-noi-23.5.0/lino_noi/lib/noi/models.py
--rw-rw-r--   0 luc       (1000) www-data    (33)     6636 2023-03-13 22:30:18.000000 lino-noi-23.5.0/lino_noi/lib/noi/settings.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     2810 2022-12-23 05:58:38.000000 lino-noi-23.5.0/lino_noi/lib/noi/user_types.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      383 2021-05-29 09:01:55.000000 lino-noi-23.5.0/lino_noi/lib/noi/workflows.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-05-09 05:22:19.816715 lino-noi-23.5.0/lino_noi/lib/products/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      301 2021-04-07 10:22:54.000000 lino-noi-23.5.0/lino_noi/lib/products/__init__.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      522 2021-04-23 19:31:33.000000 lino-noi-23.5.0/lino_noi/lib/products/models.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-05-09 05:22:19.816715 lino-noi-23.5.0/lino_noi/lib/public/
--rw-rw-rw-   0 luc       (1000) www-data    (33)     1166 2021-12-22 12:48:36.000000 lino-noi-23.5.0/lino_noi/lib/public/__init__.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-05-09 05:22:19.812715 lino-noi-23.5.0/lino_noi/lib/public/config/
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-05-09 05:22:19.816715 lino-noi-23.5.0/lino_noi/lib/public/config/noi/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      474 2019-11-25 17:29:52.000000 lino-noi-23.5.0/lino_noi/lib/public/config/noi/index.html
--rw-rw-rw-   0 luc       (1000) www-data    (33)      720 2022-09-01 18:33:50.000000 lino-noi-23.5.0/lino_noi/lib/public/config/noi/tickets.Ticket.html
--rw-rw-rw-   0 luc       (1000) www-data    (33)      554 2021-04-07 10:22:54.000000 lino-noi-23.5.0/lino_noi/lib/public/renderer.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     1583 2021-04-07 10:22:54.000000 lino-noi-23.5.0/lino_noi/lib/public/views.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-05-09 05:22:19.820716 lino-noi-23.5.0/lino_noi/lib/sales/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      311 2021-04-07 10:22:54.000000 lino-noi-23.5.0/lino_noi/lib/sales/__init__.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-05-09 05:22:19.812715 lino-noi-23.5.0/lino_noi/lib/sales/config/
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-05-09 05:22:19.812715 lino-noi-23.5.0/lino_noi/lib/sales/config/sales/
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-05-09 05:22:19.820716 lino-noi-23.5.0/lino_noi/lib/sales/config/sales/VatProductInvoice/
--rw-rw-rw-   0 luc       (1000) www-data    (33)     1413 2023-02-15 06:31:52.000000 lino-noi-23.5.0/lino_noi/lib/sales/config/sales/VatProductInvoice/default.weasy.html
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-05-09 05:22:19.820716 lino-noi-23.5.0/lino_noi/lib/sales/fixtures/
--rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2016-05-09 16:04:58.000000 lino-noi-23.5.0/lino_noi/lib/sales/fixtures/__init__.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)       51 2017-02-26 08:07:55.000000 lino-noi-23.5.0/lino_noi/lib/sales/fixtures/std.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      985 2022-12-26 16:50:31.000000 lino-noi-23.5.0/lino_noi/lib/sales/models.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-05-09 05:22:19.820716 lino-noi-23.5.0/lino_noi/lib/subscriptions/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      189 2023-01-06 20:30:18.000000 lino-noi-23.5.0/lino_noi/lib/subscriptions/__init__.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      378 2023-01-06 20:50:15.000000 lino-noi-23.5.0/lino_noi/lib/subscriptions/models.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-05-09 05:22:19.820716 lino-noi-23.5.0/lino_noi/lib/tickets/
--rw-rw-rw-   0 luc       (1000) www-data    (33)     1658 2023-01-08 01:21:19.000000 lino-noi-23.5.0/lino_noi/lib/tickets/__init__.py
--rw-rw-r--   0 luc       (1000) www-data    (33)    15885 2023-02-16 20:05:18.000000 lino-noi-23.5.0/lino_noi/lib/tickets/models.py
--rw-rw-r--   0 luc       (1000) www-data    (33)     3858 2022-10-30 00:45:53.000000 lino-noi-23.5.0/lino_noi/lib/tickets/workflows.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-05-09 05:22:19.820716 lino-noi-23.5.0/lino_noi/lib/topics/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      213 2021-04-07 10:22:54.000000 lino-noi-23.5.0/lino_noi/lib/topics/__init__.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      622 2021-04-07 10:22:54.000000 lino-noi-23.5.0/lino_noi/lib/topics/models.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-05-09 05:22:19.820716 lino-noi-23.5.0/lino_noi/lib/users/
--rw-rw-rw-   0 luc       (1000) www-data    (33)       37 2023-03-06 06:43:39.000000 lino-noi-23.5.0/lino_noi/lib/users/__init__.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-05-09 05:22:19.820716 lino-noi-23.5.0/lino_noi/lib/users/fixtures/
--rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2015-09-19 04:09:00.000000 lino-noi-23.5.0/lino_noi/lib/users/fixtures/__init__.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)       46 2017-06-13 23:56:49.000000 lino-noi-23.5.0/lino_noi/lib/users/fixtures/demo.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)       48 2017-06-13 23:56:50.000000 lino-noi-23.5.0/lino_noi/lib/users/fixtures/demo2.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)       52 2017-06-13 23:56:50.000000 lino-noi-23.5.0/lino_noi/lib/users/fixtures/demo_users.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      248 2022-11-08 12:29:27.000000 lino-noi-23.5.0/lino_noi/lib/users/models.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     1636 2023-04-15 09:49:32.000000 lino-noi-23.5.0/lino_noi/lib/users/ui.py
--rw-rw-r--   0 luc       (1000) www-data    (33)     3080 2023-05-09 05:21:48.000000 lino-noi-23.5.0/lino_noi/setup_info.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-05-09 05:22:19.812715 lino-noi-23.5.0/lino_noi.egg-info/
--rw-rw-rw-   0 luc       (1000) www-data    (33)     1518 2023-05-09 05:22:19.000000 lino-noi-23.5.0/lino_noi.egg-info/PKG-INFO
--rw-rw-rw-   0 luc       (1000) www-data    (33)     2541 2023-05-09 05:22:19.000000 lino-noi-23.5.0/lino_noi.egg-info/SOURCES.txt
--rw-rw-rw-   0 luc       (1000) www-data    (33)        1 2023-05-09 05:22:19.000000 lino-noi-23.5.0/lino_noi.egg-info/dependency_links.txt
--rw-rw-rw-   0 luc       (1000) www-data    (33)        1 2016-08-31 16:13:18.000000 lino-noi-23.5.0/lino_noi.egg-info/not-zip-safe
--rw-rw-rw-   0 luc       (1000) www-data    (33)        8 2023-05-09 05:22:19.000000 lino-noi-23.5.0/lino_noi.egg-info/requires.txt
--rw-rw-rw-   0 luc       (1000) www-data    (33)        9 2023-05-09 05:22:19.000000 lino-noi-23.5.0/lino_noi.egg-info/top_level.txt
--rw-rw-rw-   0 luc       (1000) www-data    (33)      263 2021-05-05 05:16:56.000000 lino-noi-23.5.0/requirements.txt
--rw-rw-r--   0 luc       (1000) www-data    (33)       38 2023-05-09 05:22:19.820716 lino-noi-23.5.0/setup.cfg
--rw-rw-rw-   0 luc       (1000) www-data    (33)      179 2020-07-10 07:49:24.000000 lino-noi-23.5.0/setup.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      487 2021-04-25 11:53:26.000000 lino-noi-23.5.0/tasks.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-05-09 05:22:19.820716 lino-noi-23.5.0/tests/
--rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2019-12-18 18:50:53.000000 lino-noi-23.5.0/tests/__init__.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      189 2019-12-18 18:51:44.000000 lino-noi-23.5.0/tests/test_docs.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      186 2019-12-18 18:51:08.000000 lino-noi-23.5.0/tests/test_packages.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-07-13 12:25:42.888773 lino-noi-23.7.0/
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-07-13 12:25:42.884773 lino-noi-23.7.0/.idea/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      166 2015-09-19 04:08:02.000000 lino-noi-23.7.0/.idea/encodings.xml
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     1839 2015-09-19 04:08:02.000000 lino-noi-23.7.0/.idea/misc.xml
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      260 2015-09-19 04:08:02.000000 lino-noi-23.7.0/.idea/modules.xml
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-07-13 12:25:42.884773 lino-noi-23.7.0/.idea/scopes/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      139 2015-09-19 04:08:02.000000 lino-noi-23.7.0/.idea/scopes/scope_settings.xml
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      166 2015-09-19 04:08:02.000000 lino-noi-23.7.0/.idea/vcs.xml
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     2202 2015-09-19 04:08:02.000000 lino-noi-23.7.0/.idea/workspace.xml
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    34523 2021-04-07 12:54:16.000000 lino-noi-23.7.0/COPYING
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      109 2016-08-14 01:22:00.000000 lino-noi-23.7.0/MANIFEST.in
+-rw-rw-r--   0 luc       (1000) www-data    (33)     1518 2023-07-13 12:25:42.888773 lino-noi-23.7.0/PKG-INFO
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      716 2023-03-29 14:44:08.000000 lino-noi-23.7.0/README.rst
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-07-13 12:25:42.884773 lino-noi-23.7.0/lino_noi/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      457 2022-08-17 01:06:46.000000 lino-noi-23.7.0/lino_noi/__init__.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-07-13 12:25:42.884773 lino-noi-23.7.0/lino_noi/lib/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      297 2021-04-07 10:22:54.000000 lino-noi-23.7.0/lino_noi/lib/__init__.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-07-13 12:25:42.884773 lino-noi-23.7.0/lino_noi/lib/cal/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      299 2021-04-07 10:22:54.000000 lino-noi-23.7.0/lino_noi/lib/cal/__init__.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-07-13 12:25:42.884773 lino-noi-23.7.0/lino_noi/lib/cal/fixtures/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2017-04-04 14:35:11.000000 lino-noi-23.7.0/lino_noi/lib/cal/fixtures/__init__.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)       49 2017-04-04 14:35:11.000000 lino-noi-23.7.0/lino_noi/lib/cal/fixtures/std.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     3523 2023-04-15 09:49:10.000000 lino-noi-23.7.0/lino_noi/lib/cal/models.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-07-13 12:25:42.884773 lino-noi-23.7.0/lino_noi/lib/contacts/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      274 2021-04-07 10:22:54.000000 lino-noi-23.7.0/lino_noi/lib/contacts/__init__.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-07-13 12:25:42.884773 lino-noi-23.7.0/lino_noi/lib/contacts/fixtures/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      245 2021-04-07 10:22:55.000000 lino-noi-23.7.0/lino_noi/lib/contacts/fixtures/__init__.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)       55 2020-04-04 06:56:19.000000 lino-noi-23.7.0/lino_noi/lib/contacts/fixtures/demo.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)       48 2017-05-26 22:13:00.000000 lino-noi-23.7.0/lino_noi/lib/contacts/fixtures/std.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     3239 2023-07-09 03:53:22.000000 lino-noi-23.7.0/lino_noi/lib/contacts/models.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-07-13 12:25:42.884773 lino-noi-23.7.0/lino_noi/lib/courses/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      812 2021-04-07 10:22:54.000000 lino-noi-23.7.0/lino_noi/lib/courses/__init__.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      717 2022-11-08 12:29:27.000000 lino-noi-23.7.0/lino_noi/lib/courses/models.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     2532 2022-11-08 12:30:48.000000 lino-noi-23.7.0/lino_noi/lib/courses/ui.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-07-13 12:25:42.884773 lino-noi-23.7.0/lino_noi/lib/groups/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      319 2021-04-07 10:22:54.000000 lino-noi-23.7.0/lino_noi/lib/groups/__init__.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      749 2021-08-16 10:54:17.000000 lino-noi-23.7.0/lino_noi/lib/groups/models.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-07-13 12:25:42.884773 lino-noi-23.7.0/lino_noi/lib/noi/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      329 2021-04-07 10:22:54.000000 lino-noi-23.7.0/lino_noi/lib/noi/__init__.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-07-13 12:25:42.884773 lino-noi-23.7.0/lino_noi/lib/noi/fixtures/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2015-09-19 04:09:02.000000 lino-noi-23.7.0/lino_noi/lib/noi/fixtures/__init__.py
+-rw-rw-r--   0 luc       (1000) www-data    (33)    19620 2023-07-01 05:01:29.000000 lino-noi-23.7.0/lino_noi/lib/noi/fixtures/demo.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     6630 2022-10-18 23:19:00.000000 lino-noi-23.7.0/lino_noi/lib/noi/fixtures/linotickets.py
+-rw-rw-r--   0 luc       (1000) www-data    (33)      198 2023-05-12 19:49:16.000000 lino-noi-23.7.0/lino_noi/lib/noi/fixtures/minimal_ledger.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     2138 2023-07-13 08:56:42.000000 lino-noi-23.7.0/lino_noi/lib/noi/help_texts.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      540 2021-06-15 17:12:44.000000 lino-noi-23.7.0/lino_noi/lib/noi/layouts.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-07-13 12:25:42.880772 lino-noi-23.7.0/lino_noi/lib/noi/locale/
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-07-13 12:25:42.880772 lino-noi-23.7.0/lino_noi/lib/noi/locale/de/
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-07-13 12:25:42.884773 lino-noi-23.7.0/lino_noi/lib/noi/locale/de/LC_MESSAGES/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     2008 2017-04-04 14:35:11.000000 lino-noi-23.7.0/lino_noi/lib/noi/locale/de/LC_MESSAGES/django.mo
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    14514 2019-03-29 11:25:54.000000 lino-noi-23.7.0/lino_noi/lib/noi/locale/de/LC_MESSAGES/django.po
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-07-13 12:25:42.880772 lino-noi-23.7.0/lino_noi/lib/noi/locale/et/
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-07-13 12:25:42.884773 lino-noi-23.7.0/lino_noi/lib/noi/locale/et/LC_MESSAGES/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      660 2017-04-04 14:35:11.000000 lino-noi-23.7.0/lino_noi/lib/noi/locale/et/LC_MESSAGES/django.mo
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    13858 2019-03-29 11:25:55.000000 lino-noi-23.7.0/lino_noi/lib/noi/locale/et/LC_MESSAGES/django.po
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-07-13 12:25:42.880772 lino-noi-23.7.0/lino_noi/lib/noi/locale/fr/
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-07-13 12:25:42.884773 lino-noi-23.7.0/lino_noi/lib/noi/locale/fr/LC_MESSAGES/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      490 2017-04-04 14:35:11.000000 lino-noi-23.7.0/lino_noi/lib/noi/locale/fr/LC_MESSAGES/django.mo
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    13846 2019-03-29 11:25:54.000000 lino-noi-23.7.0/lino_noi/lib/noi/locale/fr/LC_MESSAGES/django.po
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    22188 2021-04-07 10:22:54.000000 lino-noi-23.7.0/lino_noi/lib/noi/migrate.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     1131 2021-04-07 10:22:54.000000 lino-noi-23.7.0/lino_noi/lib/noi/models.py
+-rw-rw-r--   0 luc       (1000) www-data    (33)     6755 2023-06-23 08:25:25.000000 lino-noi-23.7.0/lino_noi/lib/noi/settings.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     3039 2023-05-12 19:54:48.000000 lino-noi-23.7.0/lino_noi/lib/noi/user_types.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      383 2023-05-12 19:27:14.000000 lino-noi-23.7.0/lino_noi/lib/noi/workflows.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-07-13 12:25:42.884773 lino-noi-23.7.0/lino_noi/lib/products/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      301 2021-04-07 10:22:54.000000 lino-noi-23.7.0/lino_noi/lib/products/__init__.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      947 2023-05-28 02:47:30.000000 lino-noi-23.7.0/lino_noi/lib/products/models.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-07-13 12:25:42.884773 lino-noi-23.7.0/lino_noi/lib/public/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     1166 2021-12-22 12:48:36.000000 lino-noi-23.7.0/lino_noi/lib/public/__init__.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-07-13 12:25:42.880772 lino-noi-23.7.0/lino_noi/lib/public/config/
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-07-13 12:25:42.884773 lino-noi-23.7.0/lino_noi/lib/public/config/noi/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      474 2019-11-25 17:29:52.000000 lino-noi-23.7.0/lino_noi/lib/public/config/noi/index.html
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      720 2022-09-01 18:33:50.000000 lino-noi-23.7.0/lino_noi/lib/public/config/noi/tickets.Ticket.html
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      554 2021-04-07 10:22:54.000000 lino-noi-23.7.0/lino_noi/lib/public/renderer.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     1583 2021-04-07 10:22:54.000000 lino-noi-23.7.0/lino_noi/lib/public/views.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-07-13 12:25:42.884773 lino-noi-23.7.0/lino_noi/lib/sales/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      311 2021-04-07 10:22:54.000000 lino-noi-23.7.0/lino_noi/lib/sales/__init__.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-07-13 12:25:42.880772 lino-noi-23.7.0/lino_noi/lib/sales/config/
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-07-13 12:25:42.880772 lino-noi-23.7.0/lino_noi/lib/sales/config/sales/
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-07-13 12:25:42.884773 lino-noi-23.7.0/lino_noi/lib/sales/config/sales/VatProductInvoice/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     1413 2023-02-15 06:31:52.000000 lino-noi-23.7.0/lino_noi/lib/sales/config/sales/VatProductInvoice/default.weasy.html
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-07-13 12:25:42.888773 lino-noi-23.7.0/lino_noi/lib/sales/fixtures/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2016-05-09 16:04:58.000000 lino-noi-23.7.0/lino_noi/lib/sales/fixtures/__init__.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)       51 2017-02-26 08:07:55.000000 lino-noi-23.7.0/lino_noi/lib/sales/fixtures/std.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      985 2022-12-26 16:50:31.000000 lino-noi-23.7.0/lino_noi/lib/sales/models.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-07-13 12:25:42.888773 lino-noi-23.7.0/lino_noi/lib/subscriptions/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      189 2023-01-06 20:30:18.000000 lino-noi-23.7.0/lino_noi/lib/subscriptions/__init__.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      378 2023-01-06 20:50:15.000000 lino-noi-23.7.0/lino_noi/lib/subscriptions/models.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-07-13 12:25:42.888773 lino-noi-23.7.0/lino_noi/lib/tickets/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     1658 2023-01-08 01:21:19.000000 lino-noi-23.7.0/lino_noi/lib/tickets/__init__.py
+-rw-rw-r--   0 luc       (1000) www-data    (33)    15885 2023-02-16 20:05:18.000000 lino-noi-23.7.0/lino_noi/lib/tickets/models.py
+-rw-rw-r--   0 luc       (1000) www-data    (33)     3858 2022-10-30 00:45:53.000000 lino-noi-23.7.0/lino_noi/lib/tickets/workflows.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-07-13 12:25:42.888773 lino-noi-23.7.0/lino_noi/lib/topics/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      213 2021-04-07 10:22:54.000000 lino-noi-23.7.0/lino_noi/lib/topics/__init__.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      622 2021-04-07 10:22:54.000000 lino-noi-23.7.0/lino_noi/lib/topics/models.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-07-13 12:25:42.888773 lino-noi-23.7.0/lino_noi/lib/users/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)       37 2023-03-06 06:43:39.000000 lino-noi-23.7.0/lino_noi/lib/users/__init__.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-07-13 12:25:42.888773 lino-noi-23.7.0/lino_noi/lib/users/fixtures/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2015-09-19 04:09:00.000000 lino-noi-23.7.0/lino_noi/lib/users/fixtures/__init__.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)       46 2017-06-13 23:56:49.000000 lino-noi-23.7.0/lino_noi/lib/users/fixtures/demo.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)       48 2017-06-13 23:56:50.000000 lino-noi-23.7.0/lino_noi/lib/users/fixtures/demo2.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)       52 2017-06-13 23:56:50.000000 lino-noi-23.7.0/lino_noi/lib/users/fixtures/demo_users.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      248 2022-11-08 12:29:27.000000 lino-noi-23.7.0/lino_noi/lib/users/models.py
+-rw-rw-r--   0 luc       (1000) www-data    (33)     1639 2023-07-10 20:32:06.000000 lino-noi-23.7.0/lino_noi/lib/users/ui.py
+-rw-rw-r--   0 luc       (1000) www-data    (33)     3080 2023-07-13 12:23:53.000000 lino-noi-23.7.0/lino_noi/setup_info.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-07-13 12:25:42.884773 lino-noi-23.7.0/lino_noi.egg-info/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     1518 2023-07-13 12:25:42.000000 lino-noi-23.7.0/lino_noi.egg-info/PKG-INFO
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     2585 2023-07-13 12:25:42.000000 lino-noi-23.7.0/lino_noi.egg-info/SOURCES.txt
+-rw-rw-rw-   0 luc       (1000) www-data    (33)        1 2023-07-13 12:25:42.000000 lino-noi-23.7.0/lino_noi.egg-info/dependency_links.txt
+-rw-rw-rw-   0 luc       (1000) www-data    (33)        1 2016-08-31 16:13:18.000000 lino-noi-23.7.0/lino_noi.egg-info/not-zip-safe
+-rw-rw-rw-   0 luc       (1000) www-data    (33)        8 2023-07-13 12:25:42.000000 lino-noi-23.7.0/lino_noi.egg-info/requires.txt
+-rw-rw-rw-   0 luc       (1000) www-data    (33)        9 2023-07-13 12:25:42.000000 lino-noi-23.7.0/lino_noi.egg-info/top_level.txt
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      263 2021-05-05 05:16:56.000000 lino-noi-23.7.0/requirements.txt
+-rw-rw-r--   0 luc       (1000) www-data    (33)       38 2023-07-13 12:25:42.888773 lino-noi-23.7.0/setup.cfg
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      179 2020-07-10 07:49:24.000000 lino-noi-23.7.0/setup.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      487 2021-04-25 11:53:26.000000 lino-noi-23.7.0/tasks.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-07-13 12:25:42.888773 lino-noi-23.7.0/tests/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2019-12-18 18:50:53.000000 lino-noi-23.7.0/tests/__init__.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      189 2019-12-18 18:51:44.000000 lino-noi-23.7.0/tests/test_docs.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      186 2019-12-18 18:51:08.000000 lino-noi-23.7.0/tests/test_packages.py
```

### Comparing `lino-noi-23.5.0/.idea/misc.xml` & `lino-noi-23.7.0/.idea/misc.xml`

 * *Files identical despite different names*

### Comparing `lino-noi-23.5.0/.idea/workspace.xml` & `lino-noi-23.7.0/.idea/workspace.xml`

 * *Files identical despite different names*

### Comparing `lino-noi-23.5.0/COPYING` & `lino-noi-23.7.0/COPYING`

 * *Files identical despite different names*

### Comparing `lino-noi-23.5.0/PKG-INFO` & `lino-noi-23.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lino-noi
-Version: 23.5.0
+Version: 23.7.0
 Summary: Manage support tickets and working time.
 Home-page: https://gitlab.com/lino-framework/noi
 Author: Rumma & Ko Ltd
 Author-email: info@lino-framework.org
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
```

### Comparing `lino-noi-23.5.0/README.rst` & `lino-noi-23.7.0/README.rst`

 * *Files identical despite different names*

### Comparing `lino-noi-23.5.0/lino_noi/lib/cal/models.py` & `lino-noi-23.7.0/lino_noi/lib/cal/models.py`

 * *Files identical despite different names*

### Comparing `lino-noi-23.5.0/lino_noi/lib/contacts/models.py` & `lino-noi-23.7.0/lino_noi/lib/contacts/models.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,14 +6,28 @@
 """
 
 from lino.api import dd, _
 from lino.utils import join_words
 
 from lino_xl.lib.contacts.models import *
 
+Partners.detail_layout = 'contacts.PartnerDetail'
+
+PartnerDetail.main = "general contact ledger storage"
+
+PartnerDetail.general = dd.Panel("""
+overview info_box
+checkdata.MessagesByOwner
+""", label=_("General"))
+
+PartnerDetail.contact = dd.Panel("""
+address_box:60 contact_box:30
+remarks
+""", label=_("Contact"))
+
 
 PartnerDetail.address_box = dd.Panel("""
     name_box
     country #region city zip_code:10
     #addr1
     #street_prefix street:25 street_no street_box
     #addr2
@@ -21,44 +35,53 @@
 
 PartnerDetail.contact_box = dd.Panel("""
     url
     phone
     gsm #fax
     """, label=_("Contact"))
 
+PartnerDetail.ledger = dd.Panel("""
+vat_id vat_regime purchase_account payment_term
+vat.VouchersByPartner
+ledger.MovementsByPartner
+""", label=dd.plugins.ledger.verbose_name)
+
+PartnerDetail.storage = dd.Panel("""
+storage.FillersByPartner storage.ProvisionsByPartner storage.MovementsByPartner
+""", label=dd.plugins.storage.verbose_name)
 
 
 class Person(Person):
-    
+
     class Meta(Person.Meta):
         app_label = 'contacts'
         abstract = dd.is_abstract_model(__name__, 'Person')
-        
+
     def __str__(self):
         words = []
         words.append(self.first_name)
         words.append(self.last_name)
         return join_words(*words)
 
 
 class PersonDetail(PersonDetail):
-    
-    main = "general contact #skills tickets"
+
+    main = "general contact #skills tickets ledger storage"
 
     general = dd.Panel("""
     overview info_box
     contacts.RolesByPerson
     """, label=_("General"))
 
     info_box = """
     id:5
     language:10
     email:40
     """
-    
+
     contact = dd.Panel("""
     address_box:60 contact_box:30
     remarks tickets.SitesByPerson #topics.InterestsByPartner
     """, label=_("Contact"))
 
     # skills = dd.Panel("""
     # skills.OffersByEndUser skills.SuggestedTicketsByEndUser
@@ -67,31 +90,31 @@
     tickets = dd.Panel("""
     tickets.TicketsByEndUser tickets.SitesByPerson
     """, label=dd.plugins.tickets.verbose_name)
 
 
     name_box = "last_name first_name:15 gender #title:10"
 
-    
+
 class CompanyDetail(CompanyDetail):
-    main = "general contact #skills tickets"
+    main = "general contact #skills tickets ledger storage"
 
     general = dd.Panel("""
     overview info_box
     contacts.RolesByCompany
     """, label=_("General"))
 
     info_box = """
     id:5
     language:10
     email:40
     """
-    
+
     contact = dd.Panel("""
-    address_box:60 contact_box:30 
+    address_box:60 contact_box:30
     remarks
     """, label=_("Contact"))
 
     # skills = dd.Panel("""
     # skills.OffersByEndUser topics.InterestsByPartner
     # """, label=dd.plugins.skills.verbose_name)
```

### Comparing `lino-noi-23.5.0/lino_noi/lib/courses/__init__.py` & `lino-noi-23.7.0/lino_noi/lib/courses/__init__.py`

 * *Files identical despite different names*

### Comparing `lino-noi-23.5.0/lino_noi/lib/courses/models.py` & `lino-noi-23.7.0/lino_noi/lib/courses/models.py`

 * *Files identical despite different names*

### Comparing `lino-noi-23.5.0/lino_noi/lib/courses/ui.py` & `lino-noi-23.7.0/lino_noi/lib/courses/ui.py`

 * *Files identical despite different names*

### Comparing `lino-noi-23.5.0/lino_noi/lib/groups/models.py` & `lino-noi-23.7.0/lino_noi/lib/groups/models.py`

 * *Files identical despite different names*

### Comparing `lino-noi-23.5.0/lino_noi/lib/noi/fixtures/demo.py` & `lino-noi-23.7.0/lino_noi/lib/noi/fixtures/demo.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # -*- coding: UTF-8 -*-
 # Copyright 2015-2023 Rumma & Ko Ltd
 # License: GNU Affero General Public License v3 (see file COPYING for details)
 
 import datetime ; combine = datetime.datetime.combine
 
+from django.utils.text import format_lazy
 from lino.api import rt, dd, _
 from lino.utils import Cycler, i2d, ONE_DAY
 from lino.core.roles import SiteAdmin
 from lino.modlib.system.choicelists import DurationUnits
 from lino_xl.lib.working.roles import Worker
 from lino.utils.quantities import Duration
 from lino.utils.mldbc import babel_named as named
@@ -44,31 +45,34 @@
 fiddle with get_auth()
 jitsi meeting claire and paul
 jitsi with manu
 brainstorming lou & paul
 catch the brown fox
 """.strip().splitlines())
 
+Product = rt.models.products.Product
+
 def product(name, **kwargs):
-    return rt.models.products.Product(**dd.str2kw("name", name, **kwargs))
+    return Product(**dd.str2kw("name", name, **kwargs))
 
 def tickets_objects():
     # was previously in tickets
     User = rt.models.users.User
     Company = rt.models.contacts.Company
     Person = rt.models.contacts.Person
     TT = rt.models.tickets.TicketType
     Ticket = rt.models.tickets.Ticket
     Group = rt.models.groups.Group
     Membership = rt.models.groups.Membership
     Milestone = dd.plugins.tickets.milestone_model
     Site = dd.plugins.tickets.site_model
     List = rt.models.lists.List
-    InvoicingAreas = rt.models.invoicing.InvoicingAreas
+    # InvoicingAreas = rt.models.invoicing.InvoicingAreas
     Subscription = rt.models.subscriptions.Subscription
+    Component = rt.models.storage.Component
 
 
     customer = UserTypes.customer
     contributor = UserTypes.contributor
     dev = UserTypes.developer
 
     yield create_user("marc", customer, with_person=True)
@@ -134,20 +138,42 @@
         journal_group="sales",
         **dd.str2kw("name", _("Service Level Agreements")))
     yield SLA_JNL
     # yield FollowUpRule(invoicing_area=area, source_journal=SLA_JNL)
 
     sla_hosting = product(_("Hosting (per active user)"), sales_price=600)
     sla_support = product(_("Support availability"), sales_price=249)
-    sla_maintenance = product(_("Maintenance"), sales_price=79)
+    sla_maintenance = product(_("Maintenance"), sales_price=279)
+    #     storage_management=True, delivery_unit="hour")
 
     yield sla_hosting
     yield sla_support
     yield sla_maintenance
 
+
+    devel = Product.objects.get(**dd.str2kw('name', _("Development")))
+
+    tpl = _("Time credit ({} hours)")
+    tc5 = product(format_lazy(tpl, 5), sales_price=350,
+        storage_management=False)
+    yield tc5
+    yield Component(parent=tc5, child=devel, qty="5:00")
+
+    tc10 = product(format_lazy(tpl, 10), sales_price=650,
+        storage_management=False)
+    yield tc10
+    yield Component(parent=tc10, child=devel, qty="10:00")
+
+    tc50 = product(format_lazy(tpl, 50), sales_price=3000,
+        storage_management=False)
+    yield tc50
+    yield Component(parent=tc50, child=devel, qty="50:00")
+
+    FILLERS = Cycler([tc5, tc10, tc50, None])
+
     for i, ref in enumerate(ORDER_REFS):
         obj = COMPANIES.pop()
         eu = PERSONS.pop()
         end_users.append(eu)
         yield rt.models.contacts.Role(person=eu, company=obj)
         sd = dd.today(START_OFFSET+20*i)
         sla = SLA_JNL.create_voucher(
@@ -157,25 +183,36 @@
             ref=ref,
             partner=obj, contact_person=eu,
             subscription_periodicity="y",
             start_date=sd, entry_date=sd)
         yield sla
 
         def add_item(product, qty=None, unit_price=None):
-            i = sla.add_voucher_item(product=product, qty=qty, unit_price=unit_price)
-            # i.product_changed(REQUEST)
-            yield i
+            obj = sla.add_voucher_item(product=product, qty=qty, unit_price=unit_price)
+            # obj.product_changed(REQUEST)
+            yield obj
 
-        yield add_item(sla_hosting, 10)
+        yield add_item(sla_hosting, qty=10)
         yield add_item(sla_maintenance, unit_price=400*i+400, qty=1)
         yield add_item(sla_support, unit_price=500*i+200, qty=1)
 
         sla.register(REQUEST)
         sla.save()
 
+        # This will create the SubscriptionPeriod rows, which will generate
+        # invoices:
+        sla.compute_summary_values()
+
+        Filler = rt.models.storage.Filler
+        yield Filler(partner=obj,
+            provision_product=devel,
+            # filler_product=FILLERS.pop(),
+            storage_state='purchased',
+            min_asset="2:00", fill_asset="10:00")
+
 
     END_USERS = Cycler(end_users)
     ORDERS = Cycler(Subscription.objects.order_by("id"))
 
     for i, ref in enumerate(PROJECT_REFS):
         kw = dict(ref=ref, group=GROUPS.pop(),
             state=SiteStates.active)
@@ -501,7 +538,14 @@
 
 
 def objects():
     yield tickets_objects()
     yield working_objects()
     # yield skills_objects()
     # yield votes_objects()
+
+    from lino_xl.lib.storage.choicelists import StorageStates
+    TransferRule = rt.models.storage.TransferRule
+    sls = rt.models.ledger.Journal.get_by_ref("SLS")
+    srv = rt.models.ledger.Journal.get_by_ref("SRV")
+    yield TransferRule(to_state=StorageStates.purchased, journal=sls)
+    yield TransferRule(from_state=StorageStates.purchased, journal=srv)
```

### Comparing `lino-noi-23.5.0/lino_noi/lib/noi/fixtures/linotickets.py` & `lino-noi-23.7.0/lino_noi/lib/noi/fixtures/linotickets.py`

 * *Files identical despite different names*

### Comparing `lino-noi-23.5.0/lino_noi/lib/noi/help_texts.py` & `lino-noi-23.7.0/lino_noi/lib/noi/help_texts.py`

 * *Files identical despite different names*

### Comparing `lino-noi-23.5.0/lino_noi/lib/noi/layouts.py` & `lino-noi-23.7.0/lino_noi/lib/noi/layouts.py`

 * *Files identical despite different names*

### Comparing `lino-noi-23.5.0/lino_noi/lib/noi/locale/de/LC_MESSAGES/django.mo` & `lino-noi-23.7.0/lino_noi/lib/noi/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `lino-noi-23.5.0/lino_noi/lib/noi/locale/de/LC_MESSAGES/django.po` & `lino-noi-23.7.0/lino_noi/lib/noi/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `lino-noi-23.5.0/lino_noi/lib/noi/locale/et/LC_MESSAGES/django.mo` & `lino-noi-23.7.0/lino_noi/lib/noi/locale/et/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `lino-noi-23.5.0/lino_noi/lib/noi/locale/et/LC_MESSAGES/django.po` & `lino-noi-23.7.0/lino_noi/lib/noi/locale/et/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `lino-noi-23.5.0/lino_noi/lib/noi/locale/fr/LC_MESSAGES/django.po` & `lino-noi-23.7.0/lino_noi/lib/noi/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `lino-noi-23.5.0/lino_noi/lib/noi/migrate.py` & `lino-noi-23.7.0/lino_noi/lib/noi/migrate.py`

 * *Files identical despite different names*

### Comparing `lino-noi-23.5.0/lino_noi/lib/noi/models.py` & `lino-noi-23.7.0/lino_noi/lib/noi/models.py`

 * *Files identical despite different names*

### Comparing `lino-noi-23.5.0/lino_noi/lib/noi/settings.py` & `lino-noi-23.7.0/lino_noi/lib/noi/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 
 class Site(Site):
 
     verbose_name = "Lino Noi"
     description = SETUP_INFO['description']
     version = SETUP_INFO['version']
     url = SETUP_INFO['url']
+    quantity_max_length = 7
     # project_model = 'tickets.Site'
     # 20221214 : in noi we don't want Order to point to Site.
 
 
     demo_fixtures = ['std', 'minimal_ledger', 'demo', 'demo2', 'demo_bookings',
     'checksummaries']  # 'linotickets', 'tractickets', 'luc']
 
@@ -100,14 +101,15 @@
         # yield 'lino_xl.lib.github'
         # yield 'lino.modlib.social_auth'
         yield 'lino_xl.lib.userstats'
         yield 'lino_noi.lib.groups'
 
         yield 'lino_noi.lib.products'
         yield 'lino_noi.lib.sales'
+        yield 'lino_xl.lib.storage'
         # yield 'lino_xl.lib.invoicing'  # no need to mention since subscriptions needs it
         yield 'lino_noi.lib.subscriptions'
 
         if self.has_feature('cms_functionality'):
             yield 'lino_xl.lib.pages'
             yield 'lino.modlib.publisher'
 
@@ -115,14 +117,15 @@
         yield super().get_plugin_configs()
         yield ('help', 'make_help_pages', True)
         yield ('tickets', 'end_user_model', 'contacts.Person')
         yield ('working', 'ticket_model', 'tickets.Ticket')
         # yield ('system', 'use_dashboard_layouts', True)
         yield ('invoicing', 'order_model', 'subscriptions.Subscription')
         yield ('users', 'allow_online_registration', True)
+        yield ('summaries', 'duration_max_length', 10)
 
     # def setup_plugins(self):
     #     super().setup_plugins()
     #     # self.plugins.comments.configure(
     #     #     commentable_model='tickets.Ticket')
     #     # self.plugins.skills.configure(
     #     #     demander_model='tickets.Ticket')
```

### Comparing `lino-noi-23.5.0/lino_noi/lib/noi/user_types.py` & `lino-noi-23.7.0/lino_noi/lib/noi/user_types.py`

 * *Files 13% similar despite different names*

```diff
@@ -22,14 +22,16 @@
 from lino_xl.lib.tickets.roles import Reporter, Searcher, Triager, TicketsStaff
 from lino_xl.lib.working.roles import Worker
 from lino_xl.lib.cal.roles import CalendarReader
 from lino_xl.lib.votes.roles import VotesStaff, VotesUser
 from lino_xl.lib.products.roles import ProductsStaff
 from lino_xl.lib.ledger.roles import LedgerStaff
 from lino_xl.lib.invoicing.roles import InvoicingUser, InvoicingStaff
+from lino_xl.lib.storage.roles import StorageUser, StorageStaff
+
 
 from lino.modlib.users.choicelists import UserTypes
 
 
 class Customer(SiteUser, OfficeUser, VotesUser, Searcher, Reporter, CommentsUser):
     """
     A **Customer** is somebody who uses our software and may report
@@ -52,15 +54,15 @@
     Is able to make service reports as well as manage tickets.
     """
     pass
 
 
 class SiteAdmin(
     SiteAdmin, Developer, OfficeStaff, VotesStaff, ContactsStaff,
-    CommentsStaff, ProductsStaff, LedgerStaff, InvoicingStaff):
+    CommentsStaff, ProductsStaff, LedgerStaff, InvoicingStaff, StorageStaff):
     """
     Can do everything.
     """
 
 
 # class Anonymous(CommentsReader, CalendarReader):
 class Anonymous(CalendarReader, CommentsReader, Searcher):
@@ -71,7 +73,13 @@
 add = UserTypes.add_item
 add('000', _("Anonymous"), Anonymous, 'anonymous',
     readonly=True, authenticated=False)
 add('100', _("Customer"), Customer, 'customer user')
 add('200', _("Contributor"), Contributor, 'contributor')
 add('400', _("Developer"), Developer, 'developer')
 add('900', _("Administrator"), SiteAdmin, 'admin')
+
+
+from lino_xl.lib.storage.choicelists import StorageStates
+StorageStates.clear()
+add = StorageStates.add_item
+add('10', _("Purchased"), 'purchased')
```

### Comparing `lino-noi-23.5.0/lino_noi/lib/public/__init__.py` & `lino-noi-23.7.0/lino_noi/lib/public/__init__.py`

 * *Files identical despite different names*

### Comparing `lino-noi-23.5.0/lino_noi/lib/public/config/noi/tickets.Ticket.html` & `lino-noi-23.7.0/lino_noi/lib/public/config/noi/tickets.Ticket.html`

 * *Files identical despite different names*

### Comparing `lino-noi-23.5.0/lino_noi/lib/public/renderer.py` & `lino-noi-23.7.0/lino_noi/lib/public/renderer.py`

 * *Files identical despite different names*

### Comparing `lino-noi-23.5.0/lino_noi/lib/public/views.py` & `lino-noi-23.7.0/lino_noi/lib/public/views.py`

 * *Files identical despite different names*

### Comparing `lino-noi-23.5.0/lino_noi/lib/sales/config/sales/VatProductInvoice/default.weasy.html` & `lino-noi-23.7.0/lino_noi/lib/sales/config/sales/VatProductInvoice/default.weasy.html`

 * *Files identical despite different names*

### Comparing `lino-noi-23.5.0/lino_noi/lib/sales/models.py` & `lino-noi-23.7.0/lino_noi/lib/sales/models.py`

 * *Files identical despite different names*

### Comparing `lino-noi-23.5.0/lino_noi/lib/tickets/__init__.py` & `lino-noi-23.7.0/lino_noi/lib/tickets/__init__.py`

 * *Files identical despite different names*

### Comparing `lino-noi-23.5.0/lino_noi/lib/tickets/models.py` & `lino-noi-23.7.0/lino_noi/lib/tickets/models.py`

 * *Files identical despite different names*

### Comparing `lino-noi-23.5.0/lino_noi/lib/tickets/workflows.py` & `lino-noi-23.7.0/lino_noi/lib/tickets/workflows.py`

 * *Files identical despite different names*

### Comparing `lino-noi-23.5.0/lino_noi/lib/topics/models.py` & `lino-noi-23.7.0/lino_noi/lib/topics/models.py`

 * *Files identical despite different names*

### Comparing `lino-noi-23.5.0/lino_noi/lib/users/ui.py` & `lino-noi-23.7.0/lino_noi/lib/users/ui.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: UTF-8 -*-
-# Copyright 2015-2021 Rumma & Ko Ltd
+# Copyright 2015-2023 Rumma & Ko Ltd
 # License: GNU Affero General Public License v3 (see file COPYING for details)
 
 """Desktop UI for this plugin.
 
 """
 
 from lino.modlib.users.ui import *
@@ -54,13 +54,13 @@
     email mail_mode
     notify_myself open_session_on_new_ticket
     """
 
     general3 = """
     created:12 modified:12 id
     date_format time_zone
-    #github_username
+    start_date end_date
     """
 
 
 
 # Users.detail_layout = UserDetail()
```

### Comparing `lino-noi-23.5.0/lino_noi/setup_info.py` & `lino-noi-23.7.0/lino_noi/setup_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     # srcref_url='https://gitlab.com/lino-framework/cosi/blob/master/%s',
     intersphinx_urls = dict(
         docs="https://noi.lino-framework.org"))
 
 
 SETUP_INFO = dict(
     name='lino-noi',
-    version='23.5.0',
+    version='23.7.0',
     install_requires=['lino-xl'],
     # tests_require=['pytest', 'mock'],
     test_suite='tests',
     description=("Manage support tickets and working time."),
     long_description="""\
 
 Lino Noi is a customizable ticket management and time tracking
```

### Comparing `lino-noi-23.5.0/lino_noi.egg-info/PKG-INFO` & `lino-noi-23.7.0/lino_noi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lino-noi
-Version: 23.5.0
+Version: 23.7.0
 Summary: Manage support tickets and working time.
 Home-page: https://gitlab.com/lino-framework/noi
 Author: Rumma & Ko Ltd
 Author-email: info@lino-framework.org
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
```

### Comparing `lino-noi-23.5.0/lino_noi.egg-info/SOURCES.txt` & `lino-noi-23.7.0/lino_noi.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -40,14 +40,15 @@
 lino_noi/lib/noi/models.py
 lino_noi/lib/noi/settings.py
 lino_noi/lib/noi/user_types.py
 lino_noi/lib/noi/workflows.py
 lino_noi/lib/noi/fixtures/__init__.py
 lino_noi/lib/noi/fixtures/demo.py
 lino_noi/lib/noi/fixtures/linotickets.py
+lino_noi/lib/noi/fixtures/minimal_ledger.py
 lino_noi/lib/noi/locale/de/LC_MESSAGES/django.mo
 lino_noi/lib/noi/locale/de/LC_MESSAGES/django.po
 lino_noi/lib/noi/locale/et/LC_MESSAGES/django.mo
 lino_noi/lib/noi/locale/et/LC_MESSAGES/django.po
 lino_noi/lib/noi/locale/fr/LC_MESSAGES/django.mo
 lino_noi/lib/noi/locale/fr/LC_MESSAGES/django.po
 lino_noi/lib/products/__init__.py
```

