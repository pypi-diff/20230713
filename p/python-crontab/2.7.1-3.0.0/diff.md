# Comparing `tmp/python-crontab-2.7.1.tar.gz` & `tmp/python-crontab-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-crontab-2.7.1.tar", last modified: Thu Dec 22 04:48:55 2022, max compression
+gzip compressed data, was "python-crontab-3.0.0.tar", last modified: Thu Jul 13 14:53:01 2023, max compression
```

## Comparing `python-crontab-2.7.1.tar` & `python-crontab-3.0.0.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxrwxr-x   0 doctormo  (1000) doctormo  (1000)        0 2022-12-22 04:48:55.191304 python-crontab-2.7.1/
--rw-rw-r--   0 doctormo  (1000) doctormo  (1000)       34 2015-12-28 06:36:10.000000 python-crontab-2.7.1/AUTHORS
--rw-r--r--   0 doctormo  (1000) doctormo  (1000)    14570 2022-12-22 04:33:16.000000 python-crontab-2.7.1/CHANGES.md
--rw-rw-r--   0 doctormo  (1000) doctormo  (1000)     7651 2015-12-28 06:36:10.000000 python-crontab-2.7.1/COPYING
--rw-r--r--   0 doctormo  (1000) doctormo  (1000)      322 2020-03-23 16:32:58.000000 python-crontab-2.7.1/MANIFEST.in
--rw-rw-r--   0 doctormo  (1000) doctormo  (1000)    15500 2022-12-22 04:48:55.191304 python-crontab-2.7.1/PKG-INFO
--rw-rw-r--   0 doctormo  (1000) doctormo  (1000)    14273 2022-12-22 04:32:19.000000 python-crontab-2.7.1/README.rst
--rw-rw-r--   0 doctormo  (1000) doctormo  (1000)     3773 2022-12-22 04:41:54.000000 python-crontab-2.7.1/cronlog.py
--rw-rw-r--   0 doctormo  (1000) doctormo  (1000)    46862 2022-12-22 04:43:07.000000 python-crontab-2.7.1/crontab.py
--rw-rw-r--   0 doctormo  (1000) doctormo  (1000)     4438 2015-12-28 22:23:00.000000 python-crontab-2.7.1/crontabs.py
-drwxrwxr-x   0 doctormo  (1000) doctormo  (1000)        0 2022-12-22 04:48:55.187303 python-crontab-2.7.1/python_crontab.egg-info/
--rw-rw-r--   0 doctormo  (1000) doctormo  (1000)    15500 2022-12-22 04:48:55.000000 python-crontab-2.7.1/python_crontab.egg-info/PKG-INFO
--rw-rw-r--   0 doctormo  (1000) doctormo  (1000)     1118 2022-12-22 04:48:55.000000 python-crontab-2.7.1/python_crontab.egg-info/SOURCES.txt
--rw-rw-r--   0 doctormo  (1000) doctormo  (1000)        1 2022-12-22 04:48:55.000000 python-crontab-2.7.1/python_crontab.egg-info/dependency_links.txt
--rw-rw-r--   0 doctormo  (1000) doctormo  (1000)       78 2022-12-22 04:48:55.000000 python-crontab-2.7.1/python_crontab.egg-info/requires.txt
--rw-rw-r--   0 doctormo  (1000) doctormo  (1000)       25 2022-12-22 04:48:55.000000 python-crontab-2.7.1/python_crontab.egg-info/top_level.txt
--rw-rw-r--   0 doctormo  (1000) doctormo  (1000)       38 2022-12-22 04:48:55.191304 python-crontab-2.7.1/setup.cfg
--rwxrwxr-x   0 doctormo  (1000) doctormo  (1000)     2891 2022-12-22 04:20:28.000000 python-crontab-2.7.1/setup.py
-drwxrwxr-x   0 doctormo  (1000) doctormo  (1000)        0 2022-12-22 04:48:55.191304 python-crontab-2.7.1/tests/
--rw-rw-r--   0 doctormo  (1000) doctormo  (1000)        1 2015-12-29 21:09:18.000000 python-crontab-2.7.1/tests/__init__.py
-drwxrwxr-x   0 doctormo  (1000) doctormo  (1000)        0 2022-12-22 04:48:55.191304 python-crontab-2.7.1/tests/data/
-drwxrwxr-x   0 doctormo  (1000) doctormo  (1000)        0 2022-12-22 04:48:55.191304 python-crontab-2.7.1/tests/data/anacron/
--rwxr-xr-x   0 doctormo  (1000) doctormo  (1000)        0 2015-12-28 21:48:51.000000 python-crontab-2.7.1/tests/data/anacron/an_command.sh
--rw-rw-r--   0 doctormo  (1000) doctormo  (1000)        0 2015-12-28 21:49:06.000000 python-crontab-2.7.1/tests/data/anacron/not_command.txt
--rw-rw-r--   0 doctormo  (1000) doctormo  (1000)      108 2015-12-28 06:36:10.000000 python-crontab-2.7.1/tests/data/basic.log
--rw-rw-r--   0 doctormo  (1000) doctormo  (1000)       49 2015-12-28 18:57:24.000000 python-crontab-2.7.1/tests/data/crontab
-drwxrwxr-x   0 doctormo  (1000) doctormo  (1000)        0 2022-12-22 04:48:55.191304 python-crontab-2.7.1/tests/data/crontabs/
--rw-rw-r--   0 doctormo  (1000) doctormo  (1000)        0 2015-12-28 21:47:03.000000 python-crontab-2.7.1/tests/data/crontabs/.empty
--rw-rw-r--   0 doctormo  (1000) doctormo  (1000)       50 2015-12-28 18:17:28.000000 python-crontab-2.7.1/tests/data/crontabs/system_one
--rw-rw-r--   0 doctormo  (1000) doctormo  (1000)       28 2015-12-28 18:44:58.000000 python-crontab-2.7.1/tests/data/crontabs/system_two
--rwxrwxr-x   0 doctormo  (1000) doctormo  (1000)     1366 2022-12-22 04:30:31.000000 python-crontab-2.7.1/tests/data/crontest
--rw-rw-r--   0 doctormo  (1000) doctormo  (1000)       50 2015-12-28 06:36:10.000000 python-crontab-2.7.1/tests/data/specials.tab
--rw-rw-r--   0 doctormo  (1000) doctormo  (1000)       77 2015-12-28 06:36:10.000000 python-crontab-2.7.1/tests/data/specials_enc.tab
-drwxrwxr-x   0 doctormo  (1000) doctormo  (1000)        0 2022-12-22 04:48:55.191304 python-crontab-2.7.1/tests/data/spool/
--rw-rw-r--   0 doctormo  (1000) doctormo  (1000)       23 2015-12-28 06:36:10.000000 python-crontab-2.7.1/tests/data/spool/basic
--rw-rw-r--   0 doctormo  (1000) doctormo  (1000)       82 2015-12-28 19:06:04.000000 python-crontab-2.7.1/tests/data/spool/hgreen
--rw-rw-r--   0 doctormo  (1000) doctormo  (1000)       79 2015-12-28 19:03:15.000000 python-crontab-2.7.1/tests/data/spool/jgreen
--rw-rw-r--   0 doctormo  (1000) doctormo  (1000)       42 2015-12-28 06:36:10.000000 python-crontab-2.7.1/tests/data/spool/user
--rw-rw-r--   0 doctormo  (1000) doctormo  (1000)     2409 2015-12-28 06:36:10.000000 python-crontab-2.7.1/tests/data/test.log
--rw-rw-r--   0 doctormo  (1000) doctormo  (1000)      470 2020-05-15 23:43:15.000000 python-crontab-2.7.1/tests/data/test.tab
--rw-r--r--   0 doctormo  (1000) doctormo  (1000)     4246 2020-05-17 17:13:48.000000 python-crontab-2.7.1/tests/test_compatibility.py
--rw-r--r--   0 doctormo  (1000) doctormo  (1000)     2059 2020-01-27 06:39:48.000000 python-crontab-2.7.1/tests/test_context.py
--rw-rw-r--   0 doctormo  (1000) doctormo  (1000)     2906 2015-12-28 06:36:10.000000 python-crontab-2.7.1/tests/test_croniter.py
--rw-rw-r--   0 doctormo  (1000) doctormo  (1000)     3815 2021-10-19 20:14:53.000000 python-crontab-2.7.1/tests/test_crontabs.py
--rw-rw-r--   0 doctormo  (1000) doctormo  (1000)     2041 2016-06-11 20:45:16.000000 python-crontab-2.7.1/tests/test_description.py
--rw-rw-r--   0 doctormo  (1000) doctormo  (1000)     3600 2016-12-12 16:26:39.000000 python-crontab-2.7.1/tests/test_enums.py
--rw-rw-r--   0 doctormo  (1000) doctormo  (1000)     6184 2018-05-08 19:50:48.000000 python-crontab-2.7.1/tests/test_env.py
--rwxr-xr-x   0 doctormo  (1000) doctormo  (1000)     2078 2020-01-27 07:25:15.000000 python-crontab-2.7.1/tests/test_equality.py
--rw-rw-r--   0 doctormo  (1000) doctormo  (1000)     3402 2022-12-22 04:40:59.000000 python-crontab-2.7.1/tests/test_every.py
--rw-rw-r--   0 doctormo  (1000) doctormo  (1000)     5439 2022-12-22 04:40:45.000000 python-crontab-2.7.1/tests/test_frequency.py
--rw-rw-r--   0 doctormo  (1000) doctormo  (1000)    13878 2022-12-22 04:47:17.000000 python-crontab-2.7.1/tests/test_interaction.py
--rw-rw-r--   0 doctormo  (1000) doctormo  (1000)     5603 2015-12-31 05:53:07.000000 python-crontab-2.7.1/tests/test_log.py
--rw-rw-r--   0 doctormo  (1000) doctormo  (1000)     4721 2022-12-22 04:39:45.000000 python-crontab-2.7.1/tests/test_range.py
--rw-rw-r--   0 doctormo  (1000) doctormo  (1000)     5103 2022-12-22 04:39:23.000000 python-crontab-2.7.1/tests/test_removal.py
--rw-rw-r--   0 doctormo  (1000) doctormo  (1000)     3378 2018-05-08 20:36:43.000000 python-crontab-2.7.1/tests/test_scheduler.py
--rw-rw-r--   0 doctormo  (1000) doctormo  (1000)     4123 2019-01-03 16:19:25.000000 python-crontab-2.7.1/tests/test_system_cron.py
--rw-rw-r--   0 doctormo  (1000) doctormo  (1000)     9170 2022-12-22 04:45:50.000000 python-crontab-2.7.1/tests/test_usage.py
--rw-rw-r--   0 doctormo  (1000) doctormo  (1000)     3651 2022-12-22 04:38:56.000000 python-crontab-2.7.1/tests/test_utf8.py
--rw-r--r--   0 doctormo  (1000) doctormo  (1000)     2831 2018-05-25 14:54:01.000000 python-crontab-2.7.1/tests/utils.py
+drwxrwxr-x   0 doctormo  (1000) doctormo  (1000)        0 2023-07-13 14:53:01.829805 python-crontab-3.0.0/
+-rw-rw-r--   0 doctormo  (1000) doctormo  (1000)       34 2015-12-28 06:36:10.000000 python-crontab-3.0.0/AUTHORS
+-rw-r--r--   0 doctormo  (1000) doctormo  (1000)    14570 2022-12-22 04:33:16.000000 python-crontab-3.0.0/CHANGES.md
+-rw-rw-r--   0 doctormo  (1000) doctormo  (1000)     7651 2015-12-28 06:36:10.000000 python-crontab-3.0.0/COPYING
+-rw-r--r--   0 doctormo  (1000) doctormo  (1000)      322 2020-03-23 16:32:58.000000 python-crontab-3.0.0/MANIFEST.in
+-rw-rw-r--   0 doctormo  (1000) doctormo  (1000)    17141 2023-07-13 14:53:01.829805 python-crontab-3.0.0/PKG-INFO
+-rw-rw-r--   0 doctormo  (1000) doctormo  (1000)    15879 2023-07-13 14:51:49.000000 python-crontab-3.0.0/README.rst
+-rw-rw-r--   0 doctormo  (1000) doctormo  (1000)     3773 2022-12-22 04:41:54.000000 python-crontab-3.0.0/cronlog.py
+-rw-rw-r--   0 doctormo  (1000) doctormo  (1000)    51493 2023-07-13 13:57:37.000000 python-crontab-3.0.0/crontab.py
+-rw-rw-r--   0 doctormo  (1000) doctormo  (1000)     4438 2015-12-28 22:23:00.000000 python-crontab-3.0.0/crontabs.py
+drwxrwxr-x   0 doctormo  (1000) doctormo  (1000)        0 2023-07-13 14:53:01.825805 python-crontab-3.0.0/python_crontab.egg-info/
+-rw-rw-r--   0 doctormo  (1000) doctormo  (1000)    17141 2023-07-13 14:53:01.000000 python-crontab-3.0.0/python_crontab.egg-info/PKG-INFO
+-rw-rw-r--   0 doctormo  (1000) doctormo  (1000)     1118 2023-07-13 14:53:01.000000 python-crontab-3.0.0/python_crontab.egg-info/SOURCES.txt
+-rw-rw-r--   0 doctormo  (1000) doctormo  (1000)        1 2023-07-13 14:53:01.000000 python-crontab-3.0.0/python_crontab.egg-info/dependency_links.txt
+-rw-rw-r--   0 doctormo  (1000) doctormo  (1000)       78 2023-07-13 14:53:01.000000 python-crontab-3.0.0/python_crontab.egg-info/requires.txt
+-rw-rw-r--   0 doctormo  (1000) doctormo  (1000)       25 2023-07-13 14:53:01.000000 python-crontab-3.0.0/python_crontab.egg-info/top_level.txt
+-rw-rw-r--   0 doctormo  (1000) doctormo  (1000)       38 2023-07-13 14:53:01.829805 python-crontab-3.0.0/setup.cfg
+-rwxrwxr-x   0 doctormo  (1000) doctormo  (1000)     2941 2023-07-13 14:52:41.000000 python-crontab-3.0.0/setup.py
+drwxrwxr-x   0 doctormo  (1000) doctormo  (1000)        0 2023-07-13 14:53:01.829805 python-crontab-3.0.0/tests/
+-rw-rw-r--   0 doctormo  (1000) doctormo  (1000)        1 2015-12-29 21:09:18.000000 python-crontab-3.0.0/tests/__init__.py
+drwxrwxr-x   0 doctormo  (1000) doctormo  (1000)        0 2023-07-13 14:53:01.829805 python-crontab-3.0.0/tests/data/
+drwxrwxr-x   0 doctormo  (1000) doctormo  (1000)        0 2023-07-13 14:53:01.829805 python-crontab-3.0.0/tests/data/anacron/
+-rwxr-xr-x   0 doctormo  (1000) doctormo  (1000)        0 2015-12-28 21:48:51.000000 python-crontab-3.0.0/tests/data/anacron/an_command.sh
+-rw-rw-r--   0 doctormo  (1000) doctormo  (1000)        0 2015-12-28 21:49:06.000000 python-crontab-3.0.0/tests/data/anacron/not_command.txt
+-rw-rw-r--   0 doctormo  (1000) doctormo  (1000)      108 2015-12-28 06:36:10.000000 python-crontab-3.0.0/tests/data/basic.log
+-rw-rw-r--   0 doctormo  (1000) doctormo  (1000)       49 2015-12-28 18:57:24.000000 python-crontab-3.0.0/tests/data/crontab
+drwxrwxr-x   0 doctormo  (1000) doctormo  (1000)        0 2023-07-13 14:53:01.829805 python-crontab-3.0.0/tests/data/crontabs/
+-rw-rw-r--   0 doctormo  (1000) doctormo  (1000)        0 2015-12-28 21:47:03.000000 python-crontab-3.0.0/tests/data/crontabs/.empty
+-rw-rw-r--   0 doctormo  (1000) doctormo  (1000)       50 2015-12-28 18:17:28.000000 python-crontab-3.0.0/tests/data/crontabs/system_one
+-rw-rw-r--   0 doctormo  (1000) doctormo  (1000)       28 2015-12-28 18:44:58.000000 python-crontab-3.0.0/tests/data/crontabs/system_two
+-rwxrwxr-x   0 doctormo  (1000) doctormo  (1000)     1366 2022-12-22 04:30:31.000000 python-crontab-3.0.0/tests/data/crontest
+-rw-rw-r--   0 doctormo  (1000) doctormo  (1000)       50 2015-12-28 06:36:10.000000 python-crontab-3.0.0/tests/data/specials.tab
+-rw-rw-r--   0 doctormo  (1000) doctormo  (1000)       77 2015-12-28 06:36:10.000000 python-crontab-3.0.0/tests/data/specials_enc.tab
+drwxrwxr-x   0 doctormo  (1000) doctormo  (1000)        0 2023-07-13 14:53:01.829805 python-crontab-3.0.0/tests/data/spool/
+-rw-rw-r--   0 doctormo  (1000) doctormo  (1000)       23 2015-12-28 06:36:10.000000 python-crontab-3.0.0/tests/data/spool/basic
+-rw-rw-r--   0 doctormo  (1000) doctormo  (1000)       82 2015-12-28 19:06:04.000000 python-crontab-3.0.0/tests/data/spool/hgreen
+-rw-rw-r--   0 doctormo  (1000) doctormo  (1000)       79 2015-12-28 19:03:15.000000 python-crontab-3.0.0/tests/data/spool/jgreen
+-rw-rw-r--   0 doctormo  (1000) doctormo  (1000)       42 2015-12-28 06:36:10.000000 python-crontab-3.0.0/tests/data/spool/user
+-rw-rw-r--   0 doctormo  (1000) doctormo  (1000)     2409 2015-12-28 06:36:10.000000 python-crontab-3.0.0/tests/data/test.log
+-rw-rw-r--   0 doctormo  (1000) doctormo  (1000)      470 2020-05-15 23:43:15.000000 python-crontab-3.0.0/tests/data/test.tab
+-rw-r--r--   0 doctormo  (1000) doctormo  (1000)     4249 2023-07-13 13:44:06.000000 python-crontab-3.0.0/tests/test_compatibility.py
+-rw-r--r--   0 doctormo  (1000) doctormo  (1000)     2059 2020-01-27 06:39:48.000000 python-crontab-3.0.0/tests/test_context.py
+-rw-rw-r--   0 doctormo  (1000) doctormo  (1000)     2906 2015-12-28 06:36:10.000000 python-crontab-3.0.0/tests/test_croniter.py
+-rw-rw-r--   0 doctormo  (1000) doctormo  (1000)     3815 2021-10-19 20:14:53.000000 python-crontab-3.0.0/tests/test_crontabs.py
+-rw-rw-r--   0 doctormo  (1000) doctormo  (1000)     2041 2016-06-11 20:45:16.000000 python-crontab-3.0.0/tests/test_description.py
+-rw-rw-r--   0 doctormo  (1000) doctormo  (1000)     3600 2016-12-12 16:26:39.000000 python-crontab-3.0.0/tests/test_enums.py
+-rw-rw-r--   0 doctormo  (1000) doctormo  (1000)     6184 2018-05-08 19:50:48.000000 python-crontab-3.0.0/tests/test_env.py
+-rwxr-xr-x   0 doctormo  (1000) doctormo  (1000)     2078 2020-01-27 07:25:15.000000 python-crontab-3.0.0/tests/test_equality.py
+-rw-rw-r--   0 doctormo  (1000) doctormo  (1000)     3402 2022-12-22 04:40:59.000000 python-crontab-3.0.0/tests/test_every.py
+-rw-rw-r--   0 doctormo  (1000) doctormo  (1000)     7052 2022-12-31 19:51:32.000000 python-crontab-3.0.0/tests/test_frequency.py
+-rw-rw-r--   0 doctormo  (1000) doctormo  (1000)    13878 2022-12-22 04:47:17.000000 python-crontab-3.0.0/tests/test_interaction.py
+-rw-rw-r--   0 doctormo  (1000) doctormo  (1000)     5603 2015-12-31 05:53:07.000000 python-crontab-3.0.0/tests/test_log.py
+-rw-rw-r--   0 doctormo  (1000) doctormo  (1000)     4721 2022-12-22 04:39:45.000000 python-crontab-3.0.0/tests/test_range.py
+-rw-rw-r--   0 doctormo  (1000) doctormo  (1000)     5103 2022-12-22 04:39:23.000000 python-crontab-3.0.0/tests/test_removal.py
+-rw-rw-r--   0 doctormo  (1000) doctormo  (1000)     3378 2022-12-31 19:59:46.000000 python-crontab-3.0.0/tests/test_scheduler.py
+-rw-rw-r--   0 doctormo  (1000) doctormo  (1000)     4123 2019-01-03 16:19:25.000000 python-crontab-3.0.0/tests/test_system_cron.py
+-rw-rw-r--   0 doctormo  (1000) doctormo  (1000)     9251 2023-07-13 14:00:42.000000 python-crontab-3.0.0/tests/test_usage.py
+-rw-rw-r--   0 doctormo  (1000) doctormo  (1000)     3651 2022-12-22 04:38:56.000000 python-crontab-3.0.0/tests/test_utf8.py
+-rw-r--r--   0 doctormo  (1000) doctormo  (1000)     2831 2018-05-25 14:54:01.000000 python-crontab-3.0.0/tests/utils.py
```

### Comparing `python-crontab-2.7.1/CHANGES.md` & `python-crontab-3.0.0/CHANGES.md`

 * *Files identical despite different names*

### Comparing `python-crontab-2.7.1/COPYING` & `python-crontab-3.0.0/COPYING`

 * *Files identical despite different names*

### Comparing `python-crontab-2.7.1/PKG-INFO` & `python-crontab-3.0.0/README.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,40 +1,7 @@
-Metadata-Version: 2.1
-Name: python-crontab
-Version: 2.7.1
-Summary: Python Crontab API
-Home-page: https://gitlab.com/doctormo/python-crontab/
-Author: Martin Owens
-Author-email: doctormo@gmail.com
-License: LGPLv3
-Platform: linux
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Development Status :: 6 - Mature
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Information Technology
-Classifier: Intended Audience :: System Administrators
-Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
-Classifier: Operating System :: POSIX
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Operating System :: POSIX :: SunOS/Solaris
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Provides: crontab
-Provides: crontabs
-Provides: cronlog
-Provides-Extra: cron-description
-Provides-Extra: cron-schedule
-License-File: COPYING
-License-File: AUTHORS
-
 Python Crontab
 --------------
 
 .. image:: https://gitlab.com/doctormo/python-crontab/raw/master/branding.svg
 
 .. image:: https://badge.fury.io/py/python-crontab.svg
     :target: https://badge.fury.io/py/python-crontab
@@ -341,15 +308,17 @@
 
 (note this functionality is new and not perfect, if you find bugs report them!)
 
 Running the scheduler::
 
     tab = CronTab(tabfile='MyScripts.tab')
     for result in tab.run_scheduler():
-        print("This was printed to stdout by the process.")
+        print("Return code: {result.returncode}")
+        print("Standard Out: {result.stdout}")
+        print("Standard Err: {result.stderr}")
 
 Do not do this, it won't work because it returns generator function::
 
     tab.run_scheduler()
 
 Timeout and cadence can be changed for testing or error management::
 
@@ -357,23 +326,28 @@
         print("Will run jobs every 1 minutes for ten minutes from now()")
 
     for result in tab.run_scheduler(cadence=1, warp=True):
         print("Will run jobs every 1 second, counting each second as 1 minute")
 
 Frequency Calculation
 =====================
-
 Every job's schedule has a frequency. We can attempt to calculate the number
-of times a job would execute in a give amount of time. We have three simple
-methods::
+of times a job would execute in a give amount of time. We have two variants
+`frequency_per_*` and `frequency_at_*` calculations. The `freqency_at_*` 
+always returnes *times* a job would execute and is aware of leap years.
+
+
+`frequency_per_*`
+-----------------
+For `frequency_per_*` We have three simple methods::
 
     job.setall("1,2 1,2 * * *")
     job.frequency_per_day() == 4
 
-The per year frequency method will tell you how many days a year the
+The per year frequency method will tell you how many **days** a year the
 job would execute::
 
     job.setall("* * 1,2 1,2 *")
     job.frequency_per_year(year=2010) == 4
 
 These are combined to give the number of times a job will execute in any year::
 
@@ -382,14 +356,51 @@
 
 Frequency can be quickly checked using python built-in operators::
 
     job < "*/2 * * * *"
     job > job2
     job.slices == "*/5"
 
+
+`frequency_at_*`
+----------------
+For `frequency_at_*` We have four simple methods.
+
+The at per hour frequency method will tell you how many times the job would
+execute at a given hour::
+
+    job.setall("*/2 0 * * *")
+    job.frequency_at_hour() == 30
+    job.frequency_at_hour(year=2010, month=1, day=1, hour=0) == 30  # even hour 
+    job.frequency_at_hour(year=2010, month=1, day=1, hour=1) == 0   # odd hour
+
+The at day frequency method parameterized tells you how many times the job
+would execute at a given day::
+
+    job.setall("0 0 * * 1,2")
+    job.frequency_at_day(year=2010, month=1, day=18) == 24 # Mon Jan 18th 2020
+    job.frequency_at_day(year=2010, month=1, day=21) == 0  # Thu Jan 21th 2020
+
+The at month frequency method will tell you how many times the job would
+execute at a given month::
+
+    job.setall("0 0 * * *")
+    job.frequency_at_month() == <output_of_current_month>
+    job.frequency_at_month(year=2010, month=1) == 31
+    job.frequency_at_month(year=2010, month=2) == 28
+    job.frequency_at_month(year=2012, month=2) == 29  # leap year
+
+The at year frequency method will tell you how many times a year the
+job would execute::
+
+    job.setall("* * 3,29 2 *")
+    job.frequency_at_year(year=2021) == 24
+    job.frequency_at_year(year=2024) == 48  # leap year
+
+
 Log Functionality
 =================
 
 The log functionality will read a cron log backwards to find you the last run
 instances of your crontab and cron jobs.
 
 The crontab will limit the returned entries to the user the crontab is for::
@@ -468,9 +479,7 @@
  - Customise the location of the crontab command by setting the global CRON_COMMAND
    or the per-object cron_command attribute.
  - Support for vixie cron with username addition with user flag
  - Support for SunOS, AIX & HP with compatibility 'SystemV' mode.
  - Python 3 (3.7, 3.8, 3.10) tested, python 2.6, 2.7 removed from support.
  - Windows support works for non-system crontabs only.
    ( see mem_cron and file_cron examples above for usage )
-
-
```

### Comparing `python-crontab-2.7.1/README.rst` & `python-crontab-3.0.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,41 @@
+Metadata-Version: 2.1
+Name: python-crontab
+Version: 3.0.0
+Summary: Python Crontab API
+Home-page: https://gitlab.com/doctormo/python-crontab/
+Author: Martin Owens
+Author-email: doctormo@gmail.com
+License: LGPLv3
+Platform: linux
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Development Status :: 6 - Mature
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Information Technology
+Classifier: Intended Audience :: System Administrators
+Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
+Classifier: Operating System :: POSIX
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Operating System :: POSIX :: SunOS/Solaris
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Provides: crontab
+Provides: crontabs
+Provides: cronlog
+Description-Content-Type: text/x-rst
+Provides-Extra: cron-schedule
+Provides-Extra: cron-description
+License-File: COPYING
+License-File: AUTHORS
+
 Python Crontab
 --------------
 
 .. image:: https://gitlab.com/doctormo/python-crontab/raw/master/branding.svg
 
 .. image:: https://badge.fury.io/py/python-crontab.svg
     :target: https://badge.fury.io/py/python-crontab
@@ -308,15 +342,17 @@
 
 (note this functionality is new and not perfect, if you find bugs report them!)
 
 Running the scheduler::
 
     tab = CronTab(tabfile='MyScripts.tab')
     for result in tab.run_scheduler():
-        print("This was printed to stdout by the process.")
+        print("Return code: {result.returncode}")
+        print("Standard Out: {result.stdout}")
+        print("Standard Err: {result.stderr}")
 
 Do not do this, it won't work because it returns generator function::
 
     tab.run_scheduler()
 
 Timeout and cadence can be changed for testing or error management::
 
@@ -324,23 +360,28 @@
         print("Will run jobs every 1 minutes for ten minutes from now()")
 
     for result in tab.run_scheduler(cadence=1, warp=True):
         print("Will run jobs every 1 second, counting each second as 1 minute")
 
 Frequency Calculation
 =====================
-
 Every job's schedule has a frequency. We can attempt to calculate the number
-of times a job would execute in a give amount of time. We have three simple
-methods::
+of times a job would execute in a give amount of time. We have two variants
+`frequency_per_*` and `frequency_at_*` calculations. The `freqency_at_*` 
+always returnes *times* a job would execute and is aware of leap years.
+
+
+`frequency_per_*`
+-----------------
+For `frequency_per_*` We have three simple methods::
 
     job.setall("1,2 1,2 * * *")
     job.frequency_per_day() == 4
 
-The per year frequency method will tell you how many days a year the
+The per year frequency method will tell you how many **days** a year the
 job would execute::
 
     job.setall("* * 1,2 1,2 *")
     job.frequency_per_year(year=2010) == 4
 
 These are combined to give the number of times a job will execute in any year::
 
@@ -349,14 +390,51 @@
 
 Frequency can be quickly checked using python built-in operators::
 
     job < "*/2 * * * *"
     job > job2
     job.slices == "*/5"
 
+
+`frequency_at_*`
+----------------
+For `frequency_at_*` We have four simple methods.
+
+The at per hour frequency method will tell you how many times the job would
+execute at a given hour::
+
+    job.setall("*/2 0 * * *")
+    job.frequency_at_hour() == 30
+    job.frequency_at_hour(year=2010, month=1, day=1, hour=0) == 30  # even hour 
+    job.frequency_at_hour(year=2010, month=1, day=1, hour=1) == 0   # odd hour
+
+The at day frequency method parameterized tells you how many times the job
+would execute at a given day::
+
+    job.setall("0 0 * * 1,2")
+    job.frequency_at_day(year=2010, month=1, day=18) == 24 # Mon Jan 18th 2020
+    job.frequency_at_day(year=2010, month=1, day=21) == 0  # Thu Jan 21th 2020
+
+The at month frequency method will tell you how many times the job would
+execute at a given month::
+
+    job.setall("0 0 * * *")
+    job.frequency_at_month() == <output_of_current_month>
+    job.frequency_at_month(year=2010, month=1) == 31
+    job.frequency_at_month(year=2010, month=2) == 28
+    job.frequency_at_month(year=2012, month=2) == 29  # leap year
+
+The at year frequency method will tell you how many times a year the
+job would execute::
+
+    job.setall("* * 3,29 2 *")
+    job.frequency_at_year(year=2021) == 24
+    job.frequency_at_year(year=2024) == 48  # leap year
+
+
 Log Functionality
 =================
 
 The log functionality will read a cron log backwards to find you the last run
 instances of your crontab and cron jobs.
 
 The crontab will limit the returned entries to the user the crontab is for::
```

### Comparing `python-crontab-2.7.1/cronlog.py` & `python-crontab-3.0.0/cronlog.py`

 * *Files identical despite different names*

### Comparing `python-crontab-2.7.1/crontab.py` & `python-crontab-3.0.0/crontab.py`

 * *Files 7% similar despite different names*

```diff
@@ -89,20 +89,21 @@
 import types
 import codecs
 import logging
 import tempfile
 import platform
 import subprocess as sp
 
+from calendar import monthrange
 from time import sleep
 from datetime import time, date, datetime, timedelta
 from collections import OrderedDict
 
 __pkgname__ = 'python-crontab'
-__version__ = '2.7.1'
+__version__ = '3.0.0'
 
 ITEMREX = re.compile(r'^\s*([^@#\s]+)\s+([^@#\s]+)\s+([^@#\s]+)\s+([^@#\s]+)'
                      r'\s+([^@#\s]+)\s+([^\n]*?)(\s+#\s*([^\n]*)|$)')
 SPECREX = re.compile(r'^\s*@(\w+)\s([^#\n]*)(\s+#\s*([^\n]*)|$)')
 DEVNULL = ">/dev/null 2>&1"
 
 WEEK_ENUM = ['sun', 'mon', 'tue', 'wed', 'thu', 'fri', 'sat', 'sun']
@@ -154,38 +155,69 @@
 current_user = lambda: None
 if not WINOS:
     import pwd
     def current_user():
         """Returns the username of the current user"""
         return pwd.getpwuid(os.getuid())[0]
 
-def open_pipe(cmd, *args, **flags):
-    """Runs a program and orders the arguments for compatability.
-
-    a. keyword args are flags and always appear /before/ arguments for bsd
-    """
-    cmd_args = tuple(shlex.split(cmd, posix=flags.pop('posix', POSIX)))
-    env = flags.pop('env', None)
-    for (key, value) in flags.items():
-        if len(key) == 1:
-            cmd_args += (("-%s" % key),)
-            if value is not None:
-                cmd_args += (str(value),)
-        else:
-            cmd_args += (("--%s=%s" % (key, value)),)
-    args = tuple(arg for arg in (cmd_args + tuple(args)) if arg)
-    return sp.Popen(args, stdout=sp.PIPE, stderr=sp.PIPE, env=env)
 
 def _str(text):
     """Convert to the best string format for this python version"""
     if isinstance(text, bytes):
         return text.decode('utf-8')
     return text
 
 
+class Process:
+    """Runs a program and orders the arguments for compatability.
+
+    a. keyword args are flags and always appear /before/ arguments for bsd
+    """
+    def __init__(self, cmd, *args, **flags):
+        cmd_args = tuple(shlex.split(cmd, posix=flags.pop('posix', POSIX)))
+        self.env = flags.pop('env', None)
+        for (key, value) in flags.items():
+            if len(key) == 1:
+                cmd_args += (f"-{key}",)
+                if value is not None:
+                    cmd_args += (str(value),)
+            else:
+                cmd_args += (f"--{key}={value}",)
+        self.args = tuple(arg for arg in (cmd_args + tuple(args)) if arg)
+        self.has_run = False
+        self.stdout = None
+        self.stderr = None
+        self.returncode = None
+
+    def _run(self):
+        """Run this process and return the popen process object"""
+        return sp.Popen(self.args, stdout=sp.PIPE, stderr=sp.PIPE, env=self.env)
+
+    def run(self):
+        """Run this process and store whatever is returned"""
+        process = self._run()
+        (out, err) = process.communicate()
+        self.returncode = process.returncode
+        self.stdout = out.decode("utf-8")
+        self.stderr = err.decode("utf-8")
+        return self
+
+    def __str__(self):
+        return self.stdout.strip()
+
+    def __repr__(self):
+        return f"Process({self.args})"
+
+    def __int__(self):
+        return self.returncode
+
+    def __eq__(self, other):
+        return str(self) == other
+
+
 class CronTab:
     """
     Crontab object which can access any time based cron using the standard.
 
     user    - Set the user of the crontab (default: None)
       * 'user' = Load from $username's crontab (instead of tab or tabfile)
       * None   = Don't load anything from any user crontab.
@@ -248,15 +280,15 @@
         """Catch setting crons and lines directly"""
         if name == 'lines' and value:
             for line in value:
                 self.append(CronItem.from_line(line, cron=self), line, read=True)
         elif name == 'crons' and value:
             raise AttributeError("You can NOT set crons attribute directly")
         else:
-            super(CronTab, self).__setattr__(name, value)
+            super().__setattr__(name, value)
 
     def read(self, filename=None):
         """
         Read in the crontab from the system into the object, called
         automatically when listing or using the object. use for refresh.
         """
         self.crons = []
@@ -269,20 +301,18 @@
 
         elif filename:
             self.filen = filename
             with codecs.open(filename, 'r', encoding='utf-8') as fhl:
                 lines = fhl.readlines()
 
         elif self.user:
-            (out, err) = open_pipe(self.cron_command, l='', **self.user_opt).communicate()
-            if err and 'no crontab for' in str(err):
-                pass
-            elif err:
-                raise IOError("Read crontab %s: %s" % (self.user, err))
-            lines = out.decode('utf-8').split("\n")
+            process = Process(self.cron_command, l='', **self.user_opt).run()
+            if process.stderr and 'no crontab for' not in process.stderr:
+                raise IOError(f"Read crontab {self.user}: {process.stderr}")
+            lines = process.stdout.split("\n")
 
         self.lines = lines
 
     def append(self, item, line='', read=False, before=None):
         """Append a CronItem object to this CronTab
 
         Keyword arguments:
@@ -301,16 +331,16 @@
             if isinstance(before, (list, tuple, types.GeneratorType)):
                 *_, before = before
 
             if before is not None:
                 cron_id = self.crons.index(before)
                 line_id = self.lines.index(before)
 
-        except ValueError:
-            raise ValueError("Can not find CronItem in crontab to insert before")
+        except ValueError as err:
+            raise ValueError("Can not find CronItem in crontab to insert before") from err
 
         if item.is_valid():
             item.env.update(self._parked_env)
             self._parked_env = OrderedDict()
             if read and not item.comment and self.lines and \
               self.lines[-1] and self.lines[-1][0] == '#':
                 item.set_comment(self.lines.pop()[1:].strip(), True)
@@ -345,33 +375,33 @@
         if self.intab is not None:
             self.intab = self.render()
             # And that's it if we never saved to a file
             if not self.filen:
                 return
 
         if self.filen:
-            fileh = open(self.filen, 'wb')
+            fileh = open(self.filen, 'wb') # pylint: disable=consider-using-with
         else:
             filed, path = tempfile.mkstemp()
             fileh = os.fdopen(filed, 'wb')
 
         fileh.write(self.render(errors=errors).encode('utf-8'))
         fileh.close()
 
         if not self.filen:
             # Add the entire crontab back to the user crontab
             if not self.user:
                 os.unlink(path)
                 raise IOError("Please specify user or filename to write.")
 
-            proc = open_pipe(self.cron_command, path, **self.user_opt)
+            proc = Process(self.cron_command, path, **self.user_opt)._run()
             ret = proc.wait()
             if ret != 0:
-                raise IOError("Program Error: {} returned {}: {}".format(
-                    self.cron_command, ret, proc.stderr.read()))
+                msg = proc.stderr.read()
+                raise IOError(f"Program Error: {self.cron_command} returned {ret}: {msg}")
             proc.stdout.close()
             proc.stderr.close()
             os.unlink(path)
 
     def write_to_user(self, user=True):
         """Write the crontab to a user (or root) instead of a file."""
         return self.write(user=user)
@@ -379,25 +409,25 @@
     def run_pending(self, **kwargs):
         """Run all commands in this crontab if pending (generator)"""
         for job in self:
             ret = job.run_pending(**kwargs)
             if ret not in [None, -1]:
                 yield ret
 
-    def run_scheduler(self, timeout=-1, **kwargs):
+    def run_scheduler(self, timeout=-1, cadence=60, warp=False):
         """Run the CronTab as an internal scheduler (generator)"""
         count = 0
         while count != timeout:
             now = datetime.now()
-            if 'warp' in kwargs:
+            if warp:
                 now += timedelta(seconds=count * 60)
             for value in self.run_pending(now=now):
                 yield value
 
-            sleep(kwargs.get('cadence', 60))
+            sleep(cadence)
             count += 1
 
     def render(self, errors=False, specials=True):
         """Render this crontab as it would be in the crontab.
 
         errors - Should we not comment out invalid entries and cause errors?
         specials - Turn known times into keywords such as "@daily"
@@ -409,28 +439,28 @@
         for line in self.lines:
             if isinstance(line, (str, str)):
                 if line.strip().startswith('#') or not line.strip():
                     crons.append(line.strip())
                 elif not errors:
                     crons.append('# DISABLED LINE\n# ' + line)
                 else:
-                    raise ValueError("Invalid line: %s" % line)
+                    raise ValueError(f"Invalid line: {line}")
             elif isinstance(line, CronItem):
                 if not line.is_valid() and not errors:
                     line.enabled = False
                 crons.append(line.render(specials=specials).strip())
 
         # Environment variables are attached to cron lines so order will
         # always work no matter how you add lines in the middle of the stack.
-        result = str(self.env) + u'\n'.join(crons)
-        if result and result[-1] not in (u'\n', u'\r'):
-            result += u'\n'
+        result = str(self.env) + '\n'.join(crons)
+        if result and result[-1] not in ('\n', '\r'):
+            result += '\n'
         return result
 
-    def new(self, command='', comment='', user=None, pre_comment=False, before=None):
+    def new(self, command='', comment='', user=None, pre_comment=False, before=None): # pylint: disable=too-many-arguments
         """
         Create a new CronItem and append it to the cron.
 
         Keyword arguments:
          command     - The command that will be run.
          comment     - The comment that should be associated with this command.
          user        - For system cron tabs, the user this command should run as.
@@ -537,20 +567,20 @@
         self.crons.remove(item)
         self.lines.remove(item)
         return 1
 
     def __repr__(self):
         kind = 'System ' if self._user is False else ''
         if self.filen:
-            return "<%sCronTab '%s'>" % (kind, self.filen)
+            return f"<{kind}CronTab '{self.filen}'>"
         if self.user and not self.user_opt:
             return "<My CronTab>"
         if self.user:
-            return "<User CronTab '%s'>" % self.user
-        return "<Unattached %sCronTab>" % kind
+            return f"<User CronTab '{self.user}'>"
+        return f"<Unattached {kind}CronTab>"
 
     def __iter__(self):
         """Return generator so we can track jobs after removal"""
         for job in list(self.crons.__iter__()):
             yield job
 
     def __getitem__(self, i):
@@ -691,31 +721,32 @@
         return self.valid
 
     def render(self, specials=True):
         """Render this set cron-job to a string"""
         if not self.is_valid() and self.enabled:
             raise ValueError('Refusing to render invalid crontab.'
                              ' Disable to continue.')
-        command = _str(self.command).replace(u'%', u'\\%')
+        command = _str(self.command).replace('%', '\\%')
         user = ''
         if self.cron and self.cron.user is False:
             if not self.user:
                 raise ValueError("Job to system-cron format, no user set!")
             user = self.user + ' '
-        result = u"%s %s%s" % (self.slices.render(specials=specials), user, command)
+        rend = self.slices.render(specials=specials)
+        result = f"{rend} {user}{command}"
         if self.stdin:
             result += ' %' + self.stdin.replace('\n', '%')
         if not self.enabled:
-            result = u"# " + result
+            result = "# " + result
         if self.comment:
             comment = self.comment = _str(self.comment)
             if self.marker:
-                comment = u"#%s: %s" % (self.marker, comment)
+                comment = f"#{self.marker}: {comment}"
             else:
-                comment = u"# " + comment
+                comment = "# " + comment
 
             if SYSTEMV or self.pre_comment or self.stdin:
                 result = comment + "\n" + result
             else:
                 result += ' ' + comment
 
         return str(self.env) + result
@@ -753,14 +784,42 @@
 
     def frequency(self, year=None):
         """Returns the number of times this item will execute in a given year
            (defaults to this year)
         """
         return self.slices.frequency(year=year)
 
+    def frequency_at_hour(self, year=None, month=None, day=None, hour=None):
+        """Returns the number of times this item will execute in a given hour
+           (defaults to this hour)
+        """
+        return self.slices.frequency_at_hour(year=year, month=month, day=day, hour=hour)
+
+    def frequency_at_day(self, year=None, month=None, day=None):
+        """Returns the number of times this item will execute in a given day
+           (defaults to today)
+        """
+        return self.slices.frequency_at_day(year=year, month=month, day=day)
+
+    def frequency_at_month(self, year=None, month=None):
+        """Returns the number of times this item will execute in a given month
+           (defaults to this month)
+        """
+        return self.slices.frequency_at_month(year=year, month=month)
+
+    def frequency_at_year(self, year=None):
+        """Returns the number of times this item will execute in a given year
+           (defaults to this year)
+        """
+        return self.slices.frequency_at_year(year=year)
+
+    def frequency(self, year=None):
+        """Return frequence per year times frequency per day"""
+        return self.frequency_per_year(year=year) * self.frequency_per_day()
+
     def frequency_per_year(self, year=None):
         """Returns the number of /days/ this item will execute on in a year
            (defaults to this year)
         """
         return self.slices.frequency_per_year(year=year)
 
     def frequency_per_day(self):
@@ -785,42 +844,42 @@
         return -1
 
     def run(self):
         """Runs the given command as a pipe"""
         env = os.environ.copy()
         env.update(self.env.all())
         shell = self.env.get('SHELL', SHELL)
-        (out, err) = open_pipe(shell, '-c', self.command, env=env).communicate()
-        if err:
-            LOG.error(err.decode("utf-8"))
-        return out.decode("utf-8").strip()
+        process = Process(shell, '-c', self.command, env=env).run()
+        if process.stderr:
+            LOG.error(process.stderr)
+        return process
 
     def schedule(self, date_from=None):
         """Return a croniter schedule if available."""
         if not date_from:
             date_from = datetime.now()
         try:
             # Croniter is an optional import
             from croniter.croniter import croniter # pylint: disable=import-outside-toplevel
-        except ImportError:
+        except ImportError as err:
             raise ImportError("Croniter not available. Please install croniter"
-                              " python module via pip or your package manager")
+                              " python module via pip or your package manager") from err
         return croniter(self.slices.clean_render(), date_from, ret_type=datetime)
 
     def description(self, **kw):
         """
         Returns a description of the crontab's schedule (if available)
 
         **kw - Keyword arguments to pass to cron_descriptor (see docs)
         """
         try:
             from cron_descriptor import ExpressionDescriptor # pylint: disable=import-outside-toplevel
-        except ImportError:
+        except ImportError as err:
             raise ImportError("cron_descriptor not available. Please install"\
-              "cron_descriptor python module via pip or your package manager")
+              "cron_descriptor python module via pip or your package manager") from err
 
         exdesc = ExpressionDescriptor(self.slices.clean_render(), **kw)
         return exdesc.get_description()
 
     @property
     def log(self):
         """Return a cron log specific for this job only"""
@@ -870,15 +929,15 @@
 
     @property
     def dow(self):
         """Return the day of the week slice"""
         return self.slices[4]
 
     def __repr__(self):
-        return "<CronItem '%s'>" % str(self)
+        return f"<CronItem '{self}'>"
 
     def __len__(self):
         return len(str(self))
 
     def __getitem__(self, key):
         return self.slices[key]
 
@@ -918,25 +977,25 @@
                 self.slices[key].on('<')
             self.slices[target].every(self.unit)
         return innercall
 
     def year(self):
         """Special every year target"""
         if self.unit > 1:
-            raise ValueError("Invalid value '%s', outside 1 year" % self.unit)
+            raise ValueError(f"Invalid value '{self.unit}', outside 1 year")
         self.slices.setall('@yearly')
 
 
 class CronSlices(list):
     """Controls a list of five time 'slices' which reprisent:
         minute frequency, hour frequency, day of month frequency,
         month requency and finally day of the week frequency.
      """
     def __init__(self, *args):
-        super(CronSlices, self).__init__([CronSlice(info) for info in S_INFO])
+        super().__init__([CronSlice(info) for info in S_INFO])
         self.special = None
         self.setall(*args)
         self.is_valid = self.is_self_valid
 
     def is_self_valid(self, *args):
         """Object version of is_valid"""
         return CronSlices.is_valid(*(args or (self,)))
@@ -973,27 +1032,28 @@
         if isinstance(value, time):
             return [value.minute, value.hour, '*', '*', '*'], None
         if isinstance(value, date):
             return [0, 0, value.day, value.month, '*'], None
             # It might be possible to later understand timedelta objects
             # but there's no convincing mathematics to do the conversion yet.
         if not isinstance(value, (list, tuple)):
-            raise ValueError("Unknown type: {}".format(type(value).__name__))
+            typ = type(value).__name__
+            raise ValueError(f"Unknown type: {typ}")
         return value, None
 
     @staticmethod
     def _parse_str(value):
         """Parse a string which contains slice information"""
         key = value.lstrip('@').lower()
         if value.count(' ') == 4:
             return value.strip().split(' '), None
-        if key in SPECIALS.keys():
+        if key in SPECIALS:
             return SPECIALS[key].split(' '), '@' + key
         if value.startswith('@'):
-            raise ValueError("Unknown special '{}'".format(value))
+            raise ValueError(f"Unknown special '{value}'")
         return [value], None
 
     def clean_render(self):
         """Return just numbered parts of this crontab"""
         return ' '.join([str(s) for s in self])
 
     def render(self, specials=True):
@@ -1002,15 +1062,15 @@
         if self.special and specials is not False:
             if self.special == '@reboot' or \
                     SPECIALS[self.special.strip('@')] == slices:
                 return self.special
         if not SYSTEMV and specials is True:
             for (name, value) in SPECIALS.items():
                 if value == slices and name not in SPECIAL_IGNORE:
-                    return "@%s" % name
+                    return f"@{name}"
         return slices
 
     def clear(self):
         """Clear the special and set values"""
         self.special = None
         for item in self:
             item.clear()
@@ -1041,14 +1101,90 @@
         """Returns the number of times this item will execute in any day"""
         return len(self[0]) * len(self[1])
 
     def frequency_per_hour(self):
         """Returns the number of times this item will execute in any hour"""
         return len(self[0])
 
+    def frequency_at_year(self, year=None):
+        """Returns the number of /days/ this item will execute
+           in a given year (default is this year)"""
+        if not year:
+            year = date.today().year
+
+        total = 0
+        for month in range(1, 13):
+            total += self.frequency_at_month(year, month)
+        return total
+
+    def frequency_at_month(self, year=None, month=None):
+        """Returns the number of times this item will execute in given month
+        (default: current month)
+        """
+        if year is None and month is None:
+            year = date.today().year
+            month = date.today().month
+        elif year is None or month is None:
+            raise ValueError(
+                f"One of more arguments undefined: year={year}, month={month}")
+
+        total = 0
+        if month in self[3]:
+            # Calculate amount of days of specific month
+            days = monthrange(year, month)[1]
+            for day in range(1, days + 1):
+                total += self.frequency_at_day(year, month, day)
+        return total
+
+    def frequency_at_day(self, year=None, month=None, day=None):
+        """Returns the number of times this item will execute in a day
+        (default: any executed day)
+        """
+        # If arguments provided, all needs to be provided
+        test_none = [x is None for x in [year, month, day]]
+
+        if all(test_none):
+            return len(self[0]) * len(self[1])
+
+        if any(test_none):
+            raise ValueError(
+                f"One of more arguments undefined: year={year}, month={month}, day={day}")
+
+        total = 0
+        if day in self[2]:
+            for hour in range(24):
+                total += self.frequency_at_hour(year, month, day, hour)
+        return total
+
+    def frequency_at_hour(self, year=None, month=None, day=None, hour=None):
+        """Returns the number of times this item will execute in a hour
+        (default: any executed hour)
+        """
+        # If arguments provided, all needs to be provided
+        test_none = [x is None for x in [year, month, day, hour]]
+
+        if all(test_none):
+            return len(self[0])
+
+        if any(test_none):
+            raise ValueError(
+                f"One of more arguments undefined: year={year}, month={month}, day={day}, hour={hour}")
+
+        result = 0
+        weekday = date(year, month, day).weekday()
+
+        # Check if scheduled for execution at defined moment
+        if hour in self[1] and \
+           day in self[2] and \
+           month in self[3] and \
+           ((weekday + 1) % 7) in self[4]:
+            result = len(self[0])
+
+        return result
+
     def __str__(self):
         return self.render()
 
     def __eq__(self, arg):
         return self.render() == CronSlices(arg).render()
 
 
@@ -1094,26 +1230,26 @@
         if value is not None:
             for part in str(value).split(','):
                 if part.find("/") > 0 or part.find("-") > 0 or part == '*':
                     self.parts += self.get_range(part)
                     continue
                 self.parts.append(self.parse_value(part, sunday=0))
 
-    def render(self, resolve=False, specials=True):
+    def render(self, resolve=False):
         """Return the slice rendered as a crontab.
 
         resolve - return integer values instead of enums (default False)
 
         """
         if not self.parts:
             return '*'
         return _render_values(self.parts, ',', resolve)
 
     def __repr__(self):
-        return "<CronSlice '%s'>" % str(self)
+        return f"<CronSlice '{self}'>"
 
     def __eq__(self, value):
         return str(self) == str(value)
 
     def __str__(self):
         return self.render()
 
@@ -1178,26 +1314,26 @@
         """Parse the value of the cron slice and raise any errors needed"""
         if val == '>':
             val = self.max
         elif val == '<':
             val = self.min
         try:
             out = get_cronvalue(val, self.enum)
-        except ValueError:
-            raise ValueError("Unrecognised %s: '%s'" % (self.name, val))
-        except KeyError:
-            raise KeyError("No enumeration for %s: '%s'" % (self.name, val))
+        except ValueError as err:
+            raise ValueError(f"Unrecognised {self.name}: '{val}'") from err
+        except KeyError as err:
+            raise KeyError(f"No enumeration for {self.name}: '{val}'") from err
 
         if self.max == 6 and int(out) == 7:
             if sunday is not None:
                 return sunday
             raise SundayError("Detected Sunday as 7 instead of 0!")
 
         if int(out) < self.min or int(out) > self.max:
-            raise ValueError("'{1}', not in {0.min}-{0.max} for {0.name}".format(self, val))
+            raise ValueError(f"'{val}', not in {self.min}-{self.max} for {self.name}")
         return out
 
 
 def get_cronvalue(value, enums):
     """Returns a value as int (pass-through) or a special enum value"""
     if isinstance(value, int):
         return value
@@ -1236,15 +1372,15 @@
 
 def _render(value, resolve=False):
     """Return a single value rendered"""
     if isinstance(value, CronRange):
         return value.render(resolve)
     if resolve:
         return str(int(value))
-    return str(u'{:02d}'.format(value) if ZERO_PAD else value)
+    return str(f'{value:02d}' if ZERO_PAD else value)
 
 
 class CronRange:
     """A range between one value and another for a time range."""
     def __init__(self, vslice, *vrange):
         # holds an extra dangling entry, for example sundays.
         self.dangling = None
@@ -1282,19 +1418,19 @@
             except SundayError:
                 if self.vfrom == 1:
                     self.vfrom = 0
                 else:
                     self.dangling = 0
                 self.vto = self.slice.parse_value(vto, sunday=6)
             if self.vto < self.vfrom:
-                raise ValueError("Bad range '{0.vfrom}-{0.vto}'".format(self))
+                raise ValueError(f"Bad range '{self.vfrom}-{self.vto}'")
         elif value == '*':
             self.all()
         else:
-            raise ValueError('Unknown cron range value "%s"' % value)
+            raise ValueError(f'Unknown cron range value "{value}"')
 
     def all(self):
         """Set this slice to all units between the miniumum and maximum"""
         self.vfrom = self.slice.min
         self.vto = self.slice.max
 
     def render(self, resolve=False):
@@ -1302,15 +1438,15 @@
         value = '*'
         if int(self.vfrom) > self.slice.min or int(self.vto) < self.slice.max:
             if self.vfrom == self.vto:
                 value = str(self.vfrom)
             else:
                 value = _render_values([self.vfrom, self.vto], '-', resolve)
         if self.seq != 1:
-            value += "/%d" % self.seq
+            value += f"/{self.seq:d}"
         if value != '*' and SYSTEMV:
             value = ','.join([str(val) for val in self.range()])
         return value
 
     def range(self):
         """Returns the range of this cron slice as a iterable list"""
         return range(int(self.vfrom), int(self.vto)+1, self.seq)
@@ -1340,15 +1476,15 @@
     list in the chain.
 
     This is all in aid of the ENV variables list which must exist one
     per job in the chain.
     """
     def __init__(self, *args, **kw):
         self.job = kw.pop('job', None)
-        super(OrderedVariableList, self).__init__(*args, **kw)
+        super().__init__(*args, **kw)
 
     @property
     def previous(self):
         """Returns the previous env in the list of jobs in the cron"""
         if self.job is not None and self.job.cron is not None:
             index = self.job.cron.crons.index(self.job)
             if index == 0:
@@ -1366,24 +1502,24 @@
             ret.update(self)
             return ret
         return self.copy()
 
     def __getitem__(self, key):
         previous = self.previous
         if key in self:
-            return super(OrderedVariableList, self).__getitem__(key)
+            return super().__getitem__(key)
         if previous is not None:
             return previous.all()[key]
-        raise KeyError("Environment Variable '%s' not found." % key)
+        raise KeyError(f"Environment Variable '{key}' not found.")
 
     def __str__(self):
         """Constructs to variable list output used in cron jobs"""
         ret = []
         for key, value in self.items():
             if self.previous:
                 if self.previous.all().get(key, None) == value:
                     continue
             if ' ' in str(value) or value == '':
-                value = '"%s"' % value
-            ret.append("%s=%s" % (key, str(value)))
+                value = f'"{value}"'
+            ret.append(f"{key}={value}")
         ret.append('')
         return "\n".join(ret)
```

### Comparing `python-crontab-2.7.1/crontabs.py` & `python-crontab-3.0.0/crontabs.py`

 * *Files identical despite different names*

### Comparing `python-crontab-2.7.1/python_crontab.egg-info/PKG-INFO` & `python-crontab-3.0.0/python_crontab.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-crontab
-Version: 2.7.1
+Version: 3.0.0
 Summary: Python Crontab API
 Home-page: https://gitlab.com/doctormo/python-crontab/
 Author: Martin Owens
 Author-email: doctormo@gmail.com
 License: LGPLv3
 Platform: linux
 Classifier: Development Status :: 5 - Production/Stable
@@ -22,16 +22,17 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Provides: crontab
 Provides: crontabs
 Provides: cronlog
-Provides-Extra: cron-description
+Description-Content-Type: text/x-rst
 Provides-Extra: cron-schedule
+Provides-Extra: cron-description
 License-File: COPYING
 License-File: AUTHORS
 
 Python Crontab
 --------------
 
 .. image:: https://gitlab.com/doctormo/python-crontab/raw/master/branding.svg
@@ -341,15 +342,17 @@
 
 (note this functionality is new and not perfect, if you find bugs report them!)
 
 Running the scheduler::
 
     tab = CronTab(tabfile='MyScripts.tab')
     for result in tab.run_scheduler():
-        print("This was printed to stdout by the process.")
+        print("Return code: {result.returncode}")
+        print("Standard Out: {result.stdout}")
+        print("Standard Err: {result.stderr}")
 
 Do not do this, it won't work because it returns generator function::
 
     tab.run_scheduler()
 
 Timeout and cadence can be changed for testing or error management::
 
@@ -357,23 +360,28 @@
         print("Will run jobs every 1 minutes for ten minutes from now()")
 
     for result in tab.run_scheduler(cadence=1, warp=True):
         print("Will run jobs every 1 second, counting each second as 1 minute")
 
 Frequency Calculation
 =====================
-
 Every job's schedule has a frequency. We can attempt to calculate the number
-of times a job would execute in a give amount of time. We have three simple
-methods::
+of times a job would execute in a give amount of time. We have two variants
+`frequency_per_*` and `frequency_at_*` calculations. The `freqency_at_*` 
+always returnes *times* a job would execute and is aware of leap years.
+
+
+`frequency_per_*`
+-----------------
+For `frequency_per_*` We have three simple methods::
 
     job.setall("1,2 1,2 * * *")
     job.frequency_per_day() == 4
 
-The per year frequency method will tell you how many days a year the
+The per year frequency method will tell you how many **days** a year the
 job would execute::
 
     job.setall("* * 1,2 1,2 *")
     job.frequency_per_year(year=2010) == 4
 
 These are combined to give the number of times a job will execute in any year::
 
@@ -382,14 +390,51 @@
 
 Frequency can be quickly checked using python built-in operators::
 
     job < "*/2 * * * *"
     job > job2
     job.slices == "*/5"
 
+
+`frequency_at_*`
+----------------
+For `frequency_at_*` We have four simple methods.
+
+The at per hour frequency method will tell you how many times the job would
+execute at a given hour::
+
+    job.setall("*/2 0 * * *")
+    job.frequency_at_hour() == 30
+    job.frequency_at_hour(year=2010, month=1, day=1, hour=0) == 30  # even hour 
+    job.frequency_at_hour(year=2010, month=1, day=1, hour=1) == 0   # odd hour
+
+The at day frequency method parameterized tells you how many times the job
+would execute at a given day::
+
+    job.setall("0 0 * * 1,2")
+    job.frequency_at_day(year=2010, month=1, day=18) == 24 # Mon Jan 18th 2020
+    job.frequency_at_day(year=2010, month=1, day=21) == 0  # Thu Jan 21th 2020
+
+The at month frequency method will tell you how many times the job would
+execute at a given month::
+
+    job.setall("0 0 * * *")
+    job.frequency_at_month() == <output_of_current_month>
+    job.frequency_at_month(year=2010, month=1) == 31
+    job.frequency_at_month(year=2010, month=2) == 28
+    job.frequency_at_month(year=2012, month=2) == 29  # leap year
+
+The at year frequency method will tell you how many times a year the
+job would execute::
+
+    job.setall("* * 3,29 2 *")
+    job.frequency_at_year(year=2021) == 24
+    job.frequency_at_year(year=2024) == 48  # leap year
+
+
 Log Functionality
 =================
 
 The log functionality will read a cron log backwards to find you the last run
 instances of your crontab and cron jobs.
 
 The crontab will limit the returned entries to the user the crontab is for::
@@ -468,9 +513,7 @@
  - Customise the location of the crontab command by setting the global CRON_COMMAND
    or the per-object cron_command attribute.
  - Support for vixie cron with username addition with user flag
  - Support for SunOS, AIX & HP with compatibility 'SystemV' mode.
  - Python 3 (3.7, 3.8, 3.10) tested, python 2.6, 2.7 removed from support.
  - Windows support works for non-system crontabs only.
    ( see mem_cron and file_cron examples above for usage )
-
-
```

### Comparing `python-crontab-2.7.1/python_crontab.egg-info/SOURCES.txt` & `python-crontab-3.0.0/python_crontab.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python-crontab-2.7.1/setup.py` & `python-crontab-3.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,14 +36,15 @@
 
 setup(
     name             = __pkgname__,
     version          = __version__,
     release          = RELEASE,
     description      = 'Python Crontab API',
     long_description = description,
+    long_description_content_type = "text/x-rst",
     author           = 'Martin Owens',
     url              = 'https://gitlab.com/doctormo/python-crontab/',
     author_email     = 'doctormo@gmail.com',
     test_suite       = 'tests',
     platforms        = 'linux',
     license          = 'LGPLv3',
     py_modules       = ['crontab', 'crontabs', 'cronlog'],
```

### Comparing `python-crontab-2.7.1/tests/data/crontest` & `python-crontab-3.0.0/tests/data/crontest`

 * *Files identical despite different names*

### Comparing `python-crontab-2.7.1/tests/data/test.log` & `python-crontab-3.0.0/tests/data/test.log`

 * *Files identical despite different names*

### Comparing `python-crontab-2.7.1/tests/test_compatibility.py` & `python-crontab-3.0.0/tests/test_compatibility.py`

 * *Files 2% similar despite different names*

```diff
@@ -112,17 +112,17 @@
 * * * * * cmd arg_with_\#_character # comment
 """)
         self.assertEqual(cron[0].command, 'cmd arg_with_\\#_character')
         self.assertEqual(cron[0].comment, 'comment')
 
     def test_07_non_posix_shell(self):
         """Shell in windows environments is split correctly"""
-        from crontab import open_pipe
+        from crontab import Process
         winfile = os.path.join(TEST_DIR, 'data', "bash\\win.exe")
-        pipe = open_pipe("{sys.executable} {winfile}".format(winfile=winfile, sys=sys), 'SLASHED', posix=False)
+        pipe = Process("{sys.executable} {winfile}".format(winfile=winfile, sys=sys), 'SLASHED', posix=False)._run()
         self.assertEqual(pipe.wait(), 0, 'Windows shell command not found!')
         (out, err) = pipe.communicate()
         self.assertEqual(out, b'Double Glazing Installed:SLASHED\n')
         self.assertEqual(err, b'')
 
 
 if __name__ == '__main__':
```

### Comparing `python-crontab-2.7.1/tests/test_context.py` & `python-crontab-3.0.0/tests/test_context.py`

 * *Files identical despite different names*

### Comparing `python-crontab-2.7.1/tests/test_croniter.py` & `python-crontab-3.0.0/tests/test_croniter.py`

 * *Files identical despite different names*

### Comparing `python-crontab-2.7.1/tests/test_crontabs.py` & `python-crontab-3.0.0/tests/test_crontabs.py`

 * *Files identical despite different names*

### Comparing `python-crontab-2.7.1/tests/test_description.py` & `python-crontab-3.0.0/tests/test_description.py`

 * *Files identical despite different names*

### Comparing `python-crontab-2.7.1/tests/test_enums.py` & `python-crontab-3.0.0/tests/test_enums.py`

 * *Files identical despite different names*

### Comparing `python-crontab-2.7.1/tests/test_env.py` & `python-crontab-3.0.0/tests/test_env.py`

 * *Files identical despite different names*

### Comparing `python-crontab-2.7.1/tests/test_equality.py` & `python-crontab-3.0.0/tests/test_equality.py`

 * *Files identical despite different names*

### Comparing `python-crontab-2.7.1/tests/test_every.py` & `python-crontab-3.0.0/tests/test_every.py`

 * *Files identical despite different names*

### Comparing `python-crontab-2.7.1/tests/test_frequency.py` & `python-crontab-3.0.0/tests/test_frequency.py`

 * *Files 20% similar despite different names*

```diff
@@ -149,11 +149,47 @@
 
     def test_16_frequency_per_hour(self):
         """Count per hour"""
         job = self.crontab.new(command='per_hour')
         job.setall("*/2 * * * *")
         self.assertEqual(job.frequency_per_hour(), 30)
 
+    def test_17_frequency_at_hour(self):
+        """Frequency at hour at given moment"""
+        job = self.crontab.new(command='at_hour')
+        job.setall("*/2 10 * * *")
+        self.assertEqual(job.frequency_at_hour(2021, 7, 9, 10), 30)
+        self.assertEqual(job.frequency_at_hour(2021, 7, 9, 11), 0)
+        self.assertEqual(job.frequency_at_hour(), 30)
+        self.assertRaises(ValueError, job.frequency_at_hour, 2021)
+
+    def test_18_frequency_at_day(self):
+        """Frequency per day at given moment"""
+        job = self.crontab.new(command='at_day')
+        job.setall("2,4 7 9,14 * *")
+        self.assertEqual(job.frequency_at_day(2021, 7, 9), 2)
+        self.assertEqual(job.frequency_at_day(2021, 7, 10), 0)
+        self.assertEqual(job.frequency_at_day(), 2)
+        self.assertRaises(ValueError, job.frequency_at_day, 2021)
+
+    def test_19_frequency_at_month(self):
+        """Frequency per month at moment"""
+        job = self.crontab.new(command='at_month')
+        job.setall("2,4 9 7,14 10,11 *")
+        self.assertEqual(job.frequency_at_month(2021, 10), 4)
+        self.assertEqual(job.frequency_at_month(2021, 12), 0)
+        self.assertEqual(job.frequency_at_month(), 0)
+        self.assertRaises(ValueError, job.frequency_at_month, 2021)
+
+    def test_20_frequency_at_year(self):
+        """Frequency at leap year day"""
+        job = self.crontab.new(command='at_year')
+        job.setall("0 * 3,29 2 *")
+        self.assertEqual(job.frequency_at_year(2021), 24)
+        self.assertEqual(job.frequency_at_year(2024), 48)
+        self.assertEqual(job.frequency_at_year(), 24)
+
+
 if __name__ == '__main__':
     test_support.run_unittest(
        FrequencyTestCase,
     )
```

### Comparing `python-crontab-2.7.1/tests/test_interaction.py` & `python-crontab-3.0.0/tests/test_interaction.py`

 * *Files identical despite different names*

### Comparing `python-crontab-2.7.1/tests/test_log.py` & `python-crontab-3.0.0/tests/test_log.py`

 * *Files identical despite different names*

### Comparing `python-crontab-2.7.1/tests/test_range.py` & `python-crontab-3.0.0/tests/test_range.py`

 * *Files identical despite different names*

### Comparing `python-crontab-2.7.1/tests/test_removal.py` & `python-crontab-3.0.0/tests/test_removal.py`

 * *Files identical despite different names*

### Comparing `python-crontab-2.7.1/tests/test_scheduler.py` & `python-crontab-3.0.0/tests/test_scheduler.py`

 * *Files identical despite different names*

### Comparing `python-crontab-2.7.1/tests/test_system_cron.py` & `python-crontab-3.0.0/tests/test_system_cron.py`

 * *Files identical despite different names*

### Comparing `python-crontab-2.7.1/tests/test_usage.py` & `python-crontab-3.0.0/tests/test_usage.py`

 * *Files 2% similar despite different names*

```diff
@@ -206,21 +206,22 @@
         cronitem.setall('0 0 * * *')
         self.assertEqual(cronitem.render(specials=True), '@daily true')
         self.assertEqual(cronitem.render(specials=None), '0 0 * * * true')
         cronitem.setall('@daily')
         self.assertEqual(cronitem.render(specials=None), '@daily true')
         self.assertEqual(cronitem.render(specials=False), '0 0 * * * true')
 
-    def test_25_open_pipe(self):
+    def test_25_process(self):
         """Test opening pipes"""
-        from crontab import open_pipe, CRON_COMMAND
-        pipe = open_pipe(CRON_COMMAND, h=None, a='one', abc='two')
-        (out, err) = pipe.communicate()
-        self.assertEqual(err, b'')
-        self.assertEqual(out, b'--abc=two|-a|-h|one\n')
+        from crontab import Process, CRON_COMMAND
+        process = Process(CRON_COMMAND, h=None, a='one', abc='two').run()
+        self.assertEqual(int(process), 0)
+        self.assertEqual(repr(process)[:8], "Process(")
+        self.assertEqual(process.stderr, '')
+        self.assertEqual(process.stdout, '--abc=two|-a|-h|one\n')
 
     def test_07_zero_padding(self):
         """Can we get zero padded output"""
         cron = crontab.CronTab(tab="02 3-5 2,4 */2 01 cmd")
         self.assertEqual(str(cron), '2 3-5 2,4 */2 1 cmd\n')
         with Attribute(crontab, 'ZERO_PAD', True):
             self.assertEqual(str(cron), '02 03-05 02,04 */2 01 cmd\n')
```

### Comparing `python-crontab-2.7.1/tests/test_utf8.py` & `python-crontab-3.0.0/tests/test_utf8.py`

 * *Files identical despite different names*

### Comparing `python-crontab-2.7.1/tests/utils.py` & `python-crontab-3.0.0/tests/utils.py`

 * *Files identical despite different names*

