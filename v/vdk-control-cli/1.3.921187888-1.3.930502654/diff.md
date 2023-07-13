# Comparing `tmp/vdk-control-cli-1.3.921187888.tar.gz` & `tmp/vdk-control-cli-1.3.930502654.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/vdk-control-cli-1.3.921187888.tar", last modified: Wed Jul  5 07:13:35 2023, max compression
+gzip compressed data, was "dist/vdk-control-cli-1.3.930502654.tar", last modified: Thu Jul 13 18:10:07 2023, max compression
```

## Comparing `vdk-control-cli-1.3.921187888.tar` & `vdk-control-cli-1.3.930502654.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:13:35.000000 vdk-control-cli-1.3.921187888/
--rw-rw-rw-   0 root         (0) root         (0)      270 2023-07-05 07:13:17.000000 vdk-control-cli-1.3.921187888/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     5153 2023-07-05 07:13:35.000000 vdk-control-cli-1.3.921187888/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     4192 2023-07-05 07:13:17.000000 vdk-control-cli-1.3.921187888/README.md
--rw-rw-rw-   0 root         (0) root         (0)     1747 2023-07-05 07:13:35.000000 vdk-control-cli-1.3.921187888/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      460 2023-07-05 07:13:17.000000 vdk-control-cli-1.3.921187888/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:13:35.000000 vdk-control-cli-1.3.921187888/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:13:35.000000 vdk-control-cli-1.3.921187888/src/vdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:13:35.000000 vdk-control-cli-1.3.921187888/src/vdk/api/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:13:35.000000 vdk-control-cli-1.3.921187888/src/vdk/api/control/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:13:35.000000 vdk-control-cli-1.3.921187888/src/vdk/api/control/plugin/
--rw-rw-rw-   0 root         (0) root         (0)      717 2023-07-05 07:13:17.000000 vdk-control-cli-1.3.921187888/src/vdk/api/control/plugin/markers.py
--rw-rw-rw-   0 root         (0) root         (0)     1423 2023-07-05 07:13:17.000000 vdk-control-cli-1.3.921187888/src/vdk/api/control/plugin/specs.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:13:35.000000 vdk-control-cli-1.3.921187888/src/vdk/internal/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:13:35.000000 vdk-control-cli-1.3.921187888/src/vdk/internal/control/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:13:35.000000 vdk-control-cli-1.3.921187888/src/vdk/internal/control/command_groups/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:13:35.000000 vdk-control-cli-1.3.921187888/src/vdk/internal/control/command_groups/common_group/
--rw-rw-rw-   0 root         (0) root         (0)     2284 2023-07-05 07:13:17.000000 vdk-control-cli-1.3.921187888/src/vdk/internal/control/command_groups/common_group/default.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:13:35.000000 vdk-control-cli-1.3.921187888/src/vdk/internal/control/command_groups/info_group/
--rw-rw-rw-   0 root         (0) root         (0)     1868 2023-07-05 07:13:17.000000 vdk-control-cli-1.3.921187888/src/vdk/internal/control/command_groups/info_group/info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:13:35.000000 vdk-control-cli-1.3.921187888/src/vdk/internal/control/command_groups/job/
--rw-rw-rw-   0 root         (0) root         (0)    12776 2023-07-05 07:13:17.000000 vdk-control-cli-1.3.921187888/src/vdk/internal/control/command_groups/job/create.py
--rw-rw-rw-   0 root         (0) root         (0)     2121 2023-07-05 07:13:17.000000 vdk-control-cli-1.3.921187888/src/vdk/internal/control/command_groups/job/delete.py
--rw-rw-rw-   0 root         (0) root         (0)     7121 2023-07-05 07:13:17.000000 vdk-control-cli-1.3.921187888/src/vdk/internal/control/command_groups/job/deploy_cli.py
--rw-rw-rw-   0 root         (0) root         (0)    14343 2023-07-05 07:13:17.000000 vdk-control-cli-1.3.921187888/src/vdk/internal/control/command_groups/job/deploy_cli_impl.py
--rw-rw-rw-   0 root         (0) root         (0)     5129 2023-07-05 07:13:17.000000 vdk-control-cli-1.3.921187888/src/vdk/internal/control/command_groups/job/download_job.py
--rw-rw-rw-   0 root         (0) root         (0)     2678 2023-07-05 07:13:17.000000 vdk-control-cli-1.3.921187888/src/vdk/internal/control/command_groups/job/download_key.py
--rw-rw-rw-   0 root         (0) root         (0)    12207 2023-07-05 07:13:17.000000 vdk-control-cli-1.3.921187888/src/vdk/internal/control/command_groups/job/execute.py
--rw-rw-rw-   0 root         (0) root         (0)     8735 2023-07-05 07:13:17.000000 vdk-control-cli-1.3.921187888/src/vdk/internal/control/command_groups/job/list.py
--rw-rw-rw-   0 root         (0) root         (0)    12017 2023-07-05 07:13:17.000000 vdk-control-cli-1.3.921187888/src/vdk/internal/control/command_groups/job/properties.py
--rw-rw-rw-   0 root         (0) root         (0)    11433 2023-07-05 07:13:17.000000 vdk-control-cli-1.3.921187888/src/vdk/internal/control/command_groups/job/secrets.py
--rw-rw-rw-   0 root         (0) root         (0)     3403 2023-07-05 07:13:17.000000 vdk-control-cli-1.3.921187888/src/vdk/internal/control/command_groups/job/show.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:13:35.000000 vdk-control-cli-1.3.921187888/src/vdk/internal/control/command_groups/login_group/
--rw-rw-rw-   0 root         (0) root         (0)     6510 2023-07-05 07:13:17.000000 vdk-control-cli-1.3.921187888/src/vdk/internal/control/command_groups/login_group/login.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:13:35.000000 vdk-control-cli-1.3.921187888/src/vdk/internal/control/command_groups/logout_group/
--rw-rw-rw-   0 root         (0) root         (0)      410 2023-07-05 07:13:17.000000 vdk-control-cli-1.3.921187888/src/vdk/internal/control/command_groups/logout_group/logout.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:13:35.000000 vdk-control-cli-1.3.921187888/src/vdk/internal/control/command_groups/version_group/
--rw-rw-rw-   0 root         (0) root         (0)      772 2023-07-05 07:13:17.000000 vdk-control-cli-1.3.921187888/src/vdk/internal/control/command_groups/version_group/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:13:35.000000 vdk-control-cli-1.3.921187888/src/vdk/internal/control/configuration/
--rw-rw-rw-   0 root         (0) root         (0)      424 2023-07-05 07:13:17.000000 vdk-control-cli-1.3.921187888/src/vdk/internal/control/configuration/default_options.py
--rw-rw-rw-   0 root         (0) root         (0)     1221 2023-07-05 07:13:17.000000 vdk-control-cli-1.3.921187888/src/vdk/internal/control/configuration/defaults_config.py
--rw-rw-rw-   0 root         (0) root         (0)     2272 2023-07-05 07:13:17.000000 vdk-control-cli-1.3.921187888/src/vdk/internal/control/configuration/log_config.py
--rw-rw-rw-   0 root         (0) root         (0)     9551 2023-07-05 07:13:17.000000 vdk-control-cli-1.3.921187888/src/vdk/internal/control/configuration/vdk_config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:13:35.000000 vdk-control-cli-1.3.921187888/src/vdk/internal/control/exception/
--rw-rw-rw-   0 root         (0) root         (0)      649 2023-07-05 07:13:17.000000 vdk-control-cli-1.3.921187888/src/vdk/internal/control/exception/vdk_exception.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:13:35.000000 vdk-control-cli-1.3.921187888/src/vdk/internal/control/job/
--rw-rw-rw-   0 root         (0) root         (0)     1930 2023-07-05 07:13:17.000000 vdk-control-cli-1.3.921187888/src/vdk/internal/control/job/job_archive.py
--rw-rw-rw-   0 root         (0) root         (0)     4871 2023-07-05 07:13:17.000000 vdk-control-cli-1.3.921187888/src/vdk/internal/control/job/job_config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:13:35.000000 vdk-control-cli-1.3.921187888/src/vdk/internal/control/job/sample_job/
--rw-rw-rw-   0 root         (0) root         (0)      579 2023-07-05 07:13:17.000000 vdk-control-cli-1.3.921187888/src/vdk/internal/control/job/sample_job/10_sql_step.sql
--rw-rw-rw-   0 root         (0) root         (0)      816 2023-07-05 07:13:17.000000 vdk-control-cli-1.3.921187888/src/vdk/internal/control/job/sample_job/20_python_step.py
--rw-rw-rw-   0 root         (0) root         (0)     1446 2023-07-05 07:13:17.000000 vdk-control-cli-1.3.921187888/src/vdk/internal/control/job/sample_job/README.md
--rw-rw-rw-   0 root         (0) root         (0)     2902 2023-07-05 07:13:17.000000 vdk-control-cli-1.3.921187888/src/vdk/internal/control/job/sample_job/config.ini
--rw-rw-rw-   0 root         (0) root         (0)      243 2023-07-05 07:13:17.000000 vdk-control-cli-1.3.921187888/src/vdk/internal/control/job/sample_job/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)     3666 2023-07-05 07:13:17.000000 vdk-control-cli-1.3.921187888/src/vdk/internal/control/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:13:35.000000 vdk-control-cli-1.3.921187888/src/vdk/internal/control/plugin/
--rw-rw-rw-   0 root         (0) root         (0)     3715 2023-07-05 07:13:17.000000 vdk-control-cli-1.3.921187888/src/vdk/internal/control/plugin/control_plugin_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:13:35.000000 vdk-control-cli-1.3.921187888/src/vdk/internal/control/rest_lib/
--rw-rw-rw-   0 root         (0) root         (0)     3239 2023-07-05 07:13:17.000000 vdk-control-cli-1.3.921187888/src/vdk/internal/control/rest_lib/factory.py
--rw-rw-rw-   0 root         (0) root         (0)     3845 2023-07-05 07:13:17.000000 vdk-control-cli-1.3.921187888/src/vdk/internal/control/rest_lib/rest_client_errors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:13:35.000000 vdk-control-cli-1.3.921187888/src/vdk/internal/control/utils/
--rw-rw-rw-   0 root         (0) root         (0)     7297 2023-07-05 07:13:17.000000 vdk-control-cli-1.3.921187888/src/vdk/internal/control/utils/cli_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     1413 2023-07-05 07:13:17.000000 vdk-control-cli-1.3.921187888/src/vdk/internal/control/utils/control_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     3690 2023-07-05 07:13:17.000000 vdk-control-cli-1.3.921187888/src/vdk/internal/control/utils/output_printer.py
--rw-rw-rw-   0 root         (0) root         (0)      819 2023-07-05 07:13:17.000000 vdk-control-cli-1.3.921187888/src/vdk/internal/control/utils/version_utils.py
--rw-rw-rw-   0 root         (0) root         (0)      181 2023-07-05 07:13:22.000000 vdk-control-cli-1.3.921187888/src/vdk/internal/control/vdk_control_build_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:13:35.000000 vdk-control-cli-1.3.921187888/src/vdk_control_cli.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5153 2023-07-05 07:13:35.000000 vdk-control-cli-1.3.921187888/src/vdk_control_cli.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2426 2023-07-05 07:13:35.000000 vdk-control-cli-1.3.921187888/src/vdk_control_cli.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 07:13:35.000000 vdk-control-cli-1.3.921187888/src/vdk_control_cli.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       57 2023-07-05 07:13:35.000000 vdk-control-cli-1.3.921187888/src/vdk_control_cli.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 07:13:35.000000 vdk-control-cli-1.3.921187888/src/vdk_control_cli.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      185 2023-07-05 07:13:35.000000 vdk-control-cli-1.3.921187888/src/vdk_control_cli.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2023-07-05 07:13:35.000000 vdk-control-cli-1.3.921187888/src/vdk_control_cli.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       14 2023-07-05 07:13:22.000000 vdk-control-cli-1.3.921187888/version.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 18:10:07.000000 vdk-control-cli-1.3.930502654/
+-rw-rw-rw-   0 root         (0) root         (0)      270 2023-07-13 18:09:51.000000 vdk-control-cli-1.3.930502654/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     5153 2023-07-13 18:10:07.000000 vdk-control-cli-1.3.930502654/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     4192 2023-07-13 18:09:51.000000 vdk-control-cli-1.3.930502654/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     1747 2023-07-13 18:10:07.000000 vdk-control-cli-1.3.930502654/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      460 2023-07-13 18:09:51.000000 vdk-control-cli-1.3.930502654/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 18:10:07.000000 vdk-control-cli-1.3.930502654/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 18:10:07.000000 vdk-control-cli-1.3.930502654/src/vdk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 18:10:07.000000 vdk-control-cli-1.3.930502654/src/vdk/api/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 18:10:07.000000 vdk-control-cli-1.3.930502654/src/vdk/api/control/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 18:10:07.000000 vdk-control-cli-1.3.930502654/src/vdk/api/control/plugin/
+-rw-rw-rw-   0 root         (0) root         (0)      717 2023-07-13 18:09:51.000000 vdk-control-cli-1.3.930502654/src/vdk/api/control/plugin/markers.py
+-rw-rw-rw-   0 root         (0) root         (0)     1423 2023-07-13 18:09:51.000000 vdk-control-cli-1.3.930502654/src/vdk/api/control/plugin/specs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 18:10:07.000000 vdk-control-cli-1.3.930502654/src/vdk/internal/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 18:10:07.000000 vdk-control-cli-1.3.930502654/src/vdk/internal/control/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 18:10:07.000000 vdk-control-cli-1.3.930502654/src/vdk/internal/control/command_groups/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 18:10:07.000000 vdk-control-cli-1.3.930502654/src/vdk/internal/control/command_groups/common_group/
+-rw-rw-rw-   0 root         (0) root         (0)     2284 2023-07-13 18:09:51.000000 vdk-control-cli-1.3.930502654/src/vdk/internal/control/command_groups/common_group/default.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 18:10:07.000000 vdk-control-cli-1.3.930502654/src/vdk/internal/control/command_groups/info_group/
+-rw-rw-rw-   0 root         (0) root         (0)     1868 2023-07-13 18:09:51.000000 vdk-control-cli-1.3.930502654/src/vdk/internal/control/command_groups/info_group/info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 18:10:07.000000 vdk-control-cli-1.3.930502654/src/vdk/internal/control/command_groups/job/
+-rw-rw-rw-   0 root         (0) root         (0)    12776 2023-07-13 18:09:51.000000 vdk-control-cli-1.3.930502654/src/vdk/internal/control/command_groups/job/create.py
+-rw-rw-rw-   0 root         (0) root         (0)     2121 2023-07-13 18:09:51.000000 vdk-control-cli-1.3.930502654/src/vdk/internal/control/command_groups/job/delete.py
+-rw-rw-rw-   0 root         (0) root         (0)     7121 2023-07-13 18:09:51.000000 vdk-control-cli-1.3.930502654/src/vdk/internal/control/command_groups/job/deploy_cli.py
+-rw-rw-rw-   0 root         (0) root         (0)    14343 2023-07-13 18:09:51.000000 vdk-control-cli-1.3.930502654/src/vdk/internal/control/command_groups/job/deploy_cli_impl.py
+-rw-rw-rw-   0 root         (0) root         (0)     5129 2023-07-13 18:09:51.000000 vdk-control-cli-1.3.930502654/src/vdk/internal/control/command_groups/job/download_job.py
+-rw-rw-rw-   0 root         (0) root         (0)     2678 2023-07-13 18:09:51.000000 vdk-control-cli-1.3.930502654/src/vdk/internal/control/command_groups/job/download_key.py
+-rw-rw-rw-   0 root         (0) root         (0)    12207 2023-07-13 18:09:51.000000 vdk-control-cli-1.3.930502654/src/vdk/internal/control/command_groups/job/execute.py
+-rw-rw-rw-   0 root         (0) root         (0)     8735 2023-07-13 18:09:51.000000 vdk-control-cli-1.3.930502654/src/vdk/internal/control/command_groups/job/list.py
+-rw-rw-rw-   0 root         (0) root         (0)    11314 2023-07-13 18:09:51.000000 vdk-control-cli-1.3.930502654/src/vdk/internal/control/command_groups/job/properties.py
+-rw-rw-rw-   0 root         (0) root         (0)    11433 2023-07-13 18:09:51.000000 vdk-control-cli-1.3.930502654/src/vdk/internal/control/command_groups/job/secrets.py
+-rw-rw-rw-   0 root         (0) root         (0)     3403 2023-07-13 18:09:51.000000 vdk-control-cli-1.3.930502654/src/vdk/internal/control/command_groups/job/show.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 18:10:07.000000 vdk-control-cli-1.3.930502654/src/vdk/internal/control/command_groups/login_group/
+-rw-rw-rw-   0 root         (0) root         (0)     6510 2023-07-13 18:09:51.000000 vdk-control-cli-1.3.930502654/src/vdk/internal/control/command_groups/login_group/login.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 18:10:07.000000 vdk-control-cli-1.3.930502654/src/vdk/internal/control/command_groups/logout_group/
+-rw-rw-rw-   0 root         (0) root         (0)      410 2023-07-13 18:09:51.000000 vdk-control-cli-1.3.930502654/src/vdk/internal/control/command_groups/logout_group/logout.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 18:10:07.000000 vdk-control-cli-1.3.930502654/src/vdk/internal/control/command_groups/version_group/
+-rw-rw-rw-   0 root         (0) root         (0)      772 2023-07-13 18:09:51.000000 vdk-control-cli-1.3.930502654/src/vdk/internal/control/command_groups/version_group/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 18:10:07.000000 vdk-control-cli-1.3.930502654/src/vdk/internal/control/configuration/
+-rw-rw-rw-   0 root         (0) root         (0)      424 2023-07-13 18:09:51.000000 vdk-control-cli-1.3.930502654/src/vdk/internal/control/configuration/default_options.py
+-rw-rw-rw-   0 root         (0) root         (0)     1221 2023-07-13 18:09:51.000000 vdk-control-cli-1.3.930502654/src/vdk/internal/control/configuration/defaults_config.py
+-rw-rw-rw-   0 root         (0) root         (0)     2272 2023-07-13 18:09:51.000000 vdk-control-cli-1.3.930502654/src/vdk/internal/control/configuration/log_config.py
+-rw-rw-rw-   0 root         (0) root         (0)     9551 2023-07-13 18:09:51.000000 vdk-control-cli-1.3.930502654/src/vdk/internal/control/configuration/vdk_config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 18:10:07.000000 vdk-control-cli-1.3.930502654/src/vdk/internal/control/exception/
+-rw-rw-rw-   0 root         (0) root         (0)      649 2023-07-13 18:09:51.000000 vdk-control-cli-1.3.930502654/src/vdk/internal/control/exception/vdk_exception.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 18:10:07.000000 vdk-control-cli-1.3.930502654/src/vdk/internal/control/job/
+-rw-rw-rw-   0 root         (0) root         (0)     1930 2023-07-13 18:09:51.000000 vdk-control-cli-1.3.930502654/src/vdk/internal/control/job/job_archive.py
+-rw-rw-rw-   0 root         (0) root         (0)     4871 2023-07-13 18:09:51.000000 vdk-control-cli-1.3.930502654/src/vdk/internal/control/job/job_config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 18:10:07.000000 vdk-control-cli-1.3.930502654/src/vdk/internal/control/job/sample_job/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2023-07-13 18:09:51.000000 vdk-control-cli-1.3.930502654/src/vdk/internal/control/job/sample_job/10_sql_step.sql
+-rw-rw-rw-   0 root         (0) root         (0)      816 2023-07-13 18:09:51.000000 vdk-control-cli-1.3.930502654/src/vdk/internal/control/job/sample_job/20_python_step.py
+-rw-rw-rw-   0 root         (0) root         (0)     1446 2023-07-13 18:09:51.000000 vdk-control-cli-1.3.930502654/src/vdk/internal/control/job/sample_job/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     2902 2023-07-13 18:09:51.000000 vdk-control-cli-1.3.930502654/src/vdk/internal/control/job/sample_job/config.ini
+-rw-rw-rw-   0 root         (0) root         (0)      243 2023-07-13 18:09:51.000000 vdk-control-cli-1.3.930502654/src/vdk/internal/control/job/sample_job/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)     3666 2023-07-13 18:09:51.000000 vdk-control-cli-1.3.930502654/src/vdk/internal/control/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 18:10:07.000000 vdk-control-cli-1.3.930502654/src/vdk/internal/control/plugin/
+-rw-rw-rw-   0 root         (0) root         (0)     3715 2023-07-13 18:09:51.000000 vdk-control-cli-1.3.930502654/src/vdk/internal/control/plugin/control_plugin_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 18:10:07.000000 vdk-control-cli-1.3.930502654/src/vdk/internal/control/rest_lib/
+-rw-rw-rw-   0 root         (0) root         (0)     3239 2023-07-13 18:09:51.000000 vdk-control-cli-1.3.930502654/src/vdk/internal/control/rest_lib/factory.py
+-rw-rw-rw-   0 root         (0) root         (0)     3845 2023-07-13 18:09:51.000000 vdk-control-cli-1.3.930502654/src/vdk/internal/control/rest_lib/rest_client_errors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 18:10:07.000000 vdk-control-cli-1.3.930502654/src/vdk/internal/control/utils/
+-rw-rw-rw-   0 root         (0) root         (0)     7297 2023-07-13 18:09:51.000000 vdk-control-cli-1.3.930502654/src/vdk/internal/control/utils/cli_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     1413 2023-07-13 18:09:51.000000 vdk-control-cli-1.3.930502654/src/vdk/internal/control/utils/control_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     3690 2023-07-13 18:09:51.000000 vdk-control-cli-1.3.930502654/src/vdk/internal/control/utils/output_printer.py
+-rw-rw-rw-   0 root         (0) root         (0)      819 2023-07-13 18:09:51.000000 vdk-control-cli-1.3.930502654/src/vdk/internal/control/utils/version_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)      181 2023-07-13 18:09:55.000000 vdk-control-cli-1.3.930502654/src/vdk/internal/control/vdk_control_build_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 18:10:07.000000 vdk-control-cli-1.3.930502654/src/vdk_control_cli.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5153 2023-07-13 18:10:07.000000 vdk-control-cli-1.3.930502654/src/vdk_control_cli.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2426 2023-07-13 18:10:07.000000 vdk-control-cli-1.3.930502654/src/vdk_control_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-13 18:10:07.000000 vdk-control-cli-1.3.930502654/src/vdk_control_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       57 2023-07-13 18:10:07.000000 vdk-control-cli-1.3.930502654/src/vdk_control_cli.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-13 18:10:07.000000 vdk-control-cli-1.3.930502654/src/vdk_control_cli.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      185 2023-07-13 18:10:07.000000 vdk-control-cli-1.3.930502654/src/vdk_control_cli.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-07-13 18:10:07.000000 vdk-control-cli-1.3.930502654/src/vdk_control_cli.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       14 2023-07-13 18:09:55.000000 vdk-control-cli-1.3.930502654/version.txt
```

### Comparing `vdk-control-cli-1.3.921187888/PKG-INFO` & `vdk-control-cli-1.3.930502654/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vdk-control-cli
-Version: 1.3.921187888
+Version: 1.3.930502654
 Summary: VDK Control CLI allows user to create, delete, manage and their Data Jobs in Kubernetes runtime.
 Home-page: https://github.com/vmware/versatile-data-kit
 Author: VMware Inc.
 Author-email: aivanov@vmware.com
 Project-URL: Documentation, https://github.com/vmware/versatile-data-kit/wiki
 Project-URL: Source, https://github.com/vmware/versatile-data-kit/projects/vdk-control-cli
 Platform: any
```

### Comparing `vdk-control-cli-1.3.921187888/README.md` & `vdk-control-cli-1.3.930502654/README.md`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.921187888/setup.cfg` & `vdk-control-cli-1.3.930502654/setup.cfg`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.921187888/src/vdk/api/control/plugin/markers.py` & `vdk-control-cli-1.3.930502654/src/vdk/api/control/plugin/markers.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.921187888/src/vdk/api/control/plugin/specs.py` & `vdk-control-cli-1.3.930502654/src/vdk/api/control/plugin/specs.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.921187888/src/vdk/internal/control/command_groups/common_group/default.py` & `vdk-control-cli-1.3.930502654/src/vdk/internal/control/command_groups/common_group/default.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.921187888/src/vdk/internal/control/command_groups/info_group/info.py` & `vdk-control-cli-1.3.930502654/src/vdk/internal/control/command_groups/info_group/info.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.921187888/src/vdk/internal/control/command_groups/job/create.py` & `vdk-control-cli-1.3.930502654/src/vdk/internal/control/command_groups/job/create.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.921187888/src/vdk/internal/control/command_groups/job/delete.py` & `vdk-control-cli-1.3.930502654/src/vdk/internal/control/command_groups/job/delete.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.921187888/src/vdk/internal/control/command_groups/job/deploy_cli.py` & `vdk-control-cli-1.3.930502654/src/vdk/internal/control/command_groups/job/deploy_cli.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.921187888/src/vdk/internal/control/command_groups/job/deploy_cli_impl.py` & `vdk-control-cli-1.3.930502654/src/vdk/internal/control/command_groups/job/deploy_cli_impl.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.921187888/src/vdk/internal/control/command_groups/job/download_job.py` & `vdk-control-cli-1.3.930502654/src/vdk/internal/control/command_groups/job/download_job.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.921187888/src/vdk/internal/control/command_groups/job/download_key.py` & `vdk-control-cli-1.3.930502654/src/vdk/internal/control/command_groups/job/download_key.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.921187888/src/vdk/internal/control/command_groups/job/execute.py` & `vdk-control-cli-1.3.930502654/src/vdk/internal/control/command_groups/job/execute.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.921187888/src/vdk/internal/control/command_groups/job/list.py` & `vdk-control-cli-1.3.930502654/src/vdk/internal/control/command_groups/job/list.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.921187888/src/vdk/internal/control/command_groups/job/properties.py` & `vdk-control-cli-1.3.930502654/src/vdk/internal/control/command_groups/job/properties.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,15 +25,14 @@
 @unique
 class PropertyOperation(Enum):
     """
     An enum used to store the types of deploy operations
     """
 
     SET = "set"
-    SET_SECRET = "set_secret"  # nosec
     GET = "get"
 
 
 class JobProperties:
     def __init__(
         self,
         rest_api_url: str,
@@ -172,30 +171,26 @@
 
 @click.command(
     name="properties",
     help="Properties are key value pairs that can be set per data job. "
     """
          Job properties are most commonly used to:
 
-         * store credentials securely
          * store data job state
+         * store credentials (when a secrets backend has not been configured)
 
      Examples:
 
      \b
      # Set single property with key "my-key" and value "my-value".
      vdk properties --set my-key "my-value"
 
      \b
-     # Will prompt for the value so it's not printed on the screen.
-     vdk properties --set-secret "my-secret"
-
-     \b
      # Update multiple properties at once.
-     vdk properties --set "key1" "value1" --set "key2" "value2" --set-secret "secret1" --set-secret "secret2"
+     vdk properties --set "key1" "value1" --set "key2" "value2"
 
      \b
      # Use backslash \\ to set them on multiple lines
      vdk properties \\
         --set "key1" "value1" \\
         --set "key2" "value2"
 
@@ -232,21 +227,14 @@
     multiple=True,
     help="Set key value property. "
     "If property with same key exists we will override it but we will try to preserve the type."
     "Entirely new properties will be set with string type"
     "You can set multiple properties by using --set multiple times",
 )
 @click.option(
-    "--set-secret",
-    multiple=True,
-    type=click.STRING,
-    help="Set key value property which is a secret. It behaves almost the same way as --set."
-    "The difference from --set is that it will be prompted and input would be masked. ",
-)
-@click.option(
     "--delete",
     nargs=1,
     type=click.STRING,
     multiple=True,
     help="Delete property with a given key. "
     "You can delete multiple properties by using --delete multiple times",
 )
@@ -269,43 +257,42 @@
 @cli_utils.rest_api_url_option()
 @cli_utils.output_option()
 @cli_utils.check_required_parameters
 def properties_command(
     name: str,
     team: str,
     set: Tuple[str, str],
-    set_secret: Tuple[str, str],
     delete: Tuple[str],
     delete_all_job_properties: bool,
     overwrite_all_job_properties: _io.BufferedReader,
     get: str,
     list: bool,
     rest_api_url: str,
     output: OutputFormat,
 ):
-    if (set or set_secret or delete) and (get or list):
+    if (set or delete) and (get or list):
         raise VDKException(
             what="Invalid arguments",
-            why="Wrong input. Cannot pass --get or --list at the same time as --set or --set-secret.",
+            why="Wrong input. Cannot pass --get or --list at the same time as --set.",
             consequence="Command will abort with error.",
-            countermeasure="Fix passed arguments such that get/list are not passed in the same time as set/set-secret.",
+            countermeasure="Fix passed arguments such that get/list are not passed in the same time as set/.",
         )
     if get and list:
         raise VDKException(
             what="Invalid arguments",
             why="Wrong input. Cannot pass --get at the same time as --list. Choose one of the two.",
             consequence="Command will abort with error",
             countermeasure="Fix passed arguments such that only --list or only --get are used.",
         )
     log.debug(
         f"properties passed options: name: {name}, team: {team}, "
-        f"set: {set}, set_secret: {set_secret}, get: {get}, list: {list}, delete: {delete} "
+        f"set: {set}, get: {get}, list: {list}, delete: {delete} "
         f"rest_api_url: {rest_api_url}, output: {output}"
     )
-    key_value_pairs = _get_key_value_pairs(set, set_secret)
+    key_value_pairs = _get_key_value_pairs(set)
     cmd = JobProperties(rest_api_url, name, team, output)
     if key_value_pairs:
         cmd.update_properties(key_value_pairs)
     if delete:
         cmd.delete_keys(delete)
     if delete_all_job_properties:
         cmd.delete_all_job_properties()
@@ -323,17 +310,13 @@
                 "Expected valid json for properties overwrite.",
                 "JSON was not valid; error is " + str(e),
                 "Operation is aborted. Nothing has been changed.",
                 "Fix the file to be a valid json and re-try again.",
             )
 
 
-def _get_key_value_pairs(set, set_secret):
+def _get_key_value_pairs(set):
     key_value_pairs = {}
     if set:
         for key, value in set:
             key_value_pairs[key] = value
-    if set_secret:
-        for key in set_secret:
-            value = click.prompt(f"{key}", hide_input=True)
-            key_value_pairs[key] = value
     return key_value_pairs
```

### Comparing `vdk-control-cli-1.3.921187888/src/vdk/internal/control/command_groups/job/secrets.py` & `vdk-control-cli-1.3.930502654/src/vdk/internal/control/command_groups/job/secrets.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.921187888/src/vdk/internal/control/command_groups/job/show.py` & `vdk-control-cli-1.3.930502654/src/vdk/internal/control/command_groups/job/show.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.921187888/src/vdk/internal/control/command_groups/login_group/login.py` & `vdk-control-cli-1.3.930502654/src/vdk/internal/control/command_groups/login_group/login.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.921187888/src/vdk/internal/control/command_groups/version_group/version.py` & `vdk-control-cli-1.3.930502654/src/vdk/internal/control/command_groups/version_group/version.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.921187888/src/vdk/internal/control/configuration/defaults_config.py` & `vdk-control-cli-1.3.930502654/src/vdk/internal/control/configuration/defaults_config.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.921187888/src/vdk/internal/control/configuration/log_config.py` & `vdk-control-cli-1.3.930502654/src/vdk/internal/control/configuration/log_config.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.921187888/src/vdk/internal/control/configuration/vdk_config.py` & `vdk-control-cli-1.3.930502654/src/vdk/internal/control/configuration/vdk_config.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.921187888/src/vdk/internal/control/exception/vdk_exception.py` & `vdk-control-cli-1.3.930502654/src/vdk/internal/control/exception/vdk_exception.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.921187888/src/vdk/internal/control/job/job_archive.py` & `vdk-control-cli-1.3.930502654/src/vdk/internal/control/job/job_archive.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.921187888/src/vdk/internal/control/job/job_config.py` & `vdk-control-cli-1.3.930502654/src/vdk/internal/control/job/job_config.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.921187888/src/vdk/internal/control/job/sample_job/10_sql_step.sql` & `vdk-control-cli-1.3.930502654/src/vdk/internal/control/job/sample_job/10_sql_step.sql`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.921187888/src/vdk/internal/control/job/sample_job/20_python_step.py` & `vdk-control-cli-1.3.930502654/src/vdk/internal/control/job/sample_job/20_python_step.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.921187888/src/vdk/internal/control/job/sample_job/README.md` & `vdk-control-cli-1.3.930502654/src/vdk/internal/control/job/sample_job/README.md`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.921187888/src/vdk/internal/control/job/sample_job/config.ini` & `vdk-control-cli-1.3.930502654/src/vdk/internal/control/job/sample_job/config.ini`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.921187888/src/vdk/internal/control/main.py` & `vdk-control-cli-1.3.930502654/src/vdk/internal/control/main.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.921187888/src/vdk/internal/control/plugin/control_plugin_manager.py` & `vdk-control-cli-1.3.930502654/src/vdk/internal/control/plugin/control_plugin_manager.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.921187888/src/vdk/internal/control/rest_lib/factory.py` & `vdk-control-cli-1.3.930502654/src/vdk/internal/control/rest_lib/factory.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.921187888/src/vdk/internal/control/rest_lib/rest_client_errors.py` & `vdk-control-cli-1.3.930502654/src/vdk/internal/control/rest_lib/rest_client_errors.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.921187888/src/vdk/internal/control/utils/cli_utils.py` & `vdk-control-cli-1.3.930502654/src/vdk/internal/control/utils/cli_utils.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.921187888/src/vdk/internal/control/utils/control_utils.py` & `vdk-control-cli-1.3.930502654/src/vdk/internal/control/utils/control_utils.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.921187888/src/vdk/internal/control/utils/output_printer.py` & `vdk-control-cli-1.3.930502654/src/vdk/internal/control/utils/output_printer.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.921187888/src/vdk/internal/control/utils/version_utils.py` & `vdk-control-cli-1.3.930502654/src/vdk/internal/control/utils/version_utils.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.921187888/src/vdk_control_cli.egg-info/PKG-INFO` & `vdk-control-cli-1.3.930502654/src/vdk_control_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vdk-control-cli
-Version: 1.3.921187888
+Version: 1.3.930502654
 Summary: VDK Control CLI allows user to create, delete, manage and their Data Jobs in Kubernetes runtime.
 Home-page: https://github.com/vmware/versatile-data-kit
 Author: VMware Inc.
 Author-email: aivanov@vmware.com
 Project-URL: Documentation, https://github.com/vmware/versatile-data-kit/wiki
 Project-URL: Source, https://github.com/vmware/versatile-data-kit/projects/vdk-control-cli
 Platform: any
```

### Comparing `vdk-control-cli-1.3.921187888/src/vdk_control_cli.egg-info/SOURCES.txt` & `vdk-control-cli-1.3.930502654/src/vdk_control_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

