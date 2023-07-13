# Comparing `tmp/lyteidl-0.2.0a0.tar.gz` & `tmp/lyteidl-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lyteidl-0.2.0a0.tar", last modified: Tue Nov  8 22:43:00 2022, max compression
+gzip compressed data, was "lyteidl-0.2.1.tar", last modified: Thu Jul 13 19:32:11 2023, max compression
```

## Comparing `lyteidl-0.2.0a0.tar` & `lyteidl-0.2.1.tar`

### file list

```diff
@@ -1,130 +1,171 @@
-drwxr-xr-x   0 maximsmol   (501) staff       (20)        0 2022-11-08 22:43:00.315794 lyteidl-0.2.0a0/
--rw-r--r--   0 maximsmol   (501) staff       (20)    11341 2022-05-21 19:31:58.000000 lyteidl-0.2.0a0/LICENSE
--rw-r--r--   0 maximsmol   (501) staff       (20)       89 2022-05-21 19:31:58.000000 lyteidl-0.2.0a0/NOTICE
--rw-r--r--   0 maximsmol   (501) staff       (20)      235 2022-11-08 22:43:00.315979 lyteidl-0.2.0a0/PKG-INFO
--rw-r--r--   0 maximsmol   (501) staff       (20)     2742 2022-05-21 19:31:58.000000 lyteidl-0.2.0a0/README.md
-drwxr-xr-x   0 maximsmol   (501) staff       (20)        0 2022-11-08 22:43:00.236043 lyteidl-0.2.0a0/gen/
-drwxr-xr-x   0 maximsmol   (501) staff       (20)        0 2022-11-08 22:43:00.237548 lyteidl-0.2.0a0/gen/pb_python/
-drwxr-xr-x   0 maximsmol   (501) staff       (20)        0 2022-11-08 22:43:00.239218 lyteidl-0.2.0a0/gen/pb_python/flyteidl/
--rw-r--r--   0 maximsmol   (501) staff       (20)        0 2022-11-02 18:01:40.000000 lyteidl-0.2.0a0/gen/pb_python/flyteidl/__init__.py
-drwxr-xr-x   0 maximsmol   (501) staff       (20)        0 2022-11-08 22:43:00.250556 lyteidl-0.2.0a0/gen/pb_python/flyteidl/admin/
--rw-r--r--   0 maximsmol   (501) staff       (20)        0 2022-11-02 18:01:41.000000 lyteidl-0.2.0a0/gen/pb_python/flyteidl/admin/__init__.py
--rw-r--r--   0 maximsmol   (501) staff       (20)     8661 2022-11-02 18:01:41.000000 lyteidl-0.2.0a0/gen/pb_python/flyteidl/admin/cluster_assignment_pb2.py
--rw-r--r--   0 maximsmol   (501) staff       (20)       83 2022-11-02 18:01:41.000000 lyteidl-0.2.0a0/gen/pb_python/flyteidl/admin/cluster_assignment_pb2_grpc.py
--rw-r--r--   0 maximsmol   (501) staff       (20)    50730 2022-11-02 18:01:41.000000 lyteidl-0.2.0a0/gen/pb_python/flyteidl/admin/common_pb2.py
--rw-r--r--   0 maximsmol   (501) staff       (20)       83 2022-11-02 18:01:41.000000 lyteidl-0.2.0a0/gen/pb_python/flyteidl/admin/common_pb2_grpc.py
--rw-r--r--   0 maximsmol   (501) staff       (20)    15485 2022-11-02 18:01:41.000000 lyteidl-0.2.0a0/gen/pb_python/flyteidl/admin/event_pb2.py
--rw-r--r--   0 maximsmol   (501) staff       (20)       83 2022-11-02 18:01:41.000000 lyteidl-0.2.0a0/gen/pb_python/flyteidl/admin/event_pb2_grpc.py
--rw-r--r--   0 maximsmol   (501) staff       (20)    64117 2022-11-02 18:01:41.000000 lyteidl-0.2.0a0/gen/pb_python/flyteidl/admin/execution_pb2.py
--rw-r--r--   0 maximsmol   (501) staff       (20)       83 2022-11-02 18:01:41.000000 lyteidl-0.2.0a0/gen/pb_python/flyteidl/admin/execution_pb2_grpc.py
--rw-r--r--   0 maximsmol   (501) staff       (20)    33985 2022-11-02 18:01:41.000000 lyteidl-0.2.0a0/gen/pb_python/flyteidl/admin/launch_plan_pb2.py
--rw-r--r--   0 maximsmol   (501) staff       (20)       83 2022-11-02 18:01:41.000000 lyteidl-0.2.0a0/gen/pb_python/flyteidl/admin/launch_plan_pb2_grpc.py
--rw-r--r--   0 maximsmol   (501) staff       (20)    38570 2022-11-02 18:01:41.000000 lyteidl-0.2.0a0/gen/pb_python/flyteidl/admin/matchable_resource_pb2.py
--rw-r--r--   0 maximsmol   (501) staff       (20)       83 2022-11-02 18:01:41.000000 lyteidl-0.2.0a0/gen/pb_python/flyteidl/admin/matchable_resource_pb2_grpc.py
--rw-r--r--   0 maximsmol   (501) staff       (20)    38120 2022-11-02 18:01:41.000000 lyteidl-0.2.0a0/gen/pb_python/flyteidl/admin/node_execution_pb2.py
--rw-r--r--   0 maximsmol   (501) staff       (20)       83 2022-11-02 18:01:41.000000 lyteidl-0.2.0a0/gen/pb_python/flyteidl/admin/node_execution_pb2_grpc.py
--rw-r--r--   0 maximsmol   (501) staff       (20)     3504 2022-11-02 18:01:41.000000 lyteidl-0.2.0a0/gen/pb_python/flyteidl/admin/notification_pb2.py
--rw-r--r--   0 maximsmol   (501) staff       (20)       83 2022-11-02 18:01:41.000000 lyteidl-0.2.0a0/gen/pb_python/flyteidl/admin/notification_pb2_grpc.py
--rw-r--r--   0 maximsmol   (501) staff       (20)    14189 2022-11-02 18:01:41.000000 lyteidl-0.2.0a0/gen/pb_python/flyteidl/admin/project_domain_attributes_pb2.py
--rw-r--r--   0 maximsmol   (501) staff       (20)       83 2022-11-02 18:01:41.000000 lyteidl-0.2.0a0/gen/pb_python/flyteidl/admin/project_domain_attributes_pb2_grpc.py
--rw-r--r--   0 maximsmol   (501) staff       (20)    14548 2022-11-02 18:01:41.000000 lyteidl-0.2.0a0/gen/pb_python/flyteidl/admin/project_pb2.py
--rw-r--r--   0 maximsmol   (501) staff       (20)       83 2022-11-02 18:01:41.000000 lyteidl-0.2.0a0/gen/pb_python/flyteidl/admin/project_pb2_grpc.py
--rw-r--r--   0 maximsmol   (501) staff       (20)     8833 2022-11-02 18:01:41.000000 lyteidl-0.2.0a0/gen/pb_python/flyteidl/admin/schedule_pb2.py
--rw-r--r--   0 maximsmol   (501) staff       (20)       83 2022-11-02 18:01:41.000000 lyteidl-0.2.0a0/gen/pb_python/flyteidl/admin/schedule_pb2_grpc.py
--rw-r--r--   0 maximsmol   (501) staff       (20)    26169 2022-11-02 18:01:41.000000 lyteidl-0.2.0a0/gen/pb_python/flyteidl/admin/task_execution_pb2.py
--rw-r--r--   0 maximsmol   (501) staff       (20)       83 2022-11-02 18:01:41.000000 lyteidl-0.2.0a0/gen/pb_python/flyteidl/admin/task_execution_pb2_grpc.py
--rw-r--r--   0 maximsmol   (501) staff       (20)    10810 2022-11-02 18:01:41.000000 lyteidl-0.2.0a0/gen/pb_python/flyteidl/admin/task_pb2.py
--rw-r--r--   0 maximsmol   (501) staff       (20)       83 2022-11-02 18:01:41.000000 lyteidl-0.2.0a0/gen/pb_python/flyteidl/admin/task_pb2_grpc.py
--rw-r--r--   0 maximsmol   (501) staff       (20)     5205 2022-11-02 18:01:41.000000 lyteidl-0.2.0a0/gen/pb_python/flyteidl/admin/version_pb2.py
--rw-r--r--   0 maximsmol   (501) staff       (20)       83 2022-11-02 18:01:41.000000 lyteidl-0.2.0a0/gen/pb_python/flyteidl/admin/version_pb2_grpc.py
--rw-r--r--   0 maximsmol   (501) staff       (20)    14997 2022-11-02 18:01:41.000000 lyteidl-0.2.0a0/gen/pb_python/flyteidl/admin/workflow_attributes_pb2.py
--rw-r--r--   0 maximsmol   (501) staff       (20)       83 2022-11-02 18:01:41.000000 lyteidl-0.2.0a0/gen/pb_python/flyteidl/admin/workflow_attributes_pb2_grpc.py
--rw-r--r--   0 maximsmol   (501) staff       (20)    11870 2022-11-02 18:01:41.000000 lyteidl-0.2.0a0/gen/pb_python/flyteidl/admin/workflow_pb2.py
--rw-r--r--   0 maximsmol   (501) staff       (20)       83 2022-11-02 18:01:41.000000 lyteidl-0.2.0a0/gen/pb_python/flyteidl/admin/workflow_pb2_grpc.py
-drwxr-xr-x   0 maximsmol   (501) staff       (20)        0 2022-11-08 22:43:00.293959 lyteidl-0.2.0a0/gen/pb_python/flyteidl/core/
--rw-r--r--   0 maximsmol   (501) staff       (20)        0 2022-11-02 18:01:42.000000 lyteidl-0.2.0a0/gen/pb_python/flyteidl/core/__init__.py
--rw-r--r--   0 maximsmol   (501) staff       (20)     9851 2022-11-02 18:01:42.000000 lyteidl-0.2.0a0/gen/pb_python/flyteidl/core/catalog_pb2.py
--rw-r--r--   0 maximsmol   (501) staff       (20)       83 2022-11-02 18:01:42.000000 lyteidl-0.2.0a0/gen/pb_python/flyteidl/core/catalog_pb2_grpc.py
--rw-r--r--   0 maximsmol   (501) staff       (20)    14079 2022-11-02 18:01:42.000000 lyteidl-0.2.0a0/gen/pb_python/flyteidl/core/compiler_pb2.py
--rw-r--r--   0 maximsmol   (501) staff       (20)       83 2022-11-02 18:01:42.000000 lyteidl-0.2.0a0/gen/pb_python/flyteidl/core/compiler_pb2_grpc.py
--rw-r--r--   0 maximsmol   (501) staff       (20)    13157 2022-11-02 18:01:42.000000 lyteidl-0.2.0a0/gen/pb_python/flyteidl/core/condition_pb2.py
--rw-r--r--   0 maximsmol   (501) staff       (20)       83 2022-11-02 18:01:42.000000 lyteidl-0.2.0a0/gen/pb_python/flyteidl/core/condition_pb2_grpc.py
--rw-r--r--   0 maximsmol   (501) staff       (20)     4897 2022-11-02 18:01:42.000000 lyteidl-0.2.0a0/gen/pb_python/flyteidl/core/dynamic_job_pb2.py
--rw-r--r--   0 maximsmol   (501) staff       (20)       83 2022-11-02 18:01:42.000000 lyteidl-0.2.0a0/gen/pb_python/flyteidl/core/dynamic_job_pb2_grpc.py
--rw-r--r--   0 maximsmol   (501) staff       (20)     5919 2022-11-02 18:01:42.000000 lyteidl-0.2.0a0/gen/pb_python/flyteidl/core/errors_pb2.py
--rw-r--r--   0 maximsmol   (501) staff       (20)       83 2022-11-02 18:01:42.000000 lyteidl-0.2.0a0/gen/pb_python/flyteidl/core/errors_pb2_grpc.py
--rw-r--r--   0 maximsmol   (501) staff       (20)    21446 2022-11-02 18:01:42.000000 lyteidl-0.2.0a0/gen/pb_python/flyteidl/core/execution_pb2.py
--rw-r--r--   0 maximsmol   (501) staff       (20)       83 2022-11-02 18:01:42.000000 lyteidl-0.2.0a0/gen/pb_python/flyteidl/core/execution_pb2_grpc.py
--rw-r--r--   0 maximsmol   (501) staff       (20)    11920 2022-11-02 18:01:42.000000 lyteidl-0.2.0a0/gen/pb_python/flyteidl/core/identifier_pb2.py
--rw-r--r--   0 maximsmol   (501) staff       (20)       83 2022-11-02 18:01:42.000000 lyteidl-0.2.0a0/gen/pb_python/flyteidl/core/identifier_pb2_grpc.py
--rw-r--r--   0 maximsmol   (501) staff       (20)    14008 2022-11-02 18:01:42.000000 lyteidl-0.2.0a0/gen/pb_python/flyteidl/core/interface_pb2.py
--rw-r--r--   0 maximsmol   (501) staff       (20)       83 2022-11-02 18:01:42.000000 lyteidl-0.2.0a0/gen/pb_python/flyteidl/core/interface_pb2_grpc.py
--rw-r--r--   0 maximsmol   (501) staff       (20)    55013 2022-11-02 18:01:42.000000 lyteidl-0.2.0a0/gen/pb_python/flyteidl/core/literals_pb2.py
--rw-r--r--   0 maximsmol   (501) staff       (20)       83 2022-11-02 18:01:42.000000 lyteidl-0.2.0a0/gen/pb_python/flyteidl/core/literals_pb2_grpc.py
--rw-r--r--   0 maximsmol   (501) staff       (20)    14379 2022-11-02 18:01:42.000000 lyteidl-0.2.0a0/gen/pb_python/flyteidl/core/security_pb2.py
--rw-r--r--   0 maximsmol   (501) staff       (20)       83 2022-11-02 18:01:42.000000 lyteidl-0.2.0a0/gen/pb_python/flyteidl/core/security_pb2_grpc.py
--rw-r--r--   0 maximsmol   (501) staff       (20)    49400 2022-11-02 18:01:42.000000 lyteidl-0.2.0a0/gen/pb_python/flyteidl/core/tasks_pb2.py
--rw-r--r--   0 maximsmol   (501) staff       (20)       83 2022-11-02 18:01:42.000000 lyteidl-0.2.0a0/gen/pb_python/flyteidl/core/tasks_pb2_grpc.py
--rw-r--r--   0 maximsmol   (501) staff       (20)    35289 2022-11-02 18:01:42.000000 lyteidl-0.2.0a0/gen/pb_python/flyteidl/core/types_pb2.py
--rw-r--r--   0 maximsmol   (501) staff       (20)       83 2022-11-02 18:01:42.000000 lyteidl-0.2.0a0/gen/pb_python/flyteidl/core/types_pb2_grpc.py
--rw-r--r--   0 maximsmol   (501) staff       (20)     3252 2022-11-02 18:01:42.000000 lyteidl-0.2.0a0/gen/pb_python/flyteidl/core/workflow_closure_pb2.py
--rw-r--r--   0 maximsmol   (501) staff       (20)       83 2022-11-02 18:01:42.000000 lyteidl-0.2.0a0/gen/pb_python/flyteidl/core/workflow_closure_pb2_grpc.py
--rw-r--r--   0 maximsmol   (501) staff       (20)    33680 2022-11-02 18:01:42.000000 lyteidl-0.2.0a0/gen/pb_python/flyteidl/core/workflow_pb2.py
--rw-r--r--   0 maximsmol   (501) staff       (20)       83 2022-11-02 18:01:42.000000 lyteidl-0.2.0a0/gen/pb_python/flyteidl/core/workflow_pb2_grpc.py
-drwxr-xr-x   0 maximsmol   (501) staff       (20)        0 2022-11-08 22:43:00.295312 lyteidl-0.2.0a0/gen/pb_python/flyteidl/datacatalog/
--rw-r--r--   0 maximsmol   (501) staff       (20)        0 2022-11-02 18:01:44.000000 lyteidl-0.2.0a0/gen/pb_python/flyteidl/datacatalog/__init__.py
--rw-r--r--   0 maximsmol   (501) staff       (20)    78805 2022-11-02 18:01:44.000000 lyteidl-0.2.0a0/gen/pb_python/flyteidl/datacatalog/datacatalog_pb2.py
--rw-r--r--   0 maximsmol   (501) staff       (20)    10638 2022-11-02 18:01:44.000000 lyteidl-0.2.0a0/gen/pb_python/flyteidl/datacatalog/datacatalog_pb2_grpc.py
-drwxr-xr-x   0 maximsmol   (501) staff       (20)        0 2022-11-08 22:43:00.296863 lyteidl-0.2.0a0/gen/pb_python/flyteidl/event/
--rw-r--r--   0 maximsmol   (501) staff       (20)        0 2022-11-02 18:01:43.000000 lyteidl-0.2.0a0/gen/pb_python/flyteidl/event/__init__.py
--rw-r--r--   0 maximsmol   (501) staff       (20)    49498 2022-11-02 18:01:43.000000 lyteidl-0.2.0a0/gen/pb_python/flyteidl/event/event_pb2.py
--rw-r--r--   0 maximsmol   (501) staff       (20)       83 2022-11-02 18:01:43.000000 lyteidl-0.2.0a0/gen/pb_python/flyteidl/event/event_pb2_grpc.py
-drwxr-xr-x   0 maximsmol   (501) staff       (20)        0 2022-11-08 22:43:00.305642 lyteidl-0.2.0a0/gen/pb_python/flyteidl/plugins/
--rw-r--r--   0 maximsmol   (501) staff       (20)        0 2022-11-02 18:01:44.000000 lyteidl-0.2.0a0/gen/pb_python/flyteidl/plugins/__init__.py
--rw-r--r--   0 maximsmol   (501) staff       (20)     4048 2022-11-02 18:01:44.000000 lyteidl-0.2.0a0/gen/pb_python/flyteidl/plugins/array_job_pb2.py
--rw-r--r--   0 maximsmol   (501) staff       (20)       83 2022-11-02 18:01:44.000000 lyteidl-0.2.0a0/gen/pb_python/flyteidl/plugins/array_job_pb2_grpc.py
--rw-r--r--   0 maximsmol   (501) staff       (20)     3236 2022-11-02 18:01:44.000000 lyteidl-0.2.0a0/gen/pb_python/flyteidl/plugins/mpi_pb2.py
--rw-r--r--   0 maximsmol   (501) staff       (20)       83 2022-11-02 18:01:44.000000 lyteidl-0.2.0a0/gen/pb_python/flyteidl/plugins/mpi_pb2_grpc.py
--rw-r--r--   0 maximsmol   (501) staff       (20)     3488 2022-11-02 18:01:44.000000 lyteidl-0.2.0a0/gen/pb_python/flyteidl/plugins/presto_pb2.py
--rw-r--r--   0 maximsmol   (501) staff       (20)       83 2022-11-02 18:01:44.000000 lyteidl-0.2.0a0/gen/pb_python/flyteidl/plugins/presto_pb2_grpc.py
--rw-r--r--   0 maximsmol   (501) staff       (20)     2412 2022-11-02 18:01:44.000000 lyteidl-0.2.0a0/gen/pb_python/flyteidl/plugins/pytorch_pb2.py
--rw-r--r--   0 maximsmol   (501) staff       (20)       83 2022-11-02 18:01:44.000000 lyteidl-0.2.0a0/gen/pb_python/flyteidl/plugins/pytorch_pb2_grpc.py
--rw-r--r--   0 maximsmol   (501) staff       (20)     7152 2022-11-02 18:01:44.000000 lyteidl-0.2.0a0/gen/pb_python/flyteidl/plugins/qubole_pb2.py
--rw-r--r--   0 maximsmol   (501) staff       (20)       83 2022-11-02 18:01:44.000000 lyteidl-0.2.0a0/gen/pb_python/flyteidl/plugins/qubole_pb2_grpc.py
-drwxr-xr-x   0 maximsmol   (501) staff       (20)        0 2022-11-08 22:43:00.308653 lyteidl-0.2.0a0/gen/pb_python/flyteidl/plugins/sagemaker/
--rw-r--r--   0 maximsmol   (501) staff       (20)        0 2022-11-02 18:01:44.000000 lyteidl-0.2.0a0/gen/pb_python/flyteidl/plugins/sagemaker/__init__.py
--rw-r--r--   0 maximsmol   (501) staff       (20)    15567 2022-11-02 18:01:44.000000 lyteidl-0.2.0a0/gen/pb_python/flyteidl/plugins/sagemaker/hyperparameter_tuning_job_pb2.py
--rw-r--r--   0 maximsmol   (501) staff       (20)       83 2022-11-02 18:01:44.000000 lyteidl-0.2.0a0/gen/pb_python/flyteidl/plugins/sagemaker/hyperparameter_tuning_job_pb2_grpc.py
--rw-r--r--   0 maximsmol   (501) staff       (20)    17038 2022-11-02 18:01:44.000000 lyteidl-0.2.0a0/gen/pb_python/flyteidl/plugins/sagemaker/parameter_ranges_pb2.py
--rw-r--r--   0 maximsmol   (501) staff       (20)       83 2022-11-02 18:01:44.000000 lyteidl-0.2.0a0/gen/pb_python/flyteidl/plugins/sagemaker/parameter_ranges_pb2_grpc.py
--rw-r--r--   0 maximsmol   (501) staff       (20)    17985 2022-11-02 18:01:44.000000 lyteidl-0.2.0a0/gen/pb_python/flyteidl/plugins/sagemaker/training_job_pb2.py
--rw-r--r--   0 maximsmol   (501) staff       (20)       83 2022-11-02 18:01:44.000000 lyteidl-0.2.0a0/gen/pb_python/flyteidl/plugins/sagemaker/training_job_pb2_grpc.py
--rw-r--r--   0 maximsmol   (501) staff       (20)     7719 2022-11-02 18:01:44.000000 lyteidl-0.2.0a0/gen/pb_python/flyteidl/plugins/sidecar_pb2.py
--rw-r--r--   0 maximsmol   (501) staff       (20)       83 2022-11-02 18:01:44.000000 lyteidl-0.2.0a0/gen/pb_python/flyteidl/plugins/sidecar_pb2_grpc.py
--rw-r--r--   0 maximsmol   (501) staff       (20)    10115 2022-11-02 18:01:44.000000 lyteidl-0.2.0a0/gen/pb_python/flyteidl/plugins/spark_pb2.py
--rw-r--r--   0 maximsmol   (501) staff       (20)       83 2022-11-02 18:01:44.000000 lyteidl-0.2.0a0/gen/pb_python/flyteidl/plugins/spark_pb2_grpc.py
--rw-r--r--   0 maximsmol   (501) staff       (20)     3340 2022-11-02 18:01:44.000000 lyteidl-0.2.0a0/gen/pb_python/flyteidl/plugins/tensorflow_pb2.py
--rw-r--r--   0 maximsmol   (501) staff       (20)       83 2022-11-02 18:01:44.000000 lyteidl-0.2.0a0/gen/pb_python/flyteidl/plugins/tensorflow_pb2_grpc.py
--rw-r--r--   0 maximsmol   (501) staff       (20)     3672 2022-11-02 18:01:44.000000 lyteidl-0.2.0a0/gen/pb_python/flyteidl/plugins/waitable_pb2.py
--rw-r--r--   0 maximsmol   (501) staff       (20)       83 2022-11-02 18:01:44.000000 lyteidl-0.2.0a0/gen/pb_python/flyteidl/plugins/waitable_pb2_grpc.py
-drwxr-xr-x   0 maximsmol   (501) staff       (20)        0 2022-11-08 22:43:00.312532 lyteidl-0.2.0a0/gen/pb_python/flyteidl/service/
--rw-r--r--   0 maximsmol   (501) staff       (20)        0 2022-11-02 18:01:40.000000 lyteidl-0.2.0a0/gen/pb_python/flyteidl/service/__init__.py
--rw-r--r--   0 maximsmol   (501) staff       (20)    47502 2022-11-02 18:01:40.000000 lyteidl-0.2.0a0/gen/pb_python/flyteidl/service/admin_pb2.py
--rw-r--r--   0 maximsmol   (501) staff       (20)    48007 2022-11-02 18:01:40.000000 lyteidl-0.2.0a0/gen/pb_python/flyteidl/service/admin_pb2_grpc.py
--rw-r--r--   0 maximsmol   (501) staff       (20)    13531 2022-11-02 18:01:40.000000 lyteidl-0.2.0a0/gen/pb_python/flyteidl/service/auth_pb2.py
--rw-r--r--   0 maximsmol   (501) staff       (20)     3215 2022-11-02 18:01:40.000000 lyteidl-0.2.0a0/gen/pb_python/flyteidl/service/auth_pb2_grpc.py
--rw-r--r--   0 maximsmol   (501) staff       (20)     8674 2022-11-02 18:01:40.000000 lyteidl-0.2.0a0/gen/pb_python/flyteidl/service/dataproxy_pb2.py
--rw-r--r--   0 maximsmol   (501) staff       (20)     1857 2022-11-02 18:01:40.000000 lyteidl-0.2.0a0/gen/pb_python/flyteidl/service/dataproxy_pb2_grpc.py
--rw-r--r--   0 maximsmol   (501) staff       (20)     7042 2022-11-02 18:01:40.000000 lyteidl-0.2.0a0/gen/pb_python/flyteidl/service/identity_pb2.py
--rw-r--r--   0 maximsmol   (501) staff       (20)     1676 2022-11-02 18:01:40.000000 lyteidl-0.2.0a0/gen/pb_python/flyteidl/service/identity_pb2_grpc.py
-drwxr-xr-x   0 maximsmol   (501) staff       (20)        0 2022-11-08 22:43:00.314481 lyteidl-0.2.0a0/gen/pb_python/lyteidl.egg-info/
--rw-r--r--   0 maximsmol   (501) staff       (20)      235 2022-11-08 22:43:00.000000 lyteidl-0.2.0a0/gen/pb_python/lyteidl.egg-info/PKG-INFO
--rw-r--r--   0 maximsmol   (501) staff       (20)     5504 2022-11-08 22:43:00.000000 lyteidl-0.2.0a0/gen/pb_python/lyteidl.egg-info/SOURCES.txt
--rw-r--r--   0 maximsmol   (501) staff       (20)        1 2022-11-08 22:43:00.000000 lyteidl-0.2.0a0/gen/pb_python/lyteidl.egg-info/dependency_links.txt
--rw-r--r--   0 maximsmol   (501) staff       (20)      105 2022-11-08 22:43:00.000000 lyteidl-0.2.0a0/gen/pb_python/lyteidl.egg-info/requires.txt
--rw-r--r--   0 maximsmol   (501) staff       (20)       18 2022-11-08 22:43:00.000000 lyteidl-0.2.0a0/gen/pb_python/lyteidl.egg-info/top_level.txt
-drwxr-xr-x   0 maximsmol   (501) staff       (20)        0 2022-11-08 22:43:00.315186 lyteidl-0.2.0a0/gen/pb_python/validate/
--rw-r--r--   0 maximsmol   (501) staff       (20)        0 2022-11-02 18:02:18.000000 lyteidl-0.2.0a0/gen/pb_python/validate/__init__.py
--rw-r--r--   0 maximsmol   (501) staff       (20)   110884 2022-11-02 18:02:18.000000 lyteidl-0.2.0a0/gen/pb_python/validate/validate_pb2.py
--rw-r--r--   0 maximsmol   (501) staff       (20)      848 2022-11-08 22:43:00.316871 lyteidl-0.2.0a0/setup.cfg
--rw-r--r--   0 maximsmol   (501) staff       (20)     1431 2022-05-21 22:15:42.000000 lyteidl-0.2.0a0/setup.py
+drwxr-xr-x   0 maximsmol   (501) staff       (20)        0 2023-07-13 19:32:11.890335 lyteidl-0.2.1/
+-rw-r--r--   0 maximsmol   (501) staff       (20)    11341 2022-05-21 19:31:58.000000 lyteidl-0.2.1/LICENSE
+-rw-r--r--   0 maximsmol   (501) staff       (20)       89 2022-05-21 19:31:58.000000 lyteidl-0.2.1/NOTICE
+-rw-r--r--   0 maximsmol   (501) staff       (20)      233 2023-07-13 19:32:11.890448 lyteidl-0.2.1/PKG-INFO
+-rw-r--r--   0 maximsmol   (501) staff       (20)     2742 2022-05-21 19:31:58.000000 lyteidl-0.2.1/README.md
+drwxr-xr-x   0 maximsmol   (501) staff       (20)        0 2023-07-13 19:32:11.817689 lyteidl-0.2.1/gen/
+drwxr-xr-x   0 maximsmol   (501) staff       (20)        0 2023-07-13 19:32:11.819201 lyteidl-0.2.1/gen/pb_python/
+drwxr-xr-x   0 maximsmol   (501) staff       (20)        0 2023-07-13 19:32:11.820850 lyteidl-0.2.1/gen/pb_python/flyteidl/
+-rw-r--r--   0 maximsmol   (501) staff       (20)        0 2023-07-13 19:03:14.000000 lyteidl-0.2.1/gen/pb_python/flyteidl/__init__.py
+drwxr-xr-x   0 maximsmol   (501) staff       (20)        0 2023-07-13 19:32:11.834963 lyteidl-0.2.1/gen/pb_python/flyteidl/admin/
+-rw-r--r--   0 maximsmol   (501) staff       (20)        0 2023-07-13 19:03:15.000000 lyteidl-0.2.1/gen/pb_python/flyteidl/admin/__init__.py
+-rw-r--r--   0 maximsmol   (501) staff       (20)     8661 2023-07-13 19:03:15.000000 lyteidl-0.2.1/gen/pb_python/flyteidl/admin/cluster_assignment_pb2.py
+-rw-r--r--   0 maximsmol   (501) staff       (20)     2048 2023-07-13 19:23:00.000000 lyteidl-0.2.1/gen/pb_python/flyteidl/admin/cluster_assignment_pb2.pyi
+-rw-r--r--   0 maximsmol   (501) staff       (20)       83 2023-07-13 19:03:15.000000 lyteidl-0.2.1/gen/pb_python/flyteidl/admin/cluster_assignment_pb2_grpc.py
+-rw-r--r--   0 maximsmol   (501) staff       (20)    50730 2023-07-13 19:03:15.000000 lyteidl-0.2.1/gen/pb_python/flyteidl/admin/common_pb2.py
+-rw-r--r--   0 maximsmol   (501) staff       (20)    10476 2023-07-13 19:23:00.000000 lyteidl-0.2.1/gen/pb_python/flyteidl/admin/common_pb2.pyi
+-rw-r--r--   0 maximsmol   (501) staff       (20)       83 2023-07-13 19:03:15.000000 lyteidl-0.2.1/gen/pb_python/flyteidl/admin/common_pb2_grpc.py
+-rw-r--r--   0 maximsmol   (501) staff       (20)    15485 2023-07-13 19:03:15.000000 lyteidl-0.2.1/gen/pb_python/flyteidl/admin/event_pb2.py
+-rw-r--r--   0 maximsmol   (501) staff       (20)     2785 2023-07-13 19:23:00.000000 lyteidl-0.2.1/gen/pb_python/flyteidl/admin/event_pb2.pyi
+-rw-r--r--   0 maximsmol   (501) staff       (20)       83 2023-07-13 19:03:15.000000 lyteidl-0.2.1/gen/pb_python/flyteidl/admin/event_pb2_grpc.py
+-rw-r--r--   0 maximsmol   (501) staff       (20)    64117 2023-07-13 19:03:15.000000 lyteidl-0.2.1/gen/pb_python/flyteidl/admin/execution_pb2.py
+-rw-r--r--   0 maximsmol   (501) staff       (20)    14674 2023-07-13 19:23:00.000000 lyteidl-0.2.1/gen/pb_python/flyteidl/admin/execution_pb2.pyi
+-rw-r--r--   0 maximsmol   (501) staff       (20)       83 2023-07-13 19:03:15.000000 lyteidl-0.2.1/gen/pb_python/flyteidl/admin/execution_pb2_grpc.py
+-rw-r--r--   0 maximsmol   (501) staff       (20)    33985 2023-07-13 19:03:15.000000 lyteidl-0.2.1/gen/pb_python/flyteidl/admin/launch_plan_pb2.py
+-rw-r--r--   0 maximsmol   (501) staff       (20)     8168 2023-07-13 19:23:00.000000 lyteidl-0.2.1/gen/pb_python/flyteidl/admin/launch_plan_pb2.pyi
+-rw-r--r--   0 maximsmol   (501) staff       (20)       83 2023-07-13 19:03:15.000000 lyteidl-0.2.1/gen/pb_python/flyteidl/admin/launch_plan_pb2_grpc.py
+-rw-r--r--   0 maximsmol   (501) staff       (20)    38570 2023-07-13 19:03:15.000000 lyteidl-0.2.1/gen/pb_python/flyteidl/admin/matchable_resource_pb2.py
+-rw-r--r--   0 maximsmol   (501) staff       (20)     8612 2023-07-13 19:23:00.000000 lyteidl-0.2.1/gen/pb_python/flyteidl/admin/matchable_resource_pb2.pyi
+-rw-r--r--   0 maximsmol   (501) staff       (20)       83 2023-07-13 19:03:15.000000 lyteidl-0.2.1/gen/pb_python/flyteidl/admin/matchable_resource_pb2_grpc.py
+-rw-r--r--   0 maximsmol   (501) staff       (20)    38120 2023-07-13 19:03:15.000000 lyteidl-0.2.1/gen/pb_python/flyteidl/admin/node_execution_pb2.py
+-rw-r--r--   0 maximsmol   (501) staff       (20)     8696 2023-07-13 19:23:00.000000 lyteidl-0.2.1/gen/pb_python/flyteidl/admin/node_execution_pb2.pyi
+-rw-r--r--   0 maximsmol   (501) staff       (20)       83 2023-07-13 19:03:15.000000 lyteidl-0.2.1/gen/pb_python/flyteidl/admin/node_execution_pb2_grpc.py
+-rw-r--r--   0 maximsmol   (501) staff       (20)     3504 2023-07-13 19:03:15.000000 lyteidl-0.2.1/gen/pb_python/flyteidl/admin/notification_pb2.py
+-rw-r--r--   0 maximsmol   (501) staff       (20)      901 2023-07-13 19:23:00.000000 lyteidl-0.2.1/gen/pb_python/flyteidl/admin/notification_pb2.pyi
+-rw-r--r--   0 maximsmol   (501) staff       (20)       83 2023-07-13 19:03:15.000000 lyteidl-0.2.1/gen/pb_python/flyteidl/admin/notification_pb2_grpc.py
+-rw-r--r--   0 maximsmol   (501) staff       (20)    14189 2023-07-13 19:03:15.000000 lyteidl-0.2.1/gen/pb_python/flyteidl/admin/project_domain_attributes_pb2.py
+-rw-r--r--   0 maximsmol   (501) staff       (20)     2719 2023-07-13 19:23:00.000000 lyteidl-0.2.1/gen/pb_python/flyteidl/admin/project_domain_attributes_pb2.pyi
+-rw-r--r--   0 maximsmol   (501) staff       (20)       83 2023-07-13 19:03:15.000000 lyteidl-0.2.1/gen/pb_python/flyteidl/admin/project_domain_attributes_pb2_grpc.py
+-rw-r--r--   0 maximsmol   (501) staff       (20)    14548 2023-07-13 19:03:15.000000 lyteidl-0.2.1/gen/pb_python/flyteidl/admin/project_pb2.py
+-rw-r--r--   0 maximsmol   (501) staff       (20)     3085 2023-07-13 19:23:00.000000 lyteidl-0.2.1/gen/pb_python/flyteidl/admin/project_pb2.pyi
+-rw-r--r--   0 maximsmol   (501) staff       (20)       83 2023-07-13 19:03:15.000000 lyteidl-0.2.1/gen/pb_python/flyteidl/admin/project_pb2_grpc.py
+-rw-r--r--   0 maximsmol   (501) staff       (20)     8833 2023-07-13 19:03:15.000000 lyteidl-0.2.1/gen/pb_python/flyteidl/admin/schedule_pb2.py
+-rw-r--r--   0 maximsmol   (501) staff       (20)     1726 2023-07-13 19:23:00.000000 lyteidl-0.2.1/gen/pb_python/flyteidl/admin/schedule_pb2.pyi
+-rw-r--r--   0 maximsmol   (501) staff       (20)       83 2023-07-13 19:03:15.000000 lyteidl-0.2.1/gen/pb_python/flyteidl/admin/schedule_pb2_grpc.py
+-rw-r--r--   0 maximsmol   (501) staff       (20)    26169 2023-07-13 19:03:15.000000 lyteidl-0.2.1/gen/pb_python/flyteidl/admin/task_execution_pb2.py
+-rw-r--r--   0 maximsmol   (501) staff       (20)     6154 2023-07-13 19:23:00.000000 lyteidl-0.2.1/gen/pb_python/flyteidl/admin/task_execution_pb2.pyi
+-rw-r--r--   0 maximsmol   (501) staff       (20)       83 2023-07-13 19:03:15.000000 lyteidl-0.2.1/gen/pb_python/flyteidl/admin/task_execution_pb2_grpc.py
+-rw-r--r--   0 maximsmol   (501) staff       (20)    10810 2023-07-13 19:03:15.000000 lyteidl-0.2.1/gen/pb_python/flyteidl/admin/task_pb2.py
+-rw-r--r--   0 maximsmol   (501) staff       (20)     2424 2023-07-13 19:23:00.000000 lyteidl-0.2.1/gen/pb_python/flyteidl/admin/task_pb2.pyi
+-rw-r--r--   0 maximsmol   (501) staff       (20)       83 2023-07-13 19:03:15.000000 lyteidl-0.2.1/gen/pb_python/flyteidl/admin/task_pb2_grpc.py
+-rw-r--r--   0 maximsmol   (501) staff       (20)     5205 2023-07-13 19:03:15.000000 lyteidl-0.2.1/gen/pb_python/flyteidl/admin/version_pb2.py
+-rw-r--r--   0 maximsmol   (501) staff       (20)     1010 2023-07-13 19:23:00.000000 lyteidl-0.2.1/gen/pb_python/flyteidl/admin/version_pb2.pyi
+-rw-r--r--   0 maximsmol   (501) staff       (20)       83 2023-07-13 19:03:15.000000 lyteidl-0.2.1/gen/pb_python/flyteidl/admin/version_pb2_grpc.py
+-rw-r--r--   0 maximsmol   (501) staff       (20)    14997 2023-07-13 19:03:15.000000 lyteidl-0.2.1/gen/pb_python/flyteidl/admin/workflow_attributes_pb2.py
+-rw-r--r--   0 maximsmol   (501) staff       (20)     2976 2023-07-13 19:23:00.000000 lyteidl-0.2.1/gen/pb_python/flyteidl/admin/workflow_attributes_pb2.pyi
+-rw-r--r--   0 maximsmol   (501) staff       (20)       83 2023-07-13 19:03:15.000000 lyteidl-0.2.1/gen/pb_python/flyteidl/admin/workflow_attributes_pb2_grpc.py
+-rw-r--r--   0 maximsmol   (501) staff       (20)    11870 2023-07-13 19:03:15.000000 lyteidl-0.2.1/gen/pb_python/flyteidl/admin/workflow_pb2.py
+-rw-r--r--   0 maximsmol   (501) staff       (20)     2798 2023-07-13 19:23:00.000000 lyteidl-0.2.1/gen/pb_python/flyteidl/admin/workflow_pb2.pyi
+-rw-r--r--   0 maximsmol   (501) staff       (20)       83 2023-07-13 19:03:15.000000 lyteidl-0.2.1/gen/pb_python/flyteidl/admin/workflow_pb2_grpc.py
+drwxr-xr-x   0 maximsmol   (501) staff       (20)        0 2023-07-13 19:32:11.873903 lyteidl-0.2.1/gen/pb_python/flyteidl/core/
+-rw-r--r--   0 maximsmol   (501) staff       (20)        0 2023-07-13 19:03:16.000000 lyteidl-0.2.1/gen/pb_python/flyteidl/core/__init__.py
+-rw-r--r--   0 maximsmol   (501) staff       (20)     9851 2023-07-13 19:03:16.000000 lyteidl-0.2.1/gen/pb_python/flyteidl/core/catalog_pb2.py
+-rw-r--r--   0 maximsmol   (501) staff       (20)     2125 2023-07-13 19:23:00.000000 lyteidl-0.2.1/gen/pb_python/flyteidl/core/catalog_pb2.pyi
+-rw-r--r--   0 maximsmol   (501) staff       (20)       83 2023-07-13 19:03:16.000000 lyteidl-0.2.1/gen/pb_python/flyteidl/core/catalog_pb2_grpc.py
+-rw-r--r--   0 maximsmol   (501) staff       (20)    14079 2023-07-13 19:03:16.000000 lyteidl-0.2.1/gen/pb_python/flyteidl/core/compiler_pb2.py
+-rw-r--r--   0 maximsmol   (501) staff       (20)     3176 2023-07-13 19:23:00.000000 lyteidl-0.2.1/gen/pb_python/flyteidl/core/compiler_pb2.pyi
+-rw-r--r--   0 maximsmol   (501) staff       (20)       83 2023-07-13 19:03:16.000000 lyteidl-0.2.1/gen/pb_python/flyteidl/core/compiler_pb2_grpc.py
+-rw-r--r--   0 maximsmol   (501) staff       (20)    13157 2023-07-13 19:03:16.000000 lyteidl-0.2.1/gen/pb_python/flyteidl/core/condition_pb2.py
+-rw-r--r--   0 maximsmol   (501) staff       (20)     2859 2023-07-13 19:23:00.000000 lyteidl-0.2.1/gen/pb_python/flyteidl/core/condition_pb2.pyi
+-rw-r--r--   0 maximsmol   (501) staff       (20)       83 2023-07-13 19:03:16.000000 lyteidl-0.2.1/gen/pb_python/flyteidl/core/condition_pb2_grpc.py
+-rw-r--r--   0 maximsmol   (501) staff       (20)     4897 2023-07-13 19:03:16.000000 lyteidl-0.2.1/gen/pb_python/flyteidl/core/dynamic_job_pb2.py
+-rw-r--r--   0 maximsmol   (501) staff       (20)     1570 2023-07-13 19:23:00.000000 lyteidl-0.2.1/gen/pb_python/flyteidl/core/dynamic_job_pb2.pyi
+-rw-r--r--   0 maximsmol   (501) staff       (20)       83 2023-07-13 19:03:16.000000 lyteidl-0.2.1/gen/pb_python/flyteidl/core/dynamic_job_pb2_grpc.py
+-rw-r--r--   0 maximsmol   (501) staff       (20)     5919 2023-07-13 19:03:16.000000 lyteidl-0.2.1/gen/pb_python/flyteidl/core/errors_pb2.py
+-rw-r--r--   0 maximsmol   (501) staff       (20)     1368 2023-07-13 19:23:00.000000 lyteidl-0.2.1/gen/pb_python/flyteidl/core/errors_pb2.pyi
+-rw-r--r--   0 maximsmol   (501) staff       (20)       83 2023-07-13 19:03:16.000000 lyteidl-0.2.1/gen/pb_python/flyteidl/core/errors_pb2_grpc.py
+-rw-r--r--   0 maximsmol   (501) staff       (20)    21446 2023-07-13 19:03:16.000000 lyteidl-0.2.1/gen/pb_python/flyteidl/core/execution_pb2.py
+-rw-r--r--   0 maximsmol   (501) staff       (20)     4377 2023-07-13 19:23:00.000000 lyteidl-0.2.1/gen/pb_python/flyteidl/core/execution_pb2.pyi
+-rw-r--r--   0 maximsmol   (501) staff       (20)       83 2023-07-13 19:03:16.000000 lyteidl-0.2.1/gen/pb_python/flyteidl/core/execution_pb2_grpc.py
+-rw-r--r--   0 maximsmol   (501) staff       (20)    11920 2023-07-13 19:03:16.000000 lyteidl-0.2.1/gen/pb_python/flyteidl/core/identifier_pb2.py
+-rw-r--r--   0 maximsmol   (501) staff       (20)     2494 2023-07-13 19:23:00.000000 lyteidl-0.2.1/gen/pb_python/flyteidl/core/identifier_pb2.pyi
+-rw-r--r--   0 maximsmol   (501) staff       (20)       83 2023-07-13 19:03:16.000000 lyteidl-0.2.1/gen/pb_python/flyteidl/core/identifier_pb2_grpc.py
+-rw-r--r--   0 maximsmol   (501) staff       (20)    14008 2023-07-13 19:03:16.000000 lyteidl-0.2.1/gen/pb_python/flyteidl/core/interface_pb2.py
+-rw-r--r--   0 maximsmol   (501) staff       (20)     2735 2023-07-13 19:23:00.000000 lyteidl-0.2.1/gen/pb_python/flyteidl/core/interface_pb2.pyi
+-rw-r--r--   0 maximsmol   (501) staff       (20)       83 2023-07-13 19:03:16.000000 lyteidl-0.2.1/gen/pb_python/flyteidl/core/interface_pb2_grpc.py
+-rw-r--r--   0 maximsmol   (501) staff       (20)    55013 2023-07-13 19:03:16.000000 lyteidl-0.2.1/gen/pb_python/flyteidl/core/literals_pb2.py
+-rw-r--r--   0 maximsmol   (501) staff       (20)    10490 2023-07-13 19:23:00.000000 lyteidl-0.2.1/gen/pb_python/flyteidl/core/literals_pb2.pyi
+-rw-r--r--   0 maximsmol   (501) staff       (20)       83 2023-07-13 19:03:16.000000 lyteidl-0.2.1/gen/pb_python/flyteidl/core/literals_pb2_grpc.py
+-rw-r--r--   0 maximsmol   (501) staff       (20)    14379 2023-07-13 19:03:16.000000 lyteidl-0.2.1/gen/pb_python/flyteidl/core/security_pb2.py
+-rw-r--r--   0 maximsmol   (501) staff       (20)     3482 2023-07-13 19:23:00.000000 lyteidl-0.2.1/gen/pb_python/flyteidl/core/security_pb2.pyi
+-rw-r--r--   0 maximsmol   (501) staff       (20)       83 2023-07-13 19:03:16.000000 lyteidl-0.2.1/gen/pb_python/flyteidl/core/security_pb2_grpc.py
+-rw-r--r--   0 maximsmol   (501) staff       (20)    49400 2023-07-13 19:03:16.000000 lyteidl-0.2.1/gen/pb_python/flyteidl/core/tasks_pb2.py
+-rw-r--r--   0 maximsmol   (501) staff       (20)    11489 2023-07-13 19:23:00.000000 lyteidl-0.2.1/gen/pb_python/flyteidl/core/tasks_pb2.pyi
+-rw-r--r--   0 maximsmol   (501) staff       (20)       83 2023-07-13 19:03:16.000000 lyteidl-0.2.1/gen/pb_python/flyteidl/core/tasks_pb2_grpc.py
+-rw-r--r--   0 maximsmol   (501) staff       (20)    35289 2023-07-13 19:03:16.000000 lyteidl-0.2.1/gen/pb_python/flyteidl/core/types_pb2.py
+-rw-r--r--   0 maximsmol   (501) staff       (20)     7566 2023-07-13 19:23:00.000000 lyteidl-0.2.1/gen/pb_python/flyteidl/core/types_pb2.pyi
+-rw-r--r--   0 maximsmol   (501) staff       (20)       83 2023-07-13 19:03:16.000000 lyteidl-0.2.1/gen/pb_python/flyteidl/core/types_pb2_grpc.py
+-rw-r--r--   0 maximsmol   (501) staff       (20)     3252 2023-07-13 19:03:16.000000 lyteidl-0.2.1/gen/pb_python/flyteidl/core/workflow_closure_pb2.py
+-rw-r--r--   0 maximsmol   (501) staff       (20)      913 2023-07-13 19:23:00.000000 lyteidl-0.2.1/gen/pb_python/flyteidl/core/workflow_closure_pb2.pyi
+-rw-r--r--   0 maximsmol   (501) staff       (20)       83 2023-07-13 19:03:16.000000 lyteidl-0.2.1/gen/pb_python/flyteidl/core/workflow_closure_pb2_grpc.py
+-rw-r--r--   0 maximsmol   (501) staff       (20)    33680 2023-07-13 19:03:16.000000 lyteidl-0.2.1/gen/pb_python/flyteidl/core/workflow_pb2.py
+-rw-r--r--   0 maximsmol   (501) staff       (20)     7806 2023-07-13 19:23:00.000000 lyteidl-0.2.1/gen/pb_python/flyteidl/core/workflow_pb2.pyi
+-rw-r--r--   0 maximsmol   (501) staff       (20)       83 2023-07-13 19:03:16.000000 lyteidl-0.2.1/gen/pb_python/flyteidl/core/workflow_pb2_grpc.py
+drwxr-xr-x   0 maximsmol   (501) staff       (20)        0 2023-07-13 19:32:11.875044 lyteidl-0.2.1/gen/pb_python/flyteidl/datacatalog/
+-rw-r--r--   0 maximsmol   (501) staff       (20)        0 2023-07-13 19:03:18.000000 lyteidl-0.2.1/gen/pb_python/flyteidl/datacatalog/__init__.py
+-rw-r--r--   0 maximsmol   (501) staff       (20)    78805 2023-07-13 19:03:18.000000 lyteidl-0.2.1/gen/pb_python/flyteidl/datacatalog/datacatalog_pb2.py
+-rw-r--r--   0 maximsmol   (501) staff       (20)    14647 2023-07-13 19:23:00.000000 lyteidl-0.2.1/gen/pb_python/flyteidl/datacatalog/datacatalog_pb2.pyi
+-rw-r--r--   0 maximsmol   (501) staff       (20)    10638 2023-07-13 19:03:18.000000 lyteidl-0.2.1/gen/pb_python/flyteidl/datacatalog/datacatalog_pb2_grpc.py
+drwxr-xr-x   0 maximsmol   (501) staff       (20)        0 2023-07-13 19:32:11.876181 lyteidl-0.2.1/gen/pb_python/flyteidl/event/
+-rw-r--r--   0 maximsmol   (501) staff       (20)        0 2023-07-13 19:03:17.000000 lyteidl-0.2.1/gen/pb_python/flyteidl/event/__init__.py
+-rw-r--r--   0 maximsmol   (501) staff       (20)    49498 2023-07-13 19:03:17.000000 lyteidl-0.2.1/gen/pb_python/flyteidl/event/event_pb2.py
+-rw-r--r--   0 maximsmol   (501) staff       (20)    12246 2023-07-13 19:23:00.000000 lyteidl-0.2.1/gen/pb_python/flyteidl/event/event_pb2.pyi
+-rw-r--r--   0 maximsmol   (501) staff       (20)       83 2023-07-13 19:03:17.000000 lyteidl-0.2.1/gen/pb_python/flyteidl/event/event_pb2_grpc.py
+drwxr-xr-x   0 maximsmol   (501) staff       (20)        0 2023-07-13 19:32:11.883831 lyteidl-0.2.1/gen/pb_python/flyteidl/plugins/
+-rw-r--r--   0 maximsmol   (501) staff       (20)        0 2023-07-13 19:03:18.000000 lyteidl-0.2.1/gen/pb_python/flyteidl/plugins/__init__.py
+-rw-r--r--   0 maximsmol   (501) staff       (20)     4048 2023-07-13 19:03:18.000000 lyteidl-0.2.1/gen/pb_python/flyteidl/plugins/array_job_pb2.py
+-rw-r--r--   0 maximsmol   (501) staff       (20)      766 2023-07-13 19:23:00.000000 lyteidl-0.2.1/gen/pb_python/flyteidl/plugins/array_job_pb2.pyi
+-rw-r--r--   0 maximsmol   (501) staff       (20)       83 2023-07-13 19:03:18.000000 lyteidl-0.2.1/gen/pb_python/flyteidl/plugins/array_job_pb2_grpc.py
+-rw-r--r--   0 maximsmol   (501) staff       (20)     3236 2023-07-13 19:03:18.000000 lyteidl-0.2.1/gen/pb_python/flyteidl/plugins/mpi_pb2.py
+-rw-r--r--   0 maximsmol   (501) staff       (20)      676 2023-07-13 19:23:00.000000 lyteidl-0.2.1/gen/pb_python/flyteidl/plugins/mpi_pb2.pyi
+-rw-r--r--   0 maximsmol   (501) staff       (20)       83 2023-07-13 19:03:18.000000 lyteidl-0.2.1/gen/pb_python/flyteidl/plugins/mpi_pb2_grpc.py
+-rw-r--r--   0 maximsmol   (501) staff       (20)     3488 2023-07-13 19:03:18.000000 lyteidl-0.2.1/gen/pb_python/flyteidl/plugins/presto_pb2.py
+-rw-r--r--   0 maximsmol   (501) staff       (20)      725 2023-07-13 19:23:00.000000 lyteidl-0.2.1/gen/pb_python/flyteidl/plugins/presto_pb2.pyi
+-rw-r--r--   0 maximsmol   (501) staff       (20)       83 2023-07-13 19:03:18.000000 lyteidl-0.2.1/gen/pb_python/flyteidl/plugins/presto_pb2_grpc.py
+-rw-r--r--   0 maximsmol   (501) staff       (20)     2412 2023-07-13 19:03:18.000000 lyteidl-0.2.1/gen/pb_python/flyteidl/plugins/pytorch_pb2.py
+-rw-r--r--   0 maximsmol   (501) staff       (20)      416 2023-07-13 19:23:00.000000 lyteidl-0.2.1/gen/pb_python/flyteidl/plugins/pytorch_pb2.pyi
+-rw-r--r--   0 maximsmol   (501) staff       (20)       83 2023-07-13 19:03:18.000000 lyteidl-0.2.1/gen/pb_python/flyteidl/plugins/pytorch_pb2_grpc.py
+-rw-r--r--   0 maximsmol   (501) staff       (20)     7152 2023-07-13 19:03:18.000000 lyteidl-0.2.1/gen/pb_python/flyteidl/plugins/qubole_pb2.py
+-rw-r--r--   0 maximsmol   (501) staff       (20)     1690 2023-07-13 19:23:00.000000 lyteidl-0.2.1/gen/pb_python/flyteidl/plugins/qubole_pb2.pyi
+-rw-r--r--   0 maximsmol   (501) staff       (20)       83 2023-07-13 19:03:18.000000 lyteidl-0.2.1/gen/pb_python/flyteidl/plugins/qubole_pb2_grpc.py
+drwxr-xr-x   0 maximsmol   (501) staff       (20)        0 2023-07-13 19:32:11.885731 lyteidl-0.2.1/gen/pb_python/flyteidl/plugins/sagemaker/
+-rw-r--r--   0 maximsmol   (501) staff       (20)        0 2023-07-13 19:03:18.000000 lyteidl-0.2.1/gen/pb_python/flyteidl/plugins/sagemaker/__init__.py
+-rw-r--r--   0 maximsmol   (501) staff       (20)    15567 2023-07-13 19:03:18.000000 lyteidl-0.2.1/gen/pb_python/flyteidl/plugins/sagemaker/hyperparameter_tuning_job_pb2.py
+-rw-r--r--   0 maximsmol   (501) staff       (20)       83 2023-07-13 19:03:18.000000 lyteidl-0.2.1/gen/pb_python/flyteidl/plugins/sagemaker/hyperparameter_tuning_job_pb2_grpc.py
+-rw-r--r--   0 maximsmol   (501) staff       (20)    17038 2023-07-13 19:03:18.000000 lyteidl-0.2.1/gen/pb_python/flyteidl/plugins/sagemaker/parameter_ranges_pb2.py
+-rw-r--r--   0 maximsmol   (501) staff       (20)       83 2023-07-13 19:03:18.000000 lyteidl-0.2.1/gen/pb_python/flyteidl/plugins/sagemaker/parameter_ranges_pb2_grpc.py
+-rw-r--r--   0 maximsmol   (501) staff       (20)    17985 2023-07-13 19:03:18.000000 lyteidl-0.2.1/gen/pb_python/flyteidl/plugins/sagemaker/training_job_pb2.py
+-rw-r--r--   0 maximsmol   (501) staff       (20)       83 2023-07-13 19:03:18.000000 lyteidl-0.2.1/gen/pb_python/flyteidl/plugins/sagemaker/training_job_pb2_grpc.py
+-rw-r--r--   0 maximsmol   (501) staff       (20)     7719 2023-07-13 19:03:18.000000 lyteidl-0.2.1/gen/pb_python/flyteidl/plugins/sidecar_pb2.py
+-rw-r--r--   0 maximsmol   (501) staff       (20)     1671 2023-07-13 19:23:00.000000 lyteidl-0.2.1/gen/pb_python/flyteidl/plugins/sidecar_pb2.pyi
+-rw-r--r--   0 maximsmol   (501) staff       (20)       83 2023-07-13 19:03:18.000000 lyteidl-0.2.1/gen/pb_python/flyteidl/plugins/sidecar_pb2_grpc.py
+-rw-r--r--   0 maximsmol   (501) staff       (20)    10115 2023-07-13 19:03:18.000000 lyteidl-0.2.1/gen/pb_python/flyteidl/plugins/spark_pb2.py
+-rw-r--r--   0 maximsmol   (501) staff       (20)     2246 2023-07-13 19:23:00.000000 lyteidl-0.2.1/gen/pb_python/flyteidl/plugins/spark_pb2.pyi
+-rw-r--r--   0 maximsmol   (501) staff       (20)       83 2023-07-13 19:03:18.000000 lyteidl-0.2.1/gen/pb_python/flyteidl/plugins/spark_pb2_grpc.py
+-rw-r--r--   0 maximsmol   (501) staff       (20)     3340 2023-07-13 19:03:18.000000 lyteidl-0.2.1/gen/pb_python/flyteidl/plugins/tensorflow_pb2.py
+-rw-r--r--   0 maximsmol   (501) staff       (20)      663 2023-07-13 19:23:00.000000 lyteidl-0.2.1/gen/pb_python/flyteidl/plugins/tensorflow_pb2.pyi
+-rw-r--r--   0 maximsmol   (501) staff       (20)       83 2023-07-13 19:03:18.000000 lyteidl-0.2.1/gen/pb_python/flyteidl/plugins/tensorflow_pb2_grpc.py
+-rw-r--r--   0 maximsmol   (501) staff       (20)     3672 2023-07-13 19:03:18.000000 lyteidl-0.2.1/gen/pb_python/flyteidl/plugins/waitable_pb2.py
+-rw-r--r--   0 maximsmol   (501) staff       (20)      951 2023-07-13 19:23:00.000000 lyteidl-0.2.1/gen/pb_python/flyteidl/plugins/waitable_pb2.pyi
+-rw-r--r--   0 maximsmol   (501) staff       (20)       83 2023-07-13 19:03:18.000000 lyteidl-0.2.1/gen/pb_python/flyteidl/plugins/waitable_pb2_grpc.py
+drwxr-xr-x   0 maximsmol   (501) staff       (20)        0 2023-07-13 19:32:11.888205 lyteidl-0.2.1/gen/pb_python/flyteidl/service/
+-rw-r--r--   0 maximsmol   (501) staff       (20)        0 2023-07-13 19:03:14.000000 lyteidl-0.2.1/gen/pb_python/flyteidl/service/__init__.py
+-rw-r--r--   0 maximsmol   (501) staff       (20)    47502 2023-07-13 19:03:14.000000 lyteidl-0.2.1/gen/pb_python/flyteidl/service/admin_pb2.py
+-rw-r--r--   0 maximsmol   (501) staff       (20)    48007 2023-07-13 19:03:14.000000 lyteidl-0.2.1/gen/pb_python/flyteidl/service/admin_pb2_grpc.py
+-rw-r--r--   0 maximsmol   (501) staff       (20)    13531 2023-07-13 19:03:14.000000 lyteidl-0.2.1/gen/pb_python/flyteidl/service/auth_pb2.py
+-rw-r--r--   0 maximsmol   (501) staff       (20)     3215 2023-07-13 19:03:14.000000 lyteidl-0.2.1/gen/pb_python/flyteidl/service/auth_pb2_grpc.py
+-rw-r--r--   0 maximsmol   (501) staff       (20)     8674 2023-07-13 19:03:14.000000 lyteidl-0.2.1/gen/pb_python/flyteidl/service/dataproxy_pb2.py
+-rw-r--r--   0 maximsmol   (501) staff       (20)     1857 2023-07-13 19:03:14.000000 lyteidl-0.2.1/gen/pb_python/flyteidl/service/dataproxy_pb2_grpc.py
+-rw-r--r--   0 maximsmol   (501) staff       (20)     7042 2023-07-13 19:03:14.000000 lyteidl-0.2.1/gen/pb_python/flyteidl/service/identity_pb2.py
+-rw-r--r--   0 maximsmol   (501) staff       (20)     1676 2023-07-13 19:03:14.000000 lyteidl-0.2.1/gen/pb_python/flyteidl/service/identity_pb2_grpc.py
+drwxr-xr-x   0 maximsmol   (501) staff       (20)        0 2023-07-13 19:32:11.889512 lyteidl-0.2.1/gen/pb_python/lyteidl.egg-info/
+-rw-r--r--   0 maximsmol   (501) staff       (20)      233 2023-07-13 19:32:11.000000 lyteidl-0.2.1/gen/pb_python/lyteidl.egg-info/PKG-INFO
+-rw-r--r--   0 maximsmol   (501) staff       (20)     7453 2023-07-13 19:32:11.000000 lyteidl-0.2.1/gen/pb_python/lyteidl.egg-info/SOURCES.txt
+-rw-r--r--   0 maximsmol   (501) staff       (20)        1 2023-07-13 19:32:11.000000 lyteidl-0.2.1/gen/pb_python/lyteidl.egg-info/dependency_links.txt
+-rw-r--r--   0 maximsmol   (501) staff       (20)      105 2023-07-13 19:32:11.000000 lyteidl-0.2.1/gen/pb_python/lyteidl.egg-info/requires.txt
+-rw-r--r--   0 maximsmol   (501) staff       (20)       18 2023-07-13 19:32:11.000000 lyteidl-0.2.1/gen/pb_python/lyteidl.egg-info/top_level.txt
+drwxr-xr-x   0 maximsmol   (501) staff       (20)        0 2023-07-13 19:32:11.889980 lyteidl-0.2.1/gen/pb_python/validate/
+-rw-r--r--   0 maximsmol   (501) staff       (20)        0 2023-07-13 19:23:15.000000 lyteidl-0.2.1/gen/pb_python/validate/__init__.py
+-rw-r--r--   0 maximsmol   (501) staff       (20)   110884 2023-07-13 19:23:15.000000 lyteidl-0.2.1/gen/pb_python/validate/validate_pb2.py
+-rw-r--r--   0 maximsmol   (501) staff       (20)      848 2023-07-13 19:32:11.891045 lyteidl-0.2.1/setup.cfg
+-rw-r--r--   0 maximsmol   (501) staff       (20)     1550 2023-07-13 19:31:07.000000 lyteidl-0.2.1/setup.py
```

### Comparing `lyteidl-0.2.0a0/LICENSE` & `lyteidl-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lyteidl-0.2.0a0/README.md` & `lyteidl-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `lyteidl-0.2.0a0/gen/pb_python/flyteidl/admin/cluster_assignment_pb2.py` & `lyteidl-0.2.1/gen/pb_python/flyteidl/admin/cluster_assignment_pb2.py`

 * *Files identical despite different names*

### Comparing `lyteidl-0.2.0a0/gen/pb_python/flyteidl/admin/common_pb2.py` & `lyteidl-0.2.1/gen/pb_python/flyteidl/admin/common_pb2.py`

 * *Files identical despite different names*

### Comparing `lyteidl-0.2.0a0/gen/pb_python/flyteidl/admin/event_pb2.py` & `lyteidl-0.2.1/gen/pb_python/flyteidl/admin/event_pb2.py`

 * *Files identical despite different names*

### Comparing `lyteidl-0.2.0a0/gen/pb_python/flyteidl/admin/execution_pb2.py` & `lyteidl-0.2.1/gen/pb_python/flyteidl/admin/execution_pb2.py`

 * *Files identical despite different names*

### Comparing `lyteidl-0.2.0a0/gen/pb_python/flyteidl/admin/launch_plan_pb2.py` & `lyteidl-0.2.1/gen/pb_python/flyteidl/admin/launch_plan_pb2.py`

 * *Files identical despite different names*

### Comparing `lyteidl-0.2.0a0/gen/pb_python/flyteidl/admin/matchable_resource_pb2.py` & `lyteidl-0.2.1/gen/pb_python/flyteidl/admin/matchable_resource_pb2.py`

 * *Files identical despite different names*

### Comparing `lyteidl-0.2.0a0/gen/pb_python/flyteidl/admin/node_execution_pb2.py` & `lyteidl-0.2.1/gen/pb_python/flyteidl/admin/node_execution_pb2.py`

 * *Files identical despite different names*

### Comparing `lyteidl-0.2.0a0/gen/pb_python/flyteidl/admin/notification_pb2.py` & `lyteidl-0.2.1/gen/pb_python/flyteidl/admin/notification_pb2.py`

 * *Files identical despite different names*

### Comparing `lyteidl-0.2.0a0/gen/pb_python/flyteidl/admin/project_domain_attributes_pb2.py` & `lyteidl-0.2.1/gen/pb_python/flyteidl/admin/project_domain_attributes_pb2.py`

 * *Files identical despite different names*

### Comparing `lyteidl-0.2.0a0/gen/pb_python/flyteidl/admin/project_pb2.py` & `lyteidl-0.2.1/gen/pb_python/flyteidl/admin/project_pb2.py`

 * *Files identical despite different names*

### Comparing `lyteidl-0.2.0a0/gen/pb_python/flyteidl/admin/schedule_pb2.py` & `lyteidl-0.2.1/gen/pb_python/flyteidl/admin/schedule_pb2.py`

 * *Files identical despite different names*

### Comparing `lyteidl-0.2.0a0/gen/pb_python/flyteidl/admin/task_execution_pb2.py` & `lyteidl-0.2.1/gen/pb_python/flyteidl/admin/task_execution_pb2.py`

 * *Files identical despite different names*

### Comparing `lyteidl-0.2.0a0/gen/pb_python/flyteidl/admin/task_pb2.py` & `lyteidl-0.2.1/gen/pb_python/flyteidl/admin/task_pb2.py`

 * *Files identical despite different names*

### Comparing `lyteidl-0.2.0a0/gen/pb_python/flyteidl/admin/version_pb2.py` & `lyteidl-0.2.1/gen/pb_python/flyteidl/admin/version_pb2.py`

 * *Files identical despite different names*

### Comparing `lyteidl-0.2.0a0/gen/pb_python/flyteidl/admin/workflow_attributes_pb2.py` & `lyteidl-0.2.1/gen/pb_python/flyteidl/admin/workflow_attributes_pb2.py`

 * *Files identical despite different names*

### Comparing `lyteidl-0.2.0a0/gen/pb_python/flyteidl/admin/workflow_pb2.py` & `lyteidl-0.2.1/gen/pb_python/flyteidl/admin/workflow_pb2.py`

 * *Files identical despite different names*

### Comparing `lyteidl-0.2.0a0/gen/pb_python/flyteidl/core/catalog_pb2.py` & `lyteidl-0.2.1/gen/pb_python/flyteidl/core/catalog_pb2.py`

 * *Files identical despite different names*

### Comparing `lyteidl-0.2.0a0/gen/pb_python/flyteidl/core/compiler_pb2.py` & `lyteidl-0.2.1/gen/pb_python/flyteidl/core/compiler_pb2.py`

 * *Files identical despite different names*

### Comparing `lyteidl-0.2.0a0/gen/pb_python/flyteidl/core/condition_pb2.py` & `lyteidl-0.2.1/gen/pb_python/flyteidl/core/condition_pb2.py`

 * *Files identical despite different names*

### Comparing `lyteidl-0.2.0a0/gen/pb_python/flyteidl/core/dynamic_job_pb2.py` & `lyteidl-0.2.1/gen/pb_python/flyteidl/core/dynamic_job_pb2.py`

 * *Files identical despite different names*

### Comparing `lyteidl-0.2.0a0/gen/pb_python/flyteidl/core/errors_pb2.py` & `lyteidl-0.2.1/gen/pb_python/flyteidl/core/errors_pb2.py`

 * *Files identical despite different names*

### Comparing `lyteidl-0.2.0a0/gen/pb_python/flyteidl/core/execution_pb2.py` & `lyteidl-0.2.1/gen/pb_python/flyteidl/core/execution_pb2.py`

 * *Files identical despite different names*

### Comparing `lyteidl-0.2.0a0/gen/pb_python/flyteidl/core/identifier_pb2.py` & `lyteidl-0.2.1/gen/pb_python/flyteidl/core/identifier_pb2.py`

 * *Files identical despite different names*

### Comparing `lyteidl-0.2.0a0/gen/pb_python/flyteidl/core/interface_pb2.py` & `lyteidl-0.2.1/gen/pb_python/flyteidl/core/interface_pb2.py`

 * *Files identical despite different names*

### Comparing `lyteidl-0.2.0a0/gen/pb_python/flyteidl/core/literals_pb2.py` & `lyteidl-0.2.1/gen/pb_python/flyteidl/core/literals_pb2.py`

 * *Files identical despite different names*

### Comparing `lyteidl-0.2.0a0/gen/pb_python/flyteidl/core/security_pb2.py` & `lyteidl-0.2.1/gen/pb_python/flyteidl/core/security_pb2.py`

 * *Files identical despite different names*

### Comparing `lyteidl-0.2.0a0/gen/pb_python/flyteidl/core/tasks_pb2.py` & `lyteidl-0.2.1/gen/pb_python/flyteidl/core/tasks_pb2.py`

 * *Files identical despite different names*

### Comparing `lyteidl-0.2.0a0/gen/pb_python/flyteidl/core/types_pb2.py` & `lyteidl-0.2.1/gen/pb_python/flyteidl/core/types_pb2.py`

 * *Files identical despite different names*

### Comparing `lyteidl-0.2.0a0/gen/pb_python/flyteidl/core/workflow_closure_pb2.py` & `lyteidl-0.2.1/gen/pb_python/flyteidl/core/workflow_closure_pb2.py`

 * *Files identical despite different names*

### Comparing `lyteidl-0.2.0a0/gen/pb_python/flyteidl/core/workflow_pb2.py` & `lyteidl-0.2.1/gen/pb_python/flyteidl/core/workflow_pb2.py`

 * *Files identical despite different names*

### Comparing `lyteidl-0.2.0a0/gen/pb_python/flyteidl/datacatalog/datacatalog_pb2.py` & `lyteidl-0.2.1/gen/pb_python/flyteidl/datacatalog/datacatalog_pb2.py`

 * *Files identical despite different names*

### Comparing `lyteidl-0.2.0a0/gen/pb_python/flyteidl/datacatalog/datacatalog_pb2_grpc.py` & `lyteidl-0.2.1/gen/pb_python/flyteidl/datacatalog/datacatalog_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `lyteidl-0.2.0a0/gen/pb_python/flyteidl/event/event_pb2.py` & `lyteidl-0.2.1/gen/pb_python/flyteidl/event/event_pb2.py`

 * *Files identical despite different names*

### Comparing `lyteidl-0.2.0a0/gen/pb_python/flyteidl/plugins/array_job_pb2.py` & `lyteidl-0.2.1/gen/pb_python/flyteidl/plugins/array_job_pb2.py`

 * *Files identical despite different names*

### Comparing `lyteidl-0.2.0a0/gen/pb_python/flyteidl/plugins/mpi_pb2.py` & `lyteidl-0.2.1/gen/pb_python/flyteidl/plugins/mpi_pb2.py`

 * *Files identical despite different names*

### Comparing `lyteidl-0.2.0a0/gen/pb_python/flyteidl/plugins/presto_pb2.py` & `lyteidl-0.2.1/gen/pb_python/flyteidl/plugins/presto_pb2.py`

 * *Files identical despite different names*

### Comparing `lyteidl-0.2.0a0/gen/pb_python/flyteidl/plugins/pytorch_pb2.py` & `lyteidl-0.2.1/gen/pb_python/flyteidl/plugins/pytorch_pb2.py`

 * *Files identical despite different names*

### Comparing `lyteidl-0.2.0a0/gen/pb_python/flyteidl/plugins/qubole_pb2.py` & `lyteidl-0.2.1/gen/pb_python/flyteidl/plugins/qubole_pb2.py`

 * *Files identical despite different names*

### Comparing `lyteidl-0.2.0a0/gen/pb_python/flyteidl/plugins/sagemaker/hyperparameter_tuning_job_pb2.py` & `lyteidl-0.2.1/gen/pb_python/flyteidl/plugins/sagemaker/hyperparameter_tuning_job_pb2.py`

 * *Files identical despite different names*

### Comparing `lyteidl-0.2.0a0/gen/pb_python/flyteidl/plugins/sagemaker/parameter_ranges_pb2.py` & `lyteidl-0.2.1/gen/pb_python/flyteidl/plugins/sagemaker/parameter_ranges_pb2.py`

 * *Files identical despite different names*

### Comparing `lyteidl-0.2.0a0/gen/pb_python/flyteidl/plugins/sagemaker/training_job_pb2.py` & `lyteidl-0.2.1/gen/pb_python/flyteidl/plugins/sagemaker/training_job_pb2.py`

 * *Files identical despite different names*

### Comparing `lyteidl-0.2.0a0/gen/pb_python/flyteidl/plugins/sidecar_pb2.py` & `lyteidl-0.2.1/gen/pb_python/flyteidl/plugins/sidecar_pb2.py`

 * *Files identical despite different names*

### Comparing `lyteidl-0.2.0a0/gen/pb_python/flyteidl/plugins/spark_pb2.py` & `lyteidl-0.2.1/gen/pb_python/flyteidl/plugins/spark_pb2.py`

 * *Files identical despite different names*

### Comparing `lyteidl-0.2.0a0/gen/pb_python/flyteidl/plugins/tensorflow_pb2.py` & `lyteidl-0.2.1/gen/pb_python/flyteidl/plugins/tensorflow_pb2.py`

 * *Files identical despite different names*

### Comparing `lyteidl-0.2.0a0/gen/pb_python/flyteidl/plugins/waitable_pb2.py` & `lyteidl-0.2.1/gen/pb_python/flyteidl/plugins/waitable_pb2.py`

 * *Files identical despite different names*

### Comparing `lyteidl-0.2.0a0/gen/pb_python/flyteidl/service/admin_pb2.py` & `lyteidl-0.2.1/gen/pb_python/flyteidl/service/admin_pb2.py`

 * *Files identical despite different names*

### Comparing `lyteidl-0.2.0a0/gen/pb_python/flyteidl/service/admin_pb2_grpc.py` & `lyteidl-0.2.1/gen/pb_python/flyteidl/service/admin_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `lyteidl-0.2.0a0/gen/pb_python/flyteidl/service/auth_pb2.py` & `lyteidl-0.2.1/gen/pb_python/flyteidl/service/auth_pb2.py`

 * *Files identical despite different names*

### Comparing `lyteidl-0.2.0a0/gen/pb_python/flyteidl/service/auth_pb2_grpc.py` & `lyteidl-0.2.1/gen/pb_python/flyteidl/service/auth_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `lyteidl-0.2.0a0/gen/pb_python/flyteidl/service/dataproxy_pb2.py` & `lyteidl-0.2.1/gen/pb_python/flyteidl/service/dataproxy_pb2.py`

 * *Files identical despite different names*

### Comparing `lyteidl-0.2.0a0/gen/pb_python/flyteidl/service/dataproxy_pb2_grpc.py` & `lyteidl-0.2.1/gen/pb_python/flyteidl/service/dataproxy_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `lyteidl-0.2.0a0/gen/pb_python/flyteidl/service/identity_pb2.py` & `lyteidl-0.2.1/gen/pb_python/flyteidl/service/identity_pb2.py`

 * *Files identical despite different names*

### Comparing `lyteidl-0.2.0a0/gen/pb_python/flyteidl/service/identity_pb2_grpc.py` & `lyteidl-0.2.1/gen/pb_python/flyteidl/service/identity_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `lyteidl-0.2.0a0/gen/pb_python/lyteidl.egg-info/SOURCES.txt` & `lyteidl-0.2.1/gen/pb_python/lyteidl.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -2,98 +2,139 @@
 NOTICE
 README.md
 setup.cfg
 setup.py
 gen/pb_python/flyteidl/__init__.py
 gen/pb_python/flyteidl/admin/__init__.py
 gen/pb_python/flyteidl/admin/cluster_assignment_pb2.py
+gen/pb_python/flyteidl/admin/cluster_assignment_pb2.pyi
 gen/pb_python/flyteidl/admin/cluster_assignment_pb2_grpc.py
 gen/pb_python/flyteidl/admin/common_pb2.py
+gen/pb_python/flyteidl/admin/common_pb2.pyi
 gen/pb_python/flyteidl/admin/common_pb2_grpc.py
 gen/pb_python/flyteidl/admin/event_pb2.py
+gen/pb_python/flyteidl/admin/event_pb2.pyi
 gen/pb_python/flyteidl/admin/event_pb2_grpc.py
 gen/pb_python/flyteidl/admin/execution_pb2.py
+gen/pb_python/flyteidl/admin/execution_pb2.pyi
 gen/pb_python/flyteidl/admin/execution_pb2_grpc.py
 gen/pb_python/flyteidl/admin/launch_plan_pb2.py
+gen/pb_python/flyteidl/admin/launch_plan_pb2.pyi
 gen/pb_python/flyteidl/admin/launch_plan_pb2_grpc.py
 gen/pb_python/flyteidl/admin/matchable_resource_pb2.py
+gen/pb_python/flyteidl/admin/matchable_resource_pb2.pyi
 gen/pb_python/flyteidl/admin/matchable_resource_pb2_grpc.py
 gen/pb_python/flyteidl/admin/node_execution_pb2.py
+gen/pb_python/flyteidl/admin/node_execution_pb2.pyi
 gen/pb_python/flyteidl/admin/node_execution_pb2_grpc.py
 gen/pb_python/flyteidl/admin/notification_pb2.py
+gen/pb_python/flyteidl/admin/notification_pb2.pyi
 gen/pb_python/flyteidl/admin/notification_pb2_grpc.py
 gen/pb_python/flyteidl/admin/project_domain_attributes_pb2.py
+gen/pb_python/flyteidl/admin/project_domain_attributes_pb2.pyi
 gen/pb_python/flyteidl/admin/project_domain_attributes_pb2_grpc.py
 gen/pb_python/flyteidl/admin/project_pb2.py
+gen/pb_python/flyteidl/admin/project_pb2.pyi
 gen/pb_python/flyteidl/admin/project_pb2_grpc.py
 gen/pb_python/flyteidl/admin/schedule_pb2.py
+gen/pb_python/flyteidl/admin/schedule_pb2.pyi
 gen/pb_python/flyteidl/admin/schedule_pb2_grpc.py
 gen/pb_python/flyteidl/admin/task_execution_pb2.py
+gen/pb_python/flyteidl/admin/task_execution_pb2.pyi
 gen/pb_python/flyteidl/admin/task_execution_pb2_grpc.py
 gen/pb_python/flyteidl/admin/task_pb2.py
+gen/pb_python/flyteidl/admin/task_pb2.pyi
 gen/pb_python/flyteidl/admin/task_pb2_grpc.py
 gen/pb_python/flyteidl/admin/version_pb2.py
+gen/pb_python/flyteidl/admin/version_pb2.pyi
 gen/pb_python/flyteidl/admin/version_pb2_grpc.py
 gen/pb_python/flyteidl/admin/workflow_attributes_pb2.py
+gen/pb_python/flyteidl/admin/workflow_attributes_pb2.pyi
 gen/pb_python/flyteidl/admin/workflow_attributes_pb2_grpc.py
 gen/pb_python/flyteidl/admin/workflow_pb2.py
+gen/pb_python/flyteidl/admin/workflow_pb2.pyi
 gen/pb_python/flyteidl/admin/workflow_pb2_grpc.py
 gen/pb_python/flyteidl/core/__init__.py
 gen/pb_python/flyteidl/core/catalog_pb2.py
+gen/pb_python/flyteidl/core/catalog_pb2.pyi
 gen/pb_python/flyteidl/core/catalog_pb2_grpc.py
 gen/pb_python/flyteidl/core/compiler_pb2.py
+gen/pb_python/flyteidl/core/compiler_pb2.pyi
 gen/pb_python/flyteidl/core/compiler_pb2_grpc.py
 gen/pb_python/flyteidl/core/condition_pb2.py
+gen/pb_python/flyteidl/core/condition_pb2.pyi
 gen/pb_python/flyteidl/core/condition_pb2_grpc.py
 gen/pb_python/flyteidl/core/dynamic_job_pb2.py
+gen/pb_python/flyteidl/core/dynamic_job_pb2.pyi
 gen/pb_python/flyteidl/core/dynamic_job_pb2_grpc.py
 gen/pb_python/flyteidl/core/errors_pb2.py
+gen/pb_python/flyteidl/core/errors_pb2.pyi
 gen/pb_python/flyteidl/core/errors_pb2_grpc.py
 gen/pb_python/flyteidl/core/execution_pb2.py
+gen/pb_python/flyteidl/core/execution_pb2.pyi
 gen/pb_python/flyteidl/core/execution_pb2_grpc.py
 gen/pb_python/flyteidl/core/identifier_pb2.py
+gen/pb_python/flyteidl/core/identifier_pb2.pyi
 gen/pb_python/flyteidl/core/identifier_pb2_grpc.py
 gen/pb_python/flyteidl/core/interface_pb2.py
+gen/pb_python/flyteidl/core/interface_pb2.pyi
 gen/pb_python/flyteidl/core/interface_pb2_grpc.py
 gen/pb_python/flyteidl/core/literals_pb2.py
+gen/pb_python/flyteidl/core/literals_pb2.pyi
 gen/pb_python/flyteidl/core/literals_pb2_grpc.py
 gen/pb_python/flyteidl/core/security_pb2.py
+gen/pb_python/flyteidl/core/security_pb2.pyi
 gen/pb_python/flyteidl/core/security_pb2_grpc.py
 gen/pb_python/flyteidl/core/tasks_pb2.py
+gen/pb_python/flyteidl/core/tasks_pb2.pyi
 gen/pb_python/flyteidl/core/tasks_pb2_grpc.py
 gen/pb_python/flyteidl/core/types_pb2.py
+gen/pb_python/flyteidl/core/types_pb2.pyi
 gen/pb_python/flyteidl/core/types_pb2_grpc.py
 gen/pb_python/flyteidl/core/workflow_closure_pb2.py
+gen/pb_python/flyteidl/core/workflow_closure_pb2.pyi
 gen/pb_python/flyteidl/core/workflow_closure_pb2_grpc.py
 gen/pb_python/flyteidl/core/workflow_pb2.py
+gen/pb_python/flyteidl/core/workflow_pb2.pyi
 gen/pb_python/flyteidl/core/workflow_pb2_grpc.py
 gen/pb_python/flyteidl/datacatalog/__init__.py
 gen/pb_python/flyteidl/datacatalog/datacatalog_pb2.py
+gen/pb_python/flyteidl/datacatalog/datacatalog_pb2.pyi
 gen/pb_python/flyteidl/datacatalog/datacatalog_pb2_grpc.py
 gen/pb_python/flyteidl/event/__init__.py
 gen/pb_python/flyteidl/event/event_pb2.py
+gen/pb_python/flyteidl/event/event_pb2.pyi
 gen/pb_python/flyteidl/event/event_pb2_grpc.py
 gen/pb_python/flyteidl/plugins/__init__.py
 gen/pb_python/flyteidl/plugins/array_job_pb2.py
+gen/pb_python/flyteidl/plugins/array_job_pb2.pyi
 gen/pb_python/flyteidl/plugins/array_job_pb2_grpc.py
 gen/pb_python/flyteidl/plugins/mpi_pb2.py
+gen/pb_python/flyteidl/plugins/mpi_pb2.pyi
 gen/pb_python/flyteidl/plugins/mpi_pb2_grpc.py
 gen/pb_python/flyteidl/plugins/presto_pb2.py
+gen/pb_python/flyteidl/plugins/presto_pb2.pyi
 gen/pb_python/flyteidl/plugins/presto_pb2_grpc.py
 gen/pb_python/flyteidl/plugins/pytorch_pb2.py
+gen/pb_python/flyteidl/plugins/pytorch_pb2.pyi
 gen/pb_python/flyteidl/plugins/pytorch_pb2_grpc.py
 gen/pb_python/flyteidl/plugins/qubole_pb2.py
+gen/pb_python/flyteidl/plugins/qubole_pb2.pyi
 gen/pb_python/flyteidl/plugins/qubole_pb2_grpc.py
 gen/pb_python/flyteidl/plugins/sidecar_pb2.py
+gen/pb_python/flyteidl/plugins/sidecar_pb2.pyi
 gen/pb_python/flyteidl/plugins/sidecar_pb2_grpc.py
 gen/pb_python/flyteidl/plugins/spark_pb2.py
+gen/pb_python/flyteidl/plugins/spark_pb2.pyi
 gen/pb_python/flyteidl/plugins/spark_pb2_grpc.py
 gen/pb_python/flyteidl/plugins/tensorflow_pb2.py
+gen/pb_python/flyteidl/plugins/tensorflow_pb2.pyi
 gen/pb_python/flyteidl/plugins/tensorflow_pb2_grpc.py
 gen/pb_python/flyteidl/plugins/waitable_pb2.py
+gen/pb_python/flyteidl/plugins/waitable_pb2.pyi
 gen/pb_python/flyteidl/plugins/waitable_pb2_grpc.py
 gen/pb_python/flyteidl/plugins/sagemaker/__init__.py
 gen/pb_python/flyteidl/plugins/sagemaker/hyperparameter_tuning_job_pb2.py
 gen/pb_python/flyteidl/plugins/sagemaker/hyperparameter_tuning_job_pb2_grpc.py
 gen/pb_python/flyteidl/plugins/sagemaker/parameter_ranges_pb2.py
 gen/pb_python/flyteidl/plugins/sagemaker/parameter_ranges_pb2_grpc.py
 gen/pb_python/flyteidl/plugins/sagemaker/training_job_pb2.py
```

### Comparing `lyteidl-0.2.0a0/gen/pb_python/validate/validate_pb2.py` & `lyteidl-0.2.1/gen/pb_python/validate/validate_pb2.py`

 * *Files identical despite different names*

### Comparing `lyteidl-0.2.0a0/setup.cfg` & `lyteidl-0.2.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `lyteidl-0.2.0a0/setup.py` & `lyteidl-0.2.1/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 import os
 
 from setuptools import find_packages, setup
 
 __version__ = os.getenv("VERSION") or "0.0.0+develop"
 
+packages = find_packages("gen/pb_python")
+
 setup(
     name="lyteidl",
     version=__version__,
     description="IDL for Flyte Platform",
     url="https://www.github.com/flyteorg/flyteidl",
     maintainer="FlyteOrg",
     maintainer_email="admin@flyte.org",
     packages=find_packages("gen/pb_python"),
     package_dir={"": "gen/pb_python"},
+    package_data={x: ["py.typed", "*.pyi", "**/*.pyi"] for x  in packages},
     dependency_links=[],
     install_requires=[
         "googleapis-common-protos",
         "protoc_gen_swagger",
         "protobuf>=3.5.0,<4.0.0",
         # Packages in here should rarely be pinned. This is because these
         # packages (at the specified version) are required for project
```

