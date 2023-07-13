# Comparing `tmp/kfp-tekton-server-api-1.8.0rc1.tar.gz` & `tmp/kfp-tekton-server-api-1.8.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kfp-tekton-server-api-1.8.0rc1.tar", last modified: Wed Jul 12 21:12:27 2023, max compression
+gzip compressed data, was "kfp-tekton-server-api-1.8.0rc2.tar", last modified: Thu Jul 13 21:36:56 2023, max compression
```

## Comparing `kfp-tekton-server-api-1.8.0rc1.tar` & `kfp-tekton-server-api-1.8.0rc2.tar`

### file list

```diff
@@ -1,113 +1,113 @@
-drwxr-xr-x   0 tommyli    (501) staff       (20)        0 2023-07-12 21:12:27.612959 kfp-tekton-server-api-1.8.0rc1/
--rw-r--r--   0 tommyli    (501) staff       (20)    11357 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/LICENSE
--rw-r--r--   0 tommyli    (501) staff       (20)      455 2023-07-12 21:12:27.613173 kfp-tekton-server-api-1.8.0rc1/PKG-INFO
--rw-r--r--   0 tommyli    (501) staff       (20)    13063 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/README.md
-drwxr-xr-x   0 tommyli    (501) staff       (20)        0 2023-07-12 21:12:27.564331 kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/
--rw-r--r--   0 tommyli    (501) staff       (20)     4398 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/__init__.py
-drwxr-xr-x   0 tommyli    (501) staff       (20)        0 2023-07-12 21:12:27.570540 kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/api/
--rw-r--r--   0 tommyli    (501) staff       (20)      550 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/api/__init__.py
--rw-r--r--   0 tommyli    (501) staff       (20)    36823 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/api/experiment_service_api.py
--rw-r--r--   0 tommyli    (501) staff       (20)     5448 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/api/healthz_service_api.py
--rw-r--r--   0 tommyli    (501) staff       (20)    35425 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/api/job_service_api.py
--rw-r--r--   0 tommyli    (501) staff       (20)    69047 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/api/pipeline_service_api.py
--rw-r--r--   0 tommyli    (501) staff       (20)    13674 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/api/pipeline_upload_service_api.py
--rw-r--r--   0 tommyli    (501) staff       (20)    59741 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/api/run_service_api.py
--rw-r--r--   0 tommyli    (501) staff       (20)    26288 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/api_client.py
--rw-r--r--   0 tommyli    (501) staff       (20)    13319 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/configuration.py
--rw-r--r--   0 tommyli    (501) staff       (20)     3795 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/exceptions.py
-drwxr-xr-x   0 tommyli    (501) staff       (20)        0 2023-07-12 21:12:27.590901 kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/models/
--rw-r--r--   0 tommyli    (501) staff       (20)     3447 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/models/__init__.py
--rw-r--r--   0 tommyli    (501) staff       (20)     4658 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/models/googlerpc_status.py
--rw-r--r--   0 tommyli    (501) staff       (20)     3481 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/models/inline_object.py
--rw-r--r--   0 tommyli    (501) staff       (20)     2873 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/models/job_mode.py
--rw-r--r--   0 tommyli    (501) staff       (20)     4643 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/models/pipeline_spec_runtime_config.py
--rw-r--r--   0 tommyli    (501) staff       (20)    10425 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/models/protobuf_any.py
--rw-r--r--   0 tommyli    (501) staff       (20)     6709 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/models/report_run_metrics_response_report_run_metric_result.py
--rw-r--r--   0 tommyli    (501) staff       (20)     3178 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/models/report_run_metrics_response_report_run_metric_result_status.py
--rw-r--r--   0 tommyli    (501) staff       (20)     2896 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/models/run_metric_format.py
--rw-r--r--   0 tommyli    (501) staff       (20)     4712 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/models/v1_cron_schedule.py
--rw-r--r--   0 tommyli    (501) staff       (20)     7846 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/models/v1_experiment.py
--rw-r--r--   0 tommyli    (501) staff       (20)     2983 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/models/v1_experiment_storage_state.py
--rw-r--r--   0 tommyli    (501) staff       (20)     3470 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/models/v1_get_healthz_response.py
--rw-r--r--   0 tommyli    (501) staff       (20)     3762 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/models/v1_get_template_response.py
--rw-r--r--   0 tommyli    (501) staff       (20)    14740 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/models/v1_job.py
--rw-r--r--   0 tommyli    (501) staff       (20)     5594 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/models/v1_list_experiments_response.py
--rw-r--r--   0 tommyli    (501) staff       (20)     5272 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/models/v1_list_jobs_response.py
--rw-r--r--   0 tommyli    (501) staff       (20)     5542 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/models/v1_list_pipeline_versions_response.py
--rw-r--r--   0 tommyli    (501) staff       (20)     5398 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/models/v1_list_pipelines_response.py
--rw-r--r--   0 tommyli    (501) staff       (20)     5178 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/models/v1_list_runs_response.py
--rw-r--r--   0 tommyli    (501) staff       (20)     3869 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/models/v1_parameter.py
--rw-r--r--   0 tommyli    (501) staff       (20)     5006 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/models/v1_periodic_schedule.py
--rw-r--r--   0 tommyli    (501) staff       (20)    11586 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/models/v1_pipeline.py
--rw-r--r--   0 tommyli    (501) staff       (20)     5052 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/models/v1_pipeline_runtime.py
--rw-r--r--   0 tommyli    (501) staff       (20)     8397 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/models/v1_pipeline_spec.py
--rw-r--r--   0 tommyli    (501) staff       (20)    13714 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/models/v1_pipeline_version.py
--rw-r--r--   0 tommyli    (501) staff       (20)     3868 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/models/v1_read_artifact_response.py
--rw-r--r--   0 tommyli    (501) staff       (20)     2916 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/models/v1_relationship.py
--rw-r--r--   0 tommyli    (501) staff       (20)     3597 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/models/v1_report_run_metrics_response.py
--rw-r--r--   0 tommyli    (501) staff       (20)     3989 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/models/v1_resource_key.py
--rw-r--r--   0 tommyli    (501) staff       (20)     4894 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/models/v1_resource_reference.py
--rw-r--r--   0 tommyli    (501) staff       (20)     3057 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/models/v1_resource_type.py
--rw-r--r--   0 tommyli    (501) staff       (20)    14091 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/models/v1_run.py
--rw-r--r--   0 tommyli    (501) staff       (20)     4126 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/models/v1_run_detail.py
--rw-r--r--   0 tommyli    (501) staff       (20)     6333 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/models/v1_run_metric.py
--rw-r--r--   0 tommyli    (501) staff       (20)     2897 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/models/v1_run_storage_state.py
--rw-r--r--   0 tommyli    (501) staff       (20)     4504 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/models/v1_status.py
--rw-r--r--   0 tommyli    (501) staff       (20)     4362 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/models/v1_trigger.py
--rw-r--r--   0 tommyli    (501) staff       (20)     4289 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/models/v1_url.py
--rw-r--r--   0 tommyli    (501) staff       (20)     4806 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/models/v1_value.py
--rw-r--r--   0 tommyli    (501) staff       (20)    12334 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/rest.py
-drwxr-xr-x   0 tommyli    (501) staff       (20)        0 2023-07-12 21:12:27.566967 kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api.egg-info/
--rw-r--r--   0 tommyli    (501) staff       (20)      455 2023-07-12 21:12:27.000000 kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api.egg-info/PKG-INFO
--rw-r--r--   0 tommyli    (501) staff       (20)     4343 2023-07-12 21:12:27.000000 kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api.egg-info/SOURCES.txt
--rw-r--r--   0 tommyli    (501) staff       (20)        1 2023-07-12 21:12:27.000000 kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api.egg-info/dependency_links.txt
--rw-r--r--   0 tommyli    (501) staff       (20)       48 2023-07-12 21:12:27.000000 kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api.egg-info/requires.txt
--rw-r--r--   0 tommyli    (501) staff       (20)       22 2023-07-12 21:12:27.000000 kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api.egg-info/top_level.txt
--rw-r--r--   0 tommyli    (501) staff       (20)       69 2023-07-12 21:12:27.613839 kfp-tekton-server-api-1.8.0rc1/setup.cfg
--rw-r--r--   0 tommyli    (501) staff       (20)     1201 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/setup.py
-drwxr-xr-x   0 tommyli    (501) staff       (20)        0 2023-07-12 21:12:27.612449 kfp-tekton-server-api-1.8.0rc1/test/
--rw-r--r--   0 tommyli    (501) staff       (20)     2286 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/test/test_experiment_service_api.py
--rw-r--r--   0 tommyli    (501) staff       (20)     1622 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/test/test_googlerpc_status.py
--rw-r--r--   0 tommyli    (501) staff       (20)      971 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/test/test_healthz_service_api.py
--rw-r--r--   0 tommyli    (501) staff       (20)     1694 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/test/test_inline_object.py
--rw-r--r--   0 tommyli    (501) staff       (20)     1339 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/test/test_job_mode.py
--rw-r--r--   0 tommyli    (501) staff       (20)     1848 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/test/test_job_service_api.py
--rw-r--r--   0 tommyli    (501) staff       (20)     3721 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/test/test_pipeline_service_api.py
--rw-r--r--   0 tommyli    (501) staff       (20)     1842 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/test/test_pipeline_spec_runtime_config.py
--rw-r--r--   0 tommyli    (501) staff       (20)     1071 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/test/test_pipeline_upload_service_api.py
--rw-r--r--   0 tommyli    (501) staff       (20)     1476 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/test/test_protobuf_any.py
--rw-r--r--   0 tommyli    (501) staff       (20)     1915 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/test/test_report_run_metrics_response_report_run_metric_result.py
--rw-r--r--   0 tommyli    (501) staff       (20)     1837 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/test/test_report_run_metrics_response_report_run_metric_result_status.py
--rw-r--r--   0 tommyli    (501) staff       (20)     1429 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/test/test_run_metric_format.py
--rw-r--r--   0 tommyli    (501) staff       (20)     2682 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/test/test_run_service_api.py
--rw-r--r--   0 tommyli    (501) staff       (20)     1659 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/test/test_v1_cron_schedule.py
--rw-r--r--   0 tommyli    (501) staff       (20)     2104 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/test/test_v1_experiment.py
--rw-r--r--   0 tommyli    (501) staff       (20)     1530 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/test/test_v1_experiment_storage_state.py
--rw-r--r--   0 tommyli    (501) staff       (20)     1520 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/test/test_v1_get_healthz_response.py
--rw-r--r--   0 tommyli    (501) staff       (20)     1528 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/test/test_v1_get_template_response.py
--rw-r--r--   0 tommyli    (501) staff       (20)     4344 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/test/test_v1_job.py
--rw-r--r--   0 tommyli    (501) staff       (20)     2563 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/test/test_v1_list_experiments_response.py
--rw-r--r--   0 tommyli    (501) staff       (20)     5054 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/test/test_v1_list_jobs_response.py
--rw-r--r--   0 tommyli    (501) staff       (20)     3607 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/test/test_v1_list_pipeline_versions_response.py
--rw-r--r--   0 tommyli    (501) staff       (20)     4513 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/test/test_v1_list_pipelines_response.py
--rw-r--r--   0 tommyli    (501) staff       (20)     4306 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/test/test_v1_list_runs_response.py
--rw-r--r--   0 tommyli    (501) staff       (20)     1440 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/test/test_v1_parameter.py
--rw-r--r--   0 tommyli    (501) staff       (20)     1714 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/test/test_v1_periodic_schedule.py
--rw-r--r--   0 tommyli    (501) staff       (20)     4295 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/test/test_v1_pipeline.py
--rw-r--r--   0 tommyli    (501) staff       (20)     1533 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/test/test_v1_pipeline_runtime.py
--rw-r--r--   0 tommyli    (501) staff       (20)     2232 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/test/test_v1_pipeline_spec.py
--rw-r--r--   0 tommyli    (501) staff       (20)     3261 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/test/test_v1_pipeline_version.py
--rw-r--r--   0 tommyli    (501) staff       (20)     1538 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/test/test_v1_read_artifact_response.py
--rw-r--r--   0 tommyli    (501) staff       (20)     1416 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/test/test_v1_relationship.py
--rw-r--r--   0 tommyli    (501) staff       (20)     1934 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/test/test_v1_report_run_metrics_response.py
--rw-r--r--   0 tommyli    (501) staff       (20)     1481 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/test/test_v1_resource_key.py
--rw-r--r--   0 tommyli    (501) staff       (20)     1725 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/test/test_v1_resource_reference.py
--rw-r--r--   0 tommyli    (501) staff       (20)     1418 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/test/test_v1_resource_type.py
--rw-r--r--   0 tommyli    (501) staff       (20)     3628 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/test/test_v1_run.py
--rw-r--r--   0 tommyli    (501) staff       (20)     4134 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/test/test_v1_run_detail.py
--rw-r--r--   0 tommyli    (501) staff       (20)     1524 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/test/test_v1_run_metric.py
--rw-r--r--   0 tommyli    (501) staff       (20)     1453 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/test/test_v1_run_storage_state.py
--rw-r--r--   0 tommyli    (501) staff       (20)     1543 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/test/test_v1_status.py
--rw-r--r--   0 tommyli    (501) staff       (20)     2286 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/test/test_v1_trigger.py
--rw-r--r--   0 tommyli    (501) staff       (20)     1389 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/test/test_v1_url.py
--rw-r--r--   0 tommyli    (501) staff       (20)     1447 2023-07-12 21:12:26.000000 kfp-tekton-server-api-1.8.0rc1/test/test_v1_value.py
+drwxr-xr-x   0 tommyli    (501) staff       (20)        0 2023-07-13 21:36:56.959372 kfp-tekton-server-api-1.8.0rc2/
+-rw-r--r--   0 tommyli    (501) staff       (20)    11357 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/LICENSE
+-rw-r--r--   0 tommyli    (501) staff       (20)      457 2023-07-13 21:36:56.959588 kfp-tekton-server-api-1.8.0rc2/PKG-INFO
+-rw-r--r--   0 tommyli    (501) staff       (20)    13066 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/README.md
+drwxr-xr-x   0 tommyli    (501) staff       (20)        0 2023-07-13 21:36:56.909678 kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/
+-rw-r--r--   0 tommyli    (501) staff       (20)     4398 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/__init__.py
+drwxr-xr-x   0 tommyli    (501) staff       (20)        0 2023-07-13 21:36:56.915538 kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/api/
+-rw-r--r--   0 tommyli    (501) staff       (20)      550 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/api/__init__.py
+-rw-r--r--   0 tommyli    (501) staff       (20)    36823 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/api/experiment_service_api.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     5448 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/api/healthz_service_api.py
+-rw-r--r--   0 tommyli    (501) staff       (20)    35425 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/api/job_service_api.py
+-rw-r--r--   0 tommyli    (501) staff       (20)    69047 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/api/pipeline_service_api.py
+-rw-r--r--   0 tommyli    (501) staff       (20)    13674 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/api/pipeline_upload_service_api.py
+-rw-r--r--   0 tommyli    (501) staff       (20)    59741 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/api/run_service_api.py
+-rw-r--r--   0 tommyli    (501) staff       (20)    26288 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/api_client.py
+-rw-r--r--   0 tommyli    (501) staff       (20)    13322 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/configuration.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     3795 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/exceptions.py
+drwxr-xr-x   0 tommyli    (501) staff       (20)        0 2023-07-13 21:36:56.936177 kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/models/
+-rw-r--r--   0 tommyli    (501) staff       (20)     3447 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/models/__init__.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     4658 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/models/googlerpc_status.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     3481 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/models/inline_object.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     2873 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/models/job_mode.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     4643 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/models/pipeline_spec_runtime_config.py
+-rw-r--r--   0 tommyli    (501) staff       (20)    10425 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/models/protobuf_any.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     6709 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/models/report_run_metrics_response_report_run_metric_result.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     3178 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/models/report_run_metrics_response_report_run_metric_result_status.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     2896 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/models/run_metric_format.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     4712 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/models/v1_cron_schedule.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     7846 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/models/v1_experiment.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     2983 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/models/v1_experiment_storage_state.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     3470 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/models/v1_get_healthz_response.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     3762 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/models/v1_get_template_response.py
+-rw-r--r--   0 tommyli    (501) staff       (20)    14740 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/models/v1_job.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     5594 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/models/v1_list_experiments_response.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     5272 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/models/v1_list_jobs_response.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     5542 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/models/v1_list_pipeline_versions_response.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     5398 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/models/v1_list_pipelines_response.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     5178 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/models/v1_list_runs_response.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     3869 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/models/v1_parameter.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     5006 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/models/v1_periodic_schedule.py
+-rw-r--r--   0 tommyli    (501) staff       (20)    11586 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/models/v1_pipeline.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     5052 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/models/v1_pipeline_runtime.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     8397 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/models/v1_pipeline_spec.py
+-rw-r--r--   0 tommyli    (501) staff       (20)    13714 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/models/v1_pipeline_version.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     3868 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/models/v1_read_artifact_response.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     2916 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/models/v1_relationship.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     3597 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/models/v1_report_run_metrics_response.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     3989 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/models/v1_resource_key.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     4894 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/models/v1_resource_reference.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     3057 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/models/v1_resource_type.py
+-rw-r--r--   0 tommyli    (501) staff       (20)    14091 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/models/v1_run.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     4126 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/models/v1_run_detail.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     6333 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/models/v1_run_metric.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     2897 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/models/v1_run_storage_state.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     4504 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/models/v1_status.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     4362 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/models/v1_trigger.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     4289 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/models/v1_url.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     4806 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/models/v1_value.py
+-rw-r--r--   0 tommyli    (501) staff       (20)    12334 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/rest.py
+drwxr-xr-x   0 tommyli    (501) staff       (20)        0 2023-07-13 21:36:56.912014 kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api.egg-info/
+-rw-r--r--   0 tommyli    (501) staff       (20)      457 2023-07-13 21:36:56.000000 kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api.egg-info/PKG-INFO
+-rw-r--r--   0 tommyli    (501) staff       (20)     4343 2023-07-13 21:36:56.000000 kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api.egg-info/SOURCES.txt
+-rw-r--r--   0 tommyli    (501) staff       (20)        1 2023-07-13 21:36:56.000000 kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api.egg-info/dependency_links.txt
+-rw-r--r--   0 tommyli    (501) staff       (20)       48 2023-07-13 21:36:56.000000 kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api.egg-info/requires.txt
+-rw-r--r--   0 tommyli    (501) staff       (20)       22 2023-07-13 21:36:56.000000 kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api.egg-info/top_level.txt
+-rw-r--r--   0 tommyli    (501) staff       (20)       69 2023-07-13 21:36:56.960267 kfp-tekton-server-api-1.8.0rc2/setup.cfg
+-rw-r--r--   0 tommyli    (501) staff       (20)     1203 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/setup.py
+drwxr-xr-x   0 tommyli    (501) staff       (20)        0 2023-07-13 21:36:56.958890 kfp-tekton-server-api-1.8.0rc2/test/
+-rw-r--r--   0 tommyli    (501) staff       (20)     2286 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/test/test_experiment_service_api.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     1622 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/test/test_googlerpc_status.py
+-rw-r--r--   0 tommyli    (501) staff       (20)      971 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/test/test_healthz_service_api.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     1694 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/test/test_inline_object.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     1339 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/test/test_job_mode.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     1848 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/test/test_job_service_api.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     3721 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/test/test_pipeline_service_api.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     1842 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/test/test_pipeline_spec_runtime_config.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     1071 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/test/test_pipeline_upload_service_api.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     1476 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/test/test_protobuf_any.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     1915 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/test/test_report_run_metrics_response_report_run_metric_result.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     1837 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/test/test_report_run_metrics_response_report_run_metric_result_status.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     1429 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/test/test_run_metric_format.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     2682 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/test/test_run_service_api.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     1659 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/test/test_v1_cron_schedule.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     2104 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/test/test_v1_experiment.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     1530 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/test/test_v1_experiment_storage_state.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     1520 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/test/test_v1_get_healthz_response.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     1528 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/test/test_v1_get_template_response.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     4344 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/test/test_v1_job.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     2563 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/test/test_v1_list_experiments_response.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     5054 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/test/test_v1_list_jobs_response.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     3607 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/test/test_v1_list_pipeline_versions_response.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     4513 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/test/test_v1_list_pipelines_response.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     4306 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/test/test_v1_list_runs_response.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     1440 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/test/test_v1_parameter.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     1714 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/test/test_v1_periodic_schedule.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     4295 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/test/test_v1_pipeline.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     1533 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/test/test_v1_pipeline_runtime.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     2232 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/test/test_v1_pipeline_spec.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     3261 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/test/test_v1_pipeline_version.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     1538 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/test/test_v1_read_artifact_response.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     1416 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/test/test_v1_relationship.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     1934 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/test/test_v1_report_run_metrics_response.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     1481 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/test/test_v1_resource_key.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     1725 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/test/test_v1_resource_reference.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     1418 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/test/test_v1_resource_type.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     3628 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/test/test_v1_run.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     4134 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/test/test_v1_run_detail.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     1524 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/test/test_v1_run_metric.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     1453 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/test/test_v1_run_storage_state.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     1543 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/test/test_v1_status.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     2286 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/test/test_v1_trigger.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     1389 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/test/test_v1_url.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     1447 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/test/test_v1_value.py
```

### Comparing `kfp-tekton-server-api-1.8.0rc1/LICENSE` & `kfp-tekton-server-api-1.8.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc1/README.md` & `kfp-tekton-server-api-1.8.0rc2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # kfp-tekton-server-api
 This file contains REST API specification for Kubeflow Pipelines. The file is autogenerated from the swagger definition.
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 1.7.0
-- Package version: 1.8.0rc1
+- API version: 1.8.0rc2
+- Package version: 1.8.0rc2
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 For more information, please visit [https://www.google.com](https://www.google.com)
 
 ## Requirements.
 
 Python 2.7 and 3.4+
```

### Comparing `kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/__init__.py` & `kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     Contact: kubeflow-pipelines@google.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
-__version__ = "1.8.0rc1"
+__version__ = "1.8.0rc2"
 
 # import apis into sdk package
 from kfp_tekton_server_api.api.experiment_service_api import ExperimentServiceApi
 from kfp_tekton_server_api.api.healthz_service_api import HealthzServiceApi
 from kfp_tekton_server_api.api.job_service_api import JobServiceApi
 from kfp_tekton_server_api.api.pipeline_service_api import PipelineServiceApi
 from kfp_tekton_server_api.api.pipeline_upload_service_api import PipelineUploadServiceApi
```

### Comparing `kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/api/__init__.py` & `kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/api/__init__.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/api/experiment_service_api.py` & `kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/api/experiment_service_api.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/api/healthz_service_api.py` & `kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/api/healthz_service_api.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/api/job_service_api.py` & `kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/api/job_service_api.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/api/pipeline_service_api.py` & `kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/api/pipeline_service_api.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/api/pipeline_upload_service_api.py` & `kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/api/pipeline_upload_service_api.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/api/run_service_api.py` & `kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/api/run_service_api.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/api_client.py` & `kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/api_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,15 +74,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/1.8.0rc1/python'
+        self.user_agent = 'OpenAPI-Generator/1.8.0rc2/python'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/configuration.py` & `kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -347,16 +347,16 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 1.7.0\n"\
-               "SDK Package Version: 1.8.0rc1".\
+               "Version of the API: 1.8.0rc2\n"\
+               "SDK Package Version: 1.8.0rc2".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/exceptions.py` & `kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/models/__init__.py` & `kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/models/__init__.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/models/googlerpc_status.py` & `kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/models/googlerpc_status.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/models/inline_object.py` & `kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/models/inline_object.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/models/job_mode.py` & `kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/models/job_mode.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/models/pipeline_spec_runtime_config.py` & `kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/models/pipeline_spec_runtime_config.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/models/protobuf_any.py` & `kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/models/protobuf_any.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/models/report_run_metrics_response_report_run_metric_result.py` & `kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/models/report_run_metrics_response_report_run_metric_result.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/models/report_run_metrics_response_report_run_metric_result_status.py` & `kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/models/report_run_metrics_response_report_run_metric_result_status.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/models/run_metric_format.py` & `kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/models/run_metric_format.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/models/v1_cron_schedule.py` & `kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/models/v1_cron_schedule.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/models/v1_experiment.py` & `kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/models/v1_experiment.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/models/v1_experiment_storage_state.py` & `kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/models/v1_experiment_storage_state.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/models/v1_get_healthz_response.py` & `kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/models/v1_get_healthz_response.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/models/v1_get_template_response.py` & `kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/models/v1_get_template_response.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/models/v1_job.py` & `kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/models/v1_job.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/models/v1_list_experiments_response.py` & `kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/models/v1_list_experiments_response.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/models/v1_list_jobs_response.py` & `kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/models/v1_list_jobs_response.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/models/v1_list_pipeline_versions_response.py` & `kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/models/v1_list_pipeline_versions_response.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/models/v1_list_pipelines_response.py` & `kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/models/v1_list_pipelines_response.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/models/v1_list_runs_response.py` & `kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/models/v1_list_runs_response.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/models/v1_parameter.py` & `kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/models/v1_parameter.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/models/v1_periodic_schedule.py` & `kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/models/v1_periodic_schedule.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/models/v1_pipeline.py` & `kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/models/v1_pipeline.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/models/v1_pipeline_runtime.py` & `kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/models/v1_pipeline_runtime.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/models/v1_pipeline_spec.py` & `kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/models/v1_pipeline_spec.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/models/v1_pipeline_version.py` & `kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/models/v1_pipeline_version.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/models/v1_read_artifact_response.py` & `kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/models/v1_read_artifact_response.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/models/v1_relationship.py` & `kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/models/v1_relationship.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/models/v1_report_run_metrics_response.py` & `kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/models/v1_report_run_metrics_response.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/models/v1_resource_key.py` & `kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/models/v1_resource_key.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/models/v1_resource_reference.py` & `kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/models/v1_resource_reference.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/models/v1_resource_type.py` & `kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/models/v1_resource_type.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/models/v1_run.py` & `kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/models/v1_run.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/models/v1_run_detail.py` & `kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/models/v1_run_detail.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/models/v1_run_metric.py` & `kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/models/v1_run_metric.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/models/v1_run_storage_state.py` & `kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/models/v1_run_storage_state.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/models/v1_status.py` & `kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/models/v1_status.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/models/v1_trigger.py` & `kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/models/v1_trigger.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/models/v1_url.py` & `kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/models/v1_url.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/models/v1_value.py` & `kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/models/v1_value.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api/rest.py` & `kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/rest.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc1/kfp_tekton_server_api.egg-info/SOURCES.txt` & `kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc1/setup.py` & `kfp-tekton-server-api-1.8.0rc2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,29 +9,29 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "kfp-tekton-server-api"
-VERSION = "1.8.0rc1"
+VERSION = "1.8.0rc2"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
 
 REQUIRES = ["urllib3 >= 1.15", "six >= 1.10", "certifi", "python-dateutil"]
 
 setup(
     name=NAME,
     version=VERSION,
     description="Kubeflow Pipelines API",
-    author="google",
+    author="kubeflow",
     author_email="kubeflow-pipelines@google.com",
     url="https://github.com/kubeflow/kfp-tekton",
     keywords=["OpenAPI", "OpenAPI-Generator", "Kubeflow Pipelines API"],
     install_requires=REQUIRES,
     packages=find_packages(exclude=["test", "tests"]),
     include_package_data=True,
     license="Apache 2.0",
```

### Comparing `kfp-tekton-server-api-1.8.0rc1/test/test_experiment_service_api.py` & `kfp-tekton-server-api-1.8.0rc2/test/test_experiment_service_api.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc1/test/test_googlerpc_status.py` & `kfp-tekton-server-api-1.8.0rc2/test/test_googlerpc_status.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc1/test/test_healthz_service_api.py` & `kfp-tekton-server-api-1.8.0rc2/test/test_healthz_service_api.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc1/test/test_inline_object.py` & `kfp-tekton-server-api-1.8.0rc2/test/test_inline_object.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc1/test/test_job_mode.py` & `kfp-tekton-server-api-1.8.0rc2/test/test_job_mode.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc1/test/test_job_service_api.py` & `kfp-tekton-server-api-1.8.0rc2/test/test_job_service_api.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc1/test/test_pipeline_service_api.py` & `kfp-tekton-server-api-1.8.0rc2/test/test_pipeline_service_api.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc1/test/test_pipeline_spec_runtime_config.py` & `kfp-tekton-server-api-1.8.0rc2/test/test_pipeline_spec_runtime_config.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc1/test/test_pipeline_upload_service_api.py` & `kfp-tekton-server-api-1.8.0rc2/test/test_pipeline_upload_service_api.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc1/test/test_protobuf_any.py` & `kfp-tekton-server-api-1.8.0rc2/test/test_protobuf_any.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc1/test/test_report_run_metrics_response_report_run_metric_result.py` & `kfp-tekton-server-api-1.8.0rc2/test/test_report_run_metrics_response_report_run_metric_result.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc1/test/test_report_run_metrics_response_report_run_metric_result_status.py` & `kfp-tekton-server-api-1.8.0rc2/test/test_report_run_metrics_response_report_run_metric_result_status.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc1/test/test_run_metric_format.py` & `kfp-tekton-server-api-1.8.0rc2/test/test_run_metric_format.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc1/test/test_run_service_api.py` & `kfp-tekton-server-api-1.8.0rc2/test/test_run_service_api.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc1/test/test_v1_cron_schedule.py` & `kfp-tekton-server-api-1.8.0rc2/test/test_v1_cron_schedule.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc1/test/test_v1_experiment.py` & `kfp-tekton-server-api-1.8.0rc2/test/test_v1_experiment.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc1/test/test_v1_experiment_storage_state.py` & `kfp-tekton-server-api-1.8.0rc2/test/test_v1_experiment_storage_state.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc1/test/test_v1_get_healthz_response.py` & `kfp-tekton-server-api-1.8.0rc2/test/test_v1_get_healthz_response.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc1/test/test_v1_get_template_response.py` & `kfp-tekton-server-api-1.8.0rc2/test/test_v1_get_template_response.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc1/test/test_v1_job.py` & `kfp-tekton-server-api-1.8.0rc2/test/test_v1_job.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc1/test/test_v1_list_experiments_response.py` & `kfp-tekton-server-api-1.8.0rc2/test/test_v1_list_experiments_response.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc1/test/test_v1_list_jobs_response.py` & `kfp-tekton-server-api-1.8.0rc2/test/test_v1_list_jobs_response.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc1/test/test_v1_list_pipeline_versions_response.py` & `kfp-tekton-server-api-1.8.0rc2/test/test_v1_list_pipeline_versions_response.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc1/test/test_v1_list_pipelines_response.py` & `kfp-tekton-server-api-1.8.0rc2/test/test_v1_list_pipelines_response.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc1/test/test_v1_list_runs_response.py` & `kfp-tekton-server-api-1.8.0rc2/test/test_v1_list_runs_response.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc1/test/test_v1_parameter.py` & `kfp-tekton-server-api-1.8.0rc2/test/test_v1_parameter.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc1/test/test_v1_periodic_schedule.py` & `kfp-tekton-server-api-1.8.0rc2/test/test_v1_periodic_schedule.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc1/test/test_v1_pipeline.py` & `kfp-tekton-server-api-1.8.0rc2/test/test_v1_pipeline.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc1/test/test_v1_pipeline_runtime.py` & `kfp-tekton-server-api-1.8.0rc2/test/test_v1_pipeline_runtime.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc1/test/test_v1_pipeline_spec.py` & `kfp-tekton-server-api-1.8.0rc2/test/test_v1_pipeline_spec.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc1/test/test_v1_pipeline_version.py` & `kfp-tekton-server-api-1.8.0rc2/test/test_v1_pipeline_version.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc1/test/test_v1_read_artifact_response.py` & `kfp-tekton-server-api-1.8.0rc2/test/test_v1_read_artifact_response.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc1/test/test_v1_relationship.py` & `kfp-tekton-server-api-1.8.0rc2/test/test_v1_relationship.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc1/test/test_v1_report_run_metrics_response.py` & `kfp-tekton-server-api-1.8.0rc2/test/test_v1_report_run_metrics_response.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc1/test/test_v1_resource_key.py` & `kfp-tekton-server-api-1.8.0rc2/test/test_v1_resource_key.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc1/test/test_v1_resource_reference.py` & `kfp-tekton-server-api-1.8.0rc2/test/test_v1_resource_reference.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc1/test/test_v1_resource_type.py` & `kfp-tekton-server-api-1.8.0rc2/test/test_v1_resource_type.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc1/test/test_v1_run.py` & `kfp-tekton-server-api-1.8.0rc2/test/test_v1_run.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc1/test/test_v1_run_detail.py` & `kfp-tekton-server-api-1.8.0rc2/test/test_v1_run_detail.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc1/test/test_v1_run_metric.py` & `kfp-tekton-server-api-1.8.0rc2/test/test_v1_run_metric.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc1/test/test_v1_run_storage_state.py` & `kfp-tekton-server-api-1.8.0rc2/test/test_v1_run_storage_state.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc1/test/test_v1_status.py` & `kfp-tekton-server-api-1.8.0rc2/test/test_v1_status.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc1/test/test_v1_trigger.py` & `kfp-tekton-server-api-1.8.0rc2/test/test_v1_trigger.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc1/test/test_v1_url.py` & `kfp-tekton-server-api-1.8.0rc2/test/test_v1_url.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc1/test/test_v1_value.py` & `kfp-tekton-server-api-1.8.0rc2/test/test_v1_value.py`

 * *Files identical despite different names*

