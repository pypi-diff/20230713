# Comparing `tmp/remotemanager-0.8.3.tar.gz` & `tmp/remotemanager-0.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "remotemanager-0.8.3.tar", last modified: Tue Jul 11 15:06:14 2023, max compression
+gzip compressed data, was "remotemanager-0.8.4.tar", last modified: Thu Jul 13 07:25:54 2023, max compression
```

## Comparing `remotemanager-0.8.3.tar` & `remotemanager-0.8.4.tar`

### file list

```diff
@@ -1,66 +1,67 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:06:14.258884 remotemanager-0.8.3/
--rw-rw-rw-   0 root         (0) root         (0)     1067 2023-04-18 14:24:27.000000 remotemanager-0.8.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1278 2023-07-11 15:06:14.258884 remotemanager-0.8.3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      864 2023-05-15 12:45:06.000000 remotemanager-0.8.3/README.md
--rw-rw-rw-   0 root         (0) root         (0)     1367 2023-07-11 12:30:54.000000 remotemanager-0.8.3/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:06:14.250884 remotemanager-0.8.3/remotemanager/
--rw-rw-rw-   0 root         (0) root         (0)      481 2023-07-11 12:30:54.000000 remotemanager-0.8.3/remotemanager/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:06:14.250884 remotemanager-0.8.3/remotemanager/connection/
--rw-rw-rw-   0 root         (0) root         (0)       64 2023-04-27 12:56:19.000000 remotemanager-0.8.3/remotemanager/connection/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    15806 2023-06-14 09:06:03.000000 remotemanager-0.8.3/remotemanager/connection/cmd.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:06:14.254884 remotemanager-0.8.3/remotemanager/connection/computers/
--rw-rw-rw-   0 root         (0) root         (0)      137 2023-04-27 12:56:19.000000 remotemanager-0.8.3/remotemanager/connection/computers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    12849 2023-07-11 12:50:11.000000 remotemanager-0.8.3/remotemanager/connection/computers/base.py
--rw-rw-rw-   0 root         (0) root         (0)     1613 2023-05-24 13:29:09.000000 remotemanager-0.8.3/remotemanager/connection/computers/example.py
--rw-rw-rw-   0 root         (0) root         (0)     2970 2023-05-24 13:29:09.000000 remotemanager-0.8.3/remotemanager/connection/computers/options.py
--rw-rw-rw-   0 root         (0) root         (0)     1503 2023-05-25 09:38:01.000000 remotemanager-0.8.3/remotemanager/connection/computers/parsers.py
--rw-rw-rw-   0 root         (0) root         (0)      361 2023-05-24 13:29:09.000000 remotemanager-0.8.3/remotemanager/connection/detect_locale_error.py
--rw-rw-rw-   0 root         (0) root         (0)     6672 2023-04-27 12:56:19.000000 remotemanager-0.8.3/remotemanager/connection/testing_object.py
--rw-rw-rw-   0 root         (0) root         (0)    25712 2023-07-04 13:31:41.000000 remotemanager-0.8.3/remotemanager/connection/url.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:06:14.254884 remotemanager-0.8.3/remotemanager/dataset/
--rw-rw-rw-   0 root         (0) root         (0)       73 2023-04-27 12:56:19.000000 remotemanager-0.8.3/remotemanager/dataset/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    49329 2023-07-11 13:37:44.000000 remotemanager-0.8.3/remotemanager/dataset/dataset.py
--rw-rw-rw-   0 root         (0) root         (0)     3939 2023-07-11 12:30:54.000000 remotemanager-0.8.3/remotemanager/dataset/dependency.py
--rw-rw-rw-   0 root         (0) root         (0)    26112 2023-07-11 12:30:54.000000 remotemanager-0.8.3/remotemanager/dataset/runner.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:06:14.254884 remotemanager-0.8.3/remotemanager/jupyter/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-18 14:24:27.000000 remotemanager-0.8.3/remotemanager/jupyter/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4922 2023-07-11 12:30:54.000000 remotemanager-0.8.3/remotemanager/jupyter/magic.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:06:14.254884 remotemanager-0.8.3/remotemanager/logging/
--rw-rw-rw-   0 root         (0) root         (0)     4341 2023-06-14 09:06:03.000000 remotemanager-0.8.3/remotemanager/logging/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6489 2023-06-08 11:36:38.000000 remotemanager-0.8.3/remotemanager/logging/log.py
--rw-rw-rw-   0 root         (0) root         (0)      266 2023-04-18 14:24:27.000000 remotemanager-0.8.3/remotemanager/logging/quiet.py
--rw-rw-rw-   0 root         (0) root         (0)     1893 2023-05-31 11:11:40.000000 remotemanager-0.8.3/remotemanager/logging/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     2262 2023-04-27 12:56:19.000000 remotemanager-0.8.3/remotemanager/logging/verbosity.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:06:14.254884 remotemanager-0.8.3/remotemanager/serialisation/
--rw-rw-rw-   0 root         (0) root         (0)      583 2023-06-14 07:47:50.000000 remotemanager-0.8.3/remotemanager/serialisation/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4038 2023-04-27 12:56:19.000000 remotemanager-0.8.3/remotemanager/serialisation/serial.py
--rw-rw-rw-   0 root         (0) root         (0)      402 2023-04-18 14:24:27.000000 remotemanager-0.8.3/remotemanager/serialisation/serialdill.py
--rw-rw-rw-   0 root         (0) root         (0)      427 2023-04-18 14:24:27.000000 remotemanager-0.8.3/remotemanager/serialisation/serialjson.py
--rw-rw-rw-   0 root         (0) root         (0)     1609 2023-04-27 12:56:19.000000 remotemanager-0.8.3/remotemanager/serialisation/serialjsonpickle.py
--rw-rw-rw-   0 root         (0) root         (0)     1000 2023-04-27 12:56:19.000000 remotemanager-0.8.3/remotemanager/serialisation/serialyaml.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:06:14.258884 remotemanager-0.8.3/remotemanager/storage/
--rw-rw-rw-   0 root         (0) root         (0)      164 2023-04-27 12:56:19.000000 remotemanager-0.8.3/remotemanager/storage/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5351 2023-04-27 12:56:19.000000 remotemanager-0.8.3/remotemanager/storage/database.py
--rw-rw-rw-   0 root         (0) root         (0)     5244 2023-05-31 11:11:40.000000 remotemanager-0.8.3/remotemanager/storage/function.py
--rw-rw-rw-   0 root         (0) root         (0)     1053 2023-04-27 12:56:19.000000 remotemanager-0.8.3/remotemanager/storage/remotefunction.py
--rw-rw-rw-   0 root         (0) root         (0)    11445 2023-06-06 06:58:31.000000 remotemanager-0.8.3/remotemanager/storage/sendablemixin.py
--rw-rw-rw-   0 root         (0) root         (0)     1613 2023-07-11 12:30:54.000000 remotemanager-0.8.3/remotemanager/storage/trackedfile.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:06:14.258884 remotemanager-0.8.3/remotemanager/transport/
--rw-rw-rw-   0 root         (0) root         (0)      181 2023-04-27 12:56:19.000000 remotemanager-0.8.3/remotemanager/transport/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      541 2023-04-27 12:56:19.000000 remotemanager-0.8.3/remotemanager/transport/cp.py
--rw-rw-rw-   0 root         (0) root         (0)     2251 2023-06-02 09:40:16.000000 remotemanager-0.8.3/remotemanager/transport/rsync.py
--rw-rw-rw-   0 root         (0) root         (0)     2279 2023-06-02 10:52:35.000000 remotemanager-0.8.3/remotemanager/transport/scp.py
--rw-rw-rw-   0 root         (0) root         (0)     9435 2023-07-11 12:30:54.000000 remotemanager-0.8.3/remotemanager/transport/transport.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:06:14.258884 remotemanager-0.8.3/remotemanager/utils/
--rw-rw-rw-   0 root         (0) root         (0)     4596 2023-07-11 13:37:44.000000 remotemanager-0.8.3/remotemanager/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4505 2023-04-27 12:56:19.000000 remotemanager-0.8.3/remotemanager/utils/flags.py
--rw-rw-rw-   0 root         (0) root         (0)      149 2023-04-27 12:56:19.000000 remotemanager-0.8.3/remotemanager/utils/uuid.py
--rw-rw-rw-   0 root         (0) root         (0)     1893 2023-04-27 12:56:19.000000 remotemanager-0.8.3/remotemanager/utils/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:06:14.250884 remotemanager-0.8.3/remotemanager.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1278 2023-07-11 15:06:14.000000 remotemanager-0.8.3/remotemanager.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1788 2023-07-11 15:06:14.000000 remotemanager-0.8.3/remotemanager.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-11 15:06:14.000000 remotemanager-0.8.3/remotemanager.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      163 2023-07-11 15:06:14.000000 remotemanager-0.8.3/remotemanager.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-07-11 15:06:14.000000 remotemanager-0.8.3/remotemanager.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-11 15:06:14.258884 remotemanager-0.8.3/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       38 2023-04-18 14:24:27.000000 remotemanager-0.8.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 07:25:54.880416 remotemanager-0.8.4/
+-rw-rw-rw-   0 root         (0) root         (0)     1067 2023-04-18 14:24:27.000000 remotemanager-0.8.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1278 2023-07-13 07:25:54.880416 remotemanager-0.8.4/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      864 2023-05-15 12:45:06.000000 remotemanager-0.8.4/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     1367 2023-07-12 12:21:16.000000 remotemanager-0.8.4/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 07:25:54.868415 remotemanager-0.8.4/remotemanager/
+-rw-rw-rw-   0 root         (0) root         (0)      481 2023-07-12 12:21:16.000000 remotemanager-0.8.4/remotemanager/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 07:25:54.872415 remotemanager-0.8.4/remotemanager/connection/
+-rw-rw-rw-   0 root         (0) root         (0)       64 2023-04-27 12:56:19.000000 remotemanager-0.8.4/remotemanager/connection/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    15806 2023-06-14 09:06:03.000000 remotemanager-0.8.4/remotemanager/connection/cmd.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 07:25:54.872415 remotemanager-0.8.4/remotemanager/connection/computers/
+-rw-rw-rw-   0 root         (0) root         (0)      137 2023-04-27 12:56:19.000000 remotemanager-0.8.4/remotemanager/connection/computers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    12849 2023-07-11 12:50:11.000000 remotemanager-0.8.4/remotemanager/connection/computers/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     1613 2023-05-24 13:29:09.000000 remotemanager-0.8.4/remotemanager/connection/computers/example.py
+-rw-rw-rw-   0 root         (0) root         (0)     2970 2023-05-24 13:29:09.000000 remotemanager-0.8.4/remotemanager/connection/computers/options.py
+-rw-rw-rw-   0 root         (0) root         (0)     1503 2023-05-25 09:38:01.000000 remotemanager-0.8.4/remotemanager/connection/computers/parsers.py
+-rw-rw-rw-   0 root         (0) root         (0)      361 2023-05-24 13:29:09.000000 remotemanager-0.8.4/remotemanager/connection/detect_locale_error.py
+-rw-rw-rw-   0 root         (0) root         (0)     6672 2023-04-27 12:56:19.000000 remotemanager-0.8.4/remotemanager/connection/testing_object.py
+-rw-rw-rw-   0 root         (0) root         (0)    25712 2023-07-04 13:31:41.000000 remotemanager-0.8.4/remotemanager/connection/url.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 07:25:54.872415 remotemanager-0.8.4/remotemanager/dataset/
+-rw-rw-rw-   0 root         (0) root         (0)       73 2023-04-27 12:56:19.000000 remotemanager-0.8.4/remotemanager/dataset/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    50081 2023-07-13 05:57:57.000000 remotemanager-0.8.4/remotemanager/dataset/dataset.py
+-rw-rw-rw-   0 root         (0) root         (0)     4895 2023-07-12 13:38:06.000000 remotemanager-0.8.4/remotemanager/dataset/dependency.py
+-rw-rw-rw-   0 root         (0) root         (0)      792 2023-07-12 13:38:06.000000 remotemanager-0.8.4/remotemanager/dataset/lazy_append.py
+-rw-rw-rw-   0 root         (0) root         (0)    26112 2023-07-13 05:57:57.000000 remotemanager-0.8.4/remotemanager/dataset/runner.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 07:25:54.872415 remotemanager-0.8.4/remotemanager/jupyter/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-18 14:24:27.000000 remotemanager-0.8.4/remotemanager/jupyter/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4922 2023-07-13 05:57:57.000000 remotemanager-0.8.4/remotemanager/jupyter/magic.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 07:25:54.876415 remotemanager-0.8.4/remotemanager/logging/
+-rw-rw-rw-   0 root         (0) root         (0)     4341 2023-06-14 09:06:03.000000 remotemanager-0.8.4/remotemanager/logging/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6489 2023-06-08 11:36:38.000000 remotemanager-0.8.4/remotemanager/logging/log.py
+-rw-rw-rw-   0 root         (0) root         (0)      266 2023-04-18 14:24:27.000000 remotemanager-0.8.4/remotemanager/logging/quiet.py
+-rw-rw-rw-   0 root         (0) root         (0)     1893 2023-05-31 11:11:40.000000 remotemanager-0.8.4/remotemanager/logging/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     2262 2023-04-27 12:56:19.000000 remotemanager-0.8.4/remotemanager/logging/verbosity.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 07:25:54.876415 remotemanager-0.8.4/remotemanager/serialisation/
+-rw-rw-rw-   0 root         (0) root         (0)      583 2023-06-14 07:47:50.000000 remotemanager-0.8.4/remotemanager/serialisation/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4038 2023-04-27 12:56:19.000000 remotemanager-0.8.4/remotemanager/serialisation/serial.py
+-rw-rw-rw-   0 root         (0) root         (0)      402 2023-04-18 14:24:27.000000 remotemanager-0.8.4/remotemanager/serialisation/serialdill.py
+-rw-rw-rw-   0 root         (0) root         (0)      427 2023-04-18 14:24:27.000000 remotemanager-0.8.4/remotemanager/serialisation/serialjson.py
+-rw-rw-rw-   0 root         (0) root         (0)     1609 2023-04-27 12:56:19.000000 remotemanager-0.8.4/remotemanager/serialisation/serialjsonpickle.py
+-rw-rw-rw-   0 root         (0) root         (0)     1000 2023-04-27 12:56:19.000000 remotemanager-0.8.4/remotemanager/serialisation/serialyaml.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 07:25:54.876415 remotemanager-0.8.4/remotemanager/storage/
+-rw-rw-rw-   0 root         (0) root         (0)      164 2023-04-27 12:56:19.000000 remotemanager-0.8.4/remotemanager/storage/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5351 2023-04-27 12:56:19.000000 remotemanager-0.8.4/remotemanager/storage/database.py
+-rw-rw-rw-   0 root         (0) root         (0)     5244 2023-05-31 11:11:40.000000 remotemanager-0.8.4/remotemanager/storage/function.py
+-rw-rw-rw-   0 root         (0) root         (0)     1053 2023-04-27 12:56:19.000000 remotemanager-0.8.4/remotemanager/storage/remotefunction.py
+-rw-rw-rw-   0 root         (0) root         (0)    11445 2023-06-06 06:58:31.000000 remotemanager-0.8.4/remotemanager/storage/sendablemixin.py
+-rw-rw-rw-   0 root         (0) root         (0)     1613 2023-07-13 05:57:57.000000 remotemanager-0.8.4/remotemanager/storage/trackedfile.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 07:25:54.876415 remotemanager-0.8.4/remotemanager/transport/
+-rw-rw-rw-   0 root         (0) root         (0)      181 2023-04-27 12:56:19.000000 remotemanager-0.8.4/remotemanager/transport/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      541 2023-04-27 12:56:19.000000 remotemanager-0.8.4/remotemanager/transport/cp.py
+-rw-rw-rw-   0 root         (0) root         (0)     2251 2023-06-02 09:40:16.000000 remotemanager-0.8.4/remotemanager/transport/rsync.py
+-rw-rw-rw-   0 root         (0) root         (0)     2279 2023-06-02 10:52:35.000000 remotemanager-0.8.4/remotemanager/transport/scp.py
+-rw-rw-rw-   0 root         (0) root         (0)     9435 2023-07-13 05:57:57.000000 remotemanager-0.8.4/remotemanager/transport/transport.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 07:25:54.876415 remotemanager-0.8.4/remotemanager/utils/
+-rw-rw-rw-   0 root         (0) root         (0)     4596 2023-07-13 05:57:57.000000 remotemanager-0.8.4/remotemanager/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4505 2023-04-27 12:56:19.000000 remotemanager-0.8.4/remotemanager/utils/flags.py
+-rw-rw-rw-   0 root         (0) root         (0)      149 2023-04-27 12:56:19.000000 remotemanager-0.8.4/remotemanager/utils/uuid.py
+-rw-rw-rw-   0 root         (0) root         (0)     1893 2023-04-27 12:56:19.000000 remotemanager-0.8.4/remotemanager/utils/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 07:25:54.872415 remotemanager-0.8.4/remotemanager.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1278 2023-07-13 07:25:54.000000 remotemanager-0.8.4/remotemanager.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1825 2023-07-13 07:25:54.000000 remotemanager-0.8.4/remotemanager.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-13 07:25:54.000000 remotemanager-0.8.4/remotemanager.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      163 2023-07-13 07:25:54.000000 remotemanager-0.8.4/remotemanager.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-07-13 07:25:54.000000 remotemanager-0.8.4/remotemanager.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-13 07:25:54.880416 remotemanager-0.8.4/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       38 2023-04-18 14:24:27.000000 remotemanager-0.8.4/setup.py
```

### Comparing `remotemanager-0.8.3/LICENSE` & `remotemanager-0.8.4/LICENSE`

 * *Files identical despite different names*

### Comparing `remotemanager-0.8.3/PKG-INFO` & `remotemanager-0.8.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: remotemanager
-Version: 0.8.3
+Version: 0.8.4
 Summary: remote run management tool
 Author-email: Louis Beal <louis.j.beal@gmail.com>
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dill
```

### Comparing `remotemanager-0.8.3/README.md` & `remotemanager-0.8.4/README.md`

 * *Files identical despite different names*

### Comparing `remotemanager-0.8.3/pyproject.toml` & `remotemanager-0.8.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 [tool.pytest.ini_options]
 addopts = "--nbval --cov=remotemanager --cov-report term-missing --cov-append --nbval-sanitize-with ./tests/uuid_sanitise.cfg"
 
 [tool.coverage.report]
 omit = ["remotemanager/connection/computers/*"]
 
 [tool.bumpver]
-current_version = "0.8.3"
+current_version = "0.8.4"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "[clean] bump version {old_version} -> {new_version}"
 commit = true
 tag = false
 push = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `remotemanager-0.8.3/remotemanager/connection/cmd.py` & `remotemanager-0.8.4/remotemanager/connection/cmd.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.8.3/remotemanager/connection/computers/base.py` & `remotemanager-0.8.4/remotemanager/connection/computers/base.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.8.3/remotemanager/connection/computers/example.py` & `remotemanager-0.8.4/remotemanager/connection/computers/example.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.8.3/remotemanager/connection/computers/options.py` & `remotemanager-0.8.4/remotemanager/connection/computers/options.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.8.3/remotemanager/connection/computers/parsers.py` & `remotemanager-0.8.4/remotemanager/connection/computers/parsers.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.8.3/remotemanager/connection/testing_object.py` & `remotemanager-0.8.4/remotemanager/connection/testing_object.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.8.3/remotemanager/connection/url.py` & `remotemanager-0.8.4/remotemanager/connection/url.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.8.3/remotemanager/dataset/dataset.py` & `remotemanager-0.8.4/remotemanager/dataset/dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import gc
 import os
 import typing
 import time
 import shutil
 import warnings
 
+from remotemanager.dataset.lazy_append import LazyAppend
 from remotemanager.storage.remotefunction import cached_functions
 from remotemanager.connection.url import URL
 from remotemanager.storage.database import Database
 from remotemanager.storage.function import Function
 from remotemanager.dataset.runner import Runner, localwinerror
 import remotemanager.transport as tp
 import remotemanager.serialisation as sr
@@ -429,14 +430,16 @@
         name: str = None,
         extra_files_send: list = None,
         extra_files_recv: list = None,
         dependency_call: bool = False,
         verbose: int = None,
         quiet: bool = False,
         skip: bool = True,
+        lazy: bool = False,
+        chain_run_args: bool = True,
         **run_args,
     ):
         """
         Serialise arguments for later runner construction
 
         Args:
             args (dict):
@@ -453,35 +456,44 @@
                 True if called via the dependency handler
             verbose (int, Verbose, None):
                 verbose level for this runner (defaults to Dataset level)
             quiet (bool):
                 disable printing for this append if True
             skip (bool):
                 ignores checks for an existing runner if set to False
+            lazy (bool):
+                performs a "lazy" append if True, skipping the dataset update. You MUST
+                call ds.finish_append() after you are done appending to avoid strange
+                behaviours
+            chain_run_args (bool):
+                for dependency runs, will not propagate run_args to other datasets in
+                the chain if False (defaults True)
             run_args:
                 any extra arguments to pass to runner
         """
         self._logger.debug("#### Dataset append_run called")
         Quiet.state = quiet
         if args is None and arguments is not None:
             args = arguments
 
         if verbose is None:
             verbose = self.verbose.value
 
         if self.dependency is not None and not dependency_call:
             return self.dependency.append_run(
-                self,
+                caller=self,
+                chain_run_args=chain_run_args,
                 args=args,
                 name=name,
                 extra_files_send=extra_files_send,  # noqa: E251
                 extra_files_recv=extra_files_recv,  # noqa: E251
                 verbose=verbose,
                 skip=skip,
-                **run_args,
+                lazy=lazy,
+                run_args=run_args,
             )
 
         # first grab global arguments and update them with explicit args
         run_arguments = {k: v for k, v in self._global_run_args.items()}
         run_arguments.update(run_args)
 
         extra_files_send = ensure_list(extra_files_send) + self._extra_files["send"]
@@ -520,17 +532,24 @@
         elif tmp.uuid not in self._uuids:
             self._runs[r_id] = tmp
             self._uuids.append(tmp.uuid)
             self._logger.important(f"appended run {tmp.name}")
         else:
             self._logger.important(f"runner {tmp.name} already exists")
 
-        self.database.update(self.pack())
+        if not lazy:
+            self.finish_append()
         Quiet.state = False
 
+    def finish_append(self):
+        self.database.update(self.pack())
+
+    def lazy_append(self):
+        return LazyAppend(self)
+
     def remove_run(self, id: any) -> bool:
         """
         Remove a runner with the given identifier. Search methods are identical
         get_runner(id)
 
         Args:
             id:
```

### Comparing `remotemanager-0.8.3/remotemanager/dataset/dependency.py` & `remotemanager-0.8.4/remotemanager/dataset/dependency.py`

 * *Files 15% similar despite different names*

```diff
@@ -56,36 +56,48 @@
         for pair in self.network:
             for ds in pair:
                 if ds not in datasets:
                     datasets.append(ds)
 
         return datasets
 
-    def append_run(self, caller, *args, **kwargs):
+    def append_run(self, caller, chain_run_args, run_args, *args, **kwargs):
         """
         Appends runs with the same args to all datasets
 
         Args:
             caller:
-                (Dataset): The dataset which deferrs to the dependency
+                (Dataset): The dataset which defers to the dependency
+            chain_run_args (bool):
+                for dependency runs, will not propagate run_args to other datasets in
+                the chain if False (defaults True)
             *args:
                 append_run args
             **kwargs:
                 append_run keyword args
 
         Returns:
             None
         """
         self._logger.info(f"appending run from {caller}")
 
         datasets = self.ds_list
         self._logger.info(f"There are {len(datasets)} datasets in the chain")
 
+        if chain_run_args:
+            self._logger.info("chain_args is True, propagating")
+            kwargs.update(run_args)
+
         for ds in datasets:
-            ds.append_run(dependency_call=True, *args, **kwargs)
+            if ds == caller:
+                caller_args = {k: v for k, v in kwargs.items()}
+                caller_args.update(run_args)
+                ds.append_run(dependency_call=True, *args, **caller_args)
+            else:
+                ds.append_run(dependency_call=True, *args, **kwargs)
 
         for ds in datasets:
             parents = self.get_parents(ds)
             if len(parents) > 1:
                 warnings.warn(
                     "Multiple parents detected. "
                     "Variable passing in this instance is unstable!"
@@ -125,9 +137,19 @@
             ds_store[ds] = len(ds.runners)
 
         if not len(set(ds_store.values())) == 1:
             msg = f"Datasets do not have matching numbers of runners!: " f"{ds_store}"
             self._logger.critical(msg)
             raise RuntimeError(msg)
 
+        delay = []
         for ds in ds_store:
+            # if a dataset is a child, it will skip the exec, and only send files
+            # we want to wait for all files to be present, so add the datasets that
+            # exec (parentless parents) to a list and exec later
+            if ds.is_child:
+                ds._run(*args, **kwargs)
+            else:
+                delay.append(ds)
+
+        for ds in delay:
             ds._run(*args, **kwargs)
```

### Comparing `remotemanager-0.8.3/remotemanager/dataset/runner.py` & `remotemanager-0.8.4/remotemanager/dataset/runner.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.8.3/remotemanager/jupyter/magic.py` & `remotemanager-0.8.4/remotemanager/jupyter/magic.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.8.3/remotemanager/logging/__init__.py` & `remotemanager-0.8.4/remotemanager/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.8.3/remotemanager/logging/log.py` & `remotemanager-0.8.4/remotemanager/logging/log.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.8.3/remotemanager/logging/utils.py` & `remotemanager-0.8.4/remotemanager/logging/utils.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.8.3/remotemanager/logging/verbosity.py` & `remotemanager-0.8.4/remotemanager/logging/verbosity.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.8.3/remotemanager/serialisation/__init__.py` & `remotemanager-0.8.4/remotemanager/serialisation/__init__.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.8.3/remotemanager/serialisation/serial.py` & `remotemanager-0.8.4/remotemanager/serialisation/serial.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.8.3/remotemanager/serialisation/serialjsonpickle.py` & `remotemanager-0.8.4/remotemanager/serialisation/serialjsonpickle.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.8.3/remotemanager/serialisation/serialyaml.py` & `remotemanager-0.8.4/remotemanager/serialisation/serialyaml.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.8.3/remotemanager/storage/database.py` & `remotemanager-0.8.4/remotemanager/storage/database.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.8.3/remotemanager/storage/function.py` & `remotemanager-0.8.4/remotemanager/storage/function.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.8.3/remotemanager/storage/remotefunction.py` & `remotemanager-0.8.4/remotemanager/storage/remotefunction.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.8.3/remotemanager/storage/sendablemixin.py` & `remotemanager-0.8.4/remotemanager/storage/sendablemixin.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.8.3/remotemanager/storage/trackedfile.py` & `remotemanager-0.8.4/remotemanager/storage/trackedfile.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.8.3/remotemanager/transport/cp.py` & `remotemanager-0.8.4/remotemanager/transport/cp.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.8.3/remotemanager/transport/rsync.py` & `remotemanager-0.8.4/remotemanager/transport/rsync.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.8.3/remotemanager/transport/scp.py` & `remotemanager-0.8.4/remotemanager/transport/scp.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.8.3/remotemanager/transport/transport.py` & `remotemanager-0.8.4/remotemanager/transport/transport.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.8.3/remotemanager/utils/__init__.py` & `remotemanager-0.8.4/remotemanager/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.8.3/remotemanager/utils/flags.py` & `remotemanager-0.8.4/remotemanager/utils/flags.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.8.3/remotemanager/utils/version.py` & `remotemanager-0.8.4/remotemanager/utils/version.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.8.3/remotemanager.egg-info/PKG-INFO` & `remotemanager-0.8.4/remotemanager.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: remotemanager
-Version: 0.8.3
+Version: 0.8.4
 Summary: remote run management tool
 Author-email: Louis Beal <louis.j.beal@gmail.com>
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dill
```

### Comparing `remotemanager-0.8.3/remotemanager.egg-info/SOURCES.txt` & `remotemanager-0.8.4/remotemanager.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 remotemanager/connection/computers/base.py
 remotemanager/connection/computers/example.py
 remotemanager/connection/computers/options.py
 remotemanager/connection/computers/parsers.py
 remotemanager/dataset/__init__.py
 remotemanager/dataset/dataset.py
 remotemanager/dataset/dependency.py
+remotemanager/dataset/lazy_append.py
 remotemanager/dataset/runner.py
 remotemanager/jupyter/__init__.py
 remotemanager/jupyter/magic.py
 remotemanager/logging/__init__.py
 remotemanager/logging/log.py
 remotemanager/logging/quiet.py
 remotemanager/logging/utils.py
```

