# Comparing `tmp/kfp-tekton-server-api-1.8.0rc2.tar.gz` & `tmp/kfp-tekton-server-api-1.8.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kfp-tekton-server-api-1.8.0rc2.tar", last modified: Thu Jul 13 21:36:56 2023, max compression
+gzip compressed data, was "kfp-tekton-server-api-1.8.0rc3.tar", last modified: Thu Jul 13 21:50:30 2023, max compression
```

## Comparing `kfp-tekton-server-api-1.8.0rc2.tar` & `kfp-tekton-server-api-1.8.0rc3.tar`

### file list

```diff
@@ -1,113 +1,113 @@
-drwxr-xr-x   0 tommyli    (501) staff       (20)        0 2023-07-13 21:36:56.959372 kfp-tekton-server-api-1.8.0rc2/
--rw-r--r--   0 tommyli    (501) staff       (20)    11357 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/LICENSE
--rw-r--r--   0 tommyli    (501) staff       (20)      457 2023-07-13 21:36:56.959588 kfp-tekton-server-api-1.8.0rc2/PKG-INFO
--rw-r--r--   0 tommyli    (501) staff       (20)    13066 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/README.md
-drwxr-xr-x   0 tommyli    (501) staff       (20)        0 2023-07-13 21:36:56.909678 kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/
--rw-r--r--   0 tommyli    (501) staff       (20)     4398 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/__init__.py
-drwxr-xr-x   0 tommyli    (501) staff       (20)        0 2023-07-13 21:36:56.915538 kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/api/
--rw-r--r--   0 tommyli    (501) staff       (20)      550 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/api/__init__.py
--rw-r--r--   0 tommyli    (501) staff       (20)    36823 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/api/experiment_service_api.py
--rw-r--r--   0 tommyli    (501) staff       (20)     5448 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/api/healthz_service_api.py
--rw-r--r--   0 tommyli    (501) staff       (20)    35425 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/api/job_service_api.py
--rw-r--r--   0 tommyli    (501) staff       (20)    69047 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/api/pipeline_service_api.py
--rw-r--r--   0 tommyli    (501) staff       (20)    13674 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/api/pipeline_upload_service_api.py
--rw-r--r--   0 tommyli    (501) staff       (20)    59741 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/api/run_service_api.py
--rw-r--r--   0 tommyli    (501) staff       (20)    26288 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/api_client.py
--rw-r--r--   0 tommyli    (501) staff       (20)    13322 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/configuration.py
--rw-r--r--   0 tommyli    (501) staff       (20)     3795 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/exceptions.py
-drwxr-xr-x   0 tommyli    (501) staff       (20)        0 2023-07-13 21:36:56.936177 kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/models/
--rw-r--r--   0 tommyli    (501) staff       (20)     3447 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/models/__init__.py
--rw-r--r--   0 tommyli    (501) staff       (20)     4658 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/models/googlerpc_status.py
--rw-r--r--   0 tommyli    (501) staff       (20)     3481 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/models/inline_object.py
--rw-r--r--   0 tommyli    (501) staff       (20)     2873 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/models/job_mode.py
--rw-r--r--   0 tommyli    (501) staff       (20)     4643 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/models/pipeline_spec_runtime_config.py
--rw-r--r--   0 tommyli    (501) staff       (20)    10425 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/models/protobuf_any.py
--rw-r--r--   0 tommyli    (501) staff       (20)     6709 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/models/report_run_metrics_response_report_run_metric_result.py
--rw-r--r--   0 tommyli    (501) staff       (20)     3178 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/models/report_run_metrics_response_report_run_metric_result_status.py
--rw-r--r--   0 tommyli    (501) staff       (20)     2896 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/models/run_metric_format.py
--rw-r--r--   0 tommyli    (501) staff       (20)     4712 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/models/v1_cron_schedule.py
--rw-r--r--   0 tommyli    (501) staff       (20)     7846 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/models/v1_experiment.py
--rw-r--r--   0 tommyli    (501) staff       (20)     2983 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/models/v1_experiment_storage_state.py
--rw-r--r--   0 tommyli    (501) staff       (20)     3470 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/models/v1_get_healthz_response.py
--rw-r--r--   0 tommyli    (501) staff       (20)     3762 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/models/v1_get_template_response.py
--rw-r--r--   0 tommyli    (501) staff       (20)    14740 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/models/v1_job.py
--rw-r--r--   0 tommyli    (501) staff       (20)     5594 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/models/v1_list_experiments_response.py
--rw-r--r--   0 tommyli    (501) staff       (20)     5272 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/models/v1_list_jobs_response.py
--rw-r--r--   0 tommyli    (501) staff       (20)     5542 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/models/v1_list_pipeline_versions_response.py
--rw-r--r--   0 tommyli    (501) staff       (20)     5398 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/models/v1_list_pipelines_response.py
--rw-r--r--   0 tommyli    (501) staff       (20)     5178 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/models/v1_list_runs_response.py
--rw-r--r--   0 tommyli    (501) staff       (20)     3869 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/models/v1_parameter.py
--rw-r--r--   0 tommyli    (501) staff       (20)     5006 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/models/v1_periodic_schedule.py
--rw-r--r--   0 tommyli    (501) staff       (20)    11586 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/models/v1_pipeline.py
--rw-r--r--   0 tommyli    (501) staff       (20)     5052 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/models/v1_pipeline_runtime.py
--rw-r--r--   0 tommyli    (501) staff       (20)     8397 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/models/v1_pipeline_spec.py
--rw-r--r--   0 tommyli    (501) staff       (20)    13714 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/models/v1_pipeline_version.py
--rw-r--r--   0 tommyli    (501) staff       (20)     3868 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/models/v1_read_artifact_response.py
--rw-r--r--   0 tommyli    (501) staff       (20)     2916 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/models/v1_relationship.py
--rw-r--r--   0 tommyli    (501) staff       (20)     3597 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/models/v1_report_run_metrics_response.py
--rw-r--r--   0 tommyli    (501) staff       (20)     3989 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/models/v1_resource_key.py
--rw-r--r--   0 tommyli    (501) staff       (20)     4894 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/models/v1_resource_reference.py
--rw-r--r--   0 tommyli    (501) staff       (20)     3057 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/models/v1_resource_type.py
--rw-r--r--   0 tommyli    (501) staff       (20)    14091 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/models/v1_run.py
--rw-r--r--   0 tommyli    (501) staff       (20)     4126 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/models/v1_run_detail.py
--rw-r--r--   0 tommyli    (501) staff       (20)     6333 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/models/v1_run_metric.py
--rw-r--r--   0 tommyli    (501) staff       (20)     2897 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/models/v1_run_storage_state.py
--rw-r--r--   0 tommyli    (501) staff       (20)     4504 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/models/v1_status.py
--rw-r--r--   0 tommyli    (501) staff       (20)     4362 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/models/v1_trigger.py
--rw-r--r--   0 tommyli    (501) staff       (20)     4289 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/models/v1_url.py
--rw-r--r--   0 tommyli    (501) staff       (20)     4806 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/models/v1_value.py
--rw-r--r--   0 tommyli    (501) staff       (20)    12334 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/rest.py
-drwxr-xr-x   0 tommyli    (501) staff       (20)        0 2023-07-13 21:36:56.912014 kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api.egg-info/
--rw-r--r--   0 tommyli    (501) staff       (20)      457 2023-07-13 21:36:56.000000 kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api.egg-info/PKG-INFO
--rw-r--r--   0 tommyli    (501) staff       (20)     4343 2023-07-13 21:36:56.000000 kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api.egg-info/SOURCES.txt
--rw-r--r--   0 tommyli    (501) staff       (20)        1 2023-07-13 21:36:56.000000 kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api.egg-info/dependency_links.txt
--rw-r--r--   0 tommyli    (501) staff       (20)       48 2023-07-13 21:36:56.000000 kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api.egg-info/requires.txt
--rw-r--r--   0 tommyli    (501) staff       (20)       22 2023-07-13 21:36:56.000000 kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api.egg-info/top_level.txt
--rw-r--r--   0 tommyli    (501) staff       (20)       69 2023-07-13 21:36:56.960267 kfp-tekton-server-api-1.8.0rc2/setup.cfg
--rw-r--r--   0 tommyli    (501) staff       (20)     1203 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/setup.py
-drwxr-xr-x   0 tommyli    (501) staff       (20)        0 2023-07-13 21:36:56.958890 kfp-tekton-server-api-1.8.0rc2/test/
--rw-r--r--   0 tommyli    (501) staff       (20)     2286 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/test/test_experiment_service_api.py
--rw-r--r--   0 tommyli    (501) staff       (20)     1622 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/test/test_googlerpc_status.py
--rw-r--r--   0 tommyli    (501) staff       (20)      971 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/test/test_healthz_service_api.py
--rw-r--r--   0 tommyli    (501) staff       (20)     1694 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/test/test_inline_object.py
--rw-r--r--   0 tommyli    (501) staff       (20)     1339 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/test/test_job_mode.py
--rw-r--r--   0 tommyli    (501) staff       (20)     1848 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/test/test_job_service_api.py
--rw-r--r--   0 tommyli    (501) staff       (20)     3721 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/test/test_pipeline_service_api.py
--rw-r--r--   0 tommyli    (501) staff       (20)     1842 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/test/test_pipeline_spec_runtime_config.py
--rw-r--r--   0 tommyli    (501) staff       (20)     1071 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/test/test_pipeline_upload_service_api.py
--rw-r--r--   0 tommyli    (501) staff       (20)     1476 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/test/test_protobuf_any.py
--rw-r--r--   0 tommyli    (501) staff       (20)     1915 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/test/test_report_run_metrics_response_report_run_metric_result.py
--rw-r--r--   0 tommyli    (501) staff       (20)     1837 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/test/test_report_run_metrics_response_report_run_metric_result_status.py
--rw-r--r--   0 tommyli    (501) staff       (20)     1429 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/test/test_run_metric_format.py
--rw-r--r--   0 tommyli    (501) staff       (20)     2682 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/test/test_run_service_api.py
--rw-r--r--   0 tommyli    (501) staff       (20)     1659 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/test/test_v1_cron_schedule.py
--rw-r--r--   0 tommyli    (501) staff       (20)     2104 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/test/test_v1_experiment.py
--rw-r--r--   0 tommyli    (501) staff       (20)     1530 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/test/test_v1_experiment_storage_state.py
--rw-r--r--   0 tommyli    (501) staff       (20)     1520 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/test/test_v1_get_healthz_response.py
--rw-r--r--   0 tommyli    (501) staff       (20)     1528 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/test/test_v1_get_template_response.py
--rw-r--r--   0 tommyli    (501) staff       (20)     4344 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/test/test_v1_job.py
--rw-r--r--   0 tommyli    (501) staff       (20)     2563 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/test/test_v1_list_experiments_response.py
--rw-r--r--   0 tommyli    (501) staff       (20)     5054 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/test/test_v1_list_jobs_response.py
--rw-r--r--   0 tommyli    (501) staff       (20)     3607 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/test/test_v1_list_pipeline_versions_response.py
--rw-r--r--   0 tommyli    (501) staff       (20)     4513 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/test/test_v1_list_pipelines_response.py
--rw-r--r--   0 tommyli    (501) staff       (20)     4306 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/test/test_v1_list_runs_response.py
--rw-r--r--   0 tommyli    (501) staff       (20)     1440 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/test/test_v1_parameter.py
--rw-r--r--   0 tommyli    (501) staff       (20)     1714 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/test/test_v1_periodic_schedule.py
--rw-r--r--   0 tommyli    (501) staff       (20)     4295 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/test/test_v1_pipeline.py
--rw-r--r--   0 tommyli    (501) staff       (20)     1533 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/test/test_v1_pipeline_runtime.py
--rw-r--r--   0 tommyli    (501) staff       (20)     2232 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/test/test_v1_pipeline_spec.py
--rw-r--r--   0 tommyli    (501) staff       (20)     3261 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/test/test_v1_pipeline_version.py
--rw-r--r--   0 tommyli    (501) staff       (20)     1538 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/test/test_v1_read_artifact_response.py
--rw-r--r--   0 tommyli    (501) staff       (20)     1416 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/test/test_v1_relationship.py
--rw-r--r--   0 tommyli    (501) staff       (20)     1934 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/test/test_v1_report_run_metrics_response.py
--rw-r--r--   0 tommyli    (501) staff       (20)     1481 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/test/test_v1_resource_key.py
--rw-r--r--   0 tommyli    (501) staff       (20)     1725 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/test/test_v1_resource_reference.py
--rw-r--r--   0 tommyli    (501) staff       (20)     1418 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/test/test_v1_resource_type.py
--rw-r--r--   0 tommyli    (501) staff       (20)     3628 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/test/test_v1_run.py
--rw-r--r--   0 tommyli    (501) staff       (20)     4134 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/test/test_v1_run_detail.py
--rw-r--r--   0 tommyli    (501) staff       (20)     1524 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/test/test_v1_run_metric.py
--rw-r--r--   0 tommyli    (501) staff       (20)     1453 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/test/test_v1_run_storage_state.py
--rw-r--r--   0 tommyli    (501) staff       (20)     1543 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/test/test_v1_status.py
--rw-r--r--   0 tommyli    (501) staff       (20)     2286 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/test/test_v1_trigger.py
--rw-r--r--   0 tommyli    (501) staff       (20)     1389 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/test/test_v1_url.py
--rw-r--r--   0 tommyli    (501) staff       (20)     1447 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc2/test/test_v1_value.py
+drwxr-xr-x   0 tommyli    (501) staff       (20)        0 2023-07-13 21:50:30.185585 kfp-tekton-server-api-1.8.0rc3/
+-rw-r--r--   0 tommyli    (501) staff       (20)    11357 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc3/LICENSE
+-rw-r--r--   0 tommyli    (501) staff       (20)      504 2023-07-13 21:50:30.185704 kfp-tekton-server-api-1.8.0rc3/PKG-INFO
+-rw-r--r--   0 tommyli    (501) staff       (20)    13066 2023-07-13 21:47:33.000000 kfp-tekton-server-api-1.8.0rc3/README.md
+drwxr-xr-x   0 tommyli    (501) staff       (20)        0 2023-07-13 21:50:30.150514 kfp-tekton-server-api-1.8.0rc3/kfp_tekton_server_api/
+-rw-r--r--   0 tommyli    (501) staff       (20)     4398 2023-07-13 21:46:34.000000 kfp-tekton-server-api-1.8.0rc3/kfp_tekton_server_api/__init__.py
+drwxr-xr-x   0 tommyli    (501) staff       (20)        0 2023-07-13 21:50:30.155926 kfp-tekton-server-api-1.8.0rc3/kfp_tekton_server_api/api/
+-rw-r--r--   0 tommyli    (501) staff       (20)      550 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc3/kfp_tekton_server_api/api/__init__.py
+-rw-r--r--   0 tommyli    (501) staff       (20)    36823 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc3/kfp_tekton_server_api/api/experiment_service_api.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     5448 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc3/kfp_tekton_server_api/api/healthz_service_api.py
+-rw-r--r--   0 tommyli    (501) staff       (20)    35425 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc3/kfp_tekton_server_api/api/job_service_api.py
+-rw-r--r--   0 tommyli    (501) staff       (20)    69047 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc3/kfp_tekton_server_api/api/pipeline_service_api.py
+-rw-r--r--   0 tommyli    (501) staff       (20)    13674 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc3/kfp_tekton_server_api/api/pipeline_upload_service_api.py
+-rw-r--r--   0 tommyli    (501) staff       (20)    59741 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc3/kfp_tekton_server_api/api/run_service_api.py
+-rw-r--r--   0 tommyli    (501) staff       (20)    26288 2023-07-13 21:46:42.000000 kfp-tekton-server-api-1.8.0rc3/kfp_tekton_server_api/api_client.py
+-rw-r--r--   0 tommyli    (501) staff       (20)    13322 2023-07-13 21:46:53.000000 kfp-tekton-server-api-1.8.0rc3/kfp_tekton_server_api/configuration.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     3795 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc3/kfp_tekton_server_api/exceptions.py
+drwxr-xr-x   0 tommyli    (501) staff       (20)        0 2023-07-13 21:50:30.170862 kfp-tekton-server-api-1.8.0rc3/kfp_tekton_server_api/models/
+-rw-r--r--   0 tommyli    (501) staff       (20)     3447 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc3/kfp_tekton_server_api/models/__init__.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     4658 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc3/kfp_tekton_server_api/models/googlerpc_status.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     3481 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc3/kfp_tekton_server_api/models/inline_object.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     2873 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc3/kfp_tekton_server_api/models/job_mode.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     4643 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc3/kfp_tekton_server_api/models/pipeline_spec_runtime_config.py
+-rw-r--r--   0 tommyli    (501) staff       (20)    10425 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc3/kfp_tekton_server_api/models/protobuf_any.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     6709 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc3/kfp_tekton_server_api/models/report_run_metrics_response_report_run_metric_result.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     3178 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc3/kfp_tekton_server_api/models/report_run_metrics_response_report_run_metric_result_status.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     2896 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc3/kfp_tekton_server_api/models/run_metric_format.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     4712 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc3/kfp_tekton_server_api/models/v1_cron_schedule.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     7846 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc3/kfp_tekton_server_api/models/v1_experiment.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     2983 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc3/kfp_tekton_server_api/models/v1_experiment_storage_state.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     3470 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc3/kfp_tekton_server_api/models/v1_get_healthz_response.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     3762 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc3/kfp_tekton_server_api/models/v1_get_template_response.py
+-rw-r--r--   0 tommyli    (501) staff       (20)    14740 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc3/kfp_tekton_server_api/models/v1_job.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     5594 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc3/kfp_tekton_server_api/models/v1_list_experiments_response.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     5272 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc3/kfp_tekton_server_api/models/v1_list_jobs_response.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     5542 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc3/kfp_tekton_server_api/models/v1_list_pipeline_versions_response.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     5398 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc3/kfp_tekton_server_api/models/v1_list_pipelines_response.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     5178 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc3/kfp_tekton_server_api/models/v1_list_runs_response.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     3869 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc3/kfp_tekton_server_api/models/v1_parameter.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     5006 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc3/kfp_tekton_server_api/models/v1_periodic_schedule.py
+-rw-r--r--   0 tommyli    (501) staff       (20)    10941 2023-07-13 21:38:28.000000 kfp-tekton-server-api-1.8.0rc3/kfp_tekton_server_api/models/v1_pipeline.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     5052 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc3/kfp_tekton_server_api/models/v1_pipeline_runtime.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     8397 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc3/kfp_tekton_server_api/models/v1_pipeline_spec.py
+-rw-r--r--   0 tommyli    (501) staff       (20)    10246 2023-07-13 21:39:25.000000 kfp-tekton-server-api-1.8.0rc3/kfp_tekton_server_api/models/v1_pipeline_version.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     3868 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc3/kfp_tekton_server_api/models/v1_read_artifact_response.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     2916 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc3/kfp_tekton_server_api/models/v1_relationship.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     3597 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc3/kfp_tekton_server_api/models/v1_report_run_metrics_response.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     3989 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc3/kfp_tekton_server_api/models/v1_resource_key.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     4894 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc3/kfp_tekton_server_api/models/v1_resource_reference.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     3057 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc3/kfp_tekton_server_api/models/v1_resource_type.py
+-rw-r--r--   0 tommyli    (501) staff       (20)    14091 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc3/kfp_tekton_server_api/models/v1_run.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     4126 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc3/kfp_tekton_server_api/models/v1_run_detail.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     6333 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc3/kfp_tekton_server_api/models/v1_run_metric.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     2897 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc3/kfp_tekton_server_api/models/v1_run_storage_state.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     4504 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc3/kfp_tekton_server_api/models/v1_status.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     4362 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc3/kfp_tekton_server_api/models/v1_trigger.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     4289 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc3/kfp_tekton_server_api/models/v1_url.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     4806 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc3/kfp_tekton_server_api/models/v1_value.py
+-rw-r--r--   0 tommyli    (501) staff       (20)    12334 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc3/kfp_tekton_server_api/rest.py
+drwxr-xr-x   0 tommyli    (501) staff       (20)        0 2023-07-13 21:50:30.152828 kfp-tekton-server-api-1.8.0rc3/kfp_tekton_server_api.egg-info/
+-rw-r--r--   0 tommyli    (501) staff       (20)      504 2023-07-13 21:50:30.000000 kfp-tekton-server-api-1.8.0rc3/kfp_tekton_server_api.egg-info/PKG-INFO
+-rw-r--r--   0 tommyli    (501) staff       (20)     4343 2023-07-13 21:50:30.000000 kfp-tekton-server-api-1.8.0rc3/kfp_tekton_server_api.egg-info/SOURCES.txt
+-rw-r--r--   0 tommyli    (501) staff       (20)        1 2023-07-13 21:50:30.000000 kfp-tekton-server-api-1.8.0rc3/kfp_tekton_server_api.egg-info/dependency_links.txt
+-rw-r--r--   0 tommyli    (501) staff       (20)       48 2023-07-13 21:50:30.000000 kfp-tekton-server-api-1.8.0rc3/kfp_tekton_server_api.egg-info/requires.txt
+-rw-r--r--   0 tommyli    (501) staff       (20)       22 2023-07-13 21:50:30.000000 kfp-tekton-server-api-1.8.0rc3/kfp_tekton_server_api.egg-info/top_level.txt
+-rw-r--r--   0 tommyli    (501) staff       (20)       69 2023-07-13 21:50:30.186150 kfp-tekton-server-api-1.8.0rc3/setup.cfg
+-rw-r--r--   0 tommyli    (501) staff       (20)     1247 2023-07-13 21:50:24.000000 kfp-tekton-server-api-1.8.0rc3/setup.py
+drwxr-xr-x   0 tommyli    (501) staff       (20)        0 2023-07-13 21:50:30.185304 kfp-tekton-server-api-1.8.0rc3/test/
+-rw-r--r--   0 tommyli    (501) staff       (20)     2286 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc3/test/test_experiment_service_api.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     1622 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc3/test/test_googlerpc_status.py
+-rw-r--r--   0 tommyli    (501) staff       (20)      971 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc3/test/test_healthz_service_api.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     1694 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc3/test/test_inline_object.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     1339 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc3/test/test_job_mode.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     1848 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc3/test/test_job_service_api.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     3721 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc3/test/test_pipeline_service_api.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     1842 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc3/test/test_pipeline_spec_runtime_config.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     1071 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc3/test/test_pipeline_upload_service_api.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     1476 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc3/test/test_protobuf_any.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     1915 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc3/test/test_report_run_metrics_response_report_run_metric_result.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     1837 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc3/test/test_report_run_metrics_response_report_run_metric_result_status.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     1429 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc3/test/test_run_metric_format.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     2682 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc3/test/test_run_service_api.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     1659 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc3/test/test_v1_cron_schedule.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     2104 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc3/test/test_v1_experiment.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     1530 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc3/test/test_v1_experiment_storage_state.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     1520 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc3/test/test_v1_get_healthz_response.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     1528 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc3/test/test_v1_get_template_response.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     4344 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc3/test/test_v1_job.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     2563 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc3/test/test_v1_list_experiments_response.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     5054 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc3/test/test_v1_list_jobs_response.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     3607 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc3/test/test_v1_list_pipeline_versions_response.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     4513 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc3/test/test_v1_list_pipelines_response.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     4306 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc3/test/test_v1_list_runs_response.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     1440 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc3/test/test_v1_parameter.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     1714 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc3/test/test_v1_periodic_schedule.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     4295 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc3/test/test_v1_pipeline.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     1533 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc3/test/test_v1_pipeline_runtime.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     2232 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc3/test/test_v1_pipeline_spec.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     3261 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc3/test/test_v1_pipeline_version.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     1538 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc3/test/test_v1_read_artifact_response.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     1416 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc3/test/test_v1_relationship.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     1934 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc3/test/test_v1_report_run_metrics_response.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     1481 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc3/test/test_v1_resource_key.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     1725 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc3/test/test_v1_resource_reference.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     1418 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc3/test/test_v1_resource_type.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     3628 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc3/test/test_v1_run.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     4134 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc3/test/test_v1_run_detail.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     1524 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc3/test/test_v1_run_metric.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     1453 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc3/test/test_v1_run_storage_state.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     1543 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc3/test/test_v1_status.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     2286 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc3/test/test_v1_trigger.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     1389 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc3/test/test_v1_url.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     1447 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc3/test/test_v1_value.py
```

### Comparing `kfp-tekton-server-api-1.8.0rc2/LICENSE` & `kfp-tekton-server-api-1.8.0rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc2/README.md` & `kfp-tekton-server-api-1.8.0rc3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # kfp-tekton-server-api
 This file contains REST API specification for Kubeflow Pipelines. The file is autogenerated from the swagger definition.
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 1.8.0rc2
-- Package version: 1.8.0rc2
+- API version: 1.8.0rc3
+- Package version: 1.8.0rc3
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 For more information, please visit [https://www.google.com](https://www.google.com)
 
 ## Requirements.
 
-Python 2.7 and 3.4+
+Python 2.7 and 3.7+
 
 ## Installation & Usage
 ### pip install
 
 If the python package is hosted on a repository, you can install directly using:
 
 ```sh
```

### Comparing `kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/__init__.py` & `kfp-tekton-server-api-1.8.0rc3/kfp_tekton_server_api/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     Contact: kubeflow-pipelines@google.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
-__version__ = "1.8.0rc2"
+__version__ = "1.8.0rc3"
 
 # import apis into sdk package
 from kfp_tekton_server_api.api.experiment_service_api import ExperimentServiceApi
 from kfp_tekton_server_api.api.healthz_service_api import HealthzServiceApi
 from kfp_tekton_server_api.api.job_service_api import JobServiceApi
 from kfp_tekton_server_api.api.pipeline_service_api import PipelineServiceApi
 from kfp_tekton_server_api.api.pipeline_upload_service_api import PipelineUploadServiceApi
```

### Comparing `kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/api/__init__.py` & `kfp-tekton-server-api-1.8.0rc3/kfp_tekton_server_api/api/__init__.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/api/experiment_service_api.py` & `kfp-tekton-server-api-1.8.0rc3/kfp_tekton_server_api/api/experiment_service_api.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/api/healthz_service_api.py` & `kfp-tekton-server-api-1.8.0rc3/kfp_tekton_server_api/api/healthz_service_api.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/api/job_service_api.py` & `kfp-tekton-server-api-1.8.0rc3/kfp_tekton_server_api/api/job_service_api.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/api/pipeline_service_api.py` & `kfp-tekton-server-api-1.8.0rc3/kfp_tekton_server_api/api/pipeline_service_api.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/api/pipeline_upload_service_api.py` & `kfp-tekton-server-api-1.8.0rc3/kfp_tekton_server_api/api/pipeline_upload_service_api.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/api/run_service_api.py` & `kfp-tekton-server-api-1.8.0rc3/kfp_tekton_server_api/api/run_service_api.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/api_client.py` & `kfp-tekton-server-api-1.8.0rc3/kfp_tekton_server_api/api_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,15 +74,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/1.8.0rc2/python'
+        self.user_agent = 'OpenAPI-Generator/1.8.0rc3/python'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/configuration.py` & `kfp-tekton-server-api-1.8.0rc3/kfp_tekton_server_api/configuration.py`

 * *Files identical despite different names*

```diff
@@ -347,16 +347,16 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 1.8.0rc2\n"\
-               "SDK Package Version: 1.8.0rc2".\
+               "Version of the API: 1.8.0rc3\n"\
+               "SDK Package Version: 1.8.0rc3".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/exceptions.py` & `kfp-tekton-server-api-1.8.0rc3/kfp_tekton_server_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/models/__init__.py` & `kfp-tekton-server-api-1.8.0rc3/kfp_tekton_server_api/models/__init__.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/models/googlerpc_status.py` & `kfp-tekton-server-api-1.8.0rc3/kfp_tekton_server_api/models/googlerpc_status.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/models/inline_object.py` & `kfp-tekton-server-api-1.8.0rc3/kfp_tekton_server_api/models/inline_object.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/models/job_mode.py` & `kfp-tekton-server-api-1.8.0rc3/kfp_tekton_server_api/models/job_mode.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/models/pipeline_spec_runtime_config.py` & `kfp-tekton-server-api-1.8.0rc3/kfp_tekton_server_api/models/pipeline_spec_runtime_config.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/models/protobuf_any.py` & `kfp-tekton-server-api-1.8.0rc3/kfp_tekton_server_api/models/protobuf_any.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/models/report_run_metrics_response_report_run_metric_result.py` & `kfp-tekton-server-api-1.8.0rc3/kfp_tekton_server_api/models/report_run_metrics_response_report_run_metric_result.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/models/report_run_metrics_response_report_run_metric_result_status.py` & `kfp-tekton-server-api-1.8.0rc3/kfp_tekton_server_api/models/report_run_metrics_response_report_run_metric_result_status.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/models/run_metric_format.py` & `kfp-tekton-server-api-1.8.0rc3/kfp_tekton_server_api/models/run_metric_format.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/models/v1_cron_schedule.py` & `kfp-tekton-server-api-1.8.0rc3/kfp_tekton_server_api/models/v1_cron_schedule.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/models/v1_experiment.py` & `kfp-tekton-server-api-1.8.0rc3/kfp_tekton_server_api/models/v1_experiment.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/models/v1_experiment_storage_state.py` & `kfp-tekton-server-api-1.8.0rc3/kfp_tekton_server_api/models/v1_experiment_storage_state.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/models/v1_get_healthz_response.py` & `kfp-tekton-server-api-1.8.0rc3/kfp_tekton_server_api/models/v1_get_healthz_response.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/models/v1_get_template_response.py` & `kfp-tekton-server-api-1.8.0rc3/kfp_tekton_server_api/models/v1_get_template_response.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/models/v1_job.py` & `kfp-tekton-server-api-1.8.0rc3/kfp_tekton_server_api/models/v1_job.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/models/v1_list_experiments_response.py` & `kfp-tekton-server-api-1.8.0rc3/kfp_tekton_server_api/models/v1_list_experiments_response.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/models/v1_list_jobs_response.py` & `kfp-tekton-server-api-1.8.0rc3/kfp_tekton_server_api/models/v1_list_jobs_response.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/models/v1_list_pipeline_versions_response.py` & `kfp-tekton-server-api-1.8.0rc3/kfp_tekton_server_api/models/v1_list_pipeline_versions_response.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/models/v1_list_pipelines_response.py` & `kfp-tekton-server-api-1.8.0rc3/kfp_tekton_server_api/models/v1_list_pipelines_response.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/models/v1_list_runs_response.py` & `kfp-tekton-server-api-1.8.0rc3/kfp_tekton_server_api/models/v1_list_runs_response.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/models/v1_parameter.py` & `kfp-tekton-server-api-1.8.0rc3/kfp_tekton_server_api/models/v1_parameter.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/models/v1_periodic_schedule.py` & `kfp-tekton-server-api-1.8.0rc3/kfp_tekton_server_api/models/v1_periodic_schedule.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/models/v1_pipeline.py` & `kfp-tekton-server-api-1.8.0rc3/kfp_tekton_server_api/models/v1_pipeline.py`

 * *Files 6% similar despite different names*

```diff
@@ -54,30 +54,29 @@
         'url': 'url',
         'error': 'error',
         'default_version': 'defaultVersion',
         'resource_references': 'resourceReferences',
         'created_at': 'created_at'
     }
 
-    def __init__(self, id=None, created_at=None, name=None, description=None, parameters=None, url=None, error=None, default_version=None, resource_references=None, created_at=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, id=None, created_at=None, name=None, description=None, parameters=None, url=None, error=None, default_version=None, resource_references=None, local_vars_configuration=None):  # noqa: E501
         """V1Pipeline - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._id = None
         self._created_at = None
         self._name = None
         self._description = None
         self._parameters = None
         self._url = None
         self._error = None
         self._default_version = None
         self._resource_references = None
-        self._created_at = None
         self.discriminator = None
 
         if id is not None:
             self.id = id
         if created_at is not None:
             self.created_at = created_at
         if name is not None:
@@ -90,16 +89,14 @@
             self.url = url
         if error is not None:
             self.error = error
         if default_version is not None:
             self.default_version = default_version
         if resource_references is not None:
             self.resource_references = resource_references
-        if created_at is not None:
-            self.created_at = created_at
 
     @property
     def id(self):
         """Gets the id of this V1Pipeline.  # noqa: E501
 
         Output. Unique pipeline ID. Generated by API server.  # noqa: E501
 
@@ -296,35 +293,14 @@
 
         :param resource_references: The resource_references of this V1Pipeline.  # noqa: E501
         :type resource_references: list[V1ResourceReference]
         """
 
         self._resource_references = resource_references
 
-    @property
-    def created_at(self):
-        """Gets the created_at of this V1Pipeline.  # noqa: E501
-
-
-        :return: The created_at of this V1Pipeline.  # noqa: E501
-        :rtype: datetime
-        """
-        return self._created_at
-
-    @created_at.setter
-    def created_at(self, created_at):
-        """Sets the created_at of this V1Pipeline.
-
-
-        :param created_at: The created_at of this V1Pipeline.  # noqa: E501
-        :type created_at: datetime
-        """
-
-        self._created_at = created_at
-
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
             if isinstance(value, list):
```

### Comparing `kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/models/v1_pipeline_runtime.py` & `kfp-tekton-server-api-1.8.0rc3/kfp_tekton_server_api/models/v1_pipeline_runtime.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/models/v1_pipeline_spec.py` & `kfp-tekton-server-api-1.8.0rc3/kfp_tekton_server_api/models/v1_pipeline_spec.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/models/v1_pipeline_version.py` & `kfp-tekton-server-api-1.8.0rc3/kfp_tekton_server_api/models/v1_pipeline_version.py`

 * *Files 20% similar despite different names*

```diff
@@ -58,32 +58,28 @@
         'description': 'description',
         'created_at': 'created_at',
         'code_source_url': 'code_source_url',
         'package_url': 'package_url',
         'resource_references': 'resource_references'
     }
 
-    def __init__(self, id=None, name=None, created_at=None, parameters=None, code_source_url=None, package_url=None, resource_references=None, description=None, created_at=None, code_source_url=None, package_url=None, resource_references=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, id=None, name=None, created_at=None, parameters=None, code_source_url=None, package_url=None, resource_references=None, description=None, local_vars_configuration=None):  # noqa: E501
         """V1PipelineVersion - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._id = None
         self._name = None
         self._created_at = None
         self._parameters = None
         self._code_source_url = None
         self._package_url = None
         self._resource_references = None
         self._description = None
-        self._created_at = None
-        self._code_source_url = None
-        self._package_url = None
-        self._resource_references = None
         self.discriminator = None
 
         if id is not None:
             self.id = id
         if name is not None:
             self.name = name
         if created_at is not None:
@@ -94,22 +90,14 @@
             self.code_source_url = code_source_url
         if package_url is not None:
             self.package_url = package_url
         if resource_references is not None:
             self.resource_references = resource_references
         if description is not None:
             self.description = description
-        if created_at is not None:
-            self.created_at = created_at
-        if code_source_url is not None:
-            self.code_source_url = code_source_url
-        if package_url is not None:
-            self.package_url = package_url
-        if resource_references is not None:
-            self.resource_references = resource_references
 
     @property
     def id(self):
         """Gets the id of this V1PipelineVersion.  # noqa: E501
 
         Output. Unique version ID. Generated by API server.  # noqa: E501
 
@@ -285,104 +273,14 @@
 
         :param description: The description of this V1PipelineVersion.  # noqa: E501
         :type description: str
         """
 
         self._description = description
 
-    @property
-    def created_at(self):
-        """Gets the created_at of this V1PipelineVersion.  # noqa: E501
-
-        Output. The time this pipeline version is created.  # noqa: E501
-
-        :return: The created_at of this V1PipelineVersion.  # noqa: E501
-        :rtype: datetime
-        """
-        return self._created_at
-
-    @created_at.setter
-    def created_at(self, created_at):
-        """Sets the created_at of this V1PipelineVersion.
-
-        Output. The time this pipeline version is created.  # noqa: E501
-
-        :param created_at: The created_at of this V1PipelineVersion.  # noqa: E501
-        :type created_at: datetime
-        """
-
-        self._created_at = created_at
-
-    @property
-    def code_source_url(self):
-        """Gets the code_source_url of this V1PipelineVersion.  # noqa: E501
-
-        Input. Optional. Pipeline version code source.  # noqa: E501
-
-        :return: The code_source_url of this V1PipelineVersion.  # noqa: E501
-        :rtype: str
-        """
-        return self._code_source_url
-
-    @code_source_url.setter
-    def code_source_url(self, code_source_url):
-        """Sets the code_source_url of this V1PipelineVersion.
-
-        Input. Optional. Pipeline version code source.  # noqa: E501
-
-        :param code_source_url: The code_source_url of this V1PipelineVersion.  # noqa: E501
-        :type code_source_url: str
-        """
-
-        self._code_source_url = code_source_url
-
-    @property
-    def package_url(self):
-        """Gets the package_url of this V1PipelineVersion.  # noqa: E501
-
-
-        :return: The package_url of this V1PipelineVersion.  # noqa: E501
-        :rtype: V1Url
-        """
-        return self._package_url
-
-    @package_url.setter
-    def package_url(self, package_url):
-        """Sets the package_url of this V1PipelineVersion.
-
-
-        :param package_url: The package_url of this V1PipelineVersion.  # noqa: E501
-        :type package_url: V1Url
-        """
-
-        self._package_url = package_url
-
-    @property
-    def resource_references(self):
-        """Gets the resource_references of this V1PipelineVersion.  # noqa: E501
-
-        Input. Required. E.g., specify which pipeline this pipeline version belongs to.  # noqa: E501
-
-        :return: The resource_references of this V1PipelineVersion.  # noqa: E501
-        :rtype: list[V1ResourceReference]
-        """
-        return self._resource_references
-
-    @resource_references.setter
-    def resource_references(self, resource_references):
-        """Sets the resource_references of this V1PipelineVersion.
-
-        Input. Required. E.g., specify which pipeline this pipeline version belongs to.  # noqa: E501
-
-        :param resource_references: The resource_references of this V1PipelineVersion.  # noqa: E501
-        :type resource_references: list[V1ResourceReference]
-        """
-
-        self._resource_references = resource_references
-
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
             if isinstance(value, list):
```

### Comparing `kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/models/v1_read_artifact_response.py` & `kfp-tekton-server-api-1.8.0rc3/kfp_tekton_server_api/models/v1_read_artifact_response.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/models/v1_relationship.py` & `kfp-tekton-server-api-1.8.0rc3/kfp_tekton_server_api/models/v1_relationship.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/models/v1_report_run_metrics_response.py` & `kfp-tekton-server-api-1.8.0rc3/kfp_tekton_server_api/models/v1_report_run_metrics_response.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/models/v1_resource_key.py` & `kfp-tekton-server-api-1.8.0rc3/kfp_tekton_server_api/models/v1_resource_key.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/models/v1_resource_reference.py` & `kfp-tekton-server-api-1.8.0rc3/kfp_tekton_server_api/models/v1_resource_reference.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/models/v1_resource_type.py` & `kfp-tekton-server-api-1.8.0rc3/kfp_tekton_server_api/models/v1_resource_type.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/models/v1_run.py` & `kfp-tekton-server-api-1.8.0rc3/kfp_tekton_server_api/models/v1_run.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/models/v1_run_detail.py` & `kfp-tekton-server-api-1.8.0rc3/kfp_tekton_server_api/models/v1_run_detail.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/models/v1_run_metric.py` & `kfp-tekton-server-api-1.8.0rc3/kfp_tekton_server_api/models/v1_run_metric.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/models/v1_run_storage_state.py` & `kfp-tekton-server-api-1.8.0rc3/kfp_tekton_server_api/models/v1_run_storage_state.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/models/v1_status.py` & `kfp-tekton-server-api-1.8.0rc3/kfp_tekton_server_api/models/v1_status.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/models/v1_trigger.py` & `kfp-tekton-server-api-1.8.0rc3/kfp_tekton_server_api/models/v1_trigger.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/models/v1_url.py` & `kfp-tekton-server-api-1.8.0rc3/kfp_tekton_server_api/models/v1_url.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/models/v1_value.py` & `kfp-tekton-server-api-1.8.0rc3/kfp_tekton_server_api/models/v1_value.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api/rest.py` & `kfp-tekton-server-api-1.8.0rc3/kfp_tekton_server_api/rest.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc2/kfp_tekton_server_api.egg-info/SOURCES.txt` & `kfp-tekton-server-api-1.8.0rc3/kfp_tekton_server_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc2/setup.py` & `kfp-tekton-server-api-1.8.0rc3/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 # coding: utf-8
 
 """
-    Kubeflow Pipelines API
+    Kubeflow Pipelines on Tekton API
 
-    This file contains REST API specification for Kubeflow Pipelines. The file is autogenerated from the swagger definition.
+    This file contains REST API specification for Kubeflow Pipelines on Tekton. The file is autogenerated from the swagger definition.
 
-    Contact: kubeflow-pipelines@google.com
+    Contact: tommy.chaoping.li@ibm.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "kfp-tekton-server-api"
-VERSION = "1.8.0rc2"
+VERSION = "1.8.0rc3"
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
-    description="Kubeflow Pipelines API",
-    author="kubeflow",
-    author_email="kubeflow-pipelines@google.com",
+    description="Kubeflow Pipelines on Tekton API",
+    author="kfp-tekton",
+    author_email="tommy.chaoping.li@ibm.com",
     url="https://github.com/kubeflow/kfp-tekton",
-    keywords=["OpenAPI", "OpenAPI-Generator", "Kubeflow Pipelines API"],
+    keywords=["OpenAPI", "OpenAPI-Generator", "Kubeflow Pipelines on Tekton API"],
     install_requires=REQUIRES,
     packages=find_packages(exclude=["test", "tests"]),
     include_package_data=True,
     license="Apache 2.0",
     long_description="""\
-    This file contains REST API specification for Kubeflow Pipelines. The file is autogenerated from the swagger definition.  # noqa: E501
+    This file contains REST API specification for Kubeflow Pipelines on Tekton. The file is autogenerated from the swagger definition.  # noqa: E501
     """
 )
```

### Comparing `kfp-tekton-server-api-1.8.0rc2/test/test_experiment_service_api.py` & `kfp-tekton-server-api-1.8.0rc3/test/test_experiment_service_api.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc2/test/test_googlerpc_status.py` & `kfp-tekton-server-api-1.8.0rc3/test/test_googlerpc_status.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc2/test/test_healthz_service_api.py` & `kfp-tekton-server-api-1.8.0rc3/test/test_healthz_service_api.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc2/test/test_inline_object.py` & `kfp-tekton-server-api-1.8.0rc3/test/test_inline_object.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc2/test/test_job_mode.py` & `kfp-tekton-server-api-1.8.0rc3/test/test_job_mode.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc2/test/test_job_service_api.py` & `kfp-tekton-server-api-1.8.0rc3/test/test_job_service_api.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc2/test/test_pipeline_service_api.py` & `kfp-tekton-server-api-1.8.0rc3/test/test_pipeline_service_api.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc2/test/test_pipeline_spec_runtime_config.py` & `kfp-tekton-server-api-1.8.0rc3/test/test_pipeline_spec_runtime_config.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc2/test/test_pipeline_upload_service_api.py` & `kfp-tekton-server-api-1.8.0rc3/test/test_pipeline_upload_service_api.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc2/test/test_protobuf_any.py` & `kfp-tekton-server-api-1.8.0rc3/test/test_protobuf_any.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc2/test/test_report_run_metrics_response_report_run_metric_result.py` & `kfp-tekton-server-api-1.8.0rc3/test/test_report_run_metrics_response_report_run_metric_result.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc2/test/test_report_run_metrics_response_report_run_metric_result_status.py` & `kfp-tekton-server-api-1.8.0rc3/test/test_report_run_metrics_response_report_run_metric_result_status.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc2/test/test_run_metric_format.py` & `kfp-tekton-server-api-1.8.0rc3/test/test_run_metric_format.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc2/test/test_run_service_api.py` & `kfp-tekton-server-api-1.8.0rc3/test/test_run_service_api.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc2/test/test_v1_cron_schedule.py` & `kfp-tekton-server-api-1.8.0rc3/test/test_v1_cron_schedule.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc2/test/test_v1_experiment.py` & `kfp-tekton-server-api-1.8.0rc3/test/test_v1_experiment.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc2/test/test_v1_experiment_storage_state.py` & `kfp-tekton-server-api-1.8.0rc3/test/test_v1_experiment_storage_state.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc2/test/test_v1_get_healthz_response.py` & `kfp-tekton-server-api-1.8.0rc3/test/test_v1_get_healthz_response.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc2/test/test_v1_get_template_response.py` & `kfp-tekton-server-api-1.8.0rc3/test/test_v1_get_template_response.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc2/test/test_v1_job.py` & `kfp-tekton-server-api-1.8.0rc3/test/test_v1_job.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc2/test/test_v1_list_experiments_response.py` & `kfp-tekton-server-api-1.8.0rc3/test/test_v1_list_experiments_response.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc2/test/test_v1_list_jobs_response.py` & `kfp-tekton-server-api-1.8.0rc3/test/test_v1_list_jobs_response.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc2/test/test_v1_list_pipeline_versions_response.py` & `kfp-tekton-server-api-1.8.0rc3/test/test_v1_list_pipeline_versions_response.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc2/test/test_v1_list_pipelines_response.py` & `kfp-tekton-server-api-1.8.0rc3/test/test_v1_list_pipelines_response.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc2/test/test_v1_list_runs_response.py` & `kfp-tekton-server-api-1.8.0rc3/test/test_v1_list_runs_response.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc2/test/test_v1_parameter.py` & `kfp-tekton-server-api-1.8.0rc3/test/test_v1_parameter.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc2/test/test_v1_periodic_schedule.py` & `kfp-tekton-server-api-1.8.0rc3/test/test_v1_periodic_schedule.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc2/test/test_v1_pipeline.py` & `kfp-tekton-server-api-1.8.0rc3/test/test_v1_pipeline.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc2/test/test_v1_pipeline_runtime.py` & `kfp-tekton-server-api-1.8.0rc3/test/test_v1_pipeline_runtime.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc2/test/test_v1_pipeline_spec.py` & `kfp-tekton-server-api-1.8.0rc3/test/test_v1_pipeline_spec.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc2/test/test_v1_pipeline_version.py` & `kfp-tekton-server-api-1.8.0rc3/test/test_v1_pipeline_version.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc2/test/test_v1_read_artifact_response.py` & `kfp-tekton-server-api-1.8.0rc3/test/test_v1_read_artifact_response.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc2/test/test_v1_relationship.py` & `kfp-tekton-server-api-1.8.0rc3/test/test_v1_relationship.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc2/test/test_v1_report_run_metrics_response.py` & `kfp-tekton-server-api-1.8.0rc3/test/test_v1_report_run_metrics_response.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc2/test/test_v1_resource_key.py` & `kfp-tekton-server-api-1.8.0rc3/test/test_v1_resource_key.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc2/test/test_v1_resource_reference.py` & `kfp-tekton-server-api-1.8.0rc3/test/test_v1_resource_reference.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc2/test/test_v1_resource_type.py` & `kfp-tekton-server-api-1.8.0rc3/test/test_v1_resource_type.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc2/test/test_v1_run.py` & `kfp-tekton-server-api-1.8.0rc3/test/test_v1_run.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc2/test/test_v1_run_detail.py` & `kfp-tekton-server-api-1.8.0rc3/test/test_v1_run_detail.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc2/test/test_v1_run_metric.py` & `kfp-tekton-server-api-1.8.0rc3/test/test_v1_run_metric.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc2/test/test_v1_run_storage_state.py` & `kfp-tekton-server-api-1.8.0rc3/test/test_v1_run_storage_state.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc2/test/test_v1_status.py` & `kfp-tekton-server-api-1.8.0rc3/test/test_v1_status.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc2/test/test_v1_trigger.py` & `kfp-tekton-server-api-1.8.0rc3/test/test_v1_trigger.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc2/test/test_v1_url.py` & `kfp-tekton-server-api-1.8.0rc3/test/test_v1_url.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc2/test/test_v1_value.py` & `kfp-tekton-server-api-1.8.0rc3/test/test_v1_value.py`

 * *Files identical despite different names*

