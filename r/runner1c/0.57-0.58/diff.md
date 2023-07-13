# Comparing `tmp/runner1c-0.57.tar.gz` & `tmp/runner1c-0.58.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "runner1c-0.57.tar", last modified: Tue Oct 18 11:13:24 2022, max compression
+gzip compressed data, was "runner1c-0.58.tar", last modified: Thu Jul 13 12:43:01 2023, max compression
```

## Comparing `runner1c-0.57.tar` & `runner1c-0.58.tar`

### file list

```diff
@@ -1,102 +1,106 @@
-drwxrwxrwx   0        0        0        0 2022-10-18 11:13:24.006751 runner1c-0.57/
--rw-rw-rw-   0        0        0     1363 2018-06-06 07:24:58.000000 runner1c-0.57/LICENSE
--rw-rw-rw-   0        0        0      248 2019-02-21 11:18:58.000000 runner1c-0.57/MANIFEST.in
--rw-rw-rw-   0        0        0      265 2022-10-18 11:13:24.006751 runner1c-0.57/PKG-INFO
--rw-rw-rw-   0        0        0      695 2022-01-26 08:04:08.000000 runner1c-0.57/README.md
-drwxrwxrwx   0        0        0        0 2022-10-18 11:13:23.875259 runner1c-0.57/runner1c/
--rw-rw-rw-   0        0        0       94 2022-10-18 11:10:09.000000 runner1c-0.57/runner1c/__init__.py
-drwxrwxrwx   0        0        0        0 2022-10-18 11:13:23.906502 runner1c-0.57/runner1c/build/
--rw-rw-rw-   0        0        0       68 2017-11-30 07:27:08.000000 runner1c-0.57/runner1c/build/README.md
-drwxrwxrwx   0        0        0        0 2022-10-18 11:13:23.844011 runner1c-0.57/runner1c/build/tools/
-drwxrwxrwx   0        0        0        0 2022-10-18 11:13:23.922126 runner1c-0.57/runner1c/build/tools/epf/
--rw-rw-rw-   0        0        0     5669 2022-10-18 09:38:23.000000 runner1c-0.57/runner1c/build/tools/epf/ChangeSafeModeForExtension.epf
--rw-rw-rw-   0        0        0     9688 2022-10-18 09:38:25.000000 runner1c-0.57/runner1c/build/tools/epf/CloseAfterUpdate.epf
--rw-rw-rw-   0        0        0     7837 2022-10-18 09:38:26.000000 runner1c-0.57/runner1c/build/tools/epf/FileCompareMxl.epf
--rw-rw-rw-   0        0        0    11349 2022-10-18 09:38:27.000000 runner1c-0.57/runner1c/build/tools/epf/Runner1C.epf
--rw-rw-rw-   0        0        0    18118 2022-07-15 12:08:24.000000 runner1c-0.57/runner1c/command.py
-drwxrwxrwx   0        0        0        0 2022-10-18 11:13:23.944252 runner1c-0.57/runner1c/commands/
--rw-rw-rw-   0        0        0        0 2018-01-31 10:55:59.000000 runner1c-0.57/runner1c/commands/__init__.py
--rw-rw-rw-   0        0        0     6632 2022-10-18 10:45:24.000000 runner1c-0.57/runner1c/commands/base_for_test.py
--rw-rw-rw-   0        0        0      417 2022-01-26 08:04:08.000000 runner1c-0.57/runner1c/commands/create_base.py
--rw-rw-rw-   0        0        0     1164 2022-01-26 08:04:08.000000 runner1c-0.57/runner1c/commands/create_epf.py
--rw-rw-rw-   0        0        0     1700 2022-01-26 08:04:08.000000 runner1c-0.57/runner1c/commands/diff_mxl.py
--rw-rw-rw-   0        0        0     7716 2022-07-15 12:08:24.000000 runner1c-0.57/runner1c/commands/dump_config.py
--rw-rw-rw-   0        0        0     2612 2022-01-26 08:04:08.000000 runner1c-0.57/runner1c/commands/dump_epf.py
--rw-rw-rw-   0        0        0     1334 2022-01-26 08:04:08.000000 runner1c-0.57/runner1c/commands/dump_extensions.py
--rw-rw-rw-   0        0        0      895 2022-01-26 08:04:08.000000 runner1c-0.57/runner1c/commands/file.py
--rw-rw-rw-   0        0        0     2153 2022-01-26 08:04:08.000000 runner1c-0.57/runner1c/commands/load_config.py
--rw-rw-rw-   0        0        0     5917 2022-03-11 11:36:57.000000 runner1c-0.57/runner1c/commands/load_extension.py
--rw-rw-rw-   0        0        0     5318 2022-01-26 08:04:08.000000 runner1c-0.57/runner1c/commands/platform_check.py
--rw-rw-rw-   0        0        0      956 2022-01-27 09:51:20.000000 runner1c-0.57/runner1c/commands/reg_server.py
--rw-rw-rw-   0        0        0     1749 2022-01-26 08:04:08.000000 runner1c-0.57/runner1c/commands/start.py
--rw-rw-rw-   0        0        0      821 2022-01-26 08:04:08.000000 runner1c-0.57/runner1c/commands/start_agent.py
--rw-rw-rw-   0        0        0     9361 2022-07-15 12:08:24.000000 runner1c-0.57/runner1c/commands/sync.py
--rw-rw-rw-   0        0        0      442 2022-01-26 08:04:08.000000 runner1c-0.57/runner1c/commands/version.py
--rw-rw-rw-   0        0        0     1114 2022-01-26 08:04:08.000000 runner1c-0.57/runner1c/commands/webinst.py
--rw-rw-rw-   0        0        0     2776 2022-07-15 12:08:24.000000 runner1c-0.57/runner1c/common.py
--rw-rw-rw-   0        0        0     2433 2022-03-11 10:41:24.000000 runner1c-0.57/runner1c/core.py
--rw-rw-rw-   0        0        0      208 2022-01-26 07:47:39.000000 runner1c-0.57/runner1c/exit_code.py
--rw-rw-rw-   0        0        0     1766 2022-01-26 07:47:39.000000 runner1c-0.57/runner1c/parser.py
-drwxrwxrwx   0        0        0        0 2022-10-18 11:13:23.944252 runner1c-0.57/runner1c/tests/
--rw-rw-rw-   0        0        0        0 2018-01-31 10:55:59.000000 runner1c-0.57/runner1c/tests/__init__.py
--rw-rw-rw-   0        0        0      432 2022-01-26 07:47:39.000000 runner1c-0.57/runner1c/tests/conftest.py
--rw-rw-rw-   0        0        0      599 2022-01-26 07:47:39.000000 runner1c-0.57/runner1c/tests/test_diff_mxl.py
--rw-rw-rw-   0        0        0      632 2022-01-26 07:47:39.000000 runner1c-0.57/runner1c/tests/test_sync_without_base.py
--rw-rw-rw-   0        0        0     1082 2022-01-26 07:47:39.000000 runner1c-0.57/runner1c/tests/test_version.py
--rw-rw-rw-   0        0        0     6351 2022-07-15 12:08:24.000000 runner1c-0.57/runner1c/tests/test_with_base.py
-drwxrwxrwx   0        0        0        0 2022-10-18 11:13:23.944252 runner1c-0.57/runner1c/tools/
--rw-rw-rw-   0        0        0     6630 2022-07-15 12:08:24.000000 runner1c-0.57/runner1c/tools/create_base_for_test.py
-drwxrwxrwx   0        0        0        0 2022-10-18 11:13:23.991132 runner1c-0.57/runner1c/tools/epf/
-drwxrwxrwx   0        0        0        0 2022-10-18 11:13:23.844011 runner1c-0.57/runner1c/tools/epf/ChangeSafeModeForExtension/
-drwxrwxrwx   0        0        0        0 2022-10-18 11:13:23.991132 runner1c-0.57/runner1c/tools/epf/ChangeSafeModeForExtension/Forms/
-drwxrwxrwx   0        0        0        0 2022-10-18 11:13:23.844011 runner1c-0.57/runner1c/tools/epf/ChangeSafeModeForExtension/Forms/Form/
-drwxrwxrwx   0        0        0        0 2022-10-18 11:13:23.991132 runner1c-0.57/runner1c/tools/epf/ChangeSafeModeForExtension/Forms/Form/Ext/
-drwxrwxrwx   0        0        0        0 2022-10-18 11:13:23.991132 runner1c-0.57/runner1c/tools/epf/ChangeSafeModeForExtension/Forms/Form/Ext/Form/
--rw-rw-rw-   0        0        0     1050 2022-07-15 07:16:21.000000 runner1c-0.57/runner1c/tools/epf/ChangeSafeModeForExtension/Forms/Form/Ext/Form/Module.bsl
--rw-rw-rw-   0        0        0     1340 2022-07-15 07:16:21.000000 runner1c-0.57/runner1c/tools/epf/ChangeSafeModeForExtension/Forms/Form/Ext/Form.xml
--rw-rw-rw-   0        0        0     1513 2022-07-15 07:16:21.000000 runner1c-0.57/runner1c/tools/epf/ChangeSafeModeForExtension/Forms/Form.xml
--rw-rw-rw-   0        0        0     1921 2022-07-15 07:16:21.000000 runner1c-0.57/runner1c/tools/epf/ChangeSafeModeForExtension.xml
-drwxrwxrwx   0        0        0        0 2022-10-18 11:13:23.844011 runner1c-0.57/runner1c/tools/epf/CloseAfterUpdate/
-drwxrwxrwx   0        0        0        0 2022-10-18 11:13:23.991132 runner1c-0.57/runner1c/tools/epf/CloseAfterUpdate/Ext/
--rw-rw-rw-   0        0        0     2001 2022-07-15 07:40:45.000000 runner1c-0.57/runner1c/tools/epf/CloseAfterUpdate/Ext/ObjectModule.bsl
-drwxrwxrwx   0        0        0        0 2022-10-18 11:13:23.991132 runner1c-0.57/runner1c/tools/epf/CloseAfterUpdate/Forms/
-drwxrwxrwx   0        0        0        0 2022-10-18 11:13:23.859638 runner1c-0.57/runner1c/tools/epf/CloseAfterUpdate/Forms/Managed/
-drwxrwxrwx   0        0        0        0 2022-10-18 11:13:23.991132 runner1c-0.57/runner1c/tools/epf/CloseAfterUpdate/Forms/Managed/Ext/
-drwxrwxrwx   0        0        0        0 2022-10-18 11:13:23.991132 runner1c-0.57/runner1c/tools/epf/CloseAfterUpdate/Forms/Managed/Ext/Form/
--rw-rw-rw-   0        0        0     2983 2022-07-15 12:08:24.000000 runner1c-0.57/runner1c/tools/epf/CloseAfterUpdate/Forms/Managed/Ext/Form/Module.bsl
--rw-rw-rw-   0        0        0     2170 2022-07-15 07:40:45.000000 runner1c-0.57/runner1c/tools/epf/CloseAfterUpdate/Forms/Managed/Ext/Form.xml
--rw-rw-rw-   0        0        0     1519 2022-07-15 07:40:45.000000 runner1c-0.57/runner1c/tools/epf/CloseAfterUpdate/Forms/Managed.xml
-drwxrwxrwx   0        0        0        0 2022-10-18 11:13:23.859638 runner1c-0.57/runner1c/tools/epf/CloseAfterUpdate/Forms/Ordinary/
-drwxrwxrwx   0        0        0        0 2022-10-18 11:13:23.991132 runner1c-0.57/runner1c/tools/epf/CloseAfterUpdate/Forms/Ordinary/Ext/
-drwxrwxrwx   0        0        0        0 2022-10-18 11:13:23.991132 runner1c-0.57/runner1c/tools/epf/CloseAfterUpdate/Forms/Ordinary/Ext/Form/
--rw-rw-rw-   0        0        0     1720 2022-07-15 07:40:45.000000 runner1c-0.57/runner1c/tools/epf/CloseAfterUpdate/Forms/Ordinary/Ext/Form/Module.bsl
--rw-rw-rw-   0        0        0     5911 2022-07-15 07:51:27.000000 runner1c-0.57/runner1c/tools/epf/CloseAfterUpdate/Forms/Ordinary/Ext/Form.bin
--rw-rw-rw-   0        0        0     1522 2022-07-15 07:40:45.000000 runner1c-0.57/runner1c/tools/epf/CloseAfterUpdate/Forms/Ordinary.xml
--rw-rw-rw-   0        0        0     2035 2022-07-15 07:40:45.000000 runner1c-0.57/runner1c/tools/epf/CloseAfterUpdate.xml
-drwxrwxrwx   0        0        0        0 2022-10-18 11:13:23.859638 runner1c-0.57/runner1c/tools/epf/FileCompareMxl/
-drwxrwxrwx   0        0        0        0 2022-10-18 11:13:23.991132 runner1c-0.57/runner1c/tools/epf/FileCompareMxl/Forms/
-drwxrwxrwx   0        0        0        0 2022-10-18 11:13:23.859638 runner1c-0.57/runner1c/tools/epf/FileCompareMxl/Forms/Form/
-drwxrwxrwx   0        0        0        0 2022-10-18 11:13:24.006751 runner1c-0.57/runner1c/tools/epf/FileCompareMxl/Forms/Form/Ext/
-drwxrwxrwx   0        0        0        0 2022-10-18 11:13:24.006751 runner1c-0.57/runner1c/tools/epf/FileCompareMxl/Forms/Form/Ext/Form/
--rw-rw-rw-   0        0        0    10183 2022-07-15 12:08:24.000000 runner1c-0.57/runner1c/tools/epf/FileCompareMxl/Forms/Form/Ext/Form/Module.bsl
--rw-rw-rw-   0        0        0    19173 2022-07-15 12:08:24.000000 runner1c-0.57/runner1c/tools/epf/FileCompareMxl/Forms/Form/Ext/Form.bin
--rw-rw-rw-   0        0        0     1514 2022-07-15 07:40:46.000000 runner1c-0.57/runner1c/tools/epf/FileCompareMxl/Forms/Form.xml
--rw-rw-rw-   0        0        0     1871 2022-07-15 07:40:46.000000 runner1c-0.57/runner1c/tools/epf/FileCompareMxl.xml
-drwxrwxrwx   0        0        0        0 2022-10-18 11:13:23.859638 runner1c-0.57/runner1c/tools/epf/Runner1C/
-drwxrwxrwx   0        0        0        0 2022-10-18 11:13:24.006751 runner1c-0.57/runner1c/tools/epf/Runner1C/Forms/
-drwxrwxrwx   0        0        0        0 2022-10-18 11:13:23.859638 runner1c-0.57/runner1c/tools/epf/Runner1C/Forms/Form/
-drwxrwxrwx   0        0        0        0 2022-10-18 11:13:24.006751 runner1c-0.57/runner1c/tools/epf/Runner1C/Forms/Form/Ext/
-drwxrwxrwx   0        0        0        0 2022-10-18 11:13:24.006751 runner1c-0.57/runner1c/tools/epf/Runner1C/Forms/Form/Ext/Form/
--rw-rw-rw-   0        0        0    28763 2022-08-18 06:01:03.000000 runner1c-0.57/runner1c/tools/epf/Runner1C/Forms/Form/Ext/Form/Module.bsl
--rw-rw-rw-   0        0        0    10582 2022-08-18 06:01:03.000000 runner1c-0.57/runner1c/tools/epf/Runner1C/Forms/Form/Ext/Form.xml
--rw-rw-rw-   0        0        0     1513 2022-08-18 05:46:14.000000 runner1c-0.57/runner1c/tools/epf/Runner1C/Forms/Form.xml
--rw-rw-rw-   0        0        0     1845 2022-08-18 05:46:14.000000 runner1c-0.57/runner1c/tools/epf/Runner1C.xml
-drwxrwxrwx   0        0        0        0 2022-10-18 11:13:23.890884 runner1c-0.57/runner1c.egg-info/
--rw-rw-rw-   0        0        0      265 2022-10-18 11:13:23.000000 runner1c-0.57/runner1c.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2484 2022-10-18 11:13:23.000000 runner1c-0.57/runner1c.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-10-18 11:13:23.000000 runner1c-0.57/runner1c.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2022-10-18 11:13:23.000000 runner1c-0.57/runner1c.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       67 2022-10-18 11:13:23.000000 runner1c-0.57/runner1c.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2022-10-18 11:13:23.000000 runner1c-0.57/runner1c.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-10-18 11:13:24.006751 runner1c-0.57/setup.cfg
--rw-rw-rw-   0        0        0      770 2022-01-26 07:47:39.000000 runner1c-0.57/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-13 12:43:01.364266 runner1c-0.58/
+-rw-rw-rw-   0        0        0     1363 2018-06-06 07:24:58.000000 runner1c-0.58/LICENSE
+-rw-rw-rw-   0        0        0      248 2019-02-21 11:18:58.000000 runner1c-0.58/MANIFEST.in
+-rw-rw-rw-   0        0        0      265 2023-07-13 12:43:01.364266 runner1c-0.58/PKG-INFO
+-rw-rw-rw-   0        0        0      708 2023-03-06 10:43:08.000000 runner1c-0.58/README.md
+drwxrwxrwx   0        0        0        0 2023-07-13 12:43:01.270517 runner1c-0.58/runner1c/
+-rw-rw-rw-   0        0        0       94 2023-07-13 12:41:40.000000 runner1c-0.58/runner1c/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-13 12:43:01.270517 runner1c-0.58/runner1c/build/
+-rw-rw-rw-   0        0        0       68 2017-11-30 07:27:08.000000 runner1c-0.58/runner1c/build/README.md
+drwxrwxrwx   0        0        0        0 2023-07-13 12:43:01.239282 runner1c-0.58/runner1c/build/tests/
+drwxrwxrwx   0        0        0        0 2023-07-13 12:43:01.239282 runner1c-0.58/runner1c/build/tests/repo/
+drwxrwxrwx   0        0        0        0 2023-07-13 12:43:01.270517 runner1c-0.58/runner1c/build/tests/repo/epf/
+-rw-rw-rw-   0        0        0     5563 2022-11-29 12:38:31.000000 runner1c-0.58/runner1c/build/tests/repo/epf/CheckConfig.epf
+drwxrwxrwx   0        0        0        0 2023-07-13 12:43:01.239282 runner1c-0.58/runner1c/build/tools/
+drwxrwxrwx   0        0        0        0 2023-07-13 12:43:01.286140 runner1c-0.58/runner1c/build/tools/epf/
+-rw-rw-rw-   0        0        0     5669 2022-11-29 12:38:33.000000 runner1c-0.58/runner1c/build/tools/epf/ChangeSafeModeForExtension.epf
+-rw-rw-rw-   0        0        0     9691 2022-11-29 12:38:35.000000 runner1c-0.58/runner1c/build/tools/epf/CloseAfterUpdate.epf
+-rw-rw-rw-   0        0        0     7837 2022-11-29 12:38:36.000000 runner1c-0.58/runner1c/build/tools/epf/FileCompareMxl.epf
+-rw-rw-rw-   0        0        0    11501 2023-02-27 08:40:08.000000 runner1c-0.58/runner1c/build/tools/epf/Runner1C.epf
+-rw-rw-rw-   0        0        0    18974 2023-03-06 11:18:23.000000 runner1c-0.58/runner1c/command.py
+drwxrwxrwx   0        0        0        0 2023-07-13 12:43:01.317389 runner1c-0.58/runner1c/commands/
+-rw-rw-rw-   0        0        0        0 2018-01-31 10:55:59.000000 runner1c-0.58/runner1c/commands/__init__.py
+-rw-rw-rw-   0        0        0     9674 2023-03-13 11:07:31.000000 runner1c-0.58/runner1c/commands/base_for_test.py
+-rw-rw-rw-   0        0        0      417 2022-01-26 08:04:08.000000 runner1c-0.58/runner1c/commands/create_base.py
+-rw-rw-rw-   0        0        0     1164 2022-01-26 08:04:08.000000 runner1c-0.58/runner1c/commands/create_epf.py
+-rw-rw-rw-   0        0        0     1700 2022-01-26 08:04:08.000000 runner1c-0.58/runner1c/commands/diff_mxl.py
+-rw-rw-rw-   0        0        0     7716 2023-03-06 11:18:23.000000 runner1c-0.58/runner1c/commands/dump_config.py
+-rw-rw-rw-   0        0        0     2612 2022-01-26 08:04:08.000000 runner1c-0.58/runner1c/commands/dump_epf.py
+-rw-rw-rw-   0        0        0     1334 2022-01-26 08:04:08.000000 runner1c-0.58/runner1c/commands/dump_extensions.py
+-rw-rw-rw-   0        0        0      895 2022-01-26 08:04:08.000000 runner1c-0.58/runner1c/commands/file.py
+-rw-rw-rw-   0        0        0     2127 2022-12-23 07:28:15.000000 runner1c-0.58/runner1c/commands/load_config.py
+-rw-rw-rw-   0        0        0     6045 2023-02-27 10:03:54.000000 runner1c-0.58/runner1c/commands/load_extension.py
+-rw-rw-rw-   0        0        0     5233 2023-07-13 12:10:01.000000 runner1c-0.58/runner1c/commands/platform_check.py
+-rw-rw-rw-   0        0        0      956 2022-01-27 09:51:20.000000 runner1c-0.58/runner1c/commands/reg_server.py
+-rw-rw-rw-   0        0        0     1749 2022-01-26 08:04:08.000000 runner1c-0.58/runner1c/commands/start.py
+-rw-rw-rw-   0        0        0      821 2022-01-26 08:04:08.000000 runner1c-0.58/runner1c/commands/start_agent.py
+-rw-rw-rw-   0        0        0     9397 2022-12-23 07:28:15.000000 runner1c-0.58/runner1c/commands/sync.py
+-rw-rw-rw-   0        0        0      442 2022-01-26 08:04:08.000000 runner1c-0.58/runner1c/commands/version.py
+-rw-rw-rw-   0        0        0     1114 2022-01-26 08:04:08.000000 runner1c-0.58/runner1c/commands/webinst.py
+-rw-rw-rw-   0        0        0     2889 2022-12-23 07:28:15.000000 runner1c-0.58/runner1c/common.py
+-rw-rw-rw-   0        0        0     2406 2022-11-30 15:41:24.000000 runner1c-0.58/runner1c/core.py
+-rw-rw-rw-   0        0        0      208 2022-01-26 07:47:39.000000 runner1c-0.58/runner1c/exit_code.py
+-rw-rw-rw-   0        0        0     2851 2023-02-14 07:03:32.000000 runner1c-0.58/runner1c/parser.py
+drwxrwxrwx   0        0        0        0 2023-07-13 12:43:01.333020 runner1c-0.58/runner1c/tests/
+-rw-rw-rw-   0        0        0        0 2018-01-31 10:55:59.000000 runner1c-0.58/runner1c/tests/__init__.py
+-rw-rw-rw-   0        0        0      432 2022-01-26 07:47:39.000000 runner1c-0.58/runner1c/tests/conftest.py
+-rw-rw-rw-   0        0        0      599 2022-01-26 07:47:39.000000 runner1c-0.58/runner1c/tests/test_diff_mxl.py
+-rw-rw-rw-   0        0        0      632 2022-01-26 07:47:39.000000 runner1c-0.58/runner1c/tests/test_sync_without_base.py
+-rw-rw-rw-   0        0        0     1082 2022-01-26 07:47:39.000000 runner1c-0.58/runner1c/tests/test_version.py
+-rw-rw-rw-   0        0        0     5803 2023-07-13 08:47:16.000000 runner1c-0.58/runner1c/tests/test_with_base.py
+drwxrwxrwx   0        0        0        0 2023-07-13 12:43:01.333020 runner1c-0.58/runner1c/tools/
+-rw-rw-rw-   0        0        0     6716 2023-02-27 10:04:24.000000 runner1c-0.58/runner1c/tools/create_base_for_test.py
+drwxrwxrwx   0        0        0        0 2023-07-13 12:43:01.333020 runner1c-0.58/runner1c/tools/epf/
+drwxrwxrwx   0        0        0        0 2023-07-13 12:43:01.239282 runner1c-0.58/runner1c/tools/epf/ChangeSafeModeForExtension/
+drwxrwxrwx   0        0        0        0 2023-07-13 12:43:01.333020 runner1c-0.58/runner1c/tools/epf/ChangeSafeModeForExtension/Forms/
+drwxrwxrwx   0        0        0        0 2023-07-13 12:43:01.239282 runner1c-0.58/runner1c/tools/epf/ChangeSafeModeForExtension/Forms/Form/
+drwxrwxrwx   0        0        0        0 2023-07-13 12:43:01.333020 runner1c-0.58/runner1c/tools/epf/ChangeSafeModeForExtension/Forms/Form/Ext/
+drwxrwxrwx   0        0        0        0 2023-07-13 12:43:01.333020 runner1c-0.58/runner1c/tools/epf/ChangeSafeModeForExtension/Forms/Form/Ext/Form/
+-rw-rw-rw-   0        0        0     1050 2022-07-15 07:16:21.000000 runner1c-0.58/runner1c/tools/epf/ChangeSafeModeForExtension/Forms/Form/Ext/Form/Module.bsl
+-rw-rw-rw-   0        0        0     1340 2022-07-15 07:16:21.000000 runner1c-0.58/runner1c/tools/epf/ChangeSafeModeForExtension/Forms/Form/Ext/Form.xml
+-rw-rw-rw-   0        0        0     1513 2022-07-15 07:16:21.000000 runner1c-0.58/runner1c/tools/epf/ChangeSafeModeForExtension/Forms/Form.xml
+-rw-rw-rw-   0        0        0     1921 2022-07-15 07:16:21.000000 runner1c-0.58/runner1c/tools/epf/ChangeSafeModeForExtension.xml
+drwxrwxrwx   0        0        0        0 2023-07-13 12:43:01.239282 runner1c-0.58/runner1c/tools/epf/CloseAfterUpdate/
+drwxrwxrwx   0        0        0        0 2023-07-13 12:43:01.333020 runner1c-0.58/runner1c/tools/epf/CloseAfterUpdate/Ext/
+-rw-rw-rw-   0        0        0     2001 2022-07-15 07:40:45.000000 runner1c-0.58/runner1c/tools/epf/CloseAfterUpdate/Ext/ObjectModule.bsl
+drwxrwxrwx   0        0        0        0 2023-07-13 12:43:01.348642 runner1c-0.58/runner1c/tools/epf/CloseAfterUpdate/Forms/
+drwxrwxrwx   0        0        0        0 2023-07-13 12:43:01.239282 runner1c-0.58/runner1c/tools/epf/CloseAfterUpdate/Forms/Managed/
+drwxrwxrwx   0        0        0        0 2023-07-13 12:43:01.348642 runner1c-0.58/runner1c/tools/epf/CloseAfterUpdate/Forms/Managed/Ext/
+drwxrwxrwx   0        0        0        0 2023-07-13 12:43:01.348642 runner1c-0.58/runner1c/tools/epf/CloseAfterUpdate/Forms/Managed/Ext/Form/
+-rw-rw-rw-   0        0        0     2983 2022-07-15 12:08:24.000000 runner1c-0.58/runner1c/tools/epf/CloseAfterUpdate/Forms/Managed/Ext/Form/Module.bsl
+-rw-rw-rw-   0        0        0     2170 2022-07-15 07:40:45.000000 runner1c-0.58/runner1c/tools/epf/CloseAfterUpdate/Forms/Managed/Ext/Form.xml
+-rw-rw-rw-   0        0        0     1519 2022-07-15 07:40:45.000000 runner1c-0.58/runner1c/tools/epf/CloseAfterUpdate/Forms/Managed.xml
+drwxrwxrwx   0        0        0        0 2023-07-13 12:43:01.239282 runner1c-0.58/runner1c/tools/epf/CloseAfterUpdate/Forms/Ordinary/
+drwxrwxrwx   0        0        0        0 2023-07-13 12:43:01.348642 runner1c-0.58/runner1c/tools/epf/CloseAfterUpdate/Forms/Ordinary/Ext/
+drwxrwxrwx   0        0        0        0 2023-07-13 12:43:01.348642 runner1c-0.58/runner1c/tools/epf/CloseAfterUpdate/Forms/Ordinary/Ext/Form/
+-rw-rw-rw-   0        0        0     1720 2022-07-15 07:40:45.000000 runner1c-0.58/runner1c/tools/epf/CloseAfterUpdate/Forms/Ordinary/Ext/Form/Module.bsl
+-rw-rw-rw-   0        0        0     5911 2022-07-15 07:51:27.000000 runner1c-0.58/runner1c/tools/epf/CloseAfterUpdate/Forms/Ordinary/Ext/Form.bin
+-rw-rw-rw-   0        0        0     1522 2022-07-15 07:40:45.000000 runner1c-0.58/runner1c/tools/epf/CloseAfterUpdate/Forms/Ordinary.xml
+-rw-rw-rw-   0        0        0     2035 2022-07-15 07:40:45.000000 runner1c-0.58/runner1c/tools/epf/CloseAfterUpdate.xml
+drwxrwxrwx   0        0        0        0 2023-07-13 12:43:01.239282 runner1c-0.58/runner1c/tools/epf/FileCompareMxl/
+drwxrwxrwx   0        0        0        0 2023-07-13 12:43:01.348642 runner1c-0.58/runner1c/tools/epf/FileCompareMxl/Forms/
+drwxrwxrwx   0        0        0        0 2023-07-13 12:43:01.239282 runner1c-0.58/runner1c/tools/epf/FileCompareMxl/Forms/Form/
+drwxrwxrwx   0        0        0        0 2023-07-13 12:43:01.348642 runner1c-0.58/runner1c/tools/epf/FileCompareMxl/Forms/Form/Ext/
+drwxrwxrwx   0        0        0        0 2023-07-13 12:43:01.364266 runner1c-0.58/runner1c/tools/epf/FileCompareMxl/Forms/Form/Ext/Form/
+-rw-rw-rw-   0        0        0    10183 2022-07-15 12:08:24.000000 runner1c-0.58/runner1c/tools/epf/FileCompareMxl/Forms/Form/Ext/Form/Module.bsl
+-rw-rw-rw-   0        0        0    19173 2022-07-15 12:08:24.000000 runner1c-0.58/runner1c/tools/epf/FileCompareMxl/Forms/Form/Ext/Form.bin
+-rw-rw-rw-   0        0        0     1514 2022-07-15 07:40:46.000000 runner1c-0.58/runner1c/tools/epf/FileCompareMxl/Forms/Form.xml
+-rw-rw-rw-   0        0        0     1871 2022-07-15 07:40:46.000000 runner1c-0.58/runner1c/tools/epf/FileCompareMxl.xml
+drwxrwxrwx   0        0        0        0 2023-07-13 12:43:01.239282 runner1c-0.58/runner1c/tools/epf/Runner1C/
+drwxrwxrwx   0        0        0        0 2023-07-13 12:43:01.364266 runner1c-0.58/runner1c/tools/epf/Runner1C/Forms/
+drwxrwxrwx   0        0        0        0 2023-07-13 12:43:01.239282 runner1c-0.58/runner1c/tools/epf/Runner1C/Forms/Form/
+drwxrwxrwx   0        0        0        0 2023-07-13 12:43:01.364266 runner1c-0.58/runner1c/tools/epf/Runner1C/Forms/Form/Ext/
+drwxrwxrwx   0        0        0        0 2023-07-13 12:43:01.364266 runner1c-0.58/runner1c/tools/epf/Runner1C/Forms/Form/Ext/Form/
+-rw-rw-rw-   0        0        0    29395 2023-02-27 08:40:18.000000 runner1c-0.58/runner1c/tools/epf/Runner1C/Forms/Form/Ext/Form/Module.bsl
+-rw-rw-rw-   0        0        0    10896 2023-02-27 08:40:18.000000 runner1c-0.58/runner1c/tools/epf/Runner1C/Forms/Form/Ext/Form.xml
+-rw-rw-rw-   0        0        0     1513 2023-02-27 08:40:18.000000 runner1c-0.58/runner1c/tools/epf/Runner1C/Forms/Form.xml
+-rw-rw-rw-   0        0        0     1845 2023-02-27 08:40:18.000000 runner1c-0.58/runner1c/tools/epf/Runner1C.xml
+drwxrwxrwx   0        0        0        0 2023-07-13 12:43:01.270517 runner1c-0.58/runner1c.egg-info/
+-rw-rw-rw-   0        0        0      265 2023-07-13 12:43:01.000000 runner1c-0.58/runner1c.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2530 2023-07-13 12:43:01.000000 runner1c-0.58/runner1c.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-13 12:43:01.000000 runner1c-0.58/runner1c.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-07-13 12:43:01.000000 runner1c-0.58/runner1c.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       14 2023-07-13 12:43:01.000000 runner1c-0.58/runner1c.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-13 12:43:01.000000 runner1c-0.58/runner1c.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-13 12:43:01.364266 runner1c-0.58/setup.cfg
+-rw-rw-rw-   0        0        0      684 2023-02-14 07:03:32.000000 runner1c-0.58/setup.py
```

### Comparing `runner1c-0.57/LICENSE` & `runner1c-0.58/LICENSE`

 * *Files identical despite different names*

### Comparing `runner1c-0.57/README.md` & `runner1c-0.58/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -4,8 +4,8 @@
 # runner1c
 
 Пакет для работы с 1с из python.
 Поддерживает запуск в режиме предприятия, в режиме конфигуратора.
 Режим конфигуратора может быть запущен в режиме агента.
 
 Должна быть установлена платформа 1с версии не ниже 8.3.10.2667.
-Работа проверялась на платформе 1с версии 8.3.10.2667, 8.3.12.1714, 8.3.20.1674
+Работа проверялась на платформе 1с версии 8.3.10.2667, 8.3.12.1714, 8.3.20.1674, 8.3.22.1750
```

### Comparing `runner1c-0.57/runner1c/build/tools/epf/ChangeSafeModeForExtension.epf` & `runner1c-0.58/runner1c/build/tools/epf/ChangeSafeModeForExtension.epf`

 * *Files 20% similar despite different names*

```diff
@@ -30,16 +30,16 @@
 000001d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000200: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000210: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000220: 0000 0000 0000 0000 0000 0000 0000 000d  ................
 00000230: 0a30 3030 3030 3036 3020 3030 3030 3030  .00000060 000000
-00000240: 3630 2037 6666 6666 6666 6620 0d0a f03d  60 7fffffff ...=
-00000250: ebe6 4544 0200 f03d ebe6 4544 0200 0000  ..ED...=..ED....
+00000240: 3630 2037 6666 6666 6666 6620 0d0a 90a7  60 7fffffff ....
+00000250: 4b60 4e44 0200 90a7 4b60 4e44 0200 0000  K`ND....K`ND....
 00000260: 0000 3800 3900 6600 3600 3200 6200 6300  ..8.9.f.6.2.b.c.
 00000270: 3100 2d00 3900 6600 6500 3900 2d00 3400  1.-.9.f.e.9.-.4.
 00000280: 6600 3800 3900 2d00 6200 3600 3900 3100  f.8.9.-.b.6.9.1.
 00000290: 2d00 3800 3100 6200 6200 3200 3000 3300  -.8.1.b.b.2.0.3.
 000002a0: 3700 3400 3300 6300 6600 0000 0000 0d0a  7.4.3.c.f.......
 000002b0: 3030 3030 3031 3637 2030 3030 3030 3230  00000167 0000020
 000002c0: 3020 3766 6666 6666 6666 200d 0a8d 913d  0 7fffffff ....=
@@ -72,16 +72,16 @@
 00000470: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000480: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000490: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000004a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000004b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000004c0: 0000 0000 0000 0000 0000 0000 000d 0a30  ...............0
 000004d0: 3030 3030 3036 3020 3030 3030 3030 3630  0000060 00000060
-000004e0: 2037 6666 6666 6666 6620 0d0a f03d ebe6   7fffffff ...=..
-000004f0: 4544 0200 f03d ebe6 4544 0200 0000 0000  ED...=..ED......
+000004e0: 2037 6666 6666 6666 6620 0d0a 90a7 4b60   7fffffff ....K`
+000004f0: 4e44 0200 90a7 4b60 4e44 0200 0000 0000  ND....K`ND......
 00000500: 6100 6100 3900 3800 3300 6400 3000 3000  a.a.9.8.3.d.0.0.
 00000510: 2d00 3200 3500 3400 3700 2d00 3400 6100  -.2.5.4.7.-.4.a.
 00000520: 3700 6100 2d00 6100 3200 6500 6200 2d00  7.a.-.a.2.e.b.-.
 00000530: 6500 6400 3900 6300 3900 3300 3700 6600  e.d.9.c.9.3.7.f.
 00000540: 3800 6100 3300 6200 0000 0000 0d0a 3030  8.a.3.b.......00
 00000550: 3030 3030 3966 2030 3030 3030 3230 3020  00009f 00000200 
 00000560: 3766 6666 6666 6666 200d 0a95 8f41 0a02  7fffffff ....A..
@@ -114,16 +114,16 @@
 00000710: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000720: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000730: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000740: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000750: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000760: 0000 0000 0000 0000 0000 000d 0a30 3030  .............000
 00000770: 3030 3036 3420 3030 3030 3030 3634 2037  00064 00000064 7
-00000780: 6666 6666 6666 6620 0d0a f03d ebe6 4544  fffffff ...=..ED
-00000790: 0200 f03d ebe6 4544 0200 0000 0000 6100  ...=..ED......a.
+00000780: 6666 6666 6666 6620 0d0a 90a7 4b60 4e44  fffffff ....K`ND
+00000790: 0200 90a7 4b60 4e44 0200 0000 0000 6100  ....K`ND......a.
 000007a0: 6100 3900 3800 3300 6400 3000 3000 2d00  a.9.8.3.d.0.0.-.
 000007b0: 3200 3500 3400 3700 2d00 3400 6100 3700  2.5.4.7.-.4.a.7.
 000007c0: 6100 2d00 6100 3200 6500 6200 2d00 6500  a.-.a.2.e.b.-.e.
 000007d0: 6400 3900 6300 3900 3300 3700 6600 3800  d.9.c.9.3.7.f.8.
 000007e0: 6100 3300 6200 2e00 3000 0000 0000 0d0a  a.3.b...0.......
 000007f0: 3030 3030 3034 3861 2030 3030 3030 3438  0000048a 0000048
 00000800: 6120 3766 6666 6666 6666 200d 0ab5 546d  a 7fffffff ...Tm
@@ -197,16 +197,16 @@
 00000c40: da0a 2ee6 97c6 611a fa35 180a f15e 0f46  ......a..5...^.F
 00000c50: 3030 e84d 1d9b ce98 18f1 869d 2636 db12  00.M........&6..
 00000c60: 4eb6 2518 9e61 27ab f7b6 01ae 905d dbc9  N.%..a'......]..
 00000c70: 1684 724d cf2f 8c31 293b 5a76 c484 b2f8  ..rM./.1);Zv....
 00000c80: eff2 26b0 80fd b1d8 2a08 6b15 d511 ef4e  ..&.....*.k....N
 00000c90: fc4f 5d7f d2db bf0d 0a30 3030 3030 3032  .O]......0000002
 00000ca0: 3820 3030 3030 3030 3238 2037 6666 6666  8 00000028 7ffff
-00000cb0: 6666 6620 0d0a f03d ebe6 4544 0200 f03d  fff ...=..ED...=
-00000cc0: ebe6 4544 0200 0000 0000 6300 6f00 7000  ..ED......c.o.p.
+00000cb0: 6666 6620 0d0a 90a7 4b60 4e44 0200 90a7  fff ....K`ND....
+00000cc0: 4b60 4e44 0200 0000 0000 6300 6f00 7000  K`ND......c.o.p.
 00000cd0: 7900 6900 6e00 6600 6f00 0000 0000 0d0a  y.i.n.f.o.......
 00000ce0: 3030 3030 3030 6463 2030 3030 3030 3230  000000dc 0000020
 00000cf0: 3020 3766 6666 6666 6666 200d 0a8d 9031  0 7fffffff ....1
 00000d00: 4e04 310c 45fb 95f6 1253 c792 2776 12a7  N.1.E....S..'v..
 00000d10: 46d0 5171 024f 6203 053b d242 81b4 da93  F.Qq.Ob..;.B....
 00000d20: 5170 24ae c0cc b0f4 d37c 4bd6 f7d7 fbfe  Qp$......|K.....
 00000d30: f9fa be70 381e 2e71 95c4 c418 a543 e9d6  ...p8..q.....C..
@@ -235,16 +235,16 @@
 00000ea0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000eb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000ec0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000ed0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000ee0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000ef0: 0000 0000 0000 0000 0000 0000 000d 0a30  ...............0
 00000f00: 3030 3030 3032 3020 3030 3030 3030 3230  0000020 00000020
-00000f10: 2037 6666 6666 6666 6620 0d0a f03d ebe6   7fffffff ...=..
-00000f20: 4544 0200 f03d ebe6 4544 0200 0000 0000  ED...=..ED......
+00000f10: 2037 6666 6666 6666 6620 0d0a 90a7 4b60   7fffffff ....K`
+00000f20: 4e44 0200 90a7 4b60 4e44 0200 0000 0000  ND....K`ND......
 00000f30: 7200 6f00 6f00 7400 0000 0000 0d0a 3030  r.o.o.t.......00
 00000f40: 3030 3030 3265 2030 3030 3030 3230 3020  00002e 00000200 
 00000f50: 3766 6666 6666 6666 200d 0a7b bf7b 7fb5  7fffffff ..{.{..
 00000f60: 918e 8565 9a99 5152 b2a1 ae65 5aaa a5ae  ...e..QR...eZ...
 00000f70: 499a 85a5 6e92 99a5 a1ae 8561 5292 9181  I...n......aR...
 00000f80: b1b9 8971 729a 4e2d 0000 0000 0000 0000  ...qr.N-........
 00000f90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -273,16 +273,16 @@
 00001100: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001110: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001120: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001130: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001140: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001150: 0000 0000 0000 0000 0000 000d 0a30 3030  .............000
 00001160: 3030 3032 3620 3030 3030 3030 3236 2037  00026 00000026 7
-00001170: 6666 6666 6666 6620 0d0a f03d ebe6 4544  fffffff ...=..ED
-00001180: 0200 f03d ebe6 4544 0200 0000 0000 7600  ...=..ED......v.
+00001170: 6666 6666 6666 6620 0d0a 90a7 4b60 4e44  fffffff ....K`ND
+00001180: 0200 90a7 4b60 4e44 0200 0000 0000 7600  ....K`ND......v.
 00001190: 6500 7200 7300 6900 6f00 6e00 0000 0000  e.r.s.i.o.n.....
 000011a0: 0d0a 3030 3030 3030 3163 2030 3030 3030  ..0000001c 00000
 000011b0: 3230 3020 3766 6666 6666 6666 200d 0a7b  200 7fffffff ..{
 000011c0: bf7b 7f35 2f57 b591 a199 8e81 0e90 6161  .{.5/W........aa
 000011d0: 606c 68a4 6350 cbcb 0542 0000 0000 0000  `lh.cP...B......
 000011e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000011f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -311,38 +311,38 @@
 00001360: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001370: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001380: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001390: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000013a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000013b0: 0000 0000 0000 0000 0000 0000 0000 000d  ................
 000013c0: 0a30 3030 3030 3032 3820 3030 3030 3030  .00000028 000000
-000013d0: 3238 2037 6666 6666 6666 6620 0d0a f03d  28 7fffffff ...=
-000013e0: ebe6 4544 0200 f03d ebe6 4544 0200 0000  ..ED...=..ED....
+000013d0: 3238 2037 6666 6666 6666 6620 0d0a 90a7  28 7fffffff ....
+000013e0: 4b60 4e44 0200 90a7 4b60 4e44 0200 0000  K`ND....K`ND....
 000013f0: 0000 7600 6500 7200 7300 6900 6f00 6e00  ..v.e.r.s.i.o.n.
-00001400: 7300 0000 0000 0d0a 3030 3030 3031 3163  s.......0000011c
+00001400: 7300 0000 0000 0d0a 3030 3030 3031 3161  s.......0000011a
 00001410: 2030 3030 3030 3230 3020 3766 6666 6666   00000200 7fffff
-00001420: 6666 200d 0a8d 9031 6e58 3108 40ef e2d9  ff ....1nX1.@...
-00001430: 4436 601b 8e03 3648 59f2 aba4 aa54 553d  D6`...6HY....TU=
-00001440: 5986 1ea9 57a8 a7ce d910 7a42 8ff7 f7f3  Y...W.....zB....
-00001450: cfaf 5ea5 9652 7577 db36 161c 9e0c 1c92  ..^..Ruw.6......
-00001460: 60da 0d30 da56 eeb9 5aec 5a44 73a2 ef0e  `..0.V..Z.ZDs...
-00001470: 9aa1 c029 0a3e b583 7477 6cb4 9876 961a  ...).>..twl..v..
-00001480: e94c 2608 7e74 0153 dca9 0d04 0ba2 1342  .L&.~t.S.......B
-00001490: 49e8 b598 a9d0 690d 70f0 a56c 1918 8643  I.....i.p..l...C
-000014a0: 1cdd 4a2b c5c8 af57 8f0c 4186 1396 c03c  ..J+...W..A....<
-000014b0: 02c4 5880 dd5b b4e6 7138 bf76 eba5 953a  ..X..[..q8.v...:
-000014c0: 8c75 3326 20df df78 e306 9579 60f6 4ee6  .u3& ..x...y`.N.
-000014d0: 918c 7a6a d9cf b79f af6f f994 4a2d ad9f  ..zj.....o..J-..
-000014e0: d1c1 47bb 557c 3398 6d84 d345 968b 63cf  ..G.U|3.m..E..c.
-000014f0: 5be5 fd79 be97 ca6a 71c6 1c20 d41c 7812  [..y...jq.. ..x.
-00001500: 82b2 3738 429c d395 685e f647 bc7f bc3e  ..78B...h^.G...>
-00001510: 6fa5 5edb 8ea7 099c a409 2c57 ca31 07e8  o.^.......,W.1..
-00001520: 9e7e c269 f9f2 fff8 47a9 73e0 a179 268c  .~.i....G.s..y&.
-00001530: d874 4374 05ed 3c80 ee7e 6b4b deb9 7fff  .tCt..<..~kK....
-00001540: 0300 0000 0000 0000 0000 0000 0000 0000  ................
+00001420: 6666 200d 0a8d 9031 4e45 310c 04ef 923a  ff ....1NE1....:
+00001430: 4676 e2c4 f671 9cc4 9168 78e8 7f84 8410  Fv...q...hx.....
+00001440: 27a3 e048 5c81 d050 d38f 7667 f7fb f3eb  '..H\..P..vg....
+00001450: 9db2 e694 7247 2124 2920 ac06 6c88 e0e8  ....rG!$) ..l...
+00001460: 0b7c 99b5 36d9 a397 9cd4 762f 6312 d88e  .|..6.....v/c...
+00001470: 43ed 838e 6e04 4a63 14ac c275 ee94 8daa  C...n.Jc...u....
+00001480: ae90 00ae 7d02 8fae e0a5 1c74 51db 3e69  ....}......tQ.>i
+00001490: 0b71 4eee a675 9d9e d258 805d fc50 3120  .qN..u...X.].P1 
+000014a0: 964d abb2 d5eb 4899 4fb4 73af 40de 0a30  .M....H.O.s.@..0
+000014b0: 7686 d1a6 8089 ebe0 903e 86fe 2feb 018f  v........>../...
+000014c0: 992b 7624 84a6 4ec0 6b05 78c5 09ad 6aec  .+v$..N.k.x...j.
+000014d0: 6dcc dd2d a779 3dbf 3d3e ed2b 655a bbc6  m..-.y=.=>.+eZ..
+000014e0: 7286 703e 7b27 1770 3b0a 6895 0997 c7da  r.p>{'.p;.h.....
+000014f0: 92d3 edba 5e0e 3ba5 d888 0045 7560 2ac7  ....^.;....Eu`*.
+00001500: c17f d91e 88ad 6057 6e39 bdc6 edfe 783d  ......`Wn9....x=
+00001510: 9dc3 6d5b 0c73 20a3 f394 c906 271c 50c9  ..m[.s .....'.P.
+00001520: ac4c d428 c67f f83d 6591 8d47 6241 48d1  .L.(...=e..GbAH.
+00001530: 3311 8fba 7687 1eab 1599 246c f6f1 0300  3...v.....$l....
+00001540: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001550: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001560: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001570: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001580: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001590: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000015a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000015b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
```

### Comparing `runner1c-0.57/runner1c/build/tools/epf/CloseAfterUpdate.epf` & `runner1c-0.58/runner1c/build/tools/epf/CloseAfterUpdate.epf`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 00000000: ffff ff7f 0002 0000 0a00 0000 0000 0000  ................
 00000010: 0d0a 3030 3030 3030 3738 2030 3030 3030  ..00000078 00000
 00000020: 3230 3020 3766 6666 6666 6666 200d 0a2f  200 7fffffff ../
-00000030: 0200 00b2 0200 00ff ffff 7fd5 0500 0054  ...............T
-00000040: 0600 00ff ffff 7f73 0800 00f6 0800 00ff  .......s........
-00000050: ffff 7f1a 0f00 0099 0f00 00ff ffff 7fb8  ................
-00000060: 1100 003b 1200 00ff ffff 7fac 1900 002b  ...;...........+
-00000070: 1a00 00ff ffff 7f4a 1c00 0091 1c00 00ff  .......J........
-00000080: ffff 7fb0 1e00 00ef 1e00 00ff ffff 7f0e  ................
-00000090: 2100 0053 2100 00ff ffff 7f72 2300 00b9  !..S!......r#...
+00000030: 0200 00b2 0200 00ff ffff 7fd8 0500 0057  ...............W
+00000040: 0600 00ff ffff 7f76 0800 00f9 0800 00ff  .......v........
+00000050: ffff 7f1d 0f00 009c 0f00 00ff ffff 7fbb  ................
+00000060: 1100 003e 1200 00ff ffff 7faf 1900 002e  ...>............
+00000070: 1a00 00ff ffff 7f4d 1c00 0094 1c00 00ff  .......M........
+00000080: ffff 7fb3 1e00 00f2 1e00 00ff ffff 7f11  ................
+00000090: 2100 0056 2100 00ff ffff 7f75 2300 00bc  !..V!......u#...
 000000a0: 2300 00ff ffff 7f00 0000 0000 0000 0000  #...............
 000000b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000100: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -30,92 +30,92 @@
 000001d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000200: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000210: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000220: 0000 0000 0000 0000 0000 0000 0000 000d  ................
 00000230: 0a30 3030 3030 3036 3420 3030 3030 3030  .00000064 000000
-00000240: 3634 2037 6666 6666 6666 6620 0d0a 108c  64 7fffffff ....
-00000250: ebe6 4544 0200 108c ebe6 4544 0200 0000  ..ED......ED....
+00000240: 3634 2037 6666 6666 6666 6620 0d0a b0f5  64 7fffffff ....
+00000250: 4b60 4e44 0200 b0f5 4b60 4e44 0200 0000  K`ND....K`ND....
 00000260: 0000 3500 3100 6100 3000 3400 3000 6400  ..5.1.a.0.4.0.d.
 00000270: 3400 2d00 6200 6100 3800 3500 2d00 3400  4.-.b.a.8.5.-.4.
 00000280: 3800 3600 3900 2d00 3800 3700 3200 3100  8.6.9.-.8.7.2.1.
 00000290: 2d00 3000 3400 3700 6600 3500 3400 6200  -.0.4.7.f.5.4.b.
 000002a0: 6500 3000 6400 6400 3700 2e00 3000 0000  e.0.d.d.7...0...
-000002b0: 0000 0d0a 3030 3030 3033 3034 2030 3030  ....00000304 000
-000002c0: 3030 3330 3420 3766 6666 6666 6666 200d  00304 7fffffff .
-000002d0: 0aed 55cd 4e13 5114 1ed9 39c9 bcc3 4dd9  ..U.N.Q...9...M.
-000002e0: b4b1 4291 0546 74a7 f145 a489 1bdd b830  ..B..Ft..E.....0
-000002f0: 31c6 4e8b 2029 9140 3412 1281 127f 5626  1.N. ).@4.....V&
-00000300: 4371 6ca1 76fa 0ae7 be83 71e3 c247 a8df  Cql.v.....q..G..
-00000310: 3977 ee74 3a53 5282 4b9d b6d3 3be7 ff3b  9w.t:SR.K...;..;
-00000320: 7f33 1c0e 5f38 338e 73c5 3197 e756 e45a  .3.._83.s.1..V.Z
-00000330: b8a9 92c3 52d5 5cca 73ef 4364 0dbf 21d4  ....R.\.s.Cd..!.
-00000340: 3e42 edc7 8c39 5bb5 1b15 951c 526a ceca  >B...9[.....Rj..
-00000350: af9f f7ee 42d6 fee3 7ae8 3c72 aace e331  ....B...z.<r...1
-00000360: af95 aa8a b5c7 d47f f706 cf16 cb0b e54a  ...............J
-00000370: b950 2857 9ed3 777c faba 49a7 b48b ff3a  .P(W..w|..I....:
-00000380: 85ba a657 29a4 53ed 7bae e7ce cf2b 3ad0  ...W).S.{....+:.
-00000390: 358a f43a 75c1 0e74 5d6f 2aed 5344 c7ba  5..:u..t]o*.SD..
-000003a0: 0942 9742 451d 0aa8 2daa afa0 da87 e496  .B.BE...-.......
-000003b0: 6209 1c23 307a 9638 2706 8dd5 1db0 3ad4  b..#0z.8'.....:.
-000003c0: 86ed 406f 403f 4420 9131 d607 69dd e850  ..@o@?D .1..i..P
-000003d0: 784b c415 6deb 8618 6a53 a4ae 2bda d5be  xK..m...jS..+...
-000003e0: 7887 6c59 c1b5 0f66 7782 d349 e145 1287  x.lY...fw..I.E..
-000003f0: e7d2 07d8 ecd3 995e 3311 e780 522b 8d93  .......^3...R+..
-00000400: dee5 61d2 7e1e 65b1 a4e8 0bac fa34 80b9  ..a.~.e......4..
-00000410: 9aae 7bee 557c e910 021d 46a1 378d 0375  ..{.U|....F.7..u
-00000420: 670c c772 2c77 0073 0371 7a46 0108 9335  g..r,w.s.qzF...5
-00000430: 15bd 676c 3b10 e488 053f c75c 2ce4 63c2  ..gl;....?.\,.c.
-00000440: 9dab bb8a 702e d15d 4f9c 15e7 29ee a9ee  ....p..]O...)...
-00000450: 5a7a b0a0 92c3 7877 79ee 2cbd b5e5 6871  Zz....xwy.,...hq
-00000460: b64c ce00 d5d0 8e10 598f 514b d7ed 3191  .L......Y.QK..1.
-00000470: a304 b07d c9f5 bac4 1e4a 35ba e046 f46d  ...}.....J5..F.m
-00000480: 54ca d8c6 0e9e 4354 0177 7c5a 22ff 55b2  T.....CT.w|Z".U.
-00000490: 9848 b29b 1310 036e e359 c949 0fa9 f3a5  .H.....n.Y.I....
-000004a0: 814d a9e9 84bb efff 08fc 6323 5043 9a03  .M........c#PC..
-000004b0: 060c 7e5f a44e 691b b83a ba39 c716 05f0  ..~_.Ni..:.9....
-000004c0: 4bdc b9a3 b822 9734 562c 154a 0c88 0102  K....".4V,.J....
-000004d0: 474f bf1e 9594 c97b a212 4239 0db7 6b73  GO.....{..B9..ks
-000004e0: 90ee 8eba ca27 c0c8 a5ac a44a 495d dbb9  .....'.....JI]..
-000004f0: 494b 23fa 807a 4a3c 718d 7d0a fea6 173f  IK#..zJ<q.}....?
-00000500: c709 974e ccc8 282e 66da 6bec 2adf 6e99  ...N..(.f.k.*.n.
-00000510: e890 e924 b849 2d94 c9c9 e2f2 74fc f9c9  ...$.I-.....t...
-00000520: 85bd 209e fb10 849a 6e9a f118 e886 d4c9  .. .....n.......
-00000530: c62a da59 510b bfc5 8ff0 0c71 4e40 e6b1  .*.YQ......qN@..
-00000540: 1db7 0f67 654b c9ce b1dc 09ae 2e59 819c  ...geK.......Y..
-00000550: cfe6 b95e 2f3c ec39 bc32 f049 b8c5 b4d3  ...^/<.9.2.I....
-00000560: e9f5 494b 4f29 d56c 8a99 5ad5 9699 d9de  ..IKO).l..Z.....
-00000570: 2d4c 4143 5e0b c7b2 b9c3 18ca 1abf 0610  -LAC^...........
-00000580: 2c07 be9b 7792 95e2 7230 e206 17a5 883d  ,...w...r0.....=
-00000590: 52e3 a4eb ad92 9d40 4b98 b4f6 7873 1de1  R......@K...xs..
-000005a0: e10c 9636 38e3 f486 414b e35e 5323 dd65  ...68...AK.^S#.e
-000005b0: bbcf a4fa e769 dc56 53bc d127 a0c0 1219  .....i.VS..'....
-000005c0: 5f1c 31d1 2ece f44a c926 e402 591e 31e3  _.1....J.&..Y.1.
-000005d0: 17b8 e7fe 010d 0a30 3030 3030 3036 3020  .......00000060 
-000005e0: 3030 3030 3030 3630 2037 6666 6666 6666  00000060 7ffffff
-000005f0: 6620 0d0a 108c ebe6 4544 0200 108c ebe6  f ......ED......
-00000600: 4544 0200 0000 0000 3600 3200 3100 3700  ED......6.2.1.7.
-00000610: 3600 6200 6200 3800 2d00 3600 3800 6300  6.b.b.8.-.6.8.c.
-00000620: 6600 2d00 3400 3700 6600 3300 2d00 3800  f.-.4.7.f.3.-.8.
-00000630: 6300 3900 3000 2d00 3500 6500 3500 3900  c.9.0.-.5.e.5.9.
-00000640: 3200 3800 3900 6500 6400 3600 3200 6400  2.8.9.e.d.6.2.d.
-00000650: 0000 0000 0d0a 3030 3030 3030 6135 2030  ......000000a5 0
-00000660: 3030 3030 3230 3020 3766 6666 6666 6666  0000200 7fffffff
-00000670: 200d 0a95 4f3b 0ac3 300c dd0b b984 bb5a   ...O;..0......Z
-00000680: 60f9 27fb 143d 8364 3bd0 a543 a043 293e  `.'..=.d;..C.C)>
-00000690: 5987 1ea9 57a8 9350 c85a 10e2 3df1 f49e  Y...W..P.Z..=...
-000006a0: f479 bd9f a8a7 d3de cc86 ec81 1b1d 2d52  .y............-R
-000006b0: 1449 1053 99c1 d3ec 2095 6c20 b490 6dca  .I.S.... .l ..m.
-000006c0: ad46 5bbb 5697 a55e 6fbc 3cd4 beac 96bb  .F[.V..^o.<.....
-000006d0: 3a0c 8740 0d2f d4ce 3693 8805 d067 049f  :..@./..6....g..
-000006e0: 2502 0b13 7817 08c5 2317 2bda 75bd 260f  %...x...#.+.u.&.
-000006f0: a3ed 1475 561a c9a4 b932 4391 d2c0 8f60  ...uV....2C....`
-00000700: 1047 0e0c 7160 f2d2 5a46 8dfd 2fb9 edd3  .G..q`..ZF../...
-00000710: 69ad edd3 1f36 fd0b 0000 0000 0000 0000  i....6..........
+000002b0: 0000 0d0a 3030 3030 3033 3037 2030 3030  ....00000307 000
+000002c0: 3030 3330 3720 3766 6666 6666 6666 200d  00307 7fffffff .
+000002d0: 0aed 55bd 6ed3 5014 36dd b0e4 77b8 4a97  ..U.n.P.6...w.J.
+000002e0: 4484 36a5 4311 850d 8901 8967 6080 482c  D.6.C......g`.H,
+000002f0: b030 2021 449c 9496 2a15 552b 1055 a5b6  .0 !D...*.U+.U..
+00000300: a4e2 6742 7253 4cd2 8638 af70 ee3b b033  ..gBrSL..8.p.;.3
+00000310: 3187 ef9c ebeb 3876 aa54 6504 2771 aecf  1.....8v.Te.'q..
+00000320: ff77 fe3c 1c0e 5f3a 338e 73c9 3197 e756  .w.<.._:3.s.1..V
+00000330: e45a b8ae 92c3 52d5 5cca 73ef 4064 15bf  .Z....R.\.s.@d..
+00000340: 21d4 3e41 ede7 8c39 5bb5 6b15 951c 526a  !.>A...9[.k...Rj
+00000350: c1ef bbf7 efdd 9e71 ec3f 5f8f 9cc7 4ed5  .......q.?_...N.
+00000360: 7932 e6b5 5255 b1f6 98fa afde e0f9 6279  y2..RU........by
+00000370: a15c 2917 0ae5 ca0b fa81 4f5f 37e9 8476  .\).......O_7..v
+00000380: f05f a750 d7f4 0a85 74a2 7dcf f5dc f979  ._.P....t.}....y
+00000390: 4507 ba46 915e a32e d881 aeeb 0da5 7d8a  E..F.^........}.
+000003a0: e848 3741 e852 a8a8 4301 b545 f535 54fb  .H7A.R..C..E.5T.
+000003b0: 90dc 542c 8163 0446 cf12 e7c4 a0b1 ba0d  ..T,.c.F........
+000003c0: 5687 dab0 1de8 75e8 8708 2432 c6fa 20ad  V.....u...$2.. .
+000003d0: 191d 0a6f 88b8 a22d dd10 436d 8ad4 5545  ...o...-..Cm..UE
+000003e0: 3bda 17ef 902d 2bb8 f6c1 ec4e 703a 29bc  ;....-+....Np:).
+000003f0: 48e2 f05c fa08 9b7d 3ad5 ab26 e21c 506a  H..\...}:..&..Pj
+00000400: a571 d2fb 3c4c dacf a32c 9614 7d85 559f  .q..<L...,..}.U.
+00000410: 0630 57d3 75cf bd8c 2f7d 8040 8751 e80d  .0W.u.../}.@.Q..
+00000420: e340 dd1a c3b1 1ccb 1dc0 dc40 9c9e 5200  .@.........@..R.
+00000430: c264 4d45 7b8c 6d1b 821c b1e0 e798 8b85  .dME{.m.........
+00000440: 7c4c b873 7557 10ce 05ba eba9 f3d0 7986  |L.suW........y.
+00000450: 7baa bb96 1e2c a8e4 30de 5d9e 3b4b ef6c  {....,..0.].;K.l
+00000460: 395a 9c2d 9333 4035 b443 44d6 63d4 d275  9Z.-.3@5.CD.c..u
+00000470: bb4c e428 016c 5f72 bd26 b187 528d 2eb8  .L.(.l_r.&..R...
+00000480: 117d 1f95 32b6 b18d e710 55c0 1d9f 96c8  .}..2.....U.....
+00000490: 7f93 2c26 92ec e618 c480 db78 5672 d243  ..,&.......xVr.C
+000004a0: ea7c 6960 536a 3ae6 eefb 3f02 ffd8 08d4  .|i`Sj:...?.....
+000004b0: 90e6 8001 83df 17a9 13da 02ae 8e6e ceb1  .............n..
+000004c0: 4501 fc0a 77ee 28ae c805 8d15 4b85 1203  E...w.(.....K...
+000004d0: 6280 c0d1 d36f 4625 65f2 aea8 8450 4ec3  b....oF%e....PN.
+000004e0: edda 1ca4 bba3 aef2 0930 7229 2ba9 5252  .........0r)+.RR
+000004f0: d776 6ed2 d288 3ea0 9e12 4f5c 639f 82bf  .vn...>...O\c...
+00000500: e9c5 2f71 c2a5 1333 328a 8b99 f61a bbca  ../q...32.......
+00000510: b75b 263a 643a 096e 520b 6572 b2b8 3c1d  .[&:d:.nR.er..<.
+00000520: 7f7e 7261 2f88 e73e 04a1 a69b 663c 06ba  .~ra/..>....f<..
+00000530: 2175 b2b1 8a76 56d4 c26f f123 3c43 9c13  !u...vV..o.#<C..
+00000540: 9079 6cc7 edc3 59d9 54b2 732c 7782 ab0b  .yl...Y.T.s,w...
+00000550: 5620 e7b3 79a6 d773 0f7b 0eaf 0c7c 126e  V ..y..s.{...|.n
+00000560: 31ed 747a 7dd2 d253 4a35 9b62 a656 b565  1.tz}..SJ5.b.V.e
+00000570: 66b6 770b 53d0 90d7 c291 6cee 3086 b2ca  f.w.S.....l.0...
+00000580: af01 04cb 81ef e49d 64a5 b81c 8cb8 c145  ........d......E
+00000590: 2962 8fd4 38e9 7ab3 6427 d012 26ad 3dde  )b..8.z.d'..&.=.
+000005a0: 5c87 7838 85a5 75ce 38bd 65d0 d2b8 57d4  \.x8..u.8.e...W.
+000005b0: 4877 d9ee 33a9 fe59 1a37 d514 6ff4 1928  Hw..3..Y.7..o..(
+000005c0: b044 c617 474c b48b 33bd 52b2 0939 4796  .D..GL..3.R..9G.
+000005d0: 47cc f805 eeb9 7f00 0d0a 3030 3030 3030  G.........000000
+000005e0: 3630 2030 3030 3030 3036 3020 3766 6666  60 00000060 7fff
+000005f0: 6666 6666 200d 0ab0 f54b 604e 4402 00b0  ffff ....K`ND...
+00000600: f54b 604e 4402 0000 0000 0036 0032 0031  .K`ND......6.2.1
+00000610: 0037 0036 0062 0062 0038 002d 0036 0038  .7.6.b.b.8.-.6.8
+00000620: 0063 0066 002d 0034 0037 0066 0033 002d  .c.f.-.4.7.f.3.-
+00000630: 0038 0063 0039 0030 002d 0035 0065 0035  .8.c.9.0.-.5.e.5
+00000640: 0039 0032 0038 0039 0065 0064 0036 0032  .9.2.8.9.e.d.6.2
+00000650: 0064 0000 0000 000d 0a30 3030 3030 3061  .d.......000000a
+00000660: 3520 3030 3030 3032 3030 2037 6666 6666  5 00000200 7ffff
+00000670: 6666 6620 0d0a 954f 3b0a c330 0cdd 0bb9  fff ...O;..0....
+00000680: 84bb 5a60 f927 fb14 3d83 643b d0a5 43a0  ..Z`.'..=.d;..C.
+00000690: 4329 3e59 871e a957 a893 50c8 5a10 e23d  C)>Y...W..P.Z..=
+000006a0: f1f4 9ef4 79bd 9fa8 a7d3 decc 86ec 811b  ....y...........
+000006b0: 1d2d 5214 4910 5399 c1d3 ec20 956c 20b4  .-R.I.S.... .l .
+000006c0: 906d caad 465b bb56 97a5 5e6f bc3c d4be  .m..F[.V..^o.<..
+000006d0: ac96 bb3a 0c87 400d 2fd4 ce36 9388 05d0  ...:..@./..6....
+000006e0: 6704 9f25 020b 1378 1708 c523 172b da75  g..%...x...#.+.u
+000006f0: bd26 0fa3 ed14 7556 1ac9 a4b9 3243 91d2  .&....uV....2C..
+00000700: c08f 6010 470e 0c71 60f2 d25a 468d fd2f  ..`.G..q`..ZF../
+00000710: b9ed d369 aded d31f 36fd 0b00 0000 0000  ...i....6.......
 00000720: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000730: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000740: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000750: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000760: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000770: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000780: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -129,141 +129,141 @@
 00000800: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000810: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000820: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000830: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000840: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000850: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000860: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000870: 0000 000d 0a30 3030 3030 3036 3420 3030  .....00000064 00
-00000880: 3030 3030 3634 2037 6666 6666 6666 6620  000064 7fffffff 
-00000890: 0d0a 108c ebe6 4544 0200 108c ebe6 4544  ......ED......ED
-000008a0: 0200 0000 0000 3600 3200 3100 3700 3600  ......6.2.1.7.6.
-000008b0: 6200 6200 3800 2d00 3600 3800 6300 6600  b.b.8.-.6.8.c.f.
-000008c0: 2d00 3400 3700 6600 3300 2d00 3800 6300  -.4.7.f.3.-.8.c.
-000008d0: 3900 3000 2d00 3500 6500 3500 3900 3200  9.0.-.5.e.5.9.2.
-000008e0: 3800 3900 6500 6400 3600 3200 6400 2e00  8.9.e.d.6.2.d...
-000008f0: 3000 0000 0000 0d0a 3030 3030 3036 3035  0.......00000605
-00000900: 2030 3030 3030 3630 3520 3766 6666 6666   00000605 7fffff
-00000910: 6666 200d 0aed 584b 8f1b 4510 b672 8b25  ff ...XK..E..r.%
-00000920: ff87 d1e4 b28b a643 bfe6 4584 38f0 0790  .......C..E.8...
-00000930: 1017 6ee3 99f1 8904 1425 a7c8 621f 6813  ..n......%..b.h.
-00000940: 9188 9522 5050 1059 1645 9c9d cd3a 31f1  ..."PP.Y.E...:1.
-00000950: 3efe 420f 7f84 9fb0 5457 f78c db8f d821  >.B.....TW.....!
-00000960: 9b04 2418 7b77 ba6b aaab beaa feaa 7a76  ..$.{w.k......zv
-00000970: cfce cebe 6e5d 68e9 2f5e 9d36 c58b 251e  ....n]h./^.6..%.
-00000980: de39 a55e dc33 97d7 69bf 0f7a 772e b65a  .9.^.3..i..zw..Z
-00000990: 67b0 ec1a 8c9f 5c30 e3d6 ffd7 7fe2 aae9  g.....\0........
-000009a0: c1a9 d70c 1c7a 0c3e bff9 d11f 1f5f 68d5  .....z.>....._h.
-000009b0: 777d f55a 5fb6 aeb7 ae4e 2f97 5e33 58b1  w}.Z_....N/.^3X.
-000009c0: fc2a 2c2f 5a37 5b5f b44a d744 d4b5 04d5  .*,/Z7[_.J.D....
-000009d0: 03c7 c49f e3d3 4efb 927a a49e a8b1 1a54  ......N..z.....T
-000009e0: 9bd5 5675 cfd3 d36a 430d 4078 0282 db6a  ..Vu...jC.@x...j
-000009f0: a45e c0cf be3a 01f9 dd6a 0bc6 bfab c7f0  .^...:...j......
-00000a00: 6c43 1d55 773b ed4e 5bed c1f8 a4da 5143  lC.Uw;.N[.....QC
-00000a10: 7558 6deb b51e 8a46 ea11 a8bf a836 ecb2  uXm....F.....6..
-00000a20: d1da 7aa7 7d11 beea 876a 133c 8e3c f5b3  ..z.}....j.<.<..
-00000a30: 1a6a dd6d ed1b 10ec aa7d 7009 c6c0 e560  .j.m.....}p....`
-00000a40: 4ded 8148 2339 5243 143f 80f1 a956 d68f  M..H#9RC.?...V..
-00000a50: d73d f52b 283e 5587 6a00 362f 4ee3 8695  .=.+(>U.j.6/N...
-00000a60: 10cc ac85 eaee b48d 552e ae68 b00f c1cb  ........U..h....
-00000a70: 313c dea9 615f b151 ecc1 8343 d01b 57df  1<..a_.Q...C..W.
-00000a80: e934 a1c3 45c9 7ba4 9ec1 1d60 8299 51b5  .4..E.{....`..Q.
-00000a90: bbe6 9b84 a903 30ba a1fd a8fb 00ec 1424  ......0........$
-00000aa0: 63ed 087e 8e61 f526 e64c efcd 31ea 8ef1  c..~.a.&.L..1...
-00000ab0: 09ac f703 4ffd a88e e1b1 5e7e 00cb c7a0  ....O.....^~....
-00000ac0: 768a 7bb0 0931 adaf 1b80 0ef0 990d 32db  v.{..1........2.
-00000ad0: 76c9 5170 28a0 46e6 e10c 2bf6 21cc 6d08  v.Qp(.F...+.!.m.
-00000ae0: 64a8 0101 dce1 bc51 40f5 1874 8e61 cb77  d......Q@..t.a.w
-00000af0: f476 2fe3 c66b 47ff 520e 6937 b80b 76eb  .v/..kG.R.i7..v.
-00000b00: 5dc2 0e71 5fd1 6375 a7b6 b4d8 fa2c abee  ]..q_.cu.....,..
-00000b10: c3ec b93a d0c8 abad e57c 7855 56c3 030d  ...:.....|xUV...
-00000b20: f0e1 0c63 752a 8ee6 593d 29a1 597a 817c  ...cu*..Y=).Yz.|
-00000b30: 7b6d 0547 ddb8 0d43 7f69 d8b9 0d39 1a21  {m.G...C.i...9.!
-00000b40: c6a1 2ee5 35f5 1358 7956 dd7b 45fe 2cda  ....5..XyV.{E.,.
-00000b50: dad7 aac1 07e0 6550 ddf6 dc34 ad63 812d  ......eP...4.c.-
-00000b60: cb94 f7e1 a25d 5fe9 ccf5 71e5 3583 5cb5  .....]_...q.5.\.
-00000b70: 2536 f7df 43c9 ec7a e061 0075 7388 bb7a  %6..C..z.a.us..z
-00000b80: e241 eb1c 4003 1deb 1a7e aea9 0233 e4a8  .A..@....~...3..
-00000b90: 95eb 7d58 1a77 e0f9 ef5d 2ebf ea61 1bb0  ..}X.w...]...a..
-00000ba0: 7572 8ced f037 ec36 63a4 8d6d d000 17d2  ur...7.6c..m....
-00000bb0: 741f 23bc a329 0e71 ccda 1c5d c64e 06e5  t.#..).q...].N..
-00000bc0: dd74 b1ba bd6f afd5 b0ac 0ed6 cb10 a01f  .t...o..........
-00000bd0: 55bb 4813 c7d3 e5e9 c4cc 31d3 c253 8337  U.H.......1..S.7
-00000be0: d09e f034 2b62 7bb0 eac1 f4b1 768b c741  ...4+b{.....v..A
-00000bf0: a77d 8b25 fab7 1e04 4c8f fceb 37fd c047  .}.%....L...7..G
-00000c00: 4a34 383d a6f6 3ddd 7fb0 70a0 704f e6db  J48=..=...p.pO..
-00000c10: 8207 c001 4bf5 0d84 f0d4 d0c0 b438 bfdf  ....K........8..
-00000c20: 69f7 8330 903c 9569 14f3 34ec 6b3f 34cd  i..0.<.i..4.k?4.
-00000c30: f322 8f63 5266 2c23 328b 0a92 7559 4e84  .".cRf,#2...uYN.
-00000c40: 1461 9915 1997 4220 be1a 5e64 f089 40e2  .a....B ..^d..@.
-00000c50: 72b4 ba60 1e07 22a0 a0ca 28ed c300 35d0  r..`.."...(...5.
-00000c60: 10e1 fc65 6be6 e766 453c 2be0 6c22 a166  ...ek..fE<+.l".f
-00000c70: 09dc f547 2682 f19c a684 8771 8fc8 2e4f  ...G&......q...O
-00000c80: 4997 2794 f044 1645 9296 bd9c 957d 138f  I.'..D.E.....}..
-00000c90: 5d03 00f5 bd1f f0c8 dac0 f828 a44a 180d  ]..........(.J..
-00000ca0: 9825 4628 1b6f be1f 10a6 bf60 0726 fd73  .%F(.o.....`.&.s
-00000cb0: 3db5 100c 2216 4c48 209d b125 8469 0ae6  =...".LH ..%.i..
-00000cc0: 7cde 5103 e6d7 9948 8cfd b708 911b 8828  |.Q....H.......(
-00000cd0: 658b a0ac 6686 f906 c62e 8a79 9004 cc0a  e...f......y....
-00000ce0: 6c0e ac54 a782 cf48 4598 a2ae 4069 d2c8  l..T...HE...@i..
-00000cf0: a186 b4ba 9c88 a943 74d8 ca48 d624 74c0  .......Ct..H.$t.
-00000d00: 69e5 306e cc37 8839 ce7a 795c 725a 901e  i.0n.7.9.zy\rZ..
-00000d10: 978c c888 e6a4 5bf4 2409 b322 49ca 50c6  ......[.$.."I.P.
-00000d20: 320b 8d31 f106 4a63 5521 fc93 85c1 5c4a  2..1..JcU!....\J
-00000d30: 5a1a ce75 7b0f 8e0d 3c43 9ebb 87d8 07be  Z..u{...<C......
-00000d40: 4d74 bdbd 5859 96e9 b533 f66e e86b fdca  Mt..XY...3.n.k..
-00000d50: 9a52 0eb1 e8a4 88f4 8709 a619 65fb 0012  .R..........e...
-00000d60: 026c 450d dbec c4ae b11a da2e 4b97 69bc  .lE.........K.i.
-00000d70: 8a0d 1e30 2ece 67e4 651a 361c 19b0 a6cd  ...0..g.e.6.....
-00000d80: e899 e83b e960 4d4a 9884 5dd6 47fe 211c  ...;.`MJ..].G.!.
-00000d90: 38fa d56b eef5 0146 f8da 30fd dae2 bb75  8..k...F..0....u
-00000da0: b720 c322 6165 1171 4952 ce62 22cb 4890  . ."ae.qIR.b".H.
-00000db0: 242c ba24 97b9 c8bb 495c 6459 09f5 0a9a  $,.$....I\dY....
-00000dc0: 29d2 ed93 ecc6 8df2 fa35 1f27 9f36 ddee  )........5.'.6..
-00000dd0: 5f59 7188 85b0 a4ef 043e 554e 3811 4eaa  _Yq......>UN8.N.
-00000de0: a712 5f4b 2c8f fdcf 0cad f10e 8c76 979c  .._K,........v..
-00000df0: a716 660b d105 e900 8ae2 38e6 2c0c 9af8  ..f.......8.,...
-00000e00: 30ba 348b 2329 0a4e 585a a644 8625 2749  0.4.#).NXZ.D.%'I
-00000e10: 920a 6823 b49b a72c 0db3 346e 4eae a908  ..h#...,..4nN...
-00000e20: a889 a13e 069a e6c4 9c4e 406d 1132 1141  ...>.....N@m.2.A
-00000e30: 19ea 66ff b7cb 307c 0365 4861 6f49 f256  ..f...0|.eHaoI.V
-00000e40: ab30 3455 e812 804f d7de b9ab cde6 5944  .04U...O......YD
-00000e50: c0fe d012 4cc2 27a4 b52c 8dea 5a02 30a2  ....L.'..,..Z.0.
-00000e60: 39f9 ccdc 805a 8443 4bbe 85f7 cd17 d596  9....Z.CK.......
-00000e70: 3f5f a397 fca0 80b3 26e3 5149 581e 7589  ?_......&.QIX.u.
-00000e80: 649c 93b4 2c04 e975 7bb1 48ba 51c6 4cd5  d...,..u{.H.Q.L.
-00000e90: 4c6a 99f7 2d40 7ff9 5f14 0bfc 999e 30b1  Lj..-@.._.....0.
-00000ea0: 8609 0e9b 119f 3cb5 0a61 5a44 39e7 3149  ......<..aZD9.1I
-00000eb0: 63c0 24a3 5e44 1299 5112 2632 0f33 2072  c.$.^D..Q.&2.3 r
-00000ec0: 5cda b38e 3775 52d3 75ba 1862 fd0f d5a0  \...7uR.u..b....
-00000ed0: 6451 caf3 9c93 8886 106d 2842 a2cf 547d  dQ.......m(B..T}
-00000ee0: b24a ca45 12cb 2837 fdc1 5ffc bf26 df18  .J.E..(7.._..&..
-00000ef0: 5cfe d43d 7c51 cfb3 7fc4 4d14 27d8 de96  \..=|Q....M.'...
-00000f00: f2f2 9e43 9df2 6e5e f4e4 d4d1 df9f fc7e  ...C..n^.......~
-00000f10: 6707 7efd 1609 0ffb 7f01 0d0a 3030 3030  g.~.........0000
-00000f20: 3030 3630 2030 3030 3030 3036 3020 3766  0060 00000060 7f
-00000f30: 6666 6666 6666 200d 0a10 8ceb e645 4402  ffffff ......ED.
-00000f40: 0010 8ceb e645 4402 0000 0000 0036 0034  .....ED......6.4
-00000f50: 0030 0063 0061 0063 0032 0033 002d 0035  .0.c.a.c.2.3.-.5
-00000f60: 0062 0038 0036 002d 0034 0039 0037 0065  .b.8.6.-.4.9.7.e
-00000f70: 002d 0038 0066 0030 0063 002d 0065 0038  .-.8.f.0.c.-.e.8
-00000f80: 0032 0038 0062 0062 0065 0033 0065 0061  .2.8.b.b.e.3.e.a
-00000f90: 0061 0033 0000 0000 000d 0a30 3030 3030  .a.3.......00000
-00000fa0: 3061 3120 3030 3030 3032 3030 2037 6666  0a1 00000200 7ff
-00000fb0: 6666 6666 6620 0d0a 958f 3b0e c230 0c86  fffff ....;..0..
-00000fc0: 77a4 5e22 acb1 6427 699d 1c82 43d8 a9cb  w.^"..d'i...C...
-00000fd0: c680 c484 7232 068e c415 485b 2158 912c  ....r2....H[!X.,
-00000fe0: ebf7 ebb3 fd7a 3cef e487 c3ee 7053 e127  .....z<.....pS.'
-00000ff0: 463f 25ac 5243 8451 f304 a9b0 415e b082  F?%.RC.Q....A^..
-00001000: e590 552d 9a48 6cde 9de4 2267 9bdd 3eeb  ..U-.Hl..."g..>.
-00001010: ae37 f7cd f5b2 eb24 f231 1866 1605 4a85  .7.....$.1.f..J.
-00001020: 3a4b 2710 1586 1447 264d d4f7 a8ef b4b5  :K'....G&M......
-00001030: b773 b643 dcd1 7962 cccb 2c02 55ab 410a  .s.C..yb..,.U.A.
-00001040: b980 468e 802c a370 52b3 429e da5f eda1  ..F..,.pR.B.._..
-00001050: 0d87 d5b6 3f3f 1adb 1b00 0000 0000 0000  ....??..........
+00000870: 0000 0000 0000 0d0a 3030 3030 3030 3634  ........00000064
+00000880: 2030 3030 3030 3036 3420 3766 6666 6666   00000064 7fffff
+00000890: 6666 200d 0ab0 f54b 604e 4402 00b0 f54b  ff ....K`ND....K
+000008a0: 604e 4402 0000 0000 0036 0032 0031 0037  `ND......6.2.1.7
+000008b0: 0036 0062 0062 0038 002d 0036 0038 0063  .6.b.b.8.-.6.8.c
+000008c0: 0066 002d 0034 0037 0066 0033 002d 0038  .f.-.4.7.f.3.-.8
+000008d0: 0063 0039 0030 002d 0035 0065 0035 0039  .c.9.0.-.5.e.5.9
+000008e0: 0032 0038 0039 0065 0064 0036 0032 0064  .2.8.9.e.d.6.2.d
+000008f0: 002e 0030 0000 0000 000d 0a30 3030 3030  ...0.......00000
+00000900: 3630 3520 3030 3030 3036 3035 2037 6666  605 00000605 7ff
+00000910: 6666 6666 6620 0d0a ed58 4b8f 1b45 10b6  fffff ...XK..E..
+00000920: 728b 25ff 87d1 e4b2 8ba6 43bf e645 8438  r.%.......C..E.8
+00000930: f007 9010 176e e399 f189 0414 25a7 c862  .....n......%..b
+00000940: 1f68 1391 8895 2250 5010 5916 459c 9dcd  .h...."PP.Y.E...
+00000950: 3a31 f13e fe42 0f7f 849f b054 57f7 8cdb  :1.>.B.....TW...
+00000960: 8fd8 219b 0424 187b 77ba 6baa abbe aafe  ..!..$.{w.k.....
+00000970: aa7a 76cf cece be6e 5d68 e92f 5e9d 36c5  .zv....n]h./^.6.
+00000980: 8b25 1ede 39a5 5edc 3397 d769 bf0f 7a77  .%..9.^.3..i..zw
+00000990: 2eb6 5a67 b0ec 1a8c 9f5c 30e3 d6ff d77f  ..Zg.....\0.....
+000009a0: e2aa e9c1 a9d7 0c1c 7a0c 3ebf f9d1 1f1f  ........z.>.....
+000009b0: 5f68 d577 7df5 5a5f b6ae b7ae 4e2f 975e  _h.w}.Z_....N/.^
+000009c0: 3358 b1fc 2a2c 2f5a 375b 5fb4 4ad7 44d4  3X..*,/Z7[_.J.D.
+000009d0: b504 d503 c7c4 9fe3 d34e fb92 7aa4 9ea8  .........N..z...
+000009e0: b11a 549b d556 75cf d3d3 6a43 0d40 7802  ..T..Vu...jC.@x.
+000009f0: 82db 6aa4 5ec0 cfbe 3a01 f9dd 6a0b c6bf  ..j.^...:...j...
+00000a00: abc7 f06c 431d 5577 3bed 4e5b edc1 f8a4  ...lC.Uw;.N[....
+00000a10: da51 4375 586d ebb5 1e8a 46ea 11a8 bfa8  .QCuXm....F.....
+00000a20: 36ec b2d1 da7a a77d 11be ea87 6a13 3c8e  6....z.}....j.<.
+00000a30: 3cf5 b31a 6add 6ded 1b10 ecaa 7d70 09c6  <...j.m.....}p..
+00000a40: c0e5 604d ed81 4823 3952 4314 3f80 f1a9  ..`M..H#9RC.?...
+00000a50: 56d6 8fd7 3df5 2b28 3e55 876a 0036 2f4e  V...=.+(>U.j.6/N
+00000a60: e386 9510 ccac 85ea eeb4 8d55 2eae 68b0  ...........U..h.
+00000a70: 0fc1 cb31 3cde a961 5fb1 51ec c183 43d0  ...1<..a_.Q...C.
+00000a80: 1b57 dfe9 34a1 c345 c97b a49e c11d 6082  .W..4..E.{....`.
+00000a90: 9951 b5bb e69b 84a9 0330 baa1 fda8 fb00  .Q.......0......
+00000aa0: ec14 2463 ed08 7e8e 61f5 26e6 4cef cd31  ..$c..~.a.&.L..1
+00000ab0: ea8e f109 acf7 034f fda8 8ee1 b15e 7e00  .......O.....^~.
+00000ac0: cbc7 a076 8a7b b009 31ad af1b 800e f099  ...v.{..1.......
+00000ad0: 0d32 db76 c951 7028 a046 e6e1 0c2b f621  .2.v.Qp(.F...+.!
+00000ae0: cc6d 0864 a801 01dc e1bc 5140 f518 748e  .m.d......Q@..t.
+00000af0: 61cb 77f4 762f e3c6 6b47 ff52 0e69 37b8  a.w.v/..kG.R.i7.
+00000b00: 0b76 eb5d c20e 715f d163 75a7 b6b4 d8fa  .v.]..q_.cu.....
+00000b10: 2cab eec3 ecb9 3ad0 c8ab ade5 7c78 5556  ,.....:.....|xUV
+00000b20: c303 0df0 e10c 6375 2a8e e659 3d29 a159  ......cu*..Y=).Y
+00000b30: 7a81 7c7b 6d05 47dd b80d 437f 69d8 b90d  z.|{m.G...C.i...
+00000b40: 391a 21c6 a12e e535 f513 5879 56dd 7b45  9.!....5..XyV.{E
+00000b50: fe2c dada d7aa c107 e065 50dd f6dc 34ad  .,.......eP...4.
+00000b60: 6381 2dcb 94f7 e1a2 5d5f e9cc f571 e535  c.-.....]_...q.5
+00000b70: 835c b525 36f7 df43 c9ec 7ae0 6100 7573  .\.%6..C..z.a.us
+00000b80: 88bb 7ae2 41eb 1c40 031d eb1a 7eae a902  ..z.A..@....~...
+00000b90: 33e4 a895 eb7d 581a 77e0 f9ef 5d2e bfea  3....}X.w...]...
+00000ba0: 611b b075 728c edf0 37ec 3663 a48d 6dd0  a..ur...7.6c..m.
+00000bb0: 0017 d274 1f23 bca3 290e 71cc da1c 5dc6  ...t.#..).q...].
+00000bc0: 4e06 e5dd 74b1 babd 6faf d5b0 ac0e d6cb  N...t...o.......
+00000bd0: 10a0 1f55 bb48 13c7 d3e5 e9c4 cc31 d3c2  ...U.H.......1..
+00000be0: 5383 37d0 9ef0 342b 627b b0ea c1f4 b176  S.7...4+b{.....v
+00000bf0: 8bc7 41a7 7d8b 25fa b71e 044c 8ffc eb37  ..A.}.%....L...7
+00000c00: fdc0 474a 3438 3da6 f63d dd7f b070 a070  ..GJ48=..=...p.p
+00000c10: 4fe6 db82 07c0 014b f50d 84f0 d4d0 c0b4  O......K........
+00000c20: 38bf df69 f783 3090 3c95 6914 f334 ec6b  8..i..0.<.i..4.k
+00000c30: 3f34 cdf3 228f 6352 662c 2332 8b0a 9275  ?4..".cRf,#2...u
+00000c40: 594e 8414 6199 1519 9742 20be 1a5e 64f0  YN..a....B ..^d.
+00000c50: 8940 e272 b4ba 601e 0722 a0a0 ca28 edc3  .@.r..`.."...(..
+00000c60: 0035 d010 e1fc 656b e6e7 6645 3c2b e06c  .5....ek..fE<+.l
+00000c70: 22a1 6609 dcf5 4726 82f1 9ca6 8487 718f  ".f...G&......q.
+00000c80: c82e 4f49 9727 94f0 4416 4592 96bd 9c95  ..OI.'..D.E.....
+00000c90: 7d13 8f5d 0300 f5bd 1ff0 c8da c0f8 28a4  }..]..........(.
+00000ca0: 4a18 0d98 2546 281b 6fbe 1f10 a6bf 6007  J...%F(.o.....`.
+00000cb0: 26fd 733d b510 0c22 164c 4820 9db1 2584  &.s=...".LH ..%.
+00000cc0: 690a e67c de51 03e6 d799 488c fdb7 0891  i..|.Q....H.....
+00000cd0: 1b88 2865 8ba0 ac66 86f9 06c6 2e8a 7990  ..(e...f......y.
+00000ce0: 04cc 0a6c 0eac 54a7 82cf 4845 98a2 ae40  ...l..T...HE...@
+00000cf0: 69d2 c8a1 86b4 ba9c 88a9 4374 d8ca 48d6  i.........Ct..H.
+00000d00: 2474 c069 e530 6ecc 3788 39ce 7a79 5c72  $t.i.0n.7.9.zy\r
+00000d10: 5a90 1e97 8cc8 88e6 a45b f424 09b3 2249  Z........[.$.."I
+00000d20: ca50 c632 0b8d 31f1 064a 6355 21fc 9385  .P.2..1..JcU!...
+00000d30: c15c 4a5a 1ace 757b 0f8e 0d3c 439e bb87  .\JZ..u{...<C...
+00000d40: d807 be4d 74bd bd58 5996 e9b5 33f6 6ee8  ...Mt..XY...3.n.
+00000d50: 6bfd ca9a 520e b1e8 a488 f487 09a6 1965  k...R..........e
+00000d60: fb00 1202 6c45 0ddb ecc4 aeb1 1ada 2e4b  ....lE.........K
+00000d70: 9769 bc8a 0d1e 302e ce67 e465 1a36 1c19  .i....0..g.e.6..
+00000d80: b0a6 cde8 99e8 3be9 604d 4a98 845d d647  ......;.`MJ..].G
+00000d90: fe21 1c38 fad5 6bee f501 46f8 da30 fdda  .!.8..k...F..0..
+00000da0: e2bb 75b7 20c3 2261 6511 7149 52ce 6222  ..u. ."ae.qIR.b"
+00000db0: cb48 9024 2cba 2497 b9c8 bb49 5c64 5909  .H.$,.$....I\dY.
+00000dc0: f50a 9a29 d2ed 93ec c68d f2fa 351f 279f  ...)........5.'.
+00000dd0: 36dd ee5f 5971 8885 b0a4 ef04 3e55 4e38  6.._Yq......>UN8
+00000de0: 114e aaa7 125f 4b2c 8ffd cf0c adf1 0e8c  .N..._K,........
+00000df0: 7697 9ca7 1666 0bd1 05e9 008a e238 e62c  v....f.......8.,
+00000e00: 0c9a f830 ba34 8b23 290a 4e58 5aa6 4486  ...0.4.#).NXZ.D.
+00000e10: 2527 4992 0a68 23b4 9ba7 2c0d b334 6e4e  %'I..h#...,..4nN
+00000e20: aea9 08a8 89a1 3e06 9ae6 c49c 4e40 6d11  ......>.....N@m.
+00000e30: 3211 4119 ea66 ffb7 cb30 7c03 6548 616f  2.A..f...0|.eHao
+00000e40: 49f2 56ab 3034 55e8 1280 4fd7 deb9 abcd  I.V.04U...O.....
+00000e50: e659 44c0 fed0 124c c227 a4b5 2c8d ea5a  .YD....L.'..,..Z
+00000e60: 0230 a239 f9cc dc80 5a84 434b be85 f7cd  .0.9....Z.CK....
+00000e70: 17d5 963f 5fa3 97fc a080 b326 e351 4958  ...?_......&.QIX
+00000e80: 1e75 8964 9c93 b42c 04e9 757b b148 ba51  .u.d...,..u{.H.Q
+00000e90: c64c d54c 6a99 f72d 407f f95f 140b fc99  .L.Lj..-@.._....
+00000ea0: 9e30 b186 090e 9b11 9f3c b50a 615a 4439  .0.......<..aZD9
+00000eb0: e731 4963 c024 a35e 4412 9951 1226 320f  .1Ic.$.^D..Q.&2.
+00000ec0: 3320 725c dab3 8e37 7552 d375 ba18 62fd  3 r\...7uR.u..b.
+00000ed0: 0fd5 a064 51ca f39c 9388 8610 6d28 42a2  ...dQ.......m(B.
+00000ee0: cf54 7db2 4aca 4512 cb28 37fd c15f fcbf  .T}.J.E..(7.._..
+00000ef0: 26df 185c fed4 3d7c 51cf b37f c44d 1427  &..\..=|Q....M.'
+00000f00: d8de 96f2 f29e 439d f26e 5ef4 e4d4 d1df  ......C..n^.....
+00000f10: 9ffc 7e67 077e fd16 090f fb7f 010d 0a30  ..~g.~.........0
+00000f20: 3030 3030 3036 3020 3030 3030 3030 3630  0000060 00000060
+00000f30: 2037 6666 6666 6666 6620 0d0a b0f5 4b60   7fffffff ....K`
+00000f40: 4e44 0200 b0f5 4b60 4e44 0200 0000 0000  ND....K`ND......
+00000f50: 3600 3400 3000 6300 6100 6300 3200 3300  6.4.0.c.a.c.2.3.
+00000f60: 2d00 3500 6200 3800 3600 2d00 3400 3900  -.5.b.8.6.-.4.9.
+00000f70: 3700 6500 2d00 3800 6600 3000 6300 2d00  7.e.-.8.f.0.c.-.
+00000f80: 6500 3800 3200 3800 6200 6200 6500 3300  e.8.2.8.b.b.e.3.
+00000f90: 6500 6100 6100 3300 0000 0000 0d0a 3030  e.a.a.3.......00
+00000fa0: 3030 3030 6131 2030 3030 3030 3230 3020  0000a1 00000200 
+00000fb0: 3766 6666 6666 6666 200d 0a95 8f3b 0ec2  7fffffff ....;..
+00000fc0: 300c 8677 a45e 22ac b164 2769 9d1c 8243  0..w.^"..d'i...C
+00000fd0: d8a9 cbc6 80c4 8472 3206 8ec4 1548 5b21  .......r2....H[!
+00000fe0: 5891 2ceb f7eb b3fd 7a3c efe4 87c3 ee70  X.,.....z<.....p
+00000ff0: 53e1 2746 3f25 ac52 4384 51f3 04a9 b041  S.'F?%.RC.Q....A
+00001000: 5eb0 82e5 9055 2d9a 486c de9d e422 679b  ^....U-.Hl..."g.
+00001010: dd3e ebae 37f7 cdf5 b2eb 24f2 3118 6616  .>..7.....$.1.f.
+00001020: 054a 853a 4b27 1015 8614 4726 4dd4 f7a8  .J.:K'....G&M...
+00001030: efb4 b5b7 73b6 43dc d179 62cc cb2c 0255  ....s.C..yb..,.U
+00001040: ab41 0ab9 8046 8e80 2ca3 7052 b342 9eda  .A...F..,.pR.B..
+00001050: 5fed a10d 87d5 b63f 3f1a db1b 0000 0000  _......??.......
 00001060: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001070: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001080: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001090: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000010a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000010b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000010c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -277,206 +277,206 @@
 00001140: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001150: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001160: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001170: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001180: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001190: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000011a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000011b0: 0000 0000 0000 0000 0d0a 3030 3030 3030  ..........000000
-000011c0: 3634 2030 3030 3030 3036 3420 3766 6666  64 00000064 7fff
-000011d0: 6666 6666 200d 0a10 8ceb e645 4402 0010  ffff ......ED...
-000011e0: 8ceb e645 4402 0000 0000 0036 0034 0030  ...ED......6.4.0
-000011f0: 0063 0061 0063 0032 0033 002d 0035 0062  .c.a.c.2.3.-.5.b
-00001200: 0038 0036 002d 0034 0039 0037 0065 002d  .8.6.-.4.9.7.e.-
-00001210: 0038 0066 0030 0063 002d 0065 0038 0032  .8.f.0.c.-.e.8.2
-00001220: 0038 0062 0062 0065 0033 0065 0061 0061  .8.b.b.e.3.e.a.a
-00001230: 0033 002e 0030 0000 0000 000d 0a30 3030  .3...0.......000
-00001240: 3030 3735 3220 3030 3030 3037 3532 2037  00752 00000752 7
-00001250: 6666 6666 6666 6620 0d0a bd58 6d6f 1347  fffffff ...Xmo.G
-00001260: 10fe 4c24 ff07 eba2 5649 e54b eff6 ee6c  ..L$....VI.K...l
-00001270: 5f23 3e90 024e 9013 90f3 e238 df7c 7776  _#>..N.....8.|wv
-00001280: 5e70 4204 8989 8d22 1122 012a 88b4 a815  ^pB....".".*....
-00001290: 88b6 402a 54f5 a3a1 3131 9884 bfb0 f74b  ..@*T...11.....K
-000012a0: fa17 3a3b bb67 9f9d 8bed 84b4 71ee d6b7  ..:;.g......q...
-000012b0: 3b3b 3bf3 cc33 b3b7 fea7 fef9 8e16 09f5  ;;;..3..........
-000012c0: ddd1 cd88 223e 2a6f c59f 1c70 f3fe 4014  ....">*o...p..@.
-000012d0: a682 fca6 98a8 e264 7661 bf66 db76 d450  .......dva.f.v.P
-000012e0: 7272 3eaa a9b2 6e67 7372 3ca7 69b2 96cb  rr>...ngsr<.i...
-000012f0: 66ed a8aa 5846 de8c 48f4 957b 97d6 e84b  f...XF..H..{...K
-00001300: f71e fde8 de75 1f41 5ba3 3509 d5f4 a401  .....u.A[.5.....
-00001310: 56dc 640b 8219 6810 21ec 2ec3 7ca2 102d  V.d...h.!...|..-
-00001320: aac5 e458 3c1a 97f5 ac91 97e3 462c 2ac7  ...X<.......F,*.
-00001330: 3523 1b8b e614 dbb4 b29b c26b 66c8 1b7a  5#.........kf..z
-00001340: 08a6 7ca2 15fa 821e 627b 40f7 e0aa b83b  ..|.....b{@....;
-00001350: f415 3e55 69dd 7d2c 35bc 6e7a 2f40 8b90  ..>Ui.},5.nz/@..
-00001360: 082e ae45 746e 51a8 0fa5 6211 8d03 a4f0  ...EtnQ...b.....
-00001370: 5928 2ccc 15df 9b3a 3426 cc06 63b1 7cde  Y(,....:4&..c.|.
-00001380: b689 29c7 f2c4 9175 4234 d922 242f ab66  ..)....uB4."$/.f
-00001390: 341a cdc5 88a1 5859 5c4d 1796 9cc0 5f02  4.....XY\M...._.
-000013a0: febe a46f c1df 0a7d 0b7e 03f8 f0ed 67f0  ...o...}.~....g.
-000013b0: 6f87 3e83 6f9f dd6d 778b f549 cd78 fa3c  o.>.o..mw..I.x.<
-000013c0: c696 61ed 7988 06ab a056 e108 b448 735e  ..a.y....V...Hs^
-000013d0: 6878 a9d8 32ca f106 8625 2902 d192 b994  hx..2....%).....
-000013e0: 246d 761f ed86 6ffb 78b7 e74e f1d1 4444  $mv...o.x..N..DD
-000013f0: 05cb 5984 55bc b77e 4046 9ae6 d661 0b66  ..Y.U..~@F...a.f
-00001400: 7773 93ab d37a cb35 d061 288a 1e69 18b8  ws...z.5.a(..i..
-00001410: 1900 34f1 8225 5dcb aead e56e ae48 0d92  ..4..%]....n.H..
-00001420: 7972 5f04 8d2a a0e0 6034 5755 f052 fdf5  yr_..*..`4WU.R..
-00001430: c3ff d9f4 99e0 4b51 7222 c6c6 7b65 2c66  ......KQr"..{e,f
-00001440: ef01 8c57 a1a0 6c41 7b00 cf55 fa1b 5c07  ...W..lA{..U..\.
-00001450: ee93 33ce 5e95 159f 80dc 6d8d 41eb 1310  ..3.^.....m.A...
-00001460: 4192 0429 3862 4c91 87ed 0920 517a 86e4  A..)8bL.... Qz..
-00001470: 3514 b12d f721 ad81 2cc0 d028 6a87 744f  5..-.!..,..(j.tO
-00001480: 48ec f364 3f9a baa7 04c6 1078 2827 a59f  H..d?......x('..
-00001490: d240 86ad adc7 3595 d88a 2913 2396 9775  .@....5...).#..u
-000014a0: 0baa a145 e28a 4ce2 bae3 c4cd 5cde 5673  ...E..L.....\.Vs
-000014b0: 3857 c1ac f4ea 120f ac07 af77 17d1 110d  8W.........w....
-000014c0: 0f03 1bc1 a6f9 c171 3e49 5144 f152 4436  .......q>IQD.RD6
-000014d0: c376 83cb 49a1 be7e 863d ad23 b2f7 dcc7  .v..I..~.=.#....
-000014e0: e1d6 50b8 0f60 1bfb 08d7 2e80 fc56 6c6b  ..P..`.......Vlk
-000014f0: 1fbc 3dc6 7d14 ea0b f57d 4d7f 47ba d661  ..=.}....}M.G..a
-00001500: a8ca 291b eac3 fdf0 d0bd 0f3d 7b10 3f50  ..)........={.?P
-00001510: 180e de22 0778 078b dd60 a8ef 1cfc d35f  ...".x...`....._
-00001520: 2098 a02c 0c7a ab6c d636 f29f 857a 172c   ..,.z.l.6...z.,
-00001530: 02b5 4c7c 806d 6668 e827 5ac5 ee16 ae0c  ..L|.mfh.'Z.....
-00001540: 86e9 1f20 f837 6c7d 15d0 79ae 8d61 15e6  ... .7l}..y..a..
-00001550: 6bbb 06f7 51ab 8e6e 4b0c 3363 314d 61f8  k...Q..nK.3c1Ma.
-00001560: be67 f6b0 f002 6909 7275 f709 4311 170c  .g....i.ru..C...
-00001570: c2f6 257d 0fed 1eee cc35 7767 40e2 ef12  ..%}.....5wg@...
-00001580: 87f4 1d68 bd8b c83c 05cb 3e43 4f1d 376f  ...h...<..>CO.7o
-00001590: c6fb 4384 a486 b13b 40d9 3a8e 8002 a041  ..C....;@.:....A
-000015a0: 983e e771 80f9 ef60 7e1d e43e 633c b6c0  .>.q...`~..>c<..
-000015b0: abc1 416e a2cf f4b6 60f1 b8f6 fb04 7c1c  ..An....`.....|.
-000015c0: a135 3ed8 469b 5d70 741b 5ca9 328b c0de  .5>.F.]pt.\.2...
-000015d0: ea51 a560 d51b 9039 80f0 df67 a13f 3179  .Q.`...9...g.?1y
-000015e0: 4e8d c9c0 71d4 62cb 6070 0423 fc34 af62  N...q.b.`p.#.4.b
-000015f0: b871 45a8 3942 53b0 f676 b23d 85a7 7dfa  .qE.9BS..v.=..}.
-00001600: 8e59 eede eb4c 935e c90e 03cc c017 01a5  .Y...L.^........
-00001610: f2d3 51b2 3773 ac9d 75d0 bf3d d085 ba7e  ..Q.7s..u..=...~
-00001620: bf39 715f 3748 bb0d 18d5 d0c6 2a2b 0003  .9q_7H......*+..
-00001630: f457 d0f2 de7d dc23 a978 bc77 0535 d99d  .W...}.#.x.w.5..
-00001640: c5db 470b 77e7 0ce3 c29c 6989 4518 3c81  ..G.w.....i.E.<.
-00001650: 0d15 a46a d0c9 f437 4a19 083e c31d e501  ...j...7J..>....
-00001660: 9f4f ab2c 1519 763f e01e 7c4f 9206 87ce  .O.,..v?..|O....
-00001670: ceb4 e116 ac8e c98b 2e38 75cc f2b3 f7bd  .........8u.....
-00001680: e372 3df9 d343 9e9f aa4e 0be3 c35d 0a36  .r=..C...N...].6
-00001690: 96e5 4e89 143e 1f44 be2f df26 fea3 ace8  ..N..>.D./.&....
-000016a0: 1d17 5f2d f95f 92a2 ab65 7e83 ce8c 3add  .._-._...e~...:.
-000016b0: aa9e 286f f86a 1906 8d15 d8af f6b0 701e  ..(o.j........p.
-000016c0: 86c1 e70a bcd9 d459 56ed 8771 c90f 98d3  .......YV..q....
-000016d0: a29f 95ba 8edc 8984 25e9 9ba1 dc6a 9e6f  ........%....j.o
-000016e0: c062 333a c057 913f 71a7 afb3 da8c f5f9  .b3:.W.?q.......
-000016f0: 4730 1a62 ec6e 01e1 24f8 1b6e 8cbc c233  G0.b.n..$..n...3
-00001700: 7b95 cfc6 c5c4 fa03 cd49 9186 b143 285f  {........I...C(_
-00001710: 1767 83e7 10b1 9d48 1886 fd35 f91c ef47  .g.....H...5...G
-00001720: 6a07 bc92 3c45 d81f b243 85fb 2400 b4e6  j...<E...C..$...
-00001730: b283 4d2b 5b91 f6d8 b2ed 85f5 2fd4 5067  ..M+[......./.Pg
-00001740: 2165 7469 2eb1 c3ab 612b 7443 5fa9 43cd  !eti....a+tC_.C.
-00001750: 5f2d 7c5f c59b 0c18 3fd8 58db 4714 012a  _-|_....?.X.G..*
-00001760: ad9c 7ae7 a13f c1b5 7fe4 a455 09c8 bdd3  ..z..?.....U....
-00001770: 20d7 c8be 2684 01b9 d750 83f4 6e47 a736   ...&....P..nG.6
-00001780: 14b4 765b 543a 654f 87b7 3889 9fec f1bc  ..v[T:eO..8.....
-00001790: 61e2 7963 b371 18f3 d2db 7f94 6a1c fef0  a.yc.q......j...
-000017a0: a15f 8a38 70ac c992 684e 56ed a825 eb2a  ._.8p...hNV..%.*
-000017b0: 21b2 9973 3439 6fe5 635a dc8a 6655 a236  !..s49o.cZ..fU.6
-000017c0: 7e5a 69dc a411 098f 9bbd 8cf8 7e27 f09d  ~Zi.........~'..
-000017d0: 5ffc fd42 d4e4 bfe3 a0fd 1dd3 5478 c4cf  _..B........Tx..
-000017e0: b637 d7a5 a67c 987e 0ce3 5ede 3ec3 5ba3  .7...|.~..^.>.[.
-000017f0: d5ff 49e9 cc5c 538e 774d 74f7 5bd9 5bb9  ..I..\S.wMt.[.[.
-00001800: a8fe 5d2c b6fe edb5 8ba6 6ea5 6fcf 3bcb  ..],......n.o.;.
-00001810: 3325 9b14 8ad6 92b2 383e a9df 1e5b 1c29  3%......8>...[.)
-00001820: 58cb 13c5 b944 617d aeac 2cce cca4 12c9  X....Da}..,.....
-00001830: a9f9 c56b 657d e2fb a58d a9b9 d994 120a  ...ke}..........
-00001840: f565 d3c6 8a5d 1a01 151b eb36 8865 4753  .e...].....6.eGS
-00001850: 8a7d f146 31a9 65f4 e4d2 e5a5 e4ca 1535  .}.F1.e........5
-00001860: 599e 5f1f 9f34 af67 6653 0bc9 f444 d19a  Y._..4.gfS...D..
-00001870: 1d29 c252 4a36 6dae 838a e4ec 8461 6ba9  .).RJ6m......ak.
-00001880: 8235 6996 9956 ae72 6c3e 9750 6f59 2be3  .5i..V.rl>.PoY+.
-00001890: d1b9 c444 3943 ccd2 b5c9 2b37 9cd1 d4ed  ...D9C....+7....
-000018a0: ab8b f1a2 b304 2ad3 e3eb f6ca 7411 545c  ......*.....t.T\
-000018b0: fd5e df48 92d4 8293 b8b4 06a2 6b76 c22c  .^.H........kv.,
-000018c0: 6767 53ab 16d1 d76c ad50 7612 336b 4932  ggS....l.Pv.3kI2
-000018d0: 51b4 97a7 17c7 4617 d6ac 8451 beba 32a1  Q.....F....Q..2.
-000018e0: e4d2 1b05 a616 5404 69f6 a92d 3ae9 eb45  ......T.i..-:..E
-000018f0: b0d2 b012 2d2a 0ccf 6950 d1d1 6f6d 6635  ....-*..iP..omf5
-00001900: 49e6 8ad6 4aaa 9cd4 3c87 9b4e c2b2 26a8  I...J...<..N..&.
-00001910: 185b 5e50 9cd1 0bd1 64c9 246c f54c c928  .[^P....d.$l.L.(
-00001920: 3993 7150 7909 2271 59c9 4c9a 4b96 76a5  9.qPy."qY.L.K.v.
-00001930: 00d1 1190 af92 aba3 33ab 1e36 0c8b ce4e  ........3..6...N
-00001940: f88c 770a 99a5 a311 6311 0934 1e02 9730  ..w.....c..4...0
-00001950: 4b76 c9d4 e6d2 637e 35ab 569b 1aa6 e258  Kv....c~5.V....X
-00001960: 0c9a 6a20 d0d7 2dcd 29fb 9cd1 8fc0 e968  ..j ..-.)......h
-00001970: 4ec9 d0c6 4b06 04cf 2e8e 2f5d b80d ea32  N...K...../]...2
-00001980: 53d3 1b53 19b2 50b0 d297 7c96 2c94 b353  S..S..P...|.,..S
-00001990: 4d4b 9815 dda7 af81 15c0 8fcb eb19 32bd  MK............2.
-000019a0: 982c ebe7 0373 2a20 c736 ff05 0d0a 3030  .,...s* .6....00
-000019b0: 3030 3030 3630 2030 3030 3030 3036 3020  000060 00000060 
-000019c0: 3766 6666 6666 6666 200d 0a10 8ceb e645  7fffffff ......E
-000019d0: 4402 0010 8ceb e645 4402 0000 0000 0062  D......ED......b
-000019e0: 0039 0030 0064 0038 0035 0038 0036 002d  .9.0.d.8.5.8.6.-
-000019f0: 0061 0031 0032 0065 002d 0034 0035 0066  .a.1.2.e.-.4.5.f
-00001a00: 0036 002d 0061 0031 0038 0032 002d 0034  .6.-.a.1.8.2.-.4
-00001a10: 0065 0035 0061 0030 0038 0037 0062 0031  .e.5.a.0.8.7.b.1
-00001a20: 0064 0032 0038 0000 0000 000d 0a30 3030  .d.2.8.......000
-00001a30: 3030 3161 6420 3030 3030 3032 3030 2037  001ad 00000200 7
-00001a40: 6666 6666 6666 6620 0d0a 8d52 496a 5c31  fffffff ...RIj\1
-00001a50: 10dd 1b7c 87e6 af55 509a 4aa5 65c8 1972  ...|...UP.J.e..r
-00001a60: 000d a555 20c1 7156 a6c1 19c8 2681 2cb3  ...U .qV....&.,.
-00001a70: ce0d 9c84 4063 63fb 0afa 27c9 1552 bf1b  ....@cc...'..R..
-00001a80: bc36 08f1 241e f506 e9df dde3 9535 e767  .6..$........5.g
-00001a90: 5735 63e7 c804 c53a 8110 c786 d841 9058  W5c....:.....A.X
-00001aa0: 9053 b5dd f1de 1ca9 cdb3 b7d2 183a f708  .S...........:..
-00001ab0: 6164 0f5c 9c83 91eb 2882 c9bb 3436 de91  ad.\....(...46..
-00001ac0: 1c4c 5776 7124 601b 5508 5699 59ba 8751  .LWvq$`.U.V.Y..Q
-00001ad0: 47f2 5c49 05ad 61c1 1152 8850 521b 107c  G.\I..a..R.PR..|
-00001ae0: f590 6b65 a896 c947 c2e8 84b6 71f8 3418  ..ke...G....q.4.
-00001af0: 0d9a 680b 06ec 016a 6175 c294 8193 b380  ..h....jau......
-00001b00: 218d 18aa 60ef 696f 9697 afdf bc93 17e3  !...`.io........
-00001b10: 522e 5ebd ede5 5296 d390 e5e2 fd62 96f9  R.^...R......b..
-00001b20: 63de ccdb f57a fdba 7e5c bfed ecfc b99b  c....z..~\......
-00001b30: 8ff3 61fd 30ef e6df dd7c 98bf e6bd eebf  ..a.0....|......
-00001b40: b7a3 a2c3 fa7d 376f f5e2 7efd 3c0f f3cf  .....}7o..~.<...
-00001b50: fa69 bd9e 37eb 17c5 8745 b516 b585 fbf3  .i..7....E......
-00001b60: b3bd 2167 136d 1988 b748 6968 4d2d 2344  ..!g.m...HihM-#D
-00001b70: 89d9 b156 40ae 6f7c 0ad8 4a73 1e62 d5fa  ...V@.o|..Js.b..
-00001b80: 434e 023c b081 b0e3 5ac5 4b29 7e6f c2e6  CN.<....Z.K)~o..
-00001b90: d9d5 2603 bb06 cc6c c1da 4e50 b32a 2046  ..&....l..NP.* F
-00001ba0: ac5a 7dc9 b1ab fa46 f5bd 4841 4b40 b926  .Z}....F..HAK@.&
-00001bb0: 7d45 2d29 87e8 c1ba 94ad f5c9 0d2d f444  }E-).........-.D
-00001bc0: edb1 a244 e9e0 2275 0868 1be4 e609 0679  ...D.."u.h.....y
-00001bd0: 7536 3a17 72c6 3dcb e7b3 421f 4545 3f43  u6:.r.=...B.EE?C
-00001be0: d55b a8a9 3084 9e14 49cb 4091 2da6 4239  .[..0...I.@.-.B9
-00001bf0: b771 2af2 b4fe 0300 0000 0000 0000 0000  .q*.............
+000011b0: 0000 0000 0000 0000 0000 000d 0a30 3030  .............000
+000011c0: 3030 3036 3420 3030 3030 3030 3634 2037  00064 00000064 7
+000011d0: 6666 6666 6666 6620 0d0a b0f5 4b60 4e44  fffffff ....K`ND
+000011e0: 0200 b0f5 4b60 4e44 0200 0000 0000 3600  ....K`ND......6.
+000011f0: 3400 3000 6300 6100 6300 3200 3300 2d00  4.0.c.a.c.2.3.-.
+00001200: 3500 6200 3800 3600 2d00 3400 3900 3700  5.b.8.6.-.4.9.7.
+00001210: 6500 2d00 3800 6600 3000 6300 2d00 6500  e.-.8.f.0.c.-.e.
+00001220: 3800 3200 3800 6200 6200 6500 3300 6500  8.2.8.b.b.e.3.e.
+00001230: 6100 6100 3300 2e00 3000 0000 0000 0d0a  a.a.3...0.......
+00001240: 3030 3030 3037 3532 2030 3030 3030 3735  00000752 0000075
+00001250: 3220 3766 6666 6666 6666 200d 0abd 586d  2 7fffffff ...Xm
+00001260: 6f13 4710 fe4c 24ff 07eb a256 49e5 4bef  o.G..L$....VI.K.
+00001270: f6ee 6c5f 233e 9002 4e90 1390 f3e2 38df  ..l_#>..N.....8.
+00001280: 7c77 765e 7042 0489 898d 2211 2201 2a88  |wv^pB....".".*.
+00001290: b4a8 1588 b640 2a54 f5a3 a131 3198 84bf  .....@*T...11...
+000012a0: b0f7 4bfa 173a 3bbb 679f 9d8b ed84 b471  ..K..:;.g......q
+000012b0: eed6 b73b 3b3b f3cc 33b3 b7fe a7fe f98e  ...;;;..3.......
+000012c0: 1609 f5dd d1cd 8822 3e2a 6fc5 9f1c 70f3  .......">*o...p.
+000012d0: fe40 14a6 82fc a698 a8e2 6476 61bf 66db  .@........dva.f.
+000012e0: 76d4 5072 723e aaa9 b26e 6773 723c a769  v.Prr>...ngsr<.i
+000012f0: b296 cb66 eda8 aa58 46de 8c48 f495 7b97  ...f...XF..H..{.
+00001300: d6e8 4bf7 1efd e8de 751f 415b a335 09d5  ..K.....u.A[.5..
+00001310: f4a4 0156 dc64 0b82 1968 1021 ec2e c37c  ...V.d...h.!...|
+00001320: a210 2daa c5e4 583c 1a97 f5ac 9197 e346  ..-...X<.......F
+00001330: 2c2a c735 231b 8be6 14db b4b2 9bc2 6b66  ,*.5#.........kf
+00001340: c81b 7a08 a67c a215 fa82 1e62 7b40 f7e0  ..z..|.....b{@..
+00001350: aab8 3bf4 153e 5569 dd7d 2c35 bc6e 7a2f  ..;..>Ui.},5.nz/
+00001360: 408b 9008 2eae 4574 6e51 a80f a562 118d  @.....EtnQ...b..
+00001370: 03a4 f059 282c cc15 df9b 3a34 26cc 0663  ...Y(,....:4&..c
+00001380: b17c deb6 8929 c7f2 c491 7542 34d9 2224  .|...)....uB4."$
+00001390: 2fab 6634 1acd c588 a158 595c 4d17 969c  /.f4.....XY\M...
+000013a0: c05f 02fe bea4 6fc1 df0a 7d0b 7e03 f8f0  ._....o...}.~...
+000013b0: ed67 f06f 873e 836f 9fdd 6d77 8bf5 49cd  .g.o.>.o..mw..I.
+000013c0: 78fa 3cc6 9661 ed79 8806 aba0 56e1 08b4  x.<..a.y....V...
+000013d0: 4873 5e68 78a9 d832 caf1 0686 2529 02d1  Hs^hx..2....%)..
+000013e0: 92b9 9424 6d76 1fed 866f fb78 b7e7 4ef1  ...$mv...o.x..N.
+000013f0: d144 4405 cb59 8455 bcb7 7e40 469a e6d6  .DD..Y.U..~@F...
+00001400: 610b 6677 7393 abd3 7acb 35d0 6128 8a1e  a.fws...z.5.a(..
+00001410: 6918 b819 0034 f182 255d cbae ade5 6eae  i....4..%]....n.
+00001420: 480d 9279 725f 048d 2aa0 e060 3457 55f0  H..yr_..*..`4WU.
+00001430: 52fd f5c3 ffd9 f499 e04b 5172 22c6 c67b  R........KQr"..{
+00001440: 652c 66ef 018c 57a1 a06c 417b 00cf 55fa  e,f...W..lA{..U.
+00001450: 1b5c 07ee 9333 ce5e 9515 9f80 dc6d 8d41  .\...3.^.....m.A
+00001460: eb13 1041 9204 2938 624c 9187 ed09 2051  ...A..)8bL.... Q
+00001470: 7a86 e435 14b1 2df7 21ad 812c c0d0 286a  z..5..-.!..,..(j
+00001480: 8774 4f48 ecf3 643f 9aba a704 c610 7828  .tOH..d?......x(
+00001490: 27a5 9fd2 4086 adad c735 95d8 8a29 1323  '...@....5...).#
+000014a0: 9697 750b aaa1 45e2 8a4c e2ba e3c4 cd5c  ..u...E..L.....\
+000014b0: de56 7338 57c1 acf4 ea12 0fac 07af 7717  .Vs8W.........w.
+000014c0: d111 0d0f 031b c1a6 f9c1 713e 4951 44f1  ..........q>IQD.
+000014d0: 5244 36c3 7683 cb49 a1be 7e86 3dad 23b2  RD6.v..I..~.=.#.
+000014e0: f7dc c7e1 d650 b80f 601b fb08 d72e 80fc  .....P..`.......
+000014f0: 566c 6b1f bc3d c67d 14ea 0bf5 7d4d 7f47  Vlk..=.}....}M.G
+00001500: bad6 61a8 ca29 1bea c3fd f0d0 bd0f 3d7b  ..a..)........={
+00001510: 103f 5018 0ede 2207 7807 8bdd 60a8 ef1c  .?P...".x...`...
+00001520: fcd3 5f20 98a0 2c0c 7aab 6cd6 36f2 9f85  .._ ..,.z.l.6...
+00001530: 7a17 2c02 b54c 7c80 6d66 68e8 275a c5ee  z.,..L|.mfh.'Z..
+00001540: 16ae 0c86 e91f 20f8 376c 7d15 d079 ae8d  ...... .7l}..y..
+00001550: 6115 e66b bb06 f751 ab8e 6e4b 0c33 6331  a..k...Q..nK.3c1
+00001560: 4d61 f8be 67f6 b0f0 0269 0972 75f7 0943  Ma..g....i.ru..C
+00001570: 1117 0cc2 f625 7d0f ed1e eecc 3577 6740  .....%}.....5wg@
+00001580: e2ef 1287 f41d 68bd 8bc8 3c05 cb3e 434f  ......h...<..>CO
+00001590: 1d37 6fc6 fb43 84a4 86b1 3b40 d93a 8e80  .7o..C....;@.:..
+000015a0: 02a0 4198 3ee7 7180 f9ef 607e 1de4 3e63  ..A.>.q...`~..>c
+000015b0: 3cb6 c0ab c141 6ea2 cff4 b660 f1b8 f6fb  <....An....`....
+000015c0: 047c 1ca1 353e d846 9b5d 7074 1b5c a932  .|..5>.F.]pt.\.2
+000015d0: 8bc0 deea 51a5 60d5 1b90 3980 f0df 67a1  ....Q.`...9...g.
+000015e0: 3f31 794e 8dc9 c071 d462 cb60 7004 23fc  ?1yN...q.b.`p.#.
+000015f0: 34af 62b8 7145 a839 4253 b0f6 76b2 3d85  4.b.qE.9BS..v.=.
+00001600: a77d fa8e 59ee deeb 4c93 5ec9 0e03 ccc0  .}..Y...L.^.....
+00001610: 1701 a5f2 d351 b237 73ac 9d75 d0bf 3dd0  .....Q.7s..u..=.
+00001620: 85ba 7ebf 3971 5f37 48bb 0d18 d5d0 c62a  ..~.9q_7H......*
+00001630: 2b00 03f4 57d0 f2de 7ddc 23a9 78bc 7705  +...W...}.#.x.w.
+00001640: 35d9 9dc5 db47 0b77 e70c e3c2 9c69 8945  5....G.w.....i.E
+00001650: 183c 810d 15a4 6ad0 c9f4 374a 1908 3ec3  .<....j...7J..>.
+00001660: 1de5 019f 4fab 2c15 1976 3fe0 1e7c 4f92  ....O.,..v?..|O.
+00001670: 0687 cece b4e1 16ac 8ec9 8b2e 3875 ccf2  ............8u..
+00001680: b3f7 bde3 723d f9d3 439e 9faa 4e0b e3c3  ....r=..C...N...
+00001690: 5d0a 3696 e54e 8914 3e1f 44be 2fdf 26fe  ].6..N..>.D./.&.
+000016a0: a3ac e81d 175f 2df9 5f92 a2ab 657e 83ce  ....._-._...e~..
+000016b0: 8c3a ddaa 9e28 6ff8 6a19 068d 15d8 aff6  .:...(o.j.......
+000016c0: b070 1e86 c1e7 0abc d9d4 5956 ed87 71c9  .p........YV..q.
+000016d0: 0f98 d3a2 9f95 ba8e dc89 8425 e99b a1dc  ...........%....
+000016e0: 6a9e 6fc0 6233 3ac0 5791 3f71 a7af b3da  j.o.b3:.W.?q....
+000016f0: 8cf5 f947 301a 62ec 6e01 e124 f81b 6e8c  ...G0.b.n..$..n.
+00001700: bcc2 337b 95cf c6c5 c4fa 03cd 4991 86b1  ..3{........I...
+00001710: 4328 5f17 6783 e710 b19d 4818 86fd 35f9  C(_.g.....H...5.
+00001720: 1cef 476a 07bc 923c 45d8 1fb2 4385 fb24  ..Gj...<E...C..$
+00001730: 00b4 e6b2 834d 2b5b 91f6 d8b2 ed85 f52f  .....M+[......./
+00001740: d450 6721 6574 692e b1c3 ab61 2b74 435f  .Pg!eti....a+tC_
+00001750: a943 cd5f 2d7c 5fc5 9b0c 183f d858 db47  .C._-|_....?.X.G
+00001760: 1401 2aad 9c7a e7a1 3fc1 b57f e4a4 5509  ..*..z..?.....U.
+00001770: c8bd d320 d7c8 be26 8401 b9d7 5083 f46e  ... ...&....P..n
+00001780: 47a7 3614 b476 5b54 3a65 4f87 b738 899f  G.6..v[T:eO..8..
+00001790: ecf1 bc61 e279 63b3 7118 f3d2 db7f 946a  ...a.yc.q......j
+000017a0: 1cfe f0a1 5f8a 3870 acc9 9268 4e56 eda8  ...._.8p...hNV..
+000017b0: 25eb 2a21 b299 7334 396f e563 5adc 8a66  %.*!..s49o.cZ..f
+000017c0: 55a2 367e 5a69 dca4 1109 8f9b bd8c f87e  U.6~Zi.........~
+000017d0: 27f0 9d5f fcfd 42d4 e4bf e3a0 fd1d d354  '.._..B........T
+000017e0: 78c4 cfb6 37d7 a5a6 7c98 7e0c e35e de3e  x...7...|.~..^.>
+000017f0: c35b a3d5 ff49 e9cc 5c53 8e77 4d74 f75b  .[...I..\S.wMt.[
+00001800: d95b b9a8 fe5d 2cb6 feed b58b a66e a56f  .[...],......n.o
+00001810: cf3b cb33 259b 148a d692 b238 3ea9 df1e  .;.3%......8>...
+00001820: 5b1c 2958 cb13 c5b9 4461 7dae ac2c cecc  [.)X....Da}..,..
+00001830: a412 c9a9 f9c5 6b65 7de2 fba5 8da9 b9d9  ......ke}.......
+00001840: 9412 0af5 65d3 c68a 5d1a 0115 1beb 3688  ....e...].....6.
+00001850: 6547 538a 7df1 4631 a965 f4e4 d2e5 a5e4  eGS.}.F1.e......
+00001860: ca15 3559 9e5f 1f9f 34af 6766 530b c9f4  ..5Y._..4.gfS...
+00001870: 44d1 9a1d 29c2 524a 366d ae83 8ae4 ec84  D...).RJ6m......
+00001880: 616b a982 3569 9699 56ae 726c 3e97 506f  ak..5i..V.rl>.Po
+00001890: 592b e3d1 b9c4 4439 43cc d2b5 c92b 379c  Y+....D9C....+7.
+000018a0: d1d4 edab 8bf1 a2b3 042a d3e3 ebf6 ca74  .........*.....t
+000018b0: 1154 5cfd 5edf 4892 d482 93b8 b406 a26b  .T\.^.H........k
+000018c0: 76c2 2c67 6753 ab16 d1d7 6cad 5076 1233  v.,ggS....l.Pv.3
+000018d0: 6b49 3251 b497 a717 c746 17d6 ac84 51be  kI2Q.....F....Q.
+000018e0: ba32 a1e4 d21b 05a6 1654 0469 f6a9 2d3a  .2.......T.i..-:
+000018f0: e9eb 45b0 d2b0 122d 2a0c cf69 50d1 d16f  ..E....-*..iP..o
+00001900: 6d66 3549 e68a d64a aa9c d43c 879b 4ec2  mf5I...J...<..N.
+00001910: b226 a818 5b5e 509c d10b d164 c924 6cf5  .&..[^P....d.$l.
+00001920: 4cc9 2839 9371 5079 0922 7159 c94c 9a4b  L.(9.qPy."qY.L.K
+00001930: 9676 a500 d111 90af 92ab a333 ab1e 360c  .v.........3..6.
+00001940: 8bce 4ef8 8c77 0a99 a5a3 1163 1109 341e  ..N..w.....c..4.
+00001950: 0297 304b 76c9 d4e6 d263 7e35 ab56 9b1a  ..0Kv....c~5.V..
+00001960: a6e2 580c 9a6a 20d0 d72d cd29 fb9c d18f  ..X..j ..-.)....
+00001970: c0e9 684e c9d0 c64b 0604 cf2e 8e2f 5db8  ..hN...K...../].
+00001980: 0dea 3253 d31b 5319 b250 b0d2 977c 962c  ..2S..S..P...|.,
+00001990: 94b3 534d 4b98 15dd a7af 8115 c08f cbeb  ..SMK...........
+000019a0: 1932 bd98 2ceb e703 732a 20c7 36ff 050d  .2..,...s* .6...
+000019b0: 0a30 3030 3030 3036 3020 3030 3030 3030  .00000060 000000
+000019c0: 3630 2037 6666 6666 6666 6620 0d0a b0f5  60 7fffffff ....
+000019d0: 4b60 4e44 0200 b0f5 4b60 4e44 0200 0000  K`ND....K`ND....
+000019e0: 0000 6200 3900 3000 6400 3800 3500 3800  ..b.9.0.d.8.5.8.
+000019f0: 3600 2d00 6100 3100 3200 6500 2d00 3400  6.-.a.1.2.e.-.4.
+00001a00: 3500 6600 3600 2d00 6100 3100 3800 3200  5.f.6.-.a.1.8.2.
+00001a10: 2d00 3400 6500 3500 6100 3000 3800 3700  -.4.e.5.a.0.8.7.
+00001a20: 6200 3100 6400 3200 3800 0000 0000 0d0a  b.1.d.2.8.......
+00001a30: 3030 3030 3031 6164 2030 3030 3030 3230  000001ad 0000020
+00001a40: 3020 3766 6666 6666 6666 200d 0a8d 5249  0 7fffffff ...RI
+00001a50: 6a5c 3110 dd1b 7c87 e6af 5550 9a4a a565  j\1...|...UP.J.e
+00001a60: c819 7200 0da5 5520 c171 56a6 c119 c826  ..r...U .qV....&
+00001a70: 812c b3ce 0d9c 8440 6363 fb0a fa27 c915  .,.....@cc...'..
+00001a80: 52bf 1bbc 3608 f124 1ef5 06e9 dfdd e395  R...6..$........
+00001a90: 35e7 6757 3563 e7c8 04c5 3a81 10c7 86d8  5.gW5c....:.....
+00001aa0: 4190 5890 53b5 ddf1 de1c a9cd b3b7 d218  A.X.S...........
+00001ab0: 3af7 0861 640f 5c9c 8391 eb28 82c9 bb34  :..ad.\....(...4
+00001ac0: 36de 911c 4c57 7671 2460 1b55 0856 9959  6...LWvq$`.U.V.Y
+00001ad0: ba87 5147 f25c 4905 ad61 c111 5288 5052  ..QG.\I..a..R.PR
+00001ae0: 1b10 7cf5 906b 65a8 96c9 47c2 e884 b671  ..|..ke...G....q
+00001af0: f834 180d 9a68 0b06 ec01 6a61 75c2 9481  .4...h....jau...
+00001b00: 93b3 8021 8d18 aa60 ef69 6f96 97af dfbc  ...!...`.io.....
+00001b10: 9317 e352 2e5e bded e552 96d3 90e5 e2fd  ...R.^...R......
+00001b20: 6296 f963 decc dbf5 7afd ba7e 5cbf edec  b..c....z..~\...
+00001b30: fcb9 9b8f f361 fd30 efe6 dfdd 7c98 bfe6  .....a.0....|...
+00001b40: bdee bfb7 a3a2 c3fa 7d37 6ff5 e27e fd3c  ........}7o..~.<
+00001b50: 0ff3 cffa 69bd 9e37 eb17 c587 45b5 16b5  ....i..7....E...
+00001b60: 85fb f3b3 bd21 6713 6d19 88b7 4869 684d  .....!g.m...HihM
+00001b70: 2d23 4489 d9b1 5640 ae6f 7c0a d84a 731e  -#D...V@.o|..Js.
+00001b80: 62d5 fa43 4e02 3cb0 81b0 e35a c54b 297e  b..CN.<....Z.K)~
+00001b90: 6fc2 e6d9 d526 03bb 06cc 6cc1 da4e 50b3  o....&....l..NP.
+00001ba0: 2a20 46ac 5a7d c9b1 abfa 46f5 bd48 414b  * F.Z}....F..HAK
+00001bb0: 40b9 267d 452d 2987 e8c1 ba94 adf5 c90d  @.&}E-).........
+00001bc0: 2df4 44ed b1a2 44e9 e022 7508 681b e4e6  -.D...D.."u.h...
+00001bd0: 0906 7975 363a 1772 c63d cbe7 b342 1f45  ..yu6:.r.=...B.E
+00001be0: 453f 43d5 5ba8 a930 849e 1449 cb40 912d  E?C.[..0...I.@.-
+00001bf0: a642 39b7 712a f2b4 fe03 0000 0000 0000  .B9.q*..........
 00001c00: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001c10: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001c20: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001c30: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001c40: 0000 0000 0000 0000 0000 0d0a 3030 3030  ............0000
-00001c50: 3030 3238 2030 3030 3030 3032 3820 3766  0028 00000028 7f
-00001c60: 6666 6666 6666 200d 0a10 8ceb e645 4402  ffffff ......ED.
-00001c70: 0010 8ceb e645 4402 0000 0000 0063 006f  .....ED......c.o
-00001c80: 0070 0079 0069 006e 0066 006f 0000 0000  .p.y.i.n.f.o....
-00001c90: 000d 0a30 3030 3030 3066 3920 3030 3030  ...000000f9 0000
-00001ca0: 3032 3030 2037 6666 6666 6666 6620 0d0a  0200 7fffffff ..
-00001cb0: 9591 314e 8331 0c85 f74a bd44 e758 4a9c  ..1N.1...J.D.XJ.
-00001cc0: c471 46c4 8c98 3880 133b 0809 012a 5d50  .qF...8..;...*]P
-00001cd0: d593 3170 24ae 40fe b688 f567 b125 e7bd  ..1p$.@....g.%..
-00001ce0: a7cf cef7 e7d7 31b9 ede6 1897 9283 f8e4  ......1.........
-00001cf0: 3541 13ce 9098 2a70 c100 3e95 9153 33af  5A....*p..>..S3.
-00001d00: 5adc 2a51 58e2 7ae4 18ac 3328 eb54 8e1a  Z.*QX.z...3(.T..
-00001d10: 8105 1146 6d43 cc97 8865 b8dd edf3 ebbb  ...FmC...e......
-00001d20: dd8c 83ed 1fde 540e b63b 6d37 a7c5 4e18  ......T..;m7..N.
-00001d30: 0ab5 c640 dc07 ccf4 69ef d543 b65c 91ab  ...@....i..C.\..
-00001d40: 29a1 ba55 a233 8de6 e62d 9b02 6652 483e  )..U.3...-..fRH>
-00001d50: 74a8 3d12 0c8a becb 5016 42b7 bbdf ebd3  t.=.....P.B.....
-00001d60: 8bec 3ffe 28d2 7ced 1821 3726 48b5 18f0  ..?.(.|..!7&H...
-00001d70: f01d 8c91 5bb3 6822 d1ad 12fd 83e2 4e5e  ....[.h"......N^
-00001d80: e4d1 f40c 71e5 b8b8 e741 05c9 2074 6a90  ....q....A.. tj.
-00001d90: c23c e65c 31c2 68a3 446e 2401 c3ba 0ff2  .<.\1.h.Dn$.....
-00001da0: bfb9 fe52 ddb5 2fe3 1f00 0000 0000 0000  ...R../.........
+00001c40: 0000 0000 0000 0000 0000 0000 000d 0a30  ...............0
+00001c50: 3030 3030 3032 3820 3030 3030 3030 3238  0000028 00000028
+00001c60: 2037 6666 6666 6666 6620 0d0a b0f5 4b60   7fffffff ....K`
+00001c70: 4e44 0200 b0f5 4b60 4e44 0200 0000 0000  ND....K`ND......
+00001c80: 6300 6f00 7000 7900 6900 6e00 6600 6f00  c.o.p.y.i.n.f.o.
+00001c90: 0000 0000 0d0a 3030 3030 3030 6639 2030  ......000000f9 0
+00001ca0: 3030 3030 3230 3020 3766 6666 6666 6666  0000200 7fffffff
+00001cb0: 200d 0a95 9131 4e83 310c 85f7 4abd 44e7   ....1N.1...J.D.
+00001cc0: 584a 9cc4 7146 c48c 9838 8013 3b08 0901  XJ..qF...8..;...
+00001cd0: 2a5d 50d5 9331 7024 ae40 feb6 88f5 67b1  *]P..1p$.@....g.
+00001ce0: 25e7 bda7 cfce f7e7 d731 b9ed e618 9792  %........1......
+00001cf0: 83f8 e435 4113 ce90 982a 70c1 003e 9591  ...5A....*p..>..
+00001d00: 5333 af5a dc2a 5158 e27a e418 ac33 28eb  S3.Z.*QX.z...3(.
+00001d10: 548e 1a81 0511 466d 43cc 9788 65b8 dded  T.....FmC...e...
+00001d20: f3eb bbdd 8c83 ed1f de54 0eb6 3b6d 37a7  .........T..;m7.
+00001d30: c54e 180a b5c6 40dc 07cc f469 efd5 43b6  .N....@....i..C.
+00001d40: 5c91 ab29 a1ba 55a2 338d e6e6 2d9b 0266  \..)..U.3...-..f
+00001d50: 5248 3e74 a83d 120c 8abe cb50 1642 b7bb  RH>t.=.....P.B..
+00001d60: dfeb d38b ec3f fe28 d27c ed18 2137 2648  .....?.(.|..!7&H
+00001d70: b518 f0f0 1d8c 915b b368 22d1 ad12 fd83  .......[.h".....
+00001d80: e24e 5ee4 d1f4 0c71 e5b8 b8e7 4105 c920  .N^....q....A.. 
+00001d90: 746a 90c2 3ce6 5c31 c268 a344 6e24 01c3  tj..<.\1.h.Dn$..
+00001da0: ba0f f2bf b9fe 52dd b52f e31f 0000 0000  ......R../......
 00001db0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001dc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001dd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001de0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001df0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001e00: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001e10: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -485,23 +485,23 @@
 00001e40: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001e50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001e60: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001e70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001e80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001e90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001ea0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001eb0: 0d0a 3030 3030 3030 3230 2030 3030 3030  ..00000020 00000
-00001ec0: 3032 3020 3766 6666 6666 6666 200d 0a10  020 7fffffff ...
-00001ed0: 8ceb e645 4402 0010 8ceb e645 4402 0000  ...ED......ED...
-00001ee0: 0000 0072 006f 006f 0074 0000 0000 000d  ...r.o.o.t......
-00001ef0: 0a30 3030 3030 3032 6320 3030 3030 3032  .0000002c 000002
-00001f00: 3030 2037 6666 6666 6666 6620 0d0a 7bbf  00 7fffffff ..{.
-00001f10: 7b7f b591 4e92 a541 8a85 a985 996e a2a1  {...N..A.....n..
-00001f20: 51aa ae89 691a 8865 61a4 6b92 6a9a 6860  Q...i..ea.k.j.h`
-00001f30: 619e 6498 6264 a153 0b00 0000 0000 0000  a.d.bd.S........
+00001eb0: 0000 000d 0a30 3030 3030 3032 3020 3030  .....00000020 00
+00001ec0: 3030 3030 3230 2037 6666 6666 6666 6620  000020 7fffffff 
+00001ed0: 0d0a b0f5 4b60 4e44 0200 b0f5 4b60 4e44  ....K`ND....K`ND
+00001ee0: 0200 0000 0000 7200 6f00 6f00 7400 0000  ......r.o.o.t...
+00001ef0: 0000 0d0a 3030 3030 3030 3263 2030 3030  ....0000002c 000
+00001f00: 3030 3230 3020 3766 6666 6666 6666 200d  00200 7fffffff .
+00001f10: 0a7b bf7b 7fb5 914e 92a5 418a 85a9 8599  .{.{...N..A.....
+00001f20: 6ea2 a151 aaae 8969 1a88 6561 a46b 926a  n..Q...i..ea.k.j
+00001f30: 9a68 6061 9e64 9862 64a1 530b 0000 0000  .h`a.d.bd.S.....
 00001f40: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001f50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001f60: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001f70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001f80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001f90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001fa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -522,23 +522,23 @@
 00002090: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000020a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000020b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000020c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000020d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000020e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000020f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002100: 0000 0000 0000 0000 0000 0000 0000 0d0a  ................
-00002110: 3030 3030 3030 3236 2030 3030 3030 3032  00000026 0000002
-00002120: 3620 3766 6666 6666 6666 200d 0a10 8ceb  6 7fffffff .....
-00002130: e645 4402 0010 8ceb e645 4402 0000 0000  .ED......ED.....
-00002140: 0076 0065 0072 0073 0069 006f 006e 0000  .v.e.r.s.i.o.n..
-00002150: 0000 000d 0a30 3030 3030 3031 6320 3030  .....0000001c 00
-00002160: 3030 3032 3030 2037 6666 6666 6666 6620  000200 7fffffff 
-00002170: 0d0a 7bbf 7b7f 352f 57b5 91a1 998e 810e  ..{.{.5/W.......
-00002180: 9061 6160 6c68 a463 50cb cb05 4200 0000  .aa`lh.cP...B...
+00002100: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002110: 000d 0a30 3030 3030 3032 3620 3030 3030  ...00000026 0000
+00002120: 3030 3236 2037 6666 6666 6666 6620 0d0a  0026 7fffffff ..
+00002130: b0f5 4b60 4e44 0200 b0f5 4b60 4e44 0200  ..K`ND....K`ND..
+00002140: 0000 0000 7600 6500 7200 7300 6900 6f00  ....v.e.r.s.i.o.
+00002150: 6e00 0000 0000 0d0a 3030 3030 3030 3163  n.......0000001c
+00002160: 2030 3030 3030 3230 3020 3766 6666 6666   00000200 7fffff
+00002170: 6666 200d 0a7b bf7b 7f35 2f57 b591 a199  ff ..{.{.5/W....
+00002180: 8e81 0e90 6161 606c 68a4 6350 cbcb 0542  ....aa`lh.cP...B
 00002190: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000021a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000021b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000021c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000021d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000021e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000021f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -561,46 +561,46 @@
 00002300: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002310: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002320: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002330: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002340: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002350: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002360: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002370: 0000 0d0a 3030 3030 3030 3238 2030 3030  ....00000028 000
-00002380: 3030 3032 3820 3766 6666 6666 6666 200d  00028 7fffffff .
-00002390: 0a10 8ceb e645 4402 0010 8ceb e645 4402  .....ED......ED.
-000023a0: 0000 0000 0076 0065 0072 0073 0069 006f  .....v.e.r.s.i.o
-000023b0: 006e 0073 0000 0000 000d 0a30 3030 3030  .n.s.......00000
-000023c0: 3138 6420 3030 3030 3032 3030 2037 6666  18d 00000200 7ff
-000023d0: 6666 6666 6620 0d0a 8d92 318e 5631 0c84  fffff ....1.V1..
-000023e0: eff2 ea67 643b 76e2 1cc7 4e1c 699b fd11  ...gd;v...N.i...
-000023f0: 2024 8438 1905 47e2 0af8 35d4 db44 29ec   $.8..G...5..D).
-00002400: c97c 33f9 fbfb cf4f ba89 eeeb bacf c49c  .|3....O........
-00002410: 2b36 f038 0ed2 3a81 a76c 9803 5df7 49e7  +6.8..:..l..].I.
-00002420: cdf7 a5e4 28b8 05c2 4d41 ac4f b0c1 0428  ....(...MA.O...(
-00002430: e3a8 44e2 dee3 135e b79d d984 5161 6412  ..D....^....Qad.
-00002440: 48ba 8073 6b25 a939 4312 35c6 7d75 a6d1  H..sk%.9C.5.}u..
-00002450: 230c baad 0325 d1c0 d644 d0d4 c936 7377  #....%...D...6sw
-00002460: ded7 ddc9 694c ea40 5b3a c85c 2573 3821  ....iL.@[:.\%s8!
-00002470: 3d5b 9726 7ae4 7c4c eb71 e627 49ac 2588  =[.&z.|L.q.'I.%.
-00002480: ac59 47b6 6229 e289 eb68 6050 572c 35c1  .YG.b)...h`PW,5.
-00002490: e58b 1b68 d8f3 e648 b083 0bd2 d822 b2a5  ...h...H....."..
-000024a0: 7b2b 6767 6be3 2060 1d51 99a9 c0ec d660  {+ggk. `.Q.....`
-000024b0: 3269 311e 967e 3ea6 f538 6357 cb55 71f9  2i1..~>..8cW.Uq.
-000024c0: 2003 c143 1052 b088 e2e5 1049 4f39 8b89   ..C.R.....IO9..
-000024d0: dbb4 849c 2a83 827f 6ec6 95b1 3ada 08da  ....*...n...:...
-000024e0: 6cd7 bda8 a71c 9e30 b455 1ac6 0ede 8641  l......0.U.....A
-000024f0: 549d ea66 3ece bcaf f5fa fce3 edfd bcaa  T..f>...........
-00002500: fd81 a89d 17f8 1ad5 eb69 35af 95ca d670  .........i5....p
-00002510: 5a98 a365 bbaf 2faf d7b7 eb1e ec94 a719  Z..e../.........
-00002520: e4f2 51d4 bcc1 2807 34dd 2d28 82ac 95cf  ..Q...(.4.-(....
-00002530: eff9 e5eb dbeb bdb0 428d 672f f2f1 d8a4  ........B.g/....
-00002540: 1610 26b5 6d95 47b1 138f fe7f fc6b cd13  ..&.m.G......k..
-00002550: e6ea e3c0 eafb f988 94e0 cf7a 44f7 4e86  ...........zD.N.
-00002560: ac4d 7efd 0300 0000 0000 0000 0000 0000  .M~.............
+00002370: 0000 0000 000d 0a30 3030 3030 3032 3820  .......00000028 
+00002380: 3030 3030 3030 3238 2037 6666 6666 6666  00000028 7ffffff
+00002390: 6620 0d0a b0f5 4b60 4e44 0200 b0f5 4b60  f ....K`ND....K`
+000023a0: 4e44 0200 0000 0000 7600 6500 7200 7300  ND......v.e.r.s.
+000023b0: 6900 6f00 6e00 7300 0000 0000 0d0a 3030  i.o.n.s.......00
+000023c0: 3030 3031 3863 2030 3030 3030 3230 3020  00018c 00000200 
+000023d0: 3766 6666 6666 6666 200d 0a8d 9141 6e5e  7fffffff ....An^
+000023e0: 3108 84ef f2d6 8f08 30d8 701c 6363 299b  1.......0.p.cc).
+000023f0: fc55 5255 aaaa 9eac 8b1e a957 28ff 26eb  .URU.......W(.&.
+00002400: ec90 187d cc0c fffe fcfd 4537 d17d 5df7  ...}......E7.}].
+00002410: 645c a6cd 61b5 6820 a3a6 c943 2130 6210  d\..a.h ...C!0b.
+00002420: bb0d 5af7 a534 5170 0bc4 3405 b1ee 6083  ..Z..4Qp..4...`.
+00002430: 0950 c651 89c4 bdc7 0b5e f7a6 cd39 6c81  .P.Q.....^...9l.
+00002440: a13b 084a c2cc d361 3796 43d4 7c62 dc57  .;.J...a7.C.|b.W
+00002450: 671a 3dc2 a0db 3a75 f334 b0e5 089a ea6c  g.=...:u.4.....l
+00002460: 9ebb f3be 6e3b ec31 a7c0 3009 9013 01ee  ....n;.1..0.....
+00002470: cfeb 23e6 3ec6 c14c 5f63 3d9d ad3e c789  ..#.>..L_c=..>..
+00002480: d1a1 3155 ce45 0216 7440 d754 b5ce a622  ..1U.E..t@.T..."
+00002490: 4513 5c73 7103 0deb 203e 12ec e082 34b6  E.\sq... >....4.
+000024a0: 886c 3967 2b67 b631 5b35 d5f9 7993 7580  .l9g+g.1[5..y.u.
+000024b0: 6d9f 809c 41b4 f7ac 82be c67a 3ad3 6dea  m...A......z:.m.
+000024c0: 031b 9023 8168 990f e77a c374 ef16 56e6  ...#.h...z.t..V.
+000024d0: 2a67 3896 ae40 9338 4b75 9e93 3148 ea44  *g8..@.8Ku..1H.D
+000024e0: 1b51 c5db 750f 666d d1b1 58a3 76db 8a55  .Q..u.fm..X.v..U
+000024f0: 3bc8 73b4 11c5 e9aa f7b5 1edf 7ebe be9d  ;.s.........~...
+00002500: c775 7ba5 e89d 07d0 99d5 f1d0 a856 42e1  .u{..........VB.
+00002510: 9067 1252 f65d 49de 1f8f efc5 debd 1ddd  .g.R.]I.........
+00002520: 4fd8 1ed5 2033 cc95 0ea8 bcd7 da22 d44a  O... 3.......".J
+00002530: fb23 df3f 5e1f 6fd7 1d23 5b67 61d0 73a4  .#.?^.o..#[ga.s.
+00002540: e267 8263 6fd0 b035 f685 96c7 3ee5 1fa5  .g.co..5....>...
+00002550: f7c5 58cd 41ea da15 ab7e 13b2 0f98 af91  ..X.A....~......
+00002560: 9377 88cc dfff 0100 0000 0000 0000 0000  .w..............
 00002570: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002580: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002590: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000025a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000025b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000025c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000025d0: 0000 0000 0000 0000                      ........
+000025d0: 0000 0000 0000 0000 0000 00              ...........
```

### Comparing `runner1c-0.57/runner1c/build/tools/epf/FileCompareMxl.epf` & `runner1c-0.58/runner1c/build/tools/epf/FileCompareMxl.epf`

 * *Files 15% similar despite different names*

```diff
@@ -30,16 +30,16 @@
 000001d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000200: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000210: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000220: 0000 0000 0000 0000 0000 0000 0000 000d  ................
 00000230: 0a30 3030 3030 3036 3020 3030 3030 3030  .00000060 000000
-00000240: 3630 2037 6666 6666 6666 6620 0d0a 20b3  60 7fffffff .. .
-00000250: ebe6 4544 0200 20b3 ebe6 4544 0200 0000  ..ED.. ...ED....
+00000240: 3630 2037 6666 6666 6666 6620 0d0a c01c  60 7fffffff ....
+00000250: 4c60 4e44 0200 c01c 4c60 4e44 0200 0000  L`ND....L`ND....
 00000260: 0000 3100 3900 6600 3500 6500 3700 3900  ..1.9.f.5.e.7.9.
 00000270: 3500 2d00 3900 6200 6600 3900 2d00 3400  5.-.9.b.f.9.-.4.
 00000280: 6600 3700 6500 2d00 3900 3600 3300 6300  f.7.e.-.9.6.3.c.
 00000290: 2d00 3500 3800 3700 3500 3900 6200 6100  -.5.8.7.5.9.b.a.
 000002a0: 3900 3600 3600 3100 3500 0000 0000 0d0a  9.6.6.1.5.......
 000002b0: 3030 3030 3031 3531 2030 3030 3030 3230  00000151 0000020
 000002c0: 3020 3766 6666 6666 6666 200d 0a8d 914b  0 7fffffff ....K
@@ -72,16 +72,16 @@
 00000470: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000480: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000490: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000004a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000004b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000004c0: 0000 0000 0000 0000 0000 0000 000d 0a30  ...............0
 000004d0: 3030 3030 3036 3020 3030 3030 3030 3630  0000060 00000060
-000004e0: 2037 6666 6666 6666 6620 0d0a 20b3 ebe6   7fffffff .. ...
-000004f0: 4544 0200 20b3 ebe6 4544 0200 0000 0000  ED.. ...ED......
+000004e0: 2037 6666 6666 6666 6620 0d0a c01c 4c60   7fffffff ....L`
+000004f0: 4e44 0200 c01c 4c60 4e44 0200 0000 0000  ND....L`ND......
 00000500: 3900 3300 3500 3300 3300 6300 6100 3800  9.3.5.3.3.c.a.8.
 00000510: 2d00 3300 3600 6300 3400 2d00 3400 3400  -.3.6.c.4.-.4.4.
 00000520: 3200 3300 2d00 3900 3400 3100 3900 2d00  2.3.-.9.4.1.9.-.
 00000530: 3200 3600 3000 3600 3000 3900 3000 3400  2.6.0.6.0.9.0.4.
 00000540: 3400 3600 3200 3400 0000 0000 0d0a 3030  4.6.2.4.......00
 00000550: 3030 3030 3965 2030 3030 3030 3230 3020  00009e 00000200 
 00000560: 3766 6666 6666 6666 200d 0a95 4f49 0a02  7fffffff ...OI..
@@ -114,16 +114,16 @@
 00000710: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000720: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000730: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000740: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000750: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000760: 0000 0000 0000 0000 0000 000d 0a30 3030  .............000
 00000770: 3030 3036 3420 3030 3030 3030 3634 2037  00064 00000064 7
-00000780: 6666 6666 6666 6620 0d0a 20b3 ebe6 4544  fffffff .. ...ED
-00000790: 0200 20b3 ebe6 4544 0200 0000 0000 3900  .. ...ED......9.
+00000780: 6666 6666 6666 6620 0d0a c01c 4c60 4e44  fffffff ....L`ND
+00000790: 0200 c01c 4c60 4e44 0200 0000 0000 3900  ....L`ND......9.
 000007a0: 3300 3500 3300 3300 6300 6100 3800 2d00  3.5.3.3.c.a.8.-.
 000007b0: 3300 3600 6300 3400 2d00 3400 3400 3200  3.6.c.4.-.4.4.2.
 000007c0: 3300 2d00 3900 3400 3100 3900 2d00 3200  3.-.9.4.1.9.-.2.
 000007d0: 3600 3000 3600 3000 3900 3000 3400 3400  6.0.6.0.9.0.4.4.
 000007e0: 3600 3200 3400 2e00 3000 0000 0000 0d0a  6.2.4...0.......
 000007f0: 3030 3030 3064 3032 2030 3030 3030 6430  00000d02 00000d0
 00000800: 3220 3766 6666 6666 6666 200d 0aed 5c5b  2 7fffffff ...\[
@@ -332,16 +332,16 @@
 000014b0: 8174 c917 ad61 6325 0992 349c 1112 41ec  .t...ac%..4...A.
 000014c0: 4bc1 52e1 3c84 3579 e2d8 41ec cf82 0984  K.R.<.5y..A.....
 000014d0: 8f28 e361 8188 7d0a 9f62 6533 12e1 0ddb  .(.a..}..be3....
 000014e0: 7155 c842 f33f c754 f5c6 8eab b57a 1ef6  qU.B.?.T.....z..
 000014f0: 3318 36a4 8e2d c5bf 13ec 3c3a 9547 f8cb  3.6..-....<:.G..
 00001500: c598 cdea fb3b 2bc1 9437 03d1 a5ff 0f0d  .....;+..7......
 00001510: 0a30 3030 3030 3032 3820 3030 3030 3030  .00000028 000000
-00001520: 3238 2037 6666 6666 6666 6620 0d0a 20b3  28 7fffffff .. .
-00001530: ebe6 4544 0200 20b3 ebe6 4544 0200 0000  ..ED.. ...ED....
+00001520: 3238 2037 6666 6666 6666 6620 0d0a c01c  28 7fffffff ....
+00001530: 4c60 4e44 0200 c01c 4c60 4e44 0200 0000  L`ND....L`ND....
 00001540: 0000 6300 6f00 7000 7900 6900 6e00 6600  ..c.o.p.y.i.n.f.
 00001550: 6f00 0000 0000 0d0a 3030 3030 3030 6365  o.......000000ce
 00001560: 2030 3030 3030 3230 3020 3766 6666 6666   00000200 7fffff
 00001570: 6666 200d 0a8d 8f3d 8a03 310c 46fb 402e  ff ....=..1.F.@.
 00001580: 91da 0259 7f63 d781 747b 085b b661 2121  ...Y.c..t{.[.a!!
 00001590: 4baa 8590 936d b147 ca15 7666 92ed a7f9  K....m.G..vf....
 000015a0: 04e2 d3e3 e9f9 f37b 97b0 dfdd 6989 ccca  .......{....i...
@@ -371,16 +371,16 @@
 00001720: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001730: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001740: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001750: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001760: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001770: 0000 0000 000d 0a30 3030 3030 3032 3020  .......00000020 
 00001780: 3030 3030 3030 3230 2037 6666 6666 6666  00000020 7ffffff
-00001790: 6620 0d0a 20b3 ebe6 4544 0200 20b3 ebe6  f .. ...ED.. ...
-000017a0: 4544 0200 0000 0000 7200 6f00 6f00 7400  ED......r.o.o.t.
+00001790: 6620 0d0a c01c 4c60 4e44 0200 c01c 4c60  f ....L`ND....L`
+000017a0: 4e44 0200 0000 0000 7200 6f00 6f00 7400  ND......r.o.o.t.
 000017b0: 0000 0000 0d0a 3030 3030 3030 3265 2030  ......0000002e 0
 000017c0: 3030 3030 3230 3020 3766 6666 6666 6666  0000200 7fffffff
 000017d0: 200d 0a7b bf7b 7fb5 918e a165 9a69 aab9   ..{.{.....e.i..
 000017e0: a5a9 ae65 529a a5ae 499a 79aa aea5 9971  ...eR...I.y....q
 000017f0: b2ae a985 b9a9 6552 a2a5 9999 a1a9 4e2d  ......eR......N-
 00001800: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001810: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -409,15 +409,15 @@
 00001980: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001990: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000019a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000019b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000019c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000019d0: 0000 000d 0a30 3030 3030 3032 3620 3030  .....00000026 00
 000019e0: 3030 3030 3236 2037 6666 6666 6666 6620  000026 7fffffff 
-000019f0: 0d0a 20b3 ebe6 4544 0200 20b3 ebe6 4544  .. ...ED.. ...ED
+000019f0: 0d0a c01c 4c60 4e44 0200 c01c 4c60 4e44  ....L`ND....L`ND
 00001a00: 0200 0000 0000 7600 6500 7200 7300 6900  ......v.e.r.s.i.
 00001a10: 6f00 6e00 0000 0000 0d0a 3030 3030 3030  o.n.......000000
 00001a20: 3163 2030 3030 3030 3230 3020 3766 6666  1c 00000200 7fff
 00001a30: 6666 6666 200d 0a7b bf7b 7f35 2f57 b591  ffff ..{.{.5/W..
 00001a40: a199 8e81 0e90 6161 606c 68a4 6350 cbcb  ......aa`lh.cP..
 00001a50: 0542 0000 0000 0000 0000 0000 0000 0000  .B..............
 00001a60: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -447,37 +447,37 @@
 00001be0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001bf0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001c00: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001c10: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001c20: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001c30: 0000 0000 0000 000d 0a30 3030 3030 3032  .........0000002
 00001c40: 3820 3030 3030 3030 3238 2037 6666 6666  8 00000028 7ffff
-00001c50: 6666 6620 0d0a 20b3 ebe6 4544 0200 20b3  fff .. ...ED.. .
-00001c60: ebe6 4544 0200 0000 0000 7600 6500 7200  ..ED......v.e.r.
+00001c50: 6666 6620 0d0a c01c 4c60 4e44 0200 c01c  fff ....L`ND....
+00001c60: 4c60 4e44 0200 0000 0000 7600 6500 7200  L`ND......v.e.r.
 00001c70: 7300 6900 6f00 6e00 7300 0000 0000 0d0a  s.i.o.n.s.......
 00001c80: 3030 3030 3031 3163 2030 3030 3030 3230  0000011c 0000020
-00001c90: 3020 3766 6666 6666 6666 200d 0a8d 9141  0 7fffffff ....A
-00001ca0: 4e86 210c 44ef c29a 1a28 6da1 c781 4213  N.!.D....(m...B.
-00001cb0: 377e 468d 8931 9ecc 8547 f20a f677 e1da  7~F..1...G...w..
-00001cc0: 1d09 336f a6ed f7e7 d77b cd23 a794 170b  ..3o.....{.#....
-00001cd0: ab0f 053a d380 da14 1858 1444 e560 7763  ...:.....X.D.`wc
-00001ce0: aa92 5355 e7d3 9541 9787 d4fb 0195 66c0  ..SU...A......f.
-00001cf0: a3b3 aea9 2295 5336 8bef 5337 f4c9 0234  ....".S6..S7...4
-00001d00: 1d61 f05c d087 a395 d379 969e 9336 6ecd  .a.\.....y...6n.
-00001d10: e680 2646 4084 0d94 aa02 4a91 a285 4890  ..&F@.....J...H.
-00001d20: 7e59 a5d9 98b0 3675 20e5 c866 acd0 22bc  ~Y....6u ..f..".
-00001d30: b81c b5b6 fec7 ba2b 294f 668b 678d 520b  .......+)Of.g.R.
-00001d40: 63ca c6b0 a620 1c12 2fb3 5633 b79c ec7a  c.... ../.V3...z
-00001d50: 7cbb 7ff0 eba6 3fc2 636d 686b 9f30 3504  |.....?.cmhk.05.
-00001d60: eddb 6119 1f5c 85b6 ac48 7fba ae97 94d9  ..a..\...H......
-00001d70: 25ba f60d 8b4f 6c10 2576 53c3 4a95 4bf7  %....Ol.%vS.J.K.
-00001d80: 364f 4c9f d3eb 797a bebf 1e52 ee2a c81a  6OL...yz...R.*..
-00001d90: 4031 0bb4 f502 c337 c234 772f 3845 5dfe  @1.....7.4w/8E].
-00001da0: e4cf 2957 2626 bcb5 901d f85b 1f9d e4e1  ..)W&&.....[....
-00001db0: 2ce7 047e c6fd 3e7e 0000 0000 0000 0000  ,..~..>~........
+00001c90: 3020 3766 6666 6666 6666 200d 0a8d 904b  0 7fffffff ....K
+00001ca0: 6e50 310c 45f7 9271 8cec f813 7b39 713e  nP1.E..q....{9q>
+00001cb0: 5227 7da8 4548 08b1 3206 2c89 2d90 4e3a  R'}.EH..2.,.-.N:
+00001cc0: 666e 9f7b eff9 fbfb cf4f aa5e 4ba9 3b31  fn.{.....O.^K.;1
+00001cd0: 8677 07ec 6e20 2213 86ce 017b 8f3e 0871  .w..n "....{.>.q
+00001ce0: e59a b550 1cdd 3d14 224f 809c be21 8c27  ...P..=."O...!.'
+00001cf0: a877 8d1c 6146 5aea f023 2e97 7524 1c24  .w..aFZ..#..u$.$
+00001d00: e3b2 1a13 0c5c 819e c1c2 544b b032 cfe1  .....\....TK.2..
+00001d10: c036 e526 3686 100a 6886 8681 22d6 a454  .6.&6...h..."..T
+00001d20: 6d31 f58c 0e19 ed26 2a19 8c35 1832 795d  m1.....&*..5.2y]
+00001d30: ba8d eced ff58 5fb0 d4a5 b769 ac06 e871  .....X_....i...q
+00001d40: 57f6 9310 6b6d 681c 9626 4bc4 2f6d 3e5f  W...kmh..&K./m>_
+00001d50: 7fbc bc9e a7d4 e446 a363 8261 7eec 4502  .......F.c.a~.E.
+00001d60: 8ffb c99b 8e20 db38 78ad bc3d cfb7 525b  ..... .8x..=..R[
+00001d70: e8da 1e09 53b7 5e36 250c cb03 11aa 3ad8  ....S.^6%.....:.
+00001d80: 6cc7 aee5 fb7e 7b7f 795e 4b0d 4e15 a20d  l....~{.y^K.N...
+00001d90: 9b8c 41f6 c63b cc14 d6ea ce76 dca6 c7e7  ..A..;.....v....
+00001da0: f97b a9e7 ec7d 2811 92ae 4f41 3dd7 2775  .{...}(...OA=.'u
+00001db0: 7041 5ad7 8378 e6af 7f00 0000 0000 0000  pAZ..x..........
 00001dc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001dd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001de0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001df0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001e00: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001e10: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001e20: 0000 0000 0000 0000 0000 0000 0000 0000  ................
```

### Comparing `runner1c-0.57/runner1c/command.py` & `runner1c-0.58/runner1c/command.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,54 +27,62 @@
             return func(self)
         else:
             temp_folder = tempfile.mkdtemp()
             connection = 'File={}'.format(temp_folder)
 
             p_create_base = runner1c.command.EmptyParameters(self.arguments)
             setattr(p_create_base, 'connection', connection)
-            return_code = CreateBase(arguments=p_create_base).execute()
+            # todo нужно копирование logger handler при multiprocessing
+            command = CreateBase(arguments=p_create_base)
+            return_code = command.execute()
 
             if runner1c.exit_code.success_result(return_code):
                 setattr(self.arguments, 'connection', connection)
                 return_code = self.execute()
 
             common.clear_folder(temp_folder)
 
             return return_code
 
     return wrapper
 
 
 class Command(abc.ABC):
     def __init__(self, **kwargs):
+        self._logger = kwargs.get('logger', None)
+        if self._logger is None:
+            self._logger = logging.getLogger(self.name)
+
         self.arguments = copy.copy(kwargs['arguments'])
         self._mode = kwargs.get('mode', None)
-        agent_channel = kwargs.get('agent_channel', None)
 
+        self._client = None
+        self._channel = None
+        self._connect_to_agent = False
         self._need_close_agent = False
-        self._agent_started = False
-        self._logger = logging.getLogger(self.name)
+        agent_channel = kwargs.get('agent_channel', None)
+        if agent_channel is not None:
+            self._client, self._channel = agent_channel
+            self._connect_to_agent = True
+        self._agent_port = kwargs.get('agent_port', None)
         self._agent_folder = ''
         self._agent_process = None
+        self._agent_server = '127.0.0.1'
 
         self._program_1c_arguments = []
         self._program_1c = ''
         self._version_1c = ''
 
         if self._mode == Mode.DESIGNER:
             self._set_designer()
         elif self._mode == Mode.ENTERPRISE:
             self._set_enterprise()
         elif self._mode == Mode.CREATE:
             self._set_create_base()
 
-        if agent_channel is not None:
-            self._client, self._channel = agent_channel
-            self._agent_started = True
-
         self._set_path_1c()
 
     @property
     def name(self):
         return self.__class__.__name__
 
     @property
@@ -99,58 +107,65 @@
 
     def debug(self, msg, *args):
         self._logger.debug(msg, *args)
 
     def error(self, msg, *args):
         self._logger.error(msg, *args)
 
-    def start_agent(self):
-        if self._agent_started:
+    def start_agent(self, logger=None):
+        if self._connect_to_agent:
             return
 
-        port_agent = self._get_port_for_agent()
+        self._need_close_agent = True
+
+        self._agent_port = self._get_port_for_agent()
         self._agent_folder = os.path.split(self.arguments.folder)[0]
 
         # запуск конфигуратора в режиме агента
         p_agent = runner1c.command.EmptyParameters(self.arguments)
         setattr(p_agent, 'connection', self.arguments.connection)
         setattr(p_agent, 'folder', self._agent_folder)
-        setattr(p_agent, 'port', port_agent)
-        agent = StartAgent(arguments=p_agent)
+        setattr(p_agent, 'port', self._agent_port)
+        # todo нужно копирование logger handler при multiprocessing
+        agent = StartAgent(arguments=p_agent, logger=logger)
         return_code = agent.execute()
         if not runner1c.exit_code.success_result(return_code):
             raise Exception('Failed start agent')
 
         self._agent_process = agent.process
-        self._agent_started = True
-        self._need_close_agent = True
         del agent
 
-        # подключение к агенту
+    def connect_to_agent(self):
+        if self._connect_to_agent:
+            return
+
+        self.debug(f'connect to agent port={self._agent_port}')
 
         self._client = paramiko.SSHClient()
         self._client.set_missing_host_key_policy(paramiko.AutoAddPolicy())
-        self._client.connect(hostname='127.0.0.1', username='', password='', port=port_agent)
+        self._client.connect(hostname=self._agent_server, username='', password='', port=self._agent_port)
 
         self._channel = self._client.get_transport().open_session()
         self._channel.invoke_shell()
 
+        self._connect_to_agent = True
+
         # пропуск приветствия
         self._channel.recv(common.MAXIMUM_BYTES_READ)
 
         # установка формата ответа
         self.send_to_agent('options set --output-format=json --show-prompt=no', False)
 
         return_code = self.send_to_agent('common connect-ib')
         if not runner1c.exit_code.success_result(return_code):
             raise Exception('Failed connect to agent')
 
     def send_to_agent(self, command, wait_response=True):
-        if not self._agent_started:
-            raise Exception('Agent not started')
+        if not self._connect_to_agent:
+            raise Exception('No connect to agent')
 
         result_code = runner1c.exit_code.EXIT_CODE.error
         self.debug('agent send "%s"', command)
 
         self._channel.send(command + '\n')
 
         result_sting = self._get_response_from_agent()
@@ -176,41 +191,51 @@
         else:
             result_code = runner1c.exit_code.EXIT_CODE.done
 
         self.debug('agent response result = %s', result_code)
 
         return result_code
 
+    def disconnect_from_agent(self):
+        if not self._connect_to_agent:
+            return
+
+        self.debug(f'disconnect from agent port={self._agent_port}')
+
+        self._channel.close()
+        self._client.close()
+
+        self._connect_to_agent = False
+
     def close_agent(self):
         if not self._need_close_agent:
             return
-        if not self._agent_started:
-            return
 
-        self.send_to_agent('common disconnect-ib', False)
+        if not self._connect_to_agent:
+            self.connect_to_agent()
 
+        self.send_to_agent('common disconnect-ib', False)
         if not self.bug_platform('8.3.20'):
             self.send_to_agent('common shutdown', False)
 
-        self._channel.close()
-        self._client.close()
-
-        self._agent_started = False
+        self._connect_to_agent = False
 
         if self.bug_platform('8.3.20') and self._agent_process is not None:
             self._agent_process.kill()
 
         # при старте агента 1с создает служебные файлы, иногда за собой не убирает
         common.delete_file(os.path.join(self._agent_folder, 'agentbasedir.json'))
         common.clear_folder(os.path.join(self._agent_folder, '0'))
-        #common.delete_file(os.path.join(os.getcwd(), '1cv8u.pfl'))
 
     def get_agent_channel(self):
         return self._client, self._channel
 
+    def get_agent_port(self):
+        return self._agent_port
+
     def add_argument(self, string):
         self._program_1c_arguments.append(string)
 
     def get_program_arguments(self):
         self._set_log_result()
 
         if getattr(self.arguments, 'connection', False):
@@ -455,15 +480,15 @@
 
         port_agent = 1543
         find_port = False
 
         while port_agent < 1600:
             sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
             sock.settimeout(2)
-            result = sock.connect_ex(('127.0.0.1', port_agent))
+            result = sock.connect_ex((self._agent_server, port_agent))
             if result == 0:
                 port_agent = port_agent + 1
             else:
                 sock.close()
                 find_port = True
                 break
```

### Comparing `runner1c-0.57/runner1c/commands/base_for_test.py` & `runner1c-0.58/runner1c/commands/load_extension.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,143 +1,137 @@
-import asyncio
 import os
-import tempfile
 
 import runner1c
-import runner1c.commands.load_config as load_config
-import runner1c.commands.load_extension as load_extension
 import runner1c.commands.start
-import runner1c.commands.sync as sync
 import runner1c.common as common
 import runner1c.exit_code as exit_code
 
 
-class BaseForTestParser(runner1c.parser.Parser):
+class LoadExtensionParser(runner1c.parser.Parser):
     @property
     def name(self):
-        return 'base_for_test'
+        return 'load_extension'
 
     @property
     def description(self):
-        return 'создание базы из исходников для тестирования'
+        return 'загрузка расширения из исходников'
 
     def create_handler(self, **kwargs):
-        return BaseForTest(**kwargs)
+        return LoadExtension(**kwargs)
 
     def set_up(self):
         self.add_argument_to_parser()
-        self._parser.add_argument('--thick', action='store_const', const=True, help='толстый клиент')
-        self._parser.add_argument('--folder', required=True, help='путь к папке репозитория')
-        self._parser.add_argument('--create_epf', action='store_const', const=True, help='создать внешние '
-                                                                                         'обработки репозитория')
-        self._parser.add_argument('--create_cfe', action='store_const', const=True, help='загрузить расширения '
-                                                                                         'репозитория')
+        self._parser.add_argument('--folder', required=True, help='каталог, содержащий исходники расширений '
+                                                                  'конфигурации')
+        self._parser.add_argument('--name', help='имя расширений, которые нужно загрузить через запятую')
+        self._parser.add_argument('--update', action='store_const', const=True, help='обновление конфигурации '
+                                                                                     'базы данных')
+        self._parser.add_argument('--agent',
+                                  action='store_const',
+                                  const=True,
+                                  help='запускать конфигуратор в режиме агента')
+
+
+class LoadExtension(runner1c.command.Command):
+    def __init__(self, **kwargs):
+        kwargs['mode'] = runner1c.command.Mode.DESIGNER
+        super().__init__(**kwargs)
+
+        if getattr(self.arguments, 'agent', False):
+            return
+
+        if getattr(self.arguments, 'name', False):
+            setattr(self.arguments, 'folder_with_ext', os.path.join(self.arguments.folder, self.arguments.name))
+        else:
+            setattr(self.arguments, 'folder_with_ext', self.arguments.folder)
+
+        self.add_argument('/LoadConfigFromFiles "{folder_with_ext}"')
+
+        if getattr(self.arguments, 'name', False):
+            self.add_argument('-Extension "{name}"')
+        else:
+            self.add_argument('-AllExtensions')
 
+        if getattr(self.arguments, 'update', False):
+            self.add_argument('/UpdateDBCfg')
 
-async def start_enterprise(self, path_to_fixtures):
-    p_start = runner1c.command.EmptyParameters(self.arguments)
-    setattr(p_start, 'connection', self.arguments.connection)
-    setattr(p_start, 'thick', self.arguments.thick)
-    setattr(p_start, 'epf', common.get_path_to_project(os.path.join('runner1c',
-                                                                    'build',
-                                                                    'tools',
-                                                                    'epf',
-                                                                    'CloseAfterUpdate.epf')))
-
-    if os.path.exists(path_to_fixtures):
-        setattr(p_start, 'options', path_to_fixtures)
-    command_start = runner1c.commands.start.Start(arguments=p_start)
-
-    program_arguments = command_start.get_program_arguments()
-    self.debug('get_program_arguments %s', program_arguments)
-
-    file_parameters = tempfile.mktemp('.txt')
-    with open(file_parameters, mode='w', encoding='utf8') as file_parameters_stream:
-        file_parameters_stream.write(program_arguments)
-    file_parameters_stream.close()
-
-    cmd = command_start.get_program()
-    stdin = '/@ ' + file_parameters
-
-    self.debug('create_subprocess_exec %s %s', cmd, stdin)
-    process = await asyncio.create_subprocess_exec(cmd, stdin)
-
-    await process.wait()
-
-    common.delete_file(file_parameters)
-
-
-async def start_designer(self, exclude):
-    p_sync = runner1c.command.EmptyParameters(self.arguments)
-    setattr(p_sync, 'connection', self.arguments.connection)
-    setattr(p_sync, 'folder', self.arguments.folder)
-    setattr(p_sync, 'create', True)
-    setattr(p_sync, 'exclude', exclude)
-    sync.Sync(arguments=p_sync, agent_channel=self.get_agent_channel()).execute()
-
+    @property
+    def default_result(self):
+        return runner1c.exit_code.EXIT_CODE.done
 
-class BaseForTest(runner1c.command.Command):
     def execute(self):
+        if getattr(self.arguments, 'name', False):
+            extensions_name = self.arguments.name.split(',')
+        else:
+            extensions_name = self._get_extensions_name()
+
+        if len(extensions_name) == 0:
+            return self.default_result
+
+        error_code = runner1c.exit_code.EXIT_CODE.error
+
+        if not getattr(self.arguments, 'agent', False):
+
+            if getattr(self.arguments, 'name', False) and len(extensions_name) > 1:
+                error_in_loop = False
+                for name in extensions_name:
+                    p_extensions = runner1c.command.EmptyParameters(self.arguments)
+                    setattr(p_extensions, 'connection', self.arguments.connection)
+                    setattr(p_extensions, 'folder', self.arguments.folder)
+                    setattr(p_extensions, 'name', name)
+                    return_code = LoadExtension(arguments=p_extensions).execute()
+                    if not runner1c.exit_code.success_result(return_code):
+                        error_in_loop = True
+                        break
+                if error_in_loop:
+                    return error_code
+                else:
+                    return self.default_result
+            else:
+                return self.run()
 
-        config_src = os.path.join(self.arguments.folder, 'cf')
-        lib_src = 'lib'
-        ext_src = os.path.join(self.arguments.folder, lib_src, 'ext')
-        fixtures_src = os.path.join('spec', 'fixtures')
-        epf_src_before_async = ','.join([os.path.join(self.arguments.folder, fixtures_src),
-                                          os.path.join(self.arguments.folder, lib_src)])
-        path_to_fixtures = os.path.join(self.arguments.folder, 'build', fixtures_src)
-
-        p_create = runner1c.command.EmptyParameters(self.arguments)
-        setattr(p_create, 'connection', self.arguments.connection)
-        return_code = runner1c.command.CreateBase(arguments=p_create).execute()
-
-        if exit_code.success_result(return_code):
+        else:
 
+            return_code = error_code
             self.start_agent()
+            self.connect_to_agent()
 
             try:
-                p_load_config = runner1c.command.EmptyParameters(self.arguments)
-                setattr(p_load_config, 'connection', self.arguments.connection)
-                setattr(p_load_config, 'folder', config_src)
-                setattr(p_load_config, 'agent', True)
-                setattr(p_load_config, 'update', True)
-                return_code = load_config.LoadConfig(arguments=p_load_config,
-                                                     agent_channel=self.get_agent_channel()).execute()
-
-                if exit_code.success_result(return_code):
-
-                    if getattr(self.arguments, 'create_cfe', False):
-                        p_extensions = runner1c.command.EmptyParameters(self.arguments)
-                        setattr(p_extensions, 'connection', self.arguments.connection)
-                        setattr(p_extensions, 'folder', ext_src)
-                        setattr(p_extensions, 'agent', True)
-                        setattr(p_extensions, 'update', True)
-                        return_code = load_extension.LoadExtension(arguments=p_extensions,
-                                                     agent_channel=self.get_agent_channel()).execute()
-
-                    if getattr(self.arguments, 'create_epf', False):
-                        p_sync = runner1c.command.EmptyParameters(self.arguments)
-                        setattr(p_sync, 'connection', self.arguments.connection)
-                        setattr(p_sync, 'folder', self.arguments.folder)
-                        setattr(p_sync, 'create', True)
-                        setattr(p_sync, 'include', epf_src_before_async)
-                        return_code = sync.Sync(arguments=p_sync, agent_channel=self.get_agent_channel()).execute()
-
-                    if exit_code.success_result(return_code):
-                        loop = asyncio.ProactorEventLoop()
-                        asyncio.set_event_loop(loop)
-
-                        tasks = []
-                        if getattr(self.arguments, 'create_epf', False):
-                            tasks.append(start_designer(self, epf_src_before_async))
-                        tasks.append(start_enterprise(self, path_to_fixtures))
-
-                        loop.run_until_complete(asyncio.wait(tasks))
-                        loop.close()
-
+                for name in extensions_name:
+                    command = 'config load-files --dir "{}" --extension {}'
+                    return_code = self.send_to_agent(command.format(os.path.join(self.arguments.folder, name), name))
+                    if not exit_code.success_result(return_code):
+                        break
+                    if self.version_1c_greater('8.3.14'):
+                        command = 'config extensions properties set --extension {} --safe-mode no --unsafe-action-protection no'
+                        return_code = self.send_to_agent(command.format(name))
+                        if not exit_code.success_result(return_code):
+                            break
+                    if getattr(self.arguments, 'update', False):
+                        command = 'config update-db-cfg --extension {}'
+                        return_code = self.send_to_agent(command.format(name))
+                        if not exit_code.success_result(return_code):
+                            break
             except Exception as exception:
                 self.error(exception)
-                return_code = runner1c.exit_code.EXIT_CODE.error
-            finally:
-                self.close_agent()
+                return_code = error_code
+
+            if not self.version_1c_greater('8.3.14') and exit_code.success_result(return_code):
+                p_start = runner1c.command.EmptyParameters(self.arguments)
+                setattr(p_start, 'connection', self.arguments.connection)
+                setattr(p_start, 'epf', common.get_path_to_project(os.path.join('runner1c',
+                                                                                'build',
+                                                                                'tools',
+                                                                                'epf',
+                                                                                'ChangeSafeModeForExtension.epf')))
+                return_code = runner1c.commands.start.Start(arguments=p_start).execute()
+
+            return return_code
+
+    def _get_extensions_name(self):
+        if os.path.exists(self.arguments.folder):
+            result = os.listdir(self.arguments.folder)
+        else:
+            self.debug('не найден каталог расширений')
+            result = []
 
-        return return_code
+        return result
```

### Comparing `runner1c-0.57/runner1c/commands/create_epf.py` & `runner1c-0.58/runner1c/commands/create_epf.py`

 * *Files identical despite different names*

### Comparing `runner1c-0.57/runner1c/commands/diff_mxl.py` & `runner1c-0.58/runner1c/commands/diff_mxl.py`

 * *Files identical despite different names*

### Comparing `runner1c-0.57/runner1c/commands/dump_config.py` & `runner1c-0.58/runner1c/commands/dump_config.py`

 * *Files identical despite different names*

### Comparing `runner1c-0.57/runner1c/commands/dump_epf.py` & `runner1c-0.58/runner1c/commands/dump_epf.py`

 * *Files identical despite different names*

### Comparing `runner1c-0.57/runner1c/commands/dump_extensions.py` & `runner1c-0.58/runner1c/commands/dump_extensions.py`

 * *Files identical despite different names*

### Comparing `runner1c-0.57/runner1c/commands/file.py` & `runner1c-0.58/runner1c/commands/file.py`

 * *Files identical despite different names*

### Comparing `runner1c-0.57/runner1c/commands/load_config.py` & `runner1c-0.58/runner1c/commands/load_config.py`

 * *Files 10% similar despite different names*

```diff
@@ -36,27 +36,24 @@
         self.add_argument('/LoadConfigFromFiles "{folder}"')
         if getattr(self.arguments, 'update', False):
             self.add_argument('/UpdateDBCfg')
 
     def execute(self):
         if not getattr(self.arguments, 'agent', False):
             return self.run()
+        else:
 
-        self.start_agent()
+            try:
+                command = 'config load-config-from-files --dir "{}" --update-config-dump-info'
+                return_code = self.send_to_agent(command.format(self.arguments.folder))
+                if exit_code.success_result(return_code):
+                    return_code = self.send_to_agent('config update-db-cfg')
+
+            except Exception as exception:
+                self.error(exception)
+                return_code = exit_code.EXIT_CODE.error
 
-        try:
-            command = 'config load-config-from-files --dir "{}" --update-config-dump-info'
-            return_code = self.send_to_agent(command.format(self.arguments.folder))
-            if exit_code.success_result(return_code):
-                return_code = self.send_to_agent('config update-db-cfg')
-
-        except Exception as exception:
-            self.error(exception)
-            return_code = exit_code.EXIT_CODE.error
-        finally:
-            self.close_agent()
-
-        return return_code
+            return return_code
```

### Comparing `runner1c-0.57/runner1c/commands/platform_check.py` & `runner1c-0.58/runner1c/commands/platform_check.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,34 +27,29 @@
 
 
 class PlatformCheckConfig(runner1c.command.Command):
     def __init__(self, **kwargs):
         kwargs['mode'] = runner1c.command.Mode.DESIGNER
         super().__init__(**kwargs)
 
-        options_without_commas = self.arguments.options
-        if options_without_commas.startswith('"') and options_without_commas.endswith('"'):
-            options_without_commas = options_without_commas[1:-1]
-
-        self.arguments.options1c = ' '.join(['-' + x for x in options_without_commas.split(' ')])
-        self.add_argument('/CheckConfig "{options1c}"')
+        self.arguments.options1c = ' '.join(['-' + x for x in self.arguments.options.split(' ')])
+        self.add_argument('/CheckConfig {options1c}')
 
     def execute(self):
         return_code = self.run()
 
         _delete_plug_function(self.arguments.log)
 
         if getattr(self.arguments, 'skip_modality'):
             _delete_modality_error(self.arguments.skip_modality, self.arguments.log)
 
         if getattr(self.arguments, 'skip_object'):
             _delete_skip_object(self.arguments.skip_object, self.arguments.log)
 
-        if getattr(self.arguments, 'skip_error'):
-            _delete_skip_error(self.arguments.skip_error, self.arguments.log)
+        _delete_skip_error(self.arguments, self.arguments.log)
 
         return return_code
 
 
 def _delete_plug_function(log):
     unreference_procedure_error = 'Не обнаружено ссылок на'
     procedure_name_connectable = 'Подключаемый_'
@@ -116,32 +111,32 @@
     skip_lines = _read_file_to_list(skip_object)
 
     new_log_file = tempfile.mktemp('.txt')
     new_log_file_stream = open(new_log_file, mode='w', encoding='utf-8')
 
     log_file = open(log, mode='r', encoding='utf-8')
     for line in log_file:
-        add_string = True
+        if line[0] != '\t': # если строка начинается с табуляции, значит она относиться к предыдущей строке
+            add_string = True
         for error_line in skip_lines:
             if error_line.strip() in line:
                 add_string = False
                 break
         if add_string:
             new_log_file_stream.write(line)
 
     log_file.close()
     new_log_file_stream.close()
     shutil.move(new_log_file, log)
 
 
-def _delete_skip_error(skip_error, log):
-    if not os.path.exists(skip_error):
-        return
-
-    skip_lines = _read_file_to_list(skip_error)
+def _delete_skip_error(arguments, log):
+    skip_lines = []
+    if getattr(arguments, 'skip_error'):
+        skip_lines = _read_file_to_list(arguments.skip_error)
     skip_lines.append('Ошибок не обнаружено\n')
 
     new_log_file = tempfile.mktemp('.txt')
     new_log_file_stream = open(new_log_file, mode='w', encoding='utf-8')
 
     log_file = open(log, mode='r', encoding='utf-8')
     for line in log_file:
```

### Comparing `runner1c-0.57/runner1c/commands/reg_server.py` & `runner1c-0.58/runner1c/commands/reg_server.py`

 * *Files identical despite different names*

### Comparing `runner1c-0.57/runner1c/commands/start.py` & `runner1c-0.58/runner1c/commands/start.py`

 * *Files identical despite different names*

### Comparing `runner1c-0.57/runner1c/commands/start_agent.py` & `runner1c-0.58/runner1c/commands/start_agent.py`

 * *Files identical despite different names*

### Comparing `runner1c-0.57/runner1c/commands/sync.py` & `runner1c-0.58/runner1c/commands/sync.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,14 +54,15 @@
         result_code = self.default_result
         error_in_loop = False
         source_map = {}
 
         if getattr(self.arguments, 'create', True):
 
             self.start_agent()
+            self.connect_to_agent()
 
             try:
                 source_map = self._get_source()
                 for path_source, path_binary in source_map.items():
                     if path_binary.endswith(_FEATURE_SRC):
                         common.create_path(os.path.dirname(path_binary))
                         shutil.copy(path_source, path_binary)
```

### Comparing `runner1c-0.57/runner1c/commands/webinst.py` & `runner1c-0.58/runner1c/commands/webinst.py`

 * *Files identical despite different names*

### Comparing `runner1c-0.57/runner1c/common.py` & `runner1c-0.58/runner1c/common.py`

 * *Files 4% similar despite different names*

```diff
@@ -87,7 +87,11 @@
 def convert_cp1251_to_utf8(file_name):
     new_file = tempfile.mktemp('.txt')
     with open(new_file, mode='bw') as new_file_stream, open(file_name, mode='br') as old_file_stream:
         new_file_stream.write(old_file_stream.read().decode('cp1251').encode('utf-8'))
     new_file_stream.close()
     old_file_stream.close()
     shutil.move(new_file, file_name)
+
+
+def get_formatter_string():
+    return '%(asctime)s - %(levelname)s - %(name)19s (%(process)5d) - %(message)s'
```

### Comparing `runner1c-0.57/runner1c/core.py` & `runner1c-0.58/runner1c/core.py`

 * *Files 5% similar despite different names*

```diff
@@ -60,15 +60,15 @@
     else:
         list_argument = arg
         logger_name = 'File'
 
     arguments = parser.parse_args(list_argument)
 
     if arguments.debug:
-        logging.basicConfig(level=logging.DEBUG, format='%(asctime)s - %(levelname)s - %(name)19s - %(message)s')
+        logging.basicConfig(level=logging.DEBUG, format=common.get_formatter_string())
 
     logger = logging.getLogger(logger_name)
     logger.debug('start')
 
     handler = commands[arguments.command].create_handler(arguments=arguments)
     _check_override_methods(handler)
     return_code = handler.execute()
```

### Comparing `runner1c-0.57/runner1c/tests/test_diff_mxl.py` & `runner1c-0.58/runner1c/tests/test_diff_mxl.py`

 * *Files identical despite different names*

### Comparing `runner1c-0.57/runner1c/tests/test_sync_without_base.py` & `runner1c-0.58/runner1c/tests/test_sync_without_base.py`

 * *Files identical despite different names*

### Comparing `runner1c-0.57/runner1c/tests/test_version.py` & `runner1c-0.58/runner1c/tests/test_version.py`

 * *Files identical despite different names*

### Comparing `runner1c-0.57/runner1c/tests/test_with_base.py` & `runner1c-0.58/runner1c/tests/test_with_base.py`

 * *Files 3% similar despite different names*

```diff
@@ -71,30 +71,14 @@
 
     assert os.path.exists(os.path.join(repo_folder, 'epf', 'CheckConfig.xml'))
     assert os.path.exists(os.path.join(repo_folder, 'feature', 'Example.data'))
 
 
 @pytest.mark.dependency(depends=["test_base_for_test"])
 @pytest.mark.usefixtures("set_log_level")
-def test_platform_check_with_error(tmpdir, runner, base_dir):
-    log = str(tmpdir.join("log.html"))
-    argument = ['--debug',
-                'platform_check',
-                '--connection',
-                'File={}'.format(base_dir),
-                '--log',
-                log,
-                '--options',
-                '"{}"'.format(options_for_platform_check())]
-    assert runner(argument) == 0
-    assert count_lines_in_file(log) == 1
-
-
-@pytest.mark.dependency(depends=["test_base_for_test"])
-@pytest.mark.usefixtures("set_log_level")
 def test_platform_check_skip_modality(tmpdir, runner, base_dir):
     skip_file = str(tmpdir.join("skip.txt"))
     with open(skip_file, mode='w', encoding='utf-8') as file:
         file.write('Справочник.Catalog1.Форма.Form.Форма')
     file.close()
 
     log = str(tmpdir.join("log.html"))
```

### Comparing `runner1c-0.57/runner1c/tools/create_base_for_test.py` & `runner1c-0.58/runner1c/tools/create_base_for_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import json
 import os
 import re
 import shutil
 import tkinter
 import tkinter.filedialog as filedialog
 import tkinter.messagebox as messagebox
 from configparser import ConfigParser, NoOptionError
@@ -106,18 +107,18 @@
     CONFIG.set(repo_name, 'thick_client', str(thick_client))
 
     with open(INI_FILE, 'w') as file:
         CONFIG.write(file)
     file.close()
 
 
-def _save_git_path_for_base(base_path, repo_path):
-    txt_stream = open(os.path.join(base_path, 'GitPath.txt'), 'w')
-    txt_stream.write(repo_path)
-    txt_stream.close()
+def _save_parameters_for_acc(base_path, repo_path, platform_path):
+    map = {'repo': repo_path, 'platform': platform_path}
+    with open(os.path.join(base_path, 'parameters.txt'), 'w') as outfile:
+        json.dump(map, outfile)
 
 
 def _get_extension_name_from_file(file_path):
     path_for_search = file_path
 
     if os.path.splitext(file_path)[1] == '.epf':
         path_for_search = file_path.replace('build\\', '')
@@ -169,15 +170,15 @@
         arguments.append('--create_epf')
     if THICK_CLIENT.get():
         arguments.append('--thick')
     if _folder_for_cfe_exist(repo_path):
         arguments.append('--create_cfe')
 
     _save_parameters(repo_path, BASE.get(), PLATFORM.get(), THICK_CLIENT.get())
-    _save_git_path_for_base(BASE.get(), repo_path)
+    _save_parameters_for_acc(BASE.get(), repo_path, PLATFORM.get())
 
     if runner1c.core.main(arguments) == 0:
         destroy_form = True
         if CFE_NAME.get():
             arguments = ['--debug', 'load_extension', '--agent', '--silent', '--path', PLATFORM.get(), '--connection',
                          'File=' + BASE.get(), '--folder', os.path.join(repo_path, 'spec', 'ext'), '--name',
                          extension_name, '--update']
```

### Comparing `runner1c-0.57/runner1c/tools/epf/ChangeSafeModeForExtension/Forms/Form/Ext/Form/Module.bsl` & `runner1c-0.58/runner1c/tools/epf/ChangeSafeModeForExtension/Forms/Form/Ext/Form/Module.bsl`

 * *Files identical despite different names*

### Comparing `runner1c-0.57/runner1c/tools/epf/ChangeSafeModeForExtension/Forms/Form/Ext/Form.xml` & `runner1c-0.58/runner1c/tools/epf/ChangeSafeModeForExtension/Forms/Form/Ext/Form.xml`

 * *Files identical despite different names*

### Comparing `runner1c-0.57/runner1c/tools/epf/ChangeSafeModeForExtension/Forms/Form.xml` & `runner1c-0.58/runner1c/tools/epf/ChangeSafeModeForExtension/Forms/Form.xml`

 * *Files identical despite different names*

### Comparing `runner1c-0.57/runner1c/tools/epf/ChangeSafeModeForExtension.xml` & `runner1c-0.58/runner1c/tools/epf/ChangeSafeModeForExtension.xml`

 * *Files identical despite different names*

### Comparing `runner1c-0.57/runner1c/tools/epf/CloseAfterUpdate/Ext/ObjectModule.bsl` & `runner1c-0.58/runner1c/tools/epf/CloseAfterUpdate/Ext/ObjectModule.bsl`

 * *Files identical despite different names*

### Comparing `runner1c-0.57/runner1c/tools/epf/CloseAfterUpdate/Forms/Managed/Ext/Form/Module.bsl` & `runner1c-0.58/runner1c/tools/epf/CloseAfterUpdate/Forms/Managed/Ext/Form/Module.bsl`

 * *Files identical despite different names*

### Comparing `runner1c-0.57/runner1c/tools/epf/CloseAfterUpdate/Forms/Managed/Ext/Form.xml` & `runner1c-0.58/runner1c/tools/epf/CloseAfterUpdate/Forms/Managed/Ext/Form.xml`

 * *Files identical despite different names*

### Comparing `runner1c-0.57/runner1c/tools/epf/CloseAfterUpdate/Forms/Managed.xml` & `runner1c-0.58/runner1c/tools/epf/CloseAfterUpdate/Forms/Managed.xml`

 * *Files identical despite different names*

### Comparing `runner1c-0.57/runner1c/tools/epf/CloseAfterUpdate/Forms/Ordinary/Ext/Form/Module.bsl` & `runner1c-0.58/runner1c/tools/epf/CloseAfterUpdate/Forms/Ordinary/Ext/Form/Module.bsl`

 * *Files identical despite different names*

### Comparing `runner1c-0.57/runner1c/tools/epf/CloseAfterUpdate/Forms/Ordinary/Ext/Form.bin` & `runner1c-0.58/runner1c/tools/epf/CloseAfterUpdate/Forms/Ordinary/Ext/Form.bin`

 * *Files identical despite different names*

### Comparing `runner1c-0.57/runner1c/tools/epf/CloseAfterUpdate/Forms/Ordinary.xml` & `runner1c-0.58/runner1c/tools/epf/CloseAfterUpdate/Forms/Ordinary.xml`

 * *Files identical despite different names*

### Comparing `runner1c-0.57/runner1c/tools/epf/CloseAfterUpdate.xml` & `runner1c-0.58/runner1c/tools/epf/CloseAfterUpdate.xml`

 * *Files identical despite different names*

### Comparing `runner1c-0.57/runner1c/tools/epf/FileCompareMxl/Forms/Form/Ext/Form/Module.bsl` & `runner1c-0.58/runner1c/tools/epf/FileCompareMxl/Forms/Form/Ext/Form/Module.bsl`

 * *Files identical despite different names*

### Comparing `runner1c-0.57/runner1c/tools/epf/FileCompareMxl/Forms/Form/Ext/Form.bin` & `runner1c-0.58/runner1c/tools/epf/FileCompareMxl/Forms/Form/Ext/Form.bin`

 * *Files identical despite different names*

### Comparing `runner1c-0.57/runner1c/tools/epf/FileCompareMxl/Forms/Form.xml` & `runner1c-0.58/runner1c/tools/epf/FileCompareMxl/Forms/Form.xml`

 * *Files identical despite different names*

### Comparing `runner1c-0.57/runner1c/tools/epf/FileCompareMxl.xml` & `runner1c-0.58/runner1c/tools/epf/FileCompareMxl.xml`

 * *Files identical despite different names*

### Comparing `runner1c-0.57/runner1c/tools/epf/Runner1C/Forms/Form/Ext/Form/Module.bsl` & `runner1c-0.58/runner1c/tools/epf/Runner1C/Forms/Form/Ext/Form/Module.bsl`

 * *Files 11% similar despite different names*

```diff
@@ -1,590 +1,591 @@
-﻿
-// работает в режим совместимости "Версия 8.2.16".
-// отсутствуют все методы на Стр*.
-
-#Область ОписаниеПеременных
-
-&НаКлиенте
-Перем Операции; // Название выполняемой операции.
-
-&НаКлиенте
-Перем ТекстовыйДокумент; // Кэш для показа ошибок.
-
-#КонецОбласти
-
-#Область ОбработчикиСобытий
-
-&НаКлиенте
-Процедура ПриОткрытии(Отказ)
-	
-	ПутьКПлатформе = ПутьКПлатформе();
-	СтрокаПодключенияКБазе = СтрокаСоединенияИнформационнойБазы();
-	Логин = ИмяПользователяНаСервере();
-
-	ЗаполнитьСписокВыбораТипаОперации();
-	ПрочитатьПутьКРепозиторию();
-	
-	Если ПустаяСтрока(ТипОперации) Тогда
-		ТипОперации = Операции.ПолнаяВыгрузкаCF;
-	КонецЕсли;
-	
-	УстановитьВидимостьЭлементов();
-	ВывестиВерсиюПакета();
-	
-КонецПроцедуры
-
-&НаСервере
-Процедура ОбработкаПроверкиЗаполненияНаСервере(Отказ, ПроверяемыеРеквизиты)
-	
-	Если Не ПустаяСтрока(Логин) Тогда
-		ПроверяемыеРеквизиты.Добавить("Пароль");
-	КонецЕсли;
-	
-КонецПроцедуры
-
-#КонецОбласти
-
-#Область ОбработчикиКомандФормы
-
-&НаКлиенте
-Процедура Сделать(Команда)
-	
-	Если Не ПроверитьЗаполнение() Тогда
-		Возврат;
-	КонецЕсли;
-	
-	Оповещение = Новый ОписаниеОповещения("ВыполнитьОперациюСВопросомЗавершение", ЭтаФорма);
-	
-	Если ТипОперации = Операции.СоздатьEPF Тогда
-		ПоказатьВопрос(Новый ОписаниеОповещения("РезультатВопросаПередОперациейСозданияEpf", ЭтаФорма, Оповещение),
-		               "Будут заново созданы файлы. Продолжить?",
-		               РежимДиалогаВопрос.ДаНет,
-		               60,
-		               КодВозвратаДиалога.Нет,
-		               "Внимание",
-		               КодВозвратаДиалога.Нет);
-	Иначе
-		ВыполнитьОбработкуОповещения(Оповещение, Истина);
-	КонецЕсли;
-	
-КонецПроцедуры
-
-#КонецОбласти
-
-#Область ОбработчикиСобытийЭлементовШапкиФормы
-
-&НаКлиенте
-Процедура ПутьКПлатформеНачалоВыбора(Элемент, ДанныеВыбора, СтандартнаяОбработка)
-	НачалоВыбораФайла(Элемент, СтандартнаяОбработка);
-КонецПроцедуры
-
-&НаКлиенте
-Процедура ПапкаВыгрузкиНачалоВыбора(Элемент, ДанныеВыбора, СтандартнаяОбработка)
-	НачалоВыбораФайла(Элемент, СтандартнаяОбработка);
-КонецПроцедуры
-
-&НаКлиенте
-Процедура ТипОперацииПриИзменении(Элемент)
-	УстановитьВидимостьЭлементов();
-КонецПроцедуры
-
-#КонецОбласти
-
-#Область СлужебныйПрограммныйИнтерфейс
-
-&НаКлиенте
-Процедура УстановитьПапкуВыгрузкиПоПутиВФайле(Знач Существует, Знач ДополнительныеПараметры) Экспорт
-	
-	Если Не Существует Тогда
-		Возврат;
-	КонецЕсли;
-	
-	ЧтениеТекста = Новый ЧтениеТекста(ДополнительныеПараметры.ИмяФайла);
-	ПутьКРепозиторию = ЧтениеТекста.ПрочитатьСтроку();
-	ЧтениеТекста.Закрыть();
-	
-	ПапкаВыгрузки = ПутьКРепозиторию;
-	
-КонецПроцедуры
-
-&НаКлиенте
-Процедура УстановитьВыбранныйПуть(Знач ВыбранныеФайлы, Знач ДополнительныеПараметры) Экспорт
-	
-	Если ВыбранныеФайлы = Неопределено Тогда
-		Возврат;
-	КонецЕсли;
-	
-	ЭтаФорма[ДополнительныеПараметры.ИмяЭлемента] = ВыбранныеФайлы[0];
-	
-КонецПроцедуры
-
-&НаКлиенте
-Процедура РезультатВопросаПередОперациейСозданияEpf(Знач РезультатВопроса, Знач ДополнительныеПараметры) Экспорт
-	ВыполнитьОбработкуОповещения(ДополнительныеПараметры, РезультатВопроса = КодВозвратаДиалога.Да);
-КонецПроцедуры
-
-&НаКлиенте
-Процедура ВыполнитьОперациюСВопросомЗавершение(Знач Результат, Знач ДополнительныеПараметры) Экспорт
-	
-	Если Не Результат Тогда
-		Возврат;
-	КонецЕсли;
-	
-	Для Каждого Этап Из ПолучитьЭтапы(ТипОперации) Цикл
-		ПараметрыКоманднойСтроки = РеквизитыФормыВСтруктуру();
-		ПараметрыКоманднойСтроки.Вставить("Команда", Этап.Команда);
-		ЗапуститьКоманду(Этап.СтрокаДляЗапуска, ПараметрыКоманднойСтроки);
-	КонецЦикла;
-	
-КонецПроцедуры
-
-&НаКлиенте
-Процедура ЧтениеЛогаЗавершение(Знач ДополнительныеПараметры) Экспорт
-	ТекстовыйДокумент.Показать("Ошибка при выполнении операции");
-	НачатьУдалениеФайлов(Неопределено, ДополнительныеПараметры.Лог);
-КонецПроцедуры
-
-&НаКлиенте
-Процедура ЗапуститьКомандуЗавершение(Знач КодВозврата, Знач ДополнительныеПараметры) Экспорт
-	
-	Если КодВозврата = 0 Тогда
-		Возврат;
-	КонецЕсли;
-	
-	Файл = Новый Файл(ДополнительныеПараметры.Лог);
-	Файл.НачатьПроверкуСуществования(Новый ОписаниеОповещения("ПроверкаСуществованияЛога",
-	                                                          ЭтаФорма,
-	                                                          ДополнительныеПараметры));
-	
-КонецПроцедуры
-
-&НаКлиенте
-Процедура ПроверкаСуществованияЛога(Знач Существует, Знач ДополнительныеПараметры) Экспорт
-	
-	Если Не Существует Тогда
-		ПоказатьПредупреждение( , "Команда не выполнилась. Лог не найден");
-		Возврат;
-	КонецЕсли;
-	
-	ТекстовыйДокумент = Новый ТекстовыйДокумент;
-	ТекстовыйДокумент.НачатьЧтение(Новый ОписаниеОповещения("ЧтениеЛогаЗавершение",
-	                                                        ЭтаФорма,
-	                                                        Новый Структура("Лог", ДополнительныеПараметры.Лог)),
-	                               ДополнительныеПараметры.Лог,
-	                               КодировкаТекста.UTF8);
-	
-КонецПроцедуры
-
-#КонецОбласти
-
-#Область СлужебныеПроцедурыИФункции
-
-&НаКлиенте
-Функция ПутьКПлатформе()
-	// для linux нужно по другому
-	Возврат СтрЗаменить(КаталогПрограммы(), "\bin\", "");
-КонецФункции
-
-&НаКлиенте
-Процедура ЗапуститьКоманду(Знач СтрокаДляЗапуска, Знач ПараметрыКоманднойСтроки)
-	
-	Команда = ПодставитьПараметрыВСтроку(СтрокаЗапускаСкрипта(Истина, Отладка) + " " + СтрокаДляЗапуска, ПараметрыКоманднойСтроки);
-	
-	Если Отладка Тогда
-		Сообщение(Команда);
-	Иначе
-		Описание = Новый ОписаниеОповещения("ЗапуститьКомандуЗавершение",
-											ЭтаФорма,
-											Новый Структура("Лог", ПараметрыКоманднойСтроки.Лог));
-		НачатьЗапускПриложения(Описание,
-								Команда,
-								,
-								Истина);
-	КонецЕсли;
-	
-КонецПроцедуры
-
-&НаКлиенте
-Функция РеквизитыФормыВСтруктуру()
-	
-	ПапкаВыгрузкиБезСлеша = УбратьСКонцаРазделительПути(ПапкаВыгрузки);
-	ПлатформаБезСлеша = УбратьСКонцаРазделительПути(ПутьКПлатформе);
-	
-	НастройкиВыгрузкиРасширений = Новый Структура("ПапкаВыгрузки, ИмяПапки", ПапкаВыгрузкиБезСлеша, ?(Не ВыгружатьРасширенияВSpec, "lib", "spec"));
-	
-	Структура = Новый Структура;
-	Структура.Вставить("КодРазблокировки",          ?(ПустаяСтрока(КодРазблокировки), "None", КодРазблокировки));
-	Структура.Вставить("Логин",                     Логин);
-	Структура.Вставить("ПапкаВыгрузки",             ПапкаВыгрузкиБезСлеша);
-	Структура.Вставить("ПапкаВыгрузкиКонфигурации", СоединитьПути(ПапкаВыгрузкиБезСлеша, "cf"));
-	Структура.Вставить("ПапкаВыгрузкиРасширений",   ПодставитьПараметрыВСтроку(СоединитьПути("%ПапкаВыгрузки%", "%ИмяПапки%", "ext"), НастройкиВыгрузкиРасширений));
-	Структура.Вставить("Пароль",                    Пароль);
-	Структура.Вставить("ПутьКПлатформе",            ПлатформаБезСлеша);
-	Структура.Вставить("СтрокаПодключенияКБазе",    СтрокаПодключенияКБазе);
-	Структура.Вставить("Лог",                       ПолучитьИмяВременногоФайла("txt"));
-	
-	Возврат Структура;
-	
-КонецФункции
-
-&НаСервереБезКонтекста
-Функция ИмяПользователяНаСервере()
-	Возврат ИмяПользователя();
-КонецФункции
-
-&НаКлиенте
-Процедура ЗаполнитьСписокВыбораТипаОперации()
-	
-	Для Каждого ТипОперции Из Операции Цикл
-		Элементы.ТипОперации.СписокВыбора.Добавить(ТипОперции.Значение);
-	КонецЦикла;
-
-КонецПроцедуры
-
-&НаКлиенте
-Процедура ПрочитатьПутьКРепозиторию()
-	
-	Если Не ИнформационнаяБазаФайловая(СтрокаПодключенияКБазе) Тогда
-		Возврат;
-	КонецЕсли;
-	
-	Структура = ПараметрыИзСтроки(СтрокаПодключенияКБазе);
-	
-	ПутьКФайлуРепозитория = СоединитьПути(Структура.File, "GitPath.txt");
-	
-	Файл = Новый Файл(ПутьКФайлуРепозитория);
-	Файл.НачатьПроверкуСуществования(Новый ОписаниеОповещения("УстановитьПапкуВыгрузкиПоПутиВФайле",
-	                                                          ЭтаФорма,
-	                                                          Новый Структура("ИмяФайла", ПутьКФайлуРепозитория)));
-	
-КонецПроцедуры
-
-&НаКлиенте
-Процедура НачалоВыбораФайла(Знач Элемент, СтандартнаяОбработка)
-	
-	СтандартнаяОбработка = Ложь;
-	
-	ДиалогВыбораФайла = Новый ДиалогВыбораФайла(РежимДиалогаВыбораФайла.ВыборКаталога);
-		
-	Если ЗначениеЗаполнено(Элемент.ТекстРедактирования) Тогда
-		
-		Файл = Новый Файл(Элемент.ТекстРедактирования);
-		ДиалогВыбораФайла.Каталог = Файл.Путь;
-		
-	КонецЕсли;
-	
-	ДиалогВыбораФайла.Показать(Новый ОписаниеОповещения("УстановитьВыбранныйПуть",
-	                                                    ЭтаФорма,
-	                                                    Новый Структура("ИмяЭлемента", Элемент.Имя)));
-	
-КонецПроцедуры
-
-&НаСервереБезКонтекста
-Функция КонфигурацияСОшибкамиВыгрузки()
-	
-	Результат = Ложь;
-	
-	Если Метаданные.РегистрыСведений.Найти("ВерсииПодсистем") <> Неопределено 
-		Или (Метаданные.Имя = "УправлениеТорговлей" И Лев(Метаданные.Версия, 4) = "10.3") Тогда
-		Результат = Истина;
-	КонецЕсли;
-	
-	Возврат Результат;
-	
-КонецФункции
-
-&НаКлиенте
-Функция СтрокаЗапускаСкрипта(Знач ТекущаяБаза = Истина, Знач Отладка = Ложь)
-	
-	Если ПодменитьПутьRunner Тогда
-		ВызватьИсключение "Не реализовано";
-	Иначе
-		Шаблон = "runner1c";
-	КонецЕсли;
-	
-	Если Отладка Тогда
-		Шаблон = Шаблон + " --debug";
-	КонецЕсли;
-	Шаблон = Шаблон + " %Команда%";
-	
-	ПараметрыДляДобавления = Новый Массив;
-	
-	Если ТекущаяБаза Тогда
-		
-		ПараметрыДляДобавления.Добавить(" --log ""%Лог%""");
-		ПараметрыДляДобавления.Добавить("silent");
-		ПараметрыДляДобавления.Добавить("path ""%ПутьКПлатформе%""");
-	
-		Если Не ПустаяСтрока(КодРазблокировки) Тогда
-			ПараметрыДляДобавления.Добавить("access %КодРазблокировки%");
-		КонецЕсли;
-		
-		Если Не ПустаяСтрока(Логин) Тогда
-			ПараметрыДляДобавления.Добавить("login ""%Логин%""");
-			ПараметрыДляДобавления.Добавить("password ""%Пароль%""");
-		КонецЕсли;
-		
-		ПараметрыДляДобавления.Добавить("connection ""%СтрокаПодключенияКБазе%""");
-		
-	КонецЕсли;
-	
-	Возврат Шаблон + СобратьСтрокуИзПодстрок(ПараметрыДляДобавления, " --");
-	
-КонецФункции
-
-&НаКлиенте
-Функция ИнформационнаяБазаФайловая(Знач СтрокаСоединенияИнформационнойБазы = "")
-			
-	Если ПустаяСтрока(СтрокаСоединенияИнформационнойБазы) Тогда
-		СтрокаСоединенияИнформационнойБазы =  СтрокаСоединенияИнформационнойБазы();
-	КонецЕсли;
-	Возврат Найти(Врег(СтрокаСоединенияИнформационнойБазы), "FILE=") = 1;
-	
-КонецФункции
-
-&НаКлиенте
-Функция ПараметрыИзСтроки(Знач СтрокаПараметров)
-	
-	Результат = Новый Структура;
-	
-	СимволДвойныеКавычки = Символ(34); // (")
-	
-	МассивПодстрок = РазложитьСтрокуВМассивПодстрок(СтрокаПараметров, ";");
-	
-	Для Каждого СтрокаПараметра Из МассивПодстрок Цикл
-		
-		ПозицияПервогоЗнакаРавенства = Найти(СтрокаПараметра, "=");
-		
-		// Получаем имя параметра
-		ИмяПараметра = СокрЛП(Лев(СтрокаПараметра, ПозицияПервогоЗнакаРавенства - 1));
-		
-		// Получаем значение параметра.
-		ЗначениеПараметра = СокрЛП(Сред(СтрокаПараметра, ПозицияПервогоЗнакаРавенства + 1));
-		
-		Если  Лев(ЗначениеПараметра, 1) = СимволДвойныеКавычки
-			И Прав(ЗначениеПараметра, 1) = СимволДвойныеКавычки Тогда
-			
-			ЗначениеПараметра = Сред(ЗначениеПараметра, 2, СтрДлина(ЗначениеПараметра) - 2);
-			
-		КонецЕсли;
-		
-		Если Не ПустаяСтрока(ИмяПараметра) Тогда
-			
-			Результат.Вставить(ИмяПараметра, ЗначениеПараметра);
-			
-		КонецЕсли;
-		
-	КонецЦикла;
-	
-	Возврат Результат;
-КонецФункции
-
-&НаКлиенте
-Функция ПодставитьПараметрыВСтроку(Шаблон, Знач ПарметрыСтроки)
-	
-	Строка = Шаблон;
-	Для Каждого Элемент Из ПарметрыСтроки Цикл
-		Строка = СтрЗаменить(Строка, "%" + Элемент.Ключ + "%", Элемент.Значение);
-	КонецЦикла;
-		
-	Возврат Строка;
-	
-КонецФункции
-
-&НаКлиентеНаСервереБезКонтекста
-Процедура Сообщение(Знач Текст)
-	
-	СообщениеПользователю = Новый СообщениеПользователю;
-	СообщениеПользователю.Текст = Текст;
-	СообщениеПользователю.Сообщить();
-	
-КонецПроцедуры
-
-&НаКлиенте
-Функция РазложитьСтрокуВМассивПодстрок(Знач Стр, Разделитель = ",")
-	
-	МассивСтрок = Новый Массив();
-	Если Разделитель = " " Тогда
-		Стр = СокрЛП(Стр);
-		Пока Истина Цикл
-			Поз = Найти(Стр, Разделитель);
-			Если Поз = 0 Тогда
-				МассивСтрок.Добавить(Стр);
-				Возврат МассивСтрок;
-			КонецЕсли;
-			МассивСтрок.Добавить(Лев(Стр, Поз - 1));
-			Стр = СокрЛ(Сред(Стр, Поз));
-		КонецЦикла;
-	Иначе
-		ДлинаРазделителя = СтрДлина(Разделитель);
-		Пока Истина Цикл
-			Поз = Найти(Стр, Разделитель);
-			Если Поз = 0 Тогда
-				МассивСтрок.Добавить(Стр);
-				Возврат МассивСтрок;
-			КонецЕсли;
-			МассивСтрок.Добавить(Лев(Стр, Поз - 1));
-			Стр = Сред(Стр, Поз + ДлинаРазделителя);
-		КонецЦикла;
-	КонецЕсли;
-	
-КонецФункции
-
-&НаКлиенте
-Функция СобратьСтрокуИзПодстрок(Знач Строки, Знач Разделитель)
-	
-	Результат = "";
-	
-	Для Каждого Строка Из Строки Цикл
-		Результат = Результат + ?(ПустаяСтрока(Результат), "", Разделитель) + Строка;
-	КонецЦикла;
-	
-	Возврат Результат;
-	
-КонецФункции
-
-&НаКлиенте
-Процедура УстановитьВидимостьЭлементов()
-	Элементы.ВыгружатьРасширенияВSpec.Видимость = (ТипОперации = Операции.ВыгрузкаCFE);
-КонецПроцедуры
-
-&НаСервере
-Функция ИмяФайлаОбработки()
-	Возврат РеквизитФормыВЗначение("Объект").ИспользуемоеИмяФайла;
-КонецФункции
-
-&НаКлиенте
-Процедура ВывестиВерсиюПакета()
-	
-	ЧтениеТекста = Новый ЧтениеТекста(ПутьДоRunner() + РазделительПути() + "__init__.py");
-	СтрокаВерсии = ЧтениеТекста.ПрочитатьСтроку();
-	ЧтениеТекста.Закрыть();
-	
-	ПараметрыВерсии = РазложитьСтрокуВМассивПодстрок(СтрокаВерсии, "=");
-	Версия = СокрЛП(ПараметрыВерсии[1]);
-	
-	Заголовок = Версия;
-	
-КонецПроцедуры
-
-&НаКлиенте
-Функция РазделительПути()
-	Возврат "\";
-КонецФункции
-
-&НаКлиенте
-Функция СоединитьПути(Знач ПутьКаталога, Знач Элемент1, Знач Элемент2 = "")
-	
-	Массив = Новый Массив;
-	Массив.Добавить(ПутьКаталога);
-	Массив.Добавить(Элемент1);
-	Если Не ПустаяСтрока(Элемент2) Тогда
-		Массив.Добавить(Элемент2);
-	КонецЕсли;
-	
-	Возврат СобратьСтрокуИзПодстрок(Массив, РазделительПути());
-	
-КонецФункции
-
-&НаКлиенте
-Функция УбратьСКонцаРазделительПути(Знач Путь)
-	
-	Результат = Путь;
-	Если Прав(Путь, 1) = РазделительПути() Тогда
-		Результат = Лев(Результат, СтрДлина(Результат) - 1);
-	КонецЕсли;
-	
-	Возврат Результат;
-	
-КонецФункции
-
-&НаКлиенте
-Функция ПолучитьЭтапы(Знач ВыбраннаяОперация)
-	
-	Массив = Новый Массив();
-	
-	СтрокаДляЗапуска = "";
-	
-	Если ВыбраннаяОперация = Операции.ПолнаяВыгрузкаCF Или ВыбраннаяОперация = Операции.ЧастичнаяВыгрузкаCF Тогда
-		
-		СтрокаДляЗапуска = "--folder ""%ПапкаВыгрузкиКонфигурации%""";
-		Если КонфигурацияСОшибкамиВыгрузки() Тогда
-			СтрокаДляЗапуска = СтрокаДляЗапуска + " --repair";
-		КонецЕсли;
-		Если ВыбраннаяОперация = Операции.ЧастичнаяВыгрузкаCF Тогда
-			СтрокаДляЗапуска = СтрокаДляЗапуска + " --update";
-		КонецЕсли;
-		
-		Массив.Добавить(СоздатьЭтап(СтрокаДляЗапуска, "dump_config"));
-		
-	ИначеЕсли ВыбраннаяОперация = Операции.ВыгрузкаCFE Тогда
-		
-		СтрокаДляЗапуска = "--folder ""%ПапкаВыгрузкиРасширений%""";
-		Массив.Добавить(СоздатьЭтап(СтрокаДляЗапуска, "dump_extensions"));
-		
-	ИначеЕсли ВыбраннаяОперация = Операции.ПолнаяВыгрузкаEPF Или ВыбраннаяОперация = Операции.ЧастичнаяВыгрузкаEPF Тогда
-		
-		СтрокаДляЗапуска = "--folder ""%ПапкаВыгрузки%""";
-		Если ВыбраннаяОперация = Операции.ПолнаяВыгрузкаEPF Тогда
-			СтрокаДляЗапуска = СтрокаДляЗапуска + " --clear_hash";
-		КонецЕсли;
-		
-		Массив.Добавить(СоздатьЭтап(СтрокаДляЗапуска, "sync"));
-		
-	ИначеЕсли ВыбраннаяОперация = Операции.СоздатьEPF Тогда
-		
-		СтрокаДляЗапуска = "--folder ""%ПапкаВыгрузки%"" --create";
-		Массив.Добавить(СоздатьЭтап(СтрокаДляЗапуска, "sync"));
-		
-	ИначеЕсли ВыбраннаяОперация = Операции.ЗагрузитьCF Тогда
-		
-		СтрокаДляЗапуска = "--folder ""%ПапкаВыгрузкиКонфигурации%""";
-		Массив.Добавить(СоздатьЭтап(СтрокаДляЗапуска, "load_config"));
-		
-		СтрокаДляЗапуска = "--folder ""%ПапкаВыгрузкиРасширений%""";
-		Массив.Добавить(СоздатьЭтап(СтрокаДляЗапуска, "load_extension"));
-		
-	Иначе
-		ВызватьИсключение "операция не определена";
-	КонецЕсли;
-	
-	Возврат Массив;
-	
-КонецФункции
-
-&НаКлиенте
-Функция ПутьДоRunner()
-	
-	Разделитель = РазделительПути();
-	
-	ПутьОбработки = РазложитьСтрокуВМассивПодстрок(ИмяФайлаОбработки(), Разделитель);
-	ПутьОбработки.Удалить(ПутьОбработки.Количество() - 1);
-	ПутьОбработки.Удалить(ПутьОбработки.Количество() - 1);
-	ПутьОбработки.Удалить(ПутьОбработки.Количество() - 1);
-	ПутьОбработки.Удалить(ПутьОбработки.Количество() - 1);
-	
-	ПутьВерсии = СобратьСтрокуИзПодстрок(ПутьОбработки, Разделитель);
-	
-	Возврат ПутьВерсии;
-	
-КонецФункции
-
-&НаКлиенте
-Функция СоздатьЭтап(Знач СтрокаДляЗапуска, Знач Команда)
-	Возврат Новый Структура("СтрокаДляЗапуска, Команда", СтрокаДляЗапуска, Команда);
-КонецФункции
-
-#КонецОбласти
-
-#Область Инициализация
-
-Операции = Новый Структура;
-Операции.Вставить("ПолнаяВыгрузкаCF", "CF Полная Выгрузка");
-Операции.Вставить("ЧастичнаяВыгрузкаCF", "CF Частичная Выгрузка");
-Операции.Вставить("ПолнаяВыгрузкаEPF", "EPF Полная Выгрузка");
-Операции.Вставить("ЧастичнаяВыгрузкаEPF", "EPF Частичная Выгрузка");
-Операции.Вставить("СоздатьEPF", "EPF Создать");
-Операции.Вставить("ВыгрузкаCFE", "CFE Выгрузка");
-Операции.Вставить("ЗагрузитьCF", "Загрузить конфигурацию");
-
-#КонецОбласти
+﻿
+// работает в режим совместимости "Версия 8.2.16".
+// отсутствуют все методы на Стр*.
+
+#Область ОписаниеПеременных
+
+&НаКлиенте
+Перем Операции; // Название выполняемой операции.
+
+&НаКлиенте
+Перем ТекстовыйДокумент; // Кэш для показа ошибок.
+
+#КонецОбласти
+
+#Область ОбработчикиСобытий
+
+&НаКлиенте
+Процедура ПриОткрытии(Отказ)
+	
+	ПутьКПлатформе = ПутьКПлатформе();
+	СтрокаПодключенияКБазе = СтрокаСоединенияИнформационнойБазы();
+	Логин = ИмяПользователяНаСервере();
+
+	ЗаполнитьСписокВыбораТипаОперации();
+	ПрочитатьПутьКРепозиторию();
+	
+	Если ПустаяСтрока(ТипОперации) Тогда
+		ТипОперации = Операции.ПолнаяВыгрузкаCF;
+	КонецЕсли;
+	
+	УстановитьВидимостьЭлементов();
+	ВывестиВерсиюПакета();
+	
+КонецПроцедуры
+
+&НаСервере
+Процедура ОбработкаПроверкиЗаполненияНаСервере(Отказ, ПроверяемыеРеквизиты)
+	
+	Если Не ПустаяСтрока(Логин) Тогда
+		ПроверяемыеРеквизиты.Добавить("Пароль");
+	КонецЕсли;
+	
+КонецПроцедуры
+
+#КонецОбласти
+
+#Область ОбработчикиКомандФормы
+
+&НаКлиенте
+Процедура Сделать(Команда)
+	
+	Если Не ПроверитьЗаполнение() Тогда
+		Возврат;
+	КонецЕсли;
+	
+	Оповещение = Новый ОписаниеОповещения("ВыполнитьОперациюСВопросомЗавершение", ЭтаФорма);
+	
+	Если ТипОперации = Операции.СоздатьEPF Тогда
+		ПоказатьВопрос(Новый ОписаниеОповещения("РезультатВопросаПередОперациейСозданияEpf", ЭтаФорма, Оповещение),
+		               "Будут заново созданы файлы. Продолжить?",
+		               РежимДиалогаВопрос.ДаНет,
+		               60,
+		               КодВозвратаДиалога.Нет,
+		               "Внимание",
+		               КодВозвратаДиалога.Нет);
+	Иначе
+		ВыполнитьОбработкуОповещения(Оповещение, Истина);
+	КонецЕсли;
+	
+КонецПроцедуры
+
+#КонецОбласти
+
+#Область ОбработчикиСобытийЭлементовШапкиФормы
+
+&НаКлиенте
+Процедура ПутьКПлатформеНачалоВыбора(Элемент, ДанныеВыбора, СтандартнаяОбработка)
+	НачалоВыбораФайла(Элемент, СтандартнаяОбработка);
+КонецПроцедуры
+
+&НаКлиенте
+Процедура ПапкаВыгрузкиНачалоВыбора(Элемент, ДанныеВыбора, СтандартнаяОбработка)
+	НачалоВыбораФайла(Элемент, СтандартнаяОбработка);
+КонецПроцедуры
+
+&НаКлиенте
+Процедура ТипОперацииПриИзменении(Элемент)
+	УстановитьВидимостьЭлементов();
+КонецПроцедуры
+
+#КонецОбласти
+
+#Область СлужебныйПрограммныйИнтерфейс
+
+&НаКлиенте
+Процедура УстановитьПапкуВыгрузкиПоПутиВФайле(Знач Существует, Знач ДополнительныеПараметры) Экспорт
+	
+	Если Не Существует Тогда
+		Возврат;
+	КонецЕсли;
+	
+	ЧтениеJSON = Новый ЧтениеJSON();
+	ЧтениеJSON.ОткрытьФайл(ДополнительныеПараметры.ИмяФайла);
+	ПараметрыИзФайла = ПрочитатьJSON(ЧтениеJSON);
+	ЧтениеJSON.Закрыть();
+	
+	ПапкаВыгрузки = ПараметрыИзФайла.repo;
+	
+КонецПроцедуры
+
+&НаКлиенте
+Процедура УстановитьВыбранныйПуть(Знач ВыбранныеФайлы, Знач ДополнительныеПараметры) Экспорт
+	
+	Если ВыбранныеФайлы = Неопределено Тогда
+		Возврат;
+	КонецЕсли;
+	
+	ЭтаФорма[ДополнительныеПараметры.ИмяЭлемента] = ВыбранныеФайлы[0];
+	
+КонецПроцедуры
+
+&НаКлиенте
+Процедура РезультатВопросаПередОперациейСозданияEpf(Знач РезультатВопроса, Знач ДополнительныеПараметры) Экспорт
+	ВыполнитьОбработкуОповещения(ДополнительныеПараметры, РезультатВопроса = КодВозвратаДиалога.Да);
+КонецПроцедуры
+
+&НаКлиенте
+Процедура ВыполнитьОперациюСВопросомЗавершение(Знач Результат, Знач ДополнительныеПараметры) Экспорт
+	
+	Если Не Результат Тогда
+		Возврат;
+	КонецЕсли;
+	
+	Для Каждого Этап Из ПолучитьЭтапы(ТипОперации) Цикл
+		ПараметрыКоманднойСтроки = РеквизитыФормыВСтруктуру();
+		ПараметрыКоманднойСтроки.Вставить("Команда", Этап.Команда);
+		ЗапуститьКоманду(Этап.СтрокаДляЗапуска, ПараметрыКоманднойСтроки);
+	КонецЦикла;
+	
+КонецПроцедуры
+
+&НаКлиенте
+Процедура ЧтениеЛогаЗавершение(Знач ДополнительныеПараметры) Экспорт
+	ТекстовыйДокумент.Показать("Ошибка при выполнении операции");
+	НачатьУдалениеФайлов(Неопределено, ДополнительныеПараметры.Лог);
+КонецПроцедуры
+
+&НаКлиенте
+Процедура ЗапуститьКомандуЗавершение(Знач КодВозврата, Знач ДополнительныеПараметры) Экспорт
+	
+	Если КодВозврата = 0 Тогда
+		Возврат;
+	КонецЕсли;
+	
+	Файл = Новый Файл(ДополнительныеПараметры.Лог);
+	Файл.НачатьПроверкуСуществования(Новый ОписаниеОповещения("ПроверкаСуществованияЛога",
+	                                                          ЭтаФорма,
+	                                                          ДополнительныеПараметры));
+	
+КонецПроцедуры
+
+&НаКлиенте
+Процедура ПроверкаСуществованияЛога(Знач Существует, Знач ДополнительныеПараметры) Экспорт
+	
+	Если Не Существует Тогда
+		ПоказатьПредупреждение( , "Команда не выполнилась. Лог не найден");
+		Возврат;
+	КонецЕсли;
+	
+	ТекстовыйДокумент = Новый ТекстовыйДокумент;
+	ТекстовыйДокумент.НачатьЧтение(Новый ОписаниеОповещения("ЧтениеЛогаЗавершение",
+	                                                        ЭтаФорма,
+	                                                        Новый Структура("Лог", ДополнительныеПараметры.Лог)),
+	                               ДополнительныеПараметры.Лог,
+	                               КодировкаТекста.UTF8);
+	
+КонецПроцедуры
+
+#КонецОбласти
+
+#Область СлужебныеПроцедурыИФункции
+
+&НаКлиенте
+Функция ПутьКПлатформе()
+	// для linux нужно по другому
+	Возврат СтрЗаменить(КаталогПрограммы(), "\bin\", "");
+КонецФункции
+
+&НаКлиенте
+Процедура ЗапуститьКоманду(Знач СтрокаДляЗапуска, Знач ПараметрыКоманднойСтроки)
+	
+	Команда = ПодставитьПараметрыВСтроку(СтрокаЗапускаСкрипта(Истина, Отладка) + " " + СтрокаДляЗапуска, ПараметрыКоманднойСтроки);
+	
+	Если Отладка Тогда
+		Сообщение(Команда);
+	Иначе
+		Описание = Новый ОписаниеОповещения("ЗапуститьКомандуЗавершение",
+											ЭтаФорма,
+											Новый Структура("Лог", ПараметрыКоманднойСтроки.Лог));
+		НачатьЗапускПриложения(Описание,
+								Команда,
+								,
+								Истина);
+	КонецЕсли;
+	
+КонецПроцедуры
+
+&НаКлиенте
+Функция РеквизитыФормыВСтруктуру()
+	
+	ПапкаВыгрузкиБезСлеша = УбратьСКонцаРазделительПути(ПапкаВыгрузки);
+	ПлатформаБезСлеша = УбратьСКонцаРазделительПути(ПутьКПлатформе);
+	
+	НастройкиВыгрузкиРасширений = Новый Структура("ПапкаВыгрузки, ИмяПапки", ПапкаВыгрузкиБезСлеша, ?(Не ВыгружатьРасширенияВSpec, "lib", "spec"));
+	
+	Структура = Новый Структура;
+	Структура.Вставить("КодРазблокировки",          ?(ПустаяСтрока(КодРазблокировки), "None", КодРазблокировки));
+	Структура.Вставить("Логин",                     Логин);
+	Структура.Вставить("ПапкаВыгрузки",             ПапкаВыгрузкиБезСлеша);
+	Структура.Вставить("ПапкаВыгрузкиКонфигурации", СоединитьПути(ПапкаВыгрузкиБезСлеша, "cf"));
+	Структура.Вставить("ПапкаВыгрузкиРасширений",   ПодставитьПараметрыВСтроку(СоединитьПути("%ПапкаВыгрузки%", "%ИмяПапки%", "ext"), НастройкиВыгрузкиРасширений));
+	Структура.Вставить("Пароль",                    Пароль);
+	Структура.Вставить("ПутьКПлатформе",            ПлатформаБезСлеша);
+	Структура.Вставить("СтрокаПодключенияКБазе",    СтрокаПодключенияКБазе);
+	Структура.Вставить("Лог",                       ПолучитьИмяВременногоФайла("txt"));
+	
+	Возврат Структура;
+	
+КонецФункции
+
+&НаСервереБезКонтекста
+Функция ИмяПользователяНаСервере()
+	Возврат ИмяПользователя();
+КонецФункции
+
+&НаКлиенте
+Процедура ЗаполнитьСписокВыбораТипаОперации()
+	
+	Для Каждого ТипОперции Из Операции Цикл
+		Элементы.ТипОперации.СписокВыбора.Добавить(ТипОперции.Значение);
+	КонецЦикла;
+
+КонецПроцедуры
+
+&НаКлиенте
+Процедура ПрочитатьПутьКРепозиторию()
+	
+	Если Не ИнформационнаяБазаФайловая(СтрокаПодключенияКБазе) Тогда
+		Возврат;
+	КонецЕсли;
+	
+	Структура = ПараметрыИзСтроки(СтрокаПодключенияКБазе);
+	
+	ПутьКФайлуСПараметрамиБазы = СоединитьПути(Структура.File, "parameters.txt");
+	
+	Файл = Новый Файл(ПутьКФайлуСПараметрамиБазы);
+	Файл.НачатьПроверкуСуществования(Новый ОписаниеОповещения("УстановитьПапкуВыгрузкиПоПутиВФайле",
+	                                                          ЭтаФорма,
+	                                                          Новый Структура("ИмяФайла", ПутьКФайлуСПараметрамиБазы)));
+	
+КонецПроцедуры
+
+&НаКлиенте
+Процедура НачалоВыбораФайла(Знач Элемент, СтандартнаяОбработка)
+	
+	СтандартнаяОбработка = Ложь;
+	
+	ДиалогВыбораФайла = Новый ДиалогВыбораФайла(РежимДиалогаВыбораФайла.ВыборКаталога);
+		
+	Если ЗначениеЗаполнено(Элемент.ТекстРедактирования) Тогда
+		
+		Файл = Новый Файл(Элемент.ТекстРедактирования);
+		ДиалогВыбораФайла.Каталог = Файл.Путь;
+		
+	КонецЕсли;
+	
+	ДиалогВыбораФайла.Показать(Новый ОписаниеОповещения("УстановитьВыбранныйПуть",
+	                                                    ЭтаФорма,
+	                                                    Новый Структура("ИмяЭлемента", Элемент.Имя)));
+	
+КонецПроцедуры
+
+&НаСервереБезКонтекста
+Функция КонфигурацияСОшибкамиВыгрузки()
+	
+	Результат = Ложь;
+	
+	Если Метаданные.РегистрыСведений.Найти("ВерсииПодсистем") <> Неопределено 
+		Или (Метаданные.Имя = "УправлениеТорговлей" И Лев(Метаданные.Версия, 4) = "10.3") Тогда
+		Результат = Истина;
+	КонецЕсли;
+	
+	Возврат Результат;
+	
+КонецФункции
+
+&НаКлиенте
+Функция СтрокаЗапускаСкрипта(Знач ТекущаяБаза = Истина, Знач Отладка = Ложь)
+	
+	Если ПодменитьПутьRunner Тогда
+		ВызватьИсключение "Не реализовано";
+	Иначе
+		Шаблон = "runner1c";
+	КонецЕсли;
+	
+	Если Отладка Тогда
+		Шаблон = Шаблон + " --debug";
+	КонецЕсли;
+	Шаблон = Шаблон + " %Команда%";
+	
+	ПараметрыДляДобавления = Новый Массив;
+	
+	Если ТекущаяБаза Тогда
+		
+		ПараметрыДляДобавления.Добавить(" --log ""%Лог%""");
+		ПараметрыДляДобавления.Добавить("silent");
+		ПараметрыДляДобавления.Добавить("path ""%ПутьКПлатформе%""");
+	
+		Если Не ПустаяСтрока(КодРазблокировки) Тогда
+			ПараметрыДляДобавления.Добавить("access %КодРазблокировки%");
+		КонецЕсли;
+		
+		Если Не ПустаяСтрока(Логин) Тогда
+			ПараметрыДляДобавления.Добавить("login ""%Логин%""");
+			ПараметрыДляДобавления.Добавить("password ""%Пароль%""");
+		КонецЕсли;
+		
+		ПараметрыДляДобавления.Добавить("connection ""%СтрокаПодключенияКБазе%""");
+		
+	КонецЕсли;
+	
+	Возврат Шаблон + СобратьСтрокуИзПодстрок(ПараметрыДляДобавления, " --");
+	
+КонецФункции
+
+&НаКлиенте
+Функция ИнформационнаяБазаФайловая(Знач СтрокаСоединенияИнформационнойБазы = "")
+			
+	Если ПустаяСтрока(СтрокаСоединенияИнформационнойБазы) Тогда
+		СтрокаСоединенияИнформационнойБазы =  СтрокаСоединенияИнформационнойБазы();
+	КонецЕсли;
+	Возврат Найти(Врег(СтрокаСоединенияИнформационнойБазы), "FILE=") = 1;
+	
+КонецФункции
+
+&НаКлиенте
+Функция ПараметрыИзСтроки(Знач СтрокаПараметров)
+	
+	Результат = Новый Структура;
+	
+	СимволДвойныеКавычки = Символ(34); // (")
+	
+	МассивПодстрок = РазложитьСтрокуВМассивПодстрок(СтрокаПараметров, ";");
+	
+	Для Каждого СтрокаПараметра Из МассивПодстрок Цикл
+		
+		ПозицияПервогоЗнакаРавенства = Найти(СтрокаПараметра, "=");
+		
+		// Получаем имя параметра
+		ИмяПараметра = СокрЛП(Лев(СтрокаПараметра, ПозицияПервогоЗнакаРавенства - 1));
+		
+		// Получаем значение параметра.
+		ЗначениеПараметра = СокрЛП(Сред(СтрокаПараметра, ПозицияПервогоЗнакаРавенства + 1));
+		
+		Если  Лев(ЗначениеПараметра, 1) = СимволДвойныеКавычки
+			И Прав(ЗначениеПараметра, 1) = СимволДвойныеКавычки Тогда
+			
+			ЗначениеПараметра = Сред(ЗначениеПараметра, 2, СтрДлина(ЗначениеПараметра) - 2);
+			
+		КонецЕсли;
+		
+		Если Не ПустаяСтрока(ИмяПараметра) Тогда
+			
+			Результат.Вставить(ИмяПараметра, ЗначениеПараметра);
+			
+		КонецЕсли;
+		
+	КонецЦикла;
+	
+	Возврат Результат;
+КонецФункции
+
+&НаКлиенте
+Функция ПодставитьПараметрыВСтроку(Шаблон, Знач ПарметрыСтроки)
+	
+	Строка = Шаблон;
+	Для Каждого Элемент Из ПарметрыСтроки Цикл
+		Строка = СтрЗаменить(Строка, "%" + Элемент.Ключ + "%", Элемент.Значение);
+	КонецЦикла;
+		
+	Возврат Строка;
+	
+КонецФункции
+
+&НаКлиентеНаСервереБезКонтекста
+Процедура Сообщение(Знач Текст)
+	
+	СообщениеПользователю = Новый СообщениеПользователю;
+	СообщениеПользователю.Текст = Текст;
+	СообщениеПользователю.Сообщить();
+	
+КонецПроцедуры
+
+&НаКлиенте
+Функция РазложитьСтрокуВМассивПодстрок(Знач Стр, Разделитель = ",")
+	
+	МассивСтрок = Новый Массив();
+	Если Разделитель = " " Тогда
+		Стр = СокрЛП(Стр);
+		Пока Истина Цикл
+			Поз = Найти(Стр, Разделитель);
+			Если Поз = 0 Тогда
+				МассивСтрок.Добавить(Стр);
+				Возврат МассивСтрок;
+			КонецЕсли;
+			МассивСтрок.Добавить(Лев(Стр, Поз - 1));
+			Стр = СокрЛ(Сред(Стр, Поз));
+		КонецЦикла;
+	Иначе
+		ДлинаРазделителя = СтрДлина(Разделитель);
+		Пока Истина Цикл
+			Поз = Найти(Стр, Разделитель);
+			Если Поз = 0 Тогда
+				МассивСтрок.Добавить(Стр);
+				Возврат МассивСтрок;
+			КонецЕсли;
+			МассивСтрок.Добавить(Лев(Стр, Поз - 1));
+			Стр = Сред(Стр, Поз + ДлинаРазделителя);
+		КонецЦикла;
+	КонецЕсли;
+	
+КонецФункции
+
+&НаКлиенте
+Функция СобратьСтрокуИзПодстрок(Знач Строки, Знач Разделитель)
+	
+	Результат = "";
+	
+	Для Каждого Строка Из Строки Цикл
+		Результат = Результат + ?(ПустаяСтрока(Результат), "", Разделитель) + Строка;
+	КонецЦикла;
+	
+	Возврат Результат;
+	
+КонецФункции
+
+&НаКлиенте
+Процедура УстановитьВидимостьЭлементов()
+	Элементы.ВыгружатьРасширенияВSpec.Видимость = (ТипОперации = Операции.ВыгрузкаCFE);
+КонецПроцедуры
+
+&НаСервере
+Функция ИмяФайлаОбработки()
+	Возврат РеквизитФормыВЗначение("Объект").ИспользуемоеИмяФайла;
+КонецФункции
+
+&НаКлиенте
+Процедура ВывестиВерсиюПакета()
+	
+	ЧтениеТекста = Новый ЧтениеТекста(ПутьДоRunner() + РазделительПути() + "__init__.py");
+	СтрокаВерсии = ЧтениеТекста.ПрочитатьСтроку();
+	ЧтениеТекста.Закрыть();
+	
+	ПараметрыВерсии = РазложитьСтрокуВМассивПодстрок(СтрокаВерсии, "=");
+	Версия = СокрЛП(ПараметрыВерсии[1]);
+	
+	Заголовок = Версия;
+	
+КонецПроцедуры
+
+&НаКлиенте
+Функция РазделительПути()
+	Возврат "\";
+КонецФункции
+
+&НаКлиенте
+Функция СоединитьПути(Знач ПутьКаталога, Знач Элемент1, Знач Элемент2 = "")
+	
+	Массив = Новый Массив;
+	Массив.Добавить(ПутьКаталога);
+	Массив.Добавить(Элемент1);
+	Если Не ПустаяСтрока(Элемент2) Тогда
+		Массив.Добавить(Элемент2);
+	КонецЕсли;
+	
+	Возврат СобратьСтрокуИзПодстрок(Массив, РазделительПути());
+	
+КонецФункции
+
+&НаКлиенте
+Функция УбратьСКонцаРазделительПути(Знач Путь)
+	
+	Результат = Путь;
+	Если Прав(Путь, 1) = РазделительПути() Тогда
+		Результат = Лев(Результат, СтрДлина(Результат) - 1);
+	КонецЕсли;
+	
+	Возврат Результат;
+	
+КонецФункции
+
+&НаКлиенте
+Функция ПолучитьЭтапы(Знач ВыбраннаяОперация)
+	
+	Массив = Новый Массив();
+	
+	СтрокаДляЗапуска = "";
+	
+	Если ВыбраннаяОперация = Операции.ПолнаяВыгрузкаCF Или ВыбраннаяОперация = Операции.ЧастичнаяВыгрузкаCF Тогда
+		
+		СтрокаДляЗапуска = "--folder ""%ПапкаВыгрузкиКонфигурации%""";
+		Если КонфигурацияСОшибкамиВыгрузки() Тогда
+			СтрокаДляЗапуска = СтрокаДляЗапуска + " --repair";
+		КонецЕсли;
+		Если ВыбраннаяОперация = Операции.ЧастичнаяВыгрузкаCF Тогда
+			СтрокаДляЗапуска = СтрокаДляЗапуска + " --update";
+		КонецЕсли;
+		
+		Массив.Добавить(СоздатьЭтап(СтрокаДляЗапуска, "dump_config"));
+		
+	ИначеЕсли ВыбраннаяОперация = Операции.ВыгрузкаCFE Тогда
+		
+		СтрокаДляЗапуска = "--folder ""%ПапкаВыгрузкиРасширений%""";
+		Массив.Добавить(СоздатьЭтап(СтрокаДляЗапуска, "dump_extensions"));
+		
+	ИначеЕсли ВыбраннаяОперация = Операции.ПолнаяВыгрузкаEPF Или ВыбраннаяОперация = Операции.ЧастичнаяВыгрузкаEPF Тогда
+		
+		СтрокаДляЗапуска = "--folder ""%ПапкаВыгрузки%""";
+		Если ВыбраннаяОперация = Операции.ПолнаяВыгрузкаEPF Тогда
+			СтрокаДляЗапуска = СтрокаДляЗапуска + " --clear_hash";
+		КонецЕсли;
+		
+		Массив.Добавить(СоздатьЭтап(СтрокаДляЗапуска, "sync"));
+		
+	ИначеЕсли ВыбраннаяОперация = Операции.СоздатьEPF Тогда
+		
+		СтрокаДляЗапуска = "--folder ""%ПапкаВыгрузки%"" --create";
+		Массив.Добавить(СоздатьЭтап(СтрокаДляЗапуска, "sync"));
+		
+	ИначеЕсли ВыбраннаяОперация = Операции.ЗагрузитьCF Тогда
+		
+		СтрокаДляЗапуска = "--folder ""%ПапкаВыгрузкиКонфигурации%""";
+		Массив.Добавить(СоздатьЭтап(СтрокаДляЗапуска, "load_config"));
+		
+		СтрокаДляЗапуска = "--folder ""%ПапкаВыгрузкиРасширений%""";
+		Массив.Добавить(СоздатьЭтап(СтрокаДляЗапуска, "load_extension"));
+		
+	Иначе
+		ВызватьИсключение "операция не определена";
+	КонецЕсли;
+	
+	Возврат Массив;
+	
+КонецФункции
+
+&НаКлиенте
+Функция ПутьДоRunner()
+	
+	Разделитель = РазделительПути();
+	
+	ПутьОбработки = РазложитьСтрокуВМассивПодстрок(ИмяФайлаОбработки(), Разделитель);
+	ПутьОбработки.Удалить(ПутьОбработки.Количество() - 1);
+	ПутьОбработки.Удалить(ПутьОбработки.Количество() - 1);
+	ПутьОбработки.Удалить(ПутьОбработки.Количество() - 1);
+	ПутьОбработки.Удалить(ПутьОбработки.Количество() - 1);
+	
+	ПутьВерсии = СобратьСтрокуИзПодстрок(ПутьОбработки, Разделитель);
+	
+	Возврат ПутьВерсии;
+	
+КонецФункции
+
+&НаКлиенте
+Функция СоздатьЭтап(Знач СтрокаДляЗапуска, Знач Команда)
+	Возврат Новый Структура("СтрокаДляЗапуска, Команда", СтрокаДляЗапуска, Команда);
+КонецФункции
+
+#КонецОбласти
+
+#Область Инициализация
+
+Операции = Новый Структура;
+Операции.Вставить("ПолнаяВыгрузкаCF", "CF Полная Выгрузка");
+Операции.Вставить("ЧастичнаяВыгрузкаCF", "CF Частичная Выгрузка");
+Операции.Вставить("ПолнаяВыгрузкаEPF", "EPF Полная Выгрузка");
+Операции.Вставить("ЧастичнаяВыгрузкаEPF", "EPF Частичная Выгрузка");
+Операции.Вставить("СоздатьEPF", "EPF Создать");
+Операции.Вставить("ВыгрузкаCFE", "CFE Выгрузка");
+Операции.Вставить("ЗагрузитьCF", "Загрузить конфигурацию");
+
+#КонецОбласти
```

### Comparing `runner1c-0.57/runner1c/tools/epf/Runner1C/Forms/Form/Ext/Form.xml` & `runner1c-0.58/runner1c/tools/epf/Runner1C/Forms/Form/Ext/Form.xml`

 * *Files 23% similar despite different names*

#### Comparing `runner1c-0.57/runner1c/tools/epf/Runner1C/Forms/Form/Ext/Form.xml` & `runner1c-0.58/runner1c/tools/epf/Runner1C/Forms/Form/Ext/Form.xml`

```diff
@@ -82,14 +82,15 @@
     <UsualGroup name="Группа" id="44">
       <Representation>None</Representation>
       <ShowTitle>false</ShowTitle>
       <ExtendedTooltip name="ГруппаРасширеннаяПодсказка" id="45"/>
       <ChildItems>
         <CheckBoxField name="ПодменитьПутьRunner" id="41">
           <DataPath>ПодменитьПутьRunner</DataPath>
+          <Enabled>false</Enabled>
           <CheckBoxType>Auto</CheckBoxType>
           <ContextMenu name="ПодменитьПутьRunnerКонтекстноеМеню" id="42"/>
           <ExtendedTooltip name="ПодменитьПутьRunnerРасширеннаяПодсказка" id="43"/>
         </CheckBoxField>
         <CheckBoxField name="Отладка" id="15">
           <DataPath>Отладка</DataPath>
           <CheckBoxType>Auto</CheckBoxType>
```

### Comparing `runner1c-0.57/runner1c/tools/epf/Runner1C/Forms/Form.xml` & `runner1c-0.58/runner1c/tools/epf/Runner1C/Forms/Form.xml`

 * *Files identical despite different names*

### Comparing `runner1c-0.57/runner1c/tools/epf/Runner1C.xml` & `runner1c-0.58/runner1c/tools/epf/Runner1C.xml`

 * *Files identical despite different names*

### Comparing `runner1c-0.57/runner1c.egg-info/SOURCES.txt` & `runner1c-0.58/runner1c.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 runner1c.egg-info/PKG-INFO
 runner1c.egg-info/SOURCES.txt
 runner1c.egg-info/dependency_links.txt
 runner1c.egg-info/entry_points.txt
 runner1c.egg-info/requires.txt
 runner1c.egg-info/top_level.txt
 runner1c/build/README.md
+runner1c/build/tests/repo/epf/CheckConfig.epf
 runner1c/build/tools/epf/ChangeSafeModeForExtension.epf
 runner1c/build/tools/epf/CloseAfterUpdate.epf
 runner1c/build/tools/epf/FileCompareMxl.epf
 runner1c/build/tools/epf/Runner1C.epf
 runner1c/commands/__init__.py
 runner1c/commands/base_for_test.py
 runner1c/commands/create_base.py
```

### Comparing `runner1c-0.57/setup.py` & `runner1c-0.58/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -18,13 +18,10 @@
     platforms='win32',
     entry_points={
         'console_scripts': [
             'runner1c = runner1c.core:main',
         ],
     },
     install_requires=[
-        'paramiko>=2.4',
-        'pytest>=3.4',
-        'pytest-cov>=2.5',
-        'pytest-dependency>=0.3.2'
+        'paramiko>=2.4'
     ]
 )
```

