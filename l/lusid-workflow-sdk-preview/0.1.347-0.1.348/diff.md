# Comparing `tmp/lusid-workflow-sdk-preview-0.1.347.tar.gz` & `tmp/lusid-workflow-sdk-preview-0.1.348.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/lusid-workflow-sdk-preview-0.1.347.tar", last modified: Tue Jul 11 15:37:56 2023, max compression
+gzip compressed data, was "dist/lusid-workflow-sdk-preview-0.1.348.tar", last modified: Thu Jul 13 09:37:47 2023, max compression
```

## Comparing `lusid-workflow-sdk-preview-0.1.347.tar` & `lusid-workflow-sdk-preview-0.1.348.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:37:56.000000 lusid-workflow-sdk-preview-0.1.347/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 15:37:20.000000 lusid-workflow-sdk-preview-0.1.347/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      353 2023-07-11 15:37:56.000000 lusid-workflow-sdk-preview-0.1.347/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     9652 2023-07-11 15:37:20.000000 lusid-workflow-sdk-preview-0.1.347/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:37:56.000000 lusid-workflow-sdk-preview-0.1.347/lusid_workflow/
--rw-r--r--   0 root         (0) root         (0)     4540 2023-07-11 15:37:20.000000 lusid-workflow-sdk-preview-0.1.347/lusid_workflow/__init__.py
--rw-r--r--   0 root         (0) root         (0)       24 2023-07-11 15:37:20.000000 lusid-workflow-sdk-preview-0.1.347/lusid_workflow/__version__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:37:56.000000 lusid-workflow-sdk-preview-0.1.347/lusid_workflow/api/
--rw-r--r--   0 root         (0) root         (0)      262 2023-07-11 15:37:20.000000 lusid-workflow-sdk-preview-0.1.347/lusid_workflow/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)    56187 2023-07-11 15:37:20.000000 lusid-workflow-sdk-preview-0.1.347/lusid_workflow/api/task_definitions_api.py
--rw-r--r--   0 root         (0) root         (0)    41163 2023-07-11 15:37:20.000000 lusid-workflow-sdk-preview-0.1.347/lusid_workflow/api/tasks_api.py
--rw-r--r--   0 root         (0) root         (0)    36409 2023-07-11 15:37:20.000000 lusid-workflow-sdk-preview-0.1.347/lusid_workflow/api/workers_api.py
--rw-r--r--   0 root         (0) root         (0)    27406 2023-07-11 15:37:20.000000 lusid-workflow-sdk-preview-0.1.347/lusid_workflow/api_client.py
--rw-r--r--   0 root         (0) root         (0)    16610 2023-07-11 15:37:20.000000 lusid-workflow-sdk-preview-0.1.347/lusid_workflow/configuration.py
--rw-r--r--   0 root         (0) root         (0)     5094 2023-07-11 15:37:20.000000 lusid-workflow-sdk-preview-0.1.347/lusid_workflow/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:37:56.000000 lusid-workflow-sdk-preview-0.1.347/lusid_workflow/models/
--rw-r--r--   0 root         (0) root         (0)     3460 2023-07-11 15:37:20.000000 lusid-workflow-sdk-preview-0.1.347/lusid_workflow/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6094 2023-07-11 15:37:20.000000 lusid-workflow-sdk-preview-0.1.347/lusid_workflow/models/action_definition.py
--rw-r--r--   0 root         (0) root         (0)    12089 2023-07-11 15:37:20.000000 lusid-workflow-sdk-preview-0.1.347/lusid_workflow/models/action_details.py
--rw-r--r--   0 root         (0) root         (0)     6004 2023-07-11 15:37:20.000000 lusid-workflow-sdk-preview-0.1.347/lusid_workflow/models/create_child_tasks_action.py
--rw-r--r--   0 root         (0) root         (0)    13450 2023-07-11 15:37:20.000000 lusid-workflow-sdk-preview-0.1.347/lusid_workflow/models/create_task_definition_request.py
--rw-r--r--   0 root         (0) root         (0)     6783 2023-07-11 15:37:20.000000 lusid-workflow-sdk-preview-0.1.347/lusid_workflow/models/create_task_request.py
--rw-r--r--   0 root         (0) root         (0)     9176 2023-07-11 15:37:20.000000 lusid-workflow-sdk-preview-0.1.347/lusid_workflow/models/create_worker_request.py
--rw-r--r--   0 root         (0) root         (0)     6852 2023-07-11 15:37:20.000000 lusid-workflow-sdk-preview-0.1.347/lusid_workflow/models/deleted_entity_response.py
--rw-r--r--   0 root         (0) root         (0)     6403 2023-07-11 15:37:20.000000 lusid-workflow-sdk-preview-0.1.347/lusid_workflow/models/field_mapping.py
--rw-r--r--   0 root         (0) root         (0)     5878 2023-07-11 15:37:20.000000 lusid-workflow-sdk-preview-0.1.347/lusid_workflow/models/health_check.py
--rw-r--r--   0 root         (0) root         (0)     5984 2023-07-11 15:37:20.000000 lusid-workflow-sdk-preview-0.1.347/lusid_workflow/models/initial_state.py
--rw-r--r--   0 root         (0) root         (0)     6416 2023-07-11 15:37:20.000000 lusid-workflow-sdk-preview-0.1.347/lusid_workflow/models/link.py
--rw-r--r--   0 root         (0) root         (0)     6165 2023-07-11 15:37:20.000000 lusid-workflow-sdk-preview-0.1.347/lusid_workflow/models/luminesce_view.py
--rw-r--r--   0 root         (0) root         (0)     9530 2023-07-11 15:37:20.000000 lusid-workflow-sdk-preview-0.1.347/lusid_workflow/models/lusid_problem_details.py
--rw-r--r--   0 root         (0) root         (0)    10695 2023-07-11 15:37:20.000000 lusid-workflow-sdk-preview-0.1.347/lusid_workflow/models/lusid_validation_problem_details.py
--rw-r--r--   0 root         (0) root         (0)     7295 2023-07-11 15:37:20.000000 lusid-workflow-sdk-preview-0.1.347/lusid_workflow/models/paged_resource_list_of_task.py
--rw-r--r--   0 root         (0) root         (0)     7575 2023-07-11 15:37:20.000000 lusid-workflow-sdk-preview-0.1.347/lusid_workflow/models/paged_resource_list_of_task_definition.py
--rw-r--r--   0 root         (0) root         (0)     7351 2023-07-11 15:37:20.000000 lusid-workflow-sdk-preview-0.1.347/lusid_workflow/models/paged_resource_list_of_worker.py
--rw-r--r--   0 root         (0) root         (0)     9076 2023-07-11 15:37:20.000000 lusid-workflow-sdk-preview-0.1.347/lusid_workflow/models/parameter.py
--rw-r--r--   0 root         (0) root         (0)     5767 2023-07-11 15:37:20.000000 lusid-workflow-sdk-preview-0.1.347/lusid_workflow/models/parameter_value.py
--rw-r--r--   0 root         (0) root         (0)     4822 2023-07-11 15:37:20.000000 lusid-workflow-sdk-preview-0.1.347/lusid_workflow/models/resource_id.py
--rw-r--r--   0 root         (0) root         (0)     7175 2023-07-11 15:37:20.000000 lusid-workflow-sdk-preview-0.1.347/lusid_workflow/models/resource_list_of_task.py
--rw-r--r--   0 root         (0) root         (0)     7211 2023-07-11 15:37:20.000000 lusid-workflow-sdk-preview-0.1.347/lusid_workflow/models/result_field.py
--rw-r--r--   0 root         (0) root         (0)     4985 2023-07-11 15:37:20.000000 lusid-workflow-sdk-preview-0.1.347/lusid_workflow/models/result_matching_pattern.py
--rw-r--r--   0 root         (0) root         (0)    10269 2023-07-11 15:37:20.000000 lusid-workflow-sdk-preview-0.1.347/lusid_workflow/models/resultant_child_task_configuration.py
--rw-r--r--   0 root         (0) root         (0)    10386 2023-07-11 15:37:20.000000 lusid-workflow-sdk-preview-0.1.347/lusid_workflow/models/run_worker_action.py
--rw-r--r--   0 root         (0) root         (0)     4435 2023-07-11 15:37:20.000000 lusid-workflow-sdk-preview-0.1.347/lusid_workflow/models/run_worker_request.py
--rw-r--r--   0 root         (0) root         (0)     6704 2023-07-11 15:37:20.000000 lusid-workflow-sdk-preview-0.1.347/lusid_workflow/models/run_worker_response.py
--rw-r--r--   0 root         (0) root         (0)    12984 2023-07-11 15:37:20.000000 lusid-workflow-sdk-preview-0.1.347/lusid_workflow/models/task.py
--rw-r--r--   0 root         (0) root         (0)    14061 2023-07-11 15:37:20.000000 lusid-workflow-sdk-preview-0.1.347/lusid_workflow/models/task_definition.py
--rw-r--r--   0 root         (0) root         (0)     4386 2023-07-11 15:37:20.000000 lusid-workflow-sdk-preview-0.1.347/lusid_workflow/models/task_definition_version.py
--rw-r--r--   0 root         (0) root         (0)     6387 2023-07-11 15:37:20.000000 lusid-workflow-sdk-preview-0.1.347/lusid_workflow/models/task_field_definition.py
--rw-r--r--   0 root         (0) root         (0)     5231 2023-07-11 15:37:20.000000 lusid-workflow-sdk-preview-0.1.347/lusid_workflow/models/task_instance_field.py
--rw-r--r--   0 root         (0) root         (0)     4944 2023-07-11 15:37:20.000000 lusid-workflow-sdk-preview-0.1.347/lusid_workflow/models/task_state_definition.py
--rw-r--r--   0 root         (0) root         (0)    12376 2023-07-11 15:37:20.000000 lusid-workflow-sdk-preview-0.1.347/lusid_workflow/models/task_transition_definition.py
--rw-r--r--   0 root         (0) root         (0)     6067 2023-07-11 15:37:20.000000 lusid-workflow-sdk-preview-0.1.347/lusid_workflow/models/transition_trigger_definition.py
--rw-r--r--   0 root         (0) root         (0)     6451 2023-07-11 15:37:20.000000 lusid-workflow-sdk-preview-0.1.347/lusid_workflow/models/trigger_parent_task_action.py
--rw-r--r--   0 root         (0) root         (0)     4440 2023-07-11 15:37:20.000000 lusid-workflow-sdk-preview-0.1.347/lusid_workflow/models/trigger_schema.py
--rw-r--r--   0 root         (0) root         (0)    12546 2023-07-11 15:37:20.000000 lusid-workflow-sdk-preview-0.1.347/lusid_workflow/models/update_task_definition_request.py
--rw-r--r--   0 root         (0) root         (0)     5389 2023-07-11 15:37:20.000000 lusid-workflow-sdk-preview-0.1.347/lusid_workflow/models/update_task_request.py
--rw-r--r--   0 root         (0) root         (0)    11105 2023-07-11 15:37:20.000000 lusid-workflow-sdk-preview-0.1.347/lusid_workflow/models/version_info.py
--rw-r--r--   0 root         (0) root         (0)    11023 2023-07-11 15:37:20.000000 lusid-workflow-sdk-preview-0.1.347/lusid_workflow/models/worker.py
--rw-r--r--   0 root         (0) root         (0)     7614 2023-07-11 15:37:20.000000 lusid-workflow-sdk-preview-0.1.347/lusid_workflow/models/worker_configuration.py
--rw-r--r--   0 root         (0) root         (0)     8967 2023-07-11 15:37:20.000000 lusid-workflow-sdk-preview-0.1.347/lusid_workflow/models/worker_status_triggers.py
--rw-r--r--   0 root         (0) root         (0)    13551 2023-07-11 15:37:20.000000 lusid-workflow-sdk-preview-0.1.347/lusid_workflow/rest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:37:56.000000 lusid-workflow-sdk-preview-0.1.347/lusid_workflow_sdk_preview.egg-info/
--rw-r--r--   0 root         (0) root         (0)      353 2023-07-11 15:37:56.000000 lusid-workflow-sdk-preview-0.1.347/lusid_workflow_sdk_preview.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2579 2023-07-11 15:37:56.000000 lusid-workflow-sdk-preview-0.1.347/lusid_workflow_sdk_preview.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-11 15:37:56.000000 lusid-workflow-sdk-preview-0.1.347/lusid_workflow_sdk_preview.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      116 2023-07-11 15:37:56.000000 lusid-workflow-sdk-preview-0.1.347/lusid_workflow_sdk_preview.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-07-11 15:37:56.000000 lusid-workflow-sdk-preview-0.1.347/lusid_workflow_sdk_preview.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-11 15:37:56.000000 lusid-workflow-sdk-preview-0.1.347/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2237 2023-07-11 15:37:20.000000 lusid-workflow-sdk-preview-0.1.347/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 09:37:47.000000 lusid-workflow-sdk-preview-0.1.348/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-13 09:36:01.000000 lusid-workflow-sdk-preview-0.1.348/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      353 2023-07-13 09:37:47.000000 lusid-workflow-sdk-preview-0.1.348/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     9652 2023-07-13 09:36:01.000000 lusid-workflow-sdk-preview-0.1.348/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 09:37:47.000000 lusid-workflow-sdk-preview-0.1.348/lusid_workflow/
+-rw-r--r--   0 root         (0) root         (0)     4540 2023-07-13 09:36:01.000000 lusid-workflow-sdk-preview-0.1.348/lusid_workflow/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       24 2023-07-13 09:36:01.000000 lusid-workflow-sdk-preview-0.1.348/lusid_workflow/__version__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 09:37:47.000000 lusid-workflow-sdk-preview-0.1.348/lusid_workflow/api/
+-rw-r--r--   0 root         (0) root         (0)      262 2023-07-13 09:36:01.000000 lusid-workflow-sdk-preview-0.1.348/lusid_workflow/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    56187 2023-07-13 09:36:01.000000 lusid-workflow-sdk-preview-0.1.348/lusid_workflow/api/task_definitions_api.py
+-rw-r--r--   0 root         (0) root         (0)    41163 2023-07-13 09:36:01.000000 lusid-workflow-sdk-preview-0.1.348/lusid_workflow/api/tasks_api.py
+-rw-r--r--   0 root         (0) root         (0)    36409 2023-07-13 09:36:01.000000 lusid-workflow-sdk-preview-0.1.348/lusid_workflow/api/workers_api.py
+-rw-r--r--   0 root         (0) root         (0)    27406 2023-07-13 09:36:01.000000 lusid-workflow-sdk-preview-0.1.348/lusid_workflow/api_client.py
+-rw-r--r--   0 root         (0) root         (0)    16610 2023-07-13 09:36:01.000000 lusid-workflow-sdk-preview-0.1.348/lusid_workflow/configuration.py
+-rw-r--r--   0 root         (0) root         (0)     5094 2023-07-13 09:36:01.000000 lusid-workflow-sdk-preview-0.1.348/lusid_workflow/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 09:37:47.000000 lusid-workflow-sdk-preview-0.1.348/lusid_workflow/models/
+-rw-r--r--   0 root         (0) root         (0)     3460 2023-07-13 09:36:01.000000 lusid-workflow-sdk-preview-0.1.348/lusid_workflow/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6094 2023-07-13 09:36:01.000000 lusid-workflow-sdk-preview-0.1.348/lusid_workflow/models/action_definition.py
+-rw-r--r--   0 root         (0) root         (0)    12089 2023-07-13 09:36:01.000000 lusid-workflow-sdk-preview-0.1.348/lusid_workflow/models/action_details.py
+-rw-r--r--   0 root         (0) root         (0)     6004 2023-07-13 09:36:01.000000 lusid-workflow-sdk-preview-0.1.348/lusid_workflow/models/create_child_tasks_action.py
+-rw-r--r--   0 root         (0) root         (0)    13450 2023-07-13 09:36:01.000000 lusid-workflow-sdk-preview-0.1.348/lusid_workflow/models/create_task_definition_request.py
+-rw-r--r--   0 root         (0) root         (0)     6783 2023-07-13 09:36:01.000000 lusid-workflow-sdk-preview-0.1.348/lusid_workflow/models/create_task_request.py
+-rw-r--r--   0 root         (0) root         (0)     9176 2023-07-13 09:36:01.000000 lusid-workflow-sdk-preview-0.1.348/lusid_workflow/models/create_worker_request.py
+-rw-r--r--   0 root         (0) root         (0)     6852 2023-07-13 09:36:01.000000 lusid-workflow-sdk-preview-0.1.348/lusid_workflow/models/deleted_entity_response.py
+-rw-r--r--   0 root         (0) root         (0)     6403 2023-07-13 09:36:01.000000 lusid-workflow-sdk-preview-0.1.348/lusid_workflow/models/field_mapping.py
+-rw-r--r--   0 root         (0) root         (0)     5878 2023-07-13 09:36:01.000000 lusid-workflow-sdk-preview-0.1.348/lusid_workflow/models/health_check.py
+-rw-r--r--   0 root         (0) root         (0)     5984 2023-07-13 09:36:01.000000 lusid-workflow-sdk-preview-0.1.348/lusid_workflow/models/initial_state.py
+-rw-r--r--   0 root         (0) root         (0)     6416 2023-07-13 09:36:01.000000 lusid-workflow-sdk-preview-0.1.348/lusid_workflow/models/link.py
+-rw-r--r--   0 root         (0) root         (0)     6165 2023-07-13 09:36:01.000000 lusid-workflow-sdk-preview-0.1.348/lusid_workflow/models/luminesce_view.py
+-rw-r--r--   0 root         (0) root         (0)     9530 2023-07-13 09:36:01.000000 lusid-workflow-sdk-preview-0.1.348/lusid_workflow/models/lusid_problem_details.py
+-rw-r--r--   0 root         (0) root         (0)    10695 2023-07-13 09:36:01.000000 lusid-workflow-sdk-preview-0.1.348/lusid_workflow/models/lusid_validation_problem_details.py
+-rw-r--r--   0 root         (0) root         (0)     7295 2023-07-13 09:36:01.000000 lusid-workflow-sdk-preview-0.1.348/lusid_workflow/models/paged_resource_list_of_task.py
+-rw-r--r--   0 root         (0) root         (0)     7575 2023-07-13 09:36:01.000000 lusid-workflow-sdk-preview-0.1.348/lusid_workflow/models/paged_resource_list_of_task_definition.py
+-rw-r--r--   0 root         (0) root         (0)     7351 2023-07-13 09:36:01.000000 lusid-workflow-sdk-preview-0.1.348/lusid_workflow/models/paged_resource_list_of_worker.py
+-rw-r--r--   0 root         (0) root         (0)     9076 2023-07-13 09:36:01.000000 lusid-workflow-sdk-preview-0.1.348/lusid_workflow/models/parameter.py
+-rw-r--r--   0 root         (0) root         (0)     5767 2023-07-13 09:36:01.000000 lusid-workflow-sdk-preview-0.1.348/lusid_workflow/models/parameter_value.py
+-rw-r--r--   0 root         (0) root         (0)     4822 2023-07-13 09:36:01.000000 lusid-workflow-sdk-preview-0.1.348/lusid_workflow/models/resource_id.py
+-rw-r--r--   0 root         (0) root         (0)     7175 2023-07-13 09:36:01.000000 lusid-workflow-sdk-preview-0.1.348/lusid_workflow/models/resource_list_of_task.py
+-rw-r--r--   0 root         (0) root         (0)     7211 2023-07-13 09:36:01.000000 lusid-workflow-sdk-preview-0.1.348/lusid_workflow/models/result_field.py
+-rw-r--r--   0 root         (0) root         (0)     4985 2023-07-13 09:36:01.000000 lusid-workflow-sdk-preview-0.1.348/lusid_workflow/models/result_matching_pattern.py
+-rw-r--r--   0 root         (0) root         (0)    10269 2023-07-13 09:36:01.000000 lusid-workflow-sdk-preview-0.1.348/lusid_workflow/models/resultant_child_task_configuration.py
+-rw-r--r--   0 root         (0) root         (0)    10386 2023-07-13 09:36:01.000000 lusid-workflow-sdk-preview-0.1.348/lusid_workflow/models/run_worker_action.py
+-rw-r--r--   0 root         (0) root         (0)     4435 2023-07-13 09:36:01.000000 lusid-workflow-sdk-preview-0.1.348/lusid_workflow/models/run_worker_request.py
+-rw-r--r--   0 root         (0) root         (0)     6704 2023-07-13 09:36:01.000000 lusid-workflow-sdk-preview-0.1.348/lusid_workflow/models/run_worker_response.py
+-rw-r--r--   0 root         (0) root         (0)    12984 2023-07-13 09:36:01.000000 lusid-workflow-sdk-preview-0.1.348/lusid_workflow/models/task.py
+-rw-r--r--   0 root         (0) root         (0)    14061 2023-07-13 09:36:01.000000 lusid-workflow-sdk-preview-0.1.348/lusid_workflow/models/task_definition.py
+-rw-r--r--   0 root         (0) root         (0)     4386 2023-07-13 09:36:01.000000 lusid-workflow-sdk-preview-0.1.348/lusid_workflow/models/task_definition_version.py
+-rw-r--r--   0 root         (0) root         (0)     6387 2023-07-13 09:36:01.000000 lusid-workflow-sdk-preview-0.1.348/lusid_workflow/models/task_field_definition.py
+-rw-r--r--   0 root         (0) root         (0)     5231 2023-07-13 09:36:01.000000 lusid-workflow-sdk-preview-0.1.348/lusid_workflow/models/task_instance_field.py
+-rw-r--r--   0 root         (0) root         (0)     4944 2023-07-13 09:36:01.000000 lusid-workflow-sdk-preview-0.1.348/lusid_workflow/models/task_state_definition.py
+-rw-r--r--   0 root         (0) root         (0)    12376 2023-07-13 09:36:01.000000 lusid-workflow-sdk-preview-0.1.348/lusid_workflow/models/task_transition_definition.py
+-rw-r--r--   0 root         (0) root         (0)     6067 2023-07-13 09:36:01.000000 lusid-workflow-sdk-preview-0.1.348/lusid_workflow/models/transition_trigger_definition.py
+-rw-r--r--   0 root         (0) root         (0)     6451 2023-07-13 09:36:01.000000 lusid-workflow-sdk-preview-0.1.348/lusid_workflow/models/trigger_parent_task_action.py
+-rw-r--r--   0 root         (0) root         (0)     4440 2023-07-13 09:36:01.000000 lusid-workflow-sdk-preview-0.1.348/lusid_workflow/models/trigger_schema.py
+-rw-r--r--   0 root         (0) root         (0)    12546 2023-07-13 09:36:01.000000 lusid-workflow-sdk-preview-0.1.348/lusid_workflow/models/update_task_definition_request.py
+-rw-r--r--   0 root         (0) root         (0)     5389 2023-07-13 09:36:01.000000 lusid-workflow-sdk-preview-0.1.348/lusid_workflow/models/update_task_request.py
+-rw-r--r--   0 root         (0) root         (0)    11105 2023-07-13 09:36:01.000000 lusid-workflow-sdk-preview-0.1.348/lusid_workflow/models/version_info.py
+-rw-r--r--   0 root         (0) root         (0)    11023 2023-07-13 09:36:01.000000 lusid-workflow-sdk-preview-0.1.348/lusid_workflow/models/worker.py
+-rw-r--r--   0 root         (0) root         (0)     7614 2023-07-13 09:36:01.000000 lusid-workflow-sdk-preview-0.1.348/lusid_workflow/models/worker_configuration.py
+-rw-r--r--   0 root         (0) root         (0)     8967 2023-07-13 09:36:01.000000 lusid-workflow-sdk-preview-0.1.348/lusid_workflow/models/worker_status_triggers.py
+-rw-r--r--   0 root         (0) root         (0)    13551 2023-07-13 09:36:01.000000 lusid-workflow-sdk-preview-0.1.348/lusid_workflow/rest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 09:37:47.000000 lusid-workflow-sdk-preview-0.1.348/lusid_workflow_sdk_preview.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      353 2023-07-13 09:37:47.000000 lusid-workflow-sdk-preview-0.1.348/lusid_workflow_sdk_preview.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2579 2023-07-13 09:37:47.000000 lusid-workflow-sdk-preview-0.1.348/lusid_workflow_sdk_preview.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-13 09:37:47.000000 lusid-workflow-sdk-preview-0.1.348/lusid_workflow_sdk_preview.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      116 2023-07-13 09:37:47.000000 lusid-workflow-sdk-preview-0.1.348/lusid_workflow_sdk_preview.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-07-13 09:37:47.000000 lusid-workflow-sdk-preview-0.1.348/lusid_workflow_sdk_preview.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-13 09:37:47.000000 lusid-workflow-sdk-preview-0.1.348/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2237 2023-07-13 09:36:01.000000 lusid-workflow-sdk-preview-0.1.348/setup.py
```

### Comparing `lusid-workflow-sdk-preview-0.1.347/README.md` & `lusid-workflow-sdk-preview-0.1.348/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # lusid-workflow-sdk
 FINBOURNE Technology
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 0.1.347
-- Package version: 0.1.347
+- API version: 0.1.348
+- Package version: 0.1.348
 - Build package: org.openapitools.codegen.languages.PythonLegacyClientCodegen
 For more information, please visit [https://www.finbourne.com](https://www.finbourne.com)
 
 ## Requirements.
 
 Python 2.7 and 3.4+
```

### Comparing `lusid-workflow-sdk-preview-0.1.347/lusid_workflow/__init__.py` & `lusid-workflow-sdk-preview-0.1.348/lusid_workflow/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 # flake8: noqa
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.347
+    The version of the OpenAPI document: 0.1.348
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
-__version__ = "0.1.347"
+__version__ = "0.1.348"
 
 # import apis into sdk package
 from lusid_workflow.api.task_definitions_api import TaskDefinitionsApi
 from lusid_workflow.api.tasks_api import TasksApi
 from lusid_workflow.api.workers_api import WorkersApi
 
 # import ApiClient
```

### Comparing `lusid-workflow-sdk-preview-0.1.347/lusid_workflow/api/task_definitions_api.py` & `lusid-workflow-sdk-preview-0.1.348/lusid_workflow/api/task_definitions_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.347
+    The version of the OpenAPI document: 0.1.348
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -159,15 +159,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.347'
+        header_params['X-LUSID-SDK-Version'] = '0.1.348'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             201: "TaskDefinition",
             400: "LusidValidationProblemDetails",
@@ -328,15 +328,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.347'
+        header_params['X-LUSID-SDK-Version'] = '0.1.348'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "DeletedEntityResponse",
             400: "LusidValidationProblemDetails",
@@ -505,15 +505,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.347'
+        header_params['X-LUSID-SDK-Version'] = '0.1.348'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "TaskDefinition",
             400: "LusidValidationProblemDetails",
@@ -666,15 +666,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.347'
+        header_params['X-LUSID-SDK-Version'] = '0.1.348'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "PagedResourceListOfTaskDefinition",
             400: "LusidValidationProblemDetails",
@@ -843,15 +843,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.347'
+        header_params['X-LUSID-SDK-Version'] = '0.1.348'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "ResourceListOfTask",
             400: "LusidValidationProblemDetails",
@@ -1027,15 +1027,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.347'
+        header_params['X-LUSID-SDK-Version'] = '0.1.348'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "TaskDefinition",
             400: "LusidValidationProblemDetails",
```

### Comparing `lusid-workflow-sdk-preview-0.1.347/lusid_workflow/api/tasks_api.py` & `lusid-workflow-sdk-preview-0.1.348/lusid_workflow/api/tasks_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.347
+    The version of the OpenAPI document: 0.1.348
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -173,15 +173,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.347'
+        header_params['X-LUSID-SDK-Version'] = '0.1.348'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             201: "Task",
             400: "LusidValidationProblemDetails",
@@ -323,15 +323,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.347'
+        header_params['X-LUSID-SDK-Version'] = '0.1.348'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "DeletedEntityResponse",
             400: "LusidValidationProblemDetails",
@@ -481,15 +481,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.347'
+        header_params['X-LUSID-SDK-Version'] = '0.1.348'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "Task",
             400: "LusidValidationProblemDetails",
@@ -642,15 +642,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.347'
+        header_params['X-LUSID-SDK-Version'] = '0.1.348'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "PagedResourceListOfTask",
             400: "LusidValidationProblemDetails",
@@ -818,15 +818,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.347'
+        header_params['X-LUSID-SDK-Version'] = '0.1.348'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "Task",
             400: "LusidValidationProblemDetails",
```

### Comparing `lusid-workflow-sdk-preview-0.1.347/lusid_workflow/api/workers_api.py` & `lusid-workflow-sdk-preview-0.1.348/lusid_workflow/api/workers_api.py`

 * *Files identical despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.347
+    The version of the OpenAPI document: 0.1.348
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -160,15 +160,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.347'
+        header_params['X-LUSID-SDK-Version'] = '0.1.348'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             201: "Worker",
             400: "LusidValidationProblemDetails",
@@ -338,15 +338,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.347'
+        header_params['X-LUSID-SDK-Version'] = '0.1.348'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             201: "Worker",
             400: "LusidValidationProblemDetails",
@@ -498,15 +498,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.347'
+        header_params['X-LUSID-SDK-Version'] = '0.1.348'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             201: "PagedResourceListOfWorker",
             400: "LusidValidationProblemDetails",
@@ -688,15 +688,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.347'
+        header_params['X-LUSID-SDK-Version'] = '0.1.348'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "RunWorkerResponse",
             400: "LusidValidationProblemDetails",
```

### Comparing `lusid-workflow-sdk-preview-0.1.347/lusid_workflow/api_client.py` & `lusid-workflow-sdk-preview-0.1.348/lusid_workflow/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.347
+    The version of the OpenAPI document: 0.1.348
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 from __future__ import absolute_import
 
 import atexit
@@ -75,15 +75,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/0.1.347/python'
+        self.user_agent = 'OpenAPI-Generator/0.1.348/python'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `lusid-workflow-sdk-preview-0.1.347/lusid_workflow/configuration.py` & `lusid-workflow-sdk-preview-0.1.348/lusid_workflow/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.347
+    The version of the OpenAPI document: 0.1.348
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -392,16 +392,16 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 0.1.347\n"\
-               "SDK Package Version: 0.1.347".\
+               "Version of the API: 0.1.348\n"\
+               "SDK Package Version: 0.1.348".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `lusid-workflow-sdk-preview-0.1.347/lusid_workflow/exceptions.py` & `lusid-workflow-sdk-preview-0.1.348/lusid_workflow/exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.347
+    The version of the OpenAPI document: 0.1.348
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import six
```

### Comparing `lusid-workflow-sdk-preview-0.1.347/lusid_workflow/models/__init__.py` & `lusid-workflow-sdk-preview-0.1.348/lusid_workflow/models/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # flake8: noqa
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.347
+    The version of the OpenAPI document: 0.1.348
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `lusid-workflow-sdk-preview-0.1.347/lusid_workflow/models/action_definition.py` & `lusid-workflow-sdk-preview-0.1.348/lusid_workflow/models/action_definition.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.347
+    The version of the OpenAPI document: 0.1.348
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.347/lusid_workflow/models/action_details.py` & `lusid-workflow-sdk-preview-0.1.348/lusid_workflow/models/action_details.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.347
+    The version of the OpenAPI document: 0.1.348
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.347/lusid_workflow/models/create_child_tasks_action.py` & `lusid-workflow-sdk-preview-0.1.348/lusid_workflow/models/create_child_tasks_action.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.347
+    The version of the OpenAPI document: 0.1.348
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.347/lusid_workflow/models/create_task_definition_request.py` & `lusid-workflow-sdk-preview-0.1.348/lusid_workflow/models/create_task_definition_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.347
+    The version of the OpenAPI document: 0.1.348
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.347/lusid_workflow/models/create_task_request.py` & `lusid-workflow-sdk-preview-0.1.348/lusid_workflow/models/create_task_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.347
+    The version of the OpenAPI document: 0.1.348
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.347/lusid_workflow/models/create_worker_request.py` & `lusid-workflow-sdk-preview-0.1.348/lusid_workflow/models/create_worker_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.347
+    The version of the OpenAPI document: 0.1.348
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.347/lusid_workflow/models/deleted_entity_response.py` & `lusid-workflow-sdk-preview-0.1.348/lusid_workflow/models/deleted_entity_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.347
+    The version of the OpenAPI document: 0.1.348
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.347/lusid_workflow/models/field_mapping.py` & `lusid-workflow-sdk-preview-0.1.348/lusid_workflow/models/field_mapping.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.347
+    The version of the OpenAPI document: 0.1.348
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.347/lusid_workflow/models/health_check.py` & `lusid-workflow-sdk-preview-0.1.348/lusid_workflow/models/health_check.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.347
+    The version of the OpenAPI document: 0.1.348
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.347/lusid_workflow/models/initial_state.py` & `lusid-workflow-sdk-preview-0.1.348/lusid_workflow/models/initial_state.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.347
+    The version of the OpenAPI document: 0.1.348
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.347/lusid_workflow/models/link.py` & `lusid-workflow-sdk-preview-0.1.348/lusid_workflow/models/link.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.347
+    The version of the OpenAPI document: 0.1.348
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.347/lusid_workflow/models/luminesce_view.py` & `lusid-workflow-sdk-preview-0.1.348/lusid_workflow/models/luminesce_view.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.347
+    The version of the OpenAPI document: 0.1.348
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.347/lusid_workflow/models/lusid_problem_details.py` & `lusid-workflow-sdk-preview-0.1.348/lusid_workflow/models/lusid_problem_details.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.347
+    The version of the OpenAPI document: 0.1.348
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.347/lusid_workflow/models/lusid_validation_problem_details.py` & `lusid-workflow-sdk-preview-0.1.348/lusid_workflow/models/lusid_validation_problem_details.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.347
+    The version of the OpenAPI document: 0.1.348
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.347/lusid_workflow/models/paged_resource_list_of_task.py` & `lusid-workflow-sdk-preview-0.1.348/lusid_workflow/models/paged_resource_list_of_task.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.347
+    The version of the OpenAPI document: 0.1.348
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.347/lusid_workflow/models/paged_resource_list_of_task_definition.py` & `lusid-workflow-sdk-preview-0.1.348/lusid_workflow/models/paged_resource_list_of_task_definition.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.347
+    The version of the OpenAPI document: 0.1.348
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.347/lusid_workflow/models/paged_resource_list_of_worker.py` & `lusid-workflow-sdk-preview-0.1.348/lusid_workflow/models/paged_resource_list_of_worker.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.347
+    The version of the OpenAPI document: 0.1.348
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.347/lusid_workflow/models/parameter.py` & `lusid-workflow-sdk-preview-0.1.348/lusid_workflow/models/parameter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.347
+    The version of the OpenAPI document: 0.1.348
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.347/lusid_workflow/models/parameter_value.py` & `lusid-workflow-sdk-preview-0.1.348/lusid_workflow/models/parameter_value.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.347
+    The version of the OpenAPI document: 0.1.348
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.347/lusid_workflow/models/resource_id.py` & `lusid-workflow-sdk-preview-0.1.348/lusid_workflow/models/resource_id.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.347
+    The version of the OpenAPI document: 0.1.348
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.347/lusid_workflow/models/resource_list_of_task.py` & `lusid-workflow-sdk-preview-0.1.348/lusid_workflow/models/resource_list_of_task.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.347
+    The version of the OpenAPI document: 0.1.348
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.347/lusid_workflow/models/result_field.py` & `lusid-workflow-sdk-preview-0.1.348/lusid_workflow/models/result_field.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.347
+    The version of the OpenAPI document: 0.1.348
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.347/lusid_workflow/models/result_matching_pattern.py` & `lusid-workflow-sdk-preview-0.1.348/lusid_workflow/models/result_matching_pattern.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.347
+    The version of the OpenAPI document: 0.1.348
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.347/lusid_workflow/models/resultant_child_task_configuration.py` & `lusid-workflow-sdk-preview-0.1.348/lusid_workflow/models/resultant_child_task_configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.347
+    The version of the OpenAPI document: 0.1.348
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.347/lusid_workflow/models/run_worker_action.py` & `lusid-workflow-sdk-preview-0.1.348/lusid_workflow/models/run_worker_action.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.347
+    The version of the OpenAPI document: 0.1.348
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.347/lusid_workflow/models/run_worker_request.py` & `lusid-workflow-sdk-preview-0.1.348/lusid_workflow/models/run_worker_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.347
+    The version of the OpenAPI document: 0.1.348
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.347/lusid_workflow/models/run_worker_response.py` & `lusid-workflow-sdk-preview-0.1.348/lusid_workflow/models/run_worker_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.347
+    The version of the OpenAPI document: 0.1.348
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.347/lusid_workflow/models/task.py` & `lusid-workflow-sdk-preview-0.1.348/lusid_workflow/models/task.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.347
+    The version of the OpenAPI document: 0.1.348
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.347/lusid_workflow/models/task_definition.py` & `lusid-workflow-sdk-preview-0.1.348/lusid_workflow/models/task_definition.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.347
+    The version of the OpenAPI document: 0.1.348
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.347/lusid_workflow/models/task_definition_version.py` & `lusid-workflow-sdk-preview-0.1.348/lusid_workflow/models/task_definition_version.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.347
+    The version of the OpenAPI document: 0.1.348
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.347/lusid_workflow/models/task_field_definition.py` & `lusid-workflow-sdk-preview-0.1.348/lusid_workflow/models/task_field_definition.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.347
+    The version of the OpenAPI document: 0.1.348
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.347/lusid_workflow/models/task_instance_field.py` & `lusid-workflow-sdk-preview-0.1.348/lusid_workflow/models/task_instance_field.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.347
+    The version of the OpenAPI document: 0.1.348
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.347/lusid_workflow/models/task_state_definition.py` & `lusid-workflow-sdk-preview-0.1.348/lusid_workflow/models/task_state_definition.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.347
+    The version of the OpenAPI document: 0.1.348
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.347/lusid_workflow/models/task_transition_definition.py` & `lusid-workflow-sdk-preview-0.1.348/lusid_workflow/models/task_transition_definition.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.347
+    The version of the OpenAPI document: 0.1.348
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.347/lusid_workflow/models/transition_trigger_definition.py` & `lusid-workflow-sdk-preview-0.1.348/lusid_workflow/models/transition_trigger_definition.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.347
+    The version of the OpenAPI document: 0.1.348
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.347/lusid_workflow/models/trigger_parent_task_action.py` & `lusid-workflow-sdk-preview-0.1.348/lusid_workflow/models/trigger_parent_task_action.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.347
+    The version of the OpenAPI document: 0.1.348
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.347/lusid_workflow/models/trigger_schema.py` & `lusid-workflow-sdk-preview-0.1.348/lusid_workflow/models/trigger_schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.347
+    The version of the OpenAPI document: 0.1.348
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.347/lusid_workflow/models/update_task_definition_request.py` & `lusid-workflow-sdk-preview-0.1.348/lusid_workflow/models/update_task_definition_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.347
+    The version of the OpenAPI document: 0.1.348
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.347/lusid_workflow/models/update_task_request.py` & `lusid-workflow-sdk-preview-0.1.348/lusid_workflow/models/update_task_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.347
+    The version of the OpenAPI document: 0.1.348
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.347/lusid_workflow/models/version_info.py` & `lusid-workflow-sdk-preview-0.1.348/lusid_workflow/models/version_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.347
+    The version of the OpenAPI document: 0.1.348
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.347/lusid_workflow/models/worker.py` & `lusid-workflow-sdk-preview-0.1.348/lusid_workflow/models/worker.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.347
+    The version of the OpenAPI document: 0.1.348
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.347/lusid_workflow/models/worker_configuration.py` & `lusid-workflow-sdk-preview-0.1.348/lusid_workflow/models/worker_configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.347
+    The version of the OpenAPI document: 0.1.348
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.347/lusid_workflow/models/worker_status_triggers.py` & `lusid-workflow-sdk-preview-0.1.348/lusid_workflow/models/worker_status_triggers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.347
+    The version of the OpenAPI document: 0.1.348
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.347/lusid_workflow/rest.py` & `lusid-workflow-sdk-preview-0.1.348/lusid_workflow/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.347
+    The version of the OpenAPI document: 0.1.348
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `lusid-workflow-sdk-preview-0.1.347/lusid_workflow_sdk_preview.egg-info/SOURCES.txt` & `lusid-workflow-sdk-preview-0.1.348/lusid_workflow_sdk_preview.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lusid-workflow-sdk-preview-0.1.347/setup.py` & `lusid-workflow-sdk-preview-0.1.348/setup.py`

 * *Files identical despite different names*

