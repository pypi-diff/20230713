# Comparing `tmp/sbcommons-0.0.83.tar.gz` & `tmp/sbcommons-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sbcommons-0.0.83.tar", last modified: Thu Jul 13 11:47:08 2023, max compression
+gzip compressed data, was "dist/sbcommons-0.0.9.tar", last modified: Thu Jan 17 10:21:20 2019, max compression
```

## Comparing `sbcommons-0.0.83.tar` & `sbcommons-0.0.9.tar`

### file list

```diff
@@ -1,55 +1,33 @@
-drwxr-xr-x   0 josephakande   (501) staff       (20)        0 2023-07-13 11:47:08.232563 sbcommons-0.0.83/
--rw-r--r--   0 josephakande   (501) staff       (20)     1074 2022-07-19 07:56:19.000000 sbcommons-0.0.83/LICENSE
--rw-r--r--   0 josephakande   (501) staff       (20)     3570 2023-07-13 11:47:08.232157 sbcommons-0.0.83/PKG-INFO
--rw-r--r--   0 josephakande   (501) staff       (20)     3132 2023-07-13 11:45:48.000000 sbcommons-0.0.83/README.md
-drwxr-xr-x   0 josephakande   (501) staff       (20)        0 2023-07-13 11:47:08.107023 sbcommons-0.0.83/sbcommons/
--rw-r--r--   0 josephakande   (501) staff       (20)       19 2022-07-19 07:56:19.000000 sbcommons-0.0.83/sbcommons/__init__.py
-drwxr-xr-x   0 josephakande   (501) staff       (20)        0 2023-07-13 11:47:08.116034 sbcommons-0.0.83/sbcommons/aws/
--rw-r--r--   0 josephakande   (501) staff       (20)        0 2022-07-19 07:56:19.000000 sbcommons-0.0.83/sbcommons/aws/__init__.py
--rw-r--r--   0 josephakande   (501) staff       (20)      649 2022-07-19 07:56:19.000000 sbcommons-0.0.83/sbcommons/aws/dms.py
--rw-r--r--   0 josephakande   (501) staff       (20)      631 2022-07-19 07:56:19.000000 sbcommons-0.0.83/sbcommons/aws/lambdas.py
--rw-r--r--   0 josephakande   (501) staff       (20)     9340 2022-07-19 07:56:19.000000 sbcommons-0.0.83/sbcommons/aws/redshift.py
--rw-r--r--   0 josephakande   (501) staff       (20)     6276 2023-04-12 10:24:11.000000 sbcommons-0.0.83/sbcommons/aws/s3.py
--rw-r--r--   0 josephakande   (501) staff       (20)     3007 2022-12-29 13:02:15.000000 sbcommons-0.0.83/sbcommons/aws/secrets.py
--rw-r--r--   0 josephakande   (501) staff       (20)     1622 2022-12-29 09:38:18.000000 sbcommons-0.0.83/sbcommons/aws/sns.py
-drwxr-xr-x   0 josephakande   (501) staff       (20)        0 2023-07-13 11:47:08.153495 sbcommons-0.0.83/sbcommons/crm/
--rw-r--r--   0 josephakande   (501) staff       (20)        0 2022-10-31 12:28:47.000000 sbcommons-0.0.83/sbcommons/crm/__init__.py
--rw-r--r--   0 josephakande   (501) staff       (20)     5182 2022-12-29 09:38:18.000000 sbcommons-0.0.83/sbcommons/crm/client.py
--rw-r--r--   0 josephakande   (501) staff       (20)     2745 2022-12-29 09:38:18.000000 sbcommons-0.0.83/sbcommons/crm/factories.py
-drwxr-xr-x   0 josephakande   (501) staff       (20)        0 2023-07-13 11:47:08.178167 sbcommons-0.0.83/sbcommons/crm/klaviyo/
--rw-r--r--   0 josephakande   (501) staff       (20)      218 2022-12-29 09:38:18.000000 sbcommons-0.0.83/sbcommons/crm/klaviyo/__init__.py
--rw-r--r--   0 josephakande   (501) staff       (20)    16687 2023-07-13 11:45:48.000000 sbcommons-0.0.83/sbcommons/crm/klaviyo/client.py
--rw-r--r--   0 josephakande   (501) staff       (20)    10058 2023-04-12 10:24:11.000000 sbcommons-0.0.83/sbcommons/crm/klaviyo/event.py
--rw-r--r--   0 josephakande   (501) staff       (20)     3279 2022-10-31 12:28:47.000000 sbcommons-0.0.83/sbcommons/crm/klaviyo/metric.py
--rw-r--r--   0 josephakande   (501) staff       (20)     1069 2022-12-29 09:38:18.000000 sbcommons-0.0.83/sbcommons/crm/klaviyo/parser.py
--rw-r--r--   0 josephakande   (501) staff       (20)     2017 2022-12-29 09:38:18.000000 sbcommons-0.0.83/sbcommons/crm/parser.py
-drwxr-xr-x   0 josephakande   (501) staff       (20)        0 2023-07-13 11:47:08.181290 sbcommons-0.0.83/sbcommons/crm/symplify/
--rw-r--r--   0 josephakande   (501) staff       (20)      114 2022-12-29 09:38:18.000000 sbcommons-0.0.83/sbcommons/crm/symplify/__init__.py
--rw-r--r--   0 josephakande   (501) staff       (20)     8135 2022-12-29 09:38:18.000000 sbcommons-0.0.83/sbcommons/crm/symplify/client.py
--rw-r--r--   0 josephakande   (501) staff       (20)     2004 2022-12-29 09:38:18.000000 sbcommons-0.0.83/sbcommons/crm/symplify/parser.py
-drwxr-xr-x   0 josephakande   (501) staff       (20)        0 2023-07-13 11:47:08.223567 sbcommons-0.0.83/sbcommons/logging/
--rw-r--r--   0 josephakande   (501) staff       (20)       72 2022-10-03 14:05:28.000000 sbcommons-0.0.83/sbcommons/logging/__init__.py
--rw-r--r--   0 josephakande   (501) staff       (20)      422 2022-07-19 07:56:19.000000 sbcommons-0.0.83/sbcommons/logging/lambda_logger.py
--rw-r--r--   0 josephakande   (501) staff       (20)     4865 2022-10-03 14:05:28.000000 sbcommons-0.0.83/sbcommons/logging/rotating_file_handler.py
-drwxr-xr-x   0 josephakande   (501) staff       (20)        0 2023-07-13 11:47:08.225947 sbcommons-0.0.83/sbcommons/messaging/
--rw-r--r--   0 josephakande   (501) staff       (20)        0 2022-10-21 14:11:50.000000 sbcommons-0.0.83/sbcommons/messaging/__init__.py
--rw-r--r--   0 josephakande   (501) staff       (20)      617 2022-10-21 14:11:50.000000 sbcommons-0.0.83/sbcommons/messaging/webhooks.py
-drwxr-xr-x   0 josephakande   (501) staff       (20)        0 2023-07-13 11:47:08.226977 sbcommons-0.0.83/sbcommons/parse_utils/
--rw-r--r--   0 josephakande   (501) staff       (20)     1284 2022-10-03 14:05:28.000000 sbcommons-0.0.83/sbcommons/parse_utils/__init__.py
-drwxr-xr-x   0 josephakande   (501) staff       (20)        0 2023-07-13 11:47:08.228494 sbcommons-0.0.83/sbcommons/slack/
--rw-r--r--   0 josephakande   (501) staff       (20)        0 2022-10-21 14:11:50.000000 sbcommons-0.0.83/sbcommons/slack/__init__.py
--rw-r--r--   0 josephakande   (501) staff       (20)      601 2022-10-21 14:11:50.000000 sbcommons-0.0.83/sbcommons/slack/slack.py
-drwxr-xr-x   0 josephakande   (501) staff       (20)        0 2023-07-13 11:47:08.230253 sbcommons-0.0.83/sbcommons/teams/
--rw-r--r--   0 josephakande   (501) staff       (20)        0 2022-07-19 07:56:19.000000 sbcommons-0.0.83/sbcommons/teams/__init__.py
--rw-r--r--   0 josephakande   (501) staff       (20)      289 2022-10-21 14:11:50.000000 sbcommons-0.0.83/sbcommons/teams/teams.py
--rw-r--r--   0 josephakande   (501) staff       (20)     1597 2023-04-12 10:24:11.000000 sbcommons-0.0.83/sbcommons/utils.py
-drwxr-xr-x   0 josephakande   (501) staff       (20)        0 2023-07-13 11:47:08.110067 sbcommons-0.0.83/sbcommons.egg-info/
--rw-r--r--   0 josephakande   (501) staff       (20)     3570 2023-07-13 11:47:08.000000 sbcommons-0.0.83/sbcommons.egg-info/PKG-INFO
--rw-r--r--   0 josephakande   (501) staff       (20)     1088 2023-07-13 11:47:08.000000 sbcommons-0.0.83/sbcommons.egg-info/SOURCES.txt
--rw-r--r--   0 josephakande   (501) staff       (20)        1 2023-07-13 11:47:08.000000 sbcommons-0.0.83/sbcommons.egg-info/dependency_links.txt
--rw-r--r--   0 josephakande   (501) staff       (20)      103 2023-07-13 11:47:08.000000 sbcommons-0.0.83/sbcommons.egg-info/requires.txt
--rw-r--r--   0 josephakande   (501) staff       (20)       16 2023-07-13 11:47:08.000000 sbcommons-0.0.83/sbcommons.egg-info/top_level.txt
--rw-r--r--   0 josephakande   (501) staff       (20)       38 2023-07-13 11:47:08.232743 sbcommons-0.0.83/setup.cfg
--rw-r--r--   0 josephakande   (501) staff       (20)      834 2023-07-13 11:45:48.000000 sbcommons-0.0.83/setup.py
-drwxr-xr-x   0 josephakande   (501) staff       (20)        0 2023-07-13 11:47:08.231531 sbcommons-0.0.83/tests/
--rw-r--r--   0 josephakande   (501) staff       (20)        0 2022-07-19 07:56:19.000000 sbcommons-0.0.83/tests/__init__.py
+drwxr-xr-x   0 olof       (501) staff       (20)        0 2019-01-17 10:21:20.000000 sbcommons-0.0.9/
+-rw-r--r--   0 olof       (501) staff       (20)      539 2019-01-17 10:21:20.000000 sbcommons-0.0.9/PKG-INFO
+drwxr-xr-x   0 olof       (501) staff       (20)        0 2019-01-17 10:21:20.000000 sbcommons-0.0.9/test/
+-rw-r--r--   0 olof       (501) staff       (20)        0 2019-01-14 08:24:38.000000 sbcommons-0.0.9/test/__init__.py
+drwxr-xr-x   0 olof       (501) staff       (20)        0 2019-01-17 10:21:20.000000 sbcommons-0.0.9/sbcommons/
+-rw-r--r--   0 olof       (501) staff       (20)       19 2019-01-14 08:24:38.000000 sbcommons-0.0.9/sbcommons/__init__.py
+drwxr-xr-x   0 olof       (501) staff       (20)        0 2019-01-17 10:21:20.000000 sbcommons-0.0.9/sbcommons/aws/
+-rw-r--r--   0 olof       (501) staff       (20)        0 2019-01-16 09:32:22.000000 sbcommons-0.0.9/sbcommons/aws/redshift.py
+-rw-r--r--   0 olof       (501) staff       (20)        0 2019-01-16 09:32:22.000000 sbcommons-0.0.9/sbcommons/aws/__init__.py
+-rw-r--r--   0 olof       (501) staff       (20)      980 2019-01-16 09:32:22.000000 sbcommons-0.0.9/sbcommons/aws/s3.py
+drwxr-xr-x   0 olof       (501) staff       (20)        0 2019-01-17 10:21:20.000000 sbcommons-0.0.9/sbcommons/psycopg2/
+-rw-r--r--   0 olof       (501) staff       (20)     7845 2019-01-14 08:24:38.000000 sbcommons-0.0.9/sbcommons/psycopg2/_json.py
+-rw-r--r--   0 olof       (501) staff       (20)    42337 2019-01-14 08:24:38.000000 sbcommons-0.0.9/sbcommons/psycopg2/extras.py
+-rw-r--r--   0 olof       (501) staff       (20)    13242 2019-01-14 08:24:38.000000 sbcommons-0.0.9/sbcommons/psycopg2/errorcodes.py
+-rw-r--r--   0 olof       (501) staff       (20)     4424 2019-01-14 08:24:38.000000 sbcommons-0.0.9/sbcommons/psycopg2/tz.py
+-rw-r--r--   0 olof       (501) staff       (20)    17259 2019-01-14 08:24:38.000000 sbcommons-0.0.9/sbcommons/psycopg2/_range.py
+-rw-r--r--   0 olof       (501) staff       (20)     2874 2019-01-14 08:24:38.000000 sbcommons-0.0.9/sbcommons/psycopg2/_ipaddress.py
+-rw-r--r--   0 olof       (501) staff       (20)     4899 2019-01-14 08:24:38.000000 sbcommons-0.0.9/sbcommons/psycopg2/__init__.py
+-rw-r--r--   0 olof       (501) staff       (20)     3329 2019-01-14 08:24:38.000000 sbcommons-0.0.9/sbcommons/psycopg2/psycopg1.py
+-rw-r--r--   0 olof       (501) staff       (20)     7020 2019-01-14 08:24:38.000000 sbcommons-0.0.9/sbcommons/psycopg2/extensions.py
+-rw-r--r--   0 olof       (501) staff       (20)    13757 2019-01-14 08:24:38.000000 sbcommons-0.0.9/sbcommons/psycopg2/sql.py
+-rw-r--r--   0 olof       (501) staff       (20)     8173 2019-01-14 08:24:38.000000 sbcommons-0.0.9/sbcommons/psycopg2/pool.py
+drwxr-xr-x   0 olof       (501) staff       (20)        0 2019-01-17 10:21:20.000000 sbcommons-0.0.9/sbcommons/logging/
+-rw-r--r--   0 olof       (501) staff       (20)        0 2019-01-17 09:25:36.000000 sbcommons-0.0.9/sbcommons/logging/__init__.py
+-rw-r--r--   0 olof       (501) staff       (20)      457 2019-01-17 09:30:44.000000 sbcommons-0.0.9/sbcommons/logging/lambda_logger.py
+-rw-r--r--   0 olof       (501) staff       (20)       64 2019-01-16 09:32:22.000000 sbcommons-0.0.9/README.md
+-rw-r--r--   0 olof       (501) staff       (20)      633 2019-01-17 10:21:08.000000 sbcommons-0.0.9/setup.py
+drwxr-xr-x   0 olof       (501) staff       (20)        0 2019-01-17 10:21:20.000000 sbcommons-0.0.9/sbcommons.egg-info/
+-rw-r--r--   0 olof       (501) staff       (20)      539 2019-01-17 10:21:19.000000 sbcommons-0.0.9/sbcommons.egg-info/PKG-INFO
+-rw-r--r--   0 olof       (501) staff       (20)      651 2019-01-17 10:21:19.000000 sbcommons-0.0.9/sbcommons.egg-info/SOURCES.txt
+-rw-r--r--   0 olof       (501) staff       (20)       15 2019-01-17 10:21:19.000000 sbcommons-0.0.9/sbcommons.egg-info/top_level.txt
+-rw-r--r--   0 olof       (501) staff       (20)        1 2019-01-17 10:21:19.000000 sbcommons-0.0.9/sbcommons.egg-info/dependency_links.txt
+-rw-r--r--   0 olof       (501) staff       (20)       38 2019-01-17 10:21:20.000000 sbcommons-0.0.9/setup.cfg
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

