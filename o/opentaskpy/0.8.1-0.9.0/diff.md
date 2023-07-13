# Comparing `tmp/opentaskpy-0.8.1.tar.gz` & `tmp/opentaskpy-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opentaskpy-0.8.1.tar", last modified: Mon Apr 17 16:02:47 2023, max compression
+gzip compressed data, was "opentaskpy-0.9.0.tar", last modified: Tue Jul  4 23:34:38 2023, max compression
```

## Comparing `opentaskpy-0.8.1.tar` & `opentaskpy-0.9.0.tar`

### file list

```diff
@@ -1,86 +1,86 @@
-drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2023-04-17 16:02:47.414677 opentaskpy-0.8.1/
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)       72 2023-04-17 16:01:52.000000 opentaskpy-0.8.1/AUTHORS
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)    35149 2023-04-17 16:01:52.000000 opentaskpy-0.8.1/LICENSE
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)       44 2023-04-17 16:01:52.000000 opentaskpy-0.8.1/MANIFEST.in
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)    17790 2023-04-17 16:02:47.414677 opentaskpy-0.8.1/PKG-INFO
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)    16943 2023-04-17 16:01:52.000000 opentaskpy-0.8.1/README.md
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     1853 2023-04-17 16:01:52.000000 opentaskpy-0.8.1/pyproject.toml
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)       38 2023-04-17 16:02:47.414677 opentaskpy-0.8.1/setup.cfg
-drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2023-04-17 16:02:47.402677 opentaskpy-0.8.1/src/
-drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2023-04-17 16:02:47.406678 opentaskpy-0.8.1/src/opentaskpy/
-drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2023-04-17 16:02:47.406678 opentaskpy-0.8.1/src/opentaskpy/cli/
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     2052 2023-04-17 16:01:52.000000 opentaskpy-0.8.1/src/opentaskpy/cli/task_run.py
-drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2023-04-17 16:02:47.406678 opentaskpy-0.8.1/src/opentaskpy/config/
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)        0 2023-04-06 12:19:29.000000 opentaskpy-0.8.1/src/opentaskpy/config/__init__.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)    10322 2023-04-06 12:19:29.000000 opentaskpy-0.8.1/src/opentaskpy/config/loader.py
-drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2023-04-17 16:02:47.406678 opentaskpy-0.8.1/src/opentaskpy/config/schemas/
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     1659 2023-04-17 16:01:52.000000 opentaskpy-0.8.1/src/opentaskpy/config/schemas/batch.json
-drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2023-04-17 16:02:47.402677 opentaskpy-0.8.1/src/opentaskpy/config/schemas/execution/
-drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2023-04-17 16:02:47.406678 opentaskpy-0.8.1/src/opentaskpy/config/schemas/execution/ssh/
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)      497 2023-04-17 16:01:52.000000 opentaskpy-0.8.1/src/opentaskpy/config/schemas/execution/ssh/protocol.json
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)      461 2023-04-17 16:01:52.000000 opentaskpy-0.8.1/src/opentaskpy/config/schemas/execution/ssh/ssh.json
-drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2023-04-17 16:02:47.410678 opentaskpy-0.8.1/src/opentaskpy/config/schemas/transfer/
-drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2023-04-17 16:02:47.410678 opentaskpy-0.8.1/src/opentaskpy/config/schemas/transfer/email/
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)      762 2023-04-17 16:01:52.000000 opentaskpy-0.8.1/src/opentaskpy/config/schemas/transfer/email/protocol.json
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)      385 2023-04-17 16:01:52.000000 opentaskpy-0.8.1/src/opentaskpy/config/schemas/transfer/email_destination.json
-drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2023-04-17 16:02:47.410678 opentaskpy-0.8.1/src/opentaskpy/config/schemas/transfer/ssh_destination/
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)      162 2023-04-17 16:01:52.000000 opentaskpy-0.8.1/src/opentaskpy/config/schemas/transfer/ssh_destination/flags.json
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)      212 2023-04-17 16:01:52.000000 opentaskpy-0.8.1/src/opentaskpy/config/schemas/transfer/ssh_destination/permissions.json
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)      565 2023-04-17 16:01:52.000000 opentaskpy-0.8.1/src/opentaskpy/config/schemas/transfer/ssh_destination/protocol.json
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)      214 2023-04-17 16:01:52.000000 opentaskpy-0.8.1/src/opentaskpy/config/schemas/transfer/ssh_destination/rename.json
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)      693 2023-04-17 16:01:52.000000 opentaskpy-0.8.1/src/opentaskpy/config/schemas/transfer/ssh_destination.json
-drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2023-04-17 16:02:47.410678 opentaskpy-0.8.1/src/opentaskpy/config/schemas/transfer/ssh_source/
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)      865 2023-04-17 16:01:52.000000 opentaskpy-0.8.1/src/opentaskpy/config/schemas/transfer/ssh_source/conditionals.json
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)      274 2023-04-17 16:01:52.000000 opentaskpy-0.8.1/src/opentaskpy/config/schemas/transfer/ssh_source/fileWatch.json
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)      383 2023-04-17 16:01:52.000000 opentaskpy-0.8.1/src/opentaskpy/config/schemas/transfer/ssh_source/logWatch.json
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     1284 2023-04-17 16:01:52.000000 opentaskpy-0.8.1/src/opentaskpy/config/schemas/transfer/ssh_source/postCopyAction.json
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)      497 2023-04-17 16:01:52.000000 opentaskpy-0.8.1/src/opentaskpy/config/schemas/transfer/ssh_source/protocol.json
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)      691 2023-04-17 16:01:52.000000 opentaskpy-0.8.1/src/opentaskpy/config/schemas/transfer/ssh_source.json
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     9714 2023-04-06 12:19:29.000000 opentaskpy-0.8.1/src/opentaskpy/config/schemas.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     1236 2023-04-06 12:19:29.000000 opentaskpy-0.8.1/src/opentaskpy/exceptions.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     5685 2023-04-06 12:19:29.000000 opentaskpy-0.8.1/src/opentaskpy/logging.py
-drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2023-04-17 16:02:47.402677 opentaskpy-0.8.1/src/opentaskpy/plugins/
-drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2023-04-17 16:02:47.410678 opentaskpy-0.8.1/src/opentaskpy/plugins/lookup/
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)      844 2023-04-06 12:19:29.000000 opentaskpy-0.8.1/src/opentaskpy/plugins/lookup/file.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     1191 2023-04-06 12:19:29.000000 opentaskpy-0.8.1/src/opentaskpy/plugins/lookup/http_json.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)      627 2023-04-06 12:19:29.000000 opentaskpy-0.8.1/src/opentaskpy/plugins/lookup/random.py
-drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2023-04-17 16:02:47.410678 opentaskpy-0.8.1/src/opentaskpy/remotehandlers/
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)        0 2023-04-06 12:19:29.000000 opentaskpy-0.8.1/src/opentaskpy/remotehandlers/__init__.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     4099 2023-04-06 12:19:29.000000 opentaskpy-0.8.1/src/opentaskpy/remotehandlers/email.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)      930 2023-04-06 12:19:29.000000 opentaskpy-0.8.1/src/opentaskpy/remotehandlers/remotehandler.py
-drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2023-04-17 16:02:47.410678 opentaskpy-0.8.1/src/opentaskpy/remotehandlers/scripts/
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     6265 2023-04-06 12:19:29.000000 opentaskpy-0.8.1/src/opentaskpy/remotehandlers/scripts/transfer.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)    29670 2023-04-06 12:19:29.000000 opentaskpy-0.8.1/src/opentaskpy/remotehandlers/ssh.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     2754 2023-04-06 12:19:29.000000 opentaskpy-0.8.1/src/opentaskpy/task_run.py
-drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2023-04-17 16:02:47.414677 opentaskpy-0.8.1/src/opentaskpy/taskhandlers/
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)        0 2023-04-06 12:19:29.000000 opentaskpy-0.8.1/src/opentaskpy/taskhandlers/__init__.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)    16851 2023-04-06 12:19:29.000000 opentaskpy-0.8.1/src/opentaskpy/taskhandlers/batch.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     6612 2023-04-06 12:19:29.000000 opentaskpy-0.8.1/src/opentaskpy/taskhandlers/execution.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     2692 2023-04-06 12:19:29.000000 opentaskpy-0.8.1/src/opentaskpy/taskhandlers/taskhandler.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)    23016 2023-04-06 12:19:29.000000 opentaskpy-0.8.1/src/opentaskpy/taskhandlers/transfer.py
-drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2023-04-17 16:02:47.406678 opentaskpy-0.8.1/src/opentaskpy.egg-info/
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)    17790 2023-04-17 16:02:47.000000 opentaskpy-0.8.1/src/opentaskpy.egg-info/PKG-INFO
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     2630 2023-04-17 16:02:47.000000 opentaskpy-0.8.1/src/opentaskpy.egg-info/SOURCES.txt
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)        1 2023-04-17 16:02:47.000000 opentaskpy-0.8.1/src/opentaskpy.egg-info/dependency_links.txt
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)       58 2023-04-17 16:02:47.000000 opentaskpy-0.8.1/src/opentaskpy.egg-info/entry_points.txt
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)      241 2023-04-17 16:02:47.000000 opentaskpy-0.8.1/src/opentaskpy.egg-info/requires.txt
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)       11 2023-04-17 16:02:47.000000 opentaskpy-0.8.1/src/opentaskpy.egg-info/top_level.txt
-drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2023-04-17 16:02:47.414677 opentaskpy-0.8.1/tests/
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     1463 2023-04-11 16:45:44.000000 opentaskpy-0.8.1/tests/test_batch_schema_validate.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)    13804 2023-04-06 12:19:29.000000 opentaskpy-0.8.1/tests/test_config_loader.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     6939 2023-04-06 12:19:29.000000 opentaskpy-0.8.1/tests/test_docker_task_run.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)      969 2023-04-06 12:19:29.000000 opentaskpy-0.8.1/tests/test_email_transfer_schema_validate.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)      836 2023-04-06 12:19:29.000000 opentaskpy-0.8.1/tests/test_file_helper.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     7891 2023-04-06 12:19:29.000000 opentaskpy-0.8.1/tests/test_logging.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)      911 2023-04-06 12:19:29.000000 opentaskpy-0.8.1/tests/test_plugin_file.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     1126 2023-04-06 12:19:29.000000 opentaskpy-0.8.1/tests/test_plugin_http_json.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     8416 2023-04-06 12:19:29.000000 opentaskpy-0.8.1/tests/test_remote_transfer_script.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     1920 2023-04-06 12:19:29.000000 opentaskpy-0.8.1/tests/test_schema_validate.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     3535 2023-04-06 12:19:29.000000 opentaskpy-0.8.1/tests/test_ssh_dest_schema_validate.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     1060 2023-04-06 12:19:29.000000 opentaskpy-0.8.1/tests/test_ssh_execution_schema_validate.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     5874 2023-04-06 12:19:29.000000 opentaskpy-0.8.1/tests/test_ssh_source_schema_validate.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)    14719 2023-04-06 12:19:29.000000 opentaskpy-0.8.1/tests/test_task_run.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)    14301 2023-04-06 12:19:29.000000 opentaskpy-0.8.1/tests/test_taskhandler_batch.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     4420 2023-04-06 12:19:29.000000 opentaskpy-0.8.1/tests/test_taskhandler_execution.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     4205 2023-04-06 12:19:29.000000 opentaskpy-0.8.1/tests/test_taskhandler_transfer_email.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)    14339 2023-04-06 12:19:29.000000 opentaskpy-0.8.1/tests/test_taskhandler_transfer_ssh.py
+drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2023-07-04 23:34:38.634912 opentaskpy-0.9.0/
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)       72 2023-06-21 12:17:10.000000 opentaskpy-0.9.0/AUTHORS
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)    35149 2023-06-21 12:17:10.000000 opentaskpy-0.9.0/LICENSE
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)       44 2023-06-21 12:17:10.000000 opentaskpy-0.9.0/MANIFEST.in
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)    18568 2023-07-04 23:34:38.634912 opentaskpy-0.9.0/PKG-INFO
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)    17721 2023-07-03 16:18:31.000000 opentaskpy-0.9.0/README.md
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)    12964 2023-07-04 23:24:00.000000 opentaskpy-0.9.0/pyproject.toml
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)       38 2023-07-04 23:34:38.634912 opentaskpy-0.9.0/setup.cfg
+drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2023-07-04 23:34:38.586912 opentaskpy-0.9.0/src/
+drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2023-07-04 23:34:38.606912 opentaskpy-0.9.0/src/opentaskpy/
+drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2023-07-04 23:34:38.606912 opentaskpy-0.9.0/src/opentaskpy/cli/
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     2348 2023-07-03 15:48:53.000000 opentaskpy-0.9.0/src/opentaskpy/cli/task_run.py
+drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2023-07-04 23:34:38.610912 opentaskpy-0.9.0/src/opentaskpy/config/
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)        0 2023-06-22 14:36:44.000000 opentaskpy-0.9.0/src/opentaskpy/config/__init__.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)    12443 2023-07-03 16:18:03.000000 opentaskpy-0.9.0/src/opentaskpy/config/loader.py
+drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2023-07-04 23:34:38.610912 opentaskpy-0.9.0/src/opentaskpy/config/schemas/
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     1647 2023-06-21 12:17:10.000000 opentaskpy-0.9.0/src/opentaskpy/config/schemas/batch.json
+drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2023-07-04 23:34:38.586912 opentaskpy-0.9.0/src/opentaskpy/config/schemas/execution/
+drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2023-07-04 23:34:38.614912 opentaskpy-0.9.0/src/opentaskpy/config/schemas/execution/ssh/
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)      453 2023-06-21 12:17:10.000000 opentaskpy-0.9.0/src/opentaskpy/config/schemas/execution/ssh/protocol.json
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)      437 2023-06-21 12:17:10.000000 opentaskpy-0.9.0/src/opentaskpy/config/schemas/execution/ssh/ssh.json
+drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2023-07-04 23:34:38.618912 opentaskpy-0.9.0/src/opentaskpy/config/schemas/transfer/
+drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2023-07-04 23:34:38.618912 opentaskpy-0.9.0/src/opentaskpy/config/schemas/transfer/email/
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)      714 2023-06-21 12:17:10.000000 opentaskpy-0.9.0/src/opentaskpy/config/schemas/transfer/email/protocol.json
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)      369 2023-06-21 12:17:10.000000 opentaskpy-0.9.0/src/opentaskpy/config/schemas/transfer/email_destination.json
+drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2023-07-04 23:34:38.618912 opentaskpy-0.9.0/src/opentaskpy/config/schemas/transfer/ssh_destination/
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)      154 2023-06-21 12:17:10.000000 opentaskpy-0.9.0/src/opentaskpy/config/schemas/transfer/ssh_destination/flags.json
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)      212 2023-06-21 12:17:10.000000 opentaskpy-0.9.0/src/opentaskpy/config/schemas/transfer/ssh_destination/permissions.json
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)      521 2023-06-21 12:17:10.000000 opentaskpy-0.9.0/src/opentaskpy/config/schemas/transfer/ssh_destination/protocol.json
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)      202 2023-06-21 12:17:10.000000 opentaskpy-0.9.0/src/opentaskpy/config/schemas/transfer/ssh_destination/rename.json
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)      645 2023-06-21 12:17:10.000000 opentaskpy-0.9.0/src/opentaskpy/config/schemas/transfer/ssh_destination.json
+drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2023-07-04 23:34:38.622913 opentaskpy-0.9.0/src/opentaskpy/config/schemas/transfer/ssh_source/
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)      769 2023-06-21 12:17:10.000000 opentaskpy-0.9.0/src/opentaskpy/config/schemas/transfer/ssh_source/conditionals.json
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)      274 2023-06-21 12:17:10.000000 opentaskpy-0.9.0/src/opentaskpy/config/schemas/transfer/ssh_source/fileWatch.json
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)      367 2023-06-21 12:17:10.000000 opentaskpy-0.9.0/src/opentaskpy/config/schemas/transfer/ssh_source/logWatch.json
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     1106 2023-06-21 12:17:10.000000 opentaskpy-0.9.0/src/opentaskpy/config/schemas/transfer/ssh_source/postCopyAction.json
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)      453 2023-06-21 12:17:10.000000 opentaskpy-0.9.0/src/opentaskpy/config/schemas/transfer/ssh_source/protocol.json
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)      675 2023-06-21 12:17:10.000000 opentaskpy-0.9.0/src/opentaskpy/config/schemas/transfer/ssh_source.json
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)    10526 2023-06-22 14:36:52.000000 opentaskpy-0.9.0/src/opentaskpy/config/schemas.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     2399 2023-07-03 16:04:55.000000 opentaskpy-0.9.0/src/opentaskpy/exceptions.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     7751 2023-07-03 16:17:13.000000 opentaskpy-0.9.0/src/opentaskpy/otflogging.py
+drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2023-07-04 23:34:38.586912 opentaskpy-0.9.0/src/opentaskpy/plugins/
+drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2023-07-04 23:34:38.622913 opentaskpy-0.9.0/src/opentaskpy/plugins/lookup/
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     1414 2023-06-21 12:17:10.000000 opentaskpy-0.9.0/src/opentaskpy/plugins/lookup/file.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     1904 2023-06-21 12:17:10.000000 opentaskpy-0.9.0/src/opentaskpy/plugins/lookup/http_json.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     1109 2023-06-21 12:17:10.000000 opentaskpy-0.9.0/src/opentaskpy/plugins/lookup/random_number.py
+drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2023-07-04 23:34:38.626912 opentaskpy-0.9.0/src/opentaskpy/remotehandlers/
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)        0 2023-06-21 12:17:10.000000 opentaskpy-0.9.0/src/opentaskpy/remotehandlers/__init__.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     5607 2023-07-03 15:48:53.000000 opentaskpy-0.9.0/src/opentaskpy/remotehandlers/email.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     4284 2023-07-03 15:48:53.000000 opentaskpy-0.9.0/src/opentaskpy/remotehandlers/remotehandler.py
+drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2023-07-04 23:34:38.626912 opentaskpy-0.9.0/src/opentaskpy/remotehandlers/scripts/
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     7567 2023-07-03 16:17:04.000000 opentaskpy-0.9.0/src/opentaskpy/remotehandlers/scripts/transfer.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)    39110 2023-07-04 23:14:49.000000 opentaskpy-0.9.0/src/opentaskpy/remotehandlers/ssh.py
+drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2023-07-04 23:34:38.626912 opentaskpy-0.9.0/src/opentaskpy/taskhandlers/
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)        0 2023-06-21 12:17:10.000000 opentaskpy-0.9.0/src/opentaskpy/taskhandlers/__init__.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)    18253 2023-07-03 16:06:06.000000 opentaskpy-0.9.0/src/opentaskpy/taskhandlers/batch.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     7914 2023-07-03 16:04:01.000000 opentaskpy-0.9.0/src/opentaskpy/taskhandlers/execution.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     4651 2023-07-03 16:02:43.000000 opentaskpy-0.9.0/src/opentaskpy/taskhandlers/taskhandler.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)    24356 2023-07-03 16:59:17.000000 opentaskpy-0.9.0/src/opentaskpy/taskhandlers/transfer.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     3425 2023-07-03 16:17:09.000000 opentaskpy-0.9.0/src/opentaskpy/taskrun.py
+drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2023-07-04 23:34:38.606912 opentaskpy-0.9.0/src/opentaskpy.egg-info/
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)    18568 2023-07-04 23:34:38.000000 opentaskpy-0.9.0/src/opentaskpy.egg-info/PKG-INFO
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     2639 2023-07-04 23:34:38.000000 opentaskpy-0.9.0/src/opentaskpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)        1 2023-07-04 23:34:38.000000 opentaskpy-0.9.0/src/opentaskpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)       58 2023-07-04 23:34:38.000000 opentaskpy-0.9.0/src/opentaskpy.egg-info/entry_points.txt
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)      229 2023-07-04 23:34:38.000000 opentaskpy-0.9.0/src/opentaskpy.egg-info/requires.txt
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)       11 2023-07-04 23:34:38.000000 opentaskpy-0.9.0/src/opentaskpy.egg-info/top_level.txt
+drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2023-07-04 23:34:38.634912 opentaskpy-0.9.0/tests/
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     1483 2023-07-03 17:03:48.000000 opentaskpy-0.9.0/tests/test_batch_schema_validate.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)    14985 2023-07-04 15:01:59.000000 opentaskpy-0.9.0/tests/test_config_loader.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     6928 2023-07-04 14:47:34.000000 opentaskpy-0.9.0/tests/test_docker_task_run.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)      989 2023-07-03 17:03:41.000000 opentaskpy-0.9.0/tests/test_email_transfer_schema_validate.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)      852 2023-07-03 17:03:39.000000 opentaskpy-0.9.0/tests/test_file_helper.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     8070 2023-07-03 16:16:37.000000 opentaskpy-0.9.0/tests/test_logging.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)      942 2023-07-03 17:03:34.000000 opentaskpy-0.9.0/tests/test_plugin_file.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     1146 2023-07-03 17:03:32.000000 opentaskpy-0.9.0/tests/test_plugin_http_json.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     8441 2023-07-03 17:03:29.000000 opentaskpy-0.9.0/tests/test_remote_transfer_script.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     1940 2023-07-03 17:03:26.000000 opentaskpy-0.9.0/tests/test_schema_validate.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     3555 2023-07-03 17:03:23.000000 opentaskpy-0.9.0/tests/test_ssh_dest_schema_validate.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     1080 2023-07-03 17:03:01.000000 opentaskpy-0.9.0/tests/test_ssh_execution_schema_validate.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     5894 2023-07-03 17:02:57.000000 opentaskpy-0.9.0/tests/test_ssh_source_schema_validate.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)    14769 2023-07-03 16:19:14.000000 opentaskpy-0.9.0/tests/test_task_run.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)    14484 2023-07-03 17:02:51.000000 opentaskpy-0.9.0/tests/test_taskhandler_batch.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     4461 2023-07-03 17:02:47.000000 opentaskpy-0.9.0/tests/test_taskhandler_execution.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     4377 2023-07-03 17:02:43.000000 opentaskpy-0.9.0/tests/test_taskhandler_transfer_email.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)    14515 2023-07-03 17:02:28.000000 opentaskpy-0.9.0/tests/test_taskhandler_transfer_ssh.py
```

### Comparing `opentaskpy-0.8.1/LICENSE` & `opentaskpy-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `opentaskpy-0.8.1/PKG-INFO` & `opentaskpy-0.9.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 Metadata-Version: 2.1
 Name: opentaskpy
-Version: 0.8.1
+Version: 0.9.0
 Summary: A framework for automation execution of commands and transferring files between hosts
 Author-email: Adam McDonagh <adam@elitemonkey.net>
 License: GPLv3
 Project-URL: Homepage, https://github.com/adammcdonagh/open-task-framework
 Project-URL: Bug Tracker, https://github.com/adammcdonagh/open-task-framework/issues
 Project-URL: Changelog, https://github.com/adammcdonagh/open-task-framework/blob/main/CHANGELOG.md
 Keywords: automation,task,framework,scheduling,ssh,sftp,remote,execution,command
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: POSIX
-Requires-Python: >=3.10
+Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 License-File: AUTHORS
 
-
 ![unittest status](https://github.com/adammcdonagh/open-task-framework/actions/workflows/main.yml/badge.svg?event=push)
 
 <h1>Open Task Framework (opentaskpy)</h1>
 
 - [Installation](#installation)
+  - [Example Deployment](#example-deployment)
 - [Configuration](#configuration)
   - [Command Line Arguments](#command-line-arguments)
   - [Environment Variables](#environment-variables)
   - [Logging](#logging)
   - [Variables](#variables)
   - [Runtime Overrides](#runtime-overrides)
   - [Lookup plugins](#lookup-plugins)
-      - [Adding your own](#adding-your-own)
+    - [Adding your own](#adding-your-own)
     - [Example Variables](#example-variables)
 - [Task Definitions](#task-definitions)
   - [Transfers](#transfers)
   - [Executions](#executions)
   - [Batches](#batches)
 - [Development](#development)
   - [Quickstart for development](#quickstart-for-development)
@@ -46,25 +46,27 @@
     - [Addons](#addons)
 
 Open Task Framework (OTF) is a Python based framework to make it easy to run predefined file transfers and scripts/commands on remote machines.
 
 Currently the framework is primarily based around being able to use SSH to communicate with remote hosts in order to manipulate files and run commands. This is done via the use of SSH keys, which must be set up in advance.
 
 OTF has 3 main concepts for tasks. These are:
-* Transfers
-* Executions
-* Batches
+
+- Transfers
+- Executions
+- Batches
 
 For more details, see the [task types](docs/task-types.md) doc
 
 # Installation
 
 OTF can be run either as an installed script, or via a docker container
 
 Install via pip:
+
 ```shell
 pip install opentaskpy
 ```
 
 The `task-run` script will be added to your PATH, and you can invoke it directly.
 
 To run via docker, use the `Dockerfile` to create your own base image using just the standard opentaskpy library. However if you want to install addons, you'll need to customise this, to install the additional packages first, before bundling it as a Docker image.
@@ -74,14 +76,22 @@
 docker run --rm --volume /opt/otf/cfg:/cfg --volume /var/log/otf:/logs--volume /home/<USER>/.ssh/id_rsa:/id_rsa -e OTF_SSH_KEY=/id_rsa -e OTF_LOG_DIRECTORY=/logs task-run -t <TASK NAME> -c /cfg # Run a task
 ```
 
 The default `opentaskpy` library is only really designed to use SSH for executions and file transfers. To do this, you need to make sure that the host/container that is running the `task-run` script has a private RSA key, that is trusted on all remote hosts that you're running against.
 
 An environment variable `OTF_SSH_KEY` can be used to define a default SSH key to use for all SSH connectivity. This can be overridden at the transfer/execution level by specifying a `keyFile` in the `credentials` section of the protocol definition.
 
+## Example Deployment
+
+This is an example deployment for using OTF in an AWS environment, using BMC Control-M as the job scheduler. Control-M could be replaced with any job scheduler, AWS EventBridge for example, depending on your requirements.
+
+![AWS Deployment](docs/aws.png)
+
+"Admin/Status Portal" currently does not exist, and is a placeholder for a potential further project to visualise the OTF configs, as well as including real-time job statuses from the job scheduler.
+
 # Configuration
 
 There are several ways to customise the running of tasks.
 
 ## Command Line Arguments
 
 The following details the syntax of the `task-run` command:
@@ -121,18 +131,20 @@
 
 In order for the process to run, you must have at least one task, and a `variables.json.j2` file, even if it's just an empty object definition
 
 ## Environment Variables
 
 These are some environment variables that can be used to customise the behaviour of the application. There are some internally used variables too, but changing them without a full understanding of the code is not advised.
 
-   * `OTF_NO_LOG` - Disable logging to file. Only log to stderr
-   * `OTF_LOG_DIRECTORY` - Path under which log files are written
-   * `OTF_RUN_ID` - (meant for internal use) An aggregator for log files. When set, all log files for a run will go under this sub directory. E.g. running a batch, all execution and transfer logs will be dropped into this sub directory, rather than a directory for each task name. This is equivalent to using `-r` or `--runId` command line arguments, which is generally preferred.
-   * `OTF_SSH_KEY` - The private SSH key to use by default for all SSH connections. This is essential when using a basic docker container to trigger OTF. If not specified, it will default to use any private SSH keys available to the user executing the application.
+- `OTF_NO_LOG` - Disable logging to file. Only log to stderr
+- `OTF_LOG_DIRECTORY` - Path under which log files are written
+- `OTF_RUN_ID` - (meant for internal use) An aggregator for log files. When set, all log files for a run will go under this sub directory. E.g. running a batch, all execution and transfer logs will be dropped into this sub directory, rather than a directory for each task name. This is equivalent to using `-r` or `--runId` command line arguments, which is generally preferred.
+- `OTF_SSH_KEY` - The private SSH key to use by default for all SSH connections. This is essential when using a basic docker container to trigger OTF. If not specified, it will default to use any private SSH keys available to the user executing the application.
+- `OTF_REMOTE_SCRIPT_BASE_DIR` - Alternative location to drop the temporary `transfer.py` script on remote hosts using SSH protocol. Default is `/tmp`
+- `OTF_STAGING_DIR` - Staging base directory to place files before they're dropped into their final location. Default is `/tmp`
 
 ## Logging
 
 By default, OTF will log to a directory called `logs` in the current working directory. For the docker containers, unless overridden by `OTF_LOG_DIRECTORY`, it will write to `/logs` using a symlink at `/app/logs`
 
 ## Variables
 
@@ -146,14 +158,15 @@
 
 ## Runtime Overrides
 
 Sometimes you might want to override the current date, or something specific about a file transfer when you manually run a task. This can be done using environment variables.
 
 Standard global variables can be overridden simply by setting an environment variable that matches the name of the variable you want to override e.g. `export DD=01`
 In the log output, you'll see something like this:
+
 ```
 Overriding global variable (DD: 05) with environment variable (01)
 ```
 
 To override task specific values, you can use the following format in the environment variable name:
 `OTF_OVERRIDE_<TASK_TYPE>_<ATTRIBUTE>_<ATTRIBUTE>_<ATTRIBUTE>`
 
@@ -161,45 +174,49 @@
 
 Case doesn't matter here. For attributes that are nested within an array, you can specify the array index
 
 e.g. `OTF_OVERRIDE_TRANSFER_DESTINATION_0_PROTOCOL_CREDENTIALS_USERNAME`
 
 Again this will be logged to show you that the override is being applied.
 
-
 ## Lookup plugins
 
 Static variables are useful, however sometimes you need to look up something a bit more dynamic, or secret, that you don't want to hard code into the variables file.
 
 There are 2 default lookup plugins available:
 
-* File
-* HTTP JSON
+- File
+- HTTP JSON
 
 The file plugin will load the content of a file into the variable e.g.
+
 ```jinja
 "{{ lookup('file', path='/tmp/variable_lookup.txt') }}"
 ```
 
 The HTTP JSON plugin will perform a very basic HTTP GET request, expecting a JSON response. The value to extract is defined by a jsonpath e.g.
+
 ```jinja
 "{{ lookup('http_json', url='https://jsonplaceholder.typicode.com/posts/1', jsonpath='$.title') }}"
 ```
+
 This will hit the typicode.com side, and extract the title attribute from from the returned JSON file
 
 #### Adding your own
 
 OTF will look for plugins that are either available as an installed module (under the `opentaskpy.plugins.lookup` namespace), or dropped in a `plugins` under the config directory.
 
 An example Python module might be: `opentaskpy.plugins.lookup.aws.ssm`. This can then be referenced as a variable in a template like so:
+
 ```jinja
 "{{ lookup('aws.ssm', name='my_test_param') }}"
 ```
 
 Alternatively a lookup plugin could be placed under `cfg/plugins` named `my_lookup.py`, and used in a template:
+
 ```jinja
 "{{ lookup('my_lookup', name='my_param') }}"
 ```
 
 ### Example Variables
 
 Below are examples of some useful variables to start with:
@@ -306,37 +323,34 @@
         }
       }
     }
   ]
 }
 ```
 
-An explaination of what's going on in the order it will handled:
+An explanation of what's going on in the order it will handled:
 
 1. Tail the log file matching named: `/tmp/testFiles/src/log{{ YYYY }}Watch1.log` for lines matching containing the regex `someText[0-9]`, for up to 15 seconds, before giving up.
 2. Poll for a file matching the regex `/tmp/testFiles/src/fileWatch\.txt` for up to 15 seconds.
 3. Find all files matching the regex `/tmp/testFiles/src/.*\.txt`, with the conditions that the are >10B and <20B in size, as well as being older than 60 seconds, but newer than 600 seconds since last modification
 4. Transfer the files that were found to 2 destinations.
    1. The first destination is a simple SCP from `HOST_A` to `HOST_B` where the file is placed under `/tmp/testFiles/dest`. The group ownership of the file(s) is then set to `operator`
    2. The second destination is done via a pull from the destination server into the same directory. The SCP connects to `HOST_A` as `transferUsername`. Once the file has been retrieved, it is renamed using the following regex match `^(.*)\.txt$` and substitution `\1-2.txt`
 5. Transferred files are moved into `/tmp/testFiles/archive` on `HOST_A`
 
-
 ## Executions
 
 Executions are the simplest task to configure. They consist of a list of hosts to run on, the username to run/connect as, and the command to run.
 
 Executions do not currently have a timeout, so can in theory run forever, or until they are killed. If a timeout is required, either use a wrapper script on the host the command is being executed on, or they should be wrapped inside a batch.
 
 ```json
 {
   "type": "execution",
-  "hosts": [
-    "{{ HOST_A }}"
-  ],
+  "hosts": ["{{ HOST_A }}"],
   "directory": "/tmp/testFiles/src",
   "command": "touch touchedFile.txt",
   "protocol": {
     "name": "ssh",
     "credentials": {
       "username": "{{ SSH_USERNAME }}"
     }
@@ -346,59 +360,61 @@
 
 The above is running the command `touch touchedFile.txt` on `{{ HOST_A }}`, from within the `/tmp/testFiles/src` directory.
 
 If multiple `hosts` are defined, a thread is spawned in parallel for each host. If the command fails on any of the hosts in the list, it will cause the task run to fail, once all processes have returned a result.
 
 ## Batches
 
-Batches are a little more complex. They do not contain any task definitions, only the list, and order of excecution for each task.
+Batches are a little more complex. They do not contain any task definitions, only the list, and order of execution for each task.
 
 A batch task can have multiple options set that determine the execution order and conditions, as well as how failures and task reruns are handled.
 
 Each task in a batch has an `order_id`, this is a unique ID for each task, and is primarily used to define dependencies.
 
 `dependencies` can be applied to any task, and are simply a list of other tasks that must be completed before it is triggered.
 
 `continue_on_fail` is a boolean that defines whether a failure would cause the whole batch to fail immediately (after existing tasks have finished executing), or whether following steps get run. This defaults to false if not defined.
 
 `retry_on_rerun` is a boolean that determines whether a successful task is run a second time following a failed run. If a batch exits with a failure, and then the script is reun later on that same day, by default only the steps that failed will be run. All steps can be forced to run by setting this to true
 
 `timeout` specifies the number of seconds a task is allowed to be running before it gets terminated. This counts as a failure. The default timeout, if not specified is 300 seconds.
 
-
 # Development
 
 This repo has been primarily configured to work with GitHub Codespaces devcontainers, though it can obviously be used directly on your machine too.
 
 Dev and runtime packages are defined via pipenv, with a `requirements.txt` for the runtime package requirements
 
 ## Quickstart for development
 
-* Clone this repo
-* pip install pipenv
-* pipenv --python 3.10 && pipenv install && cd src && pipenv install --editable .
+- Clone this repo
+- pip install pipenv
+- pipenv --python 3.10 && pipenv install && cd src && pipenv install --editable .
 
 ### Building and uploading to PyPi
 
 ```bash
 python3 -m build
 python3 -m twine upload --repository testpypi dist/*
 ```
 
 ## Official Addons/Plugins
 
 Here's a list of official addons:
+
 ### [otf-addons-aws](https://github.com/adammcdonagh/otf-addons-aws)
 
 Provides transfer and execution addons:
-   * Remote handler for interacting with AWS S3 buckets
-   * Remote handler for executing AWS Lambda functions
+
+- Remote handler for interacting with AWS S3 buckets
+- Remote handler for executing AWS Lambda functions
 
 Lookup plugins:
-   * Support for AWS SSM Parameter Store for retrieving global variables
+
+- Support for AWS SSM Parameter Store for retrieving global variables
 
 ## Developing your own addon/plugin
 
 ### Lookup Plugins
 
 Plugins are very simple. They simply need a `run` function, and to return the required variable based on a list of kwargs provided within the config template.
```

### Comparing `opentaskpy-0.8.1/README.md` & `opentaskpy-0.9.0/src/opentaskpy.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,40 @@
+Metadata-Version: 2.1
+Name: opentaskpy
+Version: 0.9.0
+Summary: A framework for automation execution of commands and transferring files between hosts
+Author-email: Adam McDonagh <adam@elitemonkey.net>
+License: GPLv3
+Project-URL: Homepage, https://github.com/adammcdonagh/open-task-framework
+Project-URL: Bug Tracker, https://github.com/adammcdonagh/open-task-framework/issues
+Project-URL: Changelog, https://github.com/adammcdonagh/open-task-framework/blob/main/CHANGELOG.md
+Keywords: automation,task,framework,scheduling,ssh,sftp,remote,execution,command
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Operating System :: POSIX
+Requires-Python: >=3.11
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+License-File: LICENSE
+License-File: AUTHORS
 
 ![unittest status](https://github.com/adammcdonagh/open-task-framework/actions/workflows/main.yml/badge.svg?event=push)
 
 <h1>Open Task Framework (opentaskpy)</h1>
 
 - [Installation](#installation)
+  - [Example Deployment](#example-deployment)
 - [Configuration](#configuration)
   - [Command Line Arguments](#command-line-arguments)
   - [Environment Variables](#environment-variables)
   - [Logging](#logging)
   - [Variables](#variables)
   - [Runtime Overrides](#runtime-overrides)
   - [Lookup plugins](#lookup-plugins)
-      - [Adding your own](#adding-your-own)
+    - [Adding your own](#adding-your-own)
     - [Example Variables](#example-variables)
 - [Task Definitions](#task-definitions)
   - [Transfers](#transfers)
   - [Executions](#executions)
   - [Batches](#batches)
 - [Development](#development)
   - [Quickstart for development](#quickstart-for-development)
@@ -27,25 +46,27 @@
     - [Addons](#addons)
 
 Open Task Framework (OTF) is a Python based framework to make it easy to run predefined file transfers and scripts/commands on remote machines.
 
 Currently the framework is primarily based around being able to use SSH to communicate with remote hosts in order to manipulate files and run commands. This is done via the use of SSH keys, which must be set up in advance.
 
 OTF has 3 main concepts for tasks. These are:
-* Transfers
-* Executions
-* Batches
+
+- Transfers
+- Executions
+- Batches
 
 For more details, see the [task types](docs/task-types.md) doc
 
 # Installation
 
 OTF can be run either as an installed script, or via a docker container
 
 Install via pip:
+
 ```shell
 pip install opentaskpy
 ```
 
 The `task-run` script will be added to your PATH, and you can invoke it directly.
 
 To run via docker, use the `Dockerfile` to create your own base image using just the standard opentaskpy library. However if you want to install addons, you'll need to customise this, to install the additional packages first, before bundling it as a Docker image.
@@ -55,14 +76,22 @@
 docker run --rm --volume /opt/otf/cfg:/cfg --volume /var/log/otf:/logs--volume /home/<USER>/.ssh/id_rsa:/id_rsa -e OTF_SSH_KEY=/id_rsa -e OTF_LOG_DIRECTORY=/logs task-run -t <TASK NAME> -c /cfg # Run a task
 ```
 
 The default `opentaskpy` library is only really designed to use SSH for executions and file transfers. To do this, you need to make sure that the host/container that is running the `task-run` script has a private RSA key, that is trusted on all remote hosts that you're running against.
 
 An environment variable `OTF_SSH_KEY` can be used to define a default SSH key to use for all SSH connectivity. This can be overridden at the transfer/execution level by specifying a `keyFile` in the `credentials` section of the protocol definition.
 
+## Example Deployment
+
+This is an example deployment for using OTF in an AWS environment, using BMC Control-M as the job scheduler. Control-M could be replaced with any job scheduler, AWS EventBridge for example, depending on your requirements.
+
+![AWS Deployment](docs/aws.png)
+
+"Admin/Status Portal" currently does not exist, and is a placeholder for a potential further project to visualise the OTF configs, as well as including real-time job statuses from the job scheduler.
+
 # Configuration
 
 There are several ways to customise the running of tasks.
 
 ## Command Line Arguments
 
 The following details the syntax of the `task-run` command:
@@ -102,18 +131,20 @@
 
 In order for the process to run, you must have at least one task, and a `variables.json.j2` file, even if it's just an empty object definition
 
 ## Environment Variables
 
 These are some environment variables that can be used to customise the behaviour of the application. There are some internally used variables too, but changing them without a full understanding of the code is not advised.
 
-   * `OTF_NO_LOG` - Disable logging to file. Only log to stderr
-   * `OTF_LOG_DIRECTORY` - Path under which log files are written
-   * `OTF_RUN_ID` - (meant for internal use) An aggregator for log files. When set, all log files for a run will go under this sub directory. E.g. running a batch, all execution and transfer logs will be dropped into this sub directory, rather than a directory for each task name. This is equivalent to using `-r` or `--runId` command line arguments, which is generally preferred.
-   * `OTF_SSH_KEY` - The private SSH key to use by default for all SSH connections. This is essential when using a basic docker container to trigger OTF. If not specified, it will default to use any private SSH keys available to the user executing the application.
+- `OTF_NO_LOG` - Disable logging to file. Only log to stderr
+- `OTF_LOG_DIRECTORY` - Path under which log files are written
+- `OTF_RUN_ID` - (meant for internal use) An aggregator for log files. When set, all log files for a run will go under this sub directory. E.g. running a batch, all execution and transfer logs will be dropped into this sub directory, rather than a directory for each task name. This is equivalent to using `-r` or `--runId` command line arguments, which is generally preferred.
+- `OTF_SSH_KEY` - The private SSH key to use by default for all SSH connections. This is essential when using a basic docker container to trigger OTF. If not specified, it will default to use any private SSH keys available to the user executing the application.
+- `OTF_REMOTE_SCRIPT_BASE_DIR` - Alternative location to drop the temporary `transfer.py` script on remote hosts using SSH protocol. Default is `/tmp`
+- `OTF_STAGING_DIR` - Staging base directory to place files before they're dropped into their final location. Default is `/tmp`
 
 ## Logging
 
 By default, OTF will log to a directory called `logs` in the current working directory. For the docker containers, unless overridden by `OTF_LOG_DIRECTORY`, it will write to `/logs` using a symlink at `/app/logs`
 
 ## Variables
 
@@ -127,14 +158,15 @@
 
 ## Runtime Overrides
 
 Sometimes you might want to override the current date, or something specific about a file transfer when you manually run a task. This can be done using environment variables.
 
 Standard global variables can be overridden simply by setting an environment variable that matches the name of the variable you want to override e.g. `export DD=01`
 In the log output, you'll see something like this:
+
 ```
 Overriding global variable (DD: 05) with environment variable (01)
 ```
 
 To override task specific values, you can use the following format in the environment variable name:
 `OTF_OVERRIDE_<TASK_TYPE>_<ATTRIBUTE>_<ATTRIBUTE>_<ATTRIBUTE>`
 
@@ -142,45 +174,49 @@
 
 Case doesn't matter here. For attributes that are nested within an array, you can specify the array index
 
 e.g. `OTF_OVERRIDE_TRANSFER_DESTINATION_0_PROTOCOL_CREDENTIALS_USERNAME`
 
 Again this will be logged to show you that the override is being applied.
 
-
 ## Lookup plugins
 
 Static variables are useful, however sometimes you need to look up something a bit more dynamic, or secret, that you don't want to hard code into the variables file.
 
 There are 2 default lookup plugins available:
 
-* File
-* HTTP JSON
+- File
+- HTTP JSON
 
 The file plugin will load the content of a file into the variable e.g.
+
 ```jinja
 "{{ lookup('file', path='/tmp/variable_lookup.txt') }}"
 ```
 
 The HTTP JSON plugin will perform a very basic HTTP GET request, expecting a JSON response. The value to extract is defined by a jsonpath e.g.
+
 ```jinja
 "{{ lookup('http_json', url='https://jsonplaceholder.typicode.com/posts/1', jsonpath='$.title') }}"
 ```
+
 This will hit the typicode.com side, and extract the title attribute from from the returned JSON file
 
 #### Adding your own
 
 OTF will look for plugins that are either available as an installed module (under the `opentaskpy.plugins.lookup` namespace), or dropped in a `plugins` under the config directory.
 
 An example Python module might be: `opentaskpy.plugins.lookup.aws.ssm`. This can then be referenced as a variable in a template like so:
+
 ```jinja
 "{{ lookup('aws.ssm', name='my_test_param') }}"
 ```
 
 Alternatively a lookup plugin could be placed under `cfg/plugins` named `my_lookup.py`, and used in a template:
+
 ```jinja
 "{{ lookup('my_lookup', name='my_param') }}"
 ```
 
 ### Example Variables
 
 Below are examples of some useful variables to start with:
@@ -287,37 +323,34 @@
         }
       }
     }
   ]
 }
 ```
 
-An explaination of what's going on in the order it will handled:
+An explanation of what's going on in the order it will handled:
 
 1. Tail the log file matching named: `/tmp/testFiles/src/log{{ YYYY }}Watch1.log` for lines matching containing the regex `someText[0-9]`, for up to 15 seconds, before giving up.
 2. Poll for a file matching the regex `/tmp/testFiles/src/fileWatch\.txt` for up to 15 seconds.
 3. Find all files matching the regex `/tmp/testFiles/src/.*\.txt`, with the conditions that the are >10B and <20B in size, as well as being older than 60 seconds, but newer than 600 seconds since last modification
 4. Transfer the files that were found to 2 destinations.
    1. The first destination is a simple SCP from `HOST_A` to `HOST_B` where the file is placed under `/tmp/testFiles/dest`. The group ownership of the file(s) is then set to `operator`
    2. The second destination is done via a pull from the destination server into the same directory. The SCP connects to `HOST_A` as `transferUsername`. Once the file has been retrieved, it is renamed using the following regex match `^(.*)\.txt$` and substitution `\1-2.txt`
 5. Transferred files are moved into `/tmp/testFiles/archive` on `HOST_A`
 
-
 ## Executions
 
 Executions are the simplest task to configure. They consist of a list of hosts to run on, the username to run/connect as, and the command to run.
 
 Executions do not currently have a timeout, so can in theory run forever, or until they are killed. If a timeout is required, either use a wrapper script on the host the command is being executed on, or they should be wrapped inside a batch.
 
 ```json
 {
   "type": "execution",
-  "hosts": [
-    "{{ HOST_A }}"
-  ],
+  "hosts": ["{{ HOST_A }}"],
   "directory": "/tmp/testFiles/src",
   "command": "touch touchedFile.txt",
   "protocol": {
     "name": "ssh",
     "credentials": {
       "username": "{{ SSH_USERNAME }}"
     }
@@ -327,59 +360,61 @@
 
 The above is running the command `touch touchedFile.txt` on `{{ HOST_A }}`, from within the `/tmp/testFiles/src` directory.
 
 If multiple `hosts` are defined, a thread is spawned in parallel for each host. If the command fails on any of the hosts in the list, it will cause the task run to fail, once all processes have returned a result.
 
 ## Batches
 
-Batches are a little more complex. They do not contain any task definitions, only the list, and order of excecution for each task.
+Batches are a little more complex. They do not contain any task definitions, only the list, and order of execution for each task.
 
 A batch task can have multiple options set that determine the execution order and conditions, as well as how failures and task reruns are handled.
 
 Each task in a batch has an `order_id`, this is a unique ID for each task, and is primarily used to define dependencies.
 
 `dependencies` can be applied to any task, and are simply a list of other tasks that must be completed before it is triggered.
 
 `continue_on_fail` is a boolean that defines whether a failure would cause the whole batch to fail immediately (after existing tasks have finished executing), or whether following steps get run. This defaults to false if not defined.
 
 `retry_on_rerun` is a boolean that determines whether a successful task is run a second time following a failed run. If a batch exits with a failure, and then the script is reun later on that same day, by default only the steps that failed will be run. All steps can be forced to run by setting this to true
 
 `timeout` specifies the number of seconds a task is allowed to be running before it gets terminated. This counts as a failure. The default timeout, if not specified is 300 seconds.
 
-
 # Development
 
 This repo has been primarily configured to work with GitHub Codespaces devcontainers, though it can obviously be used directly on your machine too.
 
 Dev and runtime packages are defined via pipenv, with a `requirements.txt` for the runtime package requirements
 
 ## Quickstart for development
 
-* Clone this repo
-* pip install pipenv
-* pipenv --python 3.10 && pipenv install && cd src && pipenv install --editable .
+- Clone this repo
+- pip install pipenv
+- pipenv --python 3.10 && pipenv install && cd src && pipenv install --editable .
 
 ### Building and uploading to PyPi
 
 ```bash
 python3 -m build
 python3 -m twine upload --repository testpypi dist/*
 ```
 
 ## Official Addons/Plugins
 
 Here's a list of official addons:
+
 ### [otf-addons-aws](https://github.com/adammcdonagh/otf-addons-aws)
 
 Provides transfer and execution addons:
-   * Remote handler for interacting with AWS S3 buckets
-   * Remote handler for executing AWS Lambda functions
+
+- Remote handler for interacting with AWS S3 buckets
+- Remote handler for executing AWS Lambda functions
 
 Lookup plugins:
-   * Support for AWS SSM Parameter Store for retrieving global variables
+
+- Support for AWS SSM Parameter Store for retrieving global variables
 
 ## Developing your own addon/plugin
 
 ### Lookup Plugins
 
 Plugins are very simple. They simply need a `run` function, and to return the required variable based on a list of kwargs provided within the config template.
```

### Comparing `opentaskpy-0.8.1/src/opentaskpy/cli/task_run.py` & `opentaskpy-0.9.0/src/opentaskpy/cli/task_run.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,41 +1,47 @@
 #!/bin/env python3
+"""CLI script wrapper for handling env vars and triggering the TaskRun class."""
 
 import argparse
 import logging
 import os
+import sys
 from datetime import datetime
 
-from opentaskpy import task_run
-from opentaskpy.logging import OTF_LOG_FORMAT
+from opentaskpy import taskrun  # type: ignore[attr-defined]
+from opentaskpy.otflogging import OTF_LOG_FORMAT
 
 CONFIG_PATH = f"{os.getcwd()}/cfg"
 
 
-def main():
+def main() -> None:
+    """Parse args and call TaskRun class."""
     parser = argparse.ArgumentParser()
     parser.add_argument(
         "-t", "--taskId", help="Name of the JSON config to run", type=str, required=True
     )
     parser.add_argument(
         "-r",
         "--runId",
-        help="Unique identifier to correlate logs with. e.g. if being triggered by an external scheduler",
+        help=(
+            "Unique identifier to correlate logs with. e.g. if being triggered by an"
+            " external scheduler"
+        ),
         type=str,
         required=False,
     )
     parser.add_argument("-v", "--verbosity", help="Increase verbosity", type=int)
     parser.add_argument(
         "-c", "--configDir", help="Directory containing task configurations", type=str
     )
 
     args = parser.parse_args()
 
     if args.configDir:
-        global CONFIG_PATH
+        global CONFIG_PATH  # pylint: disable=global-statement
         CONFIG_PATH = args.configDir
 
     # If given a runId, then set the environment variable
     if args.runId:
         os.environ["OTF_RUN_ID"] = args.runId
 
     os.environ["OTF_LOG_RUN_PREFIX"] = datetime.now().strftime("%Y%m%d-%H%M%S.%f")
@@ -60,20 +66,20 @@
     logger = logging.getLogger()
     logger.setLevel(logging_level)
 
     logger = logging.getLogger(__name__)
     logger.log(11, f"Log verbosity: {args.verbosity}")
 
     # Create the TaskRun object
-    task_run_obj = task_run.TaskRun(args.taskId, CONFIG_PATH)
+    task_run_obj = taskrun.TaskRun(args.taskId, CONFIG_PATH)
 
     try:
         task_run_obj.run()
-    except Exception as e:
-        logger.error(f"Error running task: {e}")
+    except Exception as ex:  # pylint: disable=broad-exception-caught
+        logger.error(f"Error running task: {ex}")
         if logger.getEffectiveLevel() <= 12:
-            raise e
-        os._exit(1)
+            raise ex
+        sys.exit(1)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `opentaskpy-0.8.1/src/opentaskpy/config/loader.py` & `opentaskpy-0.9.0/src/opentaskpy/config/loader.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,55 +1,96 @@
+"""Config loader."""
 import datetime
 import importlib
 import json
 import os
 import sys
 from glob import glob
 
 import jinja2
 
-import opentaskpy.logging
-from opentaskpy.exceptions import DuplicateConfigFileError
+import opentaskpy.otflogging
+from opentaskpy.exceptions import (
+    DuplicateConfigFileError,
+    VariableResolutionTooDeepError,
+)
 
 MAX_DEPTH = 5
 
 
 class ConfigLoader:
-    def __init__(self, config_dir):
-        self.logger = opentaskpy.logging.init_logging(__name__)
+    """Class responsible for loading and validating config files."""
+
+    def __init__(self, config_dir: str) -> None:
+        """Parse config files and expand variables.
+
+        Args:
+            config_dir (str): The path to the config files to load.
+        """
+        self.logger = opentaskpy.otflogging.init_logging(__name__)
         self.config_dir = config_dir
-        self.template_env = None
-        self.global_variables = dict()
+        self.global_variables: dict = {}
 
         self.logger.log(12, f"Looking in {self.config_dir}")
 
         # Force Jinja2 to log undefined variables
-        jinja2.make_logging_undefined(logger=self.logger, base=jinja2.Undefined)  # noqa
+        jinja2.make_logging_undefined(logger=self.logger, base=jinja2.Undefined)
         self.template_env = jinja2.Environment(undefined=jinja2.StrictUndefined)
         self.template_env.filters["delta_days"] = self.delta_days
 
         self._load_global_variables()
         self._resolve_templated_variables()
 
-    def get_global_variables(self):
+    def get_global_variables(self) -> dict:
+        """Return the set of global variables that have been assigned via config files.
+
+        This will first check for anything that has been overridden in the environment
+        first, and replace those if necessary.
+
+        Returns:
+            dict: _description_
+        """
         # Before we return the variables, we need to check for any environment variables that match the same name, and are set
         # if this is the case, then we replace the value with the environment variable
         for key, _ in self.global_variables.items():
             if key in os.environ:
                 self.logger.info(
-                    f"Overriding global variable ({key}: {self.global_variables[key]}) with environment variable ({os.environ[key]})"
+                    f"Overriding global variable ({key}: {self.global_variables[key]})"
+                    f" with environment variable ({os.environ[key]})"
                 )
                 self.global_variables[key] = os.environ[key]
 
         return self.global_variables
 
-    def delta_days(self, value, days):
+    def delta_days(self, value: datetime.datetime, days: int) -> datetime.datetime:
+        """Returns a new datetime object + or - the number of delta days.
+
+        Args:
+            value (datetime.datetime): Starting datetime object
+            days (int): Days to increment or decrement the value
+
+        Returns:
+            datetime.datetime: New datetime object with the delta applied
+        """
         return value + datetime.timedelta(days)
 
-    def template_lookup(self, plugin, **kwargs):
+    def template_lookup(self, plugin: str, **kwargs) -> str:  # type: ignore[no-untyped-def]
+        """Lookup function used by Jinja.
+
+        This function is responsible for calling the lookup plugins to evaluate custom
+        variables. This imports the necessary Python module and calls the lookup
+        function's run method.
+
+        Args:
+            plugin (str): The name of the plugin to call
+            **kwargs: The arguments to pass to the plugin
+
+        Returns:
+            str: The result of the lookup plugin
+        """
         self.logger.log(
             11, f"Got call to lookup function {plugin} with kwargs {kwargs}"
         )
 
         # Append the globals to the kwargs
         kwargs["globals"] = self.global_variables
 
@@ -57,36 +98,53 @@
         if f"opentaskpy.plugins.lookup.{plugin}" not in sys.modules:
             # Check the module is loadable
             try:
                 importlib.import_module(f"opentaskpy.plugins.lookup.{plugin}")
             except ModuleNotFoundError:
                 self.logger.log(
                     11,
-                    f"Module not found: opentaskpy.plugins.lookup.{plugin}. Looking in plugins directory instead",
+                    (
+                        f"Module not found: opentaskpy.plugins.lookup.{plugin}. Looking"
+                        " in plugins directory instead"
+                    ),
                 )
-                pass
 
         # If we haven't loaded the plugin yet, then look in the cfg/plugins directory and see if we can find it
         if f"opentaskpy.plugins.lookup.{plugin}" not in sys.modules:
-            plugin_path = f"{self.config_dir}/plugins/{plugin}.py"
+            plugin_path = f"{self.config_dir}/plugins/lookup/{plugin}.py"
             if os.path.isfile(plugin_path):
-                spec = importlib.util.spec_from_file_location(
+                spec = importlib.util.spec_from_file_location(  # type: ignore[attr-defined]
                     f"opentaskpy.plugins.lookup.{plugin}", plugin_path
                 )
-                module = importlib.util.module_from_spec(spec)
+                module = importlib.util.module_from_spec(spec)  # type: ignore[attr-defined]
                 spec.loader.exec_module(module)
                 sys.modules[f"opentaskpy.plugins.lookup.{plugin}"] = module
 
         # Run the run function of the imported module
-        return getattr(  # noqa: B009
-            sys.modules[f"opentaskpy.plugins.lookup.{plugin}"], "run"
-        )(**kwargs)
+        return str(
+            getattr(  # noqa: B009
+                sys.modules[f"opentaskpy.plugins.lookup.{plugin}"], "run"
+            )(**kwargs)
+        )
 
     # TASK DEFINITION FIND FILE
-    def load_task_definition(self, task_id):
+    def load_task_definition(self, task_id: str) -> dict:
+        """Load the task definition from the config directory.
+
+        Args:
+            task_id (str): The id of the task to load
+
+        Raises:
+            DuplicateConfigFileError: Raised if more than one config file is found
+            matching the task_id
+            FileNotFoundError: Raised if no config file is found matching the task_id
+
+        Returns:
+            dict: A dictionary representing the task definition
+        """
         json_config = glob(f"{self.config_dir}/**/{task_id}.json", recursive=True)
         if not json_config or len(json_config) != 1:
             if len(json_config) > 1:
                 raise DuplicateConfigFileError(
                     f"Found more than one task with name: {task_id}"
                 )
 
@@ -101,15 +159,15 @@
         if "variables" in task_definition:
             for key, _ in task_definition["variables"].items():
                 if key in os.environ:
                     task_definition["variables"][key] = os.environ[key]
 
         # Check to see if this is not a batch type
         if "type" in task_definition and task_definition["type"] == "batch":
-            self.logger.warn("Cannot apply overrides to batch tasks. Ignoring")
+            self.logger.warning("Cannot apply overrides to batch tasks. Ignoring")
             return task_definition
 
         # Finally, attributes of the task definition can also be overridden by environment variables
         # e.g. OTF_OVERRIDE_TRANSFER_SOURCE_HOSTNAME will override ["source"]["hostname"], we need to handle this
         # The format is OTF_OVERRIDE_<TASK_TYPE>_<ATTRIBUTE>_<ATTRIBUTE>_<ATTRIBUTE>
         # e.g. OTF_OVERRIDE_TRANSFER_SOURCE_HOSTNAME
         for key, value in os.environ.items():
@@ -121,16 +179,16 @@
                 self._apply_env_var_overrides_to_task_definition(
                     task_definition, split_key, value
                 )
 
         return task_definition
 
     def _apply_env_var_overrides_to_task_definition(
-        self, task_definition, split_key, value
-    ):
+        self, task_definition: dict, split_key: str, value: str
+    ) -> None:
         attribute = split_key[0]
 
         # Match the attribute, to an attribute in the task_definition, bearing in mind that the case may not match
         # e.g. "source" may be "Source"
         for task_definition_attribute in task_definition:
             if task_definition_attribute.lower() == attribute.lower():
                 attribute = task_definition_attribute
@@ -155,17 +213,17 @@
         else:
             self._apply_env_var_overrides_to_task_definition(
                 task_definition[attribute], split_key[1:], value
             )
 
     # POPULATE VARIABLES INSIDE TASK DEFINITION
     # AND LOAD ADDITIONAL VARIABLES FROM TASK DEFINITION
-    def _enrich_variables(self, task_definition_file):
+    def _enrich_variables(self, task_definition_file: str) -> dict:
         active_task_definition = None
-        with open(task_definition_file) as json_file:
+        with open(task_definition_file, encoding="utf-8") as json_file:
             json_content = json_file.read()
             template = self.template_env.from_string(json_content)
 
             # From this, convert it to JSON and pull out the variables key if there is one
             task_definition = json.loads(json_content)
             # Extend or replace any local variables for this task
             if "variables" in task_definition:
@@ -177,48 +235,47 @@
 
             template.globals["now"] = datetime.datetime.utcnow
 
             # Define lookup function
             template.globals["lookup"] = self.template_lookup
 
             rendered_template = template.render(self.global_variables)
-            active_task_definition = json.loads(rendered_template)
+            active_task_definition = dict(json.loads(rendered_template))
             self.logger.log(
                 12, f"Evaluated task definition: {json.dumps(active_task_definition)}"
             )
 
         return active_task_definition
 
     # READ AND PARSE ACTUAL VARIABLE FILES
-    def _load_global_variables(self):
-        global_variables = dict()
+    def _load_global_variables(self) -> None:
+        global_variables: dict = {}
         variable_configs = []
         file_types = (".json.j2", ".json")
         for file_type in file_types:
             variable_configs.extend(
                 glob(f"{self.config_dir}/**/variables{file_type}", recursive=True)
             )
         if not variable_configs:
-            # self.logger.error("Couldn't find any variables.(json|json.j2) files")
             raise FileNotFoundError(
-                f"Couldn't find any variables.(json|json.j2) files under {self.config_dir}"
+                "Couldn't find any variables.(json|json.j2) files under"
+                f" {self.config_dir}"
             )
-        else:
-            for variable_file in variable_configs:
-                with open(variable_file) as json_file:
-                    this_variable_config = json.load(json_file)
-                    global_variables = global_variables | this_variable_config
+
+        for variable_file in variable_configs:
+            with open(variable_file, encoding="utf-8") as json_file:
+                this_variable_config = json.load(json_file)
+                global_variables = global_variables | this_variable_config
 
         self.global_variables = global_variables
 
     # RESOLVE ANY VARIABLES THAT USE OTHER VARIABLES IN THE VARIABLE FILES
-    def _resolve_templated_variables(self):
-        # We need to evaluate the variables themselves, incase theres any recursion
+    def _resolve_templated_variables(self) -> None:
+        # We need to evaluate the variables themselves, in case there's any recursion
         # Convert the variables to a JSON string which we can process with the jinja2 templater
-        global MAX_DEPTH
         current_depth = 0
         previous_render = None
 
         template = self.global_variables
 
         variables_template = self.template_env.from_string(json.dumps(template))
         variables_template.globals["now"] = datetime.datetime.utcnow
@@ -235,12 +292,15 @@
             evaluated_variables = variables_template.render(
                 json.loads(evaluated_variables)
             )
 
             current_depth += 1
             if current_depth >= MAX_DEPTH:
                 self.logger.error(
-                    "Reached max depth of recursive template evaluation. Please check the task as variable definitions for infinite recursion"
+                    "Reached max depth of recursive template evaluation. Please check"
+                    " the task as variable definitions for infinite recursion"
+                )
+                raise VariableResolutionTooDeepError(
+                    "Reached max depth of recursive template evaluation"
                 )
-                raise Exception("Reached max depth of recursive template evaluation")
 
         self.global_variables = json.loads(evaluated_variables)
```

### Comparing `opentaskpy-0.8.1/src/opentaskpy/config/schemas/batch.json` & `opentaskpy-0.9.0/src/opentaskpy/config/schemas/batch.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 4% similar despite different names*

```diff
@@ -95,10 +95,9 @@
 000005e0: 207b 0a20 2020 2020 2020 2022 7479 7065   {.        "type
 000005f0: 223a 2022 696e 7465 6765 7222 2c0a 2020  ": "integer",.  
 00000600: 2020 2020 2020 226d 696e 696d 756d 223a        "minimum":
 00000610: 2031 0a20 2020 2020 207d 0a20 2020 207d   1.      }.    }
 00000620: 0a20 207d 2c0a 2020 2261 6464 6974 696f  .  },.  "additio
 00000630: 6e61 6c50 726f 7065 7274 6965 7322 3a20  nalProperties": 
 00000640: 6661 6c73 652c 0a20 2022 7265 7175 6972  false,.  "requir
-00000650: 6564 223a 205b 0a20 2020 2022 6f72 6465  ed": [.    "orde
-00000660: 725f 6964 222c 0a20 2020 2022 7461 736b  r_id",.    "task
-00000670: 5f69 6422 0a20 205d 0a7d 0a              _id".  ].}.
+00000650: 6564 223a 205b 226f 7264 6572 5f69 6422  ed": ["order_id"
+00000660: 2c20 2274 6173 6b5f 6964 225d 0a7d 0a    , "task_id"].}.
```

### Comparing `opentaskpy-0.8.1/src/opentaskpy/config/schemas/transfer/email/protocol.json` & `opentaskpy-0.9.0/src/opentaskpy/config/schemas/transfer/email/protocol.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 8% similar despite different names*

```diff
@@ -1,48 +1,45 @@
 00000000: 7b0a 2020 2274 7970 6522 3a20 226f 626a  {.  "type": "obj
 00000010: 6563 7422 2c0a 2020 2270 726f 7065 7274  ect",.  "propert
 00000020: 6965 7322 3a20 7b0a 2020 2020 226e 616d  ies": {.    "nam
 00000030: 6522 3a20 7b0a 2020 2020 2020 2274 7970  e": {.      "typ
 00000040: 6522 3a20 2273 7472 696e 6722 2c0a 2020  e": "string",.  
-00000050: 2020 2020 2265 6e75 6d22 3a20 5b0a 2020      "enum": [.  
-00000060: 2020 2020 2020 2265 6d61 696c 220a 2020        "email".  
-00000070: 2020 2020 5d0a 2020 2020 7d2c 0a20 2020      ].    },.   
-00000080: 2022 736d 7470 5f70 6f72 7422 3a20 7b0a   "smtp_port": {.
-00000090: 2020 2020 2020 2274 7970 6522 3a20 226e        "type": "n
-000000a0: 756d 6265 7222 2c0a 2020 2020 2020 226d  umber",.      "m
-000000b0: 696e 696d 756d 223a 2031 2c0a 2020 2020  inimum": 1,.    
-000000c0: 2020 226d 6178 696d 756d 223a 2036 3535    "maximum": 655
-000000d0: 3335 0a20 2020 207d 2c0a 2020 2020 2273  35.    },.    "s
-000000e0: 6d74 705f 7365 7276 6572 223a 207b 0a20  mtp_server": {. 
-000000f0: 2020 2020 2022 7479 7065 223a 2022 7374       "type": "st
-00000100: 7269 6e67 220a 2020 2020 7d2c 0a20 2020  ring".    },.   
-00000110: 2022 7365 6e64 6572 223a 207b 0a20 2020   "sender": {.   
-00000120: 2020 2022 7479 7065 223a 2022 7374 7269     "type": "stri
-00000130: 6e67 222c 0a20 2020 2020 2022 7061 7474  ng",.      "patt
-00000140: 6572 6e22 3a20 225e 282e 2a3f 5c5c 732b  ern": "^(.*?\\s+
-00000150: 3c29 3f5b 5c5c 772e 2d5d 2b40 5b5c 5c77  <)?[\\w.-]+@[\\w
-00000160: 2e2d 5d2b 5c5c 2e5b 612d 7a41 2d5a 5d7b  .-]+\\.[a-zA-Z]{
-00000170: 322c 367d 283e 3f29 2422 0a20 2020 207d  2,6}(>?)$".    }
-00000180: 2c0a 2020 2020 2263 7265 6465 6e74 6961  ,.    "credentia
-00000190: 6c73 223a 207b 0a20 2020 2020 2022 7479  ls": {.      "ty
-000001a0: 7065 223a 2022 6f62 6a65 6374 222c 0a20  pe": "object",. 
-000001b0: 2020 2020 2022 7072 6f70 6572 7469 6573       "properties
-000001c0: 223a 207b 0a20 2020 2020 2020 2022 7573  ": {.        "us
-000001d0: 6572 6e61 6d65 223a 207b 0a20 2020 2020  ername": {.     
-000001e0: 2020 2020 2022 7479 7065 223a 2022 7374       "type": "st
-000001f0: 7269 6e67 220a 2020 2020 2020 2020 7d2c  ring".        },
-00000200: 0a20 2020 2020 2020 2022 7061 7373 776f  .        "passwo
-00000210: 7264 223a 207b 0a20 2020 2020 2020 2020  rd": {.         
-00000220: 2022 7479 7065 223a 2022 7374 7269 6e67   "type": "string
-00000230: 220a 2020 2020 2020 2020 7d0a 2020 2020  ".        }.    
-00000240: 2020 7d2c 0a20 2020 2020 2022 7265 7175    },.      "requ
-00000250: 6972 6564 223a 205b 0a20 2020 2020 2020  ired": [.       
-00000260: 2022 7573 6572 6e61 6d65 222c 0a20 2020   "username",.   
-00000270: 2020 2020 2022 7061 7373 776f 7264 220a       "password".
-00000280: 2020 2020 2020 5d2c 0a20 2020 2020 2022        ],.      "
-00000290: 6164 6469 7469 6f6e 616c 5072 6f70 6572  additionalProper
-000002a0: 7469 6573 223a 2066 616c 7365 0a20 2020  ties": false.   
-000002b0: 207d 0a20 207d 2c0a 2020 2272 6571 7569   }.  },.  "requi
-000002c0: 7265 6422 3a20 5b0a 2020 2020 226e 616d  red": [.    "nam
-000002d0: 6522 0a20 205d 2c0a 2020 2261 6464 6974  e".  ],.  "addit
-000002e0: 696f 6e61 6c50 726f 7065 7274 6965 7322  ionalProperties"
-000002f0: 3a20 6661 6c73 650a 7d0a                 : false.}.
+00000050: 2020 2020 2265 6e75 6d22 3a20 5b22 656d      "enum": ["em
+00000060: 6169 6c22 5d0a 2020 2020 7d2c 0a20 2020  ail"].    },.   
+00000070: 2022 736d 7470 5f70 6f72 7422 3a20 7b0a   "smtp_port": {.
+00000080: 2020 2020 2020 2274 7970 6522 3a20 226e        "type": "n
+00000090: 756d 6265 7222 2c0a 2020 2020 2020 226d  umber",.      "m
+000000a0: 696e 696d 756d 223a 2031 2c0a 2020 2020  inimum": 1,.    
+000000b0: 2020 226d 6178 696d 756d 223a 2036 3535    "maximum": 655
+000000c0: 3335 0a20 2020 207d 2c0a 2020 2020 2273  35.    },.    "s
+000000d0: 6d74 705f 7365 7276 6572 223a 207b 0a20  mtp_server": {. 
+000000e0: 2020 2020 2022 7479 7065 223a 2022 7374       "type": "st
+000000f0: 7269 6e67 220a 2020 2020 7d2c 0a20 2020  ring".    },.   
+00000100: 2022 7365 6e64 6572 223a 207b 0a20 2020   "sender": {.   
+00000110: 2020 2022 7479 7065 223a 2022 7374 7269     "type": "stri
+00000120: 6e67 222c 0a20 2020 2020 2022 7061 7474  ng",.      "patt
+00000130: 6572 6e22 3a20 225e 282e 2a3f 5c5c 732b  ern": "^(.*?\\s+
+00000140: 3c29 3f5b 5c5c 772e 2d5d 2b40 5b5c 5c77  <)?[\\w.-]+@[\\w
+00000150: 2e2d 5d2b 5c5c 2e5b 612d 7a41 2d5a 5d7b  .-]+\\.[a-zA-Z]{
+00000160: 322c 367d 283e 3f29 2422 0a20 2020 207d  2,6}(>?)$".    }
+00000170: 2c0a 2020 2020 2263 7265 6465 6e74 6961  ,.    "credentia
+00000180: 6c73 223a 207b 0a20 2020 2020 2022 7479  ls": {.      "ty
+00000190: 7065 223a 2022 6f62 6a65 6374 222c 0a20  pe": "object",. 
+000001a0: 2020 2020 2022 7072 6f70 6572 7469 6573       "properties
+000001b0: 223a 207b 0a20 2020 2020 2020 2022 7573  ": {.        "us
+000001c0: 6572 6e61 6d65 223a 207b 0a20 2020 2020  ername": {.     
+000001d0: 2020 2020 2022 7479 7065 223a 2022 7374       "type": "st
+000001e0: 7269 6e67 220a 2020 2020 2020 2020 7d2c  ring".        },
+000001f0: 0a20 2020 2020 2020 2022 7061 7373 776f  .        "passwo
+00000200: 7264 223a 207b 0a20 2020 2020 2020 2020  rd": {.         
+00000210: 2022 7479 7065 223a 2022 7374 7269 6e67   "type": "string
+00000220: 220a 2020 2020 2020 2020 7d0a 2020 2020  ".        }.    
+00000230: 2020 7d2c 0a20 2020 2020 2022 7265 7175    },.      "requ
+00000240: 6972 6564 223a 205b 2275 7365 726e 616d  ired": ["usernam
+00000250: 6522 2c20 2270 6173 7377 6f72 6422 5d2c  e", "password"],
+00000260: 0a20 2020 2020 2022 6164 6469 7469 6f6e  .      "addition
+00000270: 616c 5072 6f70 6572 7469 6573 223a 2066  alProperties": f
+00000280: 616c 7365 0a20 2020 207d 0a20 207d 2c0a  alse.    }.  },.
+00000290: 2020 2272 6571 7569 7265 6422 3a20 5b22    "required": ["
+000002a0: 6e61 6d65 225d 2c0a 2020 2261 6464 6974  name"],.  "addit
+000002b0: 696f 6e61 6c50 726f 7065 7274 6965 7322  ionalProperties"
+000002c0: 3a20 6661 6c73 650a 7d0a                 : false.}.
```

### Comparing `opentaskpy-0.8.1/src/opentaskpy/config/schemas/transfer/ssh_destination/protocol.json` & `opentaskpy-0.9.0/src/opentaskpy/config/schemas/transfer/ssh_destination/protocol.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 4% similar despite different names*

```diff
@@ -1,36 +1,33 @@
 00000000: 7b0a 2020 2274 7970 6522 3a20 226f 626a  {.  "type": "obj
 00000010: 6563 7422 2c0a 2020 2270 726f 7065 7274  ect",.  "propert
 00000020: 6965 7322 3a20 7b0a 2020 2020 226e 616d  ies": {.    "nam
 00000030: 6522 3a20 7b0a 2020 2020 2020 2274 7970  e": {.      "typ
 00000040: 6522 3a20 2273 7472 696e 6722 2c0a 2020  e": "string",.  
-00000050: 2020 2020 2265 6e75 6d22 3a20 5b0a 2020      "enum": [.  
-00000060: 2020 2020 2020 2273 7368 220a 2020 2020        "ssh".    
-00000070: 2020 5d0a 2020 2020 7d2c 0a20 2020 2022    ].    },.    "
-00000080: 6372 6564 656e 7469 616c 7322 3a20 7b0a  credentials": {.
-00000090: 2020 2020 2020 2274 7970 6522 3a20 226f        "type": "o
-000000a0: 626a 6563 7422 2c0a 2020 2020 2020 2270  bject",.      "p
-000000b0: 726f 7065 7274 6965 7322 3a20 7b0a 2020  roperties": {.  
-000000c0: 2020 2020 2020 2275 7365 726e 616d 6522        "username"
-000000d0: 3a20 7b0a 2020 2020 2020 2020 2020 2274  : {.          "t
-000000e0: 7970 6522 3a20 2273 7472 696e 6722 0a20  ype": "string". 
-000000f0: 2020 2020 2020 207d 2c0a 2020 2020 2020         },.      
-00000100: 2020 2274 7261 6e73 6665 7255 7365 726e    "transferUsern
-00000110: 616d 6522 3a20 7b0a 2020 2020 2020 2020  ame": {.        
-00000120: 2020 2274 7970 6522 3a20 2273 7472 696e    "type": "strin
-00000130: 6722 0a20 2020 2020 2020 207d 2c0a 2020  g".        },.  
-00000140: 2020 2020 2020 226b 6579 4669 6c65 223a        "keyFile":
-00000150: 207b 0a20 2020 2020 2020 2020 2022 7479   {.          "ty
-00000160: 7065 223a 2022 7374 7269 6e67 220a 2020  pe": "string".  
-00000170: 2020 2020 2020 7d0a 2020 2020 2020 7d2c        }.      },
-00000180: 0a20 2020 2020 2022 7265 7175 6972 6564  .      "required
-00000190: 223a 205b 0a20 2020 2020 2020 2022 7573  ": [.        "us
-000001a0: 6572 6e61 6d65 220a 2020 2020 2020 5d2c  ername".      ],
-000001b0: 0a20 2020 2020 2022 6164 6469 7469 6f6e  .      "addition
-000001c0: 616c 5072 6f70 6572 7469 6573 223a 2066  alProperties": f
-000001d0: 616c 7365 0a20 2020 207d 0a20 207d 2c0a  alse.    }.  },.
-000001e0: 2020 2272 6571 7569 7265 6422 3a20 5b0a    "required": [.
-000001f0: 2020 2020 226e 616d 6522 2c0a 2020 2020      "name",.    
-00000200: 2263 7265 6465 6e74 6961 6c73 220a 2020  "credentials".  
-00000210: 5d2c 0a20 2022 6164 6469 7469 6f6e 616c  ],.  "additional
-00000220: 5072 6f70 6572 7469 6573 223a 2066 616c  Properties": fal
-00000230: 7365 0a7d 0a                             se.}.
+00000050: 2020 2020 2265 6e75 6d22 3a20 5b22 7373      "enum": ["ss
+00000060: 6822 5d0a 2020 2020 7d2c 0a20 2020 2022  h"].    },.    "
+00000070: 6372 6564 656e 7469 616c 7322 3a20 7b0a  credentials": {.
+00000080: 2020 2020 2020 2274 7970 6522 3a20 226f        "type": "o
+00000090: 626a 6563 7422 2c0a 2020 2020 2020 2270  bject",.      "p
+000000a0: 726f 7065 7274 6965 7322 3a20 7b0a 2020  roperties": {.  
+000000b0: 2020 2020 2020 2275 7365 726e 616d 6522        "username"
+000000c0: 3a20 7b0a 2020 2020 2020 2020 2020 2274  : {.          "t
+000000d0: 7970 6522 3a20 2273 7472 696e 6722 0a20  ype": "string". 
+000000e0: 2020 2020 2020 207d 2c0a 2020 2020 2020         },.      
+000000f0: 2020 2274 7261 6e73 6665 7255 7365 726e    "transferUsern
+00000100: 616d 6522 3a20 7b0a 2020 2020 2020 2020  ame": {.        
+00000110: 2020 2274 7970 6522 3a20 2273 7472 696e    "type": "strin
+00000120: 6722 0a20 2020 2020 2020 207d 2c0a 2020  g".        },.  
+00000130: 2020 2020 2020 226b 6579 4669 6c65 223a        "keyFile":
+00000140: 207b 0a20 2020 2020 2020 2020 2022 7479   {.          "ty
+00000150: 7065 223a 2022 7374 7269 6e67 220a 2020  pe": "string".  
+00000160: 2020 2020 2020 7d0a 2020 2020 2020 7d2c        }.      },
+00000170: 0a20 2020 2020 2022 7265 7175 6972 6564  .      "required
+00000180: 223a 205b 2275 7365 726e 616d 6522 5d2c  ": ["username"],
+00000190: 0a20 2020 2020 2022 6164 6469 7469 6f6e  .      "addition
+000001a0: 616c 5072 6f70 6572 7469 6573 223a 2066  alProperties": f
+000001b0: 616c 7365 0a20 2020 207d 0a20 207d 2c0a  alse.    }.  },.
+000001c0: 2020 2272 6571 7569 7265 6422 3a20 5b22    "required": ["
+000001d0: 6e61 6d65 222c 2022 6372 6564 656e 7469  name", "credenti
+000001e0: 616c 7322 5d2c 0a20 2022 6164 6469 7469  als"],.  "additi
+000001f0: 6f6e 616c 5072 6f70 6572 7469 6573 223a  onalProperties":
+00000200: 2066 616c 7365 0a7d 0a                    false.}.
```

### Comparing `opentaskpy-0.8.1/src/opentaskpy/config/schemas/transfer/ssh_destination.json` & `opentaskpy-0.9.0/src/opentaskpy/config/schemas/transfer/ssh_source.json`

 * *Files 20% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8370535714285714%*

 * *Differences: {"'properties'": "{'protocol': {'$ref': 'ssh_source/protocol.json'}, 'fileRegex': "*

 * *                 "OrderedDict([('type', 'string')]), 'conditionals': OrderedDict([('$ref', "*

 * *                 "'ssh_source/conditionals.json')]), 'fileWatch': OrderedDict([('$ref', "*

 * *                 "'ssh_source/fileWatch.json')]), 'logWatch': OrderedDict([('$ref', "*

 * *                 "'ssh_source/logWatch.json')]), 'error': OrderedDict([('type', 'boolean')]), "*

 * *                 "'postCopyAction': OrderedDict([('$ref', 'ssh_ […]*

```diff
@@ -1,40 +1,38 @@
 {
     "additionalProperties": false,
     "properties": {
+        "conditionals": {
+            "$ref": "ssh_source/conditionals.json"
+        },
         "directory": {
             "type": "string"
         },
-        "flags": {
-            "$ref": "ssh_destination/flags.json"
+        "error": {
+            "type": "boolean"
         },
-        "hostname": {
+        "fileRegex": {
             "type": "string"
         },
-        "mode": {
-            "type": "string"
+        "fileWatch": {
+            "$ref": "ssh_source/fileWatch.json"
         },
-        "permissions": {
-            "$ref": "ssh_destination/permissions.json"
+        "hostname": {
+            "type": "string"
         },
-        "protocol": {
-            "$ref": "ssh_destination/protocol.json"
+        "logWatch": {
+            "$ref": "ssh_source/logWatch.json"
         },
-        "rename": {
-            "$ref": "ssh_destination/rename.json"
+        "postCopyAction": {
+            "$ref": "ssh_source/postCopyAction.json"
         },
-        "transferType": {
-            "enum": [
-                "push",
-                "pull",
-                "proxy"
-            ],
-            "type": "string"
+        "protocol": {
+            "$ref": "ssh_source/protocol.json"
         }
     },
     "required": [
         "hostname",
-        "directory",
+        "fileRegex",
         "protocol"
     ],
     "type": "object"
 }
```

### Comparing `opentaskpy-0.8.1/src/opentaskpy/config/schemas/transfer/ssh_source/conditionals.json` & `opentaskpy-0.9.0/src/opentaskpy/config/schemas/transfer/ssh_source/conditionals.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 19% similar despite different names*

```diff
@@ -10,46 +10,40 @@
 00000090: 2020 2020 2020 2020 7d2c 0a20 2020 2020          },.     
 000000a0: 2020 2022 6c74 223a 207b 0a20 2020 2020     "lt": {.     
 000000b0: 2020 2020 2022 7479 7065 223a 2022 696e       "type": "in
 000000c0: 7465 6765 7222 0a20 2020 2020 2020 207d  teger".        }
 000000d0: 0a20 2020 2020 207d 2c0a 2020 2020 2020  .      },.      
 000000e0: 2261 6e79 4f66 223a 205b 0a20 2020 2020  "anyOf": [.     
 000000f0: 2020 207b 0a20 2020 2020 2020 2020 2022     {.          "
-00000100: 7265 7175 6972 6564 223a 205b 0a20 2020  required": [.   
-00000110: 2020 2020 2020 2020 2022 6774 220a 2020           "gt".  
-00000120: 2020 2020 2020 2020 5d0a 2020 2020 2020          ].      
-00000130: 2020 7d2c 0a20 2020 2020 2020 207b 0a20    },.        {. 
-00000140: 2020 2020 2020 2020 2022 7265 7175 6972           "requir
-00000150: 6564 223a 205b 0a20 2020 2020 2020 2020  ed": [.         
-00000160: 2020 2022 6c74 220a 2020 2020 2020 2020     "lt".        
-00000170: 2020 5d0a 2020 2020 2020 2020 7d0a 2020    ].        }.  
-00000180: 2020 2020 5d2c 0a20 2020 2020 2022 6164      ],.      "ad
-00000190: 6469 7469 6f6e 616c 5072 6f70 6572 7469  ditionalProperti
-000001a0: 6573 223a 2066 616c 7365 0a20 2020 207d  es": false.    }
-000001b0: 2c0a 2020 2020 2261 6765 223a 207b 0a20  ,.    "age": {. 
-000001c0: 2020 2020 2022 7479 7065 223a 2022 6f62       "type": "ob
-000001d0: 6a65 6374 222c 0a20 2020 2020 2022 7072  ject",.      "pr
-000001e0: 6f70 6572 7469 6573 223a 207b 0a20 2020  operties": {.   
-000001f0: 2020 2020 2022 6774 223a 207b 0a20 2020       "gt": {.   
-00000200: 2020 2020 2020 2022 7479 7065 223a 2022         "type": "
-00000210: 696e 7465 6765 7222 0a20 2020 2020 2020  integer".       
-00000220: 207d 2c0a 2020 2020 2020 2020 226c 7422   },.        "lt"
-00000230: 3a20 7b0a 2020 2020 2020 2020 2020 2274  : {.          "t
-00000240: 7970 6522 3a20 2269 6e74 6567 6572 220a  ype": "integer".
-00000250: 2020 2020 2020 2020 7d0a 2020 2020 2020          }.      
-00000260: 7d2c 0a20 2020 2020 2022 616e 794f 6622  },.      "anyOf"
-00000270: 3a20 5b0a 2020 2020 2020 2020 7b0a 2020  : [.        {.  
-00000280: 2020 2020 2020 2020 2272 6571 7569 7265          "require
-00000290: 6422 3a20 5b0a 2020 2020 2020 2020 2020  d": [.          
-000002a0: 2020 2267 7422 0a20 2020 2020 2020 2020    "gt".         
-000002b0: 205d 0a20 2020 2020 2020 207d 2c0a 2020   ].        },.  
-000002c0: 2020 2020 2020 7b0a 2020 2020 2020 2020        {.        
-000002d0: 2020 2272 6571 7569 7265 6422 3a20 5b0a    "required": [.
-000002e0: 2020 2020 2020 2020 2020 2020 226c 7422              "lt"
-000002f0: 0a20 2020 2020 2020 2020 205d 0a20 2020  .          ].   
-00000300: 2020 2020 207d 0a20 2020 2020 205d 2c0a       }.      ],.
-00000310: 2020 2020 2020 2261 6464 6974 696f 6e61        "additiona
-00000320: 6c50 726f 7065 7274 6965 7322 3a20 6661  lProperties": fa
-00000330: 6c73 650a 2020 2020 7d0a 2020 7d2c 0a20  lse.    }.  },. 
-00000340: 2022 6164 6469 7469 6f6e 616c 5072 6f70   "additionalProp
-00000350: 6572 7469 6573 223a 2066 616c 7365 0a7d  erties": false.}
-00000360: 0a                                       .
+00000100: 7265 7175 6972 6564 223a 205b 2267 7422  required": ["gt"
+00000110: 5d0a 2020 2020 2020 2020 7d2c 0a20 2020  ].        },.   
+00000120: 2020 2020 207b 0a20 2020 2020 2020 2020       {.         
+00000130: 2022 7265 7175 6972 6564 223a 205b 226c   "required": ["l
+00000140: 7422 5d0a 2020 2020 2020 2020 7d0a 2020  t"].        }.  
+00000150: 2020 2020 5d2c 0a20 2020 2020 2022 6164      ],.      "ad
+00000160: 6469 7469 6f6e 616c 5072 6f70 6572 7469  ditionalProperti
+00000170: 6573 223a 2066 616c 7365 0a20 2020 207d  es": false.    }
+00000180: 2c0a 2020 2020 2261 6765 223a 207b 0a20  ,.    "age": {. 
+00000190: 2020 2020 2022 7479 7065 223a 2022 6f62       "type": "ob
+000001a0: 6a65 6374 222c 0a20 2020 2020 2022 7072  ject",.      "pr
+000001b0: 6f70 6572 7469 6573 223a 207b 0a20 2020  operties": {.   
+000001c0: 2020 2020 2022 6774 223a 207b 0a20 2020       "gt": {.   
+000001d0: 2020 2020 2020 2022 7479 7065 223a 2022         "type": "
+000001e0: 696e 7465 6765 7222 0a20 2020 2020 2020  integer".       
+000001f0: 207d 2c0a 2020 2020 2020 2020 226c 7422   },.        "lt"
+00000200: 3a20 7b0a 2020 2020 2020 2020 2020 2274  : {.          "t
+00000210: 7970 6522 3a20 2269 6e74 6567 6572 220a  ype": "integer".
+00000220: 2020 2020 2020 2020 7d0a 2020 2020 2020          }.      
+00000230: 7d2c 0a20 2020 2020 2022 616e 794f 6622  },.      "anyOf"
+00000240: 3a20 5b0a 2020 2020 2020 2020 7b0a 2020  : [.        {.  
+00000250: 2020 2020 2020 2020 2272 6571 7569 7265          "require
+00000260: 6422 3a20 5b22 6774 225d 0a20 2020 2020  d": ["gt"].     
+00000270: 2020 207d 2c0a 2020 2020 2020 2020 7b0a     },.        {.
+00000280: 2020 2020 2020 2020 2020 2272 6571 7569            "requi
+00000290: 7265 6422 3a20 5b22 6c74 225d 0a20 2020  red": ["lt"].   
+000002a0: 2020 2020 207d 0a20 2020 2020 205d 2c0a       }.      ],.
+000002b0: 2020 2020 2020 2261 6464 6974 696f 6e61        "additiona
+000002c0: 6c50 726f 7065 7274 6965 7322 3a20 6661  lProperties": fa
+000002d0: 6c73 650a 2020 2020 7d0a 2020 7d2c 0a20  lse.    }.  },. 
+000002e0: 2022 6164 6469 7469 6f6e 616c 5072 6f70   "additionalProp
+000002f0: 6572 7469 6573 223a 2066 616c 7365 0a7d  erties": false.}
+00000300: 0a                                       .
```

### Comparing `opentaskpy-0.8.1/src/opentaskpy/config/schemas/transfer/ssh_source/postCopyAction.json` & `opentaskpy-0.9.0/src/opentaskpy/config/schemas/transfer/ssh_source/postCopyAction.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 8% similar despite different names*

```diff
@@ -1,81 +1,70 @@
 00000000: 7b0a 2020 2274 7970 6522 3a20 226f 626a  {.  "type": "obj
 00000010: 6563 7422 2c0a 2020 2270 726f 7065 7274  ect",.  "propert
 00000020: 6965 7322 3a20 7b0a 2020 2020 2261 6374  ies": {.    "act
 00000030: 696f 6e22 3a20 7b0a 2020 2020 2020 2274  ion": {.      "t
 00000040: 7970 6522 3a20 2273 7472 696e 6722 2c0a  ype": "string",.
-00000050: 2020 2020 2020 2265 6e75 6d22 3a20 5b0a        "enum": [.
-00000060: 2020 2020 2020 2020 226d 6f76 6522 2c0a          "move",.
-00000070: 2020 2020 2020 2020 2272 656e 616d 6522          "rename"
-00000080: 2c0a 2020 2020 2020 2020 2264 656c 6574  ,.        "delet
-00000090: 6522 0a20 2020 2020 205d 0a20 2020 207d  e".      ].    }
-000000a0: 2c0a 2020 2020 2264 6573 7469 6e61 7469  ,.    "destinati
-000000b0: 6f6e 223a 207b 0a20 2020 2020 2022 7479  on": {.      "ty
-000000c0: 7065 223a 2022 7374 7269 6e67 220a 2020  pe": "string".  
-000000d0: 2020 7d2c 0a20 2020 2022 7375 6222 3a20    },.    "sub": 
-000000e0: 7b0a 2020 2020 2020 2274 7970 6522 3a20  {.      "type": 
-000000f0: 2273 7472 696e 6722 0a20 2020 207d 2c0a  "string".    },.
-00000100: 2020 2020 2270 6174 7465 726e 223a 207b      "pattern": {
-00000110: 0a20 2020 2020 2022 7479 7065 223a 2022  .      "type": "
-00000120: 7374 7269 6e67 220a 2020 2020 7d0a 2020  string".    }.  
-00000130: 7d2c 0a20 2022 7265 7175 6972 6564 223a  },.  "required":
-00000140: 205b 0a20 2020 2022 6163 7469 6f6e 220a   [.    "action".
-00000150: 2020 5d2c 0a20 2022 616c 6c4f 6622 3a20    ],.  "allOf": 
-00000160: 5b0a 2020 2020 7b0a 2020 2020 2020 2269  [.    {.      "i
-00000170: 6622 3a20 7b0a 2020 2020 2020 2020 2270  f": {.        "p
-00000180: 726f 7065 7274 6965 7322 3a20 7b0a 2020  roperties": {.  
-00000190: 2020 2020 2020 2020 2261 6374 696f 6e22          "action"
-000001a0: 3a20 7b0a 2020 2020 2020 2020 2020 2020  : {.            
-000001b0: 2265 6e75 6d22 3a20 5b0a 2020 2020 2020  "enum": [.      
-000001c0: 2020 2020 2020 2020 226d 6f76 6522 2c0a          "move",.
-000001d0: 2020 2020 2020 2020 2020 2020 2020 2272                "r
-000001e0: 656e 616d 6522 0a20 2020 2020 2020 2020  ename".         
-000001f0: 2020 205d 0a20 2020 2020 2020 2020 207d     ].          }
-00000200: 0a20 2020 2020 2020 207d 0a20 2020 2020  .        }.     
-00000210: 207d 2c0a 2020 2020 2020 2274 6865 6e22   },.      "then"
-00000220: 3a20 7b0a 2020 2020 2020 2020 2272 6571  : {.        "req
-00000230: 7569 7265 6422 3a20 5b0a 2020 2020 2020  uired": [.      
-00000240: 2020 2020 2261 6374 696f 6e22 2c0a 2020      "action",.  
-00000250: 2020 2020 2020 2020 2264 6573 7469 6e61          "destina
-00000260: 7469 6f6e 220a 2020 2020 2020 2020 5d0a  tion".        ].
-00000270: 2020 2020 2020 7d2c 0a20 2020 2020 2022        },.      "
-00000280: 656c 7365 223a 207b 0a20 2020 2020 2020  else": {.       
-00000290: 2022 7072 6f70 6572 7469 6573 223a 207b   "properties": {
-000002a0: 0a20 2020 2020 2020 2020 2022 6465 7374  .          "dest
-000002b0: 696e 6174 696f 6e22 3a20 7b0a 2020 2020  ination": {.    
-000002c0: 2020 2020 2020 2020 226e 6f74 223a 207b          "not": {
-000002d0: 7d0a 2020 2020 2020 2020 2020 7d0a 2020  }.          }.  
-000002e0: 2020 2020 2020 7d0a 2020 2020 2020 7d0a        }.      }.
-000002f0: 2020 2020 7d2c 0a20 2020 207b 0a20 2020      },.    {.   
-00000300: 2020 2022 6966 223a 207b 0a20 2020 2020     "if": {.     
-00000310: 2020 2022 7072 6f70 6572 7469 6573 223a     "properties":
-00000320: 207b 0a20 2020 2020 2020 2020 2022 6163   {.          "ac
-00000330: 7469 6f6e 223a 207b 0a20 2020 2020 2020  tion": {.       
-00000340: 2020 2020 2022 636f 6e73 7422 3a20 2272       "const": "r
-00000350: 656e 616d 6522 0a20 2020 2020 2020 2020  ename".         
-00000360: 207d 0a20 2020 2020 2020 207d 0a20 2020   }.        }.   
-00000370: 2020 207d 2c0a 2020 2020 2020 2274 6865     },.      "the
-00000380: 6e22 3a20 7b0a 2020 2020 2020 2020 2272  n": {.        "r
-00000390: 6571 7569 7265 6422 3a20 5b0a 2020 2020  equired": [.    
-000003a0: 2020 2020 2020 2273 7562 222c 0a20 2020        "sub",.   
-000003b0: 2020 2020 2020 2022 7061 7474 6572 6e22         "pattern"
-000003c0: 0a20 2020 2020 2020 205d 0a20 2020 2020  .        ].     
-000003d0: 207d 0a20 2020 207d 2c0a 2020 2020 7b0a   }.    },.    {.
-000003e0: 2020 2020 2020 2269 6622 3a20 7b0a 2020        "if": {.  
-000003f0: 2020 2020 2020 2270 726f 7065 7274 6965        "propertie
-00000400: 7322 3a20 7b0a 2020 2020 2020 2020 2020  s": {.          
-00000410: 2261 6374 696f 6e22 3a20 7b0a 2020 2020  "action": {.    
-00000420: 2020 2020 2020 2020 2263 6f6e 7374 223a          "const":
-00000430: 2022 6d6f 7665 220a 2020 2020 2020 2020   "move".        
-00000440: 2020 7d0a 2020 2020 2020 2020 7d0a 2020    }.        }.  
-00000450: 2020 2020 7d2c 0a20 2020 2020 2022 7468      },.      "th
-00000460: 656e 223a 207b 0a20 2020 2020 2020 2022  en": {.        "
-00000470: 6e6f 7422 3a20 7b0a 2020 2020 2020 2020  not": {.        
-00000480: 2020 2272 6571 7569 7265 6422 3a20 5b0a    "required": [.
-00000490: 2020 2020 2020 2020 2020 2020 2273 7562              "sub
-000004a0: 222c 0a20 2020 2020 2020 2020 2020 2022  ",.            "
-000004b0: 7061 7474 6572 6e22 0a20 2020 2020 2020  pattern".       
-000004c0: 2020 205d 0a20 2020 2020 2020 207d 0a20     ].        }. 
-000004d0: 2020 2020 207d 0a20 2020 207d 0a20 205d       }.    }.  ]
-000004e0: 2c0a 2020 2261 6464 6974 696f 6e61 6c50  ,.  "additionalP
-000004f0: 726f 7065 7274 6965 7322 3a20 6661 6c73  roperties": fals
-00000500: 650a 7d0a                                e.}.
+00000050: 2020 2020 2020 2265 6e75 6d22 3a20 5b22        "enum": ["
+00000060: 6d6f 7665 222c 2022 7265 6e61 6d65 222c  move", "rename",
+00000070: 2022 6465 6c65 7465 225d 0a20 2020 207d   "delete"].    }
+00000080: 2c0a 2020 2020 2264 6573 7469 6e61 7469  ,.    "destinati
+00000090: 6f6e 223a 207b 0a20 2020 2020 2022 7479  on": {.      "ty
+000000a0: 7065 223a 2022 7374 7269 6e67 220a 2020  pe": "string".  
+000000b0: 2020 7d2c 0a20 2020 2022 7375 6222 3a20    },.    "sub": 
+000000c0: 7b0a 2020 2020 2020 2274 7970 6522 3a20  {.      "type": 
+000000d0: 2273 7472 696e 6722 0a20 2020 207d 2c0a  "string".    },.
+000000e0: 2020 2020 2270 6174 7465 726e 223a 207b      "pattern": {
+000000f0: 0a20 2020 2020 2022 7479 7065 223a 2022  .      "type": "
+00000100: 7374 7269 6e67 220a 2020 2020 7d0a 2020  string".    }.  
+00000110: 7d2c 0a20 2022 7265 7175 6972 6564 223a  },.  "required":
+00000120: 205b 2261 6374 696f 6e22 5d2c 0a20 2022   ["action"],.  "
+00000130: 616c 6c4f 6622 3a20 5b0a 2020 2020 7b0a  allOf": [.    {.
+00000140: 2020 2020 2020 2269 6622 3a20 7b0a 2020        "if": {.  
+00000150: 2020 2020 2020 2270 726f 7065 7274 6965        "propertie
+00000160: 7322 3a20 7b0a 2020 2020 2020 2020 2020  s": {.          
+00000170: 2261 6374 696f 6e22 3a20 7b0a 2020 2020  "action": {.    
+00000180: 2020 2020 2020 2020 2265 6e75 6d22 3a20          "enum": 
+00000190: 5b22 6d6f 7665 222c 2022 7265 6e61 6d65  ["move", "rename
+000001a0: 225d 0a20 2020 2020 2020 2020 207d 0a20  "].          }. 
+000001b0: 2020 2020 2020 207d 0a20 2020 2020 207d         }.      }
+000001c0: 2c0a 2020 2020 2020 2274 6865 6e22 3a20  ,.      "then": 
+000001d0: 7b0a 2020 2020 2020 2020 2272 6571 7569  {.        "requi
+000001e0: 7265 6422 3a20 5b22 6163 7469 6f6e 222c  red": ["action",
+000001f0: 2022 6465 7374 696e 6174 696f 6e22 5d0a   "destination"].
+00000200: 2020 2020 2020 7d2c 0a20 2020 2020 2022        },.      "
+00000210: 656c 7365 223a 207b 0a20 2020 2020 2020  else": {.       
+00000220: 2022 7072 6f70 6572 7469 6573 223a 207b   "properties": {
+00000230: 0a20 2020 2020 2020 2020 2022 6465 7374  .          "dest
+00000240: 696e 6174 696f 6e22 3a20 7b0a 2020 2020  ination": {.    
+00000250: 2020 2020 2020 2020 226e 6f74 223a 207b          "not": {
+00000260: 7d0a 2020 2020 2020 2020 2020 7d0a 2020  }.          }.  
+00000270: 2020 2020 2020 7d0a 2020 2020 2020 7d0a        }.      }.
+00000280: 2020 2020 7d2c 0a20 2020 207b 0a20 2020      },.    {.   
+00000290: 2020 2022 6966 223a 207b 0a20 2020 2020     "if": {.     
+000002a0: 2020 2022 7072 6f70 6572 7469 6573 223a     "properties":
+000002b0: 207b 0a20 2020 2020 2020 2020 2022 6163   {.          "ac
+000002c0: 7469 6f6e 223a 207b 0a20 2020 2020 2020  tion": {.       
+000002d0: 2020 2020 2022 636f 6e73 7422 3a20 2272       "const": "r
+000002e0: 656e 616d 6522 0a20 2020 2020 2020 2020  ename".         
+000002f0: 207d 0a20 2020 2020 2020 207d 0a20 2020   }.        }.   
+00000300: 2020 207d 2c0a 2020 2020 2020 2274 6865     },.      "the
+00000310: 6e22 3a20 7b0a 2020 2020 2020 2020 2272  n": {.        "r
+00000320: 6571 7569 7265 6422 3a20 5b22 7375 6222  equired": ["sub"
+00000330: 2c20 2270 6174 7465 726e 225d 0a20 2020  , "pattern"].   
+00000340: 2020 207d 0a20 2020 207d 2c0a 2020 2020     }.    },.    
+00000350: 7b0a 2020 2020 2020 2269 6622 3a20 7b0a  {.      "if": {.
+00000360: 2020 2020 2020 2020 2270 726f 7065 7274          "propert
+00000370: 6965 7322 3a20 7b0a 2020 2020 2020 2020  ies": {.        
+00000380: 2020 2261 6374 696f 6e22 3a20 7b0a 2020    "action": {.  
+00000390: 2020 2020 2020 2020 2020 2263 6f6e 7374            "const
+000003a0: 223a 2022 6d6f 7665 220a 2020 2020 2020  ": "move".      
+000003b0: 2020 2020 7d0a 2020 2020 2020 2020 7d0a      }.        }.
+000003c0: 2020 2020 2020 7d2c 0a20 2020 2020 2022        },.      "
+000003d0: 7468 656e 223a 207b 0a20 2020 2020 2020  then": {.       
+000003e0: 2022 6e6f 7422 3a20 7b0a 2020 2020 2020   "not": {.      
+000003f0: 2020 2020 2272 6571 7569 7265 6422 3a20      "required": 
+00000400: 5b22 7375 6222 2c20 2270 6174 7465 726e  ["sub", "pattern
+00000410: 225d 0a20 2020 2020 2020 207d 0a20 2020  "].        }.   
+00000420: 2020 207d 0a20 2020 207d 0a20 205d 2c0a     }.    }.  ],.
+00000430: 2020 2261 6464 6974 696f 6e61 6c50 726f    "additionalPro
+00000440: 7065 7274 6965 7322 3a20 6661 6c73 650a  perties": false.
+00000450: 7d0a                                     }.
```

### Comparing `opentaskpy-0.8.1/src/opentaskpy/config/schemas.py` & `opentaskpy-0.9.0/src/opentaskpy/config/schemas.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from importlib.resources import files
 from pathlib import Path
 
 from jsonschema import validate
 from jsonschema.exceptions import ValidationError
 from jsonschema.validators import RefResolver
 
-import opentaskpy.logging
+import opentaskpy.otflogging
 
 TRANSFER_SCHEMA = {
     "type": "object",
     "properties": {
         "type": {"type": "string"},
         "source": {
             "type": "object",
@@ -75,19 +75,27 @@
     "properties": {
         "type": {"type": "string"},
         "tasks": {"type": "array", "items": {"$ref": "batch.json"}},
     },
     "required": ["type", "tasks"],
 }
 
-logger = opentaskpy.logging.init_logging(__name__)
+logger = opentaskpy.otflogging.init_logging(__name__)
 
 
-def validate_transfer_json(json_data):
-    new_schema = None
+def validate_transfer_json(json_data: dict) -> bool:
+    """Validate the JSON data against the transfer schema.
+
+    Args:
+        json_data (dict): The Transfer JSON definition
+
+    Returns:
+        bool: Whether the JSON data is valid or not
+    """
+    new_schema: dict
     try:
         validate(instance=json_data, schema=TRANSFER_SCHEMA)
 
         # If this works, then determine the protocol and apply the correct sub schema
         # Source protocol
         source_protocol = json_data["source"]["protocol"]["name"]
 
@@ -97,36 +105,37 @@
 
         schema_dir = files("opentaskpy.config").joinpath("schemas")
         # This gets us the right path for default protocol schemas. But we need to be able to load custom schemas too
         # based on the protocol name, we need to find the location of the package using the files() function
 
         # Load the schema file for XXX_source
         resolver = RefResolver(
-            base_uri=f"{schema_dir.as_uri()}/",
+            base_uri=f"{schema_dir.as_uri()}/",  # type: ignore[attr-defined]
             referrer=True,
         )
 
         # source_protocol is the class name within the plugin, we need to determine if it's a default protocol or a custom one
         # If it's a default protocol, then we can use the files() function to get the path to the schema file
         # If it's a custom protocol, then we need to look in the plugins directory for the schema file
         # Default protocols are the only ones that aren't prefixed with a package name, and we don't need to do anything more
         if "." in source_protocol:
             # Get the full package name from the class name (strip the class off the end)
-            package_name = ".".join(source_protocol.split(".")[:-2])
-            if package_name not in sys.modules:
+            if (
+                package_name := ".".join(source_protocol.split(".")[:-2])
+            ) not in sys.modules:
                 # Check the module is loadable
                 importlib.import_module(package_name)
             # Get the path to the module
             module_path = files(package_name).joinpath("schemas")
 
             # Shorten the source_protocol to just the name of the class
             source_protocol = source_protocol.split(".")[-2]
 
             # Append new path to the resolver
-            resolver.store[module_path.as_uri()] = module_path
+            resolver.store[module_path.as_uri()] = module_path  # type: ignore[attr-defined]
         else:
             # Default protocol
             module_path = schema_dir
 
         # Schema reference name should be schemas/transfer/xxx_source
         source_schema_name = Path(
             f"{module_path}/transfer/{source_protocol}_source.json"
@@ -135,30 +144,29 @@
         # Destination protocol can be different for each destination in the array. Loop through each destination and get the protocol name
         schema_refs = []
         if "destination" in json_data:
             for destination in json_data["destination"]:
                 # Get the protocol name
                 destination_protocol = destination["protocol"]["name"]
                 # As above, we need to determine the path of the protocol schema file if it's not a default protocol
-                module_path = None
                 if "." in destination_protocol:
                     # Get the full package name from the class name (strip the class off the end)
                     package_name = ".".join(destination_protocol.split(".")[:-2])
 
                     if package_name not in sys.modules:
                         # Check the module is loadable
                         importlib.import_module(package_name)
                     # Get the path to the module
                     module_path = files(package_name).joinpath("schemas")
 
                     # Shorten the destination_protocol to just the name of the class
                     destination_protocol = destination_protocol.split(".")[-2]
 
                     # Append new path to the resolver
-                    resolver.store[module_path.as_uri()] = module_path
+                    resolver.store[module_path.as_uri()] = module_path  # type: ignore[attr-defined]
                 else:
                     # Default protocol
                     module_path = schema_dir
 
                 schema_def = {
                     "$ref": Path(
                         f"{module_path}/transfer/{destination_protocol}_destination.json"
@@ -185,52 +193,58 @@
                 },
             }
 
         # Validate the new schema
         validate(instance=json_data, schema=new_schema, resolver=resolver)
 
     except ValidationError as err:
-        print(err.message)
+        print(err.message)  # noqa: T201
         return False
     return True
 
 
-def validate_execution_json(json_data):
+def validate_execution_json(json_data: dict) -> bool:
+    """Validate the JSON data against the execution schema.
+
+    Args:
+        json_data (dict): The Execution JSON definition
+
+    Returns:
+        bool: Whether the JSON data is valid or not
+    """
     try:
         validate(instance=json_data, schema=EXECUTION_SCHEMA)
 
         # If this works, then determine the protocol and apply the correct sub schema
         protocol = json_data["protocol"]["name"]
 
         # Dynamically apply the correct sub schema based on the protocol
         # We need to locate the schema files from the base location of this package
         # Get the directory of this package
         schema_dir = files("opentaskpy.config").joinpath("schemas")
 
         # Load the schema file for xxx
         resolver = RefResolver(
-            base_uri=f"{schema_dir.as_uri()}/",
+            base_uri=f"{schema_dir.as_uri()}/",  # type: ignore[attr-defined]
             referrer=True,
         )
 
         if "." in protocol:
             # Get the full package name from the class name (strip the class off the end)
-            package_name = ".".join(protocol.split(".")[:-2])
-
-            if package_name not in sys.modules:
+            if (package_name := ".".join(protocol.split(".")[:-2])) not in sys.modules:
                 # Check the module is loadable
                 importlib.import_module(package_name)
             # Get the path to the module
             module_path = files(package_name).joinpath("schemas")
 
             # Shorten the protocol to just the name of the class
             protocol = protocol.split(".")[-2]
 
             # Append new path to the resolver
-            resolver.store[module_path.as_uri()] = module_path
+            resolver.store[module_path.as_uri()] = module_path  # type: ignore[attr-defined]
         else:
             # Default protocol
             module_path = schema_dir
 
         # Schema reference name should be schemas/execution/xxx
         schema_name = Path(
             f"{module_path}/execution/{protocol}/{protocol}.json"
@@ -240,27 +254,35 @@
         new_schema = {}
         new_schema["$ref"] = schema_name
 
         # Validate the new schema
         validate(instance=json_data, schema=new_schema, resolver=resolver)
 
     except ValidationError as err:
-        print(err.message)
+        print(err.message)  # noqa: T201
         return False
     return True
 
 
-def validate_batch_json(json_data):
+def validate_batch_json(json_data: dict) -> bool:
+    """Validate the JSON data against the batch schema.
+
+    Args:
+        json_data (dict): The Batch JSON definition
+
+    Returns:
+        bool: Whether the JSON data is valid or not
+    """
     try:
         schema_dir = files("opentaskpy.config").joinpath("schemas")
 
         # Load the schema file for xxx
         resolver = RefResolver(
-            base_uri=f"{schema_dir.as_uri()}/",
+            base_uri=f"{schema_dir.as_uri()}/",  # type: ignore[attr-defined]
             referrer=True,
         )
 
         validate(instance=json_data, schema=BATCH_SCHEMA, resolver=resolver)
     except ValidationError as err:
-        print(err.message)
+        print(err.message)  # noqa: T201
         return False
     return True
```

### Comparing `opentaskpy-0.8.1/src/opentaskpy/remotehandlers/scripts/transfer.py` & `opentaskpy-0.9.0/src/opentaskpy/remotehandlers/scripts/transfer.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,68 +1,102 @@
+#!/usr/bin/env python3
+"""Remote script to handle complex transfer related tasks."""
 import argparse
 import grp
 import json
 import logging
 import os
 import pwd
 import re
 import shutil
 
 logger = logging.getLogger("opentaskpy.remotehandlers.scripts.transfer")
 
 # Remote script intended to serve as a utility to the main script for dealing with file transfers
 
 
-def list_files(pattern, details=False):
+def list_files(pattern: str, details: bool = False):  # type: ignore[no-untyped-def]
+    """List files matching the pattern.
+
+    Args:
+        pattern (str): The pattern to match files against
+        details (bool): Whether to return file details or not
+
+    Returns:
+        dict: A dict of files and their details (if requested)
+    """
     file_regex = os.path.basename(pattern)
     directory = os.path.dirname(pattern)
     files = None
     try:
         files = [
             f"{directory}/{f}" for f in os.listdir(directory) if re.match(file_regex, f)
         ]
     except FileNotFoundError:
         files = []
 
-    # For each file get the file age and size (incase we need then for file watches)
+    # For each file get the file age and size (in case we need then for file watches)
     if details:
-        result = dict()
+        result: dict = {}
         for file in files:
             file_stat = os.stat(file)
             modified_time = file_stat.st_mtime
             size = file_stat.st_size
-            result[file] = dict()
+            result[file] = {}
             result[file]["size"] = size
             result[file]["modified_time"] = modified_time
         return result
 
     return files
 
 
-def delete_files(files, delimiter):
-    files = files.split(delimiter)
-    for file in list(files):
+def delete_files(files: str, delimiter: str) -> None:
+    """Delete files from a given list.
+
+    Args:
+        files (str): File paths as a delimited string
+        delimiter (str): String delimiter
+    """
+    files_ = files.split(delimiter)
+    for file in list(files_):
         logger.info(f"Deleting {file}")
         os.unlink(file)
 
 
 def move_files(
-    files,
-    delimiter,
-    destination,
-    create_dest_dir,
-    owner,
-    group,
-    mode,
-    rename_regex,
-    rename_sub,
-):
+    files: str,
+    delimiter: str,
+    destination: str,
+    create_dest_dir: bool,
+    owner: str,
+    group: str,
+    mode: str,
+    rename_regex: str,
+    rename_sub: str,
+) -> None:
+    """Move files from a given list.
+
+    Args:
+        files (str): File paths as a delimited string
+        delimiter (str): String delimiter
+        destination (str): Destination directory
+        create_dest_dir (bool): Whether to create the destination directory if it
+        doesn't exist
+        owner (str): The owner to set on the files
+        group (str): The group to set on the files
+        mode (str): The mode to set on the files
+        rename_regex (str): A regex pattern to rename the files
+        rename_sub (str): The substitution to use when renaming the files
+
+    Returns:
+        None
+    """
     # Split the moveFiles arg into a list
-    files = files.split(delimiter)
-    for file in list(files):
+    files_ = files.split(delimiter)
+    for file in list(files_):
         file = os.path.expanduser(file)
         logger.info(f"Handling {file}")
 
         # Change ownership and permissions
         if owner:
             uid = pwd.getpwnam(owner).pw_uid
             logger.info(f"Setting owner to {owner}")
@@ -90,15 +124,16 @@
 
         # Verify the destination directory exists
         if not os.path.exists(destination) and create_dest_dir:
             logger.info(f"Creating destination directory: {destination}")
             os.makedirs(destination)
         elif not os.path.exists(destination):
             logger.error(
-                f"ERROR: Destination directory does not exist: {destination}, and not requested to create it"
+                f"ERROR: Destination directory does not exist: {destination}, and not"
+                " requested to create it"
             )
             raise FileNotFoundError
 
         # Now we can move the file into it's final location
         filename = os.path.basename(file)
         logger.info(f"Moving {file} to {destination}/{filename}")
 
@@ -117,15 +152,16 @@
         if file_stat.st_gid not in os.getgroups():
             set_group = -1
 
         os.chown(f"{destination}/{filename}", file_stat.st_uid, set_group)
         os.chmod(f"{destination}/{filename}", file_stat.st_mode)
 
 
-def main():
+def main() -> None:
+    """Main function."""
     logging.basicConfig(
         format="%(asctime)s — %(name)s — %(levelname)s — %(message)s",
         level=logging.INFO,
     )
 
     parser = argparse.ArgumentParser()
     parser.add_argument(
@@ -180,15 +216,15 @@
         required=False,
         action="store_true",
     )
 
     args = parser.parse_args()
 
     if args.listFiles:
-        print(json.dumps(list_files(args.listFiles, args.details)))
+        print(json.dumps(list_files(args.listFiles, args.details)))  # noqa: T201
 
     if args.deleteFiles:
         delete_files(args.deleteFiles, args.delimiter)
 
     if args.moveFiles:
         move_files(
             args.moveFiles,
```

### Comparing `opentaskpy-0.8.1/src/opentaskpy/remotehandlers/ssh.py` & `opentaskpy-0.9.0/src/opentaskpy/remotehandlers/ssh.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,205 +1,303 @@
+"""SSH Remote Handlers.
+
+This module contains the SSH remote handlers for transfers and executions.
+"""
 import glob
+import logging
 import os
 import random
 import re
 import stat
 import time
+from shlex import quote
 
-from paramiko import AutoAddPolicy, RSAKey, SSHClient
+from paramiko import AutoAddPolicy, RSAKey, SFTPClient, SSHClient, Transport
 
-import opentaskpy.logging
+import opentaskpy.otflogging
+from opentaskpy.exceptions import SSHClientError
 from opentaskpy.remotehandlers.remotehandler import (
     RemoteExecutionHandler,
     RemoteTransferHandler,
 )
 
-SSH_OPTIONS = "-o StrictHostKeyChecking=no -o BatchMode=yes -o ConnectTimeout=5"
+SSH_OPTIONS: str = "-o StrictHostKeyChecking=no -o BatchMode=yes -o ConnectTimeout=5"
+REMOTE_SCRIPT_BASE_DIR: str = "/tmp"  # nosec B108
 
 
 class SSHTransfer(RemoteTransferHandler):
+    """SSH Transfer Handler."""
+
     TASK_TYPE = "T"
 
     FILE_NAME_DELIMITER = "|||"
 
-    def __init__(self, spec):
-        self.spec = spec
-        self.ssh_client = None
-        self.sftp_connection = None
-        self.log_watch_start_row = 0
-
-        self.logger = opentaskpy.logging.init_logging(
+    ssh_client: SSHClient | None = None
+    sftp_connection: SFTPClient | None = None
+    log_watch_start_row = 0
+
+    def __init__(self, spec: dict):
+        """Initialise the SSHTransfer handler.
+
+        Args:
+            spec (dict): The spec for the transfer. This is either the source, or the
+            destination spec.
+        """
+        self.logger = opentaskpy.otflogging.init_logging(
             __name__, os.environ.get("OTF_TASK_ID"), self.TASK_TYPE
         )
 
         client = SSHClient()
         client.set_log_channel(
             f"{__name__}.{os.environ.get('OTF_TASK_ID')}.paramiko.transport"
         )
         client.set_missing_host_key_policy(AutoAddPolicy())
         self.ssh_client = client
 
-    def connect(self, hostname, ssh_client=None):
+        # Allow override of REMOTE_SCRIPT_BASE_DIR
+        if os.environ.get("OTF_REMOTE_SCRIPT_BASE_DIR"):
+            global REMOTE_SCRIPT_BASE_DIR  # pylint: disable=global-statement
+            REMOTE_SCRIPT_BASE_DIR = str(os.environ.get("OTF_REMOTE_SCRIPT_BASE_DIR"))
+
+        super().__init__(spec)
+
+    def connect(self, hostname: str, ssh_client: SSHClient | None = None) -> None:
+        """Connect to the remote host.
+
+        Args:
+            hostname (str): The hostname to connect to.
+            ssh_client (SSHClient, optional): An existing SSHClient to use. Defaults to None.
+        """
         is_remote_host = False
         if ssh_client is not None:
             is_remote_host = True
         else:
             ssh_client = self.ssh_client
 
-        if ssh_client.get_transport() and ssh_client.get_transport().is_active():
+        if ssh_client is None:
+            self.logger.error(f"[{self.spec['hostname']}] SSH client not initialised")
+            raise SSHClientError("SSH Client not initialised")
+
+        if ssh_client.get_transport() and ssh_client.get_transport().is_active():  # type: ignore[union-attr]
             self.logger.debug(
                 f"[{self.spec['hostname']}] SSH connection to {hostname} already active"
             )
             return
         try:
             kwargs = {
                 "hostname": hostname,
                 "username": self.spec["protocol"]["credentials"]["username"],
                 "timeout": 5,
             }
             # If a custom key is set via env vars, then set that
             if (
                 os.environ.get("OTF_SSH_KEY")
-                and os.path.exists(os.environ.get("OTF_SSH_KEY"))
+                and os.path.exists(str(os.environ.get("OTF_SSH_KEY")))
             ) and "keyFile" not in self.spec["protocol"]["credentials"]:
                 self.logger.info(
                     "Loading custom private SSH key from OTF_SSH_KEY env var"
                 )
-                key = RSAKey.from_private_key_file(os.environ.get("OTF_SSH_KEY"))
+                key = RSAKey.from_private_key_file(str(os.environ.get("OTF_SSH_KEY")))
                 kwargs["pkey"] = key
 
             # If a specific key file has been defined, then use that
             elif "keyFile" in self.spec["protocol"]["credentials"]:
                 self.logger.info("Using key file from task spec")
                 kwargs["key_filename"] = self.spec["protocol"]["credentials"]["keyFile"]
 
             ssh_client.connect(**kwargs)
-            _, stdout, _ = ssh_client.exec_command("uname -a")
+            _, stdout, _ = ssh_client.exec_command("uname -a")  # nosec B601
             with stdout as stdout_fh:
                 self.logger.log(
                     11,
-                    f"[{self.spec['hostname']}] Remote uname: {stdout_fh.read().decode('UTF-8')}",
+                    (
+                        f"[{self.spec['hostname']}] Remote uname:"
+                        f" {stdout_fh.read().decode('UTF-8')}"
+                    ),
                 )
 
             # Transfer over the transfer.py script
             local_script = (
                 f"{os.path.dirname(os.path.realpath(__file__))}/scripts/transfer.py"
             )
 
             sftp = ssh_client.open_sftp()
-            sftp.put(local_script, "/tmp/transfer.py")
+            sftp.put(local_script, f"{REMOTE_SCRIPT_BASE_DIR}/transfer.py")
 
             if not is_remote_host:
                 self.sftp_connection = sftp
-        except Exception as e:
+        except Exception as ex:
             self.logger.error(
-                f"[{self.spec['hostname']}] Unable to connect to {hostname}: {e}"
+                f"[{self.spec['hostname']}] Unable to connect to {hostname}: {ex}"
             )
-            raise e
+            raise ex
+
+    def tidy(self) -> None:
+        """Tidy up the SSH connection.
 
-    def tidy(self):
+        Shut down the SSH connection and remove the remote transfer script from the
+        remote host.
+        """
         # Remove remote scripts
         if self.sftp_connection:
-            file_list = self.sftp_connection.listdir("/tmp")
+            file_list = self.sftp_connection.listdir(REMOTE_SCRIPT_BASE_DIR)
             if "transfer.py" in file_list:
-                self.sftp_connection.remove("/tmp/transfer.py")
+                self.sftp_connection.remove(f"{REMOTE_SCRIPT_BASE_DIR}/transfer.py")
             self.sftp_connection.close()
 
             self.logger.debug(
-                f"[{self.spec['hostname']}] Closing SSH connection to {self.spec['hostname']}"
+                f"[{self.spec['hostname']}] Closing SSH connection to"
+                f" {self.spec['hostname']}"
             )
-            self.ssh_client.close()
+            if self.ssh_client:
+                self.ssh_client.close()
 
-    def get_staging_directory(self, remote_spec):
+    def get_staging_directory(self, remote_spec: dict) -> str:
+        """Get the staging directory for the remote host.
+
+        Args:
+            remote_spec (dict): The remote spec.
+
+        Returns:
+            str: The staging directory on the remote host.
+        """
         # Get the user's home directory
         if "stagingDirectory" in remote_spec:
-            return remote_spec["stagingDirectory"]
-        else:
-            _, stdout, _ = self.ssh_client.exec_command("echo $HOME")
-            with stdout as stdout_fh:
-                home_dir = stdout_fh.read().decode("UTF-8").strip()
+            return str(remote_spec["stagingDirectory"])
 
-            return f"{home_dir}/otf/{os.environ['OTF_TASK_ID']}/"
+        # Check SSH connection is established
+        if not self.ssh_client.get_transport().is_active():  # type: ignore[union-attr]
+            raise SSHClientError("SSH connection not active")
 
-    """
-    Determine the list of files that match the source definition
-    List remote files based on the source file pattern
-    """
+        _, stdout, _ = self.ssh_client.exec_command("echo $HOME")  # type: ignore[union-attr]  # nosec B601
+        with stdout as stdout_fh:
+            home_dir = stdout_fh.read().decode("UTF-8").strip()
+
+        return f"{home_dir}/otf/{os.environ.get('OTF_TASK_ID')}/"
 
-    def list_files(self, directory=None, file_pattern=None):
+    def list_files(
+        self, directory: str | None = None, file_pattern: str | None = None
+    ) -> dict:
+        """Return list of files that match the source definition.
+
+        Args:
+            directory (str, optional): The directory to search in. Defaults to None.
+            file_pattern (str, optional): The file pattern to search for. Defaults to
+            None.
+
+        Returns:
+            dict: A dict of files that match the source definition.
+        """
         self.connect(self.spec["hostname"])
         if not directory:
-            directory = self.spec["directory"]
+            directory = str(self.spec["directory"])
         if not file_pattern:
-            file_pattern = self.spec["fileRegex"]
+            file_pattern = str(self.spec["fileRegex"])
 
         self.logger.log(
             12,
-            f"[{self.spec['hostname']}] Searching in {directory} for files with pattern {file_pattern}",
+            (
+                f"[{self.spec['hostname']}] Searching in {directory} for files with"
+                f" pattern {file_pattern}"
+            ),
         )
-        remote_files = dict()
-        remote_file_list = self.sftp_connection.listdir(directory)
+        remote_files = {}
+        remote_file_list = self.sftp_connection.listdir(directory)  # type: ignore[union-attr]
         for file in list(remote_file_list):
             if re.match(file_pattern, file):
                 # Get the file attributes
-                file_attr = self.sftp_connection.lstat(f"{directory}/{file}")
+                file_attr = self.sftp_connection.lstat(f"{directory}/{file}")  # type: ignore[union-attr]
                 self.logger.log(12, f"File attributes {file_attr}")
                 remote_files[f"{directory}/{file}"] = {
                     "size": file_attr.st_size,
                     "modified_time": file_attr.st_mtime,
                 }
 
         return remote_files
 
-    ###
-    # This function is used when we need to download source files from the source server
-    # onto the worker. These are then later pushed to the destination server
-    ##
-    def pull_files_to_worker(self, files, local_staging_directory):
+    def pull_files_to_worker(
+        self, files: list[str], local_staging_directory: str
+    ) -> int:
+        """Pull files to the worker.
+
+        This function is used when we need to download source files from the source
+        server onto the worker. These are then later pushed to the destination server
+
+        Args:
+            files (list): A list of files to download.
+            local_staging_directory (str): The local staging directory to download the
+            files to.
+
+        Returns:
+            int: 0 if successful, 1 if not.
+        """
+        result = 0
         # Connect to the source
         self.connect(self.spec["hostname"])
 
         # Create the staging directory locally
         if not os.path.exists(local_staging_directory):
             os.makedirs(local_staging_directory)
 
         # Download the files via SFTP
         for file in files:
             self.logger.info(
                 f"[LOCALHOST] Downloading file {file} to {local_staging_directory}"
             )
             file_name = os.path.basename(file)
-            self.sftp_connection.get(file, f"{local_staging_directory}/{file_name}")
+            try:
+                self.sftp_connection.get(file, f"{local_staging_directory}/{file_name}")  # type: ignore[union-attr]
+            except Exception as ex:  # pylint: disable=broad-exception-caught
+                self.logger.error(
+                    f"[LOCALHOST] Unable to download file locally via SFTP: {ex}"
+                )
+                result = 1
 
-        return 0
+        return result
 
-    ###
-    # This function is used when the source files have been downloaded locally and
-    # need to be uploaded to the destination server
-    # This would be expected to be called against the remote handler for the destination server
-    ###
-    def push_files_from_worker(self, local_staging_directory):
+    def push_files_from_worker(self, local_staging_directory: str) -> int:
+        """Push files from the worker to the destination server.
+
+        This function is used when the source files have been downloaded locally and
+        need to be uploaded to the destination server. This would be expected to be
+        called against the remote handler for the destination server.
+
+        Args:
+            local_staging_directory (str): The local staging directory to upload the
+            files from.
+
+        Returns:
+            int: 0 if successful, 1 if not.
+        """
         # Connect to the destination server
         self.connect(self.spec["hostname"])
+        # Check that the SFTP client is connected and active
+        if not isinstance(self.sftp_connection, SFTPClient):
+            self.logger.error(f"[{self.spec['hostname']}] Cannot connect via SFTP")
+            return 1
 
         # Handle the staging directory
         destination_directory = self.get_staging_directory(self.spec)
 
+        # Sanitize the destination directory
+        destination_directory = quote(destination_directory)
+
         # Create/validate staging directory exists on destination
         remote_command = (
             f"test -e {destination_directory} || mkdir -p {destination_directory}"
         )
 
         self.logger.info(
-            f"[{self.spec['hostname']}] Validating staging dir via SSH: {remote_command}"
+            f"[{self.spec['hostname']}] Validating staging dir via SSH:"
+            f" {remote_command}"
         )
-        _, stdout, stderr = self.ssh_client.exec_command(remote_command)
+
+        _, stdout, stderr = self.ssh_client.exec_command(remote_command)  # type: ignore[union-attr] # nosec B601 # We've sanitised as much as possible above
         with stdout as stdout_fh:
-            str_stdout = stdout_fh.read().decode("UTF-8")
-            if str_stdout:
+            if str_stdout := stdout_fh.read().decode("UTF-8"):
                 log_stdout(str_stdout, self.spec["hostname"], self.logger)
 
         with stderr as stderr_fh:
             str_stderr = stderr_fh.read().decode("UTF-8")
             if str_stderr and len(str_stderr) > 0:
                 self.logger.info(
                     f"[{self.spec['hostname']}] Remote stderr returned:\n{str_stderr}"
@@ -215,21 +313,38 @@
         # Get list of files in local_staging_directory
         files = glob.glob(f"{local_staging_directory}/*")
         for file in files:
             self.logger.info(f"[LOCALHOST] Transferring file via SFTP: {file}")
             file_name = os.path.basename(file)
             try:
                 self.sftp_connection.put(file, f"{destination_directory}{file_name}")
-            except Exception as e:
-                self.logger.error(f"[LOCALHOST] Unable to transfer file via SFTP: {e}")
+            except Exception as ex:  # pylint: disable=broad-exception-caught
+                self.logger.error(f"[LOCALHOST] Unable to transfer file via SFTP: {ex}")
                 result = 1
 
         return result
 
-    def transfer_files(self, files, remote_spec, dest_remote_handler=None):
+    def transfer_files(
+        self,
+        files: list[str],
+        remote_spec: dict,
+        dest_remote_handler: RemoteTransferHandler | None = None,
+    ) -> int:
+        """Transfer files from the source server to the destination server.
+
+        Args:
+            files (dict): A dictionary of files to transfer.
+            remote_spec (dict): The remote specification for the destination server.
+            dest_remote_handler (RemoteTransferHandler, optional): The remote handler
+            for the destination server. Defaults to None.
+
+        Returns:
+            int: 0 if successful, if not, the return code from the remotely executed SCP
+            command.
+        """
         self.connect(self.spec["hostname"])
 
         # If we are given a destination handler, make sure we connect to the host
         if dest_remote_handler:
             self.connect(remote_spec["hostname"], dest_remote_handler.ssh_client)
 
         # Construct an SCP command to transfer the files to the destination server
@@ -239,44 +354,56 @@
             else remote_spec["protocol"]["credentials"]["username"]
         )
         remote_host = remote_spec["hostname"]
         # Handle staging directory if there is one
         destination_directory = self.get_staging_directory(remote_spec)
 
         # Create/validate staging directory exists on destination
+        destination_directory = quote(destination_directory)
         remote_command = (
             f"test -e {destination_directory} || mkdir -p {destination_directory}"
         )
         self.logger.info(
             f"[{remote_host}] Validating staging dir via SSH: {remote_command}"
         )
-        _, stdout, stderr = dest_remote_handler.ssh_client.exec_command(remote_command)
+
+        _, stdout, stderr = dest_remote_handler.ssh_client.exec_command(  # nosec B601
+            remote_command
+        )
         with stdout as stdout_fh:
             str_stdout = stdout_fh.read().decode("UTF-8")
             if str_stdout:
                 log_stdout(str_stdout, remote_host, self.logger)
 
         with stderr as stderr_fh:
             str_stderr = stderr_fh.read().decode("UTF-8")
             if str_stderr and len(str_stderr) > 0:
                 self.logger.info(
                     f"[{remote_host}] Remote stderr returned:\n{str_stderr}"
                 )
 
-        remote_rc = stdout.channel.recv_exit_status()
+        remote_rc: int = stdout.channel.recv_exit_status()
         self.logger.info(
             f"[{remote_host}] Got return code {remote_rc} from SSH command"
         )
 
-        remote_command = f'scp {SSH_OPTIONS} {" ".join(files)} {remote_user}@{remote_host}:"{destination_directory}"'
+        # Sanitise arguments
+        files = [quote(file) for file in files]
+        destination_directory = quote(destination_directory)
+        remote_user = quote(remote_user)
+        remote_host = quote(remote_host)
+
+        remote_command = (
+            f'scp {SSH_OPTIONS} {" ".join(files)} {remote_user}@{remote_host}:"{destination_directory}"'
+        )
         self.logger.info(
             f"[{self.spec['hostname']}] Transferring files via SCP: {remote_command}"
         )
 
-        _, stdout, stderr = self.ssh_client.exec_command(remote_command)
+        _, stdout, stderr = self.ssh_client.exec_command(remote_command)  # type: ignore[union-attr] # nosec B601
 
         with stdout as stdout_fh:
             str_stdout = stdout_fh.read().decode("UTF-8")
             if str_stdout:
                 log_stdout(str_stdout, self.spec["hostname"], self.logger)
 
         with stderr as stderr_fh:
@@ -289,60 +416,81 @@
         remote_rc = stdout.channel.recv_exit_status()
         self.logger.info(
             f"[{self.spec['hostname']}] Got return code {remote_rc} from SCP command"
         )
 
         return remote_rc
 
-    def pull_files(self, files, remote_spec):
+    def pull_files(self, files: list[str], remote_spec: dict) -> int:
+        """Pull files from the source server to the destination server.
+
+        Args:
+            files (list[str]): A list of files to pull.
+            remote_spec (dict): The remote specification for the source server.
+
+        Returns:
+            int: 0 if successful, if not, the return code from the remotely executed SCP
+        """
         self.connect(self.spec["hostname"])
         # Construct an SCP command to transfer the files from the source server
         source_user = self.spec["protocol"]["credentials"]["transferUsername"]
         source_host = remote_spec["hostname"]
 
         # Handle staging directory if there is one
         destination_directory = self.get_staging_directory(self.spec)
 
+        # Sanitise arguments
+        destination_directory = quote(destination_directory)
+
         # Create/validate staging directory exists
         remote_command = (
             f"test -e {destination_directory} || mkdir -p {destination_directory}"
         )
         self.logger.info(
-            f"[{self.spec['hostname']}] Validating staging dir via SSH: {remote_command}"
+            f"[{self.spec['hostname']}] Validating staging dir via SSH:"
+            f" {remote_command}"
         )
-        _, stdout, stderr = self.ssh_client.exec_command(remote_command)
+
+        _, stdout, stderr = self.ssh_client.exec_command(remote_command)  # type: ignore[union-attr] # nosec B601
         with stdout as stdout_fh:
             str_stdout = stdout_fh.read().decode("UTF-8")
             if str_stdout:
                 log_stdout(str_stdout, self.spec["hostname"], self.logger)
 
         with stderr as stderr_fh:
             str_stderr = stderr_fh.read().decode("UTF-8")
             if str_stderr and len(str_stderr) > 0:
                 self.logger.info(
                     f"[{self.spec['hostname']}] Remote stderr returned:\n{str_stderr}"
                 )
 
-        remote_rc = stdout.channel.recv_exit_status()
+        remote_rc: int = stdout.channel.recv_exit_status()
         self.logger.info(
             f"[{self.spec['hostname']}] Got return code {remote_rc} from SSH command"
         )
 
         files_str = ""
         for file in files:
+            # Sanitise file
+            file = quote(file)
+            source_host = quote(source_host)
+            source_user = quote(source_user)
+
             files_str += f"{source_user}@{source_host}:{file} "
 
+        destination_directory = quote(destination_directory)
+
         remote_command = (
             f"scp {SSH_OPTIONS} {files_str.strip()} {destination_directory}"
         )
         self.logger.info(
             f"[{self.spec['hostname']}] Transferring files via SCP: {remote_command}"
         )
 
-        _, stdout, stderr = self.ssh_client.exec_command(remote_command)
+        _, stdout, stderr = self.ssh_client.exec_command(remote_command)  # type: ignore[union-attr] # nosec B601
 
         with stdout as stdout_fh:
             str_stdout = stdout_fh.read().decode("UTF-8")
             if str_stdout:
                 log_stdout(str_stdout, self.spec["hostname"], self.logger)
 
         with stderr as stderr_fh:
@@ -355,111 +503,144 @@
         remote_rc = stdout.channel.recv_exit_status()
         self.logger.info(
             f"[{self.spec['hostname']}] Got return code {remote_rc} from SCP command"
         )
 
         return remote_rc
 
-    def move_files_to_final_location(self, files):
+    def move_files_to_final_location(self, files: dict) -> int:
+        """Move files from the staging directory to their final location.
+
+        Args:
+            files (dict): A dictionary of files to move.
+
+        Returns:
+            int: 0 if successful, if not, the return code from the remotely executed
+            transfer.py
+        """
         self.connect(self.spec["hostname"])
 
         # Convert all the source file names into the filename with the destination directory as a prefix
         file_names_str = ""
         files_with_directory = []
         for file in list(files):
             files_with_directory.append(
-                f"{self.get_staging_directory(self.spec)}{os.path.basename(file)}"
+                quote(
+                    f"{self.get_staging_directory(self.spec)}{os.path.basename(file)}"
+                )
             )
         file_names_str = self.FILE_NAME_DELIMITER.join(files_with_directory).strip()
 
         # Next step is to move the file to it's final resting place with the correct permissions and ownership
-        # Build a commnd to pass to the remote transfer.py to do the work
+        # Build a command to pass to the remote transfer.py to do the work
         owner_args = (
-            f"--owner {self.spec['permissions']['owner']}"
+            f"--owner {quote(self.spec['permissions']['owner'])}"
             if "permissions" in self.spec and "owner" in self.spec["permissions"]
             else ""
         )
         group_args = (
-            f"--group {self.spec['permissions']['group']}"
+            f"--group {quote(self.spec['permissions']['group'])}"
             if "permissions" in self.spec and "group" in self.spec["permissions"]
             else ""
         )
-        mode_args = f"--mode {self.spec['mode']}" if "mode" in self.spec else ""
+        mode_args = f"--mode {quote(self.spec['mode'])}" if "mode" in self.spec else ""
         rename_args = (
-            f"--renameRegex '{self.spec['rename']['pattern']}' --renameSub '{self.spec['rename']['sub']}'"
+            f"--renameRegex {quote(self.spec['rename']['pattern'])} --renameSub"
+            f" {quote(self.spec['rename']['sub'])}"
             if "rename" in self.spec
             else ""
         )
-        remote_command = f"python3 /tmp/transfer.py --moveFiles '{file_names_str}' --destination {self.spec['directory']} {owner_args} {group_args} {mode_args} {rename_args}"
+
+        directory = quote(self.spec["directory"])
+
+        remote_command = (
+            f"python3 {REMOTE_SCRIPT_BASE_DIR}/transfer.py --moveFiles"
+            f" '{file_names_str}' --destination"
+            f" {directory} {owner_args} {group_args} {mode_args} {rename_args}"
+        )
         self.logger.info(f"[{self.spec['hostname']}] Running: {remote_command}")
 
-        stdin, stdout, stderr = self.ssh_client.exec_command(remote_command)
+        stdin, stdout, stderr = self.ssh_client.exec_command(remote_command)  # type: ignore[union-attr] # nosec B601
 
         with stdout as stdout_fh:
             str_stdout = stdout_fh.read().decode("UTF-8")
             if str_stdout:
                 log_stdout(str_stdout, self.spec["hostname"], self.logger)
 
         with stderr as stderr_fh:
             str_stderr = stderr_fh.read().decode("UTF-8")
             if str_stderr and len(str_stderr) > 0:
                 self.logger.info(
                     f"[{self.spec['hostname']}] Remote stderr returned:\n{str_stderr}"
                 )
 
-        remote_rc = stdout.channel.recv_exit_status()
+        remote_rc: int = stdout.channel.recv_exit_status()
         self.logger.info(
-            f"[{self.spec['hostname']}] Got return code {remote_rc} from SSH move command"
+            f"[{self.spec['hostname']}] Got return code {remote_rc} from SSH move"
+            " command"
         )
         return remote_rc
 
-    def handle_post_copy_action(self, files):
+    def handle_post_copy_action(self, files: list[str]) -> int:
+        """Handle the post copy action specified in the config.
+
+        Args:
+            files (list[str]): A list of files that need to be handled.
+
+        Returns:
+            int: 0 if successful, 1 if not.
+        """
         self.connect(self.spec["hostname"])
-        sftp_client = self.ssh_client.open_sftp()
+        sftp_client = self.ssh_client.open_sftp()  # type: ignore[union-attr]
 
         if self.spec["postCopyAction"]["action"] == "delete":
             # Loop through each file and use the sftp client to delete the files
 
             for file in files:
                 try:
                     sftp_client.remove(file)
-                except IOError:
+                except OSError:
                     self.logger.error(
-                        f"[{self.spec['hostname']}] Could not delete file {file} on source host"
+                        f"[{self.spec['hostname']}] Could not delete file {file} on"
+                        " source host"
                     )
                     return 1
 
         if (
             self.spec["postCopyAction"]["action"] == "move"
             or self.spec["postCopyAction"]["action"] == "rename"
         ):
             # Use the SFTP client, and check that the destination directory exists
             move_dir = os.path.dirname(self.spec["postCopyAction"]["destination"])
 
             try:
                 stat_result = sftp_client.stat(move_dir)
                 # If it exists, then we need to ensure its a directory and not just a file
-                if not stat.S_ISDIR(stat_result.st_mode):
+                if not stat.S_ISDIR(stat_result.st_mode):  # type: ignore[arg-type]
                     self.logger.error(
-                        f"[{self.spec['hostname']}] Destination directory {move_dir} is not a directory on source host"
+                        f"[{self.spec['hostname']}] Destination directory {move_dir} is"
+                        " not a directory on source host"
                     )
                     return 1
-            except IOError:
+            except OSError:
                 self.logger.error(
-                    f"[{self.spec['hostname']}] Destination directory {move_dir} does not exist on source host"
+                    f"[{self.spec['hostname']}] Destination directory {move_dir} does"
+                    " not exist on source host"
                 )
                 return 1
 
-            # Loop through the files and move them
-            try:
-                for file in files:
+                # Loop through the files and move them
+
+            for file in files:
+                try:
                     # If this is a move, then just move the file
                     if self.spec["postCopyAction"]["action"] == "move":
                         self.logger.info(
-                            f"[{self.spec['hostname']}] Moving {file} to {self.spec['postCopyAction']['destination']}"
+                            f"[{self.spec['hostname']}] Moving {file} to"
+                            f" {self.spec['postCopyAction']['destination']}"
                         )
                         # Get the actual file name
                         file_name = os.path.basename(file)
                         sftp_client.posix_rename(
                             file,
                             f"{self.spec['postCopyAction']['destination']}/{file_name}",
                         )
@@ -475,30 +656,40 @@
                         rename_sub = self.spec["postCopyAction"]["sub"]
 
                         new_file_name = re.sub(
                             rename_regex, rename_sub, current_file_name
                         )
 
                         self.logger.info(
-                            f"[{self.spec['hostname']}] Renaming {file} to {new_file_dir}/{new_file_name}"
+                            f"[{self.spec['hostname']}] Renaming {file} to"
+                            f" {new_file_dir}/{new_file_name}"
                         )
                         sftp_client.posix_rename(
                             file, f"{new_file_dir}/{new_file_name}"
                         )
-            except IOError as e:
-                self.logger.error(f"[{self.spec['hostname']}] Error: {e}")
-                self.logger.error(
-                    f"[{self.spec['hostname']}] Error moving or renaming file {file}"
-                )
-                return 1
+                except OSError as e:
+                    self.logger.error(f"[{self.spec['hostname']}] Error: {e}")
+                    self.logger.error(
+                        f"[{self.spec['hostname']}] Error moving or renaming file"
+                        f" {file}"
+                    )
+                    return 1
 
         return 0
 
-    def init_logwatch(self):
+    def init_logwatch(self) -> int:
+        """Initialise the logwatch process.
+
+        Returns:
+            int: 0 if successful, 1 if not.
+        """
         self.connect(self.spec["hostname"])
+        if not isinstance(self.sftp_connection, SFTPClient):
+            self.logger.error(f"[{self.spec['hostname']}] Cannot connect via SFTP")
+            return 1
 
         # There are 2 options for logwatches. One is to watch for new entries, the other is to scan the entire log.
         # Default if not specified is to watch for new entries
 
         # Determine the log details and check it exists first
         log_file = (
             f"{self.spec['logWatch']['directory']}/{self.spec['logWatch']['log']}"
@@ -517,25 +708,33 @@
                 f"[{self.spec['hostname']}] Log file {log_file} cannot be accessed"
             )
             return 1
 
         # Open the existing file and determine the number of rows
         with self.sftp_connection.open(log_file) as log_fh:
             rows = 0
-            for rows, _ in enumerate(log_fh):  # noqa #B007
+            for _, _ in enumerate(log_fh):
                 pass
             self.logger.log(
                 12, f"[{self.spec['hostname']}] Found {rows+1} lines in log"
             )
             self.log_watch_start_row = rows + 1
 
         return 0
 
-    def do_logwatch(self):
+    def do_logwatch(self) -> int:
+        """Perform the logwatch process.
+
+        Returns:
+            int: 0 if successful, 1 if not.
+        """
         self.connect(self.spec["hostname"])
+        if not isinstance(self.sftp_connection, SFTPClient):
+            self.logger.error(f"[{self.spec['hostname']}] Cannot connect via SFTP")
+            return 1
 
         # Determine if the config requires scanning the entire log, or just from the start_row determine in the init function
         start_row = (
             self.log_watch_start_row
             if "tail" in self.spec["logWatch"] and self.spec["logWatch"]["tail"]
             else 0
         )
@@ -554,184 +753,247 @@
                 if i >= start_row:
                     self.logger.log(
                         11, f"[{self.spec['hostname']}] Log line: {line.strip()}"
                     )
                     if re.search(self.spec["logWatch"]["contentRegex"], line.strip()):
                         self.logger.log(
                             12,
-                            f"[{self.spec['hostname']}] Found matching line in log: {line.strip()} on line: {i+1}",
+                            (
+                                f"[{self.spec['hostname']}] Found matching line in log:"
+                                f" {line.strip()} on line: {i+1}"
+                            ),
                         )
                         return 0
 
         return 1
 
-    def create_flag_files(self):
+    def create_flag_files(self) -> int:
+        """Create the flag files on the remote host.
+
+        Returns:
+            int: 0 if successful, 1 if not.
+        """
         self.connect(self.spec["hostname"])
+
+        if not isinstance(self.ssh_client, SSHClient):
+            self.logger.error(f"[{self.spec['hostname']}] Cannot connect via SSH")
+            return 1
+
+        # Manually open SFTP client
         sftp_client = self.ssh_client.open_sftp()
         filename = self.spec["flags"]["fullPath"]
 
         try:
             # Use the SFTP client to create an empty file at this path
             sftp_client.file(filename, "w").close()
 
-            # TODO: File permissions
+            # Set permissions on the file to whatever was specified in the spec,
+            # otherwise we leave them as is
+            # We cannot change ownership without using sudo, so we don't bother
+            if "permissions" in self.spec:
+                sftp_client.chmod(filename, self.spec["permissions"])
 
-        except IOError as e:
+        except OSError as e:
             self.logger.error(f"[{self.spec['hostname']}] Error: {e}")
             self.logger.error(
                 f"[{self.spec['hostname']}] Error creating flag file: {filename}"
             )
             return 1
 
         return 0
 
 
-def log_stdout(str_stdout, hostname, logger):
-    # self.logger.info(f"[{hostname}] Remote stdout returned:")
-    # self.logger.info(f"[{hostname}] ###########")
+def log_stdout(str_stdout: str, hostname: str, logger: logging.Logger) -> None:
+    """Log the stdout from a remote command in a nice format.
+
+    Args:
+        str_stdout (str): The stdout from the remote command
+        hostname (str): The hostname of the remote host
+        logger (logging.Logger): The logger to use
+    """
     for line in str_stdout.splitlines():
         logger.info(f"[{hostname}] REMOTE OUTPUT: {line}")
-    # self.logger.info(f"[{hostname}] ###########")
 
 
 class SSHExecution(RemoteExecutionHandler):
+    """Class to handle SSH execution of remote commands."""
+
     TASK_TYPE = "E"
     ps_regex = r"(\S+)\s+(\d+)\s+(\d+)\s+(\d+)\s+(\S+)\s+(\S+)\s+(\S+)\s+(.*)"
+    ssh_client: SSHClient
+    remote_pid: int
 
-    def tidy(self):
+    def tidy(self) -> None:
+        """Tidy up the SSH connection."""
         self.logger.debug(f"[{self.remote_host}] Closing SSH connection")
-        self.ssh_client.close()
+        if self.ssh_client:
+            self.ssh_client.close()
+
+    def __init__(self, remote_host: str, spec: dict):
+        """Initialise the SSHExecution class.
 
-    def __init__(self, remote_host, spec):
-        self.remote_host = remote_host
-        self.spec = spec
-        self.ssh_client = None
-        self.remote_pid = None
-        self.random = random.randint(
+        Args:
+            remote_host (str): The hostname of the remote host
+            spec (dict): The specification for the remote command
+        """
+        self.remote_host: str = remote_host
+        self.random: int = random.randint(
             100000, 999999
         )  # Random number used to make sure when we kill stuff, we always kill the right thing
 
-        self.remote_host = remote_host
-
-        self.logger = opentaskpy.logging.init_logging(
+        self.logger = opentaskpy.otflogging.init_logging(
             __name__, os.environ.get("OTF_TASK_ID"), self.TASK_TYPE
         )
 
+        super().__init__(spec)
+
         client = SSHClient()
         client.set_log_channel(
             f"{__name__}.{os.environ.get('OTF_TASK_ID')}.paramiko.transport"
         )
         client.set_missing_host_key_policy(AutoAddPolicy())
 
         self.ssh_client = client
 
-    def connect(self):
-        if (
-            self.ssh_client
-            and self.ssh_client.get_transport()
-            and self.ssh_client.get_transport().is_active()
-        ):
-            return
+    def connect(self) -> None:
+        """Connect to the remote host."""
+        if self.ssh_client and isinstance(self.ssh_client, SSHClient):
+            transport = self.ssh_client.get_transport()
+            if (
+                transport is not None
+                and isinstance(transport, Transport)
+                and transport.is_active()
+            ):
+                return
 
         kwargs = {
             "hostname": self.remote_host,
             "username": self.spec["protocol"]["credentials"]["username"],
             "timeout": 5,
         }
 
         # If a custom key is set via env vars, then set that
         if (
             os.environ.get("OTF_SSH_KEY")
-            and os.path.exists(os.environ.get("OTF_SSH_KEY"))
+            and os.path.exists(str(os.environ.get("OTF_SSH_KEY")))
         ) and "keyFile" not in self.spec["protocol"]["credentials"]:
             self.logger.info("Loading custom private SSH key from OTF_SSH_KEY env var")
-            key = RSAKey.from_private_key_file(os.environ.get("OTF_SSH_KEY"))
+            key = RSAKey.from_private_key_file(str(os.environ.get("OTF_SSH_KEY")))
             kwargs["pkey"] = key
 
         # If a specific key file has been defined, then use that
         elif "keyFile" in self.spec["protocol"]["credentials"]:
             self.logger.info("Using key file from task spec")
             kwargs["key_filename"] = self.spec["protocol"]["credentials"]["keyFile"]
 
         self.ssh_client.connect(**kwargs)
-        _, stdout, _ = self.ssh_client.exec_command("uname -a")
+        _, stdout, _ = self.ssh_client.exec_command("uname -a")  # nosec B601
         with stdout as stdout_fh:
             output = stdout_fh.read().decode("UTF-8")
             self.logger.log(11, f"[{self.remote_host}] Remote uname: {output}")
 
-    def _get_child_processes(self, parent_pid, process_listing):
+    def _get_child_processes(self, parent_pid: int, process_listing: list) -> list:
+        """Get the child processes of a given PID.
+
+        Args:
+            parent_pid (int): The PID of the parent process
+            process_listing (list): The list of processes running on the remote host
+
+        Returns:
+            list: A list of child PIDs
+        """
         children = []
         for line in process_listing:
             match = re.search(self.ps_regex, line)
             if match:
                 if int(match.group(3)) == parent_pid:
                     child_pid = int(match.group(2))
                     # Never add PID 1 or 0!
-                    if child_pid == 1 or child_pid == 0:
+                    if child_pid in (1, 0):
                         continue
                     self.logger.debug(
-                        f"[{self.remote_host}] Found child process with PID: {child_pid}"
+                        f"[{self.remote_host}] Found child process with PID:"
+                        f" {child_pid}"
                     )
                     children.append(child_pid)
                     # Recurse to find the children of this child
                     children.extend(
                         self._get_child_processes(child_pid, process_listing)
                     )
         return children
 
-    def kill(self):
+    def kill(self) -> None:
+        """Kill the remote process."""
         self.logger.info(f"[{self.remote_host}] Killing remote process")
 
         self.connect()
         # We know the top level remote PID, we need to get all the child processes associated with it
-        _, stdout, _ = self.ssh_client.exec_command("ps -ef")
+        _, stdout, _ = self.ssh_client.exec_command("ps -ef")  # nosec B601
         process_listing = []
         # Get the process listing
         with stdout as stdout_fh:
             process_listing = stdout_fh.read().decode("UTF-8").splitlines()
 
         # Now we have this, parse it, find the parent PID, and then all the children
         children = self._get_child_processes(self.remote_pid, process_listing)
         children.append(self.remote_pid)
         self.logger.info(
-            f"[{self.remote_host}] Found {len(children)} child processes to kill - {children}"
+            f"[{self.remote_host}] Found {len(children)} child processes to kill -"
+            f" {children}"
         )
 
         # Now we have the list of children, kill them
         command = f"kill {' '.join([str(x) for x in children])}"
         self.logger.info(
             f"[{self.remote_host}] Killing remote processes with command: {command}"
         )
-        _, stdout, _ = self.ssh_client.exec_command(command)
+
+        # Make sure we're not killing PID 1 or 0
+        if command in ("kill 1", "kill 0"):
+            self.logger.error(
+                f"[{self.remote_host}] Refusing to kill PID 1 or 0, aborting"
+            )
+            return
+        _, stdout, _ = self.ssh_client.exec_command(command)  # nosec B601
         # Wait for the command to finish
         while not stdout.channel.exit_status_ready():
             time.sleep(0.1)
 
         # Disconnect SSH
         self.tidy()
 
-    def execute(self):
-        # Establish the SSH connection
+    def execute(self) -> bool:
+        """Execute the remote command.
+
+        Returns:
+            bool: True if the command was executed successfully, False otherwise
+        """
         try:
             self.connect()
 
-            # Command needs the directory to be changed to appended to it
-            command = f"echo __OTF_TOKEN__$$_{self.random}__; cd {self.spec['directory']} && {self.spec['command']}"
+            directory = quote(self.spec["directory"])
+
+            command = (
+                f"echo __OTF_TOKEN__$$_{self.random}__; cd {directory} &&"
+                f" {self.spec['command']}"
+            )
 
             self.logger.info(f"[{self.remote_host}] Executing command: {command}")
-            _, stdout, stderr = self.ssh_client.exec_command(command)
+
+            _, stdout, stderr = self.ssh_client.exec_command(command)  # nosec B601
 
             # Log the stdout and stderr
-            for line in iter(lambda: stdout.readline(2048), ""):
+            for line in iter(lambda: str(stdout.readline(2048)), ""):
                 log_stdout(line, self.remote_host, self.logger)
 
                 # Check the line for the token and pull out the PID
                 regex = f"__OTF_TOKEN__(\\d+)_{self.random}__"
-                if re.search(regex, line):
-                    self.remote_pid = int(re.search(regex, line).group(1))
+                pid_search = re.search(regex, line)
+                if pid_search:
+                    self.remote_pid = int(pid_search.group(1))
                     self.logger.info(
                         f"[{self.remote_host}] Found remote PID: {self.remote_pid}"
                     )
 
             with stderr as stderr_fh:
                 str_stderr = stderr_fh.read().decode("UTF-8")
                 if str_stderr and len(str_stderr) > 0:
@@ -743,12 +1005,12 @@
             remote_rc = stdout.channel.recv_exit_status()
             self.tidy()
             if remote_rc != 0:
                 self.logger.error(
                     f"[{self.remote_host}] Got return code {remote_rc} from SSH command"
                 )
                 return False
-            else:
-                return True
-        except Exception as e:
+
+            return True
+        except Exception as e:  # pylint: disable=broad-exception-caught
             self.logger.error(f"[{self.remote_host}] Exception caught: {e}")
             return False
```

### Comparing `opentaskpy-0.8.1/src/opentaskpy/taskhandlers/batch.py` & `opentaskpy-0.9.0/src/opentaskpy/taskhandlers/batch.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,50 +1,72 @@
+"""Batch task handler class."""
 import threading
 import time
 from concurrent.futures import ThreadPoolExecutor, wait
 from os import environ
 
-import opentaskpy.logging
+import opentaskpy.otflogging
+from opentaskpy.config.loader import ConfigLoader
+from opentaskpy.exceptions import InvalidConfigError
 from opentaskpy.taskhandlers.execution import Execution
 from opentaskpy.taskhandlers.taskhandler import TaskHandler
 from opentaskpy.taskhandlers.transfer import Transfer
 
 DEFAULT_TASK_TIMEOUT = 300
 DEFAULT_TASK_CONTINUE_ON_FAIL = False
 DEFAULT_TASK_RETRY_ON_RERUN = False
 DEFAULT_TASK_EXIT_CODE = 0
 TASK_TYPE = "B"
 BATCH_TASK_LOG_MARKER = "__OTF_BATCH_TASK_MARKER__"
 
 
 class Batch(TaskHandler):
+    """Batch task handler class."""
+
     overall_result = False
 
-    def __init__(self, global_config, task_id, batch_definition, config_loader):
+    def __init__(
+        self,
+        global_config: dict,
+        task_id: str,
+        batch_definition: dict,
+        config_loader: ConfigLoader,
+    ):
+        """Initialise the batch task handler.
+
+        Args:
+            global_config (dict): The global configuration for the task.
+            task_id (str): The ID of the task.
+            batch_definition (dict): The definition of the batch task.
+            config_loader (ConfigLoader): The config loader to use to load
+            task definitions within the batch.
+        """
         self.task_id = task_id
         self.batch_definition = batch_definition
         self.config_loader = config_loader
-        self.tasks = dict()
-        self.task_order_tree = dict()
+        self.tasks = {}
+        self.task_order_tree = {}
 
         super().__init__(global_config)
 
-        self.logger = opentaskpy.logging.init_logging(__name__, self.task_id, TASK_TYPE)
+        self.logger = opentaskpy.otflogging.init_logging(
+            __name__, self.task_id, TASK_TYPE
+        )
 
         # We need to get the latest log file (if there is one), to determine
         # where to start from (if we are resuming a batch)
-        previous_log_file = opentaskpy.logging.get_latest_log_file(
+        previous_log_file = opentaskpy.otflogging.get_latest_log_file(
             self.task_id, TASK_TYPE
         )
-        previous_status = dict()
+        previous_status = {}
         if previous_log_file:
             self.logger.info("Parsing previous log file for log marks")
 
             # Parse the previous log file to determine where we left off
-            with open(previous_log_file, "r") as f:
+            with open(previous_log_file, encoding="utf-8") as f:
                 for line in f:
                     if BATCH_TASK_LOG_MARKER in line:
                         log_mark = line.split(f"{BATCH_TASK_LOG_MARKER}: ")[1].strip()
                         self.logger.info(f"Found log mark: {log_mark}")
                         # Mark the task with the appropriate status
                         # Determine which order id this is for
                         mark_metadata = log_mark.split("::")
@@ -61,52 +83,48 @@
             order_id = task["order_id"]
 
             # Add it to the list of tasks
             self.tasks[order_id] = task_definition
 
             # Set the timeout for the task
             timeout = None
-            if "timeout" in task:
-                timeout = task["timeout"]
-            else:
-                timeout = DEFAULT_TASK_TIMEOUT
+            timeout = task.get("timeout", DEFAULT_TASK_TIMEOUT)
 
             # Same for continue on fail
             continue_on_fail = None
             if "continue_on_fail" in task:
                 continue_on_fail = task["continue_on_fail"]
             else:
                 continue_on_fail = DEFAULT_TASK_CONTINUE_ON_FAIL
 
             # Same for retry on rerun
             retry_on_rerun = None
-            if "retry_on_rerun" in task:
-                retry_on_rerun = task["retry_on_rerun"]
-            else:
-                retry_on_rerun = DEFAULT_TASK_RETRY_ON_RERUN
+            retry_on_rerun = task.get("retry_on_rerun", DEFAULT_TASK_RETRY_ON_RERUN)
 
             # Set the status of the task
             status = "NOT_STARTED"
             if order_id in previous_status:
                 # Check whether it should be rerun if it worked last time
                 if retry_on_rerun:
                     if previous_status[order_id] == "COMPLETED":
                         # Log something to make it clear that we are rerunning
                         self.logger.info(
-                            f"Task {task_id} succeeded last time, but is marked to be rerun"
+                            f"Task {task_id} succeeded last time, but is marked to be"
+                            " rerun"
                         )
                     status = "NOT_STARTED"
                 elif previous_status[order_id] == "COMPLETED":
                     self.logger.info(
-                        f"Task {task_id} succeeded last time, and is not marked to be rerun, so marking as complete"
+                        f"Task {task_id} succeeded last time, and is not marked to be"
+                        " rerun, so marking as complete"
                     )
                     # Output the log mark
                     self._log_task_result(
                         "COMPLETED",
-                        order_id,
+                        str(order_id),
                         task["task_id"],
                     )
                     status = "COMPLETED"
 
             # Create the task handlers for anything we intend on running
             task_handler = None
             if status == "NOT_STARTED":
@@ -123,15 +141,15 @@
                     task_handler = Batch(
                         global_config,
                         task["task_id"],
                         task_definition,
                         self.config_loader,
                     )
                 else:
-                    raise Exception("Unknown task type")
+                    raise InvalidConfigError("Unknown task type")
 
             self.task_order_tree[order_id] = {
                 "task_id": task["task_id"],
                 "batch_task_spec": task,
                 "task": task_definition,
                 "task_handler": task_handler,
                 "timeout": timeout,
@@ -140,36 +158,44 @@
                 "status": status,
                 "result": None,
             }
 
         # Debug to show the structure of the tree
         self.logger.debug(f"Task order tree: {self.task_order_tree}")
 
-    def _set_remote_handlers(self):
+    def _set_remote_handlers(self) -> None:
         pass
 
-    def return_result(self, status, message=None, exception=None):
-        if message:
-            if status == 0:
-                self.logger.info(message)
-            else:
-                self.logger.error(message)
-                self.overall_result = False
-
-        # Close the file handler
-        self.logger.info("Closing log file handler")
-        opentaskpy.logging.close_log_file(self.logger, self.overall_result)
-
-        # Throw an exception if we have one
-        if exception:
-            raise exception(message)
-
-        return status == 0
-
-    def run(self, kill_event=None):
+    def return_result(
+        self,
+        status: int,
+        message: str | None = None,
+        exception: type[Exception] | None = None,
+    ) -> bool:
+        """Return the result of the task run.
+
+        Args:
+            status (int): The status code to return.
+            message (str, optional): The message to return. Defaults to None.
+            exception (Exception, optional): The exception to return. Defaults to None.
+
+        Returns:
+            bool: The result of the task run.
+        """
+        return super().return_result(status, message, exception)  # type: ignore[no-any-return]
+
+    def run(self, kill_event: threading.Event | None = None) -> bool:
+        """Run the batch.
+
+        Args:
+            kill_event (threading.Event, optional): An event to kill the batch. Defaults to None.
+
+        Returns:
+            bool: True if the batch completed successfully, False otherwise.
+        """
         self.logger.info("Running batch")
         environ["OTF_TASK_ID"] = self.task_id
 
         # This is where we could potentially be waiting for a while. So,
         # for each task handler, we should spawn a new thread to run
         # the command. Then we can wait for all threads to complete.
 
@@ -186,20 +212,25 @@
                 # Check if there are dependencies for this task that have not yet completed, if so then we skip it
                 if "dependencies" in batch_task["batch_task_spec"]:
                     all_dependencies_complete = True
                     for dependency in batch_task["batch_task_spec"]["dependencies"]:
                         if self.task_order_tree[dependency]["status"] != "COMPLETED":
                             self.logger.log(
                                 12,
-                                f"Skipping task {order_id} ({batch_task['task_id']}) as dependency {dependency} has not completed",
+                                (
+                                    "Skipping task"
+                                    f" {order_id} ({batch_task['task_id']}) as"
+                                    f" dependency {dependency} has not completed"
+                                ),
                             )
                             all_dependencies_complete = False
                             continue
                         self.logger.info(
-                            f"All dependencies for task {order_id} ({batch_task['task_id']}) have completed"
+                            "All dependencies for task"
+                            f" {order_id} ({batch_task['task_id']}) have completed"
                         )
                     if not all_dependencies_complete:
                         continue
 
                 # Check if the task has already been triggered
                 if batch_task["status"] == "NOT_STARTED":
                     # Create a new thread to run the task. Pass an event into the thread so we can handle timeouts
@@ -255,15 +286,16 @@
 
                 # Handle instances where we timed out or failed, and we should continue on fail
                 if (
                     batch_task["status"] in ["TIMED_OUT", "FAILED"]
                     and batch_task["continue_on_fail"]
                 ):
                     self.logger.info(
-                        f"Task {order_id} ({batch_task['task_id']}) has failed, but continuing on fail"
+                        f"Task {order_id} ({batch_task['task_id']}) has failed, but"
+                        " continuing on fail"
                     )
                     batch_task["status"] = "COMPLETED"
                     batch_task["result"] = False
 
             # Check if there are any tasks that are still in RUNNING state, if not then we are done
             running_tasks = [
                 task
@@ -298,20 +330,24 @@
         if len(failed_tasks) == 0:
             self.overall_result = True
 
         self.logger.info(f"Batch completed with result {self.overall_result}")
 
         if self.overall_result:
             return self.return_result(0, "All batch tasks completed successfully")
-        else:
-            return self.return_result(1, "Batch failed", ex)
 
-    def task_runner(self, batch_task, event):
-        # Thread to trigger the task itself
+        return self.return_result(1, "Batch failed", ex)
 
+    def task_runner(self, batch_task: dict, event: threading.Event) -> None:
+        """Run the task in a separate thread.
+
+        Args:
+            batch_task (dict): The task to run
+            event (threading.Event): The event to use to kill the thread
+        """
         self.logger.info(f"Running task {batch_task['task_id']}")
         with ThreadPoolExecutor(
             max_workers=1, thread_name_prefix=batch_task["task_id"]
         ) as executor:
             while True:
                 if batch_task["executing_thread"] is None:
                     self.logger.log(
@@ -344,53 +380,57 @@
                             batch_task["status"] = "FAILED"
                         self._log_task_result(
                             batch_task["status"],
                             batch_task["batch_task_spec"]["order_id"],
                             batch_task["task_id"],
                         )
                         break
-                    else:
-                        # Check if we have been asked to kill the thread
-                        if event.is_set():
-                            self.logger.log(
-                                12, f"Killing task handler for {batch_task['task_id']}"
-                            )
-                            # Kill the thread and all it's child processes
-                            batch_task["executing_thread"][0].cancel()
-                            executor.shutdown(wait=False)
-                            self._log_task_result(
-                                "FAILED",
-                                batch_task["batch_task_spec"]["order_id"],
-                                batch_task["task_id"],
-                            )
-
-                            break
 
-                        # Wait for the thread to complete
+                    # Check if we have been asked to kill the thread
+                    if event.is_set():
                         self.logger.log(
-                            12, f"Waiting for task handler for {batch_task['task_id']}"
+                            12, f"Killing task handler for {batch_task['task_id']}"
+                        )
+                        # Kill the thread and all it's child processes
+                        batch_task["executing_thread"][0].cancel()
+                        executor.shutdown(wait=False)
+                        self._log_task_result(
+                            "FAILED",
+                            batch_task["batch_task_spec"]["order_id"],
+                            batch_task["task_id"],
                         )
-                        wait(batch_task["executing_thread"], timeout=2)
+
+                        break
+
+                    # Wait for the thread to complete
+                    self.logger.log(
+                        12, f"Waiting for task handler for {batch_task['task_id']}"
+                    )
+                    wait(batch_task["executing_thread"], timeout=2)
 
             batch_task["end_time"] = time.time()
 
-    def _log_task_result(self, status, order_id, task_id):
+    def _log_task_result(self, status: str, order_id: str, task_id: str) -> None:
         self.logger.info(
             f"{BATCH_TASK_LOG_MARKER}: ORDER_ID::{order_id}::TASK::{task_id}::{status}"
         )
 
-    def _execute(self, remote_handler, event=None):
+    def _execute(
+        self, task_handler: TaskHandler, event: threading.Event | None = None
+    ) -> bool:  #
+        result = False
         try:
-            result = remote_handler.run(kill_event=event)
-        except Exception as ex:
-            self.logger.error(f"[{remote_handler.task_id}] Failed to run task")
+            result = task_handler.run(kill_event=event)
+        except Exception as ex:  # pylint: disable=broad-exception-caught
+            self.logger.error(f"[{task_handler.task_id}] Failed to run task")
             self.logger.error(ex)
             result = False
 
-        self.logger.info(f"[{remote_handler.task_id}] Returned {result}")
+        self.logger.info(f"[{task_handler.task_id}] Returned {result}")
         return result
 
     # Destructor to handle when the batch is finished. Make sure the log file
     # gets renamed as appropriate
-    def __del__(self):
+    def __del__(self) -> None:
+        """Destructor to handle closing log file correctly."""
         self.logger.debug("Batch object deleted")
-        opentaskpy.logging.close_log_file(self.logger, self.overall_result)
+        opentaskpy.otflogging.close_log_file(self.logger, self.overall_result)
```

### Comparing `opentaskpy-0.8.1/src/opentaskpy/taskhandlers/execution.py` & `opentaskpy-0.9.0/src/opentaskpy/taskhandlers/execution.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,72 +1,86 @@
+"""Execution task handler."""
+import threading
 from concurrent.futures import ThreadPoolExecutor, wait
 from os import environ
 
-import opentaskpy.logging
+import opentaskpy.otflogging
+from opentaskpy.remotehandlers.remotehandler import RemoteHandler
 from opentaskpy.remotehandlers.ssh import SSHExecution
 from opentaskpy.taskhandlers.taskhandler import TaskHandler
 
 TASK_TYPE = "E"
 
 
 class Execution(TaskHandler):
-    def __init__(self, global_config, task_id, execution_definition):
+    """Execution task handler."""
+
+    remote_handlers: list[RemoteHandler] | None = None
+    overall_result: bool = False
+
+    def __init__(self, global_config: dict, task_id: str, execution_definition: dict):
+        """Initialize the execution handler.
+
+        Args:
+            global_config (dict): The global config.
+            task_id (str): The task ID.
+            execution_definition (dict): The execution definition.
+        """
         self.task_id = task_id
         self.execution_definition = execution_definition
-        self.remote_handlers = None
-        self.overall_result = False
 
-        self.logger = opentaskpy.logging.init_logging(
+        self.logger = opentaskpy.otflogging.init_logging(
             "opentaskpy.taskhandlers.execution", self.task_id, TASK_TYPE
         )
 
         super().__init__(global_config)
 
-    def return_result(self, status, message=None, exception=None):
-        if message:
-            if status == 0:
-                self.logger.info(message)
-            else:
-                self.logger.error(message)
-
-        if status == 0:
-            self.overall_result = True
-
+    def return_result(
+        self,
+        status: int,
+        message: str | None = None,
+        exception: Exception | None = None,
+    ) -> bool:
+        """Return the result of the task run.
+
+        Args:
+            status (int): The status code to return.
+            message (str, optional): The message to return. Defaults to None.
+            exception (Exception, optional): The exception to return. Defaults to None.
+
+        Returns:
+            bool: The result of the task run.
+        """
         # Delete the remote connection objects
         if self.remote_handlers:
             for remote_handler in self.remote_handlers:
                 remote_host = self._get_remote_host_name(remote_handler)
 
                 self.logger.log(
                     12,
                     f"[{remote_host}] Closing source connection for {remote_handler}",
                 )
                 remote_handler.tidy()
 
-        # Close the file handler
-        self.logger.info("Closing log file handler")
-        opentaskpy.logging.close_log_file(self.logger, self.overall_result)
-
-        # Throw an exception if we have one
-        if exception:
-            if callable(exception):
-                raise exception(message)
-            else:
-                raise Exception(message)
+        # Call super to do the rest
+        return super().return_result(status, message, exception)  # type: ignore[no-any-return]
 
-        return status == 0
-
-    def _get_remote_host_name(self, remote_handler):
+    def _get_remote_host_name(self, remote_handler: RemoteHandler) -> str:
         return (
-            remote_handler.remote_host
+            str(remote_handler.remote_host)
             if hasattr(remote_handler, "remote_host")
             else "REMOTE"
         )
 
-    def _set_remote_handlers(self):
+    def _set_remote_handlers(self) -> None:
+        """Set the remote handlers.
+
+        Determine which protocols are in use and create the appropriate objects for
+        each.
+        """
         # Based on the transfer definition, determine what to do first
         # Based on the remote protocol pick the appropriate remote handler
         # For each host, create a remote handler
         self.remote_handlers = []
         remote_protocol = self.execution_definition["protocol"]["name"]
         if remote_protocol == "ssh":
             for host in self.execution_definition["hosts"]:
@@ -77,20 +91,33 @@
             remote_handler = super()._get_handler_for_protocol(
                 remote_protocol, self.execution_definition
             )
             self.remote_handlers.append(remote_handler)
 
             super()._set_handler_vars(remote_protocol, remote_handler)
 
-    def run(self, kill_event=None):
+    def run(self, kill_event: threading.Event | None = None) -> bool:
+        """Run the execution.
+
+        Args:
+            kill_event (threading.Event, optional): An event to kill the execution. Defaults to None.
+
+        Returns:
+            bool: The result of the execution.
+        """
         self.logger.info("Running execution")
         environ["OTF_TASK_ID"] = self.task_id
 
         self._set_remote_handlers()
 
+        # Check that we have remote handlers, if not something has gone very wrong
+        if not self.remote_handlers:
+            self.logger.error("No remote handlers set")
+            return self.return_result(1, "No remote handlers set")
+
         # This is where we could potentially be waiting for a while. So,
         # for each remote handler, we should spawn a new thread to run
         # the command. Then we can wait for all threads to complete.
 
         ex = None
 
         with ThreadPoolExecutor(len(self.remote_handlers)) as executor:
@@ -122,15 +149,18 @@
                     executor.shutdown(wait=False)
                     # Make sure all threaeds are dead
                     for future in futures:
                         future.cancel()
                         # Check it's dead
                         if future.running():
                             self.logger.error(
-                                f"Thread {future} is still running after kill. Cannot kill a running thread. Will have to wait for it to complete. Consider altering the plugin so that it cannot block."
+                                f"Thread {future} is still running after kill. Cannot"
+                                " kill a running thread. Will have to wait for it to"
+                                " complete. Consider altering the plugin so that it"
+                                " cannot block."
                             )
 
                     return self.return_result(
                         1, "Execution(s) failed - Kill signal received"
                     )
 
                 # Break once all threads are done
@@ -140,36 +170,37 @@
             # Check the results
             failures = False
             for future in futures:
                 try:
                     result = future.result()
                     if not result:
                         failures = True
-                except Exception as e:
+                except Exception as e:  # pylint: disable=broad-exception-caught
                     self.overall_result = False
                     ex = e
                     self.logger.error("Thread returned exception")
                     # Ensure we log the exception
                     self.logger.exception(e)
                     failures = True
 
             if not failures:
                 self.overall_result = True
 
         if self.overall_result:
             return self.return_result(0, "All executions completed successfully")
-        else:
-            return self.return_result(1, "Execution(s) failed", ex)
 
-    def _execute(self, remote_handler):
-        result = remote_handler.execute()
+        return self.return_result(1, "Execution(s) failed", ex)
+
+    def _execute(self, remote_handler: RemoteHandler) -> bool:
+        result: bool = remote_handler.execute()
         remote_host = self._get_remote_host_name(remote_handler)
         self.logger.info(f"[{remote_host}] Execution returned {result}")
         return result
 
     # Destructor to handle when the execution is finished. Make sure the log file
     # gets renamed as appropriate
-    def __del__(self):
+    def __del__(self) -> None:
+        """Destructor to handle closing log file correctly."""
         self.logger.debug("Execution object deleted")
         # Close the file handler
         self.logger.info("Closing log file handler")
-        opentaskpy.logging.close_log_file(self.logger, self.overall_result)
+        opentaskpy.otflogging.close_log_file(self.logger, self.overall_result)
```

### Comparing `opentaskpy-0.8.1/src/opentaskpy/taskhandlers/transfer.py` & `opentaskpy-0.9.0/src/opentaskpy/taskhandlers/transfer.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,58 +1,97 @@
+"""Task handler for running transfers."""
 import random
 import shutil
+import threading
 import time
 from importlib import import_module
 from math import ceil, floor
 from os import environ, getpid, makedirs, path
 from sys import modules
+from typing import NamedTuple
 
-import opentaskpy.logging
+import opentaskpy.otflogging
 from opentaskpy import exceptions
+from opentaskpy.remotehandlers.remotehandler import RemoteTransferHandler
 from opentaskpy.taskhandlers.taskhandler import TaskHandler
 
 # Full transfers expect that the remote host has a base install of python3
 # We transfer over the wrapper script to the remote host and trigger it, which is responsible
 # for doing some of the more complex work, rather than triggering a tonne of shell commands
 
+
+class DefaultProtocolCharacteristics(NamedTuple):
+    """Class defining the configuration for default protocols."""
+
+    module: str
+    class_: str
+
+
 TASK_TYPE = "T"
 DEFAULT_PROTOCOL_MAP = {
-    "ssh": {"module": "opentaskpy.remotehandlers.ssh", "class": "SSHTransfer"},
-    "email": {"module": "opentaskpy.remotehandlers.email", "class": "EmailTransfer"},
+    "ssh": DefaultProtocolCharacteristics(
+        "opentaskpy.remotehandlers.ssh", "SSHTransfer"
+    ),
+    "email": DefaultProtocolCharacteristics(
+        "opentaskpy.remotehandlers.email", "EmailTransfer"
+    ),
 }
+DEFAULT_STAGING_DIR_BASE = "/tmp"  # nosec B108
 
 
-class Transfer(TaskHandler):
-    def __init__(self, global_config, task_id, transfer_definition):
+class Transfer(TaskHandler):  # pylint: disable=too-many-instance-attributes
+    """Task handler for running transfers."""
+
+    source_remote_handler: RemoteTransferHandler
+    dest_remote_handlers: RemoteTransferHandler = None
+    source_file_spec: dict
+    dest_file_specs: list[dict] | None = None
+    overall_result: bool = False
+
+    def __init__(self, global_config: dict, task_id: str, transfer_definition: dict):
+        """Create a new transfer task handler.
+
+        Args:
+            global_config (dict): Global configuration dictionary
+            task_id (str): Task ID
+            transfer_definition (dict): Transfer definition
+        """
         self.task_id = task_id
         self.transfer_definition = transfer_definition
-        self.source_remote_handler = None
-        self.dest_remote_handlers = None
-        self.source_file_spec = None
-        self.dest_file_specs = None
-        self.overall_result = False
 
-        self.local_staging_dir = f"/tmp/staging/{getpid()}.{random.randint(0, 1000000)}"
+        # Set up the local staging directory
+        # Allow for a custom staging directory to be set via environment variable
+        staging_dir_name = f"OTF_STAGING_{getpid()}.{random.randint(0, 1000000)}"
+        if "OTF_STAGING_DIR" in environ:
+            self.local_staging_dir = f"{environ['OTF_STAGING_DIR']}/{staging_dir_name}"
+        else:
+            self.local_staging_dir = f"/{DEFAULT_STAGING_DIR_BASE}/{staging_dir_name}"
 
-        self.logger = opentaskpy.logging.init_logging(
+        self.logger = opentaskpy.otflogging.init_logging(
             "opentaskpy.taskhandlers.transfer", self.task_id, TASK_TYPE
         )
 
         super().__init__(global_config)
 
-    def return_result(self, status, message=None, exception=None):
-        if message:
-            if status == 0:
-                self.logger.info(message)
-            else:
-                self.logger.error(message)
-
-        if status == 0:
-            self.overall_result = True
-
+    def return_result(
+        self,
+        status: int,
+        message: str | None = None,
+        exception: Exception | None = None,
+    ) -> bool:
+        """Return the result of the task run.
+
+        Args:
+            status (int): The status code to return.
+            message (str, optional): The message to return. Defaults to None.
+            exception (Exception, optional): The exception to return. Defaults to None.
+
+        Returns:
+            bool: The result of the task run.
+        """
         # Delete the remote connection objects
         if self.source_remote_handler:
             self.logger.log(12, "Closing source connection")
             self.source_remote_handler.tidy()
         if self.dest_remote_handlers:
             for remote_handler in self.dest_remote_handlers:
                 self.logger.log(12, f"Closing dest connection for {remote_handler}")
@@ -61,34 +100,28 @@
         # Remove local staging directory if it exists
         if path.exists(self.local_staging_dir):
             self.logger.log(
                 12, f"Removing local staging directory {self.local_staging_dir}"
             )
             shutil.rmtree(self.local_staging_dir)
 
-        self.logger.info("Closing log file handler")
-        opentaskpy.logging.close_log_file(self.logger, self.overall_result)
-
-        # Throw an exception if we have one
-        if exception:
-            raise exception(message)
+        # Call super to do the rest
+        return super().return_result(status, message, exception)  # type: ignore[no-any-return]
 
-        return status == 0
-
-    def _get_default_class(self, protocol_name):
-        class_name = DEFAULT_PROTOCOL_MAP[protocol_name]["class"]
-        module_name = DEFAULT_PROTOCOL_MAP[protocol_name]["module"]
+    def _get_default_class(self, protocol_name: str) -> type:
+        class_name = DEFAULT_PROTOCOL_MAP[protocol_name].class_
+        module_name = DEFAULT_PROTOCOL_MAP[protocol_name].module
 
         # Load module
         if module_name not in modules:
             import_module(module_name)
 
-        return getattr(modules[module_name], class_name)
+        return getattr(modules[module_name], class_name)  # type: ignore[no-any-return]
 
-    def _set_remote_handlers(self):
+    def _set_remote_handlers(self) -> None:
         # Based on the transfer definition, determine what to do first
         self.source_file_spec = self.transfer_definition["source"]
         source_protocol = self.source_file_spec["protocol"]["name"]
 
         # Create a list of destination file specs
         if (
             "destination" in self.transfer_definition
@@ -127,24 +160,33 @@
                     remote_handler = super()._get_handler_for_protocol(
                         remote_protocol, dest_file_spec
                     )
 
                 self.dest_remote_handlers.append(remote_handler)
                 super()._set_handler_vars(remote_protocol, remote_handler)
 
-    def run(self, kill_event=None):
+    def run(self, kill_event: threading.Event | None = None) -> bool:  # noqa: C901
+        """Run the transfer task.
+
+        Args:
+            kill_event (threading.Event, optional): Event to kill the task. Defaults to None.
+
+        Returns:
+            bool: The result of the task run.
+        """
         self.logger.info("Running transfer")
         environ["OTF_TASK_ID"] = self.task_id
 
         self._set_remote_handlers()
 
         # If log watching, do that first
         if "logWatch" in self.source_file_spec:
             self.logger.info(
-                f"Performing a log watch of {self.source_file_spec['logWatch']['directory']}/{self.source_file_spec['logWatch']['log']}"
+                "Performing a log watch of"
+                f" {self.source_file_spec['logWatch']['directory']}/{self.source_file_spec['logWatch']['log']}"
             )
 
             if self.source_remote_handler.init_logwatch() != 0:
                 return self.return_result(
                     1, "Logwatch init failed", exception=exceptions.LogWatchInitError
                 )
 
@@ -162,31 +204,30 @@
             # Now we start the loop to monitor the log file
             start_time = time.time()
             found_log_entry = False
             while floor(time.time() - start_time) <= timeout_seconds:
                 if self.source_remote_handler.do_logwatch() == 0:
                     found_log_entry = True
                     break
-                else:
-                    remaining_seconds = ceil(
-                        (start_time + timeout_seconds) - time.time()
-                    )
-                    if remaining_seconds == 0:
-                        break
 
-                    # If the sleep time is longer than the time remaining, sleep for that long instead
-                    if remaining_seconds < sleep_seconds:
-                        actual_sleep_seconds = remaining_seconds
-                    else:
-                        actual_sleep_seconds = sleep_seconds
+                remaining_seconds = ceil((start_time + timeout_seconds) - time.time())
+                if remaining_seconds == 0:
+                    break
 
-                    self.logger.info(
-                        f"No entry found in log. Sleeping for {sleep_seconds} secs. {remaining_seconds} seconds remain"
-                    )
-                    time.sleep(actual_sleep_seconds)
+                # If the sleep time is longer than the time remaining, sleep for that long instead
+                if remaining_seconds < sleep_seconds:
+                    actual_sleep_seconds = remaining_seconds
+                else:
+                    actual_sleep_seconds = sleep_seconds
+
+                self.logger.info(
+                    f"No entry found in log. Sleeping for {sleep_seconds} secs."
+                    f" {remaining_seconds} seconds remain"
+                )
+                time.sleep(actual_sleep_seconds)
 
             if found_log_entry:
                 self.logger.info("Found pattern in log file")
             else:
                 return self.return_result(
                     1,
                     f"No log entry found after {timeout_seconds} seconds",
@@ -204,15 +245,15 @@
             sleep_seconds = (
                 10
                 if "sleepTime" not in self.source_file_spec["fileWatch"]
                 else self.source_file_spec["fileWatch"]["sleepTime"]
             )
 
             start_time = time.time()
-            remote_files = []
+            remote_files: dict = {}
 
             # Determine if we're doing a plain filewatch, or looking for a different file to what we are transferring
             watch_directory = (
                 self.source_file_spec["fileWatch"]["directory"]
                 if "directory" in self.source_file_spec["fileWatch"]
                 else self.source_file_spec["directory"]
             )
@@ -228,58 +269,57 @@
 
             while (
                 not remote_files and floor(time.time() - start_time) <= timeout_seconds
             ):
                 remote_files = self.source_remote_handler.list_files(
                     directory=watch_directory, file_pattern=watch_file_pattern
                 )
-                # TODO: #5 Change all references to remote_files to expect a generato
+                # TODO: #5 Change all references to remote_files to expect a generator # pylint: disable=fixme
                 if remote_files:
                     self.logger.info("Filewatch found remote file(s)")
                     break
-                else:
-                    remaining_seconds = ceil(
-                        (start_time + timeout_seconds) - time.time()
-                    )
-                    if remaining_seconds == 0:
-                        break
 
-                    # If the sleep time is longer than the time remaining, sleep for that long instead
-                    if remaining_seconds < sleep_seconds:
-                        actual_sleep_seconds = remaining_seconds
-                    else:
-                        actual_sleep_seconds = sleep_seconds
+                remaining_seconds = ceil((start_time + timeout_seconds) - time.time())
+                if remaining_seconds == 0:
+                    break
 
-                    self.logger.info(
-                        f"No files found. Sleeping for {sleep_seconds} secs. {remaining_seconds} seconds remain"
-                    )
-                    time.sleep(actual_sleep_seconds)
+                # If the sleep time is longer than the time remaining, sleep for that long instead
+                if remaining_seconds < sleep_seconds:
+                    actual_sleep_seconds = remaining_seconds
+                else:
+                    actual_sleep_seconds = sleep_seconds
+
+                self.logger.info(
+                    f"No files found. Sleeping for {sleep_seconds} secs."
+                    f" {remaining_seconds} seconds remain"
+                )
+                time.sleep(actual_sleep_seconds)
 
             if (
                 remote_files
                 and "watchOnly" in self.source_file_spec["fileWatch"]
                 and self.source_file_spec["fileWatch"]["watchOnly"]
             ):
-                return self.return_result("0", "Just performing filewatch")
-            elif not remote_files:
+                return self.return_result(0, "Just performing filewatch")
+            if not remote_files:
                 # Only error if error is not set to false
                 if (
                     "error" in self.source_file_spec
                     and not self.source_file_spec["error"]
                 ):
                     self.logger.info(
                         "No files found after timeout, but error is set to false"
                     )
                     return self.return_result(0, "No files found")
-                else:
-                    return self.return_result(
-                        1,
-                        f"No files found after {timeout_seconds} seconds",
-                        exception=exceptions.RemoteFileNotFoundError,
-                    )
+
+                return self.return_result(
+                    1,
+                    f"No files found after {timeout_seconds} seconds",
+                    exception=exceptions.RemoteFileNotFoundError,
+                )
 
         # Determine what needs to be transferred
 
         remote_files = self.source_remote_handler.list_files()
 
         # Loop through the returned files to see if they match the file age and size spec (if defined)
         if "conditionals" in self.source_file_spec and remote_files:
@@ -302,21 +342,23 @@
                         else None
                     )
 
                     file_size = remote_files[remote_file]["size"]
 
                     if min_size and file_size <= min_size:
                         self.logger.info(
-                            f"File is too small: Min size: [{min_size} B] Actual size: [{file_size} B]"
+                            f"File is too small: Min size: [{min_size} B] Actual size:"
+                            f" [{file_size} B]"
                         )
                         meets_condition = False
 
                     if max_size and file_size >= max_size:
                         self.logger.info(
-                            f"File is too big: Max size: [{max_size} B] Actual size: [{file_size} B]"
+                            f"File is too big: Max size: [{max_size} B] Actual size:"
+                            f" [{file_size} B]"
                         )
                         meets_condition = False
 
                 if "age" in self.source_file_spec["conditionals"]:
                     min_age = (
                         None
                         if "gt" not in self.source_file_spec["conditionals"]["age"]
@@ -329,69 +371,80 @@
                     )
 
                     file_modified_time = remote_files[remote_file]["modified_time"]
                     file_age = time.time() - file_modified_time
 
                     self.logger.log(
                         12,
-                        f"Checking file age - Last modified time: {time.ctime(file_modified_time)} - Age in secs: {file_age} secs",
+                        (
+                            "Checking file age - Last modified time:"
+                            f" {time.ctime(file_modified_time)} - Age in secs:"
+                            f" {file_age} secs"
+                        ),
                     )
 
                     if min_age and file_age <= min_age:
                         self.logger.info(
-                            f"File is too new: Min age: [{min_age} secs] Actual age: [{file_age} secs]"
+                            f"File is too new: Min age: [{min_age} secs] Actual age:"
+                            f" [{file_age} secs]"
                         )
                         meets_condition = False
 
                     if max_age and file_age >= max_age:
                         self.logger.info(
-                            f"File is too old: Max age: [{max_age} secs] Actual age: [{file_age} secs]"
+                            f"File is too old: Max age: [{max_age} secs] Actual age:"
+                            f" [{file_age} secs]"
                         )
                         meets_condition = False
 
                 if not meets_condition:
                     remote_files.pop(remote_file)
 
         if not remote_files:
             if "error" in self.source_file_spec and not self.source_file_spec["error"]:
                 return self.return_result(
                     0,
-                    "No remote files could be found to transfer. But not erroring due to config",
-                    exception=exceptions.FilesDoNotMeetConditionsError,
-                )
-            else:
-                return self.return_result(
-                    1,
-                    "No remote files could be found to transfer",
+                    (
+                        "No remote files could be found to transfer. But not erroring"
+                        " due to config"
+                    ),
                     exception=exceptions.FilesDoNotMeetConditionsError,
                 )
-        else:
-            self.logger.info("Found the following file(s) that match all requirements:")
-            for file in remote_files:
-                self.logger.info(f" * {file}")
-
-            # If there's a destination file spec, then we need to transfer the files
-            if self.dest_file_specs:
-                # Loop through all dest_file specs and see if there are any transfers where the source and dest protocols are different
-                # If there are, then we need to do a pull transfer first, then a push transfer
-                different_protocols = False
-                i = 0
-                for dest_file_spec in self.dest_file_specs:
-                    if (
+
+            return self.return_result(
+                1,
+                "No remote files could be found to transfer",
+                exception=exceptions.FilesDoNotMeetConditionsError,
+            )
+
+        self.logger.info("Found the following file(s) that match all requirements:")
+        for file in remote_files:
+            self.logger.info(f" * {file}")
+
+        # If there's a destination file spec, then we need to transfer the files
+        if self.dest_file_specs:
+            # Loop through all dest_file specs and see if there are any transfers where the source and dest protocols are different
+            # If there are, then we need to do a pull transfer first, then a push transfer
+            different_protocols = False
+            i = 0
+            for dest_file_spec in self.dest_file_specs:
+                if (
+                    (
                         "transferType" not in dest_file_spec
                         or dest_file_spec["transferType"] == "push"
-                        # And the destination and source remote handler classes are the same
-                        and (
-                            self.source_remote_handler.__class__
-                            != self.dest_remote_handlers[i].__class__
-                        )
-                    ):
-                        different_protocols = True
-                        i += 1
-                        break
+                    )
+                    # And the destination and source remote handler classes are not the same
+                    and (
+                        self.source_remote_handler.__class__
+                        != self.dest_remote_handlers[i].__class__
+                    )
+                ):
+                    different_protocols = True
+                    i += 1
+                    break
 
                 # If there are differences, download the file locally first
                 # so it's ready to upload to multiple destinations at once
                 if different_protocols or (
                     "transferType" in dest_file_spec
                     and dest_file_spec["transferType"] == "proxy"
                 ):
@@ -403,128 +456,130 @@
                     if transfer_result != 0:
                         return self.return_result(
                             1,
                             "Pull to worker from remote source errored",
                             exception=exceptions.RemoteTransferError,
                         )
 
-                i = 0
-                for dest_file_spec in self.dest_file_specs:
-                    # Handle the push transfers first
-                    associated_dest_remote_handler = self.dest_remote_handlers[i]
-                    # If this is a default push transfer, and both source and dest protocols are the same
-                    if (
-                        "transferType" not in dest_file_spec
-                        or dest_file_spec["transferType"] == "push"
-                        # And the destination and source remote handler classes are the same
-                    ) and not different_protocols:
-                        transfer_result = self.source_remote_handler.transfer_files(
-                            remote_files,
-                            dest_file_spec,
-                            dest_remote_handler=associated_dest_remote_handler,
-                        )
-                        if transfer_result != 0:
-                            return self.return_result(
-                                1,
-                                "Remote transfer errored",
-                                exception=exceptions.RemoteTransferError,
-                            )
-
-                        self.logger.info("Transfer completed successfully")
-                    # If this is a default push transfer, and source and dest protocols are different
-                    elif (
-                        "transferType" in dest_file_spec
-                        and (
-                            dest_file_spec["transferType"] == "push"
-                            or dest_file_spec["transferType"] == "proxy"
-                        )
-                    ) or different_protocols:
-                        self.logger.debug(
-                            "Transfer protocols are different, or proxy transfer is requested"
-                        )
-
-                        transfer_result = (
-                            associated_dest_remote_handler.push_files_from_worker(
-                                self.local_staging_dir
-                            )
-                        )
-
-                        if transfer_result != 0:
-                            return self.return_result(
-                                1,
-                                "Push of files to destination errored",
-                                exception=exceptions.RemoteTransferError,
-                            )
-
-                    elif (
-                        "transferType" in dest_file_spec
-                        and dest_file_spec["transferType"] == "pull"
-                    ):
-                        transfer_result = associated_dest_remote_handler.pull_files(
-                            remote_files, self.source_file_spec
-                        )
-                        if transfer_result != 0:
-                            return self.return_result(
-                                1,
-                                "Remote PULL transfer errored",
-                                exception=exceptions.RemoteTransferError,
-                            )
-
-                        self.logger.info("Transfer completed successfully")
-
-                    # Handle any ownership and permissions changes
-                    if dest_file_spec["protocol"]["name"] == "ssh":
-                        move_result = self.dest_remote_handlers[
-                            i
-                        ].move_files_to_final_location(remote_files)
-                        if move_result != 0:
-                            return self.return_result(
-                                1,
-                                "Error moving file into final location",
-                                exception=exceptions.RemoteTransferError,
-                            )
-
-                    # Create any flag files that might need creating
-                    if "flags" in dest_file_spec:
-                        flag_result = self.dest_remote_handlers[i].create_flag_files()
-                        if flag_result != 0:
-                            return self.return_result(
-                                1,
-                                "Error creating flag files",
-                                exception=exceptions.RemoteTransferError,
-                            )
+            i = 0
+            for dest_file_spec in self.dest_file_specs:
+                # Handle the push transfers first
+                associated_dest_remote_handler = self.dest_remote_handlers[i]
+                # If this is a default push transfer, and both source and dest protocols are the same
+                if (
+                    "transferType" not in dest_file_spec
+                    or dest_file_spec["transferType"] == "push"
+                    # And the destination and source remote handler classes are the same
+                ) and not different_protocols:
+                    transfer_result = self.source_remote_handler.transfer_files(
+                        remote_files,
+                        dest_file_spec,
+                        dest_remote_handler=associated_dest_remote_handler,
+                    )
+                    if transfer_result != 0:
+                        return self.return_result(
+                            1,
+                            "Remote transfer errored",
+                            exception=exceptions.RemoteTransferError,
+                        )
 
-                    i += 1
+                    self.logger.info("Transfer completed successfully")
+                # If this is a default push transfer, and source and dest protocols are different
+                elif (
+                    "transferType" in dest_file_spec
+                    and (
+                        dest_file_spec["transferType"] == "push"
+                        or dest_file_spec["transferType"] == "proxy"
+                    )
+                ) or different_protocols:
+                    self.logger.debug(
+                        "Transfer protocols are different, or proxy transfer is"
+                        " requested"
+                    )
 
-                if different_protocols:
-                    self.logger.debug("Removing local staging directory")
-                    shutil.rmtree(self.local_staging_dir)
-            else:
-                self.logger.info("Performing filewatch only")
+                    transfer_result = (
+                        associated_dest_remote_handler.push_files_from_worker(
+                            self.local_staging_dir
+                        )
+                    )
 
-            if "postCopyAction" in self.source_file_spec:
-                try:
-                    pca_result = self.source_remote_handler.handle_post_copy_action(
-                        remote_files
-                    )
-                except Exception as e:
-                    pca_result = 1
-                    return self.return_result(
-                        1,
-                        "Error performing post copy action",
-                        exception=e,
-                    )
-                if pca_result != 0:
-                    return self.return_result(
-                        1,
-                        "Error performing post copy action",
-                        exception=exceptions.RemoteTransferError,
+                    if transfer_result != 0:
+                        return self.return_result(
+                            1,
+                            "Push of files to destination errored",
+                            exception=exceptions.RemoteTransferError,
+                        )
+
+                elif (
+                    "transferType" in dest_file_spec
+                    and dest_file_spec["transferType"] == "pull"
+                ):
+                    transfer_result = associated_dest_remote_handler.pull_files(
+                        remote_files, self.source_file_spec
                     )
+                    if transfer_result != 0:
+                        return self.return_result(
+                            1,
+                            "Remote PULL transfer errored",
+                            exception=exceptions.RemoteTransferError,
+                        )
+
+                    self.logger.info("Transfer completed successfully")
+
+                # Handle any ownership and permissions changes
+                if dest_file_spec["protocol"]["name"] == "ssh":
+                    move_result = self.dest_remote_handlers[
+                        i
+                    ].move_files_to_final_location(remote_files)
+                    if move_result != 0:
+                        return self.return_result(
+                            1,
+                            "Error moving file into final location",
+                            exception=exceptions.RemoteTransferError,
+                        )
+
+                # Create any flag files that might need creating
+                if "flags" in dest_file_spec:
+                    flag_result = self.dest_remote_handlers[i].create_flag_files()
+                    if flag_result != 0:
+                        return self.return_result(
+                            1,
+                            "Error creating flag files",
+                            exception=exceptions.RemoteTransferError,
+                        )
+
+                i += 1
+
+            if different_protocols:
+                self.logger.debug("Removing local staging directory")
+                shutil.rmtree(self.local_staging_dir)
+        else:
+            self.logger.info("Performing filewatch only")
+
+        if "postCopyAction" in self.source_file_spec:
+            try:
+                pca_result = self.source_remote_handler.handle_post_copy_action(
+                    remote_files
+                )
+            except Exception as e:  # pylint: disable=broad-exception-caught
+                pca_result = 1
+                return self.return_result(
+                    1,
+                    "Error performing post copy action",
+                    exception=e,
+                )
+            if pca_result != 0:
+                return self.return_result(
+                    1,
+                    "Error performing post copy action",
+                    exception=exceptions.RemoteTransferError,
+                )
 
-            return self.return_result(0)
+        return self.return_result(0)
 
     # Destructor to handle when the transfer is finished. Make sure the log file
     # gets renamed as appropriate
-    def __del__(self):
+    def __del__(self) -> None:
+        """Destructor to handle closing log file correctly."""
         self.logger.debug("Transfer object deleted")
         self.logger.info("Closing log file handler")
-        opentaskpy.logging.close_log_file(self.logger, self.overall_result)
+        opentaskpy.otflogging.close_log_file(self.logger, self.overall_result)
```

### Comparing `opentaskpy-0.8.1/src/opentaskpy.egg-info/PKG-INFO` & `opentaskpy-0.9.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,40 +1,21 @@
-Metadata-Version: 2.1
-Name: opentaskpy
-Version: 0.8.1
-Summary: A framework for automation execution of commands and transferring files between hosts
-Author-email: Adam McDonagh <adam@elitemonkey.net>
-License: GPLv3
-Project-URL: Homepage, https://github.com/adammcdonagh/open-task-framework
-Project-URL: Bug Tracker, https://github.com/adammcdonagh/open-task-framework/issues
-Project-URL: Changelog, https://github.com/adammcdonagh/open-task-framework/blob/main/CHANGELOG.md
-Keywords: automation,task,framework,scheduling,ssh,sftp,remote,execution,command
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Operating System :: POSIX
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE
-License-File: AUTHORS
-
-
 ![unittest status](https://github.com/adammcdonagh/open-task-framework/actions/workflows/main.yml/badge.svg?event=push)
 
 <h1>Open Task Framework (opentaskpy)</h1>
 
 - [Installation](#installation)
+  - [Example Deployment](#example-deployment)
 - [Configuration](#configuration)
   - [Command Line Arguments](#command-line-arguments)
   - [Environment Variables](#environment-variables)
   - [Logging](#logging)
   - [Variables](#variables)
   - [Runtime Overrides](#runtime-overrides)
   - [Lookup plugins](#lookup-plugins)
-      - [Adding your own](#adding-your-own)
+    - [Adding your own](#adding-your-own)
     - [Example Variables](#example-variables)
 - [Task Definitions](#task-definitions)
   - [Transfers](#transfers)
   - [Executions](#executions)
   - [Batches](#batches)
 - [Development](#development)
   - [Quickstart for development](#quickstart-for-development)
@@ -46,25 +27,27 @@
     - [Addons](#addons)
 
 Open Task Framework (OTF) is a Python based framework to make it easy to run predefined file transfers and scripts/commands on remote machines.
 
 Currently the framework is primarily based around being able to use SSH to communicate with remote hosts in order to manipulate files and run commands. This is done via the use of SSH keys, which must be set up in advance.
 
 OTF has 3 main concepts for tasks. These are:
-* Transfers
-* Executions
-* Batches
+
+- Transfers
+- Executions
+- Batches
 
 For more details, see the [task types](docs/task-types.md) doc
 
 # Installation
 
 OTF can be run either as an installed script, or via a docker container
 
 Install via pip:
+
 ```shell
 pip install opentaskpy
 ```
 
 The `task-run` script will be added to your PATH, and you can invoke it directly.
 
 To run via docker, use the `Dockerfile` to create your own base image using just the standard opentaskpy library. However if you want to install addons, you'll need to customise this, to install the additional packages first, before bundling it as a Docker image.
@@ -74,14 +57,22 @@
 docker run --rm --volume /opt/otf/cfg:/cfg --volume /var/log/otf:/logs--volume /home/<USER>/.ssh/id_rsa:/id_rsa -e OTF_SSH_KEY=/id_rsa -e OTF_LOG_DIRECTORY=/logs task-run -t <TASK NAME> -c /cfg # Run a task
 ```
 
 The default `opentaskpy` library is only really designed to use SSH for executions and file transfers. To do this, you need to make sure that the host/container that is running the `task-run` script has a private RSA key, that is trusted on all remote hosts that you're running against.
 
 An environment variable `OTF_SSH_KEY` can be used to define a default SSH key to use for all SSH connectivity. This can be overridden at the transfer/execution level by specifying a `keyFile` in the `credentials` section of the protocol definition.
 
+## Example Deployment
+
+This is an example deployment for using OTF in an AWS environment, using BMC Control-M as the job scheduler. Control-M could be replaced with any job scheduler, AWS EventBridge for example, depending on your requirements.
+
+![AWS Deployment](docs/aws.png)
+
+"Admin/Status Portal" currently does not exist, and is a placeholder for a potential further project to visualise the OTF configs, as well as including real-time job statuses from the job scheduler.
+
 # Configuration
 
 There are several ways to customise the running of tasks.
 
 ## Command Line Arguments
 
 The following details the syntax of the `task-run` command:
@@ -121,18 +112,20 @@
 
 In order for the process to run, you must have at least one task, and a `variables.json.j2` file, even if it's just an empty object definition
 
 ## Environment Variables
 
 These are some environment variables that can be used to customise the behaviour of the application. There are some internally used variables too, but changing them without a full understanding of the code is not advised.
 
-   * `OTF_NO_LOG` - Disable logging to file. Only log to stderr
-   * `OTF_LOG_DIRECTORY` - Path under which log files are written
-   * `OTF_RUN_ID` - (meant for internal use) An aggregator for log files. When set, all log files for a run will go under this sub directory. E.g. running a batch, all execution and transfer logs will be dropped into this sub directory, rather than a directory for each task name. This is equivalent to using `-r` or `--runId` command line arguments, which is generally preferred.
-   * `OTF_SSH_KEY` - The private SSH key to use by default for all SSH connections. This is essential when using a basic docker container to trigger OTF. If not specified, it will default to use any private SSH keys available to the user executing the application.
+- `OTF_NO_LOG` - Disable logging to file. Only log to stderr
+- `OTF_LOG_DIRECTORY` - Path under which log files are written
+- `OTF_RUN_ID` - (meant for internal use) An aggregator for log files. When set, all log files for a run will go under this sub directory. E.g. running a batch, all execution and transfer logs will be dropped into this sub directory, rather than a directory for each task name. This is equivalent to using `-r` or `--runId` command line arguments, which is generally preferred.
+- `OTF_SSH_KEY` - The private SSH key to use by default for all SSH connections. This is essential when using a basic docker container to trigger OTF. If not specified, it will default to use any private SSH keys available to the user executing the application.
+- `OTF_REMOTE_SCRIPT_BASE_DIR` - Alternative location to drop the temporary `transfer.py` script on remote hosts using SSH protocol. Default is `/tmp`
+- `OTF_STAGING_DIR` - Staging base directory to place files before they're dropped into their final location. Default is `/tmp`
 
 ## Logging
 
 By default, OTF will log to a directory called `logs` in the current working directory. For the docker containers, unless overridden by `OTF_LOG_DIRECTORY`, it will write to `/logs` using a symlink at `/app/logs`
 
 ## Variables
 
@@ -146,14 +139,15 @@
 
 ## Runtime Overrides
 
 Sometimes you might want to override the current date, or something specific about a file transfer when you manually run a task. This can be done using environment variables.
 
 Standard global variables can be overridden simply by setting an environment variable that matches the name of the variable you want to override e.g. `export DD=01`
 In the log output, you'll see something like this:
+
 ```
 Overriding global variable (DD: 05) with environment variable (01)
 ```
 
 To override task specific values, you can use the following format in the environment variable name:
 `OTF_OVERRIDE_<TASK_TYPE>_<ATTRIBUTE>_<ATTRIBUTE>_<ATTRIBUTE>`
 
@@ -161,45 +155,49 @@
 
 Case doesn't matter here. For attributes that are nested within an array, you can specify the array index
 
 e.g. `OTF_OVERRIDE_TRANSFER_DESTINATION_0_PROTOCOL_CREDENTIALS_USERNAME`
 
 Again this will be logged to show you that the override is being applied.
 
-
 ## Lookup plugins
 
 Static variables are useful, however sometimes you need to look up something a bit more dynamic, or secret, that you don't want to hard code into the variables file.
 
 There are 2 default lookup plugins available:
 
-* File
-* HTTP JSON
+- File
+- HTTP JSON
 
 The file plugin will load the content of a file into the variable e.g.
+
 ```jinja
 "{{ lookup('file', path='/tmp/variable_lookup.txt') }}"
 ```
 
 The HTTP JSON plugin will perform a very basic HTTP GET request, expecting a JSON response. The value to extract is defined by a jsonpath e.g.
+
 ```jinja
 "{{ lookup('http_json', url='https://jsonplaceholder.typicode.com/posts/1', jsonpath='$.title') }}"
 ```
+
 This will hit the typicode.com side, and extract the title attribute from from the returned JSON file
 
 #### Adding your own
 
 OTF will look for plugins that are either available as an installed module (under the `opentaskpy.plugins.lookup` namespace), or dropped in a `plugins` under the config directory.
 
 An example Python module might be: `opentaskpy.plugins.lookup.aws.ssm`. This can then be referenced as a variable in a template like so:
+
 ```jinja
 "{{ lookup('aws.ssm', name='my_test_param') }}"
 ```
 
 Alternatively a lookup plugin could be placed under `cfg/plugins` named `my_lookup.py`, and used in a template:
+
 ```jinja
 "{{ lookup('my_lookup', name='my_param') }}"
 ```
 
 ### Example Variables
 
 Below are examples of some useful variables to start with:
@@ -306,37 +304,34 @@
         }
       }
     }
   ]
 }
 ```
 
-An explaination of what's going on in the order it will handled:
+An explanation of what's going on in the order it will handled:
 
 1. Tail the log file matching named: `/tmp/testFiles/src/log{{ YYYY }}Watch1.log` for lines matching containing the regex `someText[0-9]`, for up to 15 seconds, before giving up.
 2. Poll for a file matching the regex `/tmp/testFiles/src/fileWatch\.txt` for up to 15 seconds.
 3. Find all files matching the regex `/tmp/testFiles/src/.*\.txt`, with the conditions that the are >10B and <20B in size, as well as being older than 60 seconds, but newer than 600 seconds since last modification
 4. Transfer the files that were found to 2 destinations.
    1. The first destination is a simple SCP from `HOST_A` to `HOST_B` where the file is placed under `/tmp/testFiles/dest`. The group ownership of the file(s) is then set to `operator`
    2. The second destination is done via a pull from the destination server into the same directory. The SCP connects to `HOST_A` as `transferUsername`. Once the file has been retrieved, it is renamed using the following regex match `^(.*)\.txt$` and substitution `\1-2.txt`
 5. Transferred files are moved into `/tmp/testFiles/archive` on `HOST_A`
 
-
 ## Executions
 
 Executions are the simplest task to configure. They consist of a list of hosts to run on, the username to run/connect as, and the command to run.
 
 Executions do not currently have a timeout, so can in theory run forever, or until they are killed. If a timeout is required, either use a wrapper script on the host the command is being executed on, or they should be wrapped inside a batch.
 
 ```json
 {
   "type": "execution",
-  "hosts": [
-    "{{ HOST_A }}"
-  ],
+  "hosts": ["{{ HOST_A }}"],
   "directory": "/tmp/testFiles/src",
   "command": "touch touchedFile.txt",
   "protocol": {
     "name": "ssh",
     "credentials": {
       "username": "{{ SSH_USERNAME }}"
     }
@@ -346,59 +341,61 @@
 
 The above is running the command `touch touchedFile.txt` on `{{ HOST_A }}`, from within the `/tmp/testFiles/src` directory.
 
 If multiple `hosts` are defined, a thread is spawned in parallel for each host. If the command fails on any of the hosts in the list, it will cause the task run to fail, once all processes have returned a result.
 
 ## Batches
 
-Batches are a little more complex. They do not contain any task definitions, only the list, and order of excecution for each task.
+Batches are a little more complex. They do not contain any task definitions, only the list, and order of execution for each task.
 
 A batch task can have multiple options set that determine the execution order and conditions, as well as how failures and task reruns are handled.
 
 Each task in a batch has an `order_id`, this is a unique ID for each task, and is primarily used to define dependencies.
 
 `dependencies` can be applied to any task, and are simply a list of other tasks that must be completed before it is triggered.
 
 `continue_on_fail` is a boolean that defines whether a failure would cause the whole batch to fail immediately (after existing tasks have finished executing), or whether following steps get run. This defaults to false if not defined.
 
 `retry_on_rerun` is a boolean that determines whether a successful task is run a second time following a failed run. If a batch exits with a failure, and then the script is reun later on that same day, by default only the steps that failed will be run. All steps can be forced to run by setting this to true
 
 `timeout` specifies the number of seconds a task is allowed to be running before it gets terminated. This counts as a failure. The default timeout, if not specified is 300 seconds.
 
-
 # Development
 
 This repo has been primarily configured to work with GitHub Codespaces devcontainers, though it can obviously be used directly on your machine too.
 
 Dev and runtime packages are defined via pipenv, with a `requirements.txt` for the runtime package requirements
 
 ## Quickstart for development
 
-* Clone this repo
-* pip install pipenv
-* pipenv --python 3.10 && pipenv install && cd src && pipenv install --editable .
+- Clone this repo
+- pip install pipenv
+- pipenv --python 3.10 && pipenv install && cd src && pipenv install --editable .
 
 ### Building and uploading to PyPi
 
 ```bash
 python3 -m build
 python3 -m twine upload --repository testpypi dist/*
 ```
 
 ## Official Addons/Plugins
 
 Here's a list of official addons:
+
 ### [otf-addons-aws](https://github.com/adammcdonagh/otf-addons-aws)
 
 Provides transfer and execution addons:
-   * Remote handler for interacting with AWS S3 buckets
-   * Remote handler for executing AWS Lambda functions
+
+- Remote handler for interacting with AWS S3 buckets
+- Remote handler for executing AWS Lambda functions
 
 Lookup plugins:
-   * Support for AWS SSM Parameter Store for retrieving global variables
+
+- Support for AWS SSM Parameter Store for retrieving global variables
 
 ## Developing your own addon/plugin
 
 ### Lookup Plugins
 
 Plugins are very simple. They simply need a `run` function, and to return the required variable based on a list of kwargs provided within the config template.
```

### Comparing `opentaskpy-0.8.1/src/opentaskpy.egg-info/SOURCES.txt` & `opentaskpy-0.9.0/src/opentaskpy.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 AUTHORS
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 src/opentaskpy/exceptions.py
-src/opentaskpy/logging.py
-src/opentaskpy/task_run.py
+src/opentaskpy/otflogging.py
+src/opentaskpy/taskrun.py
 src/opentaskpy.egg-info/PKG-INFO
 src/opentaskpy.egg-info/SOURCES.txt
 src/opentaskpy.egg-info/dependency_links.txt
 src/opentaskpy.egg-info/entry_points.txt
 src/opentaskpy.egg-info/requires.txt
 src/opentaskpy.egg-info/top_level.txt
 src/opentaskpy/cli/task_run.py
@@ -30,15 +30,15 @@
 src/opentaskpy/config/schemas/transfer/ssh_source/conditionals.json
 src/opentaskpy/config/schemas/transfer/ssh_source/fileWatch.json
 src/opentaskpy/config/schemas/transfer/ssh_source/logWatch.json
 src/opentaskpy/config/schemas/transfer/ssh_source/postCopyAction.json
 src/opentaskpy/config/schemas/transfer/ssh_source/protocol.json
 src/opentaskpy/plugins/lookup/file.py
 src/opentaskpy/plugins/lookup/http_json.py
-src/opentaskpy/plugins/lookup/random.py
+src/opentaskpy/plugins/lookup/random_number.py
 src/opentaskpy/remotehandlers/__init__.py
 src/opentaskpy/remotehandlers/email.py
 src/opentaskpy/remotehandlers/remotehandler.py
 src/opentaskpy/remotehandlers/ssh.py
 src/opentaskpy/remotehandlers/scripts/transfer.py
 src/opentaskpy/taskhandlers/__init__.py
 src/opentaskpy/taskhandlers/batch.py
```

### Comparing `opentaskpy-0.8.1/tests/test_batch_schema_validate.py` & `opentaskpy-0.9.0/tests/test_batch_schema_validate.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# pylint: skip-file
 import pytest
 
 from opentaskpy.config.schemas import validate_batch_json
 
 
 @pytest.fixture(scope="function")
 def valid_batch_definition():
```

### Comparing `opentaskpy-0.8.1/tests/test_config_loader.py` & `opentaskpy-0.9.0/tests/test_config_loader.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,19 @@
+# pylint: skip-file
 import json
 import os
 import random
 from datetime import datetime, timedelta
 
 import pytest
 from pytest_shell import fs
 
 from opentaskpy.config.loader import ConfigLoader
 
-GLOBAL_VARIABLES = None
+GLOBAL_VARIABLES: str | None = None
 
 RANDOM = random.randint(10000, 99999)
 
 
 @pytest.fixture(scope="function")
 def write_dummy_variables_file(tmpdir):
     # Write a nested variable to the global variables file
@@ -25,14 +26,29 @@
     fs.create_files(
         [
             {f"{tmpdir}/variables.json.j2": {"content": json.dumps(json_obj)}},
         ]
     )
 
 
+def test_load_variables(tmpdir):
+    # Ensure something satisfies the file lookup plugin
+    fs.create_files(
+        [
+            {
+                "/tmp/variable_lookup.txt": {
+                    "content": "hello",
+                }
+            },
+        ]
+    )
+
+    assert ConfigLoader("test/cfg") is not None
+
+
 def test_load_task_definition(write_dummy_variables_file, tmpdir):
     # Initialise the task runner
     config_loader = ConfigLoader(tmpdir)
     # Create a task definition file (this isn't valid, but it proves if the evaluation of variables works)
     fs.create_files([{f"{tmpdir}/task.json": {"content": '{"test": "{{ test }}"}'}}])
 
     expected_task_definition = {"test": "test123456"}
@@ -51,29 +67,55 @@
     config_loader = ConfigLoader(tmpdir)
 
     # Create a task definition file (this isn't valid, but it proves if the evaluation of variables works)
     fs.create_files(
         [
             {
                 f"{tmpdir}/task.json": {
-                    "content": '{"test_var": "{{ test }}", "variables": {"NEW_VARIABLE": "NEW_VALUE"}}'
+                    "content": (
+                        '{"test_var": "{{ test }}", "variables": {"NEW_VARIABLE":'
+                        ' "NEW_VALUE"}}'
+                    )
                 }
             }
         ]
     )
 
     expected_task_definition = {
         "test_var": "test123456",
         "variables": {"NEW_VARIABLE": "NEW_VALUE"},
     }
 
     # Test that the task definition is loaded correctly
     assert config_loader.load_task_definition("task") == expected_task_definition
 
 
+def test_custom_plugin(tmpdir):
+    # Create a JSON file with some test variables in it
+    fs.create_files(
+        [
+            {
+                f"{tmpdir}/variables.json.j2": {
+                    "content": '{"test": "{{ lookup(\'test_plugin\') }}"}'
+                }
+            },
+        ]
+    )
+    # Symlink test/cfg/plugins to tmpdir/plugins
+    os.symlink(
+        os.path.join(os.path.dirname(__file__), "../test/cfg", "plugins"),
+        f"{tmpdir}/plugins",
+    )
+
+    # Test that the global variables are loaded correctly
+    config_loader = ConfigLoader(tmpdir)
+
+    assert config_loader.get_global_variables() == {"test": "hello"}
+
+
 def test_load_global_variables(tmpdir):
     # Create a JSON file with some test variables in it
     fs.create_files(
         [
             {f"{tmpdir}/variables.json": {"content": '{"test": "test1234"}'}},
         ]
     )
@@ -185,15 +227,17 @@
         "test": "{{ SOME_VARIABLE }}7",
         "SOME_VARIABLE": "{{ SOME_VARIABLE2 }}6",
         "SOME_VARIABLE2": "{{ SOME_VARIABLE3 }}5",
         "SOME_VARIABLE3": "{{ SOME_VARIABLE4 }}4",
         "SOME_VARIABLE4": "{{ SOME_VARIABLE5 }}3",
         "SOME_VARIABLE5": "{{ SOME_VARIABLE6 }}2",
         "SOME_VARIABLE6": "{{ SOME_VARIABLE7 }}1",
-        "SOME_VARIABLE7": "{{ SOME_VARIABLE8 }}{{ SOME_VARIABLE2 }}{{ SOME_VARIABLE3 }}",
+        "SOME_VARIABLE7": (
+            "{{ SOME_VARIABLE8 }}{{ SOME_VARIABLE2 }}{{ SOME_VARIABLE3 }}"
+        ),
         "SOME_VARIABLE8": "test1234",
     }
 
     # Create a JSON file with some test variables in it
     fs.create_files(
         [
             {f"{tmpdir}/variables.json.j2": {"content": json.dumps(json_obj)}},
@@ -328,15 +372,18 @@
     config_loader = ConfigLoader(tmpdir)
 
     # Create a task definition file (this isn't valid, but it proves if the evaluation of variables works)
     fs.create_files(
         [
             {
                 f"{tmpdir}/task.json": {
-                    "content": '{"test_var": "{{ test }}", "variables": {"MY_VARIABLE": "value123"}}'
+                    "content": (
+                        '{"test_var": "{{ test }}", "variables": {"MY_VARIABLE":'
+                        ' "value123"}}'
+                    )
                 }
             }
         ]
     )
 
     expected_task_definition = {
         "test_var": "test123456",
@@ -387,17 +434,17 @@
             }
         ]
     )
 
     # Override things
     os.environ["OTF_OVERRIDE_TRANSFER_SOURCE_HOSTNAME"] = "non_existent_host"
     os.environ["OTF_OVERRIDE_TRANSFER_DESTINATION_0_HOSTNAME"] = "non_existent_host2"
-    os.environ[
-        "OTF_OVERRIDE_TRANSFER_DESTINATION_0_PROTOCOL_CREDENTIALS_USERNAME"
-    ] = "my_username"
+    os.environ["OTF_OVERRIDE_TRANSFER_DESTINATION_0_PROTOCOL_CREDENTIALS_USERNAME"] = (
+        "my_username"
+    )
 
     # Load the task definition
     config_loader = ConfigLoader(tmpdir)
     task_definition = config_loader.load_task_definition("test-task")
 
     del os.environ["OTF_OVERRIDE_TRANSFER_SOURCE_HOSTNAME"]
     del os.environ["OTF_OVERRIDE_TRANSFER_DESTINATION_0_HOSTNAME"]
```

### Comparing `opentaskpy-0.8.1/tests/test_docker_task_run.py` & `opentaskpy-0.9.0/tests/test_docker_task_run.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,18 @@
+# pylint: skip-file
+import logging
 import os
 import random
+import shutil
 import subprocess
 
 import pytest
-from fixtures.ssh_clients import *  # noqa:F401
+from pytest_shell import fs
+
+from tests.fixtures.ssh_clients import *  # noqa: F403
 
 IMAGE_PREFIX = "opentaskpy_unittest"
 MOVED_FILES_DIR = "archive"
 DELIMITER = ","
 
 """
 #################
@@ -35,100 +40,95 @@
     # Remove all images with the prefix
     result = subprocess.run(
         [
             "docker",
             "images",
             f"{IMAGE_PREFIX}_*",
         ],
-        stdout=subprocess.PIPE,
-        stderr=subprocess.PIPE,
+        capture_output=True,
     )
     if result.stdout:
         images = result.stdout.decode("utf-8").split("\n")
         # Split the repository name from the rest of the line
         image_ids = [image.split(" ")[0] for image in images if image]
         for image_id in image_ids:
             # If this image name matches the prefix, remove it
             if image_id.startswith(IMAGE_PREFIX):
-                print(f"Removing image: {image_id}")
+                logging.info(f"Removing image: {image_id}")
                 result = subprocess.run(
                     [
                         "docker",
                         "rmi",
                         image_id,
                     ],
-                    stdout=subprocess.PIPE,
-                    stderr=subprocess.PIPE,
+                    capture_output=True,
                 )
-                print(result.stdout.decode("utf-8"))
-                print(result.stderr.decode("utf-8"))
+                logging.info(result.stdout.decode("utf-8"))
+                logging.info(result.stderr.decode("utf-8"))
     else:
-        print("No images to remove")
+        logging.info("No images to remove")
 
 
 @pytest.fixture(scope="module")
 def docker_build_dev_image(tidy_images, image_name_dev, root_dir):
-    print("Building dev docker image")
-    print(root_dir)
+    logging.info("Building dev docker image")
+    logging.info(root_dir)
 
     # Trigger docker build
     command_args = [
         "docker",
         "build",
         "-t",
         image_name_dev,
         "-f",
         "Dockerfile.dev",
         f"{root_dir}/..",
     ]
     result = subprocess.run(
         command_args,
-        stdout=subprocess.PIPE,
-        stderr=subprocess.PIPE,
+        capture_output=True,
     )
     assert result.returncode == 0
 
 
 @pytest.fixture(scope="module")
 def docker_build_image(tidy_images, image_name, root_dir):
-    print("Building docker image")
-    print(root_dir)
+    logging.info("Building docker image")
+    logging.info(root_dir)
 
     # Trigger docker build
     command_args = [
         "docker",
         "build",
         "-t",
         image_name,
         "-f",
         "Dockerfile",
         f"{root_dir}/..",
     ]
     result = subprocess.run(
         command_args,
-        stdout=subprocess.PIPE,
-        stderr=subprocess.PIPE,
+        capture_output=True,
     )
     assert result.returncode == 0
 
 
 @pytest.fixture(scope="module")
 def test_network_id():
-    # Get the webdevops/ssh container thats running, and determine the network it's attached to
+    # Get the webdevops/ssh container that's running, and determine the network it's attached to
     result = subprocess.run(
         [
             "docker",
             "ps",
             "--filter",
             "name=^ssh_1",
             "--format",
             "{{.Networks}}",
         ],
-        stdout=subprocess.PIPE,
-        stderr=subprocess.PIPE,
+        capture_output=True,
     )
     assert result.returncode == 0
 
     # We need to extract the network name
     network = result.stdout.decode("utf-8").strip()
 
     # Get the network ID
@@ -137,16 +137,15 @@
             "docker",
             "network",
             "inspect",
             network,
             "--format",
             "{{.Id}}",
         ],
-        stdout=subprocess.PIPE,
-        stderr=subprocess.PIPE,
+        capture_output=True,
     )
     assert result.returncode == 0
     return result.stdout.decode("utf-8").strip()
 
 
 @pytest.fixture(scope="module")
 def log_dir(root_dir):
@@ -179,28 +178,32 @@
     test_network_id,
     image_name_dev,
     root_dir,
     env_vars,
     clear_logs,
     create_test_file,
 ):
+    # Create the testLogs directory
+    log_dir = f"{root_dir}/testLogs"
+    os.makedirs(log_dir, exist_ok=True)
+
     # Run the container
-    print("Running docker container")
+    logging.info("Running docker container")
     command_args = [
         "docker",
         "run",
         "--rm",
         "--user",
         f"{user_id}:{group_id}",
         "--network",
         test_network_id,
         "--volume",
         f"{root_dir}:/test",
         "--volume",
-        f"{root_dir}/testLogs:/logs",
+        f"{log_dir}:/logs",
         "--volume",
         "/tmp/variable_lookup.txt:/tmp/variable_lookup.txt",
         "-e",
         "OTF_SSH_KEY=/test/testFiles/id_rsa",
         image_name_dev,
         "task-run",
         "-t",
@@ -209,19 +212,18 @@
         "2",
         "-c",
         "/test/cfg",
     ]
 
     result = subprocess.run(
         command_args,
-        stdout=subprocess.PIPE,
-        stderr=subprocess.PIPE,
+        capture_output=True,
     )
-    print(result.stdout.decode("utf-8"))
-    print(result.stderr.decode("utf-8"))
+    logging.info(result.stdout.decode("utf-8"))
+    logging.info(result.stderr.decode("utf-8"))
 
     assert result.returncode == 0
 
 
 def test_standard_docker_image(
     setup_ssh_keys,
     docker_build_image,
@@ -237,15 +239,15 @@
     fs.create_files(
         [{f"{root_dir}/testFiles/ssh_1/src/text.txt": {"content": "test1234"}}]
     )
 
     # This image pulls down whatever is on pypi, so we're not really testing the code here. Just that we can call a simple transfer.
     # We want to check that the logging works correctly when running in a docker container and mapping volumes
     # Run the container
-    print("Running docker container")
+    logging.info("Running docker container")
     command_args = [
         "docker",
         "run",
         "--rm",
         "--user",
         f"{user_id}:{group_id}",
         "--network",
@@ -263,19 +265,18 @@
         "-t",
         "scp-basic",
         "-v",
         "2",
         "-c",
         "/test/cfg",
     ]
-    print(" ".join(command_args))
+    logging.info(" ".join(command_args))
 
     subprocess.run(
         command_args,
-        stdout=subprocess.PIPE,
-        stderr=subprocess.PIPE,
+        capture_output=True,
     )
     # We dont care whether this worked or not, we just want to check the logs
     # Check that the log file exists containing scp-basic in the name in log_dir
     log_files = os.listdir(f"{log_dir}/docker_log_test")
     assert len(log_files) == 1
     assert "scp-basic" in log_files[0]
```

### Comparing `opentaskpy-0.8.1/tests/test_email_transfer_schema_validate.py` & `opentaskpy-0.9.0/tests/test_email_transfer_schema_validate.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# pylint: skip-file
 import pytest
 
 from opentaskpy.config.schemas import validate_transfer_json
 
 
 @pytest.fixture(scope="function")
 def valid_protocol_definition():
```

### Comparing `opentaskpy-0.8.1/tests/test_file_helper.py` & `opentaskpy-0.9.0/tests/test_file_helper.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,24 @@
-from file_helper import list_test_files, write_test_file
+# pylint: skip-file
+from tests.file_helper import list_test_files, write_test_file
 
 
 def test_write_test_file_with_content(tmpdir):
     file_name = f"{tmpdir}/test.txt"
     content = "test1234"
     write_test_file(file_name, content)
-    with open(file_name, "r") as f:
+    with open(file_name) as f:
         assert f.read() == content
 
 
 def test_write_test_file_with_length(tmpdir):
     file_name = f"{tmpdir}/test.txt"
     length = 100
     write_test_file(file_name, length=length)
-    with open(file_name, "r") as f:
+    with open(file_name) as f:
         assert len(f.read()) == length
 
 
 def test_list_test_files(tmpdir):
     file_name = f"{tmpdir}/test.txt"
     content = "test1234"
     write_test_file(file_name, content)
```

### Comparing `opentaskpy-0.8.1/tests/test_logging.py` & `opentaskpy-0.9.0/tests/test_logging.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,100 +1,103 @@
+# pylint: skip-file
+import logging
 import os
 import re
 import time
 from datetime import datetime
 
-from fixtures.ssh_clients import *  # noqa:F401
+import opentaskpy.otflogging
+from tests.fixtures.ssh_clients import *  # noqa: F403
 
-import opentaskpy.logging
 
-
-def test_define_log_file_name(env_vars, tmpdir):
+def test_define_log_file_name(env_vars, tmpdir, top_level_root_dir):
     # Pass in different task types and validate that the log file name is correct
     timestamp = datetime.now().strftime("%Y%m%d-") + r"\d{6}\.\d{6}"
     log_path = "logs"
     expected_result_regex = rf"{log_path}/no_task_id/{timestamp}_B_running.log"
 
     assert re.search(
-        expected_result_regex, opentaskpy.logging._define_log_file_name(None, "B")
+        expected_result_regex, opentaskpy.otflogging._define_log_file_name(None, "B")
     )
 
     # Pass in a task ID and validate that the log file name is correct
     expected_result_regex = f"{log_path}/123/{timestamp}_B_running.log"
     assert re.search(
-        expected_result_regex, opentaskpy.logging._define_log_file_name("123", "B")
+        expected_result_regex, opentaskpy.otflogging._define_log_file_name("123", "B")
     )
 
     # Manually override the log directory and validate that the path changes
     os.environ["OTF_LOG_DIRECTORY"] = str(tmpdir)
     expected_result_regex = rf"{tmpdir}/no_task_id/{timestamp}_B_running.log"
     assert re.search(
-        expected_result_regex, opentaskpy.logging._define_log_file_name(None, "B")
+        expected_result_regex, opentaskpy.otflogging._define_log_file_name(None, "B")
     )
 
     # unset the environment variable
     del os.environ["OTF_LOG_DIRECTORY"]
 
     # Set a run prefix and check that log file names correlate
     os.environ["OTF_LOG_RUN_PREFIX"] = "test"
     expected_result = rf"{log_path}/no_task_id/test_B_running.log"
-    assert opentaskpy.logging._define_log_file_name(None, "B") == expected_result
+    assert opentaskpy.otflogging._define_log_file_name(None, "B") == expected_result
 
     # unset the environment variable if it's set
     if "OTF_LOG_RUN_PREFIX" in os.environ:
         del os.environ["OTF_LOG_RUN_PREFIX"]
 
     # Call the function to get the current name prefix, then call it again and validate the prefix is the same
-    log_filename = opentaskpy.logging._define_log_file_name(None, "B")
+    log_filename = opentaskpy.otflogging._define_log_file_name(None, "B")
     # Sleep 1 second to make sure the filename would have changed
     import time
 
     time.sleep(1)
-    assert log_filename == opentaskpy.logging._define_log_file_name(None, "B")
+    assert log_filename == opentaskpy.otflogging._define_log_file_name(None, "B")
 
     # Set an OTF_RUN_ID and validate that the directory name gets set to that
     os.environ["OTF_RUN_ID"] = "some-run-id"
     expected_result_regex = (
         rf"{log_path}/some-run-id/{timestamp}_B_some-task-id_running.log"
     )
     assert re.search(
         expected_result_regex,
-        opentaskpy.logging._define_log_file_name("some-task-id", "B"),
+        opentaskpy.otflogging._define_log_file_name("some-task-id", "B"),
     )
 
     # unset the environment variable if it's set
     if "OTF_RUN_ID" in os.environ:
         del os.environ["OTF_RUN_ID"]
 
     # Pass no task type, and expect None in it's place
-    expected_result_regex = rf"{log_path}/no_task_id/{timestamp}_None_running.log"
+    expected_result_regex = rf"{log_path}/no_task_id/{timestamp}_running.log"
     assert re.search(
-        expected_result_regex, opentaskpy.logging._define_log_file_name(None, None)
+        expected_result_regex, opentaskpy.otflogging._define_log_file_name(None, None)
     )
 
 
-def test_init_logging(env_vars):
+def test_init_logging(env_vars, top_level_root_dir):
     # Call init logging function and ensure that the returned logger includes a TaskFileHandler
     # pointing at the correct filename
     timestamp = datetime.now().strftime("%Y%m%d-") + r"\d{6}\.\d{6}"
-    log_path = "logs"
-    expected_result_regex = rf"{log_path}/some_task_id/{timestamp}_None_running.log"
-    logger = opentaskpy.logging.init_logging("some.class.name1", task_id="some_task_id")
+    log_path = f"{top_level_root_dir}/logs"
+    expected_result_regex = rf"{log_path}/some_task_id/{timestamp}_running.log"
+    logger = opentaskpy.otflogging.init_logging(
+        "some.class.name1", task_id="some_task_id"
+    )
 
     found_handler = False
     for log_handler in logger.handlers:
         if log_handler.__class__.__name__ == "TaskFileHandler":
             assert re.search(expected_result_regex, log_handler.baseFilename)
             found_handler = True
             break
 
     assert found_handler
 
     # Create a logger with a valid task type
-    logger = opentaskpy.logging.init_logging(
+    logger = opentaskpy.otflogging.init_logging(
         "some.class.name2", task_id="some_task_id", task_type="B"
     )
     expected_result_regex = rf"{log_path}/some_task_id/{timestamp}_B_running.log"
     # Find a handler of type TaskFileHandler in the logger
     found_handler = False
     for log_handler in logger.handlers:
         if log_handler.__class__.__name__ == "TaskFileHandler":
@@ -102,30 +105,30 @@
             found_handler = True
             break
 
     assert found_handler
 
     # Disable logging via env variable and ensure there's no handler defined
     os.environ["OTF_NO_LOG"] = "1"
-    logger = opentaskpy.logging.init_logging(
+    logger = opentaskpy.otflogging.init_logging(
         "some.class.name3", task_id="some_task_id", task_type="B"
     )
     assert len(logger.handlers) == 0
 
 
 def test_get_latest_log_file(env_vars):
     # Setup some dummy log files
     log_path = "test/testLogs"
     os.environ["OTF_LOG_DIRECTORY"] = log_path
 
     last_created_file = None
 
     # loop 1 to 10
     for _ in range(1, 11):
-        log_file_name = opentaskpy.logging._define_log_file_name(None, "B")
+        log_file_name = opentaskpy.otflogging._define_log_file_name(None, "B")
         # Ensure the directory exists, if not, create it
         if not os.path.exists(os.path.dirname(log_file_name)):
             os.makedirs(os.path.dirname(log_file_name))
 
         # Create the file
         with open(log_file_name, "w") as f:
             f.write("test")
@@ -133,71 +136,71 @@
         time.sleep(0.01)
         # Clear the prefix which will have been set in the environment
         del os.environ["OTF_LOG_RUN_PREFIX"]
         last_created_file = log_file_name
 
     # Run the function to see what it thinks the latest file is,
     # this should return none, because they are all in the _running state to being with
-    assert opentaskpy.logging.get_latest_log_file(None, "B") is None
+    assert opentaskpy.otflogging.get_latest_log_file(None, "B") is None
 
     # Rename the last created file to remove the _running suffix
     os.rename(last_created_file, last_created_file.replace("_running", ""))
     last_created_file = last_created_file.replace("_running", "")
     # Run the function again and validate that it still returns nothing
-    assert opentaskpy.logging.get_latest_log_file(None, "B") is None
+    assert opentaskpy.otflogging.get_latest_log_file(None, "B") is None
 
     # Rename this file to _failed
     os.rename(last_created_file, last_created_file.replace("_B", "_B_failed"))
     last_created_file = last_created_file.replace("_B", "_B_failed")
     # Run the function again and validate that it returns this file
-    assert opentaskpy.logging.get_latest_log_file(None, "B") == last_created_file
+    assert opentaskpy.otflogging.get_latest_log_file(None, "B") == last_created_file
 
-    # Create a new file that has succeeded, make sure it still returns None, as the lastest
+    # Create a new file that has succeeded, make sure it still returns None, as the latest
     # state is success
-    log_file_name = opentaskpy.logging._define_log_file_name(None, "B")
+    log_file_name = opentaskpy.otflogging._define_log_file_name(None, "B")
     # Write to the file
     with open(log_file_name, "w") as f:
         f.write("test")
     # Rename the file to remove the _running suffix
     os.rename(log_file_name, log_file_name.replace("_running", ""))
 
     # Run the function again and validate that it returns nothing, as last state is success
-    assert opentaskpy.logging.get_latest_log_file(None, "B") is None
+    assert opentaskpy.otflogging.get_latest_log_file(None, "B") is None
 
 
 def test_close_log_file(env_vars, tmpdir):
     os.environ["OTF_LOG_DIRECTORY"] = f"{tmpdir}/test/testLogs"
 
     # Create a logger and log something to it
-    logger = opentaskpy.logging.init_logging(
+    logger = opentaskpy.otflogging.init_logging(
         "some.class.name4", task_id="some_task_id", task_type="B"
     )
     logger.info("test")
 
     # Find a handler of type TaskFileHandler in the logger
     found_handler = None
     for log_handler in logger.handlers:
-        print(log_handler)
+        logging.info(log_handler)
         if log_handler.__class__.__name__ == "TaskFileHandler":
             found_handler = log_handler
             break
 
     assert found_handler is not None
 
     # Now the file should exist, we will close it with a success state and then check it's been renamed
-    opentaskpy.logging.close_log_file(logger, True)
+    opentaskpy.otflogging.close_log_file(logger, True)
 
     # Check the file has been renamed
     assert os.path.exists(found_handler.baseFilename.replace("_running", ""))
 
     # Now create a new logger and log something to it
-    logger = opentaskpy.logging.init_logging(
+    logger = opentaskpy.otflogging.init_logging(
         "some.class.name5", task_id="some_task_id", task_type="B"
     )
     logger.info("test")
 
     # Do the same, but make it fail
-    opentaskpy.logging.close_log_file(logger, False)
+    opentaskpy.otflogging.close_log_file(logger, False)
     # Check the file has been renamed
     assert os.path.exists(
         logger.handlers[0].baseFilename.replace("_running", "_failed")
     )
```

### Comparing `opentaskpy-0.8.1/tests/test_plugin_file.py` & `opentaskpy-0.9.0/tests/test_plugin_file.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# pylint: skip-file
 import pytest
 from pytest_shell import fs
 
 from opentaskpy.plugins.lookup.file import run
 
 
 def test_file_plugin_missing_path():
@@ -16,15 +17,16 @@
 
 def test_file_plugin_file_not_found(tmpdir):
     with pytest.raises(FileNotFoundError) as ex:
         run(path=f"{tmpdir}/does_not_exist.txt")
 
     assert (
         ex.value.args[0]
-        == f"File {tmpdir}/does_not_exist.txt does not exist while trying to run lookup plugin 'file'"
+        == f"File {tmpdir}/does_not_exist.txt does not exist while trying to run lookup"
+        " plugin 'file'"
     )
 
 
 def test_file_plugin(tmpdir):
     # Run test with a valid variable file, and ensure it's read and contains that value
     file_name = f"{tmpdir}/test.variable.txt"
     content = "test1234"
```

### Comparing `opentaskpy-0.8.1/tests/test_plugin_http_json.py` & `opentaskpy-0.9.0/tests/test_plugin_http_json.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# pylint: skip-file
 import pytest
 
 from opentaskpy.plugins.lookup.http_json import run
 
 
 def test_http_json_plugin_missing_all():
     with pytest.raises(Exception) as ex:
```

### Comparing `opentaskpy-0.8.1/tests/test_remote_transfer_script.py` & `opentaskpy-0.9.0/tests/test_remote_transfer_script.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,34 +1,35 @@
+# pylint: skip-file
 import grp
 import os
 import re
 import shutil
 import time
 
 import pytest
 from pytest_shell import fs
 
-from opentaskpy.remotehandlers.scripts import transfer as transfer
+from opentaskpy.remotehandlers.scripts import transfer
 
 FILE_PREFIX = "unittest_testfile"
 FILE_CONTENT = "test1234"
 MOVED_FILES_DIR = "test_move_files"
 DELIMITER = ","
 
-list = None
+list_: list[str]
 
 
 @pytest.fixture(scope="function")
 def setup(tmpdir):
     # Write 10 random files to /tmp
     for i in range(10):
         fs.create_files([{f"{tmpdir}/{FILE_PREFIX}_{i}": {"content": FILE_CONTENT}}])
 
-    global list
-    list = list_test_files(tmpdir, f"{FILE_PREFIX}_.*", delimiter=DELIMITER)
+    global list_
+    list_ = list_test_files(tmpdir, f"{FILE_PREFIX}_.*", delimiter=DELIMITER)
 
     # If directory doesn't exist, create it
     if not os.path.exists(f"{tmpdir}/{MOVED_FILES_DIR}"):
         os.mkdir(f"{tmpdir}/{MOVED_FILES_DIR}")
 
 
 def test_list_files_no_details(setup, tmpdir):
@@ -77,42 +78,42 @@
         # Check the modified time is within 1 second of now
         assert file["modified_time"] <= time.time()
         assert file["modified_time"] >= time.time() - 1
 
 
 def test_move_files_basic(setup, tmpdir):
     transfer.move_files(
-        list, ",", f"{tmpdir}/{MOVED_FILES_DIR}", False, None, None, None, None, None
+        list_, ",", f"{tmpdir}/{MOVED_FILES_DIR}", False, None, None, None, None, None
     )
 
     # Check that the files were moved
     for i in range(10):
         assert not os.path.exists(f"{tmpdir}/{FILE_PREFIX}_{i}")
 
         assert os.path.exists(f"{tmpdir}/{MOVED_FILES_DIR}/{FILE_PREFIX}_{i}")
 
 
 def test_move_files_create_dest_dir_1(setup, tmpdir):
     # Try moving to a directory that doesn't exist without asking to create one and expect an error
     with pytest.raises(FileNotFoundError):
         transfer.move_files(
-            list,
+            list_,
             DELIMITER,
             f"{tmpdir}/{MOVED_FILES_DIR}/non_existent_directory",
             False,
             None,
             None,
             None,
             None,
             None,
         )
 
     # Now move to a directory that doesn't exist and ask to create it
     transfer.move_files(
-        list,
+        list_,
         DELIMITER,
         f"{tmpdir}/{MOVED_FILES_DIR}/created_directory",
         True,
         None,
         None,
         None,
         None,
@@ -126,15 +127,15 @@
             f"{tmpdir}/{MOVED_FILES_DIR}/created_directory/{FILE_PREFIX}_{i}"
         )
 
 
 def test_move_files_create_dest_dir_2(setup, tmpdir):
     # Move the files in there again, now that the directory exists, this should still work
     transfer.move_files(
-        list,
+        list_,
         DELIMITER,
         f"{tmpdir}/created_directory",
         True,
         None,
         None,
         None,
         None,
@@ -147,15 +148,15 @@
 
     # Remove the created directory
     shutil.rmtree(f"{tmpdir}/created_directory")
 
 
 def test_move_files_rename(setup, tmpdir):
     transfer.move_files(
-        list,
+        list_,
         DELIMITER,
         f"{tmpdir}/{MOVED_FILES_DIR}",
         False,
         None,
         None,
         None,
         f"({FILE_PREFIX})_(.*)",
@@ -172,15 +173,15 @@
     # Determine if the current user is root or not
     is_root = os.getuid() == 0
 
     # Try setting the owner. This should fail because you cannot change the owner of a file unless you are root
     if not is_root:
         with pytest.raises(PermissionError):
             transfer.move_files(
-                list,
+                list_,
                 DELIMITER,
                 f"{tmpdir}/{MOVED_FILES_DIR}",
                 False,
                 "root",
                 None,
                 None,
                 None,
@@ -191,15 +192,15 @@
         for i in range(10):
             assert os.path.exists(f"{tmpdir}/{FILE_PREFIX}_{i}")
 
             assert not os.path.exists(f"{tmpdir}/{MOVED_FILES_DIR}/{FILE_PREFIX}_{i}")
 
     # Now try setting the owner to the current user - Doesn't really make sense, but should work without throwing an exception
     transfer.move_files(
-        list,
+        list_,
         DELIMITER,
         f"{tmpdir}/{MOVED_FILES_DIR}",
         False,
         os.environ.get("USER"),
         None,
         None,
         None,
@@ -216,15 +217,15 @@
 def test_move_files_set_group(setup, tmpdir):
     is_root = os.getuid() == 0
 
     # Try setting the group. This should fail because you cannot change the group of a file if you're not a member of it
     if not is_root:
         with pytest.raises(PermissionError):
             transfer.move_files(
-                list,
+                list_,
                 DELIMITER,
                 f"{tmpdir}/{MOVED_FILES_DIR}",
                 False,
                 None,
                 "root",
                 None,
                 None,
@@ -239,15 +240,15 @@
         # Now try setting the group to one of the secondary groups of the current user
         groups = os.getgrouplist(os.environ.get("USER"), os.getgid())
 
         # Convert group ID to name
         groups = [grp.getgrgid(group).gr_name for group in groups]
 
         transfer.move_files(
-            list,
+            list_,
             DELIMITER,
             f"{tmpdir}/{MOVED_FILES_DIR}",
             False,
             None,
             groups[0],
             None,
             None,
@@ -265,15 +266,15 @@
             # Convert group ID to name
             file_group = grp.getgrgid(file_group).gr_name
 
             assert groups[0] == file_group
 
 
 def test_delete_files(setup, tmpdir):
-    transfer.delete_files(list, DELIMITER)
+    transfer.delete_files(list_, DELIMITER)
 
     # Check that the files were moved
     for i in range(10):
         assert not os.path.exists(f"{tmpdir}/{FILE_PREFIX}_{i}")
 
 
 def list_test_files(directory, file_pattern, delimiter):
```

### Comparing `opentaskpy-0.8.1/tests/test_schema_validate.py` & `opentaskpy-0.9.0/tests/test_schema_validate.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# pylint: skip-file
 import pytest
 
 from opentaskpy.config.schemas import validate_transfer_json
 
 
 @pytest.fixture(scope="function")
 def valid_protocol_definition():
```

### Comparing `opentaskpy-0.8.1/tests/test_ssh_dest_schema_validate.py` & `opentaskpy-0.9.0/tests/test_ssh_dest_schema_validate.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# pylint: skip-file
 import pytest
 
 from opentaskpy.config.schemas import validate_transfer_json
 
 
 @pytest.fixture(scope="function")
 def valid_protocol_definition():
```

### Comparing `opentaskpy-0.8.1/tests/test_ssh_execution_schema_validate.py` & `opentaskpy-0.9.0/tests/test_ssh_execution_schema_validate.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# pylint: skip-file
 import pytest
 
 from opentaskpy.config.schemas import validate_execution_json
 
 
 @pytest.fixture(scope="function")
 def valid_protocol_definition():
```

### Comparing `opentaskpy-0.8.1/tests/test_ssh_source_schema_validate.py` & `opentaskpy-0.9.0/tests/test_ssh_source_schema_validate.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# pylint: skip-file
 import pytest
 
 from opentaskpy.config.schemas import validate_transfer_json
 
 
 @pytest.fixture(scope="function")
 def valid_protocol_definition():
```

### Comparing `opentaskpy-0.8.1/tests/test_task_run.py` & `opentaskpy-0.9.0/tests/test_task_run.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,21 @@
+# pylint: skip-file
 import datetime
+import logging
 import os
 import random
 import subprocess
 import threading
 import time
 
-from fixtures.ssh_clients import *  # noqa:F401
+import pytest
 from pytest_shell import fs
 
-from opentaskpy import exceptions, task_run
+from opentaskpy import exceptions, taskrun
+from tests.fixtures.ssh_clients import *  # noqa: F403
 
 # Create a variable with a random number
 RANDOM = random.randint(10000, 99999)
 FILE_PREFIX = "unittest_task_run"
 MOVED_FILES_DIR = "archive"
 DELIMITER = ","
 
@@ -77,70 +80,70 @@
 #################
 Tests using the Python code directly
 #################
 """
 
 
 def test_unknown_task_name(env_vars, setup_ssh_keys, root_dir):
-    task_runner = task_run.TaskRun("non-existent", "test/cfg")
+    task_runner = taskrun.TaskRun("non-existent", "test/cfg")
 
     # Verify an exception with appropriate text is thrown
     with pytest.raises(FileNotFoundError) as e:
         task_runner.run()
     assert e.value.args[0] == "Couldn't find task with name: non-existent"
 
 
 def test_batch_basic(env_vars, setup_ssh_keys, root_dir):
     # Create a test file
     fs.create_files(
         [{f"{root_dir}/testFiles/ssh_1/src/test.txt": {"content": "test1234"}}]
     )
 
     # Use the TaskRun class to trigger the job properly
-    task_runner = task_run.TaskRun("batch-basic", "test/cfg")
+    task_runner = taskrun.TaskRun("batch-basic", "test/cfg")
     assert task_runner.run()
 
 
 def test_execution_basic(env_vars, setup_ssh_keys, root_dir):
     # Use the TaskRun class to trigger the job properly
-    task_runner = task_run.TaskRun("df", "test/cfg")
+    task_runner = taskrun.TaskRun("df", "test/cfg")
     assert task_runner.run()
 
 
 def test_execution_fail(env_vars, setup_ssh_keys, root_dir):
     # Use the TaskRun class to trigger the job properly
-    task_runner = task_run.TaskRun("fail-command", "test/cfg")
+    task_runner = taskrun.TaskRun("fail-command", "test/cfg")
     assert not task_runner.run()
 
 
 def test_scp_basic(env_vars, setup_ssh_keys, root_dir):
     # Required files for this test:
     # ssh_1 : test/testFiles/ssh_1/src/.*\.txt
 
     # Create a test file
     fs.create_files(
         [{f"{root_dir}/testFiles/ssh_1/src/test.txt": {"content": "test1234"}}]
     )
 
     # Use the TaskRun class to trigger the job properly
-    task_runner = task_run.TaskRun("scp-basic", "test/cfg")
+    task_runner = taskrun.TaskRun("scp-basic", "test/cfg")
     assert task_runner.run()
 
 
 def test_scp_basic_multiple_dests(env_vars, setup_ssh_keys, root_dir):
     # Required files for this test:
     # ssh_1 : test/testFiles/ssh_1/src/.*\.txt
 
     # Create a test file
     fs.create_files(
         [{f"{root_dir}/testFiles/ssh_1/src/test.txt": {"content": "test1234"}}]
     )
 
     # Use the TaskRun class to trigger the job properly
-    task_runner = task_run.TaskRun("scp-basic-multiple-dests", "test/cfg")
+    task_runner = taskrun.TaskRun("scp-basic-multiple-dests", "test/cfg")
     assert task_runner.run()
 
     # Check the files were copied to all 3 destinations
     assert os.path.exists(f"{root_dir}/testFiles/ssh_2/dest/test.txt")
     assert os.path.exists(f"{root_dir}/testFiles/ssh_2/dest/test-2.txt")
     assert os.path.exists(f"{root_dir}/testFiles/ssh_2/dest/test-3.txt")
 
@@ -152,15 +155,15 @@
     # Create 10 test files
     for i in range(10):
         fs.create_files(
             [{f"{root_dir}/testFiles/ssh_1/src/test{i}.txt": {"content": "test1234"}}]
         )
 
     # Use the TaskRun class to trigger the job properly
-    task_runner = task_run.TaskRun("scp-basic", "test/cfg")
+    task_runner = taskrun.TaskRun("scp-basic", "test/cfg")
     assert task_runner.run()
 
     # Check that the files were all transferred
     for i in range(10):
         assert os.path.exists(f"{root_dir}/testFiles/ssh_2/dest/test{i}.txt")
 
 
@@ -169,29 +172,29 @@
     # ssh_1 : test/testFiles/ssh_1/src/.*\.txt
 
     # Create a test file
     fs.create_files(
         [{f"{root_dir}/testFiles/ssh_1/src/test.txt": {"content": "test1234"}}]
     )
 
-    task_runner = task_run.TaskRun("scp-basic-pull", "test/cfg")
+    task_runner = taskrun.TaskRun("scp-basic-pull", "test/cfg")
     assert task_runner.run()
 
 
 def test_scp_basic_pca_delete(env_vars, setup_ssh_keys, root_dir):
     # Required files for this test:
     # ssh_1 : test/testFiles/ssh_1/src/test1.txt
     # File will be delteted after transfer
 
     # Create a test file
     fs.create_files(
         [{f"{root_dir}/testFiles/ssh_1/src/test1.txt": {"content": "test1234"}}]
     )
 
-    task_runner = task_run.TaskRun("scp-basic-pca-delete", "test/cfg")
+    task_runner = taskrun.TaskRun("scp-basic-pca-delete", "test/cfg")
     assert task_runner.run()
 
     # Verify the file has disappeared
     assert not os.path.exists(f"{root_dir}/testFiles/ssh_1/src/test1.txt")
 
 
 def test_scp_basic_pca_move(env_vars, setup_ssh_keys, root_dir):
@@ -200,15 +203,15 @@
     # File will be moved after transfer
 
     # Create a test file
     fs.create_files(
         [{f"{root_dir}/testFiles/ssh_1/src/test2.txt": {"content": "test1234"}}]
     )
 
-    task_runner = task_run.TaskRun("scp-basic-pca-move", "test/cfg")
+    task_runner = taskrun.TaskRun("scp-basic-pca-move", "test/cfg")
     assert task_runner.run()
 
     # Verify the file has disappeared
     assert not os.path.exists(f"{root_dir}/testFiles/ssh_1/src/test2.txt")
 
     # Verify the file has been moved
     assert os.path.exists(f"{root_dir}/testFiles/ssh_1/archive/test2.txt")
@@ -223,64 +226,64 @@
     # Write a 11 byte long file
 
     write_test_file(
         f"{root_dir}/testFiles/ssh_1/src/log.unittset.log", content="01234567890"
     )
 
     # This should fail, because the file is too new
-    task_runner = task_run.TaskRun("scp-source-file-conditions", "test/cfg")
+    task_runner = taskrun.TaskRun("scp-source-file-conditions", "test/cfg")
     with pytest.raises(exceptions.FilesDoNotMeetConditionsError) as cm:
         task_runner.run()
     assert "No remote files could be found to transfer" in (cm.value.args[0])
 
     # Modify the file to be older than 1 minute and try again
     os.utime(
         f"{root_dir}/testFiles/ssh_1/src/log.unittset.log",
         (time.time() - 61, time.time() - 61),
     )
 
-    task_runner = task_run.TaskRun("scp-source-file-conditions", "test/cfg")
+    task_runner = taskrun.TaskRun("scp-source-file-conditions", "test/cfg")
     assert task_runner.run()
 
     # Modify the file to be older than 10 minutes and try again
     os.utime(
         f"{root_dir}/testFiles/ssh_1/src/log.unittset.log",
         (time.time() - 601, time.time() - 601),
     )
-    task_runner = task_run.TaskRun("scp-source-file-conditions", "test/cfg")
+    task_runner = taskrun.TaskRun("scp-source-file-conditions", "test/cfg")
     with pytest.raises(exceptions.FilesDoNotMeetConditionsError) as cm:
         task_runner.run()
     assert "No remote files could be found to transfer" in (cm.value.args[0])
 
     # Write a 9 byte long file - we need to change the age again
     write_test_file(
         f"{root_dir}/testFiles/ssh_1/src/log.unittset.log", content="012345678"
     )
 
     os.utime(
         f"{root_dir}/testFiles/ssh_1/src/log.unittset.log",
         (time.time() - 61, time.time() - 61),
     )
 
-    task_runner = task_run.TaskRun("scp-source-file-conditions", "test/cfg")
+    task_runner = taskrun.TaskRun("scp-source-file-conditions", "test/cfg")
     with pytest.raises(exceptions.FilesDoNotMeetConditionsError) as cm:
         task_runner.run()
     assert "No remote files could be found to transfer" in (cm.value.args[0])
 
     # Write a 21 byte long file - we need to change the age again
     write_test_file(
         f"{root_dir}/testFiles/ssh_1/src/log.unittset.log",
         content="012345678901234567890",
     )
     os.utime(
         f"{root_dir}/testFiles/ssh_1/src/log.unittset.log",
         (time.time() - 61, time.time() - 61),
     )
 
-    task_runner = task_run.TaskRun("scp-source-file-conditions", "test/cfg")
+    task_runner = taskrun.TaskRun("scp-source-file-conditions", "test/cfg")
     with pytest.raises(exceptions.FilesDoNotMeetConditionsError) as cm:
         task_runner.run()
     assert "No remote files could be found to transfer" in (cm.value.args[0])
 
 
 def test_scp_file_watch(env_vars, setup_ssh_keys, root_dir):
     # Required files for this test:
@@ -289,31 +292,31 @@
 
     # Create the source file
     fs.create_files(
         [{f"{root_dir}/testFiles/ssh_1/src/fileWatch.log": {"content": "01234567890"}}]
     )
 
     # Filewatch configured to wait 15 seconds before giving up. Expect it to fail
-    task_runner = task_run.TaskRun("scp-file-watch", "test/cfg")
+    task_runner = taskrun.TaskRun("scp-file-watch", "test/cfg")
     with pytest.raises(exceptions.RemoteFileNotFoundError) as cm:
         task_runner.run()
     assert "No files found after " in (cm.value.args[0])
 
     # This time, we run it again, but after 5 seconds, create the file
     # Create a thread that will run fs.create_fi:e{"s [{aft":r 5 second}}])
     t = threading.Timer(
         5,
         write_test_file,
         [f"{root_dir}/testFiles/ssh_1/src/fileWatch.txt"],
         {"content": "01234567890"},
     )
     t.start()
-    print("Started thread - Expect file in 5 seconds, starting task-run now...")
+    logging.info("Started thread - Expect file in 5 seconds, starting task-run now...")
 
-    task_runner = task_run.TaskRun("scp-file-watch", "test/cfg")
+    task_runner = taskrun.TaskRun("scp-file-watch", "test/cfg")
     assert task_runner.run()
 
     # Delete the fileWatch.txt and log file
     os.remove(f"{root_dir}/testFiles/ssh_1/src/fileWatch.txt")
     os.remove(f"{root_dir}/testFiles/ssh_1/src/fileWatch.log")
 
 
@@ -324,39 +327,39 @@
     # To succeed, the file should contain the text "someText"
     year = datetime.datetime.now().year
     # Ensure the log file is removed
     log_file = f"{root_dir}/testFiles/ssh_1/src/log{year}Watch.log"
     if os.path.exists(log_file):
         os.remove(log_file)
 
-    # Logwatch will fail if the log file dosent exist
-    task_runner = task_run.TaskRun("scp-log-watch", "test/cfg")
+    # Logwatch will fail if the log file doesn't exist
+    task_runner = taskrun.TaskRun("scp-log-watch", "test/cfg")
     with pytest.raises(exceptions.LogWatchInitError) as cm:
         task_runner.run()
     assert "Logwatch init failed" in (cm.value.args[0])
 
-    # This time, we run it again with the file created and populated. It should fail because the file dosent contain the expected text
+    # This time, we run it again with the file created and populated. It should fail because the file doesn't contain the expected text
     # Write the file
     fs.create_files([{log_file: {"content": "NOT_THE_RIGHT_PATTERN"}}])
 
-    task_runner = task_run.TaskRun("scp-log-watch", "test/cfg")
+    task_runner = taskrun.TaskRun("scp-log-watch", "test/cfg")
     with pytest.raises(exceptions.LogWatchTimeoutError) as cm:
         task_runner.run()
     assert "No log entry found after " in (cm.value.args[0])
 
     # This time we run again, but populate the file after 5 seconds
     t = threading.Timer(
         5,
         write_test_file,
         [log_file],
         {"content": "someText\n"},
     )
     t.start()
-    print("Started thread - Expect file in 5 seconds, starting task-run now...")
-    task_runner = task_run.TaskRun("scp-log-watch", "test/cfg")
+    logging.info("Started thread - Expect file in 5 seconds, starting task-run now...")
+    task_runner = taskrun.TaskRun("scp-log-watch", "test/cfg")
     assert task_runner.run()
 
 
 def test_scp_log_watch_tail(env_vars, setup_ssh_keys, root_dir):
     # Required files for this test:
     # ssh_1 : test/testFiles/ssh_1/src/logYYYYWatch.log
     # File should not exist to start with
@@ -374,29 +377,29 @@
             {
                 f"{root_dir}/testFiles/ssh_1/src/log{year}Watch1.log": {
                     "content": "someText\n"
                 }
             }
         ]
     )
-    task_runner = task_run.TaskRun("scp-log-watch-tail", "test/cfg")
+    task_runner = taskrun.TaskRun("scp-log-watch-tail", "test/cfg")
     with pytest.raises(exceptions.LogWatchTimeoutError) as cm:
         task_runner.run()
     assert "No log entry found after " in (cm.value.args[0])
 
     # This time write the contents after 5 seconds
     t = threading.Timer(
         5,
         write_test_file,
         [f"{root_dir}/testFiles/ssh_1/src/log{year}Watch1.log"],
         {"content": "someText\n", "mode": "a"},
     )
     t.start()
-    print("Started thread - Expect file in 5 seconds, starting task-run now...")
-    task_runner = task_run.TaskRun("scp-log-watch-tail", "test/cfg")
+    logging.info("Started thread - Expect file in 5 seconds, starting task-run now...")
+    task_runner = taskrun.TaskRun("scp-log-watch-tail", "test/cfg")
     assert task_runner.run()
 
 
 def run_task_run(task, verbose="2", config="test/cfg"):
     # We need to run the bin/task-run script to test this
     script = "python"
     args = [
@@ -406,32 +409,30 @@
         "-v",
         verbose,
         "-c",
         config,
     ]
 
     # Run the script
-    result = subprocess.run(
-        [script] + args, stdout=subprocess.PIPE, stderr=subprocess.PIPE
-    )
+    result = subprocess.run([script] + args, capture_output=True)
     # Write stdout and stderr to the console
-    print("\n########## STDOUT ##########")
-    print(result.stdout.decode("utf-8"))
+    logging.info("\n########## STDOUT ##########")
+    logging.info(result.stdout.decode("utf-8"))
     # Get the console colour for red
 
-    print("########## STDERR ##########")
-    print(f"{result.stderr.decode('utf-8')}")
+    logging.info("########## STDERR ##########")
+    logging.info(f"{result.stderr.decode('utf-8')}")
 
     return {
         "returncode": result.returncode,
         "stdout": result.stdout.decode("utf-8"),
         "stderr": result.stderr.decode("utf-8"),
     }
 
 
 def write_test_file(file_name, content=None, length=0, mode="w"):
     with open(file_name, mode) as f:
         if content is not None:
             f.write(content)
         else:
             f.write("a" * length)
-    print(f"Wrote file: {file_name}")
+    logging.info(f"Wrote file: {file_name}")
```

### Comparing `opentaskpy-0.8.1/tests/test_taskhandler_batch.py` & `opentaskpy-0.9.0/tests/test_taskhandler_batch.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,21 @@
+# pylint: skip-file
 import os
 import random
+import shutil
 
-from fixtures.ssh_clients import *  # noqa:F401
+import pytest
 from pytest_shell import fs
 
-import opentaskpy.logging
+import opentaskpy.otflogging
 from opentaskpy.config.loader import ConfigLoader
 
 # from opentaskpy.taskhandlers.batch import Batch
 from opentaskpy.taskhandlers import batch, execution, transfer
+from tests.fixtures.ssh_clients import *  # noqa: F403
 
 os.environ["OTF_NO_LOG"] = "1"
 os.environ["OTF_LOG_LEVEL"] = "DEBUG"
 
 
 # Create a task definition
 basic_batch_definition = {
@@ -230,16 +233,16 @@
 
     config_loader = ConfigLoader("test/cfg")
     batch_obj = batch.Batch(None, "timeout", timeout_batch_definition, config_loader)
     assert not batch_obj.run()
 
     # Validate that a log has been created with the correct status
     # Use the logging module to get the right log file name
-    log_file_name_batch = opentaskpy.logging._define_log_file_name("timeout", "B")
-    log_file_name_task = opentaskpy.logging._define_log_file_name("sleep-300", "E")
+    log_file_name_batch = opentaskpy.otflogging._define_log_file_name("timeout", "B")
+    log_file_name_task = opentaskpy.otflogging._define_log_file_name("sleep-300", "E")
 
     # Check that both exist, but renamed with _failed
     assert os.path.exists(log_file_name_batch.replace("_running", "_failed"))
     assert os.path.exists(log_file_name_task.replace("_running", "_failed"))
 
 
 def test_batch_parallel_single_success(setup_ssh_keys, env_vars, root_dir):
@@ -257,46 +260,48 @@
         config_loader,
     )
     # Run and expect a false status
     assert not batch_obj.run()
 
     # Validate that a log has been created with the correct status
     # Use the logging module to get the right log file name
-    log_file_name_batch = opentaskpy.logging._define_log_file_name(task_id, "B")
-    log_file_name_touch_task = opentaskpy.logging._define_log_file_name("touch", "E")
-    log_file_name_failed_task = opentaskpy.logging._define_log_file_name(
+    log_file_name_batch = opentaskpy.otflogging._define_log_file_name(task_id, "B")
+    log_file_name_touch_task = opentaskpy.otflogging._define_log_file_name("touch", "E")
+    log_file_name_failed_task = opentaskpy.otflogging._define_log_file_name(
         "fail-command", "E"
     )
 
     # Check that all exist, with the right status
     assert os.path.exists(log_file_name_batch.replace("_running", "_failed"))
     assert os.path.exists(log_file_name_touch_task.replace("_running", ""))
     assert os.path.exists(log_file_name_failed_task.replace("_running", "_failed"))
 
 
 def test_batch_resume_after_failure(setup_ssh_keys, env_vars, root_dir):
     task_id = f"parallel-single-failure-1-{RANDOM}"
     # Ensure there are no logs for this batch
-    shutil.rmtree(f"{opentaskpy.logging.LOG_DIRECTORY}/{task_id}", ignore_errors=True)
+    shutil.rmtree(
+        f"{opentaskpy.otflogging.LOG_DIRECTORY}/{task_id}", ignore_errors=True
+    )
 
     config_loader = ConfigLoader("test/cfg")
     batch_obj = batch.Batch(
         None,
         task_id,
         parallel_batch_with_single_failure_definition,
         config_loader,
     )
     # Run and expect a false status
     assert not batch_obj.run()
 
     # Validate that a log has been created with the correct status
     # Use the logging module to get the right log file name
-    log_file_name_batch = opentaskpy.logging._define_log_file_name(task_id, "B")
-    log_file_name_touch_task = opentaskpy.logging._define_log_file_name("touch", "E")
-    log_file_name_failed_task = opentaskpy.logging._define_log_file_name(
+    log_file_name_batch = opentaskpy.otflogging._define_log_file_name(task_id, "B")
+    log_file_name_touch_task = opentaskpy.otflogging._define_log_file_name("touch", "E")
+    log_file_name_failed_task = opentaskpy.otflogging._define_log_file_name(
         "fail-command", "E"
     )
 
     # Check that all exist, with the right status
     assert os.path.exists(log_file_name_batch.replace("_running", "_failed"))
     assert os.path.exists(log_file_name_touch_task.replace("_running", ""))
     assert os.path.exists(log_file_name_failed_task.replace("_running", "_failed"))
@@ -316,48 +321,50 @@
     assert batch_obj.task_order_tree[1]["status"] == "COMPLETED"
     assert batch_obj.task_order_tree[2]["status"] == "NOT_STARTED"
 
     # Run and expect a false status
     assert not batch_obj.run()
 
     # Validate that the touch task has been skipped, so there's no log file
-    log_file_name_batch = opentaskpy.logging._define_log_file_name(task_id, "B")
-    log_file_name_touch_task = opentaskpy.logging._define_log_file_name("touch", "E")
-    log_file_name_failed_task = opentaskpy.logging._define_log_file_name(
+    log_file_name_batch = opentaskpy.otflogging._define_log_file_name(task_id, "B")
+    log_file_name_touch_task = opentaskpy.otflogging._define_log_file_name("touch", "E")
+    log_file_name_failed_task = opentaskpy.otflogging._define_log_file_name(
         "fail-command", "E"
     )
 
     # Check that all exist, with the right status
     assert os.path.exists(log_file_name_batch.replace("_running", "_failed"))
     assert not os.path.exists(log_file_name_touch_task)
     assert os.path.exists(log_file_name_failed_task.replace("_running", "_failed"))
 
 
 def test_batch_resume_after_failure_retry_successful_tasks(
     setup_ssh_keys, env_vars, root_dir
 ):
     task_id = f"parallel-single-failure-2-{RANDOM}"
     # Ensure there are no logs for this batch
-    shutil.rmtree(f"{opentaskpy.logging.LOG_DIRECTORY}/{task_id}", ignore_errors=True)
+    shutil.rmtree(
+        f"{opentaskpy.otflogging.LOG_DIRECTORY}/{task_id}", ignore_errors=True
+    )
 
     config_loader = ConfigLoader("test/cfg")
     batch_obj = batch.Batch(
         None,
         task_id,
         parallel_batch_with_single_failure_with_retry_definition,
         config_loader,
     )
     # Run and expect a false status
     assert not batch_obj.run()
 
     # Validate that a log has been created with the correct status
     # Use the logging module to get the right log file name
-    log_file_name_batch = opentaskpy.logging._define_log_file_name(task_id, "B")
-    log_file_name_touch_task = opentaskpy.logging._define_log_file_name("touch", "E")
-    log_file_name_failed_task = opentaskpy.logging._define_log_file_name(
+    log_file_name_batch = opentaskpy.otflogging._define_log_file_name(task_id, "B")
+    log_file_name_touch_task = opentaskpy.otflogging._define_log_file_name("touch", "E")
+    log_file_name_failed_task = opentaskpy.otflogging._define_log_file_name(
         "fail-command", "E"
     )
 
     # Check that all exist, with the right status
     assert os.path.exists(log_file_name_batch.replace("_running", "_failed"))
     assert os.path.exists(log_file_name_touch_task.replace("_running", ""))
     assert os.path.exists(log_file_name_failed_task.replace("_running", "_failed"))
@@ -377,48 +384,52 @@
     assert batch_obj.task_order_tree[1]["status"], "NOT_STARTED"
     assert batch_obj.task_order_tree[2]["status"], "NOT_STARTED"
 
     # Run and expect a false status
     assert not batch_obj.run()
 
     # Validate that the touch task has been skipped, so there's no log file
-    log_file_name_batch = opentaskpy.logging._define_log_file_name(task_id, "B")
-    log_file_name_touch_task = opentaskpy.logging._define_log_file_name("touch", "E")
-    log_file_name_failed_task = opentaskpy.logging._define_log_file_name(
+    log_file_name_batch = opentaskpy.otflogging._define_log_file_name(task_id, "B")
+    log_file_name_touch_task = opentaskpy.otflogging._define_log_file_name("touch", "E")
+    log_file_name_failed_task = opentaskpy.otflogging._define_log_file_name(
         "fail-command", "E"
     )
 
     # Check that all exist, with the right status
     assert os.path.exists(log_file_name_batch.replace("_running", "_failed"))
     assert os.path.exists(log_file_name_touch_task.replace("_running", ""))
     assert os.path.exists(log_file_name_failed_task.replace("_running", "_failed"))
 
 
 def test_batch_continue_on_failure(setup_ssh_keys, env_vars, root_dir):
     task_id = f"dependency-continue-on-fail-1-{RANDOM}"
     # Ensure there are no logs for this batch
-    shutil.rmtree(f"{opentaskpy.logging.LOG_DIRECTORY}/{task_id}", ignore_errors=True)
+    shutil.rmtree(
+        f"{opentaskpy.otflogging.LOG_DIRECTORY}/{task_id}", ignore_errors=True
+    )
 
     config_loader = ConfigLoader("test/cfg")
     batch_obj = batch.Batch(
         None,
         task_id,
         dependent_batch_continue_on_fail_definition,
         config_loader,
     )
     # Run and expect a false status
     assert not batch_obj.run()
 
     # Validate that a log has been created with the correct status
     # Use the logging module to get the right log file name
-    log_file_name_batch = opentaskpy.logging._define_log_file_name(task_id, "B")
-    log_file_name_fail_task = opentaskpy.logging._define_log_file_name(
+    log_file_name_batch = opentaskpy.otflogging._define_log_file_name(task_id, "B")
+    log_file_name_fail_task = opentaskpy.otflogging._define_log_file_name(
         "fail-command", "E"
     )
-    log_file_name_scp_task = opentaskpy.logging._define_log_file_name("scp-basic", "T")
+    log_file_name_scp_task = opentaskpy.otflogging._define_log_file_name(
+        "scp-basic", "T"
+    )
 
     # Check that all exist, with the right status
     assert os.path.exists(log_file_name_batch.replace("_running", "_failed"))
 
     # The failed task that we continue on, should still have a failed log
     assert os.path.exists(log_file_name_fail_task.replace("_running", "_failed"))
```

### Comparing `opentaskpy-0.8.1/tests/test_taskhandler_execution.py` & `opentaskpy-0.9.0/tests/test_taskhandler_execution.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,16 @@
+# pylint: skip-file
 import os
 
-from fixtures.ssh_clients import *  # noqa:F401
+import pytest
 from pytest_shell import fs
 
 from opentaskpy import exceptions
 from opentaskpy.taskhandlers import execution
+from tests.fixtures.ssh_clients import *  # noqa: F403
 
 os.environ["OTF_NO_LOG"] = "1"
 os.environ["OTF_LOG_LEVEL"] = "DEBUG"
 
 # Create a task definition
 touch_task_definition = {
     "type": "execution",
```

### Comparing `opentaskpy-0.8.1/tests/test_taskhandler_transfer_email.py` & `opentaskpy-0.9.0/tests/test_taskhandler_transfer_email.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,16 @@
+# pylint: skip-file
 import json
 import os
 
-from fixtures.ssh_clients import *  # noqa:F401
 from pytest_shell import fs
 
 from opentaskpy.config.loader import ConfigLoader
 from opentaskpy.taskhandlers import transfer
+from tests.fixtures.ssh_clients import *  # noqa: F403
 
 os.environ["OTF_NO_LOG"] = "1"
 os.environ["OTF_LOG_LEVEL"] = "DEBUG"
 
 # Create a task definition
 email_task_definition = {
     "type": "transfer",
@@ -49,15 +50,15 @@
     # dest_remote_handler should be an array
     assert isinstance(transfer_obj.dest_remote_handlers, list)
     assert len(transfer_obj.dest_remote_handlers) == 1
     #  of SSHTransfer objects
     assert transfer_obj.dest_remote_handlers[0].__class__.__name__ == "EmailTransfer"
 
 
-def test_remote_handler_vars():
+def test_remote_handler_vars(env_vars):
     # Load the global config
     config_loader = ConfigLoader("test/cfg")
     global_variables = config_loader.get_global_variables()
     global_variables["global_protocol_vars"] = [
         {"name": "email", "smtp_port": 587, "smtp_server": "smtp.gmail.com"}
     ]
 
@@ -78,15 +79,15 @@
     # Check that the transfer object has an SMTP server config from the global config
     assert (
         transfer_obj.dest_remote_handlers[0].protocol_vars["smtp_server"]
         == "smtp.gmail.com"
     )
 
 
-def test_email_transfer(setup_ssh_keys, root_dir):
+def test_email_transfer(env_vars, setup_ssh_keys, root_dir):
     # Dont run this test if the env var GITHUB_ACTIONS is set
     if os.getenv("GITHUB_ACTIONS"):
         return
 
     # Create a file to transfer
     fs.create_files(
         [{f"{root_dir}/testFiles/ssh_1/src/emailhandler.txt": {"content": "test1234"}}]
@@ -115,8 +116,11 @@
 
     transfer_obj = transfer.Transfer(
         global_variables, "email-transfer", imported_task_def
     )
     transfer_obj._set_remote_handlers()
 
     # Run the transfer
-    transfer_obj.run()
+    assert transfer_obj.run()
+
+    # Check that files have been tidied up on the worker
+    assert not os.path.exists(transfer_obj.local_staging_dir)
```

### Comparing `opentaskpy-0.8.1/tests/test_taskhandler_transfer_ssh.py` & `opentaskpy-0.9.0/tests/test_taskhandler_transfer_ssh.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
+# pylint: skip-file
 import os
 
 import pytest
-from fixtures.ssh_clients import *  # noqa:F401
 from pytest_shell import fs
 
 from opentaskpy import exceptions
 from opentaskpy.taskhandlers import transfer
+from tests.fixtures.ssh_clients import *  # noqa: F403
 
 os.environ["OTF_NO_LOG"] = "1"
 os.environ["OTF_LOG_LEVEL"] = "DEBUG"
 
 # Create a task definition
 scp_task_definition = {
     "type": "transfer",
@@ -434,12 +435,16 @@
                 }
             }
         ]
     )
 
     # Create a transfer object
     transfer_obj = transfer.Transfer(None, "scp-basic", scp_proxy_task_definition)
+    local_staging_dir = transfer_obj.local_staging_dir
 
     # Run the transfer and expect a true status
     assert transfer_obj.run()
     # Check the destination file exists
     assert os.path.exists(f"{root_dir}/testFiles/ssh_2/dest/test.taskhandler.proxy.txt")
+
+    # Ensure that local files are tidied up
+    assert not os.path.exists(local_staging_dir)
```

