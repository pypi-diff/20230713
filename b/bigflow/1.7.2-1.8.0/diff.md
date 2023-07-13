# Comparing `tmp/bigflow-1.7.2.tar.gz` & `tmp/bigflow-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bigflow-1.7.2.tar", last modified: Wed May 17 20:06:08 2023, max compression
+gzip compressed data, was "bigflow-1.8.0.tar", last modified: Thu Jul 13 06:45:08 2023, max compression
```

## Comparing `bigflow-1.7.2.tar` & `bigflow-1.8.0.tar`

### file list

```diff
@@ -1,151 +1,151 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:06:08.810688 bigflow-1.7.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11896 2023-05-17 20:05:12.000000 bigflow-1.7.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-17 20:05:12.000000 bigflow-1.7.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-05-17 20:05:12.000000 bigflow-1.7.2/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-05-17 20:06:08.810688 bigflow-1.7.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-05-17 20:05:12.000000 bigflow-1.7.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:06:08.798688 bigflow-1.7.2/bigflow/
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-05-17 20:05:12.000000 bigflow-1.7.2/bigflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-17 20:05:12.000000 bigflow-1.7.2/bigflow/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-17 20:05:12.000000 bigflow-1.7.2/bigflow/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:06:08.798688 bigflow-1.7.2/bigflow/bigquery/
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-05-17 20:05:12.000000 bigflow-1.7.2/bigflow/bigquery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4366 2023-05-17 20:05:12.000000 bigflow-1.7.2/bigflow/bigquery/dataset_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)    20401 2023-05-17 20:05:12.000000 bigflow-1.7.2/bigflow/bigquery/dataset_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    21110 2023-05-17 20:05:12.000000 bigflow-1.7.2/bigflow/bigquery/interactive.py
--rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-05-17 20:05:12.000000 bigflow-1.7.2/bigflow/bigquery/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-05-17 20:05:12.000000 bigflow-1.7.2/bigflow/bigquery/job.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:06:08.802688 bigflow-1.7.2/bigflow/build/
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-17 20:05:12.000000 bigflow-1.7.2/bigflow/build/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:06:08.802688 bigflow-1.7.2/bigflow/build/dataflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 20:05:12.000000 bigflow-1.7.2/bigflow/build/dataflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4256 2023-05-17 20:05:12.000000 bigflow-1.7.2/bigflow/build/dev.py
--rw-r--r--   0 runner    (1001) docker     (123)     7920 2023-05-17 20:05:12.000000 bigflow-1.7.2/bigflow/build/dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-05-17 20:05:12.000000 bigflow-1.7.2/bigflow/build/legacy.py
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-17 20:05:12.000000 bigflow-1.7.2/bigflow/build/meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     9569 2023-05-17 20:05:12.000000 bigflow-1.7.2/bigflow/build/operate.py
--rw-r--r--   0 runner    (1001) docker     (123)     8774 2023-05-17 20:05:12.000000 bigflow-1.7.2/bigflow/build/pip.py
--rw-r--r--   0 runner    (1001) docker     (123)     8416 2023-05-17 20:05:12.000000 bigflow-1.7.2/bigflow/build/reflect.py
--rw-r--r--   0 runner    (1001) docker     (123)     9156 2023-05-17 20:05:12.000000 bigflow-1.7.2/bigflow/build/spec.py
--rw-r--r--   0 runner    (1001) docker     (123)    35088 2023-05-17 20:05:12.000000 bigflow-1.7.2/bigflow/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     9815 2023-05-17 20:05:12.000000 bigflow-1.7.2/bigflow/commons.py
--rw-r--r--   0 runner    (1001) docker     (123)     4841 2023-05-17 20:05:12.000000 bigflow-1.7.2/bigflow/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     6458 2023-05-17 20:05:12.000000 bigflow-1.7.2/bigflow/dagbuilder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:06:08.802688 bigflow-1.7.2/bigflow/dataflow/
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-17 20:05:12.000000 bigflow-1.7.2/bigflow/dataflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-05-17 20:05:12.000000 bigflow-1.7.2/bigflow/dataflow/io.py
--rw-r--r--   0 runner    (1001) docker     (123)    10006 2023-05-17 20:05:12.000000 bigflow-1.7.2/bigflow/dataflow/job.py
--rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-05-17 20:05:12.000000 bigflow-1.7.2/bigflow/dataflow/ml.py
--rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-05-17 20:05:12.000000 bigflow-1.7.2/bigflow/dataflow/options.py
--rw-r--r--   0 runner    (1001) docker     (123)    10332 2023-05-17 20:05:12.000000 bigflow-1.7.2/bigflow/deploy.py
--rw-r--r--   0 runner    (1001) docker     (123)     9180 2023-05-17 20:05:12.000000 bigflow-1.7.2/bigflow/konfig.py
--rw-r--r--   0 runner    (1001) docker     (123)     4158 2023-05-17 20:05:12.000000 bigflow-1.7.2/bigflow/migrate.py
--rw-r--r--   0 runner    (1001) docker     (123)     4940 2023-05-17 20:05:12.000000 bigflow-1.7.2/bigflow/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:06:08.802688 bigflow-1.7.2/bigflow/scaffold/
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-17 20:05:12.000000 bigflow-1.7.2/bigflow/scaffold/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6765 2023-05-17 20:05:12.000000 bigflow-1.7.2/bigflow/scaffold/infra.py
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-05-17 20:05:12.000000 bigflow-1.7.2/bigflow/scaffold/scaffold.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:06:08.802688 bigflow-1.7.2/bigflow/scaffold/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-05-17 20:05:12.000000 bigflow-1.7.2/bigflow/scaffold/templates/README.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:06:08.802688 bigflow-1.7.2/bigflow/scaffold/templates/migrate-11/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-17 20:05:12.000000 bigflow-1.7.2/bigflow/scaffold/templates/migrate-11/pyproject.toml.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:06:08.802688 bigflow-1.7.2/bigflow/scaffold/templates/new-project/
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-05-17 20:05:12.000000 bigflow-1.7.2/bigflow/scaffold/templates/new-project/.gitignore.j2
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-05-17 20:05:12.000000 bigflow-1.7.2/bigflow/scaffold/templates/new-project/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-05-17 20:05:12.000000 bigflow-1.7.2/bigflow/scaffold/templates/new-project/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-05-17 20:05:12.000000 bigflow-1.7.2/bigflow/scaffold/templates/new-project/deployment_config.py.j2
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-17 20:05:12.000000 bigflow-1.7.2/bigflow/scaffold/templates/new-project/pyproject.toml.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:06:08.802688 bigflow-1.7.2/bigflow/scaffold/templates/new-project/resources/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-17 20:05:12.000000 bigflow-1.7.2/bigflow/scaffold/templates/new-project/resources/requirements.in.j2
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-17 20:05:12.000000 bigflow-1.7.2/bigflow/scaffold/templates/new-project/setup.py.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:06:08.802688 bigflow-1.7.2/bigflow/scaffold/templates/new-project/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 20:05:12.000000 bigflow-1.7.2/bigflow/scaffold/templates/new-project/test/__init__.py.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:06:08.802688 bigflow-1.7.2/bigflow/scaffold/templates/new-project/test/pi_estimator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 20:05:12.000000 bigflow-1.7.2/bigflow/scaffold/templates/new-project/test/pi_estimator/__init__.py.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-05-17 20:05:12.000000 bigflow-1.7.2/bigflow/scaffold/templates/new-project/test/pi_estimator/test_processing.py.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-05-17 20:05:12.000000 bigflow-1.7.2/bigflow/scaffold/templates/new-project/test/test_wordcount_workflow.py.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:06:08.802688 bigflow-1.7.2/bigflow/scaffold/templates/new-project/{{project_name}}/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 20:05:12.000000 bigflow-1.7.2/bigflow/scaffold/templates/new-project/{{project_name}}/__init__.py.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:06:08.806688 bigflow-1.7.2/bigflow/scaffold/templates/new-project/{{project_name}}/internationalports/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 20:05:12.000000 bigflow-1.7.2/bigflow/scaffold/templates/new-project/{{project_name}}/internationalports/__init__.py.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-05-17 20:05:12.000000 bigflow-1.7.2/bigflow/scaffold/templates/new-project/{{project_name}}/internationalports/workflow.py.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:06:08.806688 bigflow-1.7.2/bigflow/scaffold/templates/new-project/{{project_name}}/pi_estimator/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-17 20:05:12.000000 bigflow-1.7.2/bigflow/scaffold/templates/new-project/{{project_name}}/pi_estimator/__init__.py.j2
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-05-17 20:05:12.000000 bigflow-1.7.2/bigflow/scaffold/templates/new-project/{{project_name}}/pi_estimator/config.py.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-05-17 20:05:12.000000 bigflow-1.7.2/bigflow/scaffold/templates/new-project/{{project_name}}/pi_estimator/processing.py.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-05-17 20:05:12.000000 bigflow-1.7.2/bigflow/scaffold/templates/new-project/{{project_name}}/pi_estimator/workflow.py.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:06:08.806688 bigflow-1.7.2/bigflow/scaffold/templates/new-project/{{project_name}}/wordcount/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 20:05:12.000000 bigflow-1.7.2/bigflow/scaffold/templates/new-project/{{project_name}}/wordcount/__init__.py.j2
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-05-17 20:05:12.000000 bigflow-1.7.2/bigflow/scaffold/templates/new-project/{{project_name}}/wordcount/pipeline.py.j2
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-05-17 20:05:12.000000 bigflow-1.7.2/bigflow/scaffold/templates/new-project/{{project_name}}/wordcount/processing.py.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-05-17 20:05:12.000000 bigflow-1.7.2/bigflow/scaffold/templates/new-project/{{project_name}}/wordcount/workflow.py.j2
--rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-05-17 20:05:12.000000 bigflow-1.7.2/bigflow/scaffold/templating.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:06:08.806688 bigflow-1.7.2/bigflow/testing/
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-05-17 20:05:12.000000 bigflow-1.7.2/bigflow/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8644 2023-05-17 20:05:12.000000 bigflow-1.7.2/bigflow/testing/isolate.py
--rw-r--r--   0 runner    (1001) docker     (123)     5200 2023-05-17 20:05:12.000000 bigflow-1.7.2/bigflow/version.py
--rw-r--r--   0 runner    (1001) docker     (123)    13756 2023-05-17 20:05:12.000000 bigflow-1.7.2/bigflow/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:06:08.798688 bigflow-1.7.2/bigflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-05-17 20:06:08.000000 bigflow-1.7.2/bigflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-05-17 20:06:08.000000 bigflow-1.7.2/bigflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 20:06:08.000000 bigflow-1.7.2/bigflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-05-17 20:06:08.000000 bigflow-1.7.2/bigflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-17 20:06:08.000000 bigflow-1.7.2/bigflow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-17 20:05:12.000000 bigflow-1.7.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:06:08.806688 bigflow-1.7.2/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-17 20:05:12.000000 bigflow-1.7.2/scripts/bf
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-17 20:05:12.000000 bigflow-1.7.2/scripts/bigflow
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 20:06:08.810688 bigflow-1.7.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-05-17 20:05:12.000000 bigflow-1.7.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:06:08.806688 bigflow-1.7.2/test/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:06:08.806688 bigflow-1.7.2/test/buildd/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 20:05:12.000000 bigflow-1.7.2/test/buildd/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:06:08.810688 bigflow-1.7.2/test/buildd/dataflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 20:05:12.000000 bigflow-1.7.2/test/buildd/dataflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-05-17 20:05:12.000000 bigflow-1.7.2/test/buildd/test_dev.py
--rw-r--r--   0 runner    (1001) docker     (123)    12099 2023-05-17 20:05:12.000000 bigflow-1.7.2/test/buildd/test_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     5108 2023-05-17 20:05:12.000000 bigflow-1.7.2/test/buildd/test_operate.py
--rw-r--r--   0 runner    (1001) docker     (123)     4207 2023-05-17 20:05:12.000000 bigflow-1.7.2/test/buildd/test_pip.py
--rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-05-17 20:05:12.000000 bigflow-1.7.2/test/buildd/test_reflect.py
--rw-r--r--   0 runner    (1001) docker     (123)     4957 2023-05-17 20:05:12.000000 bigflow-1.7.2/test/buildd/test_spec.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:06:08.810688 bigflow-1.7.2/test/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 20:05:12.000000 bigflow-1.7.2/test/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:06:08.810688 bigflow-1.7.2/test/cli/cli_logs_duplicated_workflows/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 20:05:12.000000 bigflow-1.7.2/test/cli/cli_logs_duplicated_workflows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-05-17 20:05:12.000000 bigflow-1.7.2/test/cli/cli_logs_duplicated_workflows/workflows.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:06:08.810688 bigflow-1.7.2/test/cli/cli_logs_log_name_workflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 20:05:12.000000 bigflow-1.7.2/test/cli/cli_logs_log_name_workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-17 20:05:12.000000 bigflow-1.7.2/test/cli/cli_logs_log_name_workflow/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:06:08.810688 bigflow-1.7.2/test/cli/cli_logs_regular_workflows/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 20:05:12.000000 bigflow-1.7.2/test/cli/cli_logs_regular_workflows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-05-17 20:05:12.000000 bigflow-1.7.2/test/cli/cli_logs_regular_workflows/workflows.py
--rw-r--r--   0 runner    (1001) docker     (123)    41823 2023-05-17 20:05:12.000000 bigflow-1.7.2/test/cli/test_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:06:08.810688 bigflow-1.7.2/test/cli/test_module/
--rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-05-17 20:05:12.000000 bigflow-1.7.2/test/cli/test_module/Unused1.py
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-17 20:05:12.000000 bigflow-1.7.2/test/cli/test_module/Unused2.py
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-17 20:05:12.000000 bigflow-1.7.2/test/cli/test_module/Unused3.py
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-17 20:05:12.000000 bigflow-1.7.2/test/cli/test_module/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:06:08.810688 bigflow-1.7.2/test/dagbuilder/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 20:05:12.000000 bigflow-1.7.2/test/dagbuilder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6116 2023-05-17 20:05:12.000000 bigflow-1.7.2/test/dagbuilder/test_dagbuilder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2577 2023-05-17 20:05:12.000000 bigflow-1.7.2/test/test_commons.py
--rw-r--r--   0 runner    (1001) docker     (123)    12127 2023-05-17 20:05:12.000000 bigflow-1.7.2/test/test_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)    16480 2023-05-17 20:05:12.000000 bigflow-1.7.2/test/test_dataflow.py
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-17 20:05:12.000000 bigflow-1.7.2/test/test_dataset_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    13497 2023-05-17 20:05:12.000000 bigflow-1.7.2/test/test_deploy.py
--rw-r--r--   0 runner    (1001) docker     (123)    23905 2023-05-17 20:05:12.000000 bigflow-1.7.2/test/test_interactive.py
--rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-05-17 20:05:12.000000 bigflow-1.7.2/test/test_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     8869 2023-05-17 20:05:12.000000 bigflow-1.7.2/test/test_konfig.py
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-05-17 20:05:12.000000 bigflow-1.7.2/test/test_migrate.py
--rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-05-17 20:05:12.000000 bigflow-1.7.2/test/test_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)    13548 2023-05-17 20:05:12.000000 bigflow-1.7.2/test/test_scaffold.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:06:08.810688 bigflow-1.7.2/test/test_user_commons/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 20:05:12.000000 bigflow-1.7.2/test/test_user_commons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-05-17 20:05:12.000000 bigflow-1.7.2/test/test_user_commons/test_labels.py
--rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-05-17 20:05:12.000000 bigflow-1.7.2/test/test_user_commons/test_sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4035 2023-05-17 20:05:12.000000 bigflow-1.7.2/test/test_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     8607 2023-05-17 20:05:12.000000 bigflow-1.7.2/test/test_workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:06:08.810688 bigflow-1.7.2/test/testing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 20:05:12.000000 bigflow-1.7.2/test/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-17 20:05:12.000000 bigflow-1.7.2/test/testing/nonpure.py
--rw-r--r--   0 runner    (1001) docker     (123)     4586 2023-05-17 20:05:12.000000 bigflow-1.7.2/test/testing/test_isolate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:45:08.158999 bigflow-1.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11896 2023-07-13 06:44:09.000000 bigflow-1.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-13 06:44:09.000000 bigflow-1.8.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-07-13 06:44:09.000000 bigflow-1.8.0/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-07-13 06:45:08.158999 bigflow-1.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-07-13 06:44:09.000000 bigflow-1.8.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:45:08.146999 bigflow-1.8.0/bigflow/
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-07-13 06:44:09.000000 bigflow-1.8.0/bigflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-13 06:44:09.000000 bigflow-1.8.0/bigflow/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-13 06:44:09.000000 bigflow-1.8.0/bigflow/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:45:08.146999 bigflow-1.8.0/bigflow/bigquery/
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-07-13 06:44:09.000000 bigflow-1.8.0/bigflow/bigquery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4366 2023-07-13 06:44:09.000000 bigflow-1.8.0/bigflow/bigquery/dataset_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20401 2023-07-13 06:44:09.000000 bigflow-1.8.0/bigflow/bigquery/dataset_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21110 2023-07-13 06:44:09.000000 bigflow-1.8.0/bigflow/bigquery/interactive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-07-13 06:44:09.000000 bigflow-1.8.0/bigflow/bigquery/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-07-13 06:44:09.000000 bigflow-1.8.0/bigflow/bigquery/job.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:45:08.146999 bigflow-1.8.0/bigflow/build/
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-13 06:44:09.000000 bigflow-1.8.0/bigflow/build/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:45:08.146999 bigflow-1.8.0/bigflow/build/dataflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:44:09.000000 bigflow-1.8.0/bigflow/build/dataflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4256 2023-07-13 06:44:09.000000 bigflow-1.8.0/bigflow/build/dev.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7920 2023-07-13 06:44:09.000000 bigflow-1.8.0/bigflow/build/dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-07-13 06:44:09.000000 bigflow-1.8.0/bigflow/build/legacy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-13 06:44:09.000000 bigflow-1.8.0/bigflow/build/meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9569 2023-07-13 06:44:09.000000 bigflow-1.8.0/bigflow/build/operate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8774 2023-07-13 06:44:09.000000 bigflow-1.8.0/bigflow/build/pip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8416 2023-07-13 06:44:09.000000 bigflow-1.8.0/bigflow/build/reflect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9156 2023-07-13 06:44:09.000000 bigflow-1.8.0/bigflow/build/spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35088 2023-07-13 06:44:09.000000 bigflow-1.8.0/bigflow/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9815 2023-07-13 06:44:09.000000 bigflow-1.8.0/bigflow/commons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4841 2023-07-13 06:44:09.000000 bigflow-1.8.0/bigflow/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6514 2023-07-13 06:44:09.000000 bigflow-1.8.0/bigflow/dagbuilder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:45:08.150999 bigflow-1.8.0/bigflow/dataflow/
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-07-13 06:44:09.000000 bigflow-1.8.0/bigflow/dataflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-07-13 06:44:09.000000 bigflow-1.8.0/bigflow/dataflow/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10006 2023-07-13 06:44:09.000000 bigflow-1.8.0/bigflow/dataflow/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-07-13 06:44:09.000000 bigflow-1.8.0/bigflow/dataflow/ml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-07-13 06:44:09.000000 bigflow-1.8.0/bigflow/dataflow/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10332 2023-07-13 06:44:09.000000 bigflow-1.8.0/bigflow/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9180 2023-07-13 06:44:09.000000 bigflow-1.8.0/bigflow/konfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4158 2023-07-13 06:44:09.000000 bigflow-1.8.0/bigflow/migrate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4940 2023-07-13 06:44:09.000000 bigflow-1.8.0/bigflow/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:45:08.150999 bigflow-1.8.0/bigflow/scaffold/
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-07-13 06:44:09.000000 bigflow-1.8.0/bigflow/scaffold/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6765 2023-07-13 06:44:09.000000 bigflow-1.8.0/bigflow/scaffold/infra.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-07-13 06:44:09.000000 bigflow-1.8.0/bigflow/scaffold/scaffold.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:45:08.150999 bigflow-1.8.0/bigflow/scaffold/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-07-13 06:44:09.000000 bigflow-1.8.0/bigflow/scaffold/templates/README.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:45:08.150999 bigflow-1.8.0/bigflow/scaffold/templates/migrate-11/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-13 06:44:09.000000 bigflow-1.8.0/bigflow/scaffold/templates/migrate-11/pyproject.toml.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:45:08.150999 bigflow-1.8.0/bigflow/scaffold/templates/new-project/
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-07-13 06:44:09.000000 bigflow-1.8.0/bigflow/scaffold/templates/new-project/.gitignore.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-07-13 06:44:09.000000 bigflow-1.8.0/bigflow/scaffold/templates/new-project/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-07-13 06:44:09.000000 bigflow-1.8.0/bigflow/scaffold/templates/new-project/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-07-13 06:44:09.000000 bigflow-1.8.0/bigflow/scaffold/templates/new-project/deployment_config.py.j2
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-13 06:44:09.000000 bigflow-1.8.0/bigflow/scaffold/templates/new-project/pyproject.toml.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:45:08.150999 bigflow-1.8.0/bigflow/scaffold/templates/new-project/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-13 06:44:09.000000 bigflow-1.8.0/bigflow/scaffold/templates/new-project/resources/requirements.in.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-13 06:44:09.000000 bigflow-1.8.0/bigflow/scaffold/templates/new-project/setup.py.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:45:08.150999 bigflow-1.8.0/bigflow/scaffold/templates/new-project/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:44:09.000000 bigflow-1.8.0/bigflow/scaffold/templates/new-project/test/__init__.py.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:45:08.150999 bigflow-1.8.0/bigflow/scaffold/templates/new-project/test/pi_estimator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:44:09.000000 bigflow-1.8.0/bigflow/scaffold/templates/new-project/test/pi_estimator/__init__.py.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-07-13 06:44:09.000000 bigflow-1.8.0/bigflow/scaffold/templates/new-project/test/pi_estimator/test_processing.py.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-07-13 06:44:09.000000 bigflow-1.8.0/bigflow/scaffold/templates/new-project/test/test_wordcount_workflow.py.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:45:08.150999 bigflow-1.8.0/bigflow/scaffold/templates/new-project/{{project_name}}/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:44:09.000000 bigflow-1.8.0/bigflow/scaffold/templates/new-project/{{project_name}}/__init__.py.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:45:08.150999 bigflow-1.8.0/bigflow/scaffold/templates/new-project/{{project_name}}/internationalports/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:44:09.000000 bigflow-1.8.0/bigflow/scaffold/templates/new-project/{{project_name}}/internationalports/__init__.py.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-07-13 06:44:09.000000 bigflow-1.8.0/bigflow/scaffold/templates/new-project/{{project_name}}/internationalports/workflow.py.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:45:08.150999 bigflow-1.8.0/bigflow/scaffold/templates/new-project/{{project_name}}/pi_estimator/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-13 06:44:09.000000 bigflow-1.8.0/bigflow/scaffold/templates/new-project/{{project_name}}/pi_estimator/__init__.py.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-13 06:44:09.000000 bigflow-1.8.0/bigflow/scaffold/templates/new-project/{{project_name}}/pi_estimator/config.py.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-07-13 06:44:09.000000 bigflow-1.8.0/bigflow/scaffold/templates/new-project/{{project_name}}/pi_estimator/processing.py.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-07-13 06:44:09.000000 bigflow-1.8.0/bigflow/scaffold/templates/new-project/{{project_name}}/pi_estimator/workflow.py.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:45:08.150999 bigflow-1.8.0/bigflow/scaffold/templates/new-project/{{project_name}}/wordcount/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:44:09.000000 bigflow-1.8.0/bigflow/scaffold/templates/new-project/{{project_name}}/wordcount/__init__.py.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-07-13 06:44:09.000000 bigflow-1.8.0/bigflow/scaffold/templates/new-project/{{project_name}}/wordcount/pipeline.py.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-07-13 06:44:09.000000 bigflow-1.8.0/bigflow/scaffold/templates/new-project/{{project_name}}/wordcount/processing.py.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-07-13 06:44:09.000000 bigflow-1.8.0/bigflow/scaffold/templates/new-project/{{project_name}}/wordcount/workflow.py.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-07-13 06:44:09.000000 bigflow-1.8.0/bigflow/scaffold/templating.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:45:08.154999 bigflow-1.8.0/bigflow/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 06:44:09.000000 bigflow-1.8.0/bigflow/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8644 2023-07-13 06:44:09.000000 bigflow-1.8.0/bigflow/testing/isolate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5200 2023-07-13 06:44:09.000000 bigflow-1.8.0/bigflow/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13832 2023-07-13 06:44:09.000000 bigflow-1.8.0/bigflow/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:45:08.146999 bigflow-1.8.0/bigflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-07-13 06:45:08.000000 bigflow-1.8.0/bigflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-07-13 06:45:08.000000 bigflow-1.8.0/bigflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 06:45:08.000000 bigflow-1.8.0/bigflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-07-13 06:45:08.000000 bigflow-1.8.0/bigflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-13 06:45:08.000000 bigflow-1.8.0/bigflow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-13 06:44:09.000000 bigflow-1.8.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:45:08.154999 bigflow-1.8.0/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-13 06:44:09.000000 bigflow-1.8.0/scripts/bf
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-13 06:44:09.000000 bigflow-1.8.0/scripts/bigflow
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 06:45:08.158999 bigflow-1.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-07-13 06:44:09.000000 bigflow-1.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:45:08.154999 bigflow-1.8.0/test/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:45:08.154999 bigflow-1.8.0/test/buildd/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:44:09.000000 bigflow-1.8.0/test/buildd/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:45:08.154999 bigflow-1.8.0/test/buildd/dataflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:44:09.000000 bigflow-1.8.0/test/buildd/dataflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-07-13 06:44:09.000000 bigflow-1.8.0/test/buildd/test_dev.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12099 2023-07-13 06:44:09.000000 bigflow-1.8.0/test/buildd/test_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5108 2023-07-13 06:44:09.000000 bigflow-1.8.0/test/buildd/test_operate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4207 2023-07-13 06:44:09.000000 bigflow-1.8.0/test/buildd/test_pip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-07-13 06:44:09.000000 bigflow-1.8.0/test/buildd/test_reflect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4957 2023-07-13 06:44:09.000000 bigflow-1.8.0/test/buildd/test_spec.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:45:08.154999 bigflow-1.8.0/test/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:44:09.000000 bigflow-1.8.0/test/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:45:08.154999 bigflow-1.8.0/test/cli/cli_logs_duplicated_workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:44:09.000000 bigflow-1.8.0/test/cli/cli_logs_duplicated_workflows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-07-13 06:44:09.000000 bigflow-1.8.0/test/cli/cli_logs_duplicated_workflows/workflows.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:45:08.154999 bigflow-1.8.0/test/cli/cli_logs_log_name_workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:44:09.000000 bigflow-1.8.0/test/cli/cli_logs_log_name_workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-13 06:44:09.000000 bigflow-1.8.0/test/cli/cli_logs_log_name_workflow/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:45:08.154999 bigflow-1.8.0/test/cli/cli_logs_regular_workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:44:09.000000 bigflow-1.8.0/test/cli/cli_logs_regular_workflows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-07-13 06:44:09.000000 bigflow-1.8.0/test/cli/cli_logs_regular_workflows/workflows.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41823 2023-07-13 06:44:09.000000 bigflow-1.8.0/test/cli/test_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:45:08.158999 bigflow-1.8.0/test/cli/test_module/
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-07-13 06:44:09.000000 bigflow-1.8.0/test/cli/test_module/Unused1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-13 06:44:09.000000 bigflow-1.8.0/test/cli/test_module/Unused2.py
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-13 06:44:09.000000 bigflow-1.8.0/test/cli/test_module/Unused3.py
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-13 06:44:09.000000 bigflow-1.8.0/test/cli/test_module/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:45:08.158999 bigflow-1.8.0/test/dagbuilder/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:44:09.000000 bigflow-1.8.0/test/dagbuilder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7496 2023-07-13 06:44:09.000000 bigflow-1.8.0/test/dagbuilder/test_dagbuilder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2577 2023-07-13 06:44:09.000000 bigflow-1.8.0/test/test_commons.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12127 2023-07-13 06:44:09.000000 bigflow-1.8.0/test/test_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16480 2023-07-13 06:44:09.000000 bigflow-1.8.0/test/test_dataflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-07-13 06:44:09.000000 bigflow-1.8.0/test/test_dataset_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13497 2023-07-13 06:44:09.000000 bigflow-1.8.0/test/test_deploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23905 2023-07-13 06:44:09.000000 bigflow-1.8.0/test/test_interactive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-07-13 06:44:09.000000 bigflow-1.8.0/test/test_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8869 2023-07-13 06:44:09.000000 bigflow-1.8.0/test/test_konfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-07-13 06:44:09.000000 bigflow-1.8.0/test/test_migrate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-07-13 06:44:09.000000 bigflow-1.8.0/test/test_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13548 2023-07-13 06:44:09.000000 bigflow-1.8.0/test/test_scaffold.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:45:08.158999 bigflow-1.8.0/test/test_user_commons/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:44:09.000000 bigflow-1.8.0/test/test_user_commons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-07-13 06:44:09.000000 bigflow-1.8.0/test/test_user_commons/test_labels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-07-13 06:44:09.000000 bigflow-1.8.0/test/test_user_commons/test_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4035 2023-07-13 06:44:09.000000 bigflow-1.8.0/test/test_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8607 2023-07-13 06:44:09.000000 bigflow-1.8.0/test/test_workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:45:08.158999 bigflow-1.8.0/test/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:44:09.000000 bigflow-1.8.0/test/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-13 06:44:09.000000 bigflow-1.8.0/test/testing/nonpure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4586 2023-07-13 06:44:09.000000 bigflow-1.8.0/test/testing/test_isolate.py
```

### Comparing `bigflow-1.7.2/LICENSE` & `bigflow-1.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.2/NOTICE` & `bigflow-1.8.0/NOTICE`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.2/PKG-INFO` & `bigflow-1.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bigflow
-Version: 1.7.2
+Version: 1.8.0
 Summary: BigQuery client wrapper with clean API
 Home-page: https://github.com/allegro/bigflow
 Author: Pogranicze
 Author-email: pogranicze-team@allegro.pl
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `bigflow-1.7.2/README.md` & `bigflow-1.8.0/README.md`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.2/bigflow/__init__.py` & `bigflow-1.8.0/bigflow/__init__.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.2/bigflow/bigquery/__init__.py` & `bigflow-1.8.0/bigflow/bigquery/__init__.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.2/bigflow/bigquery/dataset_configuration.py` & `bigflow-1.8.0/bigflow/bigquery/dataset_configuration.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.2/bigflow/bigquery/dataset_manager.py` & `bigflow-1.8.0/bigflow/bigquery/dataset_manager.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.2/bigflow/bigquery/interactive.py` & `bigflow-1.8.0/bigflow/bigquery/interactive.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.2/bigflow/bigquery/interface.py` & `bigflow-1.8.0/bigflow/bigquery/interface.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.2/bigflow/bigquery/job.py` & `bigflow-1.8.0/bigflow/bigquery/job.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.2/bigflow/build/dev.py` & `bigflow-1.8.0/bigflow/build/dev.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.2/bigflow/build/dist.py` & `bigflow-1.8.0/bigflow/build/dist.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.2/bigflow/build/legacy.py` & `bigflow-1.8.0/bigflow/build/legacy.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.2/bigflow/build/operate.py` & `bigflow-1.8.0/bigflow/build/operate.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.2/bigflow/build/pip.py` & `bigflow-1.8.0/bigflow/build/pip.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.2/bigflow/build/reflect.py` & `bigflow-1.8.0/bigflow/build/reflect.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.2/bigflow/build/spec.py` & `bigflow-1.8.0/bigflow/build/spec.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.2/bigflow/cli.py` & `bigflow-1.8.0/bigflow/cli.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.2/bigflow/commons.py` & `bigflow-1.8.0/bigflow/commons.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.2/bigflow/configuration.py` & `bigflow-1.8.0/bigflow/configuration.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.2/bigflow/dagbuilder.py` & `bigflow-1.8.0/bigflow/dagbuilder.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,14 +95,15 @@
 
         job = workflow_job.job
         job_var = f"t{job.id}"
         pod_operator_params_var = f"{job_var}_pod_operator_params"
         task_id = job.id.replace("_", "-")
         retries = getattr(job, 'retry_count', 3)
         bf_job = workflow.workflow_id + "." + job.id
+        env_var_name = workflow.env_variable
 
         if workflow.secrets:
             indent_prefix =  """\
                 """
             secrets_definitions = "".join(
                 f"{indent_prefix}    {secret_template(s)},\n"
                 for s in workflow.secrets
@@ -122,15 +123,15 @@
                 'task_id': {task_id!r},
                 'name': {task_id!r},
                 'cmds': ['python', '-m', 'bigflow', 'run'],
                 'arguments': [
                     '--job', {bf_job!r},
                     '--runtime', '{{{{ execution_date.strftime("%Y-%m-%d %H:%M:%S") }}}}',
                     '--project-package', {root_package_name!r},
-                    '--config', '{{{{var.value.env}}}}',
+                    '--config', '{{{{var.value.{env_var_name}}}}}',
                 ],
                 'namespace': namespace,
                 'image': {image_version!r},
                 'is_delete_operator_pod': True,
                 'retries': {retries!r},
                 'retry_delay': {retry_delay!r},
                 'secrets': {secrets_definition_list},
```

### Comparing `bigflow-1.7.2/bigflow/dataflow/io.py` & `bigflow-1.8.0/bigflow/dataflow/io.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.2/bigflow/dataflow/job.py` & `bigflow-1.8.0/bigflow/dataflow/job.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.2/bigflow/dataflow/ml.py` & `bigflow-1.8.0/bigflow/dataflow/ml.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.2/bigflow/dataflow/options.py` & `bigflow-1.8.0/bigflow/dataflow/options.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.2/bigflow/deploy.py` & `bigflow-1.8.0/bigflow/deploy.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.2/bigflow/konfig.py` & `bigflow-1.8.0/bigflow/konfig.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.2/bigflow/migrate.py` & `bigflow-1.8.0/bigflow/migrate.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.2/bigflow/resources.py` & `bigflow-1.8.0/bigflow/resources.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.2/bigflow/scaffold/infra.py` & `bigflow-1.8.0/bigflow/scaffold/infra.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.2/bigflow/scaffold/scaffold.py` & `bigflow-1.8.0/bigflow/scaffold/scaffold.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.2/bigflow/scaffold/templates/README.txt` & `bigflow-1.8.0/bigflow/scaffold/templates/README.txt`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.2/bigflow/scaffold/templates/new-project/.gitignore.j2` & `bigflow-1.8.0/bigflow/scaffold/templates/new-project/.gitignore.j2`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.2/bigflow/scaffold/templates/new-project/Dockerfile` & `bigflow-1.8.0/bigflow/scaffold/templates/new-project/Dockerfile`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.2/bigflow/scaffold/templates/new-project/README.md` & `bigflow-1.8.0/bigflow/scaffold/templates/new-project/README.md`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.2/bigflow/scaffold/templates/new-project/deployment_config.py.j2` & `bigflow-1.8.0/bigflow/scaffold/templates/new-project/deployment_config.py.j2`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.2/bigflow/scaffold/templates/new-project/test/pi_estimator/test_processing.py.j2` & `bigflow-1.8.0/bigflow/scaffold/templates/new-project/test/pi_estimator/test_processing.py.j2`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.2/bigflow/scaffold/templates/new-project/test/test_wordcount_workflow.py.j2` & `bigflow-1.8.0/bigflow/scaffold/templates/new-project/test/test_wordcount_workflow.py.j2`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.2/bigflow/scaffold/templates/new-project/{{project_name}}/internationalports/workflow.py.j2` & `bigflow-1.8.0/bigflow/scaffold/templates/new-project/{{project_name}}/internationalports/workflow.py.j2`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.2/bigflow/scaffold/templates/new-project/{{project_name}}/pi_estimator/processing.py.j2` & `bigflow-1.8.0/bigflow/scaffold/templates/new-project/{{project_name}}/pi_estimator/processing.py.j2`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.2/bigflow/scaffold/templates/new-project/{{project_name}}/pi_estimator/workflow.py.j2` & `bigflow-1.8.0/bigflow/scaffold/templates/new-project/{{project_name}}/pi_estimator/workflow.py.j2`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.2/bigflow/scaffold/templates/new-project/{{project_name}}/wordcount/pipeline.py.j2` & `bigflow-1.8.0/bigflow/scaffold/templates/new-project/{{project_name}}/wordcount/pipeline.py.j2`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.2/bigflow/scaffold/templates/new-project/{{project_name}}/wordcount/workflow.py.j2` & `bigflow-1.8.0/bigflow/scaffold/templates/new-project/{{project_name}}/wordcount/workflow.py.j2`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.2/bigflow/scaffold/templating.py` & `bigflow-1.8.0/bigflow/scaffold/templating.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.2/bigflow/testing/isolate.py` & `bigflow-1.8.0/bigflow/testing/isolate.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.2/bigflow/version.py` & `bigflow-1.8.0/bigflow/version.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.2/bigflow/workflow.py` & `bigflow-1.8.0/bigflow/workflow.py`

 * *Files 1% similar despite different names*

```diff
@@ -165,22 +165,24 @@
     def __init__(
         self,
         workflow_id: str,
         definition: Union['Definition', List['Job']],
         schedule_interval: str = DEFAULT_SCHEDULE_INTERVAL,
         start_time_factory: Callable[[dt.datetime], dt.datetime] = daily_start_time,
         depends_on_past: bool = True,
-        secrets: Iterable[str] = ()
+        secrets: Iterable[str] = (),
+        env_variable: str = "env"
     ):
         self.definition = self._parse_definition(definition)
         self.schedule_interval = schedule_interval
         self.workflow_id = workflow_id
         self.start_time_factory = start_time_factory
         self.depends_on_past = depends_on_past
         self.secrets = secrets
+        self.env_variable = env_variable
 
     @staticmethod
     def _execute_job(job: Job, context: JobContext) -> None:
         if not isinstance(job, Job):
             logger.debug("It is recommended to inherit your job %r from `bigflow.Job` class", job)
         if hasattr(job, 'execute'):
             job.execute(context)
```

### Comparing `bigflow-1.7.2/bigflow.egg-info/PKG-INFO` & `bigflow-1.8.0/bigflow.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bigflow
-Version: 1.7.2
+Version: 1.8.0
 Summary: BigQuery client wrapper with clean API
 Home-page: https://github.com/allegro/bigflow
 Author: Pogranicze
 Author-email: pogranicze-team@allegro.pl
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `bigflow-1.7.2/bigflow.egg-info/SOURCES.txt` & `bigflow-1.8.0/bigflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.2/bigflow.egg-info/requires.txt` & `bigflow-1.8.0/bigflow.egg-info/requires.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 grpcio-status<=1.48.2
-google-cloud-storage<2,>=1.30
+google-cloud-storage<3,>=2
 MarkupSafe>2.1.0
 google-auth<3,>=1.20
 unittest-xml-reporting<4,>=3.0.2
 jinja2<4,>=3
 pip-tools<7,>=5.3
 deprecated<2,>=1.2.10
 toml>=0.10
@@ -20,23 +20,22 @@
 cachetools==5.0.0
 certifi==2021.10.8
 charset-normalizer==2.0.12
 click==8.0.4
 deprecated==1.2.13
 google-api-core==2.7.1
 google-auth==2.6.2
-google-cloud-core==2.2.3
-google-cloud-storage==1.44.0
+google-cloud-core==2.3.2
+google-cloud-storage==2.9.0
 google-crc32c==1.3.0
 google-resumable-media==2.3.2
 googleapis-common-protos==1.56.0
 grpcio==1.50.0
 grpcio-status==1.48.2
 idna==3.3
-importlib-metadata==4.11.3
 jinja2==3.1.2
 lazy-object-proxy==1.7.1
 lxml==4.8.0
 markupsafe==2.1.1
 pep517==0.12.0
 pip-tools==6.5.1
 protobuf==3.19.4
@@ -49,20 +48,19 @@
 toml==0.10.2
 tomli==2.0.1
 typing-extensions==3.10.0.2
 unittest-xml-reporting==3.2.0
 urllib3==1.26.9
 wheel==0.37.1
 wrapt==1.14.0
-zipp==3.7.0
 
 [base_frozen:python_version <= "3.8"]
 backports-cached-property==1.0.1
 
 [bigquery]
 google-cloud-bigquery<4,>=1.6
 db-dtypes>=1.0.5
 pandas<2,>=0.25
 six<2,>=1.14
 
 [dataflow]
-apache-beam[gcp]<2.46,>=2.24
+apache-beam[gcp]<=2.48,>=2.24
```

### Comparing `bigflow-1.7.2/setup.py` & `bigflow-1.8.0/setup.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.2/test/buildd/test_dev.py` & `bigflow-1.8.0/test/buildd/test_dev.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.2/test/buildd/test_dist.py` & `bigflow-1.8.0/test/buildd/test_dist.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.2/test/buildd/test_operate.py` & `bigflow-1.8.0/test/buildd/test_operate.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.2/test/buildd/test_pip.py` & `bigflow-1.8.0/test/buildd/test_pip.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.2/test/buildd/test_reflect.py` & `bigflow-1.8.0/test/buildd/test_reflect.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.2/test/buildd/test_spec.py` & `bigflow-1.8.0/test/buildd/test_spec.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.2/test/cli/test_cli.py` & `bigflow-1.8.0/test/cli/test_cli.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.2/test/cli/test_module/Unused1.py` & `bigflow-1.8.0/test/cli/test_module/Unused1.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.2/test/dagbuilder/test_dagbuilder.py` & `bigflow-1.8.0/test/dagbuilder/test_dagbuilder.py`

 * *Files 12% similar despite different names*

```diff
@@ -131,14 +131,51 @@
         # then passes the depends_on_past parameter value
         self.assertEqual(dag_file_path, str(workdir / '.dags/my_parametrized_workflow__v0_3_0__2020_07_02_00_00_00_dag.py'))
 
         dag_file_content = Path(dag_file_path).read_text()
         expected_dag_content = (Path(__file__).parent / "my_parametrized_workflow__dag.py.txt").read_text()
         self.assert_files_are_equal(expected_dag_content, dag_file_content)
 
+    def test_should_set_different_env_variable_name_for_dag(self):
+        # given
+        workdir = self.cwd
+        docker_repository = 'eu.gcr.io/my_docker_repository_project/my-project'
+        version = '0.3.0'
+        image = f'{docker_repository}:{version}'
+
+        # given
+        job1 = Job(
+            id='job1',
+            component=mock.Mock(),
+            retry_count=10,
+            retry_pause_sec=20
+        )
+        w_job1 = WorkflowJob(job1, 1)
+        graph = {
+            w_job1: ()
+        }
+        workflow = Workflow(
+            workflow_id='my_parametrized_env_workflow',
+            definition=Definition(graph),
+            depends_on_past=False,
+            schedule_interval='@daily',
+            secrets=['bf_secret_password', 'bf_secret_token'],
+            env_variable='prod_env',
+        )
+
+        # when
+        dag_file_path = generate_dag_file(workdir, image, workflow, '2020-07-02', version, 'ca')
+
+        # then passes the depends_on_past parameter value
+        self.assertEqual(dag_file_path, str(workdir / '.dags/my_parametrized_env_workflow__v0_3_0__2020_07_02_00_00_00_dag.py'))
+
+        dag_file_content = Path(dag_file_path).read_text()
+        expected_dag_content = (Path(__file__).parent / "my_parametrized_env_workflow__dag.py.txt").read_text()
+        self.assert_files_are_equal(expected_dag_content, dag_file_content)
+
     def test_should_generate_DAG_file_from_workflow_with_daily_scheduling(self):
         # given
         workdir = self.cwd
         docker_repository = 'eu.gcr.io/my_docker_repository_project/my-project'
         version = '0.3.0'
         image = f'{docker_repository}:{version}'
```

### Comparing `bigflow-1.7.2/test/test_commons.py` & `bigflow-1.8.0/test/test_commons.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.2/test/test_configuration.py` & `bigflow-1.8.0/test/test_configuration.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.2/test/test_dataflow.py` & `bigflow-1.8.0/test/test_dataflow.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.2/test/test_deploy.py` & `bigflow-1.8.0/test/test_deploy.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.2/test/test_interactive.py` & `bigflow-1.8.0/test/test_interactive.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.2/test/test_job.py` & `bigflow-1.8.0/test/test_job.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.2/test/test_konfig.py` & `bigflow-1.8.0/test/test_konfig.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.2/test/test_migrate.py` & `bigflow-1.8.0/test/test_migrate.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.2/test/test_resources.py` & `bigflow-1.8.0/test/test_resources.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.2/test/test_scaffold.py` & `bigflow-1.8.0/test/test_scaffold.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.2/test/test_user_commons/test_labels.py` & `bigflow-1.8.0/test/test_user_commons/test_labels.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.2/test/test_user_commons/test_sensor.py` & `bigflow-1.8.0/test/test_user_commons/test_sensor.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.2/test/test_version.py` & `bigflow-1.8.0/test/test_version.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.2/test/test_workflow.py` & `bigflow-1.8.0/test/test_workflow.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.7.2/test/testing/test_isolate.py` & `bigflow-1.8.0/test/testing/test_isolate.py`

 * *Files identical despite different names*

