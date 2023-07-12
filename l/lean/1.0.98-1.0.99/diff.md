# Comparing `tmp/lean-1.0.98.tar.gz` & `tmp/lean-1.0.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/lean-1.0.98.tar", last modified: Tue Aug  9 23:47:05 2022, max compression
+gzip compressed data, was "dist/lean-1.0.99.tar", last modified: Fri Aug 12 22:04:54 2022, max compression
```

## Comparing `lean-1.0.98.tar` & `lean-1.0.99.tar`

### file list

```diff
@@ -1,141 +1,157 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 23:47:05.000000 lean-1.0.98/
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-09 23:47:05.000000 lean-1.0.98/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)    62194 2022-08-09 23:47:05.000000 lean-1.0.98/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 23:47:05.000000 lean-1.0.98/lean.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3769 2022-08-09 23:47:04.000000 lean-1.0.98/lean.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)    62194 2022-08-09 23:47:04.000000 lean-1.0.98/lean.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      275 2022-08-09 23:47:04.000000 lean-1.0.98/lean.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-09 23:47:04.000000 lean-1.0.98/lean.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       41 2022-08-09 23:47:04.000000 lean-1.0.98/lean.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        5 2022-08-09 23:47:04.000000 lean-1.0.98/lean.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 23:47:05.000000 lean-1.0.98/lean/
--rw-r--r--   0 runner    (1001) docker     (121)     5962 2022-08-09 23:46:58.000000 lean-1.0.98/lean/container.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 23:47:05.000000 lean-1.0.98/lean/commands/
--rw-r--r--   0 runner    (1001) docker     (121)     1748 2022-08-09 23:46:58.000000 lean-1.0.98/lean/commands/whoami.py
--rw-r--r--   0 runner    (1001) docker     (121)    10756 2022-08-09 23:46:58.000000 lean-1.0.98/lean/commands/create_project.py
--rw-r--r--   0 runner    (1001) docker     (121)      900 2022-08-09 23:46:58.000000 lean-1.0.98/lean/commands/logout.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 23:47:05.000000 lean-1.0.98/lean/commands/data/
--rw-r--r--   0 runner    (1001) docker     (121)    19544 2022-08-09 23:46:58.000000 lean-1.0.98/lean/commands/data/download.py
--rw-r--r--   0 runner    (1001) docker     (121)     1048 2022-08-09 23:46:58.000000 lean-1.0.98/lean/commands/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6286 2022-08-09 23:46:58.000000 lean-1.0.98/lean/commands/data/generate.py
--rw-r--r--   0 runner    (1001) docker     (121)    18399 2022-08-09 23:46:58.000000 lean-1.0.98/lean/commands/live.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 23:47:05.000000 lean-1.0.98/lean/commands/library/
--rw-r--r--   0 runner    (1001) docker     (121)     5061 2022-08-09 23:46:58.000000 lean-1.0.98/lean/commands/library/remove.py
--rw-r--r--   0 runner    (1001) docker     (121)     1042 2022-08-09 23:46:58.000000 lean-1.0.98/lean/commands/library/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    13480 2022-08-09 23:46:58.000000 lean-1.0.98/lean/commands/library/add.py
--rw-r--r--   0 runner    (1001) docker     (121)     5939 2022-08-09 23:46:58.000000 lean-1.0.98/lean/commands/init.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 23:47:05.000000 lean-1.0.98/lean/commands/cloud/
--rw-r--r--   0 runner    (1001) docker     (121)     2855 2022-08-09 23:46:58.000000 lean-1.0.98/lean/commands/cloud/status.py
--rw-r--r--   0 runner    (1001) docker     (121)    15216 2022-08-09 23:46:58.000000 lean-1.0.98/lean/commands/cloud/live.py
--rw-r--r--   0 runner    (1001) docker     (121)     2062 2022-08-09 23:46:58.000000 lean-1.0.98/lean/commands/cloud/pull.py
--rw-r--r--   0 runner    (1001) docker     (121)     1920 2022-08-09 23:46:58.000000 lean-1.0.98/lean/commands/cloud/push.py
--rw-r--r--   0 runner    (1001) docker     (121)    13982 2022-08-09 23:46:58.000000 lean-1.0.98/lean/commands/cloud/optimize.py
--rw-r--r--   0 runner    (1001) docker     (121)     1321 2022-08-09 23:46:58.000000 lean-1.0.98/lean/commands/cloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3172 2022-08-09 23:46:58.000000 lean-1.0.98/lean/commands/cloud/backtest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 23:47:05.000000 lean-1.0.98/lean/commands/config/
--rw-r--r--   0 runner    (1001) docker     (121)     1254 2022-08-09 23:46:58.000000 lean-1.0.98/lean/commands/config/set.py
--rw-r--r--   0 runner    (1001) docker     (121)     1156 2022-08-09 23:46:58.000000 lean-1.0.98/lean/commands/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1649 2022-08-09 23:46:58.000000 lean-1.0.98/lean/commands/config/list.py
--rw-r--r--   0 runner    (1001) docker     (121)     1161 2022-08-09 23:46:58.000000 lean-1.0.98/lean/commands/config/unset.py
--rw-r--r--   0 runner    (1001) docker     (121)     1766 2022-08-09 23:46:58.000000 lean-1.0.98/lean/commands/config/get.py
--rw-r--r--   0 runner    (1001) docker     (121)    12375 2022-08-09 23:46:58.000000 lean-1.0.98/lean/commands/optimize.py
--rw-r--r--   0 runner    (1001) docker     (121)     3618 2022-08-09 23:46:58.000000 lean-1.0.98/lean/commands/logs.py
--rw-r--r--   0 runner    (1001) docker     (121)     1997 2022-08-09 23:46:58.000000 lean-1.0.98/lean/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8573 2022-08-09 23:46:58.000000 lean-1.0.98/lean/commands/research.py
--rw-r--r--   0 runner    (1001) docker     (121)    11361 2022-08-09 23:46:58.000000 lean-1.0.98/lean/commands/report.py
--rw-r--r--   0 runner    (1001) docker     (121)     8380 2022-08-09 23:46:58.000000 lean-1.0.98/lean/commands/build.py
--rw-r--r--   0 runner    (1001) docker     (121)    14681 2022-08-09 23:46:58.000000 lean-1.0.98/lean/commands/backtest.py
--rw-r--r--   0 runner    (1001) docker     (121)     2364 2022-08-09 23:46:58.000000 lean-1.0.98/lean/commands/login.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 23:47:05.000000 lean-1.0.98/lean/models/
--rw-r--r--   0 runner    (1001) docker     (121)     3903 2022-08-09 23:46:58.000000 lean-1.0.98/lean/models/click_options.py
--rw-r--r--   0 runner    (1001) docker     (121)     5972 2022-08-09 23:46:58.000000 lean-1.0.98/lean/models/lean_config_configurer.py
--rw-r--r--   0 runner    (1001) docker     (121)     1277 2022-08-09 23:46:58.000000 lean-1.0.98/lean/models/pydantic.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 23:47:05.000000 lean-1.0.98/lean/models/data_providers/
--rw-r--r--   0 runner    (1001) docker     (121)     1278 2022-08-09 23:46:58.000000 lean-1.0.98/lean/models/data_providers/data_provider.py
--rw-r--r--   0 runner    (1001) docker     (121)     1137 2022-08-09 23:46:58.000000 lean-1.0.98/lean/models/data_providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      907 2022-08-09 23:46:58.000000 lean-1.0.98/lean/models/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 23:47:05.000000 lean-1.0.98/lean/models/brokerages/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 23:47:05.000000 lean-1.0.98/lean/models/brokerages/cloud/
--rw-r--r--   0 runner    (1001) docker     (121)     3529 2022-08-09 23:46:58.000000 lean-1.0.98/lean/models/brokerages/cloud/cloud_brokerage.py
--rw-r--r--   0 runner    (1001) docker     (121)     1139 2022-08-09 23:46:58.000000 lean-1.0.98/lean/models/brokerages/cloud/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 23:47:05.000000 lean-1.0.98/lean/models/brokerages/local/
--rw-r--r--   0 runner    (1001) docker     (121)     1780 2022-08-09 23:46:58.000000 lean-1.0.98/lean/models/brokerages/local/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1418 2022-08-09 23:46:58.000000 lean-1.0.98/lean/models/brokerages/local/local_brokerage.py
--rw-r--r--   0 runner    (1001) docker     (121)     1409 2022-08-09 23:46:58.000000 lean-1.0.98/lean/models/brokerages/local/data_feed.py
--rw-r--r--   0 runner    (1001) docker     (121)      664 2022-08-09 23:46:58.000000 lean-1.0.98/lean/models/brokerages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3936 2022-08-09 23:46:58.000000 lean-1.0.98/lean/models/options.py
--rw-r--r--   0 runner    (1001) docker     (121)    17999 2022-08-09 23:46:58.000000 lean-1.0.98/lean/models/configuration.py
--rw-r--r--   0 runner    (1001) docker     (121)     1491 2022-08-09 23:46:58.000000 lean-1.0.98/lean/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    14204 2022-08-09 23:46:58.000000 lean-1.0.98/lean/models/api.py
--rw-r--r--   0 runner    (1001) docker     (121)     1416 2022-08-09 23:46:58.000000 lean-1.0.98/lean/models/docker.py
--rw-r--r--   0 runner    (1001) docker     (121)     1513 2022-08-09 23:46:58.000000 lean-1.0.98/lean/models/modules.py
--rw-r--r--   0 runner    (1001) docker     (121)    17459 2022-08-09 23:46:58.000000 lean-1.0.98/lean/models/data.py
--rw-r--r--   0 runner    (1001) docker     (121)     1924 2022-08-09 23:46:58.000000 lean-1.0.98/lean/models/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (121)     2248 2022-08-09 23:46:58.000000 lean-1.0.98/lean/models/errors.py
--rw-r--r--   0 runner    (1001) docker     (121)     8876 2022-08-09 23:46:58.000000 lean-1.0.98/lean/models/json_module.py
--rw-r--r--   0 runner    (1001) docker     (121)     1622 2022-08-09 23:46:58.000000 lean-1.0.98/lean/models/market_hours_database.py
--rw-r--r--   0 runner    (1001) docker     (121)     1407 2022-08-09 23:46:58.000000 lean-1.0.98/lean/models/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     5856 2022-08-09 23:46:58.000000 lean-1.0.98/lean/main.py
--rw-r--r--   0 runner    (1001) docker     (121)      914 2022-08-09 23:47:03.000000 lean-1.0.98/lean/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 23:47:05.000000 lean-1.0.98/lean/ssh/
--rw-r--r--   0 runner    (1001) docker     (121)      411 2022-08-09 23:46:58.000000 lean-1.0.98/lean/ssh/key.pub
--rw-r--r--   0 runner    (1001) docker     (121)     1679 2022-08-09 23:46:58.000000 lean-1.0.98/lean/ssh/key
--rw-r--r--   0 runner    (1001) docker     (121)      274 2022-08-09 23:46:58.000000 lean-1.0.98/lean/ssh/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 23:47:05.000000 lean-1.0.98/lean/components/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 23:47:05.000000 lean-1.0.98/lean/components/api/
--rw-r--r--   0 runner    (1001) docker     (121)     1387 2022-08-09 23:46:58.000000 lean-1.0.98/lean/components/api/market_client.py
--rw-r--r--   0 runner    (1001) docker     (121)     1497 2022-08-09 23:46:58.000000 lean-1.0.98/lean/components/api/service_client.py
--rw-r--r--   0 runner    (1001) docker     (121)     4213 2022-08-09 23:46:58.000000 lean-1.0.98/lean/components/api/backtest_client.py
--rw-r--r--   0 runner    (1001) docker     (121)     7716 2022-08-09 23:46:58.000000 lean-1.0.98/lean/components/api/api_client.py
--rw-r--r--   0 runner    (1001) docker     (121)     3453 2022-08-09 23:46:58.000000 lean-1.0.98/lean/components/api/file_client.py
--rw-r--r--   0 runner    (1001) docker     (121)     2250 2022-08-09 23:46:58.000000 lean-1.0.98/lean/components/api/module_client.py
--rw-r--r--   0 runner    (1001) docker     (121)     5227 2022-08-09 23:46:58.000000 lean-1.0.98/lean/components/api/project_client.py
--rw-r--r--   0 runner    (1001) docker     (121)     1663 2022-08-09 23:46:58.000000 lean-1.0.98/lean/components/api/user_client.py
--rw-r--r--   0 runner    (1001) docker     (121)     1640 2022-08-09 23:46:58.000000 lean-1.0.98/lean/components/api/account_client.py
--rw-r--r--   0 runner    (1001) docker     (121)      664 2022-08-09 23:46:58.000000 lean-1.0.98/lean/components/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2023 2022-08-09 23:46:58.000000 lean-1.0.98/lean/components/api/organization_client.py
--rw-r--r--   0 runner    (1001) docker     (121)     3332 2022-08-09 23:46:58.000000 lean-1.0.98/lean/components/api/node_client.py
--rw-r--r--   0 runner    (1001) docker     (121)     4700 2022-08-09 23:46:58.000000 lean-1.0.98/lean/components/api/data_client.py
--rw-r--r--   0 runner    (1001) docker     (121)     8441 2022-08-09 23:46:58.000000 lean-1.0.98/lean/components/api/optimization_client.py
--rw-r--r--   0 runner    (1001) docker     (121)     2003 2022-08-09 23:46:58.000000 lean-1.0.98/lean/components/api/compile_client.py
--rw-r--r--   0 runner    (1001) docker     (121)     5043 2022-08-09 23:46:58.000000 lean-1.0.98/lean/components/api/live_client.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 23:47:05.000000 lean-1.0.98/lean/components/cloud/
--rw-r--r--   0 runner    (1001) docker     (121)     8981 2022-08-09 23:46:58.000000 lean-1.0.98/lean/components/cloud/pull_manager.py
--rw-r--r--   0 runner    (1001) docker     (121)     7803 2022-08-09 23:46:58.000000 lean-1.0.98/lean/components/cloud/cloud_runner.py
--rw-r--r--   0 runner    (1001) docker     (121)     4789 2022-08-09 23:46:58.000000 lean-1.0.98/lean/components/cloud/cloud_project_manager.py
--rw-r--r--   0 runner    (1001) docker     (121)     7506 2022-08-09 23:46:58.000000 lean-1.0.98/lean/components/cloud/push_manager.py
--rw-r--r--   0 runner    (1001) docker     (121)     7248 2022-08-09 23:46:58.000000 lean-1.0.98/lean/components/cloud/data_downloader.py
--rw-r--r--   0 runner    (1001) docker     (121)      664 2022-08-09 23:46:58.000000 lean-1.0.98/lean/components/cloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5600 2022-08-09 23:46:58.000000 lean-1.0.98/lean/components/cloud/module_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 23:47:05.000000 lean-1.0.98/lean/components/docker/
--rw-r--r--   0 runner    (1001) docker     (121)    35810 2022-08-09 23:46:58.000000 lean-1.0.98/lean/components/docker/lean_runner.py
--rw-r--r--   0 runner    (1001) docker     (121)      664 2022-08-09 23:46:58.000000 lean-1.0.98/lean/components/docker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    19743 2022-08-09 23:46:58.000000 lean-1.0.98/lean/components/docker/docker_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 23:47:05.000000 lean-1.0.98/lean/components/config/
--rw-r--r--   0 runner    (1001) docker     (121)     5050 2022-08-09 23:46:58.000000 lean-1.0.98/lean/components/config/cli_config_manager.py
--rw-r--r--   0 runner    (1001) docker     (121)    13245 2022-08-09 23:46:58.000000 lean-1.0.98/lean/components/config/lean_config_manager.py
--rw-r--r--   0 runner    (1001) docker     (121)     3108 2022-08-09 23:46:58.000000 lean-1.0.98/lean/components/config/storage.py
--rw-r--r--   0 runner    (1001) docker     (121)     6255 2022-08-09 23:46:58.000000 lean-1.0.98/lean/components/config/output_config_manager.py
--rw-r--r--   0 runner    (1001) docker     (121)    10763 2022-08-09 23:46:58.000000 lean-1.0.98/lean/components/config/optimizer_config_manager.py
--rw-r--r--   0 runner    (1001) docker     (121)      664 2022-08-09 23:46:58.000000 lean-1.0.98/lean/components/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3402 2022-08-09 23:46:58.000000 lean-1.0.98/lean/components/config/project_config_manager.py
--rw-r--r--   0 runner    (1001) docker     (121)      664 2022-08-09 23:46:58.000000 lean-1.0.98/lean/components/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 23:47:05.000000 lean-1.0.98/lean/components/util/
--rw-r--r--   0 runner    (1001) docker     (121)     4455 2022-08-09 23:46:58.000000 lean-1.0.98/lean/components/util/http_client.py
--rw-r--r--   0 runner    (1001) docker     (121)     3188 2022-08-09 23:46:58.000000 lean-1.0.98/lean/components/util/path_manager.py
--rw-r--r--   0 runner    (1001) docker     (121)     5676 2022-08-09 23:46:58.000000 lean-1.0.98/lean/components/util/logger.py
--rw-r--r--   0 runner    (1001) docker     (121)     6518 2022-08-09 23:46:58.000000 lean-1.0.98/lean/components/util/compiler.py
--rw-r--r--   0 runner    (1001) docker     (121)     4474 2022-08-09 23:46:58.000000 lean-1.0.98/lean/components/util/platform_manager.py
--rw-r--r--   0 runner    (1001) docker     (121)     4440 2022-08-09 23:46:58.000000 lean-1.0.98/lean/components/util/task_manager.py
--rw-r--r--   0 runner    (1001) docker     (121)      664 2022-08-09 23:46:58.000000 lean-1.0.98/lean/components/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    22077 2022-08-09 23:46:58.000000 lean-1.0.98/lean/components/util/project_manager.py
--rw-r--r--   0 runner    (1001) docker     (121)     1641 2022-08-09 23:46:58.000000 lean-1.0.98/lean/components/util/xml_manager.py
--rw-r--r--   0 runner    (1001) docker     (121)     7677 2022-08-09 23:46:58.000000 lean-1.0.98/lean/components/util/update_manager.py
--rw-r--r--   0 runner    (1001) docker     (121)     1647 2022-08-09 23:46:58.000000 lean-1.0.98/lean/components/util/temp_manager.py
--rw-r--r--   0 runner    (1001) docker     (121)     1335 2022-08-09 23:46:58.000000 lean-1.0.98/lean/components/util/name_extraction.py
--rw-r--r--   0 runner    (1001) docker     (121)     3156 2022-08-09 23:46:58.000000 lean-1.0.98/lean/components/util/name_generator.py
--rw-r--r--   0 runner    (1001) docker     (121)     3174 2022-08-09 23:46:58.000000 lean-1.0.98/lean/components/util/market_hours_database.py
--rw-r--r--   0 runner    (1001) docker     (121)    11687 2022-08-09 23:46:58.000000 lean-1.0.98/lean/click.py
--rw-r--r--   0 runner    (1001) docker     (121)     3939 2022-08-09 23:46:58.000000 lean-1.0.98/lean/constants.py
--rw-r--r--   0 runner    (1001) docker     (121)     3291 2022-08-09 23:46:58.000000 lean-1.0.98/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)    51489 2022-08-09 23:46:58.000000 lean-1.0.98/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-12 22:04:54.000000 lean-1.0.99/
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-12 22:04:54.000000 lean-1.0.99/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)    72240 2022-08-12 22:04:54.000000 lean-1.0.99/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-12 22:04:54.000000 lean-1.0.99/lean.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     4281 2022-08-12 22:04:54.000000 lean-1.0.99/lean.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    72240 2022-08-12 22:04:54.000000 lean-1.0.99/lean.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      275 2022-08-12 22:04:54.000000 lean-1.0.99/lean.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-12 22:04:54.000000 lean-1.0.99/lean.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       41 2022-08-12 22:04:54.000000 lean-1.0.99/lean.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        5 2022-08-12 22:04:54.000000 lean-1.0.99/lean.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-12 22:04:54.000000 lean-1.0.99/lean/
+-rw-r--r--   0 runner    (1001) docker     (121)     5962 2022-08-12 22:04:48.000000 lean-1.0.99/lean/container.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-12 22:04:54.000000 lean-1.0.99/lean/commands/
+-rw-r--r--   0 runner    (1001) docker     (121)     1748 2022-08-12 22:04:48.000000 lean-1.0.99/lean/commands/whoami.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10756 2022-08-12 22:04:48.000000 lean-1.0.99/lean/commands/create_project.py
+-rw-r--r--   0 runner    (1001) docker     (121)      900 2022-08-12 22:04:48.000000 lean-1.0.99/lean/commands/logout.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-12 22:04:54.000000 lean-1.0.99/lean/commands/data/
+-rw-r--r--   0 runner    (1001) docker     (121)    19544 2022-08-12 22:04:48.000000 lean-1.0.99/lean/commands/data/download.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1048 2022-08-12 22:04:48.000000 lean-1.0.99/lean/commands/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6286 2022-08-12 22:04:48.000000 lean-1.0.99/lean/commands/data/generate.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-12 22:04:54.000000 lean-1.0.99/lean/commands/live/
+-rw-r--r--   0 runner    (1001) docker     (121)     2833 2022-08-12 22:04:48.000000 lean-1.0.99/lean/commands/live/submit_order.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1910 2022-08-12 22:04:48.000000 lean-1.0.99/lean/commands/live/liquidate.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18478 2022-08-12 22:04:48.000000 lean-1.0.99/lean/commands/live/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3927 2022-08-12 22:04:48.000000 lean-1.0.99/lean/commands/live/live.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3079 2022-08-12 22:04:48.000000 lean-1.0.99/lean/commands/live/add_security.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1580 2022-08-12 22:04:48.000000 lean-1.0.99/lean/commands/live/cancel_order.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2332 2022-08-12 22:04:48.000000 lean-1.0.99/lean/commands/live/update_order.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1271 2022-08-12 22:04:48.000000 lean-1.0.99/lean/commands/live/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1408 2022-08-12 22:04:48.000000 lean-1.0.99/lean/commands/live/stop.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-12 22:04:54.000000 lean-1.0.99/lean/commands/library/
+-rw-r--r--   0 runner    (1001) docker     (121)     5061 2022-08-12 22:04:48.000000 lean-1.0.99/lean/commands/library/remove.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1042 2022-08-12 22:04:48.000000 lean-1.0.99/lean/commands/library/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13480 2022-08-12 22:04:48.000000 lean-1.0.99/lean/commands/library/add.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5939 2022-08-12 22:04:48.000000 lean-1.0.99/lean/commands/init.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-12 22:04:54.000000 lean-1.0.99/lean/commands/cloud/
+-rw-r--r--   0 runner    (1001) docker     (121)     2855 2022-08-12 22:04:48.000000 lean-1.0.99/lean/commands/cloud/status.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2062 2022-08-12 22:04:48.000000 lean-1.0.99/lean/commands/cloud/pull.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-12 22:04:54.000000 lean-1.0.99/lean/commands/cloud/live/
+-rw-r--r--   0 runner    (1001) docker     (121)     1511 2022-08-12 22:04:48.000000 lean-1.0.99/lean/commands/cloud/live/liquidate.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15301 2022-08-12 22:04:48.000000 lean-1.0.99/lean/commands/cloud/live/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1011 2022-08-12 22:04:48.000000 lean-1.0.99/lean/commands/cloud/live/live.py
+-rw-r--r--   0 runner    (1001) docker     (121)      944 2022-08-12 22:04:48.000000 lean-1.0.99/lean/commands/cloud/live/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1486 2022-08-12 22:04:48.000000 lean-1.0.99/lean/commands/cloud/live/stop.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1920 2022-08-12 22:04:48.000000 lean-1.0.99/lean/commands/cloud/push.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13982 2022-08-12 22:04:48.000000 lean-1.0.99/lean/commands/cloud/optimize.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1326 2022-08-12 22:04:48.000000 lean-1.0.99/lean/commands/cloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3172 2022-08-12 22:04:48.000000 lean-1.0.99/lean/commands/cloud/backtest.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-12 22:04:54.000000 lean-1.0.99/lean/commands/config/
+-rw-r--r--   0 runner    (1001) docker     (121)     1254 2022-08-12 22:04:48.000000 lean-1.0.99/lean/commands/config/set.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1156 2022-08-12 22:04:48.000000 lean-1.0.99/lean/commands/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1649 2022-08-12 22:04:48.000000 lean-1.0.99/lean/commands/config/list.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1161 2022-08-12 22:04:48.000000 lean-1.0.99/lean/commands/config/unset.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1766 2022-08-12 22:04:48.000000 lean-1.0.99/lean/commands/config/get.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12375 2022-08-12 22:04:48.000000 lean-1.0.99/lean/commands/optimize.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3618 2022-08-12 22:04:48.000000 lean-1.0.99/lean/commands/logs.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2001 2022-08-12 22:04:48.000000 lean-1.0.99/lean/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8573 2022-08-12 22:04:48.000000 lean-1.0.99/lean/commands/research.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11361 2022-08-12 22:04:48.000000 lean-1.0.99/lean/commands/report.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8380 2022-08-12 22:04:48.000000 lean-1.0.99/lean/commands/build.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14681 2022-08-12 22:04:48.000000 lean-1.0.99/lean/commands/backtest.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2364 2022-08-12 22:04:48.000000 lean-1.0.99/lean/commands/login.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-12 22:04:54.000000 lean-1.0.99/lean/models/
+-rw-r--r--   0 runner    (1001) docker     (121)     4381 2022-08-12 22:04:48.000000 lean-1.0.99/lean/models/click_options.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5972 2022-08-12 22:04:48.000000 lean-1.0.99/lean/models/lean_config_configurer.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1277 2022-08-12 22:04:48.000000 lean-1.0.99/lean/models/pydantic.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-12 22:04:54.000000 lean-1.0.99/lean/models/data_providers/
+-rw-r--r--   0 runner    (1001) docker     (121)     1278 2022-08-12 22:04:48.000000 lean-1.0.99/lean/models/data_providers/data_provider.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1137 2022-08-12 22:04:48.000000 lean-1.0.99/lean/models/data_providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      907 2022-08-12 22:04:48.000000 lean-1.0.99/lean/models/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-12 22:04:54.000000 lean-1.0.99/lean/models/brokerages/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-12 22:04:54.000000 lean-1.0.99/lean/models/brokerages/cloud/
+-rw-r--r--   0 runner    (1001) docker     (121)     3529 2022-08-12 22:04:48.000000 lean-1.0.99/lean/models/brokerages/cloud/cloud_brokerage.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1139 2022-08-12 22:04:48.000000 lean-1.0.99/lean/models/brokerages/cloud/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-12 22:04:54.000000 lean-1.0.99/lean/models/brokerages/local/
+-rw-r--r--   0 runner    (1001) docker     (121)     1780 2022-08-12 22:04:48.000000 lean-1.0.99/lean/models/brokerages/local/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1418 2022-08-12 22:04:48.000000 lean-1.0.99/lean/models/brokerages/local/local_brokerage.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1409 2022-08-12 22:04:48.000000 lean-1.0.99/lean/models/brokerages/local/data_feed.py
+-rw-r--r--   0 runner    (1001) docker     (121)      664 2022-08-12 22:04:48.000000 lean-1.0.99/lean/models/brokerages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3936 2022-08-12 22:04:48.000000 lean-1.0.99/lean/models/options.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17999 2022-08-12 22:04:48.000000 lean-1.0.99/lean/models/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1491 2022-08-12 22:04:48.000000 lean-1.0.99/lean/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14294 2022-08-12 22:04:48.000000 lean-1.0.99/lean/models/api.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1416 2022-08-12 22:04:48.000000 lean-1.0.99/lean/models/docker.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1513 2022-08-12 22:04:48.000000 lean-1.0.99/lean/models/modules.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17459 2022-08-12 22:04:48.000000 lean-1.0.99/lean/models/data.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1924 2022-08-12 22:04:48.000000 lean-1.0.99/lean/models/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2248 2022-08-12 22:04:48.000000 lean-1.0.99/lean/models/errors.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8876 2022-08-12 22:04:48.000000 lean-1.0.99/lean/models/json_module.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1622 2022-08-12 22:04:48.000000 lean-1.0.99/lean/models/market_hours_database.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1407 2022-08-12 22:04:48.000000 lean-1.0.99/lean/models/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5856 2022-08-12 22:04:48.000000 lean-1.0.99/lean/main.py
+-rw-r--r--   0 runner    (1001) docker     (121)      914 2022-08-12 22:04:53.000000 lean-1.0.99/lean/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-12 22:04:54.000000 lean-1.0.99/lean/ssh/
+-rw-r--r--   0 runner    (1001) docker     (121)      411 2022-08-12 22:04:48.000000 lean-1.0.99/lean/ssh/key.pub
+-rw-r--r--   0 runner    (1001) docker     (121)     1679 2022-08-12 22:04:48.000000 lean-1.0.99/lean/ssh/key
+-rw-r--r--   0 runner    (1001) docker     (121)      274 2022-08-12 22:04:48.000000 lean-1.0.99/lean/ssh/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-12 22:04:54.000000 lean-1.0.99/lean/components/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-12 22:04:54.000000 lean-1.0.99/lean/components/api/
+-rw-r--r--   0 runner    (1001) docker     (121)     1387 2022-08-12 22:04:48.000000 lean-1.0.99/lean/components/api/market_client.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1497 2022-08-12 22:04:48.000000 lean-1.0.99/lean/components/api/service_client.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4213 2022-08-12 22:04:48.000000 lean-1.0.99/lean/components/api/backtest_client.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7716 2022-08-12 22:04:48.000000 lean-1.0.99/lean/components/api/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3453 2022-08-12 22:04:48.000000 lean-1.0.99/lean/components/api/file_client.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2250 2022-08-12 22:04:48.000000 lean-1.0.99/lean/components/api/module_client.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5227 2022-08-12 22:04:48.000000 lean-1.0.99/lean/components/api/project_client.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1663 2022-08-12 22:04:48.000000 lean-1.0.99/lean/components/api/user_client.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1640 2022-08-12 22:04:48.000000 lean-1.0.99/lean/components/api/account_client.py
+-rw-r--r--   0 runner    (1001) docker     (121)      664 2022-08-12 22:04:48.000000 lean-1.0.99/lean/components/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2023 2022-08-12 22:04:48.000000 lean-1.0.99/lean/components/api/organization_client.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3332 2022-08-12 22:04:48.000000 lean-1.0.99/lean/components/api/node_client.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4700 2022-08-12 22:04:48.000000 lean-1.0.99/lean/components/api/data_client.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8441 2022-08-12 22:04:48.000000 lean-1.0.99/lean/components/api/optimization_client.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2003 2022-08-12 22:04:48.000000 lean-1.0.99/lean/components/api/compile_client.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5168 2022-08-12 22:04:48.000000 lean-1.0.99/lean/components/api/live_client.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-12 22:04:54.000000 lean-1.0.99/lean/components/cloud/
+-rw-r--r--   0 runner    (1001) docker     (121)     8981 2022-08-12 22:04:48.000000 lean-1.0.99/lean/components/cloud/pull_manager.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7803 2022-08-12 22:04:48.000000 lean-1.0.99/lean/components/cloud/cloud_runner.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4789 2022-08-12 22:04:48.000000 lean-1.0.99/lean/components/cloud/cloud_project_manager.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7506 2022-08-12 22:04:48.000000 lean-1.0.99/lean/components/cloud/push_manager.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7248 2022-08-12 22:04:48.000000 lean-1.0.99/lean/components/cloud/data_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (121)      664 2022-08-12 22:04:48.000000 lean-1.0.99/lean/components/cloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5600 2022-08-12 22:04:48.000000 lean-1.0.99/lean/components/cloud/module_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-12 22:04:54.000000 lean-1.0.99/lean/components/docker/
+-rw-r--r--   0 runner    (1001) docker     (121)    35810 2022-08-12 22:04:48.000000 lean-1.0.99/lean/components/docker/lean_runner.py
+-rw-r--r--   0 runner    (1001) docker     (121)      664 2022-08-12 22:04:48.000000 lean-1.0.99/lean/components/docker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    23324 2022-08-12 22:04:48.000000 lean-1.0.99/lean/components/docker/docker_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-12 22:04:54.000000 lean-1.0.99/lean/components/config/
+-rw-r--r--   0 runner    (1001) docker     (121)     5050 2022-08-12 22:04:48.000000 lean-1.0.99/lean/components/config/cli_config_manager.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13245 2022-08-12 22:04:48.000000 lean-1.0.99/lean/components/config/lean_config_manager.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3108 2022-08-12 22:04:48.000000 lean-1.0.99/lean/components/config/storage.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6255 2022-08-12 22:04:48.000000 lean-1.0.99/lean/components/config/output_config_manager.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10763 2022-08-12 22:04:48.000000 lean-1.0.99/lean/components/config/optimizer_config_manager.py
+-rw-r--r--   0 runner    (1001) docker     (121)      664 2022-08-12 22:04:48.000000 lean-1.0.99/lean/components/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4130 2022-08-12 22:04:48.000000 lean-1.0.99/lean/components/config/project_config_manager.py
+-rw-r--r--   0 runner    (1001) docker     (121)      664 2022-08-12 22:04:48.000000 lean-1.0.99/lean/components/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-12 22:04:54.000000 lean-1.0.99/lean/components/util/
+-rw-r--r--   0 runner    (1001) docker     (121)     1728 2022-08-12 22:04:48.000000 lean-1.0.99/lean/components/util/click_group_default_command.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4455 2022-08-12 22:04:48.000000 lean-1.0.99/lean/components/util/http_client.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3188 2022-08-12 22:04:48.000000 lean-1.0.99/lean/components/util/path_manager.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1010 2022-08-12 22:04:48.000000 lean-1.0.99/lean/components/util/click_custom_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5676 2022-08-12 22:04:48.000000 lean-1.0.99/lean/components/util/logger.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6518 2022-08-12 22:04:48.000000 lean-1.0.99/lean/components/util/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4474 2022-08-12 22:04:48.000000 lean-1.0.99/lean/components/util/platform_manager.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4440 2022-08-12 22:04:48.000000 lean-1.0.99/lean/components/util/task_manager.py
+-rw-r--r--   0 runner    (1001) docker     (121)      664 2022-08-12 22:04:48.000000 lean-1.0.99/lean/components/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    22077 2022-08-12 22:04:48.000000 lean-1.0.99/lean/components/util/project_manager.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1641 2022-08-12 22:04:48.000000 lean-1.0.99/lean/components/util/xml_manager.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7677 2022-08-12 22:04:48.000000 lean-1.0.99/lean/components/util/update_manager.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1647 2022-08-12 22:04:48.000000 lean-1.0.99/lean/components/util/temp_manager.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1335 2022-08-12 22:04:48.000000 lean-1.0.99/lean/components/util/name_extraction.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3156 2022-08-12 22:04:48.000000 lean-1.0.99/lean/components/util/name_generator.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3174 2022-08-12 22:04:48.000000 lean-1.0.99/lean/components/util/market_hours_database.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11687 2022-08-12 22:04:48.000000 lean-1.0.99/lean/click.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4135 2022-08-12 22:04:48.000000 lean-1.0.99/lean/constants.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3291 2022-08-12 22:04:48.000000 lean-1.0.99/setup.py
+-rw-r--r--   0 runner    (1001) docker     (121)    59277 2022-08-12 22:04:48.000000 lean-1.0.99/README.md
```

### Comparing `lean-1.0.98/PKG-INFO` & `lean-1.0.99/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lean
-Version: 1.0.98
+Version: 1.0.99
 Summary: A CLI aimed at making it easier to run QuantConnect's LEAN engine locally and in the cloud
 Home-page: https://lean.io/cli
 Author: QuantConnect
 Author-email: support@quantconnect.com
 License: UNKNOWN
 Project-URL: Documentation, https://www.lean.io/docs/lean-cli/key-concepts/getting-started
 Project-URL: Source, https://github.com/QuantConnect/lean-cli
@@ -78,14 +78,17 @@
         *Note: the readme only contains the `--help` text of all commands. Visit the [documentation website](https://www.lean.io/docs/lean-cli/key-concepts/getting-started) for more comprehensive documentation.*
         
         <!-- commands start -->
         - [`lean backtest`](#lean-backtest)
         - [`lean build`](#lean-build)
         - [`lean cloud backtest`](#lean-cloud-backtest)
         - [`lean cloud live`](#lean-cloud-live)
+        - [`lean cloud live deploy`](#lean-cloud-live-deploy)
+        - [`lean cloud live liquidate`](#lean-cloud-live-liquidate)
+        - [`lean cloud live stop`](#lean-cloud-live-stop)
         - [`lean cloud optimize`](#lean-cloud-optimize)
         - [`lean cloud pull`](#lean-cloud-pull)
         - [`lean cloud push`](#lean-cloud-push)
         - [`lean cloud status`](#lean-cloud-status)
         - [`lean config get`](#lean-config-get)
         - [`lean config list`](#lean-config-list)
         - [`lean config set`](#lean-config-set)
@@ -93,14 +96,21 @@
         - [`lean create-project`](#lean-create-project)
         - [`lean data download`](#lean-data-download)
         - [`lean data generate`](#lean-data-generate)
         - [`lean init`](#lean-init)
         - [`lean library add`](#lean-library-add)
         - [`lean library remove`](#lean-library-remove)
         - [`lean live`](#lean-live)
+        - [`lean live add-security`](#lean-live-add-security)
+        - [`lean live cancel-order`](#lean-live-cancel-order)
+        - [`lean live deploy`](#lean-live-deploy)
+        - [`lean live liquidate`](#lean-live-liquidate)
+        - [`lean live stop`](#lean-live-stop)
+        - [`lean live submit-order`](#lean-live-submit-order)
+        - [`lean live update-order`](#lean-live-update-order)
         - [`lean login`](#lean-login)
         - [`lean logout`](#lean-logout)
         - [`lean logs`](#lean-logs)
         - [`lean optimize`](#lean-optimize)
         - [`lean report`](#lean-report)
         - [`lean research`](#lean-research)
         - [`lean whoami`](#lean-whoami)
@@ -201,18 +211,38 @@
           --help       Show this message and exit.
         ```
         
         _See code: [lean/commands/cloud/backtest.py](https://github.com/QuantConnect/lean-cli/blob/master/lean/commands/cloud/backtest.py)_
         
         ### `lean cloud live`
         
+        Interact with the QuantConnect cloud live deployments.
+        
+        ```
+        Usage: lean cloud live [OPTIONS] COMMAND [ARGS]...
+        
+          Interact with the QuantConnect cloud live deployments.
+        
+        Options:
+          --help  Show this message and exit.
+        
+        Commands:
+          deploy     Start live trading for a project in the cloud.
+          liquidate  Stops live trading and liquidates existing positions for a certain project.
+          stop       Stops live trading for a certain project without liquidating existing positions.
+        ```
+        
+        _See code: [lean/commands/cloud/live.py](https://github.com/QuantConnect/lean-cli/blob/master/lean/commands/cloud/live.py)_
+        
+        ### `lean cloud live deploy`
+        
         Start live trading for a project in the cloud.
         
         ```
-        Usage: lean cloud live [OPTIONS] PROJECT
+        Usage: lean cloud live deploy [OPTIONS] PROJECT
         
           Start live trading for a project in the cloud.
         
           PROJECT must be the name or the id of the project to start live trading for.
         
           By default an interactive wizard is shown letting you configure the deployment. If --brokerage is given the command
           runs in non-interactive mode. In this mode the CLI does not prompt for input or confirmation. In non-interactive mode
@@ -248,27 +278,29 @@
                                           Whether the testnet should be used
           --binance-api-key TEXT          Your Binance API key
           --binanceus-api-key TEXT        Your Binance API key
           --binance-api-secret TEXT       Your Binance API secret
           --binanceus-api-secret TEXT     Your Binance API secret
           --zerodha-api-key TEXT          Your Kite Connect API key
           --zerodha-access-token TEXT     Your Kite Connect access token
-          --zerodha-product-type [MIS|CNC|NRML]
+          --zerodha-product-type [mis|cnc|nrml]
                                           MIS if you are targeting intraday products, CNC if you are targeting delivery
                                           products, NRML if you are targeting carry forward products
-          --zerodha-trading-segment [EQUITY|COMMODITY]
+          --zerodha-trading-segment [equity|commodity]
                                           EQUITY if you are trading equities on NSE or BSE, COMMODITY if you are trading
                                           commodities on MCX
+          --zerodha-history-subscription [true|false]
+                                          Whether you have a history API subscription for Zerodha
           --samco-client-id TEXT          Your Samco account Client ID
           --samco-client-password TEXT    Your Samco account password
           --samco-year-of-birth TEXT      Your year of birth (YYYY) registered with Samco
-          --samco-product-type [MIS|CNC|NRML]
+          --samco-product-type [mis|cnc|nrml]
                                           MIS if you are targeting intraday products, CNC if you are targeting delivery
                                           products, NRML if you are targeting carry forward products
-          --samco-trading-segment [EQUITY|COMMODITY]
+          --samco-trading-segment [equity|commodity]
                                           EQUITY if you are trading equities on NSE or BSE, COMMODITY if you are trading
                                           commodities on MCX
           --kraken-api-key TEXT           Your Kraken API key
           --kraken-api-secret TEXT        Your Kraken API secret
           --kraken-verification-tier [Starter|Intermediate|Pro]
                                           Your Kraken Verification Tier
           --ftx-exchange-name [FTX|FTXUS]
@@ -291,15 +323,47 @@
           --notify-sms TEXT               A comma-separated list of phone numbers configuring SMS-notifications
           --push                          Push local modifications to the cloud before starting live trading
           --open                          Automatically open the live results in the browser once the deployment starts
           --verbose                       Enable debug logging
           --help                          Show this message and exit.
         ```
         
-        _See code: [lean/commands/cloud/live.py](https://github.com/QuantConnect/lean-cli/blob/master/lean/commands/cloud/live.py)_
+        _See code: [lean/commands/cloud/live/deploy.py](https://github.com/QuantConnect/lean-cli/blob/master/lean/commands/cloud/live/deploy.py)_
+        
+        ### `lean cloud live liquidate`
+        
+        Stops live trading and liquidates existing positions for a certain project.
+        
+        ```
+        Usage: lean cloud live liquidate [OPTIONS] PROJECT
+        
+          Stops live trading and liquidates existing positions for a certain project.
+        
+        Options:
+          --verbose  Enable debug logging
+          --help     Show this message and exit.
+        ```
+        
+        _See code: [lean/commands/cloud/live/liquidate.py](https://github.com/QuantConnect/lean-cli/blob/master/lean/commands/cloud/live/liquidate.py)_
+        
+        ### `lean cloud live stop`
+        
+        Stops live trading for a certain project without liquidating existing positions.
+        
+        ```
+        Usage: lean cloud live stop [OPTIONS] PROJECT
+        
+          Stops live trading for a certain project without liquidating existing positions.
+        
+        Options:
+          --verbose  Enable debug logging
+          --help     Show this message and exit.
+        ```
+        
+        _See code: [lean/commands/cloud/live/stop.py](https://github.com/QuantConnect/lean-cli/blob/master/lean/commands/cloud/live/stop.py)_
         
         ### `lean cloud optimize`
         
         Optimize a project in the cloud.
         
         ```
         Usage: lean cloud optimize [OPTIONS] PROJECT
@@ -665,18 +729,86 @@
           --help      Show this message and exit.
         ```
         
         _See code: [lean/commands/library/remove.py](https://github.com/QuantConnect/lean-cli/blob/master/lean/commands/library/remove.py)_
         
         ### `lean live`
         
+        Interact with the local machine.
+        
+        ```
+        Usage: lean live [OPTIONS] COMMAND [ARGS]...
+        
+          Interact with the local machine.
+        
+        Options:
+          --help  Show this message and exit.
+        
+        Commands:
+          add-security  Represents a command to add a security to the algorithm.
+          cancel-order  Represents a command to cancel a specific order by id.
+          deploy        Start live trading a project locally using Docker.
+          liquidate     Liquidate the given symbol from the latest deployment of the given project.
+          stop          Stop an already running local live trading project.
+          submit-order  Represents a command to submit an order to the algorithm.
+          update-order  Represents a command to update a specific order by id.
+        ```
+        
+        _See code: [lean/commands/live.py](https://github.com/QuantConnect/lean-cli/blob/master/lean/commands/live.py)_
+        
+        ### `lean live add-security`
+        
+        Represents a command to add a security to the algorithm.
+        
+        ```
+        Usage: lean live add-security [OPTIONS] PROJECT
+        
+          Represents a command to add a security to the algorithm.
+        
+        Options:
+          --ticker TEXT            The ticker of the symbol to add  [required]
+          --market TEXT            The market of the symbol to add  [required]
+          --security-type TEXT     The security type of the symbol to add  [required]
+          --resolution TEXT        The resolution of the symbol to add
+          --fill-data-forward      The fill forward behavior, true to fill forward, false otherwise - defaults to true
+          --leverage DECIMAL       The leverage for the security, defaults to 2 for equity, 50 for forex, and 1 for everything
+                                   else
+          --extended-market-hours  The extended market hours flag, true to allow pre/post market data, false for only in market
+                                   data
+          --lean-config FILE       The Lean configuration file that should be used (defaults to the nearest lean.json)
+          --verbose                Enable debug logging
+          --help                   Show this message and exit.
+        ```
+        
+        _See code: [lean/commands/live/add_security.py](https://github.com/QuantConnect/lean-cli/blob/master/lean/commands/live/add_security.py)_
+        
+        ### `lean live cancel-order`
+        
+        Represents a command to cancel a specific order by id.
+        
+        ```
+        Usage: lean live cancel-order [OPTIONS] PROJECT
+        
+          Represents a command to cancel a specific order by id.
+        
+        Options:
+          --order-id INTEGER  The order id to be cancelled  [required]
+          --lean-config FILE  The Lean configuration file that should be used (defaults to the nearest lean.json)
+          --verbose           Enable debug logging
+          --help              Show this message and exit.
+        ```
+        
+        _See code: [lean/commands/live/cancel_order.py](https://github.com/QuantConnect/lean-cli/blob/master/lean/commands/live/cancel_order.py)_
+        
+        ### `lean live deploy`
+        
         Start live trading a project locally using Docker.
         
         ```
-        Usage: lean live [OPTIONS] PROJECT
+        Usage: lean live deploy [OPTIONS] PROJECT
         
           Start live trading a project locally using Docker.
         
           If PROJECT is a directory, the algorithm in the main.py or Main.cs file inside it will be executed.
           If PROJECT is a file, the algorithm in the specified file will be executed.
         
           By default an interactive wizard is shown letting you configure the brokerage and data feed to use. If --environment,
@@ -736,30 +868,30 @@
           --binance-api-key TEXT          Your Binance API key
           --binanceus-api-key TEXT        Your Binance API key
           --binance-api-secret TEXT       Your Binance API secret
           --binanceus-api-secret TEXT     Your Binance API secret
           --zerodha-organization TEXT     The name or id of the organization with the zerodha module subscription
           --zerodha-api-key TEXT          Your Kite Connect API key
           --zerodha-access-token TEXT     Your Kite Connect access token
-          --zerodha-product-type [MIS|CNC|NRML]
+          --zerodha-product-type [mis|cnc|nrml]
                                           MIS if you are targeting intraday products, CNC if you are targeting delivery
                                           products, NRML if you are targeting carry forward products
-          --zerodha-trading-segment [EQUITY|COMMODITY]
+          --zerodha-trading-segment [equity|commodity]
                                           EQUITY if you are trading equities on NSE or BSE, COMMODITY if you are trading
                                           commodities on MCX
-          --zerodha-history-subscription BOOLEAN
+          --zerodha-history-subscription [true|false]
                                           Whether you have a history API subscription for Zerodha
           --samco-organization TEXT       The name or id of the organization with the samco module subscription
           --samco-client-id TEXT          Your Samco account Client ID
           --samco-client-password TEXT    Your Samco account password
           --samco-year-of-birth TEXT      Your year of birth (YYYY) registered with Samco
-          --samco-product-type [MIS|CNC|NRML]
+          --samco-product-type [mis|cnc|nrml]
                                           MIS if you are targeting intraday products, CNC if you are targeting delivery
                                           products, NRML if you are targeting carry forward products
-          --samco-trading-segment [EQUITY|COMMODITY]
+          --samco-trading-segment [equity|commodity]
                                           EQUITY if you are trading equities on NSE or BSE, COMMODITY if you are trading
                                           commodities on MCX
           --terminal-link-organization TEXT
                                           The name or id of the organization with the Terminal Link module subscription
           --bloomberg-environment [Production|Beta]
                                           The environment to run in
           --bloomberg-server-host TEXT    The host of the Bloomberg server
@@ -833,15 +965,99 @@
           --image TEXT                    The LEAN engine image to use (defaults to quantconnect/lean:latest)
           --update                        Pull the LEAN engine image before starting live trading
           --lean-config FILE              The Lean configuration file that should be used (defaults to the nearest lean.json)
           --verbose                       Enable debug logging
           --help                          Show this message and exit.
         ```
         
-        _See code: [lean/commands/live.py](https://github.com/QuantConnect/lean-cli/blob/master/lean/commands/live.py)_
+        _See code: [lean/commands/live/deploy.py](https://github.com/QuantConnect/lean-cli/blob/master/lean/commands/live/deploy.py)_
+        
+        ### `lean live liquidate`
+        
+        Liquidate the given symbol from the latest deployment of the given project.
+        
+        ```
+        Usage: lean live liquidate [OPTIONS] PROJECT
+        
+          Liquidate the given symbol from the latest deployment of the given project.
+        
+        Options:
+          --ticker TEXT         The ticker of the symbol to liquidate
+          --market TEXT         The market of the symbol to liquidate
+          --security-type TEXT  The security type of the symbol to liquidate
+          --lean-config FILE    The Lean configuration file that should be used (defaults to the nearest lean.json)
+          --verbose             Enable debug logging
+          --help                Show this message and exit.
+        ```
+        
+        _See code: [lean/commands/live/liquidate.py](https://github.com/QuantConnect/lean-cli/blob/master/lean/commands/live/liquidate.py)_
+        
+        ### `lean live stop`
+        
+        Stop an already running local live trading project.
+        
+        ```
+        Usage: lean live stop [OPTIONS] PROJECT
+        
+          Stop an already running local live trading project.
+        
+        Options:
+          --lean-config FILE  The Lean configuration file that should be used (defaults to the nearest lean.json)
+          --verbose           Enable debug logging
+          --help              Show this message and exit.
+        ```
+        
+        _See code: [lean/commands/live/stop.py](https://github.com/QuantConnect/lean-cli/blob/master/lean/commands/live/stop.py)_
+        
+        ### `lean live submit-order`
+        
+        Represents a command to submit an order to the algorithm.
+        
+        ```
+        Usage: lean live submit-order [OPTIONS] PROJECT
+        
+          Represents a command to submit an order to the algorithm.
+        
+        Options:
+          --ticker TEXT          The ticker of the symbol to be submitted  [required]
+          --market TEXT          The market of the symbol to be submitted  [required]
+          --security-type TEXT   The security type of the symbol to be submitted  [required]
+          --order-type TEXT      The order type to be submitted  [required]
+          --quantity DECIMAL     The number of units to be ordered (directional)  [required]
+          --limit-price DECIMAL  The limit price of the order be submitted
+          --stop-price DECIMAL   The stop price of the order to be submitted
+          --tag TEXT             The tag to be attached to the order
+          --lean-config FILE     The Lean configuration file that should be used (defaults to the nearest lean.json)
+          --verbose              Enable debug logging
+          --help                 Show this message and exit.
+        ```
+        
+        _See code: [lean/commands/live/submit_order.py](https://github.com/QuantConnect/lean-cli/blob/master/lean/commands/live/submit_order.py)_
+        
+        ### `lean live update-order`
+        
+        Represents a command to update a specific order by id.
+        
+        ```
+        Usage: lean live update-order [OPTIONS] PROJECT
+        
+          Represents a command to update a specific order by id.
+        
+        Options:
+          --order-id INTEGER     The order id to be updated  [required]
+          --quantity DECIMAL     The number of units to be updated (directional)
+          --limit-price DECIMAL  The limit price of the order to be updated
+          --stop-price DECIMAL   The stop price of the order to be updated
+          --tag TEXT             The tag to be attached to the order
+          --lean-config FILE     The Lean configuration file that should be used (defaults to the nearest lean.json)
+          --verbose              Enable debug logging
+          --help                 Show this message and exit.
+        ```
+        
+        _See code: [lean/commands/live/update_order.py](https://github.com/QuantConnect/lean-cli/blob/master/lean/commands/live/update_order.py)_
         
         ### `lean login`
         
         Log in with a QuantConnect account.
         
         ```
         Usage: lean login [OPTIONS]
```

### Comparing `lean-1.0.98/lean.egg-info/SOURCES.txt` & `lean-1.0.99/lean.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -12,40 +12,52 @@
 lean.egg-info/requires.txt
 lean.egg-info/top_level.txt
 lean/commands/__init__.py
 lean/commands/backtest.py
 lean/commands/build.py
 lean/commands/create_project.py
 lean/commands/init.py
-lean/commands/live.py
 lean/commands/login.py
 lean/commands/logout.py
 lean/commands/logs.py
 lean/commands/optimize.py
 lean/commands/report.py
 lean/commands/research.py
 lean/commands/whoami.py
 lean/commands/cloud/__init__.py
 lean/commands/cloud/backtest.py
-lean/commands/cloud/live.py
 lean/commands/cloud/optimize.py
 lean/commands/cloud/pull.py
 lean/commands/cloud/push.py
 lean/commands/cloud/status.py
+lean/commands/cloud/live/__init__.py
+lean/commands/cloud/live/deploy.py
+lean/commands/cloud/live/liquidate.py
+lean/commands/cloud/live/live.py
+lean/commands/cloud/live/stop.py
 lean/commands/config/__init__.py
 lean/commands/config/get.py
 lean/commands/config/list.py
 lean/commands/config/set.py
 lean/commands/config/unset.py
 lean/commands/data/__init__.py
 lean/commands/data/download.py
 lean/commands/data/generate.py
 lean/commands/library/__init__.py
 lean/commands/library/add.py
 lean/commands/library/remove.py
+lean/commands/live/__init__.py
+lean/commands/live/add_security.py
+lean/commands/live/cancel_order.py
+lean/commands/live/deploy.py
+lean/commands/live/liquidate.py
+lean/commands/live/live.py
+lean/commands/live/stop.py
+lean/commands/live/submit_order.py
+lean/commands/live/update_order.py
 lean/components/__init__.py
 lean/components/api/__init__.py
 lean/components/api/account_client.py
 lean/components/api/api_client.py
 lean/components/api/backtest_client.py
 lean/components/api/compile_client.py
 lean/components/api/data_client.py
@@ -73,14 +85,16 @@
 lean/components/config/output_config_manager.py
 lean/components/config/project_config_manager.py
 lean/components/config/storage.py
 lean/components/docker/__init__.py
 lean/components/docker/docker_manager.py
 lean/components/docker/lean_runner.py
 lean/components/util/__init__.py
+lean/components/util/click_custom_parameters.py
+lean/components/util/click_group_default_command.py
 lean/components/util/compiler.py
 lean/components/util/http_client.py
 lean/components/util/logger.py
 lean/components/util/market_hours_database.py
 lean/components/util/name_extraction.py
 lean/components/util/name_generator.py
 lean/components/util/path_manager.py
```

### Comparing `lean-1.0.98/lean.egg-info/PKG-INFO` & `lean-1.0.99/lean.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lean
-Version: 1.0.98
+Version: 1.0.99
 Summary: A CLI aimed at making it easier to run QuantConnect's LEAN engine locally and in the cloud
 Home-page: https://lean.io/cli
 Author: QuantConnect
 Author-email: support@quantconnect.com
 License: UNKNOWN
 Project-URL: Documentation, https://www.lean.io/docs/lean-cli/key-concepts/getting-started
 Project-URL: Source, https://github.com/QuantConnect/lean-cli
@@ -78,14 +78,17 @@
         *Note: the readme only contains the `--help` text of all commands. Visit the [documentation website](https://www.lean.io/docs/lean-cli/key-concepts/getting-started) for more comprehensive documentation.*
         
         <!-- commands start -->
         - [`lean backtest`](#lean-backtest)
         - [`lean build`](#lean-build)
         - [`lean cloud backtest`](#lean-cloud-backtest)
         - [`lean cloud live`](#lean-cloud-live)
+        - [`lean cloud live deploy`](#lean-cloud-live-deploy)
+        - [`lean cloud live liquidate`](#lean-cloud-live-liquidate)
+        - [`lean cloud live stop`](#lean-cloud-live-stop)
         - [`lean cloud optimize`](#lean-cloud-optimize)
         - [`lean cloud pull`](#lean-cloud-pull)
         - [`lean cloud push`](#lean-cloud-push)
         - [`lean cloud status`](#lean-cloud-status)
         - [`lean config get`](#lean-config-get)
         - [`lean config list`](#lean-config-list)
         - [`lean config set`](#lean-config-set)
@@ -93,14 +96,21 @@
         - [`lean create-project`](#lean-create-project)
         - [`lean data download`](#lean-data-download)
         - [`lean data generate`](#lean-data-generate)
         - [`lean init`](#lean-init)
         - [`lean library add`](#lean-library-add)
         - [`lean library remove`](#lean-library-remove)
         - [`lean live`](#lean-live)
+        - [`lean live add-security`](#lean-live-add-security)
+        - [`lean live cancel-order`](#lean-live-cancel-order)
+        - [`lean live deploy`](#lean-live-deploy)
+        - [`lean live liquidate`](#lean-live-liquidate)
+        - [`lean live stop`](#lean-live-stop)
+        - [`lean live submit-order`](#lean-live-submit-order)
+        - [`lean live update-order`](#lean-live-update-order)
         - [`lean login`](#lean-login)
         - [`lean logout`](#lean-logout)
         - [`lean logs`](#lean-logs)
         - [`lean optimize`](#lean-optimize)
         - [`lean report`](#lean-report)
         - [`lean research`](#lean-research)
         - [`lean whoami`](#lean-whoami)
@@ -201,18 +211,38 @@
           --help       Show this message and exit.
         ```
         
         _See code: [lean/commands/cloud/backtest.py](https://github.com/QuantConnect/lean-cli/blob/master/lean/commands/cloud/backtest.py)_
         
         ### `lean cloud live`
         
+        Interact with the QuantConnect cloud live deployments.
+        
+        ```
+        Usage: lean cloud live [OPTIONS] COMMAND [ARGS]...
+        
+          Interact with the QuantConnect cloud live deployments.
+        
+        Options:
+          --help  Show this message and exit.
+        
+        Commands:
+          deploy     Start live trading for a project in the cloud.
+          liquidate  Stops live trading and liquidates existing positions for a certain project.
+          stop       Stops live trading for a certain project without liquidating existing positions.
+        ```
+        
+        _See code: [lean/commands/cloud/live.py](https://github.com/QuantConnect/lean-cli/blob/master/lean/commands/cloud/live.py)_
+        
+        ### `lean cloud live deploy`
+        
         Start live trading for a project in the cloud.
         
         ```
-        Usage: lean cloud live [OPTIONS] PROJECT
+        Usage: lean cloud live deploy [OPTIONS] PROJECT
         
           Start live trading for a project in the cloud.
         
           PROJECT must be the name or the id of the project to start live trading for.
         
           By default an interactive wizard is shown letting you configure the deployment. If --brokerage is given the command
           runs in non-interactive mode. In this mode the CLI does not prompt for input or confirmation. In non-interactive mode
@@ -248,27 +278,29 @@
                                           Whether the testnet should be used
           --binance-api-key TEXT          Your Binance API key
           --binanceus-api-key TEXT        Your Binance API key
           --binance-api-secret TEXT       Your Binance API secret
           --binanceus-api-secret TEXT     Your Binance API secret
           --zerodha-api-key TEXT          Your Kite Connect API key
           --zerodha-access-token TEXT     Your Kite Connect access token
-          --zerodha-product-type [MIS|CNC|NRML]
+          --zerodha-product-type [mis|cnc|nrml]
                                           MIS if you are targeting intraday products, CNC if you are targeting delivery
                                           products, NRML if you are targeting carry forward products
-          --zerodha-trading-segment [EQUITY|COMMODITY]
+          --zerodha-trading-segment [equity|commodity]
                                           EQUITY if you are trading equities on NSE or BSE, COMMODITY if you are trading
                                           commodities on MCX
+          --zerodha-history-subscription [true|false]
+                                          Whether you have a history API subscription for Zerodha
           --samco-client-id TEXT          Your Samco account Client ID
           --samco-client-password TEXT    Your Samco account password
           --samco-year-of-birth TEXT      Your year of birth (YYYY) registered with Samco
-          --samco-product-type [MIS|CNC|NRML]
+          --samco-product-type [mis|cnc|nrml]
                                           MIS if you are targeting intraday products, CNC if you are targeting delivery
                                           products, NRML if you are targeting carry forward products
-          --samco-trading-segment [EQUITY|COMMODITY]
+          --samco-trading-segment [equity|commodity]
                                           EQUITY if you are trading equities on NSE or BSE, COMMODITY if you are trading
                                           commodities on MCX
           --kraken-api-key TEXT           Your Kraken API key
           --kraken-api-secret TEXT        Your Kraken API secret
           --kraken-verification-tier [Starter|Intermediate|Pro]
                                           Your Kraken Verification Tier
           --ftx-exchange-name [FTX|FTXUS]
@@ -291,15 +323,47 @@
           --notify-sms TEXT               A comma-separated list of phone numbers configuring SMS-notifications
           --push                          Push local modifications to the cloud before starting live trading
           --open                          Automatically open the live results in the browser once the deployment starts
           --verbose                       Enable debug logging
           --help                          Show this message and exit.
         ```
         
-        _See code: [lean/commands/cloud/live.py](https://github.com/QuantConnect/lean-cli/blob/master/lean/commands/cloud/live.py)_
+        _See code: [lean/commands/cloud/live/deploy.py](https://github.com/QuantConnect/lean-cli/blob/master/lean/commands/cloud/live/deploy.py)_
+        
+        ### `lean cloud live liquidate`
+        
+        Stops live trading and liquidates existing positions for a certain project.
+        
+        ```
+        Usage: lean cloud live liquidate [OPTIONS] PROJECT
+        
+          Stops live trading and liquidates existing positions for a certain project.
+        
+        Options:
+          --verbose  Enable debug logging
+          --help     Show this message and exit.
+        ```
+        
+        _See code: [lean/commands/cloud/live/liquidate.py](https://github.com/QuantConnect/lean-cli/blob/master/lean/commands/cloud/live/liquidate.py)_
+        
+        ### `lean cloud live stop`
+        
+        Stops live trading for a certain project without liquidating existing positions.
+        
+        ```
+        Usage: lean cloud live stop [OPTIONS] PROJECT
+        
+          Stops live trading for a certain project without liquidating existing positions.
+        
+        Options:
+          --verbose  Enable debug logging
+          --help     Show this message and exit.
+        ```
+        
+        _See code: [lean/commands/cloud/live/stop.py](https://github.com/QuantConnect/lean-cli/blob/master/lean/commands/cloud/live/stop.py)_
         
         ### `lean cloud optimize`
         
         Optimize a project in the cloud.
         
         ```
         Usage: lean cloud optimize [OPTIONS] PROJECT
@@ -665,18 +729,86 @@
           --help      Show this message and exit.
         ```
         
         _See code: [lean/commands/library/remove.py](https://github.com/QuantConnect/lean-cli/blob/master/lean/commands/library/remove.py)_
         
         ### `lean live`
         
+        Interact with the local machine.
+        
+        ```
+        Usage: lean live [OPTIONS] COMMAND [ARGS]...
+        
+          Interact with the local machine.
+        
+        Options:
+          --help  Show this message and exit.
+        
+        Commands:
+          add-security  Represents a command to add a security to the algorithm.
+          cancel-order  Represents a command to cancel a specific order by id.
+          deploy        Start live trading a project locally using Docker.
+          liquidate     Liquidate the given symbol from the latest deployment of the given project.
+          stop          Stop an already running local live trading project.
+          submit-order  Represents a command to submit an order to the algorithm.
+          update-order  Represents a command to update a specific order by id.
+        ```
+        
+        _See code: [lean/commands/live.py](https://github.com/QuantConnect/lean-cli/blob/master/lean/commands/live.py)_
+        
+        ### `lean live add-security`
+        
+        Represents a command to add a security to the algorithm.
+        
+        ```
+        Usage: lean live add-security [OPTIONS] PROJECT
+        
+          Represents a command to add a security to the algorithm.
+        
+        Options:
+          --ticker TEXT            The ticker of the symbol to add  [required]
+          --market TEXT            The market of the symbol to add  [required]
+          --security-type TEXT     The security type of the symbol to add  [required]
+          --resolution TEXT        The resolution of the symbol to add
+          --fill-data-forward      The fill forward behavior, true to fill forward, false otherwise - defaults to true
+          --leverage DECIMAL       The leverage for the security, defaults to 2 for equity, 50 for forex, and 1 for everything
+                                   else
+          --extended-market-hours  The extended market hours flag, true to allow pre/post market data, false for only in market
+                                   data
+          --lean-config FILE       The Lean configuration file that should be used (defaults to the nearest lean.json)
+          --verbose                Enable debug logging
+          --help                   Show this message and exit.
+        ```
+        
+        _See code: [lean/commands/live/add_security.py](https://github.com/QuantConnect/lean-cli/blob/master/lean/commands/live/add_security.py)_
+        
+        ### `lean live cancel-order`
+        
+        Represents a command to cancel a specific order by id.
+        
+        ```
+        Usage: lean live cancel-order [OPTIONS] PROJECT
+        
+          Represents a command to cancel a specific order by id.
+        
+        Options:
+          --order-id INTEGER  The order id to be cancelled  [required]
+          --lean-config FILE  The Lean configuration file that should be used (defaults to the nearest lean.json)
+          --verbose           Enable debug logging
+          --help              Show this message and exit.
+        ```
+        
+        _See code: [lean/commands/live/cancel_order.py](https://github.com/QuantConnect/lean-cli/blob/master/lean/commands/live/cancel_order.py)_
+        
+        ### `lean live deploy`
+        
         Start live trading a project locally using Docker.
         
         ```
-        Usage: lean live [OPTIONS] PROJECT
+        Usage: lean live deploy [OPTIONS] PROJECT
         
           Start live trading a project locally using Docker.
         
           If PROJECT is a directory, the algorithm in the main.py or Main.cs file inside it will be executed.
           If PROJECT is a file, the algorithm in the specified file will be executed.
         
           By default an interactive wizard is shown letting you configure the brokerage and data feed to use. If --environment,
@@ -736,30 +868,30 @@
           --binance-api-key TEXT          Your Binance API key
           --binanceus-api-key TEXT        Your Binance API key
           --binance-api-secret TEXT       Your Binance API secret
           --binanceus-api-secret TEXT     Your Binance API secret
           --zerodha-organization TEXT     The name or id of the organization with the zerodha module subscription
           --zerodha-api-key TEXT          Your Kite Connect API key
           --zerodha-access-token TEXT     Your Kite Connect access token
-          --zerodha-product-type [MIS|CNC|NRML]
+          --zerodha-product-type [mis|cnc|nrml]
                                           MIS if you are targeting intraday products, CNC if you are targeting delivery
                                           products, NRML if you are targeting carry forward products
-          --zerodha-trading-segment [EQUITY|COMMODITY]
+          --zerodha-trading-segment [equity|commodity]
                                           EQUITY if you are trading equities on NSE or BSE, COMMODITY if you are trading
                                           commodities on MCX
-          --zerodha-history-subscription BOOLEAN
+          --zerodha-history-subscription [true|false]
                                           Whether you have a history API subscription for Zerodha
           --samco-organization TEXT       The name or id of the organization with the samco module subscription
           --samco-client-id TEXT          Your Samco account Client ID
           --samco-client-password TEXT    Your Samco account password
           --samco-year-of-birth TEXT      Your year of birth (YYYY) registered with Samco
-          --samco-product-type [MIS|CNC|NRML]
+          --samco-product-type [mis|cnc|nrml]
                                           MIS if you are targeting intraday products, CNC if you are targeting delivery
                                           products, NRML if you are targeting carry forward products
-          --samco-trading-segment [EQUITY|COMMODITY]
+          --samco-trading-segment [equity|commodity]
                                           EQUITY if you are trading equities on NSE or BSE, COMMODITY if you are trading
                                           commodities on MCX
           --terminal-link-organization TEXT
                                           The name or id of the organization with the Terminal Link module subscription
           --bloomberg-environment [Production|Beta]
                                           The environment to run in
           --bloomberg-server-host TEXT    The host of the Bloomberg server
@@ -833,15 +965,99 @@
           --image TEXT                    The LEAN engine image to use (defaults to quantconnect/lean:latest)
           --update                        Pull the LEAN engine image before starting live trading
           --lean-config FILE              The Lean configuration file that should be used (defaults to the nearest lean.json)
           --verbose                       Enable debug logging
           --help                          Show this message and exit.
         ```
         
-        _See code: [lean/commands/live.py](https://github.com/QuantConnect/lean-cli/blob/master/lean/commands/live.py)_
+        _See code: [lean/commands/live/deploy.py](https://github.com/QuantConnect/lean-cli/blob/master/lean/commands/live/deploy.py)_
+        
+        ### `lean live liquidate`
+        
+        Liquidate the given symbol from the latest deployment of the given project.
+        
+        ```
+        Usage: lean live liquidate [OPTIONS] PROJECT
+        
+          Liquidate the given symbol from the latest deployment of the given project.
+        
+        Options:
+          --ticker TEXT         The ticker of the symbol to liquidate
+          --market TEXT         The market of the symbol to liquidate
+          --security-type TEXT  The security type of the symbol to liquidate
+          --lean-config FILE    The Lean configuration file that should be used (defaults to the nearest lean.json)
+          --verbose             Enable debug logging
+          --help                Show this message and exit.
+        ```
+        
+        _See code: [lean/commands/live/liquidate.py](https://github.com/QuantConnect/lean-cli/blob/master/lean/commands/live/liquidate.py)_
+        
+        ### `lean live stop`
+        
+        Stop an already running local live trading project.
+        
+        ```
+        Usage: lean live stop [OPTIONS] PROJECT
+        
+          Stop an already running local live trading project.
+        
+        Options:
+          --lean-config FILE  The Lean configuration file that should be used (defaults to the nearest lean.json)
+          --verbose           Enable debug logging
+          --help              Show this message and exit.
+        ```
+        
+        _See code: [lean/commands/live/stop.py](https://github.com/QuantConnect/lean-cli/blob/master/lean/commands/live/stop.py)_
+        
+        ### `lean live submit-order`
+        
+        Represents a command to submit an order to the algorithm.
+        
+        ```
+        Usage: lean live submit-order [OPTIONS] PROJECT
+        
+          Represents a command to submit an order to the algorithm.
+        
+        Options:
+          --ticker TEXT          The ticker of the symbol to be submitted  [required]
+          --market TEXT          The market of the symbol to be submitted  [required]
+          --security-type TEXT   The security type of the symbol to be submitted  [required]
+          --order-type TEXT      The order type to be submitted  [required]
+          --quantity DECIMAL     The number of units to be ordered (directional)  [required]
+          --limit-price DECIMAL  The limit price of the order be submitted
+          --stop-price DECIMAL   The stop price of the order to be submitted
+          --tag TEXT             The tag to be attached to the order
+          --lean-config FILE     The Lean configuration file that should be used (defaults to the nearest lean.json)
+          --verbose              Enable debug logging
+          --help                 Show this message and exit.
+        ```
+        
+        _See code: [lean/commands/live/submit_order.py](https://github.com/QuantConnect/lean-cli/blob/master/lean/commands/live/submit_order.py)_
+        
+        ### `lean live update-order`
+        
+        Represents a command to update a specific order by id.
+        
+        ```
+        Usage: lean live update-order [OPTIONS] PROJECT
+        
+          Represents a command to update a specific order by id.
+        
+        Options:
+          --order-id INTEGER     The order id to be updated  [required]
+          --quantity DECIMAL     The number of units to be updated (directional)
+          --limit-price DECIMAL  The limit price of the order to be updated
+          --stop-price DECIMAL   The stop price of the order to be updated
+          --tag TEXT             The tag to be attached to the order
+          --lean-config FILE     The Lean configuration file that should be used (defaults to the nearest lean.json)
+          --verbose              Enable debug logging
+          --help                 Show this message and exit.
+        ```
+        
+        _See code: [lean/commands/live/update_order.py](https://github.com/QuantConnect/lean-cli/blob/master/lean/commands/live/update_order.py)_
         
         ### `lean login`
         
         Log in with a QuantConnect account.
         
         ```
         Usage: lean login [OPTIONS]
```

### Comparing `lean-1.0.98/lean/container.py` & `lean-1.0.99/lean/container.py`

 * *Files identical despite different names*

### Comparing `lean-1.0.98/lean/commands/whoami.py` & `lean-1.0.99/lean/commands/whoami.py`

 * *Files identical despite different names*

### Comparing `lean-1.0.98/lean/commands/create_project.py` & `lean-1.0.99/lean/commands/create_project.py`

 * *Files identical despite different names*

### Comparing `lean-1.0.98/lean/commands/logout.py` & `lean-1.0.99/lean/commands/logout.py`

 * *Files identical despite different names*

### Comparing `lean-1.0.98/lean/commands/data/download.py` & `lean-1.0.99/lean/commands/data/download.py`

 * *Files identical despite different names*

### Comparing `lean-1.0.98/lean/commands/data/__init__.py` & `lean-1.0.99/lean/commands/data/__init__.py`

 * *Files identical despite different names*

### Comparing `lean-1.0.98/lean/commands/data/generate.py` & `lean-1.0.99/lean/commands/data/generate.py`

 * *Files identical despite different names*

### Comparing `lean-1.0.98/lean/commands/live.py` & `lean-1.0.99/lean/commands/live/deploy.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 from lean.container import container
 from lean.models.brokerages.local import all_local_brokerages, local_brokerage_data_feeds, all_local_data_feeds
 from lean.models.errors import MoreInfoError
 from lean.models.logger import Option
 from lean.models.configuration import Configuration, InfoConfiguration, InternalInputUserInput
 from lean.models.click_options import options_from_json
 from lean.models.json_module import JsonModule
+from lean.commands.live.live import live
 from lean.models.data_providers import all_data_providers
 
 _environment_skeleton = {
     "live-mode": True,
     "setup-handler": "QuantConnect.Lean.Engine.Setup.BrokerageSetupHandler",
     "result-handler": "QuantConnect.Lean.Engine.Results.LiveTradingResultHandler",
     "data-feed-handler": "QuantConnect.Lean.Engine.DataFeeds.LiveTradingDataFeed",
@@ -231,15 +232,15 @@
                     continue
                 else:
                     raise ValueError(f'Options names should be unique. Duplicate key present: {config._id}')
             run_options[config._id] = config
             config_with_module_id[config._id] = module._id
     return list(run_options.values())
 
-@click.command(cls=LeanCommand, requires_lean_config=True, requires_docker=True)
+@live.command(cls=LeanCommand, requires_lean_config=True, requires_docker=True, default_command=True, name="deploy")
 @click.argument("project", type=PathParameter(exists=True, file_okay=True, dir_okay=True))
 @click.option("--environment",
               type=str,
               help="The environment to use")
 @click.option("--output",
               type=PathParameter(exists=False, file_okay=False, dir_okay=True),
               help="Directory to store results in (defaults to PROJECT/live/TIMESTAMP)")
@@ -265,15 +266,15 @@
 @click.option("--image",
               type=str,
               help=f"The LEAN engine image to use (defaults to {DEFAULT_ENGINE_IMAGE})")
 @click.option("--update",
               is_flag=True,
               default=False,
               help="Pull the LEAN engine image before starting live trading")
-def live(project: Path,
+def deploy(project: Path,
         environment: Optional[str],
         output: Optional[Path],
         detach: bool,
         brokerage: Optional[str],
         data_feed: Optional[str],
         data_provider: Optional[str],
         release: bool,
```

### Comparing `lean-1.0.98/lean/commands/library/remove.py` & `lean-1.0.99/lean/commands/library/remove.py`

 * *Files identical despite different names*

### Comparing `lean-1.0.98/lean/commands/library/__init__.py` & `lean-1.0.99/lean/commands/library/__init__.py`

 * *Files identical despite different names*

### Comparing `lean-1.0.98/lean/commands/library/add.py` & `lean-1.0.99/lean/commands/library/add.py`

 * *Files identical despite different names*

### Comparing `lean-1.0.98/lean/commands/init.py` & `lean-1.0.99/lean/commands/init.py`

 * *Files identical despite different names*

### Comparing `lean-1.0.98/lean/commands/cloud/status.py` & `lean-1.0.99/lean/commands/cloud/status.py`

 * *Files identical despite different names*

### Comparing `lean-1.0.98/lean/commands/cloud/live.py` & `lean-1.0.99/lean/commands/cloud/live/deploy.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 from lean.models.api import (QCEmailNotificationMethod, QCNode, QCNotificationMethod, QCSMSNotificationMethod,
                              QCWebhookNotificationMethod, QCProject)
 from lean.models.logger import Option
 from lean.models.brokerages.cloud.cloud_brokerage import CloudBrokerage
 from lean.models.configuration import Configuration, InfoConfiguration, InternalInputUserInput, OrganzationIdConfiguration
 from lean.models.click_options import options_from_json
 from lean.models.brokerages.cloud import all_cloud_brokerages
+from lean.commands.cloud.live.live import live
 
 def _log_notification_methods(methods: List[QCNotificationMethod]) -> None:
     """Logs a list of notification methods."""
     logger = container.logger()
 
     email_methods = [method for method in methods if isinstance(method, QCEmailNotificationMethod)]
     email_methods = "None" if len(email_methods) == 0 else ", ".join(method.address for method in email_methods)
@@ -150,15 +151,15 @@
     for module in all_cloud_brokerages:
         for config in module.get_all_input_configs([InternalInputUserInput, InfoConfiguration]):
             if config._id in run_options:
                 raise ValueError(f'Options names should be unique. Duplicate key present: {config._id}')
             run_options[config._id] = config
     return list(run_options.values())
 
-@click.command(cls=LeanCommand)
+@live.command(cls=LeanCommand, default_command=True, name="deploy")
 @click.argument("project", type=str)
 @click.option("--brokerage",
               type=click.Choice([b.get_name() for b in all_cloud_brokerages], case_sensitive=False),
               help="The brokerage to use")
 @options_from_json(_get_configs_for_options())
 @click.option("--node", type=str, help="The name or id of the live node to run on")
 @click.option("--auto-restart", type=bool, help="Whether automatic algorithm restarting must be enabled")
@@ -175,15 +176,15 @@
               is_flag=True,
               default=False,
               help="Push local modifications to the cloud before starting live trading")
 @click.option("--open", "open_browser",
               is_flag=True,
               default=False,
               help="Automatically open the live results in the browser once the deployment starts")
-def live(project: str,
+def deploy(project: str,
          brokerage: str,
          node: str,
          auto_restart: bool,
          notify_order_events: Optional[bool],
          notify_insights: Optional[bool],
          notify_emails: Optional[str],
          notify_webhooks: Optional[str],
```

### Comparing `lean-1.0.98/lean/commands/cloud/pull.py` & `lean-1.0.99/lean/commands/cloud/pull.py`

 * *Files identical despite different names*

### Comparing `lean-1.0.98/lean/commands/cloud/push.py` & `lean-1.0.99/lean/commands/cloud/push.py`

 * *Files identical despite different names*

### Comparing `lean-1.0.98/lean/commands/cloud/optimize.py` & `lean-1.0.99/lean/commands/cloud/optimize.py`

 * *Files identical despite different names*

### Comparing `lean-1.0.98/lean/commands/cloud/__init__.py` & `lean-1.0.99/lean/commands/cloud/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import click
 
 from lean.commands.cloud.backtest import backtest
-from lean.commands.cloud.live import live
+from lean.commands.cloud.live.live import live
 from lean.commands.cloud.optimize import optimize
 from lean.commands.cloud.pull import pull
 from lean.commands.cloud.push import push
 from lean.commands.cloud.status import status
 
 
 @click.group()
```

### Comparing `lean-1.0.98/lean/commands/cloud/backtest.py` & `lean-1.0.99/lean/commands/cloud/backtest.py`

 * *Files identical despite different names*

### Comparing `lean-1.0.98/lean/commands/config/set.py` & `lean-1.0.99/lean/commands/config/set.py`

 * *Files identical despite different names*

### Comparing `lean-1.0.98/lean/commands/config/__init__.py` & `lean-1.0.99/lean/commands/config/__init__.py`

 * *Files identical despite different names*

### Comparing `lean-1.0.98/lean/commands/config/list.py` & `lean-1.0.99/lean/commands/config/list.py`

 * *Files identical despite different names*

### Comparing `lean-1.0.98/lean/commands/config/unset.py` & `lean-1.0.99/lean/commands/config/unset.py`

 * *Files identical despite different names*

### Comparing `lean-1.0.98/lean/commands/config/get.py` & `lean-1.0.99/lean/commands/config/get.py`

 * *Files identical despite different names*

### Comparing `lean-1.0.98/lean/commands/optimize.py` & `lean-1.0.99/lean/commands/optimize.py`

 * *Files identical despite different names*

### Comparing `lean-1.0.98/lean/commands/logs.py` & `lean-1.0.99/lean/commands/logs.py`

 * *Files identical despite different names*

### Comparing `lean-1.0.98/lean/commands/__init__.py` & `lean-1.0.99/lean/commands/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 from lean.commands.build import build
 from lean.commands.cloud import cloud
 from lean.commands.config import config
 from lean.commands.create_project import create_project
 from lean.commands.data import data
 from lean.commands.init import init
 from lean.commands.library import library
-from lean.commands.live import live
+from lean.commands.live.live import live
 from lean.commands.login import login
 from lean.commands.logout import logout
 from lean.commands.logs import logs
 from lean.commands.optimize import optimize
 from lean.commands.report import report
 from lean.commands.research import research
 from lean.commands.whoami import whoami
@@ -41,20 +41,19 @@
     pass
 
 
 lean.add_command(config)
 lean.add_command(cloud)
 lean.add_command(data)
 lean.add_command(library)
-
+lean.add_command(live)
 lean.add_command(login)
 lean.add_command(logout)
 lean.add_command(whoami)
 lean.add_command(init)
 lean.add_command(create_project)
 lean.add_command(backtest)
 lean.add_command(optimize)
 lean.add_command(research)
 lean.add_command(report)
-lean.add_command(live)
 lean.add_command(build)
 lean.add_command(logs)
```

### Comparing `lean-1.0.98/lean/commands/research.py` & `lean-1.0.99/lean/commands/research.py`

 * *Files identical despite different names*

### Comparing `lean-1.0.98/lean/commands/report.py` & `lean-1.0.99/lean/commands/report.py`

 * *Files identical despite different names*

### Comparing `lean-1.0.98/lean/commands/build.py` & `lean-1.0.99/lean/commands/build.py`

 * *Files identical despite different names*

### Comparing `lean-1.0.98/lean/commands/backtest.py` & `lean-1.0.99/lean/commands/backtest.py`

 * *Files identical despite different names*

### Comparing `lean-1.0.98/lean/commands/login.py` & `lean-1.0.99/lean/commands/login.py`

 * *Files identical despite different names*

### Comparing `lean-1.0.98/lean/models/click_options.py` & `lean-1.0.99/lean/models/click_options.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,16 +8,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-from pathlib import Path
-from typing import Any, Dict, List
+from typing import Any, List
 import click
 from lean.click import PathParameter
 from lean.models.configuration import Configuration
 
 
 def get_click_option_type(configuration: Configuration):
     # get type should be a method of configurations class itself.
@@ -49,32 +48,40 @@
         return configuration.get_input_type()
     elif configuration._input_method == "prompt-password":
         return str
     elif configuration._input_method == "path-parameter":
         return str
 
 
-def get_the_correct_type_default_value(default_lean_config_key: str, default_input_value: str, expected_type: Any):
-    from lean.commands.live import _get_default_value
+def get_the_correct_type_default_value(default_lean_config_key: str, default_input_value: str, expected_type: Any,
+                                       choices: List[str] = None):
+    from lean.commands.live.deploy import _get_default_value
     lean_value = _get_default_value(default_lean_config_key)
     if lean_value is None and default_input_value is not None:
         lean_value = default_input_value
+    # This handles backwards compatibility for the old modules.json values.
     if lean_value is not None and type(lean_value) != expected_type and type(lean_value) == bool:
-        lean_value = "paper" if lean_value else "live"
+        if choices and "true" in choices and "false" in choices:
+            # Backwards compatibility for zeroha-history-subscription.
+            lean_value = "true" if lean_value else "false"
+        else:
+            # Backwards compatibility for tradier-use-sandbox
+            lean_value = "paper" if lean_value else "live"
     return lean_value
 
 
 def get_options_attributes(configuration: Configuration, default_lean_config_key=None):
     options_attributes = {
         "type": get_click_option_type(configuration),
         "help": configuration._help
     }
     default_input_value = configuration._input_default if configuration._is_required_from_user else None
     options_attributes["default"] = lambda: get_the_correct_type_default_value(
-        default_lean_config_key, default_input_value, get_attribute_type(configuration))
+        default_lean_config_key, default_input_value, get_attribute_type(configuration),
+        configuration._choices if configuration._input_method == "choice" else None)
     return options_attributes
 
 
 def get_default_key(configuration: Configuration):
     return "job-organization-id" if configuration.is_type_organization_id else configuration._id
```

### Comparing `lean-1.0.98/lean/models/lean_config_configurer.py` & `lean-1.0.99/lean/models/lean_config_configurer.py`

 * *Files identical despite different names*

### Comparing `lean-1.0.98/lean/models/pydantic.py` & `lean-1.0.99/lean/models/pydantic.py`

 * *Files identical despite different names*

### Comparing `lean-1.0.98/lean/models/data_providers/data_provider.py` & `lean-1.0.99/lean/models/data_providers/data_provider.py`

 * *Files identical despite different names*

### Comparing `lean-1.0.98/lean/models/data_providers/__init__.py` & `lean-1.0.99/lean/models/data_providers/__init__.py`

 * *Files identical despite different names*

### Comparing `lean-1.0.98/lean/models/logger.py` & `lean-1.0.99/lean/models/logger.py`

 * *Files identical despite different names*

### Comparing `lean-1.0.98/lean/models/brokerages/cloud/cloud_brokerage.py` & `lean-1.0.99/lean/models/brokerages/cloud/cloud_brokerage.py`

 * *Files identical despite different names*

### Comparing `lean-1.0.98/lean/models/brokerages/cloud/__init__.py` & `lean-1.0.99/lean/models/brokerages/cloud/__init__.py`

 * *Files identical despite different names*

### Comparing `lean-1.0.98/lean/models/brokerages/local/__init__.py` & `lean-1.0.99/lean/models/brokerages/local/__init__.py`

 * *Files identical despite different names*

### Comparing `lean-1.0.98/lean/models/brokerages/local/local_brokerage.py` & `lean-1.0.99/lean/models/brokerages/local/local_brokerage.py`

 * *Files identical despite different names*

### Comparing `lean-1.0.98/lean/models/brokerages/local/data_feed.py` & `lean-1.0.99/lean/models/brokerages/local/data_feed.py`

 * *Files identical despite different names*

### Comparing `lean-1.0.98/lean/models/brokerages/__init__.py` & `lean-1.0.99/lean/models/brokerages/__init__.py`

 * *Files identical despite different names*

### Comparing `lean-1.0.98/lean/models/options.py` & `lean-1.0.99/lean/models/options.py`

 * *Files identical despite different names*

### Comparing `lean-1.0.98/lean/models/configuration.py` & `lean-1.0.99/lean/models/configuration.py`

 * *Files identical despite different names*

### Comparing `lean-1.0.98/lean/models/__init__.py` & `lean-1.0.99/lean/models/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import os
 import json
 import requests
 from pathlib import Path
 
 json_modules = {}
-file_name = "modules-1.2.json"
+file_name = "modules-1.3.json"
 dirname = os.path.dirname(__file__)
 file_path = os.path.join(dirname, f'../{file_name}')
 
 # check if new file is avaiable online
 url = f"https://cdn.quantconnect.com/cli/{file_name}"
 try:
     res = requests.get(url)
```

### Comparing `lean-1.0.98/lean/models/api.py` & `lean-1.0.99/lean/models/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -274,14 +274,18 @@
     RuntimeError = "RuntimeError"
     Invalid = "Invalid"
     LoggingIn = "LoggingIn"
     Initializing = "Initializing"
     History = "History"
 
 
+class QCRestResponse(WrappedBaseModel):
+    success: bool
+    error: Optional[List[str]]
+
 class QCMinimalLiveAlgorithm(WrappedBaseModel):
     projectId: int
     deployId: str
     status: Optional[QCLiveAlgorithmStatus] = None
 
     def get_url(self) -> str:
         """Returns the url of the live deployment in the cloud.
```

### Comparing `lean-1.0.98/lean/models/docker.py` & `lean-1.0.99/lean/models/docker.py`

 * *Files identical despite different names*

### Comparing `lean-1.0.98/lean/models/modules.py` & `lean-1.0.99/lean/models/modules.py`

 * *Files identical despite different names*

### Comparing `lean-1.0.98/lean/models/data.py` & `lean-1.0.99/lean/models/data.py`

 * *Files identical despite different names*

### Comparing `lean-1.0.98/lean/models/optimizer.py` & `lean-1.0.99/lean/models/optimizer.py`

 * *Files identical despite different names*

### Comparing `lean-1.0.98/lean/models/errors.py` & `lean-1.0.99/lean/models/errors.py`

 * *Files identical despite different names*

### Comparing `lean-1.0.98/lean/models/json_module.py` & `lean-1.0.99/lean/models/json_module.py`

 * *Files identical despite different names*

### Comparing `lean-1.0.98/lean/models/market_hours_database.py` & `lean-1.0.99/lean/models/market_hours_database.py`

 * *Files identical despite different names*

### Comparing `lean-1.0.98/lean/models/utils.py` & `lean-1.0.99/lean/models/utils.py`

 * *Files identical despite different names*

### Comparing `lean-1.0.98/lean/main.py` & `lean-1.0.99/lean/main.py`

 * *Files identical despite different names*

### Comparing `lean-1.0.98/lean/__init__.py` & `lean-1.0.99/lean/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 # The version is always set to "dev" in the Git repository. When a new release is ready,
 # a maintainer will push a new Git tag which will trigger GitHub Actions to publish a new
 # package to PyPI with the version of the tag.
-__version__ = "1.0.98"
+__version__ = "1.0.99"
```

### Comparing `lean-1.0.98/lean/ssh/key` & `lean-1.0.99/lean/ssh/key`

 * *Files identical despite different names*

### Comparing `lean-1.0.98/lean/components/api/market_client.py` & `lean-1.0.99/lean/components/api/market_client.py`

 * *Files identical despite different names*

### Comparing `lean-1.0.98/lean/components/api/service_client.py` & `lean-1.0.99/lean/components/api/service_client.py`

 * *Files identical despite different names*

### Comparing `lean-1.0.98/lean/components/api/backtest_client.py` & `lean-1.0.99/lean/components/api/backtest_client.py`

 * *Files identical despite different names*

### Comparing `lean-1.0.98/lean/components/api/api_client.py` & `lean-1.0.99/lean/components/api/api_client.py`

 * *Files identical despite different names*

### Comparing `lean-1.0.98/lean/components/api/file_client.py` & `lean-1.0.99/lean/components/api/file_client.py`

 * *Files identical despite different names*

### Comparing `lean-1.0.98/lean/components/api/module_client.py` & `lean-1.0.99/lean/components/api/module_client.py`

 * *Files identical despite different names*

### Comparing `lean-1.0.98/lean/components/api/project_client.py` & `lean-1.0.99/lean/components/api/project_client.py`

 * *Files identical despite different names*

### Comparing `lean-1.0.98/lean/components/api/user_client.py` & `lean-1.0.99/lean/components/api/user_client.py`

 * *Files identical despite different names*

### Comparing `lean-1.0.98/lean/components/api/account_client.py` & `lean-1.0.99/lean/components/api/account_client.py`

 * *Files identical despite different names*

### Comparing `lean-1.0.98/lean/components/api/__init__.py` & `lean-1.0.99/lean/components/api/__init__.py`

 * *Files identical despite different names*

### Comparing `lean-1.0.98/lean/components/api/organization_client.py` & `lean-1.0.99/lean/components/api/organization_client.py`

 * *Files identical despite different names*

### Comparing `lean-1.0.98/lean/components/api/node_client.py` & `lean-1.0.99/lean/components/api/node_client.py`

 * *Files identical despite different names*

### Comparing `lean-1.0.98/lean/components/api/data_client.py` & `lean-1.0.99/lean/components/api/data_client.py`

 * *Files identical despite different names*

### Comparing `lean-1.0.98/lean/components/api/optimization_client.py` & `lean-1.0.99/lean/components/api/optimization_client.py`

 * *Files identical despite different names*

### Comparing `lean-1.0.98/lean/components/api/compile_client.py` & `lean-1.0.99/lean/components/api/compile_client.py`

 * *Files identical despite different names*

### Comparing `lean-1.0.98/lean/components/api/live_client.py` & `lean-1.0.99/lean/components/api/live_client.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # limitations under the License.
 
 from datetime import datetime
 from math import floor
 from typing import List, Optional
 
 from lean.components.api.api_client import *
-from lean.models.api import QCFullLiveAlgorithm, QCLiveAlgorithmStatus, QCMinimalLiveAlgorithm, QCNotificationMethod
+from lean.models.api import QCFullLiveAlgorithm, QCLiveAlgorithmStatus, QCMinimalLiveAlgorithm, QCNotificationMethod, QCRestResponse
 
 
 class LiveClient:
     """The LiveClient class contains methods to interact with live/* API endpoints."""
 
     def __init__(self, api_client: 'APIClient') -> None:
         """Creates a new LiveClient instance.
@@ -99,24 +99,26 @@
                 "events": events,
                 "targets": [method.dict() for method in notify_methods]
             }
 
         data = self._api.post("live/create", parameters)
         return QCMinimalLiveAlgorithm(**data)
 
-    def stop(self, project_id: int) -> None:
+    def stop(self, project_id: int) -> QCRestResponse:
         """Stops live trading for a certain project without liquidated existing positions.
 
         :param project_id: the id of the project to stop live trading for
         """
-        self._api.post("live/update/stop", {
+        data = self._api.post("live/update/stop", {
             "projectId": project_id
         })
+        return QCRestResponse(**data)
 
-    def liquidate_and_stop(self, project_id: int) -> None:
+    def liquidate_and_stop(self, project_id: int) -> QCRestResponse:
         """Stops live trading and liquidates existing positions for a certain project.
 
         :param project_id: the id of the project to stop live trading and liquidate existing positions for
         """
-        self._api.post("live/update/liquidate", {
+        data = self._api.post("live/update/liquidate", {
             "projectId": project_id
         })
+        return QCRestResponse(**data)
```

### Comparing `lean-1.0.98/lean/components/cloud/pull_manager.py` & `lean-1.0.99/lean/components/cloud/pull_manager.py`

 * *Files identical despite different names*

### Comparing `lean-1.0.98/lean/components/cloud/cloud_runner.py` & `lean-1.0.99/lean/components/cloud/cloud_runner.py`

 * *Files identical despite different names*

### Comparing `lean-1.0.98/lean/components/cloud/cloud_project_manager.py` & `lean-1.0.99/lean/components/cloud/cloud_project_manager.py`

 * *Files identical despite different names*

### Comparing `lean-1.0.98/lean/components/cloud/push_manager.py` & `lean-1.0.99/lean/components/cloud/push_manager.py`

 * *Files identical despite different names*

### Comparing `lean-1.0.98/lean/components/cloud/data_downloader.py` & `lean-1.0.99/lean/components/cloud/data_downloader.py`

 * *Files identical despite different names*

### Comparing `lean-1.0.98/lean/components/cloud/__init__.py` & `lean-1.0.99/lean/components/cloud/__init__.py`

 * *Files identical despite different names*

### Comparing `lean-1.0.98/lean/components/cloud/module_manager.py` & `lean-1.0.99/lean/components/cloud/module_manager.py`

 * *Files identical despite different names*

### Comparing `lean-1.0.98/lean/components/docker/lean_runner.py` & `lean-1.0.99/lean/components/docker/lean_runner.py`

 * *Files identical despite different names*

### Comparing `lean-1.0.98/lean/components/docker/__init__.py` & `lean-1.0.99/lean/components/docker/__init__.py`

 * *Files identical despite different names*

### Comparing `lean-1.0.98/lean/components/docker/docker_manager.py` & `lean-1.0.99/lean/components/docker/docker_manager.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,18 +16,19 @@
 import os
 import platform
 import shutil
 import signal
 import subprocess
 import sys
 import threading
+import time
 import types
 from pathlib import Path
-from typing import Optional, Set
-
+from typing import Optional, Set, Any, Dict
+from subprocess import Popen, PIPE
 import docker
 from dateutil.parser import isoparse
 from docker.errors import APIError
 from docker.models.containers import Container
 from docker.types import Mount
 
 from lean.components.util.logger import Logger
@@ -420,14 +421,86 @@
         """
         try:
             docker.from_env()
         except Exception as exception:
             return "Permission denied" in str(exception)
         return False
 
+    def write_to_file(self, docker_container_name: str, docker_file: Path, data: Dict[str, Any]) -> None:        
+        """Write data to the file in docker.
+
+        Args:
+            docker_container_name: The name of the container to write to
+            docker_file: The Dockerfile to write to.
+            data: The data to write to the Dockerfile.
+        """
+        docker_container = self.get_container_by_name(docker_container_name)
+        if docker_container is None:
+            raise ValueError(f"Container {docker_container_name} does not exist")
+        if docker_container.status != "running":
+            raise ValueError(f"Container {docker_container_name} is not running")
+            
+        data = json.dumps(data)
+        data = data.replace('"','\\"')
+        command = f'docker exec {docker_container_name} bash -c "echo \'{data}\' > {docker_file.as_posix()}"'
+        try:
+            subprocess.run(command, shell=True, check=True)
+        except subprocess.CalledProcessError as exception:
+            raise ValueError(f"Failed to write to {docker_file.name}: {exception.output.decode('utf-8')}")
+        except Exception as e:
+            raise ValueError(f"Failed to write to {docker_file.name}: {e}")
+    
+    def read_from_file(self, docker_container_name: str, docker_file: Path, interval=1, timeout=30) -> Dict[str,Any]:
+        """Read data from file in docker.
+
+        Args:
+            docker_container_name: The name of the container to write to
+            docker_file: The Dockerfile to write to.
+            interval: The interval to sleep before checking again.
+            timeout: The timeout to wait for the file.
+        """
+        command = f'docker exec {docker_container_name} bash -c "cat {docker_file.as_posix()}"'
+        start = time.time()
+        success = False
+        error_message = None
+        container_running = True
+        while time.time() - start < timeout:
+            try:
+                docker_container = self.get_container_by_name(docker_container_name)
+                if docker_container is None:
+                    error_message = f"Container {docker_container_name} does not exist"
+                    container_running = False
+                    break
+                p = Popen(command, shell=True, stdin=PIPE, stdout=PIPE, stderr=PIPE)
+                output = p.stdout.read().decode('utf-8')
+                if output is not None and output != "":
+                    success = True
+                    break
+            except subprocess.CalledProcessError as exception:
+                error_message = f"Failed to read result from docker file {docker_file.name}: {exception.output.decode('utf-8')} {p.stderr.read().decode('utf-8')}"
+                time.sleep(interval)
+            except Exception as e:
+                error_message = f"Failed to read result from docker file {docker_file.name}: {e} {p.stderr.read().decode('utf-8')}"
+                time.sleep(interval)
+
+        if success:
+            result = json.loads(output)
+            success = result["Success"]
+            if not success:
+                error_message = "Rejected by Lean. Possible arguments error. Please check your logs and try again."
+        if not success and not error_message:
+            error_message = f"Failed to read result from docker file {docker_file.name} within {timeout} seconds"
+        
+        return {
+            "error": error_message,
+            "success": success,
+            "container-running": container_running
+        }
+
+
     def _get_docker_client(self) -> docker.DockerClient:
         """Creates a DockerClient instance.
 
         Raises an error if Docker is not running.
 
         :return: a DockerClient instance which responds to requests
         """
```

### Comparing `lean-1.0.98/lean/components/config/cli_config_manager.py` & `lean-1.0.99/lean/components/config/cli_config_manager.py`

 * *Files identical despite different names*

### Comparing `lean-1.0.98/lean/components/config/lean_config_manager.py` & `lean-1.0.99/lean/components/config/lean_config_manager.py`

 * *Files identical despite different names*

### Comparing `lean-1.0.98/lean/components/config/storage.py` & `lean-1.0.99/lean/components/config/storage.py`

 * *Files identical despite different names*

### Comparing `lean-1.0.98/lean/components/config/output_config_manager.py` & `lean-1.0.99/lean/components/config/output_config_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,28 +41,28 @@
         """Returns the id of a backtest.
 
         :param backtest_directory: the path to the backtest to retrieve the id of
         :return: the id of the given backtest
         """
         return self._get_id(backtest_directory, 1)
 
-    def get_backtest_name(self, backtest_directory: Path) -> int:
+    def get_backtest_name(self, backtest_directory: Path) -> str:
         """Returns the name of a backtest.
 
         :param backtest_directory: the path to the backtest to retrieve the id of
         :return: the name of the given backtest
         """
         config = self.get_output_config(backtest_directory)
 
         if config.has("backtest-name"):
             return config.get("backtest-name")
 
         raise ValueError("Backtest name is not set")
 
-    def get_container_name(self, backtest_directory: Path) -> int:
+    def get_container_name(self, backtest_directory: Path) -> str:
         """Returns the name of a the docker container lean is running in.
 
         :param backtest_directory: the path to the backtest to retrieve the id of
         :return: the name of the docker container lean is running in.
         """
         config = self.get_output_config(backtest_directory)
```

### Comparing `lean-1.0.98/lean/components/config/optimizer_config_manager.py` & `lean-1.0.99/lean/components/config/optimizer_config_manager.py`

 * *Files identical despite different names*

### Comparing `lean-1.0.98/lean/components/config/__init__.py` & `lean-1.0.99/lean/components/config/__init__.py`

 * *Files identical despite different names*

### Comparing `lean-1.0.98/lean/components/config/project_config_manager.py` & `lean-1.0.99/lean/components/config/project_config_manager.py`

 * *Files 17% similar despite different names*

```diff
@@ -53,14 +53,32 @@
             return project_config.get("local-id")
 
         project_id = random.randint(100_000_000, 999_999_999)
         project_config.set("local-id", project_id)
 
         return project_id
 
+    def get_latest_live_directory(self, project_directory: Path) -> Path:
+        """Returns the path of the latest live directory.
+
+        :param project_directory: the path to the project to retrieve the local id of
+        :return: the path of the latest live directory
+        """
+        live_root_dir = project_directory / "live"
+        if not live_root_dir.is_dir():
+            raise ValueError(f"live directory {live_root_dir} is not a directory")
+
+        for live_dir in sorted(list(live_root_dir.iterdir()), reverse=True):
+            if not (live_dir / "log.txt").is_file():
+                continue
+            return live_dir
+        
+        raise ValueError("live directory with log.txt not found")
+
+        
     def get_csharp_libraries(self, project_directory: Path) -> List[CSharpLibrary]:
         """Returns the custom C# libraries in a project.
 
         :param project_directory: the path to the project to retrieve the C# libraries of
         :return: a list containing the information of all PackageReferences in the project's .csproj file, if any
         """
         csproj_file = next((p for p in project_directory.iterdir() if p.name.endswith(".csproj")), None)
```

### Comparing `lean-1.0.98/lean/components/__init__.py` & `lean-1.0.99/lean/components/__init__.py`

 * *Files identical despite different names*

### Comparing `lean-1.0.98/lean/components/util/http_client.py` & `lean-1.0.99/lean/components/util/http_client.py`

 * *Files identical despite different names*

### Comparing `lean-1.0.98/lean/components/util/path_manager.py` & `lean-1.0.99/lean/components/util/path_manager.py`

 * *Files identical despite different names*

### Comparing `lean-1.0.98/lean/components/util/logger.py` & `lean-1.0.99/lean/components/util/logger.py`

 * *Files identical despite different names*

### Comparing `lean-1.0.98/lean/components/util/compiler.py` & `lean-1.0.99/lean/components/util/compiler.py`

 * *Files identical despite different names*

### Comparing `lean-1.0.98/lean/components/util/platform_manager.py` & `lean-1.0.99/lean/components/util/platform_manager.py`

 * *Files identical despite different names*

### Comparing `lean-1.0.98/lean/components/util/task_manager.py` & `lean-1.0.99/lean/components/util/task_manager.py`

 * *Files identical despite different names*

### Comparing `lean-1.0.98/lean/components/util/__init__.py` & `lean-1.0.99/lean/components/util/__init__.py`

 * *Files identical despite different names*

### Comparing `lean-1.0.98/lean/components/util/project_manager.py` & `lean-1.0.99/lean/components/util/project_manager.py`

 * *Files identical despite different names*

### Comparing `lean-1.0.98/lean/components/util/xml_manager.py` & `lean-1.0.99/lean/components/util/xml_manager.py`

 * *Files identical despite different names*

### Comparing `lean-1.0.98/lean/components/util/update_manager.py` & `lean-1.0.99/lean/components/util/update_manager.py`

 * *Files identical despite different names*

### Comparing `lean-1.0.98/lean/components/util/temp_manager.py` & `lean-1.0.99/lean/components/util/temp_manager.py`

 * *Files identical despite different names*

### Comparing `lean-1.0.98/lean/components/util/name_extraction.py` & `lean-1.0.99/lean/components/util/name_extraction.py`

 * *Files identical despite different names*

### Comparing `lean-1.0.98/lean/components/util/name_generator.py` & `lean-1.0.99/lean/components/util/name_generator.py`

 * *Files identical despite different names*

### Comparing `lean-1.0.98/lean/components/util/market_hours_database.py` & `lean-1.0.99/lean/components/util/market_hours_database.py`

 * *Files identical despite different names*

### Comparing `lean-1.0.98/lean/click.py` & `lean-1.0.99/lean/click.py`

 * *Files identical despite different names*

### Comparing `lean-1.0.98/lean/constants.py` & `lean-1.0.99/lean/constants.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import os
-from datetime import datetime, timezone
 from pathlib import Path
 
 # Due to the way the filesystem is mocked in unit tests, values should not be Path instances.
 
 # The file in which general CLI configuration is stored
 GENERAL_CONFIG_PATH = str(Path("~/.lean/config").expanduser())
 
@@ -25,14 +24,20 @@
 
 # The file in which we store when we last checked for updates
 CACHE_PATH = str(Path("~/.lean/cache").expanduser())
 
 # The directory in which modules are stored
 MODULES_DIRECTORY = str(Path("~/.lean/modules").expanduser())
 
+# The file in which we send live commands to running docker container
+COMMAND_FILE_BASENAME = "command"
+
+# The file from which we read results of the command sent to the docker container
+COMMAND_RESULT_FILE_BASENAME = "result-command"
+
 # The default name of the file containing the Lean engine configuration
 DEFAULT_LEAN_CONFIG_FILE_NAME = "lean.json"
 
 # The default name of the directory containing the market data
 DEFAULT_DATA_DIRECTORY_NAME = "data"
 
 # The name of the file in containing the project configuration
```

### Comparing `lean-1.0.98/setup.py` & `lean-1.0.99/setup.py`

 * *Files identical despite different names*

### Comparing `lean-1.0.98/README.md` & `lean-1.0.99/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -68,14 +68,17 @@
 *Note: the readme only contains the `--help` text of all commands. Visit the [documentation website](https://www.lean.io/docs/lean-cli/key-concepts/getting-started) for more comprehensive documentation.*
 
 <!-- commands start -->
 - [`lean backtest`](#lean-backtest)
 - [`lean build`](#lean-build)
 - [`lean cloud backtest`](#lean-cloud-backtest)
 - [`lean cloud live`](#lean-cloud-live)
+- [`lean cloud live deploy`](#lean-cloud-live-deploy)
+- [`lean cloud live liquidate`](#lean-cloud-live-liquidate)
+- [`lean cloud live stop`](#lean-cloud-live-stop)
 - [`lean cloud optimize`](#lean-cloud-optimize)
 - [`lean cloud pull`](#lean-cloud-pull)
 - [`lean cloud push`](#lean-cloud-push)
 - [`lean cloud status`](#lean-cloud-status)
 - [`lean config get`](#lean-config-get)
 - [`lean config list`](#lean-config-list)
 - [`lean config set`](#lean-config-set)
@@ -83,14 +86,21 @@
 - [`lean create-project`](#lean-create-project)
 - [`lean data download`](#lean-data-download)
 - [`lean data generate`](#lean-data-generate)
 - [`lean init`](#lean-init)
 - [`lean library add`](#lean-library-add)
 - [`lean library remove`](#lean-library-remove)
 - [`lean live`](#lean-live)
+- [`lean live add-security`](#lean-live-add-security)
+- [`lean live cancel-order`](#lean-live-cancel-order)
+- [`lean live deploy`](#lean-live-deploy)
+- [`lean live liquidate`](#lean-live-liquidate)
+- [`lean live stop`](#lean-live-stop)
+- [`lean live submit-order`](#lean-live-submit-order)
+- [`lean live update-order`](#lean-live-update-order)
 - [`lean login`](#lean-login)
 - [`lean logout`](#lean-logout)
 - [`lean logs`](#lean-logs)
 - [`lean optimize`](#lean-optimize)
 - [`lean report`](#lean-report)
 - [`lean research`](#lean-research)
 - [`lean whoami`](#lean-whoami)
@@ -191,18 +201,38 @@
   --help       Show this message and exit.
 ```
 
 _See code: [lean/commands/cloud/backtest.py](lean/commands/cloud/backtest.py)_
 
 ### `lean cloud live`
 
+Interact with the QuantConnect cloud live deployments.
+
+```
+Usage: lean cloud live [OPTIONS] COMMAND [ARGS]...
+
+  Interact with the QuantConnect cloud live deployments.
+
+Options:
+  --help  Show this message and exit.
+
+Commands:
+  deploy     Start live trading for a project in the cloud.
+  liquidate  Stops live trading and liquidates existing positions for a certain project.
+  stop       Stops live trading for a certain project without liquidating existing positions.
+```
+
+_See code: [lean/commands/cloud/live.py](lean/commands/cloud/live.py)_
+
+### `lean cloud live deploy`
+
 Start live trading for a project in the cloud.
 
 ```
-Usage: lean cloud live [OPTIONS] PROJECT
+Usage: lean cloud live deploy [OPTIONS] PROJECT
 
   Start live trading for a project in the cloud.
 
   PROJECT must be the name or the id of the project to start live trading for.
 
   By default an interactive wizard is shown letting you configure the deployment. If --brokerage is given the command
   runs in non-interactive mode. In this mode the CLI does not prompt for input or confirmation. In non-interactive mode
@@ -238,27 +268,29 @@
                                   Whether the testnet should be used
   --binance-api-key TEXT          Your Binance API key
   --binanceus-api-key TEXT        Your Binance API key
   --binance-api-secret TEXT       Your Binance API secret
   --binanceus-api-secret TEXT     Your Binance API secret
   --zerodha-api-key TEXT          Your Kite Connect API key
   --zerodha-access-token TEXT     Your Kite Connect access token
-  --zerodha-product-type [MIS|CNC|NRML]
+  --zerodha-product-type [mis|cnc|nrml]
                                   MIS if you are targeting intraday products, CNC if you are targeting delivery
                                   products, NRML if you are targeting carry forward products
-  --zerodha-trading-segment [EQUITY|COMMODITY]
+  --zerodha-trading-segment [equity|commodity]
                                   EQUITY if you are trading equities on NSE or BSE, COMMODITY if you are trading
                                   commodities on MCX
+  --zerodha-history-subscription [true|false]
+                                  Whether you have a history API subscription for Zerodha
   --samco-client-id TEXT          Your Samco account Client ID
   --samco-client-password TEXT    Your Samco account password
   --samco-year-of-birth TEXT      Your year of birth (YYYY) registered with Samco
-  --samco-product-type [MIS|CNC|NRML]
+  --samco-product-type [mis|cnc|nrml]
                                   MIS if you are targeting intraday products, CNC if you are targeting delivery
                                   products, NRML if you are targeting carry forward products
-  --samco-trading-segment [EQUITY|COMMODITY]
+  --samco-trading-segment [equity|commodity]
                                   EQUITY if you are trading equities on NSE or BSE, COMMODITY if you are trading
                                   commodities on MCX
   --kraken-api-key TEXT           Your Kraken API key
   --kraken-api-secret TEXT        Your Kraken API secret
   --kraken-verification-tier [Starter|Intermediate|Pro]
                                   Your Kraken Verification Tier
   --ftx-exchange-name [FTX|FTXUS]
@@ -281,15 +313,47 @@
   --notify-sms TEXT               A comma-separated list of phone numbers configuring SMS-notifications
   --push                          Push local modifications to the cloud before starting live trading
   --open                          Automatically open the live results in the browser once the deployment starts
   --verbose                       Enable debug logging
   --help                          Show this message and exit.
 ```
 
-_See code: [lean/commands/cloud/live.py](lean/commands/cloud/live.py)_
+_See code: [lean/commands/cloud/live/deploy.py](lean/commands/cloud/live/deploy.py)_
+
+### `lean cloud live liquidate`
+
+Stops live trading and liquidates existing positions for a certain project.
+
+```
+Usage: lean cloud live liquidate [OPTIONS] PROJECT
+
+  Stops live trading and liquidates existing positions for a certain project.
+
+Options:
+  --verbose  Enable debug logging
+  --help     Show this message and exit.
+```
+
+_See code: [lean/commands/cloud/live/liquidate.py](lean/commands/cloud/live/liquidate.py)_
+
+### `lean cloud live stop`
+
+Stops live trading for a certain project without liquidating existing positions.
+
+```
+Usage: lean cloud live stop [OPTIONS] PROJECT
+
+  Stops live trading for a certain project without liquidating existing positions.
+
+Options:
+  --verbose  Enable debug logging
+  --help     Show this message and exit.
+```
+
+_See code: [lean/commands/cloud/live/stop.py](lean/commands/cloud/live/stop.py)_
 
 ### `lean cloud optimize`
 
 Optimize a project in the cloud.
 
 ```
 Usage: lean cloud optimize [OPTIONS] PROJECT
@@ -655,18 +719,86 @@
   --help      Show this message and exit.
 ```
 
 _See code: [lean/commands/library/remove.py](lean/commands/library/remove.py)_
 
 ### `lean live`
 
+Interact with the local machine.
+
+```
+Usage: lean live [OPTIONS] COMMAND [ARGS]...
+
+  Interact with the local machine.
+
+Options:
+  --help  Show this message and exit.
+
+Commands:
+  add-security  Represents a command to add a security to the algorithm.
+  cancel-order  Represents a command to cancel a specific order by id.
+  deploy        Start live trading a project locally using Docker.
+  liquidate     Liquidate the given symbol from the latest deployment of the given project.
+  stop          Stop an already running local live trading project.
+  submit-order  Represents a command to submit an order to the algorithm.
+  update-order  Represents a command to update a specific order by id.
+```
+
+_See code: [lean/commands/live.py](lean/commands/live.py)_
+
+### `lean live add-security`
+
+Represents a command to add a security to the algorithm.
+
+```
+Usage: lean live add-security [OPTIONS] PROJECT
+
+  Represents a command to add a security to the algorithm.
+
+Options:
+  --ticker TEXT            The ticker of the symbol to add  [required]
+  --market TEXT            The market of the symbol to add  [required]
+  --security-type TEXT     The security type of the symbol to add  [required]
+  --resolution TEXT        The resolution of the symbol to add
+  --fill-data-forward      The fill forward behavior, true to fill forward, false otherwise - defaults to true
+  --leverage DECIMAL       The leverage for the security, defaults to 2 for equity, 50 for forex, and 1 for everything
+                           else
+  --extended-market-hours  The extended market hours flag, true to allow pre/post market data, false for only in market
+                           data
+  --lean-config FILE       The Lean configuration file that should be used (defaults to the nearest lean.json)
+  --verbose                Enable debug logging
+  --help                   Show this message and exit.
+```
+
+_See code: [lean/commands/live/add_security.py](lean/commands/live/add_security.py)_
+
+### `lean live cancel-order`
+
+Represents a command to cancel a specific order by id.
+
+```
+Usage: lean live cancel-order [OPTIONS] PROJECT
+
+  Represents a command to cancel a specific order by id.
+
+Options:
+  --order-id INTEGER  The order id to be cancelled  [required]
+  --lean-config FILE  The Lean configuration file that should be used (defaults to the nearest lean.json)
+  --verbose           Enable debug logging
+  --help              Show this message and exit.
+```
+
+_See code: [lean/commands/live/cancel_order.py](lean/commands/live/cancel_order.py)_
+
+### `lean live deploy`
+
 Start live trading a project locally using Docker.
 
 ```
-Usage: lean live [OPTIONS] PROJECT
+Usage: lean live deploy [OPTIONS] PROJECT
 
   Start live trading a project locally using Docker.
 
   If PROJECT is a directory, the algorithm in the main.py or Main.cs file inside it will be executed.
   If PROJECT is a file, the algorithm in the specified file will be executed.
 
   By default an interactive wizard is shown letting you configure the brokerage and data feed to use. If --environment,
@@ -726,30 +858,30 @@
   --binance-api-key TEXT          Your Binance API key
   --binanceus-api-key TEXT        Your Binance API key
   --binance-api-secret TEXT       Your Binance API secret
   --binanceus-api-secret TEXT     Your Binance API secret
   --zerodha-organization TEXT     The name or id of the organization with the zerodha module subscription
   --zerodha-api-key TEXT          Your Kite Connect API key
   --zerodha-access-token TEXT     Your Kite Connect access token
-  --zerodha-product-type [MIS|CNC|NRML]
+  --zerodha-product-type [mis|cnc|nrml]
                                   MIS if you are targeting intraday products, CNC if you are targeting delivery
                                   products, NRML if you are targeting carry forward products
-  --zerodha-trading-segment [EQUITY|COMMODITY]
+  --zerodha-trading-segment [equity|commodity]
                                   EQUITY if you are trading equities on NSE or BSE, COMMODITY if you are trading
                                   commodities on MCX
-  --zerodha-history-subscription BOOLEAN
+  --zerodha-history-subscription [true|false]
                                   Whether you have a history API subscription for Zerodha
   --samco-organization TEXT       The name or id of the organization with the samco module subscription
   --samco-client-id TEXT          Your Samco account Client ID
   --samco-client-password TEXT    Your Samco account password
   --samco-year-of-birth TEXT      Your year of birth (YYYY) registered with Samco
-  --samco-product-type [MIS|CNC|NRML]
+  --samco-product-type [mis|cnc|nrml]
                                   MIS if you are targeting intraday products, CNC if you are targeting delivery
                                   products, NRML if you are targeting carry forward products
-  --samco-trading-segment [EQUITY|COMMODITY]
+  --samco-trading-segment [equity|commodity]
                                   EQUITY if you are trading equities on NSE or BSE, COMMODITY if you are trading
                                   commodities on MCX
   --terminal-link-organization TEXT
                                   The name or id of the organization with the Terminal Link module subscription
   --bloomberg-environment [Production|Beta]
                                   The environment to run in
   --bloomberg-server-host TEXT    The host of the Bloomberg server
@@ -823,15 +955,99 @@
   --image TEXT                    The LEAN engine image to use (defaults to quantconnect/lean:latest)
   --update                        Pull the LEAN engine image before starting live trading
   --lean-config FILE              The Lean configuration file that should be used (defaults to the nearest lean.json)
   --verbose                       Enable debug logging
   --help                          Show this message and exit.
 ```
 
-_See code: [lean/commands/live.py](lean/commands/live.py)_
+_See code: [lean/commands/live/deploy.py](lean/commands/live/deploy.py)_
+
+### `lean live liquidate`
+
+Liquidate the given symbol from the latest deployment of the given project.
+
+```
+Usage: lean live liquidate [OPTIONS] PROJECT
+
+  Liquidate the given symbol from the latest deployment of the given project.
+
+Options:
+  --ticker TEXT         The ticker of the symbol to liquidate
+  --market TEXT         The market of the symbol to liquidate
+  --security-type TEXT  The security type of the symbol to liquidate
+  --lean-config FILE    The Lean configuration file that should be used (defaults to the nearest lean.json)
+  --verbose             Enable debug logging
+  --help                Show this message and exit.
+```
+
+_See code: [lean/commands/live/liquidate.py](lean/commands/live/liquidate.py)_
+
+### `lean live stop`
+
+Stop an already running local live trading project.
+
+```
+Usage: lean live stop [OPTIONS] PROJECT
+
+  Stop an already running local live trading project.
+
+Options:
+  --lean-config FILE  The Lean configuration file that should be used (defaults to the nearest lean.json)
+  --verbose           Enable debug logging
+  --help              Show this message and exit.
+```
+
+_See code: [lean/commands/live/stop.py](lean/commands/live/stop.py)_
+
+### `lean live submit-order`
+
+Represents a command to submit an order to the algorithm.
+
+```
+Usage: lean live submit-order [OPTIONS] PROJECT
+
+  Represents a command to submit an order to the algorithm.
+
+Options:
+  --ticker TEXT          The ticker of the symbol to be submitted  [required]
+  --market TEXT          The market of the symbol to be submitted  [required]
+  --security-type TEXT   The security type of the symbol to be submitted  [required]
+  --order-type TEXT      The order type to be submitted  [required]
+  --quantity DECIMAL     The number of units to be ordered (directional)  [required]
+  --limit-price DECIMAL  The limit price of the order be submitted
+  --stop-price DECIMAL   The stop price of the order to be submitted
+  --tag TEXT             The tag to be attached to the order
+  --lean-config FILE     The Lean configuration file that should be used (defaults to the nearest lean.json)
+  --verbose              Enable debug logging
+  --help                 Show this message and exit.
+```
+
+_See code: [lean/commands/live/submit_order.py](lean/commands/live/submit_order.py)_
+
+### `lean live update-order`
+
+Represents a command to update a specific order by id.
+
+```
+Usage: lean live update-order [OPTIONS] PROJECT
+
+  Represents a command to update a specific order by id.
+
+Options:
+  --order-id INTEGER     The order id to be updated  [required]
+  --quantity DECIMAL     The number of units to be updated (directional)
+  --limit-price DECIMAL  The limit price of the order to be updated
+  --stop-price DECIMAL   The stop price of the order to be updated
+  --tag TEXT             The tag to be attached to the order
+  --lean-config FILE     The Lean configuration file that should be used (defaults to the nearest lean.json)
+  --verbose              Enable debug logging
+  --help                 Show this message and exit.
+```
+
+_See code: [lean/commands/live/update_order.py](lean/commands/live/update_order.py)_
 
 ### `lean login`
 
 Log in with a QuantConnect account.
 
 ```
 Usage: lean login [OPTIONS]
```

