# Comparing `tmp/apache-dolphinscheduler-4.0.2a9.tar.gz` & `tmp/apache-dolphinscheduler-4.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-dolphinscheduler-4.0.2a9.tar", last modified: Thu Jul 13 01:58:59 2023, max compression
+gzip compressed data, was "apache-dolphinscheduler-4.0.3.tar", last modified: Fri Apr 14 05:54:06 2023, max compression
```

## Comparing `apache-dolphinscheduler-4.0.2a9.tar` & `apache-dolphinscheduler-4.0.3.tar`

### file list

```diff
@@ -1,124 +1,119 @@
-drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-07-13 01:58:59.198837 apache-dolphinscheduler-4.0.2a9/
--rw-r--r--   0 zhongjiajie   (501) staff       (20)    12843 2023-07-05 10:40:26.000000 apache-dolphinscheduler-4.0.2a9/CONTRIBUTING.md
--rw-r--r--   0 zhongjiajie   (501) staff       (20)    12553 2022-12-14 07:25:00.000000 apache-dolphinscheduler-4.0.2a9/LICENSE
--rw-r--r--   0 zhongjiajie   (501) staff       (20)      177 2022-12-14 07:25:00.000000 apache-dolphinscheduler-4.0.2a9/NOTICE
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     7853 2023-07-13 01:58:59.198932 apache-dolphinscheduler-4.0.2a9/PKG-INFO
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     6015 2023-04-04 15:19:49.000000 apache-dolphinscheduler-4.0.2a9/README.md
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     9814 2023-07-05 10:40:26.000000 apache-dolphinscheduler-4.0.2a9/RELEASE.md
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     2832 2023-04-04 15:19:49.000000 apache-dolphinscheduler-4.0.2a9/UPDATING.md
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     2635 2023-07-13 01:58:59.199406 apache-dolphinscheduler-4.0.2a9/setup.cfg
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     3027 2023-07-05 08:11:55.000000 apache-dolphinscheduler-4.0.2a9/setup.py
-drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-07-13 01:58:59.173219 apache-dolphinscheduler-4.0.2a9/src/
-drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-07-13 01:58:59.176690 apache-dolphinscheduler-4.0.2a9/src/apache_dolphinscheduler.egg-info/
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     7853 2023-07-13 01:58:59.000000 apache-dolphinscheduler-4.0.2a9/src/apache_dolphinscheduler.egg-info/PKG-INFO
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     4672 2023-07-13 01:58:59.000000 apache-dolphinscheduler-4.0.2a9/src/apache_dolphinscheduler.egg-info/SOURCES.txt
--rw-r--r--   0 zhongjiajie   (501) staff       (20)        1 2023-07-13 01:58:59.000000 apache-dolphinscheduler-4.0.2a9/src/apache_dolphinscheduler.egg-info/dependency_links.txt
--rw-r--r--   0 zhongjiajie   (501) staff       (20)       75 2023-07-13 01:58:59.000000 apache-dolphinscheduler-4.0.2a9/src/apache_dolphinscheduler.egg-info/entry_points.txt
--rw-r--r--   0 zhongjiajie   (501) staff       (20)      577 2023-07-13 01:58:59.000000 apache-dolphinscheduler-4.0.2a9/src/apache_dolphinscheduler.egg-info/requires.txt
--rw-r--r--   0 zhongjiajie   (501) staff       (20)       19 2023-07-13 01:58:59.000000 apache-dolphinscheduler-4.0.2a9/src/apache_dolphinscheduler.egg-info/top_level.txt
--rw-r--r--   0 zhongjiajie   (501) staff       (20)        1 2023-01-31 10:37:45.000000 apache-dolphinscheduler-4.0.2a9/src/apache_dolphinscheduler.egg-info/zip-safe
-drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-07-13 01:58:59.178495 apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/
--rw-r--r--   0 zhongjiajie   (501) staff       (20)      850 2023-07-13 01:33:25.000000 apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/__init__.py
-drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-07-13 01:58:59.179111 apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/cli/
--rw-r--r--   0 zhongjiajie   (501) staff       (20)      839 2023-02-01 06:51:22.000000 apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/cli/__init__.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     3023 2023-03-21 06:23:03.000000 apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/cli/commands.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     7268 2023-04-04 15:19:49.000000 apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/configuration.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     3053 2023-07-05 10:40:26.000000 apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/constants.py
-drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-07-13 01:58:59.182517 apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/core/
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     1038 2023-04-04 15:19:49.000000 apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/core/__init__.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     3363 2023-03-21 06:23:03.000000 apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/core/engine.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     4557 2023-04-04 15:19:49.000000 apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/core/parameter.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     1168 2023-03-21 06:23:03.000000 apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/core/process_definition.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     2696 2023-07-05 10:40:26.000000 apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/core/resource.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     1997 2023-03-21 06:23:03.000000 apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/core/resource_plugin.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)    18112 2023-07-05 10:40:26.000000 apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/core/task.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)    16756 2023-07-06 10:48:38.000000 apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/core/workflow.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)    17251 2023-04-04 15:19:49.000000 apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/core/yaml_workflow.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     3102 2023-07-06 10:56:36.000000 apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/default_config.yaml
-drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-07-13 01:58:59.187913 apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/examples/
--rw-r--r--   0 zhongjiajie   (501) staff       (20)      869 2023-02-01 06:51:22.000000 apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/examples/__init__.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     2217 2023-04-04 15:19:49.000000 apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/examples/bulk_create_example.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     3841 2023-04-04 15:19:49.000000 apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/examples/local_parameter_example.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     2923 2023-04-04 15:19:49.000000 apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/examples/multi_resources_example.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     2341 2023-04-04 15:19:49.000000 apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/examples/task_condition_example.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     3596 2023-07-06 10:56:36.000000 apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/examples/task_datax_example.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     2510 2023-04-04 15:19:49.000000 apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/examples/task_dependent_example.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     1755 2023-04-04 15:19:49.000000 apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/examples/task_dvc_example.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     1326 2023-04-04 15:19:49.000000 apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/examples/task_flink_example.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     1289 2023-04-04 15:19:49.000000 apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/examples/task_kubernetes_example.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     1375 2023-04-04 15:19:49.000000 apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/examples/task_map_reduce_example.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     3104 2023-04-04 15:19:49.000000 apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/examples/task_mlflow_example.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     1415 2023-04-04 15:19:49.000000 apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/examples/task_openmldb_example.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     2794 2023-07-06 10:48:37.000000 apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/examples/task_python_example.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     2183 2023-04-04 15:19:49.000000 apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/examples/task_pytorch_example.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     1645 2023-04-04 15:19:49.000000 apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/examples/task_sagemaker_example.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     2637 2023-07-06 10:48:37.000000 apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/examples/task_shell_example.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     1320 2023-04-04 15:19:49.000000 apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/examples/task_spark_example.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     2111 2023-07-06 10:56:05.000000 apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/examples/task_sql_example.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     2084 2023-04-04 15:19:49.000000 apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/examples/task_switch_example.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     2352 2023-07-06 10:56:36.000000 apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/examples/tutorial.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     2763 2023-04-04 15:19:49.000000 apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/examples/tutorial_decorator.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     2070 2023-04-04 15:19:49.000000 apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/examples/tutorial_resource_plugin.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     1624 2023-03-21 06:23:03.000000 apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/exceptions.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)    10423 2023-07-06 10:18:33.000000 apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/java_gateway.py
-drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-07-13 01:58:59.190705 apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/models/
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     1379 2023-02-23 11:36:13.000000 apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/models/__init__.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     2776 2023-02-01 06:51:22.000000 apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/models/base.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     1667 2023-03-21 06:23:03.000000 apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/models/base_side.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     1083 2023-04-04 15:19:49.000000 apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/models/connection.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     5983 2023-07-06 10:56:59.000000 apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/models/datasource.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     4779 2023-04-04 15:19:49.000000 apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/models/meta.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     2503 2023-03-21 06:23:03.000000 apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/models/project.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     1185 2023-03-21 06:23:03.000000 apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/models/queue.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     2802 2023-04-04 15:19:49.000000 apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/models/tenant.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     3948 2023-04-04 15:19:49.000000 apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/models/user.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     1146 2023-02-01 06:51:22.000000 apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/models/worker_group.py
-drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-07-13 01:58:59.191910 apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/resources_plugin/
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     1171 2023-03-21 06:23:03.000000 apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/resources_plugin/__init__.py
-drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-07-13 01:58:59.192506 apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/resources_plugin/base/
--rw-r--r--   0 zhongjiajie   (501) staff       (20)      811 2023-03-21 06:23:03.000000 apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/resources_plugin/base/__init__.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     2806 2023-03-21 06:23:03.000000 apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/resources_plugin/base/bucket.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     3824 2023-03-21 06:23:03.000000 apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/resources_plugin/base/git.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     3922 2023-03-21 06:23:03.000000 apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/resources_plugin/github.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     4312 2023-03-21 06:23:03.000000 apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/resources_plugin/gitlab.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     2019 2023-03-21 06:23:03.000000 apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/resources_plugin/local.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     3038 2023-03-21 06:23:03.000000 apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/resources_plugin/oss.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     2838 2023-03-21 06:23:03.000000 apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/resources_plugin/s3.py
-drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-07-13 01:58:59.196718 apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/tasks/
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     2475 2023-03-21 06:23:03.000000 apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/tasks/__init__.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     6813 2023-02-01 06:51:22.000000 apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/tasks/condition.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     4987 2023-07-06 10:54:10.000000 apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/tasks/datax.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     9737 2023-03-21 06:23:03.000000 apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/tasks/dependent.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     3605 2023-03-21 06:23:03.000000 apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/tasks/dvc.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     2883 2023-02-01 06:51:22.000000 apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/tasks/flink.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     2221 2023-04-04 15:19:49.000000 apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/tasks/func_wrap.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     3542 2023-04-04 15:19:44.000000 apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/tasks/http.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     1949 2023-03-21 06:23:03.000000 apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/tasks/kubernetes.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     1679 2023-02-01 06:51:22.000000 apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/tasks/map_reduce.py
-drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-07-13 01:58:59.197160 apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/tasks/mixin/
--rw-r--r--   0 zhongjiajie   (501) staff       (20)        0 2023-07-06 09:03:45.000000 apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/tasks/mixin/__init__.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)      832 2023-07-06 10:48:37.000000 apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/tasks/mixin/datasource_list_mixin.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)      841 2023-07-06 10:48:38.000000 apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/tasks/mixin/remote_connection_mixin.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     8634 2023-03-21 06:23:03.000000 apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/tasks/mlflow.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     1754 2023-03-21 06:23:03.000000 apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/tasks/openmldb.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     2435 2023-07-06 10:48:38.000000 apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/tasks/procedure.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     4503 2023-07-06 10:48:38.000000 apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/tasks/python.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     3527 2023-03-21 06:23:03.000000 apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/tasks/pytorch.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     1585 2023-03-21 06:23:03.000000 apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/tasks/sagemaker.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     3011 2023-07-06 10:48:37.000000 apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/tasks/shell.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     2636 2023-03-21 06:23:03.000000 apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/tasks/spark.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     5549 2023-07-06 10:48:38.000000 apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/tasks/sql.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     1627 2023-03-21 06:23:03.000000 apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/tasks/sub_process.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     2225 2023-03-21 06:23:03.000000 apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/tasks/sub_workflow.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     5980 2023-03-21 06:23:03.000000 apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/tasks/switch.py
-drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-07-13 01:58:59.198161 apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/utils/
--rw-r--r--   0 zhongjiajie   (501) staff       (20)      812 2023-02-01 06:51:22.000000 apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/utils/__init__.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     3364 2023-03-21 06:23:03.000000 apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/utils/date.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     2193 2023-02-01 06:51:22.000000 apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/utils/file.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     1490 2023-02-01 06:51:22.000000 apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/utils/string.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     1790 2023-03-21 06:23:03.000000 apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/utils/versions.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     5311 2023-02-01 06:51:22.000000 apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/utils/yaml_parser.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)       23 2023-07-05 10:40:26.000000 apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/version_ext
-drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-07-13 01:58:59.198581 apache-dolphinscheduler-4.0.2a9/tests/
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     9827 2023-04-04 15:19:49.000000 apache-dolphinscheduler-4.0.2a9/tests/test_configuration.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     2398 2023-03-21 06:23:03.000000 apache-dolphinscheduler-4.0.2a9/tests/test_docs.py
+drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-04-14 05:54:06.792517 apache-dolphinscheduler-4.0.3/
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)    12843 2023-04-14 05:53:48.000000 apache-dolphinscheduler-4.0.3/CONTRIBUTING.md
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)    12553 2022-12-14 07:25:00.000000 apache-dolphinscheduler-4.0.3/LICENSE
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)      898 2023-04-04 15:19:49.000000 apache-dolphinscheduler-4.0.3/MANIFEST.in
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)      177 2022-12-14 07:25:00.000000 apache-dolphinscheduler-4.0.3/NOTICE
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     7851 2023-04-14 05:54:06.792642 apache-dolphinscheduler-4.0.3/PKG-INFO
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     6015 2023-04-04 15:19:49.000000 apache-dolphinscheduler-4.0.3/README.md
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     9770 2023-04-14 05:50:48.000000 apache-dolphinscheduler-4.0.3/RELEASE.md
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     2832 2023-04-04 15:19:49.000000 apache-dolphinscheduler-4.0.3/UPDATING.md
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     4781 2023-04-14 05:54:06.793482 apache-dolphinscheduler-4.0.3/setup.cfg
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     3027 2023-04-04 15:19:49.000000 apache-dolphinscheduler-4.0.3/setup.py
+drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-04-14 05:54:06.767804 apache-dolphinscheduler-4.0.3/src/
+drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-04-14 05:54:06.771202 apache-dolphinscheduler-4.0.3/src/apache_dolphinscheduler.egg-info/
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     7851 2023-04-14 05:54:06.000000 apache-dolphinscheduler-4.0.3/src/apache_dolphinscheduler.egg-info/PKG-INFO
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     4406 2023-04-14 05:54:06.000000 apache-dolphinscheduler-4.0.3/src/apache_dolphinscheduler.egg-info/SOURCES.txt
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)        1 2023-04-14 05:54:06.000000 apache-dolphinscheduler-4.0.3/src/apache_dolphinscheduler.egg-info/dependency_links.txt
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)       75 2023-04-14 05:54:06.000000 apache-dolphinscheduler-4.0.3/src/apache_dolphinscheduler.egg-info/entry_points.txt
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)      577 2023-04-14 05:54:06.000000 apache-dolphinscheduler-4.0.3/src/apache_dolphinscheduler.egg-info/requires.txt
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)       19 2023-04-14 05:54:06.000000 apache-dolphinscheduler-4.0.3/src/apache_dolphinscheduler.egg-info/top_level.txt
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)        1 2023-01-31 10:37:45.000000 apache-dolphinscheduler-4.0.3/src/apache_dolphinscheduler.egg-info/zip-safe
+drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-04-14 05:54:06.772986 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)      848 2023-04-14 05:53:48.000000 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/__init__.py
+drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-04-14 05:54:06.773420 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/cli/
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)      839 2023-02-01 06:51:22.000000 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/cli/__init__.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     3023 2023-03-21 06:23:03.000000 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/cli/commands.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     7268 2023-04-04 15:19:49.000000 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/configuration.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     2981 2023-04-14 05:53:48.000000 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/constants.py
+drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-04-14 05:54:06.775975 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/core/
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     1038 2023-04-04 15:19:49.000000 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/core/__init__.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     3363 2023-03-21 06:23:03.000000 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/core/engine.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     4557 2023-04-04 15:19:49.000000 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/core/parameter.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     1168 2023-03-21 06:23:03.000000 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/core/process_definition.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     2721 2023-04-14 05:53:48.000000 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/core/resource.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     1997 2023-03-21 06:23:03.000000 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/core/resource_plugin.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)    17725 2023-04-14 05:53:48.000000 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/core/task.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)    18099 2023-04-04 15:19:49.000000 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/core/workflow.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)    17251 2023-04-04 15:19:49.000000 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/core/yaml_workflow.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     3093 2023-04-04 15:20:36.000000 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/default_config.yaml
+drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-04-14 05:54:06.780672 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/examples/
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)      869 2023-02-01 06:51:22.000000 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/examples/__init__.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     2217 2023-04-04 15:19:49.000000 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/examples/bulk_create_example.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     3841 2023-04-04 15:19:49.000000 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/examples/local_parameter_example.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     2923 2023-04-04 15:19:49.000000 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/examples/multi_resources_example.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     2341 2023-04-04 15:19:49.000000 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/examples/task_condition_example.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     3570 2023-04-04 15:19:49.000000 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/examples/task_datax_example.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     2510 2023-04-04 15:19:49.000000 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/examples/task_dependent_example.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     1755 2023-04-04 15:19:49.000000 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/examples/task_dvc_example.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     1326 2023-04-04 15:19:49.000000 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/examples/task_flink_example.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     1289 2023-04-04 15:19:49.000000 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/examples/task_kubernetes_example.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     1375 2023-04-04 15:19:49.000000 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/examples/task_map_reduce_example.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     3104 2023-04-04 15:19:49.000000 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/examples/task_mlflow_example.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     1415 2023-04-04 15:19:49.000000 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/examples/task_openmldb_example.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     2183 2023-04-04 15:19:49.000000 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/examples/task_pytorch_example.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     1645 2023-04-04 15:19:49.000000 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/examples/task_sagemaker_example.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     1320 2023-04-04 15:19:49.000000 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/examples/task_spark_example.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     2110 2023-04-04 15:19:49.000000 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/examples/task_sql_example.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     2084 2023-04-04 15:19:49.000000 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/examples/task_switch_example.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     1903 2023-04-11 03:29:16.000000 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/examples/tutorial.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     2763 2023-04-04 15:19:49.000000 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/examples/tutorial_decorator.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     2070 2023-04-04 15:19:49.000000 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/examples/tutorial_resource_plugin.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     1624 2023-03-21 06:23:03.000000 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/exceptions.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)    11531 2023-04-14 05:53:48.000000 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/java_gateway.py
+drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-04-14 05:54:06.782996 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/models/
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     1379 2023-02-23 11:36:13.000000 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/models/__init__.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     2776 2023-02-01 06:51:22.000000 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/models/base.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     1667 2023-03-21 06:23:03.000000 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/models/base_side.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     1083 2023-04-04 15:19:49.000000 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/models/connection.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     6290 2023-04-04 15:19:49.000000 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/models/datasource.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     4779 2023-04-04 15:19:49.000000 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/models/meta.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     2503 2023-03-21 06:23:03.000000 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/models/project.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     1185 2023-03-21 06:23:03.000000 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/models/queue.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     2802 2023-04-04 15:19:49.000000 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/models/tenant.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     3948 2023-04-04 15:19:49.000000 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/models/user.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     1146 2023-02-01 06:51:22.000000 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/models/worker_group.py
+drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-04-14 05:54:06.784232 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/resources_plugin/
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     1171 2023-03-21 06:23:03.000000 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/resources_plugin/__init__.py
+drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-04-14 05:54:06.784756 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/resources_plugin/base/
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)      811 2023-03-21 06:23:03.000000 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/resources_plugin/base/__init__.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     2806 2023-03-21 06:23:03.000000 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/resources_plugin/base/bucket.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     3824 2023-03-21 06:23:03.000000 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/resources_plugin/base/git.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     3922 2023-03-21 06:23:03.000000 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/resources_plugin/github.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     4312 2023-03-21 06:23:03.000000 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/resources_plugin/gitlab.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     2019 2023-03-21 06:23:03.000000 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/resources_plugin/local.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     3038 2023-03-21 06:23:03.000000 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/resources_plugin/oss.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     2838 2023-03-21 06:23:03.000000 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/resources_plugin/s3.py
+drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-04-14 05:54:06.790786 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/tasks/
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     2475 2023-03-21 06:23:03.000000 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/tasks/__init__.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     6813 2023-02-01 06:51:22.000000 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/tasks/condition.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     5209 2023-04-04 15:19:49.000000 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/tasks/datax.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     9737 2023-03-21 06:23:03.000000 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/tasks/dependent.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     3605 2023-03-21 06:23:03.000000 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/tasks/dvc.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     2883 2023-02-01 06:51:22.000000 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/tasks/flink.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     2221 2023-04-04 15:19:49.000000 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/tasks/func_wrap.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     3542 2023-04-04 15:19:44.000000 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/tasks/http.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     1949 2023-03-21 06:23:03.000000 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/tasks/kubernetes.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     1679 2023-02-01 06:51:22.000000 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/tasks/map_reduce.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     8634 2023-03-21 06:23:03.000000 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/tasks/mlflow.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     1754 2023-03-21 06:23:03.000000 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/tasks/openmldb.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     2637 2023-04-04 15:19:49.000000 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/tasks/procedure.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     3763 2023-04-04 15:19:49.000000 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/tasks/python.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     3527 2023-03-21 06:23:03.000000 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/tasks/pytorch.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     1585 2023-03-21 06:23:03.000000 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/tasks/sagemaker.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     1952 2023-03-21 06:23:03.000000 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/tasks/shell.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     2636 2023-03-21 06:23:03.000000 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/tasks/spark.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     5687 2023-04-04 15:19:49.000000 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/tasks/sql.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     1627 2023-03-21 06:23:03.000000 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/tasks/sub_process.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     2225 2023-03-21 06:23:03.000000 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/tasks/sub_workflow.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     5980 2023-03-21 06:23:03.000000 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/tasks/switch.py
+drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-04-14 05:54:06.791866 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/utils/
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)      812 2023-02-01 06:51:22.000000 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/utils/__init__.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     3364 2023-03-21 06:23:03.000000 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/utils/date.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     2193 2023-02-01 06:51:22.000000 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/utils/file.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     1490 2023-02-01 06:51:22.000000 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/utils/string.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     1790 2023-03-21 06:23:03.000000 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/utils/versions.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     5311 2023-02-01 06:51:22.000000 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/utils/yaml_parser.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)       31 2023-04-14 05:53:48.000000 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/version_ext
+drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-04-14 05:54:06.792182 apache-dolphinscheduler-4.0.3/tests/
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     9827 2023-04-04 15:19:49.000000 apache-dolphinscheduler-4.0.3/tests/test_configuration.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     2398 2023-03-21 06:23:03.000000 apache-dolphinscheduler-4.0.3/tests/test_docs.py
```

### Comparing `apache-dolphinscheduler-4.0.2a9/CONTRIBUTING.md` & `apache-dolphinscheduler-4.0.3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `apache-dolphinscheduler-4.0.2a9/LICENSE` & `apache-dolphinscheduler-4.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-dolphinscheduler-4.0.2a9/PKG-INFO` & `apache-dolphinscheduler-4.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-dolphinscheduler
-Version: 4.0.2a9
+Version: 4.0.3
 Summary: pydolphinscheduler is Apache DolphinScheduler Python API.
 Home-page: https://dolphinscheduler.apache.org/python/main/index.html
 Author: Apache Software Foundation
 Author-email: dev@dolphinscheduler.apache.org
 License: Apache License 2.0
 Project-URL: Homepage, https://dolphinscheduler.apache.org/python/main/index.html
 Project-URL: Documentation, https://dolphinscheduler.apache.org/python/main/index.html
```

### Comparing `apache-dolphinscheduler-4.0.2a9/README.md` & `apache-dolphinscheduler-4.0.3/README.md`

 * *Files identical despite different names*

### Comparing `apache-dolphinscheduler-4.0.2a9/RELEASE.md` & `apache-dolphinscheduler-4.0.3/RELEASE.md`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,16 @@
 ## Prepare
 
 * Remove `sphinx-multiversion` dependency in `setup.py`, we still can not fix this issue
   [Distribute tarball and wheel error with direct dependency](https://github.com/apache/dolphinscheduler/issues/12238)
 * Change `version_ext` about the dolphinscheduler version current support, the syntax is respect [pep-044](https://peps.python.org/pep-0440/#version-specifiers)
 * Run all test locally, `tox -e local-ci && tox -e local-integrate-test`, after you start dolphinscheduler to
   pass `local-integrate-test`
-* Show revert some dolphinscheduler not release commit `git revert 85a1dfaa`
+* Revert commit Apache dolphinscheduler not release yet, see [this link](https://github.com/apache/dolphinscheduler-sdk-python/pulls?q=is%3Apr+is%3Aclosed+label%3Adep-main-repo)
+  add check whether apache/dolphinscheduler commit is released, for some commit not release should revert the change
 
 ## Build and Sign Package
 
 We use [build](https://pypi.org/project/build/) to build package, and [twine](https://pypi.org/project/twine/) to
 upload package to PyPi. You could first install and upgrade them by:
 
 ```shell
@@ -77,21 +78,21 @@
 ```
 
 ### Vote Mail
 
 Create a new vote in dev@dolphinscheduler.apache.org
 
 ```text
-TITLE: [VOTE] Release Apache DolphinScheduler SDK Python <VERSION>
+TITLE: [VOTE] Release Apache DolphinScheduler Python SDK <VERSION>
 
 BODY:
 
 Hello DolphinScheduler Community,
 
-This is a call for the vote to release Apache DolphinScheduler SDK Python version <VERSION>
+This is a call for the vote to release Apache DolphinScheduler Python SDK version <VERSION>
 
 Release notes: https://github.com/apache/dolphinscheduler-sdk-python/releases/tag/<VERSION>
 
 The release candidates: https://dist.apache.org/repos/dist/dev/dolphinscheduler/python/<VERSION>/
 
 Git tag for the release: https://github.com/apache/dolphinscheduler-sdk-python/tree/<VERSION>
 
@@ -141,15 +142,15 @@
 Vote result should follow these:
 
 - PMC vote is +1 binding, all others is +1 no binding.
 - Within 72 hours, you get at least 3 (+1 binding), and have more +1 than -1. Vote pass.
 - **Send the closing vote mail to announce the result**. When count the binding and no binding votes, please list the names of voters. An example like this:
 
     ```text
-    [RESULT][VOTE] Release Apache SkyWalking Python version $VERSION
+    [RESULT][VOTE] Release Apache DolphinScheduler Python version $VERSION
     
     72+ hours passed, we’ve got ($NUMBER) +1 bindings (and ... +1 non-bindings):
     
     (list names)
     +1 bindings:
     xxx
     ...
@@ -172,29 +173,27 @@
     svn delete -m "remove old release Python SDK" https://dist.apache.org/repos/dist/release/dolphinscheduler/python/<PREVIOUS-RELEASE-VERSION>
     ```
 
 - Update [GitHub release page](https://github.com/apache/dolphinscheduler-sdk-python/releases) and set it as formal release.
 - Send ANNOUNCE email to `dev@dolphinscheduler.apache.org` and `announce@apache.org`.
 
     ```text
-    Subject: [ANNOUNCE] Apache DolphinScheduler SDK Python $VERSION Released
+    Subject: [ANNOUNCE] Apache DolphinScheduler Python SDK $VERSION Released
 
     Content:
 
     Hi Community,
 
-    We are glad to announce the release of Apache DolphinScheduler SDK Python $VERSION.
+    We are glad to announce the release of Apache DolphinScheduler Python SDK $VERSION.
 
-    Apache DolphinScheduler SDK Python is an API for Apache DolphinScheduler which allow you definition your workflow by Python code, aka workflow-as-codes.
+    Apache DolphinScheduler Python SDK is an API for Apache DolphinScheduler which allows you to define your workflow by Python code, aka workflow-as-codes.
   
     DolphinScheduler is a distributed and easy-to-extend visual workflow scheduler system,
     dedicated to solving the complex task dependencies in data processing, making the scheduler system out of the box for data processing.
 
-    Download Links: https://dolphinscheduler.apache.org/#/en-us/download
-
     Release Notes: https://github.com/apache/dolphinscheduler-sdk-python/releases/tag/$VERSION
 
     DolphinScheduler Resources:
     - Issue: https://github.com/apache/dolphinscheduler-sdk-python/issues/
     - Mailing list: dev@dolphinscheduler.apache.org
     - Website: https://dolphinscheduler.apache.org
     - Documents: https://dolphinscheduler.apache.org/python/$VERSION
@@ -204,28 +203,24 @@
 
 [PyPI](https://pypi.org), Python Package Index, is a repository of software for the Python programming language.
 
 ### Release to TestPyPi
 
 TestPyPi is a test environment of PyPi, you could release to it to test whether the package is work or not.
 
-1. Create an account in [TestPyPi](https://test.pypi.org/account/register/).
-2. Clean unrelated files in `dist` directory, and build package `python3 setup.py clean`.
-3. Build package `python3 -m build`, and you will see two new files in `dist` directory, with extension
-   `.tar.gz` and `.whl`.
-4. Upload to TestPyPi `python3 -m twine upload --repository testpypi dist/*`.
-5. Check the package in [TestPyPi](https://test.pypi.org/project/apache-dolphinscheduler/) and install it
+1. (Optional) Create an account in [TestPyPi](https://test.pypi.org/account/register/), only need for first release.
+2. Clean `dist` directory and build `python3 setup.py clean && python3 -m build`.
+3. Upload to TestPyPi `python3 -m twine upload --repository testpypi dist/*`.
+4. Check the package in [TestPyPi](https://test.pypi.org/project/apache-dolphinscheduler/) and install it
    by `python3 -m pip install --index-url https://test.pypi.org/simple/ --no-deps apache-dolphinscheduler` to
    test whether it is work or not.
 
 ### Release to PyPi
 
 PyPi is the official repository of Python packages, it is highly recommended [releasing package to TestPyPi](#release-to-testpypi)
 first to test whether the package is correct.
 
-1. Create an account in [PyPI](https://pypi.org/account/register/).
-2. Clean unrelated files in `dist` directory, and build package `python3 setup.py clean`.
-3. Build package `python3 -m build`, and you will see two new files in `dist` directory, with extension
-   `.tar.gz` and `.whl`.
-4. Upload to TestPyPi `python3 -m twine upload dist/*`.
-5. Check the package in [PyPi](https://pypi.org/project/apache-dolphinscheduler/) and install it
+1. (Optional) Create an account in [PyPI](https://pypi.org/account/register/), only need for first release.
+2. Clean `dist` directory and build `python3 setup.py clean && python3 -m build`.
+3. Upload to TestPyPi `python3 -m twine upload dist/*`.
+4. Check the package in [PyPi](https://pypi.org/project/apache-dolphinscheduler/) and install it
    by `python3 -m pip install apache-dolphinscheduler` to install it.
```

### Comparing `apache-dolphinscheduler-4.0.2a9/UPDATING.md` & `apache-dolphinscheduler-4.0.3/UPDATING.md`

 * *Files identical despite different names*

### Comparing `apache-dolphinscheduler-4.0.2a9/setup.py` & `apache-dolphinscheduler-4.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `apache-dolphinscheduler-4.0.2a9/src/apache_dolphinscheduler.egg-info/PKG-INFO` & `apache-dolphinscheduler-4.0.3/src/apache_dolphinscheduler.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-dolphinscheduler
-Version: 4.0.2a9
+Version: 4.0.3
 Summary: pydolphinscheduler is Apache DolphinScheduler Python API.
 Home-page: https://dolphinscheduler.apache.org/python/main/index.html
 Author: Apache Software Foundation
 Author-email: dev@dolphinscheduler.apache.org
 License: Apache License 2.0
 Project-URL: Homepage, https://dolphinscheduler.apache.org/python/main/index.html
 Project-URL: Documentation, https://dolphinscheduler.apache.org/python/main/index.html
```

### Comparing `apache-dolphinscheduler-4.0.2a9/src/apache_dolphinscheduler.egg-info/SOURCES.txt` & `apache-dolphinscheduler-4.0.3/src/apache_dolphinscheduler.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 CONTRIBUTING.md
 LICENSE
+MANIFEST.in
 NOTICE
 README.md
 RELEASE.md
 UPDATING.md
 setup.cfg
 setup.py
 src/apache_dolphinscheduler.egg-info/PKG-INFO
@@ -40,18 +41,16 @@
 src/pydolphinscheduler/examples/task_dependent_example.py
 src/pydolphinscheduler/examples/task_dvc_example.py
 src/pydolphinscheduler/examples/task_flink_example.py
 src/pydolphinscheduler/examples/task_kubernetes_example.py
 src/pydolphinscheduler/examples/task_map_reduce_example.py
 src/pydolphinscheduler/examples/task_mlflow_example.py
 src/pydolphinscheduler/examples/task_openmldb_example.py
-src/pydolphinscheduler/examples/task_python_example.py
 src/pydolphinscheduler/examples/task_pytorch_example.py
 src/pydolphinscheduler/examples/task_sagemaker_example.py
-src/pydolphinscheduler/examples/task_shell_example.py
 src/pydolphinscheduler/examples/task_spark_example.py
 src/pydolphinscheduler/examples/task_sql_example.py
 src/pydolphinscheduler/examples/task_switch_example.py
 src/pydolphinscheduler/examples/tutorial.py
 src/pydolphinscheduler/examples/tutorial_decorator.py
 src/pydolphinscheduler/examples/tutorial_resource_plugin.py
 src/pydolphinscheduler/models/__init__.py
@@ -92,17 +91,14 @@
 src/pydolphinscheduler/tasks/sagemaker.py
 src/pydolphinscheduler/tasks/shell.py
 src/pydolphinscheduler/tasks/spark.py
 src/pydolphinscheduler/tasks/sql.py
 src/pydolphinscheduler/tasks/sub_process.py
 src/pydolphinscheduler/tasks/sub_workflow.py
 src/pydolphinscheduler/tasks/switch.py
-src/pydolphinscheduler/tasks/mixin/__init__.py
-src/pydolphinscheduler/tasks/mixin/datasource_list_mixin.py
-src/pydolphinscheduler/tasks/mixin/remote_connection_mixin.py
 src/pydolphinscheduler/utils/__init__.py
 src/pydolphinscheduler/utils/date.py
 src/pydolphinscheduler/utils/file.py
 src/pydolphinscheduler/utils/string.py
 src/pydolphinscheduler/utils/versions.py
 src/pydolphinscheduler/utils/yaml_parser.py
 tests/test_configuration.py
```

### Comparing `apache-dolphinscheduler-4.0.2a9/src/apache_dolphinscheduler.egg-info/requires.txt` & `apache-dolphinscheduler-4.0.3/src/apache_dolphinscheduler.egg-info/requires.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 boto3>=1.23.10
 oss2>=2.16.0
 python-gitlab>=2.10.1
 click>=8.0.0
 py4j~=0.10
 ruamel.yaml
 stmdency>=0.0.2
-packaging==21.3
+packaging>=21.3
 
 [build]
 build
 setuptools>=42
 wheel
 
 [dev]
```

### Comparing `apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/__init__.py` & `apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,8 +13,8 @@
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 """Init root of pydolphinscheduler."""
 
-__version__ = "4.0.2a9"
+__version__ = "4.0.3"
```

### Comparing `apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/cli/__init__.py` & `apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/cli/commands.py` & `apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/cli/commands.py`

 * *Files identical despite different names*

### Comparing `apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/configuration.py` & `apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/configuration.py`

 * *Files identical despite different names*

### Comparing `apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/constants.py` & `apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/constants.py`

 * *Files 5% similar despite different names*

```diff
@@ -31,21 +31,14 @@
 class TaskFlag(str):
     """Constants for task flag."""
 
     YES = "YES"
     NO = "NO"
 
 
-class IsCache(str):
-    """Constants for Cache."""
-
-    YES = "YES"
-    NO = "NO"
-
-
 class TaskTimeoutFlag(str):
     """Constants for task timeout flag."""
 
     OFF = "CLOSE"
     ON = "OPEN"
 
 
@@ -115,15 +108,15 @@
     FMT_STD_TIME = "%H:%M:%S"
     FMT_NO_COLON_TIME = "%H%M%S"
 
 
 class ResourceKey(str):
     """Constants for key of resource."""
 
-    ID = "id"
+    NAME = "resourceName"
 
 
 class Symbol(str):
     """Constants for symbol."""
 
     SLASH = "/"
     POINT = "."
```

### Comparing `apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/core/__init__.py` & `apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/core/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/core/engine.py` & `apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/core/engine.py`

 * *Files identical despite different names*

### Comparing `apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/core/parameter.py` & `apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/core/parameter.py`

 * *Files identical despite different names*

### Comparing `apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/core/process_definition.py` & `apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/core/process_definition.py`

 * *Files identical despite different names*

### Comparing `apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/core/resource.py` & `apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/core/resource.py`

 * *Files 11% similar despite different names*

```diff
@@ -51,23 +51,23 @@
         """Get resource info from java gateway, contains resource id, name."""
         if not self.user_name:
             raise PyDSParamException(
                 "`user_name` is required when querying resources from python gate."
             )
         return gateway.query_resources_file_info(self.user_name, self.name)
 
-    def get_id_from_database(self):
-        """Get resource id from java gateway."""
-        return self.get_info_from_database().getId()
+    def get_fullname_from_database(self):
+        """Get resource fullname from java gateway."""
+        return self.get_info_from_database().getFullName()
 
     def create_or_update_resource(self):
         """Create or update resource via java gateway."""
         if not self.content or not self.user_name:
             raise PyDSParamException(
                 "`user_name` and `content` are required when create or update resource from python gate."
             )
-        gateway.create_or_update_resource(
+        return gateway.create_or_update_resource(
             self.user_name,
             self.name,
-            self.content,
             self.description,
+            self.content,
         )
```

### Comparing `apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/core/resource_plugin.py` & `apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/core/resource_plugin.py`

 * *Files identical despite different names*

### Comparing `apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/core/task.py` & `apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/core/task.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,14 @@
 from datetime import timedelta
 from logging import getLogger
 from typing import Dict, List, Optional, Sequence, Set, Tuple, Union
 
 from pydolphinscheduler import configuration
 from pydolphinscheduler.constants import (
     Delimiter,
-    IsCache,
     ResourceKey,
     Symbol,
     TaskFlag,
     TaskPriority,
     TaskTimeoutFlag,
 )
 from pydolphinscheduler.core.parameter import BaseDataType, Direction, ParameterHelper
@@ -97,15 +96,14 @@
     :param fail_retry_interval: default 1
     :param timeout_notify_strategy: default, None
     :param timeout: default None
     :param resource_list: default None
     :param wait_start_timeout: default None
     :param condition_result: default None,
     :param resource_plugin: default None
-    :param is_cache: default False
     :param input_params: default None, input parameters, {param_name: param_value}
     :param output_params: default None, input parameters, {param_name: param_value}
     """
 
     _DEFINE_ATTR = {
         "name",
         "code",
@@ -119,15 +117,14 @@
         "environment_code",
         "delay_time",
         "fail_retry_times",
         "fail_retry_interval",
         "timeout_flag",
         "timeout_notify_strategy",
         "timeout",
-        "is_cache",
     }
 
     # task default attribute will into `task_params` property
     _task_default_attr = {
         "local_params",
         "resource_list",
         "dependence",
@@ -160,24 +157,22 @@
         timeout: Optional[timedelta] = None,
         workflow: Optional[Workflow] = None,
         resource_list: Optional[List] = None,
         dependence: Optional[Dict] = None,
         wait_start_timeout: Optional[Dict] = None,
         condition_result: Optional[Dict] = None,
         resource_plugin: Optional[ResourcePlugin] = None,
-        is_cache: Optional[bool] = False,
         input_params: Optional[Dict] = None,
         output_params: Optional[Dict] = None,
         *args,
         **kwargs,
     ):
         super().__init__(name, description)
         self.task_type = task_type
         self.flag = flag
-        self._is_cache = is_cache
         self.task_priority = task_priority
         self.worker_group = worker_group
         self._environment_name = environment_name
         self.fail_retry_times = fail_retry_times
         self.fail_retry_interval = fail_retry_interval
         self.delay_time = delay_time
         self.timeout_notify_strategy = timeout_notify_strategy
@@ -248,40 +243,34 @@
 
     @property
     def timeout_flag(self) -> str:
         """Whether the timeout attribute is being set or not."""
         return TaskTimeoutFlag.ON if self._timeout else TaskTimeoutFlag.OFF
 
     @property
-    def is_cache(self) -> str:
-        """Whether the cache is being set or not."""
-        if isinstance(self._is_cache, bool):
-            return IsCache.YES if self._is_cache else IsCache.NO
-        else:
-            raise PyDSParamException("is_cache must be a bool")
-
-    @property
     def resource_list(self) -> List[Dict[str, Resource]]:
         """Get task define attribute `resource_list`."""
         resources = set()
         for res in self._resource_list:
             if type(res) == str:
                 resources.add(
-                    Resource(name=res, user_name=self.user_name).get_id_from_database()
+                    Resource(
+                        name=res, user_name=self.user_name
+                    ).get_fullname_from_database()
                 )
-            elif type(res) == dict and res.get(ResourceKey.ID) is not None:
+            elif type(res) == dict and ResourceKey.NAME in res:
                 warnings.warn(
                     """`resource_list` should be defined using List[str] with resource paths,
                        the use of ids to define resources will be remove in version 3.2.0.
                     """,
                     DeprecationWarning,
                     stacklevel=2,
                 )
-                resources.add(res.get(ResourceKey.ID))
-        return [{ResourceKey.ID: r} for r in resources]
+                resources.add(res.get(ResourceKey.NAME))
+        return [{ResourceKey.NAME: r} for r in resources]
 
     @property
     def user_name(self) -> Optional[str]:
         """Return username of workflow."""
         if self.workflow:
             return self.workflow.user.name
         else:
```

### Comparing `apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/core/workflow.py` & `apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/core/workflow.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,21 +18,21 @@
 """Module workflow, core class for workflow define."""
 
 import json
 from datetime import datetime
 from typing import Any, Dict, List, Optional, Set, Union
 
 from pydolphinscheduler import configuration
-from pydolphinscheduler.constants import TaskType
+from pydolphinscheduler.constants import Symbol, TaskType
 from pydolphinscheduler.core.resource import Resource
 from pydolphinscheduler.core.resource_plugin import ResourcePlugin
 from pydolphinscheduler.exceptions import PyDSParamException, PyDSTaskNoFoundException
 from pydolphinscheduler.java_gateway import gateway
 from pydolphinscheduler.models import Base, Project, User
-from pydolphinscheduler.utils.date import conv_from_str
+from pydolphinscheduler.utils.date import MAX_DATETIME, conv_from_str, conv_to_schedule
 
 
 class WorkflowContext:
     """Class workflow context, use when task get workflow from context expression."""
 
     _context_managed_workflow: Optional["Workflow"] = None
 
@@ -115,15 +115,16 @@
 
     _EXPECT_SCHEDULE_CHAR_NUM = 7
 
     def __init__(
         self,
         name: str,
         description: Optional[str] = None,
-        timing_name: Optional[str] = None,
+        schedule: Optional[str] = None,
+        online_schedule: Optional[bool] = None,
         start_time: Optional[Union[str, datetime]] = None,
         end_time: Optional[Union[str, datetime]] = None,
         timezone: Optional[str] = configuration.WORKFLOW_TIME_ZONE,
         user: Optional[str] = configuration.WORKFLOW_USER,
         project: Optional[str] = configuration.WORKFLOW_PROJECT,
         worker_group: Optional[str] = configuration.WORKFLOW_WORKER_GROUP,
         warning_type: Optional[str] = configuration.WORKFLOW_WARNING_TYPE,
@@ -134,17 +135,30 @@
         param: Optional[Dict] = None,
         resource_plugin: Optional[ResourcePlugin] = None,
         resource_list: Optional[List[Resource]] = None,
         *args,
         **kwargs,
     ):
         super().__init__(name, description)
-        self.timing_name = timing_name.strip() if timing_name else timing_name
+        self.schedule = schedule.strip() if schedule else schedule
+        if (
+            self.schedule
+            and self.schedule.count(Symbol.BLANK) != self._EXPECT_SCHEDULE_CHAR_NUM - 1
+        ):
+            raise PyDSParamException(
+                "Invlaid parameter schedule, expect crontab char is %d but get %s",
+                self._EXPECT_SCHEDULE_CHAR_NUM,
+                schedule,
+            )
 
         #  handle workflow schedule state according to init value
+        if self.schedule and online_schedule is None:
+            self.online_schedule = True
+        else:
+            self.online_schedule = online_schedule or False
         self._start_time = start_time
         self._end_time = end_time
         self.timezone = timezone
         self._user = user
         self._project = project
         self.worker_group = worker_group
         self.warning_type = warning_type
@@ -289,14 +303,33 @@
         if not self.tasks:
             return [self.tasks]
         else:
             self._handle_root_relation()
             return [tr.get_define() for tr in self._task_relations]
 
     @property
+    def schedule_json(self) -> Optional[Dict]:
+        """Get schedule parameter json object. This is requests from java gateway interface."""
+        if not self.schedule:
+            return None
+        else:
+            start_time = conv_to_schedule(
+                self.start_time if self.start_time else datetime.now()
+            )
+            end_time = conv_to_schedule(
+                self.end_time if self.end_time else MAX_DATETIME
+            )
+            return {
+                "startTime": start_time,
+                "endTime": end_time,
+                "crontab": self.schedule,
+                "timezoneId": self.timezone,
+            }
+
+    @property
     def task_list(self) -> List["Task"]:  # noqa: F821
         """Return list of tasks objects."""
         return list(self.tasks.values())
 
     def _handle_root_relation(self):
         """Handle root task property :class:`pydolphinscheduler.core.task.TaskRelation`.
 
@@ -414,15 +447,16 @@
             self.execution_type,
             self.timeout,
             self.worker_group,
             self.release_state,
             # TODO add serialization function
             json.dumps(self.task_relation_json),
             json.dumps(self.task_definition_json),
-            self.timing_name,
+            json.dumps(self.schedule_json) if self.schedule_json else None,
+            self.online_schedule,
             None,
         )
         return self._workflow_code
 
     def start(self) -> None:
         """Create and start Workflow instance.
```

### Comparing `apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/core/yaml_workflow.py` & `apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/core/yaml_workflow.py`

 * *Files identical despite different names*

### Comparing `apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/default_config.yaml` & `apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/default_config.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -38,26 +38,26 @@
 # including ``user``, ``workflow`` 
 default:
   # Default value for dolphinscheduler's user object
   user:
     name: admin
     password: dolphinscheduler123
     email: userPythonGateway@dolphinscheduler.com
-    tenant: whalescheduler
+    tenant: default
     phone: 11111111111
     state: 1
   # Default value for dolphinscheduler's workflow object
   workflow:
-    project: pydolphinscheduler
+    project: project-pydolphin
     user: admin
     queue: queuePythonGateway
     worker_group: default
     # Release state of workflow, default value is ``online`` which mean setting workflow online when it submits
     # to Java gateway, if you want to set workflow offline set its value to ``offline``
-    release_state: offline
+    release_state: online
     time_zone: Asia/Shanghai
     # Warning type of the workflow, default value is ``NONE`` mean do not warn user in any cases of workflow state,
     # change to ``FAILURE`` if you want to warn users when workflow failed. All available enum value are
     # ``NONE``, ``SUCCESS``, ``FAILURE``, ``ALL`` 
     warning_type: NONE
     # Default execution type about how to run multiple workflow instances, default value is ``parallel`` which
     # mean run all workflow instances parallel and the other value is ``SERIAL_WAIT``, ``SERIAL_DISCARD``, ``SERIAL_PRIORITY``
```

### Comparing `apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/examples/__init__.py` & `apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/examples/bulk_create_example.py` & `apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/examples/bulk_create_example.py`

 * *Files identical despite different names*

### Comparing `apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/examples/local_parameter_example.py` & `apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/examples/local_parameter_example.py`

 * *Files identical despite different names*

### Comparing `apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/examples/multi_resources_example.py` & `apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/examples/multi_resources_example.py`

 * *Files identical despite different names*

### Comparing `apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/examples/task_condition_example.py` & `apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/examples/task_condition_example.py`

 * *Files identical despite different names*

### Comparing `apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/examples/task_datax_example.py` & `apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/examples/task_datax_example.py`

 * *Files 6% similar despite different names*

```diff
@@ -70,15 +70,14 @@
             "speed": {"channel": 1, "record": 1000},
         },
     }
 }
 
 with Workflow(
     name="task_datax_example",
-    release_state="offline",
 ) as workflow:
     # This task synchronizes the data in `t_ds_project`
     # of `first_mysql` database to `target_project` of `second_mysql` database.
     # You have to make sure data source named `first_mysql` and `second_mysql` exists
     # in your environment.
     task1 = DataX(
         name="task_datax",
@@ -86,10 +85,10 @@
         datatarget_name="second_mysql",
         sql="select id, name, code, description from source_table",
         target_table="target_table",
     )
 
     # You can custom json_template of datax to sync data. This task create a new
     # datax job same as task1, transfer record from `first_mysql` to `second_mysql`
-    task2 = CustomDataX(name="task_custom_datax", config=JSON_TEMPLATE)
+    task2 = CustomDataX(name="task_custom_datax", json=str(JSON_TEMPLATE))
     workflow.run()
 # [end workflow_declare]
```

### Comparing `apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/examples/task_dependent_example.py` & `apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/examples/task_dependent_example.py`

 * *Files identical despite different names*

### Comparing `apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/examples/task_dvc_example.py` & `apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/examples/task_dvc_example.py`

 * *Files identical despite different names*

### Comparing `apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/examples/task_flink_example.py` & `apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/examples/task_flink_example.py`

 * *Files identical despite different names*

### Comparing `apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/examples/task_kubernetes_example.py` & `apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/examples/task_kubernetes_example.py`

 * *Files identical despite different names*

### Comparing `apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/examples/task_map_reduce_example.py` & `apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/examples/task_map_reduce_example.py`

 * *Files identical despite different names*

### Comparing `apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/examples/task_mlflow_example.py` & `apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/examples/task_mlflow_example.py`

 * *Files identical despite different names*

### Comparing `apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/examples/task_openmldb_example.py` & `apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/examples/task_openmldb_example.py`

 * *Files identical despite different names*

### Comparing `apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/examples/task_python_example.py` & `apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/examples/tutorial_decorator.py`

 * *Files 14% similar despite different names*

```diff
@@ -27,24 +27,22 @@
                 \                    /
                   --> task_child_two
 
 it will instantiate and run all the task it have.
 """
 
 import time
-from datetime import datetime
 
 # [start tutorial]
 # [start package_import]
 # Import Workflow object to define your workflow attributes
 from pydolphinscheduler.core.workflow import Workflow
 
 # Import task Shell object cause we would create some shell tasks later
 from pydolphinscheduler.tasks.func_wrap import task
-from pydolphinscheduler.tasks.python import Python
 
 # [end package_import]
 
 scope_global = "global-var"
 
 
 # [start task_declare]
@@ -56,51 +54,53 @@
 
 @task
 def depend_import():
     """Depend on import module."""
     time.sleep(2)
 
 
-definition_str = """
-from datetime import datetime
+@task
+def depend_global_var():
+    """Depend on global var."""
+    print(f"Use global variable {scope_global}")
+
+
+@task
+def depend_local_var():
+    """Depend on local variable."""
+    scope_global = "local"
+    print(f"Use local variable overwrite global {scope_global}")
+
 
 def foo():
-    print("hello world in function foo")
-    print(f"Current time is {datetime.now()}")
-"""
+    """Call in other task."""
+    print("this is a global function")
 
 
-def bar():
-    print("hello world in function bar")
-    print(f"Current time is {datetime.now()}")
+@task
+def depend_func():
+    """Depend on global function."""
+    foo()
 
 
 # [end task_declare]
 
 
 # [start workflow_declare]
 with Workflow(
-    name="task_python",
+    name="tutorial_decorator",
     schedule="0 0 0 * * ? *",
     start_time="2021-01-01",
 ) as workflow:
     # [end workflow_declare]
 
-    python_str = Python(
-        name="python_str",
-        definition=definition_str,
-    )
-
-    python_func = Python(
-        name="python_func",
-        definition=bar,
-        datasource_name=["mysql-meta"],
-    )
-
     # [start task_relation_declare]
-    print_something() >> depend_import() >> python_str >> python_func
+    task_group = [depend_import(), depend_global_var()]
+    print_something().set_downstream(task_group)
+
+    task_group >> depend_local_var() >> depend_func()
     # [end task_relation_declare]
 
     # [start submit_or_run]
     workflow.submit()
     # [end submit_or_run]
 # [end tutorial]
```

### Comparing `apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/examples/task_pytorch_example.py` & `apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/examples/task_pytorch_example.py`

 * *Files identical despite different names*

### Comparing `apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/examples/task_sagemaker_example.py` & `apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/examples/task_sagemaker_example.py`

 * *Files identical despite different names*

### Comparing `apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/examples/task_spark_example.py` & `apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/examples/task_spark_example.py`

 * *Files identical despite different names*

### Comparing `apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/examples/task_sql_example.py` & `apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/examples/task_sql_example.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,38 +26,41 @@
 
 with Workflow(
     name="task_sql_example",
 ) as workflow:
     # [start bare_sql_desc]
     bare_sql = Sql(
         name="bare_sql",
-        datasource_name="whalescheduler",
+        datasource_name="metadata",
         sql="select * from t_ds_version",
     )
     # [end bare_sql_desc]
     # [start sql_file_desc]
     sql_file = Sql(
         name="sql_file",
-        datasource_name="whalescheduler",
+        datasource_name="metadata",
         sql="ext/example.sql",
         sql_type=SqlType.SELECT,
         resource_plugin=Local(prefix=str(Path(__file__).parent)),
     )
     # [end sql_file_desc]
     # [start sql_with_pre_post_desc]
     sql_with_pre_post = Sql(
         name="sql_with_pre_post",
-        datasource_name="whalescheduler",
+        datasource_name="metadata",
         sql="select * from t_ds_version",
         pre_statements=[
-            "update test.table_one set name = '1.3.6'",
-            "delete from test.table_two where name = '1.3.6'",
+            "update table_one set version = '1.3.6'",
+            "delete from table_two where version = '1.3.6'",
         ],
-        post_statements="update test.table_one set name = '3.0.0'",
+        post_statements="update table_one set version = '3.0.0'",
     )
     # [end sql_with_pre_post_desc]
 
-    bare_sql >> sql_file >> sql_with_pre_post
+    bare_sql >> [
+        sql_file,
+        sql_with_pre_post,
+    ]
 
     workflow.submit()
 
 # [end workflow_declare]
```

### Comparing `apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/examples/task_switch_example.py` & `apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/examples/task_switch_example.py`

 * *Files identical despite different names*

### Comparing `apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/examples/tutorial.py` & `apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/examples/tutorial_resource_plugin.py`

 * *Files 21% similar despite different names*

```diff
@@ -12,56 +12,52 @@
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 r"""
-A tutorial example take you to experience pydolphinscheduler.
+A tutorial example take you to experience pydolphinscheduler resource plugin.
 
-After tutorial.py file submit to Apache DolphinScheduler server a DAG would be create,
-and workflow DAG graph as below:
-
-                  --> task_child_one
-                /                    \
-task_parent -->                        -->  task_union
-                \                    /
-                  --> task_child_two
+Resource plug-ins can be defined in workflows and tasks
 
 it will instantiate and run all the task it have.
 """
+import os
+from pathlib import Path
 
-# [start tutorial]
+# [start tutorial_resource_plugin]
 # [start package_import]
 # Import Workflow object to define your workflow attributes
 from pydolphinscheduler.core.workflow import Workflow
 
 # Import task Shell object cause we would create some shell tasks later
+from pydolphinscheduler.resources_plugin.local import Local
 from pydolphinscheduler.tasks.shell import Shell
 
 # [end package_import]
 
 # [start workflow_declare]
 with Workflow(
-    name="tutorial",
+    name="tutorial_resource_plugin",
+    schedule="0 0 0 * * ? *",
     start_time="2021-01-01",
-    release_state="online",
+    resource_plugin=Local("/tmp"),
 ) as workflow:
     # [end workflow_declare]
     # [start task_declare]
-    task_parent = Shell(name="task_parent", command="echo hello pydolphinscheduler")
-    task_child_one = Shell(name="task_child_one", command="echo 'child one'")
-    task_child_two = Shell(name="task_child_two", command="echo 'child two'")
-    task_union = Shell(name="task_union", command="echo union")
+    file = "resource.sh"
+    path = Path("/tmp").joinpath(file)
+    with open(str(path), "w") as f:
+        f.write("echo tutorial resource plugin")
+    task_parent = Shell(
+        name="local-resource-example",
+        command=file,
+    )
+    print(task_parent.task_params)
+    os.remove(path)
     # [end task_declare]
 
-    # [start task_relation_declare]
-    task_group = [task_child_one, task_child_two]
-    task_parent.set_downstream(task_group)
-
-    task_union << task_group
-    # [end task_relation_declare]
-
     # [start submit_or_run]
-    workflow.submit()
+    workflow.run()
     # [end submit_or_run]
-# [end tutorial]
+# [end tutorial_resource_plugin]
```

### Comparing `apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/exceptions.py` & `apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/exceptions.py`

 * *Files identical despite different names*

### Comparing `apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/java_gateway.py` & `apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/java_gateway.py`

 * *Files 13% similar despite different names*

```diff
@@ -13,23 +13,27 @@
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 """Module java gateway, contain gateway behavior."""
 
+import contextlib
+import warnings
 from logging import getLogger
 from typing import Any, Optional
 
 from py4j.java_collections import JavaMap
 from py4j.java_gateway import GatewayParameters, JavaGateway
+from py4j.protocol import Py4JError
 
-from pydolphinscheduler import configuration
-from pydolphinscheduler.constants import JavaGatewayDefault
+from pydolphinscheduler import __version__, configuration
+from pydolphinscheduler.constants import JavaGatewayDefault, Version
 from pydolphinscheduler.exceptions import PyDSJavaGatewayException
+from pydolphinscheduler.utils.versions import version_match
 
 logger = getLogger(__name__)
 
 
 def gateway_result_checker(
     result: JavaMap,
     msg_check: Optional[str] = JavaGatewayDefault.RESULT_MESSAGE_SUCCESS,
@@ -59,14 +63,32 @@
         auth_token: Optional[str] = None,
     ):
         self._gateway = None
         self.address = address or configuration.JAVA_GATEWAY_ADDRESS
         self.port = port or configuration.JAVA_GATEWAY_PORT
         self.auto_convert = auto_convert or configuration.JAVA_GATEWAY_AUTO_CONVERT
         self.auth_token = auth_token or configuration.JAVA_GATEWAY_AUTH_TOKEN
+        gateway_version = "unknown"
+        with contextlib.suppress(Py4JError):
+            # 1. Java gateway version is too old: doesn't have method 'getGatewayVersion()'
+            # 2. Error connecting to Java gateway
+            gateway_version = self.get_gateway_version()
+        if (
+            not __version__.endswith("dev")
+            and gateway_version
+            and not version_match(Version.DS, gateway_version)
+        ):
+            warnings.warn(
+                f"Using unmatched version of pydolphinscheduler (version {__version__}) "
+                f"and Java gateway (version {gateway_version}) may cause errors. "
+                "We strongly recommend you to find the matched version "
+                "(check: https://pypi.org/project/apache-dolphinscheduler)",
+                UserWarning,
+                stacklevel=2,
+            )
 
     @property
     def gateway(self) -> JavaGateway:
         """Launch java gateway to pydolphinscheduler.
 
         TODO Note that automatic conversion makes calling Java methods slightly less efficient because
         in the worst case, Py4J needs to go through all registered converters for all parameters.
@@ -84,30 +106,30 @@
         self._gateway = JavaGateway(gateway_parameters=gateway_parameters)
         return self._gateway
 
     def get_gateway_version(self):
         """Get the java gateway version, expected to be equal with pydolphinscheduler."""
         return self.gateway.entry_point.getGatewayVersion()
 
-    def get_datasource(self, name: str):
+    def get_datasource(self, name: str, type: Optional[str] = None):
         """Get single datasource by java gateway.
 
         Will use datasource_name to query database, and then filter by datasource_type if provided.
 
         :param name: datasource name of the datasource to be queried
         :param type: datasource type of the datasource, only used to filter the result.
         """
-        return self.gateway.entry_point.getDatasource(name)
+        return self.gateway.entry_point.getDatasource(name, type)
 
     def get_resources_file_info(self, program_type: str, main_package: str):
         """Get resources file info through java gateway."""
         return self.gateway.entry_point.getResourcesFileInfo(program_type, main_package)
 
     def create_or_update_resource(
-        self, user_name: str, name: str, content: str, description: Optional[str] = None
+        self, user_name: str, name: str, description: str, content: str
     ):
         """Create or update resource through java gateway."""
         return self.gateway.entry_point.createOrUpdateResource(
             user_name, name, description, content
         )
 
     def query_resources_file_info(self, user_name: str, name: str):
@@ -247,25 +269,27 @@
         warning_group_id: int,
         execution_type: str,
         timeout: int,
         worker_group: str,
         release_state: int,
         task_relation_json: str,
         task_definition_json: str,
-        timingName: Optional[str] = None,
+        schedule: Optional[str] = None,
+        online_schedule: Optional[bool] = None,
         other_params_json: Optional[str] = None,
     ):
         """Create or update workflow through java gateway."""
         return self.gateway.entry_point.createOrUpdateWorkflow(
             user_name,
             project_name,
             name,
             description,
             global_params,
-            timingName,
+            schedule,
+            online_schedule,
             warning_type,
             warning_group_id,
             timeout,
             worker_group,
             release_state,
             task_relation_json,
             task_definition_json,
```

### Comparing `apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/models/__init__.py` & `apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/models/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/models/base.py` & `apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/models/base.py`

 * *Files identical despite different names*

### Comparing `apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/models/base_side.py` & `apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/models/base_side.py`

 * *Files identical despite different names*

### Comparing `apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/models/connection.py` & `apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/models/connection.py`

 * *Files identical despite different names*

### Comparing `apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/models/datasource.py` & `apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/models/datasource.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,25 +16,26 @@
 # under the License.
 
 """Module database."""
 import json
 import re
 from typing import NamedTuple, Optional
 
+from py4j.java_gateway import JavaObject
+
 from pydolphinscheduler.java_gateway import gateway
 from pydolphinscheduler.models.connection import Connection
 from pydolphinscheduler.models.meta import ModelMeta
 
 
 class TaskUsage(NamedTuple):
     """Class for task usage just like datasource in web ui."""
 
-    id: str
+    id: int
     type: str
-    name: str
 
 
 class Datasource(metaclass=ModelMeta):
     """Model datasource, communicate with DolphinScheduler API server and convert Java Object into Python.
 
     We use metaclass :class:`pydolphinscheduler.models.meta.ModelMeta` to convert Java Object into Python.
     And code in this class just call Java API method.
@@ -64,17 +65,15 @@
                 "jdbcUrl": "jdbc:mysql://127.0.0.1:3306/test",
                 "driverClassName": "com.mysql.cj.jdbc.Driver",
                 "validationQuery": "select 1"
             }
 
     """
 
-    _PATTERN = re.compile(
-        "jdbc:.*://(?P<host>[\\w\\W]+):(?P<port>\\d+)/(?P<database>[\\w\\W]+)\\?"
-    )
+    _PATTERN = re.compile("jdbc:.*://(?P<host>[\\w\\W]+):(?P<port>\\d+)")
 
     _DATABASE_TYPE_MAP = dict(
         mysql=0,
         postgresql=1,
         hive=2,
         spark=3,
         clickhouse=4,
@@ -86,68 +85,82 @@
         redshift=10,
         dameng=11,
         starrocks=12,
     )
 
     def __init__(
         self,
-        datasource_name: str,
-        plugin_name: str,
-        plugin_version: str,
-        datasource_config: str = None,
+        type_: str,
+        name: str,
+        connection_params: str,
+        user_id: Optional[int] = None,
         id_: Optional[int] = None,
-        description: Optional[str] = None,
+        note: Optional[str] = None,
     ):
         self.id = id_
-        self.datasource_name = datasource_name
-        self.plugin_name = plugin_name
-        self.plugin_version = plugin_version
-        self.datasource_config = datasource_config
-        self.description = description
+        self.name = name
+        self.note = note
+        # TODO try to handle type_ in metaclass
+        self.type_: JavaObject = type_
+        self.user_id = user_id
+        self.connection_params = connection_params
 
     @classmethod
-    def get(cls, datasource_name: str) -> "Datasource":
+    def get(
+        cls, datasource_name: str, datasource_type: Optional[str] = None
+    ) -> "Datasource":
         """Get single datasource.
 
         :param datasource_name: datasource name
         :param datasource_type: datasource type, if not provided, will get datasource by name only
         """
-        datasource = gateway.get_datasource(datasource_name)
+        datasource = gateway.get_datasource(datasource_name, datasource_type)
         if datasource is None:
-            raise ValueError(f"Datasource with name: {datasource_name} not found.")
+            raise ValueError(
+                f"Datasource with name: {datasource_name} and type: {datasource_type} not found."
+            )
         return datasource
 
     @classmethod
-    def get_task_usage_4j(cls, datasource_name: str) -> TaskUsage:
+    def get_task_usage_4j(
+        cls, datasource_name: str, datasource_type: Optional[str] = None
+    ) -> TaskUsage:
         """Get the necessary information of datasource for task usage in web UI."""
-        datasource: "Datasource" = cls.get(datasource_name)
+        datasource: "Datasource" = cls.get(datasource_name, datasource_type)
         return TaskUsage(
-            id=str(datasource.id),
-            type=datasource.plugin_name,
-            name=datasource.datasource_name,
+            id=datasource.id,
+            type=datasource.type.upper(),
         )
 
     @property
     def connection(self) -> Connection:
-        """Parse dolphinscheduler datasource_config to Connection."""
-        data = json.loads(self.datasource_config)
+        """Parse dolphinscheduler connection_params to Connection."""
+        data = json.loads(self.connection_params)
 
-        pattern_match = self._PATTERN.match(
-            data.get("jdbcUrl", data.get("url", None))
-        ).groupdict()
+        address_match = self._PATTERN.match(data.get("jdbcUrl", None)).groupdict()
 
         return Connection(
-            host=pattern_match.get("host", None),
-            port=int(pattern_match.get("port", None)),
-            schema=pattern_match.get("database", None),
+            host=address_match.get("host", None),
+            port=int(address_match.get("port", None)),
+            schema=data.get("database", None),
             username=data.get("user", None),
             password=data.get("password", None),
         )
 
     @property
+    def type(self) -> str:
+        """Property datasource type."""
+        return self.type_.getDescp()
+
+    @property
+    def type_code(self) -> str:
+        """Property datasource type."""
+        return self.type_.getCode()
+
+    @property
     def host(self) -> str:
         """Property datasource host, such as ``127.0.0.1`` or ``localhosts``."""
         return self.connection.host
 
     @property
     def port(self) -> int:
         """Property datasource host, such as ``3306`` or ``5432``."""
```

### Comparing `apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/models/meta.py` & `apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/models/meta.py`

 * *Files identical despite different names*

### Comparing `apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/models/project.py` & `apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/models/project.py`

 * *Files identical despite different names*

### Comparing `apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/models/queue.py` & `apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/models/queue.py`

 * *Files identical despite different names*

### Comparing `apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/models/tenant.py` & `apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/models/tenant.py`

 * *Files identical despite different names*

### Comparing `apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/models/user.py` & `apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/models/user.py`

 * *Files identical despite different names*

### Comparing `apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/models/worker_group.py` & `apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/models/worker_group.py`

 * *Files identical despite different names*

### Comparing `apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/resources_plugin/__init__.py` & `apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/resources_plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/resources_plugin/base/__init__.py` & `apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/resources_plugin/base/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/resources_plugin/base/bucket.py` & `apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/resources_plugin/base/bucket.py`

 * *Files identical despite different names*

### Comparing `apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/resources_plugin/base/git.py` & `apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/resources_plugin/base/git.py`

 * *Files identical despite different names*

### Comparing `apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/resources_plugin/github.py` & `apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/resources_plugin/github.py`

 * *Files identical despite different names*

### Comparing `apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/resources_plugin/gitlab.py` & `apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/resources_plugin/gitlab.py`

 * *Files identical despite different names*

### Comparing `apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/resources_plugin/local.py` & `apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/resources_plugin/local.py`

 * *Files identical despite different names*

### Comparing `apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/resources_plugin/oss.py` & `apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/resources_plugin/oss.py`

 * *Files identical despite different names*

### Comparing `apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/resources_plugin/s3.py` & `apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/resources_plugin/s3.py`

 * *Files identical despite different names*

### Comparing `apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/tasks/__init__.py` & `apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/tasks/condition.py` & `apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/tasks/condition.py`

 * *Files identical despite different names*

### Comparing `apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/tasks/datax.py` & `apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/tasks/datax.py`

 * *Files 22% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 """Task datax."""
-import json as json_pkg
+
 from typing import Dict, List, Optional
 
 from pydolphinscheduler.constants import TaskType
 from pydolphinscheduler.core.task import Task
 from pydolphinscheduler.models.datasource import Datasource
 
 
@@ -36,21 +36,21 @@
 
     ext: set = {".json"}
     ext_attr: str = "_json"
 
     def __init__(
         self,
         name: str,
-        config: dict,
+        json: str,
         xms: Optional[int] = 1,
         xmx: Optional[int] = 1,
         *args,
         **kwargs
     ):
-        self._json = json_pkg.dumps(config, indent=2)
+        self._json = json
         super().__init__(name, TaskType.DATAX, *args, **kwargs)
         self.custom_config = self.CUSTOM_CONFIG
         self.xms = xms
         self.xmx = xmx
 
 
 class DataX(Task):
@@ -94,49 +94,57 @@
     def __init__(
         self,
         name: str,
         datasource_name: str,
         datatarget_name: str,
         sql: str,
         target_table: str,
+        datasource_type: Optional[str] = None,
+        datatarget_type: Optional[str] = None,
         job_speed_byte: Optional[int] = 0,
         job_speed_record: Optional[int] = 1000,
         pre_statements: Optional[List[str]] = None,
         post_statements: Optional[List[str]] = None,
         xms: Optional[int] = 1,
         xmx: Optional[int] = 1,
         *args,
         **kwargs
     ):
         self._sql = sql
         super().__init__(name, TaskType.DATAX, *args, **kwargs)
         self.custom_config = self.CUSTOM_CONFIG
+        self.datasource_type = datasource_type
         self.datasource_name = datasource_name
+        self.datatarget_type = datatarget_type
         self.datatarget_name = datatarget_name
         self.target_table = target_table
         self.job_speed_byte = job_speed_byte
         self.job_speed_record = job_speed_record
         self.pre_statements = pre_statements or []
         self.post_statements = post_statements or []
         self.xms = xms
         self.xmx = xmx
 
     @property
     def source_params(self) -> Dict:
         """Get source params for datax task."""
-        datasource_task_u = Datasource.get_task_usage_4j(self.datasource_name)
+        datasource_task_u = Datasource.get_task_usage_4j(
+            self.datasource_name, self.datasource_type
+        )
         return {
             "dsType": datasource_task_u.type,
             "dataSource": datasource_task_u.id,
         }
 
     @property
     def target_params(self) -> Dict:
         """Get target params for datax task."""
-        datasource_task_u = Datasource.get_task_usage_4j(self.datatarget_name)
+        datasource_task_u = Datasource.get_task_usage_4j(
+            self.datatarget_name, self.datatarget_type
+        )
         return {
             "dtType": datasource_task_u.type,
             "dataTarget": datasource_task_u.id,
         }
 
     @property
     def task_params(self, camel_attr: bool = True, custom_attr: set = None) -> Dict:
```

### Comparing `apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/tasks/dependent.py` & `apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/tasks/dependent.py`

 * *Files identical despite different names*

### Comparing `apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/tasks/dvc.py` & `apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/tasks/dvc.py`

 * *Files identical despite different names*

### Comparing `apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/tasks/flink.py` & `apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/tasks/flink.py`

 * *Files identical despite different names*

### Comparing `apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/tasks/func_wrap.py` & `apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/tasks/func_wrap.py`

 * *Files identical despite different names*

### Comparing `apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/tasks/http.py` & `apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/tasks/http.py`

 * *Files identical despite different names*

### Comparing `apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/tasks/kubernetes.py` & `apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/tasks/kubernetes.py`

 * *Files identical despite different names*

### Comparing `apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/tasks/map_reduce.py` & `apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/tasks/map_reduce.py`

 * *Files identical despite different names*

### Comparing `apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/tasks/mlflow.py` & `apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/tasks/mlflow.py`

 * *Files identical despite different names*

### Comparing `apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/tasks/openmldb.py` & `apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/tasks/openmldb.py`

 * *Files identical despite different names*

### Comparing `apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/tasks/procedure.py` & `apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/tasks/procedure.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 """Task procedure."""
 
-from typing import Dict
+from typing import Dict, Optional
 
 from pydolphinscheduler.constants import TaskType
 from pydolphinscheduler.core.task import Task
 from pydolphinscheduler.models.datasource import Datasource
 
 
 class Procedure(Task):
@@ -38,23 +38,34 @@
     - SQLServer
     You provider datasource_name contain connection information, it decisions which
     database type and database instance would run this sql.
     """
 
     _task_custom_attr = {"method"}
 
-    def __init__(self, name: str, datasource_name: str, method: str, *args, **kwargs):
+    def __init__(
+        self,
+        name: str,
+        datasource_name: str,
+        method: str,
+        datasource_type: Optional[str] = None,
+        *args,
+        **kwargs
+    ):
         super().__init__(name, TaskType.PROCEDURE, *args, **kwargs)
         self.datasource_name = datasource_name
+        self.datasource_type = datasource_type
         self.method = method
 
     @property
     def datasource(self) -> Dict:
         """Get datasource for procedure task."""
-        datasource_task_u = Datasource.get_task_usage_4j(self.datasource_name)
+        datasource_task_u = Datasource.get_task_usage_4j(
+            self.datasource_name, self.datasource_type
+        )
         return {
             "datasource": datasource_task_u.id,
             "type": datasource_task_u.type,
         }
 
     @property
     def task_params(self, camel_attr: bool = True, custom_attr: set = None) -> Dict:
```

### Comparing `apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/tasks/pytorch.py` & `apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/tasks/pytorch.py`

 * *Files identical despite different names*

### Comparing `apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/tasks/sagemaker.py` & `apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/tasks/sagemaker.py`

 * *Files identical despite different names*

### Comparing `apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/tasks/spark.py` & `apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/tasks/spark.py`

 * *Files identical despite different names*

### Comparing `apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/tasks/sql.py` & `apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/tasks/sql.py`

 * *Files 5% similar despite different names*

```diff
@@ -75,25 +75,27 @@
     ext_attr: str = "_sql"
 
     def __init__(
         self,
         name: str,
         datasource_name: str,
         sql: str,
+        datasource_type: Optional[str] = None,
         sql_type: Optional[str] = None,
         pre_statements: Union[str, Sequence[str], None] = None,
         post_statements: Union[str, Sequence[str], None] = None,
         display_rows: Optional[int] = 10,
         *args,
         **kwargs
     ):
         self._sql = sql
         super().__init__(name, TaskType.SQL, *args, **kwargs)
         self.param_sql_type = sql_type
         self.datasource_name = datasource_name
+        self.datasource_type = datasource_type
         self.pre_statements = self.get_stm_list(pre_statements)
         self.post_statements = self.get_stm_list(post_statements)
         self.display_rows = display_rows
 
     @staticmethod
     def get_stm_list(stm: Union[str, Sequence[str]]) -> List[str]:
         """Convert statement to str of list.
@@ -133,15 +135,17 @@
             return SqlType.NOT_SELECT
         else:
             return SqlType.SELECT
 
     @property
     def datasource(self) -> Dict:
         """Get datasource for procedure sql."""
-        datasource_task_u = Datasource.get_task_usage_4j(self.datasource_name)
+        datasource_task_u = Datasource.get_task_usage_4j(
+            self.datasource_name, self.datasource_type
+        )
         return {
             "datasource": datasource_task_u.id,
             "type": datasource_task_u.type,
         }
 
     @property
     def task_params(self, camel_attr: bool = True, custom_attr: set = None) -> Dict:
```

### Comparing `apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/tasks/sub_process.py` & `apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/tasks/sub_process.py`

 * *Files identical despite different names*

### Comparing `apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/tasks/sub_workflow.py` & `apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/tasks/sub_workflow.py`

 * *Files identical despite different names*

### Comparing `apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/tasks/switch.py` & `apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/tasks/switch.py`

 * *Files identical despite different names*

### Comparing `apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/utils/__init__.py` & `apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/utils/date.py` & `apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/utils/date.py`

 * *Files identical despite different names*

### Comparing `apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/utils/file.py` & `apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/utils/file.py`

 * *Files identical despite different names*

### Comparing `apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/utils/string.py` & `apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/utils/string.py`

 * *Files identical despite different names*

### Comparing `apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/utils/versions.py` & `apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/utils/versions.py`

 * *Files identical despite different names*

### Comparing `apache-dolphinscheduler-4.0.2a9/src/pydolphinscheduler/utils/yaml_parser.py` & `apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/utils/yaml_parser.py`

 * *Files identical despite different names*

### Comparing `apache-dolphinscheduler-4.0.2a9/tests/test_configuration.py` & `apache-dolphinscheduler-4.0.3/tests/test_configuration.py`

 * *Files identical despite different names*

### Comparing `apache-dolphinscheduler-4.0.2a9/tests/test_docs.py` & `apache-dolphinscheduler-4.0.3/tests/test_docs.py`

 * *Files identical despite different names*

