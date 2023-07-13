# Comparing `tmp/inhandtest-0.0.60.tar.gz` & `tmp/inhandtest-0.0.61.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\inhandtest-0.0.60.tar", last modified: Mon Jul 10 05:54:06 2023, max compression
+gzip compressed data, was "dist\inhandtest-0.0.61.tar", last modified: Thu Jul 13 10:13:10 2023, max compression
```

## Comparing `inhandtest-0.0.60.tar` & `inhandtest-0.0.61.tar`

### file list

```diff
@@ -1,69 +1,70 @@
-drwxrwxrwx   0        0        0        0 2023-07-10 05:54:06.000000 inhandtest-0.0.60/
--rw-rw-rw-   0        0        0       81 2023-04-13 01:59:22.000000 inhandtest-0.0.60/MANIFEST.in
--rw-rw-rw-   0        0        0      593 2023-07-10 05:54:06.000000 inhandtest-0.0.60/PKG-INFO
--rw-rw-rw-   0        0        0    12238 2023-02-27 03:43:37.000000 inhandtest-0.0.60/README.md
-drwxrwxrwx   0        0        0        0 2023-07-10 05:54:06.000000 inhandtest-0.0.60/inhandtest/
--rw-rw-rw-   0        0        0        0 2023-01-31 08:41:58.000000 inhandtest-0.0.60/inhandtest/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-10 05:54:06.000000 inhandtest-0.0.60/inhandtest/base_page/
--rw-rw-rw-   0        0        0      330 2023-05-31 07:35:39.000000 inhandtest-0.0.60/inhandtest/base_page/__init__.py
--rw-rw-rw-   0        0        0    43260 2023-07-03 08:13:32.000000 inhandtest-0.0.60/inhandtest/base_page/_ig_contents_locators.py
--rw-rw-rw-   0        0        0    27868 2023-05-17 02:51:06.000000 inhandtest-0.0.60/inhandtest/base_page/_ir3XX_contents_locators.py
--rw-rw-rw-   0        0        0    64964 2023-05-11 07:07:35.000000 inhandtest-0.0.60/inhandtest/base_page/_vg710_contents_locators.py
--rw-rw-rw-   0        0        0    63306 2023-07-10 05:49:05.000000 inhandtest-0.0.60/inhandtest/base_page/base_page.py
--rw-rw-rw-   0        0        0    26127 2023-07-05 03:02:01.000000 inhandtest-0.0.60/inhandtest/base_page/table_tr.py
--rw-rw-rw-   0        0        0      608 2023-03-31 07:18:06.000000 inhandtest-0.0.60/inhandtest/exception.py
--rw-rw-rw-   0        0        0     3971 2023-06-16 00:48:06.000000 inhandtest-0.0.60/inhandtest/file.py
--rw-rw-rw-   0        0        0    10907 2023-06-15 06:06:07.000000 inhandtest-0.0.60/inhandtest/inmodbus.py
--rw-rw-rw-   0        0        0     4451 2023-06-15 05:47:54.000000 inhandtest-0.0.60/inhandtest/inmongodb.py
--rw-rw-rw-   0        0        0    22542 2023-07-03 10:18:22.000000 inhandtest-0.0.60/inhandtest/inmqtt.py
-drwxrwxrwx   0        0        0        0 2023-07-10 05:54:06.000000 inhandtest-0.0.60/inhandtest/inrequest/
--rw-rw-rw-   0        0        0      503 2023-07-10 05:21:05.000000 inhandtest-0.0.60/inhandtest/inrequest/__init__.py
--rw-rw-rw-   0        0        0     8021 2023-07-06 09:44:41.000000 inhandtest-0.0.60/inhandtest/inrequest/console.py
--rw-rw-rw-   0        0        0    26186 2023-07-05 05:25:12.000000 inhandtest-0.0.60/inhandtest/inrequest/dm.py
--rw-rw-rw-   0        0        0     4043 2023-07-05 05:22:24.000000 inhandtest-0.0.60/inhandtest/inrequest/dn.py
--rw-rw-rw-   0        0        0      183 2023-07-06 10:28:04.000000 inhandtest-0.0.60/inhandtest/inrequest/er_device.py
--rw-rw-rw-   0        0        0     7352 2023-07-05 05:27:06.000000 inhandtest-0.0.60/inhandtest/inrequest/ics.py
--rw-rw-rw-   0        0        0     9584 2023-07-06 10:16:13.000000 inhandtest-0.0.60/inhandtest/inrequest/inrequest.py
--rw-rw-rw-   0        0        0    24111 2023-07-10 05:16:38.000000 inhandtest-0.0.60/inhandtest/inrequest/nezha.py
--rw-rw-rw-   0        0        0     8389 2023-07-03 08:50:33.000000 inhandtest-0.0.60/inhandtest/inserial.py
--rw-rw-rw-   0        0        0    16027 2023-07-06 07:21:54.000000 inhandtest-0.0.60/inhandtest/insocket.py
--rw-rw-rw-   0        0        0     8481 2023-06-15 06:12:16.000000 inhandtest-0.0.60/inhandtest/inssh.py
--rw-rw-rw-   0        0        0     1569 2023-05-24 09:45:24.000000 inhandtest-0.0.60/inhandtest/ip.py
--rw-rw-rw-   0        0        0     1390 2023-06-15 09:39:25.000000 inhandtest-0.0.60/inhandtest/log.py
--rw-rw-rw-   0        0        0    13757 2023-06-15 05:47:54.000000 inhandtest-0.0.60/inhandtest/mail.py
--rw-rw-rw-   0        0        0      387 2023-06-12 09:08:02.000000 inhandtest-0.0.60/inhandtest/notice_email.html
-drwxrwxrwx   0        0        0        0 2023-07-10 05:54:06.000000 inhandtest-0.0.60/inhandtest/pages/
--rw-rw-rw-   0        0        0      230 2023-05-31 07:29:45.000000 inhandtest-0.0.60/inhandtest/pages/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-10 05:54:06.000000 inhandtest-0.0.60/inhandtest/pages/ingateway/
--rw-rw-rw-   0        0        0      136 2023-05-31 07:30:00.000000 inhandtest-0.0.60/inhandtest/pages/ingateway/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-10 05:54:06.000000 inhandtest-0.0.60/inhandtest/pages/ingateway/edge_computing/
--rw-rw-rw-   0        0        0      134 2023-05-25 07:33:25.000000 inhandtest-0.0.60/inhandtest/pages/ingateway/edge_computing/__init__.py
--rw-rw-rw-   0        0        0    67724 2023-07-10 05:52:27.000000 inhandtest-0.0.60/inhandtest/pages/ingateway/edge_computing/edge_computing_locators.py
--rw-rw-rw-   0        0        0    72025 2023-07-05 08:11:13.000000 inhandtest-0.0.60/inhandtest/pages/ingateway/edge_computing/python_edge_computing.py
--rw-rw-rw-   0        0        0     3247 2023-07-05 03:12:45.000000 inhandtest-0.0.60/inhandtest/pages/ingateway/ingateway.py
--rw-rw-rw-   0        0        0    11890 2023-07-05 02:55:07.000000 inhandtest-0.0.60/inhandtest/pages/ingateway/locale.yml
--rw-rw-rw-   0        0        0      911 2023-06-02 06:30:38.000000 inhandtest-0.0.60/inhandtest/pages/ingateway/locators.py
-drwxrwxrwx   0        0        0        0 2023-07-10 05:54:06.000000 inhandtest-0.0.60/inhandtest/pages/ingateway/network/
--rw-rw-rw-   0        0        0      134 2023-05-15 07:33:50.000000 inhandtest-0.0.60/inhandtest/pages/ingateway/network/__init__.py
--rw-rw-rw-   0        0        0    68039 2023-07-05 01:05:37.000000 inhandtest-0.0.60/inhandtest/pages/ingateway/network/network.py
--rw-rw-rw-   0        0        0    86226 2023-07-05 01:05:03.000000 inhandtest-0.0.60/inhandtest/pages/ingateway/network/network_locators.py
-drwxrwxrwx   0        0        0        0 2023-07-10 05:54:06.000000 inhandtest-0.0.60/inhandtest/pages/ingateway/overview/
--rw-rw-rw-   0        0        0      134 2023-05-15 07:33:50.000000 inhandtest-0.0.60/inhandtest/pages/ingateway/overview/__init__.py
--rw-rw-rw-   0        0        0     6953 2023-06-02 09:29:07.000000 inhandtest-0.0.60/inhandtest/pages/ingateway/overview/overview.py
--rw-rw-rw-   0        0        0     6260 2023-05-18 07:02:23.000000 inhandtest-0.0.60/inhandtest/pages/ingateway/overview/overview_locators.py
-drwxrwxrwx   0        0        0        0 2023-07-10 05:54:06.000000 inhandtest-0.0.60/inhandtest/pages/ingateway/system/
--rw-rw-rw-   0        0        0      133 2023-06-02 06:29:57.000000 inhandtest-0.0.60/inhandtest/pages/ingateway/system/__init__.py
--rw-rw-rw-   0        0        0    28514 2023-06-26 05:24:31.000000 inhandtest-0.0.60/inhandtest/pages/ingateway/system/system.py
--rw-rw-rw-   0        0        0    30656 2023-06-26 05:24:31.000000 inhandtest-0.0.60/inhandtest/pages/ingateway/system/system_locators.py
--rw-rw-rw-   0        0        0     1224 2023-04-28 06:53:30.000000 inhandtest-0.0.60/inhandtest/pytest_email.html
--rw-rw-rw-   0        0        0    34823 2023-07-06 06:11:52.000000 inhandtest-0.0.60/inhandtest/telnet.py
--rw-rw-rw-   0        0        0    30311 2023-07-10 05:36:50.000000 inhandtest-0.0.60/inhandtest/tools.py
-drwxrwxrwx   0        0        0        0 2023-07-10 05:54:06.000000 inhandtest-0.0.60/inhandtest.egg-info/
--rw-rw-rw-   0        0        0      593 2023-07-10 05:54:06.000000 inhandtest-0.0.60/inhandtest.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1877 2023-07-10 05:54:06.000000 inhandtest-0.0.60/inhandtest.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-10 05:54:06.000000 inhandtest-0.0.60/inhandtest.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      123 2023-07-10 05:54:06.000000 inhandtest-0.0.60/inhandtest.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-07-10 05:54:06.000000 inhandtest-0.0.60/inhandtest.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      147 2023-06-01 10:06:41.000000 inhandtest-0.0.60/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-10 05:54:06.000000 inhandtest-0.0.60/setup.cfg
--rw-rw-rw-   0        0        0     1615 2023-07-10 05:53:53.000000 inhandtest-0.0.60/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-13 10:13:10.000000 inhandtest-0.0.61/
+-rw-rw-rw-   0        0        0       81 2023-04-13 01:59:22.000000 inhandtest-0.0.61/MANIFEST.in
+-rw-rw-rw-   0        0        0      593 2023-07-13 10:13:10.000000 inhandtest-0.0.61/PKG-INFO
+-rw-rw-rw-   0        0        0    12238 2023-02-27 03:43:37.000000 inhandtest-0.0.61/README.md
+drwxrwxrwx   0        0        0        0 2023-07-13 10:13:10.000000 inhandtest-0.0.61/inhandtest/
+-rw-rw-rw-   0        0        0        0 2023-01-31 08:41:58.000000 inhandtest-0.0.61/inhandtest/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-13 10:13:10.000000 inhandtest-0.0.61/inhandtest/base_page/
+-rw-rw-rw-   0        0        0      330 2023-05-31 07:35:39.000000 inhandtest-0.0.61/inhandtest/base_page/__init__.py
+-rw-rw-rw-   0        0        0    43260 2023-07-03 08:13:32.000000 inhandtest-0.0.61/inhandtest/base_page/_ig_contents_locators.py
+-rw-rw-rw-   0        0        0    27868 2023-05-17 02:51:06.000000 inhandtest-0.0.61/inhandtest/base_page/_ir3XX_contents_locators.py
+-rw-rw-rw-   0        0        0    64964 2023-05-11 07:07:35.000000 inhandtest-0.0.61/inhandtest/base_page/_vg710_contents_locators.py
+-rw-rw-rw-   0        0        0    63709 2023-07-10 10:33:04.000000 inhandtest-0.0.61/inhandtest/base_page/base_page.py
+-rw-rw-rw-   0        0        0    26127 2023-07-05 03:02:01.000000 inhandtest-0.0.61/inhandtest/base_page/table_tr.py
+-rw-rw-rw-   0        0        0      608 2023-03-31 07:18:06.000000 inhandtest-0.0.61/inhandtest/exception.py
+-rw-rw-rw-   0        0        0     3971 2023-06-16 00:48:06.000000 inhandtest-0.0.61/inhandtest/file.py
+-rw-rw-rw-   0        0        0    11506 2023-07-10 10:34:36.000000 inhandtest-0.0.61/inhandtest/inmodbus.py
+-rw-rw-rw-   0        0        0     4451 2023-06-15 05:47:54.000000 inhandtest-0.0.61/inhandtest/inmongodb.py
+-rw-rw-rw-   0        0        0    22542 2023-07-03 10:18:22.000000 inhandtest-0.0.61/inhandtest/inmqtt.py
+drwxrwxrwx   0        0        0        0 2023-07-13 10:13:10.000000 inhandtest-0.0.61/inhandtest/inrequest/
+-rw-rw-rw-   0        0        0      573 2023-07-13 10:11:38.000000 inhandtest-0.0.61/inhandtest/inrequest/__init__.py
+-rw-rw-rw-   0        0        0     8343 2023-07-13 10:03:57.000000 inhandtest-0.0.61/inhandtest/inrequest/console.py
+-rw-rw-rw-   0        0        0    26186 2023-07-05 05:25:12.000000 inhandtest-0.0.61/inhandtest/inrequest/dm.py
+-rw-rw-rw-   0        0        0     4043 2023-07-05 05:22:24.000000 inhandtest-0.0.61/inhandtest/inrequest/dn.py
+-rw-rw-rw-   0        0        0    15433 2023-07-13 10:03:57.000000 inhandtest-0.0.61/inhandtest/inrequest/er_default_config.py
+-rw-rw-rw-   0        0        0    16311 2023-07-13 10:10:47.000000 inhandtest-0.0.61/inhandtest/inrequest/er_device.py
+-rw-rw-rw-   0        0        0     7352 2023-07-05 05:27:06.000000 inhandtest-0.0.61/inhandtest/inrequest/ics.py
+-rw-rw-rw-   0        0        0    10205 2023-07-13 10:03:57.000000 inhandtest-0.0.61/inhandtest/inrequest/inrequest.py
+-rw-rw-rw-   0        0        0    32013 2023-07-13 10:03:57.000000 inhandtest-0.0.61/inhandtest/inrequest/nezha.py
+-rw-rw-rw-   0        0        0     8389 2023-07-03 08:50:33.000000 inhandtest-0.0.61/inhandtest/inserial.py
+-rw-rw-rw-   0        0        0    16027 2023-07-06 07:21:54.000000 inhandtest-0.0.61/inhandtest/insocket.py
+-rw-rw-rw-   0        0        0     8481 2023-06-15 06:12:16.000000 inhandtest-0.0.61/inhandtest/inssh.py
+-rw-rw-rw-   0        0        0     1569 2023-05-24 09:45:24.000000 inhandtest-0.0.61/inhandtest/ip.py
+-rw-rw-rw-   0        0        0     1390 2023-06-15 09:39:25.000000 inhandtest-0.0.61/inhandtest/log.py
+-rw-rw-rw-   0        0        0    13757 2023-06-15 05:47:54.000000 inhandtest-0.0.61/inhandtest/mail.py
+-rw-rw-rw-   0        0        0      387 2023-06-12 09:08:02.000000 inhandtest-0.0.61/inhandtest/notice_email.html
+drwxrwxrwx   0        0        0        0 2023-07-13 10:13:10.000000 inhandtest-0.0.61/inhandtest/pages/
+-rw-rw-rw-   0        0        0      230 2023-05-31 07:29:45.000000 inhandtest-0.0.61/inhandtest/pages/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-13 10:13:10.000000 inhandtest-0.0.61/inhandtest/pages/ingateway/
+-rw-rw-rw-   0        0        0      136 2023-05-31 07:30:00.000000 inhandtest-0.0.61/inhandtest/pages/ingateway/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-13 10:13:10.000000 inhandtest-0.0.61/inhandtest/pages/ingateway/edge_computing/
+-rw-rw-rw-   0        0        0      134 2023-05-25 07:33:25.000000 inhandtest-0.0.61/inhandtest/pages/ingateway/edge_computing/__init__.py
+-rw-rw-rw-   0        0        0    67902 2023-07-10 10:29:49.000000 inhandtest-0.0.61/inhandtest/pages/ingateway/edge_computing/edge_computing_locators.py
+-rw-rw-rw-   0        0        0    72695 2023-07-10 09:51:55.000000 inhandtest-0.0.61/inhandtest/pages/ingateway/edge_computing/python_edge_computing.py
+-rw-rw-rw-   0        0        0     3247 2023-07-05 03:12:45.000000 inhandtest-0.0.61/inhandtest/pages/ingateway/ingateway.py
+-rw-rw-rw-   0        0        0    11890 2023-07-05 02:55:07.000000 inhandtest-0.0.61/inhandtest/pages/ingateway/locale.yml
+-rw-rw-rw-   0        0        0      911 2023-06-02 06:30:38.000000 inhandtest-0.0.61/inhandtest/pages/ingateway/locators.py
+drwxrwxrwx   0        0        0        0 2023-07-13 10:13:10.000000 inhandtest-0.0.61/inhandtest/pages/ingateway/network/
+-rw-rw-rw-   0        0        0      134 2023-05-15 07:33:50.000000 inhandtest-0.0.61/inhandtest/pages/ingateway/network/__init__.py
+-rw-rw-rw-   0        0        0    68039 2023-07-05 01:05:37.000000 inhandtest-0.0.61/inhandtest/pages/ingateway/network/network.py
+-rw-rw-rw-   0        0        0    86226 2023-07-05 01:05:03.000000 inhandtest-0.0.61/inhandtest/pages/ingateway/network/network_locators.py
+drwxrwxrwx   0        0        0        0 2023-07-13 10:13:10.000000 inhandtest-0.0.61/inhandtest/pages/ingateway/overview/
+-rw-rw-rw-   0        0        0      134 2023-05-15 07:33:50.000000 inhandtest-0.0.61/inhandtest/pages/ingateway/overview/__init__.py
+-rw-rw-rw-   0        0        0     6953 2023-06-02 09:29:07.000000 inhandtest-0.0.61/inhandtest/pages/ingateway/overview/overview.py
+-rw-rw-rw-   0        0        0     6260 2023-05-18 07:02:23.000000 inhandtest-0.0.61/inhandtest/pages/ingateway/overview/overview_locators.py
+drwxrwxrwx   0        0        0        0 2023-07-13 10:13:10.000000 inhandtest-0.0.61/inhandtest/pages/ingateway/system/
+-rw-rw-rw-   0        0        0      133 2023-06-02 06:29:57.000000 inhandtest-0.0.61/inhandtest/pages/ingateway/system/__init__.py
+-rw-rw-rw-   0        0        0    28514 2023-06-26 05:24:31.000000 inhandtest-0.0.61/inhandtest/pages/ingateway/system/system.py
+-rw-rw-rw-   0        0        0    30656 2023-06-26 05:24:31.000000 inhandtest-0.0.61/inhandtest/pages/ingateway/system/system_locators.py
+-rw-rw-rw-   0        0        0     1224 2023-04-28 06:53:30.000000 inhandtest-0.0.61/inhandtest/pytest_email.html
+-rw-rw-rw-   0        0        0    35349 2023-07-13 10:03:57.000000 inhandtest-0.0.61/inhandtest/telnet.py
+-rw-rw-rw-   0        0        0    30375 2023-07-13 10:03:57.000000 inhandtest-0.0.61/inhandtest/tools.py
+drwxrwxrwx   0        0        0        0 2023-07-13 10:13:10.000000 inhandtest-0.0.61/inhandtest.egg-info/
+-rw-rw-rw-   0        0        0      593 2023-07-13 10:13:09.000000 inhandtest-0.0.61/inhandtest.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1919 2023-07-13 10:13:09.000000 inhandtest-0.0.61/inhandtest.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-13 10:13:09.000000 inhandtest-0.0.61/inhandtest.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      123 2023-07-13 10:13:09.000000 inhandtest-0.0.61/inhandtest.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-13 10:13:09.000000 inhandtest-0.0.61/inhandtest.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      147 2023-06-01 10:06:41.000000 inhandtest-0.0.61/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-13 10:13:10.000000 inhandtest-0.0.61/setup.cfg
+-rw-rw-rw-   0        0        0     1615 2023-07-13 10:12:28.000000 inhandtest-0.0.61/setup.py
```

### Comparing `inhandtest-0.0.60/PKG-INFO` & `inhandtest-0.0.61/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: inhandtest
-Version: 0.0.60
+Version: 0.0.61
 Summary: inhand test tools, so easy
 Home-page: https://inhandnetworks.yuque.com/irhb08/mrpu1r/qgu0imvigkm2xry9?singleDoc# 《inhandtest docs》
 Author: liwei
 Author-email: liwei@inhand.com.cn
 Maintainer: liwei
 Maintainer-email: liwei@inhand.com.cn
 License: UNKNOWN
```

### Comparing `inhandtest-0.0.60/README.md` & `inhandtest-0.0.61/README.md`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.60/inhandtest/base_page/_ig_contents_locators.py` & `inhandtest-0.0.61/inhandtest/base_page/_ig_contents_locators.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.60/inhandtest/base_page/_ir3XX_contents_locators.py` & `inhandtest-0.0.61/inhandtest/base_page/_ir3XX_contents_locators.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.60/inhandtest/base_page/_vg710_contents_locators.py` & `inhandtest-0.0.61/inhandtest/base_page/_vg710_contents_locators.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.60/inhandtest/base_page/base_page.py` & `inhandtest-0.0.61/inhandtest/base_page/base_page.py`

 * *Files 1% similar despite different names*

```diff
@@ -303,40 +303,45 @@
             locator.fill(str(value), force=force)
             locator.blur()  # 鼠标移出输入框
             if log_desc:
                 logging.info(f'Device {self.host} fill {log_desc} {value}')
 
     @allure.step('点击按钮')
     def click(self, locator: Locator or list or tuple, log_desc=None, dialog_message: str = None,
-              tip_messages: str or list = None, wait_for_time: int = None, tip_messages_timeout=30) -> None:
+              tip_messages: str or list = None, text_messages: str or list = None, wait_for_time: int = None,
+              tip_messages_timeout=30) -> None:
         """ 封装公共的点击操作 支持多个元素点击, 对点击最后一次的属性做校验
 
         :param locator:  元素定位
         :param log_desc: 功能描述，用英文 如 Static Routing Destination
         :param dialog_message: str  点击按钮后有dialog弹出，并且期望对信息做验证， 支持模糊匹配, 点击最后一个元素
-        :param tip_messages: str or list 点击后等待该tip出现 再等待tip消失，如果有多个，使用列表传入
+        :param tip_messages: str or list 点击后等待该tip出现 再等待tip消失，如果有多个，使用列表传入 内容是正则表达式
                             tip_messages 是支持模糊匹配
                             该项校验 页面元素必须停留时间1秒及更多时间，否则不容易检测到导致报错， 点击最后一个元素
+        :param text_messages: str or list 点击后等待该文本内容出现，如果有多个，使用列表传入， 内容是正则表达式
         :param wait_for_time: ms  当做完所有操作后是否需要等待时间， 点击最后一个元素
         :param tip_messages_timeout: 默认30秒， 单位秒
         :return:
         """
+
         def last_click(last_locator: Locator):
             if not last_locator.is_disabled():
                 if dialog_message:
                     self.dialog_massage(last_locator.click, dialog_message)
                 else:
                     last_locator.click()
                 if log_desc:
                     logging.info(f'Device {self.host} click {log_desc}')
                 self.tip_messages(tip_messages, tip_messages_timeout)
+                self.text_messages(text_messages, tip_messages_timeout)
                 if wait_for_time:
                     self.page.wait_for_timeout(wait_for_time)
             else:
                 logging.warning(f'Device {self.host} click {log_desc} is disabled')
+
         if isinstance(locator, (tuple, list)):
             for locator_ in locator[:-1]:
                 locator_.click()
             last_click(locator[-1])
         elif isinstance(locator, Locator):
             last_click(locator)
         else:
@@ -904,23 +909,24 @@
                 self.radio(param_locator.get('locator'), value, param)
             elif param_locator.get('type') == 'switch_button':
                 self.switch_button(param_locator.get('locator'), value, param)
             elif param_locator.get('type') == 'expand':
                 self.expand(param_locator.get('locator'), value)  # 此处获取到的locator 是一个str
             elif param_locator.get('type') == 'button':
                 if value:
-                    dialog_message, tip_messages, wait_for_time, tip_messages_timeout = None, None, None, 30
+                    dialog_message, tip_messages, wait_for_time, text_messages, tip_messages_timeout = None, None, None, None, 30
                     if isinstance(value, dict):
                         dialog_message = value.get('dialog_message')
                         tip_messages = value.get('tip_messages')
                         wait_for_time = value.get('wait_for_time')
+                        text_messages = value.get('text_messages')
                         tip_messages_timeout = value.get('tip_messages_timeout') if value.get(
                             'tip_messages_timeout') is not None else 30
-                    self.click(param_locator.get('locator'), param, dialog_message, tip_messages, wait_for_time,
-                               tip_messages_timeout)
+                    self.click(param_locator.get('locator'), param, dialog_message, tip_messages, text_messages,
+                               wait_for_time, tip_messages_timeout)
             elif param_locator.get('type') == 'check':
                 if value:
                     value_, tip_messages = value, None
                     if isinstance(value, dict):
                         value_ = value.get('value')
                         tip_messages = value.get('tip_messages')
                     self.check(param_locator.get('locator'), value_, param, tip_messages)
```

### Comparing `inhandtest-0.0.60/inhandtest/base_page/table_tr.py` & `inhandtest-0.0.61/inhandtest/base_page/table_tr.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.60/inhandtest/exception.py` & `inhandtest-0.0.61/inhandtest/exception.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.60/inhandtest/file.py` & `inhandtest-0.0.61/inhandtest/file.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.60/inhandtest/inmodbus.py` & `inhandtest-0.0.61/inhandtest/inmodbus.py`

 * *Files 4% similar despite different names*

```diff
@@ -55,35 +55,40 @@
         :param datatype: 数据类型
         :param length: datatype为string类型时，必填项
         :param decimal: datatype为float类型时，必填项
         :return:
         """
         function_code_dict = {'0': cst.READ_COILS, '1': cst.READ_DISCRETE_INPUTS, '3': cst.READ_INPUT_REGISTERS,
                               '4': cst.READ_HOLDING_REGISTERS}
+        addr = str(addr)
         function_code = function_code_dict[addr[0]]
         # print('function code is %s' % function_code)
         self.logging.info('PLC address function code is %s.' % function_code)
         type_ = datatype.upper()
         data = None
         if function_code in [1, 2] and type_ == 'BIT':
             return self.master.execute(self.slave_id, function_code, int(addr[1:]) - 1, 1)[0]
         elif function_code in [3, 4] and type_ in \
-                ['INT', 'WORD', 'DINT', 'DWORD', 'LONG', 'ULONG', 'BCD', 'FLOAT', 'DOUBLE', 'STRING']:
+                ['INT', 'WORD', 'DINT', 'DWORD', 'LONG', 'ULONG', 'BCD16', 'BCD32', 'FLOAT', 'DOUBLE', 'STRING']:
             if type_ == 'INT':
                 data = self.read_holding_registers(addr, function_code, 1, symbol=True)[0]
-            elif type_ in ['WORD', 'BCD']:
+            elif type_ == 'WORD':
                 data = self.read_holding_registers(addr, function_code, 1, symbol=False)[0]
+            elif type_  == 'BCD16':
+                data = int('{:x}'.format(self.read_holding_registers(addr, function_code, 1, symbol=False)[0]))
             elif type_ == 'FLOAT':
                 data = self.read_float_data(addr, function_code)
-            elif type_ in ['DINT', 'DWORD']:
+            elif type_ in ['DINT', 'DWORD', 'BCD32']:
                 data_tuple = self.read_holding_registers(addr, function_code, 2, symbol=False)
                 if type_ == 'DINT':
                     data = self.read_not_16int_data(data_tuple, datatype=type_)
-                else:
+                elif type_ == 'DWORD':
                     data = ctypes.c_uint32(self.read_not_16int_data(data_tuple, datatype='DINT')).value
+                else:
+                    data = int('{:x}'.format(ctypes.c_uint32(self.read_not_16int_data(data_tuple, datatype='DINT')).value))
             elif type_ in ['LONG', 'ULONG', 'DOUBLE']:
                 data_tuple = self.read_holding_registers(addr, function_code, 4, symbol=False)
                 print(data_tuple)
                 if type_ == 'ULONG':
                     data = ctypes.c_uint64(self.read_not_16int_data(data_tuple, datatype='LONG')).value
                 else:
                     data = self.read_not_16int_data(data_tuple, datatype=type_)
@@ -105,33 +110,38 @@
         都指定寄存器地址写入值
         :param addr: 寄存器地址
         :param datatype: datatype
         :param write_value: 写入值
         :return:
         """
         type_ = datatype.upper()
-        address = int(addr[1:]) - 1
+        address = int(str(addr)[1:]) - 1
+        addr = str(addr)
         if isinstance(write_value, str) and type_ != 'STRING':
             write_value = int(write_value)
         if addr[0] == '0':
             if write_value not in [0, 1, True, False]:
                 logging.exception('This address type does not support writing such values.')
                 raise Exception('This address type does not support writing such values.')
             else:
                 self.master.execute(self.slave_id, cst.WRITE_MULTIPLE_COILS, address, output_value=[write_value])
         elif addr[0] == '4':
             if type_ == 'FLOAT':
                 self.write_float_data(addr, write_value)
             elif type_ == 'INT':
                 self.master.execute(self.slave_id, cst.WRITE_MULTIPLE_REGISTERS, address, output_value=[write_value],
                                     data_format=">" + (1 * "h"))
-            elif type_ in ['WORD', 'BCD']:
+            elif type_ in ['WORD', 'BCD16']:
+                if type_ == 'BCD16':
+                    write_value = int(write_value, 16)
                 self.master.execute(self.slave_id, cst.WRITE_MULTIPLE_REGISTERS, address, output_value=[write_value])
-            elif type_ in ['DINT', 'LONG', 'DOUBLE', 'DWORD', 'ULONG', 'STRING']:
-                if type_ in ['DWORD']:
+            elif type_ in ['DINT', 'LONG', 'DOUBLE', 'DWORD', 'ULONG', 'STRING', 'BCD32']:
+                if type_ in ['DWORD', 'BCD32']:
+                    if type_ == 'BCD32':
+                        write_value = int(write_value, 16)
                     value = ctypes.c_int32(write_value).value
                     type_ = 'DINT'
                 elif type_ in ['ULONG']:
                     value = ctypes.c_int64(write_value).value
                     type_ = 'LONG'
                 elif type_ == 'STRING':
                     value = write_value.ljust(math.ceil(len(write_value)/2) * 2)
```

### Comparing `inhandtest-0.0.60/inhandtest/inmongodb.py` & `inhandtest-0.0.61/inhandtest/inmongodb.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.60/inhandtest/inmqtt.py` & `inhandtest-0.0.61/inhandtest/inmqtt.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.60/inhandtest/inrequest/console.py` & `inhandtest-0.0.61/inhandtest/inrequest/console.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,14 +3,17 @@
 # @Author  : Pane Li
 # @File    : console.py
 """
 console
 
 """
 import logging
+
+from inhandtest.tools import dict_in
+
 from inhandtest.exception import ResourceNotFoundError
 from inhandtest.inrequest.inrequest import InRequest
 
 
 class Console:
     __doc__ = """nezha PaaS 后台 管理"""
 
@@ -77,17 +80,18 @@
             logging.exception(f'licenses create fail, please check the licenses info')
             raise
 
     def device(self, sn: str, action='delete', **kwargs):
         """
 
         :param sn: 设备序列号
-        :param action: delete
+        :param action: delete|info
         :param kwargs:
                 org_email: 当删除时， 如果填写了org_email, 则删除该机构下的设备，如果sn 为None, 则删除该机构下所有设备
+                state: {} 当获取到info 时 可以对 state 做判断
         :return:
         """
         if action == 'delete':
             oid = self.__get_org_info(kwargs.get('org_email')).get('_id') if kwargs.get('org_email') else None
             if sn:
                 param = {'oid': oid, 'serial_number': sn, 'limit': 100, 'page': 0}
                 _id = self.api.send_request(f'/api/v1/devices', 'get', param=param).json().get('result')[0].get('_id')
@@ -101,14 +105,18 @@
                         if result.get('total') == 0:
                             break
                         else:
                             for device in result.get('result'):
                                 self.api.send_request(f'api/v1/devices/{device.get("_id")}', 'delete')
                                 logging.debug(f'device {device.get("serialNumber")} delete success')
                     logging.info(f'admin delete {kwargs.get("org_email")} org all devices success')
+        elif action == 'info':
+            param = {'serial_number': sn, 'limit': 100, 'page': 0}
+            result = self.api.send_request(f'/api/v1/devices', 'get', param=param).json().get('result')[0]
+            dict_in(result, kwargs.get('state'))
 
     def user(self, email: str, action='update_password', **kwargs):
         """
 
         :param email: 用户邮箱
         :param action: update_password|delete
                     update_password:
@@ -150,21 +158,18 @@
                     self.org(org_email, action='delete')
                     self.api.send_request('api/v1/orgs', 'post', body=org_info)
                     logging.debug(f'admin create {org_info.get("email")} org success')
                 else:
                     self.user(org_email, action='update_password', password=kwargs.get('password'))
                     logging.debug(f'admin update {org_info.get("email")} org success')
             except ResourceNotFoundError:
+                try:
+                    self.user(org_email, 'delete')   # 删除该用户邮箱
+                except ResourceNotFoundError:
+                    pass
                 self.api.send_request('api/v1/orgs', 'post', body=org_info)
                 logging.debug(f'admin create {org_info.get("email")} org success')
         elif action == 'delete':
             org_id = self.__get_org_info(org_email).get('_id')
             self.device(sn='', action='delete', org_email=org_email)
             self.api.send_request(f'api/v1/orgs/{org_id}', 'delete')
             logging.info(f'admin delete {org_email} org success')
-
-
-if __name__ == '__main__':
-    from inhandtest.log import enable_log
-
-    enable_log(console_level='debug')
-    Console('123456', 'star.nezha.inhand.design').org('das@aliyun.com', 'create', password='123456', force=True)
```

### Comparing `inhandtest-0.0.60/inhandtest/inrequest/dm.py` & `inhandtest-0.0.61/inhandtest/inrequest/dm.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.60/inhandtest/inrequest/dn.py` & `inhandtest-0.0.61/inhandtest/inrequest/dn.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.60/inhandtest/inrequest/ics.py` & `inhandtest-0.0.61/inhandtest/inrequest/ics.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.60/inhandtest/inrequest/inrequest.py` & `inhandtest-0.0.61/inhandtest/inrequest/inrequest.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,31 +14,34 @@
 from inhandtest.file import file_hash
 from inhandtest.tools import dict_in, dict_merge
 import logging
 
 
 class InRequest:
 
-    def __init__(self, host: str, username: str, password: str, type_='device', protocol='https', port=443):
+    def __init__(self, host: str, username: str, password: str, type_='device', protocol='https', port=443, **kwargs):
         """支持设备，平台登录及操作API, 自动识别地址
 
         :param host:  主机地址，如果是平台的就填写平台server，如果是设备就填写设备的地址
         :param username:  用户名
         :param password: 密码
         :param type_: device|iot|ics|star|iscada|iwos|dn4  区分平台和设备
         :param protocol: 协议，当前只支持http https
         :param port: 端口
+        :param kwargs: 'device_model'
+                        device_model: 设备型号，用于区分设备类型
         """
         self.protocol = protocol
         self.host = host
         self.username = username
         self.password = password
         self.headers = {}
         self.type_ = type_
         self.port = port
+        self.device_model = kwargs.get('device_model').upper() if kwargs and 'device_model' in kwargs.keys() else None
         self.__login()
 
     def __url_pre(self, path: str):
         """host+path
 
         :param path:  请求路径
         :return:
@@ -85,16 +88,21 @@
             self.headers = {'Authorization': 'Bearer ' + response['access_token']}
             self.protocol = protocol_re
             self.host = host_re
         elif self.type_ == 'device':
             username_password = '%s:%s' % (self.username, self.password)
             base_auth = base64.b64encode(username_password.encode()).decode()
             self.headers = {'Authorization': 'Basic %s' % base_auth}
-            resp = self.send_request('v1/user/login', 'post').json()
-            self.headers['Authorization'] = 'Bearer ' + resp['results']['web_session']
+            if self.device_model and self.device_model in ('ER805',):
+                resp = self.send_request('/api/v1/user/login', 'post',
+                                         body={'username': self.username, 'password': self.password}).json()
+                self.headers['Authorization'] = 'Bearer ' + resp.get('result').get('token')
+            else:
+                resp = self.send_request('v1/user/login', 'post').json()
+                self.headers['Authorization'] = 'Bearer ' + resp['results']['web_session']
         logging.info(f'{self.username} login success')
 
     def send_request(self, path, method, param=None, body=None, expect=None, file_path=None,
                      params_type='json', header=None, code=200, auth=True):
         """封装http请求，根据请求方式及参数类型自动判断使用哪些参数来发送请求
 
         :param path: 请求路径
```

### Comparing `inhandtest-0.0.60/inhandtest/inrequest/nezha.py` & `inhandtest-0.0.61/inhandtest/inrequest/nezha.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,115 +7,148 @@
 
 """
 import logging
 import random
 import re
 import time
 from inhandtest.exception import TimeOutError, ResourceNotFoundError
-from inhandtest.tools import generate_string, replace_str, get_time_stamp
+from inhandtest.tools import generate_string, get_time_stamp, dict_in
 from inhandtest.inrequest.inrequest import InRequest
 
 
 class Base:
-    def __init__(self, api, email, host):
+    def __init__(self, api: InRequest, email: str, host: str):
         self.api = api
         self.host = host
         self.email = email
 
     @property
     def me(self) -> dict:
         """ 获取me的各种信息 包括oid
 
         :return:
         """
         return self.api.send_request('/api/v1/users/me', method='get', param={"expand": 'org'}).json().get('result')
 
+    def location_suggestion(self, q: str, provider, expect=None):
+        """位置查询
+
+        :param q: 位置
+        :param provider: 服务商 baidu|google
+        :param expect: 每个返回的地址都包含的字段
+        :return:
+        """
+        address = self.api.send_request('/api/v1/places/suggestion', method='get',
+                                        param={'q': q, 'provider': provider}).json().get('result')
+        if address:
+            if expect:
+                for item in address:
+                    assert expect in item.get('address')
+        else:
+            raise ResourceNotFoundError(f'the {q} address not found')
+
+
+class Overview(Base):
+
+    def __init__(self, api, email, host):
+        super().__init__(api, email, host)
+        self.__device = Device(api, email, host)
+
+    def map(self, sn: str, expect=None):
+        """对概览的地图进行验证
+
+        :param sn: 设备序列号
+        :param expect: 期望值  字典 {'location': {'source': 'gps'}}
+        :return:
+        """
+        if expect:
+            name = self.__device.info(sn).get('name')
+            devices = self.api.send_request('/api/v1/devices/locations', method='get').json().get('result')
+            for device in devices:
+                if device.get('name') == name:
+                    assert dict_in(device, expect)
+                    break
+
 
 class Device(Base):
+    def __init__(self, api, email, host):
+        super().__init__(api, email, host)
+        self.__firmware = Firmware(api, email, host)
 
-    def info(self, sn: str) -> dict:
+    def info(self, sn: str, type_='list') -> dict:
         """根据sn 转换属性 属性值有：  online: 在线|离线   True|False
                                        iccid:
                                        imei:
                                        imsi:
                                        version: 固件版本
                                        licenseStatus: 'licensed'
                                        sn: 序列号
                                        address
                                        _id: 设备_id
                                        name: 设备名字
                                        org:  {'_id': oid, 'name': 'org_name', 'email': 'org_email'}
-        :param sn: 列表
+        :param sn: 设备序列号
+        :param type_:  list|detail,  分别为设备列表或者设备详情返回该设备的信息
         :return: {'sn': $sn, 'online': 1, 'iccid': '', 'imei'}
         """
 
         try:
             response = self.api.send_request('/api/v1/devices', method='get', param={'serialNumber': sn}).json()
-            return response.get('result')[0]
+            info = response.get('result')[0]
         except Exception:
             raise ResourceNotFoundError(f'the device {sn} not exist')
+        if type_ == 'list':
+            return info
+        else:
+            return self.api.send_request(f'/api/v1/devices/{info["_id"]}', method='get').json().get('result')
 
     def add(self, sn: str, mac_or_imei: str) -> None:
         """添加设备，
 
         :param sn: 设备序列号
         :param mac_or_imei: 添加设备时需要依赖设备的mac地址或者IMEI号，去生产库查询该设备是否是映翰通设备
         :return:
         """
         validated_field = self.api.send_request(f'api/v1/serialnumber/{sn}/validate', method='post').json().get(
             'result').get('validatedField')
         try:
             self.info(sn)
         except ResourceNotFoundError:
             self.api.send_request('api/v1/devices', 'post',
-                                  body={"name": sn + str(int(time.time())), "serialNumber": sn, 'oid': self.me.oid,
+                                  body={"name": sn + str(int(time.time())), "serialNumber": sn,
+                                        'oid': self.me.get('oid'),
                                         validated_field: mac_or_imei})
         logging.info(f"the {sn} device add success")
 
-    def assert_state(self, sn: str, state: dict, timeout=120, interval=5) -> None:
+    def assert_state(self, sn: str, state: dict, timeout=120, interval=5, type_='list') -> None:
         """校验设备基本状态
 
         :param sn: 序列号
-        :param state:   支持表达式${value} ex: {'version': "'${value}' in 'V1.1.3.r4956'"}
+        :param state:
                         online: 在线|离线   True|False
                         iccid:
                         imei:
                         imsi:
                         version: 固件版本
                         licenseStatus: 'licensed'
                         sn: 序列号
                         address
         :param timeout: 校验信息，最大超时时间
         :param interval: 校验信息，校验间隔时间
+        :param type_: list|detail, 分别是列表和详情返回的具体信息
         :return: True or False
         """
         if state:
             for i in range(0, timeout, interval):
-                result = self.info(sn)
-                for key, value in state.items():
-                    if '${value}' in value:
-                        value = replace_str(value, {'${value}': result.get(key)})
-                        logging.debug(f'start assert {sn} state {key} {value}')
-                        try:
-                            if not eval(value):
-                                logging.debug(f'the {sn} device {key} info eval {value} is false')
-                                break
-                        except Exception as e:
-                            logging.error(e)
-                            break
-                    else:
-                        logging.debug(f'start assert {sn} state {key} {value}')
-                        if result.get(key) != value:
-                            logging.debug(f'the {sn} device {key} info value is {result.get(key)} not {value}')
-                            break
-                else:
-                    logging.info(f"check {sn} device all state success")
+                result = self.info(sn, type_)
+                try:
+                    dict_in(result, state)
                     break
-                logging.info(f"check {sn} device state failed, please wait for {interval}s")
-                time.sleep(interval)
+                except AssertionError:
+                    time.sleep(interval)
             else:
                 logging.exception(f"the {sn} state {state} check failed")
                 raise TimeOutError(f"the {sn} state {state} check failed")
 
     def delete(self, sn: str or list) -> None:
         """
 
@@ -164,14 +197,58 @@
             device_ids = [self.info(sn_).get('_id') for sn_ in sn]
             for license_, _id in zip(licenses_, device_ids):
                 self.api.send_request(f'/api/v1/billing/licenses/{license_}/device', 'put',
                                       body={'deviceId': _id},
                                       code=200)
             logging.info(f'bind license success')
 
+    def location(self, sn: str, type_='sync', location=None, address=None) -> None:
+        """对设备位置做操作
+
+        :param sn:
+        :param type_: sync|manually
+        :param location:  {"latitude":30.588423465204404,"longitude":104.0541738405845}  仅手动方式有用
+        :param address: "成都市-武侯区-府城大道西段399号"  仅手动方式有用
+        :return:  None
+        """
+        if type_ == 'sync':
+            body = {'pinned': False}
+        else:
+            body = {"pinned": True, "location": location, "address": address}
+        self.api.send_request(f'/api/v1/devices/{self.info(sn).get("_id")}/location', 'put', body=body)
+
+    def upgrade_firmware(self, sn: str or list, version: str, schedule=None) -> str:
+        """ 升级任务
+
+        :param sn: 设备序列号 一个或多个，他们需要都是同一个产品型号
+        :param version: 版本号
+        :param schedule: 计划升级时间， int， 单位分钟
+        :return str， job_id
+        """
+        if isinstance(sn, str):
+            product = self.info(sn).get('product')
+            _id = [self.info(sn).get('_id')]
+        else:
+            product = self.info(sn[0]).get('product')
+            _id = [self.info(sn_).get('_id') for sn_ in sn]
+        firmware_id = self.__firmware.info(product, version).get('_id')
+        payload = {"jobs": [{"targets": _id, "firmware": firmware_id}], "targetType": "device"}
+        if schedule:
+            payload["scheduledAt"] = get_time_stamp(delta=schedule, delta_type='m')
+        return self.api.send_request('/api/v1/firmwares/batch/jobs', 'post', body=payload).json().get('result')[0][
+            '_id']
+
+    def cancel_latest_task(self, sn: str):
+        detail = self.info(sn, 'detail')
+        if detail.get('firmwareUpgradeStatus'):
+            if detail.get('firmwareUpgradeStatus').get('status') == 'queued':
+                self.api.send_request(
+                    f'/api/v1/job/executions/{detail.get("firmwareUpgradeStatus").get("jobExecutionId")}/cancel',
+                    'put')
+
     def assert_cellular_history(self, sn: str, state, delta_day=-1, data_interval=None):
         """
 
         :param sn:
         :param state:
         :param delta_day: 查询开始时间的起点， 默认晚一天时间
         :param data_interval: 当查询的时间越长时，返回的数据会少，防止页面在渲染时卡顿，所以返回的数据间隔增大，可以对间隔做判断， 单位秒
@@ -225,14 +302,44 @@
             cellular_type = []
             for each_type in resp:
                 cellular_type.append(each_type['type'])
                 timestamp_ls = [i[0] for i in each_type['data']]
                 time_reduction(timestamp_ls, delta=data_interval)
             assert len(cellular_type) == len(set(cellular_type)), '蜂窝历史返回数据不对'
 
+    def assert_traffic(self, sn: str, date_='hourly', type_='overview', expect=None, **kwargs):
+        """
+
+        :param sn: 设备序列号
+        :param date_: hourly|daily|monthly
+        :param expect: 期望返回的内容
+        :param type_: overview|detail
+        :param kwargs: after|before|month|year|param
+                       after: int数, 在type_为hourly 时必传， 过期时间为天， 传0表示今天，传-1 表示昨天
+                       before: int数, 在type_为hourly 时必传， 过期时间为天， 传0表示今天，传-1 表示昨天
+                       month: 2023-07
+                       year: 查询今年传0， 过去一年 传-1， 依次类推
+        :return:
+        """
+        if date_ == 'hourly':
+            param = {'after': get_time_stamp('', kwargs.get('after'), 'd', '%Y-%m-%dT16:00:00.000Z'),
+                     'before': get_time_stamp('', kwargs.get('before'), 'd', '%Y-%m-%dT16:00:00.000Z')}
+        elif date_ == 'daily':
+            param = {'month': kwargs.get('month')}
+        else:
+            param = {'year': kwargs.get('year')}
+        if kwargs.get('param'):
+            param.update(kwargs.get('param'))
+        if type_ == 'overview':
+            self.api.send_request(f'/api/v1/devices/{self.info(sn).get("_id")}/datausage-{date_}/overview', 'get',
+                                  param=param, expect=expect, )
+        else:
+            self.api.send_request(f'/api/v1/devices/{self.info(sn).get("_id")}/datausage-{date_}', 'get',
+                                  param=param, expect=expect, )
+
 
 class Config(Base):
 
     def __init__(self, api, email, host):
         super().__init__(api, email, host)
         self.__device = Device(api, email, host)
         self.__group = Group(api, email, host)
@@ -281,17 +388,21 @@
         :param sn: 设备序列号
         :param expect: 配置内容，完整的配置路径，如{'lan': {'type': 'dhcp'}}
         :param type_: actual 实际设备上传的配置
                       group 设备所在组的配置
                       pending 正在下发的配置
                       target 目标配置
                       individual 个性化配置
+                      none
         :return: 如果 expect 为None 就返回设备当前实际的配置
         """
-        expect = {'result': {type_: expect}}
+        if type_ == 'none':
+            expect = {'result': expect}
+        else:
+            expect = {'result': {type_: expect}}
         if expect is not None:
             self.api.send_request(f'/api/v1/devices/{self.__device.info(sn).get("_id")}/config', 'get',
                                   expect=expect)
         else:
             return self.api.send_request(f'/api/v1/devices/{self.__device.info(sn).get("_id")}/config',
                                          'get').json().get('result').get(type_)
 
@@ -318,17 +429,17 @@
         """
         if target_sns:
             body = {"sourceDeviceId": self.__device.info(source_sn).get("_id"),
                     "targetDeviceIds": [self.__device.info(device).get('_id') for device in target_sns]}
             self.api.send_request(f'/api/v1/config/layer/bulk-copy', 'post', body=body, expect={"result": 'ok'})
         if target_group or target_group_id:
             if not target_group_id:
-                [self.__group.info(name).get('_id') for name in target_group]
+                target_group_id = [self.__group.info(name).get('_id') for name in target_group]
             body = {"sourceDeviceId": self.__device.info(source_sn).get("_id"),
-                    "targetGroupId": target_group_id}
+                    "targetGroupIds": target_group_id}
             self.api.send_request(f'/api/v1/config/layer/bulk-copy', 'post', body=body, expect={"result": 'ok'})
 
 
 class Org(Base):
 
     def org_info(self, name, _id=None, level=None) -> dict:
         for i in range(0, 20):  # 20次查询，如果组织数量超过100，就需要多次查询
@@ -483,40 +594,116 @@
         :param group_name: 设备序列号
         :param expect: 配置内容，完整的配置路径，如{'lan': {'type': 'dhcp'}}
         :param type_: actual 实际设备上传的配置
                       group 设备所在组的配置
                       pending 正在下发的配置
                       target 目标配置
                       individual 个性化配置
+                      'none'
         :param group_id: 分组id 二选一, 传入id时，不用传入group_name
         :return: 如果 expect 为None 就返回分组当前实际的配置
         """
-        expect = {'result': {type_: expect}}
+        if type_ == 'none':
+            expect = {'result': expect}
+        else:
+            expect = {'result': {type_: expect}}
         _id = self.info(group_name, group_id).get('_id')
         if expect is not None:
             self.api.send_request(f'/api/v1/config/layer/group/{_id}', 'get', expect=expect)
         else:
             return self.api.send_request(f'/api/v1/config/layer/group/{_id}', 'get').json().get('result').get(type_)
 
 
+class Firmware(Base):
+
+    def info(self, product: str, version=None) -> dict or list:
+        """查询账号下对应产品 已发布版本
+
+        :param product: ER805
+        :param version: None 当版本为None返回所有的已发布版本
+        :return:
+        """
+        param = {'fields': 'version,_id,latest,recommended', 'limit': 1000, 'status': 'published'}
+        ver = self.api.send_request(f'/api/v1/products/{product.upper()}/firmwares', 'get', param).json().get('result')
+        if version:
+            for v in ver:
+                if v.get('version') == version:
+                    return v
+            else:
+                raise ResourceNotFoundError(f'{product} product version {version} not publish')
+        else:
+            return ver
+
+
+class Log(Base):
+    def __init__(self, api, email, host):
+        super().__init__(api, email, host)
+        self.__device = Device(api, email, host)
+
+    def assert_job(self, job_id: str, **kwargs):
+        """
+        :param job_id: 任务id
+        :param kwargs:
+               status: canceled|
+               type: firmware
+               jobProcessDetails.total  总计下发的设备数
+        :return:
+        """
+        param = {'jobId': job_id, 'expand': 'jobProcessDetails', 'limit': 20, 'page': 0}
+        try:
+            result = self.api.send_request(f'api/v1/jobs', 'get', param=param).json().get('result')[0]
+        except IndexError:
+            raise ResourceNotFoundError(f'job {job_id} not found')
+        dict_in(result, kwargs)
+
+    def assert_device_task(self, sn: str, job_id: str, **kwargs):
+        param = {'jobId': job_id, 'serialNumber': sn, 'limit': 20, 'page': 0}
+        try:
+            result = self.api.send_request('/api/v1/job/executions', 'get', param=param).json().get('result')[0]
+        except IndexError:
+            raise ResourceNotFoundError(f'job {job_id} not found')
+        dict_in(result, kwargs)
+
+    def cancel_device_latest_task(self, sn: str):
+        param = {'serialNumber': sn, 'limit': 20, 'page': 0}
+        try:
+            result = self.api.send_request('/api/v1/job/executions', 'get', param=param).json().get('result')[0]
+            if result.get('status') == 'queued':
+                self.api.send_request(f'/api/v1/job/executions/{result.get("_id")}/cancel', 'put')
+            else:
+                logging.warning(f'the {sn} latest task status is {result.get("status")}, can not cancel')
+        except IndexError:
+            raise ResourceNotFoundError(f'the {sn} not has task')
+
+    def cancel_job(self, job_id: str):
+        """
+
+        :param job_id: 任务id
+        :return:
+        """
+        self.api.send_request(f'api/v1/jobs/{job_id}/cancel', 'put', expect={'result': 'ok'})
+
+
 class StarInterface:
 
     def __init__(self, email, password, host='star.inhandcloud.cn'):
         """ 须确保用户关闭了多因素认证
 
         :param email  平台用户名
         :param password  平台密码
         :param host: 'star.inhandcloud.cn'|'star.inhandcloud.cn'|'star.nezha.inhand.dev'|'star.nezha.inhand.design' 平台是哪个环境,
         """
         self.api = InRequest(host, email, password, 'star')
+        self.overview = Overview(self.api, email, host)
         self.device = Device(self.api, email, host)
         self.config = Config(self.api, email, host)
         self.org = Org(self.api, email, host)
         self.group = Group(self.api, email, host)
+        self.log = Log(self.api, email, host)
 
 
 if __name__ == '__main__':
     from inhandtest.log import enable_log
 
     enable_log(console_level='debug')
     star = StarInterface('liwei@inhand.com.cn', '123456', 'star.nezha.inhand.design')
-    print(star.device.delete('MR8051234501166'))
+    print(star.device.assert_traffic('RT805LIWEI82113', after=-1, before=0))
```

### Comparing `inhandtest-0.0.60/inhandtest/inserial.py` & `inhandtest-0.0.61/inhandtest/inserial.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.60/inhandtest/insocket.py` & `inhandtest-0.0.61/inhandtest/insocket.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.60/inhandtest/inssh.py` & `inhandtest-0.0.61/inhandtest/inssh.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.60/inhandtest/ip.py` & `inhandtest-0.0.61/inhandtest/ip.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.60/inhandtest/log.py` & `inhandtest-0.0.61/inhandtest/log.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.60/inhandtest/mail.py` & `inhandtest-0.0.61/inhandtest/mail.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.60/inhandtest/pages/ingateway/edge_computing/edge_computing_locators.py` & `inhandtest-0.0.61/inhandtest/pages/ingateway/edge_computing/edge_computing_locators.py`

 * *Files 0% similar despite different names*

```diff
@@ -371,14 +371,16 @@
             ('delete_confirm',
              {'locator': self.page.locator('.ant-popover-content').locator('.ant-btn.ant-btn-primary'),
               'type': 'button', 'wait_for': {'type': 'tip_messages', 'messages': self.locale.submit_success}}),
             ('value_edit', {'locator': self.page.locator(f'{measure_name}/../../../../td[6]//button'),
                             'type': 'button'}),
             ('value', {'locator': self.page.locator(f'{measure_name}/../../../../td[6]//input'),
                        'type': 'text'}),
+            ('value_select', {'locator': self.page.locator(f'{measure_name}/../../../../td[6]').locator(
+                '.ant-select.ant-select-enabled'), 'type': 'select'}),
             ('submit', {'locator': self.page.locator(f'{measure_name}/../../../../td[6]//i[2]'),
                         'type': 'button'}),
             ('text_messages', {'type': 'text_messages'}),
             ('tip_messages', {'type': 'tip_messages'}),
             ('cancel', {'locator': self.page.locator(f'{measure_name}/../../../../td[6]//i[1]'),
                         'type': 'button'}),
         ]
```

### Comparing `inhandtest-0.0.60/inhandtest/pages/ingateway/edge_computing/python_edge_computing.py` & `inhandtest-0.0.61/inhandtest/pages/ingateway/edge_computing/python_edge_computing.py`

 * *Files 1% similar despite different names*

```diff
@@ -275,18 +275,28 @@
                 self.agg_in(self.edge_locators.measure_operation, {'delete_bulk': True, 'delete_bulk_confirm': True})
             elif ac[0] == 'delete_all':
                 self.__measure([('check_all',)])
                 self.agg_in(self.edge_locators.measure_operation, {'delete_bulk': True, 'delete_bulk_confirm': True})
             elif ac[0] == 'delete':
                 self.agg_in(self.edge_locators.measure_table(ac[1]), {'delete': True, 'delete_confirm': True})
             elif ac[0] == 'value':
-                if isinstance(ac[2], str):
-                    value = {'value_edit': True, 'value': ac[2], 'submit': {"wait_for_time": 2 * 1000}}
+                if list(filter(lambda x: x[0] == 'datatype', self.edge_locators.measure_card_status(ac[1])))[0][1].get(
+                        'locator').inner_text() == 'BIT':    # BIT 类型时是选择框
+                    if isinstance(ac[2], str):
+                        value = {'value_edit': True, 'value_select': ac[2], 'submit': {"wait_for_time": 2 * 1000}}
+                    else:
+                        value = {'value_edit': True}
+                        ac[2]['value_select'] = ac[2].pop('value')
+                        value.update(ac[2])
                 else:
-                    value = {'value_edit': True}.update(ac[2])
+                    if isinstance(ac[2], str):
+                        value = {'value_edit': True, 'value': ac[2], 'submit': {"wait_for_time": 2 * 1000}}
+                    else:
+                        value = {'value_edit': True}
+                        value.update(ac[2])
                 self.agg_in(self.edge_locators.measure_table(ac[1]), value)
             elif ac[0] == 'add_to_group':
                 if ac[1] == 'all':
                     self.__measure([('check_all',)])
                 else:
                     self.agg_in(self.edge_locators.measure_operation, {'check_all': False})  # 先取消选择所有的
                     all_measure = [ac[1]] if isinstance(ac[1], str) else ac[1]
@@ -690,15 +700,16 @@
                     all_measure = [ac[1]] if isinstance(ac[1], str) else ac[1]
                     self.__measure_point(cloud_measure=[('check', x, True) for x in all_measure], mute_measure=None)
                     self.agg_in(self.edge_locators.cloud_measuring_point, {'mute_bulk': True, 'bulk_confirm': True})
                 elif ac[0] == 'name':
                     if isinstance(ac[2], str):
                         value = {'name_edit': True, 'value': ac[2], 'submit': {"wait_for_time": 3 * 1000}}
                     else:
-                        value = {'name_edit': True}.update(ac[2])
+                        value = {'name_edit': True}
+                        value.update(ac[2])
                     self.agg_in(self.edge_locators.cloud_measuring_point_table(ac[1]), value)
                 else:
                     pass
         if mute_measure:
             self.access_menu('edge_computing.device_supervisor.cloud.mqtt_cloud_service.cloud_measuring_setting.mute')
             for ac in mute_measure:
                 if ac[0] == 'search':
```

### Comparing `inhandtest-0.0.60/inhandtest/pages/ingateway/ingateway.py` & `inhandtest-0.0.61/inhandtest/pages/ingateway/ingateway.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.60/inhandtest/pages/ingateway/locale.yml` & `inhandtest-0.0.61/inhandtest/pages/ingateway/locale.yml`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.60/inhandtest/pages/ingateway/locators.py` & `inhandtest-0.0.61/inhandtest/pages/ingateway/locators.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.60/inhandtest/pages/ingateway/network/network.py` & `inhandtest-0.0.61/inhandtest/pages/ingateway/network/network.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.60/inhandtest/pages/ingateway/network/network_locators.py` & `inhandtest-0.0.61/inhandtest/pages/ingateway/network/network_locators.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.60/inhandtest/pages/ingateway/overview/overview.py` & `inhandtest-0.0.61/inhandtest/pages/ingateway/overview/overview.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.60/inhandtest/pages/ingateway/overview/overview_locators.py` & `inhandtest-0.0.61/inhandtest/pages/ingateway/overview/overview_locators.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.60/inhandtest/pages/ingateway/system/system.py` & `inhandtest-0.0.61/inhandtest/pages/ingateway/system/system.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.60/inhandtest/pages/ingateway/system/system_locators.py` & `inhandtest-0.0.61/inhandtest/pages/ingateway/system/system_locators.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.60/inhandtest/pytest_email.html` & `inhandtest-0.0.61/inhandtest/pytest_email.html`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.60/inhandtest/telnet.py` & `inhandtest-0.0.61/inhandtest/telnet.py`

 * *Files 2% similar despite different names*

```diff
@@ -318,19 +318,21 @@
                                  'last_read': 仅替换最后读取到的内容
                                  'cli_last_read': 既要替换cli 也要替换最后读取到的内容
                interface_replace_type: 'cli'|'last_read'|'cli_last_read'，仅在interface_replace 有值时生效，默认cli
                                  'cli': 仅替换发出去的命令
                                  'last_read': 仅替换最后读取到的内容
                                  'cli_last_read': 既要替换cli 也要替换最后读取到的内容
                read_until_timeout_no_raise: bool, 读取超时时是否抛出异常，默认False
+               read_content_decode: str, 读取内容的解码方式，默认cp936
 
         :return: 读取超时时返回Exception， 如果命令执行正确，返回最后一条命令输入后的结果
         """
         interface_replace_type = kwargs.get('interface_replace_type') if kwargs.get('interface_replace_type') else 'cli'
         key_replace_type = kwargs.get('key_replace_type') if kwargs.get('key_replace_type') else 'last_read'
+        read_content_decode = kwargs.get('read_content_decode') if kwargs.get('read_content_decode') else 'cp936'
         if kwargs.get('key_replace') and 'cli' in key_replace_type:  # 替换方法的关键字
             command = replace_str(command, kwargs.get('key_replace'))
         if self.interface_replace and 'cli' in interface_replace_type:  # 替换接口的关键字
             command = replace_str(command, self.interface_replace)
         timeout = kwargs.get('timeout') if kwargs.get('timeout') else 30
         result = ''
         if type_ == 'super':
@@ -355,15 +357,15 @@
                 read_until = [None for i in range(0, len(command))]
             self.tn.read_very_eager()
             for com, read_until_ in zip(command, read_until):
                 self.tn.write((com + "\n").encode("cp936"))
                 until_result = []
                 for i in range(0, timeout, 1):  # 30秒没有找到期望的就主动断开
                     time.sleep(1)
-                    result = self.tn.read_very_eager().decode('cp936', "ignore").strip().replace('\x08', '')
+                    result = self.tn.read_very_eager().decode(read_content_decode, "ignore").strip().replace('\x08', '')
                     if result:
                         logging.debug(result)
                         result = result.split(com + "\r\n")[-1]
                     if read_until_:
                         until_result.append(result)
                         if isinstance(read_until_, str):
                             if read_until_ in ''.join(until_result):
@@ -416,14 +418,26 @@
                                  'expect': 仅替换期望校验的值
                                  'cli_last_read'|'cli_expect'|'last_read_expect' 任意两种组合
 
                                  'cli_expect_last_read': 既要替换cli 也要替换最后读取到的内容还有校验的值
         :return: None|Exception
         """
 
+        def contain_(expect_, result_) -> bool:
+            if expect_ in result_:    # 为str 时 如果在里面直接返回True
+                return True
+            else:
+                try:
+                    if len(re.findall(expect_, result_)):   # 匹配正则表达式
+                        return True
+                    else:
+                        return False
+                except Exception:
+                    return False
+
         if key_replace is None:
             key_replace = {'\r\n': ''}
         if cli is not None:
             for i in range(0, timeout, interval):
                 if key_replace and 'cli' in key_replace_type:
                     cli = replace_str(cli, key_replace)
                     key_replace_type = key_replace_type.replace('cli', '')
@@ -435,28 +449,27 @@
                 if expect:
                     if 'expect' in key_replace_type:
                         expect = replace_str(expect, key_replace)
                     if 'expect' in interface_replace_type:
                         expect = replace_str(expect, self.interface_replace)
                     logging.debug(f'start assert cli expect {expect}')
                     if isinstance(expect, str):
-                        if not ((expect in result) or len(re.findall(expect, result))):
+                        if not contain_(expect, result):
                             check_ = False
                     elif isinstance(expect, list):
-                        if [expect_ for expect_ in expect if
-                                not ((expect_ in result) or len(re.findall(expect_, result)))]:
+                        if [expect_ for expect_ in expect if not contain_(expect_, result)]:
                             check_ = False
                     elif isinstance(expect, dict):
                         for k, v in expect.items():
                             if v:
-                                if not ((k in result) or len(re.findall(k, result))):
+                                if not contain_(k, result):
                                     check_ = False
                                     break
                             else:
-                                if (k in result) or len(re.findall(k, result)):
+                                if contain_(k, result):
                                     check_ = False
                                     break
                     else:
                         logging.exception(f'parameter expect type error, expect {expect}')
                         raise Exception('parameter expect is error')
                 if check_:
                     break
```

### Comparing `inhandtest-0.0.60/inhandtest/tools.py` & `inhandtest-0.0.61/inhandtest/tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -390,15 +390,15 @@
 
 
 def dict_in(expect_dict: dict, contain: dict) -> None:
     """验证字典包含关系
 
     :param expect_dict: dict {key: value}
     :param contain: dict,  支持${value} 表达式判断
-    :return: True or False
+    :return: AssertionError
     """
     if expect_dict and contain:
         contain_flatten = dict_flatten(contain)  # 平铺字典
         expect_dict_flatten = dict_flatten(expect_dict)  # 平铺字典
         for contain_item, contain_value in contain_flatten.items():
             value = expect_dict_flatten.get(contain_item)
             if isinstance(contain_value, str) and '${value}' in contain_value:
@@ -620,14 +620,15 @@
         except:
             pass
     else:
         logging.exception(f'all installed software is {all_installed}')
         raise ResourceNotFoundError(f'Not found the software {name}')
 
 
+
 @loop_inspector('PC Ping',)
 def pc_ping(host_or_ip: str or list or tuple = 'www.baidu.com', number: int = 4, src=None,
             lost_packets=False, assert_result=True, timeout=120, interval=10) -> bool:
     """ 验证在PC机上ping某个地址是否丢包， 仅判断丢包
 
     :param lost_packets:
     :param src: 验证的源IP地址 '192.168.2.100'
@@ -681,14 +682,16 @@
         except KeyError:
             logging.exception(f'Not found the key {key}')
             raise AttributeError(key)
 
     def __setattr__(self, key, value):
         self[key] = value
 
-
 if __name__ == '__main__':
-    kill_windows_port('10.5.24.224', 1111)
+    # kill_windows_port('10.5.24.224', 1111)
+
+    for i in range(0,10):
+        print(generate_uuid())
     # is_installed('Google Chrome123')
     # print(windows_cmd('route delete 192.168.2.102 mask 255.255.255.255 192.168.4.2', '操作完成', {' ': '', '\n': ''}))
     # print(generate_password(length=2, lowercase=True, uppercase=True, special_chars=True, chinese_chars=True))
     # print(get_time_stamp('2022-02-18T13:39:32Z', -2))
```

### Comparing `inhandtest-0.0.60/inhandtest.egg-info/PKG-INFO` & `inhandtest-0.0.61/inhandtest.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: inhandtest
-Version: 0.0.60
+Version: 0.0.61
 Summary: inhand test tools, so easy
 Home-page: https://inhandnetworks.yuque.com/irhb08/mrpu1r/qgu0imvigkm2xry9?singleDoc# 《inhandtest docs》
 Author: liwei
 Author-email: liwei@inhand.com.cn
 Maintainer: liwei
 Maintainer-email: liwei@inhand.com.cn
 License: UNKNOWN
```

### Comparing `inhandtest-0.0.60/inhandtest.egg-info/SOURCES.txt` & `inhandtest-0.0.61/inhandtest.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 inhandtest/base_page/_vg710_contents_locators.py
 inhandtest/base_page/base_page.py
 inhandtest/base_page/table_tr.py
 inhandtest/inrequest/__init__.py
 inhandtest/inrequest/console.py
 inhandtest/inrequest/dm.py
 inhandtest/inrequest/dn.py
+inhandtest/inrequest/er_default_config.py
 inhandtest/inrequest/er_device.py
 inhandtest/inrequest/ics.py
 inhandtest/inrequest/inrequest.py
 inhandtest/inrequest/nezha.py
 inhandtest/pages/__init__.py
 inhandtest/pages/ingateway/__init__.py
 inhandtest/pages/ingateway/ingateway.py
```

### Comparing `inhandtest-0.0.60/setup.py` & `inhandtest-0.0.61/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 """
 from distutils.core import setup
 from setuptools import find_packages
 
 setup(
     name='inhandtest',
-    version='0.0.60',
+    version='0.0.61',
     author='liwei',
     author_email='liwei@inhand.com.cn',
     description='inhand test tools, so easy',
     maintainer='liwei',
     maintainer_email='liwei@inhand.com.cn',
     # py_modules=['inhandtest.tools', 'inhandtest.telnet', 'inhandtest.inmodbus', 'inhandtest.inmqtt', 'inhandtest.file',
     #             'inhandtest.inrequest', 'inhandtest.inssh', 'inhandtest.base_page'],
```

